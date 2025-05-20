# Struct: <code>agp_bridge_driver</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct agp_bridge_driver {
    struct module *owner;
    const void *aperture_sizes;
    int num_aperture_sizes;
    enum aper_size_type size_type;
    bool cant_use_aperture;
    bool needs_scratch_page;
    const struct gatt_mask *masks;
    int (*fetch_size)();
    int (*configure)();
    void (*agp_enable)(struct agp_bridge_data *, u32);
    void (*cleanup)();
    void (*tlb_flush)(struct agp_memory *);
    long unsigned int (*mask_memory)(struct agp_bridge_data *, dma_addr_t, int);
    void (*cache_flush)();
    int (*create_gatt_table)(struct agp_bridge_data *);
    int (*free_gatt_table)(struct agp_bridge_data *);
    int (*insert_memory)(struct agp_memory *, off_t, int);
    int (*remove_memory)(struct agp_memory *, off_t, int);
    struct agp_memory * (*alloc_by_type)(size_t, int);
    void (*free_by_type)(struct agp_memory *);
    struct page * (*agp_alloc_page)(struct agp_bridge_data *);
    int (*agp_alloc_pages)(struct agp_bridge_data *, struct agp_memory *, size_t);
    void (*agp_destroy_page)(struct page *, int);
    void (*agp_destroy_pages)(struct agp_memory *);
    int (*agp_type_to_mask_type)(struct agp_bridge_data *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct agp_bridge_driver {
    struct module *owner;
    const void *aperture_sizes;
    int num_aperture_sizes;
    enum aper_size_type size_type;
    bool cant_use_aperture;
    bool needs_scratch_page;
    const struct gatt_mask *masks;
    int (*fetch_size)();
    int (*configure)();
    void (*agp_enable)(struct agp_bridge_data *, u32);
    void (*cleanup)();
    void (*tlb_flush)(struct agp_memory *);
    long unsigned int (*mask_memory)(struct agp_bridge_data *, dma_addr_t, int);
    void (*cache_flush)();
    int (*create_gatt_table)(struct agp_bridge_data *);
    int (*free_gatt_table)(struct agp_bridge_data *);
    int (*insert_memory)(struct agp_memory *, off_t, int);
    int (*remove_memory)(struct agp_memory *, off_t, int);
    struct agp_memory * (*alloc_by_type)(size_t, int);
    void (*free_by_type)(struct agp_memory *);
    struct page * (*agp_alloc_page)(struct agp_bridge_data *);
    int (*agp_alloc_pages)(struct agp_bridge_data *, struct agp_memory *, size_t);
    void (*agp_destroy_page)(struct page *, int);
    void (*agp_destroy_pages)(struct agp_memory *);
    int (*agp_type_to_mask_type)(struct agp_bridge_data *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct agp_bridge_driver {
    struct module *owner;
    const void *aperture_sizes;
    int num_aperture_sizes;
    enum aper_size_type size_type;
    bool cant_use_aperture;
    bool needs_scratch_page;
    const struct gatt_mask *masks;
    int (*fetch_size)();
    int (*configure)();
    void (*agp_enable)(struct agp_bridge_data *, u32);
    void (*cleanup)();
    void (*tlb_flush)(struct agp_memory *);
    long unsigned int (*mask_memory)(struct agp_bridge_data *, dma_addr_t, int);
    void (*cache_flush)();
    int (*create_gatt_table)(struct agp_bridge_data *);
    int (*free_gatt_table)(struct agp_bridge_data *);
    int (*insert_memory)(struct agp_memory *, off_t, int);
    int (*remove_memory)(struct agp_memory *, off_t, int);
    struct agp_memory * (*alloc_by_type)(size_t, int);
    void (*free_by_type)(struct agp_memory *);
    struct page * (*agp_alloc_page)(struct agp_bridge_data *);
    int (*agp_alloc_pages)(struct agp_bridge_data *, struct agp_memory *, size_t);
    void (*agp_destroy_page)(struct page *, int);
    void (*agp_destroy_pages)(struct agp_memory *);
    int (*agp_type_to_mask_type)(struct agp_bridge_data *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct agp_bridge_driver {
    struct module *owner;
    const void *aperture_sizes;
    int num_aperture_sizes;
    enum aper_size_type size_type;
    bool cant_use_aperture;
    bool needs_scratch_page;
    const struct gatt_mask *masks;
    int (*fetch_size)();
    int (*configure)();
    void (*agp_enable)(struct agp_bridge_data *, u32);
    void (*cleanup)();
    void (*tlb_flush)(struct agp_memory *);
    long unsigned int (*mask_memory)(struct agp_bridge_data *, dma_addr_t, int);
    void (*cache_flush)();
    int (*create_gatt_table)(struct agp_bridge_data *);
    int (*free_gatt_table)(struct agp_bridge_data *);
    int (*insert_memory)(struct agp_memory *, off_t, int);
    int (*remove_memory)(struct agp_memory *, off_t, int);
    struct agp_memory * (*alloc_by_type)(size_t, int);
    void (*free_by_type)(struct agp_memory *);
    struct page * (*agp_alloc_page)(struct agp_bridge_data *);
    int (*agp_alloc_pages)(struct agp_bridge_data *, struct agp_memory *, size_t);
    void (*agp_destroy_page)(struct page *, int);
    void (*agp_destroy_pages)(struct agp_memory *);
    int (*agp_type_to_mask_type)(struct agp_bridge_data *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct agp_bridge_driver {
    struct module *owner;
    const void *aperture_sizes;
    int num_aperture_sizes;
    enum aper_size_type size_type;
    bool cant_use_aperture;
    bool needs_scratch_page;
    const struct gatt_mask *masks;
    int (*fetch_size)();
    int (*configure)();
    void (*agp_enable)(struct agp_bridge_data *, u32);
    void (*cleanup)();
    void (*tlb_flush)(struct agp_memory *);
    long unsigned int (*mask_memory)(struct agp_bridge_data *, dma_addr_t, int);
    void (*cache_flush)();
    int (*create_gatt_table)(struct agp_bridge_data *);
    int (*free_gatt_table)(struct agp_bridge_data *);
    int (*insert_memory)(struct agp_memory *, off_t, int);
    int (*remove_memory)(struct agp_memory *, off_t, int);
    struct agp_memory * (*alloc_by_type)(size_t, int);
    void (*free_by_type)(struct agp_memory *);
    struct page * (*agp_alloc_page)(struct agp_bridge_data *);
    int (*agp_alloc_pages)(struct agp_bridge_data *, struct agp_memory *, size_t);
    void (*agp_destroy_page)(struct page *, int);
    void (*agp_destroy_pages)(struct agp_memory *);
    int (*agp_type_to_mask_type)(struct agp_bridge_data *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct agp_bridge_driver {
    struct module *owner;
    const void *aperture_sizes;
    int num_aperture_sizes;
    enum aper_size_type size_type;
    bool cant_use_aperture;
    bool needs_scratch_page;
    const struct gatt_mask *masks;
    int (*fetch_size)();
    int (*configure)();
    void (*agp_enable)(struct agp_bridge_data *, u32);
    void (*cleanup)();
    void (*tlb_flush)(struct agp_memory *);
    long unsigned int (*mask_memory)(struct agp_bridge_data *, dma_addr_t, int);
    void (*cache_flush)();
    int (*create_gatt_table)(struct agp_bridge_data *);
    int (*free_gatt_table)(struct agp_bridge_data *);
    int (*insert_memory)(struct agp_memory *, off_t, int);
    int (*remove_memory)(struct agp_memory *, off_t, int);
    struct agp_memory * (*alloc_by_type)(size_t, int);
    void (*free_by_type)(struct agp_memory *);
    struct page * (*agp_alloc_page)(struct agp_bridge_data *);
    int (*agp_alloc_pages)(struct agp_bridge_data *, struct agp_memory *, size_t);
    void (*agp_destroy_page)(struct page *, int);
    void (*agp_destroy_pages)(struct agp_memory *);
    int (*agp_type_to_mask_type)(struct agp_bridge_data *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct agp_bridge_driver {
    struct module *owner;
    const void *aperture_sizes;
    int num_aperture_sizes;
    enum aper_size_type size_type;
    bool cant_use_aperture;
    bool needs_scratch_page;
    const struct gatt_mask *masks;
    int (*fetch_size)();
    int (*configure)();
    void (*agp_enable)(struct agp_bridge_data *, u32);
    void (*cleanup)();
    void (*tlb_flush)(struct agp_memory *);
    long unsigned int (*mask_memory)(struct agp_bridge_data *, dma_addr_t, int);
    void (*cache_flush)();
    int (*create_gatt_table)(struct agp_bridge_data *);
    int (*free_gatt_table)(struct agp_bridge_data *);
    int (*insert_memory)(struct agp_memory *, off_t, int);
    int (*remove_memory)(struct agp_memory *, off_t, int);
    struct agp_memory * (*alloc_by_type)(size_t, int);
    void (*free_by_type)(struct agp_memory *);
    struct page * (*agp_alloc_page)(struct agp_bridge_data *);
    int (*agp_alloc_pages)(struct agp_bridge_data *, struct agp_memory *, size_t);
    void (*agp_destroy_page)(struct page *, int);
    void (*agp_destroy_pages)(struct agp_memory *);
    int (*agp_type_to_mask_type)(struct agp_bridge_data *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct agp_bridge_driver {
    struct module *owner;
    const void *aperture_sizes;
    int num_aperture_sizes;
    enum aper_size_type size_type;
    bool cant_use_aperture;
    bool needs_scratch_page;
    const struct gatt_mask *masks;
    int (*fetch_size)();
    int (*configure)();
    void (*agp_enable)(struct agp_bridge_data *, u32);
    void (*cleanup)();
    void (*tlb_flush)(struct agp_memory *);
    long unsigned int (*mask_memory)(struct agp_bridge_data *, dma_addr_t, int);
    void (*cache_flush)();
    int (*create_gatt_table)(struct agp_bridge_data *);
    int (*free_gatt_table)(struct agp_bridge_data *);
    int (*insert_memory)(struct agp_memory *, off_t, int);
    int (*remove_memory)(struct agp_memory *, off_t, int);
    struct agp_memory * (*alloc_by_type)(size_t, int);
    void (*free_by_type)(struct agp_memory *);
    struct page * (*agp_alloc_page)(struct agp_bridge_data *);
    int (*agp_alloc_pages)(struct agp_bridge_data *, struct agp_memory *, size_t);
    void (*agp_destroy_page)(struct page *, int);
    void (*agp_destroy_pages)(struct agp_memory *);
    int (*agp_type_to_mask_type)(struct agp_bridge_data *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct agp_bridge_driver {
    struct module *owner;
    const void *aperture_sizes;
    int num_aperture_sizes;
    enum aper_size_type size_type;
    bool cant_use_aperture;
    bool needs_scratch_page;
    const struct gatt_mask *masks;
    int (*fetch_size)();
    int (*configure)();
    void (*agp_enable)(struct agp_bridge_data *, u32);
    void (*cleanup)();
    void (*tlb_flush)(struct agp_memory *);
    long unsigned int (*mask_memory)(struct agp_bridge_data *, dma_addr_t, int);
    void (*cache_flush)();
    int (*create_gatt_table)(struct agp_bridge_data *);
    int (*free_gatt_table)(struct agp_bridge_data *);
    int (*insert_memory)(struct agp_memory *, off_t, int);
    int (*remove_memory)(struct agp_memory *, off_t, int);
    struct agp_memory * (*alloc_by_type)(size_t, int);
    void (*free_by_type)(struct agp_memory *);
    struct page * (*agp_alloc_page)(struct agp_bridge_data *);
    int (*agp_alloc_pages)(struct agp_bridge_data *, struct agp_memory *, size_t);
    void (*agp_destroy_page)(struct page *, int);
    void (*agp_destroy_pages)(struct agp_memory *);
    int (*agp_type_to_mask_type)(struct agp_bridge_data *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct agp_bridge_driver {
    struct module *owner;
    const void *aperture_sizes;
    int num_aperture_sizes;
    enum aper_size_type size_type;
    bool cant_use_aperture;
    bool needs_scratch_page;
    const struct gatt_mask *masks;
    int (*fetch_size)();
    int (*configure)();
    void (*agp_enable)(struct agp_bridge_data *, u32);
    void (*cleanup)();
    void (*tlb_flush)(struct agp_memory *);
    long unsigned int (*mask_memory)(struct agp_bridge_data *, dma_addr_t, int);
    void (*cache_flush)();
    int (*create_gatt_table)(struct agp_bridge_data *);
    int (*free_gatt_table)(struct agp_bridge_data *);
    int (*insert_memory)(struct agp_memory *, off_t, int);
    int (*remove_memory)(struct agp_memory *, off_t, int);
    struct agp_memory * (*alloc_by_type)(size_t, int);
    void (*free_by_type)(struct agp_memory *);
    struct page * (*agp_alloc_page)(struct agp_bridge_data *);
    int (*agp_alloc_pages)(struct agp_bridge_data *, struct agp_memory *, size_t);
    void (*agp_destroy_page)(struct page *, int);
    void (*agp_destroy_pages)(struct agp_memory *);
    int (*agp_type_to_mask_type)(struct agp_bridge_data *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct agp_bridge_driver {
    struct module *owner;
    const void *aperture_sizes;
    int num_aperture_sizes;
    enum aper_size_type size_type;
    bool cant_use_aperture;
    bool needs_scratch_page;
    const struct gatt_mask *masks;
    int (*fetch_size)();
    int (*configure)();
    void (*agp_enable)(struct agp_bridge_data *, u32);
    void (*cleanup)();
    void (*tlb_flush)(struct agp_memory *);
    long unsigned int (*mask_memory)(struct agp_bridge_data *, dma_addr_t, int);
    void (*cache_flush)();
    int (*create_gatt_table)(struct agp_bridge_data *);
    int (*free_gatt_table)(struct agp_bridge_data *);
    int (*insert_memory)(struct agp_memory *, off_t, int);
    int (*remove_memory)(struct agp_memory *, off_t, int);
    struct agp_memory * (*alloc_by_type)(size_t, int);
    void (*free_by_type)(struct agp_memory *);
    struct page * (*agp_alloc_page)(struct agp_bridge_data *);
    int (*agp_alloc_pages)(struct agp_bridge_data *, struct agp_memory *, size_t);
    void (*agp_destroy_page)(struct page *, int);
    void (*agp_destroy_pages)(struct agp_memory *);
    int (*agp_type_to_mask_type)(struct agp_bridge_data *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct agp_bridge_driver {
    struct module *owner;
    const void *aperture_sizes;
    int num_aperture_sizes;
    enum aper_size_type size_type;
    bool cant_use_aperture;
    bool needs_scratch_page;
    const struct gatt_mask *masks;
    int (*fetch_size)();
    int (*configure)();
    void (*agp_enable)(struct agp_bridge_data *, u32);
    void (*cleanup)();
    void (*tlb_flush)(struct agp_memory *);
    long unsigned int (*mask_memory)(struct agp_bridge_data *, dma_addr_t, int);
    void (*cache_flush)();
    int (*create_gatt_table)(struct agp_bridge_data *);
    int (*free_gatt_table)(struct agp_bridge_data *);
    int (*insert_memory)(struct agp_memory *, off_t, int);
    int (*remove_memory)(struct agp_memory *, off_t, int);
    struct agp_memory * (*alloc_by_type)(size_t, int);
    void (*free_by_type)(struct agp_memory *);
    struct page * (*agp_alloc_page)(struct agp_bridge_data *);
    int (*agp_alloc_pages)(struct agp_bridge_data *, struct agp_memory *, size_t);
    void (*agp_destroy_page)(struct page *, int);
    void (*agp_destroy_pages)(struct agp_memory *);
    int (*agp_type_to_mask_type)(struct agp_bridge_data *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct agp_bridge_driver {
    struct module *owner;
    const void *aperture_sizes;
    int num_aperture_sizes;
    enum aper_size_type size_type;
    bool cant_use_aperture;
    bool needs_scratch_page;
    const struct gatt_mask *masks;
    int (*fetch_size)();
    int (*configure)();
    void (*agp_enable)(struct agp_bridge_data *, u32);
    void (*cleanup)();
    void (*tlb_flush)(struct agp_memory *);
    long unsigned int (*mask_memory)(struct agp_bridge_data *, dma_addr_t, int);
    void (*cache_flush)();
    int (*create_gatt_table)(struct agp_bridge_data *);
    int (*free_gatt_table)(struct agp_bridge_data *);
    int (*insert_memory)(struct agp_memory *, off_t, int);
    int (*remove_memory)(struct agp_memory *, off_t, int);
    struct agp_memory * (*alloc_by_type)(size_t, int);
    void (*free_by_type)(struct agp_memory *);
    struct page * (*agp_alloc_page)(struct agp_bridge_data *);
    int (*agp_alloc_pages)(struct agp_bridge_data *, struct agp_memory *, size_t);
    void (*agp_destroy_page)(struct page *, int);
    void (*agp_destroy_pages)(struct agp_memory *);
    int (*agp_type_to_mask_type)(struct agp_bridge_data *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct agp_bridge_driver {
    struct module *owner;
    const void *aperture_sizes;
    int num_aperture_sizes;
    enum aper_size_type size_type;
    bool cant_use_aperture;
    bool needs_scratch_page;
    const struct gatt_mask *masks;
    int (*fetch_size)();
    int (*configure)();
    void (*agp_enable)(struct agp_bridge_data *, u32);
    void (*cleanup)();
    void (*tlb_flush)(struct agp_memory *);
    long unsigned int (*mask_memory)(struct agp_bridge_data *, dma_addr_t, int);
    void (*cache_flush)();
    int (*create_gatt_table)(struct agp_bridge_data *);
    int (*free_gatt_table)(struct agp_bridge_data *);
    int (*insert_memory)(struct agp_memory *, off_t, int);
    int (*remove_memory)(struct agp_memory *, off_t, int);
    struct agp_memory * (*alloc_by_type)(size_t, int);
    void (*free_by_type)(struct agp_memory *);
    struct page * (*agp_alloc_page)(struct agp_bridge_data *);
    int (*agp_alloc_pages)(struct agp_bridge_data *, struct agp_memory *, size_t);
    void (*agp_destroy_page)(struct page *, int);
    void (*agp_destroy_pages)(struct agp_memory *);
    int (*agp_type_to_mask_type)(struct agp_bridge_data *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct agp_bridge_driver {
    struct module *owner;
    const void *aperture_sizes;
    int num_aperture_sizes;
    enum aper_size_type size_type;
    bool cant_use_aperture;
    bool needs_scratch_page;
    const struct gatt_mask *masks;
    int (*fetch_size)();
    int (*configure)();
    void (*agp_enable)(struct agp_bridge_data *, u32);
    void (*cleanup)();
    void (*tlb_flush)(struct agp_memory *);
    long unsigned int (*mask_memory)(struct agp_bridge_data *, dma_addr_t, int);
    void (*cache_flush)();
    int (*create_gatt_table)(struct agp_bridge_data *);
    int (*free_gatt_table)(struct agp_bridge_data *);
    int (*insert_memory)(struct agp_memory *, off_t, int);
    int (*remove_memory)(struct agp_memory *, off_t, int);
    struct agp_memory * (*alloc_by_type)(size_t, int);
    void (*free_by_type)(struct agp_memory *);
    struct page * (*agp_alloc_page)(struct agp_bridge_data *);
    int (*agp_alloc_pages)(struct agp_bridge_data *, struct agp_memory *, size_t);
    void (*agp_destroy_page)(struct page *, int);
    void (*agp_destroy_pages)(struct agp_memory *);
    int (*agp_type_to_mask_type)(struct agp_bridge_data *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct agp_bridge_driver {
    struct module *owner;
    const void *aperture_sizes;
    int num_aperture_sizes;
    enum aper_size_type size_type;
    bool cant_use_aperture;
    bool needs_scratch_page;
    const struct gatt_mask *masks;
    int (*fetch_size)();
    int (*configure)();
    void (*agp_enable)(struct agp_bridge_data *, u32);
    void (*cleanup)();
    void (*tlb_flush)(struct agp_memory *);
    long unsigned int (*mask_memory)(struct agp_bridge_data *, dma_addr_t, int);
    void (*cache_flush)();
    int (*create_gatt_table)(struct agp_bridge_data *);
    int (*free_gatt_table)(struct agp_bridge_data *);
    int (*insert_memory)(struct agp_memory *, off_t, int);
    int (*remove_memory)(struct agp_memory *, off_t, int);
    struct agp_memory * (*alloc_by_type)(size_t, int);
    void (*free_by_type)(struct agp_memory *);
    struct page * (*agp_alloc_page)(struct agp_bridge_data *);
    int (*agp_alloc_pages)(struct agp_bridge_data *, struct agp_memory *, size_t);
    void (*agp_destroy_page)(struct page *, int);
    void (*agp_destroy_pages)(struct agp_memory *);
    int (*agp_type_to_mask_type)(struct agp_bridge_data *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct agp_bridge_driver {
    struct module *owner;
    const void *aperture_sizes;
    int num_aperture_sizes;
    enum aper_size_type size_type;
    bool cant_use_aperture;
    bool needs_scratch_page;
    const struct gatt_mask *masks;
    int (*fetch_size)();
    int (*configure)();
    void (*agp_enable)(struct agp_bridge_data *, u32);
    void (*cleanup)();
    void (*tlb_flush)(struct agp_memory *);
    long unsigned int (*mask_memory)(struct agp_bridge_data *, dma_addr_t, int);
    void (*cache_flush)();
    int (*create_gatt_table)(struct agp_bridge_data *);
    int (*free_gatt_table)(struct agp_bridge_data *);
    int (*insert_memory)(struct agp_memory *, off_t, int);
    int (*remove_memory)(struct agp_memory *, off_t, int);
    struct agp_memory * (*alloc_by_type)(size_t, int);
    void (*free_by_type)(struct agp_memory *);
    struct page * (*agp_alloc_page)(struct agp_bridge_data *);
    int (*agp_alloc_pages)(struct agp_bridge_data *, struct agp_memory *, size_t);
    void (*agp_destroy_page)(struct page *, int);
    void (*agp_destroy_pages)(struct agp_memory *);
    int (*agp_type_to_mask_type)(struct agp_bridge_data *, int);
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
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct agp_bridge_driver {
    struct module *owner;
    const void *aperture_sizes;
    int num_aperture_sizes;
    enum aper_size_type size_type;
    bool cant_use_aperture;
    bool needs_scratch_page;
    const struct gatt_mask *masks;
    int (*fetch_size)();
    int (*configure)();
    void (*agp_enable)(struct agp_bridge_data *, u32);
    void (*cleanup)();
    void (*tlb_flush)(struct agp_memory *);
    long unsigned int (*mask_memory)(struct agp_bridge_data *, dma_addr_t, int);
    void (*cache_flush)();
    int (*create_gatt_table)(struct agp_bridge_data *);
    int (*free_gatt_table)(struct agp_bridge_data *);
    int (*insert_memory)(struct agp_memory *, off_t, int);
    int (*remove_memory)(struct agp_memory *, off_t, int);
    struct agp_memory * (*alloc_by_type)(size_t, int);
    void (*free_by_type)(struct agp_memory *);
    struct page * (*agp_alloc_page)(struct agp_bridge_data *);
    int (*agp_alloc_pages)(struct agp_bridge_data *, struct agp_memory *, size_t);
    void (*agp_destroy_page)(struct page *, int);
    void (*agp_destroy_pages)(struct agp_memory *);
    int (*agp_type_to_mask_type)(struct agp_bridge_data *, int);
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
struct agp_bridge_driver {
    struct module *owner;
    const void *aperture_sizes;
    int num_aperture_sizes;
    enum aper_size_type size_type;
    bool cant_use_aperture;
    bool needs_scratch_page;
    const struct gatt_mask *masks;
    int (*fetch_size)();
    int (*configure)();
    void (*agp_enable)(struct agp_bridge_data *, u32);
    void (*cleanup)();
    void (*tlb_flush)(struct agp_memory *);
    long unsigned int (*mask_memory)(struct agp_bridge_data *, dma_addr_t, int);
    void (*cache_flush)();
    int (*create_gatt_table)(struct agp_bridge_data *);
    int (*free_gatt_table)(struct agp_bridge_data *);
    int (*insert_memory)(struct agp_memory *, off_t, int);
    int (*remove_memory)(struct agp_memory *, off_t, int);
    struct agp_memory * (*alloc_by_type)(size_t, int);
    void (*free_by_type)(struct agp_memory *);
    struct page * (*agp_alloc_page)(struct agp_bridge_data *);
    int (*agp_alloc_pages)(struct agp_bridge_data *, struct agp_memory *, size_t);
    void (*agp_destroy_page)(struct page *, int);
    void (*agp_destroy_pages)(struct agp_memory *);
    int (*agp_type_to_mask_type)(struct agp_bridge_data *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct agp_bridge_driver {
    struct module *owner;
    const void *aperture_sizes;
    int num_aperture_sizes;
    enum aper_size_type size_type;
    bool cant_use_aperture;
    bool needs_scratch_page;
    const struct gatt_mask *masks;
    int (*fetch_size)();
    int (*configure)();
    void (*agp_enable)(struct agp_bridge_data *, u32);
    void (*cleanup)();
    void (*tlb_flush)(struct agp_memory *);
    long unsigned int (*mask_memory)(struct agp_bridge_data *, dma_addr_t, int);
    void (*cache_flush)();
    int (*create_gatt_table)(struct agp_bridge_data *);
    int (*free_gatt_table)(struct agp_bridge_data *);
    int (*insert_memory)(struct agp_memory *, off_t, int);
    int (*remove_memory)(struct agp_memory *, off_t, int);
    struct agp_memory * (*alloc_by_type)(size_t, int);
    void (*free_by_type)(struct agp_memory *);
    struct page * (*agp_alloc_page)(struct agp_bridge_data *);
    int (*agp_alloc_pages)(struct agp_bridge_data *, struct agp_memory *, size_t);
    void (*agp_destroy_page)(struct page *, int);
    void (*agp_destroy_pages)(struct agp_memory *);
    int (*agp_type_to_mask_type)(struct agp_bridge_data *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct agp_bridge_driver {
    struct module *owner;
    const void *aperture_sizes;
    int num_aperture_sizes;
    enum aper_size_type size_type;
    bool cant_use_aperture;
    bool needs_scratch_page;
    const struct gatt_mask *masks;
    int (*fetch_size)();
    int (*configure)();
    void (*agp_enable)(struct agp_bridge_data *, u32);
    void (*cleanup)();
    void (*tlb_flush)(struct agp_memory *);
    long unsigned int (*mask_memory)(struct agp_bridge_data *, dma_addr_t, int);
    void (*cache_flush)();
    int (*create_gatt_table)(struct agp_bridge_data *);
    int (*free_gatt_table)(struct agp_bridge_data *);
    int (*insert_memory)(struct agp_memory *, off_t, int);
    int (*remove_memory)(struct agp_memory *, off_t, int);
    struct agp_memory * (*alloc_by_type)(size_t, int);
    void (*free_by_type)(struct agp_memory *);
    struct page * (*agp_alloc_page)(struct agp_bridge_data *);
    int (*agp_alloc_pages)(struct agp_bridge_data *, struct agp_memory *, size_t);
    void (*agp_destroy_page)(struct page *, int);
    void (*agp_destroy_pages)(struct agp_memory *);
    int (*agp_type_to_mask_type)(struct agp_bridge_data *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct agp_bridge_driver {
    struct module *owner;
    const void *aperture_sizes;
    int num_aperture_sizes;
    enum aper_size_type size_type;
    bool cant_use_aperture;
    bool needs_scratch_page;
    const struct gatt_mask *masks;
    int (*fetch_size)();
    int (*configure)();
    void (*agp_enable)(struct agp_bridge_data *, u32);
    void (*cleanup)();
    void (*tlb_flush)(struct agp_memory *);
    long unsigned int (*mask_memory)(struct agp_bridge_data *, dma_addr_t, int);
    void (*cache_flush)();
    int (*create_gatt_table)(struct agp_bridge_data *);
    int (*free_gatt_table)(struct agp_bridge_data *);
    int (*insert_memory)(struct agp_memory *, off_t, int);
    int (*remove_memory)(struct agp_memory *, off_t, int);
    struct agp_memory * (*alloc_by_type)(size_t, int);
    void (*free_by_type)(struct agp_memory *);
    struct page * (*agp_alloc_page)(struct agp_bridge_data *);
    int (*agp_alloc_pages)(struct agp_bridge_data *, struct agp_memory *, size_t);
    void (*agp_destroy_page)(struct page *, int);
    void (*agp_destroy_pages)(struct agp_memory *);
    int (*agp_type_to_mask_type)(struct agp_bridge_data *, int);
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
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
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
