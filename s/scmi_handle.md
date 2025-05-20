# Struct: <code>scmi_handle</code>

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
struct scmi_handle {
    struct device *dev;
    struct scmi_revision_info *version;
    struct scmi_perf_ops *perf_ops;
    struct scmi_clk_ops *clk_ops;
    struct scmi_power_ops *power_ops;
    struct scmi_sensor_ops *sensor_ops;
    struct scmi_reset_ops *reset_ops;
    void *perf_priv;
    void *clk_priv;
    void *power_priv;
    void *sensor_priv;
    void *reset_priv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct scmi_handle {
    struct device *dev;
    struct scmi_revision_info *version;
    struct scmi_perf_ops *perf_ops;
    struct scmi_clk_ops *clk_ops;
    struct scmi_power_ops *power_ops;
    struct scmi_sensor_ops *sensor_ops;
    struct scmi_reset_ops *reset_ops;
    void *perf_priv;
    void *clk_priv;
    void *power_priv;
    void *sensor_priv;
    void *reset_priv;
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
