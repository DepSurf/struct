# Struct: <code>neighbour</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct neighbour {
    struct neighbour *next;
    struct neigh_table *tbl;
    struct neigh_parms *parms;
    long unsigned int confirmed;
    long unsigned int updated;
    rwlock_t lock;
    atomic_t refcnt;
    struct sk_buff_head arp_queue;
    unsigned int arp_queue_len_bytes;
    struct timer_list timer;
    long unsigned int used;
    atomic_t probes;
    __u8 flags;
    __u8 nud_state;
    __u8 type;
    __u8 dead;
    seqlock_t ha_lock;
    unsigned char ha[32];
    struct hh_cache hh;
    int (*output)(struct neighbour *, struct sk_buff *);
    const struct neigh_ops *ops;
    struct callback_head rcu;
    struct net_device *dev;
    u8 primary_key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct neighbour {
    struct neighbour *next;
    struct neigh_table *tbl;
    struct neigh_parms *parms;
    long unsigned int confirmed;
    long unsigned int updated;
    rwlock_t lock;
    atomic_t refcnt;
    struct sk_buff_head arp_queue;
    unsigned int arp_queue_len_bytes;
    struct timer_list timer;
    long unsigned int used;
    atomic_t probes;
    __u8 flags;
    __u8 nud_state;
    __u8 type;
    __u8 dead;
    seqlock_t ha_lock;
    unsigned char ha[32];
    struct hh_cache hh;
    int (*output)(struct neighbour *, struct sk_buff *);
    const struct neigh_ops *ops;
    struct callback_head rcu;
    struct net_device *dev;
    u8 primary_key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct neighbour {
    struct neighbour *next;
    struct neigh_table *tbl;
    struct neigh_parms *parms;
    long unsigned int confirmed;
    long unsigned int updated;
    rwlock_t lock;
    atomic_t refcnt;
    struct sk_buff_head arp_queue;
    unsigned int arp_queue_len_bytes;
    struct timer_list timer;
    long unsigned int used;
    atomic_t probes;
    __u8 flags;
    __u8 nud_state;
    __u8 type;
    __u8 dead;
    seqlock_t ha_lock;
    unsigned char ha[32];
    struct hh_cache hh;
    int (*output)(struct neighbour *, struct sk_buff *);
    const struct neigh_ops *ops;
    struct callback_head rcu;
    struct net_device *dev;
    u8 primary_key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct neighbour {
    struct neighbour *next;
    struct neigh_table *tbl;
    struct neigh_parms *parms;
    long unsigned int confirmed;
    long unsigned int updated;
    rwlock_t lock;
    refcount_t refcnt;
    struct sk_buff_head arp_queue;
    unsigned int arp_queue_len_bytes;
    struct timer_list timer;
    long unsigned int used;
    atomic_t probes;
    __u8 flags;
    __u8 nud_state;
    __u8 type;
    __u8 dead;
    seqlock_t ha_lock;
    unsigned char ha[32];
    struct hh_cache hh;
    int (*output)(struct neighbour *, struct sk_buff *);
    const struct neigh_ops *ops;
    struct callback_head rcu;
    struct net_device *dev;
    u8 primary_key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct neighbour {
    struct neighbour *next;
    struct neigh_table *tbl;
    struct neigh_parms *parms;
    long unsigned int confirmed;
    long unsigned int updated;
    rwlock_t lock;
    refcount_t refcnt;
    struct sk_buff_head arp_queue;
    unsigned int arp_queue_len_bytes;
    struct timer_list timer;
    long unsigned int used;
    atomic_t probes;
    __u8 flags;
    __u8 nud_state;
    __u8 type;
    __u8 dead;
    seqlock_t ha_lock;
    unsigned char ha[32];
    struct hh_cache hh;
    int (*output)(struct neighbour *, struct sk_buff *);
    const struct neigh_ops *ops;
    struct callback_head rcu;
    struct net_device *dev;
    u8 primary_key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct neighbour {
    struct neighbour *next;
    struct neigh_table *tbl;
    struct neigh_parms *parms;
    long unsigned int confirmed;
    long unsigned int updated;
    rwlock_t lock;
    refcount_t refcnt;
    struct sk_buff_head arp_queue;
    unsigned int arp_queue_len_bytes;
    struct timer_list timer;
    long unsigned int used;
    atomic_t probes;
    __u8 flags;
    __u8 nud_state;
    __u8 type;
    __u8 dead;
    seqlock_t ha_lock;
    unsigned char ha[32];
    struct hh_cache hh;
    int (*output)(struct neighbour *, struct sk_buff *);
    const struct neigh_ops *ops;
    struct callback_head rcu;
    struct net_device *dev;
    u8 primary_key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct neighbour {
    struct neighbour *next;
    struct neigh_table *tbl;
    struct neigh_parms *parms;
    long unsigned int confirmed;
    long unsigned int updated;
    rwlock_t lock;
    refcount_t refcnt;
    unsigned int arp_queue_len_bytes;
    struct sk_buff_head arp_queue;
    struct timer_list timer;
    long unsigned int used;
    atomic_t probes;
    __u8 flags;
    __u8 nud_state;
    __u8 type;
    __u8 dead;
    u8 protocol;
    seqlock_t ha_lock;
    unsigned char ha[32];
    struct hh_cache hh;
    int (*output)(struct neighbour *, struct sk_buff *);
    const struct neigh_ops *ops;
    struct list_head gc_list;
    struct callback_head rcu;
    struct net_device *dev;
    u8 primary_key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct neighbour {
    struct neighbour *next;
    struct neigh_table *tbl;
    struct neigh_parms *parms;
    long unsigned int confirmed;
    long unsigned int updated;
    rwlock_t lock;
    refcount_t refcnt;
    unsigned int arp_queue_len_bytes;
    struct sk_buff_head arp_queue;
    struct timer_list timer;
    long unsigned int used;
    atomic_t probes;
    __u8 flags;
    __u8 nud_state;
    __u8 type;
    __u8 dead;
    u8 protocol;
    seqlock_t ha_lock;
    unsigned char ha[32];
    struct hh_cache hh;
    int (*output)(struct neighbour *, struct sk_buff *);
    const struct neigh_ops *ops;
    struct list_head gc_list;
    struct callback_head rcu;
    struct net_device *dev;
    u8 primary_key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct neighbour {
    struct neighbour *next;
    struct neigh_table *tbl;
    struct neigh_parms *parms;
    long unsigned int confirmed;
    long unsigned int updated;
    rwlock_t lock;
    refcount_t refcnt;
    unsigned int arp_queue_len_bytes;
    struct sk_buff_head arp_queue;
    struct timer_list timer;
    long unsigned int used;
    atomic_t probes;
    __u8 flags;
    __u8 nud_state;
    __u8 type;
    __u8 dead;
    u8 protocol;
    seqlock_t ha_lock;
    unsigned char ha[32];
    struct hh_cache hh;
    int (*output)(struct neighbour *, struct sk_buff *);
    const struct neigh_ops *ops;
    struct list_head gc_list;
    struct callback_head rcu;
    struct net_device *dev;
    u8 primary_key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct neighbour {
    struct neighbour *next;
    struct neigh_table *tbl;
    struct neigh_parms *parms;
    long unsigned int confirmed;
    long unsigned int updated;
    rwlock_t lock;
    refcount_t refcnt;
    unsigned int arp_queue_len_bytes;
    struct sk_buff_head arp_queue;
    struct timer_list timer;
    long unsigned int used;
    atomic_t probes;
    __u8 flags;
    __u8 nud_state;
    __u8 type;
    __u8 dead;
    u8 protocol;
    seqlock_t ha_lock;
    unsigned char ha[32];
    struct hh_cache hh;
    int (*output)(struct neighbour *, struct sk_buff *);
    const struct neigh_ops *ops;
    struct list_head gc_list;
    struct callback_head rcu;
    struct net_device *dev;
    u8 primary_key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct neighbour {
    struct neighbour *next;
    struct neigh_table *tbl;
    struct neigh_parms *parms;
    long unsigned int confirmed;
    long unsigned int updated;
    rwlock_t lock;
    refcount_t refcnt;
    unsigned int arp_queue_len_bytes;
    struct sk_buff_head arp_queue;
    struct timer_list timer;
    long unsigned int used;
    atomic_t probes;
    __u8 flags;
    __u8 nud_state;
    __u8 type;
    __u8 dead;
    u8 protocol;
    seqlock_t ha_lock;
    unsigned char ha[32];
    struct hh_cache hh;
    int (*output)(struct neighbour *, struct sk_buff *);
    const struct neigh_ops *ops;
    struct list_head gc_list;
    struct callback_head rcu;
    struct net_device *dev;
    u8 primary_key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct neighbour {
    struct neighbour *next;
    struct neigh_table *tbl;
    struct neigh_parms *parms;
    long unsigned int confirmed;
    long unsigned int updated;
    rwlock_t lock;
    refcount_t refcnt;
    unsigned int arp_queue_len_bytes;
    struct sk_buff_head arp_queue;
    struct timer_list timer;
    long unsigned int used;
    atomic_t probes;
    __u8 flags;
    __u8 nud_state;
    __u8 type;
    __u8 dead;
    u8 protocol;
    seqlock_t ha_lock;
    unsigned char ha[32];
    struct hh_cache hh;
    int (*output)(struct neighbour *, struct sk_buff *);
    const struct neigh_ops *ops;
    struct list_head gc_list;
    struct callback_head rcu;
    struct net_device *dev;
    u8 primary_key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct neighbour {
    struct neighbour *next;
    struct neigh_table *tbl;
    struct neigh_parms *parms;
    long unsigned int confirmed;
    long unsigned int updated;
    rwlock_t lock;
    refcount_t refcnt;
    unsigned int arp_queue_len_bytes;
    struct sk_buff_head arp_queue;
    struct timer_list timer;
    long unsigned int used;
    atomic_t probes;
    __u8 flags;
    __u8 nud_state;
    __u8 type;
    __u8 dead;
    u8 protocol;
    seqlock_t ha_lock;
    unsigned char ha[32];
    struct hh_cache hh;
    int (*output)(struct neighbour *, struct sk_buff *);
    const struct neigh_ops *ops;
    struct list_head gc_list;
    struct callback_head rcu;
    struct net_device *dev;
    u8 primary_key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct neighbour {
    struct neighbour *next;
    struct neigh_table *tbl;
    struct neigh_parms *parms;
    long unsigned int confirmed;
    long unsigned int updated;
    rwlock_t lock;
    refcount_t refcnt;
    unsigned int arp_queue_len_bytes;
    struct sk_buff_head arp_queue;
    struct timer_list timer;
    long unsigned int used;
    atomic_t probes;
    u8 nud_state;
    u8 type;
    u8 dead;
    u8 protocol;
    u32 flags;
    seqlock_t ha_lock;
    unsigned char ha[32];
    struct hh_cache hh;
    int (*output)(struct neighbour *, struct sk_buff *);
    const struct neigh_ops *ops;
    struct list_head gc_list;
    struct list_head managed_list;
    struct callback_head rcu;
    struct net_device *dev;
    netdevice_tracker dev_tracker;
    u8 primary_key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct neighbour {
    struct neighbour *next;
    struct neigh_table *tbl;
    struct neigh_parms *parms;
    long unsigned int confirmed;
    long unsigned int updated;
    rwlock_t lock;
    refcount_t refcnt;
    unsigned int arp_queue_len_bytes;
    struct sk_buff_head arp_queue;
    struct timer_list timer;
    long unsigned int used;
    atomic_t probes;
    u8 nud_state;
    u8 type;
    u8 dead;
    u8 protocol;
    u32 flags;
    seqlock_t ha_lock;
    unsigned char ha[32];
    struct hh_cache hh;
    int (*output)(struct neighbour *, struct sk_buff *);
    const struct neigh_ops *ops;
    struct list_head gc_list;
    struct list_head managed_list;
    struct callback_head rcu;
    struct net_device *dev;
    netdevice_tracker dev_tracker;
    u8 primary_key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct neighbour {
    struct neighbour *next;
    struct neigh_table *tbl;
    struct neigh_parms *parms;
    long unsigned int confirmed;
    long unsigned int updated;
    rwlock_t lock;
    refcount_t refcnt;
    unsigned int arp_queue_len_bytes;
    struct sk_buff_head arp_queue;
    struct timer_list timer;
    long unsigned int used;
    atomic_t probes;
    u8 nud_state;
    u8 type;
    u8 dead;
    u8 protocol;
    u32 flags;
    seqlock_t ha_lock;
    unsigned char ha[32];
    struct hh_cache hh;
    int (*output)(struct neighbour *, struct sk_buff *);
    const struct neigh_ops *ops;
    struct list_head gc_list;
    struct list_head managed_list;
    struct callback_head rcu;
    struct net_device *dev;
    netdevice_tracker dev_tracker;
    u8 primary_key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct neighbour {
    struct neighbour *next;
    struct neigh_table *tbl;
    struct neigh_parms *parms;
    long unsigned int confirmed;
    long unsigned int updated;
    rwlock_t lock;
    refcount_t refcnt;
    unsigned int arp_queue_len_bytes;
    struct sk_buff_head arp_queue;
    struct timer_list timer;
    long unsigned int used;
    atomic_t probes;
    u8 nud_state;
    u8 type;
    u8 dead;
    u8 protocol;
    u32 flags;
    seqlock_t ha_lock;
    unsigned char ha[32];
    struct hh_cache hh;
    int (*output)(struct neighbour *, struct sk_buff *);
    const struct neigh_ops *ops;
    struct list_head gc_list;
    struct list_head managed_list;
    struct callback_head rcu;
    struct net_device *dev;
    netdevice_tracker dev_tracker;
    u8 primary_key[0];
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
struct neighbour {
    struct neighbour *next;
    struct neigh_table *tbl;
    struct neigh_parms *parms;
    long unsigned int confirmed;
    long unsigned int updated;
    rwlock_t lock;
    refcount_t refcnt;
    unsigned int arp_queue_len_bytes;
    struct sk_buff_head arp_queue;
    struct timer_list timer;
    long unsigned int used;
    atomic_t probes;
    __u8 flags;
    __u8 nud_state;
    __u8 type;
    __u8 dead;
    u8 protocol;
    seqlock_t ha_lock;
    unsigned char ha[32];
    struct hh_cache hh;
    int (*output)(struct neighbour *, struct sk_buff *);
    const struct neigh_ops *ops;
    struct list_head gc_list;
    struct callback_head rcu;
    struct net_device *dev;
    u8 primary_key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct neighbour {
    struct neighbour *next;
    struct neigh_table *tbl;
    struct neigh_parms *parms;
    long unsigned int confirmed;
    long unsigned int updated;
    rwlock_t lock;
    refcount_t refcnt;
    unsigned int arp_queue_len_bytes;
    struct sk_buff_head arp_queue;
    struct timer_list timer;
    long unsigned int used;
    atomic_t probes;
    __u8 flags;
    __u8 nud_state;
    __u8 type;
    __u8 dead;
    u8 protocol;
    seqlock_t ha_lock;
    unsigned char ha[32];
    struct hh_cache hh;
    int (*output)(struct neighbour *, struct sk_buff *);
    const struct neigh_ops *ops;
    struct list_head gc_list;
    struct callback_head rcu;
    struct net_device *dev;
    u8 primary_key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct neighbour {
    struct neighbour *next;
    struct neigh_table *tbl;
    struct neigh_parms *parms;
    long unsigned int confirmed;
    long unsigned int updated;
    rwlock_t lock;
    refcount_t refcnt;
    unsigned int arp_queue_len_bytes;
    struct sk_buff_head arp_queue;
    struct timer_list timer;
    long unsigned int used;
    atomic_t probes;
    __u8 flags;
    __u8 nud_state;
    __u8 type;
    __u8 dead;
    u8 protocol;
    seqlock_t ha_lock;
    unsigned char ha[32];
    struct hh_cache hh;
    int (*output)(struct neighbour *, struct sk_buff *);
    const struct neigh_ops *ops;
    struct list_head gc_list;
    struct callback_head rcu;
    struct net_device *dev;
    u8 primary_key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct neighbour {
    struct neighbour *next;
    struct neigh_table *tbl;
    struct neigh_parms *parms;
    long unsigned int confirmed;
    long unsigned int updated;
    rwlock_t lock;
    refcount_t refcnt;
    unsigned int arp_queue_len_bytes;
    struct sk_buff_head arp_queue;
    struct timer_list timer;
    long unsigned int used;
    atomic_t probes;
    __u8 flags;
    __u8 nud_state;
    __u8 type;
    __u8 dead;
    u8 protocol;
    seqlock_t ha_lock;
    unsigned char ha[32];
    struct hh_cache hh;
    int (*output)(struct neighbour *, struct sk_buff *);
    const struct neigh_ops *ops;
    struct list_head gc_list;
    struct callback_head rcu;
    struct net_device *dev;
    u8 primary_key[0];
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
struct neighbour {
    struct neighbour *next;
    struct neigh_table *tbl;
    struct neigh_parms *parms;
    long unsigned int confirmed;
    long unsigned int updated;
    rwlock_t lock;
    refcount_t refcnt;
    unsigned int arp_queue_len_bytes;
    struct sk_buff_head arp_queue;
    struct timer_list timer;
    long unsigned int used;
    atomic_t probes;
    __u8 flags;
    __u8 nud_state;
    __u8 type;
    __u8 dead;
    u8 protocol;
    seqlock_t ha_lock;
    unsigned char ha[32];
    struct hh_cache hh;
    int (*output)(struct neighbour *, struct sk_buff *);
    const struct neigh_ops *ops;
    struct list_head gc_list;
    struct callback_head rcu;
    struct net_device *dev;
    u8 primary_key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct neighbour {
    struct neighbour *next;
    struct neigh_table *tbl;
    struct neigh_parms *parms;
    long unsigned int confirmed;
    long unsigned int updated;
    rwlock_t lock;
    refcount_t refcnt;
    unsigned int arp_queue_len_bytes;
    struct sk_buff_head arp_queue;
    struct timer_list timer;
    long unsigned int used;
    atomic_t probes;
    __u8 flags;
    __u8 nud_state;
    __u8 type;
    __u8 dead;
    u8 protocol;
    seqlock_t ha_lock;
    unsigned char ha[32];
    struct hh_cache hh;
    int (*output)(struct neighbour *, struct sk_buff *);
    const struct neigh_ops *ops;
    struct list_head gc_list;
    struct callback_head rcu;
    struct net_device *dev;
    u8 primary_key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct neighbour {
    struct neighbour *next;
    struct neigh_table *tbl;
    struct neigh_parms *parms;
    long unsigned int confirmed;
    long unsigned int updated;
    rwlock_t lock;
    refcount_t refcnt;
    unsigned int arp_queue_len_bytes;
    struct sk_buff_head arp_queue;
    struct timer_list timer;
    long unsigned int used;
    atomic_t probes;
    __u8 flags;
    __u8 nud_state;
    __u8 type;
    __u8 dead;
    u8 protocol;
    seqlock_t ha_lock;
    unsigned char ha[32];
    struct hh_cache hh;
    int (*output)(struct neighbour *, struct sk_buff *);
    const struct neigh_ops *ops;
    struct list_head gc_list;
    struct callback_head rcu;
    struct net_device *dev;
    u8 primary_key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct neighbour {
    struct neighbour *next;
    struct neigh_table *tbl;
    struct neigh_parms *parms;
    long unsigned int confirmed;
    long unsigned int updated;
    rwlock_t lock;
    refcount_t refcnt;
    unsigned int arp_queue_len_bytes;
    struct sk_buff_head arp_queue;
    struct timer_list timer;
    long unsigned int used;
    atomic_t probes;
    __u8 flags;
    __u8 nud_state;
    __u8 type;
    __u8 dead;
    u8 protocol;
    seqlock_t ha_lock;
    unsigned char ha[32];
    struct hh_cache hh;
    int (*output)(struct neighbour *, struct sk_buff *);
    const struct neigh_ops *ops;
    struct list_head gc_list;
    struct callback_head rcu;
    struct net_device *dev;
    u8 primary_key[0];
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
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>atomic_t refcnt</code> ➡️ <code>refcount_t refcnt</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 protocol</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head gc_list</code>
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
No changes between <code>5.8</code> and <code>5.11</code> ✅
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
<code>struct list_head managed_list</code>
</li>
<li>
<b>Field added. </b>
<code>netdevice_tracker dev_tracker</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u8 flags</code> ➡️ <code>u32 flags</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u8 nud_state</code> ➡️ <code>u8 nud_state</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u8 type</code> ➡️ <code>u8 type</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u8 dead</code> ➡️ <code>u8 dead</code>
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
