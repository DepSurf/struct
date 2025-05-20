# Struct: <code>paca_struct</code>

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
struct paca_struct {
    struct lppaca *lppaca_ptr;
    u16 paca_index;
    u16 lock_token;
    u64 kernel_toc;
    u64 kernelbase;
    u64 kernel_msr;
    void *emergency_sp;
    u64 data_offset;
    s16 hw_cpu_id;
    u8 cpu_start;
    u8 kexec_state;
    struct slb_shadow *slb_shadow_ptr;
    struct dtl_entry *dispatch_log;
    struct dtl_entry *dispatch_log_end;
    u64 dscr_default;
    u64 exgen[10];
    u64 exslb[10];
    u16 vmalloc_sllp;
    u8 slb_cache_ptr;
    u8 stab_rr;
    u32 slb_used_bitmap;
    u32 slb_kern_bitmap;
    u32 slb_cache[8];
    mm_context_id_t mm_ctx_id;
    unsigned char mm_ctx_low_slices_psize[8];
    unsigned char mm_ctx_high_slices_psize[2048];
    long unsigned int mm_ctx_slb_addr_limit;
    struct task_struct *__current;
    u64 kstack;
    u64 saved_r1;
    u64 saved_msr;
    u8 irq_soft_mask;
    u8 irq_happened;
    u8 irq_work_pending;
    u8 pmcregs_in_use;
    u64 sprg_vdso;
    u64 tm_scratch;
    long unsigned int idle_state;
    u8 thread_idle_state;
    u8 subcore_sibling_mask;
    u64 requested_psscr;
    atomic_t dont_stop;
    u64 exnmi[10];
    u64 exmc[10];
    void *nmi_emergency_sp;
    void *mc_emergency_sp;
    u16 in_nmi;
    u16 in_mce;
    u8 hmi_event_available;
    u8 hmi_p9_special_emu;
    u8 ftrace_enabled;
    struct cpu_accounting_data accounting;
    u64 dtl_ridx;
    struct dtl_entry *dtl_curr;
    struct kvmppc_book3s_shadow_vcpu shadow_vcpu;
    struct kvmppc_host_state kvm_hstate;
    struct sibling_subcore_state *sibling_subcore_state;
    u64 exrfi[10];
    void *rfi_flush_fallback_area;
    u64 l1d_flush_size;
    u8 *mce_data_buf;
    struct slb_entry *mce_faulty_slbs;
    u16 slb_save_cache_ptr;
    long unsigned int canary;
    struct mmiowb_state mmiowb_state;
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
