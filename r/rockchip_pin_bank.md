# Struct: <code>rockchip_pin_bank</code>

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
struct rockchip_pin_bank {
    void *reg_base;
    struct regmap *regmap_pull;
    struct clk *clk;
    int irq;
    u32 saved_masks;
    u32 pin_base;
    u8 nr_pins;
    char *name;
    u8 bank_num;
    struct rockchip_iomux iomux[4];
    struct rockchip_drv drv[4];
    enum rockchip_pin_pull_type pull_type[4];
    bool valid;
    struct device_node *of_node;
    struct rockchip_pinctrl *drvdata;
    struct irq_domain *domain;
    struct gpio_chip gpio_chip;
    struct pinctrl_gpio_range grange;
    raw_spinlock_t slock;
    u32 toggle_edge_mode;
    u32 recalced_mask;
    u32 route_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rockchip_pin_bank {
    void *reg_base;
    struct regmap *regmap_pull;
    struct clk *clk;
    int irq;
    u32 saved_masks;
    u32 pin_base;
    u8 nr_pins;
    char *name;
    u8 bank_num;
    struct rockchip_iomux iomux[4];
    struct rockchip_drv drv[4];
    enum rockchip_pin_pull_type pull_type[4];
    bool valid;
    struct device_node *of_node;
    struct rockchip_pinctrl *drvdata;
    struct irq_domain *domain;
    struct gpio_chip gpio_chip;
    struct pinctrl_gpio_range grange;
    raw_spinlock_t slock;
    u32 toggle_edge_mode;
    u32 recalced_mask;
    u32 route_mask;
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
