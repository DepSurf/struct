# Struct: <code>vfio</code>

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
struct vfio {
    struct class *class;
    struct list_head iommu_drivers_list;
    struct mutex iommu_drivers_lock;
    struct list_head group_list;
    struct idr group_idr;
    struct mutex group_lock;
    struct cdev group_cdev;
    dev_t group_devt;
    wait_queue_head_t release_q;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct vfio {
    struct class *class;
    struct list_head iommu_drivers_list;
    struct mutex iommu_drivers_lock;
    struct list_head group_list;
    struct idr group_idr;
    struct mutex group_lock;
    struct cdev group_cdev;
    dev_t group_devt;
    wait_queue_head_t release_q;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct vfio {
    struct class *class;
    struct list_head iommu_drivers_list;
    struct mutex iommu_drivers_lock;
    struct list_head group_list;
    struct idr group_idr;
    struct mutex group_lock;
    struct cdev group_cdev;
    dev_t group_devt;
    wait_queue_head_t release_q;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct vfio {
    struct class *class;
    struct list_head iommu_drivers_list;
    struct mutex iommu_drivers_lock;
    struct list_head group_list;
    struct idr group_idr;
    struct mutex group_lock;
    struct cdev group_cdev;
    dev_t group_devt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct vfio {
    struct class *class;
    struct list_head iommu_drivers_list;
    struct mutex iommu_drivers_lock;
    struct list_head group_list;
    struct idr group_idr;
    struct mutex group_lock;
    struct cdev group_cdev;
    dev_t group_devt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct vfio {
    struct class *class;
    struct list_head iommu_drivers_list;
    struct mutex iommu_drivers_lock;
    struct list_head group_list;
    struct mutex group_lock;
    struct ida group_ida;
    dev_t group_devt;
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
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct vfio {
    struct class *class;
    struct list_head iommu_drivers_list;
    struct mutex iommu_drivers_lock;
    struct list_head group_list;
    struct idr group_idr;
    struct mutex group_lock;
    struct cdev group_cdev;
    dev_t group_devt;
    wait_queue_head_t release_q;
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
In <code>aws</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct vfio {
    struct class *class;
    struct list_head iommu_drivers_list;
    struct mutex iommu_drivers_lock;
    struct list_head group_list;
    struct idr group_idr;
    struct mutex group_lock;
    struct cdev group_cdev;
    dev_t group_devt;
    wait_queue_head_t release_q;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct vfio {
    struct class *class;
    struct list_head iommu_drivers_list;
    struct mutex iommu_drivers_lock;
    struct list_head group_list;
    struct idr group_idr;
    struct mutex group_lock;
    struct cdev group_cdev;
    dev_t group_devt;
    wait_queue_head_t release_q;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct vfio {
    struct class *class;
    struct list_head iommu_drivers_list;
    struct mutex iommu_drivers_lock;
    struct list_head group_list;
    struct idr group_idr;
    struct mutex group_lock;
    struct cdev group_cdev;
    dev_t group_devt;
    wait_queue_head_t release_q;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>wait_queue_head_t release_q</code>
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
<code>struct ida group_ida</code>
</li>
<li>
<b>Field removed. </b>
<code>struct idr group_idr</code>
</li>
<li>
<b>Field removed. </b>
<code>struct cdev group_cdev</code>
</li>
</ul>
</details>
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
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
