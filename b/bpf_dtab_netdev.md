# Struct: <code>bpf_dtab_netdev</code>

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
struct bpf_dtab_netdev {
    struct net_device *dev;
    struct bpf_dtab *dtab;
    unsigned int bit;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct bpf_dtab_netdev {
    struct net_device *dev;
    struct bpf_dtab *dtab;
    unsigned int bit;
    struct xdp_bulk_queue *bulkq;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct bpf_dtab_netdev {
    struct net_device *dev;
    struct bpf_dtab *dtab;
    unsigned int bit;
    struct xdp_bulk_queue *bulkq;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct bpf_dtab_netdev {
    struct net_device *dev;
    struct bpf_dtab *dtab;
    unsigned int bit;
    struct xdp_bulk_queue *bulkq;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct bpf_dtab_netdev {
    struct net_device *dev;
    struct hlist_node index_hlist;
    struct bpf_dtab *dtab;
    struct xdp_bulk_queue *bulkq;
    struct callback_head rcu;
    unsigned int idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct bpf_dtab_netdev {
    struct net_device *dev;
    struct hlist_node index_hlist;
    struct bpf_dtab *dtab;
    struct bpf_prog *xdp_prog;
    struct callback_head rcu;
    unsigned int idx;
    struct bpf_devmap_val val;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct bpf_dtab_netdev {
    struct net_device *dev;
    struct hlist_node index_hlist;
    struct bpf_dtab *dtab;
    struct bpf_prog *xdp_prog;
    struct callback_head rcu;
    unsigned int idx;
    struct bpf_devmap_val val;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct bpf_dtab_netdev {
    struct net_device *dev;
    struct hlist_node index_hlist;
    struct bpf_dtab *dtab;
    struct bpf_prog *xdp_prog;
    struct callback_head rcu;
    unsigned int idx;
    struct bpf_devmap_val val;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct bpf_dtab_netdev {
    struct net_device *dev;
    struct hlist_node index_hlist;
    struct bpf_dtab *dtab;
    struct bpf_prog *xdp_prog;
    struct callback_head rcu;
    unsigned int idx;
    struct bpf_devmap_val val;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct bpf_dtab_netdev {
    struct net_device *dev;
    struct hlist_node index_hlist;
    struct bpf_dtab *dtab;
    struct bpf_prog *xdp_prog;
    struct callback_head rcu;
    unsigned int idx;
    struct bpf_devmap_val val;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct bpf_dtab_netdev {
    struct net_device *dev;
    struct hlist_node index_hlist;
    struct bpf_dtab *dtab;
    struct bpf_prog *xdp_prog;
    struct callback_head rcu;
    unsigned int idx;
    struct bpf_devmap_val val;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct bpf_dtab_netdev {
    struct net_device *dev;
    struct hlist_node index_hlist;
    struct bpf_dtab *dtab;
    struct bpf_prog *xdp_prog;
    struct callback_head rcu;
    unsigned int idx;
    struct bpf_devmap_val val;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct bpf_dtab_netdev {
    struct net_device *dev;
    struct hlist_node index_hlist;
    struct bpf_prog *xdp_prog;
    struct callback_head rcu;
    unsigned int idx;
    struct bpf_devmap_val val;
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
struct bpf_dtab_netdev {
    struct net_device *dev;
    struct hlist_node index_hlist;
    struct bpf_dtab *dtab;
    struct xdp_bulk_queue *bulkq;
    struct callback_head rcu;
    unsigned int idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct bpf_dtab_netdev {
    struct net_device *dev;
    struct hlist_node index_hlist;
    struct bpf_dtab *dtab;
    struct xdp_bulk_queue *bulkq;
    struct callback_head rcu;
    unsigned int idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct bpf_dtab_netdev {
    struct net_device *dev;
    struct hlist_node index_hlist;
    struct bpf_dtab *dtab;
    struct xdp_bulk_queue *bulkq;
    struct callback_head rcu;
    unsigned int idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct bpf_dtab_netdev {
    struct net_device *dev;
    struct hlist_node index_hlist;
    struct bpf_dtab *dtab;
    struct xdp_bulk_queue *bulkq;
    struct callback_head rcu;
    unsigned int idx;
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
struct bpf_dtab_netdev {
    struct net_device *dev;
    struct hlist_node index_hlist;
    struct bpf_dtab *dtab;
    struct xdp_bulk_queue *bulkq;
    struct callback_head rcu;
    unsigned int idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct bpf_dtab_netdev {
    struct net_device *dev;
    struct hlist_node index_hlist;
    struct bpf_dtab *dtab;
    struct xdp_bulk_queue *bulkq;
    struct callback_head rcu;
    unsigned int idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct bpf_dtab_netdev {
    struct net_device *dev;
    struct hlist_node index_hlist;
    struct bpf_dtab *dtab;
    struct xdp_bulk_queue *bulkq;
    struct callback_head rcu;
    unsigned int idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct bpf_dtab_netdev {
    struct net_device *dev;
    struct hlist_node index_hlist;
    struct bpf_dtab *dtab;
    struct xdp_bulk_queue *bulkq;
    struct callback_head rcu;
    unsigned int idx;
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
<code>struct xdp_bulk_queue *bulkq</code>
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
<b>Field added. </b>
<code>struct hlist_node index_hlist</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int idx</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int bit</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct bpf_prog *xdp_prog</code>
</li>
<li>
<b>Field added. </b>
<code>struct bpf_devmap_val val</code>
</li>
<li>
<b>Field removed. </b>
<code>struct xdp_bulk_queue *bulkq</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
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
<b>Field removed. </b>
<code>struct bpf_dtab *dtab</code>
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
