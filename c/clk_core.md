# Struct: <code>clk_core</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct clk_core {
    const char *name;
    const struct clk_ops *ops;
    struct clk_hw *hw;
    struct module *owner;
    struct clk_core *parent;
    const char **parent_names;
    struct clk_core **parents;
    u8 num_parents;
    u8 new_parent_index;
    long unsigned int rate;
    long unsigned int req_rate;
    long unsigned int new_rate;
    struct clk_core *new_parent;
    struct clk_core *new_child;
    long unsigned int flags;
    bool orphan;
    unsigned int enable_count;
    unsigned int prepare_count;
    long unsigned int min_rate;
    long unsigned int max_rate;
    long unsigned int accuracy;
    int phase;
    struct hlist_head children;
    struct hlist_node child_node;
    struct hlist_head clks;
    unsigned int notifier_count;
    struct dentry *dentry;
    struct hlist_node debug_node;
    struct kref ref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct clk_core {
    const char *name;
    const struct clk_ops *ops;
    struct clk_hw *hw;
    struct module *owner;
    struct clk_core *parent;
    const char **parent_names;
    struct clk_core **parents;
    u8 num_parents;
    u8 new_parent_index;
    long unsigned int rate;
    long unsigned int req_rate;
    long unsigned int new_rate;
    struct clk_core *new_parent;
    struct clk_core *new_child;
    long unsigned int flags;
    bool orphan;
    unsigned int enable_count;
    unsigned int prepare_count;
    long unsigned int min_rate;
    long unsigned int max_rate;
    long unsigned int accuracy;
    int phase;
    struct hlist_head children;
    struct hlist_node child_node;
    struct hlist_head clks;
    unsigned int notifier_count;
    struct dentry *dentry;
    struct hlist_node debug_node;
    struct kref ref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct clk_core {
    const char *name;
    const struct clk_ops *ops;
    struct clk_hw *hw;
    struct module *owner;
    struct clk_core *parent;
    const char **parent_names;
    struct clk_core **parents;
    u8 num_parents;
    u8 new_parent_index;
    long unsigned int rate;
    long unsigned int req_rate;
    long unsigned int new_rate;
    struct clk_core *new_parent;
    struct clk_core *new_child;
    long unsigned int flags;
    bool orphan;
    unsigned int enable_count;
    unsigned int prepare_count;
    long unsigned int min_rate;
    long unsigned int max_rate;
    long unsigned int accuracy;
    int phase;
    struct hlist_head children;
    struct hlist_node child_node;
    struct hlist_head clks;
    unsigned int notifier_count;
    struct dentry *dentry;
    struct hlist_node debug_node;
    struct kref ref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct clk_core {
    const char *name;
    const struct clk_ops *ops;
    struct clk_hw *hw;
    struct module *owner;
    struct clk_core *parent;
    const char **parent_names;
    struct clk_core **parents;
    u8 num_parents;
    u8 new_parent_index;
    long unsigned int rate;
    long unsigned int req_rate;
    long unsigned int new_rate;
    struct clk_core *new_parent;
    struct clk_core *new_child;
    long unsigned int flags;
    bool orphan;
    unsigned int enable_count;
    unsigned int prepare_count;
    long unsigned int min_rate;
    long unsigned int max_rate;
    long unsigned int accuracy;
    int phase;
    struct hlist_head children;
    struct hlist_node child_node;
    struct hlist_head clks;
    unsigned int notifier_count;
    struct dentry *dentry;
    struct hlist_node debug_node;
    struct kref ref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct clk_core {
    const char *name;
    const struct clk_ops *ops;
    struct clk_hw *hw;
    struct module *owner;
    struct device *dev;
    struct clk_core *parent;
    const char **parent_names;
    struct clk_core **parents;
    u8 num_parents;
    u8 new_parent_index;
    long unsigned int rate;
    long unsigned int req_rate;
    long unsigned int new_rate;
    struct clk_core *new_parent;
    struct clk_core *new_child;
    long unsigned int flags;
    bool orphan;
    unsigned int enable_count;
    unsigned int prepare_count;
    long unsigned int min_rate;
    long unsigned int max_rate;
    long unsigned int accuracy;
    int phase;
    struct hlist_head children;
    struct hlist_node child_node;
    struct hlist_head clks;
    unsigned int notifier_count;
    struct dentry *dentry;
    struct hlist_node debug_node;
    struct kref ref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct clk_core {
    const char *name;
    const struct clk_ops *ops;
    struct clk_hw *hw;
    struct module *owner;
    struct device *dev;
    struct clk_core *parent;
    const char **parent_names;
    struct clk_core **parents;
    u8 num_parents;
    u8 new_parent_index;
    long unsigned int rate;
    long unsigned int req_rate;
    long unsigned int new_rate;
    struct clk_core *new_parent;
    struct clk_core *new_child;
    long unsigned int flags;
    bool orphan;
    unsigned int enable_count;
    unsigned int prepare_count;
    unsigned int protect_count;
    long unsigned int min_rate;
    long unsigned int max_rate;
    long unsigned int accuracy;
    int phase;
    struct hlist_head children;
    struct hlist_node child_node;
    struct hlist_head clks;
    unsigned int notifier_count;
    struct dentry *dentry;
    struct hlist_node debug_node;
    struct kref ref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct clk_core {
    const char *name;
    const struct clk_ops *ops;
    struct clk_hw *hw;
    struct module *owner;
    struct device *dev;
    struct clk_core *parent;
    const char **parent_names;
    struct clk_core **parents;
    u8 num_parents;
    u8 new_parent_index;
    long unsigned int rate;
    long unsigned int req_rate;
    long unsigned int new_rate;
    struct clk_core *new_parent;
    struct clk_core *new_child;
    long unsigned int flags;
    bool orphan;
    unsigned int enable_count;
    unsigned int prepare_count;
    unsigned int protect_count;
    long unsigned int min_rate;
    long unsigned int max_rate;
    long unsigned int accuracy;
    int phase;
    struct clk_duty duty;
    struct hlist_head children;
    struct hlist_node child_node;
    struct hlist_head clks;
    unsigned int notifier_count;
    struct dentry *dentry;
    struct hlist_node debug_node;
    struct kref ref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct clk_core {
    const char *name;
    const struct clk_ops *ops;
    struct clk_hw *hw;
    struct module *owner;
    struct device *dev;
    struct device_node *of_node;
    struct clk_core *parent;
    struct clk_parent_map *parents;
    u8 num_parents;
    u8 new_parent_index;
    long unsigned int rate;
    long unsigned int req_rate;
    long unsigned int new_rate;
    struct clk_core *new_parent;
    struct clk_core *new_child;
    long unsigned int flags;
    bool orphan;
    bool rpm_enabled;
    unsigned int enable_count;
    unsigned int prepare_count;
    unsigned int protect_count;
    long unsigned int min_rate;
    long unsigned int max_rate;
    long unsigned int accuracy;
    int phase;
    struct clk_duty duty;
    struct hlist_head children;
    struct hlist_node child_node;
    struct hlist_head clks;
    unsigned int notifier_count;
    struct dentry *dentry;
    struct hlist_node debug_node;
    struct kref ref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct clk_core {
    const char *name;
    const struct clk_ops *ops;
    struct clk_hw *hw;
    struct module *owner;
    struct device *dev;
    struct device_node *of_node;
    struct clk_core *parent;
    struct clk_parent_map *parents;
    u8 num_parents;
    u8 new_parent_index;
    long unsigned int rate;
    long unsigned int req_rate;
    long unsigned int new_rate;
    struct clk_core *new_parent;
    struct clk_core *new_child;
    long unsigned int flags;
    bool orphan;
    bool rpm_enabled;
    unsigned int enable_count;
    unsigned int prepare_count;
    unsigned int protect_count;
    long unsigned int min_rate;
    long unsigned int max_rate;
    long unsigned int accuracy;
    int phase;
    struct clk_duty duty;
    struct hlist_head children;
    struct hlist_node child_node;
    struct hlist_head clks;
    unsigned int notifier_count;
    struct dentry *dentry;
    struct hlist_node debug_node;
    struct kref ref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct clk_core {
    const char *name;
    const struct clk_ops *ops;
    struct clk_hw *hw;
    struct module *owner;
    struct device *dev;
    struct device_node *of_node;
    struct clk_core *parent;
    struct clk_parent_map *parents;
    u8 num_parents;
    u8 new_parent_index;
    long unsigned int rate;
    long unsigned int req_rate;
    long unsigned int new_rate;
    struct clk_core *new_parent;
    struct clk_core *new_child;
    long unsigned int flags;
    bool orphan;
    bool rpm_enabled;
    unsigned int enable_count;
    unsigned int prepare_count;
    unsigned int protect_count;
    long unsigned int min_rate;
    long unsigned int max_rate;
    long unsigned int accuracy;
    int phase;
    struct clk_duty duty;
    struct hlist_head children;
    struct hlist_node child_node;
    struct hlist_head clks;
    unsigned int notifier_count;
    struct dentry *dentry;
    struct hlist_node debug_node;
    struct kref ref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct clk_core {
    const char *name;
    const struct clk_ops *ops;
    struct clk_hw *hw;
    struct module *owner;
    struct device *dev;
    struct device_node *of_node;
    struct clk_core *parent;
    struct clk_parent_map *parents;
    u8 num_parents;
    u8 new_parent_index;
    long unsigned int rate;
    long unsigned int req_rate;
    long unsigned int new_rate;
    struct clk_core *new_parent;
    struct clk_core *new_child;
    long unsigned int flags;
    bool orphan;
    bool rpm_enabled;
    unsigned int enable_count;
    unsigned int prepare_count;
    unsigned int protect_count;
    long unsigned int min_rate;
    long unsigned int max_rate;
    long unsigned int accuracy;
    int phase;
    struct clk_duty duty;
    struct hlist_head children;
    struct hlist_node child_node;
    struct hlist_head clks;
    unsigned int notifier_count;
    struct dentry *dentry;
    struct hlist_node debug_node;
    struct kref ref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct clk_core {
    const char *name;
    const struct clk_ops *ops;
    struct clk_hw *hw;
    struct module *owner;
    struct device *dev;
    struct device_node *of_node;
    struct clk_core *parent;
    struct clk_parent_map *parents;
    u8 num_parents;
    u8 new_parent_index;
    long unsigned int rate;
    long unsigned int req_rate;
    long unsigned int new_rate;
    struct clk_core *new_parent;
    struct clk_core *new_child;
    long unsigned int flags;
    bool orphan;
    bool rpm_enabled;
    unsigned int enable_count;
    unsigned int prepare_count;
    unsigned int protect_count;
    long unsigned int min_rate;
    long unsigned int max_rate;
    long unsigned int accuracy;
    int phase;
    struct clk_duty duty;
    struct hlist_head children;
    struct hlist_node child_node;
    struct hlist_head clks;
    unsigned int notifier_count;
    struct dentry *dentry;
    struct hlist_node debug_node;
    struct kref ref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct clk_core {
    const char *name;
    const struct clk_ops *ops;
    struct clk_hw *hw;
    struct module *owner;
    struct device *dev;
    struct device_node *of_node;
    struct clk_core *parent;
    struct clk_parent_map *parents;
    u8 num_parents;
    u8 new_parent_index;
    long unsigned int rate;
    long unsigned int req_rate;
    long unsigned int new_rate;
    struct clk_core *new_parent;
    struct clk_core *new_child;
    long unsigned int flags;
    bool orphan;
    bool rpm_enabled;
    unsigned int enable_count;
    unsigned int prepare_count;
    unsigned int protect_count;
    long unsigned int min_rate;
    long unsigned int max_rate;
    long unsigned int accuracy;
    int phase;
    struct clk_duty duty;
    struct hlist_head children;
    struct hlist_node child_node;
    struct hlist_head clks;
    unsigned int notifier_count;
    struct dentry *dentry;
    struct hlist_node debug_node;
    struct kref ref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct clk_core {
    const char *name;
    const struct clk_ops *ops;
    struct clk_hw *hw;
    struct module *owner;
    struct device *dev;
    struct device_node *of_node;
    struct clk_core *parent;
    struct clk_parent_map *parents;
    u8 num_parents;
    u8 new_parent_index;
    long unsigned int rate;
    long unsigned int req_rate;
    long unsigned int new_rate;
    struct clk_core *new_parent;
    struct clk_core *new_child;
    long unsigned int flags;
    bool orphan;
    bool rpm_enabled;
    unsigned int enable_count;
    unsigned int prepare_count;
    unsigned int protect_count;
    long unsigned int min_rate;
    long unsigned int max_rate;
    long unsigned int accuracy;
    int phase;
    struct clk_duty duty;
    struct hlist_head children;
    struct hlist_node child_node;
    struct hlist_head clks;
    unsigned int notifier_count;
    struct dentry *dentry;
    struct hlist_node debug_node;
    struct kref ref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct clk_core {
    const char *name;
    const struct clk_ops *ops;
    struct clk_hw *hw;
    struct module *owner;
    struct device *dev;
    struct device_node *of_node;
    struct clk_core *parent;
    struct clk_parent_map *parents;
    u8 num_parents;
    u8 new_parent_index;
    long unsigned int rate;
    long unsigned int req_rate;
    long unsigned int new_rate;
    struct clk_core *new_parent;
    struct clk_core *new_child;
    long unsigned int flags;
    bool orphan;
    bool rpm_enabled;
    unsigned int enable_count;
    unsigned int prepare_count;
    unsigned int protect_count;
    long unsigned int min_rate;
    long unsigned int max_rate;
    long unsigned int accuracy;
    int phase;
    struct clk_duty duty;
    struct hlist_head children;
    struct hlist_node child_node;
    struct hlist_head clks;
    unsigned int notifier_count;
    struct dentry *dentry;
    struct hlist_node debug_node;
    struct kref ref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct clk_core {
    const char *name;
    const struct clk_ops *ops;
    struct clk_hw *hw;
    struct module *owner;
    struct device *dev;
    struct device_node *of_node;
    struct clk_core *parent;
    struct clk_parent_map *parents;
    u8 num_parents;
    u8 new_parent_index;
    long unsigned int rate;
    long unsigned int req_rate;
    long unsigned int new_rate;
    struct clk_core *new_parent;
    struct clk_core *new_child;
    long unsigned int flags;
    bool orphan;
    bool rpm_enabled;
    unsigned int enable_count;
    unsigned int prepare_count;
    unsigned int protect_count;
    long unsigned int min_rate;
    long unsigned int max_rate;
    long unsigned int accuracy;
    int phase;
    struct clk_duty duty;
    struct hlist_head children;
    struct hlist_node child_node;
    struct hlist_head clks;
    unsigned int notifier_count;
    struct dentry *dentry;
    struct hlist_node debug_node;
    struct kref ref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct clk_core {
    const char *name;
    const struct clk_ops *ops;
    struct clk_hw *hw;
    struct module *owner;
    struct device *dev;
    struct device_node *of_node;
    struct clk_core *parent;
    struct clk_parent_map *parents;
    u8 num_parents;
    u8 new_parent_index;
    long unsigned int rate;
    long unsigned int req_rate;
    long unsigned int new_rate;
    struct clk_core *new_parent;
    struct clk_core *new_child;
    long unsigned int flags;
    bool orphan;
    bool rpm_enabled;
    unsigned int enable_count;
    unsigned int prepare_count;
    unsigned int protect_count;
    long unsigned int min_rate;
    long unsigned int max_rate;
    long unsigned int accuracy;
    int phase;
    struct clk_duty duty;
    struct hlist_head children;
    struct hlist_node child_node;
    struct hlist_head clks;
    unsigned int notifier_count;
    struct dentry *dentry;
    struct hlist_node debug_node;
    struct kref ref;
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
struct clk_core {
    const char *name;
    const struct clk_ops *ops;
    struct clk_hw *hw;
    struct module *owner;
    struct device *dev;
    struct device_node *of_node;
    struct clk_core *parent;
    struct clk_parent_map *parents;
    u8 num_parents;
    u8 new_parent_index;
    long unsigned int rate;
    long unsigned int req_rate;
    long unsigned int new_rate;
    struct clk_core *new_parent;
    struct clk_core *new_child;
    long unsigned int flags;
    bool orphan;
    bool rpm_enabled;
    unsigned int enable_count;
    unsigned int prepare_count;
    unsigned int protect_count;
    long unsigned int min_rate;
    long unsigned int max_rate;
    long unsigned int accuracy;
    int phase;
    struct clk_duty duty;
    struct hlist_head children;
    struct hlist_node child_node;
    struct hlist_head clks;
    unsigned int notifier_count;
    struct dentry *dentry;
    struct hlist_node debug_node;
    struct kref ref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct clk_core {
    const char *name;
    const struct clk_ops *ops;
    struct clk_hw *hw;
    struct module *owner;
    struct device *dev;
    struct device_node *of_node;
    struct clk_core *parent;
    struct clk_parent_map *parents;
    u8 num_parents;
    u8 new_parent_index;
    long unsigned int rate;
    long unsigned int req_rate;
    long unsigned int new_rate;
    struct clk_core *new_parent;
    struct clk_core *new_child;
    long unsigned int flags;
    bool orphan;
    bool rpm_enabled;
    unsigned int enable_count;
    unsigned int prepare_count;
    unsigned int protect_count;
    long unsigned int min_rate;
    long unsigned int max_rate;
    long unsigned int accuracy;
    int phase;
    struct clk_duty duty;
    struct hlist_head children;
    struct hlist_node child_node;
    struct hlist_head clks;
    unsigned int notifier_count;
    struct dentry *dentry;
    struct hlist_node debug_node;
    struct kref ref;
};
```
</details>
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct clk_core {
    const char *name;
    const struct clk_ops *ops;
    struct clk_hw *hw;
    struct module *owner;
    struct device *dev;
    struct device_node *of_node;
    struct clk_core *parent;
    struct clk_parent_map *parents;
    u8 num_parents;
    u8 new_parent_index;
    long unsigned int rate;
    long unsigned int req_rate;
    long unsigned int new_rate;
    struct clk_core *new_parent;
    struct clk_core *new_child;
    long unsigned int flags;
    bool orphan;
    bool rpm_enabled;
    unsigned int enable_count;
    unsigned int prepare_count;
    unsigned int protect_count;
    long unsigned int min_rate;
    long unsigned int max_rate;
    long unsigned int accuracy;
    int phase;
    struct clk_duty duty;
    struct hlist_head children;
    struct hlist_node child_node;
    struct hlist_head clks;
    unsigned int notifier_count;
    struct dentry *dentry;
    struct hlist_node debug_node;
    struct kref ref;
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
struct clk_core {
    const char *name;
    const struct clk_ops *ops;
    struct clk_hw *hw;
    struct module *owner;
    struct device *dev;
    struct device_node *of_node;
    struct clk_core *parent;
    struct clk_parent_map *parents;
    u8 num_parents;
    u8 new_parent_index;
    long unsigned int rate;
    long unsigned int req_rate;
    long unsigned int new_rate;
    struct clk_core *new_parent;
    struct clk_core *new_child;
    long unsigned int flags;
    bool orphan;
    bool rpm_enabled;
    unsigned int enable_count;
    unsigned int prepare_count;
    unsigned int protect_count;
    long unsigned int min_rate;
    long unsigned int max_rate;
    long unsigned int accuracy;
    int phase;
    struct clk_duty duty;
    struct hlist_head children;
    struct hlist_node child_node;
    struct hlist_head clks;
    unsigned int notifier_count;
    struct dentry *dentry;
    struct hlist_node debug_node;
    struct kref ref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct clk_core {
    const char *name;
    const struct clk_ops *ops;
    struct clk_hw *hw;
    struct module *owner;
    struct device *dev;
    struct device_node *of_node;
    struct clk_core *parent;
    struct clk_parent_map *parents;
    u8 num_parents;
    u8 new_parent_index;
    long unsigned int rate;
    long unsigned int req_rate;
    long unsigned int new_rate;
    struct clk_core *new_parent;
    struct clk_core *new_child;
    long unsigned int flags;
    bool orphan;
    bool rpm_enabled;
    unsigned int enable_count;
    unsigned int prepare_count;
    unsigned int protect_count;
    long unsigned int min_rate;
    long unsigned int max_rate;
    long unsigned int accuracy;
    int phase;
    struct clk_duty duty;
    struct hlist_head children;
    struct hlist_node child_node;
    struct hlist_head clks;
    unsigned int notifier_count;
    struct dentry *dentry;
    struct hlist_node debug_node;
    struct kref ref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct clk_core {
    const char *name;
    const struct clk_ops *ops;
    struct clk_hw *hw;
    struct module *owner;
    struct device *dev;
    struct device_node *of_node;
    struct clk_core *parent;
    struct clk_parent_map *parents;
    u8 num_parents;
    u8 new_parent_index;
    long unsigned int rate;
    long unsigned int req_rate;
    long unsigned int new_rate;
    struct clk_core *new_parent;
    struct clk_core *new_child;
    long unsigned int flags;
    bool orphan;
    bool rpm_enabled;
    unsigned int enable_count;
    unsigned int prepare_count;
    unsigned int protect_count;
    long unsigned int min_rate;
    long unsigned int max_rate;
    long unsigned int accuracy;
    int phase;
    struct clk_duty duty;
    struct hlist_head children;
    struct hlist_node child_node;
    struct hlist_head clks;
    unsigned int notifier_count;
    struct dentry *dentry;
    struct hlist_node debug_node;
    struct kref ref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct clk_core {
    const char *name;
    const struct clk_ops *ops;
    struct clk_hw *hw;
    struct module *owner;
    struct device *dev;
    struct device_node *of_node;
    struct clk_core *parent;
    struct clk_parent_map *parents;
    u8 num_parents;
    u8 new_parent_index;
    long unsigned int rate;
    long unsigned int req_rate;
    long unsigned int new_rate;
    struct clk_core *new_parent;
    struct clk_core *new_child;
    long unsigned int flags;
    bool orphan;
    bool rpm_enabled;
    unsigned int enable_count;
    unsigned int prepare_count;
    unsigned int protect_count;
    long unsigned int min_rate;
    long unsigned int max_rate;
    long unsigned int accuracy;
    int phase;
    struct clk_duty duty;
    struct hlist_head children;
    struct hlist_node child_node;
    struct hlist_head clks;
    unsigned int notifier_count;
    struct dentry *dentry;
    struct hlist_node debug_node;
    struct kref ref;
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
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct device *dev</code>
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
<code>unsigned int protect_count</code>
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
<code>struct clk_duty duty</code>
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
<code>struct device_node *of_node</code>
</li>
<li>
<b>Field added. </b>
<code>bool rpm_enabled</code>
</li>
<li>
<b>Field removed. </b>
<code>const char **parent_names</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct clk_core **parents</code> ➡️ <code>struct clk_parent_map *parents</code>
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
