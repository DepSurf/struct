# Struct: <code>cpg_mssr_info</code>

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
struct cpg_mssr_info {
    const struct cpg_core_clk *early_core_clks;
    unsigned int num_early_core_clks;
    const struct mssr_mod_clk *early_mod_clks;
    unsigned int num_early_mod_clks;
    const struct cpg_core_clk *core_clks;
    unsigned int num_core_clks;
    unsigned int last_dt_core_clk;
    unsigned int num_total_core_clks;
    bool stbyctrl;
    const struct mssr_mod_clk *mod_clks;
    unsigned int num_mod_clks;
    unsigned int num_hw_mod_clks;
    const unsigned int *crit_mod_clks;
    unsigned int num_crit_mod_clks;
    const unsigned int *core_pm_clks;
    unsigned int num_core_pm_clks;
    int (*init)(struct device *);
    struct clk * (*cpg_clk_register)(struct device *, const struct cpg_core_clk *, const struct cpg_mssr_info *, struct clk **, void *, struct raw_notifier_head *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct cpg_mssr_info {
    const struct cpg_core_clk *early_core_clks;
    unsigned int num_early_core_clks;
    const struct mssr_mod_clk *early_mod_clks;
    unsigned int num_early_mod_clks;
    const struct cpg_core_clk *core_clks;
    unsigned int num_core_clks;
    unsigned int last_dt_core_clk;
    unsigned int num_total_core_clks;
    bool stbyctrl;
    const struct mssr_mod_clk *mod_clks;
    unsigned int num_mod_clks;
    unsigned int num_hw_mod_clks;
    const unsigned int *crit_mod_clks;
    unsigned int num_crit_mod_clks;
    const unsigned int *core_pm_clks;
    unsigned int num_core_pm_clks;
    int (*init)(struct device *);
    struct clk * (*cpg_clk_register)(struct device *, const struct cpg_core_clk *, const struct cpg_mssr_info *, struct clk **, void *, struct raw_notifier_head *);
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
