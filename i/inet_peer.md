# Struct: <code>inet_peer</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct inet_peer {
    struct inet_peer *avl_left;
    struct inet_peer *avl_right;
    struct inetpeer_addr daddr;
    __u32 avl_height;
    u32 metrics[16];
    u32 rate_tokens;
    long unsigned int rate_last;
    struct list_head gc_list;
    struct callback_head gc_rcu;
    atomic_t rid;
    struct callback_head rcu;
    struct inet_peer *gc_next;
    __u32 dtime;
    atomic_t refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct inet_peer {
    struct inet_peer *avl_left;
    struct inet_peer *avl_right;
    struct inetpeer_addr daddr;
    __u32 avl_height;
    u32 metrics[16];
    u32 rate_tokens;
    long unsigned int rate_last;
    struct list_head gc_list;
    struct callback_head gc_rcu;
    atomic_t rid;
    struct callback_head rcu;
    struct inet_peer *gc_next;
    __u32 dtime;
    atomic_t refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct inet_peer {
    struct inet_peer *avl_left;
    struct inet_peer *avl_right;
    struct inetpeer_addr daddr;
    __u32 avl_height;
    u32 metrics[16];
    u32 rate_tokens;
    long unsigned int rate_last;
    struct list_head gc_list;
    struct callback_head gc_rcu;
    atomic_t rid;
    struct callback_head rcu;
    struct inet_peer *gc_next;
    __u32 dtime;
    atomic_t refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct inet_peer {
    struct inet_peer *avl_left;
    struct inet_peer *avl_right;
    struct inetpeer_addr daddr;
    __u32 avl_height;
    u32 metrics[16];
    u32 rate_tokens;
    long unsigned int rate_last;
    struct list_head gc_list;
    struct callback_head gc_rcu;
    atomic_t rid;
    struct callback_head rcu;
    struct inet_peer *gc_next;
    __u32 dtime;
    refcount_t refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct inet_peer {
    struct rb_node rb_node;
    struct inetpeer_addr daddr;
    u32 metrics[17];
    u32 rate_tokens;
    long unsigned int rate_last;
    atomic_t rid;
    struct callback_head rcu;
    __u32 dtime;
    refcount_t refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct inet_peer {
    struct rb_node rb_node;
    struct inetpeer_addr daddr;
    u32 metrics[17];
    u32 rate_tokens;
    long unsigned int rate_last;
    atomic_t rid;
    struct callback_head rcu;
    __u32 dtime;
    refcount_t refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct inet_peer {
    struct rb_node rb_node;
    struct inetpeer_addr daddr;
    u32 metrics[17];
    u32 rate_tokens;
    u32 n_redirects;
    long unsigned int rate_last;
    atomic_t rid;
    struct callback_head rcu;
    __u32 dtime;
    refcount_t refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct inet_peer {
    struct rb_node rb_node;
    struct inetpeer_addr daddr;
    u32 metrics[17];
    u32 rate_tokens;
    u32 n_redirects;
    long unsigned int rate_last;
    atomic_t rid;
    struct callback_head rcu;
    __u32 dtime;
    refcount_t refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct inet_peer {
    struct rb_node rb_node;
    struct inetpeer_addr daddr;
    u32 metrics[17];
    u32 rate_tokens;
    u32 n_redirects;
    long unsigned int rate_last;
    atomic_t rid;
    struct callback_head rcu;
    __u32 dtime;
    refcount_t refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct inet_peer {
    struct rb_node rb_node;
    struct inetpeer_addr daddr;
    u32 metrics[17];
    u32 rate_tokens;
    u32 n_redirects;
    long unsigned int rate_last;
    atomic_t rid;
    struct callback_head rcu;
    __u32 dtime;
    refcount_t refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct inet_peer {
    struct rb_node rb_node;
    struct inetpeer_addr daddr;
    u32 metrics[17];
    u32 rate_tokens;
    u32 n_redirects;
    long unsigned int rate_last;
    atomic_t rid;
    struct callback_head rcu;
    __u32 dtime;
    refcount_t refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct inet_peer {
    struct rb_node rb_node;
    struct inetpeer_addr daddr;
    u32 metrics[17];
    u32 rate_tokens;
    u32 n_redirects;
    long unsigned int rate_last;
    atomic_t rid;
    struct callback_head rcu;
    __u32 dtime;
    refcount_t refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct inet_peer {
    struct rb_node rb_node;
    struct inetpeer_addr daddr;
    u32 metrics[17];
    u32 rate_tokens;
    u32 n_redirects;
    long unsigned int rate_last;
    atomic_t rid;
    struct callback_head rcu;
    __u32 dtime;
    refcount_t refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct inet_peer {
    struct rb_node rb_node;
    struct inetpeer_addr daddr;
    u32 metrics[17];
    u32 rate_tokens;
    u32 n_redirects;
    long unsigned int rate_last;
    atomic_t rid;
    struct callback_head rcu;
    __u32 dtime;
    refcount_t refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct inet_peer {
    struct rb_node rb_node;
    struct inetpeer_addr daddr;
    u32 metrics[17];
    u32 rate_tokens;
    u32 n_redirects;
    long unsigned int rate_last;
    atomic_t rid;
    struct callback_head rcu;
    __u32 dtime;
    refcount_t refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct inet_peer {
    struct rb_node rb_node;
    struct inetpeer_addr daddr;
    u32 metrics[17];
    u32 rate_tokens;
    u32 n_redirects;
    long unsigned int rate_last;
    atomic_t rid;
    struct callback_head rcu;
    __u32 dtime;
    refcount_t refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct inet_peer {
    struct rb_node rb_node;
    struct inetpeer_addr daddr;
    u32 metrics[17];
    u32 rate_tokens;
    u32 n_redirects;
    long unsigned int rate_last;
    atomic_t rid;
    struct callback_head rcu;
    __u32 dtime;
    refcount_t refcnt;
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
struct inet_peer {
    struct rb_node rb_node;
    struct inetpeer_addr daddr;
    u32 metrics[17];
    u32 rate_tokens;
    u32 n_redirects;
    long unsigned int rate_last;
    atomic_t rid;
    struct callback_head rcu;
    __u32 dtime;
    refcount_t refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct inet_peer {
    struct rb_node rb_node;
    struct inetpeer_addr daddr;
    u32 metrics[17];
    u32 rate_tokens;
    u32 n_redirects;
    long unsigned int rate_last;
    atomic_t rid;
    struct callback_head rcu;
    __u32 dtime;
    refcount_t refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct inet_peer {
    struct rb_node rb_node;
    struct inetpeer_addr daddr;
    u32 metrics[17];
    u32 rate_tokens;
    u32 n_redirects;
    long unsigned int rate_last;
    atomic_t rid;
    struct callback_head rcu;
    __u32 dtime;
    refcount_t refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct inet_peer {
    struct rb_node rb_node;
    struct inetpeer_addr daddr;
    u32 metrics[17];
    u32 rate_tokens;
    u32 n_redirects;
    long unsigned int rate_last;
    atomic_t rid;
    struct callback_head rcu;
    __u32 dtime;
    refcount_t refcnt;
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
struct inet_peer {
    struct rb_node rb_node;
    struct inetpeer_addr daddr;
    u32 metrics[17];
    u32 rate_tokens;
    u32 n_redirects;
    long unsigned int rate_last;
    atomic_t rid;
    struct callback_head rcu;
    __u32 dtime;
    refcount_t refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct inet_peer {
    struct rb_node rb_node;
    struct inetpeer_addr daddr;
    u32 metrics[17];
    u32 rate_tokens;
    u32 n_redirects;
    long unsigned int rate_last;
    atomic_t rid;
    struct callback_head rcu;
    __u32 dtime;
    refcount_t refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct inet_peer {
    struct rb_node rb_node;
    struct inetpeer_addr daddr;
    u32 metrics[17];
    u32 rate_tokens;
    u32 n_redirects;
    long unsigned int rate_last;
    atomic_t rid;
    struct callback_head rcu;
    __u32 dtime;
    refcount_t refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct inet_peer {
    struct rb_node rb_node;
    struct inetpeer_addr daddr;
    u32 metrics[17];
    u32 rate_tokens;
    u32 n_redirects;
    long unsigned int rate_last;
    atomic_t rid;
    struct callback_head rcu;
    __u32 dtime;
    refcount_t refcnt;
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
<b>Field added. </b>
<code>struct rb_node rb_node</code>
</li>
<li>
<b>Field removed. </b>
<code>struct inet_peer *avl_left</code>
</li>
<li>
<b>Field removed. </b>
<code>struct inet_peer *avl_right</code>
</li>
<li>
<b>Field removed. </b>
<code>__u32 avl_height</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head gc_list</code>
</li>
<li>
<b>Field removed. </b>
<code>struct callback_head gc_rcu</code>
</li>
<li>
<b>Field removed. </b>
<code>struct inet_peer *gc_next</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 metrics[16]</code> ➡️ <code>u32 metrics[17]</code>
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
<code>u32 n_redirects</code>
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
