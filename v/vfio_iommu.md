# Struct: <code>vfio_iommu</code>

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
struct vfio_iommu {
    struct list_head domain_list;
    struct list_head iova_list;
    struct vfio_domain *external_domain;
    struct mutex lock;
    struct rb_root dma_list;
    struct blocking_notifier_head notifier;
    unsigned int dma_avail;
    bool v2;
    bool nesting;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct vfio_iommu {
    struct list_head domain_list;
    struct list_head iova_list;
    struct vfio_domain *external_domain;
    struct mutex lock;
    struct rb_root dma_list;
    struct blocking_notifier_head notifier;
    unsigned int dma_avail;
    uint64_t pgsize_bitmap;
    bool v2;
    bool nesting;
    bool dirty_page_tracking;
    bool pinned_page_dirty_scope;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct vfio_iommu {
    struct list_head domain_list;
    struct list_head iova_list;
    struct vfio_domain *external_domain;
    struct mutex lock;
    struct rb_root dma_list;
    struct blocking_notifier_head notifier;
    unsigned int dma_avail;
    uint64_t pgsize_bitmap;
    bool v2;
    bool nesting;
    bool dirty_page_tracking;
    bool pinned_page_dirty_scope;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct vfio_iommu {
    struct list_head domain_list;
    struct list_head iova_list;
    struct vfio_domain *external_domain;
    struct mutex lock;
    struct rb_root dma_list;
    struct blocking_notifier_head notifier;
    unsigned int dma_avail;
    unsigned int vaddr_invalid_count;
    uint64_t pgsize_bitmap;
    uint64_t num_non_pinned_groups;
    wait_queue_head_t vaddr_wait;
    bool v2;
    bool nesting;
    bool dirty_page_tracking;
    bool container_open;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct vfio_iommu {
    struct list_head domain_list;
    struct list_head iova_list;
    struct vfio_domain *external_domain;
    struct mutex lock;
    struct rb_root dma_list;
    struct blocking_notifier_head notifier;
    unsigned int dma_avail;
    unsigned int vaddr_invalid_count;
    uint64_t pgsize_bitmap;
    uint64_t num_non_pinned_groups;
    wait_queue_head_t vaddr_wait;
    bool v2;
    bool nesting;
    bool dirty_page_tracking;
    bool container_open;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct vfio_iommu {
    struct list_head domain_list;
    struct list_head iova_list;
    struct mutex lock;
    struct rb_root dma_list;
    struct blocking_notifier_head notifier;
    unsigned int dma_avail;
    unsigned int vaddr_invalid_count;
    uint64_t pgsize_bitmap;
    uint64_t num_non_pinned_groups;
    wait_queue_head_t vaddr_wait;
    bool v2;
    bool nesting;
    bool dirty_page_tracking;
    bool container_open;
    struct list_head emulated_iommu_groups;
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
struct vfio_iommu {
    struct list_head domain_list;
    struct list_head iova_list;
    struct vfio_domain *external_domain;
    struct mutex lock;
    struct rb_root dma_list;
    struct blocking_notifier_head notifier;
    unsigned int dma_avail;
    bool v2;
    bool nesting;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct vfio_iommu {
    struct list_head domain_list;
    struct list_head iova_list;
    struct vfio_domain *external_domain;
    struct mutex lock;
    struct rb_root dma_list;
    struct blocking_notifier_head notifier;
    unsigned int dma_avail;
    bool v2;
    bool nesting;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct vfio_iommu {
    struct list_head domain_list;
    struct list_head iova_list;
    struct vfio_domain *external_domain;
    struct mutex lock;
    struct rb_root dma_list;
    struct blocking_notifier_head notifier;
    unsigned int dma_avail;
    bool v2;
    bool nesting;
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
<code>uint64_t pgsize_bitmap</code>
</li>
<li>
<b>Field added. </b>
<code>bool dirty_page_tracking</code>
</li>
<li>
<b>Field added. </b>
<code>bool pinned_page_dirty_scope</code>
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
<code>unsigned int vaddr_invalid_count</code>
</li>
<li>
<b>Field added. </b>
<code>uint64_t num_non_pinned_groups</code>
</li>
<li>
<b>Field added. </b>
<code>wait_queue_head_t vaddr_wait</code>
</li>
<li>
<b>Field added. </b>
<code>bool container_open</code>
</li>
<li>
<b>Field removed. </b>
<code>bool pinned_page_dirty_scope</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head emulated_iommu_groups</code>
</li>
<li>
<b>Field removed. </b>
<code>struct vfio_domain *external_domain</code>
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
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
