# Struct: <code>pmu</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct pmu {
    struct list_head entry;
    struct module *module;
    struct device *dev;
    const struct attribute_group **attr_groups;
    const char *name;
    int type;
    int capabilities;
    int *pmu_disable_count;
    struct perf_cpu_context *pmu_cpu_context;
    atomic_t exclusive_cnt;
    int task_ctx_nr;
    int hrtimer_interval_ms;
    void (*pmu_enable)(struct pmu *);
    void (*pmu_disable)(struct pmu *);
    int (*event_init)(struct perf_event *);
    void (*event_mapped)(struct perf_event *);
    void (*event_unmapped)(struct perf_event *);
    int (*add)(struct perf_event *, int);
    void (*del)(struct perf_event *, int);
    void (*start)(struct perf_event *, int);
    void (*stop)(struct perf_event *, int);
    void (*read)(struct perf_event *);
    void (*start_txn)(struct pmu *, unsigned int);
    int (*commit_txn)(struct pmu *);
    void (*cancel_txn)(struct pmu *);
    int (*event_idx)(struct perf_event *);
    void (*sched_task)(struct perf_event_context *, bool);
    size_t task_ctx_size;
    u64 (*count)(struct perf_event *);
    void * (*setup_aux)(int, void **, int, bool);
    void (*free_aux)(void *);
    int (*filter_match)(struct perf_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct pmu {
    struct list_head entry;
    struct module *module;
    struct device *dev;
    const struct attribute_group **attr_groups;
    const char *name;
    int type;
    int capabilities;
    int *pmu_disable_count;
    struct perf_cpu_context *pmu_cpu_context;
    atomic_t exclusive_cnt;
    int task_ctx_nr;
    int hrtimer_interval_ms;
    unsigned int nr_addr_filters;
    void (*pmu_enable)(struct pmu *);
    void (*pmu_disable)(struct pmu *);
    int (*event_init)(struct perf_event *);
    void (*event_mapped)(struct perf_event *);
    void (*event_unmapped)(struct perf_event *);
    int (*add)(struct perf_event *, int);
    void (*del)(struct perf_event *, int);
    void (*start)(struct perf_event *, int);
    void (*stop)(struct perf_event *, int);
    void (*read)(struct perf_event *);
    void (*start_txn)(struct pmu *, unsigned int);
    int (*commit_txn)(struct pmu *);
    void (*cancel_txn)(struct pmu *);
    int (*event_idx)(struct perf_event *);
    void (*sched_task)(struct perf_event_context *, bool);
    size_t task_ctx_size;
    u64 (*count)(struct perf_event *);
    void * (*setup_aux)(int, void **, int, bool);
    void (*free_aux)(void *);
    int (*addr_filters_validate)(struct list_head *);
    void (*addr_filters_sync)(struct perf_event *);
    int (*filter_match)(struct perf_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct pmu {
    struct list_head entry;
    struct module *module;
    struct device *dev;
    const struct attribute_group **attr_groups;
    const char *name;
    int type;
    int capabilities;
    int *pmu_disable_count;
    struct perf_cpu_context *pmu_cpu_context;
    atomic_t exclusive_cnt;
    int task_ctx_nr;
    int hrtimer_interval_ms;
    unsigned int nr_addr_filters;
    void (*pmu_enable)(struct pmu *);
    void (*pmu_disable)(struct pmu *);
    int (*event_init)(struct perf_event *);
    void (*event_mapped)(struct perf_event *);
    void (*event_unmapped)(struct perf_event *);
    int (*add)(struct perf_event *, int);
    void (*del)(struct perf_event *, int);
    void (*start)(struct perf_event *, int);
    void (*stop)(struct perf_event *, int);
    void (*read)(struct perf_event *);
    void (*start_txn)(struct pmu *, unsigned int);
    int (*commit_txn)(struct pmu *);
    void (*cancel_txn)(struct pmu *);
    int (*event_idx)(struct perf_event *);
    void (*sched_task)(struct perf_event_context *, bool);
    size_t task_ctx_size;
    u64 (*count)(struct perf_event *);
    void * (*setup_aux)(int, void **, int, bool);
    void (*free_aux)(void *);
    int (*addr_filters_validate)(struct list_head *);
    void (*addr_filters_sync)(struct perf_event *);
    int (*filter_match)(struct perf_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct pmu {
    struct list_head entry;
    struct module *module;
    struct device *dev;
    const struct attribute_group **attr_groups;
    const char *name;
    int type;
    int capabilities;
    int *pmu_disable_count;
    struct perf_cpu_context *pmu_cpu_context;
    atomic_t exclusive_cnt;
    int task_ctx_nr;
    int hrtimer_interval_ms;
    unsigned int nr_addr_filters;
    void (*pmu_enable)(struct pmu *);
    void (*pmu_disable)(struct pmu *);
    int (*event_init)(struct perf_event *);
    void (*event_mapped)(struct perf_event *, struct mm_struct *);
    void (*event_unmapped)(struct perf_event *, struct mm_struct *);
    int (*add)(struct perf_event *, int);
    void (*del)(struct perf_event *, int);
    void (*start)(struct perf_event *, int);
    void (*stop)(struct perf_event *, int);
    void (*read)(struct perf_event *);
    void (*start_txn)(struct pmu *, unsigned int);
    int (*commit_txn)(struct pmu *);
    void (*cancel_txn)(struct pmu *);
    int (*event_idx)(struct perf_event *);
    void (*sched_task)(struct perf_event_context *, bool);
    size_t task_ctx_size;
    void * (*setup_aux)(int, void **, int, bool);
    void (*free_aux)(void *);
    int (*addr_filters_validate)(struct list_head *);
    void (*addr_filters_sync)(struct perf_event *);
    int (*filter_match)(struct perf_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct pmu {
    struct list_head entry;
    struct module *module;
    struct device *dev;
    const struct attribute_group **attr_groups;
    const char *name;
    int type;
    int capabilities;
    int *pmu_disable_count;
    struct perf_cpu_context *pmu_cpu_context;
    atomic_t exclusive_cnt;
    int task_ctx_nr;
    int hrtimer_interval_ms;
    unsigned int nr_addr_filters;
    void (*pmu_enable)(struct pmu *);
    void (*pmu_disable)(struct pmu *);
    int (*event_init)(struct perf_event *);
    void (*event_mapped)(struct perf_event *, struct mm_struct *);
    void (*event_unmapped)(struct perf_event *, struct mm_struct *);
    int (*add)(struct perf_event *, int);
    void (*del)(struct perf_event *, int);
    void (*start)(struct perf_event *, int);
    void (*stop)(struct perf_event *, int);
    void (*read)(struct perf_event *);
    void (*start_txn)(struct pmu *, unsigned int);
    int (*commit_txn)(struct pmu *);
    void (*cancel_txn)(struct pmu *);
    int (*event_idx)(struct perf_event *);
    void (*sched_task)(struct perf_event_context *, bool);
    size_t task_ctx_size;
    void * (*setup_aux)(int, void **, int, bool);
    void (*free_aux)(void *);
    int (*addr_filters_validate)(struct list_head *);
    void (*addr_filters_sync)(struct perf_event *);
    int (*filter_match)(struct perf_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct pmu {
    struct list_head entry;
    struct module *module;
    struct device *dev;
    const struct attribute_group **attr_groups;
    const char *name;
    int type;
    int capabilities;
    int *pmu_disable_count;
    struct perf_cpu_context *pmu_cpu_context;
    atomic_t exclusive_cnt;
    int task_ctx_nr;
    int hrtimer_interval_ms;
    unsigned int nr_addr_filters;
    void (*pmu_enable)(struct pmu *);
    void (*pmu_disable)(struct pmu *);
    int (*event_init)(struct perf_event *);
    void (*event_mapped)(struct perf_event *, struct mm_struct *);
    void (*event_unmapped)(struct perf_event *, struct mm_struct *);
    int (*add)(struct perf_event *, int);
    void (*del)(struct perf_event *, int);
    void (*start)(struct perf_event *, int);
    void (*stop)(struct perf_event *, int);
    void (*read)(struct perf_event *);
    void (*start_txn)(struct pmu *, unsigned int);
    int (*commit_txn)(struct pmu *);
    void (*cancel_txn)(struct pmu *);
    int (*event_idx)(struct perf_event *);
    void (*sched_task)(struct perf_event_context *, bool);
    size_t task_ctx_size;
    void * (*setup_aux)(int, void **, int, bool);
    void (*free_aux)(void *);
    int (*addr_filters_validate)(struct list_head *);
    void (*addr_filters_sync)(struct perf_event *);
    int (*filter_match)(struct perf_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct pmu {
    struct list_head entry;
    struct module *module;
    struct device *dev;
    const struct attribute_group **attr_groups;
    const char *name;
    int type;
    int capabilities;
    int *pmu_disable_count;
    struct perf_cpu_context *pmu_cpu_context;
    atomic_t exclusive_cnt;
    int task_ctx_nr;
    int hrtimer_interval_ms;
    unsigned int nr_addr_filters;
    void (*pmu_enable)(struct pmu *);
    void (*pmu_disable)(struct pmu *);
    int (*event_init)(struct perf_event *);
    void (*event_mapped)(struct perf_event *, struct mm_struct *);
    void (*event_unmapped)(struct perf_event *, struct mm_struct *);
    int (*add)(struct perf_event *, int);
    void (*del)(struct perf_event *, int);
    void (*start)(struct perf_event *, int);
    void (*stop)(struct perf_event *, int);
    void (*read)(struct perf_event *);
    void (*start_txn)(struct pmu *, unsigned int);
    int (*commit_txn)(struct pmu *);
    void (*cancel_txn)(struct pmu *);
    int (*event_idx)(struct perf_event *);
    void (*sched_task)(struct perf_event_context *, bool);
    size_t task_ctx_size;
    void * (*setup_aux)(int, void **, int, bool);
    void (*free_aux)(void *);
    int (*addr_filters_validate)(struct list_head *);
    void (*addr_filters_sync)(struct perf_event *);
    int (*filter_match)(struct perf_event *);
    int (*check_period)(struct perf_event *, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct pmu {
    struct list_head entry;
    struct module *module;
    struct device *dev;
    const struct attribute_group **attr_groups;
    const struct attribute_group **attr_update;
    const char *name;
    int type;
    int capabilities;
    int *pmu_disable_count;
    struct perf_cpu_context *pmu_cpu_context;
    atomic_t exclusive_cnt;
    int task_ctx_nr;
    int hrtimer_interval_ms;
    unsigned int nr_addr_filters;
    void (*pmu_enable)(struct pmu *);
    void (*pmu_disable)(struct pmu *);
    int (*event_init)(struct perf_event *);
    void (*event_mapped)(struct perf_event *, struct mm_struct *);
    void (*event_unmapped)(struct perf_event *, struct mm_struct *);
    int (*add)(struct perf_event *, int);
    void (*del)(struct perf_event *, int);
    void (*start)(struct perf_event *, int);
    void (*stop)(struct perf_event *, int);
    void (*read)(struct perf_event *);
    void (*start_txn)(struct pmu *, unsigned int);
    int (*commit_txn)(struct pmu *);
    void (*cancel_txn)(struct pmu *);
    int (*event_idx)(struct perf_event *);
    void (*sched_task)(struct perf_event_context *, bool);
    size_t task_ctx_size;
    void * (*setup_aux)(struct perf_event *, void **, int, bool);
    void (*free_aux)(void *);
    int (*addr_filters_validate)(struct list_head *);
    void (*addr_filters_sync)(struct perf_event *);
    int (*filter_match)(struct perf_event *);
    int (*check_period)(struct perf_event *, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct pmu {
    struct list_head entry;
    struct module *module;
    struct device *dev;
    const struct attribute_group **attr_groups;
    const struct attribute_group **attr_update;
    const char *name;
    int type;
    int capabilities;
    int *pmu_disable_count;
    struct perf_cpu_context *pmu_cpu_context;
    atomic_t exclusive_cnt;
    int task_ctx_nr;
    int hrtimer_interval_ms;
    unsigned int nr_addr_filters;
    void (*pmu_enable)(struct pmu *);
    void (*pmu_disable)(struct pmu *);
    int (*event_init)(struct perf_event *);
    void (*event_mapped)(struct perf_event *, struct mm_struct *);
    void (*event_unmapped)(struct perf_event *, struct mm_struct *);
    int (*add)(struct perf_event *, int);
    void (*del)(struct perf_event *, int);
    void (*start)(struct perf_event *, int);
    void (*stop)(struct perf_event *, int);
    void (*read)(struct perf_event *);
    void (*start_txn)(struct pmu *, unsigned int);
    int (*commit_txn)(struct pmu *);
    void (*cancel_txn)(struct pmu *);
    int (*event_idx)(struct perf_event *);
    void (*sched_task)(struct perf_event_context *, bool);
    size_t task_ctx_size;
    void * (*setup_aux)(struct perf_event *, void **, int, bool);
    void (*free_aux)(void *);
    int (*addr_filters_validate)(struct list_head *);
    void (*addr_filters_sync)(struct perf_event *);
    int (*aux_output_match)(struct perf_event *);
    int (*filter_match)(struct perf_event *);
    int (*check_period)(struct perf_event *, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct pmu {
    struct list_head entry;
    struct module *module;
    struct device *dev;
    const struct attribute_group **attr_groups;
    const struct attribute_group **attr_update;
    const char *name;
    int type;
    int capabilities;
    int *pmu_disable_count;
    struct perf_cpu_context *pmu_cpu_context;
    atomic_t exclusive_cnt;
    int task_ctx_nr;
    int hrtimer_interval_ms;
    unsigned int nr_addr_filters;
    void (*pmu_enable)(struct pmu *);
    void (*pmu_disable)(struct pmu *);
    int (*event_init)(struct perf_event *);
    void (*event_mapped)(struct perf_event *, struct mm_struct *);
    void (*event_unmapped)(struct perf_event *, struct mm_struct *);
    int (*add)(struct perf_event *, int);
    void (*del)(struct perf_event *, int);
    void (*start)(struct perf_event *, int);
    void (*stop)(struct perf_event *, int);
    void (*read)(struct perf_event *);
    void (*start_txn)(struct pmu *, unsigned int);
    int (*commit_txn)(struct pmu *);
    void (*cancel_txn)(struct pmu *);
    int (*event_idx)(struct perf_event *);
    void (*sched_task)(struct perf_event_context *, bool);
    size_t task_ctx_size;
    void (*swap_task_ctx)(struct perf_event_context *, struct perf_event_context *);
    void * (*setup_aux)(struct perf_event *, void **, int, bool);
    void (*free_aux)(void *);
    long int (*snapshot_aux)(struct perf_event *, struct perf_output_handle *, long unsigned int);
    int (*addr_filters_validate)(struct list_head *);
    void (*addr_filters_sync)(struct perf_event *);
    int (*aux_output_match)(struct perf_event *);
    int (*filter_match)(struct perf_event *);
    int (*check_period)(struct perf_event *, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct pmu {
    struct list_head entry;
    struct module *module;
    struct device *dev;
    const struct attribute_group **attr_groups;
    const struct attribute_group **attr_update;
    const char *name;
    int type;
    int capabilities;
    int *pmu_disable_count;
    struct perf_cpu_context *pmu_cpu_context;
    atomic_t exclusive_cnt;
    int task_ctx_nr;
    int hrtimer_interval_ms;
    unsigned int nr_addr_filters;
    void (*pmu_enable)(struct pmu *);
    void (*pmu_disable)(struct pmu *);
    int (*event_init)(struct perf_event *);
    void (*event_mapped)(struct perf_event *, struct mm_struct *);
    void (*event_unmapped)(struct perf_event *, struct mm_struct *);
    int (*add)(struct perf_event *, int);
    void (*del)(struct perf_event *, int);
    void (*start)(struct perf_event *, int);
    void (*stop)(struct perf_event *, int);
    void (*read)(struct perf_event *);
    void (*start_txn)(struct pmu *, unsigned int);
    int (*commit_txn)(struct pmu *);
    void (*cancel_txn)(struct pmu *);
    int (*event_idx)(struct perf_event *);
    void (*sched_task)(struct perf_event_context *, bool);
    struct kmem_cache *task_ctx_cache;
    void (*swap_task_ctx)(struct perf_event_context *, struct perf_event_context *);
    void * (*setup_aux)(struct perf_event *, void **, int, bool);
    void (*free_aux)(void *);
    long int (*snapshot_aux)(struct perf_event *, struct perf_output_handle *, long unsigned int);
    int (*addr_filters_validate)(struct list_head *);
    void (*addr_filters_sync)(struct perf_event *);
    int (*aux_output_match)(struct perf_event *);
    int (*filter_match)(struct perf_event *);
    int (*check_period)(struct perf_event *, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct pmu {
    struct list_head entry;
    struct module *module;
    struct device *dev;
    const struct attribute_group **attr_groups;
    const struct attribute_group **attr_update;
    const char *name;
    int type;
    int capabilities;
    int *pmu_disable_count;
    struct perf_cpu_context *pmu_cpu_context;
    atomic_t exclusive_cnt;
    int task_ctx_nr;
    int hrtimer_interval_ms;
    unsigned int nr_addr_filters;
    void (*pmu_enable)(struct pmu *);
    void (*pmu_disable)(struct pmu *);
    int (*event_init)(struct perf_event *);
    void (*event_mapped)(struct perf_event *, struct mm_struct *);
    void (*event_unmapped)(struct perf_event *, struct mm_struct *);
    int (*add)(struct perf_event *, int);
    void (*del)(struct perf_event *, int);
    void (*start)(struct perf_event *, int);
    void (*stop)(struct perf_event *, int);
    void (*read)(struct perf_event *);
    void (*start_txn)(struct pmu *, unsigned int);
    int (*commit_txn)(struct pmu *);
    void (*cancel_txn)(struct pmu *);
    int (*event_idx)(struct perf_event *);
    void (*sched_task)(struct perf_event_context *, bool);
    struct kmem_cache *task_ctx_cache;
    void (*swap_task_ctx)(struct perf_event_context *, struct perf_event_context *);
    void * (*setup_aux)(struct perf_event *, void **, int, bool);
    void (*free_aux)(void *);
    long int (*snapshot_aux)(struct perf_event *, struct perf_output_handle *, long unsigned int);
    int (*addr_filters_validate)(struct list_head *);
    void (*addr_filters_sync)(struct perf_event *);
    int (*aux_output_match)(struct perf_event *);
    int (*filter_match)(struct perf_event *);
    int (*check_period)(struct perf_event *, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct pmu {
    struct list_head entry;
    struct module *module;
    struct device *dev;
    const struct attribute_group **attr_groups;
    const struct attribute_group **attr_update;
    const char *name;
    int type;
    int capabilities;
    int *pmu_disable_count;
    struct perf_cpu_context *pmu_cpu_context;
    atomic_t exclusive_cnt;
    int task_ctx_nr;
    int hrtimer_interval_ms;
    unsigned int nr_addr_filters;
    void (*pmu_enable)(struct pmu *);
    void (*pmu_disable)(struct pmu *);
    int (*event_init)(struct perf_event *);
    void (*event_mapped)(struct perf_event *, struct mm_struct *);
    void (*event_unmapped)(struct perf_event *, struct mm_struct *);
    int (*add)(struct perf_event *, int);
    void (*del)(struct perf_event *, int);
    void (*start)(struct perf_event *, int);
    void (*stop)(struct perf_event *, int);
    void (*read)(struct perf_event *);
    void (*start_txn)(struct pmu *, unsigned int);
    int (*commit_txn)(struct pmu *);
    void (*cancel_txn)(struct pmu *);
    int (*event_idx)(struct perf_event *);
    void (*sched_task)(struct perf_event_context *, bool);
    struct kmem_cache *task_ctx_cache;
    void (*swap_task_ctx)(struct perf_event_context *, struct perf_event_context *);
    void * (*setup_aux)(struct perf_event *, void **, int, bool);
    void (*free_aux)(void *);
    long int (*snapshot_aux)(struct perf_event *, struct perf_output_handle *, long unsigned int);
    int (*addr_filters_validate)(struct list_head *);
    void (*addr_filters_sync)(struct perf_event *);
    int (*aux_output_match)(struct perf_event *);
    int (*filter_match)(struct perf_event *);
    int (*check_period)(struct perf_event *, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct pmu {
    struct list_head entry;
    struct module *module;
    struct device *dev;
    const struct attribute_group **attr_groups;
    const struct attribute_group **attr_update;
    const char *name;
    int type;
    int capabilities;
    int *pmu_disable_count;
    struct perf_cpu_context *pmu_cpu_context;
    atomic_t exclusive_cnt;
    int task_ctx_nr;
    int hrtimer_interval_ms;
    unsigned int nr_addr_filters;
    void (*pmu_enable)(struct pmu *);
    void (*pmu_disable)(struct pmu *);
    int (*event_init)(struct perf_event *);
    void (*event_mapped)(struct perf_event *, struct mm_struct *);
    void (*event_unmapped)(struct perf_event *, struct mm_struct *);
    int (*add)(struct perf_event *, int);
    void (*del)(struct perf_event *, int);
    void (*start)(struct perf_event *, int);
    void (*stop)(struct perf_event *, int);
    void (*read)(struct perf_event *);
    void (*start_txn)(struct pmu *, unsigned int);
    int (*commit_txn)(struct pmu *);
    void (*cancel_txn)(struct pmu *);
    int (*event_idx)(struct perf_event *);
    void (*sched_task)(struct perf_event_context *, bool);
    struct kmem_cache *task_ctx_cache;
    void (*swap_task_ctx)(struct perf_event_context *, struct perf_event_context *);
    void * (*setup_aux)(struct perf_event *, void **, int, bool);
    void (*free_aux)(void *);
    long int (*snapshot_aux)(struct perf_event *, struct perf_output_handle *, long unsigned int);
    int (*addr_filters_validate)(struct list_head *);
    void (*addr_filters_sync)(struct perf_event *);
    int (*aux_output_match)(struct perf_event *);
    int (*filter_match)(struct perf_event *);
    int (*check_period)(struct perf_event *, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct pmu {
    struct list_head entry;
    struct module *module;
    struct device *dev;
    const struct attribute_group **attr_groups;
    const struct attribute_group **attr_update;
    const char *name;
    int type;
    int capabilities;
    int *pmu_disable_count;
    struct perf_cpu_pmu_context *cpu_pmu_context;
    atomic_t exclusive_cnt;
    int task_ctx_nr;
    int hrtimer_interval_ms;
    unsigned int nr_addr_filters;
    void (*pmu_enable)(struct pmu *);
    void (*pmu_disable)(struct pmu *);
    int (*event_init)(struct perf_event *);
    void (*event_mapped)(struct perf_event *, struct mm_struct *);
    void (*event_unmapped)(struct perf_event *, struct mm_struct *);
    int (*add)(struct perf_event *, int);
    void (*del)(struct perf_event *, int);
    void (*start)(struct perf_event *, int);
    void (*stop)(struct perf_event *, int);
    void (*read)(struct perf_event *);
    void (*start_txn)(struct pmu *, unsigned int);
    int (*commit_txn)(struct pmu *);
    void (*cancel_txn)(struct pmu *);
    int (*event_idx)(struct perf_event *);
    void (*sched_task)(struct perf_event_pmu_context *, bool);
    struct kmem_cache *task_ctx_cache;
    void (*swap_task_ctx)(struct perf_event_pmu_context *, struct perf_event_pmu_context *);
    void * (*setup_aux)(struct perf_event *, void **, int, bool);
    void (*free_aux)(void *);
    long int (*snapshot_aux)(struct perf_event *, struct perf_output_handle *, long unsigned int);
    int (*addr_filters_validate)(struct list_head *);
    void (*addr_filters_sync)(struct perf_event *);
    int (*aux_output_match)(struct perf_event *);
    bool (*filter)(struct pmu *, int);
    int (*check_period)(struct perf_event *, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct pmu {
    struct list_head entry;
    struct module *module;
    struct device *dev;
    struct device *parent;
    const struct attribute_group **attr_groups;
    const struct attribute_group **attr_update;
    const char *name;
    int type;
    int capabilities;
    int *pmu_disable_count;
    struct perf_cpu_pmu_context *cpu_pmu_context;
    atomic_t exclusive_cnt;
    int task_ctx_nr;
    int hrtimer_interval_ms;
    unsigned int nr_addr_filters;
    void (*pmu_enable)(struct pmu *);
    void (*pmu_disable)(struct pmu *);
    int (*event_init)(struct perf_event *);
    void (*event_mapped)(struct perf_event *, struct mm_struct *);
    void (*event_unmapped)(struct perf_event *, struct mm_struct *);
    int (*add)(struct perf_event *, int);
    void (*del)(struct perf_event *, int);
    void (*start)(struct perf_event *, int);
    void (*stop)(struct perf_event *, int);
    void (*read)(struct perf_event *);
    void (*start_txn)(struct pmu *, unsigned int);
    int (*commit_txn)(struct pmu *);
    void (*cancel_txn)(struct pmu *);
    int (*event_idx)(struct perf_event *);
    void (*sched_task)(struct perf_event_pmu_context *, bool);
    struct kmem_cache *task_ctx_cache;
    void (*swap_task_ctx)(struct perf_event_pmu_context *, struct perf_event_pmu_context *);
    void * (*setup_aux)(struct perf_event *, void **, int, bool);
    void (*free_aux)(void *);
    long int (*snapshot_aux)(struct perf_event *, struct perf_output_handle *, long unsigned int);
    int (*addr_filters_validate)(struct list_head *);
    void (*addr_filters_sync)(struct perf_event *);
    int (*aux_output_match)(struct perf_event *);
    bool (*filter)(struct pmu *, int);
    int (*check_period)(struct perf_event *, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct pmu {
    struct list_head entry;
    struct module *module;
    struct device *dev;
    struct device *parent;
    const struct attribute_group **attr_groups;
    const struct attribute_group **attr_update;
    const char *name;
    int type;
    int capabilities;
    int *pmu_disable_count;
    struct perf_cpu_pmu_context *cpu_pmu_context;
    atomic_t exclusive_cnt;
    int task_ctx_nr;
    int hrtimer_interval_ms;
    unsigned int nr_addr_filters;
    void (*pmu_enable)(struct pmu *);
    void (*pmu_disable)(struct pmu *);
    int (*event_init)(struct perf_event *);
    void (*event_mapped)(struct perf_event *, struct mm_struct *);
    void (*event_unmapped)(struct perf_event *, struct mm_struct *);
    int (*add)(struct perf_event *, int);
    void (*del)(struct perf_event *, int);
    void (*start)(struct perf_event *, int);
    void (*stop)(struct perf_event *, int);
    void (*read)(struct perf_event *);
    void (*start_txn)(struct pmu *, unsigned int);
    int (*commit_txn)(struct pmu *);
    void (*cancel_txn)(struct pmu *);
    int (*event_idx)(struct perf_event *);
    void (*sched_task)(struct perf_event_pmu_context *, bool);
    struct kmem_cache *task_ctx_cache;
    void (*swap_task_ctx)(struct perf_event_pmu_context *, struct perf_event_pmu_context *);
    void * (*setup_aux)(struct perf_event *, void **, int, bool);
    void (*free_aux)(void *);
    long int (*snapshot_aux)(struct perf_event *, struct perf_output_handle *, long unsigned int);
    int (*addr_filters_validate)(struct list_head *);
    void (*addr_filters_sync)(struct perf_event *);
    int (*aux_output_match)(struct perf_event *);
    bool (*filter)(struct pmu *, int);
    int (*check_period)(struct perf_event *, u64);
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
struct pmu {
    struct list_head entry;
    struct module *module;
    struct device *dev;
    const struct attribute_group **attr_groups;
    const struct attribute_group **attr_update;
    const char *name;
    int type;
    int capabilities;
    int *pmu_disable_count;
    struct perf_cpu_context *pmu_cpu_context;
    atomic_t exclusive_cnt;
    int task_ctx_nr;
    int hrtimer_interval_ms;
    unsigned int nr_addr_filters;
    void (*pmu_enable)(struct pmu *);
    void (*pmu_disable)(struct pmu *);
    int (*event_init)(struct perf_event *);
    void (*event_mapped)(struct perf_event *, struct mm_struct *);
    void (*event_unmapped)(struct perf_event *, struct mm_struct *);
    int (*add)(struct perf_event *, int);
    void (*del)(struct perf_event *, int);
    void (*start)(struct perf_event *, int);
    void (*stop)(struct perf_event *, int);
    void (*read)(struct perf_event *);
    void (*start_txn)(struct pmu *, unsigned int);
    int (*commit_txn)(struct pmu *);
    void (*cancel_txn)(struct pmu *);
    int (*event_idx)(struct perf_event *);
    void (*sched_task)(struct perf_event_context *, bool);
    size_t task_ctx_size;
    void * (*setup_aux)(struct perf_event *, void **, int, bool);
    void (*free_aux)(void *);
    int (*addr_filters_validate)(struct list_head *);
    void (*addr_filters_sync)(struct perf_event *);
    int (*aux_output_match)(struct perf_event *);
    int (*filter_match)(struct perf_event *);
    int (*check_period)(struct perf_event *, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct pmu {
    struct list_head entry;
    struct module *module;
    struct device *dev;
    const struct attribute_group **attr_groups;
    const struct attribute_group **attr_update;
    const char *name;
    int type;
    int capabilities;
    int *pmu_disable_count;
    struct perf_cpu_context *pmu_cpu_context;
    atomic_t exclusive_cnt;
    int task_ctx_nr;
    int hrtimer_interval_ms;
    unsigned int nr_addr_filters;
    void (*pmu_enable)(struct pmu *);
    void (*pmu_disable)(struct pmu *);
    int (*event_init)(struct perf_event *);
    void (*event_mapped)(struct perf_event *, struct mm_struct *);
    void (*event_unmapped)(struct perf_event *, struct mm_struct *);
    int (*add)(struct perf_event *, int);
    void (*del)(struct perf_event *, int);
    void (*start)(struct perf_event *, int);
    void (*stop)(struct perf_event *, int);
    void (*read)(struct perf_event *);
    void (*start_txn)(struct pmu *, unsigned int);
    int (*commit_txn)(struct pmu *);
    void (*cancel_txn)(struct pmu *);
    int (*event_idx)(struct perf_event *);
    void (*sched_task)(struct perf_event_context *, bool);
    size_t task_ctx_size;
    void * (*setup_aux)(struct perf_event *, void **, int, bool);
    void (*free_aux)(void *);
    int (*addr_filters_validate)(struct list_head *);
    void (*addr_filters_sync)(struct perf_event *);
    int (*aux_output_match)(struct perf_event *);
    int (*filter_match)(struct perf_event *);
    int (*check_period)(struct perf_event *, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct pmu {
    struct list_head entry;
    struct module *module;
    struct device *dev;
    const struct attribute_group **attr_groups;
    const struct attribute_group **attr_update;
    const char *name;
    int type;
    int capabilities;
    int *pmu_disable_count;
    struct perf_cpu_context *pmu_cpu_context;
    atomic_t exclusive_cnt;
    int task_ctx_nr;
    int hrtimer_interval_ms;
    unsigned int nr_addr_filters;
    void (*pmu_enable)(struct pmu *);
    void (*pmu_disable)(struct pmu *);
    int (*event_init)(struct perf_event *);
    void (*event_mapped)(struct perf_event *, struct mm_struct *);
    void (*event_unmapped)(struct perf_event *, struct mm_struct *);
    int (*add)(struct perf_event *, int);
    void (*del)(struct perf_event *, int);
    void (*start)(struct perf_event *, int);
    void (*stop)(struct perf_event *, int);
    void (*read)(struct perf_event *);
    void (*start_txn)(struct pmu *, unsigned int);
    int (*commit_txn)(struct pmu *);
    void (*cancel_txn)(struct pmu *);
    int (*event_idx)(struct perf_event *);
    void (*sched_task)(struct perf_event_context *, bool);
    size_t task_ctx_size;
    void * (*setup_aux)(struct perf_event *, void **, int, bool);
    void (*free_aux)(void *);
    int (*addr_filters_validate)(struct list_head *);
    void (*addr_filters_sync)(struct perf_event *);
    int (*aux_output_match)(struct perf_event *);
    int (*filter_match)(struct perf_event *);
    int (*check_period)(struct perf_event *, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct pmu {
    struct list_head entry;
    struct module *module;
    struct device *dev;
    const struct attribute_group **attr_groups;
    const struct attribute_group **attr_update;
    const char *name;
    int type;
    int capabilities;
    int *pmu_disable_count;
    struct perf_cpu_context *pmu_cpu_context;
    atomic_t exclusive_cnt;
    int task_ctx_nr;
    int hrtimer_interval_ms;
    unsigned int nr_addr_filters;
    void (*pmu_enable)(struct pmu *);
    void (*pmu_disable)(struct pmu *);
    int (*event_init)(struct perf_event *);
    void (*event_mapped)(struct perf_event *, struct mm_struct *);
    void (*event_unmapped)(struct perf_event *, struct mm_struct *);
    int (*add)(struct perf_event *, int);
    void (*del)(struct perf_event *, int);
    void (*start)(struct perf_event *, int);
    void (*stop)(struct perf_event *, int);
    void (*read)(struct perf_event *);
    void (*start_txn)(struct pmu *, unsigned int);
    int (*commit_txn)(struct pmu *);
    void (*cancel_txn)(struct pmu *);
    int (*event_idx)(struct perf_event *);
    void (*sched_task)(struct perf_event_context *, bool);
    size_t task_ctx_size;
    void * (*setup_aux)(struct perf_event *, void **, int, bool);
    void (*free_aux)(void *);
    int (*addr_filters_validate)(struct list_head *);
    void (*addr_filters_sync)(struct perf_event *);
    int (*aux_output_match)(struct perf_event *);
    int (*filter_match)(struct perf_event *);
    int (*check_period)(struct perf_event *, u64);
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
struct pmu {
    struct list_head entry;
    struct module *module;
    struct device *dev;
    const struct attribute_group **attr_groups;
    const struct attribute_group **attr_update;
    const char *name;
    int type;
    int capabilities;
    int *pmu_disable_count;
    struct perf_cpu_context *pmu_cpu_context;
    atomic_t exclusive_cnt;
    int task_ctx_nr;
    int hrtimer_interval_ms;
    unsigned int nr_addr_filters;
    void (*pmu_enable)(struct pmu *);
    void (*pmu_disable)(struct pmu *);
    int (*event_init)(struct perf_event *);
    void (*event_mapped)(struct perf_event *, struct mm_struct *);
    void (*event_unmapped)(struct perf_event *, struct mm_struct *);
    int (*add)(struct perf_event *, int);
    void (*del)(struct perf_event *, int);
    void (*start)(struct perf_event *, int);
    void (*stop)(struct perf_event *, int);
    void (*read)(struct perf_event *);
    void (*start_txn)(struct pmu *, unsigned int);
    int (*commit_txn)(struct pmu *);
    void (*cancel_txn)(struct pmu *);
    int (*event_idx)(struct perf_event *);
    void (*sched_task)(struct perf_event_context *, bool);
    size_t task_ctx_size;
    void * (*setup_aux)(struct perf_event *, void **, int, bool);
    void (*free_aux)(void *);
    int (*addr_filters_validate)(struct list_head *);
    void (*addr_filters_sync)(struct perf_event *);
    int (*aux_output_match)(struct perf_event *);
    int (*filter_match)(struct perf_event *);
    int (*check_period)(struct perf_event *, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct pmu {
    struct list_head entry;
    struct module *module;
    struct device *dev;
    const struct attribute_group **attr_groups;
    const struct attribute_group **attr_update;
    const char *name;
    int type;
    int capabilities;
    int *pmu_disable_count;
    struct perf_cpu_context *pmu_cpu_context;
    atomic_t exclusive_cnt;
    int task_ctx_nr;
    int hrtimer_interval_ms;
    unsigned int nr_addr_filters;
    void (*pmu_enable)(struct pmu *);
    void (*pmu_disable)(struct pmu *);
    int (*event_init)(struct perf_event *);
    void (*event_mapped)(struct perf_event *, struct mm_struct *);
    void (*event_unmapped)(struct perf_event *, struct mm_struct *);
    int (*add)(struct perf_event *, int);
    void (*del)(struct perf_event *, int);
    void (*start)(struct perf_event *, int);
    void (*stop)(struct perf_event *, int);
    void (*read)(struct perf_event *);
    void (*start_txn)(struct pmu *, unsigned int);
    int (*commit_txn)(struct pmu *);
    void (*cancel_txn)(struct pmu *);
    int (*event_idx)(struct perf_event *);
    void (*sched_task)(struct perf_event_context *, bool);
    size_t task_ctx_size;
    void * (*setup_aux)(struct perf_event *, void **, int, bool);
    void (*free_aux)(void *);
    int (*addr_filters_validate)(struct list_head *);
    void (*addr_filters_sync)(struct perf_event *);
    int (*aux_output_match)(struct perf_event *);
    int (*filter_match)(struct perf_event *);
    int (*check_period)(struct perf_event *, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct pmu {
    struct list_head entry;
    struct module *module;
    struct device *dev;
    const struct attribute_group **attr_groups;
    const struct attribute_group **attr_update;
    const char *name;
    int type;
    int capabilities;
    int *pmu_disable_count;
    struct perf_cpu_context *pmu_cpu_context;
    atomic_t exclusive_cnt;
    int task_ctx_nr;
    int hrtimer_interval_ms;
    unsigned int nr_addr_filters;
    void (*pmu_enable)(struct pmu *);
    void (*pmu_disable)(struct pmu *);
    int (*event_init)(struct perf_event *);
    void (*event_mapped)(struct perf_event *, struct mm_struct *);
    void (*event_unmapped)(struct perf_event *, struct mm_struct *);
    int (*add)(struct perf_event *, int);
    void (*del)(struct perf_event *, int);
    void (*start)(struct perf_event *, int);
    void (*stop)(struct perf_event *, int);
    void (*read)(struct perf_event *);
    void (*start_txn)(struct pmu *, unsigned int);
    int (*commit_txn)(struct pmu *);
    void (*cancel_txn)(struct pmu *);
    int (*event_idx)(struct perf_event *);
    void (*sched_task)(struct perf_event_context *, bool);
    size_t task_ctx_size;
    void * (*setup_aux)(struct perf_event *, void **, int, bool);
    void (*free_aux)(void *);
    int (*addr_filters_validate)(struct list_head *);
    void (*addr_filters_sync)(struct perf_event *);
    int (*aux_output_match)(struct perf_event *);
    int (*filter_match)(struct perf_event *);
    int (*check_period)(struct perf_event *, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct pmu {
    struct list_head entry;
    struct module *module;
    struct device *dev;
    const struct attribute_group **attr_groups;
    const struct attribute_group **attr_update;
    const char *name;
    int type;
    int capabilities;
    int *pmu_disable_count;
    struct perf_cpu_context *pmu_cpu_context;
    atomic_t exclusive_cnt;
    int task_ctx_nr;
    int hrtimer_interval_ms;
    unsigned int nr_addr_filters;
    void (*pmu_enable)(struct pmu *);
    void (*pmu_disable)(struct pmu *);
    int (*event_init)(struct perf_event *);
    void (*event_mapped)(struct perf_event *, struct mm_struct *);
    void (*event_unmapped)(struct perf_event *, struct mm_struct *);
    int (*add)(struct perf_event *, int);
    void (*del)(struct perf_event *, int);
    void (*start)(struct perf_event *, int);
    void (*stop)(struct perf_event *, int);
    void (*read)(struct perf_event *);
    void (*start_txn)(struct pmu *, unsigned int);
    int (*commit_txn)(struct pmu *);
    void (*cancel_txn)(struct pmu *);
    int (*event_idx)(struct perf_event *);
    void (*sched_task)(struct perf_event_context *, bool);
    size_t task_ctx_size;
    void * (*setup_aux)(struct perf_event *, void **, int, bool);
    void (*free_aux)(void *);
    int (*addr_filters_validate)(struct list_head *);
    void (*addr_filters_sync)(struct perf_event *);
    int (*aux_output_match)(struct perf_event *);
    int (*filter_match)(struct perf_event *);
    int (*check_period)(struct perf_event *, u64);
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
<code>unsigned int nr_addr_filters</code>
</li>
<li>
<b>Field added. </b>
<code>int (*addr_filters_validate)(struct list_head *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*addr_filters_sync)(struct perf_event *)</code>
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
<b>Field removed. </b>
<code>u64 (*count)(struct perf_event *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*event_mapped)(struct perf_event *)</code> ➡️ <code>void (*event_mapped)(struct perf_event *, struct mm_struct *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*event_unmapped)(struct perf_event *)</code> ➡️ <code>void (*event_unmapped)(struct perf_event *, struct mm_struct *)</code>
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
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*check_period)(struct perf_event *, u64)</code>
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
<code>const struct attribute_group **attr_update</code>
</li>
<li>
<b>Field type changed. </b>
<code>void * (*setup_aux)(int, void **, int, bool)</code> ➡️ <code>void * (*setup_aux)(struct perf_event *, void **, int, bool)</code>
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
<code>int (*aux_output_match)(struct perf_event *)</code>
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
<code>void (*swap_task_ctx)(struct perf_event_context *, struct perf_event_context *)</code>
</li>
<li>
<b>Field added. </b>
<code>long int (*snapshot_aux)(struct perf_event *, struct perf_output_handle *, long unsigned int)</code>
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
<code>struct kmem_cache *task_ctx_cache</code>
</li>
<li>
<b>Field removed. </b>
<code>size_t task_ctx_size</code>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct perf_cpu_pmu_context *cpu_pmu_context</code>
</li>
<li>
<b>Field added. </b>
<code>bool (*filter)(struct pmu *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct perf_cpu_context *pmu_cpu_context</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*filter_match)(struct perf_event *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*sched_task)(struct perf_event_context *, bool)</code> ➡️ <code>void (*sched_task)(struct perf_event_pmu_context *, bool)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*swap_task_ctx)(struct perf_event_context *, struct perf_event_context *)</code> ➡️ <code>void (*swap_task_ctx)(struct perf_event_pmu_context *, struct perf_event_pmu_context *)</code>
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
<code>struct device *parent</code>
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
