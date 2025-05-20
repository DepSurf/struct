# Struct: <code>rq</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct rq {
    raw_spinlock_t lock;
    unsigned int nr_running;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
    long unsigned int cpu_load[5];
    long unsigned int last_load_update_tick;
    u64 nohz_stamp;
    long unsigned int nohz_flags;
    struct load_weight load;
    long unsigned int nr_load_updates;
    u64 nr_switches;
    struct cfs_rq cfs;
    struct rt_rq rt;
    struct dl_rq dl;
    struct list_head leaf_cfs_rq_list;
    long unsigned int nr_uninterruptible;
    struct task_struct *curr;
    struct task_struct *idle;
    struct task_struct *stop;
    long unsigned int next_balance;
    struct mm_struct *prev_mm;
    unsigned int clock_skip_update;
    u64 clock;
    u64 clock_task;
    atomic_t nr_iowait;
    struct root_domain *rd;
    struct sched_domain *sd;
    long unsigned int cpu_capacity;
    long unsigned int cpu_capacity_orig;
    struct callback_head *balance_callback;
    unsigned char idle_balance;
    int active_balance;
    int push_cpu;
    struct cpu_stop_work active_balance_work;
    int cpu;
    int online;
    struct list_head cfs_tasks;
    u64 rt_avg;
    u64 age_stamp;
    u64 idle_stamp;
    u64 avg_idle;
    u64 max_idle_balance_cost;
    u64 prev_steal_time;
    long unsigned int calc_load_update;
    long int calc_load_active;
    int hrtick_csd_pending;
    struct call_single_data hrtick_csd;
    struct hrtimer hrtick_timer;
    struct sched_info rq_sched_info;
    long long unsigned int rq_cpu_time;
    unsigned int yld_count;
    unsigned int sched_count;
    unsigned int sched_goidle;
    unsigned int ttwu_count;
    unsigned int ttwu_local;
    struct llist_head wake_list;
    struct cpuidle_state *idle_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct rq {
    raw_spinlock_t lock;
    unsigned int nr_running;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
    long unsigned int cpu_load[5];
    long unsigned int last_load_update_tick;
    u64 nohz_stamp;
    long unsigned int nohz_flags;
    struct load_weight load;
    long unsigned int nr_load_updates;
    u64 nr_switches;
    struct cfs_rq cfs;
    struct rt_rq rt;
    struct dl_rq dl;
    struct list_head leaf_cfs_rq_list;
    long unsigned int nr_uninterruptible;
    struct task_struct *curr;
    struct task_struct *idle;
    struct task_struct *stop;
    long unsigned int next_balance;
    struct mm_struct *prev_mm;
    unsigned int clock_skip_update;
    u64 clock;
    u64 clock_task;
    atomic_t nr_iowait;
    struct root_domain *rd;
    struct sched_domain *sd;
    long unsigned int cpu_capacity;
    long unsigned int cpu_capacity_orig;
    struct callback_head *balance_callback;
    unsigned char idle_balance;
    int active_balance;
    int push_cpu;
    struct cpu_stop_work active_balance_work;
    int cpu;
    int online;
    struct list_head cfs_tasks;
    u64 rt_avg;
    u64 age_stamp;
    u64 idle_stamp;
    u64 avg_idle;
    u64 max_idle_balance_cost;
    u64 prev_steal_time;
    long unsigned int calc_load_update;
    long int calc_load_active;
    int hrtick_csd_pending;
    struct call_single_data hrtick_csd;
    struct hrtimer hrtick_timer;
    struct sched_info rq_sched_info;
    long long unsigned int rq_cpu_time;
    unsigned int yld_count;
    unsigned int sched_count;
    unsigned int sched_goidle;
    unsigned int ttwu_count;
    unsigned int ttwu_local;
    struct llist_head wake_list;
    struct cpuidle_state *idle_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rq {
    raw_spinlock_t lock;
    unsigned int nr_running;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
    long unsigned int cpu_load[5];
    long unsigned int last_load_update_tick;
    long unsigned int nohz_flags;
    struct load_weight load;
    long unsigned int nr_load_updates;
    u64 nr_switches;
    struct cfs_rq cfs;
    struct rt_rq rt;
    struct dl_rq dl;
    struct list_head leaf_cfs_rq_list;
    struct list_head *tmp_alone_branch;
    long unsigned int nr_uninterruptible;
    struct task_struct *curr;
    struct task_struct *idle;
    struct task_struct *stop;
    long unsigned int next_balance;
    struct mm_struct *prev_mm;
    unsigned int clock_skip_update;
    u64 clock;
    u64 clock_task;
    atomic_t nr_iowait;
    struct root_domain *rd;
    struct sched_domain *sd;
    long unsigned int cpu_capacity;
    long unsigned int cpu_capacity_orig;
    struct callback_head *balance_callback;
    unsigned char idle_balance;
    int active_balance;
    int push_cpu;
    struct cpu_stop_work active_balance_work;
    int cpu;
    int online;
    struct list_head cfs_tasks;
    u64 rt_avg;
    u64 age_stamp;
    u64 idle_stamp;
    u64 avg_idle;
    u64 max_idle_balance_cost;
    u64 prev_steal_time;
    long unsigned int calc_load_update;
    long int calc_load_active;
    int hrtick_csd_pending;
    struct call_single_data hrtick_csd;
    struct hrtimer hrtick_timer;
    struct sched_info rq_sched_info;
    long long unsigned int rq_cpu_time;
    unsigned int yld_count;
    unsigned int sched_count;
    unsigned int sched_goidle;
    unsigned int ttwu_count;
    unsigned int ttwu_local;
    struct llist_head wake_list;
    struct cpuidle_state *idle_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rq {
    raw_spinlock_t lock;
    unsigned int nr_running;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
    long unsigned int cpu_load[5];
    long unsigned int last_load_update_tick;
    long unsigned int nohz_flags;
    struct load_weight load;
    long unsigned int nr_load_updates;
    u64 nr_switches;
    struct cfs_rq cfs;
    struct rt_rq rt;
    struct dl_rq dl;
    struct list_head leaf_cfs_rq_list;
    struct list_head *tmp_alone_branch;
    long unsigned int nr_uninterruptible;
    struct task_struct *curr;
    struct task_struct *idle;
    struct task_struct *stop;
    long unsigned int next_balance;
    struct mm_struct *prev_mm;
    unsigned int clock_update_flags;
    u64 clock;
    u64 clock_task;
    atomic_t nr_iowait;
    struct root_domain *rd;
    struct sched_domain *sd;
    long unsigned int cpu_capacity;
    long unsigned int cpu_capacity_orig;
    struct callback_head *balance_callback;
    unsigned char idle_balance;
    int active_balance;
    int push_cpu;
    struct cpu_stop_work active_balance_work;
    int cpu;
    int online;
    struct list_head cfs_tasks;
    u64 rt_avg;
    u64 age_stamp;
    u64 idle_stamp;
    u64 avg_idle;
    u64 max_idle_balance_cost;
    u64 prev_steal_time;
    long unsigned int calc_load_update;
    long int calc_load_active;
    int hrtick_csd_pending;
    struct call_single_data hrtick_csd;
    struct hrtimer hrtick_timer;
    struct sched_info rq_sched_info;
    long long unsigned int rq_cpu_time;
    unsigned int yld_count;
    unsigned int sched_count;
    unsigned int sched_goidle;
    unsigned int ttwu_count;
    unsigned int ttwu_local;
    struct llist_head wake_list;
    struct cpuidle_state *idle_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rq {
    raw_spinlock_t lock;
    unsigned int nr_running;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
    long unsigned int cpu_load[5];
    long unsigned int last_load_update_tick;
    long unsigned int nohz_flags;
    struct load_weight load;
    long unsigned int nr_load_updates;
    u64 nr_switches;
    struct cfs_rq cfs;
    struct rt_rq rt;
    struct dl_rq dl;
    struct list_head leaf_cfs_rq_list;
    struct list_head *tmp_alone_branch;
    long unsigned int nr_uninterruptible;
    struct task_struct *curr;
    struct task_struct *idle;
    struct task_struct *stop;
    long unsigned int next_balance;
    struct mm_struct *prev_mm;
    unsigned int clock_update_flags;
    u64 clock;
    u64 clock_task;
    atomic_t nr_iowait;
    struct root_domain *rd;
    struct sched_domain *sd;
    long unsigned int cpu_capacity;
    long unsigned int cpu_capacity_orig;
    struct callback_head *balance_callback;
    unsigned char idle_balance;
    int active_balance;
    int push_cpu;
    struct cpu_stop_work active_balance_work;
    int cpu;
    int online;
    struct list_head cfs_tasks;
    u64 rt_avg;
    u64 age_stamp;
    u64 idle_stamp;
    u64 avg_idle;
    u64 max_idle_balance_cost;
    u64 prev_steal_time;
    long unsigned int calc_load_update;
    long int calc_load_active;
    int hrtick_csd_pending;
    call_single_data_t hrtick_csd;
    struct hrtimer hrtick_timer;
    struct sched_info rq_sched_info;
    long long unsigned int rq_cpu_time;
    unsigned int yld_count;
    unsigned int sched_count;
    unsigned int sched_goidle;
    unsigned int ttwu_count;
    unsigned int ttwu_local;
    struct llist_head wake_list;
    struct cpuidle_state *idle_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rq {
    raw_spinlock_t lock;
    unsigned int nr_running;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
    long unsigned int cpu_load[5];
    long unsigned int last_load_update_tick;
    long unsigned int last_blocked_load_update_tick;
    unsigned int has_blocked_load;
    unsigned int nohz_tick_stopped;
    atomic_t nohz_flags;
    struct load_weight load;
    long unsigned int nr_load_updates;
    u64 nr_switches;
    struct cfs_rq cfs;
    struct rt_rq rt;
    struct dl_rq dl;
    struct list_head leaf_cfs_rq_list;
    struct list_head *tmp_alone_branch;
    long unsigned int nr_uninterruptible;
    struct task_struct *curr;
    struct task_struct *idle;
    struct task_struct *stop;
    long unsigned int next_balance;
    struct mm_struct *prev_mm;
    unsigned int clock_update_flags;
    u64 clock;
    u64 clock_task;
    atomic_t nr_iowait;
    struct root_domain *rd;
    struct sched_domain *sd;
    long unsigned int cpu_capacity;
    long unsigned int cpu_capacity_orig;
    struct callback_head *balance_callback;
    unsigned char idle_balance;
    int active_balance;
    int push_cpu;
    struct cpu_stop_work active_balance_work;
    int cpu;
    int online;
    struct list_head cfs_tasks;
    u64 rt_avg;
    u64 age_stamp;
    u64 idle_stamp;
    u64 avg_idle;
    u64 max_idle_balance_cost;
    u64 prev_steal_time;
    long unsigned int calc_load_update;
    long int calc_load_active;
    int hrtick_csd_pending;
    call_single_data_t hrtick_csd;
    struct hrtimer hrtick_timer;
    struct sched_info rq_sched_info;
    long long unsigned int rq_cpu_time;
    unsigned int yld_count;
    unsigned int sched_count;
    unsigned int sched_goidle;
    unsigned int ttwu_count;
    unsigned int ttwu_local;
    struct llist_head wake_list;
    struct cpuidle_state *idle_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rq {
    raw_spinlock_t lock;
    unsigned int nr_running;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
    unsigned int numa_migrate_on;
    long unsigned int cpu_load[5];
    long unsigned int last_load_update_tick;
    long unsigned int last_blocked_load_update_tick;
    unsigned int has_blocked_load;
    unsigned int nohz_tick_stopped;
    atomic_t nohz_flags;
    struct load_weight load;
    long unsigned int nr_load_updates;
    u64 nr_switches;
    struct cfs_rq cfs;
    struct rt_rq rt;
    struct dl_rq dl;
    struct list_head leaf_cfs_rq_list;
    struct list_head *tmp_alone_branch;
    long unsigned int nr_uninterruptible;
    struct task_struct *curr;
    struct task_struct *idle;
    struct task_struct *stop;
    long unsigned int next_balance;
    struct mm_struct *prev_mm;
    unsigned int clock_update_flags;
    u64 clock;
    u64 clock_task;
    atomic_t nr_iowait;
    struct root_domain *rd;
    struct sched_domain *sd;
    long unsigned int cpu_capacity;
    long unsigned int cpu_capacity_orig;
    struct callback_head *balance_callback;
    unsigned char idle_balance;
    long unsigned int misfit_task_load;
    int active_balance;
    int push_cpu;
    struct cpu_stop_work active_balance_work;
    int cpu;
    int online;
    struct list_head cfs_tasks;
    struct sched_avg avg_rt;
    struct sched_avg avg_dl;
    u64 idle_stamp;
    u64 avg_idle;
    u64 max_idle_balance_cost;
    u64 prev_steal_time;
    long unsigned int calc_load_update;
    long int calc_load_active;
    int hrtick_csd_pending;
    call_single_data_t hrtick_csd;
    struct hrtimer hrtick_timer;
    struct sched_info rq_sched_info;
    long long unsigned int rq_cpu_time;
    unsigned int yld_count;
    unsigned int sched_count;
    unsigned int sched_goidle;
    unsigned int ttwu_count;
    unsigned int ttwu_local;
    struct llist_head wake_list;
    struct cpuidle_state *idle_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rq {
    raw_spinlock_t lock;
    unsigned int nr_running;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
    unsigned int numa_migrate_on;
    long unsigned int last_load_update_tick;
    long unsigned int last_blocked_load_update_tick;
    unsigned int has_blocked_load;
    unsigned int nohz_tick_stopped;
    atomic_t nohz_flags;
    long unsigned int nr_load_updates;
    u64 nr_switches;
    struct uclamp_rq uclamp[2];
    unsigned int uclamp_flags;
    struct cfs_rq cfs;
    struct rt_rq rt;
    struct dl_rq dl;
    struct list_head leaf_cfs_rq_list;
    struct list_head *tmp_alone_branch;
    long unsigned int nr_uninterruptible;
    struct task_struct *curr;
    struct task_struct *idle;
    struct task_struct *stop;
    long unsigned int next_balance;
    struct mm_struct *prev_mm;
    unsigned int clock_update_flags;
    u64 clock;
    u64 clock_task;
    u64 clock_pelt;
    long unsigned int lost_idle_time;
    atomic_t nr_iowait;
    struct root_domain *rd;
    struct sched_domain *sd;
    long unsigned int cpu_capacity;
    long unsigned int cpu_capacity_orig;
    struct callback_head *balance_callback;
    unsigned char idle_balance;
    long unsigned int misfit_task_load;
    int active_balance;
    int push_cpu;
    struct cpu_stop_work active_balance_work;
    int cpu;
    int online;
    struct list_head cfs_tasks;
    struct sched_avg avg_rt;
    struct sched_avg avg_dl;
    u64 idle_stamp;
    u64 avg_idle;
    u64 max_idle_balance_cost;
    u64 prev_steal_time;
    long unsigned int calc_load_update;
    long int calc_load_active;
    int hrtick_csd_pending;
    call_single_data_t hrtick_csd;
    struct hrtimer hrtick_timer;
    struct sched_info rq_sched_info;
    long long unsigned int rq_cpu_time;
    unsigned int yld_count;
    unsigned int sched_count;
    unsigned int sched_goidle;
    unsigned int ttwu_count;
    unsigned int ttwu_local;
    struct llist_head wake_list;
    struct cpuidle_state *idle_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rq {
    raw_spinlock_t lock;
    unsigned int nr_running;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
    unsigned int numa_migrate_on;
    long unsigned int last_load_update_tick;
    long unsigned int last_blocked_load_update_tick;
    unsigned int has_blocked_load;
    unsigned int nohz_tick_stopped;
    atomic_t nohz_flags;
    long unsigned int nr_load_updates;
    u64 nr_switches;
    struct uclamp_rq uclamp[2];
    unsigned int uclamp_flags;
    struct cfs_rq cfs;
    struct rt_rq rt;
    struct dl_rq dl;
    struct list_head leaf_cfs_rq_list;
    struct list_head *tmp_alone_branch;
    long unsigned int nr_uninterruptible;
    struct task_struct *curr;
    struct task_struct *idle;
    struct task_struct *stop;
    long unsigned int next_balance;
    struct mm_struct *prev_mm;
    unsigned int clock_update_flags;
    u64 clock;
    u64 clock_task;
    u64 clock_pelt;
    long unsigned int lost_idle_time;
    atomic_t nr_iowait;
    int membarrier_state;
    struct root_domain *rd;
    struct sched_domain *sd;
    long unsigned int cpu_capacity;
    long unsigned int cpu_capacity_orig;
    struct callback_head *balance_callback;
    unsigned char idle_balance;
    long unsigned int misfit_task_load;
    int active_balance;
    int push_cpu;
    struct cpu_stop_work active_balance_work;
    int cpu;
    int online;
    struct list_head cfs_tasks;
    struct sched_avg avg_rt;
    struct sched_avg avg_dl;
    u64 idle_stamp;
    u64 avg_idle;
    u64 max_idle_balance_cost;
    u64 prev_steal_time;
    long unsigned int calc_load_update;
    long int calc_load_active;
    int hrtick_csd_pending;
    call_single_data_t hrtick_csd;
    struct hrtimer hrtick_timer;
    struct sched_info rq_sched_info;
    long long unsigned int rq_cpu_time;
    unsigned int yld_count;
    unsigned int sched_count;
    unsigned int sched_goidle;
    unsigned int ttwu_count;
    unsigned int ttwu_local;
    struct llist_head wake_list;
    struct cpuidle_state *idle_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct rq {
    raw_spinlock_t lock;
    unsigned int nr_running;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
    unsigned int numa_migrate_on;
    long unsigned int last_blocked_load_update_tick;
    unsigned int has_blocked_load;
    call_single_data_t nohz_csd;
    unsigned int nohz_tick_stopped;
    atomic_t nohz_flags;
    unsigned int ttwu_pending;
    u64 nr_switches;
    struct uclamp_rq uclamp[2];
    unsigned int uclamp_flags;
    struct cfs_rq cfs;
    struct rt_rq rt;
    struct dl_rq dl;
    struct list_head leaf_cfs_rq_list;
    struct list_head *tmp_alone_branch;
    long unsigned int nr_uninterruptible;
    struct task_struct *curr;
    struct task_struct *idle;
    struct task_struct *stop;
    long unsigned int next_balance;
    struct mm_struct *prev_mm;
    unsigned int clock_update_flags;
    u64 clock;
    u64 clock_task;
    u64 clock_pelt;
    long unsigned int lost_idle_time;
    atomic_t nr_iowait;
    int membarrier_state;
    struct root_domain *rd;
    struct sched_domain *sd;
    long unsigned int cpu_capacity;
    long unsigned int cpu_capacity_orig;
    struct callback_head *balance_callback;
    unsigned char nohz_idle_balance;
    unsigned char idle_balance;
    long unsigned int misfit_task_load;
    int active_balance;
    int push_cpu;
    struct cpu_stop_work active_balance_work;
    int cpu;
    int online;
    struct list_head cfs_tasks;
    struct sched_avg avg_rt;
    struct sched_avg avg_dl;
    u64 idle_stamp;
    u64 avg_idle;
    u64 max_idle_balance_cost;
    u64 prev_steal_time;
    long unsigned int calc_load_update;
    long int calc_load_active;
    call_single_data_t hrtick_csd;
    struct hrtimer hrtick_timer;
    struct sched_info rq_sched_info;
    long long unsigned int rq_cpu_time;
    unsigned int yld_count;
    unsigned int sched_count;
    unsigned int sched_goidle;
    unsigned int ttwu_count;
    unsigned int ttwu_local;
    struct cpuidle_state *idle_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct rq {
    raw_spinlock_t lock;
    unsigned int nr_running;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
    unsigned int numa_migrate_on;
    long unsigned int last_blocked_load_update_tick;
    unsigned int has_blocked_load;
    call_single_data_t nohz_csd;
    unsigned int nohz_tick_stopped;
    atomic_t nohz_flags;
    unsigned int ttwu_pending;
    u64 nr_switches;
    struct uclamp_rq uclamp[2];
    unsigned int uclamp_flags;
    struct cfs_rq cfs;
    struct rt_rq rt;
    struct dl_rq dl;
    struct list_head leaf_cfs_rq_list;
    struct list_head *tmp_alone_branch;
    long unsigned int nr_uninterruptible;
    struct task_struct *curr;
    struct task_struct *idle;
    struct task_struct *stop;
    long unsigned int next_balance;
    struct mm_struct *prev_mm;
    unsigned int clock_update_flags;
    u64 clock;
    u64 clock_task;
    u64 clock_pelt;
    long unsigned int lost_idle_time;
    atomic_t nr_iowait;
    int membarrier_state;
    struct root_domain *rd;
    struct sched_domain *sd;
    long unsigned int cpu_capacity;
    long unsigned int cpu_capacity_orig;
    struct callback_head *balance_callback;
    unsigned char balance_push;
    unsigned char nohz_idle_balance;
    unsigned char idle_balance;
    long unsigned int misfit_task_load;
    int active_balance;
    int push_cpu;
    struct cpu_stop_work active_balance_work;
    int cpu;
    int online;
    struct list_head cfs_tasks;
    struct sched_avg avg_rt;
    struct sched_avg avg_dl;
    u64 idle_stamp;
    u64 avg_idle;
    u64 max_idle_balance_cost;
    struct rcuwait hotplug_wait;
    u64 prev_steal_time;
    long unsigned int calc_load_update;
    long int calc_load_active;
    call_single_data_t hrtick_csd;
    struct hrtimer hrtick_timer;
    ktime_t hrtick_time;
    struct sched_info rq_sched_info;
    long long unsigned int rq_cpu_time;
    unsigned int yld_count;
    unsigned int sched_count;
    unsigned int sched_goidle;
    unsigned int ttwu_count;
    unsigned int ttwu_local;
    struct cpuidle_state *idle_state;
    unsigned int nr_pinned;
    unsigned int push_busy;
    struct cpu_stop_work push_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rq {
    raw_spinlock_t lock;
    unsigned int nr_running;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
    unsigned int numa_migrate_on;
    long unsigned int last_blocked_load_update_tick;
    unsigned int has_blocked_load;
    call_single_data_t nohz_csd;
    unsigned int nohz_tick_stopped;
    atomic_t nohz_flags;
    unsigned int ttwu_pending;
    u64 nr_switches;
    struct uclamp_rq uclamp[2];
    unsigned int uclamp_flags;
    struct cfs_rq cfs;
    struct rt_rq rt;
    struct dl_rq dl;
    struct list_head leaf_cfs_rq_list;
    struct list_head *tmp_alone_branch;
    long unsigned int nr_uninterruptible;
    struct task_struct *curr;
    struct task_struct *idle;
    struct task_struct *stop;
    long unsigned int next_balance;
    struct mm_struct *prev_mm;
    unsigned int clock_update_flags;
    u64 clock;
    u64 clock_task;
    u64 clock_pelt;
    long unsigned int lost_idle_time;
    atomic_t nr_iowait;
    u64 last_seen_need_resched_ns;
    int ticks_without_resched;
    int membarrier_state;
    struct root_domain *rd;
    struct sched_domain *sd;
    long unsigned int cpu_capacity;
    long unsigned int cpu_capacity_orig;
    struct callback_head *balance_callback;
    unsigned char nohz_idle_balance;
    unsigned char idle_balance;
    long unsigned int misfit_task_load;
    int active_balance;
    int push_cpu;
    struct cpu_stop_work active_balance_work;
    int cpu;
    int online;
    struct list_head cfs_tasks;
    struct sched_avg avg_rt;
    struct sched_avg avg_dl;
    u64 idle_stamp;
    u64 avg_idle;
    u64 max_idle_balance_cost;
    struct rcuwait hotplug_wait;
    u64 prev_steal_time;
    long unsigned int calc_load_update;
    long int calc_load_active;
    call_single_data_t hrtick_csd;
    struct hrtimer hrtick_timer;
    ktime_t hrtick_time;
    struct sched_info rq_sched_info;
    long long unsigned int rq_cpu_time;
    unsigned int yld_count;
    unsigned int sched_count;
    unsigned int sched_goidle;
    unsigned int ttwu_count;
    unsigned int ttwu_local;
    struct cpuidle_state *idle_state;
    unsigned int nr_pinned;
    unsigned int push_busy;
    struct cpu_stop_work push_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rq {
    raw_spinlock_t __lock;
    unsigned int nr_running;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
    unsigned int numa_migrate_on;
    long unsigned int last_blocked_load_update_tick;
    unsigned int has_blocked_load;
    call_single_data_t nohz_csd;
    unsigned int nohz_tick_stopped;
    atomic_t nohz_flags;
    unsigned int ttwu_pending;
    u64 nr_switches;
    struct uclamp_rq uclamp[2];
    unsigned int uclamp_flags;
    struct cfs_rq cfs;
    struct rt_rq rt;
    struct dl_rq dl;
    struct list_head leaf_cfs_rq_list;
    struct list_head *tmp_alone_branch;
    unsigned int nr_uninterruptible;
    struct task_struct *curr;
    struct task_struct *idle;
    struct task_struct *stop;
    long unsigned int next_balance;
    struct mm_struct *prev_mm;
    unsigned int clock_update_flags;
    u64 clock;
    u64 clock_task;
    u64 clock_pelt;
    long unsigned int lost_idle_time;
    atomic_t nr_iowait;
    u64 last_seen_need_resched_ns;
    int ticks_without_resched;
    int membarrier_state;
    struct root_domain *rd;
    struct sched_domain *sd;
    long unsigned int cpu_capacity;
    long unsigned int cpu_capacity_orig;
    struct callback_head *balance_callback;
    unsigned char nohz_idle_balance;
    unsigned char idle_balance;
    long unsigned int misfit_task_load;
    int active_balance;
    int push_cpu;
    struct cpu_stop_work active_balance_work;
    int cpu;
    int online;
    struct list_head cfs_tasks;
    struct sched_avg avg_rt;
    struct sched_avg avg_dl;
    u64 idle_stamp;
    u64 avg_idle;
    long unsigned int wake_stamp;
    u64 wake_avg_idle;
    u64 max_idle_balance_cost;
    struct rcuwait hotplug_wait;
    u64 prev_steal_time;
    long unsigned int calc_load_update;
    long int calc_load_active;
    call_single_data_t hrtick_csd;
    struct hrtimer hrtick_timer;
    ktime_t hrtick_time;
    struct sched_info rq_sched_info;
    long long unsigned int rq_cpu_time;
    unsigned int yld_count;
    unsigned int sched_count;
    unsigned int sched_goidle;
    unsigned int ttwu_count;
    unsigned int ttwu_local;
    struct cpuidle_state *idle_state;
    unsigned int nr_pinned;
    unsigned int push_busy;
    struct cpu_stop_work push_work;
    struct rq *core;
    struct task_struct *core_pick;
    unsigned int core_enabled;
    unsigned int core_sched_seq;
    struct rb_root core_tree;
    unsigned int core_task_seq;
    unsigned int core_pick_seq;
    long unsigned int core_cookie;
    unsigned char core_forceidle;
    unsigned int core_forceidle_seq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rq {
    raw_spinlock_t __lock;
    unsigned int nr_running;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
    unsigned int numa_migrate_on;
    long unsigned int last_blocked_load_update_tick;
    unsigned int has_blocked_load;
    call_single_data_t nohz_csd;
    unsigned int nohz_tick_stopped;
    atomic_t nohz_flags;
    unsigned int ttwu_pending;
    u64 nr_switches;
    struct uclamp_rq uclamp[2];
    unsigned int uclamp_flags;
    struct cfs_rq cfs;
    struct rt_rq rt;
    struct dl_rq dl;
    struct list_head leaf_cfs_rq_list;
    struct list_head *tmp_alone_branch;
    unsigned int nr_uninterruptible;
    struct task_struct *curr;
    struct task_struct *idle;
    struct task_struct *stop;
    long unsigned int next_balance;
    struct mm_struct *prev_mm;
    unsigned int clock_update_flags;
    u64 clock;
    u64 clock_task;
    u64 clock_pelt;
    long unsigned int lost_idle_time;
    atomic_t nr_iowait;
    u64 last_seen_need_resched_ns;
    int ticks_without_resched;
    int membarrier_state;
    struct root_domain *rd;
    struct sched_domain *sd;
    long unsigned int cpu_capacity;
    long unsigned int cpu_capacity_orig;
    struct callback_head *balance_callback;
    unsigned char nohz_idle_balance;
    unsigned char idle_balance;
    long unsigned int misfit_task_load;
    int active_balance;
    int push_cpu;
    struct cpu_stop_work active_balance_work;
    int cpu;
    int online;
    struct list_head cfs_tasks;
    struct sched_avg avg_rt;
    struct sched_avg avg_dl;
    u64 idle_stamp;
    u64 avg_idle;
    long unsigned int wake_stamp;
    u64 wake_avg_idle;
    u64 max_idle_balance_cost;
    struct rcuwait hotplug_wait;
    u64 prev_steal_time;
    long unsigned int calc_load_update;
    long int calc_load_active;
    call_single_data_t hrtick_csd;
    struct hrtimer hrtick_timer;
    ktime_t hrtick_time;
    struct sched_info rq_sched_info;
    long long unsigned int rq_cpu_time;
    unsigned int yld_count;
    unsigned int sched_count;
    unsigned int sched_goidle;
    unsigned int ttwu_count;
    unsigned int ttwu_local;
    struct cpuidle_state *idle_state;
    unsigned int nr_pinned;
    unsigned int push_busy;
    struct cpu_stop_work push_work;
    struct rq *core;
    struct task_struct *core_pick;
    unsigned int core_enabled;
    unsigned int core_sched_seq;
    struct rb_root core_tree;
    unsigned int core_task_seq;
    unsigned int core_pick_seq;
    long unsigned int core_cookie;
    unsigned int core_forceidle_count;
    unsigned int core_forceidle_seq;
    unsigned int core_forceidle_occupation;
    u64 core_forceidle_start;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rq {
    raw_spinlock_t __lock;
    unsigned int nr_running;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
    unsigned int numa_migrate_on;
    long unsigned int last_blocked_load_update_tick;
    unsigned int has_blocked_load;
    call_single_data_t nohz_csd;
    unsigned int nohz_tick_stopped;
    atomic_t nohz_flags;
    unsigned int ttwu_pending;
    u64 nr_switches;
    struct uclamp_rq uclamp[2];
    unsigned int uclamp_flags;
    struct cfs_rq cfs;
    struct rt_rq rt;
    struct dl_rq dl;
    struct list_head leaf_cfs_rq_list;
    struct list_head *tmp_alone_branch;
    unsigned int nr_uninterruptible;
    struct task_struct *curr;
    struct task_struct *idle;
    struct task_struct *stop;
    long unsigned int next_balance;
    struct mm_struct *prev_mm;
    unsigned int clock_update_flags;
    u64 clock;
    u64 clock_task;
    u64 clock_pelt;
    long unsigned int lost_idle_time;
    u64 clock_pelt_idle;
    u64 clock_idle;
    atomic_t nr_iowait;
    u64 last_seen_need_resched_ns;
    int ticks_without_resched;
    int membarrier_state;
    struct root_domain *rd;
    struct sched_domain *sd;
    long unsigned int cpu_capacity;
    long unsigned int cpu_capacity_orig;
    long unsigned int cpu_capacity_inverted;
    struct balance_callback *balance_callback;
    unsigned char nohz_idle_balance;
    unsigned char idle_balance;
    long unsigned int misfit_task_load;
    int active_balance;
    int push_cpu;
    struct cpu_stop_work active_balance_work;
    int cpu;
    int online;
    struct list_head cfs_tasks;
    struct sched_avg avg_rt;
    struct sched_avg avg_dl;
    u64 idle_stamp;
    u64 avg_idle;
    long unsigned int wake_stamp;
    u64 wake_avg_idle;
    u64 max_idle_balance_cost;
    struct rcuwait hotplug_wait;
    u64 prev_steal_time;
    long unsigned int calc_load_update;
    long int calc_load_active;
    call_single_data_t hrtick_csd;
    struct hrtimer hrtick_timer;
    ktime_t hrtick_time;
    struct sched_info rq_sched_info;
    long long unsigned int rq_cpu_time;
    unsigned int yld_count;
    unsigned int sched_count;
    unsigned int sched_goidle;
    unsigned int ttwu_count;
    unsigned int ttwu_local;
    struct cpuidle_state *idle_state;
    unsigned int nr_pinned;
    unsigned int push_busy;
    struct cpu_stop_work push_work;
    struct rq *core;
    struct task_struct *core_pick;
    unsigned int core_enabled;
    unsigned int core_sched_seq;
    struct rb_root core_tree;
    unsigned int core_task_seq;
    unsigned int core_pick_seq;
    long unsigned int core_cookie;
    unsigned int core_forceidle_count;
    unsigned int core_forceidle_seq;
    unsigned int core_forceidle_occupation;
    u64 core_forceidle_start;
    cpumask_var_t scratch_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rq {
    raw_spinlock_t __lock;
    unsigned int nr_running;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
    unsigned int numa_migrate_on;
    long unsigned int last_blocked_load_update_tick;
    unsigned int has_blocked_load;
    call_single_data_t nohz_csd;
    unsigned int nohz_tick_stopped;
    atomic_t nohz_flags;
    unsigned int ttwu_pending;
    u64 nr_switches;
    struct uclamp_rq uclamp[2];
    unsigned int uclamp_flags;
    struct cfs_rq cfs;
    struct rt_rq rt;
    struct dl_rq dl;
    struct list_head leaf_cfs_rq_list;
    struct list_head *tmp_alone_branch;
    unsigned int nr_uninterruptible;
    struct task_struct *curr;
    struct task_struct *idle;
    struct task_struct *stop;
    long unsigned int next_balance;
    struct mm_struct *prev_mm;
    unsigned int clock_update_flags;
    u64 clock;
    u64 clock_task;
    u64 clock_pelt;
    long unsigned int lost_idle_time;
    u64 clock_pelt_idle;
    u64 clock_idle;
    atomic_t nr_iowait;
    u64 last_seen_need_resched_ns;
    int ticks_without_resched;
    int membarrier_state;
    struct root_domain *rd;
    struct sched_domain *sd;
    long unsigned int cpu_capacity;
    long unsigned int cpu_capacity_orig;
    struct balance_callback *balance_callback;
    unsigned char nohz_idle_balance;
    unsigned char idle_balance;
    long unsigned int misfit_task_load;
    int active_balance;
    int push_cpu;
    struct cpu_stop_work active_balance_work;
    int cpu;
    int online;
    struct list_head cfs_tasks;
    struct sched_avg avg_rt;
    struct sched_avg avg_dl;
    u64 idle_stamp;
    u64 avg_idle;
    long unsigned int wake_stamp;
    u64 wake_avg_idle;
    u64 max_idle_balance_cost;
    struct rcuwait hotplug_wait;
    u64 prev_steal_time;
    long unsigned int calc_load_update;
    long int calc_load_active;
    call_single_data_t hrtick_csd;
    struct hrtimer hrtick_timer;
    ktime_t hrtick_time;
    struct sched_info rq_sched_info;
    long long unsigned int rq_cpu_time;
    unsigned int yld_count;
    unsigned int sched_count;
    unsigned int sched_goidle;
    unsigned int ttwu_count;
    unsigned int ttwu_local;
    struct cpuidle_state *idle_state;
    unsigned int nr_pinned;
    unsigned int push_busy;
    struct cpu_stop_work push_work;
    struct rq *core;
    struct task_struct *core_pick;
    unsigned int core_enabled;
    unsigned int core_sched_seq;
    struct rb_root core_tree;
    unsigned int core_task_seq;
    unsigned int core_pick_seq;
    long unsigned int core_cookie;
    unsigned int core_forceidle_count;
    unsigned int core_forceidle_seq;
    unsigned int core_forceidle_occupation;
    u64 core_forceidle_start;
    cpumask_var_t scratch_mask;
    call_single_data_t cfsb_csd;
    struct list_head cfsb_csd_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rq {
    raw_spinlock_t __lock;
    unsigned int nr_running;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
    unsigned int numa_migrate_on;
    long unsigned int last_blocked_load_update_tick;
    unsigned int has_blocked_load;
    call_single_data_t nohz_csd;
    unsigned int nohz_tick_stopped;
    atomic_t nohz_flags;
    unsigned int ttwu_pending;
    u64 nr_switches;
    struct uclamp_rq uclamp[2];
    unsigned int uclamp_flags;
    struct cfs_rq cfs;
    struct rt_rq rt;
    struct dl_rq dl;
    struct list_head leaf_cfs_rq_list;
    struct list_head *tmp_alone_branch;
    unsigned int nr_uninterruptible;
    struct task_struct *curr;
    struct task_struct *idle;
    struct task_struct *stop;
    long unsigned int next_balance;
    struct mm_struct *prev_mm;
    unsigned int clock_update_flags;
    u64 clock;
    u64 clock_task;
    u64 clock_pelt;
    long unsigned int lost_idle_time;
    u64 clock_pelt_idle;
    u64 clock_idle;
    atomic_t nr_iowait;
    u64 last_seen_need_resched_ns;
    int ticks_without_resched;
    int membarrier_state;
    struct root_domain *rd;
    struct sched_domain *sd;
    long unsigned int cpu_capacity;
    struct balance_callback *balance_callback;
    unsigned char nohz_idle_balance;
    unsigned char idle_balance;
    long unsigned int misfit_task_load;
    int active_balance;
    int push_cpu;
    struct cpu_stop_work active_balance_work;
    int cpu;
    int online;
    struct list_head cfs_tasks;
    struct sched_avg avg_rt;
    struct sched_avg avg_dl;
    u64 idle_stamp;
    u64 avg_idle;
    u64 max_idle_balance_cost;
    struct rcuwait hotplug_wait;
    u64 prev_steal_time;
    long unsigned int calc_load_update;
    long int calc_load_active;
    call_single_data_t hrtick_csd;
    struct hrtimer hrtick_timer;
    ktime_t hrtick_time;
    struct sched_info rq_sched_info;
    long long unsigned int rq_cpu_time;
    unsigned int yld_count;
    unsigned int sched_count;
    unsigned int sched_goidle;
    unsigned int ttwu_count;
    unsigned int ttwu_local;
    struct cpuidle_state *idle_state;
    unsigned int nr_pinned;
    unsigned int push_busy;
    struct cpu_stop_work push_work;
    struct rq *core;
    struct task_struct *core_pick;
    unsigned int core_enabled;
    unsigned int core_sched_seq;
    struct rb_root core_tree;
    unsigned int core_task_seq;
    unsigned int core_pick_seq;
    long unsigned int core_cookie;
    unsigned int core_forceidle_count;
    unsigned int core_forceidle_seq;
    unsigned int core_forceidle_occupation;
    u64 core_forceidle_start;
    cpumask_var_t scratch_mask;
    call_single_data_t cfsb_csd;
    struct list_head cfsb_csd_list;
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
struct rq {
    raw_spinlock_t lock;
    unsigned int nr_running;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
    unsigned int numa_migrate_on;
    long unsigned int last_load_update_tick;
    long unsigned int last_blocked_load_update_tick;
    unsigned int has_blocked_load;
    unsigned int nohz_tick_stopped;
    atomic_t nohz_flags;
    long unsigned int nr_load_updates;
    u64 nr_switches;
    struct uclamp_rq uclamp[2];
    unsigned int uclamp_flags;
    struct cfs_rq cfs;
    struct rt_rq rt;
    struct dl_rq dl;
    struct list_head leaf_cfs_rq_list;
    struct list_head *tmp_alone_branch;
    long unsigned int nr_uninterruptible;
    struct task_struct *curr;
    struct task_struct *idle;
    struct task_struct *stop;
    long unsigned int next_balance;
    struct mm_struct *prev_mm;
    unsigned int clock_update_flags;
    u64 clock;
    u64 clock_task;
    u64 clock_pelt;
    long unsigned int lost_idle_time;
    atomic_t nr_iowait;
    int membarrier_state;
    struct root_domain *rd;
    struct sched_domain *sd;
    long unsigned int cpu_capacity;
    long unsigned int cpu_capacity_orig;
    struct callback_head *balance_callback;
    unsigned char idle_balance;
    long unsigned int misfit_task_load;
    int active_balance;
    int push_cpu;
    struct cpu_stop_work active_balance_work;
    int cpu;
    int online;
    struct list_head cfs_tasks;
    struct sched_avg avg_rt;
    struct sched_avg avg_dl;
    u64 idle_stamp;
    u64 avg_idle;
    u64 max_idle_balance_cost;
    u64 prev_steal_time;
    long unsigned int calc_load_update;
    long int calc_load_active;
    int hrtick_csd_pending;
    call_single_data_t hrtick_csd;
    struct hrtimer hrtick_timer;
    struct sched_info rq_sched_info;
    long long unsigned int rq_cpu_time;
    unsigned int yld_count;
    unsigned int sched_count;
    unsigned int sched_goidle;
    unsigned int ttwu_count;
    unsigned int ttwu_local;
    struct llist_head wake_list;
    struct cpuidle_state *idle_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rq {
    raw_spinlock_t lock;
    unsigned int nr_running;
    long unsigned int last_load_update_tick;
    long unsigned int last_blocked_load_update_tick;
    unsigned int has_blocked_load;
    unsigned int nohz_tick_stopped;
    atomic_t nohz_flags;
    long unsigned int nr_load_updates;
    u64 nr_switches;
    struct uclamp_rq uclamp[2];
    unsigned int uclamp_flags;
    struct cfs_rq cfs;
    struct rt_rq rt;
    struct dl_rq dl;
    struct list_head leaf_cfs_rq_list;
    struct list_head *tmp_alone_branch;
    long unsigned int nr_uninterruptible;
    struct task_struct *curr;
    struct task_struct *idle;
    struct task_struct *stop;
    long unsigned int next_balance;
    struct mm_struct *prev_mm;
    unsigned int clock_update_flags;
    u64 clock;
    u64 clock_task;
    u64 clock_pelt;
    long unsigned int lost_idle_time;
    atomic_t nr_iowait;
    int membarrier_state;
    struct root_domain *rd;
    struct sched_domain *sd;
    long unsigned int cpu_capacity;
    long unsigned int cpu_capacity_orig;
    struct callback_head *balance_callback;
    unsigned char idle_balance;
    long unsigned int misfit_task_load;
    int active_balance;
    int push_cpu;
    struct cpu_stop_work active_balance_work;
    int cpu;
    int online;
    struct list_head cfs_tasks;
    struct sched_avg avg_rt;
    struct sched_avg avg_dl;
    u64 idle_stamp;
    u64 avg_idle;
    u64 max_idle_balance_cost;
    long unsigned int calc_load_update;
    long int calc_load_active;
    int hrtick_csd_pending;
    call_single_data_t hrtick_csd;
    struct hrtimer hrtick_timer;
    struct sched_info rq_sched_info;
    long long unsigned int rq_cpu_time;
    unsigned int yld_count;
    unsigned int sched_count;
    unsigned int sched_goidle;
    unsigned int ttwu_count;
    unsigned int ttwu_local;
    struct llist_head wake_list;
    struct cpuidle_state *idle_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rq {
    raw_spinlock_t lock;
    unsigned int nr_running;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
    unsigned int numa_migrate_on;
    long unsigned int last_load_update_tick;
    long unsigned int last_blocked_load_update_tick;
    unsigned int has_blocked_load;
    unsigned int nohz_tick_stopped;
    atomic_t nohz_flags;
    long unsigned int nr_load_updates;
    u64 nr_switches;
    struct uclamp_rq uclamp[2];
    unsigned int uclamp_flags;
    struct cfs_rq cfs;
    struct rt_rq rt;
    struct dl_rq dl;
    struct list_head leaf_cfs_rq_list;
    struct list_head *tmp_alone_branch;
    long unsigned int nr_uninterruptible;
    struct task_struct *curr;
    struct task_struct *idle;
    struct task_struct *stop;
    long unsigned int next_balance;
    struct mm_struct *prev_mm;
    unsigned int clock_update_flags;
    u64 clock;
    u64 clock_task;
    u64 clock_pelt;
    long unsigned int lost_idle_time;
    atomic_t nr_iowait;
    int membarrier_state;
    struct root_domain *rd;
    struct sched_domain *sd;
    long unsigned int cpu_capacity;
    long unsigned int cpu_capacity_orig;
    struct callback_head *balance_callback;
    unsigned char idle_balance;
    long unsigned int misfit_task_load;
    int active_balance;
    int push_cpu;
    struct cpu_stop_work active_balance_work;
    int cpu;
    int online;
    struct list_head cfs_tasks;
    struct sched_avg avg_rt;
    struct sched_avg avg_dl;
    u64 idle_stamp;
    u64 avg_idle;
    u64 max_idle_balance_cost;
    long unsigned int calc_load_update;
    long int calc_load_active;
    int hrtick_csd_pending;
    call_single_data_t hrtick_csd;
    struct hrtimer hrtick_timer;
    struct sched_info rq_sched_info;
    long long unsigned int rq_cpu_time;
    unsigned int yld_count;
    unsigned int sched_count;
    unsigned int sched_goidle;
    unsigned int ttwu_count;
    unsigned int ttwu_local;
    struct llist_head wake_list;
    struct cpuidle_state *idle_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct rq {
    raw_spinlock_t lock;
    unsigned int nr_running;
    long unsigned int last_load_update_tick;
    long unsigned int last_blocked_load_update_tick;
    unsigned int has_blocked_load;
    unsigned int nohz_tick_stopped;
    atomic_t nohz_flags;
    long unsigned int nr_load_updates;
    u64 nr_switches;
    struct cfs_rq cfs;
    struct rt_rq rt;
    struct dl_rq dl;
    struct list_head leaf_cfs_rq_list;
    struct list_head *tmp_alone_branch;
    long unsigned int nr_uninterruptible;
    struct task_struct *curr;
    struct task_struct *idle;
    struct task_struct *stop;
    long unsigned int next_balance;
    struct mm_struct *prev_mm;
    unsigned int clock_update_flags;
    u64 clock;
    u64 clock_task;
    u64 clock_pelt;
    long unsigned int lost_idle_time;
    atomic_t nr_iowait;
    int membarrier_state;
    struct root_domain *rd;
    struct sched_domain *sd;
    long unsigned int cpu_capacity;
    long unsigned int cpu_capacity_orig;
    struct callback_head *balance_callback;
    unsigned char idle_balance;
    long unsigned int misfit_task_load;
    int active_balance;
    int push_cpu;
    struct cpu_stop_work active_balance_work;
    int cpu;
    int online;
    struct list_head cfs_tasks;
    struct sched_avg avg_rt;
    struct sched_avg avg_dl;
    u64 idle_stamp;
    u64 avg_idle;
    u64 max_idle_balance_cost;
    long unsigned int calc_load_update;
    long int calc_load_active;
    int hrtick_csd_pending;
    call_single_data_t hrtick_csd;
    struct hrtimer hrtick_timer;
    struct sched_info rq_sched_info;
    long long unsigned int rq_cpu_time;
    unsigned int yld_count;
    unsigned int sched_count;
    unsigned int sched_goidle;
    unsigned int ttwu_count;
    unsigned int ttwu_local;
    struct llist_head wake_list;
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
struct rq {
    raw_spinlock_t lock;
    unsigned int nr_running;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
    unsigned int numa_migrate_on;
    long unsigned int last_load_update_tick;
    long unsigned int last_blocked_load_update_tick;
    unsigned int has_blocked_load;
    unsigned int nohz_tick_stopped;
    atomic_t nohz_flags;
    long unsigned int nr_load_updates;
    u64 nr_switches;
    struct uclamp_rq uclamp[2];
    unsigned int uclamp_flags;
    struct cfs_rq cfs;
    struct rt_rq rt;
    struct dl_rq dl;
    struct list_head leaf_cfs_rq_list;
    struct list_head *tmp_alone_branch;
    long unsigned int nr_uninterruptible;
    struct task_struct *curr;
    struct task_struct *idle;
    struct task_struct *stop;
    long unsigned int next_balance;
    struct mm_struct *prev_mm;
    unsigned int clock_update_flags;
    u64 clock;
    u64 clock_task;
    u64 clock_pelt;
    long unsigned int lost_idle_time;
    atomic_t nr_iowait;
    int membarrier_state;
    struct root_domain *rd;
    struct sched_domain *sd;
    long unsigned int cpu_capacity;
    long unsigned int cpu_capacity_orig;
    struct callback_head *balance_callback;
    unsigned char idle_balance;
    long unsigned int misfit_task_load;
    int active_balance;
    int push_cpu;
    struct cpu_stop_work active_balance_work;
    int cpu;
    int online;
    struct list_head cfs_tasks;
    struct sched_avg avg_rt;
    struct sched_avg avg_dl;
    u64 idle_stamp;
    u64 avg_idle;
    u64 max_idle_balance_cost;
    u64 prev_steal_time;
    long unsigned int calc_load_update;
    long int calc_load_active;
    int hrtick_csd_pending;
    call_single_data_t hrtick_csd;
    struct hrtimer hrtick_timer;
    struct sched_info rq_sched_info;
    long long unsigned int rq_cpu_time;
    unsigned int yld_count;
    unsigned int sched_count;
    unsigned int sched_goidle;
    unsigned int ttwu_count;
    unsigned int ttwu_local;
    struct llist_head wake_list;
    struct cpuidle_state *idle_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rq {
    raw_spinlock_t lock;
    unsigned int nr_running;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
    unsigned int numa_migrate_on;
    long unsigned int last_load_update_tick;
    long unsigned int last_blocked_load_update_tick;
    unsigned int has_blocked_load;
    unsigned int nohz_tick_stopped;
    atomic_t nohz_flags;
    long unsigned int nr_load_updates;
    u64 nr_switches;
    struct uclamp_rq uclamp[2];
    unsigned int uclamp_flags;
    struct cfs_rq cfs;
    struct rt_rq rt;
    struct dl_rq dl;
    struct list_head leaf_cfs_rq_list;
    struct list_head *tmp_alone_branch;
    long unsigned int nr_uninterruptible;
    struct task_struct *curr;
    struct task_struct *idle;
    struct task_struct *stop;
    long unsigned int next_balance;
    struct mm_struct *prev_mm;
    unsigned int clock_update_flags;
    u64 clock;
    u64 clock_task;
    u64 clock_pelt;
    long unsigned int lost_idle_time;
    atomic_t nr_iowait;
    int membarrier_state;
    struct root_domain *rd;
    struct sched_domain *sd;
    long unsigned int cpu_capacity;
    long unsigned int cpu_capacity_orig;
    struct callback_head *balance_callback;
    unsigned char idle_balance;
    long unsigned int misfit_task_load;
    int active_balance;
    int push_cpu;
    struct cpu_stop_work active_balance_work;
    int cpu;
    int online;
    struct list_head cfs_tasks;
    struct sched_avg avg_rt;
    struct sched_avg avg_dl;
    u64 idle_stamp;
    u64 avg_idle;
    u64 max_idle_balance_cost;
    u64 prev_steal_time;
    long unsigned int calc_load_update;
    long int calc_load_active;
    int hrtick_csd_pending;
    call_single_data_t hrtick_csd;
    struct hrtimer hrtick_timer;
    struct sched_info rq_sched_info;
    long long unsigned int rq_cpu_time;
    unsigned int yld_count;
    unsigned int sched_count;
    unsigned int sched_goidle;
    unsigned int ttwu_count;
    unsigned int ttwu_local;
    struct llist_head wake_list;
    struct cpuidle_state *idle_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rq {
    raw_spinlock_t lock;
    unsigned int nr_running;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
    unsigned int numa_migrate_on;
    long unsigned int last_load_update_tick;
    long unsigned int last_blocked_load_update_tick;
    unsigned int has_blocked_load;
    unsigned int nohz_tick_stopped;
    atomic_t nohz_flags;
    long unsigned int nr_load_updates;
    u64 nr_switches;
    struct cfs_rq cfs;
    struct rt_rq rt;
    struct dl_rq dl;
    struct list_head leaf_cfs_rq_list;
    struct list_head *tmp_alone_branch;
    long unsigned int nr_uninterruptible;
    struct task_struct *curr;
    struct task_struct *idle;
    struct task_struct *stop;
    long unsigned int next_balance;
    struct mm_struct *prev_mm;
    unsigned int clock_update_flags;
    u64 clock;
    u64 clock_task;
    u64 clock_pelt;
    long unsigned int lost_idle_time;
    atomic_t nr_iowait;
    int membarrier_state;
    struct root_domain *rd;
    struct sched_domain *sd;
    long unsigned int cpu_capacity;
    long unsigned int cpu_capacity_orig;
    struct callback_head *balance_callback;
    unsigned char idle_balance;
    long unsigned int misfit_task_load;
    int active_balance;
    int push_cpu;
    struct cpu_stop_work active_balance_work;
    int cpu;
    int online;
    struct list_head cfs_tasks;
    struct sched_avg avg_rt;
    struct sched_avg avg_dl;
    u64 idle_stamp;
    u64 avg_idle;
    u64 max_idle_balance_cost;
    u64 prev_steal_time;
    long unsigned int calc_load_update;
    long int calc_load_active;
    int hrtick_csd_pending;
    call_single_data_t hrtick_csd;
    struct hrtimer hrtick_timer;
    struct sched_info rq_sched_info;
    long long unsigned int rq_cpu_time;
    unsigned int yld_count;
    unsigned int sched_count;
    unsigned int sched_goidle;
    unsigned int ttwu_count;
    unsigned int ttwu_local;
    struct llist_head wake_list;
    struct cpuidle_state *idle_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rq {
    raw_spinlock_t lock;
    unsigned int nr_running;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
    unsigned int numa_migrate_on;
    long unsigned int last_load_update_tick;
    long unsigned int last_blocked_load_update_tick;
    unsigned int has_blocked_load;
    unsigned int nohz_tick_stopped;
    atomic_t nohz_flags;
    long unsigned int nr_load_updates;
    u64 nr_switches;
    struct uclamp_rq uclamp[2];
    unsigned int uclamp_flags;
    struct cfs_rq cfs;
    struct rt_rq rt;
    struct dl_rq dl;
    struct list_head leaf_cfs_rq_list;
    struct list_head *tmp_alone_branch;
    long unsigned int nr_uninterruptible;
    struct task_struct *curr;
    struct task_struct *idle;
    struct task_struct *stop;
    long unsigned int next_balance;
    struct mm_struct *prev_mm;
    unsigned int clock_update_flags;
    u64 clock;
    u64 clock_task;
    u64 clock_pelt;
    long unsigned int lost_idle_time;
    atomic_t nr_iowait;
    int membarrier_state;
    struct root_domain *rd;
    struct sched_domain *sd;
    long unsigned int cpu_capacity;
    long unsigned int cpu_capacity_orig;
    struct callback_head *balance_callback;
    unsigned char idle_balance;
    long unsigned int misfit_task_load;
    int active_balance;
    int push_cpu;
    struct cpu_stop_work active_balance_work;
    int cpu;
    int online;
    struct list_head cfs_tasks;
    struct sched_avg avg_rt;
    struct sched_avg avg_dl;
    u64 idle_stamp;
    u64 avg_idle;
    u64 max_idle_balance_cost;
    u64 prev_steal_time;
    long unsigned int calc_load_update;
    long int calc_load_active;
    int hrtick_csd_pending;
    call_single_data_t hrtick_csd;
    struct hrtimer hrtick_timer;
    struct sched_info rq_sched_info;
    long long unsigned int rq_cpu_time;
    unsigned int yld_count;
    unsigned int sched_count;
    unsigned int sched_goidle;
    unsigned int ttwu_count;
    unsigned int ttwu_local;
    struct llist_head wake_list;
    struct cpuidle_state *idle_state;
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
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head *tmp_alone_branch</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 nohz_stamp</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int clock_update_flags</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int clock_skip_update</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct call_single_data hrtick_csd</code> ➡️ <code>call_single_data_t hrtick_csd</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int last_blocked_load_update_tick</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int has_blocked_load</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int nohz_tick_stopped</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int nohz_flags</code> ➡️ <code>atomic_t nohz_flags</code>
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
<code>unsigned int numa_migrate_on</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int misfit_task_load</code>
</li>
<li>
<b>Field added. </b>
<code>struct sched_avg avg_rt</code>
</li>
<li>
<b>Field added. </b>
<code>struct sched_avg avg_dl</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 rt_avg</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 age_stamp</code>
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
<code>struct uclamp_rq uclamp[2]</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int uclamp_flags</code>
</li>
<li>
<b>Field added. </b>
<code>u64 clock_pelt</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int lost_idle_time</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int cpu_load[5]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct load_weight load</code>
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
<code>int membarrier_state</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>call_single_data_t nohz_csd</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int ttwu_pending</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned char nohz_idle_balance</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int last_load_update_tick</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int nr_load_updates</code>
</li>
<li>
<b>Field removed. </b>
<code>int hrtick_csd_pending</code>
</li>
<li>
<b>Field removed. </b>
<code>struct llist_head wake_list</code>
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
<code>unsigned char balance_push</code>
</li>
<li>
<b>Field added. </b>
<code>struct rcuwait hotplug_wait</code>
</li>
<li>
<b>Field added. </b>
<code>ktime_t hrtick_time</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int nr_pinned</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int push_busy</code>
</li>
<li>
<b>Field added. </b>
<code>struct cpu_stop_work push_work</code>
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
<code>u64 last_seen_need_resched_ns</code>
</li>
<li>
<b>Field added. </b>
<code>int ticks_without_resched</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned char balance_push</code>
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
<code>raw_spinlock_t __lock</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int wake_stamp</code>
</li>
<li>
<b>Field added. </b>
<code>u64 wake_avg_idle</code>
</li>
<li>
<b>Field added. </b>
<code>struct rq *core</code>
</li>
<li>
<b>Field added. </b>
<code>struct task_struct *core_pick</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int core_enabled</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int core_sched_seq</code>
</li>
<li>
<b>Field added. </b>
<code>struct rb_root core_tree</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int core_task_seq</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int core_pick_seq</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int core_cookie</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned char core_forceidle</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int core_forceidle_seq</code>
</li>
<li>
<b>Field removed. </b>
<code>raw_spinlock_t lock</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int nr_uninterruptible</code> ➡️ <code>unsigned int nr_uninterruptible</code>
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
<code>unsigned int core_forceidle_count</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int core_forceidle_occupation</code>
</li>
<li>
<b>Field added. </b>
<code>u64 core_forceidle_start</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned char core_forceidle</code>
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
<code>u64 clock_pelt_idle</code>
</li>
<li>
<b>Field added. </b>
<code>u64 clock_idle</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int cpu_capacity_inverted</code>
</li>
<li>
<b>Field added. </b>
<code>cpumask_var_t scratch_mask</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct callback_head *balance_callback</code> ➡️ <code>struct balance_callback *balance_callback</code>
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
<code>call_single_data_t cfsb_csd</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head cfsb_csd_list</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int cpu_capacity_inverted</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>long unsigned int cpu_capacity_orig</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int wake_stamp</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 wake_avg_idle</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned int nr_numa_running</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int nr_preferred_running</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int numa_migrate_on</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 prev_steal_time</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>u64 prev_steal_time</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned int nr_numa_running</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int nr_preferred_running</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int numa_migrate_on</code>
</li>
<li>
<b>Field removed. </b>
<code>struct uclamp_rq uclamp[2]</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int uclamp_flags</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 prev_steal_time</code>
</li>
<li>
<b>Field removed. </b>
<code>struct cpuidle_state *idle_state</code>
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
<code>struct uclamp_rq uclamp[2]</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int uclamp_flags</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
