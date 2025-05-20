# Struct: <code>fman_port</code>

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
struct fman_port {
    void *fm;
    struct device *dev;
    struct fman_rev_info rev_info;
    u8 port_id;
    enum fman_port_type port_type;
    u16 port_speed;
    union fman_port_bmi_regs *bmi_regs;
    struct fman_port_qmi_regs *qmi_regs;
    struct fman_port_hwp_regs *hwp_regs;
    struct fman_sp_buffer_offsets buffer_offsets;
    u8 internal_buf_offset;
    struct fman_ext_pools ext_buf_pools;
    u16 max_frame_length;
    struct fman_port_rsrc open_dmas;
    struct fman_port_rsrc tasks;
    struct fman_port_rsrc fifo_bufs;
    struct fman_port_rx_pools_params rx_pools_params;
    struct fman_port_cfg *cfg;
    struct fman_port_dts_params dts_params;
    u8 ext_pools_num;
    u32 max_port_fifo_size;
    u32 max_num_of_ext_pools;
    u32 max_num_of_sub_portals;
    u32 bm_max_num_of_pools;
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
