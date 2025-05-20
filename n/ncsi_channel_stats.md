# Struct: <code>ncsi_channel_stats</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ncsi_channel_stats {
    u32 hnc_cnt_hi;
    u32 hnc_cnt_lo;
    u32 hnc_rx_bytes;
    u32 hnc_tx_bytes;
    u32 hnc_rx_uc_pkts;
    u32 hnc_rx_mc_pkts;
    u32 hnc_rx_bc_pkts;
    u32 hnc_tx_uc_pkts;
    u32 hnc_tx_mc_pkts;
    u32 hnc_tx_bc_pkts;
    u32 hnc_fcs_err;
    u32 hnc_align_err;
    u32 hnc_false_carrier;
    u32 hnc_runt_pkts;
    u32 hnc_jabber_pkts;
    u32 hnc_rx_pause_xon;
    u32 hnc_rx_pause_xoff;
    u32 hnc_tx_pause_xon;
    u32 hnc_tx_pause_xoff;
    u32 hnc_tx_s_collision;
    u32 hnc_tx_m_collision;
    u32 hnc_l_collision;
    u32 hnc_e_collision;
    u32 hnc_rx_ctl_frames;
    u32 hnc_rx_64_frames;
    u32 hnc_rx_127_frames;
    u32 hnc_rx_255_frames;
    u32 hnc_rx_511_frames;
    u32 hnc_rx_1023_frames;
    u32 hnc_rx_1522_frames;
    u32 hnc_rx_9022_frames;
    u32 hnc_tx_64_frames;
    u32 hnc_tx_127_frames;
    u32 hnc_tx_255_frames;
    u32 hnc_tx_511_frames;
    u32 hnc_tx_1023_frames;
    u32 hnc_tx_1522_frames;
    u32 hnc_tx_9022_frames;
    u32 hnc_rx_valid_bytes;
    u32 hnc_rx_runt_pkts;
    u32 hnc_rx_jabber_pkts;
    u32 ncsi_rx_cmds;
    u32 ncsi_dropped_cmds;
    u32 ncsi_cmd_type_errs;
    u32 ncsi_cmd_csum_errs;
    u32 ncsi_rx_pkts;
    u32 ncsi_tx_pkts;
    u32 ncsi_tx_aen_pkts;
    u32 pt_tx_pkts;
    u32 pt_tx_dropped;
    u32 pt_tx_channel_err;
    u32 pt_tx_us_err;
    u32 pt_rx_pkts;
    u32 pt_rx_dropped;
    u32 pt_rx_channel_err;
    u32 pt_rx_us_err;
    u32 pt_rx_os_err;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ncsi_channel_stats {
    u32 hnc_cnt_hi;
    u32 hnc_cnt_lo;
    u32 hnc_rx_bytes;
    u32 hnc_tx_bytes;
    u32 hnc_rx_uc_pkts;
    u32 hnc_rx_mc_pkts;
    u32 hnc_rx_bc_pkts;
    u32 hnc_tx_uc_pkts;
    u32 hnc_tx_mc_pkts;
    u32 hnc_tx_bc_pkts;
    u32 hnc_fcs_err;
    u32 hnc_align_err;
    u32 hnc_false_carrier;
    u32 hnc_runt_pkts;
    u32 hnc_jabber_pkts;
    u32 hnc_rx_pause_xon;
    u32 hnc_rx_pause_xoff;
    u32 hnc_tx_pause_xon;
    u32 hnc_tx_pause_xoff;
    u32 hnc_tx_s_collision;
    u32 hnc_tx_m_collision;
    u32 hnc_l_collision;
    u32 hnc_e_collision;
    u32 hnc_rx_ctl_frames;
    u32 hnc_rx_64_frames;
    u32 hnc_rx_127_frames;
    u32 hnc_rx_255_frames;
    u32 hnc_rx_511_frames;
    u32 hnc_rx_1023_frames;
    u32 hnc_rx_1522_frames;
    u32 hnc_rx_9022_frames;
    u32 hnc_tx_64_frames;
    u32 hnc_tx_127_frames;
    u32 hnc_tx_255_frames;
    u32 hnc_tx_511_frames;
    u32 hnc_tx_1023_frames;
    u32 hnc_tx_1522_frames;
    u32 hnc_tx_9022_frames;
    u32 hnc_rx_valid_bytes;
    u32 hnc_rx_runt_pkts;
    u32 hnc_rx_jabber_pkts;
    u32 ncsi_rx_cmds;
    u32 ncsi_dropped_cmds;
    u32 ncsi_cmd_type_errs;
    u32 ncsi_cmd_csum_errs;
    u32 ncsi_rx_pkts;
    u32 ncsi_tx_pkts;
    u32 ncsi_tx_aen_pkts;
    u32 pt_tx_pkts;
    u32 pt_tx_dropped;
    u32 pt_tx_channel_err;
    u32 pt_tx_us_err;
    u32 pt_rx_pkts;
    u32 pt_rx_dropped;
    u32 pt_rx_channel_err;
    u32 pt_rx_us_err;
    u32 pt_rx_os_err;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ncsi_channel_stats {
    u32 hnc_cnt_hi;
    u32 hnc_cnt_lo;
    u32 hnc_rx_bytes;
    u32 hnc_tx_bytes;
    u32 hnc_rx_uc_pkts;
    u32 hnc_rx_mc_pkts;
    u32 hnc_rx_bc_pkts;
    u32 hnc_tx_uc_pkts;
    u32 hnc_tx_mc_pkts;
    u32 hnc_tx_bc_pkts;
    u32 hnc_fcs_err;
    u32 hnc_align_err;
    u32 hnc_false_carrier;
    u32 hnc_runt_pkts;
    u32 hnc_jabber_pkts;
    u32 hnc_rx_pause_xon;
    u32 hnc_rx_pause_xoff;
    u32 hnc_tx_pause_xon;
    u32 hnc_tx_pause_xoff;
    u32 hnc_tx_s_collision;
    u32 hnc_tx_m_collision;
    u32 hnc_l_collision;
    u32 hnc_e_collision;
    u32 hnc_rx_ctl_frames;
    u32 hnc_rx_64_frames;
    u32 hnc_rx_127_frames;
    u32 hnc_rx_255_frames;
    u32 hnc_rx_511_frames;
    u32 hnc_rx_1023_frames;
    u32 hnc_rx_1522_frames;
    u32 hnc_rx_9022_frames;
    u32 hnc_tx_64_frames;
    u32 hnc_tx_127_frames;
    u32 hnc_tx_255_frames;
    u32 hnc_tx_511_frames;
    u32 hnc_tx_1023_frames;
    u32 hnc_tx_1522_frames;
    u32 hnc_tx_9022_frames;
    u32 hnc_rx_valid_bytes;
    u32 hnc_rx_runt_pkts;
    u32 hnc_rx_jabber_pkts;
    u32 ncsi_rx_cmds;
    u32 ncsi_dropped_cmds;
    u32 ncsi_cmd_type_errs;
    u32 ncsi_cmd_csum_errs;
    u32 ncsi_rx_pkts;
    u32 ncsi_tx_pkts;
    u32 ncsi_tx_aen_pkts;
    u32 pt_tx_pkts;
    u32 pt_tx_dropped;
    u32 pt_tx_channel_err;
    u32 pt_tx_us_err;
    u32 pt_rx_pkts;
    u32 pt_rx_dropped;
    u32 pt_rx_channel_err;
    u32 pt_rx_us_err;
    u32 pt_rx_os_err;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ncsi_channel_stats {
    u32 hnc_cnt_hi;
    u32 hnc_cnt_lo;
    u32 hnc_rx_bytes;
    u32 hnc_tx_bytes;
    u32 hnc_rx_uc_pkts;
    u32 hnc_rx_mc_pkts;
    u32 hnc_rx_bc_pkts;
    u32 hnc_tx_uc_pkts;
    u32 hnc_tx_mc_pkts;
    u32 hnc_tx_bc_pkts;
    u32 hnc_fcs_err;
    u32 hnc_align_err;
    u32 hnc_false_carrier;
    u32 hnc_runt_pkts;
    u32 hnc_jabber_pkts;
    u32 hnc_rx_pause_xon;
    u32 hnc_rx_pause_xoff;
    u32 hnc_tx_pause_xon;
    u32 hnc_tx_pause_xoff;
    u32 hnc_tx_s_collision;
    u32 hnc_tx_m_collision;
    u32 hnc_l_collision;
    u32 hnc_e_collision;
    u32 hnc_rx_ctl_frames;
    u32 hnc_rx_64_frames;
    u32 hnc_rx_127_frames;
    u32 hnc_rx_255_frames;
    u32 hnc_rx_511_frames;
    u32 hnc_rx_1023_frames;
    u32 hnc_rx_1522_frames;
    u32 hnc_rx_9022_frames;
    u32 hnc_tx_64_frames;
    u32 hnc_tx_127_frames;
    u32 hnc_tx_255_frames;
    u32 hnc_tx_511_frames;
    u32 hnc_tx_1023_frames;
    u32 hnc_tx_1522_frames;
    u32 hnc_tx_9022_frames;
    u32 hnc_rx_valid_bytes;
    u32 hnc_rx_runt_pkts;
    u32 hnc_rx_jabber_pkts;
    u32 ncsi_rx_cmds;
    u32 ncsi_dropped_cmds;
    u32 ncsi_cmd_type_errs;
    u32 ncsi_cmd_csum_errs;
    u32 ncsi_rx_pkts;
    u32 ncsi_tx_pkts;
    u32 ncsi_tx_aen_pkts;
    u32 pt_tx_pkts;
    u32 pt_tx_dropped;
    u32 pt_tx_channel_err;
    u32 pt_tx_us_err;
    u32 pt_rx_pkts;
    u32 pt_rx_dropped;
    u32 pt_rx_channel_err;
    u32 pt_rx_us_err;
    u32 pt_rx_os_err;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ncsi_channel_stats {
    u32 hnc_cnt_hi;
    u32 hnc_cnt_lo;
    u32 hnc_rx_bytes;
    u32 hnc_tx_bytes;
    u32 hnc_rx_uc_pkts;
    u32 hnc_rx_mc_pkts;
    u32 hnc_rx_bc_pkts;
    u32 hnc_tx_uc_pkts;
    u32 hnc_tx_mc_pkts;
    u32 hnc_tx_bc_pkts;
    u32 hnc_fcs_err;
    u32 hnc_align_err;
    u32 hnc_false_carrier;
    u32 hnc_runt_pkts;
    u32 hnc_jabber_pkts;
    u32 hnc_rx_pause_xon;
    u32 hnc_rx_pause_xoff;
    u32 hnc_tx_pause_xon;
    u32 hnc_tx_pause_xoff;
    u32 hnc_tx_s_collision;
    u32 hnc_tx_m_collision;
    u32 hnc_l_collision;
    u32 hnc_e_collision;
    u32 hnc_rx_ctl_frames;
    u32 hnc_rx_64_frames;
    u32 hnc_rx_127_frames;
    u32 hnc_rx_255_frames;
    u32 hnc_rx_511_frames;
    u32 hnc_rx_1023_frames;
    u32 hnc_rx_1522_frames;
    u32 hnc_rx_9022_frames;
    u32 hnc_tx_64_frames;
    u32 hnc_tx_127_frames;
    u32 hnc_tx_255_frames;
    u32 hnc_tx_511_frames;
    u32 hnc_tx_1023_frames;
    u32 hnc_tx_1522_frames;
    u32 hnc_tx_9022_frames;
    u32 hnc_rx_valid_bytes;
    u32 hnc_rx_runt_pkts;
    u32 hnc_rx_jabber_pkts;
    u32 ncsi_rx_cmds;
    u32 ncsi_dropped_cmds;
    u32 ncsi_cmd_type_errs;
    u32 ncsi_cmd_csum_errs;
    u32 ncsi_rx_pkts;
    u32 ncsi_tx_pkts;
    u32 ncsi_tx_aen_pkts;
    u32 pt_tx_pkts;
    u32 pt_tx_dropped;
    u32 pt_tx_channel_err;
    u32 pt_tx_us_err;
    u32 pt_rx_pkts;
    u32 pt_rx_dropped;
    u32 pt_rx_channel_err;
    u32 pt_rx_us_err;
    u32 pt_rx_os_err;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ncsi_channel_stats {
    u32 hnc_cnt_hi;
    u32 hnc_cnt_lo;
    u32 hnc_rx_bytes;
    u32 hnc_tx_bytes;
    u32 hnc_rx_uc_pkts;
    u32 hnc_rx_mc_pkts;
    u32 hnc_rx_bc_pkts;
    u32 hnc_tx_uc_pkts;
    u32 hnc_tx_mc_pkts;
    u32 hnc_tx_bc_pkts;
    u32 hnc_fcs_err;
    u32 hnc_align_err;
    u32 hnc_false_carrier;
    u32 hnc_runt_pkts;
    u32 hnc_jabber_pkts;
    u32 hnc_rx_pause_xon;
    u32 hnc_rx_pause_xoff;
    u32 hnc_tx_pause_xon;
    u32 hnc_tx_pause_xoff;
    u32 hnc_tx_s_collision;
    u32 hnc_tx_m_collision;
    u32 hnc_l_collision;
    u32 hnc_e_collision;
    u32 hnc_rx_ctl_frames;
    u32 hnc_rx_64_frames;
    u32 hnc_rx_127_frames;
    u32 hnc_rx_255_frames;
    u32 hnc_rx_511_frames;
    u32 hnc_rx_1023_frames;
    u32 hnc_rx_1522_frames;
    u32 hnc_rx_9022_frames;
    u32 hnc_tx_64_frames;
    u32 hnc_tx_127_frames;
    u32 hnc_tx_255_frames;
    u32 hnc_tx_511_frames;
    u32 hnc_tx_1023_frames;
    u32 hnc_tx_1522_frames;
    u32 hnc_tx_9022_frames;
    u32 hnc_rx_valid_bytes;
    u32 hnc_rx_runt_pkts;
    u32 hnc_rx_jabber_pkts;
    u32 ncsi_rx_cmds;
    u32 ncsi_dropped_cmds;
    u32 ncsi_cmd_type_errs;
    u32 ncsi_cmd_csum_errs;
    u32 ncsi_rx_pkts;
    u32 ncsi_tx_pkts;
    u32 ncsi_tx_aen_pkts;
    u32 pt_tx_pkts;
    u32 pt_tx_dropped;
    u32 pt_tx_channel_err;
    u32 pt_tx_us_err;
    u32 pt_rx_pkts;
    u32 pt_rx_dropped;
    u32 pt_rx_channel_err;
    u32 pt_rx_us_err;
    u32 pt_rx_os_err;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ncsi_channel_stats {
    u32 hnc_cnt_hi;
    u32 hnc_cnt_lo;
    u32 hnc_rx_bytes;
    u32 hnc_tx_bytes;
    u32 hnc_rx_uc_pkts;
    u32 hnc_rx_mc_pkts;
    u32 hnc_rx_bc_pkts;
    u32 hnc_tx_uc_pkts;
    u32 hnc_tx_mc_pkts;
    u32 hnc_tx_bc_pkts;
    u32 hnc_fcs_err;
    u32 hnc_align_err;
    u32 hnc_false_carrier;
    u32 hnc_runt_pkts;
    u32 hnc_jabber_pkts;
    u32 hnc_rx_pause_xon;
    u32 hnc_rx_pause_xoff;
    u32 hnc_tx_pause_xon;
    u32 hnc_tx_pause_xoff;
    u32 hnc_tx_s_collision;
    u32 hnc_tx_m_collision;
    u32 hnc_l_collision;
    u32 hnc_e_collision;
    u32 hnc_rx_ctl_frames;
    u32 hnc_rx_64_frames;
    u32 hnc_rx_127_frames;
    u32 hnc_rx_255_frames;
    u32 hnc_rx_511_frames;
    u32 hnc_rx_1023_frames;
    u32 hnc_rx_1522_frames;
    u32 hnc_rx_9022_frames;
    u32 hnc_tx_64_frames;
    u32 hnc_tx_127_frames;
    u32 hnc_tx_255_frames;
    u32 hnc_tx_511_frames;
    u32 hnc_tx_1023_frames;
    u32 hnc_tx_1522_frames;
    u32 hnc_tx_9022_frames;
    u32 hnc_rx_valid_bytes;
    u32 hnc_rx_runt_pkts;
    u32 hnc_rx_jabber_pkts;
    u32 ncsi_rx_cmds;
    u32 ncsi_dropped_cmds;
    u32 ncsi_cmd_type_errs;
    u32 ncsi_cmd_csum_errs;
    u32 ncsi_rx_pkts;
    u32 ncsi_tx_pkts;
    u32 ncsi_tx_aen_pkts;
    u32 pt_tx_pkts;
    u32 pt_tx_dropped;
    u32 pt_tx_channel_err;
    u32 pt_tx_us_err;
    u32 pt_rx_pkts;
    u32 pt_rx_dropped;
    u32 pt_rx_channel_err;
    u32 pt_rx_us_err;
    u32 pt_rx_os_err;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ncsi_channel_stats {
    u32 hnc_cnt_hi;
    u32 hnc_cnt_lo;
    u32 hnc_rx_bytes;
    u32 hnc_tx_bytes;
    u32 hnc_rx_uc_pkts;
    u32 hnc_rx_mc_pkts;
    u32 hnc_rx_bc_pkts;
    u32 hnc_tx_uc_pkts;
    u32 hnc_tx_mc_pkts;
    u32 hnc_tx_bc_pkts;
    u32 hnc_fcs_err;
    u32 hnc_align_err;
    u32 hnc_false_carrier;
    u32 hnc_runt_pkts;
    u32 hnc_jabber_pkts;
    u32 hnc_rx_pause_xon;
    u32 hnc_rx_pause_xoff;
    u32 hnc_tx_pause_xon;
    u32 hnc_tx_pause_xoff;
    u32 hnc_tx_s_collision;
    u32 hnc_tx_m_collision;
    u32 hnc_l_collision;
    u32 hnc_e_collision;
    u32 hnc_rx_ctl_frames;
    u32 hnc_rx_64_frames;
    u32 hnc_rx_127_frames;
    u32 hnc_rx_255_frames;
    u32 hnc_rx_511_frames;
    u32 hnc_rx_1023_frames;
    u32 hnc_rx_1522_frames;
    u32 hnc_rx_9022_frames;
    u32 hnc_tx_64_frames;
    u32 hnc_tx_127_frames;
    u32 hnc_tx_255_frames;
    u32 hnc_tx_511_frames;
    u32 hnc_tx_1023_frames;
    u32 hnc_tx_1522_frames;
    u32 hnc_tx_9022_frames;
    u32 hnc_rx_valid_bytes;
    u32 hnc_rx_runt_pkts;
    u32 hnc_rx_jabber_pkts;
    u32 ncsi_rx_cmds;
    u32 ncsi_dropped_cmds;
    u32 ncsi_cmd_type_errs;
    u32 ncsi_cmd_csum_errs;
    u32 ncsi_rx_pkts;
    u32 ncsi_tx_pkts;
    u32 ncsi_tx_aen_pkts;
    u32 pt_tx_pkts;
    u32 pt_tx_dropped;
    u32 pt_tx_channel_err;
    u32 pt_tx_us_err;
    u32 pt_rx_pkts;
    u32 pt_rx_dropped;
    u32 pt_rx_channel_err;
    u32 pt_rx_us_err;
    u32 pt_rx_os_err;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ncsi_channel_stats {
    u32 hnc_cnt_hi;
    u32 hnc_cnt_lo;
    u32 hnc_rx_bytes;
    u32 hnc_tx_bytes;
    u32 hnc_rx_uc_pkts;
    u32 hnc_rx_mc_pkts;
    u32 hnc_rx_bc_pkts;
    u32 hnc_tx_uc_pkts;
    u32 hnc_tx_mc_pkts;
    u32 hnc_tx_bc_pkts;
    u32 hnc_fcs_err;
    u32 hnc_align_err;
    u32 hnc_false_carrier;
    u32 hnc_runt_pkts;
    u32 hnc_jabber_pkts;
    u32 hnc_rx_pause_xon;
    u32 hnc_rx_pause_xoff;
    u32 hnc_tx_pause_xon;
    u32 hnc_tx_pause_xoff;
    u32 hnc_tx_s_collision;
    u32 hnc_tx_m_collision;
    u32 hnc_l_collision;
    u32 hnc_e_collision;
    u32 hnc_rx_ctl_frames;
    u32 hnc_rx_64_frames;
    u32 hnc_rx_127_frames;
    u32 hnc_rx_255_frames;
    u32 hnc_rx_511_frames;
    u32 hnc_rx_1023_frames;
    u32 hnc_rx_1522_frames;
    u32 hnc_rx_9022_frames;
    u32 hnc_tx_64_frames;
    u32 hnc_tx_127_frames;
    u32 hnc_tx_255_frames;
    u32 hnc_tx_511_frames;
    u32 hnc_tx_1023_frames;
    u32 hnc_tx_1522_frames;
    u32 hnc_tx_9022_frames;
    u32 hnc_rx_valid_bytes;
    u32 hnc_rx_runt_pkts;
    u32 hnc_rx_jabber_pkts;
    u32 ncsi_rx_cmds;
    u32 ncsi_dropped_cmds;
    u32 ncsi_cmd_type_errs;
    u32 ncsi_cmd_csum_errs;
    u32 ncsi_rx_pkts;
    u32 ncsi_tx_pkts;
    u32 ncsi_tx_aen_pkts;
    u32 pt_tx_pkts;
    u32 pt_tx_dropped;
    u32 pt_tx_channel_err;
    u32 pt_tx_us_err;
    u32 pt_rx_pkts;
    u32 pt_rx_dropped;
    u32 pt_rx_channel_err;
    u32 pt_rx_us_err;
    u32 pt_rx_os_err;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ncsi_channel_stats {
    u32 hnc_cnt_hi;
    u32 hnc_cnt_lo;
    u32 hnc_rx_bytes;
    u32 hnc_tx_bytes;
    u32 hnc_rx_uc_pkts;
    u32 hnc_rx_mc_pkts;
    u32 hnc_rx_bc_pkts;
    u32 hnc_tx_uc_pkts;
    u32 hnc_tx_mc_pkts;
    u32 hnc_tx_bc_pkts;
    u32 hnc_fcs_err;
    u32 hnc_align_err;
    u32 hnc_false_carrier;
    u32 hnc_runt_pkts;
    u32 hnc_jabber_pkts;
    u32 hnc_rx_pause_xon;
    u32 hnc_rx_pause_xoff;
    u32 hnc_tx_pause_xon;
    u32 hnc_tx_pause_xoff;
    u32 hnc_tx_s_collision;
    u32 hnc_tx_m_collision;
    u32 hnc_l_collision;
    u32 hnc_e_collision;
    u32 hnc_rx_ctl_frames;
    u32 hnc_rx_64_frames;
    u32 hnc_rx_127_frames;
    u32 hnc_rx_255_frames;
    u32 hnc_rx_511_frames;
    u32 hnc_rx_1023_frames;
    u32 hnc_rx_1522_frames;
    u32 hnc_rx_9022_frames;
    u32 hnc_tx_64_frames;
    u32 hnc_tx_127_frames;
    u32 hnc_tx_255_frames;
    u32 hnc_tx_511_frames;
    u32 hnc_tx_1023_frames;
    u32 hnc_tx_1522_frames;
    u32 hnc_tx_9022_frames;
    u32 hnc_rx_valid_bytes;
    u32 hnc_rx_runt_pkts;
    u32 hnc_rx_jabber_pkts;
    u32 ncsi_rx_cmds;
    u32 ncsi_dropped_cmds;
    u32 ncsi_cmd_type_errs;
    u32 ncsi_cmd_csum_errs;
    u32 ncsi_rx_pkts;
    u32 ncsi_tx_pkts;
    u32 ncsi_tx_aen_pkts;
    u32 pt_tx_pkts;
    u32 pt_tx_dropped;
    u32 pt_tx_channel_err;
    u32 pt_tx_us_err;
    u32 pt_rx_pkts;
    u32 pt_rx_dropped;
    u32 pt_rx_channel_err;
    u32 pt_rx_us_err;
    u32 pt_rx_os_err;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ncsi_channel_stats {
    u32 hnc_cnt_hi;
    u32 hnc_cnt_lo;
    u32 hnc_rx_bytes;
    u32 hnc_tx_bytes;
    u32 hnc_rx_uc_pkts;
    u32 hnc_rx_mc_pkts;
    u32 hnc_rx_bc_pkts;
    u32 hnc_tx_uc_pkts;
    u32 hnc_tx_mc_pkts;
    u32 hnc_tx_bc_pkts;
    u32 hnc_fcs_err;
    u32 hnc_align_err;
    u32 hnc_false_carrier;
    u32 hnc_runt_pkts;
    u32 hnc_jabber_pkts;
    u32 hnc_rx_pause_xon;
    u32 hnc_rx_pause_xoff;
    u32 hnc_tx_pause_xon;
    u32 hnc_tx_pause_xoff;
    u32 hnc_tx_s_collision;
    u32 hnc_tx_m_collision;
    u32 hnc_l_collision;
    u32 hnc_e_collision;
    u32 hnc_rx_ctl_frames;
    u32 hnc_rx_64_frames;
    u32 hnc_rx_127_frames;
    u32 hnc_rx_255_frames;
    u32 hnc_rx_511_frames;
    u32 hnc_rx_1023_frames;
    u32 hnc_rx_1522_frames;
    u32 hnc_rx_9022_frames;
    u32 hnc_tx_64_frames;
    u32 hnc_tx_127_frames;
    u32 hnc_tx_255_frames;
    u32 hnc_tx_511_frames;
    u32 hnc_tx_1023_frames;
    u32 hnc_tx_1522_frames;
    u32 hnc_tx_9022_frames;
    u32 hnc_rx_valid_bytes;
    u32 hnc_rx_runt_pkts;
    u32 hnc_rx_jabber_pkts;
    u32 ncsi_rx_cmds;
    u32 ncsi_dropped_cmds;
    u32 ncsi_cmd_type_errs;
    u32 ncsi_cmd_csum_errs;
    u32 ncsi_rx_pkts;
    u32 ncsi_tx_pkts;
    u32 ncsi_tx_aen_pkts;
    u32 pt_tx_pkts;
    u32 pt_tx_dropped;
    u32 pt_tx_channel_err;
    u32 pt_tx_us_err;
    u32 pt_rx_pkts;
    u32 pt_rx_dropped;
    u32 pt_rx_channel_err;
    u32 pt_rx_us_err;
    u32 pt_rx_os_err;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ncsi_channel_stats {
    u32 hnc_cnt_hi;
    u32 hnc_cnt_lo;
    u32 hnc_rx_bytes;
    u32 hnc_tx_bytes;
    u32 hnc_rx_uc_pkts;
    u32 hnc_rx_mc_pkts;
    u32 hnc_rx_bc_pkts;
    u32 hnc_tx_uc_pkts;
    u32 hnc_tx_mc_pkts;
    u32 hnc_tx_bc_pkts;
    u32 hnc_fcs_err;
    u32 hnc_align_err;
    u32 hnc_false_carrier;
    u32 hnc_runt_pkts;
    u32 hnc_jabber_pkts;
    u32 hnc_rx_pause_xon;
    u32 hnc_rx_pause_xoff;
    u32 hnc_tx_pause_xon;
    u32 hnc_tx_pause_xoff;
    u32 hnc_tx_s_collision;
    u32 hnc_tx_m_collision;
    u32 hnc_l_collision;
    u32 hnc_e_collision;
    u32 hnc_rx_ctl_frames;
    u32 hnc_rx_64_frames;
    u32 hnc_rx_127_frames;
    u32 hnc_rx_255_frames;
    u32 hnc_rx_511_frames;
    u32 hnc_rx_1023_frames;
    u32 hnc_rx_1522_frames;
    u32 hnc_rx_9022_frames;
    u32 hnc_tx_64_frames;
    u32 hnc_tx_127_frames;
    u32 hnc_tx_255_frames;
    u32 hnc_tx_511_frames;
    u32 hnc_tx_1023_frames;
    u32 hnc_tx_1522_frames;
    u32 hnc_tx_9022_frames;
    u32 hnc_rx_valid_bytes;
    u32 hnc_rx_runt_pkts;
    u32 hnc_rx_jabber_pkts;
    u32 ncsi_rx_cmds;
    u32 ncsi_dropped_cmds;
    u32 ncsi_cmd_type_errs;
    u32 ncsi_cmd_csum_errs;
    u32 ncsi_rx_pkts;
    u32 ncsi_tx_pkts;
    u32 ncsi_tx_aen_pkts;
    u32 pt_tx_pkts;
    u32 pt_tx_dropped;
    u32 pt_tx_channel_err;
    u32 pt_tx_us_err;
    u32 pt_rx_pkts;
    u32 pt_rx_dropped;
    u32 pt_rx_channel_err;
    u32 pt_rx_us_err;
    u32 pt_rx_os_err;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ncsi_channel_stats {
    u32 hnc_cnt_hi;
    u32 hnc_cnt_lo;
    u32 hnc_rx_bytes;
    u32 hnc_tx_bytes;
    u32 hnc_rx_uc_pkts;
    u32 hnc_rx_mc_pkts;
    u32 hnc_rx_bc_pkts;
    u32 hnc_tx_uc_pkts;
    u32 hnc_tx_mc_pkts;
    u32 hnc_tx_bc_pkts;
    u32 hnc_fcs_err;
    u32 hnc_align_err;
    u32 hnc_false_carrier;
    u32 hnc_runt_pkts;
    u32 hnc_jabber_pkts;
    u32 hnc_rx_pause_xon;
    u32 hnc_rx_pause_xoff;
    u32 hnc_tx_pause_xon;
    u32 hnc_tx_pause_xoff;
    u32 hnc_tx_s_collision;
    u32 hnc_tx_m_collision;
    u32 hnc_l_collision;
    u32 hnc_e_collision;
    u32 hnc_rx_ctl_frames;
    u32 hnc_rx_64_frames;
    u32 hnc_rx_127_frames;
    u32 hnc_rx_255_frames;
    u32 hnc_rx_511_frames;
    u32 hnc_rx_1023_frames;
    u32 hnc_rx_1522_frames;
    u32 hnc_rx_9022_frames;
    u32 hnc_tx_64_frames;
    u32 hnc_tx_127_frames;
    u32 hnc_tx_255_frames;
    u32 hnc_tx_511_frames;
    u32 hnc_tx_1023_frames;
    u32 hnc_tx_1522_frames;
    u32 hnc_tx_9022_frames;
    u32 hnc_rx_valid_bytes;
    u32 hnc_rx_runt_pkts;
    u32 hnc_rx_jabber_pkts;
    u32 ncsi_rx_cmds;
    u32 ncsi_dropped_cmds;
    u32 ncsi_cmd_type_errs;
    u32 ncsi_cmd_csum_errs;
    u32 ncsi_rx_pkts;
    u32 ncsi_tx_pkts;
    u32 ncsi_tx_aen_pkts;
    u32 pt_tx_pkts;
    u32 pt_tx_dropped;
    u32 pt_tx_channel_err;
    u32 pt_tx_us_err;
    u32 pt_rx_pkts;
    u32 pt_rx_dropped;
    u32 pt_rx_channel_err;
    u32 pt_rx_us_err;
    u32 pt_rx_os_err;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ncsi_channel_stats {
    u32 hnc_cnt_hi;
    u32 hnc_cnt_lo;
    u32 hnc_rx_bytes;
    u32 hnc_tx_bytes;
    u32 hnc_rx_uc_pkts;
    u32 hnc_rx_mc_pkts;
    u32 hnc_rx_bc_pkts;
    u32 hnc_tx_uc_pkts;
    u32 hnc_tx_mc_pkts;
    u32 hnc_tx_bc_pkts;
    u32 hnc_fcs_err;
    u32 hnc_align_err;
    u32 hnc_false_carrier;
    u32 hnc_runt_pkts;
    u32 hnc_jabber_pkts;
    u32 hnc_rx_pause_xon;
    u32 hnc_rx_pause_xoff;
    u32 hnc_tx_pause_xon;
    u32 hnc_tx_pause_xoff;
    u32 hnc_tx_s_collision;
    u32 hnc_tx_m_collision;
    u32 hnc_l_collision;
    u32 hnc_e_collision;
    u32 hnc_rx_ctl_frames;
    u32 hnc_rx_64_frames;
    u32 hnc_rx_127_frames;
    u32 hnc_rx_255_frames;
    u32 hnc_rx_511_frames;
    u32 hnc_rx_1023_frames;
    u32 hnc_rx_1522_frames;
    u32 hnc_rx_9022_frames;
    u32 hnc_tx_64_frames;
    u32 hnc_tx_127_frames;
    u32 hnc_tx_255_frames;
    u32 hnc_tx_511_frames;
    u32 hnc_tx_1023_frames;
    u32 hnc_tx_1522_frames;
    u32 hnc_tx_9022_frames;
    u32 hnc_rx_valid_bytes;
    u32 hnc_rx_runt_pkts;
    u32 hnc_rx_jabber_pkts;
    u32 ncsi_rx_cmds;
    u32 ncsi_dropped_cmds;
    u32 ncsi_cmd_type_errs;
    u32 ncsi_cmd_csum_errs;
    u32 ncsi_rx_pkts;
    u32 ncsi_tx_pkts;
    u32 ncsi_tx_aen_pkts;
    u32 pt_tx_pkts;
    u32 pt_tx_dropped;
    u32 pt_tx_channel_err;
    u32 pt_tx_us_err;
    u32 pt_rx_pkts;
    u32 pt_rx_dropped;
    u32 pt_rx_channel_err;
    u32 pt_rx_us_err;
    u32 pt_rx_os_err;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ncsi_channel_stats {
    u32 hnc_cnt_hi;
    u32 hnc_cnt_lo;
    u32 hnc_rx_bytes;
    u32 hnc_tx_bytes;
    u32 hnc_rx_uc_pkts;
    u32 hnc_rx_mc_pkts;
    u32 hnc_rx_bc_pkts;
    u32 hnc_tx_uc_pkts;
    u32 hnc_tx_mc_pkts;
    u32 hnc_tx_bc_pkts;
    u32 hnc_fcs_err;
    u32 hnc_align_err;
    u32 hnc_false_carrier;
    u32 hnc_runt_pkts;
    u32 hnc_jabber_pkts;
    u32 hnc_rx_pause_xon;
    u32 hnc_rx_pause_xoff;
    u32 hnc_tx_pause_xon;
    u32 hnc_tx_pause_xoff;
    u32 hnc_tx_s_collision;
    u32 hnc_tx_m_collision;
    u32 hnc_l_collision;
    u32 hnc_e_collision;
    u32 hnc_rx_ctl_frames;
    u32 hnc_rx_64_frames;
    u32 hnc_rx_127_frames;
    u32 hnc_rx_255_frames;
    u32 hnc_rx_511_frames;
    u32 hnc_rx_1023_frames;
    u32 hnc_rx_1522_frames;
    u32 hnc_rx_9022_frames;
    u32 hnc_tx_64_frames;
    u32 hnc_tx_127_frames;
    u32 hnc_tx_255_frames;
    u32 hnc_tx_511_frames;
    u32 hnc_tx_1023_frames;
    u32 hnc_tx_1522_frames;
    u32 hnc_tx_9022_frames;
    u32 hnc_rx_valid_bytes;
    u32 hnc_rx_runt_pkts;
    u32 hnc_rx_jabber_pkts;
    u32 ncsi_rx_cmds;
    u32 ncsi_dropped_cmds;
    u32 ncsi_cmd_type_errs;
    u32 ncsi_cmd_csum_errs;
    u32 ncsi_rx_pkts;
    u32 ncsi_tx_pkts;
    u32 ncsi_tx_aen_pkts;
    u32 pt_tx_pkts;
    u32 pt_tx_dropped;
    u32 pt_tx_channel_err;
    u32 pt_tx_us_err;
    u32 pt_rx_pkts;
    u32 pt_rx_dropped;
    u32 pt_rx_channel_err;
    u32 pt_rx_us_err;
    u32 pt_rx_os_err;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ncsi_channel_stats {
    u32 hnc_cnt_hi;
    u32 hnc_cnt_lo;
    u32 hnc_rx_bytes;
    u32 hnc_tx_bytes;
    u32 hnc_rx_uc_pkts;
    u32 hnc_rx_mc_pkts;
    u32 hnc_rx_bc_pkts;
    u32 hnc_tx_uc_pkts;
    u32 hnc_tx_mc_pkts;
    u32 hnc_tx_bc_pkts;
    u32 hnc_fcs_err;
    u32 hnc_align_err;
    u32 hnc_false_carrier;
    u32 hnc_runt_pkts;
    u32 hnc_jabber_pkts;
    u32 hnc_rx_pause_xon;
    u32 hnc_rx_pause_xoff;
    u32 hnc_tx_pause_xon;
    u32 hnc_tx_pause_xoff;
    u32 hnc_tx_s_collision;
    u32 hnc_tx_m_collision;
    u32 hnc_l_collision;
    u32 hnc_e_collision;
    u32 hnc_rx_ctl_frames;
    u32 hnc_rx_64_frames;
    u32 hnc_rx_127_frames;
    u32 hnc_rx_255_frames;
    u32 hnc_rx_511_frames;
    u32 hnc_rx_1023_frames;
    u32 hnc_rx_1522_frames;
    u32 hnc_rx_9022_frames;
    u32 hnc_tx_64_frames;
    u32 hnc_tx_127_frames;
    u32 hnc_tx_255_frames;
    u32 hnc_tx_511_frames;
    u32 hnc_tx_1023_frames;
    u32 hnc_tx_1522_frames;
    u32 hnc_tx_9022_frames;
    u32 hnc_rx_valid_bytes;
    u32 hnc_rx_runt_pkts;
    u32 hnc_rx_jabber_pkts;
    u32 ncsi_rx_cmds;
    u32 ncsi_dropped_cmds;
    u32 ncsi_cmd_type_errs;
    u32 ncsi_cmd_csum_errs;
    u32 ncsi_rx_pkts;
    u32 ncsi_tx_pkts;
    u32 ncsi_tx_aen_pkts;
    u32 pt_tx_pkts;
    u32 pt_tx_dropped;
    u32 pt_tx_channel_err;
    u32 pt_tx_us_err;
    u32 pt_rx_pkts;
    u32 pt_rx_dropped;
    u32 pt_rx_channel_err;
    u32 pt_rx_us_err;
    u32 pt_rx_os_err;
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct ncsi_channel_stats {
    u32 hnc_cnt_hi;
    u32 hnc_cnt_lo;
    u32 hnc_rx_bytes;
    u32 hnc_tx_bytes;
    u32 hnc_rx_uc_pkts;
    u32 hnc_rx_mc_pkts;
    u32 hnc_rx_bc_pkts;
    u32 hnc_tx_uc_pkts;
    u32 hnc_tx_mc_pkts;
    u32 hnc_tx_bc_pkts;
    u32 hnc_fcs_err;
    u32 hnc_align_err;
    u32 hnc_false_carrier;
    u32 hnc_runt_pkts;
    u32 hnc_jabber_pkts;
    u32 hnc_rx_pause_xon;
    u32 hnc_rx_pause_xoff;
    u32 hnc_tx_pause_xon;
    u32 hnc_tx_pause_xoff;
    u32 hnc_tx_s_collision;
    u32 hnc_tx_m_collision;
    u32 hnc_l_collision;
    u32 hnc_e_collision;
    u32 hnc_rx_ctl_frames;
    u32 hnc_rx_64_frames;
    u32 hnc_rx_127_frames;
    u32 hnc_rx_255_frames;
    u32 hnc_rx_511_frames;
    u32 hnc_rx_1023_frames;
    u32 hnc_rx_1522_frames;
    u32 hnc_rx_9022_frames;
    u32 hnc_tx_64_frames;
    u32 hnc_tx_127_frames;
    u32 hnc_tx_255_frames;
    u32 hnc_tx_511_frames;
    u32 hnc_tx_1023_frames;
    u32 hnc_tx_1522_frames;
    u32 hnc_tx_9022_frames;
    u32 hnc_rx_valid_bytes;
    u32 hnc_rx_runt_pkts;
    u32 hnc_rx_jabber_pkts;
    u32 ncsi_rx_cmds;
    u32 ncsi_dropped_cmds;
    u32 ncsi_cmd_type_errs;
    u32 ncsi_cmd_csum_errs;
    u32 ncsi_rx_pkts;
    u32 ncsi_tx_pkts;
    u32 ncsi_tx_aen_pkts;
    u32 pt_tx_pkts;
    u32 pt_tx_dropped;
    u32 pt_tx_channel_err;
    u32 pt_tx_us_err;
    u32 pt_rx_pkts;
    u32 pt_rx_dropped;
    u32 pt_rx_channel_err;
    u32 pt_rx_us_err;
    u32 pt_rx_os_err;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ncsi_channel_stats {
    u32 hnc_cnt_hi;
    u32 hnc_cnt_lo;
    u32 hnc_rx_bytes;
    u32 hnc_tx_bytes;
    u32 hnc_rx_uc_pkts;
    u32 hnc_rx_mc_pkts;
    u32 hnc_rx_bc_pkts;
    u32 hnc_tx_uc_pkts;
    u32 hnc_tx_mc_pkts;
    u32 hnc_tx_bc_pkts;
    u32 hnc_fcs_err;
    u32 hnc_align_err;
    u32 hnc_false_carrier;
    u32 hnc_runt_pkts;
    u32 hnc_jabber_pkts;
    u32 hnc_rx_pause_xon;
    u32 hnc_rx_pause_xoff;
    u32 hnc_tx_pause_xon;
    u32 hnc_tx_pause_xoff;
    u32 hnc_tx_s_collision;
    u32 hnc_tx_m_collision;
    u32 hnc_l_collision;
    u32 hnc_e_collision;
    u32 hnc_rx_ctl_frames;
    u32 hnc_rx_64_frames;
    u32 hnc_rx_127_frames;
    u32 hnc_rx_255_frames;
    u32 hnc_rx_511_frames;
    u32 hnc_rx_1023_frames;
    u32 hnc_rx_1522_frames;
    u32 hnc_rx_9022_frames;
    u32 hnc_tx_64_frames;
    u32 hnc_tx_127_frames;
    u32 hnc_tx_255_frames;
    u32 hnc_tx_511_frames;
    u32 hnc_tx_1023_frames;
    u32 hnc_tx_1522_frames;
    u32 hnc_tx_9022_frames;
    u32 hnc_rx_valid_bytes;
    u32 hnc_rx_runt_pkts;
    u32 hnc_rx_jabber_pkts;
    u32 ncsi_rx_cmds;
    u32 ncsi_dropped_cmds;
    u32 ncsi_cmd_type_errs;
    u32 ncsi_cmd_csum_errs;
    u32 ncsi_rx_pkts;
    u32 ncsi_tx_pkts;
    u32 ncsi_tx_aen_pkts;
    u32 pt_tx_pkts;
    u32 pt_tx_dropped;
    u32 pt_tx_channel_err;
    u32 pt_tx_us_err;
    u32 pt_rx_pkts;
    u32 pt_rx_dropped;
    u32 pt_rx_channel_err;
    u32 pt_rx_us_err;
    u32 pt_rx_os_err;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ncsi_channel_stats {
    u32 hnc_cnt_hi;
    u32 hnc_cnt_lo;
    u32 hnc_rx_bytes;
    u32 hnc_tx_bytes;
    u32 hnc_rx_uc_pkts;
    u32 hnc_rx_mc_pkts;
    u32 hnc_rx_bc_pkts;
    u32 hnc_tx_uc_pkts;
    u32 hnc_tx_mc_pkts;
    u32 hnc_tx_bc_pkts;
    u32 hnc_fcs_err;
    u32 hnc_align_err;
    u32 hnc_false_carrier;
    u32 hnc_runt_pkts;
    u32 hnc_jabber_pkts;
    u32 hnc_rx_pause_xon;
    u32 hnc_rx_pause_xoff;
    u32 hnc_tx_pause_xon;
    u32 hnc_tx_pause_xoff;
    u32 hnc_tx_s_collision;
    u32 hnc_tx_m_collision;
    u32 hnc_l_collision;
    u32 hnc_e_collision;
    u32 hnc_rx_ctl_frames;
    u32 hnc_rx_64_frames;
    u32 hnc_rx_127_frames;
    u32 hnc_rx_255_frames;
    u32 hnc_rx_511_frames;
    u32 hnc_rx_1023_frames;
    u32 hnc_rx_1522_frames;
    u32 hnc_rx_9022_frames;
    u32 hnc_tx_64_frames;
    u32 hnc_tx_127_frames;
    u32 hnc_tx_255_frames;
    u32 hnc_tx_511_frames;
    u32 hnc_tx_1023_frames;
    u32 hnc_tx_1522_frames;
    u32 hnc_tx_9022_frames;
    u32 hnc_rx_valid_bytes;
    u32 hnc_rx_runt_pkts;
    u32 hnc_rx_jabber_pkts;
    u32 ncsi_rx_cmds;
    u32 ncsi_dropped_cmds;
    u32 ncsi_cmd_type_errs;
    u32 ncsi_cmd_csum_errs;
    u32 ncsi_rx_pkts;
    u32 ncsi_tx_pkts;
    u32 ncsi_tx_aen_pkts;
    u32 pt_tx_pkts;
    u32 pt_tx_dropped;
    u32 pt_tx_channel_err;
    u32 pt_tx_us_err;
    u32 pt_rx_pkts;
    u32 pt_rx_dropped;
    u32 pt_rx_channel_err;
    u32 pt_rx_us_err;
    u32 pt_rx_os_err;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ncsi_channel_stats {
    u32 hnc_cnt_hi;
    u32 hnc_cnt_lo;
    u32 hnc_rx_bytes;
    u32 hnc_tx_bytes;
    u32 hnc_rx_uc_pkts;
    u32 hnc_rx_mc_pkts;
    u32 hnc_rx_bc_pkts;
    u32 hnc_tx_uc_pkts;
    u32 hnc_tx_mc_pkts;
    u32 hnc_tx_bc_pkts;
    u32 hnc_fcs_err;
    u32 hnc_align_err;
    u32 hnc_false_carrier;
    u32 hnc_runt_pkts;
    u32 hnc_jabber_pkts;
    u32 hnc_rx_pause_xon;
    u32 hnc_rx_pause_xoff;
    u32 hnc_tx_pause_xon;
    u32 hnc_tx_pause_xoff;
    u32 hnc_tx_s_collision;
    u32 hnc_tx_m_collision;
    u32 hnc_l_collision;
    u32 hnc_e_collision;
    u32 hnc_rx_ctl_frames;
    u32 hnc_rx_64_frames;
    u32 hnc_rx_127_frames;
    u32 hnc_rx_255_frames;
    u32 hnc_rx_511_frames;
    u32 hnc_rx_1023_frames;
    u32 hnc_rx_1522_frames;
    u32 hnc_rx_9022_frames;
    u32 hnc_tx_64_frames;
    u32 hnc_tx_127_frames;
    u32 hnc_tx_255_frames;
    u32 hnc_tx_511_frames;
    u32 hnc_tx_1023_frames;
    u32 hnc_tx_1522_frames;
    u32 hnc_tx_9022_frames;
    u32 hnc_rx_valid_bytes;
    u32 hnc_rx_runt_pkts;
    u32 hnc_rx_jabber_pkts;
    u32 ncsi_rx_cmds;
    u32 ncsi_dropped_cmds;
    u32 ncsi_cmd_type_errs;
    u32 ncsi_cmd_csum_errs;
    u32 ncsi_rx_pkts;
    u32 ncsi_tx_pkts;
    u32 ncsi_tx_aen_pkts;
    u32 pt_tx_pkts;
    u32 pt_tx_dropped;
    u32 pt_tx_channel_err;
    u32 pt_tx_us_err;
    u32 pt_rx_pkts;
    u32 pt_rx_dropped;
    u32 pt_rx_channel_err;
    u32 pt_rx_us_err;
    u32 pt_rx_os_err;
};
```
</details>
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct ncsi_channel_stats {
    u32 hnc_cnt_hi;
    u32 hnc_cnt_lo;
    u32 hnc_rx_bytes;
    u32 hnc_tx_bytes;
    u32 hnc_rx_uc_pkts;
    u32 hnc_rx_mc_pkts;
    u32 hnc_rx_bc_pkts;
    u32 hnc_tx_uc_pkts;
    u32 hnc_tx_mc_pkts;
    u32 hnc_tx_bc_pkts;
    u32 hnc_fcs_err;
    u32 hnc_align_err;
    u32 hnc_false_carrier;
    u32 hnc_runt_pkts;
    u32 hnc_jabber_pkts;
    u32 hnc_rx_pause_xon;
    u32 hnc_rx_pause_xoff;
    u32 hnc_tx_pause_xon;
    u32 hnc_tx_pause_xoff;
    u32 hnc_tx_s_collision;
    u32 hnc_tx_m_collision;
    u32 hnc_l_collision;
    u32 hnc_e_collision;
    u32 hnc_rx_ctl_frames;
    u32 hnc_rx_64_frames;
    u32 hnc_rx_127_frames;
    u32 hnc_rx_255_frames;
    u32 hnc_rx_511_frames;
    u32 hnc_rx_1023_frames;
    u32 hnc_rx_1522_frames;
    u32 hnc_rx_9022_frames;
    u32 hnc_tx_64_frames;
    u32 hnc_tx_127_frames;
    u32 hnc_tx_255_frames;
    u32 hnc_tx_511_frames;
    u32 hnc_tx_1023_frames;
    u32 hnc_tx_1522_frames;
    u32 hnc_tx_9022_frames;
    u32 hnc_rx_valid_bytes;
    u32 hnc_rx_runt_pkts;
    u32 hnc_rx_jabber_pkts;
    u32 ncsi_rx_cmds;
    u32 ncsi_dropped_cmds;
    u32 ncsi_cmd_type_errs;
    u32 ncsi_cmd_csum_errs;
    u32 ncsi_rx_pkts;
    u32 ncsi_tx_pkts;
    u32 ncsi_tx_aen_pkts;
    u32 pt_tx_pkts;
    u32 pt_tx_dropped;
    u32 pt_tx_channel_err;
    u32 pt_tx_us_err;
    u32 pt_rx_pkts;
    u32 pt_rx_dropped;
    u32 pt_rx_channel_err;
    u32 pt_rx_us_err;
    u32 pt_rx_os_err;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ncsi_channel_stats {
    u32 hnc_cnt_hi;
    u32 hnc_cnt_lo;
    u32 hnc_rx_bytes;
    u32 hnc_tx_bytes;
    u32 hnc_rx_uc_pkts;
    u32 hnc_rx_mc_pkts;
    u32 hnc_rx_bc_pkts;
    u32 hnc_tx_uc_pkts;
    u32 hnc_tx_mc_pkts;
    u32 hnc_tx_bc_pkts;
    u32 hnc_fcs_err;
    u32 hnc_align_err;
    u32 hnc_false_carrier;
    u32 hnc_runt_pkts;
    u32 hnc_jabber_pkts;
    u32 hnc_rx_pause_xon;
    u32 hnc_rx_pause_xoff;
    u32 hnc_tx_pause_xon;
    u32 hnc_tx_pause_xoff;
    u32 hnc_tx_s_collision;
    u32 hnc_tx_m_collision;
    u32 hnc_l_collision;
    u32 hnc_e_collision;
    u32 hnc_rx_ctl_frames;
    u32 hnc_rx_64_frames;
    u32 hnc_rx_127_frames;
    u32 hnc_rx_255_frames;
    u32 hnc_rx_511_frames;
    u32 hnc_rx_1023_frames;
    u32 hnc_rx_1522_frames;
    u32 hnc_rx_9022_frames;
    u32 hnc_tx_64_frames;
    u32 hnc_tx_127_frames;
    u32 hnc_tx_255_frames;
    u32 hnc_tx_511_frames;
    u32 hnc_tx_1023_frames;
    u32 hnc_tx_1522_frames;
    u32 hnc_tx_9022_frames;
    u32 hnc_rx_valid_bytes;
    u32 hnc_rx_runt_pkts;
    u32 hnc_rx_jabber_pkts;
    u32 ncsi_rx_cmds;
    u32 ncsi_dropped_cmds;
    u32 ncsi_cmd_type_errs;
    u32 ncsi_cmd_csum_errs;
    u32 ncsi_rx_pkts;
    u32 ncsi_tx_pkts;
    u32 ncsi_tx_aen_pkts;
    u32 pt_tx_pkts;
    u32 pt_tx_dropped;
    u32 pt_tx_channel_err;
    u32 pt_tx_us_err;
    u32 pt_rx_pkts;
    u32 pt_rx_dropped;
    u32 pt_rx_channel_err;
    u32 pt_rx_us_err;
    u32 pt_rx_os_err;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ncsi_channel_stats {
    u32 hnc_cnt_hi;
    u32 hnc_cnt_lo;
    u32 hnc_rx_bytes;
    u32 hnc_tx_bytes;
    u32 hnc_rx_uc_pkts;
    u32 hnc_rx_mc_pkts;
    u32 hnc_rx_bc_pkts;
    u32 hnc_tx_uc_pkts;
    u32 hnc_tx_mc_pkts;
    u32 hnc_tx_bc_pkts;
    u32 hnc_fcs_err;
    u32 hnc_align_err;
    u32 hnc_false_carrier;
    u32 hnc_runt_pkts;
    u32 hnc_jabber_pkts;
    u32 hnc_rx_pause_xon;
    u32 hnc_rx_pause_xoff;
    u32 hnc_tx_pause_xon;
    u32 hnc_tx_pause_xoff;
    u32 hnc_tx_s_collision;
    u32 hnc_tx_m_collision;
    u32 hnc_l_collision;
    u32 hnc_e_collision;
    u32 hnc_rx_ctl_frames;
    u32 hnc_rx_64_frames;
    u32 hnc_rx_127_frames;
    u32 hnc_rx_255_frames;
    u32 hnc_rx_511_frames;
    u32 hnc_rx_1023_frames;
    u32 hnc_rx_1522_frames;
    u32 hnc_rx_9022_frames;
    u32 hnc_tx_64_frames;
    u32 hnc_tx_127_frames;
    u32 hnc_tx_255_frames;
    u32 hnc_tx_511_frames;
    u32 hnc_tx_1023_frames;
    u32 hnc_tx_1522_frames;
    u32 hnc_tx_9022_frames;
    u32 hnc_rx_valid_bytes;
    u32 hnc_rx_runt_pkts;
    u32 hnc_rx_jabber_pkts;
    u32 ncsi_rx_cmds;
    u32 ncsi_dropped_cmds;
    u32 ncsi_cmd_type_errs;
    u32 ncsi_cmd_csum_errs;
    u32 ncsi_rx_pkts;
    u32 ncsi_tx_pkts;
    u32 ncsi_tx_aen_pkts;
    u32 pt_tx_pkts;
    u32 pt_tx_dropped;
    u32 pt_tx_channel_err;
    u32 pt_tx_us_err;
    u32 pt_rx_pkts;
    u32 pt_rx_dropped;
    u32 pt_rx_channel_err;
    u32 pt_rx_us_err;
    u32 pt_rx_os_err;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ncsi_channel_stats {
    u32 hnc_cnt_hi;
    u32 hnc_cnt_lo;
    u32 hnc_rx_bytes;
    u32 hnc_tx_bytes;
    u32 hnc_rx_uc_pkts;
    u32 hnc_rx_mc_pkts;
    u32 hnc_rx_bc_pkts;
    u32 hnc_tx_uc_pkts;
    u32 hnc_tx_mc_pkts;
    u32 hnc_tx_bc_pkts;
    u32 hnc_fcs_err;
    u32 hnc_align_err;
    u32 hnc_false_carrier;
    u32 hnc_runt_pkts;
    u32 hnc_jabber_pkts;
    u32 hnc_rx_pause_xon;
    u32 hnc_rx_pause_xoff;
    u32 hnc_tx_pause_xon;
    u32 hnc_tx_pause_xoff;
    u32 hnc_tx_s_collision;
    u32 hnc_tx_m_collision;
    u32 hnc_l_collision;
    u32 hnc_e_collision;
    u32 hnc_rx_ctl_frames;
    u32 hnc_rx_64_frames;
    u32 hnc_rx_127_frames;
    u32 hnc_rx_255_frames;
    u32 hnc_rx_511_frames;
    u32 hnc_rx_1023_frames;
    u32 hnc_rx_1522_frames;
    u32 hnc_rx_9022_frames;
    u32 hnc_tx_64_frames;
    u32 hnc_tx_127_frames;
    u32 hnc_tx_255_frames;
    u32 hnc_tx_511_frames;
    u32 hnc_tx_1023_frames;
    u32 hnc_tx_1522_frames;
    u32 hnc_tx_9022_frames;
    u32 hnc_rx_valid_bytes;
    u32 hnc_rx_runt_pkts;
    u32 hnc_rx_jabber_pkts;
    u32 ncsi_rx_cmds;
    u32 ncsi_dropped_cmds;
    u32 ncsi_cmd_type_errs;
    u32 ncsi_cmd_csum_errs;
    u32 ncsi_rx_pkts;
    u32 ncsi_tx_pkts;
    u32 ncsi_tx_aen_pkts;
    u32 pt_tx_pkts;
    u32 pt_tx_dropped;
    u32 pt_tx_channel_err;
    u32 pt_tx_us_err;
    u32 pt_rx_pkts;
    u32 pt_rx_dropped;
    u32 pt_rx_channel_err;
    u32 pt_rx_us_err;
    u32 pt_rx_os_err;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
<b>Arch</b>
<ul>
<li>
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>armhf</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>riscv64</code> ✅
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
No changes between <code>generic</code> and <code>aws</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
