# Struct: <code>tegra_pingroup</code>

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
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct tegra_pingroup {
    const char *name;
    const unsigned int *pins;
    u8 npins;
    u8 funcs[4];
    s32 mux_reg;
    s32 pupd_reg;
    s32 tri_reg;
    s32 drv_reg;
    u32 mux_bank;
    u32 pupd_bank;
    u32 tri_bank;
    u32 drv_bank;
    s32 mux_bit;
    s32 pupd_bit;
    s32 tri_bit;
    s32 einput_bit;
    s32 odrain_bit;
    s32 lock_bit;
    s32 ioreset_bit;
    s32 rcv_sel_bit;
    s32 hsm_bit;
    s32 schmitt_bit;
    s32 lpmd_bit;
    s32 drvdn_bit;
    s32 drvup_bit;
    s32 slwr_bit;
    s32 slwf_bit;
    s32 drvtype_bit;
    s32 drvdn_width;
    s32 drvup_width;
    s32 slwr_width;
    s32 slwf_width;
    u32 parked_bitmask;
};
```
</details>
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
