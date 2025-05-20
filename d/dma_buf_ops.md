# Struct: <code>dma_buf_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct dma_buf_ops {
    int (*attach)(struct dma_buf *, struct device *, struct dma_buf_attachment *);
    void (*detach)(struct dma_buf *, struct dma_buf_attachment *);
    struct sg_table * (*map_dma_buf)(struct dma_buf_attachment *, enum dma_data_direction);
    void (*unmap_dma_buf)(struct dma_buf_attachment *, struct sg_table *, enum dma_data_direction);
    void (*release)(struct dma_buf *);
    int (*begin_cpu_access)(struct dma_buf *, size_t, size_t, enum dma_data_direction);
    void (*end_cpu_access)(struct dma_buf *, size_t, size_t, enum dma_data_direction);
    void * (*kmap_atomic)(struct dma_buf *, long unsigned int);
    void (*kunmap_atomic)(struct dma_buf *, long unsigned int, void *);
    void * (*kmap)(struct dma_buf *, long unsigned int);
    void (*kunmap)(struct dma_buf *, long unsigned int, void *);
    int (*mmap)(struct dma_buf *, struct vm_area_struct *);
    void * (*vmap)(struct dma_buf *);
    void (*vunmap)(struct dma_buf *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct dma_buf_ops {
    int (*attach)(struct dma_buf *, struct device *, struct dma_buf_attachment *);
    void (*detach)(struct dma_buf *, struct dma_buf_attachment *);
    struct sg_table * (*map_dma_buf)(struct dma_buf_attachment *, enum dma_data_direction);
    void (*unmap_dma_buf)(struct dma_buf_attachment *, struct sg_table *, enum dma_data_direction);
    void (*release)(struct dma_buf *);
    int (*begin_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*end_cpu_access)(struct dma_buf *, enum dma_data_direction);
    void * (*kmap_atomic)(struct dma_buf *, long unsigned int);
    void (*kunmap_atomic)(struct dma_buf *, long unsigned int, void *);
    void * (*kmap)(struct dma_buf *, long unsigned int);
    void (*kunmap)(struct dma_buf *, long unsigned int, void *);
    int (*mmap)(struct dma_buf *, struct vm_area_struct *);
    void * (*vmap)(struct dma_buf *);
    void (*vunmap)(struct dma_buf *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct dma_buf_ops {
    int (*attach)(struct dma_buf *, struct device *, struct dma_buf_attachment *);
    void (*detach)(struct dma_buf *, struct dma_buf_attachment *);
    struct sg_table * (*map_dma_buf)(struct dma_buf_attachment *, enum dma_data_direction);
    void (*unmap_dma_buf)(struct dma_buf_attachment *, struct sg_table *, enum dma_data_direction);
    void (*release)(struct dma_buf *);
    int (*begin_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*end_cpu_access)(struct dma_buf *, enum dma_data_direction);
    void * (*kmap_atomic)(struct dma_buf *, long unsigned int);
    void (*kunmap_atomic)(struct dma_buf *, long unsigned int, void *);
    void * (*kmap)(struct dma_buf *, long unsigned int);
    void (*kunmap)(struct dma_buf *, long unsigned int, void *);
    int (*mmap)(struct dma_buf *, struct vm_area_struct *);
    void * (*vmap)(struct dma_buf *);
    void (*vunmap)(struct dma_buf *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct dma_buf_ops {
    int (*attach)(struct dma_buf *, struct device *, struct dma_buf_attachment *);
    void (*detach)(struct dma_buf *, struct dma_buf_attachment *);
    struct sg_table * (*map_dma_buf)(struct dma_buf_attachment *, enum dma_data_direction);
    void (*unmap_dma_buf)(struct dma_buf_attachment *, struct sg_table *, enum dma_data_direction);
    void (*release)(struct dma_buf *);
    int (*begin_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*end_cpu_access)(struct dma_buf *, enum dma_data_direction);
    void * (*map_atomic)(struct dma_buf *, long unsigned int);
    void (*unmap_atomic)(struct dma_buf *, long unsigned int, void *);
    void * (*map)(struct dma_buf *, long unsigned int);
    void (*unmap)(struct dma_buf *, long unsigned int, void *);
    int (*mmap)(struct dma_buf *, struct vm_area_struct *);
    void * (*vmap)(struct dma_buf *);
    void (*vunmap)(struct dma_buf *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dma_buf_ops {
    int (*attach)(struct dma_buf *, struct device *, struct dma_buf_attachment *);
    void (*detach)(struct dma_buf *, struct dma_buf_attachment *);
    struct sg_table * (*map_dma_buf)(struct dma_buf_attachment *, enum dma_data_direction);
    void (*unmap_dma_buf)(struct dma_buf_attachment *, struct sg_table *, enum dma_data_direction);
    void (*release)(struct dma_buf *);
    int (*begin_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*end_cpu_access)(struct dma_buf *, enum dma_data_direction);
    void * (*map_atomic)(struct dma_buf *, long unsigned int);
    void (*unmap_atomic)(struct dma_buf *, long unsigned int, void *);
    void * (*map)(struct dma_buf *, long unsigned int);
    void (*unmap)(struct dma_buf *, long unsigned int, void *);
    int (*mmap)(struct dma_buf *, struct vm_area_struct *);
    void * (*vmap)(struct dma_buf *);
    void (*vunmap)(struct dma_buf *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dma_buf_ops {
    int (*attach)(struct dma_buf *, struct device *, struct dma_buf_attachment *);
    void (*detach)(struct dma_buf *, struct dma_buf_attachment *);
    struct sg_table * (*map_dma_buf)(struct dma_buf_attachment *, enum dma_data_direction);
    void (*unmap_dma_buf)(struct dma_buf_attachment *, struct sg_table *, enum dma_data_direction);
    void (*release)(struct dma_buf *);
    int (*begin_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*end_cpu_access)(struct dma_buf *, enum dma_data_direction);
    void * (*map_atomic)(struct dma_buf *, long unsigned int);
    void (*unmap_atomic)(struct dma_buf *, long unsigned int, void *);
    void * (*map)(struct dma_buf *, long unsigned int);
    void (*unmap)(struct dma_buf *, long unsigned int, void *);
    int (*mmap)(struct dma_buf *, struct vm_area_struct *);
    void * (*vmap)(struct dma_buf *);
    void (*vunmap)(struct dma_buf *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dma_buf_ops {
    int (*attach)(struct dma_buf *, struct dma_buf_attachment *);
    void (*detach)(struct dma_buf *, struct dma_buf_attachment *);
    struct sg_table * (*map_dma_buf)(struct dma_buf_attachment *, enum dma_data_direction);
    void (*unmap_dma_buf)(struct dma_buf_attachment *, struct sg_table *, enum dma_data_direction);
    void (*release)(struct dma_buf *);
    int (*begin_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*end_cpu_access)(struct dma_buf *, enum dma_data_direction);
    void * (*map)(struct dma_buf *, long unsigned int);
    void (*unmap)(struct dma_buf *, long unsigned int, void *);
    int (*mmap)(struct dma_buf *, struct vm_area_struct *);
    void * (*vmap)(struct dma_buf *);
    void (*vunmap)(struct dma_buf *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dma_buf_ops {
    bool cache_sgt_mapping;
    int (*attach)(struct dma_buf *, struct dma_buf_attachment *);
    void (*detach)(struct dma_buf *, struct dma_buf_attachment *);
    struct sg_table * (*map_dma_buf)(struct dma_buf_attachment *, enum dma_data_direction);
    void (*unmap_dma_buf)(struct dma_buf_attachment *, struct sg_table *, enum dma_data_direction);
    void (*release)(struct dma_buf *);
    int (*begin_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*end_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*mmap)(struct dma_buf *, struct vm_area_struct *);
    void * (*map)(struct dma_buf *, long unsigned int);
    void (*unmap)(struct dma_buf *, long unsigned int, void *);
    void * (*vmap)(struct dma_buf *);
    void (*vunmap)(struct dma_buf *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dma_buf_ops {
    bool cache_sgt_mapping;
    int (*attach)(struct dma_buf *, struct dma_buf_attachment *);
    void (*detach)(struct dma_buf *, struct dma_buf_attachment *);
    struct sg_table * (*map_dma_buf)(struct dma_buf_attachment *, enum dma_data_direction);
    void (*unmap_dma_buf)(struct dma_buf_attachment *, struct sg_table *, enum dma_data_direction);
    void (*release)(struct dma_buf *);
    int (*begin_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*end_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*mmap)(struct dma_buf *, struct vm_area_struct *);
    void * (*map)(struct dma_buf *, long unsigned int);
    void (*unmap)(struct dma_buf *, long unsigned int, void *);
    void * (*vmap)(struct dma_buf *);
    void (*vunmap)(struct dma_buf *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dma_buf_ops {
    bool cache_sgt_mapping;
    int (*attach)(struct dma_buf *, struct dma_buf_attachment *);
    void (*detach)(struct dma_buf *, struct dma_buf_attachment *);
    int (*pin)(struct dma_buf_attachment *);
    void (*unpin)(struct dma_buf_attachment *);
    struct sg_table * (*map_dma_buf)(struct dma_buf_attachment *, enum dma_data_direction);
    void (*unmap_dma_buf)(struct dma_buf_attachment *, struct sg_table *, enum dma_data_direction);
    void (*release)(struct dma_buf *);
    int (*begin_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*end_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*mmap)(struct dma_buf *, struct vm_area_struct *);
    void * (*vmap)(struct dma_buf *);
    void (*vunmap)(struct dma_buf *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dma_buf_ops {
    bool cache_sgt_mapping;
    int (*attach)(struct dma_buf *, struct dma_buf_attachment *);
    void (*detach)(struct dma_buf *, struct dma_buf_attachment *);
    int (*pin)(struct dma_buf_attachment *);
    void (*unpin)(struct dma_buf_attachment *);
    struct sg_table * (*map_dma_buf)(struct dma_buf_attachment *, enum dma_data_direction);
    void (*unmap_dma_buf)(struct dma_buf_attachment *, struct sg_table *, enum dma_data_direction);
    void (*release)(struct dma_buf *);
    int (*begin_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*end_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*mmap)(struct dma_buf *, struct vm_area_struct *);
    int (*vmap)(struct dma_buf *, struct dma_buf_map *);
    void (*vunmap)(struct dma_buf *, struct dma_buf_map *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dma_buf_ops {
    bool cache_sgt_mapping;
    int (*attach)(struct dma_buf *, struct dma_buf_attachment *);
    void (*detach)(struct dma_buf *, struct dma_buf_attachment *);
    int (*pin)(struct dma_buf_attachment *);
    void (*unpin)(struct dma_buf_attachment *);
    struct sg_table * (*map_dma_buf)(struct dma_buf_attachment *, enum dma_data_direction);
    void (*unmap_dma_buf)(struct dma_buf_attachment *, struct sg_table *, enum dma_data_direction);
    void (*release)(struct dma_buf *);
    int (*begin_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*end_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*mmap)(struct dma_buf *, struct vm_area_struct *);
    int (*vmap)(struct dma_buf *, struct dma_buf_map *);
    void (*vunmap)(struct dma_buf *, struct dma_buf_map *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dma_buf_ops {
    bool cache_sgt_mapping;
    int (*attach)(struct dma_buf *, struct dma_buf_attachment *);
    void (*detach)(struct dma_buf *, struct dma_buf_attachment *);
    int (*pin)(struct dma_buf_attachment *);
    void (*unpin)(struct dma_buf_attachment *);
    struct sg_table * (*map_dma_buf)(struct dma_buf_attachment *, enum dma_data_direction);
    void (*unmap_dma_buf)(struct dma_buf_attachment *, struct sg_table *, enum dma_data_direction);
    void (*release)(struct dma_buf *);
    int (*begin_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*end_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*mmap)(struct dma_buf *, struct vm_area_struct *);
    int (*vmap)(struct dma_buf *, struct dma_buf_map *);
    void (*vunmap)(struct dma_buf *, struct dma_buf_map *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dma_buf_ops {
    bool cache_sgt_mapping;
    int (*attach)(struct dma_buf *, struct dma_buf_attachment *);
    void (*detach)(struct dma_buf *, struct dma_buf_attachment *);
    int (*pin)(struct dma_buf_attachment *);
    void (*unpin)(struct dma_buf_attachment *);
    struct sg_table * (*map_dma_buf)(struct dma_buf_attachment *, enum dma_data_direction);
    void (*unmap_dma_buf)(struct dma_buf_attachment *, struct sg_table *, enum dma_data_direction);
    void (*release)(struct dma_buf *);
    int (*begin_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*end_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*mmap)(struct dma_buf *, struct vm_area_struct *);
    int (*vmap)(struct dma_buf *, struct iosys_map *);
    void (*vunmap)(struct dma_buf *, struct iosys_map *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dma_buf_ops {
    bool cache_sgt_mapping;
    int (*attach)(struct dma_buf *, struct dma_buf_attachment *);
    void (*detach)(struct dma_buf *, struct dma_buf_attachment *);
    int (*pin)(struct dma_buf_attachment *);
    void (*unpin)(struct dma_buf_attachment *);
    struct sg_table * (*map_dma_buf)(struct dma_buf_attachment *, enum dma_data_direction);
    void (*unmap_dma_buf)(struct dma_buf_attachment *, struct sg_table *, enum dma_data_direction);
    void (*release)(struct dma_buf *);
    int (*begin_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*end_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*mmap)(struct dma_buf *, struct vm_area_struct *);
    int (*vmap)(struct dma_buf *, struct iosys_map *);
    void (*vunmap)(struct dma_buf *, struct iosys_map *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dma_buf_ops {
    bool cache_sgt_mapping;
    int (*attach)(struct dma_buf *, struct dma_buf_attachment *);
    void (*detach)(struct dma_buf *, struct dma_buf_attachment *);
    int (*pin)(struct dma_buf_attachment *);
    void (*unpin)(struct dma_buf_attachment *);
    struct sg_table * (*map_dma_buf)(struct dma_buf_attachment *, enum dma_data_direction);
    void (*unmap_dma_buf)(struct dma_buf_attachment *, struct sg_table *, enum dma_data_direction);
    void (*release)(struct dma_buf *);
    int (*begin_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*end_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*mmap)(struct dma_buf *, struct vm_area_struct *);
    int (*vmap)(struct dma_buf *, struct iosys_map *);
    void (*vunmap)(struct dma_buf *, struct iosys_map *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dma_buf_ops {
    bool cache_sgt_mapping;
    int (*attach)(struct dma_buf *, struct dma_buf_attachment *);
    void (*detach)(struct dma_buf *, struct dma_buf_attachment *);
    int (*pin)(struct dma_buf_attachment *);
    void (*unpin)(struct dma_buf_attachment *);
    struct sg_table * (*map_dma_buf)(struct dma_buf_attachment *, enum dma_data_direction);
    void (*unmap_dma_buf)(struct dma_buf_attachment *, struct sg_table *, enum dma_data_direction);
    void (*release)(struct dma_buf *);
    int (*begin_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*end_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*mmap)(struct dma_buf *, struct vm_area_struct *);
    int (*vmap)(struct dma_buf *, struct iosys_map *);
    void (*vunmap)(struct dma_buf *, struct iosys_map *);
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
struct dma_buf_ops {
    bool cache_sgt_mapping;
    int (*attach)(struct dma_buf *, struct dma_buf_attachment *);
    void (*detach)(struct dma_buf *, struct dma_buf_attachment *);
    struct sg_table * (*map_dma_buf)(struct dma_buf_attachment *, enum dma_data_direction);
    void (*unmap_dma_buf)(struct dma_buf_attachment *, struct sg_table *, enum dma_data_direction);
    void (*release)(struct dma_buf *);
    int (*begin_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*end_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*mmap)(struct dma_buf *, struct vm_area_struct *);
    void * (*map)(struct dma_buf *, long unsigned int);
    void (*unmap)(struct dma_buf *, long unsigned int, void *);
    void * (*vmap)(struct dma_buf *);
    void (*vunmap)(struct dma_buf *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dma_buf_ops {
    bool cache_sgt_mapping;
    int (*attach)(struct dma_buf *, struct dma_buf_attachment *);
    void (*detach)(struct dma_buf *, struct dma_buf_attachment *);
    struct sg_table * (*map_dma_buf)(struct dma_buf_attachment *, enum dma_data_direction);
    void (*unmap_dma_buf)(struct dma_buf_attachment *, struct sg_table *, enum dma_data_direction);
    void (*release)(struct dma_buf *);
    int (*begin_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*end_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*mmap)(struct dma_buf *, struct vm_area_struct *);
    void * (*map)(struct dma_buf *, long unsigned int);
    void (*unmap)(struct dma_buf *, long unsigned int, void *);
    void * (*vmap)(struct dma_buf *);
    void (*vunmap)(struct dma_buf *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dma_buf_ops {
    bool cache_sgt_mapping;
    int (*attach)(struct dma_buf *, struct dma_buf_attachment *);
    void (*detach)(struct dma_buf *, struct dma_buf_attachment *);
    struct sg_table * (*map_dma_buf)(struct dma_buf_attachment *, enum dma_data_direction);
    void (*unmap_dma_buf)(struct dma_buf_attachment *, struct sg_table *, enum dma_data_direction);
    void (*release)(struct dma_buf *);
    int (*begin_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*end_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*mmap)(struct dma_buf *, struct vm_area_struct *);
    void * (*map)(struct dma_buf *, long unsigned int);
    void (*unmap)(struct dma_buf *, long unsigned int, void *);
    void * (*vmap)(struct dma_buf *);
    void (*vunmap)(struct dma_buf *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dma_buf_ops {
    bool cache_sgt_mapping;
    int (*attach)(struct dma_buf *, struct dma_buf_attachment *);
    void (*detach)(struct dma_buf *, struct dma_buf_attachment *);
    struct sg_table * (*map_dma_buf)(struct dma_buf_attachment *, enum dma_data_direction);
    void (*unmap_dma_buf)(struct dma_buf_attachment *, struct sg_table *, enum dma_data_direction);
    void (*release)(struct dma_buf *);
    int (*begin_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*end_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*mmap)(struct dma_buf *, struct vm_area_struct *);
    void * (*map)(struct dma_buf *, long unsigned int);
    void (*unmap)(struct dma_buf *, long unsigned int, void *);
    void * (*vmap)(struct dma_buf *);
    void (*vunmap)(struct dma_buf *, void *);
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
struct dma_buf_ops {
    bool cache_sgt_mapping;
    int (*attach)(struct dma_buf *, struct dma_buf_attachment *);
    void (*detach)(struct dma_buf *, struct dma_buf_attachment *);
    struct sg_table * (*map_dma_buf)(struct dma_buf_attachment *, enum dma_data_direction);
    void (*unmap_dma_buf)(struct dma_buf_attachment *, struct sg_table *, enum dma_data_direction);
    void (*release)(struct dma_buf *);
    int (*begin_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*end_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*mmap)(struct dma_buf *, struct vm_area_struct *);
    void * (*map)(struct dma_buf *, long unsigned int);
    void (*unmap)(struct dma_buf *, long unsigned int, void *);
    void * (*vmap)(struct dma_buf *);
    void (*vunmap)(struct dma_buf *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dma_buf_ops {
    bool cache_sgt_mapping;
    int (*attach)(struct dma_buf *, struct dma_buf_attachment *);
    void (*detach)(struct dma_buf *, struct dma_buf_attachment *);
    struct sg_table * (*map_dma_buf)(struct dma_buf_attachment *, enum dma_data_direction);
    void (*unmap_dma_buf)(struct dma_buf_attachment *, struct sg_table *, enum dma_data_direction);
    void (*release)(struct dma_buf *);
    int (*begin_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*end_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*mmap)(struct dma_buf *, struct vm_area_struct *);
    void * (*map)(struct dma_buf *, long unsigned int);
    void (*unmap)(struct dma_buf *, long unsigned int, void *);
    void * (*vmap)(struct dma_buf *);
    void (*vunmap)(struct dma_buf *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dma_buf_ops {
    bool cache_sgt_mapping;
    int (*attach)(struct dma_buf *, struct dma_buf_attachment *);
    void (*detach)(struct dma_buf *, struct dma_buf_attachment *);
    struct sg_table * (*map_dma_buf)(struct dma_buf_attachment *, enum dma_data_direction);
    void (*unmap_dma_buf)(struct dma_buf_attachment *, struct sg_table *, enum dma_data_direction);
    void (*release)(struct dma_buf *);
    int (*begin_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*end_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*mmap)(struct dma_buf *, struct vm_area_struct *);
    void * (*map)(struct dma_buf *, long unsigned int);
    void (*unmap)(struct dma_buf *, long unsigned int, void *);
    void * (*vmap)(struct dma_buf *);
    void (*vunmap)(struct dma_buf *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dma_buf_ops {
    bool cache_sgt_mapping;
    int (*attach)(struct dma_buf *, struct dma_buf_attachment *);
    void (*detach)(struct dma_buf *, struct dma_buf_attachment *);
    struct sg_table * (*map_dma_buf)(struct dma_buf_attachment *, enum dma_data_direction);
    void (*unmap_dma_buf)(struct dma_buf_attachment *, struct sg_table *, enum dma_data_direction);
    void (*release)(struct dma_buf *);
    int (*begin_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*end_cpu_access)(struct dma_buf *, enum dma_data_direction);
    int (*mmap)(struct dma_buf *, struct vm_area_struct *);
    void * (*map)(struct dma_buf *, long unsigned int);
    void (*unmap)(struct dma_buf *, long unsigned int, void *);
    void * (*vmap)(struct dma_buf *);
    void (*vunmap)(struct dma_buf *, void *);
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
<code>int (*begin_cpu_access)(struct dma_buf *, size_t, size_t, enum dma_data_direction)</code> ➡️ <code>int (*begin_cpu_access)(struct dma_buf *, enum dma_data_direction)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*end_cpu_access)(struct dma_buf *, size_t, size_t, enum dma_data_direction)</code> ➡️ <code>int (*end_cpu_access)(struct dma_buf *, enum dma_data_direction)</code>
</li>
</ul>
</details>
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
<code>void * (*map_atomic)(struct dma_buf *, long unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*unmap_atomic)(struct dma_buf *, long unsigned int, void *)</code>
</li>
<li>
<b>Field added. </b>
<code>void * (*map)(struct dma_buf *, long unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*unmap)(struct dma_buf *, long unsigned int, void *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void * (*kmap_atomic)(struct dma_buf *, long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*kunmap_atomic)(struct dma_buf *, long unsigned int, void *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void * (*kmap)(struct dma_buf *, long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*kunmap)(struct dma_buf *, long unsigned int, void *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
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
<code>void * (*map_atomic)(struct dma_buf *, long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*unmap_atomic)(struct dma_buf *, long unsigned int, void *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*attach)(struct dma_buf *, struct device *, struct dma_buf_attachment *)</code> ➡️ <code>int (*attach)(struct dma_buf *, struct dma_buf_attachment *)</code>
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
<code>bool cache_sgt_mapping</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*pin)(struct dma_buf_attachment *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*unpin)(struct dma_buf_attachment *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void * (*map)(struct dma_buf *, long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*unmap)(struct dma_buf *, long unsigned int, void *)</code>
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
<code>void * (*vmap)(struct dma_buf *)</code> ➡️ <code>int (*vmap)(struct dma_buf *, struct dma_buf_map *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*vunmap)(struct dma_buf *, void *)</code> ➡️ <code>void (*vunmap)(struct dma_buf *, struct dma_buf_map *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*vmap)(struct dma_buf *, struct dma_buf_map *)</code> ➡️ <code>int (*vmap)(struct dma_buf *, struct iosys_map *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*vunmap)(struct dma_buf *, struct dma_buf_map *)</code> ➡️ <code>void (*vunmap)(struct dma_buf *, struct iosys_map *)</code>
</li>
</ul>
</details>
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
