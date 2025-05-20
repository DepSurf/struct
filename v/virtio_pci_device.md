# Struct: <code>virtio_pci_device</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct virtio_pci_device {
    struct virtio_device vdev;
    struct pci_dev *pci_dev;
    u8 *isr;
    struct virtio_pci_common_cfg *common;
    void *device;
    void *notify_base;
    size_t notify_len;
    size_t device_len;
    int notify_map_cap;
    u32 notify_offset_multiplier;
    int modern_bars;
    void *ioaddr;
    spinlock_t lock;
    struct list_head virtqueues;
    struct virtio_pci_vq_info **vqs;
    int msix_enabled;
    int intx_enabled;
    struct msix_entry *msix_entries;
    cpumask_var_t *msix_affinity_masks;
    char[256] *msix_names;
    unsigned int msix_vectors;
    unsigned int msix_used_vectors;
    bool per_vq_vectors;
    struct virtqueue * (*setup_vq)(struct virtio_pci_device *, struct virtio_pci_vq_info *, unsigned int, void(*)(struct virtqueue *), const char *, u16);
    void (*del_vq)(struct virtio_pci_vq_info *);
    u16 (*config_vector)(struct virtio_pci_device *, u16);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct virtio_pci_device {
    struct virtio_device vdev;
    struct pci_dev *pci_dev;
    u8 *isr;
    struct virtio_pci_common_cfg *common;
    void *device;
    void *notify_base;
    size_t notify_len;
    size_t device_len;
    int notify_map_cap;
    u32 notify_offset_multiplier;
    int modern_bars;
    void *ioaddr;
    spinlock_t lock;
    struct list_head virtqueues;
    struct virtio_pci_vq_info **vqs;
    int msix_enabled;
    int intx_enabled;
    struct msix_entry *msix_entries;
    cpumask_var_t *msix_affinity_masks;
    char[256] *msix_names;
    unsigned int msix_vectors;
    unsigned int msix_used_vectors;
    bool per_vq_vectors;
    struct virtqueue * (*setup_vq)(struct virtio_pci_device *, struct virtio_pci_vq_info *, unsigned int, void(*)(struct virtqueue *), const char *, u16);
    void (*del_vq)(struct virtio_pci_vq_info *);
    u16 (*config_vector)(struct virtio_pci_device *, u16);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct virtio_pci_device {
    struct virtio_device vdev;
    struct pci_dev *pci_dev;
    u8 *isr;
    struct virtio_pci_common_cfg *common;
    void *device;
    void *notify_base;
    size_t notify_len;
    size_t device_len;
    int notify_map_cap;
    u32 notify_offset_multiplier;
    int modern_bars;
    void *ioaddr;
    spinlock_t lock;
    struct list_head virtqueues;
    struct virtio_pci_vq_info **vqs;
    int msix_enabled;
    int intx_enabled;
    cpumask_var_t *msix_affinity_masks;
    char[256] *msix_names;
    unsigned int msix_vectors;
    unsigned int msix_used_vectors;
    bool per_vq_vectors;
    struct virtqueue * (*setup_vq)(struct virtio_pci_device *, struct virtio_pci_vq_info *, unsigned int, void(*)(struct virtqueue *), const char *, u16);
    void (*del_vq)(struct virtio_pci_vq_info *);
    u16 (*config_vector)(struct virtio_pci_device *, u16);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct virtio_pci_device {
    struct virtio_device vdev;
    struct pci_dev *pci_dev;
    u8 *isr;
    struct virtio_pci_common_cfg *common;
    void *device;
    void *notify_base;
    size_t notify_len;
    size_t device_len;
    int notify_map_cap;
    u32 notify_offset_multiplier;
    int modern_bars;
    void *ioaddr;
    spinlock_t lock;
    struct list_head virtqueues;
    struct virtio_pci_vq_info **vqs;
    int msix_enabled;
    int intx_enabled;
    cpumask_var_t *msix_affinity_masks;
    char[256] *msix_names;
    unsigned int msix_vectors;
    unsigned int msix_used_vectors;
    bool per_vq_vectors;
    struct virtqueue * (*setup_vq)(struct virtio_pci_device *, struct virtio_pci_vq_info *, unsigned int, void(*)(struct virtqueue *), const char *, bool, u16);
    void (*del_vq)(struct virtio_pci_vq_info *);
    u16 (*config_vector)(struct virtio_pci_device *, u16);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct virtio_pci_device {
    struct virtio_device vdev;
    struct pci_dev *pci_dev;
    u8 *isr;
    struct virtio_pci_common_cfg *common;
    void *device;
    void *notify_base;
    size_t notify_len;
    size_t device_len;
    int notify_map_cap;
    u32 notify_offset_multiplier;
    int modern_bars;
    void *ioaddr;
    spinlock_t lock;
    struct list_head virtqueues;
    struct virtio_pci_vq_info **vqs;
    int msix_enabled;
    int intx_enabled;
    cpumask_var_t *msix_affinity_masks;
    char[256] *msix_names;
    unsigned int msix_vectors;
    unsigned int msix_used_vectors;
    bool per_vq_vectors;
    struct virtqueue * (*setup_vq)(struct virtio_pci_device *, struct virtio_pci_vq_info *, unsigned int, void(*)(struct virtqueue *), const char *, bool, u16);
    void (*del_vq)(struct virtio_pci_vq_info *);
    u16 (*config_vector)(struct virtio_pci_device *, u16);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct virtio_pci_device {
    struct virtio_device vdev;
    struct pci_dev *pci_dev;
    u8 *isr;
    struct virtio_pci_common_cfg *common;
    void *device;
    void *notify_base;
    size_t notify_len;
    size_t device_len;
    int notify_map_cap;
    u32 notify_offset_multiplier;
    int modern_bars;
    void *ioaddr;
    spinlock_t lock;
    struct list_head virtqueues;
    struct virtio_pci_vq_info **vqs;
    int msix_enabled;
    int intx_enabled;
    cpumask_var_t *msix_affinity_masks;
    char[256] *msix_names;
    unsigned int msix_vectors;
    unsigned int msix_used_vectors;
    bool per_vq_vectors;
    struct virtqueue * (*setup_vq)(struct virtio_pci_device *, struct virtio_pci_vq_info *, unsigned int, void(*)(struct virtqueue *), const char *, bool, u16);
    void (*del_vq)(struct virtio_pci_vq_info *);
    u16 (*config_vector)(struct virtio_pci_device *, u16);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct virtio_pci_device {
    struct virtio_device vdev;
    struct pci_dev *pci_dev;
    u8 *isr;
    struct virtio_pci_common_cfg *common;
    void *device;
    void *notify_base;
    size_t notify_len;
    size_t device_len;
    int notify_map_cap;
    u32 notify_offset_multiplier;
    int modern_bars;
    void *ioaddr;
    spinlock_t lock;
    struct list_head virtqueues;
    struct virtio_pci_vq_info **vqs;
    int msix_enabled;
    int intx_enabled;
    cpumask_var_t *msix_affinity_masks;
    char[256] *msix_names;
    unsigned int msix_vectors;
    unsigned int msix_used_vectors;
    bool per_vq_vectors;
    struct virtqueue * (*setup_vq)(struct virtio_pci_device *, struct virtio_pci_vq_info *, unsigned int, void(*)(struct virtqueue *), const char *, bool, u16);
    void (*del_vq)(struct virtio_pci_vq_info *);
    u16 (*config_vector)(struct virtio_pci_device *, u16);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct virtio_pci_device {
    struct virtio_device vdev;
    struct pci_dev *pci_dev;
    u8 *isr;
    struct virtio_pci_common_cfg *common;
    void *device;
    void *notify_base;
    size_t notify_len;
    size_t device_len;
    int notify_map_cap;
    u32 notify_offset_multiplier;
    int modern_bars;
    void *ioaddr;
    spinlock_t lock;
    struct list_head virtqueues;
    struct virtio_pci_vq_info **vqs;
    int msix_enabled;
    int intx_enabled;
    cpumask_var_t *msix_affinity_masks;
    char[256] *msix_names;
    unsigned int msix_vectors;
    unsigned int msix_used_vectors;
    bool per_vq_vectors;
    struct virtqueue * (*setup_vq)(struct virtio_pci_device *, struct virtio_pci_vq_info *, unsigned int, void(*)(struct virtqueue *), const char *, bool, u16);
    void (*del_vq)(struct virtio_pci_vq_info *);
    u16 (*config_vector)(struct virtio_pci_device *, u16);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct virtio_pci_device {
    struct virtio_device vdev;
    struct pci_dev *pci_dev;
    u8 *isr;
    struct virtio_pci_common_cfg *common;
    void *device;
    void *notify_base;
    size_t notify_len;
    size_t device_len;
    int notify_map_cap;
    u32 notify_offset_multiplier;
    int modern_bars;
    void *ioaddr;
    spinlock_t lock;
    struct list_head virtqueues;
    struct virtio_pci_vq_info **vqs;
    int msix_enabled;
    int intx_enabled;
    cpumask_var_t *msix_affinity_masks;
    char[256] *msix_names;
    unsigned int msix_vectors;
    unsigned int msix_used_vectors;
    bool per_vq_vectors;
    struct virtqueue * (*setup_vq)(struct virtio_pci_device *, struct virtio_pci_vq_info *, unsigned int, void(*)(struct virtqueue *), const char *, bool, u16);
    void (*del_vq)(struct virtio_pci_vq_info *);
    u16 (*config_vector)(struct virtio_pci_device *, u16);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct virtio_pci_device {
    struct virtio_device vdev;
    struct pci_dev *pci_dev;
    u8 *isr;
    struct virtio_pci_common_cfg *common;
    void *device;
    void *notify_base;
    size_t notify_len;
    size_t device_len;
    int notify_map_cap;
    u32 notify_offset_multiplier;
    int modern_bars;
    void *ioaddr;
    spinlock_t lock;
    struct list_head virtqueues;
    struct virtio_pci_vq_info **vqs;
    int msix_enabled;
    int intx_enabled;
    cpumask_var_t *msix_affinity_masks;
    char[256] *msix_names;
    unsigned int msix_vectors;
    unsigned int msix_used_vectors;
    bool per_vq_vectors;
    struct virtqueue * (*setup_vq)(struct virtio_pci_device *, struct virtio_pci_vq_info *, unsigned int, void(*)(struct virtqueue *), const char *, bool, u16);
    void (*del_vq)(struct virtio_pci_vq_info *);
    u16 (*config_vector)(struct virtio_pci_device *, u16);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct virtio_pci_device {
    struct virtio_device vdev;
    struct pci_dev *pci_dev;
    u8 *isr;
    struct virtio_pci_common_cfg *common;
    void *device;
    void *notify_base;
    size_t notify_len;
    size_t device_len;
    int notify_map_cap;
    u32 notify_offset_multiplier;
    int modern_bars;
    void *ioaddr;
    spinlock_t lock;
    struct list_head virtqueues;
    struct virtio_pci_vq_info **vqs;
    int msix_enabled;
    int intx_enabled;
    cpumask_var_t *msix_affinity_masks;
    char[256] *msix_names;
    unsigned int msix_vectors;
    unsigned int msix_used_vectors;
    bool per_vq_vectors;
    struct virtqueue * (*setup_vq)(struct virtio_pci_device *, struct virtio_pci_vq_info *, unsigned int, void(*)(struct virtqueue *), const char *, bool, u16);
    void (*del_vq)(struct virtio_pci_vq_info *);
    u16 (*config_vector)(struct virtio_pci_device *, u16);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct virtio_pci_device {
    struct virtio_device vdev;
    struct pci_dev *pci_dev;
    struct virtio_pci_modern_device mdev;
    u8 *isr;
    void *ioaddr;
    spinlock_t lock;
    struct list_head virtqueues;
    struct virtio_pci_vq_info **vqs;
    int msix_enabled;
    int intx_enabled;
    cpumask_var_t *msix_affinity_masks;
    char[256] *msix_names;
    unsigned int msix_vectors;
    unsigned int msix_used_vectors;
    bool per_vq_vectors;
    struct virtqueue * (*setup_vq)(struct virtio_pci_device *, struct virtio_pci_vq_info *, unsigned int, void(*)(struct virtqueue *), const char *, bool, u16);
    void (*del_vq)(struct virtio_pci_vq_info *);
    u16 (*config_vector)(struct virtio_pci_device *, u16);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct virtio_pci_device {
    struct virtio_device vdev;
    struct pci_dev *pci_dev;
    struct virtio_pci_modern_device mdev;
    u8 *isr;
    void *ioaddr;
    spinlock_t lock;
    struct list_head virtqueues;
    struct virtio_pci_vq_info **vqs;
    int msix_enabled;
    int intx_enabled;
    cpumask_var_t *msix_affinity_masks;
    char[256] *msix_names;
    unsigned int msix_vectors;
    unsigned int msix_used_vectors;
    bool per_vq_vectors;
    struct virtqueue * (*setup_vq)(struct virtio_pci_device *, struct virtio_pci_vq_info *, unsigned int, void(*)(struct virtqueue *), const char *, bool, u16);
    void (*del_vq)(struct virtio_pci_vq_info *);
    u16 (*config_vector)(struct virtio_pci_device *, u16);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct virtio_pci_device {
    struct virtio_device vdev;
    struct pci_dev *pci_dev;
    struct virtio_pci_legacy_device ldev;
    struct virtio_pci_modern_device mdev;
    bool is_legacy;
    u8 *isr;
    spinlock_t lock;
    struct list_head virtqueues;
    struct virtio_pci_vq_info **vqs;
    int msix_enabled;
    int intx_enabled;
    cpumask_var_t *msix_affinity_masks;
    char[256] *msix_names;
    unsigned int msix_vectors;
    unsigned int msix_used_vectors;
    bool per_vq_vectors;
    struct virtqueue * (*setup_vq)(struct virtio_pci_device *, struct virtio_pci_vq_info *, unsigned int, void(*)(struct virtqueue *), const char *, bool, u16);
    void (*del_vq)(struct virtio_pci_vq_info *);
    u16 (*config_vector)(struct virtio_pci_device *, u16);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct virtio_pci_device {
    struct virtio_device vdev;
    struct pci_dev *pci_dev;
    struct virtio_pci_legacy_device ldev;
    struct virtio_pci_modern_device mdev;
    bool is_legacy;
    u8 *isr;
    spinlock_t lock;
    struct list_head virtqueues;
    struct virtio_pci_vq_info **vqs;
    int msix_enabled;
    int intx_enabled;
    cpumask_var_t *msix_affinity_masks;
    char[256] *msix_names;
    unsigned int msix_vectors;
    unsigned int msix_used_vectors;
    bool per_vq_vectors;
    struct virtqueue * (*setup_vq)(struct virtio_pci_device *, struct virtio_pci_vq_info *, unsigned int, void(*)(struct virtqueue *), const char *, bool, u16);
    void (*del_vq)(struct virtio_pci_vq_info *);
    u16 (*config_vector)(struct virtio_pci_device *, u16);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct virtio_pci_device {
    struct virtio_device vdev;
    struct pci_dev *pci_dev;
    struct virtio_pci_legacy_device ldev;
    struct virtio_pci_modern_device mdev;
    bool is_legacy;
    u8 *isr;
    spinlock_t lock;
    struct list_head virtqueues;
    struct virtio_pci_vq_info **vqs;
    int msix_enabled;
    int intx_enabled;
    cpumask_var_t *msix_affinity_masks;
    char[256] *msix_names;
    unsigned int msix_vectors;
    unsigned int msix_used_vectors;
    bool per_vq_vectors;
    struct virtqueue * (*setup_vq)(struct virtio_pci_device *, struct virtio_pci_vq_info *, unsigned int, void(*)(struct virtqueue *), const char *, bool, u16);
    void (*del_vq)(struct virtio_pci_vq_info *);
    u16 (*config_vector)(struct virtio_pci_device *, u16);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct virtio_pci_device {
    struct virtio_device vdev;
    struct pci_dev *pci_dev;
    struct virtio_pci_legacy_device ldev;
    struct virtio_pci_modern_device mdev;
    bool is_legacy;
    u8 *isr;
    spinlock_t lock;
    struct list_head virtqueues;
    struct virtio_pci_vq_info **vqs;
    struct virtio_pci_admin_vq admin_vq;
    int msix_enabled;
    int intx_enabled;
    cpumask_var_t *msix_affinity_masks;
    char[256] *msix_names;
    unsigned int msix_vectors;
    unsigned int msix_used_vectors;
    bool per_vq_vectors;
    struct virtqueue * (*setup_vq)(struct virtio_pci_device *, struct virtio_pci_vq_info *, unsigned int, void(*)(struct virtqueue *), const char *, bool, u16);
    void (*del_vq)(struct virtio_pci_vq_info *);
    u16 (*config_vector)(struct virtio_pci_device *, u16);
    bool (*is_avq)(struct virtio_device *, unsigned int);
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
struct virtio_pci_device {
    struct virtio_device vdev;
    struct pci_dev *pci_dev;
    u8 *isr;
    struct virtio_pci_common_cfg *common;
    void *device;
    void *notify_base;
    size_t notify_len;
    size_t device_len;
    int notify_map_cap;
    u32 notify_offset_multiplier;
    int modern_bars;
    void *ioaddr;
    spinlock_t lock;
    struct list_head virtqueues;
    struct virtio_pci_vq_info **vqs;
    int msix_enabled;
    int intx_enabled;
    cpumask_var_t *msix_affinity_masks;
    char[256] *msix_names;
    unsigned int msix_vectors;
    unsigned int msix_used_vectors;
    bool per_vq_vectors;
    struct virtqueue * (*setup_vq)(struct virtio_pci_device *, struct virtio_pci_vq_info *, unsigned int, void(*)(struct virtqueue *), const char *, bool, u16);
    void (*del_vq)(struct virtio_pci_vq_info *);
    u16 (*config_vector)(struct virtio_pci_device *, u16);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct virtio_pci_device {
    struct virtio_device vdev;
    struct pci_dev *pci_dev;
    u8 *isr;
    struct virtio_pci_common_cfg *common;
    void *device;
    void *notify_base;
    size_t notify_len;
    size_t device_len;
    int notify_map_cap;
    u32 notify_offset_multiplier;
    int modern_bars;
    void *ioaddr;
    spinlock_t lock;
    struct list_head virtqueues;
    struct virtio_pci_vq_info **vqs;
    int msix_enabled;
    int intx_enabled;
    cpumask_var_t *msix_affinity_masks;
    char[256] *msix_names;
    unsigned int msix_vectors;
    unsigned int msix_used_vectors;
    bool per_vq_vectors;
    struct virtqueue * (*setup_vq)(struct virtio_pci_device *, struct virtio_pci_vq_info *, unsigned int, void(*)(struct virtqueue *), const char *, bool, u16);
    void (*del_vq)(struct virtio_pci_vq_info *);
    u16 (*config_vector)(struct virtio_pci_device *, u16);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct virtio_pci_device {
    struct virtio_device vdev;
    struct pci_dev *pci_dev;
    u8 *isr;
    struct virtio_pci_common_cfg *common;
    void *device;
    void *notify_base;
    size_t notify_len;
    size_t device_len;
    int notify_map_cap;
    u32 notify_offset_multiplier;
    int modern_bars;
    void *ioaddr;
    spinlock_t lock;
    struct list_head virtqueues;
    struct virtio_pci_vq_info **vqs;
    int msix_enabled;
    int intx_enabled;
    cpumask_var_t *msix_affinity_masks;
    char[256] *msix_names;
    unsigned int msix_vectors;
    unsigned int msix_used_vectors;
    bool per_vq_vectors;
    struct virtqueue * (*setup_vq)(struct virtio_pci_device *, struct virtio_pci_vq_info *, unsigned int, void(*)(struct virtqueue *), const char *, bool, u16);
    void (*del_vq)(struct virtio_pci_vq_info *);
    u16 (*config_vector)(struct virtio_pci_device *, u16);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct virtio_pci_device {
    struct virtio_device vdev;
    struct pci_dev *pci_dev;
    u8 *isr;
    struct virtio_pci_common_cfg *common;
    void *device;
    void *notify_base;
    size_t notify_len;
    size_t device_len;
    int notify_map_cap;
    u32 notify_offset_multiplier;
    int modern_bars;
    void *ioaddr;
    spinlock_t lock;
    struct list_head virtqueues;
    struct virtio_pci_vq_info **vqs;
    int msix_enabled;
    int intx_enabled;
    cpumask_var_t *msix_affinity_masks;
    char[256] *msix_names;
    unsigned int msix_vectors;
    unsigned int msix_used_vectors;
    bool per_vq_vectors;
    struct virtqueue * (*setup_vq)(struct virtio_pci_device *, struct virtio_pci_vq_info *, unsigned int, void(*)(struct virtqueue *), const char *, bool, u16);
    void (*del_vq)(struct virtio_pci_vq_info *);
    u16 (*config_vector)(struct virtio_pci_device *, u16);
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
struct virtio_pci_device {
    struct virtio_device vdev;
    struct pci_dev *pci_dev;
    u8 *isr;
    struct virtio_pci_common_cfg *common;
    void *device;
    void *notify_base;
    size_t notify_len;
    size_t device_len;
    int notify_map_cap;
    u32 notify_offset_multiplier;
    int modern_bars;
    void *ioaddr;
    spinlock_t lock;
    struct list_head virtqueues;
    struct virtio_pci_vq_info **vqs;
    int msix_enabled;
    int intx_enabled;
    cpumask_var_t *msix_affinity_masks;
    char[256] *msix_names;
    unsigned int msix_vectors;
    unsigned int msix_used_vectors;
    bool per_vq_vectors;
    struct virtqueue * (*setup_vq)(struct virtio_pci_device *, struct virtio_pci_vq_info *, unsigned int, void(*)(struct virtqueue *), const char *, bool, u16);
    void (*del_vq)(struct virtio_pci_vq_info *);
    u16 (*config_vector)(struct virtio_pci_device *, u16);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct virtio_pci_device {
    struct virtio_device vdev;
    struct pci_dev *pci_dev;
    u8 *isr;
    struct virtio_pci_common_cfg *common;
    void *device;
    void *notify_base;
    size_t notify_len;
    size_t device_len;
    int notify_map_cap;
    u32 notify_offset_multiplier;
    int modern_bars;
    void *ioaddr;
    spinlock_t lock;
    struct list_head virtqueues;
    struct virtio_pci_vq_info **vqs;
    int msix_enabled;
    int intx_enabled;
    cpumask_var_t *msix_affinity_masks;
    char[256] *msix_names;
    unsigned int msix_vectors;
    unsigned int msix_used_vectors;
    bool per_vq_vectors;
    struct virtqueue * (*setup_vq)(struct virtio_pci_device *, struct virtio_pci_vq_info *, unsigned int, void(*)(struct virtqueue *), const char *, bool, u16);
    void (*del_vq)(struct virtio_pci_vq_info *);
    u16 (*config_vector)(struct virtio_pci_device *, u16);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct virtio_pci_device {
    struct virtio_device vdev;
    struct pci_dev *pci_dev;
    u8 *isr;
    struct virtio_pci_common_cfg *common;
    void *device;
    void *notify_base;
    size_t notify_len;
    size_t device_len;
    int notify_map_cap;
    u32 notify_offset_multiplier;
    int modern_bars;
    void *ioaddr;
    spinlock_t lock;
    struct list_head virtqueues;
    struct virtio_pci_vq_info **vqs;
    int msix_enabled;
    int intx_enabled;
    cpumask_var_t *msix_affinity_masks;
    char[256] *msix_names;
    unsigned int msix_vectors;
    unsigned int msix_used_vectors;
    bool per_vq_vectors;
    struct virtqueue * (*setup_vq)(struct virtio_pci_device *, struct virtio_pci_vq_info *, unsigned int, void(*)(struct virtqueue *), const char *, bool, u16);
    void (*del_vq)(struct virtio_pci_vq_info *);
    u16 (*config_vector)(struct virtio_pci_device *, u16);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct virtio_pci_device {
    struct virtio_device vdev;
    struct pci_dev *pci_dev;
    u8 *isr;
    struct virtio_pci_common_cfg *common;
    void *device;
    void *notify_base;
    size_t notify_len;
    size_t device_len;
    int notify_map_cap;
    u32 notify_offset_multiplier;
    int modern_bars;
    void *ioaddr;
    spinlock_t lock;
    struct list_head virtqueues;
    struct virtio_pci_vq_info **vqs;
    int msix_enabled;
    int intx_enabled;
    cpumask_var_t *msix_affinity_masks;
    char[256] *msix_names;
    unsigned int msix_vectors;
    unsigned int msix_used_vectors;
    bool per_vq_vectors;
    struct virtqueue * (*setup_vq)(struct virtio_pci_device *, struct virtio_pci_vq_info *, unsigned int, void(*)(struct virtqueue *), const char *, bool, u16);
    void (*del_vq)(struct virtio_pci_vq_info *);
    u16 (*config_vector)(struct virtio_pci_device *, u16);
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
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct msix_entry *msix_entries</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct virtqueue * (*setup_vq)(struct virtio_pci_device *, struct virtio_pci_vq_info *, unsigned int, void(*)(struct virtqueue *), const char *, u16)</code> ➡️ <code>struct virtqueue * (*setup_vq)(struct virtio_pci_device *, struct virtio_pci_vq_info *, unsigned int, void(*)(struct virtqueue *), const char *, bool, u16)</code>
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
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct virtio_pci_modern_device mdev</code>
</li>
<li>
<b>Field removed. </b>
<code>struct virtio_pci_common_cfg *common</code>
</li>
<li>
<b>Field removed. </b>
<code>void *device</code>
</li>
<li>
<b>Field removed. </b>
<code>void *notify_base</code>
</li>
<li>
<b>Field removed. </b>
<code>size_t notify_len</code>
</li>
<li>
<b>Field removed. </b>
<code>size_t device_len</code>
</li>
<li>
<b>Field removed. </b>
<code>int notify_map_cap</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 notify_offset_multiplier</code>
</li>
<li>
<b>Field removed. </b>
<code>int modern_bars</code>
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
<code>struct virtio_pci_legacy_device ldev</code>
</li>
<li>
<b>Field added. </b>
<code>bool is_legacy</code>
</li>
<li>
<b>Field removed. </b>
<code>void *ioaddr</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct virtio_pci_admin_vq admin_vq</code>
</li>
<li>
<b>Field added. </b>
<code>bool (*is_avq)(struct virtio_device *, unsigned int)</code>
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
