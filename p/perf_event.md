# Struct: <code>perf_event</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct perf_event {
    struct list_head event_entry;
    struct list_head group_entry;
    struct list_head sibling_list;
    struct list_head migrate_entry;
    struct hlist_node hlist_entry;
    struct list_head active_entry;
    int nr_siblings;
    int group_flags;
    struct perf_event *group_leader;
    struct pmu *pmu;
    enum perf_event_active_state state;
    unsigned int attach_state;
    local64_t count;
    atomic64_t child_count;
    u64 total_time_enabled;
    u64 total_time_running;
    u64 tstamp_enabled;
    u64 tstamp_running;
    u64 tstamp_stopped;
    u64 shadow_ctx_time;
    struct perf_event_attr attr;
    u16 header_size;
    u16 id_header_size;
    u16 read_size;
    struct hw_perf_event hw;
    struct perf_event_context *ctx;
    atomic_long_t refcount;
    atomic64_t child_total_time_enabled;
    atomic64_t child_total_time_running;
    struct mutex child_mutex;
    struct list_head child_list;
    struct perf_event *parent;
    int oncpu;
    int cpu;
    struct list_head owner_entry;
    struct task_struct *owner;
    struct mutex mmap_mutex;
    atomic_t mmap_count;
    struct ring_buffer *rb;
    struct list_head rb_entry;
    long unsigned int rcu_batches;
    int rcu_pending;
    wait_queue_head_t waitq;
    struct fasync_struct *fasync;
    int pending_wakeup;
    int pending_kill;
    int pending_disable;
    struct irq_work pending;
    atomic_t event_limit;
    void (*destroy)(struct perf_event *);
    struct callback_head callback_head;
    struct pid_namespace *ns;
    u64 id;
    u64 (*clock)();
    perf_overflow_handler_t overflow_handler;
    void *overflow_handler_context;
    struct trace_event_call *tp_event;
    struct event_filter *filter;
    struct ftrace_ops ftrace_ops;
    struct perf_cgroup *cgrp;
    int cgrp_defer_enabled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct perf_event {
    struct list_head event_entry;
    struct list_head group_entry;
    struct list_head sibling_list;
    struct list_head migrate_entry;
    struct hlist_node hlist_entry;
    struct list_head active_entry;
    int nr_siblings;
    int group_flags;
    struct perf_event *group_leader;
    struct pmu *pmu;
    void *pmu_private;
    enum perf_event_active_state state;
    unsigned int attach_state;
    local64_t count;
    atomic64_t child_count;
    u64 total_time_enabled;
    u64 total_time_running;
    u64 tstamp_enabled;
    u64 tstamp_running;
    u64 tstamp_stopped;
    u64 shadow_ctx_time;
    struct perf_event_attr attr;
    u16 header_size;
    u16 id_header_size;
    u16 read_size;
    struct hw_perf_event hw;
    struct perf_event_context *ctx;
    atomic_long_t refcount;
    atomic64_t child_total_time_enabled;
    atomic64_t child_total_time_running;
    struct mutex child_mutex;
    struct list_head child_list;
    struct perf_event *parent;
    int oncpu;
    int cpu;
    struct list_head owner_entry;
    struct task_struct *owner;
    struct mutex mmap_mutex;
    atomic_t mmap_count;
    struct ring_buffer *rb;
    struct list_head rb_entry;
    long unsigned int rcu_batches;
    int rcu_pending;
    wait_queue_head_t waitq;
    struct fasync_struct *fasync;
    int pending_wakeup;
    int pending_kill;
    int pending_disable;
    struct irq_work pending;
    atomic_t event_limit;
    struct perf_addr_filters_head addr_filters;
    long unsigned int *addr_filters_offs;
    long unsigned int addr_filters_gen;
    void (*destroy)(struct perf_event *);
    struct callback_head callback_head;
    struct pid_namespace *ns;
    u64 id;
    u64 (*clock)();
    perf_overflow_handler_t overflow_handler;
    void *overflow_handler_context;
    struct trace_event_call *tp_event;
    struct event_filter *filter;
    struct ftrace_ops ftrace_ops;
    struct perf_cgroup *cgrp;
    int cgrp_defer_enabled;
    struct list_head sb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct perf_event {
    struct list_head event_entry;
    struct list_head group_entry;
    struct list_head sibling_list;
    struct list_head migrate_entry;
    struct hlist_node hlist_entry;
    struct list_head active_entry;
    int nr_siblings;
    int event_caps;
    int group_caps;
    struct perf_event *group_leader;
    struct pmu *pmu;
    void *pmu_private;
    enum perf_event_active_state state;
    unsigned int attach_state;
    local64_t count;
    atomic64_t child_count;
    u64 total_time_enabled;
    u64 total_time_running;
    u64 tstamp_enabled;
    u64 tstamp_running;
    u64 tstamp_stopped;
    u64 shadow_ctx_time;
    struct perf_event_attr attr;
    u16 header_size;
    u16 id_header_size;
    u16 read_size;
    struct hw_perf_event hw;
    struct perf_event_context *ctx;
    atomic_long_t refcount;
    atomic64_t child_total_time_enabled;
    atomic64_t child_total_time_running;
    struct mutex child_mutex;
    struct list_head child_list;
    struct perf_event *parent;
    int oncpu;
    int cpu;
    struct list_head owner_entry;
    struct task_struct *owner;
    struct mutex mmap_mutex;
    atomic_t mmap_count;
    struct ring_buffer *rb;
    struct list_head rb_entry;
    long unsigned int rcu_batches;
    int rcu_pending;
    wait_queue_head_t waitq;
    struct fasync_struct *fasync;
    int pending_wakeup;
    int pending_kill;
    int pending_disable;
    struct irq_work pending;
    atomic_t event_limit;
    struct perf_addr_filters_head addr_filters;
    long unsigned int *addr_filters_offs;
    long unsigned int addr_filters_gen;
    void (*destroy)(struct perf_event *);
    struct callback_head callback_head;
    struct pid_namespace *ns;
    u64 id;
    u64 (*clock)();
    perf_overflow_handler_t overflow_handler;
    void *overflow_handler_context;
    perf_overflow_handler_t orig_overflow_handler;
    struct bpf_prog *prog;
    struct trace_event_call *tp_event;
    struct event_filter *filter;
    struct ftrace_ops ftrace_ops;
    struct perf_cgroup *cgrp;
    int cgrp_defer_enabled;
    struct list_head sb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct perf_event {
    struct list_head event_entry;
    struct list_head group_entry;
    struct list_head sibling_list;
    struct list_head migrate_entry;
    struct hlist_node hlist_entry;
    struct list_head active_entry;
    int nr_siblings;
    int event_caps;
    int group_caps;
    struct perf_event *group_leader;
    struct pmu *pmu;
    void *pmu_private;
    enum perf_event_active_state state;
    unsigned int attach_state;
    local64_t count;
    atomic64_t child_count;
    u64 total_time_enabled;
    u64 total_time_running;
    u64 tstamp_enabled;
    u64 tstamp_running;
    u64 tstamp_stopped;
    u64 shadow_ctx_time;
    struct perf_event_attr attr;
    u16 header_size;
    u16 id_header_size;
    u16 read_size;
    struct hw_perf_event hw;
    struct perf_event_context *ctx;
    atomic_long_t refcount;
    atomic64_t child_total_time_enabled;
    atomic64_t child_total_time_running;
    struct mutex child_mutex;
    struct list_head child_list;
    struct perf_event *parent;
    int oncpu;
    int cpu;
    struct list_head owner_entry;
    struct task_struct *owner;
    struct mutex mmap_mutex;
    atomic_t mmap_count;
    struct ring_buffer *rb;
    struct list_head rb_entry;
    long unsigned int rcu_batches;
    int rcu_pending;
    wait_queue_head_t waitq;
    struct fasync_struct *fasync;
    int pending_wakeup;
    int pending_kill;
    int pending_disable;
    struct irq_work pending;
    atomic_t event_limit;
    struct perf_addr_filters_head addr_filters;
    long unsigned int *addr_filters_offs;
    long unsigned int addr_filters_gen;
    void (*destroy)(struct perf_event *);
    struct callback_head callback_head;
    struct pid_namespace *ns;
    u64 id;
    u64 (*clock)();
    perf_overflow_handler_t overflow_handler;
    void *overflow_handler_context;
    perf_overflow_handler_t orig_overflow_handler;
    struct bpf_prog *prog;
    struct trace_event_call *tp_event;
    struct event_filter *filter;
    struct ftrace_ops ftrace_ops;
    struct perf_cgroup *cgrp;
    int cgrp_defer_enabled;
    struct list_head sb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct perf_event {
    struct list_head event_entry;
    struct list_head group_entry;
    struct list_head sibling_list;
    struct list_head migrate_entry;
    struct hlist_node hlist_entry;
    struct list_head active_entry;
    int nr_siblings;
    int event_caps;
    int group_caps;
    struct perf_event *group_leader;
    struct pmu *pmu;
    void *pmu_private;
    enum perf_event_state state;
    unsigned int attach_state;
    local64_t count;
    atomic64_t child_count;
    u64 total_time_enabled;
    u64 total_time_running;
    u64 tstamp;
    u64 shadow_ctx_time;
    struct perf_event_attr attr;
    u16 header_size;
    u16 id_header_size;
    u16 read_size;
    struct hw_perf_event hw;
    struct perf_event_context *ctx;
    atomic_long_t refcount;
    atomic64_t child_total_time_enabled;
    atomic64_t child_total_time_running;
    struct mutex child_mutex;
    struct list_head child_list;
    struct perf_event *parent;
    int oncpu;
    int cpu;
    struct list_head owner_entry;
    struct task_struct *owner;
    struct mutex mmap_mutex;
    atomic_t mmap_count;
    struct ring_buffer *rb;
    struct list_head rb_entry;
    long unsigned int rcu_batches;
    int rcu_pending;
    wait_queue_head_t waitq;
    struct fasync_struct *fasync;
    int pending_wakeup;
    int pending_kill;
    int pending_disable;
    struct irq_work pending;
    atomic_t event_limit;
    struct perf_addr_filters_head addr_filters;
    long unsigned int *addr_filters_offs;
    long unsigned int addr_filters_gen;
    void (*destroy)(struct perf_event *);
    struct callback_head callback_head;
    struct pid_namespace *ns;
    u64 id;
    u64 (*clock)();
    perf_overflow_handler_t overflow_handler;
    void *overflow_handler_context;
    perf_overflow_handler_t orig_overflow_handler;
    struct bpf_prog *prog;
    struct trace_event_call *tp_event;
    struct event_filter *filter;
    struct ftrace_ops ftrace_ops;
    struct perf_cgroup *cgrp;
    struct list_head sb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct perf_event {
    struct list_head event_entry;
    struct list_head sibling_list;
    struct list_head active_list;
    struct rb_node group_node;
    u64 group_index;
    struct list_head migrate_entry;
    struct hlist_node hlist_entry;
    struct list_head active_entry;
    int nr_siblings;
    int event_caps;
    int group_caps;
    struct perf_event *group_leader;
    struct pmu *pmu;
    void *pmu_private;
    enum perf_event_state state;
    unsigned int attach_state;
    local64_t count;
    atomic64_t child_count;
    u64 total_time_enabled;
    u64 total_time_running;
    u64 tstamp;
    u64 shadow_ctx_time;
    struct perf_event_attr attr;
    u16 header_size;
    u16 id_header_size;
    u16 read_size;
    struct hw_perf_event hw;
    struct perf_event_context *ctx;
    atomic_long_t refcount;
    atomic64_t child_total_time_enabled;
    atomic64_t child_total_time_running;
    struct mutex child_mutex;
    struct list_head child_list;
    struct perf_event *parent;
    int oncpu;
    int cpu;
    struct list_head owner_entry;
    struct task_struct *owner;
    struct mutex mmap_mutex;
    atomic_t mmap_count;
    struct ring_buffer *rb;
    struct list_head rb_entry;
    long unsigned int rcu_batches;
    int rcu_pending;
    wait_queue_head_t waitq;
    struct fasync_struct *fasync;
    int pending_wakeup;
    int pending_kill;
    int pending_disable;
    struct irq_work pending;
    atomic_t event_limit;
    struct perf_addr_filters_head addr_filters;
    long unsigned int *addr_filters_offs;
    long unsigned int addr_filters_gen;
    void (*destroy)(struct perf_event *);
    struct callback_head callback_head;
    struct pid_namespace *ns;
    u64 id;
    u64 (*clock)();
    perf_overflow_handler_t overflow_handler;
    void *overflow_handler_context;
    perf_overflow_handler_t orig_overflow_handler;
    struct bpf_prog *prog;
    struct trace_event_call *tp_event;
    struct event_filter *filter;
    struct ftrace_ops ftrace_ops;
    struct perf_cgroup *cgrp;
    struct list_head sb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct perf_event {
    struct list_head event_entry;
    struct list_head sibling_list;
    struct list_head active_list;
    struct rb_node group_node;
    u64 group_index;
    struct list_head migrate_entry;
    struct hlist_node hlist_entry;
    struct list_head active_entry;
    int nr_siblings;
    int event_caps;
    int group_caps;
    struct perf_event *group_leader;
    struct pmu *pmu;
    void *pmu_private;
    enum perf_event_state state;
    unsigned int attach_state;
    local64_t count;
    atomic64_t child_count;
    u64 total_time_enabled;
    u64 total_time_running;
    u64 tstamp;
    u64 shadow_ctx_time;
    struct perf_event_attr attr;
    u16 header_size;
    u16 id_header_size;
    u16 read_size;
    struct hw_perf_event hw;
    struct perf_event_context *ctx;
    atomic_long_t refcount;
    atomic64_t child_total_time_enabled;
    atomic64_t child_total_time_running;
    struct mutex child_mutex;
    struct list_head child_list;
    struct perf_event *parent;
    int oncpu;
    int cpu;
    struct list_head owner_entry;
    struct task_struct *owner;
    struct mutex mmap_mutex;
    atomic_t mmap_count;
    struct ring_buffer *rb;
    struct list_head rb_entry;
    long unsigned int rcu_batches;
    int rcu_pending;
    wait_queue_head_t waitq;
    struct fasync_struct *fasync;
    int pending_wakeup;
    int pending_kill;
    int pending_disable;
    struct irq_work pending;
    atomic_t event_limit;
    struct perf_addr_filters_head addr_filters;
    long unsigned int *addr_filters_offs;
    long unsigned int addr_filters_gen;
    void (*destroy)(struct perf_event *);
    struct callback_head callback_head;
    struct pid_namespace *ns;
    u64 id;
    u64 (*clock)();
    perf_overflow_handler_t overflow_handler;
    void *overflow_handler_context;
    perf_overflow_handler_t orig_overflow_handler;
    struct bpf_prog *prog;
    struct trace_event_call *tp_event;
    struct event_filter *filter;
    struct ftrace_ops ftrace_ops;
    struct perf_cgroup *cgrp;
    struct list_head sb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct perf_event {
    struct list_head event_entry;
    struct list_head sibling_list;
    struct list_head active_list;
    struct rb_node group_node;
    u64 group_index;
    struct list_head migrate_entry;
    struct hlist_node hlist_entry;
    struct list_head active_entry;
    int nr_siblings;
    int event_caps;
    int group_caps;
    struct perf_event *group_leader;
    struct pmu *pmu;
    void *pmu_private;
    enum perf_event_state state;
    unsigned int attach_state;
    local64_t count;
    atomic64_t child_count;
    u64 total_time_enabled;
    u64 total_time_running;
    u64 tstamp;
    u64 shadow_ctx_time;
    struct perf_event_attr attr;
    u16 header_size;
    u16 id_header_size;
    u16 read_size;
    struct hw_perf_event hw;
    struct perf_event_context *ctx;
    atomic_long_t refcount;
    atomic64_t child_total_time_enabled;
    atomic64_t child_total_time_running;
    struct mutex child_mutex;
    struct list_head child_list;
    struct perf_event *parent;
    int oncpu;
    int cpu;
    struct list_head owner_entry;
    struct task_struct *owner;
    struct mutex mmap_mutex;
    atomic_t mmap_count;
    struct ring_buffer *rb;
    struct list_head rb_entry;
    long unsigned int rcu_batches;
    int rcu_pending;
    wait_queue_head_t waitq;
    struct fasync_struct *fasync;
    int pending_wakeup;
    int pending_kill;
    int pending_disable;
    struct irq_work pending;
    atomic_t event_limit;
    struct perf_addr_filters_head addr_filters;
    struct perf_addr_filter_range *addr_filter_ranges;
    long unsigned int addr_filters_gen;
    void (*destroy)(struct perf_event *);
    struct callback_head callback_head;
    struct pid_namespace *ns;
    u64 id;
    u64 (*clock)();
    perf_overflow_handler_t overflow_handler;
    void *overflow_handler_context;
    perf_overflow_handler_t orig_overflow_handler;
    struct bpf_prog *prog;
    struct trace_event_call *tp_event;
    struct event_filter *filter;
    struct ftrace_ops ftrace_ops;
    struct perf_cgroup *cgrp;
    struct list_head sb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct perf_event {
    struct list_head event_entry;
    struct list_head sibling_list;
    struct list_head active_list;
    struct rb_node group_node;
    u64 group_index;
    struct list_head migrate_entry;
    struct hlist_node hlist_entry;
    struct list_head active_entry;
    int nr_siblings;
    int event_caps;
    int group_caps;
    struct perf_event *group_leader;
    struct pmu *pmu;
    void *pmu_private;
    enum perf_event_state state;
    unsigned int attach_state;
    local64_t count;
    atomic64_t child_count;
    u64 total_time_enabled;
    u64 total_time_running;
    u64 tstamp;
    u64 shadow_ctx_time;
    struct perf_event_attr attr;
    u16 header_size;
    u16 id_header_size;
    u16 read_size;
    struct hw_perf_event hw;
    struct perf_event_context *ctx;
    atomic_long_t refcount;
    atomic64_t child_total_time_enabled;
    atomic64_t child_total_time_running;
    struct mutex child_mutex;
    struct list_head child_list;
    struct perf_event *parent;
    int oncpu;
    int cpu;
    struct list_head owner_entry;
    struct task_struct *owner;
    struct mutex mmap_mutex;
    atomic_t mmap_count;
    struct ring_buffer *rb;
    struct list_head rb_entry;
    long unsigned int rcu_batches;
    int rcu_pending;
    wait_queue_head_t waitq;
    struct fasync_struct *fasync;
    int pending_wakeup;
    int pending_kill;
    int pending_disable;
    struct irq_work pending;
    atomic_t event_limit;
    struct perf_addr_filters_head addr_filters;
    struct perf_addr_filter_range *addr_filter_ranges;
    long unsigned int addr_filters_gen;
    struct perf_event *aux_event;
    void (*destroy)(struct perf_event *);
    struct callback_head callback_head;
    struct pid_namespace *ns;
    u64 id;
    u64 (*clock)();
    perf_overflow_handler_t overflow_handler;
    void *overflow_handler_context;
    perf_overflow_handler_t orig_overflow_handler;
    struct bpf_prog *prog;
    struct trace_event_call *tp_event;
    struct event_filter *filter;
    struct ftrace_ops ftrace_ops;
    struct perf_cgroup *cgrp;
    struct list_head sb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct perf_event {
    struct list_head event_entry;
    struct list_head sibling_list;
    struct list_head active_list;
    struct rb_node group_node;
    u64 group_index;
    struct list_head migrate_entry;
    struct hlist_node hlist_entry;
    struct list_head active_entry;
    int nr_siblings;
    int event_caps;
    int group_caps;
    struct perf_event *group_leader;
    struct pmu *pmu;
    void *pmu_private;
    enum perf_event_state state;
    unsigned int attach_state;
    local64_t count;
    atomic64_t child_count;
    u64 total_time_enabled;
    u64 total_time_running;
    u64 tstamp;
    u64 shadow_ctx_time;
    struct perf_event_attr attr;
    u16 header_size;
    u16 id_header_size;
    u16 read_size;
    struct hw_perf_event hw;
    struct perf_event_context *ctx;
    atomic_long_t refcount;
    atomic64_t child_total_time_enabled;
    atomic64_t child_total_time_running;
    struct mutex child_mutex;
    struct list_head child_list;
    struct perf_event *parent;
    int oncpu;
    int cpu;
    struct list_head owner_entry;
    struct task_struct *owner;
    struct mutex mmap_mutex;
    atomic_t mmap_count;
    struct perf_buffer *rb;
    struct list_head rb_entry;
    long unsigned int rcu_batches;
    int rcu_pending;
    wait_queue_head_t waitq;
    struct fasync_struct *fasync;
    int pending_wakeup;
    int pending_kill;
    int pending_disable;
    struct irq_work pending;
    atomic_t event_limit;
    struct perf_addr_filters_head addr_filters;
    struct perf_addr_filter_range *addr_filter_ranges;
    long unsigned int addr_filters_gen;
    struct perf_event *aux_event;
    void (*destroy)(struct perf_event *);
    struct callback_head callback_head;
    struct pid_namespace *ns;
    u64 id;
    u64 (*clock)();
    perf_overflow_handler_t overflow_handler;
    void *overflow_handler_context;
    perf_overflow_handler_t orig_overflow_handler;
    struct bpf_prog *prog;
    struct trace_event_call *tp_event;
    struct event_filter *filter;
    struct ftrace_ops ftrace_ops;
    struct perf_cgroup *cgrp;
    void *security;
    struct list_head sb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct perf_event {
    struct list_head event_entry;
    struct list_head sibling_list;
    struct list_head active_list;
    struct rb_node group_node;
    u64 group_index;
    struct list_head migrate_entry;
    struct hlist_node hlist_entry;
    struct list_head active_entry;
    int nr_siblings;
    int event_caps;
    int group_caps;
    struct perf_event *group_leader;
    struct pmu *pmu;
    void *pmu_private;
    enum perf_event_state state;
    unsigned int attach_state;
    local64_t count;
    atomic64_t child_count;
    u64 total_time_enabled;
    u64 total_time_running;
    u64 tstamp;
    u64 shadow_ctx_time;
    struct perf_event_attr attr;
    u16 header_size;
    u16 id_header_size;
    u16 read_size;
    struct hw_perf_event hw;
    struct perf_event_context *ctx;
    atomic_long_t refcount;
    atomic64_t child_total_time_enabled;
    atomic64_t child_total_time_running;
    struct mutex child_mutex;
    struct list_head child_list;
    struct perf_event *parent;
    int oncpu;
    int cpu;
    struct list_head owner_entry;
    struct task_struct *owner;
    struct mutex mmap_mutex;
    atomic_t mmap_count;
    struct perf_buffer *rb;
    struct list_head rb_entry;
    long unsigned int rcu_batches;
    int rcu_pending;
    wait_queue_head_t waitq;
    struct fasync_struct *fasync;
    int pending_wakeup;
    int pending_kill;
    int pending_disable;
    struct irq_work pending;
    atomic_t event_limit;
    struct perf_addr_filters_head addr_filters;
    struct perf_addr_filter_range *addr_filter_ranges;
    long unsigned int addr_filters_gen;
    struct perf_event *aux_event;
    void (*destroy)(struct perf_event *);
    struct callback_head callback_head;
    struct pid_namespace *ns;
    u64 id;
    u64 (*clock)();
    perf_overflow_handler_t overflow_handler;
    void *overflow_handler_context;
    perf_overflow_handler_t orig_overflow_handler;
    struct bpf_prog *prog;
    struct trace_event_call *tp_event;
    struct event_filter *filter;
    struct ftrace_ops ftrace_ops;
    struct perf_cgroup *cgrp;
    void *security;
    struct list_head sb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct perf_event {
    struct list_head event_entry;
    struct list_head sibling_list;
    struct list_head active_list;
    struct rb_node group_node;
    u64 group_index;
    struct list_head migrate_entry;
    struct hlist_node hlist_entry;
    struct list_head active_entry;
    int nr_siblings;
    int event_caps;
    int group_caps;
    struct perf_event *group_leader;
    struct pmu *pmu;
    void *pmu_private;
    enum perf_event_state state;
    unsigned int attach_state;
    local64_t count;
    atomic64_t child_count;
    u64 total_time_enabled;
    u64 total_time_running;
    u64 tstamp;
    u64 shadow_ctx_time;
    struct perf_event_attr attr;
    u16 header_size;
    u16 id_header_size;
    u16 read_size;
    struct hw_perf_event hw;
    struct perf_event_context *ctx;
    atomic_long_t refcount;
    atomic64_t child_total_time_enabled;
    atomic64_t child_total_time_running;
    struct mutex child_mutex;
    struct list_head child_list;
    struct perf_event *parent;
    int oncpu;
    int cpu;
    struct list_head owner_entry;
    struct task_struct *owner;
    struct mutex mmap_mutex;
    atomic_t mmap_count;
    struct perf_buffer *rb;
    struct list_head rb_entry;
    long unsigned int rcu_batches;
    int rcu_pending;
    wait_queue_head_t waitq;
    struct fasync_struct *fasync;
    int pending_wakeup;
    int pending_kill;
    int pending_disable;
    long unsigned int pending_addr;
    struct irq_work pending;
    atomic_t event_limit;
    struct perf_addr_filters_head addr_filters;
    struct perf_addr_filter_range *addr_filter_ranges;
    long unsigned int addr_filters_gen;
    struct perf_event *aux_event;
    void (*destroy)(struct perf_event *);
    struct callback_head callback_head;
    struct pid_namespace *ns;
    u64 id;
    u64 (*clock)();
    perf_overflow_handler_t overflow_handler;
    void *overflow_handler_context;
    perf_overflow_handler_t orig_overflow_handler;
    struct bpf_prog *prog;
    struct trace_event_call *tp_event;
    struct event_filter *filter;
    struct ftrace_ops ftrace_ops;
    struct perf_cgroup *cgrp;
    void *security;
    struct list_head sb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct perf_event {
    struct list_head event_entry;
    struct list_head sibling_list;
    struct list_head active_list;
    struct rb_node group_node;
    u64 group_index;
    struct list_head migrate_entry;
    struct hlist_node hlist_entry;
    struct list_head active_entry;
    int nr_siblings;
    int event_caps;
    int group_caps;
    struct perf_event *group_leader;
    struct pmu *pmu;
    void *pmu_private;
    enum perf_event_state state;
    unsigned int attach_state;
    local64_t count;
    atomic64_t child_count;
    u64 total_time_enabled;
    u64 total_time_running;
    u64 tstamp;
    struct perf_event_attr attr;
    u16 header_size;
    u16 id_header_size;
    u16 read_size;
    struct hw_perf_event hw;
    struct perf_event_context *ctx;
    atomic_long_t refcount;
    atomic64_t child_total_time_enabled;
    atomic64_t child_total_time_running;
    struct mutex child_mutex;
    struct list_head child_list;
    struct perf_event *parent;
    int oncpu;
    int cpu;
    struct list_head owner_entry;
    struct task_struct *owner;
    struct mutex mmap_mutex;
    atomic_t mmap_count;
    struct perf_buffer *rb;
    struct list_head rb_entry;
    long unsigned int rcu_batches;
    int rcu_pending;
    wait_queue_head_t waitq;
    struct fasync_struct *fasync;
    int pending_wakeup;
    int pending_kill;
    int pending_disable;
    long unsigned int pending_addr;
    struct irq_work pending;
    atomic_t event_limit;
    struct perf_addr_filters_head addr_filters;
    struct perf_addr_filter_range *addr_filter_ranges;
    long unsigned int addr_filters_gen;
    struct perf_event *aux_event;
    void (*destroy)(struct perf_event *);
    struct callback_head callback_head;
    struct pid_namespace *ns;
    u64 id;
    u64 (*clock)();
    perf_overflow_handler_t overflow_handler;
    void *overflow_handler_context;
    perf_overflow_handler_t orig_overflow_handler;
    struct bpf_prog *prog;
    u64 bpf_cookie;
    struct trace_event_call *tp_event;
    struct event_filter *filter;
    struct ftrace_ops ftrace_ops;
    struct perf_cgroup *cgrp;
    void *security;
    struct list_head sb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct perf_event {
    struct list_head event_entry;
    struct list_head sibling_list;
    struct list_head active_list;
    struct rb_node group_node;
    u64 group_index;
    struct list_head migrate_entry;
    struct hlist_node hlist_entry;
    struct list_head active_entry;
    int nr_siblings;
    int event_caps;
    int group_caps;
    struct perf_event *group_leader;
    struct pmu *pmu;
    void *pmu_private;
    enum perf_event_state state;
    unsigned int attach_state;
    local64_t count;
    atomic64_t child_count;
    u64 total_time_enabled;
    u64 total_time_running;
    u64 tstamp;
    struct perf_event_attr attr;
    u16 header_size;
    u16 id_header_size;
    u16 read_size;
    struct hw_perf_event hw;
    struct perf_event_context *ctx;
    atomic_long_t refcount;
    atomic64_t child_total_time_enabled;
    atomic64_t child_total_time_running;
    struct mutex child_mutex;
    struct list_head child_list;
    struct perf_event *parent;
    int oncpu;
    int cpu;
    struct list_head owner_entry;
    struct task_struct *owner;
    struct mutex mmap_mutex;
    atomic_t mmap_count;
    struct perf_buffer *rb;
    struct list_head rb_entry;
    long unsigned int rcu_batches;
    int rcu_pending;
    wait_queue_head_t waitq;
    struct fasync_struct *fasync;
    int pending_wakeup;
    int pending_kill;
    int pending_disable;
    long unsigned int pending_addr;
    struct irq_work pending;
    atomic_t event_limit;
    struct perf_addr_filters_head addr_filters;
    struct perf_addr_filter_range *addr_filter_ranges;
    long unsigned int addr_filters_gen;
    struct perf_event *aux_event;
    void (*destroy)(struct perf_event *);
    struct callback_head callback_head;
    struct pid_namespace *ns;
    u64 id;
    u64 (*clock)();
    perf_overflow_handler_t overflow_handler;
    void *overflow_handler_context;
    perf_overflow_handler_t orig_overflow_handler;
    struct bpf_prog *prog;
    u64 bpf_cookie;
    struct trace_event_call *tp_event;
    struct event_filter *filter;
    struct ftrace_ops ftrace_ops;
    struct perf_cgroup *cgrp;
    void *security;
    struct list_head sb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct perf_event {
    struct list_head event_entry;
    struct list_head sibling_list;
    struct list_head active_list;
    struct rb_node group_node;
    u64 group_index;
    struct list_head migrate_entry;
    struct hlist_node hlist_entry;
    struct list_head active_entry;
    int nr_siblings;
    int event_caps;
    int group_caps;
    struct perf_event *group_leader;
    struct pmu *pmu;
    void *pmu_private;
    enum perf_event_state state;
    unsigned int attach_state;
    local64_t count;
    atomic64_t child_count;
    u64 total_time_enabled;
    u64 total_time_running;
    u64 tstamp;
    struct perf_event_attr attr;
    u16 header_size;
    u16 id_header_size;
    u16 read_size;
    struct hw_perf_event hw;
    struct perf_event_context *ctx;
    struct perf_event_pmu_context *pmu_ctx;
    atomic_long_t refcount;
    atomic64_t child_total_time_enabled;
    atomic64_t child_total_time_running;
    struct mutex child_mutex;
    struct list_head child_list;
    struct perf_event *parent;
    int oncpu;
    int cpu;
    struct list_head owner_entry;
    struct task_struct *owner;
    struct mutex mmap_mutex;
    atomic_t mmap_count;
    struct perf_buffer *rb;
    struct list_head rb_entry;
    long unsigned int rcu_batches;
    int rcu_pending;
    wait_queue_head_t waitq;
    struct fasync_struct *fasync;
    unsigned int pending_wakeup;
    unsigned int pending_kill;
    unsigned int pending_disable;
    unsigned int pending_sigtrap;
    long unsigned int pending_addr;
    struct irq_work pending_irq;
    struct callback_head pending_task;
    unsigned int pending_work;
    atomic_t event_limit;
    struct perf_addr_filters_head addr_filters;
    struct perf_addr_filter_range *addr_filter_ranges;
    long unsigned int addr_filters_gen;
    struct perf_event *aux_event;
    void (*destroy)(struct perf_event *);
    struct callback_head callback_head;
    struct pid_namespace *ns;
    u64 id;
    atomic64_t lost_samples;
    u64 (*clock)();
    perf_overflow_handler_t overflow_handler;
    void *overflow_handler_context;
    perf_overflow_handler_t orig_overflow_handler;
    struct bpf_prog *prog;
    u64 bpf_cookie;
    struct trace_event_call *tp_event;
    struct event_filter *filter;
    struct ftrace_ops ftrace_ops;
    struct perf_cgroup *cgrp;
    void *security;
    struct list_head sb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct perf_event {
    struct list_head event_entry;
    struct list_head sibling_list;
    struct list_head active_list;
    struct rb_node group_node;
    u64 group_index;
    struct list_head migrate_entry;
    struct hlist_node hlist_entry;
    struct list_head active_entry;
    int nr_siblings;
    int event_caps;
    int group_caps;
    struct perf_event *group_leader;
    struct pmu *pmu;
    void *pmu_private;
    enum perf_event_state state;
    unsigned int attach_state;
    local64_t count;
    atomic64_t child_count;
    u64 total_time_enabled;
    u64 total_time_running;
    u64 tstamp;
    struct perf_event_attr attr;
    u16 header_size;
    u16 id_header_size;
    u16 read_size;
    struct hw_perf_event hw;
    struct perf_event_context *ctx;
    struct perf_event_pmu_context *pmu_ctx;
    atomic_long_t refcount;
    atomic64_t child_total_time_enabled;
    atomic64_t child_total_time_running;
    struct mutex child_mutex;
    struct list_head child_list;
    struct perf_event *parent;
    int oncpu;
    int cpu;
    struct list_head owner_entry;
    struct task_struct *owner;
    struct mutex mmap_mutex;
    atomic_t mmap_count;
    struct perf_buffer *rb;
    struct list_head rb_entry;
    long unsigned int rcu_batches;
    int rcu_pending;
    wait_queue_head_t waitq;
    struct fasync_struct *fasync;
    unsigned int pending_wakeup;
    unsigned int pending_kill;
    unsigned int pending_disable;
    unsigned int pending_sigtrap;
    long unsigned int pending_addr;
    struct irq_work pending_irq;
    struct callback_head pending_task;
    unsigned int pending_work;
    atomic_t event_limit;
    struct perf_addr_filters_head addr_filters;
    struct perf_addr_filter_range *addr_filter_ranges;
    long unsigned int addr_filters_gen;
    struct perf_event *aux_event;
    void (*destroy)(struct perf_event *);
    struct callback_head callback_head;
    struct pid_namespace *ns;
    u64 id;
    atomic64_t lost_samples;
    u64 (*clock)();
    perf_overflow_handler_t overflow_handler;
    void *overflow_handler_context;
    perf_overflow_handler_t orig_overflow_handler;
    struct bpf_prog *prog;
    u64 bpf_cookie;
    struct trace_event_call *tp_event;
    struct event_filter *filter;
    struct ftrace_ops ftrace_ops;
    struct perf_cgroup *cgrp;
    void *security;
    struct list_head sb_list;
    __u32 orig_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct perf_event {
    struct list_head event_entry;
    struct list_head sibling_list;
    struct list_head active_list;
    struct rb_node group_node;
    u64 group_index;
    struct list_head migrate_entry;
    struct hlist_node hlist_entry;
    struct list_head active_entry;
    int nr_siblings;
    int event_caps;
    int group_caps;
    unsigned int group_generation;
    struct perf_event *group_leader;
    struct pmu *pmu;
    void *pmu_private;
    enum perf_event_state state;
    unsigned int attach_state;
    local64_t count;
    atomic64_t child_count;
    u64 total_time_enabled;
    u64 total_time_running;
    u64 tstamp;
    struct perf_event_attr attr;
    u16 header_size;
    u16 id_header_size;
    u16 read_size;
    struct hw_perf_event hw;
    struct perf_event_context *ctx;
    struct perf_event_pmu_context *pmu_ctx;
    atomic_long_t refcount;
    atomic64_t child_total_time_enabled;
    atomic64_t child_total_time_running;
    struct mutex child_mutex;
    struct list_head child_list;
    struct perf_event *parent;
    int oncpu;
    int cpu;
    struct list_head owner_entry;
    struct task_struct *owner;
    struct mutex mmap_mutex;
    atomic_t mmap_count;
    struct perf_buffer *rb;
    struct list_head rb_entry;
    long unsigned int rcu_batches;
    int rcu_pending;
    wait_queue_head_t waitq;
    struct fasync_struct *fasync;
    unsigned int pending_wakeup;
    unsigned int pending_kill;
    unsigned int pending_disable;
    unsigned int pending_sigtrap;
    long unsigned int pending_addr;
    struct irq_work pending_irq;
    struct callback_head pending_task;
    unsigned int pending_work;
    atomic_t event_limit;
    struct perf_addr_filters_head addr_filters;
    struct perf_addr_filter_range *addr_filter_ranges;
    long unsigned int addr_filters_gen;
    struct perf_event *aux_event;
    void (*destroy)(struct perf_event *);
    struct callback_head callback_head;
    struct pid_namespace *ns;
    u64 id;
    atomic64_t lost_samples;
    u64 (*clock)();
    perf_overflow_handler_t overflow_handler;
    void *overflow_handler_context;
    perf_overflow_handler_t orig_overflow_handler;
    struct bpf_prog *prog;
    u64 bpf_cookie;
    struct trace_event_call *tp_event;
    struct event_filter *filter;
    struct ftrace_ops ftrace_ops;
    struct perf_cgroup *cgrp;
    void *security;
    struct list_head sb_list;
    __u32 orig_type;
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
struct perf_event {
    struct list_head event_entry;
    struct list_head sibling_list;
    struct list_head active_list;
    struct rb_node group_node;
    u64 group_index;
    struct list_head migrate_entry;
    struct hlist_node hlist_entry;
    struct list_head active_entry;
    int nr_siblings;
    int event_caps;
    int group_caps;
    struct perf_event *group_leader;
    struct pmu *pmu;
    void *pmu_private;
    enum perf_event_state state;
    unsigned int attach_state;
    local64_t count;
    atomic64_t child_count;
    u64 total_time_enabled;
    u64 total_time_running;
    u64 tstamp;
    u64 shadow_ctx_time;
    struct perf_event_attr attr;
    u16 header_size;
    u16 id_header_size;
    u16 read_size;
    struct hw_perf_event hw;
    struct perf_event_context *ctx;
    atomic_long_t refcount;
    atomic64_t child_total_time_enabled;
    atomic64_t child_total_time_running;
    struct mutex child_mutex;
    struct list_head child_list;
    struct perf_event *parent;
    int oncpu;
    int cpu;
    struct list_head owner_entry;
    struct task_struct *owner;
    struct mutex mmap_mutex;
    atomic_t mmap_count;
    struct ring_buffer *rb;
    struct list_head rb_entry;
    long unsigned int rcu_batches;
    int rcu_pending;
    wait_queue_head_t waitq;
    struct fasync_struct *fasync;
    int pending_wakeup;
    int pending_kill;
    int pending_disable;
    struct irq_work pending;
    atomic_t event_limit;
    struct perf_addr_filters_head addr_filters;
    struct perf_addr_filter_range *addr_filter_ranges;
    long unsigned int addr_filters_gen;
    struct perf_event *aux_event;
    void (*destroy)(struct perf_event *);
    struct callback_head callback_head;
    struct pid_namespace *ns;
    u64 id;
    u64 (*clock)();
    perf_overflow_handler_t overflow_handler;
    void *overflow_handler_context;
    perf_overflow_handler_t orig_overflow_handler;
    struct bpf_prog *prog;
    struct trace_event_call *tp_event;
    struct event_filter *filter;
    struct ftrace_ops ftrace_ops;
    struct perf_cgroup *cgrp;
    struct list_head sb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct perf_event {
    struct list_head event_entry;
    struct list_head sibling_list;
    struct list_head active_list;
    struct rb_node group_node;
    u64 group_index;
    struct list_head migrate_entry;
    struct hlist_node hlist_entry;
    struct list_head active_entry;
    int nr_siblings;
    int event_caps;
    int group_caps;
    struct perf_event *group_leader;
    struct pmu *pmu;
    void *pmu_private;
    enum perf_event_state state;
    unsigned int attach_state;
    local64_t count;
    atomic64_t child_count;
    u64 total_time_enabled;
    u64 total_time_running;
    u64 tstamp;
    u64 shadow_ctx_time;
    struct perf_event_attr attr;
    u16 header_size;
    u16 id_header_size;
    u16 read_size;
    struct hw_perf_event hw;
    struct perf_event_context *ctx;
    atomic_long_t refcount;
    atomic64_t child_total_time_enabled;
    atomic64_t child_total_time_running;
    struct mutex child_mutex;
    struct list_head child_list;
    struct perf_event *parent;
    int oncpu;
    int cpu;
    struct list_head owner_entry;
    struct task_struct *owner;
    struct mutex mmap_mutex;
    atomic_t mmap_count;
    struct ring_buffer *rb;
    struct list_head rb_entry;
    long unsigned int rcu_batches;
    int rcu_pending;
    wait_queue_head_t waitq;
    struct fasync_struct *fasync;
    int pending_wakeup;
    int pending_kill;
    int pending_disable;
    struct irq_work pending;
    atomic_t event_limit;
    struct perf_addr_filters_head addr_filters;
    struct perf_addr_filter_range *addr_filter_ranges;
    long unsigned int addr_filters_gen;
    struct perf_event *aux_event;
    void (*destroy)(struct perf_event *);
    struct callback_head callback_head;
    struct pid_namespace *ns;
    u64 id;
    u64 (*clock)();
    perf_overflow_handler_t overflow_handler;
    void *overflow_handler_context;
    perf_overflow_handler_t orig_overflow_handler;
    struct bpf_prog *prog;
    struct trace_event_call *tp_event;
    struct event_filter *filter;
    struct ftrace_ops ftrace_ops;
    struct perf_cgroup *cgrp;
    struct list_head sb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct perf_event {
    struct list_head event_entry;
    struct list_head sibling_list;
    struct list_head active_list;
    struct rb_node group_node;
    u64 group_index;
    struct list_head migrate_entry;
    struct hlist_node hlist_entry;
    struct list_head active_entry;
    int nr_siblings;
    int event_caps;
    int group_caps;
    struct perf_event *group_leader;
    struct pmu *pmu;
    void *pmu_private;
    enum perf_event_state state;
    unsigned int attach_state;
    local64_t count;
    atomic64_t child_count;
    u64 total_time_enabled;
    u64 total_time_running;
    u64 tstamp;
    u64 shadow_ctx_time;
    struct perf_event_attr attr;
    u16 header_size;
    u16 id_header_size;
    u16 read_size;
    struct hw_perf_event hw;
    struct perf_event_context *ctx;
    atomic_long_t refcount;
    atomic64_t child_total_time_enabled;
    atomic64_t child_total_time_running;
    struct mutex child_mutex;
    struct list_head child_list;
    struct perf_event *parent;
    int oncpu;
    int cpu;
    struct list_head owner_entry;
    struct task_struct *owner;
    struct mutex mmap_mutex;
    atomic_t mmap_count;
    struct ring_buffer *rb;
    struct list_head rb_entry;
    long unsigned int rcu_batches;
    int rcu_pending;
    wait_queue_head_t waitq;
    struct fasync_struct *fasync;
    int pending_wakeup;
    int pending_kill;
    int pending_disable;
    struct irq_work pending;
    atomic_t event_limit;
    struct perf_addr_filters_head addr_filters;
    struct perf_addr_filter_range *addr_filter_ranges;
    long unsigned int addr_filters_gen;
    struct perf_event *aux_event;
    void (*destroy)(struct perf_event *);
    struct callback_head callback_head;
    struct pid_namespace *ns;
    u64 id;
    u64 (*clock)();
    perf_overflow_handler_t overflow_handler;
    void *overflow_handler_context;
    perf_overflow_handler_t orig_overflow_handler;
    struct bpf_prog *prog;
    struct trace_event_call *tp_event;
    struct event_filter *filter;
    struct ftrace_ops ftrace_ops;
    struct perf_cgroup *cgrp;
    struct list_head sb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct perf_event {
    struct list_head event_entry;
    struct list_head sibling_list;
    struct list_head active_list;
    struct rb_node group_node;
    u64 group_index;
    struct list_head migrate_entry;
    struct hlist_node hlist_entry;
    struct list_head active_entry;
    int nr_siblings;
    int event_caps;
    int group_caps;
    struct perf_event *group_leader;
    struct pmu *pmu;
    void *pmu_private;
    enum perf_event_state state;
    unsigned int attach_state;
    local64_t count;
    atomic64_t child_count;
    u64 total_time_enabled;
    u64 total_time_running;
    u64 tstamp;
    u64 shadow_ctx_time;
    struct perf_event_attr attr;
    u16 header_size;
    u16 id_header_size;
    u16 read_size;
    struct hw_perf_event hw;
    struct perf_event_context *ctx;
    atomic_long_t refcount;
    atomic64_t child_total_time_enabled;
    atomic64_t child_total_time_running;
    struct mutex child_mutex;
    struct list_head child_list;
    struct perf_event *parent;
    int oncpu;
    int cpu;
    struct list_head owner_entry;
    struct task_struct *owner;
    struct mutex mmap_mutex;
    atomic_t mmap_count;
    struct ring_buffer *rb;
    struct list_head rb_entry;
    long unsigned int rcu_batches;
    int rcu_pending;
    wait_queue_head_t waitq;
    struct fasync_struct *fasync;
    int pending_wakeup;
    int pending_kill;
    int pending_disable;
    struct irq_work pending;
    atomic_t event_limit;
    struct perf_addr_filters_head addr_filters;
    struct perf_addr_filter_range *addr_filter_ranges;
    long unsigned int addr_filters_gen;
    struct perf_event *aux_event;
    void (*destroy)(struct perf_event *);
    struct callback_head callback_head;
    struct pid_namespace *ns;
    u64 id;
    u64 (*clock)();
    perf_overflow_handler_t overflow_handler;
    void *overflow_handler_context;
    perf_overflow_handler_t orig_overflow_handler;
    struct bpf_prog *prog;
    struct trace_event_call *tp_event;
    struct event_filter *filter;
    struct ftrace_ops ftrace_ops;
    struct perf_cgroup *cgrp;
    struct list_head sb_list;
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
struct perf_event {
    struct list_head event_entry;
    struct list_head sibling_list;
    struct list_head active_list;
    struct rb_node group_node;
    u64 group_index;
    struct list_head migrate_entry;
    struct hlist_node hlist_entry;
    struct list_head active_entry;
    int nr_siblings;
    int event_caps;
    int group_caps;
    struct perf_event *group_leader;
    struct pmu *pmu;
    void *pmu_private;
    enum perf_event_state state;
    unsigned int attach_state;
    local64_t count;
    atomic64_t child_count;
    u64 total_time_enabled;
    u64 total_time_running;
    u64 tstamp;
    u64 shadow_ctx_time;
    struct perf_event_attr attr;
    u16 header_size;
    u16 id_header_size;
    u16 read_size;
    struct hw_perf_event hw;
    struct perf_event_context *ctx;
    atomic_long_t refcount;
    atomic64_t child_total_time_enabled;
    atomic64_t child_total_time_running;
    struct mutex child_mutex;
    struct list_head child_list;
    struct perf_event *parent;
    int oncpu;
    int cpu;
    struct list_head owner_entry;
    struct task_struct *owner;
    struct mutex mmap_mutex;
    atomic_t mmap_count;
    struct ring_buffer *rb;
    struct list_head rb_entry;
    long unsigned int rcu_batches;
    int rcu_pending;
    wait_queue_head_t waitq;
    struct fasync_struct *fasync;
    int pending_wakeup;
    int pending_kill;
    int pending_disable;
    struct irq_work pending;
    atomic_t event_limit;
    struct perf_addr_filters_head addr_filters;
    struct perf_addr_filter_range *addr_filter_ranges;
    long unsigned int addr_filters_gen;
    struct perf_event *aux_event;
    void (*destroy)(struct perf_event *);
    struct callback_head callback_head;
    struct pid_namespace *ns;
    u64 id;
    u64 (*clock)();
    perf_overflow_handler_t overflow_handler;
    void *overflow_handler_context;
    perf_overflow_handler_t orig_overflow_handler;
    struct bpf_prog *prog;
    struct trace_event_call *tp_event;
    struct event_filter *filter;
    struct ftrace_ops ftrace_ops;
    struct perf_cgroup *cgrp;
    struct list_head sb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct perf_event {
    struct list_head event_entry;
    struct list_head sibling_list;
    struct list_head active_list;
    struct rb_node group_node;
    u64 group_index;
    struct list_head migrate_entry;
    struct hlist_node hlist_entry;
    struct list_head active_entry;
    int nr_siblings;
    int event_caps;
    int group_caps;
    struct perf_event *group_leader;
    struct pmu *pmu;
    void *pmu_private;
    enum perf_event_state state;
    unsigned int attach_state;
    local64_t count;
    atomic64_t child_count;
    u64 total_time_enabled;
    u64 total_time_running;
    u64 tstamp;
    u64 shadow_ctx_time;
    struct perf_event_attr attr;
    u16 header_size;
    u16 id_header_size;
    u16 read_size;
    struct hw_perf_event hw;
    struct perf_event_context *ctx;
    atomic_long_t refcount;
    atomic64_t child_total_time_enabled;
    atomic64_t child_total_time_running;
    struct mutex child_mutex;
    struct list_head child_list;
    struct perf_event *parent;
    int oncpu;
    int cpu;
    struct list_head owner_entry;
    struct task_struct *owner;
    struct mutex mmap_mutex;
    atomic_t mmap_count;
    struct ring_buffer *rb;
    struct list_head rb_entry;
    long unsigned int rcu_batches;
    int rcu_pending;
    wait_queue_head_t waitq;
    struct fasync_struct *fasync;
    int pending_wakeup;
    int pending_kill;
    int pending_disable;
    struct irq_work pending;
    atomic_t event_limit;
    struct perf_addr_filters_head addr_filters;
    struct perf_addr_filter_range *addr_filter_ranges;
    long unsigned int addr_filters_gen;
    struct perf_event *aux_event;
    void (*destroy)(struct perf_event *);
    struct callback_head callback_head;
    struct pid_namespace *ns;
    u64 id;
    u64 (*clock)();
    perf_overflow_handler_t overflow_handler;
    void *overflow_handler_context;
    perf_overflow_handler_t orig_overflow_handler;
    struct bpf_prog *prog;
    struct trace_event_call *tp_event;
    struct event_filter *filter;
    struct ftrace_ops ftrace_ops;
    struct perf_cgroup *cgrp;
    struct list_head sb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct perf_event {
    struct list_head event_entry;
    struct list_head sibling_list;
    struct list_head active_list;
    struct rb_node group_node;
    u64 group_index;
    struct list_head migrate_entry;
    struct hlist_node hlist_entry;
    struct list_head active_entry;
    int nr_siblings;
    int event_caps;
    int group_caps;
    struct perf_event *group_leader;
    struct pmu *pmu;
    void *pmu_private;
    enum perf_event_state state;
    unsigned int attach_state;
    local64_t count;
    atomic64_t child_count;
    u64 total_time_enabled;
    u64 total_time_running;
    u64 tstamp;
    u64 shadow_ctx_time;
    struct perf_event_attr attr;
    u16 header_size;
    u16 id_header_size;
    u16 read_size;
    struct hw_perf_event hw;
    struct perf_event_context *ctx;
    atomic_long_t refcount;
    atomic64_t child_total_time_enabled;
    atomic64_t child_total_time_running;
    struct mutex child_mutex;
    struct list_head child_list;
    struct perf_event *parent;
    int oncpu;
    int cpu;
    struct list_head owner_entry;
    struct task_struct *owner;
    struct mutex mmap_mutex;
    atomic_t mmap_count;
    struct ring_buffer *rb;
    struct list_head rb_entry;
    long unsigned int rcu_batches;
    int rcu_pending;
    wait_queue_head_t waitq;
    struct fasync_struct *fasync;
    int pending_wakeup;
    int pending_kill;
    int pending_disable;
    struct irq_work pending;
    atomic_t event_limit;
    struct perf_addr_filters_head addr_filters;
    struct perf_addr_filter_range *addr_filter_ranges;
    long unsigned int addr_filters_gen;
    struct perf_event *aux_event;
    void (*destroy)(struct perf_event *);
    struct callback_head callback_head;
    struct pid_namespace *ns;
    u64 id;
    u64 (*clock)();
    perf_overflow_handler_t overflow_handler;
    void *overflow_handler_context;
    perf_overflow_handler_t orig_overflow_handler;
    struct bpf_prog *prog;
    struct trace_event_call *tp_event;
    struct event_filter *filter;
    struct ftrace_ops ftrace_ops;
    struct perf_cgroup *cgrp;
    struct list_head sb_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct perf_event {
    struct list_head event_entry;
    struct list_head sibling_list;
    struct list_head active_list;
    struct rb_node group_node;
    u64 group_index;
    struct list_head migrate_entry;
    struct hlist_node hlist_entry;
    struct list_head active_entry;
    int nr_siblings;
    int event_caps;
    int group_caps;
    struct perf_event *group_leader;
    struct pmu *pmu;
    void *pmu_private;
    enum perf_event_state state;
    unsigned int attach_state;
    local64_t count;
    atomic64_t child_count;
    u64 total_time_enabled;
    u64 total_time_running;
    u64 tstamp;
    u64 shadow_ctx_time;
    struct perf_event_attr attr;
    u16 header_size;
    u16 id_header_size;
    u16 read_size;
    struct hw_perf_event hw;
    struct perf_event_context *ctx;
    atomic_long_t refcount;
    atomic64_t child_total_time_enabled;
    atomic64_t child_total_time_running;
    struct mutex child_mutex;
    struct list_head child_list;
    struct perf_event *parent;
    int oncpu;
    int cpu;
    struct list_head owner_entry;
    struct task_struct *owner;
    struct mutex mmap_mutex;
    atomic_t mmap_count;
    struct ring_buffer *rb;
    struct list_head rb_entry;
    long unsigned int rcu_batches;
    int rcu_pending;
    wait_queue_head_t waitq;
    struct fasync_struct *fasync;
    int pending_wakeup;
    int pending_kill;
    int pending_disable;
    struct irq_work pending;
    atomic_t event_limit;
    struct perf_addr_filters_head addr_filters;
    struct perf_addr_filter_range *addr_filter_ranges;
    long unsigned int addr_filters_gen;
    struct perf_event *aux_event;
    void (*destroy)(struct perf_event *);
    struct callback_head callback_head;
    struct pid_namespace *ns;
    u64 id;
    u64 (*clock)();
    perf_overflow_handler_t overflow_handler;
    void *overflow_handler_context;
    perf_overflow_handler_t orig_overflow_handler;
    struct bpf_prog *prog;
    struct trace_event_call *tp_event;
    struct event_filter *filter;
    struct ftrace_ops ftrace_ops;
    struct perf_cgroup *cgrp;
    struct list_head sb_list;
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
<code>void *pmu_private</code>
</li>
<li>
<b>Field added. </b>
<code>struct perf_addr_filters_head addr_filters</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int *addr_filters_offs</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int addr_filters_gen</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head sb_list</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int event_caps</code>
</li>
<li>
<b>Field added. </b>
<code>int group_caps</code>
</li>
<li>
<b>Field added. </b>
<code>perf_overflow_handler_t orig_overflow_handler</code>
</li>
<li>
<b>Field added. </b>
<code>struct bpf_prog *prog</code>
</li>
<li>
<b>Field removed. </b>
<code>int group_flags</code>
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
<code>u64 tstamp</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 tstamp_enabled</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 tstamp_running</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 tstamp_stopped</code>
</li>
<li>
<b>Field removed. </b>
<code>int cgrp_defer_enabled</code>
</li>
<li>
<b>Field type changed. </b>
<code>enum perf_event_active_state state</code> ➡️ <code>enum perf_event_state state</code>
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
<code>struct list_head active_list</code>
</li>
<li>
<b>Field added. </b>
<code>struct rb_node group_node</code>
</li>
<li>
<b>Field added. </b>
<code>u64 group_index</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head group_entry</code>
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
<code>struct perf_addr_filter_range *addr_filter_ranges</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int *addr_filters_offs</code>
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
<code>struct perf_event *aux_event</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void *security</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct ring_buffer *rb</code> ➡️ <code>struct perf_buffer *rb</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int pending_addr</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 bpf_cookie</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 shadow_ctx_time</code>
</li>
</ul>
</details>
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
<code>struct perf_event_pmu_context *pmu_ctx</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int pending_sigtrap</code>
</li>
<li>
<b>Field added. </b>
<code>struct irq_work pending_irq</code>
</li>
<li>
<b>Field added. </b>
<code>struct callback_head pending_task</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int pending_work</code>
</li>
<li>
<b>Field added. </b>
<code>atomic64_t lost_samples</code>
</li>
<li>
<b>Field removed. </b>
<code>struct irq_work pending</code>
</li>
<li>
<b>Field type changed. </b>
<code>int pending_wakeup</code> ➡️ <code>unsigned int pending_wakeup</code>
</li>
<li>
<b>Field type changed. </b>
<code>int pending_kill</code> ➡️ <code>unsigned int pending_kill</code>
</li>
<li>
<b>Field type changed. </b>
<code>int pending_disable</code> ➡️ <code>unsigned int pending_disable</code>
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
<code>__u32 orig_type</code>
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
<code>unsigned int group_generation</code>
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
