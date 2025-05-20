# Struct: <code>kvm_vcpu_hv</code>

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
struct kvm_vcpu_hv {
    u32 vp_index;
    u64 hv_vapic;
    s64 runtime_offset;
    struct kvm_vcpu_hv_synic synic;
    struct kvm_hyperv_exit exit;
    struct kvm_vcpu_hv_stimer stimer[4];
    long unsigned int stimer_pending_bitmap[1];
    cpumask_t tlb_flush;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kvm_vcpu_hv {
    struct kvm_vcpu *vcpu;
    u32 vp_index;
    u64 hv_vapic;
    s64 runtime_offset;
    struct kvm_vcpu_hv_synic synic;
    struct kvm_hyperv_exit exit;
    struct kvm_vcpu_hv_stimer stimer[4];
    long unsigned int stimer_pending_bitmap[1];
    cpumask_t tlb_flush;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kvm_vcpu_hv {
    struct kvm_vcpu *vcpu;
    u32 vp_index;
    u64 hv_vapic;
    s64 runtime_offset;
    struct kvm_vcpu_hv_synic synic;
    struct kvm_hyperv_exit exit;
    struct kvm_vcpu_hv_stimer stimer[4];
    long unsigned int stimer_pending_bitmap[1];
    cpumask_t tlb_flush;
    bool enforce_cpuid;
    struct (anon) cpuid_cache;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kvm_vcpu_hv {
    struct kvm_vcpu *vcpu;
    u32 vp_index;
    u64 hv_vapic;
    s64 runtime_offset;
    struct kvm_vcpu_hv_synic synic;
    struct kvm_hyperv_exit exit;
    struct kvm_vcpu_hv_stimer stimer[4];
    long unsigned int stimer_pending_bitmap[1];
    bool enforce_cpuid;
    struct (anon) cpuid_cache;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kvm_vcpu_hv {
    struct kvm_vcpu *vcpu;
    u32 vp_index;
    u64 hv_vapic;
    s64 runtime_offset;
    struct kvm_vcpu_hv_synic synic;
    struct kvm_hyperv_exit exit;
    struct kvm_vcpu_hv_stimer stimer[4];
    long unsigned int stimer_pending_bitmap[1];
    bool enforce_cpuid;
    struct (anon) cpuid_cache;
    struct kvm_vcpu_hv_tlb_flush_fifo tlb_flush_fifo[2];
    u64 sparse_banks[64];
    struct hv_vp_assist_page vp_assist_page;
    struct (anon) nested;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kvm_vcpu_hv {
    struct kvm_vcpu *vcpu;
    u32 vp_index;
    u64 hv_vapic;
    s64 runtime_offset;
    struct kvm_vcpu_hv_synic synic;
    struct kvm_hyperv_exit exit;
    struct kvm_vcpu_hv_stimer stimer[4];
    long unsigned int stimer_pending_bitmap[1];
    bool enforce_cpuid;
    struct (anon) cpuid_cache;
    struct kvm_vcpu_hv_tlb_flush_fifo tlb_flush_fifo[2];
    u64 sparse_banks[64];
    struct hv_vp_assist_page vp_assist_page;
    struct (anon) nested;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kvm_vcpu_hv {
    struct kvm_vcpu *vcpu;
    u32 vp_index;
    u64 hv_vapic;
    s64 runtime_offset;
    struct kvm_vcpu_hv_synic synic;
    struct kvm_hyperv_exit exit;
    struct kvm_vcpu_hv_stimer stimer[4];
    long unsigned int stimer_pending_bitmap[1];
    bool enforce_cpuid;
    struct (anon) cpuid_cache;
    struct kvm_vcpu_hv_tlb_flush_fifo tlb_flush_fifo[2];
    u64 sparse_banks[64];
    struct hv_vp_assist_page vp_assist_page;
    struct (anon) nested;
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
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct kvm_vcpu *vcpu</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool enforce_cpuid</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) cpuid_cache</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>cpumask_t tlb_flush</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct kvm_vcpu_hv_tlb_flush_fifo tlb_flush_fifo[2]</code>
</li>
<li>
<b>Field added. </b>
<code>u64 sparse_banks[64]</code>
</li>
<li>
<b>Field added. </b>
<code>struct hv_vp_assist_page vp_assist_page</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) nested</code>
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
