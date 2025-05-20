# Struct: <code>srcu_struct</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct srcu_struct {
    long unsigned int completed;
    struct srcu_struct_array *per_cpu_ref;
    spinlock_t queue_lock;
    bool running;
    struct rcu_batch batch_queue;
    struct rcu_batch batch_check0;
    struct rcu_batch batch_check1;
    struct rcu_batch batch_done;
    struct delayed_work work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct srcu_struct {
    long unsigned int completed;
    struct srcu_struct_array *per_cpu_ref;
    spinlock_t queue_lock;
    bool running;
    struct rcu_batch batch_queue;
    struct rcu_batch batch_check0;
    struct rcu_batch batch_check1;
    struct rcu_batch batch_done;
    struct delayed_work work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct srcu_struct {
    long unsigned int completed;
    struct srcu_struct_array *per_cpu_ref;
    spinlock_t queue_lock;
    bool running;
    struct rcu_batch batch_queue;
    struct rcu_batch batch_check0;
    struct rcu_batch batch_check1;
    struct rcu_batch batch_done;
    struct delayed_work work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct srcu_struct {
    struct srcu_node node[521];
    struct srcu_node * level[4];
    struct mutex srcu_cb_mutex;
    raw_spinlock_t lock;
    struct mutex srcu_gp_mutex;
    unsigned int srcu_idx;
    long unsigned int srcu_gp_seq;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    long unsigned int srcu_last_gp_end;
    struct srcu_data *sda;
    long unsigned int srcu_barrier_seq;
    struct mutex srcu_barrier_mutex;
    struct completion srcu_barrier_completion;
    atomic_t srcu_barrier_cpu_cnt;
    struct delayed_work work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct srcu_struct {
    struct srcu_node node[521];
    struct srcu_node * level[4];
    struct mutex srcu_cb_mutex;
    raw_spinlock_t lock;
    struct mutex srcu_gp_mutex;
    unsigned int srcu_idx;
    long unsigned int srcu_gp_seq;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    long unsigned int srcu_last_gp_end;
    struct srcu_data *sda;
    long unsigned int srcu_barrier_seq;
    struct mutex srcu_barrier_mutex;
    struct completion srcu_barrier_completion;
    atomic_t srcu_barrier_cpu_cnt;
    struct delayed_work work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct srcu_struct {
    struct srcu_node node[521];
    struct srcu_node * level[4];
    struct mutex srcu_cb_mutex;
    spinlock_t lock;
    struct mutex srcu_gp_mutex;
    unsigned int srcu_idx;
    long unsigned int srcu_gp_seq;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    long unsigned int srcu_last_gp_end;
    struct srcu_data *sda;
    long unsigned int srcu_barrier_seq;
    struct mutex srcu_barrier_mutex;
    struct completion srcu_barrier_completion;
    atomic_t srcu_barrier_cpu_cnt;
    struct delayed_work work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct srcu_struct {
    struct srcu_node node[521];
    struct srcu_node * level[4];
    struct mutex srcu_cb_mutex;
    spinlock_t lock;
    struct mutex srcu_gp_mutex;
    unsigned int srcu_idx;
    long unsigned int srcu_gp_seq;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    long unsigned int srcu_last_gp_end;
    struct srcu_data *sda;
    long unsigned int srcu_barrier_seq;
    struct mutex srcu_barrier_mutex;
    struct completion srcu_barrier_completion;
    atomic_t srcu_barrier_cpu_cnt;
    struct delayed_work work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct srcu_struct {
    struct srcu_node node[521];
    struct srcu_node * level[4];
    struct mutex srcu_cb_mutex;
    spinlock_t lock;
    struct mutex srcu_gp_mutex;
    unsigned int srcu_idx;
    long unsigned int srcu_gp_seq;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    long unsigned int srcu_last_gp_end;
    struct srcu_data *sda;
    long unsigned int srcu_barrier_seq;
    struct mutex srcu_barrier_mutex;
    struct completion srcu_barrier_completion;
    atomic_t srcu_barrier_cpu_cnt;
    struct delayed_work work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct srcu_struct {
    struct srcu_node node[521];
    struct srcu_node * level[4];
    struct mutex srcu_cb_mutex;
    spinlock_t lock;
    struct mutex srcu_gp_mutex;
    unsigned int srcu_idx;
    long unsigned int srcu_gp_seq;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    long unsigned int srcu_last_gp_end;
    struct srcu_data *sda;
    long unsigned int srcu_barrier_seq;
    struct mutex srcu_barrier_mutex;
    struct completion srcu_barrier_completion;
    atomic_t srcu_barrier_cpu_cnt;
    struct delayed_work work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct srcu_struct {
    struct srcu_node node[521];
    struct srcu_node * level[4];
    struct mutex srcu_cb_mutex;
    spinlock_t lock;
    struct mutex srcu_gp_mutex;
    unsigned int srcu_idx;
    long unsigned int srcu_gp_seq;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    long unsigned int srcu_last_gp_end;
    struct srcu_data *sda;
    long unsigned int srcu_barrier_seq;
    struct mutex srcu_barrier_mutex;
    struct completion srcu_barrier_completion;
    atomic_t srcu_barrier_cpu_cnt;
    struct delayed_work work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct srcu_struct {
    struct srcu_node node[521];
    struct srcu_node * level[4];
    struct mutex srcu_cb_mutex;
    spinlock_t lock;
    struct mutex srcu_gp_mutex;
    unsigned int srcu_idx;
    long unsigned int srcu_gp_seq;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    long unsigned int srcu_last_gp_end;
    struct srcu_data *sda;
    long unsigned int srcu_barrier_seq;
    struct mutex srcu_barrier_mutex;
    struct completion srcu_barrier_completion;
    atomic_t srcu_barrier_cpu_cnt;
    struct delayed_work work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct srcu_struct {
    struct srcu_node node[521];
    struct srcu_node * level[4];
    struct mutex srcu_cb_mutex;
    spinlock_t lock;
    struct mutex srcu_gp_mutex;
    unsigned int srcu_idx;
    long unsigned int srcu_gp_seq;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    long unsigned int srcu_last_gp_end;
    struct srcu_data *sda;
    long unsigned int srcu_barrier_seq;
    struct mutex srcu_barrier_mutex;
    struct completion srcu_barrier_completion;
    atomic_t srcu_barrier_cpu_cnt;
    struct delayed_work work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct srcu_struct {
    struct srcu_node node[521];
    struct srcu_node * level[4];
    struct mutex srcu_cb_mutex;
    spinlock_t lock;
    struct mutex srcu_gp_mutex;
    unsigned int srcu_idx;
    long unsigned int srcu_gp_seq;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    long unsigned int srcu_last_gp_end;
    struct srcu_data *sda;
    long unsigned int srcu_barrier_seq;
    struct mutex srcu_barrier_mutex;
    struct completion srcu_barrier_completion;
    atomic_t srcu_barrier_cpu_cnt;
    struct delayed_work work;
    struct lockdep_map dep_map;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct srcu_struct {
    struct srcu_node *node;
    struct srcu_node * level[4];
    int srcu_size_state;
    struct mutex srcu_cb_mutex;
    spinlock_t lock;
    struct mutex srcu_gp_mutex;
    unsigned int srcu_idx;
    long unsigned int srcu_gp_seq;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    long unsigned int srcu_gp_start;
    long unsigned int srcu_last_gp_end;
    long unsigned int srcu_size_jiffies;
    long unsigned int srcu_n_lock_retries;
    long unsigned int srcu_n_exp_nodelay;
    struct srcu_data *sda;
    bool sda_is_static;
    long unsigned int srcu_barrier_seq;
    struct mutex srcu_barrier_mutex;
    struct completion srcu_barrier_completion;
    atomic_t srcu_barrier_cpu_cnt;
    long unsigned int reschedule_jiffies;
    long unsigned int reschedule_count;
    struct delayed_work work;
    struct lockdep_map dep_map;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct srcu_struct {
    struct srcu_node *node;
    struct srcu_node * level[4];
    int srcu_size_state;
    struct mutex srcu_cb_mutex;
    spinlock_t lock;
    struct mutex srcu_gp_mutex;
    unsigned int srcu_idx;
    long unsigned int srcu_gp_seq;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    long unsigned int srcu_gp_start;
    long unsigned int srcu_last_gp_end;
    long unsigned int srcu_size_jiffies;
    long unsigned int srcu_n_lock_retries;
    long unsigned int srcu_n_exp_nodelay;
    struct srcu_data *sda;
    bool sda_is_static;
    long unsigned int srcu_barrier_seq;
    struct mutex srcu_barrier_mutex;
    struct completion srcu_barrier_completion;
    atomic_t srcu_barrier_cpu_cnt;
    long unsigned int reschedule_jiffies;
    long unsigned int reschedule_count;
    struct delayed_work work;
    struct lockdep_map dep_map;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct srcu_struct {
    unsigned int srcu_idx;
    struct srcu_data *sda;
    struct lockdep_map dep_map;
    struct srcu_usage *srcu_sup;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct srcu_struct {
    unsigned int srcu_idx;
    struct srcu_data *sda;
    struct lockdep_map dep_map;
    struct srcu_usage *srcu_sup;
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
struct srcu_struct {
    struct srcu_node node[17];
    struct srcu_node * level[3];
    struct mutex srcu_cb_mutex;
    spinlock_t lock;
    struct mutex srcu_gp_mutex;
    unsigned int srcu_idx;
    long unsigned int srcu_gp_seq;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    long unsigned int srcu_last_gp_end;
    struct srcu_data *sda;
    long unsigned int srcu_barrier_seq;
    struct mutex srcu_barrier_mutex;
    struct completion srcu_barrier_completion;
    atomic_t srcu_barrier_cpu_cnt;
    struct delayed_work work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct srcu_struct {
    struct srcu_node node[1];
    struct srcu_node * level[2];
    struct mutex srcu_cb_mutex;
    spinlock_t lock;
    struct mutex srcu_gp_mutex;
    unsigned int srcu_idx;
    long unsigned int srcu_gp_seq;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    long unsigned int srcu_last_gp_end;
    struct srcu_data *sda;
    long unsigned int srcu_barrier_seq;
    struct mutex srcu_barrier_mutex;
    struct completion srcu_barrier_completion;
    atomic_t srcu_barrier_cpu_cnt;
    struct delayed_work work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct srcu_struct {
    struct srcu_node node[131];
    struct srcu_node * level[4];
    struct mutex srcu_cb_mutex;
    spinlock_t lock;
    struct mutex srcu_gp_mutex;
    unsigned int srcu_idx;
    long unsigned int srcu_gp_seq;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    long unsigned int srcu_last_gp_end;
    struct srcu_data *sda;
    long unsigned int srcu_barrier_seq;
    struct mutex srcu_barrier_mutex;
    struct completion srcu_barrier_completion;
    atomic_t srcu_barrier_cpu_cnt;
    struct delayed_work work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct srcu_struct {
    struct srcu_node node[1];
    struct srcu_node * level[2];
    struct mutex srcu_cb_mutex;
    spinlock_t lock;
    struct mutex srcu_gp_mutex;
    unsigned int srcu_idx;
    long unsigned int srcu_gp_seq;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    long unsigned int srcu_last_gp_end;
    struct srcu_data *sda;
    long unsigned int srcu_barrier_seq;
    struct mutex srcu_barrier_mutex;
    struct completion srcu_barrier_completion;
    atomic_t srcu_barrier_cpu_cnt;
    struct delayed_work work;
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
struct srcu_struct {
    struct srcu_node node[521];
    struct srcu_node * level[4];
    struct mutex srcu_cb_mutex;
    spinlock_t lock;
    struct mutex srcu_gp_mutex;
    unsigned int srcu_idx;
    long unsigned int srcu_gp_seq;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    long unsigned int srcu_last_gp_end;
    struct srcu_data *sda;
    long unsigned int srcu_barrier_seq;
    struct mutex srcu_barrier_mutex;
    struct completion srcu_barrier_completion;
    atomic_t srcu_barrier_cpu_cnt;
    struct delayed_work work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct srcu_struct {
    struct srcu_node node[521];
    struct srcu_node * level[4];
    struct mutex srcu_cb_mutex;
    spinlock_t lock;
    struct mutex srcu_gp_mutex;
    unsigned int srcu_idx;
    long unsigned int srcu_gp_seq;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    long unsigned int srcu_last_gp_end;
    struct srcu_data *sda;
    long unsigned int srcu_barrier_seq;
    struct mutex srcu_barrier_mutex;
    struct completion srcu_barrier_completion;
    atomic_t srcu_barrier_cpu_cnt;
    struct delayed_work work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct srcu_struct {
    struct srcu_node node[521];
    struct srcu_node * level[4];
    struct mutex srcu_cb_mutex;
    spinlock_t lock;
    struct mutex srcu_gp_mutex;
    unsigned int srcu_idx;
    long unsigned int srcu_gp_seq;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    long unsigned int srcu_last_gp_end;
    struct srcu_data *sda;
    long unsigned int srcu_barrier_seq;
    struct mutex srcu_barrier_mutex;
    struct completion srcu_barrier_completion;
    atomic_t srcu_barrier_cpu_cnt;
    struct delayed_work work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct srcu_struct {
    struct srcu_node node[521];
    struct srcu_node * level[4];
    struct mutex srcu_cb_mutex;
    spinlock_t lock;
    struct mutex srcu_gp_mutex;
    unsigned int srcu_idx;
    long unsigned int srcu_gp_seq;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    long unsigned int srcu_last_gp_end;
    struct srcu_data *sda;
    long unsigned int srcu_barrier_seq;
    struct mutex srcu_barrier_mutex;
    struct completion srcu_barrier_completion;
    atomic_t srcu_barrier_cpu_cnt;
    struct delayed_work work;
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
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct srcu_node node[521]</code>
</li>
<li>
<b>Field added. </b>
<code>struct srcu_node * level[4]</code>
</li>
<li>
<b>Field added. </b>
<code>struct mutex srcu_cb_mutex</code>
</li>
<li>
<b>Field added. </b>
<code>raw_spinlock_t lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct mutex srcu_gp_mutex</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int srcu_idx</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int srcu_gp_seq</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int srcu_gp_seq_needed</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int srcu_gp_seq_needed_exp</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int srcu_last_gp_end</code>
</li>
<li>
<b>Field added. </b>
<code>struct srcu_data *sda</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int srcu_barrier_seq</code>
</li>
<li>
<b>Field added. </b>
<code>struct mutex srcu_barrier_mutex</code>
</li>
<li>
<b>Field added. </b>
<code>struct completion srcu_barrier_completion</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t srcu_barrier_cpu_cnt</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int completed</code>
</li>
<li>
<b>Field removed. </b>
<code>struct srcu_struct_array *per_cpu_ref</code>
</li>
<li>
<b>Field removed. </b>
<code>spinlock_t queue_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>bool running</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rcu_batch batch_queue</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rcu_batch batch_check0</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rcu_batch batch_check1</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rcu_batch batch_done</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>raw_spinlock_t lock</code> ➡️ <code>spinlock_t lock</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
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
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct lockdep_map dep_map</code>
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
<code>int srcu_size_state</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int srcu_gp_start</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int srcu_size_jiffies</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int srcu_n_lock_retries</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int srcu_n_exp_nodelay</code>
</li>
<li>
<b>Field added. </b>
<code>bool sda_is_static</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int reschedule_jiffies</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int reschedule_count</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct srcu_node node[521]</code> ➡️ <code>struct srcu_node *node</code>
</li>
</ul>
</details>
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
<code>struct srcu_usage *srcu_sup</code>
</li>
<li>
<b>Field removed. </b>
<code>struct srcu_node *node</code>
</li>
<li>
<b>Field removed. </b>
<code>struct srcu_node * level[4]</code>
</li>
<li>
<b>Field removed. </b>
<code>int srcu_size_state</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mutex srcu_cb_mutex</code>
</li>
<li>
<b>Field removed. </b>
<code>spinlock_t lock</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mutex srcu_gp_mutex</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int srcu_gp_seq</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int srcu_gp_seq_needed</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int srcu_gp_seq_needed_exp</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int srcu_gp_start</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int srcu_last_gp_end</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int srcu_size_jiffies</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int srcu_n_lock_retries</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int srcu_n_exp_nodelay</code>
</li>
<li>
<b>Field removed. </b>
<code>bool sda_is_static</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int srcu_barrier_seq</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mutex srcu_barrier_mutex</code>
</li>
<li>
<b>Field removed. </b>
<code>struct completion srcu_barrier_completion</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t srcu_barrier_cpu_cnt</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int reschedule_jiffies</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int reschedule_count</code>
</li>
<li>
<b>Field removed. </b>
<code>struct delayed_work work</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>arm64</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct srcu_node node[521]</code> ➡️ <code>struct srcu_node node[17]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct srcu_node * level[4]</code> ➡️ <code>struct srcu_node * level[3]</code>
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
<code>struct srcu_node node[521]</code> ➡️ <code>struct srcu_node node[1]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct srcu_node * level[4]</code> ➡️ <code>struct srcu_node * level[2]</code>
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
<code>struct srcu_node node[521]</code> ➡️ <code>struct srcu_node node[131]</code>
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
<code>struct srcu_node node[521]</code> ➡️ <code>struct srcu_node node[1]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct srcu_node * level[4]</code> ➡️ <code>struct srcu_node * level[2]</code>
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
