# Struct: <code>mac_device</code>

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
struct mac_device {
    struct resource *res;
    u8 addr[6];
    struct fman_port * port[2];
    u32 if_support;
    struct phy_device *phy_dev;
    phy_interface_t phy_if;
    struct device_node *phy_node;
    bool autoneg_pause;
    bool rx_pause_req;
    bool tx_pause_req;
    bool rx_pause_active;
    bool tx_pause_active;
    bool promisc;
    bool allmulti;
    int (*init)(struct mac_device *);
    int (*start)(struct mac_device *);
    int (*stop)(struct mac_device *);
    void (*adjust_link)(struct mac_device *);
    int (*set_promisc)(struct fman_mac *, bool);
    int (*change_addr)(struct fman_mac *, enet_addr_t *);
    int (*set_allmulti)(struct fman_mac *, bool);
    int (*set_tstamp)(struct fman_mac *, bool);
    int (*set_multi)(struct net_device *, struct mac_device *);
    int (*set_rx_pause)(struct fman_mac *, bool);
    int (*set_tx_pause)(struct fman_mac *, u8, u16, u16);
    int (*set_exception)(struct fman_mac *, enum fman_mac_exceptions, bool);
    int (*add_hash_mac_addr)(struct fman_mac *, enet_addr_t *);
    int (*remove_hash_mac_addr)(struct fman_mac *, enet_addr_t *);
    struct fman_mac *fman_mac;
    struct mac_priv_s *priv;
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
