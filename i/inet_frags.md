# Struct: <code>inet_frags</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct inet_frags {
    struct inet_frag_bucket hash[1024];
    struct work_struct frags_work;
    unsigned int next_bucket;
    long unsigned int last_rebuild_jiffies;
    bool rebuild;
    u32 rnd;
    seqlock_t rnd_seqlock;
    int qsize;
    unsigned int (*hashfn)(const struct inet_frag_queue *);
    bool (*match)(const struct inet_frag_queue *, const void *);
    void (*constructor)(struct inet_frag_queue *, const void *);
    void (*destructor)(struct inet_frag_queue *);
    void (*skb_free)(struct sk_buff *);
    void (*frag_expire)(long unsigned int);
    struct kmem_cache *frags_cachep;
    const char *frags_cache_name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct inet_frags {
    struct inet_frag_bucket hash[1024];
    struct work_struct frags_work;
    unsigned int next_bucket;
    long unsigned int last_rebuild_jiffies;
    bool rebuild;
    u32 rnd;
    seqlock_t rnd_seqlock;
    int qsize;
    unsigned int (*hashfn)(const struct inet_frag_queue *);
    bool (*match)(const struct inet_frag_queue *, const void *);
    void (*constructor)(struct inet_frag_queue *, const void *);
    void (*destructor)(struct inet_frag_queue *);
    void (*frag_expire)(long unsigned int);
    struct kmem_cache *frags_cachep;
    const char *frags_cache_name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct inet_frags {
    struct inet_frag_bucket hash[1024];
    struct work_struct frags_work;
    unsigned int next_bucket;
    long unsigned int last_rebuild_jiffies;
    bool rebuild;
    u32 rnd;
    seqlock_t rnd_seqlock;
    int qsize;
    unsigned int (*hashfn)(const struct inet_frag_queue *);
    bool (*match)(const struct inet_frag_queue *, const void *);
    void (*constructor)(struct inet_frag_queue *, const void *);
    void (*destructor)(struct inet_frag_queue *);
    void (*frag_expire)(long unsigned int);
    struct kmem_cache *frags_cachep;
    const char *frags_cache_name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct inet_frags {
    struct inet_frag_bucket hash[1024];
    struct work_struct frags_work;
    unsigned int next_bucket;
    long unsigned int last_rebuild_jiffies;
    bool rebuild;
    u32 rnd;
    seqlock_t rnd_seqlock;
    unsigned int qsize;
    unsigned int (*hashfn)(const struct inet_frag_queue *);
    bool (*match)(const struct inet_frag_queue *, const void *);
    void (*constructor)(struct inet_frag_queue *, const void *);
    void (*destructor)(struct inet_frag_queue *);
    void (*frag_expire)(long unsigned int);
    struct kmem_cache *frags_cachep;
    const char *frags_cache_name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct inet_frags {
    struct inet_frag_bucket hash[1024];
    struct work_struct frags_work;
    unsigned int next_bucket;
    long unsigned int last_rebuild_jiffies;
    bool rebuild;
    u32 rnd;
    seqlock_t rnd_seqlock;
    unsigned int qsize;
    unsigned int (*hashfn)(const struct inet_frag_queue *);
    bool (*match)(const struct inet_frag_queue *, const void *);
    void (*constructor)(struct inet_frag_queue *, const void *);
    void (*destructor)(struct inet_frag_queue *);
    void (*frag_expire)(struct timer_list *);
    struct kmem_cache *frags_cachep;
    const char *frags_cache_name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct inet_frags {
    unsigned int qsize;
    void (*constructor)(struct inet_frag_queue *, const void *);
    void (*destructor)(struct inet_frag_queue *);
    void (*frag_expire)(struct timer_list *);
    struct kmem_cache *frags_cachep;
    const char *frags_cache_name;
    struct rhashtable_params rhash_params;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct inet_frags {
    unsigned int qsize;
    void (*constructor)(struct inet_frag_queue *, const void *);
    void (*destructor)(struct inet_frag_queue *);
    void (*frag_expire)(struct timer_list *);
    struct kmem_cache *frags_cachep;
    const char *frags_cache_name;
    struct rhashtable_params rhash_params;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct inet_frags {
    unsigned int qsize;
    void (*constructor)(struct inet_frag_queue *, const void *);
    void (*destructor)(struct inet_frag_queue *);
    void (*frag_expire)(struct timer_list *);
    struct kmem_cache *frags_cachep;
    const char *frags_cache_name;
    struct rhashtable_params rhash_params;
    refcount_t refcnt;
    struct completion completion;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct inet_frags {
    unsigned int qsize;
    void (*constructor)(struct inet_frag_queue *, const void *);
    void (*destructor)(struct inet_frag_queue *);
    void (*frag_expire)(struct timer_list *);
    struct kmem_cache *frags_cachep;
    const char *frags_cache_name;
    struct rhashtable_params rhash_params;
    refcount_t refcnt;
    struct completion completion;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct inet_frags {
    unsigned int qsize;
    void (*constructor)(struct inet_frag_queue *, const void *);
    void (*destructor)(struct inet_frag_queue *);
    void (*frag_expire)(struct timer_list *);
    struct kmem_cache *frags_cachep;
    const char *frags_cache_name;
    struct rhashtable_params rhash_params;
    refcount_t refcnt;
    struct completion completion;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct inet_frags {
    unsigned int qsize;
    void (*constructor)(struct inet_frag_queue *, const void *);
    void (*destructor)(struct inet_frag_queue *);
    void (*frag_expire)(struct timer_list *);
    struct kmem_cache *frags_cachep;
    const char *frags_cache_name;
    struct rhashtable_params rhash_params;
    refcount_t refcnt;
    struct completion completion;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct inet_frags {
    unsigned int qsize;
    void (*constructor)(struct inet_frag_queue *, const void *);
    void (*destructor)(struct inet_frag_queue *);
    void (*frag_expire)(struct timer_list *);
    struct kmem_cache *frags_cachep;
    const char *frags_cache_name;
    struct rhashtable_params rhash_params;
    refcount_t refcnt;
    struct completion completion;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct inet_frags {
    unsigned int qsize;
    void (*constructor)(struct inet_frag_queue *, const void *);
    void (*destructor)(struct inet_frag_queue *);
    void (*frag_expire)(struct timer_list *);
    struct kmem_cache *frags_cachep;
    const char *frags_cache_name;
    struct rhashtable_params rhash_params;
    refcount_t refcnt;
    struct completion completion;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct inet_frags {
    unsigned int qsize;
    void (*constructor)(struct inet_frag_queue *, const void *);
    void (*destructor)(struct inet_frag_queue *);
    void (*frag_expire)(struct timer_list *);
    struct kmem_cache *frags_cachep;
    const char *frags_cache_name;
    struct rhashtable_params rhash_params;
    refcount_t refcnt;
    struct completion completion;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct inet_frags {
    unsigned int qsize;
    void (*constructor)(struct inet_frag_queue *, const void *);
    void (*destructor)(struct inet_frag_queue *);
    void (*frag_expire)(struct timer_list *);
    struct kmem_cache *frags_cachep;
    const char *frags_cache_name;
    struct rhashtable_params rhash_params;
    refcount_t refcnt;
    struct completion completion;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct inet_frags {
    unsigned int qsize;
    void (*constructor)(struct inet_frag_queue *, const void *);
    void (*destructor)(struct inet_frag_queue *);
    void (*frag_expire)(struct timer_list *);
    struct kmem_cache *frags_cachep;
    const char *frags_cache_name;
    struct rhashtable_params rhash_params;
    refcount_t refcnt;
    struct completion completion;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct inet_frags {
    unsigned int qsize;
    void (*constructor)(struct inet_frag_queue *, const void *);
    void (*destructor)(struct inet_frag_queue *);
    void (*frag_expire)(struct timer_list *);
    struct kmem_cache *frags_cachep;
    const char *frags_cache_name;
    struct rhashtable_params rhash_params;
    refcount_t refcnt;
    struct completion completion;
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
struct inet_frags {
    unsigned int qsize;
    void (*constructor)(struct inet_frag_queue *, const void *);
    void (*destructor)(struct inet_frag_queue *);
    void (*frag_expire)(struct timer_list *);
    struct kmem_cache *frags_cachep;
    const char *frags_cache_name;
    struct rhashtable_params rhash_params;
    refcount_t refcnt;
    struct completion completion;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct inet_frags {
    unsigned int qsize;
    void (*constructor)(struct inet_frag_queue *, const void *);
    void (*destructor)(struct inet_frag_queue *);
    void (*frag_expire)(struct timer_list *);
    struct kmem_cache *frags_cachep;
    const char *frags_cache_name;
    struct rhashtable_params rhash_params;
    refcount_t refcnt;
    struct completion completion;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct inet_frags {
    unsigned int qsize;
    void (*constructor)(struct inet_frag_queue *, const void *);
    void (*destructor)(struct inet_frag_queue *);
    void (*frag_expire)(struct timer_list *);
    struct kmem_cache *frags_cachep;
    const char *frags_cache_name;
    struct rhashtable_params rhash_params;
    refcount_t refcnt;
    struct completion completion;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct inet_frags {
    unsigned int qsize;
    void (*constructor)(struct inet_frag_queue *, const void *);
    void (*destructor)(struct inet_frag_queue *);
    void (*frag_expire)(struct timer_list *);
    struct kmem_cache *frags_cachep;
    const char *frags_cache_name;
    struct rhashtable_params rhash_params;
    refcount_t refcnt;
    struct completion completion;
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
struct inet_frags {
    unsigned int qsize;
    void (*constructor)(struct inet_frag_queue *, const void *);
    void (*destructor)(struct inet_frag_queue *);
    void (*frag_expire)(struct timer_list *);
    struct kmem_cache *frags_cachep;
    const char *frags_cache_name;
    struct rhashtable_params rhash_params;
    refcount_t refcnt;
    struct completion completion;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct inet_frags {
    unsigned int qsize;
    void (*constructor)(struct inet_frag_queue *, const void *);
    void (*destructor)(struct inet_frag_queue *);
    void (*frag_expire)(struct timer_list *);
    struct kmem_cache *frags_cachep;
    const char *frags_cache_name;
    struct rhashtable_params rhash_params;
    refcount_t refcnt;
    struct completion completion;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct inet_frags {
    unsigned int qsize;
    void (*constructor)(struct inet_frag_queue *, const void *);
    void (*destructor)(struct inet_frag_queue *);
    void (*frag_expire)(struct timer_list *);
    struct kmem_cache *frags_cachep;
    const char *frags_cache_name;
    struct rhashtable_params rhash_params;
    refcount_t refcnt;
    struct completion completion;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct inet_frags {
    unsigned int qsize;
    void (*constructor)(struct inet_frag_queue *, const void *);
    void (*destructor)(struct inet_frag_queue *);
    void (*frag_expire)(struct timer_list *);
    struct kmem_cache *frags_cachep;
    const char *frags_cache_name;
    struct rhashtable_params rhash_params;
    refcount_t refcnt;
    struct completion completion;
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
<code>void (*skb_free)(struct sk_buff *)</code>
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
<code>int qsize</code> ➡️ <code>unsigned int qsize</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>void (*frag_expire)(long unsigned int)</code> ➡️ <code>void (*frag_expire)(struct timer_list *)</code>
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
<code>struct rhashtable_params rhash_params</code>
</li>
<li>
<b>Field removed. </b>
<code>struct inet_frag_bucket hash[1024]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct work_struct frags_work</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int next_bucket</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int last_rebuild_jiffies</code>
</li>
<li>
<b>Field removed. </b>
<code>bool rebuild</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 rnd</code>
</li>
<li>
<b>Field removed. </b>
<code>seqlock_t rnd_seqlock</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int (*hashfn)(const struct inet_frag_queue *)</code>
</li>
<li>
<b>Field removed. </b>
<code>bool (*match)(const struct inet_frag_queue *, const void *)</code>
</li>
</ul>
</details>
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
<code>refcount_t refcnt</code>
</li>
<li>
<b>Field added. </b>
<code>struct completion completion</code>
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
