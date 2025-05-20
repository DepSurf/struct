# Struct: <code>omap_dm_timer_ops</code>

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
struct omap_dm_timer_ops {
    struct omap_dm_timer * (*request_by_node)(struct device_node *);
    struct omap_dm_timer * (*request_specific)(int);
    struct omap_dm_timer * (*request)();
    int (*free)(struct omap_dm_timer *);
    void (*enable)(struct omap_dm_timer *);
    void (*disable)(struct omap_dm_timer *);
    int (*get_irq)(struct omap_dm_timer *);
    int (*set_int_enable)(struct omap_dm_timer *, unsigned int);
    int (*set_int_disable)(struct omap_dm_timer *, u32);
    struct clk * (*get_fclk)(struct omap_dm_timer *);
    int (*start)(struct omap_dm_timer *);
    int (*stop)(struct omap_dm_timer *);
    int (*set_source)(struct omap_dm_timer *, int);
    int (*set_load)(struct omap_dm_timer *, int, unsigned int);
    int (*set_match)(struct omap_dm_timer *, int, unsigned int);
    int (*set_pwm)(struct omap_dm_timer *, int, int, int);
    int (*set_prescaler)(struct omap_dm_timer *, int);
    unsigned int (*read_counter)(struct omap_dm_timer *);
    int (*write_counter)(struct omap_dm_timer *, unsigned int);
    unsigned int (*read_status)(struct omap_dm_timer *);
    int (*write_status)(struct omap_dm_timer *, unsigned int);
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
