# Struct: <code>cpufreq_policy</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct cpufreq_policy {
    cpumask_var_t cpus;
    cpumask_var_t related_cpus;
    cpumask_var_t real_cpus;
    unsigned int shared_type;
    unsigned int cpu;
    struct clk *clk;
    struct cpufreq_cpuinfo cpuinfo;
    unsigned int min;
    unsigned int max;
    unsigned int cur;
    unsigned int restore_freq;
    unsigned int suspend_freq;
    unsigned int policy;
    unsigned int last_policy;
    struct cpufreq_governor *governor;
    void *governor_data;
    bool governor_enabled;
    char last_governor[16];
    struct work_struct update;
    struct cpufreq_user_policy user_policy;
    struct cpufreq_frequency_table *freq_table;
    struct list_head policy_list;
    struct kobject kobj;
    struct completion kobj_unregister;
    struct rw_semaphore rwsem;
    bool transition_ongoing;
    spinlock_t transition_lock;
    wait_queue_head_t transition_wait;
    struct task_struct *transition_task;
    struct cpufreq_stats *stats;
    void *driver_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct cpufreq_policy {
    cpumask_var_t cpus;
    cpumask_var_t related_cpus;
    cpumask_var_t real_cpus;
    unsigned int shared_type;
    unsigned int cpu;
    struct clk *clk;
    struct cpufreq_cpuinfo cpuinfo;
    unsigned int min;
    unsigned int max;
    unsigned int cur;
    unsigned int restore_freq;
    unsigned int suspend_freq;
    unsigned int policy;
    unsigned int last_policy;
    struct cpufreq_governor *governor;
    void *governor_data;
    char last_governor[16];
    struct work_struct update;
    struct cpufreq_user_policy user_policy;
    struct cpufreq_frequency_table *freq_table;
    enum cpufreq_table_sorting freq_table_sorted;
    struct list_head policy_list;
    struct kobject kobj;
    struct completion kobj_unregister;
    struct rw_semaphore rwsem;
    bool fast_switch_possible;
    bool fast_switch_enabled;
    unsigned int cached_target_freq;
    int cached_resolved_idx;
    bool transition_ongoing;
    spinlock_t transition_lock;
    wait_queue_head_t transition_wait;
    struct task_struct *transition_task;
    struct cpufreq_stats *stats;
    void *driver_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct cpufreq_policy {
    cpumask_var_t cpus;
    cpumask_var_t related_cpus;
    cpumask_var_t real_cpus;
    unsigned int shared_type;
    unsigned int cpu;
    struct clk *clk;
    struct cpufreq_cpuinfo cpuinfo;
    unsigned int min;
    unsigned int max;
    unsigned int cur;
    unsigned int restore_freq;
    unsigned int suspend_freq;
    unsigned int policy;
    unsigned int last_policy;
    struct cpufreq_governor *governor;
    void *governor_data;
    char last_governor[16];
    struct work_struct update;
    struct cpufreq_user_policy user_policy;
    struct cpufreq_frequency_table *freq_table;
    enum cpufreq_table_sorting freq_table_sorted;
    struct list_head policy_list;
    struct kobject kobj;
    struct completion kobj_unregister;
    struct rw_semaphore rwsem;
    bool fast_switch_possible;
    bool fast_switch_enabled;
    unsigned int cached_target_freq;
    int cached_resolved_idx;
    bool transition_ongoing;
    spinlock_t transition_lock;
    wait_queue_head_t transition_wait;
    struct task_struct *transition_task;
    struct cpufreq_stats *stats;
    void *driver_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct cpufreq_policy {
    cpumask_var_t cpus;
    cpumask_var_t related_cpus;
    cpumask_var_t real_cpus;
    unsigned int shared_type;
    unsigned int cpu;
    struct clk *clk;
    struct cpufreq_cpuinfo cpuinfo;
    unsigned int min;
    unsigned int max;
    unsigned int cur;
    unsigned int restore_freq;
    unsigned int suspend_freq;
    unsigned int policy;
    unsigned int last_policy;
    struct cpufreq_governor *governor;
    void *governor_data;
    char last_governor[16];
    struct work_struct update;
    struct cpufreq_user_policy user_policy;
    struct cpufreq_frequency_table *freq_table;
    enum cpufreq_table_sorting freq_table_sorted;
    struct list_head policy_list;
    struct kobject kobj;
    struct completion kobj_unregister;
    struct rw_semaphore rwsem;
    bool fast_switch_possible;
    bool fast_switch_enabled;
    unsigned int transition_delay_us;
    unsigned int cached_target_freq;
    int cached_resolved_idx;
    bool transition_ongoing;
    spinlock_t transition_lock;
    wait_queue_head_t transition_wait;
    struct task_struct *transition_task;
    struct cpufreq_stats *stats;
    void *driver_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct cpufreq_policy {
    cpumask_var_t cpus;
    cpumask_var_t related_cpus;
    cpumask_var_t real_cpus;
    unsigned int shared_type;
    unsigned int cpu;
    struct clk *clk;
    struct cpufreq_cpuinfo cpuinfo;
    unsigned int min;
    unsigned int max;
    unsigned int cur;
    unsigned int restore_freq;
    unsigned int suspend_freq;
    unsigned int policy;
    unsigned int last_policy;
    struct cpufreq_governor *governor;
    void *governor_data;
    char last_governor[16];
    struct work_struct update;
    struct cpufreq_user_policy user_policy;
    struct cpufreq_frequency_table *freq_table;
    enum cpufreq_table_sorting freq_table_sorted;
    struct list_head policy_list;
    struct kobject kobj;
    struct completion kobj_unregister;
    struct rw_semaphore rwsem;
    bool fast_switch_possible;
    bool fast_switch_enabled;
    unsigned int transition_delay_us;
    bool dvfs_possible_from_any_cpu;
    unsigned int cached_target_freq;
    int cached_resolved_idx;
    bool transition_ongoing;
    spinlock_t transition_lock;
    wait_queue_head_t transition_wait;
    struct task_struct *transition_task;
    struct cpufreq_stats *stats;
    void *driver_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct cpufreq_policy {
    cpumask_var_t cpus;
    cpumask_var_t related_cpus;
    cpumask_var_t real_cpus;
    unsigned int shared_type;
    unsigned int cpu;
    struct clk *clk;
    struct cpufreq_cpuinfo cpuinfo;
    unsigned int min;
    unsigned int max;
    unsigned int cur;
    unsigned int restore_freq;
    unsigned int suspend_freq;
    unsigned int policy;
    unsigned int last_policy;
    struct cpufreq_governor *governor;
    void *governor_data;
    char last_governor[16];
    struct work_struct update;
    struct cpufreq_user_policy user_policy;
    struct cpufreq_frequency_table *freq_table;
    enum cpufreq_table_sorting freq_table_sorted;
    struct list_head policy_list;
    struct kobject kobj;
    struct completion kobj_unregister;
    struct rw_semaphore rwsem;
    bool fast_switch_possible;
    bool fast_switch_enabled;
    unsigned int transition_delay_us;
    bool dvfs_possible_from_any_cpu;
    unsigned int cached_target_freq;
    int cached_resolved_idx;
    bool transition_ongoing;
    spinlock_t transition_lock;
    wait_queue_head_t transition_wait;
    struct task_struct *transition_task;
    struct cpufreq_stats *stats;
    void *driver_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct cpufreq_policy {
    cpumask_var_t cpus;
    cpumask_var_t related_cpus;
    cpumask_var_t real_cpus;
    unsigned int shared_type;
    unsigned int cpu;
    struct clk *clk;
    struct cpufreq_cpuinfo cpuinfo;
    unsigned int min;
    unsigned int max;
    unsigned int cur;
    unsigned int restore_freq;
    unsigned int suspend_freq;
    unsigned int policy;
    unsigned int last_policy;
    struct cpufreq_governor *governor;
    void *governor_data;
    char last_governor[16];
    struct work_struct update;
    struct cpufreq_user_policy user_policy;
    struct cpufreq_frequency_table *freq_table;
    enum cpufreq_table_sorting freq_table_sorted;
    struct list_head policy_list;
    struct kobject kobj;
    struct completion kobj_unregister;
    struct rw_semaphore rwsem;
    bool fast_switch_possible;
    bool fast_switch_enabled;
    unsigned int transition_delay_us;
    bool dvfs_possible_from_any_cpu;
    unsigned int cached_target_freq;
    int cached_resolved_idx;
    bool transition_ongoing;
    spinlock_t transition_lock;
    wait_queue_head_t transition_wait;
    struct task_struct *transition_task;
    struct cpufreq_stats *stats;
    void *driver_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct cpufreq_policy {
    cpumask_var_t cpus;
    cpumask_var_t related_cpus;
    cpumask_var_t real_cpus;
    unsigned int shared_type;
    unsigned int cpu;
    struct clk *clk;
    struct cpufreq_cpuinfo cpuinfo;
    unsigned int min;
    unsigned int max;
    unsigned int cur;
    unsigned int restore_freq;
    unsigned int suspend_freq;
    unsigned int policy;
    unsigned int last_policy;
    struct cpufreq_governor *governor;
    void *governor_data;
    char last_governor[16];
    struct work_struct update;
    struct dev_pm_qos_request *min_freq_req;
    struct dev_pm_qos_request *max_freq_req;
    struct cpufreq_frequency_table *freq_table;
    enum cpufreq_table_sorting freq_table_sorted;
    struct list_head policy_list;
    struct kobject kobj;
    struct completion kobj_unregister;
    struct rw_semaphore rwsem;
    bool fast_switch_possible;
    bool fast_switch_enabled;
    unsigned int transition_delay_us;
    bool dvfs_possible_from_any_cpu;
    unsigned int cached_target_freq;
    int cached_resolved_idx;
    bool transition_ongoing;
    spinlock_t transition_lock;
    wait_queue_head_t transition_wait;
    struct task_struct *transition_task;
    struct cpufreq_stats *stats;
    void *driver_data;
    struct thermal_cooling_device *cdev;
    struct notifier_block nb_min;
    struct notifier_block nb_max;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct cpufreq_policy {
    cpumask_var_t cpus;
    cpumask_var_t related_cpus;
    cpumask_var_t real_cpus;
    unsigned int shared_type;
    unsigned int cpu;
    struct clk *clk;
    struct cpufreq_cpuinfo cpuinfo;
    unsigned int min;
    unsigned int max;
    unsigned int cur;
    unsigned int restore_freq;
    unsigned int suspend_freq;
    unsigned int policy;
    unsigned int last_policy;
    struct cpufreq_governor *governor;
    void *governor_data;
    char last_governor[16];
    struct work_struct update;
    struct freq_constraints constraints;
    struct freq_qos_request *min_freq_req;
    struct freq_qos_request *max_freq_req;
    struct cpufreq_frequency_table *freq_table;
    enum cpufreq_table_sorting freq_table_sorted;
    struct list_head policy_list;
    struct kobject kobj;
    struct completion kobj_unregister;
    struct rw_semaphore rwsem;
    bool fast_switch_possible;
    bool fast_switch_enabled;
    unsigned int transition_delay_us;
    bool dvfs_possible_from_any_cpu;
    unsigned int cached_target_freq;
    int cached_resolved_idx;
    bool transition_ongoing;
    spinlock_t transition_lock;
    wait_queue_head_t transition_wait;
    struct task_struct *transition_task;
    struct cpufreq_stats *stats;
    void *driver_data;
    struct thermal_cooling_device *cdev;
    struct notifier_block nb_min;
    struct notifier_block nb_max;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct cpufreq_policy {
    cpumask_var_t cpus;
    cpumask_var_t related_cpus;
    cpumask_var_t real_cpus;
    unsigned int shared_type;
    unsigned int cpu;
    struct clk *clk;
    struct cpufreq_cpuinfo cpuinfo;
    unsigned int min;
    unsigned int max;
    unsigned int cur;
    unsigned int restore_freq;
    unsigned int suspend_freq;
    unsigned int policy;
    unsigned int last_policy;
    struct cpufreq_governor *governor;
    void *governor_data;
    char last_governor[16];
    struct work_struct update;
    struct freq_constraints constraints;
    struct freq_qos_request *min_freq_req;
    struct freq_qos_request *max_freq_req;
    struct cpufreq_frequency_table *freq_table;
    enum cpufreq_table_sorting freq_table_sorted;
    struct list_head policy_list;
    struct kobject kobj;
    struct completion kobj_unregister;
    struct rw_semaphore rwsem;
    bool fast_switch_possible;
    bool fast_switch_enabled;
    unsigned int transition_delay_us;
    bool dvfs_possible_from_any_cpu;
    unsigned int cached_target_freq;
    int cached_resolved_idx;
    bool transition_ongoing;
    spinlock_t transition_lock;
    wait_queue_head_t transition_wait;
    struct task_struct *transition_task;
    struct cpufreq_stats *stats;
    void *driver_data;
    struct thermal_cooling_device *cdev;
    struct notifier_block nb_min;
    struct notifier_block nb_max;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct cpufreq_policy {
    cpumask_var_t cpus;
    cpumask_var_t related_cpus;
    cpumask_var_t real_cpus;
    unsigned int shared_type;
    unsigned int cpu;
    struct clk *clk;
    struct cpufreq_cpuinfo cpuinfo;
    unsigned int min;
    unsigned int max;
    unsigned int cur;
    unsigned int suspend_freq;
    unsigned int policy;
    unsigned int last_policy;
    struct cpufreq_governor *governor;
    void *governor_data;
    char last_governor[16];
    struct work_struct update;
    struct freq_constraints constraints;
    struct freq_qos_request *min_freq_req;
    struct freq_qos_request *max_freq_req;
    struct cpufreq_frequency_table *freq_table;
    enum cpufreq_table_sorting freq_table_sorted;
    struct list_head policy_list;
    struct kobject kobj;
    struct completion kobj_unregister;
    struct rw_semaphore rwsem;
    bool fast_switch_possible;
    bool fast_switch_enabled;
    bool strict_target;
    unsigned int transition_delay_us;
    bool dvfs_possible_from_any_cpu;
    unsigned int cached_target_freq;
    unsigned int cached_resolved_idx;
    bool transition_ongoing;
    spinlock_t transition_lock;
    wait_queue_head_t transition_wait;
    struct task_struct *transition_task;
    struct cpufreq_stats *stats;
    void *driver_data;
    struct thermal_cooling_device *cdev;
    struct notifier_block nb_min;
    struct notifier_block nb_max;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct cpufreq_policy {
    cpumask_var_t cpus;
    cpumask_var_t related_cpus;
    cpumask_var_t real_cpus;
    unsigned int shared_type;
    unsigned int cpu;
    struct clk *clk;
    struct cpufreq_cpuinfo cpuinfo;
    unsigned int min;
    unsigned int max;
    unsigned int cur;
    unsigned int suspend_freq;
    unsigned int policy;
    unsigned int last_policy;
    struct cpufreq_governor *governor;
    void *governor_data;
    char last_governor[16];
    struct work_struct update;
    struct freq_constraints constraints;
    struct freq_qos_request *min_freq_req;
    struct freq_qos_request *max_freq_req;
    struct cpufreq_frequency_table *freq_table;
    enum cpufreq_table_sorting freq_table_sorted;
    struct list_head policy_list;
    struct kobject kobj;
    struct completion kobj_unregister;
    struct rw_semaphore rwsem;
    bool fast_switch_possible;
    bool fast_switch_enabled;
    bool strict_target;
    unsigned int transition_delay_us;
    bool dvfs_possible_from_any_cpu;
    unsigned int cached_target_freq;
    unsigned int cached_resolved_idx;
    bool transition_ongoing;
    spinlock_t transition_lock;
    wait_queue_head_t transition_wait;
    struct task_struct *transition_task;
    struct cpufreq_stats *stats;
    void *driver_data;
    struct thermal_cooling_device *cdev;
    struct notifier_block nb_min;
    struct notifier_block nb_max;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct cpufreq_policy {
    cpumask_var_t cpus;
    cpumask_var_t related_cpus;
    cpumask_var_t real_cpus;
    unsigned int shared_type;
    unsigned int cpu;
    struct clk *clk;
    struct cpufreq_cpuinfo cpuinfo;
    unsigned int min;
    unsigned int max;
    unsigned int cur;
    unsigned int suspend_freq;
    unsigned int policy;
    unsigned int last_policy;
    struct cpufreq_governor *governor;
    void *governor_data;
    char last_governor[16];
    struct work_struct update;
    struct freq_constraints constraints;
    struct freq_qos_request *min_freq_req;
    struct freq_qos_request *max_freq_req;
    struct cpufreq_frequency_table *freq_table;
    enum cpufreq_table_sorting freq_table_sorted;
    struct list_head policy_list;
    struct kobject kobj;
    struct completion kobj_unregister;
    struct rw_semaphore rwsem;
    bool fast_switch_possible;
    bool fast_switch_enabled;
    bool strict_target;
    unsigned int transition_delay_us;
    bool dvfs_possible_from_any_cpu;
    unsigned int cached_target_freq;
    unsigned int cached_resolved_idx;
    bool transition_ongoing;
    spinlock_t transition_lock;
    wait_queue_head_t transition_wait;
    struct task_struct *transition_task;
    struct cpufreq_stats *stats;
    void *driver_data;
    struct thermal_cooling_device *cdev;
    struct notifier_block nb_min;
    struct notifier_block nb_max;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct cpufreq_policy {
    cpumask_var_t cpus;
    cpumask_var_t related_cpus;
    cpumask_var_t real_cpus;
    unsigned int shared_type;
    unsigned int cpu;
    struct clk *clk;
    struct cpufreq_cpuinfo cpuinfo;
    unsigned int min;
    unsigned int max;
    unsigned int cur;
    unsigned int suspend_freq;
    unsigned int policy;
    unsigned int last_policy;
    struct cpufreq_governor *governor;
    void *governor_data;
    char last_governor[16];
    struct work_struct update;
    struct freq_constraints constraints;
    struct freq_qos_request *min_freq_req;
    struct freq_qos_request *max_freq_req;
    struct cpufreq_frequency_table *freq_table;
    enum cpufreq_table_sorting freq_table_sorted;
    struct list_head policy_list;
    struct kobject kobj;
    struct completion kobj_unregister;
    struct rw_semaphore rwsem;
    bool fast_switch_possible;
    bool fast_switch_enabled;
    bool strict_target;
    bool efficiencies_available;
    unsigned int transition_delay_us;
    bool dvfs_possible_from_any_cpu;
    unsigned int cached_target_freq;
    unsigned int cached_resolved_idx;
    bool transition_ongoing;
    spinlock_t transition_lock;
    wait_queue_head_t transition_wait;
    struct task_struct *transition_task;
    struct cpufreq_stats *stats;
    void *driver_data;
    struct thermal_cooling_device *cdev;
    struct notifier_block nb_min;
    struct notifier_block nb_max;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct cpufreq_policy {
    cpumask_var_t cpus;
    cpumask_var_t related_cpus;
    cpumask_var_t real_cpus;
    unsigned int shared_type;
    unsigned int cpu;
    struct clk *clk;
    struct cpufreq_cpuinfo cpuinfo;
    unsigned int min;
    unsigned int max;
    unsigned int cur;
    unsigned int suspend_freq;
    unsigned int policy;
    unsigned int last_policy;
    struct cpufreq_governor *governor;
    void *governor_data;
    char last_governor[16];
    struct work_struct update;
    struct freq_constraints constraints;
    struct freq_qos_request *min_freq_req;
    struct freq_qos_request *max_freq_req;
    struct cpufreq_frequency_table *freq_table;
    enum cpufreq_table_sorting freq_table_sorted;
    struct list_head policy_list;
    struct kobject kobj;
    struct completion kobj_unregister;
    struct rw_semaphore rwsem;
    bool fast_switch_possible;
    bool fast_switch_enabled;
    bool strict_target;
    bool efficiencies_available;
    unsigned int transition_delay_us;
    bool dvfs_possible_from_any_cpu;
    unsigned int cached_target_freq;
    unsigned int cached_resolved_idx;
    bool transition_ongoing;
    spinlock_t transition_lock;
    wait_queue_head_t transition_wait;
    struct task_struct *transition_task;
    struct cpufreq_stats *stats;
    void *driver_data;
    struct thermal_cooling_device *cdev;
    struct notifier_block nb_min;
    struct notifier_block nb_max;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct cpufreq_policy {
    cpumask_var_t cpus;
    cpumask_var_t related_cpus;
    cpumask_var_t real_cpus;
    unsigned int shared_type;
    unsigned int cpu;
    struct clk *clk;
    struct cpufreq_cpuinfo cpuinfo;
    unsigned int min;
    unsigned int max;
    unsigned int cur;
    unsigned int suspend_freq;
    unsigned int policy;
    unsigned int last_policy;
    struct cpufreq_governor *governor;
    void *governor_data;
    char last_governor[16];
    struct work_struct update;
    struct freq_constraints constraints;
    struct freq_qos_request *min_freq_req;
    struct freq_qos_request *max_freq_req;
    struct cpufreq_frequency_table *freq_table;
    enum cpufreq_table_sorting freq_table_sorted;
    struct list_head policy_list;
    struct kobject kobj;
    struct completion kobj_unregister;
    struct rw_semaphore rwsem;
    bool fast_switch_possible;
    bool fast_switch_enabled;
    bool strict_target;
    bool efficiencies_available;
    unsigned int transition_delay_us;
    bool dvfs_possible_from_any_cpu;
    unsigned int cached_target_freq;
    unsigned int cached_resolved_idx;
    bool transition_ongoing;
    spinlock_t transition_lock;
    wait_queue_head_t transition_wait;
    struct task_struct *transition_task;
    struct cpufreq_stats *stats;
    void *driver_data;
    struct thermal_cooling_device *cdev;
    struct notifier_block nb_min;
    struct notifier_block nb_max;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct cpufreq_policy {
    cpumask_var_t cpus;
    cpumask_var_t related_cpus;
    cpumask_var_t real_cpus;
    unsigned int shared_type;
    unsigned int cpu;
    struct clk *clk;
    struct cpufreq_cpuinfo cpuinfo;
    unsigned int min;
    unsigned int max;
    unsigned int cur;
    unsigned int suspend_freq;
    unsigned int policy;
    unsigned int last_policy;
    struct cpufreq_governor *governor;
    void *governor_data;
    char last_governor[16];
    struct work_struct update;
    struct freq_constraints constraints;
    struct freq_qos_request *min_freq_req;
    struct freq_qos_request *max_freq_req;
    struct cpufreq_frequency_table *freq_table;
    enum cpufreq_table_sorting freq_table_sorted;
    struct list_head policy_list;
    struct kobject kobj;
    struct completion kobj_unregister;
    struct rw_semaphore rwsem;
    bool fast_switch_possible;
    bool fast_switch_enabled;
    bool strict_target;
    bool efficiencies_available;
    unsigned int transition_delay_us;
    bool dvfs_possible_from_any_cpu;
    bool boost_enabled;
    unsigned int cached_target_freq;
    unsigned int cached_resolved_idx;
    bool transition_ongoing;
    spinlock_t transition_lock;
    wait_queue_head_t transition_wait;
    struct task_struct *transition_task;
    struct cpufreq_stats *stats;
    void *driver_data;
    struct thermal_cooling_device *cdev;
    struct notifier_block nb_min;
    struct notifier_block nb_max;
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
struct cpufreq_policy {
    cpumask_var_t cpus;
    cpumask_var_t related_cpus;
    cpumask_var_t real_cpus;
    unsigned int shared_type;
    unsigned int cpu;
    struct clk *clk;
    struct cpufreq_cpuinfo cpuinfo;
    unsigned int min;
    unsigned int max;
    unsigned int cur;
    unsigned int restore_freq;
    unsigned int suspend_freq;
    unsigned int policy;
    unsigned int last_policy;
    struct cpufreq_governor *governor;
    void *governor_data;
    char last_governor[16];
    struct work_struct update;
    struct freq_constraints constraints;
    struct freq_qos_request *min_freq_req;
    struct freq_qos_request *max_freq_req;
    struct cpufreq_frequency_table *freq_table;
    enum cpufreq_table_sorting freq_table_sorted;
    struct list_head policy_list;
    struct kobject kobj;
    struct completion kobj_unregister;
    struct rw_semaphore rwsem;
    bool fast_switch_possible;
    bool fast_switch_enabled;
    unsigned int transition_delay_us;
    bool dvfs_possible_from_any_cpu;
    unsigned int cached_target_freq;
    int cached_resolved_idx;
    bool transition_ongoing;
    spinlock_t transition_lock;
    wait_queue_head_t transition_wait;
    struct task_struct *transition_task;
    struct cpufreq_stats *stats;
    void *driver_data;
    struct thermal_cooling_device *cdev;
    struct notifier_block nb_min;
    struct notifier_block nb_max;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct cpufreq_policy {
    cpumask_var_t cpus;
    cpumask_var_t related_cpus;
    cpumask_var_t real_cpus;
    unsigned int shared_type;
    unsigned int cpu;
    struct clk *clk;
    struct cpufreq_cpuinfo cpuinfo;
    unsigned int min;
    unsigned int max;
    unsigned int cur;
    unsigned int restore_freq;
    unsigned int suspend_freq;
    unsigned int policy;
    unsigned int last_policy;
    struct cpufreq_governor *governor;
    void *governor_data;
    char last_governor[16];
    struct work_struct update;
    struct freq_constraints constraints;
    struct freq_qos_request *min_freq_req;
    struct freq_qos_request *max_freq_req;
    struct cpufreq_frequency_table *freq_table;
    enum cpufreq_table_sorting freq_table_sorted;
    struct list_head policy_list;
    struct kobject kobj;
    struct completion kobj_unregister;
    struct rw_semaphore rwsem;
    bool fast_switch_possible;
    bool fast_switch_enabled;
    unsigned int transition_delay_us;
    bool dvfs_possible_from_any_cpu;
    unsigned int cached_target_freq;
    int cached_resolved_idx;
    bool transition_ongoing;
    spinlock_t transition_lock;
    wait_queue_head_t transition_wait;
    struct task_struct *transition_task;
    struct cpufreq_stats *stats;
    void *driver_data;
    struct thermal_cooling_device *cdev;
    struct notifier_block nb_min;
    struct notifier_block nb_max;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct cpufreq_policy {
    cpumask_var_t cpus;
    cpumask_var_t related_cpus;
    cpumask_var_t real_cpus;
    unsigned int shared_type;
    unsigned int cpu;
    struct clk *clk;
    struct cpufreq_cpuinfo cpuinfo;
    unsigned int min;
    unsigned int max;
    unsigned int cur;
    unsigned int restore_freq;
    unsigned int suspend_freq;
    unsigned int policy;
    unsigned int last_policy;
    struct cpufreq_governor *governor;
    void *governor_data;
    char last_governor[16];
    struct work_struct update;
    struct freq_constraints constraints;
    struct freq_qos_request *min_freq_req;
    struct freq_qos_request *max_freq_req;
    struct cpufreq_frequency_table *freq_table;
    enum cpufreq_table_sorting freq_table_sorted;
    struct list_head policy_list;
    struct kobject kobj;
    struct completion kobj_unregister;
    struct rw_semaphore rwsem;
    bool fast_switch_possible;
    bool fast_switch_enabled;
    unsigned int transition_delay_us;
    bool dvfs_possible_from_any_cpu;
    unsigned int cached_target_freq;
    int cached_resolved_idx;
    bool transition_ongoing;
    spinlock_t transition_lock;
    wait_queue_head_t transition_wait;
    struct task_struct *transition_task;
    struct cpufreq_stats *stats;
    void *driver_data;
    struct thermal_cooling_device *cdev;
    struct notifier_block nb_min;
    struct notifier_block nb_max;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct cpufreq_policy {
    cpumask_var_t cpus;
    cpumask_var_t related_cpus;
    cpumask_var_t real_cpus;
    unsigned int shared_type;
    unsigned int cpu;
    struct clk *clk;
    struct cpufreq_cpuinfo cpuinfo;
    unsigned int min;
    unsigned int max;
    unsigned int cur;
    unsigned int restore_freq;
    unsigned int suspend_freq;
    unsigned int policy;
    unsigned int last_policy;
    struct cpufreq_governor *governor;
    void *governor_data;
    char last_governor[16];
    struct work_struct update;
    struct freq_constraints constraints;
    struct freq_qos_request *min_freq_req;
    struct freq_qos_request *max_freq_req;
    struct cpufreq_frequency_table *freq_table;
    enum cpufreq_table_sorting freq_table_sorted;
    struct list_head policy_list;
    struct kobject kobj;
    struct completion kobj_unregister;
    struct rw_semaphore rwsem;
    bool fast_switch_possible;
    bool fast_switch_enabled;
    unsigned int transition_delay_us;
    bool dvfs_possible_from_any_cpu;
    unsigned int cached_target_freq;
    int cached_resolved_idx;
    bool transition_ongoing;
    spinlock_t transition_lock;
    wait_queue_head_t transition_wait;
    struct task_struct *transition_task;
    struct cpufreq_stats *stats;
    void *driver_data;
    struct thermal_cooling_device *cdev;
    struct notifier_block nb_min;
    struct notifier_block nb_max;
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
struct cpufreq_policy {
    cpumask_var_t cpus;
    cpumask_var_t related_cpus;
    cpumask_var_t real_cpus;
    unsigned int shared_type;
    unsigned int cpu;
    struct clk *clk;
    struct cpufreq_cpuinfo cpuinfo;
    unsigned int min;
    unsigned int max;
    unsigned int cur;
    unsigned int restore_freq;
    unsigned int suspend_freq;
    unsigned int policy;
    unsigned int last_policy;
    struct cpufreq_governor *governor;
    void *governor_data;
    char last_governor[16];
    struct work_struct update;
    struct freq_constraints constraints;
    struct freq_qos_request *min_freq_req;
    struct freq_qos_request *max_freq_req;
    struct cpufreq_frequency_table *freq_table;
    enum cpufreq_table_sorting freq_table_sorted;
    struct list_head policy_list;
    struct kobject kobj;
    struct completion kobj_unregister;
    struct rw_semaphore rwsem;
    bool fast_switch_possible;
    bool fast_switch_enabled;
    unsigned int transition_delay_us;
    bool dvfs_possible_from_any_cpu;
    unsigned int cached_target_freq;
    int cached_resolved_idx;
    bool transition_ongoing;
    spinlock_t transition_lock;
    wait_queue_head_t transition_wait;
    struct task_struct *transition_task;
    struct cpufreq_stats *stats;
    void *driver_data;
    struct thermal_cooling_device *cdev;
    struct notifier_block nb_min;
    struct notifier_block nb_max;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct cpufreq_policy {
    cpumask_var_t cpus;
    cpumask_var_t related_cpus;
    cpumask_var_t real_cpus;
    unsigned int shared_type;
    unsigned int cpu;
    struct clk *clk;
    struct cpufreq_cpuinfo cpuinfo;
    unsigned int min;
    unsigned int max;
    unsigned int cur;
    unsigned int restore_freq;
    unsigned int suspend_freq;
    unsigned int policy;
    unsigned int last_policy;
    struct cpufreq_governor *governor;
    void *governor_data;
    char last_governor[16];
    struct work_struct update;
    struct freq_constraints constraints;
    struct freq_qos_request *min_freq_req;
    struct freq_qos_request *max_freq_req;
    struct cpufreq_frequency_table *freq_table;
    enum cpufreq_table_sorting freq_table_sorted;
    struct list_head policy_list;
    struct kobject kobj;
    struct completion kobj_unregister;
    struct rw_semaphore rwsem;
    bool fast_switch_possible;
    bool fast_switch_enabled;
    unsigned int transition_delay_us;
    bool dvfs_possible_from_any_cpu;
    unsigned int cached_target_freq;
    int cached_resolved_idx;
    bool transition_ongoing;
    spinlock_t transition_lock;
    wait_queue_head_t transition_wait;
    struct task_struct *transition_task;
    struct cpufreq_stats *stats;
    void *driver_data;
    struct thermal_cooling_device *cdev;
    struct notifier_block nb_min;
    struct notifier_block nb_max;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct cpufreq_policy {
    cpumask_var_t cpus;
    cpumask_var_t related_cpus;
    cpumask_var_t real_cpus;
    unsigned int shared_type;
    unsigned int cpu;
    struct clk *clk;
    struct cpufreq_cpuinfo cpuinfo;
    unsigned int min;
    unsigned int max;
    unsigned int cur;
    unsigned int restore_freq;
    unsigned int suspend_freq;
    unsigned int policy;
    unsigned int last_policy;
    struct cpufreq_governor *governor;
    void *governor_data;
    char last_governor[16];
    struct work_struct update;
    struct freq_constraints constraints;
    struct freq_qos_request *min_freq_req;
    struct freq_qos_request *max_freq_req;
    struct cpufreq_frequency_table *freq_table;
    enum cpufreq_table_sorting freq_table_sorted;
    struct list_head policy_list;
    struct kobject kobj;
    struct completion kobj_unregister;
    struct rw_semaphore rwsem;
    bool fast_switch_possible;
    bool fast_switch_enabled;
    unsigned int transition_delay_us;
    bool dvfs_possible_from_any_cpu;
    unsigned int cached_target_freq;
    int cached_resolved_idx;
    bool transition_ongoing;
    spinlock_t transition_lock;
    wait_queue_head_t transition_wait;
    struct task_struct *transition_task;
    struct cpufreq_stats *stats;
    void *driver_data;
    struct thermal_cooling_device *cdev;
    struct notifier_block nb_min;
    struct notifier_block nb_max;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cpufreq_policy {
    cpumask_var_t cpus;
    cpumask_var_t related_cpus;
    cpumask_var_t real_cpus;
    unsigned int shared_type;
    unsigned int cpu;
    struct clk *clk;
    struct cpufreq_cpuinfo cpuinfo;
    unsigned int min;
    unsigned int max;
    unsigned int cur;
    unsigned int restore_freq;
    unsigned int suspend_freq;
    unsigned int policy;
    unsigned int last_policy;
    struct cpufreq_governor *governor;
    void *governor_data;
    char last_governor[16];
    struct work_struct update;
    struct freq_constraints constraints;
    struct freq_qos_request *min_freq_req;
    struct freq_qos_request *max_freq_req;
    struct cpufreq_frequency_table *freq_table;
    enum cpufreq_table_sorting freq_table_sorted;
    struct list_head policy_list;
    struct kobject kobj;
    struct completion kobj_unregister;
    struct rw_semaphore rwsem;
    bool fast_switch_possible;
    bool fast_switch_enabled;
    unsigned int transition_delay_us;
    bool dvfs_possible_from_any_cpu;
    unsigned int cached_target_freq;
    int cached_resolved_idx;
    bool transition_ongoing;
    spinlock_t transition_lock;
    wait_queue_head_t transition_wait;
    struct task_struct *transition_task;
    struct cpufreq_stats *stats;
    void *driver_data;
    struct thermal_cooling_device *cdev;
    struct notifier_block nb_min;
    struct notifier_block nb_max;
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
<code>enum cpufreq_table_sorting freq_table_sorted</code>
</li>
<li>
<b>Field added. </b>
<code>bool fast_switch_possible</code>
</li>
<li>
<b>Field added. </b>
<code>bool fast_switch_enabled</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int cached_target_freq</code>
</li>
<li>
<b>Field added. </b>
<code>int cached_resolved_idx</code>
</li>
<li>
<b>Field removed. </b>
<code>bool governor_enabled</code>
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
<b>Field added. </b>
<code>unsigned int transition_delay_us</code>
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
<code>bool dvfs_possible_from_any_cpu</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct dev_pm_qos_request *min_freq_req</code>
</li>
<li>
<b>Field added. </b>
<code>struct dev_pm_qos_request *max_freq_req</code>
</li>
<li>
<b>Field added. </b>
<code>struct thermal_cooling_device *cdev</code>
</li>
<li>
<b>Field added. </b>
<code>struct notifier_block nb_min</code>
</li>
<li>
<b>Field added. </b>
<code>struct notifier_block nb_max</code>
</li>
<li>
<b>Field removed. </b>
<code>struct cpufreq_user_policy user_policy</code>
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
<code>struct freq_constraints constraints</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct dev_pm_qos_request *min_freq_req</code> ➡️ <code>struct freq_qos_request *min_freq_req</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct dev_pm_qos_request *max_freq_req</code> ➡️ <code>struct freq_qos_request *max_freq_req</code>
</li>
</ul>
</details>
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
<code>bool strict_target</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int restore_freq</code>
</li>
<li>
<b>Field type changed. </b>
<code>int cached_resolved_idx</code> ➡️ <code>unsigned int cached_resolved_idx</code>
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
<code>bool efficiencies_available</code>
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
<b>Field added. </b>
<code>bool boost_enabled</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct clk *clk</code> ➡️ <code>struct clk *clk</code>
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
<code>struct cpufreq_stats *stats</code> ➡️ <code>struct cpufreq_stats *stats</code>
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
