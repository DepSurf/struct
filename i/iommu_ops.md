# Struct: <code>iommu_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct iommu_ops {
    bool (*capable)(enum iommu_cap);
    struct iommu_domain * (*domain_alloc)(unsigned int);
    void (*domain_free)(struct iommu_domain *);
    int (*attach_dev)(struct iommu_domain *, struct device *);
    void (*detach_dev)(struct iommu_domain *, struct device *);
    int (*map)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, int);
    size_t (*unmap)(struct iommu_domain *, long unsigned int, size_t);
    size_t (*map_sg)(struct iommu_domain *, long unsigned int, struct scatterlist *, unsigned int, int);
    phys_addr_t (*iova_to_phys)(struct iommu_domain *, dma_addr_t);
    int (*add_device)(struct device *);
    void (*remove_device)(struct device *);
    struct iommu_group * (*device_group)(struct device *);
    int (*domain_get_attr)(struct iommu_domain *, enum iommu_attr, void *);
    int (*domain_set_attr)(struct iommu_domain *, enum iommu_attr, void *);
    void (*get_dm_regions)(struct device *, struct list_head *);
    void (*put_dm_regions)(struct device *, struct list_head *);
    int (*domain_window_enable)(struct iommu_domain *, u32, phys_addr_t, u64, int);
    void (*domain_window_disable)(struct iommu_domain *, u32);
    int (*domain_set_windows)(struct iommu_domain *, u32);
    u32 (*domain_get_windows)(struct iommu_domain *);
    long unsigned int pgsize_bitmap;
    void *priv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct iommu_ops {
    bool (*capable)(enum iommu_cap);
    struct iommu_domain * (*domain_alloc)(unsigned int);
    void (*domain_free)(struct iommu_domain *);
    int (*attach_dev)(struct iommu_domain *, struct device *);
    void (*detach_dev)(struct iommu_domain *, struct device *);
    int (*map)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, int);
    size_t (*unmap)(struct iommu_domain *, long unsigned int, size_t);
    size_t (*map_sg)(struct iommu_domain *, long unsigned int, struct scatterlist *, unsigned int, int);
    phys_addr_t (*iova_to_phys)(struct iommu_domain *, dma_addr_t);
    int (*add_device)(struct device *);
    void (*remove_device)(struct device *);
    struct iommu_group * (*device_group)(struct device *);
    int (*domain_get_attr)(struct iommu_domain *, enum iommu_attr, void *);
    int (*domain_set_attr)(struct iommu_domain *, enum iommu_attr, void *);
    void (*get_dm_regions)(struct device *, struct list_head *);
    void (*put_dm_regions)(struct device *, struct list_head *);
    void (*apply_dm_region)(struct device *, struct iommu_domain *, struct iommu_dm_region *);
    int (*domain_window_enable)(struct iommu_domain *, u32, phys_addr_t, u64, int);
    void (*domain_window_disable)(struct iommu_domain *, u32);
    int (*domain_set_windows)(struct iommu_domain *, u32);
    u32 (*domain_get_windows)(struct iommu_domain *);
    int (*of_xlate)(struct device *, struct of_phandle_args *);
    long unsigned int pgsize_bitmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct iommu_ops {
    bool (*capable)(enum iommu_cap);
    struct iommu_domain * (*domain_alloc)(unsigned int);
    void (*domain_free)(struct iommu_domain *);
    int (*attach_dev)(struct iommu_domain *, struct device *);
    void (*detach_dev)(struct iommu_domain *, struct device *);
    int (*map)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, int);
    size_t (*unmap)(struct iommu_domain *, long unsigned int, size_t);
    size_t (*map_sg)(struct iommu_domain *, long unsigned int, struct scatterlist *, unsigned int, int);
    phys_addr_t (*iova_to_phys)(struct iommu_domain *, dma_addr_t);
    int (*add_device)(struct device *);
    void (*remove_device)(struct device *);
    struct iommu_group * (*device_group)(struct device *);
    int (*domain_get_attr)(struct iommu_domain *, enum iommu_attr, void *);
    int (*domain_set_attr)(struct iommu_domain *, enum iommu_attr, void *);
    void (*get_resv_regions)(struct device *, struct list_head *);
    void (*put_resv_regions)(struct device *, struct list_head *);
    void (*apply_resv_region)(struct device *, struct iommu_domain *, struct iommu_resv_region *);
    int (*domain_window_enable)(struct iommu_domain *, u32, phys_addr_t, u64, int);
    void (*domain_window_disable)(struct iommu_domain *, u32);
    int (*domain_set_windows)(struct iommu_domain *, u32);
    u32 (*domain_get_windows)(struct iommu_domain *);
    int (*of_xlate)(struct device *, struct of_phandle_args *);
    long unsigned int pgsize_bitmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct iommu_ops {
    bool (*capable)(enum iommu_cap);
    struct iommu_domain * (*domain_alloc)(unsigned int);
    void (*domain_free)(struct iommu_domain *);
    int (*attach_dev)(struct iommu_domain *, struct device *);
    void (*detach_dev)(struct iommu_domain *, struct device *);
    int (*map)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, int);
    size_t (*unmap)(struct iommu_domain *, long unsigned int, size_t);
    size_t (*map_sg)(struct iommu_domain *, long unsigned int, struct scatterlist *, unsigned int, int);
    phys_addr_t (*iova_to_phys)(struct iommu_domain *, dma_addr_t);
    int (*add_device)(struct device *);
    void (*remove_device)(struct device *);
    struct iommu_group * (*device_group)(struct device *);
    int (*domain_get_attr)(struct iommu_domain *, enum iommu_attr, void *);
    int (*domain_set_attr)(struct iommu_domain *, enum iommu_attr, void *);
    void (*get_resv_regions)(struct device *, struct list_head *);
    void (*put_resv_regions)(struct device *, struct list_head *);
    void (*apply_resv_region)(struct device *, struct iommu_domain *, struct iommu_resv_region *);
    int (*domain_window_enable)(struct iommu_domain *, u32, phys_addr_t, u64, int);
    void (*domain_window_disable)(struct iommu_domain *, u32);
    int (*domain_set_windows)(struct iommu_domain *, u32);
    u32 (*domain_get_windows)(struct iommu_domain *);
    int (*of_xlate)(struct device *, struct of_phandle_args *);
    long unsigned int pgsize_bitmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct iommu_ops {
    bool (*capable)(enum iommu_cap);
    struct iommu_domain * (*domain_alloc)(unsigned int);
    void (*domain_free)(struct iommu_domain *);
    int (*attach_dev)(struct iommu_domain *, struct device *);
    void (*detach_dev)(struct iommu_domain *, struct device *);
    int (*map)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, int);
    size_t (*unmap)(struct iommu_domain *, long unsigned int, size_t);
    size_t (*map_sg)(struct iommu_domain *, long unsigned int, struct scatterlist *, unsigned int, int);
    void (*flush_iotlb_all)(struct iommu_domain *);
    void (*iotlb_range_add)(struct iommu_domain *, long unsigned int, size_t);
    void (*iotlb_sync)(struct iommu_domain *);
    phys_addr_t (*iova_to_phys)(struct iommu_domain *, dma_addr_t);
    int (*add_device)(struct device *);
    void (*remove_device)(struct device *);
    struct iommu_group * (*device_group)(struct device *);
    int (*domain_get_attr)(struct iommu_domain *, enum iommu_attr, void *);
    int (*domain_set_attr)(struct iommu_domain *, enum iommu_attr, void *);
    void (*get_resv_regions)(struct device *, struct list_head *);
    void (*put_resv_regions)(struct device *, struct list_head *);
    void (*apply_resv_region)(struct device *, struct iommu_domain *, struct iommu_resv_region *);
    int (*domain_window_enable)(struct iommu_domain *, u32, phys_addr_t, u64, int);
    void (*domain_window_disable)(struct iommu_domain *, u32);
    int (*domain_set_windows)(struct iommu_domain *, u32);
    u32 (*domain_get_windows)(struct iommu_domain *);
    int (*of_xlate)(struct device *, struct of_phandle_args *);
    bool (*is_attach_deferred)(struct iommu_domain *, struct device *);
    long unsigned int pgsize_bitmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct iommu_ops {
    bool (*capable)(enum iommu_cap);
    struct iommu_domain * (*domain_alloc)(unsigned int);
    void (*domain_free)(struct iommu_domain *);
    int (*attach_dev)(struct iommu_domain *, struct device *);
    void (*detach_dev)(struct iommu_domain *, struct device *);
    int (*map)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, int);
    size_t (*unmap)(struct iommu_domain *, long unsigned int, size_t);
    size_t (*map_sg)(struct iommu_domain *, long unsigned int, struct scatterlist *, unsigned int, int);
    void (*flush_iotlb_all)(struct iommu_domain *);
    void (*iotlb_range_add)(struct iommu_domain *, long unsigned int, size_t);
    void (*iotlb_sync)(struct iommu_domain *);
    phys_addr_t (*iova_to_phys)(struct iommu_domain *, dma_addr_t);
    int (*add_device)(struct device *);
    void (*remove_device)(struct device *);
    struct iommu_group * (*device_group)(struct device *);
    int (*domain_get_attr)(struct iommu_domain *, enum iommu_attr, void *);
    int (*domain_set_attr)(struct iommu_domain *, enum iommu_attr, void *);
    void (*get_resv_regions)(struct device *, struct list_head *);
    void (*put_resv_regions)(struct device *, struct list_head *);
    void (*apply_resv_region)(struct device *, struct iommu_domain *, struct iommu_resv_region *);
    int (*domain_window_enable)(struct iommu_domain *, u32, phys_addr_t, u64, int);
    void (*domain_window_disable)(struct iommu_domain *, u32);
    int (*domain_set_windows)(struct iommu_domain *, u32);
    u32 (*domain_get_windows)(struct iommu_domain *);
    int (*of_xlate)(struct device *, struct of_phandle_args *);
    bool (*is_attach_deferred)(struct iommu_domain *, struct device *);
    long unsigned int pgsize_bitmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct iommu_ops {
    bool (*capable)(enum iommu_cap);
    struct iommu_domain * (*domain_alloc)(unsigned int);
    void (*domain_free)(struct iommu_domain *);
    int (*attach_dev)(struct iommu_domain *, struct device *);
    void (*detach_dev)(struct iommu_domain *, struct device *);
    int (*map)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, int);
    size_t (*unmap)(struct iommu_domain *, long unsigned int, size_t);
    void (*flush_iotlb_all)(struct iommu_domain *);
    void (*iotlb_range_add)(struct iommu_domain *, long unsigned int, size_t);
    void (*iotlb_sync)(struct iommu_domain *);
    phys_addr_t (*iova_to_phys)(struct iommu_domain *, dma_addr_t);
    int (*add_device)(struct device *);
    void (*remove_device)(struct device *);
    struct iommu_group * (*device_group)(struct device *);
    int (*domain_get_attr)(struct iommu_domain *, enum iommu_attr, void *);
    int (*domain_set_attr)(struct iommu_domain *, enum iommu_attr, void *);
    void (*get_resv_regions)(struct device *, struct list_head *);
    void (*put_resv_regions)(struct device *, struct list_head *);
    void (*apply_resv_region)(struct device *, struct iommu_domain *, struct iommu_resv_region *);
    int (*domain_window_enable)(struct iommu_domain *, u32, phys_addr_t, u64, int);
    void (*domain_window_disable)(struct iommu_domain *, u32);
    int (*of_xlate)(struct device *, struct of_phandle_args *);
    bool (*is_attach_deferred)(struct iommu_domain *, struct device *);
    long unsigned int pgsize_bitmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct iommu_ops {
    bool (*capable)(enum iommu_cap);
    struct iommu_domain * (*domain_alloc)(unsigned int);
    void (*domain_free)(struct iommu_domain *);
    int (*attach_dev)(struct iommu_domain *, struct device *);
    void (*detach_dev)(struct iommu_domain *, struct device *);
    int (*map)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, int);
    size_t (*unmap)(struct iommu_domain *, long unsigned int, size_t);
    void (*flush_iotlb_all)(struct iommu_domain *);
    void (*iotlb_range_add)(struct iommu_domain *, long unsigned int, size_t);
    void (*iotlb_sync_map)(struct iommu_domain *);
    void (*iotlb_sync)(struct iommu_domain *);
    phys_addr_t (*iova_to_phys)(struct iommu_domain *, dma_addr_t);
    int (*add_device)(struct device *);
    void (*remove_device)(struct device *);
    struct iommu_group * (*device_group)(struct device *);
    int (*domain_get_attr)(struct iommu_domain *, enum iommu_attr, void *);
    int (*domain_set_attr)(struct iommu_domain *, enum iommu_attr, void *);
    void (*get_resv_regions)(struct device *, struct list_head *);
    void (*put_resv_regions)(struct device *, struct list_head *);
    void (*apply_resv_region)(struct device *, struct iommu_domain *, struct iommu_resv_region *);
    int (*domain_window_enable)(struct iommu_domain *, u32, phys_addr_t, u64, int);
    void (*domain_window_disable)(struct iommu_domain *, u32);
    int (*of_xlate)(struct device *, struct of_phandle_args *);
    bool (*is_attach_deferred)(struct iommu_domain *, struct device *);
    bool (*dev_has_feat)(struct device *, enum iommu_dev_features);
    bool (*dev_feat_enabled)(struct device *, enum iommu_dev_features);
    int (*dev_enable_feat)(struct device *, enum iommu_dev_features);
    int (*dev_disable_feat)(struct device *, enum iommu_dev_features);
    int (*aux_attach_dev)(struct iommu_domain *, struct device *);
    void (*aux_detach_dev)(struct iommu_domain *, struct device *);
    int (*aux_get_pasid)(struct iommu_domain *, struct device *);
    struct iommu_sva * (*sva_bind)(struct device *, struct mm_struct *, void *);
    void (*sva_unbind)(struct iommu_sva *);
    int (*sva_get_pasid)(struct iommu_sva *);
    int (*page_response)(struct device *, struct iommu_fault_event *, struct iommu_page_response *);
    long unsigned int pgsize_bitmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct iommu_ops {
    bool (*capable)(enum iommu_cap);
    struct iommu_domain * (*domain_alloc)(unsigned int);
    void (*domain_free)(struct iommu_domain *);
    int (*attach_dev)(struct iommu_domain *, struct device *);
    void (*detach_dev)(struct iommu_domain *, struct device *);
    int (*map)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, int);
    size_t (*unmap)(struct iommu_domain *, long unsigned int, size_t, struct iommu_iotlb_gather *);
    void (*flush_iotlb_all)(struct iommu_domain *);
    void (*iotlb_sync_map)(struct iommu_domain *);
    void (*iotlb_sync)(struct iommu_domain *, struct iommu_iotlb_gather *);
    phys_addr_t (*iova_to_phys)(struct iommu_domain *, dma_addr_t);
    int (*add_device)(struct device *);
    void (*remove_device)(struct device *);
    struct iommu_group * (*device_group)(struct device *);
    int (*domain_get_attr)(struct iommu_domain *, enum iommu_attr, void *);
    int (*domain_set_attr)(struct iommu_domain *, enum iommu_attr, void *);
    void (*get_resv_regions)(struct device *, struct list_head *);
    void (*put_resv_regions)(struct device *, struct list_head *);
    void (*apply_resv_region)(struct device *, struct iommu_domain *, struct iommu_resv_region *);
    int (*domain_window_enable)(struct iommu_domain *, u32, phys_addr_t, u64, int);
    void (*domain_window_disable)(struct iommu_domain *, u32);
    int (*of_xlate)(struct device *, struct of_phandle_args *);
    bool (*is_attach_deferred)(struct iommu_domain *, struct device *);
    bool (*dev_has_feat)(struct device *, enum iommu_dev_features);
    bool (*dev_feat_enabled)(struct device *, enum iommu_dev_features);
    int (*dev_enable_feat)(struct device *, enum iommu_dev_features);
    int (*dev_disable_feat)(struct device *, enum iommu_dev_features);
    int (*aux_attach_dev)(struct iommu_domain *, struct device *);
    void (*aux_detach_dev)(struct iommu_domain *, struct device *);
    int (*aux_get_pasid)(struct iommu_domain *, struct device *);
    struct iommu_sva * (*sva_bind)(struct device *, struct mm_struct *, void *);
    void (*sva_unbind)(struct iommu_sva *);
    int (*sva_get_pasid)(struct iommu_sva *);
    int (*page_response)(struct device *, struct iommu_fault_event *, struct iommu_page_response *);
    long unsigned int pgsize_bitmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct iommu_ops {
    bool (*capable)(enum iommu_cap);
    struct iommu_domain * (*domain_alloc)(unsigned int);
    void (*domain_free)(struct iommu_domain *);
    int (*attach_dev)(struct iommu_domain *, struct device *);
    void (*detach_dev)(struct iommu_domain *, struct device *);
    int (*map)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, int, gfp_t);
    size_t (*unmap)(struct iommu_domain *, long unsigned int, size_t, struct iommu_iotlb_gather *);
    void (*flush_iotlb_all)(struct iommu_domain *);
    void (*iotlb_sync_map)(struct iommu_domain *);
    void (*iotlb_sync)(struct iommu_domain *, struct iommu_iotlb_gather *);
    phys_addr_t (*iova_to_phys)(struct iommu_domain *, dma_addr_t);
    struct iommu_device * (*probe_device)(struct device *);
    void (*release_device)(struct device *);
    void (*probe_finalize)(struct device *);
    struct iommu_group * (*device_group)(struct device *);
    int (*domain_get_attr)(struct iommu_domain *, enum iommu_attr, void *);
    int (*domain_set_attr)(struct iommu_domain *, enum iommu_attr, void *);
    void (*get_resv_regions)(struct device *, struct list_head *);
    void (*put_resv_regions)(struct device *, struct list_head *);
    void (*apply_resv_region)(struct device *, struct iommu_domain *, struct iommu_resv_region *);
    int (*domain_window_enable)(struct iommu_domain *, u32, phys_addr_t, u64, int);
    void (*domain_window_disable)(struct iommu_domain *, u32);
    int (*of_xlate)(struct device *, struct of_phandle_args *);
    bool (*is_attach_deferred)(struct iommu_domain *, struct device *);
    bool (*dev_has_feat)(struct device *, enum iommu_dev_features);
    bool (*dev_feat_enabled)(struct device *, enum iommu_dev_features);
    int (*dev_enable_feat)(struct device *, enum iommu_dev_features);
    int (*dev_disable_feat)(struct device *, enum iommu_dev_features);
    int (*aux_attach_dev)(struct iommu_domain *, struct device *);
    void (*aux_detach_dev)(struct iommu_domain *, struct device *);
    int (*aux_get_pasid)(struct iommu_domain *, struct device *);
    struct iommu_sva * (*sva_bind)(struct device *, struct mm_struct *, void *);
    void (*sva_unbind)(struct iommu_sva *);
    int (*sva_get_pasid)(struct iommu_sva *);
    int (*page_response)(struct device *, struct iommu_fault_event *, struct iommu_page_response *);
    int (*cache_invalidate)(struct iommu_domain *, struct device *, struct iommu_cache_invalidate_info *);
    int (*sva_bind_gpasid)(struct iommu_domain *, struct device *, struct iommu_gpasid_bind_data *);
    int (*sva_unbind_gpasid)(struct device *, int);
    int (*def_domain_type)(struct device *);
    long unsigned int pgsize_bitmap;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct iommu_ops {
    bool (*capable)(enum iommu_cap);
    struct iommu_domain * (*domain_alloc)(unsigned int);
    void (*domain_free)(struct iommu_domain *);
    int (*attach_dev)(struct iommu_domain *, struct device *);
    void (*detach_dev)(struct iommu_domain *, struct device *);
    int (*map)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, int, gfp_t);
    size_t (*unmap)(struct iommu_domain *, long unsigned int, size_t, struct iommu_iotlb_gather *);
    void (*flush_iotlb_all)(struct iommu_domain *);
    void (*iotlb_sync_map)(struct iommu_domain *);
    void (*iotlb_sync)(struct iommu_domain *, struct iommu_iotlb_gather *);
    phys_addr_t (*iova_to_phys)(struct iommu_domain *, dma_addr_t);
    struct iommu_device * (*probe_device)(struct device *);
    void (*release_device)(struct device *);
    void (*probe_finalize)(struct device *);
    struct iommu_group * (*device_group)(struct device *);
    int (*domain_get_attr)(struct iommu_domain *, enum iommu_attr, void *);
    int (*domain_set_attr)(struct iommu_domain *, enum iommu_attr, void *);
    void (*get_resv_regions)(struct device *, struct list_head *);
    void (*put_resv_regions)(struct device *, struct list_head *);
    void (*apply_resv_region)(struct device *, struct iommu_domain *, struct iommu_resv_region *);
    int (*domain_window_enable)(struct iommu_domain *, u32, phys_addr_t, u64, int);
    void (*domain_window_disable)(struct iommu_domain *, u32);
    int (*of_xlate)(struct device *, struct of_phandle_args *);
    bool (*is_attach_deferred)(struct iommu_domain *, struct device *);
    bool (*dev_has_feat)(struct device *, enum iommu_dev_features);
    bool (*dev_feat_enabled)(struct device *, enum iommu_dev_features);
    int (*dev_enable_feat)(struct device *, enum iommu_dev_features);
    int (*dev_disable_feat)(struct device *, enum iommu_dev_features);
    int (*aux_attach_dev)(struct iommu_domain *, struct device *);
    void (*aux_detach_dev)(struct iommu_domain *, struct device *);
    int (*aux_get_pasid)(struct iommu_domain *, struct device *);
    struct iommu_sva * (*sva_bind)(struct device *, struct mm_struct *, void *);
    void (*sva_unbind)(struct iommu_sva *);
    u32 (*sva_get_pasid)(struct iommu_sva *);
    int (*page_response)(struct device *, struct iommu_fault_event *, struct iommu_page_response *);
    int (*cache_invalidate)(struct iommu_domain *, struct device *, struct iommu_cache_invalidate_info *);
    int (*sva_bind_gpasid)(struct iommu_domain *, struct device *, struct iommu_gpasid_bind_data *);
    int (*sva_unbind_gpasid)(struct device *, u32);
    int (*def_domain_type)(struct device *);
    long unsigned int pgsize_bitmap;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct iommu_ops {
    bool (*capable)(enum iommu_cap);
    struct iommu_domain * (*domain_alloc)(unsigned int);
    void (*domain_free)(struct iommu_domain *);
    int (*attach_dev)(struct iommu_domain *, struct device *);
    void (*detach_dev)(struct iommu_domain *, struct device *);
    int (*map)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, int, gfp_t);
    size_t (*unmap)(struct iommu_domain *, long unsigned int, size_t, struct iommu_iotlb_gather *);
    void (*flush_iotlb_all)(struct iommu_domain *);
    void (*iotlb_sync_map)(struct iommu_domain *, long unsigned int, size_t);
    void (*iotlb_sync)(struct iommu_domain *, struct iommu_iotlb_gather *);
    phys_addr_t (*iova_to_phys)(struct iommu_domain *, dma_addr_t);
    struct iommu_device * (*probe_device)(struct device *);
    void (*release_device)(struct device *);
    void (*probe_finalize)(struct device *);
    struct iommu_group * (*device_group)(struct device *);
    int (*enable_nesting)(struct iommu_domain *);
    int (*set_pgtable_quirks)(struct iommu_domain *, long unsigned int);
    void (*get_resv_regions)(struct device *, struct list_head *);
    void (*put_resv_regions)(struct device *, struct list_head *);
    void (*apply_resv_region)(struct device *, struct iommu_domain *, struct iommu_resv_region *);
    int (*of_xlate)(struct device *, struct of_phandle_args *);
    bool (*is_attach_deferred)(struct iommu_domain *, struct device *);
    bool (*dev_has_feat)(struct device *, enum iommu_dev_features);
    bool (*dev_feat_enabled)(struct device *, enum iommu_dev_features);
    int (*dev_enable_feat)(struct device *, enum iommu_dev_features);
    int (*dev_disable_feat)(struct device *, enum iommu_dev_features);
    int (*aux_attach_dev)(struct iommu_domain *, struct device *);
    void (*aux_detach_dev)(struct iommu_domain *, struct device *);
    int (*aux_get_pasid)(struct iommu_domain *, struct device *);
    struct iommu_sva * (*sva_bind)(struct device *, struct mm_struct *, void *);
    void (*sva_unbind)(struct iommu_sva *);
    u32 (*sva_get_pasid)(struct iommu_sva *);
    int (*page_response)(struct device *, struct iommu_fault_event *, struct iommu_page_response *);
    int (*cache_invalidate)(struct iommu_domain *, struct device *, struct iommu_cache_invalidate_info *);
    int (*sva_bind_gpasid)(struct iommu_domain *, struct device *, struct iommu_gpasid_bind_data *);
    int (*sva_unbind_gpasid)(struct device *, u32);
    int (*def_domain_type)(struct device *);
    long unsigned int pgsize_bitmap;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct iommu_ops {
    bool (*capable)(enum iommu_cap);
    struct iommu_domain * (*domain_alloc)(unsigned int);
    void (*domain_free)(struct iommu_domain *);
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
    struct iommu_device * (*probe_device)(struct device *);
    void (*release_device)(struct device *);
    void (*probe_finalize)(struct device *);
    struct iommu_group * (*device_group)(struct device *);
    int (*enable_nesting)(struct iommu_domain *);
    int (*set_pgtable_quirks)(struct iommu_domain *, long unsigned int);
    void (*get_resv_regions)(struct device *, struct list_head *);
    void (*put_resv_regions)(struct device *, struct list_head *);
    void (*apply_resv_region)(struct device *, struct iommu_domain *, struct iommu_resv_region *);
    int (*of_xlate)(struct device *, struct of_phandle_args *);
    bool (*is_attach_deferred)(struct iommu_domain *, struct device *);
    bool (*dev_has_feat)(struct device *, enum iommu_dev_features);
    bool (*dev_feat_enabled)(struct device *, enum iommu_dev_features);
    int (*dev_enable_feat)(struct device *, enum iommu_dev_features);
    int (*dev_disable_feat)(struct device *, enum iommu_dev_features);
    int (*aux_attach_dev)(struct iommu_domain *, struct device *);
    void (*aux_detach_dev)(struct iommu_domain *, struct device *);
    int (*aux_get_pasid)(struct iommu_domain *, struct device *);
    struct iommu_sva * (*sva_bind)(struct device *, struct mm_struct *, void *);
    void (*sva_unbind)(struct iommu_sva *);
    u32 (*sva_get_pasid)(struct iommu_sva *);
    int (*page_response)(struct device *, struct iommu_fault_event *, struct iommu_page_response *);
    int (*cache_invalidate)(struct iommu_domain *, struct device *, struct iommu_cache_invalidate_info *);
    int (*sva_bind_gpasid)(struct iommu_domain *, struct device *, struct iommu_gpasid_bind_data *);
    int (*sva_unbind_gpasid)(struct device *, u32);
    int (*def_domain_type)(struct device *);
    long unsigned int pgsize_bitmap;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct iommu_ops {
    bool (*capable)(enum iommu_cap);
    struct iommu_domain * (*domain_alloc)(unsigned int);
    struct iommu_device * (*probe_device)(struct device *);
    void (*release_device)(struct device *);
    void (*probe_finalize)(struct device *);
    struct iommu_group * (*device_group)(struct device *);
    void (*get_resv_regions)(struct device *, struct list_head *);
    void (*put_resv_regions)(struct device *, struct list_head *);
    int (*of_xlate)(struct device *, struct of_phandle_args *);
    bool (*is_attach_deferred)(struct device *);
    bool (*dev_has_feat)(struct device *, enum iommu_dev_features);
    bool (*dev_feat_enabled)(struct device *, enum iommu_dev_features);
    int (*dev_enable_feat)(struct device *, enum iommu_dev_features);
    int (*dev_disable_feat)(struct device *, enum iommu_dev_features);
    struct iommu_sva * (*sva_bind)(struct device *, struct mm_struct *, void *);
    void (*sva_unbind)(struct iommu_sva *);
    u32 (*sva_get_pasid)(struct iommu_sva *);
    int (*page_response)(struct device *, struct iommu_fault_event *, struct iommu_page_response *);
    int (*def_domain_type)(struct device *);
    const struct iommu_domain_ops *default_domain_ops;
    long unsigned int pgsize_bitmap;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct iommu_ops {
    bool (*capable)(struct device *, enum iommu_cap);
    struct iommu_domain * (*domain_alloc)(unsigned int);
    struct iommu_device * (*probe_device)(struct device *);
    void (*release_device)(struct device *);
    void (*probe_finalize)(struct device *);
    struct iommu_group * (*device_group)(struct device *);
    void (*get_resv_regions)(struct device *, struct list_head *);
    int (*of_xlate)(struct device *, struct of_phandle_args *);
    bool (*is_attach_deferred)(struct device *);
    int (*dev_enable_feat)(struct device *, enum iommu_dev_features);
    int (*dev_disable_feat)(struct device *, enum iommu_dev_features);
    int (*page_response)(struct device *, struct iommu_fault_event *, struct iommu_page_response *);
    int (*def_domain_type)(struct device *);
    void (*remove_dev_pasid)(struct device *, ioasid_t);
    const struct iommu_domain_ops *default_domain_ops;
    long unsigned int pgsize_bitmap;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct iommu_ops {
    bool (*capable)(struct device *, enum iommu_cap);
    struct iommu_domain * (*domain_alloc)(unsigned int);
    struct iommu_device * (*probe_device)(struct device *);
    void (*release_device)(struct device *);
    void (*probe_finalize)(struct device *);
    void (*set_platform_dma_ops)(struct device *);
    struct iommu_group * (*device_group)(struct device *);
    void (*get_resv_regions)(struct device *, struct list_head *);
    int (*of_xlate)(struct device *, struct of_phandle_args *);
    bool (*is_attach_deferred)(struct device *);
    int (*dev_enable_feat)(struct device *, enum iommu_dev_features);
    int (*dev_disable_feat)(struct device *, enum iommu_dev_features);
    int (*page_response)(struct device *, struct iommu_fault_event *, struct iommu_page_response *);
    int (*def_domain_type)(struct device *);
    void (*remove_dev_pasid)(struct device *, ioasid_t);
    const struct iommu_domain_ops *default_domain_ops;
    long unsigned int pgsize_bitmap;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct iommu_ops {
    bool (*capable)(struct device *, enum iommu_cap);
    void * (*hw_info)(struct device *, u32 *, u32 *);
    struct iommu_domain * (*domain_alloc)(unsigned int);
    struct iommu_domain * (*domain_alloc_user)(struct device *, u32, struct iommu_domain *, const struct iommu_user_data *);
    struct iommu_domain * (*domain_alloc_paging)(struct device *);
    struct iommu_device * (*probe_device)(struct device *);
    void (*release_device)(struct device *);
    void (*probe_finalize)(struct device *);
    struct iommu_group * (*device_group)(struct device *);
    void (*get_resv_regions)(struct device *, struct list_head *);
    int (*of_xlate)(struct device *, struct of_phandle_args *);
    bool (*is_attach_deferred)(struct device *);
    int (*dev_enable_feat)(struct device *, enum iommu_dev_features);
    int (*dev_disable_feat)(struct device *, enum iommu_dev_features);
    int (*page_response)(struct device *, struct iommu_fault_event *, struct iommu_page_response *);
    int (*def_domain_type)(struct device *);
    void (*remove_dev_pasid)(struct device *, ioasid_t);
    const struct iommu_domain_ops *default_domain_ops;
    long unsigned int pgsize_bitmap;
    struct module *owner;
    struct iommu_domain *identity_domain;
    struct iommu_domain *blocked_domain;
    struct iommu_domain *default_domain;
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
struct iommu_ops {
    bool (*capable)(enum iommu_cap);
    struct iommu_domain * (*domain_alloc)(unsigned int);
    void (*domain_free)(struct iommu_domain *);
    int (*attach_dev)(struct iommu_domain *, struct device *);
    void (*detach_dev)(struct iommu_domain *, struct device *);
    int (*map)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, int);
    size_t (*unmap)(struct iommu_domain *, long unsigned int, size_t, struct iommu_iotlb_gather *);
    void (*flush_iotlb_all)(struct iommu_domain *);
    void (*iotlb_sync_map)(struct iommu_domain *);
    void (*iotlb_sync)(struct iommu_domain *, struct iommu_iotlb_gather *);
    phys_addr_t (*iova_to_phys)(struct iommu_domain *, dma_addr_t);
    int (*add_device)(struct device *);
    void (*remove_device)(struct device *);
    struct iommu_group * (*device_group)(struct device *);
    int (*domain_get_attr)(struct iommu_domain *, enum iommu_attr, void *);
    int (*domain_set_attr)(struct iommu_domain *, enum iommu_attr, void *);
    void (*get_resv_regions)(struct device *, struct list_head *);
    void (*put_resv_regions)(struct device *, struct list_head *);
    void (*apply_resv_region)(struct device *, struct iommu_domain *, struct iommu_resv_region *);
    int (*domain_window_enable)(struct iommu_domain *, u32, phys_addr_t, u64, int);
    void (*domain_window_disable)(struct iommu_domain *, u32);
    int (*of_xlate)(struct device *, struct of_phandle_args *);
    bool (*is_attach_deferred)(struct iommu_domain *, struct device *);
    bool (*dev_has_feat)(struct device *, enum iommu_dev_features);
    bool (*dev_feat_enabled)(struct device *, enum iommu_dev_features);
    int (*dev_enable_feat)(struct device *, enum iommu_dev_features);
    int (*dev_disable_feat)(struct device *, enum iommu_dev_features);
    int (*aux_attach_dev)(struct iommu_domain *, struct device *);
    void (*aux_detach_dev)(struct iommu_domain *, struct device *);
    int (*aux_get_pasid)(struct iommu_domain *, struct device *);
    struct iommu_sva * (*sva_bind)(struct device *, struct mm_struct *, void *);
    void (*sva_unbind)(struct iommu_sva *);
    int (*sva_get_pasid)(struct iommu_sva *);
    int (*page_response)(struct device *, struct iommu_fault_event *, struct iommu_page_response *);
    long unsigned int pgsize_bitmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct iommu_ops {
    bool (*capable)(enum iommu_cap);
    struct iommu_domain * (*domain_alloc)(unsigned int);
    void (*domain_free)(struct iommu_domain *);
    int (*attach_dev)(struct iommu_domain *, struct device *);
    void (*detach_dev)(struct iommu_domain *, struct device *);
    int (*map)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, int);
    size_t (*unmap)(struct iommu_domain *, long unsigned int, size_t, struct iommu_iotlb_gather *);
    void (*flush_iotlb_all)(struct iommu_domain *);
    void (*iotlb_sync_map)(struct iommu_domain *);
    void (*iotlb_sync)(struct iommu_domain *, struct iommu_iotlb_gather *);
    phys_addr_t (*iova_to_phys)(struct iommu_domain *, dma_addr_t);
    int (*add_device)(struct device *);
    void (*remove_device)(struct device *);
    struct iommu_group * (*device_group)(struct device *);
    int (*domain_get_attr)(struct iommu_domain *, enum iommu_attr, void *);
    int (*domain_set_attr)(struct iommu_domain *, enum iommu_attr, void *);
    void (*get_resv_regions)(struct device *, struct list_head *);
    void (*put_resv_regions)(struct device *, struct list_head *);
    void (*apply_resv_region)(struct device *, struct iommu_domain *, struct iommu_resv_region *);
    int (*domain_window_enable)(struct iommu_domain *, u32, phys_addr_t, u64, int);
    void (*domain_window_disable)(struct iommu_domain *, u32);
    int (*of_xlate)(struct device *, struct of_phandle_args *);
    bool (*is_attach_deferred)(struct iommu_domain *, struct device *);
    bool (*dev_has_feat)(struct device *, enum iommu_dev_features);
    bool (*dev_feat_enabled)(struct device *, enum iommu_dev_features);
    int (*dev_enable_feat)(struct device *, enum iommu_dev_features);
    int (*dev_disable_feat)(struct device *, enum iommu_dev_features);
    int (*aux_attach_dev)(struct iommu_domain *, struct device *);
    void (*aux_detach_dev)(struct iommu_domain *, struct device *);
    int (*aux_get_pasid)(struct iommu_domain *, struct device *);
    struct iommu_sva * (*sva_bind)(struct device *, struct mm_struct *, void *);
    void (*sva_unbind)(struct iommu_sva *);
    int (*sva_get_pasid)(struct iommu_sva *);
    int (*page_response)(struct device *, struct iommu_fault_event *, struct iommu_page_response *);
    long unsigned int pgsize_bitmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct iommu_ops {
    bool (*capable)(enum iommu_cap);
    struct iommu_domain * (*domain_alloc)(unsigned int);
    void (*domain_free)(struct iommu_domain *);
    int (*attach_dev)(struct iommu_domain *, struct device *);
    void (*detach_dev)(struct iommu_domain *, struct device *);
    int (*map)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, int);
    size_t (*unmap)(struct iommu_domain *, long unsigned int, size_t, struct iommu_iotlb_gather *);
    void (*flush_iotlb_all)(struct iommu_domain *);
    void (*iotlb_sync_map)(struct iommu_domain *);
    void (*iotlb_sync)(struct iommu_domain *, struct iommu_iotlb_gather *);
    phys_addr_t (*iova_to_phys)(struct iommu_domain *, dma_addr_t);
    int (*add_device)(struct device *);
    void (*remove_device)(struct device *);
    struct iommu_group * (*device_group)(struct device *);
    int (*domain_get_attr)(struct iommu_domain *, enum iommu_attr, void *);
    int (*domain_set_attr)(struct iommu_domain *, enum iommu_attr, void *);
    void (*get_resv_regions)(struct device *, struct list_head *);
    void (*put_resv_regions)(struct device *, struct list_head *);
    void (*apply_resv_region)(struct device *, struct iommu_domain *, struct iommu_resv_region *);
    int (*domain_window_enable)(struct iommu_domain *, u32, phys_addr_t, u64, int);
    void (*domain_window_disable)(struct iommu_domain *, u32);
    int (*of_xlate)(struct device *, struct of_phandle_args *);
    bool (*is_attach_deferred)(struct iommu_domain *, struct device *);
    bool (*dev_has_feat)(struct device *, enum iommu_dev_features);
    bool (*dev_feat_enabled)(struct device *, enum iommu_dev_features);
    int (*dev_enable_feat)(struct device *, enum iommu_dev_features);
    int (*dev_disable_feat)(struct device *, enum iommu_dev_features);
    int (*aux_attach_dev)(struct iommu_domain *, struct device *);
    void (*aux_detach_dev)(struct iommu_domain *, struct device *);
    int (*aux_get_pasid)(struct iommu_domain *, struct device *);
    struct iommu_sva * (*sva_bind)(struct device *, struct mm_struct *, void *);
    void (*sva_unbind)(struct iommu_sva *);
    int (*sva_get_pasid)(struct iommu_sva *);
    int (*page_response)(struct device *, struct iommu_fault_event *, struct iommu_page_response *);
    long unsigned int pgsize_bitmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct iommu_ops {
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
struct iommu_ops {
    bool (*capable)(enum iommu_cap);
    struct iommu_domain * (*domain_alloc)(unsigned int);
    void (*domain_free)(struct iommu_domain *);
    int (*attach_dev)(struct iommu_domain *, struct device *);
    void (*detach_dev)(struct iommu_domain *, struct device *);
    int (*map)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, int);
    size_t (*unmap)(struct iommu_domain *, long unsigned int, size_t, struct iommu_iotlb_gather *);
    void (*flush_iotlb_all)(struct iommu_domain *);
    void (*iotlb_sync_map)(struct iommu_domain *);
    void (*iotlb_sync)(struct iommu_domain *, struct iommu_iotlb_gather *);
    phys_addr_t (*iova_to_phys)(struct iommu_domain *, dma_addr_t);
    int (*add_device)(struct device *);
    void (*remove_device)(struct device *);
    struct iommu_group * (*device_group)(struct device *);
    int (*domain_get_attr)(struct iommu_domain *, enum iommu_attr, void *);
    int (*domain_set_attr)(struct iommu_domain *, enum iommu_attr, void *);
    void (*get_resv_regions)(struct device *, struct list_head *);
    void (*put_resv_regions)(struct device *, struct list_head *);
    void (*apply_resv_region)(struct device *, struct iommu_domain *, struct iommu_resv_region *);
    int (*domain_window_enable)(struct iommu_domain *, u32, phys_addr_t, u64, int);
    void (*domain_window_disable)(struct iommu_domain *, u32);
    int (*of_xlate)(struct device *, struct of_phandle_args *);
    bool (*is_attach_deferred)(struct iommu_domain *, struct device *);
    bool (*dev_has_feat)(struct device *, enum iommu_dev_features);
    bool (*dev_feat_enabled)(struct device *, enum iommu_dev_features);
    int (*dev_enable_feat)(struct device *, enum iommu_dev_features);
    int (*dev_disable_feat)(struct device *, enum iommu_dev_features);
    int (*aux_attach_dev)(struct iommu_domain *, struct device *);
    void (*aux_detach_dev)(struct iommu_domain *, struct device *);
    int (*aux_get_pasid)(struct iommu_domain *, struct device *);
    struct iommu_sva * (*sva_bind)(struct device *, struct mm_struct *, void *);
    void (*sva_unbind)(struct iommu_sva *);
    int (*sva_get_pasid)(struct iommu_sva *);
    int (*page_response)(struct device *, struct iommu_fault_event *, struct iommu_page_response *);
    long unsigned int pgsize_bitmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct iommu_ops {
    bool (*capable)(enum iommu_cap);
    struct iommu_domain * (*domain_alloc)(unsigned int);
    void (*domain_free)(struct iommu_domain *);
    int (*attach_dev)(struct iommu_domain *, struct device *);
    void (*detach_dev)(struct iommu_domain *, struct device *);
    int (*map)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, int);
    size_t (*unmap)(struct iommu_domain *, long unsigned int, size_t, struct iommu_iotlb_gather *);
    void (*flush_iotlb_all)(struct iommu_domain *);
    void (*iotlb_sync_map)(struct iommu_domain *);
    void (*iotlb_sync)(struct iommu_domain *, struct iommu_iotlb_gather *);
    phys_addr_t (*iova_to_phys)(struct iommu_domain *, dma_addr_t);
    int (*add_device)(struct device *);
    void (*remove_device)(struct device *);
    struct iommu_group * (*device_group)(struct device *);
    int (*domain_get_attr)(struct iommu_domain *, enum iommu_attr, void *);
    int (*domain_set_attr)(struct iommu_domain *, enum iommu_attr, void *);
    void (*get_resv_regions)(struct device *, struct list_head *);
    void (*put_resv_regions)(struct device *, struct list_head *);
    void (*apply_resv_region)(struct device *, struct iommu_domain *, struct iommu_resv_region *);
    int (*domain_window_enable)(struct iommu_domain *, u32, phys_addr_t, u64, int);
    void (*domain_window_disable)(struct iommu_domain *, u32);
    int (*of_xlate)(struct device *, struct of_phandle_args *);
    bool (*is_attach_deferred)(struct iommu_domain *, struct device *);
    bool (*dev_has_feat)(struct device *, enum iommu_dev_features);
    bool (*dev_feat_enabled)(struct device *, enum iommu_dev_features);
    int (*dev_enable_feat)(struct device *, enum iommu_dev_features);
    int (*dev_disable_feat)(struct device *, enum iommu_dev_features);
    int (*aux_attach_dev)(struct iommu_domain *, struct device *);
    void (*aux_detach_dev)(struct iommu_domain *, struct device *);
    int (*aux_get_pasid)(struct iommu_domain *, struct device *);
    struct iommu_sva * (*sva_bind)(struct device *, struct mm_struct *, void *);
    void (*sva_unbind)(struct iommu_sva *);
    int (*sva_get_pasid)(struct iommu_sva *);
    int (*page_response)(struct device *, struct iommu_fault_event *, struct iommu_page_response *);
    long unsigned int pgsize_bitmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct iommu_ops {
    bool (*capable)(enum iommu_cap);
    struct iommu_domain * (*domain_alloc)(unsigned int);
    void (*domain_free)(struct iommu_domain *);
    int (*attach_dev)(struct iommu_domain *, struct device *);
    void (*detach_dev)(struct iommu_domain *, struct device *);
    int (*map)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, int);
    size_t (*unmap)(struct iommu_domain *, long unsigned int, size_t, struct iommu_iotlb_gather *);
    void (*flush_iotlb_all)(struct iommu_domain *);
    void (*iotlb_sync_map)(struct iommu_domain *);
    void (*iotlb_sync)(struct iommu_domain *, struct iommu_iotlb_gather *);
    phys_addr_t (*iova_to_phys)(struct iommu_domain *, dma_addr_t);
    int (*add_device)(struct device *);
    void (*remove_device)(struct device *);
    struct iommu_group * (*device_group)(struct device *);
    int (*domain_get_attr)(struct iommu_domain *, enum iommu_attr, void *);
    int (*domain_set_attr)(struct iommu_domain *, enum iommu_attr, void *);
    void (*get_resv_regions)(struct device *, struct list_head *);
    void (*put_resv_regions)(struct device *, struct list_head *);
    void (*apply_resv_region)(struct device *, struct iommu_domain *, struct iommu_resv_region *);
    int (*domain_window_enable)(struct iommu_domain *, u32, phys_addr_t, u64, int);
    void (*domain_window_disable)(struct iommu_domain *, u32);
    int (*of_xlate)(struct device *, struct of_phandle_args *);
    bool (*is_attach_deferred)(struct iommu_domain *, struct device *);
    bool (*dev_has_feat)(struct device *, enum iommu_dev_features);
    bool (*dev_feat_enabled)(struct device *, enum iommu_dev_features);
    int (*dev_enable_feat)(struct device *, enum iommu_dev_features);
    int (*dev_disable_feat)(struct device *, enum iommu_dev_features);
    int (*aux_attach_dev)(struct iommu_domain *, struct device *);
    void (*aux_detach_dev)(struct iommu_domain *, struct device *);
    int (*aux_get_pasid)(struct iommu_domain *, struct device *);
    struct iommu_sva * (*sva_bind)(struct device *, struct mm_struct *, void *);
    void (*sva_unbind)(struct iommu_sva *);
    int (*sva_get_pasid)(struct iommu_sva *);
    int (*page_response)(struct device *, struct iommu_fault_event *, struct iommu_page_response *);
    long unsigned int pgsize_bitmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct iommu_ops {
    bool (*capable)(enum iommu_cap);
    struct iommu_domain * (*domain_alloc)(unsigned int);
    void (*domain_free)(struct iommu_domain *);
    int (*attach_dev)(struct iommu_domain *, struct device *);
    void (*detach_dev)(struct iommu_domain *, struct device *);
    int (*map)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, int);
    size_t (*unmap)(struct iommu_domain *, long unsigned int, size_t, struct iommu_iotlb_gather *);
    void (*flush_iotlb_all)(struct iommu_domain *);
    void (*iotlb_sync_map)(struct iommu_domain *);
    void (*iotlb_sync)(struct iommu_domain *, struct iommu_iotlb_gather *);
    phys_addr_t (*iova_to_phys)(struct iommu_domain *, dma_addr_t);
    int (*add_device)(struct device *);
    void (*remove_device)(struct device *);
    struct iommu_group * (*device_group)(struct device *);
    int (*domain_get_attr)(struct iommu_domain *, enum iommu_attr, void *);
    int (*domain_set_attr)(struct iommu_domain *, enum iommu_attr, void *);
    void (*get_resv_regions)(struct device *, struct list_head *);
    void (*put_resv_regions)(struct device *, struct list_head *);
    void (*apply_resv_region)(struct device *, struct iommu_domain *, struct iommu_resv_region *);
    int (*domain_window_enable)(struct iommu_domain *, u32, phys_addr_t, u64, int);
    void (*domain_window_disable)(struct iommu_domain *, u32);
    int (*of_xlate)(struct device *, struct of_phandle_args *);
    bool (*is_attach_deferred)(struct iommu_domain *, struct device *);
    bool (*dev_has_feat)(struct device *, enum iommu_dev_features);
    bool (*dev_feat_enabled)(struct device *, enum iommu_dev_features);
    int (*dev_enable_feat)(struct device *, enum iommu_dev_features);
    int (*dev_disable_feat)(struct device *, enum iommu_dev_features);
    int (*aux_attach_dev)(struct iommu_domain *, struct device *);
    void (*aux_detach_dev)(struct iommu_domain *, struct device *);
    int (*aux_get_pasid)(struct iommu_domain *, struct device *);
    struct iommu_sva * (*sva_bind)(struct device *, struct mm_struct *, void *);
    void (*sva_unbind)(struct iommu_sva *);
    int (*sva_get_pasid)(struct iommu_sva *);
    int (*page_response)(struct device *, struct iommu_fault_event *, struct iommu_page_response *);
    long unsigned int pgsize_bitmap;
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
<b>Field added. </b>
<code>void (*apply_dm_region)(struct device *, struct iommu_domain *, struct iommu_dm_region *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*of_xlate)(struct device *, struct of_phandle_args *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void *priv</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*get_resv_regions)(struct device *, struct list_head *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*put_resv_regions)(struct device *, struct list_head *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*apply_resv_region)(struct device *, struct iommu_domain *, struct iommu_resv_region *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*get_dm_regions)(struct device *, struct list_head *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*put_dm_regions)(struct device *, struct list_head *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*apply_dm_region)(struct device *, struct iommu_domain *, struct iommu_dm_region *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*flush_iotlb_all)(struct iommu_domain *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*iotlb_range_add)(struct iommu_domain *, long unsigned int, size_t)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*iotlb_sync)(struct iommu_domain *)</code>
</li>
<li>
<b>Field added. </b>
<code>bool (*is_attach_deferred)(struct iommu_domain *, struct device *)</code>
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
<b>Field removed. </b>
<code>size_t (*map_sg)(struct iommu_domain *, long unsigned int, struct scatterlist *, unsigned int, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*domain_set_windows)(struct iommu_domain *, u32)</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 (*domain_get_windows)(struct iommu_domain *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*iotlb_sync_map)(struct iommu_domain *)</code>
</li>
<li>
<b>Field added. </b>
<code>bool (*dev_has_feat)(struct device *, enum iommu_dev_features)</code>
</li>
<li>
<b>Field added. </b>
<code>bool (*dev_feat_enabled)(struct device *, enum iommu_dev_features)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*dev_enable_feat)(struct device *, enum iommu_dev_features)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*dev_disable_feat)(struct device *, enum iommu_dev_features)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*aux_attach_dev)(struct iommu_domain *, struct device *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*aux_detach_dev)(struct iommu_domain *, struct device *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*aux_get_pasid)(struct iommu_domain *, struct device *)</code>
</li>
<li>
<b>Field added. </b>
<code>struct iommu_sva * (*sva_bind)(struct device *, struct mm_struct *, void *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*sva_unbind)(struct iommu_sva *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*sva_get_pasid)(struct iommu_sva *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*page_response)(struct device *, struct iommu_fault_event *, struct iommu_page_response *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>void (*iotlb_range_add)(struct iommu_domain *, long unsigned int, size_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>size_t (*unmap)(struct iommu_domain *, long unsigned int, size_t)</code> ➡️ <code>size_t (*unmap)(struct iommu_domain *, long unsigned int, size_t, struct iommu_iotlb_gather *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*iotlb_sync)(struct iommu_domain *)</code> ➡️ <code>void (*iotlb_sync)(struct iommu_domain *, struct iommu_iotlb_gather *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct iommu_device * (*probe_device)(struct device *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*release_device)(struct device *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*probe_finalize)(struct device *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*cache_invalidate)(struct iommu_domain *, struct device *, struct iommu_cache_invalidate_info *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*sva_bind_gpasid)(struct iommu_domain *, struct device *, struct iommu_gpasid_bind_data *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*sva_unbind_gpasid)(struct device *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*def_domain_type)(struct device *)</code>
</li>
<li>
<b>Field added. </b>
<code>struct module *owner</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*add_device)(struct device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*remove_device)(struct device *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*map)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, int)</code> ➡️ <code>int (*map)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, int, gfp_t)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*sva_get_pasid)(struct iommu_sva *)</code> ➡️ <code>u32 (*sva_get_pasid)(struct iommu_sva *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*sva_unbind_gpasid)(struct device *, int)</code> ➡️ <code>int (*sva_unbind_gpasid)(struct device *, u32)</code>
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
<code>int (*enable_nesting)(struct iommu_domain *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_pgtable_quirks)(struct iommu_domain *, long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*domain_get_attr)(struct iommu_domain *, enum iommu_attr, void *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*domain_set_attr)(struct iommu_domain *, enum iommu_attr, void *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*domain_window_enable)(struct iommu_domain *, u32, phys_addr_t, u64, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*domain_window_disable)(struct iommu_domain *, u32)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*iotlb_sync_map)(struct iommu_domain *)</code> ➡️ <code>void (*iotlb_sync_map)(struct iommu_domain *, long unsigned int, size_t)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*map_pages)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, size_t, int, gfp_t, size_t *)</code>
</li>
<li>
<b>Field added. </b>
<code>size_t (*unmap_pages)(struct iommu_domain *, long unsigned int, size_t, size_t, struct iommu_iotlb_gather *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const struct iommu_domain_ops *default_domain_ops</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*domain_free)(struct iommu_domain *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*attach_dev)(struct iommu_domain *, struct device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*detach_dev)(struct iommu_domain *, struct device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*map)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, int, gfp_t)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*map_pages)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, size_t, int, gfp_t, size_t *)</code>
</li>
<li>
<b>Field removed. </b>
<code>size_t (*unmap)(struct iommu_domain *, long unsigned int, size_t, struct iommu_iotlb_gather *)</code>
</li>
<li>
<b>Field removed. </b>
<code>size_t (*unmap_pages)(struct iommu_domain *, long unsigned int, size_t, size_t, struct iommu_iotlb_gather *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*flush_iotlb_all)(struct iommu_domain *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*iotlb_sync_map)(struct iommu_domain *, long unsigned int, size_t)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*iotlb_sync)(struct iommu_domain *, struct iommu_iotlb_gather *)</code>
</li>
<li>
<b>Field removed. </b>
<code>phys_addr_t (*iova_to_phys)(struct iommu_domain *, dma_addr_t)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*enable_nesting)(struct iommu_domain *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*set_pgtable_quirks)(struct iommu_domain *, long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*apply_resv_region)(struct device *, struct iommu_domain *, struct iommu_resv_region *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*aux_attach_dev)(struct iommu_domain *, struct device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*aux_detach_dev)(struct iommu_domain *, struct device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*aux_get_pasid)(struct iommu_domain *, struct device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*cache_invalidate)(struct iommu_domain *, struct device *, struct iommu_cache_invalidate_info *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*sva_bind_gpasid)(struct iommu_domain *, struct device *, struct iommu_gpasid_bind_data *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*sva_unbind_gpasid)(struct device *, u32)</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool (*is_attach_deferred)(struct iommu_domain *, struct device *)</code> ➡️ <code>bool (*is_attach_deferred)(struct device *)</code>
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
<code>void (*remove_dev_pasid)(struct device *, ioasid_t)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*put_resv_regions)(struct device *, struct list_head *)</code>
</li>
<li>
<b>Field removed. </b>
<code>bool (*dev_has_feat)(struct device *, enum iommu_dev_features)</code>
</li>
<li>
<b>Field removed. </b>
<code>bool (*dev_feat_enabled)(struct device *, enum iommu_dev_features)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct iommu_sva * (*sva_bind)(struct device *, struct mm_struct *, void *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*sva_unbind)(struct iommu_sva *)</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 (*sva_get_pasid)(struct iommu_sva *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool (*capable)(enum iommu_cap)</code> ➡️ <code>bool (*capable)(struct device *, enum iommu_cap)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*set_platform_dma_ops)(struct device *)</code>
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
<code>void * (*hw_info)(struct device *, u32 *, u32 *)</code>
</li>
<li>
<b>Field added. </b>
<code>struct iommu_domain * (*domain_alloc_user)(struct device *, u32, struct iommu_domain *, const struct iommu_user_data *)</code>
</li>
<li>
<b>Field added. </b>
<code>struct iommu_domain * (*domain_alloc_paging)(struct device *)</code>
</li>
<li>
<b>Field added. </b>
<code>struct iommu_domain *identity_domain</code>
</li>
<li>
<b>Field added. </b>
<code>struct iommu_domain *blocked_domain</code>
</li>
<li>
<b>Field added. </b>
<code>struct iommu_domain *default_domain</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*set_platform_dma_ops)(struct device *)</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>bool (*capable)(enum iommu_cap)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct iommu_domain * (*domain_alloc)(unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*domain_free)(struct iommu_domain *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*attach_dev)(struct iommu_domain *, struct device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*detach_dev)(struct iommu_domain *, struct device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*map)(struct iommu_domain *, long unsigned int, phys_addr_t, size_t, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>size_t (*unmap)(struct iommu_domain *, long unsigned int, size_t, struct iommu_iotlb_gather *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*flush_iotlb_all)(struct iommu_domain *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*iotlb_sync_map)(struct iommu_domain *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*iotlb_sync)(struct iommu_domain *, struct iommu_iotlb_gather *)</code>
</li>
<li>
<b>Field removed. </b>
<code>phys_addr_t (*iova_to_phys)(struct iommu_domain *, dma_addr_t)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*add_device)(struct device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*remove_device)(struct device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct iommu_group * (*device_group)(struct device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*domain_get_attr)(struct iommu_domain *, enum iommu_attr, void *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*domain_set_attr)(struct iommu_domain *, enum iommu_attr, void *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*get_resv_regions)(struct device *, struct list_head *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*put_resv_regions)(struct device *, struct list_head *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*apply_resv_region)(struct device *, struct iommu_domain *, struct iommu_resv_region *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*domain_window_enable)(struct iommu_domain *, u32, phys_addr_t, u64, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*domain_window_disable)(struct iommu_domain *, u32)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*of_xlate)(struct device *, struct of_phandle_args *)</code>
</li>
<li>
<b>Field removed. </b>
<code>bool (*is_attach_deferred)(struct iommu_domain *, struct device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>bool (*dev_has_feat)(struct device *, enum iommu_dev_features)</code>
</li>
<li>
<b>Field removed. </b>
<code>bool (*dev_feat_enabled)(struct device *, enum iommu_dev_features)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*dev_enable_feat)(struct device *, enum iommu_dev_features)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*dev_disable_feat)(struct device *, enum iommu_dev_features)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*aux_attach_dev)(struct iommu_domain *, struct device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*aux_detach_dev)(struct iommu_domain *, struct device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*aux_get_pasid)(struct iommu_domain *, struct device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct iommu_sva * (*sva_bind)(struct device *, struct mm_struct *, void *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*sva_unbind)(struct iommu_sva *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*sva_get_pasid)(struct iommu_sva *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*page_response)(struct device *, struct iommu_fault_event *, struct iommu_page_response *)</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int pgsize_bitmap</code>
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
