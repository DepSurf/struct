# Struct: <code>imx_pinctrl_soc_info</code>

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
struct imx_pinctrl_soc_info {
    const struct pinctrl_pin_desc *pins;
    unsigned int npins;
    unsigned int flags;
    const char *gpr_compatible;
    unsigned int mux_mask;
    u8 mux_shift;
    bool generic_pinconf;
    const struct pinconf_generic_params *custom_params;
    unsigned int num_custom_params;
    const struct imx_cfg_params_decode *decodes;
    unsigned int num_decodes;
    void (*fixup)(long unsigned int *, unsigned int, u32 *);
    int (*gpio_set_direction)(struct pinctrl_dev *, struct pinctrl_gpio_range *, unsigned int, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct imx_pinctrl_soc_info {
    const struct pinctrl_pin_desc *pins;
    unsigned int npins;
    unsigned int flags;
    const char *gpr_compatible;
    unsigned int mux_mask;
    u8 mux_shift;
    bool generic_pinconf;
    const struct pinconf_generic_params *custom_params;
    unsigned int num_custom_params;
    const struct imx_cfg_params_decode *decodes;
    unsigned int num_decodes;
    void (*fixup)(long unsigned int *, unsigned int, u32 *);
    int (*gpio_set_direction)(struct pinctrl_dev *, struct pinctrl_gpio_range *, unsigned int, bool);
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
