# Struct: <code>msm_pingroup</code>

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
struct msm_pingroup {
    const char *name;
    const unsigned int *pins;
    unsigned int npins;
    unsigned int *funcs;
    unsigned int nfuncs;
    u32 ctl_reg;
    u32 io_reg;
    u32 intr_cfg_reg;
    u32 intr_status_reg;
    u32 intr_target_reg;
    unsigned int tile;
    unsigned int mux_bit;
    unsigned int pull_bit;
    unsigned int drv_bit;
    unsigned int oe_bit;
    unsigned int in_bit;
    unsigned int out_bit;
    unsigned int intr_enable_bit;
    unsigned int intr_status_bit;
    unsigned int intr_ack_high;
    unsigned int intr_target_bit;
    unsigned int intr_target_kpss_val;
    unsigned int intr_raw_status_bit;
    unsigned int intr_polarity_bit;
    unsigned int intr_detection_bit;
    unsigned int intr_detection_width;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct msm_pingroup {
    const char *name;
    const unsigned int *pins;
    unsigned int npins;
    unsigned int *funcs;
    unsigned int nfuncs;
    u32 ctl_reg;
    u32 io_reg;
    u32 intr_cfg_reg;
    u32 intr_status_reg;
    u32 intr_target_reg;
    unsigned int tile;
    unsigned int mux_bit;
    unsigned int pull_bit;
    unsigned int drv_bit;
    unsigned int oe_bit;
    unsigned int in_bit;
    unsigned int out_bit;
    unsigned int intr_enable_bit;
    unsigned int intr_status_bit;
    unsigned int intr_ack_high;
    unsigned int intr_target_bit;
    unsigned int intr_target_kpss_val;
    unsigned int intr_raw_status_bit;
    unsigned int intr_polarity_bit;
    unsigned int intr_detection_bit;
    unsigned int intr_detection_width;
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
