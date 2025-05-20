# Struct: <code>imx6_pcie</code>

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
struct imx6_pcie {
    struct dw_pcie *pci;
    int reset_gpio;
    bool gpio_active_high;
    struct clk *pcie_bus;
    struct clk *pcie_phy;
    struct clk *pcie_inbound_axi;
    struct clk *pcie;
    struct clk *pcie_aux;
    struct regmap *iomuxc_gpr;
    u32 controller_id;
    struct reset_control *pciephy_reset;
    struct reset_control *apps_reset;
    struct reset_control *turnoff_reset;
    u32 tx_deemph_gen1;
    u32 tx_deemph_gen2_3p5db;
    u32 tx_deemph_gen2_6db;
    u32 tx_swing_full;
    u32 tx_swing_low;
    int link_gen;
    struct regulator *vpcie;
    void *phy_base;
    struct device *pd_pcie;
    struct device *pd_pcie_phy;
    const struct imx6_pcie_drvdata *drvdata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct imx6_pcie {
    struct dw_pcie *pci;
    int reset_gpio;
    bool gpio_active_high;
    struct clk *pcie_bus;
    struct clk *pcie_phy;
    struct clk *pcie_inbound_axi;
    struct clk *pcie;
    struct clk *pcie_aux;
    struct regmap *iomuxc_gpr;
    u32 controller_id;
    struct reset_control *pciephy_reset;
    struct reset_control *apps_reset;
    struct reset_control *turnoff_reset;
    u32 tx_deemph_gen1;
    u32 tx_deemph_gen2_3p5db;
    u32 tx_deemph_gen2_6db;
    u32 tx_swing_full;
    u32 tx_swing_low;
    int link_gen;
    struct regulator *vpcie;
    void *phy_base;
    struct device *pd_pcie;
    struct device *pd_pcie_phy;
    const struct imx6_pcie_drvdata *drvdata;
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
