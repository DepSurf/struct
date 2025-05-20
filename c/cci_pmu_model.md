# Struct: <code>cci_pmu_model</code>

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
struct cci_pmu_model {
    char *name;
    u32 fixed_hw_cntrs;
    u32 num_hw_cntrs;
    u32 cntr_size;
    struct attribute **format_attrs;
    struct attribute **event_attrs;
    struct event_range event_ranges[3];
    int (*validate_hw_event)(struct cci_pmu *, long unsigned int);
    int (*get_event_idx)(struct cci_pmu *, struct cci_pmu_hw_events *, long unsigned int);
    void (*write_counters)(struct cci_pmu *, long unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct cci_pmu_model {
    char *name;
    u32 fixed_hw_cntrs;
    u32 num_hw_cntrs;
    u32 cntr_size;
    struct attribute **format_attrs;
    struct attribute **event_attrs;
    struct event_range event_ranges[3];
    int (*validate_hw_event)(struct cci_pmu *, long unsigned int);
    int (*get_event_idx)(struct cci_pmu *, struct cci_pmu_hw_events *, long unsigned int);
    void (*write_counters)(struct cci_pmu *, long unsigned int *);
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
