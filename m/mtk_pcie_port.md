# Struct: <code>mtk_pcie_port</code>

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
struct mtk_pcie_port {
    void *base;
    struct list_head list;
    struct mtk_pcie *pcie;
    struct reset_control *reset;
    struct clk *sys_ck;
    struct clk *ahb_ck;
    struct clk *axi_ck;
    struct clk *aux_ck;
    struct clk *obff_ck;
    struct clk *pipe_ck;
    struct phy *phy;
    u32 slot;
    int irq;
    struct irq_domain *irq_domain;
    struct irq_domain *inner_domain;
    struct irq_domain *msi_domain;
    struct mutex lock;
    long unsigned int msi_irq_in_use[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mtk_pcie_port {
    void *base;
    struct list_head list;
    struct mtk_pcie *pcie;
    struct reset_control *reset;
    struct clk *sys_ck;
    struct clk *ahb_ck;
    struct clk *axi_ck;
    struct clk *aux_ck;
    struct clk *obff_ck;
    struct clk *pipe_ck;
    struct phy *phy;
    u32 slot;
    int irq;
    struct irq_domain *irq_domain;
    struct irq_domain *inner_domain;
    struct irq_domain *msi_domain;
    struct mutex lock;
    long unsigned int msi_irq_in_use[1];
};
```
</details>
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
<b>Arch</b>
<ul>
</ul>
