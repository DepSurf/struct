# Struct: <code>rproc_ops</code>

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
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rproc_ops {
    int (*start)(struct rproc *);
    int (*stop)(struct rproc *);
    void (*kick)(struct rproc *, int);
    void * (*da_to_va)(struct rproc *, u64, int);
    int (*parse_fw)(struct rproc *, const struct firmware *);
    int (*handle_rsc)(struct rproc *, u32, void *, int, int);
    struct resource_table * (*find_loaded_rsc_table)(struct rproc *, const struct firmware *);
    int (*load)(struct rproc *, const struct firmware *);
    int (*sanity_check)(struct rproc *, const struct firmware *);
    u32 (*get_boot_addr)(struct rproc *, const struct firmware *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct rproc_ops {
    int (*prepare)(struct rproc *);
    int (*unprepare)(struct rproc *);
    int (*start)(struct rproc *);
    int (*stop)(struct rproc *);
    void (*kick)(struct rproc *, int);
    void * (*da_to_va)(struct rproc *, u64, size_t);
    int (*parse_fw)(struct rproc *, const struct firmware *);
    int (*handle_rsc)(struct rproc *, u32, void *, int, int);
    struct resource_table * (*find_loaded_rsc_table)(struct rproc *, const struct firmware *);
    int (*load)(struct rproc *, const struct firmware *);
    int (*sanity_check)(struct rproc *, const struct firmware *);
    u64 (*get_boot_addr)(struct rproc *, const struct firmware *);
    long unsigned int (*panic)(struct rproc *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct rproc_ops {
    int (*prepare)(struct rproc *);
    int (*unprepare)(struct rproc *);
    int (*start)(struct rproc *);
    int (*stop)(struct rproc *);
    int (*attach)(struct rproc *);
    void (*kick)(struct rproc *, int);
    void * (*da_to_va)(struct rproc *, u64, size_t);
    int (*parse_fw)(struct rproc *, const struct firmware *);
    int (*handle_rsc)(struct rproc *, u32, void *, int, int);
    struct resource_table * (*find_loaded_rsc_table)(struct rproc *, const struct firmware *);
    int (*load)(struct rproc *, const struct firmware *);
    int (*sanity_check)(struct rproc *, const struct firmware *);
    u64 (*get_boot_addr)(struct rproc *, const struct firmware *);
    long unsigned int (*panic)(struct rproc *);
    void (*coredump)(struct rproc *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rproc_ops {
    int (*prepare)(struct rproc *);
    int (*unprepare)(struct rproc *);
    int (*start)(struct rproc *);
    int (*stop)(struct rproc *);
    int (*attach)(struct rproc *);
    int (*detach)(struct rproc *);
    void (*kick)(struct rproc *, int);
    void * (*da_to_va)(struct rproc *, u64, size_t, bool *);
    int (*parse_fw)(struct rproc *, const struct firmware *);
    int (*handle_rsc)(struct rproc *, u32, void *, int, int);
    struct resource_table * (*find_loaded_rsc_table)(struct rproc *, const struct firmware *);
    struct resource_table * (*get_loaded_rsc_table)(struct rproc *, size_t *);
    int (*load)(struct rproc *, const struct firmware *);
    int (*sanity_check)(struct rproc *, const struct firmware *);
    u64 (*get_boot_addr)(struct rproc *, const struct firmware *);
    long unsigned int (*panic)(struct rproc *);
    void (*coredump)(struct rproc *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rproc_ops {
    int (*prepare)(struct rproc *);
    int (*unprepare)(struct rproc *);
    int (*start)(struct rproc *);
    int (*stop)(struct rproc *);
    int (*attach)(struct rproc *);
    int (*detach)(struct rproc *);
    void (*kick)(struct rproc *, int);
    void * (*da_to_va)(struct rproc *, u64, size_t, bool *);
    int (*parse_fw)(struct rproc *, const struct firmware *);
    int (*handle_rsc)(struct rproc *, u32, void *, int, int);
    struct resource_table * (*find_loaded_rsc_table)(struct rproc *, const struct firmware *);
    struct resource_table * (*get_loaded_rsc_table)(struct rproc *, size_t *);
    int (*load)(struct rproc *, const struct firmware *);
    int (*sanity_check)(struct rproc *, const struct firmware *);
    u64 (*get_boot_addr)(struct rproc *, const struct firmware *);
    long unsigned int (*panic)(struct rproc *);
    void (*coredump)(struct rproc *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rproc_ops {
    int (*prepare)(struct rproc *);
    int (*unprepare)(struct rproc *);
    int (*start)(struct rproc *);
    int (*stop)(struct rproc *);
    int (*attach)(struct rproc *);
    int (*detach)(struct rproc *);
    void (*kick)(struct rproc *, int);
    void * (*da_to_va)(struct rproc *, u64, size_t, bool *);
    int (*parse_fw)(struct rproc *, const struct firmware *);
    int (*handle_rsc)(struct rproc *, u32, void *, int, int);
    struct resource_table * (*find_loaded_rsc_table)(struct rproc *, const struct firmware *);
    struct resource_table * (*get_loaded_rsc_table)(struct rproc *, size_t *);
    int (*load)(struct rproc *, const struct firmware *);
    int (*sanity_check)(struct rproc *, const struct firmware *);
    u64 (*get_boot_addr)(struct rproc *, const struct firmware *);
    long unsigned int (*panic)(struct rproc *);
    void (*coredump)(struct rproc *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rproc_ops {
    int (*prepare)(struct rproc *);
    int (*unprepare)(struct rproc *);
    int (*start)(struct rproc *);
    int (*stop)(struct rproc *);
    int (*attach)(struct rproc *);
    int (*detach)(struct rproc *);
    void (*kick)(struct rproc *, int);
    void * (*da_to_va)(struct rproc *, u64, size_t, bool *);
    int (*parse_fw)(struct rproc *, const struct firmware *);
    int (*handle_rsc)(struct rproc *, u32, void *, int, int);
    struct resource_table * (*find_loaded_rsc_table)(struct rproc *, const struct firmware *);
    struct resource_table * (*get_loaded_rsc_table)(struct rproc *, size_t *);
    int (*load)(struct rproc *, const struct firmware *);
    int (*sanity_check)(struct rproc *, const struct firmware *);
    u64 (*get_boot_addr)(struct rproc *, const struct firmware *);
    long unsigned int (*panic)(struct rproc *);
    void (*coredump)(struct rproc *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rproc_ops {
    int (*prepare)(struct rproc *);
    int (*unprepare)(struct rproc *);
    int (*start)(struct rproc *);
    int (*stop)(struct rproc *);
    int (*attach)(struct rproc *);
    int (*detach)(struct rproc *);
    void (*kick)(struct rproc *, int);
    void * (*da_to_va)(struct rproc *, u64, size_t, bool *);
    int (*parse_fw)(struct rproc *, const struct firmware *);
    int (*handle_rsc)(struct rproc *, u32, void *, int, int);
    struct resource_table * (*find_loaded_rsc_table)(struct rproc *, const struct firmware *);
    struct resource_table * (*get_loaded_rsc_table)(struct rproc *, size_t *);
    int (*load)(struct rproc *, const struct firmware *);
    int (*sanity_check)(struct rproc *, const struct firmware *);
    u64 (*get_boot_addr)(struct rproc *, const struct firmware *);
    long unsigned int (*panic)(struct rproc *);
    void (*coredump)(struct rproc *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rproc_ops {
    int (*prepare)(struct rproc *);
    int (*unprepare)(struct rproc *);
    int (*start)(struct rproc *);
    int (*stop)(struct rproc *);
    int (*attach)(struct rproc *);
    int (*detach)(struct rproc *);
    void (*kick)(struct rproc *, int);
    void * (*da_to_va)(struct rproc *, u64, size_t, bool *);
    int (*parse_fw)(struct rproc *, const struct firmware *);
    int (*handle_rsc)(struct rproc *, u32, void *, int, int);
    struct resource_table * (*find_loaded_rsc_table)(struct rproc *, const struct firmware *);
    struct resource_table * (*get_loaded_rsc_table)(struct rproc *, size_t *);
    int (*load)(struct rproc *, const struct firmware *);
    int (*sanity_check)(struct rproc *, const struct firmware *);
    u64 (*get_boot_addr)(struct rproc *, const struct firmware *);
    long unsigned int (*panic)(struct rproc *);
    void (*coredump)(struct rproc *);
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
struct rproc_ops {
    int (*start)(struct rproc *);
    int (*stop)(struct rproc *);
    void (*kick)(struct rproc *, int);
    void * (*da_to_va)(struct rproc *, u64, int);
    int (*parse_fw)(struct rproc *, const struct firmware *);
    int (*handle_rsc)(struct rproc *, u32, void *, int, int);
    struct resource_table * (*find_loaded_rsc_table)(struct rproc *, const struct firmware *);
    int (*load)(struct rproc *, const struct firmware *);
    int (*sanity_check)(struct rproc *, const struct firmware *);
    u32 (*get_boot_addr)(struct rproc *, const struct firmware *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rproc_ops {
    int (*start)(struct rproc *);
    int (*stop)(struct rproc *);
    void (*kick)(struct rproc *, int);
    void * (*da_to_va)(struct rproc *, u64, int);
    int (*parse_fw)(struct rproc *, const struct firmware *);
    int (*handle_rsc)(struct rproc *, u32, void *, int, int);
    struct resource_table * (*find_loaded_rsc_table)(struct rproc *, const struct firmware *);
    int (*load)(struct rproc *, const struct firmware *);
    int (*sanity_check)(struct rproc *, const struct firmware *);
    u32 (*get_boot_addr)(struct rproc *, const struct firmware *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rproc_ops {
    int (*start)(struct rproc *);
    int (*stop)(struct rproc *);
    void (*kick)(struct rproc *, int);
    void * (*da_to_va)(struct rproc *, u64, int);
    int (*parse_fw)(struct rproc *, const struct firmware *);
    int (*handle_rsc)(struct rproc *, u32, void *, int, int);
    struct resource_table * (*find_loaded_rsc_table)(struct rproc *, const struct firmware *);
    int (*load)(struct rproc *, const struct firmware *);
    int (*sanity_check)(struct rproc *, const struct firmware *);
    u32 (*get_boot_addr)(struct rproc *, const struct firmware *);
};
```
</details>
</li>
<li>
In <code>riscv64</code>: Absent ⚠️
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct rproc_ops {
    int (*start)(struct rproc *);
    int (*stop)(struct rproc *);
    void (*kick)(struct rproc *, int);
    void * (*da_to_va)(struct rproc *, u64, int);
    int (*parse_fw)(struct rproc *, const struct firmware *);
    int (*handle_rsc)(struct rproc *, u32, void *, int, int);
    struct resource_table * (*find_loaded_rsc_table)(struct rproc *, const struct firmware *);
    int (*load)(struct rproc *, const struct firmware *);
    int (*sanity_check)(struct rproc *, const struct firmware *);
    u32 (*get_boot_addr)(struct rproc *, const struct firmware *);
};
```
</details>
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rproc_ops {
    int (*start)(struct rproc *);
    int (*stop)(struct rproc *);
    void (*kick)(struct rproc *, int);
    void * (*da_to_va)(struct rproc *, u64, int);
    int (*parse_fw)(struct rproc *, const struct firmware *);
    int (*handle_rsc)(struct rproc *, u32, void *, int, int);
    struct resource_table * (*find_loaded_rsc_table)(struct rproc *, const struct firmware *);
    int (*load)(struct rproc *, const struct firmware *);
    int (*sanity_check)(struct rproc *, const struct firmware *);
    u32 (*get_boot_addr)(struct rproc *, const struct firmware *);
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
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*prepare)(struct rproc *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*unprepare)(struct rproc *)</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int (*panic)(struct rproc *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void * (*da_to_va)(struct rproc *, u64, int)</code> ➡️ <code>void * (*da_to_va)(struct rproc *, u64, size_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 (*get_boot_addr)(struct rproc *, const struct firmware *)</code> ➡️ <code>u64 (*get_boot_addr)(struct rproc *, const struct firmware *)</code>
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
<code>int (*attach)(struct rproc *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*coredump)(struct rproc *)</code>
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
<code>int (*detach)(struct rproc *)</code>
</li>
<li>
<b>Field added. </b>
<code>struct resource_table * (*get_loaded_rsc_table)(struct rproc *, size_t *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void * (*da_to_va)(struct rproc *, u64, size_t)</code> ➡️ <code>void * (*da_to_va)(struct rproc *, u64, size_t, bool *)</code>
</li>
</ul>
</details>
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
</ul>
<b>Flavor</b>
<ul>
<li>
No changes between <code>generic</code> and <code>aws</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
