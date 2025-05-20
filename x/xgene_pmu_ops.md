# Struct: <code>xgene_pmu_ops</code>

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
struct xgene_pmu_ops {
    void (*mask_int)(struct xgene_pmu *);
    void (*unmask_int)(struct xgene_pmu *);
    u64 (*read_counter)(struct xgene_pmu_dev *, int);
    void (*write_counter)(struct xgene_pmu_dev *, int, u64);
    void (*write_evttype)(struct xgene_pmu_dev *, int, u32);
    void (*write_agentmsk)(struct xgene_pmu_dev *, u32);
    void (*write_agent1msk)(struct xgene_pmu_dev *, u32);
    void (*enable_counter)(struct xgene_pmu_dev *, int);
    void (*disable_counter)(struct xgene_pmu_dev *, int);
    void (*enable_counter_int)(struct xgene_pmu_dev *, int);
    void (*disable_counter_int)(struct xgene_pmu_dev *, int);
    void (*reset_counters)(struct xgene_pmu_dev *);
    void (*start_counters)(struct xgene_pmu_dev *);
    void (*stop_counters)(struct xgene_pmu_dev *);
};
```
</details>
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
<b>Arch</b>
<ul>
</ul>
