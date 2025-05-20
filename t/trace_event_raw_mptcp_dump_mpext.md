# Struct: <code>trace_event_raw_mptcp_dump_mpext</code>

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
struct trace_event_raw_mptcp_dump_mpext {
    struct trace_entry ent;
    u64 data_ack;
    u64 data_seq;
    u32 subflow_seq;
    u16 data_len;
    u8 use_map;
    u8 dsn64;
    u8 data_fin;
    u8 use_ack;
    u8 ack64;
    u8 mpc_map;
    u8 frozen;
    u8 reset_transient;
    u8 reset_reason;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct trace_event_raw_mptcp_dump_mpext {
    struct trace_entry ent;
    u64 data_ack;
    u64 data_seq;
    u32 subflow_seq;
    u16 data_len;
    u16 csum;
    u8 use_map;
    u8 dsn64;
    u8 data_fin;
    u8 use_ack;
    u8 ack64;
    u8 mpc_map;
    u8 frozen;
    u8 reset_transient;
    u8 reset_reason;
    u8 csum_reqd;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct trace_event_raw_mptcp_dump_mpext {
    struct trace_entry ent;
    u64 data_ack;
    u64 data_seq;
    u32 subflow_seq;
    u16 data_len;
    u16 csum;
    u8 use_map;
    u8 dsn64;
    u8 data_fin;
    u8 use_ack;
    u8 ack64;
    u8 mpc_map;
    u8 frozen;
    u8 reset_transient;
    u8 reset_reason;
    u8 csum_reqd;
    u8 infinite_map;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct trace_event_raw_mptcp_dump_mpext {
    struct trace_entry ent;
    u64 data_ack;
    u64 data_seq;
    u32 subflow_seq;
    u16 data_len;
    u16 csum;
    u8 use_map;
    u8 dsn64;
    u8 data_fin;
    u8 use_ack;
    u8 ack64;
    u8 mpc_map;
    u8 frozen;
    u8 reset_transient;
    u8 reset_reason;
    u8 csum_reqd;
    u8 infinite_map;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct trace_event_raw_mptcp_dump_mpext {
    struct trace_entry ent;
    u64 data_ack;
    u64 data_seq;
    u32 subflow_seq;
    u16 data_len;
    u16 csum;
    u8 use_map;
    u8 dsn64;
    u8 data_fin;
    u8 use_ack;
    u8 ack64;
    u8 mpc_map;
    u8 frozen;
    u8 reset_transient;
    u8 reset_reason;
    u8 csum_reqd;
    u8 infinite_map;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct trace_event_raw_mptcp_dump_mpext {
    struct trace_entry ent;
    u64 data_ack;
    u64 data_seq;
    u32 subflow_seq;
    u16 data_len;
    u16 csum;
    u8 use_map;
    u8 dsn64;
    u8 data_fin;
    u8 use_ack;
    u8 ack64;
    u8 mpc_map;
    u8 frozen;
    u8 reset_transient;
    u8 reset_reason;
    u8 csum_reqd;
    u8 infinite_map;
    char __data[0];
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
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 csum</code>
</li>
<li>
<b>Field added. </b>
<code>u8 csum_reqd</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 infinite_map</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
