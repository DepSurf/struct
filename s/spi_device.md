# Struct: <code>spi_device</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct spi_device {
    struct device dev;
    struct spi_master *master;
    u32 max_speed_hz;
    u8 chip_select;
    u8 bits_per_word;
    u16 mode;
    int irq;
    void *controller_state;
    void *controller_data;
    char modalias[32];
    int cs_gpio;
    struct spi_statistics statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct spi_device {
    struct device dev;
    struct spi_master *master;
    u32 max_speed_hz;
    u8 chip_select;
    u8 bits_per_word;
    u16 mode;
    int irq;
    void *controller_state;
    void *controller_data;
    char modalias[32];
    int cs_gpio;
    struct spi_statistics statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct spi_device {
    struct device dev;
    struct spi_master *master;
    u32 max_speed_hz;
    u8 chip_select;
    u8 bits_per_word;
    u16 mode;
    int irq;
    void *controller_state;
    void *controller_data;
    char modalias[32];
    int cs_gpio;
    struct spi_statistics statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct spi_device {
    struct device dev;
    struct spi_controller *controller;
    struct spi_controller *master;
    u32 max_speed_hz;
    u8 chip_select;
    u8 bits_per_word;
    u16 mode;
    int irq;
    void *controller_state;
    void *controller_data;
    char modalias[32];
    int cs_gpio;
    struct spi_statistics statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct spi_device {
    struct device dev;
    struct spi_controller *controller;
    struct spi_controller *master;
    u32 max_speed_hz;
    u8 chip_select;
    u8 bits_per_word;
    u16 mode;
    int irq;
    void *controller_state;
    void *controller_data;
    char modalias[32];
    int cs_gpio;
    struct spi_statistics statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct spi_device {
    struct device dev;
    struct spi_controller *controller;
    struct spi_controller *master;
    u32 max_speed_hz;
    u8 chip_select;
    u8 bits_per_word;
    u16 mode;
    int irq;
    void *controller_state;
    void *controller_data;
    char modalias[32];
    int cs_gpio;
    struct spi_statistics statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct spi_device {
    struct device dev;
    struct spi_controller *controller;
    struct spi_controller *master;
    u32 max_speed_hz;
    u8 chip_select;
    u8 bits_per_word;
    u16 mode;
    int irq;
    void *controller_state;
    void *controller_data;
    char modalias[32];
    const char *driver_override;
    int cs_gpio;
    struct spi_statistics statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct spi_device {
    struct device dev;
    struct spi_controller *controller;
    struct spi_controller *master;
    u32 max_speed_hz;
    u8 chip_select;
    u8 bits_per_word;
    bool rt;
    u32 mode;
    int irq;
    void *controller_state;
    void *controller_data;
    char modalias[32];
    const char *driver_override;
    int cs_gpio;
    struct gpio_desc *cs_gpiod;
    uint8_t word_delay_usecs;
    struct spi_statistics statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct spi_device {
    struct device dev;
    struct spi_controller *controller;
    struct spi_controller *master;
    u32 max_speed_hz;
    u8 chip_select;
    u8 bits_per_word;
    bool rt;
    u32 mode;
    int irq;
    void *controller_state;
    void *controller_data;
    char modalias[32];
    const char *driver_override;
    int cs_gpio;
    struct gpio_desc *cs_gpiod;
    uint8_t word_delay_usecs;
    struct spi_statistics statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct spi_device {
    struct device dev;
    struct spi_controller *controller;
    struct spi_controller *master;
    u32 max_speed_hz;
    u8 chip_select;
    u8 bits_per_word;
    bool rt;
    u32 mode;
    int irq;
    void *controller_state;
    void *controller_data;
    char modalias[32];
    const char *driver_override;
    int cs_gpio;
    struct gpio_desc *cs_gpiod;
    struct spi_delay word_delay;
    struct spi_statistics statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct spi_device {
    struct device dev;
    struct spi_controller *controller;
    struct spi_controller *master;
    u32 max_speed_hz;
    u8 chip_select;
    u8 bits_per_word;
    bool rt;
    u32 mode;
    int irq;
    void *controller_state;
    void *controller_data;
    char modalias[32];
    const char *driver_override;
    int cs_gpio;
    struct gpio_desc *cs_gpiod;
    struct spi_delay word_delay;
    struct spi_statistics statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct spi_device {
    struct device dev;
    struct spi_controller *controller;
    struct spi_controller *master;
    u32 max_speed_hz;
    u8 chip_select;
    u8 bits_per_word;
    bool rt;
    u32 mode;
    int irq;
    void *controller_state;
    void *controller_data;
    char modalias[32];
    const char *driver_override;
    int cs_gpio;
    struct gpio_desc *cs_gpiod;
    struct spi_delay word_delay;
    struct spi_statistics statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct spi_device {
    struct device dev;
    struct spi_controller *controller;
    struct spi_controller *master;
    u32 max_speed_hz;
    u8 chip_select;
    u8 bits_per_word;
    bool rt;
    u32 mode;
    int irq;
    void *controller_state;
    void *controller_data;
    char modalias[32];
    const char *driver_override;
    int cs_gpio;
    struct gpio_desc *cs_gpiod;
    struct spi_delay word_delay;
    struct spi_delay cs_setup;
    struct spi_delay cs_hold;
    struct spi_delay cs_inactive;
    struct spi_statistics statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct spi_device {
    struct device dev;
    struct spi_controller *controller;
    struct spi_controller *master;
    u32 max_speed_hz;
    u8 chip_select;
    u8 bits_per_word;
    bool rt;
    u32 mode;
    int irq;
    void *controller_state;
    void *controller_data;
    char modalias[32];
    const char *driver_override;
    struct gpio_desc *cs_gpiod;
    struct spi_delay word_delay;
    struct spi_delay cs_setup;
    struct spi_delay cs_hold;
    struct spi_delay cs_inactive;
    struct spi_statistics statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct spi_device {
    struct device dev;
    struct spi_controller *controller;
    struct spi_controller *master;
    u32 max_speed_hz;
    u8 chip_select;
    u8 bits_per_word;
    bool rt;
    u32 mode;
    int irq;
    void *controller_state;
    void *controller_data;
    char modalias[32];
    const char *driver_override;
    struct gpio_desc *cs_gpiod;
    struct spi_delay word_delay;
    struct spi_delay cs_setup;
    struct spi_delay cs_hold;
    struct spi_delay cs_inactive;
    struct spi_statistics *pcpu_statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct spi_device {
    struct device dev;
    struct spi_controller *controller;
    struct spi_controller *master;
    u32 max_speed_hz;
    u8 chip_select;
    u8 bits_per_word;
    bool rt;
    u32 mode;
    int irq;
    void *controller_state;
    void *controller_data;
    char modalias[32];
    const char *driver_override;
    struct gpio_desc *cs_gpiod;
    struct spi_delay word_delay;
    struct spi_delay cs_setup;
    struct spi_delay cs_hold;
    struct spi_delay cs_inactive;
    struct spi_statistics *pcpu_statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct spi_device {
    struct device dev;
    struct spi_controller *controller;
    struct spi_controller *master;
    u32 max_speed_hz;
    u8 chip_select[16];
    u8 bits_per_word;
    bool rt;
    u32 mode;
    int irq;
    void *controller_state;
    void *controller_data;
    char modalias[32];
    const char *driver_override;
    struct gpio_desc * cs_gpiod[16];
    struct spi_delay word_delay;
    struct spi_delay cs_setup;
    struct spi_delay cs_hold;
    struct spi_delay cs_inactive;
    struct spi_statistics *pcpu_statistics;
    u32 cs_index_mask;
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
struct spi_device {
    struct device dev;
    struct spi_controller *controller;
    struct spi_controller *master;
    u32 max_speed_hz;
    u8 chip_select;
    u8 bits_per_word;
    bool rt;
    u32 mode;
    int irq;
    void *controller_state;
    void *controller_data;
    char modalias[32];
    const char *driver_override;
    int cs_gpio;
    struct gpio_desc *cs_gpiod;
    uint8_t word_delay_usecs;
    struct spi_statistics statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct spi_device {
    struct device dev;
    struct spi_controller *controller;
    struct spi_controller *master;
    u32 max_speed_hz;
    u8 chip_select;
    u8 bits_per_word;
    bool rt;
    u32 mode;
    int irq;
    void *controller_state;
    void *controller_data;
    char modalias[32];
    const char *driver_override;
    int cs_gpio;
    struct gpio_desc *cs_gpiod;
    uint8_t word_delay_usecs;
    struct spi_statistics statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct spi_device {
    struct device dev;
    struct spi_controller *controller;
    struct spi_controller *master;
    u32 max_speed_hz;
    u8 chip_select;
    u8 bits_per_word;
    bool rt;
    u32 mode;
    int irq;
    void *controller_state;
    void *controller_data;
    char modalias[32];
    const char *driver_override;
    int cs_gpio;
    struct gpio_desc *cs_gpiod;
    uint8_t word_delay_usecs;
    struct spi_statistics statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct spi_device {
    struct device dev;
    struct spi_controller *controller;
    struct spi_controller *master;
    u32 max_speed_hz;
    u8 chip_select;
    u8 bits_per_word;
    bool rt;
    u32 mode;
    int irq;
    void *controller_state;
    void *controller_data;
    char modalias[32];
    const char *driver_override;
    int cs_gpio;
    struct gpio_desc *cs_gpiod;
    uint8_t word_delay_usecs;
    struct spi_statistics statistics;
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
struct spi_device {
    struct device dev;
    struct spi_controller *controller;
    struct spi_controller *master;
    u32 max_speed_hz;
    u8 chip_select;
    u8 bits_per_word;
    bool rt;
    u32 mode;
    int irq;
    void *controller_state;
    void *controller_data;
    char modalias[32];
    const char *driver_override;
    int cs_gpio;
    struct gpio_desc *cs_gpiod;
    uint8_t word_delay_usecs;
    struct spi_statistics statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct spi_device {
    struct device dev;
    struct spi_controller *controller;
    struct spi_controller *master;
    u32 max_speed_hz;
    u8 chip_select;
    u8 bits_per_word;
    bool rt;
    u32 mode;
    int irq;
    void *controller_state;
    void *controller_data;
    char modalias[32];
    const char *driver_override;
    int cs_gpio;
    struct gpio_desc *cs_gpiod;
    uint8_t word_delay_usecs;
    struct spi_statistics statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct spi_device {
    struct device dev;
    struct spi_controller *controller;
    struct spi_controller *master;
    u32 max_speed_hz;
    u8 chip_select;
    u8 bits_per_word;
    bool rt;
    u32 mode;
    int irq;
    void *controller_state;
    void *controller_data;
    char modalias[32];
    const char *driver_override;
    int cs_gpio;
    struct gpio_desc *cs_gpiod;
    uint8_t word_delay_usecs;
    struct spi_statistics statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct spi_device {
    struct device dev;
    struct spi_controller *controller;
    struct spi_controller *master;
    u32 max_speed_hz;
    u8 chip_select;
    u8 bits_per_word;
    bool rt;
    u32 mode;
    int irq;
    void *controller_state;
    void *controller_data;
    char modalias[32];
    const char *driver_override;
    int cs_gpio;
    struct gpio_desc *cs_gpiod;
    uint8_t word_delay_usecs;
    struct spi_statistics statistics;
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
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct spi_controller *controller</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct spi_master *master</code> ➡️ <code>struct spi_controller *master</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const char *driver_override</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool rt</code>
</li>
<li>
<b>Field added. </b>
<code>struct gpio_desc *cs_gpiod</code>
</li>
<li>
<b>Field added. </b>
<code>uint8_t word_delay_usecs</code>
</li>
<li>
<b>Field type changed. </b>
<code>u16 mode</code> ➡️ <code>u32 mode</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct spi_delay word_delay</code>
</li>
<li>
<b>Field removed. </b>
<code>uint8_t word_delay_usecs</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct spi_delay cs_setup</code>
</li>
<li>
<b>Field added. </b>
<code>struct spi_delay cs_hold</code>
</li>
<li>
<b>Field added. </b>
<code>struct spi_delay cs_inactive</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int cs_gpio</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct spi_statistics *pcpu_statistics</code>
</li>
<li>
<b>Field removed. </b>
<code>struct spi_statistics statistics</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 cs_index_mask</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 chip_select</code> ➡️ <code>u8 chip_select[16]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct gpio_desc *cs_gpiod</code> ➡️ <code>struct gpio_desc * cs_gpiod[16]</code>
</li>
</ul>
</details>
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
