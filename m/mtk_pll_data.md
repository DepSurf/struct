# Struct: <code>mtk_pll_data</code>

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
struct mtk_pll_data {
    int id;
    const char *name;
    uint32_t reg;
    uint32_t pwr_reg;
    uint32_t en_mask;
    uint32_t pd_reg;
    uint32_t tuner_reg;
    uint32_t tuner_en_reg;
    uint8_t tuner_en_bit;
    int pd_shift;
    unsigned int flags;
    const struct clk_ops *ops;
    u32 rst_bar_mask;
    long unsigned int fmin;
    long unsigned int fmax;
    int pcwbits;
    int pcwibits;
    uint32_t pcw_reg;
    int pcw_shift;
    uint32_t pcw_chg_reg;
    const struct mtk_pll_div_table *div_table;
    const char *parent_name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mtk_pll_data {
    int id;
    const char *name;
    uint32_t reg;
    uint32_t pwr_reg;
    uint32_t en_mask;
    uint32_t pd_reg;
    uint32_t tuner_reg;
    uint32_t tuner_en_reg;
    uint8_t tuner_en_bit;
    int pd_shift;
    unsigned int flags;
    const struct clk_ops *ops;
    u32 rst_bar_mask;
    long unsigned int fmin;
    long unsigned int fmax;
    int pcwbits;
    int pcwibits;
    uint32_t pcw_reg;
    int pcw_shift;
    uint32_t pcw_chg_reg;
    const struct mtk_pll_div_table *div_table;
    const char *parent_name;
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
