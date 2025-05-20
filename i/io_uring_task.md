# Struct: <code>io_uring_task</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
In <code>4.8</code>: Absent ⚠️
</li>
<li>
In <code>4.10</code>: Absent ⚠️
</li>
<li>
In <code>4.13</code>: Absent ⚠️
</li>
<li>
In <code>4.15</code>: Absent ⚠️
</li>
<li>
In <code>4.18</code>: Absent ⚠️
</li>
<li>
In <code>5.0</code>: Absent ⚠️
</li>
<li>
In <code>5.3</code>: Absent ⚠️
</li>
<li>
In <code>5.4</code>: Absent ⚠️
</li>
<li>
In <code>5.8</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct io_uring_task {
    struct xarray xa;
    struct wait_queue_head wait;
    struct file *last;
    struct percpu_counter inflight;
    struct io_identity __identity;
    struct io_identity *identity;
    atomic_t in_idle;
    bool sqpoll;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct io_uring_task {
    struct xarray xa;
    struct wait_queue_head wait;
    const struct io_ring_ctx *last;
    struct io_wq *io_wq;
    struct percpu_counter inflight;
    atomic_t inflight_tracked;
    atomic_t in_idle;
    spinlock_t task_lock;
    struct io_wq_work_list task_list;
    long unsigned int task_state;
    struct callback_head task_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct io_uring_task {
    int cached_refs;
    struct xarray xa;
    struct wait_queue_head wait;
    const struct io_ring_ctx *last;
    struct io_wq *io_wq;
    struct percpu_counter inflight;
    atomic_t inflight_tracked;
    atomic_t in_idle;
    spinlock_t task_lock;
    struct io_wq_work_list task_list;
    struct callback_head task_work;
    bool task_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct io_uring_task {
    int cached_refs;
    struct xarray xa;
    struct wait_queue_head wait;
    const struct io_ring_ctx *last;
    struct io_wq *io_wq;
    struct percpu_counter inflight;
    atomic_t inflight_tracked;
    atomic_t in_idle;
    spinlock_t task_lock;
    struct io_wq_work_list task_list;
    struct io_wq_work_list prio_task_list;
    struct callback_head task_work;
    struct file **registered_rings;
    bool task_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct io_uring_task {
    int cached_refs;
    const struct io_ring_ctx *last;
    struct io_wq *io_wq;
    struct file * registered_rings[16];
    struct xarray xa;
    struct wait_queue_head wait;
    atomic_t in_idle;
    atomic_t inflight_tracked;
    struct percpu_counter inflight;
    struct llist_head task_list;
    struct callback_head task_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct io_uring_task {
    int cached_refs;
    const struct io_ring_ctx *last;
    struct io_wq *io_wq;
    struct file * registered_rings[16];
    struct xarray xa;
    struct wait_queue_head wait;
    atomic_t in_cancel;
    atomic_t inflight_tracked;
    struct percpu_counter inflight;
    struct llist_head task_list;
    struct callback_head task_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct io_uring_task {
    int cached_refs;
    const struct io_ring_ctx *last;
    struct io_wq *io_wq;
    struct file * registered_rings[16];
    struct xarray xa;
    struct wait_queue_head wait;
    atomic_t in_cancel;
    atomic_t inflight_tracked;
    struct percpu_counter inflight;
    struct llist_head task_list;
    struct callback_head task_work;
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
In <code>arm64</code>: Absent ⚠️
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
In <code>aws</code>: Absent ⚠️
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct io_wq *io_wq</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t inflight_tracked</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t task_lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct io_wq_work_list task_list</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int task_state</code>
</li>
<li>
<b>Field added. </b>
<code>struct callback_head task_work</code>
</li>
<li>
<b>Field removed. </b>
<code>struct io_identity __identity</code>
</li>
<li>
<b>Field removed. </b>
<code>struct io_identity *identity</code>
</li>
<li>
<b>Field removed. </b>
<code>bool sqpoll</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct file *last</code> ➡️ <code>const struct io_ring_ctx *last</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int cached_refs</code>
</li>
<li>
<b>Field added. </b>
<code>bool task_running</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int task_state</code>
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
<code>struct io_wq_work_list prio_task_list</code>
</li>
<li>
<b>Field added. </b>
<code>struct file **registered_rings</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>spinlock_t task_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>struct io_wq_work_list prio_task_list</code>
</li>
<li>
<b>Field removed. </b>
<code>bool task_running</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct io_wq_work_list task_list</code> ➡️ <code>struct llist_head task_list</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct file **registered_rings</code> ➡️ <code>struct file * registered_rings[16]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>atomic_t in_cancel</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t in_idle</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
