# Struct: <code>tegra_dfll</code>

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
struct tegra_dfll {
    struct device *dev;
    struct tegra_dfll_soc_data *soc;
    void *base;
    void *i2c_base;
    void *i2c_controller_base;
    void *lut_base;
    struct regulator *vdd_reg;
    struct clk *soc_clk;
    struct clk *ref_clk;
    struct clk *i2c_clk;
    struct clk *dfll_clk;
    struct reset_control *dvco_rst;
    long unsigned int ref_rate;
    long unsigned int i2c_clk_rate;
    long unsigned int dvco_rate_min;
    enum dfll_ctrl_mode mode;
    enum dfll_tune_range tune_range;
    struct dentry *debugfs_dir;
    struct clk_hw dfll_clk_hw;
    const char *output_clock_name;
    struct dfll_rate_req last_req;
    long unsigned int last_unrounded_rate;
    u32 droop_ctrl;
    u32 sample_rate;
    u32 force_mode;
    u32 cf;
    u32 ci;
    u32 cg;
    bool cg_scale;
    u32 i2c_fs_rate;
    u32 i2c_reg;
    u32 i2c_slave_addr;
    unsigned int lut[33];
    long unsigned int lut_uv[33];
    int lut_size;
    u8 lut_bottom;
    u8 lut_min;
    u8 lut_max;
    u8 lut_safe;
    enum tegra_dfll_pmu_if pmu_if;
    long unsigned int pwm_rate;
    struct pinctrl *pwm_pin;
    struct pinctrl_state *pwm_enable_state;
    struct pinctrl_state *pwm_disable_state;
    u32 reg_init_uV;
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
