# Struct: <code>protection_domain</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct protection_domain {
    struct list_head list;
    struct list_head dev_list;
    struct iommu_domain domain;
    spinlock_t lock;
    struct mutex api_lock;
    u16 id;
    int mode;
    u64 *pt_root;
    int glx;
    u64 *gcr3_tbl;
    long unsigned int flags;
    bool updated;
    unsigned int dev_cnt;
    unsigned int dev_iommu[32];
    void *priv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct protection_domain {
    struct list_head list;
    struct list_head dev_list;
    struct iommu_domain domain;
    spinlock_t lock;
    struct mutex api_lock;
    u16 id;
    int mode;
    u64 *pt_root;
    int glx;
    u64 *gcr3_tbl;
    long unsigned int flags;
    bool updated;
    unsigned int dev_cnt;
    unsigned int dev_iommu[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct protection_domain {
    struct list_head list;
    struct list_head dev_list;
    struct iommu_domain domain;
    spinlock_t lock;
    struct mutex api_lock;
    u16 id;
    int mode;
    u64 *pt_root;
    int glx;
    u64 *gcr3_tbl;
    long unsigned int flags;
    bool updated;
    unsigned int dev_cnt;
    unsigned int dev_iommu[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct protection_domain {
    struct list_head list;
    struct list_head dev_list;
    struct iommu_domain domain;
    spinlock_t lock;
    struct mutex api_lock;
    u16 id;
    int mode;
    u64 *pt_root;
    int glx;
    u64 *gcr3_tbl;
    long unsigned int flags;
    bool updated;
    unsigned int dev_cnt;
    unsigned int dev_iommu[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct protection_domain {
    struct list_head list;
    struct list_head dev_list;
    struct iommu_domain domain;
    spinlock_t lock;
    struct mutex api_lock;
    u16 id;
    int mode;
    u64 *pt_root;
    int glx;
    u64 *gcr3_tbl;
    long unsigned int flags;
    bool updated;
    unsigned int dev_cnt;
    unsigned int dev_iommu[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct protection_domain {
    struct list_head list;
    struct list_head dev_list;
    struct iommu_domain domain;
    spinlock_t lock;
    struct mutex api_lock;
    u16 id;
    int mode;
    u64 *pt_root;
    int glx;
    u64 *gcr3_tbl;
    long unsigned int flags;
    bool updated;
    unsigned int dev_cnt;
    unsigned int dev_iommu[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct protection_domain {
    struct list_head list;
    struct list_head dev_list;
    struct iommu_domain domain;
    spinlock_t lock;
    struct mutex api_lock;
    u16 id;
    int mode;
    u64 *pt_root;
    int glx;
    u64 *gcr3_tbl;
    long unsigned int flags;
    bool updated;
    unsigned int dev_cnt;
    unsigned int dev_iommu[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct protection_domain {
    struct list_head list;
    struct list_head dev_list;
    struct iommu_domain domain;
    spinlock_t lock;
    struct mutex api_lock;
    u16 id;
    int mode;
    u64 *pt_root;
    int glx;
    u64 *gcr3_tbl;
    long unsigned int flags;
    bool updated;
    unsigned int dev_cnt;
    unsigned int dev_iommu[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct protection_domain {
    struct list_head list;
    struct list_head dev_list;
    struct iommu_domain domain;
    spinlock_t lock;
    struct mutex api_lock;
    u16 id;
    int mode;
    u64 *pt_root;
    int glx;
    u64 *gcr3_tbl;
    long unsigned int flags;
    unsigned int dev_cnt;
    unsigned int dev_iommu[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct protection_domain {
    struct list_head dev_list;
    struct iommu_domain domain;
    spinlock_t lock;
    u16 id;
    atomic64_t pt_root;
    int glx;
    u64 *gcr3_tbl;
    long unsigned int flags;
    unsigned int dev_cnt;
    unsigned int dev_iommu[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct protection_domain {
    struct list_head dev_list;
    struct iommu_domain domain;
    spinlock_t lock;
    u16 id;
    atomic64_t pt_root;
    int glx;
    u64 *gcr3_tbl;
    long unsigned int flags;
    unsigned int dev_cnt;
    unsigned int dev_iommu[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct protection_domain {
    struct list_head dev_list;
    struct iommu_domain domain;
    struct amd_io_pgtable iop;
    spinlock_t lock;
    u16 id;
    int glx;
    u64 *gcr3_tbl;
    long unsigned int flags;
    unsigned int dev_cnt;
    unsigned int dev_iommu[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct protection_domain {
    struct list_head dev_list;
    struct iommu_domain domain;
    struct amd_io_pgtable iop;
    spinlock_t lock;
    u16 id;
    int glx;
    u64 *gcr3_tbl;
    long unsigned int flags;
    unsigned int dev_cnt;
    unsigned int dev_iommu[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct protection_domain {
    struct list_head dev_list;
    struct iommu_domain domain;
    struct amd_io_pgtable iop;
    spinlock_t lock;
    u16 id;
    int glx;
    u64 *gcr3_tbl;
    long unsigned int flags;
    unsigned int dev_cnt;
    unsigned int dev_iommu[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct protection_domain {
    struct list_head dev_list;
    struct iommu_domain domain;
    struct amd_io_pgtable iop;
    spinlock_t lock;
    u16 id;
    int glx;
    u64 *gcr3_tbl;
    long unsigned int flags;
    unsigned int dev_cnt;
    unsigned int dev_iommu[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct protection_domain {
    struct list_head dev_list;
    struct iommu_domain domain;
    struct amd_io_pgtable iop;
    spinlock_t lock;
    u16 id;
    int glx;
    int nid;
    u64 *gcr3_tbl;
    long unsigned int flags;
    unsigned int dev_cnt;
    unsigned int dev_iommu[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct protection_domain {
    struct list_head dev_list;
    struct iommu_domain domain;
    struct amd_io_pgtable iop;
    spinlock_t lock;
    u16 id;
    int glx;
    int nid;
    u64 *gcr3_tbl;
    long unsigned int flags;
    bool dirty_tracking;
    unsigned int dev_cnt;
    unsigned int dev_iommu[32];
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
struct protection_domain {
    struct list_head list;
    struct list_head dev_list;
    struct iommu_domain domain;
    spinlock_t lock;
    struct mutex api_lock;
    u16 id;
    int mode;
    u64 *pt_root;
    int glx;
    u64 *gcr3_tbl;
    long unsigned int flags;
    unsigned int dev_cnt;
    unsigned int dev_iommu[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct protection_domain {
    struct list_head list;
    struct list_head dev_list;
    struct iommu_domain domain;
    spinlock_t lock;
    struct mutex api_lock;
    u16 id;
    int mode;
    u64 *pt_root;
    int glx;
    u64 *gcr3_tbl;
    long unsigned int flags;
    unsigned int dev_cnt;
    unsigned int dev_iommu[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct protection_domain {
    struct list_head list;
    struct list_head dev_list;
    struct iommu_domain domain;
    spinlock_t lock;
    struct mutex api_lock;
    u16 id;
    int mode;
    u64 *pt_root;
    int glx;
    u64 *gcr3_tbl;
    long unsigned int flags;
    unsigned int dev_cnt;
    unsigned int dev_iommu[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct protection_domain {
    struct list_head list;
    struct list_head dev_list;
    struct iommu_domain domain;
    spinlock_t lock;
    struct mutex api_lock;
    u16 id;
    int mode;
    u64 *pt_root;
    int glx;
    u64 *gcr3_tbl;
    long unsigned int flags;
    unsigned int dev_cnt;
    unsigned int dev_iommu[32];
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
<b>Field removed. </b>
<code>void *priv</code>
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
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>bool updated</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct list_head list</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mutex api_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>int mode</code>
</li>
<li>
<b>Field type changed. </b>
<code>u64 *pt_root</code> ➡️ <code>atomic64_t pt_root</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct amd_io_pgtable iop</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic64_t pt_root</code>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int nid</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool dirty_tracking</code>
</li>
</ul>
</details>
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
