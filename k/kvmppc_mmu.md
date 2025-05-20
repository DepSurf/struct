# Struct: <code>kvmppc_mmu</code>

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
struct kvmppc_mmu {
    void (*slbmte)(struct kvm_vcpu *, u64, u64);
    u64 (*slbmfee)(struct kvm_vcpu *, u64);
    u64 (*slbmfev)(struct kvm_vcpu *, u64);
    int (*slbfee)(struct kvm_vcpu *, gva_t, ulong *);
    void (*slbie)(struct kvm_vcpu *, u64);
    void (*slbia)(struct kvm_vcpu *);
    void (*mtsrin)(struct kvm_vcpu *, u32, ulong);
    u32 (*mfsrin)(struct kvm_vcpu *, u32);
    int (*xlate)(struct kvm_vcpu *, gva_t, struct kvmppc_pte *, bool, bool);
    void (*reset_msr)(struct kvm_vcpu *);
    void (*tlbie)(struct kvm_vcpu *, ulong, bool);
    int (*esid_to_vsid)(struct kvm_vcpu *, ulong, u64 *);
    u64 (*ea_to_vp)(struct kvm_vcpu *, gva_t, bool);
    bool (*is_dcbz32)(struct kvm_vcpu *);
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
