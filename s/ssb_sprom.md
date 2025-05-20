# Struct: <code>ssb_sprom</code>

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
struct ssb_sprom {
    u8 revision;
    u8 il0mac[6];
    u8 et0mac[6];
    u8 et1mac[6];
    u8 et2mac[6];
    u8 et0phyaddr;
    u8 et1phyaddr;
    u8 et2phyaddr;
    u8 et0mdcport;
    u8 et1mdcport;
    u8 et2mdcport;
    u16 dev_id;
    u16 board_rev;
    u16 board_num;
    u16 board_type;
    u8 country_code;
    char alpha2[2];
    u8 leddc_on_time;
    u8 leddc_off_time;
    u8 ant_available_a;
    u8 ant_available_bg;
    u16 pa0b0;
    u16 pa0b1;
    u16 pa0b2;
    u16 pa1b0;
    u16 pa1b1;
    u16 pa1b2;
    u16 pa1lob0;
    u16 pa1lob1;
    u16 pa1lob2;
    u16 pa1hib0;
    u16 pa1hib1;
    u16 pa1hib2;
    u8 gpio0;
    u8 gpio1;
    u8 gpio2;
    u8 gpio3;
    u8 maxpwr_bg;
    u8 maxpwr_al;
    u8 maxpwr_a;
    u8 maxpwr_ah;
    u8 itssi_a;
    u8 itssi_bg;
    u8 tri2g;
    u8 tri5gl;
    u8 tri5g;
    u8 tri5gh;
    u8 txpid2g[4];
    u8 txpid5gl[4];
    u8 txpid5g[4];
    u8 txpid5gh[4];
    s8 rxpo2g;
    s8 rxpo5g;
    u8 rssisav2g;
    u8 rssismc2g;
    u8 rssismf2g;
    u8 bxa2g;
    u8 rssisav5g;
    u8 rssismc5g;
    u8 rssismf5g;
    u8 bxa5g;
    u16 cck2gpo;
    u32 ofdm2gpo;
    u32 ofdm5glpo;
    u32 ofdm5gpo;
    u32 ofdm5ghpo;
    u32 boardflags;
    u32 boardflags2;
    u32 boardflags3;
    u16 boardflags_lo;
    u16 boardflags_hi;
    u16 boardflags2_lo;
    u16 boardflags2_hi;
    struct ssb_sprom_core_pwr_info core_pwr_info[4];
    struct (anon) antenna_gain;
    struct (anon) fem;
    u16 mcs2gpo[8];
    u16 mcs5gpo[8];
    u16 mcs5glpo[8];
    u16 mcs5ghpo[8];
    u8 opo;
    u8 rxgainerr2ga[3];
    u8 rxgainerr5gla[3];
    u8 rxgainerr5gma[3];
    u8 rxgainerr5gha[3];
    u8 rxgainerr5gua[3];
    u8 noiselvl2ga[3];
    u8 noiselvl5gla[3];
    u8 noiselvl5gma[3];
    u8 noiselvl5gha[3];
    u8 noiselvl5gua[3];
    u8 regrev;
    u8 txchain;
    u8 rxchain;
    u8 antswitch;
    u16 cddpo;
    u16 stbcpo;
    u16 bw40po;
    u16 bwduppo;
    u8 tempthresh;
    u8 tempoffset;
    u16 rawtempsense;
    u8 measpower;
    u8 tempsense_slope;
    u8 tempcorrx;
    u8 tempsense_option;
    u8 freqoffset_corr;
    u8 iqcal_swp_dis;
    u8 hw_iqcal_en;
    u8 elna2g;
    u8 elna5g;
    u8 phycal_tempdelta;
    u8 temps_period;
    u8 temps_hysteresis;
    u8 measpower1;
    u8 measpower2;
    u8 pcieingress_war;
    u16 cckbw202gpo;
    u16 cckbw20ul2gpo;
    u32 legofdmbw202gpo;
    u32 legofdmbw20ul2gpo;
    u32 legofdmbw205glpo;
    u32 legofdmbw20ul5glpo;
    u32 legofdmbw205gmpo;
    u32 legofdmbw20ul5gmpo;
    u32 legofdmbw205ghpo;
    u32 legofdmbw20ul5ghpo;
    u32 mcsbw202gpo;
    u32 mcsbw20ul2gpo;
    u32 mcsbw402gpo;
    u32 mcsbw205glpo;
    u32 mcsbw20ul5glpo;
    u32 mcsbw405glpo;
    u32 mcsbw205gmpo;
    u32 mcsbw20ul5gmpo;
    u32 mcsbw405gmpo;
    u32 mcsbw205ghpo;
    u32 mcsbw20ul5ghpo;
    u32 mcsbw405ghpo;
    u16 mcs32po;
    u16 legofdm40duppo;
    u8 sar2g;
    u8 sar5g;
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
