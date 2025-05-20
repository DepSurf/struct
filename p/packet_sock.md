# Struct: <code>packet_sock</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct packet_sock {
    struct sock sk;
    struct packet_fanout *fanout;
    union tpacket_stats_u stats;
    struct packet_ring_buffer rx_ring;
    struct packet_ring_buffer tx_ring;
    int copy_thresh;
    spinlock_t bind_lock;
    struct mutex pg_vec_lock;
    unsigned int running;
    unsigned int auxdata;
    unsigned int origdev;
    unsigned int has_vnet_hdr;
    int pressure;
    int ifindex;
    __be16 num;
    struct packet_rollover *rollover;
    struct packet_mclist *mclist;
    atomic_t mapped;
    enum tpacket_versions tp_version;
    unsigned int tp_hdrlen;
    unsigned int tp_reserve;
    unsigned int tp_loss;
    unsigned int tp_tx_has_off;
    unsigned int tp_tstamp;
    struct net_device *cached_dev;
    int (*xmit)(struct sk_buff *);
    struct packet_type prot_hook;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct packet_sock {
    struct sock sk;
    struct packet_fanout *fanout;
    union tpacket_stats_u stats;
    struct packet_ring_buffer rx_ring;
    struct packet_ring_buffer tx_ring;
    int copy_thresh;
    spinlock_t bind_lock;
    struct mutex pg_vec_lock;
    unsigned int running;
    unsigned int auxdata;
    unsigned int origdev;
    unsigned int has_vnet_hdr;
    int pressure;
    int ifindex;
    __be16 num;
    struct packet_rollover *rollover;
    struct packet_mclist *mclist;
    atomic_t mapped;
    enum tpacket_versions tp_version;
    unsigned int tp_hdrlen;
    unsigned int tp_reserve;
    unsigned int tp_loss;
    unsigned int tp_tx_has_off;
    unsigned int tp_tstamp;
    struct net_device *cached_dev;
    int (*xmit)(struct sk_buff *);
    struct packet_type prot_hook;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct packet_sock {
    struct sock sk;
    struct packet_fanout *fanout;
    union tpacket_stats_u stats;
    struct packet_ring_buffer rx_ring;
    struct packet_ring_buffer tx_ring;
    int copy_thresh;
    spinlock_t bind_lock;
    struct mutex pg_vec_lock;
    unsigned int running;
    unsigned int auxdata;
    unsigned int origdev;
    unsigned int has_vnet_hdr;
    int pressure;
    int ifindex;
    __be16 num;
    struct packet_rollover *rollover;
    struct packet_mclist *mclist;
    atomic_t mapped;
    enum tpacket_versions tp_version;
    unsigned int tp_hdrlen;
    unsigned int tp_reserve;
    unsigned int tp_loss;
    unsigned int tp_tx_has_off;
    unsigned int tp_tstamp;
    struct net_device *cached_dev;
    int (*xmit)(struct sk_buff *);
    struct packet_type prot_hook;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct packet_sock {
    struct sock sk;
    struct packet_fanout *fanout;
    union tpacket_stats_u stats;
    struct packet_ring_buffer rx_ring;
    struct packet_ring_buffer tx_ring;
    int copy_thresh;
    spinlock_t bind_lock;
    struct mutex pg_vec_lock;
    unsigned int running;
    unsigned int auxdata;
    unsigned int origdev;
    unsigned int has_vnet_hdr;
    int pressure;
    int ifindex;
    __be16 num;
    struct packet_rollover *rollover;
    struct packet_mclist *mclist;
    atomic_t mapped;
    enum tpacket_versions tp_version;
    unsigned int tp_hdrlen;
    unsigned int tp_reserve;
    unsigned int tp_loss;
    unsigned int tp_tx_has_off;
    unsigned int tp_tstamp;
    struct net_device *cached_dev;
    int (*xmit)(struct sk_buff *);
    struct packet_type prot_hook;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct packet_sock {
    struct sock sk;
    struct packet_fanout *fanout;
    union tpacket_stats_u stats;
    struct packet_ring_buffer rx_ring;
    struct packet_ring_buffer tx_ring;
    int copy_thresh;
    spinlock_t bind_lock;
    struct mutex pg_vec_lock;
    unsigned int running;
    unsigned int auxdata;
    unsigned int origdev;
    unsigned int has_vnet_hdr;
    int pressure;
    int ifindex;
    __be16 num;
    struct packet_rollover *rollover;
    struct packet_mclist *mclist;
    atomic_t mapped;
    enum tpacket_versions tp_version;
    unsigned int tp_hdrlen;
    unsigned int tp_reserve;
    unsigned int tp_loss;
    unsigned int tp_tx_has_off;
    unsigned int tp_tstamp;
    struct net_device *cached_dev;
    int (*xmit)(struct sk_buff *);
    struct packet_type prot_hook;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct packet_sock {
    struct sock sk;
    struct packet_fanout *fanout;
    union tpacket_stats_u stats;
    struct packet_ring_buffer rx_ring;
    struct packet_ring_buffer tx_ring;
    int copy_thresh;
    spinlock_t bind_lock;
    struct mutex pg_vec_lock;
    unsigned int running;
    unsigned int auxdata;
    unsigned int origdev;
    unsigned int has_vnet_hdr;
    unsigned int tp_loss;
    unsigned int tp_tx_has_off;
    int pressure;
    int ifindex;
    __be16 num;
    struct packet_rollover *rollover;
    struct packet_mclist *mclist;
    atomic_t mapped;
    enum tpacket_versions tp_version;
    unsigned int tp_hdrlen;
    unsigned int tp_reserve;
    unsigned int tp_tstamp;
    struct net_device *cached_dev;
    int (*xmit)(struct sk_buff *);
    struct packet_type prot_hook;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct packet_sock {
    struct sock sk;
    struct packet_fanout *fanout;
    union tpacket_stats_u stats;
    struct packet_ring_buffer rx_ring;
    struct packet_ring_buffer tx_ring;
    int copy_thresh;
    spinlock_t bind_lock;
    struct mutex pg_vec_lock;
    unsigned int running;
    unsigned int auxdata;
    unsigned int origdev;
    unsigned int has_vnet_hdr;
    unsigned int tp_loss;
    unsigned int tp_tx_has_off;
    int pressure;
    int ifindex;
    __be16 num;
    struct packet_rollover *rollover;
    struct packet_mclist *mclist;
    atomic_t mapped;
    enum tpacket_versions tp_version;
    unsigned int tp_hdrlen;
    unsigned int tp_reserve;
    unsigned int tp_tstamp;
    struct net_device *cached_dev;
    int (*xmit)(struct sk_buff *);
    struct packet_type prot_hook;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct packet_sock {
    struct sock sk;
    struct packet_fanout *fanout;
    union tpacket_stats_u stats;
    struct packet_ring_buffer rx_ring;
    struct packet_ring_buffer tx_ring;
    int copy_thresh;
    spinlock_t bind_lock;
    struct mutex pg_vec_lock;
    unsigned int running;
    unsigned int auxdata;
    unsigned int origdev;
    unsigned int has_vnet_hdr;
    unsigned int tp_loss;
    unsigned int tp_tx_has_off;
    int pressure;
    int ifindex;
    __be16 num;
    struct packet_rollover *rollover;
    struct packet_mclist *mclist;
    atomic_t mapped;
    enum tpacket_versions tp_version;
    unsigned int tp_hdrlen;
    unsigned int tp_reserve;
    unsigned int tp_tstamp;
    struct completion skb_completion;
    struct net_device *cached_dev;
    int (*xmit)(struct sk_buff *);
    struct packet_type prot_hook;
    atomic_t tp_drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct packet_sock {
    struct sock sk;
    struct packet_fanout *fanout;
    union tpacket_stats_u stats;
    struct packet_ring_buffer rx_ring;
    struct packet_ring_buffer tx_ring;
    int copy_thresh;
    spinlock_t bind_lock;
    struct mutex pg_vec_lock;
    unsigned int running;
    unsigned int auxdata;
    unsigned int origdev;
    unsigned int has_vnet_hdr;
    unsigned int tp_loss;
    unsigned int tp_tx_has_off;
    int pressure;
    int ifindex;
    __be16 num;
    struct packet_rollover *rollover;
    struct packet_mclist *mclist;
    atomic_t mapped;
    enum tpacket_versions tp_version;
    unsigned int tp_hdrlen;
    unsigned int tp_reserve;
    unsigned int tp_tstamp;
    struct completion skb_completion;
    struct net_device *cached_dev;
    int (*xmit)(struct sk_buff *);
    struct packet_type prot_hook;
    atomic_t tp_drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct packet_sock {
    struct sock sk;
    struct packet_fanout *fanout;
    union tpacket_stats_u stats;
    struct packet_ring_buffer rx_ring;
    struct packet_ring_buffer tx_ring;
    int copy_thresh;
    spinlock_t bind_lock;
    struct mutex pg_vec_lock;
    unsigned int running;
    unsigned int auxdata;
    unsigned int origdev;
    unsigned int has_vnet_hdr;
    unsigned int tp_loss;
    unsigned int tp_tx_has_off;
    int pressure;
    int ifindex;
    __be16 num;
    struct packet_rollover *rollover;
    struct packet_mclist *mclist;
    atomic_t mapped;
    enum tpacket_versions tp_version;
    unsigned int tp_hdrlen;
    unsigned int tp_reserve;
    unsigned int tp_tstamp;
    struct completion skb_completion;
    struct net_device *cached_dev;
    int (*xmit)(struct sk_buff *);
    struct packet_type prot_hook;
    atomic_t tp_drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct packet_sock {
    struct sock sk;
    struct packet_fanout *fanout;
    union tpacket_stats_u stats;
    struct packet_ring_buffer rx_ring;
    struct packet_ring_buffer tx_ring;
    int copy_thresh;
    spinlock_t bind_lock;
    struct mutex pg_vec_lock;
    unsigned int running;
    unsigned int auxdata;
    unsigned int origdev;
    unsigned int has_vnet_hdr;
    unsigned int tp_loss;
    unsigned int tp_tx_has_off;
    int pressure;
    int ifindex;
    __be16 num;
    struct packet_rollover *rollover;
    struct packet_mclist *mclist;
    atomic_t mapped;
    enum tpacket_versions tp_version;
    unsigned int tp_hdrlen;
    unsigned int tp_reserve;
    unsigned int tp_tstamp;
    struct completion skb_completion;
    struct net_device *cached_dev;
    int (*xmit)(struct sk_buff *);
    struct packet_type prot_hook;
    atomic_t tp_drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct packet_sock {
    struct sock sk;
    struct packet_fanout *fanout;
    union tpacket_stats_u stats;
    struct packet_ring_buffer rx_ring;
    struct packet_ring_buffer tx_ring;
    int copy_thresh;
    spinlock_t bind_lock;
    struct mutex pg_vec_lock;
    unsigned int running;
    unsigned int auxdata;
    unsigned int origdev;
    unsigned int has_vnet_hdr;
    unsigned int tp_loss;
    unsigned int tp_tx_has_off;
    int pressure;
    int ifindex;
    __be16 num;
    struct packet_rollover *rollover;
    struct packet_mclist *mclist;
    atomic_t mapped;
    enum tpacket_versions tp_version;
    unsigned int tp_hdrlen;
    unsigned int tp_reserve;
    unsigned int tp_tstamp;
    struct completion skb_completion;
    struct net_device *cached_dev;
    int (*xmit)(struct sk_buff *);
    struct packet_type prot_hook;
    atomic_t tp_drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct packet_sock {
    struct sock sk;
    struct packet_fanout *fanout;
    union tpacket_stats_u stats;
    struct packet_ring_buffer rx_ring;
    struct packet_ring_buffer tx_ring;
    int copy_thresh;
    spinlock_t bind_lock;
    struct mutex pg_vec_lock;
    unsigned int running;
    unsigned int auxdata;
    unsigned int origdev;
    unsigned int has_vnet_hdr;
    unsigned int tp_loss;
    unsigned int tp_tx_has_off;
    int pressure;
    int ifindex;
    __be16 num;
    struct packet_rollover *rollover;
    struct packet_mclist *mclist;
    atomic_t mapped;
    enum tpacket_versions tp_version;
    unsigned int tp_hdrlen;
    unsigned int tp_reserve;
    unsigned int tp_tstamp;
    struct completion skb_completion;
    struct net_device *cached_dev;
    int (*xmit)(struct sk_buff *);
    struct packet_type prot_hook;
    atomic_t tp_drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct packet_sock {
    struct sock sk;
    struct packet_fanout *fanout;
    union tpacket_stats_u stats;
    struct packet_ring_buffer rx_ring;
    struct packet_ring_buffer tx_ring;
    int copy_thresh;
    spinlock_t bind_lock;
    struct mutex pg_vec_lock;
    unsigned int running;
    unsigned int auxdata;
    unsigned int origdev;
    unsigned int has_vnet_hdr;
    unsigned int tp_loss;
    unsigned int tp_tx_has_off;
    int pressure;
    int ifindex;
    __be16 num;
    struct packet_rollover *rollover;
    struct packet_mclist *mclist;
    atomic_t mapped;
    enum tpacket_versions tp_version;
    unsigned int tp_hdrlen;
    unsigned int tp_reserve;
    unsigned int tp_tstamp;
    struct completion skb_completion;
    struct net_device *cached_dev;
    int (*xmit)(struct sk_buff *);
    struct packet_type prot_hook;
    atomic_t tp_drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct packet_sock {
    struct sock sk;
    struct packet_fanout *fanout;
    union tpacket_stats_u stats;
    struct packet_ring_buffer rx_ring;
    struct packet_ring_buffer tx_ring;
    int copy_thresh;
    spinlock_t bind_lock;
    struct mutex pg_vec_lock;
    unsigned int running;
    unsigned int auxdata;
    unsigned int origdev;
    unsigned int has_vnet_hdr;
    unsigned int tp_loss;
    unsigned int tp_tx_has_off;
    int pressure;
    int ifindex;
    __be16 num;
    struct packet_rollover *rollover;
    struct packet_mclist *mclist;
    atomic_t mapped;
    enum tpacket_versions tp_version;
    unsigned int tp_hdrlen;
    unsigned int tp_reserve;
    unsigned int tp_tstamp;
    struct completion skb_completion;
    struct net_device *cached_dev;
    int (*xmit)(struct sk_buff *);
    struct packet_type prot_hook;
    atomic_t tp_drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct packet_sock {
    struct sock sk;
    struct packet_fanout *fanout;
    union tpacket_stats_u stats;
    struct packet_ring_buffer rx_ring;
    struct packet_ring_buffer tx_ring;
    int copy_thresh;
    spinlock_t bind_lock;
    struct mutex pg_vec_lock;
    long unsigned int flags;
    int ifindex;
    u8 vnet_hdr_sz;
    __be16 num;
    struct packet_rollover *rollover;
    struct packet_mclist *mclist;
    atomic_t mapped;
    enum tpacket_versions tp_version;
    unsigned int tp_hdrlen;
    unsigned int tp_reserve;
    unsigned int tp_tstamp;
    struct completion skb_completion;
    struct net_device *cached_dev;
    struct packet_type prot_hook;
    atomic_t tp_drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct packet_sock {
    struct sock sk;
    struct packet_fanout *fanout;
    union tpacket_stats_u stats;
    struct packet_ring_buffer rx_ring;
    struct packet_ring_buffer tx_ring;
    int copy_thresh;
    spinlock_t bind_lock;
    struct mutex pg_vec_lock;
    long unsigned int flags;
    int ifindex;
    u8 vnet_hdr_sz;
    __be16 num;
    struct packet_rollover *rollover;
    struct packet_mclist *mclist;
    atomic_long_t mapped;
    enum tpacket_versions tp_version;
    unsigned int tp_hdrlen;
    unsigned int tp_reserve;
    unsigned int tp_tstamp;
    struct completion skb_completion;
    struct net_device *cached_dev;
    struct packet_type prot_hook;
    atomic_t tp_drops;
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
struct packet_sock {
    struct sock sk;
    struct packet_fanout *fanout;
    union tpacket_stats_u stats;
    struct packet_ring_buffer rx_ring;
    struct packet_ring_buffer tx_ring;
    int copy_thresh;
    spinlock_t bind_lock;
    struct mutex pg_vec_lock;
    unsigned int running;
    unsigned int auxdata;
    unsigned int origdev;
    unsigned int has_vnet_hdr;
    unsigned int tp_loss;
    unsigned int tp_tx_has_off;
    int pressure;
    int ifindex;
    __be16 num;
    struct packet_rollover *rollover;
    struct packet_mclist *mclist;
    atomic_t mapped;
    enum tpacket_versions tp_version;
    unsigned int tp_hdrlen;
    unsigned int tp_reserve;
    unsigned int tp_tstamp;
    struct completion skb_completion;
    struct net_device *cached_dev;
    int (*xmit)(struct sk_buff *);
    struct packet_type prot_hook;
    atomic_t tp_drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct packet_sock {
    struct sock sk;
    struct packet_fanout *fanout;
    union tpacket_stats_u stats;
    struct packet_ring_buffer rx_ring;
    struct packet_ring_buffer tx_ring;
    int copy_thresh;
    spinlock_t bind_lock;
    struct mutex pg_vec_lock;
    unsigned int running;
    unsigned int auxdata;
    unsigned int origdev;
    unsigned int has_vnet_hdr;
    unsigned int tp_loss;
    unsigned int tp_tx_has_off;
    int pressure;
    int ifindex;
    __be16 num;
    struct packet_rollover *rollover;
    struct packet_mclist *mclist;
    atomic_t mapped;
    enum tpacket_versions tp_version;
    unsigned int tp_hdrlen;
    unsigned int tp_reserve;
    unsigned int tp_tstamp;
    struct completion skb_completion;
    struct net_device *cached_dev;
    int (*xmit)(struct sk_buff *);
    struct packet_type prot_hook;
    atomic_t tp_drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct packet_sock {
    struct sock sk;
    struct packet_fanout *fanout;
    union tpacket_stats_u stats;
    struct packet_ring_buffer rx_ring;
    struct packet_ring_buffer tx_ring;
    int copy_thresh;
    spinlock_t bind_lock;
    struct mutex pg_vec_lock;
    unsigned int running;
    unsigned int auxdata;
    unsigned int origdev;
    unsigned int has_vnet_hdr;
    unsigned int tp_loss;
    unsigned int tp_tx_has_off;
    int pressure;
    int ifindex;
    __be16 num;
    struct packet_rollover *rollover;
    struct packet_mclist *mclist;
    atomic_t mapped;
    enum tpacket_versions tp_version;
    unsigned int tp_hdrlen;
    unsigned int tp_reserve;
    unsigned int tp_tstamp;
    struct completion skb_completion;
    struct net_device *cached_dev;
    int (*xmit)(struct sk_buff *);
    struct packet_type prot_hook;
    atomic_t tp_drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct packet_sock {
    struct sock sk;
    struct packet_fanout *fanout;
    union tpacket_stats_u stats;
    struct packet_ring_buffer rx_ring;
    struct packet_ring_buffer tx_ring;
    int copy_thresh;
    spinlock_t bind_lock;
    struct mutex pg_vec_lock;
    unsigned int running;
    unsigned int auxdata;
    unsigned int origdev;
    unsigned int has_vnet_hdr;
    unsigned int tp_loss;
    unsigned int tp_tx_has_off;
    int pressure;
    int ifindex;
    __be16 num;
    struct packet_rollover *rollover;
    struct packet_mclist *mclist;
    atomic_t mapped;
    enum tpacket_versions tp_version;
    unsigned int tp_hdrlen;
    unsigned int tp_reserve;
    unsigned int tp_tstamp;
    struct completion skb_completion;
    struct net_device *cached_dev;
    int (*xmit)(struct sk_buff *);
    struct packet_type prot_hook;
    atomic_t tp_drops;
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
struct packet_sock {
    struct sock sk;
    struct packet_fanout *fanout;
    union tpacket_stats_u stats;
    struct packet_ring_buffer rx_ring;
    struct packet_ring_buffer tx_ring;
    int copy_thresh;
    spinlock_t bind_lock;
    struct mutex pg_vec_lock;
    unsigned int running;
    unsigned int auxdata;
    unsigned int origdev;
    unsigned int has_vnet_hdr;
    unsigned int tp_loss;
    unsigned int tp_tx_has_off;
    int pressure;
    int ifindex;
    __be16 num;
    struct packet_rollover *rollover;
    struct packet_mclist *mclist;
    atomic_t mapped;
    enum tpacket_versions tp_version;
    unsigned int tp_hdrlen;
    unsigned int tp_reserve;
    unsigned int tp_tstamp;
    struct completion skb_completion;
    struct net_device *cached_dev;
    int (*xmit)(struct sk_buff *);
    struct packet_type prot_hook;
    atomic_t tp_drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct packet_sock {
    struct sock sk;
    struct packet_fanout *fanout;
    union tpacket_stats_u stats;
    struct packet_ring_buffer rx_ring;
    struct packet_ring_buffer tx_ring;
    int copy_thresh;
    spinlock_t bind_lock;
    struct mutex pg_vec_lock;
    unsigned int running;
    unsigned int auxdata;
    unsigned int origdev;
    unsigned int has_vnet_hdr;
    unsigned int tp_loss;
    unsigned int tp_tx_has_off;
    int pressure;
    int ifindex;
    __be16 num;
    struct packet_rollover *rollover;
    struct packet_mclist *mclist;
    atomic_t mapped;
    enum tpacket_versions tp_version;
    unsigned int tp_hdrlen;
    unsigned int tp_reserve;
    unsigned int tp_tstamp;
    struct completion skb_completion;
    struct net_device *cached_dev;
    int (*xmit)(struct sk_buff *);
    struct packet_type prot_hook;
    atomic_t tp_drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct packet_sock {
    struct sock sk;
    struct packet_fanout *fanout;
    union tpacket_stats_u stats;
    struct packet_ring_buffer rx_ring;
    struct packet_ring_buffer tx_ring;
    int copy_thresh;
    spinlock_t bind_lock;
    struct mutex pg_vec_lock;
    unsigned int running;
    unsigned int auxdata;
    unsigned int origdev;
    unsigned int has_vnet_hdr;
    unsigned int tp_loss;
    unsigned int tp_tx_has_off;
    int pressure;
    int ifindex;
    __be16 num;
    struct packet_rollover *rollover;
    struct packet_mclist *mclist;
    atomic_t mapped;
    enum tpacket_versions tp_version;
    unsigned int tp_hdrlen;
    unsigned int tp_reserve;
    unsigned int tp_tstamp;
    struct completion skb_completion;
    struct net_device *cached_dev;
    int (*xmit)(struct sk_buff *);
    struct packet_type prot_hook;
    atomic_t tp_drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct packet_sock {
    struct sock sk;
    struct packet_fanout *fanout;
    union tpacket_stats_u stats;
    struct packet_ring_buffer rx_ring;
    struct packet_ring_buffer tx_ring;
    int copy_thresh;
    spinlock_t bind_lock;
    struct mutex pg_vec_lock;
    unsigned int running;
    unsigned int auxdata;
    unsigned int origdev;
    unsigned int has_vnet_hdr;
    unsigned int tp_loss;
    unsigned int tp_tx_has_off;
    int pressure;
    int ifindex;
    __be16 num;
    struct packet_rollover *rollover;
    struct packet_mclist *mclist;
    atomic_t mapped;
    enum tpacket_versions tp_version;
    unsigned int tp_hdrlen;
    unsigned int tp_reserve;
    unsigned int tp_tstamp;
    struct completion skb_completion;
    struct net_device *cached_dev;
    int (*xmit)(struct sk_buff *);
    struct packet_type prot_hook;
    atomic_t tp_drops;
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct completion skb_completion</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t tp_drops</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int flags</code>
</li>
<li>
<b>Field added. </b>
<code>u8 vnet_hdr_sz</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int running</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int auxdata</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int origdev</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int has_vnet_hdr</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int tp_loss</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int tp_tx_has_off</code>
</li>
<li>
<b>Field removed. </b>
<code>int pressure</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*xmit)(struct sk_buff *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>atomic_t mapped</code> ➡️ <code>atomic_long_t mapped</code>
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
