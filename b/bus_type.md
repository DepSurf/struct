# Struct: <code>bus_type</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct bus_type {
    const char *name;
    const char *dev_name;
    struct device *dev_root;
    struct device_attribute *dev_attrs;
    const struct attribute_group **bus_groups;
    const struct attribute_group **dev_groups;
    const struct attribute_group **drv_groups;
    int (*match)(struct device *, struct device_driver *);
    int (*uevent)(struct device *, struct kobj_uevent_env *);
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*online)(struct device *);
    int (*offline)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct dev_pm_ops *pm;
    const struct iommu_ops *iommu_ops;
    struct subsys_private *p;
    struct lock_class_key lock_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct bus_type {
    const char *name;
    const char *dev_name;
    struct device *dev_root;
    struct device_attribute *dev_attrs;
    const struct attribute_group **bus_groups;
    const struct attribute_group **dev_groups;
    const struct attribute_group **drv_groups;
    int (*match)(struct device *, struct device_driver *);
    int (*uevent)(struct device *, struct kobj_uevent_env *);
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*online)(struct device *);
    int (*offline)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct dev_pm_ops *pm;
    const struct iommu_ops *iommu_ops;
    struct subsys_private *p;
    struct lock_class_key lock_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct bus_type {
    const char *name;
    const char *dev_name;
    struct device *dev_root;
    struct device_attribute *dev_attrs;
    const struct attribute_group **bus_groups;
    const struct attribute_group **dev_groups;
    const struct attribute_group **drv_groups;
    int (*match)(struct device *, struct device_driver *);
    int (*uevent)(struct device *, struct kobj_uevent_env *);
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*online)(struct device *);
    int (*offline)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct dev_pm_ops *pm;
    const struct iommu_ops *iommu_ops;
    struct subsys_private *p;
    struct lock_class_key lock_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct bus_type {
    const char *name;
    const char *dev_name;
    struct device *dev_root;
    const struct attribute_group **bus_groups;
    const struct attribute_group **dev_groups;
    const struct attribute_group **drv_groups;
    int (*match)(struct device *, struct device_driver *);
    int (*uevent)(struct device *, struct kobj_uevent_env *);
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*online)(struct device *);
    int (*offline)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    int (*num_vf)(struct device *);
    const struct dev_pm_ops *pm;
    const struct iommu_ops *iommu_ops;
    struct subsys_private *p;
    struct lock_class_key lock_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct bus_type {
    const char *name;
    const char *dev_name;
    struct device *dev_root;
    const struct attribute_group **bus_groups;
    const struct attribute_group **dev_groups;
    const struct attribute_group **drv_groups;
    int (*match)(struct device *, struct device_driver *);
    int (*uevent)(struct device *, struct kobj_uevent_env *);
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*online)(struct device *);
    int (*offline)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    int (*num_vf)(struct device *);
    const struct dev_pm_ops *pm;
    const struct iommu_ops *iommu_ops;
    struct subsys_private *p;
    struct lock_class_key lock_key;
    bool force_dma;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct bus_type {
    const char *name;
    const char *dev_name;
    struct device *dev_root;
    const struct attribute_group **bus_groups;
    const struct attribute_group **dev_groups;
    const struct attribute_group **drv_groups;
    int (*match)(struct device *, struct device_driver *);
    int (*uevent)(struct device *, struct kobj_uevent_env *);
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*online)(struct device *);
    int (*offline)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    int (*num_vf)(struct device *);
    int (*dma_configure)(struct device *);
    const struct dev_pm_ops *pm;
    const struct iommu_ops *iommu_ops;
    struct subsys_private *p;
    struct lock_class_key lock_key;
    bool need_parent_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct bus_type {
    const char *name;
    const char *dev_name;
    struct device *dev_root;
    const struct attribute_group **bus_groups;
    const struct attribute_group **dev_groups;
    const struct attribute_group **drv_groups;
    int (*match)(struct device *, struct device_driver *);
    int (*uevent)(struct device *, struct kobj_uevent_env *);
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*online)(struct device *);
    int (*offline)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    int (*num_vf)(struct device *);
    int (*dma_configure)(struct device *);
    const struct dev_pm_ops *pm;
    const struct iommu_ops *iommu_ops;
    struct subsys_private *p;
    struct lock_class_key lock_key;
    bool need_parent_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct bus_type {
    const char *name;
    const char *dev_name;
    struct device *dev_root;
    const struct attribute_group **bus_groups;
    const struct attribute_group **dev_groups;
    const struct attribute_group **drv_groups;
    int (*match)(struct device *, struct device_driver *);
    int (*uevent)(struct device *, struct kobj_uevent_env *);
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*online)(struct device *);
    int (*offline)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    int (*num_vf)(struct device *);
    int (*dma_configure)(struct device *);
    const struct dev_pm_ops *pm;
    const struct iommu_ops *iommu_ops;
    struct subsys_private *p;
    struct lock_class_key lock_key;
    bool need_parent_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct bus_type {
    const char *name;
    const char *dev_name;
    struct device *dev_root;
    const struct attribute_group **bus_groups;
    const struct attribute_group **dev_groups;
    const struct attribute_group **drv_groups;
    int (*match)(struct device *, struct device_driver *);
    int (*uevent)(struct device *, struct kobj_uevent_env *);
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*online)(struct device *);
    int (*offline)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    int (*num_vf)(struct device *);
    int (*dma_configure)(struct device *);
    const struct dev_pm_ops *pm;
    const struct iommu_ops *iommu_ops;
    struct subsys_private *p;
    struct lock_class_key lock_key;
    bool need_parent_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct bus_type {
    const char *name;
    const char *dev_name;
    struct device *dev_root;
    const struct attribute_group **bus_groups;
    const struct attribute_group **dev_groups;
    const struct attribute_group **drv_groups;
    int (*match)(struct device *, struct device_driver *);
    int (*uevent)(struct device *, struct kobj_uevent_env *);
    int (*probe)(struct device *);
    void (*sync_state)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*online)(struct device *);
    int (*offline)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    int (*num_vf)(struct device *);
    int (*dma_configure)(struct device *);
    const struct dev_pm_ops *pm;
    const struct iommu_ops *iommu_ops;
    struct subsys_private *p;
    struct lock_class_key lock_key;
    bool need_parent_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct bus_type {
    const char *name;
    const char *dev_name;
    struct device *dev_root;
    const struct attribute_group **bus_groups;
    const struct attribute_group **dev_groups;
    const struct attribute_group **drv_groups;
    int (*match)(struct device *, struct device_driver *);
    int (*uevent)(struct device *, struct kobj_uevent_env *);
    int (*probe)(struct device *);
    void (*sync_state)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*online)(struct device *);
    int (*offline)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    int (*num_vf)(struct device *);
    int (*dma_configure)(struct device *);
    const struct dev_pm_ops *pm;
    const struct iommu_ops *iommu_ops;
    struct subsys_private *p;
    struct lock_class_key lock_key;
    bool need_parent_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct bus_type {
    const char *name;
    const char *dev_name;
    struct device *dev_root;
    const struct attribute_group **bus_groups;
    const struct attribute_group **dev_groups;
    const struct attribute_group **drv_groups;
    int (*match)(struct device *, struct device_driver *);
    int (*uevent)(struct device *, struct kobj_uevent_env *);
    int (*probe)(struct device *);
    void (*sync_state)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*online)(struct device *);
    int (*offline)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    int (*num_vf)(struct device *);
    int (*dma_configure)(struct device *);
    const struct dev_pm_ops *pm;
    const struct iommu_ops *iommu_ops;
    struct subsys_private *p;
    struct lock_class_key lock_key;
    bool need_parent_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct bus_type {
    const char *name;
    const char *dev_name;
    struct device *dev_root;
    const struct attribute_group **bus_groups;
    const struct attribute_group **dev_groups;
    const struct attribute_group **drv_groups;
    int (*match)(struct device *, struct device_driver *);
    int (*uevent)(struct device *, struct kobj_uevent_env *);
    int (*probe)(struct device *);
    void (*sync_state)(struct device *);
    void (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*online)(struct device *);
    int (*offline)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    int (*num_vf)(struct device *);
    int (*dma_configure)(struct device *);
    const struct dev_pm_ops *pm;
    const struct iommu_ops *iommu_ops;
    struct subsys_private *p;
    struct lock_class_key lock_key;
    bool need_parent_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct bus_type {
    const char *name;
    const char *dev_name;
    struct device *dev_root;
    const struct attribute_group **bus_groups;
    const struct attribute_group **dev_groups;
    const struct attribute_group **drv_groups;
    int (*match)(struct device *, struct device_driver *);
    int (*uevent)(struct device *, struct kobj_uevent_env *);
    int (*probe)(struct device *);
    void (*sync_state)(struct device *);
    void (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*online)(struct device *);
    int (*offline)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    int (*num_vf)(struct device *);
    int (*dma_configure)(struct device *);
    void (*dma_cleanup)(struct device *);
    const struct dev_pm_ops *pm;
    const struct iommu_ops *iommu_ops;
    struct subsys_private *p;
    struct lock_class_key lock_key;
    bool need_parent_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct bus_type {
    const char *name;
    const char *dev_name;
    struct device *dev_root;
    const struct attribute_group **bus_groups;
    const struct attribute_group **dev_groups;
    const struct attribute_group **drv_groups;
    int (*match)(struct device *, struct device_driver *);
    int (*uevent)(struct device *, struct kobj_uevent_env *);
    int (*probe)(struct device *);
    void (*sync_state)(struct device *);
    void (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*online)(struct device *);
    int (*offline)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    int (*num_vf)(struct device *);
    int (*dma_configure)(struct device *);
    void (*dma_cleanup)(struct device *);
    const struct dev_pm_ops *pm;
    const struct iommu_ops *iommu_ops;
    struct subsys_private *p;
    struct lock_class_key lock_key;
    bool need_parent_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct bus_type {
    const char *name;
    const char *dev_name;
    const struct attribute_group **bus_groups;
    const struct attribute_group **dev_groups;
    const struct attribute_group **drv_groups;
    int (*match)(struct device *, struct device_driver *);
    int (*uevent)(const struct device *, struct kobj_uevent_env *);
    int (*probe)(struct device *);
    void (*sync_state)(struct device *);
    void (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*online)(struct device *);
    int (*offline)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    int (*num_vf)(struct device *);
    int (*dma_configure)(struct device *);
    void (*dma_cleanup)(struct device *);
    const struct dev_pm_ops *pm;
    const struct iommu_ops *iommu_ops;
    bool need_parent_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct bus_type {
    const char *name;
    const char *dev_name;
    const struct attribute_group **bus_groups;
    const struct attribute_group **dev_groups;
    const struct attribute_group **drv_groups;
    int (*match)(struct device *, struct device_driver *);
    int (*uevent)(const struct device *, struct kobj_uevent_env *);
    int (*probe)(struct device *);
    void (*sync_state)(struct device *);
    void (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*online)(struct device *);
    int (*offline)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    int (*num_vf)(struct device *);
    int (*dma_configure)(struct device *);
    void (*dma_cleanup)(struct device *);
    const struct dev_pm_ops *pm;
    bool need_parent_lock;
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
struct bus_type {
    const char *name;
    const char *dev_name;
    struct device *dev_root;
    const struct attribute_group **bus_groups;
    const struct attribute_group **dev_groups;
    const struct attribute_group **drv_groups;
    int (*match)(struct device *, struct device_driver *);
    int (*uevent)(struct device *, struct kobj_uevent_env *);
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*online)(struct device *);
    int (*offline)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    int (*num_vf)(struct device *);
    int (*dma_configure)(struct device *);
    const struct dev_pm_ops *pm;
    const struct iommu_ops *iommu_ops;
    struct subsys_private *p;
    struct lock_class_key lock_key;
    bool need_parent_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct bus_type {
    const char *name;
    const char *dev_name;
    struct device *dev_root;
    const struct attribute_group **bus_groups;
    const struct attribute_group **dev_groups;
    const struct attribute_group **drv_groups;
    int (*match)(struct device *, struct device_driver *);
    int (*uevent)(struct device *, struct kobj_uevent_env *);
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*online)(struct device *);
    int (*offline)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    int (*num_vf)(struct device *);
    int (*dma_configure)(struct device *);
    const struct dev_pm_ops *pm;
    const struct iommu_ops *iommu_ops;
    struct subsys_private *p;
    struct lock_class_key lock_key;
    bool need_parent_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct bus_type {
    const char *name;
    const char *dev_name;
    struct device *dev_root;
    const struct attribute_group **bus_groups;
    const struct attribute_group **dev_groups;
    const struct attribute_group **drv_groups;
    int (*match)(struct device *, struct device_driver *);
    int (*uevent)(struct device *, struct kobj_uevent_env *);
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*online)(struct device *);
    int (*offline)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    int (*num_vf)(struct device *);
    int (*dma_configure)(struct device *);
    const struct dev_pm_ops *pm;
    const struct iommu_ops *iommu_ops;
    struct subsys_private *p;
    struct lock_class_key lock_key;
    bool need_parent_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct bus_type {
    const char *name;
    const char *dev_name;
    struct device *dev_root;
    const struct attribute_group **bus_groups;
    const struct attribute_group **dev_groups;
    const struct attribute_group **drv_groups;
    int (*match)(struct device *, struct device_driver *);
    int (*uevent)(struct device *, struct kobj_uevent_env *);
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*online)(struct device *);
    int (*offline)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    int (*num_vf)(struct device *);
    int (*dma_configure)(struct device *);
    const struct dev_pm_ops *pm;
    const struct iommu_ops *iommu_ops;
    struct subsys_private *p;
    struct lock_class_key lock_key;
    bool need_parent_lock;
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
struct bus_type {
    const char *name;
    const char *dev_name;
    struct device *dev_root;
    const struct attribute_group **bus_groups;
    const struct attribute_group **dev_groups;
    const struct attribute_group **drv_groups;
    int (*match)(struct device *, struct device_driver *);
    int (*uevent)(struct device *, struct kobj_uevent_env *);
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*online)(struct device *);
    int (*offline)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    int (*num_vf)(struct device *);
    int (*dma_configure)(struct device *);
    const struct dev_pm_ops *pm;
    const struct iommu_ops *iommu_ops;
    struct subsys_private *p;
    struct lock_class_key lock_key;
    bool need_parent_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct bus_type {
    const char *name;
    const char *dev_name;
    struct device *dev_root;
    const struct attribute_group **bus_groups;
    const struct attribute_group **dev_groups;
    const struct attribute_group **drv_groups;
    int (*match)(struct device *, struct device_driver *);
    int (*uevent)(struct device *, struct kobj_uevent_env *);
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*online)(struct device *);
    int (*offline)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    int (*num_vf)(struct device *);
    int (*dma_configure)(struct device *);
    const struct dev_pm_ops *pm;
    const struct iommu_ops *iommu_ops;
    struct subsys_private *p;
    struct lock_class_key lock_key;
    bool need_parent_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct bus_type {
    const char *name;
    const char *dev_name;
    struct device *dev_root;
    const struct attribute_group **bus_groups;
    const struct attribute_group **dev_groups;
    const struct attribute_group **drv_groups;
    int (*match)(struct device *, struct device_driver *);
    int (*uevent)(struct device *, struct kobj_uevent_env *);
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*online)(struct device *);
    int (*offline)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    int (*num_vf)(struct device *);
    int (*dma_configure)(struct device *);
    const struct dev_pm_ops *pm;
    const struct iommu_ops *iommu_ops;
    struct subsys_private *p;
    struct lock_class_key lock_key;
    bool need_parent_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct bus_type {
    const char *name;
    const char *dev_name;
    struct device *dev_root;
    const struct attribute_group **bus_groups;
    const struct attribute_group **dev_groups;
    const struct attribute_group **drv_groups;
    int (*match)(struct device *, struct device_driver *);
    int (*uevent)(struct device *, struct kobj_uevent_env *);
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*online)(struct device *);
    int (*offline)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    int (*num_vf)(struct device *);
    int (*dma_configure)(struct device *);
    const struct dev_pm_ops *pm;
    const struct iommu_ops *iommu_ops;
    struct subsys_private *p;
    struct lock_class_key lock_key;
    bool need_parent_lock;
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
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*num_vf)(struct device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct device_attribute *dev_attrs</code>
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
<code>bool force_dma</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*dma_configure)(struct device *)</code>
</li>
<li>
<b>Field added. </b>
<code>bool need_parent_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>bool force_dma</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*sync_state)(struct device *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*remove)(struct device *)</code> ➡️ <code>void (*remove)(struct device *)</code>
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
<code>void (*dma_cleanup)(struct device *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct device *dev_root</code>
</li>
<li>
<b>Field removed. </b>
<code>struct subsys_private *p</code>
</li>
<li>
<b>Field removed. </b>
<code>struct lock_class_key lock_key</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*uevent)(struct device *, struct kobj_uevent_env *)</code> ➡️ <code>int (*uevent)(const struct device *, struct kobj_uevent_env *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>const struct iommu_ops *iommu_ops</code>
</li>
</ul>
</details>
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
