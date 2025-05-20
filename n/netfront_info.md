# Struct: <code>netfront_info</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct netfront_info {
    struct list_head list;
    struct net_device *netdev;
    struct xenbus_device *xbdev;
    struct netfront_queue *queues;
    struct netfront_stats *rx_stats;
    struct netfront_stats *tx_stats;
    atomic_t rx_gso_checksum_fixup;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct netfront_info {
    struct list_head list;
    struct net_device *netdev;
    struct xenbus_device *xbdev;
    struct netfront_queue *queues;
    struct netfront_stats *rx_stats;
    struct netfront_stats *tx_stats;
    atomic_t rx_gso_checksum_fixup;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct netfront_info {
    struct list_head list;
    struct net_device *netdev;
    struct xenbus_device *xbdev;
    struct netfront_queue *queues;
    struct netfront_stats *rx_stats;
    struct netfront_stats *tx_stats;
    atomic_t rx_gso_checksum_fixup;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct netfront_info {
    struct list_head list;
    struct net_device *netdev;
    struct xenbus_device *xbdev;
    struct netfront_queue *queues;
    struct netfront_stats *rx_stats;
    struct netfront_stats *tx_stats;
    atomic_t rx_gso_checksum_fixup;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct netfront_info {
    struct list_head list;
    struct net_device *netdev;
    struct xenbus_device *xbdev;
    struct netfront_queue *queues;
    struct netfront_stats *rx_stats;
    struct netfront_stats *tx_stats;
    atomic_t rx_gso_checksum_fixup;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct netfront_info {
    struct list_head list;
    struct net_device *netdev;
    struct xenbus_device *xbdev;
    struct netfront_queue *queues;
    struct netfront_stats *rx_stats;
    struct netfront_stats *tx_stats;
    atomic_t rx_gso_checksum_fixup;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct netfront_info {
    struct list_head list;
    struct net_device *netdev;
    struct xenbus_device *xbdev;
    struct netfront_queue *queues;
    struct netfront_stats *rx_stats;
    struct netfront_stats *tx_stats;
    atomic_t rx_gso_checksum_fixup;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct netfront_info {
    struct list_head list;
    struct net_device *netdev;
    struct xenbus_device *xbdev;
    struct netfront_queue *queues;
    struct netfront_stats *rx_stats;
    struct netfront_stats *tx_stats;
    atomic_t rx_gso_checksum_fixup;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct netfront_info {
    struct list_head list;
    struct net_device *netdev;
    struct xenbus_device *xbdev;
    struct netfront_queue *queues;
    struct netfront_stats *rx_stats;
    struct netfront_stats *tx_stats;
    atomic_t rx_gso_checksum_fixup;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct netfront_info {
    struct list_head list;
    struct net_device *netdev;
    struct xenbus_device *xbdev;
    struct netfront_queue *queues;
    struct netfront_stats *rx_stats;
    struct netfront_stats *tx_stats;
    atomic_t rx_gso_checksum_fixup;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct netfront_info {
    struct list_head list;
    struct net_device *netdev;
    struct xenbus_device *xbdev;
    struct netfront_queue *queues;
    struct netfront_stats *rx_stats;
    struct netfront_stats *tx_stats;
    bool netback_has_xdp_headroom;
    bool netfront_xdp_enabled;
    atomic_t rx_gso_checksum_fixup;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct netfront_info {
    struct list_head list;
    struct net_device *netdev;
    struct xenbus_device *xbdev;
    struct netfront_queue *queues;
    struct netfront_stats *rx_stats;
    struct netfront_stats *tx_stats;
    bool netback_has_xdp_headroom;
    bool netfront_xdp_enabled;
    atomic_t rx_gso_checksum_fixup;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct netfront_info {
    struct list_head list;
    struct net_device *netdev;
    struct xenbus_device *xbdev;
    struct netfront_queue *queues;
    struct netfront_stats *rx_stats;
    struct netfront_stats *tx_stats;
    bool netback_has_xdp_headroom;
    bool netfront_xdp_enabled;
    bool broken;
    atomic_t rx_gso_checksum_fixup;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct netfront_info {
    struct list_head list;
    struct net_device *netdev;
    struct xenbus_device *xbdev;
    struct netfront_queue *queues;
    struct netfront_stats *rx_stats;
    struct netfront_stats *tx_stats;
    bool netback_has_xdp_headroom;
    bool netfront_xdp_enabled;
    bool broken;
    bool bounce;
    atomic_t rx_gso_checksum_fixup;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct netfront_info {
    struct list_head list;
    struct net_device *netdev;
    struct xenbus_device *xbdev;
    struct netfront_queue *queues;
    struct netfront_stats *rx_stats;
    struct netfront_stats *tx_stats;
    bool netback_has_xdp_headroom;
    bool netfront_xdp_enabled;
    bool broken;
    bool bounce;
    atomic_t rx_gso_checksum_fixup;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct netfront_info {
    struct list_head list;
    struct net_device *netdev;
    struct xenbus_device *xbdev;
    struct netfront_queue *queues;
    struct netfront_stats *rx_stats;
    struct netfront_stats *tx_stats;
    bool netback_has_xdp_headroom;
    bool netfront_xdp_enabled;
    bool broken;
    bool bounce;
    atomic_t rx_gso_checksum_fixup;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct netfront_info {
    struct list_head list;
    struct net_device *netdev;
    struct xenbus_device *xbdev;
    struct netfront_queue *queues;
    struct netfront_stats *rx_stats;
    struct netfront_stats *tx_stats;
    bool netback_has_xdp_headroom;
    bool netfront_xdp_enabled;
    bool broken;
    bool bounce;
    atomic_t rx_gso_checksum_fixup;
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct netfront_info {
    struct list_head list;
    struct net_device *netdev;
    struct xenbus_device *xbdev;
    struct netfront_queue *queues;
    struct netfront_stats *rx_stats;
    struct netfront_stats *tx_stats;
    atomic_t rx_gso_checksum_fixup;
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct netfront_info {
    struct list_head list;
    struct net_device *netdev;
    struct xenbus_device *xbdev;
    struct netfront_queue *queues;
    struct netfront_stats *rx_stats;
    struct netfront_stats *tx_stats;
    atomic_t rx_gso_checksum_fixup;
    int freeze_state;
    struct completion wait_backend_disconnected;
};
```
</details>
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct netfront_info {
    struct list_head list;
    struct net_device *netdev;
    struct xenbus_device *xbdev;
    struct netfront_queue *queues;
    struct netfront_stats *rx_stats;
    struct netfront_stats *tx_stats;
    atomic_t rx_gso_checksum_fixup;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct netfront_info {
    struct list_head list;
    struct net_device *netdev;
    struct xenbus_device *xbdev;
    struct netfront_queue *queues;
    struct netfront_stats *rx_stats;
    struct netfront_stats *tx_stats;
    atomic_t rx_gso_checksum_fixup;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.4</code> and <code>4.8</code> ✅
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
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
<code>bool netback_has_xdp_headroom</code>
</li>
<li>
<b>Field added. </b>
<code>bool netfront_xdp_enabled</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool broken</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool bounce</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
<b>Arch</b>
<ul>
<li>
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
<details>
<summary>Changed between <code>generic</code> and <code>aws</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int freeze_state</code>
</li>
<li>
<b>Field added. </b>
<code>struct completion wait_backend_disconnected</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
