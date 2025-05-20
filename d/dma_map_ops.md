# Struct: <code>dma_map_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct dma_map_ops {
    void * (*alloc)(struct device *, size_t, dma_addr_t *, gfp_t, struct dma_attrs *);
    void (*free)(struct device *, size_t, void *, dma_addr_t, struct dma_attrs *);
    int (*mmap)(struct device *, struct vm_area_struct *, void *, dma_addr_t, size_t, struct dma_attrs *);
    int (*get_sgtable)(struct device *, struct sg_table *, void *, dma_addr_t, size_t, struct dma_attrs *);
    dma_addr_t (*map_page)(struct device *, struct page *, long unsigned int, size_t, enum dma_data_direction, struct dma_attrs *);
    void (*unmap_page)(struct device *, dma_addr_t, size_t, enum dma_data_direction, struct dma_attrs *);
    int (*map_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, struct dma_attrs *);
    void (*unmap_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, struct dma_attrs *);
    void (*sync_single_for_cpu)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_single_for_device)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_sg_for_cpu)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*sync_sg_for_device)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    int (*mapping_error)(struct device *, dma_addr_t);
    int (*dma_supported)(struct device *, u64);
    int (*set_dma_mask)(struct device *, u64);
    int is_phys;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct dma_map_ops {
    void * (*alloc)(struct device *, size_t, dma_addr_t *, gfp_t, long unsigned int);
    void (*free)(struct device *, size_t, void *, dma_addr_t, long unsigned int);
    int (*mmap)(struct device *, struct vm_area_struct *, void *, dma_addr_t, size_t, long unsigned int);
    int (*get_sgtable)(struct device *, struct sg_table *, void *, dma_addr_t, size_t, long unsigned int);
    dma_addr_t (*map_page)(struct device *, struct page *, long unsigned int, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_page)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    int (*map_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    void (*unmap_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    void (*sync_single_for_cpu)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_single_for_device)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_sg_for_cpu)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*sync_sg_for_device)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    int (*mapping_error)(struct device *, dma_addr_t);
    int (*dma_supported)(struct device *, u64);
    int (*set_dma_mask)(struct device *, u64);
    int is_phys;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct dma_map_ops {
    void * (*alloc)(struct device *, size_t, dma_addr_t *, gfp_t, long unsigned int);
    void (*free)(struct device *, size_t, void *, dma_addr_t, long unsigned int);
    int (*mmap)(struct device *, struct vm_area_struct *, void *, dma_addr_t, size_t, long unsigned int);
    int (*get_sgtable)(struct device *, struct sg_table *, void *, dma_addr_t, size_t, long unsigned int);
    dma_addr_t (*map_page)(struct device *, struct page *, long unsigned int, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_page)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    int (*map_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    void (*unmap_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    dma_addr_t (*map_resource)(struct device *, phys_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_resource)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*sync_single_for_cpu)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_single_for_device)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_sg_for_cpu)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*sync_sg_for_device)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    int (*mapping_error)(struct device *, dma_addr_t);
    int (*dma_supported)(struct device *, u64);
    int (*set_dma_mask)(struct device *, u64);
    int is_phys;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct dma_map_ops {
    void * (*alloc)(struct device *, size_t, dma_addr_t *, gfp_t, long unsigned int);
    void (*free)(struct device *, size_t, void *, dma_addr_t, long unsigned int);
    int (*mmap)(struct device *, struct vm_area_struct *, void *, dma_addr_t, size_t, long unsigned int);
    int (*get_sgtable)(struct device *, struct sg_table *, void *, dma_addr_t, size_t, long unsigned int);
    dma_addr_t (*map_page)(struct device *, struct page *, long unsigned int, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_page)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    int (*map_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    void (*unmap_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    dma_addr_t (*map_resource)(struct device *, phys_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_resource)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*sync_single_for_cpu)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_single_for_device)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_sg_for_cpu)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*sync_sg_for_device)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    int (*mapping_error)(struct device *, dma_addr_t);
    int (*dma_supported)(struct device *, u64);
    int is_phys;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dma_map_ops {
    void * (*alloc)(struct device *, size_t, dma_addr_t *, gfp_t, long unsigned int);
    void (*free)(struct device *, size_t, void *, dma_addr_t, long unsigned int);
    int (*mmap)(struct device *, struct vm_area_struct *, void *, dma_addr_t, size_t, long unsigned int);
    int (*get_sgtable)(struct device *, struct sg_table *, void *, dma_addr_t, size_t, long unsigned int);
    dma_addr_t (*map_page)(struct device *, struct page *, long unsigned int, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_page)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    int (*map_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    void (*unmap_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    dma_addr_t (*map_resource)(struct device *, phys_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_resource)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*sync_single_for_cpu)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_single_for_device)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_sg_for_cpu)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*sync_sg_for_device)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*cache_sync)(struct device *, void *, size_t, enum dma_data_direction);
    int (*mapping_error)(struct device *, dma_addr_t);
    int (*dma_supported)(struct device *, u64);
    int is_phys;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dma_map_ops {
    void * (*alloc)(struct device *, size_t, dma_addr_t *, gfp_t, long unsigned int);
    void (*free)(struct device *, size_t, void *, dma_addr_t, long unsigned int);
    int (*mmap)(struct device *, struct vm_area_struct *, void *, dma_addr_t, size_t, long unsigned int);
    int (*get_sgtable)(struct device *, struct sg_table *, void *, dma_addr_t, size_t, long unsigned int);
    dma_addr_t (*map_page)(struct device *, struct page *, long unsigned int, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_page)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    int (*map_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    void (*unmap_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    dma_addr_t (*map_resource)(struct device *, phys_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_resource)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*sync_single_for_cpu)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_single_for_device)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_sg_for_cpu)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*sync_sg_for_device)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*cache_sync)(struct device *, void *, size_t, enum dma_data_direction);
    int (*mapping_error)(struct device *, dma_addr_t);
    int (*dma_supported)(struct device *, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dma_map_ops {
    void * (*alloc)(struct device *, size_t, dma_addr_t *, gfp_t, long unsigned int);
    void (*free)(struct device *, size_t, void *, dma_addr_t, long unsigned int);
    int (*mmap)(struct device *, struct vm_area_struct *, void *, dma_addr_t, size_t, long unsigned int);
    int (*get_sgtable)(struct device *, struct sg_table *, void *, dma_addr_t, size_t, long unsigned int);
    dma_addr_t (*map_page)(struct device *, struct page *, long unsigned int, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_page)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    int (*map_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    void (*unmap_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    dma_addr_t (*map_resource)(struct device *, phys_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_resource)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*sync_single_for_cpu)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_single_for_device)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_sg_for_cpu)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*sync_sg_for_device)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*cache_sync)(struct device *, void *, size_t, enum dma_data_direction);
    int (*dma_supported)(struct device *, u64);
    u64 (*get_required_mask)(struct device *);
    size_t (*max_mapping_size)(struct device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dma_map_ops {
    void * (*alloc)(struct device *, size_t, dma_addr_t *, gfp_t, long unsigned int);
    void (*free)(struct device *, size_t, void *, dma_addr_t, long unsigned int);
    int (*mmap)(struct device *, struct vm_area_struct *, void *, dma_addr_t, size_t, long unsigned int);
    int (*get_sgtable)(struct device *, struct sg_table *, void *, dma_addr_t, size_t, long unsigned int);
    dma_addr_t (*map_page)(struct device *, struct page *, long unsigned int, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_page)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    int (*map_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    void (*unmap_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    dma_addr_t (*map_resource)(struct device *, phys_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_resource)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*sync_single_for_cpu)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_single_for_device)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_sg_for_cpu)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*sync_sg_for_device)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*cache_sync)(struct device *, void *, size_t, enum dma_data_direction);
    int (*dma_supported)(struct device *, u64);
    u64 (*get_required_mask)(struct device *);
    size_t (*max_mapping_size)(struct device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dma_map_ops {
    void * (*alloc)(struct device *, size_t, dma_addr_t *, gfp_t, long unsigned int);
    void (*free)(struct device *, size_t, void *, dma_addr_t, long unsigned int);
    int (*mmap)(struct device *, struct vm_area_struct *, void *, dma_addr_t, size_t, long unsigned int);
    int (*get_sgtable)(struct device *, struct sg_table *, void *, dma_addr_t, size_t, long unsigned int);
    dma_addr_t (*map_page)(struct device *, struct page *, long unsigned int, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_page)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    int (*map_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    void (*unmap_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    dma_addr_t (*map_resource)(struct device *, phys_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_resource)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*sync_single_for_cpu)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_single_for_device)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_sg_for_cpu)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*sync_sg_for_device)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*cache_sync)(struct device *, void *, size_t, enum dma_data_direction);
    int (*dma_supported)(struct device *, u64);
    u64 (*get_required_mask)(struct device *);
    size_t (*max_mapping_size)(struct device *);
    long unsigned int (*get_merge_boundary)(struct device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dma_map_ops {
    void * (*alloc)(struct device *, size_t, dma_addr_t *, gfp_t, long unsigned int);
    void (*free)(struct device *, size_t, void *, dma_addr_t, long unsigned int);
    int (*mmap)(struct device *, struct vm_area_struct *, void *, dma_addr_t, size_t, long unsigned int);
    int (*get_sgtable)(struct device *, struct sg_table *, void *, dma_addr_t, size_t, long unsigned int);
    dma_addr_t (*map_page)(struct device *, struct page *, long unsigned int, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_page)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    int (*map_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    void (*unmap_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    dma_addr_t (*map_resource)(struct device *, phys_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_resource)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*sync_single_for_cpu)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_single_for_device)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_sg_for_cpu)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*sync_sg_for_device)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*cache_sync)(struct device *, void *, size_t, enum dma_data_direction);
    int (*dma_supported)(struct device *, u64);
    u64 (*get_required_mask)(struct device *);
    size_t (*max_mapping_size)(struct device *);
    long unsigned int (*get_merge_boundary)(struct device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dma_map_ops {
    void * (*alloc)(struct device *, size_t, dma_addr_t *, gfp_t, long unsigned int);
    void (*free)(struct device *, size_t, void *, dma_addr_t, long unsigned int);
    struct page * (*alloc_pages)(struct device *, size_t, dma_addr_t *, enum dma_data_direction, gfp_t);
    void (*free_pages)(struct device *, size_t, struct page *, dma_addr_t, enum dma_data_direction);
    void * (*alloc_noncoherent)(struct device *, size_t, dma_addr_t *, enum dma_data_direction, gfp_t);
    void (*free_noncoherent)(struct device *, size_t, void *, dma_addr_t, enum dma_data_direction);
    int (*mmap)(struct device *, struct vm_area_struct *, void *, dma_addr_t, size_t, long unsigned int);
    int (*get_sgtable)(struct device *, struct sg_table *, void *, dma_addr_t, size_t, long unsigned int);
    dma_addr_t (*map_page)(struct device *, struct page *, long unsigned int, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_page)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    int (*map_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    void (*unmap_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    dma_addr_t (*map_resource)(struct device *, phys_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_resource)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*sync_single_for_cpu)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_single_for_device)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_sg_for_cpu)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*sync_sg_for_device)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*cache_sync)(struct device *, void *, size_t, enum dma_data_direction);
    int (*dma_supported)(struct device *, u64);
    u64 (*get_required_mask)(struct device *);
    size_t (*max_mapping_size)(struct device *);
    long unsigned int (*get_merge_boundary)(struct device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dma_map_ops {
    void * (*alloc)(struct device *, size_t, dma_addr_t *, gfp_t, long unsigned int);
    void (*free)(struct device *, size_t, void *, dma_addr_t, long unsigned int);
    struct page * (*alloc_pages)(struct device *, size_t, dma_addr_t *, enum dma_data_direction, gfp_t);
    void (*free_pages)(struct device *, size_t, struct page *, dma_addr_t, enum dma_data_direction);
    struct sg_table * (*alloc_noncontiguous)(struct device *, size_t, enum dma_data_direction, gfp_t, long unsigned int);
    void (*free_noncontiguous)(struct device *, size_t, struct sg_table *, enum dma_data_direction);
    int (*mmap)(struct device *, struct vm_area_struct *, void *, dma_addr_t, size_t, long unsigned int);
    int (*get_sgtable)(struct device *, struct sg_table *, void *, dma_addr_t, size_t, long unsigned int);
    dma_addr_t (*map_page)(struct device *, struct page *, long unsigned int, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_page)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    int (*map_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    void (*unmap_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    dma_addr_t (*map_resource)(struct device *, phys_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_resource)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*sync_single_for_cpu)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_single_for_device)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_sg_for_cpu)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*sync_sg_for_device)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*cache_sync)(struct device *, void *, size_t, enum dma_data_direction);
    int (*dma_supported)(struct device *, u64);
    u64 (*get_required_mask)(struct device *);
    size_t (*max_mapping_size)(struct device *);
    long unsigned int (*get_merge_boundary)(struct device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dma_map_ops {
    void * (*alloc)(struct device *, size_t, dma_addr_t *, gfp_t, long unsigned int);
    void (*free)(struct device *, size_t, void *, dma_addr_t, long unsigned int);
    struct page * (*alloc_pages)(struct device *, size_t, dma_addr_t *, enum dma_data_direction, gfp_t);
    void (*free_pages)(struct device *, size_t, struct page *, dma_addr_t, enum dma_data_direction);
    struct sg_table * (*alloc_noncontiguous)(struct device *, size_t, enum dma_data_direction, gfp_t, long unsigned int);
    void (*free_noncontiguous)(struct device *, size_t, struct sg_table *, enum dma_data_direction);
    int (*mmap)(struct device *, struct vm_area_struct *, void *, dma_addr_t, size_t, long unsigned int);
    int (*get_sgtable)(struct device *, struct sg_table *, void *, dma_addr_t, size_t, long unsigned int);
    dma_addr_t (*map_page)(struct device *, struct page *, long unsigned int, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_page)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    int (*map_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    void (*unmap_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    dma_addr_t (*map_resource)(struct device *, phys_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_resource)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*sync_single_for_cpu)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_single_for_device)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_sg_for_cpu)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*sync_sg_for_device)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*cache_sync)(struct device *, void *, size_t, enum dma_data_direction);
    int (*dma_supported)(struct device *, u64);
    u64 (*get_required_mask)(struct device *);
    size_t (*max_mapping_size)(struct device *);
    long unsigned int (*get_merge_boundary)(struct device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dma_map_ops {
    void * (*alloc)(struct device *, size_t, dma_addr_t *, gfp_t, long unsigned int);
    void (*free)(struct device *, size_t, void *, dma_addr_t, long unsigned int);
    struct page * (*alloc_pages)(struct device *, size_t, dma_addr_t *, enum dma_data_direction, gfp_t);
    void (*free_pages)(struct device *, size_t, struct page *, dma_addr_t, enum dma_data_direction);
    struct sg_table * (*alloc_noncontiguous)(struct device *, size_t, enum dma_data_direction, gfp_t, long unsigned int);
    void (*free_noncontiguous)(struct device *, size_t, struct sg_table *, enum dma_data_direction);
    int (*mmap)(struct device *, struct vm_area_struct *, void *, dma_addr_t, size_t, long unsigned int);
    int (*get_sgtable)(struct device *, struct sg_table *, void *, dma_addr_t, size_t, long unsigned int);
    dma_addr_t (*map_page)(struct device *, struct page *, long unsigned int, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_page)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    int (*map_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    void (*unmap_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    dma_addr_t (*map_resource)(struct device *, phys_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_resource)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*sync_single_for_cpu)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_single_for_device)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_sg_for_cpu)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*sync_sg_for_device)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*cache_sync)(struct device *, void *, size_t, enum dma_data_direction);
    int (*dma_supported)(struct device *, u64);
    u64 (*get_required_mask)(struct device *);
    size_t (*max_mapping_size)(struct device *);
    long unsigned int (*get_merge_boundary)(struct device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dma_map_ops {
    unsigned int flags;
    void * (*alloc)(struct device *, size_t, dma_addr_t *, gfp_t, long unsigned int);
    void (*free)(struct device *, size_t, void *, dma_addr_t, long unsigned int);
    struct page * (*alloc_pages)(struct device *, size_t, dma_addr_t *, enum dma_data_direction, gfp_t);
    void (*free_pages)(struct device *, size_t, struct page *, dma_addr_t, enum dma_data_direction);
    struct sg_table * (*alloc_noncontiguous)(struct device *, size_t, enum dma_data_direction, gfp_t, long unsigned int);
    void (*free_noncontiguous)(struct device *, size_t, struct sg_table *, enum dma_data_direction);
    int (*mmap)(struct device *, struct vm_area_struct *, void *, dma_addr_t, size_t, long unsigned int);
    int (*get_sgtable)(struct device *, struct sg_table *, void *, dma_addr_t, size_t, long unsigned int);
    dma_addr_t (*map_page)(struct device *, struct page *, long unsigned int, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_page)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    int (*map_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    void (*unmap_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    dma_addr_t (*map_resource)(struct device *, phys_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_resource)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*sync_single_for_cpu)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_single_for_device)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_sg_for_cpu)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*sync_sg_for_device)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*cache_sync)(struct device *, void *, size_t, enum dma_data_direction);
    int (*dma_supported)(struct device *, u64);
    u64 (*get_required_mask)(struct device *);
    size_t (*max_mapping_size)(struct device *);
    size_t (*opt_mapping_size)();
    long unsigned int (*get_merge_boundary)(struct device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dma_map_ops {
    unsigned int flags;
    void * (*alloc)(struct device *, size_t, dma_addr_t *, gfp_t, long unsigned int);
    void (*free)(struct device *, size_t, void *, dma_addr_t, long unsigned int);
    struct page * (*alloc_pages)(struct device *, size_t, dma_addr_t *, enum dma_data_direction, gfp_t);
    void (*free_pages)(struct device *, size_t, struct page *, dma_addr_t, enum dma_data_direction);
    struct sg_table * (*alloc_noncontiguous)(struct device *, size_t, enum dma_data_direction, gfp_t, long unsigned int);
    void (*free_noncontiguous)(struct device *, size_t, struct sg_table *, enum dma_data_direction);
    int (*mmap)(struct device *, struct vm_area_struct *, void *, dma_addr_t, size_t, long unsigned int);
    int (*get_sgtable)(struct device *, struct sg_table *, void *, dma_addr_t, size_t, long unsigned int);
    dma_addr_t (*map_page)(struct device *, struct page *, long unsigned int, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_page)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    int (*map_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    void (*unmap_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    dma_addr_t (*map_resource)(struct device *, phys_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_resource)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*sync_single_for_cpu)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_single_for_device)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_sg_for_cpu)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*sync_sg_for_device)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*cache_sync)(struct device *, void *, size_t, enum dma_data_direction);
    int (*dma_supported)(struct device *, u64);
    u64 (*get_required_mask)(struct device *);
    size_t (*max_mapping_size)(struct device *);
    size_t (*opt_mapping_size)();
    long unsigned int (*get_merge_boundary)(struct device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dma_map_ops {
    unsigned int flags;
    void * (*alloc)(struct device *, size_t, dma_addr_t *, gfp_t, long unsigned int);
    void (*free)(struct device *, size_t, void *, dma_addr_t, long unsigned int);
    struct page * (*alloc_pages)(struct device *, size_t, dma_addr_t *, enum dma_data_direction, gfp_t);
    void (*free_pages)(struct device *, size_t, struct page *, dma_addr_t, enum dma_data_direction);
    struct sg_table * (*alloc_noncontiguous)(struct device *, size_t, enum dma_data_direction, gfp_t, long unsigned int);
    void (*free_noncontiguous)(struct device *, size_t, struct sg_table *, enum dma_data_direction);
    int (*mmap)(struct device *, struct vm_area_struct *, void *, dma_addr_t, size_t, long unsigned int);
    int (*get_sgtable)(struct device *, struct sg_table *, void *, dma_addr_t, size_t, long unsigned int);
    dma_addr_t (*map_page)(struct device *, struct page *, long unsigned int, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_page)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    int (*map_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    void (*unmap_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    dma_addr_t (*map_resource)(struct device *, phys_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_resource)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*sync_single_for_cpu)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_single_for_device)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_sg_for_cpu)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*sync_sg_for_device)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*cache_sync)(struct device *, void *, size_t, enum dma_data_direction);
    int (*dma_supported)(struct device *, u64);
    u64 (*get_required_mask)(struct device *);
    size_t (*max_mapping_size)(struct device *);
    size_t (*opt_mapping_size)();
    long unsigned int (*get_merge_boundary)(struct device *);
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
struct dma_map_ops {
    void * (*alloc)(struct device *, size_t, dma_addr_t *, gfp_t, long unsigned int);
    void (*free)(struct device *, size_t, void *, dma_addr_t, long unsigned int);
    int (*mmap)(struct device *, struct vm_area_struct *, void *, dma_addr_t, size_t, long unsigned int);
    int (*get_sgtable)(struct device *, struct sg_table *, void *, dma_addr_t, size_t, long unsigned int);
    dma_addr_t (*map_page)(struct device *, struct page *, long unsigned int, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_page)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    int (*map_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    void (*unmap_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    dma_addr_t (*map_resource)(struct device *, phys_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_resource)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*sync_single_for_cpu)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_single_for_device)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_sg_for_cpu)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*sync_sg_for_device)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*cache_sync)(struct device *, void *, size_t, enum dma_data_direction);
    int (*dma_supported)(struct device *, u64);
    u64 (*get_required_mask)(struct device *);
    size_t (*max_mapping_size)(struct device *);
    long unsigned int (*get_merge_boundary)(struct device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dma_map_ops {
    void * (*alloc)(struct device *, size_t, dma_addr_t *, gfp_t, long unsigned int);
    void (*free)(struct device *, size_t, void *, dma_addr_t, long unsigned int);
    int (*mmap)(struct device *, struct vm_area_struct *, void *, dma_addr_t, size_t, long unsigned int);
    int (*get_sgtable)(struct device *, struct sg_table *, void *, dma_addr_t, size_t, long unsigned int);
    dma_addr_t (*map_page)(struct device *, struct page *, long unsigned int, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_page)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    int (*map_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    void (*unmap_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    dma_addr_t (*map_resource)(struct device *, phys_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_resource)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*sync_single_for_cpu)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_single_for_device)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_sg_for_cpu)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*sync_sg_for_device)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*cache_sync)(struct device *, void *, size_t, enum dma_data_direction);
    int (*dma_supported)(struct device *, u64);
    u64 (*get_required_mask)(struct device *);
    size_t (*max_mapping_size)(struct device *);
    long unsigned int (*get_merge_boundary)(struct device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dma_map_ops {
    void * (*alloc)(struct device *, size_t, dma_addr_t *, gfp_t, long unsigned int);
    void (*free)(struct device *, size_t, void *, dma_addr_t, long unsigned int);
    int (*mmap)(struct device *, struct vm_area_struct *, void *, dma_addr_t, size_t, long unsigned int);
    int (*get_sgtable)(struct device *, struct sg_table *, void *, dma_addr_t, size_t, long unsigned int);
    dma_addr_t (*map_page)(struct device *, struct page *, long unsigned int, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_page)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    int (*map_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    void (*unmap_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    dma_addr_t (*map_resource)(struct device *, phys_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_resource)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*sync_single_for_cpu)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_single_for_device)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_sg_for_cpu)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*sync_sg_for_device)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*cache_sync)(struct device *, void *, size_t, enum dma_data_direction);
    int (*dma_supported)(struct device *, u64);
    u64 (*get_required_mask)(struct device *);
    size_t (*max_mapping_size)(struct device *);
    long unsigned int (*get_merge_boundary)(struct device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dma_map_ops {
    void * (*alloc)(struct device *, size_t, dma_addr_t *, gfp_t, long unsigned int);
    void (*free)(struct device *, size_t, void *, dma_addr_t, long unsigned int);
    int (*mmap)(struct device *, struct vm_area_struct *, void *, dma_addr_t, size_t, long unsigned int);
    int (*get_sgtable)(struct device *, struct sg_table *, void *, dma_addr_t, size_t, long unsigned int);
    dma_addr_t (*map_page)(struct device *, struct page *, long unsigned int, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_page)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    int (*map_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    void (*unmap_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    dma_addr_t (*map_resource)(struct device *, phys_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_resource)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*sync_single_for_cpu)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_single_for_device)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_sg_for_cpu)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*sync_sg_for_device)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*cache_sync)(struct device *, void *, size_t, enum dma_data_direction);
    int (*dma_supported)(struct device *, u64);
    u64 (*get_required_mask)(struct device *);
    size_t (*max_mapping_size)(struct device *);
    long unsigned int (*get_merge_boundary)(struct device *);
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
struct dma_map_ops {
    void * (*alloc)(struct device *, size_t, dma_addr_t *, gfp_t, long unsigned int);
    void (*free)(struct device *, size_t, void *, dma_addr_t, long unsigned int);
    int (*mmap)(struct device *, struct vm_area_struct *, void *, dma_addr_t, size_t, long unsigned int);
    int (*get_sgtable)(struct device *, struct sg_table *, void *, dma_addr_t, size_t, long unsigned int);
    dma_addr_t (*map_page)(struct device *, struct page *, long unsigned int, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_page)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    int (*map_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    void (*unmap_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    dma_addr_t (*map_resource)(struct device *, phys_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_resource)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*sync_single_for_cpu)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_single_for_device)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_sg_for_cpu)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*sync_sg_for_device)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*cache_sync)(struct device *, void *, size_t, enum dma_data_direction);
    int (*dma_supported)(struct device *, u64);
    u64 (*get_required_mask)(struct device *);
    size_t (*max_mapping_size)(struct device *);
    long unsigned int (*get_merge_boundary)(struct device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dma_map_ops {
    void * (*alloc)(struct device *, size_t, dma_addr_t *, gfp_t, long unsigned int);
    void (*free)(struct device *, size_t, void *, dma_addr_t, long unsigned int);
    int (*mmap)(struct device *, struct vm_area_struct *, void *, dma_addr_t, size_t, long unsigned int);
    int (*get_sgtable)(struct device *, struct sg_table *, void *, dma_addr_t, size_t, long unsigned int);
    dma_addr_t (*map_page)(struct device *, struct page *, long unsigned int, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_page)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    int (*map_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    void (*unmap_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    dma_addr_t (*map_resource)(struct device *, phys_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_resource)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*sync_single_for_cpu)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_single_for_device)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_sg_for_cpu)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*sync_sg_for_device)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*cache_sync)(struct device *, void *, size_t, enum dma_data_direction);
    int (*dma_supported)(struct device *, u64);
    u64 (*get_required_mask)(struct device *);
    size_t (*max_mapping_size)(struct device *);
    long unsigned int (*get_merge_boundary)(struct device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dma_map_ops {
    void * (*alloc)(struct device *, size_t, dma_addr_t *, gfp_t, long unsigned int);
    void (*free)(struct device *, size_t, void *, dma_addr_t, long unsigned int);
    int (*mmap)(struct device *, struct vm_area_struct *, void *, dma_addr_t, size_t, long unsigned int);
    int (*get_sgtable)(struct device *, struct sg_table *, void *, dma_addr_t, size_t, long unsigned int);
    dma_addr_t (*map_page)(struct device *, struct page *, long unsigned int, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_page)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    int (*map_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    void (*unmap_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    dma_addr_t (*map_resource)(struct device *, phys_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_resource)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*sync_single_for_cpu)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_single_for_device)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_sg_for_cpu)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*sync_sg_for_device)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*cache_sync)(struct device *, void *, size_t, enum dma_data_direction);
    int (*dma_supported)(struct device *, u64);
    u64 (*get_required_mask)(struct device *);
    size_t (*max_mapping_size)(struct device *);
    long unsigned int (*get_merge_boundary)(struct device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dma_map_ops {
    void * (*alloc)(struct device *, size_t, dma_addr_t *, gfp_t, long unsigned int);
    void (*free)(struct device *, size_t, void *, dma_addr_t, long unsigned int);
    int (*mmap)(struct device *, struct vm_area_struct *, void *, dma_addr_t, size_t, long unsigned int);
    int (*get_sgtable)(struct device *, struct sg_table *, void *, dma_addr_t, size_t, long unsigned int);
    dma_addr_t (*map_page)(struct device *, struct page *, long unsigned int, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_page)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    int (*map_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    void (*unmap_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int);
    dma_addr_t (*map_resource)(struct device *, phys_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*unmap_resource)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int);
    void (*sync_single_for_cpu)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_single_for_device)(struct device *, dma_addr_t, size_t, enum dma_data_direction);
    void (*sync_sg_for_cpu)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*sync_sg_for_device)(struct device *, struct scatterlist *, int, enum dma_data_direction);
    void (*cache_sync)(struct device *, void *, size_t, enum dma_data_direction);
    int (*dma_supported)(struct device *, u64);
    u64 (*get_required_mask)(struct device *);
    size_t (*max_mapping_size)(struct device *);
    long unsigned int (*get_merge_boundary)(struct device *);
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
<code>void * (*alloc)(struct device *, size_t, dma_addr_t *, gfp_t, struct dma_attrs *)</code> ➡️ <code>void * (*alloc)(struct device *, size_t, dma_addr_t *, gfp_t, long unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*free)(struct device *, size_t, void *, dma_addr_t, struct dma_attrs *)</code> ➡️ <code>void (*free)(struct device *, size_t, void *, dma_addr_t, long unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*mmap)(struct device *, struct vm_area_struct *, void *, dma_addr_t, size_t, struct dma_attrs *)</code> ➡️ <code>int (*mmap)(struct device *, struct vm_area_struct *, void *, dma_addr_t, size_t, long unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*get_sgtable)(struct device *, struct sg_table *, void *, dma_addr_t, size_t, struct dma_attrs *)</code> ➡️ <code>int (*get_sgtable)(struct device *, struct sg_table *, void *, dma_addr_t, size_t, long unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>dma_addr_t (*map_page)(struct device *, struct page *, long unsigned int, size_t, enum dma_data_direction, struct dma_attrs *)</code> ➡️ <code>dma_addr_t (*map_page)(struct device *, struct page *, long unsigned int, size_t, enum dma_data_direction, long unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*unmap_page)(struct device *, dma_addr_t, size_t, enum dma_data_direction, struct dma_attrs *)</code> ➡️ <code>void (*unmap_page)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*map_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, struct dma_attrs *)</code> ➡️ <code>int (*map_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*unmap_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, struct dma_attrs *)</code> ➡️ <code>void (*unmap_sg)(struct device *, struct scatterlist *, int, enum dma_data_direction, long unsigned int)</code>
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
<code>dma_addr_t (*map_resource)(struct device *, phys_addr_t, size_t, enum dma_data_direction, long unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*unmap_resource)(struct device *, dma_addr_t, size_t, enum dma_data_direction, long unsigned int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*set_dma_mask)(struct device *, u64)</code>
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
<code>void (*cache_sync)(struct device *, void *, size_t, enum dma_data_direction)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int is_phys</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 (*get_required_mask)(struct device *)</code>
</li>
<li>
<b>Field added. </b>
<code>size_t (*max_mapping_size)(struct device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*mapping_error)(struct device *, dma_addr_t)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int (*get_merge_boundary)(struct device *)</code>
</li>
</ul>
</details>
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
<code>struct page * (*alloc_pages)(struct device *, size_t, dma_addr_t *, enum dma_data_direction, gfp_t)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*free_pages)(struct device *, size_t, struct page *, dma_addr_t, enum dma_data_direction)</code>
</li>
<li>
<b>Field added. </b>
<code>void * (*alloc_noncoherent)(struct device *, size_t, dma_addr_t *, enum dma_data_direction, gfp_t)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*free_noncoherent)(struct device *, size_t, void *, dma_addr_t, enum dma_data_direction)</code>
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
<code>struct sg_table * (*alloc_noncontiguous)(struct device *, size_t, enum dma_data_direction, gfp_t, long unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*free_noncontiguous)(struct device *, size_t, struct sg_table *, enum dma_data_direction)</code>
</li>
<li>
<b>Field removed. </b>
<code>void * (*alloc_noncoherent)(struct device *, size_t, dma_addr_t *, enum dma_data_direction, gfp_t)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*free_noncoherent)(struct device *, size_t, void *, dma_addr_t, enum dma_data_direction)</code>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int flags</code>
</li>
<li>
<b>Field added. </b>
<code>size_t (*opt_mapping_size)()</code>
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
