# Struct: <code>pci_host_bridge</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct pci_host_bridge {
    struct device dev;
    struct pci_bus *bus;
    struct list_head windows;
    void (*release_fn)(struct pci_host_bridge *);
    void *release_data;
    unsigned int ignore_reset_delay;
    resource_size_t (*align_resource)(struct pci_dev *, const struct resource *, resource_size_t, resource_size_t, resource_size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct pci_host_bridge {
    struct device dev;
    struct pci_bus *bus;
    struct list_head windows;
    void (*release_fn)(struct pci_host_bridge *);
    void *release_data;
    unsigned int ignore_reset_delay;
    resource_size_t (*align_resource)(struct pci_dev *, const struct resource *, resource_size_t, resource_size_t, resource_size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct pci_host_bridge {
    struct device dev;
    struct pci_bus *bus;
    struct pci_ops *ops;
    void *sysdata;
    int busnr;
    struct list_head windows;
    void (*release_fn)(struct pci_host_bridge *);
    void *release_data;
    struct msi_controller *msi;
    unsigned int ignore_reset_delay;
    resource_size_t (*align_resource)(struct pci_dev *, const struct resource *, resource_size_t, resource_size_t, resource_size_t);
    long unsigned int private[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct pci_host_bridge {
    struct device dev;
    struct pci_bus *bus;
    struct pci_ops *ops;
    void *sysdata;
    int busnr;
    struct list_head windows;
    u8 (*swizzle_irq)(struct pci_dev *, u8 *);
    int (*map_irq)(const struct pci_dev *, u8, u8);
    void (*release_fn)(struct pci_host_bridge *);
    void *release_data;
    struct msi_controller *msi;
    unsigned int ignore_reset_delay;
    resource_size_t (*align_resource)(struct pci_dev *, const struct resource *, resource_size_t, resource_size_t, resource_size_t);
    long unsigned int private[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct pci_host_bridge {
    struct device dev;
    struct pci_bus *bus;
    struct pci_ops *ops;
    void *sysdata;
    int busnr;
    struct list_head windows;
    u8 (*swizzle_irq)(struct pci_dev *, u8 *);
    int (*map_irq)(const struct pci_dev *, u8, u8);
    void (*release_fn)(struct pci_host_bridge *);
    void *release_data;
    struct msi_controller *msi;
    unsigned int ignore_reset_delay;
    unsigned int no_ext_tags;
    resource_size_t (*align_resource)(struct pci_dev *, const struct resource *, resource_size_t, resource_size_t, resource_size_t);
    long unsigned int private[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct pci_host_bridge {
    struct device dev;
    struct pci_bus *bus;
    struct pci_ops *ops;
    void *sysdata;
    int busnr;
    struct list_head windows;
    u8 (*swizzle_irq)(struct pci_dev *, u8 *);
    int (*map_irq)(const struct pci_dev *, u8, u8);
    void (*release_fn)(struct pci_host_bridge *);
    void *release_data;
    struct msi_controller *msi;
    unsigned int ignore_reset_delay;
    unsigned int no_ext_tags;
    unsigned int native_aer;
    unsigned int native_pcie_hotplug;
    unsigned int native_shpc_hotplug;
    unsigned int native_pme;
    unsigned int native_ltr;
    resource_size_t (*align_resource)(struct pci_dev *, const struct resource *, resource_size_t, resource_size_t, resource_size_t);
    long unsigned int private[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct pci_host_bridge {
    struct device dev;
    struct pci_bus *bus;
    struct pci_ops *ops;
    void *sysdata;
    int busnr;
    struct list_head windows;
    u8 (*swizzle_irq)(struct pci_dev *, u8 *);
    int (*map_irq)(const struct pci_dev *, u8, u8);
    void (*release_fn)(struct pci_host_bridge *);
    void *release_data;
    struct msi_controller *msi;
    unsigned int ignore_reset_delay;
    unsigned int no_ext_tags;
    unsigned int native_aer;
    unsigned int native_pcie_hotplug;
    unsigned int native_shpc_hotplug;
    unsigned int native_pme;
    unsigned int native_ltr;
    resource_size_t (*align_resource)(struct pci_dev *, const struct resource *, resource_size_t, resource_size_t, resource_size_t);
    long unsigned int private[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct pci_host_bridge {
    struct device dev;
    struct pci_bus *bus;
    struct pci_ops *ops;
    void *sysdata;
    int busnr;
    struct list_head windows;
    struct list_head dma_ranges;
    u8 (*swizzle_irq)(struct pci_dev *, u8 *);
    int (*map_irq)(const struct pci_dev *, u8, u8);
    void (*release_fn)(struct pci_host_bridge *);
    void *release_data;
    struct msi_controller *msi;
    unsigned int ignore_reset_delay;
    unsigned int no_ext_tags;
    unsigned int native_aer;
    unsigned int native_pcie_hotplug;
    unsigned int native_shpc_hotplug;
    unsigned int native_pme;
    unsigned int native_ltr;
    unsigned int preserve_config;
    resource_size_t (*align_resource)(struct pci_dev *, const struct resource *, resource_size_t, resource_size_t, resource_size_t);
    long unsigned int private[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct pci_host_bridge {
    struct device dev;
    struct pci_bus *bus;
    struct pci_ops *ops;
    void *sysdata;
    int busnr;
    struct list_head windows;
    struct list_head dma_ranges;
    u8 (*swizzle_irq)(struct pci_dev *, u8 *);
    int (*map_irq)(const struct pci_dev *, u8, u8);
    void (*release_fn)(struct pci_host_bridge *);
    void *release_data;
    struct msi_controller *msi;
    unsigned int ignore_reset_delay;
    unsigned int no_ext_tags;
    unsigned int native_aer;
    unsigned int native_pcie_hotplug;
    unsigned int native_shpc_hotplug;
    unsigned int native_pme;
    unsigned int native_ltr;
    unsigned int preserve_config;
    resource_size_t (*align_resource)(struct pci_dev *, const struct resource *, resource_size_t, resource_size_t, resource_size_t);
    long unsigned int private[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct pci_host_bridge {
    struct device dev;
    struct pci_bus *bus;
    struct pci_ops *ops;
    void *sysdata;
    int busnr;
    struct list_head windows;
    struct list_head dma_ranges;
    u8 (*swizzle_irq)(struct pci_dev *, u8 *);
    int (*map_irq)(const struct pci_dev *, u8, u8);
    void (*release_fn)(struct pci_host_bridge *);
    void *release_data;
    struct msi_controller *msi;
    unsigned int ignore_reset_delay;
    unsigned int no_ext_tags;
    unsigned int native_aer;
    unsigned int native_pcie_hotplug;
    unsigned int native_shpc_hotplug;
    unsigned int native_pme;
    unsigned int native_ltr;
    unsigned int native_dpc;
    unsigned int preserve_config;
    unsigned int size_windows;
    resource_size_t (*align_resource)(struct pci_dev *, const struct resource *, resource_size_t, resource_size_t, resource_size_t);
    long unsigned int private[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct pci_host_bridge {
    struct device dev;
    struct pci_bus *bus;
    struct pci_ops *ops;
    struct pci_ops *child_ops;
    void *sysdata;
    int busnr;
    struct list_head windows;
    struct list_head dma_ranges;
    u8 (*swizzle_irq)(struct pci_dev *, u8 *);
    int (*map_irq)(const struct pci_dev *, u8, u8);
    void (*release_fn)(struct pci_host_bridge *);
    void *release_data;
    struct msi_controller *msi;
    unsigned int ignore_reset_delay;
    unsigned int no_ext_tags;
    unsigned int native_aer;
    unsigned int native_pcie_hotplug;
    unsigned int native_shpc_hotplug;
    unsigned int native_pme;
    unsigned int native_ltr;
    unsigned int native_dpc;
    unsigned int preserve_config;
    unsigned int size_windows;
    resource_size_t (*align_resource)(struct pci_dev *, const struct resource *, resource_size_t, resource_size_t, resource_size_t);
    long unsigned int private[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct pci_host_bridge {
    struct device dev;
    struct pci_bus *bus;
    struct pci_ops *ops;
    struct pci_ops *child_ops;
    void *sysdata;
    int busnr;
    struct list_head windows;
    struct list_head dma_ranges;
    u8 (*swizzle_irq)(struct pci_dev *, u8 *);
    int (*map_irq)(const struct pci_dev *, u8, u8);
    void (*release_fn)(struct pci_host_bridge *);
    void *release_data;
    unsigned int ignore_reset_delay;
    unsigned int no_ext_tags;
    unsigned int native_aer;
    unsigned int native_pcie_hotplug;
    unsigned int native_shpc_hotplug;
    unsigned int native_pme;
    unsigned int native_ltr;
    unsigned int native_dpc;
    unsigned int preserve_config;
    unsigned int size_windows;
    unsigned int msi_domain;
    resource_size_t (*align_resource)(struct pci_dev *, const struct resource *, resource_size_t, resource_size_t, resource_size_t);
    long unsigned int private[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct pci_host_bridge {
    struct device dev;
    struct pci_bus *bus;
    struct pci_ops *ops;
    struct pci_ops *child_ops;
    void *sysdata;
    int busnr;
    int domain_nr;
    struct list_head windows;
    struct list_head dma_ranges;
    u8 (*swizzle_irq)(struct pci_dev *, u8 *);
    int (*map_irq)(const struct pci_dev *, u8, u8);
    void (*release_fn)(struct pci_host_bridge *);
    void *release_data;
    unsigned int ignore_reset_delay;
    unsigned int no_ext_tags;
    unsigned int native_aer;
    unsigned int native_pcie_hotplug;
    unsigned int native_shpc_hotplug;
    unsigned int native_pme;
    unsigned int native_ltr;
    unsigned int native_dpc;
    unsigned int preserve_config;
    unsigned int size_windows;
    unsigned int msi_domain;
    resource_size_t (*align_resource)(struct pci_dev *, const struct resource *, resource_size_t, resource_size_t, resource_size_t);
    long unsigned int private[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct pci_host_bridge {
    struct device dev;
    struct pci_bus *bus;
    struct pci_ops *ops;
    struct pci_ops *child_ops;
    void *sysdata;
    int busnr;
    int domain_nr;
    struct list_head windows;
    struct list_head dma_ranges;
    u8 (*swizzle_irq)(struct pci_dev *, u8 *);
    int (*map_irq)(const struct pci_dev *, u8, u8);
    void (*release_fn)(struct pci_host_bridge *);
    void *release_data;
    unsigned int ignore_reset_delay;
    unsigned int no_ext_tags;
    unsigned int native_aer;
    unsigned int native_pcie_hotplug;
    unsigned int native_shpc_hotplug;
    unsigned int native_pme;
    unsigned int native_ltr;
    unsigned int native_dpc;
    unsigned int preserve_config;
    unsigned int size_windows;
    unsigned int msi_domain;
    resource_size_t (*align_resource)(struct pci_dev *, const struct resource *, resource_size_t, resource_size_t, resource_size_t);
    long unsigned int private[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct pci_host_bridge {
    struct device dev;
    struct pci_bus *bus;
    struct pci_ops *ops;
    struct pci_ops *child_ops;
    void *sysdata;
    int busnr;
    int domain_nr;
    struct list_head windows;
    struct list_head dma_ranges;
    u8 (*swizzle_irq)(struct pci_dev *, u8 *);
    int (*map_irq)(const struct pci_dev *, u8, u8);
    void (*release_fn)(struct pci_host_bridge *);
    void *release_data;
    unsigned int ignore_reset_delay;
    unsigned int no_ext_tags;
    unsigned int no_inc_mrrs;
    unsigned int native_aer;
    unsigned int native_pcie_hotplug;
    unsigned int native_shpc_hotplug;
    unsigned int native_pme;
    unsigned int native_ltr;
    unsigned int native_dpc;
    unsigned int preserve_config;
    unsigned int size_windows;
    unsigned int msi_domain;
    resource_size_t (*align_resource)(struct pci_dev *, const struct resource *, resource_size_t, resource_size_t, resource_size_t);
    long unsigned int private[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct pci_host_bridge {
    struct device dev;
    struct pci_bus *bus;
    struct pci_ops *ops;
    struct pci_ops *child_ops;
    void *sysdata;
    int busnr;
    int domain_nr;
    struct list_head windows;
    struct list_head dma_ranges;
    u8 (*swizzle_irq)(struct pci_dev *, u8 *);
    int (*map_irq)(const struct pci_dev *, u8, u8);
    void (*release_fn)(struct pci_host_bridge *);
    void *release_data;
    unsigned int ignore_reset_delay;
    unsigned int no_ext_tags;
    unsigned int no_inc_mrrs;
    unsigned int native_aer;
    unsigned int native_pcie_hotplug;
    unsigned int native_shpc_hotplug;
    unsigned int native_pme;
    unsigned int native_ltr;
    unsigned int native_dpc;
    unsigned int native_cxl_error;
    unsigned int preserve_config;
    unsigned int size_windows;
    unsigned int msi_domain;
    resource_size_t (*align_resource)(struct pci_dev *, const struct resource *, resource_size_t, resource_size_t, resource_size_t);
    long unsigned int private[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct pci_host_bridge {
    struct device dev;
    struct pci_bus *bus;
    struct pci_ops *ops;
    struct pci_ops *child_ops;
    void *sysdata;
    int busnr;
    int domain_nr;
    struct list_head windows;
    struct list_head dma_ranges;
    u8 (*swizzle_irq)(struct pci_dev *, u8 *);
    int (*map_irq)(const struct pci_dev *, u8, u8);
    void (*release_fn)(struct pci_host_bridge *);
    void *release_data;
    unsigned int ignore_reset_delay;
    unsigned int no_ext_tags;
    unsigned int no_inc_mrrs;
    unsigned int native_aer;
    unsigned int native_pcie_hotplug;
    unsigned int native_shpc_hotplug;
    unsigned int native_pme;
    unsigned int native_ltr;
    unsigned int native_dpc;
    unsigned int native_cxl_error;
    unsigned int preserve_config;
    unsigned int size_windows;
    unsigned int msi_domain;
    resource_size_t (*align_resource)(struct pci_dev *, const struct resource *, resource_size_t, resource_size_t, resource_size_t);
    long unsigned int private[0];
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
struct pci_host_bridge {
    struct device dev;
    struct pci_bus *bus;
    struct pci_ops *ops;
    void *sysdata;
    int busnr;
    struct list_head windows;
    struct list_head dma_ranges;
    u8 (*swizzle_irq)(struct pci_dev *, u8 *);
    int (*map_irq)(const struct pci_dev *, u8, u8);
    void (*release_fn)(struct pci_host_bridge *);
    void *release_data;
    struct msi_controller *msi;
    unsigned int ignore_reset_delay;
    unsigned int no_ext_tags;
    unsigned int native_aer;
    unsigned int native_pcie_hotplug;
    unsigned int native_shpc_hotplug;
    unsigned int native_pme;
    unsigned int native_ltr;
    unsigned int preserve_config;
    resource_size_t (*align_resource)(struct pci_dev *, const struct resource *, resource_size_t, resource_size_t, resource_size_t);
    long unsigned int private[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct pci_host_bridge {
    struct device dev;
    struct pci_bus *bus;
    struct pci_ops *ops;
    void *sysdata;
    int busnr;
    struct list_head windows;
    struct list_head dma_ranges;
    u8 (*swizzle_irq)(struct pci_dev *, u8 *);
    int (*map_irq)(const struct pci_dev *, u8, u8);
    void (*release_fn)(struct pci_host_bridge *);
    void *release_data;
    struct msi_controller *msi;
    unsigned int ignore_reset_delay;
    unsigned int no_ext_tags;
    unsigned int native_aer;
    unsigned int native_pcie_hotplug;
    unsigned int native_shpc_hotplug;
    unsigned int native_pme;
    unsigned int native_ltr;
    unsigned int preserve_config;
    resource_size_t (*align_resource)(struct pci_dev *, const struct resource *, resource_size_t, resource_size_t, resource_size_t);
    long unsigned int private[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct pci_host_bridge {
    struct device dev;
    struct pci_bus *bus;
    struct pci_ops *ops;
    void *sysdata;
    int busnr;
    struct list_head windows;
    struct list_head dma_ranges;
    u8 (*swizzle_irq)(struct pci_dev *, u8 *);
    int (*map_irq)(const struct pci_dev *, u8, u8);
    void (*release_fn)(struct pci_host_bridge *);
    void *release_data;
    struct msi_controller *msi;
    unsigned int ignore_reset_delay;
    unsigned int no_ext_tags;
    unsigned int native_aer;
    unsigned int native_pcie_hotplug;
    unsigned int native_shpc_hotplug;
    unsigned int native_pme;
    unsigned int native_ltr;
    unsigned int preserve_config;
    resource_size_t (*align_resource)(struct pci_dev *, const struct resource *, resource_size_t, resource_size_t, resource_size_t);
    long unsigned int private[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct pci_host_bridge {
    struct device dev;
    struct pci_bus *bus;
    struct pci_ops *ops;
    void *sysdata;
    int busnr;
    struct list_head windows;
    struct list_head dma_ranges;
    u8 (*swizzle_irq)(struct pci_dev *, u8 *);
    int (*map_irq)(const struct pci_dev *, u8, u8);
    void (*release_fn)(struct pci_host_bridge *);
    void *release_data;
    struct msi_controller *msi;
    unsigned int ignore_reset_delay;
    unsigned int no_ext_tags;
    unsigned int native_aer;
    unsigned int native_pcie_hotplug;
    unsigned int native_shpc_hotplug;
    unsigned int native_pme;
    unsigned int native_ltr;
    unsigned int preserve_config;
    resource_size_t (*align_resource)(struct pci_dev *, const struct resource *, resource_size_t, resource_size_t, resource_size_t);
    long unsigned int private[0];
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
struct pci_host_bridge {
    struct device dev;
    struct pci_bus *bus;
    struct pci_ops *ops;
    void *sysdata;
    int busnr;
    struct list_head windows;
    struct list_head dma_ranges;
    u8 (*swizzle_irq)(struct pci_dev *, u8 *);
    int (*map_irq)(const struct pci_dev *, u8, u8);
    void (*release_fn)(struct pci_host_bridge *);
    void *release_data;
    struct msi_controller *msi;
    unsigned int ignore_reset_delay;
    unsigned int no_ext_tags;
    unsigned int native_aer;
    unsigned int native_pcie_hotplug;
    unsigned int native_shpc_hotplug;
    unsigned int native_pme;
    unsigned int native_ltr;
    unsigned int preserve_config;
    resource_size_t (*align_resource)(struct pci_dev *, const struct resource *, resource_size_t, resource_size_t, resource_size_t);
    long unsigned int private[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct pci_host_bridge {
    struct device dev;
    struct pci_bus *bus;
    struct pci_ops *ops;
    void *sysdata;
    int busnr;
    struct list_head windows;
    struct list_head dma_ranges;
    u8 (*swizzle_irq)(struct pci_dev *, u8 *);
    int (*map_irq)(const struct pci_dev *, u8, u8);
    void (*release_fn)(struct pci_host_bridge *);
    void *release_data;
    struct msi_controller *msi;
    unsigned int ignore_reset_delay;
    unsigned int no_ext_tags;
    unsigned int native_aer;
    unsigned int native_pcie_hotplug;
    unsigned int native_shpc_hotplug;
    unsigned int native_pme;
    unsigned int native_ltr;
    unsigned int preserve_config;
    resource_size_t (*align_resource)(struct pci_dev *, const struct resource *, resource_size_t, resource_size_t, resource_size_t);
    long unsigned int private[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct pci_host_bridge {
    struct device dev;
    struct pci_bus *bus;
    struct pci_ops *ops;
    void *sysdata;
    int busnr;
    struct list_head windows;
    struct list_head dma_ranges;
    u8 (*swizzle_irq)(struct pci_dev *, u8 *);
    int (*map_irq)(const struct pci_dev *, u8, u8);
    void (*release_fn)(struct pci_host_bridge *);
    void *release_data;
    struct msi_controller *msi;
    unsigned int ignore_reset_delay;
    unsigned int no_ext_tags;
    unsigned int native_aer;
    unsigned int native_pcie_hotplug;
    unsigned int native_shpc_hotplug;
    unsigned int native_pme;
    unsigned int native_ltr;
    unsigned int preserve_config;
    resource_size_t (*align_resource)(struct pci_dev *, const struct resource *, resource_size_t, resource_size_t, resource_size_t);
    long unsigned int private[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct pci_host_bridge {
    struct device dev;
    struct pci_bus *bus;
    struct pci_ops *ops;
    void *sysdata;
    int busnr;
    struct list_head windows;
    struct list_head dma_ranges;
    u8 (*swizzle_irq)(struct pci_dev *, u8 *);
    int (*map_irq)(const struct pci_dev *, u8, u8);
    void (*release_fn)(struct pci_host_bridge *);
    void *release_data;
    struct msi_controller *msi;
    unsigned int ignore_reset_delay;
    unsigned int no_ext_tags;
    unsigned int native_aer;
    unsigned int native_pcie_hotplug;
    unsigned int native_shpc_hotplug;
    unsigned int native_pme;
    unsigned int native_ltr;
    unsigned int preserve_config;
    resource_size_t (*align_resource)(struct pci_dev *, const struct resource *, resource_size_t, resource_size_t, resource_size_t);
    long unsigned int private[0];
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
<b>Field added. </b>
<code>struct pci_ops *ops</code>
</li>
<li>
<b>Field added. </b>
<code>void *sysdata</code>
</li>
<li>
<b>Field added. </b>
<code>int busnr</code>
</li>
<li>
<b>Field added. </b>
<code>struct msi_controller *msi</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int private[0]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 (*swizzle_irq)(struct pci_dev *, u8 *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*map_irq)(const struct pci_dev *, u8, u8)</code>
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
<code>unsigned int no_ext_tags</code>
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
<code>unsigned int native_aer</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int native_pcie_hotplug</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int native_shpc_hotplug</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int native_pme</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int native_ltr</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head dma_ranges</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int preserve_config</code>
</li>
</ul>
</details>
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
<code>unsigned int native_dpc</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int size_windows</code>
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
<code>struct pci_ops *child_ops</code>
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
<code>unsigned int msi_domain</code>
</li>
<li>
<b>Field removed. </b>
<code>struct msi_controller *msi</code>
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
<code>int domain_nr</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int no_inc_mrrs</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int native_cxl_error</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
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
