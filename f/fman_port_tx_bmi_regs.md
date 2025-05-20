# Struct: <code>fman_port_tx_bmi_regs</code>

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
struct fman_port_tx_bmi_regs {
    u32 fmbm_tcfg;
    u32 fmbm_tst;
    u32 fmbm_tda;
    u32 fmbm_tfp;
    u32 fmbm_tfed;
    u32 fmbm_ticp;
    u32 fmbm_tfdne;
    u32 fmbm_tfca;
    u32 fmbm_tcfqid;
    u32 fmbm_tefqid;
    u32 fmbm_tfene;
    u32 fmbm_trlmts;
    u32 fmbm_trlmt;
    u32 reserved0034[14];
    u32 fmbm_tccb;
    u32 fmbm_tfne;
    u32 fmbm_tpfcm[2];
    u32 fmbm_tcmne;
    u32 reserved0080[96];
    u32 fmbm_tstc;
    u32 fmbm_tfrc;
    u32 fmbm_tfdc;
    u32 fmbm_tfledc;
    u32 fmbm_tfufdc;
    u32 fmbm_tbdc;
    u32 reserved0218[26];
    u32 fmbm_tpc;
    u32 fmbm_tpcp;
    u32 fmbm_tccn;
    u32 fmbm_ttuc;
    u32 fmbm_ttcquc;
    u32 fmbm_tduc;
    u32 fmbm_tfuc;
    u32 reserved029c[16];
    u32 fmbm_tdcfg[3];
    u32 fmbm_tgpr;
    u32 reserved0310[58];
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
