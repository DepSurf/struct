# Struct: <code>bpf_array</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct bpf_array {
    struct bpf_map map;
    u32 elem_size;
    enum bpf_prog_type owner_prog_type;
    bool owner_jited;
    char value[0];
    void * ptrs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct bpf_array {
    struct bpf_map map;
    u32 elem_size;
    enum bpf_prog_type owner_prog_type;
    bool owner_jited;
    char value[0];
    void * ptrs[0];
    void * pptrs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct bpf_array {
    struct bpf_map map;
    u32 elem_size;
    enum bpf_prog_type owner_prog_type;
    bool owner_jited;
    char value[0];
    void * ptrs[0];
    void * pptrs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct bpf_array {
    struct bpf_map map;
    u32 elem_size;
    enum bpf_prog_type owner_prog_type;
    bool owner_jited;
    char value[0];
    void * ptrs[0];
    void * pptrs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct bpf_array {
    struct bpf_map map;
    u32 elem_size;
    u32 index_mask;
    enum bpf_prog_type owner_prog_type;
    bool owner_jited;
    char value[0];
    void * ptrs[0];
    void * pptrs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct bpf_array {
    struct bpf_map map;
    u32 elem_size;
    u32 index_mask;
    enum bpf_prog_type owner_prog_type;
    bool owner_jited;
    char value[0];
    void * ptrs[0];
    void * pptrs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct bpf_array {
    struct bpf_map map;
    u32 elem_size;
    u32 index_mask;
    enum bpf_prog_type owner_prog_type;
    bool owner_jited;
    char value[0];
    void * ptrs[0];
    void * pptrs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct bpf_array {
    struct bpf_map map;
    u32 elem_size;
    u32 index_mask;
    enum bpf_prog_type owner_prog_type;
    bool owner_jited;
    char value[0];
    void * ptrs[0];
    void * pptrs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct bpf_array {
    struct bpf_map map;
    u32 elem_size;
    u32 index_mask;
    enum bpf_prog_type owner_prog_type;
    bool owner_jited;
    char value[0];
    void * ptrs[0];
    void * pptrs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct bpf_array {
    struct bpf_map map;
    u32 elem_size;
    u32 index_mask;
    struct bpf_array_aux *aux;
    char value[0];
    void * ptrs[0];
    void * pptrs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct bpf_array {
    struct bpf_map map;
    u32 elem_size;
    u32 index_mask;
    struct bpf_array_aux *aux;
    char value[0];
    void * ptrs[0];
    void * pptrs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct bpf_array {
    struct bpf_map map;
    u32 elem_size;
    u32 index_mask;
    struct bpf_array_aux *aux;
    char value[0];
    void * ptrs[0];
    void * pptrs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct bpf_array {
    struct bpf_map map;
    u32 elem_size;
    u32 index_mask;
    struct bpf_array_aux *aux;
    char value[0];
    void * ptrs[0];
    void * pptrs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct bpf_array {
    struct bpf_map map;
    u32 elem_size;
    u32 index_mask;
    struct bpf_array_aux *aux;
    char value[0];
    void * ptrs[0];
    void * pptrs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct bpf_array {
    struct bpf_map map;
    u32 elem_size;
    u32 index_mask;
    struct bpf_array_aux *aux;
    char value[0];
    void * ptrs[0];
    void * pptrs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct bpf_array {
    struct bpf_map map;
    u32 elem_size;
    u32 index_mask;
    struct bpf_array_aux *aux;
    struct (anon) __empty_value;
    char value[0];
    struct (anon) __empty_ptrs;
    void * ptrs[0];
    struct (anon) __empty_pptrs;
    void * pptrs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct bpf_array {
    struct bpf_map map;
    u32 elem_size;
    u32 index_mask;
    struct bpf_array_aux *aux;
    struct (anon) __empty_value;
    char value[0];
    struct (anon) __empty_ptrs;
    void * ptrs[0];
    struct (anon) __empty_pptrs;
    void * pptrs[0];
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct bpf_array {
    struct bpf_map map;
    u32 elem_size;
    u32 index_mask;
    enum bpf_prog_type owner_prog_type;
    bool owner_jited;
    char value[0];
    void * ptrs[0];
    void * pptrs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct bpf_array {
    struct bpf_map map;
    u32 elem_size;
    u32 index_mask;
    enum bpf_prog_type owner_prog_type;
    bool owner_jited;
    char value[0];
    void * ptrs[0];
    void * pptrs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct bpf_array {
    struct bpf_map map;
    u32 elem_size;
    u32 index_mask;
    enum bpf_prog_type owner_prog_type;
    bool owner_jited;
    char value[0];
    void * ptrs[0];
    void * pptrs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct bpf_array {
    struct bpf_map map;
    u32 elem_size;
    u32 index_mask;
    enum bpf_prog_type owner_prog_type;
    bool owner_jited;
    char value[0];
    void * ptrs[0];
    void * pptrs[0];
};
```
</details>
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct bpf_array {
    struct bpf_map map;
    u32 elem_size;
    u32 index_mask;
    enum bpf_prog_type owner_prog_type;
    bool owner_jited;
    char value[0];
    void * ptrs[0];
    void * pptrs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct bpf_array {
    struct bpf_map map;
    u32 elem_size;
    u32 index_mask;
    enum bpf_prog_type owner_prog_type;
    bool owner_jited;
    char value[0];
    void * ptrs[0];
    void * pptrs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct bpf_array {
    struct bpf_map map;
    u32 elem_size;
    u32 index_mask;
    enum bpf_prog_type owner_prog_type;
    bool owner_jited;
    char value[0];
    void * ptrs[0];
    void * pptrs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct bpf_array {
    struct bpf_map map;
    u32 elem_size;
    u32 index_mask;
    enum bpf_prog_type owner_prog_type;
    bool owner_jited;
    char value[0];
    void * ptrs[0];
    void * pptrs[0];
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void * pptrs[0]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 index_mask</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct bpf_array_aux *aux</code>
</li>
<li>
<b>Field removed. </b>
<code>enum bpf_prog_type owner_prog_type</code>
</li>
<li>
<b>Field removed. </b>
<code>bool owner_jited</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct (anon) __empty_value</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) __empty_ptrs</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) __empty_pptrs</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
<b>Arch</b>
<ul>
<li>
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>armhf</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>riscv64</code> ✅
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
No changes between <code>generic</code> and <code>aws</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
