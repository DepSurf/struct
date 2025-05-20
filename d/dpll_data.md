# Struct: <code>dpll_data</code>

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
In <code>arm64</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dpll_data {
    struct clk_omap_reg mult_div1_reg;
    u32 mult_mask;
    u32 div1_mask;
    struct clk_hw *clk_bypass;
    struct clk_hw *clk_ref;
    struct clk_omap_reg control_reg;
    u32 enable_mask;
    long unsigned int last_rounded_rate;
    u16 last_rounded_m;
    u8 last_rounded_m4xen;
    u8 last_rounded_lpmode;
    u16 max_multiplier;
    u8 last_rounded_n;
    u8 min_divider;
    u16 max_divider;
    long unsigned int max_rate;
    u8 modes;
    struct clk_omap_reg autoidle_reg;
    struct clk_omap_reg idlest_reg;
    u32 autoidle_mask;
    u32 freqsel_mask;
    u32 idlest_mask;
    u32 dco_mask;
    u32 sddiv_mask;
    u32 dcc_mask;
    long unsigned int dcc_rate;
    u32 lpmode_mask;
    u32 m4xen_mask;
    u8 auto_recal_bit;
    u8 recal_en_bit;
    u8 recal_st_bit;
    u8 flags;
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
