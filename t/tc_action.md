# Struct: <code>tc_action</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct tc_action {
    void *priv;
    const struct tc_action_ops *ops;
    __u32 type;
    __u32 order;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct tc_action {
    const struct tc_action_ops *ops;
    __u32 type;
    __u32 order;
    struct list_head list;
    struct tcf_hashinfo *hinfo;
    struct hlist_node tcfa_head;
    u32 tcfa_index;
    int tcfa_refcnt;
    int tcfa_bindcnt;
    u32 tcfa_capab;
    int tcfa_action;
    struct tcf_t tcfa_tm;
    struct gnet_stats_basic_packed tcfa_bstats;
    struct gnet_stats_queue tcfa_qstats;
    struct gnet_stats_rate_est64 tcfa_rate_est;
    spinlock_t tcfa_lock;
    struct callback_head tcfa_rcu;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_queue *cpu_qstats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct tc_action {
    const struct tc_action_ops *ops;
    __u32 type;
    __u32 order;
    struct list_head list;
    struct tcf_hashinfo *hinfo;
    struct hlist_node tcfa_head;
    u32 tcfa_index;
    int tcfa_refcnt;
    int tcfa_bindcnt;
    u32 tcfa_capab;
    int tcfa_action;
    struct tcf_t tcfa_tm;
    struct gnet_stats_basic_packed tcfa_bstats;
    struct gnet_stats_queue tcfa_qstats;
    struct net_rate_estimator *tcfa_rate_est;
    spinlock_t tcfa_lock;
    struct callback_head tcfa_rcu;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_queue *cpu_qstats;
    struct tc_cookie *act_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct tc_action {
    const struct tc_action_ops *ops;
    __u32 type;
    __u32 order;
    struct list_head list;
    struct tcf_hashinfo *hinfo;
    struct hlist_node tcfa_head;
    u32 tcfa_index;
    int tcfa_refcnt;
    int tcfa_bindcnt;
    u32 tcfa_capab;
    int tcfa_action;
    struct tcf_t tcfa_tm;
    struct gnet_stats_basic_packed tcfa_bstats;
    struct gnet_stats_queue tcfa_qstats;
    struct net_rate_estimator *tcfa_rate_est;
    spinlock_t tcfa_lock;
    struct callback_head tcfa_rcu;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_queue *cpu_qstats;
    struct tc_cookie *act_cookie;
    struct tcf_chain *goto_chain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct tc_action {
    const struct tc_action_ops *ops;
    __u32 type;
    __u32 order;
    struct list_head list;
    struct tcf_idrinfo *idrinfo;
    u32 tcfa_index;
    int tcfa_refcnt;
    int tcfa_bindcnt;
    u32 tcfa_capab;
    int tcfa_action;
    struct tcf_t tcfa_tm;
    struct gnet_stats_basic_packed tcfa_bstats;
    struct gnet_stats_queue tcfa_qstats;
    struct net_rate_estimator *tcfa_rate_est;
    spinlock_t tcfa_lock;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_queue *cpu_qstats;
    struct tc_cookie *act_cookie;
    struct tcf_chain *goto_chain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct tc_action {
    const struct tc_action_ops *ops;
    __u32 type;
    __u32 order;
    struct list_head list;
    struct tcf_idrinfo *idrinfo;
    u32 tcfa_index;
    int tcfa_refcnt;
    int tcfa_bindcnt;
    u32 tcfa_capab;
    int tcfa_action;
    struct tcf_t tcfa_tm;
    struct gnet_stats_basic_packed tcfa_bstats;
    struct gnet_stats_queue tcfa_qstats;
    struct net_rate_estimator *tcfa_rate_est;
    spinlock_t tcfa_lock;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_queue *cpu_qstats;
    struct tc_cookie *act_cookie;
    struct tcf_chain *goto_chain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct tc_action {
    const struct tc_action_ops *ops;
    __u32 type;
    __u32 order;
    struct tcf_idrinfo *idrinfo;
    u32 tcfa_index;
    refcount_t tcfa_refcnt;
    atomic_t tcfa_bindcnt;
    int tcfa_action;
    struct tcf_t tcfa_tm;
    struct gnet_stats_basic_packed tcfa_bstats;
    struct gnet_stats_basic_packed tcfa_bstats_hw;
    struct gnet_stats_queue tcfa_qstats;
    struct net_rate_estimator *tcfa_rate_est;
    spinlock_t tcfa_lock;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_basic_cpu *cpu_bstats_hw;
    struct gnet_stats_queue *cpu_qstats;
    struct tc_cookie *act_cookie;
    struct tcf_chain *goto_chain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct tc_action {
    const struct tc_action_ops *ops;
    __u32 type;
    __u32 order;
    struct tcf_idrinfo *idrinfo;
    u32 tcfa_index;
    refcount_t tcfa_refcnt;
    atomic_t tcfa_bindcnt;
    int tcfa_action;
    struct tcf_t tcfa_tm;
    struct gnet_stats_basic_packed tcfa_bstats;
    struct gnet_stats_basic_packed tcfa_bstats_hw;
    struct gnet_stats_queue tcfa_qstats;
    struct net_rate_estimator *tcfa_rate_est;
    spinlock_t tcfa_lock;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_basic_cpu *cpu_bstats_hw;
    struct gnet_stats_queue *cpu_qstats;
    struct tc_cookie *act_cookie;
    struct tcf_chain *goto_chain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct tc_action {
    const struct tc_action_ops *ops;
    __u32 type;
    __u32 order;
    struct tcf_idrinfo *idrinfo;
    u32 tcfa_index;
    refcount_t tcfa_refcnt;
    atomic_t tcfa_bindcnt;
    int tcfa_action;
    struct tcf_t tcfa_tm;
    struct gnet_stats_basic_packed tcfa_bstats;
    struct gnet_stats_basic_packed tcfa_bstats_hw;
    struct gnet_stats_queue tcfa_qstats;
    struct net_rate_estimator *tcfa_rate_est;
    spinlock_t tcfa_lock;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_basic_cpu *cpu_bstats_hw;
    struct gnet_stats_queue *cpu_qstats;
    struct tc_cookie *act_cookie;
    struct tcf_chain *goto_chain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct tc_action {
    const struct tc_action_ops *ops;
    __u32 type;
    struct tcf_idrinfo *idrinfo;
    u32 tcfa_index;
    refcount_t tcfa_refcnt;
    atomic_t tcfa_bindcnt;
    int tcfa_action;
    struct tcf_t tcfa_tm;
    struct gnet_stats_basic_packed tcfa_bstats;
    struct gnet_stats_basic_packed tcfa_bstats_hw;
    struct gnet_stats_queue tcfa_qstats;
    struct net_rate_estimator *tcfa_rate_est;
    spinlock_t tcfa_lock;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_basic_cpu *cpu_bstats_hw;
    struct gnet_stats_queue *cpu_qstats;
    struct tc_cookie *act_cookie;
    struct tcf_chain *goto_chain;
    u32 tcfa_flags;
    u8 hw_stats;
    u8 used_hw_stats;
    bool used_hw_stats_valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct tc_action {
    const struct tc_action_ops *ops;
    __u32 type;
    struct tcf_idrinfo *idrinfo;
    u32 tcfa_index;
    refcount_t tcfa_refcnt;
    atomic_t tcfa_bindcnt;
    int tcfa_action;
    struct tcf_t tcfa_tm;
    struct gnet_stats_basic_packed tcfa_bstats;
    struct gnet_stats_basic_packed tcfa_bstats_hw;
    struct gnet_stats_queue tcfa_qstats;
    struct net_rate_estimator *tcfa_rate_est;
    spinlock_t tcfa_lock;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_basic_cpu *cpu_bstats_hw;
    struct gnet_stats_queue *cpu_qstats;
    struct tc_cookie *act_cookie;
    struct tcf_chain *goto_chain;
    u32 tcfa_flags;
    u8 hw_stats;
    u8 used_hw_stats;
    bool used_hw_stats_valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct tc_action {
    const struct tc_action_ops *ops;
    __u32 type;
    struct tcf_idrinfo *idrinfo;
    u32 tcfa_index;
    refcount_t tcfa_refcnt;
    atomic_t tcfa_bindcnt;
    int tcfa_action;
    struct tcf_t tcfa_tm;
    struct gnet_stats_basic_packed tcfa_bstats;
    struct gnet_stats_basic_packed tcfa_bstats_hw;
    struct gnet_stats_queue tcfa_qstats;
    struct net_rate_estimator *tcfa_rate_est;
    spinlock_t tcfa_lock;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_basic_cpu *cpu_bstats_hw;
    struct gnet_stats_queue *cpu_qstats;
    struct tc_cookie *act_cookie;
    struct tcf_chain *goto_chain;
    u32 tcfa_flags;
    u8 hw_stats;
    u8 used_hw_stats;
    bool used_hw_stats_valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct tc_action {
    const struct tc_action_ops *ops;
    __u32 type;
    struct tcf_idrinfo *idrinfo;
    u32 tcfa_index;
    refcount_t tcfa_refcnt;
    atomic_t tcfa_bindcnt;
    int tcfa_action;
    struct tcf_t tcfa_tm;
    struct gnet_stats_basic_packed tcfa_bstats;
    struct gnet_stats_basic_packed tcfa_bstats_hw;
    struct gnet_stats_queue tcfa_qstats;
    struct net_rate_estimator *tcfa_rate_est;
    spinlock_t tcfa_lock;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_basic_cpu *cpu_bstats_hw;
    struct gnet_stats_queue *cpu_qstats;
    struct tc_cookie *act_cookie;
    struct tcf_chain *goto_chain;
    u32 tcfa_flags;
    u8 hw_stats;
    u8 used_hw_stats;
    bool used_hw_stats_valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct tc_action {
    const struct tc_action_ops *ops;
    __u32 type;
    struct tcf_idrinfo *idrinfo;
    u32 tcfa_index;
    refcount_t tcfa_refcnt;
    atomic_t tcfa_bindcnt;
    int tcfa_action;
    struct tcf_t tcfa_tm;
    struct gnet_stats_basic_sync tcfa_bstats;
    struct gnet_stats_basic_sync tcfa_bstats_hw;
    struct gnet_stats_queue tcfa_qstats;
    struct net_rate_estimator *tcfa_rate_est;
    spinlock_t tcfa_lock;
    struct gnet_stats_basic_sync *cpu_bstats;
    struct gnet_stats_basic_sync *cpu_bstats_hw;
    struct gnet_stats_queue *cpu_qstats;
    struct tc_cookie *act_cookie;
    struct tcf_chain *goto_chain;
    u32 tcfa_flags;
    u8 hw_stats;
    u8 used_hw_stats;
    bool used_hw_stats_valid;
    u32 in_hw_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct tc_action {
    const struct tc_action_ops *ops;
    __u32 type;
    struct tcf_idrinfo *idrinfo;
    u32 tcfa_index;
    refcount_t tcfa_refcnt;
    atomic_t tcfa_bindcnt;
    int tcfa_action;
    struct tcf_t tcfa_tm;
    struct gnet_stats_basic_sync tcfa_bstats;
    struct gnet_stats_basic_sync tcfa_bstats_hw;
    struct gnet_stats_queue tcfa_qstats;
    struct net_rate_estimator *tcfa_rate_est;
    spinlock_t tcfa_lock;
    struct gnet_stats_basic_sync *cpu_bstats;
    struct gnet_stats_basic_sync *cpu_bstats_hw;
    struct gnet_stats_queue *cpu_qstats;
    struct tc_cookie *act_cookie;
    struct tcf_chain *goto_chain;
    u32 tcfa_flags;
    u8 hw_stats;
    u8 used_hw_stats;
    bool used_hw_stats_valid;
    u32 in_hw_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct tc_action {
    const struct tc_action_ops *ops;
    __u32 type;
    struct tcf_idrinfo *idrinfo;
    u32 tcfa_index;
    refcount_t tcfa_refcnt;
    atomic_t tcfa_bindcnt;
    int tcfa_action;
    struct tcf_t tcfa_tm;
    struct gnet_stats_basic_sync tcfa_bstats;
    struct gnet_stats_basic_sync tcfa_bstats_hw;
    struct gnet_stats_queue tcfa_qstats;
    struct net_rate_estimator *tcfa_rate_est;
    spinlock_t tcfa_lock;
    struct gnet_stats_basic_sync *cpu_bstats;
    struct gnet_stats_basic_sync *cpu_bstats_hw;
    struct gnet_stats_queue *cpu_qstats;
    struct tc_cookie *user_cookie;
    struct tcf_chain *goto_chain;
    u32 tcfa_flags;
    u8 hw_stats;
    u8 used_hw_stats;
    bool used_hw_stats_valid;
    u32 in_hw_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct tc_action {
    const struct tc_action_ops *ops;
    __u32 type;
    struct tcf_idrinfo *idrinfo;
    u32 tcfa_index;
    refcount_t tcfa_refcnt;
    atomic_t tcfa_bindcnt;
    int tcfa_action;
    struct tcf_t tcfa_tm;
    struct gnet_stats_basic_sync tcfa_bstats;
    struct gnet_stats_basic_sync tcfa_bstats_hw;
    struct gnet_stats_queue tcfa_qstats;
    struct net_rate_estimator *tcfa_rate_est;
    spinlock_t tcfa_lock;
    struct gnet_stats_basic_sync *cpu_bstats;
    struct gnet_stats_basic_sync *cpu_bstats_hw;
    struct gnet_stats_queue *cpu_qstats;
    struct tc_cookie *user_cookie;
    struct tcf_chain *goto_chain;
    u32 tcfa_flags;
    u8 hw_stats;
    u8 used_hw_stats;
    bool used_hw_stats_valid;
    u32 in_hw_count;
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
struct tc_action {
    const struct tc_action_ops *ops;
    __u32 type;
    __u32 order;
    struct tcf_idrinfo *idrinfo;
    u32 tcfa_index;
    refcount_t tcfa_refcnt;
    atomic_t tcfa_bindcnt;
    int tcfa_action;
    struct tcf_t tcfa_tm;
    struct gnet_stats_basic_packed tcfa_bstats;
    struct gnet_stats_basic_packed tcfa_bstats_hw;
    struct gnet_stats_queue tcfa_qstats;
    struct net_rate_estimator *tcfa_rate_est;
    spinlock_t tcfa_lock;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_basic_cpu *cpu_bstats_hw;
    struct gnet_stats_queue *cpu_qstats;
    struct tc_cookie *act_cookie;
    struct tcf_chain *goto_chain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct tc_action {
    const struct tc_action_ops *ops;
    __u32 type;
    __u32 order;
    struct tcf_idrinfo *idrinfo;
    u32 tcfa_index;
    refcount_t tcfa_refcnt;
    atomic_t tcfa_bindcnt;
    int tcfa_action;
    struct tcf_t tcfa_tm;
    struct gnet_stats_basic_packed tcfa_bstats;
    struct gnet_stats_basic_packed tcfa_bstats_hw;
    struct gnet_stats_queue tcfa_qstats;
    struct net_rate_estimator *tcfa_rate_est;
    spinlock_t tcfa_lock;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_basic_cpu *cpu_bstats_hw;
    struct gnet_stats_queue *cpu_qstats;
    struct tc_cookie *act_cookie;
    struct tcf_chain *goto_chain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct tc_action {
    const struct tc_action_ops *ops;
    __u32 type;
    __u32 order;
    struct tcf_idrinfo *idrinfo;
    u32 tcfa_index;
    refcount_t tcfa_refcnt;
    atomic_t tcfa_bindcnt;
    int tcfa_action;
    struct tcf_t tcfa_tm;
    struct gnet_stats_basic_packed tcfa_bstats;
    struct gnet_stats_basic_packed tcfa_bstats_hw;
    struct gnet_stats_queue tcfa_qstats;
    struct net_rate_estimator *tcfa_rate_est;
    spinlock_t tcfa_lock;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_basic_cpu *cpu_bstats_hw;
    struct gnet_stats_queue *cpu_qstats;
    struct tc_cookie *act_cookie;
    struct tcf_chain *goto_chain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct tc_action {
    const struct tc_action_ops *ops;
    __u32 type;
    __u32 order;
    struct tcf_idrinfo *idrinfo;
    u32 tcfa_index;
    refcount_t tcfa_refcnt;
    atomic_t tcfa_bindcnt;
    int tcfa_action;
    struct tcf_t tcfa_tm;
    struct gnet_stats_basic_packed tcfa_bstats;
    struct gnet_stats_basic_packed tcfa_bstats_hw;
    struct gnet_stats_queue tcfa_qstats;
    struct net_rate_estimator *tcfa_rate_est;
    spinlock_t tcfa_lock;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_basic_cpu *cpu_bstats_hw;
    struct gnet_stats_queue *cpu_qstats;
    struct tc_cookie *act_cookie;
    struct tcf_chain *goto_chain;
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
struct tc_action {
    const struct tc_action_ops *ops;
    __u32 type;
    __u32 order;
    struct tcf_idrinfo *idrinfo;
    u32 tcfa_index;
    refcount_t tcfa_refcnt;
    atomic_t tcfa_bindcnt;
    int tcfa_action;
    struct tcf_t tcfa_tm;
    struct gnet_stats_basic_packed tcfa_bstats;
    struct gnet_stats_basic_packed tcfa_bstats_hw;
    struct gnet_stats_queue tcfa_qstats;
    struct net_rate_estimator *tcfa_rate_est;
    spinlock_t tcfa_lock;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_basic_cpu *cpu_bstats_hw;
    struct gnet_stats_queue *cpu_qstats;
    struct tc_cookie *act_cookie;
    struct tcf_chain *goto_chain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct tc_action {
    const struct tc_action_ops *ops;
    __u32 type;
    __u32 order;
    struct tcf_idrinfo *idrinfo;
    u32 tcfa_index;
    refcount_t tcfa_refcnt;
    atomic_t tcfa_bindcnt;
    int tcfa_action;
    struct tcf_t tcfa_tm;
    struct gnet_stats_basic_packed tcfa_bstats;
    struct gnet_stats_basic_packed tcfa_bstats_hw;
    struct gnet_stats_queue tcfa_qstats;
    struct net_rate_estimator *tcfa_rate_est;
    spinlock_t tcfa_lock;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_basic_cpu *cpu_bstats_hw;
    struct gnet_stats_queue *cpu_qstats;
    struct tc_cookie *act_cookie;
    struct tcf_chain *goto_chain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct tc_action {
    const struct tc_action_ops *ops;
    __u32 type;
    __u32 order;
    struct tcf_idrinfo *idrinfo;
    u32 tcfa_index;
    refcount_t tcfa_refcnt;
    atomic_t tcfa_bindcnt;
    int tcfa_action;
    struct tcf_t tcfa_tm;
    struct gnet_stats_basic_packed tcfa_bstats;
    struct gnet_stats_basic_packed tcfa_bstats_hw;
    struct gnet_stats_queue tcfa_qstats;
    struct net_rate_estimator *tcfa_rate_est;
    spinlock_t tcfa_lock;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_basic_cpu *cpu_bstats_hw;
    struct gnet_stats_queue *cpu_qstats;
    struct tc_cookie *act_cookie;
    struct tcf_chain *goto_chain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct tc_action {
    const struct tc_action_ops *ops;
    __u32 type;
    __u32 order;
    struct tcf_idrinfo *idrinfo;
    u32 tcfa_index;
    refcount_t tcfa_refcnt;
    atomic_t tcfa_bindcnt;
    int tcfa_action;
    struct tcf_t tcfa_tm;
    struct gnet_stats_basic_packed tcfa_bstats;
    struct gnet_stats_basic_packed tcfa_bstats_hw;
    struct gnet_stats_queue tcfa_qstats;
    struct net_rate_estimator *tcfa_rate_est;
    spinlock_t tcfa_lock;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_basic_cpu *cpu_bstats_hw;
    struct gnet_stats_queue *cpu_qstats;
    struct tc_cookie *act_cookie;
    struct tcf_chain *goto_chain;
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
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct tcf_hashinfo *hinfo</code>
</li>
<li>
<b>Field added. </b>
<code>struct hlist_node tcfa_head</code>
</li>
<li>
<b>Field added. </b>
<code>u32 tcfa_index</code>
</li>
<li>
<b>Field added. </b>
<code>int tcfa_refcnt</code>
</li>
<li>
<b>Field added. </b>
<code>int tcfa_bindcnt</code>
</li>
<li>
<b>Field added. </b>
<code>u32 tcfa_capab</code>
</li>
<li>
<b>Field added. </b>
<code>int tcfa_action</code>
</li>
<li>
<b>Field added. </b>
<code>struct tcf_t tcfa_tm</code>
</li>
<li>
<b>Field added. </b>
<code>struct gnet_stats_basic_packed tcfa_bstats</code>
</li>
<li>
<b>Field added. </b>
<code>struct gnet_stats_queue tcfa_qstats</code>
</li>
<li>
<b>Field added. </b>
<code>struct gnet_stats_rate_est64 tcfa_rate_est</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t tcfa_lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct callback_head tcfa_rcu</code>
</li>
<li>
<b>Field added. </b>
<code>struct gnet_stats_basic_cpu *cpu_bstats</code>
</li>
<li>
<b>Field added. </b>
<code>struct gnet_stats_queue *cpu_qstats</code>
</li>
<li>
<b>Field removed. </b>
<code>void *priv</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct tc_cookie *act_cookie</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct gnet_stats_rate_est64 tcfa_rate_est</code> ➡️ <code>struct net_rate_estimator *tcfa_rate_est</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct tcf_chain *goto_chain</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct tcf_idrinfo *idrinfo</code>
</li>
<li>
<b>Field removed. </b>
<code>struct tcf_hashinfo *hinfo</code>
</li>
<li>
<b>Field removed. </b>
<code>struct hlist_node tcfa_head</code>
</li>
<li>
<b>Field removed. </b>
<code>struct callback_head tcfa_rcu</code>
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
<code>struct gnet_stats_basic_packed tcfa_bstats_hw</code>
</li>
<li>
<b>Field added. </b>
<code>struct gnet_stats_basic_cpu *cpu_bstats_hw</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head list</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 tcfa_capab</code>
</li>
<li>
<b>Field type changed. </b>
<code>int tcfa_refcnt</code> ➡️ <code>refcount_t tcfa_refcnt</code>
</li>
<li>
<b>Field type changed. </b>
<code>int tcfa_bindcnt</code> ➡️ <code>atomic_t tcfa_bindcnt</code>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 tcfa_flags</code>
</li>
<li>
<b>Field added. </b>
<code>u8 hw_stats</code>
</li>
<li>
<b>Field added. </b>
<code>u8 used_hw_stats</code>
</li>
<li>
<b>Field added. </b>
<code>bool used_hw_stats_valid</code>
</li>
<li>
<b>Field removed. </b>
<code>__u32 order</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 in_hw_count</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct gnet_stats_basic_packed tcfa_bstats</code> ➡️ <code>struct gnet_stats_basic_sync tcfa_bstats</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct gnet_stats_basic_packed tcfa_bstats_hw</code> ➡️ <code>struct gnet_stats_basic_sync tcfa_bstats_hw</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct gnet_stats_basic_cpu *cpu_bstats</code> ➡️ <code>struct gnet_stats_basic_sync *cpu_bstats</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct gnet_stats_basic_cpu *cpu_bstats_hw</code> ➡️ <code>struct gnet_stats_basic_sync *cpu_bstats_hw</code>
</li>
</ul>
</details>
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
<code>struct tc_cookie *user_cookie</code>
</li>
<li>
<b>Field removed. </b>
<code>struct tc_cookie *act_cookie</code>
</li>
</ul>
</details>
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
