# Struct: <code>fib_info</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct fib_info {
    struct hlist_node fib_hash;
    struct hlist_node fib_lhash;
    struct net *fib_net;
    int fib_treeref;
    atomic_t fib_clntref;
    unsigned int fib_flags;
    unsigned char fib_dead;
    unsigned char fib_protocol;
    unsigned char fib_scope;
    unsigned char fib_type;
    __be32 fib_prefsrc;
    u32 fib_priority;
    u32 *fib_metrics;
    int fib_nhs;
    int fib_weight;
    struct callback_head rcu;
    struct fib_nh fib_nh[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct fib_info {
    struct hlist_node fib_hash;
    struct hlist_node fib_lhash;
    struct net *fib_net;
    int fib_treeref;
    atomic_t fib_clntref;
    unsigned int fib_flags;
    unsigned char fib_dead;
    unsigned char fib_protocol;
    unsigned char fib_scope;
    unsigned char fib_type;
    __be32 fib_prefsrc;
    u32 fib_tb_id;
    u32 fib_priority;
    u32 *fib_metrics;
    int fib_nhs;
    int fib_weight;
    struct callback_head rcu;
    struct fib_nh fib_nh[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct fib_info {
    struct hlist_node fib_hash;
    struct hlist_node fib_lhash;
    struct net *fib_net;
    int fib_treeref;
    atomic_t fib_clntref;
    unsigned int fib_flags;
    unsigned char fib_dead;
    unsigned char fib_protocol;
    unsigned char fib_scope;
    unsigned char fib_type;
    __be32 fib_prefsrc;
    u32 fib_tb_id;
    u32 fib_priority;
    u32 *fib_metrics;
    int fib_nhs;
    int fib_weight;
    unsigned int fib_offload_cnt;
    struct callback_head rcu;
    struct fib_nh fib_nh[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct fib_info {
    struct hlist_node fib_hash;
    struct hlist_node fib_lhash;
    struct net *fib_net;
    int fib_treeref;
    refcount_t fib_clntref;
    unsigned int fib_flags;
    unsigned char fib_dead;
    unsigned char fib_protocol;
    unsigned char fib_scope;
    unsigned char fib_type;
    __be32 fib_prefsrc;
    u32 fib_tb_id;
    u32 fib_priority;
    struct dst_metrics *fib_metrics;
    int fib_nhs;
    int fib_weight;
    unsigned int fib_offload_cnt;
    struct callback_head rcu;
    struct fib_nh fib_nh[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct fib_info {
    struct hlist_node fib_hash;
    struct hlist_node fib_lhash;
    struct net *fib_net;
    int fib_treeref;
    refcount_t fib_clntref;
    unsigned int fib_flags;
    unsigned char fib_dead;
    unsigned char fib_protocol;
    unsigned char fib_scope;
    unsigned char fib_type;
    __be32 fib_prefsrc;
    u32 fib_tb_id;
    u32 fib_priority;
    struct dst_metrics *fib_metrics;
    int fib_nhs;
    struct callback_head rcu;
    struct fib_nh fib_nh[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct fib_info {
    struct hlist_node fib_hash;
    struct hlist_node fib_lhash;
    struct net *fib_net;
    int fib_treeref;
    refcount_t fib_clntref;
    unsigned int fib_flags;
    unsigned char fib_dead;
    unsigned char fib_protocol;
    unsigned char fib_scope;
    unsigned char fib_type;
    __be32 fib_prefsrc;
    u32 fib_tb_id;
    u32 fib_priority;
    struct dst_metrics *fib_metrics;
    int fib_nhs;
    struct callback_head rcu;
    struct fib_nh fib_nh[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct fib_info {
    struct hlist_node fib_hash;
    struct hlist_node fib_lhash;
    struct net *fib_net;
    int fib_treeref;
    refcount_t fib_clntref;
    unsigned int fib_flags;
    unsigned char fib_dead;
    unsigned char fib_protocol;
    unsigned char fib_scope;
    unsigned char fib_type;
    __be32 fib_prefsrc;
    u32 fib_tb_id;
    u32 fib_priority;
    struct dst_metrics *fib_metrics;
    int fib_nhs;
    struct callback_head rcu;
    struct fib_nh fib_nh[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct fib_info {
    struct hlist_node fib_hash;
    struct hlist_node fib_lhash;
    struct list_head nh_list;
    struct net *fib_net;
    int fib_treeref;
    refcount_t fib_clntref;
    unsigned int fib_flags;
    unsigned char fib_dead;
    unsigned char fib_protocol;
    unsigned char fib_scope;
    unsigned char fib_type;
    __be32 fib_prefsrc;
    u32 fib_tb_id;
    u32 fib_priority;
    struct dst_metrics *fib_metrics;
    int fib_nhs;
    bool fib_nh_is_v6;
    bool nh_updated;
    struct nexthop *nh;
    struct callback_head rcu;
    struct fib_nh fib_nh[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct fib_info {
    struct hlist_node fib_hash;
    struct hlist_node fib_lhash;
    struct list_head nh_list;
    struct net *fib_net;
    int fib_treeref;
    refcount_t fib_clntref;
    unsigned int fib_flags;
    unsigned char fib_dead;
    unsigned char fib_protocol;
    unsigned char fib_scope;
    unsigned char fib_type;
    __be32 fib_prefsrc;
    u32 fib_tb_id;
    u32 fib_priority;
    struct dst_metrics *fib_metrics;
    int fib_nhs;
    bool fib_nh_is_v6;
    bool nh_updated;
    struct nexthop *nh;
    struct callback_head rcu;
    struct fib_nh fib_nh[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct fib_info {
    struct hlist_node fib_hash;
    struct hlist_node fib_lhash;
    struct list_head nh_list;
    struct net *fib_net;
    int fib_treeref;
    refcount_t fib_clntref;
    unsigned int fib_flags;
    unsigned char fib_dead;
    unsigned char fib_protocol;
    unsigned char fib_scope;
    unsigned char fib_type;
    __be32 fib_prefsrc;
    u32 fib_tb_id;
    u32 fib_priority;
    struct dst_metrics *fib_metrics;
    int fib_nhs;
    bool fib_nh_is_v6;
    bool nh_updated;
    struct nexthop *nh;
    struct callback_head rcu;
    struct fib_nh fib_nh[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct fib_info {
    struct hlist_node fib_hash;
    struct hlist_node fib_lhash;
    struct list_head nh_list;
    struct net *fib_net;
    int fib_treeref;
    refcount_t fib_clntref;
    unsigned int fib_flags;
    unsigned char fib_dead;
    unsigned char fib_protocol;
    unsigned char fib_scope;
    unsigned char fib_type;
    __be32 fib_prefsrc;
    u32 fib_tb_id;
    u32 fib_priority;
    struct dst_metrics *fib_metrics;
    int fib_nhs;
    bool fib_nh_is_v6;
    bool nh_updated;
    struct nexthop *nh;
    struct callback_head rcu;
    struct fib_nh fib_nh[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct fib_info {
    struct hlist_node fib_hash;
    struct hlist_node fib_lhash;
    struct list_head nh_list;
    struct net *fib_net;
    int fib_treeref;
    refcount_t fib_clntref;
    unsigned int fib_flags;
    unsigned char fib_dead;
    unsigned char fib_protocol;
    unsigned char fib_scope;
    unsigned char fib_type;
    __be32 fib_prefsrc;
    u32 fib_tb_id;
    u32 fib_priority;
    struct dst_metrics *fib_metrics;
    int fib_nhs;
    bool fib_nh_is_v6;
    bool nh_updated;
    struct nexthop *nh;
    struct callback_head rcu;
    struct fib_nh fib_nh[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct fib_info {
    struct hlist_node fib_hash;
    struct hlist_node fib_lhash;
    struct list_head nh_list;
    struct net *fib_net;
    refcount_t fib_treeref;
    refcount_t fib_clntref;
    unsigned int fib_flags;
    unsigned char fib_dead;
    unsigned char fib_protocol;
    unsigned char fib_scope;
    unsigned char fib_type;
    __be32 fib_prefsrc;
    u32 fib_tb_id;
    u32 fib_priority;
    struct dst_metrics *fib_metrics;
    int fib_nhs;
    bool fib_nh_is_v6;
    bool nh_updated;
    struct nexthop *nh;
    struct callback_head rcu;
    struct fib_nh fib_nh[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct fib_info {
    struct hlist_node fib_hash;
    struct hlist_node fib_lhash;
    struct list_head nh_list;
    struct net *fib_net;
    refcount_t fib_treeref;
    refcount_t fib_clntref;
    unsigned int fib_flags;
    unsigned char fib_dead;
    unsigned char fib_protocol;
    unsigned char fib_scope;
    unsigned char fib_type;
    __be32 fib_prefsrc;
    u32 fib_tb_id;
    u32 fib_priority;
    struct dst_metrics *fib_metrics;
    int fib_nhs;
    bool fib_nh_is_v6;
    bool nh_updated;
    struct nexthop *nh;
    struct callback_head rcu;
    struct fib_nh fib_nh[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct fib_info {
    struct hlist_node fib_hash;
    struct hlist_node fib_lhash;
    struct list_head nh_list;
    struct net *fib_net;
    refcount_t fib_treeref;
    refcount_t fib_clntref;
    unsigned int fib_flags;
    unsigned char fib_dead;
    unsigned char fib_protocol;
    unsigned char fib_scope;
    unsigned char fib_type;
    __be32 fib_prefsrc;
    u32 fib_tb_id;
    u32 fib_priority;
    struct dst_metrics *fib_metrics;
    int fib_nhs;
    bool fib_nh_is_v6;
    bool nh_updated;
    struct nexthop *nh;
    struct callback_head rcu;
    struct fib_nh fib_nh[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct fib_info {
    struct hlist_node fib_hash;
    struct hlist_node fib_lhash;
    struct list_head nh_list;
    struct net *fib_net;
    refcount_t fib_treeref;
    refcount_t fib_clntref;
    unsigned int fib_flags;
    unsigned char fib_dead;
    unsigned char fib_protocol;
    unsigned char fib_scope;
    unsigned char fib_type;
    __be32 fib_prefsrc;
    u32 fib_tb_id;
    u32 fib_priority;
    struct dst_metrics *fib_metrics;
    int fib_nhs;
    bool fib_nh_is_v6;
    bool nh_updated;
    struct nexthop *nh;
    struct callback_head rcu;
    struct fib_nh fib_nh[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct fib_info {
    struct hlist_node fib_hash;
    struct hlist_node fib_lhash;
    struct list_head nh_list;
    struct net *fib_net;
    refcount_t fib_treeref;
    refcount_t fib_clntref;
    unsigned int fib_flags;
    unsigned char fib_dead;
    unsigned char fib_protocol;
    unsigned char fib_scope;
    unsigned char fib_type;
    __be32 fib_prefsrc;
    u32 fib_tb_id;
    u32 fib_priority;
    struct dst_metrics *fib_metrics;
    int fib_nhs;
    bool fib_nh_is_v6;
    bool nh_updated;
    bool pfsrc_removed;
    struct nexthop *nh;
    struct callback_head rcu;
    struct fib_nh fib_nh[0];
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
struct fib_info {
    struct hlist_node fib_hash;
    struct hlist_node fib_lhash;
    struct list_head nh_list;
    struct net *fib_net;
    int fib_treeref;
    refcount_t fib_clntref;
    unsigned int fib_flags;
    unsigned char fib_dead;
    unsigned char fib_protocol;
    unsigned char fib_scope;
    unsigned char fib_type;
    __be32 fib_prefsrc;
    u32 fib_tb_id;
    u32 fib_priority;
    struct dst_metrics *fib_metrics;
    int fib_nhs;
    bool fib_nh_is_v6;
    bool nh_updated;
    struct nexthop *nh;
    struct callback_head rcu;
    struct fib_nh fib_nh[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct fib_info {
    struct hlist_node fib_hash;
    struct hlist_node fib_lhash;
    struct list_head nh_list;
    struct net *fib_net;
    int fib_treeref;
    refcount_t fib_clntref;
    unsigned int fib_flags;
    unsigned char fib_dead;
    unsigned char fib_protocol;
    unsigned char fib_scope;
    unsigned char fib_type;
    __be32 fib_prefsrc;
    u32 fib_tb_id;
    u32 fib_priority;
    struct dst_metrics *fib_metrics;
    int fib_nhs;
    bool fib_nh_is_v6;
    bool nh_updated;
    struct nexthop *nh;
    struct callback_head rcu;
    struct fib_nh fib_nh[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct fib_info {
    struct hlist_node fib_hash;
    struct hlist_node fib_lhash;
    struct list_head nh_list;
    struct net *fib_net;
    int fib_treeref;
    refcount_t fib_clntref;
    unsigned int fib_flags;
    unsigned char fib_dead;
    unsigned char fib_protocol;
    unsigned char fib_scope;
    unsigned char fib_type;
    __be32 fib_prefsrc;
    u32 fib_tb_id;
    u32 fib_priority;
    struct dst_metrics *fib_metrics;
    int fib_nhs;
    bool fib_nh_is_v6;
    bool nh_updated;
    struct nexthop *nh;
    struct callback_head rcu;
    struct fib_nh fib_nh[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct fib_info {
    struct hlist_node fib_hash;
    struct hlist_node fib_lhash;
    struct list_head nh_list;
    struct net *fib_net;
    int fib_treeref;
    refcount_t fib_clntref;
    unsigned int fib_flags;
    unsigned char fib_dead;
    unsigned char fib_protocol;
    unsigned char fib_scope;
    unsigned char fib_type;
    __be32 fib_prefsrc;
    u32 fib_tb_id;
    u32 fib_priority;
    struct dst_metrics *fib_metrics;
    int fib_nhs;
    bool fib_nh_is_v6;
    bool nh_updated;
    struct nexthop *nh;
    struct callback_head rcu;
    struct fib_nh fib_nh[0];
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
struct fib_info {
    struct hlist_node fib_hash;
    struct hlist_node fib_lhash;
    struct list_head nh_list;
    struct net *fib_net;
    int fib_treeref;
    refcount_t fib_clntref;
    unsigned int fib_flags;
    unsigned char fib_dead;
    unsigned char fib_protocol;
    unsigned char fib_scope;
    unsigned char fib_type;
    __be32 fib_prefsrc;
    u32 fib_tb_id;
    u32 fib_priority;
    struct dst_metrics *fib_metrics;
    int fib_nhs;
    bool fib_nh_is_v6;
    bool nh_updated;
    struct nexthop *nh;
    struct callback_head rcu;
    struct fib_nh fib_nh[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct fib_info {
    struct hlist_node fib_hash;
    struct hlist_node fib_lhash;
    struct list_head nh_list;
    struct net *fib_net;
    int fib_treeref;
    refcount_t fib_clntref;
    unsigned int fib_flags;
    unsigned char fib_dead;
    unsigned char fib_protocol;
    unsigned char fib_scope;
    unsigned char fib_type;
    __be32 fib_prefsrc;
    u32 fib_tb_id;
    u32 fib_priority;
    struct dst_metrics *fib_metrics;
    int fib_nhs;
    bool fib_nh_is_v6;
    bool nh_updated;
    struct nexthop *nh;
    struct callback_head rcu;
    struct fib_nh fib_nh[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct fib_info {
    struct hlist_node fib_hash;
    struct hlist_node fib_lhash;
    struct list_head nh_list;
    struct net *fib_net;
    int fib_treeref;
    refcount_t fib_clntref;
    unsigned int fib_flags;
    unsigned char fib_dead;
    unsigned char fib_protocol;
    unsigned char fib_scope;
    unsigned char fib_type;
    __be32 fib_prefsrc;
    u32 fib_tb_id;
    u32 fib_priority;
    struct dst_metrics *fib_metrics;
    int fib_nhs;
    bool fib_nh_is_v6;
    bool nh_updated;
    struct nexthop *nh;
    struct callback_head rcu;
    struct fib_nh fib_nh[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct fib_info {
    struct hlist_node fib_hash;
    struct hlist_node fib_lhash;
    struct list_head nh_list;
    struct net *fib_net;
    int fib_treeref;
    refcount_t fib_clntref;
    unsigned int fib_flags;
    unsigned char fib_dead;
    unsigned char fib_protocol;
    unsigned char fib_scope;
    unsigned char fib_type;
    __be32 fib_prefsrc;
    u32 fib_tb_id;
    u32 fib_priority;
    struct dst_metrics *fib_metrics;
    int fib_nhs;
    bool fib_nh_is_v6;
    bool nh_updated;
    struct nexthop *nh;
    struct callback_head rcu;
    struct fib_nh fib_nh[0];
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
<code>u32 fib_tb_id</code>
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
<code>unsigned int fib_offload_cnt</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>atomic_t fib_clntref</code> ➡️ <code>refcount_t fib_clntref</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 *fib_metrics</code> ➡️ <code>struct dst_metrics *fib_metrics</code>
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
<code>int fib_weight</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int fib_offload_cnt</code>
</li>
</ul>
</details>
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
<code>struct list_head nh_list</code>
</li>
<li>
<b>Field added. </b>
<code>bool fib_nh_is_v6</code>
</li>
<li>
<b>Field added. </b>
<code>bool nh_updated</code>
</li>
<li>
<b>Field added. </b>
<code>struct nexthop *nh</code>
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
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int fib_treeref</code> ➡️ <code>refcount_t fib_treeref</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool pfsrc_removed</code>
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
