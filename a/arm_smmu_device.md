# Struct: <code>arm_smmu_device</code>

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
struct arm_smmu_device {
    struct device *dev;
    void *base;
    unsigned int numpage;
    unsigned int pgshift;
    u32 features;
    enum arm_smmu_arch_version version;
    enum arm_smmu_implementation model;
    const struct arm_smmu_impl *impl;
    u32 num_context_banks;
    u32 num_s2_context_banks;
    long unsigned int context_map[2];
    struct arm_smmu_cb *cbs;
    atomic_t irptndx;
    u32 num_mapping_groups;
    u16 streamid_mask;
    u16 smr_mask_mask;
    struct arm_smmu_smr *smrs;
    struct arm_smmu_s2cr *s2crs;
    struct mutex stream_map_mutex;
    long unsigned int va_size;
    long unsigned int ipa_size;
    long unsigned int pa_size;
    long unsigned int pgsize_bitmap;
    u32 num_global_irqs;
    u32 num_context_irqs;
    unsigned int *irqs;
    struct clk_bulk_data *clks;
    int num_clks;
    spinlock_t global_sync_lock;
    struct iommu_device iommu;
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
