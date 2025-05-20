# Struct: <code>chv_pinctrl</code>

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
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct chv_pinctrl {
    struct device *dev;
    struct pinctrl_desc pctldesc;
    struct pinctrl_dev *pctldev;
    struct gpio_chip chip;
    void *regs;
    unsigned int intr_lines[16];
    const struct chv_community *community;
    u32 saved_intmask;
    struct chv_pin_context *saved_pin_context;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct chv_pinctrl {
    struct device *dev;
    struct pinctrl_desc pctldesc;
    struct pinctrl_dev *pctldev;
    struct gpio_chip chip;
    void *regs;
    unsigned int intr_lines[16];
    const struct chv_community *community;
    u32 saved_intmask;
    struct chv_pin_context *saved_pin_context;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct chv_pinctrl {
    struct device *dev;
    struct pinctrl_desc pctldesc;
    struct pinctrl_dev *pctldev;
    struct gpio_chip chip;
    void *regs;
    unsigned int intr_lines[16];
    const struct chv_community *community;
    u32 saved_intmask;
    struct chv_pin_context *saved_pin_context;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct chv_pinctrl {
    struct device *dev;
    struct pinctrl_desc pctldesc;
    struct pinctrl_dev *pctldev;
    struct gpio_chip chip;
    void *regs;
    unsigned int intr_lines[16];
    const struct chv_community *community;
    u32 saved_intmask;
    struct chv_pin_context *saved_pin_context;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct chv_pinctrl {
    struct device *dev;
    struct pinctrl_desc pctldesc;
    struct pinctrl_dev *pctldev;
    struct gpio_chip chip;
    void *regs;
    unsigned int intr_lines[16];
    const struct chv_community *community;
    u32 saved_intmask;
    struct chv_pin_context *saved_pin_context;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct chv_pinctrl {
    struct device *dev;
    struct pinctrl_desc pctldesc;
    struct pinctrl_dev *pctldev;
    struct gpio_chip chip;
    void *regs;
    unsigned int intr_lines[16];
    const struct chv_community *community;
    u32 saved_intmask;
    struct chv_pin_context *saved_pin_context;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct chv_pinctrl {
    struct device *dev;
    struct pinctrl_desc pctldesc;
    struct pinctrl_dev *pctldev;
    struct gpio_chip chip;
    struct irq_chip irqchip;
    void *regs;
    unsigned int intr_lines[16];
    const struct chv_community *community;
    u32 saved_intmask;
    struct chv_pin_context *saved_pin_context;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct chv_pinctrl {
    struct device *dev;
    struct pinctrl_desc pctldesc;
    struct pinctrl_dev *pctldev;
    struct gpio_chip chip;
    struct irq_chip irqchip;
    void *regs;
    unsigned int irq;
    unsigned int intr_lines[16];
    const struct chv_community *community;
    u32 saved_intmask;
    struct chv_pin_context *saved_pin_context;
};
```
</details>
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
In <code>armhf</code>: Absent ⚠️
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
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct chv_pinctrl {
    struct device *dev;
    struct pinctrl_desc pctldesc;
    struct pinctrl_dev *pctldev;
    struct gpio_chip chip;
    struct irq_chip irqchip;
    void *regs;
    unsigned int intr_lines[16];
    const struct chv_community *community;
    u32 saved_intmask;
    struct chv_pin_context *saved_pin_context;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct chv_pinctrl {
    struct device *dev;
    struct pinctrl_desc pctldesc;
    struct pinctrl_dev *pctldev;
    struct gpio_chip chip;
    struct irq_chip irqchip;
    void *regs;
    unsigned int intr_lines[16];
    const struct chv_community *community;
    u32 saved_intmask;
    struct chv_pin_context *saved_pin_context;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct chv_pinctrl {
    struct device *dev;
    struct pinctrl_desc pctldesc;
    struct pinctrl_dev *pctldev;
    struct gpio_chip chip;
    struct irq_chip irqchip;
    void *regs;
    unsigned int intr_lines[16];
    const struct chv_community *community;
    u32 saved_intmask;
    struct chv_pin_context *saved_pin_context;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct irq_chip irqchip</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int irq</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Arch</b>
<ul>
</ul>
<b>Flavor</b>
<ul>
<li>
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
