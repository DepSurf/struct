# Struct: <code>gic_chip_data</code>

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
struct gic_chip_data {
    struct irq_chip chip;
    union gic_base dist_base;
    union gic_base cpu_base;
    void *raw_dist_base;
    void *raw_cpu_base;
    u32 percpu_offset;
    u32 saved_spi_enable[32];
    u32 saved_spi_active[32];
    u32 saved_spi_conf[64];
    u32 saved_spi_target[255];
    u32 *saved_ppi_enable;
    u32 *saved_ppi_active;
    u32 *saved_ppi_conf;
    struct irq_domain *domain;
    unsigned int gic_irqs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct gic_chip_data {
    struct irq_chip chip;
    union gic_base dist_base;
    union gic_base cpu_base;
    void *raw_dist_base;
    void *raw_cpu_base;
    u32 percpu_offset;
    u32 saved_spi_enable[32];
    u32 saved_spi_active[32];
    u32 saved_spi_conf[64];
    u32 saved_spi_target[255];
    u32 *saved_ppi_enable;
    u32 *saved_ppi_active;
    u32 *saved_ppi_conf;
    struct irq_domain *domain;
    unsigned int gic_irqs;
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
