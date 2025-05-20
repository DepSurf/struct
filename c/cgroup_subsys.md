# Struct: <code>cgroup_subsys</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct cgroup_subsys {
    struct cgroup_subsys_state * (*css_alloc)(struct cgroup_subsys_state *);
    int (*css_online)(struct cgroup_subsys_state *);
    void (*css_offline)(struct cgroup_subsys_state *);
    void (*css_released)(struct cgroup_subsys_state *);
    void (*css_free)(struct cgroup_subsys_state *);
    void (*css_reset)(struct cgroup_subsys_state *);
    void (*css_e_css_changed)(struct cgroup_subsys_state *);
    int (*can_attach)(struct cgroup_taskset *);
    void (*cancel_attach)(struct cgroup_taskset *);
    void (*attach)(struct cgroup_taskset *);
    int (*can_fork)(struct task_struct *, void **);
    void (*cancel_fork)(struct task_struct *, void *);
    void (*fork)(struct task_struct *, void *);
    void (*exit)(struct task_struct *);
    void (*free)(struct task_struct *);
    void (*bind)(struct cgroup_subsys_state *);
    int early_init;
    bool broken_hierarchy;
    bool warned_broken_hierarchy;
    int id;
    const char *name;
    const char *legacy_name;
    struct cgroup_root *root;
    struct idr css_idr;
    struct list_head cfts;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    unsigned int depends_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct cgroup_subsys {
    struct cgroup_subsys_state * (*css_alloc)(struct cgroup_subsys_state *);
    int (*css_online)(struct cgroup_subsys_state *);
    void (*css_offline)(struct cgroup_subsys_state *);
    void (*css_released)(struct cgroup_subsys_state *);
    void (*css_free)(struct cgroup_subsys_state *);
    void (*css_reset)(struct cgroup_subsys_state *);
    int (*can_attach)(struct cgroup_taskset *);
    void (*cancel_attach)(struct cgroup_taskset *);
    void (*attach)(struct cgroup_taskset *);
    void (*post_attach)();
    int (*can_fork)(struct task_struct *);
    void (*cancel_fork)(struct task_struct *);
    void (*fork)(struct task_struct *);
    void (*exit)(struct task_struct *);
    void (*free)(struct task_struct *);
    void (*bind)(struct cgroup_subsys_state *);
    bool early_init;
    bool implicit_on_dfl;
    bool broken_hierarchy;
    bool warned_broken_hierarchy;
    int id;
    const char *name;
    const char *legacy_name;
    struct cgroup_root *root;
    struct idr css_idr;
    struct list_head cfts;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    unsigned int depends_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct cgroup_subsys {
    struct cgroup_subsys_state * (*css_alloc)(struct cgroup_subsys_state *);
    int (*css_online)(struct cgroup_subsys_state *);
    void (*css_offline)(struct cgroup_subsys_state *);
    void (*css_released)(struct cgroup_subsys_state *);
    void (*css_free)(struct cgroup_subsys_state *);
    void (*css_reset)(struct cgroup_subsys_state *);
    int (*can_attach)(struct cgroup_taskset *);
    void (*cancel_attach)(struct cgroup_taskset *);
    void (*attach)(struct cgroup_taskset *);
    void (*post_attach)();
    int (*can_fork)(struct task_struct *);
    void (*cancel_fork)(struct task_struct *);
    void (*fork)(struct task_struct *);
    void (*exit)(struct task_struct *);
    void (*free)(struct task_struct *);
    void (*bind)(struct cgroup_subsys_state *);
    bool early_init;
    bool implicit_on_dfl;
    bool broken_hierarchy;
    bool warned_broken_hierarchy;
    int id;
    const char *name;
    const char *legacy_name;
    struct cgroup_root *root;
    struct idr css_idr;
    struct list_head cfts;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    unsigned int depends_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct cgroup_subsys {
    struct cgroup_subsys_state * (*css_alloc)(struct cgroup_subsys_state *);
    int (*css_online)(struct cgroup_subsys_state *);
    void (*css_offline)(struct cgroup_subsys_state *);
    void (*css_released)(struct cgroup_subsys_state *);
    void (*css_free)(struct cgroup_subsys_state *);
    void (*css_reset)(struct cgroup_subsys_state *);
    int (*can_attach)(struct cgroup_taskset *);
    void (*cancel_attach)(struct cgroup_taskset *);
    void (*attach)(struct cgroup_taskset *);
    void (*post_attach)();
    int (*can_fork)(struct task_struct *);
    void (*cancel_fork)(struct task_struct *);
    void (*fork)(struct task_struct *);
    void (*exit)(struct task_struct *);
    void (*free)(struct task_struct *);
    void (*bind)(struct cgroup_subsys_state *);
    bool early_init;
    bool implicit_on_dfl;
    bool broken_hierarchy;
    bool warned_broken_hierarchy;
    int id;
    const char *name;
    const char *legacy_name;
    struct cgroup_root *root;
    struct idr css_idr;
    struct list_head cfts;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    unsigned int depends_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct cgroup_subsys {
    struct cgroup_subsys_state * (*css_alloc)(struct cgroup_subsys_state *);
    int (*css_online)(struct cgroup_subsys_state *);
    void (*css_offline)(struct cgroup_subsys_state *);
    void (*css_released)(struct cgroup_subsys_state *);
    void (*css_free)(struct cgroup_subsys_state *);
    void (*css_reset)(struct cgroup_subsys_state *);
    int (*css_extra_stat_show)(struct seq_file *, struct cgroup_subsys_state *);
    int (*can_attach)(struct cgroup_taskset *);
    void (*cancel_attach)(struct cgroup_taskset *);
    void (*attach)(struct cgroup_taskset *);
    void (*post_attach)();
    int (*can_fork)(struct task_struct *);
    void (*cancel_fork)(struct task_struct *);
    void (*fork)(struct task_struct *);
    void (*exit)(struct task_struct *);
    void (*free)(struct task_struct *);
    void (*bind)(struct cgroup_subsys_state *);
    bool early_init;
    bool implicit_on_dfl;
    bool threaded;
    bool broken_hierarchy;
    bool warned_broken_hierarchy;
    int id;
    const char *name;
    const char *legacy_name;
    struct cgroup_root *root;
    struct idr css_idr;
    struct list_head cfts;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    unsigned int depends_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct cgroup_subsys {
    struct cgroup_subsys_state * (*css_alloc)(struct cgroup_subsys_state *);
    int (*css_online)(struct cgroup_subsys_state *);
    void (*css_offline)(struct cgroup_subsys_state *);
    void (*css_released)(struct cgroup_subsys_state *);
    void (*css_free)(struct cgroup_subsys_state *);
    void (*css_reset)(struct cgroup_subsys_state *);
    void (*css_rstat_flush)(struct cgroup_subsys_state *, int);
    int (*css_extra_stat_show)(struct seq_file *, struct cgroup_subsys_state *);
    int (*can_attach)(struct cgroup_taskset *);
    void (*cancel_attach)(struct cgroup_taskset *);
    void (*attach)(struct cgroup_taskset *);
    void (*post_attach)();
    int (*can_fork)(struct task_struct *);
    void (*cancel_fork)(struct task_struct *);
    void (*fork)(struct task_struct *);
    void (*exit)(struct task_struct *);
    void (*free)(struct task_struct *);
    void (*bind)(struct cgroup_subsys_state *);
    bool early_init;
    bool implicit_on_dfl;
    bool threaded;
    bool broken_hierarchy;
    bool warned_broken_hierarchy;
    int id;
    const char *name;
    const char *legacy_name;
    struct cgroup_root *root;
    struct idr css_idr;
    struct list_head cfts;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    unsigned int depends_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct cgroup_subsys {
    struct cgroup_subsys_state * (*css_alloc)(struct cgroup_subsys_state *);
    int (*css_online)(struct cgroup_subsys_state *);
    void (*css_offline)(struct cgroup_subsys_state *);
    void (*css_released)(struct cgroup_subsys_state *);
    void (*css_free)(struct cgroup_subsys_state *);
    void (*css_reset)(struct cgroup_subsys_state *);
    void (*css_rstat_flush)(struct cgroup_subsys_state *, int);
    int (*css_extra_stat_show)(struct seq_file *, struct cgroup_subsys_state *);
    int (*can_attach)(struct cgroup_taskset *);
    void (*cancel_attach)(struct cgroup_taskset *);
    void (*attach)(struct cgroup_taskset *);
    void (*post_attach)();
    int (*can_fork)(struct task_struct *);
    void (*cancel_fork)(struct task_struct *);
    void (*fork)(struct task_struct *);
    void (*exit)(struct task_struct *);
    void (*free)(struct task_struct *);
    void (*bind)(struct cgroup_subsys_state *);
    bool early_init;
    bool implicit_on_dfl;
    bool threaded;
    bool broken_hierarchy;
    bool warned_broken_hierarchy;
    int id;
    const char *name;
    const char *legacy_name;
    struct cgroup_root *root;
    struct idr css_idr;
    struct list_head cfts;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    unsigned int depends_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct cgroup_subsys {
    struct cgroup_subsys_state * (*css_alloc)(struct cgroup_subsys_state *);
    int (*css_online)(struct cgroup_subsys_state *);
    void (*css_offline)(struct cgroup_subsys_state *);
    void (*css_released)(struct cgroup_subsys_state *);
    void (*css_free)(struct cgroup_subsys_state *);
    void (*css_reset)(struct cgroup_subsys_state *);
    void (*css_rstat_flush)(struct cgroup_subsys_state *, int);
    int (*css_extra_stat_show)(struct seq_file *, struct cgroup_subsys_state *);
    int (*can_attach)(struct cgroup_taskset *);
    void (*cancel_attach)(struct cgroup_taskset *);
    void (*attach)(struct cgroup_taskset *);
    void (*post_attach)();
    int (*can_fork)(struct task_struct *);
    void (*cancel_fork)(struct task_struct *);
    void (*fork)(struct task_struct *);
    void (*exit)(struct task_struct *);
    void (*release)(struct task_struct *);
    void (*bind)(struct cgroup_subsys_state *);
    bool early_init;
    bool implicit_on_dfl;
    bool threaded;
    bool broken_hierarchy;
    bool warned_broken_hierarchy;
    int id;
    const char *name;
    const char *legacy_name;
    struct cgroup_root *root;
    struct idr css_idr;
    struct list_head cfts;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    unsigned int depends_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct cgroup_subsys {
    struct cgroup_subsys_state * (*css_alloc)(struct cgroup_subsys_state *);
    int (*css_online)(struct cgroup_subsys_state *);
    void (*css_offline)(struct cgroup_subsys_state *);
    void (*css_released)(struct cgroup_subsys_state *);
    void (*css_free)(struct cgroup_subsys_state *);
    void (*css_reset)(struct cgroup_subsys_state *);
    void (*css_rstat_flush)(struct cgroup_subsys_state *, int);
    int (*css_extra_stat_show)(struct seq_file *, struct cgroup_subsys_state *);
    int (*can_attach)(struct cgroup_taskset *);
    void (*cancel_attach)(struct cgroup_taskset *);
    void (*attach)(struct cgroup_taskset *);
    void (*post_attach)();
    int (*can_fork)(struct task_struct *);
    void (*cancel_fork)(struct task_struct *);
    void (*fork)(struct task_struct *);
    void (*exit)(struct task_struct *);
    void (*release)(struct task_struct *);
    void (*bind)(struct cgroup_subsys_state *);
    bool early_init;
    bool implicit_on_dfl;
    bool threaded;
    bool broken_hierarchy;
    bool warned_broken_hierarchy;
    int id;
    const char *name;
    const char *legacy_name;
    struct cgroup_root *root;
    struct idr css_idr;
    struct list_head cfts;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    unsigned int depends_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct cgroup_subsys {
    struct cgroup_subsys_state * (*css_alloc)(struct cgroup_subsys_state *);
    int (*css_online)(struct cgroup_subsys_state *);
    void (*css_offline)(struct cgroup_subsys_state *);
    void (*css_released)(struct cgroup_subsys_state *);
    void (*css_free)(struct cgroup_subsys_state *);
    void (*css_reset)(struct cgroup_subsys_state *);
    void (*css_rstat_flush)(struct cgroup_subsys_state *, int);
    int (*css_extra_stat_show)(struct seq_file *, struct cgroup_subsys_state *);
    int (*can_attach)(struct cgroup_taskset *);
    void (*cancel_attach)(struct cgroup_taskset *);
    void (*attach)(struct cgroup_taskset *);
    void (*post_attach)();
    int (*can_fork)(struct task_struct *, struct css_set *);
    void (*cancel_fork)(struct task_struct *, struct css_set *);
    void (*fork)(struct task_struct *);
    void (*exit)(struct task_struct *);
    void (*release)(struct task_struct *);
    void (*bind)(struct cgroup_subsys_state *);
    bool early_init;
    bool implicit_on_dfl;
    bool threaded;
    bool broken_hierarchy;
    bool warned_broken_hierarchy;
    int id;
    const char *name;
    const char *legacy_name;
    struct cgroup_root *root;
    struct idr css_idr;
    struct list_head cfts;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    unsigned int depends_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct cgroup_subsys {
    struct cgroup_subsys_state * (*css_alloc)(struct cgroup_subsys_state *);
    int (*css_online)(struct cgroup_subsys_state *);
    void (*css_offline)(struct cgroup_subsys_state *);
    void (*css_released)(struct cgroup_subsys_state *);
    void (*css_free)(struct cgroup_subsys_state *);
    void (*css_reset)(struct cgroup_subsys_state *);
    void (*css_rstat_flush)(struct cgroup_subsys_state *, int);
    int (*css_extra_stat_show)(struct seq_file *, struct cgroup_subsys_state *);
    int (*can_attach)(struct cgroup_taskset *);
    void (*cancel_attach)(struct cgroup_taskset *);
    void (*attach)(struct cgroup_taskset *);
    void (*post_attach)();
    int (*can_fork)(struct task_struct *, struct css_set *);
    void (*cancel_fork)(struct task_struct *, struct css_set *);
    void (*fork)(struct task_struct *);
    void (*exit)(struct task_struct *);
    void (*release)(struct task_struct *);
    void (*bind)(struct cgroup_subsys_state *);
    bool early_init;
    bool implicit_on_dfl;
    bool threaded;
    int id;
    const char *name;
    const char *legacy_name;
    struct cgroup_root *root;
    struct idr css_idr;
    struct list_head cfts;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    unsigned int depends_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct cgroup_subsys {
    struct cgroup_subsys_state * (*css_alloc)(struct cgroup_subsys_state *);
    int (*css_online)(struct cgroup_subsys_state *);
    void (*css_offline)(struct cgroup_subsys_state *);
    void (*css_released)(struct cgroup_subsys_state *);
    void (*css_free)(struct cgroup_subsys_state *);
    void (*css_reset)(struct cgroup_subsys_state *);
    void (*css_rstat_flush)(struct cgroup_subsys_state *, int);
    int (*css_extra_stat_show)(struct seq_file *, struct cgroup_subsys_state *);
    int (*can_attach)(struct cgroup_taskset *);
    void (*cancel_attach)(struct cgroup_taskset *);
    void (*attach)(struct cgroup_taskset *);
    void (*post_attach)();
    int (*can_fork)(struct task_struct *, struct css_set *);
    void (*cancel_fork)(struct task_struct *, struct css_set *);
    void (*fork)(struct task_struct *);
    void (*exit)(struct task_struct *);
    void (*release)(struct task_struct *);
    void (*bind)(struct cgroup_subsys_state *);
    bool early_init;
    bool implicit_on_dfl;
    bool threaded;
    int id;
    const char *name;
    const char *legacy_name;
    struct cgroup_root *root;
    struct idr css_idr;
    struct list_head cfts;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    unsigned int depends_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct cgroup_subsys {
    struct cgroup_subsys_state * (*css_alloc)(struct cgroup_subsys_state *);
    int (*css_online)(struct cgroup_subsys_state *);
    void (*css_offline)(struct cgroup_subsys_state *);
    void (*css_released)(struct cgroup_subsys_state *);
    void (*css_free)(struct cgroup_subsys_state *);
    void (*css_reset)(struct cgroup_subsys_state *);
    void (*css_rstat_flush)(struct cgroup_subsys_state *, int);
    int (*css_extra_stat_show)(struct seq_file *, struct cgroup_subsys_state *);
    int (*can_attach)(struct cgroup_taskset *);
    void (*cancel_attach)(struct cgroup_taskset *);
    void (*attach)(struct cgroup_taskset *);
    void (*post_attach)();
    int (*can_fork)(struct task_struct *, struct css_set *);
    void (*cancel_fork)(struct task_struct *, struct css_set *);
    void (*fork)(struct task_struct *);
    void (*exit)(struct task_struct *);
    void (*release)(struct task_struct *);
    void (*bind)(struct cgroup_subsys_state *);
    bool early_init;
    bool implicit_on_dfl;
    bool threaded;
    int id;
    const char *name;
    const char *legacy_name;
    struct cgroup_root *root;
    struct idr css_idr;
    struct list_head cfts;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    unsigned int depends_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct cgroup_subsys {
    struct cgroup_subsys_state * (*css_alloc)(struct cgroup_subsys_state *);
    int (*css_online)(struct cgroup_subsys_state *);
    void (*css_offline)(struct cgroup_subsys_state *);
    void (*css_released)(struct cgroup_subsys_state *);
    void (*css_free)(struct cgroup_subsys_state *);
    void (*css_reset)(struct cgroup_subsys_state *);
    void (*css_rstat_flush)(struct cgroup_subsys_state *, int);
    int (*css_extra_stat_show)(struct seq_file *, struct cgroup_subsys_state *);
    int (*can_attach)(struct cgroup_taskset *);
    void (*cancel_attach)(struct cgroup_taskset *);
    void (*attach)(struct cgroup_taskset *);
    void (*post_attach)();
    int (*can_fork)(struct task_struct *, struct css_set *);
    void (*cancel_fork)(struct task_struct *, struct css_set *);
    void (*fork)(struct task_struct *);
    void (*exit)(struct task_struct *);
    void (*release)(struct task_struct *);
    void (*bind)(struct cgroup_subsys_state *);
    bool early_init;
    bool implicit_on_dfl;
    bool threaded;
    int id;
    const char *name;
    const char *legacy_name;
    struct cgroup_root *root;
    struct idr css_idr;
    struct list_head cfts;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    unsigned int depends_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct cgroup_subsys {
    struct cgroup_subsys_state * (*css_alloc)(struct cgroup_subsys_state *);
    int (*css_online)(struct cgroup_subsys_state *);
    void (*css_offline)(struct cgroup_subsys_state *);
    void (*css_released)(struct cgroup_subsys_state *);
    void (*css_free)(struct cgroup_subsys_state *);
    void (*css_reset)(struct cgroup_subsys_state *);
    void (*css_rstat_flush)(struct cgroup_subsys_state *, int);
    int (*css_extra_stat_show)(struct seq_file *, struct cgroup_subsys_state *);
    int (*can_attach)(struct cgroup_taskset *);
    void (*cancel_attach)(struct cgroup_taskset *);
    void (*attach)(struct cgroup_taskset *);
    void (*post_attach)();
    int (*can_fork)(struct task_struct *, struct css_set *);
    void (*cancel_fork)(struct task_struct *, struct css_set *);
    void (*fork)(struct task_struct *);
    void (*exit)(struct task_struct *);
    void (*release)(struct task_struct *);
    void (*bind)(struct cgroup_subsys_state *);
    bool early_init;
    bool implicit_on_dfl;
    bool threaded;
    int id;
    const char *name;
    const char *legacy_name;
    struct cgroup_root *root;
    struct idr css_idr;
    struct list_head cfts;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    unsigned int depends_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct cgroup_subsys {
    struct cgroup_subsys_state * (*css_alloc)(struct cgroup_subsys_state *);
    int (*css_online)(struct cgroup_subsys_state *);
    void (*css_offline)(struct cgroup_subsys_state *);
    void (*css_released)(struct cgroup_subsys_state *);
    void (*css_free)(struct cgroup_subsys_state *);
    void (*css_reset)(struct cgroup_subsys_state *);
    void (*css_rstat_flush)(struct cgroup_subsys_state *, int);
    int (*css_extra_stat_show)(struct seq_file *, struct cgroup_subsys_state *);
    int (*can_attach)(struct cgroup_taskset *);
    void (*cancel_attach)(struct cgroup_taskset *);
    void (*attach)(struct cgroup_taskset *);
    void (*post_attach)();
    int (*can_fork)(struct task_struct *, struct css_set *);
    void (*cancel_fork)(struct task_struct *, struct css_set *);
    void (*fork)(struct task_struct *);
    void (*exit)(struct task_struct *);
    void (*release)(struct task_struct *);
    void (*bind)(struct cgroup_subsys_state *);
    bool early_init;
    bool implicit_on_dfl;
    bool threaded;
    int id;
    const char *name;
    const char *legacy_name;
    struct cgroup_root *root;
    struct idr css_idr;
    struct list_head cfts;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    unsigned int depends_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct cgroup_subsys {
    struct cgroup_subsys_state * (*css_alloc)(struct cgroup_subsys_state *);
    int (*css_online)(struct cgroup_subsys_state *);
    void (*css_offline)(struct cgroup_subsys_state *);
    void (*css_released)(struct cgroup_subsys_state *);
    void (*css_free)(struct cgroup_subsys_state *);
    void (*css_reset)(struct cgroup_subsys_state *);
    void (*css_rstat_flush)(struct cgroup_subsys_state *, int);
    int (*css_extra_stat_show)(struct seq_file *, struct cgroup_subsys_state *);
    int (*css_local_stat_show)(struct seq_file *, struct cgroup_subsys_state *);
    int (*can_attach)(struct cgroup_taskset *);
    void (*cancel_attach)(struct cgroup_taskset *);
    void (*attach)(struct cgroup_taskset *);
    void (*post_attach)();
    int (*can_fork)(struct task_struct *, struct css_set *);
    void (*cancel_fork)(struct task_struct *, struct css_set *);
    void (*fork)(struct task_struct *);
    void (*exit)(struct task_struct *);
    void (*release)(struct task_struct *);
    void (*bind)(struct cgroup_subsys_state *);
    bool early_init;
    bool implicit_on_dfl;
    bool threaded;
    int id;
    const char *name;
    const char *legacy_name;
    struct cgroup_root *root;
    struct idr css_idr;
    struct list_head cfts;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    unsigned int depends_on;
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
struct cgroup_subsys {
    struct cgroup_subsys_state * (*css_alloc)(struct cgroup_subsys_state *);
    int (*css_online)(struct cgroup_subsys_state *);
    void (*css_offline)(struct cgroup_subsys_state *);
    void (*css_released)(struct cgroup_subsys_state *);
    void (*css_free)(struct cgroup_subsys_state *);
    void (*css_reset)(struct cgroup_subsys_state *);
    void (*css_rstat_flush)(struct cgroup_subsys_state *, int);
    int (*css_extra_stat_show)(struct seq_file *, struct cgroup_subsys_state *);
    int (*can_attach)(struct cgroup_taskset *);
    void (*cancel_attach)(struct cgroup_taskset *);
    void (*attach)(struct cgroup_taskset *);
    void (*post_attach)();
    int (*can_fork)(struct task_struct *);
    void (*cancel_fork)(struct task_struct *);
    void (*fork)(struct task_struct *);
    void (*exit)(struct task_struct *);
    void (*release)(struct task_struct *);
    void (*bind)(struct cgroup_subsys_state *);
    bool early_init;
    bool implicit_on_dfl;
    bool threaded;
    bool broken_hierarchy;
    bool warned_broken_hierarchy;
    int id;
    const char *name;
    const char *legacy_name;
    struct cgroup_root *root;
    struct idr css_idr;
    struct list_head cfts;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    unsigned int depends_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct cgroup_subsys {
    struct cgroup_subsys_state * (*css_alloc)(struct cgroup_subsys_state *);
    int (*css_online)(struct cgroup_subsys_state *);
    void (*css_offline)(struct cgroup_subsys_state *);
    void (*css_released)(struct cgroup_subsys_state *);
    void (*css_free)(struct cgroup_subsys_state *);
    void (*css_reset)(struct cgroup_subsys_state *);
    void (*css_rstat_flush)(struct cgroup_subsys_state *, int);
    int (*css_extra_stat_show)(struct seq_file *, struct cgroup_subsys_state *);
    int (*can_attach)(struct cgroup_taskset *);
    void (*cancel_attach)(struct cgroup_taskset *);
    void (*attach)(struct cgroup_taskset *);
    void (*post_attach)();
    int (*can_fork)(struct task_struct *);
    void (*cancel_fork)(struct task_struct *);
    void (*fork)(struct task_struct *);
    void (*exit)(struct task_struct *);
    void (*release)(struct task_struct *);
    void (*bind)(struct cgroup_subsys_state *);
    bool early_init;
    bool implicit_on_dfl;
    bool threaded;
    bool broken_hierarchy;
    bool warned_broken_hierarchy;
    int id;
    const char *name;
    const char *legacy_name;
    struct cgroup_root *root;
    struct idr css_idr;
    struct list_head cfts;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    unsigned int depends_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct cgroup_subsys {
    struct cgroup_subsys_state * (*css_alloc)(struct cgroup_subsys_state *);
    int (*css_online)(struct cgroup_subsys_state *);
    void (*css_offline)(struct cgroup_subsys_state *);
    void (*css_released)(struct cgroup_subsys_state *);
    void (*css_free)(struct cgroup_subsys_state *);
    void (*css_reset)(struct cgroup_subsys_state *);
    void (*css_rstat_flush)(struct cgroup_subsys_state *, int);
    int (*css_extra_stat_show)(struct seq_file *, struct cgroup_subsys_state *);
    int (*can_attach)(struct cgroup_taskset *);
    void (*cancel_attach)(struct cgroup_taskset *);
    void (*attach)(struct cgroup_taskset *);
    void (*post_attach)();
    int (*can_fork)(struct task_struct *);
    void (*cancel_fork)(struct task_struct *);
    void (*fork)(struct task_struct *);
    void (*exit)(struct task_struct *);
    void (*release)(struct task_struct *);
    void (*bind)(struct cgroup_subsys_state *);
    bool early_init;
    bool implicit_on_dfl;
    bool threaded;
    bool broken_hierarchy;
    bool warned_broken_hierarchy;
    int id;
    const char *name;
    const char *legacy_name;
    struct cgroup_root *root;
    struct idr css_idr;
    struct list_head cfts;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    unsigned int depends_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct cgroup_subsys {
    struct cgroup_subsys_state * (*css_alloc)(struct cgroup_subsys_state *);
    int (*css_online)(struct cgroup_subsys_state *);
    void (*css_offline)(struct cgroup_subsys_state *);
    void (*css_released)(struct cgroup_subsys_state *);
    void (*css_free)(struct cgroup_subsys_state *);
    void (*css_reset)(struct cgroup_subsys_state *);
    void (*css_rstat_flush)(struct cgroup_subsys_state *, int);
    int (*css_extra_stat_show)(struct seq_file *, struct cgroup_subsys_state *);
    int (*can_attach)(struct cgroup_taskset *);
    void (*cancel_attach)(struct cgroup_taskset *);
    void (*attach)(struct cgroup_taskset *);
    void (*post_attach)();
    int (*can_fork)(struct task_struct *);
    void (*cancel_fork)(struct task_struct *);
    void (*fork)(struct task_struct *);
    void (*exit)(struct task_struct *);
    void (*release)(struct task_struct *);
    void (*bind)(struct cgroup_subsys_state *);
    bool early_init;
    bool implicit_on_dfl;
    bool threaded;
    bool broken_hierarchy;
    bool warned_broken_hierarchy;
    int id;
    const char *name;
    const char *legacy_name;
    struct cgroup_root *root;
    struct idr css_idr;
    struct list_head cfts;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    unsigned int depends_on;
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
struct cgroup_subsys {
    struct cgroup_subsys_state * (*css_alloc)(struct cgroup_subsys_state *);
    int (*css_online)(struct cgroup_subsys_state *);
    void (*css_offline)(struct cgroup_subsys_state *);
    void (*css_released)(struct cgroup_subsys_state *);
    void (*css_free)(struct cgroup_subsys_state *);
    void (*css_reset)(struct cgroup_subsys_state *);
    void (*css_rstat_flush)(struct cgroup_subsys_state *, int);
    int (*css_extra_stat_show)(struct seq_file *, struct cgroup_subsys_state *);
    int (*can_attach)(struct cgroup_taskset *);
    void (*cancel_attach)(struct cgroup_taskset *);
    void (*attach)(struct cgroup_taskset *);
    void (*post_attach)();
    int (*can_fork)(struct task_struct *);
    void (*cancel_fork)(struct task_struct *);
    void (*fork)(struct task_struct *);
    void (*exit)(struct task_struct *);
    void (*release)(struct task_struct *);
    void (*bind)(struct cgroup_subsys_state *);
    bool early_init;
    bool implicit_on_dfl;
    bool threaded;
    bool broken_hierarchy;
    bool warned_broken_hierarchy;
    int id;
    const char *name;
    const char *legacy_name;
    struct cgroup_root *root;
    struct idr css_idr;
    struct list_head cfts;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    unsigned int depends_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct cgroup_subsys {
    struct cgroup_subsys_state * (*css_alloc)(struct cgroup_subsys_state *);
    int (*css_online)(struct cgroup_subsys_state *);
    void (*css_offline)(struct cgroup_subsys_state *);
    void (*css_released)(struct cgroup_subsys_state *);
    void (*css_free)(struct cgroup_subsys_state *);
    void (*css_reset)(struct cgroup_subsys_state *);
    void (*css_rstat_flush)(struct cgroup_subsys_state *, int);
    int (*css_extra_stat_show)(struct seq_file *, struct cgroup_subsys_state *);
    int (*can_attach)(struct cgroup_taskset *);
    void (*cancel_attach)(struct cgroup_taskset *);
    void (*attach)(struct cgroup_taskset *);
    void (*post_attach)();
    int (*can_fork)(struct task_struct *);
    void (*cancel_fork)(struct task_struct *);
    void (*fork)(struct task_struct *);
    void (*exit)(struct task_struct *);
    void (*release)(struct task_struct *);
    void (*bind)(struct cgroup_subsys_state *);
    bool early_init;
    bool implicit_on_dfl;
    bool threaded;
    bool broken_hierarchy;
    bool warned_broken_hierarchy;
    int id;
    const char *name;
    const char *legacy_name;
    struct cgroup_root *root;
    struct idr css_idr;
    struct list_head cfts;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    unsigned int depends_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct cgroup_subsys {
    struct cgroup_subsys_state * (*css_alloc)(struct cgroup_subsys_state *);
    int (*css_online)(struct cgroup_subsys_state *);
    void (*css_offline)(struct cgroup_subsys_state *);
    void (*css_released)(struct cgroup_subsys_state *);
    void (*css_free)(struct cgroup_subsys_state *);
    void (*css_reset)(struct cgroup_subsys_state *);
    void (*css_rstat_flush)(struct cgroup_subsys_state *, int);
    int (*css_extra_stat_show)(struct seq_file *, struct cgroup_subsys_state *);
    int (*can_attach)(struct cgroup_taskset *);
    void (*cancel_attach)(struct cgroup_taskset *);
    void (*attach)(struct cgroup_taskset *);
    void (*post_attach)();
    int (*can_fork)(struct task_struct *);
    void (*cancel_fork)(struct task_struct *);
    void (*fork)(struct task_struct *);
    void (*exit)(struct task_struct *);
    void (*release)(struct task_struct *);
    void (*bind)(struct cgroup_subsys_state *);
    bool early_init;
    bool implicit_on_dfl;
    bool threaded;
    bool broken_hierarchy;
    bool warned_broken_hierarchy;
    int id;
    const char *name;
    const char *legacy_name;
    struct cgroup_root *root;
    struct idr css_idr;
    struct list_head cfts;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    unsigned int depends_on;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cgroup_subsys {
    struct cgroup_subsys_state * (*css_alloc)(struct cgroup_subsys_state *);
    int (*css_online)(struct cgroup_subsys_state *);
    void (*css_offline)(struct cgroup_subsys_state *);
    void (*css_released)(struct cgroup_subsys_state *);
    void (*css_free)(struct cgroup_subsys_state *);
    void (*css_reset)(struct cgroup_subsys_state *);
    void (*css_rstat_flush)(struct cgroup_subsys_state *, int);
    int (*css_extra_stat_show)(struct seq_file *, struct cgroup_subsys_state *);
    int (*can_attach)(struct cgroup_taskset *);
    void (*cancel_attach)(struct cgroup_taskset *);
    void (*attach)(struct cgroup_taskset *);
    void (*post_attach)();
    int (*can_fork)(struct task_struct *);
    void (*cancel_fork)(struct task_struct *);
    void (*fork)(struct task_struct *);
    void (*exit)(struct task_struct *);
    void (*release)(struct task_struct *);
    void (*bind)(struct cgroup_subsys_state *);
    bool early_init;
    bool implicit_on_dfl;
    bool threaded;
    bool broken_hierarchy;
    bool warned_broken_hierarchy;
    int id;
    const char *name;
    const char *legacy_name;
    struct cgroup_root *root;
    struct idr css_idr;
    struct list_head cfts;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    unsigned int depends_on;
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
<code>void (*post_attach)()</code>
</li>
<li>
<b>Field added. </b>
<code>bool implicit_on_dfl</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*css_e_css_changed)(struct cgroup_subsys_state *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*can_fork)(struct task_struct *, void **)</code> ➡️ <code>int (*can_fork)(struct task_struct *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*cancel_fork)(struct task_struct *, void *)</code> ➡️ <code>void (*cancel_fork)(struct task_struct *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*fork)(struct task_struct *, void *)</code> ➡️ <code>void (*fork)(struct task_struct *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int early_init</code> ➡️ <code>bool early_init</code>
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
<code>int (*css_extra_stat_show)(struct seq_file *, struct cgroup_subsys_state *)</code>
</li>
<li>
<b>Field added. </b>
<code>bool threaded</code>
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
<code>void (*css_rstat_flush)(struct cgroup_subsys_state *, int)</code>
</li>
</ul>
</details>
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
<code>void (*release)(struct task_struct *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*free)(struct task_struct *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*can_fork)(struct task_struct *)</code> ➡️ <code>int (*can_fork)(struct task_struct *, struct css_set *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*cancel_fork)(struct task_struct *)</code> ➡️ <code>void (*cancel_fork)(struct task_struct *, struct css_set *)</code>
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
<code>bool broken_hierarchy</code>
</li>
<li>
<b>Field removed. </b>
<code>bool warned_broken_hierarchy</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*css_local_stat_show)(struct seq_file *, struct cgroup_subsys_state *)</code>
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
