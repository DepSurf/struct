# Struct: <code>fsl_lbc_regs</code>

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
struct fsl_lbc_regs {
    struct fsl_lbc_bank bank[12];
    u8 res0[8];
    __be32 mar;
    u8 res1[4];
    __be32 mamr;
    __be32 mbmr;
    __be32 mcmr;
    u8 res2[8];
    __be32 mrtpr;
    __be32 mdr;
    u8 res3[4];
    __be32 lsor;
    __be32 lsdmr;
    u8 res4[8];
    __be32 lurt;
    __be32 lsrt;
    u8 res5[8];
    __be32 ltesr;
    __be32 ltedr;
    __be32 lteir;
    __be32 lteatr;
    __be32 ltear;
    __be32 lteccr;
    u8 res6[8];
    __be32 lbcr;
    __be32 lcrr;
    u8 res7[8];
    __be32 fmr;
    __be32 fir;
    __be32 fcr;
    __be32 fbar;
    __be32 fpar;
    __be32 fbcr;
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
