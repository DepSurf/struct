# Struct: <code>virtnet_rq_stats</code>

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
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct virtnet_rq_stats {
    struct u64_stats_sync syncp;
    u64 packets;
    u64 bytes;
    u64 drops;
    u64 xdp_packets;
    u64 xdp_tx;
    u64 xdp_redirects;
    u64 xdp_drops;
    u64 kicks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct virtnet_rq_stats {
    struct u64_stats_sync syncp;
    u64_stats_t packets;
    u64_stats_t bytes;
    u64_stats_t drops;
    u64_stats_t xdp_packets;
    u64_stats_t xdp_tx;
    u64_stats_t xdp_redirects;
    u64_stats_t xdp_drops;
    u64_stats_t kicks;
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>u64 packets</code> ➡️ <code>u64_stats_t packets</code>
</li>
<li>
<b>Field type changed. </b>
<code>u64 bytes</code> ➡️ <code>u64_stats_t bytes</code>
</li>
<li>
<b>Field type changed. </b>
<code>u64 drops</code> ➡️ <code>u64_stats_t drops</code>
</li>
<li>
<b>Field type changed. </b>
<code>u64 xdp_packets</code> ➡️ <code>u64_stats_t xdp_packets</code>
</li>
<li>
<b>Field type changed. </b>
<code>u64 xdp_tx</code> ➡️ <code>u64_stats_t xdp_tx</code>
</li>
<li>
<b>Field type changed. </b>
<code>u64 xdp_redirects</code> ➡️ <code>u64_stats_t xdp_redirects</code>
</li>
<li>
<b>Field type changed. </b>
<code>u64 xdp_drops</code> ➡️ <code>u64_stats_t xdp_drops</code>
</li>
<li>
<b>Field type changed. </b>
<code>u64 kicks</code> ➡️ <code>u64_stats_t kicks</code>
</li>
</ul>
</details>
</li>
</ul>
