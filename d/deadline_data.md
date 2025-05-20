# Struct: <code>deadline_data</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct deadline_data {
    struct rb_root sort_list[2];
    struct list_head fifo_list[2];
    struct request * next_rq[2];
    unsigned int batching;
    sector_t last_sector;
    unsigned int starved;
    int fifo_expire[2];
    int fifo_batch;
    int writes_starved;
    int front_merges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct deadline_data {
    struct rb_root sort_list[2];
    struct list_head fifo_list[2];
    struct request * next_rq[2];
    unsigned int batching;
    unsigned int starved;
    int fifo_expire[2];
    int fifo_batch;
    int writes_starved;
    int front_merges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct deadline_data {
    struct rb_root sort_list[2];
    struct list_head fifo_list[2];
    struct request * next_rq[2];
    unsigned int batching;
    unsigned int starved;
    int fifo_expire[2];
    int fifo_batch;
    int writes_starved;
    int front_merges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct deadline_data {
    struct rb_root sort_list[2];
    struct list_head fifo_list[2];
    struct request * next_rq[2];
    unsigned int batching;
    unsigned int starved;
    int fifo_expire[2];
    int fifo_batch;
    int writes_starved;
    int front_merges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct deadline_data {
    struct rb_root sort_list[2];
    struct list_head fifo_list[2];
    struct request * next_rq[2];
    unsigned int batching;
    unsigned int starved;
    int fifo_expire[2];
    int fifo_batch;
    int writes_starved;
    int front_merges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct deadline_data {
    struct rb_root sort_list[2];
    struct list_head fifo_list[2];
    struct request * next_rq[2];
    unsigned int batching;
    unsigned int starved;
    int fifo_expire[2];
    int fifo_batch;
    int writes_starved;
    int front_merges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct deadline_data {
    struct rb_root sort_list[2];
    struct list_head fifo_list[2];
    struct request * next_rq[2];
    unsigned int batching;
    unsigned int starved;
    int fifo_expire[2];
    int fifo_batch;
    int writes_starved;
    int front_merges;
    spinlock_t lock;
    spinlock_t zone_lock;
    struct list_head dispatch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct deadline_data {
    struct rb_root sort_list[2];
    struct list_head fifo_list[2];
    struct request * next_rq[2];
    unsigned int batching;
    unsigned int starved;
    int fifo_expire[2];
    int fifo_batch;
    int writes_starved;
    int front_merges;
    spinlock_t lock;
    spinlock_t zone_lock;
    struct list_head dispatch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct deadline_data {
    struct rb_root sort_list[2];
    struct list_head fifo_list[2];
    struct request * next_rq[2];
    unsigned int batching;
    unsigned int starved;
    int fifo_expire[2];
    int fifo_batch;
    int writes_starved;
    int front_merges;
    spinlock_t lock;
    spinlock_t zone_lock;
    struct list_head dispatch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct deadline_data {
    struct rb_root sort_list[2];
    struct list_head fifo_list[2];
    struct request * next_rq[2];
    unsigned int batching;
    unsigned int starved;
    int fifo_expire[2];
    int fifo_batch;
    int writes_starved;
    int front_merges;
    spinlock_t lock;
    spinlock_t zone_lock;
    struct list_head dispatch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct deadline_data {
    struct rb_root sort_list[2];
    struct list_head fifo_list[2];
    struct request * next_rq[2];
    unsigned int batching;
    unsigned int starved;
    int fifo_expire[2];
    int fifo_batch;
    int writes_starved;
    int front_merges;
    spinlock_t lock;
    spinlock_t zone_lock;
    struct list_head dispatch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct deadline_data {
    struct rb_root sort_list[2];
    struct list_head fifo_list[2];
    struct request * next_rq[2];
    unsigned int batching;
    unsigned int starved;
    int fifo_expire[2];
    int fifo_batch;
    int writes_starved;
    int front_merges;
    spinlock_t lock;
    spinlock_t zone_lock;
    struct list_head dispatch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct deadline_data {
    struct dd_per_prio per_prio[3];
    enum dd_data_dir last_dir;
    unsigned int batching;
    unsigned int starved;
    struct io_stats *stats;
    int fifo_expire[2];
    int fifo_batch;
    int writes_starved;
    int front_merges;
    u32 async_depth;
    spinlock_t lock;
    spinlock_t zone_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct deadline_data {
    struct dd_per_prio per_prio[3];
    enum dd_data_dir last_dir;
    unsigned int batching;
    unsigned int starved;
    int fifo_expire[2];
    int fifo_batch;
    int writes_starved;
    int front_merges;
    u32 async_depth;
    int prio_aging_expire;
    spinlock_t lock;
    spinlock_t zone_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct deadline_data {
    struct dd_per_prio per_prio[3];
    enum dd_data_dir last_dir;
    unsigned int batching;
    unsigned int starved;
    int fifo_expire[2];
    int fifo_batch;
    int writes_starved;
    int front_merges;
    u32 async_depth;
    int prio_aging_expire;
    spinlock_t lock;
    spinlock_t zone_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct deadline_data {
    struct dd_per_prio per_prio[3];
    enum dd_data_dir last_dir;
    unsigned int batching;
    unsigned int starved;
    int fifo_expire[2];
    int fifo_batch;
    int writes_starved;
    int front_merges;
    u32 async_depth;
    int prio_aging_expire;
    spinlock_t lock;
    spinlock_t zone_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct deadline_data {
    struct dd_per_prio per_prio[3];
    enum dd_data_dir last_dir;
    unsigned int batching;
    unsigned int starved;
    int fifo_expire[2];
    int fifo_batch;
    int writes_starved;
    int front_merges;
    u32 async_depth;
    int prio_aging_expire;
    spinlock_t lock;
    spinlock_t zone_lock;
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
struct deadline_data {
    struct rb_root sort_list[2];
    struct list_head fifo_list[2];
    struct request * next_rq[2];
    unsigned int batching;
    unsigned int starved;
    int fifo_expire[2];
    int fifo_batch;
    int writes_starved;
    int front_merges;
    spinlock_t lock;
    spinlock_t zone_lock;
    struct list_head dispatch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct deadline_data {
    struct rb_root sort_list[2];
    struct list_head fifo_list[2];
    struct request * next_rq[2];
    unsigned int batching;
    unsigned int starved;
    int fifo_expire[2];
    int fifo_batch;
    int writes_starved;
    int front_merges;
    spinlock_t lock;
    spinlock_t zone_lock;
    struct list_head dispatch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct deadline_data {
    struct rb_root sort_list[2];
    struct list_head fifo_list[2];
    struct request * next_rq[2];
    unsigned int batching;
    unsigned int starved;
    int fifo_expire[2];
    int fifo_batch;
    int writes_starved;
    int front_merges;
    spinlock_t lock;
    spinlock_t zone_lock;
    struct list_head dispatch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct deadline_data {
    struct rb_root sort_list[2];
    struct list_head fifo_list[2];
    struct request * next_rq[2];
    unsigned int batching;
    unsigned int starved;
    int fifo_expire[2];
    int fifo_batch;
    int writes_starved;
    int front_merges;
    spinlock_t lock;
    spinlock_t zone_lock;
    struct list_head dispatch;
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
struct deadline_data {
    struct rb_root sort_list[2];
    struct list_head fifo_list[2];
    struct request * next_rq[2];
    unsigned int batching;
    unsigned int starved;
    int fifo_expire[2];
    int fifo_batch;
    int writes_starved;
    int front_merges;
    spinlock_t lock;
    spinlock_t zone_lock;
    struct list_head dispatch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct deadline_data {
    struct rb_root sort_list[2];
    struct list_head fifo_list[2];
    struct request * next_rq[2];
    unsigned int batching;
    unsigned int starved;
    int fifo_expire[2];
    int fifo_batch;
    int writes_starved;
    int front_merges;
    spinlock_t lock;
    spinlock_t zone_lock;
    struct list_head dispatch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct deadline_data {
    struct rb_root sort_list[2];
    struct list_head fifo_list[2];
    struct request * next_rq[2];
    unsigned int batching;
    unsigned int starved;
    int fifo_expire[2];
    int fifo_batch;
    int writes_starved;
    int front_merges;
    spinlock_t lock;
    spinlock_t zone_lock;
    struct list_head dispatch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct deadline_data {
    struct rb_root sort_list[2];
    struct list_head fifo_list[2];
    struct request * next_rq[2];
    unsigned int batching;
    unsigned int starved;
    int fifo_expire[2];
    int fifo_batch;
    int writes_starved;
    int front_merges;
    spinlock_t lock;
    spinlock_t zone_lock;
    struct list_head dispatch;
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
<code>sector_t last_sector</code>
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
<code>spinlock_t lock</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t zone_lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head dispatch</code>
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
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct dd_per_prio per_prio[3]</code>
</li>
<li>
<b>Field added. </b>
<code>enum dd_data_dir last_dir</code>
</li>
<li>
<b>Field added. </b>
<code>struct io_stats *stats</code>
</li>
<li>
<b>Field added. </b>
<code>u32 async_depth</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rb_root sort_list[2]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head fifo_list[2]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct request * next_rq[2]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head dispatch</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int prio_aging_expire</code>
</li>
<li>
<b>Field removed. </b>
<code>struct io_stats *stats</code>
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
