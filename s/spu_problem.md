# Struct: <code>spu_problem</code>

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
struct spu_problem {
    u64 spc_mssync_RW;
    u8 pad_0x0008_0x3000[12280];
    u8 pad_0x3000_0x3004[4];
    u32 mfc_lsa_W;
    u64 mfc_ea_W;
    union mfc_tag_size_class_cmd mfc_union_W;
    u8 pad_0x3018_0x3104[236];
    u32 dma_qstatus_R;
    u8 pad_0x3108_0x3204[252];
    u32 dma_querytype_RW;
    u8 pad_0x3208_0x321c[20];
    u32 dma_querymask_RW;
    u8 pad_0x3220_0x322c[12];
    u32 dma_tagstatus_R;
    u8 pad_0x3230_0x4000[3536];
    u8 pad_0x4000_0x4004[4];
    u32 pu_mb_R;
    u8 pad_0x4008_0x400c[4];
    u32 spu_mb_W;
    u8 pad_0x4010_0x4014[4];
    u32 mb_stat_R;
    u8 pad_0x4018_0x401c[4];
    u32 spu_runcntl_RW;
    u8 pad_0x4020_0x4024[4];
    u32 spu_status_R;
    u8 pad_0x4028_0x402c[4];
    u32 spu_spe_R;
    u8 pad_0x4030_0x4034[4];
    u32 spu_npc_RW;
    u8 pad_0x4038_0x14000[65480];
    u8 pad_0x14000_0x1400c[12];
    u32 signal_notify1;
    u8 pad_0x14010_0x1c00c[32764];
    u32 signal_notify2;
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
