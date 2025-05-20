# Struct: <code>devfreq</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct devfreq {
    struct list_head node;
    struct mutex lock;
    struct device dev;
    struct devfreq_dev_profile *profile;
    const struct devfreq_governor *governor;
    char governor_name[16];
    struct notifier_block nb;
    struct delayed_work work;
    long unsigned int previous_freq;
    struct devfreq_dev_status last_status;
    void *data;
    long unsigned int min_freq;
    long unsigned int max_freq;
    bool stop_polling;
    unsigned int total_trans;
    unsigned int *trans_table;
    long unsigned int *time_in_state;
    long unsigned int last_stat_updated;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct devfreq {
    struct list_head node;
    struct mutex lock;
    struct device dev;
    struct devfreq_dev_profile *profile;
    const struct devfreq_governor *governor;
    char governor_name[16];
    struct notifier_block nb;
    struct delayed_work work;
    long unsigned int previous_freq;
    struct devfreq_dev_status last_status;
    void *data;
    long unsigned int min_freq;
    long unsigned int max_freq;
    bool stop_polling;
    unsigned int total_trans;
    unsigned int *trans_table;
    long unsigned int *time_in_state;
    long unsigned int last_stat_updated;
    struct srcu_notifier_head transition_notifier_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct devfreq {
    struct list_head node;
    struct mutex lock;
    struct device dev;
    struct devfreq_dev_profile *profile;
    const struct devfreq_governor *governor;
    char governor_name[16];
    struct notifier_block nb;
    struct delayed_work work;
    long unsigned int previous_freq;
    struct devfreq_dev_status last_status;
    void *data;
    long unsigned int min_freq;
    long unsigned int max_freq;
    bool stop_polling;
    unsigned int total_trans;
    unsigned int *trans_table;
    long unsigned int *time_in_state;
    long unsigned int last_stat_updated;
    struct srcu_notifier_head transition_notifier_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct devfreq {
    struct list_head node;
    struct mutex lock;
    struct device dev;
    struct devfreq_dev_profile *profile;
    const struct devfreq_governor *governor;
    char governor_name[16];
    struct notifier_block nb;
    struct delayed_work work;
    long unsigned int previous_freq;
    struct devfreq_dev_status last_status;
    void *data;
    long unsigned int min_freq;
    long unsigned int max_freq;
    bool stop_polling;
    unsigned int total_trans;
    unsigned int *trans_table;
    long unsigned int *time_in_state;
    long unsigned int last_stat_updated;
    struct srcu_notifier_head transition_notifier_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct devfreq {
    struct list_head node;
    struct mutex lock;
    struct device dev;
    struct devfreq_dev_profile *profile;
    const struct devfreq_governor *governor;
    char governor_name[16];
    struct notifier_block nb;
    struct delayed_work work;
    long unsigned int previous_freq;
    struct devfreq_dev_status last_status;
    void *data;
    long unsigned int min_freq;
    long unsigned int max_freq;
    long unsigned int scaling_min_freq;
    long unsigned int scaling_max_freq;
    bool stop_polling;
    unsigned int total_trans;
    unsigned int *trans_table;
    long unsigned int *time_in_state;
    long unsigned int last_stat_updated;
    struct srcu_notifier_head transition_notifier_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct devfreq {
    struct list_head node;
    struct mutex lock;
    struct device dev;
    struct devfreq_dev_profile *profile;
    const struct devfreq_governor *governor;
    char governor_name[16];
    struct notifier_block nb;
    struct delayed_work work;
    long unsigned int previous_freq;
    struct devfreq_dev_status last_status;
    void *data;
    long unsigned int min_freq;
    long unsigned int max_freq;
    long unsigned int scaling_min_freq;
    long unsigned int scaling_max_freq;
    bool stop_polling;
    unsigned int total_trans;
    unsigned int *trans_table;
    long unsigned int *time_in_state;
    long unsigned int last_stat_updated;
    struct srcu_notifier_head transition_notifier_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct devfreq {
    struct list_head node;
    struct mutex lock;
    struct device dev;
    struct devfreq_dev_profile *profile;
    const struct devfreq_governor *governor;
    char governor_name[16];
    struct notifier_block nb;
    struct delayed_work work;
    long unsigned int previous_freq;
    struct devfreq_dev_status last_status;
    void *data;
    long unsigned int min_freq;
    long unsigned int max_freq;
    long unsigned int scaling_min_freq;
    long unsigned int scaling_max_freq;
    bool stop_polling;
    long unsigned int suspend_freq;
    long unsigned int resume_freq;
    atomic_t suspend_count;
    unsigned int total_trans;
    unsigned int *trans_table;
    long unsigned int *time_in_state;
    long unsigned int last_stat_updated;
    struct srcu_notifier_head transition_notifier_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct devfreq {
    struct list_head node;
    struct mutex lock;
    struct device dev;
    struct devfreq_dev_profile *profile;
    const struct devfreq_governor *governor;
    char governor_name[16];
    struct notifier_block nb;
    struct delayed_work work;
    long unsigned int previous_freq;
    struct devfreq_dev_status last_status;
    void *data;
    long unsigned int min_freq;
    long unsigned int max_freq;
    long unsigned int scaling_min_freq;
    long unsigned int scaling_max_freq;
    bool stop_polling;
    long unsigned int suspend_freq;
    long unsigned int resume_freq;
    atomic_t suspend_count;
    unsigned int total_trans;
    unsigned int *trans_table;
    long unsigned int *time_in_state;
    long unsigned int last_stat_updated;
    struct srcu_notifier_head transition_notifier_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct devfreq {
    struct list_head node;
    struct mutex lock;
    struct device dev;
    struct devfreq_dev_profile *profile;
    const struct devfreq_governor *governor;
    char governor_name[16];
    struct notifier_block nb;
    struct delayed_work work;
    long unsigned int previous_freq;
    struct devfreq_dev_status last_status;
    void *data;
    long unsigned int min_freq;
    long unsigned int max_freq;
    long unsigned int scaling_min_freq;
    long unsigned int scaling_max_freq;
    bool stop_polling;
    long unsigned int suspend_freq;
    long unsigned int resume_freq;
    atomic_t suspend_count;
    unsigned int total_trans;
    unsigned int *trans_table;
    long unsigned int *time_in_state;
    long unsigned int last_stat_updated;
    struct srcu_notifier_head transition_notifier_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct devfreq {
    struct list_head node;
    struct mutex lock;
    struct device dev;
    struct devfreq_dev_profile *profile;
    const struct devfreq_governor *governor;
    char governor_name[16];
    struct notifier_block nb;
    struct delayed_work work;
    long unsigned int previous_freq;
    struct devfreq_dev_status last_status;
    void *data;
    struct dev_pm_qos_request user_min_freq_req;
    struct dev_pm_qos_request user_max_freq_req;
    long unsigned int scaling_min_freq;
    long unsigned int scaling_max_freq;
    bool stop_polling;
    long unsigned int suspend_freq;
    long unsigned int resume_freq;
    atomic_t suspend_count;
    struct devfreq_stats stats;
    struct srcu_notifier_head transition_notifier_list;
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
struct devfreq {
    struct list_head node;
    struct mutex lock;
    struct device dev;
    struct devfreq_dev_profile *profile;
    const struct devfreq_governor *governor;
    struct notifier_block nb;
    struct delayed_work work;
    long unsigned int previous_freq;
    struct devfreq_dev_status last_status;
    void *data;
    struct dev_pm_qos_request user_min_freq_req;
    struct dev_pm_qos_request user_max_freq_req;
    long unsigned int scaling_min_freq;
    long unsigned int scaling_max_freq;
    bool stop_polling;
    long unsigned int suspend_freq;
    long unsigned int resume_freq;
    atomic_t suspend_count;
    struct devfreq_stats stats;
    struct srcu_notifier_head transition_notifier_list;
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
struct devfreq {
    struct list_head node;
    struct mutex lock;
    struct device dev;
    struct devfreq_dev_profile *profile;
    const struct devfreq_governor *governor;
    struct opp_table *opp_table;
    struct notifier_block nb;
    struct delayed_work work;
    long unsigned int previous_freq;
    struct devfreq_dev_status last_status;
    void *data;
    struct dev_pm_qos_request user_min_freq_req;
    struct dev_pm_qos_request user_max_freq_req;
    long unsigned int scaling_min_freq;
    long unsigned int scaling_max_freq;
    bool stop_polling;
    long unsigned int suspend_freq;
    long unsigned int resume_freq;
    atomic_t suspend_count;
    struct devfreq_stats stats;
    struct srcu_notifier_head transition_notifier_list;
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
struct devfreq {
    struct list_head node;
    struct mutex lock;
    struct device dev;
    struct devfreq_dev_profile *profile;
    const struct devfreq_governor *governor;
    struct opp_table *opp_table;
    struct notifier_block nb;
    struct delayed_work work;
    long unsigned int previous_freq;
    struct devfreq_dev_status last_status;
    void *data;
    struct dev_pm_qos_request user_min_freq_req;
    struct dev_pm_qos_request user_max_freq_req;
    long unsigned int scaling_min_freq;
    long unsigned int scaling_max_freq;
    bool stop_polling;
    long unsigned int suspend_freq;
    long unsigned int resume_freq;
    atomic_t suspend_count;
    struct devfreq_stats stats;
    struct srcu_notifier_head transition_notifier_list;
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
struct devfreq {
    struct list_head node;
    struct mutex lock;
    struct device dev;
    struct devfreq_dev_profile *profile;
    const struct devfreq_governor *governor;
    struct opp_table *opp_table;
    struct notifier_block nb;
    struct delayed_work work;
    long unsigned int *freq_table;
    unsigned int max_state;
    long unsigned int previous_freq;
    struct devfreq_dev_status last_status;
    void *data;
    struct dev_pm_qos_request user_min_freq_req;
    struct dev_pm_qos_request user_max_freq_req;
    long unsigned int scaling_min_freq;
    long unsigned int scaling_max_freq;
    bool stop_polling;
    long unsigned int suspend_freq;
    long unsigned int resume_freq;
    atomic_t suspend_count;
    struct devfreq_stats stats;
    struct srcu_notifier_head transition_notifier_list;
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
struct devfreq {
    struct list_head node;
    struct mutex lock;
    struct device dev;
    struct devfreq_dev_profile *profile;
    const struct devfreq_governor *governor;
    struct opp_table *opp_table;
    struct notifier_block nb;
    struct delayed_work work;
    long unsigned int *freq_table;
    unsigned int max_state;
    long unsigned int previous_freq;
    struct devfreq_dev_status last_status;
    void *data;
    void *governor_data;
    struct dev_pm_qos_request user_min_freq_req;
    struct dev_pm_qos_request user_max_freq_req;
    long unsigned int scaling_min_freq;
    long unsigned int scaling_max_freq;
    bool stop_polling;
    long unsigned int suspend_freq;
    long unsigned int resume_freq;
    atomic_t suspend_count;
    struct devfreq_stats stats;
    struct srcu_notifier_head transition_notifier_list;
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
struct devfreq {
    struct list_head node;
    struct mutex lock;
    struct device dev;
    struct devfreq_dev_profile *profile;
    const struct devfreq_governor *governor;
    struct opp_table *opp_table;
    struct notifier_block nb;
    struct delayed_work work;
    long unsigned int *freq_table;
    unsigned int max_state;
    long unsigned int previous_freq;
    struct devfreq_dev_status last_status;
    void *data;
    void *governor_data;
    struct dev_pm_qos_request user_min_freq_req;
    struct dev_pm_qos_request user_max_freq_req;
    long unsigned int scaling_min_freq;
    long unsigned int scaling_max_freq;
    bool stop_polling;
    long unsigned int suspend_freq;
    long unsigned int resume_freq;
    atomic_t suspend_count;
    struct devfreq_stats stats;
    struct srcu_notifier_head transition_notifier_list;
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
struct devfreq {
    struct list_head node;
    struct mutex lock;
    struct device dev;
    struct devfreq_dev_profile *profile;
    const struct devfreq_governor *governor;
    struct opp_table *opp_table;
    struct notifier_block nb;
    struct delayed_work work;
    long unsigned int *freq_table;
    unsigned int max_state;
    long unsigned int previous_freq;
    struct devfreq_dev_status last_status;
    void *data;
    void *governor_data;
    struct dev_pm_qos_request user_min_freq_req;
    struct dev_pm_qos_request user_max_freq_req;
    long unsigned int scaling_min_freq;
    long unsigned int scaling_max_freq;
    bool stop_polling;
    long unsigned int suspend_freq;
    long unsigned int resume_freq;
    atomic_t suspend_count;
    struct devfreq_stats stats;
    struct srcu_notifier_head transition_notifier_list;
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
struct devfreq {
    struct list_head node;
    struct mutex lock;
    struct device dev;
    struct devfreq_dev_profile *profile;
    const struct devfreq_governor *governor;
    char governor_name[16];
    struct notifier_block nb;
    struct delayed_work work;
    long unsigned int previous_freq;
    struct devfreq_dev_status last_status;
    void *data;
    long unsigned int min_freq;
    long unsigned int max_freq;
    long unsigned int scaling_min_freq;
    long unsigned int scaling_max_freq;
    bool stop_polling;
    long unsigned int suspend_freq;
    long unsigned int resume_freq;
    atomic_t suspend_count;
    unsigned int total_trans;
    unsigned int *trans_table;
    long unsigned int *time_in_state;
    long unsigned int last_stat_updated;
    struct srcu_notifier_head transition_notifier_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct devfreq {
    struct list_head node;
    struct mutex lock;
    struct device dev;
    struct devfreq_dev_profile *profile;
    const struct devfreq_governor *governor;
    char governor_name[16];
    struct notifier_block nb;
    struct delayed_work work;
    long unsigned int previous_freq;
    struct devfreq_dev_status last_status;
    void *data;
    long unsigned int min_freq;
    long unsigned int max_freq;
    long unsigned int scaling_min_freq;
    long unsigned int scaling_max_freq;
    bool stop_polling;
    long unsigned int suspend_freq;
    long unsigned int resume_freq;
    atomic_t suspend_count;
    unsigned int total_trans;
    unsigned int *trans_table;
    long unsigned int *time_in_state;
    long unsigned int last_stat_updated;
    struct srcu_notifier_head transition_notifier_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct devfreq {
    struct list_head node;
    struct mutex lock;
    struct device dev;
    struct devfreq_dev_profile *profile;
    const struct devfreq_governor *governor;
    char governor_name[16];
    struct notifier_block nb;
    struct delayed_work work;
    long unsigned int previous_freq;
    struct devfreq_dev_status last_status;
    void *data;
    long unsigned int min_freq;
    long unsigned int max_freq;
    long unsigned int scaling_min_freq;
    long unsigned int scaling_max_freq;
    bool stop_polling;
    long unsigned int suspend_freq;
    long unsigned int resume_freq;
    atomic_t suspend_count;
    unsigned int total_trans;
    unsigned int *trans_table;
    long unsigned int *time_in_state;
    long unsigned int last_stat_updated;
    struct srcu_notifier_head transition_notifier_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct devfreq {
    struct list_head node;
    struct mutex lock;
    struct device dev;
    struct devfreq_dev_profile *profile;
    const struct devfreq_governor *governor;
    char governor_name[16];
    struct notifier_block nb;
    struct delayed_work work;
    long unsigned int previous_freq;
    struct devfreq_dev_status last_status;
    void *data;
    long unsigned int min_freq;
    long unsigned int max_freq;
    long unsigned int scaling_min_freq;
    long unsigned int scaling_max_freq;
    bool stop_polling;
    long unsigned int suspend_freq;
    long unsigned int resume_freq;
    atomic_t suspend_count;
    unsigned int total_trans;
    unsigned int *trans_table;
    long unsigned int *time_in_state;
    long unsigned int last_stat_updated;
    struct srcu_notifier_head transition_notifier_list;
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
struct devfreq {
    struct list_head node;
    struct mutex lock;
    struct device dev;
    struct devfreq_dev_profile *profile;
    const struct devfreq_governor *governor;
    char governor_name[16];
    struct notifier_block nb;
    struct delayed_work work;
    long unsigned int previous_freq;
    struct devfreq_dev_status last_status;
    void *data;
    long unsigned int min_freq;
    long unsigned int max_freq;
    long unsigned int scaling_min_freq;
    long unsigned int scaling_max_freq;
    bool stop_polling;
    long unsigned int suspend_freq;
    long unsigned int resume_freq;
    atomic_t suspend_count;
    unsigned int total_trans;
    unsigned int *trans_table;
    long unsigned int *time_in_state;
    long unsigned int last_stat_updated;
    struct srcu_notifier_head transition_notifier_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct devfreq {
    struct list_head node;
    struct mutex lock;
    struct device dev;
    struct devfreq_dev_profile *profile;
    const struct devfreq_governor *governor;
    char governor_name[16];
    struct notifier_block nb;
    struct delayed_work work;
    long unsigned int previous_freq;
    struct devfreq_dev_status last_status;
    void *data;
    long unsigned int min_freq;
    long unsigned int max_freq;
    long unsigned int scaling_min_freq;
    long unsigned int scaling_max_freq;
    bool stop_polling;
    long unsigned int suspend_freq;
    long unsigned int resume_freq;
    atomic_t suspend_count;
    unsigned int total_trans;
    unsigned int *trans_table;
    long unsigned int *time_in_state;
    long unsigned int last_stat_updated;
    struct srcu_notifier_head transition_notifier_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct devfreq {
    struct list_head node;
    struct mutex lock;
    struct device dev;
    struct devfreq_dev_profile *profile;
    const struct devfreq_governor *governor;
    char governor_name[16];
    struct notifier_block nb;
    struct delayed_work work;
    long unsigned int previous_freq;
    struct devfreq_dev_status last_status;
    void *data;
    long unsigned int min_freq;
    long unsigned int max_freq;
    long unsigned int scaling_min_freq;
    long unsigned int scaling_max_freq;
    bool stop_polling;
    long unsigned int suspend_freq;
    long unsigned int resume_freq;
    atomic_t suspend_count;
    unsigned int total_trans;
    unsigned int *trans_table;
    long unsigned int *time_in_state;
    long unsigned int last_stat_updated;
    struct srcu_notifier_head transition_notifier_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct devfreq {
    struct list_head node;
    struct mutex lock;
    struct device dev;
    struct devfreq_dev_profile *profile;
    const struct devfreq_governor *governor;
    char governor_name[16];
    struct notifier_block nb;
    struct delayed_work work;
    long unsigned int previous_freq;
    struct devfreq_dev_status last_status;
    void *data;
    long unsigned int min_freq;
    long unsigned int max_freq;
    long unsigned int scaling_min_freq;
    long unsigned int scaling_max_freq;
    bool stop_polling;
    long unsigned int suspend_freq;
    long unsigned int resume_freq;
    atomic_t suspend_count;
    unsigned int total_trans;
    unsigned int *trans_table;
    long unsigned int *time_in_state;
    long unsigned int last_stat_updated;
    struct srcu_notifier_head transition_notifier_list;
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
<code>struct srcu_notifier_head transition_notifier_list</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int scaling_min_freq</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int scaling_max_freq</code>
</li>
</ul>
</details>
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
<code>long unsigned int suspend_freq</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int resume_freq</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t suspend_count</code>
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
<code>struct dev_pm_qos_request user_min_freq_req</code>
</li>
<li>
<b>Field added. </b>
<code>struct dev_pm_qos_request user_max_freq_req</code>
</li>
<li>
<b>Field added. </b>
<code>struct devfreq_stats stats</code>
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
<code>long unsigned int min_freq</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int max_freq</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int total_trans</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int *trans_table</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int *time_in_state</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int last_stat_updated</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>char governor_name[16]</code>
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
<code>struct opp_table *opp_table</code>
</li>
<li>
<b>Field added. </b>
<code>struct thermal_cooling_device *cdev</code>
</li>
</ul>
</details>
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
<code>long unsigned int *freq_table</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int max_state</code>
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
<code>void *governor_data</code>
</li>
</ul>
</details>
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
