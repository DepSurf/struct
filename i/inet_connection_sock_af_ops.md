# Struct: <code>inet_connection_sock_af_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct inet_connection_sock_af_ops {
    int (*queue_xmit)(struct sock *, struct sk_buff *, struct flowi *);
    void (*send_check)(struct sock *, struct sk_buff *);
    int (*rebuild_header)(struct sock *);
    void (*sk_rx_dst_set)(struct sock *, const struct sk_buff *);
    int (*conn_request)(struct sock *, struct sk_buff *);
    struct sock * (*syn_recv_sock)(const struct sock *, struct sk_buff *, struct request_sock *, struct dst_entry *, struct request_sock *, bool *);
    u16 net_header_len;
    u16 net_frag_header_len;
    u16 sockaddr_len;
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*addr2sockaddr)(struct sock *, struct sockaddr *);
    int (*bind_conflict)(const struct sock *, const struct inet_bind_bucket *, bool);
    void (*mtu_reduced)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct inet_connection_sock_af_ops {
    int (*queue_xmit)(struct sock *, struct sk_buff *, struct flowi *);
    void (*send_check)(struct sock *, struct sk_buff *);
    int (*rebuild_header)(struct sock *);
    void (*sk_rx_dst_set)(struct sock *, const struct sk_buff *);
    int (*conn_request)(struct sock *, struct sk_buff *);
    struct sock * (*syn_recv_sock)(const struct sock *, struct sk_buff *, struct request_sock *, struct dst_entry *, struct request_sock *, bool *);
    u16 net_header_len;
    u16 net_frag_header_len;
    u16 sockaddr_len;
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*addr2sockaddr)(struct sock *, struct sockaddr *);
    int (*bind_conflict)(const struct sock *, const struct inet_bind_bucket *, bool);
    void (*mtu_reduced)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct inet_connection_sock_af_ops {
    int (*queue_xmit)(struct sock *, struct sk_buff *, struct flowi *);
    void (*send_check)(struct sock *, struct sk_buff *);
    int (*rebuild_header)(struct sock *);
    void (*sk_rx_dst_set)(struct sock *, const struct sk_buff *);
    int (*conn_request)(struct sock *, struct sk_buff *);
    struct sock * (*syn_recv_sock)(const struct sock *, struct sk_buff *, struct request_sock *, struct dst_entry *, struct request_sock *, bool *);
    u16 net_header_len;
    u16 net_frag_header_len;
    u16 sockaddr_len;
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*addr2sockaddr)(struct sock *, struct sockaddr *);
    int (*bind_conflict)(const struct sock *, const struct inet_bind_bucket *, bool, bool);
    void (*mtu_reduced)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct inet_connection_sock_af_ops {
    int (*queue_xmit)(struct sock *, struct sk_buff *, struct flowi *);
    void (*send_check)(struct sock *, struct sk_buff *);
    int (*rebuild_header)(struct sock *);
    void (*sk_rx_dst_set)(struct sock *, const struct sk_buff *);
    int (*conn_request)(struct sock *, struct sk_buff *);
    struct sock * (*syn_recv_sock)(const struct sock *, struct sk_buff *, struct request_sock *, struct dst_entry *, struct request_sock *, bool *);
    u16 net_header_len;
    u16 net_frag_header_len;
    u16 sockaddr_len;
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*addr2sockaddr)(struct sock *, struct sockaddr *);
    void (*mtu_reduced)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct inet_connection_sock_af_ops {
    int (*queue_xmit)(struct sock *, struct sk_buff *, struct flowi *);
    void (*send_check)(struct sock *, struct sk_buff *);
    int (*rebuild_header)(struct sock *);
    void (*sk_rx_dst_set)(struct sock *, const struct sk_buff *);
    int (*conn_request)(struct sock *, struct sk_buff *);
    struct sock * (*syn_recv_sock)(const struct sock *, struct sk_buff *, struct request_sock *, struct dst_entry *, struct request_sock *, bool *);
    u16 net_header_len;
    u16 net_frag_header_len;
    u16 sockaddr_len;
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*addr2sockaddr)(struct sock *, struct sockaddr *);
    void (*mtu_reduced)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct inet_connection_sock_af_ops {
    int (*queue_xmit)(struct sock *, struct sk_buff *, struct flowi *);
    void (*send_check)(struct sock *, struct sk_buff *);
    int (*rebuild_header)(struct sock *);
    void (*sk_rx_dst_set)(struct sock *, const struct sk_buff *);
    int (*conn_request)(struct sock *, struct sk_buff *);
    struct sock * (*syn_recv_sock)(const struct sock *, struct sk_buff *, struct request_sock *, struct dst_entry *, struct request_sock *, bool *);
    u16 net_header_len;
    u16 net_frag_header_len;
    u16 sockaddr_len;
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*addr2sockaddr)(struct sock *, struct sockaddr *);
    void (*mtu_reduced)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct inet_connection_sock_af_ops {
    int (*queue_xmit)(struct sock *, struct sk_buff *, struct flowi *);
    void (*send_check)(struct sock *, struct sk_buff *);
    int (*rebuild_header)(struct sock *);
    void (*sk_rx_dst_set)(struct sock *, const struct sk_buff *);
    int (*conn_request)(struct sock *, struct sk_buff *);
    struct sock * (*syn_recv_sock)(const struct sock *, struct sk_buff *, struct request_sock *, struct dst_entry *, struct request_sock *, bool *);
    u16 net_header_len;
    u16 net_frag_header_len;
    u16 sockaddr_len;
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*addr2sockaddr)(struct sock *, struct sockaddr *);
    void (*mtu_reduced)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct inet_connection_sock_af_ops {
    int (*queue_xmit)(struct sock *, struct sk_buff *, struct flowi *);
    void (*send_check)(struct sock *, struct sk_buff *);
    int (*rebuild_header)(struct sock *);
    void (*sk_rx_dst_set)(struct sock *, const struct sk_buff *);
    int (*conn_request)(struct sock *, struct sk_buff *);
    struct sock * (*syn_recv_sock)(const struct sock *, struct sk_buff *, struct request_sock *, struct dst_entry *, struct request_sock *, bool *);
    u16 net_header_len;
    u16 net_frag_header_len;
    u16 sockaddr_len;
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*addr2sockaddr)(struct sock *, struct sockaddr *);
    void (*mtu_reduced)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct inet_connection_sock_af_ops {
    int (*queue_xmit)(struct sock *, struct sk_buff *, struct flowi *);
    void (*send_check)(struct sock *, struct sk_buff *);
    int (*rebuild_header)(struct sock *);
    void (*sk_rx_dst_set)(struct sock *, const struct sk_buff *);
    int (*conn_request)(struct sock *, struct sk_buff *);
    struct sock * (*syn_recv_sock)(const struct sock *, struct sk_buff *, struct request_sock *, struct dst_entry *, struct request_sock *, bool *);
    u16 net_header_len;
    u16 net_frag_header_len;
    u16 sockaddr_len;
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*addr2sockaddr)(struct sock *, struct sockaddr *);
    void (*mtu_reduced)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct inet_connection_sock_af_ops {
    int (*queue_xmit)(struct sock *, struct sk_buff *, struct flowi *);
    void (*send_check)(struct sock *, struct sk_buff *);
    int (*rebuild_header)(struct sock *);
    void (*sk_rx_dst_set)(struct sock *, const struct sk_buff *);
    int (*conn_request)(struct sock *, struct sk_buff *);
    struct sock * (*syn_recv_sock)(const struct sock *, struct sk_buff *, struct request_sock *, struct dst_entry *, struct request_sock *, bool *);
    u16 net_header_len;
    u16 net_frag_header_len;
    u16 sockaddr_len;
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*addr2sockaddr)(struct sock *, struct sockaddr *);
    void (*mtu_reduced)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct inet_connection_sock_af_ops {
    int (*queue_xmit)(struct sock *, struct sk_buff *, struct flowi *);
    void (*send_check)(struct sock *, struct sk_buff *);
    int (*rebuild_header)(struct sock *);
    void (*sk_rx_dst_set)(struct sock *, const struct sk_buff *);
    int (*conn_request)(struct sock *, struct sk_buff *);
    struct sock * (*syn_recv_sock)(const struct sock *, struct sk_buff *, struct request_sock *, struct dst_entry *, struct request_sock *, bool *);
    u16 net_header_len;
    u16 net_frag_header_len;
    u16 sockaddr_len;
    int (*setsockopt)(struct sock *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*addr2sockaddr)(struct sock *, struct sockaddr *);
    void (*mtu_reduced)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct inet_connection_sock_af_ops {
    int (*queue_xmit)(struct sock *, struct sk_buff *, struct flowi *);
    void (*send_check)(struct sock *, struct sk_buff *);
    int (*rebuild_header)(struct sock *);
    void (*sk_rx_dst_set)(struct sock *, const struct sk_buff *);
    int (*conn_request)(struct sock *, struct sk_buff *);
    struct sock * (*syn_recv_sock)(const struct sock *, struct sk_buff *, struct request_sock *, struct dst_entry *, struct request_sock *, bool *);
    u16 net_header_len;
    u16 net_frag_header_len;
    u16 sockaddr_len;
    int (*setsockopt)(struct sock *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*addr2sockaddr)(struct sock *, struct sockaddr *);
    void (*mtu_reduced)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct inet_connection_sock_af_ops {
    int (*queue_xmit)(struct sock *, struct sk_buff *, struct flowi *);
    void (*send_check)(struct sock *, struct sk_buff *);
    int (*rebuild_header)(struct sock *);
    void (*sk_rx_dst_set)(struct sock *, const struct sk_buff *);
    int (*conn_request)(struct sock *, struct sk_buff *);
    struct sock * (*syn_recv_sock)(const struct sock *, struct sk_buff *, struct request_sock *, struct dst_entry *, struct request_sock *, bool *);
    u16 net_header_len;
    u16 net_frag_header_len;
    u16 sockaddr_len;
    int (*setsockopt)(struct sock *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*addr2sockaddr)(struct sock *, struct sockaddr *);
    void (*mtu_reduced)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct inet_connection_sock_af_ops {
    int (*queue_xmit)(struct sock *, struct sk_buff *, struct flowi *);
    void (*send_check)(struct sock *, struct sk_buff *);
    int (*rebuild_header)(struct sock *);
    void (*sk_rx_dst_set)(struct sock *, const struct sk_buff *);
    int (*conn_request)(struct sock *, struct sk_buff *);
    struct sock * (*syn_recv_sock)(const struct sock *, struct sk_buff *, struct request_sock *, struct dst_entry *, struct request_sock *, bool *);
    u16 net_header_len;
    u16 net_frag_header_len;
    u16 sockaddr_len;
    int (*setsockopt)(struct sock *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*addr2sockaddr)(struct sock *, struct sockaddr *);
    void (*mtu_reduced)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct inet_connection_sock_af_ops {
    int (*queue_xmit)(struct sock *, struct sk_buff *, struct flowi *);
    void (*send_check)(struct sock *, struct sk_buff *);
    int (*rebuild_header)(struct sock *);
    void (*sk_rx_dst_set)(struct sock *, const struct sk_buff *);
    int (*conn_request)(struct sock *, struct sk_buff *);
    struct sock * (*syn_recv_sock)(const struct sock *, struct sk_buff *, struct request_sock *, struct dst_entry *, struct request_sock *, bool *);
    u16 net_header_len;
    u16 net_frag_header_len;
    u16 sockaddr_len;
    int (*setsockopt)(struct sock *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*addr2sockaddr)(struct sock *, struct sockaddr *);
    void (*mtu_reduced)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct inet_connection_sock_af_ops {
    int (*queue_xmit)(struct sock *, struct sk_buff *, struct flowi *);
    void (*send_check)(struct sock *, struct sk_buff *);
    int (*rebuild_header)(struct sock *);
    void (*sk_rx_dst_set)(struct sock *, const struct sk_buff *);
    int (*conn_request)(struct sock *, struct sk_buff *);
    struct sock * (*syn_recv_sock)(const struct sock *, struct sk_buff *, struct request_sock *, struct dst_entry *, struct request_sock *, bool *);
    u16 net_header_len;
    u16 net_frag_header_len;
    u16 sockaddr_len;
    int (*setsockopt)(struct sock *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*addr2sockaddr)(struct sock *, struct sockaddr *);
    void (*mtu_reduced)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct inet_connection_sock_af_ops {
    int (*queue_xmit)(struct sock *, struct sk_buff *, struct flowi *);
    void (*send_check)(struct sock *, struct sk_buff *);
    int (*rebuild_header)(struct sock *);
    void (*sk_rx_dst_set)(struct sock *, const struct sk_buff *);
    int (*conn_request)(struct sock *, struct sk_buff *);
    struct sock * (*syn_recv_sock)(const struct sock *, struct sk_buff *, struct request_sock *, struct dst_entry *, struct request_sock *, bool *);
    u16 net_header_len;
    u16 sockaddr_len;
    int (*setsockopt)(struct sock *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*addr2sockaddr)(struct sock *, struct sockaddr *);
    void (*mtu_reduced)(struct sock *);
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
struct inet_connection_sock_af_ops {
    int (*queue_xmit)(struct sock *, struct sk_buff *, struct flowi *);
    void (*send_check)(struct sock *, struct sk_buff *);
    int (*rebuild_header)(struct sock *);
    void (*sk_rx_dst_set)(struct sock *, const struct sk_buff *);
    int (*conn_request)(struct sock *, struct sk_buff *);
    struct sock * (*syn_recv_sock)(const struct sock *, struct sk_buff *, struct request_sock *, struct dst_entry *, struct request_sock *, bool *);
    u16 net_header_len;
    u16 net_frag_header_len;
    u16 sockaddr_len;
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*addr2sockaddr)(struct sock *, struct sockaddr *);
    void (*mtu_reduced)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct inet_connection_sock_af_ops {
    int (*queue_xmit)(struct sock *, struct sk_buff *, struct flowi *);
    void (*send_check)(struct sock *, struct sk_buff *);
    int (*rebuild_header)(struct sock *);
    void (*sk_rx_dst_set)(struct sock *, const struct sk_buff *);
    int (*conn_request)(struct sock *, struct sk_buff *);
    struct sock * (*syn_recv_sock)(const struct sock *, struct sk_buff *, struct request_sock *, struct dst_entry *, struct request_sock *, bool *);
    u16 net_header_len;
    u16 net_frag_header_len;
    u16 sockaddr_len;
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*addr2sockaddr)(struct sock *, struct sockaddr *);
    void (*mtu_reduced)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct inet_connection_sock_af_ops {
    int (*queue_xmit)(struct sock *, struct sk_buff *, struct flowi *);
    void (*send_check)(struct sock *, struct sk_buff *);
    int (*rebuild_header)(struct sock *);
    void (*sk_rx_dst_set)(struct sock *, const struct sk_buff *);
    int (*conn_request)(struct sock *, struct sk_buff *);
    struct sock * (*syn_recv_sock)(const struct sock *, struct sk_buff *, struct request_sock *, struct dst_entry *, struct request_sock *, bool *);
    u16 net_header_len;
    u16 net_frag_header_len;
    u16 sockaddr_len;
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*addr2sockaddr)(struct sock *, struct sockaddr *);
    void (*mtu_reduced)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct inet_connection_sock_af_ops {
    int (*queue_xmit)(struct sock *, struct sk_buff *, struct flowi *);
    void (*send_check)(struct sock *, struct sk_buff *);
    int (*rebuild_header)(struct sock *);
    void (*sk_rx_dst_set)(struct sock *, const struct sk_buff *);
    int (*conn_request)(struct sock *, struct sk_buff *);
    struct sock * (*syn_recv_sock)(const struct sock *, struct sk_buff *, struct request_sock *, struct dst_entry *, struct request_sock *, bool *);
    u16 net_header_len;
    u16 net_frag_header_len;
    u16 sockaddr_len;
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*addr2sockaddr)(struct sock *, struct sockaddr *);
    void (*mtu_reduced)(struct sock *);
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
struct inet_connection_sock_af_ops {
    int (*queue_xmit)(struct sock *, struct sk_buff *, struct flowi *);
    void (*send_check)(struct sock *, struct sk_buff *);
    int (*rebuild_header)(struct sock *);
    void (*sk_rx_dst_set)(struct sock *, const struct sk_buff *);
    int (*conn_request)(struct sock *, struct sk_buff *);
    struct sock * (*syn_recv_sock)(const struct sock *, struct sk_buff *, struct request_sock *, struct dst_entry *, struct request_sock *, bool *);
    u16 net_header_len;
    u16 net_frag_header_len;
    u16 sockaddr_len;
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*addr2sockaddr)(struct sock *, struct sockaddr *);
    void (*mtu_reduced)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct inet_connection_sock_af_ops {
    int (*queue_xmit)(struct sock *, struct sk_buff *, struct flowi *);
    void (*send_check)(struct sock *, struct sk_buff *);
    int (*rebuild_header)(struct sock *);
    void (*sk_rx_dst_set)(struct sock *, const struct sk_buff *);
    int (*conn_request)(struct sock *, struct sk_buff *);
    struct sock * (*syn_recv_sock)(const struct sock *, struct sk_buff *, struct request_sock *, struct dst_entry *, struct request_sock *, bool *);
    u16 net_header_len;
    u16 net_frag_header_len;
    u16 sockaddr_len;
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*addr2sockaddr)(struct sock *, struct sockaddr *);
    void (*mtu_reduced)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct inet_connection_sock_af_ops {
    int (*queue_xmit)(struct sock *, struct sk_buff *, struct flowi *);
    void (*send_check)(struct sock *, struct sk_buff *);
    int (*rebuild_header)(struct sock *);
    void (*sk_rx_dst_set)(struct sock *, const struct sk_buff *);
    int (*conn_request)(struct sock *, struct sk_buff *);
    struct sock * (*syn_recv_sock)(const struct sock *, struct sk_buff *, struct request_sock *, struct dst_entry *, struct request_sock *, bool *);
    u16 net_header_len;
    u16 net_frag_header_len;
    u16 sockaddr_len;
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*addr2sockaddr)(struct sock *, struct sockaddr *);
    void (*mtu_reduced)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct inet_connection_sock_af_ops {
    int (*queue_xmit)(struct sock *, struct sk_buff *, struct flowi *);
    void (*send_check)(struct sock *, struct sk_buff *);
    int (*rebuild_header)(struct sock *);
    void (*sk_rx_dst_set)(struct sock *, const struct sk_buff *);
    int (*conn_request)(struct sock *, struct sk_buff *);
    struct sock * (*syn_recv_sock)(const struct sock *, struct sk_buff *, struct request_sock *, struct dst_entry *, struct request_sock *, bool *);
    u16 net_header_len;
    u16 net_frag_header_len;
    u16 sockaddr_len;
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*addr2sockaddr)(struct sock *, struct sockaddr *);
    void (*mtu_reduced)(struct sock *);
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
<code>int (*bind_conflict)(const struct sock *, const struct inet_bind_bucket *, bool)</code> ➡️ <code>int (*bind_conflict)(const struct sock *, const struct inet_bind_bucket *, bool, bool)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*bind_conflict)(const struct sock *, const struct inet_bind_bucket *, bool, bool)</code>
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
<code>int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*compat_getsockopt)(struct sock *, int, int, char *, int *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*setsockopt)(struct sock *, int, int, char *, unsigned int)</code> ➡️ <code>int (*setsockopt)(struct sock *, int, int, sockptr_t, unsigned int)</code>
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
<b>Field removed. </b>
<code>u16 net_frag_header_len</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*compat_getsockopt)(struct sock *, int, int, char *, int *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*compat_getsockopt)(struct sock *, int, int, char *, int *)</code>
</li>
</ul>
</details>
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
