# Struct: <code>omap_hwmod</code>

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
struct omap_hwmod {
    const char *name;
    struct omap_hwmod_class *class;
    struct omap_device *od;
    struct omap_hwmod_rst_info *rst_lines;
    union (anon) prcm;
    const char *main_clk;
    struct clk *_clk;
    struct omap_hwmod_opt_clk *opt_clks;
    const char *clkdm_name;
    struct clockdomain *clkdm;
    struct list_head slave_ports;
    void *dev_attr;
    u32 _sysc_cache;
    void *_mpu_rt_va;
    spinlock_t _lock;
    struct lock_class_key hwmod_key;
    struct list_head node;
    struct omap_hwmod_ocp_if *_mpu_port;
    u32 flags;
    u8 mpu_rt_idx;
    u8 response_lat;
    u8 rst_lines_cnt;
    u8 opt_clks_cnt;
    u8 slaves_cnt;
    u8 hwmods_cnt;
    u8 _int_flags;
    u8 _state;
    u8 _postsetup_state;
    struct omap_hwmod *parent_hwmod;
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
