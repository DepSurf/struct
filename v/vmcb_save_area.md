# Struct: <code>vmcb_save_area</code>

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
struct vmcb_save_area {
    struct vmcb_seg es;
    struct vmcb_seg cs;
    struct vmcb_seg ss;
    struct vmcb_seg ds;
    struct vmcb_seg fs;
    struct vmcb_seg gs;
    struct vmcb_seg gdtr;
    struct vmcb_seg ldtr;
    struct vmcb_seg idtr;
    struct vmcb_seg tr;
    u8 reserved_1[43];
    u8 cpl;
    u8 reserved_2[4];
    u64 efer;
    u8 reserved_3[104];
    u64 xss;
    u64 cr4;
    u64 cr3;
    u64 cr0;
    u64 dr7;
    u64 dr6;
    u64 rflags;
    u64 rip;
    u8 reserved_4[88];
    u64 rsp;
    u8 reserved_5[24];
    u64 rax;
    u64 star;
    u64 lstar;
    u64 cstar;
    u64 sfmask;
    u64 kernel_gs_base;
    u64 sysenter_cs;
    u64 sysenter_esp;
    u64 sysenter_eip;
    u64 cr2;
    u8 reserved_6[32];
    u64 g_pat;
    u64 dbgctl;
    u64 br_from;
    u64 br_to;
    u64 last_excp_from;
    u64 last_excp_to;
    u8 reserved_7[80];
    u32 pkru;
    u8 reserved_7a[20];
    u64 reserved_8;
    u64 rcx;
    u64 rdx;
    u64 rbx;
    u64 reserved_9;
    u64 rbp;
    u64 rsi;
    u64 rdi;
    u64 r8;
    u64 r9;
    u64 r10;
    u64 r11;
    u64 r12;
    u64 r13;
    u64 r14;
    u64 r15;
    u8 reserved_10[16];
    u64 sw_exit_code;
    u64 sw_exit_info_1;
    u64 sw_exit_info_2;
    u64 sw_scratch;
    u8 reserved_11[56];
    u64 xcr0;
    u8 valid_bitmap[16];
    u64 x87_state_gpa;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct vmcb_save_area {
    struct vmcb_seg es;
    struct vmcb_seg cs;
    struct vmcb_seg ss;
    struct vmcb_seg ds;
    struct vmcb_seg fs;
    struct vmcb_seg gs;
    struct vmcb_seg gdtr;
    struct vmcb_seg ldtr;
    struct vmcb_seg idtr;
    struct vmcb_seg tr;
    u8 reserved_1[43];
    u8 cpl;
    u8 reserved_2[4];
    u64 efer;
    u8 reserved_3[104];
    u64 xss;
    u64 cr4;
    u64 cr3;
    u64 cr0;
    u64 dr7;
    u64 dr6;
    u64 rflags;
    u64 rip;
    u8 reserved_4[88];
    u64 rsp;
    u8 reserved_5[24];
    u64 rax;
    u64 star;
    u64 lstar;
    u64 cstar;
    u64 sfmask;
    u64 kernel_gs_base;
    u64 sysenter_cs;
    u64 sysenter_esp;
    u64 sysenter_eip;
    u64 cr2;
    u8 reserved_6[32];
    u64 g_pat;
    u64 dbgctl;
    u64 br_from;
    u64 br_to;
    u64 last_excp_from;
    u64 last_excp_to;
    u8 reserved_7[72];
    u32 spec_ctrl;
    u8 reserved_7b[4];
    u32 pkru;
    u8 reserved_7a[20];
    u64 reserved_8;
    u64 rcx;
    u64 rdx;
    u64 rbx;
    u64 reserved_9;
    u64 rbp;
    u64 rsi;
    u64 rdi;
    u64 r8;
    u64 r9;
    u64 r10;
    u64 r11;
    u64 r12;
    u64 r13;
    u64 r14;
    u64 r15;
    u8 reserved_10[16];
    u64 sw_exit_code;
    u64 sw_exit_info_1;
    u64 sw_exit_info_2;
    u64 sw_scratch;
    u8 reserved_11[56];
    u64 xcr0;
    u8 valid_bitmap[16];
    u64 x87_state_gpa;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct vmcb_save_area {
    struct vmcb_seg es;
    struct vmcb_seg cs;
    struct vmcb_seg ss;
    struct vmcb_seg ds;
    struct vmcb_seg fs;
    struct vmcb_seg gs;
    struct vmcb_seg gdtr;
    struct vmcb_seg ldtr;
    struct vmcb_seg idtr;
    struct vmcb_seg tr;
    u8 reserved_1[43];
    u8 cpl;
    u8 reserved_2[4];
    u64 efer;
    u8 reserved_3[104];
    u64 xss;
    u64 cr4;
    u64 cr3;
    u64 cr0;
    u64 dr7;
    u64 dr6;
    u64 rflags;
    u64 rip;
    u8 reserved_4[88];
    u64 rsp;
    u8 reserved_5[24];
    u64 rax;
    u64 star;
    u64 lstar;
    u64 cstar;
    u64 sfmask;
    u64 kernel_gs_base;
    u64 sysenter_cs;
    u64 sysenter_esp;
    u64 sysenter_eip;
    u64 cr2;
    u8 reserved_6[32];
    u64 g_pat;
    u64 dbgctl;
    u64 br_from;
    u64 br_to;
    u64 last_excp_from;
    u64 last_excp_to;
    u8 reserved_7[72];
    u32 spec_ctrl;
    u8 reserved_7b[4];
    u32 pkru;
    u8 reserved_7a[20];
    u64 reserved_8;
    u64 rcx;
    u64 rdx;
    u64 rbx;
    u64 reserved_9;
    u64 rbp;
    u64 rsi;
    u64 rdi;
    u64 r8;
    u64 r9;
    u64 r10;
    u64 r11;
    u64 r12;
    u64 r13;
    u64 r14;
    u64 r15;
    u8 reserved_10[16];
    u64 sw_exit_code;
    u64 sw_exit_info_1;
    u64 sw_exit_info_2;
    u64 sw_scratch;
    u8 reserved_11[56];
    u64 xcr0;
    u8 valid_bitmap[16];
    u64 x87_state_gpa;
};
```
</details>
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
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 spec_ctrl</code>
</li>
<li>
<b>Field added. </b>
<code>u8 reserved_7b[4]</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 reserved_7[80]</code> ➡️ <code>u8 reserved_7[72]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
</ul>
