# Struct: <code>rcu_node</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct rcu_node {
    raw_spinlock_t lock;
    long unsigned int gpnum;
    long unsigned int completed;
    long unsigned int qsmask;
    long unsigned int qsmaskinit;
    long unsigned int qsmaskinitnext;
    long unsigned int expmask;
    long unsigned int expmaskinit;
    long unsigned int expmaskinitnext;
    long unsigned int grpmask;
    int grplo;
    int grphi;
    u8 grpnum;
    u8 level;
    bool wait_blkd_tasks;
    struct rcu_node *parent;
    struct list_head blkd_tasks;
    struct list_head *gp_tasks;
    struct list_head *exp_tasks;
    struct list_head *boost_tasks;
    struct rt_mutex boost_mtx;
    long unsigned int boost_time;
    struct task_struct *boost_kthread_task;
    unsigned int boost_kthread_status;
    long unsigned int n_tasks_boosted;
    long unsigned int n_exp_boosts;
    long unsigned int n_normal_boosts;
    long unsigned int n_balk_blkd_tasks;
    long unsigned int n_balk_exp_gp_tasks;
    long unsigned int n_balk_boost_tasks;
    long unsigned int n_balk_notblocked;
    long unsigned int n_balk_notyet;
    long unsigned int n_balk_nos;
    int need_future_gp[2];
    raw_spinlock_t fqslock;
    struct mutex exp_funnel_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct rcu_node {
    raw_spinlock_t lock;
    long unsigned int gpnum;
    long unsigned int completed;
    long unsigned int qsmask;
    long unsigned int qsmaskinit;
    long unsigned int qsmaskinitnext;
    long unsigned int expmask;
    long unsigned int expmaskinit;
    long unsigned int expmaskinitnext;
    long unsigned int grpmask;
    int grplo;
    int grphi;
    u8 grpnum;
    u8 level;
    bool wait_blkd_tasks;
    struct rcu_node *parent;
    struct list_head blkd_tasks;
    struct list_head *gp_tasks;
    struct list_head *exp_tasks;
    struct list_head *boost_tasks;
    struct rt_mutex boost_mtx;
    long unsigned int boost_time;
    struct task_struct *boost_kthread_task;
    unsigned int boost_kthread_status;
    long unsigned int n_tasks_boosted;
    long unsigned int n_exp_boosts;
    long unsigned int n_normal_boosts;
    long unsigned int n_balk_blkd_tasks;
    long unsigned int n_balk_exp_gp_tasks;
    long unsigned int n_balk_boost_tasks;
    long unsigned int n_balk_notblocked;
    long unsigned int n_balk_notyet;
    long unsigned int n_balk_nos;
    int need_future_gp[2];
    raw_spinlock_t fqslock;
    spinlock_t exp_lock;
    long unsigned int exp_seq_rq;
    wait_queue_head_t exp_wq[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rcu_node {
    raw_spinlock_t lock;
    long unsigned int gpnum;
    long unsigned int completed;
    long unsigned int qsmask;
    long unsigned int qsmaskinit;
    long unsigned int qsmaskinitnext;
    long unsigned int expmask;
    long unsigned int expmaskinit;
    long unsigned int expmaskinitnext;
    long unsigned int grpmask;
    int grplo;
    int grphi;
    u8 grpnum;
    u8 level;
    bool wait_blkd_tasks;
    struct rcu_node *parent;
    struct list_head blkd_tasks;
    struct list_head *gp_tasks;
    struct list_head *exp_tasks;
    struct list_head *boost_tasks;
    struct rt_mutex boost_mtx;
    long unsigned int boost_time;
    struct task_struct *boost_kthread_task;
    unsigned int boost_kthread_status;
    long unsigned int n_tasks_boosted;
    long unsigned int n_exp_boosts;
    long unsigned int n_normal_boosts;
    long unsigned int n_balk_blkd_tasks;
    long unsigned int n_balk_exp_gp_tasks;
    long unsigned int n_balk_boost_tasks;
    long unsigned int n_balk_notblocked;
    long unsigned int n_balk_notyet;
    long unsigned int n_balk_nos;
    int need_future_gp[2];
    raw_spinlock_t fqslock;
    spinlock_t exp_lock;
    long unsigned int exp_seq_rq;
    wait_queue_head_t exp_wq[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rcu_node {
    raw_spinlock_t lock;
    long unsigned int gpnum;
    long unsigned int completed;
    long unsigned int qsmask;
    long unsigned int qsmaskinit;
    long unsigned int qsmaskinitnext;
    long unsigned int expmask;
    long unsigned int expmaskinit;
    long unsigned int expmaskinitnext;
    long unsigned int grpmask;
    int grplo;
    int grphi;
    u8 grpnum;
    u8 level;
    bool wait_blkd_tasks;
    struct rcu_node *parent;
    struct list_head blkd_tasks;
    struct list_head *gp_tasks;
    struct list_head *exp_tasks;
    struct list_head *boost_tasks;
    struct rt_mutex boost_mtx;
    long unsigned int boost_time;
    struct task_struct *boost_kthread_task;
    unsigned int boost_kthread_status;
    long unsigned int n_tasks_boosted;
    long unsigned int n_exp_boosts;
    long unsigned int n_normal_boosts;
    int need_future_gp[2];
    raw_spinlock_t fqslock;
    spinlock_t exp_lock;
    long unsigned int exp_seq_rq;
    wait_queue_head_t exp_wq[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rcu_node {
    raw_spinlock_t lock;
    long unsigned int gpnum;
    long unsigned int completed;
    long unsigned int qsmask;
    long unsigned int qsmaskinit;
    long unsigned int qsmaskinitnext;
    long unsigned int expmask;
    long unsigned int expmaskinit;
    long unsigned int expmaskinitnext;
    long unsigned int ffmask;
    long unsigned int grpmask;
    int grplo;
    int grphi;
    u8 grpnum;
    u8 level;
    bool wait_blkd_tasks;
    struct rcu_node *parent;
    struct list_head blkd_tasks;
    struct list_head *gp_tasks;
    struct list_head *exp_tasks;
    struct list_head *boost_tasks;
    struct rt_mutex boost_mtx;
    long unsigned int boost_time;
    struct task_struct *boost_kthread_task;
    unsigned int boost_kthread_status;
    long unsigned int n_tasks_boosted;
    long unsigned int n_exp_boosts;
    long unsigned int n_normal_boosts;
    int need_future_gp[2];
    raw_spinlock_t fqslock;
    spinlock_t exp_lock;
    long unsigned int exp_seq_rq;
    wait_queue_head_t exp_wq[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rcu_node {
    raw_spinlock_t lock;
    long unsigned int gpnum;
    long unsigned int completed;
    long unsigned int qsmask;
    long unsigned int qsmaskinit;
    long unsigned int qsmaskinitnext;
    long unsigned int expmask;
    long unsigned int expmaskinit;
    long unsigned int expmaskinitnext;
    long unsigned int ffmask;
    long unsigned int grpmask;
    int grplo;
    int grphi;
    u8 grpnum;
    u8 level;
    bool wait_blkd_tasks;
    struct rcu_node *parent;
    struct list_head blkd_tasks;
    struct list_head *gp_tasks;
    struct list_head *exp_tasks;
    struct list_head *boost_tasks;
    struct rt_mutex boost_mtx;
    long unsigned int boost_time;
    struct task_struct *boost_kthread_task;
    unsigned int boost_kthread_status;
    u8 need_future_gp[4];
    raw_spinlock_t fqslock;
    spinlock_t exp_lock;
    long unsigned int exp_seq_rq;
    wait_queue_head_t exp_wq[4];
    struct rcu_exp_work rew;
    bool exp_need_flush;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rcu_node {
    raw_spinlock_t lock;
    long unsigned int gp_seq;
    long unsigned int gp_seq_needed;
    long unsigned int completedqs;
    long unsigned int qsmask;
    long unsigned int rcu_gp_init_mask;
    long unsigned int qsmaskinit;
    long unsigned int qsmaskinitnext;
    long unsigned int expmask;
    long unsigned int expmaskinit;
    long unsigned int expmaskinitnext;
    long unsigned int ffmask;
    long unsigned int grpmask;
    int grplo;
    int grphi;
    u8 grpnum;
    u8 level;
    bool wait_blkd_tasks;
    struct rcu_node *parent;
    struct list_head blkd_tasks;
    struct list_head *gp_tasks;
    struct list_head *exp_tasks;
    struct list_head *boost_tasks;
    struct rt_mutex boost_mtx;
    long unsigned int boost_time;
    struct task_struct *boost_kthread_task;
    unsigned int boost_kthread_status;
    raw_spinlock_t fqslock;
    spinlock_t exp_lock;
    long unsigned int exp_seq_rq;
    wait_queue_head_t exp_wq[4];
    struct rcu_exp_work rew;
    bool exp_need_flush;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rcu_node {
    raw_spinlock_t lock;
    long unsigned int gp_seq;
    long unsigned int gp_seq_needed;
    long unsigned int completedqs;
    long unsigned int qsmask;
    long unsigned int rcu_gp_init_mask;
    long unsigned int qsmaskinit;
    long unsigned int qsmaskinitnext;
    long unsigned int expmask;
    long unsigned int expmaskinit;
    long unsigned int expmaskinitnext;
    long unsigned int ffmask;
    long unsigned int grpmask;
    int grplo;
    int grphi;
    u8 grpnum;
    u8 level;
    bool wait_blkd_tasks;
    struct rcu_node *parent;
    struct list_head blkd_tasks;
    struct list_head *gp_tasks;
    struct list_head *exp_tasks;
    struct list_head *boost_tasks;
    struct rt_mutex boost_mtx;
    long unsigned int boost_time;
    struct task_struct *boost_kthread_task;
    unsigned int boost_kthread_status;
    raw_spinlock_t fqslock;
    spinlock_t exp_lock;
    long unsigned int exp_seq_rq;
    wait_queue_head_t exp_wq[4];
    struct rcu_exp_work rew;
    bool exp_need_flush;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rcu_node {
    raw_spinlock_t lock;
    long unsigned int gp_seq;
    long unsigned int gp_seq_needed;
    long unsigned int completedqs;
    long unsigned int qsmask;
    long unsigned int rcu_gp_init_mask;
    long unsigned int qsmaskinit;
    long unsigned int qsmaskinitnext;
    long unsigned int expmask;
    long unsigned int expmaskinit;
    long unsigned int expmaskinitnext;
    long unsigned int ffmask;
    long unsigned int grpmask;
    int grplo;
    int grphi;
    u8 grpnum;
    u8 level;
    bool wait_blkd_tasks;
    struct rcu_node *parent;
    struct list_head blkd_tasks;
    struct list_head *gp_tasks;
    struct list_head *exp_tasks;
    struct list_head *boost_tasks;
    struct rt_mutex boost_mtx;
    long unsigned int boost_time;
    struct task_struct *boost_kthread_task;
    unsigned int boost_kthread_status;
    raw_spinlock_t fqslock;
    spinlock_t exp_lock;
    long unsigned int exp_seq_rq;
    wait_queue_head_t exp_wq[4];
    struct rcu_exp_work rew;
    bool exp_need_flush;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct rcu_node {
    raw_spinlock_t lock;
    long unsigned int gp_seq;
    long unsigned int gp_seq_needed;
    long unsigned int completedqs;
    long unsigned int qsmask;
    long unsigned int rcu_gp_init_mask;
    long unsigned int qsmaskinit;
    long unsigned int qsmaskinitnext;
    long unsigned int expmask;
    long unsigned int expmaskinit;
    long unsigned int expmaskinitnext;
    long unsigned int cbovldmask;
    long unsigned int ffmask;
    long unsigned int grpmask;
    int grplo;
    int grphi;
    u8 grpnum;
    u8 level;
    bool wait_blkd_tasks;
    struct rcu_node *parent;
    struct list_head blkd_tasks;
    struct list_head *gp_tasks;
    struct list_head *exp_tasks;
    struct list_head *boost_tasks;
    struct rt_mutex boost_mtx;
    long unsigned int boost_time;
    struct task_struct *boost_kthread_task;
    unsigned int boost_kthread_status;
    raw_spinlock_t fqslock;
    spinlock_t exp_lock;
    long unsigned int exp_seq_rq;
    wait_queue_head_t exp_wq[4];
    struct rcu_exp_work rew;
    bool exp_need_flush;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct rcu_node {
    raw_spinlock_t lock;
    long unsigned int gp_seq;
    long unsigned int gp_seq_needed;
    long unsigned int completedqs;
    long unsigned int qsmask;
    long unsigned int rcu_gp_init_mask;
    long unsigned int qsmaskinit;
    long unsigned int qsmaskinitnext;
    long unsigned int ofl_seq;
    long unsigned int expmask;
    long unsigned int expmaskinit;
    long unsigned int expmaskinitnext;
    long unsigned int cbovldmask;
    long unsigned int ffmask;
    long unsigned int grpmask;
    int grplo;
    int grphi;
    u8 grpnum;
    u8 level;
    bool wait_blkd_tasks;
    struct rcu_node *parent;
    struct list_head blkd_tasks;
    struct list_head *gp_tasks;
    struct list_head *exp_tasks;
    struct list_head *boost_tasks;
    struct rt_mutex boost_mtx;
    long unsigned int boost_time;
    struct task_struct *boost_kthread_task;
    unsigned int boost_kthread_status;
    raw_spinlock_t fqslock;
    spinlock_t exp_lock;
    long unsigned int exp_seq_rq;
    wait_queue_head_t exp_wq[4];
    struct rcu_exp_work rew;
    bool exp_need_flush;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rcu_node {
    raw_spinlock_t lock;
    long unsigned int gp_seq;
    long unsigned int gp_seq_needed;
    long unsigned int completedqs;
    long unsigned int qsmask;
    long unsigned int rcu_gp_init_mask;
    long unsigned int qsmaskinit;
    long unsigned int qsmaskinitnext;
    long unsigned int ofl_seq;
    long unsigned int expmask;
    long unsigned int expmaskinit;
    long unsigned int expmaskinitnext;
    long unsigned int cbovldmask;
    long unsigned int ffmask;
    long unsigned int grpmask;
    int grplo;
    int grphi;
    u8 grpnum;
    u8 level;
    bool wait_blkd_tasks;
    struct rcu_node *parent;
    struct list_head blkd_tasks;
    struct list_head *gp_tasks;
    struct list_head *exp_tasks;
    struct list_head *boost_tasks;
    struct rt_mutex boost_mtx;
    long unsigned int boost_time;
    struct task_struct *boost_kthread_task;
    unsigned int boost_kthread_status;
    raw_spinlock_t fqslock;
    spinlock_t exp_lock;
    long unsigned int exp_seq_rq;
    wait_queue_head_t exp_wq[4];
    struct rcu_exp_work rew;
    bool exp_need_flush;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rcu_node {
    raw_spinlock_t lock;
    long unsigned int gp_seq;
    long unsigned int gp_seq_needed;
    long unsigned int completedqs;
    long unsigned int qsmask;
    long unsigned int rcu_gp_init_mask;
    long unsigned int qsmaskinit;
    long unsigned int qsmaskinitnext;
    long unsigned int ofl_seq;
    long unsigned int expmask;
    long unsigned int expmaskinit;
    long unsigned int expmaskinitnext;
    long unsigned int cbovldmask;
    long unsigned int ffmask;
    long unsigned int grpmask;
    int grplo;
    int grphi;
    u8 grpnum;
    u8 level;
    bool wait_blkd_tasks;
    struct rcu_node *parent;
    struct list_head blkd_tasks;
    struct list_head *gp_tasks;
    struct list_head *exp_tasks;
    struct list_head *boost_tasks;
    struct rt_mutex boost_mtx;
    long unsigned int boost_time;
    struct task_struct *boost_kthread_task;
    unsigned int boost_kthread_status;
    long unsigned int n_boosts;
    raw_spinlock_t fqslock;
    spinlock_t exp_lock;
    long unsigned int exp_seq_rq;
    wait_queue_head_t exp_wq[4];
    struct rcu_exp_work rew;
    bool exp_need_flush;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rcu_node {
    raw_spinlock_t lock;
    long unsigned int gp_seq;
    long unsigned int gp_seq_needed;
    long unsigned int completedqs;
    long unsigned int qsmask;
    long unsigned int rcu_gp_init_mask;
    long unsigned int qsmaskinit;
    long unsigned int qsmaskinitnext;
    long unsigned int expmask;
    long unsigned int expmaskinit;
    long unsigned int expmaskinitnext;
    long unsigned int cbovldmask;
    long unsigned int ffmask;
    long unsigned int grpmask;
    int grplo;
    int grphi;
    u8 grpnum;
    u8 level;
    bool wait_blkd_tasks;
    struct rcu_node *parent;
    struct list_head blkd_tasks;
    struct list_head *gp_tasks;
    struct list_head *exp_tasks;
    struct list_head *boost_tasks;
    struct rt_mutex boost_mtx;
    long unsigned int boost_time;
    struct mutex boost_kthread_mutex;
    struct task_struct *boost_kthread_task;
    unsigned int boost_kthread_status;
    long unsigned int n_boosts;
    raw_spinlock_t fqslock;
    spinlock_t exp_lock;
    long unsigned int exp_seq_rq;
    wait_queue_head_t exp_wq[4];
    struct rcu_exp_work rew;
    bool exp_need_flush;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rcu_node {
    raw_spinlock_t lock;
    long unsigned int gp_seq;
    long unsigned int gp_seq_needed;
    long unsigned int completedqs;
    long unsigned int qsmask;
    long unsigned int rcu_gp_init_mask;
    long unsigned int qsmaskinit;
    long unsigned int qsmaskinitnext;
    long unsigned int expmask;
    long unsigned int expmaskinit;
    long unsigned int expmaskinitnext;
    long unsigned int cbovldmask;
    long unsigned int ffmask;
    long unsigned int grpmask;
    int grplo;
    int grphi;
    u8 grpnum;
    u8 level;
    bool wait_blkd_tasks;
    struct rcu_node *parent;
    struct list_head blkd_tasks;
    struct list_head *gp_tasks;
    struct list_head *exp_tasks;
    struct list_head *boost_tasks;
    struct rt_mutex boost_mtx;
    long unsigned int boost_time;
    struct mutex boost_kthread_mutex;
    struct task_struct *boost_kthread_task;
    unsigned int boost_kthread_status;
    long unsigned int n_boosts;
    raw_spinlock_t fqslock;
    spinlock_t exp_lock;
    long unsigned int exp_seq_rq;
    wait_queue_head_t exp_wq[4];
    struct rcu_exp_work rew;
    bool exp_need_flush;
    raw_spinlock_t exp_poll_lock;
    long unsigned int exp_seq_poll_rq;
    struct work_struct exp_poll_wq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rcu_node {
    raw_spinlock_t lock;
    long unsigned int gp_seq;
    long unsigned int gp_seq_needed;
    long unsigned int completedqs;
    long unsigned int qsmask;
    long unsigned int rcu_gp_init_mask;
    long unsigned int qsmaskinit;
    long unsigned int qsmaskinitnext;
    long unsigned int expmask;
    long unsigned int expmaskinit;
    long unsigned int expmaskinitnext;
    long unsigned int cbovldmask;
    long unsigned int ffmask;
    long unsigned int grpmask;
    int grplo;
    int grphi;
    u8 grpnum;
    u8 level;
    bool wait_blkd_tasks;
    struct rcu_node *parent;
    struct list_head blkd_tasks;
    struct list_head *gp_tasks;
    struct list_head *exp_tasks;
    struct list_head *boost_tasks;
    struct rt_mutex boost_mtx;
    long unsigned int boost_time;
    struct mutex boost_kthread_mutex;
    struct task_struct *boost_kthread_task;
    unsigned int boost_kthread_status;
    long unsigned int n_boosts;
    raw_spinlock_t fqslock;
    spinlock_t exp_lock;
    long unsigned int exp_seq_rq;
    wait_queue_head_t exp_wq[4];
    struct rcu_exp_work rew;
    bool exp_need_flush;
    raw_spinlock_t exp_poll_lock;
    long unsigned int exp_seq_poll_rq;
    struct work_struct exp_poll_wq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rcu_node {
    raw_spinlock_t lock;
    long unsigned int gp_seq;
    long unsigned int gp_seq_needed;
    long unsigned int completedqs;
    long unsigned int qsmask;
    long unsigned int rcu_gp_init_mask;
    long unsigned int qsmaskinit;
    long unsigned int qsmaskinitnext;
    long unsigned int expmask;
    long unsigned int expmaskinit;
    long unsigned int expmaskinitnext;
    long unsigned int cbovldmask;
    long unsigned int ffmask;
    long unsigned int grpmask;
    int grplo;
    int grphi;
    u8 grpnum;
    u8 level;
    bool wait_blkd_tasks;
    struct rcu_node *parent;
    struct list_head blkd_tasks;
    struct list_head *gp_tasks;
    struct list_head *exp_tasks;
    struct list_head *boost_tasks;
    struct rt_mutex boost_mtx;
    long unsigned int boost_time;
    struct mutex boost_kthread_mutex;
    struct task_struct *boost_kthread_task;
    unsigned int boost_kthread_status;
    long unsigned int n_boosts;
    struct swait_queue_head nocb_gp_wq[2];
    raw_spinlock_t fqslock;
    spinlock_t exp_lock;
    long unsigned int exp_seq_rq;
    wait_queue_head_t exp_wq[4];
    struct rcu_exp_work rew;
    bool exp_need_flush;
    raw_spinlock_t exp_poll_lock;
    long unsigned int exp_seq_poll_rq;
    struct work_struct exp_poll_wq;
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
struct rcu_node {
    raw_spinlock_t lock;
    long unsigned int gp_seq;
    long unsigned int gp_seq_needed;
    long unsigned int completedqs;
    long unsigned int qsmask;
    long unsigned int rcu_gp_init_mask;
    long unsigned int qsmaskinit;
    long unsigned int qsmaskinitnext;
    long unsigned int expmask;
    long unsigned int expmaskinit;
    long unsigned int expmaskinitnext;
    long unsigned int ffmask;
    long unsigned int grpmask;
    int grplo;
    int grphi;
    u8 grpnum;
    u8 level;
    bool wait_blkd_tasks;
    struct rcu_node *parent;
    struct list_head blkd_tasks;
    struct list_head *gp_tasks;
    struct list_head *exp_tasks;
    struct list_head *boost_tasks;
    struct rt_mutex boost_mtx;
    long unsigned int boost_time;
    struct task_struct *boost_kthread_task;
    unsigned int boost_kthread_status;
    raw_spinlock_t fqslock;
    spinlock_t exp_lock;
    long unsigned int exp_seq_rq;
    wait_queue_head_t exp_wq[4];
    struct rcu_exp_work rew;
    bool exp_need_flush;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rcu_node {
    raw_spinlock_t lock;
    long unsigned int gp_seq;
    long unsigned int gp_seq_needed;
    long unsigned int completedqs;
    long unsigned int qsmask;
    long unsigned int rcu_gp_init_mask;
    long unsigned int qsmaskinit;
    long unsigned int qsmaskinitnext;
    long unsigned int expmask;
    long unsigned int expmaskinit;
    long unsigned int expmaskinitnext;
    long unsigned int ffmask;
    long unsigned int grpmask;
    int grplo;
    int grphi;
    u8 grpnum;
    u8 level;
    bool wait_blkd_tasks;
    struct rcu_node *parent;
    struct list_head blkd_tasks;
    struct list_head *gp_tasks;
    struct list_head *exp_tasks;
    struct list_head *boost_tasks;
    struct rt_mutex boost_mtx;
    long unsigned int boost_time;
    struct task_struct *boost_kthread_task;
    unsigned int boost_kthread_status;
    raw_spinlock_t fqslock;
    spinlock_t exp_lock;
    long unsigned int exp_seq_rq;
    wait_queue_head_t exp_wq[4];
    struct rcu_exp_work rew;
    bool exp_need_flush;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rcu_node {
    raw_spinlock_t lock;
    long unsigned int gp_seq;
    long unsigned int gp_seq_needed;
    long unsigned int completedqs;
    long unsigned int qsmask;
    long unsigned int rcu_gp_init_mask;
    long unsigned int qsmaskinit;
    long unsigned int qsmaskinitnext;
    long unsigned int expmask;
    long unsigned int expmaskinit;
    long unsigned int expmaskinitnext;
    long unsigned int ffmask;
    long unsigned int grpmask;
    int grplo;
    int grphi;
    u8 grpnum;
    u8 level;
    bool wait_blkd_tasks;
    struct rcu_node *parent;
    struct list_head blkd_tasks;
    struct list_head *gp_tasks;
    struct list_head *exp_tasks;
    struct list_head *boost_tasks;
    struct rt_mutex boost_mtx;
    long unsigned int boost_time;
    struct task_struct *boost_kthread_task;
    unsigned int boost_kthread_status;
    raw_spinlock_t fqslock;
    spinlock_t exp_lock;
    long unsigned int exp_seq_rq;
    wait_queue_head_t exp_wq[4];
    struct rcu_exp_work rew;
    bool exp_need_flush;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct rcu_node {
    raw_spinlock_t lock;
    long unsigned int gp_seq;
    long unsigned int gp_seq_needed;
    long unsigned int completedqs;
    long unsigned int qsmask;
    long unsigned int rcu_gp_init_mask;
    long unsigned int qsmaskinit;
    long unsigned int qsmaskinitnext;
    long unsigned int expmask;
    long unsigned int expmaskinit;
    long unsigned int expmaskinitnext;
    long unsigned int ffmask;
    long unsigned int grpmask;
    int grplo;
    int grphi;
    u8 grpnum;
    u8 level;
    bool wait_blkd_tasks;
    struct rcu_node *parent;
    struct list_head blkd_tasks;
    struct list_head *gp_tasks;
    struct list_head *exp_tasks;
    struct list_head *boost_tasks;
    struct rt_mutex boost_mtx;
    long unsigned int boost_time;
    struct task_struct *boost_kthread_task;
    unsigned int boost_kthread_status;
    raw_spinlock_t fqslock;
    spinlock_t exp_lock;
    long unsigned int exp_seq_rq;
    wait_queue_head_t exp_wq[4];
    struct rcu_exp_work rew;
    bool exp_need_flush;
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
struct rcu_node {
    raw_spinlock_t lock;
    long unsigned int gp_seq;
    long unsigned int gp_seq_needed;
    long unsigned int completedqs;
    long unsigned int qsmask;
    long unsigned int rcu_gp_init_mask;
    long unsigned int qsmaskinit;
    long unsigned int qsmaskinitnext;
    long unsigned int expmask;
    long unsigned int expmaskinit;
    long unsigned int expmaskinitnext;
    long unsigned int ffmask;
    long unsigned int grpmask;
    int grplo;
    int grphi;
    u8 grpnum;
    u8 level;
    bool wait_blkd_tasks;
    struct rcu_node *parent;
    struct list_head blkd_tasks;
    struct list_head *gp_tasks;
    struct list_head *exp_tasks;
    struct list_head *boost_tasks;
    struct rt_mutex boost_mtx;
    long unsigned int boost_time;
    struct task_struct *boost_kthread_task;
    unsigned int boost_kthread_status;
    raw_spinlock_t fqslock;
    spinlock_t exp_lock;
    long unsigned int exp_seq_rq;
    wait_queue_head_t exp_wq[4];
    struct rcu_exp_work rew;
    bool exp_need_flush;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rcu_node {
    raw_spinlock_t lock;
    long unsigned int gp_seq;
    long unsigned int gp_seq_needed;
    long unsigned int completedqs;
    long unsigned int qsmask;
    long unsigned int rcu_gp_init_mask;
    long unsigned int qsmaskinit;
    long unsigned int qsmaskinitnext;
    long unsigned int expmask;
    long unsigned int expmaskinit;
    long unsigned int expmaskinitnext;
    long unsigned int ffmask;
    long unsigned int grpmask;
    int grplo;
    int grphi;
    u8 grpnum;
    u8 level;
    bool wait_blkd_tasks;
    struct rcu_node *parent;
    struct list_head blkd_tasks;
    struct list_head *gp_tasks;
    struct list_head *exp_tasks;
    struct list_head *boost_tasks;
    struct rt_mutex boost_mtx;
    long unsigned int boost_time;
    struct task_struct *boost_kthread_task;
    unsigned int boost_kthread_status;
    struct swait_queue_head nocb_gp_wq[2];
    raw_spinlock_t fqslock;
    spinlock_t exp_lock;
    long unsigned int exp_seq_rq;
    wait_queue_head_t exp_wq[4];
    struct rcu_exp_work rew;
    bool exp_need_flush;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rcu_node {
    raw_spinlock_t lock;
    long unsigned int gp_seq;
    long unsigned int gp_seq_needed;
    long unsigned int completedqs;
    long unsigned int qsmask;
    long unsigned int rcu_gp_init_mask;
    long unsigned int qsmaskinit;
    long unsigned int qsmaskinitnext;
    long unsigned int expmask;
    long unsigned int expmaskinit;
    long unsigned int expmaskinitnext;
    long unsigned int ffmask;
    long unsigned int grpmask;
    int grplo;
    int grphi;
    u8 grpnum;
    u8 level;
    bool wait_blkd_tasks;
    struct rcu_node *parent;
    struct list_head blkd_tasks;
    struct list_head *gp_tasks;
    struct list_head *exp_tasks;
    struct list_head *boost_tasks;
    struct rt_mutex boost_mtx;
    long unsigned int boost_time;
    struct task_struct *boost_kthread_task;
    unsigned int boost_kthread_status;
    raw_spinlock_t fqslock;
    spinlock_t exp_lock;
    long unsigned int exp_seq_rq;
    wait_queue_head_t exp_wq[4];
    struct rcu_exp_work rew;
    bool exp_need_flush;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rcu_node {
    raw_spinlock_t lock;
    long unsigned int gp_seq;
    long unsigned int gp_seq_needed;
    long unsigned int completedqs;
    long unsigned int qsmask;
    long unsigned int rcu_gp_init_mask;
    long unsigned int qsmaskinit;
    long unsigned int qsmaskinitnext;
    long unsigned int expmask;
    long unsigned int expmaskinit;
    long unsigned int expmaskinitnext;
    long unsigned int ffmask;
    long unsigned int grpmask;
    int grplo;
    int grphi;
    u8 grpnum;
    u8 level;
    bool wait_blkd_tasks;
    struct rcu_node *parent;
    struct list_head blkd_tasks;
    struct list_head *gp_tasks;
    struct list_head *exp_tasks;
    struct list_head *boost_tasks;
    struct rt_mutex boost_mtx;
    long unsigned int boost_time;
    struct task_struct *boost_kthread_task;
    unsigned int boost_kthread_status;
    raw_spinlock_t fqslock;
    spinlock_t exp_lock;
    long unsigned int exp_seq_rq;
    wait_queue_head_t exp_wq[4];
    struct rcu_exp_work rew;
    bool exp_need_flush;
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
<code>spinlock_t exp_lock</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int exp_seq_rq</code>
</li>
<li>
<b>Field added. </b>
<code>wait_queue_head_t exp_wq[4]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mutex exp_funnel_mutex</code>
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
<b>Field removed. </b>
<code>long unsigned int n_balk_blkd_tasks</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int n_balk_exp_gp_tasks</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int n_balk_boost_tasks</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int n_balk_notblocked</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int n_balk_notyet</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int n_balk_nos</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int ffmask</code>
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
<code>struct rcu_exp_work rew</code>
</li>
<li>
<b>Field added. </b>
<code>bool exp_need_flush</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int n_tasks_boosted</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int n_exp_boosts</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int n_normal_boosts</code>
</li>
<li>
<b>Field type changed. </b>
<code>int need_future_gp[2]</code> ➡️ <code>u8 need_future_gp[4]</code>
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
<code>long unsigned int gp_seq_needed</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int completedqs</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int rcu_gp_init_mask</code>
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
<code>u8 need_future_gp[4]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
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
<code>long unsigned int cbovldmask</code>
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
<code>long unsigned int ofl_seq</code>
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
<code>long unsigned int n_boosts</code>
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
<code>struct mutex boost_kthread_mutex</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int ofl_seq</code>
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
<code>raw_spinlock_t exp_poll_lock</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int exp_seq_poll_rq</code>
</li>
<li>
<b>Field added. </b>
<code>struct work_struct exp_poll_wq</code>
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
<code>struct swait_queue_head nocb_gp_wq[2]</code>
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
<details>
<summary>Changed between <code>generic</code> and <code>azure</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct swait_queue_head nocb_gp_wq[2]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
