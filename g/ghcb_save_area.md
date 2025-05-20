# Struct: <code>ghcb_save_area</code>

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
struct ghcb_save_area {
    u8 reserved_1[203];
    u8 cpl;
    u8 reserved_2[116];
    u64 xss;
    u8 reserved_3[24];
    u64 dr7;
    u8 reserved_4[16];
    u64 rip;
    u8 reserved_5[88];
    u64 rsp;
    u8 reserved_6[24];
    u64 rax;
    u8 reserved_7[264];
    u64 rcx;
    u64 rdx;
    u64 rbx;
    u8 reserved_8[8];
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
    u8 reserved_9[16];
    u64 sw_exit_code;
    u64 sw_exit_info_1;
    u64 sw_exit_info_2;
    u64 sw_scratch;
    u8 reserved_10[56];
    u64 xcr0;
    u8 valid_bitmap[16];
    u64 x87_state_gpa;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ghcb_save_area {
    u8 reserved_0x0[203];
    u8 cpl;
    u8 reserved_0xcc[116];
    u64 xss;
    u8 reserved_0x148[24];
    u64 dr7;
    u8 reserved_0x168[16];
    u64 rip;
    u8 reserved_0x180[88];
    u64 rsp;
    u8 reserved_0x1e0[24];
    u64 rax;
    u8 reserved_0x200[264];
    u64 rcx;
    u64 rdx;
    u64 rbx;
    u8 reserved_0x320[8];
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
    u64 sw_exit_code;
    u64 sw_exit_info_1;
    u64 sw_exit_info_2;
    u64 sw_scratch;
    u8 reserved_0x3b0[56];
    u64 xcr0;
    u8 valid_bitmap[16];
    u64 x87_state_gpa;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ghcb_save_area {
    u8 reserved_0x0[203];
    u8 cpl;
    u8 reserved_0xcc[116];
    u64 xss;
    u8 reserved_0x148[24];
    u64 dr7;
    u8 reserved_0x168[16];
    u64 rip;
    u8 reserved_0x180[88];
    u64 rsp;
    u8 reserved_0x1e0[24];
    u64 rax;
    u8 reserved_0x200[264];
    u64 rcx;
    u64 rdx;
    u64 rbx;
    u8 reserved_0x320[8];
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
    u64 sw_exit_code;
    u64 sw_exit_info_1;
    u64 sw_exit_info_2;
    u64 sw_scratch;
    u8 reserved_0x3b0[56];
    u64 xcr0;
    u8 valid_bitmap[16];
    u64 x87_state_gpa;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ghcb_save_area {
    u8 reserved_0x0[203];
    u8 cpl;
    u8 reserved_0xcc[116];
    u64 xss;
    u8 reserved_0x148[24];
    u64 dr7;
    u8 reserved_0x168[16];
    u64 rip;
    u8 reserved_0x180[88];
    u64 rsp;
    u8 reserved_0x1e0[24];
    u64 rax;
    u8 reserved_0x200[264];
    u64 rcx;
    u64 rdx;
    u64 rbx;
    u8 reserved_0x320[8];
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
    u64 sw_exit_code;
    u64 sw_exit_info_1;
    u64 sw_exit_info_2;
    u64 sw_scratch;
    u8 reserved_0x3b0[56];
    u64 xcr0;
    u8 valid_bitmap[16];
    u64 x87_state_gpa;
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
<code>u8 reserved_0x0[203]</code>
</li>
<li>
<b>Field added. </b>
<code>u8 reserved_0xcc[116]</code>
</li>
<li>
<b>Field added. </b>
<code>u8 reserved_0x148[24]</code>
</li>
<li>
<b>Field added. </b>
<code>u8 reserved_0x168[16]</code>
</li>
<li>
<b>Field added. </b>
<code>u8 reserved_0x180[88]</code>
</li>
<li>
<b>Field added. </b>
<code>u8 reserved_0x1e0[24]</code>
</li>
<li>
<b>Field added. </b>
<code>u8 reserved_0x200[264]</code>
</li>
<li>
<b>Field added. </b>
<code>u8 reserved_0x320[8]</code>
</li>
<li>
<b>Field added. </b>
<code>u8 reserved_0x380[16]</code>
</li>
<li>
<b>Field added. </b>
<code>u8 reserved_0x3b0[56]</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 reserved_1[203]</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 reserved_2[116]</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 reserved_3[24]</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 reserved_4[16]</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 reserved_5[88]</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 reserved_6[24]</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 reserved_7[264]</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 reserved_8[8]</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 reserved_9[16]</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 reserved_10[56]</code>
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
