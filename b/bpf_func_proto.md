# Struct: <code>bpf_func_proto</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct bpf_func_proto {
    u64 (*func)(u64, u64, u64, u64, u64);
    bool gpl_only;
    enum bpf_return_type ret_type;
    enum bpf_arg_type arg1_type;
    enum bpf_arg_type arg2_type;
    enum bpf_arg_type arg3_type;
    enum bpf_arg_type arg4_type;
    enum bpf_arg_type arg5_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct bpf_func_proto {
    u64 (*func)(u64, u64, u64, u64, u64);
    bool gpl_only;
    enum bpf_return_type ret_type;
    enum bpf_arg_type arg1_type;
    enum bpf_arg_type arg2_type;
    enum bpf_arg_type arg3_type;
    enum bpf_arg_type arg4_type;
    enum bpf_arg_type arg5_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct bpf_func_proto {
    u64 (*func)(u64, u64, u64, u64, u64);
    bool gpl_only;
    bool pkt_access;
    enum bpf_return_type ret_type;
    enum bpf_arg_type arg1_type;
    enum bpf_arg_type arg2_type;
    enum bpf_arg_type arg3_type;
    enum bpf_arg_type arg4_type;
    enum bpf_arg_type arg5_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct bpf_func_proto {
    u64 (*func)(u64, u64, u64, u64, u64);
    bool gpl_only;
    bool pkt_access;
    enum bpf_return_type ret_type;
    enum bpf_arg_type arg1_type;
    enum bpf_arg_type arg2_type;
    enum bpf_arg_type arg3_type;
    enum bpf_arg_type arg4_type;
    enum bpf_arg_type arg5_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct bpf_func_proto {
    u64 (*func)(u64, u64, u64, u64, u64);
    bool gpl_only;
    bool pkt_access;
    enum bpf_return_type ret_type;
    enum bpf_arg_type arg1_type;
    enum bpf_arg_type arg2_type;
    enum bpf_arg_type arg3_type;
    enum bpf_arg_type arg4_type;
    enum bpf_arg_type arg5_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct bpf_func_proto {
    u64 (*func)(u64, u64, u64, u64, u64);
    bool gpl_only;
    bool pkt_access;
    enum bpf_return_type ret_type;
    enum bpf_arg_type arg1_type;
    enum bpf_arg_type arg2_type;
    enum bpf_arg_type arg3_type;
    enum bpf_arg_type arg4_type;
    enum bpf_arg_type arg5_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct bpf_func_proto {
    u64 (*func)(u64, u64, u64, u64, u64);
    bool gpl_only;
    bool pkt_access;
    enum bpf_return_type ret_type;
    enum bpf_arg_type arg1_type;
    enum bpf_arg_type arg2_type;
    enum bpf_arg_type arg3_type;
    enum bpf_arg_type arg4_type;
    enum bpf_arg_type arg5_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct bpf_func_proto {
    u64 (*func)(u64, u64, u64, u64, u64);
    bool gpl_only;
    bool pkt_access;
    enum bpf_return_type ret_type;
    enum bpf_arg_type arg1_type;
    enum bpf_arg_type arg2_type;
    enum bpf_arg_type arg3_type;
    enum bpf_arg_type arg4_type;
    enum bpf_arg_type arg5_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct bpf_func_proto {
    u64 (*func)(u64, u64, u64, u64, u64);
    bool gpl_only;
    bool pkt_access;
    enum bpf_return_type ret_type;
    enum bpf_arg_type arg1_type;
    enum bpf_arg_type arg2_type;
    enum bpf_arg_type arg3_type;
    enum bpf_arg_type arg4_type;
    enum bpf_arg_type arg5_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct bpf_func_proto {
    u64 (*func)(u64, u64, u64, u64, u64);
    bool gpl_only;
    bool pkt_access;
    enum bpf_return_type ret_type;
    enum bpf_arg_type arg1_type;
    enum bpf_arg_type arg2_type;
    enum bpf_arg_type arg3_type;
    enum bpf_arg_type arg4_type;
    enum bpf_arg_type arg5_type;
    enum bpf_arg_type arg_type[5];
    int *btf_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct bpf_func_proto {
    u64 (*func)(u64, u64, u64, u64, u64);
    bool gpl_only;
    bool pkt_access;
    enum bpf_return_type ret_type;
    enum bpf_arg_type arg1_type;
    enum bpf_arg_type arg2_type;
    enum bpf_arg_type arg3_type;
    enum bpf_arg_type arg4_type;
    enum bpf_arg_type arg5_type;
    enum bpf_arg_type arg_type[5];
    u32 *arg1_btf_id;
    u32 *arg2_btf_id;
    u32 *arg3_btf_id;
    u32 *arg4_btf_id;
    u32 *arg5_btf_id;
    u32 * arg_btf_id[5];
    int *ret_btf_id;
    bool (*allowed)(const struct bpf_prog *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct bpf_func_proto {
    u64 (*func)(u64, u64, u64, u64, u64);
    bool gpl_only;
    bool pkt_access;
    enum bpf_return_type ret_type;
    enum bpf_arg_type arg1_type;
    enum bpf_arg_type arg2_type;
    enum bpf_arg_type arg3_type;
    enum bpf_arg_type arg4_type;
    enum bpf_arg_type arg5_type;
    enum bpf_arg_type arg_type[5];
    u32 *arg1_btf_id;
    u32 *arg2_btf_id;
    u32 *arg3_btf_id;
    u32 *arg4_btf_id;
    u32 *arg5_btf_id;
    u32 * arg_btf_id[5];
    int *ret_btf_id;
    bool (*allowed)(const struct bpf_prog *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct bpf_func_proto {
    u64 (*func)(u64, u64, u64, u64, u64);
    bool gpl_only;
    bool pkt_access;
    enum bpf_return_type ret_type;
    enum bpf_arg_type arg1_type;
    enum bpf_arg_type arg2_type;
    enum bpf_arg_type arg3_type;
    enum bpf_arg_type arg4_type;
    enum bpf_arg_type arg5_type;
    enum bpf_arg_type arg_type[5];
    u32 *arg1_btf_id;
    u32 *arg2_btf_id;
    u32 *arg3_btf_id;
    u32 *arg4_btf_id;
    u32 *arg5_btf_id;
    u32 * arg_btf_id[5];
    int *ret_btf_id;
    bool (*allowed)(const struct bpf_prog *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct bpf_func_proto {
    u64 (*func)(u64, u64, u64, u64, u64);
    bool gpl_only;
    bool pkt_access;
    enum bpf_return_type ret_type;
    enum bpf_arg_type arg1_type;
    enum bpf_arg_type arg2_type;
    enum bpf_arg_type arg3_type;
    enum bpf_arg_type arg4_type;
    enum bpf_arg_type arg5_type;
    enum bpf_arg_type arg_type[5];
    u32 *arg1_btf_id;
    u32 *arg2_btf_id;
    u32 *arg3_btf_id;
    u32 *arg4_btf_id;
    u32 *arg5_btf_id;
    u32 * arg_btf_id[5];
    int *ret_btf_id;
    bool (*allowed)(const struct bpf_prog *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct bpf_func_proto {
    u64 (*func)(u64, u64, u64, u64, u64);
    bool gpl_only;
    bool pkt_access;
    bool might_sleep;
    enum bpf_return_type ret_type;
    enum bpf_arg_type arg1_type;
    enum bpf_arg_type arg2_type;
    enum bpf_arg_type arg3_type;
    enum bpf_arg_type arg4_type;
    enum bpf_arg_type arg5_type;
    enum bpf_arg_type arg_type[5];
    u32 *arg1_btf_id;
    u32 *arg2_btf_id;
    u32 *arg3_btf_id;
    u32 *arg4_btf_id;
    u32 *arg5_btf_id;
    u32 * arg_btf_id[5];
    size_t arg1_size;
    size_t arg2_size;
    size_t arg3_size;
    size_t arg4_size;
    size_t arg5_size;
    size_t arg_size[5];
    int *ret_btf_id;
    bool (*allowed)(const struct bpf_prog *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct bpf_func_proto {
    u64 (*func)(u64, u64, u64, u64, u64);
    bool gpl_only;
    bool pkt_access;
    bool might_sleep;
    enum bpf_return_type ret_type;
    enum bpf_arg_type arg1_type;
    enum bpf_arg_type arg2_type;
    enum bpf_arg_type arg3_type;
    enum bpf_arg_type arg4_type;
    enum bpf_arg_type arg5_type;
    enum bpf_arg_type arg_type[5];
    u32 *arg1_btf_id;
    u32 *arg2_btf_id;
    u32 *arg3_btf_id;
    u32 *arg4_btf_id;
    u32 *arg5_btf_id;
    u32 * arg_btf_id[5];
    size_t arg1_size;
    size_t arg2_size;
    size_t arg3_size;
    size_t arg4_size;
    size_t arg5_size;
    size_t arg_size[5];
    int *ret_btf_id;
    bool (*allowed)(const struct bpf_prog *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct bpf_func_proto {
    u64 (*func)(u64, u64, u64, u64, u64);
    bool gpl_only;
    bool pkt_access;
    bool might_sleep;
    enum bpf_return_type ret_type;
    enum bpf_arg_type arg1_type;
    enum bpf_arg_type arg2_type;
    enum bpf_arg_type arg3_type;
    enum bpf_arg_type arg4_type;
    enum bpf_arg_type arg5_type;
    enum bpf_arg_type arg_type[5];
    u32 *arg1_btf_id;
    u32 *arg2_btf_id;
    u32 *arg3_btf_id;
    u32 *arg4_btf_id;
    u32 *arg5_btf_id;
    u32 * arg_btf_id[5];
    size_t arg1_size;
    size_t arg2_size;
    size_t arg3_size;
    size_t arg4_size;
    size_t arg5_size;
    size_t arg_size[5];
    int *ret_btf_id;
    bool (*allowed)(const struct bpf_prog *);
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
struct bpf_func_proto {
    u64 (*func)(u64, u64, u64, u64, u64);
    bool gpl_only;
    bool pkt_access;
    enum bpf_return_type ret_type;
    enum bpf_arg_type arg1_type;
    enum bpf_arg_type arg2_type;
    enum bpf_arg_type arg3_type;
    enum bpf_arg_type arg4_type;
    enum bpf_arg_type arg5_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct bpf_func_proto {
    u64 (*func)(u64, u64, u64, u64, u64);
    bool gpl_only;
    bool pkt_access;
    enum bpf_return_type ret_type;
    enum bpf_arg_type arg1_type;
    enum bpf_arg_type arg2_type;
    enum bpf_arg_type arg3_type;
    enum bpf_arg_type arg4_type;
    enum bpf_arg_type arg5_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct bpf_func_proto {
    u64 (*func)(u64, u64, u64, u64, u64);
    bool gpl_only;
    bool pkt_access;
    enum bpf_return_type ret_type;
    enum bpf_arg_type arg1_type;
    enum bpf_arg_type arg2_type;
    enum bpf_arg_type arg3_type;
    enum bpf_arg_type arg4_type;
    enum bpf_arg_type arg5_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct bpf_func_proto {
    u64 (*func)(u64, u64, u64, u64, u64);
    bool gpl_only;
    bool pkt_access;
    enum bpf_return_type ret_type;
    enum bpf_arg_type arg1_type;
    enum bpf_arg_type arg2_type;
    enum bpf_arg_type arg3_type;
    enum bpf_arg_type arg4_type;
    enum bpf_arg_type arg5_type;
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
struct bpf_func_proto {
    u64 (*func)(u64, u64, u64, u64, u64);
    bool gpl_only;
    bool pkt_access;
    enum bpf_return_type ret_type;
    enum bpf_arg_type arg1_type;
    enum bpf_arg_type arg2_type;
    enum bpf_arg_type arg3_type;
    enum bpf_arg_type arg4_type;
    enum bpf_arg_type arg5_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct bpf_func_proto {
    u64 (*func)(u64, u64, u64, u64, u64);
    bool gpl_only;
    bool pkt_access;
    enum bpf_return_type ret_type;
    enum bpf_arg_type arg1_type;
    enum bpf_arg_type arg2_type;
    enum bpf_arg_type arg3_type;
    enum bpf_arg_type arg4_type;
    enum bpf_arg_type arg5_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct bpf_func_proto {
    u64 (*func)(u64, u64, u64, u64, u64);
    bool gpl_only;
    bool pkt_access;
    enum bpf_return_type ret_type;
    enum bpf_arg_type arg1_type;
    enum bpf_arg_type arg2_type;
    enum bpf_arg_type arg3_type;
    enum bpf_arg_type arg4_type;
    enum bpf_arg_type arg5_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct bpf_func_proto {
    u64 (*func)(u64, u64, u64, u64, u64);
    bool gpl_only;
    bool pkt_access;
    enum bpf_return_type ret_type;
    enum bpf_arg_type arg1_type;
    enum bpf_arg_type arg2_type;
    enum bpf_arg_type arg3_type;
    enum bpf_arg_type arg4_type;
    enum bpf_arg_type arg5_type;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.4</code> and <code>4.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool pkt_access</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
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
<code>enum bpf_arg_type arg_type[5]</code>
</li>
<li>
<b>Field added. </b>
<code>int *btf_id</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 *arg1_btf_id</code>
</li>
<li>
<b>Field added. </b>
<code>u32 *arg2_btf_id</code>
</li>
<li>
<b>Field added. </b>
<code>u32 *arg3_btf_id</code>
</li>
<li>
<b>Field added. </b>
<code>u32 *arg4_btf_id</code>
</li>
<li>
<b>Field added. </b>
<code>u32 *arg5_btf_id</code>
</li>
<li>
<b>Field added. </b>
<code>u32 * arg_btf_id[5]</code>
</li>
<li>
<b>Field added. </b>
<code>int *ret_btf_id</code>
</li>
<li>
<b>Field added. </b>
<code>bool (*allowed)(const struct bpf_prog *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int *btf_id</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool might_sleep</code>
</li>
<li>
<b>Field added. </b>
<code>size_t arg1_size</code>
</li>
<li>
<b>Field added. </b>
<code>size_t arg2_size</code>
</li>
<li>
<b>Field added. </b>
<code>size_t arg3_size</code>
</li>
<li>
<b>Field added. </b>
<code>size_t arg4_size</code>
</li>
<li>
<b>Field added. </b>
<code>size_t arg5_size</code>
</li>
<li>
<b>Field added. </b>
<code>size_t arg_size[5]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
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
