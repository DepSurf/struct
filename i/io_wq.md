# Struct: <code>io_wq</code>

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
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct io_wq {
    struct io_wqe **wqes;
    long unsigned int state;
    free_work_fn *free_work;
    io_wq_work_fn *do_work;
    struct task_struct *manager;
    struct user_struct *user;
    refcount_t refs;
    struct completion done;
    refcount_t use_refs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct io_wq {
    struct io_wqe **wqes;
    long unsigned int state;
    free_work_fn *free_work;
    io_wq_work_fn *do_work;
    struct task_struct *manager;
    struct user_struct *user;
    refcount_t refs;
    struct completion done;
    struct hlist_node cpuhp_node;
    refcount_t use_refs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct io_wq {
    struct io_wqe **wqes;
    long unsigned int state;
    free_work_fn *free_work;
    io_wq_work_fn *do_work;
    struct io_wq_hash *hash;
    refcount_t refs;
    atomic_t worker_refs;
    struct completion worker_done;
    struct hlist_node cpuhp_node;
    struct task_struct *task;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct io_wq {
    long unsigned int state;
    free_work_fn *free_work;
    io_wq_work_fn *do_work;
    struct io_wq_hash *hash;
    atomic_t worker_refs;
    struct completion worker_done;
    struct hlist_node cpuhp_node;
    struct task_struct *task;
    struct io_wqe * wqes[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct io_wq {
    long unsigned int state;
    free_work_fn *free_work;
    io_wq_work_fn *do_work;
    struct io_wq_hash *hash;
    atomic_t worker_refs;
    struct completion worker_done;
    struct hlist_node cpuhp_node;
    struct task_struct *task;
    struct io_wqe * wqes[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct io_wq {
    long unsigned int state;
    free_work_fn *free_work;
    io_wq_work_fn *do_work;
    struct io_wq_hash *hash;
    atomic_t worker_refs;
    struct completion worker_done;
    struct hlist_node cpuhp_node;
    struct task_struct *task;
    struct io_wqe * wqes[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct io_wq {
    long unsigned int state;
    free_work_fn *free_work;
    io_wq_work_fn *do_work;
    struct io_wq_hash *hash;
    atomic_t worker_refs;
    struct completion worker_done;
    struct hlist_node cpuhp_node;
    struct task_struct *task;
    struct io_wq_acct acct[2];
    raw_spinlock_t lock;
    struct hlist_nulls_head free_list;
    struct list_head all_list;
    struct wait_queue_entry wait;
    struct io_wq_work * hash_tail[64];
    cpumask_var_t cpu_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct io_wq {
    long unsigned int state;
    free_work_fn *free_work;
    io_wq_work_fn *do_work;
    struct io_wq_hash *hash;
    atomic_t worker_refs;
    struct completion worker_done;
    struct hlist_node cpuhp_node;
    struct task_struct *task;
    struct io_wq_acct acct[2];
    raw_spinlock_t lock;
    struct hlist_nulls_head free_list;
    struct list_head all_list;
    struct wait_queue_entry wait;
    struct io_wq_work * hash_tail[64];
    cpumask_var_t cpu_mask;
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
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct hlist_node cpuhp_node</code>
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
<code>struct io_wq_hash *hash</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t worker_refs</code>
</li>
<li>
<b>Field added. </b>
<code>struct completion worker_done</code>
</li>
<li>
<b>Field added. </b>
<code>struct task_struct *task</code>
</li>
<li>
<b>Field removed. </b>
<code>struct task_struct *manager</code>
</li>
<li>
<b>Field removed. </b>
<code>struct user_struct *user</code>
</li>
<li>
<b>Field removed. </b>
<code>struct completion done</code>
</li>
<li>
<b>Field removed. </b>
<code>refcount_t use_refs</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>refcount_t refs</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct io_wqe **wqes</code> ➡️ <code>struct io_wqe * wqes[0]</code>
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
<code>struct io_wq_acct acct[2]</code>
</li>
<li>
<b>Field added. </b>
<code>raw_spinlock_t lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct hlist_nulls_head free_list</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head all_list</code>
</li>
<li>
<b>Field added. </b>
<code>struct wait_queue_entry wait</code>
</li>
<li>
<b>Field added. </b>
<code>struct io_wq_work * hash_tail[64]</code>
</li>
<li>
<b>Field added. </b>
<code>cpumask_var_t cpu_mask</code>
</li>
<li>
<b>Field removed. </b>
<code>struct io_wqe * wqes[0]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
