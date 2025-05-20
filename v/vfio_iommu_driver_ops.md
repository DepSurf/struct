# Struct: <code>vfio_iommu_driver_ops</code>

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
struct vfio_iommu_driver_ops {
    char *name;
    struct module *owner;
    void * (*open)(long unsigned int);
    void (*release)(void *);
    ssize_t (*read)(void *, char *, size_t, loff_t *);
    ssize_t (*write)(void *, const char *, size_t, loff_t *);
    long int (*ioctl)(void *, unsigned int, long unsigned int);
    int (*mmap)(void *, struct vm_area_struct *);
    int (*attach_group)(void *, struct iommu_group *);
    void (*detach_group)(void *, struct iommu_group *);
    int (*pin_pages)(void *, long unsigned int *, int, int, long unsigned int *);
    int (*unpin_pages)(void *, long unsigned int *, int);
    int (*register_notifier)(void *, long unsigned int *, struct notifier_block *);
    int (*unregister_notifier)(void *, struct notifier_block *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct vfio_iommu_driver_ops {
    char *name;
    struct module *owner;
    void * (*open)(long unsigned int);
    void (*release)(void *);
    ssize_t (*read)(void *, char *, size_t, loff_t *);
    ssize_t (*write)(void *, const char *, size_t, loff_t *);
    long int (*ioctl)(void *, unsigned int, long unsigned int);
    int (*mmap)(void *, struct vm_area_struct *);
    int (*attach_group)(void *, struct iommu_group *);
    void (*detach_group)(void *, struct iommu_group *);
    int (*pin_pages)(void *, struct iommu_group *, long unsigned int *, int, int, long unsigned int *);
    int (*unpin_pages)(void *, long unsigned int *, int);
    int (*register_notifier)(void *, long unsigned int *, struct notifier_block *);
    int (*unregister_notifier)(void *, struct notifier_block *);
    int (*dma_rw)(void *, dma_addr_t, void *, size_t, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct vfio_iommu_driver_ops {
    char *name;
    struct module *owner;
    void * (*open)(long unsigned int);
    void (*release)(void *);
    ssize_t (*read)(void *, char *, size_t, loff_t *);
    ssize_t (*write)(void *, const char *, size_t, loff_t *);
    long int (*ioctl)(void *, unsigned int, long unsigned int);
    int (*mmap)(void *, struct vm_area_struct *);
    int (*attach_group)(void *, struct iommu_group *);
    void (*detach_group)(void *, struct iommu_group *);
    int (*pin_pages)(void *, struct iommu_group *, long unsigned int *, int, int, long unsigned int *);
    int (*unpin_pages)(void *, long unsigned int *, int);
    int (*register_notifier)(void *, long unsigned int *, struct notifier_block *);
    int (*unregister_notifier)(void *, struct notifier_block *);
    int (*dma_rw)(void *, dma_addr_t, void *, size_t, bool);
    struct iommu_domain * (*group_iommu_domain)(void *, struct iommu_group *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct vfio_iommu_driver_ops {
    char *name;
    struct module *owner;
    void * (*open)(long unsigned int);
    void (*release)(void *);
    ssize_t (*read)(void *, char *, size_t, loff_t *);
    ssize_t (*write)(void *, const char *, size_t, loff_t *);
    long int (*ioctl)(void *, unsigned int, long unsigned int);
    int (*mmap)(void *, struct vm_area_struct *);
    int (*attach_group)(void *, struct iommu_group *);
    void (*detach_group)(void *, struct iommu_group *);
    int (*pin_pages)(void *, struct iommu_group *, long unsigned int *, int, int, long unsigned int *);
    int (*unpin_pages)(void *, long unsigned int *, int);
    int (*register_notifier)(void *, long unsigned int *, struct notifier_block *);
    int (*unregister_notifier)(void *, struct notifier_block *);
    int (*dma_rw)(void *, dma_addr_t, void *, size_t, bool);
    struct iommu_domain * (*group_iommu_domain)(void *, struct iommu_group *);
    void (*notify)(void *, enum vfio_iommu_notify_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct vfio_iommu_driver_ops {
    char *name;
    struct module *owner;
    void * (*open)(long unsigned int);
    void (*release)(void *);
    ssize_t (*read)(void *, char *, size_t, loff_t *);
    ssize_t (*write)(void *, const char *, size_t, loff_t *);
    long int (*ioctl)(void *, unsigned int, long unsigned int);
    int (*mmap)(void *, struct vm_area_struct *);
    int (*attach_group)(void *, struct iommu_group *);
    void (*detach_group)(void *, struct iommu_group *);
    int (*pin_pages)(void *, struct iommu_group *, long unsigned int *, int, int, long unsigned int *);
    int (*unpin_pages)(void *, long unsigned int *, int);
    int (*register_notifier)(void *, long unsigned int *, struct notifier_block *);
    int (*unregister_notifier)(void *, struct notifier_block *);
    int (*dma_rw)(void *, dma_addr_t, void *, size_t, bool);
    struct iommu_domain * (*group_iommu_domain)(void *, struct iommu_group *);
    void (*notify)(void *, enum vfio_iommu_notify_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct vfio_iommu_driver_ops {
    char *name;
    struct module *owner;
    void * (*open)(long unsigned int);
    void (*release)(void *);
    long int (*ioctl)(void *, unsigned int, long unsigned int);
    int (*attach_group)(void *, struct iommu_group *, enum vfio_group_type);
    void (*detach_group)(void *, struct iommu_group *);
    int (*pin_pages)(void *, struct iommu_group *, long unsigned int *, int, int, long unsigned int *);
    int (*unpin_pages)(void *, long unsigned int *, int);
    int (*register_notifier)(void *, long unsigned int *, struct notifier_block *);
    int (*unregister_notifier)(void *, struct notifier_block *);
    int (*dma_rw)(void *, dma_addr_t, void *, size_t, bool);
    struct iommu_domain * (*group_iommu_domain)(void *, struct iommu_group *);
    void (*notify)(void *, enum vfio_iommu_notify_type);
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
struct vfio_iommu_driver_ops {
    char *name;
    struct module *owner;
    void * (*open)(long unsigned int);
    void (*release)(void *);
    ssize_t (*read)(void *, char *, size_t, loff_t *);
    ssize_t (*write)(void *, const char *, size_t, loff_t *);
    long int (*ioctl)(void *, unsigned int, long unsigned int);
    int (*mmap)(void *, struct vm_area_struct *);
    int (*attach_group)(void *, struct iommu_group *);
    void (*detach_group)(void *, struct iommu_group *);
    int (*pin_pages)(void *, long unsigned int *, int, int, long unsigned int *);
    int (*unpin_pages)(void *, long unsigned int *, int);
    int (*register_notifier)(void *, long unsigned int *, struct notifier_block *);
    int (*unregister_notifier)(void *, struct notifier_block *);
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
struct vfio_iommu_driver_ops {
    char *name;
    struct module *owner;
    void * (*open)(long unsigned int);
    void (*release)(void *);
    ssize_t (*read)(void *, char *, size_t, loff_t *);
    ssize_t (*write)(void *, const char *, size_t, loff_t *);
    long int (*ioctl)(void *, unsigned int, long unsigned int);
    int (*mmap)(void *, struct vm_area_struct *);
    int (*attach_group)(void *, struct iommu_group *);
    void (*detach_group)(void *, struct iommu_group *);
    int (*pin_pages)(void *, long unsigned int *, int, int, long unsigned int *);
    int (*unpin_pages)(void *, long unsigned int *, int);
    int (*register_notifier)(void *, long unsigned int *, struct notifier_block *);
    int (*unregister_notifier)(void *, struct notifier_block *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct vfio_iommu_driver_ops {
    char *name;
    struct module *owner;
    void * (*open)(long unsigned int);
    void (*release)(void *);
    ssize_t (*read)(void *, char *, size_t, loff_t *);
    ssize_t (*write)(void *, const char *, size_t, loff_t *);
    long int (*ioctl)(void *, unsigned int, long unsigned int);
    int (*mmap)(void *, struct vm_area_struct *);
    int (*attach_group)(void *, struct iommu_group *);
    void (*detach_group)(void *, struct iommu_group *);
    int (*pin_pages)(void *, long unsigned int *, int, int, long unsigned int *);
    int (*unpin_pages)(void *, long unsigned int *, int);
    int (*register_notifier)(void *, long unsigned int *, struct notifier_block *);
    int (*unregister_notifier)(void *, struct notifier_block *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct vfio_iommu_driver_ops {
    char *name;
    struct module *owner;
    void * (*open)(long unsigned int);
    void (*release)(void *);
    ssize_t (*read)(void *, char *, size_t, loff_t *);
    ssize_t (*write)(void *, const char *, size_t, loff_t *);
    long int (*ioctl)(void *, unsigned int, long unsigned int);
    int (*mmap)(void *, struct vm_area_struct *);
    int (*attach_group)(void *, struct iommu_group *);
    void (*detach_group)(void *, struct iommu_group *);
    int (*pin_pages)(void *, long unsigned int *, int, int, long unsigned int *);
    int (*unpin_pages)(void *, long unsigned int *, int);
    int (*register_notifier)(void *, long unsigned int *, struct notifier_block *);
    int (*unregister_notifier)(void *, struct notifier_block *);
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
<code>int (*dma_rw)(void *, dma_addr_t, void *, size_t, bool)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*pin_pages)(void *, long unsigned int *, int, int, long unsigned int *)</code> ➡️ <code>int (*pin_pages)(void *, struct iommu_group *, long unsigned int *, int, int, long unsigned int *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct iommu_domain * (*group_iommu_domain)(void *, struct iommu_group *)</code>
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
<code>void (*notify)(void *, enum vfio_iommu_notify_type)</code>
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
<b>Field removed. </b>
<code>ssize_t (*read)(void *, char *, size_t, loff_t *)</code>
</li>
<li>
<b>Field removed. </b>
<code>ssize_t (*write)(void *, const char *, size_t, loff_t *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*mmap)(void *, struct vm_area_struct *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*attach_group)(void *, struct iommu_group *)</code> ➡️ <code>int (*attach_group)(void *, struct iommu_group *, enum vfio_group_type)</code>
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
