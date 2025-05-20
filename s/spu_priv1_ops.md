# Struct: <code>spu_priv1_ops</code>

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
struct spu_priv1_ops {
    void (*int_mask_and)(struct spu *, int, u64);
    void (*int_mask_or)(struct spu *, int, u64);
    void (*int_mask_set)(struct spu *, int, u64);
    u64 (*int_mask_get)(struct spu *, int);
    void (*int_stat_clear)(struct spu *, int, u64);
    u64 (*int_stat_get)(struct spu *, int);
    void (*cpu_affinity_set)(struct spu *, int);
    u64 (*mfc_dar_get)(struct spu *);
    u64 (*mfc_dsisr_get)(struct spu *);
    void (*mfc_dsisr_set)(struct spu *, u64);
    void (*mfc_sdr_setup)(struct spu *);
    void (*mfc_sr1_set)(struct spu *, u64);
    u64 (*mfc_sr1_get)(struct spu *);
    void (*mfc_tclass_id_set)(struct spu *, u64);
    u64 (*mfc_tclass_id_get)(struct spu *);
    void (*tlb_invalidate)(struct spu *);
    void (*resource_allocation_groupID_set)(struct spu *, u64);
    u64 (*resource_allocation_groupID_get)(struct spu *);
    void (*resource_allocation_enable_set)(struct spu *, u64);
    u64 (*resource_allocation_enable_get)(struct spu *);
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
