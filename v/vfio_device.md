# Struct: <code>vfio_device</code>

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
struct vfio_device {
    struct kref kref;
    struct device *dev;
    const struct vfio_device_ops *ops;
    struct vfio_group *group;
    struct list_head group_next;
    void *device_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct vfio_device {
    struct kref kref;
    struct device *dev;
    const struct vfio_device_ops *ops;
    struct vfio_group *group;
    struct list_head group_next;
    void *device_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct vfio_device {
    struct kref kref;
    struct device *dev;
    const struct vfio_device_ops *ops;
    struct vfio_group *group;
    struct list_head group_next;
    void *device_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct vfio_device {
    struct device *dev;
    const struct vfio_device_ops *ops;
    struct vfio_group *group;
    refcount_t refcount;
    struct completion comp;
    struct list_head group_next;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct vfio_device {
    struct device *dev;
    const struct vfio_device_ops *ops;
    struct vfio_group *group;
    struct vfio_device_set *dev_set;
    struct list_head dev_set_list;
    refcount_t refcount;
    unsigned int open_count;
    struct completion comp;
    struct list_head group_next;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct vfio_device {
    struct device *dev;
    const struct vfio_device_ops *ops;
    const struct vfio_migration_ops *mig_ops;
    struct vfio_group *group;
    struct vfio_device_set *dev_set;
    struct list_head dev_set_list;
    unsigned int migration_flags;
    struct kvm *kvm;
    refcount_t refcount;
    unsigned int open_count;
    struct completion comp;
    struct list_head group_next;
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
struct vfio_device {
    struct kref kref;
    struct device *dev;
    const struct vfio_device_ops *ops;
    struct vfio_group *group;
    struct list_head group_next;
    void *device_data;
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
struct vfio_device {
    struct kref kref;
    struct device *dev;
    const struct vfio_device_ops *ops;
    struct vfio_group *group;
    struct list_head group_next;
    void *device_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct vfio_device {
    struct kref kref;
    struct device *dev;
    const struct vfio_device_ops *ops;
    struct vfio_group *group;
    struct list_head group_next;
    void *device_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct vfio_device {
    struct kref kref;
    struct device *dev;
    const struct vfio_device_ops *ops;
    struct vfio_group *group;
    struct list_head group_next;
    void *device_data;
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
<b>Field added. </b>
<code>refcount_t refcount</code>
</li>
<li>
<b>Field added. </b>
<code>struct completion comp</code>
</li>
<li>
<b>Field removed. </b>
<code>struct kref kref</code>
</li>
<li>
<b>Field removed. </b>
<code>void *device_data</code>
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
<code>struct vfio_device_set *dev_set</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head dev_set_list</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int open_count</code>
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
<code>const struct vfio_migration_ops *mig_ops</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int migration_flags</code>
</li>
<li>
<b>Field added. </b>
<code>struct kvm *kvm</code>
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
