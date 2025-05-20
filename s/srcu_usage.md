# Struct: <code>srcu_usage</code>

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
In <code>5.19</code>: Absent ⚠️
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct srcu_usage {
    struct srcu_node *node;
    struct srcu_node * level[4];
    int srcu_size_state;
    struct mutex srcu_cb_mutex;
    spinlock_t lock;
    struct mutex srcu_gp_mutex;
    long unsigned int srcu_gp_seq;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    long unsigned int srcu_gp_start;
    long unsigned int srcu_last_gp_end;
    long unsigned int srcu_size_jiffies;
    long unsigned int srcu_n_lock_retries;
    long unsigned int srcu_n_exp_nodelay;
    bool sda_is_static;
    long unsigned int srcu_barrier_seq;
    struct mutex srcu_barrier_mutex;
    struct completion srcu_barrier_completion;
    atomic_t srcu_barrier_cpu_cnt;
    long unsigned int reschedule_jiffies;
    long unsigned int reschedule_count;
    struct delayed_work work;
    struct srcu_struct *srcu_ssp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct srcu_usage {
    struct srcu_node *node;
    struct srcu_node * level[4];
    int srcu_size_state;
    struct mutex srcu_cb_mutex;
    spinlock_t lock;
    struct mutex srcu_gp_mutex;
    long unsigned int srcu_gp_seq;
    long unsigned int srcu_gp_seq_needed;
    long unsigned int srcu_gp_seq_needed_exp;
    long unsigned int srcu_gp_start;
    long unsigned int srcu_last_gp_end;
    long unsigned int srcu_size_jiffies;
    long unsigned int srcu_n_lock_retries;
    long unsigned int srcu_n_exp_nodelay;
    bool sda_is_static;
    long unsigned int srcu_barrier_seq;
    struct mutex srcu_barrier_mutex;
    struct completion srcu_barrier_completion;
    atomic_t srcu_barrier_cpu_cnt;
    long unsigned int reschedule_jiffies;
    long unsigned int reschedule_count;
    struct delayed_work work;
    struct srcu_struct *srcu_ssp;
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
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
