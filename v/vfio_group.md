# Struct: <code>vfio_group</code>

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
struct vfio_group {
    struct kref kref;
    int minor;
    atomic_t container_users;
    struct iommu_group *iommu_group;
    struct vfio_container *container;
    struct list_head device_list;
    struct mutex device_lock;
    struct device *dev;
    struct notifier_block nb;
    struct list_head vfio_next;
    struct list_head container_next;
    struct list_head unbound_list;
    struct mutex unbound_lock;
    atomic_t opened;
    wait_queue_head_t container_q;
    bool noiommu;
    struct kvm *kvm;
    struct blocking_notifier_head notifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct vfio_group {
    struct kref kref;
    int minor;
    atomic_t container_users;
    struct iommu_group *iommu_group;
    struct vfio_container *container;
    struct list_head device_list;
    struct mutex device_lock;
    struct device *dev;
    struct notifier_block nb;
    struct list_head vfio_next;
    struct list_head container_next;
    struct list_head unbound_list;
    struct mutex unbound_lock;
    atomic_t opened;
    wait_queue_head_t container_q;
    bool noiommu;
    unsigned int dev_counter;
    struct kvm *kvm;
    struct blocking_notifier_head notifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct vfio_group {
    struct kref kref;
    int minor;
    atomic_t container_users;
    struct iommu_group *iommu_group;
    struct vfio_container *container;
    struct list_head device_list;
    struct mutex device_lock;
    struct device *dev;
    struct notifier_block nb;
    struct list_head vfio_next;
    struct list_head container_next;
    struct list_head unbound_list;
    struct mutex unbound_lock;
    atomic_t opened;
    wait_queue_head_t container_q;
    bool noiommu;
    unsigned int dev_counter;
    struct kvm *kvm;
    struct blocking_notifier_head notifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct vfio_group {
    struct kref kref;
    int minor;
    atomic_t container_users;
    struct iommu_group *iommu_group;
    struct vfio_container *container;
    struct list_head device_list;
    struct mutex device_lock;
    struct device *dev;
    struct notifier_block nb;
    struct list_head vfio_next;
    struct list_head container_next;
    struct list_head unbound_list;
    struct mutex unbound_lock;
    atomic_t opened;
    wait_queue_head_t container_q;
    bool noiommu;
    unsigned int dev_counter;
    struct kvm *kvm;
    struct blocking_notifier_head notifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct vfio_group {
    struct kref kref;
    int minor;
    atomic_t container_users;
    struct iommu_group *iommu_group;
    struct vfio_container *container;
    struct list_head device_list;
    struct mutex device_lock;
    struct device *dev;
    struct notifier_block nb;
    struct list_head vfio_next;
    struct list_head container_next;
    struct list_head unbound_list;
    struct mutex unbound_lock;
    atomic_t opened;
    wait_queue_head_t container_q;
    bool noiommu;
    unsigned int dev_counter;
    struct kvm *kvm;
    struct blocking_notifier_head notifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct vfio_group {
    struct device dev;
    struct cdev cdev;
    refcount_t users;
    unsigned int container_users;
    struct iommu_group *iommu_group;
    struct vfio_container *container;
    struct list_head device_list;
    struct mutex device_lock;
    struct list_head vfio_next;
    struct list_head container_next;
    enum vfio_group_type type;
    unsigned int dev_counter;
    struct rw_semaphore group_rwsem;
    struct kvm *kvm;
    struct file *opened_file;
    struct blocking_notifier_head notifier;
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
struct vfio_group {
    struct kref kref;
    int minor;
    atomic_t container_users;
    struct iommu_group *iommu_group;
    struct vfio_container *container;
    struct list_head device_list;
    struct mutex device_lock;
    struct device *dev;
    struct notifier_block nb;
    struct list_head vfio_next;
    struct list_head container_next;
    struct list_head unbound_list;
    struct mutex unbound_lock;
    atomic_t opened;
    wait_queue_head_t container_q;
    bool noiommu;
    struct kvm *kvm;
    struct blocking_notifier_head notifier;
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
struct vfio_group {
    struct kref kref;
    int minor;
    atomic_t container_users;
    struct iommu_group *iommu_group;
    struct vfio_container *container;
    struct list_head device_list;
    struct mutex device_lock;
    struct device *dev;
    struct notifier_block nb;
    struct list_head vfio_next;
    struct list_head container_next;
    struct list_head unbound_list;
    struct mutex unbound_lock;
    atomic_t opened;
    wait_queue_head_t container_q;
    bool noiommu;
    struct kvm *kvm;
    struct blocking_notifier_head notifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct vfio_group {
    struct kref kref;
    int minor;
    atomic_t container_users;
    struct iommu_group *iommu_group;
    struct vfio_container *container;
    struct list_head device_list;
    struct mutex device_lock;
    struct device *dev;
    struct notifier_block nb;
    struct list_head vfio_next;
    struct list_head container_next;
    struct list_head unbound_list;
    struct mutex unbound_lock;
    atomic_t opened;
    wait_queue_head_t container_q;
    bool noiommu;
    struct kvm *kvm;
    struct blocking_notifier_head notifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct vfio_group {
    struct kref kref;
    int minor;
    atomic_t container_users;
    struct iommu_group *iommu_group;
    struct vfio_container *container;
    struct list_head device_list;
    struct mutex device_lock;
    struct device *dev;
    struct notifier_block nb;
    struct list_head vfio_next;
    struct list_head container_next;
    struct list_head unbound_list;
    struct mutex unbound_lock;
    atomic_t opened;
    wait_queue_head_t container_q;
    bool noiommu;
    struct kvm *kvm;
    struct blocking_notifier_head notifier;
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
<code>unsigned int dev_counter</code>
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
<code>struct kvm *kvm</code> ➡️ <code>struct kvm *kvm</code>
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
<b>Field added. </b>
<code>struct cdev cdev</code>
</li>
<li>
<b>Field added. </b>
<code>refcount_t users</code>
</li>
<li>
<b>Field added. </b>
<code>enum vfio_group_type type</code>
</li>
<li>
<b>Field added. </b>
<code>struct rw_semaphore group_rwsem</code>
</li>
<li>
<b>Field added. </b>
<code>struct file *opened_file</code>
</li>
<li>
<b>Field removed. </b>
<code>struct kref kref</code>
</li>
<li>
<b>Field removed. </b>
<code>int minor</code>
</li>
<li>
<b>Field removed. </b>
<code>struct notifier_block nb</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head unbound_list</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mutex unbound_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t opened</code>
</li>
<li>
<b>Field removed. </b>
<code>wait_queue_head_t container_q</code>
</li>
<li>
<b>Field removed. </b>
<code>bool noiommu</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_t container_users</code> ➡️ <code>unsigned int container_users</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct device *dev</code> ➡️ <code>struct device dev</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct kvm *kvm</code> ➡️ <code>struct kvm *kvm</code>
</li>
</ul>
</details>
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
