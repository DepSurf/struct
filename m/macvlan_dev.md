# Struct: <code>macvlan_dev</code>

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
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct macvlan_dev {
    struct net_device *dev;
    struct list_head list;
    struct hlist_node hlist;
    struct macvlan_port *port;
    struct net_device *lowerdev;
    void *fwd_priv;
    struct vlan_pcpu_stats *pcpu_stats;
    long unsigned int mc_filter[4];
    netdev_features_t set_features;
    enum macvlan_mode mode;
    u16 flags;
    int nest_level;
    struct netpoll *netpoll;
    unsigned int macaddr_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct macvlan_dev {
    struct net_device *dev;
    struct list_head list;
    struct hlist_node hlist;
    struct macvlan_port *port;
    struct net_device *lowerdev;
    void *accel_priv;
    struct vlan_pcpu_stats *pcpu_stats;
    long unsigned int mc_filter[4];
    netdev_features_t set_features;
    enum macvlan_mode mode;
    u16 flags;
    int nest_level;
    unsigned int macaddr_count;
    struct netpoll *netpoll;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct macvlan_dev {
    struct net_device *dev;
    struct list_head list;
    struct hlist_node hlist;
    struct macvlan_port *port;
    struct net_device *lowerdev;
    void *accel_priv;
    struct vlan_pcpu_stats *pcpu_stats;
    long unsigned int mc_filter[4];
    netdev_features_t set_features;
    enum macvlan_mode mode;
    u16 flags;
    int nest_level;
    unsigned int macaddr_count;
    struct netpoll *netpoll;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct macvlan_dev {
    struct net_device *dev;
    struct list_head list;
    struct hlist_node hlist;
    struct macvlan_port *port;
    struct net_device *lowerdev;
    void *accel_priv;
    struct vlan_pcpu_stats *pcpu_stats;
    long unsigned int mc_filter[4];
    netdev_features_t set_features;
    enum macvlan_mode mode;
    u16 flags;
    int nest_level;
    unsigned int macaddr_count;
    struct netpoll *netpoll;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct macvlan_dev {
    struct net_device *dev;
    struct list_head list;
    struct hlist_node hlist;
    struct macvlan_port *port;
    struct net_device *lowerdev;
    void *accel_priv;
    struct vlan_pcpu_stats *pcpu_stats;
    long unsigned int mc_filter[4];
    netdev_features_t set_features;
    enum macvlan_mode mode;
    u16 flags;
    unsigned int macaddr_count;
    struct netpoll *netpoll;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct macvlan_dev {
    struct net_device *dev;
    struct list_head list;
    struct hlist_node hlist;
    struct macvlan_port *port;
    struct net_device *lowerdev;
    void *accel_priv;
    struct vlan_pcpu_stats *pcpu_stats;
    long unsigned int mc_filter[4];
    netdev_features_t set_features;
    enum macvlan_mode mode;
    u16 flags;
    unsigned int macaddr_count;
    struct netpoll *netpoll;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct macvlan_dev {
    struct net_device *dev;
    struct list_head list;
    struct hlist_node hlist;
    struct macvlan_port *port;
    struct net_device *lowerdev;
    void *accel_priv;
    struct vlan_pcpu_stats *pcpu_stats;
    long unsigned int mc_filter[4];
    netdev_features_t set_features;
    enum macvlan_mode mode;
    u16 flags;
    unsigned int macaddr_count;
    u32 bc_queue_len_req;
    struct netpoll *netpoll;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct macvlan_dev {
    struct net_device *dev;
    struct list_head list;
    struct hlist_node hlist;
    struct macvlan_port *port;
    struct net_device *lowerdev;
    void *accel_priv;
    struct vlan_pcpu_stats *pcpu_stats;
    long unsigned int mc_filter[4];
    netdev_features_t set_features;
    enum macvlan_mode mode;
    u16 flags;
    unsigned int macaddr_count;
    u32 bc_queue_len_req;
    struct netpoll *netpoll;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct macvlan_dev {
    struct net_device *dev;
    struct list_head list;
    struct hlist_node hlist;
    struct macvlan_port *port;
    struct net_device *lowerdev;
    void *accel_priv;
    struct vlan_pcpu_stats *pcpu_stats;
    long unsigned int mc_filter[4];
    netdev_features_t set_features;
    enum macvlan_mode mode;
    u16 flags;
    unsigned int macaddr_count;
    u32 bc_queue_len_req;
    struct netpoll *netpoll;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct macvlan_dev {
    struct net_device *dev;
    struct list_head list;
    struct hlist_node hlist;
    struct macvlan_port *port;
    struct net_device *lowerdev;
    netdevice_tracker dev_tracker;
    void *accel_priv;
    struct vlan_pcpu_stats *pcpu_stats;
    long unsigned int mc_filter[4];
    netdev_features_t set_features;
    enum macvlan_mode mode;
    u16 flags;
    unsigned int macaddr_count;
    u32 bc_queue_len_req;
    struct netpoll *netpoll;
};
```
</details>
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
struct macvlan_dev {
    struct net_device *dev;
    struct list_head list;
    struct hlist_node hlist;
    struct macvlan_port *port;
    struct net_device *lowerdev;
    void *accel_priv;
    struct vlan_pcpu_stats *pcpu_stats;
    long unsigned int mc_filter[4];
    netdev_features_t set_features;
    enum macvlan_mode mode;
    u16 flags;
    unsigned int macaddr_count;
    struct netpoll *netpoll;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct macvlan_dev {
    struct net_device *dev;
    struct list_head list;
    struct hlist_node hlist;
    struct macvlan_port *port;
    struct net_device *lowerdev;
    void *accel_priv;
    struct vlan_pcpu_stats *pcpu_stats;
    long unsigned int mc_filter[8];
    netdev_features_t set_features;
    enum macvlan_mode mode;
    u16 flags;
    unsigned int macaddr_count;
    struct netpoll *netpoll;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct macvlan_dev {
    struct net_device *dev;
    struct list_head list;
    struct hlist_node hlist;
    struct macvlan_port *port;
    struct net_device *lowerdev;
    void *accel_priv;
    struct vlan_pcpu_stats *pcpu_stats;
    long unsigned int mc_filter[4];
    netdev_features_t set_features;
    enum macvlan_mode mode;
    u16 flags;
    unsigned int macaddr_count;
    struct netpoll *netpoll;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct macvlan_dev {
    struct net_device *dev;
    struct list_head list;
    struct hlist_node hlist;
    struct macvlan_port *port;
    struct net_device *lowerdev;
    void *accel_priv;
    struct vlan_pcpu_stats *pcpu_stats;
    long unsigned int mc_filter[4];
    netdev_features_t set_features;
    enum macvlan_mode mode;
    u16 flags;
    unsigned int macaddr_count;
    struct netpoll *netpoll;
};
```
</details>
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct macvlan_dev {
    struct net_device *dev;
    struct list_head list;
    struct hlist_node hlist;
    struct macvlan_port *port;
    struct net_device *lowerdev;
    void *accel_priv;
    struct vlan_pcpu_stats *pcpu_stats;
    long unsigned int mc_filter[4];
    netdev_features_t set_features;
    enum macvlan_mode mode;
    u16 flags;
    unsigned int macaddr_count;
    struct netpoll *netpoll;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct macvlan_dev {
    struct net_device *dev;
    struct list_head list;
    struct hlist_node hlist;
    struct macvlan_port *port;
    struct net_device *lowerdev;
    void *accel_priv;
    struct vlan_pcpu_stats *pcpu_stats;
    long unsigned int mc_filter[4];
    netdev_features_t set_features;
    enum macvlan_mode mode;
    u16 flags;
    unsigned int macaddr_count;
    struct netpoll *netpoll;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct macvlan_dev {
    struct net_device *dev;
    struct list_head list;
    struct hlist_node hlist;
    struct macvlan_port *port;
    struct net_device *lowerdev;
    void *accel_priv;
    struct vlan_pcpu_stats *pcpu_stats;
    long unsigned int mc_filter[4];
    netdev_features_t set_features;
    enum macvlan_mode mode;
    u16 flags;
    unsigned int macaddr_count;
    struct netpoll *netpoll;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct macvlan_dev {
    struct net_device *dev;
    struct list_head list;
    struct hlist_node hlist;
    struct macvlan_port *port;
    struct net_device *lowerdev;
    void *accel_priv;
    struct vlan_pcpu_stats *pcpu_stats;
    long unsigned int mc_filter[4];
    netdev_features_t set_features;
    enum macvlan_mode mode;
    u16 flags;
    unsigned int macaddr_count;
    struct netpoll *netpoll;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void *accel_priv</code>
</li>
<li>
<b>Field removed. </b>
<code>void *fwd_priv</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int nest_level</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 bc_queue_len_req</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>netdevice_tracker dev_tracker</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long unsigned int mc_filter[4]</code> ➡️ <code>long unsigned int mc_filter[8]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>riscv64</code> ✅
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
No changes between <code>generic</code> and <code>aws</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
