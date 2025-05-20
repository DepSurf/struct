# Struct: <code>ti_sci_clk_ops</code>

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
struct ti_sci_clk_ops {
    int (*get_clock)(const struct ti_sci_handle *, u32, u32, bool, bool, bool);
    int (*idle_clock)(const struct ti_sci_handle *, u32, u32);
    int (*put_clock)(const struct ti_sci_handle *, u32, u32);
    int (*is_auto)(const struct ti_sci_handle *, u32, u32, bool *);
    int (*is_on)(const struct ti_sci_handle *, u32, u32, bool *, bool *);
    int (*is_off)(const struct ti_sci_handle *, u32, u32, bool *, bool *);
    int (*set_parent)(const struct ti_sci_handle *, u32, u32, u32);
    int (*get_parent)(const struct ti_sci_handle *, u32, u32, u32 *);
    int (*get_num_parents)(const struct ti_sci_handle *, u32, u32, u32 *);
    int (*get_best_match_freq)(const struct ti_sci_handle *, u32, u32, u64, u64, u64, u64 *);
    int (*set_freq)(const struct ti_sci_handle *, u32, u32, u64, u64, u64);
    int (*get_freq)(const struct ti_sci_handle *, u32, u32, u64 *);
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
