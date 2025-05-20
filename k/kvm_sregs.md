# Struct: <code>kvm_sregs</code>

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
struct kvm_sregs {
    struct kvm_segment cs;
    struct kvm_segment ds;
    struct kvm_segment es;
    struct kvm_segment fs;
    struct kvm_segment gs;
    struct kvm_segment ss;
    struct kvm_segment tr;
    struct kvm_segment ldt;
    struct kvm_dtable gdt;
    struct kvm_dtable idt;
    __u64 cr0;
    __u64 cr2;
    __u64 cr3;
    __u64 cr4;
    __u64 cr8;
    __u64 efer;
    __u64 apic_base;
    __u64 interrupt_bitmap[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kvm_sregs {
    struct kvm_segment cs;
    struct kvm_segment ds;
    struct kvm_segment es;
    struct kvm_segment fs;
    struct kvm_segment gs;
    struct kvm_segment ss;
    struct kvm_segment tr;
    struct kvm_segment ldt;
    struct kvm_dtable gdt;
    struct kvm_dtable idt;
    __u64 cr0;
    __u64 cr2;
    __u64 cr3;
    __u64 cr4;
    __u64 cr8;
    __u64 efer;
    __u64 apic_base;
    __u64 interrupt_bitmap[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kvm_sregs {
    struct kvm_segment cs;
    struct kvm_segment ds;
    struct kvm_segment es;
    struct kvm_segment fs;
    struct kvm_segment gs;
    struct kvm_segment ss;
    struct kvm_segment tr;
    struct kvm_segment ldt;
    struct kvm_dtable gdt;
    struct kvm_dtable idt;
    __u64 cr0;
    __u64 cr2;
    __u64 cr3;
    __u64 cr4;
    __u64 cr8;
    __u64 efer;
    __u64 apic_base;
    __u64 interrupt_bitmap[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kvm_sregs {
    struct kvm_segment cs;
    struct kvm_segment ds;
    struct kvm_segment es;
    struct kvm_segment fs;
    struct kvm_segment gs;
    struct kvm_segment ss;
    struct kvm_segment tr;
    struct kvm_segment ldt;
    struct kvm_dtable gdt;
    struct kvm_dtable idt;
    __u64 cr0;
    __u64 cr2;
    __u64 cr3;
    __u64 cr4;
    __u64 cr8;
    __u64 efer;
    __u64 apic_base;
    __u64 interrupt_bitmap[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kvm_sregs {
    struct kvm_segment cs;
    struct kvm_segment ds;
    struct kvm_segment es;
    struct kvm_segment fs;
    struct kvm_segment gs;
    struct kvm_segment ss;
    struct kvm_segment tr;
    struct kvm_segment ldt;
    struct kvm_dtable gdt;
    struct kvm_dtable idt;
    __u64 cr0;
    __u64 cr2;
    __u64 cr3;
    __u64 cr4;
    __u64 cr8;
    __u64 efer;
    __u64 apic_base;
    __u64 interrupt_bitmap[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kvm_sregs {
    struct kvm_segment cs;
    struct kvm_segment ds;
    struct kvm_segment es;
    struct kvm_segment fs;
    struct kvm_segment gs;
    struct kvm_segment ss;
    struct kvm_segment tr;
    struct kvm_segment ldt;
    struct kvm_dtable gdt;
    struct kvm_dtable idt;
    __u64 cr0;
    __u64 cr2;
    __u64 cr3;
    __u64 cr4;
    __u64 cr8;
    __u64 efer;
    __u64 apic_base;
    __u64 interrupt_bitmap[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kvm_sregs {
    struct kvm_segment cs;
    struct kvm_segment ds;
    struct kvm_segment es;
    struct kvm_segment fs;
    struct kvm_segment gs;
    struct kvm_segment ss;
    struct kvm_segment tr;
    struct kvm_segment ldt;
    struct kvm_dtable gdt;
    struct kvm_dtable idt;
    __u64 cr0;
    __u64 cr2;
    __u64 cr3;
    __u64 cr4;
    __u64 cr8;
    __u64 efer;
    __u64 apic_base;
    __u64 interrupt_bitmap[4];
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
struct kvm_sregs {
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
struct kvm_sregs {
    __u32 pvr;
    union (anon) u;
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
