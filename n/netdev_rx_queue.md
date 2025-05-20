# Struct: <code>netdev_rx_queue</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct netdev_rx_queue {
    struct rps_map *rps_map;
    struct rps_dev_flow_table *rps_flow_table;
    struct kobject kobj;
    struct net_device *dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct netdev_rx_queue {
    struct rps_map *rps_map;
    struct rps_dev_flow_table *rps_flow_table;
    struct kobject kobj;
    struct net_device *dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct netdev_rx_queue {
    struct rps_map *rps_map;
    struct rps_dev_flow_table *rps_flow_table;
    struct kobject kobj;
    struct net_device *dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct netdev_rx_queue {
    struct rps_map *rps_map;
    struct rps_dev_flow_table *rps_flow_table;
    struct kobject kobj;
    struct net_device *dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct netdev_rx_queue {
    struct rps_map *rps_map;
    struct rps_dev_flow_table *rps_flow_table;
    struct kobject kobj;
    struct net_device *dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct netdev_rx_queue {
    struct rps_map *rps_map;
    struct rps_dev_flow_table *rps_flow_table;
    struct kobject kobj;
    struct net_device *dev;
    struct xdp_rxq_info xdp_rxq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct netdev_rx_queue {
    struct rps_map *rps_map;
    struct rps_dev_flow_table *rps_flow_table;
    struct kobject kobj;
    struct net_device *dev;
    struct xdp_rxq_info xdp_rxq;
    struct xdp_umem *umem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct netdev_rx_queue {
    struct rps_map *rps_map;
    struct rps_dev_flow_table *rps_flow_table;
    struct kobject kobj;
    struct net_device *dev;
    struct xdp_rxq_info xdp_rxq;
    struct xdp_umem *umem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct netdev_rx_queue {
    struct rps_map *rps_map;
    struct rps_dev_flow_table *rps_flow_table;
    struct kobject kobj;
    struct net_device *dev;
    struct xdp_rxq_info xdp_rxq;
    struct xdp_umem *umem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct netdev_rx_queue {
    struct rps_map *rps_map;
    struct rps_dev_flow_table *rps_flow_table;
    struct kobject kobj;
    struct net_device *dev;
    struct xdp_rxq_info xdp_rxq;
    struct xdp_umem *umem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct netdev_rx_queue {
    struct rps_map *rps_map;
    struct rps_dev_flow_table *rps_flow_table;
    struct kobject kobj;
    struct net_device *dev;
    struct xdp_rxq_info xdp_rxq;
    struct xsk_buff_pool *pool;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct netdev_rx_queue {
    struct rps_map *rps_map;
    struct rps_dev_flow_table *rps_flow_table;
    struct kobject kobj;
    struct net_device *dev;
    struct xdp_rxq_info xdp_rxq;
    struct xsk_buff_pool *pool;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct netdev_rx_queue {
    struct xdp_rxq_info xdp_rxq;
    struct rps_map *rps_map;
    struct rps_dev_flow_table *rps_flow_table;
    struct kobject kobj;
    struct net_device *dev;
    struct xsk_buff_pool *pool;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct netdev_rx_queue {
    struct xdp_rxq_info xdp_rxq;
    struct rps_map *rps_map;
    struct rps_dev_flow_table *rps_flow_table;
    struct kobject kobj;
    struct net_device *dev;
    netdevice_tracker dev_tracker;
    struct xsk_buff_pool *pool;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct netdev_rx_queue {
    struct xdp_rxq_info xdp_rxq;
    struct rps_map *rps_map;
    struct rps_dev_flow_table *rps_flow_table;
    struct kobject kobj;
    struct net_device *dev;
    netdevice_tracker dev_tracker;
    struct xsk_buff_pool *pool;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct netdev_rx_queue {
    struct xdp_rxq_info xdp_rxq;
    struct rps_map *rps_map;
    struct rps_dev_flow_table *rps_flow_table;
    struct kobject kobj;
    struct net_device *dev;
    netdevice_tracker dev_tracker;
    struct xsk_buff_pool *pool;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct netdev_rx_queue {
    struct xdp_rxq_info xdp_rxq;
    struct rps_map *rps_map;
    struct rps_dev_flow_table *rps_flow_table;
    struct kobject kobj;
    struct net_device *dev;
    netdevice_tracker dev_tracker;
    struct xsk_buff_pool *pool;
    struct napi_struct *napi;
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
struct netdev_rx_queue {
    struct rps_map *rps_map;
    struct rps_dev_flow_table *rps_flow_table;
    struct kobject kobj;
    struct net_device *dev;
    struct xdp_rxq_info xdp_rxq;
    struct xdp_umem *umem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct netdev_rx_queue {
    struct rps_map *rps_map;
    struct rps_dev_flow_table *rps_flow_table;
    struct kobject kobj;
    struct net_device *dev;
    struct xdp_rxq_info xdp_rxq;
    struct xdp_umem *umem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct netdev_rx_queue {
    struct rps_map *rps_map;
    struct rps_dev_flow_table *rps_flow_table;
    struct kobject kobj;
    struct net_device *dev;
    struct xdp_rxq_info xdp_rxq;
    struct xdp_umem *umem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct netdev_rx_queue {
    struct rps_map *rps_map;
    struct rps_dev_flow_table *rps_flow_table;
    struct kobject kobj;
    struct net_device *dev;
    struct xdp_rxq_info xdp_rxq;
    struct xdp_umem *umem;
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
struct netdev_rx_queue {
    struct rps_map *rps_map;
    struct rps_dev_flow_table *rps_flow_table;
    struct kobject kobj;
    struct net_device *dev;
    struct xdp_rxq_info xdp_rxq;
    struct xdp_umem *umem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct netdev_rx_queue {
    struct rps_map *rps_map;
    struct rps_dev_flow_table *rps_flow_table;
    struct kobject kobj;
    struct net_device *dev;
    struct xdp_rxq_info xdp_rxq;
    struct xdp_umem *umem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct netdev_rx_queue {
    struct rps_map *rps_map;
    struct rps_dev_flow_table *rps_flow_table;
    struct kobject kobj;
    struct net_device *dev;
    struct xdp_rxq_info xdp_rxq;
    struct xdp_umem *umem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct netdev_rx_queue {
    struct rps_map *rps_map;
    struct rps_dev_flow_table *rps_flow_table;
    struct kobject kobj;
    struct net_device *dev;
    struct xdp_rxq_info xdp_rxq;
    struct xdp_umem *umem;
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
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct xdp_rxq_info xdp_rxq</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct xdp_umem *umem</code>
</li>
</ul>
</details>
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
<code>struct xsk_buff_pool *pool</code>
</li>
<li>
<b>Field removed. </b>
<code>struct xdp_umem *umem</code>
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
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct napi_struct *napi</code>
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
No changes between <code>amd64</code> and <code>armhf</code> ✅
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
