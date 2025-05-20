# Struct: <code>rcu_tasks</code>

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
struct rcu_tasks {
    struct callback_head *cbs_head;
    struct callback_head **cbs_tail;
    struct wait_queue_head cbs_wq;
    raw_spinlock_t cbs_lock;
    int gp_state;
    long unsigned int gp_jiffies;
    long unsigned int gp_start;
    long unsigned int n_gps;
    long unsigned int n_ipis;
    long unsigned int n_ipis_fails;
    struct task_struct *kthread_ptr;
    rcu_tasks_gp_func_t gp_func;
    pregp_func_t pregp_func;
    pertask_func_t pertask_func;
    postscan_func_t postscan_func;
    holdouts_func_t holdouts_func;
    postgp_func_t postgp_func;
    call_rcu_func_t call_func;
    char *name;
    char *kname;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct rcu_tasks {
    struct callback_head *cbs_head;
    struct callback_head **cbs_tail;
    struct wait_queue_head cbs_wq;
    raw_spinlock_t cbs_lock;
    int gp_state;
    int gp_sleep;
    int init_fract;
    long unsigned int gp_jiffies;
    long unsigned int gp_start;
    long unsigned int n_gps;
    long unsigned int n_ipis;
    long unsigned int n_ipis_fails;
    struct task_struct *kthread_ptr;
    rcu_tasks_gp_func_t gp_func;
    pregp_func_t pregp_func;
    pertask_func_t pertask_func;
    postscan_func_t postscan_func;
    holdouts_func_t holdouts_func;
    postgp_func_t postgp_func;
    call_rcu_func_t call_func;
    char *name;
    char *kname;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rcu_tasks {
    struct callback_head *cbs_head;
    struct callback_head **cbs_tail;
    struct wait_queue_head cbs_wq;
    raw_spinlock_t cbs_lock;
    int gp_state;
    int gp_sleep;
    int init_fract;
    long unsigned int gp_jiffies;
    long unsigned int gp_start;
    long unsigned int n_gps;
    long unsigned int n_ipis;
    long unsigned int n_ipis_fails;
    struct task_struct *kthread_ptr;
    rcu_tasks_gp_func_t gp_func;
    pregp_func_t pregp_func;
    pertask_func_t pertask_func;
    postscan_func_t postscan_func;
    holdouts_func_t holdouts_func;
    postgp_func_t postgp_func;
    call_rcu_func_t call_func;
    char *name;
    char *kname;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rcu_tasks {
    struct callback_head *cbs_head;
    struct callback_head **cbs_tail;
    struct wait_queue_head cbs_wq;
    raw_spinlock_t cbs_lock;
    int gp_state;
    int gp_sleep;
    int init_fract;
    long unsigned int gp_jiffies;
    long unsigned int gp_start;
    long unsigned int n_gps;
    long unsigned int n_ipis;
    long unsigned int n_ipis_fails;
    struct task_struct *kthread_ptr;
    rcu_tasks_gp_func_t gp_func;
    pregp_func_t pregp_func;
    pertask_func_t pertask_func;
    postscan_func_t postscan_func;
    holdouts_func_t holdouts_func;
    postgp_func_t postgp_func;
    call_rcu_func_t call_func;
    char *name;
    char *kname;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rcu_tasks {
    struct rcuwait cbs_wait;
    raw_spinlock_t cbs_gbl_lock;
    int gp_state;
    int gp_sleep;
    int init_fract;
    long unsigned int gp_jiffies;
    long unsigned int gp_start;
    long unsigned int tasks_gp_seq;
    long unsigned int n_ipis;
    long unsigned int n_ipis_fails;
    struct task_struct *kthread_ptr;
    rcu_tasks_gp_func_t gp_func;
    pregp_func_t pregp_func;
    pertask_func_t pertask_func;
    postscan_func_t postscan_func;
    holdouts_func_t holdouts_func;
    postgp_func_t postgp_func;
    call_rcu_func_t call_func;
    struct rcu_tasks_percpu *rtpcpu;
    int percpu_enqueue_shift;
    int percpu_enqueue_lim;
    int percpu_dequeue_lim;
    long unsigned int percpu_dequeue_gpseq;
    struct mutex barrier_q_mutex;
    atomic_t barrier_q_count;
    struct completion barrier_q_completion;
    long unsigned int barrier_q_seq;
    char *name;
    char *kname;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rcu_tasks {
    struct rcuwait cbs_wait;
    raw_spinlock_t cbs_gbl_lock;
    struct mutex tasks_gp_mutex;
    int gp_state;
    int gp_sleep;
    int init_fract;
    long unsigned int gp_jiffies;
    long unsigned int gp_start;
    long unsigned int tasks_gp_seq;
    long unsigned int n_ipis;
    long unsigned int n_ipis_fails;
    struct task_struct *kthread_ptr;
    rcu_tasks_gp_func_t gp_func;
    pregp_func_t pregp_func;
    pertask_func_t pertask_func;
    postscan_func_t postscan_func;
    holdouts_func_t holdouts_func;
    postgp_func_t postgp_func;
    call_rcu_func_t call_func;
    struct rcu_tasks_percpu *rtpcpu;
    int percpu_enqueue_shift;
    int percpu_enqueue_lim;
    int percpu_dequeue_lim;
    long unsigned int percpu_dequeue_gpseq;
    struct mutex barrier_q_mutex;
    atomic_t barrier_q_count;
    struct completion barrier_q_completion;
    long unsigned int barrier_q_seq;
    char *name;
    char *kname;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rcu_tasks {
    struct rcuwait cbs_wait;
    raw_spinlock_t cbs_gbl_lock;
    struct mutex tasks_gp_mutex;
    int gp_state;
    int gp_sleep;
    int init_fract;
    long unsigned int gp_jiffies;
    long unsigned int gp_start;
    long unsigned int tasks_gp_seq;
    long unsigned int n_ipis;
    long unsigned int n_ipis_fails;
    struct task_struct *kthread_ptr;
    rcu_tasks_gp_func_t gp_func;
    pregp_func_t pregp_func;
    pertask_func_t pertask_func;
    postscan_func_t postscan_func;
    holdouts_func_t holdouts_func;
    postgp_func_t postgp_func;
    call_rcu_func_t call_func;
    struct rcu_tasks_percpu *rtpcpu;
    int percpu_enqueue_shift;
    int percpu_enqueue_lim;
    int percpu_dequeue_lim;
    long unsigned int percpu_dequeue_gpseq;
    struct mutex barrier_q_mutex;
    atomic_t barrier_q_count;
    struct completion barrier_q_completion;
    long unsigned int barrier_q_seq;
    char *name;
    char *kname;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rcu_tasks {
    struct rcuwait cbs_wait;
    raw_spinlock_t cbs_gbl_lock;
    struct mutex tasks_gp_mutex;
    int gp_state;
    int gp_sleep;
    int init_fract;
    long unsigned int gp_jiffies;
    long unsigned int gp_start;
    long unsigned int tasks_gp_seq;
    long unsigned int n_ipis;
    long unsigned int n_ipis_fails;
    struct task_struct *kthread_ptr;
    long unsigned int lazy_jiffies;
    rcu_tasks_gp_func_t gp_func;
    pregp_func_t pregp_func;
    pertask_func_t pertask_func;
    postscan_func_t postscan_func;
    holdouts_func_t holdouts_func;
    postgp_func_t postgp_func;
    call_rcu_func_t call_func;
    struct rcu_tasks_percpu *rtpcpu;
    int percpu_enqueue_shift;
    int percpu_enqueue_lim;
    int percpu_dequeue_lim;
    long unsigned int percpu_dequeue_gpseq;
    struct mutex barrier_q_mutex;
    atomic_t barrier_q_count;
    struct completion barrier_q_completion;
    long unsigned int barrier_q_seq;
    char *name;
    char *kname;
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
<code>int gp_sleep</code>
</li>
<li>
<b>Field added. </b>
<code>int init_fract</code>
</li>
</ul>
</details>
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
<b>Field added. </b>
<code>struct rcuwait cbs_wait</code>
</li>
<li>
<b>Field added. </b>
<code>raw_spinlock_t cbs_gbl_lock</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int tasks_gp_seq</code>
</li>
<li>
<b>Field added. </b>
<code>struct rcu_tasks_percpu *rtpcpu</code>
</li>
<li>
<b>Field added. </b>
<code>int percpu_enqueue_shift</code>
</li>
<li>
<b>Field added. </b>
<code>int percpu_enqueue_lim</code>
</li>
<li>
<b>Field added. </b>
<code>int percpu_dequeue_lim</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int percpu_dequeue_gpseq</code>
</li>
<li>
<b>Field added. </b>
<code>struct mutex barrier_q_mutex</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t barrier_q_count</code>
</li>
<li>
<b>Field added. </b>
<code>struct completion barrier_q_completion</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int barrier_q_seq</code>
</li>
<li>
<b>Field removed. </b>
<code>struct callback_head *cbs_head</code>
</li>
<li>
<b>Field removed. </b>
<code>struct callback_head **cbs_tail</code>
</li>
<li>
<b>Field removed. </b>
<code>struct wait_queue_head cbs_wq</code>
</li>
<li>
<b>Field removed. </b>
<code>raw_spinlock_t cbs_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int n_gps</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct mutex tasks_gp_mutex</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int lazy_jiffies</code>
</li>
</ul>
</details>
</li>
</ul>
