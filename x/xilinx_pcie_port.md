# Struct: <code>xilinx_pcie_port</code>

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
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct xilinx_pcie_port {
    void *reg_base;
    u32 irq;
    long unsigned int msi_pages;
    u8 root_busno;
    struct device *dev;
    struct irq_domain *msi_domain;
    struct irq_domain *leg_domain;
    struct list_head resources;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct xilinx_pcie_port {
    void *reg_base;
    u32 irq;
    long unsigned int msi_pages;
    u8 root_busno;
    struct device *dev;
    struct irq_domain *msi_domain;
    struct irq_domain *leg_domain;
    struct list_head resources;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct xilinx_pcie_port {
    void *reg_base;
    u32 irq;
    long unsigned int msi_pages;
    u8 root_busno;
    struct device *dev;
    struct irq_domain *msi_domain;
    struct irq_domain *leg_domain;
    struct list_head resources;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct xilinx_pcie_port {
    void *reg_base;
    u32 irq;
    long unsigned int msi_pages;
    u8 root_busno;
    struct device *dev;
    struct irq_domain *msi_domain;
    struct irq_domain *leg_domain;
    struct list_head resources;
};
```
</details>
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
<b>Arch</b>
<ul>
</ul>
