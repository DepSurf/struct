# Struct: <code>net_device_stats</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct net_device_stats {
    long unsigned int rx_packets;
    long unsigned int tx_packets;
    long unsigned int rx_bytes;
    long unsigned int tx_bytes;
    long unsigned int rx_errors;
    long unsigned int tx_errors;
    long unsigned int rx_dropped;
    long unsigned int tx_dropped;
    long unsigned int multicast;
    long unsigned int collisions;
    long unsigned int rx_length_errors;
    long unsigned int rx_over_errors;
    long unsigned int rx_crc_errors;
    long unsigned int rx_frame_errors;
    long unsigned int rx_fifo_errors;
    long unsigned int rx_missed_errors;
    long unsigned int tx_aborted_errors;
    long unsigned int tx_carrier_errors;
    long unsigned int tx_fifo_errors;
    long unsigned int tx_heartbeat_errors;
    long unsigned int tx_window_errors;
    long unsigned int rx_compressed;
    long unsigned int tx_compressed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct net_device_stats {
    long unsigned int rx_packets;
    long unsigned int tx_packets;
    long unsigned int rx_bytes;
    long unsigned int tx_bytes;
    long unsigned int rx_errors;
    long unsigned int tx_errors;
    long unsigned int rx_dropped;
    long unsigned int tx_dropped;
    long unsigned int multicast;
    long unsigned int collisions;
    long unsigned int rx_length_errors;
    long unsigned int rx_over_errors;
    long unsigned int rx_crc_errors;
    long unsigned int rx_frame_errors;
    long unsigned int rx_fifo_errors;
    long unsigned int rx_missed_errors;
    long unsigned int tx_aborted_errors;
    long unsigned int tx_carrier_errors;
    long unsigned int tx_fifo_errors;
    long unsigned int tx_heartbeat_errors;
    long unsigned int tx_window_errors;
    long unsigned int rx_compressed;
    long unsigned int tx_compressed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct net_device_stats {
    long unsigned int rx_packets;
    long unsigned int tx_packets;
    long unsigned int rx_bytes;
    long unsigned int tx_bytes;
    long unsigned int rx_errors;
    long unsigned int tx_errors;
    long unsigned int rx_dropped;
    long unsigned int tx_dropped;
    long unsigned int multicast;
    long unsigned int collisions;
    long unsigned int rx_length_errors;
    long unsigned int rx_over_errors;
    long unsigned int rx_crc_errors;
    long unsigned int rx_frame_errors;
    long unsigned int rx_fifo_errors;
    long unsigned int rx_missed_errors;
    long unsigned int tx_aborted_errors;
    long unsigned int tx_carrier_errors;
    long unsigned int tx_fifo_errors;
    long unsigned int tx_heartbeat_errors;
    long unsigned int tx_window_errors;
    long unsigned int rx_compressed;
    long unsigned int tx_compressed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct net_device_stats {
    long unsigned int rx_packets;
    long unsigned int tx_packets;
    long unsigned int rx_bytes;
    long unsigned int tx_bytes;
    long unsigned int rx_errors;
    long unsigned int tx_errors;
    long unsigned int rx_dropped;
    long unsigned int tx_dropped;
    long unsigned int multicast;
    long unsigned int collisions;
    long unsigned int rx_length_errors;
    long unsigned int rx_over_errors;
    long unsigned int rx_crc_errors;
    long unsigned int rx_frame_errors;
    long unsigned int rx_fifo_errors;
    long unsigned int rx_missed_errors;
    long unsigned int tx_aborted_errors;
    long unsigned int tx_carrier_errors;
    long unsigned int tx_fifo_errors;
    long unsigned int tx_heartbeat_errors;
    long unsigned int tx_window_errors;
    long unsigned int rx_compressed;
    long unsigned int tx_compressed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct net_device_stats {
    long unsigned int rx_packets;
    long unsigned int tx_packets;
    long unsigned int rx_bytes;
    long unsigned int tx_bytes;
    long unsigned int rx_errors;
    long unsigned int tx_errors;
    long unsigned int rx_dropped;
    long unsigned int tx_dropped;
    long unsigned int multicast;
    long unsigned int collisions;
    long unsigned int rx_length_errors;
    long unsigned int rx_over_errors;
    long unsigned int rx_crc_errors;
    long unsigned int rx_frame_errors;
    long unsigned int rx_fifo_errors;
    long unsigned int rx_missed_errors;
    long unsigned int tx_aborted_errors;
    long unsigned int tx_carrier_errors;
    long unsigned int tx_fifo_errors;
    long unsigned int tx_heartbeat_errors;
    long unsigned int tx_window_errors;
    long unsigned int rx_compressed;
    long unsigned int tx_compressed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct net_device_stats {
    long unsigned int rx_packets;
    long unsigned int tx_packets;
    long unsigned int rx_bytes;
    long unsigned int tx_bytes;
    long unsigned int rx_errors;
    long unsigned int tx_errors;
    long unsigned int rx_dropped;
    long unsigned int tx_dropped;
    long unsigned int multicast;
    long unsigned int collisions;
    long unsigned int rx_length_errors;
    long unsigned int rx_over_errors;
    long unsigned int rx_crc_errors;
    long unsigned int rx_frame_errors;
    long unsigned int rx_fifo_errors;
    long unsigned int rx_missed_errors;
    long unsigned int tx_aborted_errors;
    long unsigned int tx_carrier_errors;
    long unsigned int tx_fifo_errors;
    long unsigned int tx_heartbeat_errors;
    long unsigned int tx_window_errors;
    long unsigned int rx_compressed;
    long unsigned int tx_compressed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct net_device_stats {
    long unsigned int rx_packets;
    long unsigned int tx_packets;
    long unsigned int rx_bytes;
    long unsigned int tx_bytes;
    long unsigned int rx_errors;
    long unsigned int tx_errors;
    long unsigned int rx_dropped;
    long unsigned int tx_dropped;
    long unsigned int multicast;
    long unsigned int collisions;
    long unsigned int rx_length_errors;
    long unsigned int rx_over_errors;
    long unsigned int rx_crc_errors;
    long unsigned int rx_frame_errors;
    long unsigned int rx_fifo_errors;
    long unsigned int rx_missed_errors;
    long unsigned int tx_aborted_errors;
    long unsigned int tx_carrier_errors;
    long unsigned int tx_fifo_errors;
    long unsigned int tx_heartbeat_errors;
    long unsigned int tx_window_errors;
    long unsigned int rx_compressed;
    long unsigned int tx_compressed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct net_device_stats {
    long unsigned int rx_packets;
    long unsigned int tx_packets;
    long unsigned int rx_bytes;
    long unsigned int tx_bytes;
    long unsigned int rx_errors;
    long unsigned int tx_errors;
    long unsigned int rx_dropped;
    long unsigned int tx_dropped;
    long unsigned int multicast;
    long unsigned int collisions;
    long unsigned int rx_length_errors;
    long unsigned int rx_over_errors;
    long unsigned int rx_crc_errors;
    long unsigned int rx_frame_errors;
    long unsigned int rx_fifo_errors;
    long unsigned int rx_missed_errors;
    long unsigned int tx_aborted_errors;
    long unsigned int tx_carrier_errors;
    long unsigned int tx_fifo_errors;
    long unsigned int tx_heartbeat_errors;
    long unsigned int tx_window_errors;
    long unsigned int rx_compressed;
    long unsigned int tx_compressed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct net_device_stats {
    long unsigned int rx_packets;
    long unsigned int tx_packets;
    long unsigned int rx_bytes;
    long unsigned int tx_bytes;
    long unsigned int rx_errors;
    long unsigned int tx_errors;
    long unsigned int rx_dropped;
    long unsigned int tx_dropped;
    long unsigned int multicast;
    long unsigned int collisions;
    long unsigned int rx_length_errors;
    long unsigned int rx_over_errors;
    long unsigned int rx_crc_errors;
    long unsigned int rx_frame_errors;
    long unsigned int rx_fifo_errors;
    long unsigned int rx_missed_errors;
    long unsigned int tx_aborted_errors;
    long unsigned int tx_carrier_errors;
    long unsigned int tx_fifo_errors;
    long unsigned int tx_heartbeat_errors;
    long unsigned int tx_window_errors;
    long unsigned int rx_compressed;
    long unsigned int tx_compressed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct net_device_stats {
    long unsigned int rx_packets;
    long unsigned int tx_packets;
    long unsigned int rx_bytes;
    long unsigned int tx_bytes;
    long unsigned int rx_errors;
    long unsigned int tx_errors;
    long unsigned int rx_dropped;
    long unsigned int tx_dropped;
    long unsigned int multicast;
    long unsigned int collisions;
    long unsigned int rx_length_errors;
    long unsigned int rx_over_errors;
    long unsigned int rx_crc_errors;
    long unsigned int rx_frame_errors;
    long unsigned int rx_fifo_errors;
    long unsigned int rx_missed_errors;
    long unsigned int tx_aborted_errors;
    long unsigned int tx_carrier_errors;
    long unsigned int tx_fifo_errors;
    long unsigned int tx_heartbeat_errors;
    long unsigned int tx_window_errors;
    long unsigned int rx_compressed;
    long unsigned int tx_compressed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct net_device_stats {
    long unsigned int rx_packets;
    long unsigned int tx_packets;
    long unsigned int rx_bytes;
    long unsigned int tx_bytes;
    long unsigned int rx_errors;
    long unsigned int tx_errors;
    long unsigned int rx_dropped;
    long unsigned int tx_dropped;
    long unsigned int multicast;
    long unsigned int collisions;
    long unsigned int rx_length_errors;
    long unsigned int rx_over_errors;
    long unsigned int rx_crc_errors;
    long unsigned int rx_frame_errors;
    long unsigned int rx_fifo_errors;
    long unsigned int rx_missed_errors;
    long unsigned int tx_aborted_errors;
    long unsigned int tx_carrier_errors;
    long unsigned int tx_fifo_errors;
    long unsigned int tx_heartbeat_errors;
    long unsigned int tx_window_errors;
    long unsigned int rx_compressed;
    long unsigned int tx_compressed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct net_device_stats {
    long unsigned int rx_packets;
    long unsigned int tx_packets;
    long unsigned int rx_bytes;
    long unsigned int tx_bytes;
    long unsigned int rx_errors;
    long unsigned int tx_errors;
    long unsigned int rx_dropped;
    long unsigned int tx_dropped;
    long unsigned int multicast;
    long unsigned int collisions;
    long unsigned int rx_length_errors;
    long unsigned int rx_over_errors;
    long unsigned int rx_crc_errors;
    long unsigned int rx_frame_errors;
    long unsigned int rx_fifo_errors;
    long unsigned int rx_missed_errors;
    long unsigned int tx_aborted_errors;
    long unsigned int tx_carrier_errors;
    long unsigned int tx_fifo_errors;
    long unsigned int tx_heartbeat_errors;
    long unsigned int tx_window_errors;
    long unsigned int rx_compressed;
    long unsigned int tx_compressed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct net_device_stats {
    long unsigned int rx_packets;
    long unsigned int tx_packets;
    long unsigned int rx_bytes;
    long unsigned int tx_bytes;
    long unsigned int rx_errors;
    long unsigned int tx_errors;
    long unsigned int rx_dropped;
    long unsigned int tx_dropped;
    long unsigned int multicast;
    long unsigned int collisions;
    long unsigned int rx_length_errors;
    long unsigned int rx_over_errors;
    long unsigned int rx_crc_errors;
    long unsigned int rx_frame_errors;
    long unsigned int rx_fifo_errors;
    long unsigned int rx_missed_errors;
    long unsigned int tx_aborted_errors;
    long unsigned int tx_carrier_errors;
    long unsigned int tx_fifo_errors;
    long unsigned int tx_heartbeat_errors;
    long unsigned int tx_window_errors;
    long unsigned int rx_compressed;
    long unsigned int tx_compressed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct net_device_stats {
    long unsigned int rx_packets;
    long unsigned int tx_packets;
    long unsigned int rx_bytes;
    long unsigned int tx_bytes;
    long unsigned int rx_errors;
    long unsigned int tx_errors;
    long unsigned int rx_dropped;
    long unsigned int tx_dropped;
    long unsigned int multicast;
    long unsigned int collisions;
    long unsigned int rx_length_errors;
    long unsigned int rx_over_errors;
    long unsigned int rx_crc_errors;
    long unsigned int rx_frame_errors;
    long unsigned int rx_fifo_errors;
    long unsigned int rx_missed_errors;
    long unsigned int tx_aborted_errors;
    long unsigned int tx_carrier_errors;
    long unsigned int tx_fifo_errors;
    long unsigned int tx_heartbeat_errors;
    long unsigned int tx_window_errors;
    long unsigned int rx_compressed;
    long unsigned int tx_compressed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct net_device_stats {
    long unsigned int rx_packets;
    atomic_long_t __rx_packets;
    long unsigned int tx_packets;
    atomic_long_t __tx_packets;
    long unsigned int rx_bytes;
    atomic_long_t __rx_bytes;
    long unsigned int tx_bytes;
    atomic_long_t __tx_bytes;
    long unsigned int rx_errors;
    atomic_long_t __rx_errors;
    long unsigned int tx_errors;
    atomic_long_t __tx_errors;
    long unsigned int rx_dropped;
    atomic_long_t __rx_dropped;
    long unsigned int tx_dropped;
    atomic_long_t __tx_dropped;
    long unsigned int multicast;
    atomic_long_t __multicast;
    long unsigned int collisions;
    atomic_long_t __collisions;
    long unsigned int rx_length_errors;
    atomic_long_t __rx_length_errors;
    long unsigned int rx_over_errors;
    atomic_long_t __rx_over_errors;
    long unsigned int rx_crc_errors;
    atomic_long_t __rx_crc_errors;
    long unsigned int rx_frame_errors;
    atomic_long_t __rx_frame_errors;
    long unsigned int rx_fifo_errors;
    atomic_long_t __rx_fifo_errors;
    long unsigned int rx_missed_errors;
    atomic_long_t __rx_missed_errors;
    long unsigned int tx_aborted_errors;
    atomic_long_t __tx_aborted_errors;
    long unsigned int tx_carrier_errors;
    atomic_long_t __tx_carrier_errors;
    long unsigned int tx_fifo_errors;
    atomic_long_t __tx_fifo_errors;
    long unsigned int tx_heartbeat_errors;
    atomic_long_t __tx_heartbeat_errors;
    long unsigned int tx_window_errors;
    atomic_long_t __tx_window_errors;
    long unsigned int rx_compressed;
    atomic_long_t __rx_compressed;
    long unsigned int tx_compressed;
    atomic_long_t __tx_compressed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct net_device_stats {
    long unsigned int rx_packets;
    atomic_long_t __rx_packets;
    long unsigned int tx_packets;
    atomic_long_t __tx_packets;
    long unsigned int rx_bytes;
    atomic_long_t __rx_bytes;
    long unsigned int tx_bytes;
    atomic_long_t __tx_bytes;
    long unsigned int rx_errors;
    atomic_long_t __rx_errors;
    long unsigned int tx_errors;
    atomic_long_t __tx_errors;
    long unsigned int rx_dropped;
    atomic_long_t __rx_dropped;
    long unsigned int tx_dropped;
    atomic_long_t __tx_dropped;
    long unsigned int multicast;
    atomic_long_t __multicast;
    long unsigned int collisions;
    atomic_long_t __collisions;
    long unsigned int rx_length_errors;
    atomic_long_t __rx_length_errors;
    long unsigned int rx_over_errors;
    atomic_long_t __rx_over_errors;
    long unsigned int rx_crc_errors;
    atomic_long_t __rx_crc_errors;
    long unsigned int rx_frame_errors;
    atomic_long_t __rx_frame_errors;
    long unsigned int rx_fifo_errors;
    atomic_long_t __rx_fifo_errors;
    long unsigned int rx_missed_errors;
    atomic_long_t __rx_missed_errors;
    long unsigned int tx_aborted_errors;
    atomic_long_t __tx_aborted_errors;
    long unsigned int tx_carrier_errors;
    atomic_long_t __tx_carrier_errors;
    long unsigned int tx_fifo_errors;
    atomic_long_t __tx_fifo_errors;
    long unsigned int tx_heartbeat_errors;
    atomic_long_t __tx_heartbeat_errors;
    long unsigned int tx_window_errors;
    atomic_long_t __tx_window_errors;
    long unsigned int rx_compressed;
    atomic_long_t __rx_compressed;
    long unsigned int tx_compressed;
    atomic_long_t __tx_compressed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct net_device_stats {
    long unsigned int rx_packets;
    atomic_long_t __rx_packets;
    long unsigned int tx_packets;
    atomic_long_t __tx_packets;
    long unsigned int rx_bytes;
    atomic_long_t __rx_bytes;
    long unsigned int tx_bytes;
    atomic_long_t __tx_bytes;
    long unsigned int rx_errors;
    atomic_long_t __rx_errors;
    long unsigned int tx_errors;
    atomic_long_t __tx_errors;
    long unsigned int rx_dropped;
    atomic_long_t __rx_dropped;
    long unsigned int tx_dropped;
    atomic_long_t __tx_dropped;
    long unsigned int multicast;
    atomic_long_t __multicast;
    long unsigned int collisions;
    atomic_long_t __collisions;
    long unsigned int rx_length_errors;
    atomic_long_t __rx_length_errors;
    long unsigned int rx_over_errors;
    atomic_long_t __rx_over_errors;
    long unsigned int rx_crc_errors;
    atomic_long_t __rx_crc_errors;
    long unsigned int rx_frame_errors;
    atomic_long_t __rx_frame_errors;
    long unsigned int rx_fifo_errors;
    atomic_long_t __rx_fifo_errors;
    long unsigned int rx_missed_errors;
    atomic_long_t __rx_missed_errors;
    long unsigned int tx_aborted_errors;
    atomic_long_t __tx_aborted_errors;
    long unsigned int tx_carrier_errors;
    atomic_long_t __tx_carrier_errors;
    long unsigned int tx_fifo_errors;
    atomic_long_t __tx_fifo_errors;
    long unsigned int tx_heartbeat_errors;
    atomic_long_t __tx_heartbeat_errors;
    long unsigned int tx_window_errors;
    atomic_long_t __tx_window_errors;
    long unsigned int rx_compressed;
    atomic_long_t __rx_compressed;
    long unsigned int tx_compressed;
    atomic_long_t __tx_compressed;
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct net_device_stats {
    long unsigned int rx_packets;
    long unsigned int tx_packets;
    long unsigned int rx_bytes;
    long unsigned int tx_bytes;
    long unsigned int rx_errors;
    long unsigned int tx_errors;
    long unsigned int rx_dropped;
    long unsigned int tx_dropped;
    long unsigned int multicast;
    long unsigned int collisions;
    long unsigned int rx_length_errors;
    long unsigned int rx_over_errors;
    long unsigned int rx_crc_errors;
    long unsigned int rx_frame_errors;
    long unsigned int rx_fifo_errors;
    long unsigned int rx_missed_errors;
    long unsigned int tx_aborted_errors;
    long unsigned int tx_carrier_errors;
    long unsigned int tx_fifo_errors;
    long unsigned int tx_heartbeat_errors;
    long unsigned int tx_window_errors;
    long unsigned int rx_compressed;
    long unsigned int tx_compressed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct net_device_stats {
    long unsigned int rx_packets;
    long unsigned int tx_packets;
    long unsigned int rx_bytes;
    long unsigned int tx_bytes;
    long unsigned int rx_errors;
    long unsigned int tx_errors;
    long unsigned int rx_dropped;
    long unsigned int tx_dropped;
    long unsigned int multicast;
    long unsigned int collisions;
    long unsigned int rx_length_errors;
    long unsigned int rx_over_errors;
    long unsigned int rx_crc_errors;
    long unsigned int rx_frame_errors;
    long unsigned int rx_fifo_errors;
    long unsigned int rx_missed_errors;
    long unsigned int tx_aborted_errors;
    long unsigned int tx_carrier_errors;
    long unsigned int tx_fifo_errors;
    long unsigned int tx_heartbeat_errors;
    long unsigned int tx_window_errors;
    long unsigned int rx_compressed;
    long unsigned int tx_compressed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct net_device_stats {
    long unsigned int rx_packets;
    long unsigned int tx_packets;
    long unsigned int rx_bytes;
    long unsigned int tx_bytes;
    long unsigned int rx_errors;
    long unsigned int tx_errors;
    long unsigned int rx_dropped;
    long unsigned int tx_dropped;
    long unsigned int multicast;
    long unsigned int collisions;
    long unsigned int rx_length_errors;
    long unsigned int rx_over_errors;
    long unsigned int rx_crc_errors;
    long unsigned int rx_frame_errors;
    long unsigned int rx_fifo_errors;
    long unsigned int rx_missed_errors;
    long unsigned int tx_aborted_errors;
    long unsigned int tx_carrier_errors;
    long unsigned int tx_fifo_errors;
    long unsigned int tx_heartbeat_errors;
    long unsigned int tx_window_errors;
    long unsigned int rx_compressed;
    long unsigned int tx_compressed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct net_device_stats {
    long unsigned int rx_packets;
    long unsigned int tx_packets;
    long unsigned int rx_bytes;
    long unsigned int tx_bytes;
    long unsigned int rx_errors;
    long unsigned int tx_errors;
    long unsigned int rx_dropped;
    long unsigned int tx_dropped;
    long unsigned int multicast;
    long unsigned int collisions;
    long unsigned int rx_length_errors;
    long unsigned int rx_over_errors;
    long unsigned int rx_crc_errors;
    long unsigned int rx_frame_errors;
    long unsigned int rx_fifo_errors;
    long unsigned int rx_missed_errors;
    long unsigned int tx_aborted_errors;
    long unsigned int tx_carrier_errors;
    long unsigned int tx_fifo_errors;
    long unsigned int tx_heartbeat_errors;
    long unsigned int tx_window_errors;
    long unsigned int rx_compressed;
    long unsigned int tx_compressed;
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
struct net_device_stats {
    long unsigned int rx_packets;
    long unsigned int tx_packets;
    long unsigned int rx_bytes;
    long unsigned int tx_bytes;
    long unsigned int rx_errors;
    long unsigned int tx_errors;
    long unsigned int rx_dropped;
    long unsigned int tx_dropped;
    long unsigned int multicast;
    long unsigned int collisions;
    long unsigned int rx_length_errors;
    long unsigned int rx_over_errors;
    long unsigned int rx_crc_errors;
    long unsigned int rx_frame_errors;
    long unsigned int rx_fifo_errors;
    long unsigned int rx_missed_errors;
    long unsigned int tx_aborted_errors;
    long unsigned int tx_carrier_errors;
    long unsigned int tx_fifo_errors;
    long unsigned int tx_heartbeat_errors;
    long unsigned int tx_window_errors;
    long unsigned int rx_compressed;
    long unsigned int tx_compressed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct net_device_stats {
    long unsigned int rx_packets;
    long unsigned int tx_packets;
    long unsigned int rx_bytes;
    long unsigned int tx_bytes;
    long unsigned int rx_errors;
    long unsigned int tx_errors;
    long unsigned int rx_dropped;
    long unsigned int tx_dropped;
    long unsigned int multicast;
    long unsigned int collisions;
    long unsigned int rx_length_errors;
    long unsigned int rx_over_errors;
    long unsigned int rx_crc_errors;
    long unsigned int rx_frame_errors;
    long unsigned int rx_fifo_errors;
    long unsigned int rx_missed_errors;
    long unsigned int tx_aborted_errors;
    long unsigned int tx_carrier_errors;
    long unsigned int tx_fifo_errors;
    long unsigned int tx_heartbeat_errors;
    long unsigned int tx_window_errors;
    long unsigned int rx_compressed;
    long unsigned int tx_compressed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct net_device_stats {
    long unsigned int rx_packets;
    long unsigned int tx_packets;
    long unsigned int rx_bytes;
    long unsigned int tx_bytes;
    long unsigned int rx_errors;
    long unsigned int tx_errors;
    long unsigned int rx_dropped;
    long unsigned int tx_dropped;
    long unsigned int multicast;
    long unsigned int collisions;
    long unsigned int rx_length_errors;
    long unsigned int rx_over_errors;
    long unsigned int rx_crc_errors;
    long unsigned int rx_frame_errors;
    long unsigned int rx_fifo_errors;
    long unsigned int rx_missed_errors;
    long unsigned int tx_aborted_errors;
    long unsigned int tx_carrier_errors;
    long unsigned int tx_fifo_errors;
    long unsigned int tx_heartbeat_errors;
    long unsigned int tx_window_errors;
    long unsigned int rx_compressed;
    long unsigned int tx_compressed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct net_device_stats {
    long unsigned int rx_packets;
    long unsigned int tx_packets;
    long unsigned int rx_bytes;
    long unsigned int tx_bytes;
    long unsigned int rx_errors;
    long unsigned int tx_errors;
    long unsigned int rx_dropped;
    long unsigned int tx_dropped;
    long unsigned int multicast;
    long unsigned int collisions;
    long unsigned int rx_length_errors;
    long unsigned int rx_over_errors;
    long unsigned int rx_crc_errors;
    long unsigned int rx_frame_errors;
    long unsigned int rx_fifo_errors;
    long unsigned int rx_missed_errors;
    long unsigned int tx_aborted_errors;
    long unsigned int tx_carrier_errors;
    long unsigned int tx_fifo_errors;
    long unsigned int tx_heartbeat_errors;
    long unsigned int tx_window_errors;
    long unsigned int rx_compressed;
    long unsigned int tx_compressed;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.4</code> and <code>4.8</code> ✅
</li>
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
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>atomic_long_t __rx_packets</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t __tx_packets</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t __rx_bytes</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t __tx_bytes</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t __rx_errors</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t __tx_errors</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t __rx_dropped</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t __tx_dropped</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t __multicast</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t __collisions</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t __rx_length_errors</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t __rx_over_errors</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t __rx_crc_errors</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t __rx_frame_errors</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t __rx_fifo_errors</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t __rx_missed_errors</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t __tx_aborted_errors</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t __tx_carrier_errors</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t __tx_fifo_errors</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t __tx_heartbeat_errors</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t __tx_window_errors</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t __rx_compressed</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t __tx_compressed</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
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
