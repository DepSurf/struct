# Struct: <code>tun_pcpu_stats</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct tun_pcpu_stats {
    u64 rx_packets;
    u64 rx_bytes;
    u64 tx_packets;
    u64 tx_bytes;
    struct u64_stats_sync syncp;
    u32 rx_dropped;
    u32 tx_dropped;
    u32 rx_frame_errors;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct tun_pcpu_stats {
    u64 rx_packets;
    u64 rx_bytes;
    u64 tx_packets;
    u64 tx_bytes;
    struct u64_stats_sync syncp;
    u32 rx_dropped;
    u32 tx_dropped;
    u32 rx_frame_errors;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct tun_pcpu_stats {
    u64 rx_packets;
    u64 rx_bytes;
    u64 tx_packets;
    u64 tx_bytes;
    struct u64_stats_sync syncp;
    u32 rx_dropped;
    u32 tx_dropped;
    u32 rx_frame_errors;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct tun_pcpu_stats {
    u64 rx_packets;
    u64 rx_bytes;
    u64 tx_packets;
    u64 tx_bytes;
    struct u64_stats_sync syncp;
    u32 rx_dropped;
    u32 tx_dropped;
    u32 rx_frame_errors;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct tun_pcpu_stats {
    u64 rx_packets;
    u64 rx_bytes;
    u64 tx_packets;
    u64 tx_bytes;
    struct u64_stats_sync syncp;
    u32 rx_dropped;
    u32 tx_dropped;
    u32 rx_frame_errors;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct tun_pcpu_stats {
    u64 rx_packets;
    u64 rx_bytes;
    u64 tx_packets;
    u64 tx_bytes;
    struct u64_stats_sync syncp;
    u32 rx_dropped;
    u32 tx_dropped;
    u32 rx_frame_errors;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct tun_pcpu_stats {
    u64 rx_packets;
    u64 rx_bytes;
    u64 tx_packets;
    u64 tx_bytes;
    struct u64_stats_sync syncp;
    u32 rx_dropped;
    u32 tx_dropped;
    u32 rx_frame_errors;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct tun_pcpu_stats {
    u64 rx_packets;
    u64 rx_bytes;
    u64 tx_packets;
    u64 tx_bytes;
    struct u64_stats_sync syncp;
    u32 rx_dropped;
    u32 tx_dropped;
    u32 rx_frame_errors;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct tun_pcpu_stats {
    u64_stats_t rx_packets;
    u64_stats_t rx_bytes;
    u64_stats_t tx_packets;
    u64_stats_t tx_bytes;
    struct u64_stats_sync syncp;
    u32 rx_dropped;
    u32 tx_dropped;
    u32 rx_frame_errors;
};
```
</details>
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
struct tun_pcpu_stats {
    u64 rx_packets;
    u64 rx_bytes;
    u64 tx_packets;
    u64 tx_bytes;
    struct u64_stats_sync syncp;
    u32 rx_dropped;
    u32 tx_dropped;
    u32 rx_frame_errors;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct tun_pcpu_stats {
    u64 rx_packets;
    u64 rx_bytes;
    u64 tx_packets;
    u64 tx_bytes;
    struct u64_stats_sync syncp;
    u32 rx_dropped;
    u32 tx_dropped;
    u32 rx_frame_errors;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct tun_pcpu_stats {
    u64 rx_packets;
    u64 rx_bytes;
    u64 tx_packets;
    u64 tx_bytes;
    struct u64_stats_sync syncp;
    u32 rx_dropped;
    u32 tx_dropped;
    u32 rx_frame_errors;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct tun_pcpu_stats {
    u64 rx_packets;
    u64 rx_bytes;
    u64 tx_packets;
    u64 tx_bytes;
    struct u64_stats_sync syncp;
    u32 rx_dropped;
    u32 tx_dropped;
    u32 rx_frame_errors;
};
```
</details>
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct tun_pcpu_stats {
    u64 rx_packets;
    u64 rx_bytes;
    u64 tx_packets;
    u64 tx_bytes;
    struct u64_stats_sync syncp;
    u32 rx_dropped;
    u32 tx_dropped;
    u32 rx_frame_errors;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct tun_pcpu_stats {
    u64 rx_packets;
    u64 rx_bytes;
    u64 tx_packets;
    u64 tx_bytes;
    struct u64_stats_sync syncp;
    u32 rx_dropped;
    u32 tx_dropped;
    u32 rx_frame_errors;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct tun_pcpu_stats {
    u64 rx_packets;
    u64 rx_bytes;
    u64 tx_packets;
    u64 tx_bytes;
    struct u64_stats_sync syncp;
    u32 rx_dropped;
    u32 tx_dropped;
    u32 rx_frame_errors;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct tun_pcpu_stats {
    u64 rx_packets;
    u64 rx_bytes;
    u64 tx_packets;
    u64 tx_bytes;
    struct u64_stats_sync syncp;
    u32 rx_dropped;
    u32 tx_dropped;
    u32 rx_frame_errors;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>u64 rx_packets</code> ➡️ <code>u64_stats_t rx_packets</code>
</li>
<li>
<b>Field type changed. </b>
<code>u64 rx_bytes</code> ➡️ <code>u64_stats_t rx_bytes</code>
</li>
<li>
<b>Field type changed. </b>
<code>u64 tx_packets</code> ➡️ <code>u64_stats_t tx_packets</code>
</li>
<li>
<b>Field type changed. </b>
<code>u64 tx_bytes</code> ➡️ <code>u64_stats_t tx_bytes</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>armhf</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>riscv64</code> ✅
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
No changes between <code>generic</code> and <code>aws</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
