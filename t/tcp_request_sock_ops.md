# Struct: <code>tcp_request_sock_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct tcp_request_sock_ops {
    u16 mss_clamp;
    struct tcp_md5sig_key * (*req_md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    void (*init_req)(struct request_sock *, const struct sock *, struct sk_buff *);
    __u32 (*cookie_init_seq)(const struct sk_buff *, __u16 *);
    struct dst_entry * (*route_req)(const struct sock *, struct flowi *, const struct request_sock *, bool *);
    __u32 (*init_seq)(const struct sk_buff *);
    int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct tcp_request_sock_ops {
    u16 mss_clamp;
    struct tcp_md5sig_key * (*req_md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    void (*init_req)(struct request_sock *, const struct sock *, struct sk_buff *);
    __u32 (*cookie_init_seq)(const struct sk_buff *, __u16 *);
    struct dst_entry * (*route_req)(const struct sock *, struct flowi *, const struct request_sock *, bool *);
    __u32 (*init_seq)(const struct sk_buff *);
    int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, enum tcp_synack_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct tcp_request_sock_ops {
    u16 mss_clamp;
    struct tcp_md5sig_key * (*req_md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    void (*init_req)(struct request_sock *, const struct sock *, struct sk_buff *);
    __u32 (*cookie_init_seq)(const struct sk_buff *, __u16 *);
    struct dst_entry * (*route_req)(const struct sock *, struct flowi *, const struct request_sock *, bool *);
    __u32 (*init_seq)(const struct sk_buff *, u32 *);
    int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, enum tcp_synack_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct tcp_request_sock_ops {
    u16 mss_clamp;
    struct tcp_md5sig_key * (*req_md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    void (*init_req)(struct request_sock *, const struct sock *, struct sk_buff *);
    __u32 (*cookie_init_seq)(const struct sk_buff *, __u16 *);
    struct dst_entry * (*route_req)(const struct sock *, struct flowi *, const struct request_sock *);
    u32 (*init_seq)(const struct sk_buff *);
    u32 (*init_ts_off)(const struct net *, const struct sk_buff *);
    int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, enum tcp_synack_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct tcp_request_sock_ops {
    u16 mss_clamp;
    struct tcp_md5sig_key * (*req_md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    void (*init_req)(struct request_sock *, const struct sock *, struct sk_buff *);
    __u32 (*cookie_init_seq)(const struct sk_buff *, __u16 *);
    struct dst_entry * (*route_req)(const struct sock *, struct flowi *, const struct request_sock *);
    u32 (*init_seq)(const struct sk_buff *);
    u32 (*init_ts_off)(const struct net *, const struct sk_buff *);
    int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, enum tcp_synack_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct tcp_request_sock_ops {
    u16 mss_clamp;
    struct tcp_md5sig_key * (*req_md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    void (*init_req)(struct request_sock *, const struct sock *, struct sk_buff *);
    __u32 (*cookie_init_seq)(const struct sk_buff *, __u16 *);
    struct dst_entry * (*route_req)(const struct sock *, struct flowi *, const struct request_sock *);
    u32 (*init_seq)(const struct sk_buff *);
    u32 (*init_ts_off)(const struct net *, const struct sk_buff *);
    int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, enum tcp_synack_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct tcp_request_sock_ops {
    u16 mss_clamp;
    struct tcp_md5sig_key * (*req_md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    void (*init_req)(struct request_sock *, const struct sock *, struct sk_buff *);
    __u32 (*cookie_init_seq)(const struct sk_buff *, __u16 *);
    struct dst_entry * (*route_req)(const struct sock *, struct flowi *, const struct request_sock *);
    u32 (*init_seq)(const struct sk_buff *);
    u32 (*init_ts_off)(const struct net *, const struct sk_buff *);
    int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, enum tcp_synack_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct tcp_request_sock_ops {
    u16 mss_clamp;
    struct tcp_md5sig_key * (*req_md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    void (*init_req)(struct request_sock *, const struct sock *, struct sk_buff *);
    __u32 (*cookie_init_seq)(const struct sk_buff *, __u16 *);
    struct dst_entry * (*route_req)(const struct sock *, struct flowi *, const struct request_sock *);
    u32 (*init_seq)(const struct sk_buff *);
    u32 (*init_ts_off)(const struct net *, const struct sk_buff *);
    int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, enum tcp_synack_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct tcp_request_sock_ops {
    u16 mss_clamp;
    struct tcp_md5sig_key * (*req_md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    void (*init_req)(struct request_sock *, const struct sock *, struct sk_buff *);
    __u32 (*cookie_init_seq)(const struct sk_buff *, __u16 *);
    struct dst_entry * (*route_req)(const struct sock *, struct flowi *, const struct request_sock *);
    u32 (*init_seq)(const struct sk_buff *);
    u32 (*init_ts_off)(const struct net *, const struct sk_buff *);
    int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, enum tcp_synack_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct tcp_request_sock_ops {
    u16 mss_clamp;
    struct tcp_md5sig_key * (*req_md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    void (*init_req)(struct request_sock *, const struct sock *, struct sk_buff *);
    __u32 (*cookie_init_seq)(const struct sk_buff *, __u16 *);
    struct dst_entry * (*route_req)(const struct sock *, struct flowi *, const struct request_sock *);
    u32 (*init_seq)(const struct sk_buff *);
    u32 (*init_ts_off)(const struct net *, const struct sk_buff *);
    int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, enum tcp_synack_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct tcp_request_sock_ops {
    u16 mss_clamp;
    struct tcp_md5sig_key * (*req_md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    __u32 (*cookie_init_seq)(const struct sk_buff *, __u16 *);
    struct dst_entry * (*route_req)(const struct sock *, struct sk_buff *, struct flowi *, struct request_sock *);
    u32 (*init_seq)(const struct sk_buff *);
    u32 (*init_ts_off)(const struct net *, const struct sk_buff *);
    int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, enum tcp_synack_type, struct sk_buff *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct tcp_request_sock_ops {
    u16 mss_clamp;
    struct tcp_md5sig_key * (*req_md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    __u32 (*cookie_init_seq)(const struct sk_buff *, __u16 *);
    struct dst_entry * (*route_req)(const struct sock *, struct sk_buff *, struct flowi *, struct request_sock *);
    u32 (*init_seq)(const struct sk_buff *);
    u32 (*init_ts_off)(const struct net *, const struct sk_buff *);
    int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, enum tcp_synack_type, struct sk_buff *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct tcp_request_sock_ops {
    u16 mss_clamp;
    struct tcp_md5sig_key * (*req_md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    __u32 (*cookie_init_seq)(const struct sk_buff *, __u16 *);
    struct dst_entry * (*route_req)(const struct sock *, struct sk_buff *, struct flowi *, struct request_sock *);
    u32 (*init_seq)(const struct sk_buff *);
    u32 (*init_ts_off)(const struct net *, const struct sk_buff *);
    int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, enum tcp_synack_type, struct sk_buff *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct tcp_request_sock_ops {
    u16 mss_clamp;
    struct tcp_md5sig_key * (*req_md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    __u32 (*cookie_init_seq)(const struct sk_buff *, __u16 *);
    struct dst_entry * (*route_req)(const struct sock *, struct sk_buff *, struct flowi *, struct request_sock *);
    u32 (*init_seq)(const struct sk_buff *);
    u32 (*init_ts_off)(const struct net *, const struct sk_buff *);
    int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, enum tcp_synack_type, struct sk_buff *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct tcp_request_sock_ops {
    u16 mss_clamp;
    struct tcp_md5sig_key * (*req_md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    __u32 (*cookie_init_seq)(const struct sk_buff *, __u16 *);
    struct dst_entry * (*route_req)(const struct sock *, struct sk_buff *, struct flowi *, struct request_sock *);
    u32 (*init_seq)(const struct sk_buff *);
    u32 (*init_ts_off)(const struct net *, const struct sk_buff *);
    int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, enum tcp_synack_type, struct sk_buff *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct tcp_request_sock_ops {
    u16 mss_clamp;
    struct tcp_md5sig_key * (*req_md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    __u32 (*cookie_init_seq)(const struct sk_buff *, __u16 *);
    struct dst_entry * (*route_req)(const struct sock *, struct sk_buff *, struct flowi *, struct request_sock *);
    u32 (*init_seq)(const struct sk_buff *);
    u32 (*init_ts_off)(const struct net *, const struct sk_buff *);
    int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, enum tcp_synack_type, struct sk_buff *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct tcp_request_sock_ops {
    u16 mss_clamp;
    struct tcp_md5sig_key * (*req_md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    struct tcp_ao_key * (*ao_lookup)(const struct sock *, struct request_sock *, int, int);
    int (*ao_calc_key)(struct tcp_ao_key *, u8 *, struct request_sock *);
    int (*ao_synack_hash)(char *, struct tcp_ao_key *, struct request_sock *, const struct sk_buff *, int, u32);
    __u32 (*cookie_init_seq)(const struct sk_buff *, __u16 *);
    struct dst_entry * (*route_req)(const struct sock *, struct sk_buff *, struct flowi *, struct request_sock *);
    u32 (*init_seq)(const struct sk_buff *);
    u32 (*init_ts_off)(const struct net *, const struct sk_buff *);
    int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, enum tcp_synack_type, struct sk_buff *);
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
struct tcp_request_sock_ops {
    u16 mss_clamp;
    struct tcp_md5sig_key * (*req_md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    void (*init_req)(struct request_sock *, const struct sock *, struct sk_buff *);
    __u32 (*cookie_init_seq)(const struct sk_buff *, __u16 *);
    struct dst_entry * (*route_req)(const struct sock *, struct flowi *, const struct request_sock *);
    u32 (*init_seq)(const struct sk_buff *);
    u32 (*init_ts_off)(const struct net *, const struct sk_buff *);
    int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, enum tcp_synack_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct tcp_request_sock_ops {
    u16 mss_clamp;
    struct tcp_md5sig_key * (*req_md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    void (*init_req)(struct request_sock *, const struct sock *, struct sk_buff *);
    __u32 (*cookie_init_seq)(const struct sk_buff *, __u16 *);
    struct dst_entry * (*route_req)(const struct sock *, struct flowi *, const struct request_sock *);
    u32 (*init_seq)(const struct sk_buff *);
    u32 (*init_ts_off)(const struct net *, const struct sk_buff *);
    int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, enum tcp_synack_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct tcp_request_sock_ops {
    u16 mss_clamp;
    struct tcp_md5sig_key * (*req_md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    void (*init_req)(struct request_sock *, const struct sock *, struct sk_buff *);
    __u32 (*cookie_init_seq)(const struct sk_buff *, __u16 *);
    struct dst_entry * (*route_req)(const struct sock *, struct flowi *, const struct request_sock *);
    u32 (*init_seq)(const struct sk_buff *);
    u32 (*init_ts_off)(const struct net *, const struct sk_buff *);
    int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, enum tcp_synack_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct tcp_request_sock_ops {
    u16 mss_clamp;
    struct tcp_md5sig_key * (*req_md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    void (*init_req)(struct request_sock *, const struct sock *, struct sk_buff *);
    __u32 (*cookie_init_seq)(const struct sk_buff *, __u16 *);
    struct dst_entry * (*route_req)(const struct sock *, struct flowi *, const struct request_sock *);
    u32 (*init_seq)(const struct sk_buff *);
    u32 (*init_ts_off)(const struct net *, const struct sk_buff *);
    int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, enum tcp_synack_type);
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
struct tcp_request_sock_ops {
    u16 mss_clamp;
    struct tcp_md5sig_key * (*req_md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    void (*init_req)(struct request_sock *, const struct sock *, struct sk_buff *);
    __u32 (*cookie_init_seq)(const struct sk_buff *, __u16 *);
    struct dst_entry * (*route_req)(const struct sock *, struct flowi *, const struct request_sock *);
    u32 (*init_seq)(const struct sk_buff *);
    u32 (*init_ts_off)(const struct net *, const struct sk_buff *);
    int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, enum tcp_synack_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct tcp_request_sock_ops {
    u16 mss_clamp;
    struct tcp_md5sig_key * (*req_md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    void (*init_req)(struct request_sock *, const struct sock *, struct sk_buff *);
    __u32 (*cookie_init_seq)(const struct sk_buff *, __u16 *);
    struct dst_entry * (*route_req)(const struct sock *, struct flowi *, const struct request_sock *);
    u32 (*init_seq)(const struct sk_buff *);
    u32 (*init_ts_off)(const struct net *, const struct sk_buff *);
    int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, enum tcp_synack_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct tcp_request_sock_ops {
    u16 mss_clamp;
    struct tcp_md5sig_key * (*req_md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    void (*init_req)(struct request_sock *, const struct sock *, struct sk_buff *);
    __u32 (*cookie_init_seq)(const struct sk_buff *, __u16 *);
    struct dst_entry * (*route_req)(const struct sock *, struct flowi *, const struct request_sock *);
    u32 (*init_seq)(const struct sk_buff *);
    u32 (*init_ts_off)(const struct net *, const struct sk_buff *);
    int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, enum tcp_synack_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct tcp_request_sock_ops {
    u16 mss_clamp;
    struct tcp_md5sig_key * (*req_md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    void (*init_req)(struct request_sock *, const struct sock *, struct sk_buff *);
    __u32 (*cookie_init_seq)(const struct sk_buff *, __u16 *);
    struct dst_entry * (*route_req)(const struct sock *, struct flowi *, const struct request_sock *);
    u32 (*init_seq)(const struct sk_buff *);
    u32 (*init_ts_off)(const struct net *, const struct sk_buff *);
    int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, enum tcp_synack_type);
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, bool)</code> ➡️ <code>int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, enum tcp_synack_type)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>__u32 (*init_seq)(const struct sk_buff *)</code> ➡️ <code>__u32 (*init_seq)(const struct sk_buff *, u32 *)</code>
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
<code>u32 (*init_ts_off)(const struct net *, const struct sk_buff *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct dst_entry * (*route_req)(const struct sock *, struct flowi *, const struct request_sock *, bool *)</code> ➡️ <code>struct dst_entry * (*route_req)(const struct sock *, struct flowi *, const struct request_sock *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u32 (*init_seq)(const struct sk_buff *, u32 *)</code> ➡️ <code>u32 (*init_seq)(const struct sk_buff *)</code>
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
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>void (*init_req)(struct request_sock *, const struct sock *, struct sk_buff *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct dst_entry * (*route_req)(const struct sock *, struct flowi *, const struct request_sock *)</code> ➡️ <code>struct dst_entry * (*route_req)(const struct sock *, struct sk_buff *, struct flowi *, struct request_sock *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, enum tcp_synack_type)</code> ➡️ <code>int (*send_synack)(const struct sock *, struct dst_entry *, struct flowi *, struct request_sock *, struct tcp_fastopen_cookie *, enum tcp_synack_type, struct sk_buff *)</code>
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
<code>struct tcp_ao_key * (*ao_lookup)(const struct sock *, struct request_sock *, int, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*ao_calc_key)(struct tcp_ao_key *, u8 *, struct request_sock *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*ao_synack_hash)(char *, struct tcp_ao_key *, struct request_sock *, const struct sk_buff *, int, u32)</code>
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
