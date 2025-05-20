# Struct: <code>fman_state_struct</code>

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
struct fman_state_struct {
    u8 fm_id;
    u16 fm_clk_freq;
    struct fman_rev_info rev_info;
    bool enabled_time_stamp;
    u8 count1_micro_bit;
    u8 total_num_of_tasks;
    u8 accumulated_num_of_tasks;
    u32 accumulated_fifo_size;
    u8 accumulated_num_of_open_dmas;
    u8 accumulated_num_of_deq_tnums;
    u32 exceptions;
    u32 extra_fifo_pool_size;
    u8 extra_tasks_pool_size;
    u8 extra_open_dmas_pool_size;
    u16 port_mfl[10];
    u16 mac_mfl[10];
    u32 fm_iram_size;
    u32 dma_thresh_max_commq;
    u32 dma_thresh_max_buf;
    u32 max_num_of_open_dmas;
    u32 qmi_max_num_of_tnums;
    u32 qmi_def_tnums_thresh;
    u32 bmi_max_num_of_tasks;
    u32 bmi_max_fifo_size;
    u32 fm_port_num_of_cg;
    u32 num_of_rx_ports;
    u32 total_fifo_size;
    u32 qman_channel_base;
    u32 num_of_qman_channels;
    struct resource *res;
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
<b>Arch</b>
<ul>
</ul>
