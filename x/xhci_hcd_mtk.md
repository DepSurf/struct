# Struct: <code>xhci_hcd_mtk</code>

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
struct xhci_hcd_mtk {
    struct device *dev;
    struct usb_hcd *hcd;
    struct mu3h_sch_bw_info *sch_array;
    struct mu3c_ippc_regs *ippc_regs;
    bool has_ippc;
    int num_u2_ports;
    int num_u3_ports;
    int u3p_dis_msk;
    struct regulator *vusb33;
    struct regulator *vbus;
    struct clk *sys_clk;
    struct clk *xhci_clk;
    struct clk *ref_clk;
    struct clk *mcu_clk;
    struct clk *dma_clk;
    struct regmap *pericfg;
    struct phy **phys;
    int num_phys;
    bool lpm_support;
    bool uwk_en;
    struct regmap *uwk;
    u32 uwk_reg_base;
    u32 uwk_vers;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct xhci_hcd_mtk {
    struct device *dev;
    struct usb_hcd *hcd;
    struct mu3h_sch_bw_info *sch_array;
    struct mu3c_ippc_regs *ippc_regs;
    bool has_ippc;
    int num_u2_ports;
    int num_u3_ports;
    int u3p_dis_msk;
    struct regulator *vusb33;
    struct regulator *vbus;
    struct clk *sys_clk;
    struct clk *xhci_clk;
    struct clk *ref_clk;
    struct clk *mcu_clk;
    struct clk *dma_clk;
    struct regmap *pericfg;
    struct phy **phys;
    int num_phys;
    bool lpm_support;
    bool uwk_en;
    struct regmap *uwk;
    u32 uwk_reg_base;
    u32 uwk_vers;
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
