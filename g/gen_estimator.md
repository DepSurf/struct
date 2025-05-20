# Struct: <code>gen_estimator</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct gen_estimator {
    struct list_head list;
    struct gnet_stats_basic_packed *bstats;
    struct gnet_stats_rate_est64 *rate_est;
    spinlock_t *stats_lock;
    int ewma_log;
    u32 last_packets;
    long unsigned int avpps;
    u64 last_bytes;
    u64 avbps;
    struct callback_head e_rcu;
    struct rb_node node;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct callback_head head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct gen_estimator {
    struct list_head list;
    struct gnet_stats_basic_packed *bstats;
    struct gnet_stats_rate_est64 *rate_est;
    spinlock_t *stats_lock;
    seqcount_t *running;
    int ewma_log;
    u32 last_packets;
    long unsigned int avpps;
    u64 last_bytes;
    u64 avbps;
    struct callback_head e_rcu;
    struct rb_node node;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct callback_head head;
};
```
</details>
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
<details>
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>seqcount_t *running</code>
</li>
</ul>
</details>
</li>
</ul>
