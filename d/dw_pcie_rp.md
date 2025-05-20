# Struct: <code>dw_pcie_rp</code>

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
In <code>5.15</code>: Absent ⚠️
</li>
<li>
In <code>5.19</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dw_pcie_rp {
    bool has_msi_ctrl;
    bool cfg0_io_shared;
    u64 cfg0_base;
    void *va_cfg0_base;
    u32 cfg0_size;
    resource_size_t io_base;
    phys_addr_t io_bus_addr;
    u32 io_size;
    int irq;
    const struct dw_pcie_host_ops *ops;
    int msi_irq[8];
    struct irq_domain *irq_domain;
    struct irq_domain *msi_domain;
    dma_addr_t msi_data;
    struct irq_chip *msi_irq_chip;
    u32 num_vectors;
    u32 irq_mask[8];
    struct pci_host_bridge *bridge;
    raw_spinlock_t lock;
    long unsigned int msi_irq_in_use[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dw_pcie_rp {
    bool has_msi_ctrl;
    bool cfg0_io_shared;
    u64 cfg0_base;
    void *va_cfg0_base;
    u32 cfg0_size;
    resource_size_t io_base;
    phys_addr_t io_bus_addr;
    u32 io_size;
    int irq;
    const struct dw_pcie_host_ops *ops;
    int msi_irq[8];
    struct irq_domain *irq_domain;
    struct irq_domain *msi_domain;
    dma_addr_t msi_data;
    struct irq_chip *msi_irq_chip;
    u32 num_vectors;
    u32 irq_mask[8];
    struct pci_host_bridge *bridge;
    raw_spinlock_t lock;
    long unsigned int msi_irq_in_use[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dw_pcie_rp {
    bool has_msi_ctrl;
    bool cfg0_io_shared;
    u64 cfg0_base;
    void *va_cfg0_base;
    u32 cfg0_size;
    resource_size_t io_base;
    phys_addr_t io_bus_addr;
    u32 io_size;
    int irq;
    const struct dw_pcie_host_ops *ops;
    int msi_irq[8];
    struct irq_domain *irq_domain;
    struct irq_domain *msi_domain;
    dma_addr_t msi_data;
    struct irq_chip *msi_irq_chip;
    u32 num_vectors;
    u32 irq_mask[8];
    struct pci_host_bridge *bridge;
    raw_spinlock_t lock;
    long unsigned int msi_irq_in_use[4];
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
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
