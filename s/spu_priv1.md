# Struct: <code>spu_priv1</code>

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
In <code>armhf</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct spu_priv1 {
    u64 mfc_sr1_RW;
    u64 mfc_lpid_RW;
    u64 spu_idr_RW;
    u64 mfc_vr_RO;
    u64 spu_vr_RO;
    u8 pad_0x28_0x100[216];
    u64 int_mask_RW[3];
    u8 pad_0x118_0x140[40];
    u64 int_stat_RW[3];
    u8 pad_0x158_0x180[40];
    u64 int_route_RW;
    u8 pad_0x188_0x200[120];
    u64 mfc_atomic_flush_RW;
    u8 pad_0x208_0x280[120];
    u64 resource_allocation_groupID_RW;
    u64 resource_allocation_enable_RW;
    u8 pad_0x290_0x3c8[312];
    u64 smf_sbi_signal_sel;
    u64 smf_ato_signal_sel;
    u8 pad_0x3d8_0x400[40];
    u64 mfc_sdr_RW;
    u8 pad_0x408_0x500[248];
    u64 tlb_index_hint_RO;
    u64 tlb_index_W;
    u64 tlb_vpn_RW;
    u64 tlb_rpn_RW;
    u8 pad_0x520_0x540[32];
    u64 tlb_invalidate_entry_W;
    u64 tlb_invalidate_all_W;
    u8 pad_0x550_0x580[48];
    u64 smm_hid;
    u8 pad_0x588_0x600[120];
    u64 mfc_accr_RW;
    u8 pad_0x608_0x610[8];
    u64 mfc_dsisr_RW;
    u8 pad_0x618_0x620[8];
    u64 mfc_dar_RW;
    u8 pad_0x628_0x700[216];
    u64 rmt_index_RW;
    u8 pad_0x708_0x710[8];
    u64 rmt_data1_RW;
    u8 pad_0x718_0x800[232];
    u64 mfc_dsir_R;
    u64 mfc_lsacr_RW;
    u64 mfc_lscrr_R;
    u8 pad_0x818_0x820[8];
    u64 mfc_tclass_id_RW;
    u8 pad_0x828_0x900[216];
    u64 mfc_rm_boundary;
    u8 pad_0x908_0x938[48];
    u64 smf_dma_signal_sel;
    u8 pad_0x940_0xa38[248];
    u64 smm_signal_sel;
    u8 pad_0xa40_0xc00[448];
    u64 mfc_cer_R;
    u8 pad_0xc08_0x1000[1016];
    u64 spu_ecc_cntl_RW;
    u64 spu_ecc_stat_RW;
    u64 spu_ecc_addr_RW;
    u64 spu_err_mask_RW;
    u8 pad_0x1020_0x1028[8];
    u64 spu_trig0_sel;
    u64 spu_trig1_sel;
    u64 spu_trig2_sel;
    u64 spu_trig3_sel;
    u64 spu_trace_sel;
    u64 spu_event0_sel;
    u64 spu_event1_sel;
    u64 spu_event2_sel;
    u64 spu_event3_sel;
    u64 spu_trace_cntl;
};
```
</details>
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
