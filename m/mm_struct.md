# Struct: <code>mm_struct</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct mm_struct {
    struct vm_area_struct *mmap;
    struct rb_root mm_rb;
    u32 vmacache_seqnum;
    long unsigned int (*get_unmapped_area)(struct file *, long unsigned int, long unsigned int, long unsigned int, long unsigned int);
    long unsigned int mmap_base;
    long unsigned int mmap_legacy_base;
    long unsigned int task_size;
    long unsigned int highest_vm_end;
    pgd_t *pgd;
    atomic_t mm_users;
    atomic_t mm_count;
    atomic_long_t nr_ptes;
    atomic_long_t nr_pmds;
    int map_count;
    spinlock_t page_table_lock;
    struct rw_semaphore mmap_sem;
    struct list_head mmlist;
    long unsigned int hiwater_rss;
    long unsigned int hiwater_vm;
    long unsigned int total_vm;
    long unsigned int locked_vm;
    long unsigned int pinned_vm;
    long unsigned int shared_vm;
    long unsigned int exec_vm;
    long unsigned int stack_vm;
    long unsigned int def_flags;
    long unsigned int start_code;
    long unsigned int end_code;
    long unsigned int start_data;
    long unsigned int end_data;
    long unsigned int start_brk;
    long unsigned int brk;
    long unsigned int start_stack;
    long unsigned int arg_start;
    long unsigned int arg_end;
    long unsigned int env_start;
    long unsigned int env_end;
    long unsigned int saved_auxv[46];
    struct mm_rss_stat rss_stat;
    struct linux_binfmt *binfmt;
    cpumask_var_t cpu_vm_mask_var;
    mm_context_t context;
    long unsigned int flags;
    struct core_state *core_state;
    spinlock_t ioctx_lock;
    struct kioctx_table *ioctx_table;
    struct task_struct *owner;
    struct file *exe_file;
    struct mmu_notifier_mm *mmu_notifier_mm;
    long unsigned int numa_next_scan;
    long unsigned int numa_scan_offset;
    int numa_scan_seq;
    bool tlb_flush_pending;
    struct uprobes_state uprobes_state;
    void *bd_addr;
    atomic_long_t hugetlb_usage;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct mm_struct {
    struct vm_area_struct *mmap;
    struct rb_root mm_rb;
    u32 vmacache_seqnum;
    long unsigned int (*get_unmapped_area)(struct file *, long unsigned int, long unsigned int, long unsigned int, long unsigned int);
    long unsigned int mmap_base;
    long unsigned int mmap_legacy_base;
    long unsigned int task_size;
    long unsigned int highest_vm_end;
    pgd_t *pgd;
    atomic_t mm_users;
    atomic_t mm_count;
    atomic_long_t nr_ptes;
    atomic_long_t nr_pmds;
    int map_count;
    spinlock_t page_table_lock;
    struct rw_semaphore mmap_sem;
    struct list_head mmlist;
    long unsigned int hiwater_rss;
    long unsigned int hiwater_vm;
    long unsigned int total_vm;
    long unsigned int locked_vm;
    long unsigned int pinned_vm;
    long unsigned int data_vm;
    long unsigned int exec_vm;
    long unsigned int stack_vm;
    long unsigned int def_flags;
    long unsigned int start_code;
    long unsigned int end_code;
    long unsigned int start_data;
    long unsigned int end_data;
    long unsigned int start_brk;
    long unsigned int brk;
    long unsigned int start_stack;
    long unsigned int arg_start;
    long unsigned int arg_end;
    long unsigned int env_start;
    long unsigned int env_end;
    long unsigned int saved_auxv[46];
    struct mm_rss_stat rss_stat;
    struct linux_binfmt *binfmt;
    cpumask_var_t cpu_vm_mask_var;
    mm_context_t context;
    long unsigned int flags;
    struct core_state *core_state;
    spinlock_t ioctx_lock;
    struct kioctx_table *ioctx_table;
    struct task_struct *owner;
    struct file *exe_file;
    struct mmu_notifier_mm *mmu_notifier_mm;
    long unsigned int numa_next_scan;
    long unsigned int numa_scan_offset;
    int numa_scan_seq;
    bool tlb_flush_pending;
    struct uprobes_state uprobes_state;
    void *bd_addr;
    atomic_long_t hugetlb_usage;
    struct work_struct async_put_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct mm_struct {
    struct vm_area_struct *mmap;
    struct rb_root mm_rb;
    u32 vmacache_seqnum;
    long unsigned int (*get_unmapped_area)(struct file *, long unsigned int, long unsigned int, long unsigned int, long unsigned int);
    long unsigned int mmap_base;
    long unsigned int mmap_legacy_base;
    long unsigned int task_size;
    long unsigned int highest_vm_end;
    pgd_t *pgd;
    atomic_t mm_users;
    atomic_t mm_count;
    atomic_long_t nr_ptes;
    atomic_long_t nr_pmds;
    int map_count;
    spinlock_t page_table_lock;
    struct rw_semaphore mmap_sem;
    struct list_head mmlist;
    long unsigned int hiwater_rss;
    long unsigned int hiwater_vm;
    long unsigned int total_vm;
    long unsigned int locked_vm;
    long unsigned int pinned_vm;
    long unsigned int data_vm;
    long unsigned int exec_vm;
    long unsigned int stack_vm;
    long unsigned int def_flags;
    long unsigned int start_code;
    long unsigned int end_code;
    long unsigned int start_data;
    long unsigned int end_data;
    long unsigned int start_brk;
    long unsigned int brk;
    long unsigned int start_stack;
    long unsigned int arg_start;
    long unsigned int arg_end;
    long unsigned int env_start;
    long unsigned int env_end;
    long unsigned int saved_auxv[46];
    struct mm_rss_stat rss_stat;
    struct linux_binfmt *binfmt;
    cpumask_var_t cpu_vm_mask_var;
    mm_context_t context;
    long unsigned int flags;
    struct core_state *core_state;
    spinlock_t ioctx_lock;
    struct kioctx_table *ioctx_table;
    struct task_struct *owner;
    struct user_namespace *user_ns;
    struct file *exe_file;
    struct mmu_notifier_mm *mmu_notifier_mm;
    struct cpumask cpumask_allocation;
    long unsigned int numa_next_scan;
    long unsigned int numa_scan_offset;
    int numa_scan_seq;
    bool tlb_flush_pending;
    struct uprobes_state uprobes_state;
    atomic_long_t hugetlb_usage;
    struct work_struct async_put_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct mm_struct {
    struct vm_area_struct *mmap;
    struct rb_root mm_rb;
    u32 vmacache_seqnum;
    long unsigned int (*get_unmapped_area)(struct file *, long unsigned int, long unsigned int, long unsigned int, long unsigned int);
    long unsigned int mmap_base;
    long unsigned int mmap_legacy_base;
    long unsigned int mmap_compat_base;
    long unsigned int mmap_compat_legacy_base;
    long unsigned int task_size;
    long unsigned int highest_vm_end;
    pgd_t *pgd;
    atomic_t mm_users;
    atomic_t mm_count;
    atomic_long_t nr_ptes;
    atomic_long_t nr_pmds;
    int map_count;
    spinlock_t page_table_lock;
    struct rw_semaphore mmap_sem;
    struct list_head mmlist;
    long unsigned int hiwater_rss;
    long unsigned int hiwater_vm;
    long unsigned int total_vm;
    long unsigned int locked_vm;
    long unsigned int pinned_vm;
    long unsigned int data_vm;
    long unsigned int exec_vm;
    long unsigned int stack_vm;
    long unsigned int def_flags;
    long unsigned int start_code;
    long unsigned int end_code;
    long unsigned int start_data;
    long unsigned int end_data;
    long unsigned int start_brk;
    long unsigned int brk;
    long unsigned int start_stack;
    long unsigned int arg_start;
    long unsigned int arg_end;
    long unsigned int env_start;
    long unsigned int env_end;
    long unsigned int saved_auxv[46];
    struct mm_rss_stat rss_stat;
    struct linux_binfmt *binfmt;
    cpumask_var_t cpu_vm_mask_var;
    mm_context_t context;
    long unsigned int flags;
    struct core_state *core_state;
    spinlock_t ioctx_lock;
    struct kioctx_table *ioctx_table;
    struct task_struct *owner;
    struct user_namespace *user_ns;
    struct file *exe_file;
    struct mmu_notifier_mm *mmu_notifier_mm;
    struct cpumask cpumask_allocation;
    long unsigned int numa_next_scan;
    long unsigned int numa_scan_offset;
    int numa_scan_seq;
    atomic_t tlb_flush_pending;
    bool tlb_flush_batched;
    struct uprobes_state uprobes_state;
    atomic_long_t hugetlb_usage;
    struct work_struct async_put_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct mm_struct {
    struct vm_area_struct *mmap;
    struct rb_root mm_rb;
    u32 vmacache_seqnum;
    long unsigned int (*get_unmapped_area)(struct file *, long unsigned int, long unsigned int, long unsigned int, long unsigned int);
    long unsigned int mmap_base;
    long unsigned int mmap_legacy_base;
    long unsigned int mmap_compat_base;
    long unsigned int mmap_compat_legacy_base;
    long unsigned int task_size;
    long unsigned int highest_vm_end;
    pgd_t *pgd;
    atomic_t mm_users;
    atomic_t mm_count;
    atomic_long_t pgtables_bytes;
    int map_count;
    spinlock_t page_table_lock;
    struct rw_semaphore mmap_sem;
    struct list_head mmlist;
    long unsigned int hiwater_rss;
    long unsigned int hiwater_vm;
    long unsigned int total_vm;
    long unsigned int locked_vm;
    long unsigned int pinned_vm;
    long unsigned int data_vm;
    long unsigned int exec_vm;
    long unsigned int stack_vm;
    long unsigned int def_flags;
    long unsigned int start_code;
    long unsigned int end_code;
    long unsigned int start_data;
    long unsigned int end_data;
    long unsigned int start_brk;
    long unsigned int brk;
    long unsigned int start_stack;
    long unsigned int arg_start;
    long unsigned int arg_end;
    long unsigned int env_start;
    long unsigned int env_end;
    long unsigned int saved_auxv[46];
    struct mm_rss_stat rss_stat;
    struct linux_binfmt *binfmt;
    cpumask_var_t cpu_vm_mask_var;
    mm_context_t context;
    long unsigned int flags;
    struct core_state *core_state;
    atomic_t membarrier_state;
    spinlock_t ioctx_lock;
    struct kioctx_table *ioctx_table;
    struct task_struct *owner;
    struct user_namespace *user_ns;
    struct file *exe_file;
    struct mmu_notifier_mm *mmu_notifier_mm;
    struct cpumask cpumask_allocation;
    long unsigned int numa_next_scan;
    long unsigned int numa_scan_offset;
    int numa_scan_seq;
    atomic_t tlb_flush_pending;
    bool tlb_flush_batched;
    struct uprobes_state uprobes_state;
    atomic_long_t hugetlb_usage;
    struct work_struct async_put_work;
    struct hmm *hmm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct mm_struct {
    struct vm_area_struct *mmap;
    struct rb_root mm_rb;
    u64 vmacache_seqnum;
    long unsigned int (*get_unmapped_area)(struct file *, long unsigned int, long unsigned int, long unsigned int, long unsigned int);
    long unsigned int mmap_base;
    long unsigned int mmap_legacy_base;
    long unsigned int mmap_compat_base;
    long unsigned int mmap_compat_legacy_base;
    long unsigned int task_size;
    long unsigned int highest_vm_end;
    pgd_t *pgd;
    atomic_t mm_users;
    atomic_t mm_count;
    atomic_long_t pgtables_bytes;
    int map_count;
    spinlock_t page_table_lock;
    struct rw_semaphore mmap_sem;
    struct list_head mmlist;
    long unsigned int hiwater_rss;
    long unsigned int hiwater_vm;
    long unsigned int total_vm;
    long unsigned int locked_vm;
    long unsigned int pinned_vm;
    long unsigned int data_vm;
    long unsigned int exec_vm;
    long unsigned int stack_vm;
    long unsigned int def_flags;
    spinlock_t arg_lock;
    long unsigned int start_code;
    long unsigned int end_code;
    long unsigned int start_data;
    long unsigned int end_data;
    long unsigned int start_brk;
    long unsigned int brk;
    long unsigned int start_stack;
    long unsigned int arg_start;
    long unsigned int arg_end;
    long unsigned int env_start;
    long unsigned int env_end;
    long unsigned int saved_auxv[46];
    struct mm_rss_stat rss_stat;
    struct linux_binfmt *binfmt;
    cpumask_var_t cpu_vm_mask_var;
    mm_context_t context;
    long unsigned int flags;
    struct core_state *core_state;
    atomic_t membarrier_state;
    spinlock_t ioctx_lock;
    struct kioctx_table *ioctx_table;
    struct task_struct *owner;
    struct user_namespace *user_ns;
    struct file *exe_file;
    struct mmu_notifier_mm *mmu_notifier_mm;
    struct cpumask cpumask_allocation;
    long unsigned int numa_next_scan;
    long unsigned int numa_scan_offset;
    int numa_scan_seq;
    atomic_t tlb_flush_pending;
    bool tlb_flush_batched;
    struct uprobes_state uprobes_state;
    atomic_long_t hugetlb_usage;
    struct work_struct async_put_work;
    struct hmm *hmm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct mm_struct {
    struct vm_area_struct *mmap;
    struct rb_root mm_rb;
    u64 vmacache_seqnum;
    long unsigned int (*get_unmapped_area)(struct file *, long unsigned int, long unsigned int, long unsigned int, long unsigned int);
    long unsigned int mmap_base;
    long unsigned int mmap_legacy_base;
    long unsigned int mmap_compat_base;
    long unsigned int mmap_compat_legacy_base;
    long unsigned int task_size;
    long unsigned int highest_vm_end;
    pgd_t *pgd;
    atomic_t mm_users;
    atomic_t mm_count;
    atomic_long_t pgtables_bytes;
    int map_count;
    spinlock_t page_table_lock;
    struct rw_semaphore mmap_sem;
    struct list_head mmlist;
    long unsigned int hiwater_rss;
    long unsigned int hiwater_vm;
    long unsigned int total_vm;
    long unsigned int locked_vm;
    long unsigned int pinned_vm;
    long unsigned int data_vm;
    long unsigned int exec_vm;
    long unsigned int stack_vm;
    long unsigned int def_flags;
    spinlock_t arg_lock;
    long unsigned int start_code;
    long unsigned int end_code;
    long unsigned int start_data;
    long unsigned int end_data;
    long unsigned int start_brk;
    long unsigned int brk;
    long unsigned int start_stack;
    long unsigned int arg_start;
    long unsigned int arg_end;
    long unsigned int env_start;
    long unsigned int env_end;
    long unsigned int saved_auxv[46];
    struct mm_rss_stat rss_stat;
    struct linux_binfmt *binfmt;
    mm_context_t context;
    long unsigned int flags;
    struct core_state *core_state;
    atomic_t membarrier_state;
    spinlock_t ioctx_lock;
    struct kioctx_table *ioctx_table;
    struct task_struct *owner;
    struct user_namespace *user_ns;
    struct file *exe_file;
    struct mmu_notifier_mm *mmu_notifier_mm;
    long unsigned int numa_next_scan;
    long unsigned int numa_scan_offset;
    int numa_scan_seq;
    atomic_t tlb_flush_pending;
    bool tlb_flush_batched;
    struct uprobes_state uprobes_state;
    atomic_long_t hugetlb_usage;
    struct work_struct async_put_work;
    struct hmm *hmm;
    long unsigned int cpu_bitmap[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct mm_struct {
    struct vm_area_struct *mmap;
    struct rb_root mm_rb;
    u64 vmacache_seqnum;
    long unsigned int (*get_unmapped_area)(struct file *, long unsigned int, long unsigned int, long unsigned int, long unsigned int);
    long unsigned int mmap_base;
    long unsigned int mmap_legacy_base;
    long unsigned int mmap_compat_base;
    long unsigned int mmap_compat_legacy_base;
    long unsigned int task_size;
    long unsigned int highest_vm_end;
    pgd_t *pgd;
    atomic_t mm_users;
    atomic_t mm_count;
    atomic_long_t pgtables_bytes;
    int map_count;
    spinlock_t page_table_lock;
    struct rw_semaphore mmap_sem;
    struct list_head mmlist;
    long unsigned int hiwater_rss;
    long unsigned int hiwater_vm;
    long unsigned int total_vm;
    long unsigned int locked_vm;
    atomic64_t pinned_vm;
    long unsigned int data_vm;
    long unsigned int exec_vm;
    long unsigned int stack_vm;
    long unsigned int def_flags;
    spinlock_t arg_lock;
    long unsigned int start_code;
    long unsigned int end_code;
    long unsigned int start_data;
    long unsigned int end_data;
    long unsigned int start_brk;
    long unsigned int brk;
    long unsigned int start_stack;
    long unsigned int arg_start;
    long unsigned int arg_end;
    long unsigned int env_start;
    long unsigned int env_end;
    long unsigned int saved_auxv[46];
    struct mm_rss_stat rss_stat;
    struct linux_binfmt *binfmt;
    mm_context_t context;
    long unsigned int flags;
    struct core_state *core_state;
    atomic_t membarrier_state;
    spinlock_t ioctx_lock;
    struct kioctx_table *ioctx_table;
    struct task_struct *owner;
    struct user_namespace *user_ns;
    struct file *exe_file;
    struct mmu_notifier_mm *mmu_notifier_mm;
    long unsigned int numa_next_scan;
    long unsigned int numa_scan_offset;
    int numa_scan_seq;
    atomic_t tlb_flush_pending;
    bool tlb_flush_batched;
    struct uprobes_state uprobes_state;
    atomic_long_t hugetlb_usage;
    struct work_struct async_put_work;
    struct hmm *hmm;
    long unsigned int cpu_bitmap[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct mm_struct {
    struct vm_area_struct *mmap;
    struct rb_root mm_rb;
    u64 vmacache_seqnum;
    long unsigned int (*get_unmapped_area)(struct file *, long unsigned int, long unsigned int, long unsigned int, long unsigned int);
    long unsigned int mmap_base;
    long unsigned int mmap_legacy_base;
    long unsigned int mmap_compat_base;
    long unsigned int mmap_compat_legacy_base;
    long unsigned int task_size;
    long unsigned int highest_vm_end;
    pgd_t *pgd;
    atomic_t membarrier_state;
    atomic_t mm_users;
    atomic_t mm_count;
    atomic_long_t pgtables_bytes;
    int map_count;
    spinlock_t page_table_lock;
    struct rw_semaphore mmap_sem;
    struct list_head mmlist;
    long unsigned int hiwater_rss;
    long unsigned int hiwater_vm;
    long unsigned int total_vm;
    long unsigned int locked_vm;
    atomic64_t pinned_vm;
    long unsigned int data_vm;
    long unsigned int exec_vm;
    long unsigned int stack_vm;
    long unsigned int def_flags;
    spinlock_t arg_lock;
    long unsigned int start_code;
    long unsigned int end_code;
    long unsigned int start_data;
    long unsigned int end_data;
    long unsigned int start_brk;
    long unsigned int brk;
    long unsigned int start_stack;
    long unsigned int arg_start;
    long unsigned int arg_end;
    long unsigned int env_start;
    long unsigned int env_end;
    long unsigned int saved_auxv[46];
    struct mm_rss_stat rss_stat;
    struct linux_binfmt *binfmt;
    mm_context_t context;
    long unsigned int flags;
    struct core_state *core_state;
    spinlock_t ioctx_lock;
    struct kioctx_table *ioctx_table;
    struct task_struct *owner;
    struct user_namespace *user_ns;
    struct file *exe_file;
    struct mmu_notifier_mm *mmu_notifier_mm;
    long unsigned int numa_next_scan;
    long unsigned int numa_scan_offset;
    int numa_scan_seq;
    atomic_t tlb_flush_pending;
    bool tlb_flush_batched;
    struct uprobes_state uprobes_state;
    atomic_long_t hugetlb_usage;
    struct work_struct async_put_work;
    long unsigned int cpu_bitmap[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct mm_struct {
    struct vm_area_struct *mmap;
    struct rb_root mm_rb;
    u64 vmacache_seqnum;
    long unsigned int (*get_unmapped_area)(struct file *, long unsigned int, long unsigned int, long unsigned int, long unsigned int);
    long unsigned int mmap_base;
    long unsigned int mmap_legacy_base;
    long unsigned int mmap_compat_base;
    long unsigned int mmap_compat_legacy_base;
    long unsigned int task_size;
    long unsigned int highest_vm_end;
    pgd_t *pgd;
    atomic_t membarrier_state;
    atomic_t mm_users;
    atomic_t mm_count;
    atomic_long_t pgtables_bytes;
    int map_count;
    spinlock_t page_table_lock;
    struct rw_semaphore mmap_lock;
    struct list_head mmlist;
    long unsigned int hiwater_rss;
    long unsigned int hiwater_vm;
    long unsigned int total_vm;
    long unsigned int locked_vm;
    atomic64_t pinned_vm;
    long unsigned int data_vm;
    long unsigned int exec_vm;
    long unsigned int stack_vm;
    long unsigned int def_flags;
    spinlock_t arg_lock;
    long unsigned int start_code;
    long unsigned int end_code;
    long unsigned int start_data;
    long unsigned int end_data;
    long unsigned int start_brk;
    long unsigned int brk;
    long unsigned int start_stack;
    long unsigned int arg_start;
    long unsigned int arg_end;
    long unsigned int env_start;
    long unsigned int env_end;
    long unsigned int saved_auxv[46];
    struct mm_rss_stat rss_stat;
    struct linux_binfmt *binfmt;
    mm_context_t context;
    long unsigned int flags;
    struct core_state *core_state;
    spinlock_t ioctx_lock;
    struct kioctx_table *ioctx_table;
    struct task_struct *owner;
    struct user_namespace *user_ns;
    struct file *exe_file;
    struct mmu_notifier_subscriptions *notifier_subscriptions;
    long unsigned int numa_next_scan;
    long unsigned int numa_scan_offset;
    int numa_scan_seq;
    atomic_t tlb_flush_pending;
    bool tlb_flush_batched;
    struct uprobes_state uprobes_state;
    atomic_long_t hugetlb_usage;
    struct work_struct async_put_work;
    long unsigned int cpu_bitmap[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mm_struct {
    struct vm_area_struct *mmap;
    struct rb_root mm_rb;
    u64 vmacache_seqnum;
    long unsigned int (*get_unmapped_area)(struct file *, long unsigned int, long unsigned int, long unsigned int, long unsigned int);
    long unsigned int mmap_base;
    long unsigned int mmap_legacy_base;
    long unsigned int mmap_compat_base;
    long unsigned int mmap_compat_legacy_base;
    long unsigned int task_size;
    long unsigned int highest_vm_end;
    pgd_t *pgd;
    atomic_t membarrier_state;
    atomic_t mm_users;
    atomic_t mm_count;
    atomic_t has_pinned;
    seqcount_t write_protect_seq;
    atomic_long_t pgtables_bytes;
    int map_count;
    spinlock_t page_table_lock;
    struct rw_semaphore mmap_lock;
    struct list_head mmlist;
    long unsigned int hiwater_rss;
    long unsigned int hiwater_vm;
    long unsigned int total_vm;
    long unsigned int locked_vm;
    atomic64_t pinned_vm;
    long unsigned int data_vm;
    long unsigned int exec_vm;
    long unsigned int stack_vm;
    long unsigned int def_flags;
    spinlock_t arg_lock;
    long unsigned int start_code;
    long unsigned int end_code;
    long unsigned int start_data;
    long unsigned int end_data;
    long unsigned int start_brk;
    long unsigned int brk;
    long unsigned int start_stack;
    long unsigned int arg_start;
    long unsigned int arg_end;
    long unsigned int env_start;
    long unsigned int env_end;
    long unsigned int saved_auxv[46];
    struct mm_rss_stat rss_stat;
    struct linux_binfmt *binfmt;
    mm_context_t context;
    long unsigned int flags;
    struct core_state *core_state;
    spinlock_t ioctx_lock;
    struct kioctx_table *ioctx_table;
    struct task_struct *owner;
    struct user_namespace *user_ns;
    struct file *exe_file;
    struct mmu_notifier_subscriptions *notifier_subscriptions;
    long unsigned int numa_next_scan;
    long unsigned int numa_scan_offset;
    int numa_scan_seq;
    atomic_t tlb_flush_pending;
    bool tlb_flush_batched;
    struct uprobes_state uprobes_state;
    atomic_long_t hugetlb_usage;
    struct work_struct async_put_work;
    u32 pasid;
    long unsigned int cpu_bitmap[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mm_struct {
    struct vm_area_struct *mmap;
    struct rb_root mm_rb;
    u64 vmacache_seqnum;
    long unsigned int (*get_unmapped_area)(struct file *, long unsigned int, long unsigned int, long unsigned int, long unsigned int);
    long unsigned int mmap_base;
    long unsigned int mmap_legacy_base;
    long unsigned int mmap_compat_base;
    long unsigned int mmap_compat_legacy_base;
    long unsigned int task_size;
    long unsigned int highest_vm_end;
    pgd_t *pgd;
    atomic_t membarrier_state;
    atomic_t mm_users;
    atomic_t mm_count;
    atomic_t has_pinned;
    atomic_long_t pgtables_bytes;
    int map_count;
    spinlock_t page_table_lock;
    struct rw_semaphore mmap_lock;
    struct list_head mmlist;
    long unsigned int hiwater_rss;
    long unsigned int hiwater_vm;
    long unsigned int total_vm;
    long unsigned int locked_vm;
    atomic64_t pinned_vm;
    long unsigned int data_vm;
    long unsigned int exec_vm;
    long unsigned int stack_vm;
    long unsigned int def_flags;
    seqcount_t write_protect_seq;
    spinlock_t arg_lock;
    long unsigned int start_code;
    long unsigned int end_code;
    long unsigned int start_data;
    long unsigned int end_data;
    long unsigned int start_brk;
    long unsigned int brk;
    long unsigned int start_stack;
    long unsigned int arg_start;
    long unsigned int arg_end;
    long unsigned int env_start;
    long unsigned int env_end;
    long unsigned int saved_auxv[46];
    struct mm_rss_stat rss_stat;
    struct linux_binfmt *binfmt;
    mm_context_t context;
    long unsigned int flags;
    struct core_state *core_state;
    spinlock_t ioctx_lock;
    struct kioctx_table *ioctx_table;
    struct task_struct *owner;
    struct user_namespace *user_ns;
    struct file *exe_file;
    struct mmu_notifier_subscriptions *notifier_subscriptions;
    long unsigned int numa_next_scan;
    long unsigned int numa_scan_offset;
    int numa_scan_seq;
    atomic_t tlb_flush_pending;
    bool tlb_flush_batched;
    struct uprobes_state uprobes_state;
    atomic_long_t hugetlb_usage;
    struct work_struct async_put_work;
    u32 pasid;
    long unsigned int cpu_bitmap[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mm_struct {
    struct vm_area_struct *mmap;
    struct rb_root mm_rb;
    u64 vmacache_seqnum;
    long unsigned int (*get_unmapped_area)(struct file *, long unsigned int, long unsigned int, long unsigned int, long unsigned int);
    long unsigned int mmap_base;
    long unsigned int mmap_legacy_base;
    long unsigned int mmap_compat_base;
    long unsigned int mmap_compat_legacy_base;
    long unsigned int task_size;
    long unsigned int highest_vm_end;
    pgd_t *pgd;
    atomic_t membarrier_state;
    atomic_t mm_users;
    atomic_t mm_count;
    atomic_long_t pgtables_bytes;
    int map_count;
    spinlock_t page_table_lock;
    struct rw_semaphore mmap_lock;
    struct list_head mmlist;
    long unsigned int hiwater_rss;
    long unsigned int hiwater_vm;
    long unsigned int total_vm;
    long unsigned int locked_vm;
    atomic64_t pinned_vm;
    long unsigned int data_vm;
    long unsigned int exec_vm;
    long unsigned int stack_vm;
    long unsigned int def_flags;
    seqcount_t write_protect_seq;
    spinlock_t arg_lock;
    long unsigned int start_code;
    long unsigned int end_code;
    long unsigned int start_data;
    long unsigned int end_data;
    long unsigned int start_brk;
    long unsigned int brk;
    long unsigned int start_stack;
    long unsigned int arg_start;
    long unsigned int arg_end;
    long unsigned int env_start;
    long unsigned int env_end;
    long unsigned int saved_auxv[48];
    struct mm_rss_stat rss_stat;
    struct linux_binfmt *binfmt;
    mm_context_t context;
    long unsigned int flags;
    struct core_state *core_state;
    spinlock_t ioctx_lock;
    struct kioctx_table *ioctx_table;
    struct task_struct *owner;
    struct user_namespace *user_ns;
    struct file *exe_file;
    struct mmu_notifier_subscriptions *notifier_subscriptions;
    long unsigned int numa_next_scan;
    long unsigned int numa_scan_offset;
    int numa_scan_seq;
    atomic_t tlb_flush_pending;
    bool tlb_flush_batched;
    struct uprobes_state uprobes_state;
    atomic_long_t hugetlb_usage;
    struct work_struct async_put_work;
    u32 pasid;
    long unsigned int cpu_bitmap[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mm_struct {
    struct vm_area_struct *mmap;
    struct rb_root mm_rb;
    u64 vmacache_seqnum;
    long unsigned int (*get_unmapped_area)(struct file *, long unsigned int, long unsigned int, long unsigned int, long unsigned int);
    long unsigned int mmap_base;
    long unsigned int mmap_legacy_base;
    long unsigned int mmap_compat_base;
    long unsigned int mmap_compat_legacy_base;
    long unsigned int task_size;
    long unsigned int highest_vm_end;
    pgd_t *pgd;
    atomic_t membarrier_state;
    atomic_t mm_users;
    atomic_t mm_count;
    atomic_long_t pgtables_bytes;
    int map_count;
    spinlock_t page_table_lock;
    struct rw_semaphore mmap_lock;
    struct list_head mmlist;
    long unsigned int hiwater_rss;
    long unsigned int hiwater_vm;
    long unsigned int total_vm;
    long unsigned int locked_vm;
    atomic64_t pinned_vm;
    long unsigned int data_vm;
    long unsigned int exec_vm;
    long unsigned int stack_vm;
    long unsigned int def_flags;
    seqcount_t write_protect_seq;
    spinlock_t arg_lock;
    long unsigned int start_code;
    long unsigned int end_code;
    long unsigned int start_data;
    long unsigned int end_data;
    long unsigned int start_brk;
    long unsigned int brk;
    long unsigned int start_stack;
    long unsigned int arg_start;
    long unsigned int arg_end;
    long unsigned int env_start;
    long unsigned int env_end;
    long unsigned int saved_auxv[48];
    struct mm_rss_stat rss_stat;
    struct linux_binfmt *binfmt;
    mm_context_t context;
    long unsigned int flags;
    spinlock_t ioctx_lock;
    struct kioctx_table *ioctx_table;
    struct task_struct *owner;
    struct user_namespace *user_ns;
    struct file *exe_file;
    struct mmu_notifier_subscriptions *notifier_subscriptions;
    long unsigned int numa_next_scan;
    long unsigned int numa_scan_offset;
    int numa_scan_seq;
    atomic_t tlb_flush_pending;
    atomic_t tlb_flush_batched;
    struct uprobes_state uprobes_state;
    atomic_long_t hugetlb_usage;
    struct work_struct async_put_work;
    u32 pasid;
    long unsigned int ksm_merging_pages;
    long unsigned int cpu_bitmap[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mm_struct {
    struct maple_tree mm_mt;
    long unsigned int (*get_unmapped_area)(struct file *, long unsigned int, long unsigned int, long unsigned int, long unsigned int);
    long unsigned int mmap_base;
    long unsigned int mmap_legacy_base;
    long unsigned int mmap_compat_base;
    long unsigned int mmap_compat_legacy_base;
    long unsigned int task_size;
    pgd_t *pgd;
    atomic_t membarrier_state;
    atomic_t mm_users;
    atomic_t mm_count;
    atomic_long_t pgtables_bytes;
    int map_count;
    spinlock_t page_table_lock;
    struct rw_semaphore mmap_lock;
    struct list_head mmlist;
    long unsigned int hiwater_rss;
    long unsigned int hiwater_vm;
    long unsigned int total_vm;
    long unsigned int locked_vm;
    atomic64_t pinned_vm;
    long unsigned int data_vm;
    long unsigned int exec_vm;
    long unsigned int stack_vm;
    long unsigned int def_flags;
    seqcount_t write_protect_seq;
    spinlock_t arg_lock;
    long unsigned int start_code;
    long unsigned int end_code;
    long unsigned int start_data;
    long unsigned int end_data;
    long unsigned int start_brk;
    long unsigned int brk;
    long unsigned int start_stack;
    long unsigned int arg_start;
    long unsigned int arg_end;
    long unsigned int env_start;
    long unsigned int env_end;
    long unsigned int saved_auxv[48];
    struct percpu_counter rss_stat[4];
    struct linux_binfmt *binfmt;
    mm_context_t context;
    long unsigned int flags;
    spinlock_t ioctx_lock;
    struct kioctx_table *ioctx_table;
    struct task_struct *owner;
    struct user_namespace *user_ns;
    struct file *exe_file;
    struct mmu_notifier_subscriptions *notifier_subscriptions;
    long unsigned int numa_next_scan;
    long unsigned int numa_scan_offset;
    int numa_scan_seq;
    atomic_t tlb_flush_pending;
    atomic_t tlb_flush_batched;
    struct uprobes_state uprobes_state;
    atomic_long_t hugetlb_usage;
    struct work_struct async_put_work;
    u32 pasid;
    long unsigned int ksm_merging_pages;
    long unsigned int ksm_rmap_items;
    struct (anon) lru_gen;
    long unsigned int cpu_bitmap[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mm_struct {
    atomic_t mm_count;
    struct maple_tree mm_mt;
    long unsigned int (*get_unmapped_area)(struct file *, long unsigned int, long unsigned int, long unsigned int, long unsigned int);
    long unsigned int mmap_base;
    long unsigned int mmap_legacy_base;
    long unsigned int mmap_compat_base;
    long unsigned int mmap_compat_legacy_base;
    long unsigned int task_size;
    pgd_t *pgd;
    atomic_t membarrier_state;
    atomic_t mm_users;
    struct mm_cid *pcpu_cid;
    long unsigned int mm_cid_next_scan;
    atomic_long_t pgtables_bytes;
    int map_count;
    spinlock_t page_table_lock;
    struct rw_semaphore mmap_lock;
    struct list_head mmlist;
    int mm_lock_seq;
    long unsigned int hiwater_rss;
    long unsigned int hiwater_vm;
    long unsigned int total_vm;
    long unsigned int locked_vm;
    atomic64_t pinned_vm;
    long unsigned int data_vm;
    long unsigned int exec_vm;
    long unsigned int stack_vm;
    long unsigned int def_flags;
    seqcount_t write_protect_seq;
    spinlock_t arg_lock;
    long unsigned int start_code;
    long unsigned int end_code;
    long unsigned int start_data;
    long unsigned int end_data;
    long unsigned int start_brk;
    long unsigned int brk;
    long unsigned int start_stack;
    long unsigned int arg_start;
    long unsigned int arg_end;
    long unsigned int env_start;
    long unsigned int env_end;
    long unsigned int saved_auxv[52];
    struct percpu_counter rss_stat[4];
    struct linux_binfmt *binfmt;
    mm_context_t context;
    long unsigned int flags;
    spinlock_t ioctx_lock;
    struct kioctx_table *ioctx_table;
    struct task_struct *owner;
    struct user_namespace *user_ns;
    struct file *exe_file;
    struct mmu_notifier_subscriptions *notifier_subscriptions;
    long unsigned int numa_next_scan;
    long unsigned int numa_scan_offset;
    int numa_scan_seq;
    atomic_t tlb_flush_pending;
    atomic_t tlb_flush_batched;
    struct uprobes_state uprobes_state;
    atomic_long_t hugetlb_usage;
    struct work_struct async_put_work;
    u32 pasid;
    long unsigned int ksm_merging_pages;
    long unsigned int ksm_rmap_items;
    struct (anon) lru_gen;
    long unsigned int cpu_bitmap[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mm_struct {
    atomic_t mm_count;
    struct maple_tree mm_mt;
    long unsigned int (*get_unmapped_area)(struct file *, long unsigned int, long unsigned int, long unsigned int, long unsigned int);
    long unsigned int mmap_base;
    long unsigned int mmap_legacy_base;
    long unsigned int mmap_compat_base;
    long unsigned int mmap_compat_legacy_base;
    long unsigned int task_size;
    pgd_t *pgd;
    atomic_t membarrier_state;
    atomic_t mm_users;
    struct mm_cid *pcpu_cid;
    long unsigned int mm_cid_next_scan;
    atomic_long_t pgtables_bytes;
    int map_count;
    spinlock_t page_table_lock;
    struct rw_semaphore mmap_lock;
    struct list_head mmlist;
    int mm_lock_seq;
    long unsigned int hiwater_rss;
    long unsigned int hiwater_vm;
    long unsigned int total_vm;
    long unsigned int locked_vm;
    atomic64_t pinned_vm;
    long unsigned int data_vm;
    long unsigned int exec_vm;
    long unsigned int stack_vm;
    long unsigned int def_flags;
    seqcount_t write_protect_seq;
    spinlock_t arg_lock;
    long unsigned int start_code;
    long unsigned int end_code;
    long unsigned int start_data;
    long unsigned int end_data;
    long unsigned int start_brk;
    long unsigned int brk;
    long unsigned int start_stack;
    long unsigned int arg_start;
    long unsigned int arg_end;
    long unsigned int env_start;
    long unsigned int env_end;
    long unsigned int saved_auxv[52];
    struct percpu_counter rss_stat[4];
    struct linux_binfmt *binfmt;
    mm_context_t context;
    long unsigned int flags;
    spinlock_t ioctx_lock;
    struct kioctx_table *ioctx_table;
    struct task_struct *owner;
    struct user_namespace *user_ns;
    struct file *exe_file;
    struct mmu_notifier_subscriptions *notifier_subscriptions;
    long unsigned int numa_next_scan;
    long unsigned int numa_scan_offset;
    int numa_scan_seq;
    atomic_t tlb_flush_pending;
    atomic_t tlb_flush_batched;
    struct uprobes_state uprobes_state;
    atomic_long_t hugetlb_usage;
    struct work_struct async_put_work;
    struct iommu_mm_data *iommu_mm;
    long unsigned int ksm_merging_pages;
    long unsigned int ksm_rmap_items;
    long unsigned int ksm_zero_pages;
    struct (anon) lru_gen;
    long unsigned int cpu_bitmap[0];
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
struct mm_struct {
    struct vm_area_struct *mmap;
    struct rb_root mm_rb;
    u64 vmacache_seqnum;
    long unsigned int (*get_unmapped_area)(struct file *, long unsigned int, long unsigned int, long unsigned int, long unsigned int);
    long unsigned int mmap_base;
    long unsigned int mmap_legacy_base;
    long unsigned int task_size;
    long unsigned int highest_vm_end;
    pgd_t *pgd;
    atomic_t membarrier_state;
    atomic_t mm_users;
    atomic_t mm_count;
    atomic_long_t pgtables_bytes;
    int map_count;
    spinlock_t page_table_lock;
    struct rw_semaphore mmap_sem;
    struct list_head mmlist;
    long unsigned int hiwater_rss;
    long unsigned int hiwater_vm;
    long unsigned int total_vm;
    long unsigned int locked_vm;
    atomic64_t pinned_vm;
    long unsigned int data_vm;
    long unsigned int exec_vm;
    long unsigned int stack_vm;
    long unsigned int def_flags;
    spinlock_t arg_lock;
    long unsigned int start_code;
    long unsigned int end_code;
    long unsigned int start_data;
    long unsigned int end_data;
    long unsigned int start_brk;
    long unsigned int brk;
    long unsigned int start_stack;
    long unsigned int arg_start;
    long unsigned int arg_end;
    long unsigned int env_start;
    long unsigned int env_end;
    long unsigned int saved_auxv[46];
    struct mm_rss_stat rss_stat;
    struct linux_binfmt *binfmt;
    mm_context_t context;
    long unsigned int flags;
    struct core_state *core_state;
    spinlock_t ioctx_lock;
    struct kioctx_table *ioctx_table;
    struct task_struct *owner;
    struct user_namespace *user_ns;
    struct file *exe_file;
    struct mmu_notifier_mm *mmu_notifier_mm;
    long unsigned int numa_next_scan;
    long unsigned int numa_scan_offset;
    int numa_scan_seq;
    atomic_t tlb_flush_pending;
    struct uprobes_state uprobes_state;
    atomic_long_t hugetlb_usage;
    struct work_struct async_put_work;
    long unsigned int cpu_bitmap[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mm_struct {
    struct vm_area_struct *mmap;
    struct rb_root mm_rb;
    u64 vmacache_seqnum;
    long unsigned int (*get_unmapped_area)(struct file *, long unsigned int, long unsigned int, long unsigned int, long unsigned int);
    long unsigned int mmap_base;
    long unsigned int mmap_legacy_base;
    long unsigned int task_size;
    long unsigned int highest_vm_end;
    pgd_t *pgd;
    atomic_t membarrier_state;
    atomic_t mm_users;
    atomic_t mm_count;
    atomic_long_t pgtables_bytes;
    int map_count;
    spinlock_t page_table_lock;
    struct rw_semaphore mmap_sem;
    struct list_head mmlist;
    long unsigned int hiwater_rss;
    long unsigned int hiwater_vm;
    long unsigned int total_vm;
    long unsigned int locked_vm;
    atomic64_t pinned_vm;
    long unsigned int data_vm;
    long unsigned int exec_vm;
    long unsigned int stack_vm;
    long unsigned int def_flags;
    spinlock_t arg_lock;
    long unsigned int start_code;
    long unsigned int end_code;
    long unsigned int start_data;
    long unsigned int end_data;
    long unsigned int start_brk;
    long unsigned int brk;
    long unsigned int start_stack;
    long unsigned int arg_start;
    long unsigned int arg_end;
    long unsigned int env_start;
    long unsigned int env_end;
    long unsigned int saved_auxv[42];
    struct mm_rss_stat rss_stat;
    struct linux_binfmt *binfmt;
    mm_context_t context;
    long unsigned int flags;
    struct core_state *core_state;
    spinlock_t ioctx_lock;
    struct kioctx_table *ioctx_table;
    struct task_struct *owner;
    struct user_namespace *user_ns;
    struct file *exe_file;
    struct mmu_notifier_mm *mmu_notifier_mm;
    atomic_t tlb_flush_pending;
    struct uprobes_state uprobes_state;
    struct work_struct async_put_work;
    long unsigned int cpu_bitmap[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct mm_struct {
    struct vm_area_struct *mmap;
    struct rb_root mm_rb;
    u64 vmacache_seqnum;
    long unsigned int (*get_unmapped_area)(struct file *, long unsigned int, long unsigned int, long unsigned int, long unsigned int);
    long unsigned int mmap_base;
    long unsigned int mmap_legacy_base;
    long unsigned int task_size;
    long unsigned int highest_vm_end;
    pgd_t *pgd;
    atomic_t membarrier_state;
    atomic_t mm_users;
    atomic_t mm_count;
    atomic_long_t pgtables_bytes;
    int map_count;
    spinlock_t page_table_lock;
    struct rw_semaphore mmap_sem;
    struct list_head mmlist;
    long unsigned int hiwater_rss;
    long unsigned int hiwater_vm;
    long unsigned int total_vm;
    long unsigned int locked_vm;
    atomic64_t pinned_vm;
    long unsigned int data_vm;
    long unsigned int exec_vm;
    long unsigned int stack_vm;
    long unsigned int def_flags;
    spinlock_t arg_lock;
    long unsigned int start_code;
    long unsigned int end_code;
    long unsigned int start_data;
    long unsigned int end_data;
    long unsigned int start_brk;
    long unsigned int brk;
    long unsigned int start_stack;
    long unsigned int arg_start;
    long unsigned int arg_end;
    long unsigned int env_start;
    long unsigned int env_end;
    long unsigned int saved_auxv[70];
    struct mm_rss_stat rss_stat;
    struct linux_binfmt *binfmt;
    mm_context_t context;
    long unsigned int flags;
    struct core_state *core_state;
    spinlock_t ioctx_lock;
    struct kioctx_table *ioctx_table;
    struct task_struct *owner;
    struct user_namespace *user_ns;
    struct file *exe_file;
    struct mmu_notifier_mm *mmu_notifier_mm;
    long unsigned int numa_next_scan;
    long unsigned int numa_scan_offset;
    int numa_scan_seq;
    atomic_t tlb_flush_pending;
    struct uprobes_state uprobes_state;
    atomic_long_t hugetlb_usage;
    struct work_struct async_put_work;
    long unsigned int cpu_bitmap[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct mm_struct {
    struct vm_area_struct *mmap;
    struct rb_root mm_rb;
    u64 vmacache_seqnum;
    long unsigned int (*get_unmapped_area)(struct file *, long unsigned int, long unsigned int, long unsigned int, long unsigned int);
    long unsigned int mmap_base;
    long unsigned int mmap_legacy_base;
    long unsigned int task_size;
    long unsigned int highest_vm_end;
    pgd_t *pgd;
    atomic_t membarrier_state;
    atomic_t mm_users;
    atomic_t mm_count;
    atomic_long_t pgtables_bytes;
    int map_count;
    spinlock_t page_table_lock;
    struct rw_semaphore mmap_sem;
    struct list_head mmlist;
    long unsigned int hiwater_rss;
    long unsigned int hiwater_vm;
    long unsigned int total_vm;
    long unsigned int locked_vm;
    atomic64_t pinned_vm;
    long unsigned int data_vm;
    long unsigned int exec_vm;
    long unsigned int stack_vm;
    long unsigned int def_flags;
    spinlock_t arg_lock;
    long unsigned int start_code;
    long unsigned int end_code;
    long unsigned int start_data;
    long unsigned int end_data;
    long unsigned int start_brk;
    long unsigned int brk;
    long unsigned int start_stack;
    long unsigned int arg_start;
    long unsigned int arg_end;
    long unsigned int env_start;
    long unsigned int env_end;
    long unsigned int saved_auxv[42];
    struct mm_rss_stat rss_stat;
    struct linux_binfmt *binfmt;
    mm_context_t context;
    long unsigned int flags;
    struct core_state *core_state;
    spinlock_t ioctx_lock;
    struct kioctx_table *ioctx_table;
    struct task_struct *owner;
    struct user_namespace *user_ns;
    struct file *exe_file;
    struct mmu_notifier_mm *mmu_notifier_mm;
    atomic_t tlb_flush_pending;
    struct uprobes_state uprobes_state;
    atomic_long_t hugetlb_usage;
    struct work_struct async_put_work;
    long unsigned int cpu_bitmap[0];
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
struct mm_struct {
    struct vm_area_struct *mmap;
    struct rb_root mm_rb;
    u64 vmacache_seqnum;
    long unsigned int (*get_unmapped_area)(struct file *, long unsigned int, long unsigned int, long unsigned int, long unsigned int);
    long unsigned int mmap_base;
    long unsigned int mmap_legacy_base;
    long unsigned int mmap_compat_base;
    long unsigned int mmap_compat_legacy_base;
    long unsigned int task_size;
    long unsigned int highest_vm_end;
    pgd_t *pgd;
    atomic_t membarrier_state;
    atomic_t mm_users;
    atomic_t mm_count;
    atomic_long_t pgtables_bytes;
    int map_count;
    spinlock_t page_table_lock;
    struct rw_semaphore mmap_sem;
    struct list_head mmlist;
    long unsigned int hiwater_rss;
    long unsigned int hiwater_vm;
    long unsigned int total_vm;
    long unsigned int locked_vm;
    atomic64_t pinned_vm;
    long unsigned int data_vm;
    long unsigned int exec_vm;
    long unsigned int stack_vm;
    long unsigned int def_flags;
    spinlock_t arg_lock;
    long unsigned int start_code;
    long unsigned int end_code;
    long unsigned int start_data;
    long unsigned int end_data;
    long unsigned int start_brk;
    long unsigned int brk;
    long unsigned int start_stack;
    long unsigned int arg_start;
    long unsigned int arg_end;
    long unsigned int env_start;
    long unsigned int env_end;
    long unsigned int saved_auxv[46];
    struct mm_rss_stat rss_stat;
    struct linux_binfmt *binfmt;
    mm_context_t context;
    long unsigned int flags;
    struct core_state *core_state;
    spinlock_t ioctx_lock;
    struct kioctx_table *ioctx_table;
    struct task_struct *owner;
    struct user_namespace *user_ns;
    struct file *exe_file;
    struct mmu_notifier_mm *mmu_notifier_mm;
    long unsigned int numa_next_scan;
    long unsigned int numa_scan_offset;
    int numa_scan_seq;
    atomic_t tlb_flush_pending;
    bool tlb_flush_batched;
    struct uprobes_state uprobes_state;
    atomic_long_t hugetlb_usage;
    struct work_struct async_put_work;
    long unsigned int cpu_bitmap[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct mm_struct {
    struct vm_area_struct *mmap;
    struct rb_root mm_rb;
    u64 vmacache_seqnum;
    long unsigned int (*get_unmapped_area)(struct file *, long unsigned int, long unsigned int, long unsigned int, long unsigned int);
    long unsigned int mmap_base;
    long unsigned int mmap_legacy_base;
    long unsigned int mmap_compat_base;
    long unsigned int mmap_compat_legacy_base;
    long unsigned int task_size;
    long unsigned int highest_vm_end;
    pgd_t *pgd;
    atomic_t membarrier_state;
    atomic_t mm_users;
    atomic_t mm_count;
    atomic_long_t pgtables_bytes;
    int map_count;
    spinlock_t page_table_lock;
    struct rw_semaphore mmap_sem;
    struct list_head mmlist;
    long unsigned int hiwater_rss;
    long unsigned int hiwater_vm;
    long unsigned int total_vm;
    long unsigned int locked_vm;
    atomic64_t pinned_vm;
    long unsigned int data_vm;
    long unsigned int exec_vm;
    long unsigned int stack_vm;
    long unsigned int def_flags;
    spinlock_t arg_lock;
    long unsigned int start_code;
    long unsigned int end_code;
    long unsigned int start_data;
    long unsigned int end_data;
    long unsigned int start_brk;
    long unsigned int brk;
    long unsigned int start_stack;
    long unsigned int arg_start;
    long unsigned int arg_end;
    long unsigned int env_start;
    long unsigned int env_end;
    long unsigned int saved_auxv[46];
    struct mm_rss_stat rss_stat;
    struct linux_binfmt *binfmt;
    mm_context_t context;
    long unsigned int flags;
    struct core_state *core_state;
    spinlock_t ioctx_lock;
    struct kioctx_table *ioctx_table;
    struct task_struct *owner;
    struct user_namespace *user_ns;
    struct file *exe_file;
    struct mmu_notifier_mm *mmu_notifier_mm;
    long unsigned int numa_next_scan;
    long unsigned int numa_scan_offset;
    int numa_scan_seq;
    atomic_t tlb_flush_pending;
    bool tlb_flush_batched;
    struct uprobes_state uprobes_state;
    atomic_long_t hugetlb_usage;
    struct work_struct async_put_work;
    long unsigned int cpu_bitmap[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct mm_struct {
    struct vm_area_struct *mmap;
    struct rb_root mm_rb;
    u64 vmacache_seqnum;
    long unsigned int (*get_unmapped_area)(struct file *, long unsigned int, long unsigned int, long unsigned int, long unsigned int);
    long unsigned int mmap_base;
    long unsigned int mmap_legacy_base;
    long unsigned int mmap_compat_base;
    long unsigned int mmap_compat_legacy_base;
    long unsigned int task_size;
    long unsigned int highest_vm_end;
    pgd_t *pgd;
    atomic_t membarrier_state;
    atomic_t mm_users;
    atomic_t mm_count;
    atomic_long_t pgtables_bytes;
    int map_count;
    spinlock_t page_table_lock;
    struct rw_semaphore mmap_sem;
    struct list_head mmlist;
    long unsigned int hiwater_rss;
    long unsigned int hiwater_vm;
    long unsigned int total_vm;
    long unsigned int locked_vm;
    atomic64_t pinned_vm;
    long unsigned int data_vm;
    long unsigned int exec_vm;
    long unsigned int stack_vm;
    long unsigned int def_flags;
    spinlock_t arg_lock;
    long unsigned int start_code;
    long unsigned int end_code;
    long unsigned int start_data;
    long unsigned int end_data;
    long unsigned int start_brk;
    long unsigned int brk;
    long unsigned int start_stack;
    long unsigned int arg_start;
    long unsigned int arg_end;
    long unsigned int env_start;
    long unsigned int env_end;
    long unsigned int saved_auxv[46];
    struct mm_rss_stat rss_stat;
    struct linux_binfmt *binfmt;
    mm_context_t context;
    long unsigned int flags;
    struct core_state *core_state;
    spinlock_t ioctx_lock;
    struct kioctx_table *ioctx_table;
    struct task_struct *owner;
    struct user_namespace *user_ns;
    struct file *exe_file;
    struct mmu_notifier_mm *mmu_notifier_mm;
    long unsigned int numa_next_scan;
    long unsigned int numa_scan_offset;
    int numa_scan_seq;
    atomic_t tlb_flush_pending;
    bool tlb_flush_batched;
    struct uprobes_state uprobes_state;
    atomic_long_t hugetlb_usage;
    struct work_struct async_put_work;
    long unsigned int cpu_bitmap[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct mm_struct {
    struct vm_area_struct *mmap;
    struct rb_root mm_rb;
    u64 vmacache_seqnum;
    long unsigned int (*get_unmapped_area)(struct file *, long unsigned int, long unsigned int, long unsigned int, long unsigned int);
    long unsigned int mmap_base;
    long unsigned int mmap_legacy_base;
    long unsigned int mmap_compat_base;
    long unsigned int mmap_compat_legacy_base;
    long unsigned int task_size;
    long unsigned int highest_vm_end;
    pgd_t *pgd;
    atomic_t membarrier_state;
    atomic_t mm_users;
    atomic_t mm_count;
    atomic_long_t pgtables_bytes;
    int map_count;
    spinlock_t page_table_lock;
    struct rw_semaphore mmap_sem;
    struct list_head mmlist;
    long unsigned int hiwater_rss;
    long unsigned int hiwater_vm;
    long unsigned int total_vm;
    long unsigned int locked_vm;
    atomic64_t pinned_vm;
    long unsigned int data_vm;
    long unsigned int exec_vm;
    long unsigned int stack_vm;
    long unsigned int def_flags;
    spinlock_t arg_lock;
    long unsigned int start_code;
    long unsigned int end_code;
    long unsigned int start_data;
    long unsigned int end_data;
    long unsigned int start_brk;
    long unsigned int brk;
    long unsigned int start_stack;
    long unsigned int arg_start;
    long unsigned int arg_end;
    long unsigned int env_start;
    long unsigned int env_end;
    long unsigned int saved_auxv[46];
    struct mm_rss_stat rss_stat;
    struct linux_binfmt *binfmt;
    mm_context_t context;
    long unsigned int flags;
    struct core_state *core_state;
    spinlock_t ioctx_lock;
    struct kioctx_table *ioctx_table;
    struct task_struct *owner;
    struct user_namespace *user_ns;
    struct file *exe_file;
    struct mmu_notifier_mm *mmu_notifier_mm;
    long unsigned int numa_next_scan;
    long unsigned int numa_scan_offset;
    int numa_scan_seq;
    atomic_t tlb_flush_pending;
    bool tlb_flush_batched;
    struct uprobes_state uprobes_state;
    atomic_long_t hugetlb_usage;
    struct work_struct async_put_work;
    long unsigned int cpu_bitmap[0];
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
<code>long unsigned int data_vm</code>
</li>
<li>
<b>Field added. </b>
<code>struct work_struct async_put_work</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int shared_vm</code>
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
<code>struct user_namespace *user_ns</code>
</li>
<li>
<b>Field added. </b>
<code>struct cpumask cpumask_allocation</code>
</li>
<li>
<b>Field removed. </b>
<code>void *bd_addr</code>
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
<code>long unsigned int mmap_compat_base</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int mmap_compat_legacy_base</code>
</li>
<li>
<b>Field added. </b>
<code>bool tlb_flush_batched</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool tlb_flush_pending</code> ➡️ <code>atomic_t tlb_flush_pending</code>
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
<code>atomic_long_t pgtables_bytes</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t membarrier_state</code>
</li>
<li>
<b>Field added. </b>
<code>struct hmm *hmm</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_long_t nr_ptes</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_long_t nr_pmds</code>
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
<code>spinlock_t arg_lock</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 vmacache_seqnum</code> ➡️ <code>u64 vmacache_seqnum</code>
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
<code>long unsigned int cpu_bitmap[0]</code>
</li>
<li>
<b>Field removed. </b>
<code>cpumask_var_t cpu_vm_mask_var</code>
</li>
<li>
<b>Field removed. </b>
<code>struct cpumask cpumask_allocation</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long unsigned int pinned_vm</code> ➡️ <code>atomic64_t pinned_vm</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct hmm *hmm</code>
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
<code>struct rw_semaphore mmap_lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct mmu_notifier_subscriptions *notifier_subscriptions</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rw_semaphore mmap_sem</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mmu_notifier_mm *mmu_notifier_mm</code>
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
<code>atomic_t has_pinned</code>
</li>
<li>
<b>Field added. </b>
<code>seqcount_t write_protect_seq</code>
</li>
<li>
<b>Field added. </b>
<code>u32 pasid</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>atomic_t has_pinned</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int saved_auxv[46]</code> ➡️ <code>long unsigned int saved_auxv[48]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int ksm_merging_pages</code>
</li>
<li>
<b>Field removed. </b>
<code>struct core_state *core_state</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool tlb_flush_batched</code> ➡️ <code>atomic_t tlb_flush_batched</code>
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
<code>struct maple_tree mm_mt</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int ksm_rmap_items</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) lru_gen</code>
</li>
<li>
<b>Field removed. </b>
<code>struct vm_area_struct *mmap</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rb_root mm_rb</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 vmacache_seqnum</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int highest_vm_end</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct mm_rss_stat rss_stat</code> ➡️ <code>struct percpu_counter rss_stat[4]</code>
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
<code>struct mm_cid *pcpu_cid</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int mm_cid_next_scan</code>
</li>
<li>
<b>Field added. </b>
<code>int mm_lock_seq</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int saved_auxv[48]</code> ➡️ <code>long unsigned int saved_auxv[52]</code>
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
<code>struct iommu_mm_data *iommu_mm</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int ksm_zero_pages</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 pasid</code>
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
<b>Field removed. </b>
<code>long unsigned int mmap_compat_base</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int mmap_compat_legacy_base</code>
</li>
<li>
<b>Field removed. </b>
<code>bool tlb_flush_batched</code>
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
<code>long unsigned int mmap_compat_base</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int mmap_compat_legacy_base</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int numa_next_scan</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int numa_scan_offset</code>
</li>
<li>
<b>Field removed. </b>
<code>int numa_scan_seq</code>
</li>
<li>
<b>Field removed. </b>
<code>bool tlb_flush_batched</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_long_t hugetlb_usage</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int saved_auxv[46]</code> ➡️ <code>long unsigned int saved_auxv[42]</code>
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
<code>long unsigned int mmap_compat_base</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int mmap_compat_legacy_base</code>
</li>
<li>
<b>Field removed. </b>
<code>bool tlb_flush_batched</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int saved_auxv[46]</code> ➡️ <code>long unsigned int saved_auxv[70]</code>
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
<code>long unsigned int mmap_compat_base</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int mmap_compat_legacy_base</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int numa_next_scan</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int numa_scan_offset</code>
</li>
<li>
<b>Field removed. </b>
<code>int numa_scan_seq</code>
</li>
<li>
<b>Field removed. </b>
<code>bool tlb_flush_batched</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int saved_auxv[46]</code> ➡️ <code>long unsigned int saved_auxv[42]</code>
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
