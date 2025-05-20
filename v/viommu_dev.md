# Struct: <code>viommu_dev</code>

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
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct viommu_dev {
    struct iommu_device iommu;
    struct device *dev;
    struct virtio_device *vdev;
    struct ida domain_ids;
    struct virtqueue * vqs[2];
    spinlock_t request_lock;
    struct list_head requests;
    void *evts;
    struct iommu_domain_geometry geometry;
    u64 pgsize_bitmap;
    u32 first_domain;
    u32 last_domain;
    u32 map_flags;
    u32 probe_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct viommu_dev {
    struct iommu_device iommu;
    struct device *dev;
    struct virtio_device *vdev;
    struct ida domain_ids;
    struct virtqueue * vqs[2];
    spinlock_t request_lock;
    struct list_head requests;
    void *evts;
    struct iommu_domain_geometry geometry;
    u64 pgsize_bitmap;
    u32 first_domain;
    u32 last_domain;
    u32 map_flags;
    u32 probe_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct viommu_dev {
    struct iommu_device iommu;
    struct device *dev;
    struct virtio_device *vdev;
    struct ida domain_ids;
    struct virtqueue * vqs[2];
    spinlock_t request_lock;
    struct list_head requests;
    void *evts;
    struct iommu_domain_geometry geometry;
    u64 pgsize_bitmap;
    u32 first_domain;
    u32 last_domain;
    u32 map_flags;
    u32 probe_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct viommu_dev {
    struct iommu_device iommu;
    struct device *dev;
    struct virtio_device *vdev;
    struct ida domain_ids;
    struct virtqueue * vqs[2];
    spinlock_t request_lock;
    struct list_head requests;
    void *evts;
    struct iommu_domain_geometry geometry;
    u64 pgsize_bitmap;
    u32 first_domain;
    u32 last_domain;
    u32 map_flags;
    u32 probe_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct viommu_dev {
    struct iommu_device iommu;
    struct device *dev;
    struct virtio_device *vdev;
    struct ida domain_ids;
    struct virtqueue * vqs[2];
    spinlock_t request_lock;
    struct list_head requests;
    void *evts;
    struct iommu_domain_geometry geometry;
    u64 pgsize_bitmap;
    u32 first_domain;
    u32 last_domain;
    u32 map_flags;
    u32 probe_size;
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
struct viommu_dev {
    struct iommu_device iommu;
    struct device *dev;
    struct virtio_device *vdev;
    struct ida domain_ids;
    struct virtqueue * vqs[2];
    spinlock_t request_lock;
    struct list_head requests;
    void *evts;
    struct iommu_domain_geometry geometry;
    u64 pgsize_bitmap;
    u32 first_domain;
    u32 last_domain;
    u32 map_flags;
    u32 probe_size;
};
```
</details>
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
</ul>
