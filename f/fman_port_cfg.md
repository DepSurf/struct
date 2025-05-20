# Struct: <code>fman_port_cfg</code>

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
struct fman_port_cfg {
    u32 dflt_fqid;
    u32 err_fqid;
    u32 pcd_base_fqid;
    u32 pcd_fqs_count;
    u8 deq_sp;
    bool deq_high_priority;
    enum fman_port_deq_type deq_type;
    enum fman_port_deq_prefetch deq_prefetch_option;
    u16 deq_byte_cnt;
    u8 cheksum_last_bytes_ignore;
    u8 rx_cut_end_bytes;
    struct fman_buf_pool_depletion buf_pool_depletion;
    struct fman_ext_pools ext_buf_pools;
    u32 tx_fifo_min_level;
    u32 tx_fifo_low_comf_level;
    u32 rx_pri_elevation;
    u32 rx_fifo_thr;
    struct fman_sp_buf_margins buf_margins;
    u32 int_buf_start_margin;
    struct fman_sp_int_context_data_copy int_context;
    u32 discard_mask;
    u32 err_mask;
    struct fman_buffer_prefix_content buffer_prefix_content;
    bool dont_release_buf;
    u8 rx_fd_bits;
    u32 tx_fifo_deq_pipeline_depth;
    bool errata_A006320;
    bool excessive_threshold_register;
    bool fmbm_tfne_has_features;
    enum fman_port_dma_swap dma_swap_data;
    enum fman_port_color color;
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
