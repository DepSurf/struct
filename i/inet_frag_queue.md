# Struct: <code>inet_frag_queue</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct inet_frag_queue {
    spinlock_t lock;
    struct timer_list timer;
    struct hlist_node list;
    atomic_t refcnt;
    struct sk_buff *fragments;
    struct sk_buff *fragments_tail;
    ktime_t stamp;
    int len;
    int meat;
    __u8 flags;
    u16 max_size;
    struct netns_frags *net;
    struct hlist_node list_evictor;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct inet_frag_queue {
    spinlock_t lock;
    struct timer_list timer;
    struct hlist_node list;
    atomic_t refcnt;
    struct sk_buff *fragments;
    struct sk_buff *fragments_tail;
    ktime_t stamp;
    int len;
    int meat;
    __u8 flags;
    u16 max_size;
    struct netns_frags *net;
    struct hlist_node list_evictor;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct inet_frag_queue {
    spinlock_t lock;
    struct timer_list timer;
    struct hlist_node list;
    atomic_t refcnt;
    struct sk_buff *fragments;
    struct sk_buff *fragments_tail;
    ktime_t stamp;
    int len;
    int meat;
    __u8 flags;
    u16 max_size;
    struct netns_frags *net;
    struct hlist_node list_evictor;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct inet_frag_queue {
    spinlock_t lock;
    struct timer_list timer;
    struct hlist_node list;
    refcount_t refcnt;
    struct sk_buff *fragments;
    struct sk_buff *fragments_tail;
    ktime_t stamp;
    int len;
    int meat;
    __u8 flags;
    u16 max_size;
    struct netns_frags *net;
    struct hlist_node list_evictor;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct inet_frag_queue {
    spinlock_t lock;
    struct timer_list timer;
    struct hlist_node list;
    refcount_t refcnt;
    struct sk_buff *fragments;
    struct sk_buff *fragments_tail;
    ktime_t stamp;
    int len;
    int meat;
    __u8 flags;
    u16 max_size;
    struct netns_frags *net;
    struct hlist_node list_evictor;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct inet_frag_queue {
    struct rhash_head node;
    union (anon) key;
    struct timer_list timer;
    spinlock_t lock;
    refcount_t refcnt;
    struct sk_buff *fragments;
    struct sk_buff *fragments_tail;
    ktime_t stamp;
    int len;
    int meat;
    __u8 flags;
    u16 max_size;
    struct netns_frags *net;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct inet_frag_queue {
    struct rhash_head node;
    union (anon) key;
    struct timer_list timer;
    spinlock_t lock;
    refcount_t refcnt;
    struct sk_buff *fragments;
    struct rb_root rb_fragments;
    struct sk_buff *fragments_tail;
    struct sk_buff *last_run_head;
    ktime_t stamp;
    int len;
    int meat;
    __u8 flags;
    u16 max_size;
    struct netns_frags *net;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct inet_frag_queue {
    struct rhash_head node;
    union (anon) key;
    struct timer_list timer;
    spinlock_t lock;
    refcount_t refcnt;
    struct rb_root rb_fragments;
    struct sk_buff *fragments_tail;
    struct sk_buff *last_run_head;
    ktime_t stamp;
    int len;
    int meat;
    __u8 flags;
    u16 max_size;
    struct fqdir *fqdir;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct inet_frag_queue {
    struct rhash_head node;
    union (anon) key;
    struct timer_list timer;
    spinlock_t lock;
    refcount_t refcnt;
    struct rb_root rb_fragments;
    struct sk_buff *fragments_tail;
    struct sk_buff *last_run_head;
    ktime_t stamp;
    int len;
    int meat;
    __u8 flags;
    u16 max_size;
    struct fqdir *fqdir;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct inet_frag_queue {
    struct rhash_head node;
    union (anon) key;
    struct timer_list timer;
    spinlock_t lock;
    refcount_t refcnt;
    struct rb_root rb_fragments;
    struct sk_buff *fragments_tail;
    struct sk_buff *last_run_head;
    ktime_t stamp;
    int len;
    int meat;
    __u8 flags;
    u16 max_size;
    struct fqdir *fqdir;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct inet_frag_queue {
    struct rhash_head node;
    union (anon) key;
    struct timer_list timer;
    spinlock_t lock;
    refcount_t refcnt;
    struct rb_root rb_fragments;
    struct sk_buff *fragments_tail;
    struct sk_buff *last_run_head;
    ktime_t stamp;
    int len;
    int meat;
    __u8 flags;
    u16 max_size;
    struct fqdir *fqdir;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct inet_frag_queue {
    struct rhash_head node;
    union (anon) key;
    struct timer_list timer;
    spinlock_t lock;
    refcount_t refcnt;
    struct rb_root rb_fragments;
    struct sk_buff *fragments_tail;
    struct sk_buff *last_run_head;
    ktime_t stamp;
    int len;
    int meat;
    __u8 flags;
    u16 max_size;
    struct fqdir *fqdir;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct inet_frag_queue {
    struct rhash_head node;
    union (anon) key;
    struct timer_list timer;
    spinlock_t lock;
    refcount_t refcnt;
    struct rb_root rb_fragments;
    struct sk_buff *fragments_tail;
    struct sk_buff *last_run_head;
    ktime_t stamp;
    int len;
    int meat;
    __u8 flags;
    u16 max_size;
    struct fqdir *fqdir;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct inet_frag_queue {
    struct rhash_head node;
    union (anon) key;
    struct timer_list timer;
    spinlock_t lock;
    refcount_t refcnt;
    struct rb_root rb_fragments;
    struct sk_buff *fragments_tail;
    struct sk_buff *last_run_head;
    ktime_t stamp;
    int len;
    int meat;
    u8 mono_delivery_time;
    __u8 flags;
    u16 max_size;
    struct fqdir *fqdir;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct inet_frag_queue {
    struct rhash_head node;
    union (anon) key;
    struct timer_list timer;
    spinlock_t lock;
    refcount_t refcnt;
    struct rb_root rb_fragments;
    struct sk_buff *fragments_tail;
    struct sk_buff *last_run_head;
    ktime_t stamp;
    int len;
    int meat;
    u8 mono_delivery_time;
    __u8 flags;
    u16 max_size;
    struct fqdir *fqdir;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct inet_frag_queue {
    struct rhash_head node;
    union (anon) key;
    struct timer_list timer;
    spinlock_t lock;
    refcount_t refcnt;
    struct rb_root rb_fragments;
    struct sk_buff *fragments_tail;
    struct sk_buff *last_run_head;
    ktime_t stamp;
    int len;
    int meat;
    u8 mono_delivery_time;
    __u8 flags;
    u16 max_size;
    struct fqdir *fqdir;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct inet_frag_queue {
    struct rhash_head node;
    union (anon) key;
    struct timer_list timer;
    spinlock_t lock;
    refcount_t refcnt;
    struct rb_root rb_fragments;
    struct sk_buff *fragments_tail;
    struct sk_buff *last_run_head;
    ktime_t stamp;
    int len;
    int meat;
    u8 mono_delivery_time;
    __u8 flags;
    u16 max_size;
    struct fqdir *fqdir;
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
struct inet_frag_queue {
    struct rhash_head node;
    union (anon) key;
    struct timer_list timer;
    spinlock_t lock;
    refcount_t refcnt;
    struct rb_root rb_fragments;
    struct sk_buff *fragments_tail;
    struct sk_buff *last_run_head;
    ktime_t stamp;
    int len;
    int meat;
    __u8 flags;
    u16 max_size;
    struct fqdir *fqdir;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct inet_frag_queue {
    struct rhash_head node;
    union (anon) key;
    struct timer_list timer;
    spinlock_t lock;
    refcount_t refcnt;
    struct rb_root rb_fragments;
    struct sk_buff *fragments_tail;
    struct sk_buff *last_run_head;
    ktime_t stamp;
    int len;
    int meat;
    __u8 flags;
    u16 max_size;
    struct fqdir *fqdir;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct inet_frag_queue {
    struct rhash_head node;
    union (anon) key;
    struct timer_list timer;
    spinlock_t lock;
    refcount_t refcnt;
    struct rb_root rb_fragments;
    struct sk_buff *fragments_tail;
    struct sk_buff *last_run_head;
    ktime_t stamp;
    int len;
    int meat;
    __u8 flags;
    u16 max_size;
    struct fqdir *fqdir;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct inet_frag_queue {
    struct rhash_head node;
    union (anon) key;
    struct timer_list timer;
    spinlock_t lock;
    refcount_t refcnt;
    struct rb_root rb_fragments;
    struct sk_buff *fragments_tail;
    struct sk_buff *last_run_head;
    ktime_t stamp;
    int len;
    int meat;
    __u8 flags;
    u16 max_size;
    struct fqdir *fqdir;
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
struct inet_frag_queue {
    struct rhash_head node;
    union (anon) key;
    struct timer_list timer;
    spinlock_t lock;
    refcount_t refcnt;
    struct rb_root rb_fragments;
    struct sk_buff *fragments_tail;
    struct sk_buff *last_run_head;
    ktime_t stamp;
    int len;
    int meat;
    __u8 flags;
    u16 max_size;
    struct fqdir *fqdir;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct inet_frag_queue {
    struct rhash_head node;
    union (anon) key;
    struct timer_list timer;
    spinlock_t lock;
    refcount_t refcnt;
    struct rb_root rb_fragments;
    struct sk_buff *fragments_tail;
    struct sk_buff *last_run_head;
    ktime_t stamp;
    int len;
    int meat;
    __u8 flags;
    u16 max_size;
    struct fqdir *fqdir;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct inet_frag_queue {
    struct rhash_head node;
    union (anon) key;
    struct timer_list timer;
    spinlock_t lock;
    refcount_t refcnt;
    struct rb_root rb_fragments;
    struct sk_buff *fragments_tail;
    struct sk_buff *last_run_head;
    ktime_t stamp;
    int len;
    int meat;
    __u8 flags;
    u16 max_size;
    struct fqdir *fqdir;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct inet_frag_queue {
    struct rhash_head node;
    union (anon) key;
    struct timer_list timer;
    spinlock_t lock;
    refcount_t refcnt;
    struct rb_root rb_fragments;
    struct sk_buff *fragments_tail;
    struct sk_buff *last_run_head;
    ktime_t stamp;
    int len;
    int meat;
    __u8 flags;
    u16 max_size;
    struct fqdir *fqdir;
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
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct rhash_head node</code>
</li>
<li>
<b>Field added. </b>
<code>union (anon) key</code>
</li>
<li>
<b>Field added. </b>
<code>struct callback_head rcu</code>
</li>
<li>
<b>Field removed. </b>
<code>struct hlist_node list</code>
</li>
<li>
<b>Field removed. </b>
<code>struct hlist_node list_evictor</code>
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
<code>struct rb_root rb_fragments</code>
</li>
<li>
<b>Field added. </b>
<code>struct sk_buff *last_run_head</code>
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
<code>struct fqdir *fqdir</code>
</li>
<li>
<b>Field removed. </b>
<code>struct sk_buff *fragments</code>
</li>
<li>
<b>Field removed. </b>
<code>struct netns_frags *net</code>
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
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 mono_delivery_time</code>
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
