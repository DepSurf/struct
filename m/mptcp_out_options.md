# Struct: <code>mptcp_out_options</code>

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
struct mptcp_out_options {
    u16 suboptions;
    u64 sndr_key;
    u64 rcvr_key;
    struct in_addr addr;
    struct in6_addr addr6;
    u8 addr_id;
    u64 ahmac;
    u8 rm_id;
    u8 join_id;
    u8 backup;
    u32 nonce;
    u64 thmac;
    u32 token;
    u8 hmac[20];
    struct mptcp_ext ext_copy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mptcp_out_options {
    u16 suboptions;
    u64 sndr_key;
    u64 rcvr_key;
    struct in_addr addr;
    struct in6_addr addr6;
    u8 addr_id;
    u16 port;
    u64 ahmac;
    u8 rm_id;
    u8 join_id;
    u8 backup;
    u32 nonce;
    u64 thmac;
    u32 token;
    u8 hmac[20];
    struct mptcp_ext ext_copy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mptcp_out_options {
    u16 suboptions;
    u64 sndr_key;
    u64 rcvr_key;
    u64 ahmac;
    struct mptcp_addr_info addr;
    struct mptcp_rm_list rm_list;
    u8 join_id;
    u8 backup;
    u8 reset_reason;
    u8 reset_transient;
    u32 nonce;
    u64 thmac;
    u32 token;
    u8 hmac[20];
    struct mptcp_ext ext_copy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mptcp_out_options {
    u16 suboptions;
    struct mptcp_rm_list rm_list;
    u8 join_id;
    u8 backup;
    u8 reset_reason;
    u8 reset_transient;
    u8 csum_reqd;
    u8 allow_join_id0;
    u64 sndr_key;
    u64 rcvr_key;
    u64 data_seq;
    u32 subflow_seq;
    u16 data_len;
    __sum16 csum;
    struct mptcp_addr_info addr;
    u64 ahmac;
    struct mptcp_ext ext_copy;
    u64 fail_seq;
    u32 nonce;
    u32 token;
    u64 thmac;
    u8 hmac[20];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mptcp_out_options {
    u16 suboptions;
    struct mptcp_rm_list rm_list;
    u8 join_id;
    u8 backup;
    u8 reset_reason;
    u8 reset_transient;
    u8 csum_reqd;
    u8 allow_join_id0;
    u64 sndr_key;
    u64 rcvr_key;
    u64 data_seq;
    u32 subflow_seq;
    u16 data_len;
    __sum16 csum;
    struct mptcp_addr_info addr;
    u64 ahmac;
    struct mptcp_ext ext_copy;
    u64 fail_seq;
    u32 nonce;
    u32 token;
    u64 thmac;
    u8 hmac[20];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mptcp_out_options {
    u16 suboptions;
    struct mptcp_rm_list rm_list;
    u8 join_id;
    u8 backup;
    u8 reset_reason;
    u8 reset_transient;
    u8 csum_reqd;
    u8 allow_join_id0;
    u64 sndr_key;
    u64 rcvr_key;
    u64 data_seq;
    u32 subflow_seq;
    u16 data_len;
    __sum16 csum;
    struct mptcp_addr_info addr;
    u64 ahmac;
    struct mptcp_ext ext_copy;
    u64 fail_seq;
    u32 nonce;
    u32 token;
    u64 thmac;
    u8 hmac[20];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mptcp_out_options {
    u16 suboptions;
    struct mptcp_rm_list rm_list;
    u8 join_id;
    u8 backup;
    u8 reset_reason;
    u8 reset_transient;
    u8 csum_reqd;
    u8 allow_join_id0;
    u64 sndr_key;
    u64 rcvr_key;
    u64 data_seq;
    u32 subflow_seq;
    u16 data_len;
    __sum16 csum;
    struct mptcp_addr_info addr;
    u64 ahmac;
    struct mptcp_ext ext_copy;
    u64 fail_seq;
    u32 nonce;
    u32 token;
    u64 thmac;
    u8 hmac[20];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mptcp_out_options {
    u16 suboptions;
    struct mptcp_rm_list rm_list;
    u8 join_id;
    u8 backup;
    u8 reset_reason;
    u8 reset_transient;
    u8 csum_reqd;
    u8 allow_join_id0;
    u64 sndr_key;
    u64 rcvr_key;
    u64 data_seq;
    u32 subflow_seq;
    u16 data_len;
    __sum16 csum;
    struct mptcp_addr_info addr;
    u64 ahmac;
    struct mptcp_ext ext_copy;
    u64 fail_seq;
    u32 nonce;
    u32 token;
    u64 thmac;
    u8 hmac[20];
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
<code>u16 port</code>
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
<code>struct in6_addr addr6</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 addr_id</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 port</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 rm_id</code>
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
<code>u8 csum_reqd</code>
</li>
<li>
<b>Field added. </b>
<code>u8 allow_join_id0</code>
</li>
<li>
<b>Field added. </b>
<code>u64 data_seq</code>
</li>
<li>
<b>Field added. </b>
<code>u32 subflow_seq</code>
</li>
<li>
<b>Field added. </b>
<code>u16 data_len</code>
</li>
<li>
<b>Field added. </b>
<code>__sum16 csum</code>
</li>
<li>
<b>Field added. </b>
<code>u64 fail_seq</code>
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
