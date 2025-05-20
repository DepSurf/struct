# Struct: <code>inet6_ifaddr</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct inet6_ifaddr {
    struct in6_addr addr;
    __u32 prefix_len;
    __u32 valid_lft;
    __u32 prefered_lft;
    atomic_t refcnt;
    spinlock_t lock;
    int state;
    __u32 flags;
    __u8 dad_probes;
    __u8 stable_privacy_retry;
    __u16 scope;
    long unsigned int cstamp;
    long unsigned int tstamp;
    struct delayed_work dad_work;
    struct inet6_dev *idev;
    struct rt6_info *rt;
    struct hlist_node addr_lst;
    struct list_head if_list;
    struct list_head tmp_list;
    struct inet6_ifaddr *ifpub;
    int regen_count;
    bool tokenized;
    struct callback_head rcu;
    struct in6_addr peer_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct inet6_ifaddr {
    struct in6_addr addr;
    __u32 prefix_len;
    __u32 valid_lft;
    __u32 prefered_lft;
    atomic_t refcnt;
    spinlock_t lock;
    int state;
    __u32 flags;
    __u8 dad_probes;
    __u8 stable_privacy_retry;
    __u16 scope;
    long unsigned int cstamp;
    long unsigned int tstamp;
    struct delayed_work dad_work;
    struct inet6_dev *idev;
    struct rt6_info *rt;
    struct hlist_node addr_lst;
    struct list_head if_list;
    struct list_head tmp_list;
    struct inet6_ifaddr *ifpub;
    int regen_count;
    bool tokenized;
    struct callback_head rcu;
    struct in6_addr peer_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct inet6_ifaddr {
    struct in6_addr addr;
    __u32 prefix_len;
    __u32 valid_lft;
    __u32 prefered_lft;
    atomic_t refcnt;
    spinlock_t lock;
    int state;
    __u32 flags;
    __u8 dad_probes;
    __u8 stable_privacy_retry;
    __u16 scope;
    __u64 dad_nonce;
    long unsigned int cstamp;
    long unsigned int tstamp;
    struct delayed_work dad_work;
    struct inet6_dev *idev;
    struct rt6_info *rt;
    struct hlist_node addr_lst;
    struct list_head if_list;
    struct list_head tmp_list;
    struct inet6_ifaddr *ifpub;
    int regen_count;
    bool tokenized;
    struct callback_head rcu;
    struct in6_addr peer_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct inet6_ifaddr {
    struct in6_addr addr;
    __u32 prefix_len;
    __u32 valid_lft;
    __u32 prefered_lft;
    refcount_t refcnt;
    spinlock_t lock;
    int state;
    __u32 flags;
    __u8 dad_probes;
    __u8 stable_privacy_retry;
    __u16 scope;
    __u64 dad_nonce;
    long unsigned int cstamp;
    long unsigned int tstamp;
    struct delayed_work dad_work;
    struct inet6_dev *idev;
    struct rt6_info *rt;
    struct hlist_node addr_lst;
    struct list_head if_list;
    struct list_head tmp_list;
    struct inet6_ifaddr *ifpub;
    int regen_count;
    bool tokenized;
    struct callback_head rcu;
    struct in6_addr peer_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct inet6_ifaddr {
    struct in6_addr addr;
    __u32 prefix_len;
    __u32 valid_lft;
    __u32 prefered_lft;
    refcount_t refcnt;
    spinlock_t lock;
    int state;
    __u32 flags;
    __u8 dad_probes;
    __u8 stable_privacy_retry;
    __u16 scope;
    __u64 dad_nonce;
    long unsigned int cstamp;
    long unsigned int tstamp;
    struct delayed_work dad_work;
    struct inet6_dev *idev;
    struct rt6_info *rt;
    struct hlist_node addr_lst;
    struct list_head if_list;
    struct list_head tmp_list;
    struct inet6_ifaddr *ifpub;
    int regen_count;
    bool tokenized;
    struct callback_head rcu;
    struct in6_addr peer_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct inet6_ifaddr {
    struct in6_addr addr;
    __u32 prefix_len;
    __u32 rt_priority;
    __u32 valid_lft;
    __u32 prefered_lft;
    refcount_t refcnt;
    spinlock_t lock;
    int state;
    __u32 flags;
    __u8 dad_probes;
    __u8 stable_privacy_retry;
    __u16 scope;
    __u64 dad_nonce;
    long unsigned int cstamp;
    long unsigned int tstamp;
    struct delayed_work dad_work;
    struct inet6_dev *idev;
    struct fib6_info *rt;
    struct hlist_node addr_lst;
    struct list_head if_list;
    struct list_head tmp_list;
    struct inet6_ifaddr *ifpub;
    int regen_count;
    bool tokenized;
    struct callback_head rcu;
    struct in6_addr peer_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct inet6_ifaddr {
    struct in6_addr addr;
    __u32 prefix_len;
    __u32 rt_priority;
    __u32 valid_lft;
    __u32 prefered_lft;
    refcount_t refcnt;
    spinlock_t lock;
    int state;
    __u32 flags;
    __u8 dad_probes;
    __u8 stable_privacy_retry;
    __u16 scope;
    __u64 dad_nonce;
    long unsigned int cstamp;
    long unsigned int tstamp;
    struct delayed_work dad_work;
    struct inet6_dev *idev;
    struct fib6_info *rt;
    struct hlist_node addr_lst;
    struct list_head if_list;
    struct list_head tmp_list;
    struct inet6_ifaddr *ifpub;
    int regen_count;
    bool tokenized;
    struct callback_head rcu;
    struct in6_addr peer_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct inet6_ifaddr {
    struct in6_addr addr;
    __u32 prefix_len;
    __u32 rt_priority;
    __u32 valid_lft;
    __u32 prefered_lft;
    refcount_t refcnt;
    spinlock_t lock;
    int state;
    __u32 flags;
    __u8 dad_probes;
    __u8 stable_privacy_retry;
    __u16 scope;
    __u64 dad_nonce;
    long unsigned int cstamp;
    long unsigned int tstamp;
    struct delayed_work dad_work;
    struct inet6_dev *idev;
    struct fib6_info *rt;
    struct hlist_node addr_lst;
    struct list_head if_list;
    struct list_head tmp_list;
    struct inet6_ifaddr *ifpub;
    int regen_count;
    bool tokenized;
    struct callback_head rcu;
    struct in6_addr peer_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct inet6_ifaddr {
    struct in6_addr addr;
    __u32 prefix_len;
    __u32 rt_priority;
    __u32 valid_lft;
    __u32 prefered_lft;
    refcount_t refcnt;
    spinlock_t lock;
    int state;
    __u32 flags;
    __u8 dad_probes;
    __u8 stable_privacy_retry;
    __u16 scope;
    __u64 dad_nonce;
    long unsigned int cstamp;
    long unsigned int tstamp;
    struct delayed_work dad_work;
    struct inet6_dev *idev;
    struct fib6_info *rt;
    struct hlist_node addr_lst;
    struct list_head if_list;
    struct list_head tmp_list;
    struct inet6_ifaddr *ifpub;
    int regen_count;
    bool tokenized;
    struct callback_head rcu;
    struct in6_addr peer_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct inet6_ifaddr {
    struct in6_addr addr;
    __u32 prefix_len;
    __u32 rt_priority;
    __u32 valid_lft;
    __u32 prefered_lft;
    refcount_t refcnt;
    spinlock_t lock;
    int state;
    __u32 flags;
    __u8 dad_probes;
    __u8 stable_privacy_retry;
    __u16 scope;
    __u64 dad_nonce;
    long unsigned int cstamp;
    long unsigned int tstamp;
    struct delayed_work dad_work;
    struct inet6_dev *idev;
    struct fib6_info *rt;
    struct hlist_node addr_lst;
    struct list_head if_list;
    struct list_head tmp_list;
    struct inet6_ifaddr *ifpub;
    int regen_count;
    bool tokenized;
    struct callback_head rcu;
    struct in6_addr peer_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct inet6_ifaddr {
    struct in6_addr addr;
    __u32 prefix_len;
    __u32 rt_priority;
    __u32 valid_lft;
    __u32 prefered_lft;
    refcount_t refcnt;
    spinlock_t lock;
    int state;
    __u32 flags;
    __u8 dad_probes;
    __u8 stable_privacy_retry;
    __u16 scope;
    __u64 dad_nonce;
    long unsigned int cstamp;
    long unsigned int tstamp;
    struct delayed_work dad_work;
    struct inet6_dev *idev;
    struct fib6_info *rt;
    struct hlist_node addr_lst;
    struct list_head if_list;
    struct list_head tmp_list;
    struct inet6_ifaddr *ifpub;
    int regen_count;
    bool tokenized;
    struct callback_head rcu;
    struct in6_addr peer_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct inet6_ifaddr {
    struct in6_addr addr;
    __u32 prefix_len;
    __u32 rt_priority;
    __u32 valid_lft;
    __u32 prefered_lft;
    refcount_t refcnt;
    spinlock_t lock;
    int state;
    __u32 flags;
    __u8 dad_probes;
    __u8 stable_privacy_retry;
    __u16 scope;
    __u64 dad_nonce;
    long unsigned int cstamp;
    long unsigned int tstamp;
    struct delayed_work dad_work;
    struct inet6_dev *idev;
    struct fib6_info *rt;
    struct hlist_node addr_lst;
    struct list_head if_list;
    struct list_head tmp_list;
    struct inet6_ifaddr *ifpub;
    int regen_count;
    bool tokenized;
    struct callback_head rcu;
    struct in6_addr peer_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct inet6_ifaddr {
    struct in6_addr addr;
    __u32 prefix_len;
    __u32 rt_priority;
    __u32 valid_lft;
    __u32 prefered_lft;
    refcount_t refcnt;
    spinlock_t lock;
    int state;
    __u32 flags;
    __u8 dad_probes;
    __u8 stable_privacy_retry;
    __u16 scope;
    __u64 dad_nonce;
    long unsigned int cstamp;
    long unsigned int tstamp;
    struct delayed_work dad_work;
    struct inet6_dev *idev;
    struct fib6_info *rt;
    struct hlist_node addr_lst;
    struct list_head if_list;
    struct list_head tmp_list;
    struct inet6_ifaddr *ifpub;
    int regen_count;
    bool tokenized;
    struct callback_head rcu;
    struct in6_addr peer_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct inet6_ifaddr {
    struct in6_addr addr;
    __u32 prefix_len;
    __u32 rt_priority;
    __u32 valid_lft;
    __u32 prefered_lft;
    refcount_t refcnt;
    spinlock_t lock;
    int state;
    __u32 flags;
    __u8 dad_probes;
    __u8 stable_privacy_retry;
    __u16 scope;
    __u64 dad_nonce;
    long unsigned int cstamp;
    long unsigned int tstamp;
    struct delayed_work dad_work;
    struct inet6_dev *idev;
    struct fib6_info *rt;
    struct hlist_node addr_lst;
    struct list_head if_list;
    struct list_head if_list_aux;
    struct list_head tmp_list;
    struct inet6_ifaddr *ifpub;
    int regen_count;
    bool tokenized;
    u8 ifa_proto;
    struct callback_head rcu;
    struct in6_addr peer_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct inet6_ifaddr {
    struct in6_addr addr;
    __u32 prefix_len;
    __u32 rt_priority;
    __u32 valid_lft;
    __u32 prefered_lft;
    refcount_t refcnt;
    spinlock_t lock;
    int state;
    __u32 flags;
    __u8 dad_probes;
    __u8 stable_privacy_retry;
    __u16 scope;
    __u64 dad_nonce;
    long unsigned int cstamp;
    long unsigned int tstamp;
    struct delayed_work dad_work;
    struct inet6_dev *idev;
    struct fib6_info *rt;
    struct hlist_node addr_lst;
    struct list_head if_list;
    struct list_head if_list_aux;
    struct list_head tmp_list;
    struct inet6_ifaddr *ifpub;
    int regen_count;
    bool tokenized;
    u8 ifa_proto;
    struct callback_head rcu;
    struct in6_addr peer_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct inet6_ifaddr {
    struct in6_addr addr;
    __u32 prefix_len;
    __u32 rt_priority;
    __u32 valid_lft;
    __u32 prefered_lft;
    refcount_t refcnt;
    spinlock_t lock;
    int state;
    __u32 flags;
    __u8 dad_probes;
    __u8 stable_privacy_retry;
    __u16 scope;
    __u64 dad_nonce;
    long unsigned int cstamp;
    long unsigned int tstamp;
    struct delayed_work dad_work;
    struct inet6_dev *idev;
    struct fib6_info *rt;
    struct hlist_node addr_lst;
    struct list_head if_list;
    struct list_head if_list_aux;
    struct list_head tmp_list;
    struct inet6_ifaddr *ifpub;
    int regen_count;
    bool tokenized;
    u8 ifa_proto;
    struct callback_head rcu;
    struct in6_addr peer_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct inet6_ifaddr {
    struct in6_addr addr;
    __u32 prefix_len;
    __u32 rt_priority;
    __u32 valid_lft;
    __u32 prefered_lft;
    refcount_t refcnt;
    spinlock_t lock;
    int state;
    __u32 flags;
    __u8 dad_probes;
    __u8 stable_privacy_retry;
    __u16 scope;
    __u64 dad_nonce;
    long unsigned int cstamp;
    long unsigned int tstamp;
    struct delayed_work dad_work;
    struct inet6_dev *idev;
    struct fib6_info *rt;
    struct hlist_node addr_lst;
    struct list_head if_list;
    struct list_head if_list_aux;
    struct list_head tmp_list;
    struct inet6_ifaddr *ifpub;
    int regen_count;
    bool tokenized;
    u8 ifa_proto;
    struct callback_head rcu;
    struct in6_addr peer_addr;
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
struct inet6_ifaddr {
    struct in6_addr addr;
    __u32 prefix_len;
    __u32 rt_priority;
    __u32 valid_lft;
    __u32 prefered_lft;
    refcount_t refcnt;
    spinlock_t lock;
    int state;
    __u32 flags;
    __u8 dad_probes;
    __u8 stable_privacy_retry;
    __u16 scope;
    __u64 dad_nonce;
    long unsigned int cstamp;
    long unsigned int tstamp;
    struct delayed_work dad_work;
    struct inet6_dev *idev;
    struct fib6_info *rt;
    struct hlist_node addr_lst;
    struct list_head if_list;
    struct list_head tmp_list;
    struct inet6_ifaddr *ifpub;
    int regen_count;
    bool tokenized;
    struct callback_head rcu;
    struct in6_addr peer_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct inet6_ifaddr {
    struct in6_addr addr;
    __u32 prefix_len;
    __u32 rt_priority;
    __u32 valid_lft;
    __u32 prefered_lft;
    refcount_t refcnt;
    spinlock_t lock;
    int state;
    __u32 flags;
    __u8 dad_probes;
    __u8 stable_privacy_retry;
    __u16 scope;
    __u64 dad_nonce;
    long unsigned int cstamp;
    long unsigned int tstamp;
    struct delayed_work dad_work;
    struct inet6_dev *idev;
    struct fib6_info *rt;
    struct hlist_node addr_lst;
    struct list_head if_list;
    struct list_head tmp_list;
    struct inet6_ifaddr *ifpub;
    int regen_count;
    bool tokenized;
    struct callback_head rcu;
    struct in6_addr peer_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct inet6_ifaddr {
    struct in6_addr addr;
    __u32 prefix_len;
    __u32 rt_priority;
    __u32 valid_lft;
    __u32 prefered_lft;
    refcount_t refcnt;
    spinlock_t lock;
    int state;
    __u32 flags;
    __u8 dad_probes;
    __u8 stable_privacy_retry;
    __u16 scope;
    __u64 dad_nonce;
    long unsigned int cstamp;
    long unsigned int tstamp;
    struct delayed_work dad_work;
    struct inet6_dev *idev;
    struct fib6_info *rt;
    struct hlist_node addr_lst;
    struct list_head if_list;
    struct list_head tmp_list;
    struct inet6_ifaddr *ifpub;
    int regen_count;
    bool tokenized;
    struct callback_head rcu;
    struct in6_addr peer_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct inet6_ifaddr {
    struct in6_addr addr;
    __u32 prefix_len;
    __u32 rt_priority;
    __u32 valid_lft;
    __u32 prefered_lft;
    refcount_t refcnt;
    spinlock_t lock;
    int state;
    __u32 flags;
    __u8 dad_probes;
    __u8 stable_privacy_retry;
    __u16 scope;
    __u64 dad_nonce;
    long unsigned int cstamp;
    long unsigned int tstamp;
    struct delayed_work dad_work;
    struct inet6_dev *idev;
    struct fib6_info *rt;
    struct hlist_node addr_lst;
    struct list_head if_list;
    struct list_head tmp_list;
    struct inet6_ifaddr *ifpub;
    int regen_count;
    bool tokenized;
    struct callback_head rcu;
    struct in6_addr peer_addr;
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
struct inet6_ifaddr {
    struct in6_addr addr;
    __u32 prefix_len;
    __u32 rt_priority;
    __u32 valid_lft;
    __u32 prefered_lft;
    refcount_t refcnt;
    spinlock_t lock;
    int state;
    __u32 flags;
    __u8 dad_probes;
    __u8 stable_privacy_retry;
    __u16 scope;
    __u64 dad_nonce;
    long unsigned int cstamp;
    long unsigned int tstamp;
    struct delayed_work dad_work;
    struct inet6_dev *idev;
    struct fib6_info *rt;
    struct hlist_node addr_lst;
    struct list_head if_list;
    struct list_head tmp_list;
    struct inet6_ifaddr *ifpub;
    int regen_count;
    bool tokenized;
    struct callback_head rcu;
    struct in6_addr peer_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct inet6_ifaddr {
    struct in6_addr addr;
    __u32 prefix_len;
    __u32 rt_priority;
    __u32 valid_lft;
    __u32 prefered_lft;
    refcount_t refcnt;
    spinlock_t lock;
    int state;
    __u32 flags;
    __u8 dad_probes;
    __u8 stable_privacy_retry;
    __u16 scope;
    __u64 dad_nonce;
    long unsigned int cstamp;
    long unsigned int tstamp;
    struct delayed_work dad_work;
    struct inet6_dev *idev;
    struct fib6_info *rt;
    struct hlist_node addr_lst;
    struct list_head if_list;
    struct list_head tmp_list;
    struct inet6_ifaddr *ifpub;
    int regen_count;
    bool tokenized;
    struct callback_head rcu;
    struct in6_addr peer_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct inet6_ifaddr {
    struct in6_addr addr;
    __u32 prefix_len;
    __u32 rt_priority;
    __u32 valid_lft;
    __u32 prefered_lft;
    refcount_t refcnt;
    spinlock_t lock;
    int state;
    __u32 flags;
    __u8 dad_probes;
    __u8 stable_privacy_retry;
    __u16 scope;
    __u64 dad_nonce;
    long unsigned int cstamp;
    long unsigned int tstamp;
    struct delayed_work dad_work;
    struct inet6_dev *idev;
    struct fib6_info *rt;
    struct hlist_node addr_lst;
    struct list_head if_list;
    struct list_head tmp_list;
    struct inet6_ifaddr *ifpub;
    int regen_count;
    bool tokenized;
    struct callback_head rcu;
    struct in6_addr peer_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct inet6_ifaddr {
    struct in6_addr addr;
    __u32 prefix_len;
    __u32 rt_priority;
    __u32 valid_lft;
    __u32 prefered_lft;
    refcount_t refcnt;
    spinlock_t lock;
    int state;
    __u32 flags;
    __u8 dad_probes;
    __u8 stable_privacy_retry;
    __u16 scope;
    __u64 dad_nonce;
    long unsigned int cstamp;
    long unsigned int tstamp;
    struct delayed_work dad_work;
    struct inet6_dev *idev;
    struct fib6_info *rt;
    struct hlist_node addr_lst;
    struct list_head if_list;
    struct list_head tmp_list;
    struct inet6_ifaddr *ifpub;
    int regen_count;
    bool tokenized;
    struct callback_head rcu;
    struct in6_addr peer_addr;
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
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u64 dad_nonce</code>
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
<code>atomic_t refcnt</code> ➡️ <code>refcount_t refcnt</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u32 rt_priority</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct rt6_info *rt</code> ➡️ <code>struct fib6_info *rt</code>
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
<code>struct list_head if_list_aux</code>
</li>
<li>
<b>Field added. </b>
<code>u8 ifa_proto</code>
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
