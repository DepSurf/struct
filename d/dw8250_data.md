# Struct: <code>dw8250_data</code>

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
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dw8250_data {
    struct dw8250_port_data data;
    const struct dw8250_platform_data *pdata;
    int msr_mask_on;
    int msr_mask_off;
    struct clk *clk;
    struct clk *pclk;
    struct notifier_block clk_notifier;
    struct work_struct clk_work;
    struct reset_control *rst;
    unsigned int skip_autocfg;
    unsigned int uart_16550_compatible;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dw8250_data {
    struct dw8250_port_data data;
    const struct dw8250_platform_data *pdata;
    int msr_mask_on;
    int msr_mask_off;
    struct clk *clk;
    struct clk *pclk;
    struct notifier_block clk_notifier;
    struct work_struct clk_work;
    struct reset_control *rst;
    unsigned int skip_autocfg;
    unsigned int uart_16550_compatible;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dw8250_data {
    struct dw8250_port_data data;
    const struct dw8250_platform_data *pdata;
    int msr_mask_on;
    int msr_mask_off;
    struct clk *clk;
    struct clk *pclk;
    struct notifier_block clk_notifier;
    struct work_struct clk_work;
    struct reset_control *rst;
    unsigned int skip_autocfg;
    unsigned int uart_16550_compatible;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dw8250_data {
    struct dw8250_port_data data;
    const struct dw8250_platform_data *pdata;
    int msr_mask_on;
    int msr_mask_off;
    struct clk *clk;
    struct clk *pclk;
    struct notifier_block clk_notifier;
    struct work_struct clk_work;
    struct reset_control *rst;
    unsigned int skip_autocfg;
    unsigned int uart_16550_compatible;
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
struct dw8250_data {
    struct dw8250_port_data data;
    u8 usr_reg;
    int msr_mask_on;
    int msr_mask_off;
    struct clk *clk;
    struct clk *pclk;
    struct reset_control *rst;
    unsigned int skip_autocfg;
    unsigned int uart_16550_compatible;
};
```
</details>
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
<b>Regular</b>
<ul>
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
</ul>
