# Struct: <code>acpi_gpio_info</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct acpi_gpio_info {
    bool gpioint;
    bool active_low;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct acpi_gpio_info {
    bool gpioint;
    int polarity;
    int triggering;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct acpi_gpio_info {
    bool gpioint;
    int polarity;
    int triggering;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct acpi_gpio_info {
    enum gpiod_flags flags;
    bool gpioint;
    int polarity;
    int triggering;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct acpi_gpio_info {
    enum gpiod_flags flags;
    bool gpioint;
    int polarity;
    int triggering;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct acpi_gpio_info {
    struct acpi_device *adev;
    enum gpiod_flags flags;
    bool gpioint;
    int polarity;
    int triggering;
    unsigned int quirks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct acpi_gpio_info {
    struct acpi_device *adev;
    enum gpiod_flags flags;
    bool gpioint;
    int polarity;
    int triggering;
    unsigned int quirks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct acpi_gpio_info {
    struct acpi_device *adev;
    enum gpiod_flags flags;
    bool gpioint;
    int pin_config;
    int polarity;
    int triggering;
    unsigned int quirks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct acpi_gpio_info {
    struct acpi_device *adev;
    enum gpiod_flags flags;
    bool gpioint;
    int pin_config;
    int polarity;
    int triggering;
    unsigned int quirks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct acpi_gpio_info {
    struct acpi_device *adev;
    enum gpiod_flags flags;
    bool gpioint;
    int pin_config;
    int polarity;
    int triggering;
    unsigned int quirks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct acpi_gpio_info {
    struct acpi_device *adev;
    enum gpiod_flags flags;
    bool gpioint;
    int pin_config;
    int polarity;
    int triggering;
    unsigned int debounce;
    unsigned int quirks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct acpi_gpio_info {
    struct acpi_device *adev;
    enum gpiod_flags flags;
    bool gpioint;
    int pin_config;
    int polarity;
    int triggering;
    unsigned int debounce;
    unsigned int quirks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct acpi_gpio_info {
    struct acpi_device *adev;
    enum gpiod_flags flags;
    bool gpioint;
    int pin_config;
    int polarity;
    int triggering;
    unsigned int debounce;
    unsigned int quirks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct acpi_gpio_info {
    struct acpi_device *adev;
    enum gpiod_flags flags;
    bool gpioint;
    int pin_config;
    int polarity;
    int triggering;
    unsigned int debounce;
    unsigned int quirks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct acpi_gpio_info {
    struct acpi_device *adev;
    enum gpiod_flags flags;
    bool gpioint;
    int pin_config;
    int polarity;
    int triggering;
    bool wake_capable;
    unsigned int debounce;
    unsigned int quirks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct acpi_gpio_info {
    struct acpi_device *adev;
    enum gpiod_flags flags;
    bool gpioint;
    int pin_config;
    int polarity;
    int triggering;
    bool wake_capable;
    unsigned int debounce;
    unsigned int quirks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct acpi_gpio_info {
    struct acpi_device *adev;
    enum gpiod_flags flags;
    bool gpioint;
    int pin_config;
    int polarity;
    int triggering;
    bool wake_capable;
    unsigned int debounce;
    unsigned int quirks;
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
struct acpi_gpio_info {
    struct acpi_device *adev;
    enum gpiod_flags flags;
    bool gpioint;
    int pin_config;
    int polarity;
    int triggering;
    unsigned int quirks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct acpi_gpio_info {
    struct acpi_device *adev;
    enum gpiod_flags flags;
    bool gpioint;
    int pin_config;
    int polarity;
    int triggering;
    unsigned int quirks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct acpi_gpio_info {
    struct acpi_device *adev;
    enum gpiod_flags flags;
    bool gpioint;
    int pin_config;
    int polarity;
    int triggering;
    unsigned int quirks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct acpi_gpio_info {
    struct acpi_device *adev;
    enum gpiod_flags flags;
    bool gpioint;
    int pin_config;
    int polarity;
    int triggering;
    unsigned int quirks;
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
struct acpi_gpio_info {
    struct acpi_device *adev;
    enum gpiod_flags flags;
    bool gpioint;
    int pin_config;
    int polarity;
    int triggering;
    unsigned int quirks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct acpi_gpio_info {
    struct acpi_device *adev;
    enum gpiod_flags flags;
    bool gpioint;
    int pin_config;
    int polarity;
    int triggering;
    unsigned int quirks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct acpi_gpio_info {
    struct acpi_device *adev;
    enum gpiod_flags flags;
    bool gpioint;
    int pin_config;
    int polarity;
    int triggering;
    unsigned int quirks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct acpi_gpio_info {
    struct acpi_device *adev;
    enum gpiod_flags flags;
    bool gpioint;
    int pin_config;
    int polarity;
    int triggering;
    unsigned int quirks;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int polarity</code>
</li>
<li>
<b>Field added. </b>
<code>int triggering</code>
</li>
<li>
<b>Field removed. </b>
<code>bool active_low</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>enum gpiod_flags flags</code>
</li>
</ul>
</details>
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
<code>struct acpi_device *adev</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int quirks</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int pin_config</code>
</li>
</ul>
</details>
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
<code>unsigned int debounce</code>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool wake_capable</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct acpi_device *adev</code> ➡️ <code>struct acpi_device *adev</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct acpi_device *adev</code> ➡️ <code>struct acpi_device *adev</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct acpi_device *adev</code> ➡️ <code>struct acpi_device *adev</code>
</li>
</ul>
</details>
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
