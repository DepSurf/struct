# Struct: <code>generic_pm_domain</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct generic_pm_domain {
    struct dev_pm_domain domain;
    struct list_head gpd_list_node;
    struct list_head master_links;
    struct list_head slave_links;
    struct list_head dev_list;
    struct mutex lock;
    struct dev_power_governor *gov;
    struct work_struct power_off_work;
    const char *name;
    atomic_t sd_count;
    enum gpd_status status;
    unsigned int device_count;
    unsigned int suspended_count;
    unsigned int prepared_count;
    int (*power_off)(struct generic_pm_domain *);
    int (*power_on)(struct generic_pm_domain *);
    struct gpd_dev_ops dev_ops;
    s64 max_off_time_ns;
    bool max_off_time_changed;
    bool cached_power_down_ok;
    int (*attach_dev)(struct generic_pm_domain *, struct device *);
    void (*detach_dev)(struct generic_pm_domain *, struct device *);
    unsigned int flags;
    struct genpd_power_state states[8];
    unsigned int state_count;
    unsigned int state_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct generic_pm_domain {
    struct dev_pm_domain domain;
    struct list_head gpd_list_node;
    struct list_head master_links;
    struct list_head slave_links;
    struct list_head dev_list;
    struct dev_power_governor *gov;
    struct work_struct power_off_work;
    struct fwnode_handle *provider;
    bool has_provider;
    const char *name;
    atomic_t sd_count;
    enum gpd_status status;
    unsigned int device_count;
    unsigned int suspended_count;
    unsigned int prepared_count;
    int (*power_off)(struct generic_pm_domain *);
    int (*power_on)(struct generic_pm_domain *);
    struct gpd_dev_ops dev_ops;
    s64 max_off_time_ns;
    bool max_off_time_changed;
    bool cached_power_down_ok;
    int (*attach_dev)(struct generic_pm_domain *, struct device *);
    void (*detach_dev)(struct generic_pm_domain *, struct device *);
    unsigned int flags;
    struct genpd_power_state *states;
    unsigned int state_count;
    unsigned int state_idx;
    void *free;
    const struct genpd_lock_ops *lock_ops;
    struct mutex mlock;
    spinlock_t slock;
    long unsigned int lock_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct generic_pm_domain {
    struct dev_pm_domain domain;
    struct list_head gpd_list_node;
    struct list_head master_links;
    struct list_head slave_links;
    struct list_head dev_list;
    struct dev_power_governor *gov;
    struct work_struct power_off_work;
    struct fwnode_handle *provider;
    bool has_provider;
    const char *name;
    atomic_t sd_count;
    enum gpd_status status;
    unsigned int device_count;
    unsigned int suspended_count;
    unsigned int prepared_count;
    int (*power_off)(struct generic_pm_domain *);
    int (*power_on)(struct generic_pm_domain *);
    struct gpd_dev_ops dev_ops;
    s64 max_off_time_ns;
    bool max_off_time_changed;
    bool cached_power_down_ok;
    int (*attach_dev)(struct generic_pm_domain *, struct device *);
    void (*detach_dev)(struct generic_pm_domain *, struct device *);
    unsigned int flags;
    struct genpd_power_state *states;
    unsigned int state_count;
    unsigned int state_idx;
    void *free;
    const struct genpd_lock_ops *lock_ops;
    struct mutex mlock;
    spinlock_t slock;
    long unsigned int lock_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct generic_pm_domain {
    struct dev_pm_domain domain;
    struct list_head gpd_list_node;
    struct list_head master_links;
    struct list_head slave_links;
    struct list_head dev_list;
    struct dev_power_governor *gov;
    struct work_struct power_off_work;
    struct fwnode_handle *provider;
    bool has_provider;
    const char *name;
    atomic_t sd_count;
    enum gpd_status status;
    unsigned int device_count;
    unsigned int suspended_count;
    unsigned int prepared_count;
    unsigned int performance_state;
    int (*power_off)(struct generic_pm_domain *);
    int (*power_on)(struct generic_pm_domain *);
    int (*set_performance_state)(struct generic_pm_domain *, unsigned int);
    struct gpd_dev_ops dev_ops;
    s64 max_off_time_ns;
    bool max_off_time_changed;
    bool cached_power_down_ok;
    int (*attach_dev)(struct generic_pm_domain *, struct device *);
    void (*detach_dev)(struct generic_pm_domain *, struct device *);
    unsigned int flags;
    struct genpd_power_state *states;
    unsigned int state_count;
    unsigned int state_idx;
    void *free;
    ktime_t on_time;
    ktime_t accounting_time;
    const struct genpd_lock_ops *lock_ops;
    struct mutex mlock;
    spinlock_t slock;
    long unsigned int lock_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct generic_pm_domain {
    struct device dev;
    struct dev_pm_domain domain;
    struct list_head gpd_list_node;
    struct list_head master_links;
    struct list_head slave_links;
    struct list_head dev_list;
    struct dev_power_governor *gov;
    struct work_struct power_off_work;
    struct fwnode_handle *provider;
    bool has_provider;
    const char *name;
    atomic_t sd_count;
    enum gpd_status status;
    unsigned int device_count;
    unsigned int suspended_count;
    unsigned int prepared_count;
    unsigned int performance_state;
    int (*power_off)(struct generic_pm_domain *);
    int (*power_on)(struct generic_pm_domain *);
    unsigned int (*opp_to_performance_state)(struct generic_pm_domain *, struct dev_pm_opp *);
    int (*set_performance_state)(struct generic_pm_domain *, unsigned int);
    struct gpd_dev_ops dev_ops;
    s64 max_off_time_ns;
    bool max_off_time_changed;
    bool cached_power_down_ok;
    int (*attach_dev)(struct generic_pm_domain *, struct device *);
    void (*detach_dev)(struct generic_pm_domain *, struct device *);
    unsigned int flags;
    struct genpd_power_state *states;
    unsigned int state_count;
    unsigned int state_idx;
    void *free;
    ktime_t on_time;
    ktime_t accounting_time;
    const struct genpd_lock_ops *lock_ops;
    struct mutex mlock;
    spinlock_t slock;
    long unsigned int lock_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct generic_pm_domain {
    struct device dev;
    struct dev_pm_domain domain;
    struct list_head gpd_list_node;
    struct list_head master_links;
    struct list_head slave_links;
    struct list_head dev_list;
    struct dev_power_governor *gov;
    struct work_struct power_off_work;
    struct fwnode_handle *provider;
    bool has_provider;
    const char *name;
    atomic_t sd_count;
    enum gpd_status status;
    unsigned int device_count;
    unsigned int suspended_count;
    unsigned int prepared_count;
    unsigned int performance_state;
    int (*power_off)(struct generic_pm_domain *);
    int (*power_on)(struct generic_pm_domain *);
    struct opp_table *opp_table;
    unsigned int (*opp_to_performance_state)(struct generic_pm_domain *, struct dev_pm_opp *);
    int (*set_performance_state)(struct generic_pm_domain *, unsigned int);
    struct gpd_dev_ops dev_ops;
    s64 max_off_time_ns;
    bool max_off_time_changed;
    bool cached_power_down_ok;
    int (*attach_dev)(struct generic_pm_domain *, struct device *);
    void (*detach_dev)(struct generic_pm_domain *, struct device *);
    unsigned int flags;
    struct genpd_power_state *states;
    unsigned int state_count;
    unsigned int state_idx;
    void *free;
    ktime_t on_time;
    ktime_t accounting_time;
    const struct genpd_lock_ops *lock_ops;
    struct mutex mlock;
    spinlock_t slock;
    long unsigned int lock_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct generic_pm_domain {
    struct device dev;
    struct dev_pm_domain domain;
    struct list_head gpd_list_node;
    struct list_head master_links;
    struct list_head slave_links;
    struct list_head dev_list;
    struct dev_power_governor *gov;
    struct work_struct power_off_work;
    struct fwnode_handle *provider;
    bool has_provider;
    const char *name;
    atomic_t sd_count;
    enum gpd_status status;
    unsigned int device_count;
    unsigned int suspended_count;
    unsigned int prepared_count;
    unsigned int performance_state;
    cpumask_var_t cpus;
    int (*power_off)(struct generic_pm_domain *);
    int (*power_on)(struct generic_pm_domain *);
    struct opp_table *opp_table;
    unsigned int (*opp_to_performance_state)(struct generic_pm_domain *, struct dev_pm_opp *);
    int (*set_performance_state)(struct generic_pm_domain *, unsigned int);
    struct gpd_dev_ops dev_ops;
    s64 max_off_time_ns;
    bool max_off_time_changed;
    bool cached_power_down_ok;
    bool cached_power_down_state_idx;
    int (*attach_dev)(struct generic_pm_domain *, struct device *);
    void (*detach_dev)(struct generic_pm_domain *, struct device *);
    unsigned int flags;
    struct genpd_power_state *states;
    void (*free_states)(struct genpd_power_state *, unsigned int);
    unsigned int state_count;
    unsigned int state_idx;
    ktime_t on_time;
    ktime_t accounting_time;
    const struct genpd_lock_ops *lock_ops;
    struct mutex mlock;
    spinlock_t slock;
    long unsigned int lock_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct generic_pm_domain {
    struct device dev;
    struct dev_pm_domain domain;
    struct list_head gpd_list_node;
    struct list_head master_links;
    struct list_head slave_links;
    struct list_head dev_list;
    struct dev_power_governor *gov;
    struct work_struct power_off_work;
    struct fwnode_handle *provider;
    bool has_provider;
    const char *name;
    atomic_t sd_count;
    enum gpd_status status;
    unsigned int device_count;
    unsigned int suspended_count;
    unsigned int prepared_count;
    unsigned int performance_state;
    cpumask_var_t cpus;
    int (*power_off)(struct generic_pm_domain *);
    int (*power_on)(struct generic_pm_domain *);
    struct opp_table *opp_table;
    unsigned int (*opp_to_performance_state)(struct generic_pm_domain *, struct dev_pm_opp *);
    int (*set_performance_state)(struct generic_pm_domain *, unsigned int);
    struct gpd_dev_ops dev_ops;
    s64 max_off_time_ns;
    bool max_off_time_changed;
    bool cached_power_down_ok;
    bool cached_power_down_state_idx;
    int (*attach_dev)(struct generic_pm_domain *, struct device *);
    void (*detach_dev)(struct generic_pm_domain *, struct device *);
    unsigned int flags;
    struct genpd_power_state *states;
    void (*free_states)(struct genpd_power_state *, unsigned int);
    unsigned int state_count;
    unsigned int state_idx;
    ktime_t on_time;
    ktime_t accounting_time;
    const struct genpd_lock_ops *lock_ops;
    struct mutex mlock;
    spinlock_t slock;
    long unsigned int lock_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct generic_pm_domain {
    struct device dev;
    struct dev_pm_domain domain;
    struct list_head gpd_list_node;
    struct list_head master_links;
    struct list_head slave_links;
    struct list_head dev_list;
    struct dev_power_governor *gov;
    struct work_struct power_off_work;
    struct fwnode_handle *provider;
    bool has_provider;
    const char *name;
    atomic_t sd_count;
    enum gpd_status status;
    unsigned int device_count;
    unsigned int suspended_count;
    unsigned int prepared_count;
    unsigned int performance_state;
    cpumask_var_t cpus;
    int (*power_off)(struct generic_pm_domain *);
    int (*power_on)(struct generic_pm_domain *);
    struct opp_table *opp_table;
    unsigned int (*opp_to_performance_state)(struct generic_pm_domain *, struct dev_pm_opp *);
    int (*set_performance_state)(struct generic_pm_domain *, unsigned int);
    struct gpd_dev_ops dev_ops;
    s64 max_off_time_ns;
    bool max_off_time_changed;
    bool cached_power_down_ok;
    bool cached_power_down_state_idx;
    int (*attach_dev)(struct generic_pm_domain *, struct device *);
    void (*detach_dev)(struct generic_pm_domain *, struct device *);
    unsigned int flags;
    struct genpd_power_state *states;
    void (*free_states)(struct genpd_power_state *, unsigned int);
    unsigned int state_count;
    unsigned int state_idx;
    ktime_t on_time;
    ktime_t accounting_time;
    const struct genpd_lock_ops *lock_ops;
    struct mutex mlock;
    spinlock_t slock;
    long unsigned int lock_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct generic_pm_domain {
    struct device dev;
    struct dev_pm_domain domain;
    struct list_head gpd_list_node;
    struct list_head parent_links;
    struct list_head child_links;
    struct list_head dev_list;
    struct dev_power_governor *gov;
    struct work_struct power_off_work;
    struct fwnode_handle *provider;
    bool has_provider;
    const char *name;
    atomic_t sd_count;
    enum gpd_status status;
    unsigned int device_count;
    unsigned int suspended_count;
    unsigned int prepared_count;
    unsigned int performance_state;
    cpumask_var_t cpus;
    int (*power_off)(struct generic_pm_domain *);
    int (*power_on)(struct generic_pm_domain *);
    struct raw_notifier_head power_notifiers;
    struct opp_table *opp_table;
    unsigned int (*opp_to_performance_state)(struct generic_pm_domain *, struct dev_pm_opp *);
    int (*set_performance_state)(struct generic_pm_domain *, unsigned int);
    struct gpd_dev_ops dev_ops;
    s64 max_off_time_ns;
    bool max_off_time_changed;
    bool cached_power_down_ok;
    bool cached_power_down_state_idx;
    int (*attach_dev)(struct generic_pm_domain *, struct device *);
    void (*detach_dev)(struct generic_pm_domain *, struct device *);
    unsigned int flags;
    struct genpd_power_state *states;
    void (*free_states)(struct genpd_power_state *, unsigned int);
    unsigned int state_count;
    unsigned int state_idx;
    ktime_t on_time;
    ktime_t accounting_time;
    const struct genpd_lock_ops *lock_ops;
    struct mutex mlock;
    spinlock_t slock;
    long unsigned int lock_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct generic_pm_domain {
    struct device dev;
    struct dev_pm_domain domain;
    struct list_head gpd_list_node;
    struct list_head parent_links;
    struct list_head child_links;
    struct list_head dev_list;
    struct dev_power_governor *gov;
    struct work_struct power_off_work;
    struct fwnode_handle *provider;
    bool has_provider;
    const char *name;
    atomic_t sd_count;
    enum gpd_status status;
    unsigned int device_count;
    unsigned int suspended_count;
    unsigned int prepared_count;
    unsigned int performance_state;
    cpumask_var_t cpus;
    int (*power_off)(struct generic_pm_domain *);
    int (*power_on)(struct generic_pm_domain *);
    struct raw_notifier_head power_notifiers;
    struct opp_table *opp_table;
    unsigned int (*opp_to_performance_state)(struct generic_pm_domain *, struct dev_pm_opp *);
    int (*set_performance_state)(struct generic_pm_domain *, unsigned int);
    struct gpd_dev_ops dev_ops;
    s64 max_off_time_ns;
    ktime_t next_wakeup;
    bool max_off_time_changed;
    bool cached_power_down_ok;
    bool cached_power_down_state_idx;
    int (*attach_dev)(struct generic_pm_domain *, struct device *);
    void (*detach_dev)(struct generic_pm_domain *, struct device *);
    unsigned int flags;
    struct genpd_power_state *states;
    void (*free_states)(struct genpd_power_state *, unsigned int);
    unsigned int state_count;
    unsigned int state_idx;
    ktime_t on_time;
    ktime_t accounting_time;
    const struct genpd_lock_ops *lock_ops;
    struct mutex mlock;
    spinlock_t slock;
    long unsigned int lock_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct generic_pm_domain {
    struct device dev;
    struct dev_pm_domain domain;
    struct list_head gpd_list_node;
    struct list_head parent_links;
    struct list_head child_links;
    struct list_head dev_list;
    struct dev_power_governor *gov;
    struct work_struct power_off_work;
    struct fwnode_handle *provider;
    bool has_provider;
    const char *name;
    atomic_t sd_count;
    enum gpd_status status;
    unsigned int device_count;
    unsigned int suspended_count;
    unsigned int prepared_count;
    unsigned int performance_state;
    cpumask_var_t cpus;
    int (*power_off)(struct generic_pm_domain *);
    int (*power_on)(struct generic_pm_domain *);
    struct raw_notifier_head power_notifiers;
    struct opp_table *opp_table;
    unsigned int (*opp_to_performance_state)(struct generic_pm_domain *, struct dev_pm_opp *);
    int (*set_performance_state)(struct generic_pm_domain *, unsigned int);
    struct gpd_dev_ops dev_ops;
    s64 max_off_time_ns;
    ktime_t next_wakeup;
    bool max_off_time_changed;
    bool cached_power_down_ok;
    bool cached_power_down_state_idx;
    int (*attach_dev)(struct generic_pm_domain *, struct device *);
    void (*detach_dev)(struct generic_pm_domain *, struct device *);
    unsigned int flags;
    struct genpd_power_state *states;
    void (*free_states)(struct genpd_power_state *, unsigned int);
    unsigned int state_count;
    unsigned int state_idx;
    ktime_t on_time;
    ktime_t accounting_time;
    const struct genpd_lock_ops *lock_ops;
    struct mutex mlock;
    spinlock_t slock;
    long unsigned int lock_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct generic_pm_domain {
    struct device dev;
    struct dev_pm_domain domain;
    struct list_head gpd_list_node;
    struct list_head parent_links;
    struct list_head child_links;
    struct list_head dev_list;
    struct dev_power_governor *gov;
    struct genpd_governor_data *gd;
    struct work_struct power_off_work;
    struct fwnode_handle *provider;
    bool has_provider;
    const char *name;
    atomic_t sd_count;
    enum gpd_status status;
    unsigned int device_count;
    unsigned int suspended_count;
    unsigned int prepared_count;
    unsigned int performance_state;
    cpumask_var_t cpus;
    int (*power_off)(struct generic_pm_domain *);
    int (*power_on)(struct generic_pm_domain *);
    struct raw_notifier_head power_notifiers;
    struct opp_table *opp_table;
    unsigned int (*opp_to_performance_state)(struct generic_pm_domain *, struct dev_pm_opp *);
    int (*set_performance_state)(struct generic_pm_domain *, unsigned int);
    struct gpd_dev_ops dev_ops;
    int (*attach_dev)(struct generic_pm_domain *, struct device *);
    void (*detach_dev)(struct generic_pm_domain *, struct device *);
    unsigned int flags;
    struct genpd_power_state *states;
    void (*free_states)(struct genpd_power_state *, unsigned int);
    unsigned int state_count;
    unsigned int state_idx;
    u64 on_time;
    u64 accounting_time;
    const struct genpd_lock_ops *lock_ops;
    struct mutex mlock;
    spinlock_t slock;
    long unsigned int lock_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct generic_pm_domain {
    struct device dev;
    struct dev_pm_domain domain;
    struct list_head gpd_list_node;
    struct list_head parent_links;
    struct list_head child_links;
    struct list_head dev_list;
    struct dev_power_governor *gov;
    struct genpd_governor_data *gd;
    struct work_struct power_off_work;
    struct fwnode_handle *provider;
    bool has_provider;
    const char *name;
    atomic_t sd_count;
    enum gpd_status status;
    unsigned int device_count;
    unsigned int suspended_count;
    unsigned int prepared_count;
    unsigned int performance_state;
    cpumask_var_t cpus;
    int (*power_off)(struct generic_pm_domain *);
    int (*power_on)(struct generic_pm_domain *);
    struct raw_notifier_head power_notifiers;
    struct opp_table *opp_table;
    unsigned int (*opp_to_performance_state)(struct generic_pm_domain *, struct dev_pm_opp *);
    int (*set_performance_state)(struct generic_pm_domain *, unsigned int);
    struct gpd_dev_ops dev_ops;
    int (*attach_dev)(struct generic_pm_domain *, struct device *);
    void (*detach_dev)(struct generic_pm_domain *, struct device *);
    unsigned int flags;
    struct genpd_power_state *states;
    void (*free_states)(struct genpd_power_state *, unsigned int);
    unsigned int state_count;
    unsigned int state_idx;
    u64 on_time;
    u64 accounting_time;
    const struct genpd_lock_ops *lock_ops;
    struct mutex mlock;
    spinlock_t slock;
    long unsigned int lock_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct generic_pm_domain {
    struct device dev;
    struct dev_pm_domain domain;
    struct list_head gpd_list_node;
    struct list_head parent_links;
    struct list_head child_links;
    struct list_head dev_list;
    struct dev_power_governor *gov;
    struct genpd_governor_data *gd;
    struct work_struct power_off_work;
    struct fwnode_handle *provider;
    bool has_provider;
    const char *name;
    atomic_t sd_count;
    enum gpd_status status;
    unsigned int device_count;
    unsigned int suspended_count;
    unsigned int prepared_count;
    unsigned int performance_state;
    cpumask_var_t cpus;
    bool synced_poweroff;
    int (*power_off)(struct generic_pm_domain *);
    int (*power_on)(struct generic_pm_domain *);
    struct raw_notifier_head power_notifiers;
    struct opp_table *opp_table;
    unsigned int (*opp_to_performance_state)(struct generic_pm_domain *, struct dev_pm_opp *);
    int (*set_performance_state)(struct generic_pm_domain *, unsigned int);
    struct gpd_dev_ops dev_ops;
    int (*attach_dev)(struct generic_pm_domain *, struct device *);
    void (*detach_dev)(struct generic_pm_domain *, struct device *);
    unsigned int flags;
    struct genpd_power_state *states;
    void (*free_states)(struct genpd_power_state *, unsigned int);
    unsigned int state_count;
    unsigned int state_idx;
    u64 on_time;
    u64 accounting_time;
    const struct genpd_lock_ops *lock_ops;
    struct mutex mlock;
    spinlock_t slock;
    long unsigned int lock_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct generic_pm_domain {
    struct device dev;
    struct dev_pm_domain domain;
    struct list_head gpd_list_node;
    struct list_head parent_links;
    struct list_head child_links;
    struct list_head dev_list;
    struct dev_power_governor *gov;
    struct genpd_governor_data *gd;
    struct work_struct power_off_work;
    struct fwnode_handle *provider;
    bool has_provider;
    const char *name;
    atomic_t sd_count;
    enum gpd_status status;
    unsigned int device_count;
    unsigned int suspended_count;
    unsigned int prepared_count;
    unsigned int performance_state;
    cpumask_var_t cpus;
    bool synced_poweroff;
    int (*power_off)(struct generic_pm_domain *);
    int (*power_on)(struct generic_pm_domain *);
    struct raw_notifier_head power_notifiers;
    struct opp_table *opp_table;
    int (*set_performance_state)(struct generic_pm_domain *, unsigned int);
    struct gpd_dev_ops dev_ops;
    int (*attach_dev)(struct generic_pm_domain *, struct device *);
    void (*detach_dev)(struct generic_pm_domain *, struct device *);
    unsigned int flags;
    struct genpd_power_state *states;
    void (*free_states)(struct genpd_power_state *, unsigned int);
    unsigned int state_count;
    unsigned int state_idx;
    u64 on_time;
    u64 accounting_time;
    const struct genpd_lock_ops *lock_ops;
    struct mutex mlock;
    spinlock_t slock;
    long unsigned int lock_flags;
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
struct generic_pm_domain {
    struct device dev;
    struct dev_pm_domain domain;
    struct list_head gpd_list_node;
    struct list_head master_links;
    struct list_head slave_links;
    struct list_head dev_list;
    struct dev_power_governor *gov;
    struct work_struct power_off_work;
    struct fwnode_handle *provider;
    bool has_provider;
    const char *name;
    atomic_t sd_count;
    enum gpd_status status;
    unsigned int device_count;
    unsigned int suspended_count;
    unsigned int prepared_count;
    unsigned int performance_state;
    cpumask_var_t cpus;
    int (*power_off)(struct generic_pm_domain *);
    int (*power_on)(struct generic_pm_domain *);
    struct opp_table *opp_table;
    unsigned int (*opp_to_performance_state)(struct generic_pm_domain *, struct dev_pm_opp *);
    int (*set_performance_state)(struct generic_pm_domain *, unsigned int);
    struct gpd_dev_ops dev_ops;
    s64 max_off_time_ns;
    bool max_off_time_changed;
    bool cached_power_down_ok;
    bool cached_power_down_state_idx;
    int (*attach_dev)(struct generic_pm_domain *, struct device *);
    void (*detach_dev)(struct generic_pm_domain *, struct device *);
    unsigned int flags;
    struct genpd_power_state *states;
    void (*free_states)(struct genpd_power_state *, unsigned int);
    unsigned int state_count;
    unsigned int state_idx;
    ktime_t on_time;
    ktime_t accounting_time;
    const struct genpd_lock_ops *lock_ops;
    struct mutex mlock;
    spinlock_t slock;
    long unsigned int lock_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct generic_pm_domain {
    struct device dev;
    struct dev_pm_domain domain;
    struct list_head gpd_list_node;
    struct list_head master_links;
    struct list_head slave_links;
    struct list_head dev_list;
    struct dev_power_governor *gov;
    struct work_struct power_off_work;
    struct fwnode_handle *provider;
    bool has_provider;
    const char *name;
    atomic_t sd_count;
    enum gpd_status status;
    unsigned int device_count;
    unsigned int suspended_count;
    unsigned int prepared_count;
    unsigned int performance_state;
    cpumask_var_t cpus;
    int (*power_off)(struct generic_pm_domain *);
    int (*power_on)(struct generic_pm_domain *);
    struct opp_table *opp_table;
    unsigned int (*opp_to_performance_state)(struct generic_pm_domain *, struct dev_pm_opp *);
    int (*set_performance_state)(struct generic_pm_domain *, unsigned int);
    struct gpd_dev_ops dev_ops;
    s64 max_off_time_ns;
    bool max_off_time_changed;
    bool cached_power_down_ok;
    bool cached_power_down_state_idx;
    int (*attach_dev)(struct generic_pm_domain *, struct device *);
    void (*detach_dev)(struct generic_pm_domain *, struct device *);
    unsigned int flags;
    struct genpd_power_state *states;
    void (*free_states)(struct genpd_power_state *, unsigned int);
    unsigned int state_count;
    unsigned int state_idx;
    ktime_t on_time;
    ktime_t accounting_time;
    const struct genpd_lock_ops *lock_ops;
    struct mutex mlock;
    spinlock_t slock;
    long unsigned int lock_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct generic_pm_domain {
    struct device dev;
    struct dev_pm_domain domain;
    struct list_head gpd_list_node;
    struct list_head master_links;
    struct list_head slave_links;
    struct list_head dev_list;
    struct dev_power_governor *gov;
    struct work_struct power_off_work;
    struct fwnode_handle *provider;
    bool has_provider;
    const char *name;
    atomic_t sd_count;
    enum gpd_status status;
    unsigned int device_count;
    unsigned int suspended_count;
    unsigned int prepared_count;
    unsigned int performance_state;
    cpumask_var_t cpus;
    int (*power_off)(struct generic_pm_domain *);
    int (*power_on)(struct generic_pm_domain *);
    struct opp_table *opp_table;
    unsigned int (*opp_to_performance_state)(struct generic_pm_domain *, struct dev_pm_opp *);
    int (*set_performance_state)(struct generic_pm_domain *, unsigned int);
    struct gpd_dev_ops dev_ops;
    s64 max_off_time_ns;
    bool max_off_time_changed;
    bool cached_power_down_ok;
    bool cached_power_down_state_idx;
    int (*attach_dev)(struct generic_pm_domain *, struct device *);
    void (*detach_dev)(struct generic_pm_domain *, struct device *);
    unsigned int flags;
    struct genpd_power_state *states;
    void (*free_states)(struct genpd_power_state *, unsigned int);
    unsigned int state_count;
    unsigned int state_idx;
    ktime_t on_time;
    ktime_t accounting_time;
    const struct genpd_lock_ops *lock_ops;
    struct mutex mlock;
    spinlock_t slock;
    long unsigned int lock_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct generic_pm_domain {
    struct device dev;
    struct dev_pm_domain domain;
    struct list_head gpd_list_node;
    struct list_head master_links;
    struct list_head slave_links;
    struct list_head dev_list;
    struct dev_power_governor *gov;
    struct work_struct power_off_work;
    struct fwnode_handle *provider;
    bool has_provider;
    const char *name;
    atomic_t sd_count;
    enum gpd_status status;
    unsigned int device_count;
    unsigned int suspended_count;
    unsigned int prepared_count;
    unsigned int performance_state;
    cpumask_var_t cpus;
    int (*power_off)(struct generic_pm_domain *);
    int (*power_on)(struct generic_pm_domain *);
    struct opp_table *opp_table;
    unsigned int (*opp_to_performance_state)(struct generic_pm_domain *, struct dev_pm_opp *);
    int (*set_performance_state)(struct generic_pm_domain *, unsigned int);
    struct gpd_dev_ops dev_ops;
    s64 max_off_time_ns;
    bool max_off_time_changed;
    bool cached_power_down_ok;
    bool cached_power_down_state_idx;
    int (*attach_dev)(struct generic_pm_domain *, struct device *);
    void (*detach_dev)(struct generic_pm_domain *, struct device *);
    unsigned int flags;
    struct genpd_power_state *states;
    void (*free_states)(struct genpd_power_state *, unsigned int);
    unsigned int state_count;
    unsigned int state_idx;
    ktime_t on_time;
    ktime_t accounting_time;
    const struct genpd_lock_ops *lock_ops;
    struct mutex mlock;
    spinlock_t slock;
    long unsigned int lock_flags;
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
struct generic_pm_domain {
    struct device dev;
    struct dev_pm_domain domain;
    struct list_head gpd_list_node;
    struct list_head master_links;
    struct list_head slave_links;
    struct list_head dev_list;
    struct dev_power_governor *gov;
    struct work_struct power_off_work;
    struct fwnode_handle *provider;
    bool has_provider;
    const char *name;
    atomic_t sd_count;
    enum gpd_status status;
    unsigned int device_count;
    unsigned int suspended_count;
    unsigned int prepared_count;
    unsigned int performance_state;
    cpumask_var_t cpus;
    int (*power_off)(struct generic_pm_domain *);
    int (*power_on)(struct generic_pm_domain *);
    struct opp_table *opp_table;
    unsigned int (*opp_to_performance_state)(struct generic_pm_domain *, struct dev_pm_opp *);
    int (*set_performance_state)(struct generic_pm_domain *, unsigned int);
    struct gpd_dev_ops dev_ops;
    s64 max_off_time_ns;
    bool max_off_time_changed;
    bool cached_power_down_ok;
    bool cached_power_down_state_idx;
    int (*attach_dev)(struct generic_pm_domain *, struct device *);
    void (*detach_dev)(struct generic_pm_domain *, struct device *);
    unsigned int flags;
    struct genpd_power_state *states;
    void (*free_states)(struct genpd_power_state *, unsigned int);
    unsigned int state_count;
    unsigned int state_idx;
    ktime_t on_time;
    ktime_t accounting_time;
    const struct genpd_lock_ops *lock_ops;
    struct mutex mlock;
    spinlock_t slock;
    long unsigned int lock_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct generic_pm_domain {
    struct device dev;
    struct dev_pm_domain domain;
    struct list_head gpd_list_node;
    struct list_head master_links;
    struct list_head slave_links;
    struct list_head dev_list;
    struct dev_power_governor *gov;
    struct work_struct power_off_work;
    struct fwnode_handle *provider;
    bool has_provider;
    const char *name;
    atomic_t sd_count;
    enum gpd_status status;
    unsigned int device_count;
    unsigned int suspended_count;
    unsigned int prepared_count;
    unsigned int performance_state;
    cpumask_var_t cpus;
    int (*power_off)(struct generic_pm_domain *);
    int (*power_on)(struct generic_pm_domain *);
    struct opp_table *opp_table;
    unsigned int (*opp_to_performance_state)(struct generic_pm_domain *, struct dev_pm_opp *);
    int (*set_performance_state)(struct generic_pm_domain *, unsigned int);
    struct gpd_dev_ops dev_ops;
    s64 max_off_time_ns;
    bool max_off_time_changed;
    bool cached_power_down_ok;
    bool cached_power_down_state_idx;
    int (*attach_dev)(struct generic_pm_domain *, struct device *);
    void (*detach_dev)(struct generic_pm_domain *, struct device *);
    unsigned int flags;
    struct genpd_power_state *states;
    void (*free_states)(struct genpd_power_state *, unsigned int);
    unsigned int state_count;
    unsigned int state_idx;
    ktime_t on_time;
    ktime_t accounting_time;
    const struct genpd_lock_ops *lock_ops;
    struct mutex mlock;
    spinlock_t slock;
    long unsigned int lock_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct generic_pm_domain {
    struct device dev;
    struct dev_pm_domain domain;
    struct list_head gpd_list_node;
    struct list_head master_links;
    struct list_head slave_links;
    struct list_head dev_list;
    struct dev_power_governor *gov;
    struct work_struct power_off_work;
    struct fwnode_handle *provider;
    bool has_provider;
    const char *name;
    atomic_t sd_count;
    enum gpd_status status;
    unsigned int device_count;
    unsigned int suspended_count;
    unsigned int prepared_count;
    unsigned int performance_state;
    cpumask_var_t cpus;
    int (*power_off)(struct generic_pm_domain *);
    int (*power_on)(struct generic_pm_domain *);
    struct opp_table *opp_table;
    unsigned int (*opp_to_performance_state)(struct generic_pm_domain *, struct dev_pm_opp *);
    int (*set_performance_state)(struct generic_pm_domain *, unsigned int);
    struct gpd_dev_ops dev_ops;
    s64 max_off_time_ns;
    bool max_off_time_changed;
    bool cached_power_down_ok;
    bool cached_power_down_state_idx;
    int (*attach_dev)(struct generic_pm_domain *, struct device *);
    void (*detach_dev)(struct generic_pm_domain *, struct device *);
    unsigned int flags;
    struct genpd_power_state *states;
    void (*free_states)(struct genpd_power_state *, unsigned int);
    unsigned int state_count;
    unsigned int state_idx;
    ktime_t on_time;
    ktime_t accounting_time;
    const struct genpd_lock_ops *lock_ops;
    struct mutex mlock;
    spinlock_t slock;
    long unsigned int lock_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct generic_pm_domain {
    struct device dev;
    struct dev_pm_domain domain;
    struct list_head gpd_list_node;
    struct list_head master_links;
    struct list_head slave_links;
    struct list_head dev_list;
    struct dev_power_governor *gov;
    struct work_struct power_off_work;
    struct fwnode_handle *provider;
    bool has_provider;
    const char *name;
    atomic_t sd_count;
    enum gpd_status status;
    unsigned int device_count;
    unsigned int suspended_count;
    unsigned int prepared_count;
    unsigned int performance_state;
    cpumask_var_t cpus;
    int (*power_off)(struct generic_pm_domain *);
    int (*power_on)(struct generic_pm_domain *);
    struct opp_table *opp_table;
    unsigned int (*opp_to_performance_state)(struct generic_pm_domain *, struct dev_pm_opp *);
    int (*set_performance_state)(struct generic_pm_domain *, unsigned int);
    struct gpd_dev_ops dev_ops;
    s64 max_off_time_ns;
    bool max_off_time_changed;
    bool cached_power_down_ok;
    bool cached_power_down_state_idx;
    int (*attach_dev)(struct generic_pm_domain *, struct device *);
    void (*detach_dev)(struct generic_pm_domain *, struct device *);
    unsigned int flags;
    struct genpd_power_state *states;
    void (*free_states)(struct genpd_power_state *, unsigned int);
    unsigned int state_count;
    unsigned int state_idx;
    ktime_t on_time;
    ktime_t accounting_time;
    const struct genpd_lock_ops *lock_ops;
    struct mutex mlock;
    spinlock_t slock;
    long unsigned int lock_flags;
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
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct fwnode_handle *provider</code>
</li>
<li>
<b>Field added. </b>
<code>bool has_provider</code>
</li>
<li>
<b>Field added. </b>
<code>void *free</code>
</li>
<li>
<b>Field added. </b>
<code>const struct genpd_lock_ops *lock_ops</code>
</li>
<li>
<b>Field added. </b>
<code>struct mutex mlock</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t slock</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int lock_flags</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mutex lock</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct genpd_power_state states[8]</code> ➡️ <code>struct genpd_power_state *states</code>
</li>
</ul>
</details>
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
<code>unsigned int performance_state</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_performance_state)(struct generic_pm_domain *, unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>ktime_t on_time</code>
</li>
<li>
<b>Field added. </b>
<code>ktime_t accounting_time</code>
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
<code>struct device dev</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int (*opp_to_performance_state)(struct generic_pm_domain *, struct dev_pm_opp *)</code>
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
<code>struct opp_table *opp_table</code>
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
<code>cpumask_var_t cpus</code>
</li>
<li>
<b>Field added. </b>
<code>bool cached_power_down_state_idx</code>
</li>
<li>
<b>Field added. </b>
<code>void (*free_states)(struct genpd_power_state *, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void *free</code>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head parent_links</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head child_links</code>
</li>
<li>
<b>Field added. </b>
<code>struct raw_notifier_head power_notifiers</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head master_links</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head slave_links</code>
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
<code>ktime_t next_wakeup</code>
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
<code>struct genpd_governor_data *gd</code>
</li>
<li>
<b>Field removed. </b>
<code>s64 max_off_time_ns</code>
</li>
<li>
<b>Field removed. </b>
<code>ktime_t next_wakeup</code>
</li>
<li>
<b>Field removed. </b>
<code>bool max_off_time_changed</code>
</li>
<li>
<b>Field removed. </b>
<code>bool cached_power_down_ok</code>
</li>
<li>
<b>Field removed. </b>
<code>bool cached_power_down_state_idx</code>
</li>
<li>
<b>Field type changed. </b>
<code>ktime_t on_time</code> ➡️ <code>u64 on_time</code>
</li>
<li>
<b>Field type changed. </b>
<code>ktime_t accounting_time</code> ➡️ <code>u64 accounting_time</code>
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
<code>bool synced_poweroff</code>
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
<code>unsigned int (*opp_to_performance_state)(struct generic_pm_domain *, struct dev_pm_opp *)</code>
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
