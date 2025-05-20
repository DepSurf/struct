# Struct: <code>cpu_user_regs</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct cpu_user_regs {
    uint64_t r15;
    uint64_t r14;
    uint64_t r13;
    uint64_t r12;
    uint64_t rbp;
    uint64_t ebp;
    uint32_t _ebp;
    uint64_t rbx;
    uint64_t ebx;
    uint32_t _ebx;
    uint64_t r11;
    uint64_t r10;
    uint64_t r9;
    uint64_t r8;
    uint64_t rax;
    uint64_t eax;
    uint32_t _eax;
    uint64_t rcx;
    uint64_t ecx;
    uint32_t _ecx;
    uint64_t rdx;
    uint64_t edx;
    uint32_t _edx;
    uint64_t rsi;
    uint64_t esi;
    uint32_t _esi;
    uint64_t rdi;
    uint64_t edi;
    uint32_t _edi;
    uint32_t error_code;
    uint32_t entry_vector;
    uint64_t rip;
    uint64_t eip;
    uint32_t _eip;
    uint16_t cs;
    uint16_t _pad0[1];
    uint8_t saved_upcall_mask;
    uint8_t _pad1[3];
    uint64_t rflags;
    uint64_t eflags;
    uint32_t _eflags;
    uint64_t rsp;
    uint64_t esp;
    uint32_t _esp;
    uint16_t ss;
    uint16_t _pad2[3];
    uint16_t es;
    uint16_t _pad3[3];
    uint16_t ds;
    uint16_t _pad4[3];
    uint16_t fs;
    uint16_t _pad5[3];
    uint16_t gs;
    uint16_t _pad6[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct cpu_user_regs {
    uint64_t r15;
    uint64_t r14;
    uint64_t r13;
    uint64_t r12;
    uint64_t rbp;
    uint64_t ebp;
    uint32_t _ebp;
    uint64_t rbx;
    uint64_t ebx;
    uint32_t _ebx;
    uint64_t r11;
    uint64_t r10;
    uint64_t r9;
    uint64_t r8;
    uint64_t rax;
    uint64_t eax;
    uint32_t _eax;
    uint64_t rcx;
    uint64_t ecx;
    uint32_t _ecx;
    uint64_t rdx;
    uint64_t edx;
    uint32_t _edx;
    uint64_t rsi;
    uint64_t esi;
    uint32_t _esi;
    uint64_t rdi;
    uint64_t edi;
    uint32_t _edi;
    uint32_t error_code;
    uint32_t entry_vector;
    uint64_t rip;
    uint64_t eip;
    uint32_t _eip;
    uint16_t cs;
    uint16_t _pad0[1];
    uint8_t saved_upcall_mask;
    uint8_t _pad1[3];
    uint64_t rflags;
    uint64_t eflags;
    uint32_t _eflags;
    uint64_t rsp;
    uint64_t esp;
    uint32_t _esp;
    uint16_t ss;
    uint16_t _pad2[3];
    uint16_t es;
    uint16_t _pad3[3];
    uint16_t ds;
    uint16_t _pad4[3];
    uint16_t fs;
    uint16_t _pad5[3];
    uint16_t gs;
    uint16_t _pad6[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct cpu_user_regs {
    uint64_t r15;
    uint64_t r14;
    uint64_t r13;
    uint64_t r12;
    uint64_t rbp;
    uint64_t ebp;
    uint32_t _ebp;
    uint64_t rbx;
    uint64_t ebx;
    uint32_t _ebx;
    uint64_t r11;
    uint64_t r10;
    uint64_t r9;
    uint64_t r8;
    uint64_t rax;
    uint64_t eax;
    uint32_t _eax;
    uint64_t rcx;
    uint64_t ecx;
    uint32_t _ecx;
    uint64_t rdx;
    uint64_t edx;
    uint32_t _edx;
    uint64_t rsi;
    uint64_t esi;
    uint32_t _esi;
    uint64_t rdi;
    uint64_t edi;
    uint32_t _edi;
    uint32_t error_code;
    uint32_t entry_vector;
    uint64_t rip;
    uint64_t eip;
    uint32_t _eip;
    uint16_t cs;
    uint16_t _pad0[1];
    uint8_t saved_upcall_mask;
    uint8_t _pad1[3];
    uint64_t rflags;
    uint64_t eflags;
    uint32_t _eflags;
    uint64_t rsp;
    uint64_t esp;
    uint32_t _esp;
    uint16_t ss;
    uint16_t _pad2[3];
    uint16_t es;
    uint16_t _pad3[3];
    uint16_t ds;
    uint16_t _pad4[3];
    uint16_t fs;
    uint16_t _pad5[3];
    uint16_t gs;
    uint16_t _pad6[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct cpu_user_regs {
    uint64_t r15;
    uint64_t r14;
    uint64_t r13;
    uint64_t r12;
    uint64_t rbp;
    uint64_t ebp;
    uint32_t _ebp;
    uint64_t rbx;
    uint64_t ebx;
    uint32_t _ebx;
    uint64_t r11;
    uint64_t r10;
    uint64_t r9;
    uint64_t r8;
    uint64_t rax;
    uint64_t eax;
    uint32_t _eax;
    uint64_t rcx;
    uint64_t ecx;
    uint32_t _ecx;
    uint64_t rdx;
    uint64_t edx;
    uint32_t _edx;
    uint64_t rsi;
    uint64_t esi;
    uint32_t _esi;
    uint64_t rdi;
    uint64_t edi;
    uint32_t _edi;
    uint32_t error_code;
    uint32_t entry_vector;
    uint64_t rip;
    uint64_t eip;
    uint32_t _eip;
    uint16_t cs;
    uint16_t _pad0[1];
    uint8_t saved_upcall_mask;
    uint8_t _pad1[3];
    uint64_t rflags;
    uint64_t eflags;
    uint32_t _eflags;
    uint64_t rsp;
    uint64_t esp;
    uint32_t _esp;
    uint16_t ss;
    uint16_t _pad2[3];
    uint16_t es;
    uint16_t _pad3[3];
    uint16_t ds;
    uint16_t _pad4[3];
    uint16_t fs;
    uint16_t _pad5[3];
    uint16_t gs;
    uint16_t _pad6[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct cpu_user_regs {
    uint64_t r15;
    uint64_t r14;
    uint64_t r13;
    uint64_t r12;
    uint64_t rbp;
    uint64_t ebp;
    uint32_t _ebp;
    uint64_t rbx;
    uint64_t ebx;
    uint32_t _ebx;
    uint64_t r11;
    uint64_t r10;
    uint64_t r9;
    uint64_t r8;
    uint64_t rax;
    uint64_t eax;
    uint32_t _eax;
    uint64_t rcx;
    uint64_t ecx;
    uint32_t _ecx;
    uint64_t rdx;
    uint64_t edx;
    uint32_t _edx;
    uint64_t rsi;
    uint64_t esi;
    uint32_t _esi;
    uint64_t rdi;
    uint64_t edi;
    uint32_t _edi;
    uint32_t error_code;
    uint32_t entry_vector;
    uint64_t rip;
    uint64_t eip;
    uint32_t _eip;
    uint16_t cs;
    uint16_t _pad0[1];
    uint8_t saved_upcall_mask;
    uint8_t _pad1[3];
    uint64_t rflags;
    uint64_t eflags;
    uint32_t _eflags;
    uint64_t rsp;
    uint64_t esp;
    uint32_t _esp;
    uint16_t ss;
    uint16_t _pad2[3];
    uint16_t es;
    uint16_t _pad3[3];
    uint16_t ds;
    uint16_t _pad4[3];
    uint16_t fs;
    uint16_t _pad5[3];
    uint16_t gs;
    uint16_t _pad6[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct cpu_user_regs {
    uint64_t r15;
    uint64_t r14;
    uint64_t r13;
    uint64_t r12;
    uint64_t rbp;
    uint64_t ebp;
    uint32_t _ebp;
    uint64_t rbx;
    uint64_t ebx;
    uint32_t _ebx;
    uint64_t r11;
    uint64_t r10;
    uint64_t r9;
    uint64_t r8;
    uint64_t rax;
    uint64_t eax;
    uint32_t _eax;
    uint64_t rcx;
    uint64_t ecx;
    uint32_t _ecx;
    uint64_t rdx;
    uint64_t edx;
    uint32_t _edx;
    uint64_t rsi;
    uint64_t esi;
    uint32_t _esi;
    uint64_t rdi;
    uint64_t edi;
    uint32_t _edi;
    uint32_t error_code;
    uint32_t entry_vector;
    uint64_t rip;
    uint64_t eip;
    uint32_t _eip;
    uint16_t cs;
    uint16_t _pad0[1];
    uint8_t saved_upcall_mask;
    uint8_t _pad1[3];
    uint64_t rflags;
    uint64_t eflags;
    uint32_t _eflags;
    uint64_t rsp;
    uint64_t esp;
    uint32_t _esp;
    uint16_t ss;
    uint16_t _pad2[3];
    uint16_t es;
    uint16_t _pad3[3];
    uint16_t ds;
    uint16_t _pad4[3];
    uint16_t fs;
    uint16_t _pad5[3];
    uint16_t gs;
    uint16_t _pad6[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct cpu_user_regs {
    uint64_t r15;
    uint64_t r14;
    uint64_t r13;
    uint64_t r12;
    uint64_t rbp;
    uint64_t ebp;
    uint32_t _ebp;
    uint64_t rbx;
    uint64_t ebx;
    uint32_t _ebx;
    uint64_t r11;
    uint64_t r10;
    uint64_t r9;
    uint64_t r8;
    uint64_t rax;
    uint64_t eax;
    uint32_t _eax;
    uint64_t rcx;
    uint64_t ecx;
    uint32_t _ecx;
    uint64_t rdx;
    uint64_t edx;
    uint32_t _edx;
    uint64_t rsi;
    uint64_t esi;
    uint32_t _esi;
    uint64_t rdi;
    uint64_t edi;
    uint32_t _edi;
    uint32_t error_code;
    uint32_t entry_vector;
    uint64_t rip;
    uint64_t eip;
    uint32_t _eip;
    uint16_t cs;
    uint16_t _pad0[1];
    uint8_t saved_upcall_mask;
    uint8_t _pad1[3];
    uint64_t rflags;
    uint64_t eflags;
    uint32_t _eflags;
    uint64_t rsp;
    uint64_t esp;
    uint32_t _esp;
    uint16_t ss;
    uint16_t _pad2[3];
    uint16_t es;
    uint16_t _pad3[3];
    uint16_t ds;
    uint16_t _pad4[3];
    uint16_t fs;
    uint16_t _pad5[3];
    uint16_t gs;
    uint16_t _pad6[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct cpu_user_regs {
    uint64_t r15;
    uint64_t r14;
    uint64_t r13;
    uint64_t r12;
    uint64_t rbp;
    uint64_t ebp;
    uint32_t _ebp;
    uint64_t rbx;
    uint64_t ebx;
    uint32_t _ebx;
    uint64_t r11;
    uint64_t r10;
    uint64_t r9;
    uint64_t r8;
    uint64_t rax;
    uint64_t eax;
    uint32_t _eax;
    uint64_t rcx;
    uint64_t ecx;
    uint32_t _ecx;
    uint64_t rdx;
    uint64_t edx;
    uint32_t _edx;
    uint64_t rsi;
    uint64_t esi;
    uint32_t _esi;
    uint64_t rdi;
    uint64_t edi;
    uint32_t _edi;
    uint32_t error_code;
    uint32_t entry_vector;
    uint64_t rip;
    uint64_t eip;
    uint32_t _eip;
    uint16_t cs;
    uint16_t _pad0[1];
    uint8_t saved_upcall_mask;
    uint8_t _pad1[3];
    uint64_t rflags;
    uint64_t eflags;
    uint32_t _eflags;
    uint64_t rsp;
    uint64_t esp;
    uint32_t _esp;
    uint16_t ss;
    uint16_t _pad2[3];
    uint16_t es;
    uint16_t _pad3[3];
    uint16_t ds;
    uint16_t _pad4[3];
    uint16_t fs;
    uint16_t _pad5[3];
    uint16_t gs;
    uint16_t _pad6[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct cpu_user_regs {
    uint64_t r15;
    uint64_t r14;
    uint64_t r13;
    uint64_t r12;
    uint64_t rbp;
    uint64_t ebp;
    uint32_t _ebp;
    uint64_t rbx;
    uint64_t ebx;
    uint32_t _ebx;
    uint64_t r11;
    uint64_t r10;
    uint64_t r9;
    uint64_t r8;
    uint64_t rax;
    uint64_t eax;
    uint32_t _eax;
    uint64_t rcx;
    uint64_t ecx;
    uint32_t _ecx;
    uint64_t rdx;
    uint64_t edx;
    uint32_t _edx;
    uint64_t rsi;
    uint64_t esi;
    uint32_t _esi;
    uint64_t rdi;
    uint64_t edi;
    uint32_t _edi;
    uint32_t error_code;
    uint32_t entry_vector;
    uint64_t rip;
    uint64_t eip;
    uint32_t _eip;
    uint16_t cs;
    uint16_t _pad0[1];
    uint8_t saved_upcall_mask;
    uint8_t _pad1[3];
    uint64_t rflags;
    uint64_t eflags;
    uint32_t _eflags;
    uint64_t rsp;
    uint64_t esp;
    uint32_t _esp;
    uint16_t ss;
    uint16_t _pad2[3];
    uint16_t es;
    uint16_t _pad3[3];
    uint16_t ds;
    uint16_t _pad4[3];
    uint16_t fs;
    uint16_t _pad5[3];
    uint16_t gs;
    uint16_t _pad6[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct cpu_user_regs {
    uint64_t r15;
    uint64_t r14;
    uint64_t r13;
    uint64_t r12;
    uint64_t rbp;
    uint64_t ebp;
    uint32_t _ebp;
    uint64_t rbx;
    uint64_t ebx;
    uint32_t _ebx;
    uint64_t r11;
    uint64_t r10;
    uint64_t r9;
    uint64_t r8;
    uint64_t rax;
    uint64_t eax;
    uint32_t _eax;
    uint64_t rcx;
    uint64_t ecx;
    uint32_t _ecx;
    uint64_t rdx;
    uint64_t edx;
    uint32_t _edx;
    uint64_t rsi;
    uint64_t esi;
    uint32_t _esi;
    uint64_t rdi;
    uint64_t edi;
    uint32_t _edi;
    uint32_t error_code;
    uint32_t entry_vector;
    uint64_t rip;
    uint64_t eip;
    uint32_t _eip;
    uint16_t cs;
    uint16_t _pad0[1];
    uint8_t saved_upcall_mask;
    uint8_t _pad1[3];
    uint64_t rflags;
    uint64_t eflags;
    uint32_t _eflags;
    uint64_t rsp;
    uint64_t esp;
    uint32_t _esp;
    uint16_t ss;
    uint16_t _pad2[3];
    uint16_t es;
    uint16_t _pad3[3];
    uint16_t ds;
    uint16_t _pad4[3];
    uint16_t fs;
    uint16_t _pad5[3];
    uint16_t gs;
    uint16_t _pad6[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct cpu_user_regs {
    uint64_t r15;
    uint64_t r14;
    uint64_t r13;
    uint64_t r12;
    uint64_t rbp;
    uint64_t ebp;
    uint32_t _ebp;
    uint64_t rbx;
    uint64_t ebx;
    uint32_t _ebx;
    uint64_t r11;
    uint64_t r10;
    uint64_t r9;
    uint64_t r8;
    uint64_t rax;
    uint64_t eax;
    uint32_t _eax;
    uint64_t rcx;
    uint64_t ecx;
    uint32_t _ecx;
    uint64_t rdx;
    uint64_t edx;
    uint32_t _edx;
    uint64_t rsi;
    uint64_t esi;
    uint32_t _esi;
    uint64_t rdi;
    uint64_t edi;
    uint32_t _edi;
    uint32_t error_code;
    uint32_t entry_vector;
    uint64_t rip;
    uint64_t eip;
    uint32_t _eip;
    uint16_t cs;
    uint16_t _pad0[1];
    uint8_t saved_upcall_mask;
    uint8_t _pad1[3];
    uint64_t rflags;
    uint64_t eflags;
    uint32_t _eflags;
    uint64_t rsp;
    uint64_t esp;
    uint32_t _esp;
    uint16_t ss;
    uint16_t _pad2[3];
    uint16_t es;
    uint16_t _pad3[3];
    uint16_t ds;
    uint16_t _pad4[3];
    uint16_t fs;
    uint16_t _pad5[3];
    uint16_t gs;
    uint16_t _pad6[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct cpu_user_regs {
    uint64_t r15;
    uint64_t r14;
    uint64_t r13;
    uint64_t r12;
    uint64_t rbp;
    uint64_t ebp;
    uint32_t _ebp;
    uint64_t rbx;
    uint64_t ebx;
    uint32_t _ebx;
    uint64_t r11;
    uint64_t r10;
    uint64_t r9;
    uint64_t r8;
    uint64_t rax;
    uint64_t eax;
    uint32_t _eax;
    uint64_t rcx;
    uint64_t ecx;
    uint32_t _ecx;
    uint64_t rdx;
    uint64_t edx;
    uint32_t _edx;
    uint64_t rsi;
    uint64_t esi;
    uint32_t _esi;
    uint64_t rdi;
    uint64_t edi;
    uint32_t _edi;
    uint32_t error_code;
    uint32_t entry_vector;
    uint64_t rip;
    uint64_t eip;
    uint32_t _eip;
    uint16_t cs;
    uint16_t _pad0[1];
    uint8_t saved_upcall_mask;
    uint8_t _pad1[3];
    uint64_t rflags;
    uint64_t eflags;
    uint32_t _eflags;
    uint64_t rsp;
    uint64_t esp;
    uint32_t _esp;
    uint16_t ss;
    uint16_t _pad2[3];
    uint16_t es;
    uint16_t _pad3[3];
    uint16_t ds;
    uint16_t _pad4[3];
    uint16_t fs;
    uint16_t _pad5[3];
    uint16_t gs;
    uint16_t _pad6[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct cpu_user_regs {
    uint64_t r15;
    uint64_t r14;
    uint64_t r13;
    uint64_t r12;
    uint64_t rbp;
    uint64_t ebp;
    uint32_t _ebp;
    uint64_t rbx;
    uint64_t ebx;
    uint32_t _ebx;
    uint64_t r11;
    uint64_t r10;
    uint64_t r9;
    uint64_t r8;
    uint64_t rax;
    uint64_t eax;
    uint32_t _eax;
    uint64_t rcx;
    uint64_t ecx;
    uint32_t _ecx;
    uint64_t rdx;
    uint64_t edx;
    uint32_t _edx;
    uint64_t rsi;
    uint64_t esi;
    uint32_t _esi;
    uint64_t rdi;
    uint64_t edi;
    uint32_t _edi;
    uint32_t error_code;
    uint32_t entry_vector;
    uint64_t rip;
    uint64_t eip;
    uint32_t _eip;
    uint16_t cs;
    uint16_t _pad0[1];
    uint8_t saved_upcall_mask;
    uint8_t _pad1[3];
    uint64_t rflags;
    uint64_t eflags;
    uint32_t _eflags;
    uint64_t rsp;
    uint64_t esp;
    uint32_t _esp;
    uint16_t ss;
    uint16_t _pad2[3];
    uint16_t es;
    uint16_t _pad3[3];
    uint16_t ds;
    uint16_t _pad4[3];
    uint16_t fs;
    uint16_t _pad5[3];
    uint16_t gs;
    uint16_t _pad6[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct cpu_user_regs {
    uint64_t r15;
    uint64_t r14;
    uint64_t r13;
    uint64_t r12;
    uint64_t rbp;
    uint64_t ebp;
    uint32_t _ebp;
    uint64_t rbx;
    uint64_t ebx;
    uint32_t _ebx;
    uint64_t r11;
    uint64_t r10;
    uint64_t r9;
    uint64_t r8;
    uint64_t rax;
    uint64_t eax;
    uint32_t _eax;
    uint64_t rcx;
    uint64_t ecx;
    uint32_t _ecx;
    uint64_t rdx;
    uint64_t edx;
    uint32_t _edx;
    uint64_t rsi;
    uint64_t esi;
    uint32_t _esi;
    uint64_t rdi;
    uint64_t edi;
    uint32_t _edi;
    uint32_t error_code;
    uint32_t entry_vector;
    uint64_t rip;
    uint64_t eip;
    uint32_t _eip;
    uint16_t cs;
    uint16_t _pad0[1];
    uint8_t saved_upcall_mask;
    uint8_t _pad1[3];
    uint64_t rflags;
    uint64_t eflags;
    uint32_t _eflags;
    uint64_t rsp;
    uint64_t esp;
    uint32_t _esp;
    uint16_t ss;
    uint16_t _pad2[3];
    uint16_t es;
    uint16_t _pad3[3];
    uint16_t ds;
    uint16_t _pad4[3];
    uint16_t fs;
    uint16_t _pad5[3];
    uint16_t gs;
    uint16_t _pad6[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct cpu_user_regs {
    uint64_t r15;
    uint64_t r14;
    uint64_t r13;
    uint64_t r12;
    uint64_t rbp;
    uint64_t ebp;
    uint32_t _ebp;
    uint64_t rbx;
    uint64_t ebx;
    uint32_t _ebx;
    uint64_t r11;
    uint64_t r10;
    uint64_t r9;
    uint64_t r8;
    uint64_t rax;
    uint64_t eax;
    uint32_t _eax;
    uint64_t rcx;
    uint64_t ecx;
    uint32_t _ecx;
    uint64_t rdx;
    uint64_t edx;
    uint32_t _edx;
    uint64_t rsi;
    uint64_t esi;
    uint32_t _esi;
    uint64_t rdi;
    uint64_t edi;
    uint32_t _edi;
    uint32_t error_code;
    uint32_t entry_vector;
    uint64_t rip;
    uint64_t eip;
    uint32_t _eip;
    uint16_t cs;
    uint16_t _pad0[1];
    uint8_t saved_upcall_mask;
    uint8_t _pad1[3];
    uint64_t rflags;
    uint64_t eflags;
    uint32_t _eflags;
    uint64_t rsp;
    uint64_t esp;
    uint32_t _esp;
    uint16_t ss;
    uint16_t _pad2[3];
    uint16_t es;
    uint16_t _pad3[3];
    uint16_t ds;
    uint16_t _pad4[3];
    uint16_t fs;
    uint16_t _pad5[3];
    uint16_t gs;
    uint16_t _pad6[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct cpu_user_regs {
    uint64_t r15;
    uint64_t r14;
    uint64_t r13;
    uint64_t r12;
    uint64_t rbp;
    uint64_t ebp;
    uint32_t _ebp;
    uint64_t rbx;
    uint64_t ebx;
    uint32_t _ebx;
    uint64_t r11;
    uint64_t r10;
    uint64_t r9;
    uint64_t r8;
    uint64_t rax;
    uint64_t eax;
    uint32_t _eax;
    uint64_t rcx;
    uint64_t ecx;
    uint32_t _ecx;
    uint64_t rdx;
    uint64_t edx;
    uint32_t _edx;
    uint64_t rsi;
    uint64_t esi;
    uint32_t _esi;
    uint64_t rdi;
    uint64_t edi;
    uint32_t _edi;
    uint32_t error_code;
    uint32_t entry_vector;
    uint64_t rip;
    uint64_t eip;
    uint32_t _eip;
    uint16_t cs;
    uint16_t _pad0[1];
    uint8_t saved_upcall_mask;
    uint8_t _pad1[3];
    uint64_t rflags;
    uint64_t eflags;
    uint32_t _eflags;
    uint64_t rsp;
    uint64_t esp;
    uint32_t _esp;
    uint16_t ss;
    uint16_t _pad2[3];
    uint16_t es;
    uint16_t _pad3[3];
    uint16_t ds;
    uint16_t _pad4[3];
    uint16_t fs;
    uint16_t _pad5[3];
    uint16_t gs;
    uint16_t _pad6[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct cpu_user_regs {
    uint64_t r15;
    uint64_t r14;
    uint64_t r13;
    uint64_t r12;
    uint64_t rbp;
    uint64_t ebp;
    uint32_t _ebp;
    uint64_t rbx;
    uint64_t ebx;
    uint32_t _ebx;
    uint64_t r11;
    uint64_t r10;
    uint64_t r9;
    uint64_t r8;
    uint64_t rax;
    uint64_t eax;
    uint32_t _eax;
    uint64_t rcx;
    uint64_t ecx;
    uint32_t _ecx;
    uint64_t rdx;
    uint64_t edx;
    uint32_t _edx;
    uint64_t rsi;
    uint64_t esi;
    uint32_t _esi;
    uint64_t rdi;
    uint64_t edi;
    uint32_t _edi;
    uint32_t error_code;
    uint32_t entry_vector;
    uint64_t rip;
    uint64_t eip;
    uint32_t _eip;
    uint16_t cs;
    uint16_t _pad0[1];
    uint8_t saved_upcall_mask;
    uint8_t _pad1[3];
    uint64_t rflags;
    uint64_t eflags;
    uint32_t _eflags;
    uint64_t rsp;
    uint64_t esp;
    uint32_t _esp;
    uint16_t ss;
    uint16_t _pad2[3];
    uint16_t es;
    uint16_t _pad3[3];
    uint16_t ds;
    uint16_t _pad4[3];
    uint16_t fs;
    uint16_t _pad5[3];
    uint16_t gs;
    uint16_t _pad6[3];
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
struct cpu_user_regs {
    uint64_t r15;
    uint64_t r14;
    uint64_t r13;
    uint64_t r12;
    uint64_t rbp;
    uint64_t ebp;
    uint32_t _ebp;
    uint64_t rbx;
    uint64_t ebx;
    uint32_t _ebx;
    uint64_t r11;
    uint64_t r10;
    uint64_t r9;
    uint64_t r8;
    uint64_t rax;
    uint64_t eax;
    uint32_t _eax;
    uint64_t rcx;
    uint64_t ecx;
    uint32_t _ecx;
    uint64_t rdx;
    uint64_t edx;
    uint32_t _edx;
    uint64_t rsi;
    uint64_t esi;
    uint32_t _esi;
    uint64_t rdi;
    uint64_t edi;
    uint32_t _edi;
    uint32_t error_code;
    uint32_t entry_vector;
    uint64_t rip;
    uint64_t eip;
    uint32_t _eip;
    uint16_t cs;
    uint16_t _pad0[1];
    uint8_t saved_upcall_mask;
    uint8_t _pad1[3];
    uint64_t rflags;
    uint64_t eflags;
    uint32_t _eflags;
    uint64_t rsp;
    uint64_t esp;
    uint32_t _esp;
    uint16_t ss;
    uint16_t _pad2[3];
    uint16_t es;
    uint16_t _pad3[3];
    uint16_t ds;
    uint16_t _pad4[3];
    uint16_t fs;
    uint16_t _pad5[3];
    uint16_t gs;
    uint16_t _pad6[3];
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
struct cpu_user_regs {
    uint64_t r15;
    uint64_t r14;
    uint64_t r13;
    uint64_t r12;
    uint64_t rbp;
    uint64_t ebp;
    uint32_t _ebp;
    uint64_t rbx;
    uint64_t ebx;
    uint32_t _ebx;
    uint64_t r11;
    uint64_t r10;
    uint64_t r9;
    uint64_t r8;
    uint64_t rax;
    uint64_t eax;
    uint32_t _eax;
    uint64_t rcx;
    uint64_t ecx;
    uint32_t _ecx;
    uint64_t rdx;
    uint64_t edx;
    uint32_t _edx;
    uint64_t rsi;
    uint64_t esi;
    uint32_t _esi;
    uint64_t rdi;
    uint64_t edi;
    uint32_t _edi;
    uint32_t error_code;
    uint32_t entry_vector;
    uint64_t rip;
    uint64_t eip;
    uint32_t _eip;
    uint16_t cs;
    uint16_t _pad0[1];
    uint8_t saved_upcall_mask;
    uint8_t _pad1[3];
    uint64_t rflags;
    uint64_t eflags;
    uint32_t _eflags;
    uint64_t rsp;
    uint64_t esp;
    uint32_t _esp;
    uint16_t ss;
    uint16_t _pad2[3];
    uint16_t es;
    uint16_t _pad3[3];
    uint16_t ds;
    uint16_t _pad4[3];
    uint16_t fs;
    uint16_t _pad5[3];
    uint16_t gs;
    uint16_t _pad6[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cpu_user_regs {
    uint64_t r15;
    uint64_t r14;
    uint64_t r13;
    uint64_t r12;
    uint64_t rbp;
    uint64_t ebp;
    uint32_t _ebp;
    uint64_t rbx;
    uint64_t ebx;
    uint32_t _ebx;
    uint64_t r11;
    uint64_t r10;
    uint64_t r9;
    uint64_t r8;
    uint64_t rax;
    uint64_t eax;
    uint32_t _eax;
    uint64_t rcx;
    uint64_t ecx;
    uint32_t _ecx;
    uint64_t rdx;
    uint64_t edx;
    uint32_t _edx;
    uint64_t rsi;
    uint64_t esi;
    uint32_t _esi;
    uint64_t rdi;
    uint64_t edi;
    uint32_t _edi;
    uint32_t error_code;
    uint32_t entry_vector;
    uint64_t rip;
    uint64_t eip;
    uint32_t _eip;
    uint16_t cs;
    uint16_t _pad0[1];
    uint8_t saved_upcall_mask;
    uint8_t _pad1[3];
    uint64_t rflags;
    uint64_t eflags;
    uint32_t _eflags;
    uint64_t rsp;
    uint64_t esp;
    uint32_t _esp;
    uint16_t ss;
    uint16_t _pad2[3];
    uint16_t es;
    uint16_t _pad3[3];
    uint16_t ds;
    uint16_t _pad4[3];
    uint16_t fs;
    uint16_t _pad5[3];
    uint16_t gs;
    uint16_t _pad6[3];
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
