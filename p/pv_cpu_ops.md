# Struct: <code>pv_cpu_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct pv_cpu_ops {
    long unsigned int (*get_debugreg)(int);
    void (*set_debugreg)(int, long unsigned int);
    void (*clts)();
    long unsigned int (*read_cr0)();
    void (*write_cr0)(long unsigned int);
    long unsigned int (*read_cr4_safe)();
    long unsigned int (*read_cr4)();
    void (*write_cr4)(long unsigned int);
    long unsigned int (*read_cr8)();
    void (*write_cr8)(long unsigned int);
    void (*load_tr_desc)();
    void (*load_gdt)(const struct desc_ptr *);
    void (*load_idt)(const struct desc_ptr *);
    void (*store_idt)(struct desc_ptr *);
    void (*set_ldt)(const void *, unsigned int);
    long unsigned int (*store_tr)();
    void (*load_tls)(struct thread_struct *, unsigned int);
    void (*load_gs_index)(unsigned int);
    void (*write_ldt_entry)(struct desc_struct *, int, const void *);
    void (*write_gdt_entry)(struct desc_struct *, int, const void *, int);
    void (*write_idt_entry)(gate_desc *, int, const gate_desc *);
    void (*alloc_ldt)(struct desc_struct *, unsigned int);
    void (*free_ldt)(struct desc_struct *, unsigned int);
    void (*load_sp0)(struct tss_struct *, struct thread_struct *);
    void (*set_iopl_mask)(unsigned int);
    void (*wbinvd)();
    void (*io_delay)();
    void (*cpuid)(unsigned int *, unsigned int *, unsigned int *, unsigned int *);
    u64 (*read_msr)(unsigned int, int *);
    int (*write_msr)(unsigned int, unsigned int, unsigned int);
    u64 (*read_pmc)(int);
    void (*usergs_sysret64)();
    void (*usergs_sysret32)();
    void (*iret)();
    void (*swapgs)();
    void (*start_context_switch)(struct task_struct *);
    void (*end_context_switch)(struct task_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct pv_cpu_ops {
    long unsigned int (*get_debugreg)(int);
    void (*set_debugreg)(int, long unsigned int);
    void (*clts)();
    long unsigned int (*read_cr0)();
    void (*write_cr0)(long unsigned int);
    long unsigned int (*read_cr4_safe)();
    long unsigned int (*read_cr4)();
    void (*write_cr4)(long unsigned int);
    long unsigned int (*read_cr8)();
    void (*write_cr8)(long unsigned int);
    void (*load_tr_desc)();
    void (*load_gdt)(const struct desc_ptr *);
    void (*load_idt)(const struct desc_ptr *);
    void (*store_idt)(struct desc_ptr *);
    void (*set_ldt)(const void *, unsigned int);
    long unsigned int (*store_tr)();
    void (*load_tls)(struct thread_struct *, unsigned int);
    void (*load_gs_index)(unsigned int);
    void (*write_ldt_entry)(struct desc_struct *, int, const void *);
    void (*write_gdt_entry)(struct desc_struct *, int, const void *, int);
    void (*write_idt_entry)(gate_desc *, int, const gate_desc *);
    void (*alloc_ldt)(struct desc_struct *, unsigned int);
    void (*free_ldt)(struct desc_struct *, unsigned int);
    void (*load_sp0)(struct tss_struct *, struct thread_struct *);
    void (*set_iopl_mask)(unsigned int);
    void (*wbinvd)();
    void (*io_delay)();
    void (*cpuid)(unsigned int *, unsigned int *, unsigned int *, unsigned int *);
    u64 (*read_msr)(unsigned int);
    void (*write_msr)(unsigned int, unsigned int, unsigned int);
    u64 (*read_msr_safe)(unsigned int, int *);
    int (*write_msr_safe)(unsigned int, unsigned int, unsigned int);
    u64 (*read_pmc)(int);
    void (*usergs_sysret64)();
    void (*iret)();
    void (*swapgs)();
    void (*start_context_switch)(struct task_struct *);
    void (*end_context_switch)(struct task_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct pv_cpu_ops {
    long unsigned int (*get_debugreg)(int);
    void (*set_debugreg)(int, long unsigned int);
    long unsigned int (*read_cr0)();
    void (*write_cr0)(long unsigned int);
    long unsigned int (*read_cr4)();
    void (*write_cr4)(long unsigned int);
    long unsigned int (*read_cr8)();
    void (*write_cr8)(long unsigned int);
    void (*load_tr_desc)();
    void (*load_gdt)(const struct desc_ptr *);
    void (*load_idt)(const struct desc_ptr *);
    void (*store_idt)(struct desc_ptr *);
    void (*set_ldt)(const void *, unsigned int);
    long unsigned int (*store_tr)();
    void (*load_tls)(struct thread_struct *, unsigned int);
    void (*load_gs_index)(unsigned int);
    void (*write_ldt_entry)(struct desc_struct *, int, const void *);
    void (*write_gdt_entry)(struct desc_struct *, int, const void *, int);
    void (*write_idt_entry)(gate_desc *, int, const gate_desc *);
    void (*alloc_ldt)(struct desc_struct *, unsigned int);
    void (*free_ldt)(struct desc_struct *, unsigned int);
    void (*load_sp0)(struct tss_struct *, struct thread_struct *);
    void (*set_iopl_mask)(unsigned int);
    void (*wbinvd)();
    void (*io_delay)();
    void (*cpuid)(unsigned int *, unsigned int *, unsigned int *, unsigned int *);
    u64 (*read_msr)(unsigned int);
    void (*write_msr)(unsigned int, unsigned int, unsigned int);
    u64 (*read_msr_safe)(unsigned int, int *);
    int (*write_msr_safe)(unsigned int, unsigned int, unsigned int);
    u64 (*read_pmc)(int);
    void (*usergs_sysret64)();
    void (*iret)();
    void (*swapgs)();
    void (*start_context_switch)(struct task_struct *);
    void (*end_context_switch)(struct task_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct pv_cpu_ops {
    long unsigned int (*get_debugreg)(int);
    void (*set_debugreg)(int, long unsigned int);
    long unsigned int (*read_cr0)();
    void (*write_cr0)(long unsigned int);
    long unsigned int (*read_cr4)();
    void (*write_cr4)(long unsigned int);
    long unsigned int (*read_cr8)();
    void (*write_cr8)(long unsigned int);
    void (*load_tr_desc)();
    void (*load_gdt)(const struct desc_ptr *);
    void (*load_idt)(const struct desc_ptr *);
    void (*store_idt)(struct desc_ptr *);
    void (*set_ldt)(const void *, unsigned int);
    long unsigned int (*store_tr)();
    void (*load_tls)(struct thread_struct *, unsigned int);
    void (*load_gs_index)(unsigned int);
    void (*write_ldt_entry)(struct desc_struct *, int, const void *);
    void (*write_gdt_entry)(struct desc_struct *, int, const void *, int);
    void (*write_idt_entry)(gate_desc *, int, const gate_desc *);
    void (*alloc_ldt)(struct desc_struct *, unsigned int);
    void (*free_ldt)(struct desc_struct *, unsigned int);
    void (*load_sp0)(struct tss_struct *, struct thread_struct *);
    void (*set_iopl_mask)(unsigned int);
    void (*wbinvd)();
    void (*io_delay)();
    void (*cpuid)(unsigned int *, unsigned int *, unsigned int *, unsigned int *);
    u64 (*read_msr)(unsigned int);
    void (*write_msr)(unsigned int, unsigned int, unsigned int);
    u64 (*read_msr_safe)(unsigned int, int *);
    int (*write_msr_safe)(unsigned int, unsigned int, unsigned int);
    u64 (*read_pmc)(int);
    void (*usergs_sysret64)();
    void (*iret)();
    void (*swapgs)();
    void (*start_context_switch)(struct task_struct *);
    void (*end_context_switch)(struct task_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct pv_cpu_ops {
    long unsigned int (*get_debugreg)(int);
    void (*set_debugreg)(int, long unsigned int);
    long unsigned int (*read_cr0)();
    void (*write_cr0)(long unsigned int);
    void (*write_cr4)(long unsigned int);
    long unsigned int (*read_cr8)();
    void (*write_cr8)(long unsigned int);
    void (*load_tr_desc)();
    void (*load_gdt)(const struct desc_ptr *);
    void (*load_idt)(const struct desc_ptr *);
    void (*set_ldt)(const void *, unsigned int);
    long unsigned int (*store_tr)();
    void (*load_tls)(struct thread_struct *, unsigned int);
    void (*load_gs_index)(unsigned int);
    void (*write_ldt_entry)(struct desc_struct *, int, const void *);
    void (*write_gdt_entry)(struct desc_struct *, int, const void *, int);
    void (*write_idt_entry)(gate_desc *, int, const gate_desc *);
    void (*alloc_ldt)(struct desc_struct *, unsigned int);
    void (*free_ldt)(struct desc_struct *, unsigned int);
    void (*load_sp0)(long unsigned int);
    void (*set_iopl_mask)(unsigned int);
    void (*wbinvd)();
    void (*io_delay)();
    void (*cpuid)(unsigned int *, unsigned int *, unsigned int *, unsigned int *);
    u64 (*read_msr)(unsigned int);
    void (*write_msr)(unsigned int, unsigned int, unsigned int);
    u64 (*read_msr_safe)(unsigned int, int *);
    int (*write_msr_safe)(unsigned int, unsigned int, unsigned int);
    u64 (*read_pmc)(int);
    void (*usergs_sysret64)();
    void (*iret)();
    void (*swapgs)();
    void (*start_context_switch)(struct task_struct *);
    void (*end_context_switch)(struct task_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct pv_cpu_ops {
    long unsigned int (*get_debugreg)(int);
    void (*set_debugreg)(int, long unsigned int);
    long unsigned int (*read_cr0)();
    void (*write_cr0)(long unsigned int);
    void (*write_cr4)(long unsigned int);
    long unsigned int (*read_cr8)();
    void (*write_cr8)(long unsigned int);
    void (*load_tr_desc)();
    void (*load_gdt)(const struct desc_ptr *);
    void (*load_idt)(const struct desc_ptr *);
    void (*set_ldt)(const void *, unsigned int);
    long unsigned int (*store_tr)();
    void (*load_tls)(struct thread_struct *, unsigned int);
    void (*load_gs_index)(unsigned int);
    void (*write_ldt_entry)(struct desc_struct *, int, const void *);
    void (*write_gdt_entry)(struct desc_struct *, int, const void *, int);
    void (*write_idt_entry)(gate_desc *, int, const gate_desc *);
    void (*alloc_ldt)(struct desc_struct *, unsigned int);
    void (*free_ldt)(struct desc_struct *, unsigned int);
    void (*load_sp0)(long unsigned int);
    void (*set_iopl_mask)(unsigned int);
    void (*wbinvd)();
    void (*io_delay)();
    void (*cpuid)(unsigned int *, unsigned int *, unsigned int *, unsigned int *);
    u64 (*read_msr)(unsigned int);
    void (*write_msr)(unsigned int, unsigned int, unsigned int);
    u64 (*read_msr_safe)(unsigned int, int *);
    int (*write_msr_safe)(unsigned int, unsigned int, unsigned int);
    u64 (*read_pmc)(int);
    void (*usergs_sysret64)();
    void (*iret)();
    void (*swapgs)();
    void (*start_context_switch)(struct task_struct *);
    void (*end_context_switch)(struct task_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct pv_cpu_ops {
    void (*io_delay)();
    long unsigned int (*get_debugreg)(int);
    void (*set_debugreg)(int, long unsigned int);
    long unsigned int (*read_cr0)();
    void (*write_cr0)(long unsigned int);
    void (*write_cr4)(long unsigned int);
    long unsigned int (*read_cr8)();
    void (*write_cr8)(long unsigned int);
    void (*load_tr_desc)();
    void (*load_gdt)(const struct desc_ptr *);
    void (*load_idt)(const struct desc_ptr *);
    void (*set_ldt)(const void *, unsigned int);
    long unsigned int (*store_tr)();
    void (*load_tls)(struct thread_struct *, unsigned int);
    void (*load_gs_index)(unsigned int);
    void (*write_ldt_entry)(struct desc_struct *, int, const void *);
    void (*write_gdt_entry)(struct desc_struct *, int, const void *, int);
    void (*write_idt_entry)(gate_desc *, int, const gate_desc *);
    void (*alloc_ldt)(struct desc_struct *, unsigned int);
    void (*free_ldt)(struct desc_struct *, unsigned int);
    void (*load_sp0)(long unsigned int);
    void (*set_iopl_mask)(unsigned int);
    void (*wbinvd)();
    void (*cpuid)(unsigned int *, unsigned int *, unsigned int *, unsigned int *);
    u64 (*read_msr)(unsigned int);
    void (*write_msr)(unsigned int, unsigned int, unsigned int);
    u64 (*read_msr_safe)(unsigned int, int *);
    int (*write_msr_safe)(unsigned int, unsigned int, unsigned int);
    u64 (*read_pmc)(int);
    void (*usergs_sysret64)();
    void (*iret)();
    void (*swapgs)();
    void (*start_context_switch)(struct task_struct *);
    void (*end_context_switch)(struct task_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct pv_cpu_ops {
    void (*io_delay)();
    long unsigned int (*get_debugreg)(int);
    void (*set_debugreg)(int, long unsigned int);
    long unsigned int (*read_cr0)();
    void (*write_cr0)(long unsigned int);
    void (*write_cr4)(long unsigned int);
    long unsigned int (*read_cr8)();
    void (*write_cr8)(long unsigned int);
    void (*load_tr_desc)();
    void (*load_gdt)(const struct desc_ptr *);
    void (*load_idt)(const struct desc_ptr *);
    void (*set_ldt)(const void *, unsigned int);
    long unsigned int (*store_tr)();
    void (*load_tls)(struct thread_struct *, unsigned int);
    void (*load_gs_index)(unsigned int);
    void (*write_ldt_entry)(struct desc_struct *, int, const void *);
    void (*write_gdt_entry)(struct desc_struct *, int, const void *, int);
    void (*write_idt_entry)(gate_desc *, int, const gate_desc *);
    void (*alloc_ldt)(struct desc_struct *, unsigned int);
    void (*free_ldt)(struct desc_struct *, unsigned int);
    void (*load_sp0)(long unsigned int);
    void (*set_iopl_mask)(unsigned int);
    void (*wbinvd)();
    void (*cpuid)(unsigned int *, unsigned int *, unsigned int *, unsigned int *);
    u64 (*read_msr)(unsigned int);
    void (*write_msr)(unsigned int, unsigned int, unsigned int);
    u64 (*read_msr_safe)(unsigned int, int *);
    int (*write_msr_safe)(unsigned int, unsigned int, unsigned int);
    u64 (*read_pmc)(int);
    void (*usergs_sysret64)();
    void (*iret)();
    void (*swapgs)();
    void (*start_context_switch)(struct task_struct *);
    void (*end_context_switch)(struct task_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct pv_cpu_ops {
    void (*io_delay)();
    long unsigned int (*get_debugreg)(int);
    void (*set_debugreg)(int, long unsigned int);
    long unsigned int (*read_cr0)();
    void (*write_cr0)(long unsigned int);
    void (*write_cr4)(long unsigned int);
    void (*load_tr_desc)();
    void (*load_gdt)(const struct desc_ptr *);
    void (*load_idt)(const struct desc_ptr *);
    void (*set_ldt)(const void *, unsigned int);
    long unsigned int (*store_tr)();
    void (*load_tls)(struct thread_struct *, unsigned int);
    void (*load_gs_index)(unsigned int);
    void (*write_ldt_entry)(struct desc_struct *, int, const void *);
    void (*write_gdt_entry)(struct desc_struct *, int, const void *, int);
    void (*write_idt_entry)(gate_desc *, int, const gate_desc *);
    void (*alloc_ldt)(struct desc_struct *, unsigned int);
    void (*free_ldt)(struct desc_struct *, unsigned int);
    void (*load_sp0)(long unsigned int);
    void (*set_iopl_mask)(unsigned int);
    void (*wbinvd)();
    void (*cpuid)(unsigned int *, unsigned int *, unsigned int *, unsigned int *);
    u64 (*read_msr)(unsigned int);
    void (*write_msr)(unsigned int, unsigned int, unsigned int);
    u64 (*read_msr_safe)(unsigned int, int *);
    int (*write_msr_safe)(unsigned int, unsigned int, unsigned int);
    u64 (*read_pmc)(int);
    void (*usergs_sysret64)();
    void (*iret)();
    void (*swapgs)();
    void (*start_context_switch)(struct task_struct *);
    void (*end_context_switch)(struct task_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct pv_cpu_ops {
    void (*io_delay)();
    long unsigned int (*get_debugreg)(int);
    void (*set_debugreg)(int, long unsigned int);
    long unsigned int (*read_cr0)();
    void (*write_cr0)(long unsigned int);
    void (*write_cr4)(long unsigned int);
    void (*load_tr_desc)();
    void (*load_gdt)(const struct desc_ptr *);
    void (*load_idt)(const struct desc_ptr *);
    void (*set_ldt)(const void *, unsigned int);
    long unsigned int (*store_tr)();
    void (*load_tls)(struct thread_struct *, unsigned int);
    void (*load_gs_index)(unsigned int);
    void (*write_ldt_entry)(struct desc_struct *, int, const void *);
    void (*write_gdt_entry)(struct desc_struct *, int, const void *, int);
    void (*write_idt_entry)(gate_desc *, int, const gate_desc *);
    void (*alloc_ldt)(struct desc_struct *, unsigned int);
    void (*free_ldt)(struct desc_struct *, unsigned int);
    void (*load_sp0)(long unsigned int);
    void (*invalidate_io_bitmap)();
    void (*update_io_bitmap)();
    void (*wbinvd)();
    void (*cpuid)(unsigned int *, unsigned int *, unsigned int *, unsigned int *);
    u64 (*read_msr)(unsigned int);
    void (*write_msr)(unsigned int, unsigned int, unsigned int);
    u64 (*read_msr_safe)(unsigned int, int *);
    int (*write_msr_safe)(unsigned int, unsigned int, unsigned int);
    u64 (*read_pmc)(int);
    void (*usergs_sysret64)();
    void (*iret)();
    void (*swapgs)();
    void (*start_context_switch)(struct task_struct *);
    void (*end_context_switch)(struct task_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct pv_cpu_ops {
    void (*io_delay)();
    long unsigned int (*get_debugreg)(int);
    void (*set_debugreg)(int, long unsigned int);
    long unsigned int (*read_cr0)();
    void (*write_cr0)(long unsigned int);
    void (*write_cr4)(long unsigned int);
    void (*load_tr_desc)();
    void (*load_gdt)(const struct desc_ptr *);
    void (*load_idt)(const struct desc_ptr *);
    void (*set_ldt)(const void *, unsigned int);
    long unsigned int (*store_tr)();
    void (*load_tls)(struct thread_struct *, unsigned int);
    void (*load_gs_index)(unsigned int);
    void (*write_ldt_entry)(struct desc_struct *, int, const void *);
    void (*write_gdt_entry)(struct desc_struct *, int, const void *, int);
    void (*write_idt_entry)(gate_desc *, int, const gate_desc *);
    void (*alloc_ldt)(struct desc_struct *, unsigned int);
    void (*free_ldt)(struct desc_struct *, unsigned int);
    void (*load_sp0)(long unsigned int);
    void (*invalidate_io_bitmap)();
    void (*update_io_bitmap)();
    void (*wbinvd)();
    void (*cpuid)(unsigned int *, unsigned int *, unsigned int *, unsigned int *);
    u64 (*read_msr)(unsigned int);
    void (*write_msr)(unsigned int, unsigned int, unsigned int);
    u64 (*read_msr_safe)(unsigned int, int *);
    int (*write_msr_safe)(unsigned int, unsigned int, unsigned int);
    u64 (*read_pmc)(int);
    void (*usergs_sysret64)();
    void (*iret)();
    void (*swapgs)();
    void (*start_context_switch)(struct task_struct *);
    void (*end_context_switch)(struct task_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct pv_cpu_ops {
    void (*io_delay)();
    long unsigned int (*get_debugreg)(int);
    void (*set_debugreg)(int, long unsigned int);
    long unsigned int (*read_cr0)();
    void (*write_cr0)(long unsigned int);
    void (*write_cr4)(long unsigned int);
    void (*load_tr_desc)();
    void (*load_gdt)(const struct desc_ptr *);
    void (*load_idt)(const struct desc_ptr *);
    void (*set_ldt)(const void *, unsigned int);
    long unsigned int (*store_tr)();
    void (*load_tls)(struct thread_struct *, unsigned int);
    void (*load_gs_index)(unsigned int);
    void (*write_ldt_entry)(struct desc_struct *, int, const void *);
    void (*write_gdt_entry)(struct desc_struct *, int, const void *, int);
    void (*write_idt_entry)(gate_desc *, int, const gate_desc *);
    void (*alloc_ldt)(struct desc_struct *, unsigned int);
    void (*free_ldt)(struct desc_struct *, unsigned int);
    void (*load_sp0)(long unsigned int);
    void (*invalidate_io_bitmap)();
    void (*update_io_bitmap)();
    void (*wbinvd)();
    void (*cpuid)(unsigned int *, unsigned int *, unsigned int *, unsigned int *);
    u64 (*read_msr)(unsigned int);
    void (*write_msr)(unsigned int, unsigned int, unsigned int);
    u64 (*read_msr_safe)(unsigned int, int *);
    int (*write_msr_safe)(unsigned int, unsigned int, unsigned int);
    u64 (*read_pmc)(int);
    void (*start_context_switch)(struct task_struct *);
    void (*end_context_switch)(struct task_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct pv_cpu_ops {
    void (*io_delay)();
    long unsigned int (*get_debugreg)(int);
    void (*set_debugreg)(int, long unsigned int);
    long unsigned int (*read_cr0)();
    void (*write_cr0)(long unsigned int);
    void (*write_cr4)(long unsigned int);
    void (*load_tr_desc)();
    void (*load_gdt)(const struct desc_ptr *);
    void (*load_idt)(const struct desc_ptr *);
    void (*set_ldt)(const void *, unsigned int);
    long unsigned int (*store_tr)();
    void (*load_tls)(struct thread_struct *, unsigned int);
    void (*load_gs_index)(unsigned int);
    void (*write_ldt_entry)(struct desc_struct *, int, const void *);
    void (*write_gdt_entry)(struct desc_struct *, int, const void *, int);
    void (*write_idt_entry)(gate_desc *, int, const gate_desc *);
    void (*alloc_ldt)(struct desc_struct *, unsigned int);
    void (*free_ldt)(struct desc_struct *, unsigned int);
    void (*load_sp0)(long unsigned int);
    void (*invalidate_io_bitmap)();
    void (*update_io_bitmap)();
    void (*wbinvd)();
    void (*cpuid)(unsigned int *, unsigned int *, unsigned int *, unsigned int *);
    u64 (*read_msr)(unsigned int);
    void (*write_msr)(unsigned int, unsigned int, unsigned int);
    u64 (*read_msr_safe)(unsigned int, int *);
    int (*write_msr_safe)(unsigned int, unsigned int, unsigned int);
    u64 (*read_pmc)(int);
    void (*start_context_switch)(struct task_struct *);
    void (*end_context_switch)(struct task_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct pv_cpu_ops {
    void (*io_delay)();
    long unsigned int (*get_debugreg)(int);
    void (*set_debugreg)(int, long unsigned int);
    long unsigned int (*read_cr0)();
    void (*write_cr0)(long unsigned int);
    void (*write_cr4)(long unsigned int);
    void (*load_tr_desc)();
    void (*load_gdt)(const struct desc_ptr *);
    void (*load_idt)(const struct desc_ptr *);
    void (*set_ldt)(const void *, unsigned int);
    long unsigned int (*store_tr)();
    void (*load_tls)(struct thread_struct *, unsigned int);
    void (*load_gs_index)(unsigned int);
    void (*write_ldt_entry)(struct desc_struct *, int, const void *);
    void (*write_gdt_entry)(struct desc_struct *, int, const void *, int);
    void (*write_idt_entry)(gate_desc *, int, const gate_desc *);
    void (*alloc_ldt)(struct desc_struct *, unsigned int);
    void (*free_ldt)(struct desc_struct *, unsigned int);
    void (*load_sp0)(long unsigned int);
    void (*invalidate_io_bitmap)();
    void (*update_io_bitmap)();
    void (*wbinvd)();
    void (*cpuid)(unsigned int *, unsigned int *, unsigned int *, unsigned int *);
    u64 (*read_msr)(unsigned int);
    void (*write_msr)(unsigned int, unsigned int, unsigned int);
    u64 (*read_msr_safe)(unsigned int, int *);
    int (*write_msr_safe)(unsigned int, unsigned int, unsigned int);
    u64 (*read_pmc)(int);
    void (*start_context_switch)(struct task_struct *);
    void (*end_context_switch)(struct task_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct pv_cpu_ops {
    void (*io_delay)();
    long unsigned int (*get_debugreg)(int);
    void (*set_debugreg)(int, long unsigned int);
    long unsigned int (*read_cr0)();
    void (*write_cr0)(long unsigned int);
    void (*write_cr4)(long unsigned int);
    void (*load_tr_desc)();
    void (*load_gdt)(const struct desc_ptr *);
    void (*load_idt)(const struct desc_ptr *);
    void (*set_ldt)(const void *, unsigned int);
    long unsigned int (*store_tr)();
    void (*load_tls)(struct thread_struct *, unsigned int);
    void (*load_gs_index)(unsigned int);
    void (*write_ldt_entry)(struct desc_struct *, int, const void *);
    void (*write_gdt_entry)(struct desc_struct *, int, const void *, int);
    void (*write_idt_entry)(gate_desc *, int, const gate_desc *);
    void (*alloc_ldt)(struct desc_struct *, unsigned int);
    void (*free_ldt)(struct desc_struct *, unsigned int);
    void (*load_sp0)(long unsigned int);
    void (*invalidate_io_bitmap)();
    void (*update_io_bitmap)();
    void (*wbinvd)();
    void (*cpuid)(unsigned int *, unsigned int *, unsigned int *, unsigned int *);
    u64 (*read_msr)(unsigned int);
    void (*write_msr)(unsigned int, unsigned int, unsigned int);
    u64 (*read_msr_safe)(unsigned int, int *);
    int (*write_msr_safe)(unsigned int, unsigned int, unsigned int);
    u64 (*read_pmc)(int);
    void (*start_context_switch)(struct task_struct *);
    void (*end_context_switch)(struct task_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct pv_cpu_ops {
    void (*io_delay)();
    long unsigned int (*get_debugreg)(int);
    void (*set_debugreg)(int, long unsigned int);
    long unsigned int (*read_cr0)();
    void (*write_cr0)(long unsigned int);
    void (*write_cr4)(long unsigned int);
    void (*load_tr_desc)();
    void (*load_gdt)(const struct desc_ptr *);
    void (*load_idt)(const struct desc_ptr *);
    void (*set_ldt)(const void *, unsigned int);
    long unsigned int (*store_tr)();
    void (*load_tls)(struct thread_struct *, unsigned int);
    void (*load_gs_index)(unsigned int);
    void (*write_ldt_entry)(struct desc_struct *, int, const void *);
    void (*write_gdt_entry)(struct desc_struct *, int, const void *, int);
    void (*write_idt_entry)(gate_desc *, int, const gate_desc *);
    void (*alloc_ldt)(struct desc_struct *, unsigned int);
    void (*free_ldt)(struct desc_struct *, unsigned int);
    void (*load_sp0)(long unsigned int);
    void (*invalidate_io_bitmap)();
    void (*update_io_bitmap)();
    void (*wbinvd)();
    void (*cpuid)(unsigned int *, unsigned int *, unsigned int *, unsigned int *);
    u64 (*read_msr)(unsigned int);
    void (*write_msr)(unsigned int, unsigned int, unsigned int);
    u64 (*read_msr_safe)(unsigned int, int *);
    int (*write_msr_safe)(unsigned int, unsigned int, unsigned int);
    u64 (*read_pmc)(int);
    void (*start_context_switch)(struct task_struct *);
    void (*end_context_switch)(struct task_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct pv_cpu_ops {
    void (*io_delay)();
    long unsigned int (*get_debugreg)(int);
    void (*set_debugreg)(int, long unsigned int);
    long unsigned int (*read_cr0)();
    void (*write_cr0)(long unsigned int);
    void (*write_cr4)(long unsigned int);
    void (*load_tr_desc)();
    void (*load_gdt)(const struct desc_ptr *);
    void (*load_idt)(const struct desc_ptr *);
    void (*set_ldt)(const void *, unsigned int);
    long unsigned int (*store_tr)();
    void (*load_tls)(struct thread_struct *, unsigned int);
    void (*load_gs_index)(unsigned int);
    void (*write_ldt_entry)(struct desc_struct *, int, const void *);
    void (*write_gdt_entry)(struct desc_struct *, int, const void *, int);
    void (*write_idt_entry)(gate_desc *, int, const gate_desc *);
    void (*alloc_ldt)(struct desc_struct *, unsigned int);
    void (*free_ldt)(struct desc_struct *, unsigned int);
    void (*load_sp0)(long unsigned int);
    void (*invalidate_io_bitmap)();
    void (*update_io_bitmap)();
    void (*wbinvd)();
    void (*cpuid)(unsigned int *, unsigned int *, unsigned int *, unsigned int *);
    u64 (*read_msr)(unsigned int);
    void (*write_msr)(unsigned int, unsigned int, unsigned int);
    u64 (*read_msr_safe)(unsigned int, int *);
    int (*write_msr_safe)(unsigned int, unsigned int, unsigned int);
    u64 (*read_pmc)(int);
    void (*start_context_switch)(struct task_struct *);
    void (*end_context_switch)(struct task_struct *);
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct pv_cpu_ops {
    void (*io_delay)();
    long unsigned int (*get_debugreg)(int);
    void (*set_debugreg)(int, long unsigned int);
    long unsigned int (*read_cr0)();
    void (*write_cr0)(long unsigned int);
    void (*write_cr4)(long unsigned int);
    void (*load_tr_desc)();
    void (*load_gdt)(const struct desc_ptr *);
    void (*load_idt)(const struct desc_ptr *);
    void (*set_ldt)(const void *, unsigned int);
    long unsigned int (*store_tr)();
    void (*load_tls)(struct thread_struct *, unsigned int);
    void (*load_gs_index)(unsigned int);
    void (*write_ldt_entry)(struct desc_struct *, int, const void *);
    void (*write_gdt_entry)(struct desc_struct *, int, const void *, int);
    void (*write_idt_entry)(gate_desc *, int, const gate_desc *);
    void (*alloc_ldt)(struct desc_struct *, unsigned int);
    void (*free_ldt)(struct desc_struct *, unsigned int);
    void (*load_sp0)(long unsigned int);
    void (*set_iopl_mask)(unsigned int);
    void (*wbinvd)();
    void (*cpuid)(unsigned int *, unsigned int *, unsigned int *, unsigned int *);
    u64 (*read_msr)(unsigned int);
    void (*write_msr)(unsigned int, unsigned int, unsigned int);
    u64 (*read_msr_safe)(unsigned int, int *);
    int (*write_msr_safe)(unsigned int, unsigned int, unsigned int);
    u64 (*read_pmc)(int);
    void (*usergs_sysret64)();
    void (*iret)();
    void (*swapgs)();
    void (*start_context_switch)(struct task_struct *);
    void (*end_context_switch)(struct task_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct pv_cpu_ops {
    void (*io_delay)();
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct pv_cpu_ops {
    void (*io_delay)();
    long unsigned int (*get_debugreg)(int);
    void (*set_debugreg)(int, long unsigned int);
    long unsigned int (*read_cr0)();
    void (*write_cr0)(long unsigned int);
    void (*write_cr4)(long unsigned int);
    void (*load_tr_desc)();
    void (*load_gdt)(const struct desc_ptr *);
    void (*load_idt)(const struct desc_ptr *);
    void (*set_ldt)(const void *, unsigned int);
    long unsigned int (*store_tr)();
    void (*load_tls)(struct thread_struct *, unsigned int);
    void (*load_gs_index)(unsigned int);
    void (*write_ldt_entry)(struct desc_struct *, int, const void *);
    void (*write_gdt_entry)(struct desc_struct *, int, const void *, int);
    void (*write_idt_entry)(gate_desc *, int, const gate_desc *);
    void (*alloc_ldt)(struct desc_struct *, unsigned int);
    void (*free_ldt)(struct desc_struct *, unsigned int);
    void (*load_sp0)(long unsigned int);
    void (*set_iopl_mask)(unsigned int);
    void (*wbinvd)();
    void (*cpuid)(unsigned int *, unsigned int *, unsigned int *, unsigned int *);
    u64 (*read_msr)(unsigned int);
    void (*write_msr)(unsigned int, unsigned int, unsigned int);
    u64 (*read_msr_safe)(unsigned int, int *);
    int (*write_msr_safe)(unsigned int, unsigned int, unsigned int);
    u64 (*read_pmc)(int);
    void (*usergs_sysret64)();
    void (*iret)();
    void (*swapgs)();
    void (*start_context_switch)(struct task_struct *);
    void (*end_context_switch)(struct task_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct pv_cpu_ops {
    void (*io_delay)();
    long unsigned int (*get_debugreg)(int);
    void (*set_debugreg)(int, long unsigned int);
    long unsigned int (*read_cr0)();
    void (*write_cr0)(long unsigned int);
    void (*write_cr4)(long unsigned int);
    void (*load_tr_desc)();
    void (*load_gdt)(const struct desc_ptr *);
    void (*load_idt)(const struct desc_ptr *);
    void (*set_ldt)(const void *, unsigned int);
    long unsigned int (*store_tr)();
    void (*load_tls)(struct thread_struct *, unsigned int);
    void (*load_gs_index)(unsigned int);
    void (*write_ldt_entry)(struct desc_struct *, int, const void *);
    void (*write_gdt_entry)(struct desc_struct *, int, const void *, int);
    void (*write_idt_entry)(gate_desc *, int, const gate_desc *);
    void (*alloc_ldt)(struct desc_struct *, unsigned int);
    void (*free_ldt)(struct desc_struct *, unsigned int);
    void (*load_sp0)(long unsigned int);
    void (*set_iopl_mask)(unsigned int);
    void (*wbinvd)();
    void (*cpuid)(unsigned int *, unsigned int *, unsigned int *, unsigned int *);
    u64 (*read_msr)(unsigned int);
    void (*write_msr)(unsigned int, unsigned int, unsigned int);
    u64 (*read_msr_safe)(unsigned int, int *);
    int (*write_msr_safe)(unsigned int, unsigned int, unsigned int);
    u64 (*read_pmc)(int);
    void (*usergs_sysret64)();
    void (*iret)();
    void (*swapgs)();
    void (*start_context_switch)(struct task_struct *);
    void (*end_context_switch)(struct task_struct *);
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 (*read_msr_safe)(unsigned int, int *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*write_msr_safe)(unsigned int, unsigned int, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*usergs_sysret32)()</code>
</li>
<li>
<b>Field type changed. </b>
<code>u64 (*read_msr)(unsigned int, int *)</code> ➡️ <code>u64 (*read_msr)(unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*write_msr)(unsigned int, unsigned int, unsigned int)</code> ➡️ <code>void (*write_msr)(unsigned int, unsigned int, unsigned int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>void (*clts)()</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int (*read_cr4_safe)()</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>long unsigned int (*read_cr4)()</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*store_idt)(struct desc_ptr *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*load_sp0)(struct tss_struct *, struct thread_struct *)</code> ➡️ <code>void (*load_sp0)(long unsigned int)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>long unsigned int (*read_cr8)()</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*write_cr8)(long unsigned int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*invalidate_io_bitmap)()</code>
</li>
<li>
<b>Field added. </b>
<code>void (*update_io_bitmap)()</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*set_iopl_mask)(unsigned int)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>void (*usergs_sysret64)()</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*iret)()</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*swapgs)()</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
<b>Arch</b>
<ul>
</ul>
<b>Flavor</b>
<ul>
<li>
No changes between <code>generic</code> and <code>aws</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>generic</code> and <code>azure</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>long unsigned int (*get_debugreg)(int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*set_debugreg)(int, long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int (*read_cr0)()</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*write_cr0)(long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*write_cr4)(long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*load_tr_desc)()</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*load_gdt)(const struct desc_ptr *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*load_idt)(const struct desc_ptr *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*set_ldt)(const void *, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int (*store_tr)()</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*load_tls)(struct thread_struct *, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*load_gs_index)(unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*write_ldt_entry)(struct desc_struct *, int, const void *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*write_gdt_entry)(struct desc_struct *, int, const void *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*write_idt_entry)(gate_desc *, int, const gate_desc *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*alloc_ldt)(struct desc_struct *, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*free_ldt)(struct desc_struct *, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*load_sp0)(long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*set_iopl_mask)(unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*wbinvd)()</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*cpuid)(unsigned int *, unsigned int *, unsigned int *, unsigned int *)</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 (*read_msr)(unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*write_msr)(unsigned int, unsigned int, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 (*read_msr_safe)(unsigned int, int *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*write_msr_safe)(unsigned int, unsigned int, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 (*read_pmc)(int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*usergs_sysret64)()</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*iret)()</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*swapgs)()</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*start_context_switch)(struct task_struct *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*end_context_switch)(struct task_struct *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
