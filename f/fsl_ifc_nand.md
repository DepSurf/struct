# Struct: <code>fsl_ifc_nand</code>

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
struct fsl_ifc_nand {
    __be32 ncfgr;
    u32 res1[4];
    __be32 nand_fcr0;
    __be32 nand_fcr1;
    u32 res2[8];
    __be32 row0;
    u32 res3;
    __be32 col0;
    u32 res4;
    __be32 row1;
    u32 res5;
    __be32 col1;
    u32 res6;
    __be32 row2;
    u32 res7;
    __be32 col2;
    u32 res8;
    __be32 row3;
    u32 res9;
    __be32 col3;
    u32 res10[36];
    __be32 nand_fbcr;
    u32 res11;
    __be32 nand_fir0;
    __be32 nand_fir1;
    __be32 nand_fir2;
    u32 res12[16];
    __be32 nand_csel;
    u32 res13;
    __be32 nandseq_strt;
    u32 res14;
    __be32 nand_evter_stat;
    u32 res15;
    __be32 pgrdcmpl_evt_stat;
    u32 res16[2];
    __be32 nand_evter_en;
    u32 res17[2];
    __be32 nand_evter_intr_en;
    __be32 nand_vol_addr_stat;
    u32 res18;
    __be32 nand_erattr0;
    __be32 nand_erattr1;
    u32 res19[16];
    __be32 nand_fsr;
    u32 res20;
    __be32 nand_eccstat[8];
    u32 res21[28];
    __be32 nanndcr;
    u32 res22[2];
    __be32 nand_autoboot_trgr;
    u32 res23;
    __be32 nand_mdr;
    u32 res24[28];
    __be32 nand_dll_lowcfg0;
    __be32 nand_dll_lowcfg1;
    u32 res25;
    __be32 nand_dll_lowstat;
    u32 res26[60];
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
