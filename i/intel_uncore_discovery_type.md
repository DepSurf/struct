# Struct: <code>intel_uncore_discovery_type</code>

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
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct intel_uncore_discovery_type {
    struct rb_node node;
    enum uncore_access_type access_type;
    u64 box_ctrl;
    u64 *box_ctrl_die;
    u16 type;
    u8 num_counters;
    u8 counter_width;
    u8 ctl_offset;
    u8 ctr_offset;
    u16 num_boxes;
    unsigned int *ids;
    unsigned int *box_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct intel_uncore_discovery_type {
    struct rb_node node;
    enum uncore_access_type access_type;
    u64 box_ctrl;
    u64 *box_ctrl_die;
    u16 type;
    u8 num_counters;
    u8 counter_width;
    u8 ctl_offset;
    u8 ctr_offset;
    u16 num_boxes;
    unsigned int *ids;
    unsigned int *box_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct intel_uncore_discovery_type {
    struct rb_node node;
    enum uncore_access_type access_type;
    u64 box_ctrl;
    u64 *box_ctrl_die;
    u16 type;
    u8 num_counters;
    u8 counter_width;
    u8 ctl_offset;
    u8 ctr_offset;
    u16 num_boxes;
    unsigned int *ids;
    unsigned int *box_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct intel_uncore_discovery_type {
    struct rb_node node;
    enum uncore_access_type access_type;
    u64 box_ctrl;
    u64 *box_ctrl_die;
    u16 type;
    u8 num_counters;
    u8 counter_width;
    u8 ctl_offset;
    u8 ctr_offset;
    u16 num_boxes;
    unsigned int *ids;
    unsigned int *box_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct intel_uncore_discovery_type {
    struct rb_node node;
    enum uncore_access_type access_type;
    u64 box_ctrl;
    u64 *box_ctrl_die;
    u16 type;
    u8 num_counters;
    u8 counter_width;
    u8 ctl_offset;
    u8 ctr_offset;
    u16 num_boxes;
    unsigned int *ids;
    unsigned int *box_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct intel_uncore_discovery_type {
    struct rb_node node;
    enum uncore_access_type access_type;
    u64 box_ctrl;
    u64 *box_ctrl_die;
    u16 type;
    u8 num_counters;
    u8 counter_width;
    u8 ctl_offset;
    u8 ctr_offset;
    u16 num_boxes;
    unsigned int *ids;
    u64 *box_offset;
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>unsigned int *box_offset</code> ➡️ <code>u64 *box_offset</code>
</li>
</ul>
</details>
</li>
</ul>
