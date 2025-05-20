# Struct: <code>fman_fpm_regs</code>

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
struct fman_fpm_regs {
    u32 fmfp_tnc;
    u32 fmfp_prc;
    u32 fmfp_brkc;
    u32 fmfp_mxd;
    u32 fmfp_dist1;
    u32 fmfp_dist2;
    u32 fm_epi;
    u32 fm_rie;
    u32 fmfp_fcev[4];
    u32 res0030[4];
    u32 fmfp_cee[4];
    u32 res0050[4];
    u32 fmfp_tsc1;
    u32 fmfp_tsc2;
    u32 fmfp_tsp;
    u32 fmfp_tsf;
    u32 fm_rcr;
    u32 fmfp_extc;
    u32 fmfp_ext1;
    u32 fmfp_ext2;
    u32 fmfp_drd[16];
    u32 fmfp_dra;
    u32 fm_ip_rev_1;
    u32 fm_ip_rev_2;
    u32 fm_rstc;
    u32 fm_cld;
    u32 fm_npi;
    u32 fmfp_exte;
    u32 fmfp_ee;
    u32 fmfp_cev[4];
    u32 res00f0[4];
    u32 fmfp_ps[50];
    u32 res01c8[14];
    u32 fmfp_clfabc;
    u32 fmfp_clfcc;
    u32 fmfp_clfaval;
    u32 fmfp_clfbval;
    u32 fmfp_clfcval;
    u32 fmfp_clfamsk;
    u32 fmfp_clfbmsk;
    u32 fmfp_clfcmsk;
    u32 fmfp_clfamc;
    u32 fmfp_clfbmc;
    u32 fmfp_clfcmc;
    u32 fmfp_decceh;
    u32 res0230[116];
    u32 fmfp_ts[128];
    u32 res0600[640];
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
