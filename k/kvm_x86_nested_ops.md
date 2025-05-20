# Struct: <code>kvm_x86_nested_ops</code>

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
struct kvm_x86_nested_ops {
    int (*check_events)(struct kvm_vcpu *);
    bool (*hv_timer_pending)(struct kvm_vcpu *);
    void (*triple_fault)(struct kvm_vcpu *);
    int (*get_state)(struct kvm_vcpu *, struct kvm_nested_state *, unsigned int);
    int (*set_state)(struct kvm_vcpu *, struct kvm_nested_state *, struct kvm_nested_state *);
    bool (*get_nested_state_pages)(struct kvm_vcpu *);
    int (*write_log_dirty)(struct kvm_vcpu *, gpa_t);
    int (*enable_evmcs)(struct kvm_vcpu *, uint16_t *);
    uint16_t (*get_evmcs_version)(struct kvm_vcpu *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kvm_x86_nested_ops {
    void (*leave_nested)(struct kvm_vcpu *);
    int (*check_events)(struct kvm_vcpu *);
    bool (*hv_timer_pending)(struct kvm_vcpu *);
    void (*triple_fault)(struct kvm_vcpu *);
    int (*get_state)(struct kvm_vcpu *, struct kvm_nested_state *, unsigned int);
    int (*set_state)(struct kvm_vcpu *, struct kvm_nested_state *, struct kvm_nested_state *);
    bool (*get_nested_state_pages)(struct kvm_vcpu *);
    int (*write_log_dirty)(struct kvm_vcpu *, gpa_t);
    int (*enable_evmcs)(struct kvm_vcpu *, uint16_t *);
    uint16_t (*get_evmcs_version)(struct kvm_vcpu *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kvm_x86_nested_ops {
    void (*leave_nested)(struct kvm_vcpu *);
    int (*check_events)(struct kvm_vcpu *);
    bool (*handle_page_fault_workaround)(struct kvm_vcpu *, struct x86_exception *);
    bool (*hv_timer_pending)(struct kvm_vcpu *);
    void (*triple_fault)(struct kvm_vcpu *);
    int (*get_state)(struct kvm_vcpu *, struct kvm_nested_state *, unsigned int);
    int (*set_state)(struct kvm_vcpu *, struct kvm_nested_state *, struct kvm_nested_state *);
    bool (*get_nested_state_pages)(struct kvm_vcpu *);
    int (*write_log_dirty)(struct kvm_vcpu *, gpa_t);
    int (*enable_evmcs)(struct kvm_vcpu *, uint16_t *);
    uint16_t (*get_evmcs_version)(struct kvm_vcpu *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kvm_x86_nested_ops {
    void (*leave_nested)(struct kvm_vcpu *);
    bool (*is_exception_vmexit)(struct kvm_vcpu *, u8, u32);
    int (*check_events)(struct kvm_vcpu *);
    bool (*has_events)(struct kvm_vcpu *);
    void (*triple_fault)(struct kvm_vcpu *);
    int (*get_state)(struct kvm_vcpu *, struct kvm_nested_state *, unsigned int);
    int (*set_state)(struct kvm_vcpu *, struct kvm_nested_state *, struct kvm_nested_state *);
    bool (*get_nested_state_pages)(struct kvm_vcpu *);
    int (*write_log_dirty)(struct kvm_vcpu *, gpa_t);
    int (*enable_evmcs)(struct kvm_vcpu *, uint16_t *);
    uint16_t (*get_evmcs_version)(struct kvm_vcpu *);
    void (*hv_inject_synthetic_vmexit_post_tlb_flush)(struct kvm_vcpu *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kvm_x86_nested_ops {
    void (*leave_nested)(struct kvm_vcpu *);
    bool (*is_exception_vmexit)(struct kvm_vcpu *, u8, u32);
    int (*check_events)(struct kvm_vcpu *);
    bool (*has_events)(struct kvm_vcpu *);
    void (*triple_fault)(struct kvm_vcpu *);
    int (*get_state)(struct kvm_vcpu *, struct kvm_nested_state *, unsigned int);
    int (*set_state)(struct kvm_vcpu *, struct kvm_nested_state *, struct kvm_nested_state *);
    bool (*get_nested_state_pages)(struct kvm_vcpu *);
    int (*write_log_dirty)(struct kvm_vcpu *, gpa_t);
    int (*enable_evmcs)(struct kvm_vcpu *, uint16_t *);
    uint16_t (*get_evmcs_version)(struct kvm_vcpu *);
    void (*hv_inject_synthetic_vmexit_post_tlb_flush)(struct kvm_vcpu *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kvm_x86_nested_ops {
    void (*leave_nested)(struct kvm_vcpu *);
    bool (*is_exception_vmexit)(struct kvm_vcpu *, u8, u32);
    int (*check_events)(struct kvm_vcpu *);
    bool (*has_events)(struct kvm_vcpu *);
    void (*triple_fault)(struct kvm_vcpu *);
    int (*get_state)(struct kvm_vcpu *, struct kvm_nested_state *, unsigned int);
    int (*set_state)(struct kvm_vcpu *, struct kvm_nested_state *, struct kvm_nested_state *);
    bool (*get_nested_state_pages)(struct kvm_vcpu *);
    int (*write_log_dirty)(struct kvm_vcpu *, gpa_t);
    int (*enable_evmcs)(struct kvm_vcpu *, uint16_t *);
    uint16_t (*get_evmcs_version)(struct kvm_vcpu *);
    void (*hv_inject_synthetic_vmexit_post_tlb_flush)(struct kvm_vcpu *);
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
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*leave_nested)(struct kvm_vcpu *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool (*handle_page_fault_workaround)(struct kvm_vcpu *, struct x86_exception *)</code>
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
<code>bool (*is_exception_vmexit)(struct kvm_vcpu *, u8, u32)</code>
</li>
<li>
<b>Field added. </b>
<code>bool (*has_events)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*hv_inject_synthetic_vmexit_post_tlb_flush)(struct kvm_vcpu *)</code>
</li>
<li>
<b>Field removed. </b>
<code>bool (*handle_page_fault_workaround)(struct kvm_vcpu *, struct x86_exception *)</code>
</li>
<li>
<b>Field removed. </b>
<code>bool (*hv_timer_pending)(struct kvm_vcpu *)</code>
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
