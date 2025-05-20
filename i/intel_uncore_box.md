# Struct: <code>intel_uncore_box</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct intel_uncore_box {
    int phys_id;
    int n_active;
    int n_events;
    int cpu;
    long unsigned int flags;
    atomic_t refcnt;
    struct perf_event * events[9];
    struct perf_event * event_list[9];
    struct event_constraint * event_constraint[9];
    long unsigned int active_mask[1];
    u64 tags[9];
    struct pci_dev *pci_dev;
    struct intel_uncore_pmu *pmu;
    u64 hrtimer_duration;
    struct hrtimer hrtimer;
    struct list_head list;
    struct list_head active_list;
    void *io_addr;
    struct intel_uncore_extra_reg shared_regs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct intel_uncore_box {
    int pci_phys_id;
    int pkgid;
    int n_active;
    int n_events;
    int cpu;
    long unsigned int flags;
    atomic_t refcnt;
    struct perf_event * events[9];
    struct perf_event * event_list[9];
    struct event_constraint * event_constraint[9];
    long unsigned int active_mask[1];
    u64 tags[9];
    struct pci_dev *pci_dev;
    struct intel_uncore_pmu *pmu;
    u64 hrtimer_duration;
    struct hrtimer hrtimer;
    struct list_head list;
    struct list_head active_list;
    void *io_addr;
    struct intel_uncore_extra_reg shared_regs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct intel_uncore_box {
    int pci_phys_id;
    int pkgid;
    int n_active;
    int n_events;
    int cpu;
    long unsigned int flags;
    atomic_t refcnt;
    struct perf_event * events[9];
    struct perf_event * event_list[9];
    struct event_constraint * event_constraint[9];
    long unsigned int active_mask[1];
    u64 tags[9];
    struct pci_dev *pci_dev;
    struct intel_uncore_pmu *pmu;
    u64 hrtimer_duration;
    struct hrtimer hrtimer;
    struct list_head list;
    struct list_head active_list;
    void *io_addr;
    struct intel_uncore_extra_reg shared_regs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct intel_uncore_box {
    int pci_phys_id;
    int pkgid;
    int n_active;
    int n_events;
    int cpu;
    long unsigned int flags;
    atomic_t refcnt;
    struct perf_event * events[9];
    struct perf_event * event_list[9];
    struct event_constraint * event_constraint[9];
    long unsigned int active_mask[1];
    u64 tags[9];
    struct pci_dev *pci_dev;
    struct intel_uncore_pmu *pmu;
    u64 hrtimer_duration;
    struct hrtimer hrtimer;
    struct list_head list;
    struct list_head active_list;
    void *io_addr;
    struct intel_uncore_extra_reg shared_regs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct intel_uncore_box {
    int pci_phys_id;
    int pkgid;
    int n_active;
    int n_events;
    int cpu;
    long unsigned int flags;
    atomic_t refcnt;
    struct perf_event * events[9];
    struct perf_event * event_list[9];
    struct event_constraint * event_constraint[9];
    long unsigned int active_mask[1];
    u64 tags[9];
    struct pci_dev *pci_dev;
    struct intel_uncore_pmu *pmu;
    u64 hrtimer_duration;
    struct hrtimer hrtimer;
    struct list_head list;
    struct list_head active_list;
    void *io_addr;
    struct intel_uncore_extra_reg shared_regs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct intel_uncore_box {
    int pci_phys_id;
    int pkgid;
    int n_active;
    int n_events;
    int cpu;
    long unsigned int flags;
    atomic_t refcnt;
    struct perf_event * events[10];
    struct perf_event * event_list[10];
    struct event_constraint * event_constraint[10];
    long unsigned int active_mask[1];
    u64 tags[10];
    struct pci_dev *pci_dev;
    struct intel_uncore_pmu *pmu;
    u64 hrtimer_duration;
    struct hrtimer hrtimer;
    struct list_head list;
    struct list_head active_list;
    void *io_addr;
    struct intel_uncore_extra_reg shared_regs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct intel_uncore_box {
    int pci_phys_id;
    int pkgid;
    int n_active;
    int n_events;
    int cpu;
    long unsigned int flags;
    atomic_t refcnt;
    struct perf_event * events[10];
    struct perf_event * event_list[10];
    struct event_constraint * event_constraint[10];
    long unsigned int active_mask[1];
    u64 tags[10];
    struct pci_dev *pci_dev;
    struct intel_uncore_pmu *pmu;
    u64 hrtimer_duration;
    struct hrtimer hrtimer;
    struct list_head list;
    struct list_head active_list;
    void *io_addr;
    struct intel_uncore_extra_reg shared_regs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct intel_uncore_box {
    int pci_phys_id;
    int dieid;
    int n_active;
    int n_events;
    int cpu;
    long unsigned int flags;
    atomic_t refcnt;
    struct perf_event * events[10];
    struct perf_event * event_list[10];
    struct event_constraint * event_constraint[10];
    long unsigned int active_mask[1];
    u64 tags[10];
    struct pci_dev *pci_dev;
    struct intel_uncore_pmu *pmu;
    u64 hrtimer_duration;
    struct hrtimer hrtimer;
    struct list_head list;
    struct list_head active_list;
    void *io_addr;
    struct intel_uncore_extra_reg shared_regs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct intel_uncore_box {
    int pci_phys_id;
    int dieid;
    int n_active;
    int n_events;
    int cpu;
    long unsigned int flags;
    atomic_t refcnt;
    struct perf_event * events[10];
    struct perf_event * event_list[10];
    struct event_constraint * event_constraint[10];
    long unsigned int active_mask[1];
    u64 tags[10];
    struct pci_dev *pci_dev;
    struct intel_uncore_pmu *pmu;
    u64 hrtimer_duration;
    struct hrtimer hrtimer;
    struct list_head list;
    struct list_head active_list;
    void *io_addr;
    struct intel_uncore_extra_reg shared_regs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct intel_uncore_box {
    int pci_phys_id;
    int dieid;
    int n_active;
    int n_events;
    int cpu;
    long unsigned int flags;
    atomic_t refcnt;
    struct perf_event * events[10];
    struct perf_event * event_list[10];
    struct event_constraint * event_constraint[10];
    long unsigned int active_mask[1];
    u64 tags[10];
    struct pci_dev *pci_dev;
    struct intel_uncore_pmu *pmu;
    u64 hrtimer_duration;
    struct hrtimer hrtimer;
    struct list_head list;
    struct list_head active_list;
    void *io_addr;
    struct intel_uncore_extra_reg shared_regs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct intel_uncore_box {
    int pci_phys_id;
    int dieid;
    int n_active;
    int n_events;
    int cpu;
    long unsigned int flags;
    atomic_t refcnt;
    struct perf_event * events[10];
    struct perf_event * event_list[10];
    struct event_constraint * event_constraint[10];
    long unsigned int active_mask[1];
    u64 tags[10];
    struct pci_dev *pci_dev;
    struct intel_uncore_pmu *pmu;
    u64 hrtimer_duration;
    struct hrtimer hrtimer;
    struct list_head list;
    struct list_head active_list;
    void *io_addr;
    struct intel_uncore_extra_reg shared_regs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct intel_uncore_box {
    int dieid;
    int n_active;
    int n_events;
    int cpu;
    long unsigned int flags;
    atomic_t refcnt;
    struct perf_event * events[10];
    struct perf_event * event_list[10];
    struct event_constraint * event_constraint[10];
    long unsigned int active_mask[1];
    u64 tags[10];
    struct pci_dev *pci_dev;
    struct intel_uncore_pmu *pmu;
    u64 hrtimer_duration;
    struct hrtimer hrtimer;
    struct list_head list;
    struct list_head active_list;
    void *io_addr;
    struct intel_uncore_extra_reg shared_regs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct intel_uncore_box {
    int dieid;
    int n_active;
    int n_events;
    int cpu;
    long unsigned int flags;
    atomic_t refcnt;
    struct perf_event * events[10];
    struct perf_event * event_list[10];
    struct event_constraint * event_constraint[10];
    long unsigned int active_mask[1];
    u64 tags[10];
    struct pci_dev *pci_dev;
    struct intel_uncore_pmu *pmu;
    u64 hrtimer_duration;
    struct hrtimer hrtimer;
    struct list_head list;
    struct list_head active_list;
    void *io_addr;
    struct intel_uncore_extra_reg shared_regs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct intel_uncore_box {
    int dieid;
    int n_active;
    int n_events;
    int cpu;
    long unsigned int flags;
    atomic_t refcnt;
    struct perf_event * events[10];
    struct perf_event * event_list[10];
    struct event_constraint * event_constraint[10];
    long unsigned int active_mask[1];
    u64 tags[10];
    struct pci_dev *pci_dev;
    struct intel_uncore_pmu *pmu;
    u64 hrtimer_duration;
    struct hrtimer hrtimer;
    struct list_head list;
    struct list_head active_list;
    void *io_addr;
    struct intel_uncore_extra_reg shared_regs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct intel_uncore_box {
    int dieid;
    int n_active;
    int n_events;
    int cpu;
    long unsigned int flags;
    atomic_t refcnt;
    struct perf_event * events[10];
    struct perf_event * event_list[10];
    struct event_constraint * event_constraint[10];
    long unsigned int active_mask[1];
    u64 tags[10];
    struct pci_dev *pci_dev;
    struct intel_uncore_pmu *pmu;
    u64 hrtimer_duration;
    struct hrtimer hrtimer;
    struct list_head list;
    struct list_head active_list;
    void *io_addr;
    struct intel_uncore_extra_reg shared_regs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct intel_uncore_box {
    int dieid;
    int n_active;
    int n_events;
    int cpu;
    long unsigned int flags;
    atomic_t refcnt;
    struct perf_event * events[10];
    struct perf_event * event_list[10];
    struct event_constraint * event_constraint[10];
    long unsigned int active_mask[1];
    u64 tags[10];
    struct pci_dev *pci_dev;
    struct intel_uncore_pmu *pmu;
    u64 hrtimer_duration;
    struct hrtimer hrtimer;
    struct list_head list;
    struct list_head active_list;
    void *io_addr;
    struct intel_uncore_extra_reg shared_regs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct intel_uncore_box {
    int dieid;
    int n_active;
    int n_events;
    int cpu;
    long unsigned int flags;
    atomic_t refcnt;
    struct perf_event * events[10];
    struct perf_event * event_list[10];
    struct event_constraint * event_constraint[10];
    long unsigned int active_mask[1];
    u64 tags[10];
    struct pci_dev *pci_dev;
    struct intel_uncore_pmu *pmu;
    u64 hrtimer_duration;
    struct hrtimer hrtimer;
    struct list_head list;
    struct list_head active_list;
    void *io_addr;
    struct intel_uncore_extra_reg shared_regs[0];
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct intel_uncore_box {
    int pci_phys_id;
    int dieid;
    int n_active;
    int n_events;
    int cpu;
    long unsigned int flags;
    atomic_t refcnt;
    struct perf_event * events[10];
    struct perf_event * event_list[10];
    struct event_constraint * event_constraint[10];
    long unsigned int active_mask[1];
    u64 tags[10];
    struct pci_dev *pci_dev;
    struct intel_uncore_pmu *pmu;
    u64 hrtimer_duration;
    struct hrtimer hrtimer;
    struct list_head list;
    struct list_head active_list;
    void *io_addr;
    struct intel_uncore_extra_reg shared_regs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct intel_uncore_box {
    int pci_phys_id;
    int dieid;
    int n_active;
    int n_events;
    int cpu;
    long unsigned int flags;
    atomic_t refcnt;
    struct perf_event * events[10];
    struct perf_event * event_list[10];
    struct event_constraint * event_constraint[10];
    long unsigned int active_mask[1];
    u64 tags[10];
    struct pci_dev *pci_dev;
    struct intel_uncore_pmu *pmu;
    u64 hrtimer_duration;
    struct hrtimer hrtimer;
    struct list_head list;
    struct list_head active_list;
    void *io_addr;
    struct intel_uncore_extra_reg shared_regs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct intel_uncore_box {
    int pci_phys_id;
    int dieid;
    int n_active;
    int n_events;
    int cpu;
    long unsigned int flags;
    atomic_t refcnt;
    struct perf_event * events[10];
    struct perf_event * event_list[10];
    struct event_constraint * event_constraint[10];
    long unsigned int active_mask[1];
    u64 tags[10];
    struct pci_dev *pci_dev;
    struct intel_uncore_pmu *pmu;
    u64 hrtimer_duration;
    struct hrtimer hrtimer;
    struct list_head list;
    struct list_head active_list;
    void *io_addr;
    struct intel_uncore_extra_reg shared_regs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct intel_uncore_box {
    int pci_phys_id;
    int dieid;
    int n_active;
    int n_events;
    int cpu;
    long unsigned int flags;
    atomic_t refcnt;
    struct perf_event * events[10];
    struct perf_event * event_list[10];
    struct event_constraint * event_constraint[10];
    long unsigned int active_mask[1];
    u64 tags[10];
    struct pci_dev *pci_dev;
    struct intel_uncore_pmu *pmu;
    u64 hrtimer_duration;
    struct hrtimer hrtimer;
    struct list_head list;
    struct list_head active_list;
    void *io_addr;
    struct intel_uncore_extra_reg shared_regs[0];
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int pci_phys_id</code>
</li>
<li>
<b>Field added. </b>
<code>int pkgid</code>
</li>
<li>
<b>Field removed. </b>
<code>int phys_id</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct perf_event * events[9]</code> ➡️ <code>struct perf_event * events[10]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct perf_event * event_list[9]</code> ➡️ <code>struct perf_event * event_list[10]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct event_constraint * event_constraint[9]</code> ➡️ <code>struct event_constraint * event_constraint[10]</code>
</li>
<li>
<b>Field type changed. </b>
<code>u64 tags[9]</code> ➡️ <code>u64 tags[10]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int dieid</code>
</li>
<li>
<b>Field removed. </b>
<code>int pkgid</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int pci_phys_id</code>
</li>
</ul>
</details>
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
<b>Flavor</b>
<ul>
<li>
No changes between <code>generic</code> and <code>aws</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
