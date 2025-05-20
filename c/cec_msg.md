# Struct: <code>cec_msg</code>

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
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct cec_msg {
    __u64 tx_ts;
    __u64 rx_ts;
    __u32 len;
    __u32 timeout;
    __u32 sequence;
    __u32 flags;
    __u8 msg[16];
    __u8 reply;
    __u8 rx_status;
    __u8 tx_status;
    __u8 tx_arb_lost_cnt;
    __u8 tx_nack_cnt;
    __u8 tx_low_drive_cnt;
    __u8 tx_error_cnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct cec_msg {
    __u64 tx_ts;
    __u64 rx_ts;
    __u32 len;
    __u32 timeout;
    __u32 sequence;
    __u32 flags;
    __u8 msg[16];
    __u8 reply;
    __u8 rx_status;
    __u8 tx_status;
    __u8 tx_arb_lost_cnt;
    __u8 tx_nack_cnt;
    __u8 tx_low_drive_cnt;
    __u8 tx_error_cnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct cec_msg {
    __u64 tx_ts;
    __u64 rx_ts;
    __u32 len;
    __u32 timeout;
    __u32 sequence;
    __u32 flags;
    __u8 msg[16];
    __u8 reply;
    __u8 rx_status;
    __u8 tx_status;
    __u8 tx_arb_lost_cnt;
    __u8 tx_nack_cnt;
    __u8 tx_low_drive_cnt;
    __u8 tx_error_cnt;
};
```
</details>
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
struct cec_msg {
    __u64 tx_ts;
    __u64 rx_ts;
    __u32 len;
    __u32 timeout;
    __u32 sequence;
    __u32 flags;
    __u8 msg[16];
    __u8 reply;
    __u8 rx_status;
    __u8 tx_status;
    __u8 tx_arb_lost_cnt;
    __u8 tx_nack_cnt;
    __u8 tx_low_drive_cnt;
    __u8 tx_error_cnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct cec_msg {
    __u64 tx_ts;
    __u64 rx_ts;
    __u32 len;
    __u32 timeout;
    __u32 sequence;
    __u32 flags;
    __u8 msg[16];
    __u8 reply;
    __u8 rx_status;
    __u8 tx_status;
    __u8 tx_arb_lost_cnt;
    __u8 tx_nack_cnt;
    __u8 tx_low_drive_cnt;
    __u8 tx_error_cnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct cec_msg {
    __u64 tx_ts;
    __u64 rx_ts;
    __u32 len;
    __u32 timeout;
    __u32 sequence;
    __u32 flags;
    __u8 msg[16];
    __u8 reply;
    __u8 rx_status;
    __u8 tx_status;
    __u8 tx_arb_lost_cnt;
    __u8 tx_nack_cnt;
    __u8 tx_low_drive_cnt;
    __u8 tx_error_cnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct cec_msg {
    __u64 tx_ts;
    __u64 rx_ts;
    __u32 len;
    __u32 timeout;
    __u32 sequence;
    __u32 flags;
    __u8 msg[16];
    __u8 reply;
    __u8 rx_status;
    __u8 tx_status;
    __u8 tx_arb_lost_cnt;
    __u8 tx_nack_cnt;
    __u8 tx_low_drive_cnt;
    __u8 tx_error_cnt;
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
struct cec_msg {
    __u64 tx_ts;
    __u64 rx_ts;
    __u32 len;
    __u32 timeout;
    __u32 sequence;
    __u32 flags;
    __u8 msg[16];
    __u8 reply;
    __u8 rx_status;
    __u8 tx_status;
    __u8 tx_arb_lost_cnt;
    __u8 tx_nack_cnt;
    __u8 tx_low_drive_cnt;
    __u8 tx_error_cnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct cec_msg {
    __u64 tx_ts;
    __u64 rx_ts;
    __u32 len;
    __u32 timeout;
    __u32 sequence;
    __u32 flags;
    __u8 msg[16];
    __u8 reply;
    __u8 rx_status;
    __u8 tx_status;
    __u8 tx_arb_lost_cnt;
    __u8 tx_nack_cnt;
    __u8 tx_low_drive_cnt;
    __u8 tx_error_cnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct cec_msg {
    __u64 tx_ts;
    __u64 rx_ts;
    __u32 len;
    __u32 timeout;
    __u32 sequence;
    __u32 flags;
    __u8 msg[16];
    __u8 reply;
    __u8 rx_status;
    __u8 tx_status;
    __u8 tx_arb_lost_cnt;
    __u8 tx_nack_cnt;
    __u8 tx_low_drive_cnt;
    __u8 tx_error_cnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cec_msg {
    __u64 tx_ts;
    __u64 rx_ts;
    __u32 len;
    __u32 timeout;
    __u32 sequence;
    __u32 flags;
    __u8 msg[16];
    __u8 reply;
    __u8 rx_status;
    __u8 tx_status;
    __u8 tx_arb_lost_cnt;
    __u8 tx_nack_cnt;
    __u8 tx_low_drive_cnt;
    __u8 tx_error_cnt;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
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
