# Struct: <code>stmpe</code>

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
struct stmpe {
    struct regulator *vcc;
    struct regulator *vio;
    struct mutex lock;
    struct mutex irq_lock;
    struct device *dev;
    struct irq_domain *domain;
    void *client;
    struct stmpe_client_info *ci;
    enum stmpe_partnum partnum;
    struct stmpe_variant_info *variant;
    const u8 *regs;
    int irq;
    int num_gpios;
    u8 ier[2];
    u8 oldier[2];
    struct stmpe_platform_data *pdata;
    u8 sample_time;
    u8 mod_12b;
    u8 ref_sel;
    u8 adc_freq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct stmpe {
    struct regulator *vcc;
    struct regulator *vio;
    struct mutex lock;
    struct mutex irq_lock;
    struct device *dev;
    struct irq_domain *domain;
    void *client;
    struct stmpe_client_info *ci;
    enum stmpe_partnum partnum;
    struct stmpe_variant_info *variant;
    const u8 *regs;
    int irq;
    int num_gpios;
    u8 ier[2];
    u8 oldier[2];
    struct stmpe_platform_data *pdata;
    u8 sample_time;
    u8 mod_12b;
    u8 ref_sel;
    u8 adc_freq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct stmpe {
    struct regulator *vcc;
    struct regulator *vio;
    struct mutex lock;
    struct mutex irq_lock;
    struct device *dev;
    struct irq_domain *domain;
    void *client;
    struct stmpe_client_info *ci;
    enum stmpe_partnum partnum;
    struct stmpe_variant_info *variant;
    const u8 *regs;
    int irq;
    int num_gpios;
    u8 ier[2];
    u8 oldier[2];
    struct stmpe_platform_data *pdata;
    u8 sample_time;
    u8 mod_12b;
    u8 ref_sel;
    u8 adc_freq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct stmpe {
    struct regulator *vcc;
    struct regulator *vio;
    struct mutex lock;
    struct mutex irq_lock;
    struct device *dev;
    struct irq_domain *domain;
    void *client;
    struct stmpe_client_info *ci;
    enum stmpe_partnum partnum;
    struct stmpe_variant_info *variant;
    const u8 *regs;
    int irq;
    int num_gpios;
    u8 ier[2];
    u8 oldier[2];
    struct stmpe_platform_data *pdata;
    u8 sample_time;
    u8 mod_12b;
    u8 ref_sel;
    u8 adc_freq;
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
