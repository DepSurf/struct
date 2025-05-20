# Struct: <code>kvm_vcpu_xen</code>

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
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kvm_vcpu_xen {
    u64 hypercall_rip;
    u32 current_runstate;
    bool vcpu_info_set;
    bool vcpu_time_info_set;
    bool runstate_set;
    struct gfn_to_hva_cache vcpu_info_cache;
    struct gfn_to_hva_cache vcpu_time_info_cache;
    struct gfn_to_hva_cache runstate_cache;
    u64 last_steal;
    u64 runstate_entry_time;
    u64 runstate_times[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kvm_vcpu_xen {
    u64 hypercall_rip;
    u32 current_runstate;
    bool vcpu_info_set;
    bool vcpu_time_info_set;
    bool runstate_set;
    struct gfn_to_hva_cache vcpu_info_cache;
    struct gfn_to_hva_cache vcpu_time_info_cache;
    struct gfn_to_hva_cache runstate_cache;
    u64 last_steal;
    u64 runstate_entry_time;
    u64 runstate_times[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kvm_vcpu_xen {
    u64 hypercall_rip;
    u32 current_runstate;
    u8 upcall_vector;
    struct gfn_to_pfn_cache vcpu_info_cache;
    struct gfn_to_pfn_cache vcpu_time_info_cache;
    struct gfn_to_pfn_cache runstate_cache;
    u64 last_steal;
    u64 runstate_entry_time;
    u64 runstate_times[4];
    long unsigned int evtchn_pending_sel;
    u32 vcpu_id;
    u32 timer_virq;
    u64 timer_expires;
    atomic_t timer_pending;
    struct hrtimer timer;
    int poll_evtchn;
    struct timer_list poll_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kvm_vcpu_xen {
    u64 hypercall_rip;
    u32 current_runstate;
    u8 upcall_vector;
    struct gfn_to_pfn_cache vcpu_info_cache;
    struct gfn_to_pfn_cache vcpu_time_info_cache;
    struct gfn_to_pfn_cache runstate_cache;
    struct gfn_to_pfn_cache runstate2_cache;
    u64 last_steal;
    u64 runstate_entry_time;
    u64 runstate_times[4];
    long unsigned int evtchn_pending_sel;
    u32 vcpu_id;
    u32 timer_virq;
    u64 timer_expires;
    atomic_t timer_pending;
    struct hrtimer timer;
    int poll_evtchn;
    struct timer_list poll_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kvm_vcpu_xen {
    u64 hypercall_rip;
    u32 current_runstate;
    u8 upcall_vector;
    struct gfn_to_pfn_cache vcpu_info_cache;
    struct gfn_to_pfn_cache vcpu_time_info_cache;
    struct gfn_to_pfn_cache runstate_cache;
    struct gfn_to_pfn_cache runstate2_cache;
    u64 last_steal;
    u64 runstate_entry_time;
    u64 runstate_times[4];
    long unsigned int evtchn_pending_sel;
    u32 vcpu_id;
    u32 timer_virq;
    u64 timer_expires;
    atomic_t timer_pending;
    struct hrtimer timer;
    int poll_evtchn;
    struct timer_list poll_timer;
    struct kvm_hypervisor_cpuid cpuid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kvm_vcpu_xen {
    u64 hypercall_rip;
    u32 current_runstate;
    u8 upcall_vector;
    struct gfn_to_pfn_cache vcpu_info_cache;
    struct gfn_to_pfn_cache vcpu_time_info_cache;
    struct gfn_to_pfn_cache runstate_cache;
    struct gfn_to_pfn_cache runstate2_cache;
    u64 last_steal;
    u64 runstate_entry_time;
    u64 runstate_times[4];
    long unsigned int evtchn_pending_sel;
    u32 vcpu_id;
    u32 timer_virq;
    u64 timer_expires;
    atomic_t timer_pending;
    struct hrtimer timer;
    int poll_evtchn;
    struct timer_list poll_timer;
    struct kvm_hypervisor_cpuid cpuid;
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
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 upcall_vector</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int evtchn_pending_sel</code>
</li>
<li>
<b>Field added. </b>
<code>u32 vcpu_id</code>
</li>
<li>
<b>Field added. </b>
<code>u32 timer_virq</code>
</li>
<li>
<b>Field added. </b>
<code>u64 timer_expires</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t timer_pending</code>
</li>
<li>
<b>Field added. </b>
<code>struct hrtimer timer</code>
</li>
<li>
<b>Field added. </b>
<code>int poll_evtchn</code>
</li>
<li>
<b>Field added. </b>
<code>struct timer_list poll_timer</code>
</li>
<li>
<b>Field removed. </b>
<code>bool vcpu_info_set</code>
</li>
<li>
<b>Field removed. </b>
<code>bool vcpu_time_info_set</code>
</li>
<li>
<b>Field removed. </b>
<code>bool runstate_set</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct gfn_to_hva_cache vcpu_info_cache</code> ➡️ <code>struct gfn_to_pfn_cache vcpu_info_cache</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct gfn_to_hva_cache vcpu_time_info_cache</code> ➡️ <code>struct gfn_to_pfn_cache vcpu_time_info_cache</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct gfn_to_hva_cache runstate_cache</code> ➡️ <code>struct gfn_to_pfn_cache runstate_cache</code>
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
<code>struct gfn_to_pfn_cache runstate2_cache</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct kvm_hypervisor_cpuid cpuid</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
