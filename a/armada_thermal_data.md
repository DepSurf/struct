# Struct: <code>armada_thermal_data</code>

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
struct armada_thermal_data {
    void (*init)(struct platform_device *, struct armada_thermal_priv *);
    s64 coef_b;
    s64 coef_m;
    u32 coef_div;
    bool inverted;
    bool signed_sample;
    unsigned int temp_shift;
    unsigned int temp_mask;
    unsigned int thresh_shift;
    unsigned int hyst_shift;
    unsigned int hyst_mask;
    u32 is_valid_bit;
    unsigned int syscon_control0_off;
    unsigned int syscon_control1_off;
    unsigned int syscon_status_off;
    unsigned int dfx_irq_cause_off;
    unsigned int dfx_irq_mask_off;
    unsigned int dfx_overheat_irq;
    unsigned int dfx_server_irq_mask_off;
    unsigned int dfx_server_irq_en;
    unsigned int cpu_nr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct armada_thermal_data {
    void (*init)(struct platform_device *, struct armada_thermal_priv *);
    s64 coef_b;
    s64 coef_m;
    u32 coef_div;
    bool inverted;
    bool signed_sample;
    unsigned int temp_shift;
    unsigned int temp_mask;
    unsigned int thresh_shift;
    unsigned int hyst_shift;
    unsigned int hyst_mask;
    u32 is_valid_bit;
    unsigned int syscon_control0_off;
    unsigned int syscon_control1_off;
    unsigned int syscon_status_off;
    unsigned int dfx_irq_cause_off;
    unsigned int dfx_irq_mask_off;
    unsigned int dfx_overheat_irq;
    unsigned int dfx_server_irq_mask_off;
    unsigned int dfx_server_irq_en;
    unsigned int cpu_nr;
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
