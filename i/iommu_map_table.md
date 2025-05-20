# Struct: <code>iommu_map_table</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct iommu_map_table {
    long unsigned int table_map_base;
    long unsigned int table_shift;
    long unsigned int nr_pools;
    void (*lazy_flush)(struct iommu_map_table *);
    long unsigned int poolsize;
    struct iommu_pool pools[16];
    u32 flags;
    struct iommu_pool large_pool;
    long unsigned int *map;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct iommu_map_table {
    long unsigned int table_map_base;
    long unsigned int table_shift;
    long unsigned int nr_pools;
    void (*lazy_flush)(struct iommu_map_table *);
    long unsigned int poolsize;
    struct iommu_pool pools[16];
    u32 flags;
    struct iommu_pool large_pool;
    long unsigned int *map;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct iommu_map_table {
    long unsigned int table_map_base;
    long unsigned int table_shift;
    long unsigned int nr_pools;
    void (*lazy_flush)(struct iommu_map_table *);
    long unsigned int poolsize;
    struct iommu_pool pools[16];
    u32 flags;
    struct iommu_pool large_pool;
    long unsigned int *map;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct iommu_map_table {
    long unsigned int table_map_base;
    long unsigned int table_shift;
    long unsigned int nr_pools;
    void (*lazy_flush)(struct iommu_map_table *);
    long unsigned int poolsize;
    struct iommu_pool pools[16];
    u32 flags;
    struct iommu_pool large_pool;
    long unsigned int *map;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct iommu_map_table {
    long unsigned int table_map_base;
    long unsigned int table_shift;
    long unsigned int nr_pools;
    void (*lazy_flush)(struct iommu_map_table *);
    long unsigned int poolsize;
    struct iommu_pool pools[16];
    u32 flags;
    struct iommu_pool large_pool;
    long unsigned int *map;
};
```
</details>
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
No changes between <code>4.4</code> and <code>4.8</code> ✅
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
</ul>
