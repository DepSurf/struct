# Struct: <code>qcom_pcie_resources_2_4_0</code>

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
struct qcom_pcie_resources_2_4_0 {
    struct clk_bulk_data clks[4];
    int num_clks;
    struct reset_control *axi_m_reset;
    struct reset_control *axi_s_reset;
    struct reset_control *pipe_reset;
    struct reset_control *axi_m_vmid_reset;
    struct reset_control *axi_s_xpu_reset;
    struct reset_control *parf_reset;
    struct reset_control *phy_reset;
    struct reset_control *axi_m_sticky_reset;
    struct reset_control *pipe_sticky_reset;
    struct reset_control *pwr_reset;
    struct reset_control *ahb_reset;
    struct reset_control *phy_ahb_reset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct qcom_pcie_resources_2_4_0 {
    struct clk_bulk_data clks[4];
    int num_clks;
    struct reset_control *axi_m_reset;
    struct reset_control *axi_s_reset;
    struct reset_control *pipe_reset;
    struct reset_control *axi_m_vmid_reset;
    struct reset_control *axi_s_xpu_reset;
    struct reset_control *parf_reset;
    struct reset_control *phy_reset;
    struct reset_control *axi_m_sticky_reset;
    struct reset_control *pipe_sticky_reset;
    struct reset_control *pwr_reset;
    struct reset_control *ahb_reset;
    struct reset_control *phy_ahb_reset;
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
