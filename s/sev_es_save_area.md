# Struct: <code>sev_es_save_area</code>

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
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct sev_es_save_area {
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
    u64 vmpl0_ssp;
    u64 vmpl1_ssp;
    u64 vmpl2_ssp;
    u64 vmpl3_ssp;
    u64 u_cet;
    u8 reserved_1[2];
    u8 vmpl;
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
    u64 dr0;
    u64 dr1;
    u64 dr2;
    u64 dr3;
    u64 dr0_addr_mask;
    u64 dr1_addr_mask;
    u64 dr2_addr_mask;
    u64 dr3_addr_mask;
    u8 reserved_4[24];
    u64 rsp;
    u64 s_cet;
    u64 ssp;
    u64 isst_addr;
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
    u8 reserved_5[32];
    u64 g_pat;
    u64 dbgctl;
    u64 br_from;
    u64 br_to;
    u64 last_excp_from;
    u64 last_excp_to;
    u8 reserved_7[80];
    u32 pkru;
    u8 reserved_8[20];
    u64 reserved_9;
    u64 rcx;
    u64 rdx;
    u64 rbx;
    u64 reserved_10;
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
    u8 reserved_11[16];
    u64 guest_exit_info_1;
    u64 guest_exit_info_2;
    u64 guest_exit_int_info;
    u64 guest_nrip;
    u64 sev_features;
    u64 vintr_ctrl;
    u64 guest_exit_code;
    u64 virtual_tom;
    u64 tlb_id;
    u64 pcpu_id;
    u64 event_inj;
    u64 xcr0;
    u8 reserved_12[16];
    u64 x87_dp;
    u32 mxcsr;
    u16 x87_ftw;
    u16 x87_fsw;
    u16 x87_fcw;
    u16 x87_fop;
    u16 x87_ds;
    u16 x87_cs;
    u64 x87_rip;
    u8 fpreg_x87[80];
    u8 fpreg_xmm[256];
    u8 fpreg_ymm[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct sev_es_save_area {
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
    u64 vmpl0_ssp;
    u64 vmpl1_ssp;
    u64 vmpl2_ssp;
    u64 vmpl3_ssp;
    u64 u_cet;
    u8 reserved_0xc8[2];
    u8 vmpl;
    u8 cpl;
    u8 reserved_0xcc[4];
    u64 efer;
    u8 reserved_0xd8[104];
    u64 xss;
    u64 cr4;
    u64 cr3;
    u64 cr0;
    u64 dr7;
    u64 dr6;
    u64 rflags;
    u64 rip;
    u64 dr0;
    u64 dr1;
    u64 dr2;
    u64 dr3;
    u64 dr0_addr_mask;
    u64 dr1_addr_mask;
    u64 dr2_addr_mask;
    u64 dr3_addr_mask;
    u8 reserved_0x1c0[24];
    u64 rsp;
    u64 s_cet;
    u64 ssp;
    u64 isst_addr;
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
    u8 reserved_0x248[32];
    u64 g_pat;
    u64 dbgctl;
    u64 br_from;
    u64 br_to;
    u64 last_excp_from;
    u64 last_excp_to;
    u8 reserved_0x298[80];
    u32 pkru;
    u32 tsc_aux;
    u8 reserved_0x2f0[24];
    u64 rcx;
    u64 rdx;
    u64 rbx;
    u64 reserved_0x320;
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
    u8 reserved_0x380[16];
    u64 guest_exit_info_1;
    u64 guest_exit_info_2;
    u64 guest_exit_int_info;
    u64 guest_nrip;
    u64 sev_features;
    u64 vintr_ctrl;
    u64 guest_exit_code;
    u64 virtual_tom;
    u64 tlb_id;
    u64 pcpu_id;
    u64 event_inj;
    u64 xcr0;
    u8 reserved_0x3f0[16];
    u64 x87_dp;
    u32 mxcsr;
    u16 x87_ftw;
    u16 x87_fsw;
    u16 x87_fcw;
    u16 x87_fop;
    u16 x87_ds;
    u16 x87_cs;
    u64 x87_rip;
    u8 fpreg_x87[80];
    u8 fpreg_xmm[256];
    u8 fpreg_ymm[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct sev_es_save_area {
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
    u64 vmpl0_ssp;
    u64 vmpl1_ssp;
    u64 vmpl2_ssp;
    u64 vmpl3_ssp;
    u64 u_cet;
    u8 reserved_0xc8[2];
    u8 vmpl;
    u8 cpl;
    u8 reserved_0xcc[4];
    u64 efer;
    u8 reserved_0xd8[104];
    u64 xss;
    u64 cr4;
    u64 cr3;
    u64 cr0;
    u64 dr7;
    u64 dr6;
    u64 rflags;
    u64 rip;
    u64 dr0;
    u64 dr1;
    u64 dr2;
    u64 dr3;
    u64 dr0_addr_mask;
    u64 dr1_addr_mask;
    u64 dr2_addr_mask;
    u64 dr3_addr_mask;
    u8 reserved_0x1c0[24];
    u64 rsp;
    u64 s_cet;
    u64 ssp;
    u64 isst_addr;
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
    u8 reserved_0x248[32];
    u64 g_pat;
    u64 dbgctl;
    u64 br_from;
    u64 br_to;
    u64 last_excp_from;
    u64 last_excp_to;
    u8 reserved_0x298[80];
    u32 pkru;
    u32 tsc_aux;
    u8 reserved_0x2f0[24];
    u64 rcx;
    u64 rdx;
    u64 rbx;
    u64 reserved_0x320;
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
    u8 reserved_0x380[16];
    u64 guest_exit_info_1;
    u64 guest_exit_info_2;
    u64 guest_exit_int_info;
    u64 guest_nrip;
    u64 sev_features;
    u64 vintr_ctrl;
    u64 guest_exit_code;
    u64 virtual_tom;
    u64 tlb_id;
    u64 pcpu_id;
    u64 event_inj;
    u64 xcr0;
    u8 reserved_0x3f0[16];
    u64 x87_dp;
    u32 mxcsr;
    u16 x87_ftw;
    u16 x87_fsw;
    u16 x87_fcw;
    u16 x87_fop;
    u16 x87_ds;
    u16 x87_cs;
    u64 x87_rip;
    u8 fpreg_x87[80];
    u8 fpreg_xmm[256];
    u8 fpreg_ymm[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct sev_es_save_area {
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
    u64 vmpl0_ssp;
    u64 vmpl1_ssp;
    u64 vmpl2_ssp;
    u64 vmpl3_ssp;
    u64 u_cet;
    u8 reserved_0xc8[2];
    u8 vmpl;
    u8 cpl;
    u8 reserved_0xcc[4];
    u64 efer;
    u8 reserved_0xd8[104];
    u64 xss;
    u64 cr4;
    u64 cr3;
    u64 cr0;
    u64 dr7;
    u64 dr6;
    u64 rflags;
    u64 rip;
    u64 dr0;
    u64 dr1;
    u64 dr2;
    u64 dr3;
    u64 dr0_addr_mask;
    u64 dr1_addr_mask;
    u64 dr2_addr_mask;
    u64 dr3_addr_mask;
    u8 reserved_0x1c0[24];
    u64 rsp;
    u64 s_cet;
    u64 ssp;
    u64 isst_addr;
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
    u8 reserved_0x248[32];
    u64 g_pat;
    u64 dbgctl;
    u64 br_from;
    u64 br_to;
    u64 last_excp_from;
    u64 last_excp_to;
    u8 reserved_0x298[80];
    u32 pkru;
    u32 tsc_aux;
    u8 reserved_0x2f0[24];
    u64 rcx;
    u64 rdx;
    u64 rbx;
    u64 reserved_0x320;
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
    u8 reserved_0x380[16];
    u64 guest_exit_info_1;
    u64 guest_exit_info_2;
    u64 guest_exit_int_info;
    u64 guest_nrip;
    u64 sev_features;
    u64 vintr_ctrl;
    u64 guest_exit_code;
    u64 virtual_tom;
    u64 tlb_id;
    u64 pcpu_id;
    u64 event_inj;
    u64 xcr0;
    u8 reserved_0x3f0[16];
    u64 x87_dp;
    u32 mxcsr;
    u16 x87_ftw;
    u16 x87_fsw;
    u16 x87_fcw;
    u16 x87_fop;
    u16 x87_ds;
    u16 x87_cs;
    u64 x87_rip;
    u8 fpreg_x87[80];
    u8 fpreg_xmm[256];
    u8 fpreg_ymm[256];
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
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 reserved_0xc8[2]</code>
</li>
<li>
<b>Field added. </b>
<code>u8 reserved_0xcc[4]</code>
</li>
<li>
<b>Field added. </b>
<code>u8 reserved_0xd8[104]</code>
</li>
<li>
<b>Field added. </b>
<code>u8 reserved_0x1c0[24]</code>
</li>
<li>
<b>Field added. </b>
<code>u8 reserved_0x248[32]</code>
</li>
<li>
<b>Field added. </b>
<code>u8 reserved_0x298[80]</code>
</li>
<li>
<b>Field added. </b>
<code>u32 tsc_aux</code>
</li>
<li>
<b>Field added. </b>
<code>u8 reserved_0x2f0[24]</code>
</li>
<li>
<b>Field added. </b>
<code>u64 reserved_0x320</code>
</li>
<li>
<b>Field added. </b>
<code>u8 reserved_0x380[16]</code>
</li>
<li>
<b>Field added. </b>
<code>u8 reserved_0x3f0[16]</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 reserved_1[2]</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 reserved_2[4]</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 reserved_3[104]</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 reserved_4[24]</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 reserved_5[32]</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 reserved_7[80]</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 reserved_8[20]</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 reserved_9</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 reserved_10</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 reserved_11[16]</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 reserved_12[16]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
