# Struct: <code>worker</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct worker {
    struct list_head entry;
    struct hlist_node hentry;
    struct work_struct *current_work;
    work_func_t current_func;
    struct pool_workqueue *current_pwq;
    bool desc_valid;
    struct list_head scheduled;
    struct task_struct *task;
    struct worker_pool *pool;
    struct list_head node;
    long unsigned int last_active;
    unsigned int flags;
    int id;
    char desc[24];
    struct workqueue_struct *rescue_wq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct worker {
    struct list_head entry;
    struct hlist_node hentry;
    struct work_struct *current_work;
    work_func_t current_func;
    struct pool_workqueue *current_pwq;
    bool desc_valid;
    struct list_head scheduled;
    struct task_struct *task;
    struct worker_pool *pool;
    struct list_head node;
    long unsigned int last_active;
    unsigned int flags;
    int id;
    char desc[24];
    struct workqueue_struct *rescue_wq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct worker {
    struct list_head entry;
    struct hlist_node hentry;
    struct work_struct *current_work;
    work_func_t current_func;
    struct pool_workqueue *current_pwq;
    bool desc_valid;
    struct list_head scheduled;
    struct task_struct *task;
    struct worker_pool *pool;
    struct list_head node;
    long unsigned int last_active;
    unsigned int flags;
    int id;
    char desc[24];
    struct workqueue_struct *rescue_wq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct worker {
    struct list_head entry;
    struct hlist_node hentry;
    struct work_struct *current_work;
    work_func_t current_func;
    struct pool_workqueue *current_pwq;
    bool desc_valid;
    struct list_head scheduled;
    struct task_struct *task;
    struct worker_pool *pool;
    struct list_head node;
    long unsigned int last_active;
    unsigned int flags;
    int id;
    char desc[24];
    struct workqueue_struct *rescue_wq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct worker {
    struct list_head entry;
    struct hlist_node hentry;
    struct work_struct *current_work;
    work_func_t current_func;
    struct pool_workqueue *current_pwq;
    bool desc_valid;
    struct list_head scheduled;
    struct task_struct *task;
    struct worker_pool *pool;
    struct list_head node;
    long unsigned int last_active;
    unsigned int flags;
    int id;
    char desc[24];
    struct workqueue_struct *rescue_wq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct worker {
    struct list_head entry;
    struct hlist_node hentry;
    struct work_struct *current_work;
    work_func_t current_func;
    struct pool_workqueue *current_pwq;
    struct list_head scheduled;
    struct task_struct *task;
    struct worker_pool *pool;
    struct list_head node;
    long unsigned int last_active;
    unsigned int flags;
    int id;
    char desc[24];
    struct workqueue_struct *rescue_wq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct worker {
    struct list_head entry;
    struct hlist_node hentry;
    struct work_struct *current_work;
    work_func_t current_func;
    struct pool_workqueue *current_pwq;
    struct list_head scheduled;
    struct task_struct *task;
    struct worker_pool *pool;
    struct list_head node;
    long unsigned int last_active;
    unsigned int flags;
    int id;
    char desc[24];
    struct workqueue_struct *rescue_wq;
    work_func_t last_func;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct worker {
    struct list_head entry;
    struct hlist_node hentry;
    struct work_struct *current_work;
    work_func_t current_func;
    struct pool_workqueue *current_pwq;
    struct list_head scheduled;
    struct task_struct *task;
    struct worker_pool *pool;
    struct list_head node;
    long unsigned int last_active;
    unsigned int flags;
    int id;
    int sleeping;
    char desc[24];
    struct workqueue_struct *rescue_wq;
    work_func_t last_func;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct worker {
    struct list_head entry;
    struct hlist_node hentry;
    struct work_struct *current_work;
    work_func_t current_func;
    struct pool_workqueue *current_pwq;
    struct list_head scheduled;
    struct task_struct *task;
    struct worker_pool *pool;
    struct list_head node;
    long unsigned int last_active;
    unsigned int flags;
    int id;
    int sleeping;
    char desc[24];
    struct workqueue_struct *rescue_wq;
    work_func_t last_func;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct worker {
    struct list_head entry;
    struct hlist_node hentry;
    struct work_struct *current_work;
    work_func_t current_func;
    struct pool_workqueue *current_pwq;
    struct list_head scheduled;
    struct task_struct *task;
    struct worker_pool *pool;
    struct list_head node;
    long unsigned int last_active;
    unsigned int flags;
    int id;
    int sleeping;
    char desc[24];
    struct workqueue_struct *rescue_wq;
    work_func_t last_func;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct worker {
    struct list_head entry;
    struct hlist_node hentry;
    struct work_struct *current_work;
    work_func_t current_func;
    struct pool_workqueue *current_pwq;
    struct list_head scheduled;
    struct task_struct *task;
    struct worker_pool *pool;
    struct list_head node;
    long unsigned int last_active;
    unsigned int flags;
    int id;
    int sleeping;
    char desc[24];
    struct workqueue_struct *rescue_wq;
    work_func_t last_func;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct worker {
    struct list_head entry;
    struct hlist_node hentry;
    struct work_struct *current_work;
    work_func_t current_func;
    struct pool_workqueue *current_pwq;
    struct list_head scheduled;
    struct task_struct *task;
    struct worker_pool *pool;
    struct list_head node;
    long unsigned int last_active;
    unsigned int flags;
    int id;
    int sleeping;
    char desc[24];
    struct workqueue_struct *rescue_wq;
    work_func_t last_func;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct worker {
    struct list_head entry;
    struct hlist_node hentry;
    struct work_struct *current_work;
    work_func_t current_func;
    struct pool_workqueue *current_pwq;
    unsigned int current_color;
    struct list_head scheduled;
    struct task_struct *task;
    struct worker_pool *pool;
    struct list_head node;
    long unsigned int last_active;
    unsigned int flags;
    int id;
    int sleeping;
    char desc[24];
    struct workqueue_struct *rescue_wq;
    work_func_t last_func;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct worker {
    struct list_head entry;
    struct hlist_node hentry;
    struct work_struct *current_work;
    work_func_t current_func;
    struct pool_workqueue *current_pwq;
    unsigned int current_color;
    struct list_head scheduled;
    struct task_struct *task;
    struct worker_pool *pool;
    struct list_head node;
    long unsigned int last_active;
    unsigned int flags;
    int id;
    int sleeping;
    char desc[24];
    struct workqueue_struct *rescue_wq;
    work_func_t last_func;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct worker {
    struct list_head entry;
    struct hlist_node hentry;
    struct work_struct *current_work;
    work_func_t current_func;
    struct pool_workqueue *current_pwq;
    unsigned int current_color;
    struct list_head scheduled;
    struct task_struct *task;
    struct worker_pool *pool;
    struct list_head node;
    long unsigned int last_active;
    unsigned int flags;
    int id;
    int sleeping;
    char desc[24];
    struct workqueue_struct *rescue_wq;
    work_func_t last_func;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct worker {
    struct list_head entry;
    struct hlist_node hentry;
    struct work_struct *current_work;
    work_func_t current_func;
    struct pool_workqueue *current_pwq;
    u64 current_at;
    unsigned int current_color;
    int sleeping;
    work_func_t last_func;
    struct list_head scheduled;
    struct task_struct *task;
    struct worker_pool *pool;
    struct list_head node;
    long unsigned int last_active;
    unsigned int flags;
    int id;
    char desc[24];
    struct workqueue_struct *rescue_wq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct worker {
    struct list_head entry;
    struct hlist_node hentry;
    struct work_struct *current_work;
    work_func_t current_func;
    struct pool_workqueue *current_pwq;
    u64 current_at;
    unsigned int current_color;
    int sleeping;
    work_func_t last_func;
    struct list_head scheduled;
    struct task_struct *task;
    struct worker_pool *pool;
    struct list_head node;
    long unsigned int last_active;
    unsigned int flags;
    int id;
    char desc[24];
    struct workqueue_struct *rescue_wq;
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
struct worker {
    struct list_head entry;
    struct hlist_node hentry;
    struct work_struct *current_work;
    work_func_t current_func;
    struct pool_workqueue *current_pwq;
    struct list_head scheduled;
    struct task_struct *task;
    struct worker_pool *pool;
    struct list_head node;
    long unsigned int last_active;
    unsigned int flags;
    int id;
    int sleeping;
    char desc[24];
    struct workqueue_struct *rescue_wq;
    work_func_t last_func;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct worker {
    struct list_head entry;
    struct hlist_node hentry;
    struct work_struct *current_work;
    work_func_t current_func;
    struct pool_workqueue *current_pwq;
    struct list_head scheduled;
    struct task_struct *task;
    struct worker_pool *pool;
    struct list_head node;
    long unsigned int last_active;
    unsigned int flags;
    int id;
    int sleeping;
    char desc[24];
    struct workqueue_struct *rescue_wq;
    work_func_t last_func;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct worker {
    struct list_head entry;
    struct hlist_node hentry;
    struct work_struct *current_work;
    work_func_t current_func;
    struct pool_workqueue *current_pwq;
    struct list_head scheduled;
    struct task_struct *task;
    struct worker_pool *pool;
    struct list_head node;
    long unsigned int last_active;
    unsigned int flags;
    int id;
    int sleeping;
    char desc[24];
    struct workqueue_struct *rescue_wq;
    work_func_t last_func;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct worker {
    struct list_head entry;
    struct hlist_node hentry;
    struct work_struct *current_work;
    work_func_t current_func;
    struct pool_workqueue *current_pwq;
    struct list_head scheduled;
    struct task_struct *task;
    struct worker_pool *pool;
    struct list_head node;
    long unsigned int last_active;
    unsigned int flags;
    int id;
    int sleeping;
    char desc[24];
    struct workqueue_struct *rescue_wq;
    work_func_t last_func;
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
struct worker {
    struct list_head entry;
    struct hlist_node hentry;
    struct work_struct *current_work;
    work_func_t current_func;
    struct pool_workqueue *current_pwq;
    struct list_head scheduled;
    struct task_struct *task;
    struct worker_pool *pool;
    struct list_head node;
    long unsigned int last_active;
    unsigned int flags;
    int id;
    int sleeping;
    char desc[24];
    struct workqueue_struct *rescue_wq;
    work_func_t last_func;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct worker {
    struct list_head entry;
    struct hlist_node hentry;
    struct work_struct *current_work;
    work_func_t current_func;
    struct pool_workqueue *current_pwq;
    struct list_head scheduled;
    struct task_struct *task;
    struct worker_pool *pool;
    struct list_head node;
    long unsigned int last_active;
    unsigned int flags;
    int id;
    int sleeping;
    char desc[24];
    struct workqueue_struct *rescue_wq;
    work_func_t last_func;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct worker {
    struct list_head entry;
    struct hlist_node hentry;
    struct work_struct *current_work;
    work_func_t current_func;
    struct pool_workqueue *current_pwq;
    struct list_head scheduled;
    struct task_struct *task;
    struct worker_pool *pool;
    struct list_head node;
    long unsigned int last_active;
    unsigned int flags;
    int id;
    int sleeping;
    char desc[24];
    struct workqueue_struct *rescue_wq;
    work_func_t last_func;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct worker {
    struct list_head entry;
    struct hlist_node hentry;
    struct work_struct *current_work;
    work_func_t current_func;
    struct pool_workqueue *current_pwq;
    struct list_head scheduled;
    struct task_struct *task;
    struct worker_pool *pool;
    struct list_head node;
    long unsigned int last_active;
    unsigned int flags;
    int id;
    int sleeping;
    char desc[24];
    struct workqueue_struct *rescue_wq;
    work_func_t last_func;
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
<b>Field removed. </b>
<code>bool desc_valid</code>
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
<code>work_func_t last_func</code>
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
<code>int sleeping</code>
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
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int current_color</code>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 current_at</code>
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
