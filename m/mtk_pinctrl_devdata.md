# Struct: <code>mtk_pinctrl_devdata</code>

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
struct mtk_pinctrl_devdata {
    const struct mtk_desc_pin *pins;
    unsigned int npins;
    const struct mtk_drv_group_desc *grp_desc;
    unsigned int n_grp_cls;
    const struct mtk_pin_drv_grp *pin_drv_grp;
    unsigned int n_pin_drv_grps;
    int (*spec_pull_set)(struct regmap *, unsigned int, unsigned char, bool, unsigned int);
    int (*spec_ies_smt_set)(struct regmap *, unsigned int, unsigned char, int, enum pin_config_param);
    void (*spec_pinmux_set)(struct regmap *, unsigned int, unsigned int);
    void (*spec_dir_set)(unsigned int *, unsigned int);
    unsigned int dir_offset;
    unsigned int ies_offset;
    unsigned int smt_offset;
    unsigned int pullen_offset;
    unsigned int pullsel_offset;
    unsigned int drv_offset;
    unsigned int dout_offset;
    unsigned int din_offset;
    unsigned int pinmux_offset;
    short unsigned int type1_start;
    short unsigned int type1_end;
    unsigned char port_shf;
    unsigned char port_mask;
    unsigned char port_align;
    struct mtk_eint_hw eint_hw;
    struct mtk_eint_regs *eint_regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mtk_pinctrl_devdata {
    const struct mtk_desc_pin *pins;
    unsigned int npins;
    const struct mtk_drv_group_desc *grp_desc;
    unsigned int n_grp_cls;
    const struct mtk_pin_drv_grp *pin_drv_grp;
    unsigned int n_pin_drv_grps;
    int (*spec_pull_set)(struct regmap *, unsigned int, unsigned char, bool, unsigned int);
    int (*spec_ies_smt_set)(struct regmap *, unsigned int, unsigned char, int, enum pin_config_param);
    void (*spec_pinmux_set)(struct regmap *, unsigned int, unsigned int);
    void (*spec_dir_set)(unsigned int *, unsigned int);
    unsigned int dir_offset;
    unsigned int ies_offset;
    unsigned int smt_offset;
    unsigned int pullen_offset;
    unsigned int pullsel_offset;
    unsigned int drv_offset;
    unsigned int dout_offset;
    unsigned int din_offset;
    unsigned int pinmux_offset;
    short unsigned int type1_start;
    short unsigned int type1_end;
    unsigned char port_shf;
    unsigned char port_mask;
    unsigned char port_align;
    struct mtk_eint_hw eint_hw;
    struct mtk_eint_regs *eint_regs;
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
