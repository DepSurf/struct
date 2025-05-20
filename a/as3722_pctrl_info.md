# Struct: <code>as3722_pctrl_info</code>

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
struct as3722_pctrl_info {
    struct device *dev;
    struct pinctrl_dev *pctl;
    struct as3722 *as3722;
    struct gpio_chip gpio_chip;
    int pins_current_opt[8];
    const struct as3722_pin_function *functions;
    unsigned int num_functions;
    const struct as3722_pingroup *pin_groups;
    int num_pin_groups;
    const struct pinctrl_pin_desc *pins;
    unsigned int num_pins;
    struct as3722_gpio_pin_control gpio_control[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct as3722_pctrl_info {
    struct device *dev;
    struct pinctrl_dev *pctl;
    struct as3722 *as3722;
    struct gpio_chip gpio_chip;
    int pins_current_opt[8];
    const struct as3722_pin_function *functions;
    unsigned int num_functions;
    const struct as3722_pingroup *pin_groups;
    int num_pin_groups;
    const struct pinctrl_pin_desc *pins;
    unsigned int num_pins;
    struct as3722_gpio_pin_control gpio_control[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct as3722_pctrl_info {
    struct device *dev;
    struct pinctrl_dev *pctl;
    struct as3722 *as3722;
    struct gpio_chip gpio_chip;
    int pins_current_opt[8];
    const struct as3722_pin_function *functions;
    unsigned int num_functions;
    const struct as3722_pingroup *pin_groups;
    int num_pin_groups;
    const struct pinctrl_pin_desc *pins;
    unsigned int num_pins;
    struct as3722_gpio_pin_control gpio_control[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct as3722_pctrl_info {
    struct device *dev;
    struct pinctrl_dev *pctl;
    struct as3722 *as3722;
    struct gpio_chip gpio_chip;
    int pins_current_opt[8];
    const struct as3722_pin_function *functions;
    unsigned int num_functions;
    const struct as3722_pingroup *pin_groups;
    int num_pin_groups;
    const struct pinctrl_pin_desc *pins;
    unsigned int num_pins;
    struct as3722_gpio_pin_control gpio_control[8];
};
```
</details>
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
