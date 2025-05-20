# Struct: <code>mptcp_info</code>

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
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mptcp_info {
    __u8 mptcpi_subflows;
    __u8 mptcpi_add_addr_signal;
    __u8 mptcpi_add_addr_accepted;
    __u8 mptcpi_subflows_max;
    __u8 mptcpi_add_addr_signal_max;
    __u8 mptcpi_add_addr_accepted_max;
    __u32 mptcpi_flags;
    __u32 mptcpi_token;
    __u64 mptcpi_write_seq;
    __u64 mptcpi_snd_una;
    __u64 mptcpi_rcv_nxt;
    __u8 mptcpi_local_addr_used;
    __u8 mptcpi_local_addr_max;
    __u8 mptcpi_csum_enabled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mptcp_info {
    __u8 mptcpi_subflows;
    __u8 mptcpi_add_addr_signal;
    __u8 mptcpi_add_addr_accepted;
    __u8 mptcpi_subflows_max;
    __u8 mptcpi_add_addr_signal_max;
    __u8 mptcpi_add_addr_accepted_max;
    __u32 mptcpi_flags;
    __u32 mptcpi_token;
    __u64 mptcpi_write_seq;
    __u64 mptcpi_snd_una;
    __u64 mptcpi_rcv_nxt;
    __u8 mptcpi_local_addr_used;
    __u8 mptcpi_local_addr_max;
    __u8 mptcpi_csum_enabled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mptcp_info {
    __u8 mptcpi_subflows;
    __u8 mptcpi_add_addr_signal;
    __u8 mptcpi_add_addr_accepted;
    __u8 mptcpi_subflows_max;
    __u8 mptcpi_add_addr_signal_max;
    __u8 mptcpi_add_addr_accepted_max;
    __u32 mptcpi_flags;
    __u32 mptcpi_token;
    __u64 mptcpi_write_seq;
    __u64 mptcpi_snd_una;
    __u64 mptcpi_rcv_nxt;
    __u8 mptcpi_local_addr_used;
    __u8 mptcpi_local_addr_max;
    __u8 mptcpi_csum_enabled;
    __u32 mptcpi_retransmits;
    __u64 mptcpi_bytes_retrans;
    __u64 mptcpi_bytes_sent;
    __u64 mptcpi_bytes_received;
    __u64 mptcpi_bytes_acked;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mptcp_info {
    __u8 mptcpi_subflows;
    __u8 mptcpi_add_addr_signal;
    __u8 mptcpi_add_addr_accepted;
    __u8 mptcpi_subflows_max;
    __u8 mptcpi_add_addr_signal_max;
    __u8 mptcpi_add_addr_accepted_max;
    __u32 mptcpi_flags;
    __u32 mptcpi_token;
    __u64 mptcpi_write_seq;
    __u64 mptcpi_snd_una;
    __u64 mptcpi_rcv_nxt;
    __u8 mptcpi_local_addr_used;
    __u8 mptcpi_local_addr_max;
    __u8 mptcpi_csum_enabled;
    __u32 mptcpi_retransmits;
    __u64 mptcpi_bytes_retrans;
    __u64 mptcpi_bytes_sent;
    __u64 mptcpi_bytes_received;
    __u64 mptcpi_bytes_acked;
    __u8 mptcpi_subflows_total;
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
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u32 mptcpi_retransmits</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 mptcpi_bytes_retrans</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 mptcpi_bytes_sent</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 mptcpi_bytes_received</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 mptcpi_bytes_acked</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u8 mptcpi_subflows_total</code>
</li>
</ul>
</details>
</li>
</ul>
