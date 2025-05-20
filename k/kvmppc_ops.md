# Struct: <code>kvmppc_ops</code>

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
struct kvmppc_ops {
    struct module *owner;
    int (*get_sregs)(struct kvm_vcpu *, struct kvm_sregs *);
    int (*set_sregs)(struct kvm_vcpu *, struct kvm_sregs *);
    int (*get_one_reg)(struct kvm_vcpu *, u64, union kvmppc_one_reg *);
    int (*set_one_reg)(struct kvm_vcpu *, u64, union kvmppc_one_reg *);
    void (*vcpu_load)(struct kvm_vcpu *, int);
    void (*vcpu_put)(struct kvm_vcpu *);
    void (*set_msr)(struct kvm_vcpu *, u64);
    int (*vcpu_run)(struct kvm_run *, struct kvm_vcpu *);
    struct kvm_vcpu * (*vcpu_create)(struct kvm *, unsigned int);
    void (*vcpu_free)(struct kvm_vcpu *);
    int (*check_requests)(struct kvm_vcpu *);
    int (*get_dirty_log)(struct kvm *, struct kvm_dirty_log *);
    void (*flush_memslot)(struct kvm *, struct kvm_memory_slot *);
    int (*prepare_memory_region)(struct kvm *, struct kvm_memory_slot *, const struct kvm_userspace_memory_region *);
    void (*commit_memory_region)(struct kvm *, const struct kvm_userspace_memory_region *, const struct kvm_memory_slot *, const struct kvm_memory_slot *, enum kvm_mr_change);
    int (*unmap_hva_range)(struct kvm *, long unsigned int, long unsigned int);
    int (*age_hva)(struct kvm *, long unsigned int, long unsigned int);
    int (*test_age_hva)(struct kvm *, long unsigned int);
    void (*set_spte_hva)(struct kvm *, long unsigned int, pte_t);
    void (*mmu_destroy)(struct kvm_vcpu *);
    void (*free_memslot)(struct kvm_memory_slot *, struct kvm_memory_slot *);
    int (*create_memslot)(struct kvm_memory_slot *, long unsigned int);
    int (*init_vm)(struct kvm *);
    void (*destroy_vm)(struct kvm *);
    int (*get_smmu_info)(struct kvm *, struct kvm_ppc_smmu_info *);
    int (*emulate_op)(struct kvm_run *, struct kvm_vcpu *, unsigned int, int *);
    int (*emulate_mtspr)(struct kvm_vcpu *, int, ulong);
    int (*emulate_mfspr)(struct kvm_vcpu *, int, ulong *);
    void (*fast_vcpu_kick)(struct kvm_vcpu *);
    long int (*arch_vm_ioctl)(struct file *, unsigned int, long unsigned int);
    int (*hcall_implemented)(long unsigned int);
    int (*irq_bypass_add_producer)(struct irq_bypass_consumer *, struct irq_bypass_producer *);
    void (*irq_bypass_del_producer)(struct irq_bypass_consumer *, struct irq_bypass_producer *);
    int (*configure_mmu)(struct kvm *, struct kvm_ppc_mmuv3_cfg *);
    int (*get_rmmu_info)(struct kvm *, struct kvm_ppc_rmmu_info *);
    int (*set_smt_mode)(struct kvm *, long unsigned int, long unsigned int);
    void (*giveup_ext)(struct kvm_vcpu *, ulong);
    int (*enable_nested)(struct kvm *);
    int (*load_from_eaddr)(struct kvm_vcpu *, ulong *, void *, int);
    int (*store_to_eaddr)(struct kvm_vcpu *, ulong *, void *, int);
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
