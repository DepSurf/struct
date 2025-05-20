# Struct: <code>vfio_dma</code>

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
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct vfio_dma {
    struct rb_node node;
    dma_addr_t iova;
    long unsigned int vaddr;
    size_t size;
    int prot;
    bool iommu_mapped;
    bool lock_cap;
    struct task_struct *task;
    struct rb_root pfn_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct vfio_dma {
    struct rb_node node;
    dma_addr_t iova;
    long unsigned int vaddr;
    size_t size;
    int prot;
    bool iommu_mapped;
    bool lock_cap;
    struct task_struct *task;
    struct rb_root pfn_list;
    long unsigned int *bitmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct vfio_dma {
    struct rb_node node;
    dma_addr_t iova;
    long unsigned int vaddr;
    size_t size;
    int prot;
    bool iommu_mapped;
    bool lock_cap;
    struct task_struct *task;
    struct rb_root pfn_list;
    long unsigned int *bitmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct vfio_dma {
    struct rb_node node;
    dma_addr_t iova;
    long unsigned int vaddr;
    size_t size;
    int prot;
    bool iommu_mapped;
    bool lock_cap;
    bool vaddr_invalid;
    struct task_struct *task;
    struct rb_root pfn_list;
    long unsigned int *bitmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct vfio_dma {
    struct rb_node node;
    dma_addr_t iova;
    long unsigned int vaddr;
    size_t size;
    int prot;
    bool iommu_mapped;
    bool lock_cap;
    bool vaddr_invalid;
    struct task_struct *task;
    struct rb_root pfn_list;
    long unsigned int *bitmap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct vfio_dma {
    struct rb_node node;
    dma_addr_t iova;
    long unsigned int vaddr;
    size_t size;
    int prot;
    bool iommu_mapped;
    bool lock_cap;
    bool vaddr_invalid;
    struct task_struct *task;
    struct rb_root pfn_list;
    long unsigned int *bitmap;
};
```
</details>
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
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct vfio_dma {
    struct rb_node node;
    dma_addr_t iova;
    long unsigned int vaddr;
    size_t size;
    int prot;
    bool iommu_mapped;
    bool lock_cap;
    struct task_struct *task;
    struct rb_root pfn_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct vfio_dma {
    struct rb_node node;
    dma_addr_t iova;
    long unsigned int vaddr;
    size_t size;
    int prot;
    bool iommu_mapped;
    bool lock_cap;
    struct task_struct *task;
    struct rb_root pfn_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct vfio_dma {
    struct rb_node node;
    dma_addr_t iova;
    long unsigned int vaddr;
    size_t size;
    int prot;
    bool iommu_mapped;
    bool lock_cap;
    struct task_struct *task;
    struct rb_root pfn_list;
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
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int *bitmap</code>
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
<code>bool vaddr_invalid</code>
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
</ul>
<b>Arch</b>
<ul>
</ul>
<b>Flavor</b>
<ul>
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
