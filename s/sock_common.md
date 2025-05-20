# Struct: <code>sock_common</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct sock_common {
    __addrpair skc_addrpair;
    __be32 skc_daddr;
    __be32 skc_rcv_saddr;
    unsigned int skc_hash;
    __u16 skc_u16hashes[2];
    __portpair skc_portpair;
    __be16 skc_dport;
    __u16 skc_num;
    short unsigned int skc_family;
    volatile unsigned char skc_state;
    unsigned char skc_reuse;
    unsigned char skc_reuseport;
    unsigned char skc_ipv6only;
    unsigned char skc_net_refcnt;
    int skc_bound_dev_if;
    struct hlist_node skc_bind_node;
    struct hlist_nulls_node skc_portaddr_node;
    struct proto *skc_prot;
    possible_net_t skc_net;
    struct in6_addr skc_v6_daddr;
    struct in6_addr skc_v6_rcv_saddr;
    atomic64_t skc_cookie;
    long unsigned int skc_flags;
    struct sock *skc_listener;
    struct inet_timewait_death_row *skc_tw_dr;
    int skc_dontcopy_begin[0];
    struct hlist_node skc_node;
    struct hlist_nulls_node skc_nulls_node;
    int skc_tx_queue_mapping;
    int skc_incoming_cpu;
    u32 skc_rcv_wnd;
    u32 skc_tw_rcv_nxt;
    atomic_t skc_refcnt;
    int skc_dontcopy_end[0];
    u32 skc_rxhash;
    u32 skc_window_clamp;
    u32 skc_tw_snd_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct sock_common {
    __addrpair skc_addrpair;
    __be32 skc_daddr;
    __be32 skc_rcv_saddr;
    unsigned int skc_hash;
    __u16 skc_u16hashes[2];
    __portpair skc_portpair;
    __be16 skc_dport;
    __u16 skc_num;
    short unsigned int skc_family;
    volatile unsigned char skc_state;
    unsigned char skc_reuse;
    unsigned char skc_reuseport;
    unsigned char skc_ipv6only;
    unsigned char skc_net_refcnt;
    int skc_bound_dev_if;
    struct hlist_node skc_bind_node;
    struct hlist_node skc_portaddr_node;
    struct proto *skc_prot;
    possible_net_t skc_net;
    struct in6_addr skc_v6_daddr;
    struct in6_addr skc_v6_rcv_saddr;
    atomic64_t skc_cookie;
    long unsigned int skc_flags;
    struct sock *skc_listener;
    struct inet_timewait_death_row *skc_tw_dr;
    int skc_dontcopy_begin[0];
    struct hlist_node skc_node;
    struct hlist_nulls_node skc_nulls_node;
    int skc_tx_queue_mapping;
    int skc_incoming_cpu;
    u32 skc_rcv_wnd;
    u32 skc_tw_rcv_nxt;
    atomic_t skc_refcnt;
    int skc_dontcopy_end[0];
    u32 skc_rxhash;
    u32 skc_window_clamp;
    u32 skc_tw_snd_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct sock_common {
    __addrpair skc_addrpair;
    __be32 skc_daddr;
    __be32 skc_rcv_saddr;
    unsigned int skc_hash;
    __u16 skc_u16hashes[2];
    __portpair skc_portpair;
    __be16 skc_dport;
    __u16 skc_num;
    short unsigned int skc_family;
    volatile unsigned char skc_state;
    unsigned char skc_reuse;
    unsigned char skc_reuseport;
    unsigned char skc_ipv6only;
    unsigned char skc_net_refcnt;
    int skc_bound_dev_if;
    struct hlist_node skc_bind_node;
    struct hlist_node skc_portaddr_node;
    struct proto *skc_prot;
    possible_net_t skc_net;
    struct in6_addr skc_v6_daddr;
    struct in6_addr skc_v6_rcv_saddr;
    atomic64_t skc_cookie;
    long unsigned int skc_flags;
    struct sock *skc_listener;
    struct inet_timewait_death_row *skc_tw_dr;
    int skc_dontcopy_begin[0];
    struct hlist_node skc_node;
    struct hlist_nulls_node skc_nulls_node;
    int skc_tx_queue_mapping;
    int skc_incoming_cpu;
    u32 skc_rcv_wnd;
    u32 skc_tw_rcv_nxt;
    atomic_t skc_refcnt;
    int skc_dontcopy_end[0];
    u32 skc_rxhash;
    u32 skc_window_clamp;
    u32 skc_tw_snd_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct sock_common {
    __addrpair skc_addrpair;
    __be32 skc_daddr;
    __be32 skc_rcv_saddr;
    unsigned int skc_hash;
    __u16 skc_u16hashes[2];
    __portpair skc_portpair;
    __be16 skc_dport;
    __u16 skc_num;
    short unsigned int skc_family;
    volatile unsigned char skc_state;
    unsigned char skc_reuse;
    unsigned char skc_reuseport;
    unsigned char skc_ipv6only;
    unsigned char skc_net_refcnt;
    int skc_bound_dev_if;
    struct hlist_node skc_bind_node;
    struct hlist_node skc_portaddr_node;
    struct proto *skc_prot;
    possible_net_t skc_net;
    struct in6_addr skc_v6_daddr;
    struct in6_addr skc_v6_rcv_saddr;
    atomic64_t skc_cookie;
    long unsigned int skc_flags;
    struct sock *skc_listener;
    struct inet_timewait_death_row *skc_tw_dr;
    int skc_dontcopy_begin[0];
    struct hlist_node skc_node;
    struct hlist_nulls_node skc_nulls_node;
    int skc_tx_queue_mapping;
    int skc_incoming_cpu;
    u32 skc_rcv_wnd;
    u32 skc_tw_rcv_nxt;
    refcount_t skc_refcnt;
    int skc_dontcopy_end[0];
    u32 skc_rxhash;
    u32 skc_window_clamp;
    u32 skc_tw_snd_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct sock_common {
    __addrpair skc_addrpair;
    __be32 skc_daddr;
    __be32 skc_rcv_saddr;
    unsigned int skc_hash;
    __u16 skc_u16hashes[2];
    __portpair skc_portpair;
    __be16 skc_dport;
    __u16 skc_num;
    short unsigned int skc_family;
    volatile unsigned char skc_state;
    unsigned char skc_reuse;
    unsigned char skc_reuseport;
    unsigned char skc_ipv6only;
    unsigned char skc_net_refcnt;
    int skc_bound_dev_if;
    struct hlist_node skc_bind_node;
    struct hlist_node skc_portaddr_node;
    struct proto *skc_prot;
    possible_net_t skc_net;
    struct in6_addr skc_v6_daddr;
    struct in6_addr skc_v6_rcv_saddr;
    atomic64_t skc_cookie;
    long unsigned int skc_flags;
    struct sock *skc_listener;
    struct inet_timewait_death_row *skc_tw_dr;
    int skc_dontcopy_begin[0];
    struct hlist_node skc_node;
    struct hlist_nulls_node skc_nulls_node;
    int skc_tx_queue_mapping;
    int skc_incoming_cpu;
    u32 skc_rcv_wnd;
    u32 skc_tw_rcv_nxt;
    refcount_t skc_refcnt;
    int skc_dontcopy_end[0];
    u32 skc_rxhash;
    u32 skc_window_clamp;
    u32 skc_tw_snd_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct sock_common {
    __addrpair skc_addrpair;
    __be32 skc_daddr;
    __be32 skc_rcv_saddr;
    unsigned int skc_hash;
    __u16 skc_u16hashes[2];
    __portpair skc_portpair;
    __be16 skc_dport;
    __u16 skc_num;
    short unsigned int skc_family;
    volatile unsigned char skc_state;
    unsigned char skc_reuse;
    unsigned char skc_reuseport;
    unsigned char skc_ipv6only;
    unsigned char skc_net_refcnt;
    int skc_bound_dev_if;
    struct hlist_node skc_bind_node;
    struct hlist_node skc_portaddr_node;
    struct proto *skc_prot;
    possible_net_t skc_net;
    struct in6_addr skc_v6_daddr;
    struct in6_addr skc_v6_rcv_saddr;
    atomic64_t skc_cookie;
    long unsigned int skc_flags;
    struct sock *skc_listener;
    struct inet_timewait_death_row *skc_tw_dr;
    int skc_dontcopy_begin[0];
    struct hlist_node skc_node;
    struct hlist_nulls_node skc_nulls_node;
    int skc_tx_queue_mapping;
    int skc_incoming_cpu;
    u32 skc_rcv_wnd;
    u32 skc_tw_rcv_nxt;
    refcount_t skc_refcnt;
    int skc_dontcopy_end[0];
    u32 skc_rxhash;
    u32 skc_window_clamp;
    u32 skc_tw_snd_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct sock_common {
    __addrpair skc_addrpair;
    __be32 skc_daddr;
    __be32 skc_rcv_saddr;
    unsigned int skc_hash;
    __u16 skc_u16hashes[2];
    __portpair skc_portpair;
    __be16 skc_dport;
    __u16 skc_num;
    short unsigned int skc_family;
    volatile unsigned char skc_state;
    unsigned char skc_reuse;
    unsigned char skc_reuseport;
    unsigned char skc_ipv6only;
    unsigned char skc_net_refcnt;
    int skc_bound_dev_if;
    struct hlist_node skc_bind_node;
    struct hlist_node skc_portaddr_node;
    struct proto *skc_prot;
    possible_net_t skc_net;
    struct in6_addr skc_v6_daddr;
    struct in6_addr skc_v6_rcv_saddr;
    atomic64_t skc_cookie;
    long unsigned int skc_flags;
    struct sock *skc_listener;
    struct inet_timewait_death_row *skc_tw_dr;
    int skc_dontcopy_begin[0];
    struct hlist_node skc_node;
    struct hlist_nulls_node skc_nulls_node;
    short unsigned int skc_tx_queue_mapping;
    short unsigned int skc_rx_queue_mapping;
    int skc_incoming_cpu;
    u32 skc_rcv_wnd;
    u32 skc_tw_rcv_nxt;
    refcount_t skc_refcnt;
    int skc_dontcopy_end[0];
    u32 skc_rxhash;
    u32 skc_window_clamp;
    u32 skc_tw_snd_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct sock_common {
    __addrpair skc_addrpair;
    __be32 skc_daddr;
    __be32 skc_rcv_saddr;
    unsigned int skc_hash;
    __u16 skc_u16hashes[2];
    __portpair skc_portpair;
    __be16 skc_dport;
    __u16 skc_num;
    short unsigned int skc_family;
    volatile unsigned char skc_state;
    unsigned char skc_reuse;
    unsigned char skc_reuseport;
    unsigned char skc_ipv6only;
    unsigned char skc_net_refcnt;
    int skc_bound_dev_if;
    struct hlist_node skc_bind_node;
    struct hlist_node skc_portaddr_node;
    struct proto *skc_prot;
    possible_net_t skc_net;
    struct in6_addr skc_v6_daddr;
    struct in6_addr skc_v6_rcv_saddr;
    atomic64_t skc_cookie;
    long unsigned int skc_flags;
    struct sock *skc_listener;
    struct inet_timewait_death_row *skc_tw_dr;
    int skc_dontcopy_begin[0];
    struct hlist_node skc_node;
    struct hlist_nulls_node skc_nulls_node;
    short unsigned int skc_tx_queue_mapping;
    short unsigned int skc_rx_queue_mapping;
    int skc_incoming_cpu;
    u32 skc_rcv_wnd;
    u32 skc_tw_rcv_nxt;
    refcount_t skc_refcnt;
    int skc_dontcopy_end[0];
    u32 skc_rxhash;
    u32 skc_window_clamp;
    u32 skc_tw_snd_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct sock_common {
    __addrpair skc_addrpair;
    __be32 skc_daddr;
    __be32 skc_rcv_saddr;
    unsigned int skc_hash;
    __u16 skc_u16hashes[2];
    __portpair skc_portpair;
    __be16 skc_dport;
    __u16 skc_num;
    short unsigned int skc_family;
    volatile unsigned char skc_state;
    unsigned char skc_reuse;
    unsigned char skc_reuseport;
    unsigned char skc_ipv6only;
    unsigned char skc_net_refcnt;
    int skc_bound_dev_if;
    struct hlist_node skc_bind_node;
    struct hlist_node skc_portaddr_node;
    struct proto *skc_prot;
    possible_net_t skc_net;
    struct in6_addr skc_v6_daddr;
    struct in6_addr skc_v6_rcv_saddr;
    atomic64_t skc_cookie;
    long unsigned int skc_flags;
    struct sock *skc_listener;
    struct inet_timewait_death_row *skc_tw_dr;
    int skc_dontcopy_begin[0];
    struct hlist_node skc_node;
    struct hlist_nulls_node skc_nulls_node;
    short unsigned int skc_tx_queue_mapping;
    short unsigned int skc_rx_queue_mapping;
    int skc_incoming_cpu;
    u32 skc_rcv_wnd;
    u32 skc_tw_rcv_nxt;
    refcount_t skc_refcnt;
    int skc_dontcopy_end[0];
    u32 skc_rxhash;
    u32 skc_window_clamp;
    u32 skc_tw_snd_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct sock_common {
    __addrpair skc_addrpair;
    __be32 skc_daddr;
    __be32 skc_rcv_saddr;
    unsigned int skc_hash;
    __u16 skc_u16hashes[2];
    __portpair skc_portpair;
    __be16 skc_dport;
    __u16 skc_num;
    short unsigned int skc_family;
    volatile unsigned char skc_state;
    unsigned char skc_reuse;
    unsigned char skc_reuseport;
    unsigned char skc_ipv6only;
    unsigned char skc_net_refcnt;
    int skc_bound_dev_if;
    struct hlist_node skc_bind_node;
    struct hlist_node skc_portaddr_node;
    struct proto *skc_prot;
    possible_net_t skc_net;
    struct in6_addr skc_v6_daddr;
    struct in6_addr skc_v6_rcv_saddr;
    atomic64_t skc_cookie;
    long unsigned int skc_flags;
    struct sock *skc_listener;
    struct inet_timewait_death_row *skc_tw_dr;
    int skc_dontcopy_begin[0];
    struct hlist_node skc_node;
    struct hlist_nulls_node skc_nulls_node;
    short unsigned int skc_tx_queue_mapping;
    short unsigned int skc_rx_queue_mapping;
    int skc_incoming_cpu;
    u32 skc_rcv_wnd;
    u32 skc_tw_rcv_nxt;
    refcount_t skc_refcnt;
    int skc_dontcopy_end[0];
    u32 skc_rxhash;
    u32 skc_window_clamp;
    u32 skc_tw_snd_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct sock_common {
    __addrpair skc_addrpair;
    __be32 skc_daddr;
    __be32 skc_rcv_saddr;
    unsigned int skc_hash;
    __u16 skc_u16hashes[2];
    __portpair skc_portpair;
    __be16 skc_dport;
    __u16 skc_num;
    short unsigned int skc_family;
    volatile unsigned char skc_state;
    unsigned char skc_reuse;
    unsigned char skc_reuseport;
    unsigned char skc_ipv6only;
    unsigned char skc_net_refcnt;
    int skc_bound_dev_if;
    struct hlist_node skc_bind_node;
    struct hlist_node skc_portaddr_node;
    struct proto *skc_prot;
    possible_net_t skc_net;
    struct in6_addr skc_v6_daddr;
    struct in6_addr skc_v6_rcv_saddr;
    atomic64_t skc_cookie;
    long unsigned int skc_flags;
    struct sock *skc_listener;
    struct inet_timewait_death_row *skc_tw_dr;
    int skc_dontcopy_begin[0];
    struct hlist_node skc_node;
    struct hlist_nulls_node skc_nulls_node;
    short unsigned int skc_tx_queue_mapping;
    short unsigned int skc_rx_queue_mapping;
    int skc_incoming_cpu;
    u32 skc_rcv_wnd;
    u32 skc_tw_rcv_nxt;
    refcount_t skc_refcnt;
    int skc_dontcopy_end[0];
    u32 skc_rxhash;
    u32 skc_window_clamp;
    u32 skc_tw_snd_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct sock_common {
    __addrpair skc_addrpair;
    __be32 skc_daddr;
    __be32 skc_rcv_saddr;
    unsigned int skc_hash;
    __u16 skc_u16hashes[2];
    __portpair skc_portpair;
    __be16 skc_dport;
    __u16 skc_num;
    short unsigned int skc_family;
    volatile unsigned char skc_state;
    unsigned char skc_reuse;
    unsigned char skc_reuseport;
    unsigned char skc_ipv6only;
    unsigned char skc_net_refcnt;
    int skc_bound_dev_if;
    struct hlist_node skc_bind_node;
    struct hlist_node skc_portaddr_node;
    struct proto *skc_prot;
    possible_net_t skc_net;
    struct in6_addr skc_v6_daddr;
    struct in6_addr skc_v6_rcv_saddr;
    atomic64_t skc_cookie;
    long unsigned int skc_flags;
    struct sock *skc_listener;
    struct inet_timewait_death_row *skc_tw_dr;
    int skc_dontcopy_begin[0];
    struct hlist_node skc_node;
    struct hlist_nulls_node skc_nulls_node;
    short unsigned int skc_tx_queue_mapping;
    short unsigned int skc_rx_queue_mapping;
    int skc_incoming_cpu;
    u32 skc_rcv_wnd;
    u32 skc_tw_rcv_nxt;
    refcount_t skc_refcnt;
    int skc_dontcopy_end[0];
    u32 skc_rxhash;
    u32 skc_window_clamp;
    u32 skc_tw_snd_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct sock_common {
    __addrpair skc_addrpair;
    __be32 skc_daddr;
    __be32 skc_rcv_saddr;
    unsigned int skc_hash;
    __u16 skc_u16hashes[2];
    __portpair skc_portpair;
    __be16 skc_dport;
    __u16 skc_num;
    short unsigned int skc_family;
    volatile unsigned char skc_state;
    unsigned char skc_reuse;
    unsigned char skc_reuseport;
    unsigned char skc_ipv6only;
    unsigned char skc_net_refcnt;
    int skc_bound_dev_if;
    struct hlist_node skc_bind_node;
    struct hlist_node skc_portaddr_node;
    struct proto *skc_prot;
    possible_net_t skc_net;
    struct in6_addr skc_v6_daddr;
    struct in6_addr skc_v6_rcv_saddr;
    atomic64_t skc_cookie;
    long unsigned int skc_flags;
    struct sock *skc_listener;
    struct inet_timewait_death_row *skc_tw_dr;
    int skc_dontcopy_begin[0];
    struct hlist_node skc_node;
    struct hlist_nulls_node skc_nulls_node;
    short unsigned int skc_tx_queue_mapping;
    short unsigned int skc_rx_queue_mapping;
    int skc_incoming_cpu;
    u32 skc_rcv_wnd;
    u32 skc_tw_rcv_nxt;
    refcount_t skc_refcnt;
    int skc_dontcopy_end[0];
    u32 skc_rxhash;
    u32 skc_window_clamp;
    u32 skc_tw_snd_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct sock_common {
    __addrpair skc_addrpair;
    __be32 skc_daddr;
    __be32 skc_rcv_saddr;
    unsigned int skc_hash;
    __u16 skc_u16hashes[2];
    __portpair skc_portpair;
    __be16 skc_dport;
    __u16 skc_num;
    short unsigned int skc_family;
    volatile unsigned char skc_state;
    unsigned char skc_reuse;
    unsigned char skc_reuseport;
    unsigned char skc_ipv6only;
    unsigned char skc_net_refcnt;
    int skc_bound_dev_if;
    struct hlist_node skc_bind_node;
    struct hlist_node skc_portaddr_node;
    struct proto *skc_prot;
    possible_net_t skc_net;
    struct in6_addr skc_v6_daddr;
    struct in6_addr skc_v6_rcv_saddr;
    atomic64_t skc_cookie;
    long unsigned int skc_flags;
    struct sock *skc_listener;
    struct inet_timewait_death_row *skc_tw_dr;
    int skc_dontcopy_begin[0];
    struct hlist_node skc_node;
    struct hlist_nulls_node skc_nulls_node;
    short unsigned int skc_tx_queue_mapping;
    short unsigned int skc_rx_queue_mapping;
    int skc_incoming_cpu;
    u32 skc_rcv_wnd;
    u32 skc_tw_rcv_nxt;
    refcount_t skc_refcnt;
    int skc_dontcopy_end[0];
    u32 skc_rxhash;
    u32 skc_window_clamp;
    u32 skc_tw_snd_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct sock_common {
    __addrpair skc_addrpair;
    __be32 skc_daddr;
    __be32 skc_rcv_saddr;
    unsigned int skc_hash;
    __u16 skc_u16hashes[2];
    __portpair skc_portpair;
    __be16 skc_dport;
    __u16 skc_num;
    short unsigned int skc_family;
    volatile unsigned char skc_state;
    unsigned char skc_reuse;
    unsigned char skc_reuseport;
    unsigned char skc_ipv6only;
    unsigned char skc_net_refcnt;
    int skc_bound_dev_if;
    struct hlist_node skc_bind_node;
    struct hlist_node skc_portaddr_node;
    struct proto *skc_prot;
    possible_net_t skc_net;
    struct in6_addr skc_v6_daddr;
    struct in6_addr skc_v6_rcv_saddr;
    atomic64_t skc_cookie;
    long unsigned int skc_flags;
    struct sock *skc_listener;
    struct inet_timewait_death_row *skc_tw_dr;
    int skc_dontcopy_begin[0];
    struct hlist_node skc_node;
    struct hlist_nulls_node skc_nulls_node;
    short unsigned int skc_tx_queue_mapping;
    short unsigned int skc_rx_queue_mapping;
    int skc_incoming_cpu;
    u32 skc_rcv_wnd;
    u32 skc_tw_rcv_nxt;
    refcount_t skc_refcnt;
    int skc_dontcopy_end[0];
    u32 skc_rxhash;
    u32 skc_window_clamp;
    u32 skc_tw_snd_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct sock_common {
    __addrpair skc_addrpair;
    __be32 skc_daddr;
    __be32 skc_rcv_saddr;
    unsigned int skc_hash;
    __u16 skc_u16hashes[2];
    __portpair skc_portpair;
    __be16 skc_dport;
    __u16 skc_num;
    short unsigned int skc_family;
    volatile unsigned char skc_state;
    unsigned char skc_reuse;
    unsigned char skc_reuseport;
    unsigned char skc_ipv6only;
    unsigned char skc_net_refcnt;
    int skc_bound_dev_if;
    struct hlist_node skc_bind_node;
    struct hlist_node skc_portaddr_node;
    struct proto *skc_prot;
    possible_net_t skc_net;
    struct in6_addr skc_v6_daddr;
    struct in6_addr skc_v6_rcv_saddr;
    atomic64_t skc_cookie;
    long unsigned int skc_flags;
    struct sock *skc_listener;
    struct inet_timewait_death_row *skc_tw_dr;
    int skc_dontcopy_begin[0];
    struct hlist_node skc_node;
    struct hlist_nulls_node skc_nulls_node;
    short unsigned int skc_tx_queue_mapping;
    short unsigned int skc_rx_queue_mapping;
    int skc_incoming_cpu;
    u32 skc_rcv_wnd;
    u32 skc_tw_rcv_nxt;
    refcount_t skc_refcnt;
    int skc_dontcopy_end[0];
    u32 skc_rxhash;
    u32 skc_window_clamp;
    u32 skc_tw_snd_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct sock_common {
    __addrpair skc_addrpair;
    __be32 skc_daddr;
    __be32 skc_rcv_saddr;
    unsigned int skc_hash;
    __u16 skc_u16hashes[2];
    __portpair skc_portpair;
    __be16 skc_dport;
    __u16 skc_num;
    short unsigned int skc_family;
    volatile unsigned char skc_state;
    unsigned char skc_reuse;
    unsigned char skc_reuseport;
    unsigned char skc_ipv6only;
    unsigned char skc_net_refcnt;
    int skc_bound_dev_if;
    struct hlist_node skc_bind_node;
    struct hlist_node skc_portaddr_node;
    struct proto *skc_prot;
    possible_net_t skc_net;
    struct in6_addr skc_v6_daddr;
    struct in6_addr skc_v6_rcv_saddr;
    atomic64_t skc_cookie;
    long unsigned int skc_flags;
    struct sock *skc_listener;
    struct inet_timewait_death_row *skc_tw_dr;
    int skc_dontcopy_begin[0];
    struct hlist_node skc_node;
    struct hlist_nulls_node skc_nulls_node;
    short unsigned int skc_tx_queue_mapping;
    short unsigned int skc_rx_queue_mapping;
    int skc_incoming_cpu;
    u32 skc_rcv_wnd;
    u32 skc_tw_rcv_nxt;
    refcount_t skc_refcnt;
    int skc_dontcopy_end[0];
    u32 skc_rxhash;
    u32 skc_window_clamp;
    u32 skc_tw_snd_nxt;
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
struct sock_common {
    __addrpair skc_addrpair;
    __be32 skc_daddr;
    __be32 skc_rcv_saddr;
    unsigned int skc_hash;
    __u16 skc_u16hashes[2];
    __portpair skc_portpair;
    __be16 skc_dport;
    __u16 skc_num;
    short unsigned int skc_family;
    volatile unsigned char skc_state;
    unsigned char skc_reuse;
    unsigned char skc_reuseport;
    unsigned char skc_ipv6only;
    unsigned char skc_net_refcnt;
    int skc_bound_dev_if;
    struct hlist_node skc_bind_node;
    struct hlist_node skc_portaddr_node;
    struct proto *skc_prot;
    possible_net_t skc_net;
    struct in6_addr skc_v6_daddr;
    struct in6_addr skc_v6_rcv_saddr;
    atomic64_t skc_cookie;
    long unsigned int skc_flags;
    struct sock *skc_listener;
    struct inet_timewait_death_row *skc_tw_dr;
    int skc_dontcopy_begin[0];
    struct hlist_node skc_node;
    struct hlist_nulls_node skc_nulls_node;
    short unsigned int skc_tx_queue_mapping;
    short unsigned int skc_rx_queue_mapping;
    int skc_incoming_cpu;
    u32 skc_rcv_wnd;
    u32 skc_tw_rcv_nxt;
    refcount_t skc_refcnt;
    int skc_dontcopy_end[0];
    u32 skc_rxhash;
    u32 skc_window_clamp;
    u32 skc_tw_snd_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct sock_common {
    __addrpair skc_addrpair;
    __be32 skc_daddr;
    __be32 skc_rcv_saddr;
    unsigned int skc_hash;
    __u16 skc_u16hashes[2];
    __portpair skc_portpair;
    __be16 skc_dport;
    __u16 skc_num;
    short unsigned int skc_family;
    volatile unsigned char skc_state;
    unsigned char skc_reuse;
    unsigned char skc_reuseport;
    unsigned char skc_ipv6only;
    unsigned char skc_net_refcnt;
    int skc_bound_dev_if;
    struct hlist_node skc_bind_node;
    struct hlist_node skc_portaddr_node;
    struct proto *skc_prot;
    possible_net_t skc_net;
    struct in6_addr skc_v6_daddr;
    struct in6_addr skc_v6_rcv_saddr;
    atomic64_t skc_cookie;
    long unsigned int skc_flags;
    struct sock *skc_listener;
    struct inet_timewait_death_row *skc_tw_dr;
    int skc_dontcopy_begin[0];
    struct hlist_node skc_node;
    struct hlist_nulls_node skc_nulls_node;
    short unsigned int skc_tx_queue_mapping;
    short unsigned int skc_rx_queue_mapping;
    int skc_incoming_cpu;
    u32 skc_rcv_wnd;
    u32 skc_tw_rcv_nxt;
    refcount_t skc_refcnt;
    int skc_dontcopy_end[0];
    u32 skc_rxhash;
    u32 skc_window_clamp;
    u32 skc_tw_snd_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct sock_common {
    __addrpair skc_addrpair;
    __be32 skc_daddr;
    __be32 skc_rcv_saddr;
    unsigned int skc_hash;
    __u16 skc_u16hashes[2];
    __portpair skc_portpair;
    __be16 skc_dport;
    __u16 skc_num;
    short unsigned int skc_family;
    volatile unsigned char skc_state;
    unsigned char skc_reuse;
    unsigned char skc_reuseport;
    unsigned char skc_ipv6only;
    unsigned char skc_net_refcnt;
    int skc_bound_dev_if;
    struct hlist_node skc_bind_node;
    struct hlist_node skc_portaddr_node;
    struct proto *skc_prot;
    possible_net_t skc_net;
    struct in6_addr skc_v6_daddr;
    struct in6_addr skc_v6_rcv_saddr;
    atomic64_t skc_cookie;
    long unsigned int skc_flags;
    struct sock *skc_listener;
    struct inet_timewait_death_row *skc_tw_dr;
    int skc_dontcopy_begin[0];
    struct hlist_node skc_node;
    struct hlist_nulls_node skc_nulls_node;
    short unsigned int skc_tx_queue_mapping;
    short unsigned int skc_rx_queue_mapping;
    int skc_incoming_cpu;
    u32 skc_rcv_wnd;
    u32 skc_tw_rcv_nxt;
    refcount_t skc_refcnt;
    int skc_dontcopy_end[0];
    u32 skc_rxhash;
    u32 skc_window_clamp;
    u32 skc_tw_snd_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct sock_common {
    __addrpair skc_addrpair;
    __be32 skc_daddr;
    __be32 skc_rcv_saddr;
    unsigned int skc_hash;
    __u16 skc_u16hashes[2];
    __portpair skc_portpair;
    __be16 skc_dport;
    __u16 skc_num;
    short unsigned int skc_family;
    volatile unsigned char skc_state;
    unsigned char skc_reuse;
    unsigned char skc_reuseport;
    unsigned char skc_ipv6only;
    unsigned char skc_net_refcnt;
    int skc_bound_dev_if;
    struct hlist_node skc_bind_node;
    struct hlist_node skc_portaddr_node;
    struct proto *skc_prot;
    possible_net_t skc_net;
    struct in6_addr skc_v6_daddr;
    struct in6_addr skc_v6_rcv_saddr;
    atomic64_t skc_cookie;
    long unsigned int skc_flags;
    struct sock *skc_listener;
    struct inet_timewait_death_row *skc_tw_dr;
    int skc_dontcopy_begin[0];
    struct hlist_node skc_node;
    struct hlist_nulls_node skc_nulls_node;
    short unsigned int skc_tx_queue_mapping;
    short unsigned int skc_rx_queue_mapping;
    int skc_incoming_cpu;
    u32 skc_rcv_wnd;
    u32 skc_tw_rcv_nxt;
    refcount_t skc_refcnt;
    int skc_dontcopy_end[0];
    u32 skc_rxhash;
    u32 skc_window_clamp;
    u32 skc_tw_snd_nxt;
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
struct sock_common {
    __addrpair skc_addrpair;
    __be32 skc_daddr;
    __be32 skc_rcv_saddr;
    unsigned int skc_hash;
    __u16 skc_u16hashes[2];
    __portpair skc_portpair;
    __be16 skc_dport;
    __u16 skc_num;
    short unsigned int skc_family;
    volatile unsigned char skc_state;
    unsigned char skc_reuse;
    unsigned char skc_reuseport;
    unsigned char skc_ipv6only;
    unsigned char skc_net_refcnt;
    int skc_bound_dev_if;
    struct hlist_node skc_bind_node;
    struct hlist_node skc_portaddr_node;
    struct proto *skc_prot;
    possible_net_t skc_net;
    struct in6_addr skc_v6_daddr;
    struct in6_addr skc_v6_rcv_saddr;
    atomic64_t skc_cookie;
    long unsigned int skc_flags;
    struct sock *skc_listener;
    struct inet_timewait_death_row *skc_tw_dr;
    int skc_dontcopy_begin[0];
    struct hlist_node skc_node;
    struct hlist_nulls_node skc_nulls_node;
    short unsigned int skc_tx_queue_mapping;
    short unsigned int skc_rx_queue_mapping;
    int skc_incoming_cpu;
    u32 skc_rcv_wnd;
    u32 skc_tw_rcv_nxt;
    refcount_t skc_refcnt;
    int skc_dontcopy_end[0];
    u32 skc_rxhash;
    u32 skc_window_clamp;
    u32 skc_tw_snd_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct sock_common {
    __addrpair skc_addrpair;
    __be32 skc_daddr;
    __be32 skc_rcv_saddr;
    unsigned int skc_hash;
    __u16 skc_u16hashes[2];
    __portpair skc_portpair;
    __be16 skc_dport;
    __u16 skc_num;
    short unsigned int skc_family;
    volatile unsigned char skc_state;
    unsigned char skc_reuse;
    unsigned char skc_reuseport;
    unsigned char skc_ipv6only;
    unsigned char skc_net_refcnt;
    int skc_bound_dev_if;
    struct hlist_node skc_bind_node;
    struct hlist_node skc_portaddr_node;
    struct proto *skc_prot;
    possible_net_t skc_net;
    struct in6_addr skc_v6_daddr;
    struct in6_addr skc_v6_rcv_saddr;
    atomic64_t skc_cookie;
    long unsigned int skc_flags;
    struct sock *skc_listener;
    struct inet_timewait_death_row *skc_tw_dr;
    int skc_dontcopy_begin[0];
    struct hlist_node skc_node;
    struct hlist_nulls_node skc_nulls_node;
    short unsigned int skc_tx_queue_mapping;
    short unsigned int skc_rx_queue_mapping;
    int skc_incoming_cpu;
    u32 skc_rcv_wnd;
    u32 skc_tw_rcv_nxt;
    refcount_t skc_refcnt;
    int skc_dontcopy_end[0];
    u32 skc_rxhash;
    u32 skc_window_clamp;
    u32 skc_tw_snd_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct sock_common {
    __addrpair skc_addrpair;
    __be32 skc_daddr;
    __be32 skc_rcv_saddr;
    unsigned int skc_hash;
    __u16 skc_u16hashes[2];
    __portpair skc_portpair;
    __be16 skc_dport;
    __u16 skc_num;
    short unsigned int skc_family;
    volatile unsigned char skc_state;
    unsigned char skc_reuse;
    unsigned char skc_reuseport;
    unsigned char skc_ipv6only;
    unsigned char skc_net_refcnt;
    int skc_bound_dev_if;
    struct hlist_node skc_bind_node;
    struct hlist_node skc_portaddr_node;
    struct proto *skc_prot;
    possible_net_t skc_net;
    struct in6_addr skc_v6_daddr;
    struct in6_addr skc_v6_rcv_saddr;
    atomic64_t skc_cookie;
    long unsigned int skc_flags;
    struct sock *skc_listener;
    struct inet_timewait_death_row *skc_tw_dr;
    int skc_dontcopy_begin[0];
    struct hlist_node skc_node;
    struct hlist_nulls_node skc_nulls_node;
    short unsigned int skc_tx_queue_mapping;
    short unsigned int skc_rx_queue_mapping;
    int skc_incoming_cpu;
    u32 skc_rcv_wnd;
    u32 skc_tw_rcv_nxt;
    refcount_t skc_refcnt;
    int skc_dontcopy_end[0];
    u32 skc_rxhash;
    u32 skc_window_clamp;
    u32 skc_tw_snd_nxt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct sock_common {
    __addrpair skc_addrpair;
    __be32 skc_daddr;
    __be32 skc_rcv_saddr;
    unsigned int skc_hash;
    __u16 skc_u16hashes[2];
    __portpair skc_portpair;
    __be16 skc_dport;
    __u16 skc_num;
    short unsigned int skc_family;
    volatile unsigned char skc_state;
    unsigned char skc_reuse;
    unsigned char skc_reuseport;
    unsigned char skc_ipv6only;
    unsigned char skc_net_refcnt;
    int skc_bound_dev_if;
    struct hlist_node skc_bind_node;
    struct hlist_node skc_portaddr_node;
    struct proto *skc_prot;
    possible_net_t skc_net;
    struct in6_addr skc_v6_daddr;
    struct in6_addr skc_v6_rcv_saddr;
    atomic64_t skc_cookie;
    long unsigned int skc_flags;
    struct sock *skc_listener;
    struct inet_timewait_death_row *skc_tw_dr;
    int skc_dontcopy_begin[0];
    struct hlist_node skc_node;
    struct hlist_nulls_node skc_nulls_node;
    short unsigned int skc_tx_queue_mapping;
    short unsigned int skc_rx_queue_mapping;
    int skc_incoming_cpu;
    u32 skc_rcv_wnd;
    u32 skc_tw_rcv_nxt;
    refcount_t skc_refcnt;
    int skc_dontcopy_end[0];
    u32 skc_rxhash;
    u32 skc_window_clamp;
    u32 skc_tw_snd_nxt;
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
<code>struct hlist_nulls_node skc_portaddr_node</code> ➡️ <code>struct hlist_node skc_portaddr_node</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>atomic_t skc_refcnt</code> ➡️ <code>refcount_t skc_refcnt</code>
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
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>short unsigned int skc_rx_queue_mapping</code>
</li>
<li>
<b>Field type changed. </b>
<code>int skc_tx_queue_mapping</code> ➡️ <code>short unsigned int skc_tx_queue_mapping</code>
</li>
</ul>
</details>
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
No changes between <code>5.8</code> and <code>5.11</code> ✅
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
