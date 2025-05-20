# Struct: <code>kvm_pmu</code>

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
struct kvm_pmu {
    unsigned int nr_arch_gp_counters;
    unsigned int nr_arch_fixed_counters;
    unsigned int available_event_types;
    u64 fixed_ctr_ctrl;
    u64 global_ctrl;
    u64 global_status;
    u64 global_ovf_ctrl;
    u64 counter_bitmask[2];
    u64 global_ctrl_mask;
    u64 global_ovf_ctrl_mask;
    u64 reserved_bits;
    u8 version;
    struct kvm_pmc gp_counters[32];
    struct kvm_pmc fixed_counters[4];
    struct irq_work irq_work;
    long unsigned int reprogram_pmi[1];
    long unsigned int all_valid_pmc_idx[1];
    long unsigned int pmc_in_use[1];
    bool need_cleanup;
    u8 event_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kvm_pmu {
    unsigned int nr_arch_gp_counters;
    unsigned int nr_arch_fixed_counters;
    unsigned int available_event_types;
    u64 fixed_ctr_ctrl;
    u64 global_ctrl;
    u64 global_status;
    u64 global_ovf_ctrl;
    u64 counter_bitmask[2];
    u64 global_ctrl_mask;
    u64 global_ovf_ctrl_mask;
    u64 reserved_bits;
    u8 version;
    struct kvm_pmc gp_counters[32];
    struct kvm_pmc fixed_counters[4];
    struct irq_work irq_work;
    long unsigned int reprogram_pmi[1];
    long unsigned int all_valid_pmc_idx[1];
    long unsigned int pmc_in_use[1];
    bool need_cleanup;
    u8 event_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kvm_pmu {
    unsigned int nr_arch_gp_counters;
    unsigned int nr_arch_fixed_counters;
    unsigned int available_event_types;
    u64 fixed_ctr_ctrl;
    u64 global_ctrl;
    u64 global_status;
    u64 global_ovf_ctrl;
    u64 counter_bitmask[2];
    u64 global_ctrl_mask;
    u64 global_ovf_ctrl_mask;
    u64 reserved_bits;
    u8 version;
    struct kvm_pmc gp_counters[32];
    struct kvm_pmc fixed_counters[4];
    struct irq_work irq_work;
    long unsigned int reprogram_pmi[1];
    long unsigned int all_valid_pmc_idx[1];
    long unsigned int pmc_in_use[1];
    bool need_cleanup;
    u8 event_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kvm_pmu {
    unsigned int nr_arch_gp_counters;
    unsigned int nr_arch_fixed_counters;
    unsigned int available_event_types;
    u64 fixed_ctr_ctrl;
    u64 fixed_ctr_ctrl_mask;
    u64 global_ctrl;
    u64 global_status;
    u64 counter_bitmask[2];
    u64 global_ctrl_mask;
    u64 global_ovf_ctrl_mask;
    u64 reserved_bits;
    u64 raw_event_mask;
    u8 version;
    struct kvm_pmc gp_counters[32];
    struct kvm_pmc fixed_counters[3];
    struct irq_work irq_work;
    long unsigned int reprogram_pmi[1];
    long unsigned int all_valid_pmc_idx[1];
    long unsigned int pmc_in_use[1];
    bool need_cleanup;
    u8 event_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kvm_pmu {
    unsigned int nr_arch_gp_counters;
    unsigned int nr_arch_fixed_counters;
    unsigned int available_event_types;
    u64 fixed_ctr_ctrl;
    u64 fixed_ctr_ctrl_mask;
    u64 global_ctrl;
    u64 global_status;
    u64 counter_bitmask[2];
    u64 global_ctrl_mask;
    u64 global_ovf_ctrl_mask;
    u64 reserved_bits;
    u64 raw_event_mask;
    u8 version;
    struct kvm_pmc gp_counters[8];
    struct kvm_pmc fixed_counters[3];
    struct irq_work irq_work;
    long unsigned int reprogram_pmi[1];
    atomic64_t __reprogram_pmi;
    long unsigned int all_valid_pmc_idx[1];
    long unsigned int pmc_in_use[1];
    u64 ds_area;
    u64 pebs_enable;
    u64 pebs_enable_mask;
    u64 pebs_data_cfg;
    u64 pebs_data_cfg_mask;
    u64 host_cross_mapped_mask;
    bool need_cleanup;
    u8 event_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kvm_pmu {
    u8 version;
    unsigned int nr_arch_gp_counters;
    unsigned int nr_arch_fixed_counters;
    unsigned int available_event_types;
    u64 fixed_ctr_ctrl;
    u64 fixed_ctr_ctrl_mask;
    u64 global_ctrl;
    u64 global_status;
    u64 counter_bitmask[2];
    u64 global_ctrl_mask;
    u64 global_status_mask;
    u64 reserved_bits;
    u64 raw_event_mask;
    struct kvm_pmc gp_counters[8];
    struct kvm_pmc fixed_counters[3];
    struct irq_work irq_work;
    long unsigned int reprogram_pmi[1];
    atomic64_t __reprogram_pmi;
    long unsigned int all_valid_pmc_idx[1];
    long unsigned int pmc_in_use[1];
    u64 ds_area;
    u64 pebs_enable;
    u64 pebs_enable_mask;
    u64 pebs_data_cfg;
    u64 pebs_data_cfg_mask;
    u64 host_cross_mapped_mask;
    bool need_cleanup;
    u8 event_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kvm_pmu {
    u8 version;
    unsigned int nr_arch_gp_counters;
    unsigned int nr_arch_fixed_counters;
    unsigned int available_event_types;
    u64 fixed_ctr_ctrl;
    u64 fixed_ctr_ctrl_mask;
    u64 global_ctrl;
    u64 global_status;
    u64 counter_bitmask[2];
    u64 global_ctrl_mask;
    u64 global_status_mask;
    u64 reserved_bits;
    u64 raw_event_mask;
    struct kvm_pmc gp_counters[8];
    struct kvm_pmc fixed_counters[3];
    long unsigned int reprogram_pmi[1];
    atomic64_t __reprogram_pmi;
    long unsigned int all_valid_pmc_idx[1];
    long unsigned int pmc_in_use[1];
    u64 ds_area;
    u64 pebs_enable;
    u64 pebs_enable_mask;
    u64 pebs_data_cfg;
    u64 pebs_data_cfg_mask;
    u64 host_cross_mapped_mask;
    bool need_cleanup;
    u8 event_count;
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
struct kvm_pmu {
    int irq_num;
    struct kvm_pmc pmc[32];
    long unsigned int chained[1];
    bool ready;
    bool created;
    bool irq_level;
};
```
</details>
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
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 fixed_ctr_ctrl_mask</code>
</li>
<li>
<b>Field added. </b>
<code>u64 raw_event_mask</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 global_ovf_ctrl</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct kvm_pmc fixed_counters[4]</code> ➡️ <code>struct kvm_pmc fixed_counters[3]</code>
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
<code>atomic64_t __reprogram_pmi</code>
</li>
<li>
<b>Field added. </b>
<code>u64 ds_area</code>
</li>
<li>
<b>Field added. </b>
<code>u64 pebs_enable</code>
</li>
<li>
<b>Field added. </b>
<code>u64 pebs_enable_mask</code>
</li>
<li>
<b>Field added. </b>
<code>u64 pebs_data_cfg</code>
</li>
<li>
<b>Field added. </b>
<code>u64 pebs_data_cfg_mask</code>
</li>
<li>
<b>Field added. </b>
<code>u64 host_cross_mapped_mask</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct kvm_pmc gp_counters[32]</code> ➡️ <code>struct kvm_pmc gp_counters[8]</code>
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
<code>u64 global_status_mask</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 global_ovf_ctrl_mask</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct irq_work irq_work</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Arch</b>
<ul>
</ul>
