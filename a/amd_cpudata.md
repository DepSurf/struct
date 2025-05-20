# Struct: <code>amd_cpudata</code>

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
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct amd_cpudata {
    int cpu;
    struct freq_qos_request req[2];
    u64 cppc_req_cached;
    u32 highest_perf;
    u32 nominal_perf;
    u32 lowest_nonlinear_perf;
    u32 lowest_perf;
    u32 max_freq;
    u32 min_freq;
    u32 nominal_freq;
    u32 lowest_nonlinear_freq;
    struct amd_aperf_mperf cur;
    struct amd_aperf_mperf prev;
    u64 freq;
    bool boost_supported;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct amd_cpudata {
    int cpu;
    struct freq_qos_request req[2];
    u64 cppc_req_cached;
    u32 highest_perf;
    u32 nominal_perf;
    u32 lowest_nonlinear_perf;
    u32 lowest_perf;
    u32 max_freq;
    u32 min_freq;
    u32 nominal_freq;
    u32 lowest_nonlinear_freq;
    struct amd_aperf_mperf cur;
    struct amd_aperf_mperf prev;
    u64 freq;
    bool boost_supported;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct amd_cpudata {
    int cpu;
    struct freq_qos_request req[2];
    u64 cppc_req_cached;
    u32 highest_perf;
    u32 nominal_perf;
    u32 lowest_nonlinear_perf;
    u32 lowest_perf;
    u32 max_freq;
    u32 min_freq;
    u32 nominal_freq;
    u32 lowest_nonlinear_freq;
    struct amd_aperf_mperf cur;
    struct amd_aperf_mperf prev;
    u64 freq;
    bool boost_supported;
    s16 epp_policy;
    s16 epp_cached;
    u32 policy;
    u64 cppc_cap1_cached;
    bool suspended;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct amd_cpudata {
    int cpu;
    struct freq_qos_request req[2];
    u64 cppc_req_cached;
    u32 highest_perf;
    u32 nominal_perf;
    u32 lowest_nonlinear_perf;
    u32 lowest_perf;
    u32 min_limit_perf;
    u32 max_limit_perf;
    u32 min_limit_freq;
    u32 max_limit_freq;
    u32 max_freq;
    u32 min_freq;
    u32 nominal_freq;
    u32 lowest_nonlinear_freq;
    struct amd_aperf_mperf cur;
    struct amd_aperf_mperf prev;
    u64 freq;
    bool boost_supported;
    s16 epp_policy;
    s16 epp_cached;
    u32 policy;
    u64 cppc_cap1_cached;
    bool suspended;
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
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>s16 epp_policy</code>
</li>
<li>
<b>Field added. </b>
<code>s16 epp_cached</code>
</li>
<li>
<b>Field added. </b>
<code>u32 policy</code>
</li>
<li>
<b>Field added. </b>
<code>u64 cppc_cap1_cached</code>
</li>
<li>
<b>Field added. </b>
<code>bool suspended</code>
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
<code>u32 min_limit_perf</code>
</li>
<li>
<b>Field added. </b>
<code>u32 max_limit_perf</code>
</li>
<li>
<b>Field added. </b>
<code>u32 min_limit_freq</code>
</li>
<li>
<b>Field added. </b>
<code>u32 max_limit_freq</code>
</li>
</ul>
</details>
</li>
</ul>
