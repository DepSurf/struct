# Struct: <code>mem_cgroup</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct mem_cgroup {
    struct cgroup_subsys_state css;
    struct page_counter memory;
    struct page_counter memsw;
    struct page_counter kmem;
    long unsigned int low;
    long unsigned int high;
    long unsigned int soft_limit;
    struct vmpressure vmpressure;
    int initialized;
    bool use_hierarchy;
    bool oom_lock;
    int under_oom;
    int swappiness;
    int oom_kill_disable;
    struct cgroup_file events_file;
    struct mutex thresholds_lock;
    struct mem_cgroup_thresholds thresholds;
    struct mem_cgroup_thresholds memsw_thresholds;
    struct list_head oom_notify;
    long unsigned int move_charge_at_immigrate;
    atomic_t moving_account;
    spinlock_t move_lock;
    struct task_struct *move_lock_task;
    long unsigned int move_lock_flags;
    struct mem_cgroup_stat_cpu *stat;
    struct cg_proto tcp_mem;
    int kmemcg_id;
    bool kmem_acct_activated;
    bool kmem_acct_active;
    int last_scanned_node;
    nodemask_t scan_nodes;
    atomic_t numainfo_events;
    atomic_t numainfo_updating;
    struct list_head cgwb_list;
    struct wb_domain cgwb_domain;
    struct list_head event_list;
    spinlock_t event_list_lock;
    struct mem_cgroup_per_node * nodeinfo[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct mem_cgroup {
    struct cgroup_subsys_state css;
    struct mem_cgroup_id id;
    struct page_counter memory;
    struct page_counter swap;
    struct page_counter memsw;
    struct page_counter kmem;
    struct page_counter tcpmem;
    long unsigned int low;
    long unsigned int high;
    struct work_struct high_work;
    long unsigned int soft_limit;
    struct vmpressure vmpressure;
    bool use_hierarchy;
    bool oom_lock;
    int under_oom;
    int swappiness;
    int oom_kill_disable;
    struct cgroup_file events_file;
    struct mutex thresholds_lock;
    struct mem_cgroup_thresholds thresholds;
    struct mem_cgroup_thresholds memsw_thresholds;
    struct list_head oom_notify;
    long unsigned int move_charge_at_immigrate;
    atomic_t moving_account;
    spinlock_t move_lock;
    struct task_struct *move_lock_task;
    long unsigned int move_lock_flags;
    struct mem_cgroup_stat_cpu *stat;
    long unsigned int socket_pressure;
    bool tcpmem_active;
    int tcpmem_pressure;
    int kmemcg_id;
    enum memcg_kmem_state kmem_state;
    int last_scanned_node;
    nodemask_t scan_nodes;
    atomic_t numainfo_events;
    atomic_t numainfo_updating;
    struct list_head cgwb_list;
    struct wb_domain cgwb_domain;
    struct list_head event_list;
    spinlock_t event_list_lock;
    struct mem_cgroup_per_node * nodeinfo[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct mem_cgroup {
    struct cgroup_subsys_state css;
    struct mem_cgroup_id id;
    struct page_counter memory;
    struct page_counter swap;
    struct page_counter memsw;
    struct page_counter kmem;
    struct page_counter tcpmem;
    long unsigned int low;
    long unsigned int high;
    struct work_struct high_work;
    long unsigned int soft_limit;
    struct vmpressure vmpressure;
    bool use_hierarchy;
    bool oom_lock;
    int under_oom;
    int swappiness;
    int oom_kill_disable;
    struct cgroup_file events_file;
    struct mutex thresholds_lock;
    struct mem_cgroup_thresholds thresholds;
    struct mem_cgroup_thresholds memsw_thresholds;
    struct list_head oom_notify;
    long unsigned int move_charge_at_immigrate;
    atomic_t moving_account;
    spinlock_t move_lock;
    struct task_struct *move_lock_task;
    long unsigned int move_lock_flags;
    struct mem_cgroup_stat_cpu *stat;
    long unsigned int socket_pressure;
    bool tcpmem_active;
    int tcpmem_pressure;
    int kmemcg_id;
    enum memcg_kmem_state kmem_state;
    int last_scanned_node;
    nodemask_t scan_nodes;
    atomic_t numainfo_events;
    atomic_t numainfo_updating;
    struct list_head cgwb_list;
    struct wb_domain cgwb_domain;
    struct list_head event_list;
    spinlock_t event_list_lock;
    struct mem_cgroup_per_node * nodeinfo[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct mem_cgroup {
    struct cgroup_subsys_state css;
    struct mem_cgroup_id id;
    struct page_counter memory;
    struct page_counter swap;
    struct page_counter memsw;
    struct page_counter kmem;
    struct page_counter tcpmem;
    long unsigned int low;
    long unsigned int high;
    struct work_struct high_work;
    long unsigned int soft_limit;
    struct vmpressure vmpressure;
    bool use_hierarchy;
    bool oom_lock;
    int under_oom;
    int swappiness;
    int oom_kill_disable;
    struct cgroup_file events_file;
    struct mutex thresholds_lock;
    struct mem_cgroup_thresholds thresholds;
    struct mem_cgroup_thresholds memsw_thresholds;
    struct list_head oom_notify;
    long unsigned int move_charge_at_immigrate;
    atomic_t moving_account;
    spinlock_t move_lock;
    struct task_struct *move_lock_task;
    long unsigned int move_lock_flags;
    struct mem_cgroup_stat_cpu *stat;
    long unsigned int socket_pressure;
    bool tcpmem_active;
    int tcpmem_pressure;
    int kmemcg_id;
    enum memcg_kmem_state kmem_state;
    struct list_head kmem_caches;
    int last_scanned_node;
    nodemask_t scan_nodes;
    atomic_t numainfo_events;
    atomic_t numainfo_updating;
    struct list_head cgwb_list;
    struct wb_domain cgwb_domain;
    struct list_head event_list;
    spinlock_t event_list_lock;
    struct mem_cgroup_per_node * nodeinfo[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct mem_cgroup {
    struct cgroup_subsys_state css;
    struct mem_cgroup_id id;
    struct page_counter memory;
    struct page_counter swap;
    struct page_counter memsw;
    struct page_counter kmem;
    struct page_counter tcpmem;
    long unsigned int low;
    long unsigned int high;
    struct work_struct high_work;
    long unsigned int soft_limit;
    struct vmpressure vmpressure;
    bool use_hierarchy;
    bool oom_lock;
    int under_oom;
    int swappiness;
    int oom_kill_disable;
    struct cgroup_file events_file;
    struct mutex thresholds_lock;
    struct mem_cgroup_thresholds thresholds;
    struct mem_cgroup_thresholds memsw_thresholds;
    struct list_head oom_notify;
    long unsigned int move_charge_at_immigrate;
    atomic_t moving_account;
    spinlock_t move_lock;
    struct task_struct *move_lock_task;
    long unsigned int move_lock_flags;
    struct mem_cgroup_stat_cpu *stat;
    long unsigned int socket_pressure;
    bool tcpmem_active;
    int tcpmem_pressure;
    int kmemcg_id;
    enum memcg_kmem_state kmem_state;
    struct list_head kmem_caches;
    int last_scanned_node;
    nodemask_t scan_nodes;
    atomic_t numainfo_events;
    atomic_t numainfo_updating;
    struct list_head cgwb_list;
    struct wb_domain cgwb_domain;
    struct list_head event_list;
    spinlock_t event_list_lock;
    struct mem_cgroup_per_node * nodeinfo[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct mem_cgroup {
    struct cgroup_subsys_state css;
    struct mem_cgroup_id id;
    struct page_counter memory;
    struct page_counter swap;
    struct page_counter memsw;
    struct page_counter kmem;
    struct page_counter tcpmem;
    long unsigned int high;
    struct work_struct high_work;
    long unsigned int soft_limit;
    struct vmpressure vmpressure;
    bool use_hierarchy;
    bool oom_lock;
    int under_oom;
    int swappiness;
    int oom_kill_disable;
    struct cgroup_file events_file;
    struct cgroup_file swap_events_file;
    struct mutex thresholds_lock;
    struct mem_cgroup_thresholds thresholds;
    struct mem_cgroup_thresholds memsw_thresholds;
    struct list_head oom_notify;
    long unsigned int move_charge_at_immigrate;
    spinlock_t move_lock;
    long unsigned int move_lock_flags;
    struct memcg_padding _pad1_;
    atomic_t moving_account;
    struct task_struct *move_lock_task;
    struct mem_cgroup_stat_cpu *stat_cpu;
    struct memcg_padding _pad2_;
    atomic_long_t stat[34];
    atomic_long_t events[85];
    atomic_long_t memory_events[7];
    long unsigned int socket_pressure;
    bool tcpmem_active;
    int tcpmem_pressure;
    int kmemcg_id;
    enum memcg_kmem_state kmem_state;
    struct list_head kmem_caches;
    int last_scanned_node;
    nodemask_t scan_nodes;
    atomic_t numainfo_events;
    atomic_t numainfo_updating;
    struct list_head cgwb_list;
    struct wb_domain cgwb_domain;
    struct list_head event_list;
    spinlock_t event_list_lock;
    struct mem_cgroup_per_node * nodeinfo[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct mem_cgroup {
    struct cgroup_subsys_state css;
    struct mem_cgroup_id id;
    struct page_counter memory;
    struct page_counter swap;
    struct page_counter memsw;
    struct page_counter kmem;
    struct page_counter tcpmem;
    long unsigned int high;
    struct work_struct high_work;
    long unsigned int soft_limit;
    struct vmpressure vmpressure;
    bool use_hierarchy;
    bool oom_group;
    bool oom_lock;
    int under_oom;
    int swappiness;
    int oom_kill_disable;
    struct cgroup_file events_file;
    struct cgroup_file swap_events_file;
    struct mutex thresholds_lock;
    struct mem_cgroup_thresholds thresholds;
    struct mem_cgroup_thresholds memsw_thresholds;
    struct list_head oom_notify;
    long unsigned int move_charge_at_immigrate;
    spinlock_t move_lock;
    long unsigned int move_lock_flags;
    struct memcg_padding _pad1_;
    atomic_t moving_account;
    struct task_struct *move_lock_task;
    struct mem_cgroup_stat_cpu *stat_cpu;
    struct memcg_padding _pad2_;
    atomic_long_t stat[36];
    atomic_long_t events[85];
    atomic_long_t memory_events[7];
    long unsigned int socket_pressure;
    bool tcpmem_active;
    int tcpmem_pressure;
    int kmemcg_id;
    enum memcg_kmem_state kmem_state;
    struct list_head kmem_caches;
    int last_scanned_node;
    nodemask_t scan_nodes;
    atomic_t numainfo_events;
    atomic_t numainfo_updating;
    struct list_head cgwb_list;
    struct wb_domain cgwb_domain;
    struct list_head event_list;
    spinlock_t event_list_lock;
    struct mem_cgroup_per_node * nodeinfo[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct mem_cgroup {
    struct cgroup_subsys_state css;
    struct mem_cgroup_id id;
    struct page_counter memory;
    struct page_counter swap;
    struct page_counter memsw;
    struct page_counter kmem;
    struct page_counter tcpmem;
    long unsigned int high;
    struct work_struct high_work;
    long unsigned int soft_limit;
    struct vmpressure vmpressure;
    bool use_hierarchy;
    bool oom_group;
    bool oom_lock;
    int under_oom;
    int swappiness;
    int oom_kill_disable;
    struct cgroup_file events_file;
    struct cgroup_file events_local_file;
    struct cgroup_file swap_events_file;
    struct mutex thresholds_lock;
    struct mem_cgroup_thresholds thresholds;
    struct mem_cgroup_thresholds memsw_thresholds;
    struct list_head oom_notify;
    long unsigned int move_charge_at_immigrate;
    spinlock_t move_lock;
    long unsigned int move_lock_flags;
    struct memcg_padding _pad1_;
    atomic_t moving_account;
    struct task_struct *move_lock_task;
    struct memcg_vmstats_percpu *vmstats_local;
    struct memcg_vmstats_percpu *vmstats_percpu;
    struct memcg_padding _pad2_;
    atomic_long_t vmstats[36];
    atomic_long_t vmevents[85];
    atomic_long_t memory_events[7];
    atomic_long_t memory_events_local[7];
    long unsigned int socket_pressure;
    bool tcpmem_active;
    int tcpmem_pressure;
    int kmemcg_id;
    enum memcg_kmem_state kmem_state;
    struct list_head kmem_caches;
    int last_scanned_node;
    nodemask_t scan_nodes;
    atomic_t numainfo_events;
    atomic_t numainfo_updating;
    struct list_head cgwb_list;
    struct wb_domain cgwb_domain;
    struct list_head event_list;
    spinlock_t event_list_lock;
    struct mem_cgroup_per_node * nodeinfo[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct mem_cgroup {
    struct cgroup_subsys_state css;
    struct mem_cgroup_id id;
    struct page_counter memory;
    struct page_counter swap;
    struct page_counter memsw;
    struct page_counter kmem;
    struct page_counter tcpmem;
    long unsigned int high;
    struct work_struct high_work;
    long unsigned int soft_limit;
    struct vmpressure vmpressure;
    bool use_hierarchy;
    bool oom_group;
    bool oom_lock;
    int under_oom;
    int swappiness;
    int oom_kill_disable;
    struct cgroup_file events_file;
    struct cgroup_file events_local_file;
    struct cgroup_file swap_events_file;
    struct mutex thresholds_lock;
    struct mem_cgroup_thresholds thresholds;
    struct mem_cgroup_thresholds memsw_thresholds;
    struct list_head oom_notify;
    long unsigned int move_charge_at_immigrate;
    spinlock_t move_lock;
    long unsigned int move_lock_flags;
    struct memcg_padding _pad1_;
    atomic_t moving_account;
    struct task_struct *move_lock_task;
    struct memcg_vmstats_percpu *vmstats_local;
    struct memcg_vmstats_percpu *vmstats_percpu;
    struct memcg_padding _pad2_;
    atomic_long_t vmstats[38];
    atomic_long_t vmevents[85];
    atomic_long_t memory_events[7];
    atomic_long_t memory_events_local[7];
    long unsigned int socket_pressure;
    bool tcpmem_active;
    int tcpmem_pressure;
    int kmemcg_id;
    enum memcg_kmem_state kmem_state;
    struct list_head kmem_caches;
    int last_scanned_node;
    nodemask_t scan_nodes;
    atomic_t numainfo_events;
    atomic_t numainfo_updating;
    struct list_head cgwb_list;
    struct wb_domain cgwb_domain;
    struct memcg_cgwb_frn cgwb_frn[4];
    struct list_head event_list;
    spinlock_t event_list_lock;
    struct deferred_split deferred_split_queue;
    struct mem_cgroup_per_node * nodeinfo[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct mem_cgroup {
    struct cgroup_subsys_state css;
    struct mem_cgroup_id id;
    struct page_counter memory;
    struct page_counter swap;
    struct page_counter memsw;
    struct page_counter kmem;
    struct page_counter tcpmem;
    struct work_struct high_work;
    long unsigned int soft_limit;
    struct vmpressure vmpressure;
    bool use_hierarchy;
    bool oom_group;
    bool oom_lock;
    int under_oom;
    int swappiness;
    int oom_kill_disable;
    struct cgroup_file events_file;
    struct cgroup_file events_local_file;
    struct cgroup_file swap_events_file;
    struct mutex thresholds_lock;
    struct mem_cgroup_thresholds thresholds;
    struct mem_cgroup_thresholds memsw_thresholds;
    struct list_head oom_notify;
    long unsigned int move_charge_at_immigrate;
    spinlock_t move_lock;
    long unsigned int move_lock_flags;
    struct memcg_padding _pad1_;
    atomic_t moving_account;
    struct task_struct *move_lock_task;
    struct memcg_vmstats_percpu *vmstats_local;
    struct memcg_vmstats_percpu *vmstats_percpu;
    struct memcg_padding _pad2_;
    atomic_long_t vmstats[36];
    atomic_long_t vmevents[92];
    atomic_long_t memory_events[8];
    atomic_long_t memory_events_local[8];
    long unsigned int socket_pressure;
    bool tcpmem_active;
    int tcpmem_pressure;
    int kmemcg_id;
    enum memcg_kmem_state kmem_state;
    struct list_head kmem_caches;
    struct list_head cgwb_list;
    struct wb_domain cgwb_domain;
    struct memcg_cgwb_frn cgwb_frn[4];
    struct list_head event_list;
    spinlock_t event_list_lock;
    struct deferred_split deferred_split_queue;
    struct mem_cgroup_per_node * nodeinfo[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mem_cgroup {
    struct cgroup_subsys_state css;
    struct mem_cgroup_id id;
    struct page_counter memory;
    struct page_counter swap;
    struct page_counter memsw;
    struct page_counter kmem;
    struct page_counter tcpmem;
    struct work_struct high_work;
    long unsigned int soft_limit;
    struct vmpressure vmpressure;
    bool oom_group;
    bool oom_lock;
    int under_oom;
    int swappiness;
    int oom_kill_disable;
    struct cgroup_file events_file;
    struct cgroup_file events_local_file;
    struct cgroup_file swap_events_file;
    struct mutex thresholds_lock;
    struct mem_cgroup_thresholds thresholds;
    struct mem_cgroup_thresholds memsw_thresholds;
    struct list_head oom_notify;
    long unsigned int move_charge_at_immigrate;
    spinlock_t move_lock;
    long unsigned int move_lock_flags;
    struct memcg_padding _pad1_;
    atomic_long_t vmstats[41];
    atomic_long_t vmevents[96];
    atomic_long_t memory_events[8];
    atomic_long_t memory_events_local[8];
    long unsigned int socket_pressure;
    bool tcpmem_active;
    int tcpmem_pressure;
    int kmemcg_id;
    enum memcg_kmem_state kmem_state;
    struct obj_cgroup *objcg;
    struct list_head objcg_list;
    struct memcg_padding _pad2_;
    atomic_t moving_account;
    struct task_struct *move_lock_task;
    struct memcg_vmstats_percpu *vmstats_local;
    struct memcg_vmstats_percpu *vmstats_percpu;
    struct list_head cgwb_list;
    struct wb_domain cgwb_domain;
    struct memcg_cgwb_frn cgwb_frn[4];
    struct list_head event_list;
    spinlock_t event_list_lock;
    struct deferred_split deferred_split_queue;
    struct mem_cgroup_per_node * nodeinfo[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mem_cgroup {
    struct cgroup_subsys_state css;
    struct mem_cgroup_id id;
    struct page_counter memory;
    struct page_counter swap;
    struct page_counter memsw;
    struct page_counter kmem;
    struct page_counter tcpmem;
    struct work_struct high_work;
    long unsigned int soft_limit;
    struct vmpressure vmpressure;
    bool oom_group;
    bool oom_lock;
    int under_oom;
    int swappiness;
    int oom_kill_disable;
    struct cgroup_file events_file;
    struct cgroup_file events_local_file;
    struct cgroup_file swap_events_file;
    struct mutex thresholds_lock;
    struct mem_cgroup_thresholds thresholds;
    struct mem_cgroup_thresholds memsw_thresholds;
    struct list_head oom_notify;
    long unsigned int move_charge_at_immigrate;
    spinlock_t move_lock;
    long unsigned int move_lock_flags;
    struct memcg_padding _pad1_;
    struct memcg_vmstats vmstats;
    atomic_long_t memory_events[8];
    atomic_long_t memory_events_local[8];
    long unsigned int socket_pressure;
    bool tcpmem_active;
    int tcpmem_pressure;
    int kmemcg_id;
    enum memcg_kmem_state kmem_state;
    struct obj_cgroup *objcg;
    struct list_head objcg_list;
    struct memcg_padding _pad2_;
    atomic_t moving_account;
    struct task_struct *move_lock_task;
    struct memcg_vmstats_percpu *vmstats_percpu;
    struct list_head cgwb_list;
    struct wb_domain cgwb_domain;
    struct memcg_cgwb_frn cgwb_frn[4];
    struct list_head event_list;
    spinlock_t event_list_lock;
    struct deferred_split deferred_split_queue;
    struct mem_cgroup_per_node * nodeinfo[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mem_cgroup {
    struct cgroup_subsys_state css;
    struct mem_cgroup_id id;
    struct page_counter memory;
    struct page_counter swap;
    struct page_counter memsw;
    struct page_counter kmem;
    struct page_counter tcpmem;
    struct work_struct high_work;
    long unsigned int soft_limit;
    struct vmpressure vmpressure;
    bool oom_group;
    bool oom_lock;
    int under_oom;
    int swappiness;
    int oom_kill_disable;
    struct cgroup_file events_file;
    struct cgroup_file events_local_file;
    struct cgroup_file swap_events_file;
    struct mutex thresholds_lock;
    struct mem_cgroup_thresholds thresholds;
    struct mem_cgroup_thresholds memsw_thresholds;
    struct list_head oom_notify;
    long unsigned int move_charge_at_immigrate;
    spinlock_t move_lock;
    long unsigned int move_lock_flags;
    struct memcg_padding _pad1_;
    struct memcg_vmstats vmstats;
    atomic_long_t memory_events[8];
    atomic_long_t memory_events_local[8];
    long unsigned int socket_pressure;
    bool tcpmem_active;
    int tcpmem_pressure;
    int kmemcg_id;
    enum memcg_kmem_state kmem_state;
    struct obj_cgroup *objcg;
    struct list_head objcg_list;
    struct memcg_padding _pad2_;
    atomic_t moving_account;
    struct task_struct *move_lock_task;
    struct memcg_vmstats_percpu *vmstats_percpu;
    struct list_head cgwb_list;
    struct wb_domain cgwb_domain;
    struct memcg_cgwb_frn cgwb_frn[4];
    struct list_head event_list;
    spinlock_t event_list_lock;
    struct deferred_split deferred_split_queue;
    struct mem_cgroup_per_node * nodeinfo[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mem_cgroup {
    struct cgroup_subsys_state css;
    struct mem_cgroup_id id;
    struct page_counter memory;
    struct page_counter swap;
    struct page_counter memsw;
    struct page_counter kmem;
    struct page_counter tcpmem;
    struct work_struct high_work;
    long unsigned int zswap_max;
    long unsigned int soft_limit;
    struct vmpressure vmpressure;
    bool oom_group;
    bool oom_lock;
    int under_oom;
    int swappiness;
    int oom_kill_disable;
    struct cgroup_file events_file;
    struct cgroup_file events_local_file;
    struct cgroup_file swap_events_file;
    struct mutex thresholds_lock;
    struct mem_cgroup_thresholds thresholds;
    struct mem_cgroup_thresholds memsw_thresholds;
    struct list_head oom_notify;
    long unsigned int move_charge_at_immigrate;
    spinlock_t move_lock;
    long unsigned int move_lock_flags;
    struct memcg_padding _pad1_;
    struct memcg_vmstats vmstats;
    atomic_long_t memory_events[9];
    atomic_long_t memory_events_local[9];
    long unsigned int socket_pressure;
    bool tcpmem_active;
    int tcpmem_pressure;
    int kmemcg_id;
    struct obj_cgroup *objcg;
    struct list_head objcg_list;
    struct memcg_padding _pad2_;
    atomic_t moving_account;
    struct task_struct *move_lock_task;
    struct memcg_vmstats_percpu *vmstats_percpu;
    struct list_head cgwb_list;
    struct wb_domain cgwb_domain;
    struct memcg_cgwb_frn cgwb_frn[4];
    struct list_head event_list;
    spinlock_t event_list_lock;
    struct deferred_split deferred_split_queue;
    struct mem_cgroup_per_node * nodeinfo[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mem_cgroup {
    struct cgroup_subsys_state css;
    struct mem_cgroup_id id;
    struct page_counter memory;
    struct page_counter swap;
    struct page_counter memsw;
    struct page_counter kmem;
    struct page_counter tcpmem;
    struct work_struct high_work;
    long unsigned int zswap_max;
    long unsigned int soft_limit;
    struct vmpressure vmpressure;
    bool oom_group;
    bool oom_lock;
    int under_oom;
    int swappiness;
    int oom_kill_disable;
    struct cgroup_file events_file;
    struct cgroup_file events_local_file;
    struct cgroup_file swap_events_file;
    struct mutex thresholds_lock;
    struct mem_cgroup_thresholds thresholds;
    struct mem_cgroup_thresholds memsw_thresholds;
    struct list_head oom_notify;
    long unsigned int move_charge_at_immigrate;
    spinlock_t move_lock;
    long unsigned int move_lock_flags;
    struct cacheline_padding _pad1_;
    struct memcg_vmstats *vmstats;
    atomic_long_t memory_events[9];
    atomic_long_t memory_events_local[9];
    long unsigned int socket_pressure;
    bool tcpmem_active;
    int tcpmem_pressure;
    int kmemcg_id;
    struct obj_cgroup *objcg;
    struct list_head objcg_list;
    struct cacheline_padding _pad2_;
    atomic_t moving_account;
    struct task_struct *move_lock_task;
    struct memcg_vmstats_percpu *vmstats_percpu;
    struct list_head cgwb_list;
    struct wb_domain cgwb_domain;
    struct memcg_cgwb_frn cgwb_frn[4];
    struct list_head event_list;
    spinlock_t event_list_lock;
    struct deferred_split deferred_split_queue;
    struct lru_gen_mm_list mm_list;
    struct mem_cgroup_per_node * nodeinfo[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mem_cgroup {
    struct cgroup_subsys_state css;
    struct mem_cgroup_id id;
    struct page_counter memory;
    struct page_counter swap;
    struct page_counter memsw;
    struct page_counter kmem;
    struct page_counter tcpmem;
    struct work_struct high_work;
    long unsigned int zswap_max;
    long unsigned int soft_limit;
    struct vmpressure vmpressure;
    bool oom_group;
    bool oom_lock;
    int under_oom;
    int swappiness;
    int oom_kill_disable;
    struct cgroup_file events_file;
    struct cgroup_file events_local_file;
    struct cgroup_file swap_events_file;
    struct mutex thresholds_lock;
    struct mem_cgroup_thresholds thresholds;
    struct mem_cgroup_thresholds memsw_thresholds;
    struct list_head oom_notify;
    long unsigned int move_charge_at_immigrate;
    spinlock_t move_lock;
    long unsigned int move_lock_flags;
    struct cacheline_padding _pad1_;
    struct memcg_vmstats *vmstats;
    atomic_long_t memory_events[9];
    atomic_long_t memory_events_local[9];
    long unsigned int socket_pressure;
    bool tcpmem_active;
    int tcpmem_pressure;
    int kmemcg_id;
    struct obj_cgroup *objcg;
    struct list_head objcg_list;
    struct cacheline_padding _pad2_;
    atomic_t moving_account;
    struct task_struct *move_lock_task;
    struct memcg_vmstats_percpu *vmstats_percpu;
    struct list_head cgwb_list;
    struct wb_domain cgwb_domain;
    struct memcg_cgwb_frn cgwb_frn[4];
    struct list_head event_list;
    spinlock_t event_list_lock;
    struct deferred_split deferred_split_queue;
    struct lru_gen_mm_list mm_list;
    struct mem_cgroup_per_node * nodeinfo[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mem_cgroup {
    struct cgroup_subsys_state css;
    struct mem_cgroup_id id;
    struct page_counter memory;
    struct page_counter swap;
    struct page_counter memsw;
    struct page_counter kmem;
    struct page_counter tcpmem;
    struct work_struct high_work;
    long unsigned int zswap_max;
    bool zswap_writeback;
    long unsigned int soft_limit;
    struct vmpressure vmpressure;
    bool oom_group;
    bool oom_lock;
    int under_oom;
    int swappiness;
    int oom_kill_disable;
    struct cgroup_file events_file;
    struct cgroup_file events_local_file;
    struct cgroup_file swap_events_file;
    struct mutex thresholds_lock;
    struct mem_cgroup_thresholds thresholds;
    struct mem_cgroup_thresholds memsw_thresholds;
    struct list_head oom_notify;
    long unsigned int move_charge_at_immigrate;
    spinlock_t move_lock;
    long unsigned int move_lock_flags;
    struct cacheline_padding _pad1_;
    struct memcg_vmstats *vmstats;
    atomic_long_t memory_events[9];
    atomic_long_t memory_events_local[9];
    long unsigned int socket_pressure;
    bool tcpmem_active;
    int tcpmem_pressure;
    int kmemcg_id;
    struct obj_cgroup *objcg;
    struct obj_cgroup *orig_objcg;
    struct list_head objcg_list;
    struct cacheline_padding _pad2_;
    atomic_t moving_account;
    struct task_struct *move_lock_task;
    struct memcg_vmstats_percpu *vmstats_percpu;
    struct list_head cgwb_list;
    struct wb_domain cgwb_domain;
    struct memcg_cgwb_frn cgwb_frn[4];
    struct list_head event_list;
    spinlock_t event_list_lock;
    struct deferred_split deferred_split_queue;
    struct lru_gen_mm_list mm_list;
    struct mem_cgroup_per_node * nodeinfo[0];
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
struct mem_cgroup {
    struct cgroup_subsys_state css;
    struct mem_cgroup_id id;
    struct page_counter memory;
    struct page_counter swap;
    struct page_counter memsw;
    struct page_counter kmem;
    struct page_counter tcpmem;
    long unsigned int high;
    struct work_struct high_work;
    long unsigned int soft_limit;
    struct vmpressure vmpressure;
    bool use_hierarchy;
    bool oom_group;
    bool oom_lock;
    int under_oom;
    int swappiness;
    int oom_kill_disable;
    struct cgroup_file events_file;
    struct cgroup_file events_local_file;
    struct cgroup_file swap_events_file;
    struct mutex thresholds_lock;
    struct mem_cgroup_thresholds thresholds;
    struct mem_cgroup_thresholds memsw_thresholds;
    struct list_head oom_notify;
    long unsigned int move_charge_at_immigrate;
    spinlock_t move_lock;
    long unsigned int move_lock_flags;
    struct memcg_padding _pad1_;
    atomic_t moving_account;
    struct task_struct *move_lock_task;
    struct memcg_vmstats_percpu *vmstats_local;
    struct memcg_vmstats_percpu *vmstats_percpu;
    struct memcg_padding _pad2_;
    atomic_long_t vmstats[38];
    atomic_long_t vmevents[81];
    atomic_long_t memory_events[7];
    atomic_long_t memory_events_local[7];
    long unsigned int socket_pressure;
    bool tcpmem_active;
    int tcpmem_pressure;
    int kmemcg_id;
    enum memcg_kmem_state kmem_state;
    struct list_head kmem_caches;
    int last_scanned_node;
    nodemask_t scan_nodes;
    atomic_t numainfo_events;
    atomic_t numainfo_updating;
    struct list_head cgwb_list;
    struct wb_domain cgwb_domain;
    struct memcg_cgwb_frn cgwb_frn[4];
    struct list_head event_list;
    spinlock_t event_list_lock;
    struct deferred_split deferred_split_queue;
    struct mem_cgroup_per_node * nodeinfo[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mem_cgroup {
    struct cgroup_subsys_state css;
    struct mem_cgroup_id id;
    struct page_counter memory;
    struct page_counter swap;
    struct page_counter memsw;
    struct page_counter kmem;
    struct page_counter tcpmem;
    long unsigned int high;
    struct work_struct high_work;
    long unsigned int soft_limit;
    struct vmpressure vmpressure;
    bool use_hierarchy;
    bool oom_group;
    bool oom_lock;
    int under_oom;
    int swappiness;
    int oom_kill_disable;
    struct cgroup_file events_file;
    struct cgroup_file events_local_file;
    struct cgroup_file swap_events_file;
    struct mutex thresholds_lock;
    struct mem_cgroup_thresholds thresholds;
    struct mem_cgroup_thresholds memsw_thresholds;
    struct list_head oom_notify;
    long unsigned int move_charge_at_immigrate;
    spinlock_t move_lock;
    long unsigned int move_lock_flags;
    struct memcg_padding _pad1_;
    atomic_t moving_account;
    struct task_struct *move_lock_task;
    struct memcg_vmstats_percpu *vmstats_local;
    struct memcg_vmstats_percpu *vmstats_percpu;
    struct memcg_padding _pad2_;
    atomic_long_t vmstats[38];
    atomic_long_t vmevents[59];
    atomic_long_t memory_events[7];
    atomic_long_t memory_events_local[7];
    long unsigned int socket_pressure;
    bool tcpmem_active;
    int tcpmem_pressure;
    int kmemcg_id;
    enum memcg_kmem_state kmem_state;
    struct list_head kmem_caches;
    int last_scanned_node;
    struct list_head cgwb_list;
    struct wb_domain cgwb_domain;
    struct memcg_cgwb_frn cgwb_frn[4];
    struct list_head event_list;
    spinlock_t event_list_lock;
    struct mem_cgroup_per_node * nodeinfo[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct mem_cgroup {
    struct cgroup_subsys_state css;
    struct mem_cgroup_id id;
    struct page_counter memory;
    struct page_counter swap;
    struct page_counter memsw;
    struct page_counter kmem;
    struct page_counter tcpmem;
    long unsigned int high;
    struct work_struct high_work;
    long unsigned int soft_limit;
    struct vmpressure vmpressure;
    bool use_hierarchy;
    bool oom_group;
    bool oom_lock;
    int under_oom;
    int swappiness;
    int oom_kill_disable;
    struct cgroup_file events_file;
    struct cgroup_file events_local_file;
    struct cgroup_file swap_events_file;
    struct mutex thresholds_lock;
    struct mem_cgroup_thresholds thresholds;
    struct mem_cgroup_thresholds memsw_thresholds;
    struct list_head oom_notify;
    long unsigned int move_charge_at_immigrate;
    spinlock_t move_lock;
    long unsigned int move_lock_flags;
    struct memcg_padding _pad1_;
    atomic_t moving_account;
    struct task_struct *move_lock_task;
    struct memcg_vmstats_percpu *vmstats_local;
    struct memcg_vmstats_percpu *vmstats_percpu;
    struct memcg_padding _pad2_;
    atomic_long_t vmstats[38];
    atomic_long_t vmevents[78];
    atomic_long_t memory_events[7];
    atomic_long_t memory_events_local[7];
    long unsigned int socket_pressure;
    bool tcpmem_active;
    int tcpmem_pressure;
    int kmemcg_id;
    enum memcg_kmem_state kmem_state;
    struct list_head kmem_caches;
    int last_scanned_node;
    nodemask_t scan_nodes;
    atomic_t numainfo_events;
    atomic_t numainfo_updating;
    struct list_head cgwb_list;
    struct wb_domain cgwb_domain;
    struct memcg_cgwb_frn cgwb_frn[4];
    struct list_head event_list;
    spinlock_t event_list_lock;
    struct deferred_split deferred_split_queue;
    struct mem_cgroup_per_node * nodeinfo[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct mem_cgroup {
    struct cgroup_subsys_state css;
    struct mem_cgroup_id id;
    struct page_counter memory;
    struct page_counter swap;
    struct page_counter memsw;
    struct page_counter kmem;
    struct page_counter tcpmem;
    long unsigned int high;
    struct work_struct high_work;
    long unsigned int soft_limit;
    struct vmpressure vmpressure;
    bool use_hierarchy;
    bool oom_group;
    bool oom_lock;
    int under_oom;
    int swappiness;
    int oom_kill_disable;
    struct cgroup_file events_file;
    struct cgroup_file events_local_file;
    struct cgroup_file swap_events_file;
    struct mutex thresholds_lock;
    struct mem_cgroup_thresholds thresholds;
    struct mem_cgroup_thresholds memsw_thresholds;
    struct list_head oom_notify;
    long unsigned int move_charge_at_immigrate;
    spinlock_t move_lock;
    long unsigned int move_lock_flags;
    struct memcg_padding _pad1_;
    atomic_t moving_account;
    struct task_struct *move_lock_task;
    struct memcg_vmstats_percpu *vmstats_local;
    struct memcg_vmstats_percpu *vmstats_percpu;
    struct memcg_padding _pad2_;
    atomic_long_t vmstats[38];
    atomic_long_t vmevents[61];
    atomic_long_t memory_events[7];
    atomic_long_t memory_events_local[7];
    long unsigned int socket_pressure;
    bool tcpmem_active;
    int tcpmem_pressure;
    int kmemcg_id;
    enum memcg_kmem_state kmem_state;
    struct list_head kmem_caches;
    int last_scanned_node;
    struct list_head cgwb_list;
    struct wb_domain cgwb_domain;
    struct memcg_cgwb_frn cgwb_frn[4];
    struct list_head event_list;
    spinlock_t event_list_lock;
    struct mem_cgroup_per_node * nodeinfo[0];
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
struct mem_cgroup {
    struct cgroup_subsys_state css;
    struct mem_cgroup_id id;
    struct page_counter memory;
    struct page_counter swap;
    struct page_counter memsw;
    struct page_counter kmem;
    struct page_counter tcpmem;
    long unsigned int high;
    struct work_struct high_work;
    long unsigned int soft_limit;
    struct vmpressure vmpressure;
    bool use_hierarchy;
    bool oom_group;
    bool oom_lock;
    int under_oom;
    int swappiness;
    int oom_kill_disable;
    struct cgroup_file events_file;
    struct cgroup_file events_local_file;
    struct cgroup_file swap_events_file;
    struct mutex thresholds_lock;
    struct mem_cgroup_thresholds thresholds;
    struct mem_cgroup_thresholds memsw_thresholds;
    struct list_head oom_notify;
    long unsigned int move_charge_at_immigrate;
    spinlock_t move_lock;
    long unsigned int move_lock_flags;
    struct memcg_padding _pad1_;
    atomic_t moving_account;
    struct task_struct *move_lock_task;
    struct memcg_vmstats_percpu *vmstats_local;
    struct memcg_vmstats_percpu *vmstats_percpu;
    struct memcg_padding _pad2_;
    atomic_long_t vmstats[38];
    atomic_long_t vmevents[85];
    atomic_long_t memory_events[7];
    atomic_long_t memory_events_local[7];
    long unsigned int socket_pressure;
    bool tcpmem_active;
    int tcpmem_pressure;
    int kmemcg_id;
    enum memcg_kmem_state kmem_state;
    struct list_head kmem_caches;
    int last_scanned_node;
    nodemask_t scan_nodes;
    atomic_t numainfo_events;
    atomic_t numainfo_updating;
    struct list_head cgwb_list;
    struct wb_domain cgwb_domain;
    struct memcg_cgwb_frn cgwb_frn[4];
    struct list_head event_list;
    spinlock_t event_list_lock;
    struct deferred_split deferred_split_queue;
    struct mem_cgroup_per_node * nodeinfo[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct mem_cgroup {
    struct cgroup_subsys_state css;
    struct mem_cgroup_id id;
    struct page_counter memory;
    struct page_counter swap;
    struct page_counter memsw;
    struct page_counter kmem;
    struct page_counter tcpmem;
    long unsigned int high;
    struct work_struct high_work;
    long unsigned int soft_limit;
    struct vmpressure vmpressure;
    bool use_hierarchy;
    bool oom_group;
    bool oom_lock;
    int under_oom;
    int swappiness;
    int oom_kill_disable;
    struct cgroup_file events_file;
    struct cgroup_file events_local_file;
    struct cgroup_file swap_events_file;
    struct mutex thresholds_lock;
    struct mem_cgroup_thresholds thresholds;
    struct mem_cgroup_thresholds memsw_thresholds;
    struct list_head oom_notify;
    long unsigned int move_charge_at_immigrate;
    spinlock_t move_lock;
    long unsigned int move_lock_flags;
    struct memcg_padding _pad1_;
    atomic_t moving_account;
    struct task_struct *move_lock_task;
    struct memcg_vmstats_percpu *vmstats_local;
    struct memcg_vmstats_percpu *vmstats_percpu;
    struct memcg_padding _pad2_;
    atomic_long_t vmstats[38];
    atomic_long_t vmevents[85];
    atomic_long_t memory_events[7];
    atomic_long_t memory_events_local[7];
    long unsigned int socket_pressure;
    bool tcpmem_active;
    int tcpmem_pressure;
    int kmemcg_id;
    enum memcg_kmem_state kmem_state;
    struct list_head kmem_caches;
    int last_scanned_node;
    nodemask_t scan_nodes;
    atomic_t numainfo_events;
    atomic_t numainfo_updating;
    struct list_head cgwb_list;
    struct wb_domain cgwb_domain;
    struct memcg_cgwb_frn cgwb_frn[4];
    struct list_head event_list;
    spinlock_t event_list_lock;
    struct deferred_split deferred_split_queue;
    struct mem_cgroup_per_node * nodeinfo[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct mem_cgroup {
    struct cgroup_subsys_state css;
    struct mem_cgroup_id id;
    struct page_counter memory;
    struct page_counter swap;
    struct page_counter memsw;
    struct page_counter kmem;
    struct page_counter tcpmem;
    long unsigned int high;
    struct work_struct high_work;
    long unsigned int soft_limit;
    struct vmpressure vmpressure;
    bool use_hierarchy;
    bool oom_group;
    bool oom_lock;
    int under_oom;
    int swappiness;
    int oom_kill_disable;
    struct cgroup_file events_file;
    struct cgroup_file events_local_file;
    struct cgroup_file swap_events_file;
    struct mutex thresholds_lock;
    struct mem_cgroup_thresholds thresholds;
    struct mem_cgroup_thresholds memsw_thresholds;
    struct list_head oom_notify;
    long unsigned int move_charge_at_immigrate;
    spinlock_t move_lock;
    long unsigned int move_lock_flags;
    struct memcg_padding _pad1_;
    atomic_t moving_account;
    struct task_struct *move_lock_task;
    struct memcg_vmstats_percpu *vmstats_local;
    struct memcg_vmstats_percpu *vmstats_percpu;
    struct memcg_padding _pad2_;
    atomic_long_t vmstats[38];
    atomic_long_t vmevents[85];
    atomic_long_t memory_events[7];
    atomic_long_t memory_events_local[7];
    long unsigned int socket_pressure;
    bool tcpmem_active;
    int tcpmem_pressure;
    int kmemcg_id;
    enum memcg_kmem_state kmem_state;
    struct list_head kmem_caches;
    int last_scanned_node;
    nodemask_t scan_nodes;
    atomic_t numainfo_events;
    atomic_t numainfo_updating;
    struct list_head cgwb_list;
    struct wb_domain cgwb_domain;
    struct memcg_cgwb_frn cgwb_frn[4];
    struct list_head event_list;
    spinlock_t event_list_lock;
    struct deferred_split deferred_split_queue;
    struct mem_cgroup_per_node * nodeinfo[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct mem_cgroup {
    struct cgroup_subsys_state css;
    struct mem_cgroup_id id;
    struct page_counter memory;
    struct page_counter swap;
    struct page_counter memsw;
    struct page_counter kmem;
    struct page_counter tcpmem;
    long unsigned int high;
    struct work_struct high_work;
    long unsigned int soft_limit;
    struct vmpressure vmpressure;
    bool use_hierarchy;
    bool oom_group;
    bool oom_lock;
    int under_oom;
    int swappiness;
    int oom_kill_disable;
    struct cgroup_file events_file;
    struct cgroup_file events_local_file;
    struct cgroup_file swap_events_file;
    struct mutex thresholds_lock;
    struct mem_cgroup_thresholds thresholds;
    struct mem_cgroup_thresholds memsw_thresholds;
    struct list_head oom_notify;
    long unsigned int move_charge_at_immigrate;
    spinlock_t move_lock;
    long unsigned int move_lock_flags;
    struct memcg_padding _pad1_;
    atomic_t moving_account;
    struct task_struct *move_lock_task;
    struct memcg_vmstats_percpu *vmstats_local;
    struct memcg_vmstats_percpu *vmstats_percpu;
    struct memcg_padding _pad2_;
    atomic_long_t vmstats[38];
    atomic_long_t vmevents[85];
    atomic_long_t memory_events[7];
    atomic_long_t memory_events_local[7];
    long unsigned int socket_pressure;
    bool tcpmem_active;
    int tcpmem_pressure;
    int kmemcg_id;
    enum memcg_kmem_state kmem_state;
    struct list_head kmem_caches;
    int last_scanned_node;
    nodemask_t scan_nodes;
    atomic_t numainfo_events;
    atomic_t numainfo_updating;
    struct list_head cgwb_list;
    struct wb_domain cgwb_domain;
    struct memcg_cgwb_frn cgwb_frn[4];
    struct list_head event_list;
    spinlock_t event_list_lock;
    struct deferred_split deferred_split_queue;
    struct mem_cgroup_per_node * nodeinfo[0];
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
<code>struct mem_cgroup_id id</code>
</li>
<li>
<b>Field added. </b>
<code>struct page_counter swap</code>
</li>
<li>
<b>Field added. </b>
<code>struct page_counter tcpmem</code>
</li>
<li>
<b>Field added. </b>
<code>struct work_struct high_work</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int socket_pressure</code>
</li>
<li>
<b>Field added. </b>
<code>bool tcpmem_active</code>
</li>
<li>
<b>Field added. </b>
<code>int tcpmem_pressure</code>
</li>
<li>
<b>Field added. </b>
<code>enum memcg_kmem_state kmem_state</code>
</li>
<li>
<b>Field removed. </b>
<code>int initialized</code>
</li>
<li>
<b>Field removed. </b>
<code>struct cg_proto tcp_mem</code>
</li>
<li>
<b>Field removed. </b>
<code>bool kmem_acct_activated</code>
</li>
<li>
<b>Field removed. </b>
<code>bool kmem_acct_active</code>
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
<code>struct list_head kmem_caches</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct cgroup_file swap_events_file</code>
</li>
<li>
<b>Field added. </b>
<code>struct memcg_padding _pad1_</code>
</li>
<li>
<b>Field added. </b>
<code>struct mem_cgroup_stat_cpu *stat_cpu</code>
</li>
<li>
<b>Field added. </b>
<code>struct memcg_padding _pad2_</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t events[85]</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t memory_events[7]</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int low</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct mem_cgroup_stat_cpu *stat</code> ➡️ <code>atomic_long_t stat[34]</code>
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
<code>bool oom_group</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t stat[34]</code> ➡️ <code>atomic_long_t stat[36]</code>
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
<code>struct cgroup_file events_local_file</code>
</li>
<li>
<b>Field added. </b>
<code>struct memcg_vmstats_percpu *vmstats_local</code>
</li>
<li>
<b>Field added. </b>
<code>struct memcg_vmstats_percpu *vmstats_percpu</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t vmstats[36]</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t vmevents[85]</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t memory_events_local[7]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mem_cgroup_stat_cpu *stat_cpu</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_long_t stat[36]</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_long_t events[85]</code>
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
<code>struct memcg_cgwb_frn cgwb_frn[4]</code>
</li>
<li>
<b>Field added. </b>
<code>struct deferred_split deferred_split_queue</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t vmstats[36]</code> ➡️ <code>atomic_long_t vmstats[38]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>long unsigned int high</code>
</li>
<li>
<b>Field removed. </b>
<code>int last_scanned_node</code>
</li>
<li>
<b>Field removed. </b>
<code>nodemask_t scan_nodes</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t numainfo_events</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t numainfo_updating</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t vmstats[38]</code> ➡️ <code>atomic_long_t vmstats[36]</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t vmevents[85]</code> ➡️ <code>atomic_long_t vmevents[92]</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t memory_events[7]</code> ➡️ <code>atomic_long_t memory_events[8]</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t memory_events_local[7]</code> ➡️ <code>atomic_long_t memory_events_local[8]</code>
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
<code>struct obj_cgroup *objcg</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head objcg_list</code>
</li>
<li>
<b>Field removed. </b>
<code>bool use_hierarchy</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head kmem_caches</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t vmstats[36]</code> ➡️ <code>atomic_long_t vmstats[41]</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t vmevents[92]</code> ➡️ <code>atomic_long_t vmevents[96]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>atomic_long_t vmevents[96]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct memcg_vmstats_percpu *vmstats_local</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t vmstats[41]</code> ➡️ <code>struct memcg_vmstats vmstats</code>
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
<code>long unsigned int zswap_max</code>
</li>
<li>
<b>Field removed. </b>
<code>enum memcg_kmem_state kmem_state</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t memory_events[8]</code> ➡️ <code>atomic_long_t memory_events[9]</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t memory_events_local[8]</code> ➡️ <code>atomic_long_t memory_events_local[9]</code>
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
<code>struct lru_gen_mm_list mm_list</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct memcg_padding _pad1_</code> ➡️ <code>struct cacheline_padding _pad1_</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct memcg_vmstats vmstats</code> ➡️ <code>struct memcg_vmstats *vmstats</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct memcg_padding _pad2_</code> ➡️ <code>struct cacheline_padding _pad2_</code>
</li>
</ul>
</details>
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
<code>bool zswap_writeback</code>
</li>
<li>
<b>Field added. </b>
<code>struct obj_cgroup *orig_objcg</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>arm64</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>atomic_long_t vmevents[85]</code> ➡️ <code>atomic_long_t vmevents[81]</code>
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
<code>nodemask_t scan_nodes</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t numainfo_events</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t numainfo_updating</code>
</li>
<li>
<b>Field removed. </b>
<code>struct deferred_split deferred_split_queue</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t vmevents[85]</code> ➡️ <code>atomic_long_t vmevents[59]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>atomic_long_t vmevents[85]</code> ➡️ <code>atomic_long_t vmevents[78]</code>
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
<code>nodemask_t scan_nodes</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t numainfo_events</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t numainfo_updating</code>
</li>
<li>
<b>Field removed. </b>
<code>struct deferred_split deferred_split_queue</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t vmevents[85]</code> ➡️ <code>atomic_long_t vmevents[61]</code>
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
