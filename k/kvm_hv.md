# Struct: <code>kvm_hv</code>

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
struct kvm_hv {
    struct mutex hv_lock;
    u64 hv_guest_os_id;
    u64 hv_hypercall;
    u64 hv_tsc_page;
    u64 hv_crash_param[5];
    u64 hv_crash_ctl;
    struct ms_hyperv_tsc_page tsc_ref;
    struct idr conn_to_evt;
    u64 hv_reenlightenment_control;
    u64 hv_tsc_emulation_control;
    u64 hv_tsc_emulation_status;
    atomic_t num_mismatched_vp_indexes;
    struct hv_partition_assist_pg *hv_pa_pg;
    struct kvm_hv_syndbg hv_syndbg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kvm_hv {
    struct mutex hv_lock;
    u64 hv_guest_os_id;
    u64 hv_hypercall;
    u64 hv_tsc_page;
    enum hv_tsc_page_status hv_tsc_page_status;
    u64 hv_crash_param[5];
    u64 hv_crash_ctl;
    struct ms_hyperv_tsc_page tsc_ref;
    struct idr conn_to_evt;
    u64 hv_reenlightenment_control;
    u64 hv_tsc_emulation_control;
    u64 hv_tsc_emulation_status;
    atomic_t num_mismatched_vp_indexes;
    struct hv_partition_assist_pg *hv_pa_pg;
    struct kvm_hv_syndbg hv_syndbg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kvm_hv {
    struct mutex hv_lock;
    u64 hv_guest_os_id;
    u64 hv_hypercall;
    u64 hv_tsc_page;
    enum hv_tsc_page_status hv_tsc_page_status;
    u64 hv_crash_param[5];
    u64 hv_crash_ctl;
    struct ms_hyperv_tsc_page tsc_ref;
    struct idr conn_to_evt;
    u64 hv_reenlightenment_control;
    u64 hv_tsc_emulation_control;
    u64 hv_tsc_emulation_status;
    atomic_t num_mismatched_vp_indexes;
    unsigned int synic_auto_eoi_used;
    struct hv_partition_assist_pg *hv_pa_pg;
    struct kvm_hv_syndbg hv_syndbg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kvm_hv {
    struct mutex hv_lock;
    u64 hv_guest_os_id;
    u64 hv_hypercall;
    u64 hv_tsc_page;
    enum hv_tsc_page_status hv_tsc_page_status;
    u64 hv_crash_param[5];
    u64 hv_crash_ctl;
    struct ms_hyperv_tsc_page tsc_ref;
    struct idr conn_to_evt;
    u64 hv_reenlightenment_control;
    u64 hv_tsc_emulation_control;
    u64 hv_tsc_emulation_status;
    atomic_t num_mismatched_vp_indexes;
    unsigned int synic_auto_eoi_used;
    struct hv_partition_assist_pg *hv_pa_pg;
    struct kvm_hv_syndbg hv_syndbg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kvm_hv {
    struct mutex hv_lock;
    u64 hv_guest_os_id;
    u64 hv_hypercall;
    u64 hv_tsc_page;
    enum hv_tsc_page_status hv_tsc_page_status;
    u64 hv_crash_param[5];
    u64 hv_crash_ctl;
    struct ms_hyperv_tsc_page tsc_ref;
    struct idr conn_to_evt;
    u64 hv_reenlightenment_control;
    u64 hv_tsc_emulation_control;
    u64 hv_tsc_emulation_status;
    atomic_t num_mismatched_vp_indexes;
    unsigned int synic_auto_eoi_used;
    struct hv_partition_assist_pg *hv_pa_pg;
    struct kvm_hv_syndbg hv_syndbg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kvm_hv {
    struct mutex hv_lock;
    u64 hv_guest_os_id;
    u64 hv_hypercall;
    u64 hv_tsc_page;
    enum hv_tsc_page_status hv_tsc_page_status;
    u64 hv_crash_param[5];
    u64 hv_crash_ctl;
    struct ms_hyperv_tsc_page tsc_ref;
    struct idr conn_to_evt;
    u64 hv_reenlightenment_control;
    u64 hv_tsc_emulation_control;
    u64 hv_tsc_emulation_status;
    u64 hv_invtsc_control;
    atomic_t num_mismatched_vp_indexes;
    unsigned int synic_auto_eoi_used;
    struct hv_partition_assist_pg *hv_pa_pg;
    struct kvm_hv_syndbg hv_syndbg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kvm_hv {
    struct mutex hv_lock;
    u64 hv_guest_os_id;
    u64 hv_hypercall;
    u64 hv_tsc_page;
    enum hv_tsc_page_status hv_tsc_page_status;
    u64 hv_crash_param[5];
    u64 hv_crash_ctl;
    struct ms_hyperv_tsc_page tsc_ref;
    struct idr conn_to_evt;
    u64 hv_reenlightenment_control;
    u64 hv_tsc_emulation_control;
    u64 hv_tsc_emulation_status;
    u64 hv_invtsc_control;
    atomic_t num_mismatched_vp_indexes;
    unsigned int synic_auto_eoi_used;
    struct kvm_hv_syndbg hv_syndbg;
    bool xsaves_xsavec_checked;
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
<code>enum hv_tsc_page_status hv_tsc_page_status</code>
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
<code>unsigned int synic_auto_eoi_used</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 hv_invtsc_control</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool xsaves_xsavec_checked</code>
</li>
<li>
<b>Field removed. </b>
<code>struct hv_partition_assist_pg *hv_pa_pg</code>
</li>
</ul>
</details>
</li>
</ul>
