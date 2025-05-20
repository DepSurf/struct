# Struct: <code>pcie_host_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct pcie_host_ops {
    void (*readl_rc)(struct pcie_port *, void *, u32 *);
    void (*writel_rc)(struct pcie_port *, u32, void *);
    int (*rd_own_conf)(struct pcie_port *, int, int, u32 *);
    int (*wr_own_conf)(struct pcie_port *, int, int, u32);
    int (*rd_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32 *);
    int (*wr_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32);
    int (*link_up)(struct pcie_port *);
    void (*host_init)(struct pcie_port *);
    void (*msi_set_irq)(struct pcie_port *, int);
    void (*msi_clear_irq)(struct pcie_port *, int);
    phys_addr_t (*get_msi_addr)(struct pcie_port *);
    u32 (*get_msi_data)(struct pcie_port *, int);
    void (*scan_bus)(struct pcie_port *);
    int (*msi_host_init)(struct pcie_port *, struct msi_controller *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct pcie_host_ops {
    u32 (*readl_rc)(struct pcie_port *, u32);
    void (*writel_rc)(struct pcie_port *, u32, u32);
    int (*rd_own_conf)(struct pcie_port *, int, int, u32 *);
    int (*wr_own_conf)(struct pcie_port *, int, int, u32);
    int (*rd_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32 *);
    int (*wr_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32);
    int (*link_up)(struct pcie_port *);
    void (*host_init)(struct pcie_port *);
    void (*msi_set_irq)(struct pcie_port *, int);
    void (*msi_clear_irq)(struct pcie_port *, int);
    phys_addr_t (*get_msi_addr)(struct pcie_port *);
    u32 (*get_msi_data)(struct pcie_port *, int);
    void (*scan_bus)(struct pcie_port *);
    int (*msi_host_init)(struct pcie_port *, struct msi_controller *);
};
```
</details>
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
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>void (*readl_rc)(struct pcie_port *, void *, u32 *)</code> ➡️ <code>u32 (*readl_rc)(struct pcie_port *, u32)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*writel_rc)(struct pcie_port *, u32, void *)</code> ➡️ <code>void (*writel_rc)(struct pcie_port *, u32, u32)</code>
</li>
</ul>
</details>
</li>
</ul>
