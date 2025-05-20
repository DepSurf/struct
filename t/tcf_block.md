# Struct: <code>tcf_block</code>

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
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct tcf_block {
    struct list_head chain_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct tcf_block {
    struct list_head chain_list;
    struct net *net;
    struct Qdisc *q;
    struct list_head cb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct tcf_block {
    struct list_head chain_list;
    u32 index;
    unsigned int refcnt;
    struct net *net;
    struct Qdisc *q;
    struct list_head cb_list;
    struct list_head owner_list;
    bool keep_dst;
    unsigned int offloadcnt;
    unsigned int nooffloaddevcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct tcf_block {
    struct list_head chain_list;
    u32 index;
    refcount_t refcnt;
    struct net *net;
    struct Qdisc *q;
    struct list_head cb_list;
    struct list_head owner_list;
    bool keep_dst;
    unsigned int offloadcnt;
    unsigned int nooffloaddevcnt;
    struct (anon) chain0;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct tcf_block {
    struct mutex lock;
    struct list_head chain_list;
    u32 index;
    refcount_t refcnt;
    struct net *net;
    struct Qdisc *q;
    struct flow_block flow_block;
    struct list_head owner_list;
    bool keep_dst;
    unsigned int offloadcnt;
    unsigned int nooffloaddevcnt;
    struct (anon) chain0;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct tcf_block {
    struct mutex lock;
    struct list_head chain_list;
    u32 index;
    refcount_t refcnt;
    struct net *net;
    struct Qdisc *q;
    struct rw_semaphore cb_lock;
    struct flow_block flow_block;
    struct list_head owner_list;
    bool keep_dst;
    atomic_t offloadcnt;
    unsigned int nooffloaddevcnt;
    unsigned int lockeddevcnt;
    struct (anon) chain0;
    struct callback_head rcu;
    struct hlist_head proto_destroy_ht[128];
    struct mutex proto_destroy_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct tcf_block {
    struct mutex lock;
    struct list_head chain_list;
    u32 index;
    u32 classid;
    refcount_t refcnt;
    struct net *net;
    struct Qdisc *q;
    struct rw_semaphore cb_lock;
    struct flow_block flow_block;
    struct list_head owner_list;
    bool keep_dst;
    atomic_t offloadcnt;
    unsigned int nooffloaddevcnt;
    unsigned int lockeddevcnt;
    struct (anon) chain0;
    struct callback_head rcu;
    struct hlist_head proto_destroy_ht[128];
    struct mutex proto_destroy_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct tcf_block {
    struct mutex lock;
    struct list_head chain_list;
    u32 index;
    u32 classid;
    refcount_t refcnt;
    struct net *net;
    struct Qdisc *q;
    struct rw_semaphore cb_lock;
    struct flow_block flow_block;
    struct list_head owner_list;
    bool keep_dst;
    atomic_t offloadcnt;
    unsigned int nooffloaddevcnt;
    unsigned int lockeddevcnt;
    struct (anon) chain0;
    struct callback_head rcu;
    struct hlist_head proto_destroy_ht[128];
    struct mutex proto_destroy_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct tcf_block {
    struct mutex lock;
    struct list_head chain_list;
    u32 index;
    u32 classid;
    refcount_t refcnt;
    struct net *net;
    struct Qdisc *q;
    struct rw_semaphore cb_lock;
    struct flow_block flow_block;
    struct list_head owner_list;
    bool keep_dst;
    atomic_t offloadcnt;
    unsigned int nooffloaddevcnt;
    unsigned int lockeddevcnt;
    struct (anon) chain0;
    struct callback_head rcu;
    struct hlist_head proto_destroy_ht[128];
    struct mutex proto_destroy_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct tcf_block {
    struct mutex lock;
    struct list_head chain_list;
    u32 index;
    u32 classid;
    refcount_t refcnt;
    struct net *net;
    struct Qdisc *q;
    struct rw_semaphore cb_lock;
    struct flow_block flow_block;
    struct list_head owner_list;
    bool keep_dst;
    atomic_t offloadcnt;
    unsigned int nooffloaddevcnt;
    unsigned int lockeddevcnt;
    struct (anon) chain0;
    struct callback_head rcu;
    struct hlist_head proto_destroy_ht[128];
    struct mutex proto_destroy_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct tcf_block {
    struct mutex lock;
    struct list_head chain_list;
    u32 index;
    u32 classid;
    refcount_t refcnt;
    struct net *net;
    struct Qdisc *q;
    struct rw_semaphore cb_lock;
    struct flow_block flow_block;
    struct list_head owner_list;
    bool keep_dst;
    atomic_t offloadcnt;
    unsigned int nooffloaddevcnt;
    unsigned int lockeddevcnt;
    struct (anon) chain0;
    struct callback_head rcu;
    struct hlist_head proto_destroy_ht[128];
    struct mutex proto_destroy_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct tcf_block {
    struct mutex lock;
    struct list_head chain_list;
    u32 index;
    u32 classid;
    refcount_t refcnt;
    struct net *net;
    struct Qdisc *q;
    struct rw_semaphore cb_lock;
    struct flow_block flow_block;
    struct list_head owner_list;
    bool keep_dst;
    atomic_t offloadcnt;
    unsigned int nooffloaddevcnt;
    unsigned int lockeddevcnt;
    struct (anon) chain0;
    struct callback_head rcu;
    struct hlist_head proto_destroy_ht[128];
    struct mutex proto_destroy_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct tcf_block {
    struct mutex lock;
    struct list_head chain_list;
    u32 index;
    u32 classid;
    refcount_t refcnt;
    struct net *net;
    struct Qdisc *q;
    struct rw_semaphore cb_lock;
    struct flow_block flow_block;
    struct list_head owner_list;
    bool keep_dst;
    atomic_t offloadcnt;
    unsigned int nooffloaddevcnt;
    unsigned int lockeddevcnt;
    struct (anon) chain0;
    struct callback_head rcu;
    struct hlist_head proto_destroy_ht[128];
    struct mutex proto_destroy_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct tcf_block {
    struct xarray ports;
    struct mutex lock;
    struct list_head chain_list;
    u32 index;
    u32 classid;
    refcount_t refcnt;
    struct net *net;
    struct Qdisc *q;
    struct rw_semaphore cb_lock;
    struct flow_block flow_block;
    struct list_head owner_list;
    bool keep_dst;
    atomic_t offloadcnt;
    unsigned int nooffloaddevcnt;
    unsigned int lockeddevcnt;
    struct (anon) chain0;
    struct callback_head rcu;
    struct hlist_head proto_destroy_ht[128];
    struct mutex proto_destroy_lock;
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
struct tcf_block {
    struct mutex lock;
    struct list_head chain_list;
    u32 index;
    refcount_t refcnt;
    struct net *net;
    struct Qdisc *q;
    struct rw_semaphore cb_lock;
    struct flow_block flow_block;
    struct list_head owner_list;
    bool keep_dst;
    atomic_t offloadcnt;
    unsigned int nooffloaddevcnt;
    unsigned int lockeddevcnt;
    struct (anon) chain0;
    struct callback_head rcu;
    struct hlist_head proto_destroy_ht[128];
    struct mutex proto_destroy_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct tcf_block {
    struct mutex lock;
    struct list_head chain_list;
    u32 index;
    refcount_t refcnt;
    struct net *net;
    struct Qdisc *q;
    struct rw_semaphore cb_lock;
    struct flow_block flow_block;
    struct list_head owner_list;
    bool keep_dst;
    atomic_t offloadcnt;
    unsigned int nooffloaddevcnt;
    unsigned int lockeddevcnt;
    struct (anon) chain0;
    struct callback_head rcu;
    struct hlist_head proto_destroy_ht[128];
    struct mutex proto_destroy_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct tcf_block {
    struct mutex lock;
    struct list_head chain_list;
    u32 index;
    refcount_t refcnt;
    struct net *net;
    struct Qdisc *q;
    struct rw_semaphore cb_lock;
    struct flow_block flow_block;
    struct list_head owner_list;
    bool keep_dst;
    atomic_t offloadcnt;
    unsigned int nooffloaddevcnt;
    unsigned int lockeddevcnt;
    struct (anon) chain0;
    struct callback_head rcu;
    struct hlist_head proto_destroy_ht[128];
    struct mutex proto_destroy_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct tcf_block {
    struct mutex lock;
    struct list_head chain_list;
    u32 index;
    refcount_t refcnt;
    struct net *net;
    struct Qdisc *q;
    struct rw_semaphore cb_lock;
    struct flow_block flow_block;
    struct list_head owner_list;
    bool keep_dst;
    atomic_t offloadcnt;
    unsigned int nooffloaddevcnt;
    unsigned int lockeddevcnt;
    struct (anon) chain0;
    struct callback_head rcu;
    struct hlist_head proto_destroy_ht[128];
    struct mutex proto_destroy_lock;
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
struct tcf_block {
    struct mutex lock;
    struct list_head chain_list;
    u32 index;
    refcount_t refcnt;
    struct net *net;
    struct Qdisc *q;
    struct rw_semaphore cb_lock;
    struct flow_block flow_block;
    struct list_head owner_list;
    bool keep_dst;
    atomic_t offloadcnt;
    unsigned int nooffloaddevcnt;
    unsigned int lockeddevcnt;
    struct (anon) chain0;
    struct callback_head rcu;
    struct hlist_head proto_destroy_ht[128];
    struct mutex proto_destroy_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct tcf_block {
    struct mutex lock;
    struct list_head chain_list;
    u32 index;
    refcount_t refcnt;
    struct net *net;
    struct Qdisc *q;
    struct rw_semaphore cb_lock;
    struct flow_block flow_block;
    struct list_head owner_list;
    bool keep_dst;
    atomic_t offloadcnt;
    unsigned int nooffloaddevcnt;
    unsigned int lockeddevcnt;
    struct (anon) chain0;
    struct callback_head rcu;
    struct hlist_head proto_destroy_ht[128];
    struct mutex proto_destroy_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct tcf_block {
    struct mutex lock;
    struct list_head chain_list;
    u32 index;
    refcount_t refcnt;
    struct net *net;
    struct Qdisc *q;
    struct rw_semaphore cb_lock;
    struct flow_block flow_block;
    struct list_head owner_list;
    bool keep_dst;
    atomic_t offloadcnt;
    unsigned int nooffloaddevcnt;
    unsigned int lockeddevcnt;
    struct (anon) chain0;
    struct callback_head rcu;
    struct hlist_head proto_destroy_ht[128];
    struct mutex proto_destroy_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct tcf_block {
    struct mutex lock;
    struct list_head chain_list;
    u32 index;
    refcount_t refcnt;
    struct net *net;
    struct Qdisc *q;
    struct rw_semaphore cb_lock;
    struct flow_block flow_block;
    struct list_head owner_list;
    bool keep_dst;
    atomic_t offloadcnt;
    unsigned int nooffloaddevcnt;
    unsigned int lockeddevcnt;
    struct (anon) chain0;
    struct callback_head rcu;
    struct hlist_head proto_destroy_ht[128];
    struct mutex proto_destroy_lock;
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
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct net *net</code>
</li>
<li>
<b>Field added. </b>
<code>struct Qdisc *q</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head cb_list</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 index</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int refcnt</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head owner_list</code>
</li>
<li>
<b>Field added. </b>
<code>bool keep_dst</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int offloadcnt</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int nooffloaddevcnt</code>
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
<code>struct (anon) chain0</code>
</li>
<li>
<b>Field added. </b>
<code>struct callback_head rcu</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int refcnt</code> ➡️ <code>refcount_t refcnt</code>
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
<code>struct mutex lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct flow_block flow_block</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head cb_list</code>
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
<code>struct rw_semaphore cb_lock</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int lockeddevcnt</code>
</li>
<li>
<b>Field added. </b>
<code>struct hlist_head proto_destroy_ht[128]</code>
</li>
<li>
<b>Field added. </b>
<code>struct mutex proto_destroy_lock</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int offloadcnt</code> ➡️ <code>atomic_t offloadcnt</code>
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
<code>u32 classid</code>
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
<b>Field added. </b>
<code>struct xarray ports</code>
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
