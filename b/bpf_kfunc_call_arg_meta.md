# Struct: <code>bpf_kfunc_call_arg_meta</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
In <code>4.8</code>: Absent ⚠️
</li>
<li>
In <code>4.10</code>: Absent ⚠️
</li>
<li>
In <code>4.13</code>: Absent ⚠️
</li>
<li>
In <code>4.15</code>: Absent ⚠️
</li>
<li>
In <code>4.18</code>: Absent ⚠️
</li>
<li>
In <code>5.0</code>: Absent ⚠️
</li>
<li>
In <code>5.3</code>: Absent ⚠️
</li>
<li>
In <code>5.4</code>: Absent ⚠️
</li>
<li>
In <code>5.8</code>: Absent ⚠️
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
In <code>5.19</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct bpf_kfunc_call_arg_meta {
    struct btf *btf;
    u32 func_id;
    u32 kfunc_flags;
    const struct btf_type *func_proto;
    const char *func_name;
    u32 ref_obj_id;
    u8 release_regno;
    bool r0_rdonly;
    u32 ret_btf_id;
    u64 r0_size;
    struct (anon) arg_constant;
    struct (anon) arg_obj_drop;
    struct (anon) arg_list_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct bpf_kfunc_call_arg_meta {
    struct btf *btf;
    u32 func_id;
    u32 kfunc_flags;
    const struct btf_type *func_proto;
    const char *func_name;
    u32 ref_obj_id;
    u8 release_regno;
    bool r0_rdonly;
    u32 ret_btf_id;
    u64 r0_size;
    u32 subprogno;
    struct (anon) arg_constant;
    struct btf *arg_btf;
    u32 arg_btf_id;
    bool arg_owning_ref;
    struct (anon) arg_list_head;
    struct (anon) arg_rbtree_root;
    struct (anon) initialized_dynptr;
    struct (anon) iter;
    u64 mem_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct bpf_kfunc_call_arg_meta {
    struct btf *btf;
    u32 func_id;
    u32 kfunc_flags;
    const struct btf_type *func_proto;
    const char *func_name;
    u32 ref_obj_id;
    u8 release_regno;
    bool r0_rdonly;
    u32 ret_btf_id;
    u64 r0_size;
    u32 subprogno;
    struct (anon) arg_constant;
    struct btf *arg_btf;
    u32 arg_btf_id;
    bool arg_owning_ref;
    struct (anon) arg_list_head;
    struct (anon) arg_rbtree_root;
    struct (anon) initialized_dynptr;
    struct (anon) iter;
    u64 mem_size;
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
In <code>arm64</code>: Absent ⚠️
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
</li>
<li>
In <code>riscv64</code>: Absent ⚠️
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
In <code>aws</code>: Absent ⚠️
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 subprogno</code>
</li>
<li>
<b>Field added. </b>
<code>struct btf *arg_btf</code>
</li>
<li>
<b>Field added. </b>
<code>u32 arg_btf_id</code>
</li>
<li>
<b>Field added. </b>
<code>bool arg_owning_ref</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) arg_rbtree_root</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) initialized_dynptr</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) iter</code>
</li>
<li>
<b>Field added. </b>
<code>u64 mem_size</code>
</li>
<li>
<b>Field removed. </b>
<code>struct (anon) arg_obj_drop</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
