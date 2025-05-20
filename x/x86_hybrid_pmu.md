# Struct: <code>x86_hybrid_pmu</code>

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
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct x86_hybrid_pmu {
    struct pmu pmu;
    const char *name;
    u8 cpu_type;
    cpumask_t supported_cpus;
    union perf_capabilities intel_cap;
    u64 intel_ctrl;
    int max_pebs_events;
    int num_counters;
    int num_counters_fixed;
    struct event_constraint unconstrained;
    u64 hw_cache_event_ids[42];
    u64 hw_cache_extra_regs[42];
    struct event_constraint *event_constraints;
    struct event_constraint *pebs_constraints;
    struct extra_reg *extra_regs;
    unsigned int late_ack;
    unsigned int mid_ack;
    unsigned int enabled_ack;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct x86_hybrid_pmu {
    struct pmu pmu;
    const char *name;
    u8 cpu_type;
    cpumask_t supported_cpus;
    union perf_capabilities intel_cap;
    u64 intel_ctrl;
    int max_pebs_events;
    int num_counters;
    int num_counters_fixed;
    struct event_constraint unconstrained;
    u64 hw_cache_event_ids[42];
    u64 hw_cache_extra_regs[42];
    struct event_constraint *event_constraints;
    struct event_constraint *pebs_constraints;
    struct extra_reg *extra_regs;
    unsigned int late_ack;
    unsigned int mid_ack;
    unsigned int enabled_ack;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct x86_hybrid_pmu {
    struct pmu pmu;
    const char *name;
    u8 cpu_type;
    cpumask_t supported_cpus;
    union perf_capabilities intel_cap;
    u64 intel_ctrl;
    int max_pebs_events;
    int num_counters;
    int num_counters_fixed;
    struct event_constraint unconstrained;
    u64 hw_cache_event_ids[42];
    u64 hw_cache_extra_regs[42];
    struct event_constraint *event_constraints;
    struct event_constraint *pebs_constraints;
    struct extra_reg *extra_regs;
    unsigned int late_ack;
    unsigned int mid_ack;
    unsigned int enabled_ack;
    u64 pebs_data_source[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct x86_hybrid_pmu {
    struct pmu pmu;
    const char *name;
    u8 cpu_type;
    cpumask_t supported_cpus;
    union perf_capabilities intel_cap;
    u64 intel_ctrl;
    int max_pebs_events;
    int num_counters;
    int num_counters_fixed;
    struct event_constraint unconstrained;
    u64 hw_cache_event_ids[42];
    u64 hw_cache_extra_regs[42];
    struct event_constraint *event_constraints;
    struct event_constraint *pebs_constraints;
    struct extra_reg *extra_regs;
    unsigned int late_ack;
    unsigned int mid_ack;
    unsigned int enabled_ack;
    u64 pebs_data_source[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct x86_hybrid_pmu {
    struct pmu pmu;
    const char *name;
    u8 cpu_type;
    cpumask_t supported_cpus;
    union perf_capabilities intel_cap;
    u64 intel_ctrl;
    int max_pebs_events;
    int num_counters;
    int num_counters_fixed;
    struct event_constraint unconstrained;
    u64 hw_cache_event_ids[42];
    u64 hw_cache_extra_regs[42];
    struct event_constraint *event_constraints;
    struct event_constraint *pebs_constraints;
    struct extra_reg *extra_regs;
    unsigned int late_ack;
    unsigned int mid_ack;
    unsigned int enabled_ack;
    u64 pebs_data_source[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct x86_hybrid_pmu {
    struct pmu pmu;
    const char *name;
    enum hybrid_pmu_type pmu_type;
    cpumask_t supported_cpus;
    union perf_capabilities intel_cap;
    u64 intel_ctrl;
    int max_pebs_events;
    int num_counters;
    int num_counters_fixed;
    struct event_constraint unconstrained;
    u64 hw_cache_event_ids[42];
    u64 hw_cache_extra_regs[42];
    struct event_constraint *event_constraints;
    struct event_constraint *pebs_constraints;
    struct extra_reg *extra_regs;
    unsigned int late_ack;
    unsigned int mid_ack;
    unsigned int enabled_ack;
    u64 pebs_data_source[16];
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
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 pebs_data_source[16]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
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
<code>enum hybrid_pmu_type pmu_type</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 cpu_type</code>
</li>
</ul>
</details>
</li>
</ul>
