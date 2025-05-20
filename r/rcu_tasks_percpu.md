# Struct: <code>rcu_tasks_percpu</code>

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
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rcu_tasks_percpu {
    struct rcu_segcblist cblist;
    raw_spinlock_t lock;
    long unsigned int rtp_jiffies;
    long unsigned int rtp_n_lock_retries;
    struct work_struct rtp_work;
    struct irq_work rtp_irq_work;
    struct callback_head barrier_q_head;
    int cpu;
    struct rcu_tasks *rtpp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rcu_tasks_percpu {
    struct rcu_segcblist cblist;
    raw_spinlock_t lock;
    long unsigned int rtp_jiffies;
    long unsigned int rtp_n_lock_retries;
    struct work_struct rtp_work;
    struct irq_work rtp_irq_work;
    struct callback_head barrier_q_head;
    struct list_head rtp_blkd_tasks;
    int cpu;
    struct rcu_tasks *rtpp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rcu_tasks_percpu {
    struct rcu_segcblist cblist;
    raw_spinlock_t lock;
    long unsigned int rtp_jiffies;
    long unsigned int rtp_n_lock_retries;
    struct work_struct rtp_work;
    struct irq_work rtp_irq_work;
    struct callback_head barrier_q_head;
    struct list_head rtp_blkd_tasks;
    int cpu;
    struct rcu_tasks *rtpp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rcu_tasks_percpu {
    struct rcu_segcblist cblist;
    raw_spinlock_t lock;
    long unsigned int rtp_jiffies;
    long unsigned int rtp_n_lock_retries;
    struct timer_list lazy_timer;
    unsigned int urgent_gp;
    struct work_struct rtp_work;
    struct irq_work rtp_irq_work;
    struct callback_head barrier_q_head;
    struct list_head rtp_blkd_tasks;
    int cpu;
    struct rcu_tasks *rtpp;
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
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head rtp_blkd_tasks</code>
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
<code>struct timer_list lazy_timer</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int urgent_gp</code>
</li>
</ul>
</details>
</li>
</ul>
