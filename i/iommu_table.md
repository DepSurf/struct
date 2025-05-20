# Struct: <code>iommu_table</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct iommu_table {
    struct cal_chipset_ops *chip_ops;
    long unsigned int it_base;
    long unsigned int it_hint;
    long unsigned int *it_map;
    void *bbar;
    u64 tar_val;
    struct timer_list watchdog_timer;
    spinlock_t it_lock;
    unsigned int it_size;
    unsigned char it_busno;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct iommu_table {
    const struct cal_chipset_ops *chip_ops;
    long unsigned int it_base;
    long unsigned int it_hint;
    long unsigned int *it_map;
    void *bbar;
    u64 tar_val;
    struct timer_list watchdog_timer;
    spinlock_t it_lock;
    unsigned int it_size;
    unsigned char it_busno;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct iommu_table {
    const struct cal_chipset_ops *chip_ops;
    long unsigned int it_base;
    long unsigned int it_hint;
    long unsigned int *it_map;
    void *bbar;
    u64 tar_val;
    struct timer_list watchdog_timer;
    spinlock_t it_lock;
    unsigned int it_size;
    unsigned char it_busno;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct iommu_table {
    const struct cal_chipset_ops *chip_ops;
    long unsigned int it_base;
    long unsigned int it_hint;
    long unsigned int *it_map;
    void *bbar;
    u64 tar_val;
    struct timer_list watchdog_timer;
    spinlock_t it_lock;
    unsigned int it_size;
    unsigned char it_busno;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct iommu_table {
    const struct cal_chipset_ops *chip_ops;
    long unsigned int it_base;
    long unsigned int it_hint;
    long unsigned int *it_map;
    void *bbar;
    u64 tar_val;
    struct timer_list watchdog_timer;
    spinlock_t it_lock;
    unsigned int it_size;
    unsigned char it_busno;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct iommu_table {
    const struct cal_chipset_ops *chip_ops;
    long unsigned int it_base;
    long unsigned int it_hint;
    long unsigned int *it_map;
    void *bbar;
    u64 tar_val;
    struct timer_list watchdog_timer;
    spinlock_t it_lock;
    unsigned int it_size;
    unsigned char it_busno;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct iommu_table {
    const struct cal_chipset_ops *chip_ops;
    long unsigned int it_base;
    long unsigned int it_hint;
    long unsigned int *it_map;
    void *bbar;
    u64 tar_val;
    struct timer_list watchdog_timer;
    spinlock_t it_lock;
    unsigned int it_size;
    unsigned char it_busno;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct iommu_table {
    const struct cal_chipset_ops *chip_ops;
    long unsigned int it_base;
    long unsigned int it_hint;
    long unsigned int *it_map;
    void *bbar;
    u64 tar_val;
    struct timer_list watchdog_timer;
    spinlock_t it_lock;
    unsigned int it_size;
    unsigned char it_busno;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct iommu_table {
    const struct cal_chipset_ops *chip_ops;
    long unsigned int it_base;
    long unsigned int it_hint;
    long unsigned int *it_map;
    void *bbar;
    u64 tar_val;
    struct timer_list watchdog_timer;
    spinlock_t it_lock;
    unsigned int it_size;
    unsigned char it_busno;
};
```
</details>
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
In <code>arm64</code>: Absent ⚠️
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct iommu_table {
    long unsigned int it_busno;
    long unsigned int it_size;
    long unsigned int it_indirect_levels;
    long unsigned int it_level_size;
    long unsigned int it_allocated_size;
    long unsigned int it_offset;
    long unsigned int it_base;
    long unsigned int it_index;
    long unsigned int it_type;
    long unsigned int it_blocksize;
    long unsigned int poolsize;
    long unsigned int nr_pools;
    struct iommu_pool large_pool;
    struct iommu_pool pools[4];
    long unsigned int *it_map;
    long unsigned int it_page_shift;
    struct list_head it_group_list;
    __be64 *it_userspace;
    struct iommu_table_ops *it_ops;
    struct kref it_kref;
    int it_nid;
    long unsigned int it_reserved_start;
    long unsigned int it_reserved_end;
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
struct iommu_table {
    const struct cal_chipset_ops *chip_ops;
    long unsigned int it_base;
    long unsigned int it_hint;
    long unsigned int *it_map;
    void *bbar;
    u64 tar_val;
    struct timer_list watchdog_timer;
    spinlock_t it_lock;
    unsigned int it_size;
    unsigned char it_busno;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct iommu_table {
    const struct cal_chipset_ops *chip_ops;
    long unsigned int it_base;
    long unsigned int it_hint;
    long unsigned int *it_map;
    void *bbar;
    u64 tar_val;
    struct timer_list watchdog_timer;
    spinlock_t it_lock;
    unsigned int it_size;
    unsigned char it_busno;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct iommu_table {
    const struct cal_chipset_ops *chip_ops;
    long unsigned int it_base;
    long unsigned int it_hint;
    long unsigned int *it_map;
    void *bbar;
    u64 tar_val;
    struct timer_list watchdog_timer;
    spinlock_t it_lock;
    unsigned int it_size;
    unsigned char it_busno;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct iommu_table {
    const struct cal_chipset_ops *chip_ops;
    long unsigned int it_base;
    long unsigned int it_hint;
    long unsigned int *it_map;
    void *bbar;
    u64 tar_val;
    struct timer_list watchdog_timer;
    spinlock_t it_lock;
    unsigned int it_size;
    unsigned char it_busno;
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
<b>Field type changed. </b>
<code>struct cal_chipset_ops *chip_ops</code> ➡️ <code>const struct cal_chipset_ops *chip_ops</code>
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
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int it_indirect_levels</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int it_level_size</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int it_allocated_size</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int it_offset</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int it_index</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int it_type</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int it_blocksize</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int poolsize</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int nr_pools</code>
</li>
<li>
<b>Field added. </b>
<code>struct iommu_pool large_pool</code>
</li>
<li>
<b>Field added. </b>
<code>struct iommu_pool pools[4]</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int it_page_shift</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head it_group_list</code>
</li>
<li>
<b>Field added. </b>
<code>__be64 *it_userspace</code>
</li>
<li>
<b>Field added. </b>
<code>struct iommu_table_ops *it_ops</code>
</li>
<li>
<b>Field added. </b>
<code>struct kref it_kref</code>
</li>
<li>
<b>Field added. </b>
<code>int it_nid</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int it_reserved_start</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int it_reserved_end</code>
</li>
<li>
<b>Field removed. </b>
<code>const struct cal_chipset_ops *chip_ops</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int it_hint</code>
</li>
<li>
<b>Field removed. </b>
<code>void *bbar</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 tar_val</code>
</li>
<li>
<b>Field removed. </b>
<code>struct timer_list watchdog_timer</code>
</li>
<li>
<b>Field removed. </b>
<code>spinlock_t it_lock</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int it_size</code> ➡️ <code>long unsigned int it_size</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned char it_busno</code> ➡️ <code>long unsigned int it_busno</code>
</li>
</ul>
</details>
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
