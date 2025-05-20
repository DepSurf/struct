# Struct: <code>memac_regs</code>

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
struct memac_regs {
    u32 res0000[2];
    u32 command_config;
    struct mac_addr mac_addr0;
    u32 maxfrm;
    u32 res0018[1];
    u32 rx_fifo_sections;
    u32 tx_fifo_sections;
    u32 res0024[2];
    u32 hashtable_ctrl;
    u32 res0030[4];
    u32 ievent;
    u32 tx_ipg_length;
    u32 res0048;
    u32 imask;
    u32 res0050;
    u32 pause_quanta[4];
    u32 pause_thresh[4];
    u32 rx_pause_status;
    u32 res0078[2];
    struct mac_addr mac_addr[7];
    u32 lpwake_timer;
    u32 sleep_timer;
    u32 res00c0[8];
    u32 statn_config;
    u32 res00e4[7];
    u32 reoct_l;
    u32 reoct_u;
    u32 roct_l;
    u32 roct_u;
    u32 raln_l;
    u32 raln_u;
    u32 rxpf_l;
    u32 rxpf_u;
    u32 rfrm_l;
    u32 rfrm_u;
    u32 rfcs_l;
    u32 rfcs_u;
    u32 rvlan_l;
    u32 rvlan_u;
    u32 rerr_l;
    u32 rerr_u;
    u32 ruca_l;
    u32 ruca_u;
    u32 rmca_l;
    u32 rmca_u;
    u32 rbca_l;
    u32 rbca_u;
    u32 rdrp_l;
    u32 rdrp_u;
    u32 rpkt_l;
    u32 rpkt_u;
    u32 rund_l;
    u32 rund_u;
    u32 r64_l;
    u32 r64_u;
    u32 r127_l;
    u32 r127_u;
    u32 r255_l;
    u32 r255_u;
    u32 r511_l;
    u32 r511_u;
    u32 r1023_l;
    u32 r1023_u;
    u32 r1518_l;
    u32 r1518_u;
    u32 r1519x_l;
    u32 r1519x_u;
    u32 rovr_l;
    u32 rovr_u;
    u32 rjbr_l;
    u32 rjbr_u;
    u32 rfrg_l;
    u32 rfrg_u;
    u32 rcnp_l;
    u32 rcnp_u;
    u32 rdrntp_l;
    u32 rdrntp_u;
    u32 res01d0[12];
    u32 teoct_l;
    u32 teoct_u;
    u32 toct_l;
    u32 toct_u;
    u32 res0210[2];
    u32 txpf_l;
    u32 txpf_u;
    u32 tfrm_l;
    u32 tfrm_u;
    u32 tfcs_l;
    u32 tfcs_u;
    u32 tvlan_l;
    u32 tvlan_u;
    u32 terr_l;
    u32 terr_u;
    u32 tuca_l;
    u32 tuca_u;
    u32 tmca_l;
    u32 tmca_u;
    u32 tbca_l;
    u32 tbca_u;
    u32 res0258[2];
    u32 tpkt_l;
    u32 tpkt_u;
    u32 tund_l;
    u32 tund_u;
    u32 t64_l;
    u32 t64_u;
    u32 t127_l;
    u32 t127_u;
    u32 t255_l;
    u32 t255_u;
    u32 t511_l;
    u32 t511_u;
    u32 t1023_l;
    u32 t1023_u;
    u32 t1518_l;
    u32 t1518_u;
    u32 t1519x_l;
    u32 t1519x_u;
    u32 res02a8[6];
    u32 tcnp_l;
    u32 tcnp_u;
    u32 res02c8[14];
    u32 if_mode;
    u32 if_status;
    u32 res0308[14];
    u32 hg_config;
    u32 res0344[3];
    u32 hg_pause_quanta;
    u32 res0354[3];
    u32 hg_pause_thresh;
    u32 res0364[3];
    u32 hgrx_pause_status;
    u32 hg_fifos_status;
    u32 rhm;
    u32 thm;
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
