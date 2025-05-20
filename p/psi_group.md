# Struct: <code>psi_group</code>

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
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct psi_group {
    struct mutex stat_lock;
    struct psi_group_cpu *pcpu;
    u64 total_prev[5];
    u64 last_update;
    u64 next_update;
    struct delayed_work clock_work;
    u64 total[5];
    long unsigned int avg[15];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct psi_group {
    struct mutex avgs_lock;
    struct psi_group_cpu *pcpu;
    u64 avg_total[5];
    u64 avg_last_update;
    u64 avg_next_update;
    struct delayed_work avgs_work;
    u64 total[10];
    long unsigned int avg[15];
    atomic_t poll_scheduled;
    struct kthread_worker *poll_kworker;
    struct kthread_delayed_work poll_work;
    struct mutex trigger_lock;
    struct list_head triggers;
    u32 nr_triggers[5];
    u32 poll_states;
    u64 poll_min_period;
    u64 polling_total[5];
    u64 polling_next_update;
    u64 polling_until;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct psi_group {
    struct mutex avgs_lock;
    struct psi_group_cpu *pcpu;
    u64 avg_total[5];
    u64 avg_last_update;
    u64 avg_next_update;
    struct delayed_work avgs_work;
    u64 total[10];
    long unsigned int avg[15];
    atomic_t poll_scheduled;
    struct kthread_worker *poll_kworker;
    struct kthread_delayed_work poll_work;
    struct mutex trigger_lock;
    struct list_head triggers;
    u32 nr_triggers[5];
    u32 poll_states;
    u64 poll_min_period;
    u64 polling_total[5];
    u64 polling_next_update;
    u64 polling_until;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct psi_group {
    struct mutex avgs_lock;
    struct psi_group_cpu *pcpu;
    u64 avg_total[5];
    u64 avg_last_update;
    u64 avg_next_update;
    struct delayed_work avgs_work;
    u64 total[10];
    long unsigned int avg[15];
    atomic_t poll_scheduled;
    struct kthread_worker *poll_kworker;
    struct kthread_delayed_work poll_work;
    struct mutex trigger_lock;
    struct list_head triggers;
    u32 nr_triggers[5];
    u32 poll_states;
    u64 poll_min_period;
    u64 polling_total[5];
    u64 polling_next_update;
    u64 polling_until;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct psi_group {
    struct mutex avgs_lock;
    struct psi_group_cpu *pcpu;
    u64 avg_total[5];
    u64 avg_last_update;
    u64 avg_next_update;
    struct delayed_work avgs_work;
    u64 total[10];
    long unsigned int avg[15];
    struct task_struct *poll_task;
    struct timer_list poll_timer;
    wait_queue_head_t poll_wait;
    atomic_t poll_wakeup;
    struct mutex trigger_lock;
    struct list_head triggers;
    u32 nr_triggers[5];
    u32 poll_states;
    u64 poll_min_period;
    u64 polling_total[5];
    u64 polling_next_update;
    u64 polling_until;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct psi_group {
    struct mutex avgs_lock;
    struct psi_group_cpu *pcpu;
    u64 avg_total[6];
    u64 avg_last_update;
    u64 avg_next_update;
    struct delayed_work avgs_work;
    u64 total[12];
    long unsigned int avg[18];
    struct task_struct *poll_task;
    struct timer_list poll_timer;
    wait_queue_head_t poll_wait;
    atomic_t poll_wakeup;
    struct mutex trigger_lock;
    struct list_head triggers;
    u32 nr_triggers[6];
    u32 poll_states;
    u64 poll_min_period;
    u64 polling_total[6];
    u64 polling_next_update;
    u64 polling_until;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct psi_group {
    struct mutex avgs_lock;
    struct psi_group_cpu *pcpu;
    u64 avg_total[6];
    u64 avg_last_update;
    u64 avg_next_update;
    struct delayed_work avgs_work;
    u64 total[12];
    long unsigned int avg[18];
    struct task_struct *poll_task;
    struct timer_list poll_timer;
    wait_queue_head_t poll_wait;
    atomic_t poll_wakeup;
    struct mutex trigger_lock;
    struct list_head triggers;
    u32 nr_triggers[6];
    u32 poll_states;
    u64 poll_min_period;
    u64 polling_total[6];
    u64 polling_next_update;
    u64 polling_until;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct psi_group {
    struct mutex avgs_lock;
    struct psi_group_cpu *pcpu;
    u64 avg_total[6];
    u64 avg_last_update;
    u64 avg_next_update;
    struct delayed_work avgs_work;
    u64 total[12];
    long unsigned int avg[18];
    struct task_struct *poll_task;
    struct timer_list poll_timer;
    wait_queue_head_t poll_wait;
    atomic_t poll_wakeup;
    struct mutex trigger_lock;
    struct list_head triggers;
    u32 nr_triggers[6];
    u32 poll_states;
    u64 poll_min_period;
    u64 polling_total[6];
    u64 polling_next_update;
    u64 polling_until;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct psi_group {
    struct psi_group *parent;
    bool enabled;
    struct mutex avgs_lock;
    struct psi_group_cpu *pcpu;
    u64 avg_total[6];
    u64 avg_last_update;
    u64 avg_next_update;
    struct delayed_work avgs_work;
    u64 total[12];
    long unsigned int avg[18];
    struct task_struct *poll_task;
    struct timer_list poll_timer;
    wait_queue_head_t poll_wait;
    atomic_t poll_wakeup;
    atomic_t poll_scheduled;
    struct mutex trigger_lock;
    struct list_head triggers;
    u32 nr_triggers[6];
    u32 poll_states;
    u64 poll_min_period;
    u64 polling_total[6];
    u64 polling_next_update;
    u64 polling_until;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct psi_group {
    struct psi_group *parent;
    bool enabled;
    struct mutex avgs_lock;
    struct psi_group_cpu *pcpu;
    u64 avg_total[6];
    u64 avg_last_update;
    u64 avg_next_update;
    struct delayed_work avgs_work;
    struct list_head avg_triggers;
    u32 avg_nr_triggers[6];
    u64 total[12];
    long unsigned int avg[18];
    struct task_struct *rtpoll_task;
    struct timer_list rtpoll_timer;
    wait_queue_head_t rtpoll_wait;
    atomic_t rtpoll_wakeup;
    atomic_t rtpoll_scheduled;
    struct mutex rtpoll_trigger_lock;
    struct list_head rtpoll_triggers;
    u32 rtpoll_nr_triggers[6];
    u32 rtpoll_states;
    u64 rtpoll_min_period;
    u64 rtpoll_total[6];
    u64 rtpoll_next_update;
    u64 rtpoll_until;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct psi_group {
    struct psi_group *parent;
    bool enabled;
    struct mutex avgs_lock;
    struct psi_group_cpu *pcpu;
    u64 avg_total[6];
    u64 avg_last_update;
    u64 avg_next_update;
    struct delayed_work avgs_work;
    struct list_head avg_triggers;
    u32 avg_nr_triggers[6];
    u64 total[12];
    long unsigned int avg[18];
    struct task_struct *rtpoll_task;
    struct timer_list rtpoll_timer;
    wait_queue_head_t rtpoll_wait;
    atomic_t rtpoll_wakeup;
    atomic_t rtpoll_scheduled;
    struct mutex rtpoll_trigger_lock;
    struct list_head rtpoll_triggers;
    u32 rtpoll_nr_triggers[6];
    u32 rtpoll_states;
    u64 rtpoll_min_period;
    u64 rtpoll_total[6];
    u64 rtpoll_next_update;
    u64 rtpoll_until;
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
struct psi_group {
    struct mutex avgs_lock;
    struct psi_group_cpu *pcpu;
    u64 avg_total[5];
    u64 avg_last_update;
    u64 avg_next_update;
    struct delayed_work avgs_work;
    u64 total[10];
    long unsigned int avg[15];
    atomic_t poll_scheduled;
    struct kthread_worker *poll_kworker;
    struct kthread_delayed_work poll_work;
    struct mutex trigger_lock;
    struct list_head triggers;
    u32 nr_triggers[5];
    u32 poll_states;
    u64 poll_min_period;
    u64 polling_total[5];
    u64 polling_next_update;
    u64 polling_until;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct psi_group {
    struct mutex avgs_lock;
    struct psi_group_cpu *pcpu;
    u64 avg_total[5];
    u64 avg_last_update;
    u64 avg_next_update;
    struct delayed_work avgs_work;
    u64 total[10];
    long unsigned int avg[15];
    atomic_t poll_scheduled;
    struct kthread_worker *poll_kworker;
    struct kthread_delayed_work poll_work;
    struct mutex trigger_lock;
    struct list_head triggers;
    u32 nr_triggers[5];
    u32 poll_states;
    u64 poll_min_period;
    u64 polling_total[5];
    u64 polling_next_update;
    u64 polling_until;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct psi_group {
    struct mutex avgs_lock;
    struct psi_group_cpu *pcpu;
    u64 avg_total[5];
    u64 avg_last_update;
    u64 avg_next_update;
    struct delayed_work avgs_work;
    u64 total[10];
    long unsigned int avg[15];
    atomic_t poll_scheduled;
    struct kthread_worker *poll_kworker;
    struct kthread_delayed_work poll_work;
    struct mutex trigger_lock;
    struct list_head triggers;
    u32 nr_triggers[5];
    u32 poll_states;
    u64 poll_min_period;
    u64 polling_total[5];
    u64 polling_next_update;
    u64 polling_until;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct psi_group {
    struct mutex avgs_lock;
    struct psi_group_cpu *pcpu;
    u64 avg_total[5];
    u64 avg_last_update;
    u64 avg_next_update;
    struct delayed_work avgs_work;
    u64 total[10];
    long unsigned int avg[15];
    atomic_t poll_scheduled;
    struct kthread_worker *poll_kworker;
    struct kthread_delayed_work poll_work;
    struct mutex trigger_lock;
    struct list_head triggers;
    u32 nr_triggers[5];
    u32 poll_states;
    u64 poll_min_period;
    u64 polling_total[5];
    u64 polling_next_update;
    u64 polling_until;
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
struct psi_group {
    struct mutex avgs_lock;
    struct psi_group_cpu *pcpu;
    u64 avg_total[5];
    u64 avg_last_update;
    u64 avg_next_update;
    struct delayed_work avgs_work;
    u64 total[10];
    long unsigned int avg[15];
    atomic_t poll_scheduled;
    struct kthread_worker *poll_kworker;
    struct kthread_delayed_work poll_work;
    struct mutex trigger_lock;
    struct list_head triggers;
    u32 nr_triggers[5];
    u32 poll_states;
    u64 poll_min_period;
    u64 polling_total[5];
    u64 polling_next_update;
    u64 polling_until;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct psi_group {
    struct mutex avgs_lock;
    struct psi_group_cpu *pcpu;
    u64 avg_total[5];
    u64 avg_last_update;
    u64 avg_next_update;
    struct delayed_work avgs_work;
    u64 total[10];
    long unsigned int avg[15];
    atomic_t poll_scheduled;
    struct kthread_worker *poll_kworker;
    struct kthread_delayed_work poll_work;
    struct mutex trigger_lock;
    struct list_head triggers;
    u32 nr_triggers[5];
    u32 poll_states;
    u64 poll_min_period;
    u64 polling_total[5];
    u64 polling_next_update;
    u64 polling_until;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct psi_group {
    struct mutex avgs_lock;
    struct psi_group_cpu *pcpu;
    u64 avg_total[5];
    u64 avg_last_update;
    u64 avg_next_update;
    struct delayed_work avgs_work;
    u64 total[10];
    long unsigned int avg[15];
    atomic_t poll_scheduled;
    struct kthread_worker *poll_kworker;
    struct kthread_delayed_work poll_work;
    struct mutex trigger_lock;
    struct list_head triggers;
    u32 nr_triggers[5];
    u32 poll_states;
    u64 poll_min_period;
    u64 polling_total[5];
    u64 polling_next_update;
    u64 polling_until;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct psi_group {
    struct mutex avgs_lock;
    struct psi_group_cpu *pcpu;
    u64 avg_total[5];
    u64 avg_last_update;
    u64 avg_next_update;
    struct delayed_work avgs_work;
    u64 total[10];
    long unsigned int avg[15];
    atomic_t poll_scheduled;
    struct kthread_worker *poll_kworker;
    struct kthread_delayed_work poll_work;
    struct mutex trigger_lock;
    struct list_head triggers;
    u32 nr_triggers[5];
    u32 poll_states;
    u64 poll_min_period;
    u64 polling_total[5];
    u64 polling_next_update;
    u64 polling_until;
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
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct mutex avgs_lock</code>
</li>
<li>
<b>Field added. </b>
<code>u64 avg_total[5]</code>
</li>
<li>
<b>Field added. </b>
<code>u64 avg_last_update</code>
</li>
<li>
<b>Field added. </b>
<code>u64 avg_next_update</code>
</li>
<li>
<b>Field added. </b>
<code>struct delayed_work avgs_work</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t poll_scheduled</code>
</li>
<li>
<b>Field added. </b>
<code>struct kthread_worker *poll_kworker</code>
</li>
<li>
<b>Field added. </b>
<code>struct kthread_delayed_work poll_work</code>
</li>
<li>
<b>Field added. </b>
<code>struct mutex trigger_lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head triggers</code>
</li>
<li>
<b>Field added. </b>
<code>u32 nr_triggers[5]</code>
</li>
<li>
<b>Field added. </b>
<code>u32 poll_states</code>
</li>
<li>
<b>Field added. </b>
<code>u64 poll_min_period</code>
</li>
<li>
<b>Field added. </b>
<code>u64 polling_total[5]</code>
</li>
<li>
<b>Field added. </b>
<code>u64 polling_next_update</code>
</li>
<li>
<b>Field added. </b>
<code>u64 polling_until</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mutex stat_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 total_prev[5]</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 last_update</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 next_update</code>
</li>
<li>
<b>Field removed. </b>
<code>struct delayed_work clock_work</code>
</li>
<li>
<b>Field type changed. </b>
<code>u64 total[5]</code> ➡️ <code>u64 total[10]</code>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct task_struct *poll_task</code>
</li>
<li>
<b>Field added. </b>
<code>struct timer_list poll_timer</code>
</li>
<li>
<b>Field added. </b>
<code>wait_queue_head_t poll_wait</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t poll_wakeup</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t poll_scheduled</code>
</li>
<li>
<b>Field removed. </b>
<code>struct kthread_worker *poll_kworker</code>
</li>
<li>
<b>Field removed. </b>
<code>struct kthread_delayed_work poll_work</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>u64 avg_total[5]</code> ➡️ <code>u64 avg_total[6]</code>
</li>
<li>
<b>Field type changed. </b>
<code>u64 total[10]</code> ➡️ <code>u64 total[12]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int avg[15]</code> ➡️ <code>long unsigned int avg[18]</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 nr_triggers[5]</code> ➡️ <code>u32 nr_triggers[6]</code>
</li>
<li>
<b>Field type changed. </b>
<code>u64 polling_total[5]</code> ➡️ <code>u64 polling_total[6]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct psi_group *parent</code>
</li>
<li>
<b>Field added. </b>
<code>bool enabled</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t poll_scheduled</code>
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
<code>struct list_head avg_triggers</code>
</li>
<li>
<b>Field added. </b>
<code>u32 avg_nr_triggers[6]</code>
</li>
<li>
<b>Field added. </b>
<code>struct task_struct *rtpoll_task</code>
</li>
<li>
<b>Field added. </b>
<code>struct timer_list rtpoll_timer</code>
</li>
<li>
<b>Field added. </b>
<code>wait_queue_head_t rtpoll_wait</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t rtpoll_wakeup</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t rtpoll_scheduled</code>
</li>
<li>
<b>Field added. </b>
<code>struct mutex rtpoll_trigger_lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head rtpoll_triggers</code>
</li>
<li>
<b>Field added. </b>
<code>u32 rtpoll_nr_triggers[6]</code>
</li>
<li>
<b>Field added. </b>
<code>u32 rtpoll_states</code>
</li>
<li>
<b>Field added. </b>
<code>u64 rtpoll_min_period</code>
</li>
<li>
<b>Field added. </b>
<code>u64 rtpoll_total[6]</code>
</li>
<li>
<b>Field added. </b>
<code>u64 rtpoll_next_update</code>
</li>
<li>
<b>Field added. </b>
<code>u64 rtpoll_until</code>
</li>
<li>
<b>Field removed. </b>
<code>struct task_struct *poll_task</code>
</li>
<li>
<b>Field removed. </b>
<code>struct timer_list poll_timer</code>
</li>
<li>
<b>Field removed. </b>
<code>wait_queue_head_t poll_wait</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t poll_wakeup</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t poll_scheduled</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mutex trigger_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head triggers</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 nr_triggers[6]</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 poll_states</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 poll_min_period</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 polling_total[6]</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 polling_next_update</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 polling_until</code>
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
