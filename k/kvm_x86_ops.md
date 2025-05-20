# Struct: <code>kvm_x86_ops</code>

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
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kvm_x86_ops {
    int (*hardware_enable)();
    void (*hardware_disable)();
    void (*hardware_unsetup)();
    bool (*cpu_has_accelerated_tpr)();
    bool (*has_emulated_msr)(struct kvm *, u32);
    void (*vcpu_after_set_cpuid)(struct kvm_vcpu *);
    unsigned int vm_size;
    int (*vm_init)(struct kvm *);
    void (*vm_destroy)(struct kvm *);
    int (*vcpu_create)(struct kvm_vcpu *);
    void (*vcpu_free)(struct kvm_vcpu *);
    void (*vcpu_reset)(struct kvm_vcpu *, bool);
    void (*prepare_guest_switch)(struct kvm_vcpu *);
    void (*vcpu_load)(struct kvm_vcpu *, int);
    void (*vcpu_put)(struct kvm_vcpu *);
    void (*update_exception_bitmap)(struct kvm_vcpu *);
    int (*get_msr)(struct kvm_vcpu *, struct msr_data *);
    int (*set_msr)(struct kvm_vcpu *, struct msr_data *);
    u64 (*get_segment_base)(struct kvm_vcpu *, int);
    void (*get_segment)(struct kvm_vcpu *, struct kvm_segment *, int);
    int (*get_cpl)(struct kvm_vcpu *);
    void (*set_segment)(struct kvm_vcpu *, struct kvm_segment *, int);
    void (*get_cs_db_l_bits)(struct kvm_vcpu *, int *, int *);
    void (*set_cr0)(struct kvm_vcpu *, long unsigned int);
    bool (*is_valid_cr4)(struct kvm_vcpu *, long unsigned int);
    void (*set_cr4)(struct kvm_vcpu *, long unsigned int);
    int (*set_efer)(struct kvm_vcpu *, u64);
    void (*get_idt)(struct kvm_vcpu *, struct desc_ptr *);
    void (*set_idt)(struct kvm_vcpu *, struct desc_ptr *);
    void (*get_gdt)(struct kvm_vcpu *, struct desc_ptr *);
    void (*set_gdt)(struct kvm_vcpu *, struct desc_ptr *);
    void (*sync_dirty_debug_regs)(struct kvm_vcpu *);
    void (*set_dr7)(struct kvm_vcpu *, long unsigned int);
    void (*cache_reg)(struct kvm_vcpu *, enum kvm_reg);
    long unsigned int (*get_rflags)(struct kvm_vcpu *);
    void (*set_rflags)(struct kvm_vcpu *, long unsigned int);
    void (*tlb_flush_all)(struct kvm_vcpu *);
    void (*tlb_flush_current)(struct kvm_vcpu *);
    int (*tlb_remote_flush)(struct kvm *);
    int (*tlb_remote_flush_with_range)(struct kvm *, struct kvm_tlb_range *);
    void (*tlb_flush_gva)(struct kvm_vcpu *, gva_t);
    void (*tlb_flush_guest)(struct kvm_vcpu *);
    enum exit_fastpath_completion (*run)(struct kvm_vcpu *);
    int (*handle_exit)(struct kvm_vcpu *, enum exit_fastpath_completion);
    int (*skip_emulated_instruction)(struct kvm_vcpu *);
    void (*update_emulated_instruction)(struct kvm_vcpu *);
    void (*set_interrupt_shadow)(struct kvm_vcpu *, int);
    u32 (*get_interrupt_shadow)(struct kvm_vcpu *);
    void (*patch_hypercall)(struct kvm_vcpu *, unsigned char *);
    void (*set_irq)(struct kvm_vcpu *);
    void (*set_nmi)(struct kvm_vcpu *);
    void (*queue_exception)(struct kvm_vcpu *);
    void (*cancel_injection)(struct kvm_vcpu *);
    int (*interrupt_allowed)(struct kvm_vcpu *, bool);
    int (*nmi_allowed)(struct kvm_vcpu *, bool);
    bool (*get_nmi_mask)(struct kvm_vcpu *);
    void (*set_nmi_mask)(struct kvm_vcpu *, bool);
    void (*enable_nmi_window)(struct kvm_vcpu *);
    void (*enable_irq_window)(struct kvm_vcpu *);
    void (*update_cr8_intercept)(struct kvm_vcpu *, int, int);
    bool (*check_apicv_inhibit_reasons)(ulong);
    void (*pre_update_apicv_exec_ctrl)(struct kvm *, bool);
    void (*refresh_apicv_exec_ctrl)(struct kvm_vcpu *);
    void (*hwapic_irr_update)(struct kvm_vcpu *, int);
    void (*hwapic_isr_update)(struct kvm_vcpu *, int);
    bool (*guest_apic_has_interrupt)(struct kvm_vcpu *);
    void (*load_eoi_exitmap)(struct kvm_vcpu *, u64 *);
    void (*set_virtual_apic_mode)(struct kvm_vcpu *);
    void (*set_apic_access_page_addr)(struct kvm_vcpu *);
    int (*deliver_posted_interrupt)(struct kvm_vcpu *, int);
    int (*sync_pir_to_irr)(struct kvm_vcpu *);
    int (*set_tss_addr)(struct kvm *, unsigned int);
    int (*set_identity_map_addr)(struct kvm *, u64);
    u64 (*get_mt_mask)(struct kvm_vcpu *, gfn_t, bool);
    void (*load_mmu_pgd)(struct kvm_vcpu *, hpa_t, int);
    bool (*has_wbinvd_exit)();
    u64 (*write_l1_tsc_offset)(struct kvm_vcpu *, u64);
    void (*get_exit_info)(struct kvm_vcpu *, u64 *, u64 *, u32 *, u32 *);
    int (*check_intercept)(struct kvm_vcpu *, struct x86_instruction_info *, enum x86_intercept_stage, struct x86_exception *);
    void (*handle_exit_irqoff)(struct kvm_vcpu *);
    void (*request_immediate_exit)(struct kvm_vcpu *);
    void (*sched_in)(struct kvm_vcpu *, int);
    int cpu_dirty_log_size;
    void (*update_cpu_dirty_logging)(struct kvm_vcpu *);
    const struct kvm_pmu_ops *pmu_ops;
    const struct kvm_x86_nested_ops *nested_ops;
    int (*pre_block)(struct kvm_vcpu *);
    void (*post_block)(struct kvm_vcpu *);
    void (*vcpu_blocking)(struct kvm_vcpu *);
    void (*vcpu_unblocking)(struct kvm_vcpu *);
    int (*update_pi_irte)(struct kvm *, unsigned int, uint32_t, bool);
    void (*start_assignment)(struct kvm *);
    void (*apicv_post_state_restore)(struct kvm_vcpu *);
    bool (*dy_apicv_has_pending_interrupt)(struct kvm_vcpu *);
    int (*set_hv_timer)(struct kvm_vcpu *, u64, bool *);
    void (*cancel_hv_timer)(struct kvm_vcpu *);
    void (*setup_mce)(struct kvm_vcpu *);
    int (*smi_allowed)(struct kvm_vcpu *, bool);
    int (*pre_enter_smm)(struct kvm_vcpu *, char *);
    int (*pre_leave_smm)(struct kvm_vcpu *, const char *);
    void (*enable_smi_window)(struct kvm_vcpu *);
    int (*mem_enc_op)(struct kvm *, void *);
    int (*mem_enc_reg_region)(struct kvm *, struct kvm_enc_region *);
    int (*mem_enc_unreg_region)(struct kvm *, struct kvm_enc_region *);
    int (*vm_copy_enc_context_from)(struct kvm *, unsigned int);
    int (*get_msr_feature)(struct kvm_msr_entry *);
    bool (*can_emulate_instruction)(struct kvm_vcpu *, void *, int);
    bool (*apic_init_signal_blocked)(struct kvm_vcpu *);
    int (*enable_direct_tlbflush)(struct kvm_vcpu *);
    void (*migrate_timers)(struct kvm_vcpu *);
    void (*msr_filter_changed)(struct kvm_vcpu *);
    int (*complete_emulated_msr)(struct kvm_vcpu *, int);
    void (*vcpu_deliver_sipi_vector)(struct kvm_vcpu *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kvm_x86_ops {
    int (*hardware_enable)();
    void (*hardware_disable)();
    void (*hardware_unsetup)();
    bool (*cpu_has_accelerated_tpr)();
    bool (*has_emulated_msr)(struct kvm *, u32);
    void (*vcpu_after_set_cpuid)(struct kvm_vcpu *);
    unsigned int vm_size;
    int (*vm_init)(struct kvm *);
    void (*vm_destroy)(struct kvm *);
    int (*vcpu_create)(struct kvm_vcpu *);
    void (*vcpu_free)(struct kvm_vcpu *);
    void (*vcpu_reset)(struct kvm_vcpu *, bool);
    void (*prepare_guest_switch)(struct kvm_vcpu *);
    void (*vcpu_load)(struct kvm_vcpu *, int);
    void (*vcpu_put)(struct kvm_vcpu *);
    void (*update_exception_bitmap)(struct kvm_vcpu *);
    int (*get_msr)(struct kvm_vcpu *, struct msr_data *);
    int (*set_msr)(struct kvm_vcpu *, struct msr_data *);
    u64 (*get_segment_base)(struct kvm_vcpu *, int);
    void (*get_segment)(struct kvm_vcpu *, struct kvm_segment *, int);
    int (*get_cpl)(struct kvm_vcpu *);
    void (*set_segment)(struct kvm_vcpu *, struct kvm_segment *, int);
    void (*get_cs_db_l_bits)(struct kvm_vcpu *, int *, int *);
    void (*set_cr0)(struct kvm_vcpu *, long unsigned int);
    bool (*is_valid_cr4)(struct kvm_vcpu *, long unsigned int);
    void (*set_cr4)(struct kvm_vcpu *, long unsigned int);
    int (*set_efer)(struct kvm_vcpu *, u64);
    void (*get_idt)(struct kvm_vcpu *, struct desc_ptr *);
    void (*set_idt)(struct kvm_vcpu *, struct desc_ptr *);
    void (*get_gdt)(struct kvm_vcpu *, struct desc_ptr *);
    void (*set_gdt)(struct kvm_vcpu *, struct desc_ptr *);
    void (*sync_dirty_debug_regs)(struct kvm_vcpu *);
    void (*set_dr7)(struct kvm_vcpu *, long unsigned int);
    void (*cache_reg)(struct kvm_vcpu *, enum kvm_reg);
    long unsigned int (*get_rflags)(struct kvm_vcpu *);
    void (*set_rflags)(struct kvm_vcpu *, long unsigned int);
    bool (*get_if_flag)(struct kvm_vcpu *);
    void (*tlb_flush_all)(struct kvm_vcpu *);
    void (*tlb_flush_current)(struct kvm_vcpu *);
    int (*tlb_remote_flush)(struct kvm *);
    int (*tlb_remote_flush_with_range)(struct kvm *, struct kvm_tlb_range *);
    void (*tlb_flush_gva)(struct kvm_vcpu *, gva_t);
    void (*tlb_flush_guest)(struct kvm_vcpu *);
    enum exit_fastpath_completion (*run)(struct kvm_vcpu *);
    int (*handle_exit)(struct kvm_vcpu *, enum exit_fastpath_completion);
    int (*skip_emulated_instruction)(struct kvm_vcpu *);
    void (*update_emulated_instruction)(struct kvm_vcpu *);
    void (*set_interrupt_shadow)(struct kvm_vcpu *, int);
    u32 (*get_interrupt_shadow)(struct kvm_vcpu *);
    void (*patch_hypercall)(struct kvm_vcpu *, unsigned char *);
    void (*set_irq)(struct kvm_vcpu *);
    void (*set_nmi)(struct kvm_vcpu *);
    void (*queue_exception)(struct kvm_vcpu *);
    void (*cancel_injection)(struct kvm_vcpu *);
    int (*interrupt_allowed)(struct kvm_vcpu *, bool);
    int (*nmi_allowed)(struct kvm_vcpu *, bool);
    bool (*get_nmi_mask)(struct kvm_vcpu *);
    void (*set_nmi_mask)(struct kvm_vcpu *, bool);
    void (*enable_nmi_window)(struct kvm_vcpu *);
    void (*enable_irq_window)(struct kvm_vcpu *);
    void (*update_cr8_intercept)(struct kvm_vcpu *, int, int);
    bool (*check_apicv_inhibit_reasons)(ulong);
    void (*refresh_apicv_exec_ctrl)(struct kvm_vcpu *);
    void (*hwapic_irr_update)(struct kvm_vcpu *, int);
    void (*hwapic_isr_update)(struct kvm_vcpu *, int);
    bool (*guest_apic_has_interrupt)(struct kvm_vcpu *);
    void (*load_eoi_exitmap)(struct kvm_vcpu *, u64 *);
    void (*set_virtual_apic_mode)(struct kvm_vcpu *);
    void (*set_apic_access_page_addr)(struct kvm_vcpu *);
    int (*deliver_posted_interrupt)(struct kvm_vcpu *, int);
    int (*sync_pir_to_irr)(struct kvm_vcpu *);
    int (*set_tss_addr)(struct kvm *, unsigned int);
    int (*set_identity_map_addr)(struct kvm *, u64);
    u64 (*get_mt_mask)(struct kvm_vcpu *, gfn_t, bool);
    void (*load_mmu_pgd)(struct kvm_vcpu *, hpa_t, int);
    bool (*has_wbinvd_exit)();
    u64 (*get_l2_tsc_offset)(struct kvm_vcpu *);
    u64 (*get_l2_tsc_multiplier)(struct kvm_vcpu *);
    void (*write_tsc_offset)(struct kvm_vcpu *, u64);
    void (*write_tsc_multiplier)(struct kvm_vcpu *, u64);
    void (*get_exit_info)(struct kvm_vcpu *, u64 *, u64 *, u32 *, u32 *);
    int (*check_intercept)(struct kvm_vcpu *, struct x86_instruction_info *, enum x86_intercept_stage, struct x86_exception *);
    void (*handle_exit_irqoff)(struct kvm_vcpu *);
    void (*request_immediate_exit)(struct kvm_vcpu *);
    void (*sched_in)(struct kvm_vcpu *, int);
    int cpu_dirty_log_size;
    void (*update_cpu_dirty_logging)(struct kvm_vcpu *);
    const struct kvm_pmu_ops *pmu_ops;
    const struct kvm_x86_nested_ops *nested_ops;
    int (*pre_block)(struct kvm_vcpu *);
    void (*post_block)(struct kvm_vcpu *);
    void (*vcpu_blocking)(struct kvm_vcpu *);
    void (*vcpu_unblocking)(struct kvm_vcpu *);
    int (*update_pi_irte)(struct kvm *, unsigned int, uint32_t, bool);
    void (*start_assignment)(struct kvm *);
    void (*apicv_post_state_restore)(struct kvm_vcpu *);
    bool (*dy_apicv_has_pending_interrupt)(struct kvm_vcpu *);
    int (*set_hv_timer)(struct kvm_vcpu *, u64, bool *);
    void (*cancel_hv_timer)(struct kvm_vcpu *);
    void (*setup_mce)(struct kvm_vcpu *);
    int (*smi_allowed)(struct kvm_vcpu *, bool);
    int (*enter_smm)(struct kvm_vcpu *, char *);
    int (*leave_smm)(struct kvm_vcpu *, const char *);
    void (*enable_smi_window)(struct kvm_vcpu *);
    int (*mem_enc_op)(struct kvm *, void *);
    int (*mem_enc_reg_region)(struct kvm *, struct kvm_enc_region *);
    int (*mem_enc_unreg_region)(struct kvm *, struct kvm_enc_region *);
    int (*vm_copy_enc_context_from)(struct kvm *, unsigned int);
    int (*get_msr_feature)(struct kvm_msr_entry *);
    bool (*can_emulate_instruction)(struct kvm_vcpu *, void *, int);
    bool (*apic_init_signal_blocked)(struct kvm_vcpu *);
    int (*enable_direct_tlbflush)(struct kvm_vcpu *);
    void (*migrate_timers)(struct kvm_vcpu *);
    void (*msr_filter_changed)(struct kvm_vcpu *);
    int (*complete_emulated_msr)(struct kvm_vcpu *, int);
    void (*vcpu_deliver_sipi_vector)(struct kvm_vcpu *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kvm_x86_ops {
    const char *name;
    int (*hardware_enable)();
    void (*hardware_disable)();
    void (*hardware_unsetup)();
    bool (*has_emulated_msr)(struct kvm *, u32);
    void (*vcpu_after_set_cpuid)(struct kvm_vcpu *);
    unsigned int vm_size;
    int (*vm_init)(struct kvm *);
    void (*vm_destroy)(struct kvm *);
    int (*vcpu_create)(struct kvm_vcpu *);
    void (*vcpu_free)(struct kvm_vcpu *);
    void (*vcpu_reset)(struct kvm_vcpu *, bool);
    void (*prepare_switch_to_guest)(struct kvm_vcpu *);
    void (*vcpu_load)(struct kvm_vcpu *, int);
    void (*vcpu_put)(struct kvm_vcpu *);
    void (*update_exception_bitmap)(struct kvm_vcpu *);
    int (*get_msr)(struct kvm_vcpu *, struct msr_data *);
    int (*set_msr)(struct kvm_vcpu *, struct msr_data *);
    u64 (*get_segment_base)(struct kvm_vcpu *, int);
    void (*get_segment)(struct kvm_vcpu *, struct kvm_segment *, int);
    int (*get_cpl)(struct kvm_vcpu *);
    void (*set_segment)(struct kvm_vcpu *, struct kvm_segment *, int);
    void (*get_cs_db_l_bits)(struct kvm_vcpu *, int *, int *);
    void (*set_cr0)(struct kvm_vcpu *, long unsigned int);
    void (*post_set_cr3)(struct kvm_vcpu *, long unsigned int);
    bool (*is_valid_cr4)(struct kvm_vcpu *, long unsigned int);
    void (*set_cr4)(struct kvm_vcpu *, long unsigned int);
    int (*set_efer)(struct kvm_vcpu *, u64);
    void (*get_idt)(struct kvm_vcpu *, struct desc_ptr *);
    void (*set_idt)(struct kvm_vcpu *, struct desc_ptr *);
    void (*get_gdt)(struct kvm_vcpu *, struct desc_ptr *);
    void (*set_gdt)(struct kvm_vcpu *, struct desc_ptr *);
    void (*sync_dirty_debug_regs)(struct kvm_vcpu *);
    void (*set_dr7)(struct kvm_vcpu *, long unsigned int);
    void (*cache_reg)(struct kvm_vcpu *, enum kvm_reg);
    long unsigned int (*get_rflags)(struct kvm_vcpu *);
    void (*set_rflags)(struct kvm_vcpu *, long unsigned int);
    bool (*get_if_flag)(struct kvm_vcpu *);
    void (*flush_tlb_all)(struct kvm_vcpu *);
    void (*flush_tlb_current)(struct kvm_vcpu *);
    int (*tlb_remote_flush)(struct kvm *);
    int (*tlb_remote_flush_with_range)(struct kvm *, struct kvm_tlb_range *);
    void (*flush_tlb_gva)(struct kvm_vcpu *, gva_t);
    void (*flush_tlb_guest)(struct kvm_vcpu *);
    int (*vcpu_pre_run)(struct kvm_vcpu *);
    enum exit_fastpath_completion (*vcpu_run)(struct kvm_vcpu *);
    int (*handle_exit)(struct kvm_vcpu *, enum exit_fastpath_completion);
    int (*skip_emulated_instruction)(struct kvm_vcpu *);
    void (*update_emulated_instruction)(struct kvm_vcpu *);
    void (*set_interrupt_shadow)(struct kvm_vcpu *, int);
    u32 (*get_interrupt_shadow)(struct kvm_vcpu *);
    void (*patch_hypercall)(struct kvm_vcpu *, unsigned char *);
    void (*inject_irq)(struct kvm_vcpu *);
    void (*inject_nmi)(struct kvm_vcpu *);
    void (*queue_exception)(struct kvm_vcpu *);
    void (*cancel_injection)(struct kvm_vcpu *);
    int (*interrupt_allowed)(struct kvm_vcpu *, bool);
    int (*nmi_allowed)(struct kvm_vcpu *, bool);
    bool (*get_nmi_mask)(struct kvm_vcpu *);
    void (*set_nmi_mask)(struct kvm_vcpu *, bool);
    void (*enable_nmi_window)(struct kvm_vcpu *);
    void (*enable_irq_window)(struct kvm_vcpu *);
    void (*update_cr8_intercept)(struct kvm_vcpu *, int, int);
    bool (*check_apicv_inhibit_reasons)(enum kvm_apicv_inhibit);
    void (*refresh_apicv_exec_ctrl)(struct kvm_vcpu *);
    void (*hwapic_irr_update)(struct kvm_vcpu *, int);
    void (*hwapic_isr_update)(struct kvm_vcpu *, int);
    bool (*guest_apic_has_interrupt)(struct kvm_vcpu *);
    void (*load_eoi_exitmap)(struct kvm_vcpu *, u64 *);
    void (*set_virtual_apic_mode)(struct kvm_vcpu *);
    void (*set_apic_access_page_addr)(struct kvm_vcpu *);
    void (*deliver_interrupt)(struct kvm_lapic *, int, int, int);
    int (*sync_pir_to_irr)(struct kvm_vcpu *);
    int (*set_tss_addr)(struct kvm *, unsigned int);
    int (*set_identity_map_addr)(struct kvm *, u64);
    u64 (*get_mt_mask)(struct kvm_vcpu *, gfn_t, bool);
    void (*load_mmu_pgd)(struct kvm_vcpu *, hpa_t, int);
    bool (*has_wbinvd_exit)();
    u64 (*get_l2_tsc_offset)(struct kvm_vcpu *);
    u64 (*get_l2_tsc_multiplier)(struct kvm_vcpu *);
    void (*write_tsc_offset)(struct kvm_vcpu *, u64);
    void (*write_tsc_multiplier)(struct kvm_vcpu *, u64);
    void (*get_exit_info)(struct kvm_vcpu *, u32 *, u64 *, u64 *, u32 *, u32 *);
    int (*check_intercept)(struct kvm_vcpu *, struct x86_instruction_info *, enum x86_intercept_stage, struct x86_exception *);
    void (*handle_exit_irqoff)(struct kvm_vcpu *);
    void (*request_immediate_exit)(struct kvm_vcpu *);
    void (*sched_in)(struct kvm_vcpu *, int);
    int cpu_dirty_log_size;
    void (*update_cpu_dirty_logging)(struct kvm_vcpu *);
    const struct kvm_x86_nested_ops *nested_ops;
    void (*vcpu_blocking)(struct kvm_vcpu *);
    void (*vcpu_unblocking)(struct kvm_vcpu *);
    int (*pi_update_irte)(struct kvm *, unsigned int, uint32_t, bool);
    void (*pi_start_assignment)(struct kvm *);
    void (*apicv_post_state_restore)(struct kvm_vcpu *);
    bool (*dy_apicv_has_pending_interrupt)(struct kvm_vcpu *);
    int (*set_hv_timer)(struct kvm_vcpu *, u64, bool *);
    void (*cancel_hv_timer)(struct kvm_vcpu *);
    void (*setup_mce)(struct kvm_vcpu *);
    int (*smi_allowed)(struct kvm_vcpu *, bool);
    int (*enter_smm)(struct kvm_vcpu *, char *);
    int (*leave_smm)(struct kvm_vcpu *, const char *);
    void (*enable_smi_window)(struct kvm_vcpu *);
    int (*mem_enc_ioctl)(struct kvm *, void *);
    int (*mem_enc_register_region)(struct kvm *, struct kvm_enc_region *);
    int (*mem_enc_unregister_region)(struct kvm *, struct kvm_enc_region *);
    int (*vm_copy_enc_context_from)(struct kvm *, unsigned int);
    int (*vm_move_enc_context_from)(struct kvm *, unsigned int);
    void (*guest_memory_reclaimed)(struct kvm *);
    int (*get_msr_feature)(struct kvm_msr_entry *);
    bool (*can_emulate_instruction)(struct kvm_vcpu *, int, void *, int);
    bool (*apic_init_signal_blocked)(struct kvm_vcpu *);
    int (*enable_direct_tlbflush)(struct kvm_vcpu *);
    void (*migrate_timers)(struct kvm_vcpu *);
    void (*msr_filter_changed)(struct kvm_vcpu *);
    int (*complete_emulated_msr)(struct kvm_vcpu *, int);
    void (*vcpu_deliver_sipi_vector)(struct kvm_vcpu *, u8);
    long unsigned int (*vcpu_get_apicv_inhibit_reasons)(struct kvm_vcpu *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kvm_x86_ops {
    const char *name;
    int (*hardware_enable)();
    void (*hardware_disable)();
    void (*hardware_unsetup)();
    bool (*has_emulated_msr)(struct kvm *, u32);
    void (*vcpu_after_set_cpuid)(struct kvm_vcpu *);
    unsigned int vm_size;
    int (*vm_init)(struct kvm *);
    void (*vm_destroy)(struct kvm *);
    int (*vcpu_precreate)(struct kvm *);
    int (*vcpu_create)(struct kvm_vcpu *);
    void (*vcpu_free)(struct kvm_vcpu *);
    void (*vcpu_reset)(struct kvm_vcpu *, bool);
    void (*prepare_switch_to_guest)(struct kvm_vcpu *);
    void (*vcpu_load)(struct kvm_vcpu *, int);
    void (*vcpu_put)(struct kvm_vcpu *);
    void (*update_exception_bitmap)(struct kvm_vcpu *);
    int (*get_msr)(struct kvm_vcpu *, struct msr_data *);
    int (*set_msr)(struct kvm_vcpu *, struct msr_data *);
    u64 (*get_segment_base)(struct kvm_vcpu *, int);
    void (*get_segment)(struct kvm_vcpu *, struct kvm_segment *, int);
    int (*get_cpl)(struct kvm_vcpu *);
    void (*set_segment)(struct kvm_vcpu *, struct kvm_segment *, int);
    void (*get_cs_db_l_bits)(struct kvm_vcpu *, int *, int *);
    void (*set_cr0)(struct kvm_vcpu *, long unsigned int);
    void (*post_set_cr3)(struct kvm_vcpu *, long unsigned int);
    bool (*is_valid_cr4)(struct kvm_vcpu *, long unsigned int);
    void (*set_cr4)(struct kvm_vcpu *, long unsigned int);
    int (*set_efer)(struct kvm_vcpu *, u64);
    void (*get_idt)(struct kvm_vcpu *, struct desc_ptr *);
    void (*set_idt)(struct kvm_vcpu *, struct desc_ptr *);
    void (*get_gdt)(struct kvm_vcpu *, struct desc_ptr *);
    void (*set_gdt)(struct kvm_vcpu *, struct desc_ptr *);
    void (*sync_dirty_debug_regs)(struct kvm_vcpu *);
    void (*set_dr7)(struct kvm_vcpu *, long unsigned int);
    void (*cache_reg)(struct kvm_vcpu *, enum kvm_reg);
    long unsigned int (*get_rflags)(struct kvm_vcpu *);
    void (*set_rflags)(struct kvm_vcpu *, long unsigned int);
    bool (*get_if_flag)(struct kvm_vcpu *);
    void (*flush_tlb_all)(struct kvm_vcpu *);
    void (*flush_tlb_current)(struct kvm_vcpu *);
    int (*tlb_remote_flush)(struct kvm *);
    int (*tlb_remote_flush_with_range)(struct kvm *, struct kvm_tlb_range *);
    void (*flush_tlb_gva)(struct kvm_vcpu *, gva_t);
    void (*flush_tlb_guest)(struct kvm_vcpu *);
    int (*vcpu_pre_run)(struct kvm_vcpu *);
    enum exit_fastpath_completion (*vcpu_run)(struct kvm_vcpu *);
    int (*handle_exit)(struct kvm_vcpu *, enum exit_fastpath_completion);
    int (*skip_emulated_instruction)(struct kvm_vcpu *);
    void (*update_emulated_instruction)(struct kvm_vcpu *);
    void (*set_interrupt_shadow)(struct kvm_vcpu *, int);
    u32 (*get_interrupt_shadow)(struct kvm_vcpu *);
    void (*patch_hypercall)(struct kvm_vcpu *, unsigned char *);
    void (*inject_irq)(struct kvm_vcpu *, bool);
    void (*inject_nmi)(struct kvm_vcpu *);
    void (*inject_exception)(struct kvm_vcpu *);
    void (*cancel_injection)(struct kvm_vcpu *);
    int (*interrupt_allowed)(struct kvm_vcpu *, bool);
    int (*nmi_allowed)(struct kvm_vcpu *, bool);
    bool (*get_nmi_mask)(struct kvm_vcpu *);
    void (*set_nmi_mask)(struct kvm_vcpu *, bool);
    void (*enable_nmi_window)(struct kvm_vcpu *);
    void (*enable_irq_window)(struct kvm_vcpu *);
    void (*update_cr8_intercept)(struct kvm_vcpu *, int, int);
    bool (*check_apicv_inhibit_reasons)(enum kvm_apicv_inhibit);
    void (*refresh_apicv_exec_ctrl)(struct kvm_vcpu *);
    void (*hwapic_irr_update)(struct kvm_vcpu *, int);
    void (*hwapic_isr_update)(int);
    bool (*guest_apic_has_interrupt)(struct kvm_vcpu *);
    void (*load_eoi_exitmap)(struct kvm_vcpu *, u64 *);
    void (*set_virtual_apic_mode)(struct kvm_vcpu *);
    void (*set_apic_access_page_addr)(struct kvm_vcpu *);
    void (*deliver_interrupt)(struct kvm_lapic *, int, int, int);
    int (*sync_pir_to_irr)(struct kvm_vcpu *);
    int (*set_tss_addr)(struct kvm *, unsigned int);
    int (*set_identity_map_addr)(struct kvm *, u64);
    u8 (*get_mt_mask)(struct kvm_vcpu *, gfn_t, bool);
    void (*load_mmu_pgd)(struct kvm_vcpu *, hpa_t, int);
    bool (*has_wbinvd_exit)();
    u64 (*get_l2_tsc_offset)(struct kvm_vcpu *);
    u64 (*get_l2_tsc_multiplier)(struct kvm_vcpu *);
    void (*write_tsc_offset)(struct kvm_vcpu *, u64);
    void (*write_tsc_multiplier)(struct kvm_vcpu *, u64);
    void (*get_exit_info)(struct kvm_vcpu *, u32 *, u64 *, u64 *, u32 *, u32 *);
    int (*check_intercept)(struct kvm_vcpu *, struct x86_instruction_info *, enum x86_intercept_stage, struct x86_exception *);
    void (*handle_exit_irqoff)(struct kvm_vcpu *);
    void (*request_immediate_exit)(struct kvm_vcpu *);
    void (*sched_in)(struct kvm_vcpu *, int);
    int cpu_dirty_log_size;
    void (*update_cpu_dirty_logging)(struct kvm_vcpu *);
    const struct kvm_x86_nested_ops *nested_ops;
    void (*vcpu_blocking)(struct kvm_vcpu *);
    void (*vcpu_unblocking)(struct kvm_vcpu *);
    int (*pi_update_irte)(struct kvm *, unsigned int, uint32_t, bool);
    void (*pi_start_assignment)(struct kvm *);
    void (*apicv_post_state_restore)(struct kvm_vcpu *);
    bool (*dy_apicv_has_pending_interrupt)(struct kvm_vcpu *);
    int (*set_hv_timer)(struct kvm_vcpu *, u64, bool *);
    void (*cancel_hv_timer)(struct kvm_vcpu *);
    void (*setup_mce)(struct kvm_vcpu *);
    int (*smi_allowed)(struct kvm_vcpu *, bool);
    int (*enter_smm)(struct kvm_vcpu *, union kvm_smram *);
    int (*leave_smm)(struct kvm_vcpu *, const union kvm_smram *);
    void (*enable_smi_window)(struct kvm_vcpu *);
    int (*mem_enc_ioctl)(struct kvm *, void *);
    int (*mem_enc_register_region)(struct kvm *, struct kvm_enc_region *);
    int (*mem_enc_unregister_region)(struct kvm *, struct kvm_enc_region *);
    int (*vm_copy_enc_context_from)(struct kvm *, unsigned int);
    int (*vm_move_enc_context_from)(struct kvm *, unsigned int);
    void (*guest_memory_reclaimed)(struct kvm *);
    int (*get_msr_feature)(struct kvm_msr_entry *);
    bool (*can_emulate_instruction)(struct kvm_vcpu *, int, void *, int);
    bool (*apic_init_signal_blocked)(struct kvm_vcpu *);
    int (*enable_l2_tlb_flush)(struct kvm_vcpu *);
    void (*migrate_timers)(struct kvm_vcpu *);
    void (*msr_filter_changed)(struct kvm_vcpu *);
    int (*complete_emulated_msr)(struct kvm_vcpu *, int);
    void (*vcpu_deliver_sipi_vector)(struct kvm_vcpu *, u8);
    long unsigned int (*vcpu_get_apicv_inhibit_reasons)(struct kvm_vcpu *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kvm_x86_ops {
    const char *name;
    int (*check_processor_compatibility)();
    int (*hardware_enable)();
    void (*hardware_disable)();
    void (*hardware_unsetup)();
    bool (*has_emulated_msr)(struct kvm *, u32);
    void (*vcpu_after_set_cpuid)(struct kvm_vcpu *);
    unsigned int vm_size;
    int (*vm_init)(struct kvm *);
    void (*vm_destroy)(struct kvm *);
    int (*vcpu_precreate)(struct kvm *);
    int (*vcpu_create)(struct kvm_vcpu *);
    void (*vcpu_free)(struct kvm_vcpu *);
    void (*vcpu_reset)(struct kvm_vcpu *, bool);
    void (*prepare_switch_to_guest)(struct kvm_vcpu *);
    void (*vcpu_load)(struct kvm_vcpu *, int);
    void (*vcpu_put)(struct kvm_vcpu *);
    void (*update_exception_bitmap)(struct kvm_vcpu *);
    int (*get_msr)(struct kvm_vcpu *, struct msr_data *);
    int (*set_msr)(struct kvm_vcpu *, struct msr_data *);
    u64 (*get_segment_base)(struct kvm_vcpu *, int);
    void (*get_segment)(struct kvm_vcpu *, struct kvm_segment *, int);
    int (*get_cpl)(struct kvm_vcpu *);
    void (*set_segment)(struct kvm_vcpu *, struct kvm_segment *, int);
    void (*get_cs_db_l_bits)(struct kvm_vcpu *, int *, int *);
    bool (*is_valid_cr0)(struct kvm_vcpu *, long unsigned int);
    void (*set_cr0)(struct kvm_vcpu *, long unsigned int);
    void (*post_set_cr3)(struct kvm_vcpu *, long unsigned int);
    bool (*is_valid_cr4)(struct kvm_vcpu *, long unsigned int);
    void (*set_cr4)(struct kvm_vcpu *, long unsigned int);
    int (*set_efer)(struct kvm_vcpu *, u64);
    void (*get_idt)(struct kvm_vcpu *, struct desc_ptr *);
    void (*set_idt)(struct kvm_vcpu *, struct desc_ptr *);
    void (*get_gdt)(struct kvm_vcpu *, struct desc_ptr *);
    void (*set_gdt)(struct kvm_vcpu *, struct desc_ptr *);
    void (*sync_dirty_debug_regs)(struct kvm_vcpu *);
    void (*set_dr7)(struct kvm_vcpu *, long unsigned int);
    void (*cache_reg)(struct kvm_vcpu *, enum kvm_reg);
    long unsigned int (*get_rflags)(struct kvm_vcpu *);
    void (*set_rflags)(struct kvm_vcpu *, long unsigned int);
    bool (*get_if_flag)(struct kvm_vcpu *);
    void (*flush_tlb_all)(struct kvm_vcpu *);
    void (*flush_tlb_current)(struct kvm_vcpu *);
    int (*flush_remote_tlbs)(struct kvm *);
    int (*flush_remote_tlbs_range)(struct kvm *, gfn_t, gfn_t);
    void (*flush_tlb_gva)(struct kvm_vcpu *, gva_t);
    void (*flush_tlb_guest)(struct kvm_vcpu *);
    int (*vcpu_pre_run)(struct kvm_vcpu *);
    enum exit_fastpath_completion (*vcpu_run)(struct kvm_vcpu *);
    int (*handle_exit)(struct kvm_vcpu *, enum exit_fastpath_completion);
    int (*skip_emulated_instruction)(struct kvm_vcpu *);
    void (*update_emulated_instruction)(struct kvm_vcpu *);
    void (*set_interrupt_shadow)(struct kvm_vcpu *, int);
    u32 (*get_interrupt_shadow)(struct kvm_vcpu *);
    void (*patch_hypercall)(struct kvm_vcpu *, unsigned char *);
    void (*inject_irq)(struct kvm_vcpu *, bool);
    void (*inject_nmi)(struct kvm_vcpu *);
    void (*inject_exception)(struct kvm_vcpu *);
    void (*cancel_injection)(struct kvm_vcpu *);
    int (*interrupt_allowed)(struct kvm_vcpu *, bool);
    int (*nmi_allowed)(struct kvm_vcpu *, bool);
    bool (*get_nmi_mask)(struct kvm_vcpu *);
    void (*set_nmi_mask)(struct kvm_vcpu *, bool);
    bool (*is_vnmi_pending)(struct kvm_vcpu *);
    bool (*set_vnmi_pending)(struct kvm_vcpu *);
    void (*enable_nmi_window)(struct kvm_vcpu *);
    void (*enable_irq_window)(struct kvm_vcpu *);
    void (*update_cr8_intercept)(struct kvm_vcpu *, int, int);
    bool (*check_apicv_inhibit_reasons)(enum kvm_apicv_inhibit);
    const long unsigned int required_apicv_inhibits;
    bool allow_apicv_in_x2apic_without_x2apic_virtualization;
    void (*refresh_apicv_exec_ctrl)(struct kvm_vcpu *);
    void (*hwapic_irr_update)(struct kvm_vcpu *, int);
    void (*hwapic_isr_update)(int);
    bool (*guest_apic_has_interrupt)(struct kvm_vcpu *);
    void (*load_eoi_exitmap)(struct kvm_vcpu *, u64 *);
    void (*set_virtual_apic_mode)(struct kvm_vcpu *);
    void (*set_apic_access_page_addr)(struct kvm_vcpu *);
    void (*deliver_interrupt)(struct kvm_lapic *, int, int, int);
    int (*sync_pir_to_irr)(struct kvm_vcpu *);
    int (*set_tss_addr)(struct kvm *, unsigned int);
    int (*set_identity_map_addr)(struct kvm *, u64);
    u8 (*get_mt_mask)(struct kvm_vcpu *, gfn_t, bool);
    void (*load_mmu_pgd)(struct kvm_vcpu *, hpa_t, int);
    bool (*has_wbinvd_exit)();
    u64 (*get_l2_tsc_offset)(struct kvm_vcpu *);
    u64 (*get_l2_tsc_multiplier)(struct kvm_vcpu *);
    void (*write_tsc_offset)(struct kvm_vcpu *, u64);
    void (*write_tsc_multiplier)(struct kvm_vcpu *, u64);
    void (*get_exit_info)(struct kvm_vcpu *, u32 *, u64 *, u64 *, u32 *, u32 *);
    int (*check_intercept)(struct kvm_vcpu *, struct x86_instruction_info *, enum x86_intercept_stage, struct x86_exception *);
    void (*handle_exit_irqoff)(struct kvm_vcpu *);
    void (*request_immediate_exit)(struct kvm_vcpu *);
    void (*sched_in)(struct kvm_vcpu *, int);
    int cpu_dirty_log_size;
    void (*update_cpu_dirty_logging)(struct kvm_vcpu *);
    const struct kvm_x86_nested_ops *nested_ops;
    void (*vcpu_blocking)(struct kvm_vcpu *);
    void (*vcpu_unblocking)(struct kvm_vcpu *);
    int (*pi_update_irte)(struct kvm *, unsigned int, uint32_t, bool);
    void (*pi_start_assignment)(struct kvm *);
    void (*apicv_post_state_restore)(struct kvm_vcpu *);
    bool (*dy_apicv_has_pending_interrupt)(struct kvm_vcpu *);
    int (*set_hv_timer)(struct kvm_vcpu *, u64, bool *);
    void (*cancel_hv_timer)(struct kvm_vcpu *);
    void (*setup_mce)(struct kvm_vcpu *);
    int (*smi_allowed)(struct kvm_vcpu *, bool);
    int (*enter_smm)(struct kvm_vcpu *, union kvm_smram *);
    int (*leave_smm)(struct kvm_vcpu *, const union kvm_smram *);
    void (*enable_smi_window)(struct kvm_vcpu *);
    int (*mem_enc_ioctl)(struct kvm *, void *);
    int (*mem_enc_register_region)(struct kvm *, struct kvm_enc_region *);
    int (*mem_enc_unregister_region)(struct kvm *, struct kvm_enc_region *);
    int (*vm_copy_enc_context_from)(struct kvm *, unsigned int);
    int (*vm_move_enc_context_from)(struct kvm *, unsigned int);
    void (*guest_memory_reclaimed)(struct kvm *);
    int (*get_msr_feature)(struct kvm_msr_entry *);
    bool (*can_emulate_instruction)(struct kvm_vcpu *, int, void *, int);
    bool (*apic_init_signal_blocked)(struct kvm_vcpu *);
    int (*enable_l2_tlb_flush)(struct kvm_vcpu *);
    void (*migrate_timers)(struct kvm_vcpu *);
    void (*msr_filter_changed)(struct kvm_vcpu *);
    int (*complete_emulated_msr)(struct kvm_vcpu *, int);
    void (*vcpu_deliver_sipi_vector)(struct kvm_vcpu *, u8);
    long unsigned int (*vcpu_get_apicv_inhibit_reasons)(struct kvm_vcpu *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kvm_x86_ops {
    const char *name;
    int (*check_processor_compatibility)();
    int (*hardware_enable)();
    void (*hardware_disable)();
    void (*hardware_unsetup)();
    bool (*has_emulated_msr)(struct kvm *, u32);
    void (*vcpu_after_set_cpuid)(struct kvm_vcpu *);
    unsigned int vm_size;
    int (*vm_init)(struct kvm *);
    void (*vm_destroy)(struct kvm *);
    int (*vcpu_precreate)(struct kvm *);
    int (*vcpu_create)(struct kvm_vcpu *);
    void (*vcpu_free)(struct kvm_vcpu *);
    void (*vcpu_reset)(struct kvm_vcpu *, bool);
    void (*prepare_switch_to_guest)(struct kvm_vcpu *);
    void (*vcpu_load)(struct kvm_vcpu *, int);
    void (*vcpu_put)(struct kvm_vcpu *);
    void (*update_exception_bitmap)(struct kvm_vcpu *);
    int (*get_msr)(struct kvm_vcpu *, struct msr_data *);
    int (*set_msr)(struct kvm_vcpu *, struct msr_data *);
    u64 (*get_segment_base)(struct kvm_vcpu *, int);
    void (*get_segment)(struct kvm_vcpu *, struct kvm_segment *, int);
    int (*get_cpl)(struct kvm_vcpu *);
    void (*set_segment)(struct kvm_vcpu *, struct kvm_segment *, int);
    void (*get_cs_db_l_bits)(struct kvm_vcpu *, int *, int *);
    bool (*is_valid_cr0)(struct kvm_vcpu *, long unsigned int);
    void (*set_cr0)(struct kvm_vcpu *, long unsigned int);
    void (*post_set_cr3)(struct kvm_vcpu *, long unsigned int);
    bool (*is_valid_cr4)(struct kvm_vcpu *, long unsigned int);
    void (*set_cr4)(struct kvm_vcpu *, long unsigned int);
    int (*set_efer)(struct kvm_vcpu *, u64);
    void (*get_idt)(struct kvm_vcpu *, struct desc_ptr *);
    void (*set_idt)(struct kvm_vcpu *, struct desc_ptr *);
    void (*get_gdt)(struct kvm_vcpu *, struct desc_ptr *);
    void (*set_gdt)(struct kvm_vcpu *, struct desc_ptr *);
    void (*sync_dirty_debug_regs)(struct kvm_vcpu *);
    void (*set_dr7)(struct kvm_vcpu *, long unsigned int);
    void (*cache_reg)(struct kvm_vcpu *, enum kvm_reg);
    long unsigned int (*get_rflags)(struct kvm_vcpu *);
    void (*set_rflags)(struct kvm_vcpu *, long unsigned int);
    bool (*get_if_flag)(struct kvm_vcpu *);
    void (*flush_tlb_all)(struct kvm_vcpu *);
    void (*flush_tlb_current)(struct kvm_vcpu *);
    int (*flush_remote_tlbs)(struct kvm *);
    int (*flush_remote_tlbs_range)(struct kvm *, gfn_t, gfn_t);
    void (*flush_tlb_gva)(struct kvm_vcpu *, gva_t);
    void (*flush_tlb_guest)(struct kvm_vcpu *);
    int (*vcpu_pre_run)(struct kvm_vcpu *);
    enum exit_fastpath_completion (*vcpu_run)(struct kvm_vcpu *);
    int (*handle_exit)(struct kvm_vcpu *, enum exit_fastpath_completion);
    int (*skip_emulated_instruction)(struct kvm_vcpu *);
    void (*update_emulated_instruction)(struct kvm_vcpu *);
    void (*set_interrupt_shadow)(struct kvm_vcpu *, int);
    u32 (*get_interrupt_shadow)(struct kvm_vcpu *);
    void (*patch_hypercall)(struct kvm_vcpu *, unsigned char *);
    void (*inject_irq)(struct kvm_vcpu *, bool);
    void (*inject_nmi)(struct kvm_vcpu *);
    void (*inject_exception)(struct kvm_vcpu *);
    void (*cancel_injection)(struct kvm_vcpu *);
    int (*interrupt_allowed)(struct kvm_vcpu *, bool);
    int (*nmi_allowed)(struct kvm_vcpu *, bool);
    bool (*get_nmi_mask)(struct kvm_vcpu *);
    void (*set_nmi_mask)(struct kvm_vcpu *, bool);
    bool (*is_vnmi_pending)(struct kvm_vcpu *);
    bool (*set_vnmi_pending)(struct kvm_vcpu *);
    void (*enable_nmi_window)(struct kvm_vcpu *);
    void (*enable_irq_window)(struct kvm_vcpu *);
    void (*update_cr8_intercept)(struct kvm_vcpu *, int, int);
    bool (*check_apicv_inhibit_reasons)(enum kvm_apicv_inhibit);
    const long unsigned int required_apicv_inhibits;
    bool allow_apicv_in_x2apic_without_x2apic_virtualization;
    void (*refresh_apicv_exec_ctrl)(struct kvm_vcpu *);
    void (*hwapic_irr_update)(struct kvm_vcpu *, int);
    void (*hwapic_isr_update)(int);
    bool (*guest_apic_has_interrupt)(struct kvm_vcpu *);
    void (*load_eoi_exitmap)(struct kvm_vcpu *, u64 *);
    void (*set_virtual_apic_mode)(struct kvm_vcpu *);
    void (*set_apic_access_page_addr)(struct kvm_vcpu *);
    void (*deliver_interrupt)(struct kvm_lapic *, int, int, int);
    int (*sync_pir_to_irr)(struct kvm_vcpu *);
    int (*set_tss_addr)(struct kvm *, unsigned int);
    int (*set_identity_map_addr)(struct kvm *, u64);
    u8 (*get_mt_mask)(struct kvm_vcpu *, gfn_t, bool);
    void (*load_mmu_pgd)(struct kvm_vcpu *, hpa_t, int);
    bool (*has_wbinvd_exit)();
    u64 (*get_l2_tsc_offset)(struct kvm_vcpu *);
    u64 (*get_l2_tsc_multiplier)(struct kvm_vcpu *);
    void (*write_tsc_offset)(struct kvm_vcpu *);
    void (*write_tsc_multiplier)(struct kvm_vcpu *);
    void (*get_exit_info)(struct kvm_vcpu *, u32 *, u64 *, u64 *, u32 *, u32 *);
    int (*check_intercept)(struct kvm_vcpu *, struct x86_instruction_info *, enum x86_intercept_stage, struct x86_exception *);
    void (*handle_exit_irqoff)(struct kvm_vcpu *);
    void (*request_immediate_exit)(struct kvm_vcpu *);
    void (*sched_in)(struct kvm_vcpu *, int);
    int cpu_dirty_log_size;
    void (*update_cpu_dirty_logging)(struct kvm_vcpu *);
    const struct kvm_x86_nested_ops *nested_ops;
    void (*vcpu_blocking)(struct kvm_vcpu *);
    void (*vcpu_unblocking)(struct kvm_vcpu *);
    int (*pi_update_irte)(struct kvm *, unsigned int, uint32_t, bool);
    void (*pi_start_assignment)(struct kvm *);
    void (*apicv_pre_state_restore)(struct kvm_vcpu *);
    void (*apicv_post_state_restore)(struct kvm_vcpu *);
    bool (*dy_apicv_has_pending_interrupt)(struct kvm_vcpu *);
    int (*set_hv_timer)(struct kvm_vcpu *, u64, bool *);
    void (*cancel_hv_timer)(struct kvm_vcpu *);
    void (*setup_mce)(struct kvm_vcpu *);
    int (*smi_allowed)(struct kvm_vcpu *, bool);
    int (*enter_smm)(struct kvm_vcpu *, union kvm_smram *);
    int (*leave_smm)(struct kvm_vcpu *, const union kvm_smram *);
    void (*enable_smi_window)(struct kvm_vcpu *);
    int (*mem_enc_ioctl)(struct kvm *, void *);
    int (*mem_enc_register_region)(struct kvm *, struct kvm_enc_region *);
    int (*mem_enc_unregister_region)(struct kvm *, struct kvm_enc_region *);
    int (*vm_copy_enc_context_from)(struct kvm *, unsigned int);
    int (*vm_move_enc_context_from)(struct kvm *, unsigned int);
    void (*guest_memory_reclaimed)(struct kvm *);
    int (*get_msr_feature)(struct kvm_msr_entry *);
    int (*check_emulate_instruction)(struct kvm_vcpu *, int, void *, int);
    bool (*apic_init_signal_blocked)(struct kvm_vcpu *);
    int (*enable_l2_tlb_flush)(struct kvm_vcpu *);
    void (*migrate_timers)(struct kvm_vcpu *);
    void (*msr_filter_changed)(struct kvm_vcpu *);
    int (*complete_emulated_msr)(struct kvm_vcpu *, int);
    void (*vcpu_deliver_sipi_vector)(struct kvm_vcpu *, u8);
    long unsigned int (*vcpu_get_apicv_inhibit_reasons)(struct kvm_vcpu *);
    gva_t (*get_untagged_addr)(struct kvm_vcpu *, gva_t, unsigned int);
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
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool (*get_if_flag)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field added. </b>
<code>u64 (*get_l2_tsc_offset)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field added. </b>
<code>u64 (*get_l2_tsc_multiplier)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*write_tsc_offset)(struct kvm_vcpu *, u64)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*write_tsc_multiplier)(struct kvm_vcpu *, u64)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*enter_smm)(struct kvm_vcpu *, char *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*leave_smm)(struct kvm_vcpu *, const char *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*pre_update_apicv_exec_ctrl)(struct kvm *, bool)</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 (*write_l1_tsc_offset)(struct kvm_vcpu *, u64)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*pre_enter_smm)(struct kvm_vcpu *, char *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*pre_leave_smm)(struct kvm_vcpu *, const char *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const char *name</code>
</li>
<li>
<b>Field added. </b>
<code>void (*prepare_switch_to_guest)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*post_set_cr3)(struct kvm_vcpu *, long unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*flush_tlb_all)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*flush_tlb_current)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*flush_tlb_gva)(struct kvm_vcpu *, gva_t)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*flush_tlb_guest)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*vcpu_pre_run)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field added. </b>
<code>enum exit_fastpath_completion (*vcpu_run)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*inject_irq)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*inject_nmi)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*deliver_interrupt)(struct kvm_lapic *, int, int, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*pi_update_irte)(struct kvm *, unsigned int, uint32_t, bool)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*pi_start_assignment)(struct kvm *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*mem_enc_ioctl)(struct kvm *, void *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*mem_enc_register_region)(struct kvm *, struct kvm_enc_region *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*mem_enc_unregister_region)(struct kvm *, struct kvm_enc_region *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*vm_move_enc_context_from)(struct kvm *, unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*guest_memory_reclaimed)(struct kvm *)</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int (*vcpu_get_apicv_inhibit_reasons)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field removed. </b>
<code>bool (*cpu_has_accelerated_tpr)()</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*prepare_guest_switch)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*tlb_flush_all)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*tlb_flush_current)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*tlb_flush_gva)(struct kvm_vcpu *, gva_t)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*tlb_flush_guest)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field removed. </b>
<code>enum exit_fastpath_completion (*run)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*set_irq)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*set_nmi)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*deliver_posted_interrupt)(struct kvm_vcpu *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>const struct kvm_pmu_ops *pmu_ops</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*pre_block)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*post_block)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*update_pi_irte)(struct kvm *, unsigned int, uint32_t, bool)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*start_assignment)(struct kvm *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*mem_enc_op)(struct kvm *, void *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*mem_enc_reg_region)(struct kvm *, struct kvm_enc_region *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*mem_enc_unreg_region)(struct kvm *, struct kvm_enc_region *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool (*check_apicv_inhibit_reasons)(ulong)</code> ➡️ <code>bool (*check_apicv_inhibit_reasons)(enum kvm_apicv_inhibit)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*get_exit_info)(struct kvm_vcpu *, u64 *, u64 *, u32 *, u32 *)</code> ➡️ <code>void (*get_exit_info)(struct kvm_vcpu *, u32 *, u64 *, u64 *, u32 *, u32 *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool (*can_emulate_instruction)(struct kvm_vcpu *, void *, int)</code> ➡️ <code>bool (*can_emulate_instruction)(struct kvm_vcpu *, int, void *, int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*vcpu_precreate)(struct kvm *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*inject_exception)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*enable_l2_tlb_flush)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*queue_exception)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*enable_direct_tlbflush)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*inject_irq)(struct kvm_vcpu *)</code> ➡️ <code>void (*inject_irq)(struct kvm_vcpu *, bool)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*hwapic_isr_update)(struct kvm_vcpu *, int)</code> ➡️ <code>void (*hwapic_isr_update)(int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>u64 (*get_mt_mask)(struct kvm_vcpu *, gfn_t, bool)</code> ➡️ <code>u8 (*get_mt_mask)(struct kvm_vcpu *, gfn_t, bool)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*enter_smm)(struct kvm_vcpu *, char *)</code> ➡️ <code>int (*enter_smm)(struct kvm_vcpu *, union kvm_smram *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*leave_smm)(struct kvm_vcpu *, const char *)</code> ➡️ <code>int (*leave_smm)(struct kvm_vcpu *, const union kvm_smram *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*check_processor_compatibility)()</code>
</li>
<li>
<b>Field added. </b>
<code>bool (*is_valid_cr0)(struct kvm_vcpu *, long unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*flush_remote_tlbs)(struct kvm *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*flush_remote_tlbs_range)(struct kvm *, gfn_t, gfn_t)</code>
</li>
<li>
<b>Field added. </b>
<code>bool (*is_vnmi_pending)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field added. </b>
<code>bool (*set_vnmi_pending)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field added. </b>
<code>const long unsigned int required_apicv_inhibits</code>
</li>
<li>
<b>Field added. </b>
<code>bool allow_apicv_in_x2apic_without_x2apic_virtualization</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*tlb_remote_flush)(struct kvm *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*tlb_remote_flush_with_range)(struct kvm *, struct kvm_tlb_range *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*apicv_pre_state_restore)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*check_emulate_instruction)(struct kvm_vcpu *, int, void *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>gva_t (*get_untagged_addr)(struct kvm_vcpu *, gva_t, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>bool (*can_emulate_instruction)(struct kvm_vcpu *, int, void *, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*write_tsc_offset)(struct kvm_vcpu *, u64)</code> ➡️ <code>void (*write_tsc_offset)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*write_tsc_multiplier)(struct kvm_vcpu *, u64)</code> ➡️ <code>void (*write_tsc_multiplier)(struct kvm_vcpu *)</code>
</li>
</ul>
</details>
</li>
</ul>
