# Struct: <code>rcu_state</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct rcu_state {
    struct rcu_node node[5];
    struct rcu_node * level[3];
    u8 flavor_mask;
    struct rcu_data *rda;
    call_rcu_func_t call;
    int ncpus;
    u8 boost;
    long unsigned int gpnum;
    long unsigned int completed;
    struct task_struct *gp_kthread;
    wait_queue_head_t gp_wq;
    short int gp_flags;
    short int gp_state;
    raw_spinlock_t orphan_lock;
    struct callback_head *orphan_nxtlist;
    struct callback_head **orphan_nxttail;
    struct callback_head *orphan_donelist;
    struct callback_head **orphan_donetail;
    long int qlen_lazy;
    long int qlen;
    struct mutex barrier_mutex;
    atomic_t barrier_cpu_count;
    struct completion barrier_completion;
    long unsigned int barrier_sequence;
    long unsigned int expedited_sequence;
    atomic_long_t expedited_workdone0;
    atomic_long_t expedited_workdone1;
    atomic_long_t expedited_workdone2;
    atomic_long_t expedited_workdone3;
    atomic_long_t expedited_normal;
    atomic_t expedited_need_qs;
    wait_queue_head_t expedited_wq;
    int ncpus_snap;
    long unsigned int jiffies_force_qs;
    long unsigned int n_force_qs;
    long unsigned int n_force_qs_lh;
    long unsigned int n_force_qs_ngp;
    long unsigned int gp_start;
    long unsigned int gp_activity;
    long unsigned int jiffies_stall;
    long unsigned int jiffies_resched;
    long unsigned int n_force_qs_gpstart;
    long unsigned int gp_max;
    const char *name;
    char abbr;
    struct list_head flavors;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct rcu_state {
    struct rcu_node node[5];
    struct rcu_node * level[3];
    u8 flavor_mask;
    struct rcu_data *rda;
    call_rcu_func_t call;
    int ncpus;
    u8 boost;
    long unsigned int gpnum;
    long unsigned int completed;
    struct task_struct *gp_kthread;
    struct swait_queue_head gp_wq;
    short int gp_flags;
    short int gp_state;
    raw_spinlock_t orphan_lock;
    struct callback_head *orphan_nxtlist;
    struct callback_head **orphan_nxttail;
    struct callback_head *orphan_donelist;
    struct callback_head **orphan_donetail;
    long int qlen_lazy;
    long int qlen;
    struct mutex barrier_mutex;
    atomic_t barrier_cpu_count;
    struct completion barrier_completion;
    long unsigned int barrier_sequence;
    struct mutex exp_mutex;
    struct mutex exp_wake_mutex;
    long unsigned int expedited_sequence;
    atomic_long_t expedited_normal;
    atomic_t expedited_need_qs;
    struct swait_queue_head expedited_wq;
    int ncpus_snap;
    long unsigned int jiffies_force_qs;
    long unsigned int jiffies_kick_kthreads;
    long unsigned int n_force_qs;
    long unsigned int n_force_qs_lh;
    long unsigned int n_force_qs_ngp;
    long unsigned int gp_start;
    long unsigned int gp_activity;
    long unsigned int jiffies_stall;
    long unsigned int jiffies_resched;
    long unsigned int n_force_qs_gpstart;
    long unsigned int gp_max;
    const char *name;
    char abbr;
    struct list_head flavors;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rcu_state {
    struct rcu_node node[131];
    struct rcu_node * level[4];
    u8 flavor_mask;
    struct rcu_data *rda;
    call_rcu_func_t call;
    int ncpus;
    u8 boost;
    long unsigned int gpnum;
    long unsigned int completed;
    struct task_struct *gp_kthread;
    struct swait_queue_head gp_wq;
    short int gp_flags;
    short int gp_state;
    raw_spinlock_t orphan_lock;
    struct callback_head *orphan_nxtlist;
    struct callback_head **orphan_nxttail;
    struct callback_head *orphan_donelist;
    struct callback_head **orphan_donetail;
    long int qlen_lazy;
    long int qlen;
    struct mutex barrier_mutex;
    atomic_t barrier_cpu_count;
    struct completion barrier_completion;
    long unsigned int barrier_sequence;
    struct mutex exp_mutex;
    struct mutex exp_wake_mutex;
    long unsigned int expedited_sequence;
    atomic_long_t expedited_normal;
    atomic_t expedited_need_qs;
    struct swait_queue_head expedited_wq;
    int ncpus_snap;
    long unsigned int jiffies_force_qs;
    long unsigned int jiffies_kick_kthreads;
    long unsigned int n_force_qs;
    long unsigned int n_force_qs_lh;
    long unsigned int n_force_qs_ngp;
    long unsigned int gp_start;
    long unsigned int gp_activity;
    long unsigned int jiffies_stall;
    long unsigned int jiffies_resched;
    long unsigned int n_force_qs_gpstart;
    long unsigned int gp_max;
    const char *name;
    char abbr;
    struct list_head flavors;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rcu_state {
    struct rcu_node node[521];
    struct rcu_node * level[4];
    struct rcu_data *rda;
    call_rcu_func_t call;
    int ncpus;
    u8 boost;
    long unsigned int gpnum;
    long unsigned int completed;
    struct task_struct *gp_kthread;
    struct swait_queue_head gp_wq;
    short int gp_flags;
    short int gp_state;
    raw_spinlock_t orphan_lock;
    struct rcu_cblist orphan_pend;
    struct rcu_cblist orphan_done;
    struct mutex barrier_mutex;
    atomic_t barrier_cpu_count;
    struct completion barrier_completion;
    long unsigned int barrier_sequence;
    struct mutex exp_mutex;
    struct mutex exp_wake_mutex;
    long unsigned int expedited_sequence;
    atomic_t expedited_need_qs;
    struct swait_queue_head expedited_wq;
    int ncpus_snap;
    long unsigned int jiffies_force_qs;
    long unsigned int jiffies_kick_kthreads;
    long unsigned int n_force_qs;
    long unsigned int n_force_qs_lh;
    long unsigned int n_force_qs_ngp;
    long unsigned int gp_start;
    long unsigned int gp_activity;
    long unsigned int jiffies_stall;
    long unsigned int jiffies_resched;
    long unsigned int n_force_qs_gpstart;
    long unsigned int gp_max;
    const char *name;
    char abbr;
    struct list_head flavors;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rcu_state {
    struct rcu_node node[521];
    struct rcu_node * level[4];
    struct rcu_data *rda;
    call_rcu_func_t call;
    int ncpus;
    u8 boost;
    long unsigned int gpnum;
    long unsigned int completed;
    struct task_struct *gp_kthread;
    struct swait_queue_head gp_wq;
    short int gp_flags;
    short int gp_state;
    struct mutex barrier_mutex;
    atomic_t barrier_cpu_count;
    struct completion barrier_completion;
    long unsigned int barrier_sequence;
    struct mutex exp_mutex;
    struct mutex exp_wake_mutex;
    long unsigned int expedited_sequence;
    atomic_t expedited_need_qs;
    struct swait_queue_head expedited_wq;
    int ncpus_snap;
    long unsigned int jiffies_force_qs;
    long unsigned int jiffies_kick_kthreads;
    long unsigned int n_force_qs;
    long unsigned int n_force_qs_lh;
    long unsigned int n_force_qs_ngp;
    long unsigned int gp_start;
    long unsigned int gp_activity;
    long unsigned int jiffies_stall;
    long unsigned int jiffies_resched;
    long unsigned int n_force_qs_gpstart;
    long unsigned int gp_max;
    const char *name;
    char abbr;
    struct list_head flavors;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rcu_state {
    struct rcu_node node[521];
    struct rcu_node * level[4];
    struct rcu_data *rda;
    call_rcu_func_t call;
    int ncpus;
    u8 boost;
    long unsigned int gpnum;
    long unsigned int completed;
    struct task_struct *gp_kthread;
    struct swait_queue_head gp_wq;
    short int gp_flags;
    short int gp_state;
    struct mutex barrier_mutex;
    atomic_t barrier_cpu_count;
    struct completion barrier_completion;
    long unsigned int barrier_sequence;
    struct mutex exp_mutex;
    struct mutex exp_wake_mutex;
    long unsigned int expedited_sequence;
    atomic_t expedited_need_qs;
    struct swait_queue_head expedited_wq;
    int ncpus_snap;
    long unsigned int jiffies_force_qs;
    long unsigned int jiffies_kick_kthreads;
    long unsigned int n_force_qs;
    long unsigned int gp_start;
    long unsigned int gp_activity;
    long unsigned int jiffies_stall;
    long unsigned int jiffies_resched;
    long unsigned int n_force_qs_gpstart;
    long unsigned int gp_max;
    const char *name;
    char abbr;
    struct list_head flavors;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rcu_state {
    struct rcu_node node[521];
    struct rcu_node * level[4];
    int ncpus;
    u8 boost;
    long unsigned int gp_seq;
    struct task_struct *gp_kthread;
    struct swait_queue_head gp_wq;
    short int gp_flags;
    short int gp_state;
    struct mutex barrier_mutex;
    atomic_t barrier_cpu_count;
    struct completion barrier_completion;
    long unsigned int barrier_sequence;
    struct mutex exp_mutex;
    struct mutex exp_wake_mutex;
    long unsigned int expedited_sequence;
    atomic_t expedited_need_qs;
    struct swait_queue_head expedited_wq;
    int ncpus_snap;
    long unsigned int jiffies_force_qs;
    long unsigned int jiffies_kick_kthreads;
    long unsigned int n_force_qs;
    long unsigned int gp_start;
    long unsigned int gp_end;
    long unsigned int gp_activity;
    long unsigned int gp_req_activity;
    long unsigned int jiffies_stall;
    long unsigned int jiffies_resched;
    long unsigned int n_force_qs_gpstart;
    long unsigned int gp_max;
    const char *name;
    char abbr;
    raw_spinlock_t ofl_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rcu_state {
    struct rcu_node node[521];
    struct rcu_node * level[4];
    int ncpus;
    u8 boost;
    long unsigned int gp_seq;
    struct task_struct *gp_kthread;
    struct swait_queue_head gp_wq;
    short int gp_flags;
    short int gp_state;
    long unsigned int gp_wake_time;
    long unsigned int gp_wake_seq;
    struct mutex barrier_mutex;
    atomic_t barrier_cpu_count;
    struct completion barrier_completion;
    long unsigned int barrier_sequence;
    struct mutex exp_mutex;
    struct mutex exp_wake_mutex;
    long unsigned int expedited_sequence;
    atomic_t expedited_need_qs;
    struct swait_queue_head expedited_wq;
    int ncpus_snap;
    long unsigned int jiffies_force_qs;
    long unsigned int jiffies_kick_kthreads;
    long unsigned int n_force_qs;
    long unsigned int gp_start;
    long unsigned int gp_end;
    long unsigned int gp_activity;
    long unsigned int gp_req_activity;
    long unsigned int jiffies_stall;
    long unsigned int jiffies_resched;
    long unsigned int n_force_qs_gpstart;
    long unsigned int gp_max;
    const char *name;
    char abbr;
    raw_spinlock_t ofl_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rcu_state {
    struct rcu_node node[521];
    struct rcu_node * level[4];
    int ncpus;
    u8 boost;
    long unsigned int gp_seq;
    struct task_struct *gp_kthread;
    struct swait_queue_head gp_wq;
    short int gp_flags;
    short int gp_state;
    long unsigned int gp_wake_time;
    long unsigned int gp_wake_seq;
    struct mutex barrier_mutex;
    atomic_t barrier_cpu_count;
    struct completion barrier_completion;
    long unsigned int barrier_sequence;
    struct mutex exp_mutex;
    struct mutex exp_wake_mutex;
    long unsigned int expedited_sequence;
    atomic_t expedited_need_qs;
    struct swait_queue_head expedited_wq;
    int ncpus_snap;
    long unsigned int jiffies_force_qs;
    long unsigned int jiffies_kick_kthreads;
    long unsigned int n_force_qs;
    long unsigned int gp_start;
    long unsigned int gp_end;
    long unsigned int gp_activity;
    long unsigned int gp_req_activity;
    long unsigned int jiffies_stall;
    long unsigned int jiffies_resched;
    long unsigned int n_force_qs_gpstart;
    long unsigned int gp_max;
    const char *name;
    char abbr;
    raw_spinlock_t ofl_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct rcu_state {
    struct rcu_node node[521];
    struct rcu_node * level[4];
    int ncpus;
    u8 boost;
    long unsigned int gp_seq;
    struct task_struct *gp_kthread;
    struct swait_queue_head gp_wq;
    short int gp_flags;
    short int gp_state;
    long unsigned int gp_wake_time;
    long unsigned int gp_wake_seq;
    struct mutex barrier_mutex;
    atomic_t barrier_cpu_count;
    struct completion barrier_completion;
    long unsigned int barrier_sequence;
    struct mutex exp_mutex;
    struct mutex exp_wake_mutex;
    long unsigned int expedited_sequence;
    atomic_t expedited_need_qs;
    struct swait_queue_head expedited_wq;
    int ncpus_snap;
    u8 cbovld;
    u8 cbovldnext;
    long unsigned int jiffies_force_qs;
    long unsigned int jiffies_kick_kthreads;
    long unsigned int n_force_qs;
    long unsigned int gp_start;
    long unsigned int gp_end;
    long unsigned int gp_activity;
    long unsigned int gp_req_activity;
    long unsigned int jiffies_stall;
    long unsigned int jiffies_resched;
    long unsigned int n_force_qs_gpstart;
    long unsigned int gp_max;
    const char *name;
    char abbr;
    raw_spinlock_t ofl_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct rcu_state {
    struct rcu_node node[521];
    struct rcu_node * level[4];
    int ncpus;
    int n_online_cpus;
    u8 boost;
    long unsigned int gp_seq;
    long unsigned int gp_max;
    struct task_struct *gp_kthread;
    struct swait_queue_head gp_wq;
    short int gp_flags;
    short int gp_state;
    long unsigned int gp_wake_time;
    long unsigned int gp_wake_seq;
    struct mutex barrier_mutex;
    atomic_t barrier_cpu_count;
    struct completion barrier_completion;
    long unsigned int barrier_sequence;
    struct mutex exp_mutex;
    struct mutex exp_wake_mutex;
    long unsigned int expedited_sequence;
    atomic_t expedited_need_qs;
    struct swait_queue_head expedited_wq;
    int ncpus_snap;
    u8 cbovld;
    u8 cbovldnext;
    long unsigned int jiffies_force_qs;
    long unsigned int jiffies_kick_kthreads;
    long unsigned int n_force_qs;
    long unsigned int gp_start;
    long unsigned int gp_end;
    long unsigned int gp_activity;
    long unsigned int gp_req_activity;
    long unsigned int jiffies_stall;
    long unsigned int jiffies_resched;
    long unsigned int n_force_qs_gpstart;
    const char *name;
    char abbr;
    raw_spinlock_t ofl_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rcu_state {
    struct rcu_node node[521];
    struct rcu_node * level[4];
    int ncpus;
    int n_online_cpus;
    u8 boost;
    long unsigned int gp_seq;
    long unsigned int gp_max;
    struct task_struct *gp_kthread;
    struct swait_queue_head gp_wq;
    short int gp_flags;
    short int gp_state;
    long unsigned int gp_wake_time;
    long unsigned int gp_wake_seq;
    struct mutex barrier_mutex;
    atomic_t barrier_cpu_count;
    struct completion barrier_completion;
    long unsigned int barrier_sequence;
    struct mutex exp_mutex;
    struct mutex exp_wake_mutex;
    long unsigned int expedited_sequence;
    atomic_t expedited_need_qs;
    struct swait_queue_head expedited_wq;
    int ncpus_snap;
    u8 cbovld;
    u8 cbovldnext;
    long unsigned int jiffies_force_qs;
    long unsigned int jiffies_kick_kthreads;
    long unsigned int n_force_qs;
    long unsigned int gp_start;
    long unsigned int gp_end;
    long unsigned int gp_activity;
    long unsigned int gp_req_activity;
    long unsigned int jiffies_stall;
    long unsigned int jiffies_resched;
    long unsigned int n_force_qs_gpstart;
    const char *name;
    char abbr;
    raw_spinlock_t ofl_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rcu_state {
    struct rcu_node node[521];
    struct rcu_node * level[4];
    int ncpus;
    int n_online_cpus;
    u8 boost;
    long unsigned int gp_seq;
    long unsigned int gp_max;
    struct task_struct *gp_kthread;
    struct swait_queue_head gp_wq;
    short int gp_flags;
    short int gp_state;
    long unsigned int gp_wake_time;
    long unsigned int gp_wake_seq;
    struct mutex barrier_mutex;
    atomic_t barrier_cpu_count;
    struct completion barrier_completion;
    long unsigned int barrier_sequence;
    struct mutex exp_mutex;
    struct mutex exp_wake_mutex;
    long unsigned int expedited_sequence;
    atomic_t expedited_need_qs;
    struct swait_queue_head expedited_wq;
    int ncpus_snap;
    u8 cbovld;
    u8 cbovldnext;
    long unsigned int jiffies_force_qs;
    long unsigned int jiffies_kick_kthreads;
    long unsigned int n_force_qs;
    long unsigned int gp_start;
    long unsigned int gp_end;
    long unsigned int gp_activity;
    long unsigned int gp_req_activity;
    long unsigned int jiffies_stall;
    long unsigned int jiffies_resched;
    long unsigned int n_force_qs_gpstart;
    const char *name;
    char abbr;
    raw_spinlock_t ofl_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rcu_state {
    struct rcu_node node[521];
    struct rcu_node * level[4];
    int ncpus;
    int n_online_cpus;
    long unsigned int gp_seq;
    long unsigned int gp_max;
    struct task_struct *gp_kthread;
    struct swait_queue_head gp_wq;
    short int gp_flags;
    short int gp_state;
    long unsigned int gp_wake_time;
    long unsigned int gp_wake_seq;
    struct mutex barrier_mutex;
    atomic_t barrier_cpu_count;
    struct completion barrier_completion;
    long unsigned int barrier_sequence;
    raw_spinlock_t barrier_lock;
    struct mutex exp_mutex;
    struct mutex exp_wake_mutex;
    long unsigned int expedited_sequence;
    atomic_t expedited_need_qs;
    struct swait_queue_head expedited_wq;
    int ncpus_snap;
    u8 cbovld;
    u8 cbovldnext;
    long unsigned int jiffies_force_qs;
    long unsigned int jiffies_kick_kthreads;
    long unsigned int n_force_qs;
    long unsigned int gp_start;
    long unsigned int gp_end;
    long unsigned int gp_activity;
    long unsigned int gp_req_activity;
    long unsigned int jiffies_stall;
    long unsigned int jiffies_resched;
    long unsigned int n_force_qs_gpstart;
    const char *name;
    char abbr;
    arch_spinlock_t ofl_lock;
    int nocb_is_setup;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rcu_state {
    struct rcu_node node[521];
    struct rcu_node * level[4];
    int ncpus;
    int n_online_cpus;
    long unsigned int gp_seq;
    long unsigned int gp_max;
    struct task_struct *gp_kthread;
    struct swait_queue_head gp_wq;
    short int gp_flags;
    short int gp_state;
    long unsigned int gp_wake_time;
    long unsigned int gp_wake_seq;
    long unsigned int gp_seq_polled;
    long unsigned int gp_seq_polled_snap;
    long unsigned int gp_seq_polled_exp_snap;
    struct mutex barrier_mutex;
    atomic_t barrier_cpu_count;
    struct completion barrier_completion;
    long unsigned int barrier_sequence;
    raw_spinlock_t barrier_lock;
    struct mutex exp_mutex;
    struct mutex exp_wake_mutex;
    long unsigned int expedited_sequence;
    atomic_t expedited_need_qs;
    struct swait_queue_head expedited_wq;
    int ncpus_snap;
    u8 cbovld;
    u8 cbovldnext;
    long unsigned int jiffies_force_qs;
    long unsigned int jiffies_kick_kthreads;
    long unsigned int n_force_qs;
    long unsigned int gp_start;
    long unsigned int gp_end;
    long unsigned int gp_activity;
    long unsigned int gp_req_activity;
    long unsigned int jiffies_stall;
    long unsigned int jiffies_resched;
    long unsigned int n_force_qs_gpstart;
    const char *name;
    char abbr;
    arch_spinlock_t ofl_lock;
    int nocb_is_setup;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rcu_state {
    struct rcu_node node[521];
    struct rcu_node * level[4];
    int ncpus;
    int n_online_cpus;
    long unsigned int gp_seq;
    long unsigned int gp_max;
    struct task_struct *gp_kthread;
    struct swait_queue_head gp_wq;
    short int gp_flags;
    short int gp_state;
    long unsigned int gp_wake_time;
    long unsigned int gp_wake_seq;
    long unsigned int gp_seq_polled;
    long unsigned int gp_seq_polled_snap;
    long unsigned int gp_seq_polled_exp_snap;
    struct mutex barrier_mutex;
    atomic_t barrier_cpu_count;
    struct completion barrier_completion;
    long unsigned int barrier_sequence;
    raw_spinlock_t barrier_lock;
    struct mutex exp_mutex;
    struct mutex exp_wake_mutex;
    long unsigned int expedited_sequence;
    atomic_t expedited_need_qs;
    struct swait_queue_head expedited_wq;
    int ncpus_snap;
    u8 cbovld;
    u8 cbovldnext;
    long unsigned int jiffies_force_qs;
    long unsigned int jiffies_kick_kthreads;
    long unsigned int n_force_qs;
    long unsigned int gp_start;
    long unsigned int gp_end;
    long unsigned int gp_activity;
    long unsigned int gp_req_activity;
    long unsigned int jiffies_stall;
    long unsigned int jiffies_resched;
    long unsigned int n_force_qs_gpstart;
    const char *name;
    char abbr;
    arch_spinlock_t ofl_lock;
    int nocb_is_setup;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rcu_state {
    struct rcu_node node[521];
    struct rcu_node * level[4];
    int ncpus;
    int n_online_cpus;
    long unsigned int gp_seq;
    long unsigned int gp_max;
    struct task_struct *gp_kthread;
    struct swait_queue_head gp_wq;
    short int gp_flags;
    short int gp_state;
    long unsigned int gp_wake_time;
    long unsigned int gp_wake_seq;
    long unsigned int gp_seq_polled;
    long unsigned int gp_seq_polled_snap;
    long unsigned int gp_seq_polled_exp_snap;
    struct mutex barrier_mutex;
    atomic_t barrier_cpu_count;
    struct completion barrier_completion;
    long unsigned int barrier_sequence;
    raw_spinlock_t barrier_lock;
    struct mutex exp_mutex;
    struct mutex exp_wake_mutex;
    long unsigned int expedited_sequence;
    atomic_t expedited_need_qs;
    struct swait_queue_head expedited_wq;
    int ncpus_snap;
    u8 cbovld;
    u8 cbovldnext;
    long unsigned int jiffies_force_qs;
    long unsigned int jiffies_kick_kthreads;
    long unsigned int n_force_qs;
    long unsigned int gp_start;
    long unsigned int gp_end;
    long unsigned int gp_activity;
    long unsigned int gp_req_activity;
    long unsigned int jiffies_stall;
    int nr_fqs_jiffies_stall;
    long unsigned int jiffies_resched;
    long unsigned int n_force_qs_gpstart;
    const char *name;
    char abbr;
    arch_spinlock_t ofl_lock;
    int nocb_is_setup;
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
struct rcu_state {
    struct rcu_node node[17];
    struct rcu_node * level[3];
    int ncpus;
    u8 boost;
    long unsigned int gp_seq;
    struct task_struct *gp_kthread;
    struct swait_queue_head gp_wq;
    short int gp_flags;
    short int gp_state;
    long unsigned int gp_wake_time;
    long unsigned int gp_wake_seq;
    struct mutex barrier_mutex;
    atomic_t barrier_cpu_count;
    struct completion barrier_completion;
    long unsigned int barrier_sequence;
    struct mutex exp_mutex;
    struct mutex exp_wake_mutex;
    long unsigned int expedited_sequence;
    atomic_t expedited_need_qs;
    struct swait_queue_head expedited_wq;
    int ncpus_snap;
    long unsigned int jiffies_force_qs;
    long unsigned int jiffies_kick_kthreads;
    long unsigned int n_force_qs;
    long unsigned int gp_start;
    long unsigned int gp_end;
    long unsigned int gp_activity;
    long unsigned int gp_req_activity;
    long unsigned int jiffies_stall;
    long unsigned int jiffies_resched;
    long unsigned int n_force_qs_gpstart;
    long unsigned int gp_max;
    const char *name;
    char abbr;
    raw_spinlock_t ofl_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rcu_state {
    struct rcu_node node[1];
    struct rcu_node * level[2];
    int ncpus;
    u8 boost;
    long unsigned int gp_seq;
    struct task_struct *gp_kthread;
    struct swait_queue_head gp_wq;
    short int gp_flags;
    short int gp_state;
    long unsigned int gp_wake_time;
    long unsigned int gp_wake_seq;
    struct mutex barrier_mutex;
    atomic_t barrier_cpu_count;
    struct completion barrier_completion;
    long unsigned int barrier_sequence;
    struct mutex exp_mutex;
    struct mutex exp_wake_mutex;
    long unsigned int expedited_sequence;
    atomic_t expedited_need_qs;
    struct swait_queue_head expedited_wq;
    int ncpus_snap;
    long unsigned int jiffies_force_qs;
    long unsigned int jiffies_kick_kthreads;
    long unsigned int n_force_qs;
    long unsigned int gp_start;
    long unsigned int gp_end;
    long unsigned int gp_activity;
    long unsigned int gp_req_activity;
    long unsigned int jiffies_stall;
    long unsigned int jiffies_resched;
    long unsigned int n_force_qs_gpstart;
    long unsigned int gp_max;
    const char *name;
    char abbr;
    raw_spinlock_t ofl_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rcu_state {
    struct rcu_node node[131];
    struct rcu_node * level[4];
    int ncpus;
    u8 boost;
    long unsigned int gp_seq;
    struct task_struct *gp_kthread;
    struct swait_queue_head gp_wq;
    short int gp_flags;
    short int gp_state;
    long unsigned int gp_wake_time;
    long unsigned int gp_wake_seq;
    struct mutex barrier_mutex;
    atomic_t barrier_cpu_count;
    struct completion barrier_completion;
    long unsigned int barrier_sequence;
    struct mutex exp_mutex;
    struct mutex exp_wake_mutex;
    long unsigned int expedited_sequence;
    atomic_t expedited_need_qs;
    struct swait_queue_head expedited_wq;
    int ncpus_snap;
    long unsigned int jiffies_force_qs;
    long unsigned int jiffies_kick_kthreads;
    long unsigned int n_force_qs;
    long unsigned int gp_start;
    long unsigned int gp_end;
    long unsigned int gp_activity;
    long unsigned int gp_req_activity;
    long unsigned int jiffies_stall;
    long unsigned int jiffies_resched;
    long unsigned int n_force_qs_gpstart;
    long unsigned int gp_max;
    const char *name;
    char abbr;
    raw_spinlock_t ofl_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct rcu_state {
    struct rcu_node node[1];
    struct rcu_node * level[2];
    int ncpus;
    u8 boost;
    long unsigned int gp_seq;
    struct task_struct *gp_kthread;
    struct swait_queue_head gp_wq;
    short int gp_flags;
    short int gp_state;
    long unsigned int gp_wake_time;
    long unsigned int gp_wake_seq;
    struct mutex barrier_mutex;
    atomic_t barrier_cpu_count;
    struct completion barrier_completion;
    long unsigned int barrier_sequence;
    struct mutex exp_mutex;
    struct mutex exp_wake_mutex;
    long unsigned int expedited_sequence;
    atomic_t expedited_need_qs;
    struct swait_queue_head expedited_wq;
    int ncpus_snap;
    long unsigned int jiffies_force_qs;
    long unsigned int jiffies_kick_kthreads;
    long unsigned int n_force_qs;
    long unsigned int gp_start;
    long unsigned int gp_end;
    long unsigned int gp_activity;
    long unsigned int gp_req_activity;
    long unsigned int jiffies_stall;
    long unsigned int jiffies_resched;
    long unsigned int n_force_qs_gpstart;
    long unsigned int gp_max;
    const char *name;
    char abbr;
    raw_spinlock_t ofl_lock;
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
struct rcu_state {
    struct rcu_node node[521];
    struct rcu_node * level[4];
    int ncpus;
    u8 boost;
    long unsigned int gp_seq;
    struct task_struct *gp_kthread;
    struct swait_queue_head gp_wq;
    short int gp_flags;
    short int gp_state;
    long unsigned int gp_wake_time;
    long unsigned int gp_wake_seq;
    struct mutex barrier_mutex;
    atomic_t barrier_cpu_count;
    struct completion barrier_completion;
    long unsigned int barrier_sequence;
    struct mutex exp_mutex;
    struct mutex exp_wake_mutex;
    long unsigned int expedited_sequence;
    atomic_t expedited_need_qs;
    struct swait_queue_head expedited_wq;
    int ncpus_snap;
    long unsigned int jiffies_force_qs;
    long unsigned int jiffies_kick_kthreads;
    long unsigned int n_force_qs;
    long unsigned int gp_start;
    long unsigned int gp_end;
    long unsigned int gp_activity;
    long unsigned int gp_req_activity;
    long unsigned int jiffies_stall;
    long unsigned int jiffies_resched;
    long unsigned int n_force_qs_gpstart;
    long unsigned int gp_max;
    const char *name;
    char abbr;
    raw_spinlock_t ofl_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rcu_state {
    struct rcu_node node[521];
    struct rcu_node * level[4];
    int ncpus;
    u8 boost;
    long unsigned int gp_seq;
    struct task_struct *gp_kthread;
    struct swait_queue_head gp_wq;
    short int gp_flags;
    short int gp_state;
    long unsigned int gp_wake_time;
    long unsigned int gp_wake_seq;
    struct mutex barrier_mutex;
    atomic_t barrier_cpu_count;
    struct completion barrier_completion;
    long unsigned int barrier_sequence;
    struct mutex exp_mutex;
    struct mutex exp_wake_mutex;
    long unsigned int expedited_sequence;
    atomic_t expedited_need_qs;
    struct swait_queue_head expedited_wq;
    int ncpus_snap;
    long unsigned int jiffies_force_qs;
    long unsigned int jiffies_kick_kthreads;
    long unsigned int n_force_qs;
    long unsigned int gp_start;
    long unsigned int gp_end;
    long unsigned int gp_activity;
    long unsigned int gp_req_activity;
    long unsigned int jiffies_stall;
    long unsigned int jiffies_resched;
    long unsigned int n_force_qs_gpstart;
    long unsigned int gp_max;
    const char *name;
    char abbr;
    raw_spinlock_t ofl_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rcu_state {
    struct rcu_node node[521];
    struct rcu_node * level[4];
    int ncpus;
    u8 boost;
    long unsigned int gp_seq;
    struct task_struct *gp_kthread;
    struct swait_queue_head gp_wq;
    short int gp_flags;
    short int gp_state;
    long unsigned int gp_wake_time;
    long unsigned int gp_wake_seq;
    struct mutex barrier_mutex;
    atomic_t barrier_cpu_count;
    struct completion barrier_completion;
    long unsigned int barrier_sequence;
    struct mutex exp_mutex;
    struct mutex exp_wake_mutex;
    long unsigned int expedited_sequence;
    atomic_t expedited_need_qs;
    struct swait_queue_head expedited_wq;
    int ncpus_snap;
    long unsigned int jiffies_force_qs;
    long unsigned int jiffies_kick_kthreads;
    long unsigned int n_force_qs;
    long unsigned int gp_start;
    long unsigned int gp_end;
    long unsigned int gp_activity;
    long unsigned int gp_req_activity;
    long unsigned int jiffies_stall;
    long unsigned int jiffies_resched;
    long unsigned int n_force_qs_gpstart;
    long unsigned int gp_max;
    const char *name;
    char abbr;
    raw_spinlock_t ofl_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rcu_state {
    struct rcu_node node[521];
    struct rcu_node * level[4];
    int ncpus;
    u8 boost;
    long unsigned int gp_seq;
    struct task_struct *gp_kthread;
    struct swait_queue_head gp_wq;
    short int gp_flags;
    short int gp_state;
    long unsigned int gp_wake_time;
    long unsigned int gp_wake_seq;
    struct mutex barrier_mutex;
    atomic_t barrier_cpu_count;
    struct completion barrier_completion;
    long unsigned int barrier_sequence;
    struct mutex exp_mutex;
    struct mutex exp_wake_mutex;
    long unsigned int expedited_sequence;
    atomic_t expedited_need_qs;
    struct swait_queue_head expedited_wq;
    int ncpus_snap;
    long unsigned int jiffies_force_qs;
    long unsigned int jiffies_kick_kthreads;
    long unsigned int n_force_qs;
    long unsigned int gp_start;
    long unsigned int gp_end;
    long unsigned int gp_activity;
    long unsigned int gp_req_activity;
    long unsigned int jiffies_stall;
    long unsigned int jiffies_resched;
    long unsigned int n_force_qs_gpstart;
    long unsigned int gp_max;
    const char *name;
    char abbr;
    raw_spinlock_t ofl_lock;
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
<code>struct mutex exp_mutex</code>
</li>
<li>
<b>Field added. </b>
<code>struct mutex exp_wake_mutex</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int jiffies_kick_kthreads</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_long_t expedited_workdone0</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_long_t expedited_workdone1</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_long_t expedited_workdone2</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_long_t expedited_workdone3</code>
</li>
<li>
<b>Field type changed. </b>
<code>wait_queue_head_t gp_wq</code> ➡️ <code>struct swait_queue_head gp_wq</code>
</li>
<li>
<b>Field type changed. </b>
<code>wait_queue_head_t expedited_wq</code> ➡️ <code>struct swait_queue_head expedited_wq</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct rcu_node node[5]</code> ➡️ <code>struct rcu_node node[131]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct rcu_node * level[3]</code> ➡️ <code>struct rcu_node * level[4]</code>
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
<code>struct rcu_cblist orphan_pend</code>
</li>
<li>
<b>Field added. </b>
<code>struct rcu_cblist orphan_done</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 flavor_mask</code>
</li>
<li>
<b>Field removed. </b>
<code>struct callback_head *orphan_nxtlist</code>
</li>
<li>
<b>Field removed. </b>
<code>struct callback_head **orphan_nxttail</code>
</li>
<li>
<b>Field removed. </b>
<code>struct callback_head *orphan_donelist</code>
</li>
<li>
<b>Field removed. </b>
<code>struct callback_head **orphan_donetail</code>
</li>
<li>
<b>Field removed. </b>
<code>long int qlen_lazy</code>
</li>
<li>
<b>Field removed. </b>
<code>long int qlen</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_long_t expedited_normal</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct rcu_node node[131]</code> ➡️ <code>struct rcu_node node[521]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>raw_spinlock_t orphan_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rcu_cblist orphan_pend</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rcu_cblist orphan_done</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>long unsigned int n_force_qs_lh</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int n_force_qs_ngp</code>
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
<code>long unsigned int gp_seq</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int gp_end</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int gp_req_activity</code>
</li>
<li>
<b>Field added. </b>
<code>raw_spinlock_t ofl_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rcu_data *rda</code>
</li>
<li>
<b>Field removed. </b>
<code>call_rcu_func_t call</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int gpnum</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int completed</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head flavors</code>
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
<code>long unsigned int gp_wake_time</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int gp_wake_seq</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 cbovld</code>
</li>
<li>
<b>Field added. </b>
<code>u8 cbovldnext</code>
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
<code>int n_online_cpus</code>
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
<code>raw_spinlock_t barrier_lock</code>
</li>
<li>
<b>Field added. </b>
<code>int nocb_is_setup</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 boost</code>
</li>
<li>
<b>Field type changed. </b>
<code>raw_spinlock_t ofl_lock</code> ➡️ <code>arch_spinlock_t ofl_lock</code>
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
<code>long unsigned int gp_seq_polled</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int gp_seq_polled_snap</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int gp_seq_polled_exp_snap</code>
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
<code>int nr_fqs_jiffies_stall</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>arm64</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct rcu_node node[521]</code> ➡️ <code>struct rcu_node node[17]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct rcu_node * level[4]</code> ➡️ <code>struct rcu_node * level[3]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct rcu_node node[521]</code> ➡️ <code>struct rcu_node node[1]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct rcu_node * level[4]</code> ➡️ <code>struct rcu_node * level[2]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct rcu_node node[521]</code> ➡️ <code>struct rcu_node node[131]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct rcu_node node[521]</code> ➡️ <code>struct rcu_node node[1]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct rcu_node * level[4]</code> ➡️ <code>struct rcu_node * level[2]</code>
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
