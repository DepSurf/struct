# Struct: <code>irq_desc</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct irq_desc {
    struct irq_common_data irq_common_data;
    struct irq_data irq_data;
    unsigned int *kstat_irqs;
    irq_flow_handler_t handle_irq;
    struct irqaction *action;
    unsigned int status_use_accessors;
    unsigned int core_internal_state__do_not_mess_with_it;
    unsigned int depth;
    unsigned int wake_depth;
    unsigned int irq_count;
    long unsigned int last_unhandled;
    unsigned int irqs_unhandled;
    atomic_t threads_handled;
    int threads_handled_last;
    raw_spinlock_t lock;
    struct cpumask *percpu_enabled;
    const struct cpumask *affinity_hint;
    struct irq_affinity_notify *affinity_notify;
    cpumask_var_t pending_mask;
    long unsigned int threads_oneshot;
    atomic_t threads_active;
    wait_queue_head_t wait_for_threads;
    unsigned int nr_actions;
    unsigned int no_suspend_depth;
    unsigned int cond_suspend_depth;
    unsigned int force_resume_depth;
    struct proc_dir_entry *dir;
    int parent_irq;
    struct module *owner;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct irq_desc {
    struct irq_common_data irq_common_data;
    struct irq_data irq_data;
    unsigned int *kstat_irqs;
    irq_flow_handler_t handle_irq;
    struct irqaction *action;
    unsigned int status_use_accessors;
    unsigned int core_internal_state__do_not_mess_with_it;
    unsigned int depth;
    unsigned int wake_depth;
    unsigned int irq_count;
    long unsigned int last_unhandled;
    unsigned int irqs_unhandled;
    atomic_t threads_handled;
    int threads_handled_last;
    raw_spinlock_t lock;
    struct cpumask *percpu_enabled;
    const struct cpumask *percpu_affinity;
    const struct cpumask *affinity_hint;
    struct irq_affinity_notify *affinity_notify;
    cpumask_var_t pending_mask;
    long unsigned int threads_oneshot;
    atomic_t threads_active;
    wait_queue_head_t wait_for_threads;
    unsigned int nr_actions;
    unsigned int no_suspend_depth;
    unsigned int cond_suspend_depth;
    unsigned int force_resume_depth;
    struct proc_dir_entry *dir;
    struct callback_head rcu;
    int parent_irq;
    struct module *owner;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct irq_desc {
    struct irq_common_data irq_common_data;
    struct irq_data irq_data;
    unsigned int *kstat_irqs;
    irq_flow_handler_t handle_irq;
    struct irqaction *action;
    unsigned int status_use_accessors;
    unsigned int core_internal_state__do_not_mess_with_it;
    unsigned int depth;
    unsigned int wake_depth;
    unsigned int irq_count;
    long unsigned int last_unhandled;
    unsigned int irqs_unhandled;
    atomic_t threads_handled;
    int threads_handled_last;
    raw_spinlock_t lock;
    struct cpumask *percpu_enabled;
    const struct cpumask *percpu_affinity;
    const struct cpumask *affinity_hint;
    struct irq_affinity_notify *affinity_notify;
    cpumask_var_t pending_mask;
    long unsigned int threads_oneshot;
    atomic_t threads_active;
    wait_queue_head_t wait_for_threads;
    unsigned int nr_actions;
    unsigned int no_suspend_depth;
    unsigned int cond_suspend_depth;
    unsigned int force_resume_depth;
    struct proc_dir_entry *dir;
    struct callback_head rcu;
    struct kobject kobj;
    int parent_irq;
    struct module *owner;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct irq_desc {
    struct irq_common_data irq_common_data;
    struct irq_data irq_data;
    unsigned int *kstat_irqs;
    irq_flow_handler_t handle_irq;
    struct irqaction *action;
    unsigned int status_use_accessors;
    unsigned int core_internal_state__do_not_mess_with_it;
    unsigned int depth;
    unsigned int wake_depth;
    unsigned int irq_count;
    long unsigned int last_unhandled;
    unsigned int irqs_unhandled;
    atomic_t threads_handled;
    int threads_handled_last;
    raw_spinlock_t lock;
    struct cpumask *percpu_enabled;
    const struct cpumask *percpu_affinity;
    const struct cpumask *affinity_hint;
    struct irq_affinity_notify *affinity_notify;
    cpumask_var_t pending_mask;
    long unsigned int threads_oneshot;
    atomic_t threads_active;
    wait_queue_head_t wait_for_threads;
    unsigned int nr_actions;
    unsigned int no_suspend_depth;
    unsigned int cond_suspend_depth;
    unsigned int force_resume_depth;
    struct proc_dir_entry *dir;
    struct callback_head rcu;
    struct kobject kobj;
    struct mutex request_mutex;
    int parent_irq;
    struct module *owner;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct irq_desc {
    struct irq_common_data irq_common_data;
    struct irq_data irq_data;
    unsigned int *kstat_irqs;
    irq_flow_handler_t handle_irq;
    struct irqaction *action;
    unsigned int status_use_accessors;
    unsigned int core_internal_state__do_not_mess_with_it;
    unsigned int depth;
    unsigned int wake_depth;
    unsigned int irq_count;
    long unsigned int last_unhandled;
    unsigned int irqs_unhandled;
    atomic_t threads_handled;
    int threads_handled_last;
    raw_spinlock_t lock;
    struct cpumask *percpu_enabled;
    const struct cpumask *percpu_affinity;
    const struct cpumask *affinity_hint;
    struct irq_affinity_notify *affinity_notify;
    cpumask_var_t pending_mask;
    long unsigned int threads_oneshot;
    atomic_t threads_active;
    wait_queue_head_t wait_for_threads;
    unsigned int nr_actions;
    unsigned int no_suspend_depth;
    unsigned int cond_suspend_depth;
    unsigned int force_resume_depth;
    struct proc_dir_entry *dir;
    struct callback_head rcu;
    struct kobject kobj;
    struct mutex request_mutex;
    int parent_irq;
    struct module *owner;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct irq_desc {
    struct irq_common_data irq_common_data;
    struct irq_data irq_data;
    unsigned int *kstat_irqs;
    irq_flow_handler_t handle_irq;
    struct irqaction *action;
    unsigned int status_use_accessors;
    unsigned int core_internal_state__do_not_mess_with_it;
    unsigned int depth;
    unsigned int wake_depth;
    unsigned int irq_count;
    long unsigned int last_unhandled;
    unsigned int irqs_unhandled;
    atomic_t threads_handled;
    int threads_handled_last;
    raw_spinlock_t lock;
    struct cpumask *percpu_enabled;
    const struct cpumask *percpu_affinity;
    const struct cpumask *affinity_hint;
    struct irq_affinity_notify *affinity_notify;
    cpumask_var_t pending_mask;
    long unsigned int threads_oneshot;
    atomic_t threads_active;
    wait_queue_head_t wait_for_threads;
    unsigned int nr_actions;
    unsigned int no_suspend_depth;
    unsigned int cond_suspend_depth;
    unsigned int force_resume_depth;
    struct proc_dir_entry *dir;
    struct callback_head rcu;
    struct kobject kobj;
    struct mutex request_mutex;
    int parent_irq;
    struct module *owner;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct irq_desc {
    struct irq_common_data irq_common_data;
    struct irq_data irq_data;
    unsigned int *kstat_irqs;
    irq_flow_handler_t handle_irq;
    struct irqaction *action;
    unsigned int status_use_accessors;
    unsigned int core_internal_state__do_not_mess_with_it;
    unsigned int depth;
    unsigned int wake_depth;
    unsigned int irq_count;
    long unsigned int last_unhandled;
    unsigned int irqs_unhandled;
    atomic_t threads_handled;
    int threads_handled_last;
    raw_spinlock_t lock;
    struct cpumask *percpu_enabled;
    const struct cpumask *percpu_affinity;
    const struct cpumask *affinity_hint;
    struct irq_affinity_notify *affinity_notify;
    cpumask_var_t pending_mask;
    long unsigned int threads_oneshot;
    atomic_t threads_active;
    wait_queue_head_t wait_for_threads;
    unsigned int nr_actions;
    unsigned int no_suspend_depth;
    unsigned int cond_suspend_depth;
    unsigned int force_resume_depth;
    struct proc_dir_entry *dir;
    struct callback_head rcu;
    struct kobject kobj;
    struct mutex request_mutex;
    int parent_irq;
    struct module *owner;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct irq_desc {
    struct irq_common_data irq_common_data;
    struct irq_data irq_data;
    unsigned int *kstat_irqs;
    irq_flow_handler_t handle_irq;
    struct irqaction *action;
    unsigned int status_use_accessors;
    unsigned int core_internal_state__do_not_mess_with_it;
    unsigned int depth;
    unsigned int wake_depth;
    unsigned int tot_count;
    unsigned int irq_count;
    long unsigned int last_unhandled;
    unsigned int irqs_unhandled;
    atomic_t threads_handled;
    int threads_handled_last;
    raw_spinlock_t lock;
    struct cpumask *percpu_enabled;
    const struct cpumask *percpu_affinity;
    const struct cpumask *affinity_hint;
    struct irq_affinity_notify *affinity_notify;
    cpumask_var_t pending_mask;
    long unsigned int threads_oneshot;
    atomic_t threads_active;
    wait_queue_head_t wait_for_threads;
    unsigned int nr_actions;
    unsigned int no_suspend_depth;
    unsigned int cond_suspend_depth;
    unsigned int force_resume_depth;
    struct proc_dir_entry *dir;
    struct callback_head rcu;
    struct kobject kobj;
    struct mutex request_mutex;
    int parent_irq;
    struct module *owner;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct irq_desc {
    struct irq_common_data irq_common_data;
    struct irq_data irq_data;
    unsigned int *kstat_irqs;
    irq_flow_handler_t handle_irq;
    struct irqaction *action;
    unsigned int status_use_accessors;
    unsigned int core_internal_state__do_not_mess_with_it;
    unsigned int depth;
    unsigned int wake_depth;
    unsigned int tot_count;
    unsigned int irq_count;
    long unsigned int last_unhandled;
    unsigned int irqs_unhandled;
    atomic_t threads_handled;
    int threads_handled_last;
    raw_spinlock_t lock;
    struct cpumask *percpu_enabled;
    const struct cpumask *percpu_affinity;
    const struct cpumask *affinity_hint;
    struct irq_affinity_notify *affinity_notify;
    cpumask_var_t pending_mask;
    long unsigned int threads_oneshot;
    atomic_t threads_active;
    wait_queue_head_t wait_for_threads;
    unsigned int nr_actions;
    unsigned int no_suspend_depth;
    unsigned int cond_suspend_depth;
    unsigned int force_resume_depth;
    struct proc_dir_entry *dir;
    struct callback_head rcu;
    struct kobject kobj;
    struct mutex request_mutex;
    int parent_irq;
    struct module *owner;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct irq_desc {
    struct irq_common_data irq_common_data;
    struct irq_data irq_data;
    unsigned int *kstat_irqs;
    irq_flow_handler_t handle_irq;
    struct irqaction *action;
    unsigned int status_use_accessors;
    unsigned int core_internal_state__do_not_mess_with_it;
    unsigned int depth;
    unsigned int wake_depth;
    unsigned int tot_count;
    unsigned int irq_count;
    long unsigned int last_unhandled;
    unsigned int irqs_unhandled;
    atomic_t threads_handled;
    int threads_handled_last;
    raw_spinlock_t lock;
    struct cpumask *percpu_enabled;
    const struct cpumask *percpu_affinity;
    const struct cpumask *affinity_hint;
    struct irq_affinity_notify *affinity_notify;
    cpumask_var_t pending_mask;
    long unsigned int threads_oneshot;
    atomic_t threads_active;
    wait_queue_head_t wait_for_threads;
    unsigned int nr_actions;
    unsigned int no_suspend_depth;
    unsigned int cond_suspend_depth;
    unsigned int force_resume_depth;
    struct proc_dir_entry *dir;
    struct callback_head rcu;
    struct kobject kobj;
    struct mutex request_mutex;
    int parent_irq;
    struct module *owner;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct irq_desc {
    struct irq_common_data irq_common_data;
    struct irq_data irq_data;
    unsigned int *kstat_irqs;
    irq_flow_handler_t handle_irq;
    struct irqaction *action;
    unsigned int status_use_accessors;
    unsigned int core_internal_state__do_not_mess_with_it;
    unsigned int depth;
    unsigned int wake_depth;
    unsigned int tot_count;
    unsigned int irq_count;
    long unsigned int last_unhandled;
    unsigned int irqs_unhandled;
    atomic_t threads_handled;
    int threads_handled_last;
    raw_spinlock_t lock;
    struct cpumask *percpu_enabled;
    const struct cpumask *percpu_affinity;
    const struct cpumask *affinity_hint;
    struct irq_affinity_notify *affinity_notify;
    cpumask_var_t pending_mask;
    long unsigned int threads_oneshot;
    atomic_t threads_active;
    wait_queue_head_t wait_for_threads;
    unsigned int nr_actions;
    unsigned int no_suspend_depth;
    unsigned int cond_suspend_depth;
    unsigned int force_resume_depth;
    struct proc_dir_entry *dir;
    struct callback_head rcu;
    struct kobject kobj;
    struct mutex request_mutex;
    int parent_irq;
    struct module *owner;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct irq_desc {
    struct irq_common_data irq_common_data;
    struct irq_data irq_data;
    unsigned int *kstat_irqs;
    irq_flow_handler_t handle_irq;
    struct irqaction *action;
    unsigned int status_use_accessors;
    unsigned int core_internal_state__do_not_mess_with_it;
    unsigned int depth;
    unsigned int wake_depth;
    unsigned int tot_count;
    unsigned int irq_count;
    long unsigned int last_unhandled;
    unsigned int irqs_unhandled;
    atomic_t threads_handled;
    int threads_handled_last;
    raw_spinlock_t lock;
    struct cpumask *percpu_enabled;
    const struct cpumask *percpu_affinity;
    const struct cpumask *affinity_hint;
    struct irq_affinity_notify *affinity_notify;
    cpumask_var_t pending_mask;
    long unsigned int threads_oneshot;
    atomic_t threads_active;
    wait_queue_head_t wait_for_threads;
    unsigned int nr_actions;
    unsigned int no_suspend_depth;
    unsigned int cond_suspend_depth;
    unsigned int force_resume_depth;
    struct proc_dir_entry *dir;
    struct callback_head rcu;
    struct kobject kobj;
    struct mutex request_mutex;
    int parent_irq;
    struct module *owner;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct irq_desc {
    struct irq_common_data irq_common_data;
    struct irq_data irq_data;
    unsigned int *kstat_irqs;
    irq_flow_handler_t handle_irq;
    struct irqaction *action;
    unsigned int status_use_accessors;
    unsigned int core_internal_state__do_not_mess_with_it;
    unsigned int depth;
    unsigned int wake_depth;
    unsigned int tot_count;
    unsigned int irq_count;
    long unsigned int last_unhandled;
    unsigned int irqs_unhandled;
    atomic_t threads_handled;
    int threads_handled_last;
    raw_spinlock_t lock;
    struct cpumask *percpu_enabled;
    const struct cpumask *percpu_affinity;
    const struct cpumask *affinity_hint;
    struct irq_affinity_notify *affinity_notify;
    cpumask_var_t pending_mask;
    long unsigned int threads_oneshot;
    atomic_t threads_active;
    wait_queue_head_t wait_for_threads;
    unsigned int nr_actions;
    unsigned int no_suspend_depth;
    unsigned int cond_suspend_depth;
    unsigned int force_resume_depth;
    struct proc_dir_entry *dir;
    struct callback_head rcu;
    struct kobject kobj;
    struct mutex request_mutex;
    int parent_irq;
    struct module *owner;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct irq_desc {
    struct irq_common_data irq_common_data;
    struct irq_data irq_data;
    unsigned int *kstat_irqs;
    irq_flow_handler_t handle_irq;
    struct irqaction *action;
    unsigned int status_use_accessors;
    unsigned int core_internal_state__do_not_mess_with_it;
    unsigned int depth;
    unsigned int wake_depth;
    unsigned int tot_count;
    unsigned int irq_count;
    long unsigned int last_unhandled;
    unsigned int irqs_unhandled;
    atomic_t threads_handled;
    int threads_handled_last;
    raw_spinlock_t lock;
    struct cpumask *percpu_enabled;
    const struct cpumask *percpu_affinity;
    const struct cpumask *affinity_hint;
    struct irq_affinity_notify *affinity_notify;
    cpumask_var_t pending_mask;
    long unsigned int threads_oneshot;
    atomic_t threads_active;
    wait_queue_head_t wait_for_threads;
    unsigned int nr_actions;
    unsigned int no_suspend_depth;
    unsigned int cond_suspend_depth;
    unsigned int force_resume_depth;
    struct proc_dir_entry *dir;
    struct callback_head rcu;
    struct kobject kobj;
    struct mutex request_mutex;
    int parent_irq;
    struct module *owner;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct irq_desc {
    struct irq_common_data irq_common_data;
    struct irq_data irq_data;
    unsigned int *kstat_irqs;
    irq_flow_handler_t handle_irq;
    struct irqaction *action;
    unsigned int status_use_accessors;
    unsigned int core_internal_state__do_not_mess_with_it;
    unsigned int depth;
    unsigned int wake_depth;
    unsigned int tot_count;
    unsigned int irq_count;
    long unsigned int last_unhandled;
    unsigned int irqs_unhandled;
    atomic_t threads_handled;
    int threads_handled_last;
    raw_spinlock_t lock;
    struct cpumask *percpu_enabled;
    const struct cpumask *percpu_affinity;
    const struct cpumask *affinity_hint;
    struct irq_affinity_notify *affinity_notify;
    cpumask_var_t pending_mask;
    long unsigned int threads_oneshot;
    atomic_t threads_active;
    wait_queue_head_t wait_for_threads;
    unsigned int nr_actions;
    unsigned int no_suspend_depth;
    unsigned int cond_suspend_depth;
    unsigned int force_resume_depth;
    struct proc_dir_entry *dir;
    struct callback_head rcu;
    struct kobject kobj;
    struct mutex request_mutex;
    int parent_irq;
    struct module *owner;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct irq_desc {
    struct irq_common_data irq_common_data;
    struct irq_data irq_data;
    unsigned int *kstat_irqs;
    irq_flow_handler_t handle_irq;
    struct irqaction *action;
    unsigned int status_use_accessors;
    unsigned int core_internal_state__do_not_mess_with_it;
    unsigned int depth;
    unsigned int wake_depth;
    unsigned int tot_count;
    unsigned int irq_count;
    long unsigned int last_unhandled;
    unsigned int irqs_unhandled;
    atomic_t threads_handled;
    int threads_handled_last;
    raw_spinlock_t lock;
    struct cpumask *percpu_enabled;
    const struct cpumask *percpu_affinity;
    const struct cpumask *affinity_hint;
    struct irq_affinity_notify *affinity_notify;
    cpumask_var_t pending_mask;
    long unsigned int threads_oneshot;
    atomic_t threads_active;
    wait_queue_head_t wait_for_threads;
    unsigned int nr_actions;
    unsigned int no_suspend_depth;
    unsigned int cond_suspend_depth;
    unsigned int force_resume_depth;
    struct proc_dir_entry *dir;
    struct callback_head rcu;
    struct kobject kobj;
    struct mutex request_mutex;
    int parent_irq;
    struct module *owner;
    const char *name;
    struct hlist_node resend_node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct irq_desc {
    struct irq_common_data irq_common_data;
    struct irq_data irq_data;
    unsigned int *kstat_irqs;
    irq_flow_handler_t handle_irq;
    struct irqaction *action;
    unsigned int status_use_accessors;
    unsigned int core_internal_state__do_not_mess_with_it;
    unsigned int depth;
    unsigned int wake_depth;
    unsigned int tot_count;
    unsigned int irq_count;
    long unsigned int last_unhandled;
    unsigned int irqs_unhandled;
    atomic_t threads_handled;
    int threads_handled_last;
    raw_spinlock_t lock;
    struct cpumask *percpu_enabled;
    const struct cpumask *percpu_affinity;
    const struct cpumask *affinity_hint;
    struct irq_affinity_notify *affinity_notify;
    cpumask_var_t pending_mask;
    long unsigned int threads_oneshot;
    atomic_t threads_active;
    wait_queue_head_t wait_for_threads;
    unsigned int nr_actions;
    unsigned int no_suspend_depth;
    unsigned int cond_suspend_depth;
    unsigned int force_resume_depth;
    struct proc_dir_entry *dir;
    struct callback_head rcu;
    struct kobject kobj;
    struct mutex request_mutex;
    int parent_irq;
    struct module *owner;
    const char *name;
    struct hlist_node resend_node;
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
struct irq_desc {
    struct irq_common_data irq_common_data;
    struct irq_data irq_data;
    unsigned int *kstat_irqs;
    irq_flow_handler_t handle_irq;
    struct irqaction *action;
    unsigned int status_use_accessors;
    unsigned int core_internal_state__do_not_mess_with_it;
    unsigned int depth;
    unsigned int wake_depth;
    unsigned int tot_count;
    unsigned int irq_count;
    long unsigned int last_unhandled;
    unsigned int irqs_unhandled;
    atomic_t threads_handled;
    int threads_handled_last;
    raw_spinlock_t lock;
    struct cpumask *percpu_enabled;
    const struct cpumask *percpu_affinity;
    const struct cpumask *affinity_hint;
    struct irq_affinity_notify *affinity_notify;
    long unsigned int threads_oneshot;
    atomic_t threads_active;
    wait_queue_head_t wait_for_threads;
    unsigned int nr_actions;
    unsigned int no_suspend_depth;
    unsigned int cond_suspend_depth;
    unsigned int force_resume_depth;
    struct proc_dir_entry *dir;
    struct callback_head rcu;
    struct kobject kobj;
    struct mutex request_mutex;
    int parent_irq;
    struct module *owner;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct irq_desc {
    struct irq_common_data irq_common_data;
    struct irq_data irq_data;
    unsigned int *kstat_irqs;
    irq_flow_handler_t handle_irq;
    struct irqaction *action;
    unsigned int status_use_accessors;
    unsigned int core_internal_state__do_not_mess_with_it;
    unsigned int depth;
    unsigned int wake_depth;
    unsigned int tot_count;
    unsigned int irq_count;
    long unsigned int last_unhandled;
    unsigned int irqs_unhandled;
    atomic_t threads_handled;
    int threads_handled_last;
    raw_spinlock_t lock;
    struct cpumask *percpu_enabled;
    const struct cpumask *percpu_affinity;
    const struct cpumask *affinity_hint;
    struct irq_affinity_notify *affinity_notify;
    long unsigned int threads_oneshot;
    atomic_t threads_active;
    wait_queue_head_t wait_for_threads;
    unsigned int nr_actions;
    unsigned int no_suspend_depth;
    unsigned int cond_suspend_depth;
    unsigned int force_resume_depth;
    struct proc_dir_entry *dir;
    struct callback_head rcu;
    struct kobject kobj;
    struct mutex request_mutex;
    int parent_irq;
    struct module *owner;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct irq_desc {
    struct irq_common_data irq_common_data;
    struct irq_data irq_data;
    unsigned int *kstat_irqs;
    irq_flow_handler_t handle_irq;
    struct irqaction *action;
    unsigned int status_use_accessors;
    unsigned int core_internal_state__do_not_mess_with_it;
    unsigned int depth;
    unsigned int wake_depth;
    unsigned int tot_count;
    unsigned int irq_count;
    long unsigned int last_unhandled;
    unsigned int irqs_unhandled;
    atomic_t threads_handled;
    int threads_handled_last;
    raw_spinlock_t lock;
    struct cpumask *percpu_enabled;
    const struct cpumask *percpu_affinity;
    const struct cpumask *affinity_hint;
    struct irq_affinity_notify *affinity_notify;
    long unsigned int threads_oneshot;
    atomic_t threads_active;
    wait_queue_head_t wait_for_threads;
    unsigned int nr_actions;
    unsigned int no_suspend_depth;
    unsigned int cond_suspend_depth;
    unsigned int force_resume_depth;
    struct proc_dir_entry *dir;
    struct callback_head rcu;
    struct kobject kobj;
    struct mutex request_mutex;
    int parent_irq;
    struct module *owner;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct irq_desc {
    struct irq_common_data irq_common_data;
    struct irq_data irq_data;
    unsigned int *kstat_irqs;
    irq_flow_handler_t handle_irq;
    struct irqaction *action;
    unsigned int status_use_accessors;
    unsigned int core_internal_state__do_not_mess_with_it;
    unsigned int depth;
    unsigned int wake_depth;
    unsigned int tot_count;
    unsigned int irq_count;
    long unsigned int last_unhandled;
    unsigned int irqs_unhandled;
    atomic_t threads_handled;
    int threads_handled_last;
    raw_spinlock_t lock;
    struct cpumask *percpu_enabled;
    const struct cpumask *percpu_affinity;
    const struct cpumask *affinity_hint;
    struct irq_affinity_notify *affinity_notify;
    long unsigned int threads_oneshot;
    atomic_t threads_active;
    wait_queue_head_t wait_for_threads;
    struct proc_dir_entry *dir;
    struct callback_head rcu;
    struct kobject kobj;
    struct mutex request_mutex;
    int parent_irq;
    struct module *owner;
    const char *name;
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
struct irq_desc {
    struct irq_common_data irq_common_data;
    struct irq_data irq_data;
    unsigned int *kstat_irqs;
    irq_flow_handler_t handle_irq;
    struct irqaction *action;
    unsigned int status_use_accessors;
    unsigned int core_internal_state__do_not_mess_with_it;
    unsigned int depth;
    unsigned int wake_depth;
    unsigned int tot_count;
    unsigned int irq_count;
    long unsigned int last_unhandled;
    unsigned int irqs_unhandled;
    atomic_t threads_handled;
    int threads_handled_last;
    raw_spinlock_t lock;
    struct cpumask *percpu_enabled;
    const struct cpumask *percpu_affinity;
    const struct cpumask *affinity_hint;
    struct irq_affinity_notify *affinity_notify;
    cpumask_var_t pending_mask;
    long unsigned int threads_oneshot;
    atomic_t threads_active;
    wait_queue_head_t wait_for_threads;
    unsigned int nr_actions;
    unsigned int no_suspend_depth;
    unsigned int cond_suspend_depth;
    unsigned int force_resume_depth;
    struct proc_dir_entry *dir;
    struct callback_head rcu;
    struct kobject kobj;
    struct mutex request_mutex;
    int parent_irq;
    struct module *owner;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct irq_desc {
    struct irq_common_data irq_common_data;
    struct irq_data irq_data;
    unsigned int *kstat_irqs;
    irq_flow_handler_t handle_irq;
    struct irqaction *action;
    unsigned int status_use_accessors;
    unsigned int core_internal_state__do_not_mess_with_it;
    unsigned int depth;
    unsigned int wake_depth;
    unsigned int tot_count;
    unsigned int irq_count;
    long unsigned int last_unhandled;
    unsigned int irqs_unhandled;
    atomic_t threads_handled;
    int threads_handled_last;
    raw_spinlock_t lock;
    struct cpumask *percpu_enabled;
    const struct cpumask *percpu_affinity;
    const struct cpumask *affinity_hint;
    struct irq_affinity_notify *affinity_notify;
    cpumask_var_t pending_mask;
    long unsigned int threads_oneshot;
    atomic_t threads_active;
    wait_queue_head_t wait_for_threads;
    unsigned int nr_actions;
    unsigned int no_suspend_depth;
    unsigned int cond_suspend_depth;
    unsigned int force_resume_depth;
    struct proc_dir_entry *dir;
    struct callback_head rcu;
    struct kobject kobj;
    struct mutex request_mutex;
    int parent_irq;
    struct module *owner;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct irq_desc {
    struct irq_common_data irq_common_data;
    struct irq_data irq_data;
    unsigned int *kstat_irqs;
    irq_flow_handler_t handle_irq;
    struct irqaction *action;
    unsigned int status_use_accessors;
    unsigned int core_internal_state__do_not_mess_with_it;
    unsigned int depth;
    unsigned int wake_depth;
    unsigned int tot_count;
    unsigned int irq_count;
    long unsigned int last_unhandled;
    unsigned int irqs_unhandled;
    atomic_t threads_handled;
    int threads_handled_last;
    raw_spinlock_t lock;
    struct cpumask *percpu_enabled;
    const struct cpumask *percpu_affinity;
    const struct cpumask *affinity_hint;
    struct irq_affinity_notify *affinity_notify;
    cpumask_var_t pending_mask;
    long unsigned int threads_oneshot;
    atomic_t threads_active;
    wait_queue_head_t wait_for_threads;
    unsigned int nr_actions;
    unsigned int no_suspend_depth;
    unsigned int cond_suspend_depth;
    unsigned int force_resume_depth;
    struct proc_dir_entry *dir;
    struct callback_head rcu;
    struct kobject kobj;
    struct mutex request_mutex;
    int parent_irq;
    struct module *owner;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct irq_desc {
    struct irq_common_data irq_common_data;
    struct irq_data irq_data;
    unsigned int *kstat_irqs;
    irq_flow_handler_t handle_irq;
    struct irqaction *action;
    unsigned int status_use_accessors;
    unsigned int core_internal_state__do_not_mess_with_it;
    unsigned int depth;
    unsigned int wake_depth;
    unsigned int tot_count;
    unsigned int irq_count;
    long unsigned int last_unhandled;
    unsigned int irqs_unhandled;
    atomic_t threads_handled;
    int threads_handled_last;
    raw_spinlock_t lock;
    struct cpumask *percpu_enabled;
    const struct cpumask *percpu_affinity;
    const struct cpumask *affinity_hint;
    struct irq_affinity_notify *affinity_notify;
    cpumask_var_t pending_mask;
    long unsigned int threads_oneshot;
    atomic_t threads_active;
    wait_queue_head_t wait_for_threads;
    unsigned int nr_actions;
    unsigned int no_suspend_depth;
    unsigned int cond_suspend_depth;
    unsigned int force_resume_depth;
    struct proc_dir_entry *dir;
    struct callback_head rcu;
    struct kobject kobj;
    struct mutex request_mutex;
    int parent_irq;
    struct module *owner;
    const char *name;
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
<code>const struct cpumask *percpu_affinity</code>
</li>
<li>
<b>Field added. </b>
<code>struct callback_head rcu</code>
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
<code>struct kobject kobj</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct mutex request_mutex</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
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
<code>unsigned int tot_count</code>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct hlist_node resend_node</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>arm64</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>cpumask_var_t pending_mask</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>cpumask_var_t pending_mask</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>cpumask_var_t pending_mask</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>cpumask_var_t pending_mask</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int nr_actions</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int no_suspend_depth</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int cond_suspend_depth</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int force_resume_depth</code>
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
