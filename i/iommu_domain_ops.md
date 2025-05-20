# Struct: <code>iommu_domain_ops</code>

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
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct iommu_domain_ops {
    int (*attach_dev)(struct iommu_domain *, struct device *);
    void (*detach_dev)(struct iommu_domain *, struct device *);
    int (*map)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, int, gfp_t);
    int (*map_pages)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, size_t, int, gfp_t, size_t *);
    size_t (*unmap)(struct iommu_domain *, long unsigned int, size_t, struct iommu_iotlb_gather *);
    size_t (*unmap_pages)(struct iommu_domain *, long unsigned int, size_t, size_t, struct iommu_iotlb_gather *);
    void (*flush_iotlb_all)(struct iommu_domain *);
    void (*iotlb_sync_map)(struct iommu_domain *, long unsigned int, size_t);
    void (*iotlb_sync)(struct iommu_domain *, struct iommu_iotlb_gather *);
    phys_addr_t (*iova_to_phys)(struct iommu_domain *, dma_addr_t);
    bool (*enforce_cache_coherency)(struct iommu_domain *);
    int (*enable_nesting)(struct iommu_domain *);
    int (*set_pgtable_quirks)(struct iommu_domain *, long unsigned int);
    void (*free)(struct iommu_domain *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct iommu_domain_ops {
    int (*attach_dev)(struct iommu_domain *, struct device *);
    void (*detach_dev)(struct iommu_domain *, struct device *);
    int (*set_dev_pasid)(struct iommu_domain *, struct device *, ioasid_t);
    int (*map)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, int, gfp_t);
    int (*map_pages)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, size_t, int, gfp_t, size_t *);
    size_t (*unmap)(struct iommu_domain *, long unsigned int, size_t, struct iommu_iotlb_gather *);
    size_t (*unmap_pages)(struct iommu_domain *, long unsigned int, size_t, size_t, struct iommu_iotlb_gather *);
    void (*flush_iotlb_all)(struct iommu_domain *);
    void (*iotlb_sync_map)(struct iommu_domain *, long unsigned int, size_t);
    void (*iotlb_sync)(struct iommu_domain *, struct iommu_iotlb_gather *);
    phys_addr_t (*iova_to_phys)(struct iommu_domain *, dma_addr_t);
    bool (*enforce_cache_coherency)(struct iommu_domain *);
    int (*enable_nesting)(struct iommu_domain *);
    int (*set_pgtable_quirks)(struct iommu_domain *, long unsigned int);
    void (*free)(struct iommu_domain *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct iommu_domain_ops {
    int (*attach_dev)(struct iommu_domain *, struct device *);
    int (*set_dev_pasid)(struct iommu_domain *, struct device *, ioasid_t);
    int (*map)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, int, gfp_t);
    int (*map_pages)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, size_t, int, gfp_t, size_t *);
    size_t (*unmap)(struct iommu_domain *, long unsigned int, size_t, struct iommu_iotlb_gather *);
    size_t (*unmap_pages)(struct iommu_domain *, long unsigned int, size_t, size_t, struct iommu_iotlb_gather *);
    void (*flush_iotlb_all)(struct iommu_domain *);
    void (*iotlb_sync_map)(struct iommu_domain *, long unsigned int, size_t);
    void (*iotlb_sync)(struct iommu_domain *, struct iommu_iotlb_gather *);
    phys_addr_t (*iova_to_phys)(struct iommu_domain *, dma_addr_t);
    bool (*enforce_cache_coherency)(struct iommu_domain *);
    int (*enable_nesting)(struct iommu_domain *);
    int (*set_pgtable_quirks)(struct iommu_domain *, long unsigned int);
    void (*free)(struct iommu_domain *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct iommu_domain_ops {
    int (*attach_dev)(struct iommu_domain *, struct device *);
    int (*set_dev_pasid)(struct iommu_domain *, struct device *, ioasid_t);
    int (*map_pages)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, size_t, int, gfp_t, size_t *);
    size_t (*unmap_pages)(struct iommu_domain *, long unsigned int, size_t, size_t, struct iommu_iotlb_gather *);
    void (*flush_iotlb_all)(struct iommu_domain *);
    int (*iotlb_sync_map)(struct iommu_domain *, long unsigned int, size_t);
    void (*iotlb_sync)(struct iommu_domain *, struct iommu_iotlb_gather *);
    int (*cache_invalidate_user)(struct iommu_domain *, struct iommu_user_data_array *);
    phys_addr_t (*iova_to_phys)(struct iommu_domain *, dma_addr_t);
    bool (*enforce_cache_coherency)(struct iommu_domain *);
    int (*enable_nesting)(struct iommu_domain *);
    int (*set_pgtable_quirks)(struct iommu_domain *, long unsigned int);
    void (*free)(struct iommu_domain *);
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
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*set_dev_pasid)(struct iommu_domain *, struct device *, ioasid_t)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>void (*detach_dev)(struct iommu_domain *, struct device *)</code>
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
<code>int (*cache_invalidate_user)(struct iommu_domain *, struct iommu_user_data_array *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*map)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, int, gfp_t)</code>
</li>
<li>
<b>Field removed. </b>
<code>size_t (*unmap)(struct iommu_domain *, long unsigned int, size_t, struct iommu_iotlb_gather *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*iotlb_sync_map)(struct iommu_domain *, long unsigned int, size_t)</code> ➡️ <code>int (*iotlb_sync_map)(struct iommu_domain *, long unsigned int, size_t)</code>
</li>
</ul>
</details>
</li>
</ul>
