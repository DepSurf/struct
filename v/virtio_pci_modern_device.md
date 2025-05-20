# Struct: <code>virtio_pci_modern_device</code>

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
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct virtio_pci_modern_device {
    struct pci_dev *pci_dev;
    struct virtio_pci_common_cfg *common;
    void *device;
    void *notify_base;
    resource_size_t notify_pa;
    u8 *isr;
    size_t notify_len;
    size_t device_len;
    int notify_map_cap;
    u32 notify_offset_multiplier;
    int modern_bars;
    struct virtio_device_id id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct virtio_pci_modern_device {
    struct pci_dev *pci_dev;
    struct virtio_pci_common_cfg *common;
    void *device;
    void *notify_base;
    resource_size_t notify_pa;
    u8 *isr;
    size_t notify_len;
    size_t device_len;
    int notify_map_cap;
    u32 notify_offset_multiplier;
    int modern_bars;
    struct virtio_device_id id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct virtio_pci_modern_device {
    struct pci_dev *pci_dev;
    struct virtio_pci_common_cfg *common;
    void *device;
    void *notify_base;
    resource_size_t notify_pa;
    u8 *isr;
    size_t notify_len;
    size_t device_len;
    int notify_map_cap;
    u32 notify_offset_multiplier;
    int modern_bars;
    struct virtio_device_id id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct virtio_pci_modern_device {
    struct pci_dev *pci_dev;
    struct virtio_pci_common_cfg *common;
    void *device;
    void *notify_base;
    resource_size_t notify_pa;
    u8 *isr;
    size_t notify_len;
    size_t device_len;
    int notify_map_cap;
    u32 notify_offset_multiplier;
    int modern_bars;
    struct virtio_device_id id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct virtio_pci_modern_device {
    struct pci_dev *pci_dev;
    struct virtio_pci_common_cfg *common;
    void *device;
    void *notify_base;
    resource_size_t notify_pa;
    u8 *isr;
    size_t notify_len;
    size_t device_len;
    int notify_map_cap;
    u32 notify_offset_multiplier;
    int modern_bars;
    struct virtio_device_id id;
    int (*device_id_check)(struct pci_dev *);
    u64 dma_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct virtio_pci_modern_device {
    struct pci_dev *pci_dev;
    struct virtio_pci_common_cfg *common;
    void *device;
    void *notify_base;
    resource_size_t notify_pa;
    u8 *isr;
    size_t notify_len;
    size_t device_len;
    size_t common_len;
    int notify_map_cap;
    u32 notify_offset_multiplier;
    int modern_bars;
    struct virtio_device_id id;
    int (*device_id_check)(struct pci_dev *);
    u64 dma_mask;
};
```
</details>
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
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*device_id_check)(struct pci_dev *)</code>
</li>
<li>
<b>Field added. </b>
<code>u64 dma_mask</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>size_t common_len</code>
</li>
</ul>
</details>
</li>
</ul>
