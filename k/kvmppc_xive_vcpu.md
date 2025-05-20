# Struct: <code>kvmppc_xive_vcpu</code>

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
struct kvmppc_xive_vcpu {
    struct kvmppc_xive *xive;
    struct kvm_vcpu *vcpu;
    bool valid;
    u32 server_num;
    u32 vp_id;
    u32 vp_chip_id;
    u32 vp_cam;
    u32 vp_ipi;
    struct xive_irq_data vp_ipi_data;
    uint8_t cppr;
    uint8_t hw_cppr;
    uint8_t mfrr;
    uint8_t pending;
    struct xive_q queues[8];
    u32 esc_virq[8];
    char * esc_virq_names[8];
    u32 delayed_irq;
    u64 stat_rm_h_xirr;
    u64 stat_rm_h_ipoll;
    u64 stat_rm_h_cppr;
    u64 stat_rm_h_eoi;
    u64 stat_rm_h_ipi;
    u64 stat_vm_h_xirr;
    u64 stat_vm_h_ipoll;
    u64 stat_vm_h_cppr;
    u64 stat_vm_h_eoi;
    u64 stat_vm_h_ipi;
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
