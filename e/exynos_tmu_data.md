# Struct: <code>exynos_tmu_data</code>

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
In <code>arm64</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct exynos_tmu_data {
    int id;
    void *base;
    void *base_second;
    int irq;
    enum soc_type soc;
    struct work_struct irq_work;
    struct mutex lock;
    struct clk *clk;
    struct clk *clk_sec;
    struct clk *sclk;
    u32 cal_type;
    u32 efuse_value;
    u32 min_efuse_value;
    u32 max_efuse_value;
    u16 temp_error1;
    u16 temp_error2;
    u8 gain;
    u8 reference_voltage;
    struct regulator *regulator;
    struct thermal_zone_device *tzd;
    unsigned int ntrip;
    bool enabled;
    void (*tmu_set_trip_temp)(struct exynos_tmu_data *, int, u8);
    void (*tmu_set_trip_hyst)(struct exynos_tmu_data *, int, u8, u8);
    void (*tmu_initialize)(struct platform_device *);
    void (*tmu_control)(struct platform_device *, bool);
    int (*tmu_read)(struct exynos_tmu_data *);
    void (*tmu_set_emulation)(struct exynos_tmu_data *, int);
    void (*tmu_clear_irqs)(struct exynos_tmu_data *);
};
```
</details>
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
<b>Arch</b>
<ul>
</ul>
