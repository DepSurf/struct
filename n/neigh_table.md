# Struct: <code>neigh_table</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct neigh_table {
    int family;
    int entry_size;
    int key_len;
    __be16 protocol;
    __u32 (*hash)(const void *, const struct net_device *, __u32 *);
    bool (*key_eq)(const struct neighbour *, const void *);
    int (*constructor)(struct neighbour *);
    int (*pconstructor)(struct pneigh_entry *);
    void (*pdestructor)(struct pneigh_entry *);
    void (*proxy_redo)(struct sk_buff *);
    char *id;
    struct neigh_parms parms;
    struct list_head parms_list;
    int gc_interval;
    int gc_thresh1;
    int gc_thresh2;
    int gc_thresh3;
    long unsigned int last_flush;
    struct delayed_work gc_work;
    struct timer_list proxy_timer;
    struct sk_buff_head proxy_queue;
    atomic_t entries;
    rwlock_t lock;
    long unsigned int last_rand;
    struct neigh_statistics *stats;
    struct neigh_hash_table *nht;
    struct pneigh_entry **phash_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct neigh_table {
    int family;
    int entry_size;
    int key_len;
    __be16 protocol;
    __u32 (*hash)(const void *, const struct net_device *, __u32 *);
    bool (*key_eq)(const struct neighbour *, const void *);
    int (*constructor)(struct neighbour *);
    int (*pconstructor)(struct pneigh_entry *);
    void (*pdestructor)(struct pneigh_entry *);
    void (*proxy_redo)(struct sk_buff *);
    char *id;
    struct neigh_parms parms;
    struct list_head parms_list;
    int gc_interval;
    int gc_thresh1;
    int gc_thresh2;
    int gc_thresh3;
    long unsigned int last_flush;
    struct delayed_work gc_work;
    struct timer_list proxy_timer;
    struct sk_buff_head proxy_queue;
    atomic_t entries;
    rwlock_t lock;
    long unsigned int last_rand;
    struct neigh_statistics *stats;
    struct neigh_hash_table *nht;
    struct pneigh_entry **phash_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct neigh_table {
    int family;
    int entry_size;
    int key_len;
    __be16 protocol;
    __u32 (*hash)(const void *, const struct net_device *, __u32 *);
    bool (*key_eq)(const struct neighbour *, const void *);
    int (*constructor)(struct neighbour *);
    int (*pconstructor)(struct pneigh_entry *);
    void (*pdestructor)(struct pneigh_entry *);
    void (*proxy_redo)(struct sk_buff *);
    char *id;
    struct neigh_parms parms;
    struct list_head parms_list;
    int gc_interval;
    int gc_thresh1;
    int gc_thresh2;
    int gc_thresh3;
    long unsigned int last_flush;
    struct delayed_work gc_work;
    struct timer_list proxy_timer;
    struct sk_buff_head proxy_queue;
    atomic_t entries;
    rwlock_t lock;
    long unsigned int last_rand;
    struct neigh_statistics *stats;
    struct neigh_hash_table *nht;
    struct pneigh_entry **phash_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct neigh_table {
    int family;
    int entry_size;
    int key_len;
    __be16 protocol;
    __u32 (*hash)(const void *, const struct net_device *, __u32 *);
    bool (*key_eq)(const struct neighbour *, const void *);
    int (*constructor)(struct neighbour *);
    int (*pconstructor)(struct pneigh_entry *);
    void (*pdestructor)(struct pneigh_entry *);
    void (*proxy_redo)(struct sk_buff *);
    char *id;
    struct neigh_parms parms;
    struct list_head parms_list;
    int gc_interval;
    int gc_thresh1;
    int gc_thresh2;
    int gc_thresh3;
    long unsigned int last_flush;
    struct delayed_work gc_work;
    struct timer_list proxy_timer;
    struct sk_buff_head proxy_queue;
    atomic_t entries;
    rwlock_t lock;
    long unsigned int last_rand;
    struct neigh_statistics *stats;
    struct neigh_hash_table *nht;
    struct pneigh_entry **phash_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct neigh_table {
    int family;
    unsigned int entry_size;
    unsigned int key_len;
    __be16 protocol;
    __u32 (*hash)(const void *, const struct net_device *, __u32 *);
    bool (*key_eq)(const struct neighbour *, const void *);
    int (*constructor)(struct neighbour *);
    int (*pconstructor)(struct pneigh_entry *);
    void (*pdestructor)(struct pneigh_entry *);
    void (*proxy_redo)(struct sk_buff *);
    char *id;
    struct neigh_parms parms;
    struct list_head parms_list;
    int gc_interval;
    int gc_thresh1;
    int gc_thresh2;
    int gc_thresh3;
    long unsigned int last_flush;
    struct delayed_work gc_work;
    struct timer_list proxy_timer;
    struct sk_buff_head proxy_queue;
    atomic_t entries;
    rwlock_t lock;
    long unsigned int last_rand;
    struct neigh_statistics *stats;
    struct neigh_hash_table *nht;
    struct pneigh_entry **phash_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct neigh_table {
    int family;
    unsigned int entry_size;
    unsigned int key_len;
    __be16 protocol;
    __u32 (*hash)(const void *, const struct net_device *, __u32 *);
    bool (*key_eq)(const struct neighbour *, const void *);
    int (*constructor)(struct neighbour *);
    int (*pconstructor)(struct pneigh_entry *);
    void (*pdestructor)(struct pneigh_entry *);
    void (*proxy_redo)(struct sk_buff *);
    char *id;
    struct neigh_parms parms;
    struct list_head parms_list;
    int gc_interval;
    int gc_thresh1;
    int gc_thresh2;
    int gc_thresh3;
    long unsigned int last_flush;
    struct delayed_work gc_work;
    struct timer_list proxy_timer;
    struct sk_buff_head proxy_queue;
    atomic_t entries;
    rwlock_t lock;
    long unsigned int last_rand;
    struct neigh_statistics *stats;
    struct neigh_hash_table *nht;
    struct pneigh_entry **phash_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct neigh_table {
    int family;
    unsigned int entry_size;
    unsigned int key_len;
    __be16 protocol;
    __u32 (*hash)(const void *, const struct net_device *, __u32 *);
    bool (*key_eq)(const struct neighbour *, const void *);
    int (*constructor)(struct neighbour *);
    int (*pconstructor)(struct pneigh_entry *);
    void (*pdestructor)(struct pneigh_entry *);
    void (*proxy_redo)(struct sk_buff *);
    char *id;
    struct neigh_parms parms;
    struct list_head parms_list;
    int gc_interval;
    int gc_thresh1;
    int gc_thresh2;
    int gc_thresh3;
    long unsigned int last_flush;
    struct delayed_work gc_work;
    struct timer_list proxy_timer;
    struct sk_buff_head proxy_queue;
    atomic_t entries;
    atomic_t gc_entries;
    struct list_head gc_list;
    rwlock_t lock;
    long unsigned int last_rand;
    struct neigh_statistics *stats;
    struct neigh_hash_table *nht;
    struct pneigh_entry **phash_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct neigh_table {
    int family;
    unsigned int entry_size;
    unsigned int key_len;
    __be16 protocol;
    __u32 (*hash)(const void *, const struct net_device *, __u32 *);
    bool (*key_eq)(const struct neighbour *, const void *);
    int (*constructor)(struct neighbour *);
    int (*pconstructor)(struct pneigh_entry *);
    void (*pdestructor)(struct pneigh_entry *);
    void (*proxy_redo)(struct sk_buff *);
    bool (*allow_add)(const struct net_device *, struct netlink_ext_ack *);
    char *id;
    struct neigh_parms parms;
    struct list_head parms_list;
    int gc_interval;
    int gc_thresh1;
    int gc_thresh2;
    int gc_thresh3;
    long unsigned int last_flush;
    struct delayed_work gc_work;
    struct timer_list proxy_timer;
    struct sk_buff_head proxy_queue;
    atomic_t entries;
    atomic_t gc_entries;
    struct list_head gc_list;
    rwlock_t lock;
    long unsigned int last_rand;
    struct neigh_statistics *stats;
    struct neigh_hash_table *nht;
    struct pneigh_entry **phash_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct neigh_table {
    int family;
    unsigned int entry_size;
    unsigned int key_len;
    __be16 protocol;
    __u32 (*hash)(const void *, const struct net_device *, __u32 *);
    bool (*key_eq)(const struct neighbour *, const void *);
    int (*constructor)(struct neighbour *);
    int (*pconstructor)(struct pneigh_entry *);
    void (*pdestructor)(struct pneigh_entry *);
    void (*proxy_redo)(struct sk_buff *);
    bool (*allow_add)(const struct net_device *, struct netlink_ext_ack *);
    char *id;
    struct neigh_parms parms;
    struct list_head parms_list;
    int gc_interval;
    int gc_thresh1;
    int gc_thresh2;
    int gc_thresh3;
    long unsigned int last_flush;
    struct delayed_work gc_work;
    struct timer_list proxy_timer;
    struct sk_buff_head proxy_queue;
    atomic_t entries;
    atomic_t gc_entries;
    struct list_head gc_list;
    rwlock_t lock;
    long unsigned int last_rand;
    struct neigh_statistics *stats;
    struct neigh_hash_table *nht;
    struct pneigh_entry **phash_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct neigh_table {
    int family;
    unsigned int entry_size;
    unsigned int key_len;
    __be16 protocol;
    __u32 (*hash)(const void *, const struct net_device *, __u32 *);
    bool (*key_eq)(const struct neighbour *, const void *);
    int (*constructor)(struct neighbour *);
    int (*pconstructor)(struct pneigh_entry *);
    void (*pdestructor)(struct pneigh_entry *);
    void (*proxy_redo)(struct sk_buff *);
    bool (*allow_add)(const struct net_device *, struct netlink_ext_ack *);
    char *id;
    struct neigh_parms parms;
    struct list_head parms_list;
    int gc_interval;
    int gc_thresh1;
    int gc_thresh2;
    int gc_thresh3;
    long unsigned int last_flush;
    struct delayed_work gc_work;
    struct timer_list proxy_timer;
    struct sk_buff_head proxy_queue;
    atomic_t entries;
    atomic_t gc_entries;
    struct list_head gc_list;
    rwlock_t lock;
    long unsigned int last_rand;
    struct neigh_statistics *stats;
    struct neigh_hash_table *nht;
    struct pneigh_entry **phash_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct neigh_table {
    int family;
    unsigned int entry_size;
    unsigned int key_len;
    __be16 protocol;
    __u32 (*hash)(const void *, const struct net_device *, __u32 *);
    bool (*key_eq)(const struct neighbour *, const void *);
    int (*constructor)(struct neighbour *);
    int (*pconstructor)(struct pneigh_entry *);
    void (*pdestructor)(struct pneigh_entry *);
    void (*proxy_redo)(struct sk_buff *);
    int (*is_multicast)(const void *);
    bool (*allow_add)(const struct net_device *, struct netlink_ext_ack *);
    char *id;
    struct neigh_parms parms;
    struct list_head parms_list;
    int gc_interval;
    int gc_thresh1;
    int gc_thresh2;
    int gc_thresh3;
    long unsigned int last_flush;
    struct delayed_work gc_work;
    struct timer_list proxy_timer;
    struct sk_buff_head proxy_queue;
    atomic_t entries;
    atomic_t gc_entries;
    struct list_head gc_list;
    rwlock_t lock;
    long unsigned int last_rand;
    struct neigh_statistics *stats;
    struct neigh_hash_table *nht;
    struct pneigh_entry **phash_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct neigh_table {
    int family;
    unsigned int entry_size;
    unsigned int key_len;
    __be16 protocol;
    __u32 (*hash)(const void *, const struct net_device *, __u32 *);
    bool (*key_eq)(const struct neighbour *, const void *);
    int (*constructor)(struct neighbour *);
    int (*pconstructor)(struct pneigh_entry *);
    void (*pdestructor)(struct pneigh_entry *);
    void (*proxy_redo)(struct sk_buff *);
    int (*is_multicast)(const void *);
    bool (*allow_add)(const struct net_device *, struct netlink_ext_ack *);
    char *id;
    struct neigh_parms parms;
    struct list_head parms_list;
    int gc_interval;
    int gc_thresh1;
    int gc_thresh2;
    int gc_thresh3;
    long unsigned int last_flush;
    struct delayed_work gc_work;
    struct timer_list proxy_timer;
    struct sk_buff_head proxy_queue;
    atomic_t entries;
    atomic_t gc_entries;
    struct list_head gc_list;
    rwlock_t lock;
    long unsigned int last_rand;
    struct neigh_statistics *stats;
    struct neigh_hash_table *nht;
    struct pneigh_entry **phash_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct neigh_table {
    int family;
    unsigned int entry_size;
    unsigned int key_len;
    __be16 protocol;
    __u32 (*hash)(const void *, const struct net_device *, __u32 *);
    bool (*key_eq)(const struct neighbour *, const void *);
    int (*constructor)(struct neighbour *);
    int (*pconstructor)(struct pneigh_entry *);
    void (*pdestructor)(struct pneigh_entry *);
    void (*proxy_redo)(struct sk_buff *);
    int (*is_multicast)(const void *);
    bool (*allow_add)(const struct net_device *, struct netlink_ext_ack *);
    char *id;
    struct neigh_parms parms;
    struct list_head parms_list;
    int gc_interval;
    int gc_thresh1;
    int gc_thresh2;
    int gc_thresh3;
    long unsigned int last_flush;
    struct delayed_work gc_work;
    struct timer_list proxy_timer;
    struct sk_buff_head proxy_queue;
    atomic_t entries;
    atomic_t gc_entries;
    struct list_head gc_list;
    rwlock_t lock;
    long unsigned int last_rand;
    struct neigh_statistics *stats;
    struct neigh_hash_table *nht;
    struct pneigh_entry **phash_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct neigh_table {
    int family;
    unsigned int entry_size;
    unsigned int key_len;
    __be16 protocol;
    __u32 (*hash)(const void *, const struct net_device *, __u32 *);
    bool (*key_eq)(const struct neighbour *, const void *);
    int (*constructor)(struct neighbour *);
    int (*pconstructor)(struct pneigh_entry *);
    void (*pdestructor)(struct pneigh_entry *);
    void (*proxy_redo)(struct sk_buff *);
    int (*is_multicast)(const void *);
    bool (*allow_add)(const struct net_device *, struct netlink_ext_ack *);
    char *id;
    struct neigh_parms parms;
    struct list_head parms_list;
    int gc_interval;
    int gc_thresh1;
    int gc_thresh2;
    int gc_thresh3;
    long unsigned int last_flush;
    struct delayed_work gc_work;
    struct delayed_work managed_work;
    struct timer_list proxy_timer;
    struct sk_buff_head proxy_queue;
    atomic_t entries;
    atomic_t gc_entries;
    struct list_head gc_list;
    struct list_head managed_list;
    rwlock_t lock;
    long unsigned int last_rand;
    struct neigh_statistics *stats;
    struct neigh_hash_table *nht;
    struct pneigh_entry **phash_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct neigh_table {
    int family;
    unsigned int entry_size;
    unsigned int key_len;
    __be16 protocol;
    __u32 (*hash)(const void *, const struct net_device *, __u32 *);
    bool (*key_eq)(const struct neighbour *, const void *);
    int (*constructor)(struct neighbour *);
    int (*pconstructor)(struct pneigh_entry *);
    void (*pdestructor)(struct pneigh_entry *);
    void (*proxy_redo)(struct sk_buff *);
    int (*is_multicast)(const void *);
    bool (*allow_add)(const struct net_device *, struct netlink_ext_ack *);
    char *id;
    struct neigh_parms parms;
    struct list_head parms_list;
    int gc_interval;
    int gc_thresh1;
    int gc_thresh2;
    int gc_thresh3;
    long unsigned int last_flush;
    struct delayed_work gc_work;
    struct delayed_work managed_work;
    struct timer_list proxy_timer;
    struct sk_buff_head proxy_queue;
    atomic_t entries;
    atomic_t gc_entries;
    struct list_head gc_list;
    struct list_head managed_list;
    rwlock_t lock;
    long unsigned int last_rand;
    struct neigh_statistics *stats;
    struct neigh_hash_table *nht;
    struct pneigh_entry **phash_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct neigh_table {
    int family;
    unsigned int entry_size;
    unsigned int key_len;
    __be16 protocol;
    __u32 (*hash)(const void *, const struct net_device *, __u32 *);
    bool (*key_eq)(const struct neighbour *, const void *);
    int (*constructor)(struct neighbour *);
    int (*pconstructor)(struct pneigh_entry *);
    void (*pdestructor)(struct pneigh_entry *);
    void (*proxy_redo)(struct sk_buff *);
    int (*is_multicast)(const void *);
    bool (*allow_add)(const struct net_device *, struct netlink_ext_ack *);
    char *id;
    struct neigh_parms parms;
    struct list_head parms_list;
    int gc_interval;
    int gc_thresh1;
    int gc_thresh2;
    int gc_thresh3;
    long unsigned int last_flush;
    struct delayed_work gc_work;
    struct delayed_work managed_work;
    struct timer_list proxy_timer;
    struct sk_buff_head proxy_queue;
    atomic_t entries;
    atomic_t gc_entries;
    struct list_head gc_list;
    struct list_head managed_list;
    rwlock_t lock;
    long unsigned int last_rand;
    struct neigh_statistics *stats;
    struct neigh_hash_table *nht;
    struct pneigh_entry **phash_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct neigh_table {
    int family;
    unsigned int entry_size;
    unsigned int key_len;
    __be16 protocol;
    __u32 (*hash)(const void *, const struct net_device *, __u32 *);
    bool (*key_eq)(const struct neighbour *, const void *);
    int (*constructor)(struct neighbour *);
    int (*pconstructor)(struct pneigh_entry *);
    void (*pdestructor)(struct pneigh_entry *);
    void (*proxy_redo)(struct sk_buff *);
    int (*is_multicast)(const void *);
    bool (*allow_add)(const struct net_device *, struct netlink_ext_ack *);
    char *id;
    struct neigh_parms parms;
    struct list_head parms_list;
    int gc_interval;
    int gc_thresh1;
    int gc_thresh2;
    int gc_thresh3;
    long unsigned int last_flush;
    struct delayed_work gc_work;
    struct delayed_work managed_work;
    struct timer_list proxy_timer;
    struct sk_buff_head proxy_queue;
    atomic_t entries;
    atomic_t gc_entries;
    struct list_head gc_list;
    struct list_head managed_list;
    rwlock_t lock;
    long unsigned int last_rand;
    struct neigh_statistics *stats;
    struct neigh_hash_table *nht;
    struct pneigh_entry **phash_buckets;
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
struct neigh_table {
    int family;
    unsigned int entry_size;
    unsigned int key_len;
    __be16 protocol;
    __u32 (*hash)(const void *, const struct net_device *, __u32 *);
    bool (*key_eq)(const struct neighbour *, const void *);
    int (*constructor)(struct neighbour *);
    int (*pconstructor)(struct pneigh_entry *);
    void (*pdestructor)(struct pneigh_entry *);
    void (*proxy_redo)(struct sk_buff *);
    bool (*allow_add)(const struct net_device *, struct netlink_ext_ack *);
    char *id;
    struct neigh_parms parms;
    struct list_head parms_list;
    int gc_interval;
    int gc_thresh1;
    int gc_thresh2;
    int gc_thresh3;
    long unsigned int last_flush;
    struct delayed_work gc_work;
    struct timer_list proxy_timer;
    struct sk_buff_head proxy_queue;
    atomic_t entries;
    atomic_t gc_entries;
    struct list_head gc_list;
    rwlock_t lock;
    long unsigned int last_rand;
    struct neigh_statistics *stats;
    struct neigh_hash_table *nht;
    struct pneigh_entry **phash_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct neigh_table {
    int family;
    unsigned int entry_size;
    unsigned int key_len;
    __be16 protocol;
    __u32 (*hash)(const void *, const struct net_device *, __u32 *);
    bool (*key_eq)(const struct neighbour *, const void *);
    int (*constructor)(struct neighbour *);
    int (*pconstructor)(struct pneigh_entry *);
    void (*pdestructor)(struct pneigh_entry *);
    void (*proxy_redo)(struct sk_buff *);
    bool (*allow_add)(const struct net_device *, struct netlink_ext_ack *);
    char *id;
    struct neigh_parms parms;
    struct list_head parms_list;
    int gc_interval;
    int gc_thresh1;
    int gc_thresh2;
    int gc_thresh3;
    long unsigned int last_flush;
    struct delayed_work gc_work;
    struct timer_list proxy_timer;
    struct sk_buff_head proxy_queue;
    atomic_t entries;
    atomic_t gc_entries;
    struct list_head gc_list;
    rwlock_t lock;
    long unsigned int last_rand;
    struct neigh_statistics *stats;
    struct neigh_hash_table *nht;
    struct pneigh_entry **phash_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct neigh_table {
    int family;
    unsigned int entry_size;
    unsigned int key_len;
    __be16 protocol;
    __u32 (*hash)(const void *, const struct net_device *, __u32 *);
    bool (*key_eq)(const struct neighbour *, const void *);
    int (*constructor)(struct neighbour *);
    int (*pconstructor)(struct pneigh_entry *);
    void (*pdestructor)(struct pneigh_entry *);
    void (*proxy_redo)(struct sk_buff *);
    bool (*allow_add)(const struct net_device *, struct netlink_ext_ack *);
    char *id;
    struct neigh_parms parms;
    struct list_head parms_list;
    int gc_interval;
    int gc_thresh1;
    int gc_thresh2;
    int gc_thresh3;
    long unsigned int last_flush;
    struct delayed_work gc_work;
    struct timer_list proxy_timer;
    struct sk_buff_head proxy_queue;
    atomic_t entries;
    atomic_t gc_entries;
    struct list_head gc_list;
    rwlock_t lock;
    long unsigned int last_rand;
    struct neigh_statistics *stats;
    struct neigh_hash_table *nht;
    struct pneigh_entry **phash_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct neigh_table {
    int family;
    unsigned int entry_size;
    unsigned int key_len;
    __be16 protocol;
    __u32 (*hash)(const void *, const struct net_device *, __u32 *);
    bool (*key_eq)(const struct neighbour *, const void *);
    int (*constructor)(struct neighbour *);
    int (*pconstructor)(struct pneigh_entry *);
    void (*pdestructor)(struct pneigh_entry *);
    void (*proxy_redo)(struct sk_buff *);
    bool (*allow_add)(const struct net_device *, struct netlink_ext_ack *);
    char *id;
    struct neigh_parms parms;
    struct list_head parms_list;
    int gc_interval;
    int gc_thresh1;
    int gc_thresh2;
    int gc_thresh3;
    long unsigned int last_flush;
    struct delayed_work gc_work;
    struct timer_list proxy_timer;
    struct sk_buff_head proxy_queue;
    atomic_t entries;
    atomic_t gc_entries;
    struct list_head gc_list;
    rwlock_t lock;
    long unsigned int last_rand;
    struct neigh_statistics *stats;
    struct neigh_hash_table *nht;
    struct pneigh_entry **phash_buckets;
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
struct neigh_table {
    int family;
    unsigned int entry_size;
    unsigned int key_len;
    __be16 protocol;
    __u32 (*hash)(const void *, const struct net_device *, __u32 *);
    bool (*key_eq)(const struct neighbour *, const void *);
    int (*constructor)(struct neighbour *);
    int (*pconstructor)(struct pneigh_entry *);
    void (*pdestructor)(struct pneigh_entry *);
    void (*proxy_redo)(struct sk_buff *);
    bool (*allow_add)(const struct net_device *, struct netlink_ext_ack *);
    char *id;
    struct neigh_parms parms;
    struct list_head parms_list;
    int gc_interval;
    int gc_thresh1;
    int gc_thresh2;
    int gc_thresh3;
    long unsigned int last_flush;
    struct delayed_work gc_work;
    struct timer_list proxy_timer;
    struct sk_buff_head proxy_queue;
    atomic_t entries;
    atomic_t gc_entries;
    struct list_head gc_list;
    rwlock_t lock;
    long unsigned int last_rand;
    struct neigh_statistics *stats;
    struct neigh_hash_table *nht;
    struct pneigh_entry **phash_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct neigh_table {
    int family;
    unsigned int entry_size;
    unsigned int key_len;
    __be16 protocol;
    __u32 (*hash)(const void *, const struct net_device *, __u32 *);
    bool (*key_eq)(const struct neighbour *, const void *);
    int (*constructor)(struct neighbour *);
    int (*pconstructor)(struct pneigh_entry *);
    void (*pdestructor)(struct pneigh_entry *);
    void (*proxy_redo)(struct sk_buff *);
    bool (*allow_add)(const struct net_device *, struct netlink_ext_ack *);
    char *id;
    struct neigh_parms parms;
    struct list_head parms_list;
    int gc_interval;
    int gc_thresh1;
    int gc_thresh2;
    int gc_thresh3;
    long unsigned int last_flush;
    struct delayed_work gc_work;
    struct timer_list proxy_timer;
    struct sk_buff_head proxy_queue;
    atomic_t entries;
    atomic_t gc_entries;
    struct list_head gc_list;
    rwlock_t lock;
    long unsigned int last_rand;
    struct neigh_statistics *stats;
    struct neigh_hash_table *nht;
    struct pneigh_entry **phash_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct neigh_table {
    int family;
    unsigned int entry_size;
    unsigned int key_len;
    __be16 protocol;
    __u32 (*hash)(const void *, const struct net_device *, __u32 *);
    bool (*key_eq)(const struct neighbour *, const void *);
    int (*constructor)(struct neighbour *);
    int (*pconstructor)(struct pneigh_entry *);
    void (*pdestructor)(struct pneigh_entry *);
    void (*proxy_redo)(struct sk_buff *);
    bool (*allow_add)(const struct net_device *, struct netlink_ext_ack *);
    char *id;
    struct neigh_parms parms;
    struct list_head parms_list;
    int gc_interval;
    int gc_thresh1;
    int gc_thresh2;
    int gc_thresh3;
    long unsigned int last_flush;
    struct delayed_work gc_work;
    struct timer_list proxy_timer;
    struct sk_buff_head proxy_queue;
    atomic_t entries;
    atomic_t gc_entries;
    struct list_head gc_list;
    rwlock_t lock;
    long unsigned int last_rand;
    struct neigh_statistics *stats;
    struct neigh_hash_table *nht;
    struct pneigh_entry **phash_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct neigh_table {
    int family;
    unsigned int entry_size;
    unsigned int key_len;
    __be16 protocol;
    __u32 (*hash)(const void *, const struct net_device *, __u32 *);
    bool (*key_eq)(const struct neighbour *, const void *);
    int (*constructor)(struct neighbour *);
    int (*pconstructor)(struct pneigh_entry *);
    void (*pdestructor)(struct pneigh_entry *);
    void (*proxy_redo)(struct sk_buff *);
    bool (*allow_add)(const struct net_device *, struct netlink_ext_ack *);
    char *id;
    struct neigh_parms parms;
    struct list_head parms_list;
    int gc_interval;
    int gc_thresh1;
    int gc_thresh2;
    int gc_thresh3;
    long unsigned int last_flush;
    struct delayed_work gc_work;
    struct timer_list proxy_timer;
    struct sk_buff_head proxy_queue;
    atomic_t entries;
    atomic_t gc_entries;
    struct list_head gc_list;
    rwlock_t lock;
    long unsigned int last_rand;
    struct neigh_statistics *stats;
    struct neigh_hash_table *nht;
    struct pneigh_entry **phash_buckets;
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
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int entry_size</code> ➡️ <code>unsigned int entry_size</code>
</li>
<li>
<b>Field type changed. </b>
<code>int key_len</code> ➡️ <code>unsigned int key_len</code>
</li>
</ul>
</details>
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
<code>atomic_t gc_entries</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head gc_list</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool (*allow_add)(const struct net_device *, struct netlink_ext_ack *)</code>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*is_multicast)(const void *)</code>
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
<code>struct delayed_work managed_work</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head managed_list</code>
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
