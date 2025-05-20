# Struct: <code>tegra_clk_pll_params</code>

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
struct tegra_clk_pll_params {
    long unsigned int input_min;
    long unsigned int input_max;
    long unsigned int cf_min;
    long unsigned int cf_max;
    long unsigned int vco_min;
    long unsigned int vco_max;
    u32 base_reg;
    u32 misc_reg;
    u32 lock_reg;
    u32 lock_mask;
    u32 lock_enable_bit_idx;
    u32 iddq_reg;
    u32 iddq_bit_idx;
    u32 reset_reg;
    u32 reset_bit_idx;
    u32 sdm_din_reg;
    u32 sdm_din_mask;
    u32 sdm_ctrl_reg;
    u32 sdm_ctrl_en_mask;
    u32 ssc_ctrl_reg;
    u32 ssc_ctrl_en_mask;
    u32 aux_reg;
    u32 dyn_ramp_reg;
    u32 ext_misc_reg[6];
    u32 pmc_divnm_reg;
    u32 pmc_divp_reg;
    u32 flags;
    int stepa_shift;
    int stepb_shift;
    int lock_delay;
    int max_p;
    bool defaults_set;
    const struct pdiv_map *pdiv_tohw;
    struct div_nmp *div_nmp;
    struct tegra_clk_pll_freq_table *freq_table;
    long unsigned int fixed_rate;
    u16 mdiv_default;
    u32 (*round_p_to_pdiv)(u32, u32 *);
    void (*set_gain)(struct tegra_clk_pll_freq_table *);
    int (*calc_rate)(struct clk_hw *, struct tegra_clk_pll_freq_table *, long unsigned int, long unsigned int);
    long unsigned int (*adjust_vco)(struct tegra_clk_pll_params *, long unsigned int);
    void (*set_defaults)(struct tegra_clk_pll *);
    int (*dyn_ramp)(struct tegra_clk_pll *, struct tegra_clk_pll_freq_table *);
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
