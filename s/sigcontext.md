# Struct: <code>sigcontext</code>

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
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct sigcontext {
    __u64 fault_address;
    __u64 regs[31];
    __u64 sp;
    __u64 pc;
    __u64 pstate;
    __u8 __reserved[4096];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct sigcontext {
    long unsigned int trap_no;
    long unsigned int error_code;
    long unsigned int oldmask;
    long unsigned int arm_r0;
    long unsigned int arm_r1;
    long unsigned int arm_r2;
    long unsigned int arm_r3;
    long unsigned int arm_r4;
    long unsigned int arm_r5;
    long unsigned int arm_r6;
    long unsigned int arm_r7;
    long unsigned int arm_r8;
    long unsigned int arm_r9;
    long unsigned int arm_r10;
    long unsigned int arm_fp;
    long unsigned int arm_ip;
    long unsigned int arm_sp;
    long unsigned int arm_lr;
    long unsigned int arm_pc;
    long unsigned int arm_cpsr;
    long unsigned int fault_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct sigcontext {
    long unsigned int _unused[4];
    int signal;
    int _pad0;
    long unsigned int handler;
    long unsigned int oldmask;
    struct user_pt_regs *regs;
    elf_gregset_t gp_regs;
    elf_fpregset_t fp_regs;
    elf_vrreg_t *v_regs;
    long int vmx_reserve[101];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct sigcontext {
    struct user_regs_struct sc_regs;
    union __riscv_fp_state sc_fpregs;
};
```
</details>
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
