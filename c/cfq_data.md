# Struct: <code>cfq_data</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct cfq_data {
    struct request_queue *queue;
    struct cfq_rb_root grp_service_tree;
    struct cfq_group *root_group;
    enum wl_class_t serving_wl_class;
    enum wl_type_t serving_wl_type;
    long unsigned int workload_expires;
    struct cfq_group *serving_group;
    struct rb_root prio_trees[8];
    unsigned int busy_queues;
    unsigned int busy_sync_queues;
    int rq_in_driver;
    int rq_in_flight[2];
    int rq_queued;
    int hw_tag;
    int hw_tag_est_depth;
    unsigned int hw_tag_samples;
    struct timer_list idle_slice_timer;
    struct work_struct unplug_work;
    struct cfq_queue *active_queue;
    struct cfq_io_cq *active_cic;
    sector_t last_position;
    unsigned int cfq_quantum;
    unsigned int cfq_fifo_expire[2];
    unsigned int cfq_back_penalty;
    unsigned int cfq_back_max;
    unsigned int cfq_slice[2];
    unsigned int cfq_slice_async_rq;
    unsigned int cfq_slice_idle;
    unsigned int cfq_group_idle;
    unsigned int cfq_latency;
    unsigned int cfq_target_latency;
    struct cfq_queue oom_cfqq;
    long unsigned int last_delayed_sync;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct cfq_data {
    struct request_queue *queue;
    struct cfq_rb_root grp_service_tree;
    struct cfq_group *root_group;
    enum wl_class_t serving_wl_class;
    enum wl_type_t serving_wl_type;
    u64 workload_expires;
    struct cfq_group *serving_group;
    struct rb_root prio_trees[8];
    unsigned int busy_queues;
    unsigned int busy_sync_queues;
    int rq_in_driver;
    int rq_in_flight[2];
    int rq_queued;
    int hw_tag;
    int hw_tag_est_depth;
    unsigned int hw_tag_samples;
    struct hrtimer idle_slice_timer;
    struct work_struct unplug_work;
    struct cfq_queue *active_queue;
    struct cfq_io_cq *active_cic;
    sector_t last_position;
    unsigned int cfq_quantum;
    unsigned int cfq_back_penalty;
    unsigned int cfq_back_max;
    unsigned int cfq_slice_async_rq;
    unsigned int cfq_latency;
    u64 cfq_fifo_expire[2];
    u64 cfq_slice[2];
    u64 cfq_slice_idle;
    u64 cfq_group_idle;
    u64 cfq_target_latency;
    struct cfq_queue oom_cfqq;
    u64 last_delayed_sync;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct cfq_data {
    struct request_queue *queue;
    struct cfq_rb_root grp_service_tree;
    struct cfq_group *root_group;
    enum wl_class_t serving_wl_class;
    enum wl_type_t serving_wl_type;
    u64 workload_expires;
    struct cfq_group *serving_group;
    struct rb_root prio_trees[8];
    unsigned int busy_queues;
    unsigned int busy_sync_queues;
    int rq_in_driver;
    int rq_in_flight[2];
    int rq_queued;
    int hw_tag;
    int hw_tag_est_depth;
    unsigned int hw_tag_samples;
    struct hrtimer idle_slice_timer;
    struct work_struct unplug_work;
    struct cfq_queue *active_queue;
    struct cfq_io_cq *active_cic;
    sector_t last_position;
    unsigned int cfq_quantum;
    unsigned int cfq_back_penalty;
    unsigned int cfq_back_max;
    unsigned int cfq_slice_async_rq;
    unsigned int cfq_latency;
    u64 cfq_fifo_expire[2];
    u64 cfq_slice[2];
    u64 cfq_slice_idle;
    u64 cfq_group_idle;
    u64 cfq_target_latency;
    struct cfq_queue oom_cfqq;
    u64 last_delayed_sync;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct cfq_data {
    struct request_queue *queue;
    struct cfq_rb_root grp_service_tree;
    struct cfq_group *root_group;
    enum wl_class_t serving_wl_class;
    enum wl_type_t serving_wl_type;
    u64 workload_expires;
    struct cfq_group *serving_group;
    struct rb_root prio_trees[8];
    unsigned int busy_queues;
    unsigned int busy_sync_queues;
    int rq_in_driver;
    int rq_in_flight[2];
    int rq_queued;
    int hw_tag;
    int hw_tag_est_depth;
    unsigned int hw_tag_samples;
    struct hrtimer idle_slice_timer;
    struct work_struct unplug_work;
    struct cfq_queue *active_queue;
    struct cfq_io_cq *active_cic;
    sector_t last_position;
    unsigned int cfq_quantum;
    unsigned int cfq_back_penalty;
    unsigned int cfq_back_max;
    unsigned int cfq_slice_async_rq;
    unsigned int cfq_latency;
    u64 cfq_fifo_expire[2];
    u64 cfq_slice[2];
    u64 cfq_slice_idle;
    u64 cfq_group_idle;
    u64 cfq_target_latency;
    struct cfq_queue oom_cfqq;
    u64 last_delayed_sync;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct cfq_data {
    struct request_queue *queue;
    struct cfq_rb_root grp_service_tree;
    struct cfq_group *root_group;
    enum wl_class_t serving_wl_class;
    enum wl_type_t serving_wl_type;
    u64 workload_expires;
    struct cfq_group *serving_group;
    struct rb_root prio_trees[8];
    unsigned int busy_queues;
    unsigned int busy_sync_queues;
    int rq_in_driver;
    int rq_in_flight[2];
    int rq_queued;
    int hw_tag;
    int hw_tag_est_depth;
    unsigned int hw_tag_samples;
    struct hrtimer idle_slice_timer;
    struct work_struct unplug_work;
    struct cfq_queue *active_queue;
    struct cfq_io_cq *active_cic;
    sector_t last_position;
    unsigned int cfq_quantum;
    unsigned int cfq_back_penalty;
    unsigned int cfq_back_max;
    unsigned int cfq_slice_async_rq;
    unsigned int cfq_latency;
    u64 cfq_fifo_expire[2];
    u64 cfq_slice[2];
    u64 cfq_slice_idle;
    u64 cfq_group_idle;
    u64 cfq_target_latency;
    struct cfq_queue oom_cfqq;
    u64 last_delayed_sync;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct cfq_data {
    struct request_queue *queue;
    struct cfq_rb_root grp_service_tree;
    struct cfq_group *root_group;
    enum wl_class_t serving_wl_class;
    enum wl_type_t serving_wl_type;
    u64 workload_expires;
    struct cfq_group *serving_group;
    struct rb_root prio_trees[8];
    unsigned int busy_queues;
    unsigned int busy_sync_queues;
    int rq_in_driver;
    int rq_in_flight[2];
    int rq_queued;
    int hw_tag;
    int hw_tag_est_depth;
    unsigned int hw_tag_samples;
    struct hrtimer idle_slice_timer;
    struct work_struct unplug_work;
    struct cfq_queue *active_queue;
    struct cfq_io_cq *active_cic;
    sector_t last_position;
    unsigned int cfq_quantum;
    unsigned int cfq_back_penalty;
    unsigned int cfq_back_max;
    unsigned int cfq_slice_async_rq;
    unsigned int cfq_latency;
    u64 cfq_fifo_expire[2];
    u64 cfq_slice[2];
    u64 cfq_slice_idle;
    u64 cfq_group_idle;
    u64 cfq_target_latency;
    struct cfq_queue oom_cfqq;
    u64 last_delayed_sync;
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
<code>long unsigned int workload_expires</code> ➡️ <code>u64 workload_expires</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct timer_list idle_slice_timer</code> ➡️ <code>struct hrtimer idle_slice_timer</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int cfq_fifo_expire[2]</code> ➡️ <code>u64 cfq_fifo_expire[2]</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int cfq_slice[2]</code> ➡️ <code>u64 cfq_slice[2]</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int cfq_slice_idle</code> ➡️ <code>u64 cfq_slice_idle</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int cfq_group_idle</code> ➡️ <code>u64 cfq_group_idle</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int cfq_target_latency</code> ➡️ <code>u64 cfq_target_latency</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int last_delayed_sync</code> ➡️ <code>u64 last_delayed_sync</code>
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
