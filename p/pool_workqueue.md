# Struct: <code>pool_workqueue</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct pool_workqueue {
    struct worker_pool *pool;
    struct workqueue_struct *wq;
    int work_color;
    int flush_color;
    int refcnt;
    int nr_in_flight[15];
    int nr_active;
    int max_active;
    struct list_head delayed_works;
    struct list_head pwqs_node;
    struct list_head mayday_node;
    struct work_struct unbound_release_work;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct pool_workqueue {
    struct worker_pool *pool;
    struct workqueue_struct *wq;
    int work_color;
    int flush_color;
    int refcnt;
    int nr_in_flight[15];
    int nr_active;
    int max_active;
    struct list_head delayed_works;
    struct list_head pwqs_node;
    struct list_head mayday_node;
    struct work_struct unbound_release_work;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct pool_workqueue {
    struct worker_pool *pool;
    struct workqueue_struct *wq;
    int work_color;
    int flush_color;
    int refcnt;
    int nr_in_flight[15];
    int nr_active;
    int max_active;
    struct list_head delayed_works;
    struct list_head pwqs_node;
    struct list_head mayday_node;
    struct work_struct unbound_release_work;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct pool_workqueue {
    struct worker_pool *pool;
    struct workqueue_struct *wq;
    int work_color;
    int flush_color;
    int refcnt;
    int nr_in_flight[15];
    int nr_active;
    int max_active;
    struct list_head delayed_works;
    struct list_head pwqs_node;
    struct list_head mayday_node;
    struct work_struct unbound_release_work;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct pool_workqueue {
    struct worker_pool *pool;
    struct workqueue_struct *wq;
    int work_color;
    int flush_color;
    int refcnt;
    int nr_in_flight[15];
    int nr_active;
    int max_active;
    struct list_head delayed_works;
    struct list_head pwqs_node;
    struct list_head mayday_node;
    struct work_struct unbound_release_work;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct pool_workqueue {
    struct worker_pool *pool;
    struct workqueue_struct *wq;
    int work_color;
    int flush_color;
    int refcnt;
    int nr_in_flight[15];
    int nr_active;
    int max_active;
    struct list_head delayed_works;
    struct list_head pwqs_node;
    struct list_head mayday_node;
    struct work_struct unbound_release_work;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct pool_workqueue {
    struct worker_pool *pool;
    struct workqueue_struct *wq;
    int work_color;
    int flush_color;
    int refcnt;
    int nr_in_flight[15];
    int nr_active;
    int max_active;
    struct list_head delayed_works;
    struct list_head pwqs_node;
    struct list_head mayday_node;
    struct work_struct unbound_release_work;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct pool_workqueue {
    struct worker_pool *pool;
    struct workqueue_struct *wq;
    int work_color;
    int flush_color;
    int refcnt;
    int nr_in_flight[15];
    int nr_active;
    int max_active;
    struct list_head delayed_works;
    struct list_head pwqs_node;
    struct list_head mayday_node;
    struct work_struct unbound_release_work;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct pool_workqueue {
    struct worker_pool *pool;
    struct workqueue_struct *wq;
    int work_color;
    int flush_color;
    int refcnt;
    int nr_in_flight[15];
    int nr_active;
    int max_active;
    struct list_head delayed_works;
    struct list_head pwqs_node;
    struct list_head mayday_node;
    struct work_struct unbound_release_work;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct pool_workqueue {
    struct worker_pool *pool;
    struct workqueue_struct *wq;
    int work_color;
    int flush_color;
    int refcnt;
    int nr_in_flight[15];
    int nr_active;
    int max_active;
    struct list_head delayed_works;
    struct list_head pwqs_node;
    struct list_head mayday_node;
    struct work_struct unbound_release_work;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct pool_workqueue {
    struct worker_pool *pool;
    struct workqueue_struct *wq;
    int work_color;
    int flush_color;
    int refcnt;
    int nr_in_flight[15];
    int nr_active;
    int max_active;
    struct list_head delayed_works;
    struct list_head pwqs_node;
    struct list_head mayday_node;
    struct work_struct unbound_release_work;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct pool_workqueue {
    struct worker_pool *pool;
    struct workqueue_struct *wq;
    int work_color;
    int flush_color;
    int refcnt;
    int nr_in_flight[15];
    int nr_active;
    int max_active;
    struct list_head delayed_works;
    struct list_head pwqs_node;
    struct list_head mayday_node;
    struct work_struct unbound_release_work;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct pool_workqueue {
    struct worker_pool *pool;
    struct workqueue_struct *wq;
    int work_color;
    int flush_color;
    int refcnt;
    int nr_in_flight[16];
    int nr_active;
    int max_active;
    struct list_head inactive_works;
    struct list_head pwqs_node;
    struct list_head mayday_node;
    struct work_struct unbound_release_work;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct pool_workqueue {
    struct worker_pool *pool;
    struct workqueue_struct *wq;
    int work_color;
    int flush_color;
    int refcnt;
    int nr_in_flight[16];
    int nr_active;
    int max_active;
    struct list_head inactive_works;
    struct list_head pwqs_node;
    struct list_head mayday_node;
    struct work_struct unbound_release_work;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct pool_workqueue {
    struct worker_pool *pool;
    struct workqueue_struct *wq;
    int work_color;
    int flush_color;
    int refcnt;
    int nr_in_flight[16];
    int nr_active;
    int max_active;
    struct list_head inactive_works;
    struct list_head pwqs_node;
    struct list_head mayday_node;
    struct work_struct unbound_release_work;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct pool_workqueue {
    struct worker_pool *pool;
    struct workqueue_struct *wq;
    int work_color;
    int flush_color;
    int refcnt;
    int nr_in_flight[16];
    int nr_active;
    int max_active;
    struct list_head inactive_works;
    struct list_head pwqs_node;
    struct list_head mayday_node;
    u64 stats[7];
    struct work_struct unbound_release_work;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct pool_workqueue {
    struct worker_pool *pool;
    struct workqueue_struct *wq;
    int work_color;
    int flush_color;
    int refcnt;
    int nr_in_flight[16];
    int nr_active;
    int max_active;
    struct list_head inactive_works;
    struct list_head pwqs_node;
    struct list_head mayday_node;
    u64 stats[8];
    struct kthread_work release_work;
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
struct pool_workqueue {
    struct worker_pool *pool;
    struct workqueue_struct *wq;
    int work_color;
    int flush_color;
    int refcnt;
    int nr_in_flight[15];
    int nr_active;
    int max_active;
    struct list_head delayed_works;
    struct list_head pwqs_node;
    struct list_head mayday_node;
    struct work_struct unbound_release_work;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct pool_workqueue {
    struct worker_pool *pool;
    struct workqueue_struct *wq;
    int work_color;
    int flush_color;
    int refcnt;
    int nr_in_flight[15];
    int nr_active;
    int max_active;
    struct list_head delayed_works;
    struct list_head pwqs_node;
    struct list_head mayday_node;
    struct work_struct unbound_release_work;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct pool_workqueue {
    struct worker_pool *pool;
    struct workqueue_struct *wq;
    int work_color;
    int flush_color;
    int refcnt;
    int nr_in_flight[15];
    int nr_active;
    int max_active;
    struct list_head delayed_works;
    struct list_head pwqs_node;
    struct list_head mayday_node;
    struct work_struct unbound_release_work;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct pool_workqueue {
    struct worker_pool *pool;
    struct workqueue_struct *wq;
    int work_color;
    int flush_color;
    int refcnt;
    int nr_in_flight[15];
    int nr_active;
    int max_active;
    struct list_head delayed_works;
    struct list_head pwqs_node;
    struct list_head mayday_node;
    struct work_struct unbound_release_work;
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
struct pool_workqueue {
    struct worker_pool *pool;
    struct workqueue_struct *wq;
    int work_color;
    int flush_color;
    int refcnt;
    int nr_in_flight[15];
    int nr_active;
    int max_active;
    struct list_head delayed_works;
    struct list_head pwqs_node;
    struct list_head mayday_node;
    struct work_struct unbound_release_work;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct pool_workqueue {
    struct worker_pool *pool;
    struct workqueue_struct *wq;
    int work_color;
    int flush_color;
    int refcnt;
    int nr_in_flight[15];
    int nr_active;
    int max_active;
    struct list_head delayed_works;
    struct list_head pwqs_node;
    struct list_head mayday_node;
    struct work_struct unbound_release_work;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct pool_workqueue {
    struct worker_pool *pool;
    struct workqueue_struct *wq;
    int work_color;
    int flush_color;
    int refcnt;
    int nr_in_flight[15];
    int nr_active;
    int max_active;
    struct list_head delayed_works;
    struct list_head pwqs_node;
    struct list_head mayday_node;
    struct work_struct unbound_release_work;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct pool_workqueue {
    struct worker_pool *pool;
    struct workqueue_struct *wq;
    int work_color;
    int flush_color;
    int refcnt;
    int nr_in_flight[15];
    int nr_active;
    int max_active;
    struct list_head delayed_works;
    struct list_head pwqs_node;
    struct list_head mayday_node;
    struct work_struct unbound_release_work;
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
No changes between <code>4.10</code> and <code>4.13</code> ✅
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
<code>struct list_head inactive_works</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head delayed_works</code>
</li>
<li>
<b>Field type changed. </b>
<code>int nr_in_flight[15]</code> ➡️ <code>int nr_in_flight[16]</code>
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
<code>u64 stats[7]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct kthread_work release_work</code>
</li>
<li>
<b>Field removed. </b>
<code>struct work_struct unbound_release_work</code>
</li>
<li>
<b>Field type changed. </b>
<code>u64 stats[7]</code> ➡️ <code>u64 stats[8]</code>
</li>
</ul>
</details>
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
