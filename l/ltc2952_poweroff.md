# Struct: <code>ltc2952_poweroff</code>

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
struct ltc2952_poweroff {
    struct hrtimer timer_trigger;
    struct hrtimer timer_wde;
    ktime_t trigger_delay;
    ktime_t wde_interval;
    struct device *dev;
    struct gpio_desc *gpio_trigger;
    struct gpio_desc *gpio_watchdog;
    struct gpio_desc *gpio_kill;
    bool kernel_panic;
    struct notifier_block panic_notifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ltc2952_poweroff {
    struct hrtimer timer_trigger;
    struct hrtimer timer_wde;
    ktime_t trigger_delay;
    ktime_t wde_interval;
    struct device *dev;
    struct gpio_desc *gpio_trigger;
    struct gpio_desc *gpio_watchdog;
    struct gpio_desc *gpio_kill;
    bool kernel_panic;
    struct notifier_block panic_notifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ltc2952_poweroff {
    struct hrtimer timer_trigger;
    struct hrtimer timer_wde;
    ktime_t trigger_delay;
    ktime_t wde_interval;
    struct device *dev;
    struct gpio_desc *gpio_trigger;
    struct gpio_desc *gpio_watchdog;
    struct gpio_desc *gpio_kill;
    bool kernel_panic;
    struct notifier_block panic_notifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ltc2952_poweroff {
    struct hrtimer timer_trigger;
    struct hrtimer timer_wde;
    ktime_t trigger_delay;
    ktime_t wde_interval;
    struct device *dev;
    struct gpio_desc *gpio_trigger;
    struct gpio_desc *gpio_watchdog;
    struct gpio_desc *gpio_kill;
    bool kernel_panic;
    struct notifier_block panic_notifier;
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
