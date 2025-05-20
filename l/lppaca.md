# Struct: <code>lppaca</code>

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
struct lppaca {
    __be32 desc;
    __be16 size;
    u8 reserved1[3];
    u8 __old_status;
    u8 reserved3[14];
    volatile __be32 dyn_hw_node_id;
    volatile __be32 dyn_hw_proc_id;
    u8 reserved4[56];
    volatile volatile u8[8] vphn_assoc_counts;
    u8 reserved5[32];
    u8 reserved6[48];
    u8 cede_latency_hint;
    u8 ebb_regs_in_use;
    u8 reserved7[6];
    u8 dtl_enable_mask;
    u8 donate_dedicated_cpu;
    u8 fpregs_in_use;
    u8 pmcregs_in_use;
    u8 reserved8[28];
    __be64 wait_state_cycles;
    u8 reserved9[28];
    __be16 slb_count;
    u8 idle;
    u8 vmxregs_in_use;
    volatile __be32 yield_count;
    volatile __be32 dispersion_count;
    volatile __be64 cmo_faults;
    volatile __be64 cmo_fault_time;
    u8 reserved10[104];
    __be32 page_ins;
    u8 reserved11[148];
    volatile __be64 dtl_idx;
    u8 reserved12[96];
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
