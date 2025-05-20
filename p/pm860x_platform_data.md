# Struct: <code>pm860x_platform_data</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct pm860x_platform_data {
    struct pm860x_backlight_pdata *backlight;
    struct pm860x_led_pdata *led;
    struct pm860x_rtc_pdata *rtc;
    struct pm860x_touch_pdata *touch;
    struct pm860x_power_pdata *power;
    struct regulator_init_data *buck1;
    struct regulator_init_data *buck2;
    struct regulator_init_data *buck3;
    struct regulator_init_data *ldo1;
    struct regulator_init_data *ldo2;
    struct regulator_init_data *ldo3;
    struct regulator_init_data *ldo4;
    struct regulator_init_data *ldo5;
    struct regulator_init_data *ldo6;
    struct regulator_init_data *ldo7;
    struct regulator_init_data *ldo8;
    struct regulator_init_data *ldo9;
    struct regulator_init_data *ldo10;
    struct regulator_init_data *ldo12;
    struct regulator_init_data *ldo_vibrator;
    struct regulator_init_data *ldo14;
    struct charger_desc *chg_desc;
    int companion_addr;
    int i2c_port;
    int irq_mode;
    int irq_base;
    int num_leds;
    int num_backlights;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct pm860x_platform_data {
    struct pm860x_backlight_pdata *backlight;
    struct pm860x_led_pdata *led;
    struct pm860x_rtc_pdata *rtc;
    struct pm860x_touch_pdata *touch;
    struct pm860x_power_pdata *power;
    struct regulator_init_data *buck1;
    struct regulator_init_data *buck2;
    struct regulator_init_data *buck3;
    struct regulator_init_data *ldo1;
    struct regulator_init_data *ldo2;
    struct regulator_init_data *ldo3;
    struct regulator_init_data *ldo4;
    struct regulator_init_data *ldo5;
    struct regulator_init_data *ldo6;
    struct regulator_init_data *ldo7;
    struct regulator_init_data *ldo8;
    struct regulator_init_data *ldo9;
    struct regulator_init_data *ldo10;
    struct regulator_init_data *ldo12;
    struct regulator_init_data *ldo_vibrator;
    struct regulator_init_data *ldo14;
    struct charger_desc *chg_desc;
    int companion_addr;
    int i2c_port;
    int irq_mode;
    int irq_base;
    int num_leds;
    int num_backlights;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct pm860x_platform_data {
    struct pm860x_backlight_pdata *backlight;
    struct pm860x_led_pdata *led;
    struct pm860x_rtc_pdata *rtc;
    struct pm860x_touch_pdata *touch;
    struct pm860x_power_pdata *power;
    struct regulator_init_data *buck1;
    struct regulator_init_data *buck2;
    struct regulator_init_data *buck3;
    struct regulator_init_data *ldo1;
    struct regulator_init_data *ldo2;
    struct regulator_init_data *ldo3;
    struct regulator_init_data *ldo4;
    struct regulator_init_data *ldo5;
    struct regulator_init_data *ldo6;
    struct regulator_init_data *ldo7;
    struct regulator_init_data *ldo8;
    struct regulator_init_data *ldo9;
    struct regulator_init_data *ldo10;
    struct regulator_init_data *ldo12;
    struct regulator_init_data *ldo_vibrator;
    struct regulator_init_data *ldo14;
    struct charger_desc *chg_desc;
    int companion_addr;
    int i2c_port;
    int irq_mode;
    int irq_base;
    int num_leds;
    int num_backlights;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct pm860x_platform_data {
    struct pm860x_backlight_pdata *backlight;
    struct pm860x_led_pdata *led;
    struct pm860x_rtc_pdata *rtc;
    struct pm860x_touch_pdata *touch;
    struct pm860x_power_pdata *power;
    struct regulator_init_data *buck1;
    struct regulator_init_data *buck2;
    struct regulator_init_data *buck3;
    struct regulator_init_data *ldo1;
    struct regulator_init_data *ldo2;
    struct regulator_init_data *ldo3;
    struct regulator_init_data *ldo4;
    struct regulator_init_data *ldo5;
    struct regulator_init_data *ldo6;
    struct regulator_init_data *ldo7;
    struct regulator_init_data *ldo8;
    struct regulator_init_data *ldo9;
    struct regulator_init_data *ldo10;
    struct regulator_init_data *ldo12;
    struct regulator_init_data *ldo_vibrator;
    struct regulator_init_data *ldo14;
    struct charger_desc *chg_desc;
    int companion_addr;
    int i2c_port;
    int irq_mode;
    int irq_base;
    int num_leds;
    int num_backlights;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct pm860x_platform_data {
    struct pm860x_backlight_pdata *backlight;
    struct pm860x_led_pdata *led;
    struct pm860x_rtc_pdata *rtc;
    struct pm860x_touch_pdata *touch;
    struct pm860x_power_pdata *power;
    struct regulator_init_data *buck1;
    struct regulator_init_data *buck2;
    struct regulator_init_data *buck3;
    struct regulator_init_data *ldo1;
    struct regulator_init_data *ldo2;
    struct regulator_init_data *ldo3;
    struct regulator_init_data *ldo4;
    struct regulator_init_data *ldo5;
    struct regulator_init_data *ldo6;
    struct regulator_init_data *ldo7;
    struct regulator_init_data *ldo8;
    struct regulator_init_data *ldo9;
    struct regulator_init_data *ldo10;
    struct regulator_init_data *ldo12;
    struct regulator_init_data *ldo_vibrator;
    struct regulator_init_data *ldo14;
    struct charger_desc *chg_desc;
    int companion_addr;
    int i2c_port;
    int irq_mode;
    int irq_base;
    int num_leds;
    int num_backlights;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct pm860x_platform_data {
    struct pm860x_backlight_pdata *backlight;
    struct pm860x_led_pdata *led;
    struct pm860x_rtc_pdata *rtc;
    struct pm860x_touch_pdata *touch;
    struct pm860x_power_pdata *power;
    struct regulator_init_data *buck1;
    struct regulator_init_data *buck2;
    struct regulator_init_data *buck3;
    struct regulator_init_data *ldo1;
    struct regulator_init_data *ldo2;
    struct regulator_init_data *ldo3;
    struct regulator_init_data *ldo4;
    struct regulator_init_data *ldo5;
    struct regulator_init_data *ldo6;
    struct regulator_init_data *ldo7;
    struct regulator_init_data *ldo8;
    struct regulator_init_data *ldo9;
    struct regulator_init_data *ldo10;
    struct regulator_init_data *ldo12;
    struct regulator_init_data *ldo_vibrator;
    struct regulator_init_data *ldo14;
    struct charger_desc *chg_desc;
    int companion_addr;
    int i2c_port;
    int irq_mode;
    int irq_base;
    int num_leds;
    int num_backlights;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct pm860x_platform_data {
    struct pm860x_backlight_pdata *backlight;
    struct pm860x_led_pdata *led;
    struct pm860x_rtc_pdata *rtc;
    struct pm860x_touch_pdata *touch;
    struct pm860x_power_pdata *power;
    struct regulator_init_data *buck1;
    struct regulator_init_data *buck2;
    struct regulator_init_data *buck3;
    struct regulator_init_data *ldo1;
    struct regulator_init_data *ldo2;
    struct regulator_init_data *ldo3;
    struct regulator_init_data *ldo4;
    struct regulator_init_data *ldo5;
    struct regulator_init_data *ldo6;
    struct regulator_init_data *ldo7;
    struct regulator_init_data *ldo8;
    struct regulator_init_data *ldo9;
    struct regulator_init_data *ldo10;
    struct regulator_init_data *ldo12;
    struct regulator_init_data *ldo_vibrator;
    struct regulator_init_data *ldo14;
    struct charger_desc *chg_desc;
    int companion_addr;
    int i2c_port;
    int irq_mode;
    int irq_base;
    int num_leds;
    int num_backlights;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct pm860x_platform_data {
    struct pm860x_backlight_pdata *backlight;
    struct pm860x_led_pdata *led;
    struct pm860x_rtc_pdata *rtc;
    struct pm860x_touch_pdata *touch;
    struct pm860x_power_pdata *power;
    struct regulator_init_data *buck1;
    struct regulator_init_data *buck2;
    struct regulator_init_data *buck3;
    struct regulator_init_data *ldo1;
    struct regulator_init_data *ldo2;
    struct regulator_init_data *ldo3;
    struct regulator_init_data *ldo4;
    struct regulator_init_data *ldo5;
    struct regulator_init_data *ldo6;
    struct regulator_init_data *ldo7;
    struct regulator_init_data *ldo8;
    struct regulator_init_data *ldo9;
    struct regulator_init_data *ldo10;
    struct regulator_init_data *ldo12;
    struct regulator_init_data *ldo_vibrator;
    struct regulator_init_data *ldo14;
    struct charger_desc *chg_desc;
    int companion_addr;
    int i2c_port;
    int irq_mode;
    int irq_base;
    int num_leds;
    int num_backlights;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct pm860x_platform_data {
    struct pm860x_backlight_pdata *backlight;
    struct pm860x_led_pdata *led;
    struct pm860x_rtc_pdata *rtc;
    struct pm860x_touch_pdata *touch;
    struct pm860x_power_pdata *power;
    struct regulator_init_data *buck1;
    struct regulator_init_data *buck2;
    struct regulator_init_data *buck3;
    struct regulator_init_data *ldo1;
    struct regulator_init_data *ldo2;
    struct regulator_init_data *ldo3;
    struct regulator_init_data *ldo4;
    struct regulator_init_data *ldo5;
    struct regulator_init_data *ldo6;
    struct regulator_init_data *ldo7;
    struct regulator_init_data *ldo8;
    struct regulator_init_data *ldo9;
    struct regulator_init_data *ldo10;
    struct regulator_init_data *ldo12;
    struct regulator_init_data *ldo_vibrator;
    struct regulator_init_data *ldo14;
    struct charger_desc *chg_desc;
    int companion_addr;
    int i2c_port;
    int irq_mode;
    int irq_base;
    int num_leds;
    int num_backlights;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct pm860x_platform_data {
    struct pm860x_backlight_pdata *backlight;
    struct pm860x_led_pdata *led;
    struct pm860x_rtc_pdata *rtc;
    struct pm860x_touch_pdata *touch;
    struct pm860x_power_pdata *power;
    struct regulator_init_data *buck1;
    struct regulator_init_data *buck2;
    struct regulator_init_data *buck3;
    struct regulator_init_data *ldo1;
    struct regulator_init_data *ldo2;
    struct regulator_init_data *ldo3;
    struct regulator_init_data *ldo4;
    struct regulator_init_data *ldo5;
    struct regulator_init_data *ldo6;
    struct regulator_init_data *ldo7;
    struct regulator_init_data *ldo8;
    struct regulator_init_data *ldo9;
    struct regulator_init_data *ldo10;
    struct regulator_init_data *ldo12;
    struct regulator_init_data *ldo_vibrator;
    struct regulator_init_data *ldo14;
    struct charger_desc *chg_desc;
    int companion_addr;
    int i2c_port;
    int irq_mode;
    int irq_base;
    int num_leds;
    int num_backlights;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct pm860x_platform_data {
    struct pm860x_backlight_pdata *backlight;
    struct pm860x_led_pdata *led;
    struct pm860x_rtc_pdata *rtc;
    struct pm860x_touch_pdata *touch;
    struct pm860x_power_pdata *power;
    struct regulator_init_data *buck1;
    struct regulator_init_data *buck2;
    struct regulator_init_data *buck3;
    struct regulator_init_data *ldo1;
    struct regulator_init_data *ldo2;
    struct regulator_init_data *ldo3;
    struct regulator_init_data *ldo4;
    struct regulator_init_data *ldo5;
    struct regulator_init_data *ldo6;
    struct regulator_init_data *ldo7;
    struct regulator_init_data *ldo8;
    struct regulator_init_data *ldo9;
    struct regulator_init_data *ldo10;
    struct regulator_init_data *ldo12;
    struct regulator_init_data *ldo_vibrator;
    struct regulator_init_data *ldo14;
    struct charger_desc *chg_desc;
    int companion_addr;
    int i2c_port;
    int irq_mode;
    int irq_base;
    int num_leds;
    int num_backlights;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct pm860x_platform_data {
    struct pm860x_backlight_pdata *backlight;
    struct pm860x_led_pdata *led;
    struct pm860x_rtc_pdata *rtc;
    struct pm860x_touch_pdata *touch;
    struct pm860x_power_pdata *power;
    struct regulator_init_data *buck1;
    struct regulator_init_data *buck2;
    struct regulator_init_data *buck3;
    struct regulator_init_data *ldo1;
    struct regulator_init_data *ldo2;
    struct regulator_init_data *ldo3;
    struct regulator_init_data *ldo4;
    struct regulator_init_data *ldo5;
    struct regulator_init_data *ldo6;
    struct regulator_init_data *ldo7;
    struct regulator_init_data *ldo8;
    struct regulator_init_data *ldo9;
    struct regulator_init_data *ldo10;
    struct regulator_init_data *ldo12;
    struct regulator_init_data *ldo_vibrator;
    struct regulator_init_data *ldo14;
    struct charger_desc *chg_desc;
    int companion_addr;
    int i2c_port;
    int irq_mode;
    int irq_base;
    int num_leds;
    int num_backlights;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct pm860x_platform_data {
    struct pm860x_backlight_pdata *backlight;
    struct pm860x_led_pdata *led;
    struct pm860x_rtc_pdata *rtc;
    struct pm860x_touch_pdata *touch;
    struct pm860x_power_pdata *power;
    struct regulator_init_data *buck1;
    struct regulator_init_data *buck2;
    struct regulator_init_data *buck3;
    struct regulator_init_data *ldo1;
    struct regulator_init_data *ldo2;
    struct regulator_init_data *ldo3;
    struct regulator_init_data *ldo4;
    struct regulator_init_data *ldo5;
    struct regulator_init_data *ldo6;
    struct regulator_init_data *ldo7;
    struct regulator_init_data *ldo8;
    struct regulator_init_data *ldo9;
    struct regulator_init_data *ldo10;
    struct regulator_init_data *ldo12;
    struct regulator_init_data *ldo_vibrator;
    struct regulator_init_data *ldo14;
    struct charger_desc *chg_desc;
    int companion_addr;
    int i2c_port;
    int irq_mode;
    int irq_base;
    int num_leds;
    int num_backlights;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct pm860x_platform_data {
    struct pm860x_backlight_pdata *backlight;
    struct pm860x_led_pdata *led;
    struct pm860x_rtc_pdata *rtc;
    struct pm860x_touch_pdata *touch;
    struct pm860x_power_pdata *power;
    struct regulator_init_data *buck1;
    struct regulator_init_data *buck2;
    struct regulator_init_data *buck3;
    struct regulator_init_data *ldo1;
    struct regulator_init_data *ldo2;
    struct regulator_init_data *ldo3;
    struct regulator_init_data *ldo4;
    struct regulator_init_data *ldo5;
    struct regulator_init_data *ldo6;
    struct regulator_init_data *ldo7;
    struct regulator_init_data *ldo8;
    struct regulator_init_data *ldo9;
    struct regulator_init_data *ldo10;
    struct regulator_init_data *ldo12;
    struct regulator_init_data *ldo_vibrator;
    struct regulator_init_data *ldo14;
    struct charger_desc *chg_desc;
    int companion_addr;
    int i2c_port;
    int irq_mode;
    int irq_base;
    int num_leds;
    int num_backlights;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct pm860x_platform_data {
    struct pm860x_backlight_pdata *backlight;
    struct pm860x_led_pdata *led;
    struct pm860x_rtc_pdata *rtc;
    struct pm860x_touch_pdata *touch;
    struct pm860x_power_pdata *power;
    struct regulator_init_data *buck1;
    struct regulator_init_data *buck2;
    struct regulator_init_data *buck3;
    struct regulator_init_data *ldo1;
    struct regulator_init_data *ldo2;
    struct regulator_init_data *ldo3;
    struct regulator_init_data *ldo4;
    struct regulator_init_data *ldo5;
    struct regulator_init_data *ldo6;
    struct regulator_init_data *ldo7;
    struct regulator_init_data *ldo8;
    struct regulator_init_data *ldo9;
    struct regulator_init_data *ldo10;
    struct regulator_init_data *ldo12;
    struct regulator_init_data *ldo_vibrator;
    struct regulator_init_data *ldo14;
    struct charger_desc *chg_desc;
    int companion_addr;
    int i2c_port;
    int irq_mode;
    int irq_base;
    int num_leds;
    int num_backlights;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct pm860x_platform_data {
    struct pm860x_backlight_pdata *backlight;
    struct pm860x_led_pdata *led;
    struct pm860x_rtc_pdata *rtc;
    struct pm860x_touch_pdata *touch;
    struct pm860x_power_pdata *power;
    struct regulator_init_data *buck1;
    struct regulator_init_data *buck2;
    struct regulator_init_data *buck3;
    struct regulator_init_data *ldo1;
    struct regulator_init_data *ldo2;
    struct regulator_init_data *ldo3;
    struct regulator_init_data *ldo4;
    struct regulator_init_data *ldo5;
    struct regulator_init_data *ldo6;
    struct regulator_init_data *ldo7;
    struct regulator_init_data *ldo8;
    struct regulator_init_data *ldo9;
    struct regulator_init_data *ldo10;
    struct regulator_init_data *ldo12;
    struct regulator_init_data *ldo_vibrator;
    struct regulator_init_data *ldo14;
    struct charger_desc *chg_desc;
    int companion_addr;
    int i2c_port;
    int irq_mode;
    int irq_base;
    int num_leds;
    int num_backlights;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct pm860x_platform_data {
    struct pm860x_backlight_pdata *backlight;
    struct pm860x_led_pdata *led;
    struct pm860x_rtc_pdata *rtc;
    struct pm860x_touch_pdata *touch;
    struct pm860x_power_pdata *power;
    struct regulator_init_data *buck1;
    struct regulator_init_data *buck2;
    struct regulator_init_data *buck3;
    struct regulator_init_data *ldo1;
    struct regulator_init_data *ldo2;
    struct regulator_init_data *ldo3;
    struct regulator_init_data *ldo4;
    struct regulator_init_data *ldo5;
    struct regulator_init_data *ldo6;
    struct regulator_init_data *ldo7;
    struct regulator_init_data *ldo8;
    struct regulator_init_data *ldo9;
    struct regulator_init_data *ldo10;
    struct regulator_init_data *ldo12;
    struct regulator_init_data *ldo_vibrator;
    struct regulator_init_data *ldo14;
    struct charger_desc *chg_desc;
    int companion_addr;
    int i2c_port;
    int irq_mode;
    int irq_base;
    int num_leds;
    int num_backlights;
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
struct pm860x_platform_data {
    struct pm860x_backlight_pdata *backlight;
    struct pm860x_led_pdata *led;
    struct pm860x_rtc_pdata *rtc;
    struct pm860x_touch_pdata *touch;
    struct pm860x_power_pdata *power;
    struct regulator_init_data *buck1;
    struct regulator_init_data *buck2;
    struct regulator_init_data *buck3;
    struct regulator_init_data *ldo1;
    struct regulator_init_data *ldo2;
    struct regulator_init_data *ldo3;
    struct regulator_init_data *ldo4;
    struct regulator_init_data *ldo5;
    struct regulator_init_data *ldo6;
    struct regulator_init_data *ldo7;
    struct regulator_init_data *ldo8;
    struct regulator_init_data *ldo9;
    struct regulator_init_data *ldo10;
    struct regulator_init_data *ldo12;
    struct regulator_init_data *ldo_vibrator;
    struct regulator_init_data *ldo14;
    struct charger_desc *chg_desc;
    int companion_addr;
    int i2c_port;
    int irq_mode;
    int irq_base;
    int num_leds;
    int num_backlights;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct pm860x_platform_data {
    struct pm860x_backlight_pdata *backlight;
    struct pm860x_led_pdata *led;
    struct pm860x_rtc_pdata *rtc;
    struct pm860x_touch_pdata *touch;
    struct pm860x_power_pdata *power;
    struct regulator_init_data *buck1;
    struct regulator_init_data *buck2;
    struct regulator_init_data *buck3;
    struct regulator_init_data *ldo1;
    struct regulator_init_data *ldo2;
    struct regulator_init_data *ldo3;
    struct regulator_init_data *ldo4;
    struct regulator_init_data *ldo5;
    struct regulator_init_data *ldo6;
    struct regulator_init_data *ldo7;
    struct regulator_init_data *ldo8;
    struct regulator_init_data *ldo9;
    struct regulator_init_data *ldo10;
    struct regulator_init_data *ldo12;
    struct regulator_init_data *ldo_vibrator;
    struct regulator_init_data *ldo14;
    struct charger_desc *chg_desc;
    int companion_addr;
    int i2c_port;
    int irq_mode;
    int irq_base;
    int num_leds;
    int num_backlights;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct pm860x_platform_data {
    struct pm860x_backlight_pdata *backlight;
    struct pm860x_led_pdata *led;
    struct pm860x_rtc_pdata *rtc;
    struct pm860x_touch_pdata *touch;
    struct pm860x_power_pdata *power;
    struct regulator_init_data *buck1;
    struct regulator_init_data *buck2;
    struct regulator_init_data *buck3;
    struct regulator_init_data *ldo1;
    struct regulator_init_data *ldo2;
    struct regulator_init_data *ldo3;
    struct regulator_init_data *ldo4;
    struct regulator_init_data *ldo5;
    struct regulator_init_data *ldo6;
    struct regulator_init_data *ldo7;
    struct regulator_init_data *ldo8;
    struct regulator_init_data *ldo9;
    struct regulator_init_data *ldo10;
    struct regulator_init_data *ldo12;
    struct regulator_init_data *ldo_vibrator;
    struct regulator_init_data *ldo14;
    struct charger_desc *chg_desc;
    int companion_addr;
    int i2c_port;
    int irq_mode;
    int irq_base;
    int num_leds;
    int num_backlights;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct pm860x_platform_data {
    struct pm860x_backlight_pdata *backlight;
    struct pm860x_led_pdata *led;
    struct pm860x_rtc_pdata *rtc;
    struct pm860x_touch_pdata *touch;
    struct pm860x_power_pdata *power;
    struct regulator_init_data *buck1;
    struct regulator_init_data *buck2;
    struct regulator_init_data *buck3;
    struct regulator_init_data *ldo1;
    struct regulator_init_data *ldo2;
    struct regulator_init_data *ldo3;
    struct regulator_init_data *ldo4;
    struct regulator_init_data *ldo5;
    struct regulator_init_data *ldo6;
    struct regulator_init_data *ldo7;
    struct regulator_init_data *ldo8;
    struct regulator_init_data *ldo9;
    struct regulator_init_data *ldo10;
    struct regulator_init_data *ldo12;
    struct regulator_init_data *ldo_vibrator;
    struct regulator_init_data *ldo14;
    struct charger_desc *chg_desc;
    int companion_addr;
    int i2c_port;
    int irq_mode;
    int irq_base;
    int num_leds;
    int num_backlights;
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
struct pm860x_platform_data {
    struct pm860x_backlight_pdata *backlight;
    struct pm860x_led_pdata *led;
    struct pm860x_rtc_pdata *rtc;
    struct pm860x_touch_pdata *touch;
    struct pm860x_power_pdata *power;
    struct regulator_init_data *buck1;
    struct regulator_init_data *buck2;
    struct regulator_init_data *buck3;
    struct regulator_init_data *ldo1;
    struct regulator_init_data *ldo2;
    struct regulator_init_data *ldo3;
    struct regulator_init_data *ldo4;
    struct regulator_init_data *ldo5;
    struct regulator_init_data *ldo6;
    struct regulator_init_data *ldo7;
    struct regulator_init_data *ldo8;
    struct regulator_init_data *ldo9;
    struct regulator_init_data *ldo10;
    struct regulator_init_data *ldo12;
    struct regulator_init_data *ldo_vibrator;
    struct regulator_init_data *ldo14;
    struct charger_desc *chg_desc;
    int companion_addr;
    int i2c_port;
    int irq_mode;
    int irq_base;
    int num_leds;
    int num_backlights;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct pm860x_platform_data {
    struct pm860x_backlight_pdata *backlight;
    struct pm860x_led_pdata *led;
    struct pm860x_rtc_pdata *rtc;
    struct pm860x_touch_pdata *touch;
    struct pm860x_power_pdata *power;
    struct regulator_init_data *buck1;
    struct regulator_init_data *buck2;
    struct regulator_init_data *buck3;
    struct regulator_init_data *ldo1;
    struct regulator_init_data *ldo2;
    struct regulator_init_data *ldo3;
    struct regulator_init_data *ldo4;
    struct regulator_init_data *ldo5;
    struct regulator_init_data *ldo6;
    struct regulator_init_data *ldo7;
    struct regulator_init_data *ldo8;
    struct regulator_init_data *ldo9;
    struct regulator_init_data *ldo10;
    struct regulator_init_data *ldo12;
    struct regulator_init_data *ldo_vibrator;
    struct regulator_init_data *ldo14;
    struct charger_desc *chg_desc;
    int companion_addr;
    int i2c_port;
    int irq_mode;
    int irq_base;
    int num_leds;
    int num_backlights;
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
