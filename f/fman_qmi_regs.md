# Struct: <code>fman_qmi_regs</code>

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
struct fman_qmi_regs {
    u32 fmqm_gc;
    u32 res0004;
    u32 fmqm_eie;
    u32 fmqm_eien;
    u32 fmqm_eif;
    u32 fmqm_ie;
    u32 fmqm_ien;
    u32 fmqm_if;
    u32 fmqm_gs;
    u32 fmqm_ts;
    u32 fmqm_etfc;
    u32 fmqm_dtfc;
    u32 fmqm_dc0;
    u32 fmqm_dc1;
    u32 fmqm_dc2;
    u32 fmqm_dc3;
    u32 fmqm_dfdc;
    u32 fmqm_dfcc;
    u32 fmqm_dffc;
    u32 fmqm_dcc;
    u32 res0050[7];
    u32 fmqm_tapc;
    u32 fmqm_dmcvc;
    u32 fmqm_difdcc;
    u32 fmqm_da1v;
    u32 res007c;
    u32 fmqm_dtc;
    u32 fmqm_efddd;
    u32 res0088[2];
    struct (anon) dbg_traps[3];
    u8 res00f0[784];
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
