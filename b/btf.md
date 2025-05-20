# Struct: <code>btf</code>

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
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct btf {
    void *data;
    struct btf_type **types;
    u32 *resolved_ids;
    u32 *resolved_sizes;
    const char *strings;
    void *nohdr_data;
    struct btf_header hdr;
    u32 nr_types;
    u32 types_size;
    u32 data_size;
    refcount_t refcnt;
    u32 id;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct btf {
    void *data;
    struct btf_type **types;
    u32 *resolved_ids;
    u32 *resolved_sizes;
    const char *strings;
    void *nohdr_data;
    struct btf_header hdr;
    u32 nr_types;
    u32 types_size;
    u32 data_size;
    refcount_t refcnt;
    u32 id;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct btf {
    void *data;
    struct btf_type **types;
    u32 *resolved_ids;
    u32 *resolved_sizes;
    const char *strings;
    void *nohdr_data;
    struct btf_header hdr;
    u32 nr_types;
    u32 types_size;
    u32 data_size;
    refcount_t refcnt;
    u32 id;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct btf {
    void *data;
    struct btf_type **types;
    u32 *resolved_ids;
    u32 *resolved_sizes;
    const char *strings;
    void *nohdr_data;
    struct btf_header hdr;
    u32 nr_types;
    u32 types_size;
    u32 data_size;
    refcount_t refcnt;
    u32 id;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct btf {
    void *data;
    struct btf_type **types;
    u32 *resolved_ids;
    u32 *resolved_sizes;
    const char *strings;
    void *nohdr_data;
    struct btf_header hdr;
    u32 nr_types;
    u32 types_size;
    u32 data_size;
    refcount_t refcnt;
    u32 id;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct btf {
    void *data;
    struct btf_type **types;
    u32 *resolved_ids;
    u32 *resolved_sizes;
    const char *strings;
    void *nohdr_data;
    struct btf_header hdr;
    u32 nr_types;
    u32 types_size;
    u32 data_size;
    refcount_t refcnt;
    u32 id;
    struct callback_head rcu;
    struct btf *base_btf;
    u32 start_id;
    u32 start_str_off;
    char name[56];
    bool kernel_btf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct btf {
    void *data;
    struct btf_type **types;
    u32 *resolved_ids;
    u32 *resolved_sizes;
    const char *strings;
    void *nohdr_data;
    struct btf_header hdr;
    u32 nr_types;
    u32 types_size;
    u32 data_size;
    refcount_t refcnt;
    u32 id;
    struct callback_head rcu;
    struct btf *base_btf;
    u32 start_id;
    u32 start_str_off;
    char name[56];
    bool kernel_btf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct btf {
    void *data;
    struct btf_type **types;
    u32 *resolved_ids;
    u32 *resolved_sizes;
    const char *strings;
    void *nohdr_data;
    struct btf_header hdr;
    u32 nr_types;
    u32 types_size;
    u32 data_size;
    refcount_t refcnt;
    u32 id;
    struct callback_head rcu;
    struct btf *base_btf;
    u32 start_id;
    u32 start_str_off;
    char name[56];
    bool kernel_btf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct btf {
    void *data;
    struct btf_type **types;
    u32 *resolved_ids;
    u32 *resolved_sizes;
    const char *strings;
    void *nohdr_data;
    struct btf_header hdr;
    u32 nr_types;
    u32 types_size;
    u32 data_size;
    refcount_t refcnt;
    u32 id;
    struct callback_head rcu;
    struct btf_kfunc_set_tab *kfunc_set_tab;
    struct btf_id_dtor_kfunc_tab *dtor_kfunc_tab;
    struct btf *base_btf;
    u32 start_id;
    u32 start_str_off;
    char name[56];
    bool kernel_btf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct btf {
    void *data;
    struct btf_type **types;
    u32 *resolved_ids;
    u32 *resolved_sizes;
    const char *strings;
    void *nohdr_data;
    struct btf_header hdr;
    u32 nr_types;
    u32 types_size;
    u32 data_size;
    refcount_t refcnt;
    u32 id;
    struct callback_head rcu;
    struct btf_kfunc_set_tab *kfunc_set_tab;
    struct btf_id_dtor_kfunc_tab *dtor_kfunc_tab;
    struct btf_struct_metas *struct_meta_tab;
    struct btf *base_btf;
    u32 start_id;
    u32 start_str_off;
    char name[56];
    bool kernel_btf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct btf {
    void *data;
    struct btf_type **types;
    u32 *resolved_ids;
    u32 *resolved_sizes;
    const char *strings;
    void *nohdr_data;
    struct btf_header hdr;
    u32 nr_types;
    u32 types_size;
    u32 data_size;
    refcount_t refcnt;
    u32 id;
    struct callback_head rcu;
    struct btf_kfunc_set_tab *kfunc_set_tab;
    struct btf_id_dtor_kfunc_tab *dtor_kfunc_tab;
    struct btf_struct_metas *struct_meta_tab;
    struct btf *base_btf;
    u32 start_id;
    u32 start_str_off;
    char name[56];
    bool kernel_btf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct btf {
    void *data;
    struct btf_type **types;
    u32 *resolved_ids;
    u32 *resolved_sizes;
    const char *strings;
    void *nohdr_data;
    struct btf_header hdr;
    u32 nr_types;
    u32 types_size;
    u32 data_size;
    refcount_t refcnt;
    u32 id;
    struct callback_head rcu;
    struct btf_kfunc_set_tab *kfunc_set_tab;
    struct btf_id_dtor_kfunc_tab *dtor_kfunc_tab;
    struct btf_struct_metas *struct_meta_tab;
    struct btf *base_btf;
    u32 start_id;
    u32 start_str_off;
    char name[56];
    bool kernel_btf;
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
struct btf {
    void *data;
    struct btf_type **types;
    u32 *resolved_ids;
    u32 *resolved_sizes;
    const char *strings;
    void *nohdr_data;
    struct btf_header hdr;
    u32 nr_types;
    u32 types_size;
    u32 data_size;
    refcount_t refcnt;
    u32 id;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct btf {
    void *data;
    struct btf_type **types;
    u32 *resolved_ids;
    u32 *resolved_sizes;
    const char *strings;
    void *nohdr_data;
    struct btf_header hdr;
    u32 nr_types;
    u32 types_size;
    u32 data_size;
    refcount_t refcnt;
    u32 id;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct btf {
    void *data;
    struct btf_type **types;
    u32 *resolved_ids;
    u32 *resolved_sizes;
    const char *strings;
    void *nohdr_data;
    struct btf_header hdr;
    u32 nr_types;
    u32 types_size;
    u32 data_size;
    refcount_t refcnt;
    u32 id;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct btf {
    void *data;
    struct btf_type **types;
    u32 *resolved_ids;
    u32 *resolved_sizes;
    const char *strings;
    void *nohdr_data;
    struct btf_header hdr;
    u32 nr_types;
    u32 types_size;
    u32 data_size;
    refcount_t refcnt;
    u32 id;
    struct callback_head rcu;
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
struct btf {
    void *data;
    struct btf_type **types;
    u32 *resolved_ids;
    u32 *resolved_sizes;
    const char *strings;
    void *nohdr_data;
    struct btf_header hdr;
    u32 nr_types;
    u32 types_size;
    u32 data_size;
    refcount_t refcnt;
    u32 id;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct btf {
    void *data;
    struct btf_type **types;
    u32 *resolved_ids;
    u32 *resolved_sizes;
    const char *strings;
    void *nohdr_data;
    struct btf_header hdr;
    u32 nr_types;
    u32 types_size;
    u32 data_size;
    refcount_t refcnt;
    u32 id;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct btf {
    void *data;
    struct btf_type **types;
    u32 *resolved_ids;
    u32 *resolved_sizes;
    const char *strings;
    void *nohdr_data;
    struct btf_header hdr;
    u32 nr_types;
    u32 types_size;
    u32 data_size;
    refcount_t refcnt;
    u32 id;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct btf {
    void *data;
    struct btf_type **types;
    u32 *resolved_ids;
    u32 *resolved_sizes;
    const char *strings;
    void *nohdr_data;
    struct btf_header hdr;
    u32 nr_types;
    u32 types_size;
    u32 data_size;
    refcount_t refcnt;
    u32 id;
    struct callback_head rcu;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct btf *base_btf</code>
</li>
<li>
<b>Field added. </b>
<code>u32 start_id</code>
</li>
<li>
<b>Field added. </b>
<code>u32 start_str_off</code>
</li>
<li>
<b>Field added. </b>
<code>char name[56]</code>
</li>
<li>
<b>Field added. </b>
<code>bool kernel_btf</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct btf_kfunc_set_tab *kfunc_set_tab</code>
</li>
<li>
<b>Field added. </b>
<code>struct btf_id_dtor_kfunc_tab *dtor_kfunc_tab</code>
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
<code>struct btf_struct_metas *struct_meta_tab</code>
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
