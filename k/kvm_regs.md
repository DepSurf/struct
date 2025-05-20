# Struct: <code>kvm_regs</code>

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
struct kvm_regs {
    __u64 rax;
    __u64 rbx;
    __u64 rcx;
    __u64 rdx;
    __u64 rsi;
    __u64 rdi;
    __u64 rsp;
    __u64 rbp;
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 rip;
    __u64 rflags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kvm_regs {
    __u64 rax;
    __u64 rbx;
    __u64 rcx;
    __u64 rdx;
    __u64 rsi;
    __u64 rdi;
    __u64 rsp;
    __u64 rbp;
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 rip;
    __u64 rflags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kvm_regs {
    __u64 rax;
    __u64 rbx;
    __u64 rcx;
    __u64 rdx;
    __u64 rsi;
    __u64 rdi;
    __u64 rsp;
    __u64 rbp;
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 rip;
    __u64 rflags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kvm_regs {
    __u64 rax;
    __u64 rbx;
    __u64 rcx;
    __u64 rdx;
    __u64 rsi;
    __u64 rdi;
    __u64 rsp;
    __u64 rbp;
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 rip;
    __u64 rflags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kvm_regs {
    __u64 rax;
    __u64 rbx;
    __u64 rcx;
    __u64 rdx;
    __u64 rsi;
    __u64 rdi;
    __u64 rsp;
    __u64 rbp;
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 rip;
    __u64 rflags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kvm_regs {
    __u64 rax;
    __u64 rbx;
    __u64 rcx;
    __u64 rdx;
    __u64 rsi;
    __u64 rdi;
    __u64 rsp;
    __u64 rbp;
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 rip;
    __u64 rflags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kvm_regs {
    __u64 rax;
    __u64 rbx;
    __u64 rcx;
    __u64 rdx;
    __u64 rsi;
    __u64 rdi;
    __u64 rsp;
    __u64 rbp;
    __u64 r8;
    __u64 r9;
    __u64 r10;
    __u64 r11;
    __u64 r12;
    __u64 r13;
    __u64 r14;
    __u64 r15;
    __u64 rip;
    __u64 rflags;
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
struct kvm_regs {
    struct user_pt_regs regs;
    __u64 sp_el1;
    __u64 elr_el1;
    __u64 spsr[5];
    struct user_fpsimd_state fp_regs;
};
```
</details>
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
