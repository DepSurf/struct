# Struct: <code>nvm_tgt_type</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct nvm_tgt_type {
    const char *name;
    unsigned int version[3];
    nvm_tgt_make_rq_fn *make_rq;
    nvm_tgt_capacity_fn *capacity;
    nvm_end_io_fn *end_io;
    nvm_tgt_init_fn *init;
    nvm_tgt_exit_fn *exit;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct nvm_tgt_type {
    const char *name;
    unsigned int version[3];
    nvm_tgt_make_rq_fn *make_rq;
    nvm_tgt_capacity_fn *capacity;
    nvm_end_io_fn *end_io;
    nvm_tgt_init_fn *init;
    nvm_tgt_exit_fn *exit;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct nvm_tgt_type {
    const char *name;
    unsigned int version[3];
    nvm_tgt_make_rq_fn *make_rq;
    nvm_tgt_capacity_fn *capacity;
    nvm_end_io_fn *end_io;
    nvm_tgt_init_fn *init;
    nvm_tgt_exit_fn *exit;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct nvm_tgt_type {
    const char *name;
    unsigned int version[3];
    nvm_tgt_make_rq_fn *make_rq;
    nvm_tgt_capacity_fn *capacity;
    nvm_tgt_init_fn *init;
    nvm_tgt_exit_fn *exit;
    nvm_tgt_sysfs_init_fn *sysfs_init;
    nvm_tgt_sysfs_exit_fn *sysfs_exit;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct nvm_tgt_type {
    const char *name;
    unsigned int version[3];
    nvm_tgt_make_rq_fn *make_rq;
    nvm_tgt_capacity_fn *capacity;
    nvm_tgt_init_fn *init;
    nvm_tgt_exit_fn *exit;
    nvm_tgt_sysfs_init_fn *sysfs_init;
    nvm_tgt_sysfs_exit_fn *sysfs_exit;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct nvm_tgt_type {
    const char *name;
    unsigned int version[3];
    nvm_tgt_make_rq_fn *make_rq;
    nvm_tgt_capacity_fn *capacity;
    nvm_tgt_init_fn *init;
    nvm_tgt_exit_fn *exit;
    nvm_tgt_sysfs_init_fn *sysfs_init;
    nvm_tgt_sysfs_exit_fn *sysfs_exit;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct nvm_tgt_type {
    const char *name;
    unsigned int version[3];
    int flags;
    nvm_tgt_make_rq_fn *make_rq;
    nvm_tgt_capacity_fn *capacity;
    nvm_tgt_init_fn *init;
    nvm_tgt_exit_fn *exit;
    nvm_tgt_sysfs_init_fn *sysfs_init;
    nvm_tgt_sysfs_exit_fn *sysfs_exit;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct nvm_tgt_type {
    const char *name;
    unsigned int version[3];
    int flags;
    nvm_tgt_make_rq_fn *make_rq;
    nvm_tgt_capacity_fn *capacity;
    nvm_tgt_init_fn *init;
    nvm_tgt_exit_fn *exit;
    nvm_tgt_sysfs_init_fn *sysfs_init;
    nvm_tgt_sysfs_exit_fn *sysfs_exit;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct nvm_tgt_type {
    const char *name;
    unsigned int version[3];
    int flags;
    nvm_tgt_make_rq_fn *make_rq;
    nvm_tgt_capacity_fn *capacity;
    nvm_tgt_init_fn *init;
    nvm_tgt_exit_fn *exit;
    nvm_tgt_sysfs_init_fn *sysfs_init;
    nvm_tgt_sysfs_exit_fn *sysfs_exit;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct nvm_tgt_type {
    const char *name;
    unsigned int version[3];
    int flags;
    nvm_tgt_make_rq_fn *make_rq;
    nvm_tgt_capacity_fn *capacity;
    nvm_tgt_init_fn *init;
    nvm_tgt_exit_fn *exit;
    nvm_tgt_sysfs_init_fn *sysfs_init;
    nvm_tgt_sysfs_exit_fn *sysfs_exit;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct nvm_tgt_type {
    const char *name;
    unsigned int version[3];
    int flags;
    const struct block_device_operations *bops;
    nvm_tgt_capacity_fn *capacity;
    nvm_tgt_init_fn *init;
    nvm_tgt_exit_fn *exit;
    nvm_tgt_sysfs_init_fn *sysfs_init;
    nvm_tgt_sysfs_exit_fn *sysfs_exit;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct nvm_tgt_type {
    const char *name;
    unsigned int version[3];
    int flags;
    const struct block_device_operations *bops;
    nvm_tgt_capacity_fn *capacity;
    nvm_tgt_init_fn *init;
    nvm_tgt_exit_fn *exit;
    nvm_tgt_sysfs_init_fn *sysfs_init;
    nvm_tgt_sysfs_exit_fn *sysfs_exit;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
In <code>5.19</code>: Absent ⚠️
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct nvm_tgt_type {
    const char *name;
    unsigned int version[3];
    int flags;
    nvm_tgt_make_rq_fn *make_rq;
    nvm_tgt_capacity_fn *capacity;
    nvm_tgt_init_fn *init;
    nvm_tgt_exit_fn *exit;
    nvm_tgt_sysfs_init_fn *sysfs_init;
    nvm_tgt_sysfs_exit_fn *sysfs_exit;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct nvm_tgt_type {
    const char *name;
    unsigned int version[3];
    int flags;
    nvm_tgt_make_rq_fn *make_rq;
    nvm_tgt_capacity_fn *capacity;
    nvm_tgt_init_fn *init;
    nvm_tgt_exit_fn *exit;
    nvm_tgt_sysfs_init_fn *sysfs_init;
    nvm_tgt_sysfs_exit_fn *sysfs_exit;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct nvm_tgt_type {
    const char *name;
    unsigned int version[3];
    int flags;
    nvm_tgt_make_rq_fn *make_rq;
    nvm_tgt_capacity_fn *capacity;
    nvm_tgt_init_fn *init;
    nvm_tgt_exit_fn *exit;
    nvm_tgt_sysfs_init_fn *sysfs_init;
    nvm_tgt_sysfs_exit_fn *sysfs_exit;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct nvm_tgt_type {
    const char *name;
    unsigned int version[3];
    int flags;
    nvm_tgt_make_rq_fn *make_rq;
    nvm_tgt_capacity_fn *capacity;
    nvm_tgt_init_fn *init;
    nvm_tgt_exit_fn *exit;
    nvm_tgt_sysfs_init_fn *sysfs_init;
    nvm_tgt_sysfs_exit_fn *sysfs_exit;
    struct list_head list;
    struct module *owner;
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
struct nvm_tgt_type {
    const char *name;
    unsigned int version[3];
    int flags;
    nvm_tgt_make_rq_fn *make_rq;
    nvm_tgt_capacity_fn *capacity;
    nvm_tgt_init_fn *init;
    nvm_tgt_exit_fn *exit;
    nvm_tgt_sysfs_init_fn *sysfs_init;
    nvm_tgt_sysfs_exit_fn *sysfs_exit;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct nvm_tgt_type {
    const char *name;
    unsigned int version[3];
    int flags;
    nvm_tgt_make_rq_fn *make_rq;
    nvm_tgt_capacity_fn *capacity;
    nvm_tgt_init_fn *init;
    nvm_tgt_exit_fn *exit;
    nvm_tgt_sysfs_init_fn *sysfs_init;
    nvm_tgt_sysfs_exit_fn *sysfs_exit;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct nvm_tgt_type {
    const char *name;
    unsigned int version[3];
    int flags;
    nvm_tgt_make_rq_fn *make_rq;
    nvm_tgt_capacity_fn *capacity;
    nvm_tgt_init_fn *init;
    nvm_tgt_exit_fn *exit;
    nvm_tgt_sysfs_init_fn *sysfs_init;
    nvm_tgt_sysfs_exit_fn *sysfs_exit;
    struct list_head list;
    struct module *owner;
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
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>nvm_tgt_sysfs_init_fn *sysfs_init</code>
</li>
<li>
<b>Field added. </b>
<code>nvm_tgt_sysfs_exit_fn *sysfs_exit</code>
</li>
<li>
<b>Field removed. </b>
<code>nvm_end_io_fn *end_io</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct module *owner</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int flags</code>
</li>
</ul>
</details>
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
<code>const struct block_device_operations *bops</code>
</li>
<li>
<b>Field removed. </b>
<code>nvm_tgt_make_rq_fn *make_rq</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
