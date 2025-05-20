# Struct: <code>mptcp_options_received</code>

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
struct mptcp_options_received {
    u64 sndr_key;
    u64 rcvr_key;
    u64 data_ack;
    u64 data_seq;
    u32 subflow_seq;
    u16 data_len;
    u16 mp_capable;
    u16 mp_join;
    u16 dss;
    u16 add_addr;
    u16 rm_addr;
    u16 family;
    u16 echo;
    u16 backup;
    u32 token;
    u32 nonce;
    u64 thmac;
    u8 hmac[20];
    u8 join_id;
    u8 use_map;
    u8 dsn64;
    u8 data_fin;
    u8 use_ack;
    u8 ack64;
    u8 mpc_map;
    u8 __unused;
    u8 addr_id;
    u8 rm_id;
    struct in_addr addr;
    struct in6_addr addr6;
    u64 ahmac;
    u16 port;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mptcp_options_received {
    u64 sndr_key;
    u64 rcvr_key;
    u64 data_ack;
    u64 data_seq;
    u32 subflow_seq;
    u16 data_len;
    u16 mp_capable;
    u16 mp_join;
    u16 fastclose;
    u16 dss;
    u16 add_addr;
    u16 rm_addr;
    u16 family;
    u16 echo;
    u16 backup;
    u32 token;
    u32 nonce;
    u64 thmac;
    u8 hmac[20];
    u8 join_id;
    u8 use_map;
    u8 dsn64;
    u8 data_fin;
    u8 use_ack;
    u8 ack64;
    u8 mpc_map;
    u8 __unused;
    u8 addr_id;
    u8 rm_id;
    struct in_addr addr;
    struct in6_addr addr6;
    u64 ahmac;
    u16 port;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mptcp_options_received {
    u64 sndr_key;
    u64 rcvr_key;
    u64 data_ack;
    u64 data_seq;
    u32 subflow_seq;
    u16 data_len;
    u16 mp_capable;
    u16 mp_join;
    u16 fastclose;
    u16 reset;
    u16 dss;
    u16 add_addr;
    u16 rm_addr;
    u16 mp_prio;
    u16 echo;
    u16 backup;
    u32 token;
    u32 nonce;
    u64 thmac;
    u8 hmac[20];
    u8 join_id;
    u8 use_map;
    u8 dsn64;
    u8 data_fin;
    u8 use_ack;
    u8 ack64;
    u8 mpc_map;
    u8 __unused;
    struct mptcp_addr_info addr;
    struct mptcp_rm_list rm_list;
    u64 ahmac;
    u8 reset_reason;
    u8 reset_transient;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mptcp_options_received {
    u64 sndr_key;
    u64 rcvr_key;
    u64 data_ack;
    u64 data_seq;
    u32 subflow_seq;
    u16 data_len;
    __sum16 csum;
    u16 suboptions;
    u32 token;
    u32 nonce;
    u16 use_map;
    u16 dsn64;
    u16 data_fin;
    u16 use_ack;
    u16 ack64;
    u16 mpc_map;
    u16 reset_reason;
    u16 reset_transient;
    u16 echo;
    u16 backup;
    u16 deny_join_id0;
    u16 __unused;
    u8 join_id;
    u64 thmac;
    u8 hmac[20];
    struct mptcp_addr_info addr;
    struct mptcp_rm_list rm_list;
    u64 ahmac;
    u64 fail_seq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mptcp_options_received {
    u64 sndr_key;
    u64 rcvr_key;
    u64 data_ack;
    u64 data_seq;
    u32 subflow_seq;
    u16 data_len;
    __sum16 csum;
    u16 suboptions;
    u32 token;
    u32 nonce;
    u16 use_map;
    u16 dsn64;
    u16 data_fin;
    u16 use_ack;
    u16 ack64;
    u16 mpc_map;
    u16 reset_reason;
    u16 reset_transient;
    u16 echo;
    u16 backup;
    u16 deny_join_id0;
    u16 __unused;
    u8 join_id;
    u64 thmac;
    u8 hmac[20];
    struct mptcp_addr_info addr;
    struct mptcp_rm_list rm_list;
    u64 ahmac;
    u64 fail_seq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mptcp_options_received {
    u64 sndr_key;
    u64 rcvr_key;
    u64 data_ack;
    u64 data_seq;
    u32 subflow_seq;
    u16 data_len;
    __sum16 csum;
    u16 suboptions;
    u32 token;
    u32 nonce;
    u16 use_map;
    u16 dsn64;
    u16 data_fin;
    u16 use_ack;
    u16 ack64;
    u16 mpc_map;
    u16 reset_reason;
    u16 reset_transient;
    u16 echo;
    u16 backup;
    u16 deny_join_id0;
    u16 __unused;
    u8 join_id;
    u64 thmac;
    u8 hmac[20];
    struct mptcp_addr_info addr;
    struct mptcp_rm_list rm_list;
    u64 ahmac;
    u64 fail_seq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mptcp_options_received {
    u64 sndr_key;
    u64 rcvr_key;
    u64 data_ack;
    u64 data_seq;
    u32 subflow_seq;
    u16 data_len;
    __sum16 csum;
    u16 suboptions;
    u32 token;
    u32 nonce;
    u16 use_map;
    u16 dsn64;
    u16 data_fin;
    u16 use_ack;
    u16 ack64;
    u16 mpc_map;
    u16 reset_reason;
    u16 reset_transient;
    u16 echo;
    u16 backup;
    u16 deny_join_id0;
    u16 __unused;
    u8 join_id;
    u64 thmac;
    u8 hmac[20];
    struct mptcp_addr_info addr;
    struct mptcp_rm_list rm_list;
    u64 ahmac;
    u64 fail_seq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mptcp_options_received {
    u64 sndr_key;
    u64 rcvr_key;
    u64 data_ack;
    u64 data_seq;
    u32 subflow_seq;
    u16 data_len;
    __sum16 csum;
    u16 suboptions;
    u32 token;
    u32 nonce;
    u16 use_map;
    u16 dsn64;
    u16 data_fin;
    u16 use_ack;
    u16 ack64;
    u16 mpc_map;
    u16 reset_reason;
    u16 reset_transient;
    u16 echo;
    u16 backup;
    u16 deny_join_id0;
    u16 __unused;
    u8 join_id;
    u64 thmac;
    u8 hmac[20];
    struct mptcp_addr_info addr;
    struct mptcp_rm_list rm_list;
    u64 ahmac;
    u64 fail_seq;
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
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 fastclose</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 reset</code>
</li>
<li>
<b>Field added. </b>
<code>u16 mp_prio</code>
</li>
<li>
<b>Field added. </b>
<code>struct mptcp_rm_list rm_list</code>
</li>
<li>
<b>Field added. </b>
<code>u8 reset_reason</code>
</li>
<li>
<b>Field added. </b>
<code>u8 reset_transient</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 family</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 addr_id</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 rm_id</code>
</li>
<li>
<b>Field removed. </b>
<code>struct in6_addr addr6</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 port</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct in_addr addr</code> ➡️ <code>struct mptcp_addr_info addr</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__sum16 csum</code>
</li>
<li>
<b>Field added. </b>
<code>u16 suboptions</code>
</li>
<li>
<b>Field added. </b>
<code>u16 deny_join_id0</code>
</li>
<li>
<b>Field added. </b>
<code>u64 fail_seq</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 mp_capable</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 mp_join</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 fastclose</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 reset</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 dss</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 add_addr</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 rm_addr</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 mp_prio</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 use_map</code> ➡️ <code>u16 use_map</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 dsn64</code> ➡️ <code>u16 dsn64</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 data_fin</code> ➡️ <code>u16 data_fin</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 use_ack</code> ➡️ <code>u16 use_ack</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 ack64</code> ➡️ <code>u16 ack64</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 mpc_map</code> ➡️ <code>u16 mpc_map</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 __unused</code> ➡️ <code>u16 __unused</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 reset_reason</code> ➡️ <code>u16 reset_reason</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 reset_transient</code> ➡️ <code>u16 reset_transient</code>
</li>
</ul>
</details>
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
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
