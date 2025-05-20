# Struct: <code>gpmc_device_timings</code>

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
struct gpmc_device_timings {
    u32 t_ceasu;
    u32 t_avdasu;
    u32 t_avdp_r;
    u32 t_avdp_w;
    u32 t_aavdh;
    u32 t_oeasu;
    u32 t_aa;
    u32 t_iaa;
    u32 t_oe;
    u32 t_ce;
    u32 t_rd_cycle;
    u32 t_cez_r;
    u32 t_cez_w;
    u32 t_oez;
    u32 t_weasu;
    u32 t_wpl;
    u32 t_wph;
    u32 t_wr_cycle;
    u32 clk;
    u32 t_bacc;
    u32 t_ces;
    u32 t_avds;
    u32 t_avdh;
    u32 t_ach;
    u32 t_rdyo;
    u32 t_ce_rdyz;
    u32 t_ce_avd;
    u8 cyc_aavdh_oe;
    u8 cyc_aavdh_we;
    u8 cyc_oe;
    u8 cyc_wpl;
    u32 cyc_iaa;
    bool ce_xdelay;
    bool avd_xdelay;
    bool oe_xdelay;
    bool we_xdelay;
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
