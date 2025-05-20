# Struct: <code>scmi_perf_ops</code>

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
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct scmi_perf_ops {
    int (*limits_set)(const struct scmi_handle *, u32, u32, u32);
    int (*limits_get)(const struct scmi_handle *, u32, u32 *, u32 *);
    int (*level_set)(const struct scmi_handle *, u32, u32, bool);
    int (*level_get)(const struct scmi_handle *, u32, u32 *, bool);
    int (*device_domain_id)(struct device *);
    int (*transition_latency_get)(const struct scmi_handle *, struct device *);
    int (*device_opps_add)(const struct scmi_handle *, struct device *);
    int (*freq_set)(const struct scmi_handle *, u32, long unsigned int, bool);
    int (*freq_get)(const struct scmi_handle *, u32, long unsigned int *, bool);
    int (*est_power_get)(const struct scmi_handle *, u32, long unsigned int *, long unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct scmi_perf_ops {
    int (*limits_set)(const struct scmi_handle *, u32, u32, u32);
    int (*limits_get)(const struct scmi_handle *, u32, u32 *, u32 *);
    int (*level_set)(const struct scmi_handle *, u32, u32, bool);
    int (*level_get)(const struct scmi_handle *, u32, u32 *, bool);
    int (*device_domain_id)(struct device *);
    int (*transition_latency_get)(const struct scmi_handle *, struct device *);
    int (*device_opps_add)(const struct scmi_handle *, struct device *);
    int (*freq_set)(const struct scmi_handle *, u32, long unsigned int, bool);
    int (*freq_get)(const struct scmi_handle *, u32, long unsigned int *, bool);
    int (*est_power_get)(const struct scmi_handle *, u32, long unsigned int *, long unsigned int *);
};
```
</details>
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
<b>Arch</b>
<ul>
</ul>
