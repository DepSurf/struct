# Struct: <code>fec_enet_private</code>

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
struct fec_enet_private {
    void *hwp;
    struct net_device *netdev;
    struct clk *clk_ipg;
    struct clk *clk_ahb;
    struct clk *clk_ref;
    struct clk *clk_enet_out;
    struct clk *clk_ptp;
    bool ptp_clk_on;
    struct mutex ptp_clk_mutex;
    unsigned int num_tx_queues;
    unsigned int num_rx_queues;
    struct fec_enet_priv_tx_q * tx_queue[3];
    struct fec_enet_priv_rx_q * rx_queue[3];
    unsigned int total_tx_ring_size;
    unsigned int total_rx_ring_size;
    long unsigned int work_tx;
    long unsigned int work_rx;
    long unsigned int work_ts;
    long unsigned int work_mdio;
    struct platform_device *pdev;
    int dev_id;
    struct mii_bus *mii_bus;
    uint phy_speed;
    phy_interface_t phy_interface;
    struct device_node *phy_node;
    int link;
    int full_duplex;
    int speed;
    struct completion mdio_done;
    int irq[3];
    bool bufdesc_ex;
    int pause_flag;
    int wol_flag;
    u32 quirks;
    struct napi_struct napi;
    int csum_flags;
    struct work_struct tx_timeout_work;
    struct ptp_clock *ptp_clock;
    struct ptp_clock_info ptp_caps;
    long unsigned int last_overflow_check;
    spinlock_t tmreg_lock;
    struct cyclecounter cc;
    struct timecounter tc;
    int rx_hwtstamp_filter;
    u32 base_incval;
    u32 cycle_speed;
    int hwts_rx_en;
    int hwts_tx_en;
    struct delayed_work time_keep;
    struct regulator *reg_phy;
    unsigned int tx_align;
    unsigned int rx_align;
    unsigned int rx_pkts_itr;
    unsigned int rx_time_itr;
    unsigned int tx_pkts_itr;
    unsigned int tx_time_itr;
    unsigned int itr_clk_rate;
    u32 rx_copybreak;
    unsigned int ptp_inc;
    int pps_channel;
    unsigned int reload_period;
    int pps_enable;
    unsigned int next_counter;
    u64 ethtool_stats[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct fec_enet_private {
    void *hwp;
    struct net_device *netdev;
    struct clk *clk_ipg;
    struct clk *clk_ahb;
    struct clk *clk_ref;
    struct clk *clk_enet_out;
    struct clk *clk_ptp;
    bool ptp_clk_on;
    struct mutex ptp_clk_mutex;
    unsigned int num_tx_queues;
    unsigned int num_rx_queues;
    struct fec_enet_priv_tx_q * tx_queue[3];
    struct fec_enet_priv_rx_q * rx_queue[3];
    unsigned int total_tx_ring_size;
    unsigned int total_rx_ring_size;
    long unsigned int work_tx;
    long unsigned int work_rx;
    long unsigned int work_ts;
    long unsigned int work_mdio;
    struct platform_device *pdev;
    int dev_id;
    struct mii_bus *mii_bus;
    uint phy_speed;
    phy_interface_t phy_interface;
    struct device_node *phy_node;
    int link;
    int full_duplex;
    int speed;
    struct completion mdio_done;
    int irq[3];
    bool bufdesc_ex;
    int pause_flag;
    int wol_flag;
    u32 quirks;
    struct napi_struct napi;
    int csum_flags;
    struct work_struct tx_timeout_work;
    struct ptp_clock *ptp_clock;
    struct ptp_clock_info ptp_caps;
    long unsigned int last_overflow_check;
    spinlock_t tmreg_lock;
    struct cyclecounter cc;
    struct timecounter tc;
    int rx_hwtstamp_filter;
    u32 base_incval;
    u32 cycle_speed;
    int hwts_rx_en;
    int hwts_tx_en;
    struct delayed_work time_keep;
    struct regulator *reg_phy;
    unsigned int tx_align;
    unsigned int rx_align;
    unsigned int rx_pkts_itr;
    unsigned int rx_time_itr;
    unsigned int tx_pkts_itr;
    unsigned int tx_time_itr;
    unsigned int itr_clk_rate;
    u32 rx_copybreak;
    unsigned int ptp_inc;
    int pps_channel;
    unsigned int reload_period;
    int pps_enable;
    unsigned int next_counter;
    u64 ethtool_stats[0];
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
