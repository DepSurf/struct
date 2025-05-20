# Struct: <code>ncsi_rsp_gcps_pkt</code>

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
struct ncsi_rsp_gcps_pkt {
    struct ncsi_rsp_pkt_hdr rsp;
    __be32 cnt_hi;
    __be32 cnt_lo;
    __be32 rx_bytes;
    __be32 tx_bytes;
    __be32 rx_uc_pkts;
    __be32 rx_mc_pkts;
    __be32 rx_bc_pkts;
    __be32 tx_uc_pkts;
    __be32 tx_mc_pkts;
    __be32 tx_bc_pkts;
    __be32 fcs_err;
    __be32 align_err;
    __be32 false_carrier;
    __be32 runt_pkts;
    __be32 jabber_pkts;
    __be32 rx_pause_xon;
    __be32 rx_pause_xoff;
    __be32 tx_pause_xon;
    __be32 tx_pause_xoff;
    __be32 tx_s_collision;
    __be32 tx_m_collision;
    __be32 l_collision;
    __be32 e_collision;
    __be32 rx_ctl_frames;
    __be32 rx_64_frames;
    __be32 rx_127_frames;
    __be32 rx_255_frames;
    __be32 rx_511_frames;
    __be32 rx_1023_frames;
    __be32 rx_1522_frames;
    __be32 rx_9022_frames;
    __be32 tx_64_frames;
    __be32 tx_127_frames;
    __be32 tx_255_frames;
    __be32 tx_511_frames;
    __be32 tx_1023_frames;
    __be32 tx_1522_frames;
    __be32 tx_9022_frames;
    __be32 rx_valid_bytes;
    __be32 rx_runt_pkts;
    __be32 rx_jabber_pkts;
    __be32 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ncsi_rsp_gcps_pkt {
    struct ncsi_rsp_pkt_hdr rsp;
    __be32 cnt_hi;
    __be32 cnt_lo;
    __be32 rx_bytes;
    __be32 tx_bytes;
    __be32 rx_uc_pkts;
    __be32 rx_mc_pkts;
    __be32 rx_bc_pkts;
    __be32 tx_uc_pkts;
    __be32 tx_mc_pkts;
    __be32 tx_bc_pkts;
    __be32 fcs_err;
    __be32 align_err;
    __be32 false_carrier;
    __be32 runt_pkts;
    __be32 jabber_pkts;
    __be32 rx_pause_xon;
    __be32 rx_pause_xoff;
    __be32 tx_pause_xon;
    __be32 tx_pause_xoff;
    __be32 tx_s_collision;
    __be32 tx_m_collision;
    __be32 l_collision;
    __be32 e_collision;
    __be32 rx_ctl_frames;
    __be32 rx_64_frames;
    __be32 rx_127_frames;
    __be32 rx_255_frames;
    __be32 rx_511_frames;
    __be32 rx_1023_frames;
    __be32 rx_1522_frames;
    __be32 rx_9022_frames;
    __be32 tx_64_frames;
    __be32 tx_127_frames;
    __be32 tx_255_frames;
    __be32 tx_511_frames;
    __be32 tx_1023_frames;
    __be32 tx_1522_frames;
    __be32 tx_9022_frames;
    __be32 rx_valid_bytes;
    __be32 rx_runt_pkts;
    __be32 rx_jabber_pkts;
    __be32 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ncsi_rsp_gcps_pkt {
    struct ncsi_rsp_pkt_hdr rsp;
    __be32 cnt_hi;
    __be32 cnt_lo;
    __be32 rx_bytes;
    __be32 tx_bytes;
    __be32 rx_uc_pkts;
    __be32 rx_mc_pkts;
    __be32 rx_bc_pkts;
    __be32 tx_uc_pkts;
    __be32 tx_mc_pkts;
    __be32 tx_bc_pkts;
    __be32 fcs_err;
    __be32 align_err;
    __be32 false_carrier;
    __be32 runt_pkts;
    __be32 jabber_pkts;
    __be32 rx_pause_xon;
    __be32 rx_pause_xoff;
    __be32 tx_pause_xon;
    __be32 tx_pause_xoff;
    __be32 tx_s_collision;
    __be32 tx_m_collision;
    __be32 l_collision;
    __be32 e_collision;
    __be32 rx_ctl_frames;
    __be32 rx_64_frames;
    __be32 rx_127_frames;
    __be32 rx_255_frames;
    __be32 rx_511_frames;
    __be32 rx_1023_frames;
    __be32 rx_1522_frames;
    __be32 rx_9022_frames;
    __be32 tx_64_frames;
    __be32 tx_127_frames;
    __be32 tx_255_frames;
    __be32 tx_511_frames;
    __be32 tx_1023_frames;
    __be32 tx_1522_frames;
    __be32 tx_9022_frames;
    __be32 rx_valid_bytes;
    __be32 rx_runt_pkts;
    __be32 rx_jabber_pkts;
    __be32 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ncsi_rsp_gcps_pkt {
    struct ncsi_rsp_pkt_hdr rsp;
    __be32 cnt_hi;
    __be32 cnt_lo;
    __be32 rx_bytes;
    __be32 tx_bytes;
    __be32 rx_uc_pkts;
    __be32 rx_mc_pkts;
    __be32 rx_bc_pkts;
    __be32 tx_uc_pkts;
    __be32 tx_mc_pkts;
    __be32 tx_bc_pkts;
    __be32 fcs_err;
    __be32 align_err;
    __be32 false_carrier;
    __be32 runt_pkts;
    __be32 jabber_pkts;
    __be32 rx_pause_xon;
    __be32 rx_pause_xoff;
    __be32 tx_pause_xon;
    __be32 tx_pause_xoff;
    __be32 tx_s_collision;
    __be32 tx_m_collision;
    __be32 l_collision;
    __be32 e_collision;
    __be32 rx_ctl_frames;
    __be32 rx_64_frames;
    __be32 rx_127_frames;
    __be32 rx_255_frames;
    __be32 rx_511_frames;
    __be32 rx_1023_frames;
    __be32 rx_1522_frames;
    __be32 rx_9022_frames;
    __be32 tx_64_frames;
    __be32 tx_127_frames;
    __be32 tx_255_frames;
    __be32 tx_511_frames;
    __be32 tx_1023_frames;
    __be32 tx_1522_frames;
    __be32 tx_9022_frames;
    __be32 rx_valid_bytes;
    __be32 rx_runt_pkts;
    __be32 rx_jabber_pkts;
    __be32 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ncsi_rsp_gcps_pkt {
    struct ncsi_rsp_pkt_hdr rsp;
    __be32 cnt_hi;
    __be32 cnt_lo;
    __be32 rx_bytes;
    __be32 tx_bytes;
    __be32 rx_uc_pkts;
    __be32 rx_mc_pkts;
    __be32 rx_bc_pkts;
    __be32 tx_uc_pkts;
    __be32 tx_mc_pkts;
    __be32 tx_bc_pkts;
    __be32 fcs_err;
    __be32 align_err;
    __be32 false_carrier;
    __be32 runt_pkts;
    __be32 jabber_pkts;
    __be32 rx_pause_xon;
    __be32 rx_pause_xoff;
    __be32 tx_pause_xon;
    __be32 tx_pause_xoff;
    __be32 tx_s_collision;
    __be32 tx_m_collision;
    __be32 l_collision;
    __be32 e_collision;
    __be32 rx_ctl_frames;
    __be32 rx_64_frames;
    __be32 rx_127_frames;
    __be32 rx_255_frames;
    __be32 rx_511_frames;
    __be32 rx_1023_frames;
    __be32 rx_1522_frames;
    __be32 rx_9022_frames;
    __be32 tx_64_frames;
    __be32 tx_127_frames;
    __be32 tx_255_frames;
    __be32 tx_511_frames;
    __be32 tx_1023_frames;
    __be32 tx_1522_frames;
    __be32 tx_9022_frames;
    __be32 rx_valid_bytes;
    __be32 rx_runt_pkts;
    __be32 rx_jabber_pkts;
    __be32 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ncsi_rsp_gcps_pkt {
    struct ncsi_rsp_pkt_hdr rsp;
    __be32 cnt_hi;
    __be32 cnt_lo;
    __be32 rx_bytes;
    __be32 tx_bytes;
    __be32 rx_uc_pkts;
    __be32 rx_mc_pkts;
    __be32 rx_bc_pkts;
    __be32 tx_uc_pkts;
    __be32 tx_mc_pkts;
    __be32 tx_bc_pkts;
    __be32 fcs_err;
    __be32 align_err;
    __be32 false_carrier;
    __be32 runt_pkts;
    __be32 jabber_pkts;
    __be32 rx_pause_xon;
    __be32 rx_pause_xoff;
    __be32 tx_pause_xon;
    __be32 tx_pause_xoff;
    __be32 tx_s_collision;
    __be32 tx_m_collision;
    __be32 l_collision;
    __be32 e_collision;
    __be32 rx_ctl_frames;
    __be32 rx_64_frames;
    __be32 rx_127_frames;
    __be32 rx_255_frames;
    __be32 rx_511_frames;
    __be32 rx_1023_frames;
    __be32 rx_1522_frames;
    __be32 rx_9022_frames;
    __be32 tx_64_frames;
    __be32 tx_127_frames;
    __be32 tx_255_frames;
    __be32 tx_511_frames;
    __be32 tx_1023_frames;
    __be32 tx_1522_frames;
    __be32 tx_9022_frames;
    __be32 rx_valid_bytes;
    __be32 rx_runt_pkts;
    __be32 rx_jabber_pkts;
    __be32 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ncsi_rsp_gcps_pkt {
    struct ncsi_rsp_pkt_hdr rsp;
    __be32 cnt_hi;
    __be32 cnt_lo;
    __be32 rx_bytes;
    __be32 tx_bytes;
    __be32 rx_uc_pkts;
    __be32 rx_mc_pkts;
    __be32 rx_bc_pkts;
    __be32 tx_uc_pkts;
    __be32 tx_mc_pkts;
    __be32 tx_bc_pkts;
    __be32 fcs_err;
    __be32 align_err;
    __be32 false_carrier;
    __be32 runt_pkts;
    __be32 jabber_pkts;
    __be32 rx_pause_xon;
    __be32 rx_pause_xoff;
    __be32 tx_pause_xon;
    __be32 tx_pause_xoff;
    __be32 tx_s_collision;
    __be32 tx_m_collision;
    __be32 l_collision;
    __be32 e_collision;
    __be32 rx_ctl_frames;
    __be32 rx_64_frames;
    __be32 rx_127_frames;
    __be32 rx_255_frames;
    __be32 rx_511_frames;
    __be32 rx_1023_frames;
    __be32 rx_1522_frames;
    __be32 rx_9022_frames;
    __be32 tx_64_frames;
    __be32 tx_127_frames;
    __be32 tx_255_frames;
    __be32 tx_511_frames;
    __be32 tx_1023_frames;
    __be32 tx_1522_frames;
    __be32 tx_9022_frames;
    __be32 rx_valid_bytes;
    __be32 rx_runt_pkts;
    __be32 rx_jabber_pkts;
    __be32 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ncsi_rsp_gcps_pkt {
    struct ncsi_rsp_pkt_hdr rsp;
    __be32 cnt_hi;
    __be32 cnt_lo;
    __be32 rx_bytes;
    __be32 tx_bytes;
    __be32 rx_uc_pkts;
    __be32 rx_mc_pkts;
    __be32 rx_bc_pkts;
    __be32 tx_uc_pkts;
    __be32 tx_mc_pkts;
    __be32 tx_bc_pkts;
    __be32 fcs_err;
    __be32 align_err;
    __be32 false_carrier;
    __be32 runt_pkts;
    __be32 jabber_pkts;
    __be32 rx_pause_xon;
    __be32 rx_pause_xoff;
    __be32 tx_pause_xon;
    __be32 tx_pause_xoff;
    __be32 tx_s_collision;
    __be32 tx_m_collision;
    __be32 l_collision;
    __be32 e_collision;
    __be32 rx_ctl_frames;
    __be32 rx_64_frames;
    __be32 rx_127_frames;
    __be32 rx_255_frames;
    __be32 rx_511_frames;
    __be32 rx_1023_frames;
    __be32 rx_1522_frames;
    __be32 rx_9022_frames;
    __be32 tx_64_frames;
    __be32 tx_127_frames;
    __be32 tx_255_frames;
    __be32 tx_511_frames;
    __be32 tx_1023_frames;
    __be32 tx_1522_frames;
    __be32 tx_9022_frames;
    __be32 rx_valid_bytes;
    __be32 rx_runt_pkts;
    __be32 rx_jabber_pkts;
    __be32 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ncsi_rsp_gcps_pkt {
    struct ncsi_rsp_pkt_hdr rsp;
    __be32 cnt_hi;
    __be32 cnt_lo;
    __be32 rx_bytes;
    __be32 tx_bytes;
    __be32 rx_uc_pkts;
    __be32 rx_mc_pkts;
    __be32 rx_bc_pkts;
    __be32 tx_uc_pkts;
    __be32 tx_mc_pkts;
    __be32 tx_bc_pkts;
    __be32 fcs_err;
    __be32 align_err;
    __be32 false_carrier;
    __be32 runt_pkts;
    __be32 jabber_pkts;
    __be32 rx_pause_xon;
    __be32 rx_pause_xoff;
    __be32 tx_pause_xon;
    __be32 tx_pause_xoff;
    __be32 tx_s_collision;
    __be32 tx_m_collision;
    __be32 l_collision;
    __be32 e_collision;
    __be32 rx_ctl_frames;
    __be32 rx_64_frames;
    __be32 rx_127_frames;
    __be32 rx_255_frames;
    __be32 rx_511_frames;
    __be32 rx_1023_frames;
    __be32 rx_1522_frames;
    __be32 rx_9022_frames;
    __be32 tx_64_frames;
    __be32 tx_127_frames;
    __be32 tx_255_frames;
    __be32 tx_511_frames;
    __be32 tx_1023_frames;
    __be32 tx_1522_frames;
    __be32 tx_9022_frames;
    __be32 rx_valid_bytes;
    __be32 rx_runt_pkts;
    __be32 rx_jabber_pkts;
    __be32 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ncsi_rsp_gcps_pkt {
    struct ncsi_rsp_pkt_hdr rsp;
    __be32 cnt_hi;
    __be32 cnt_lo;
    __be32 rx_bytes;
    __be32 tx_bytes;
    __be32 rx_uc_pkts;
    __be32 rx_mc_pkts;
    __be32 rx_bc_pkts;
    __be32 tx_uc_pkts;
    __be32 tx_mc_pkts;
    __be32 tx_bc_pkts;
    __be32 fcs_err;
    __be32 align_err;
    __be32 false_carrier;
    __be32 runt_pkts;
    __be32 jabber_pkts;
    __be32 rx_pause_xon;
    __be32 rx_pause_xoff;
    __be32 tx_pause_xon;
    __be32 tx_pause_xoff;
    __be32 tx_s_collision;
    __be32 tx_m_collision;
    __be32 l_collision;
    __be32 e_collision;
    __be32 rx_ctl_frames;
    __be32 rx_64_frames;
    __be32 rx_127_frames;
    __be32 rx_255_frames;
    __be32 rx_511_frames;
    __be32 rx_1023_frames;
    __be32 rx_1522_frames;
    __be32 rx_9022_frames;
    __be32 tx_64_frames;
    __be32 tx_127_frames;
    __be32 tx_255_frames;
    __be32 tx_511_frames;
    __be32 tx_1023_frames;
    __be32 tx_1522_frames;
    __be32 tx_9022_frames;
    __be32 rx_valid_bytes;
    __be32 rx_runt_pkts;
    __be32 rx_jabber_pkts;
    __be32 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ncsi_rsp_gcps_pkt {
    struct ncsi_rsp_pkt_hdr rsp;
    __be32 cnt_hi;
    __be32 cnt_lo;
    __be32 rx_bytes;
    __be32 tx_bytes;
    __be32 rx_uc_pkts;
    __be32 rx_mc_pkts;
    __be32 rx_bc_pkts;
    __be32 tx_uc_pkts;
    __be32 tx_mc_pkts;
    __be32 tx_bc_pkts;
    __be32 fcs_err;
    __be32 align_err;
    __be32 false_carrier;
    __be32 runt_pkts;
    __be32 jabber_pkts;
    __be32 rx_pause_xon;
    __be32 rx_pause_xoff;
    __be32 tx_pause_xon;
    __be32 tx_pause_xoff;
    __be32 tx_s_collision;
    __be32 tx_m_collision;
    __be32 l_collision;
    __be32 e_collision;
    __be32 rx_ctl_frames;
    __be32 rx_64_frames;
    __be32 rx_127_frames;
    __be32 rx_255_frames;
    __be32 rx_511_frames;
    __be32 rx_1023_frames;
    __be32 rx_1522_frames;
    __be32 rx_9022_frames;
    __be32 tx_64_frames;
    __be32 tx_127_frames;
    __be32 tx_255_frames;
    __be32 tx_511_frames;
    __be32 tx_1023_frames;
    __be32 tx_1522_frames;
    __be32 tx_9022_frames;
    __be32 rx_valid_bytes;
    __be32 rx_runt_pkts;
    __be32 rx_jabber_pkts;
    __be32 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ncsi_rsp_gcps_pkt {
    struct ncsi_rsp_pkt_hdr rsp;
    __be32 cnt_hi;
    __be32 cnt_lo;
    __be32 rx_bytes;
    __be32 tx_bytes;
    __be32 rx_uc_pkts;
    __be32 rx_mc_pkts;
    __be32 rx_bc_pkts;
    __be32 tx_uc_pkts;
    __be32 tx_mc_pkts;
    __be32 tx_bc_pkts;
    __be32 fcs_err;
    __be32 align_err;
    __be32 false_carrier;
    __be32 runt_pkts;
    __be32 jabber_pkts;
    __be32 rx_pause_xon;
    __be32 rx_pause_xoff;
    __be32 tx_pause_xon;
    __be32 tx_pause_xoff;
    __be32 tx_s_collision;
    __be32 tx_m_collision;
    __be32 l_collision;
    __be32 e_collision;
    __be32 rx_ctl_frames;
    __be32 rx_64_frames;
    __be32 rx_127_frames;
    __be32 rx_255_frames;
    __be32 rx_511_frames;
    __be32 rx_1023_frames;
    __be32 rx_1522_frames;
    __be32 rx_9022_frames;
    __be32 tx_64_frames;
    __be32 tx_127_frames;
    __be32 tx_255_frames;
    __be32 tx_511_frames;
    __be32 tx_1023_frames;
    __be32 tx_1522_frames;
    __be32 tx_9022_frames;
    __be32 rx_valid_bytes;
    __be32 rx_runt_pkts;
    __be32 rx_jabber_pkts;
    __be32 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ncsi_rsp_gcps_pkt {
    struct ncsi_rsp_pkt_hdr rsp;
    __be32 cnt_hi;
    __be32 cnt_lo;
    __be32 rx_bytes;
    __be32 tx_bytes;
    __be32 rx_uc_pkts;
    __be32 rx_mc_pkts;
    __be32 rx_bc_pkts;
    __be32 tx_uc_pkts;
    __be32 tx_mc_pkts;
    __be32 tx_bc_pkts;
    __be32 fcs_err;
    __be32 align_err;
    __be32 false_carrier;
    __be32 runt_pkts;
    __be32 jabber_pkts;
    __be32 rx_pause_xon;
    __be32 rx_pause_xoff;
    __be32 tx_pause_xon;
    __be32 tx_pause_xoff;
    __be32 tx_s_collision;
    __be32 tx_m_collision;
    __be32 l_collision;
    __be32 e_collision;
    __be32 rx_ctl_frames;
    __be32 rx_64_frames;
    __be32 rx_127_frames;
    __be32 rx_255_frames;
    __be32 rx_511_frames;
    __be32 rx_1023_frames;
    __be32 rx_1522_frames;
    __be32 rx_9022_frames;
    __be32 tx_64_frames;
    __be32 tx_127_frames;
    __be32 tx_255_frames;
    __be32 tx_511_frames;
    __be32 tx_1023_frames;
    __be32 tx_1522_frames;
    __be32 tx_9022_frames;
    __be32 rx_valid_bytes;
    __be32 rx_runt_pkts;
    __be32 rx_jabber_pkts;
    __be32 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ncsi_rsp_gcps_pkt {
    struct ncsi_rsp_pkt_hdr rsp;
    __be32 cnt_hi;
    __be32 cnt_lo;
    __be32 rx_bytes;
    __be32 tx_bytes;
    __be32 rx_uc_pkts;
    __be32 rx_mc_pkts;
    __be32 rx_bc_pkts;
    __be32 tx_uc_pkts;
    __be32 tx_mc_pkts;
    __be32 tx_bc_pkts;
    __be32 fcs_err;
    __be32 align_err;
    __be32 false_carrier;
    __be32 runt_pkts;
    __be32 jabber_pkts;
    __be32 rx_pause_xon;
    __be32 rx_pause_xoff;
    __be32 tx_pause_xon;
    __be32 tx_pause_xoff;
    __be32 tx_s_collision;
    __be32 tx_m_collision;
    __be32 l_collision;
    __be32 e_collision;
    __be32 rx_ctl_frames;
    __be32 rx_64_frames;
    __be32 rx_127_frames;
    __be32 rx_255_frames;
    __be32 rx_511_frames;
    __be32 rx_1023_frames;
    __be32 rx_1522_frames;
    __be32 rx_9022_frames;
    __be32 tx_64_frames;
    __be32 tx_127_frames;
    __be32 tx_255_frames;
    __be32 tx_511_frames;
    __be32 tx_1023_frames;
    __be32 tx_1522_frames;
    __be32 tx_9022_frames;
    __be32 rx_valid_bytes;
    __be32 rx_runt_pkts;
    __be32 rx_jabber_pkts;
    __be32 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ncsi_rsp_gcps_pkt {
    struct ncsi_rsp_pkt_hdr rsp;
    __be32 cnt_hi;
    __be32 cnt_lo;
    __be32 rx_bytes;
    __be32 tx_bytes;
    __be32 rx_uc_pkts;
    __be32 rx_mc_pkts;
    __be32 rx_bc_pkts;
    __be32 tx_uc_pkts;
    __be32 tx_mc_pkts;
    __be32 tx_bc_pkts;
    __be32 fcs_err;
    __be32 align_err;
    __be32 false_carrier;
    __be32 runt_pkts;
    __be32 jabber_pkts;
    __be32 rx_pause_xon;
    __be32 rx_pause_xoff;
    __be32 tx_pause_xon;
    __be32 tx_pause_xoff;
    __be32 tx_s_collision;
    __be32 tx_m_collision;
    __be32 l_collision;
    __be32 e_collision;
    __be32 rx_ctl_frames;
    __be32 rx_64_frames;
    __be32 rx_127_frames;
    __be32 rx_255_frames;
    __be32 rx_511_frames;
    __be32 rx_1023_frames;
    __be32 rx_1522_frames;
    __be32 rx_9022_frames;
    __be32 tx_64_frames;
    __be32 tx_127_frames;
    __be32 tx_255_frames;
    __be32 tx_511_frames;
    __be32 tx_1023_frames;
    __be32 tx_1522_frames;
    __be32 tx_9022_frames;
    __be32 rx_valid_bytes;
    __be32 rx_runt_pkts;
    __be32 rx_jabber_pkts;
    __be32 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ncsi_rsp_gcps_pkt {
    struct ncsi_rsp_pkt_hdr rsp;
    __be32 cnt_hi;
    __be32 cnt_lo;
    __be32 rx_bytes;
    __be32 tx_bytes;
    __be32 rx_uc_pkts;
    __be32 rx_mc_pkts;
    __be32 rx_bc_pkts;
    __be32 tx_uc_pkts;
    __be32 tx_mc_pkts;
    __be32 tx_bc_pkts;
    __be32 fcs_err;
    __be32 align_err;
    __be32 false_carrier;
    __be32 runt_pkts;
    __be32 jabber_pkts;
    __be32 rx_pause_xon;
    __be32 rx_pause_xoff;
    __be32 tx_pause_xon;
    __be32 tx_pause_xoff;
    __be32 tx_s_collision;
    __be32 tx_m_collision;
    __be32 l_collision;
    __be32 e_collision;
    __be32 rx_ctl_frames;
    __be32 rx_64_frames;
    __be32 rx_127_frames;
    __be32 rx_255_frames;
    __be32 rx_511_frames;
    __be32 rx_1023_frames;
    __be32 rx_1522_frames;
    __be32 rx_9022_frames;
    __be32 tx_64_frames;
    __be32 tx_127_frames;
    __be32 tx_255_frames;
    __be32 tx_511_frames;
    __be32 tx_1023_frames;
    __be32 tx_1522_frames;
    __be32 tx_9022_frames;
    __be32 rx_valid_bytes;
    __be32 rx_runt_pkts;
    __be32 rx_jabber_pkts;
    __be32 checksum;
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
struct ncsi_rsp_gcps_pkt {
    struct ncsi_rsp_pkt_hdr rsp;
    __be32 cnt_hi;
    __be32 cnt_lo;
    __be32 rx_bytes;
    __be32 tx_bytes;
    __be32 rx_uc_pkts;
    __be32 rx_mc_pkts;
    __be32 rx_bc_pkts;
    __be32 tx_uc_pkts;
    __be32 tx_mc_pkts;
    __be32 tx_bc_pkts;
    __be32 fcs_err;
    __be32 align_err;
    __be32 false_carrier;
    __be32 runt_pkts;
    __be32 jabber_pkts;
    __be32 rx_pause_xon;
    __be32 rx_pause_xoff;
    __be32 tx_pause_xon;
    __be32 tx_pause_xoff;
    __be32 tx_s_collision;
    __be32 tx_m_collision;
    __be32 l_collision;
    __be32 e_collision;
    __be32 rx_ctl_frames;
    __be32 rx_64_frames;
    __be32 rx_127_frames;
    __be32 rx_255_frames;
    __be32 rx_511_frames;
    __be32 rx_1023_frames;
    __be32 rx_1522_frames;
    __be32 rx_9022_frames;
    __be32 tx_64_frames;
    __be32 tx_127_frames;
    __be32 tx_255_frames;
    __be32 tx_511_frames;
    __be32 tx_1023_frames;
    __be32 tx_1522_frames;
    __be32 tx_9022_frames;
    __be32 rx_valid_bytes;
    __be32 rx_runt_pkts;
    __be32 rx_jabber_pkts;
    __be32 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ncsi_rsp_gcps_pkt {
    struct ncsi_rsp_pkt_hdr rsp;
    __be32 cnt_hi;
    __be32 cnt_lo;
    __be32 rx_bytes;
    __be32 tx_bytes;
    __be32 rx_uc_pkts;
    __be32 rx_mc_pkts;
    __be32 rx_bc_pkts;
    __be32 tx_uc_pkts;
    __be32 tx_mc_pkts;
    __be32 tx_bc_pkts;
    __be32 fcs_err;
    __be32 align_err;
    __be32 false_carrier;
    __be32 runt_pkts;
    __be32 jabber_pkts;
    __be32 rx_pause_xon;
    __be32 rx_pause_xoff;
    __be32 tx_pause_xon;
    __be32 tx_pause_xoff;
    __be32 tx_s_collision;
    __be32 tx_m_collision;
    __be32 l_collision;
    __be32 e_collision;
    __be32 rx_ctl_frames;
    __be32 rx_64_frames;
    __be32 rx_127_frames;
    __be32 rx_255_frames;
    __be32 rx_511_frames;
    __be32 rx_1023_frames;
    __be32 rx_1522_frames;
    __be32 rx_9022_frames;
    __be32 tx_64_frames;
    __be32 tx_127_frames;
    __be32 tx_255_frames;
    __be32 tx_511_frames;
    __be32 tx_1023_frames;
    __be32 tx_1522_frames;
    __be32 tx_9022_frames;
    __be32 rx_valid_bytes;
    __be32 rx_runt_pkts;
    __be32 rx_jabber_pkts;
    __be32 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ncsi_rsp_gcps_pkt {
    struct ncsi_rsp_pkt_hdr rsp;
    __be32 cnt_hi;
    __be32 cnt_lo;
    __be32 rx_bytes;
    __be32 tx_bytes;
    __be32 rx_uc_pkts;
    __be32 rx_mc_pkts;
    __be32 rx_bc_pkts;
    __be32 tx_uc_pkts;
    __be32 tx_mc_pkts;
    __be32 tx_bc_pkts;
    __be32 fcs_err;
    __be32 align_err;
    __be32 false_carrier;
    __be32 runt_pkts;
    __be32 jabber_pkts;
    __be32 rx_pause_xon;
    __be32 rx_pause_xoff;
    __be32 tx_pause_xon;
    __be32 tx_pause_xoff;
    __be32 tx_s_collision;
    __be32 tx_m_collision;
    __be32 l_collision;
    __be32 e_collision;
    __be32 rx_ctl_frames;
    __be32 rx_64_frames;
    __be32 rx_127_frames;
    __be32 rx_255_frames;
    __be32 rx_511_frames;
    __be32 rx_1023_frames;
    __be32 rx_1522_frames;
    __be32 rx_9022_frames;
    __be32 tx_64_frames;
    __be32 tx_127_frames;
    __be32 tx_255_frames;
    __be32 tx_511_frames;
    __be32 tx_1023_frames;
    __be32 tx_1522_frames;
    __be32 tx_9022_frames;
    __be32 rx_valid_bytes;
    __be32 rx_runt_pkts;
    __be32 rx_jabber_pkts;
    __be32 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ncsi_rsp_gcps_pkt {
    struct ncsi_rsp_pkt_hdr rsp;
    __be32 cnt_hi;
    __be32 cnt_lo;
    __be32 rx_bytes;
    __be32 tx_bytes;
    __be32 rx_uc_pkts;
    __be32 rx_mc_pkts;
    __be32 rx_bc_pkts;
    __be32 tx_uc_pkts;
    __be32 tx_mc_pkts;
    __be32 tx_bc_pkts;
    __be32 fcs_err;
    __be32 align_err;
    __be32 false_carrier;
    __be32 runt_pkts;
    __be32 jabber_pkts;
    __be32 rx_pause_xon;
    __be32 rx_pause_xoff;
    __be32 tx_pause_xon;
    __be32 tx_pause_xoff;
    __be32 tx_s_collision;
    __be32 tx_m_collision;
    __be32 l_collision;
    __be32 e_collision;
    __be32 rx_ctl_frames;
    __be32 rx_64_frames;
    __be32 rx_127_frames;
    __be32 rx_255_frames;
    __be32 rx_511_frames;
    __be32 rx_1023_frames;
    __be32 rx_1522_frames;
    __be32 rx_9022_frames;
    __be32 tx_64_frames;
    __be32 tx_127_frames;
    __be32 tx_255_frames;
    __be32 tx_511_frames;
    __be32 tx_1023_frames;
    __be32 tx_1522_frames;
    __be32 tx_9022_frames;
    __be32 rx_valid_bytes;
    __be32 rx_runt_pkts;
    __be32 rx_jabber_pkts;
    __be32 checksum;
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
struct ncsi_rsp_gcps_pkt {
    struct ncsi_rsp_pkt_hdr rsp;
    __be32 cnt_hi;
    __be32 cnt_lo;
    __be32 rx_bytes;
    __be32 tx_bytes;
    __be32 rx_uc_pkts;
    __be32 rx_mc_pkts;
    __be32 rx_bc_pkts;
    __be32 tx_uc_pkts;
    __be32 tx_mc_pkts;
    __be32 tx_bc_pkts;
    __be32 fcs_err;
    __be32 align_err;
    __be32 false_carrier;
    __be32 runt_pkts;
    __be32 jabber_pkts;
    __be32 rx_pause_xon;
    __be32 rx_pause_xoff;
    __be32 tx_pause_xon;
    __be32 tx_pause_xoff;
    __be32 tx_s_collision;
    __be32 tx_m_collision;
    __be32 l_collision;
    __be32 e_collision;
    __be32 rx_ctl_frames;
    __be32 rx_64_frames;
    __be32 rx_127_frames;
    __be32 rx_255_frames;
    __be32 rx_511_frames;
    __be32 rx_1023_frames;
    __be32 rx_1522_frames;
    __be32 rx_9022_frames;
    __be32 tx_64_frames;
    __be32 tx_127_frames;
    __be32 tx_255_frames;
    __be32 tx_511_frames;
    __be32 tx_1023_frames;
    __be32 tx_1522_frames;
    __be32 tx_9022_frames;
    __be32 rx_valid_bytes;
    __be32 rx_runt_pkts;
    __be32 rx_jabber_pkts;
    __be32 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ncsi_rsp_gcps_pkt {
    struct ncsi_rsp_pkt_hdr rsp;
    __be32 cnt_hi;
    __be32 cnt_lo;
    __be32 rx_bytes;
    __be32 tx_bytes;
    __be32 rx_uc_pkts;
    __be32 rx_mc_pkts;
    __be32 rx_bc_pkts;
    __be32 tx_uc_pkts;
    __be32 tx_mc_pkts;
    __be32 tx_bc_pkts;
    __be32 fcs_err;
    __be32 align_err;
    __be32 false_carrier;
    __be32 runt_pkts;
    __be32 jabber_pkts;
    __be32 rx_pause_xon;
    __be32 rx_pause_xoff;
    __be32 tx_pause_xon;
    __be32 tx_pause_xoff;
    __be32 tx_s_collision;
    __be32 tx_m_collision;
    __be32 l_collision;
    __be32 e_collision;
    __be32 rx_ctl_frames;
    __be32 rx_64_frames;
    __be32 rx_127_frames;
    __be32 rx_255_frames;
    __be32 rx_511_frames;
    __be32 rx_1023_frames;
    __be32 rx_1522_frames;
    __be32 rx_9022_frames;
    __be32 tx_64_frames;
    __be32 tx_127_frames;
    __be32 tx_255_frames;
    __be32 tx_511_frames;
    __be32 tx_1023_frames;
    __be32 tx_1522_frames;
    __be32 tx_9022_frames;
    __be32 rx_valid_bytes;
    __be32 rx_runt_pkts;
    __be32 rx_jabber_pkts;
    __be32 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ncsi_rsp_gcps_pkt {
    struct ncsi_rsp_pkt_hdr rsp;
    __be32 cnt_hi;
    __be32 cnt_lo;
    __be32 rx_bytes;
    __be32 tx_bytes;
    __be32 rx_uc_pkts;
    __be32 rx_mc_pkts;
    __be32 rx_bc_pkts;
    __be32 tx_uc_pkts;
    __be32 tx_mc_pkts;
    __be32 tx_bc_pkts;
    __be32 fcs_err;
    __be32 align_err;
    __be32 false_carrier;
    __be32 runt_pkts;
    __be32 jabber_pkts;
    __be32 rx_pause_xon;
    __be32 rx_pause_xoff;
    __be32 tx_pause_xon;
    __be32 tx_pause_xoff;
    __be32 tx_s_collision;
    __be32 tx_m_collision;
    __be32 l_collision;
    __be32 e_collision;
    __be32 rx_ctl_frames;
    __be32 rx_64_frames;
    __be32 rx_127_frames;
    __be32 rx_255_frames;
    __be32 rx_511_frames;
    __be32 rx_1023_frames;
    __be32 rx_1522_frames;
    __be32 rx_9022_frames;
    __be32 tx_64_frames;
    __be32 tx_127_frames;
    __be32 tx_255_frames;
    __be32 tx_511_frames;
    __be32 tx_1023_frames;
    __be32 tx_1522_frames;
    __be32 tx_9022_frames;
    __be32 rx_valid_bytes;
    __be32 rx_runt_pkts;
    __be32 rx_jabber_pkts;
    __be32 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ncsi_rsp_gcps_pkt {
    struct ncsi_rsp_pkt_hdr rsp;
    __be32 cnt_hi;
    __be32 cnt_lo;
    __be32 rx_bytes;
    __be32 tx_bytes;
    __be32 rx_uc_pkts;
    __be32 rx_mc_pkts;
    __be32 rx_bc_pkts;
    __be32 tx_uc_pkts;
    __be32 tx_mc_pkts;
    __be32 tx_bc_pkts;
    __be32 fcs_err;
    __be32 align_err;
    __be32 false_carrier;
    __be32 runt_pkts;
    __be32 jabber_pkts;
    __be32 rx_pause_xon;
    __be32 rx_pause_xoff;
    __be32 tx_pause_xon;
    __be32 tx_pause_xoff;
    __be32 tx_s_collision;
    __be32 tx_m_collision;
    __be32 l_collision;
    __be32 e_collision;
    __be32 rx_ctl_frames;
    __be32 rx_64_frames;
    __be32 rx_127_frames;
    __be32 rx_255_frames;
    __be32 rx_511_frames;
    __be32 rx_1023_frames;
    __be32 rx_1522_frames;
    __be32 rx_9022_frames;
    __be32 tx_64_frames;
    __be32 tx_127_frames;
    __be32 tx_255_frames;
    __be32 tx_511_frames;
    __be32 tx_1023_frames;
    __be32 tx_1522_frames;
    __be32 tx_9022_frames;
    __be32 rx_valid_bytes;
    __be32 rx_runt_pkts;
    __be32 rx_jabber_pkts;
    __be32 checksum;
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
