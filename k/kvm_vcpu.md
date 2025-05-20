# Struct: <code>kvm_vcpu</code>

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
struct kvm_vcpu {
    struct kvm *kvm;
    struct preempt_notifier preempt_notifier;
    int cpu;
    int vcpu_id;
    int vcpu_idx;
    int srcu_idx;
    int mode;
    u64 requests;
    long unsigned int guest_debug;
    int pre_pcpu;
    struct list_head blocked_vcpu_list;
    struct mutex mutex;
    struct kvm_run *run;
    struct rcuwait wait;
    struct pid *pid;
    int sigset_active;
    sigset_t sigset;
    struct kvm_vcpu_stat stat;
    unsigned int halt_poll_ns;
    bool valid_wakeup;
    int mmio_needed;
    int mmio_read_completed;
    int mmio_is_write;
    int mmio_cur_fragment;
    int mmio_nr_fragments;
    struct kvm_mmio_fragment mmio_fragments[2];
    struct (anon) async_pf;
    struct (anon) spin_loop;
    bool preempted;
    bool ready;
    struct kvm_vcpu_arch arch;
    struct kvm_dirty_ring dirty_ring;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kvm_vcpu {
    struct kvm *kvm;
    struct preempt_notifier preempt_notifier;
    int cpu;
    int vcpu_id;
    int vcpu_idx;
    int srcu_idx;
    int mode;
    u64 requests;
    long unsigned int guest_debug;
    int pre_pcpu;
    struct list_head blocked_vcpu_list;
    struct mutex mutex;
    struct kvm_run *run;
    struct rcuwait wait;
    struct pid *pid;
    int sigset_active;
    sigset_t sigset;
    struct kvm_vcpu_stat stat;
    unsigned int halt_poll_ns;
    bool valid_wakeup;
    int mmio_needed;
    int mmio_read_completed;
    int mmio_is_write;
    int mmio_cur_fragment;
    int mmio_nr_fragments;
    struct kvm_mmio_fragment mmio_fragments[2];
    struct (anon) async_pf;
    struct (anon) spin_loop;
    bool preempted;
    bool ready;
    struct kvm_vcpu_arch arch;
    struct kvm_dirty_ring dirty_ring;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kvm_vcpu {
    struct kvm *kvm;
    struct preempt_notifier preempt_notifier;
    int cpu;
    int vcpu_id;
    int vcpu_idx;
    int srcu_idx;
    int mode;
    u64 requests;
    long unsigned int guest_debug;
    int pre_pcpu;
    struct list_head blocked_vcpu_list;
    struct mutex mutex;
    struct kvm_run *run;
    struct rcuwait wait;
    struct pid *pid;
    int sigset_active;
    sigset_t sigset;
    unsigned int halt_poll_ns;
    bool valid_wakeup;
    int mmio_needed;
    int mmio_read_completed;
    int mmio_is_write;
    int mmio_cur_fragment;
    int mmio_nr_fragments;
    struct kvm_mmio_fragment mmio_fragments[2];
    struct (anon) async_pf;
    struct (anon) spin_loop;
    bool preempted;
    bool ready;
    struct kvm_vcpu_arch arch;
    struct kvm_vcpu_stat stat;
    char stats_id[48];
    struct kvm_dirty_ring dirty_ring;
    int last_used_slot;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kvm_vcpu {
    struct kvm *kvm;
    struct preempt_notifier preempt_notifier;
    int cpu;
    int vcpu_id;
    int vcpu_idx;
    int ____srcu_idx;
    int mode;
    u64 requests;
    long unsigned int guest_debug;
    struct mutex mutex;
    struct kvm_run *run;
    struct rcuwait wait;
    struct pid *pid;
    int sigset_active;
    sigset_t sigset;
    unsigned int halt_poll_ns;
    bool valid_wakeup;
    int mmio_needed;
    int mmio_read_completed;
    int mmio_is_write;
    int mmio_cur_fragment;
    int mmio_nr_fragments;
    struct kvm_mmio_fragment mmio_fragments[2];
    struct (anon) async_pf;
    struct (anon) spin_loop;
    bool preempted;
    bool ready;
    struct kvm_vcpu_arch arch;
    struct kvm_vcpu_stat stat;
    char stats_id[48];
    struct kvm_dirty_ring dirty_ring;
    struct kvm_memory_slot *last_used_slot;
    u64 last_used_slot_gen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kvm_vcpu {
    struct kvm *kvm;
    struct preempt_notifier preempt_notifier;
    int cpu;
    int vcpu_id;
    int vcpu_idx;
    int ____srcu_idx;
    int mode;
    u64 requests;
    long unsigned int guest_debug;
    struct mutex mutex;
    struct kvm_run *run;
    struct rcuwait wait;
    struct pid *pid;
    int sigset_active;
    sigset_t sigset;
    unsigned int halt_poll_ns;
    bool valid_wakeup;
    int mmio_needed;
    int mmio_read_completed;
    int mmio_is_write;
    int mmio_cur_fragment;
    int mmio_nr_fragments;
    struct kvm_mmio_fragment mmio_fragments[2];
    struct (anon) async_pf;
    struct (anon) spin_loop;
    bool preempted;
    bool ready;
    struct kvm_vcpu_arch arch;
    struct kvm_vcpu_stat stat;
    char stats_id[48];
    struct kvm_dirty_ring dirty_ring;
    struct kvm_memory_slot *last_used_slot;
    u64 last_used_slot_gen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kvm_vcpu {
    struct kvm *kvm;
    struct preempt_notifier preempt_notifier;
    int cpu;
    int vcpu_id;
    int vcpu_idx;
    int ____srcu_idx;
    int mode;
    u64 requests;
    long unsigned int guest_debug;
    struct mutex mutex;
    struct kvm_run *run;
    struct rcuwait wait;
    struct pid *pid;
    int sigset_active;
    sigset_t sigset;
    unsigned int halt_poll_ns;
    bool valid_wakeup;
    int mmio_needed;
    int mmio_read_completed;
    int mmio_is_write;
    int mmio_cur_fragment;
    int mmio_nr_fragments;
    struct kvm_mmio_fragment mmio_fragments[2];
    struct (anon) async_pf;
    struct (anon) spin_loop;
    bool preempted;
    bool ready;
    struct kvm_vcpu_arch arch;
    struct kvm_vcpu_stat stat;
    char stats_id[48];
    struct kvm_dirty_ring dirty_ring;
    struct kvm_memory_slot *last_used_slot;
    u64 last_used_slot_gen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kvm_vcpu {
    struct kvm *kvm;
    struct preempt_notifier preempt_notifier;
    int cpu;
    int vcpu_id;
    int vcpu_idx;
    int ____srcu_idx;
    int mode;
    u64 requests;
    long unsigned int guest_debug;
    struct mutex mutex;
    struct kvm_run *run;
    struct rcuwait wait;
    struct pid *pid;
    int sigset_active;
    sigset_t sigset;
    unsigned int halt_poll_ns;
    bool valid_wakeup;
    int mmio_needed;
    int mmio_read_completed;
    int mmio_is_write;
    int mmio_cur_fragment;
    int mmio_nr_fragments;
    struct kvm_mmio_fragment mmio_fragments[2];
    struct (anon) async_pf;
    struct (anon) spin_loop;
    bool preempted;
    bool ready;
    struct kvm_vcpu_arch arch;
    struct kvm_vcpu_stat stat;
    char stats_id[48];
    struct kvm_dirty_ring dirty_ring;
    struct kvm_memory_slot *last_used_slot;
    u64 last_used_slot_gen;
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
struct kvm_vcpu {
    struct kvm *kvm;
    struct preempt_notifier preempt_notifier;
    int cpu;
    int vcpu_id;
    int srcu_idx;
    int mode;
    u64 requests;
    long unsigned int guest_debug;
    int pre_pcpu;
    struct list_head blocked_vcpu_list;
    struct mutex mutex;
    struct kvm_run *run;
    int guest_xcr0_loaded;
    struct swait_queue_head wq;
    struct pid *pid;
    int sigset_active;
    sigset_t sigset;
    struct kvm_vcpu_stat stat;
    unsigned int halt_poll_ns;
    bool valid_wakeup;
    int mmio_needed;
    int mmio_read_completed;
    int mmio_is_write;
    int mmio_cur_fragment;
    int mmio_nr_fragments;
    struct kvm_mmio_fragment mmio_fragments[2];
    struct (anon) spin_loop;
    bool preempted;
    bool ready;
    struct kvm_vcpu_arch arch;
    struct dentry *debugfs_dentry;
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
struct kvm_vcpu {
    struct kvm *kvm;
    struct preempt_notifier preempt_notifier;
    int cpu;
    int vcpu_id;
    int srcu_idx;
    int mode;
    u64 requests;
    long unsigned int guest_debug;
    int pre_pcpu;
    struct list_head blocked_vcpu_list;
    struct mutex mutex;
    struct kvm_run *run;
    int guest_xcr0_loaded;
    struct swait_queue_head wq;
    struct pid *pid;
    int sigset_active;
    sigset_t sigset;
    struct kvm_vcpu_stat stat;
    unsigned int halt_poll_ns;
    bool valid_wakeup;
    int mmio_needed;
    int mmio_read_completed;
    int mmio_is_write;
    int mmio_cur_fragment;
    int mmio_nr_fragments;
    struct kvm_mmio_fragment mmio_fragments[2];
    bool preempted;
    bool ready;
    struct kvm_vcpu_arch arch;
    struct dentry *debugfs_dentry;
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
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>char stats_id[48]</code>
</li>
<li>
<b>Field added. </b>
<code>int last_used_slot</code>
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
<code>int ____srcu_idx</code>
</li>
<li>
<b>Field added. </b>
<code>u64 last_used_slot_gen</code>
</li>
<li>
<b>Field removed. </b>
<code>int srcu_idx</code>
</li>
<li>
<b>Field removed. </b>
<code>int pre_pcpu</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head blocked_vcpu_list</code>
</li>
<li>
<b>Field type changed. </b>
<code>int last_used_slot</code> ➡️ <code>struct kvm_memory_slot *last_used_slot</code>
</li>
</ul>
</details>
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
