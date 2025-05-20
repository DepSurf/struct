# Struct: <code>sx150x_device_data</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct sx150x_device_data {
    u8 model;
    u8 reg_pullup;
    u8 reg_pulldn;
    u8 reg_dir;
    u8 reg_data;
    u8 reg_irq_mask;
    u8 reg_irq_src;
    u8 reg_sense;
    u8 ngpios;
    union (anon) pri;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct sx150x_device_data {
    u8 model;
    u8 reg_pullup;
    u8 reg_pulldn;
    u8 reg_dir;
    u8 reg_data;
    u8 reg_irq_mask;
    u8 reg_irq_src;
    u8 reg_sense;
    u8 ngpios;
    union (anon) pri;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct sx150x_device_data {
    u8 model;
    u8 reg_pullup;
    u8 reg_pulldn;
    u8 reg_dir;
    u8 reg_data;
    u8 reg_irq_mask;
    u8 reg_irq_src;
    u8 reg_sense;
    u8 ngpios;
    union (anon) pri;
    const struct pinctrl_pin_desc *pins;
    unsigned int npins;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct sx150x_device_data {
    u8 model;
    u8 reg_pullup;
    u8 reg_pulldn;
    u8 reg_dir;
    u8 reg_data;
    u8 reg_irq_mask;
    u8 reg_irq_src;
    u8 reg_sense;
    u8 ngpios;
    union (anon) pri;
    const struct pinctrl_pin_desc *pins;
    unsigned int npins;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct sx150x_device_data {
    u8 model;
    u8 reg_pullup;
    u8 reg_pulldn;
    u8 reg_dir;
    u8 reg_data;
    u8 reg_irq_mask;
    u8 reg_irq_src;
    u8 reg_sense;
    u8 ngpios;
    union (anon) pri;
    const struct pinctrl_pin_desc *pins;
    unsigned int npins;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct sx150x_device_data {
    u8 model;
    u8 reg_pullup;
    u8 reg_pulldn;
    u8 reg_dir;
    u8 reg_data;
    u8 reg_irq_mask;
    u8 reg_irq_src;
    u8 reg_sense;
    u8 ngpios;
    union (anon) pri;
    const struct pinctrl_pin_desc *pins;
    unsigned int npins;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct sx150x_device_data {
    u8 model;
    u8 reg_pullup;
    u8 reg_pulldn;
    u8 reg_dir;
    u8 reg_data;
    u8 reg_irq_mask;
    u8 reg_irq_src;
    u8 reg_sense;
    u8 ngpios;
    union (anon) pri;
    const struct pinctrl_pin_desc *pins;
    unsigned int npins;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct sx150x_device_data {
    u8 model;
    u8 reg_pullup;
    u8 reg_pulldn;
    u8 reg_dir;
    u8 reg_data;
    u8 reg_irq_mask;
    u8 reg_irq_src;
    u8 reg_sense;
    u8 ngpios;
    union (anon) pri;
    const struct pinctrl_pin_desc *pins;
    unsigned int npins;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct sx150x_device_data {
    u8 model;
    u8 reg_pullup;
    u8 reg_pulldn;
    u8 reg_dir;
    u8 reg_data;
    u8 reg_irq_mask;
    u8 reg_irq_src;
    u8 reg_sense;
    u8 ngpios;
    union (anon) pri;
    const struct pinctrl_pin_desc *pins;
    unsigned int npins;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct sx150x_device_data {
    u8 model;
    u8 reg_pullup;
    u8 reg_pulldn;
    u8 reg_dir;
    u8 reg_data;
    u8 reg_irq_mask;
    u8 reg_irq_src;
    u8 reg_sense;
    u8 ngpios;
    union (anon) pri;
    const struct pinctrl_pin_desc *pins;
    unsigned int npins;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct sx150x_device_data {
    u8 model;
    u8 reg_pullup;
    u8 reg_pulldn;
    u8 reg_dir;
    u8 reg_data;
    u8 reg_irq_mask;
    u8 reg_irq_src;
    u8 reg_sense;
    u8 ngpios;
    union (anon) pri;
    const struct pinctrl_pin_desc *pins;
    unsigned int npins;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct sx150x_device_data {
    u8 model;
    u8 reg_pullup;
    u8 reg_pulldn;
    u8 reg_dir;
    u8 reg_data;
    u8 reg_irq_mask;
    u8 reg_irq_src;
    u8 reg_sense;
    u8 ngpios;
    union (anon) pri;
    const struct pinctrl_pin_desc *pins;
    unsigned int npins;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct sx150x_device_data {
    u8 model;
    u8 reg_pullup;
    u8 reg_pulldn;
    u8 reg_dir;
    u8 reg_data;
    u8 reg_irq_mask;
    u8 reg_irq_src;
    u8 reg_sense;
    u8 ngpios;
    union (anon) pri;
    const struct pinctrl_pin_desc *pins;
    unsigned int npins;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct sx150x_device_data {
    u8 model;
    u8 reg_pullup;
    u8 reg_pulldn;
    u8 reg_dir;
    u8 reg_data;
    u8 reg_irq_mask;
    u8 reg_irq_src;
    u8 reg_sense;
    u8 ngpios;
    union (anon) pri;
    const struct pinctrl_pin_desc *pins;
    unsigned int npins;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct sx150x_device_data {
    u8 model;
    u8 reg_pullup;
    u8 reg_pulldn;
    u8 reg_dir;
    u8 reg_data;
    u8 reg_irq_mask;
    u8 reg_irq_src;
    u8 reg_sense;
    u8 ngpios;
    union (anon) pri;
    const struct pinctrl_pin_desc *pins;
    unsigned int npins;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct sx150x_device_data {
    u8 model;
    u8 reg_pullup;
    u8 reg_pulldn;
    u8 reg_dir;
    u8 reg_data;
    u8 reg_irq_mask;
    u8 reg_irq_src;
    u8 reg_sense;
    u8 ngpios;
    union (anon) pri;
    const struct pinctrl_pin_desc *pins;
    unsigned int npins;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct sx150x_device_data {
    u8 model;
    u8 reg_pullup;
    u8 reg_pulldn;
    u8 reg_dir;
    u8 reg_data;
    u8 reg_irq_mask;
    u8 reg_irq_src;
    u8 reg_sense;
    u8 ngpios;
    union (anon) pri;
    const struct pinctrl_pin_desc *pins;
    unsigned int npins;
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct sx150x_device_data {
    u8 model;
    u8 reg_pullup;
    u8 reg_pulldn;
    u8 reg_dir;
    u8 reg_data;
    u8 reg_irq_mask;
    u8 reg_irq_src;
    u8 reg_sense;
    u8 ngpios;
    union (anon) pri;
    const struct pinctrl_pin_desc *pins;
    unsigned int npins;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct sx150x_device_data {
    u8 model;
    u8 reg_pullup;
    u8 reg_pulldn;
    u8 reg_dir;
    u8 reg_data;
    u8 reg_irq_mask;
    u8 reg_irq_src;
    u8 reg_sense;
    u8 ngpios;
    union (anon) pri;
    const struct pinctrl_pin_desc *pins;
    unsigned int npins;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct sx150x_device_data {
    u8 model;
    u8 reg_pullup;
    u8 reg_pulldn;
    u8 reg_dir;
    u8 reg_data;
    u8 reg_irq_mask;
    u8 reg_irq_src;
    u8 reg_sense;
    u8 ngpios;
    union (anon) pri;
    const struct pinctrl_pin_desc *pins;
    unsigned int npins;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct sx150x_device_data {
    u8 model;
    u8 reg_pullup;
    u8 reg_pulldn;
    u8 reg_dir;
    u8 reg_data;
    u8 reg_irq_mask;
    u8 reg_irq_src;
    u8 reg_sense;
    u8 ngpios;
    union (anon) pri;
    const struct pinctrl_pin_desc *pins;
    unsigned int npins;
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
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct sx150x_device_data {
    u8 model;
    u8 reg_pullup;
    u8 reg_pulldn;
    u8 reg_dir;
    u8 reg_data;
    u8 reg_irq_mask;
    u8 reg_irq_src;
    u8 reg_sense;
    u8 ngpios;
    union (anon) pri;
    const struct pinctrl_pin_desc *pins;
    unsigned int npins;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct sx150x_device_data {
    u8 model;
    u8 reg_pullup;
    u8 reg_pulldn;
    u8 reg_dir;
    u8 reg_data;
    u8 reg_irq_mask;
    u8 reg_irq_src;
    u8 reg_sense;
    u8 ngpios;
    union (anon) pri;
    const struct pinctrl_pin_desc *pins;
    unsigned int npins;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.4</code> and <code>4.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const struct pinctrl_pin_desc *pins</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int npins</code>
</li>
</ul>
</details>
</li>
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
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
<b>Arch</b>
<ul>
<li>
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>armhf</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>riscv64</code> ✅
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
