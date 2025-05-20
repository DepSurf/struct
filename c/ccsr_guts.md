# Struct: <code>ccsr_guts</code>

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
struct ccsr_guts {
    u32 porpllsr;
    u32 porbmsr;
    u32 porimpscr;
    u32 pordevsr;
    u32 pordbgmsr;
    u32 pordevsr2;
    u8 res018[8];
    u32 porcir;
    u8 res024[12];
    u32 gpiocr;
    u8 res034[12];
    u32 gpoutdr;
    u8 res044[12];
    u32 gpindr;
    u8 res054[12];
    u32 pmuxcr;
    u32 pmuxcr2;
    u32 dmuxcr;
    u8 res06c[4];
    u32 devdisr;
    u32 devdisr2;
    u8 res078[4];
    u32 pmjcr;
    u32 powmgtcsr;
    u32 pmrccr;
    u32 pmpdccr;
    u32 pmcdr;
    u32 mcpsumr;
    u32 rstrscr;
    u32 ectrstcr;
    u32 autorstsr;
    u32 pvr;
    u32 svr;
    u8 res0a8[8];
    u32 rstcr;
    u8 res0b4[12];
    u32 iovselsr;
    u8 res0c4[60];
    u32 rcwsr[16];
    u8 res140[228];
    u32 iodelay1;
    u32 iodelay2;
    u8 res22c[984];
    u32 pamubypenr;
    u8 res608[504];
    u32 clkdvdr;
    u8 res804[252];
    u32 ircr;
    u8 res904[4];
    u32 dmacr;
    u8 res90c[8];
    u32 elbccr;
    u8 res918[520];
    u32 ddr1clkdr;
    u32 ddr2clkdr;
    u32 ddrclkdr;
    u8 resb2c[724];
    u32 clkocr;
    u8 rese04[12];
    u32 ddrdllcr;
    u8 rese14[12];
    u32 lbcdllcr;
    u32 cpfor;
    u8 rese28[220];
    u32 srds1cr0;
    u32 srds1cr1;
    u8 resf0c[32];
    u32 itcr;
    u8 resf30[16];
    u32 srds2cr0;
    u32 srds2cr1;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ccsr_guts {
    u32 porpllsr;
    u32 porbmsr;
    u32 porimpscr;
    u32 pordevsr;
    u32 pordbgmsr;
    u32 pordevsr2;
    u8 res018[8];
    u32 porcir;
    u8 res024[12];
    u32 gpiocr;
    u8 res034[12];
    u32 gpoutdr;
    u8 res044[12];
    u32 gpindr;
    u8 res054[12];
    u32 pmuxcr;
    u32 pmuxcr2;
    u32 dmuxcr;
    u8 res06c[4];
    u32 devdisr;
    u32 devdisr2;
    u8 res078[4];
    u32 pmjcr;
    u32 powmgtcsr;
    u32 pmrccr;
    u32 pmpdccr;
    u32 pmcdr;
    u32 mcpsumr;
    u32 rstrscr;
    u32 ectrstcr;
    u32 autorstsr;
    u32 pvr;
    u32 svr;
    u8 res0a8[8];
    u32 rstcr;
    u8 res0b4[12];
    u32 iovselsr;
    u8 res0c4[60];
    u32 rcwsr[16];
    u8 res140[228];
    u32 iodelay1;
    u32 iodelay2;
    u8 res22c[984];
    u32 pamubypenr;
    u8 res608[504];
    u32 clkdvdr;
    u8 res804[252];
    u32 ircr;
    u8 res904[4];
    u32 dmacr;
    u8 res90c[8];
    u32 elbccr;
    u8 res918[520];
    u32 ddr1clkdr;
    u32 ddr2clkdr;
    u32 ddrclkdr;
    u8 resb2c[724];
    u32 clkocr;
    u8 rese04[12];
    u32 ddrdllcr;
    u8 rese14[12];
    u32 lbcdllcr;
    u32 cpfor;
    u8 rese28[220];
    u32 srds1cr0;
    u32 srds1cr1;
    u8 resf0c[32];
    u32 itcr;
    u8 resf30[16];
    u32 srds2cr0;
    u32 srds2cr1;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ccsr_guts {
    u32 porpllsr;
    u32 porbmsr;
    u32 porimpscr;
    u32 pordevsr;
    u32 pordbgmsr;
    u32 pordevsr2;
    u8 res018[8];
    u32 porcir;
    u8 res024[12];
    u32 gpiocr;
    u8 res034[12];
    u32 gpoutdr;
    u8 res044[12];
    u32 gpindr;
    u8 res054[12];
    u32 pmuxcr;
    u32 pmuxcr2;
    u32 dmuxcr;
    u8 res06c[4];
    u32 devdisr;
    u32 devdisr2;
    u8 res078[4];
    u32 pmjcr;
    u32 powmgtcsr;
    u32 pmrccr;
    u32 pmpdccr;
    u32 pmcdr;
    u32 mcpsumr;
    u32 rstrscr;
    u32 ectrstcr;
    u32 autorstsr;
    u32 pvr;
    u32 svr;
    u8 res0a8[8];
    u32 rstcr;
    u8 res0b4[12];
    u32 iovselsr;
    u8 res0c4[60];
    u32 rcwsr[16];
    u8 res140[228];
    u32 iodelay1;
    u32 iodelay2;
    u8 res22c[984];
    u32 pamubypenr;
    u8 res608[504];
    u32 clkdvdr;
    u8 res804[252];
    u32 ircr;
    u8 res904[4];
    u32 dmacr;
    u8 res90c[8];
    u32 elbccr;
    u8 res918[520];
    u32 ddr1clkdr;
    u32 ddr2clkdr;
    u32 ddrclkdr;
    u8 resb2c[724];
    u32 clkocr;
    u8 rese04[12];
    u32 ddrdllcr;
    u8 rese14[12];
    u32 lbcdllcr;
    u32 cpfor;
    u8 rese28[220];
    u32 srds1cr0;
    u32 srds1cr1;
    u8 resf0c[32];
    u32 itcr;
    u8 resf30[16];
    u32 srds2cr0;
    u32 srds2cr1;
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
