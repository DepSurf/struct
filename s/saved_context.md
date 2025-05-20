# Struct: <code>saved_context</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct saved_context {
    struct pt_regs regs;
    u16 ds;
    u16 es;
    u16 fs;
    u16 gs;
    u16 ss;
    long unsigned int gs_base;
    long unsigned int gs_kernel_base;
    long unsigned int fs_base;
    long unsigned int cr0;
    long unsigned int cr2;
    long unsigned int cr3;
    long unsigned int cr4;
    long unsigned int cr8;
    u64 misc_enable;
    bool misc_enable_saved;
    long unsigned int efer;
    u16 gdt_pad;
    struct desc_ptr gdt_desc;
    u16 idt_pad;
    u16 idt_limit;
    long unsigned int idt_base;
    u16 ldt;
    u16 tss;
    long unsigned int tr;
    long unsigned int safety;
    long unsigned int return_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct saved_context {
    struct pt_regs regs;
    u16 ds;
    u16 es;
    u16 fs;
    u16 gs;
    u16 ss;
    long unsigned int gs_base;
    long unsigned int gs_kernel_base;
    long unsigned int fs_base;
    long unsigned int cr0;
    long unsigned int cr2;
    long unsigned int cr3;
    long unsigned int cr4;
    long unsigned int cr8;
    u64 misc_enable;
    bool misc_enable_saved;
    struct saved_msrs saved_msrs;
    long unsigned int efer;
    u16 gdt_pad;
    struct desc_ptr gdt_desc;
    u16 idt_pad;
    u16 idt_limit;
    long unsigned int idt_base;
    u16 ldt;
    u16 tss;
    long unsigned int tr;
    long unsigned int safety;
    long unsigned int return_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct saved_context {
    struct pt_regs regs;
    u16 ds;
    u16 es;
    u16 fs;
    u16 gs;
    u16 ss;
    long unsigned int gs_base;
    long unsigned int gs_kernel_base;
    long unsigned int fs_base;
    long unsigned int cr0;
    long unsigned int cr2;
    long unsigned int cr3;
    long unsigned int cr4;
    long unsigned int cr8;
    u64 misc_enable;
    bool misc_enable_saved;
    struct saved_msrs saved_msrs;
    long unsigned int efer;
    u16 gdt_pad;
    struct desc_ptr gdt_desc;
    u16 idt_pad;
    u16 idt_limit;
    long unsigned int idt_base;
    u16 ldt;
    u16 tss;
    long unsigned int tr;
    long unsigned int safety;
    long unsigned int return_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct saved_context {
    struct pt_regs regs;
    u16 ds;
    u16 es;
    u16 fs;
    u16 gs;
    u16 ss;
    long unsigned int gs_base;
    long unsigned int gs_kernel_base;
    long unsigned int fs_base;
    long unsigned int cr0;
    long unsigned int cr2;
    long unsigned int cr3;
    long unsigned int cr4;
    long unsigned int cr8;
    u64 misc_enable;
    bool misc_enable_saved;
    struct saved_msrs saved_msrs;
    long unsigned int efer;
    u16 gdt_pad;
    struct desc_ptr gdt_desc;
    u16 idt_pad;
    u16 idt_limit;
    long unsigned int idt_base;
    u16 ldt;
    u16 tss;
    long unsigned int tr;
    long unsigned int safety;
    long unsigned int return_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct saved_context {
    struct pt_regs regs;
    u16 ds;
    u16 es;
    u16 fs;
    u16 gs;
    long unsigned int kernelmode_gs_base;
    long unsigned int usermode_gs_base;
    long unsigned int fs_base;
    long unsigned int cr0;
    long unsigned int cr2;
    long unsigned int cr3;
    long unsigned int cr4;
    long unsigned int cr8;
    u64 misc_enable;
    bool misc_enable_saved;
    struct saved_msrs saved_msrs;
    long unsigned int efer;
    u16 gdt_pad;
    struct desc_ptr gdt_desc;
    u16 idt_pad;
    struct desc_ptr idt;
    u16 ldt;
    u16 tss;
    long unsigned int tr;
    long unsigned int safety;
    long unsigned int return_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct saved_context {
    struct pt_regs regs;
    u16 ds;
    u16 es;
    u16 fs;
    u16 gs;
    long unsigned int kernelmode_gs_base;
    long unsigned int usermode_gs_base;
    long unsigned int fs_base;
    long unsigned int cr0;
    long unsigned int cr2;
    long unsigned int cr3;
    long unsigned int cr4;
    long unsigned int cr8;
    u64 misc_enable;
    bool misc_enable_saved;
    struct saved_msrs saved_msrs;
    long unsigned int efer;
    u16 gdt_pad;
    struct desc_ptr gdt_desc;
    u16 idt_pad;
    struct desc_ptr idt;
    u16 ldt;
    u16 tss;
    long unsigned int tr;
    long unsigned int safety;
    long unsigned int return_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct saved_context {
    struct pt_regs regs;
    u16 ds;
    u16 es;
    u16 fs;
    u16 gs;
    long unsigned int kernelmode_gs_base;
    long unsigned int usermode_gs_base;
    long unsigned int fs_base;
    long unsigned int cr0;
    long unsigned int cr2;
    long unsigned int cr3;
    long unsigned int cr4;
    long unsigned int cr8;
    u64 misc_enable;
    bool misc_enable_saved;
    struct saved_msrs saved_msrs;
    long unsigned int efer;
    u16 gdt_pad;
    struct desc_ptr gdt_desc;
    u16 idt_pad;
    struct desc_ptr idt;
    u16 ldt;
    u16 tss;
    long unsigned int tr;
    long unsigned int safety;
    long unsigned int return_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct saved_context {
    struct pt_regs regs;
    u16 ds;
    u16 es;
    u16 fs;
    u16 gs;
    long unsigned int kernelmode_gs_base;
    long unsigned int usermode_gs_base;
    long unsigned int fs_base;
    long unsigned int cr0;
    long unsigned int cr2;
    long unsigned int cr3;
    long unsigned int cr4;
    long unsigned int cr8;
    u64 misc_enable;
    bool misc_enable_saved;
    struct saved_msrs saved_msrs;
    long unsigned int efer;
    u16 gdt_pad;
    struct desc_ptr gdt_desc;
    u16 idt_pad;
    struct desc_ptr idt;
    u16 ldt;
    u16 tss;
    long unsigned int tr;
    long unsigned int safety;
    long unsigned int return_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct saved_context {
    struct pt_regs regs;
    u16 ds;
    u16 es;
    u16 fs;
    u16 gs;
    long unsigned int kernelmode_gs_base;
    long unsigned int usermode_gs_base;
    long unsigned int fs_base;
    long unsigned int cr0;
    long unsigned int cr2;
    long unsigned int cr3;
    long unsigned int cr4;
    u64 misc_enable;
    bool misc_enable_saved;
    struct saved_msrs saved_msrs;
    long unsigned int efer;
    u16 gdt_pad;
    struct desc_ptr gdt_desc;
    u16 idt_pad;
    struct desc_ptr idt;
    u16 ldt;
    u16 tss;
    long unsigned int tr;
    long unsigned int safety;
    long unsigned int return_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct saved_context {
    struct pt_regs regs;
    u16 ds;
    u16 es;
    u16 fs;
    u16 gs;
    long unsigned int kernelmode_gs_base;
    long unsigned int usermode_gs_base;
    long unsigned int fs_base;
    long unsigned int cr0;
    long unsigned int cr2;
    long unsigned int cr3;
    long unsigned int cr4;
    u64 misc_enable;
    bool misc_enable_saved;
    struct saved_msrs saved_msrs;
    long unsigned int efer;
    u16 gdt_pad;
    struct desc_ptr gdt_desc;
    u16 idt_pad;
    struct desc_ptr idt;
    u16 ldt;
    u16 tss;
    long unsigned int tr;
    long unsigned int safety;
    long unsigned int return_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct saved_context {
    struct pt_regs regs;
    u16 ds;
    u16 es;
    u16 fs;
    u16 gs;
    long unsigned int kernelmode_gs_base;
    long unsigned int usermode_gs_base;
    long unsigned int fs_base;
    long unsigned int cr0;
    long unsigned int cr2;
    long unsigned int cr3;
    long unsigned int cr4;
    u64 misc_enable;
    bool misc_enable_saved;
    struct saved_msrs saved_msrs;
    long unsigned int efer;
    u16 gdt_pad;
    struct desc_ptr gdt_desc;
    u16 idt_pad;
    struct desc_ptr idt;
    u16 ldt;
    u16 tss;
    long unsigned int tr;
    long unsigned int safety;
    long unsigned int return_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct saved_context {
    struct pt_regs regs;
    u16 ds;
    u16 es;
    u16 fs;
    u16 gs;
    long unsigned int kernelmode_gs_base;
    long unsigned int usermode_gs_base;
    long unsigned int fs_base;
    long unsigned int cr0;
    long unsigned int cr2;
    long unsigned int cr3;
    long unsigned int cr4;
    u64 misc_enable;
    bool misc_enable_saved;
    struct saved_msrs saved_msrs;
    long unsigned int efer;
    u16 gdt_pad;
    struct desc_ptr gdt_desc;
    u16 idt_pad;
    struct desc_ptr idt;
    u16 ldt;
    u16 tss;
    long unsigned int tr;
    long unsigned int safety;
    long unsigned int return_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct saved_context {
    struct pt_regs regs;
    u16 ds;
    u16 es;
    u16 fs;
    u16 gs;
    long unsigned int kernelmode_gs_base;
    long unsigned int usermode_gs_base;
    long unsigned int fs_base;
    long unsigned int cr0;
    long unsigned int cr2;
    long unsigned int cr3;
    long unsigned int cr4;
    u64 misc_enable;
    bool misc_enable_saved;
    struct saved_msrs saved_msrs;
    long unsigned int efer;
    u16 gdt_pad;
    struct desc_ptr gdt_desc;
    u16 idt_pad;
    struct desc_ptr idt;
    u16 ldt;
    u16 tss;
    long unsigned int tr;
    long unsigned int safety;
    long unsigned int return_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct saved_context {
    struct pt_regs regs;
    u16 ds;
    u16 es;
    u16 fs;
    u16 gs;
    long unsigned int kernelmode_gs_base;
    long unsigned int usermode_gs_base;
    long unsigned int fs_base;
    long unsigned int cr0;
    long unsigned int cr2;
    long unsigned int cr3;
    long unsigned int cr4;
    u64 misc_enable;
    struct saved_msrs saved_msrs;
    long unsigned int efer;
    u16 gdt_pad;
    struct desc_ptr gdt_desc;
    u16 idt_pad;
    struct desc_ptr idt;
    u16 ldt;
    u16 tss;
    long unsigned int tr;
    long unsigned int safety;
    long unsigned int return_address;
    bool misc_enable_saved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct saved_context {
    struct pt_regs regs;
    u16 ds;
    u16 es;
    u16 fs;
    u16 gs;
    long unsigned int kernelmode_gs_base;
    long unsigned int usermode_gs_base;
    long unsigned int fs_base;
    long unsigned int cr0;
    long unsigned int cr2;
    long unsigned int cr3;
    long unsigned int cr4;
    u64 misc_enable;
    struct saved_msrs saved_msrs;
    long unsigned int efer;
    u16 gdt_pad;
    struct desc_ptr gdt_desc;
    u16 idt_pad;
    struct desc_ptr idt;
    u16 ldt;
    u16 tss;
    long unsigned int tr;
    long unsigned int safety;
    long unsigned int return_address;
    bool misc_enable_saved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct saved_context {
    struct pt_regs regs;
    u16 ds;
    u16 es;
    u16 fs;
    u16 gs;
    long unsigned int kernelmode_gs_base;
    long unsigned int usermode_gs_base;
    long unsigned int fs_base;
    long unsigned int cr0;
    long unsigned int cr2;
    long unsigned int cr3;
    long unsigned int cr4;
    u64 misc_enable;
    struct saved_msrs saved_msrs;
    long unsigned int efer;
    u16 gdt_pad;
    struct desc_ptr gdt_desc;
    u16 idt_pad;
    struct desc_ptr idt;
    u16 ldt;
    u16 tss;
    long unsigned int tr;
    long unsigned int safety;
    long unsigned int return_address;
    bool misc_enable_saved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct saved_context {
    struct pt_regs regs;
    u16 ds;
    u16 es;
    u16 fs;
    u16 gs;
    long unsigned int kernelmode_gs_base;
    long unsigned int usermode_gs_base;
    long unsigned int fs_base;
    long unsigned int cr0;
    long unsigned int cr2;
    long unsigned int cr3;
    long unsigned int cr4;
    u64 misc_enable;
    struct saved_msrs saved_msrs;
    long unsigned int efer;
    u16 gdt_pad;
    struct desc_ptr gdt_desc;
    u16 idt_pad;
    struct desc_ptr idt;
    u16 ldt;
    u16 tss;
    long unsigned int tr;
    long unsigned int safety;
    long unsigned int return_address;
    bool misc_enable_saved;
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
struct saved_context {
    struct pt_regs regs;
    u16 ds;
    u16 es;
    u16 fs;
    u16 gs;
    long unsigned int kernelmode_gs_base;
    long unsigned int usermode_gs_base;
    long unsigned int fs_base;
    long unsigned int cr0;
    long unsigned int cr2;
    long unsigned int cr3;
    long unsigned int cr4;
    u64 misc_enable;
    bool misc_enable_saved;
    struct saved_msrs saved_msrs;
    long unsigned int efer;
    u16 gdt_pad;
    struct desc_ptr gdt_desc;
    u16 idt_pad;
    struct desc_ptr idt;
    u16 ldt;
    u16 tss;
    long unsigned int tr;
    long unsigned int safety;
    long unsigned int return_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct saved_context {
    struct pt_regs regs;
    u16 ds;
    u16 es;
    u16 fs;
    u16 gs;
    long unsigned int kernelmode_gs_base;
    long unsigned int usermode_gs_base;
    long unsigned int fs_base;
    long unsigned int cr0;
    long unsigned int cr2;
    long unsigned int cr3;
    long unsigned int cr4;
    u64 misc_enable;
    bool misc_enable_saved;
    struct saved_msrs saved_msrs;
    long unsigned int efer;
    u16 gdt_pad;
    struct desc_ptr gdt_desc;
    u16 idt_pad;
    struct desc_ptr idt;
    u16 ldt;
    u16 tss;
    long unsigned int tr;
    long unsigned int safety;
    long unsigned int return_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct saved_context {
    struct pt_regs regs;
    u16 ds;
    u16 es;
    u16 fs;
    u16 gs;
    long unsigned int kernelmode_gs_base;
    long unsigned int usermode_gs_base;
    long unsigned int fs_base;
    long unsigned int cr0;
    long unsigned int cr2;
    long unsigned int cr3;
    long unsigned int cr4;
    u64 misc_enable;
    bool misc_enable_saved;
    struct saved_msrs saved_msrs;
    long unsigned int efer;
    u16 gdt_pad;
    struct desc_ptr gdt_desc;
    u16 idt_pad;
    struct desc_ptr idt;
    u16 ldt;
    u16 tss;
    long unsigned int tr;
    long unsigned int safety;
    long unsigned int return_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct saved_context {
    struct pt_regs regs;
    u16 ds;
    u16 es;
    u16 fs;
    u16 gs;
    long unsigned int kernelmode_gs_base;
    long unsigned int usermode_gs_base;
    long unsigned int fs_base;
    long unsigned int cr0;
    long unsigned int cr2;
    long unsigned int cr3;
    long unsigned int cr4;
    u64 misc_enable;
    bool misc_enable_saved;
    struct saved_msrs saved_msrs;
    long unsigned int efer;
    u16 gdt_pad;
    struct desc_ptr gdt_desc;
    u16 idt_pad;
    struct desc_ptr idt;
    u16 ldt;
    u16 tss;
    long unsigned int tr;
    long unsigned int safety;
    long unsigned int return_address;
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
<code>struct saved_msrs saved_msrs</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int kernelmode_gs_base</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int usermode_gs_base</code>
</li>
<li>
<b>Field added. </b>
<code>struct desc_ptr idt</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 ss</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int gs_base</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int gs_kernel_base</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 idt_limit</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int idt_base</code>
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
<code>long unsigned int cr8</code>
</li>
</ul>
</details>
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
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
