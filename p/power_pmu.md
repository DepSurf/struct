# Struct: <code>power_pmu</code>

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
In <code>arm64</code>: Absent ⚠️
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct power_pmu {
    const char *name;
    int n_counter;
    int max_alternatives;
    long unsigned int add_fields;
    long unsigned int test_adder;
    int (*compute_mmcr)(u64 *, int, unsigned int *, long unsigned int *, struct perf_event **);
    int (*get_constraint)(u64, long unsigned int *, long unsigned int *);
    int (*get_alternatives)(u64, unsigned int, u64 *);
    void (*get_mem_data_src)(union perf_mem_data_src *, u32, struct pt_regs *);
    void (*get_mem_weight)(u64 *);
    long unsigned int group_constraint_mask;
    long unsigned int group_constraint_val;
    u64 (*bhrb_filter_map)(u64);
    void (*config_bhrb)(u64);
    void (*disable_pmc)(unsigned int, long unsigned int *);
    int (*limited_pmc_event)(u64);
    u32 flags;
    const struct attribute_group **attr_groups;
    int n_generic;
    int *generic_events;
    int[42] *cache_events;
    int n_blacklist_ev;
    int *blacklist_ev;
    int bhrb_nr;
};
```
</details>
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
