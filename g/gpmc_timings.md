# Struct: <code>gpmc_timings</code>

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
struct gpmc_timings {
    u32 sync_clk;
    u32 cs_on;
    u32 cs_rd_off;
    u32 cs_wr_off;
    u32 adv_on;
    u32 adv_rd_off;
    u32 adv_wr_off;
    u32 adv_aad_mux_on;
    u32 adv_aad_mux_rd_off;
    u32 adv_aad_mux_wr_off;
    u32 we_on;
    u32 we_off;
    u32 oe_on;
    u32 oe_off;
    u32 oe_aad_mux_on;
    u32 oe_aad_mux_off;
    u32 page_burst_access;
    u32 access;
    u32 rd_cycle;
    u32 wr_cycle;
    u32 bus_turnaround;
    u32 cycle2cycle_delay;
    u32 wait_monitoring;
    u32 clk_activation;
    u32 wr_access;
    u32 wr_data_mux_bus;
    struct gpmc_bool_timings bool_timings;
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
