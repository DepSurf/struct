# Struct: <code>dpll_pin_ops</code>

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
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dpll_pin_ops {
    int (*frequency_set)(const struct dpll_pin *, void *, const struct dpll_device *, void *, const u64, struct netlink_ext_ack *);
    int (*frequency_get)(const struct dpll_pin *, void *, const struct dpll_device *, void *, u64 *, struct netlink_ext_ack *);
    int (*direction_set)(const struct dpll_pin *, void *, const struct dpll_device *, void *, const enum dpll_pin_direction, struct netlink_ext_ack *);
    int (*direction_get)(const struct dpll_pin *, void *, const struct dpll_device *, void *, enum dpll_pin_direction *, struct netlink_ext_ack *);
    int (*state_on_pin_get)(const struct dpll_pin *, void *, const struct dpll_pin *, void *, enum dpll_pin_state *, struct netlink_ext_ack *);
    int (*state_on_dpll_get)(const struct dpll_pin *, void *, const struct dpll_device *, void *, enum dpll_pin_state *, struct netlink_ext_ack *);
    int (*state_on_pin_set)(const struct dpll_pin *, void *, const struct dpll_pin *, void *, const enum dpll_pin_state, struct netlink_ext_ack *);
    int (*state_on_dpll_set)(const struct dpll_pin *, void *, const struct dpll_device *, void *, const enum dpll_pin_state, struct netlink_ext_ack *);
    int (*prio_get)(const struct dpll_pin *, void *, const struct dpll_device *, void *, u32 *, struct netlink_ext_ack *);
    int (*prio_set)(const struct dpll_pin *, void *, const struct dpll_device *, void *, const u32, struct netlink_ext_ack *);
    int (*phase_offset_get)(const struct dpll_pin *, void *, const struct dpll_device *, void *, s64 *, struct netlink_ext_ack *);
    int (*phase_adjust_get)(const struct dpll_pin *, void *, const struct dpll_device *, void *, s32 *, struct netlink_ext_ack *);
    int (*phase_adjust_set)(const struct dpll_pin *, void *, const struct dpll_device *, void *, const s32, struct netlink_ext_ack *);
    int (*ffo_get)(const struct dpll_pin *, void *, const struct dpll_device *, void *, s64 *, struct netlink_ext_ack *);
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
</ul>
