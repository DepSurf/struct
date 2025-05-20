# Struct: <code>xdp_sock</code>

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
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct xdp_sock {
    struct sock sk;
    struct xsk_queue *rx;
    struct net_device *dev;
    struct xdp_umem *umem;
    struct list_head flush_node;
    u16 queue_id;
    struct xsk_queue *tx;
    struct list_head list;
    bool zc;
    struct mutex mutex;
    spinlock_t tx_completion_lock;
    u64 rx_dropped;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct xdp_sock {
    struct sock sk;
    struct xsk_queue *rx;
    struct net_device *dev;
    struct xdp_umem *umem;
    struct list_head flush_node;
    u16 queue_id;
    struct xsk_queue *tx;
    struct list_head list;
    bool zc;
    struct mutex mutex;
    spinlock_t tx_completion_lock;
    u64 rx_dropped;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct xdp_sock {
    struct sock sk;
    struct xsk_queue *rx;
    struct net_device *dev;
    struct xdp_umem *umem;
    struct list_head flush_node;
    u16 queue_id;
    bool zc;
    enum (anon) state;
    struct mutex mutex;
    struct xsk_queue *tx;
    struct list_head list;
    spinlock_t tx_completion_lock;
    spinlock_t rx_lock;
    u64 rx_dropped;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct xdp_sock {
    struct sock sk;
    struct xsk_queue *rx;
    struct net_device *dev;
    struct xdp_umem *umem;
    struct list_head flush_node;
    u16 queue_id;
    bool zc;
    enum (anon) state;
    struct mutex mutex;
    struct xsk_queue *tx;
    struct list_head list;
    spinlock_t tx_completion_lock;
    spinlock_t rx_lock;
    u64 rx_dropped;
    struct list_head map_list;
    spinlock_t map_list_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct xdp_sock {
    struct sock sk;
    struct xsk_queue *rx;
    struct net_device *dev;
    struct xdp_umem *umem;
    struct list_head flush_node;
    u16 queue_id;
    bool zc;
    enum (anon) state;
    struct mutex mutex;
    struct xsk_queue *tx;
    struct list_head list;
    spinlock_t tx_completion_lock;
    spinlock_t rx_lock;
    u64 rx_dropped;
    struct list_head map_list;
    spinlock_t map_list_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct xdp_sock {
    struct sock sk;
    struct xsk_queue *rx;
    struct net_device *dev;
    struct xdp_umem *umem;
    struct list_head flush_node;
    struct xsk_buff_pool *pool;
    u16 queue_id;
    bool zc;
    enum (anon) state;
    struct xsk_queue *tx;
    struct list_head tx_list;
    spinlock_t rx_lock;
    u64 rx_dropped;
    u64 rx_queue_full;
    struct list_head map_list;
    spinlock_t map_list_lock;
    struct mutex mutex;
    struct xsk_queue *fq_tmp;
    struct xsk_queue *cq_tmp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct xdp_sock {
    struct sock sk;
    struct xsk_queue *rx;
    struct net_device *dev;
    struct xdp_umem *umem;
    struct list_head flush_node;
    struct xsk_buff_pool *pool;
    u16 queue_id;
    bool zc;
    enum (anon) state;
    struct xsk_queue *tx;
    struct list_head tx_list;
    spinlock_t rx_lock;
    u64 rx_dropped;
    u64 rx_queue_full;
    struct list_head map_list;
    spinlock_t map_list_lock;
    struct mutex mutex;
    struct xsk_queue *fq_tmp;
    struct xsk_queue *cq_tmp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct xdp_sock {
    struct sock sk;
    struct xsk_queue *rx;
    struct net_device *dev;
    struct xdp_umem *umem;
    struct list_head flush_node;
    struct xsk_buff_pool *pool;
    u16 queue_id;
    bool zc;
    enum (anon) state;
    struct xsk_queue *tx;
    struct list_head tx_list;
    spinlock_t rx_lock;
    u64 rx_dropped;
    u64 rx_queue_full;
    struct list_head map_list;
    spinlock_t map_list_lock;
    struct mutex mutex;
    struct xsk_queue *fq_tmp;
    struct xsk_queue *cq_tmp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct xdp_sock {
    struct sock sk;
    struct xsk_queue *rx;
    struct net_device *dev;
    struct xdp_umem *umem;
    struct list_head flush_node;
    struct xsk_buff_pool *pool;
    u16 queue_id;
    bool zc;
    enum (anon) state;
    struct xsk_queue *tx;
    struct list_head tx_list;
    spinlock_t rx_lock;
    u64 rx_dropped;
    u64 rx_queue_full;
    struct list_head map_list;
    spinlock_t map_list_lock;
    struct mutex mutex;
    struct xsk_queue *fq_tmp;
    struct xsk_queue *cq_tmp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct xdp_sock {
    struct sock sk;
    struct xsk_queue *rx;
    struct net_device *dev;
    struct xdp_umem *umem;
    struct list_head flush_node;
    struct xsk_buff_pool *pool;
    u16 queue_id;
    bool zc;
    enum (anon) state;
    struct xsk_queue *tx;
    struct list_head tx_list;
    spinlock_t rx_lock;
    u64 rx_dropped;
    u64 rx_queue_full;
    struct list_head map_list;
    spinlock_t map_list_lock;
    struct mutex mutex;
    struct xsk_queue *fq_tmp;
    struct xsk_queue *cq_tmp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct xdp_sock {
    struct sock sk;
    struct xsk_queue *rx;
    struct net_device *dev;
    struct xdp_umem *umem;
    struct list_head flush_node;
    struct xsk_buff_pool *pool;
    u16 queue_id;
    bool zc;
    enum (anon) state;
    struct xsk_queue *tx;
    struct list_head tx_list;
    spinlock_t rx_lock;
    u64 rx_dropped;
    u64 rx_queue_full;
    struct list_head map_list;
    spinlock_t map_list_lock;
    struct mutex mutex;
    struct xsk_queue *fq_tmp;
    struct xsk_queue *cq_tmp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct xdp_sock {
    struct sock sk;
    struct xsk_queue *rx;
    struct net_device *dev;
    struct xdp_umem *umem;
    struct list_head flush_node;
    struct xsk_buff_pool *pool;
    u16 queue_id;
    bool zc;
    bool sg;
    enum (anon) state;
    struct xsk_queue *tx;
    struct list_head tx_list;
    u32 tx_budget_spent;
    spinlock_t rx_lock;
    u64 rx_dropped;
    u64 rx_queue_full;
    struct sk_buff *skb;
    struct list_head map_list;
    spinlock_t map_list_lock;
    struct mutex mutex;
    struct xsk_queue *fq_tmp;
    struct xsk_queue *cq_tmp;
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
struct xdp_sock {
    struct sock sk;
    struct xsk_queue *rx;
    struct net_device *dev;
    struct xdp_umem *umem;
    struct list_head flush_node;
    u16 queue_id;
    bool zc;
    enum (anon) state;
    struct mutex mutex;
    struct xsk_queue *tx;
    struct list_head list;
    spinlock_t tx_completion_lock;
    spinlock_t rx_lock;
    u64 rx_dropped;
    struct list_head map_list;
    spinlock_t map_list_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct xdp_sock {
    struct sock sk;
    struct xsk_queue *rx;
    struct net_device *dev;
    struct xdp_umem *umem;
    struct list_head flush_node;
    u16 queue_id;
    bool zc;
    enum (anon) state;
    struct mutex mutex;
    struct xsk_queue *tx;
    struct list_head list;
    spinlock_t tx_completion_lock;
    spinlock_t rx_lock;
    u64 rx_dropped;
    struct list_head map_list;
    spinlock_t map_list_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct xdp_sock {
    struct sock sk;
    struct xsk_queue *rx;
    struct net_device *dev;
    struct xdp_umem *umem;
    struct list_head flush_node;
    u16 queue_id;
    bool zc;
    enum (anon) state;
    struct mutex mutex;
    struct xsk_queue *tx;
    struct list_head list;
    spinlock_t tx_completion_lock;
    spinlock_t rx_lock;
    u64 rx_dropped;
    struct list_head map_list;
    spinlock_t map_list_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct xdp_sock {
    struct sock sk;
    struct xsk_queue *rx;
    struct net_device *dev;
    struct xdp_umem *umem;
    struct list_head flush_node;
    u16 queue_id;
    bool zc;
    enum (anon) state;
    struct mutex mutex;
    struct xsk_queue *tx;
    struct list_head list;
    spinlock_t tx_completion_lock;
    spinlock_t rx_lock;
    u64 rx_dropped;
    struct list_head map_list;
    spinlock_t map_list_lock;
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
struct xdp_sock {
    struct sock sk;
    struct xsk_queue *rx;
    struct net_device *dev;
    struct xdp_umem *umem;
    struct list_head flush_node;
    u16 queue_id;
    bool zc;
    enum (anon) state;
    struct mutex mutex;
    struct xsk_queue *tx;
    struct list_head list;
    spinlock_t tx_completion_lock;
    spinlock_t rx_lock;
    u64 rx_dropped;
    struct list_head map_list;
    spinlock_t map_list_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct xdp_sock {
    struct sock sk;
    struct xsk_queue *rx;
    struct net_device *dev;
    struct xdp_umem *umem;
    struct list_head flush_node;
    u16 queue_id;
    bool zc;
    enum (anon) state;
    struct mutex mutex;
    struct xsk_queue *tx;
    struct list_head list;
    spinlock_t tx_completion_lock;
    spinlock_t rx_lock;
    u64 rx_dropped;
    struct list_head map_list;
    spinlock_t map_list_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct xdp_sock {
    struct sock sk;
    struct xsk_queue *rx;
    struct net_device *dev;
    struct xdp_umem *umem;
    struct list_head flush_node;
    u16 queue_id;
    bool zc;
    enum (anon) state;
    struct mutex mutex;
    struct xsk_queue *tx;
    struct list_head list;
    spinlock_t tx_completion_lock;
    spinlock_t rx_lock;
    u64 rx_dropped;
    struct list_head map_list;
    spinlock_t map_list_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct xdp_sock {
    struct sock sk;
    struct xsk_queue *rx;
    struct net_device *dev;
    struct xdp_umem *umem;
    struct list_head flush_node;
    u16 queue_id;
    bool zc;
    enum (anon) state;
    struct mutex mutex;
    struct xsk_queue *tx;
    struct list_head list;
    spinlock_t tx_completion_lock;
    spinlock_t rx_lock;
    u64 rx_dropped;
    struct list_head map_list;
    spinlock_t map_list_lock;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>enum (anon) state</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t rx_lock</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head map_list</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t map_list_lock</code>
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
<code>struct xsk_buff_pool *pool</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head tx_list</code>
</li>
<li>
<b>Field added. </b>
<code>u64 rx_queue_full</code>
</li>
<li>
<b>Field added. </b>
<code>struct xsk_queue *fq_tmp</code>
</li>
<li>
<b>Field added. </b>
<code>struct xsk_queue *cq_tmp</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head list</code>
</li>
<li>
<b>Field removed. </b>
<code>spinlock_t tx_completion_lock</code>
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
<b>Field added. </b>
<code>bool sg</code>
</li>
<li>
<b>Field added. </b>
<code>u32 tx_budget_spent</code>
</li>
<li>
<b>Field added. </b>
<code>struct sk_buff *skb</code>
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
