# Struct: <code>rpc_xprt_switch</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct rpc_xprt_switch {
    spinlock_t xps_lock;
    struct kref xps_kref;
    unsigned int xps_nxprts;
    struct list_head xps_xprt_list;
    struct net *xps_net;
    const struct rpc_xprt_iter_ops *xps_iter_ops;
    struct callback_head xps_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rpc_xprt_switch {
    spinlock_t xps_lock;
    struct kref xps_kref;
    unsigned int xps_nxprts;
    struct list_head xps_xprt_list;
    struct net *xps_net;
    const struct rpc_xprt_iter_ops *xps_iter_ops;
    struct callback_head xps_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rpc_xprt_switch {
    spinlock_t xps_lock;
    struct kref xps_kref;
    unsigned int xps_nxprts;
    struct list_head xps_xprt_list;
    struct net *xps_net;
    const struct rpc_xprt_iter_ops *xps_iter_ops;
    struct callback_head xps_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rpc_xprt_switch {
    spinlock_t xps_lock;
    struct kref xps_kref;
    unsigned int xps_nxprts;
    struct list_head xps_xprt_list;
    struct net *xps_net;
    const struct rpc_xprt_iter_ops *xps_iter_ops;
    struct callback_head xps_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rpc_xprt_switch {
    spinlock_t xps_lock;
    struct kref xps_kref;
    unsigned int xps_nxprts;
    struct list_head xps_xprt_list;
    struct net *xps_net;
    const struct rpc_xprt_iter_ops *xps_iter_ops;
    struct callback_head xps_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rpc_xprt_switch {
    spinlock_t xps_lock;
    struct kref xps_kref;
    unsigned int xps_nxprts;
    struct list_head xps_xprt_list;
    struct net *xps_net;
    const struct rpc_xprt_iter_ops *xps_iter_ops;
    struct callback_head xps_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rpc_xprt_switch {
    spinlock_t xps_lock;
    struct kref xps_kref;
    unsigned int xps_nxprts;
    unsigned int xps_nactive;
    atomic_long_t xps_queuelen;
    struct list_head xps_xprt_list;
    struct net *xps_net;
    const struct rpc_xprt_iter_ops *xps_iter_ops;
    struct callback_head xps_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rpc_xprt_switch {
    spinlock_t xps_lock;
    struct kref xps_kref;
    unsigned int xps_nxprts;
    unsigned int xps_nactive;
    atomic_long_t xps_queuelen;
    struct list_head xps_xprt_list;
    struct net *xps_net;
    const struct rpc_xprt_iter_ops *xps_iter_ops;
    struct callback_head xps_rcu;
};
```
</details>
</li>
<li>
In <code>5.8</code>: Absent ⚠️
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rpc_xprt_switch {
    spinlock_t xps_lock;
    struct kref xps_kref;
    unsigned int xps_nxprts;
    unsigned int xps_nactive;
    atomic_long_t xps_queuelen;
    struct list_head xps_xprt_list;
    struct net *xps_net;
    const struct rpc_xprt_iter_ops *xps_iter_ops;
    struct callback_head xps_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rpc_xprt_switch {
    spinlock_t xps_lock;
    struct kref xps_kref;
    unsigned int xps_id;
    unsigned int xps_nxprts;
    unsigned int xps_nactive;
    unsigned int xps_nunique_destaddr_xprts;
    atomic_long_t xps_queuelen;
    struct list_head xps_xprt_list;
    struct net *xps_net;
    const struct rpc_xprt_iter_ops *xps_iter_ops;
    struct rpc_sysfs_xprt_switch *xps_sysfs;
    struct callback_head xps_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rpc_xprt_switch {
    spinlock_t xps_lock;
    struct kref xps_kref;
    unsigned int xps_id;
    unsigned int xps_nxprts;
    unsigned int xps_nactive;
    unsigned int xps_nunique_destaddr_xprts;
    atomic_long_t xps_queuelen;
    struct list_head xps_xprt_list;
    struct net *xps_net;
    const struct rpc_xprt_iter_ops *xps_iter_ops;
    struct rpc_sysfs_xprt_switch *xps_sysfs;
    struct callback_head xps_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rpc_xprt_switch {
    spinlock_t xps_lock;
    struct kref xps_kref;
    unsigned int xps_id;
    unsigned int xps_nxprts;
    unsigned int xps_nactive;
    unsigned int xps_nunique_destaddr_xprts;
    atomic_long_t xps_queuelen;
    struct list_head xps_xprt_list;
    struct net *xps_net;
    const struct rpc_xprt_iter_ops *xps_iter_ops;
    struct rpc_sysfs_xprt_switch *xps_sysfs;
    struct callback_head xps_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rpc_xprt_switch {
    spinlock_t xps_lock;
    struct kref xps_kref;
    unsigned int xps_id;
    unsigned int xps_nxprts;
    unsigned int xps_nactive;
    unsigned int xps_nunique_destaddr_xprts;
    atomic_long_t xps_queuelen;
    struct list_head xps_xprt_list;
    struct net *xps_net;
    const struct rpc_xprt_iter_ops *xps_iter_ops;
    struct rpc_sysfs_xprt_switch *xps_sysfs;
    struct callback_head xps_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rpc_xprt_switch {
    spinlock_t xps_lock;
    struct kref xps_kref;
    unsigned int xps_id;
    unsigned int xps_nxprts;
    unsigned int xps_nactive;
    unsigned int xps_nunique_destaddr_xprts;
    atomic_long_t xps_queuelen;
    struct list_head xps_xprt_list;
    struct net *xps_net;
    const struct rpc_xprt_iter_ops *xps_iter_ops;
    struct rpc_sysfs_xprt_switch *xps_sysfs;
    struct callback_head xps_rcu;
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
struct rpc_xprt_switch {
    spinlock_t xps_lock;
    struct kref xps_kref;
    unsigned int xps_nxprts;
    unsigned int xps_nactive;
    atomic_long_t xps_queuelen;
    struct list_head xps_xprt_list;
    struct net *xps_net;
    const struct rpc_xprt_iter_ops *xps_iter_ops;
    struct callback_head xps_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rpc_xprt_switch {
    spinlock_t xps_lock;
    struct kref xps_kref;
    unsigned int xps_nxprts;
    unsigned int xps_nactive;
    atomic_long_t xps_queuelen;
    struct list_head xps_xprt_list;
    struct net *xps_net;
    const struct rpc_xprt_iter_ops *xps_iter_ops;
    struct callback_head xps_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rpc_xprt_switch {
    spinlock_t xps_lock;
    struct kref xps_kref;
    unsigned int xps_nxprts;
    unsigned int xps_nactive;
    atomic_long_t xps_queuelen;
    struct list_head xps_xprt_list;
    struct net *xps_net;
    const struct rpc_xprt_iter_ops *xps_iter_ops;
    struct callback_head xps_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct rpc_xprt_switch {
    spinlock_t xps_lock;
    struct kref xps_kref;
    unsigned int xps_nxprts;
    unsigned int xps_nactive;
    atomic_long_t xps_queuelen;
    struct list_head xps_xprt_list;
    struct net *xps_net;
    const struct rpc_xprt_iter_ops *xps_iter_ops;
    struct callback_head xps_rcu;
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
struct rpc_xprt_switch {
    spinlock_t xps_lock;
    struct kref xps_kref;
    unsigned int xps_nxprts;
    unsigned int xps_nactive;
    atomic_long_t xps_queuelen;
    struct list_head xps_xprt_list;
    struct net *xps_net;
    const struct rpc_xprt_iter_ops *xps_iter_ops;
    struct callback_head xps_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rpc_xprt_switch {
    spinlock_t xps_lock;
    struct kref xps_kref;
    unsigned int xps_nxprts;
    unsigned int xps_nactive;
    atomic_long_t xps_queuelen;
    struct list_head xps_xprt_list;
    struct net *xps_net;
    const struct rpc_xprt_iter_ops *xps_iter_ops;
    struct callback_head xps_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rpc_xprt_switch {
    spinlock_t xps_lock;
    struct kref xps_kref;
    unsigned int xps_nxprts;
    unsigned int xps_nactive;
    atomic_long_t xps_queuelen;
    struct list_head xps_xprt_list;
    struct net *xps_net;
    const struct rpc_xprt_iter_ops *xps_iter_ops;
    struct callback_head xps_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rpc_xprt_switch {
    spinlock_t xps_lock;
    struct kref xps_kref;
    unsigned int xps_nxprts;
    unsigned int xps_nactive;
    atomic_long_t xps_queuelen;
    struct list_head xps_xprt_list;
    struct net *xps_net;
    const struct rpc_xprt_iter_ops *xps_iter_ops;
    struct callback_head xps_rcu;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
<code>unsigned int xps_nactive</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t xps_queuelen</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int xps_id</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int xps_nunique_destaddr_xprts</code>
</li>
<li>
<b>Field added. </b>
<code>struct rpc_sysfs_xprt_switch *xps_sysfs</code>
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
