# Struct: <code>kvmppc_host_state</code>

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
struct kvmppc_host_state {
    ulong host_r1;
    ulong host_r2;
    ulong host_msr;
    ulong vmhandler;
    ulong scratch0;
    ulong scratch1;
    ulong scratch2;
    u8 in_guest;
    u8 restore_hid5;
    u8 napping;
    u8 hwthread_req;
    u8 hwthread_state;
    u8 host_ipi;
    u8 ptid;
    u8 tid;
    u8 fake_suspend;
    struct kvm_vcpu *kvm_vcpu;
    struct kvmppc_vcore *kvm_vcore;
    void *xics_phys;
    void *xive_tima_phys;
    void *xive_tima_virt;
    u32 saved_xirr;
    u64 dabr;
    u64 host_mmcr[7];
    u32 host_pmc[8];
    u64 host_purr;
    u64 host_spurr;
    u64 host_dscr;
    u64 dec_expires;
    struct kvm_split_mode *kvm_split_mode;
    u64 cfar;
    u64 ppr;
    u64 host_fscr;
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
