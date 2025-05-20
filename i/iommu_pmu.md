# Struct: <code>iommu_pmu</code>

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
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct iommu_pmu {
    struct intel_iommu *iommu;
    u32 num_cntr;
    u32 num_eg;
    u32 cntr_width;
    u32 cntr_stride;
    u32 filter;
    void *base;
    void *cfg_reg;
    void *cntr_reg;
    void *overflow;
    u64 *evcap;
    u32 **cntr_evcap;
    struct pmu pmu;
    long unsigned int used_mask[1];
    struct perf_event * event_list[64];
    unsigned char irq_name[16];
    struct hlist_node cpuhp_node;
    int cpu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct iommu_pmu {
    struct intel_iommu *iommu;
    u32 num_cntr;
    u32 num_eg;
    u32 cntr_width;
    u32 cntr_stride;
    u32 filter;
    void *base;
    void *cfg_reg;
    void *cntr_reg;
    void *overflow;
    u64 *evcap;
    u32 **cntr_evcap;
    struct pmu pmu;
    long unsigned int used_mask[1];
    struct perf_event * event_list[64];
    unsigned char irq_name[16];
    struct hlist_node cpuhp_node;
    int cpu;
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
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
