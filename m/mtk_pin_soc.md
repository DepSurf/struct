# Struct: <code>mtk_pin_soc</code>

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
struct mtk_pin_soc {
    const struct mtk_pin_reg_calc *reg_cal;
    const struct mtk_pin_desc *pins;
    unsigned int npins;
    const struct group_desc *grps;
    unsigned int ngrps;
    const struct function_desc *funcs;
    unsigned int nfuncs;
    const struct mtk_eint_regs *eint_regs;
    const struct mtk_eint_hw *eint_hw;
    u8 gpio_m;
    bool ies_present;
    const const char * *base_names;
    unsigned int nbase_names;
    int (*bias_disable_set)(struct mtk_pinctrl *, const struct mtk_pin_desc *);
    int (*bias_disable_get)(struct mtk_pinctrl *, const struct mtk_pin_desc *, int *);
    int (*bias_set)(struct mtk_pinctrl *, const struct mtk_pin_desc *, bool);
    int (*bias_get)(struct mtk_pinctrl *, const struct mtk_pin_desc *, bool, int *);
    int (*drive_set)(struct mtk_pinctrl *, const struct mtk_pin_desc *, u32);
    int (*drive_get)(struct mtk_pinctrl *, const struct mtk_pin_desc *, int *);
    int (*adv_pull_set)(struct mtk_pinctrl *, const struct mtk_pin_desc *, bool, u32);
    int (*adv_pull_get)(struct mtk_pinctrl *, const struct mtk_pin_desc *, bool, u32 *);
    int (*adv_drive_set)(struct mtk_pinctrl *, const struct mtk_pin_desc *, u32);
    int (*adv_drive_get)(struct mtk_pinctrl *, const struct mtk_pin_desc *, u32 *);
    void *driver_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mtk_pin_soc {
    const struct mtk_pin_reg_calc *reg_cal;
    const struct mtk_pin_desc *pins;
    unsigned int npins;
    const struct group_desc *grps;
    unsigned int ngrps;
    const struct function_desc *funcs;
    unsigned int nfuncs;
    const struct mtk_eint_regs *eint_regs;
    const struct mtk_eint_hw *eint_hw;
    u8 gpio_m;
    bool ies_present;
    const const char * *base_names;
    unsigned int nbase_names;
    int (*bias_disable_set)(struct mtk_pinctrl *, const struct mtk_pin_desc *);
    int (*bias_disable_get)(struct mtk_pinctrl *, const struct mtk_pin_desc *, int *);
    int (*bias_set)(struct mtk_pinctrl *, const struct mtk_pin_desc *, bool);
    int (*bias_get)(struct mtk_pinctrl *, const struct mtk_pin_desc *, bool, int *);
    int (*drive_set)(struct mtk_pinctrl *, const struct mtk_pin_desc *, u32);
    int (*drive_get)(struct mtk_pinctrl *, const struct mtk_pin_desc *, int *);
    int (*adv_pull_set)(struct mtk_pinctrl *, const struct mtk_pin_desc *, bool, u32);
    int (*adv_pull_get)(struct mtk_pinctrl *, const struct mtk_pin_desc *, bool, u32 *);
    int (*adv_drive_set)(struct mtk_pinctrl *, const struct mtk_pin_desc *, u32);
    int (*adv_drive_get)(struct mtk_pinctrl *, const struct mtk_pin_desc *, u32 *);
    void *driver_data;
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
