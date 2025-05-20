# Struct: <code>sched_domain</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct sched_domain {
    struct sched_domain *parent;
    struct sched_domain *child;
    struct sched_group *groups;
    long unsigned int min_interval;
    long unsigned int max_interval;
    unsigned int busy_factor;
    unsigned int imbalance_pct;
    unsigned int cache_nice_tries;
    unsigned int busy_idx;
    unsigned int idle_idx;
    unsigned int newidle_idx;
    unsigned int wake_idx;
    unsigned int forkexec_idx;
    unsigned int smt_gain;
    int nohz_idle;
    int flags;
    int level;
    long unsigned int last_balance;
    unsigned int balance_interval;
    unsigned int nr_balance_failed;
    u64 max_newidle_lb_cost;
    long unsigned int next_decay_max_lb_cost;
    unsigned int lb_count[3];
    unsigned int lb_failed[3];
    unsigned int lb_balanced[3];
    unsigned int lb_imbalance[3];
    unsigned int lb_gained[3];
    unsigned int lb_hot_gained[3];
    unsigned int lb_nobusyg[3];
    unsigned int lb_nobusyq[3];
    unsigned int alb_count;
    unsigned int alb_failed;
    unsigned int alb_pushed;
    unsigned int sbe_count;
    unsigned int sbe_balanced;
    unsigned int sbe_pushed;
    unsigned int sbf_count;
    unsigned int sbf_balanced;
    unsigned int sbf_pushed;
    unsigned int ttwu_wake_remote;
    unsigned int ttwu_move_affine;
    unsigned int ttwu_move_balance;
    char *name;
    void *private;
    struct callback_head rcu;
    unsigned int span_weight;
    long unsigned int span[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct sched_domain {
    struct sched_domain *parent;
    struct sched_domain *child;
    struct sched_group *groups;
    long unsigned int min_interval;
    long unsigned int max_interval;
    unsigned int busy_factor;
    unsigned int imbalance_pct;
    unsigned int cache_nice_tries;
    unsigned int busy_idx;
    unsigned int idle_idx;
    unsigned int newidle_idx;
    unsigned int wake_idx;
    unsigned int forkexec_idx;
    unsigned int smt_gain;
    int nohz_idle;
    int flags;
    int level;
    long unsigned int last_balance;
    unsigned int balance_interval;
    unsigned int nr_balance_failed;
    u64 max_newidle_lb_cost;
    long unsigned int next_decay_max_lb_cost;
    unsigned int lb_count[3];
    unsigned int lb_failed[3];
    unsigned int lb_balanced[3];
    unsigned int lb_imbalance[3];
    unsigned int lb_gained[3];
    unsigned int lb_hot_gained[3];
    unsigned int lb_nobusyg[3];
    unsigned int lb_nobusyq[3];
    unsigned int alb_count;
    unsigned int alb_failed;
    unsigned int alb_pushed;
    unsigned int sbe_count;
    unsigned int sbe_balanced;
    unsigned int sbe_pushed;
    unsigned int sbf_count;
    unsigned int sbf_balanced;
    unsigned int sbf_pushed;
    unsigned int ttwu_wake_remote;
    unsigned int ttwu_move_affine;
    unsigned int ttwu_move_balance;
    char *name;
    void *private;
    struct callback_head rcu;
    unsigned int span_weight;
    long unsigned int span[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct sched_domain {
    struct sched_domain *parent;
    struct sched_domain *child;
    struct sched_group *groups;
    long unsigned int min_interval;
    long unsigned int max_interval;
    unsigned int busy_factor;
    unsigned int imbalance_pct;
    unsigned int cache_nice_tries;
    unsigned int busy_idx;
    unsigned int idle_idx;
    unsigned int newidle_idx;
    unsigned int wake_idx;
    unsigned int forkexec_idx;
    unsigned int smt_gain;
    int nohz_idle;
    int flags;
    int level;
    long unsigned int last_balance;
    unsigned int balance_interval;
    unsigned int nr_balance_failed;
    u64 max_newidle_lb_cost;
    long unsigned int next_decay_max_lb_cost;
    u64 avg_scan_cost;
    unsigned int lb_count[3];
    unsigned int lb_failed[3];
    unsigned int lb_balanced[3];
    unsigned int lb_imbalance[3];
    unsigned int lb_gained[3];
    unsigned int lb_hot_gained[3];
    unsigned int lb_nobusyg[3];
    unsigned int lb_nobusyq[3];
    unsigned int alb_count;
    unsigned int alb_failed;
    unsigned int alb_pushed;
    unsigned int sbe_count;
    unsigned int sbe_balanced;
    unsigned int sbe_pushed;
    unsigned int sbf_count;
    unsigned int sbf_balanced;
    unsigned int sbf_pushed;
    unsigned int ttwu_wake_remote;
    unsigned int ttwu_move_affine;
    unsigned int ttwu_move_balance;
    char *name;
    void *private;
    struct callback_head rcu;
    struct sched_domain_shared *shared;
    unsigned int span_weight;
    long unsigned int span[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct sched_domain {
    struct sched_domain *parent;
    struct sched_domain *child;
    struct sched_group *groups;
    long unsigned int min_interval;
    long unsigned int max_interval;
    unsigned int busy_factor;
    unsigned int imbalance_pct;
    unsigned int cache_nice_tries;
    unsigned int busy_idx;
    unsigned int idle_idx;
    unsigned int newidle_idx;
    unsigned int wake_idx;
    unsigned int forkexec_idx;
    unsigned int smt_gain;
    int nohz_idle;
    int flags;
    int level;
    long unsigned int last_balance;
    unsigned int balance_interval;
    unsigned int nr_balance_failed;
    u64 max_newidle_lb_cost;
    long unsigned int next_decay_max_lb_cost;
    u64 avg_scan_cost;
    unsigned int lb_count[3];
    unsigned int lb_failed[3];
    unsigned int lb_balanced[3];
    unsigned int lb_imbalance[3];
    unsigned int lb_gained[3];
    unsigned int lb_hot_gained[3];
    unsigned int lb_nobusyg[3];
    unsigned int lb_nobusyq[3];
    unsigned int alb_count;
    unsigned int alb_failed;
    unsigned int alb_pushed;
    unsigned int sbe_count;
    unsigned int sbe_balanced;
    unsigned int sbe_pushed;
    unsigned int sbf_count;
    unsigned int sbf_balanced;
    unsigned int sbf_pushed;
    unsigned int ttwu_wake_remote;
    unsigned int ttwu_move_affine;
    unsigned int ttwu_move_balance;
    char *name;
    void *private;
    struct callback_head rcu;
    struct sched_domain_shared *shared;
    unsigned int span_weight;
    long unsigned int span[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct sched_domain {
    struct sched_domain *parent;
    struct sched_domain *child;
    struct sched_group *groups;
    long unsigned int min_interval;
    long unsigned int max_interval;
    unsigned int busy_factor;
    unsigned int imbalance_pct;
    unsigned int cache_nice_tries;
    unsigned int busy_idx;
    unsigned int idle_idx;
    unsigned int newidle_idx;
    unsigned int wake_idx;
    unsigned int forkexec_idx;
    unsigned int smt_gain;
    int nohz_idle;
    int flags;
    int level;
    long unsigned int last_balance;
    unsigned int balance_interval;
    unsigned int nr_balance_failed;
    u64 max_newidle_lb_cost;
    long unsigned int next_decay_max_lb_cost;
    u64 avg_scan_cost;
    unsigned int lb_count[3];
    unsigned int lb_failed[3];
    unsigned int lb_balanced[3];
    unsigned int lb_imbalance[3];
    unsigned int lb_gained[3];
    unsigned int lb_hot_gained[3];
    unsigned int lb_nobusyg[3];
    unsigned int lb_nobusyq[3];
    unsigned int alb_count;
    unsigned int alb_failed;
    unsigned int alb_pushed;
    unsigned int sbe_count;
    unsigned int sbe_balanced;
    unsigned int sbe_pushed;
    unsigned int sbf_count;
    unsigned int sbf_balanced;
    unsigned int sbf_pushed;
    unsigned int ttwu_wake_remote;
    unsigned int ttwu_move_affine;
    unsigned int ttwu_move_balance;
    char *name;
    void *private;
    struct callback_head rcu;
    struct sched_domain_shared *shared;
    unsigned int span_weight;
    long unsigned int span[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct sched_domain {
    struct sched_domain *parent;
    struct sched_domain *child;
    struct sched_group *groups;
    long unsigned int min_interval;
    long unsigned int max_interval;
    unsigned int busy_factor;
    unsigned int imbalance_pct;
    unsigned int cache_nice_tries;
    unsigned int busy_idx;
    unsigned int idle_idx;
    unsigned int newidle_idx;
    unsigned int wake_idx;
    unsigned int forkexec_idx;
    unsigned int smt_gain;
    int nohz_idle;
    int flags;
    int level;
    long unsigned int last_balance;
    unsigned int balance_interval;
    unsigned int nr_balance_failed;
    u64 max_newidle_lb_cost;
    long unsigned int next_decay_max_lb_cost;
    u64 avg_scan_cost;
    unsigned int lb_count[3];
    unsigned int lb_failed[3];
    unsigned int lb_balanced[3];
    unsigned int lb_imbalance[3];
    unsigned int lb_gained[3];
    unsigned int lb_hot_gained[3];
    unsigned int lb_nobusyg[3];
    unsigned int lb_nobusyq[3];
    unsigned int alb_count;
    unsigned int alb_failed;
    unsigned int alb_pushed;
    unsigned int sbe_count;
    unsigned int sbe_balanced;
    unsigned int sbe_pushed;
    unsigned int sbf_count;
    unsigned int sbf_balanced;
    unsigned int sbf_pushed;
    unsigned int ttwu_wake_remote;
    unsigned int ttwu_move_affine;
    unsigned int ttwu_move_balance;
    char *name;
    void *private;
    struct callback_head rcu;
    struct sched_domain_shared *shared;
    unsigned int span_weight;
    long unsigned int span[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct sched_domain {
    struct sched_domain *parent;
    struct sched_domain *child;
    struct sched_group *groups;
    long unsigned int min_interval;
    long unsigned int max_interval;
    unsigned int busy_factor;
    unsigned int imbalance_pct;
    unsigned int cache_nice_tries;
    unsigned int busy_idx;
    unsigned int idle_idx;
    unsigned int newidle_idx;
    unsigned int wake_idx;
    unsigned int forkexec_idx;
    int nohz_idle;
    int flags;
    int level;
    long unsigned int last_balance;
    unsigned int balance_interval;
    unsigned int nr_balance_failed;
    u64 max_newidle_lb_cost;
    long unsigned int next_decay_max_lb_cost;
    u64 avg_scan_cost;
    unsigned int lb_count[3];
    unsigned int lb_failed[3];
    unsigned int lb_balanced[3];
    unsigned int lb_imbalance[3];
    unsigned int lb_gained[3];
    unsigned int lb_hot_gained[3];
    unsigned int lb_nobusyg[3];
    unsigned int lb_nobusyq[3];
    unsigned int alb_count;
    unsigned int alb_failed;
    unsigned int alb_pushed;
    unsigned int sbe_count;
    unsigned int sbe_balanced;
    unsigned int sbe_pushed;
    unsigned int sbf_count;
    unsigned int sbf_balanced;
    unsigned int sbf_pushed;
    unsigned int ttwu_wake_remote;
    unsigned int ttwu_move_affine;
    unsigned int ttwu_move_balance;
    char *name;
    void *private;
    struct callback_head rcu;
    struct sched_domain_shared *shared;
    unsigned int span_weight;
    long unsigned int span[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct sched_domain {
    struct sched_domain *parent;
    struct sched_domain *child;
    struct sched_group *groups;
    long unsigned int min_interval;
    long unsigned int max_interval;
    unsigned int busy_factor;
    unsigned int imbalance_pct;
    unsigned int cache_nice_tries;
    int nohz_idle;
    int flags;
    int level;
    long unsigned int last_balance;
    unsigned int balance_interval;
    unsigned int nr_balance_failed;
    u64 max_newidle_lb_cost;
    long unsigned int next_decay_max_lb_cost;
    u64 avg_scan_cost;
    unsigned int lb_count[3];
    unsigned int lb_failed[3];
    unsigned int lb_balanced[3];
    unsigned int lb_imbalance[3];
    unsigned int lb_gained[3];
    unsigned int lb_hot_gained[3];
    unsigned int lb_nobusyg[3];
    unsigned int lb_nobusyq[3];
    unsigned int alb_count;
    unsigned int alb_failed;
    unsigned int alb_pushed;
    unsigned int sbe_count;
    unsigned int sbe_balanced;
    unsigned int sbe_pushed;
    unsigned int sbf_count;
    unsigned int sbf_balanced;
    unsigned int sbf_pushed;
    unsigned int ttwu_wake_remote;
    unsigned int ttwu_move_affine;
    unsigned int ttwu_move_balance;
    char *name;
    void *private;
    struct callback_head rcu;
    struct sched_domain_shared *shared;
    unsigned int span_weight;
    long unsigned int span[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct sched_domain {
    struct sched_domain *parent;
    struct sched_domain *child;
    struct sched_group *groups;
    long unsigned int min_interval;
    long unsigned int max_interval;
    unsigned int busy_factor;
    unsigned int imbalance_pct;
    unsigned int cache_nice_tries;
    int nohz_idle;
    int flags;
    int level;
    long unsigned int last_balance;
    unsigned int balance_interval;
    unsigned int nr_balance_failed;
    u64 max_newidle_lb_cost;
    long unsigned int next_decay_max_lb_cost;
    u64 avg_scan_cost;
    unsigned int lb_count[3];
    unsigned int lb_failed[3];
    unsigned int lb_balanced[3];
    unsigned int lb_imbalance[3];
    unsigned int lb_gained[3];
    unsigned int lb_hot_gained[3];
    unsigned int lb_nobusyg[3];
    unsigned int lb_nobusyq[3];
    unsigned int alb_count;
    unsigned int alb_failed;
    unsigned int alb_pushed;
    unsigned int sbe_count;
    unsigned int sbe_balanced;
    unsigned int sbe_pushed;
    unsigned int sbf_count;
    unsigned int sbf_balanced;
    unsigned int sbf_pushed;
    unsigned int ttwu_wake_remote;
    unsigned int ttwu_move_affine;
    unsigned int ttwu_move_balance;
    char *name;
    void *private;
    struct callback_head rcu;
    struct sched_domain_shared *shared;
    unsigned int span_weight;
    long unsigned int span[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct sched_domain {
    struct sched_domain *parent;
    struct sched_domain *child;
    struct sched_group *groups;
    long unsigned int min_interval;
    long unsigned int max_interval;
    unsigned int busy_factor;
    unsigned int imbalance_pct;
    unsigned int cache_nice_tries;
    int nohz_idle;
    int flags;
    int level;
    long unsigned int last_balance;
    unsigned int balance_interval;
    unsigned int nr_balance_failed;
    u64 max_newidle_lb_cost;
    long unsigned int next_decay_max_lb_cost;
    u64 avg_scan_cost;
    unsigned int lb_count[3];
    unsigned int lb_failed[3];
    unsigned int lb_balanced[3];
    unsigned int lb_imbalance[3];
    unsigned int lb_gained[3];
    unsigned int lb_hot_gained[3];
    unsigned int lb_nobusyg[3];
    unsigned int lb_nobusyq[3];
    unsigned int alb_count;
    unsigned int alb_failed;
    unsigned int alb_pushed;
    unsigned int sbe_count;
    unsigned int sbe_balanced;
    unsigned int sbe_pushed;
    unsigned int sbf_count;
    unsigned int sbf_balanced;
    unsigned int sbf_pushed;
    unsigned int ttwu_wake_remote;
    unsigned int ttwu_move_affine;
    unsigned int ttwu_move_balance;
    char *name;
    void *private;
    struct callback_head rcu;
    struct sched_domain_shared *shared;
    unsigned int span_weight;
    long unsigned int span[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct sched_domain {
    struct sched_domain *parent;
    struct sched_domain *child;
    struct sched_group *groups;
    long unsigned int min_interval;
    long unsigned int max_interval;
    unsigned int busy_factor;
    unsigned int imbalance_pct;
    unsigned int cache_nice_tries;
    int nohz_idle;
    int flags;
    int level;
    long unsigned int last_balance;
    unsigned int balance_interval;
    unsigned int nr_balance_failed;
    u64 max_newidle_lb_cost;
    long unsigned int next_decay_max_lb_cost;
    u64 avg_scan_cost;
    unsigned int lb_count[3];
    unsigned int lb_failed[3];
    unsigned int lb_balanced[3];
    unsigned int lb_imbalance[3];
    unsigned int lb_gained[3];
    unsigned int lb_hot_gained[3];
    unsigned int lb_nobusyg[3];
    unsigned int lb_nobusyq[3];
    unsigned int alb_count;
    unsigned int alb_failed;
    unsigned int alb_pushed;
    unsigned int sbe_count;
    unsigned int sbe_balanced;
    unsigned int sbe_pushed;
    unsigned int sbf_count;
    unsigned int sbf_balanced;
    unsigned int sbf_pushed;
    unsigned int ttwu_wake_remote;
    unsigned int ttwu_move_affine;
    unsigned int ttwu_move_balance;
    char *name;
    void *private;
    struct callback_head rcu;
    struct sched_domain_shared *shared;
    unsigned int span_weight;
    long unsigned int span[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct sched_domain {
    struct sched_domain *parent;
    struct sched_domain *child;
    struct sched_group *groups;
    long unsigned int min_interval;
    long unsigned int max_interval;
    unsigned int busy_factor;
    unsigned int imbalance_pct;
    unsigned int cache_nice_tries;
    int nohz_idle;
    int flags;
    int level;
    long unsigned int last_balance;
    unsigned int balance_interval;
    unsigned int nr_balance_failed;
    u64 max_newidle_lb_cost;
    long unsigned int next_decay_max_lb_cost;
    u64 avg_scan_cost;
    unsigned int lb_count[3];
    unsigned int lb_failed[3];
    unsigned int lb_balanced[3];
    unsigned int lb_imbalance[3];
    unsigned int lb_gained[3];
    unsigned int lb_hot_gained[3];
    unsigned int lb_nobusyg[3];
    unsigned int lb_nobusyq[3];
    unsigned int alb_count;
    unsigned int alb_failed;
    unsigned int alb_pushed;
    unsigned int sbe_count;
    unsigned int sbe_balanced;
    unsigned int sbe_pushed;
    unsigned int sbf_count;
    unsigned int sbf_balanced;
    unsigned int sbf_pushed;
    unsigned int ttwu_wake_remote;
    unsigned int ttwu_move_affine;
    unsigned int ttwu_move_balance;
    char *name;
    void *private;
    struct callback_head rcu;
    struct sched_domain_shared *shared;
    unsigned int span_weight;
    long unsigned int span[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct sched_domain {
    struct sched_domain *parent;
    struct sched_domain *child;
    struct sched_group *groups;
    long unsigned int min_interval;
    long unsigned int max_interval;
    unsigned int busy_factor;
    unsigned int imbalance_pct;
    unsigned int cache_nice_tries;
    int nohz_idle;
    int flags;
    int level;
    long unsigned int last_balance;
    unsigned int balance_interval;
    unsigned int nr_balance_failed;
    u64 max_newidle_lb_cost;
    long unsigned int next_decay_max_lb_cost;
    u64 avg_scan_cost;
    unsigned int lb_count[3];
    unsigned int lb_failed[3];
    unsigned int lb_balanced[3];
    unsigned int lb_imbalance[3];
    unsigned int lb_gained[3];
    unsigned int lb_hot_gained[3];
    unsigned int lb_nobusyg[3];
    unsigned int lb_nobusyq[3];
    unsigned int alb_count;
    unsigned int alb_failed;
    unsigned int alb_pushed;
    unsigned int sbe_count;
    unsigned int sbe_balanced;
    unsigned int sbe_pushed;
    unsigned int sbf_count;
    unsigned int sbf_balanced;
    unsigned int sbf_pushed;
    unsigned int ttwu_wake_remote;
    unsigned int ttwu_move_affine;
    unsigned int ttwu_move_balance;
    char *name;
    void *private;
    struct callback_head rcu;
    struct sched_domain_shared *shared;
    unsigned int span_weight;
    long unsigned int span[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct sched_domain {
    struct sched_domain *parent;
    struct sched_domain *child;
    struct sched_group *groups;
    long unsigned int min_interval;
    long unsigned int max_interval;
    unsigned int busy_factor;
    unsigned int imbalance_pct;
    unsigned int cache_nice_tries;
    unsigned int imb_numa_nr;
    int nohz_idle;
    int flags;
    int level;
    long unsigned int last_balance;
    unsigned int balance_interval;
    unsigned int nr_balance_failed;
    u64 max_newidle_lb_cost;
    long unsigned int last_decay_max_lb_cost;
    u64 avg_scan_cost;
    unsigned int lb_count[3];
    unsigned int lb_failed[3];
    unsigned int lb_balanced[3];
    unsigned int lb_imbalance[3];
    unsigned int lb_gained[3];
    unsigned int lb_hot_gained[3];
    unsigned int lb_nobusyg[3];
    unsigned int lb_nobusyq[3];
    unsigned int alb_count;
    unsigned int alb_failed;
    unsigned int alb_pushed;
    unsigned int sbe_count;
    unsigned int sbe_balanced;
    unsigned int sbe_pushed;
    unsigned int sbf_count;
    unsigned int sbf_balanced;
    unsigned int sbf_pushed;
    unsigned int ttwu_wake_remote;
    unsigned int ttwu_move_affine;
    unsigned int ttwu_move_balance;
    char *name;
    void *private;
    struct callback_head rcu;
    struct sched_domain_shared *shared;
    unsigned int span_weight;
    long unsigned int span[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct sched_domain {
    struct sched_domain *parent;
    struct sched_domain *child;
    struct sched_group *groups;
    long unsigned int min_interval;
    long unsigned int max_interval;
    unsigned int busy_factor;
    unsigned int imbalance_pct;
    unsigned int cache_nice_tries;
    unsigned int imb_numa_nr;
    int nohz_idle;
    int flags;
    int level;
    long unsigned int last_balance;
    unsigned int balance_interval;
    unsigned int nr_balance_failed;
    u64 max_newidle_lb_cost;
    long unsigned int last_decay_max_lb_cost;
    u64 avg_scan_cost;
    unsigned int lb_count[3];
    unsigned int lb_failed[3];
    unsigned int lb_balanced[3];
    unsigned int lb_imbalance[3];
    unsigned int lb_gained[3];
    unsigned int lb_hot_gained[3];
    unsigned int lb_nobusyg[3];
    unsigned int lb_nobusyq[3];
    unsigned int alb_count;
    unsigned int alb_failed;
    unsigned int alb_pushed;
    unsigned int sbe_count;
    unsigned int sbe_balanced;
    unsigned int sbe_pushed;
    unsigned int sbf_count;
    unsigned int sbf_balanced;
    unsigned int sbf_pushed;
    unsigned int ttwu_wake_remote;
    unsigned int ttwu_move_affine;
    unsigned int ttwu_move_balance;
    char *name;
    void *private;
    struct callback_head rcu;
    struct sched_domain_shared *shared;
    unsigned int span_weight;
    long unsigned int span[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct sched_domain {
    struct sched_domain *parent;
    struct sched_domain *child;
    struct sched_group *groups;
    long unsigned int min_interval;
    long unsigned int max_interval;
    unsigned int busy_factor;
    unsigned int imbalance_pct;
    unsigned int cache_nice_tries;
    unsigned int imb_numa_nr;
    int nohz_idle;
    int flags;
    int level;
    long unsigned int last_balance;
    unsigned int balance_interval;
    unsigned int nr_balance_failed;
    u64 max_newidle_lb_cost;
    long unsigned int last_decay_max_lb_cost;
    u64 avg_scan_cost;
    unsigned int lb_count[3];
    unsigned int lb_failed[3];
    unsigned int lb_balanced[3];
    unsigned int lb_imbalance[3];
    unsigned int lb_gained[3];
    unsigned int lb_hot_gained[3];
    unsigned int lb_nobusyg[3];
    unsigned int lb_nobusyq[3];
    unsigned int alb_count;
    unsigned int alb_failed;
    unsigned int alb_pushed;
    unsigned int sbe_count;
    unsigned int sbe_balanced;
    unsigned int sbe_pushed;
    unsigned int sbf_count;
    unsigned int sbf_balanced;
    unsigned int sbf_pushed;
    unsigned int ttwu_wake_remote;
    unsigned int ttwu_move_affine;
    unsigned int ttwu_move_balance;
    char *name;
    void *private;
    struct callback_head rcu;
    struct sched_domain_shared *shared;
    unsigned int span_weight;
    long unsigned int span[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct sched_domain {
    struct sched_domain *parent;
    struct sched_domain *child;
    struct sched_group *groups;
    long unsigned int min_interval;
    long unsigned int max_interval;
    unsigned int busy_factor;
    unsigned int imbalance_pct;
    unsigned int cache_nice_tries;
    unsigned int imb_numa_nr;
    int nohz_idle;
    int flags;
    int level;
    long unsigned int last_balance;
    unsigned int balance_interval;
    unsigned int nr_balance_failed;
    u64 max_newidle_lb_cost;
    long unsigned int last_decay_max_lb_cost;
    unsigned int lb_count[3];
    unsigned int lb_failed[3];
    unsigned int lb_balanced[3];
    unsigned int lb_imbalance[3];
    unsigned int lb_gained[3];
    unsigned int lb_hot_gained[3];
    unsigned int lb_nobusyg[3];
    unsigned int lb_nobusyq[3];
    unsigned int alb_count;
    unsigned int alb_failed;
    unsigned int alb_pushed;
    unsigned int sbe_count;
    unsigned int sbe_balanced;
    unsigned int sbe_pushed;
    unsigned int sbf_count;
    unsigned int sbf_balanced;
    unsigned int sbf_pushed;
    unsigned int ttwu_wake_remote;
    unsigned int ttwu_move_affine;
    unsigned int ttwu_move_balance;
    char *name;
    void *private;
    struct callback_head rcu;
    struct sched_domain_shared *shared;
    unsigned int span_weight;
    long unsigned int span[0];
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
struct sched_domain {
    struct sched_domain *parent;
    struct sched_domain *child;
    struct sched_group *groups;
    long unsigned int min_interval;
    long unsigned int max_interval;
    unsigned int busy_factor;
    unsigned int imbalance_pct;
    unsigned int cache_nice_tries;
    int nohz_idle;
    int flags;
    int level;
    long unsigned int last_balance;
    unsigned int balance_interval;
    unsigned int nr_balance_failed;
    u64 max_newidle_lb_cost;
    long unsigned int next_decay_max_lb_cost;
    u64 avg_scan_cost;
    unsigned int lb_count[3];
    unsigned int lb_failed[3];
    unsigned int lb_balanced[3];
    unsigned int lb_imbalance[3];
    unsigned int lb_gained[3];
    unsigned int lb_hot_gained[3];
    unsigned int lb_nobusyg[3];
    unsigned int lb_nobusyq[3];
    unsigned int alb_count;
    unsigned int alb_failed;
    unsigned int alb_pushed;
    unsigned int sbe_count;
    unsigned int sbe_balanced;
    unsigned int sbe_pushed;
    unsigned int sbf_count;
    unsigned int sbf_balanced;
    unsigned int sbf_pushed;
    unsigned int ttwu_wake_remote;
    unsigned int ttwu_move_affine;
    unsigned int ttwu_move_balance;
    char *name;
    void *private;
    struct callback_head rcu;
    struct sched_domain_shared *shared;
    unsigned int span_weight;
    long unsigned int span[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct sched_domain {
    struct sched_domain *parent;
    struct sched_domain *child;
    struct sched_group *groups;
    long unsigned int min_interval;
    long unsigned int max_interval;
    unsigned int busy_factor;
    unsigned int imbalance_pct;
    unsigned int cache_nice_tries;
    int nohz_idle;
    int flags;
    int level;
    long unsigned int last_balance;
    unsigned int balance_interval;
    unsigned int nr_balance_failed;
    u64 max_newidle_lb_cost;
    long unsigned int next_decay_max_lb_cost;
    u64 avg_scan_cost;
    unsigned int lb_count[3];
    unsigned int lb_failed[3];
    unsigned int lb_balanced[3];
    unsigned int lb_imbalance[3];
    unsigned int lb_gained[3];
    unsigned int lb_hot_gained[3];
    unsigned int lb_nobusyg[3];
    unsigned int lb_nobusyq[3];
    unsigned int alb_count;
    unsigned int alb_failed;
    unsigned int alb_pushed;
    unsigned int sbe_count;
    unsigned int sbe_balanced;
    unsigned int sbe_pushed;
    unsigned int sbf_count;
    unsigned int sbf_balanced;
    unsigned int sbf_pushed;
    unsigned int ttwu_wake_remote;
    unsigned int ttwu_move_affine;
    unsigned int ttwu_move_balance;
    char *name;
    void *private;
    struct callback_head rcu;
    struct sched_domain_shared *shared;
    unsigned int span_weight;
    long unsigned int span[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct sched_domain {
    struct sched_domain *parent;
    struct sched_domain *child;
    struct sched_group *groups;
    long unsigned int min_interval;
    long unsigned int max_interval;
    unsigned int busy_factor;
    unsigned int imbalance_pct;
    unsigned int cache_nice_tries;
    int nohz_idle;
    int flags;
    int level;
    long unsigned int last_balance;
    unsigned int balance_interval;
    unsigned int nr_balance_failed;
    u64 max_newidle_lb_cost;
    long unsigned int next_decay_max_lb_cost;
    u64 avg_scan_cost;
    unsigned int lb_count[3];
    unsigned int lb_failed[3];
    unsigned int lb_balanced[3];
    unsigned int lb_imbalance[3];
    unsigned int lb_gained[3];
    unsigned int lb_hot_gained[3];
    unsigned int lb_nobusyg[3];
    unsigned int lb_nobusyq[3];
    unsigned int alb_count;
    unsigned int alb_failed;
    unsigned int alb_pushed;
    unsigned int sbe_count;
    unsigned int sbe_balanced;
    unsigned int sbe_pushed;
    unsigned int sbf_count;
    unsigned int sbf_balanced;
    unsigned int sbf_pushed;
    unsigned int ttwu_wake_remote;
    unsigned int ttwu_move_affine;
    unsigned int ttwu_move_balance;
    char *name;
    void *private;
    struct callback_head rcu;
    struct sched_domain_shared *shared;
    unsigned int span_weight;
    long unsigned int span[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct sched_domain {
    struct sched_domain *parent;
    struct sched_domain *child;
    struct sched_group *groups;
    long unsigned int min_interval;
    long unsigned int max_interval;
    unsigned int busy_factor;
    unsigned int imbalance_pct;
    unsigned int cache_nice_tries;
    int nohz_idle;
    int flags;
    int level;
    long unsigned int last_balance;
    unsigned int balance_interval;
    unsigned int nr_balance_failed;
    u64 max_newidle_lb_cost;
    long unsigned int next_decay_max_lb_cost;
    u64 avg_scan_cost;
    unsigned int lb_count[3];
    unsigned int lb_failed[3];
    unsigned int lb_balanced[3];
    unsigned int lb_imbalance[3];
    unsigned int lb_gained[3];
    unsigned int lb_hot_gained[3];
    unsigned int lb_nobusyg[3];
    unsigned int lb_nobusyq[3];
    unsigned int alb_count;
    unsigned int alb_failed;
    unsigned int alb_pushed;
    unsigned int sbe_count;
    unsigned int sbe_balanced;
    unsigned int sbe_pushed;
    unsigned int sbf_count;
    unsigned int sbf_balanced;
    unsigned int sbf_pushed;
    unsigned int ttwu_wake_remote;
    unsigned int ttwu_move_affine;
    unsigned int ttwu_move_balance;
    char *name;
    void *private;
    struct callback_head rcu;
    struct sched_domain_shared *shared;
    unsigned int span_weight;
    long unsigned int span[0];
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
struct sched_domain {
    struct sched_domain *parent;
    struct sched_domain *child;
    struct sched_group *groups;
    long unsigned int min_interval;
    long unsigned int max_interval;
    unsigned int busy_factor;
    unsigned int imbalance_pct;
    unsigned int cache_nice_tries;
    int nohz_idle;
    int flags;
    int level;
    long unsigned int last_balance;
    unsigned int balance_interval;
    unsigned int nr_balance_failed;
    u64 max_newidle_lb_cost;
    long unsigned int next_decay_max_lb_cost;
    u64 avg_scan_cost;
    unsigned int lb_count[3];
    unsigned int lb_failed[3];
    unsigned int lb_balanced[3];
    unsigned int lb_imbalance[3];
    unsigned int lb_gained[3];
    unsigned int lb_hot_gained[3];
    unsigned int lb_nobusyg[3];
    unsigned int lb_nobusyq[3];
    unsigned int alb_count;
    unsigned int alb_failed;
    unsigned int alb_pushed;
    unsigned int sbe_count;
    unsigned int sbe_balanced;
    unsigned int sbe_pushed;
    unsigned int sbf_count;
    unsigned int sbf_balanced;
    unsigned int sbf_pushed;
    unsigned int ttwu_wake_remote;
    unsigned int ttwu_move_affine;
    unsigned int ttwu_move_balance;
    char *name;
    void *private;
    struct callback_head rcu;
    struct sched_domain_shared *shared;
    unsigned int span_weight;
    long unsigned int span[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct sched_domain {
    struct sched_domain *parent;
    struct sched_domain *child;
    struct sched_group *groups;
    long unsigned int min_interval;
    long unsigned int max_interval;
    unsigned int busy_factor;
    unsigned int imbalance_pct;
    unsigned int cache_nice_tries;
    int nohz_idle;
    int flags;
    int level;
    long unsigned int last_balance;
    unsigned int balance_interval;
    unsigned int nr_balance_failed;
    u64 max_newidle_lb_cost;
    long unsigned int next_decay_max_lb_cost;
    u64 avg_scan_cost;
    unsigned int lb_count[3];
    unsigned int lb_failed[3];
    unsigned int lb_balanced[3];
    unsigned int lb_imbalance[3];
    unsigned int lb_gained[3];
    unsigned int lb_hot_gained[3];
    unsigned int lb_nobusyg[3];
    unsigned int lb_nobusyq[3];
    unsigned int alb_count;
    unsigned int alb_failed;
    unsigned int alb_pushed;
    unsigned int sbe_count;
    unsigned int sbe_balanced;
    unsigned int sbe_pushed;
    unsigned int sbf_count;
    unsigned int sbf_balanced;
    unsigned int sbf_pushed;
    unsigned int ttwu_wake_remote;
    unsigned int ttwu_move_affine;
    unsigned int ttwu_move_balance;
    char *name;
    void *private;
    struct callback_head rcu;
    struct sched_domain_shared *shared;
    unsigned int span_weight;
    long unsigned int span[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct sched_domain {
    struct sched_domain *parent;
    struct sched_domain *child;
    struct sched_group *groups;
    long unsigned int min_interval;
    long unsigned int max_interval;
    unsigned int busy_factor;
    unsigned int imbalance_pct;
    unsigned int cache_nice_tries;
    int nohz_idle;
    int flags;
    int level;
    long unsigned int last_balance;
    unsigned int balance_interval;
    unsigned int nr_balance_failed;
    u64 max_newidle_lb_cost;
    long unsigned int next_decay_max_lb_cost;
    u64 avg_scan_cost;
    unsigned int lb_count[3];
    unsigned int lb_failed[3];
    unsigned int lb_balanced[3];
    unsigned int lb_imbalance[3];
    unsigned int lb_gained[3];
    unsigned int lb_hot_gained[3];
    unsigned int lb_nobusyg[3];
    unsigned int lb_nobusyq[3];
    unsigned int alb_count;
    unsigned int alb_failed;
    unsigned int alb_pushed;
    unsigned int sbe_count;
    unsigned int sbe_balanced;
    unsigned int sbe_pushed;
    unsigned int sbf_count;
    unsigned int sbf_balanced;
    unsigned int sbf_pushed;
    unsigned int ttwu_wake_remote;
    unsigned int ttwu_move_affine;
    unsigned int ttwu_move_balance;
    char *name;
    void *private;
    struct callback_head rcu;
    struct sched_domain_shared *shared;
    unsigned int span_weight;
    long unsigned int span[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct sched_domain {
    struct sched_domain *parent;
    struct sched_domain *child;
    struct sched_group *groups;
    long unsigned int min_interval;
    long unsigned int max_interval;
    unsigned int busy_factor;
    unsigned int imbalance_pct;
    unsigned int cache_nice_tries;
    int nohz_idle;
    int flags;
    int level;
    long unsigned int last_balance;
    unsigned int balance_interval;
    unsigned int nr_balance_failed;
    u64 max_newidle_lb_cost;
    long unsigned int next_decay_max_lb_cost;
    u64 avg_scan_cost;
    unsigned int lb_count[3];
    unsigned int lb_failed[3];
    unsigned int lb_balanced[3];
    unsigned int lb_imbalance[3];
    unsigned int lb_gained[3];
    unsigned int lb_hot_gained[3];
    unsigned int lb_nobusyg[3];
    unsigned int lb_nobusyq[3];
    unsigned int alb_count;
    unsigned int alb_failed;
    unsigned int alb_pushed;
    unsigned int sbe_count;
    unsigned int sbe_balanced;
    unsigned int sbe_pushed;
    unsigned int sbf_count;
    unsigned int sbf_balanced;
    unsigned int sbf_pushed;
    unsigned int ttwu_wake_remote;
    unsigned int ttwu_move_affine;
    unsigned int ttwu_move_balance;
    char *name;
    void *private;
    struct callback_head rcu;
    struct sched_domain_shared *shared;
    unsigned int span_weight;
    long unsigned int span[0];
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
<code>u64 avg_scan_cost</code>
</li>
<li>
<b>Field added. </b>
<code>struct sched_domain_shared *shared</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
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
<b>Field removed. </b>
<code>unsigned int smt_gain</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned int busy_idx</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int idle_idx</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int newidle_idx</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int wake_idx</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int forkexec_idx</code>
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
No changes between <code>5.8</code> and <code>5.11</code> ✅
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
<code>unsigned int imb_numa_nr</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int last_decay_max_lb_cost</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int next_decay_max_lb_cost</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>u64 avg_scan_cost</code>
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
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
