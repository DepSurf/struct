# Struct: <code>tcf_gate</code>

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
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct tcf_gate {
    struct tc_action common;
    struct tcf_gate_params param;
    u8 current_gate_status;
    ktime_t current_close_time;
    u32 current_entry_octets;
    s32 current_max_octets;
    struct tcfg_gate_entry *next_entry;
    struct hrtimer hitimer;
    enum tk_offsets tk_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct tcf_gate {
    struct tc_action common;
    struct tcf_gate_params param;
    u8 current_gate_status;
    ktime_t current_close_time;
    u32 current_entry_octets;
    s32 current_max_octets;
    struct tcfg_gate_entry *next_entry;
    struct hrtimer hitimer;
    enum tk_offsets tk_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct tcf_gate {
    struct tc_action common;
    struct tcf_gate_params param;
    u8 current_gate_status;
    ktime_t current_close_time;
    u32 current_entry_octets;
    s32 current_max_octets;
    struct tcfg_gate_entry *next_entry;
    struct hrtimer hitimer;
    enum tk_offsets tk_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct tcf_gate {
    struct tc_action common;
    struct tcf_gate_params param;
    u8 current_gate_status;
    ktime_t current_close_time;
    u32 current_entry_octets;
    s32 current_max_octets;
    struct tcfg_gate_entry *next_entry;
    struct hrtimer hitimer;
    enum tk_offsets tk_offset;
};
```
</details>
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
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
</ul>
