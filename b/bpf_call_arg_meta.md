# Struct: <code>bpf_call_arg_meta</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct bpf_call_arg_meta {
    struct bpf_map *map_ptr;
    bool raw_mode;
    int regno;
    int access_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct bpf_call_arg_meta {
    struct bpf_map *map_ptr;
    bool raw_mode;
    bool pkt_access;
    int regno;
    int access_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct bpf_call_arg_meta {
    struct bpf_map *map_ptr;
    bool raw_mode;
    bool pkt_access;
    int regno;
    int access_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct bpf_call_arg_meta {
    struct bpf_map *map_ptr;
    bool raw_mode;
    bool pkt_access;
    int regno;
    int access_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct bpf_call_arg_meta {
    struct bpf_map *map_ptr;
    bool raw_mode;
    bool pkt_access;
    int regno;
    int access_size;
    s64 msize_smax_value;
    u64 msize_umax_value;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct bpf_call_arg_meta {
    struct bpf_map *map_ptr;
    bool raw_mode;
    bool pkt_access;
    int regno;
    int access_size;
    s64 msize_smax_value;
    u64 msize_umax_value;
    int ptr_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct bpf_call_arg_meta {
    struct bpf_map *map_ptr;
    bool raw_mode;
    bool pkt_access;
    int regno;
    int access_size;
    s64 msize_smax_value;
    u64 msize_umax_value;
    int ref_obj_id;
    int func_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct bpf_call_arg_meta {
    struct bpf_map *map_ptr;
    bool raw_mode;
    bool pkt_access;
    int regno;
    int access_size;
    s64 msize_smax_value;
    u64 msize_umax_value;
    int ref_obj_id;
    int func_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct bpf_call_arg_meta {
    struct bpf_map *map_ptr;
    bool raw_mode;
    bool pkt_access;
    int regno;
    int access_size;
    int mem_size;
    u64 msize_max_value;
    int ref_obj_id;
    int func_id;
    u32 btf_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct bpf_call_arg_meta {
    struct bpf_map *map_ptr;
    bool raw_mode;
    bool pkt_access;
    int regno;
    int access_size;
    int mem_size;
    u64 msize_max_value;
    int ref_obj_id;
    int func_id;
    struct btf *btf;
    u32 btf_id;
    struct btf *ret_btf;
    u32 ret_btf_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct bpf_call_arg_meta {
    struct bpf_map *map_ptr;
    bool raw_mode;
    bool pkt_access;
    int regno;
    int access_size;
    int mem_size;
    u64 msize_max_value;
    int ref_obj_id;
    int func_id;
    struct btf *btf;
    u32 btf_id;
    struct btf *ret_btf;
    u32 ret_btf_id;
    u32 subprogno;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct bpf_call_arg_meta {
    struct bpf_map *map_ptr;
    bool raw_mode;
    bool pkt_access;
    int regno;
    int access_size;
    int mem_size;
    u64 msize_max_value;
    int ref_obj_id;
    int map_uid;
    int func_id;
    struct btf *btf;
    u32 btf_id;
    struct btf *ret_btf;
    u32 ret_btf_id;
    u32 subprogno;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct bpf_call_arg_meta {
    struct bpf_map *map_ptr;
    bool raw_mode;
    bool pkt_access;
    u8 release_regno;
    int regno;
    int access_size;
    int mem_size;
    u64 msize_max_value;
    int ref_obj_id;
    int map_uid;
    int func_id;
    struct btf *btf;
    u32 btf_id;
    struct btf *ret_btf;
    u32 ret_btf_id;
    u32 subprogno;
    struct bpf_map_value_off_desc *kptr_off_desc;
    u8 uninit_dynptr_regno;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct bpf_call_arg_meta {
    struct bpf_map *map_ptr;
    bool raw_mode;
    bool pkt_access;
    u8 release_regno;
    int regno;
    int access_size;
    int mem_size;
    u64 msize_max_value;
    int ref_obj_id;
    int map_uid;
    int func_id;
    struct btf *btf;
    u32 btf_id;
    struct btf *ret_btf;
    u32 ret_btf_id;
    u32 subprogno;
    struct btf_field *kptr_field;
    u8 uninit_dynptr_regno;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct bpf_call_arg_meta {
    struct bpf_map *map_ptr;
    bool raw_mode;
    bool pkt_access;
    u8 release_regno;
    int regno;
    int access_size;
    int mem_size;
    u64 msize_max_value;
    int ref_obj_id;
    int dynptr_id;
    int map_uid;
    int func_id;
    struct btf *btf;
    u32 btf_id;
    struct btf *ret_btf;
    u32 ret_btf_id;
    u32 subprogno;
    struct btf_field *kptr_field;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct bpf_call_arg_meta {
    struct bpf_map *map_ptr;
    bool raw_mode;
    bool pkt_access;
    u8 release_regno;
    int regno;
    int access_size;
    int mem_size;
    u64 msize_max_value;
    int ref_obj_id;
    int dynptr_id;
    int map_uid;
    int func_id;
    struct btf *btf;
    u32 btf_id;
    struct btf *ret_btf;
    u32 ret_btf_id;
    u32 subprogno;
    struct btf_field *kptr_field;
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
struct bpf_call_arg_meta {
    struct bpf_map *map_ptr;
    bool raw_mode;
    bool pkt_access;
    int regno;
    int access_size;
    s64 msize_smax_value;
    u64 msize_umax_value;
    int ref_obj_id;
    int func_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct bpf_call_arg_meta {
    struct bpf_map *map_ptr;
    bool raw_mode;
    bool pkt_access;
    int regno;
    int access_size;
    s64 msize_smax_value;
    u64 msize_umax_value;
    int ref_obj_id;
    int func_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct bpf_call_arg_meta {
    struct bpf_map *map_ptr;
    bool raw_mode;
    bool pkt_access;
    int regno;
    int access_size;
    s64 msize_smax_value;
    u64 msize_umax_value;
    int ref_obj_id;
    int func_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct bpf_call_arg_meta {
    struct bpf_map *map_ptr;
    bool raw_mode;
    bool pkt_access;
    int regno;
    int access_size;
    s64 msize_smax_value;
    u64 msize_umax_value;
    int ref_obj_id;
    int func_id;
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
struct bpf_call_arg_meta {
    struct bpf_map *map_ptr;
    bool raw_mode;
    bool pkt_access;
    int regno;
    int access_size;
    s64 msize_smax_value;
    u64 msize_umax_value;
    int ref_obj_id;
    int func_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct bpf_call_arg_meta {
    struct bpf_map *map_ptr;
    bool raw_mode;
    bool pkt_access;
    int regno;
    int access_size;
    s64 msize_smax_value;
    u64 msize_umax_value;
    int ref_obj_id;
    int func_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct bpf_call_arg_meta {
    struct bpf_map *map_ptr;
    bool raw_mode;
    bool pkt_access;
    int regno;
    int access_size;
    s64 msize_smax_value;
    u64 msize_umax_value;
    int ref_obj_id;
    int func_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct bpf_call_arg_meta {
    struct bpf_map *map_ptr;
    bool raw_mode;
    bool pkt_access;
    int regno;
    int access_size;
    s64 msize_smax_value;
    u64 msize_umax_value;
    int ref_obj_id;
    int func_id;
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
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>s64 msize_smax_value</code>
</li>
<li>
<b>Field added. </b>
<code>u64 msize_umax_value</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int ptr_id</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int ref_obj_id</code>
</li>
<li>
<b>Field added. </b>
<code>int func_id</code>
</li>
<li>
<b>Field removed. </b>
<code>int ptr_id</code>
</li>
</ul>
</details>
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
<code>int mem_size</code>
</li>
<li>
<b>Field added. </b>
<code>u64 msize_max_value</code>
</li>
<li>
<b>Field added. </b>
<code>u32 btf_id</code>
</li>
<li>
<b>Field removed. </b>
<code>s64 msize_smax_value</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 msize_umax_value</code>
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
<code>struct btf *btf</code>
</li>
<li>
<b>Field added. </b>
<code>struct btf *ret_btf</code>
</li>
<li>
<b>Field added. </b>
<code>u32 ret_btf_id</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 subprogno</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int map_uid</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 release_regno</code>
</li>
<li>
<b>Field added. </b>
<code>struct bpf_map_value_off_desc *kptr_off_desc</code>
</li>
<li>
<b>Field added. </b>
<code>u8 uninit_dynptr_regno</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct btf_field *kptr_field</code>
</li>
<li>
<b>Field removed. </b>
<code>struct bpf_map_value_off_desc *kptr_off_desc</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int dynptr_id</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 uninit_dynptr_regno</code>
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
