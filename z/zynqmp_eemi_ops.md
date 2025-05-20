# Struct: <code>zynqmp_eemi_ops</code>

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
struct zynqmp_eemi_ops {
    int (*get_api_version)(u32 *);
    int (*get_chipid)(u32 *, u32 *);
    int (*fpga_load)(const u64, const u32, const u32);
    int (*fpga_get_status)(u32 *);
    int (*query_data)(struct zynqmp_pm_query_data, u32 *);
    int (*clock_enable)(u32);
    int (*clock_disable)(u32);
    int (*clock_getstate)(u32, u32 *);
    int (*clock_setdivider)(u32, u32);
    int (*clock_getdivider)(u32, u32 *);
    int (*clock_setrate)(u32, u64);
    int (*clock_getrate)(u32, u64 *);
    int (*clock_setparent)(u32, u32);
    int (*clock_getparent)(u32, u32 *);
    int (*ioctl)(u32, u32, u32, u32, u32 *);
    int (*reset_assert)(const enum zynqmp_pm_reset, const enum zynqmp_pm_reset_action);
    int (*reset_get_status)(const enum zynqmp_pm_reset, u32 *);
    int (*init_finalize)();
    int (*set_suspend_mode)(u32);
    int (*request_node)(const u32, const u32, const u32, const enum zynqmp_pm_request_ack);
    int (*release_node)(const u32);
    int (*set_requirement)(const u32, const u32, const u32, const enum zynqmp_pm_request_ack);
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
<b>Arch</b>
<ul>
</ul>
