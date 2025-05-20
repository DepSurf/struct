# Struct: <code>blk_mq_tags</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct blk_mq_tags {
    unsigned int nr_tags;
    unsigned int nr_reserved_tags;
    atomic_t active_queues;
    struct blk_mq_bitmap_tags bitmap_tags;
    struct blk_mq_bitmap_tags breserved_tags;
    struct request **rqs;
    struct list_head page_list;
    int alloc_policy;
    cpumask_var_t cpumask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct blk_mq_tags {
    unsigned int nr_tags;
    unsigned int nr_reserved_tags;
    atomic_t active_queues;
    struct blk_mq_bitmap_tags bitmap_tags;
    struct blk_mq_bitmap_tags breserved_tags;
    struct request **rqs;
    struct list_head page_list;
    int alloc_policy;
    cpumask_var_t cpumask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct blk_mq_tags {
    unsigned int nr_tags;
    unsigned int nr_reserved_tags;
    atomic_t active_queues;
    struct sbitmap_queue bitmap_tags;
    struct sbitmap_queue breserved_tags;
    struct request **rqs;
    struct list_head page_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct blk_mq_tags {
    unsigned int nr_tags;
    unsigned int nr_reserved_tags;
    atomic_t active_queues;
    struct sbitmap_queue bitmap_tags;
    struct sbitmap_queue breserved_tags;
    struct request **rqs;
    struct request **static_rqs;
    struct list_head page_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct blk_mq_tags {
    unsigned int nr_tags;
    unsigned int nr_reserved_tags;
    atomic_t active_queues;
    struct sbitmap_queue bitmap_tags;
    struct sbitmap_queue breserved_tags;
    struct request **rqs;
    struct request **static_rqs;
    struct list_head page_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct blk_mq_tags {
    unsigned int nr_tags;
    unsigned int nr_reserved_tags;
    atomic_t active_queues;
    struct sbitmap_queue bitmap_tags;
    struct sbitmap_queue breserved_tags;
    struct request **rqs;
    struct request **static_rqs;
    struct list_head page_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct blk_mq_tags {
    unsigned int nr_tags;
    unsigned int nr_reserved_tags;
    atomic_t active_queues;
    struct sbitmap_queue bitmap_tags;
    struct sbitmap_queue breserved_tags;
    struct request **rqs;
    struct request **static_rqs;
    struct list_head page_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct blk_mq_tags {
    unsigned int nr_tags;
    unsigned int nr_reserved_tags;
    atomic_t active_queues;
    struct sbitmap_queue bitmap_tags;
    struct sbitmap_queue breserved_tags;
    struct request **rqs;
    struct request **static_rqs;
    struct list_head page_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct blk_mq_tags {
    unsigned int nr_tags;
    unsigned int nr_reserved_tags;
    atomic_t active_queues;
    struct sbitmap_queue bitmap_tags;
    struct sbitmap_queue breserved_tags;
    struct request **rqs;
    struct request **static_rqs;
    struct list_head page_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct blk_mq_tags {
    unsigned int nr_tags;
    unsigned int nr_reserved_tags;
    atomic_t active_queues;
    struct sbitmap_queue bitmap_tags;
    struct sbitmap_queue breserved_tags;
    struct request **rqs;
    struct request **static_rqs;
    struct list_head page_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct blk_mq_tags {
    unsigned int nr_tags;
    unsigned int nr_reserved_tags;
    atomic_t active_queues;
    struct sbitmap_queue *bitmap_tags;
    struct sbitmap_queue *breserved_tags;
    struct sbitmap_queue __bitmap_tags;
    struct sbitmap_queue __breserved_tags;
    struct request **rqs;
    struct request **static_rqs;
    struct list_head page_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct blk_mq_tags {
    unsigned int nr_tags;
    unsigned int nr_reserved_tags;
    atomic_t active_queues;
    struct sbitmap_queue *bitmap_tags;
    struct sbitmap_queue *breserved_tags;
    struct sbitmap_queue __bitmap_tags;
    struct sbitmap_queue __breserved_tags;
    struct request **rqs;
    struct request **static_rqs;
    struct list_head page_list;
    spinlock_t lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct blk_mq_tags {
    unsigned int nr_tags;
    unsigned int nr_reserved_tags;
    atomic_t active_queues;
    struct sbitmap_queue *bitmap_tags;
    struct sbitmap_queue *breserved_tags;
    struct sbitmap_queue __bitmap_tags;
    struct sbitmap_queue __breserved_tags;
    struct request **rqs;
    struct request **static_rqs;
    struct list_head page_list;
    spinlock_t lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct blk_mq_tags {
    unsigned int nr_tags;
    unsigned int nr_reserved_tags;
    atomic_t active_queues;
    struct sbitmap_queue bitmap_tags;
    struct sbitmap_queue breserved_tags;
    struct request **rqs;
    struct request **static_rqs;
    struct list_head page_list;
    spinlock_t lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct blk_mq_tags {
    unsigned int nr_tags;
    unsigned int nr_reserved_tags;
    atomic_t active_queues;
    struct sbitmap_queue bitmap_tags;
    struct sbitmap_queue breserved_tags;
    struct request **rqs;
    struct request **static_rqs;
    struct list_head page_list;
    spinlock_t lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct blk_mq_tags {
    unsigned int nr_tags;
    unsigned int nr_reserved_tags;
    unsigned int active_queues;
    struct sbitmap_queue bitmap_tags;
    struct sbitmap_queue breserved_tags;
    struct request **rqs;
    struct request **static_rqs;
    struct list_head page_list;
    spinlock_t lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct blk_mq_tags {
    unsigned int nr_tags;
    unsigned int nr_reserved_tags;
    unsigned int active_queues;
    struct sbitmap_queue bitmap_tags;
    struct sbitmap_queue breserved_tags;
    struct request **rqs;
    struct request **static_rqs;
    struct list_head page_list;
    spinlock_t lock;
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
struct blk_mq_tags {
    unsigned int nr_tags;
    unsigned int nr_reserved_tags;
    atomic_t active_queues;
    struct sbitmap_queue bitmap_tags;
    struct sbitmap_queue breserved_tags;
    struct request **rqs;
    struct request **static_rqs;
    struct list_head page_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct blk_mq_tags {
    unsigned int nr_tags;
    unsigned int nr_reserved_tags;
    atomic_t active_queues;
    struct sbitmap_queue bitmap_tags;
    struct sbitmap_queue breserved_tags;
    struct request **rqs;
    struct request **static_rqs;
    struct list_head page_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct blk_mq_tags {
    unsigned int nr_tags;
    unsigned int nr_reserved_tags;
    atomic_t active_queues;
    struct sbitmap_queue bitmap_tags;
    struct sbitmap_queue breserved_tags;
    struct request **rqs;
    struct request **static_rqs;
    struct list_head page_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct blk_mq_tags {
    unsigned int nr_tags;
    unsigned int nr_reserved_tags;
    atomic_t active_queues;
    struct sbitmap_queue bitmap_tags;
    struct sbitmap_queue breserved_tags;
    struct request **rqs;
    struct request **static_rqs;
    struct list_head page_list;
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
struct blk_mq_tags {
    unsigned int nr_tags;
    unsigned int nr_reserved_tags;
    atomic_t active_queues;
    struct sbitmap_queue bitmap_tags;
    struct sbitmap_queue breserved_tags;
    struct request **rqs;
    struct request **static_rqs;
    struct list_head page_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct blk_mq_tags {
    unsigned int nr_tags;
    unsigned int nr_reserved_tags;
    atomic_t active_queues;
    struct sbitmap_queue bitmap_tags;
    struct sbitmap_queue breserved_tags;
    struct request **rqs;
    struct request **static_rqs;
    struct list_head page_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct blk_mq_tags {
    unsigned int nr_tags;
    unsigned int nr_reserved_tags;
    atomic_t active_queues;
    struct sbitmap_queue bitmap_tags;
    struct sbitmap_queue breserved_tags;
    struct request **rqs;
    struct request **static_rqs;
    struct list_head page_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct blk_mq_tags {
    unsigned int nr_tags;
    unsigned int nr_reserved_tags;
    atomic_t active_queues;
    struct sbitmap_queue bitmap_tags;
    struct sbitmap_queue breserved_tags;
    struct request **rqs;
    struct request **static_rqs;
    struct list_head page_list;
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
<b>Field removed. </b>
<code>int alloc_policy</code>
</li>
<li>
<b>Field removed. </b>
<code>cpumask_var_t cpumask</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct blk_mq_bitmap_tags bitmap_tags</code> ➡️ <code>struct sbitmap_queue bitmap_tags</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct blk_mq_bitmap_tags breserved_tags</code> ➡️ <code>struct sbitmap_queue breserved_tags</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct request **static_rqs</code>
</li>
</ul>
</details>
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
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct sbitmap_queue __bitmap_tags</code>
</li>
<li>
<b>Field added. </b>
<code>struct sbitmap_queue __breserved_tags</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct sbitmap_queue bitmap_tags</code> ➡️ <code>struct sbitmap_queue *bitmap_tags</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct sbitmap_queue breserved_tags</code> ➡️ <code>struct sbitmap_queue *breserved_tags</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>spinlock_t lock</code>
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
<code>struct sbitmap_queue __bitmap_tags</code>
</li>
<li>
<b>Field removed. </b>
<code>struct sbitmap_queue __breserved_tags</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct sbitmap_queue *bitmap_tags</code> ➡️ <code>struct sbitmap_queue bitmap_tags</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct sbitmap_queue *breserved_tags</code> ➡️ <code>struct sbitmap_queue breserved_tags</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>atomic_t active_queues</code> ➡️ <code>unsigned int active_queues</code>
</li>
</ul>
</details>
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
