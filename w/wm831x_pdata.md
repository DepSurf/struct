# Struct: <code>wm831x_pdata</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct wm831x_pdata {
    int wm831x_num;
    int (*pre_init)(struct wm831x *);
    int (*post_init)(struct wm831x *);
    bool irq_cmos;
    bool disable_touch;
    bool soft_shutdown;
    int irq_base;
    int gpio_base;
    int gpio_defaults[16];
    struct wm831x_backlight_pdata *backlight;
    struct wm831x_backup_pdata *backup;
    struct wm831x_battery_pdata *battery;
    struct wm831x_touch_pdata *touch;
    struct wm831x_watchdog_pdata *watchdog;
    struct wm831x_status_pdata * status[2];
    struct regulator_init_data * dcdc[4];
    struct regulator_init_data * epe[2];
    struct regulator_init_data * ldo[11];
    struct regulator_init_data * isink[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct wm831x_pdata {
    int wm831x_num;
    int (*pre_init)(struct wm831x *);
    int (*post_init)(struct wm831x *);
    bool irq_cmos;
    bool disable_touch;
    bool soft_shutdown;
    int irq_base;
    int gpio_base;
    int gpio_defaults[16];
    struct wm831x_backlight_pdata *backlight;
    struct wm831x_backup_pdata *backup;
    struct wm831x_battery_pdata *battery;
    struct wm831x_touch_pdata *touch;
    struct wm831x_watchdog_pdata *watchdog;
    struct wm831x_status_pdata * status[2];
    struct regulator_init_data * dcdc[4];
    struct regulator_init_data * epe[2];
    struct regulator_init_data * ldo[11];
    struct regulator_init_data * isink[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct wm831x_pdata {
    int wm831x_num;
    int (*pre_init)(struct wm831x *);
    int (*post_init)(struct wm831x *);
    bool irq_cmos;
    bool disable_touch;
    bool soft_shutdown;
    int irq_base;
    int gpio_base;
    int gpio_defaults[16];
    struct wm831x_backlight_pdata *backlight;
    struct wm831x_backup_pdata *backup;
    struct wm831x_battery_pdata *battery;
    struct wm831x_touch_pdata *touch;
    struct wm831x_watchdog_pdata *watchdog;
    struct wm831x_status_pdata * status[2];
    struct regulator_init_data * dcdc[4];
    struct regulator_init_data * epe[2];
    struct regulator_init_data * ldo[11];
    struct regulator_init_data * isink[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct wm831x_pdata {
    int wm831x_num;
    int (*pre_init)(struct wm831x *);
    int (*post_init)(struct wm831x *);
    bool irq_cmos;
    bool disable_touch;
    bool soft_shutdown;
    int irq_base;
    int gpio_base;
    int gpio_defaults[16];
    struct wm831x_backlight_pdata *backlight;
    struct wm831x_backup_pdata *backup;
    struct wm831x_battery_pdata *battery;
    struct wm831x_touch_pdata *touch;
    struct wm831x_watchdog_pdata *watchdog;
    struct wm831x_status_pdata * status[2];
    struct regulator_init_data * dcdc[4];
    struct regulator_init_data * epe[2];
    struct regulator_init_data * ldo[11];
    struct regulator_init_data * isink[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct wm831x_pdata {
    int wm831x_num;
    int (*pre_init)(struct wm831x *);
    int (*post_init)(struct wm831x *);
    bool irq_cmos;
    bool disable_touch;
    bool soft_shutdown;
    int irq_base;
    int gpio_base;
    int gpio_defaults[16];
    struct wm831x_backlight_pdata *backlight;
    struct wm831x_backup_pdata *backup;
    struct wm831x_battery_pdata *battery;
    struct wm831x_touch_pdata *touch;
    struct wm831x_watchdog_pdata *watchdog;
    struct wm831x_status_pdata * status[2];
    struct regulator_init_data * dcdc[4];
    struct regulator_init_data * epe[2];
    struct regulator_init_data * ldo[11];
    struct regulator_init_data * isink[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct wm831x_pdata {
    int wm831x_num;
    int (*pre_init)(struct wm831x *);
    int (*post_init)(struct wm831x *);
    bool irq_cmos;
    bool disable_touch;
    bool soft_shutdown;
    int irq_base;
    int gpio_base;
    int gpio_defaults[16];
    struct wm831x_backlight_pdata *backlight;
    struct wm831x_backup_pdata *backup;
    struct wm831x_battery_pdata *battery;
    struct wm831x_touch_pdata *touch;
    struct wm831x_watchdog_pdata *watchdog;
    struct wm831x_status_pdata * status[2];
    struct regulator_init_data * dcdc[4];
    struct regulator_init_data * epe[2];
    struct regulator_init_data * ldo[11];
    struct regulator_init_data * isink[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct wm831x_pdata {
    int wm831x_num;
    int (*pre_init)(struct wm831x *);
    int (*post_init)(struct wm831x *);
    bool irq_cmos;
    bool disable_touch;
    bool soft_shutdown;
    int irq_base;
    int gpio_base;
    int gpio_defaults[16];
    struct wm831x_backlight_pdata *backlight;
    struct wm831x_backup_pdata *backup;
    struct wm831x_battery_pdata *battery;
    struct wm831x_touch_pdata *touch;
    struct wm831x_watchdog_pdata *watchdog;
    struct wm831x_status_pdata * status[2];
    struct regulator_init_data * dcdc[4];
    struct regulator_init_data * epe[2];
    struct regulator_init_data * ldo[11];
    struct regulator_init_data * isink[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct wm831x_pdata {
    int wm831x_num;
    int (*pre_init)(struct wm831x *);
    int (*post_init)(struct wm831x *);
    bool irq_cmos;
    bool disable_touch;
    bool soft_shutdown;
    int irq_base;
    int gpio_base;
    int gpio_defaults[16];
    struct wm831x_backlight_pdata *backlight;
    struct wm831x_backup_pdata *backup;
    struct wm831x_battery_pdata *battery;
    struct wm831x_touch_pdata *touch;
    struct wm831x_watchdog_pdata *watchdog;
    struct wm831x_status_pdata * status[2];
    struct regulator_init_data * dcdc[4];
    struct regulator_init_data * epe[2];
    struct regulator_init_data * ldo[11];
    struct regulator_init_data * isink[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct wm831x_pdata {
    int wm831x_num;
    int (*pre_init)(struct wm831x *);
    int (*post_init)(struct wm831x *);
    bool irq_cmos;
    bool disable_touch;
    bool soft_shutdown;
    int irq_base;
    int gpio_base;
    int gpio_defaults[16];
    struct wm831x_backlight_pdata *backlight;
    struct wm831x_backup_pdata *backup;
    struct wm831x_battery_pdata *battery;
    struct wm831x_touch_pdata *touch;
    struct wm831x_watchdog_pdata *watchdog;
    struct wm831x_status_pdata * status[2];
    struct regulator_init_data * dcdc[4];
    struct regulator_init_data * epe[2];
    struct regulator_init_data * ldo[11];
    struct regulator_init_data * isink[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct wm831x_pdata {
    int wm831x_num;
    int (*pre_init)(struct wm831x *);
    int (*post_init)(struct wm831x *);
    bool irq_cmos;
    bool disable_touch;
    bool soft_shutdown;
    int irq_base;
    int gpio_base;
    int gpio_defaults[16];
    struct wm831x_backlight_pdata *backlight;
    struct wm831x_backup_pdata *backup;
    struct wm831x_battery_pdata *battery;
    struct wm831x_touch_pdata *touch;
    struct wm831x_watchdog_pdata *watchdog;
    struct wm831x_status_pdata * status[2];
    struct regulator_init_data * dcdc[4];
    struct regulator_init_data * epe[2];
    struct regulator_init_data * ldo[11];
    struct regulator_init_data * isink[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct wm831x_pdata {
    int wm831x_num;
    int (*pre_init)(struct wm831x *);
    int (*post_init)(struct wm831x *);
    bool irq_cmos;
    bool disable_touch;
    bool soft_shutdown;
    int irq_base;
    int gpio_base;
    int gpio_defaults[16];
    struct wm831x_backlight_pdata *backlight;
    struct wm831x_backup_pdata *backup;
    struct wm831x_battery_pdata *battery;
    struct wm831x_touch_pdata *touch;
    struct wm831x_watchdog_pdata *watchdog;
    struct wm831x_status_pdata * status[2];
    struct regulator_init_data * dcdc[4];
    struct regulator_init_data * epe[2];
    struct regulator_init_data * ldo[11];
    struct regulator_init_data * isink[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct wm831x_pdata {
    int wm831x_num;
    int (*pre_init)(struct wm831x *);
    int (*post_init)(struct wm831x *);
    bool irq_cmos;
    bool disable_touch;
    bool soft_shutdown;
    int irq_base;
    int gpio_base;
    int gpio_defaults[16];
    struct wm831x_backlight_pdata *backlight;
    struct wm831x_backup_pdata *backup;
    struct wm831x_battery_pdata *battery;
    struct wm831x_touch_pdata *touch;
    struct wm831x_watchdog_pdata *watchdog;
    struct wm831x_status_pdata * status[2];
    struct regulator_init_data * dcdc[4];
    struct regulator_init_data * epe[2];
    struct regulator_init_data * ldo[11];
    struct regulator_init_data * isink[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct wm831x_pdata {
    int wm831x_num;
    int (*pre_init)(struct wm831x *);
    int (*post_init)(struct wm831x *);
    bool irq_cmos;
    bool disable_touch;
    bool soft_shutdown;
    int irq_base;
    int gpio_base;
    int gpio_defaults[16];
    struct wm831x_backlight_pdata *backlight;
    struct wm831x_backup_pdata *backup;
    struct wm831x_battery_pdata *battery;
    struct wm831x_touch_pdata *touch;
    struct wm831x_watchdog_pdata *watchdog;
    struct wm831x_status_pdata * status[2];
    struct regulator_init_data * dcdc[4];
    struct regulator_init_data * epe[2];
    struct regulator_init_data * ldo[11];
    struct regulator_init_data * isink[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct wm831x_pdata {
    int wm831x_num;
    int (*pre_init)(struct wm831x *);
    int (*post_init)(struct wm831x *);
    bool irq_cmos;
    bool disable_touch;
    bool soft_shutdown;
    int irq_base;
    int gpio_base;
    int gpio_defaults[16];
    struct wm831x_backlight_pdata *backlight;
    struct wm831x_backup_pdata *backup;
    struct wm831x_battery_pdata *battery;
    struct wm831x_touch_pdata *touch;
    struct wm831x_watchdog_pdata *watchdog;
    struct wm831x_status_pdata * status[2];
    struct regulator_init_data * dcdc[4];
    struct regulator_init_data * epe[2];
    struct regulator_init_data * ldo[11];
    struct regulator_init_data * isink[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct wm831x_pdata {
    int wm831x_num;
    int (*pre_init)(struct wm831x *);
    int (*post_init)(struct wm831x *);
    bool irq_cmos;
    bool disable_touch;
    bool soft_shutdown;
    int irq_base;
    int gpio_base;
    int gpio_defaults[16];
    struct wm831x_backlight_pdata *backlight;
    struct wm831x_backup_pdata *backup;
    struct wm831x_battery_pdata *battery;
    struct wm831x_touch_pdata *touch;
    struct wm831x_watchdog_pdata *watchdog;
    struct wm831x_status_pdata * status[2];
    struct regulator_init_data * dcdc[4];
    struct regulator_init_data * epe[2];
    struct regulator_init_data * ldo[11];
    struct regulator_init_data * isink[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct wm831x_pdata {
    int wm831x_num;
    int (*pre_init)(struct wm831x *);
    int (*post_init)(struct wm831x *);
    bool irq_cmos;
    bool disable_touch;
    bool soft_shutdown;
    int irq_base;
    int gpio_base;
    int gpio_defaults[16];
    struct wm831x_backlight_pdata *backlight;
    struct wm831x_backup_pdata *backup;
    struct wm831x_battery_pdata *battery;
    struct wm831x_touch_pdata *touch;
    struct wm831x_watchdog_pdata *watchdog;
    struct wm831x_status_pdata * status[2];
    struct regulator_init_data * dcdc[4];
    struct regulator_init_data * epe[2];
    struct regulator_init_data * ldo[11];
    struct regulator_init_data * isink[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct wm831x_pdata {
    int wm831x_num;
    int (*pre_init)(struct wm831x *);
    int (*post_init)(struct wm831x *);
    bool irq_cmos;
    bool disable_touch;
    bool soft_shutdown;
    int irq_base;
    int gpio_base;
    int gpio_defaults[16];
    struct wm831x_backlight_pdata *backlight;
    struct wm831x_backup_pdata *backup;
    struct wm831x_battery_pdata *battery;
    struct wm831x_touch_pdata *touch;
    struct wm831x_watchdog_pdata *watchdog;
    struct wm831x_status_pdata * status[2];
    struct regulator_init_data * dcdc[4];
    struct regulator_init_data * epe[2];
    struct regulator_init_data * ldo[11];
    struct regulator_init_data * isink[2];
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
struct wm831x_pdata {
    int wm831x_num;
    int (*pre_init)(struct wm831x *);
    int (*post_init)(struct wm831x *);
    bool irq_cmos;
    bool disable_touch;
    bool soft_shutdown;
    int irq_base;
    int gpio_base;
    int gpio_defaults[16];
    struct wm831x_backlight_pdata *backlight;
    struct wm831x_backup_pdata *backup;
    struct wm831x_battery_pdata *battery;
    struct wm831x_touch_pdata *touch;
    struct wm831x_watchdog_pdata *watchdog;
    struct wm831x_status_pdata * status[2];
    struct regulator_init_data * dcdc[4];
    struct regulator_init_data * epe[2];
    struct regulator_init_data * ldo[11];
    struct regulator_init_data * isink[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct wm831x_pdata {
    int wm831x_num;
    int (*pre_init)(struct wm831x *);
    int (*post_init)(struct wm831x *);
    bool irq_cmos;
    bool disable_touch;
    bool soft_shutdown;
    int irq_base;
    int gpio_base;
    int gpio_defaults[16];
    struct wm831x_backlight_pdata *backlight;
    struct wm831x_backup_pdata *backup;
    struct wm831x_battery_pdata *battery;
    struct wm831x_touch_pdata *touch;
    struct wm831x_watchdog_pdata *watchdog;
    struct wm831x_status_pdata * status[2];
    struct regulator_init_data * dcdc[4];
    struct regulator_init_data * epe[2];
    struct regulator_init_data * ldo[11];
    struct regulator_init_data * isink[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct wm831x_pdata {
    int wm831x_num;
    int (*pre_init)(struct wm831x *);
    int (*post_init)(struct wm831x *);
    bool irq_cmos;
    bool disable_touch;
    bool soft_shutdown;
    int irq_base;
    int gpio_base;
    int gpio_defaults[16];
    struct wm831x_backlight_pdata *backlight;
    struct wm831x_backup_pdata *backup;
    struct wm831x_battery_pdata *battery;
    struct wm831x_touch_pdata *touch;
    struct wm831x_watchdog_pdata *watchdog;
    struct wm831x_status_pdata * status[2];
    struct regulator_init_data * dcdc[4];
    struct regulator_init_data * epe[2];
    struct regulator_init_data * ldo[11];
    struct regulator_init_data * isink[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct wm831x_pdata {
    int wm831x_num;
    int (*pre_init)(struct wm831x *);
    int (*post_init)(struct wm831x *);
    bool irq_cmos;
    bool disable_touch;
    bool soft_shutdown;
    int irq_base;
    int gpio_base;
    int gpio_defaults[16];
    struct wm831x_backlight_pdata *backlight;
    struct wm831x_backup_pdata *backup;
    struct wm831x_battery_pdata *battery;
    struct wm831x_touch_pdata *touch;
    struct wm831x_watchdog_pdata *watchdog;
    struct wm831x_status_pdata * status[2];
    struct regulator_init_data * dcdc[4];
    struct regulator_init_data * epe[2];
    struct regulator_init_data * ldo[11];
    struct regulator_init_data * isink[2];
};
```
</details>
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct wm831x_pdata {
    int wm831x_num;
    int (*pre_init)(struct wm831x *);
    int (*post_init)(struct wm831x *);
    bool irq_cmos;
    bool disable_touch;
    bool soft_shutdown;
    int irq_base;
    int gpio_base;
    int gpio_defaults[16];
    struct wm831x_backlight_pdata *backlight;
    struct wm831x_backup_pdata *backup;
    struct wm831x_battery_pdata *battery;
    struct wm831x_touch_pdata *touch;
    struct wm831x_watchdog_pdata *watchdog;
    struct wm831x_status_pdata * status[2];
    struct regulator_init_data * dcdc[4];
    struct regulator_init_data * epe[2];
    struct regulator_init_data * ldo[11];
    struct regulator_init_data * isink[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct wm831x_pdata {
    int wm831x_num;
    int (*pre_init)(struct wm831x *);
    int (*post_init)(struct wm831x *);
    bool irq_cmos;
    bool disable_touch;
    bool soft_shutdown;
    int irq_base;
    int gpio_base;
    int gpio_defaults[16];
    struct wm831x_backlight_pdata *backlight;
    struct wm831x_backup_pdata *backup;
    struct wm831x_battery_pdata *battery;
    struct wm831x_touch_pdata *touch;
    struct wm831x_watchdog_pdata *watchdog;
    struct wm831x_status_pdata * status[2];
    struct regulator_init_data * dcdc[4];
    struct regulator_init_data * epe[2];
    struct regulator_init_data * ldo[11];
    struct regulator_init_data * isink[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct wm831x_pdata {
    int wm831x_num;
    int (*pre_init)(struct wm831x *);
    int (*post_init)(struct wm831x *);
    bool irq_cmos;
    bool disable_touch;
    bool soft_shutdown;
    int irq_base;
    int gpio_base;
    int gpio_defaults[16];
    struct wm831x_backlight_pdata *backlight;
    struct wm831x_backup_pdata *backup;
    struct wm831x_battery_pdata *battery;
    struct wm831x_touch_pdata *touch;
    struct wm831x_watchdog_pdata *watchdog;
    struct wm831x_status_pdata * status[2];
    struct regulator_init_data * dcdc[4];
    struct regulator_init_data * epe[2];
    struct regulator_init_data * ldo[11];
    struct regulator_init_data * isink[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct wm831x_pdata {
    int wm831x_num;
    int (*pre_init)(struct wm831x *);
    int (*post_init)(struct wm831x *);
    bool irq_cmos;
    bool disable_touch;
    bool soft_shutdown;
    int irq_base;
    int gpio_base;
    int gpio_defaults[16];
    struct wm831x_backlight_pdata *backlight;
    struct wm831x_backup_pdata *backup;
    struct wm831x_battery_pdata *battery;
    struct wm831x_touch_pdata *touch;
    struct wm831x_watchdog_pdata *watchdog;
    struct wm831x_status_pdata * status[2];
    struct regulator_init_data * dcdc[4];
    struct regulator_init_data * epe[2];
    struct regulator_init_data * ldo[11];
    struct regulator_init_data * isink[2];
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
No changes between <code>generic</code> and <code>aws</code> ✅
</li>
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
