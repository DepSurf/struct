# Struct: <code>mptcp_subflow_context</code>

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
struct mptcp_subflow_context {
    struct list_head node;
    u64 local_key;
    u64 remote_key;
    u64 idsn;
    u64 map_seq;
    u32 snd_isn;
    u32 token;
    u32 rel_write_seq;
    u32 map_subflow_seq;
    u32 ssn_offset;
    u32 map_data_len;
    u32 request_mptcp;
    u32 request_join;
    u32 request_bkup;
    u32 mp_capable;
    u32 mp_join;
    u32 fully_established;
    u32 pm_notified;
    u32 conn_finished;
    u32 map_valid;
    u32 mpc_map;
    u32 backup;
    u32 data_avail;
    u32 rx_eof;
    u32 data_fin_tx_enable;
    u32 use_64bit_ack;
    u32 can_ack;
    u64 data_fin_tx_seq;
    u32 remote_nonce;
    u64 thmac;
    u32 local_nonce;
    u32 remote_token;
    u8 hmac[20];
    u8 local_id;
    u8 remote_id;
    struct sock *tcp_sock;
    struct sock *conn;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    void (*tcp_data_ready)(struct sock *);
    void (*tcp_state_change)(struct sock *);
    void (*tcp_write_space)(struct sock *);
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mptcp_subflow_context {
    struct list_head node;
    u64 local_key;
    u64 remote_key;
    u64 idsn;
    u64 map_seq;
    u32 snd_isn;
    u32 token;
    u32 rel_write_seq;
    u32 map_subflow_seq;
    u32 ssn_offset;
    u32 map_data_len;
    u32 request_mptcp;
    u32 request_join;
    u32 request_bkup;
    u32 mp_capable;
    u32 mp_join;
    u32 fully_established;
    u32 pm_notified;
    u32 conn_finished;
    u32 map_valid;
    u32 mpc_map;
    u32 backup;
    u32 rx_eof;
    u32 can_ack;
    u32 disposable;
    enum mptcp_data_avail data_avail;
    u32 remote_nonce;
    u64 thmac;
    u32 local_nonce;
    u32 remote_token;
    u8 hmac[20];
    u8 local_id;
    u8 remote_id;
    struct sock *tcp_sock;
    struct sock *conn;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    void (*tcp_data_ready)(struct sock *);
    void (*tcp_state_change)(struct sock *);
    void (*tcp_write_space)(struct sock *);
    void (*tcp_error_report)(struct sock *);
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mptcp_subflow_context {
    struct list_head node;
    u64 local_key;
    u64 remote_key;
    u64 idsn;
    u64 map_seq;
    u32 snd_isn;
    u32 token;
    u32 rel_write_seq;
    u32 map_subflow_seq;
    u32 ssn_offset;
    u32 map_data_len;
    u32 request_mptcp;
    u32 request_join;
    u32 request_bkup;
    u32 mp_capable;
    u32 mp_join;
    u32 fully_established;
    u32 pm_notified;
    u32 conn_finished;
    u32 map_valid;
    u32 mpc_map;
    u32 backup;
    u32 send_mp_prio;
    u32 rx_eof;
    u32 can_ack;
    u32 disposable;
    enum mptcp_data_avail data_avail;
    u32 remote_nonce;
    u64 thmac;
    u32 local_nonce;
    u32 remote_token;
    u8 hmac[20];
    u8 local_id;
    u8 remote_id;
    u8 reset_seen;
    u8 reset_transient;
    u8 reset_reason;
    long int delegated_status;
    struct list_head delegated_node;
    u32 setsockopt_seq;
    struct sock *tcp_sock;
    struct sock *conn;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    void (*tcp_data_ready)(struct sock *);
    void (*tcp_state_change)(struct sock *);
    void (*tcp_write_space)(struct sock *);
    void (*tcp_error_report)(struct sock *);
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mptcp_subflow_context {
    struct list_head node;
    u64 local_key;
    u64 remote_key;
    u64 idsn;
    u64 map_seq;
    u32 snd_isn;
    u32 token;
    u32 rel_write_seq;
    u32 map_subflow_seq;
    u32 ssn_offset;
    u32 map_data_len;
    __wsum map_data_csum;
    u32 map_csum_len;
    u32 request_mptcp;
    u32 request_join;
    u32 request_bkup;
    u32 mp_capable;
    u32 mp_join;
    u32 fully_established;
    u32 pm_notified;
    u32 conn_finished;
    u32 map_valid;
    u32 map_csum_reqd;
    u32 map_data_fin;
    u32 mpc_map;
    u32 backup;
    u32 send_mp_prio;
    u32 send_mp_fail;
    u32 rx_eof;
    u32 can_ack;
    u32 disposable;
    u32 stale;
    enum mptcp_data_avail data_avail;
    u32 remote_nonce;
    u64 thmac;
    u32 local_nonce;
    u32 remote_token;
    u8 hmac[20];
    u8 local_id;
    u8 remote_id;
    u8 reset_seen;
    u8 reset_transient;
    u8 reset_reason;
    u8 stale_count;
    long int delegated_status;
    struct list_head delegated_node;
    u32 setsockopt_seq;
    u32 stale_rcv_tstamp;
    struct sock *tcp_sock;
    struct sock *conn;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    void (*tcp_data_ready)(struct sock *);
    void (*tcp_state_change)(struct sock *);
    void (*tcp_write_space)(struct sock *);
    void (*tcp_error_report)(struct sock *);
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mptcp_subflow_context {
    struct list_head node;
    long unsigned int avg_pacing_rate;
    u64 local_key;
    u64 remote_key;
    u64 idsn;
    u64 map_seq;
    u32 snd_isn;
    u32 token;
    u32 rel_write_seq;
    u32 map_subflow_seq;
    u32 ssn_offset;
    u32 map_data_len;
    __wsum map_data_csum;
    u32 map_csum_len;
    u32 request_mptcp;
    u32 request_join;
    u32 request_bkup;
    u32 mp_capable;
    u32 mp_join;
    u32 fully_established;
    u32 pm_notified;
    u32 conn_finished;
    u32 map_valid;
    u32 map_csum_reqd;
    u32 map_data_fin;
    u32 mpc_map;
    u32 backup;
    u32 send_mp_prio;
    u32 send_mp_fail;
    u32 send_fastclose;
    u32 send_infinite_map;
    u32 rx_eof;
    u32 can_ack;
    u32 disposable;
    u32 stale;
    u32 local_id_valid;
    u32 valid_csum_seen;
    enum mptcp_data_avail data_avail;
    u32 remote_nonce;
    u64 thmac;
    u32 local_nonce;
    u32 remote_token;
    u8 hmac[20];
    u8 local_id;
    u8 remote_id;
    u8 reset_seen;
    u8 reset_transient;
    u8 reset_reason;
    u8 stale_count;
    long int delegated_status;
    long unsigned int fail_tout;
    struct (anon) reset;
    struct list_head delegated_node;
    u32 setsockopt_seq;
    u32 stale_rcv_tstamp;
    struct sock *tcp_sock;
    struct sock *conn;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    void (*tcp_state_change)(struct sock *);
    void (*tcp_error_report)(struct sock *);
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mptcp_subflow_context {
    struct list_head node;
    long unsigned int avg_pacing_rate;
    u64 local_key;
    u64 remote_key;
    u64 idsn;
    u64 map_seq;
    u32 snd_isn;
    u32 token;
    u32 rel_write_seq;
    u32 map_subflow_seq;
    u32 ssn_offset;
    u32 map_data_len;
    __wsum map_data_csum;
    u32 map_csum_len;
    u32 request_mptcp;
    u32 request_join;
    u32 request_bkup;
    u32 mp_capable;
    u32 mp_join;
    u32 fully_established;
    u32 pm_notified;
    u32 conn_finished;
    u32 map_valid;
    u32 map_csum_reqd;
    u32 map_data_fin;
    u32 mpc_map;
    u32 backup;
    u32 send_mp_prio;
    u32 send_mp_fail;
    u32 send_fastclose;
    u32 send_infinite_map;
    u32 rx_eof;
    u32 remote_key_valid;
    u32 disposable;
    u32 stale;
    u32 local_id_valid;
    u32 valid_csum_seen;
    u32 is_mptfo;
    u32 __unused;
    enum mptcp_data_avail data_avail;
    u32 remote_nonce;
    u64 thmac;
    u32 local_nonce;
    u32 remote_token;
    u8 hmac[20];
    u64 iasn;
    u8 local_id;
    u8 remote_id;
    u8 reset_seen;
    u8 reset_transient;
    u8 reset_reason;
    u8 stale_count;
    long int delegated_status;
    long unsigned int fail_tout;
    struct (anon) reset;
    struct list_head delegated_node;
    u32 setsockopt_seq;
    u32 stale_rcv_tstamp;
    struct sock *tcp_sock;
    struct sock *conn;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    void (*tcp_state_change)(struct sock *);
    void (*tcp_error_report)(struct sock *);
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mptcp_subflow_context {
    struct list_head node;
    long unsigned int avg_pacing_rate;
    u64 local_key;
    u64 remote_key;
    u64 idsn;
    u64 map_seq;
    u32 snd_isn;
    u32 token;
    u32 rel_write_seq;
    u32 map_subflow_seq;
    u32 ssn_offset;
    u32 map_data_len;
    __wsum map_data_csum;
    u32 map_csum_len;
    u32 request_mptcp;
    u32 request_join;
    u32 request_bkup;
    u32 mp_capable;
    u32 mp_join;
    u32 fully_established;
    u32 pm_notified;
    u32 conn_finished;
    u32 map_valid;
    u32 map_csum_reqd;
    u32 map_data_fin;
    u32 mpc_map;
    u32 backup;
    u32 send_mp_prio;
    u32 send_mp_fail;
    u32 send_fastclose;
    u32 send_infinite_map;
    u32 remote_key_valid;
    u32 disposable;
    u32 stale;
    u32 local_id_valid;
    u32 valid_csum_seen;
    u32 is_mptfo;
    u32 __unused;
    enum mptcp_data_avail data_avail;
    u32 remote_nonce;
    u64 thmac;
    u32 local_nonce;
    u32 remote_token;
    u8 hmac[20];
    u64 iasn;
    u8 local_id;
    u8 remote_id;
    u8 reset_seen;
    u8 reset_transient;
    u8 reset_reason;
    u8 stale_count;
    u32 subflow_id;
    long int delegated_status;
    long unsigned int fail_tout;
    struct (anon) reset;
    struct list_head delegated_node;
    u32 setsockopt_seq;
    u32 stale_rcv_tstamp;
    struct sock *tcp_sock;
    struct sock *conn;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    void (*tcp_state_change)(struct sock *);
    void (*tcp_error_report)(struct sock *);
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mptcp_subflow_context {
    struct list_head node;
    long unsigned int avg_pacing_rate;
    u64 local_key;
    u64 remote_key;
    u64 idsn;
    u64 map_seq;
    u32 snd_isn;
    u32 token;
    u32 rel_write_seq;
    u32 map_subflow_seq;
    u32 ssn_offset;
    u32 map_data_len;
    __wsum map_data_csum;
    u32 map_csum_len;
    u32 request_mptcp;
    u32 request_join;
    u32 request_bkup;
    u32 mp_capable;
    u32 mp_join;
    u32 fully_established;
    u32 pm_notified;
    u32 conn_finished;
    u32 map_valid;
    u32 map_csum_reqd;
    u32 map_data_fin;
    u32 mpc_map;
    u32 backup;
    u32 send_mp_prio;
    u32 send_mp_fail;
    u32 send_fastclose;
    u32 send_infinite_map;
    u32 remote_key_valid;
    u32 disposable;
    u32 stale;
    u32 valid_csum_seen;
    u32 is_mptfo;
    u32 __unused;
    bool data_avail;
    bool scheduled;
    u32 remote_nonce;
    u64 thmac;
    u32 local_nonce;
    u32 remote_token;
    u8 hmac[20];
    u64 iasn;
    s16 local_id;
    u8 remote_id;
    u8 reset_seen;
    u8 reset_transient;
    u8 reset_reason;
    u8 stale_count;
    u32 subflow_id;
    long int delegated_status;
    long unsigned int fail_tout;
    struct (anon) reset;
    struct list_head delegated_node;
    u32 setsockopt_seq;
    u32 stale_rcv_tstamp;
    int cached_sndbuf;
    struct sock *tcp_sock;
    struct sock *conn;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    void (*tcp_state_change)(struct sock *);
    void (*tcp_error_report)(struct sock *);
    struct callback_head rcu;
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
<code>u32 disposable</code>
</li>
<li>
<b>Field added. </b>
<code>void (*tcp_error_report)(struct sock *)</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 data_fin_tx_enable</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 use_64bit_ack</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 data_fin_tx_seq</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 data_avail</code> ➡️ <code>enum mptcp_data_avail data_avail</code>
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
<code>u32 send_mp_prio</code>
</li>
<li>
<b>Field added. </b>
<code>u8 reset_seen</code>
</li>
<li>
<b>Field added. </b>
<code>u8 reset_transient</code>
</li>
<li>
<b>Field added. </b>
<code>u8 reset_reason</code>
</li>
<li>
<b>Field added. </b>
<code>long int delegated_status</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head delegated_node</code>
</li>
<li>
<b>Field added. </b>
<code>u32 setsockopt_seq</code>
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
<code>__wsum map_data_csum</code>
</li>
<li>
<b>Field added. </b>
<code>u32 map_csum_len</code>
</li>
<li>
<b>Field added. </b>
<code>u32 map_csum_reqd</code>
</li>
<li>
<b>Field added. </b>
<code>u32 map_data_fin</code>
</li>
<li>
<b>Field added. </b>
<code>u32 send_mp_fail</code>
</li>
<li>
<b>Field added. </b>
<code>u32 stale</code>
</li>
<li>
<b>Field added. </b>
<code>u8 stale_count</code>
</li>
<li>
<b>Field added. </b>
<code>u32 stale_rcv_tstamp</code>
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
<code>long unsigned int avg_pacing_rate</code>
</li>
<li>
<b>Field added. </b>
<code>u32 send_fastclose</code>
</li>
<li>
<b>Field added. </b>
<code>u32 send_infinite_map</code>
</li>
<li>
<b>Field added. </b>
<code>u32 local_id_valid</code>
</li>
<li>
<b>Field added. </b>
<code>u32 valid_csum_seen</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int fail_tout</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) reset</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*tcp_data_ready)(struct sock *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*tcp_write_space)(struct sock *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 remote_key_valid</code>
</li>
<li>
<b>Field added. </b>
<code>u32 is_mptfo</code>
</li>
<li>
<b>Field added. </b>
<code>u32 __unused</code>
</li>
<li>
<b>Field added. </b>
<code>u64 iasn</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 can_ack</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 subflow_id</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 rx_eof</code>
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
<code>bool scheduled</code>
</li>
<li>
<b>Field added. </b>
<code>int cached_sndbuf</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 local_id_valid</code>
</li>
<li>
<b>Field type changed. </b>
<code>enum mptcp_data_avail data_avail</code> ➡️ <code>bool data_avail</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 local_id</code> ➡️ <code>s16 local_id</code>
</li>
</ul>
</details>
</li>
</ul>
