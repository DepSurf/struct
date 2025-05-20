# Struct: <code>sh_pfc_soc_info</code>

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
struct sh_pfc_soc_info {
    const char *name;
    const struct sh_pfc_soc_operations *ops;
    struct pinmux_range input;
    struct pinmux_range output;
    struct pinmux_range function;
    const struct sh_pfc_pin *pins;
    unsigned int nr_pins;
    const struct sh_pfc_pin_group *groups;
    unsigned int nr_groups;
    const struct sh_pfc_function *functions;
    unsigned int nr_functions;
    const struct pinmux_cfg_reg *cfg_regs;
    const struct pinmux_drive_reg *drive_regs;
    const struct pinmux_bias_reg *bias_regs;
    const struct pinmux_ioctrl_reg *ioctrl_regs;
    const struct pinmux_data_reg *data_regs;
    const u16 *pinmux_data;
    unsigned int pinmux_data_size;
    const struct pinmux_irq *gpio_irq;
    unsigned int gpio_irq_size;
    u32 unlock_reg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct sh_pfc_soc_info {
    const char *name;
    const struct sh_pfc_soc_operations *ops;
    struct pinmux_range input;
    struct pinmux_range output;
    struct pinmux_range function;
    const struct sh_pfc_pin *pins;
    unsigned int nr_pins;
    const struct sh_pfc_pin_group *groups;
    unsigned int nr_groups;
    const struct sh_pfc_function *functions;
    unsigned int nr_functions;
    const struct pinmux_cfg_reg *cfg_regs;
    const struct pinmux_drive_reg *drive_regs;
    const struct pinmux_bias_reg *bias_regs;
    const struct pinmux_ioctrl_reg *ioctrl_regs;
    const struct pinmux_data_reg *data_regs;
    const u16 *pinmux_data;
    unsigned int pinmux_data_size;
    const struct pinmux_irq *gpio_irq;
    unsigned int gpio_irq_size;
    u32 unlock_reg;
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
