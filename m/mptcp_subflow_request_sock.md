# Struct: <code>mptcp_subflow_request_sock</code>

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
struct mptcp_subflow_request_sock {
    struct tcp_request_sock sk;
    u16 mp_capable;
    u16 mp_join;
    u16 backup;
    u8 local_id;
    u8 remote_id;
    u64 local_key;
    u64 idsn;
    u32 token;
    u32 ssn_offset;
    u64 thmac;
    u32 local_nonce;
    u32 remote_nonce;
    struct mptcp_sock *msk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mptcp_subflow_request_sock {
    struct tcp_request_sock sk;
    u16 mp_capable;
    u16 mp_join;
    u16 backup;
    u8 local_id;
    u8 remote_id;
    u64 local_key;
    u64 idsn;
    u32 token;
    u32 ssn_offset;
    u64 thmac;
    u32 local_nonce;
    u32 remote_nonce;
    struct mptcp_sock *msk;
    struct hlist_nulls_node token_node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mptcp_subflow_request_sock {
    struct tcp_request_sock sk;
    u16 mp_capable;
    u16 mp_join;
    u16 backup;
    u8 local_id;
    u8 remote_id;
    u64 local_key;
    u64 idsn;
    u32 token;
    u32 ssn_offset;
    u64 thmac;
    u32 local_nonce;
    u32 remote_nonce;
    struct mptcp_sock *msk;
    struct hlist_nulls_node token_node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mptcp_subflow_request_sock {
    struct tcp_request_sock sk;
    u16 mp_capable;
    u16 mp_join;
    u16 backup;
    u16 csum_reqd;
    u16 allow_join_id0;
    u8 local_id;
    u8 remote_id;
    u64 local_key;
    u64 idsn;
    u32 token;
    u32 ssn_offset;
    u64 thmac;
    u32 local_nonce;
    u32 remote_nonce;
    struct mptcp_sock *msk;
    struct hlist_nulls_node token_node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mptcp_subflow_request_sock {
    struct tcp_request_sock sk;
    u16 mp_capable;
    u16 mp_join;
    u16 backup;
    u16 csum_reqd;
    u16 allow_join_id0;
    u8 local_id;
    u8 remote_id;
    u64 local_key;
    u64 idsn;
    u32 token;
    u32 ssn_offset;
    u64 thmac;
    u32 local_nonce;
    u32 remote_nonce;
    struct mptcp_sock *msk;
    struct hlist_nulls_node token_node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mptcp_subflow_request_sock {
    struct tcp_request_sock sk;
    u16 mp_capable;
    u16 mp_join;
    u16 backup;
    u16 csum_reqd;
    u16 allow_join_id0;
    u8 local_id;
    u8 remote_id;
    u64 local_key;
    u64 idsn;
    u32 token;
    u32 ssn_offset;
    u64 thmac;
    u32 local_nonce;
    u32 remote_nonce;
    struct mptcp_sock *msk;
    struct hlist_nulls_node token_node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mptcp_subflow_request_sock {
    struct tcp_request_sock sk;
    u16 mp_capable;
    u16 mp_join;
    u16 backup;
    u16 csum_reqd;
    u16 allow_join_id0;
    u8 local_id;
    u8 remote_id;
    u64 local_key;
    u64 idsn;
    u32 token;
    u32 ssn_offset;
    u64 thmac;
    u32 local_nonce;
    u32 remote_nonce;
    struct mptcp_sock *msk;
    struct hlist_nulls_node token_node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mptcp_subflow_request_sock {
    struct tcp_request_sock sk;
    u16 mp_capable;
    u16 mp_join;
    u16 backup;
    u16 csum_reqd;
    u16 allow_join_id0;
    u8 local_id;
    u8 remote_id;
    u64 local_key;
    u64 idsn;
    u32 token;
    u32 ssn_offset;
    u64 thmac;
    u32 local_nonce;
    u32 remote_nonce;
    struct mptcp_sock *msk;
    struct hlist_nulls_node token_node;
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
<code>struct hlist_nulls_node token_node</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 csum_reqd</code>
</li>
<li>
<b>Field added. </b>
<code>u16 allow_join_id0</code>
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
