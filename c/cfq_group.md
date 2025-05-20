# Struct: <code>cfq_group</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct cfq_group {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    u64 vdisktime;
    int nr_active;
    unsigned int children_weight;
    unsigned int vfraction;
    unsigned int weight;
    unsigned int new_weight;
    unsigned int dev_weight;
    unsigned int leaf_weight;
    unsigned int new_leaf_weight;
    unsigned int dev_leaf_weight;
    int nr_cfqq;
    unsigned int busy_queues_avg[3];
    struct cfq_rb_root service_trees[6];
    struct cfq_rb_root service_tree_idle;
    long unsigned int saved_wl_slice;
    enum wl_type_t saved_wl_type;
    enum wl_class_t saved_wl_class;
    int dispatched;
    struct cfq_ttime ttime;
    struct cfqg_stats stats;
    struct cfq_queue * async_cfqq[16];
    struct cfq_queue *async_idle_cfqq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct cfq_group {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    u64 vdisktime;
    int nr_active;
    unsigned int children_weight;
    unsigned int vfraction;
    unsigned int weight;
    unsigned int new_weight;
    unsigned int dev_weight;
    unsigned int leaf_weight;
    unsigned int new_leaf_weight;
    unsigned int dev_leaf_weight;
    int nr_cfqq;
    unsigned int busy_queues_avg[3];
    struct cfq_rb_root service_trees[6];
    struct cfq_rb_root service_tree_idle;
    u64 saved_wl_slice;
    enum wl_type_t saved_wl_type;
    enum wl_class_t saved_wl_class;
    int dispatched;
    struct cfq_ttime ttime;
    struct cfqg_stats stats;
    struct cfq_queue * async_cfqq[16];
    struct cfq_queue *async_idle_cfqq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct cfq_group {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    u64 vdisktime;
    int nr_active;
    unsigned int children_weight;
    unsigned int vfraction;
    unsigned int weight;
    unsigned int new_weight;
    unsigned int dev_weight;
    unsigned int leaf_weight;
    unsigned int new_leaf_weight;
    unsigned int dev_leaf_weight;
    int nr_cfqq;
    unsigned int busy_queues_avg[3];
    struct cfq_rb_root service_trees[6];
    struct cfq_rb_root service_tree_idle;
    u64 saved_wl_slice;
    enum wl_type_t saved_wl_type;
    enum wl_class_t saved_wl_class;
    int dispatched;
    struct cfq_ttime ttime;
    struct cfqg_stats stats;
    struct cfq_queue * async_cfqq[16];
    struct cfq_queue *async_idle_cfqq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct cfq_group {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    u64 vdisktime;
    int nr_active;
    unsigned int children_weight;
    unsigned int vfraction;
    unsigned int weight;
    unsigned int new_weight;
    unsigned int dev_weight;
    unsigned int leaf_weight;
    unsigned int new_leaf_weight;
    unsigned int dev_leaf_weight;
    int nr_cfqq;
    unsigned int busy_queues_avg[3];
    struct cfq_rb_root service_trees[6];
    struct cfq_rb_root service_tree_idle;
    u64 saved_wl_slice;
    enum wl_type_t saved_wl_type;
    enum wl_class_t saved_wl_class;
    int dispatched;
    struct cfq_ttime ttime;
    struct cfqg_stats stats;
    struct cfq_queue * async_cfqq[16];
    struct cfq_queue *async_idle_cfqq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct cfq_group {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    u64 vdisktime;
    int nr_active;
    unsigned int children_weight;
    unsigned int vfraction;
    unsigned int weight;
    unsigned int new_weight;
    unsigned int dev_weight;
    unsigned int leaf_weight;
    unsigned int new_leaf_weight;
    unsigned int dev_leaf_weight;
    int nr_cfqq;
    unsigned int busy_queues_avg[3];
    struct cfq_rb_root service_trees[6];
    struct cfq_rb_root service_tree_idle;
    u64 saved_wl_slice;
    enum wl_type_t saved_wl_type;
    enum wl_class_t saved_wl_class;
    int dispatched;
    struct cfq_ttime ttime;
    struct cfqg_stats stats;
    struct cfq_queue * async_cfqq[16];
    struct cfq_queue *async_idle_cfqq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct cfq_group {
    struct blkg_policy_data pd;
    struct rb_node rb_node;
    u64 vdisktime;
    int nr_active;
    unsigned int children_weight;
    unsigned int vfraction;
    unsigned int weight;
    unsigned int new_weight;
    unsigned int dev_weight;
    unsigned int leaf_weight;
    unsigned int new_leaf_weight;
    unsigned int dev_leaf_weight;
    int nr_cfqq;
    unsigned int busy_queues_avg[3];
    struct cfq_rb_root service_trees[6];
    struct cfq_rb_root service_tree_idle;
    u64 saved_wl_slice;
    enum wl_type_t saved_wl_type;
    enum wl_class_t saved_wl_class;
    int dispatched;
    struct cfq_ttime ttime;
    struct cfqg_stats stats;
    struct cfq_queue * async_cfqq[16];
    struct cfq_queue *async_idle_cfqq;
};
```
</details>
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
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
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
<details>
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long unsigned int saved_wl_slice</code> ➡️ <code>u64 saved_wl_slice</code>
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
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
</ul>
