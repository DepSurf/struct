# Struct: <code>dm_kcopyd_client</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct dm_kcopyd_client {
    struct page_list *pages;
    unsigned int nr_reserved_pages;
    unsigned int nr_free_pages;
    struct dm_io_client *io_client;
    wait_queue_head_t destroyq;
    atomic_t nr_jobs;
    mempool_t *job_pool;
    struct workqueue_struct *kcopyd_wq;
    struct work_struct kcopyd_work;
    struct dm_kcopyd_throttle *throttle;
    spinlock_t job_lock;
    struct list_head complete_jobs;
    struct list_head io_jobs;
    struct list_head pages_jobs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct dm_kcopyd_client {
    struct page_list *pages;
    unsigned int nr_reserved_pages;
    unsigned int nr_free_pages;
    struct dm_io_client *io_client;
    wait_queue_head_t destroyq;
    atomic_t nr_jobs;
    mempool_t *job_pool;
    struct workqueue_struct *kcopyd_wq;
    struct work_struct kcopyd_work;
    struct dm_kcopyd_throttle *throttle;
    spinlock_t job_lock;
    struct list_head complete_jobs;
    struct list_head io_jobs;
    struct list_head pages_jobs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct dm_kcopyd_client {
    struct page_list *pages;
    unsigned int nr_reserved_pages;
    unsigned int nr_free_pages;
    struct dm_io_client *io_client;
    wait_queue_head_t destroyq;
    atomic_t nr_jobs;
    mempool_t *job_pool;
    struct workqueue_struct *kcopyd_wq;
    struct work_struct kcopyd_work;
    struct dm_kcopyd_throttle *throttle;
    spinlock_t job_lock;
    struct list_head complete_jobs;
    struct list_head io_jobs;
    struct list_head pages_jobs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct dm_kcopyd_client {
    struct page_list *pages;
    unsigned int nr_reserved_pages;
    unsigned int nr_free_pages;
    struct dm_io_client *io_client;
    wait_queue_head_t destroyq;
    atomic_t nr_jobs;
    mempool_t *job_pool;
    struct workqueue_struct *kcopyd_wq;
    struct work_struct kcopyd_work;
    struct dm_kcopyd_throttle *throttle;
    spinlock_t job_lock;
    struct list_head complete_jobs;
    struct list_head io_jobs;
    struct list_head pages_jobs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dm_kcopyd_client {
    struct page_list *pages;
    unsigned int nr_reserved_pages;
    unsigned int nr_free_pages;
    struct dm_io_client *io_client;
    wait_queue_head_t destroyq;
    atomic_t nr_jobs;
    mempool_t *job_pool;
    struct workqueue_struct *kcopyd_wq;
    struct work_struct kcopyd_work;
    struct dm_kcopyd_throttle *throttle;
    spinlock_t job_lock;
    struct list_head complete_jobs;
    struct list_head io_jobs;
    struct list_head pages_jobs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dm_kcopyd_client {
    struct page_list *pages;
    unsigned int nr_reserved_pages;
    unsigned int nr_free_pages;
    struct dm_io_client *io_client;
    wait_queue_head_t destroyq;
    mempool_t job_pool;
    struct workqueue_struct *kcopyd_wq;
    struct work_struct kcopyd_work;
    struct dm_kcopyd_throttle *throttle;
    atomic_t nr_jobs;
    spinlock_t job_lock;
    struct list_head complete_jobs;
    struct list_head io_jobs;
    struct list_head pages_jobs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dm_kcopyd_client {
    struct page_list *pages;
    unsigned int nr_reserved_pages;
    unsigned int nr_free_pages;
    struct dm_io_client *io_client;
    wait_queue_head_t destroyq;
    mempool_t job_pool;
    struct workqueue_struct *kcopyd_wq;
    struct work_struct kcopyd_work;
    struct dm_kcopyd_throttle *throttle;
    atomic_t nr_jobs;
    spinlock_t job_lock;
    struct list_head callback_jobs;
    struct list_head complete_jobs;
    struct list_head io_jobs;
    struct list_head pages_jobs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dm_kcopyd_client {
    struct page_list *pages;
    unsigned int nr_reserved_pages;
    unsigned int nr_free_pages;
    unsigned int sub_job_size;
    struct dm_io_client *io_client;
    wait_queue_head_t destroyq;
    mempool_t job_pool;
    struct workqueue_struct *kcopyd_wq;
    struct work_struct kcopyd_work;
    struct dm_kcopyd_throttle *throttle;
    atomic_t nr_jobs;
    spinlock_t job_lock;
    struct list_head callback_jobs;
    struct list_head complete_jobs;
    struct list_head io_jobs;
    struct list_head pages_jobs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dm_kcopyd_client {
    struct page_list *pages;
    unsigned int nr_reserved_pages;
    unsigned int nr_free_pages;
    unsigned int sub_job_size;
    struct dm_io_client *io_client;
    wait_queue_head_t destroyq;
    mempool_t job_pool;
    struct workqueue_struct *kcopyd_wq;
    struct work_struct kcopyd_work;
    struct dm_kcopyd_throttle *throttle;
    atomic_t nr_jobs;
    spinlock_t job_lock;
    struct list_head callback_jobs;
    struct list_head complete_jobs;
    struct list_head io_jobs;
    struct list_head pages_jobs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dm_kcopyd_client {
    struct page_list *pages;
    unsigned int nr_reserved_pages;
    unsigned int nr_free_pages;
    unsigned int sub_job_size;
    struct dm_io_client *io_client;
    wait_queue_head_t destroyq;
    mempool_t job_pool;
    struct workqueue_struct *kcopyd_wq;
    struct work_struct kcopyd_work;
    struct dm_kcopyd_throttle *throttle;
    atomic_t nr_jobs;
    spinlock_t job_lock;
    struct list_head callback_jobs;
    struct list_head complete_jobs;
    struct list_head io_jobs;
    struct list_head pages_jobs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dm_kcopyd_client {
    struct page_list *pages;
    unsigned int nr_reserved_pages;
    unsigned int nr_free_pages;
    unsigned int sub_job_size;
    struct dm_io_client *io_client;
    wait_queue_head_t destroyq;
    mempool_t job_pool;
    struct workqueue_struct *kcopyd_wq;
    struct work_struct kcopyd_work;
    struct dm_kcopyd_throttle *throttle;
    atomic_t nr_jobs;
    spinlock_t job_lock;
    struct list_head callback_jobs;
    struct list_head complete_jobs;
    struct list_head io_jobs;
    struct list_head pages_jobs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dm_kcopyd_client {
    struct page_list *pages;
    unsigned int nr_reserved_pages;
    unsigned int nr_free_pages;
    unsigned int sub_job_size;
    struct dm_io_client *io_client;
    wait_queue_head_t destroyq;
    mempool_t job_pool;
    struct workqueue_struct *kcopyd_wq;
    struct work_struct kcopyd_work;
    struct dm_kcopyd_throttle *throttle;
    atomic_t nr_jobs;
    spinlock_t job_lock;
    struct list_head callback_jobs;
    struct list_head complete_jobs;
    struct list_head io_jobs;
    struct list_head pages_jobs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dm_kcopyd_client {
    struct page_list *pages;
    unsigned int nr_reserved_pages;
    unsigned int nr_free_pages;
    unsigned int sub_job_size;
    struct dm_io_client *io_client;
    wait_queue_head_t destroyq;
    mempool_t job_pool;
    struct workqueue_struct *kcopyd_wq;
    struct work_struct kcopyd_work;
    struct dm_kcopyd_throttle *throttle;
    atomic_t nr_jobs;
    spinlock_t job_lock;
    struct list_head callback_jobs;
    struct list_head complete_jobs;
    struct list_head io_jobs;
    struct list_head pages_jobs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dm_kcopyd_client {
    struct page_list *pages;
    unsigned int nr_reserved_pages;
    unsigned int nr_free_pages;
    unsigned int sub_job_size;
    struct dm_io_client *io_client;
    wait_queue_head_t destroyq;
    mempool_t job_pool;
    struct workqueue_struct *kcopyd_wq;
    struct work_struct kcopyd_work;
    struct dm_kcopyd_throttle *throttle;
    atomic_t nr_jobs;
    spinlock_t job_lock;
    struct list_head callback_jobs;
    struct list_head complete_jobs;
    struct list_head io_jobs;
    struct list_head pages_jobs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dm_kcopyd_client {
    struct page_list *pages;
    unsigned int nr_reserved_pages;
    unsigned int nr_free_pages;
    unsigned int sub_job_size;
    struct dm_io_client *io_client;
    wait_queue_head_t destroyq;
    mempool_t job_pool;
    struct workqueue_struct *kcopyd_wq;
    struct work_struct kcopyd_work;
    struct dm_kcopyd_throttle *throttle;
    atomic_t nr_jobs;
    spinlock_t job_lock;
    struct list_head callback_jobs;
    struct list_head complete_jobs;
    struct list_head io_jobs;
    struct list_head pages_jobs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dm_kcopyd_client {
    struct page_list *pages;
    unsigned int nr_reserved_pages;
    unsigned int nr_free_pages;
    unsigned int sub_job_size;
    struct dm_io_client *io_client;
    wait_queue_head_t destroyq;
    mempool_t job_pool;
    struct workqueue_struct *kcopyd_wq;
    struct work_struct kcopyd_work;
    struct dm_kcopyd_throttle *throttle;
    atomic_t nr_jobs;
    spinlock_t job_lock;
    struct list_head callback_jobs;
    struct list_head complete_jobs;
    struct list_head io_jobs;
    struct list_head pages_jobs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dm_kcopyd_client {
    struct page_list *pages;
    unsigned int nr_reserved_pages;
    unsigned int nr_free_pages;
    unsigned int sub_job_size;
    struct dm_io_client *io_client;
    wait_queue_head_t destroyq;
    mempool_t job_pool;
    struct workqueue_struct *kcopyd_wq;
    struct work_struct kcopyd_work;
    struct dm_kcopyd_throttle *throttle;
    atomic_t nr_jobs;
    spinlock_t job_lock;
    struct list_head callback_jobs;
    struct list_head complete_jobs;
    struct list_head io_jobs;
    struct list_head pages_jobs;
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
struct dm_kcopyd_client {
    struct page_list *pages;
    unsigned int nr_reserved_pages;
    unsigned int nr_free_pages;
    unsigned int sub_job_size;
    struct dm_io_client *io_client;
    wait_queue_head_t destroyq;
    mempool_t job_pool;
    struct workqueue_struct *kcopyd_wq;
    struct work_struct kcopyd_work;
    struct dm_kcopyd_throttle *throttle;
    atomic_t nr_jobs;
    spinlock_t job_lock;
    struct list_head callback_jobs;
    struct list_head complete_jobs;
    struct list_head io_jobs;
    struct list_head pages_jobs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dm_kcopyd_client {
    struct page_list *pages;
    unsigned int nr_reserved_pages;
    unsigned int nr_free_pages;
    unsigned int sub_job_size;
    struct dm_io_client *io_client;
    wait_queue_head_t destroyq;
    mempool_t job_pool;
    struct workqueue_struct *kcopyd_wq;
    struct work_struct kcopyd_work;
    struct dm_kcopyd_throttle *throttle;
    atomic_t nr_jobs;
    spinlock_t job_lock;
    struct list_head callback_jobs;
    struct list_head complete_jobs;
    struct list_head io_jobs;
    struct list_head pages_jobs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dm_kcopyd_client {
    struct page_list *pages;
    unsigned int nr_reserved_pages;
    unsigned int nr_free_pages;
    unsigned int sub_job_size;
    struct dm_io_client *io_client;
    wait_queue_head_t destroyq;
    mempool_t job_pool;
    struct workqueue_struct *kcopyd_wq;
    struct work_struct kcopyd_work;
    struct dm_kcopyd_throttle *throttle;
    atomic_t nr_jobs;
    spinlock_t job_lock;
    struct list_head callback_jobs;
    struct list_head complete_jobs;
    struct list_head io_jobs;
    struct list_head pages_jobs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dm_kcopyd_client {
    struct page_list *pages;
    unsigned int nr_reserved_pages;
    unsigned int nr_free_pages;
    unsigned int sub_job_size;
    struct dm_io_client *io_client;
    wait_queue_head_t destroyq;
    mempool_t job_pool;
    struct workqueue_struct *kcopyd_wq;
    struct work_struct kcopyd_work;
    struct dm_kcopyd_throttle *throttle;
    atomic_t nr_jobs;
    spinlock_t job_lock;
    struct list_head callback_jobs;
    struct list_head complete_jobs;
    struct list_head io_jobs;
    struct list_head pages_jobs;
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
struct dm_kcopyd_client {
    struct page_list *pages;
    unsigned int nr_reserved_pages;
    unsigned int nr_free_pages;
    unsigned int sub_job_size;
    struct dm_io_client *io_client;
    wait_queue_head_t destroyq;
    mempool_t job_pool;
    struct workqueue_struct *kcopyd_wq;
    struct work_struct kcopyd_work;
    struct dm_kcopyd_throttle *throttle;
    atomic_t nr_jobs;
    spinlock_t job_lock;
    struct list_head callback_jobs;
    struct list_head complete_jobs;
    struct list_head io_jobs;
    struct list_head pages_jobs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dm_kcopyd_client {
    struct page_list *pages;
    unsigned int nr_reserved_pages;
    unsigned int nr_free_pages;
    unsigned int sub_job_size;
    struct dm_io_client *io_client;
    wait_queue_head_t destroyq;
    mempool_t job_pool;
    struct workqueue_struct *kcopyd_wq;
    struct work_struct kcopyd_work;
    struct dm_kcopyd_throttle *throttle;
    atomic_t nr_jobs;
    spinlock_t job_lock;
    struct list_head callback_jobs;
    struct list_head complete_jobs;
    struct list_head io_jobs;
    struct list_head pages_jobs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dm_kcopyd_client {
    struct page_list *pages;
    unsigned int nr_reserved_pages;
    unsigned int nr_free_pages;
    unsigned int sub_job_size;
    struct dm_io_client *io_client;
    wait_queue_head_t destroyq;
    mempool_t job_pool;
    struct workqueue_struct *kcopyd_wq;
    struct work_struct kcopyd_work;
    struct dm_kcopyd_throttle *throttle;
    atomic_t nr_jobs;
    spinlock_t job_lock;
    struct list_head callback_jobs;
    struct list_head complete_jobs;
    struct list_head io_jobs;
    struct list_head pages_jobs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dm_kcopyd_client {
    struct page_list *pages;
    unsigned int nr_reserved_pages;
    unsigned int nr_free_pages;
    unsigned int sub_job_size;
    struct dm_io_client *io_client;
    wait_queue_head_t destroyq;
    mempool_t job_pool;
    struct workqueue_struct *kcopyd_wq;
    struct work_struct kcopyd_work;
    struct dm_kcopyd_throttle *throttle;
    atomic_t nr_jobs;
    spinlock_t job_lock;
    struct list_head callback_jobs;
    struct list_head complete_jobs;
    struct list_head io_jobs;
    struct list_head pages_jobs;
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
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>mempool_t *job_pool</code> ➡️ <code>mempool_t job_pool</code>
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
<code>struct list_head callback_jobs</code>
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
<code>unsigned int sub_job_size</code>
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
