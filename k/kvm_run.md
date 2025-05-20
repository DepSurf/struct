# Struct: <code>kvm_run</code>

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
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct kvm_run {
    __u8 request_interrupt_window;
    __u8 immediate_exit;
    __u8 padding1[6];
    __u32 exit_reason;
    __u8 ready_for_interrupt_injection;
    __u8 if_flag;
    __u16 flags;
    __u64 cr8;
    __u64 apic_base;
    struct (anon) hw;
    struct (anon) fail_entry;
    struct (anon) ex;
    struct (anon) io;
    struct (anon) debug;
    struct (anon) mmio;
    struct (anon) hypercall;
    struct (anon) tpr_access;
    struct (anon) s390_sieic;
    __u64 s390_reset_flags;
    struct (anon) s390_ucontrol;
    struct (anon) dcr;
    struct (anon) internal;
    struct (anon) osi;
    struct (anon) papr_hcall;
    struct (anon) s390_tsch;
    struct (anon) epr;
    struct (anon) system_event;
    struct (anon) s390_stsi;
    struct (anon) eoi;
    struct kvm_hyperv_exit hyperv;
    struct (anon) arm_nisv;
    struct (anon) msr;
    char padding[256];
    __u64 kvm_valid_regs;
    __u64 kvm_dirty_regs;
    union (anon) s;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kvm_run {
    __u8 request_interrupt_window;
    __u8 immediate_exit;
    __u8 padding1[6];
    __u32 exit_reason;
    __u8 ready_for_interrupt_injection;
    __u8 if_flag;
    __u16 flags;
    __u64 cr8;
    __u64 apic_base;
    struct (anon) hw;
    struct (anon) fail_entry;
    struct (anon) ex;
    struct (anon) io;
    struct (anon) debug;
    struct (anon) mmio;
    struct (anon) hypercall;
    struct (anon) tpr_access;
    struct (anon) s390_sieic;
    __u64 s390_reset_flags;
    struct (anon) s390_ucontrol;
    struct (anon) dcr;
    struct (anon) internal;
    struct (anon) osi;
    struct (anon) papr_hcall;
    struct (anon) s390_tsch;
    struct (anon) epr;
    struct (anon) system_event;
    struct (anon) s390_stsi;
    struct (anon) eoi;
    struct kvm_hyperv_exit hyperv;
    struct (anon) arm_nisv;
    struct (anon) msr;
    struct kvm_xen_exit xen;
    char padding[256];
    __u64 kvm_valid_regs;
    __u64 kvm_dirty_regs;
    union (anon) s;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kvm_run {
    __u8 request_interrupt_window;
    __u8 immediate_exit;
    __u8 padding1[6];
    __u32 exit_reason;
    __u8 ready_for_interrupt_injection;
    __u8 if_flag;
    __u16 flags;
    __u64 cr8;
    __u64 apic_base;
    struct (anon) hw;
    struct (anon) fail_entry;
    struct (anon) ex;
    struct (anon) io;
    struct (anon) debug;
    struct (anon) mmio;
    struct (anon) hypercall;
    struct (anon) tpr_access;
    struct (anon) s390_sieic;
    __u64 s390_reset_flags;
    struct (anon) s390_ucontrol;
    struct (anon) dcr;
    struct (anon) internal;
    struct (anon) emulation_failure;
    struct (anon) osi;
    struct (anon) papr_hcall;
    struct (anon) s390_tsch;
    struct (anon) epr;
    struct (anon) system_event;
    struct (anon) s390_stsi;
    struct (anon) eoi;
    struct kvm_hyperv_exit hyperv;
    struct (anon) arm_nisv;
    struct (anon) msr;
    struct kvm_xen_exit xen;
    char padding[256];
    __u64 kvm_valid_regs;
    __u64 kvm_dirty_regs;
    union (anon) s;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kvm_run {
    __u8 request_interrupt_window;
    __u8 immediate_exit;
    __u8 padding1[6];
    __u32 exit_reason;
    __u8 ready_for_interrupt_injection;
    __u8 if_flag;
    __u16 flags;
    __u64 cr8;
    __u64 apic_base;
    struct (anon) hw;
    struct (anon) fail_entry;
    struct (anon) ex;
    struct (anon) io;
    struct (anon) debug;
    struct (anon) mmio;
    struct (anon) hypercall;
    struct (anon) tpr_access;
    struct (anon) s390_sieic;
    __u64 s390_reset_flags;
    struct (anon) s390_ucontrol;
    struct (anon) dcr;
    struct (anon) internal;
    struct (anon) emulation_failure;
    struct (anon) osi;
    struct (anon) papr_hcall;
    struct (anon) s390_tsch;
    struct (anon) epr;
    struct (anon) system_event;
    struct (anon) s390_stsi;
    struct (anon) eoi;
    struct kvm_hyperv_exit hyperv;
    struct (anon) arm_nisv;
    struct (anon) msr;
    struct kvm_xen_exit xen;
    struct (anon) riscv_sbi;
    char padding[256];
    __u64 kvm_valid_regs;
    __u64 kvm_dirty_regs;
    union (anon) s;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kvm_run {
    __u8 request_interrupt_window;
    __u8 immediate_exit;
    __u8 padding1[6];
    __u32 exit_reason;
    __u8 ready_for_interrupt_injection;
    __u8 if_flag;
    __u16 flags;
    __u64 cr8;
    __u64 apic_base;
    struct (anon) hw;
    struct (anon) fail_entry;
    struct (anon) ex;
    struct (anon) io;
    struct (anon) debug;
    struct (anon) mmio;
    struct (anon) hypercall;
    struct (anon) tpr_access;
    struct (anon) s390_sieic;
    __u64 s390_reset_flags;
    struct (anon) s390_ucontrol;
    struct (anon) dcr;
    struct (anon) internal;
    struct (anon) emulation_failure;
    struct (anon) osi;
    struct (anon) papr_hcall;
    struct (anon) s390_tsch;
    struct (anon) epr;
    struct (anon) system_event;
    struct (anon) s390_stsi;
    struct (anon) eoi;
    struct kvm_hyperv_exit hyperv;
    struct (anon) arm_nisv;
    struct (anon) msr;
    struct kvm_xen_exit xen;
    struct (anon) riscv_sbi;
    struct (anon) riscv_csr;
    struct (anon) notify;
    char padding[256];
    __u64 kvm_valid_regs;
    __u64 kvm_dirty_regs;
    union (anon) s;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kvm_run {
    __u8 request_interrupt_window;
    __u8 immediate_exit;
    __u8 padding1[6];
    __u32 exit_reason;
    __u8 ready_for_interrupt_injection;
    __u8 if_flag;
    __u16 flags;
    __u64 cr8;
    __u64 apic_base;
    struct (anon) hw;
    struct (anon) fail_entry;
    struct (anon) ex;
    struct (anon) io;
    struct (anon) debug;
    struct (anon) mmio;
    struct (anon) hypercall;
    struct (anon) tpr_access;
    struct (anon) s390_sieic;
    __u64 s390_reset_flags;
    struct (anon) s390_ucontrol;
    struct (anon) dcr;
    struct (anon) internal;
    struct (anon) emulation_failure;
    struct (anon) osi;
    struct (anon) papr_hcall;
    struct (anon) s390_tsch;
    struct (anon) epr;
    struct (anon) system_event;
    struct (anon) s390_stsi;
    struct (anon) eoi;
    struct kvm_hyperv_exit hyperv;
    struct (anon) arm_nisv;
    struct (anon) msr;
    struct kvm_xen_exit xen;
    struct (anon) riscv_sbi;
    struct (anon) riscv_csr;
    struct (anon) notify;
    char padding[256];
    __u64 kvm_valid_regs;
    __u64 kvm_dirty_regs;
    union (anon) s;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kvm_run {
    __u8 request_interrupt_window;
    __u8 immediate_exit;
    __u8 padding1[6];
    __u32 exit_reason;
    __u8 ready_for_interrupt_injection;
    __u8 if_flag;
    __u16 flags;
    __u64 cr8;
    __u64 apic_base;
    struct (anon) hw;
    struct (anon) fail_entry;
    struct (anon) ex;
    struct (anon) io;
    struct (anon) debug;
    struct (anon) mmio;
    struct (anon) iocsr_io;
    struct (anon) hypercall;
    struct (anon) tpr_access;
    struct (anon) s390_sieic;
    __u64 s390_reset_flags;
    struct (anon) s390_ucontrol;
    struct (anon) dcr;
    struct (anon) internal;
    struct (anon) emulation_failure;
    struct (anon) osi;
    struct (anon) papr_hcall;
    struct (anon) s390_tsch;
    struct (anon) epr;
    struct (anon) system_event;
    struct (anon) s390_stsi;
    struct (anon) eoi;
    struct kvm_hyperv_exit hyperv;
    struct (anon) arm_nisv;
    struct (anon) msr;
    struct kvm_xen_exit xen;
    struct (anon) riscv_sbi;
    struct (anon) riscv_csr;
    struct (anon) notify;
    struct (anon) memory_fault;
    char padding[256];
    __u64 kvm_valid_regs;
    __u64 kvm_dirty_regs;
    union (anon) s;
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct kvm_run {
    __u8 request_interrupt_window;
    __u8 immediate_exit;
    __u8 padding1[6];
    __u32 exit_reason;
    __u8 ready_for_interrupt_injection;
    __u8 if_flag;
    __u16 flags;
    __u64 cr8;
    __u64 apic_base;
    struct (anon) hw;
    struct (anon) fail_entry;
    struct (anon) ex;
    struct (anon) io;
    struct (anon) debug;
    struct (anon) mmio;
    struct (anon) hypercall;
    struct (anon) tpr_access;
    struct (anon) s390_sieic;
    __u64 s390_reset_flags;
    struct (anon) s390_ucontrol;
    struct (anon) dcr;
    struct (anon) internal;
    struct (anon) osi;
    struct (anon) papr_hcall;
    struct (anon) s390_tsch;
    struct (anon) epr;
    struct (anon) system_event;
    struct (anon) s390_stsi;
    struct (anon) eoi;
    struct kvm_hyperv_exit hyperv;
    char padding[256];
    __u64 kvm_valid_regs;
    __u64 kvm_dirty_regs;
    union (anon) s;
};
```
</details>
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct kvm_run {
    __u8 request_interrupt_window;
    __u8 immediate_exit;
    __u8 padding1[6];
    __u32 exit_reason;
    __u8 ready_for_interrupt_injection;
    __u8 if_flag;
    __u16 flags;
    __u64 cr8;
    __u64 apic_base;
    struct (anon) hw;
    struct (anon) fail_entry;
    struct (anon) ex;
    struct (anon) io;
    struct (anon) debug;
    struct (anon) mmio;
    struct (anon) hypercall;
    struct (anon) tpr_access;
    struct (anon) s390_sieic;
    __u64 s390_reset_flags;
    struct (anon) s390_ucontrol;
    struct (anon) dcr;
    struct (anon) internal;
    struct (anon) osi;
    struct (anon) papr_hcall;
    struct (anon) s390_tsch;
    struct (anon) epr;
    struct (anon) system_event;
    struct (anon) s390_stsi;
    struct (anon) eoi;
    struct kvm_hyperv_exit hyperv;
    char padding[256];
    __u64 kvm_valid_regs;
    __u64 kvm_dirty_regs;
    union (anon) s;
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
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct kvm_xen_exit xen</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct (anon) emulation_failure</code>
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
<code>struct (anon) riscv_sbi</code>
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
<code>struct (anon) riscv_csr</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) notify</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct (anon) iocsr_io</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) memory_fault</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Arch</b>
<ul>
</ul>
