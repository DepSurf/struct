# Struct: <code>ioc</code>

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
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ioc {
    struct rq_qos rqos;
    bool enabled;
    struct ioc_params params;
    u32 period_us;
    u32 margin_us;
    u64 vrate_min;
    u64 vrate_max;
    spinlock_t lock;
    struct timer_list timer;
    struct list_head active_iocgs;
    struct ioc_pcpu_stat *pcpu_stat;
    enum ioc_running running;
    atomic64_t vtime_rate;
    seqcount_t period_seqcount;
    u32 period_at;
    u64 period_at_vtime;
    atomic64_t cur_period;
    int busy_level;
    u64 inuse_margin_vtime;
    bool weights_updated;
    atomic_t hweight_gen;
    u64 autop_too_fast_at;
    u64 autop_too_slow_at;
    int autop_idx;
    bool user_qos_params;
    bool user_cost_model;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ioc {
    struct rq_qos rqos;
    bool enabled;
    struct ioc_params params;
    u32 period_us;
    u32 margin_us;
    u64 vrate_min;
    u64 vrate_max;
    spinlock_t lock;
    struct timer_list timer;
    struct list_head active_iocgs;
    struct ioc_pcpu_stat *pcpu_stat;
    enum ioc_running running;
    atomic64_t vtime_rate;
    seqcount_t period_seqcount;
    u32 period_at;
    u64 period_at_vtime;
    atomic64_t cur_period;
    int busy_level;
    u64 inuse_margin_vtime;
    bool weights_updated;
    atomic_t hweight_gen;
    u64 autop_too_fast_at;
    u64 autop_too_slow_at;
    int autop_idx;
    bool user_qos_params;
    bool user_cost_model;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ioc {
    struct rq_qos rqos;
    bool enabled;
    struct ioc_params params;
    struct ioc_margins margins;
    u32 period_us;
    u32 timer_slack_ns;
    u64 vrate_min;
    u64 vrate_max;
    spinlock_t lock;
    struct timer_list timer;
    struct list_head active_iocgs;
    struct ioc_pcpu_stat *pcpu_stat;
    enum ioc_running running;
    atomic64_t vtime_rate;
    u64 vtime_base_rate;
    s64 vtime_err;
    seqcount_spinlock_t period_seqcount;
    u64 period_at;
    u64 period_at_vtime;
    atomic64_t cur_period;
    int busy_level;
    bool weights_updated;
    atomic_t hweight_gen;
    u64 dfgv_period_at;
    u64 dfgv_period_rem;
    u64 dfgv_usage_us_sum;
    u64 autop_too_fast_at;
    u64 autop_too_slow_at;
    int autop_idx;
    bool user_qos_params;
    bool user_cost_model;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ioc {
    struct rq_qos rqos;
    bool enabled;
    struct ioc_params params;
    struct ioc_margins margins;
    u32 period_us;
    u32 timer_slack_ns;
    u64 vrate_min;
    u64 vrate_max;
    spinlock_t lock;
    struct timer_list timer;
    struct list_head active_iocgs;
    struct ioc_pcpu_stat *pcpu_stat;
    enum ioc_running running;
    atomic64_t vtime_rate;
    u64 vtime_base_rate;
    s64 vtime_err;
    seqcount_spinlock_t period_seqcount;
    u64 period_at;
    u64 period_at_vtime;
    atomic64_t cur_period;
    int busy_level;
    bool weights_updated;
    atomic_t hweight_gen;
    u64 dfgv_period_at;
    u64 dfgv_period_rem;
    u64 dfgv_usage_us_sum;
    u64 autop_too_fast_at;
    u64 autop_too_slow_at;
    int autop_idx;
    bool user_qos_params;
    bool user_cost_model;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ioc {
    struct rq_qos rqos;
    bool enabled;
    struct ioc_params params;
    struct ioc_margins margins;
    u32 period_us;
    u32 timer_slack_ns;
    u64 vrate_min;
    u64 vrate_max;
    spinlock_t lock;
    struct timer_list timer;
    struct list_head active_iocgs;
    struct ioc_pcpu_stat *pcpu_stat;
    enum ioc_running running;
    atomic64_t vtime_rate;
    u64 vtime_base_rate;
    s64 vtime_err;
    seqcount_spinlock_t period_seqcount;
    u64 period_at;
    u64 period_at_vtime;
    atomic64_t cur_period;
    int busy_level;
    bool weights_updated;
    atomic_t hweight_gen;
    u64 dfgv_period_at;
    u64 dfgv_period_rem;
    u64 dfgv_usage_us_sum;
    u64 autop_too_fast_at;
    u64 autop_too_slow_at;
    int autop_idx;
    bool user_qos_params;
    bool user_cost_model;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ioc {
    struct rq_qos rqos;
    bool enabled;
    struct ioc_params params;
    struct ioc_margins margins;
    u32 period_us;
    u32 timer_slack_ns;
    u64 vrate_min;
    u64 vrate_max;
    spinlock_t lock;
    struct timer_list timer;
    struct list_head active_iocgs;
    struct ioc_pcpu_stat *pcpu_stat;
    enum ioc_running running;
    atomic64_t vtime_rate;
    u64 vtime_base_rate;
    s64 vtime_err;
    seqcount_spinlock_t period_seqcount;
    u64 period_at;
    u64 period_at_vtime;
    atomic64_t cur_period;
    int busy_level;
    bool weights_updated;
    atomic_t hweight_gen;
    u64 dfgv_period_at;
    u64 dfgv_period_rem;
    u64 dfgv_usage_us_sum;
    u64 autop_too_fast_at;
    u64 autop_too_slow_at;
    int autop_idx;
    bool user_qos_params;
    bool user_cost_model;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ioc {
    struct rq_qos rqos;
    bool enabled;
    struct ioc_params params;
    struct ioc_margins margins;
    u32 period_us;
    u32 timer_slack_ns;
    u64 vrate_min;
    u64 vrate_max;
    spinlock_t lock;
    struct timer_list timer;
    struct list_head active_iocgs;
    struct ioc_pcpu_stat *pcpu_stat;
    enum ioc_running running;
    atomic64_t vtime_rate;
    u64 vtime_base_rate;
    s64 vtime_err;
    seqcount_spinlock_t period_seqcount;
    u64 period_at;
    u64 period_at_vtime;
    atomic64_t cur_period;
    int busy_level;
    bool weights_updated;
    atomic_t hweight_gen;
    u64 dfgv_period_at;
    u64 dfgv_period_rem;
    u64 dfgv_usage_us_sum;
    u64 autop_too_fast_at;
    u64 autop_too_slow_at;
    int autop_idx;
    bool user_qos_params;
    bool user_cost_model;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ioc {
    struct rq_qos rqos;
    bool enabled;
    struct ioc_params params;
    struct ioc_margins margins;
    u32 period_us;
    u32 timer_slack_ns;
    u64 vrate_min;
    u64 vrate_max;
    spinlock_t lock;
    struct timer_list timer;
    struct list_head active_iocgs;
    struct ioc_pcpu_stat *pcpu_stat;
    enum ioc_running running;
    atomic64_t vtime_rate;
    u64 vtime_base_rate;
    s64 vtime_err;
    seqcount_spinlock_t period_seqcount;
    u64 period_at;
    u64 period_at_vtime;
    atomic64_t cur_period;
    int busy_level;
    bool weights_updated;
    atomic_t hweight_gen;
    u64 dfgv_period_at;
    u64 dfgv_period_rem;
    u64 dfgv_usage_us_sum;
    u64 autop_too_fast_at;
    u64 autop_too_slow_at;
    int autop_idx;
    bool user_qos_params;
    bool user_cost_model;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ioc {
    struct rq_qos rqos;
    bool enabled;
    struct ioc_params params;
    struct ioc_margins margins;
    u32 period_us;
    u32 timer_slack_ns;
    u64 vrate_min;
    u64 vrate_max;
    spinlock_t lock;
    struct timer_list timer;
    struct list_head active_iocgs;
    struct ioc_pcpu_stat *pcpu_stat;
    enum ioc_running running;
    atomic64_t vtime_rate;
    u64 vtime_base_rate;
    s64 vtime_err;
    seqcount_spinlock_t period_seqcount;
    u64 period_at;
    u64 period_at_vtime;
    atomic64_t cur_period;
    int busy_level;
    bool weights_updated;
    atomic_t hweight_gen;
    u64 dfgv_period_at;
    u64 dfgv_period_rem;
    u64 dfgv_usage_us_sum;
    u64 autop_too_fast_at;
    u64 autop_too_slow_at;
    int autop_idx;
    bool user_qos_params;
    bool user_cost_model;
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
struct ioc {
    struct rq_qos rqos;
    bool enabled;
    struct ioc_params params;
    u32 period_us;
    u32 margin_us;
    u64 vrate_min;
    u64 vrate_max;
    spinlock_t lock;
    struct timer_list timer;
    struct list_head active_iocgs;
    struct ioc_pcpu_stat *pcpu_stat;
    enum ioc_running running;
    atomic64_t vtime_rate;
    seqcount_t period_seqcount;
    u32 period_at;
    u64 period_at_vtime;
    atomic64_t cur_period;
    int busy_level;
    u64 inuse_margin_vtime;
    bool weights_updated;
    atomic_t hweight_gen;
    u64 autop_too_fast_at;
    u64 autop_too_slow_at;
    int autop_idx;
    bool user_qos_params;
    bool user_cost_model;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ioc {
    struct rq_qos rqos;
    bool enabled;
    struct ioc_params params;
    u32 period_us;
    u32 margin_us;
    u64 vrate_min;
    u64 vrate_max;
    spinlock_t lock;
    struct timer_list timer;
    struct list_head active_iocgs;
    struct ioc_pcpu_stat *pcpu_stat;
    enum ioc_running running;
    atomic64_t vtime_rate;
    seqcount_t period_seqcount;
    u32 period_at;
    u64 period_at_vtime;
    atomic64_t cur_period;
    int busy_level;
    u64 inuse_margin_vtime;
    bool weights_updated;
    atomic_t hweight_gen;
    u64 autop_too_fast_at;
    u64 autop_too_slow_at;
    int autop_idx;
    bool user_qos_params;
    bool user_cost_model;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ioc {
    struct rq_qos rqos;
    bool enabled;
    struct ioc_params params;
    u32 period_us;
    u32 margin_us;
    u64 vrate_min;
    u64 vrate_max;
    spinlock_t lock;
    struct timer_list timer;
    struct list_head active_iocgs;
    struct ioc_pcpu_stat *pcpu_stat;
    enum ioc_running running;
    atomic64_t vtime_rate;
    seqcount_t period_seqcount;
    u32 period_at;
    u64 period_at_vtime;
    atomic64_t cur_period;
    int busy_level;
    u64 inuse_margin_vtime;
    bool weights_updated;
    atomic_t hweight_gen;
    u64 autop_too_fast_at;
    u64 autop_too_slow_at;
    int autop_idx;
    bool user_qos_params;
    bool user_cost_model;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ioc {
    struct rq_qos rqos;
    bool enabled;
    struct ioc_params params;
    u32 period_us;
    u32 margin_us;
    u64 vrate_min;
    u64 vrate_max;
    spinlock_t lock;
    struct timer_list timer;
    struct list_head active_iocgs;
    struct ioc_pcpu_stat *pcpu_stat;
    enum ioc_running running;
    atomic64_t vtime_rate;
    seqcount_t period_seqcount;
    u32 period_at;
    u64 period_at_vtime;
    atomic64_t cur_period;
    int busy_level;
    u64 inuse_margin_vtime;
    bool weights_updated;
    atomic_t hweight_gen;
    u64 autop_too_fast_at;
    u64 autop_too_slow_at;
    int autop_idx;
    bool user_qos_params;
    bool user_cost_model;
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
struct ioc {
    struct rq_qos rqos;
    bool enabled;
    struct ioc_params params;
    u32 period_us;
    u32 margin_us;
    u64 vrate_min;
    u64 vrate_max;
    spinlock_t lock;
    struct timer_list timer;
    struct list_head active_iocgs;
    struct ioc_pcpu_stat *pcpu_stat;
    enum ioc_running running;
    atomic64_t vtime_rate;
    seqcount_t period_seqcount;
    u32 period_at;
    u64 period_at_vtime;
    atomic64_t cur_period;
    int busy_level;
    u64 inuse_margin_vtime;
    bool weights_updated;
    atomic_t hweight_gen;
    u64 autop_too_fast_at;
    u64 autop_too_slow_at;
    int autop_idx;
    bool user_qos_params;
    bool user_cost_model;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ioc {
    struct rq_qos rqos;
    bool enabled;
    struct ioc_params params;
    u32 period_us;
    u32 margin_us;
    u64 vrate_min;
    u64 vrate_max;
    spinlock_t lock;
    struct timer_list timer;
    struct list_head active_iocgs;
    struct ioc_pcpu_stat *pcpu_stat;
    enum ioc_running running;
    atomic64_t vtime_rate;
    seqcount_t period_seqcount;
    u32 period_at;
    u64 period_at_vtime;
    atomic64_t cur_period;
    int busy_level;
    u64 inuse_margin_vtime;
    bool weights_updated;
    atomic_t hweight_gen;
    u64 autop_too_fast_at;
    u64 autop_too_slow_at;
    int autop_idx;
    bool user_qos_params;
    bool user_cost_model;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ioc {
    struct rq_qos rqos;
    bool enabled;
    struct ioc_params params;
    u32 period_us;
    u32 margin_us;
    u64 vrate_min;
    u64 vrate_max;
    spinlock_t lock;
    struct timer_list timer;
    struct list_head active_iocgs;
    struct ioc_pcpu_stat *pcpu_stat;
    enum ioc_running running;
    atomic64_t vtime_rate;
    seqcount_t period_seqcount;
    u32 period_at;
    u64 period_at_vtime;
    atomic64_t cur_period;
    int busy_level;
    u64 inuse_margin_vtime;
    bool weights_updated;
    atomic_t hweight_gen;
    u64 autop_too_fast_at;
    u64 autop_too_slow_at;
    int autop_idx;
    bool user_qos_params;
    bool user_cost_model;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ioc {
    struct rq_qos rqos;
    bool enabled;
    struct ioc_params params;
    u32 period_us;
    u32 margin_us;
    u64 vrate_min;
    u64 vrate_max;
    spinlock_t lock;
    struct timer_list timer;
    struct list_head active_iocgs;
    struct ioc_pcpu_stat *pcpu_stat;
    enum ioc_running running;
    atomic64_t vtime_rate;
    seqcount_t period_seqcount;
    u32 period_at;
    u64 period_at_vtime;
    atomic64_t cur_period;
    int busy_level;
    u64 inuse_margin_vtime;
    bool weights_updated;
    atomic_t hweight_gen;
    u64 autop_too_fast_at;
    u64 autop_too_slow_at;
    int autop_idx;
    bool user_qos_params;
    bool user_cost_model;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct ioc_margins margins</code>
</li>
<li>
<b>Field added. </b>
<code>u32 timer_slack_ns</code>
</li>
<li>
<b>Field added. </b>
<code>u64 vtime_base_rate</code>
</li>
<li>
<b>Field added. </b>
<code>s64 vtime_err</code>
</li>
<li>
<b>Field added. </b>
<code>u64 dfgv_period_at</code>
</li>
<li>
<b>Field added. </b>
<code>u64 dfgv_period_rem</code>
</li>
<li>
<b>Field added. </b>
<code>u64 dfgv_usage_us_sum</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 margin_us</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 inuse_margin_vtime</code>
</li>
<li>
<b>Field type changed. </b>
<code>seqcount_t period_seqcount</code> ➡️ <code>seqcount_spinlock_t period_seqcount</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 period_at</code> ➡️ <code>u64 period_at</code>
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
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
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
