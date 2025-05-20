# Struct: <code>tcp_request_sock</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct tcp_request_sock {
    struct inet_request_sock req;
    const struct tcp_request_sock_ops *af_specific;
    struct skb_mstamp snt_synack;
    bool tfo_listener;
    u32 txhash;
    u32 rcv_isn;
    u32 snt_isn;
    u32 last_oow_ack_time;
    u32 rcv_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct tcp_request_sock {
    struct inet_request_sock req;
    const struct tcp_request_sock_ops *af_specific;
    struct skb_mstamp snt_synack;
    bool tfo_listener;
    u32 txhash;
    u32 rcv_isn;
    u32 snt_isn;
    u32 last_oow_ack_time;
    u32 rcv_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct tcp_request_sock {
    struct inet_request_sock req;
    const struct tcp_request_sock_ops *af_specific;
    struct skb_mstamp snt_synack;
    bool tfo_listener;
    u32 txhash;
    u32 rcv_isn;
    u32 snt_isn;
    u32 ts_off;
    u32 last_oow_ack_time;
    u32 rcv_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct tcp_request_sock {
    struct inet_request_sock req;
    const struct tcp_request_sock_ops *af_specific;
    u64 snt_synack;
    bool tfo_listener;
    u32 txhash;
    u32 rcv_isn;
    u32 snt_isn;
    u32 ts_off;
    u32 last_oow_ack_time;
    u32 rcv_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct tcp_request_sock {
    struct inet_request_sock req;
    const struct tcp_request_sock_ops *af_specific;
    u64 snt_synack;
    bool tfo_listener;
    u32 txhash;
    u32 rcv_isn;
    u32 snt_isn;
    u32 ts_off;
    u32 last_oow_ack_time;
    u32 rcv_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct tcp_request_sock {
    struct inet_request_sock req;
    const struct tcp_request_sock_ops *af_specific;
    u64 snt_synack;
    bool tfo_listener;
    u32 txhash;
    u32 rcv_isn;
    u32 snt_isn;
    u32 ts_off;
    u32 last_oow_ack_time;
    u32 rcv_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct tcp_request_sock {
    struct inet_request_sock req;
    const struct tcp_request_sock_ops *af_specific;
    u64 snt_synack;
    bool tfo_listener;
    u32 txhash;
    u32 rcv_isn;
    u32 snt_isn;
    u32 ts_off;
    u32 last_oow_ack_time;
    u32 rcv_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct tcp_request_sock {
    struct inet_request_sock req;
    const struct tcp_request_sock_ops *af_specific;
    u64 snt_synack;
    bool tfo_listener;
    u32 txhash;
    u32 rcv_isn;
    u32 snt_isn;
    u32 ts_off;
    u32 last_oow_ack_time;
    u32 rcv_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct tcp_request_sock {
    struct inet_request_sock req;
    const struct tcp_request_sock_ops *af_specific;
    u64 snt_synack;
    bool tfo_listener;
    u32 txhash;
    u32 rcv_isn;
    u32 snt_isn;
    u32 ts_off;
    u32 last_oow_ack_time;
    u32 rcv_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct tcp_request_sock {
    struct inet_request_sock req;
    const struct tcp_request_sock_ops *af_specific;
    u64 snt_synack;
    bool tfo_listener;
    bool is_mptcp;
    bool drop_req;
    u32 txhash;
    u32 rcv_isn;
    u32 snt_isn;
    u32 ts_off;
    u32 last_oow_ack_time;
    u32 rcv_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct tcp_request_sock {
    struct inet_request_sock req;
    const struct tcp_request_sock_ops *af_specific;
    u64 snt_synack;
    bool tfo_listener;
    bool is_mptcp;
    bool drop_req;
    u32 txhash;
    u32 rcv_isn;
    u32 snt_isn;
    u32 ts_off;
    u32 last_oow_ack_time;
    u32 rcv_nxt;
    u8 syn_tos;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct tcp_request_sock {
    struct inet_request_sock req;
    const struct tcp_request_sock_ops *af_specific;
    u64 snt_synack;
    bool tfo_listener;
    bool is_mptcp;
    bool drop_req;
    u32 txhash;
    u32 rcv_isn;
    u32 snt_isn;
    u32 ts_off;
    u32 last_oow_ack_time;
    u32 rcv_nxt;
    u8 syn_tos;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct tcp_request_sock {
    struct inet_request_sock req;
    const struct tcp_request_sock_ops *af_specific;
    u64 snt_synack;
    bool tfo_listener;
    bool is_mptcp;
    bool drop_req;
    u32 txhash;
    u32 rcv_isn;
    u32 snt_isn;
    u32 ts_off;
    u32 last_oow_ack_time;
    u32 rcv_nxt;
    u8 syn_tos;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct tcp_request_sock {
    struct inet_request_sock req;
    const struct tcp_request_sock_ops *af_specific;
    u64 snt_synack;
    bool tfo_listener;
    bool is_mptcp;
    bool drop_req;
    u32 txhash;
    u32 rcv_isn;
    u32 snt_isn;
    u32 ts_off;
    u32 last_oow_ack_time;
    u32 rcv_nxt;
    u8 syn_tos;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct tcp_request_sock {
    struct inet_request_sock req;
    const struct tcp_request_sock_ops *af_specific;
    u64 snt_synack;
    bool tfo_listener;
    bool is_mptcp;
    bool drop_req;
    u32 txhash;
    u32 rcv_isn;
    u32 snt_isn;
    u32 ts_off;
    u32 last_oow_ack_time;
    u32 rcv_nxt;
    u8 syn_tos;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct tcp_request_sock {
    struct inet_request_sock req;
    const struct tcp_request_sock_ops *af_specific;
    u64 snt_synack;
    bool tfo_listener;
    bool is_mptcp;
    bool drop_req;
    u32 txhash;
    u32 rcv_isn;
    u32 snt_isn;
    u32 ts_off;
    u32 last_oow_ack_time;
    u32 rcv_nxt;
    u8 syn_tos;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct tcp_request_sock {
    struct inet_request_sock req;
    const struct tcp_request_sock_ops *af_specific;
    u64 snt_synack;
    bool tfo_listener;
    bool is_mptcp;
    bool req_usec_ts;
    bool drop_req;
    u32 txhash;
    u32 rcv_isn;
    u32 snt_isn;
    u32 ts_off;
    u32 last_oow_ack_time;
    u32 rcv_nxt;
    u8 syn_tos;
    u8 ao_keyid;
    u8 ao_rcv_next;
    bool used_tcp_ao;
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
struct tcp_request_sock {
    struct inet_request_sock req;
    const struct tcp_request_sock_ops *af_specific;
    u64 snt_synack;
    bool tfo_listener;
    u32 txhash;
    u32 rcv_isn;
    u32 snt_isn;
    u32 ts_off;
    u32 last_oow_ack_time;
    u32 rcv_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct tcp_request_sock {
    struct inet_request_sock req;
    const struct tcp_request_sock_ops *af_specific;
    u64 snt_synack;
    bool tfo_listener;
    u32 txhash;
    u32 rcv_isn;
    u32 snt_isn;
    u32 ts_off;
    u32 last_oow_ack_time;
    u32 rcv_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct tcp_request_sock {
    struct inet_request_sock req;
    const struct tcp_request_sock_ops *af_specific;
    u64 snt_synack;
    bool tfo_listener;
    u32 txhash;
    u32 rcv_isn;
    u32 snt_isn;
    u32 ts_off;
    u32 last_oow_ack_time;
    u32 rcv_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct tcp_request_sock {
    struct inet_request_sock req;
    const struct tcp_request_sock_ops *af_specific;
    u64 snt_synack;
    bool tfo_listener;
    u32 txhash;
    u32 rcv_isn;
    u32 snt_isn;
    u32 ts_off;
    u32 last_oow_ack_time;
    u32 rcv_nxt;
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
struct tcp_request_sock {
    struct inet_request_sock req;
    const struct tcp_request_sock_ops *af_specific;
    u64 snt_synack;
    bool tfo_listener;
    u32 txhash;
    u32 rcv_isn;
    u32 snt_isn;
    u32 ts_off;
    u32 last_oow_ack_time;
    u32 rcv_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct tcp_request_sock {
    struct inet_request_sock req;
    const struct tcp_request_sock_ops *af_specific;
    u64 snt_synack;
    bool tfo_listener;
    u32 txhash;
    u32 rcv_isn;
    u32 snt_isn;
    u32 ts_off;
    u32 last_oow_ack_time;
    u32 rcv_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct tcp_request_sock {
    struct inet_request_sock req;
    const struct tcp_request_sock_ops *af_specific;
    u64 snt_synack;
    bool tfo_listener;
    u32 txhash;
    u32 rcv_isn;
    u32 snt_isn;
    u32 ts_off;
    u32 last_oow_ack_time;
    u32 rcv_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct tcp_request_sock {
    struct inet_request_sock req;
    const struct tcp_request_sock_ops *af_specific;
    u64 snt_synack;
    bool tfo_listener;
    u32 txhash;
    u32 rcv_isn;
    u32 snt_isn;
    u32 ts_off;
    u32 last_oow_ack_time;
    u32 rcv_nxt;
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
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 ts_off</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct skb_mstamp snt_synack</code> ➡️ <code>u64 snt_synack</code>
</li>
</ul>
</details>
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
<b>Field added. </b>
<code>bool is_mptcp</code>
</li>
<li>
<b>Field added. </b>
<code>bool drop_req</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 syn_tos</code>
</li>
</ul>
</details>
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
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool req_usec_ts</code>
</li>
<li>
<b>Field added. </b>
<code>u8 ao_keyid</code>
</li>
<li>
<b>Field added. </b>
<code>u8 ao_rcv_next</code>
</li>
<li>
<b>Field added. </b>
<code>bool used_tcp_ao</code>
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
