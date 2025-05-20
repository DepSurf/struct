# Struct: <code>mu3h_sch_ep_info</code>

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
struct mu3h_sch_ep_info {
    u32 esit;
    u32 num_budget_microframes;
    u32 bw_cost_per_microframe;
    struct list_head endpoint;
    struct list_head tt_endpoint;
    struct mu3h_sch_tt *sch_tt;
    u32 ep_type;
    u32 maxpkt;
    void *ep;
    u32 offset;
    u32 repeat;
    u32 pkts;
    u32 cs_count;
    u32 burst_mode;
    u32 bw_budget_table[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mu3h_sch_ep_info {
    u32 esit;
    u32 num_budget_microframes;
    u32 bw_cost_per_microframe;
    struct list_head endpoint;
    struct list_head tt_endpoint;
    struct mu3h_sch_tt *sch_tt;
    u32 ep_type;
    u32 maxpkt;
    void *ep;
    u32 offset;
    u32 repeat;
    u32 pkts;
    u32 cs_count;
    u32 burst_mode;
    u32 bw_budget_table[0];
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
