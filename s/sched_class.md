# Struct: <code>sched_class</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct sched_class {
    const struct sched_class *next;
    void (*enqueue_task)(struct rq *, struct task_struct *, int);
    void (*dequeue_task)(struct rq *, struct task_struct *, int);
    void (*yield_task)(struct rq *);
    bool (*yield_to_task)(struct rq *, struct task_struct *, bool);
    void (*check_preempt_curr)(struct rq *, struct task_struct *, int);
    struct task_struct * (*pick_next_task)(struct rq *, struct task_struct *);
    void (*put_prev_task)(struct rq *, struct task_struct *);
    int (*select_task_rq)(struct task_struct *, int, int, int);
    void (*migrate_task_rq)(struct task_struct *);
    void (*task_waking)(struct task_struct *);
    void (*task_woken)(struct rq *, struct task_struct *);
    void (*set_cpus_allowed)(struct task_struct *, const struct cpumask *);
    void (*rq_online)(struct rq *);
    void (*rq_offline)(struct rq *);
    void (*set_curr_task)(struct rq *);
    void (*task_tick)(struct rq *, struct task_struct *, int);
    void (*task_fork)(struct task_struct *);
    void (*task_dead)(struct task_struct *);
    void (*switched_from)(struct rq *, struct task_struct *);
    void (*switched_to)(struct rq *, struct task_struct *);
    void (*prio_changed)(struct rq *, struct task_struct *, int);
    unsigned int (*get_rr_interval)(struct rq *, struct task_struct *);
    void (*update_curr)(struct rq *);
    void (*task_move_group)(struct task_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct sched_class {
    const struct sched_class *next;
    void (*enqueue_task)(struct rq *, struct task_struct *, int);
    void (*dequeue_task)(struct rq *, struct task_struct *, int);
    void (*yield_task)(struct rq *);
    bool (*yield_to_task)(struct rq *, struct task_struct *, bool);
    void (*check_preempt_curr)(struct rq *, struct task_struct *, int);
    struct task_struct * (*pick_next_task)(struct rq *, struct task_struct *, struct pin_cookie);
    void (*put_prev_task)(struct rq *, struct task_struct *);
    int (*select_task_rq)(struct task_struct *, int, int, int);
    void (*migrate_task_rq)(struct task_struct *);
    void (*task_woken)(struct rq *, struct task_struct *);
    void (*set_cpus_allowed)(struct task_struct *, const struct cpumask *);
    void (*rq_online)(struct rq *);
    void (*rq_offline)(struct rq *);
    void (*set_curr_task)(struct rq *);
    void (*task_tick)(struct rq *, struct task_struct *, int);
    void (*task_fork)(struct task_struct *);
    void (*task_dead)(struct task_struct *);
    void (*switched_from)(struct rq *, struct task_struct *);
    void (*switched_to)(struct rq *, struct task_struct *);
    void (*prio_changed)(struct rq *, struct task_struct *, int);
    unsigned int (*get_rr_interval)(struct rq *, struct task_struct *);
    void (*update_curr)(struct rq *);
    void (*task_change_group)(struct task_struct *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct sched_class {
    const struct sched_class *next;
    void (*enqueue_task)(struct rq *, struct task_struct *, int);
    void (*dequeue_task)(struct rq *, struct task_struct *, int);
    void (*yield_task)(struct rq *);
    bool (*yield_to_task)(struct rq *, struct task_struct *, bool);
    void (*check_preempt_curr)(struct rq *, struct task_struct *, int);
    struct task_struct * (*pick_next_task)(struct rq *, struct task_struct *, struct pin_cookie);
    void (*put_prev_task)(struct rq *, struct task_struct *);
    int (*select_task_rq)(struct task_struct *, int, int, int);
    void (*migrate_task_rq)(struct task_struct *);
    void (*task_woken)(struct rq *, struct task_struct *);
    void (*set_cpus_allowed)(struct task_struct *, const struct cpumask *);
    void (*rq_online)(struct rq *);
    void (*rq_offline)(struct rq *);
    void (*set_curr_task)(struct rq *);
    void (*task_tick)(struct rq *, struct task_struct *, int);
    void (*task_fork)(struct task_struct *);
    void (*task_dead)(struct task_struct *);
    void (*switched_from)(struct rq *, struct task_struct *);
    void (*switched_to)(struct rq *, struct task_struct *);
    void (*prio_changed)(struct rq *, struct task_struct *, int);
    unsigned int (*get_rr_interval)(struct rq *, struct task_struct *);
    void (*update_curr)(struct rq *);
    void (*task_change_group)(struct task_struct *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct sched_class {
    const struct sched_class *next;
    void (*enqueue_task)(struct rq *, struct task_struct *, int);
    void (*dequeue_task)(struct rq *, struct task_struct *, int);
    void (*yield_task)(struct rq *);
    bool (*yield_to_task)(struct rq *, struct task_struct *, bool);
    void (*check_preempt_curr)(struct rq *, struct task_struct *, int);
    struct task_struct * (*pick_next_task)(struct rq *, struct task_struct *, struct rq_flags *);
    void (*put_prev_task)(struct rq *, struct task_struct *);
    int (*select_task_rq)(struct task_struct *, int, int, int);
    void (*migrate_task_rq)(struct task_struct *);
    void (*task_woken)(struct rq *, struct task_struct *);
    void (*set_cpus_allowed)(struct task_struct *, const struct cpumask *);
    void (*rq_online)(struct rq *);
    void (*rq_offline)(struct rq *);
    void (*set_curr_task)(struct rq *);
    void (*task_tick)(struct rq *, struct task_struct *, int);
    void (*task_fork)(struct task_struct *);
    void (*task_dead)(struct task_struct *);
    void (*switched_from)(struct rq *, struct task_struct *);
    void (*switched_to)(struct rq *, struct task_struct *);
    void (*prio_changed)(struct rq *, struct task_struct *, int);
    unsigned int (*get_rr_interval)(struct rq *, struct task_struct *);
    void (*update_curr)(struct rq *);
    void (*task_change_group)(struct task_struct *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct sched_class {
    const struct sched_class *next;
    void (*enqueue_task)(struct rq *, struct task_struct *, int);
    void (*dequeue_task)(struct rq *, struct task_struct *, int);
    void (*yield_task)(struct rq *);
    bool (*yield_to_task)(struct rq *, struct task_struct *, bool);
    void (*check_preempt_curr)(struct rq *, struct task_struct *, int);
    struct task_struct * (*pick_next_task)(struct rq *, struct task_struct *, struct rq_flags *);
    void (*put_prev_task)(struct rq *, struct task_struct *);
    int (*select_task_rq)(struct task_struct *, int, int, int);
    void (*migrate_task_rq)(struct task_struct *);
    void (*task_woken)(struct rq *, struct task_struct *);
    void (*set_cpus_allowed)(struct task_struct *, const struct cpumask *);
    void (*rq_online)(struct rq *);
    void (*rq_offline)(struct rq *);
    void (*set_curr_task)(struct rq *);
    void (*task_tick)(struct rq *, struct task_struct *, int);
    void (*task_fork)(struct task_struct *);
    void (*task_dead)(struct task_struct *);
    void (*switched_from)(struct rq *, struct task_struct *);
    void (*switched_to)(struct rq *, struct task_struct *);
    void (*prio_changed)(struct rq *, struct task_struct *, int);
    unsigned int (*get_rr_interval)(struct rq *, struct task_struct *);
    void (*update_curr)(struct rq *);
    void (*task_change_group)(struct task_struct *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct sched_class {
    const struct sched_class *next;
    void (*enqueue_task)(struct rq *, struct task_struct *, int);
    void (*dequeue_task)(struct rq *, struct task_struct *, int);
    void (*yield_task)(struct rq *);
    bool (*yield_to_task)(struct rq *, struct task_struct *, bool);
    void (*check_preempt_curr)(struct rq *, struct task_struct *, int);
    struct task_struct * (*pick_next_task)(struct rq *, struct task_struct *, struct rq_flags *);
    void (*put_prev_task)(struct rq *, struct task_struct *);
    int (*select_task_rq)(struct task_struct *, int, int, int);
    void (*migrate_task_rq)(struct task_struct *);
    void (*task_woken)(struct rq *, struct task_struct *);
    void (*set_cpus_allowed)(struct task_struct *, const struct cpumask *);
    void (*rq_online)(struct rq *);
    void (*rq_offline)(struct rq *);
    void (*set_curr_task)(struct rq *);
    void (*task_tick)(struct rq *, struct task_struct *, int);
    void (*task_fork)(struct task_struct *);
    void (*task_dead)(struct task_struct *);
    void (*switched_from)(struct rq *, struct task_struct *);
    void (*switched_to)(struct rq *, struct task_struct *);
    void (*prio_changed)(struct rq *, struct task_struct *, int);
    unsigned int (*get_rr_interval)(struct rq *, struct task_struct *);
    void (*update_curr)(struct rq *);
    void (*task_change_group)(struct task_struct *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct sched_class {
    const struct sched_class *next;
    void (*enqueue_task)(struct rq *, struct task_struct *, int);
    void (*dequeue_task)(struct rq *, struct task_struct *, int);
    void (*yield_task)(struct rq *);
    bool (*yield_to_task)(struct rq *, struct task_struct *, bool);
    void (*check_preempt_curr)(struct rq *, struct task_struct *, int);
    struct task_struct * (*pick_next_task)(struct rq *, struct task_struct *, struct rq_flags *);
    void (*put_prev_task)(struct rq *, struct task_struct *);
    int (*select_task_rq)(struct task_struct *, int, int, int);
    void (*migrate_task_rq)(struct task_struct *, int);
    void (*task_woken)(struct rq *, struct task_struct *);
    void (*set_cpus_allowed)(struct task_struct *, const struct cpumask *);
    void (*rq_online)(struct rq *);
    void (*rq_offline)(struct rq *);
    void (*set_curr_task)(struct rq *);
    void (*task_tick)(struct rq *, struct task_struct *, int);
    void (*task_fork)(struct task_struct *);
    void (*task_dead)(struct task_struct *);
    void (*switched_from)(struct rq *, struct task_struct *);
    void (*switched_to)(struct rq *, struct task_struct *);
    void (*prio_changed)(struct rq *, struct task_struct *, int);
    unsigned int (*get_rr_interval)(struct rq *, struct task_struct *);
    void (*update_curr)(struct rq *);
    void (*task_change_group)(struct task_struct *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct sched_class {
    const struct sched_class *next;
    int uclamp_enabled;
    void (*enqueue_task)(struct rq *, struct task_struct *, int);
    void (*dequeue_task)(struct rq *, struct task_struct *, int);
    void (*yield_task)(struct rq *);
    bool (*yield_to_task)(struct rq *, struct task_struct *, bool);
    void (*check_preempt_curr)(struct rq *, struct task_struct *, int);
    struct task_struct * (*pick_next_task)(struct rq *, struct task_struct *, struct rq_flags *);
    void (*put_prev_task)(struct rq *, struct task_struct *);
    int (*select_task_rq)(struct task_struct *, int, int, int);
    void (*migrate_task_rq)(struct task_struct *, int);
    void (*task_woken)(struct rq *, struct task_struct *);
    void (*set_cpus_allowed)(struct task_struct *, const struct cpumask *);
    void (*rq_online)(struct rq *);
    void (*rq_offline)(struct rq *);
    void (*set_curr_task)(struct rq *);
    void (*task_tick)(struct rq *, struct task_struct *, int);
    void (*task_fork)(struct task_struct *);
    void (*task_dead)(struct task_struct *);
    void (*switched_from)(struct rq *, struct task_struct *);
    void (*switched_to)(struct rq *, struct task_struct *);
    void (*prio_changed)(struct rq *, struct task_struct *, int);
    unsigned int (*get_rr_interval)(struct rq *, struct task_struct *);
    void (*update_curr)(struct rq *);
    void (*task_change_group)(struct task_struct *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct sched_class {
    const struct sched_class *next;
    int uclamp_enabled;
    void (*enqueue_task)(struct rq *, struct task_struct *, int);
    void (*dequeue_task)(struct rq *, struct task_struct *, int);
    void (*yield_task)(struct rq *);
    bool (*yield_to_task)(struct rq *, struct task_struct *, bool);
    void (*check_preempt_curr)(struct rq *, struct task_struct *, int);
    struct task_struct * (*pick_next_task)(struct rq *, struct task_struct *, struct rq_flags *);
    void (*put_prev_task)(struct rq *, struct task_struct *);
    void (*set_next_task)(struct rq *, struct task_struct *, bool);
    int (*balance)(struct rq *, struct task_struct *, struct rq_flags *);
    int (*select_task_rq)(struct task_struct *, int, int, int);
    void (*migrate_task_rq)(struct task_struct *, int);
    void (*task_woken)(struct rq *, struct task_struct *);
    void (*set_cpus_allowed)(struct task_struct *, const struct cpumask *);
    void (*rq_online)(struct rq *);
    void (*rq_offline)(struct rq *);
    void (*task_tick)(struct rq *, struct task_struct *, int);
    void (*task_fork)(struct task_struct *);
    void (*task_dead)(struct task_struct *);
    void (*switched_from)(struct rq *, struct task_struct *);
    void (*switched_to)(struct rq *, struct task_struct *);
    void (*prio_changed)(struct rq *, struct task_struct *, int);
    unsigned int (*get_rr_interval)(struct rq *, struct task_struct *);
    void (*update_curr)(struct rq *);
    void (*task_change_group)(struct task_struct *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct sched_class {
    const struct sched_class *next;
    int uclamp_enabled;
    void (*enqueue_task)(struct rq *, struct task_struct *, int);
    void (*dequeue_task)(struct rq *, struct task_struct *, int);
    void (*yield_task)(struct rq *);
    bool (*yield_to_task)(struct rq *, struct task_struct *, bool);
    void (*check_preempt_curr)(struct rq *, struct task_struct *, int);
    struct task_struct * (*pick_next_task)(struct rq *);
    void (*put_prev_task)(struct rq *, struct task_struct *);
    void (*set_next_task)(struct rq *, struct task_struct *, bool);
    int (*balance)(struct rq *, struct task_struct *, struct rq_flags *);
    int (*select_task_rq)(struct task_struct *, int, int, int);
    void (*migrate_task_rq)(struct task_struct *, int);
    void (*task_woken)(struct rq *, struct task_struct *);
    void (*set_cpus_allowed)(struct task_struct *, const struct cpumask *);
    void (*rq_online)(struct rq *);
    void (*rq_offline)(struct rq *);
    void (*task_tick)(struct rq *, struct task_struct *, int);
    void (*task_fork)(struct task_struct *);
    void (*task_dead)(struct task_struct *);
    void (*switched_from)(struct rq *, struct task_struct *);
    void (*switched_to)(struct rq *, struct task_struct *);
    void (*prio_changed)(struct rq *, struct task_struct *, int);
    unsigned int (*get_rr_interval)(struct rq *, struct task_struct *);
    void (*update_curr)(struct rq *);
    void (*task_change_group)(struct task_struct *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct sched_class {
    int uclamp_enabled;
    void (*enqueue_task)(struct rq *, struct task_struct *, int);
    void (*dequeue_task)(struct rq *, struct task_struct *, int);
    void (*yield_task)(struct rq *);
    bool (*yield_to_task)(struct rq *, struct task_struct *);
    void (*check_preempt_curr)(struct rq *, struct task_struct *, int);
    struct task_struct * (*pick_next_task)(struct rq *);
    void (*put_prev_task)(struct rq *, struct task_struct *);
    void (*set_next_task)(struct rq *, struct task_struct *, bool);
    int (*balance)(struct rq *, struct task_struct *, struct rq_flags *);
    int (*select_task_rq)(struct task_struct *, int, int);
    void (*migrate_task_rq)(struct task_struct *, int);
    void (*task_woken)(struct rq *, struct task_struct *);
    void (*set_cpus_allowed)(struct task_struct *, const struct cpumask *, u32);
    void (*rq_online)(struct rq *);
    void (*rq_offline)(struct rq *);
    struct rq * (*find_lock_rq)(struct task_struct *, struct rq *);
    void (*task_tick)(struct rq *, struct task_struct *, int);
    void (*task_fork)(struct task_struct *);
    void (*task_dead)(struct task_struct *);
    void (*switched_from)(struct rq *, struct task_struct *);
    void (*switched_to)(struct rq *, struct task_struct *);
    void (*prio_changed)(struct rq *, struct task_struct *, int);
    unsigned int (*get_rr_interval)(struct rq *, struct task_struct *);
    void (*update_curr)(struct rq *);
    void (*task_change_group)(struct task_struct *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct sched_class {
    int uclamp_enabled;
    void (*enqueue_task)(struct rq *, struct task_struct *, int);
    void (*dequeue_task)(struct rq *, struct task_struct *, int);
    void (*yield_task)(struct rq *);
    bool (*yield_to_task)(struct rq *, struct task_struct *);
    void (*check_preempt_curr)(struct rq *, struct task_struct *, int);
    struct task_struct * (*pick_next_task)(struct rq *);
    void (*put_prev_task)(struct rq *, struct task_struct *);
    void (*set_next_task)(struct rq *, struct task_struct *, bool);
    int (*balance)(struct rq *, struct task_struct *, struct rq_flags *);
    int (*select_task_rq)(struct task_struct *, int, int);
    void (*migrate_task_rq)(struct task_struct *, int);
    void (*task_woken)(struct rq *, struct task_struct *);
    void (*set_cpus_allowed)(struct task_struct *, const struct cpumask *, u32);
    void (*rq_online)(struct rq *);
    void (*rq_offline)(struct rq *);
    struct rq * (*find_lock_rq)(struct task_struct *, struct rq *);
    void (*task_tick)(struct rq *, struct task_struct *, int);
    void (*task_fork)(struct task_struct *);
    void (*task_dead)(struct task_struct *);
    void (*switched_from)(struct rq *, struct task_struct *);
    void (*switched_to)(struct rq *, struct task_struct *);
    void (*prio_changed)(struct rq *, struct task_struct *, int);
    unsigned int (*get_rr_interval)(struct rq *, struct task_struct *);
    void (*update_curr)(struct rq *);
    void (*task_change_group)(struct task_struct *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct sched_class {
    int uclamp_enabled;
    void (*enqueue_task)(struct rq *, struct task_struct *, int);
    void (*dequeue_task)(struct rq *, struct task_struct *, int);
    void (*yield_task)(struct rq *);
    bool (*yield_to_task)(struct rq *, struct task_struct *);
    void (*check_preempt_curr)(struct rq *, struct task_struct *, int);
    struct task_struct * (*pick_next_task)(struct rq *);
    void (*put_prev_task)(struct rq *, struct task_struct *);
    void (*set_next_task)(struct rq *, struct task_struct *, bool);
    int (*balance)(struct rq *, struct task_struct *, struct rq_flags *);
    int (*select_task_rq)(struct task_struct *, int, int);
    struct task_struct * (*pick_task)(struct rq *);
    void (*migrate_task_rq)(struct task_struct *, int);
    void (*task_woken)(struct rq *, struct task_struct *);
    void (*set_cpus_allowed)(struct task_struct *, const struct cpumask *, u32);
    void (*rq_online)(struct rq *);
    void (*rq_offline)(struct rq *);
    struct rq * (*find_lock_rq)(struct task_struct *, struct rq *);
    void (*task_tick)(struct rq *, struct task_struct *, int);
    void (*task_fork)(struct task_struct *);
    void (*task_dead)(struct task_struct *);
    void (*switched_from)(struct rq *, struct task_struct *);
    void (*switched_to)(struct rq *, struct task_struct *);
    void (*prio_changed)(struct rq *, struct task_struct *, int);
    unsigned int (*get_rr_interval)(struct rq *, struct task_struct *);
    void (*update_curr)(struct rq *);
    void (*task_change_group)(struct task_struct *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct sched_class {
    int uclamp_enabled;
    void (*enqueue_task)(struct rq *, struct task_struct *, int);
    void (*dequeue_task)(struct rq *, struct task_struct *, int);
    void (*yield_task)(struct rq *);
    bool (*yield_to_task)(struct rq *, struct task_struct *);
    void (*check_preempt_curr)(struct rq *, struct task_struct *, int);
    struct task_struct * (*pick_next_task)(struct rq *);
    void (*put_prev_task)(struct rq *, struct task_struct *);
    void (*set_next_task)(struct rq *, struct task_struct *, bool);
    int (*balance)(struct rq *, struct task_struct *, struct rq_flags *);
    int (*select_task_rq)(struct task_struct *, int, int);
    struct task_struct * (*pick_task)(struct rq *);
    void (*migrate_task_rq)(struct task_struct *, int);
    void (*task_woken)(struct rq *, struct task_struct *);
    void (*set_cpus_allowed)(struct task_struct *, const struct cpumask *, u32);
    void (*rq_online)(struct rq *);
    void (*rq_offline)(struct rq *);
    struct rq * (*find_lock_rq)(struct task_struct *, struct rq *);
    void (*task_tick)(struct rq *, struct task_struct *, int);
    void (*task_fork)(struct task_struct *);
    void (*task_dead)(struct task_struct *);
    void (*switched_from)(struct rq *, struct task_struct *);
    void (*switched_to)(struct rq *, struct task_struct *);
    void (*prio_changed)(struct rq *, struct task_struct *, int);
    unsigned int (*get_rr_interval)(struct rq *, struct task_struct *);
    void (*update_curr)(struct rq *);
    void (*task_change_group)(struct task_struct *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct sched_class {
    int uclamp_enabled;
    void (*enqueue_task)(struct rq *, struct task_struct *, int);
    void (*dequeue_task)(struct rq *, struct task_struct *, int);
    void (*yield_task)(struct rq *);
    bool (*yield_to_task)(struct rq *, struct task_struct *);
    void (*check_preempt_curr)(struct rq *, struct task_struct *, int);
    struct task_struct * (*pick_next_task)(struct rq *);
    void (*put_prev_task)(struct rq *, struct task_struct *);
    void (*set_next_task)(struct rq *, struct task_struct *, bool);
    int (*balance)(struct rq *, struct task_struct *, struct rq_flags *);
    int (*select_task_rq)(struct task_struct *, int, int);
    struct task_struct * (*pick_task)(struct rq *);
    void (*migrate_task_rq)(struct task_struct *, int);
    void (*task_woken)(struct rq *, struct task_struct *);
    void (*set_cpus_allowed)(struct task_struct *, struct affinity_context *);
    void (*rq_online)(struct rq *);
    void (*rq_offline)(struct rq *);
    struct rq * (*find_lock_rq)(struct task_struct *, struct rq *);
    void (*task_tick)(struct rq *, struct task_struct *, int);
    void (*task_fork)(struct task_struct *);
    void (*task_dead)(struct task_struct *);
    void (*switched_from)(struct rq *, struct task_struct *);
    void (*switched_to)(struct rq *, struct task_struct *);
    void (*prio_changed)(struct rq *, struct task_struct *, int);
    unsigned int (*get_rr_interval)(struct rq *, struct task_struct *);
    void (*update_curr)(struct rq *);
    void (*task_change_group)(struct task_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct sched_class {
    int uclamp_enabled;
    void (*enqueue_task)(struct rq *, struct task_struct *, int);
    void (*dequeue_task)(struct rq *, struct task_struct *, int);
    void (*yield_task)(struct rq *);
    bool (*yield_to_task)(struct rq *, struct task_struct *);
    void (*check_preempt_curr)(struct rq *, struct task_struct *, int);
    struct task_struct * (*pick_next_task)(struct rq *);
    void (*put_prev_task)(struct rq *, struct task_struct *);
    void (*set_next_task)(struct rq *, struct task_struct *, bool);
    int (*balance)(struct rq *, struct task_struct *, struct rq_flags *);
    int (*select_task_rq)(struct task_struct *, int, int);
    struct task_struct * (*pick_task)(struct rq *);
    void (*migrate_task_rq)(struct task_struct *, int);
    void (*task_woken)(struct rq *, struct task_struct *);
    void (*set_cpus_allowed)(struct task_struct *, struct affinity_context *);
    void (*rq_online)(struct rq *);
    void (*rq_offline)(struct rq *);
    struct rq * (*find_lock_rq)(struct task_struct *, struct rq *);
    void (*task_tick)(struct rq *, struct task_struct *, int);
    void (*task_fork)(struct task_struct *);
    void (*task_dead)(struct task_struct *);
    void (*switched_from)(struct rq *, struct task_struct *);
    void (*switched_to)(struct rq *, struct task_struct *);
    void (*prio_changed)(struct rq *, struct task_struct *, int);
    unsigned int (*get_rr_interval)(struct rq *, struct task_struct *);
    void (*update_curr)(struct rq *);
    void (*task_change_group)(struct task_struct *);
    int (*task_is_throttled)(struct task_struct *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct sched_class {
    int uclamp_enabled;
    void (*enqueue_task)(struct rq *, struct task_struct *, int);
    void (*dequeue_task)(struct rq *, struct task_struct *, int);
    void (*yield_task)(struct rq *);
    bool (*yield_to_task)(struct rq *, struct task_struct *);
    void (*wakeup_preempt)(struct rq *, struct task_struct *, int);
    struct task_struct * (*pick_next_task)(struct rq *);
    void (*put_prev_task)(struct rq *, struct task_struct *);
    void (*set_next_task)(struct rq *, struct task_struct *, bool);
    int (*balance)(struct rq *, struct task_struct *, struct rq_flags *);
    int (*select_task_rq)(struct task_struct *, int, int);
    struct task_struct * (*pick_task)(struct rq *);
    void (*migrate_task_rq)(struct task_struct *, int);
    void (*task_woken)(struct rq *, struct task_struct *);
    void (*set_cpus_allowed)(struct task_struct *, struct affinity_context *);
    void (*rq_online)(struct rq *);
    void (*rq_offline)(struct rq *);
    struct rq * (*find_lock_rq)(struct task_struct *, struct rq *);
    void (*task_tick)(struct rq *, struct task_struct *, int);
    void (*task_fork)(struct task_struct *);
    void (*task_dead)(struct task_struct *);
    void (*switched_from)(struct rq *, struct task_struct *);
    void (*switched_to)(struct rq *, struct task_struct *);
    void (*prio_changed)(struct rq *, struct task_struct *, int);
    unsigned int (*get_rr_interval)(struct rq *, struct task_struct *);
    void (*update_curr)(struct rq *);
    void (*task_change_group)(struct task_struct *);
    int (*task_is_throttled)(struct task_struct *, int);
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
struct sched_class {
    const struct sched_class *next;
    int uclamp_enabled;
    void (*enqueue_task)(struct rq *, struct task_struct *, int);
    void (*dequeue_task)(struct rq *, struct task_struct *, int);
    void (*yield_task)(struct rq *);
    bool (*yield_to_task)(struct rq *, struct task_struct *, bool);
    void (*check_preempt_curr)(struct rq *, struct task_struct *, int);
    struct task_struct * (*pick_next_task)(struct rq *, struct task_struct *, struct rq_flags *);
    void (*put_prev_task)(struct rq *, struct task_struct *);
    void (*set_next_task)(struct rq *, struct task_struct *, bool);
    int (*balance)(struct rq *, struct task_struct *, struct rq_flags *);
    int (*select_task_rq)(struct task_struct *, int, int, int);
    void (*migrate_task_rq)(struct task_struct *, int);
    void (*task_woken)(struct rq *, struct task_struct *);
    void (*set_cpus_allowed)(struct task_struct *, const struct cpumask *);
    void (*rq_online)(struct rq *);
    void (*rq_offline)(struct rq *);
    void (*task_tick)(struct rq *, struct task_struct *, int);
    void (*task_fork)(struct task_struct *);
    void (*task_dead)(struct task_struct *);
    void (*switched_from)(struct rq *, struct task_struct *);
    void (*switched_to)(struct rq *, struct task_struct *);
    void (*prio_changed)(struct rq *, struct task_struct *, int);
    unsigned int (*get_rr_interval)(struct rq *, struct task_struct *);
    void (*update_curr)(struct rq *);
    void (*task_change_group)(struct task_struct *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct sched_class {
    const struct sched_class *next;
    int uclamp_enabled;
    void (*enqueue_task)(struct rq *, struct task_struct *, int);
    void (*dequeue_task)(struct rq *, struct task_struct *, int);
    void (*yield_task)(struct rq *);
    bool (*yield_to_task)(struct rq *, struct task_struct *, bool);
    void (*check_preempt_curr)(struct rq *, struct task_struct *, int);
    struct task_struct * (*pick_next_task)(struct rq *, struct task_struct *, struct rq_flags *);
    void (*put_prev_task)(struct rq *, struct task_struct *);
    void (*set_next_task)(struct rq *, struct task_struct *, bool);
    int (*balance)(struct rq *, struct task_struct *, struct rq_flags *);
    int (*select_task_rq)(struct task_struct *, int, int, int);
    void (*migrate_task_rq)(struct task_struct *, int);
    void (*task_woken)(struct rq *, struct task_struct *);
    void (*set_cpus_allowed)(struct task_struct *, const struct cpumask *);
    void (*rq_online)(struct rq *);
    void (*rq_offline)(struct rq *);
    void (*task_tick)(struct rq *, struct task_struct *, int);
    void (*task_fork)(struct task_struct *);
    void (*task_dead)(struct task_struct *);
    void (*switched_from)(struct rq *, struct task_struct *);
    void (*switched_to)(struct rq *, struct task_struct *);
    void (*prio_changed)(struct rq *, struct task_struct *, int);
    unsigned int (*get_rr_interval)(struct rq *, struct task_struct *);
    void (*update_curr)(struct rq *);
    void (*task_change_group)(struct task_struct *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct sched_class {
    const struct sched_class *next;
    int uclamp_enabled;
    void (*enqueue_task)(struct rq *, struct task_struct *, int);
    void (*dequeue_task)(struct rq *, struct task_struct *, int);
    void (*yield_task)(struct rq *);
    bool (*yield_to_task)(struct rq *, struct task_struct *, bool);
    void (*check_preempt_curr)(struct rq *, struct task_struct *, int);
    struct task_struct * (*pick_next_task)(struct rq *, struct task_struct *, struct rq_flags *);
    void (*put_prev_task)(struct rq *, struct task_struct *);
    void (*set_next_task)(struct rq *, struct task_struct *, bool);
    int (*balance)(struct rq *, struct task_struct *, struct rq_flags *);
    int (*select_task_rq)(struct task_struct *, int, int, int);
    void (*migrate_task_rq)(struct task_struct *, int);
    void (*task_woken)(struct rq *, struct task_struct *);
    void (*set_cpus_allowed)(struct task_struct *, const struct cpumask *);
    void (*rq_online)(struct rq *);
    void (*rq_offline)(struct rq *);
    void (*task_tick)(struct rq *, struct task_struct *, int);
    void (*task_fork)(struct task_struct *);
    void (*task_dead)(struct task_struct *);
    void (*switched_from)(struct rq *, struct task_struct *);
    void (*switched_to)(struct rq *, struct task_struct *);
    void (*prio_changed)(struct rq *, struct task_struct *, int);
    unsigned int (*get_rr_interval)(struct rq *, struct task_struct *);
    void (*update_curr)(struct rq *);
    void (*task_change_group)(struct task_struct *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct sched_class {
    const struct sched_class *next;
    void (*enqueue_task)(struct rq *, struct task_struct *, int);
    void (*dequeue_task)(struct rq *, struct task_struct *, int);
    void (*yield_task)(struct rq *);
    bool (*yield_to_task)(struct rq *, struct task_struct *, bool);
    void (*check_preempt_curr)(struct rq *, struct task_struct *, int);
    struct task_struct * (*pick_next_task)(struct rq *, struct task_struct *, struct rq_flags *);
    void (*put_prev_task)(struct rq *, struct task_struct *);
    void (*set_next_task)(struct rq *, struct task_struct *, bool);
    int (*balance)(struct rq *, struct task_struct *, struct rq_flags *);
    int (*select_task_rq)(struct task_struct *, int, int, int);
    void (*migrate_task_rq)(struct task_struct *, int);
    void (*task_woken)(struct rq *, struct task_struct *);
    void (*set_cpus_allowed)(struct task_struct *, const struct cpumask *);
    void (*rq_online)(struct rq *);
    void (*rq_offline)(struct rq *);
    void (*task_tick)(struct rq *, struct task_struct *, int);
    void (*task_fork)(struct task_struct *);
    void (*task_dead)(struct task_struct *);
    void (*switched_from)(struct rq *, struct task_struct *);
    void (*switched_to)(struct rq *, struct task_struct *);
    void (*prio_changed)(struct rq *, struct task_struct *, int);
    unsigned int (*get_rr_interval)(struct rq *, struct task_struct *);
    void (*update_curr)(struct rq *);
    void (*task_change_group)(struct task_struct *, int);
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
struct sched_class {
    const struct sched_class *next;
    int uclamp_enabled;
    void (*enqueue_task)(struct rq *, struct task_struct *, int);
    void (*dequeue_task)(struct rq *, struct task_struct *, int);
    void (*yield_task)(struct rq *);
    bool (*yield_to_task)(struct rq *, struct task_struct *, bool);
    void (*check_preempt_curr)(struct rq *, struct task_struct *, int);
    struct task_struct * (*pick_next_task)(struct rq *, struct task_struct *, struct rq_flags *);
    void (*put_prev_task)(struct rq *, struct task_struct *);
    void (*set_next_task)(struct rq *, struct task_struct *, bool);
    int (*balance)(struct rq *, struct task_struct *, struct rq_flags *);
    int (*select_task_rq)(struct task_struct *, int, int, int);
    void (*migrate_task_rq)(struct task_struct *, int);
    void (*task_woken)(struct rq *, struct task_struct *);
    void (*set_cpus_allowed)(struct task_struct *, const struct cpumask *);
    void (*rq_online)(struct rq *);
    void (*rq_offline)(struct rq *);
    void (*task_tick)(struct rq *, struct task_struct *, int);
    void (*task_fork)(struct task_struct *);
    void (*task_dead)(struct task_struct *);
    void (*switched_from)(struct rq *, struct task_struct *);
    void (*switched_to)(struct rq *, struct task_struct *);
    void (*prio_changed)(struct rq *, struct task_struct *, int);
    unsigned int (*get_rr_interval)(struct rq *, struct task_struct *);
    void (*update_curr)(struct rq *);
    void (*task_change_group)(struct task_struct *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct sched_class {
    const struct sched_class *next;
    int uclamp_enabled;
    void (*enqueue_task)(struct rq *, struct task_struct *, int);
    void (*dequeue_task)(struct rq *, struct task_struct *, int);
    void (*yield_task)(struct rq *);
    bool (*yield_to_task)(struct rq *, struct task_struct *, bool);
    void (*check_preempt_curr)(struct rq *, struct task_struct *, int);
    struct task_struct * (*pick_next_task)(struct rq *, struct task_struct *, struct rq_flags *);
    void (*put_prev_task)(struct rq *, struct task_struct *);
    void (*set_next_task)(struct rq *, struct task_struct *, bool);
    int (*balance)(struct rq *, struct task_struct *, struct rq_flags *);
    int (*select_task_rq)(struct task_struct *, int, int, int);
    void (*migrate_task_rq)(struct task_struct *, int);
    void (*task_woken)(struct rq *, struct task_struct *);
    void (*set_cpus_allowed)(struct task_struct *, const struct cpumask *);
    void (*rq_online)(struct rq *);
    void (*rq_offline)(struct rq *);
    void (*task_tick)(struct rq *, struct task_struct *, int);
    void (*task_fork)(struct task_struct *);
    void (*task_dead)(struct task_struct *);
    void (*switched_from)(struct rq *, struct task_struct *);
    void (*switched_to)(struct rq *, struct task_struct *);
    void (*prio_changed)(struct rq *, struct task_struct *, int);
    unsigned int (*get_rr_interval)(struct rq *, struct task_struct *);
    void (*update_curr)(struct rq *);
    void (*task_change_group)(struct task_struct *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct sched_class {
    const struct sched_class *next;
    void (*enqueue_task)(struct rq *, struct task_struct *, int);
    void (*dequeue_task)(struct rq *, struct task_struct *, int);
    void (*yield_task)(struct rq *);
    bool (*yield_to_task)(struct rq *, struct task_struct *, bool);
    void (*check_preempt_curr)(struct rq *, struct task_struct *, int);
    struct task_struct * (*pick_next_task)(struct rq *, struct task_struct *, struct rq_flags *);
    void (*put_prev_task)(struct rq *, struct task_struct *);
    void (*set_next_task)(struct rq *, struct task_struct *, bool);
    int (*balance)(struct rq *, struct task_struct *, struct rq_flags *);
    int (*select_task_rq)(struct task_struct *, int, int, int);
    void (*migrate_task_rq)(struct task_struct *, int);
    void (*task_woken)(struct rq *, struct task_struct *);
    void (*set_cpus_allowed)(struct task_struct *, const struct cpumask *);
    void (*rq_online)(struct rq *);
    void (*rq_offline)(struct rq *);
    void (*task_tick)(struct rq *, struct task_struct *, int);
    void (*task_fork)(struct task_struct *);
    void (*task_dead)(struct task_struct *);
    void (*switched_from)(struct rq *, struct task_struct *);
    void (*switched_to)(struct rq *, struct task_struct *);
    void (*prio_changed)(struct rq *, struct task_struct *, int);
    unsigned int (*get_rr_interval)(struct rq *, struct task_struct *);
    void (*update_curr)(struct rq *);
    void (*task_change_group)(struct task_struct *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct sched_class {
    const struct sched_class *next;
    int uclamp_enabled;
    void (*enqueue_task)(struct rq *, struct task_struct *, int);
    void (*dequeue_task)(struct rq *, struct task_struct *, int);
    void (*yield_task)(struct rq *);
    bool (*yield_to_task)(struct rq *, struct task_struct *, bool);
    void (*check_preempt_curr)(struct rq *, struct task_struct *, int);
    struct task_struct * (*pick_next_task)(struct rq *, struct task_struct *, struct rq_flags *);
    void (*put_prev_task)(struct rq *, struct task_struct *);
    void (*set_next_task)(struct rq *, struct task_struct *, bool);
    int (*balance)(struct rq *, struct task_struct *, struct rq_flags *);
    int (*select_task_rq)(struct task_struct *, int, int, int);
    void (*migrate_task_rq)(struct task_struct *, int);
    void (*task_woken)(struct rq *, struct task_struct *);
    void (*set_cpus_allowed)(struct task_struct *, const struct cpumask *);
    void (*rq_online)(struct rq *);
    void (*rq_offline)(struct rq *);
    void (*task_tick)(struct rq *, struct task_struct *, int);
    void (*task_fork)(struct task_struct *);
    void (*task_dead)(struct task_struct *);
    void (*switched_from)(struct rq *, struct task_struct *);
    void (*switched_to)(struct rq *, struct task_struct *);
    void (*prio_changed)(struct rq *, struct task_struct *, int);
    unsigned int (*get_rr_interval)(struct rq *, struct task_struct *);
    void (*update_curr)(struct rq *);
    void (*task_change_group)(struct task_struct *, int);
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
<b>Field added. </b>
<code>void (*task_change_group)(struct task_struct *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*task_waking)(struct task_struct *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*task_move_group)(struct task_struct *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct task_struct * (*pick_next_task)(struct rq *, struct task_struct *)</code> ➡️ <code>struct task_struct * (*pick_next_task)(struct rq *, struct task_struct *, struct pin_cookie)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct task_struct * (*pick_next_task)(struct rq *, struct task_struct *, struct pin_cookie)</code> ➡️ <code>struct task_struct * (*pick_next_task)(struct rq *, struct task_struct *, struct rq_flags *)</code>
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
<b>Field type changed. </b>
<code>void (*migrate_task_rq)(struct task_struct *)</code> ➡️ <code>void (*migrate_task_rq)(struct task_struct *, int)</code>
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
<code>int uclamp_enabled</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*set_next_task)(struct rq *, struct task_struct *, bool)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*balance)(struct rq *, struct task_struct *, struct rq_flags *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*set_curr_task)(struct rq *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct task_struct * (*pick_next_task)(struct rq *, struct task_struct *, struct rq_flags *)</code> ➡️ <code>struct task_struct * (*pick_next_task)(struct rq *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct rq * (*find_lock_rq)(struct task_struct *, struct rq *)</code>
</li>
<li>
<b>Field removed. </b>
<code>const struct sched_class *next</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool (*yield_to_task)(struct rq *, struct task_struct *, bool)</code> ➡️ <code>bool (*yield_to_task)(struct rq *, struct task_struct *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*select_task_rq)(struct task_struct *, int, int, int)</code> ➡️ <code>int (*select_task_rq)(struct task_struct *, int, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*set_cpus_allowed)(struct task_struct *, const struct cpumask *)</code> ➡️ <code>void (*set_cpus_allowed)(struct task_struct *, const struct cpumask *, u32)</code>
</li>
</ul>
</details>
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
<code>struct task_struct * (*pick_task)(struct rq *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>void (*set_cpus_allowed)(struct task_struct *, const struct cpumask *, u32)</code> ➡️ <code>void (*set_cpus_allowed)(struct task_struct *, struct affinity_context *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*task_change_group)(struct task_struct *, int)</code> ➡️ <code>void (*task_change_group)(struct task_struct *)</code>
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
<code>int (*task_is_throttled)(struct task_struct *, int)</code>
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
<code>void (*wakeup_preempt)(struct rq *, struct task_struct *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*check_preempt_curr)(struct rq *, struct task_struct *, int)</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int uclamp_enabled</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>generic</code> and <code>gcp</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int uclamp_enabled</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
