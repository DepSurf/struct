# Struct: <code>pstate_funcs</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct pstate_funcs {
    int (*get_max)();
    int (*get_max_physical)();
    int (*get_min)();
    int (*get_turbo)();
    int (*get_scaling)();
    void (*set)(struct cpudata *, int);
    void (*get_vid)(struct cpudata *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct pstate_funcs {
    int (*get_max)();
    int (*get_max_physical)();
    int (*get_min)();
    int (*get_turbo)();
    int (*get_scaling)();
    u64 (*get_val)(struct cpudata *, int);
    void (*get_vid)(struct cpudata *);
    int32_t (*get_target_pstate)(struct cpudata *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct pstate_funcs {
    int (*get_max)();
    int (*get_max_physical)();
    int (*get_min)();
    int (*get_turbo)();
    int (*get_scaling)();
    u64 (*get_val)(struct cpudata *, int);
    void (*get_vid)(struct cpudata *);
    int32_t (*get_target_pstate)(struct cpudata *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct pstate_funcs {
    int (*get_max)();
    int (*get_max_physical)();
    int (*get_min)();
    int (*get_turbo)();
    int (*get_scaling)();
    int (*get_aperf_mperf_shift)();
    u64 (*get_val)(struct cpudata *, int);
    void (*get_vid)(struct cpudata *);
    void (*update_util)(struct update_util_data *, u64, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct pstate_funcs {
    int (*get_max)();
    int (*get_max_physical)();
    int (*get_min)();
    int (*get_turbo)();
    int (*get_scaling)();
    int (*get_aperf_mperf_shift)();
    u64 (*get_val)(struct cpudata *, int);
    void (*get_vid)(struct cpudata *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct pstate_funcs {
    int (*get_max)();
    int (*get_max_physical)();
    int (*get_min)();
    int (*get_turbo)();
    int (*get_scaling)();
    int (*get_aperf_mperf_shift)();
    u64 (*get_val)(struct cpudata *, int);
    void (*get_vid)(struct cpudata *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct pstate_funcs {
    int (*get_max)();
    int (*get_max_physical)();
    int (*get_min)();
    int (*get_turbo)();
    int (*get_scaling)();
    int (*get_aperf_mperf_shift)();
    u64 (*get_val)(struct cpudata *, int);
    void (*get_vid)(struct cpudata *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct pstate_funcs {
    int (*get_max)();
    int (*get_max_physical)();
    int (*get_min)();
    int (*get_turbo)();
    int (*get_scaling)();
    int (*get_aperf_mperf_shift)();
    u64 (*get_val)(struct cpudata *, int);
    void (*get_vid)(struct cpudata *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct pstate_funcs {
    int (*get_max)();
    int (*get_max_physical)();
    int (*get_min)();
    int (*get_turbo)();
    int (*get_scaling)();
    int (*get_aperf_mperf_shift)();
    u64 (*get_val)(struct cpudata *, int);
    void (*get_vid)(struct cpudata *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct pstate_funcs {
    int (*get_max)();
    int (*get_max_physical)();
    int (*get_min)();
    int (*get_turbo)();
    int (*get_scaling)();
    int (*get_aperf_mperf_shift)();
    u64 (*get_val)(struct cpudata *, int);
    void (*get_vid)(struct cpudata *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct pstate_funcs {
    int (*get_max)();
    int (*get_max_physical)();
    int (*get_min)();
    int (*get_turbo)();
    int (*get_scaling)();
    int (*get_aperf_mperf_shift)();
    u64 (*get_val)(struct cpudata *, int);
    void (*get_vid)(struct cpudata *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct pstate_funcs {
    int (*get_max)();
    int (*get_max_physical)();
    int (*get_min)();
    int (*get_turbo)();
    int (*get_scaling)();
    int (*get_aperf_mperf_shift)();
    u64 (*get_val)(struct cpudata *, int);
    void (*get_vid)(struct cpudata *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct pstate_funcs {
    int (*get_max)();
    int (*get_max_physical)();
    int (*get_min)();
    int (*get_turbo)();
    int (*get_scaling)();
    int (*get_cpu_scaling)(int);
    int (*get_aperf_mperf_shift)();
    u64 (*get_val)(struct cpudata *, int);
    void (*get_vid)(struct cpudata *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct pstate_funcs {
    int (*get_max)();
    int (*get_max_physical)();
    int (*get_min)();
    int (*get_turbo)();
    int (*get_scaling)();
    int (*get_cpu_scaling)(int);
    int (*get_aperf_mperf_shift)();
    u64 (*get_val)(struct cpudata *, int);
    void (*get_vid)(struct cpudata *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct pstate_funcs {
    int (*get_max)(int);
    int (*get_max_physical)(int);
    int (*get_min)(int);
    int (*get_turbo)(int);
    int (*get_scaling)();
    int (*get_cpu_scaling)(int);
    int (*get_aperf_mperf_shift)();
    u64 (*get_val)(struct cpudata *, int);
    void (*get_vid)(struct cpudata *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct pstate_funcs {
    int (*get_max)(int);
    int (*get_max_physical)(int);
    int (*get_min)(int);
    int (*get_turbo)(int);
    int (*get_scaling)();
    int (*get_cpu_scaling)(int);
    int (*get_aperf_mperf_shift)();
    u64 (*get_val)(struct cpudata *, int);
    void (*get_vid)(struct cpudata *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct pstate_funcs {
    int (*get_max)(int);
    int (*get_max_physical)(int);
    int (*get_min)(int);
    int (*get_turbo)(int);
    int (*get_scaling)();
    int (*get_cpu_scaling)(int);
    int (*get_aperf_mperf_shift)();
    u64 (*get_val)(struct cpudata *, int);
    void (*get_vid)(struct cpudata *);
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
struct pstate_funcs {
    int (*get_max)();
    int (*get_max_physical)();
    int (*get_min)();
    int (*get_turbo)();
    int (*get_scaling)();
    int (*get_aperf_mperf_shift)();
    u64 (*get_val)(struct cpudata *, int);
    void (*get_vid)(struct cpudata *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct pstate_funcs {
    int (*get_max)();
    int (*get_max_physical)();
    int (*get_min)();
    int (*get_turbo)();
    int (*get_scaling)();
    int (*get_aperf_mperf_shift)();
    u64 (*get_val)(struct cpudata *, int);
    void (*get_vid)(struct cpudata *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct pstate_funcs {
    int (*get_max)();
    int (*get_max_physical)();
    int (*get_min)();
    int (*get_turbo)();
    int (*get_scaling)();
    int (*get_aperf_mperf_shift)();
    u64 (*get_val)(struct cpudata *, int);
    void (*get_vid)(struct cpudata *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct pstate_funcs {
    int (*get_max)();
    int (*get_max_physical)();
    int (*get_min)();
    int (*get_turbo)();
    int (*get_scaling)();
    int (*get_aperf_mperf_shift)();
    u64 (*get_val)(struct cpudata *, int);
    void (*get_vid)(struct cpudata *);
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
<code>u64 (*get_val)(struct cpudata *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int32_t (*get_target_pstate)(struct cpudata *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*set)(struct cpudata *, int)</code>
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
<b>Field added. </b>
<code>int (*get_aperf_mperf_shift)()</code>
</li>
<li>
<b>Field added. </b>
<code>void (*update_util)(struct update_util_data *, u64, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int32_t (*get_target_pstate)(struct cpudata *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>void (*update_util)(struct update_util_data *, u64, unsigned int)</code>
</li>
</ul>
</details>
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
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*get_cpu_scaling)(int)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*get_max)()</code> ➡️ <code>int (*get_max)(int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*get_max_physical)()</code> ➡️ <code>int (*get_max_physical)(int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*get_min)()</code> ➡️ <code>int (*get_min)(int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*get_turbo)()</code> ➡️ <code>int (*get_turbo)(int)</code>
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
