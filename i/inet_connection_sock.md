# Struct: <code>inet_connection_sock</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct inet_connection_sock {
    struct inet_sock icsk_inet;
    struct request_sock_queue icsk_accept_queue;
    struct inet_bind_bucket *icsk_bind_hash;
    long unsigned int icsk_timeout;
    struct timer_list icsk_retransmit_timer;
    struct timer_list icsk_delack_timer;
    __u32 icsk_rto;
    __u32 icsk_pmtu_cookie;
    const struct tcp_congestion_ops *icsk_ca_ops;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    unsigned int (*icsk_sync_mss)(struct sock *, u32);
    __u8 icsk_ca_state;
    __u8 icsk_ca_setsockopt;
    __u8 icsk_ca_dst_locked;
    __u8 icsk_retransmits;
    __u8 icsk_pending;
    __u8 icsk_backoff;
    __u8 icsk_syn_retries;
    __u8 icsk_probes_out;
    __u16 icsk_ext_hdr_len;
    struct (anon) icsk_ack;
    struct (anon) icsk_mtup;
    u32 icsk_user_timeout;
    u64 icsk_ca_priv[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct inet_connection_sock {
    struct inet_sock icsk_inet;
    struct request_sock_queue icsk_accept_queue;
    struct inet_bind_bucket *icsk_bind_hash;
    long unsigned int icsk_timeout;
    struct timer_list icsk_retransmit_timer;
    struct timer_list icsk_delack_timer;
    __u32 icsk_rto;
    __u32 icsk_pmtu_cookie;
    const struct tcp_congestion_ops *icsk_ca_ops;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    unsigned int (*icsk_sync_mss)(struct sock *, u32);
    __u8 icsk_ca_state;
    __u8 icsk_ca_setsockopt;
    __u8 icsk_ca_dst_locked;
    __u8 icsk_retransmits;
    __u8 icsk_pending;
    __u8 icsk_backoff;
    __u8 icsk_syn_retries;
    __u8 icsk_probes_out;
    __u16 icsk_ext_hdr_len;
    struct (anon) icsk_ack;
    struct (anon) icsk_mtup;
    u32 icsk_user_timeout;
    u64 icsk_ca_priv[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct inet_connection_sock {
    struct inet_sock icsk_inet;
    struct request_sock_queue icsk_accept_queue;
    struct inet_bind_bucket *icsk_bind_hash;
    long unsigned int icsk_timeout;
    struct timer_list icsk_retransmit_timer;
    struct timer_list icsk_delack_timer;
    __u32 icsk_rto;
    __u32 icsk_pmtu_cookie;
    const struct tcp_congestion_ops *icsk_ca_ops;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    unsigned int (*icsk_sync_mss)(struct sock *, u32);
    __u8 icsk_ca_state;
    __u8 icsk_ca_setsockopt;
    __u8 icsk_ca_dst_locked;
    __u8 icsk_retransmits;
    __u8 icsk_pending;
    __u8 icsk_backoff;
    __u8 icsk_syn_retries;
    __u8 icsk_probes_out;
    __u16 icsk_ext_hdr_len;
    struct (anon) icsk_ack;
    struct (anon) icsk_mtup;
    u32 icsk_user_timeout;
    u64 icsk_ca_priv[11];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct inet_connection_sock {
    struct inet_sock icsk_inet;
    struct request_sock_queue icsk_accept_queue;
    struct inet_bind_bucket *icsk_bind_hash;
    long unsigned int icsk_timeout;
    struct timer_list icsk_retransmit_timer;
    struct timer_list icsk_delack_timer;
    __u32 icsk_rto;
    __u32 icsk_pmtu_cookie;
    const struct tcp_congestion_ops *icsk_ca_ops;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    const struct tcp_ulp_ops *icsk_ulp_ops;
    void *icsk_ulp_data;
    unsigned int (*icsk_sync_mss)(struct sock *, u32);
    __u8 icsk_ca_state;
    __u8 icsk_ca_setsockopt;
    __u8 icsk_ca_dst_locked;
    __u8 icsk_retransmits;
    __u8 icsk_pending;
    __u8 icsk_backoff;
    __u8 icsk_syn_retries;
    __u8 icsk_probes_out;
    __u16 icsk_ext_hdr_len;
    struct (anon) icsk_ack;
    struct (anon) icsk_mtup;
    u32 icsk_user_timeout;
    u64 icsk_ca_priv[11];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct inet_connection_sock {
    struct inet_sock icsk_inet;
    struct request_sock_queue icsk_accept_queue;
    struct inet_bind_bucket *icsk_bind_hash;
    long unsigned int icsk_timeout;
    struct timer_list icsk_retransmit_timer;
    struct timer_list icsk_delack_timer;
    __u32 icsk_rto;
    __u32 icsk_pmtu_cookie;
    const struct tcp_congestion_ops *icsk_ca_ops;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    const struct tcp_ulp_ops *icsk_ulp_ops;
    void *icsk_ulp_data;
    unsigned int (*icsk_sync_mss)(struct sock *, u32);
    __u8 icsk_ca_state;
    __u8 icsk_ca_setsockopt;
    __u8 icsk_ca_dst_locked;
    __u8 icsk_retransmits;
    __u8 icsk_pending;
    __u8 icsk_backoff;
    __u8 icsk_syn_retries;
    __u8 icsk_probes_out;
    __u16 icsk_ext_hdr_len;
    struct (anon) icsk_ack;
    struct (anon) icsk_mtup;
    u32 icsk_user_timeout;
    u64 icsk_ca_priv[11];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct inet_connection_sock {
    struct inet_sock icsk_inet;
    struct request_sock_queue icsk_accept_queue;
    struct inet_bind_bucket *icsk_bind_hash;
    long unsigned int icsk_timeout;
    struct timer_list icsk_retransmit_timer;
    struct timer_list icsk_delack_timer;
    __u32 icsk_rto;
    __u32 icsk_pmtu_cookie;
    const struct tcp_congestion_ops *icsk_ca_ops;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    const struct tcp_ulp_ops *icsk_ulp_ops;
    void *icsk_ulp_data;
    void (*icsk_clean_acked)(struct sock *, u32);
    struct hlist_node icsk_listen_portaddr_node;
    unsigned int (*icsk_sync_mss)(struct sock *, u32);
    __u8 icsk_ca_state;
    __u8 icsk_ca_setsockopt;
    __u8 icsk_ca_dst_locked;
    __u8 icsk_retransmits;
    __u8 icsk_pending;
    __u8 icsk_backoff;
    __u8 icsk_syn_retries;
    __u8 icsk_probes_out;
    __u16 icsk_ext_hdr_len;
    struct (anon) icsk_ack;
    struct (anon) icsk_mtup;
    u32 icsk_user_timeout;
    u64 icsk_ca_priv[11];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct inet_connection_sock {
    struct inet_sock icsk_inet;
    struct request_sock_queue icsk_accept_queue;
    struct inet_bind_bucket *icsk_bind_hash;
    long unsigned int icsk_timeout;
    struct timer_list icsk_retransmit_timer;
    struct timer_list icsk_delack_timer;
    __u32 icsk_rto;
    __u32 icsk_pmtu_cookie;
    const struct tcp_congestion_ops *icsk_ca_ops;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    const struct tcp_ulp_ops *icsk_ulp_ops;
    void *icsk_ulp_data;
    void (*icsk_clean_acked)(struct sock *, u32);
    struct hlist_node icsk_listen_portaddr_node;
    unsigned int (*icsk_sync_mss)(struct sock *, u32);
    __u8 icsk_ca_state;
    __u8 icsk_ca_setsockopt;
    __u8 icsk_ca_dst_locked;
    __u8 icsk_retransmits;
    __u8 icsk_pending;
    __u8 icsk_backoff;
    __u8 icsk_syn_retries;
    __u8 icsk_probes_out;
    __u16 icsk_ext_hdr_len;
    struct (anon) icsk_ack;
    struct (anon) icsk_mtup;
    u32 icsk_user_timeout;
    u64 icsk_ca_priv[11];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct inet_connection_sock {
    struct inet_sock icsk_inet;
    struct request_sock_queue icsk_accept_queue;
    struct inet_bind_bucket *icsk_bind_hash;
    long unsigned int icsk_timeout;
    struct timer_list icsk_retransmit_timer;
    struct timer_list icsk_delack_timer;
    __u32 icsk_rto;
    __u32 icsk_pmtu_cookie;
    const struct tcp_congestion_ops *icsk_ca_ops;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    const struct tcp_ulp_ops *icsk_ulp_ops;
    void *icsk_ulp_data;
    void (*icsk_clean_acked)(struct sock *, u32);
    struct hlist_node icsk_listen_portaddr_node;
    unsigned int (*icsk_sync_mss)(struct sock *, u32);
    __u8 icsk_ca_state;
    __u8 icsk_ca_setsockopt;
    __u8 icsk_ca_dst_locked;
    __u8 icsk_retransmits;
    __u8 icsk_pending;
    __u8 icsk_backoff;
    __u8 icsk_syn_retries;
    __u8 icsk_probes_out;
    __u16 icsk_ext_hdr_len;
    struct (anon) icsk_ack;
    struct (anon) icsk_mtup;
    u32 icsk_user_timeout;
    u64 icsk_ca_priv[13];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct inet_connection_sock {
    struct inet_sock icsk_inet;
    struct request_sock_queue icsk_accept_queue;
    struct inet_bind_bucket *icsk_bind_hash;
    long unsigned int icsk_timeout;
    struct timer_list icsk_retransmit_timer;
    struct timer_list icsk_delack_timer;
    __u32 icsk_rto;
    __u32 icsk_pmtu_cookie;
    const struct tcp_congestion_ops *icsk_ca_ops;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    const struct tcp_ulp_ops *icsk_ulp_ops;
    void *icsk_ulp_data;
    void (*icsk_clean_acked)(struct sock *, u32);
    struct hlist_node icsk_listen_portaddr_node;
    unsigned int (*icsk_sync_mss)(struct sock *, u32);
    __u8 icsk_ca_state;
    __u8 icsk_ca_setsockopt;
    __u8 icsk_ca_dst_locked;
    __u8 icsk_retransmits;
    __u8 icsk_pending;
    __u8 icsk_backoff;
    __u8 icsk_syn_retries;
    __u8 icsk_probes_out;
    __u16 icsk_ext_hdr_len;
    struct (anon) icsk_ack;
    struct (anon) icsk_mtup;
    u32 icsk_user_timeout;
    u64 icsk_ca_priv[13];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct inet_connection_sock {
    struct inet_sock icsk_inet;
    struct request_sock_queue icsk_accept_queue;
    struct inet_bind_bucket *icsk_bind_hash;
    long unsigned int icsk_timeout;
    struct timer_list icsk_retransmit_timer;
    struct timer_list icsk_delack_timer;
    __u32 icsk_rto;
    __u32 icsk_pmtu_cookie;
    const struct tcp_congestion_ops *icsk_ca_ops;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    const struct tcp_ulp_ops *icsk_ulp_ops;
    void *icsk_ulp_data;
    void (*icsk_clean_acked)(struct sock *, u32);
    struct hlist_node icsk_listen_portaddr_node;
    unsigned int (*icsk_sync_mss)(struct sock *, u32);
    __u8 icsk_ca_state;
    __u8 icsk_ca_setsockopt;
    __u8 icsk_ca_dst_locked;
    __u8 icsk_retransmits;
    __u8 icsk_pending;
    __u8 icsk_backoff;
    __u8 icsk_syn_retries;
    __u8 icsk_probes_out;
    __u16 icsk_ext_hdr_len;
    struct (anon) icsk_ack;
    struct (anon) icsk_mtup;
    u32 icsk_user_timeout;
    u64 icsk_ca_priv[13];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct inet_connection_sock {
    struct inet_sock icsk_inet;
    struct request_sock_queue icsk_accept_queue;
    struct inet_bind_bucket *icsk_bind_hash;
    long unsigned int icsk_timeout;
    struct timer_list icsk_retransmit_timer;
    struct timer_list icsk_delack_timer;
    __u32 icsk_rto;
    __u32 icsk_rto_min;
    __u32 icsk_delack_max;
    __u32 icsk_pmtu_cookie;
    const struct tcp_congestion_ops *icsk_ca_ops;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    const struct tcp_ulp_ops *icsk_ulp_ops;
    void *icsk_ulp_data;
    void (*icsk_clean_acked)(struct sock *, u32);
    struct hlist_node icsk_listen_portaddr_node;
    unsigned int (*icsk_sync_mss)(struct sock *, u32);
    __u8 icsk_ca_state;
    __u8 icsk_ca_initialized;
    __u8 icsk_ca_setsockopt;
    __u8 icsk_ca_dst_locked;
    __u8 icsk_retransmits;
    __u8 icsk_pending;
    __u8 icsk_backoff;
    __u8 icsk_syn_retries;
    __u8 icsk_probes_out;
    __u16 icsk_ext_hdr_len;
    struct (anon) icsk_ack;
    struct (anon) icsk_mtup;
    u32 icsk_probes_tstamp;
    u32 icsk_user_timeout;
    u64 icsk_ca_priv[13];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct inet_connection_sock {
    struct inet_sock icsk_inet;
    struct request_sock_queue icsk_accept_queue;
    struct inet_bind_bucket *icsk_bind_hash;
    long unsigned int icsk_timeout;
    struct timer_list icsk_retransmit_timer;
    struct timer_list icsk_delack_timer;
    __u32 icsk_rto;
    __u32 icsk_rto_min;
    __u32 icsk_delack_max;
    __u32 icsk_pmtu_cookie;
    const struct tcp_congestion_ops *icsk_ca_ops;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    const struct tcp_ulp_ops *icsk_ulp_ops;
    void *icsk_ulp_data;
    void (*icsk_clean_acked)(struct sock *, u32);
    struct hlist_node icsk_listen_portaddr_node;
    unsigned int (*icsk_sync_mss)(struct sock *, u32);
    __u8 icsk_ca_state;
    __u8 icsk_ca_initialized;
    __u8 icsk_ca_setsockopt;
    __u8 icsk_ca_dst_locked;
    __u8 icsk_retransmits;
    __u8 icsk_pending;
    __u8 icsk_backoff;
    __u8 icsk_syn_retries;
    __u8 icsk_probes_out;
    __u16 icsk_ext_hdr_len;
    struct (anon) icsk_ack;
    struct (anon) icsk_mtup;
    u32 icsk_probes_tstamp;
    u32 icsk_user_timeout;
    u64 icsk_ca_priv[13];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct inet_connection_sock {
    struct inet_sock icsk_inet;
    struct request_sock_queue icsk_accept_queue;
    struct inet_bind_bucket *icsk_bind_hash;
    long unsigned int icsk_timeout;
    struct timer_list icsk_retransmit_timer;
    struct timer_list icsk_delack_timer;
    __u32 icsk_rto;
    __u32 icsk_rto_min;
    __u32 icsk_delack_max;
    __u32 icsk_pmtu_cookie;
    const struct tcp_congestion_ops *icsk_ca_ops;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    const struct tcp_ulp_ops *icsk_ulp_ops;
    void *icsk_ulp_data;
    void (*icsk_clean_acked)(struct sock *, u32);
    struct hlist_node icsk_listen_portaddr_node;
    unsigned int (*icsk_sync_mss)(struct sock *, u32);
    __u8 icsk_ca_state;
    __u8 icsk_ca_initialized;
    __u8 icsk_ca_setsockopt;
    __u8 icsk_ca_dst_locked;
    __u8 icsk_retransmits;
    __u8 icsk_pending;
    __u8 icsk_backoff;
    __u8 icsk_syn_retries;
    __u8 icsk_probes_out;
    __u16 icsk_ext_hdr_len;
    struct (anon) icsk_ack;
    struct (anon) icsk_mtup;
    u32 icsk_probes_tstamp;
    u32 icsk_user_timeout;
    u64 icsk_ca_priv[13];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct inet_connection_sock {
    struct inet_sock icsk_inet;
    struct request_sock_queue icsk_accept_queue;
    struct inet_bind_bucket *icsk_bind_hash;
    long unsigned int icsk_timeout;
    struct timer_list icsk_retransmit_timer;
    struct timer_list icsk_delack_timer;
    __u32 icsk_rto;
    __u32 icsk_rto_min;
    __u32 icsk_delack_max;
    __u32 icsk_pmtu_cookie;
    const struct tcp_congestion_ops *icsk_ca_ops;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    const struct tcp_ulp_ops *icsk_ulp_ops;
    void *icsk_ulp_data;
    void (*icsk_clean_acked)(struct sock *, u32);
    unsigned int (*icsk_sync_mss)(struct sock *, u32);
    __u8 icsk_ca_state;
    __u8 icsk_ca_initialized;
    __u8 icsk_ca_setsockopt;
    __u8 icsk_ca_dst_locked;
    __u8 icsk_retransmits;
    __u8 icsk_pending;
    __u8 icsk_backoff;
    __u8 icsk_syn_retries;
    __u8 icsk_probes_out;
    __u16 icsk_ext_hdr_len;
    struct (anon) icsk_ack;
    struct (anon) icsk_mtup;
    u32 icsk_probes_tstamp;
    u32 icsk_user_timeout;
    u64 icsk_ca_priv[13];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct inet_connection_sock {
    struct inet_sock icsk_inet;
    struct request_sock_queue icsk_accept_queue;
    struct inet_bind_bucket *icsk_bind_hash;
    struct inet_bind2_bucket *icsk_bind2_hash;
    long unsigned int icsk_timeout;
    struct timer_list icsk_retransmit_timer;
    struct timer_list icsk_delack_timer;
    __u32 icsk_rto;
    __u32 icsk_rto_min;
    __u32 icsk_delack_max;
    __u32 icsk_pmtu_cookie;
    const struct tcp_congestion_ops *icsk_ca_ops;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    const struct tcp_ulp_ops *icsk_ulp_ops;
    void *icsk_ulp_data;
    void (*icsk_clean_acked)(struct sock *, u32);
    unsigned int (*icsk_sync_mss)(struct sock *, u32);
    __u8 icsk_ca_state;
    __u8 icsk_ca_initialized;
    __u8 icsk_ca_setsockopt;
    __u8 icsk_ca_dst_locked;
    __u8 icsk_retransmits;
    __u8 icsk_pending;
    __u8 icsk_backoff;
    __u8 icsk_syn_retries;
    __u8 icsk_probes_out;
    __u16 icsk_ext_hdr_len;
    struct (anon) icsk_ack;
    struct (anon) icsk_mtup;
    u32 icsk_probes_tstamp;
    u32 icsk_user_timeout;
    u64 icsk_ca_priv[13];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct inet_connection_sock {
    struct inet_sock icsk_inet;
    struct request_sock_queue icsk_accept_queue;
    struct inet_bind_bucket *icsk_bind_hash;
    struct inet_bind2_bucket *icsk_bind2_hash;
    long unsigned int icsk_timeout;
    struct timer_list icsk_retransmit_timer;
    struct timer_list icsk_delack_timer;
    __u32 icsk_rto;
    __u32 icsk_rto_min;
    __u32 icsk_delack_max;
    __u32 icsk_pmtu_cookie;
    const struct tcp_congestion_ops *icsk_ca_ops;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    const struct tcp_ulp_ops *icsk_ulp_ops;
    void *icsk_ulp_data;
    void (*icsk_clean_acked)(struct sock *, u32);
    unsigned int (*icsk_sync_mss)(struct sock *, u32);
    __u8 icsk_ca_state;
    __u8 icsk_ca_initialized;
    __u8 icsk_ca_setsockopt;
    __u8 icsk_ca_dst_locked;
    __u8 icsk_retransmits;
    __u8 icsk_pending;
    __u8 icsk_backoff;
    __u8 icsk_syn_retries;
    __u8 icsk_probes_out;
    __u16 icsk_ext_hdr_len;
    struct (anon) icsk_ack;
    struct (anon) icsk_mtup;
    u32 icsk_probes_tstamp;
    u32 icsk_user_timeout;
    u64 icsk_ca_priv[13];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct inet_connection_sock {
    struct inet_sock icsk_inet;
    struct request_sock_queue icsk_accept_queue;
    struct inet_bind_bucket *icsk_bind_hash;
    struct inet_bind2_bucket *icsk_bind2_hash;
    long unsigned int icsk_timeout;
    struct timer_list icsk_retransmit_timer;
    struct timer_list icsk_delack_timer;
    __u32 icsk_rto;
    __u32 icsk_rto_min;
    __u32 icsk_delack_max;
    __u32 icsk_pmtu_cookie;
    const struct tcp_congestion_ops *icsk_ca_ops;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    const struct tcp_ulp_ops *icsk_ulp_ops;
    void *icsk_ulp_data;
    void (*icsk_clean_acked)(struct sock *, u32);
    unsigned int (*icsk_sync_mss)(struct sock *, u32);
    __u8 icsk_ca_state;
    __u8 icsk_ca_initialized;
    __u8 icsk_ca_setsockopt;
    __u8 icsk_ca_dst_locked;
    __u8 icsk_retransmits;
    __u8 icsk_pending;
    __u8 icsk_backoff;
    __u8 icsk_syn_retries;
    __u8 icsk_probes_out;
    __u16 icsk_ext_hdr_len;
    struct (anon) icsk_ack;
    struct (anon) icsk_mtup;
    u32 icsk_probes_tstamp;
    u32 icsk_user_timeout;
    u64 icsk_ca_priv[13];
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
struct inet_connection_sock {
    struct inet_sock icsk_inet;
    struct request_sock_queue icsk_accept_queue;
    struct inet_bind_bucket *icsk_bind_hash;
    long unsigned int icsk_timeout;
    struct timer_list icsk_retransmit_timer;
    struct timer_list icsk_delack_timer;
    __u32 icsk_rto;
    __u32 icsk_pmtu_cookie;
    const struct tcp_congestion_ops *icsk_ca_ops;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    const struct tcp_ulp_ops *icsk_ulp_ops;
    void *icsk_ulp_data;
    void (*icsk_clean_acked)(struct sock *, u32);
    struct hlist_node icsk_listen_portaddr_node;
    unsigned int (*icsk_sync_mss)(struct sock *, u32);
    __u8 icsk_ca_state;
    __u8 icsk_ca_setsockopt;
    __u8 icsk_ca_dst_locked;
    __u8 icsk_retransmits;
    __u8 icsk_pending;
    __u8 icsk_backoff;
    __u8 icsk_syn_retries;
    __u8 icsk_probes_out;
    __u16 icsk_ext_hdr_len;
    struct (anon) icsk_ack;
    struct (anon) icsk_mtup;
    u32 icsk_user_timeout;
    u64 icsk_ca_priv[13];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct inet_connection_sock {
    struct inet_sock icsk_inet;
    struct request_sock_queue icsk_accept_queue;
    struct inet_bind_bucket *icsk_bind_hash;
    long unsigned int icsk_timeout;
    struct timer_list icsk_retransmit_timer;
    struct timer_list icsk_delack_timer;
    __u32 icsk_rto;
    __u32 icsk_pmtu_cookie;
    const struct tcp_congestion_ops *icsk_ca_ops;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    const struct tcp_ulp_ops *icsk_ulp_ops;
    void *icsk_ulp_data;
    void (*icsk_clean_acked)(struct sock *, u32);
    struct hlist_node icsk_listen_portaddr_node;
    unsigned int (*icsk_sync_mss)(struct sock *, u32);
    __u8 icsk_ca_state;
    __u8 icsk_ca_setsockopt;
    __u8 icsk_ca_dst_locked;
    __u8 icsk_retransmits;
    __u8 icsk_pending;
    __u8 icsk_backoff;
    __u8 icsk_syn_retries;
    __u8 icsk_probes_out;
    __u16 icsk_ext_hdr_len;
    struct (anon) icsk_ack;
    struct (anon) icsk_mtup;
    u32 icsk_user_timeout;
    u64 icsk_ca_priv[13];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct inet_connection_sock {
    struct inet_sock icsk_inet;
    struct request_sock_queue icsk_accept_queue;
    struct inet_bind_bucket *icsk_bind_hash;
    long unsigned int icsk_timeout;
    struct timer_list icsk_retransmit_timer;
    struct timer_list icsk_delack_timer;
    __u32 icsk_rto;
    __u32 icsk_pmtu_cookie;
    const struct tcp_congestion_ops *icsk_ca_ops;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    const struct tcp_ulp_ops *icsk_ulp_ops;
    void *icsk_ulp_data;
    void (*icsk_clean_acked)(struct sock *, u32);
    struct hlist_node icsk_listen_portaddr_node;
    unsigned int (*icsk_sync_mss)(struct sock *, u32);
    __u8 icsk_ca_state;
    __u8 icsk_ca_setsockopt;
    __u8 icsk_ca_dst_locked;
    __u8 icsk_retransmits;
    __u8 icsk_pending;
    __u8 icsk_backoff;
    __u8 icsk_syn_retries;
    __u8 icsk_probes_out;
    __u16 icsk_ext_hdr_len;
    struct (anon) icsk_ack;
    struct (anon) icsk_mtup;
    u32 icsk_user_timeout;
    u64 icsk_ca_priv[13];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct inet_connection_sock {
    struct inet_sock icsk_inet;
    struct request_sock_queue icsk_accept_queue;
    struct inet_bind_bucket *icsk_bind_hash;
    long unsigned int icsk_timeout;
    struct timer_list icsk_retransmit_timer;
    struct timer_list icsk_delack_timer;
    __u32 icsk_rto;
    __u32 icsk_pmtu_cookie;
    const struct tcp_congestion_ops *icsk_ca_ops;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    const struct tcp_ulp_ops *icsk_ulp_ops;
    void *icsk_ulp_data;
    void (*icsk_clean_acked)(struct sock *, u32);
    struct hlist_node icsk_listen_portaddr_node;
    unsigned int (*icsk_sync_mss)(struct sock *, u32);
    __u8 icsk_ca_state;
    __u8 icsk_ca_setsockopt;
    __u8 icsk_ca_dst_locked;
    __u8 icsk_retransmits;
    __u8 icsk_pending;
    __u8 icsk_backoff;
    __u8 icsk_syn_retries;
    __u8 icsk_probes_out;
    __u16 icsk_ext_hdr_len;
    struct (anon) icsk_ack;
    struct (anon) icsk_mtup;
    u32 icsk_user_timeout;
    u64 icsk_ca_priv[13];
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
struct inet_connection_sock {
    struct inet_sock icsk_inet;
    struct request_sock_queue icsk_accept_queue;
    struct inet_bind_bucket *icsk_bind_hash;
    long unsigned int icsk_timeout;
    struct timer_list icsk_retransmit_timer;
    struct timer_list icsk_delack_timer;
    __u32 icsk_rto;
    __u32 icsk_pmtu_cookie;
    const struct tcp_congestion_ops *icsk_ca_ops;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    const struct tcp_ulp_ops *icsk_ulp_ops;
    void *icsk_ulp_data;
    void (*icsk_clean_acked)(struct sock *, u32);
    struct hlist_node icsk_listen_portaddr_node;
    unsigned int (*icsk_sync_mss)(struct sock *, u32);
    __u8 icsk_ca_state;
    __u8 icsk_ca_setsockopt;
    __u8 icsk_ca_dst_locked;
    __u8 icsk_retransmits;
    __u8 icsk_pending;
    __u8 icsk_backoff;
    __u8 icsk_syn_retries;
    __u8 icsk_probes_out;
    __u16 icsk_ext_hdr_len;
    struct (anon) icsk_ack;
    struct (anon) icsk_mtup;
    u32 icsk_user_timeout;
    u64 icsk_ca_priv[13];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct inet_connection_sock {
    struct inet_sock icsk_inet;
    struct request_sock_queue icsk_accept_queue;
    struct inet_bind_bucket *icsk_bind_hash;
    long unsigned int icsk_timeout;
    struct timer_list icsk_retransmit_timer;
    struct timer_list icsk_delack_timer;
    __u32 icsk_rto;
    __u32 icsk_pmtu_cookie;
    const struct tcp_congestion_ops *icsk_ca_ops;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    const struct tcp_ulp_ops *icsk_ulp_ops;
    void *icsk_ulp_data;
    void (*icsk_clean_acked)(struct sock *, u32);
    struct hlist_node icsk_listen_portaddr_node;
    unsigned int (*icsk_sync_mss)(struct sock *, u32);
    __u8 icsk_ca_state;
    __u8 icsk_ca_setsockopt;
    __u8 icsk_ca_dst_locked;
    __u8 icsk_retransmits;
    __u8 icsk_pending;
    __u8 icsk_backoff;
    __u8 icsk_syn_retries;
    __u8 icsk_probes_out;
    __u16 icsk_ext_hdr_len;
    struct (anon) icsk_ack;
    struct (anon) icsk_mtup;
    u32 icsk_user_timeout;
    u64 icsk_ca_priv[13];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct inet_connection_sock {
    struct inet_sock icsk_inet;
    struct request_sock_queue icsk_accept_queue;
    struct inet_bind_bucket *icsk_bind_hash;
    long unsigned int icsk_timeout;
    struct timer_list icsk_retransmit_timer;
    struct timer_list icsk_delack_timer;
    __u32 icsk_rto;
    __u32 icsk_pmtu_cookie;
    const struct tcp_congestion_ops *icsk_ca_ops;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    const struct tcp_ulp_ops *icsk_ulp_ops;
    void *icsk_ulp_data;
    void (*icsk_clean_acked)(struct sock *, u32);
    struct hlist_node icsk_listen_portaddr_node;
    unsigned int (*icsk_sync_mss)(struct sock *, u32);
    __u8 icsk_ca_state;
    __u8 icsk_ca_setsockopt;
    __u8 icsk_ca_dst_locked;
    __u8 icsk_retransmits;
    __u8 icsk_pending;
    __u8 icsk_backoff;
    __u8 icsk_syn_retries;
    __u8 icsk_probes_out;
    __u16 icsk_ext_hdr_len;
    struct (anon) icsk_ack;
    struct (anon) icsk_mtup;
    u32 icsk_user_timeout;
    u64 icsk_ca_priv[13];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct inet_connection_sock {
    struct inet_sock icsk_inet;
    struct request_sock_queue icsk_accept_queue;
    struct inet_bind_bucket *icsk_bind_hash;
    long unsigned int icsk_timeout;
    struct timer_list icsk_retransmit_timer;
    struct timer_list icsk_delack_timer;
    __u32 icsk_rto;
    __u32 icsk_pmtu_cookie;
    const struct tcp_congestion_ops *icsk_ca_ops;
    const struct inet_connection_sock_af_ops *icsk_af_ops;
    const struct tcp_ulp_ops *icsk_ulp_ops;
    void *icsk_ulp_data;
    void (*icsk_clean_acked)(struct sock *, u32);
    struct hlist_node icsk_listen_portaddr_node;
    unsigned int (*icsk_sync_mss)(struct sock *, u32);
    __u8 icsk_ca_state;
    __u8 icsk_ca_setsockopt;
    __u8 icsk_ca_dst_locked;
    __u8 icsk_retransmits;
    __u8 icsk_pending;
    __u8 icsk_backoff;
    __u8 icsk_syn_retries;
    __u8 icsk_probes_out;
    __u16 icsk_ext_hdr_len;
    struct (anon) icsk_ack;
    struct (anon) icsk_mtup;
    u32 icsk_user_timeout;
    u64 icsk_ca_priv[13];
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
<b>Field type changed. </b>
<code>u64 icsk_ca_priv[8]</code> ➡️ <code>u64 icsk_ca_priv[11]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const struct tcp_ulp_ops *icsk_ulp_ops</code>
</li>
<li>
<b>Field added. </b>
<code>void *icsk_ulp_data</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*icsk_clean_acked)(struct sock *, u32)</code>
</li>
<li>
<b>Field added. </b>
<code>struct hlist_node icsk_listen_portaddr_node</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>u64 icsk_ca_priv[11]</code> ➡️ <code>u64 icsk_ca_priv[13]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u32 icsk_rto_min</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 icsk_delack_max</code>
</li>
<li>
<b>Field added. </b>
<code>__u8 icsk_ca_initialized</code>
</li>
<li>
<b>Field added. </b>
<code>u32 icsk_probes_tstamp</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct hlist_node icsk_listen_portaddr_node</code>
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
<code>struct inet_bind2_bucket *icsk_bind2_hash</code>
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
