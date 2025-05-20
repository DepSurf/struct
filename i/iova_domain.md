# Struct: <code>iova_domain</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct iova_domain {
    spinlock_t iova_rbtree_lock;
    struct rb_root rbroot;
    struct rb_node *cached32_node;
    long unsigned int granule;
    long unsigned int start_pfn;
    long unsigned int dma_32bit_pfn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct iova_domain {
    spinlock_t iova_rbtree_lock;
    struct rb_root rbroot;
    struct rb_node *cached32_node;
    long unsigned int granule;
    long unsigned int start_pfn;
    long unsigned int dma_32bit_pfn;
    struct iova_rcache rcaches[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct iova_domain {
    spinlock_t iova_rbtree_lock;
    struct rb_root rbroot;
    struct rb_node *cached32_node;
    long unsigned int granule;
    long unsigned int start_pfn;
    long unsigned int dma_32bit_pfn;
    struct iova_rcache rcaches[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct iova_domain {
    spinlock_t iova_rbtree_lock;
    struct rb_root rbroot;
    struct rb_node *cached32_node;
    long unsigned int granule;
    long unsigned int start_pfn;
    long unsigned int dma_32bit_pfn;
    struct iova_rcache rcaches[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct iova_domain {
    spinlock_t iova_rbtree_lock;
    struct rb_root rbroot;
    struct rb_node *cached_node;
    struct rb_node *cached32_node;
    long unsigned int granule;
    long unsigned int start_pfn;
    long unsigned int dma_32bit_pfn;
    struct iova anchor;
    struct iova_rcache rcaches[6];
    iova_flush_cb flush_cb;
    iova_entry_dtor entry_dtor;
    struct iova_fq *fq;
    atomic64_t fq_flush_start_cnt;
    atomic64_t fq_flush_finish_cnt;
    struct timer_list fq_timer;
    atomic_t fq_timer_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct iova_domain {
    spinlock_t iova_rbtree_lock;
    struct rb_root rbroot;
    struct rb_node *cached_node;
    struct rb_node *cached32_node;
    long unsigned int granule;
    long unsigned int start_pfn;
    long unsigned int dma_32bit_pfn;
    struct iova anchor;
    struct iova_rcache rcaches[6];
    iova_flush_cb flush_cb;
    iova_entry_dtor entry_dtor;
    struct iova_fq *fq;
    atomic64_t fq_flush_start_cnt;
    atomic64_t fq_flush_finish_cnt;
    struct timer_list fq_timer;
    atomic_t fq_timer_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct iova_domain {
    spinlock_t iova_rbtree_lock;
    struct rb_root rbroot;
    struct rb_node *cached_node;
    struct rb_node *cached32_node;
    long unsigned int granule;
    long unsigned int start_pfn;
    long unsigned int dma_32bit_pfn;
    long unsigned int max32_alloc_size;
    struct iova anchor;
    struct iova_rcache rcaches[6];
    iova_flush_cb flush_cb;
    iova_entry_dtor entry_dtor;
    struct iova_fq *fq;
    atomic64_t fq_flush_start_cnt;
    atomic64_t fq_flush_finish_cnt;
    struct timer_list fq_timer;
    atomic_t fq_timer_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct iova_domain {
    spinlock_t iova_rbtree_lock;
    struct rb_root rbroot;
    struct rb_node *cached_node;
    struct rb_node *cached32_node;
    long unsigned int granule;
    long unsigned int start_pfn;
    long unsigned int dma_32bit_pfn;
    long unsigned int max32_alloc_size;
    struct iova_fq *fq;
    atomic64_t fq_flush_start_cnt;
    atomic64_t fq_flush_finish_cnt;
    struct iova anchor;
    struct iova_rcache rcaches[6];
    iova_flush_cb flush_cb;
    iova_entry_dtor entry_dtor;
    struct timer_list fq_timer;
    atomic_t fq_timer_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct iova_domain {
    spinlock_t iova_rbtree_lock;
    struct rb_root rbroot;
    struct rb_node *cached_node;
    struct rb_node *cached32_node;
    long unsigned int granule;
    long unsigned int start_pfn;
    long unsigned int dma_32bit_pfn;
    long unsigned int max32_alloc_size;
    struct iova_fq *fq;
    atomic64_t fq_flush_start_cnt;
    atomic64_t fq_flush_finish_cnt;
    struct iova anchor;
    struct iova_rcache rcaches[6];
    iova_flush_cb flush_cb;
    iova_entry_dtor entry_dtor;
    struct timer_list fq_timer;
    atomic_t fq_timer_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct iova_domain {
    spinlock_t iova_rbtree_lock;
    struct rb_root rbroot;
    struct rb_node *cached_node;
    struct rb_node *cached32_node;
    long unsigned int granule;
    long unsigned int start_pfn;
    long unsigned int dma_32bit_pfn;
    long unsigned int max32_alloc_size;
    struct iova_fq *fq;
    atomic64_t fq_flush_start_cnt;
    atomic64_t fq_flush_finish_cnt;
    struct iova anchor;
    struct iova_rcache rcaches[6];
    iova_flush_cb flush_cb;
    iova_entry_dtor entry_dtor;
    struct timer_list fq_timer;
    atomic_t fq_timer_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct iova_domain {
    spinlock_t iova_rbtree_lock;
    struct rb_root rbroot;
    struct rb_node *cached_node;
    struct rb_node *cached32_node;
    long unsigned int granule;
    long unsigned int start_pfn;
    long unsigned int dma_32bit_pfn;
    long unsigned int max32_alloc_size;
    struct iova_fq *fq;
    atomic64_t fq_flush_start_cnt;
    atomic64_t fq_flush_finish_cnt;
    struct iova anchor;
    struct iova_rcache rcaches[6];
    iova_flush_cb flush_cb;
    iova_entry_dtor entry_dtor;
    struct timer_list fq_timer;
    atomic_t fq_timer_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct iova_domain {
    spinlock_t iova_rbtree_lock;
    struct rb_root rbroot;
    struct rb_node *cached_node;
    struct rb_node *cached32_node;
    long unsigned int granule;
    long unsigned int start_pfn;
    long unsigned int dma_32bit_pfn;
    long unsigned int max32_alloc_size;
    struct iova_fq *fq;
    atomic64_t fq_flush_start_cnt;
    atomic64_t fq_flush_finish_cnt;
    struct iova anchor;
    struct iova_rcache rcaches[6];
    iova_flush_cb flush_cb;
    iova_entry_dtor entry_dtor;
    struct timer_list fq_timer;
    atomic_t fq_timer_on;
    struct hlist_node cpuhp_dead;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct iova_domain {
    spinlock_t iova_rbtree_lock;
    struct rb_root rbroot;
    struct rb_node *cached_node;
    struct rb_node *cached32_node;
    long unsigned int granule;
    long unsigned int start_pfn;
    long unsigned int dma_32bit_pfn;
    long unsigned int max32_alloc_size;
    struct iova_fq *fq;
    atomic64_t fq_flush_start_cnt;
    atomic64_t fq_flush_finish_cnt;
    struct iova anchor;
    struct iova_rcache rcaches[6];
    iova_flush_cb flush_cb;
    iova_entry_dtor entry_dtor;
    struct timer_list fq_timer;
    atomic_t fq_timer_on;
    struct hlist_node cpuhp_dead;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct iova_domain {
    spinlock_t iova_rbtree_lock;
    struct rb_root rbroot;
    struct rb_node *cached_node;
    struct rb_node *cached32_node;
    long unsigned int granule;
    long unsigned int start_pfn;
    long unsigned int dma_32bit_pfn;
    long unsigned int max32_alloc_size;
    struct iova anchor;
    struct iova_rcache *rcaches;
    struct hlist_node cpuhp_dead;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct iova_domain {
    spinlock_t iova_rbtree_lock;
    struct rb_root rbroot;
    struct rb_node *cached_node;
    struct rb_node *cached32_node;
    long unsigned int granule;
    long unsigned int start_pfn;
    long unsigned int dma_32bit_pfn;
    long unsigned int max32_alloc_size;
    struct iova anchor;
    struct iova_rcache *rcaches;
    struct hlist_node cpuhp_dead;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct iova_domain {
    spinlock_t iova_rbtree_lock;
    struct rb_root rbroot;
    struct rb_node *cached_node;
    struct rb_node *cached32_node;
    long unsigned int granule;
    long unsigned int start_pfn;
    long unsigned int dma_32bit_pfn;
    long unsigned int max32_alloc_size;
    struct iova anchor;
    struct iova_rcache *rcaches;
    struct hlist_node cpuhp_dead;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct iova_domain {
    spinlock_t iova_rbtree_lock;
    struct rb_root rbroot;
    struct rb_node *cached_node;
    struct rb_node *cached32_node;
    long unsigned int granule;
    long unsigned int start_pfn;
    long unsigned int dma_32bit_pfn;
    long unsigned int max32_alloc_size;
    struct iova anchor;
    struct iova_rcache *rcaches;
    struct hlist_node cpuhp_dead;
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
struct iova_domain {
    spinlock_t iova_rbtree_lock;
    struct rb_root rbroot;
    struct rb_node *cached_node;
    struct rb_node *cached32_node;
    long unsigned int granule;
    long unsigned int start_pfn;
    long unsigned int dma_32bit_pfn;
    long unsigned int max32_alloc_size;
    struct iova_fq *fq;
    atomic64_t fq_flush_start_cnt;
    atomic64_t fq_flush_finish_cnt;
    struct iova anchor;
    struct iova_rcache rcaches[6];
    iova_flush_cb flush_cb;
    iova_entry_dtor entry_dtor;
    struct timer_list fq_timer;
    atomic_t fq_timer_on;
};
```
</details>
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
</li>
<li>
In <code>riscv64</code>: Absent ⚠️
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct iova_domain {
    spinlock_t iova_rbtree_lock;
    struct rb_root rbroot;
    struct rb_node *cached_node;
    struct rb_node *cached32_node;
    long unsigned int granule;
    long unsigned int start_pfn;
    long unsigned int dma_32bit_pfn;
    long unsigned int max32_alloc_size;
    struct iova_fq *fq;
    atomic64_t fq_flush_start_cnt;
    atomic64_t fq_flush_finish_cnt;
    struct iova anchor;
    struct iova_rcache rcaches[6];
    iova_flush_cb flush_cb;
    iova_entry_dtor entry_dtor;
    struct timer_list fq_timer;
    atomic_t fq_timer_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct iova_domain {
    spinlock_t iova_rbtree_lock;
    struct rb_root rbroot;
    struct rb_node *cached_node;
    struct rb_node *cached32_node;
    long unsigned int granule;
    long unsigned int start_pfn;
    long unsigned int dma_32bit_pfn;
    long unsigned int max32_alloc_size;
    struct iova_fq *fq;
    atomic64_t fq_flush_start_cnt;
    atomic64_t fq_flush_finish_cnt;
    struct iova anchor;
    struct iova_rcache rcaches[6];
    iova_flush_cb flush_cb;
    iova_entry_dtor entry_dtor;
    struct timer_list fq_timer;
    atomic_t fq_timer_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct iova_domain {
    spinlock_t iova_rbtree_lock;
    struct rb_root rbroot;
    struct rb_node *cached_node;
    struct rb_node *cached32_node;
    long unsigned int granule;
    long unsigned int start_pfn;
    long unsigned int dma_32bit_pfn;
    long unsigned int max32_alloc_size;
    struct iova_fq *fq;
    atomic64_t fq_flush_start_cnt;
    atomic64_t fq_flush_finish_cnt;
    struct iova anchor;
    struct iova_rcache rcaches[6];
    iova_flush_cb flush_cb;
    iova_entry_dtor entry_dtor;
    struct timer_list fq_timer;
    atomic_t fq_timer_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct iova_domain {
    spinlock_t iova_rbtree_lock;
    struct rb_root rbroot;
    struct rb_node *cached_node;
    struct rb_node *cached32_node;
    long unsigned int granule;
    long unsigned int start_pfn;
    long unsigned int dma_32bit_pfn;
    long unsigned int max32_alloc_size;
    struct iova_fq *fq;
    atomic64_t fq_flush_start_cnt;
    atomic64_t fq_flush_finish_cnt;
    struct iova anchor;
    struct iova_rcache rcaches[6];
    iova_flush_cb flush_cb;
    iova_entry_dtor entry_dtor;
    struct timer_list fq_timer;
    atomic_t fq_timer_on;
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
<code>struct iova_rcache rcaches[6]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
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
<code>struct rb_node *cached_node</code>
</li>
<li>
<b>Field added. </b>
<code>struct iova anchor</code>
</li>
<li>
<b>Field added. </b>
<code>iova_flush_cb flush_cb</code>
</li>
<li>
<b>Field added. </b>
<code>iova_entry_dtor entry_dtor</code>
</li>
<li>
<b>Field added. </b>
<code>struct iova_fq *fq</code>
</li>
<li>
<b>Field added. </b>
<code>atomic64_t fq_flush_start_cnt</code>
</li>
<li>
<b>Field added. </b>
<code>atomic64_t fq_flush_finish_cnt</code>
</li>
<li>
<b>Field added. </b>
<code>struct timer_list fq_timer</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t fq_timer_on</code>
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
<code>long unsigned int max32_alloc_size</code>
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
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct hlist_node cpuhp_dead</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct iova_fq *fq</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic64_t fq_flush_start_cnt</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic64_t fq_flush_finish_cnt</code>
</li>
<li>
<b>Field removed. </b>
<code>iova_flush_cb flush_cb</code>
</li>
<li>
<b>Field removed. </b>
<code>iova_entry_dtor entry_dtor</code>
</li>
<li>
<b>Field removed. </b>
<code>struct timer_list fq_timer</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t fq_timer_on</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct iova_rcache rcaches[6]</code> ➡️ <code>struct iova_rcache *rcaches</code>
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
