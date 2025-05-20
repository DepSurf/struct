# Struct: <code>fman_cfg</code>

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
struct fman_cfg {
    u8 disp_limit_tsh;
    u8 prs_disp_tsh;
    u8 plcr_disp_tsh;
    u8 kg_disp_tsh;
    u8 bmi_disp_tsh;
    u8 qmi_enq_disp_tsh;
    u8 qmi_deq_disp_tsh;
    u8 fm_ctl1_disp_tsh;
    u8 fm_ctl2_disp_tsh;
    int dma_cache_override;
    enum fman_dma_aid_mode dma_aid_mode;
    u32 dma_axi_dbg_num_of_beats;
    u32 dma_cam_num_of_entries;
    u32 dma_watchdog;
    u8 dma_comm_qtsh_asrt_emer;
    u32 dma_write_buf_tsh_asrt_emer;
    u32 dma_read_buf_tsh_asrt_emer;
    u8 dma_comm_qtsh_clr_emer;
    u32 dma_write_buf_tsh_clr_emer;
    u32 dma_read_buf_tsh_clr_emer;
    u32 dma_sos_emergency;
    int dma_dbg_cnt_mode;
    int catastrophic_err;
    int dma_err;
    u32 exceptions;
    u16 clk_freq;
    u32 cam_base_addr;
    u32 fifo_base_addr;
    u32 total_fifo_size;
    u32 total_num_of_tasks;
    u32 qmi_def_tnums_thresh;
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
