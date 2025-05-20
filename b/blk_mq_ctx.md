# Struct: <code>blk_mq_ctx</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct blk_mq_ctx {
    spinlock_t lock;
    struct list_head rq_list;
    unsigned int cpu;
    unsigned int index_hw;
    unsigned int last_tag;
    long unsigned int rq_dispatched[2];
    long unsigned int rq_merged;
    long unsigned int rq_completed[2];
    struct request_queue *queue;
    struct kobject kobj;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct blk_mq_ctx {
    spinlock_t lock;
    struct list_head rq_list;
    unsigned int cpu;
    unsigned int index_hw;
    unsigned int last_tag;
    long unsigned int rq_dispatched[2];
    long unsigned int rq_merged;
    long unsigned int rq_completed[2];
    struct request_queue *queue;
    struct kobject kobj;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct blk_mq_ctx {
    spinlock_t lock;
    struct list_head rq_list;
    unsigned int cpu;
    unsigned int index_hw;
    long unsigned int rq_dispatched[2];
    long unsigned int rq_merged;
    long unsigned int rq_completed[2];
    struct blk_rq_stat stat[2];
    struct request_queue *queue;
    struct kobject kobj;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct blk_mq_ctx {
    spinlock_t lock;
    struct list_head rq_list;
    unsigned int cpu;
    unsigned int index_hw;
    long unsigned int rq_dispatched[2];
    long unsigned int rq_merged;
    long unsigned int rq_completed[2];
    struct request_queue *queue;
    struct kobject kobj;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct blk_mq_ctx {
    spinlock_t lock;
    struct list_head rq_list;
    unsigned int cpu;
    unsigned int index_hw;
    long unsigned int rq_dispatched[2];
    long unsigned int rq_merged;
    long unsigned int rq_completed[2];
    struct request_queue *queue;
    struct kobject kobj;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct blk_mq_ctx {
    spinlock_t lock;
    struct list_head rq_list;
    unsigned int cpu;
    unsigned int index_hw;
    long unsigned int rq_dispatched[2];
    long unsigned int rq_merged;
    long unsigned int rq_completed[2];
    struct request_queue *queue;
    struct kobject kobj;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct blk_mq_ctx {
    spinlock_t lock;
    struct list_head rq_lists[3];
    unsigned int cpu;
    short unsigned int index_hw[3];
    long unsigned int rq_dispatched[2];
    long unsigned int rq_merged;
    long unsigned int rq_completed[2];
    struct request_queue *queue;
    struct blk_mq_ctxs *ctxs;
    struct kobject kobj;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct blk_mq_ctx {
    spinlock_t lock;
    struct list_head rq_lists[3];
    unsigned int cpu;
    short unsigned int index_hw[3];
    struct blk_mq_hw_ctx * hctxs[3];
    long unsigned int rq_dispatched[2];
    long unsigned int rq_merged;
    long unsigned int rq_completed[2];
    struct request_queue *queue;
    struct blk_mq_ctxs *ctxs;
    struct kobject kobj;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct blk_mq_ctx {
    spinlock_t lock;
    struct list_head rq_lists[3];
    unsigned int cpu;
    short unsigned int index_hw[3];
    struct blk_mq_hw_ctx * hctxs[3];
    long unsigned int rq_dispatched[2];
    long unsigned int rq_merged;
    long unsigned int rq_completed[2];
    struct request_queue *queue;
    struct blk_mq_ctxs *ctxs;
    struct kobject kobj;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct blk_mq_ctx {
    spinlock_t lock;
    struct list_head rq_lists[3];
    unsigned int cpu;
    short unsigned int index_hw[3];
    struct blk_mq_hw_ctx * hctxs[3];
    long unsigned int rq_dispatched[2];
    long unsigned int rq_merged;
    long unsigned int rq_completed[2];
    struct request_queue *queue;
    struct blk_mq_ctxs *ctxs;
    struct kobject kobj;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct blk_mq_ctx {
    spinlock_t lock;
    struct list_head rq_lists[3];
    unsigned int cpu;
    short unsigned int index_hw[3];
    struct blk_mq_hw_ctx * hctxs[3];
    long unsigned int rq_dispatched[2];
    long unsigned int rq_merged;
    long unsigned int rq_completed[2];
    struct request_queue *queue;
    struct blk_mq_ctxs *ctxs;
    struct kobject kobj;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct blk_mq_ctx {
    spinlock_t lock;
    struct list_head rq_lists[3];
    unsigned int cpu;
    short unsigned int index_hw[3];
    struct blk_mq_hw_ctx * hctxs[3];
    long unsigned int rq_dispatched[2];
    long unsigned int rq_merged;
    long unsigned int rq_completed[2];
    struct request_queue *queue;
    struct blk_mq_ctxs *ctxs;
    struct kobject kobj;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct blk_mq_ctx {
    spinlock_t lock;
    struct list_head rq_lists[3];
    unsigned int cpu;
    short unsigned int index_hw[3];
    struct blk_mq_hw_ctx * hctxs[3];
    long unsigned int rq_dispatched[2];
    long unsigned int rq_merged;
    long unsigned int rq_completed[2];
    struct request_queue *queue;
    struct blk_mq_ctxs *ctxs;
    struct kobject kobj;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct blk_mq_ctx {
    spinlock_t lock;
    struct list_head rq_lists[3];
    unsigned int cpu;
    short unsigned int index_hw[3];
    struct blk_mq_hw_ctx * hctxs[3];
    struct request_queue *queue;
    struct blk_mq_ctxs *ctxs;
    struct kobject kobj;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct blk_mq_ctx {
    spinlock_t lock;
    struct list_head rq_lists[3];
    unsigned int cpu;
    short unsigned int index_hw[3];
    struct blk_mq_hw_ctx * hctxs[3];
    struct request_queue *queue;
    struct blk_mq_ctxs *ctxs;
    struct kobject kobj;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct blk_mq_ctx {
    spinlock_t lock;
    struct list_head rq_lists[3];
    unsigned int cpu;
    short unsigned int index_hw[3];
    struct blk_mq_hw_ctx * hctxs[3];
    struct request_queue *queue;
    struct blk_mq_ctxs *ctxs;
    struct kobject kobj;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct blk_mq_ctx {
    spinlock_t lock;
    struct list_head rq_lists[3];
    unsigned int cpu;
    short unsigned int index_hw[3];
    struct blk_mq_hw_ctx * hctxs[3];
    struct request_queue *queue;
    struct blk_mq_ctxs *ctxs;
    struct kobject kobj;
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
struct blk_mq_ctx {
    spinlock_t lock;
    struct list_head rq_lists[3];
    unsigned int cpu;
    short unsigned int index_hw[3];
    struct blk_mq_hw_ctx * hctxs[3];
    long unsigned int rq_dispatched[2];
    long unsigned int rq_merged;
    long unsigned int rq_completed[2];
    struct request_queue *queue;
    struct blk_mq_ctxs *ctxs;
    struct kobject kobj;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct blk_mq_ctx {
    spinlock_t lock;
    struct list_head rq_lists[3];
    unsigned int cpu;
    short unsigned int index_hw[3];
    struct blk_mq_hw_ctx * hctxs[3];
    long unsigned int rq_dispatched[2];
    long unsigned int rq_merged;
    long unsigned int rq_completed[2];
    struct request_queue *queue;
    struct blk_mq_ctxs *ctxs;
    struct kobject kobj;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct blk_mq_ctx {
    spinlock_t lock;
    struct list_head rq_lists[3];
    unsigned int cpu;
    short unsigned int index_hw[3];
    struct blk_mq_hw_ctx * hctxs[3];
    long unsigned int rq_dispatched[2];
    long unsigned int rq_merged;
    long unsigned int rq_completed[2];
    struct request_queue *queue;
    struct blk_mq_ctxs *ctxs;
    struct kobject kobj;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct blk_mq_ctx {
    spinlock_t lock;
    struct list_head rq_lists[3];
    unsigned int cpu;
    short unsigned int index_hw[3];
    struct blk_mq_hw_ctx * hctxs[3];
    long unsigned int rq_dispatched[2];
    long unsigned int rq_merged;
    long unsigned int rq_completed[2];
    struct request_queue *queue;
    struct blk_mq_ctxs *ctxs;
    struct kobject kobj;
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
struct blk_mq_ctx {
    spinlock_t lock;
    struct list_head rq_lists[3];
    unsigned int cpu;
    short unsigned int index_hw[3];
    struct blk_mq_hw_ctx * hctxs[3];
    long unsigned int rq_dispatched[2];
    long unsigned int rq_merged;
    long unsigned int rq_completed[2];
    struct request_queue *queue;
    struct blk_mq_ctxs *ctxs;
    struct kobject kobj;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct blk_mq_ctx {
    spinlock_t lock;
    struct list_head rq_lists[3];
    unsigned int cpu;
    short unsigned int index_hw[3];
    struct blk_mq_hw_ctx * hctxs[3];
    long unsigned int rq_dispatched[2];
    long unsigned int rq_merged;
    long unsigned int rq_completed[2];
    struct request_queue *queue;
    struct blk_mq_ctxs *ctxs;
    struct kobject kobj;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct blk_mq_ctx {
    spinlock_t lock;
    struct list_head rq_lists[3];
    unsigned int cpu;
    short unsigned int index_hw[3];
    struct blk_mq_hw_ctx * hctxs[3];
    long unsigned int rq_dispatched[2];
    long unsigned int rq_merged;
    long unsigned int rq_completed[2];
    struct request_queue *queue;
    struct blk_mq_ctxs *ctxs;
    struct kobject kobj;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct blk_mq_ctx {
    spinlock_t lock;
    struct list_head rq_lists[3];
    unsigned int cpu;
    short unsigned int index_hw[3];
    struct blk_mq_hw_ctx * hctxs[3];
    long unsigned int rq_dispatched[2];
    long unsigned int rq_merged;
    long unsigned int rq_completed[2];
    struct request_queue *queue;
    struct blk_mq_ctxs *ctxs;
    struct kobject kobj;
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
<code>struct blk_rq_stat stat[2]</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int last_tag</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct blk_rq_stat stat[2]</code>
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
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head rq_lists[3]</code>
</li>
<li>
<b>Field added. </b>
<code>struct blk_mq_ctxs *ctxs</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head rq_list</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int index_hw</code> ➡️ <code>short unsigned int index_hw[3]</code>
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
<code>struct blk_mq_hw_ctx * hctxs[3]</code>
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
<b>Field removed. </b>
<code>long unsigned int rq_dispatched[2]</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int rq_merged</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int rq_completed[2]</code>
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
