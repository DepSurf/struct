# Struct: <code>vcpu_guest_context</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct vcpu_guest_context {
    struct (anon) fpu_ctxt;
    long unsigned int flags;
    struct cpu_user_regs user_regs;
    struct trap_info trap_ctxt[256];
    long unsigned int ldt_base;
    long unsigned int ldt_ents;
    long unsigned int gdt_frames[16];
    long unsigned int gdt_ents;
    long unsigned int kernel_ss;
    long unsigned int kernel_sp;
    long unsigned int ctrlreg[8];
    long unsigned int debugreg[8];
    long unsigned int event_callback_eip;
    long unsigned int failsafe_callback_eip;
    long unsigned int syscall_callback_eip;
    long unsigned int vm_assist;
    uint64_t fs_base;
    uint64_t gs_base_kernel;
    uint64_t gs_base_user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct vcpu_guest_context {
    struct (anon) fpu_ctxt;
    long unsigned int flags;
    struct cpu_user_regs user_regs;
    struct trap_info trap_ctxt[256];
    long unsigned int ldt_base;
    long unsigned int ldt_ents;
    long unsigned int gdt_frames[16];
    long unsigned int gdt_ents;
    long unsigned int kernel_ss;
    long unsigned int kernel_sp;
    long unsigned int ctrlreg[8];
    long unsigned int debugreg[8];
    long unsigned int event_callback_eip;
    long unsigned int failsafe_callback_eip;
    long unsigned int syscall_callback_eip;
    long unsigned int vm_assist;
    uint64_t fs_base;
    uint64_t gs_base_kernel;
    uint64_t gs_base_user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct vcpu_guest_context {
    struct (anon) fpu_ctxt;
    long unsigned int flags;
    struct cpu_user_regs user_regs;
    struct trap_info trap_ctxt[256];
    long unsigned int ldt_base;
    long unsigned int ldt_ents;
    long unsigned int gdt_frames[16];
    long unsigned int gdt_ents;
    long unsigned int kernel_ss;
    long unsigned int kernel_sp;
    long unsigned int ctrlreg[8];
    long unsigned int debugreg[8];
    long unsigned int event_callback_eip;
    long unsigned int failsafe_callback_eip;
    long unsigned int syscall_callback_eip;
    long unsigned int vm_assist;
    uint64_t fs_base;
    uint64_t gs_base_kernel;
    uint64_t gs_base_user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct vcpu_guest_context {
    struct (anon) fpu_ctxt;
    long unsigned int flags;
    struct cpu_user_regs user_regs;
    struct trap_info trap_ctxt[256];
    long unsigned int ldt_base;
    long unsigned int ldt_ents;
    long unsigned int gdt_frames[16];
    long unsigned int gdt_ents;
    long unsigned int kernel_ss;
    long unsigned int kernel_sp;
    long unsigned int ctrlreg[8];
    long unsigned int debugreg[8];
    long unsigned int event_callback_eip;
    long unsigned int failsafe_callback_eip;
    long unsigned int syscall_callback_eip;
    long unsigned int vm_assist;
    uint64_t fs_base;
    uint64_t gs_base_kernel;
    uint64_t gs_base_user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct vcpu_guest_context {
    struct (anon) fpu_ctxt;
    long unsigned int flags;
    struct cpu_user_regs user_regs;
    struct trap_info trap_ctxt[256];
    long unsigned int ldt_base;
    long unsigned int ldt_ents;
    long unsigned int gdt_frames[16];
    long unsigned int gdt_ents;
    long unsigned int kernel_ss;
    long unsigned int kernel_sp;
    long unsigned int ctrlreg[8];
    long unsigned int debugreg[8];
    long unsigned int event_callback_eip;
    long unsigned int failsafe_callback_eip;
    long unsigned int syscall_callback_eip;
    long unsigned int vm_assist;
    uint64_t fs_base;
    uint64_t gs_base_kernel;
    uint64_t gs_base_user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct vcpu_guest_context {
    struct (anon) fpu_ctxt;
    long unsigned int flags;
    struct cpu_user_regs user_regs;
    struct trap_info trap_ctxt[256];
    long unsigned int ldt_base;
    long unsigned int ldt_ents;
    long unsigned int gdt_frames[16];
    long unsigned int gdt_ents;
    long unsigned int kernel_ss;
    long unsigned int kernel_sp;
    long unsigned int ctrlreg[8];
    long unsigned int debugreg[8];
    long unsigned int event_callback_eip;
    long unsigned int failsafe_callback_eip;
    long unsigned int syscall_callback_eip;
    long unsigned int vm_assist;
    uint64_t fs_base;
    uint64_t gs_base_kernel;
    uint64_t gs_base_user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct vcpu_guest_context {
    struct (anon) fpu_ctxt;
    long unsigned int flags;
    struct cpu_user_regs user_regs;
    struct trap_info trap_ctxt[256];
    long unsigned int ldt_base;
    long unsigned int ldt_ents;
    long unsigned int gdt_frames[16];
    long unsigned int gdt_ents;
    long unsigned int kernel_ss;
    long unsigned int kernel_sp;
    long unsigned int ctrlreg[8];
    long unsigned int debugreg[8];
    long unsigned int event_callback_eip;
    long unsigned int failsafe_callback_eip;
    long unsigned int syscall_callback_eip;
    long unsigned int vm_assist;
    uint64_t fs_base;
    uint64_t gs_base_kernel;
    uint64_t gs_base_user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct vcpu_guest_context {
    struct (anon) fpu_ctxt;
    long unsigned int flags;
    struct cpu_user_regs user_regs;
    struct trap_info trap_ctxt[256];
    long unsigned int ldt_base;
    long unsigned int ldt_ents;
    long unsigned int gdt_frames[16];
    long unsigned int gdt_ents;
    long unsigned int kernel_ss;
    long unsigned int kernel_sp;
    long unsigned int ctrlreg[8];
    long unsigned int debugreg[8];
    long unsigned int event_callback_eip;
    long unsigned int failsafe_callback_eip;
    long unsigned int syscall_callback_eip;
    long unsigned int vm_assist;
    uint64_t fs_base;
    uint64_t gs_base_kernel;
    uint64_t gs_base_user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct vcpu_guest_context {
    struct (anon) fpu_ctxt;
    long unsigned int flags;
    struct cpu_user_regs user_regs;
    struct trap_info trap_ctxt[256];
    long unsigned int ldt_base;
    long unsigned int ldt_ents;
    long unsigned int gdt_frames[16];
    long unsigned int gdt_ents;
    long unsigned int kernel_ss;
    long unsigned int kernel_sp;
    long unsigned int ctrlreg[8];
    long unsigned int debugreg[8];
    long unsigned int event_callback_eip;
    long unsigned int failsafe_callback_eip;
    long unsigned int syscall_callback_eip;
    long unsigned int vm_assist;
    uint64_t fs_base;
    uint64_t gs_base_kernel;
    uint64_t gs_base_user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct vcpu_guest_context {
    struct (anon) fpu_ctxt;
    long unsigned int flags;
    struct cpu_user_regs user_regs;
    struct trap_info trap_ctxt[256];
    long unsigned int ldt_base;
    long unsigned int ldt_ents;
    long unsigned int gdt_frames[16];
    long unsigned int gdt_ents;
    long unsigned int kernel_ss;
    long unsigned int kernel_sp;
    long unsigned int ctrlreg[8];
    long unsigned int debugreg[8];
    long unsigned int event_callback_eip;
    long unsigned int failsafe_callback_eip;
    long unsigned int syscall_callback_eip;
    long unsigned int vm_assist;
    uint64_t fs_base;
    uint64_t gs_base_kernel;
    uint64_t gs_base_user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct vcpu_guest_context {
    struct (anon) fpu_ctxt;
    long unsigned int flags;
    struct cpu_user_regs user_regs;
    struct trap_info trap_ctxt[256];
    long unsigned int ldt_base;
    long unsigned int ldt_ents;
    long unsigned int gdt_frames[16];
    long unsigned int gdt_ents;
    long unsigned int kernel_ss;
    long unsigned int kernel_sp;
    long unsigned int ctrlreg[8];
    long unsigned int debugreg[8];
    long unsigned int event_callback_eip;
    long unsigned int failsafe_callback_eip;
    long unsigned int syscall_callback_eip;
    long unsigned int vm_assist;
    uint64_t fs_base;
    uint64_t gs_base_kernel;
    uint64_t gs_base_user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct vcpu_guest_context {
    struct (anon) fpu_ctxt;
    long unsigned int flags;
    struct cpu_user_regs user_regs;
    struct trap_info trap_ctxt[256];
    long unsigned int ldt_base;
    long unsigned int ldt_ents;
    long unsigned int gdt_frames[16];
    long unsigned int gdt_ents;
    long unsigned int kernel_ss;
    long unsigned int kernel_sp;
    long unsigned int ctrlreg[8];
    long unsigned int debugreg[8];
    long unsigned int event_callback_eip;
    long unsigned int failsafe_callback_eip;
    long unsigned int syscall_callback_eip;
    long unsigned int vm_assist;
    uint64_t fs_base;
    uint64_t gs_base_kernel;
    uint64_t gs_base_user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct vcpu_guest_context {
    struct (anon) fpu_ctxt;
    long unsigned int flags;
    struct cpu_user_regs user_regs;
    struct trap_info trap_ctxt[256];
    long unsigned int ldt_base;
    long unsigned int ldt_ents;
    long unsigned int gdt_frames[16];
    long unsigned int gdt_ents;
    long unsigned int kernel_ss;
    long unsigned int kernel_sp;
    long unsigned int ctrlreg[8];
    long unsigned int debugreg[8];
    long unsigned int event_callback_eip;
    long unsigned int failsafe_callback_eip;
    long unsigned int syscall_callback_eip;
    long unsigned int vm_assist;
    uint64_t fs_base;
    uint64_t gs_base_kernel;
    uint64_t gs_base_user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct vcpu_guest_context {
    struct (anon) fpu_ctxt;
    long unsigned int flags;
    struct cpu_user_regs user_regs;
    struct trap_info trap_ctxt[256];
    long unsigned int ldt_base;
    long unsigned int ldt_ents;
    long unsigned int gdt_frames[16];
    long unsigned int gdt_ents;
    long unsigned int kernel_ss;
    long unsigned int kernel_sp;
    long unsigned int ctrlreg[8];
    long unsigned int debugreg[8];
    long unsigned int event_callback_eip;
    long unsigned int failsafe_callback_eip;
    long unsigned int syscall_callback_eip;
    long unsigned int vm_assist;
    uint64_t fs_base;
    uint64_t gs_base_kernel;
    uint64_t gs_base_user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct vcpu_guest_context {
    struct (anon) fpu_ctxt;
    long unsigned int flags;
    struct cpu_user_regs user_regs;
    struct trap_info trap_ctxt[256];
    long unsigned int ldt_base;
    long unsigned int ldt_ents;
    long unsigned int gdt_frames[16];
    long unsigned int gdt_ents;
    long unsigned int kernel_ss;
    long unsigned int kernel_sp;
    long unsigned int ctrlreg[8];
    long unsigned int debugreg[8];
    long unsigned int event_callback_eip;
    long unsigned int failsafe_callback_eip;
    long unsigned int syscall_callback_eip;
    long unsigned int vm_assist;
    uint64_t fs_base;
    uint64_t gs_base_kernel;
    uint64_t gs_base_user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct vcpu_guest_context {
    struct (anon) fpu_ctxt;
    long unsigned int flags;
    struct cpu_user_regs user_regs;
    struct trap_info trap_ctxt[256];
    long unsigned int ldt_base;
    long unsigned int ldt_ents;
    long unsigned int gdt_frames[16];
    long unsigned int gdt_ents;
    long unsigned int kernel_ss;
    long unsigned int kernel_sp;
    long unsigned int ctrlreg[8];
    long unsigned int debugreg[8];
    long unsigned int event_callback_eip;
    long unsigned int failsafe_callback_eip;
    long unsigned int syscall_callback_eip;
    long unsigned int vm_assist;
    uint64_t fs_base;
    uint64_t gs_base_kernel;
    uint64_t gs_base_user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct vcpu_guest_context {
    struct (anon) fpu_ctxt;
    long unsigned int flags;
    struct cpu_user_regs user_regs;
    struct trap_info trap_ctxt[256];
    long unsigned int ldt_base;
    long unsigned int ldt_ents;
    long unsigned int gdt_frames[16];
    long unsigned int gdt_ents;
    long unsigned int kernel_ss;
    long unsigned int kernel_sp;
    long unsigned int ctrlreg[8];
    long unsigned int debugreg[8];
    long unsigned int event_callback_eip;
    long unsigned int failsafe_callback_eip;
    long unsigned int syscall_callback_eip;
    long unsigned int vm_assist;
    uint64_t fs_base;
    uint64_t gs_base_kernel;
    uint64_t gs_base_user;
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
struct vcpu_guest_context {
    struct (anon) fpu_ctxt;
    long unsigned int flags;
    struct cpu_user_regs user_regs;
    struct trap_info trap_ctxt[256];
    long unsigned int ldt_base;
    long unsigned int ldt_ents;
    long unsigned int gdt_frames[16];
    long unsigned int gdt_ents;
    long unsigned int kernel_ss;
    long unsigned int kernel_sp;
    long unsigned int ctrlreg[8];
    long unsigned int debugreg[8];
    long unsigned int event_callback_eip;
    long unsigned int failsafe_callback_eip;
    long unsigned int syscall_callback_eip;
    long unsigned int vm_assist;
    uint64_t fs_base;
    uint64_t gs_base_kernel;
    uint64_t gs_base_user;
};
```
</details>
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct vcpu_guest_context {
    struct (anon) fpu_ctxt;
    long unsigned int flags;
    struct cpu_user_regs user_regs;
    struct trap_info trap_ctxt[256];
    long unsigned int ldt_base;
    long unsigned int ldt_ents;
    long unsigned int gdt_frames[16];
    long unsigned int gdt_ents;
    long unsigned int kernel_ss;
    long unsigned int kernel_sp;
    long unsigned int ctrlreg[8];
    long unsigned int debugreg[8];
    long unsigned int event_callback_eip;
    long unsigned int failsafe_callback_eip;
    long unsigned int syscall_callback_eip;
    long unsigned int vm_assist;
    uint64_t fs_base;
    uint64_t gs_base_kernel;
    uint64_t gs_base_user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct vcpu_guest_context {
    struct (anon) fpu_ctxt;
    long unsigned int flags;
    struct cpu_user_regs user_regs;
    struct trap_info trap_ctxt[256];
    long unsigned int ldt_base;
    long unsigned int ldt_ents;
    long unsigned int gdt_frames[16];
    long unsigned int gdt_ents;
    long unsigned int kernel_ss;
    long unsigned int kernel_sp;
    long unsigned int ctrlreg[8];
    long unsigned int debugreg[8];
    long unsigned int event_callback_eip;
    long unsigned int failsafe_callback_eip;
    long unsigned int syscall_callback_eip;
    long unsigned int vm_assist;
    uint64_t fs_base;
    uint64_t gs_base_kernel;
    uint64_t gs_base_user;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.4</code> and <code>4.8</code> ✅
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
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
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
