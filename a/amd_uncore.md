# Struct: <code>amd_uncore</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct amd_uncore {
    int id;
    int refcnt;
    int cpu;
    int num_counters;
    int rdpmc_base;
    u32 msr_base;
    cpumask_t *active_mask;
    struct pmu *pmu;
    struct perf_event * events[4];
    struct amd_uncore *free_when_cpu_online;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct amd_uncore {
    int id;
    int refcnt;
    int cpu;
    int num_counters;
    int rdpmc_base;
    u32 msr_base;
    cpumask_t *active_mask;
    struct pmu *pmu;
    struct perf_event * events[4];
    struct hlist_node node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct amd_uncore {
    int id;
    int refcnt;
    int cpu;
    int num_counters;
    int rdpmc_base;
    u32 msr_base;
    cpumask_t *active_mask;
    struct pmu *pmu;
    struct perf_event * events[4];
    struct hlist_node node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct amd_uncore {
    int id;
    int refcnt;
    int cpu;
    int num_counters;
    int rdpmc_base;
    u32 msr_base;
    cpumask_t *active_mask;
    struct pmu *pmu;
    struct perf_event * events[6];
    struct hlist_node node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct amd_uncore {
    int id;
    int refcnt;
    int cpu;
    int num_counters;
    int rdpmc_base;
    u32 msr_base;
    cpumask_t *active_mask;
    struct pmu *pmu;
    struct perf_event * events[6];
    struct hlist_node node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct amd_uncore {
    int id;
    int refcnt;
    int cpu;
    int num_counters;
    int rdpmc_base;
    u32 msr_base;
    cpumask_t *active_mask;
    struct pmu *pmu;
    struct perf_event * events[6];
    struct hlist_node node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct amd_uncore {
    int id;
    int refcnt;
    int cpu;
    int num_counters;
    int rdpmc_base;
    u32 msr_base;
    cpumask_t *active_mask;
    struct pmu *pmu;
    struct perf_event * events[6];
    struct hlist_node node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct amd_uncore {
    int id;
    int refcnt;
    int cpu;
    int num_counters;
    int rdpmc_base;
    u32 msr_base;
    cpumask_t *active_mask;
    struct pmu *pmu;
    struct perf_event * events[6];
    struct hlist_node node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct amd_uncore {
    int id;
    int refcnt;
    int cpu;
    int num_counters;
    int rdpmc_base;
    u32 msr_base;
    cpumask_t *active_mask;
    struct pmu *pmu;
    struct perf_event * events[6];
    struct hlist_node node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct amd_uncore {
    int id;
    int refcnt;
    int cpu;
    int num_counters;
    int rdpmc_base;
    u32 msr_base;
    cpumask_t *active_mask;
    struct pmu *pmu;
    struct perf_event * events[6];
    struct hlist_node node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct amd_uncore {
    int id;
    int refcnt;
    int cpu;
    int num_counters;
    int rdpmc_base;
    u32 msr_base;
    cpumask_t *active_mask;
    struct pmu *pmu;
    struct perf_event * events[6];
    struct hlist_node node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct amd_uncore {
    int id;
    int refcnt;
    int cpu;
    int num_counters;
    int rdpmc_base;
    u32 msr_base;
    cpumask_t *active_mask;
    struct pmu *pmu;
    struct perf_event * events[6];
    struct hlist_node node;
};
```
</details>
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
In <code>5.19</code>: Absent ⚠️
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
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
struct amd_uncore {
    int id;
    int refcnt;
    int cpu;
    int num_counters;
    int rdpmc_base;
    u32 msr_base;
    cpumask_t *active_mask;
    struct pmu *pmu;
    struct perf_event * events[6];
    struct hlist_node node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct amd_uncore {
    int id;
    int refcnt;
    int cpu;
    int num_counters;
    int rdpmc_base;
    u32 msr_base;
    cpumask_t *active_mask;
    struct pmu *pmu;
    struct perf_event * events[6];
    struct hlist_node node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct amd_uncore {
    int id;
    int refcnt;
    int cpu;
    int num_counters;
    int rdpmc_base;
    u32 msr_base;
    cpumask_t *active_mask;
    struct pmu *pmu;
    struct perf_event * events[6];
    struct hlist_node node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct amd_uncore {
    int id;
    int refcnt;
    int cpu;
    int num_counters;
    int rdpmc_base;
    u32 msr_base;
    cpumask_t *active_mask;
    struct pmu *pmu;
    struct perf_event * events[6];
    struct hlist_node node;
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
<code>struct hlist_node node</code>
</li>
<li>
<b>Field removed. </b>
<code>struct amd_uncore *free_when_cpu_online</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct perf_event * events[4]</code> ➡️ <code>struct perf_event * events[6]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
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
No changes between <code>5.11</code> and <code>5.13</code> ✅
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
