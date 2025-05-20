# Struct: <code>opp_table</code>

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
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct opp_table {
    struct list_head node;
    struct blocking_notifier_head head;
    struct list_head dev_list;
    struct list_head opp_list;
    struct kref kref;
    struct mutex lock;
    struct device_node *np;
    long unsigned int clock_latency_ns_max;
    unsigned int voltage_tolerance_v1;
    enum opp_table_access shared_opp;
    struct dev_pm_opp *suspend_opp;
    unsigned int *supported_hw;
    unsigned int supported_hw_count;
    const char *prop_name;
    struct clk *clk;
    struct regulator **regulators;
    unsigned int regulator_count;
    bool genpd_performance_state;
    int (*set_opp)(struct dev_pm_set_opp_data *);
    struct dev_pm_set_opp_data *set_opp_data;
    int (*get_pstate)(struct device *, long unsigned int);
    struct dentry *dentry;
    char dentry_name[255];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct opp_table {
    struct list_head node;
    struct blocking_notifier_head head;
    struct list_head dev_list;
    struct list_head opp_list;
    struct kref kref;
    struct mutex lock;
    struct device_node *np;
    long unsigned int clock_latency_ns_max;
    unsigned int voltage_tolerance_v1;
    enum opp_table_access shared_opp;
    struct dev_pm_opp *suspend_opp;
    unsigned int *supported_hw;
    unsigned int supported_hw_count;
    const char *prop_name;
    struct clk *clk;
    struct regulator **regulators;
    unsigned int regulator_count;
    bool genpd_performance_state;
    int (*set_opp)(struct dev_pm_set_opp_data *);
    struct dev_pm_set_opp_data *set_opp_data;
    struct dentry *dentry;
    char dentry_name[255];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct opp_table {
    struct list_head node;
    struct blocking_notifier_head head;
    struct list_head dev_list;
    struct list_head opp_list;
    struct kref kref;
    struct kref list_kref;
    struct mutex lock;
    struct device_node *np;
    long unsigned int clock_latency_ns_max;
    unsigned int voltage_tolerance_v1;
    bool parsed_static_opps;
    enum opp_table_access shared_opp;
    struct dev_pm_opp *suspend_opp;
    struct mutex genpd_virt_dev_lock;
    struct device **genpd_virt_devs;
    struct opp_table **required_opp_tables;
    unsigned int required_opp_count;
    unsigned int *supported_hw;
    unsigned int supported_hw_count;
    const char *prop_name;
    struct clk *clk;
    struct regulator **regulators;
    int regulator_count;
    bool genpd_performance_state;
    bool is_genpd;
    int (*set_opp)(struct dev_pm_set_opp_data *);
    struct dev_pm_set_opp_data *set_opp_data;
    struct dentry *dentry;
    char dentry_name[255];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct opp_table {
    struct list_head node;
    struct blocking_notifier_head head;
    struct list_head dev_list;
    struct list_head opp_list;
    struct kref kref;
    struct kref list_kref;
    struct mutex lock;
    struct device_node *np;
    long unsigned int clock_latency_ns_max;
    unsigned int voltage_tolerance_v1;
    bool parsed_static_opps;
    enum opp_table_access shared_opp;
    struct dev_pm_opp *suspend_opp;
    struct mutex genpd_virt_dev_lock;
    struct device **genpd_virt_devs;
    struct opp_table **required_opp_tables;
    unsigned int required_opp_count;
    unsigned int *supported_hw;
    unsigned int supported_hw_count;
    const char *prop_name;
    struct clk *clk;
    struct regulator **regulators;
    int regulator_count;
    bool genpd_performance_state;
    bool is_genpd;
    int (*set_opp)(struct dev_pm_set_opp_data *);
    struct dev_pm_set_opp_data *set_opp_data;
    struct dentry *dentry;
    char dentry_name[255];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct opp_table {
    struct list_head node;
    struct blocking_notifier_head head;
    struct list_head dev_list;
    struct list_head opp_list;
    struct kref kref;
    struct kref list_kref;
    struct mutex lock;
    struct device_node *np;
    long unsigned int clock_latency_ns_max;
    unsigned int voltage_tolerance_v1;
    bool parsed_static_opps;
    enum opp_table_access shared_opp;
    struct dev_pm_opp *suspend_opp;
    struct mutex genpd_virt_dev_lock;
    struct device **genpd_virt_devs;
    struct opp_table **required_opp_tables;
    unsigned int required_opp_count;
    unsigned int *supported_hw;
    unsigned int supported_hw_count;
    const char *prop_name;
    struct clk *clk;
    struct regulator **regulators;
    int regulator_count;
    bool genpd_performance_state;
    bool is_genpd;
    int (*set_opp)(struct dev_pm_set_opp_data *);
    struct dev_pm_set_opp_data *set_opp_data;
    struct dentry *dentry;
    char dentry_name[255];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct opp_table {
    struct list_head node;
    struct blocking_notifier_head head;
    struct list_head dev_list;
    struct list_head opp_list;
    struct kref kref;
    struct mutex lock;
    struct device_node *np;
    long unsigned int clock_latency_ns_max;
    unsigned int voltage_tolerance_v1;
    unsigned int parsed_static_opps;
    enum opp_table_access shared_opp;
    struct dev_pm_opp *suspend_opp;
    struct mutex genpd_virt_dev_lock;
    struct device **genpd_virt_devs;
    struct opp_table **required_opp_tables;
    unsigned int required_opp_count;
    unsigned int *supported_hw;
    unsigned int supported_hw_count;
    const char *prop_name;
    struct clk *clk;
    struct regulator **regulators;
    int regulator_count;
    bool regulator_enabled;
    struct icc_path **paths;
    unsigned int path_count;
    bool genpd_performance_state;
    bool is_genpd;
    int (*set_opp)(struct dev_pm_set_opp_data *);
    struct dev_pm_set_opp_data *set_opp_data;
    struct dentry *dentry;
    char dentry_name[255];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct opp_table {
    struct list_head node;
    struct blocking_notifier_head head;
    struct list_head dev_list;
    struct list_head opp_list;
    struct kref kref;
    struct mutex lock;
    struct device_node *np;
    long unsigned int clock_latency_ns_max;
    unsigned int voltage_tolerance_v1;
    unsigned int parsed_static_opps;
    enum opp_table_access shared_opp;
    struct dev_pm_opp *suspend_opp;
    struct mutex genpd_virt_dev_lock;
    struct device **genpd_virt_devs;
    struct opp_table **required_opp_tables;
    unsigned int required_opp_count;
    unsigned int *supported_hw;
    unsigned int supported_hw_count;
    const char *prop_name;
    struct clk *clk;
    struct regulator **regulators;
    int regulator_count;
    struct icc_path **paths;
    unsigned int path_count;
    bool enabled;
    bool genpd_performance_state;
    bool is_genpd;
    int (*set_opp)(struct dev_pm_set_opp_data *);
    struct dev_pm_set_opp_data *set_opp_data;
    struct dentry *dentry;
    char dentry_name[255];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct opp_table {
    struct list_head node;
    struct list_head lazy;
    struct blocking_notifier_head head;
    struct list_head dev_list;
    struct list_head opp_list;
    struct kref kref;
    struct mutex lock;
    struct device_node *np;
    long unsigned int clock_latency_ns_max;
    unsigned int voltage_tolerance_v1;
    unsigned int parsed_static_opps;
    enum opp_table_access shared_opp;
    long unsigned int current_rate;
    struct dev_pm_opp *current_opp;
    struct dev_pm_opp *suspend_opp;
    struct mutex genpd_virt_dev_lock;
    struct device **genpd_virt_devs;
    struct opp_table **required_opp_tables;
    unsigned int required_opp_count;
    unsigned int *supported_hw;
    unsigned int supported_hw_count;
    const char *prop_name;
    struct clk *clk;
    struct regulator **regulators;
    int regulator_count;
    struct icc_path **paths;
    unsigned int path_count;
    bool enabled;
    bool genpd_performance_state;
    bool is_genpd;
    int (*set_opp)(struct dev_pm_set_opp_data *);
    struct dev_pm_opp_supply *sod_supplies;
    struct dev_pm_set_opp_data *set_opp_data;
    struct dentry *dentry;
    char dentry_name[255];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct opp_table {
    struct list_head node;
    struct list_head lazy;
    struct blocking_notifier_head head;
    struct list_head dev_list;
    struct list_head opp_list;
    struct kref kref;
    struct mutex lock;
    struct device_node *np;
    long unsigned int clock_latency_ns_max;
    unsigned int voltage_tolerance_v1;
    unsigned int parsed_static_opps;
    enum opp_table_access shared_opp;
    long unsigned int current_rate;
    struct dev_pm_opp *current_opp;
    struct dev_pm_opp *suspend_opp;
    struct mutex genpd_virt_dev_lock;
    struct device **genpd_virt_devs;
    struct opp_table **required_opp_tables;
    unsigned int required_opp_count;
    unsigned int *supported_hw;
    unsigned int supported_hw_count;
    const char *prop_name;
    struct clk *clk;
    struct regulator **regulators;
    int regulator_count;
    struct icc_path **paths;
    unsigned int path_count;
    bool enabled;
    bool genpd_performance_state;
    bool is_genpd;
    int (*set_opp)(struct dev_pm_set_opp_data *);
    struct dev_pm_opp_supply *sod_supplies;
    struct dev_pm_set_opp_data *set_opp_data;
    struct dentry *dentry;
    char dentry_name[255];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct opp_table {
    struct list_head node;
    struct list_head lazy;
    struct blocking_notifier_head head;
    struct list_head dev_list;
    struct list_head opp_list;
    struct kref kref;
    struct mutex lock;
    struct device_node *np;
    long unsigned int clock_latency_ns_max;
    unsigned int voltage_tolerance_v1;
    unsigned int parsed_static_opps;
    enum opp_table_access shared_opp;
    long unsigned int current_rate;
    struct dev_pm_opp *current_opp;
    struct dev_pm_opp *suspend_opp;
    struct mutex genpd_virt_dev_lock;
    struct device **genpd_virt_devs;
    struct opp_table **required_opp_tables;
    unsigned int required_opp_count;
    unsigned int *supported_hw;
    unsigned int supported_hw_count;
    const char *prop_name;
    struct clk *clk;
    struct regulator **regulators;
    int regulator_count;
    struct icc_path **paths;
    unsigned int path_count;
    bool enabled;
    bool genpd_performance_state;
    bool is_genpd;
    int (*set_opp)(struct dev_pm_set_opp_data *);
    struct dev_pm_opp_supply *sod_supplies;
    struct dev_pm_set_opp_data *set_opp_data;
    struct dentry *dentry;
    char dentry_name[255];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct opp_table {
    struct list_head node;
    struct list_head lazy;
    struct blocking_notifier_head head;
    struct list_head dev_list;
    struct list_head opp_list;
    struct kref kref;
    struct mutex lock;
    struct device_node *np;
    long unsigned int clock_latency_ns_max;
    unsigned int voltage_tolerance_v1;
    unsigned int parsed_static_opps;
    enum opp_table_access shared_opp;
    long unsigned int rate_clk_single;
    struct dev_pm_opp *current_opp;
    struct dev_pm_opp *suspend_opp;
    struct mutex genpd_virt_dev_lock;
    struct device **genpd_virt_devs;
    struct opp_table **required_opp_tables;
    unsigned int required_opp_count;
    unsigned int *supported_hw;
    unsigned int supported_hw_count;
    const char *prop_name;
    config_clks_t config_clks;
    struct clk **clks;
    struct clk *clk;
    int clk_count;
    config_regulators_t config_regulators;
    struct regulator **regulators;
    int regulator_count;
    struct icc_path **paths;
    unsigned int path_count;
    bool enabled;
    bool genpd_performance_state;
    bool is_genpd;
    struct dentry *dentry;
    char dentry_name[255];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct opp_table {
    struct list_head node;
    struct list_head lazy;
    struct blocking_notifier_head head;
    struct list_head dev_list;
    struct list_head opp_list;
    struct kref kref;
    struct mutex lock;
    struct device_node *np;
    long unsigned int clock_latency_ns_max;
    unsigned int voltage_tolerance_v1;
    unsigned int parsed_static_opps;
    enum opp_table_access shared_opp;
    long unsigned int rate_clk_single;
    struct dev_pm_opp *current_opp;
    struct dev_pm_opp *suspend_opp;
    struct mutex genpd_virt_dev_lock;
    struct device **genpd_virt_devs;
    struct opp_table **required_opp_tables;
    unsigned int required_opp_count;
    unsigned int *supported_hw;
    unsigned int supported_hw_count;
    const char *prop_name;
    config_clks_t config_clks;
    struct clk **clks;
    struct clk *clk;
    int clk_count;
    config_regulators_t config_regulators;
    struct regulator **regulators;
    int regulator_count;
    struct icc_path **paths;
    unsigned int path_count;
    bool enabled;
    bool is_genpd;
    int (*set_required_opps)(struct device *, struct opp_table *, struct dev_pm_opp *, bool);
    struct dentry *dentry;
    char dentry_name[255];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct opp_table {
    struct list_head node;
    struct list_head lazy;
    struct blocking_notifier_head head;
    struct list_head dev_list;
    struct list_head opp_list;
    struct kref kref;
    struct mutex lock;
    struct device_node *np;
    long unsigned int clock_latency_ns_max;
    unsigned int voltage_tolerance_v1;
    unsigned int parsed_static_opps;
    enum opp_table_access shared_opp;
    long unsigned int current_rate_single_clk;
    struct dev_pm_opp *current_opp;
    struct dev_pm_opp *suspend_opp;
    struct opp_table **required_opp_tables;
    struct device **required_devs;
    unsigned int required_opp_count;
    unsigned int *supported_hw;
    unsigned int supported_hw_count;
    const char *prop_name;
    config_clks_t config_clks;
    struct clk **clks;
    struct clk *clk;
    int clk_count;
    config_regulators_t config_regulators;
    struct regulator **regulators;
    int regulator_count;
    struct icc_path **paths;
    unsigned int path_count;
    bool enabled;
    bool is_genpd;
    struct dentry *dentry;
    char dentry_name[255];
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
struct opp_table {
    struct list_head node;
    struct blocking_notifier_head head;
    struct list_head dev_list;
    struct list_head opp_list;
    struct kref kref;
    struct kref list_kref;
    struct mutex lock;
    struct device_node *np;
    long unsigned int clock_latency_ns_max;
    unsigned int voltage_tolerance_v1;
    bool parsed_static_opps;
    enum opp_table_access shared_opp;
    struct dev_pm_opp *suspend_opp;
    struct mutex genpd_virt_dev_lock;
    struct device **genpd_virt_devs;
    struct opp_table **required_opp_tables;
    unsigned int required_opp_count;
    unsigned int *supported_hw;
    unsigned int supported_hw_count;
    const char *prop_name;
    struct clk *clk;
    struct regulator **regulators;
    int regulator_count;
    bool genpd_performance_state;
    bool is_genpd;
    int (*set_opp)(struct dev_pm_set_opp_data *);
    struct dev_pm_set_opp_data *set_opp_data;
    struct dentry *dentry;
    char dentry_name[255];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct opp_table {
    struct list_head node;
    struct blocking_notifier_head head;
    struct list_head dev_list;
    struct list_head opp_list;
    struct kref kref;
    struct kref list_kref;
    struct mutex lock;
    struct device_node *np;
    long unsigned int clock_latency_ns_max;
    unsigned int voltage_tolerance_v1;
    bool parsed_static_opps;
    enum opp_table_access shared_opp;
    struct dev_pm_opp *suspend_opp;
    struct mutex genpd_virt_dev_lock;
    struct device **genpd_virt_devs;
    struct opp_table **required_opp_tables;
    unsigned int required_opp_count;
    unsigned int *supported_hw;
    unsigned int supported_hw_count;
    const char *prop_name;
    struct clk *clk;
    struct regulator **regulators;
    int regulator_count;
    bool genpd_performance_state;
    bool is_genpd;
    int (*set_opp)(struct dev_pm_set_opp_data *);
    struct dev_pm_set_opp_data *set_opp_data;
    struct dentry *dentry;
    char dentry_name[255];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct opp_table {
    struct list_head node;
    struct blocking_notifier_head head;
    struct list_head dev_list;
    struct list_head opp_list;
    struct kref kref;
    struct kref list_kref;
    struct mutex lock;
    struct device_node *np;
    long unsigned int clock_latency_ns_max;
    unsigned int voltage_tolerance_v1;
    bool parsed_static_opps;
    enum opp_table_access shared_opp;
    struct dev_pm_opp *suspend_opp;
    struct mutex genpd_virt_dev_lock;
    struct device **genpd_virt_devs;
    struct opp_table **required_opp_tables;
    unsigned int required_opp_count;
    unsigned int *supported_hw;
    unsigned int supported_hw_count;
    const char *prop_name;
    struct clk *clk;
    struct regulator **regulators;
    int regulator_count;
    bool genpd_performance_state;
    bool is_genpd;
    int (*set_opp)(struct dev_pm_set_opp_data *);
    struct dev_pm_set_opp_data *set_opp_data;
    struct dentry *dentry;
    char dentry_name[255];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct opp_table {
    struct list_head node;
    struct blocking_notifier_head head;
    struct list_head dev_list;
    struct list_head opp_list;
    struct kref kref;
    struct kref list_kref;
    struct mutex lock;
    struct device_node *np;
    long unsigned int clock_latency_ns_max;
    unsigned int voltage_tolerance_v1;
    bool parsed_static_opps;
    enum opp_table_access shared_opp;
    struct dev_pm_opp *suspend_opp;
    struct mutex genpd_virt_dev_lock;
    struct device **genpd_virt_devs;
    struct opp_table **required_opp_tables;
    unsigned int required_opp_count;
    unsigned int *supported_hw;
    unsigned int supported_hw_count;
    const char *prop_name;
    struct clk *clk;
    struct regulator **regulators;
    int regulator_count;
    bool genpd_performance_state;
    bool is_genpd;
    int (*set_opp)(struct dev_pm_set_opp_data *);
    struct dev_pm_set_opp_data *set_opp_data;
    struct dentry *dentry;
    char dentry_name[255];
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
struct opp_table {
    struct list_head node;
    struct blocking_notifier_head head;
    struct list_head dev_list;
    struct list_head opp_list;
    struct kref kref;
    struct kref list_kref;
    struct mutex lock;
    struct device_node *np;
    long unsigned int clock_latency_ns_max;
    unsigned int voltage_tolerance_v1;
    bool parsed_static_opps;
    enum opp_table_access shared_opp;
    struct dev_pm_opp *suspend_opp;
    struct mutex genpd_virt_dev_lock;
    struct device **genpd_virt_devs;
    struct opp_table **required_opp_tables;
    unsigned int required_opp_count;
    unsigned int *supported_hw;
    unsigned int supported_hw_count;
    const char *prop_name;
    struct clk *clk;
    struct regulator **regulators;
    int regulator_count;
    bool genpd_performance_state;
    bool is_genpd;
    int (*set_opp)(struct dev_pm_set_opp_data *);
    struct dev_pm_set_opp_data *set_opp_data;
    struct dentry *dentry;
    char dentry_name[255];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct opp_table {
    struct list_head node;
    struct blocking_notifier_head head;
    struct list_head dev_list;
    struct list_head opp_list;
    struct kref kref;
    struct kref list_kref;
    struct mutex lock;
    struct device_node *np;
    long unsigned int clock_latency_ns_max;
    unsigned int voltage_tolerance_v1;
    bool parsed_static_opps;
    enum opp_table_access shared_opp;
    struct dev_pm_opp *suspend_opp;
    struct mutex genpd_virt_dev_lock;
    struct device **genpd_virt_devs;
    struct opp_table **required_opp_tables;
    unsigned int required_opp_count;
    unsigned int *supported_hw;
    unsigned int supported_hw_count;
    const char *prop_name;
    struct clk *clk;
    struct regulator **regulators;
    int regulator_count;
    bool genpd_performance_state;
    bool is_genpd;
    int (*set_opp)(struct dev_pm_set_opp_data *);
    struct dev_pm_set_opp_data *set_opp_data;
    struct dentry *dentry;
    char dentry_name[255];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct opp_table {
    struct list_head node;
    struct blocking_notifier_head head;
    struct list_head dev_list;
    struct list_head opp_list;
    struct kref kref;
    struct kref list_kref;
    struct mutex lock;
    struct device_node *np;
    long unsigned int clock_latency_ns_max;
    unsigned int voltage_tolerance_v1;
    bool parsed_static_opps;
    enum opp_table_access shared_opp;
    struct dev_pm_opp *suspend_opp;
    struct mutex genpd_virt_dev_lock;
    struct device **genpd_virt_devs;
    struct opp_table **required_opp_tables;
    unsigned int required_opp_count;
    unsigned int *supported_hw;
    unsigned int supported_hw_count;
    const char *prop_name;
    struct clk *clk;
    struct regulator **regulators;
    int regulator_count;
    bool genpd_performance_state;
    bool is_genpd;
    int (*set_opp)(struct dev_pm_set_opp_data *);
    struct dev_pm_set_opp_data *set_opp_data;
    struct dentry *dentry;
    char dentry_name[255];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct opp_table {
    struct list_head node;
    struct blocking_notifier_head head;
    struct list_head dev_list;
    struct list_head opp_list;
    struct kref kref;
    struct kref list_kref;
    struct mutex lock;
    struct device_node *np;
    long unsigned int clock_latency_ns_max;
    unsigned int voltage_tolerance_v1;
    bool parsed_static_opps;
    enum opp_table_access shared_opp;
    struct dev_pm_opp *suspend_opp;
    struct mutex genpd_virt_dev_lock;
    struct device **genpd_virt_devs;
    struct opp_table **required_opp_tables;
    unsigned int required_opp_count;
    unsigned int *supported_hw;
    unsigned int supported_hw_count;
    const char *prop_name;
    struct clk *clk;
    struct regulator **regulators;
    int regulator_count;
    bool genpd_performance_state;
    bool is_genpd;
    int (*set_opp)(struct dev_pm_set_opp_data *);
    struct dev_pm_set_opp_data *set_opp_data;
    struct dentry *dentry;
    char dentry_name[255];
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
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*get_pstate)(struct device *, long unsigned int)</code>
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
<code>struct kref list_kref</code>
</li>
<li>
<b>Field added. </b>
<code>bool parsed_static_opps</code>
</li>
<li>
<b>Field added. </b>
<code>struct mutex genpd_virt_dev_lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct device **genpd_virt_devs</code>
</li>
<li>
<b>Field added. </b>
<code>struct opp_table **required_opp_tables</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int required_opp_count</code>
</li>
<li>
<b>Field added. </b>
<code>bool is_genpd</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int regulator_count</code> ➡️ <code>int regulator_count</code>
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
<code>bool regulator_enabled</code>
</li>
<li>
<b>Field added. </b>
<code>struct icc_path **paths</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int path_count</code>
</li>
<li>
<b>Field removed. </b>
<code>struct kref list_kref</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool parsed_static_opps</code> ➡️ <code>unsigned int parsed_static_opps</code>
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
<code>bool enabled</code>
</li>
<li>
<b>Field removed. </b>
<code>bool regulator_enabled</code>
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
<code>struct list_head lazy</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int current_rate</code>
</li>
<li>
<b>Field added. </b>
<code>struct dev_pm_opp *current_opp</code>
</li>
<li>
<b>Field added. </b>
<code>struct dev_pm_opp_supply *sod_supplies</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int rate_clk_single</code>
</li>
<li>
<b>Field added. </b>
<code>config_clks_t config_clks</code>
</li>
<li>
<b>Field added. </b>
<code>struct clk **clks</code>
</li>
<li>
<b>Field added. </b>
<code>int clk_count</code>
</li>
<li>
<b>Field added. </b>
<code>config_regulators_t config_regulators</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int current_rate</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*set_opp)(struct dev_pm_set_opp_data *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct dev_pm_opp_supply *sod_supplies</code>
</li>
<li>
<b>Field removed. </b>
<code>struct dev_pm_set_opp_data *set_opp_data</code>
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
<code>int (*set_required_opps)(struct device *, struct opp_table *, struct dev_pm_opp *, bool)</code>
</li>
<li>
<b>Field removed. </b>
<code>bool genpd_performance_state</code>
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
<code>long unsigned int current_rate_single_clk</code>
</li>
<li>
<b>Field added. </b>
<code>struct device **required_devs</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int rate_clk_single</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mutex genpd_virt_dev_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>struct device **genpd_virt_devs</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*set_required_opps)(struct device *, struct opp_table *, struct dev_pm_opp *, bool)</code>
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
