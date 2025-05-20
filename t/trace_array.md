# Struct: <code>trace_array</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct trace_array {
    struct list_head list;
    char *name;
    struct trace_buffer trace_buffer;
    struct trace_buffer max_buffer;
    bool allocated_snapshot;
    long unsigned int max_latency;
    struct trace_pid_list *filtered_pids;
    arch_spinlock_t max_lock;
    int buffer_disabled;
    int sys_refcount_enter;
    int sys_refcount_exit;
    struct trace_event_file * enter_syscall_files[546];
    struct trace_event_file * exit_syscall_files[546];
    int stop_count;
    int clock_id;
    int nr_topts;
    struct tracer *current_trace;
    unsigned int trace_flags;
    unsigned char trace_flags_index[32];
    unsigned int flags;
    raw_spinlock_t start_lock;
    struct dentry *dir;
    struct dentry *options;
    struct dentry *percpu_dir;
    struct dentry *event_dir;
    struct trace_options *topts;
    struct list_head systems;
    struct list_head events;
    cpumask_var_t tracing_cpumask;
    int ref;
    struct ftrace_ops *ops;
    int function_enabled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct trace_array {
    struct list_head list;
    char *name;
    struct trace_buffer trace_buffer;
    struct trace_buffer max_buffer;
    bool allocated_snapshot;
    long unsigned int max_latency;
    struct trace_pid_list *filtered_pids;
    arch_spinlock_t max_lock;
    int buffer_disabled;
    int sys_refcount_enter;
    int sys_refcount_exit;
    struct trace_event_file * enter_syscall_files[548];
    struct trace_event_file * exit_syscall_files[548];
    int stop_count;
    int clock_id;
    int nr_topts;
    struct tracer *current_trace;
    unsigned int trace_flags;
    unsigned char trace_flags_index[32];
    unsigned int flags;
    raw_spinlock_t start_lock;
    struct dentry *dir;
    struct dentry *options;
    struct dentry *percpu_dir;
    struct dentry *event_dir;
    struct trace_options *topts;
    struct list_head systems;
    struct list_head events;
    cpumask_var_t tracing_cpumask;
    int ref;
    struct ftrace_ops *ops;
    struct trace_pid_list *function_pids;
    int function_enabled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct trace_array {
    struct list_head list;
    char *name;
    struct trace_buffer trace_buffer;
    struct trace_buffer max_buffer;
    bool allocated_snapshot;
    long unsigned int max_latency;
    struct trace_pid_list *filtered_pids;
    arch_spinlock_t max_lock;
    int buffer_disabled;
    int sys_refcount_enter;
    int sys_refcount_exit;
    struct trace_event_file * enter_syscall_files[548];
    struct trace_event_file * exit_syscall_files[548];
    int stop_count;
    int clock_id;
    int nr_topts;
    struct tracer *current_trace;
    unsigned int trace_flags;
    unsigned char trace_flags_index[32];
    unsigned int flags;
    raw_spinlock_t start_lock;
    struct dentry *dir;
    struct dentry *options;
    struct dentry *percpu_dir;
    struct dentry *event_dir;
    struct trace_options *topts;
    struct list_head systems;
    struct list_head events;
    cpumask_var_t tracing_cpumask;
    int ref;
    struct ftrace_ops *ops;
    struct trace_pid_list *function_pids;
    int function_enabled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct trace_array {
    struct list_head list;
    char *name;
    struct trace_buffer trace_buffer;
    struct trace_buffer max_buffer;
    bool allocated_snapshot;
    long unsigned int max_latency;
    struct trace_pid_list *filtered_pids;
    arch_spinlock_t max_lock;
    int buffer_disabled;
    int sys_refcount_enter;
    int sys_refcount_exit;
    struct trace_event_file * enter_syscall_files[548];
    struct trace_event_file * exit_syscall_files[548];
    int stop_count;
    int clock_id;
    int nr_topts;
    struct tracer *current_trace;
    unsigned int trace_flags;
    unsigned char trace_flags_index[32];
    unsigned int flags;
    raw_spinlock_t start_lock;
    struct dentry *dir;
    struct dentry *options;
    struct dentry *percpu_dir;
    struct dentry *event_dir;
    struct trace_options *topts;
    struct list_head systems;
    struct list_head events;
    cpumask_var_t tracing_cpumask;
    int ref;
    struct ftrace_ops *ops;
    struct trace_pid_list *function_pids;
    struct list_head func_probes;
    struct list_head mod_trace;
    struct list_head mod_notrace;
    int function_enabled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct trace_array {
    struct list_head list;
    char *name;
    struct trace_buffer trace_buffer;
    struct trace_buffer max_buffer;
    bool allocated_snapshot;
    long unsigned int max_latency;
    struct trace_pid_list *filtered_pids;
    arch_spinlock_t max_lock;
    int buffer_disabled;
    int sys_refcount_enter;
    int sys_refcount_exit;
    struct trace_event_file * enter_syscall_files[548];
    struct trace_event_file * exit_syscall_files[548];
    int stop_count;
    int clock_id;
    int nr_topts;
    bool clear_trace;
    struct tracer *current_trace;
    unsigned int trace_flags;
    unsigned char trace_flags_index[32];
    unsigned int flags;
    raw_spinlock_t start_lock;
    struct dentry *dir;
    struct dentry *options;
    struct dentry *percpu_dir;
    struct dentry *event_dir;
    struct trace_options *topts;
    struct list_head systems;
    struct list_head events;
    cpumask_var_t tracing_cpumask;
    int ref;
    struct ftrace_ops *ops;
    struct trace_pid_list *function_pids;
    struct list_head func_probes;
    struct list_head mod_trace;
    struct list_head mod_notrace;
    int function_enabled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct trace_array {
    struct list_head list;
    char *name;
    struct trace_buffer trace_buffer;
    struct trace_buffer max_buffer;
    bool allocated_snapshot;
    long unsigned int max_latency;
    struct trace_pid_list *filtered_pids;
    arch_spinlock_t max_lock;
    int buffer_disabled;
    int sys_refcount_enter;
    int sys_refcount_exit;
    struct trace_event_file * enter_syscall_files[548];
    struct trace_event_file * exit_syscall_files[548];
    int stop_count;
    int clock_id;
    int nr_topts;
    bool clear_trace;
    struct tracer *current_trace;
    unsigned int trace_flags;
    unsigned char trace_flags_index[32];
    unsigned int flags;
    raw_spinlock_t start_lock;
    struct dentry *dir;
    struct dentry *options;
    struct dentry *percpu_dir;
    struct dentry *event_dir;
    struct trace_options *topts;
    struct list_head systems;
    struct list_head events;
    struct trace_event_file *trace_marker_file;
    cpumask_var_t tracing_cpumask;
    int ref;
    struct ftrace_ops *ops;
    struct trace_pid_list *function_pids;
    struct list_head func_probes;
    struct list_head mod_trace;
    struct list_head mod_notrace;
    int function_enabled;
    int time_stamp_abs_ref;
    struct list_head hist_vars;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct trace_array {
    struct list_head list;
    char *name;
    struct trace_buffer trace_buffer;
    struct trace_buffer max_buffer;
    bool allocated_snapshot;
    long unsigned int max_latency;
    struct trace_pid_list *filtered_pids;
    arch_spinlock_t max_lock;
    int buffer_disabled;
    int sys_refcount_enter;
    int sys_refcount_exit;
    struct trace_event_file * enter_syscall_files[548];
    struct trace_event_file * exit_syscall_files[548];
    int stop_count;
    int clock_id;
    int nr_topts;
    bool clear_trace;
    int buffer_percent;
    struct tracer *current_trace;
    unsigned int trace_flags;
    unsigned char trace_flags_index[32];
    unsigned int flags;
    raw_spinlock_t start_lock;
    struct dentry *dir;
    struct dentry *options;
    struct dentry *percpu_dir;
    struct dentry *event_dir;
    struct trace_options *topts;
    struct list_head systems;
    struct list_head events;
    struct trace_event_file *trace_marker_file;
    cpumask_var_t tracing_cpumask;
    int ref;
    struct ftrace_ops *ops;
    struct trace_pid_list *function_pids;
    struct list_head func_probes;
    struct list_head mod_trace;
    struct list_head mod_notrace;
    int function_enabled;
    int time_stamp_abs_ref;
    struct list_head hist_vars;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct trace_array {
    struct list_head list;
    char *name;
    struct trace_buffer trace_buffer;
    struct trace_buffer max_buffer;
    bool allocated_snapshot;
    long unsigned int max_latency;
    struct trace_pid_list *filtered_pids;
    arch_spinlock_t max_lock;
    int buffer_disabled;
    int sys_refcount_enter;
    int sys_refcount_exit;
    struct trace_event_file * enter_syscall_files[548];
    struct trace_event_file * exit_syscall_files[548];
    int stop_count;
    int clock_id;
    int nr_topts;
    bool clear_trace;
    int buffer_percent;
    unsigned int n_err_log_entries;
    struct tracer *current_trace;
    unsigned int trace_flags;
    unsigned char trace_flags_index[32];
    unsigned int flags;
    raw_spinlock_t start_lock;
    struct list_head err_log;
    struct dentry *dir;
    struct dentry *options;
    struct dentry *percpu_dir;
    struct dentry *event_dir;
    struct trace_options *topts;
    struct list_head systems;
    struct list_head events;
    struct trace_event_file *trace_marker_file;
    cpumask_var_t tracing_cpumask;
    int ref;
    struct ftrace_ops *ops;
    struct trace_pid_list *function_pids;
    struct list_head func_probes;
    struct list_head mod_trace;
    struct list_head mod_notrace;
    int function_enabled;
    int time_stamp_abs_ref;
    struct list_head hist_vars;
    struct cond_snapshot *cond_snapshot;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct trace_array {
    struct list_head list;
    char *name;
    struct trace_buffer trace_buffer;
    struct trace_buffer max_buffer;
    bool allocated_snapshot;
    long unsigned int max_latency;
    struct trace_pid_list *filtered_pids;
    arch_spinlock_t max_lock;
    int buffer_disabled;
    int sys_refcount_enter;
    int sys_refcount_exit;
    struct trace_event_file * enter_syscall_files[436];
    struct trace_event_file * exit_syscall_files[436];
    int stop_count;
    int clock_id;
    int nr_topts;
    bool clear_trace;
    int buffer_percent;
    unsigned int n_err_log_entries;
    struct tracer *current_trace;
    unsigned int trace_flags;
    unsigned char trace_flags_index[32];
    unsigned int flags;
    raw_spinlock_t start_lock;
    struct list_head err_log;
    struct dentry *dir;
    struct dentry *options;
    struct dentry *percpu_dir;
    struct dentry *event_dir;
    struct trace_options *topts;
    struct list_head systems;
    struct list_head events;
    struct trace_event_file *trace_marker_file;
    cpumask_var_t tracing_cpumask;
    int ref;
    struct ftrace_ops *ops;
    struct trace_pid_list *function_pids;
    struct list_head func_probes;
    struct list_head mod_trace;
    struct list_head mod_notrace;
    int function_enabled;
    int time_stamp_abs_ref;
    struct list_head hist_vars;
    struct cond_snapshot *cond_snapshot;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct trace_array {
    struct list_head list;
    char *name;
    struct array_buffer array_buffer;
    struct array_buffer max_buffer;
    bool allocated_snapshot;
    long unsigned int max_latency;
    struct dentry *d_max_latency;
    struct work_struct fsnotify_work;
    struct irq_work fsnotify_irqwork;
    struct trace_pid_list *filtered_pids;
    struct trace_pid_list *filtered_no_pids;
    arch_spinlock_t max_lock;
    int buffer_disabled;
    int sys_refcount_enter;
    int sys_refcount_exit;
    struct trace_event_file * enter_syscall_files[440];
    struct trace_event_file * exit_syscall_files[440];
    int stop_count;
    int clock_id;
    int nr_topts;
    bool clear_trace;
    int buffer_percent;
    unsigned int n_err_log_entries;
    struct tracer *current_trace;
    unsigned int trace_flags;
    unsigned char trace_flags_index[32];
    unsigned int flags;
    raw_spinlock_t start_lock;
    struct list_head err_log;
    struct dentry *dir;
    struct dentry *options;
    struct dentry *percpu_dir;
    struct dentry *event_dir;
    struct trace_options *topts;
    struct list_head systems;
    struct list_head events;
    struct trace_event_file *trace_marker_file;
    cpumask_var_t tracing_cpumask;
    int ref;
    int trace_ref;
    struct ftrace_ops *ops;
    struct trace_pid_list *function_pids;
    struct trace_pid_list *function_no_pids;
    struct list_head func_probes;
    struct list_head mod_trace;
    struct list_head mod_notrace;
    int function_enabled;
    int time_stamp_abs_ref;
    struct list_head hist_vars;
    struct cond_snapshot *cond_snapshot;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct trace_array {
    struct list_head list;
    char *name;
    struct array_buffer array_buffer;
    struct array_buffer max_buffer;
    bool allocated_snapshot;
    long unsigned int max_latency;
    struct dentry *d_max_latency;
    struct work_struct fsnotify_work;
    struct irq_work fsnotify_irqwork;
    struct trace_pid_list *filtered_pids;
    struct trace_pid_list *filtered_no_pids;
    arch_spinlock_t max_lock;
    int buffer_disabled;
    int sys_refcount_enter;
    int sys_refcount_exit;
    struct trace_event_file * enter_syscall_files[442];
    struct trace_event_file * exit_syscall_files[442];
    int stop_count;
    int clock_id;
    int nr_topts;
    bool clear_trace;
    int buffer_percent;
    unsigned int n_err_log_entries;
    struct tracer *current_trace;
    unsigned int trace_flags;
    unsigned char trace_flags_index[32];
    unsigned int flags;
    raw_spinlock_t start_lock;
    struct list_head err_log;
    struct dentry *dir;
    struct dentry *options;
    struct dentry *percpu_dir;
    struct dentry *event_dir;
    struct trace_options *topts;
    struct list_head systems;
    struct list_head events;
    struct trace_event_file *trace_marker_file;
    cpumask_var_t tracing_cpumask;
    int ref;
    int trace_ref;
    struct ftrace_ops *ops;
    struct trace_pid_list *function_pids;
    struct trace_pid_list *function_no_pids;
    struct list_head func_probes;
    struct list_head mod_trace;
    struct list_head mod_notrace;
    int function_enabled;
    int time_stamp_abs_ref;
    struct list_head hist_vars;
    struct cond_snapshot *cond_snapshot;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct trace_array {
    struct list_head list;
    char *name;
    struct array_buffer array_buffer;
    struct array_buffer max_buffer;
    bool allocated_snapshot;
    long unsigned int max_latency;
    struct dentry *d_max_latency;
    struct work_struct fsnotify_work;
    struct irq_work fsnotify_irqwork;
    struct trace_pid_list *filtered_pids;
    struct trace_pid_list *filtered_no_pids;
    arch_spinlock_t max_lock;
    int buffer_disabled;
    int sys_refcount_enter;
    int sys_refcount_exit;
    struct trace_event_file * enter_syscall_files[447];
    struct trace_event_file * exit_syscall_files[447];
    int stop_count;
    int clock_id;
    int nr_topts;
    bool clear_trace;
    int buffer_percent;
    unsigned int n_err_log_entries;
    struct tracer *current_trace;
    unsigned int trace_flags;
    unsigned char trace_flags_index[32];
    unsigned int flags;
    raw_spinlock_t start_lock;
    struct list_head err_log;
    struct dentry *dir;
    struct dentry *options;
    struct dentry *percpu_dir;
    struct dentry *event_dir;
    struct trace_options *topts;
    struct list_head systems;
    struct list_head events;
    struct trace_event_file *trace_marker_file;
    cpumask_var_t tracing_cpumask;
    int ref;
    int trace_ref;
    struct ftrace_ops *ops;
    struct trace_pid_list *function_pids;
    struct trace_pid_list *function_no_pids;
    struct list_head func_probes;
    struct list_head mod_trace;
    struct list_head mod_notrace;
    int function_enabled;
    int no_filter_buffering_ref;
    struct list_head hist_vars;
    struct cond_snapshot *cond_snapshot;
    struct trace_func_repeats *last_func_repeats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct trace_array {
    struct list_head list;
    char *name;
    struct array_buffer array_buffer;
    struct array_buffer max_buffer;
    bool allocated_snapshot;
    long unsigned int max_latency;
    struct dentry *d_max_latency;
    struct work_struct fsnotify_work;
    struct irq_work fsnotify_irqwork;
    struct trace_pid_list *filtered_pids;
    struct trace_pid_list *filtered_no_pids;
    arch_spinlock_t max_lock;
    int buffer_disabled;
    int sys_refcount_enter;
    int sys_refcount_exit;
    struct trace_event_file * enter_syscall_files[449];
    struct trace_event_file * exit_syscall_files[449];
    int stop_count;
    int clock_id;
    int nr_topts;
    bool clear_trace;
    int buffer_percent;
    unsigned int n_err_log_entries;
    struct tracer *current_trace;
    unsigned int trace_flags;
    unsigned char trace_flags_index[32];
    unsigned int flags;
    raw_spinlock_t start_lock;
    struct list_head err_log;
    struct dentry *dir;
    struct dentry *options;
    struct dentry *percpu_dir;
    struct dentry *event_dir;
    struct trace_options *topts;
    struct list_head systems;
    struct list_head events;
    struct trace_event_file *trace_marker_file;
    cpumask_var_t tracing_cpumask;
    int ref;
    int trace_ref;
    struct ftrace_ops *ops;
    struct trace_pid_list *function_pids;
    struct trace_pid_list *function_no_pids;
    struct list_head func_probes;
    struct list_head mod_trace;
    struct list_head mod_notrace;
    int function_enabled;
    int no_filter_buffering_ref;
    struct list_head hist_vars;
    struct cond_snapshot *cond_snapshot;
    struct trace_func_repeats *last_func_repeats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct trace_array {
    struct list_head list;
    char *name;
    struct array_buffer array_buffer;
    struct array_buffer max_buffer;
    bool allocated_snapshot;
    long unsigned int max_latency;
    struct dentry *d_max_latency;
    struct work_struct fsnotify_work;
    struct irq_work fsnotify_irqwork;
    struct trace_pid_list *filtered_pids;
    struct trace_pid_list *filtered_no_pids;
    arch_spinlock_t max_lock;
    int buffer_disabled;
    int sys_refcount_enter;
    int sys_refcount_exit;
    struct trace_event_file * enter_syscall_files[451];
    struct trace_event_file * exit_syscall_files[451];
    int stop_count;
    int clock_id;
    int nr_topts;
    bool clear_trace;
    int buffer_percent;
    unsigned int n_err_log_entries;
    struct tracer *current_trace;
    unsigned int trace_flags;
    unsigned char trace_flags_index[32];
    unsigned int flags;
    raw_spinlock_t start_lock;
    struct list_head err_log;
    struct dentry *dir;
    struct dentry *options;
    struct dentry *percpu_dir;
    struct dentry *event_dir;
    struct trace_options *topts;
    struct list_head systems;
    struct list_head events;
    struct trace_event_file *trace_marker_file;
    cpumask_var_t tracing_cpumask;
    int ref;
    int trace_ref;
    struct ftrace_ops *ops;
    struct trace_pid_list *function_pids;
    struct trace_pid_list *function_no_pids;
    struct list_head func_probes;
    struct list_head mod_trace;
    struct list_head mod_notrace;
    int function_enabled;
    int no_filter_buffering_ref;
    struct list_head hist_vars;
    struct cond_snapshot *cond_snapshot;
    struct trace_func_repeats *last_func_repeats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct trace_array {
    struct list_head list;
    char *name;
    struct array_buffer array_buffer;
    struct array_buffer max_buffer;
    bool allocated_snapshot;
    long unsigned int max_latency;
    struct dentry *d_max_latency;
    struct work_struct fsnotify_work;
    struct irq_work fsnotify_irqwork;
    struct trace_pid_list *filtered_pids;
    struct trace_pid_list *filtered_no_pids;
    arch_spinlock_t max_lock;
    int buffer_disabled;
    int sys_refcount_enter;
    int sys_refcount_exit;
    struct trace_event_file * enter_syscall_files[451];
    struct trace_event_file * exit_syscall_files[451];
    int stop_count;
    int clock_id;
    int nr_topts;
    bool clear_trace;
    int buffer_percent;
    unsigned int n_err_log_entries;
    struct tracer *current_trace;
    unsigned int trace_flags;
    unsigned char trace_flags_index[32];
    unsigned int flags;
    raw_spinlock_t start_lock;
    struct list_head err_log;
    struct dentry *dir;
    struct dentry *options;
    struct dentry *percpu_dir;
    struct dentry *event_dir;
    struct trace_options *topts;
    struct list_head systems;
    struct list_head events;
    struct trace_event_file *trace_marker_file;
    cpumask_var_t tracing_cpumask;
    int ref;
    int trace_ref;
    struct ftrace_ops *ops;
    struct trace_pid_list *function_pids;
    struct trace_pid_list *function_no_pids;
    struct list_head func_probes;
    struct list_head mod_trace;
    struct list_head mod_notrace;
    int function_enabled;
    int no_filter_buffering_ref;
    struct list_head hist_vars;
    struct cond_snapshot *cond_snapshot;
    struct trace_func_repeats *last_func_repeats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct trace_array {
    struct list_head list;
    char *name;
    struct array_buffer array_buffer;
    struct array_buffer max_buffer;
    bool allocated_snapshot;
    long unsigned int max_latency;
    struct dentry *d_max_latency;
    struct work_struct fsnotify_work;
    struct irq_work fsnotify_irqwork;
    struct trace_pid_list *filtered_pids;
    struct trace_pid_list *filtered_no_pids;
    arch_spinlock_t max_lock;
    int buffer_disabled;
    int sys_refcount_enter;
    int sys_refcount_exit;
    struct trace_event_file * enter_syscall_files[452];
    struct trace_event_file * exit_syscall_files[452];
    int stop_count;
    int clock_id;
    int nr_topts;
    bool clear_trace;
    int buffer_percent;
    unsigned int n_err_log_entries;
    struct tracer *current_trace;
    unsigned int trace_flags;
    unsigned char trace_flags_index[32];
    unsigned int flags;
    raw_spinlock_t start_lock;
    struct list_head err_log;
    struct dentry *dir;
    struct dentry *options;
    struct dentry *percpu_dir;
    struct dentry *event_dir;
    struct trace_options *topts;
    struct list_head systems;
    struct list_head events;
    struct trace_event_file *trace_marker_file;
    cpumask_var_t tracing_cpumask;
    cpumask_var_t pipe_cpumask;
    int ref;
    int trace_ref;
    struct ftrace_ops *ops;
    struct trace_pid_list *function_pids;
    struct trace_pid_list *function_no_pids;
    struct list_head func_probes;
    struct list_head mod_trace;
    struct list_head mod_notrace;
    int function_enabled;
    int no_filter_buffering_ref;
    struct list_head hist_vars;
    struct cond_snapshot *cond_snapshot;
    struct trace_func_repeats *last_func_repeats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct trace_array {
    struct list_head list;
    char *name;
    struct array_buffer array_buffer;
    struct array_buffer max_buffer;
    bool allocated_snapshot;
    long unsigned int max_latency;
    struct dentry *d_max_latency;
    struct work_struct fsnotify_work;
    struct irq_work fsnotify_irqwork;
    struct trace_pid_list *filtered_pids;
    struct trace_pid_list *filtered_no_pids;
    arch_spinlock_t max_lock;
    int buffer_disabled;
    int sys_refcount_enter;
    int sys_refcount_exit;
    struct trace_event_file * enter_syscall_files[462];
    struct trace_event_file * exit_syscall_files[462];
    int stop_count;
    int clock_id;
    int nr_topts;
    bool clear_trace;
    int buffer_percent;
    unsigned int n_err_log_entries;
    struct tracer *current_trace;
    unsigned int trace_flags;
    unsigned char trace_flags_index[32];
    unsigned int flags;
    raw_spinlock_t start_lock;
    const char *system_names;
    struct list_head err_log;
    struct dentry *dir;
    struct dentry *options;
    struct dentry *percpu_dir;
    struct eventfs_inode *event_dir;
    struct trace_options *topts;
    struct list_head systems;
    struct list_head events;
    struct trace_event_file *trace_marker_file;
    cpumask_var_t tracing_cpumask;
    cpumask_var_t pipe_cpumask;
    int ref;
    int trace_ref;
    struct ftrace_ops *ops;
    struct trace_pid_list *function_pids;
    struct trace_pid_list *function_no_pids;
    struct list_head func_probes;
    struct list_head mod_trace;
    struct list_head mod_notrace;
    int function_enabled;
    int no_filter_buffering_ref;
    struct list_head hist_vars;
    struct cond_snapshot *cond_snapshot;
    struct trace_func_repeats *last_func_repeats;
    bool ring_buffer_expanded;
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
struct trace_array {
    struct list_head list;
    char *name;
    struct trace_buffer trace_buffer;
    struct trace_buffer max_buffer;
    bool allocated_snapshot;
    long unsigned int max_latency;
    struct trace_pid_list *filtered_pids;
    arch_spinlock_t max_lock;
    int buffer_disabled;
    int sys_refcount_enter;
    int sys_refcount_exit;
    struct trace_event_file * enter_syscall_files[436];
    struct trace_event_file * exit_syscall_files[436];
    int stop_count;
    int clock_id;
    int nr_topts;
    bool clear_trace;
    int buffer_percent;
    unsigned int n_err_log_entries;
    struct tracer *current_trace;
    unsigned int trace_flags;
    unsigned char trace_flags_index[32];
    unsigned int flags;
    raw_spinlock_t start_lock;
    struct list_head err_log;
    struct dentry *dir;
    struct dentry *options;
    struct dentry *percpu_dir;
    struct dentry *event_dir;
    struct trace_options *topts;
    struct list_head systems;
    struct list_head events;
    struct trace_event_file *trace_marker_file;
    cpumask_var_t tracing_cpumask;
    int ref;
    struct ftrace_ops *ops;
    struct trace_pid_list *function_pids;
    struct list_head func_probes;
    struct list_head mod_trace;
    struct list_head mod_notrace;
    int function_enabled;
    int time_stamp_abs_ref;
    struct list_head hist_vars;
    struct cond_snapshot *cond_snapshot;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct trace_array {
    struct list_head list;
    char *name;
    struct trace_buffer trace_buffer;
    struct trace_buffer max_buffer;
    bool allocated_snapshot;
    long unsigned int max_latency;
    struct trace_pid_list *filtered_pids;
    arch_spinlock_t max_lock;
    int buffer_disabled;
    int sys_refcount_enter;
    int sys_refcount_exit;
    struct trace_event_file * enter_syscall_files[436];
    struct trace_event_file * exit_syscall_files[436];
    int stop_count;
    int clock_id;
    int nr_topts;
    bool clear_trace;
    int buffer_percent;
    unsigned int n_err_log_entries;
    struct tracer *current_trace;
    unsigned int trace_flags;
    unsigned char trace_flags_index[32];
    unsigned int flags;
    raw_spinlock_t start_lock;
    struct list_head err_log;
    struct dentry *dir;
    struct dentry *options;
    struct dentry *percpu_dir;
    struct dentry *event_dir;
    struct trace_options *topts;
    struct list_head systems;
    struct list_head events;
    struct trace_event_file *trace_marker_file;
    cpumask_var_t tracing_cpumask;
    int ref;
    struct ftrace_ops *ops;
    struct trace_pid_list *function_pids;
    struct list_head func_probes;
    struct list_head mod_trace;
    struct list_head mod_notrace;
    int function_enabled;
    int time_stamp_abs_ref;
    struct list_head hist_vars;
    struct cond_snapshot *cond_snapshot;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct trace_array {
    struct list_head list;
    char *name;
    struct trace_buffer trace_buffer;
    struct trace_buffer max_buffer;
    bool allocated_snapshot;
    long unsigned int max_latency;
    struct trace_pid_list *filtered_pids;
    arch_spinlock_t max_lock;
    int buffer_disabled;
    int sys_refcount_enter;
    int sys_refcount_exit;
    struct trace_event_file * enter_syscall_files[436];
    struct trace_event_file * exit_syscall_files[436];
    int stop_count;
    int clock_id;
    int nr_topts;
    bool clear_trace;
    int buffer_percent;
    unsigned int n_err_log_entries;
    struct tracer *current_trace;
    unsigned int trace_flags;
    unsigned char trace_flags_index[32];
    unsigned int flags;
    raw_spinlock_t start_lock;
    struct list_head err_log;
    struct dentry *dir;
    struct dentry *options;
    struct dentry *percpu_dir;
    struct dentry *event_dir;
    struct trace_options *topts;
    struct list_head systems;
    struct list_head events;
    struct trace_event_file *trace_marker_file;
    cpumask_var_t tracing_cpumask;
    int ref;
    struct ftrace_ops *ops;
    struct trace_pid_list *function_pids;
    struct list_head func_probes;
    struct list_head mod_trace;
    struct list_head mod_notrace;
    int function_enabled;
    int time_stamp_abs_ref;
    struct list_head hist_vars;
    struct cond_snapshot *cond_snapshot;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct trace_array {
    struct list_head list;
    char *name;
    struct trace_buffer trace_buffer;
    struct trace_buffer max_buffer;
    bool allocated_snapshot;
    long unsigned int max_latency;
    struct trace_pid_list *filtered_pids;
    arch_spinlock_t max_lock;
    int buffer_disabled;
    int sys_refcount_enter;
    int sys_refcount_exit;
    struct trace_event_file * enter_syscall_files[436];
    struct trace_event_file * exit_syscall_files[436];
    int stop_count;
    int clock_id;
    int nr_topts;
    bool clear_trace;
    int buffer_percent;
    unsigned int n_err_log_entries;
    struct tracer *current_trace;
    unsigned int trace_flags;
    unsigned char trace_flags_index[32];
    unsigned int flags;
    raw_spinlock_t start_lock;
    struct list_head err_log;
    struct dentry *dir;
    struct dentry *options;
    struct dentry *percpu_dir;
    struct dentry *event_dir;
    struct trace_options *topts;
    struct list_head systems;
    struct list_head events;
    struct trace_event_file *trace_marker_file;
    cpumask_var_t tracing_cpumask;
    int ref;
    struct ftrace_ops *ops;
    struct trace_pid_list *function_pids;
    struct list_head func_probes;
    struct list_head mod_trace;
    struct list_head mod_notrace;
    int function_enabled;
    int time_stamp_abs_ref;
    struct list_head hist_vars;
    struct cond_snapshot *cond_snapshot;
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
struct trace_array {
    struct list_head list;
    char *name;
    struct trace_buffer trace_buffer;
    struct trace_buffer max_buffer;
    bool allocated_snapshot;
    long unsigned int max_latency;
    struct trace_pid_list *filtered_pids;
    arch_spinlock_t max_lock;
    int buffer_disabled;
    int sys_refcount_enter;
    int sys_refcount_exit;
    struct trace_event_file * enter_syscall_files[436];
    struct trace_event_file * exit_syscall_files[436];
    int stop_count;
    int clock_id;
    int nr_topts;
    bool clear_trace;
    int buffer_percent;
    unsigned int n_err_log_entries;
    struct tracer *current_trace;
    unsigned int trace_flags;
    unsigned char trace_flags_index[32];
    unsigned int flags;
    raw_spinlock_t start_lock;
    struct list_head err_log;
    struct dentry *dir;
    struct dentry *options;
    struct dentry *percpu_dir;
    struct dentry *event_dir;
    struct trace_options *topts;
    struct list_head systems;
    struct list_head events;
    struct trace_event_file *trace_marker_file;
    cpumask_var_t tracing_cpumask;
    int ref;
    struct ftrace_ops *ops;
    struct trace_pid_list *function_pids;
    struct list_head func_probes;
    struct list_head mod_trace;
    struct list_head mod_notrace;
    int function_enabled;
    int time_stamp_abs_ref;
    struct list_head hist_vars;
    struct cond_snapshot *cond_snapshot;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct trace_array {
    struct list_head list;
    char *name;
    struct trace_buffer trace_buffer;
    struct trace_buffer max_buffer;
    bool allocated_snapshot;
    long unsigned int max_latency;
    struct trace_pid_list *filtered_pids;
    arch_spinlock_t max_lock;
    int buffer_disabled;
    int sys_refcount_enter;
    int sys_refcount_exit;
    struct trace_event_file * enter_syscall_files[436];
    struct trace_event_file * exit_syscall_files[436];
    int stop_count;
    int clock_id;
    int nr_topts;
    bool clear_trace;
    int buffer_percent;
    unsigned int n_err_log_entries;
    struct tracer *current_trace;
    unsigned int trace_flags;
    unsigned char trace_flags_index[32];
    unsigned int flags;
    raw_spinlock_t start_lock;
    struct list_head err_log;
    struct dentry *dir;
    struct dentry *options;
    struct dentry *percpu_dir;
    struct dentry *event_dir;
    struct trace_options *topts;
    struct list_head systems;
    struct list_head events;
    struct trace_event_file *trace_marker_file;
    cpumask_var_t tracing_cpumask;
    int ref;
    struct ftrace_ops *ops;
    struct trace_pid_list *function_pids;
    struct list_head func_probes;
    struct list_head mod_trace;
    struct list_head mod_notrace;
    int function_enabled;
    int time_stamp_abs_ref;
    struct list_head hist_vars;
    struct cond_snapshot *cond_snapshot;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct trace_array {
    struct list_head list;
    char *name;
    struct trace_buffer trace_buffer;
    struct trace_buffer max_buffer;
    bool allocated_snapshot;
    long unsigned int max_latency;
    struct trace_pid_list *filtered_pids;
    arch_spinlock_t max_lock;
    int buffer_disabled;
    int sys_refcount_enter;
    int sys_refcount_exit;
    struct trace_event_file * enter_syscall_files[436];
    struct trace_event_file * exit_syscall_files[436];
    int stop_count;
    int clock_id;
    int nr_topts;
    bool clear_trace;
    int buffer_percent;
    unsigned int n_err_log_entries;
    struct tracer *current_trace;
    unsigned int trace_flags;
    unsigned char trace_flags_index[32];
    unsigned int flags;
    raw_spinlock_t start_lock;
    struct list_head err_log;
    struct dentry *dir;
    struct dentry *options;
    struct dentry *percpu_dir;
    struct dentry *event_dir;
    struct trace_options *topts;
    struct list_head systems;
    struct list_head events;
    struct trace_event_file *trace_marker_file;
    cpumask_var_t tracing_cpumask;
    int ref;
    struct ftrace_ops *ops;
    struct trace_pid_list *function_pids;
    struct list_head func_probes;
    struct list_head mod_trace;
    struct list_head mod_notrace;
    int function_enabled;
    int time_stamp_abs_ref;
    struct list_head hist_vars;
    struct cond_snapshot *cond_snapshot;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct trace_array {
    struct list_head list;
    char *name;
    struct trace_buffer trace_buffer;
    struct trace_buffer max_buffer;
    bool allocated_snapshot;
    long unsigned int max_latency;
    struct trace_pid_list *filtered_pids;
    arch_spinlock_t max_lock;
    int buffer_disabled;
    int sys_refcount_enter;
    int sys_refcount_exit;
    struct trace_event_file * enter_syscall_files[436];
    struct trace_event_file * exit_syscall_files[436];
    int stop_count;
    int clock_id;
    int nr_topts;
    bool clear_trace;
    int buffer_percent;
    unsigned int n_err_log_entries;
    struct tracer *current_trace;
    unsigned int trace_flags;
    unsigned char trace_flags_index[32];
    unsigned int flags;
    raw_spinlock_t start_lock;
    struct list_head err_log;
    struct dentry *dir;
    struct dentry *options;
    struct dentry *percpu_dir;
    struct dentry *event_dir;
    struct trace_options *topts;
    struct list_head systems;
    struct list_head events;
    struct trace_event_file *trace_marker_file;
    cpumask_var_t tracing_cpumask;
    int ref;
    struct ftrace_ops *ops;
    struct trace_pid_list *function_pids;
    struct list_head func_probes;
    struct list_head mod_trace;
    struct list_head mod_notrace;
    int function_enabled;
    int time_stamp_abs_ref;
    struct list_head hist_vars;
    struct cond_snapshot *cond_snapshot;
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
<code>struct trace_pid_list *function_pids</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct trace_event_file * enter_syscall_files[546]</code> ➡️ <code>struct trace_event_file * enter_syscall_files[548]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct trace_event_file * exit_syscall_files[546]</code> ➡️ <code>struct trace_event_file * exit_syscall_files[548]</code>
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
<code>struct list_head func_probes</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head mod_trace</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head mod_notrace</code>
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
<code>bool clear_trace</code>
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
<code>struct trace_event_file *trace_marker_file</code>
</li>
<li>
<b>Field added. </b>
<code>int time_stamp_abs_ref</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head hist_vars</code>
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
<code>int buffer_percent</code>
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
<code>unsigned int n_err_log_entries</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head err_log</code>
</li>
<li>
<b>Field added. </b>
<code>struct cond_snapshot *cond_snapshot</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct trace_event_file * enter_syscall_files[548]</code> ➡️ <code>struct trace_event_file * enter_syscall_files[436]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct trace_event_file * exit_syscall_files[548]</code> ➡️ <code>struct trace_event_file * exit_syscall_files[436]</code>
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
<code>struct array_buffer array_buffer</code>
</li>
<li>
<b>Field added. </b>
<code>struct dentry *d_max_latency</code>
</li>
<li>
<b>Field added. </b>
<code>struct work_struct fsnotify_work</code>
</li>
<li>
<b>Field added. </b>
<code>struct irq_work fsnotify_irqwork</code>
</li>
<li>
<b>Field added. </b>
<code>struct trace_pid_list *filtered_no_pids</code>
</li>
<li>
<b>Field added. </b>
<code>int trace_ref</code>
</li>
<li>
<b>Field added. </b>
<code>struct trace_pid_list *function_no_pids</code>
</li>
<li>
<b>Field removed. </b>
<code>struct trace_buffer trace_buffer</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct trace_buffer max_buffer</code> ➡️ <code>struct array_buffer max_buffer</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct trace_event_file * enter_syscall_files[436]</code> ➡️ <code>struct trace_event_file * enter_syscall_files[440]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct trace_event_file * exit_syscall_files[436]</code> ➡️ <code>struct trace_event_file * exit_syscall_files[440]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct trace_event_file * enter_syscall_files[440]</code> ➡️ <code>struct trace_event_file * enter_syscall_files[442]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct trace_event_file * exit_syscall_files[440]</code> ➡️ <code>struct trace_event_file * exit_syscall_files[442]</code>
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
<code>int no_filter_buffering_ref</code>
</li>
<li>
<b>Field added. </b>
<code>struct trace_func_repeats *last_func_repeats</code>
</li>
<li>
<b>Field removed. </b>
<code>int time_stamp_abs_ref</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct trace_event_file * enter_syscall_files[442]</code> ➡️ <code>struct trace_event_file * enter_syscall_files[447]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct trace_event_file * exit_syscall_files[442]</code> ➡️ <code>struct trace_event_file * exit_syscall_files[447]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct trace_event_file * enter_syscall_files[447]</code> ➡️ <code>struct trace_event_file * enter_syscall_files[449]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct trace_event_file * exit_syscall_files[447]</code> ➡️ <code>struct trace_event_file * exit_syscall_files[449]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct trace_event_file * enter_syscall_files[449]</code> ➡️ <code>struct trace_event_file * enter_syscall_files[451]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct trace_event_file * exit_syscall_files[449]</code> ➡️ <code>struct trace_event_file * exit_syscall_files[451]</code>
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
<code>cpumask_var_t pipe_cpumask</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct trace_event_file * enter_syscall_files[451]</code> ➡️ <code>struct trace_event_file * enter_syscall_files[452]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct trace_event_file * exit_syscall_files[451]</code> ➡️ <code>struct trace_event_file * exit_syscall_files[452]</code>
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
<code>const char *system_names</code>
</li>
<li>
<b>Field added. </b>
<code>bool ring_buffer_expanded</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct trace_event_file * enter_syscall_files[452]</code> ➡️ <code>struct trace_event_file * enter_syscall_files[462]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct trace_event_file * exit_syscall_files[452]</code> ➡️ <code>struct trace_event_file * exit_syscall_files[462]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct dentry *event_dir</code> ➡️ <code>struct eventfs_inode *event_dir</code>
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
