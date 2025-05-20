# Struct: <code>imx_ahci_priv</code>

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
struct imx_ahci_priv {
    struct platform_device *ahci_pdev;
    enum ahci_imx_type type;
    struct clk *sata_clk;
    struct clk *sata_ref_clk;
    struct clk *ahb_clk;
    struct clk *epcs_tx_clk;
    struct clk *epcs_rx_clk;
    struct clk *phy_apbclk;
    struct clk *phy_pclk0;
    struct clk *phy_pclk1;
    void *phy_base;
    int clkreq_gpio;
    struct regmap *gpr;
    bool no_device;
    bool first_time;
    u32 phy_params;
    u32 imped_ratio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct imx_ahci_priv {
    struct platform_device *ahci_pdev;
    enum ahci_imx_type type;
    struct clk *sata_clk;
    struct clk *sata_ref_clk;
    struct clk *ahb_clk;
    struct clk *epcs_tx_clk;
    struct clk *epcs_rx_clk;
    struct clk *phy_apbclk;
    struct clk *phy_pclk0;
    struct clk *phy_pclk1;
    void *phy_base;
    int clkreq_gpio;
    struct regmap *gpr;
    bool no_device;
    bool first_time;
    u32 phy_params;
    u32 imped_ratio;
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
