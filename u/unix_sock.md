# Struct: <code>unix_sock</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct unix_sock {
    struct sock sk;
    struct unix_address *addr;
    struct path path;
    struct mutex readlock;
    struct sock *peer;
    struct list_head link;
    atomic_long_t inflight;
    spinlock_t lock;
    unsigned char recursion_level;
    long unsigned int gc_flags;
    struct socket_wq peer_wq;
    wait_queue_t peer_wake;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct unix_sock {
    struct sock sk;
    struct unix_address *addr;
    struct path path;
    struct mutex iolock;
    struct mutex bindlock;
    struct sock *peer;
    struct list_head link;
    atomic_long_t inflight;
    spinlock_t lock;
    unsigned char recursion_level;
    long unsigned int gc_flags;
    struct socket_wq peer_wq;
    wait_queue_t peer_wake;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct unix_sock {
    struct sock sk;
    struct unix_address *addr;
    struct path path;
    struct mutex iolock;
    struct mutex bindlock;
    struct sock *peer;
    struct list_head link;
    atomic_long_t inflight;
    spinlock_t lock;
    unsigned char recursion_level;
    long unsigned int gc_flags;
    struct socket_wq peer_wq;
    wait_queue_t peer_wake;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct unix_sock {
    struct sock sk;
    struct unix_address *addr;
    struct path path;
    struct mutex iolock;
    struct mutex bindlock;
    struct sock *peer;
    struct list_head link;
    atomic_long_t inflight;
    spinlock_t lock;
    unsigned char recursion_level;
    long unsigned int gc_flags;
    struct socket_wq peer_wq;
    wait_queue_entry_t peer_wake;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct unix_sock {
    struct sock sk;
    struct unix_address *addr;
    struct path path;
    struct mutex iolock;
    struct mutex bindlock;
    struct sock *peer;
    struct list_head link;
    atomic_long_t inflight;
    spinlock_t lock;
    long unsigned int gc_flags;
    struct socket_wq peer_wq;
    wait_queue_entry_t peer_wake;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct unix_sock {
    struct sock sk;
    struct unix_address *addr;
    struct path path;
    struct mutex iolock;
    struct mutex bindlock;
    struct sock *peer;
    struct list_head link;
    atomic_long_t inflight;
    spinlock_t lock;
    long unsigned int gc_flags;
    struct socket_wq peer_wq;
    wait_queue_entry_t peer_wake;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct unix_sock {
    struct sock sk;
    struct unix_address *addr;
    struct path path;
    struct mutex iolock;
    struct mutex bindlock;
    struct sock *peer;
    struct list_head link;
    atomic_long_t inflight;
    spinlock_t lock;
    long unsigned int gc_flags;
    struct socket_wq peer_wq;
    wait_queue_entry_t peer_wake;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct unix_sock {
    struct sock sk;
    struct unix_address *addr;
    struct path path;
    struct mutex iolock;
    struct mutex bindlock;
    struct sock *peer;
    struct list_head link;
    atomic_long_t inflight;
    spinlock_t lock;
    long unsigned int gc_flags;
    struct socket_wq peer_wq;
    wait_queue_entry_t peer_wake;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct unix_sock {
    struct sock sk;
    struct unix_address *addr;
    struct path path;
    struct mutex iolock;
    struct mutex bindlock;
    struct sock *peer;
    struct list_head link;
    atomic_long_t inflight;
    spinlock_t lock;
    long unsigned int gc_flags;
    struct socket_wq peer_wq;
    wait_queue_entry_t peer_wake;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct unix_sock {
    struct sock sk;
    struct unix_address *addr;
    struct path path;
    struct mutex iolock;
    struct mutex bindlock;
    struct sock *peer;
    struct list_head link;
    atomic_long_t inflight;
    spinlock_t lock;
    long unsigned int gc_flags;
    struct socket_wq peer_wq;
    wait_queue_entry_t peer_wake;
    struct scm_stat scm_stat;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct unix_sock {
    struct sock sk;
    struct unix_address *addr;
    struct path path;
    struct mutex iolock;
    struct mutex bindlock;
    struct sock *peer;
    struct list_head link;
    atomic_long_t inflight;
    spinlock_t lock;
    long unsigned int gc_flags;
    struct socket_wq peer_wq;
    wait_queue_entry_t peer_wake;
    struct scm_stat scm_stat;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct unix_sock {
    struct sock sk;
    struct unix_address *addr;
    struct path path;
    struct mutex iolock;
    struct mutex bindlock;
    struct sock *peer;
    struct list_head link;
    atomic_long_t inflight;
    spinlock_t lock;
    long unsigned int gc_flags;
    struct socket_wq peer_wq;
    wait_queue_entry_t peer_wake;
    struct scm_stat scm_stat;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct unix_sock {
    struct sock sk;
    struct unix_address *addr;
    struct path path;
    struct mutex iolock;
    struct mutex bindlock;
    struct sock *peer;
    struct list_head link;
    atomic_long_t inflight;
    spinlock_t lock;
    long unsigned int gc_flags;
    struct socket_wq peer_wq;
    wait_queue_entry_t peer_wake;
    struct scm_stat scm_stat;
    struct sk_buff *oob_skb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct unix_sock {
    struct sock sk;
    struct unix_address *addr;
    struct path path;
    struct mutex iolock;
    struct mutex bindlock;
    struct sock *peer;
    struct list_head link;
    atomic_long_t inflight;
    spinlock_t lock;
    long unsigned int gc_flags;
    struct socket_wq peer_wq;
    wait_queue_entry_t peer_wake;
    struct scm_stat scm_stat;
    struct sk_buff *oob_skb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct unix_sock {
    struct sock sk;
    struct unix_address *addr;
    struct path path;
    struct mutex iolock;
    struct mutex bindlock;
    struct sock *peer;
    struct list_head link;
    atomic_long_t inflight;
    spinlock_t lock;
    long unsigned int gc_flags;
    struct socket_wq peer_wq;
    wait_queue_entry_t peer_wake;
    struct scm_stat scm_stat;
    struct sk_buff *oob_skb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct unix_sock {
    struct sock sk;
    struct unix_address *addr;
    struct path path;
    struct mutex iolock;
    struct mutex bindlock;
    struct sock *peer;
    struct list_head link;
    atomic_long_t inflight;
    spinlock_t lock;
    long unsigned int gc_flags;
    struct socket_wq peer_wq;
    wait_queue_entry_t peer_wake;
    struct scm_stat scm_stat;
    struct sk_buff *oob_skb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct unix_sock {
    struct sock sk;
    struct unix_address *addr;
    struct path path;
    struct mutex iolock;
    struct mutex bindlock;
    struct sock *peer;
    struct list_head link;
    atomic_long_t inflight;
    spinlock_t lock;
    long unsigned int gc_flags;
    struct socket_wq peer_wq;
    wait_queue_entry_t peer_wake;
    struct scm_stat scm_stat;
    struct sk_buff *oob_skb;
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
struct unix_sock {
    struct sock sk;
    struct unix_address *addr;
    struct path path;
    struct mutex iolock;
    struct mutex bindlock;
    struct sock *peer;
    struct list_head link;
    atomic_long_t inflight;
    spinlock_t lock;
    long unsigned int gc_flags;
    struct socket_wq peer_wq;
    wait_queue_entry_t peer_wake;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct unix_sock {
    struct sock sk;
    struct unix_address *addr;
    struct path path;
    struct mutex iolock;
    struct mutex bindlock;
    struct sock *peer;
    struct list_head link;
    atomic_long_t inflight;
    spinlock_t lock;
    long unsigned int gc_flags;
    struct socket_wq peer_wq;
    wait_queue_entry_t peer_wake;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct unix_sock {
    struct sock sk;
    struct unix_address *addr;
    struct path path;
    struct mutex iolock;
    struct mutex bindlock;
    struct sock *peer;
    struct list_head link;
    atomic_long_t inflight;
    spinlock_t lock;
    long unsigned int gc_flags;
    struct socket_wq peer_wq;
    wait_queue_entry_t peer_wake;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct unix_sock {
    struct sock sk;
    struct unix_address *addr;
    struct path path;
    struct mutex iolock;
    struct mutex bindlock;
    struct sock *peer;
    struct list_head link;
    atomic_long_t inflight;
    spinlock_t lock;
    long unsigned int gc_flags;
    struct socket_wq peer_wq;
    wait_queue_entry_t peer_wake;
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
struct unix_sock {
    struct sock sk;
    struct unix_address *addr;
    struct path path;
    struct mutex iolock;
    struct mutex bindlock;
    struct sock *peer;
    struct list_head link;
    atomic_long_t inflight;
    spinlock_t lock;
    long unsigned int gc_flags;
    struct socket_wq peer_wq;
    wait_queue_entry_t peer_wake;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct unix_sock {
    struct sock sk;
    struct unix_address *addr;
    struct path path;
    struct mutex iolock;
    struct mutex bindlock;
    struct sock *peer;
    struct list_head link;
    atomic_long_t inflight;
    spinlock_t lock;
    long unsigned int gc_flags;
    struct socket_wq peer_wq;
    wait_queue_entry_t peer_wake;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct unix_sock {
    struct sock sk;
    struct unix_address *addr;
    struct path path;
    struct mutex iolock;
    struct mutex bindlock;
    struct sock *peer;
    struct list_head link;
    atomic_long_t inflight;
    spinlock_t lock;
    long unsigned int gc_flags;
    struct socket_wq peer_wq;
    wait_queue_entry_t peer_wake;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct unix_sock {
    struct sock sk;
    struct unix_address *addr;
    struct path path;
    struct mutex iolock;
    struct mutex bindlock;
    struct sock *peer;
    struct list_head link;
    atomic_long_t inflight;
    spinlock_t lock;
    long unsigned int gc_flags;
    struct socket_wq peer_wq;
    wait_queue_entry_t peer_wake;
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
<code>struct mutex iolock</code>
</li>
<li>
<b>Field added. </b>
<code>struct mutex bindlock</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mutex readlock</code>
</li>
</ul>
</details>
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
<code>wait_queue_t peer_wake</code> ➡️ <code>wait_queue_entry_t peer_wake</code>
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
<code>unsigned char recursion_level</code>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct scm_stat scm_stat</code>
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
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct sk_buff *oob_skb</code>
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
