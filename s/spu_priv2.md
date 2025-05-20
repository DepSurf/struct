# Struct: <code>spu_priv2</code>

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
struct spu_priv2 {
    u8 pad_0x0000_0x1100[4352];
    u8 pad_0x1100_0x1108[8];
    u64 slb_index_W;
    u64 slb_esid_RW;
    u64 slb_vsid_RW;
    u64 slb_invalidate_entry_W;
    u64 slb_invalidate_all_W;
    u8 pad_0x1130_0x2000[3792];
    struct mfc_cq_sr spuq[16];
    struct mfc_cq_sr puq[8];
    u8 pad_0x2300_0x3000[3328];
    u64 mfc_control_RW;
    u8 pad_0x3008_0x4000[4088];
    u64 puint_mb_R;
    u8 pad_0x4008_0x4040[56];
    u64 spu_privcntl_RW;
    u8 pad_0x4048_0x4058[16];
    u64 spu_lslr_RW;
    u64 spu_chnlcntptr_RW;
    u64 spu_chnlcnt_RW;
    u64 spu_chnldata_RW;
    u64 spu_cfg_RW;
    u8 pad_0x4080_0x5000[3968];
    u64 spu_pm_trace_tag_status_RW;
    u64 spu_tag_status_query_RW;
    u64 spu_cmd_buf1_RW;
    u64 spu_cmd_buf2_RW;
    u64 spu_atomic_status_RW;
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
