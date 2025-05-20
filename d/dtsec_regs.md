# Struct: <code>dtsec_regs</code>

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
struct dtsec_regs {
    u32 tsec_id;
    u32 tsec_id2;
    u32 ievent;
    u32 imask;
    u32 reserved0010[1];
    u32 ecntrl;
    u32 ptv;
    u32 tbipa;
    u32 tmr_ctrl;
    u32 tmr_pevent;
    u32 tmr_pemask;
    u32 reserved002c[5];
    u32 tctrl;
    u32 reserved0044[3];
    u32 rctrl;
    u32 reserved0054[11];
    u32 igaddr[8];
    u32 gaddr[8];
    u32 reserved00c0[16];
    u32 maccfg1;
    u32 maccfg2;
    u32 ipgifg;
    u32 hafdup;
    u32 maxfrm;
    u32 reserved0114[10];
    u32 ifstat;
    u32 macstnaddr1;
    u32 macstnaddr2;
    struct (anon) macaddr[15];
    u32 reserved01c0[16];
    u32 tr64;
    u32 tr127;
    u32 tr255;
    u32 tr511;
    u32 tr1k;
    u32 trmax;
    u32 trmgv;
    u32 rbyt;
    u32 rpkt;
    u32 rfcs;
    u32 rmca;
    u32 rbca;
    u32 rxcf;
    u32 rxpf;
    u32 rxuo;
    u32 raln;
    u32 rflr;
    u32 rcde;
    u32 rcse;
    u32 rund;
    u32 rovr;
    u32 rfrg;
    u32 rjbr;
    u32 rdrp;
    u32 tbyt;
    u32 tpkt;
    u32 tmca;
    u32 tbca;
    u32 txpf;
    u32 tdfr;
    u32 tedf;
    u32 tscl;
    u32 tmcl;
    u32 tlcl;
    u32 txcl;
    u32 tncl;
    u32 reserved0290[1];
    u32 tdrp;
    u32 tjbr;
    u32 tfcs;
    u32 txcf;
    u32 tovr;
    u32 tund;
    u32 tfrg;
    u32 car1;
    u32 car2;
    u32 cam1;
    u32 cam2;
    u32 reserved02c0[848];
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
