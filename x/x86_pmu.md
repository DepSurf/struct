# Struct: <code>x86_pmu</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct x86_pmu {
    const char *name;
    int version;
    int (*handle_irq)(struct pt_regs *);
    void (*disable_all)();
    void (*enable_all)(int);
    void (*enable)(struct perf_event *);
    void (*disable)(struct perf_event *);
    int (*hw_config)(struct perf_event *);
    int (*schedule_events)(struct cpu_hw_events *, int, int *);
    unsigned int eventsel;
    unsigned int perfctr;
    int (*addr_offset)(int, bool);
    int (*rdpmc_index)(int);
    u64 (*event_map)(int);
    int max_events;
    int num_counters;
    int num_counters_fixed;
    int cntval_bits;
    u64 cntval_mask;
    long unsigned int events_maskl;
    long unsigned int events_mask[1];
    int events_mask_len;
    int apic;
    u64 max_period;
    struct event_constraint * (*get_event_constraints)(struct cpu_hw_events *, int, struct perf_event *);
    void (*put_event_constraints)(struct cpu_hw_events *, struct perf_event *);
    void (*start_scheduling)(struct cpu_hw_events *);
    void (*commit_scheduling)(struct cpu_hw_events *, int, int);
    void (*stop_scheduling)(struct cpu_hw_events *);
    struct event_constraint *event_constraints;
    struct x86_pmu_quirk *quirks;
    int perfctr_second_write;
    bool late_ack;
    unsigned int (*limit_period)(struct perf_event *, unsigned int);
    int attr_rdpmc_broken;
    int attr_rdpmc;
    struct attribute **format_attrs;
    struct attribute **event_attrs;
    ssize_t (*events_sysfs_show)(char *, u64);
    struct attribute **cpu_events;
    int (*cpu_prepare)(int);
    void (*cpu_starting)(int);
    void (*cpu_dying)(int);
    void (*cpu_dead)(int);
    void (*check_microcode)();
    void (*sched_task)(struct perf_event_context *, bool);
    u64 intel_ctrl;
    union perf_capabilities intel_cap;
    unsigned int bts;
    unsigned int bts_active;
    unsigned int pebs;
    unsigned int pebs_active;
    unsigned int pebs_broken;
    int pebs_record_size;
    int pebs_buffer_size;
    void (*drain_pebs)(struct pt_regs *);
    struct event_constraint *pebs_constraints;
    void (*pebs_aliases)(struct perf_event *);
    int max_pebs_events;
    long unsigned int free_running_flags;
    long unsigned int lbr_tos;
    long unsigned int lbr_from;
    long unsigned int lbr_to;
    int lbr_nr;
    u64 lbr_sel_mask;
    const int *lbr_sel_map;
    bool lbr_double_abort;
    atomic_t lbr_exclusive[3];
    struct extra_reg *extra_regs;
    unsigned int flags;
    struct perf_guest_switch_msr * (*guest_get_msrs)(int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct x86_pmu {
    const char *name;
    int version;
    int (*handle_irq)(struct pt_regs *);
    void (*disable_all)();
    void (*enable_all)(int);
    void (*enable)(struct perf_event *);
    void (*disable)(struct perf_event *);
    int (*hw_config)(struct perf_event *);
    int (*schedule_events)(struct cpu_hw_events *, int, int *);
    unsigned int eventsel;
    unsigned int perfctr;
    int (*addr_offset)(int, bool);
    int (*rdpmc_index)(int);
    u64 (*event_map)(int);
    int max_events;
    int num_counters;
    int num_counters_fixed;
    int cntval_bits;
    u64 cntval_mask;
    long unsigned int events_maskl;
    long unsigned int events_mask[1];
    int events_mask_len;
    int apic;
    u64 max_period;
    struct event_constraint * (*get_event_constraints)(struct cpu_hw_events *, int, struct perf_event *);
    void (*put_event_constraints)(struct cpu_hw_events *, struct perf_event *);
    void (*start_scheduling)(struct cpu_hw_events *);
    void (*commit_scheduling)(struct cpu_hw_events *, int, int);
    void (*stop_scheduling)(struct cpu_hw_events *);
    struct event_constraint *event_constraints;
    struct x86_pmu_quirk *quirks;
    int perfctr_second_write;
    bool late_ack;
    unsigned int (*limit_period)(struct perf_event *, unsigned int);
    int attr_rdpmc_broken;
    int attr_rdpmc;
    struct attribute **format_attrs;
    struct attribute **event_attrs;
    ssize_t (*events_sysfs_show)(char *, u64);
    struct attribute **cpu_events;
    int (*cpu_prepare)(int);
    void (*cpu_starting)(int);
    void (*cpu_dying)(int);
    void (*cpu_dead)(int);
    void (*check_microcode)();
    void (*sched_task)(struct perf_event_context *, bool);
    u64 intel_ctrl;
    union perf_capabilities intel_cap;
    unsigned int bts;
    unsigned int bts_active;
    unsigned int pebs;
    unsigned int pebs_active;
    unsigned int pebs_broken;
    unsigned int pebs_prec_dist;
    int pebs_record_size;
    int pebs_buffer_size;
    void (*drain_pebs)(struct pt_regs *);
    struct event_constraint *pebs_constraints;
    void (*pebs_aliases)(struct perf_event *);
    int max_pebs_events;
    long unsigned int free_running_flags;
    long unsigned int lbr_tos;
    long unsigned int lbr_from;
    long unsigned int lbr_to;
    int lbr_nr;
    u64 lbr_sel_mask;
    const int *lbr_sel_map;
    bool lbr_double_abort;
    bool lbr_pt_coexist;
    atomic_t lbr_exclusive[3];
    unsigned int amd_nb_constraints;
    struct extra_reg *extra_regs;
    unsigned int flags;
    struct perf_guest_switch_msr * (*guest_get_msrs)(int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct x86_pmu {
    const char *name;
    int version;
    int (*handle_irq)(struct pt_regs *);
    void (*disable_all)();
    void (*enable_all)(int);
    void (*enable)(struct perf_event *);
    void (*disable)(struct perf_event *);
    void (*add)(struct perf_event *);
    void (*del)(struct perf_event *);
    int (*hw_config)(struct perf_event *);
    int (*schedule_events)(struct cpu_hw_events *, int, int *);
    unsigned int eventsel;
    unsigned int perfctr;
    int (*addr_offset)(int, bool);
    int (*rdpmc_index)(int);
    u64 (*event_map)(int);
    int max_events;
    int num_counters;
    int num_counters_fixed;
    int cntval_bits;
    u64 cntval_mask;
    long unsigned int events_maskl;
    long unsigned int events_mask[1];
    int events_mask_len;
    int apic;
    u64 max_period;
    struct event_constraint * (*get_event_constraints)(struct cpu_hw_events *, int, struct perf_event *);
    void (*put_event_constraints)(struct cpu_hw_events *, struct perf_event *);
    void (*start_scheduling)(struct cpu_hw_events *);
    void (*commit_scheduling)(struct cpu_hw_events *, int, int);
    void (*stop_scheduling)(struct cpu_hw_events *);
    struct event_constraint *event_constraints;
    struct x86_pmu_quirk *quirks;
    int perfctr_second_write;
    bool late_ack;
    unsigned int (*limit_period)(struct perf_event *, unsigned int);
    int attr_rdpmc_broken;
    int attr_rdpmc;
    struct attribute **format_attrs;
    struct attribute **event_attrs;
    ssize_t (*events_sysfs_show)(char *, u64);
    struct attribute **cpu_events;
    int (*cpu_prepare)(int);
    void (*cpu_starting)(int);
    void (*cpu_dying)(int);
    void (*cpu_dead)(int);
    void (*check_microcode)();
    void (*sched_task)(struct perf_event_context *, bool);
    u64 intel_ctrl;
    union perf_capabilities intel_cap;
    unsigned int bts;
    unsigned int bts_active;
    unsigned int pebs;
    unsigned int pebs_active;
    unsigned int pebs_broken;
    unsigned int pebs_prec_dist;
    int pebs_record_size;
    int pebs_buffer_size;
    void (*drain_pebs)(struct pt_regs *);
    struct event_constraint *pebs_constraints;
    void (*pebs_aliases)(struct perf_event *);
    int max_pebs_events;
    long unsigned int free_running_flags;
    long unsigned int lbr_tos;
    long unsigned int lbr_from;
    long unsigned int lbr_to;
    int lbr_nr;
    u64 lbr_sel_mask;
    const int *lbr_sel_map;
    bool lbr_double_abort;
    bool lbr_pt_coexist;
    atomic_t lbr_exclusive[3];
    unsigned int amd_nb_constraints;
    struct extra_reg *extra_regs;
    unsigned int flags;
    struct perf_guest_switch_msr * (*guest_get_msrs)(int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct x86_pmu {
    const char *name;
    int version;
    int (*handle_irq)(struct pt_regs *);
    void (*disable_all)();
    void (*enable_all)(int);
    void (*enable)(struct perf_event *);
    void (*disable)(struct perf_event *);
    void (*add)(struct perf_event *);
    void (*del)(struct perf_event *);
    int (*hw_config)(struct perf_event *);
    int (*schedule_events)(struct cpu_hw_events *, int, int *);
    unsigned int eventsel;
    unsigned int perfctr;
    int (*addr_offset)(int, bool);
    int (*rdpmc_index)(int);
    u64 (*event_map)(int);
    int max_events;
    int num_counters;
    int num_counters_fixed;
    int cntval_bits;
    u64 cntval_mask;
    long unsigned int events_maskl;
    long unsigned int events_mask[1];
    int events_mask_len;
    int apic;
    u64 max_period;
    struct event_constraint * (*get_event_constraints)(struct cpu_hw_events *, int, struct perf_event *);
    void (*put_event_constraints)(struct cpu_hw_events *, struct perf_event *);
    void (*start_scheduling)(struct cpu_hw_events *);
    void (*commit_scheduling)(struct cpu_hw_events *, int, int);
    void (*stop_scheduling)(struct cpu_hw_events *);
    struct event_constraint *event_constraints;
    struct x86_pmu_quirk *quirks;
    int perfctr_second_write;
    bool late_ack;
    unsigned int (*limit_period)(struct perf_event *, unsigned int);
    int attr_rdpmc_broken;
    int attr_rdpmc;
    struct attribute **format_attrs;
    struct attribute **event_attrs;
    ssize_t (*events_sysfs_show)(char *, u64);
    struct attribute **cpu_events;
    long unsigned int attr_freeze_on_smi;
    struct attribute **attrs;
    int (*cpu_prepare)(int);
    void (*cpu_starting)(int);
    void (*cpu_dying)(int);
    void (*cpu_dead)(int);
    void (*check_microcode)();
    void (*sched_task)(struct perf_event_context *, bool);
    u64 intel_ctrl;
    union perf_capabilities intel_cap;
    unsigned int bts;
    unsigned int bts_active;
    unsigned int pebs;
    unsigned int pebs_active;
    unsigned int pebs_broken;
    unsigned int pebs_prec_dist;
    unsigned int pebs_no_tlb;
    int pebs_record_size;
    int pebs_buffer_size;
    void (*drain_pebs)(struct pt_regs *);
    struct event_constraint *pebs_constraints;
    void (*pebs_aliases)(struct perf_event *);
    int max_pebs_events;
    long unsigned int free_running_flags;
    long unsigned int lbr_tos;
    long unsigned int lbr_from;
    long unsigned int lbr_to;
    int lbr_nr;
    u64 lbr_sel_mask;
    const int *lbr_sel_map;
    bool lbr_double_abort;
    bool lbr_pt_coexist;
    atomic_t lbr_exclusive[3];
    unsigned int amd_nb_constraints;
    struct extra_reg *extra_regs;
    unsigned int flags;
    struct perf_guest_switch_msr * (*guest_get_msrs)(int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct x86_pmu {
    const char *name;
    int version;
    int (*handle_irq)(struct pt_regs *);
    void (*disable_all)();
    void (*enable_all)(int);
    void (*enable)(struct perf_event *);
    void (*disable)(struct perf_event *);
    void (*add)(struct perf_event *);
    void (*del)(struct perf_event *);
    int (*hw_config)(struct perf_event *);
    int (*schedule_events)(struct cpu_hw_events *, int, int *);
    unsigned int eventsel;
    unsigned int perfctr;
    int (*addr_offset)(int, bool);
    int (*rdpmc_index)(int);
    u64 (*event_map)(int);
    int max_events;
    int num_counters;
    int num_counters_fixed;
    int cntval_bits;
    u64 cntval_mask;
    long unsigned int events_maskl;
    long unsigned int events_mask[1];
    int events_mask_len;
    int apic;
    u64 max_period;
    struct event_constraint * (*get_event_constraints)(struct cpu_hw_events *, int, struct perf_event *);
    void (*put_event_constraints)(struct cpu_hw_events *, struct perf_event *);
    void (*start_scheduling)(struct cpu_hw_events *);
    void (*commit_scheduling)(struct cpu_hw_events *, int, int);
    void (*stop_scheduling)(struct cpu_hw_events *);
    struct event_constraint *event_constraints;
    struct x86_pmu_quirk *quirks;
    int perfctr_second_write;
    bool late_ack;
    unsigned int (*limit_period)(struct perf_event *, unsigned int);
    int attr_rdpmc_broken;
    int attr_rdpmc;
    struct attribute **format_attrs;
    struct attribute **event_attrs;
    struct attribute **caps_attrs;
    ssize_t (*events_sysfs_show)(char *, u64);
    struct attribute **cpu_events;
    long unsigned int attr_freeze_on_smi;
    struct attribute **attrs;
    int (*cpu_prepare)(int);
    void (*cpu_starting)(int);
    void (*cpu_dying)(int);
    void (*cpu_dead)(int);
    void (*check_microcode)();
    void (*sched_task)(struct perf_event_context *, bool);
    u64 intel_ctrl;
    union perf_capabilities intel_cap;
    unsigned int bts;
    unsigned int bts_active;
    unsigned int pebs;
    unsigned int pebs_active;
    unsigned int pebs_broken;
    unsigned int pebs_prec_dist;
    unsigned int pebs_no_tlb;
    int pebs_record_size;
    int pebs_buffer_size;
    void (*drain_pebs)(struct pt_regs *);
    struct event_constraint *pebs_constraints;
    void (*pebs_aliases)(struct perf_event *);
    int max_pebs_events;
    long unsigned int free_running_flags;
    long unsigned int lbr_tos;
    long unsigned int lbr_from;
    long unsigned int lbr_to;
    int lbr_nr;
    u64 lbr_sel_mask;
    const int *lbr_sel_map;
    bool lbr_double_abort;
    bool lbr_pt_coexist;
    atomic_t lbr_exclusive[3];
    unsigned int amd_nb_constraints;
    struct extra_reg *extra_regs;
    unsigned int flags;
    struct perf_guest_switch_msr * (*guest_get_msrs)(int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct x86_pmu {
    const char *name;
    int version;
    int (*handle_irq)(struct pt_regs *);
    void (*disable_all)();
    void (*enable_all)(int);
    void (*enable)(struct perf_event *);
    void (*disable)(struct perf_event *);
    void (*add)(struct perf_event *);
    void (*del)(struct perf_event *);
    void (*read)(struct perf_event *);
    int (*hw_config)(struct perf_event *);
    int (*schedule_events)(struct cpu_hw_events *, int, int *);
    unsigned int eventsel;
    unsigned int perfctr;
    int (*addr_offset)(int, bool);
    int (*rdpmc_index)(int);
    u64 (*event_map)(int);
    int max_events;
    int num_counters;
    int num_counters_fixed;
    int cntval_bits;
    u64 cntval_mask;
    long unsigned int events_maskl;
    long unsigned int events_mask[1];
    int events_mask_len;
    int apic;
    u64 max_period;
    struct event_constraint * (*get_event_constraints)(struct cpu_hw_events *, int, struct perf_event *);
    void (*put_event_constraints)(struct cpu_hw_events *, struct perf_event *);
    void (*start_scheduling)(struct cpu_hw_events *);
    void (*commit_scheduling)(struct cpu_hw_events *, int, int);
    void (*stop_scheduling)(struct cpu_hw_events *);
    struct event_constraint *event_constraints;
    struct x86_pmu_quirk *quirks;
    int perfctr_second_write;
    bool late_ack;
    u64 (*limit_period)(struct perf_event *, u64);
    int attr_rdpmc_broken;
    int attr_rdpmc;
    struct attribute **format_attrs;
    struct attribute **event_attrs;
    struct attribute **caps_attrs;
    ssize_t (*events_sysfs_show)(char *, u64);
    struct attribute **cpu_events;
    long unsigned int attr_freeze_on_smi;
    struct attribute **attrs;
    int (*cpu_prepare)(int);
    void (*cpu_starting)(int);
    void (*cpu_dying)(int);
    void (*cpu_dead)(int);
    void (*check_microcode)();
    void (*sched_task)(struct perf_event_context *, bool);
    u64 intel_ctrl;
    union perf_capabilities intel_cap;
    unsigned int bts;
    unsigned int bts_active;
    unsigned int pebs;
    unsigned int pebs_active;
    unsigned int pebs_broken;
    unsigned int pebs_prec_dist;
    unsigned int pebs_no_tlb;
    int pebs_record_size;
    int pebs_buffer_size;
    void (*drain_pebs)(struct pt_regs *);
    struct event_constraint *pebs_constraints;
    void (*pebs_aliases)(struct perf_event *);
    int max_pebs_events;
    long unsigned int large_pebs_flags;
    long unsigned int lbr_tos;
    long unsigned int lbr_from;
    long unsigned int lbr_to;
    int lbr_nr;
    u64 lbr_sel_mask;
    const int *lbr_sel_map;
    bool lbr_double_abort;
    bool lbr_pt_coexist;
    atomic_t lbr_exclusive[3];
    unsigned int amd_nb_constraints;
    struct extra_reg *extra_regs;
    unsigned int flags;
    struct perf_guest_switch_msr * (*guest_get_msrs)(int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct x86_pmu {
    const char *name;
    int version;
    int (*handle_irq)(struct pt_regs *);
    void (*disable_all)();
    void (*enable_all)(int);
    void (*enable)(struct perf_event *);
    void (*disable)(struct perf_event *);
    void (*add)(struct perf_event *);
    void (*del)(struct perf_event *);
    void (*read)(struct perf_event *);
    int (*hw_config)(struct perf_event *);
    int (*schedule_events)(struct cpu_hw_events *, int, int *);
    unsigned int eventsel;
    unsigned int perfctr;
    int (*addr_offset)(int, bool);
    int (*rdpmc_index)(int);
    u64 (*event_map)(int);
    int max_events;
    int num_counters;
    int num_counters_fixed;
    int cntval_bits;
    u64 cntval_mask;
    long unsigned int events_maskl;
    long unsigned int events_mask[1];
    int events_mask_len;
    int apic;
    u64 max_period;
    struct event_constraint * (*get_event_constraints)(struct cpu_hw_events *, int, struct perf_event *);
    void (*put_event_constraints)(struct cpu_hw_events *, struct perf_event *);
    void (*start_scheduling)(struct cpu_hw_events *);
    void (*commit_scheduling)(struct cpu_hw_events *, int, int);
    void (*stop_scheduling)(struct cpu_hw_events *);
    struct event_constraint *event_constraints;
    struct x86_pmu_quirk *quirks;
    int perfctr_second_write;
    u64 (*limit_period)(struct perf_event *, u64);
    unsigned int late_ack;
    unsigned int counter_freezing;
    int attr_rdpmc_broken;
    int attr_rdpmc;
    struct attribute **format_attrs;
    struct attribute **event_attrs;
    struct attribute **caps_attrs;
    ssize_t (*events_sysfs_show)(char *, u64);
    struct attribute **cpu_events;
    long unsigned int attr_freeze_on_smi;
    struct attribute **attrs;
    int (*cpu_prepare)(int);
    void (*cpu_starting)(int);
    void (*cpu_dying)(int);
    void (*cpu_dead)(int);
    void (*check_microcode)();
    void (*sched_task)(struct perf_event_context *, bool);
    u64 intel_ctrl;
    union perf_capabilities intel_cap;
    unsigned int bts;
    unsigned int bts_active;
    unsigned int pebs;
    unsigned int pebs_active;
    unsigned int pebs_broken;
    unsigned int pebs_prec_dist;
    unsigned int pebs_no_tlb;
    int pebs_record_size;
    int pebs_buffer_size;
    void (*drain_pebs)(struct pt_regs *);
    struct event_constraint *pebs_constraints;
    void (*pebs_aliases)(struct perf_event *);
    int max_pebs_events;
    long unsigned int large_pebs_flags;
    long unsigned int lbr_tos;
    long unsigned int lbr_from;
    long unsigned int lbr_to;
    int lbr_nr;
    u64 lbr_sel_mask;
    const int *lbr_sel_map;
    bool lbr_double_abort;
    bool lbr_pt_coexist;
    atomic_t lbr_exclusive[3];
    unsigned int amd_nb_constraints;
    struct extra_reg *extra_regs;
    unsigned int flags;
    struct perf_guest_switch_msr * (*guest_get_msrs)(int *);
    int (*check_period)(struct perf_event *, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct x86_pmu {
    const char *name;
    int version;
    int (*handle_irq)(struct pt_regs *);
    void (*disable_all)();
    void (*enable_all)(int);
    void (*enable)(struct perf_event *);
    void (*disable)(struct perf_event *);
    void (*add)(struct perf_event *);
    void (*del)(struct perf_event *);
    void (*read)(struct perf_event *);
    int (*hw_config)(struct perf_event *);
    int (*schedule_events)(struct cpu_hw_events *, int, int *);
    unsigned int eventsel;
    unsigned int perfctr;
    int (*addr_offset)(int, bool);
    int (*rdpmc_index)(int);
    u64 (*event_map)(int);
    int max_events;
    int num_counters;
    int num_counters_fixed;
    int cntval_bits;
    u64 cntval_mask;
    long unsigned int events_maskl;
    long unsigned int events_mask[1];
    int events_mask_len;
    int apic;
    u64 max_period;
    struct event_constraint * (*get_event_constraints)(struct cpu_hw_events *, int, struct perf_event *);
    void (*put_event_constraints)(struct cpu_hw_events *, struct perf_event *);
    void (*start_scheduling)(struct cpu_hw_events *);
    void (*commit_scheduling)(struct cpu_hw_events *, int, int);
    void (*stop_scheduling)(struct cpu_hw_events *);
    struct event_constraint *event_constraints;
    struct x86_pmu_quirk *quirks;
    int perfctr_second_write;
    u64 (*limit_period)(struct perf_event *, u64);
    unsigned int late_ack;
    unsigned int counter_freezing;
    int attr_rdpmc_broken;
    int attr_rdpmc;
    struct attribute **format_attrs;
    ssize_t (*events_sysfs_show)(char *, u64);
    const struct attribute_group **attr_update;
    long unsigned int attr_freeze_on_smi;
    int (*cpu_prepare)(int);
    void (*cpu_starting)(int);
    void (*cpu_dying)(int);
    void (*cpu_dead)(int);
    void (*check_microcode)();
    void (*sched_task)(struct perf_event_context *, bool);
    u64 intel_ctrl;
    union perf_capabilities intel_cap;
    unsigned int bts;
    unsigned int bts_active;
    unsigned int pebs;
    unsigned int pebs_active;
    unsigned int pebs_broken;
    unsigned int pebs_prec_dist;
    unsigned int pebs_no_tlb;
    unsigned int pebs_no_isolation;
    int pebs_record_size;
    int pebs_buffer_size;
    int max_pebs_events;
    void (*drain_pebs)(struct pt_regs *);
    struct event_constraint *pebs_constraints;
    void (*pebs_aliases)(struct perf_event *);
    long unsigned int large_pebs_flags;
    u64 rtm_abort_event;
    long unsigned int lbr_tos;
    long unsigned int lbr_from;
    long unsigned int lbr_to;
    int lbr_nr;
    u64 lbr_sel_mask;
    const int *lbr_sel_map;
    bool lbr_double_abort;
    bool lbr_pt_coexist;
    atomic_t lbr_exclusive[3];
    unsigned int amd_nb_constraints;
    struct extra_reg *extra_regs;
    unsigned int flags;
    struct perf_guest_switch_msr * (*guest_get_msrs)(int *);
    int (*check_period)(struct perf_event *, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct x86_pmu {
    const char *name;
    int version;
    int (*handle_irq)(struct pt_regs *);
    void (*disable_all)();
    void (*enable_all)(int);
    void (*enable)(struct perf_event *);
    void (*disable)(struct perf_event *);
    void (*add)(struct perf_event *);
    void (*del)(struct perf_event *);
    void (*read)(struct perf_event *);
    int (*hw_config)(struct perf_event *);
    int (*schedule_events)(struct cpu_hw_events *, int, int *);
    unsigned int eventsel;
    unsigned int perfctr;
    int (*addr_offset)(int, bool);
    int (*rdpmc_index)(int);
    u64 (*event_map)(int);
    int max_events;
    int num_counters;
    int num_counters_fixed;
    int cntval_bits;
    u64 cntval_mask;
    long unsigned int events_maskl;
    long unsigned int events_mask[1];
    int events_mask_len;
    int apic;
    u64 max_period;
    struct event_constraint * (*get_event_constraints)(struct cpu_hw_events *, int, struct perf_event *);
    void (*put_event_constraints)(struct cpu_hw_events *, struct perf_event *);
    void (*start_scheduling)(struct cpu_hw_events *);
    void (*commit_scheduling)(struct cpu_hw_events *, int, int);
    void (*stop_scheduling)(struct cpu_hw_events *);
    struct event_constraint *event_constraints;
    struct x86_pmu_quirk *quirks;
    int perfctr_second_write;
    u64 (*limit_period)(struct perf_event *, u64);
    unsigned int late_ack;
    unsigned int counter_freezing;
    int attr_rdpmc_broken;
    int attr_rdpmc;
    struct attribute **format_attrs;
    ssize_t (*events_sysfs_show)(char *, u64);
    const struct attribute_group **attr_update;
    long unsigned int attr_freeze_on_smi;
    int (*cpu_prepare)(int);
    void (*cpu_starting)(int);
    void (*cpu_dying)(int);
    void (*cpu_dead)(int);
    void (*check_microcode)();
    void (*sched_task)(struct perf_event_context *, bool);
    u64 intel_ctrl;
    union perf_capabilities intel_cap;
    unsigned int bts;
    unsigned int bts_active;
    unsigned int pebs;
    unsigned int pebs_active;
    unsigned int pebs_broken;
    unsigned int pebs_prec_dist;
    unsigned int pebs_no_tlb;
    unsigned int pebs_no_isolation;
    int pebs_record_size;
    int pebs_buffer_size;
    int max_pebs_events;
    void (*drain_pebs)(struct pt_regs *);
    struct event_constraint *pebs_constraints;
    void (*pebs_aliases)(struct perf_event *);
    long unsigned int large_pebs_flags;
    u64 rtm_abort_event;
    long unsigned int lbr_tos;
    long unsigned int lbr_from;
    long unsigned int lbr_to;
    int lbr_nr;
    u64 lbr_sel_mask;
    const int *lbr_sel_map;
    bool lbr_double_abort;
    bool lbr_pt_coexist;
    atomic_t lbr_exclusive[3];
    unsigned int amd_nb_constraints;
    u64 perf_ctr_pair_en;
    struct extra_reg *extra_regs;
    unsigned int flags;
    struct perf_guest_switch_msr * (*guest_get_msrs)(int *);
    int (*check_period)(struct perf_event *, u64);
    int (*aux_output_match)(struct perf_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct x86_pmu {
    const char *name;
    int version;
    int (*handle_irq)(struct pt_regs *);
    void (*disable_all)();
    void (*enable_all)(int);
    void (*enable)(struct perf_event *);
    void (*disable)(struct perf_event *);
    void (*add)(struct perf_event *);
    void (*del)(struct perf_event *);
    void (*read)(struct perf_event *);
    int (*hw_config)(struct perf_event *);
    int (*schedule_events)(struct cpu_hw_events *, int, int *);
    unsigned int eventsel;
    unsigned int perfctr;
    int (*addr_offset)(int, bool);
    int (*rdpmc_index)(int);
    u64 (*event_map)(int);
    int max_events;
    int num_counters;
    int num_counters_fixed;
    int cntval_bits;
    u64 cntval_mask;
    long unsigned int events_maskl;
    long unsigned int events_mask[1];
    int events_mask_len;
    int apic;
    u64 max_period;
    struct event_constraint * (*get_event_constraints)(struct cpu_hw_events *, int, struct perf_event *);
    void (*put_event_constraints)(struct cpu_hw_events *, struct perf_event *);
    void (*start_scheduling)(struct cpu_hw_events *);
    void (*commit_scheduling)(struct cpu_hw_events *, int, int);
    void (*stop_scheduling)(struct cpu_hw_events *);
    struct event_constraint *event_constraints;
    struct x86_pmu_quirk *quirks;
    int perfctr_second_write;
    u64 (*limit_period)(struct perf_event *, u64);
    unsigned int late_ack;
    unsigned int enabled_ack;
    unsigned int counter_freezing;
    int attr_rdpmc_broken;
    int attr_rdpmc;
    struct attribute **format_attrs;
    ssize_t (*events_sysfs_show)(char *, u64);
    const struct attribute_group **attr_update;
    long unsigned int attr_freeze_on_smi;
    int (*cpu_prepare)(int);
    void (*cpu_starting)(int);
    void (*cpu_dying)(int);
    void (*cpu_dead)(int);
    void (*check_microcode)();
    void (*sched_task)(struct perf_event_context *, bool);
    u64 intel_ctrl;
    union perf_capabilities intel_cap;
    unsigned int bts;
    unsigned int bts_active;
    unsigned int pebs;
    unsigned int pebs_active;
    unsigned int pebs_broken;
    unsigned int pebs_prec_dist;
    unsigned int pebs_no_tlb;
    unsigned int pebs_no_isolation;
    int pebs_record_size;
    int pebs_buffer_size;
    int max_pebs_events;
    void (*drain_pebs)(struct pt_regs *);
    struct event_constraint *pebs_constraints;
    void (*pebs_aliases)(struct perf_event *);
    long unsigned int large_pebs_flags;
    u64 rtm_abort_event;
    long unsigned int lbr_tos;
    long unsigned int lbr_from;
    long unsigned int lbr_to;
    int lbr_nr;
    u64 lbr_sel_mask;
    const int *lbr_sel_map;
    bool lbr_double_abort;
    bool lbr_pt_coexist;
    atomic_t lbr_exclusive[3];
    void (*swap_task_ctx)(struct perf_event_context *, struct perf_event_context *);
    unsigned int amd_nb_constraints;
    u64 perf_ctr_pair_en;
    struct extra_reg *extra_regs;
    unsigned int flags;
    struct perf_guest_switch_msr * (*guest_get_msrs)(int *);
    int (*check_period)(struct perf_event *, u64);
    int (*aux_output_match)(struct perf_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct x86_pmu {
    const char *name;
    int version;
    int (*handle_irq)(struct pt_regs *);
    void (*disable_all)();
    void (*enable_all)(int);
    void (*enable)(struct perf_event *);
    void (*disable)(struct perf_event *);
    void (*add)(struct perf_event *);
    void (*del)(struct perf_event *);
    void (*read)(struct perf_event *);
    int (*hw_config)(struct perf_event *);
    int (*schedule_events)(struct cpu_hw_events *, int, int *);
    unsigned int eventsel;
    unsigned int perfctr;
    int (*addr_offset)(int, bool);
    int (*rdpmc_index)(int);
    u64 (*event_map)(int);
    int max_events;
    int num_counters;
    int num_counters_fixed;
    int cntval_bits;
    u64 cntval_mask;
    long unsigned int events_maskl;
    long unsigned int events_mask[1];
    int events_mask_len;
    int apic;
    u64 max_period;
    struct event_constraint * (*get_event_constraints)(struct cpu_hw_events *, int, struct perf_event *);
    void (*put_event_constraints)(struct cpu_hw_events *, struct perf_event *);
    void (*start_scheduling)(struct cpu_hw_events *);
    void (*commit_scheduling)(struct cpu_hw_events *, int, int);
    void (*stop_scheduling)(struct cpu_hw_events *);
    struct event_constraint *event_constraints;
    struct x86_pmu_quirk *quirks;
    int perfctr_second_write;
    u64 (*limit_period)(struct perf_event *, u64);
    unsigned int late_ack;
    unsigned int enabled_ack;
    unsigned int counter_freezing;
    int attr_rdpmc_broken;
    int attr_rdpmc;
    struct attribute **format_attrs;
    ssize_t (*events_sysfs_show)(char *, u64);
    const struct attribute_group **attr_update;
    long unsigned int attr_freeze_on_smi;
    int (*cpu_prepare)(int);
    void (*cpu_starting)(int);
    void (*cpu_dying)(int);
    void (*cpu_dead)(int);
    void (*check_microcode)();
    void (*sched_task)(struct perf_event_context *, bool);
    u64 intel_ctrl;
    union perf_capabilities intel_cap;
    unsigned int bts;
    unsigned int bts_active;
    unsigned int pebs;
    unsigned int pebs_active;
    unsigned int pebs_broken;
    unsigned int pebs_prec_dist;
    unsigned int pebs_no_tlb;
    unsigned int pebs_no_isolation;
    int pebs_record_size;
    int pebs_buffer_size;
    int max_pebs_events;
    void (*drain_pebs)(struct pt_regs *, struct perf_sample_data *);
    struct event_constraint *pebs_constraints;
    void (*pebs_aliases)(struct perf_event *);
    long unsigned int large_pebs_flags;
    u64 rtm_abort_event;
    unsigned int lbr_tos;
    unsigned int lbr_from;
    unsigned int lbr_to;
    unsigned int lbr_info;
    unsigned int lbr_nr;
    u64 lbr_sel_mask;
    u64 lbr_ctl_mask;
    const int *lbr_sel_map;
    int *lbr_ctl_map;
    bool lbr_double_abort;
    bool lbr_pt_coexist;
    unsigned int lbr_depth_mask;
    unsigned int lbr_deep_c_reset;
    unsigned int lbr_lip;
    unsigned int lbr_cpl;
    unsigned int lbr_filter;
    unsigned int lbr_call_stack;
    unsigned int lbr_mispred;
    unsigned int lbr_timed_lbr;
    unsigned int lbr_br_type;
    void (*lbr_reset)();
    void (*lbr_read)(struct cpu_hw_events *);
    void (*lbr_save)(void *);
    void (*lbr_restore)(void *);
    atomic_t lbr_exclusive[3];
    u64 (*update_topdown_event)(struct perf_event *);
    int (*set_topdown_event_period)(struct perf_event *);
    void (*swap_task_ctx)(struct perf_event_context *, struct perf_event_context *);
    unsigned int amd_nb_constraints;
    u64 perf_ctr_pair_en;
    struct extra_reg *extra_regs;
    unsigned int flags;
    struct perf_guest_switch_msr * (*guest_get_msrs)(int *);
    int (*check_period)(struct perf_event *, u64);
    int (*aux_output_match)(struct perf_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct x86_pmu {
    const char *name;
    int version;
    int (*handle_irq)(struct pt_regs *);
    void (*disable_all)();
    void (*enable_all)(int);
    void (*enable)(struct perf_event *);
    void (*disable)(struct perf_event *);
    void (*add)(struct perf_event *);
    void (*del)(struct perf_event *);
    void (*read)(struct perf_event *);
    int (*hw_config)(struct perf_event *);
    int (*schedule_events)(struct cpu_hw_events *, int, int *);
    unsigned int eventsel;
    unsigned int perfctr;
    int (*addr_offset)(int, bool);
    int (*rdpmc_index)(int);
    u64 (*event_map)(int);
    int max_events;
    int num_counters;
    int num_counters_fixed;
    int cntval_bits;
    u64 cntval_mask;
    long unsigned int events_maskl;
    long unsigned int events_mask[1];
    int events_mask_len;
    int apic;
    u64 max_period;
    struct event_constraint * (*get_event_constraints)(struct cpu_hw_events *, int, struct perf_event *);
    void (*put_event_constraints)(struct cpu_hw_events *, struct perf_event *);
    void (*start_scheduling)(struct cpu_hw_events *);
    void (*commit_scheduling)(struct cpu_hw_events *, int, int);
    void (*stop_scheduling)(struct cpu_hw_events *);
    struct event_constraint *event_constraints;
    struct x86_pmu_quirk *quirks;
    int perfctr_second_write;
    u64 (*limit_period)(struct perf_event *, u64);
    unsigned int late_ack;
    unsigned int mid_ack;
    unsigned int enabled_ack;
    int attr_rdpmc_broken;
    int attr_rdpmc;
    struct attribute **format_attrs;
    ssize_t (*events_sysfs_show)(char *, u64);
    const struct attribute_group **attr_update;
    long unsigned int attr_freeze_on_smi;
    int (*cpu_prepare)(int);
    void (*cpu_starting)(int);
    void (*cpu_dying)(int);
    void (*cpu_dead)(int);
    void (*check_microcode)();
    void (*sched_task)(struct perf_event_context *, bool);
    u64 intel_ctrl;
    union perf_capabilities intel_cap;
    unsigned int bts;
    unsigned int bts_active;
    unsigned int pebs;
    unsigned int pebs_active;
    unsigned int pebs_broken;
    unsigned int pebs_prec_dist;
    unsigned int pebs_no_tlb;
    unsigned int pebs_no_isolation;
    unsigned int pebs_block;
    int pebs_record_size;
    int pebs_buffer_size;
    int max_pebs_events;
    void (*drain_pebs)(struct pt_regs *, struct perf_sample_data *);
    struct event_constraint *pebs_constraints;
    void (*pebs_aliases)(struct perf_event *);
    long unsigned int large_pebs_flags;
    u64 rtm_abort_event;
    unsigned int lbr_tos;
    unsigned int lbr_from;
    unsigned int lbr_to;
    unsigned int lbr_info;
    unsigned int lbr_nr;
    u64 lbr_sel_mask;
    u64 lbr_ctl_mask;
    const int *lbr_sel_map;
    int *lbr_ctl_map;
    bool lbr_double_abort;
    bool lbr_pt_coexist;
    unsigned int lbr_depth_mask;
    unsigned int lbr_deep_c_reset;
    unsigned int lbr_lip;
    unsigned int lbr_cpl;
    unsigned int lbr_filter;
    unsigned int lbr_call_stack;
    unsigned int lbr_mispred;
    unsigned int lbr_timed_lbr;
    unsigned int lbr_br_type;
    void (*lbr_reset)();
    void (*lbr_read)(struct cpu_hw_events *);
    void (*lbr_save)(void *);
    void (*lbr_restore)(void *);
    atomic_t lbr_exclusive[3];
    int num_topdown_events;
    u64 (*update_topdown_event)(struct perf_event *);
    int (*set_topdown_event_period)(struct perf_event *);
    void (*swap_task_ctx)(struct perf_event_context *, struct perf_event_context *);
    unsigned int amd_nb_constraints;
    u64 perf_ctr_pair_en;
    struct extra_reg *extra_regs;
    unsigned int flags;
    struct perf_guest_switch_msr * (*guest_get_msrs)(int *);
    int (*check_period)(struct perf_event *, u64);
    int (*aux_output_match)(struct perf_event *);
    int (*filter_match)(struct perf_event *);
    int num_hybrid_pmus;
    struct x86_hybrid_pmu *hybrid_pmu;
    u8 (*get_hybrid_cpu_type)();
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct x86_pmu {
    const char *name;
    int version;
    int (*handle_irq)(struct pt_regs *);
    void (*disable_all)();
    void (*enable_all)(int);
    void (*enable)(struct perf_event *);
    void (*disable)(struct perf_event *);
    void (*add)(struct perf_event *);
    void (*del)(struct perf_event *);
    void (*read)(struct perf_event *);
    int (*hw_config)(struct perf_event *);
    int (*schedule_events)(struct cpu_hw_events *, int, int *);
    unsigned int eventsel;
    unsigned int perfctr;
    int (*addr_offset)(int, bool);
    int (*rdpmc_index)(int);
    u64 (*event_map)(int);
    int max_events;
    int num_counters;
    int num_counters_fixed;
    int cntval_bits;
    u64 cntval_mask;
    long unsigned int events_maskl;
    long unsigned int events_mask[1];
    int events_mask_len;
    int apic;
    u64 max_period;
    struct event_constraint * (*get_event_constraints)(struct cpu_hw_events *, int, struct perf_event *);
    void (*put_event_constraints)(struct cpu_hw_events *, struct perf_event *);
    void (*start_scheduling)(struct cpu_hw_events *);
    void (*commit_scheduling)(struct cpu_hw_events *, int, int);
    void (*stop_scheduling)(struct cpu_hw_events *);
    struct event_constraint *event_constraints;
    struct x86_pmu_quirk *quirks;
    int perfctr_second_write;
    u64 (*limit_period)(struct perf_event *, u64);
    unsigned int late_ack;
    unsigned int mid_ack;
    unsigned int enabled_ack;
    int attr_rdpmc_broken;
    int attr_rdpmc;
    struct attribute **format_attrs;
    ssize_t (*events_sysfs_show)(char *, u64);
    const struct attribute_group **attr_update;
    long unsigned int attr_freeze_on_smi;
    int (*cpu_prepare)(int);
    void (*cpu_starting)(int);
    void (*cpu_dying)(int);
    void (*cpu_dead)(int);
    void (*check_microcode)();
    void (*sched_task)(struct perf_event_context *, bool);
    u64 intel_ctrl;
    union perf_capabilities intel_cap;
    unsigned int bts;
    unsigned int bts_active;
    unsigned int pebs;
    unsigned int pebs_active;
    unsigned int pebs_broken;
    unsigned int pebs_prec_dist;
    unsigned int pebs_no_tlb;
    unsigned int pebs_no_isolation;
    unsigned int pebs_block;
    int pebs_record_size;
    int pebs_buffer_size;
    int max_pebs_events;
    void (*drain_pebs)(struct pt_regs *, struct perf_sample_data *);
    struct event_constraint *pebs_constraints;
    void (*pebs_aliases)(struct perf_event *);
    long unsigned int large_pebs_flags;
    u64 rtm_abort_event;
    unsigned int lbr_tos;
    unsigned int lbr_from;
    unsigned int lbr_to;
    unsigned int lbr_info;
    unsigned int lbr_nr;
    u64 lbr_sel_mask;
    u64 lbr_ctl_mask;
    const int *lbr_sel_map;
    int *lbr_ctl_map;
    bool lbr_double_abort;
    bool lbr_pt_coexist;
    unsigned int lbr_depth_mask;
    unsigned int lbr_deep_c_reset;
    unsigned int lbr_lip;
    unsigned int lbr_cpl;
    unsigned int lbr_filter;
    unsigned int lbr_call_stack;
    unsigned int lbr_mispred;
    unsigned int lbr_timed_lbr;
    unsigned int lbr_br_type;
    void (*lbr_reset)();
    void (*lbr_read)(struct cpu_hw_events *);
    void (*lbr_save)(void *);
    void (*lbr_restore)(void *);
    atomic_t lbr_exclusive[3];
    int num_topdown_events;
    u64 (*update_topdown_event)(struct perf_event *);
    int (*set_topdown_event_period)(struct perf_event *);
    void (*swap_task_ctx)(struct perf_event_context *, struct perf_event_context *);
    unsigned int amd_nb_constraints;
    u64 perf_ctr_pair_en;
    struct extra_reg *extra_regs;
    unsigned int flags;
    struct perf_guest_switch_msr * (*guest_get_msrs)(int *);
    int (*check_period)(struct perf_event *, u64);
    int (*aux_output_match)(struct perf_event *);
    int (*filter_match)(struct perf_event *);
    int num_hybrid_pmus;
    struct x86_hybrid_pmu *hybrid_pmu;
    u8 (*get_hybrid_cpu_type)();
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct x86_pmu {
    const char *name;
    int version;
    int (*handle_irq)(struct pt_regs *);
    void (*disable_all)();
    void (*enable_all)(int);
    void (*enable)(struct perf_event *);
    void (*disable)(struct perf_event *);
    void (*assign)(struct perf_event *, int);
    void (*add)(struct perf_event *);
    void (*del)(struct perf_event *);
    void (*read)(struct perf_event *);
    int (*hw_config)(struct perf_event *);
    int (*schedule_events)(struct cpu_hw_events *, int, int *);
    unsigned int eventsel;
    unsigned int perfctr;
    int (*addr_offset)(int, bool);
    int (*rdpmc_index)(int);
    u64 (*event_map)(int);
    int max_events;
    int num_counters;
    int num_counters_fixed;
    int cntval_bits;
    u64 cntval_mask;
    long unsigned int events_maskl;
    long unsigned int events_mask[1];
    int events_mask_len;
    int apic;
    u64 max_period;
    struct event_constraint * (*get_event_constraints)(struct cpu_hw_events *, int, struct perf_event *);
    void (*put_event_constraints)(struct cpu_hw_events *, struct perf_event *);
    void (*start_scheduling)(struct cpu_hw_events *);
    void (*commit_scheduling)(struct cpu_hw_events *, int, int);
    void (*stop_scheduling)(struct cpu_hw_events *);
    struct event_constraint *event_constraints;
    struct x86_pmu_quirk *quirks;
    int perfctr_second_write;
    u64 (*limit_period)(struct perf_event *, u64);
    unsigned int late_ack;
    unsigned int mid_ack;
    unsigned int enabled_ack;
    int attr_rdpmc_broken;
    int attr_rdpmc;
    struct attribute **format_attrs;
    ssize_t (*events_sysfs_show)(char *, u64);
    const struct attribute_group **attr_update;
    long unsigned int attr_freeze_on_smi;
    int (*cpu_prepare)(int);
    void (*cpu_starting)(int);
    void (*cpu_dying)(int);
    void (*cpu_dead)(int);
    void (*check_microcode)();
    void (*sched_task)(struct perf_event_context *, bool);
    u64 intel_ctrl;
    union perf_capabilities intel_cap;
    unsigned int bts;
    unsigned int bts_active;
    unsigned int pebs;
    unsigned int pebs_active;
    unsigned int pebs_broken;
    unsigned int pebs_prec_dist;
    unsigned int pebs_no_tlb;
    unsigned int pebs_no_isolation;
    unsigned int pebs_block;
    int pebs_record_size;
    int pebs_buffer_size;
    int max_pebs_events;
    void (*drain_pebs)(struct pt_regs *, struct perf_sample_data *);
    struct event_constraint *pebs_constraints;
    void (*pebs_aliases)(struct perf_event *);
    u64 (*pebs_latency_data)(struct perf_event *, u64);
    long unsigned int large_pebs_flags;
    u64 rtm_abort_event;
    unsigned int lbr_tos;
    unsigned int lbr_from;
    unsigned int lbr_to;
    unsigned int lbr_info;
    unsigned int lbr_nr;
    u64 lbr_sel_mask;
    u64 lbr_ctl_mask;
    const int *lbr_sel_map;
    int *lbr_ctl_map;
    bool lbr_double_abort;
    bool lbr_pt_coexist;
    unsigned int lbr_has_info;
    unsigned int lbr_has_tsx;
    unsigned int lbr_from_flags;
    unsigned int lbr_to_cycles;
    unsigned int lbr_depth_mask;
    unsigned int lbr_deep_c_reset;
    unsigned int lbr_lip;
    unsigned int lbr_cpl;
    unsigned int lbr_filter;
    unsigned int lbr_call_stack;
    unsigned int lbr_mispred;
    unsigned int lbr_timed_lbr;
    unsigned int lbr_br_type;
    void (*lbr_reset)();
    void (*lbr_read)(struct cpu_hw_events *);
    void (*lbr_save)(void *);
    void (*lbr_restore)(void *);
    atomic_t lbr_exclusive[3];
    int num_topdown_events;
    u64 (*update_topdown_event)(struct perf_event *);
    int (*set_topdown_event_period)(struct perf_event *);
    void (*swap_task_ctx)(struct perf_event_context *, struct perf_event_context *);
    unsigned int amd_nb_constraints;
    u64 perf_ctr_pair_en;
    struct extra_reg *extra_regs;
    unsigned int flags;
    struct perf_guest_switch_msr * (*guest_get_msrs)(int *);
    int (*check_period)(struct perf_event *, u64);
    int (*aux_output_match)(struct perf_event *);
    int (*filter_match)(struct perf_event *);
    int num_hybrid_pmus;
    struct x86_hybrid_pmu *hybrid_pmu;
    u8 (*get_hybrid_cpu_type)();
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct x86_pmu {
    const char *name;
    int version;
    int (*handle_irq)(struct pt_regs *);
    void (*disable_all)();
    void (*enable_all)(int);
    void (*enable)(struct perf_event *);
    void (*disable)(struct perf_event *);
    void (*assign)(struct perf_event *, int);
    void (*add)(struct perf_event *);
    void (*del)(struct perf_event *);
    void (*read)(struct perf_event *);
    int (*set_period)(struct perf_event *);
    u64 (*update)(struct perf_event *);
    int (*hw_config)(struct perf_event *);
    int (*schedule_events)(struct cpu_hw_events *, int, int *);
    unsigned int eventsel;
    unsigned int perfctr;
    int (*addr_offset)(int, bool);
    int (*rdpmc_index)(int);
    u64 (*event_map)(int);
    int max_events;
    int num_counters;
    int num_counters_fixed;
    int cntval_bits;
    u64 cntval_mask;
    long unsigned int events_maskl;
    long unsigned int events_mask[1];
    int events_mask_len;
    int apic;
    u64 max_period;
    struct event_constraint * (*get_event_constraints)(struct cpu_hw_events *, int, struct perf_event *);
    void (*put_event_constraints)(struct cpu_hw_events *, struct perf_event *);
    void (*start_scheduling)(struct cpu_hw_events *);
    void (*commit_scheduling)(struct cpu_hw_events *, int, int);
    void (*stop_scheduling)(struct cpu_hw_events *);
    struct event_constraint *event_constraints;
    struct x86_pmu_quirk *quirks;
    void (*limit_period)(struct perf_event *, s64 *);
    unsigned int late_ack;
    unsigned int mid_ack;
    unsigned int enabled_ack;
    int attr_rdpmc_broken;
    int attr_rdpmc;
    struct attribute **format_attrs;
    ssize_t (*events_sysfs_show)(char *, u64);
    const struct attribute_group **attr_update;
    long unsigned int attr_freeze_on_smi;
    int (*cpu_prepare)(int);
    void (*cpu_starting)(int);
    void (*cpu_dying)(int);
    void (*cpu_dead)(int);
    void (*check_microcode)();
    void (*sched_task)(struct perf_event_pmu_context *, bool);
    u64 intel_ctrl;
    union perf_capabilities intel_cap;
    unsigned int bts;
    unsigned int bts_active;
    unsigned int pebs;
    unsigned int pebs_active;
    unsigned int pebs_broken;
    unsigned int pebs_prec_dist;
    unsigned int pebs_no_tlb;
    unsigned int pebs_no_isolation;
    unsigned int pebs_block;
    unsigned int pebs_ept;
    int pebs_record_size;
    int pebs_buffer_size;
    int max_pebs_events;
    void (*drain_pebs)(struct pt_regs *, struct perf_sample_data *);
    struct event_constraint *pebs_constraints;
    void (*pebs_aliases)(struct perf_event *);
    u64 (*pebs_latency_data)(struct perf_event *, u64);
    long unsigned int large_pebs_flags;
    u64 rtm_abort_event;
    u64 pebs_capable;
    unsigned int lbr_tos;
    unsigned int lbr_from;
    unsigned int lbr_to;
    unsigned int lbr_info;
    unsigned int lbr_nr;
    u64 lbr_sel_mask;
    u64 lbr_ctl_mask;
    const int *lbr_sel_map;
    int *lbr_ctl_map;
    bool lbr_double_abort;
    bool lbr_pt_coexist;
    unsigned int lbr_has_info;
    unsigned int lbr_has_tsx;
    unsigned int lbr_from_flags;
    unsigned int lbr_to_cycles;
    unsigned int lbr_depth_mask;
    unsigned int lbr_deep_c_reset;
    unsigned int lbr_lip;
    unsigned int lbr_cpl;
    unsigned int lbr_filter;
    unsigned int lbr_call_stack;
    unsigned int lbr_mispred;
    unsigned int lbr_timed_lbr;
    unsigned int lbr_br_type;
    void (*lbr_reset)();
    void (*lbr_read)(struct cpu_hw_events *);
    void (*lbr_save)(void *);
    void (*lbr_restore)(void *);
    atomic_t lbr_exclusive[3];
    int num_topdown_events;
    void (*swap_task_ctx)(struct perf_event_pmu_context *, struct perf_event_pmu_context *);
    unsigned int amd_nb_constraints;
    u64 perf_ctr_pair_en;
    struct extra_reg *extra_regs;
    unsigned int flags;
    struct perf_guest_switch_msr * (*guest_get_msrs)(int *, void *);
    int (*check_period)(struct perf_event *, u64);
    int (*aux_output_match)(struct perf_event *);
    void (*filter)(struct pmu *, int, bool *);
    int num_hybrid_pmus;
    struct x86_hybrid_pmu *hybrid_pmu;
    u8 (*get_hybrid_cpu_type)();
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct x86_pmu {
    const char *name;
    int version;
    int (*handle_irq)(struct pt_regs *);
    void (*disable_all)();
    void (*enable_all)(int);
    void (*enable)(struct perf_event *);
    void (*disable)(struct perf_event *);
    void (*assign)(struct perf_event *, int);
    void (*add)(struct perf_event *);
    void (*del)(struct perf_event *);
    void (*read)(struct perf_event *);
    int (*set_period)(struct perf_event *);
    u64 (*update)(struct perf_event *);
    int (*hw_config)(struct perf_event *);
    int (*schedule_events)(struct cpu_hw_events *, int, int *);
    unsigned int eventsel;
    unsigned int perfctr;
    int (*addr_offset)(int, bool);
    int (*rdpmc_index)(int);
    u64 (*event_map)(int);
    int max_events;
    int num_counters;
    int num_counters_fixed;
    int cntval_bits;
    u64 cntval_mask;
    long unsigned int events_maskl;
    long unsigned int events_mask[1];
    int events_mask_len;
    int apic;
    u64 max_period;
    struct event_constraint * (*get_event_constraints)(struct cpu_hw_events *, int, struct perf_event *);
    void (*put_event_constraints)(struct cpu_hw_events *, struct perf_event *);
    void (*start_scheduling)(struct cpu_hw_events *);
    void (*commit_scheduling)(struct cpu_hw_events *, int, int);
    void (*stop_scheduling)(struct cpu_hw_events *);
    struct event_constraint *event_constraints;
    struct x86_pmu_quirk *quirks;
    void (*limit_period)(struct perf_event *, s64 *);
    unsigned int late_ack;
    unsigned int mid_ack;
    unsigned int enabled_ack;
    int attr_rdpmc_broken;
    int attr_rdpmc;
    struct attribute **format_attrs;
    ssize_t (*events_sysfs_show)(char *, u64);
    const struct attribute_group **attr_update;
    long unsigned int attr_freeze_on_smi;
    int (*cpu_prepare)(int);
    void (*cpu_starting)(int);
    void (*cpu_dying)(int);
    void (*cpu_dead)(int);
    void (*check_microcode)();
    void (*sched_task)(struct perf_event_pmu_context *, bool);
    u64 intel_ctrl;
    union perf_capabilities intel_cap;
    unsigned int bts;
    unsigned int bts_active;
    unsigned int pebs;
    unsigned int pebs_active;
    unsigned int pebs_broken;
    unsigned int pebs_prec_dist;
    unsigned int pebs_no_tlb;
    unsigned int pebs_no_isolation;
    unsigned int pebs_block;
    unsigned int pebs_ept;
    int pebs_record_size;
    int pebs_buffer_size;
    int max_pebs_events;
    void (*drain_pebs)(struct pt_regs *, struct perf_sample_data *);
    struct event_constraint *pebs_constraints;
    void (*pebs_aliases)(struct perf_event *);
    u64 (*pebs_latency_data)(struct perf_event *, u64);
    long unsigned int large_pebs_flags;
    u64 rtm_abort_event;
    u64 pebs_capable;
    unsigned int lbr_tos;
    unsigned int lbr_from;
    unsigned int lbr_to;
    unsigned int lbr_info;
    unsigned int lbr_nr;
    u64 lbr_sel_mask;
    u64 lbr_ctl_mask;
    const int *lbr_sel_map;
    int *lbr_ctl_map;
    bool lbr_double_abort;
    bool lbr_pt_coexist;
    unsigned int lbr_has_info;
    unsigned int lbr_has_tsx;
    unsigned int lbr_from_flags;
    unsigned int lbr_to_cycles;
    unsigned int lbr_depth_mask;
    unsigned int lbr_deep_c_reset;
    unsigned int lbr_lip;
    unsigned int lbr_cpl;
    unsigned int lbr_filter;
    unsigned int lbr_call_stack;
    unsigned int lbr_mispred;
    unsigned int lbr_timed_lbr;
    unsigned int lbr_br_type;
    void (*lbr_reset)();
    void (*lbr_read)(struct cpu_hw_events *);
    void (*lbr_save)(void *);
    void (*lbr_restore)(void *);
    atomic_t lbr_exclusive[3];
    int num_topdown_events;
    void (*swap_task_ctx)(struct perf_event_pmu_context *, struct perf_event_pmu_context *);
    unsigned int amd_nb_constraints;
    u64 perf_ctr_pair_en;
    struct extra_reg *extra_regs;
    unsigned int flags;
    struct perf_guest_switch_msr * (*guest_get_msrs)(int *, void *);
    int (*check_period)(struct perf_event *, u64);
    int (*aux_output_match)(struct perf_event *);
    void (*filter)(struct pmu *, int, bool *);
    int num_hybrid_pmus;
    struct x86_hybrid_pmu *hybrid_pmu;
    u8 (*get_hybrid_cpu_type)();
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct x86_pmu {
    const char *name;
    int version;
    int (*handle_irq)(struct pt_regs *);
    void (*disable_all)();
    void (*enable_all)(int);
    void (*enable)(struct perf_event *);
    void (*disable)(struct perf_event *);
    void (*assign)(struct perf_event *, int);
    void (*add)(struct perf_event *);
    void (*del)(struct perf_event *);
    void (*read)(struct perf_event *);
    int (*set_period)(struct perf_event *);
    u64 (*update)(struct perf_event *);
    int (*hw_config)(struct perf_event *);
    int (*schedule_events)(struct cpu_hw_events *, int, int *);
    unsigned int eventsel;
    unsigned int perfctr;
    int (*addr_offset)(int, bool);
    int (*rdpmc_index)(int);
    u64 (*event_map)(int);
    int max_events;
    int num_counters;
    int num_counters_fixed;
    int cntval_bits;
    u64 cntval_mask;
    long unsigned int events_maskl;
    long unsigned int events_mask[1];
    int events_mask_len;
    int apic;
    u64 max_period;
    struct event_constraint * (*get_event_constraints)(struct cpu_hw_events *, int, struct perf_event *);
    void (*put_event_constraints)(struct cpu_hw_events *, struct perf_event *);
    void (*start_scheduling)(struct cpu_hw_events *);
    void (*commit_scheduling)(struct cpu_hw_events *, int, int);
    void (*stop_scheduling)(struct cpu_hw_events *);
    struct event_constraint *event_constraints;
    struct x86_pmu_quirk *quirks;
    void (*limit_period)(struct perf_event *, s64 *);
    unsigned int late_ack;
    unsigned int mid_ack;
    unsigned int enabled_ack;
    int attr_rdpmc_broken;
    int attr_rdpmc;
    struct attribute **format_attrs;
    ssize_t (*events_sysfs_show)(char *, u64);
    const struct attribute_group **attr_update;
    long unsigned int attr_freeze_on_smi;
    int (*cpu_prepare)(int);
    void (*cpu_starting)(int);
    void (*cpu_dying)(int);
    void (*cpu_dead)(int);
    void (*check_microcode)();
    void (*sched_task)(struct perf_event_pmu_context *, bool);
    u64 intel_ctrl;
    union perf_capabilities intel_cap;
    unsigned int bts;
    unsigned int bts_active;
    unsigned int pebs;
    unsigned int pebs_active;
    unsigned int pebs_broken;
    unsigned int pebs_prec_dist;
    unsigned int pebs_no_tlb;
    unsigned int pebs_no_isolation;
    unsigned int pebs_block;
    unsigned int pebs_ept;
    int pebs_record_size;
    int pebs_buffer_size;
    int max_pebs_events;
    void (*drain_pebs)(struct pt_regs *, struct perf_sample_data *);
    struct event_constraint *pebs_constraints;
    void (*pebs_aliases)(struct perf_event *);
    u64 (*pebs_latency_data)(struct perf_event *, u64);
    long unsigned int large_pebs_flags;
    u64 rtm_abort_event;
    u64 pebs_capable;
    unsigned int lbr_tos;
    unsigned int lbr_from;
    unsigned int lbr_to;
    unsigned int lbr_info;
    unsigned int lbr_nr;
    u64 lbr_sel_mask;
    u64 lbr_ctl_mask;
    const int *lbr_sel_map;
    int *lbr_ctl_map;
    bool lbr_double_abort;
    bool lbr_pt_coexist;
    unsigned int lbr_has_info;
    unsigned int lbr_has_tsx;
    unsigned int lbr_from_flags;
    unsigned int lbr_to_cycles;
    unsigned int lbr_depth_mask;
    unsigned int lbr_deep_c_reset;
    unsigned int lbr_lip;
    unsigned int lbr_cpl;
    unsigned int lbr_filter;
    unsigned int lbr_call_stack;
    unsigned int lbr_mispred;
    unsigned int lbr_timed_lbr;
    unsigned int lbr_br_type;
    unsigned int lbr_counters;
    void (*lbr_reset)();
    void (*lbr_read)(struct cpu_hw_events *);
    void (*lbr_save)(void *);
    void (*lbr_restore)(void *);
    atomic_t lbr_exclusive[3];
    int num_topdown_events;
    void (*swap_task_ctx)(struct perf_event_pmu_context *, struct perf_event_pmu_context *);
    unsigned int amd_nb_constraints;
    u64 perf_ctr_pair_en;
    struct extra_reg *extra_regs;
    unsigned int flags;
    struct perf_guest_switch_msr * (*guest_get_msrs)(int *, void *);
    int (*check_period)(struct perf_event *, u64);
    int (*aux_output_match)(struct perf_event *);
    void (*filter)(struct pmu *, int, bool *);
    int num_hybrid_pmus;
    struct x86_hybrid_pmu *hybrid_pmu;
    enum hybrid_cpu_type (*get_hybrid_cpu_type)();
};
```
</details>
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct x86_pmu {
    const char *name;
    int version;
    int (*handle_irq)(struct pt_regs *);
    void (*disable_all)();
    void (*enable_all)(int);
    void (*enable)(struct perf_event *);
    void (*disable)(struct perf_event *);
    void (*add)(struct perf_event *);
    void (*del)(struct perf_event *);
    void (*read)(struct perf_event *);
    int (*hw_config)(struct perf_event *);
    int (*schedule_events)(struct cpu_hw_events *, int, int *);
    unsigned int eventsel;
    unsigned int perfctr;
    int (*addr_offset)(int, bool);
    int (*rdpmc_index)(int);
    u64 (*event_map)(int);
    int max_events;
    int num_counters;
    int num_counters_fixed;
    int cntval_bits;
    u64 cntval_mask;
    long unsigned int events_maskl;
    long unsigned int events_mask[1];
    int events_mask_len;
    int apic;
    u64 max_period;
    struct event_constraint * (*get_event_constraints)(struct cpu_hw_events *, int, struct perf_event *);
    void (*put_event_constraints)(struct cpu_hw_events *, struct perf_event *);
    void (*start_scheduling)(struct cpu_hw_events *);
    void (*commit_scheduling)(struct cpu_hw_events *, int, int);
    void (*stop_scheduling)(struct cpu_hw_events *);
    struct event_constraint *event_constraints;
    struct x86_pmu_quirk *quirks;
    int perfctr_second_write;
    u64 (*limit_period)(struct perf_event *, u64);
    unsigned int late_ack;
    unsigned int counter_freezing;
    int attr_rdpmc_broken;
    int attr_rdpmc;
    struct attribute **format_attrs;
    ssize_t (*events_sysfs_show)(char *, u64);
    const struct attribute_group **attr_update;
    long unsigned int attr_freeze_on_smi;
    int (*cpu_prepare)(int);
    void (*cpu_starting)(int);
    void (*cpu_dying)(int);
    void (*cpu_dead)(int);
    void (*check_microcode)();
    void (*sched_task)(struct perf_event_context *, bool);
    u64 intel_ctrl;
    union perf_capabilities intel_cap;
    unsigned int bts;
    unsigned int bts_active;
    unsigned int pebs;
    unsigned int pebs_active;
    unsigned int pebs_broken;
    unsigned int pebs_prec_dist;
    unsigned int pebs_no_tlb;
    unsigned int pebs_no_isolation;
    int pebs_record_size;
    int pebs_buffer_size;
    int max_pebs_events;
    void (*drain_pebs)(struct pt_regs *);
    struct event_constraint *pebs_constraints;
    void (*pebs_aliases)(struct perf_event *);
    long unsigned int large_pebs_flags;
    u64 rtm_abort_event;
    long unsigned int lbr_tos;
    long unsigned int lbr_from;
    long unsigned int lbr_to;
    int lbr_nr;
    u64 lbr_sel_mask;
    const int *lbr_sel_map;
    bool lbr_double_abort;
    bool lbr_pt_coexist;
    atomic_t lbr_exclusive[3];
    unsigned int amd_nb_constraints;
    u64 perf_ctr_pair_en;
    struct extra_reg *extra_regs;
    unsigned int flags;
    struct perf_guest_switch_msr * (*guest_get_msrs)(int *);
    int (*check_period)(struct perf_event *, u64);
    int (*aux_output_match)(struct perf_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct x86_pmu {
    const char *name;
    int version;
    int (*handle_irq)(struct pt_regs *);
    void (*disable_all)();
    void (*enable_all)(int);
    void (*enable)(struct perf_event *);
    void (*disable)(struct perf_event *);
    void (*add)(struct perf_event *);
    void (*del)(struct perf_event *);
    void (*read)(struct perf_event *);
    int (*hw_config)(struct perf_event *);
    int (*schedule_events)(struct cpu_hw_events *, int, int *);
    unsigned int eventsel;
    unsigned int perfctr;
    int (*addr_offset)(int, bool);
    int (*rdpmc_index)(int);
    u64 (*event_map)(int);
    int max_events;
    int num_counters;
    int num_counters_fixed;
    int cntval_bits;
    u64 cntval_mask;
    long unsigned int events_maskl;
    long unsigned int events_mask[1];
    int events_mask_len;
    int apic;
    u64 max_period;
    struct event_constraint * (*get_event_constraints)(struct cpu_hw_events *, int, struct perf_event *);
    void (*put_event_constraints)(struct cpu_hw_events *, struct perf_event *);
    void (*start_scheduling)(struct cpu_hw_events *);
    void (*commit_scheduling)(struct cpu_hw_events *, int, int);
    void (*stop_scheduling)(struct cpu_hw_events *);
    struct event_constraint *event_constraints;
    struct x86_pmu_quirk *quirks;
    int perfctr_second_write;
    u64 (*limit_period)(struct perf_event *, u64);
    unsigned int late_ack;
    unsigned int counter_freezing;
    int attr_rdpmc_broken;
    int attr_rdpmc;
    struct attribute **format_attrs;
    ssize_t (*events_sysfs_show)(char *, u64);
    const struct attribute_group **attr_update;
    long unsigned int attr_freeze_on_smi;
    int (*cpu_prepare)(int);
    void (*cpu_starting)(int);
    void (*cpu_dying)(int);
    void (*cpu_dead)(int);
    void (*check_microcode)();
    void (*sched_task)(struct perf_event_context *, bool);
    u64 intel_ctrl;
    union perf_capabilities intel_cap;
    unsigned int bts;
    unsigned int bts_active;
    unsigned int pebs;
    unsigned int pebs_active;
    unsigned int pebs_broken;
    unsigned int pebs_prec_dist;
    unsigned int pebs_no_tlb;
    unsigned int pebs_no_isolation;
    int pebs_record_size;
    int pebs_buffer_size;
    int max_pebs_events;
    void (*drain_pebs)(struct pt_regs *);
    struct event_constraint *pebs_constraints;
    void (*pebs_aliases)(struct perf_event *);
    long unsigned int large_pebs_flags;
    u64 rtm_abort_event;
    long unsigned int lbr_tos;
    long unsigned int lbr_from;
    long unsigned int lbr_to;
    int lbr_nr;
    u64 lbr_sel_mask;
    const int *lbr_sel_map;
    bool lbr_double_abort;
    bool lbr_pt_coexist;
    atomic_t lbr_exclusive[3];
    unsigned int amd_nb_constraints;
    u64 perf_ctr_pair_en;
    struct extra_reg *extra_regs;
    unsigned int flags;
    struct perf_guest_switch_msr * (*guest_get_msrs)(int *);
    int (*check_period)(struct perf_event *, u64);
    int (*aux_output_match)(struct perf_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct x86_pmu {
    const char *name;
    int version;
    int (*handle_irq)(struct pt_regs *);
    void (*disable_all)();
    void (*enable_all)(int);
    void (*enable)(struct perf_event *);
    void (*disable)(struct perf_event *);
    void (*add)(struct perf_event *);
    void (*del)(struct perf_event *);
    void (*read)(struct perf_event *);
    int (*hw_config)(struct perf_event *);
    int (*schedule_events)(struct cpu_hw_events *, int, int *);
    unsigned int eventsel;
    unsigned int perfctr;
    int (*addr_offset)(int, bool);
    int (*rdpmc_index)(int);
    u64 (*event_map)(int);
    int max_events;
    int num_counters;
    int num_counters_fixed;
    int cntval_bits;
    u64 cntval_mask;
    long unsigned int events_maskl;
    long unsigned int events_mask[1];
    int events_mask_len;
    int apic;
    u64 max_period;
    struct event_constraint * (*get_event_constraints)(struct cpu_hw_events *, int, struct perf_event *);
    void (*put_event_constraints)(struct cpu_hw_events *, struct perf_event *);
    void (*start_scheduling)(struct cpu_hw_events *);
    void (*commit_scheduling)(struct cpu_hw_events *, int, int);
    void (*stop_scheduling)(struct cpu_hw_events *);
    struct event_constraint *event_constraints;
    struct x86_pmu_quirk *quirks;
    int perfctr_second_write;
    u64 (*limit_period)(struct perf_event *, u64);
    unsigned int late_ack;
    unsigned int counter_freezing;
    int attr_rdpmc_broken;
    int attr_rdpmc;
    struct attribute **format_attrs;
    ssize_t (*events_sysfs_show)(char *, u64);
    const struct attribute_group **attr_update;
    long unsigned int attr_freeze_on_smi;
    int (*cpu_prepare)(int);
    void (*cpu_starting)(int);
    void (*cpu_dying)(int);
    void (*cpu_dead)(int);
    void (*check_microcode)();
    void (*sched_task)(struct perf_event_context *, bool);
    u64 intel_ctrl;
    union perf_capabilities intel_cap;
    unsigned int bts;
    unsigned int bts_active;
    unsigned int pebs;
    unsigned int pebs_active;
    unsigned int pebs_broken;
    unsigned int pebs_prec_dist;
    unsigned int pebs_no_tlb;
    unsigned int pebs_no_isolation;
    int pebs_record_size;
    int pebs_buffer_size;
    int max_pebs_events;
    void (*drain_pebs)(struct pt_regs *);
    struct event_constraint *pebs_constraints;
    void (*pebs_aliases)(struct perf_event *);
    long unsigned int large_pebs_flags;
    u64 rtm_abort_event;
    long unsigned int lbr_tos;
    long unsigned int lbr_from;
    long unsigned int lbr_to;
    int lbr_nr;
    u64 lbr_sel_mask;
    const int *lbr_sel_map;
    bool lbr_double_abort;
    bool lbr_pt_coexist;
    atomic_t lbr_exclusive[3];
    unsigned int amd_nb_constraints;
    u64 perf_ctr_pair_en;
    struct extra_reg *extra_regs;
    unsigned int flags;
    struct perf_guest_switch_msr * (*guest_get_msrs)(int *);
    int (*check_period)(struct perf_event *, u64);
    int (*aux_output_match)(struct perf_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct x86_pmu {
    const char *name;
    int version;
    int (*handle_irq)(struct pt_regs *);
    void (*disable_all)();
    void (*enable_all)(int);
    void (*enable)(struct perf_event *);
    void (*disable)(struct perf_event *);
    void (*add)(struct perf_event *);
    void (*del)(struct perf_event *);
    void (*read)(struct perf_event *);
    int (*hw_config)(struct perf_event *);
    int (*schedule_events)(struct cpu_hw_events *, int, int *);
    unsigned int eventsel;
    unsigned int perfctr;
    int (*addr_offset)(int, bool);
    int (*rdpmc_index)(int);
    u64 (*event_map)(int);
    int max_events;
    int num_counters;
    int num_counters_fixed;
    int cntval_bits;
    u64 cntval_mask;
    long unsigned int events_maskl;
    long unsigned int events_mask[1];
    int events_mask_len;
    int apic;
    u64 max_period;
    struct event_constraint * (*get_event_constraints)(struct cpu_hw_events *, int, struct perf_event *);
    void (*put_event_constraints)(struct cpu_hw_events *, struct perf_event *);
    void (*start_scheduling)(struct cpu_hw_events *);
    void (*commit_scheduling)(struct cpu_hw_events *, int, int);
    void (*stop_scheduling)(struct cpu_hw_events *);
    struct event_constraint *event_constraints;
    struct x86_pmu_quirk *quirks;
    int perfctr_second_write;
    u64 (*limit_period)(struct perf_event *, u64);
    unsigned int late_ack;
    unsigned int counter_freezing;
    int attr_rdpmc_broken;
    int attr_rdpmc;
    struct attribute **format_attrs;
    ssize_t (*events_sysfs_show)(char *, u64);
    const struct attribute_group **attr_update;
    long unsigned int attr_freeze_on_smi;
    int (*cpu_prepare)(int);
    void (*cpu_starting)(int);
    void (*cpu_dying)(int);
    void (*cpu_dead)(int);
    void (*check_microcode)();
    void (*sched_task)(struct perf_event_context *, bool);
    u64 intel_ctrl;
    union perf_capabilities intel_cap;
    unsigned int bts;
    unsigned int bts_active;
    unsigned int pebs;
    unsigned int pebs_active;
    unsigned int pebs_broken;
    unsigned int pebs_prec_dist;
    unsigned int pebs_no_tlb;
    unsigned int pebs_no_isolation;
    int pebs_record_size;
    int pebs_buffer_size;
    int max_pebs_events;
    void (*drain_pebs)(struct pt_regs *);
    struct event_constraint *pebs_constraints;
    void (*pebs_aliases)(struct perf_event *);
    long unsigned int large_pebs_flags;
    u64 rtm_abort_event;
    long unsigned int lbr_tos;
    long unsigned int lbr_from;
    long unsigned int lbr_to;
    int lbr_nr;
    u64 lbr_sel_mask;
    const int *lbr_sel_map;
    bool lbr_double_abort;
    bool lbr_pt_coexist;
    atomic_t lbr_exclusive[3];
    unsigned int amd_nb_constraints;
    u64 perf_ctr_pair_en;
    struct extra_reg *extra_regs;
    unsigned int flags;
    struct perf_guest_switch_msr * (*guest_get_msrs)(int *);
    int (*check_period)(struct perf_event *, u64);
    int (*aux_output_match)(struct perf_event *);
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
<code>unsigned int pebs_prec_dist</code>
</li>
<li>
<b>Field added. </b>
<code>bool lbr_pt_coexist</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int amd_nb_constraints</code>
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
<code>void (*add)(struct perf_event *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*del)(struct perf_event *)</code>
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
<code>long unsigned int attr_freeze_on_smi</code>
</li>
<li>
<b>Field added. </b>
<code>struct attribute **attrs</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int pebs_no_tlb</code>
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
<code>struct attribute **caps_attrs</code>
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
<code>void (*read)(struct perf_event *)</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int large_pebs_flags</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int free_running_flags</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int (*limit_period)(struct perf_event *, unsigned int)</code> ➡️ <code>u64 (*limit_period)(struct perf_event *, u64)</code>
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
<code>unsigned int counter_freezing</code>
</li>
<li>
<b>Field added. </b>
<code>int (*check_period)(struct perf_event *, u64)</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool late_ack</code> ➡️ <code>unsigned int late_ack</code>
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
<b>Field added. </b>
<code>unsigned int pebs_no_isolation</code>
</li>
<li>
<b>Field added. </b>
<code>u64 rtm_abort_event</code>
</li>
<li>
<b>Field removed. </b>
<code>struct attribute **event_attrs</code>
</li>
<li>
<b>Field removed. </b>
<code>struct attribute **caps_attrs</code>
</li>
<li>
<b>Field removed. </b>
<code>struct attribute **cpu_events</code>
</li>
<li>
<b>Field removed. </b>
<code>struct attribute **attrs</code>
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
<code>u64 perf_ctr_pair_en</code>
</li>
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
<code>unsigned int enabled_ack</code>
</li>
<li>
<b>Field added. </b>
<code>void (*swap_task_ctx)(struct perf_event_context *, struct perf_event_context *)</code>
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
<code>unsigned int lbr_info</code>
</li>
<li>
<b>Field added. </b>
<code>u64 lbr_ctl_mask</code>
</li>
<li>
<b>Field added. </b>
<code>int *lbr_ctl_map</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int lbr_depth_mask</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int lbr_deep_c_reset</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int lbr_lip</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int lbr_cpl</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int lbr_filter</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int lbr_call_stack</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int lbr_mispred</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int lbr_timed_lbr</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int lbr_br_type</code>
</li>
<li>
<b>Field added. </b>
<code>void (*lbr_reset)()</code>
</li>
<li>
<b>Field added. </b>
<code>void (*lbr_read)(struct cpu_hw_events *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*lbr_save)(void *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*lbr_restore)(void *)</code>
</li>
<li>
<b>Field added. </b>
<code>u64 (*update_topdown_event)(struct perf_event *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_topdown_event_period)(struct perf_event *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*drain_pebs)(struct pt_regs *)</code> ➡️ <code>void (*drain_pebs)(struct pt_regs *, struct perf_sample_data *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int lbr_tos</code> ➡️ <code>unsigned int lbr_tos</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int lbr_from</code> ➡️ <code>unsigned int lbr_from</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int lbr_to</code> ➡️ <code>unsigned int lbr_to</code>
</li>
<li>
<b>Field type changed. </b>
<code>int lbr_nr</code> ➡️ <code>unsigned int lbr_nr</code>
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
<code>unsigned int mid_ack</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int pebs_block</code>
</li>
<li>
<b>Field added. </b>
<code>int num_topdown_events</code>
</li>
<li>
<b>Field added. </b>
<code>int (*filter_match)(struct perf_event *)</code>
</li>
<li>
<b>Field added. </b>
<code>int num_hybrid_pmus</code>
</li>
<li>
<b>Field added. </b>
<code>struct x86_hybrid_pmu *hybrid_pmu</code>
</li>
<li>
<b>Field added. </b>
<code>u8 (*get_hybrid_cpu_type)()</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int counter_freezing</code>
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
<code>void (*assign)(struct perf_event *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>u64 (*pebs_latency_data)(struct perf_event *, u64)</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int lbr_has_info</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int lbr_has_tsx</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int lbr_from_flags</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int lbr_to_cycles</code>
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
<code>int (*set_period)(struct perf_event *)</code>
</li>
<li>
<b>Field added. </b>
<code>u64 (*update)(struct perf_event *)</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int pebs_ept</code>
</li>
<li>
<b>Field added. </b>
<code>u64 pebs_capable</code>
</li>
<li>
<b>Field added. </b>
<code>void (*filter)(struct pmu *, int, bool *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int perfctr_second_write</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 (*update_topdown_event)(struct perf_event *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*set_topdown_event_period)(struct perf_event *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*filter_match)(struct perf_event *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>u64 (*limit_period)(struct perf_event *, u64)</code> ➡️ <code>void (*limit_period)(struct perf_event *, s64 *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*sched_task)(struct perf_event_context *, bool)</code> ➡️ <code>void (*sched_task)(struct perf_event_pmu_context *, bool)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*swap_task_ctx)(struct perf_event_context *, struct perf_event_context *)</code> ➡️ <code>void (*swap_task_ctx)(struct perf_event_pmu_context *, struct perf_event_pmu_context *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct perf_guest_switch_msr * (*guest_get_msrs)(int *)</code> ➡️ <code>struct perf_guest_switch_msr * (*guest_get_msrs)(int *, void *)</code>
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
<code>unsigned int lbr_counters</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 (*get_hybrid_cpu_type)()</code> ➡️ <code>enum hybrid_cpu_type (*get_hybrid_cpu_type)()</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Arch</b>
<ul>
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
