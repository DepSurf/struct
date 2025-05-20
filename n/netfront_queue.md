# Struct: <code>netfront_queue</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct netfront_queue {
    unsigned int id;
    char name[22];
    struct netfront_info *info;
    struct napi_struct napi;
    unsigned int tx_evtchn;
    unsigned int rx_evtchn;
    unsigned int tx_irq;
    unsigned int rx_irq;
    char tx_irq_name[25];
    char rx_irq_name[25];
    spinlock_t tx_lock;
    struct xen_netif_tx_front_ring tx;
    int tx_ring_ref;
    union skb_entry tx_skbs[256];
    grant_ref_t gref_tx_head;
    grant_ref_t grant_tx_ref[256];
    struct page * grant_tx_page[256];
    unsigned int tx_skb_freelist;
    spinlock_t rx_lock;
    struct xen_netif_rx_front_ring rx;
    int rx_ring_ref;
    struct timer_list rx_refill_timer;
    struct sk_buff * rx_skbs[256];
    grant_ref_t gref_rx_head;
    grant_ref_t grant_rx_ref[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct netfront_queue {
    unsigned int id;
    char name[22];
    struct netfront_info *info;
    struct napi_struct napi;
    unsigned int tx_evtchn;
    unsigned int rx_evtchn;
    unsigned int tx_irq;
    unsigned int rx_irq;
    char tx_irq_name[25];
    char rx_irq_name[25];
    spinlock_t tx_lock;
    struct xen_netif_tx_front_ring tx;
    int tx_ring_ref;
    union skb_entry tx_skbs[256];
    grant_ref_t gref_tx_head;
    grant_ref_t grant_tx_ref[256];
    struct page * grant_tx_page[256];
    unsigned int tx_skb_freelist;
    spinlock_t rx_lock;
    struct xen_netif_rx_front_ring rx;
    int rx_ring_ref;
    struct timer_list rx_refill_timer;
    struct sk_buff * rx_skbs[256];
    grant_ref_t gref_rx_head;
    grant_ref_t grant_rx_ref[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct netfront_queue {
    unsigned int id;
    char name[22];
    struct netfront_info *info;
    struct napi_struct napi;
    unsigned int tx_evtchn;
    unsigned int rx_evtchn;
    unsigned int tx_irq;
    unsigned int rx_irq;
    char tx_irq_name[25];
    char rx_irq_name[25];
    spinlock_t tx_lock;
    struct xen_netif_tx_front_ring tx;
    int tx_ring_ref;
    union skb_entry tx_skbs[256];
    grant_ref_t gref_tx_head;
    grant_ref_t grant_tx_ref[256];
    struct page * grant_tx_page[256];
    unsigned int tx_skb_freelist;
    spinlock_t rx_lock;
    struct xen_netif_rx_front_ring rx;
    int rx_ring_ref;
    struct timer_list rx_refill_timer;
    struct sk_buff * rx_skbs[256];
    grant_ref_t gref_rx_head;
    grant_ref_t grant_rx_ref[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct netfront_queue {
    unsigned int id;
    char name[22];
    struct netfront_info *info;
    struct napi_struct napi;
    unsigned int tx_evtchn;
    unsigned int rx_evtchn;
    unsigned int tx_irq;
    unsigned int rx_irq;
    char tx_irq_name[25];
    char rx_irq_name[25];
    spinlock_t tx_lock;
    struct xen_netif_tx_front_ring tx;
    int tx_ring_ref;
    union skb_entry tx_skbs[256];
    grant_ref_t gref_tx_head;
    grant_ref_t grant_tx_ref[256];
    struct page * grant_tx_page[256];
    unsigned int tx_skb_freelist;
    spinlock_t rx_lock;
    struct xen_netif_rx_front_ring rx;
    int rx_ring_ref;
    struct timer_list rx_refill_timer;
    struct sk_buff * rx_skbs[256];
    grant_ref_t gref_rx_head;
    grant_ref_t grant_rx_ref[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct netfront_queue {
    unsigned int id;
    char name[22];
    struct netfront_info *info;
    struct napi_struct napi;
    unsigned int tx_evtchn;
    unsigned int rx_evtchn;
    unsigned int tx_irq;
    unsigned int rx_irq;
    char tx_irq_name[25];
    char rx_irq_name[25];
    spinlock_t tx_lock;
    struct xen_netif_tx_front_ring tx;
    int tx_ring_ref;
    union skb_entry tx_skbs[256];
    grant_ref_t gref_tx_head;
    grant_ref_t grant_tx_ref[256];
    struct page * grant_tx_page[256];
    unsigned int tx_skb_freelist;
    spinlock_t rx_lock;
    struct xen_netif_rx_front_ring rx;
    int rx_ring_ref;
    struct timer_list rx_refill_timer;
    struct sk_buff * rx_skbs[256];
    grant_ref_t gref_rx_head;
    grant_ref_t grant_rx_ref[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct netfront_queue {
    unsigned int id;
    char name[22];
    struct netfront_info *info;
    struct napi_struct napi;
    unsigned int tx_evtchn;
    unsigned int rx_evtchn;
    unsigned int tx_irq;
    unsigned int rx_irq;
    char tx_irq_name[25];
    char rx_irq_name[25];
    spinlock_t tx_lock;
    struct xen_netif_tx_front_ring tx;
    int tx_ring_ref;
    union skb_entry tx_skbs[256];
    grant_ref_t gref_tx_head;
    grant_ref_t grant_tx_ref[256];
    struct page * grant_tx_page[256];
    unsigned int tx_skb_freelist;
    spinlock_t rx_lock;
    struct xen_netif_rx_front_ring rx;
    int rx_ring_ref;
    struct timer_list rx_refill_timer;
    struct sk_buff * rx_skbs[256];
    grant_ref_t gref_rx_head;
    grant_ref_t grant_rx_ref[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct netfront_queue {
    unsigned int id;
    char name[22];
    struct netfront_info *info;
    struct napi_struct napi;
    unsigned int tx_evtchn;
    unsigned int rx_evtchn;
    unsigned int tx_irq;
    unsigned int rx_irq;
    char tx_irq_name[25];
    char rx_irq_name[25];
    spinlock_t tx_lock;
    struct xen_netif_tx_front_ring tx;
    int tx_ring_ref;
    union skb_entry tx_skbs[256];
    grant_ref_t gref_tx_head;
    grant_ref_t grant_tx_ref[256];
    struct page * grant_tx_page[256];
    unsigned int tx_skb_freelist;
    spinlock_t rx_lock;
    struct xen_netif_rx_front_ring rx;
    int rx_ring_ref;
    struct timer_list rx_refill_timer;
    struct sk_buff * rx_skbs[256];
    grant_ref_t gref_rx_head;
    grant_ref_t grant_rx_ref[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct netfront_queue {
    unsigned int id;
    char name[22];
    struct netfront_info *info;
    struct napi_struct napi;
    unsigned int tx_evtchn;
    unsigned int rx_evtchn;
    unsigned int tx_irq;
    unsigned int rx_irq;
    char tx_irq_name[25];
    char rx_irq_name[25];
    spinlock_t tx_lock;
    struct xen_netif_tx_front_ring tx;
    int tx_ring_ref;
    union skb_entry tx_skbs[256];
    grant_ref_t gref_tx_head;
    grant_ref_t grant_tx_ref[256];
    struct page * grant_tx_page[256];
    unsigned int tx_skb_freelist;
    spinlock_t rx_lock;
    struct xen_netif_rx_front_ring rx;
    int rx_ring_ref;
    struct timer_list rx_refill_timer;
    struct sk_buff * rx_skbs[256];
    grant_ref_t gref_rx_head;
    grant_ref_t grant_rx_ref[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct netfront_queue {
    unsigned int id;
    char name[22];
    struct netfront_info *info;
    struct napi_struct napi;
    unsigned int tx_evtchn;
    unsigned int rx_evtchn;
    unsigned int tx_irq;
    unsigned int rx_irq;
    char tx_irq_name[25];
    char rx_irq_name[25];
    spinlock_t tx_lock;
    struct xen_netif_tx_front_ring tx;
    int tx_ring_ref;
    union skb_entry tx_skbs[256];
    grant_ref_t gref_tx_head;
    grant_ref_t grant_tx_ref[256];
    struct page * grant_tx_page[256];
    unsigned int tx_skb_freelist;
    spinlock_t rx_lock;
    struct xen_netif_rx_front_ring rx;
    int rx_ring_ref;
    struct timer_list rx_refill_timer;
    struct sk_buff * rx_skbs[256];
    grant_ref_t gref_rx_head;
    grant_ref_t grant_rx_ref[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct netfront_queue {
    unsigned int id;
    char name[22];
    struct netfront_info *info;
    struct napi_struct napi;
    unsigned int tx_evtchn;
    unsigned int rx_evtchn;
    unsigned int tx_irq;
    unsigned int rx_irq;
    char tx_irq_name[25];
    char rx_irq_name[25];
    spinlock_t tx_lock;
    struct xen_netif_tx_front_ring tx;
    int tx_ring_ref;
    union skb_entry tx_skbs[256];
    grant_ref_t gref_tx_head;
    grant_ref_t grant_tx_ref[256];
    struct page * grant_tx_page[256];
    unsigned int tx_skb_freelist;
    spinlock_t rx_lock;
    struct xen_netif_rx_front_ring rx;
    int rx_ring_ref;
    struct timer_list rx_refill_timer;
    struct sk_buff * rx_skbs[256];
    grant_ref_t gref_rx_head;
    grant_ref_t grant_rx_ref[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct netfront_queue {
    unsigned int id;
    char name[22];
    struct netfront_info *info;
    struct bpf_prog *xdp_prog;
    struct napi_struct napi;
    unsigned int tx_evtchn;
    unsigned int rx_evtchn;
    unsigned int tx_irq;
    unsigned int rx_irq;
    char tx_irq_name[25];
    char rx_irq_name[25];
    spinlock_t tx_lock;
    struct xen_netif_tx_front_ring tx;
    int tx_ring_ref;
    union skb_entry tx_skbs[256];
    grant_ref_t gref_tx_head;
    grant_ref_t grant_tx_ref[256];
    struct page * grant_tx_page[256];
    unsigned int tx_skb_freelist;
    spinlock_t rx_lock;
    struct xen_netif_rx_front_ring rx;
    int rx_ring_ref;
    struct timer_list rx_refill_timer;
    struct sk_buff * rx_skbs[256];
    grant_ref_t gref_rx_head;
    grant_ref_t grant_rx_ref[256];
    struct page_pool *page_pool;
    struct xdp_rxq_info xdp_rxq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct netfront_queue {
    unsigned int id;
    char name[22];
    struct netfront_info *info;
    struct bpf_prog *xdp_prog;
    struct napi_struct napi;
    unsigned int tx_evtchn;
    unsigned int rx_evtchn;
    unsigned int tx_irq;
    unsigned int rx_irq;
    char tx_irq_name[25];
    char rx_irq_name[25];
    spinlock_t tx_lock;
    struct xen_netif_tx_front_ring tx;
    int tx_ring_ref;
    union skb_entry tx_skbs[256];
    grant_ref_t gref_tx_head;
    grant_ref_t grant_tx_ref[256];
    struct page * grant_tx_page[256];
    unsigned int tx_skb_freelist;
    spinlock_t rx_lock;
    struct xen_netif_rx_front_ring rx;
    int rx_ring_ref;
    struct timer_list rx_refill_timer;
    struct sk_buff * rx_skbs[256];
    grant_ref_t gref_rx_head;
    grant_ref_t grant_rx_ref[256];
    struct page_pool *page_pool;
    struct xdp_rxq_info xdp_rxq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct netfront_queue {
    unsigned int id;
    char name[22];
    struct netfront_info *info;
    struct bpf_prog *xdp_prog;
    struct napi_struct napi;
    unsigned int tx_evtchn;
    unsigned int rx_evtchn;
    unsigned int tx_irq;
    unsigned int rx_irq;
    char tx_irq_name[25];
    char rx_irq_name[25];
    spinlock_t tx_lock;
    struct xen_netif_tx_front_ring tx;
    int tx_ring_ref;
    struct sk_buff * tx_skbs[256];
    short unsigned int tx_link[256];
    grant_ref_t gref_tx_head;
    grant_ref_t grant_tx_ref[256];
    struct page * grant_tx_page[256];
    unsigned int tx_skb_freelist;
    unsigned int tx_pend_queue;
    spinlock_t rx_lock;
    struct xen_netif_rx_front_ring rx;
    int rx_ring_ref;
    struct timer_list rx_refill_timer;
    struct sk_buff * rx_skbs[256];
    grant_ref_t gref_rx_head;
    grant_ref_t grant_rx_ref[256];
    unsigned int rx_rsp_unconsumed;
    spinlock_t rx_cons_lock;
    struct page_pool *page_pool;
    struct xdp_rxq_info xdp_rxq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct netfront_queue {
    unsigned int id;
    char name[22];
    struct netfront_info *info;
    struct bpf_prog *xdp_prog;
    struct napi_struct napi;
    unsigned int tx_evtchn;
    unsigned int rx_evtchn;
    unsigned int tx_irq;
    unsigned int rx_irq;
    char tx_irq_name[25];
    char rx_irq_name[25];
    spinlock_t tx_lock;
    struct xen_netif_tx_front_ring tx;
    int tx_ring_ref;
    struct sk_buff * tx_skbs[256];
    short unsigned int tx_link[256];
    grant_ref_t gref_tx_head;
    grant_ref_t grant_tx_ref[256];
    struct page * grant_tx_page[256];
    unsigned int tx_skb_freelist;
    unsigned int tx_pend_queue;
    spinlock_t rx_lock;
    struct xen_netif_rx_front_ring rx;
    int rx_ring_ref;
    struct timer_list rx_refill_timer;
    struct sk_buff * rx_skbs[256];
    grant_ref_t gref_rx_head;
    grant_ref_t grant_rx_ref[256];
    unsigned int rx_rsp_unconsumed;
    spinlock_t rx_cons_lock;
    struct page_pool *page_pool;
    struct xdp_rxq_info xdp_rxq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct netfront_queue {
    unsigned int id;
    char name[22];
    struct netfront_info *info;
    struct bpf_prog *xdp_prog;
    struct napi_struct napi;
    unsigned int tx_evtchn;
    unsigned int rx_evtchn;
    unsigned int tx_irq;
    unsigned int rx_irq;
    char tx_irq_name[25];
    char rx_irq_name[25];
    spinlock_t tx_lock;
    struct xen_netif_tx_front_ring tx;
    int tx_ring_ref;
    struct sk_buff * tx_skbs[256];
    short unsigned int tx_link[256];
    grant_ref_t gref_tx_head;
    grant_ref_t grant_tx_ref[256];
    struct page * grant_tx_page[256];
    unsigned int tx_skb_freelist;
    unsigned int tx_pend_queue;
    spinlock_t rx_lock;
    struct xen_netif_rx_front_ring rx;
    int rx_ring_ref;
    struct timer_list rx_refill_timer;
    struct sk_buff * rx_skbs[256];
    grant_ref_t gref_rx_head;
    grant_ref_t grant_rx_ref[256];
    unsigned int rx_rsp_unconsumed;
    spinlock_t rx_cons_lock;
    struct page_pool *page_pool;
    struct xdp_rxq_info xdp_rxq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct netfront_queue {
    unsigned int id;
    char name[22];
    struct netfront_info *info;
    struct bpf_prog *xdp_prog;
    struct napi_struct napi;
    unsigned int tx_evtchn;
    unsigned int rx_evtchn;
    unsigned int tx_irq;
    unsigned int rx_irq;
    char tx_irq_name[25];
    char rx_irq_name[25];
    spinlock_t tx_lock;
    struct xen_netif_tx_front_ring tx;
    int tx_ring_ref;
    struct sk_buff * tx_skbs[256];
    short unsigned int tx_link[256];
    grant_ref_t gref_tx_head;
    grant_ref_t grant_tx_ref[256];
    struct page * grant_tx_page[256];
    unsigned int tx_skb_freelist;
    unsigned int tx_pend_queue;
    spinlock_t rx_lock;
    struct xen_netif_rx_front_ring rx;
    int rx_ring_ref;
    struct timer_list rx_refill_timer;
    struct sk_buff * rx_skbs[256];
    grant_ref_t gref_rx_head;
    grant_ref_t grant_rx_ref[256];
    unsigned int rx_rsp_unconsumed;
    spinlock_t rx_cons_lock;
    struct page_pool *page_pool;
    struct xdp_rxq_info xdp_rxq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct netfront_queue {
    unsigned int id;
    char name[22];
    struct netfront_info *info;
    struct bpf_prog *xdp_prog;
    struct napi_struct napi;
    unsigned int tx_evtchn;
    unsigned int rx_evtchn;
    unsigned int tx_irq;
    unsigned int rx_irq;
    char tx_irq_name[25];
    char rx_irq_name[25];
    spinlock_t tx_lock;
    struct xen_netif_tx_front_ring tx;
    int tx_ring_ref;
    struct sk_buff * tx_skbs[256];
    short unsigned int tx_link[256];
    grant_ref_t gref_tx_head;
    grant_ref_t grant_tx_ref[256];
    struct page * grant_tx_page[256];
    unsigned int tx_skb_freelist;
    unsigned int tx_pend_queue;
    spinlock_t rx_lock;
    struct xen_netif_rx_front_ring rx;
    int rx_ring_ref;
    struct timer_list rx_refill_timer;
    struct sk_buff * rx_skbs[256];
    grant_ref_t gref_rx_head;
    grant_ref_t grant_rx_ref[256];
    unsigned int rx_rsp_unconsumed;
    spinlock_t rx_cons_lock;
    struct page_pool *page_pool;
    struct xdp_rxq_info xdp_rxq;
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
struct netfront_queue {
    unsigned int id;
    char name[22];
    struct netfront_info *info;
    struct napi_struct napi;
    unsigned int tx_evtchn;
    unsigned int rx_evtchn;
    unsigned int tx_irq;
    unsigned int rx_irq;
    char tx_irq_name[25];
    char rx_irq_name[25];
    spinlock_t tx_lock;
    struct xen_netif_tx_front_ring tx;
    int tx_ring_ref;
    union skb_entry tx_skbs[256];
    grant_ref_t gref_tx_head;
    grant_ref_t grant_tx_ref[256];
    struct page * grant_tx_page[256];
    unsigned int tx_skb_freelist;
    spinlock_t rx_lock;
    struct xen_netif_rx_front_ring rx;
    int rx_ring_ref;
    struct timer_list rx_refill_timer;
    struct sk_buff * rx_skbs[256];
    grant_ref_t gref_rx_head;
    grant_ref_t grant_rx_ref[256];
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
struct netfront_queue {
    unsigned int id;
    char name[22];
    struct netfront_info *info;
    struct napi_struct napi;
    unsigned int tx_evtchn;
    unsigned int rx_evtchn;
    unsigned int tx_irq;
    unsigned int rx_irq;
    char tx_irq_name[25];
    char rx_irq_name[25];
    spinlock_t tx_lock;
    struct xen_netif_tx_front_ring tx;
    int tx_ring_ref;
    union skb_entry tx_skbs[256];
    grant_ref_t gref_tx_head;
    grant_ref_t grant_tx_ref[256];
    struct page * grant_tx_page[256];
    unsigned int tx_skb_freelist;
    spinlock_t rx_lock;
    struct xen_netif_rx_front_ring rx;
    int rx_ring_ref;
    struct timer_list rx_refill_timer;
    struct sk_buff * rx_skbs[256];
    grant_ref_t gref_rx_head;
    grant_ref_t grant_rx_ref[256];
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
struct netfront_queue {
    unsigned int id;
    char name[22];
    struct netfront_info *info;
    struct napi_struct napi;
    unsigned int tx_evtchn;
    unsigned int rx_evtchn;
    unsigned int tx_irq;
    unsigned int rx_irq;
    char tx_irq_name[25];
    char rx_irq_name[25];
    spinlock_t tx_lock;
    struct xen_netif_tx_front_ring tx;
    int tx_ring_ref;
    union skb_entry tx_skbs[256];
    grant_ref_t gref_tx_head;
    grant_ref_t grant_tx_ref[256];
    struct page * grant_tx_page[256];
    unsigned int tx_skb_freelist;
    spinlock_t rx_lock;
    struct xen_netif_rx_front_ring rx;
    int rx_ring_ref;
    struct timer_list rx_refill_timer;
    struct sk_buff * rx_skbs[256];
    grant_ref_t gref_rx_head;
    grant_ref_t grant_rx_ref[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct netfront_queue {
    unsigned int id;
    char name[22];
    struct netfront_info *info;
    struct napi_struct napi;
    unsigned int tx_evtchn;
    unsigned int rx_evtchn;
    unsigned int tx_irq;
    unsigned int rx_irq;
    char tx_irq_name[25];
    char rx_irq_name[25];
    spinlock_t tx_lock;
    struct xen_netif_tx_front_ring tx;
    int tx_ring_ref;
    union skb_entry tx_skbs[256];
    grant_ref_t gref_tx_head;
    grant_ref_t grant_tx_ref[256];
    struct page * grant_tx_page[256];
    unsigned int tx_skb_freelist;
    spinlock_t rx_lock;
    struct xen_netif_rx_front_ring rx;
    int rx_ring_ref;
    struct timer_list rx_refill_timer;
    struct sk_buff * rx_skbs[256];
    grant_ref_t gref_rx_head;
    grant_ref_t grant_rx_ref[256];
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
<code>struct bpf_prog *xdp_prog</code>
</li>
<li>
<b>Field added. </b>
<code>struct page_pool *page_pool</code>
</li>
<li>
<b>Field added. </b>
<code>struct xdp_rxq_info xdp_rxq</code>
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
<code>short unsigned int tx_link[256]</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int tx_pend_queue</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int rx_rsp_unconsumed</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t rx_cons_lock</code>
</li>
<li>
<b>Field type changed. </b>
<code>union skb_entry tx_skbs[256]</code> ➡️ <code>struct sk_buff * tx_skbs[256]</code>
</li>
</ul>
</details>
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
No changes between <code>generic</code> and <code>aws</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
