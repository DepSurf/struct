# Struct: <code>arm_pmu</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
In <code>4.8</code>: Absent ⚠️
</li>
<li>
In <code>4.10</code>: Absent ⚠️
</li>
<li>
In <code>4.13</code>: Absent ⚠️
</li>
<li>
In <code>4.15</code>: Absent ⚠️
</li>
<li>
In <code>4.18</code>: Absent ⚠️
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
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct arm_pmu {
    struct pmu pmu;
    cpumask_t supported_cpus;
    char *name;
    irqreturn_t (*handle_irq)(struct arm_pmu *);
    void (*enable)(struct perf_event *);
    void (*disable)(struct perf_event *);
    int (*get_event_idx)(struct pmu_hw_events *, struct perf_event *);
    void (*clear_event_idx)(struct pmu_hw_events *, struct perf_event *);
    int (*set_event_filter)(struct hw_perf_event *, struct perf_event_attr *);
    u64 (*read_counter)(struct perf_event *);
    void (*write_counter)(struct perf_event *, u64);
    void (*start)(struct arm_pmu *);
    void (*stop)(struct arm_pmu *);
    void (*reset)(void *);
    int (*map_event)(struct perf_event *);
    int (*filter_match)(struct perf_event *);
    int num_events;
    bool secure_access;
    long unsigned int pmceid_bitmap[1];
    long unsigned int pmceid_ext_bitmap[1];
    struct platform_device *plat_device;
    struct pmu_hw_events *hw_events;
    struct hlist_node node;
    struct notifier_block cpu_pm_nb;
    const struct attribute_group * attr_groups[4];
    long unsigned int acpi_cpuid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct arm_pmu {
    struct pmu pmu;
    cpumask_t supported_cpus;
    char *name;
    irqreturn_t (*handle_irq)(struct arm_pmu *);
    void (*enable)(struct perf_event *);
    void (*disable)(struct perf_event *);
    int (*get_event_idx)(struct pmu_hw_events *, struct perf_event *);
    void (*clear_event_idx)(struct pmu_hw_events *, struct perf_event *);
    int (*set_event_filter)(struct hw_perf_event *, struct perf_event_attr *);
    u64 (*read_counter)(struct perf_event *);
    void (*write_counter)(struct perf_event *, u64);
    void (*start)(struct arm_pmu *);
    void (*stop)(struct arm_pmu *);
    void (*reset)(void *);
    int (*map_event)(struct perf_event *);
    int (*filter_match)(struct perf_event *);
    int num_events;
    bool secure_access;
    long unsigned int pmceid_bitmap[2];
    long unsigned int pmceid_ext_bitmap[2];
    struct platform_device *plat_device;
    struct pmu_hw_events *hw_events;
    struct hlist_node node;
    struct notifier_block cpu_pm_nb;
    const struct attribute_group * attr_groups[4];
    long unsigned int acpi_cpuid;
};
```
</details>
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
<b>Arch</b>
<ul>
</ul>
