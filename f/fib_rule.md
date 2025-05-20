# Struct: <code>fib_rule</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct fib_rule {
    struct list_head list;
    int iifindex;
    int oifindex;
    u32 mark;
    u32 mark_mask;
    u32 flags;
    u32 table;
    u8 action;
    u32 target;
    __be64 tun_id;
    struct fib_rule *ctarget;
    struct net *fr_net;
    atomic_t refcnt;
    u32 pref;
    int suppress_ifgroup;
    int suppress_prefixlen;
    char iifname[16];
    char oifname[16];
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct fib_rule {
    struct list_head list;
    int iifindex;
    int oifindex;
    u32 mark;
    u32 mark_mask;
    u32 flags;
    u32 table;
    u8 action;
    u8 l3mdev;
    u32 target;
    __be64 tun_id;
    struct fib_rule *ctarget;
    struct net *fr_net;
    atomic_t refcnt;
    u32 pref;
    int suppress_ifgroup;
    int suppress_prefixlen;
    char iifname[16];
    char oifname[16];
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct fib_rule {
    struct list_head list;
    int iifindex;
    int oifindex;
    u32 mark;
    u32 mark_mask;
    u32 flags;
    u32 table;
    u8 action;
    u8 l3mdev;
    u32 target;
    __be64 tun_id;
    struct fib_rule *ctarget;
    struct net *fr_net;
    atomic_t refcnt;
    u32 pref;
    int suppress_ifgroup;
    int suppress_prefixlen;
    char iifname[16];
    char oifname[16];
    struct fib_kuid_range uid_range;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct fib_rule {
    struct list_head list;
    int iifindex;
    int oifindex;
    u32 mark;
    u32 mark_mask;
    u32 flags;
    u32 table;
    u8 action;
    u8 l3mdev;
    u32 target;
    __be64 tun_id;
    struct fib_rule *ctarget;
    struct net *fr_net;
    refcount_t refcnt;
    u32 pref;
    int suppress_ifgroup;
    int suppress_prefixlen;
    char iifname[16];
    char oifname[16];
    struct fib_kuid_range uid_range;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct fib_rule {
    struct list_head list;
    int iifindex;
    int oifindex;
    u32 mark;
    u32 mark_mask;
    u32 flags;
    u32 table;
    u8 action;
    u8 l3mdev;
    u32 target;
    __be64 tun_id;
    struct fib_rule *ctarget;
    struct net *fr_net;
    refcount_t refcnt;
    u32 pref;
    int suppress_ifgroup;
    int suppress_prefixlen;
    char iifname[16];
    char oifname[16];
    struct fib_kuid_range uid_range;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct fib_rule {
    struct list_head list;
    int iifindex;
    int oifindex;
    u32 mark;
    u32 mark_mask;
    u32 flags;
    u32 table;
    u8 action;
    u8 l3mdev;
    u8 proto;
    u8 ip_proto;
    u32 target;
    __be64 tun_id;
    struct fib_rule *ctarget;
    struct net *fr_net;
    refcount_t refcnt;
    u32 pref;
    int suppress_ifgroup;
    int suppress_prefixlen;
    char iifname[16];
    char oifname[16];
    struct fib_kuid_range uid_range;
    struct fib_rule_port_range sport_range;
    struct fib_rule_port_range dport_range;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct fib_rule {
    struct list_head list;
    int iifindex;
    int oifindex;
    u32 mark;
    u32 mark_mask;
    u32 flags;
    u32 table;
    u8 action;
    u8 l3mdev;
    u8 proto;
    u8 ip_proto;
    u32 target;
    __be64 tun_id;
    struct fib_rule *ctarget;
    struct net *fr_net;
    refcount_t refcnt;
    u32 pref;
    int suppress_ifgroup;
    int suppress_prefixlen;
    char iifname[16];
    char oifname[16];
    struct fib_kuid_range uid_range;
    struct fib_rule_port_range sport_range;
    struct fib_rule_port_range dport_range;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct fib_rule {
    struct list_head list;
    int iifindex;
    int oifindex;
    u32 mark;
    u32 mark_mask;
    u32 flags;
    u32 table;
    u8 action;
    u8 l3mdev;
    u8 proto;
    u8 ip_proto;
    u32 target;
    __be64 tun_id;
    struct fib_rule *ctarget;
    struct net *fr_net;
    refcount_t refcnt;
    u32 pref;
    int suppress_ifgroup;
    int suppress_prefixlen;
    char iifname[16];
    char oifname[16];
    struct fib_kuid_range uid_range;
    struct fib_rule_port_range sport_range;
    struct fib_rule_port_range dport_range;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct fib_rule {
    struct list_head list;
    int iifindex;
    int oifindex;
    u32 mark;
    u32 mark_mask;
    u32 flags;
    u32 table;
    u8 action;
    u8 l3mdev;
    u8 proto;
    u8 ip_proto;
    u32 target;
    __be64 tun_id;
    struct fib_rule *ctarget;
    struct net *fr_net;
    refcount_t refcnt;
    u32 pref;
    int suppress_ifgroup;
    int suppress_prefixlen;
    char iifname[16];
    char oifname[16];
    struct fib_kuid_range uid_range;
    struct fib_rule_port_range sport_range;
    struct fib_rule_port_range dport_range;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct fib_rule {
    struct list_head list;
    int iifindex;
    int oifindex;
    u32 mark;
    u32 mark_mask;
    u32 flags;
    u32 table;
    u8 action;
    u8 l3mdev;
    u8 proto;
    u8 ip_proto;
    u32 target;
    __be64 tun_id;
    struct fib_rule *ctarget;
    struct net *fr_net;
    refcount_t refcnt;
    u32 pref;
    int suppress_ifgroup;
    int suppress_prefixlen;
    char iifname[16];
    char oifname[16];
    struct fib_kuid_range uid_range;
    struct fib_rule_port_range sport_range;
    struct fib_rule_port_range dport_range;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct fib_rule {
    struct list_head list;
    int iifindex;
    int oifindex;
    u32 mark;
    u32 mark_mask;
    u32 flags;
    u32 table;
    u8 action;
    u8 l3mdev;
    u8 proto;
    u8 ip_proto;
    u32 target;
    __be64 tun_id;
    struct fib_rule *ctarget;
    struct net *fr_net;
    refcount_t refcnt;
    u32 pref;
    int suppress_ifgroup;
    int suppress_prefixlen;
    char iifname[16];
    char oifname[16];
    struct fib_kuid_range uid_range;
    struct fib_rule_port_range sport_range;
    struct fib_rule_port_range dport_range;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct fib_rule {
    struct list_head list;
    int iifindex;
    int oifindex;
    u32 mark;
    u32 mark_mask;
    u32 flags;
    u32 table;
    u8 action;
    u8 l3mdev;
    u8 proto;
    u8 ip_proto;
    u32 target;
    __be64 tun_id;
    struct fib_rule *ctarget;
    struct net *fr_net;
    refcount_t refcnt;
    u32 pref;
    int suppress_ifgroup;
    int suppress_prefixlen;
    char iifname[16];
    char oifname[16];
    struct fib_kuid_range uid_range;
    struct fib_rule_port_range sport_range;
    struct fib_rule_port_range dport_range;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct fib_rule {
    struct list_head list;
    int iifindex;
    int oifindex;
    u32 mark;
    u32 mark_mask;
    u32 flags;
    u32 table;
    u8 action;
    u8 l3mdev;
    u8 proto;
    u8 ip_proto;
    u32 target;
    __be64 tun_id;
    struct fib_rule *ctarget;
    struct net *fr_net;
    refcount_t refcnt;
    u32 pref;
    int suppress_ifgroup;
    int suppress_prefixlen;
    char iifname[16];
    char oifname[16];
    struct fib_kuid_range uid_range;
    struct fib_rule_port_range sport_range;
    struct fib_rule_port_range dport_range;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct fib_rule {
    struct list_head list;
    int iifindex;
    int oifindex;
    u32 mark;
    u32 mark_mask;
    u32 flags;
    u32 table;
    u8 action;
    u8 l3mdev;
    u8 proto;
    u8 ip_proto;
    u32 target;
    __be64 tun_id;
    struct fib_rule *ctarget;
    struct net *fr_net;
    refcount_t refcnt;
    u32 pref;
    int suppress_ifgroup;
    int suppress_prefixlen;
    char iifname[16];
    char oifname[16];
    struct fib_kuid_range uid_range;
    struct fib_rule_port_range sport_range;
    struct fib_rule_port_range dport_range;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct fib_rule {
    struct list_head list;
    int iifindex;
    int oifindex;
    u32 mark;
    u32 mark_mask;
    u32 flags;
    u32 table;
    u8 action;
    u8 l3mdev;
    u8 proto;
    u8 ip_proto;
    u32 target;
    __be64 tun_id;
    struct fib_rule *ctarget;
    struct net *fr_net;
    refcount_t refcnt;
    u32 pref;
    int suppress_ifgroup;
    int suppress_prefixlen;
    char iifname[16];
    char oifname[16];
    struct fib_kuid_range uid_range;
    struct fib_rule_port_range sport_range;
    struct fib_rule_port_range dport_range;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct fib_rule {
    struct list_head list;
    int iifindex;
    int oifindex;
    u32 mark;
    u32 mark_mask;
    u32 flags;
    u32 table;
    u8 action;
    u8 l3mdev;
    u8 proto;
    u8 ip_proto;
    u32 target;
    __be64 tun_id;
    struct fib_rule *ctarget;
    struct net *fr_net;
    refcount_t refcnt;
    u32 pref;
    int suppress_ifgroup;
    int suppress_prefixlen;
    char iifname[16];
    char oifname[16];
    struct fib_kuid_range uid_range;
    struct fib_rule_port_range sport_range;
    struct fib_rule_port_range dport_range;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct fib_rule {
    struct list_head list;
    int iifindex;
    int oifindex;
    u32 mark;
    u32 mark_mask;
    u32 flags;
    u32 table;
    u8 action;
    u8 l3mdev;
    u8 proto;
    u8 ip_proto;
    u32 target;
    __be64 tun_id;
    struct fib_rule *ctarget;
    struct net *fr_net;
    refcount_t refcnt;
    u32 pref;
    int suppress_ifgroup;
    int suppress_prefixlen;
    char iifname[16];
    char oifname[16];
    struct fib_kuid_range uid_range;
    struct fib_rule_port_range sport_range;
    struct fib_rule_port_range dport_range;
    struct callback_head rcu;
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
struct fib_rule {
    struct list_head list;
    int iifindex;
    int oifindex;
    u32 mark;
    u32 mark_mask;
    u32 flags;
    u32 table;
    u8 action;
    u8 l3mdev;
    u8 proto;
    u8 ip_proto;
    u32 target;
    __be64 tun_id;
    struct fib_rule *ctarget;
    struct net *fr_net;
    refcount_t refcnt;
    u32 pref;
    int suppress_ifgroup;
    int suppress_prefixlen;
    char iifname[16];
    char oifname[16];
    struct fib_kuid_range uid_range;
    struct fib_rule_port_range sport_range;
    struct fib_rule_port_range dport_range;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct fib_rule {
    struct list_head list;
    int iifindex;
    int oifindex;
    u32 mark;
    u32 mark_mask;
    u32 flags;
    u32 table;
    u8 action;
    u8 l3mdev;
    u8 proto;
    u8 ip_proto;
    u32 target;
    __be64 tun_id;
    struct fib_rule *ctarget;
    struct net *fr_net;
    refcount_t refcnt;
    u32 pref;
    int suppress_ifgroup;
    int suppress_prefixlen;
    char iifname[16];
    char oifname[16];
    struct fib_kuid_range uid_range;
    struct fib_rule_port_range sport_range;
    struct fib_rule_port_range dport_range;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct fib_rule {
    struct list_head list;
    int iifindex;
    int oifindex;
    u32 mark;
    u32 mark_mask;
    u32 flags;
    u32 table;
    u8 action;
    u8 l3mdev;
    u8 proto;
    u8 ip_proto;
    u32 target;
    __be64 tun_id;
    struct fib_rule *ctarget;
    struct net *fr_net;
    refcount_t refcnt;
    u32 pref;
    int suppress_ifgroup;
    int suppress_prefixlen;
    char iifname[16];
    char oifname[16];
    struct fib_kuid_range uid_range;
    struct fib_rule_port_range sport_range;
    struct fib_rule_port_range dport_range;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct fib_rule {
    struct list_head list;
    int iifindex;
    int oifindex;
    u32 mark;
    u32 mark_mask;
    u32 flags;
    u32 table;
    u8 action;
    u8 l3mdev;
    u8 proto;
    u8 ip_proto;
    u32 target;
    __be64 tun_id;
    struct fib_rule *ctarget;
    struct net *fr_net;
    refcount_t refcnt;
    u32 pref;
    int suppress_ifgroup;
    int suppress_prefixlen;
    char iifname[16];
    char oifname[16];
    struct fib_kuid_range uid_range;
    struct fib_rule_port_range sport_range;
    struct fib_rule_port_range dport_range;
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
struct fib_rule {
    struct list_head list;
    int iifindex;
    int oifindex;
    u32 mark;
    u32 mark_mask;
    u32 flags;
    u32 table;
    u8 action;
    u8 l3mdev;
    u8 proto;
    u8 ip_proto;
    u32 target;
    __be64 tun_id;
    struct fib_rule *ctarget;
    struct net *fr_net;
    refcount_t refcnt;
    u32 pref;
    int suppress_ifgroup;
    int suppress_prefixlen;
    char iifname[16];
    char oifname[16];
    struct fib_kuid_range uid_range;
    struct fib_rule_port_range sport_range;
    struct fib_rule_port_range dport_range;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct fib_rule {
    struct list_head list;
    int iifindex;
    int oifindex;
    u32 mark;
    u32 mark_mask;
    u32 flags;
    u32 table;
    u8 action;
    u8 l3mdev;
    u8 proto;
    u8 ip_proto;
    u32 target;
    __be64 tun_id;
    struct fib_rule *ctarget;
    struct net *fr_net;
    refcount_t refcnt;
    u32 pref;
    int suppress_ifgroup;
    int suppress_prefixlen;
    char iifname[16];
    char oifname[16];
    struct fib_kuid_range uid_range;
    struct fib_rule_port_range sport_range;
    struct fib_rule_port_range dport_range;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct fib_rule {
    struct list_head list;
    int iifindex;
    int oifindex;
    u32 mark;
    u32 mark_mask;
    u32 flags;
    u32 table;
    u8 action;
    u8 l3mdev;
    u8 proto;
    u8 ip_proto;
    u32 target;
    __be64 tun_id;
    struct fib_rule *ctarget;
    struct net *fr_net;
    refcount_t refcnt;
    u32 pref;
    int suppress_ifgroup;
    int suppress_prefixlen;
    char iifname[16];
    char oifname[16];
    struct fib_kuid_range uid_range;
    struct fib_rule_port_range sport_range;
    struct fib_rule_port_range dport_range;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct fib_rule {
    struct list_head list;
    int iifindex;
    int oifindex;
    u32 mark;
    u32 mark_mask;
    u32 flags;
    u32 table;
    u8 action;
    u8 l3mdev;
    u8 proto;
    u8 ip_proto;
    u32 target;
    __be64 tun_id;
    struct fib_rule *ctarget;
    struct net *fr_net;
    refcount_t refcnt;
    u32 pref;
    int suppress_ifgroup;
    int suppress_prefixlen;
    char iifname[16];
    char oifname[16];
    struct fib_kuid_range uid_range;
    struct fib_rule_port_range sport_range;
    struct fib_rule_port_range dport_range;
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
<details>
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 l3mdev</code>
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
<code>struct fib_kuid_range uid_range</code>
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
<code>u8 proto</code>
</li>
<li>
<b>Field added. </b>
<code>u8 ip_proto</code>
</li>
<li>
<b>Field added. </b>
<code>struct fib_rule_port_range sport_range</code>
</li>
<li>
<b>Field added. </b>
<code>struct fib_rule_port_range dport_range</code>
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
