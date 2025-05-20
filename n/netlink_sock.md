# Struct: <code>netlink_sock</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct netlink_sock {
    struct sock sk;
    u32 portid;
    u32 dst_portid;
    u32 dst_group;
    u32 flags;
    u32 subscriptions;
    u32 ngroups;
    long unsigned int *groups;
    long unsigned int state;
    size_t max_recvmsg_len;
    wait_queue_head_t wait;
    bool bound;
    bool cb_running;
    struct netlink_callback cb;
    struct mutex *cb_mutex;
    struct mutex cb_def_mutex;
    void (*netlink_rcv)(struct sk_buff *);
    int (*netlink_bind)(struct net *, int);
    void (*netlink_unbind)(struct net *, int);
    struct module *module;
    struct mutex pg_vec_lock;
    struct netlink_ring rx_ring;
    struct netlink_ring tx_ring;
    atomic_t mapped;
    struct rhash_head node;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct netlink_sock {
    struct sock sk;
    u32 portid;
    u32 dst_portid;
    u32 dst_group;
    u32 flags;
    u32 subscriptions;
    u32 ngroups;
    long unsigned int *groups;
    long unsigned int state;
    size_t max_recvmsg_len;
    wait_queue_head_t wait;
    bool bound;
    bool cb_running;
    struct netlink_callback cb;
    struct mutex *cb_mutex;
    struct mutex cb_def_mutex;
    void (*netlink_rcv)(struct sk_buff *);
    int (*netlink_bind)(struct net *, int);
    void (*netlink_unbind)(struct net *, int);
    struct module *module;
    struct rhash_head node;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct netlink_sock {
    struct sock sk;
    u32 portid;
    u32 dst_portid;
    u32 dst_group;
    u32 flags;
    u32 subscriptions;
    u32 ngroups;
    long unsigned int *groups;
    long unsigned int state;
    size_t max_recvmsg_len;
    wait_queue_head_t wait;
    bool bound;
    bool cb_running;
    struct netlink_callback cb;
    struct mutex *cb_mutex;
    struct mutex cb_def_mutex;
    void (*netlink_rcv)(struct sk_buff *);
    int (*netlink_bind)(struct net *, int);
    void (*netlink_unbind)(struct net *, int);
    struct module *module;
    struct rhash_head node;
    struct callback_head rcu;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct netlink_sock {
    struct sock sk;
    u32 portid;
    u32 dst_portid;
    u32 dst_group;
    u32 flags;
    u32 subscriptions;
    u32 ngroups;
    long unsigned int *groups;
    long unsigned int state;
    size_t max_recvmsg_len;
    wait_queue_head_t wait;
    bool bound;
    bool cb_running;
    struct netlink_callback cb;
    struct mutex *cb_mutex;
    struct mutex cb_def_mutex;
    void (*netlink_rcv)(struct sk_buff *);
    int (*netlink_bind)(struct net *, int);
    void (*netlink_unbind)(struct net *, int);
    struct module *module;
    struct rhash_head node;
    struct callback_head rcu;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct netlink_sock {
    struct sock sk;
    u32 portid;
    u32 dst_portid;
    u32 dst_group;
    u32 flags;
    u32 subscriptions;
    u32 ngroups;
    long unsigned int *groups;
    long unsigned int state;
    size_t max_recvmsg_len;
    wait_queue_head_t wait;
    bool bound;
    bool cb_running;
    int dump_done_errno;
    struct netlink_callback cb;
    struct mutex *cb_mutex;
    struct mutex cb_def_mutex;
    void (*netlink_rcv)(struct sk_buff *);
    int (*netlink_bind)(struct net *, int);
    void (*netlink_unbind)(struct net *, int);
    struct module *module;
    struct rhash_head node;
    struct callback_head rcu;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct netlink_sock {
    struct sock sk;
    u32 portid;
    u32 dst_portid;
    u32 dst_group;
    u32 flags;
    u32 subscriptions;
    u32 ngroups;
    long unsigned int *groups;
    long unsigned int state;
    size_t max_recvmsg_len;
    wait_queue_head_t wait;
    bool bound;
    bool cb_running;
    int dump_done_errno;
    struct netlink_callback cb;
    struct mutex *cb_mutex;
    struct mutex cb_def_mutex;
    void (*netlink_rcv)(struct sk_buff *);
    int (*netlink_bind)(struct net *, int);
    void (*netlink_unbind)(struct net *, int);
    struct module *module;
    struct rhash_head node;
    struct callback_head rcu;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct netlink_sock {
    struct sock sk;
    u32 portid;
    u32 dst_portid;
    u32 dst_group;
    u32 flags;
    u32 subscriptions;
    u32 ngroups;
    long unsigned int *groups;
    long unsigned int state;
    size_t max_recvmsg_len;
    wait_queue_head_t wait;
    bool bound;
    bool cb_running;
    int dump_done_errno;
    struct netlink_callback cb;
    struct mutex *cb_mutex;
    struct mutex cb_def_mutex;
    void (*netlink_rcv)(struct sk_buff *);
    int (*netlink_bind)(struct net *, int);
    void (*netlink_unbind)(struct net *, int);
    struct module *module;
    struct rhash_head node;
    struct callback_head rcu;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct netlink_sock {
    struct sock sk;
    u32 portid;
    u32 dst_portid;
    u32 dst_group;
    u32 flags;
    u32 subscriptions;
    u32 ngroups;
    long unsigned int *groups;
    long unsigned int state;
    size_t max_recvmsg_len;
    wait_queue_head_t wait;
    bool bound;
    bool cb_running;
    int dump_done_errno;
    struct netlink_callback cb;
    struct mutex *cb_mutex;
    struct mutex cb_def_mutex;
    void (*netlink_rcv)(struct sk_buff *);
    int (*netlink_bind)(struct net *, int);
    void (*netlink_unbind)(struct net *, int);
    struct module *module;
    struct rhash_head node;
    struct callback_head rcu;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct netlink_sock {
    struct sock sk;
    u32 portid;
    u32 dst_portid;
    u32 dst_group;
    u32 flags;
    u32 subscriptions;
    u32 ngroups;
    long unsigned int *groups;
    long unsigned int state;
    size_t max_recvmsg_len;
    wait_queue_head_t wait;
    bool bound;
    bool cb_running;
    int dump_done_errno;
    struct netlink_callback cb;
    struct mutex *cb_mutex;
    struct mutex cb_def_mutex;
    void (*netlink_rcv)(struct sk_buff *);
    int (*netlink_bind)(struct net *, int);
    void (*netlink_unbind)(struct net *, int);
    struct module *module;
    struct rhash_head node;
    struct callback_head rcu;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct netlink_sock {
    struct sock sk;
    u32 portid;
    u32 dst_portid;
    u32 dst_group;
    u32 flags;
    u32 subscriptions;
    u32 ngroups;
    long unsigned int *groups;
    long unsigned int state;
    size_t max_recvmsg_len;
    wait_queue_head_t wait;
    bool bound;
    bool cb_running;
    int dump_done_errno;
    struct netlink_callback cb;
    struct mutex *cb_mutex;
    struct mutex cb_def_mutex;
    void (*netlink_rcv)(struct sk_buff *);
    int (*netlink_bind)(struct net *, int);
    void (*netlink_unbind)(struct net *, int);
    struct module *module;
    struct rhash_head node;
    struct callback_head rcu;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct netlink_sock {
    struct sock sk;
    u32 portid;
    u32 dst_portid;
    u32 dst_group;
    u32 flags;
    u32 subscriptions;
    u32 ngroups;
    long unsigned int *groups;
    long unsigned int state;
    size_t max_recvmsg_len;
    wait_queue_head_t wait;
    bool bound;
    bool cb_running;
    int dump_done_errno;
    struct netlink_callback cb;
    struct mutex *cb_mutex;
    struct mutex cb_def_mutex;
    void (*netlink_rcv)(struct sk_buff *);
    int (*netlink_bind)(struct net *, int);
    void (*netlink_unbind)(struct net *, int);
    struct module *module;
    struct rhash_head node;
    struct callback_head rcu;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct netlink_sock {
    struct sock sk;
    u32 portid;
    u32 dst_portid;
    u32 dst_group;
    u32 flags;
    u32 subscriptions;
    u32 ngroups;
    long unsigned int *groups;
    long unsigned int state;
    size_t max_recvmsg_len;
    wait_queue_head_t wait;
    bool bound;
    bool cb_running;
    int dump_done_errno;
    struct netlink_callback cb;
    struct mutex *cb_mutex;
    struct mutex cb_def_mutex;
    void (*netlink_rcv)(struct sk_buff *);
    int (*netlink_bind)(struct net *, int);
    void (*netlink_unbind)(struct net *, int);
    struct module *module;
    struct rhash_head node;
    struct callback_head rcu;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct netlink_sock {
    struct sock sk;
    u32 portid;
    u32 dst_portid;
    u32 dst_group;
    u32 flags;
    u32 subscriptions;
    u32 ngroups;
    long unsigned int *groups;
    long unsigned int state;
    size_t max_recvmsg_len;
    wait_queue_head_t wait;
    bool bound;
    bool cb_running;
    int dump_done_errno;
    struct netlink_callback cb;
    struct mutex *cb_mutex;
    struct mutex cb_def_mutex;
    void (*netlink_rcv)(struct sk_buff *);
    int (*netlink_bind)(struct net *, int);
    void (*netlink_unbind)(struct net *, int);
    struct module *module;
    struct rhash_head node;
    struct callback_head rcu;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct netlink_sock {
    struct sock sk;
    u32 portid;
    u32 dst_portid;
    u32 dst_group;
    u32 flags;
    u32 subscriptions;
    u32 ngroups;
    long unsigned int *groups;
    long unsigned int state;
    size_t max_recvmsg_len;
    wait_queue_head_t wait;
    bool bound;
    bool cb_running;
    int dump_done_errno;
    struct netlink_callback cb;
    struct mutex *cb_mutex;
    struct mutex cb_def_mutex;
    void (*netlink_rcv)(struct sk_buff *);
    int (*netlink_bind)(struct net *, int);
    void (*netlink_unbind)(struct net *, int);
    struct module *module;
    struct rhash_head node;
    struct callback_head rcu;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct netlink_sock {
    struct sock sk;
    u32 portid;
    u32 dst_portid;
    u32 dst_group;
    u32 flags;
    u32 subscriptions;
    u32 ngroups;
    long unsigned int *groups;
    long unsigned int state;
    size_t max_recvmsg_len;
    wait_queue_head_t wait;
    bool bound;
    bool cb_running;
    int dump_done_errno;
    struct netlink_callback cb;
    struct mutex *cb_mutex;
    struct mutex cb_def_mutex;
    void (*netlink_rcv)(struct sk_buff *);
    int (*netlink_bind)(struct net *, int);
    void (*netlink_unbind)(struct net *, int);
    struct module *module;
    struct rhash_head node;
    struct callback_head rcu;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct netlink_sock {
    struct sock sk;
    u32 portid;
    u32 dst_portid;
    u32 dst_group;
    u32 flags;
    u32 subscriptions;
    u32 ngroups;
    long unsigned int *groups;
    long unsigned int state;
    size_t max_recvmsg_len;
    wait_queue_head_t wait;
    bool bound;
    bool cb_running;
    int dump_done_errno;
    struct netlink_callback cb;
    struct mutex *cb_mutex;
    struct mutex cb_def_mutex;
    void (*netlink_rcv)(struct sk_buff *);
    int (*netlink_bind)(struct net *, int);
    void (*netlink_unbind)(struct net *, int);
    struct module *module;
    struct rhash_head node;
    struct callback_head rcu;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct netlink_sock {
    struct sock sk;
    long unsigned int flags;
    u32 portid;
    u32 dst_portid;
    u32 dst_group;
    u32 subscriptions;
    u32 ngroups;
    long unsigned int *groups;
    long unsigned int state;
    size_t max_recvmsg_len;
    wait_queue_head_t wait;
    bool bound;
    bool cb_running;
    int dump_done_errno;
    struct netlink_callback cb;
    struct mutex *cb_mutex;
    struct mutex cb_def_mutex;
    void (*netlink_rcv)(struct sk_buff *);
    int (*netlink_bind)(struct net *, int);
    void (*netlink_unbind)(struct net *, int);
    void (*netlink_release)(struct sock *, long unsigned int *);
    struct module *module;
    struct rhash_head node;
    struct callback_head rcu;
    struct work_struct work;
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
struct netlink_sock {
    struct sock sk;
    u32 portid;
    u32 dst_portid;
    u32 dst_group;
    u32 flags;
    u32 subscriptions;
    u32 ngroups;
    long unsigned int *groups;
    long unsigned int state;
    size_t max_recvmsg_len;
    wait_queue_head_t wait;
    bool bound;
    bool cb_running;
    int dump_done_errno;
    struct netlink_callback cb;
    struct mutex *cb_mutex;
    struct mutex cb_def_mutex;
    void (*netlink_rcv)(struct sk_buff *);
    int (*netlink_bind)(struct net *, int);
    void (*netlink_unbind)(struct net *, int);
    struct module *module;
    struct rhash_head node;
    struct callback_head rcu;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct netlink_sock {
    struct sock sk;
    u32 portid;
    u32 dst_portid;
    u32 dst_group;
    u32 flags;
    u32 subscriptions;
    u32 ngroups;
    long unsigned int *groups;
    long unsigned int state;
    size_t max_recvmsg_len;
    wait_queue_head_t wait;
    bool bound;
    bool cb_running;
    int dump_done_errno;
    struct netlink_callback cb;
    struct mutex *cb_mutex;
    struct mutex cb_def_mutex;
    void (*netlink_rcv)(struct sk_buff *);
    int (*netlink_bind)(struct net *, int);
    void (*netlink_unbind)(struct net *, int);
    struct module *module;
    struct rhash_head node;
    struct callback_head rcu;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct netlink_sock {
    struct sock sk;
    u32 portid;
    u32 dst_portid;
    u32 dst_group;
    u32 flags;
    u32 subscriptions;
    u32 ngroups;
    long unsigned int *groups;
    long unsigned int state;
    size_t max_recvmsg_len;
    wait_queue_head_t wait;
    bool bound;
    bool cb_running;
    int dump_done_errno;
    struct netlink_callback cb;
    struct mutex *cb_mutex;
    struct mutex cb_def_mutex;
    void (*netlink_rcv)(struct sk_buff *);
    int (*netlink_bind)(struct net *, int);
    void (*netlink_unbind)(struct net *, int);
    struct module *module;
    struct rhash_head node;
    struct callback_head rcu;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct netlink_sock {
    struct sock sk;
    u32 portid;
    u32 dst_portid;
    u32 dst_group;
    u32 flags;
    u32 subscriptions;
    u32 ngroups;
    long unsigned int *groups;
    long unsigned int state;
    size_t max_recvmsg_len;
    wait_queue_head_t wait;
    bool bound;
    bool cb_running;
    int dump_done_errno;
    struct netlink_callback cb;
    struct mutex *cb_mutex;
    struct mutex cb_def_mutex;
    void (*netlink_rcv)(struct sk_buff *);
    int (*netlink_bind)(struct net *, int);
    void (*netlink_unbind)(struct net *, int);
    struct module *module;
    struct rhash_head node;
    struct callback_head rcu;
    struct work_struct work;
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
struct netlink_sock {
    struct sock sk;
    u32 portid;
    u32 dst_portid;
    u32 dst_group;
    u32 flags;
    u32 subscriptions;
    u32 ngroups;
    long unsigned int *groups;
    long unsigned int state;
    size_t max_recvmsg_len;
    wait_queue_head_t wait;
    bool bound;
    bool cb_running;
    int dump_done_errno;
    struct netlink_callback cb;
    struct mutex *cb_mutex;
    struct mutex cb_def_mutex;
    void (*netlink_rcv)(struct sk_buff *);
    int (*netlink_bind)(struct net *, int);
    void (*netlink_unbind)(struct net *, int);
    struct module *module;
    struct rhash_head node;
    struct callback_head rcu;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct netlink_sock {
    struct sock sk;
    u32 portid;
    u32 dst_portid;
    u32 dst_group;
    u32 flags;
    u32 subscriptions;
    u32 ngroups;
    long unsigned int *groups;
    long unsigned int state;
    size_t max_recvmsg_len;
    wait_queue_head_t wait;
    bool bound;
    bool cb_running;
    int dump_done_errno;
    struct netlink_callback cb;
    struct mutex *cb_mutex;
    struct mutex cb_def_mutex;
    void (*netlink_rcv)(struct sk_buff *);
    int (*netlink_bind)(struct net *, int);
    void (*netlink_unbind)(struct net *, int);
    struct module *module;
    struct rhash_head node;
    struct callback_head rcu;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct netlink_sock {
    struct sock sk;
    u32 portid;
    u32 dst_portid;
    u32 dst_group;
    u32 flags;
    u32 subscriptions;
    u32 ngroups;
    long unsigned int *groups;
    long unsigned int state;
    size_t max_recvmsg_len;
    wait_queue_head_t wait;
    bool bound;
    bool cb_running;
    int dump_done_errno;
    struct netlink_callback cb;
    struct mutex *cb_mutex;
    struct mutex cb_def_mutex;
    void (*netlink_rcv)(struct sk_buff *);
    int (*netlink_bind)(struct net *, int);
    void (*netlink_unbind)(struct net *, int);
    struct module *module;
    struct rhash_head node;
    struct callback_head rcu;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct netlink_sock {
    struct sock sk;
    u32 portid;
    u32 dst_portid;
    u32 dst_group;
    u32 flags;
    u32 subscriptions;
    u32 ngroups;
    long unsigned int *groups;
    long unsigned int state;
    size_t max_recvmsg_len;
    wait_queue_head_t wait;
    bool bound;
    bool cb_running;
    int dump_done_errno;
    struct netlink_callback cb;
    struct mutex *cb_mutex;
    struct mutex cb_def_mutex;
    void (*netlink_rcv)(struct sk_buff *);
    int (*netlink_bind)(struct net *, int);
    void (*netlink_unbind)(struct net *, int);
    struct module *module;
    struct rhash_head node;
    struct callback_head rcu;
    struct work_struct work;
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
<b>Field removed. </b>
<code>struct mutex pg_vec_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>struct netlink_ring rx_ring</code>
</li>
<li>
<b>Field removed. </b>
<code>struct netlink_ring tx_ring</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t mapped</code>
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
<code>struct work_struct work</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int dump_done_errno</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*netlink_release)(struct sock *, long unsigned int *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 flags</code> ➡️ <code>long unsigned int flags</code>
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
