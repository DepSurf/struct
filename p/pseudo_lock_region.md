# Struct: <code>pseudo_lock_region</code>

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
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct pseudo_lock_region {
    struct rdt_resource *r;
    struct rdt_domain *d;
    u32 cbm;
    wait_queue_head_t lock_thread_wq;
    int thread_done;
    int cpu;
    unsigned int line_size;
    unsigned int size;
    void *kmem;
    unsigned int minor;
    struct dentry *debugfs_dir;
    struct list_head pm_reqs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct pseudo_lock_region {
    struct rdt_resource *r;
    struct rdt_domain *d;
    u32 cbm;
    wait_queue_head_t lock_thread_wq;
    int thread_done;
    int cpu;
    unsigned int line_size;
    unsigned int size;
    void *kmem;
    unsigned int minor;
    struct dentry *debugfs_dir;
    struct list_head pm_reqs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct pseudo_lock_region {
    struct rdt_resource *r;
    struct rdt_domain *d;
    u32 cbm;
    wait_queue_head_t lock_thread_wq;
    int thread_done;
    int cpu;
    unsigned int line_size;
    unsigned int size;
    void *kmem;
    unsigned int minor;
    struct dentry *debugfs_dir;
    struct list_head pm_reqs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct pseudo_lock_region {
    struct rdt_resource *r;
    struct rdt_domain *d;
    u32 cbm;
    wait_queue_head_t lock_thread_wq;
    int thread_done;
    int cpu;
    unsigned int line_size;
    unsigned int size;
    void *kmem;
    unsigned int minor;
    struct dentry *debugfs_dir;
    struct list_head pm_reqs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct pseudo_lock_region {
    struct rdt_resource *r;
    struct rdt_domain *d;
    u32 cbm;
    wait_queue_head_t lock_thread_wq;
    int thread_done;
    int cpu;
    unsigned int line_size;
    unsigned int size;
    void *kmem;
    unsigned int minor;
    struct dentry *debugfs_dir;
    struct list_head pm_reqs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct pseudo_lock_region {
    struct rdt_resource *r;
    struct rdt_domain *d;
    u32 cbm;
    wait_queue_head_t lock_thread_wq;
    int thread_done;
    int cpu;
    unsigned int line_size;
    unsigned int size;
    void *kmem;
    unsigned int minor;
    struct dentry *debugfs_dir;
    struct list_head pm_reqs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct pseudo_lock_region {
    struct resctrl_schema *s;
    struct rdt_domain *d;
    u32 cbm;
    wait_queue_head_t lock_thread_wq;
    int thread_done;
    int cpu;
    unsigned int line_size;
    unsigned int size;
    void *kmem;
    unsigned int minor;
    struct dentry *debugfs_dir;
    struct list_head pm_reqs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct pseudo_lock_region {
    struct resctrl_schema *s;
    struct rdt_domain *d;
    u32 cbm;
    wait_queue_head_t lock_thread_wq;
    int thread_done;
    int cpu;
    unsigned int line_size;
    unsigned int size;
    void *kmem;
    unsigned int minor;
    struct dentry *debugfs_dir;
    struct list_head pm_reqs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct pseudo_lock_region {
    struct resctrl_schema *s;
    struct rdt_domain *d;
    u32 cbm;
    wait_queue_head_t lock_thread_wq;
    int thread_done;
    int cpu;
    unsigned int line_size;
    unsigned int size;
    void *kmem;
    unsigned int minor;
    struct dentry *debugfs_dir;
    struct list_head pm_reqs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct pseudo_lock_region {
    struct resctrl_schema *s;
    struct rdt_domain *d;
    u32 cbm;
    wait_queue_head_t lock_thread_wq;
    int thread_done;
    int cpu;
    unsigned int line_size;
    unsigned int size;
    void *kmem;
    unsigned int minor;
    struct dentry *debugfs_dir;
    struct list_head pm_reqs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct pseudo_lock_region {
    struct resctrl_schema *s;
    struct rdt_domain *d;
    u32 cbm;
    wait_queue_head_t lock_thread_wq;
    int thread_done;
    int cpu;
    unsigned int line_size;
    unsigned int size;
    void *kmem;
    unsigned int minor;
    struct dentry *debugfs_dir;
    struct list_head pm_reqs;
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct pseudo_lock_region {
    struct rdt_resource *r;
    struct rdt_domain *d;
    u32 cbm;
    wait_queue_head_t lock_thread_wq;
    int thread_done;
    int cpu;
    unsigned int line_size;
    unsigned int size;
    void *kmem;
    unsigned int minor;
    struct dentry *debugfs_dir;
    struct list_head pm_reqs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct pseudo_lock_region {
    struct rdt_resource *r;
    struct rdt_domain *d;
    u32 cbm;
    wait_queue_head_t lock_thread_wq;
    int thread_done;
    int cpu;
    unsigned int line_size;
    unsigned int size;
    void *kmem;
    unsigned int minor;
    struct dentry *debugfs_dir;
    struct list_head pm_reqs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct pseudo_lock_region {
    struct rdt_resource *r;
    struct rdt_domain *d;
    u32 cbm;
    wait_queue_head_t lock_thread_wq;
    int thread_done;
    int cpu;
    unsigned int line_size;
    unsigned int size;
    void *kmem;
    unsigned int minor;
    struct dentry *debugfs_dir;
    struct list_head pm_reqs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct pseudo_lock_region {
    struct rdt_resource *r;
    struct rdt_domain *d;
    u32 cbm;
    wait_queue_head_t lock_thread_wq;
    int thread_done;
    int cpu;
    unsigned int line_size;
    unsigned int size;
    void *kmem;
    unsigned int minor;
    struct dentry *debugfs_dir;
    struct list_head pm_reqs;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
No changes between <code>5.8</code> and <code>5.11</code> ✅
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
<code>struct resctrl_schema *s</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rdt_resource *r</code>
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
<b>Arch</b>
<ul>
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
