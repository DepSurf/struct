# Struct: <code>signal_struct</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct signal_struct {
    atomic_t sigcnt;
    atomic_t live;
    int nr_threads;
    struct list_head thread_head;
    wait_queue_head_t wait_chldexit;
    struct task_struct *curr_target;
    struct sigpending shared_pending;
    int group_exit_code;
    int notify_count;
    struct task_struct *group_exit_task;
    int group_stop_count;
    unsigned int flags;
    unsigned int is_child_subreaper;
    unsigned int has_child_subreaper;
    int posix_timer_id;
    struct list_head posix_timers;
    struct hrtimer real_timer;
    struct pid *leader_pid;
    ktime_t it_real_incr;
    struct cpu_itimer it[2];
    struct thread_group_cputimer cputimer;
    struct task_cputime cputime_expires;
    struct list_head cpu_timers[3];
    struct pid *tty_old_pgrp;
    int leader;
    struct tty_struct *tty;
    struct autogroup *autogroup;
    seqlock_t stats_lock;
    cputime_t utime;
    cputime_t stime;
    cputime_t cutime;
    cputime_t cstime;
    cputime_t gtime;
    cputime_t cgtime;
    struct prev_cputime prev_cputime;
    long unsigned int nvcsw;
    long unsigned int nivcsw;
    long unsigned int cnvcsw;
    long unsigned int cnivcsw;
    long unsigned int min_flt;
    long unsigned int maj_flt;
    long unsigned int cmin_flt;
    long unsigned int cmaj_flt;
    long unsigned int inblock;
    long unsigned int oublock;
    long unsigned int cinblock;
    long unsigned int coublock;
    long unsigned int maxrss;
    long unsigned int cmaxrss;
    struct task_io_accounting ioac;
    long long unsigned int sum_sched_runtime;
    struct rlimit rlim[16];
    struct pacct_struct pacct;
    struct taskstats *stats;
    unsigned int audit_tty;
    unsigned int audit_tty_log_passwd;
    struct tty_audit_buf *tty_audit_buf;
    oom_flags_t oom_flags;
    short int oom_score_adj;
    short int oom_score_adj_min;
    struct mutex cred_guard_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct signal_struct {
    atomic_t sigcnt;
    atomic_t live;
    int nr_threads;
    atomic_t oom_victims;
    struct list_head thread_head;
    wait_queue_head_t wait_chldexit;
    struct task_struct *curr_target;
    struct sigpending shared_pending;
    int group_exit_code;
    int notify_count;
    struct task_struct *group_exit_task;
    int group_stop_count;
    unsigned int flags;
    unsigned int is_child_subreaper;
    unsigned int has_child_subreaper;
    int posix_timer_id;
    struct list_head posix_timers;
    struct hrtimer real_timer;
    struct pid *leader_pid;
    ktime_t it_real_incr;
    struct cpu_itimer it[2];
    struct thread_group_cputimer cputimer;
    struct task_cputime cputime_expires;
    struct list_head cpu_timers[3];
    struct pid *tty_old_pgrp;
    int leader;
    struct tty_struct *tty;
    struct autogroup *autogroup;
    seqlock_t stats_lock;
    cputime_t utime;
    cputime_t stime;
    cputime_t cutime;
    cputime_t cstime;
    cputime_t gtime;
    cputime_t cgtime;
    struct prev_cputime prev_cputime;
    long unsigned int nvcsw;
    long unsigned int nivcsw;
    long unsigned int cnvcsw;
    long unsigned int cnivcsw;
    long unsigned int min_flt;
    long unsigned int maj_flt;
    long unsigned int cmin_flt;
    long unsigned int cmaj_flt;
    long unsigned int inblock;
    long unsigned int oublock;
    long unsigned int cinblock;
    long unsigned int coublock;
    long unsigned int maxrss;
    long unsigned int cmaxrss;
    struct task_io_accounting ioac;
    long long unsigned int sum_sched_runtime;
    struct rlimit rlim[16];
    struct pacct_struct pacct;
    struct taskstats *stats;
    unsigned int audit_tty;
    struct tty_audit_buf *tty_audit_buf;
    bool oom_flag_origin;
    short int oom_score_adj;
    short int oom_score_adj_min;
    struct mutex cred_guard_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct signal_struct {
    atomic_t sigcnt;
    atomic_t live;
    int nr_threads;
    struct list_head thread_head;
    wait_queue_head_t wait_chldexit;
    struct task_struct *curr_target;
    struct sigpending shared_pending;
    int group_exit_code;
    int notify_count;
    struct task_struct *group_exit_task;
    int group_stop_count;
    unsigned int flags;
    unsigned int is_child_subreaper;
    unsigned int has_child_subreaper;
    int posix_timer_id;
    struct list_head posix_timers;
    struct hrtimer real_timer;
    struct pid *leader_pid;
    ktime_t it_real_incr;
    struct cpu_itimer it[2];
    struct thread_group_cputimer cputimer;
    struct task_cputime cputime_expires;
    struct list_head cpu_timers[3];
    struct pid *tty_old_pgrp;
    int leader;
    struct tty_struct *tty;
    struct autogroup *autogroup;
    seqlock_t stats_lock;
    cputime_t utime;
    cputime_t stime;
    cputime_t cutime;
    cputime_t cstime;
    cputime_t gtime;
    cputime_t cgtime;
    struct prev_cputime prev_cputime;
    long unsigned int nvcsw;
    long unsigned int nivcsw;
    long unsigned int cnvcsw;
    long unsigned int cnivcsw;
    long unsigned int min_flt;
    long unsigned int maj_flt;
    long unsigned int cmin_flt;
    long unsigned int cmaj_flt;
    long unsigned int inblock;
    long unsigned int oublock;
    long unsigned int cinblock;
    long unsigned int coublock;
    long unsigned int maxrss;
    long unsigned int cmaxrss;
    struct task_io_accounting ioac;
    long long unsigned int sum_sched_runtime;
    struct rlimit rlim[16];
    struct pacct_struct pacct;
    struct taskstats *stats;
    unsigned int audit_tty;
    struct tty_audit_buf *tty_audit_buf;
    bool oom_flag_origin;
    short int oom_score_adj;
    short int oom_score_adj_min;
    struct mm_struct *oom_mm;
    struct mutex cred_guard_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct signal_struct {
    atomic_t sigcnt;
    atomic_t live;
    int nr_threads;
    struct list_head thread_head;
    wait_queue_head_t wait_chldexit;
    struct task_struct *curr_target;
    struct sigpending shared_pending;
    int group_exit_code;
    int notify_count;
    struct task_struct *group_exit_task;
    int group_stop_count;
    unsigned int flags;
    unsigned int is_child_subreaper;
    unsigned int has_child_subreaper;
    int posix_timer_id;
    struct list_head posix_timers;
    struct hrtimer real_timer;
    ktime_t it_real_incr;
    struct cpu_itimer it[2];
    struct thread_group_cputimer cputimer;
    struct task_cputime cputime_expires;
    struct list_head cpu_timers[3];
    struct pid *leader_pid;
    struct pid *tty_old_pgrp;
    int leader;
    struct tty_struct *tty;
    struct autogroup *autogroup;
    seqlock_t stats_lock;
    u64 utime;
    u64 stime;
    u64 cutime;
    u64 cstime;
    u64 gtime;
    u64 cgtime;
    struct prev_cputime prev_cputime;
    long unsigned int nvcsw;
    long unsigned int nivcsw;
    long unsigned int cnvcsw;
    long unsigned int cnivcsw;
    long unsigned int min_flt;
    long unsigned int maj_flt;
    long unsigned int cmin_flt;
    long unsigned int cmaj_flt;
    long unsigned int inblock;
    long unsigned int oublock;
    long unsigned int cinblock;
    long unsigned int coublock;
    long unsigned int maxrss;
    long unsigned int cmaxrss;
    struct task_io_accounting ioac;
    long long unsigned int sum_sched_runtime;
    struct rlimit rlim[16];
    struct pacct_struct pacct;
    struct taskstats *stats;
    unsigned int audit_tty;
    struct tty_audit_buf *tty_audit_buf;
    bool oom_flag_origin;
    short int oom_score_adj;
    short int oom_score_adj_min;
    struct mm_struct *oom_mm;
    struct mutex cred_guard_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct signal_struct {
    atomic_t sigcnt;
    atomic_t live;
    int nr_threads;
    struct list_head thread_head;
    wait_queue_head_t wait_chldexit;
    struct task_struct *curr_target;
    struct sigpending shared_pending;
    int group_exit_code;
    int notify_count;
    struct task_struct *group_exit_task;
    int group_stop_count;
    unsigned int flags;
    unsigned int is_child_subreaper;
    unsigned int has_child_subreaper;
    int posix_timer_id;
    struct list_head posix_timers;
    struct hrtimer real_timer;
    ktime_t it_real_incr;
    struct cpu_itimer it[2];
    struct thread_group_cputimer cputimer;
    struct task_cputime cputime_expires;
    struct list_head cpu_timers[3];
    struct pid *leader_pid;
    struct pid *tty_old_pgrp;
    int leader;
    struct tty_struct *tty;
    struct autogroup *autogroup;
    seqlock_t stats_lock;
    u64 utime;
    u64 stime;
    u64 cutime;
    u64 cstime;
    u64 gtime;
    u64 cgtime;
    struct prev_cputime prev_cputime;
    long unsigned int nvcsw;
    long unsigned int nivcsw;
    long unsigned int cnvcsw;
    long unsigned int cnivcsw;
    long unsigned int min_flt;
    long unsigned int maj_flt;
    long unsigned int cmin_flt;
    long unsigned int cmaj_flt;
    long unsigned int inblock;
    long unsigned int oublock;
    long unsigned int cinblock;
    long unsigned int coublock;
    long unsigned int maxrss;
    long unsigned int cmaxrss;
    struct task_io_accounting ioac;
    long long unsigned int sum_sched_runtime;
    struct rlimit rlim[16];
    struct pacct_struct pacct;
    struct taskstats *stats;
    unsigned int audit_tty;
    struct tty_audit_buf *tty_audit_buf;
    bool oom_flag_origin;
    short int oom_score_adj;
    short int oom_score_adj_min;
    struct mm_struct *oom_mm;
    struct mutex cred_guard_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct signal_struct {
    atomic_t sigcnt;
    atomic_t live;
    int nr_threads;
    struct list_head thread_head;
    wait_queue_head_t wait_chldexit;
    struct task_struct *curr_target;
    struct sigpending shared_pending;
    int group_exit_code;
    int notify_count;
    struct task_struct *group_exit_task;
    int group_stop_count;
    unsigned int flags;
    unsigned int is_child_subreaper;
    unsigned int has_child_subreaper;
    int posix_timer_id;
    struct list_head posix_timers;
    struct hrtimer real_timer;
    ktime_t it_real_incr;
    struct cpu_itimer it[2];
    struct thread_group_cputimer cputimer;
    struct task_cputime cputime_expires;
    struct list_head cpu_timers[3];
    struct pid *leader_pid;
    struct pid *tty_old_pgrp;
    int leader;
    struct tty_struct *tty;
    struct autogroup *autogroup;
    seqlock_t stats_lock;
    u64 utime;
    u64 stime;
    u64 cutime;
    u64 cstime;
    u64 gtime;
    u64 cgtime;
    struct prev_cputime prev_cputime;
    long unsigned int nvcsw;
    long unsigned int nivcsw;
    long unsigned int cnvcsw;
    long unsigned int cnivcsw;
    long unsigned int min_flt;
    long unsigned int maj_flt;
    long unsigned int cmin_flt;
    long unsigned int cmaj_flt;
    long unsigned int inblock;
    long unsigned int oublock;
    long unsigned int cinblock;
    long unsigned int coublock;
    long unsigned int maxrss;
    long unsigned int cmaxrss;
    struct task_io_accounting ioac;
    long long unsigned int sum_sched_runtime;
    struct rlimit rlim[16];
    struct pacct_struct pacct;
    struct taskstats *stats;
    unsigned int audit_tty;
    struct tty_audit_buf *tty_audit_buf;
    bool oom_flag_origin;
    short int oom_score_adj;
    short int oom_score_adj_min;
    struct mm_struct *oom_mm;
    struct mutex cred_guard_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct signal_struct {
    atomic_t sigcnt;
    atomic_t live;
    int nr_threads;
    struct list_head thread_head;
    wait_queue_head_t wait_chldexit;
    struct task_struct *curr_target;
    struct sigpending shared_pending;
    struct hlist_head multiprocess;
    int group_exit_code;
    int notify_count;
    struct task_struct *group_exit_task;
    int group_stop_count;
    unsigned int flags;
    unsigned int is_child_subreaper;
    unsigned int has_child_subreaper;
    int posix_timer_id;
    struct list_head posix_timers;
    struct hrtimer real_timer;
    ktime_t it_real_incr;
    struct cpu_itimer it[2];
    struct thread_group_cputimer cputimer;
    struct task_cputime cputime_expires;
    struct list_head cpu_timers[3];
    struct pid * pids[4];
    struct pid *tty_old_pgrp;
    int leader;
    struct tty_struct *tty;
    struct autogroup *autogroup;
    seqlock_t stats_lock;
    u64 utime;
    u64 stime;
    u64 cutime;
    u64 cstime;
    u64 gtime;
    u64 cgtime;
    struct prev_cputime prev_cputime;
    long unsigned int nvcsw;
    long unsigned int nivcsw;
    long unsigned int cnvcsw;
    long unsigned int cnivcsw;
    long unsigned int min_flt;
    long unsigned int maj_flt;
    long unsigned int cmin_flt;
    long unsigned int cmaj_flt;
    long unsigned int inblock;
    long unsigned int oublock;
    long unsigned int cinblock;
    long unsigned int coublock;
    long unsigned int maxrss;
    long unsigned int cmaxrss;
    struct task_io_accounting ioac;
    long long unsigned int sum_sched_runtime;
    struct rlimit rlim[16];
    struct pacct_struct pacct;
    struct taskstats *stats;
    unsigned int audit_tty;
    struct tty_audit_buf *tty_audit_buf;
    bool oom_flag_origin;
    short int oom_score_adj;
    short int oom_score_adj_min;
    struct mm_struct *oom_mm;
    struct mutex cred_guard_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct signal_struct {
    refcount_t sigcnt;
    atomic_t live;
    int nr_threads;
    struct list_head thread_head;
    wait_queue_head_t wait_chldexit;
    struct task_struct *curr_target;
    struct sigpending shared_pending;
    struct hlist_head multiprocess;
    int group_exit_code;
    int notify_count;
    struct task_struct *group_exit_task;
    int group_stop_count;
    unsigned int flags;
    unsigned int is_child_subreaper;
    unsigned int has_child_subreaper;
    int posix_timer_id;
    struct list_head posix_timers;
    struct hrtimer real_timer;
    ktime_t it_real_incr;
    struct cpu_itimer it[2];
    struct thread_group_cputimer cputimer;
    struct task_cputime cputime_expires;
    struct list_head cpu_timers[3];
    struct pid * pids[4];
    struct pid *tty_old_pgrp;
    int leader;
    struct tty_struct *tty;
    struct autogroup *autogroup;
    seqlock_t stats_lock;
    u64 utime;
    u64 stime;
    u64 cutime;
    u64 cstime;
    u64 gtime;
    u64 cgtime;
    struct prev_cputime prev_cputime;
    long unsigned int nvcsw;
    long unsigned int nivcsw;
    long unsigned int cnvcsw;
    long unsigned int cnivcsw;
    long unsigned int min_flt;
    long unsigned int maj_flt;
    long unsigned int cmin_flt;
    long unsigned int cmaj_flt;
    long unsigned int inblock;
    long unsigned int oublock;
    long unsigned int cinblock;
    long unsigned int coublock;
    long unsigned int maxrss;
    long unsigned int cmaxrss;
    struct task_io_accounting ioac;
    long long unsigned int sum_sched_runtime;
    struct rlimit rlim[16];
    struct pacct_struct pacct;
    struct taskstats *stats;
    unsigned int audit_tty;
    struct tty_audit_buf *tty_audit_buf;
    bool oom_flag_origin;
    short int oom_score_adj;
    short int oom_score_adj_min;
    struct mm_struct *oom_mm;
    struct mutex cred_guard_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct signal_struct {
    refcount_t sigcnt;
    atomic_t live;
    int nr_threads;
    struct list_head thread_head;
    wait_queue_head_t wait_chldexit;
    struct task_struct *curr_target;
    struct sigpending shared_pending;
    struct hlist_head multiprocess;
    int group_exit_code;
    int notify_count;
    struct task_struct *group_exit_task;
    int group_stop_count;
    unsigned int flags;
    unsigned int is_child_subreaper;
    unsigned int has_child_subreaper;
    int posix_timer_id;
    struct list_head posix_timers;
    struct hrtimer real_timer;
    ktime_t it_real_incr;
    struct cpu_itimer it[2];
    struct thread_group_cputimer cputimer;
    struct posix_cputimers posix_cputimers;
    struct pid * pids[4];
    struct pid *tty_old_pgrp;
    int leader;
    struct tty_struct *tty;
    struct autogroup *autogroup;
    seqlock_t stats_lock;
    u64 utime;
    u64 stime;
    u64 cutime;
    u64 cstime;
    u64 gtime;
    u64 cgtime;
    struct prev_cputime prev_cputime;
    long unsigned int nvcsw;
    long unsigned int nivcsw;
    long unsigned int cnvcsw;
    long unsigned int cnivcsw;
    long unsigned int min_flt;
    long unsigned int maj_flt;
    long unsigned int cmin_flt;
    long unsigned int cmaj_flt;
    long unsigned int inblock;
    long unsigned int oublock;
    long unsigned int cinblock;
    long unsigned int coublock;
    long unsigned int maxrss;
    long unsigned int cmaxrss;
    struct task_io_accounting ioac;
    long long unsigned int sum_sched_runtime;
    struct rlimit rlim[16];
    struct pacct_struct pacct;
    struct taskstats *stats;
    unsigned int audit_tty;
    struct tty_audit_buf *tty_audit_buf;
    bool oom_flag_origin;
    short int oom_score_adj;
    short int oom_score_adj_min;
    struct mm_struct *oom_mm;
    struct mutex cred_guard_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct signal_struct {
    refcount_t sigcnt;
    atomic_t live;
    int nr_threads;
    struct list_head thread_head;
    wait_queue_head_t wait_chldexit;
    struct task_struct *curr_target;
    struct sigpending shared_pending;
    struct hlist_head multiprocess;
    int group_exit_code;
    int notify_count;
    struct task_struct *group_exit_task;
    int group_stop_count;
    unsigned int flags;
    unsigned int is_child_subreaper;
    unsigned int has_child_subreaper;
    int posix_timer_id;
    struct list_head posix_timers;
    struct hrtimer real_timer;
    ktime_t it_real_incr;
    struct cpu_itimer it[2];
    struct thread_group_cputimer cputimer;
    struct posix_cputimers posix_cputimers;
    struct pid * pids[4];
    struct pid *tty_old_pgrp;
    int leader;
    struct tty_struct *tty;
    struct autogroup *autogroup;
    seqlock_t stats_lock;
    u64 utime;
    u64 stime;
    u64 cutime;
    u64 cstime;
    u64 gtime;
    u64 cgtime;
    struct prev_cputime prev_cputime;
    long unsigned int nvcsw;
    long unsigned int nivcsw;
    long unsigned int cnvcsw;
    long unsigned int cnivcsw;
    long unsigned int min_flt;
    long unsigned int maj_flt;
    long unsigned int cmin_flt;
    long unsigned int cmaj_flt;
    long unsigned int inblock;
    long unsigned int oublock;
    long unsigned int cinblock;
    long unsigned int coublock;
    long unsigned int maxrss;
    long unsigned int cmaxrss;
    struct task_io_accounting ioac;
    long long unsigned int sum_sched_runtime;
    struct rlimit rlim[16];
    struct pacct_struct pacct;
    struct taskstats *stats;
    unsigned int audit_tty;
    struct tty_audit_buf *tty_audit_buf;
    bool oom_flag_origin;
    short int oom_score_adj;
    short int oom_score_adj_min;
    struct mm_struct *oom_mm;
    struct mutex cred_guard_mutex;
    struct mutex exec_update_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct signal_struct {
    refcount_t sigcnt;
    atomic_t live;
    int nr_threads;
    struct list_head thread_head;
    wait_queue_head_t wait_chldexit;
    struct task_struct *curr_target;
    struct sigpending shared_pending;
    struct hlist_head multiprocess;
    int group_exit_code;
    int notify_count;
    struct task_struct *group_exit_task;
    int group_stop_count;
    unsigned int flags;
    unsigned int is_child_subreaper;
    unsigned int has_child_subreaper;
    int posix_timer_id;
    struct list_head posix_timers;
    struct hrtimer real_timer;
    ktime_t it_real_incr;
    struct cpu_itimer it[2];
    struct thread_group_cputimer cputimer;
    struct posix_cputimers posix_cputimers;
    struct pid * pids[4];
    struct pid *tty_old_pgrp;
    int leader;
    struct tty_struct *tty;
    struct autogroup *autogroup;
    seqlock_t stats_lock;
    u64 utime;
    u64 stime;
    u64 cutime;
    u64 cstime;
    u64 gtime;
    u64 cgtime;
    struct prev_cputime prev_cputime;
    long unsigned int nvcsw;
    long unsigned int nivcsw;
    long unsigned int cnvcsw;
    long unsigned int cnivcsw;
    long unsigned int min_flt;
    long unsigned int maj_flt;
    long unsigned int cmin_flt;
    long unsigned int cmaj_flt;
    long unsigned int inblock;
    long unsigned int oublock;
    long unsigned int cinblock;
    long unsigned int coublock;
    long unsigned int maxrss;
    long unsigned int cmaxrss;
    struct task_io_accounting ioac;
    long long unsigned int sum_sched_runtime;
    struct rlimit rlim[16];
    struct pacct_struct pacct;
    struct taskstats *stats;
    unsigned int audit_tty;
    struct tty_audit_buf *tty_audit_buf;
    bool oom_flag_origin;
    short int oom_score_adj;
    short int oom_score_adj_min;
    struct mm_struct *oom_mm;
    struct mutex cred_guard_mutex;
    struct rw_semaphore exec_update_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct signal_struct {
    refcount_t sigcnt;
    atomic_t live;
    int nr_threads;
    struct list_head thread_head;
    wait_queue_head_t wait_chldexit;
    struct task_struct *curr_target;
    struct sigpending shared_pending;
    struct hlist_head multiprocess;
    int group_exit_code;
    int notify_count;
    struct task_struct *group_exit_task;
    int group_stop_count;
    unsigned int flags;
    unsigned int is_child_subreaper;
    unsigned int has_child_subreaper;
    int posix_timer_id;
    struct list_head posix_timers;
    struct hrtimer real_timer;
    ktime_t it_real_incr;
    struct cpu_itimer it[2];
    struct thread_group_cputimer cputimer;
    struct posix_cputimers posix_cputimers;
    struct pid * pids[4];
    struct pid *tty_old_pgrp;
    int leader;
    struct tty_struct *tty;
    struct autogroup *autogroup;
    seqlock_t stats_lock;
    u64 utime;
    u64 stime;
    u64 cutime;
    u64 cstime;
    u64 gtime;
    u64 cgtime;
    struct prev_cputime prev_cputime;
    long unsigned int nvcsw;
    long unsigned int nivcsw;
    long unsigned int cnvcsw;
    long unsigned int cnivcsw;
    long unsigned int min_flt;
    long unsigned int maj_flt;
    long unsigned int cmin_flt;
    long unsigned int cmaj_flt;
    long unsigned int inblock;
    long unsigned int oublock;
    long unsigned int cinblock;
    long unsigned int coublock;
    long unsigned int maxrss;
    long unsigned int cmaxrss;
    struct task_io_accounting ioac;
    long long unsigned int sum_sched_runtime;
    struct rlimit rlim[16];
    struct pacct_struct pacct;
    struct taskstats *stats;
    unsigned int audit_tty;
    struct tty_audit_buf *tty_audit_buf;
    bool oom_flag_origin;
    short int oom_score_adj;
    short int oom_score_adj_min;
    struct mm_struct *oom_mm;
    struct mutex cred_guard_mutex;
    struct rw_semaphore exec_update_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct signal_struct {
    refcount_t sigcnt;
    atomic_t live;
    int nr_threads;
    struct list_head thread_head;
    wait_queue_head_t wait_chldexit;
    struct task_struct *curr_target;
    struct sigpending shared_pending;
    struct hlist_head multiprocess;
    int group_exit_code;
    int notify_count;
    struct task_struct *group_exit_task;
    int group_stop_count;
    unsigned int flags;
    unsigned int is_child_subreaper;
    unsigned int has_child_subreaper;
    int posix_timer_id;
    struct list_head posix_timers;
    struct hrtimer real_timer;
    ktime_t it_real_incr;
    struct cpu_itimer it[2];
    struct thread_group_cputimer cputimer;
    struct posix_cputimers posix_cputimers;
    struct pid * pids[4];
    struct pid *tty_old_pgrp;
    int leader;
    struct tty_struct *tty;
    struct autogroup *autogroup;
    seqlock_t stats_lock;
    u64 utime;
    u64 stime;
    u64 cutime;
    u64 cstime;
    u64 gtime;
    u64 cgtime;
    struct prev_cputime prev_cputime;
    long unsigned int nvcsw;
    long unsigned int nivcsw;
    long unsigned int cnvcsw;
    long unsigned int cnivcsw;
    long unsigned int min_flt;
    long unsigned int maj_flt;
    long unsigned int cmin_flt;
    long unsigned int cmaj_flt;
    long unsigned int inblock;
    long unsigned int oublock;
    long unsigned int cinblock;
    long unsigned int coublock;
    long unsigned int maxrss;
    long unsigned int cmaxrss;
    struct task_io_accounting ioac;
    long long unsigned int sum_sched_runtime;
    struct rlimit rlim[16];
    struct pacct_struct pacct;
    struct taskstats *stats;
    unsigned int audit_tty;
    struct tty_audit_buf *tty_audit_buf;
    bool oom_flag_origin;
    short int oom_score_adj;
    short int oom_score_adj_min;
    struct mm_struct *oom_mm;
    struct mutex cred_guard_mutex;
    struct rw_semaphore exec_update_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct signal_struct {
    refcount_t sigcnt;
    atomic_t live;
    int nr_threads;
    struct list_head thread_head;
    wait_queue_head_t wait_chldexit;
    struct task_struct *curr_target;
    struct sigpending shared_pending;
    struct hlist_head multiprocess;
    int group_exit_code;
    int notify_count;
    struct task_struct *group_exec_task;
    int group_stop_count;
    unsigned int flags;
    struct core_state *core_state;
    unsigned int is_child_subreaper;
    unsigned int has_child_subreaper;
    int posix_timer_id;
    struct list_head posix_timers;
    struct hrtimer real_timer;
    ktime_t it_real_incr;
    struct cpu_itimer it[2];
    struct thread_group_cputimer cputimer;
    struct posix_cputimers posix_cputimers;
    struct pid * pids[4];
    struct pid *tty_old_pgrp;
    int leader;
    struct tty_struct *tty;
    struct autogroup *autogroup;
    seqlock_t stats_lock;
    u64 utime;
    u64 stime;
    u64 cutime;
    u64 cstime;
    u64 gtime;
    u64 cgtime;
    struct prev_cputime prev_cputime;
    long unsigned int nvcsw;
    long unsigned int nivcsw;
    long unsigned int cnvcsw;
    long unsigned int cnivcsw;
    long unsigned int min_flt;
    long unsigned int maj_flt;
    long unsigned int cmin_flt;
    long unsigned int cmaj_flt;
    long unsigned int inblock;
    long unsigned int oublock;
    long unsigned int cinblock;
    long unsigned int coublock;
    long unsigned int maxrss;
    long unsigned int cmaxrss;
    struct task_io_accounting ioac;
    long long unsigned int sum_sched_runtime;
    struct rlimit rlim[16];
    struct pacct_struct pacct;
    struct taskstats *stats;
    unsigned int audit_tty;
    struct tty_audit_buf *tty_audit_buf;
    bool oom_flag_origin;
    short int oom_score_adj;
    short int oom_score_adj_min;
    struct mm_struct *oom_mm;
    struct mutex cred_guard_mutex;
    struct rw_semaphore exec_update_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct signal_struct {
    refcount_t sigcnt;
    atomic_t live;
    int nr_threads;
    int quick_threads;
    struct list_head thread_head;
    wait_queue_head_t wait_chldexit;
    struct task_struct *curr_target;
    struct sigpending shared_pending;
    struct hlist_head multiprocess;
    int group_exit_code;
    int notify_count;
    struct task_struct *group_exec_task;
    int group_stop_count;
    unsigned int flags;
    struct core_state *core_state;
    unsigned int is_child_subreaper;
    unsigned int has_child_subreaper;
    int posix_timer_id;
    struct list_head posix_timers;
    struct hrtimer real_timer;
    ktime_t it_real_incr;
    struct cpu_itimer it[2];
    struct thread_group_cputimer cputimer;
    struct posix_cputimers posix_cputimers;
    struct pid * pids[4];
    struct pid *tty_old_pgrp;
    int leader;
    struct tty_struct *tty;
    struct autogroup *autogroup;
    seqlock_t stats_lock;
    u64 utime;
    u64 stime;
    u64 cutime;
    u64 cstime;
    u64 gtime;
    u64 cgtime;
    struct prev_cputime prev_cputime;
    long unsigned int nvcsw;
    long unsigned int nivcsw;
    long unsigned int cnvcsw;
    long unsigned int cnivcsw;
    long unsigned int min_flt;
    long unsigned int maj_flt;
    long unsigned int cmin_flt;
    long unsigned int cmaj_flt;
    long unsigned int inblock;
    long unsigned int oublock;
    long unsigned int cinblock;
    long unsigned int coublock;
    long unsigned int maxrss;
    long unsigned int cmaxrss;
    struct task_io_accounting ioac;
    long long unsigned int sum_sched_runtime;
    struct rlimit rlim[16];
    struct pacct_struct pacct;
    struct taskstats *stats;
    unsigned int audit_tty;
    struct tty_audit_buf *tty_audit_buf;
    bool oom_flag_origin;
    short int oom_score_adj;
    short int oom_score_adj_min;
    struct mm_struct *oom_mm;
    struct mutex cred_guard_mutex;
    struct rw_semaphore exec_update_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct signal_struct {
    refcount_t sigcnt;
    atomic_t live;
    int nr_threads;
    int quick_threads;
    struct list_head thread_head;
    wait_queue_head_t wait_chldexit;
    struct task_struct *curr_target;
    struct sigpending shared_pending;
    struct hlist_head multiprocess;
    int group_exit_code;
    int notify_count;
    struct task_struct *group_exec_task;
    int group_stop_count;
    unsigned int flags;
    struct core_state *core_state;
    unsigned int is_child_subreaper;
    unsigned int has_child_subreaper;
    unsigned int next_posix_timer_id;
    struct list_head posix_timers;
    struct hrtimer real_timer;
    ktime_t it_real_incr;
    struct cpu_itimer it[2];
    struct thread_group_cputimer cputimer;
    struct posix_cputimers posix_cputimers;
    struct pid * pids[4];
    struct pid *tty_old_pgrp;
    int leader;
    struct tty_struct *tty;
    struct autogroup *autogroup;
    seqlock_t stats_lock;
    u64 utime;
    u64 stime;
    u64 cutime;
    u64 cstime;
    u64 gtime;
    u64 cgtime;
    struct prev_cputime prev_cputime;
    long unsigned int nvcsw;
    long unsigned int nivcsw;
    long unsigned int cnvcsw;
    long unsigned int cnivcsw;
    long unsigned int min_flt;
    long unsigned int maj_flt;
    long unsigned int cmin_flt;
    long unsigned int cmaj_flt;
    long unsigned int inblock;
    long unsigned int oublock;
    long unsigned int cinblock;
    long unsigned int coublock;
    long unsigned int maxrss;
    long unsigned int cmaxrss;
    struct task_io_accounting ioac;
    long long unsigned int sum_sched_runtime;
    struct rlimit rlim[16];
    struct pacct_struct pacct;
    struct taskstats *stats;
    unsigned int audit_tty;
    struct tty_audit_buf *tty_audit_buf;
    bool oom_flag_origin;
    short int oom_score_adj;
    short int oom_score_adj_min;
    struct mm_struct *oom_mm;
    struct mutex cred_guard_mutex;
    struct rw_semaphore exec_update_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct signal_struct {
    refcount_t sigcnt;
    atomic_t live;
    int nr_threads;
    int quick_threads;
    struct list_head thread_head;
    wait_queue_head_t wait_chldexit;
    struct task_struct *curr_target;
    struct sigpending shared_pending;
    struct hlist_head multiprocess;
    int group_exit_code;
    int notify_count;
    struct task_struct *group_exec_task;
    int group_stop_count;
    unsigned int flags;
    struct core_state *core_state;
    unsigned int is_child_subreaper;
    unsigned int has_child_subreaper;
    unsigned int next_posix_timer_id;
    struct list_head posix_timers;
    struct hrtimer real_timer;
    ktime_t it_real_incr;
    struct cpu_itimer it[2];
    struct thread_group_cputimer cputimer;
    struct posix_cputimers posix_cputimers;
    struct pid * pids[4];
    atomic_t tick_dep_mask;
    struct pid *tty_old_pgrp;
    int leader;
    struct tty_struct *tty;
    struct autogroup *autogroup;
    seqlock_t stats_lock;
    u64 utime;
    u64 stime;
    u64 cutime;
    u64 cstime;
    u64 gtime;
    u64 cgtime;
    struct prev_cputime prev_cputime;
    long unsigned int nvcsw;
    long unsigned int nivcsw;
    long unsigned int cnvcsw;
    long unsigned int cnivcsw;
    long unsigned int min_flt;
    long unsigned int maj_flt;
    long unsigned int cmin_flt;
    long unsigned int cmaj_flt;
    long unsigned int inblock;
    long unsigned int oublock;
    long unsigned int cinblock;
    long unsigned int coublock;
    long unsigned int maxrss;
    long unsigned int cmaxrss;
    struct task_io_accounting ioac;
    long long unsigned int sum_sched_runtime;
    struct rlimit rlim[16];
    struct pacct_struct pacct;
    struct taskstats *stats;
    unsigned int audit_tty;
    struct tty_audit_buf *tty_audit_buf;
    bool oom_flag_origin;
    short int oom_score_adj;
    short int oom_score_adj_min;
    struct mm_struct *oom_mm;
    struct mutex cred_guard_mutex;
    struct rw_semaphore exec_update_lock;
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
struct signal_struct {
    refcount_t sigcnt;
    atomic_t live;
    int nr_threads;
    struct list_head thread_head;
    wait_queue_head_t wait_chldexit;
    struct task_struct *curr_target;
    struct sigpending shared_pending;
    struct hlist_head multiprocess;
    int group_exit_code;
    int notify_count;
    struct task_struct *group_exit_task;
    int group_stop_count;
    unsigned int flags;
    unsigned int is_child_subreaper;
    unsigned int has_child_subreaper;
    int posix_timer_id;
    struct list_head posix_timers;
    struct hrtimer real_timer;
    ktime_t it_real_incr;
    struct cpu_itimer it[2];
    struct thread_group_cputimer cputimer;
    struct posix_cputimers posix_cputimers;
    struct pid * pids[4];
    struct pid *tty_old_pgrp;
    int leader;
    struct tty_struct *tty;
    struct autogroup *autogroup;
    seqlock_t stats_lock;
    u64 utime;
    u64 stime;
    u64 cutime;
    u64 cstime;
    u64 gtime;
    u64 cgtime;
    struct prev_cputime prev_cputime;
    long unsigned int nvcsw;
    long unsigned int nivcsw;
    long unsigned int cnvcsw;
    long unsigned int cnivcsw;
    long unsigned int min_flt;
    long unsigned int maj_flt;
    long unsigned int cmin_flt;
    long unsigned int cmaj_flt;
    long unsigned int inblock;
    long unsigned int oublock;
    long unsigned int cinblock;
    long unsigned int coublock;
    long unsigned int maxrss;
    long unsigned int cmaxrss;
    struct task_io_accounting ioac;
    long long unsigned int sum_sched_runtime;
    struct rlimit rlim[16];
    struct pacct_struct pacct;
    struct taskstats *stats;
    unsigned int audit_tty;
    struct tty_audit_buf *tty_audit_buf;
    bool oom_flag_origin;
    short int oom_score_adj;
    short int oom_score_adj_min;
    struct mm_struct *oom_mm;
    struct mutex cred_guard_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct signal_struct {
    refcount_t sigcnt;
    atomic_t live;
    int nr_threads;
    struct list_head thread_head;
    wait_queue_head_t wait_chldexit;
    struct task_struct *curr_target;
    struct sigpending shared_pending;
    struct hlist_head multiprocess;
    int group_exit_code;
    int notify_count;
    struct task_struct *group_exit_task;
    int group_stop_count;
    unsigned int flags;
    unsigned int is_child_subreaper;
    unsigned int has_child_subreaper;
    int posix_timer_id;
    struct list_head posix_timers;
    struct hrtimer real_timer;
    ktime_t it_real_incr;
    struct cpu_itimer it[2];
    struct thread_group_cputimer cputimer;
    struct posix_cputimers posix_cputimers;
    struct pid * pids[4];
    struct pid *tty_old_pgrp;
    int leader;
    struct tty_struct *tty;
    struct autogroup *autogroup;
    seqlock_t stats_lock;
    u64 utime;
    u64 stime;
    u64 cutime;
    u64 cstime;
    u64 gtime;
    u64 cgtime;
    struct prev_cputime prev_cputime;
    long unsigned int nvcsw;
    long unsigned int nivcsw;
    long unsigned int cnvcsw;
    long unsigned int cnivcsw;
    long unsigned int min_flt;
    long unsigned int maj_flt;
    long unsigned int cmin_flt;
    long unsigned int cmaj_flt;
    long unsigned int inblock;
    long unsigned int oublock;
    long unsigned int cinblock;
    long unsigned int coublock;
    long unsigned int maxrss;
    long unsigned int cmaxrss;
    struct task_io_accounting ioac;
    long long unsigned int sum_sched_runtime;
    struct rlimit rlim[16];
    struct pacct_struct pacct;
    struct taskstats *stats;
    unsigned int audit_tty;
    struct tty_audit_buf *tty_audit_buf;
    bool oom_flag_origin;
    short int oom_score_adj;
    short int oom_score_adj_min;
    struct mm_struct *oom_mm;
    struct mutex cred_guard_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct signal_struct {
    refcount_t sigcnt;
    atomic_t live;
    int nr_threads;
    struct list_head thread_head;
    wait_queue_head_t wait_chldexit;
    struct task_struct *curr_target;
    struct sigpending shared_pending;
    struct hlist_head multiprocess;
    int group_exit_code;
    int notify_count;
    struct task_struct *group_exit_task;
    int group_stop_count;
    unsigned int flags;
    unsigned int is_child_subreaper;
    unsigned int has_child_subreaper;
    int posix_timer_id;
    struct list_head posix_timers;
    struct hrtimer real_timer;
    ktime_t it_real_incr;
    struct cpu_itimer it[2];
    struct thread_group_cputimer cputimer;
    struct posix_cputimers posix_cputimers;
    struct pid * pids[4];
    struct pid *tty_old_pgrp;
    int leader;
    struct tty_struct *tty;
    struct autogroup *autogroup;
    seqlock_t stats_lock;
    u64 utime;
    u64 stime;
    u64 cutime;
    u64 cstime;
    u64 gtime;
    u64 cgtime;
    struct prev_cputime prev_cputime;
    long unsigned int nvcsw;
    long unsigned int nivcsw;
    long unsigned int cnvcsw;
    long unsigned int cnivcsw;
    long unsigned int min_flt;
    long unsigned int maj_flt;
    long unsigned int cmin_flt;
    long unsigned int cmaj_flt;
    long unsigned int inblock;
    long unsigned int oublock;
    long unsigned int cinblock;
    long unsigned int coublock;
    long unsigned int maxrss;
    long unsigned int cmaxrss;
    struct task_io_accounting ioac;
    long long unsigned int sum_sched_runtime;
    struct rlimit rlim[16];
    struct pacct_struct pacct;
    struct taskstats *stats;
    unsigned int audit_tty;
    struct tty_audit_buf *tty_audit_buf;
    bool oom_flag_origin;
    short int oom_score_adj;
    short int oom_score_adj_min;
    struct mm_struct *oom_mm;
    struct mutex cred_guard_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct signal_struct {
    refcount_t sigcnt;
    atomic_t live;
    int nr_threads;
    struct list_head thread_head;
    wait_queue_head_t wait_chldexit;
    struct task_struct *curr_target;
    struct sigpending shared_pending;
    struct hlist_head multiprocess;
    int group_exit_code;
    int notify_count;
    struct task_struct *group_exit_task;
    int group_stop_count;
    unsigned int flags;
    unsigned int is_child_subreaper;
    unsigned int has_child_subreaper;
    int posix_timer_id;
    struct list_head posix_timers;
    struct hrtimer real_timer;
    ktime_t it_real_incr;
    struct cpu_itimer it[2];
    struct thread_group_cputimer cputimer;
    struct posix_cputimers posix_cputimers;
    struct pid * pids[4];
    struct pid *tty_old_pgrp;
    int leader;
    struct tty_struct *tty;
    struct autogroup *autogroup;
    seqlock_t stats_lock;
    u64 utime;
    u64 stime;
    u64 cutime;
    u64 cstime;
    u64 gtime;
    u64 cgtime;
    struct prev_cputime prev_cputime;
    long unsigned int nvcsw;
    long unsigned int nivcsw;
    long unsigned int cnvcsw;
    long unsigned int cnivcsw;
    long unsigned int min_flt;
    long unsigned int maj_flt;
    long unsigned int cmin_flt;
    long unsigned int cmaj_flt;
    long unsigned int inblock;
    long unsigned int oublock;
    long unsigned int cinblock;
    long unsigned int coublock;
    long unsigned int maxrss;
    long unsigned int cmaxrss;
    struct task_io_accounting ioac;
    long long unsigned int sum_sched_runtime;
    struct rlimit rlim[16];
    struct pacct_struct pacct;
    struct taskstats *stats;
    unsigned int audit_tty;
    struct tty_audit_buf *tty_audit_buf;
    bool oom_flag_origin;
    short int oom_score_adj;
    short int oom_score_adj_min;
    struct mm_struct *oom_mm;
    struct mutex cred_guard_mutex;
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
struct signal_struct {
    refcount_t sigcnt;
    atomic_t live;
    int nr_threads;
    struct list_head thread_head;
    wait_queue_head_t wait_chldexit;
    struct task_struct *curr_target;
    struct sigpending shared_pending;
    struct hlist_head multiprocess;
    int group_exit_code;
    int notify_count;
    struct task_struct *group_exit_task;
    int group_stop_count;
    unsigned int flags;
    unsigned int is_child_subreaper;
    unsigned int has_child_subreaper;
    int posix_timer_id;
    struct list_head posix_timers;
    struct hrtimer real_timer;
    ktime_t it_real_incr;
    struct cpu_itimer it[2];
    struct thread_group_cputimer cputimer;
    struct posix_cputimers posix_cputimers;
    struct pid * pids[4];
    struct pid *tty_old_pgrp;
    int leader;
    struct tty_struct *tty;
    struct autogroup *autogroup;
    seqlock_t stats_lock;
    u64 utime;
    u64 stime;
    u64 cutime;
    u64 cstime;
    u64 gtime;
    u64 cgtime;
    struct prev_cputime prev_cputime;
    long unsigned int nvcsw;
    long unsigned int nivcsw;
    long unsigned int cnvcsw;
    long unsigned int cnivcsw;
    long unsigned int min_flt;
    long unsigned int maj_flt;
    long unsigned int cmin_flt;
    long unsigned int cmaj_flt;
    long unsigned int inblock;
    long unsigned int oublock;
    long unsigned int cinblock;
    long unsigned int coublock;
    long unsigned int maxrss;
    long unsigned int cmaxrss;
    struct task_io_accounting ioac;
    long long unsigned int sum_sched_runtime;
    struct rlimit rlim[16];
    struct pacct_struct pacct;
    struct taskstats *stats;
    unsigned int audit_tty;
    struct tty_audit_buf *tty_audit_buf;
    bool oom_flag_origin;
    short int oom_score_adj;
    short int oom_score_adj_min;
    struct mm_struct *oom_mm;
    struct mutex cred_guard_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct signal_struct {
    refcount_t sigcnt;
    atomic_t live;
    int nr_threads;
    struct list_head thread_head;
    wait_queue_head_t wait_chldexit;
    struct task_struct *curr_target;
    struct sigpending shared_pending;
    struct hlist_head multiprocess;
    int group_exit_code;
    int notify_count;
    struct task_struct *group_exit_task;
    int group_stop_count;
    unsigned int flags;
    unsigned int is_child_subreaper;
    unsigned int has_child_subreaper;
    int posix_timer_id;
    struct list_head posix_timers;
    struct hrtimer real_timer;
    ktime_t it_real_incr;
    struct cpu_itimer it[2];
    struct thread_group_cputimer cputimer;
    struct posix_cputimers posix_cputimers;
    struct pid * pids[4];
    atomic_t tick_dep_mask;
    struct pid *tty_old_pgrp;
    int leader;
    struct tty_struct *tty;
    struct autogroup *autogroup;
    seqlock_t stats_lock;
    u64 utime;
    u64 stime;
    u64 cutime;
    u64 cstime;
    u64 gtime;
    u64 cgtime;
    struct prev_cputime prev_cputime;
    long unsigned int nvcsw;
    long unsigned int nivcsw;
    long unsigned int cnvcsw;
    long unsigned int cnivcsw;
    long unsigned int min_flt;
    long unsigned int maj_flt;
    long unsigned int cmin_flt;
    long unsigned int cmaj_flt;
    long unsigned int inblock;
    long unsigned int oublock;
    long unsigned int cinblock;
    long unsigned int coublock;
    long unsigned int maxrss;
    long unsigned int cmaxrss;
    struct task_io_accounting ioac;
    long long unsigned int sum_sched_runtime;
    struct rlimit rlim[16];
    struct pacct_struct pacct;
    struct taskstats *stats;
    unsigned int audit_tty;
    struct tty_audit_buf *tty_audit_buf;
    bool oom_flag_origin;
    short int oom_score_adj;
    short int oom_score_adj_min;
    struct mm_struct *oom_mm;
    struct mutex cred_guard_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct signal_struct {
    refcount_t sigcnt;
    atomic_t live;
    int nr_threads;
    struct list_head thread_head;
    wait_queue_head_t wait_chldexit;
    struct task_struct *curr_target;
    struct sigpending shared_pending;
    struct hlist_head multiprocess;
    int group_exit_code;
    int notify_count;
    struct task_struct *group_exit_task;
    int group_stop_count;
    unsigned int flags;
    unsigned int is_child_subreaper;
    unsigned int has_child_subreaper;
    int posix_timer_id;
    struct list_head posix_timers;
    struct hrtimer real_timer;
    ktime_t it_real_incr;
    struct cpu_itimer it[2];
    struct thread_group_cputimer cputimer;
    struct posix_cputimers posix_cputimers;
    struct pid * pids[4];
    struct pid *tty_old_pgrp;
    int leader;
    struct tty_struct *tty;
    struct autogroup *autogroup;
    seqlock_t stats_lock;
    u64 utime;
    u64 stime;
    u64 cutime;
    u64 cstime;
    u64 gtime;
    u64 cgtime;
    struct prev_cputime prev_cputime;
    long unsigned int nvcsw;
    long unsigned int nivcsw;
    long unsigned int cnvcsw;
    long unsigned int cnivcsw;
    long unsigned int min_flt;
    long unsigned int maj_flt;
    long unsigned int cmin_flt;
    long unsigned int cmaj_flt;
    long unsigned int inblock;
    long unsigned int oublock;
    long unsigned int cinblock;
    long unsigned int coublock;
    long unsigned int maxrss;
    long unsigned int cmaxrss;
    struct task_io_accounting ioac;
    long long unsigned int sum_sched_runtime;
    struct rlimit rlim[16];
    struct pacct_struct pacct;
    struct taskstats *stats;
    unsigned int audit_tty;
    struct tty_audit_buf *tty_audit_buf;
    bool oom_flag_origin;
    short int oom_score_adj;
    short int oom_score_adj_min;
    struct mm_struct *oom_mm;
    struct mutex cred_guard_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct signal_struct {
    refcount_t sigcnt;
    atomic_t live;
    int nr_threads;
    struct list_head thread_head;
    wait_queue_head_t wait_chldexit;
    struct task_struct *curr_target;
    struct sigpending shared_pending;
    struct hlist_head multiprocess;
    int group_exit_code;
    int notify_count;
    struct task_struct *group_exit_task;
    int group_stop_count;
    unsigned int flags;
    unsigned int is_child_subreaper;
    unsigned int has_child_subreaper;
    int posix_timer_id;
    struct list_head posix_timers;
    struct hrtimer real_timer;
    ktime_t it_real_incr;
    struct cpu_itimer it[2];
    struct thread_group_cputimer cputimer;
    struct posix_cputimers posix_cputimers;
    struct pid * pids[4];
    struct pid *tty_old_pgrp;
    int leader;
    struct tty_struct *tty;
    struct autogroup *autogroup;
    seqlock_t stats_lock;
    u64 utime;
    u64 stime;
    u64 cutime;
    u64 cstime;
    u64 gtime;
    u64 cgtime;
    struct prev_cputime prev_cputime;
    long unsigned int nvcsw;
    long unsigned int nivcsw;
    long unsigned int cnvcsw;
    long unsigned int cnivcsw;
    long unsigned int min_flt;
    long unsigned int maj_flt;
    long unsigned int cmin_flt;
    long unsigned int cmaj_flt;
    long unsigned int inblock;
    long unsigned int oublock;
    long unsigned int cinblock;
    long unsigned int coublock;
    long unsigned int maxrss;
    long unsigned int cmaxrss;
    struct task_io_accounting ioac;
    long long unsigned int sum_sched_runtime;
    struct rlimit rlim[16];
    struct pacct_struct pacct;
    struct taskstats *stats;
    unsigned int audit_tty;
    struct tty_audit_buf *tty_audit_buf;
    bool oom_flag_origin;
    short int oom_score_adj;
    short int oom_score_adj_min;
    struct mm_struct *oom_mm;
    struct mutex cred_guard_mutex;
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
<code>atomic_t oom_victims</code>
</li>
<li>
<b>Field added. </b>
<code>bool oom_flag_origin</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int audit_tty_log_passwd</code>
</li>
<li>
<b>Field removed. </b>
<code>oom_flags_t oom_flags</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct mm_struct *oom_mm</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t oom_victims</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>cputime_t utime</code> ➡️ <code>u64 utime</code>
</li>
<li>
<b>Field type changed. </b>
<code>cputime_t stime</code> ➡️ <code>u64 stime</code>
</li>
<li>
<b>Field type changed. </b>
<code>cputime_t cutime</code> ➡️ <code>u64 cutime</code>
</li>
<li>
<b>Field type changed. </b>
<code>cputime_t cstime</code> ➡️ <code>u64 cstime</code>
</li>
<li>
<b>Field type changed. </b>
<code>cputime_t gtime</code> ➡️ <code>u64 gtime</code>
</li>
<li>
<b>Field type changed. </b>
<code>cputime_t cgtime</code> ➡️ <code>u64 cgtime</code>
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
<b>Field added. </b>
<code>struct hlist_head multiprocess</code>
</li>
<li>
<b>Field added. </b>
<code>struct pid * pids[4]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct pid *leader_pid</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>atomic_t sigcnt</code> ➡️ <code>refcount_t sigcnt</code>
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
<code>struct posix_cputimers posix_cputimers</code>
</li>
<li>
<b>Field removed. </b>
<code>struct task_cputime cputime_expires</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head cpu_timers[3]</code>
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
<code>struct mutex exec_update_mutex</code>
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
<code>struct rw_semaphore exec_update_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mutex exec_update_mutex</code>
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
<code>struct task_struct *group_exec_task</code>
</li>
<li>
<b>Field added. </b>
<code>struct core_state *core_state</code>
</li>
<li>
<b>Field removed. </b>
<code>struct task_struct *group_exit_task</code>
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
<code>int quick_threads</code>
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
<code>unsigned int next_posix_timer_id</code>
</li>
<li>
<b>Field removed. </b>
<code>int posix_timer_id</code>
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
<code>atomic_t tick_dep_mask</code>
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
<code>atomic_t tick_dep_mask</code>
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
