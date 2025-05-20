# Struct: <code>bpf_iter_reg</code>

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
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct bpf_iter_reg {
    const char *target;
    const struct seq_operations *seq_ops;
    bpf_iter_init_seq_priv_t init_seq_private;
    bpf_iter_fini_seq_priv_t fini_seq_private;
    u32 seq_priv_size;
    u32 ctx_arg_info_size;
    struct bpf_ctx_arg_aux ctx_arg_info[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct bpf_iter_reg {
    const char *target;
    bpf_iter_attach_target_t attach_target;
    bpf_iter_detach_target_t detach_target;
    bpf_iter_show_fdinfo_t show_fdinfo;
    bpf_iter_fill_link_info_t fill_link_info;
    u32 ctx_arg_info_size;
    u32 feature;
    struct bpf_ctx_arg_aux ctx_arg_info[2];
    const struct bpf_iter_seq_info *seq_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct bpf_iter_reg {
    const char *target;
    bpf_iter_attach_target_t attach_target;
    bpf_iter_detach_target_t detach_target;
    bpf_iter_show_fdinfo_t show_fdinfo;
    bpf_iter_fill_link_info_t fill_link_info;
    u32 ctx_arg_info_size;
    u32 feature;
    struct bpf_ctx_arg_aux ctx_arg_info[2];
    const struct bpf_iter_seq_info *seq_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct bpf_iter_reg {
    const char *target;
    bpf_iter_attach_target_t attach_target;
    bpf_iter_detach_target_t detach_target;
    bpf_iter_show_fdinfo_t show_fdinfo;
    bpf_iter_fill_link_info_t fill_link_info;
    bpf_iter_get_func_proto_t get_func_proto;
    u32 ctx_arg_info_size;
    u32 feature;
    struct bpf_ctx_arg_aux ctx_arg_info[2];
    const struct bpf_iter_seq_info *seq_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct bpf_iter_reg {
    const char *target;
    bpf_iter_attach_target_t attach_target;
    bpf_iter_detach_target_t detach_target;
    bpf_iter_show_fdinfo_t show_fdinfo;
    bpf_iter_fill_link_info_t fill_link_info;
    bpf_iter_get_func_proto_t get_func_proto;
    u32 ctx_arg_info_size;
    u32 feature;
    struct bpf_ctx_arg_aux ctx_arg_info[2];
    const struct bpf_iter_seq_info *seq_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct bpf_iter_reg {
    const char *target;
    bpf_iter_attach_target_t attach_target;
    bpf_iter_detach_target_t detach_target;
    bpf_iter_show_fdinfo_t show_fdinfo;
    bpf_iter_fill_link_info_t fill_link_info;
    bpf_iter_get_func_proto_t get_func_proto;
    u32 ctx_arg_info_size;
    u32 feature;
    struct bpf_ctx_arg_aux ctx_arg_info[2];
    const struct bpf_iter_seq_info *seq_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct bpf_iter_reg {
    const char *target;
    bpf_iter_attach_target_t attach_target;
    bpf_iter_detach_target_t detach_target;
    bpf_iter_show_fdinfo_t show_fdinfo;
    bpf_iter_fill_link_info_t fill_link_info;
    bpf_iter_get_func_proto_t get_func_proto;
    u32 ctx_arg_info_size;
    u32 feature;
    struct bpf_ctx_arg_aux ctx_arg_info[2];
    const struct bpf_iter_seq_info *seq_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct bpf_iter_reg {
    const char *target;
    bpf_iter_attach_target_t attach_target;
    bpf_iter_detach_target_t detach_target;
    bpf_iter_show_fdinfo_t show_fdinfo;
    bpf_iter_fill_link_info_t fill_link_info;
    bpf_iter_get_func_proto_t get_func_proto;
    u32 ctx_arg_info_size;
    u32 feature;
    struct bpf_ctx_arg_aux ctx_arg_info[2];
    const struct bpf_iter_seq_info *seq_info;
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
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bpf_iter_attach_target_t attach_target</code>
</li>
<li>
<b>Field added. </b>
<code>bpf_iter_detach_target_t detach_target</code>
</li>
<li>
<b>Field added. </b>
<code>bpf_iter_show_fdinfo_t show_fdinfo</code>
</li>
<li>
<b>Field added. </b>
<code>bpf_iter_fill_link_info_t fill_link_info</code>
</li>
<li>
<b>Field added. </b>
<code>u32 feature</code>
</li>
<li>
<b>Field added. </b>
<code>const struct bpf_iter_seq_info *seq_info</code>
</li>
<li>
<b>Field removed. </b>
<code>const struct seq_operations *seq_ops</code>
</li>
<li>
<b>Field removed. </b>
<code>bpf_iter_init_seq_priv_t init_seq_private</code>
</li>
<li>
<b>Field removed. </b>
<code>bpf_iter_fini_seq_priv_t fini_seq_private</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 seq_priv_size</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bpf_iter_get_func_proto_t get_func_proto</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
