# Struct: <code>fsl_ifc_global</code>

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
struct fsl_ifc_global {
    __be32 ifc_rev;
    u32 res1[2];
    struct (anon) cspr_cs[8];
    u32 res3[13];
    struct (anon) amask_cs[8];
    u32 res5[12];
    struct (anon) csor_cs[8];
    u32 res7[12];
    struct (anon) ftim_cs[8];
    u32 res9[48];
    __be32 rb_stat;
    __be32 rb_map;
    __be32 wb_map;
    __be32 ifc_gcr;
    u32 res10[2];
    __be32 cm_evter_stat;
    u32 res11[2];
    __be32 cm_evter_en;
    u32 res12[2];
    __be32 cm_evter_intr_en;
    u32 res13[2];
    __be32 cm_erattr0;
    __be32 cm_erattr1;
    u32 res14[2];
    __be32 ifc_ccr;
    __be32 ifc_csr;
    __be32 ddr_ccr_low;
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
