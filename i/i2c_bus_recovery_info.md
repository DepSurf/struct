# Struct: <code>i2c_bus_recovery_info</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct i2c_bus_recovery_info {
    int (*recover_bus)(struct i2c_adapter *);
    int (*get_scl)(struct i2c_adapter *);
    void (*set_scl)(struct i2c_adapter *, int);
    int (*get_sda)(struct i2c_adapter *);
    void (*prepare_recovery)(struct i2c_adapter *);
    void (*unprepare_recovery)(struct i2c_adapter *);
    int scl_gpio;
    int sda_gpio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct i2c_bus_recovery_info {
    int (*recover_bus)(struct i2c_adapter *);
    int (*get_scl)(struct i2c_adapter *);
    void (*set_scl)(struct i2c_adapter *, int);
    int (*get_sda)(struct i2c_adapter *);
    void (*prepare_recovery)(struct i2c_adapter *);
    void (*unprepare_recovery)(struct i2c_adapter *);
    int scl_gpio;
    int sda_gpio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct i2c_bus_recovery_info {
    int (*recover_bus)(struct i2c_adapter *);
    int (*get_scl)(struct i2c_adapter *);
    void (*set_scl)(struct i2c_adapter *, int);
    int (*get_sda)(struct i2c_adapter *);
    void (*prepare_recovery)(struct i2c_adapter *);
    void (*unprepare_recovery)(struct i2c_adapter *);
    int scl_gpio;
    int sda_gpio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct i2c_bus_recovery_info {
    int (*recover_bus)(struct i2c_adapter *);
    int (*get_scl)(struct i2c_adapter *);
    void (*set_scl)(struct i2c_adapter *, int);
    int (*get_sda)(struct i2c_adapter *);
    void (*prepare_recovery)(struct i2c_adapter *);
    void (*unprepare_recovery)(struct i2c_adapter *);
    int scl_gpio;
    int sda_gpio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct i2c_bus_recovery_info {
    int (*recover_bus)(struct i2c_adapter *);
    int (*get_scl)(struct i2c_adapter *);
    void (*set_scl)(struct i2c_adapter *, int);
    int (*get_sda)(struct i2c_adapter *);
    void (*prepare_recovery)(struct i2c_adapter *);
    void (*unprepare_recovery)(struct i2c_adapter *);
    int scl_gpio;
    int sda_gpio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct i2c_bus_recovery_info {
    int (*recover_bus)(struct i2c_adapter *);
    int (*get_scl)(struct i2c_adapter *);
    void (*set_scl)(struct i2c_adapter *, int);
    int (*get_sda)(struct i2c_adapter *);
    void (*set_sda)(struct i2c_adapter *, int);
    void (*prepare_recovery)(struct i2c_adapter *);
    void (*unprepare_recovery)(struct i2c_adapter *);
    struct gpio_desc *scl_gpiod;
    struct gpio_desc *sda_gpiod;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct i2c_bus_recovery_info {
    int (*recover_bus)(struct i2c_adapter *);
    int (*get_scl)(struct i2c_adapter *);
    void (*set_scl)(struct i2c_adapter *, int);
    int (*get_sda)(struct i2c_adapter *);
    void (*set_sda)(struct i2c_adapter *, int);
    int (*get_bus_free)(struct i2c_adapter *);
    void (*prepare_recovery)(struct i2c_adapter *);
    void (*unprepare_recovery)(struct i2c_adapter *);
    struct gpio_desc *scl_gpiod;
    struct gpio_desc *sda_gpiod;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct i2c_bus_recovery_info {
    int (*recover_bus)(struct i2c_adapter *);
    int (*get_scl)(struct i2c_adapter *);
    void (*set_scl)(struct i2c_adapter *, int);
    int (*get_sda)(struct i2c_adapter *);
    void (*set_sda)(struct i2c_adapter *, int);
    int (*get_bus_free)(struct i2c_adapter *);
    void (*prepare_recovery)(struct i2c_adapter *);
    void (*unprepare_recovery)(struct i2c_adapter *);
    struct gpio_desc *scl_gpiod;
    struct gpio_desc *sda_gpiod;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct i2c_bus_recovery_info {
    int (*recover_bus)(struct i2c_adapter *);
    int (*get_scl)(struct i2c_adapter *);
    void (*set_scl)(struct i2c_adapter *, int);
    int (*get_sda)(struct i2c_adapter *);
    void (*set_sda)(struct i2c_adapter *, int);
    int (*get_bus_free)(struct i2c_adapter *);
    void (*prepare_recovery)(struct i2c_adapter *);
    void (*unprepare_recovery)(struct i2c_adapter *);
    struct gpio_desc *scl_gpiod;
    struct gpio_desc *sda_gpiod;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct i2c_bus_recovery_info {
    int (*recover_bus)(struct i2c_adapter *);
    int (*get_scl)(struct i2c_adapter *);
    void (*set_scl)(struct i2c_adapter *, int);
    int (*get_sda)(struct i2c_adapter *);
    void (*set_sda)(struct i2c_adapter *, int);
    int (*get_bus_free)(struct i2c_adapter *);
    void (*prepare_recovery)(struct i2c_adapter *);
    void (*unprepare_recovery)(struct i2c_adapter *);
    struct gpio_desc *scl_gpiod;
    struct gpio_desc *sda_gpiod;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct i2c_bus_recovery_info {
    int (*recover_bus)(struct i2c_adapter *);
    int (*get_scl)(struct i2c_adapter *);
    void (*set_scl)(struct i2c_adapter *, int);
    int (*get_sda)(struct i2c_adapter *);
    void (*set_sda)(struct i2c_adapter *, int);
    int (*get_bus_free)(struct i2c_adapter *);
    void (*prepare_recovery)(struct i2c_adapter *);
    void (*unprepare_recovery)(struct i2c_adapter *);
    struct gpio_desc *scl_gpiod;
    struct gpio_desc *sda_gpiod;
    struct pinctrl *pinctrl;
    struct pinctrl_state *pins_default;
    struct pinctrl_state *pins_gpio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct i2c_bus_recovery_info {
    int (*recover_bus)(struct i2c_adapter *);
    int (*get_scl)(struct i2c_adapter *);
    void (*set_scl)(struct i2c_adapter *, int);
    int (*get_sda)(struct i2c_adapter *);
    void (*set_sda)(struct i2c_adapter *, int);
    int (*get_bus_free)(struct i2c_adapter *);
    void (*prepare_recovery)(struct i2c_adapter *);
    void (*unprepare_recovery)(struct i2c_adapter *);
    struct gpio_desc *scl_gpiod;
    struct gpio_desc *sda_gpiod;
    struct pinctrl *pinctrl;
    struct pinctrl_state *pins_default;
    struct pinctrl_state *pins_gpio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct i2c_bus_recovery_info {
    int (*recover_bus)(struct i2c_adapter *);
    int (*get_scl)(struct i2c_adapter *);
    void (*set_scl)(struct i2c_adapter *, int);
    int (*get_sda)(struct i2c_adapter *);
    void (*set_sda)(struct i2c_adapter *, int);
    int (*get_bus_free)(struct i2c_adapter *);
    void (*prepare_recovery)(struct i2c_adapter *);
    void (*unprepare_recovery)(struct i2c_adapter *);
    struct gpio_desc *scl_gpiod;
    struct gpio_desc *sda_gpiod;
    struct pinctrl *pinctrl;
    struct pinctrl_state *pins_default;
    struct pinctrl_state *pins_gpio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct i2c_bus_recovery_info {
    int (*recover_bus)(struct i2c_adapter *);
    int (*get_scl)(struct i2c_adapter *);
    void (*set_scl)(struct i2c_adapter *, int);
    int (*get_sda)(struct i2c_adapter *);
    void (*set_sda)(struct i2c_adapter *, int);
    int (*get_bus_free)(struct i2c_adapter *);
    void (*prepare_recovery)(struct i2c_adapter *);
    void (*unprepare_recovery)(struct i2c_adapter *);
    struct gpio_desc *scl_gpiod;
    struct gpio_desc *sda_gpiod;
    struct pinctrl *pinctrl;
    struct pinctrl_state *pins_default;
    struct pinctrl_state *pins_gpio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct i2c_bus_recovery_info {
    int (*recover_bus)(struct i2c_adapter *);
    int (*get_scl)(struct i2c_adapter *);
    void (*set_scl)(struct i2c_adapter *, int);
    int (*get_sda)(struct i2c_adapter *);
    void (*set_sda)(struct i2c_adapter *, int);
    int (*get_bus_free)(struct i2c_adapter *);
    void (*prepare_recovery)(struct i2c_adapter *);
    void (*unprepare_recovery)(struct i2c_adapter *);
    struct gpio_desc *scl_gpiod;
    struct gpio_desc *sda_gpiod;
    struct pinctrl *pinctrl;
    struct pinctrl_state *pins_default;
    struct pinctrl_state *pins_gpio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct i2c_bus_recovery_info {
    int (*recover_bus)(struct i2c_adapter *);
    int (*get_scl)(struct i2c_adapter *);
    void (*set_scl)(struct i2c_adapter *, int);
    int (*get_sda)(struct i2c_adapter *);
    void (*set_sda)(struct i2c_adapter *, int);
    int (*get_bus_free)(struct i2c_adapter *);
    void (*prepare_recovery)(struct i2c_adapter *);
    void (*unprepare_recovery)(struct i2c_adapter *);
    struct gpio_desc *scl_gpiod;
    struct gpio_desc *sda_gpiod;
    struct pinctrl *pinctrl;
    struct pinctrl_state *pins_default;
    struct pinctrl_state *pins_gpio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct i2c_bus_recovery_info {
    int (*recover_bus)(struct i2c_adapter *);
    int (*get_scl)(struct i2c_adapter *);
    void (*set_scl)(struct i2c_adapter *, int);
    int (*get_sda)(struct i2c_adapter *);
    void (*set_sda)(struct i2c_adapter *, int);
    int (*get_bus_free)(struct i2c_adapter *);
    void (*prepare_recovery)(struct i2c_adapter *);
    void (*unprepare_recovery)(struct i2c_adapter *);
    struct gpio_desc *scl_gpiod;
    struct gpio_desc *sda_gpiod;
    struct pinctrl *pinctrl;
    struct pinctrl_state *pins_default;
    struct pinctrl_state *pins_gpio;
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
struct i2c_bus_recovery_info {
    int (*recover_bus)(struct i2c_adapter *);
    int (*get_scl)(struct i2c_adapter *);
    void (*set_scl)(struct i2c_adapter *, int);
    int (*get_sda)(struct i2c_adapter *);
    void (*set_sda)(struct i2c_adapter *, int);
    int (*get_bus_free)(struct i2c_adapter *);
    void (*prepare_recovery)(struct i2c_adapter *);
    void (*unprepare_recovery)(struct i2c_adapter *);
    struct gpio_desc *scl_gpiod;
    struct gpio_desc *sda_gpiod;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct i2c_bus_recovery_info {
    int (*recover_bus)(struct i2c_adapter *);
    int (*get_scl)(struct i2c_adapter *);
    void (*set_scl)(struct i2c_adapter *, int);
    int (*get_sda)(struct i2c_adapter *);
    void (*set_sda)(struct i2c_adapter *, int);
    int (*get_bus_free)(struct i2c_adapter *);
    void (*prepare_recovery)(struct i2c_adapter *);
    void (*unprepare_recovery)(struct i2c_adapter *);
    struct gpio_desc *scl_gpiod;
    struct gpio_desc *sda_gpiod;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct i2c_bus_recovery_info {
    int (*recover_bus)(struct i2c_adapter *);
    int (*get_scl)(struct i2c_adapter *);
    void (*set_scl)(struct i2c_adapter *, int);
    int (*get_sda)(struct i2c_adapter *);
    void (*set_sda)(struct i2c_adapter *, int);
    int (*get_bus_free)(struct i2c_adapter *);
    void (*prepare_recovery)(struct i2c_adapter *);
    void (*unprepare_recovery)(struct i2c_adapter *);
    struct gpio_desc *scl_gpiod;
    struct gpio_desc *sda_gpiod;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct i2c_bus_recovery_info {
    int (*recover_bus)(struct i2c_adapter *);
    int (*get_scl)(struct i2c_adapter *);
    void (*set_scl)(struct i2c_adapter *, int);
    int (*get_sda)(struct i2c_adapter *);
    void (*set_sda)(struct i2c_adapter *, int);
    int (*get_bus_free)(struct i2c_adapter *);
    void (*prepare_recovery)(struct i2c_adapter *);
    void (*unprepare_recovery)(struct i2c_adapter *);
    struct gpio_desc *scl_gpiod;
    struct gpio_desc *sda_gpiod;
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
struct i2c_bus_recovery_info {
    int (*recover_bus)(struct i2c_adapter *);
    int (*get_scl)(struct i2c_adapter *);
    void (*set_scl)(struct i2c_adapter *, int);
    int (*get_sda)(struct i2c_adapter *);
    void (*set_sda)(struct i2c_adapter *, int);
    int (*get_bus_free)(struct i2c_adapter *);
    void (*prepare_recovery)(struct i2c_adapter *);
    void (*unprepare_recovery)(struct i2c_adapter *);
    struct gpio_desc *scl_gpiod;
    struct gpio_desc *sda_gpiod;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct i2c_bus_recovery_info {
    int (*recover_bus)(struct i2c_adapter *);
    int (*get_scl)(struct i2c_adapter *);
    void (*set_scl)(struct i2c_adapter *, int);
    int (*get_sda)(struct i2c_adapter *);
    void (*set_sda)(struct i2c_adapter *, int);
    int (*get_bus_free)(struct i2c_adapter *);
    void (*prepare_recovery)(struct i2c_adapter *);
    void (*unprepare_recovery)(struct i2c_adapter *);
    struct gpio_desc *scl_gpiod;
    struct gpio_desc *sda_gpiod;
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
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*set_sda)(struct i2c_adapter *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>struct gpio_desc *scl_gpiod</code>
</li>
<li>
<b>Field added. </b>
<code>struct gpio_desc *sda_gpiod</code>
</li>
<li>
<b>Field removed. </b>
<code>int scl_gpio</code>
</li>
<li>
<b>Field removed. </b>
<code>int sda_gpio</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*get_bus_free)(struct i2c_adapter *)</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct pinctrl *pinctrl</code>
</li>
<li>
<b>Field added. </b>
<code>struct pinctrl_state *pins_default</code>
</li>
<li>
<b>Field added. </b>
<code>struct pinctrl_state *pins_gpio</code>
</li>
</ul>
</details>
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
