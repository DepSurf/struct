# Struct: <code>io_pgtable_cfg</code>

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
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct io_pgtable_cfg {
    long unsigned int quirks;
    long unsigned int pgsize_bitmap;
    unsigned int ias;
    unsigned int oas;
    bool coherent_walk;
    const struct iommu_flush_ops *tlb;
    struct device *iommu_dev;
    struct (anon) arm_lpae_s1_cfg;
    struct (anon) arm_lpae_s2_cfg;
    struct (anon) arm_v7s_cfg;
    struct (anon) arm_mali_lpae_cfg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct io_pgtable_cfg {
    long unsigned int quirks;
    long unsigned int pgsize_bitmap;
    unsigned int ias;
    unsigned int oas;
    bool coherent_walk;
    const struct iommu_flush_ops *tlb;
    struct device *iommu_dev;
    struct (anon) arm_lpae_s1_cfg;
    struct (anon) arm_lpae_s2_cfg;
    struct (anon) arm_v7s_cfg;
    struct (anon) arm_mali_lpae_cfg;
    struct (anon) apple_dart_cfg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct io_pgtable_cfg {
    long unsigned int quirks;
    long unsigned int pgsize_bitmap;
    unsigned int ias;
    unsigned int oas;
    bool coherent_walk;
    const struct iommu_flush_ops *tlb;
    struct device *iommu_dev;
    struct (anon) arm_lpae_s1_cfg;
    struct (anon) arm_lpae_s2_cfg;
    struct (anon) arm_v7s_cfg;
    struct (anon) arm_mali_lpae_cfg;
    struct (anon) apple_dart_cfg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct io_pgtable_cfg {
    long unsigned int quirks;
    long unsigned int pgsize_bitmap;
    unsigned int ias;
    unsigned int oas;
    bool coherent_walk;
    const struct iommu_flush_ops *tlb;
    struct device *iommu_dev;
    struct (anon) arm_lpae_s1_cfg;
    struct (anon) arm_lpae_s2_cfg;
    struct (anon) arm_v7s_cfg;
    struct (anon) arm_mali_lpae_cfg;
    struct (anon) apple_dart_cfg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct io_pgtable_cfg {
    long unsigned int quirks;
    long unsigned int pgsize_bitmap;
    unsigned int ias;
    unsigned int oas;
    bool coherent_walk;
    const struct iommu_flush_ops *tlb;
    struct device *iommu_dev;
    struct (anon) arm_lpae_s1_cfg;
    struct (anon) arm_lpae_s2_cfg;
    struct (anon) arm_v7s_cfg;
    struct (anon) arm_mali_lpae_cfg;
    struct (anon) apple_dart_cfg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct io_pgtable_cfg {
    long unsigned int quirks;
    long unsigned int pgsize_bitmap;
    unsigned int ias;
    unsigned int oas;
    bool coherent_walk;
    const struct iommu_flush_ops *tlb;
    struct device *iommu_dev;
    void * (*alloc)(void *, size_t, gfp_t);
    void (*free)(void *, void *, size_t);
    struct (anon) arm_lpae_s1_cfg;
    struct (anon) arm_lpae_s2_cfg;
    struct (anon) arm_v7s_cfg;
    struct (anon) arm_mali_lpae_cfg;
    struct (anon) apple_dart_cfg;
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
struct io_pgtable_cfg {
    long unsigned int quirks;
    long unsigned int pgsize_bitmap;
    unsigned int ias;
    unsigned int oas;
    bool coherent_walk;
    const struct iommu_flush_ops *tlb;
    struct device *iommu_dev;
    struct (anon) arm_lpae_s1_cfg;
    struct (anon) arm_lpae_s2_cfg;
    struct (anon) arm_v7s_cfg;
    struct (anon) arm_mali_lpae_cfg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct io_pgtable_cfg {
    long unsigned int quirks;
    long unsigned int pgsize_bitmap;
    unsigned int ias;
    unsigned int oas;
    bool coherent_walk;
    const struct iommu_flush_ops *tlb;
    struct device *iommu_dev;
    struct (anon) arm_lpae_s1_cfg;
    struct (anon) arm_lpae_s2_cfg;
    struct (anon) arm_v7s_cfg;
    struct (anon) arm_mali_lpae_cfg;
};
```
</details>
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
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct (anon) apple_dart_cfg</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void * (*alloc)(void *, size_t, gfp_t)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*free)(void *, void *, size_t)</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Arch</b>
<ul>
</ul>
