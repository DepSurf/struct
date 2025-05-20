# Struct: <code>bgmac</code>

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
struct bgmac {
    struct (anon) plat;
    struct (anon) bcma;
    struct device *dev;
    struct device *dma_dev;
    u32 feature_flags;
    struct net_device *net_dev;
    struct napi_struct napi;
    struct mii_bus *mii_bus;
    struct bgmac_dma_ring tx_ring[4];
    struct bgmac_dma_ring rx_ring[1];
    bool stats_grabbed;
    u32 mib_tx_regs[43];
    u32 mib_rx_regs[31];
    int irq;
    u32 int_mask;
    int mac_speed;
    int mac_duplex;
    u8 phyaddr;
    bool has_robosw;
    bool loopback;
    u32 (*read)(struct bgmac *, u16);
    void (*write)(struct bgmac *, u16, u32);
    u32 (*idm_read)(struct bgmac *, u16);
    void (*idm_write)(struct bgmac *, u16, u32);
    bool (*clk_enabled)(struct bgmac *);
    void (*clk_enable)(struct bgmac *, u32);
    void (*cco_ctl_maskset)(struct bgmac *, u32, u32, u32);
    u32 (*get_bus_clock)(struct bgmac *);
    void (*cmn_maskset32)(struct bgmac *, u16, u32, u32);
    int (*phy_connect)(struct bgmac *);
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
