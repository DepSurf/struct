# Struct: <code>xfrm_policy</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct xfrm_policy {
    possible_net_t xp_net;
    struct hlist_node bydst;
    struct hlist_node byidx;
    rwlock_t lock;
    atomic_t refcnt;
    struct timer_list timer;
    struct flow_cache_object flo;
    atomic_t genid;
    u32 priority;
    u32 index;
    struct xfrm_mark mark;
    struct xfrm_selector selector;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_lifetime_cur curlft;
    struct xfrm_policy_walk_entry walk;
    struct xfrm_policy_queue polq;
    u8 type;
    u8 action;
    u8 flags;
    u8 xfrm_nr;
    u16 family;
    struct xfrm_sec_ctx *security;
    struct xfrm_tmpl xfrm_vec[6];
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct xfrm_policy {
    possible_net_t xp_net;
    struct hlist_node bydst;
    struct hlist_node byidx;
    rwlock_t lock;
    atomic_t refcnt;
    struct timer_list timer;
    struct flow_cache_object flo;
    atomic_t genid;
    u32 priority;
    u32 index;
    struct xfrm_mark mark;
    struct xfrm_selector selector;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_lifetime_cur curlft;
    struct xfrm_policy_walk_entry walk;
    struct xfrm_policy_queue polq;
    u8 type;
    u8 action;
    u8 flags;
    u8 xfrm_nr;
    u16 family;
    struct xfrm_sec_ctx *security;
    struct xfrm_tmpl xfrm_vec[6];
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct xfrm_policy {
    possible_net_t xp_net;
    struct hlist_node bydst;
    struct hlist_node byidx;
    rwlock_t lock;
    atomic_t refcnt;
    struct timer_list timer;
    struct flow_cache_object flo;
    atomic_t genid;
    u32 priority;
    u32 index;
    struct xfrm_mark mark;
    struct xfrm_selector selector;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_lifetime_cur curlft;
    struct xfrm_policy_walk_entry walk;
    struct xfrm_policy_queue polq;
    u8 type;
    u8 action;
    u8 flags;
    u8 xfrm_nr;
    u16 family;
    struct xfrm_sec_ctx *security;
    struct xfrm_tmpl xfrm_vec[6];
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct xfrm_policy {
    possible_net_t xp_net;
    struct hlist_node bydst;
    struct hlist_node byidx;
    rwlock_t lock;
    refcount_t refcnt;
    struct timer_list timer;
    struct flow_cache_object flo;
    atomic_t genid;
    u32 priority;
    u32 index;
    struct xfrm_mark mark;
    struct xfrm_selector selector;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_lifetime_cur curlft;
    struct xfrm_policy_walk_entry walk;
    struct xfrm_policy_queue polq;
    u8 type;
    u8 action;
    u8 flags;
    u8 xfrm_nr;
    u16 family;
    struct xfrm_sec_ctx *security;
    struct xfrm_tmpl xfrm_vec[6];
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct xfrm_policy {
    possible_net_t xp_net;
    struct hlist_node bydst;
    struct hlist_node byidx;
    rwlock_t lock;
    refcount_t refcnt;
    struct timer_list timer;
    atomic_t genid;
    u32 priority;
    u32 index;
    struct xfrm_mark mark;
    struct xfrm_selector selector;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_lifetime_cur curlft;
    struct xfrm_policy_walk_entry walk;
    struct xfrm_policy_queue polq;
    u8 type;
    u8 action;
    u8 flags;
    u8 xfrm_nr;
    u16 family;
    struct xfrm_sec_ctx *security;
    struct xfrm_tmpl xfrm_vec[6];
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct xfrm_policy {
    possible_net_t xp_net;
    struct hlist_node bydst;
    struct hlist_node byidx;
    rwlock_t lock;
    refcount_t refcnt;
    struct timer_list timer;
    atomic_t genid;
    u32 priority;
    u32 index;
    struct xfrm_mark mark;
    struct xfrm_selector selector;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_lifetime_cur curlft;
    struct xfrm_policy_walk_entry walk;
    struct xfrm_policy_queue polq;
    u8 type;
    u8 action;
    u8 flags;
    u8 xfrm_nr;
    u16 family;
    struct xfrm_sec_ctx *security;
    struct xfrm_tmpl xfrm_vec[6];
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct xfrm_policy {
    possible_net_t xp_net;
    struct hlist_node bydst;
    struct hlist_node byidx;
    rwlock_t lock;
    refcount_t refcnt;
    u32 pos;
    struct timer_list timer;
    atomic_t genid;
    u32 priority;
    u32 index;
    u32 if_id;
    struct xfrm_mark mark;
    struct xfrm_selector selector;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_lifetime_cur curlft;
    struct xfrm_policy_walk_entry walk;
    struct xfrm_policy_queue polq;
    bool bydst_reinsert;
    u8 type;
    u8 action;
    u8 flags;
    u8 xfrm_nr;
    u16 family;
    struct xfrm_sec_ctx *security;
    struct xfrm_tmpl xfrm_vec[6];
    struct hlist_node bydst_inexact_list;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct xfrm_policy {
    possible_net_t xp_net;
    struct hlist_node bydst;
    struct hlist_node byidx;
    rwlock_t lock;
    refcount_t refcnt;
    u32 pos;
    struct timer_list timer;
    atomic_t genid;
    u32 priority;
    u32 index;
    u32 if_id;
    struct xfrm_mark mark;
    struct xfrm_selector selector;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_lifetime_cur curlft;
    struct xfrm_policy_walk_entry walk;
    struct xfrm_policy_queue polq;
    bool bydst_reinsert;
    u8 type;
    u8 action;
    u8 flags;
    u8 xfrm_nr;
    u16 family;
    struct xfrm_sec_ctx *security;
    struct xfrm_tmpl xfrm_vec[6];
    struct hlist_node bydst_inexact_list;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct xfrm_policy {
    possible_net_t xp_net;
    struct hlist_node bydst;
    struct hlist_node byidx;
    rwlock_t lock;
    refcount_t refcnt;
    u32 pos;
    struct timer_list timer;
    atomic_t genid;
    u32 priority;
    u32 index;
    u32 if_id;
    struct xfrm_mark mark;
    struct xfrm_selector selector;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_lifetime_cur curlft;
    struct xfrm_policy_walk_entry walk;
    struct xfrm_policy_queue polq;
    bool bydst_reinsert;
    u8 type;
    u8 action;
    u8 flags;
    u8 xfrm_nr;
    u16 family;
    struct xfrm_sec_ctx *security;
    struct xfrm_tmpl xfrm_vec[6];
    struct hlist_node bydst_inexact_list;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct xfrm_policy {
    possible_net_t xp_net;
    struct hlist_node bydst;
    struct hlist_node byidx;
    rwlock_t lock;
    refcount_t refcnt;
    u32 pos;
    struct timer_list timer;
    atomic_t genid;
    u32 priority;
    u32 index;
    u32 if_id;
    struct xfrm_mark mark;
    struct xfrm_selector selector;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_lifetime_cur curlft;
    struct xfrm_policy_walk_entry walk;
    struct xfrm_policy_queue polq;
    bool bydst_reinsert;
    u8 type;
    u8 action;
    u8 flags;
    u8 xfrm_nr;
    u16 family;
    struct xfrm_sec_ctx *security;
    struct xfrm_tmpl xfrm_vec[6];
    struct hlist_node bydst_inexact_list;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct xfrm_policy {
    possible_net_t xp_net;
    struct hlist_node bydst;
    struct hlist_node byidx;
    rwlock_t lock;
    refcount_t refcnt;
    u32 pos;
    struct timer_list timer;
    atomic_t genid;
    u32 priority;
    u32 index;
    u32 if_id;
    struct xfrm_mark mark;
    struct xfrm_selector selector;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_lifetime_cur curlft;
    struct xfrm_policy_walk_entry walk;
    struct xfrm_policy_queue polq;
    bool bydst_reinsert;
    u8 type;
    u8 action;
    u8 flags;
    u8 xfrm_nr;
    u16 family;
    struct xfrm_sec_ctx *security;
    struct xfrm_tmpl xfrm_vec[6];
    struct hlist_node bydst_inexact_list;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct xfrm_policy {
    possible_net_t xp_net;
    struct hlist_node bydst;
    struct hlist_node byidx;
    rwlock_t lock;
    refcount_t refcnt;
    u32 pos;
    struct timer_list timer;
    atomic_t genid;
    u32 priority;
    u32 index;
    u32 if_id;
    struct xfrm_mark mark;
    struct xfrm_selector selector;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_lifetime_cur curlft;
    struct xfrm_policy_walk_entry walk;
    struct xfrm_policy_queue polq;
    bool bydst_reinsert;
    u8 type;
    u8 action;
    u8 flags;
    u8 xfrm_nr;
    u16 family;
    struct xfrm_sec_ctx *security;
    struct xfrm_tmpl xfrm_vec[6];
    struct hlist_node bydst_inexact_list;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct xfrm_policy {
    possible_net_t xp_net;
    struct hlist_node bydst;
    struct hlist_node byidx;
    rwlock_t lock;
    refcount_t refcnt;
    u32 pos;
    struct timer_list timer;
    atomic_t genid;
    u32 priority;
    u32 index;
    u32 if_id;
    struct xfrm_mark mark;
    struct xfrm_selector selector;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_lifetime_cur curlft;
    struct xfrm_policy_walk_entry walk;
    struct xfrm_policy_queue polq;
    bool bydst_reinsert;
    u8 type;
    u8 action;
    u8 flags;
    u8 xfrm_nr;
    u16 family;
    struct xfrm_sec_ctx *security;
    struct xfrm_tmpl xfrm_vec[6];
    struct hlist_node bydst_inexact_list;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct xfrm_policy {
    possible_net_t xp_net;
    struct hlist_node bydst;
    struct hlist_node byidx;
    rwlock_t lock;
    refcount_t refcnt;
    u32 pos;
    struct timer_list timer;
    atomic_t genid;
    u32 priority;
    u32 index;
    u32 if_id;
    struct xfrm_mark mark;
    struct xfrm_selector selector;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_lifetime_cur curlft;
    struct xfrm_policy_walk_entry walk;
    struct xfrm_policy_queue polq;
    bool bydst_reinsert;
    u8 type;
    u8 action;
    u8 flags;
    u8 xfrm_nr;
    u16 family;
    struct xfrm_sec_ctx *security;
    struct xfrm_tmpl xfrm_vec[6];
    struct hlist_node bydst_inexact_list;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct xfrm_policy {
    possible_net_t xp_net;
    struct hlist_node bydst;
    struct hlist_node byidx;
    rwlock_t lock;
    refcount_t refcnt;
    u32 pos;
    struct timer_list timer;
    atomic_t genid;
    u32 priority;
    u32 index;
    u32 if_id;
    struct xfrm_mark mark;
    struct xfrm_selector selector;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_lifetime_cur curlft;
    struct xfrm_policy_walk_entry walk;
    struct xfrm_policy_queue polq;
    bool bydst_reinsert;
    u8 type;
    u8 action;
    u8 flags;
    u8 xfrm_nr;
    u16 family;
    struct xfrm_sec_ctx *security;
    struct xfrm_tmpl xfrm_vec[6];
    struct hlist_node bydst_inexact_list;
    struct callback_head rcu;
    struct xfrm_dev_offload xdo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct xfrm_policy {
    possible_net_t xp_net;
    struct hlist_node bydst;
    struct hlist_node byidx;
    rwlock_t lock;
    refcount_t refcnt;
    u32 pos;
    struct timer_list timer;
    atomic_t genid;
    u32 priority;
    u32 index;
    u32 if_id;
    struct xfrm_mark mark;
    struct xfrm_selector selector;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_lifetime_cur curlft;
    struct xfrm_policy_walk_entry walk;
    struct xfrm_policy_queue polq;
    bool bydst_reinsert;
    u8 type;
    u8 action;
    u8 flags;
    u8 xfrm_nr;
    u16 family;
    struct xfrm_sec_ctx *security;
    struct xfrm_tmpl xfrm_vec[6];
    struct hlist_node bydst_inexact_list;
    struct callback_head rcu;
    struct xfrm_dev_offload xdo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct xfrm_policy {
    possible_net_t xp_net;
    struct hlist_node bydst;
    struct hlist_node byidx;
    rwlock_t lock;
    refcount_t refcnt;
    u32 pos;
    struct timer_list timer;
    atomic_t genid;
    u32 priority;
    u32 index;
    u32 if_id;
    struct xfrm_mark mark;
    struct xfrm_selector selector;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_lifetime_cur curlft;
    struct xfrm_policy_walk_entry walk;
    struct xfrm_policy_queue polq;
    bool bydst_reinsert;
    u8 type;
    u8 action;
    u8 flags;
    u8 xfrm_nr;
    u16 family;
    struct xfrm_sec_ctx *security;
    struct xfrm_tmpl xfrm_vec[6];
    struct hlist_node bydst_inexact_list;
    struct callback_head rcu;
    struct xfrm_dev_offload xdo;
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
struct xfrm_policy {
    possible_net_t xp_net;
    struct hlist_node bydst;
    struct hlist_node byidx;
    rwlock_t lock;
    refcount_t refcnt;
    u32 pos;
    struct timer_list timer;
    atomic_t genid;
    u32 priority;
    u32 index;
    u32 if_id;
    struct xfrm_mark mark;
    struct xfrm_selector selector;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_lifetime_cur curlft;
    struct xfrm_policy_walk_entry walk;
    struct xfrm_policy_queue polq;
    bool bydst_reinsert;
    u8 type;
    u8 action;
    u8 flags;
    u8 xfrm_nr;
    u16 family;
    struct xfrm_sec_ctx *security;
    struct xfrm_tmpl xfrm_vec[6];
    struct hlist_node bydst_inexact_list;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct xfrm_policy {
    possible_net_t xp_net;
    struct hlist_node bydst;
    struct hlist_node byidx;
    rwlock_t lock;
    refcount_t refcnt;
    u32 pos;
    struct timer_list timer;
    atomic_t genid;
    u32 priority;
    u32 index;
    u32 if_id;
    struct xfrm_mark mark;
    struct xfrm_selector selector;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_lifetime_cur curlft;
    struct xfrm_policy_walk_entry walk;
    struct xfrm_policy_queue polq;
    bool bydst_reinsert;
    u8 type;
    u8 action;
    u8 flags;
    u8 xfrm_nr;
    u16 family;
    struct xfrm_sec_ctx *security;
    struct xfrm_tmpl xfrm_vec[6];
    struct hlist_node bydst_inexact_list;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct xfrm_policy {
    possible_net_t xp_net;
    struct hlist_node bydst;
    struct hlist_node byidx;
    rwlock_t lock;
    refcount_t refcnt;
    u32 pos;
    struct timer_list timer;
    atomic_t genid;
    u32 priority;
    u32 index;
    u32 if_id;
    struct xfrm_mark mark;
    struct xfrm_selector selector;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_lifetime_cur curlft;
    struct xfrm_policy_walk_entry walk;
    struct xfrm_policy_queue polq;
    bool bydst_reinsert;
    u8 type;
    u8 action;
    u8 flags;
    u8 xfrm_nr;
    u16 family;
    struct xfrm_sec_ctx *security;
    struct xfrm_tmpl xfrm_vec[6];
    struct hlist_node bydst_inexact_list;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct xfrm_policy {
    possible_net_t xp_net;
    struct hlist_node bydst;
    struct hlist_node byidx;
    rwlock_t lock;
    refcount_t refcnt;
    u32 pos;
    struct timer_list timer;
    atomic_t genid;
    u32 priority;
    u32 index;
    u32 if_id;
    struct xfrm_mark mark;
    struct xfrm_selector selector;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_lifetime_cur curlft;
    struct xfrm_policy_walk_entry walk;
    struct xfrm_policy_queue polq;
    bool bydst_reinsert;
    u8 type;
    u8 action;
    u8 flags;
    u8 xfrm_nr;
    u16 family;
    struct xfrm_sec_ctx *security;
    struct xfrm_tmpl xfrm_vec[6];
    struct hlist_node bydst_inexact_list;
    struct callback_head rcu;
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
struct xfrm_policy {
    possible_net_t xp_net;
    struct hlist_node bydst;
    struct hlist_node byidx;
    rwlock_t lock;
    refcount_t refcnt;
    u32 pos;
    struct timer_list timer;
    atomic_t genid;
    u32 priority;
    u32 index;
    u32 if_id;
    struct xfrm_mark mark;
    struct xfrm_selector selector;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_lifetime_cur curlft;
    struct xfrm_policy_walk_entry walk;
    struct xfrm_policy_queue polq;
    bool bydst_reinsert;
    u8 type;
    u8 action;
    u8 flags;
    u8 xfrm_nr;
    u16 family;
    struct xfrm_sec_ctx *security;
    struct xfrm_tmpl xfrm_vec[6];
    struct hlist_node bydst_inexact_list;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct xfrm_policy {
    possible_net_t xp_net;
    struct hlist_node bydst;
    struct hlist_node byidx;
    rwlock_t lock;
    refcount_t refcnt;
    u32 pos;
    struct timer_list timer;
    atomic_t genid;
    u32 priority;
    u32 index;
    u32 if_id;
    struct xfrm_mark mark;
    struct xfrm_selector selector;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_lifetime_cur curlft;
    struct xfrm_policy_walk_entry walk;
    struct xfrm_policy_queue polq;
    bool bydst_reinsert;
    u8 type;
    u8 action;
    u8 flags;
    u8 xfrm_nr;
    u16 family;
    struct xfrm_sec_ctx *security;
    struct xfrm_tmpl xfrm_vec[6];
    struct hlist_node bydst_inexact_list;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct xfrm_policy {
    possible_net_t xp_net;
    struct hlist_node bydst;
    struct hlist_node byidx;
    rwlock_t lock;
    refcount_t refcnt;
    u32 pos;
    struct timer_list timer;
    atomic_t genid;
    u32 priority;
    u32 index;
    u32 if_id;
    struct xfrm_mark mark;
    struct xfrm_selector selector;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_lifetime_cur curlft;
    struct xfrm_policy_walk_entry walk;
    struct xfrm_policy_queue polq;
    bool bydst_reinsert;
    u8 type;
    u8 action;
    u8 flags;
    u8 xfrm_nr;
    u16 family;
    struct xfrm_sec_ctx *security;
    struct xfrm_tmpl xfrm_vec[6];
    struct hlist_node bydst_inexact_list;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct xfrm_policy {
    possible_net_t xp_net;
    struct hlist_node bydst;
    struct hlist_node byidx;
    rwlock_t lock;
    refcount_t refcnt;
    u32 pos;
    struct timer_list timer;
    atomic_t genid;
    u32 priority;
    u32 index;
    u32 if_id;
    struct xfrm_mark mark;
    struct xfrm_selector selector;
    struct xfrm_lifetime_cfg lft;
    struct xfrm_lifetime_cur curlft;
    struct xfrm_policy_walk_entry walk;
    struct xfrm_policy_queue polq;
    bool bydst_reinsert;
    u8 type;
    u8 action;
    u8 flags;
    u8 xfrm_nr;
    u16 family;
    struct xfrm_sec_ctx *security;
    struct xfrm_tmpl xfrm_vec[6];
    struct hlist_node bydst_inexact_list;
    struct callback_head rcu;
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
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct flow_cache_object flo</code>
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
<code>u32 pos</code>
</li>
<li>
<b>Field added. </b>
<code>u32 if_id</code>
</li>
<li>
<b>Field added. </b>
<code>bool bydst_reinsert</code>
</li>
<li>
<b>Field added. </b>
<code>struct hlist_node bydst_inexact_list</code>
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
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct xfrm_dev_offload xdo</code>
</li>
</ul>
</details>
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
