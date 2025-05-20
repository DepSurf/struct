# Struct: <code>sock</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct sock {
    struct sock_common __sk_common;
    socket_lock_t sk_lock;
    struct sk_buff_head sk_receive_queue;
    struct (anon) sk_backlog;
    int sk_forward_alloc;
    __u32 sk_txhash;
    unsigned int sk_napi_id;
    unsigned int sk_ll_usec;
    atomic_t sk_drops;
    int sk_rcvbuf;
    struct sk_filter *sk_filter;
    struct socket_wq *sk_wq;
    struct socket_wq *sk_wq_raw;
    struct xfrm_policy * sk_policy[2];
    struct dst_entry *sk_rx_dst;
    struct dst_entry *sk_dst_cache;
    atomic_t sk_wmem_alloc;
    atomic_t sk_omem_alloc;
    int sk_sndbuf;
    struct sk_buff_head sk_write_queue;
    unsigned int sk_shutdown;
    unsigned int sk_no_check_tx;
    unsigned int sk_no_check_rx;
    unsigned int sk_userlocks;
    unsigned int sk_protocol;
    unsigned int sk_type;
    int sk_wmem_queued;
    gfp_t sk_allocation;
    u32 sk_pacing_rate;
    u32 sk_max_pacing_rate;
    netdev_features_t sk_route_caps;
    netdev_features_t sk_route_nocaps;
    int sk_gso_type;
    unsigned int sk_gso_max_size;
    u16 sk_gso_max_segs;
    int sk_rcvlowat;
    long unsigned int sk_lingertime;
    struct sk_buff_head sk_error_queue;
    struct proto *sk_prot_creator;
    rwlock_t sk_callback_lock;
    int sk_err;
    int sk_err_soft;
    u32 sk_ack_backlog;
    u32 sk_max_ack_backlog;
    __u32 sk_priority;
    __u32 sk_cgrp_prioidx;
    struct pid *sk_peer_pid;
    const struct cred *sk_peer_cred;
    long int sk_rcvtimeo;
    long int sk_sndtimeo;
    struct timer_list sk_timer;
    ktime_t sk_stamp;
    u16 sk_tsflags;
    u32 sk_tskey;
    struct socket *sk_socket;
    void *sk_user_data;
    struct page_frag sk_frag;
    struct sk_buff *sk_send_head;
    __s32 sk_peek_off;
    int sk_write_pending;
    void *sk_security;
    __u32 sk_mark;
    u32 sk_classid;
    struct cg_proto *sk_cgrp;
    void (*sk_state_change)(struct sock *);
    void (*sk_data_ready)(struct sock *);
    void (*sk_write_space)(struct sock *);
    void (*sk_error_report)(struct sock *);
    int (*sk_backlog_rcv)(struct sock *, struct sk_buff *);
    void (*sk_destruct)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct sock {
    struct sock_common __sk_common;
    socket_lock_t sk_lock;
    struct sk_buff_head sk_receive_queue;
    struct (anon) sk_backlog;
    int sk_forward_alloc;
    __u32 sk_txhash;
    unsigned int sk_napi_id;
    unsigned int sk_ll_usec;
    atomic_t sk_drops;
    int sk_rcvbuf;
    struct sk_filter *sk_filter;
    struct socket_wq *sk_wq;
    struct socket_wq *sk_wq_raw;
    struct xfrm_policy * sk_policy[2];
    struct dst_entry *sk_rx_dst;
    struct dst_entry *sk_dst_cache;
    atomic_t sk_wmem_alloc;
    atomic_t sk_omem_alloc;
    int sk_sndbuf;
    struct sk_buff_head sk_write_queue;
    unsigned int sk_padding;
    unsigned int sk_no_check_tx;
    unsigned int sk_no_check_rx;
    unsigned int sk_userlocks;
    unsigned int sk_protocol;
    unsigned int sk_type;
    int sk_wmem_queued;
    gfp_t sk_allocation;
    u32 sk_pacing_rate;
    u32 sk_max_pacing_rate;
    netdev_features_t sk_route_caps;
    netdev_features_t sk_route_nocaps;
    int sk_gso_type;
    unsigned int sk_gso_max_size;
    u16 sk_gso_max_segs;
    int sk_rcvlowat;
    long unsigned int sk_lingertime;
    struct sk_buff_head sk_error_queue;
    struct proto *sk_prot_creator;
    rwlock_t sk_callback_lock;
    int sk_err;
    int sk_err_soft;
    u32 sk_ack_backlog;
    u32 sk_max_ack_backlog;
    __u32 sk_priority;
    __u32 sk_mark;
    struct pid *sk_peer_pid;
    const struct cred *sk_peer_cred;
    long int sk_rcvtimeo;
    long int sk_sndtimeo;
    struct timer_list sk_timer;
    ktime_t sk_stamp;
    u16 sk_tsflags;
    u8 sk_shutdown;
    u32 sk_tskey;
    struct socket *sk_socket;
    void *sk_user_data;
    struct page_frag sk_frag;
    struct sk_buff *sk_send_head;
    __s32 sk_peek_off;
    int sk_write_pending;
    void *sk_security;
    struct sock_cgroup_data sk_cgrp_data;
    struct mem_cgroup *sk_memcg;
    void (*sk_state_change)(struct sock *);
    void (*sk_data_ready)(struct sock *);
    void (*sk_write_space)(struct sock *);
    void (*sk_error_report)(struct sock *);
    int (*sk_backlog_rcv)(struct sock *, struct sk_buff *);
    void (*sk_destruct)(struct sock *);
    struct sock_reuseport *sk_reuseport_cb;
    struct callback_head sk_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct sock {
    struct sock_common __sk_common;
    socket_lock_t sk_lock;
    atomic_t sk_drops;
    int sk_rcvlowat;
    struct sk_buff_head sk_error_queue;
    struct sk_buff_head sk_receive_queue;
    struct (anon) sk_backlog;
    int sk_forward_alloc;
    unsigned int sk_ll_usec;
    unsigned int sk_napi_id;
    int sk_rcvbuf;
    struct sk_filter *sk_filter;
    struct socket_wq *sk_wq;
    struct socket_wq *sk_wq_raw;
    struct xfrm_policy * sk_policy[2];
    struct dst_entry *sk_rx_dst;
    struct dst_entry *sk_dst_cache;
    atomic_t sk_omem_alloc;
    int sk_sndbuf;
    int sk_wmem_queued;
    atomic_t sk_wmem_alloc;
    long unsigned int sk_tsq_flags;
    struct sk_buff *sk_send_head;
    struct sk_buff_head sk_write_queue;
    __s32 sk_peek_off;
    int sk_write_pending;
    long int sk_sndtimeo;
    struct timer_list sk_timer;
    __u32 sk_priority;
    __u32 sk_mark;
    u32 sk_pacing_rate;
    u32 sk_max_pacing_rate;
    struct page_frag sk_frag;
    netdev_features_t sk_route_caps;
    netdev_features_t sk_route_nocaps;
    int sk_gso_type;
    unsigned int sk_gso_max_size;
    gfp_t sk_allocation;
    __u32 sk_txhash;
    unsigned int __sk_flags_offset[0];
    unsigned int sk_padding;
    unsigned int sk_no_check_tx;
    unsigned int sk_no_check_rx;
    unsigned int sk_userlocks;
    unsigned int sk_protocol;
    unsigned int sk_type;
    u16 sk_gso_max_segs;
    long unsigned int sk_lingertime;
    struct proto *sk_prot_creator;
    rwlock_t sk_callback_lock;
    int sk_err;
    int sk_err_soft;
    u32 sk_ack_backlog;
    u32 sk_max_ack_backlog;
    kuid_t sk_uid;
    struct pid *sk_peer_pid;
    const struct cred *sk_peer_cred;
    long int sk_rcvtimeo;
    ktime_t sk_stamp;
    u16 sk_tsflags;
    u8 sk_shutdown;
    u32 sk_tskey;
    struct socket *sk_socket;
    void *sk_user_data;
    void *sk_security;
    struct sock_cgroup_data sk_cgrp_data;
    struct mem_cgroup *sk_memcg;
    void (*sk_state_change)(struct sock *);
    void (*sk_data_ready)(struct sock *);
    void (*sk_write_space)(struct sock *);
    void (*sk_error_report)(struct sock *);
    int (*sk_backlog_rcv)(struct sock *, struct sk_buff *);
    void (*sk_destruct)(struct sock *);
    struct sock_reuseport *sk_reuseport_cb;
    struct callback_head sk_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct sock {
    struct sock_common __sk_common;
    socket_lock_t sk_lock;
    atomic_t sk_drops;
    int sk_rcvlowat;
    struct sk_buff_head sk_error_queue;
    struct sk_buff_head sk_receive_queue;
    struct (anon) sk_backlog;
    int sk_forward_alloc;
    unsigned int sk_ll_usec;
    unsigned int sk_napi_id;
    int sk_rcvbuf;
    struct sk_filter *sk_filter;
    struct socket_wq *sk_wq;
    struct socket_wq *sk_wq_raw;
    struct xfrm_policy * sk_policy[2];
    struct dst_entry *sk_rx_dst;
    struct dst_entry *sk_dst_cache;
    atomic_t sk_omem_alloc;
    int sk_sndbuf;
    int sk_wmem_queued;
    refcount_t sk_wmem_alloc;
    long unsigned int sk_tsq_flags;
    struct sk_buff *sk_send_head;
    struct sk_buff_head sk_write_queue;
    __s32 sk_peek_off;
    int sk_write_pending;
    __u32 sk_dst_pending_confirm;
    u32 sk_pacing_status;
    long int sk_sndtimeo;
    struct timer_list sk_timer;
    __u32 sk_priority;
    __u32 sk_mark;
    u32 sk_pacing_rate;
    u32 sk_max_pacing_rate;
    struct page_frag sk_frag;
    netdev_features_t sk_route_caps;
    netdev_features_t sk_route_nocaps;
    int sk_gso_type;
    unsigned int sk_gso_max_size;
    gfp_t sk_allocation;
    __u32 sk_txhash;
    unsigned int __sk_flags_offset[0];
    unsigned int sk_padding;
    unsigned int sk_kern_sock;
    unsigned int sk_no_check_tx;
    unsigned int sk_no_check_rx;
    unsigned int sk_userlocks;
    unsigned int sk_protocol;
    unsigned int sk_type;
    u16 sk_gso_max_segs;
    long unsigned int sk_lingertime;
    struct proto *sk_prot_creator;
    rwlock_t sk_callback_lock;
    int sk_err;
    int sk_err_soft;
    u32 sk_ack_backlog;
    u32 sk_max_ack_backlog;
    kuid_t sk_uid;
    struct pid *sk_peer_pid;
    const struct cred *sk_peer_cred;
    long int sk_rcvtimeo;
    ktime_t sk_stamp;
    u16 sk_tsflags;
    u8 sk_shutdown;
    u32 sk_tskey;
    struct socket *sk_socket;
    void *sk_user_data;
    void *sk_security;
    struct sock_cgroup_data sk_cgrp_data;
    struct mem_cgroup *sk_memcg;
    void (*sk_state_change)(struct sock *);
    void (*sk_data_ready)(struct sock *);
    void (*sk_write_space)(struct sock *);
    void (*sk_error_report)(struct sock *);
    int (*sk_backlog_rcv)(struct sock *, struct sk_buff *);
    void (*sk_destruct)(struct sock *);
    struct sock_reuseport *sk_reuseport_cb;
    struct callback_head sk_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct sock {
    struct sock_common __sk_common;
    socket_lock_t sk_lock;
    atomic_t sk_drops;
    int sk_rcvlowat;
    struct sk_buff_head sk_error_queue;
    struct sk_buff_head sk_receive_queue;
    struct (anon) sk_backlog;
    int sk_forward_alloc;
    unsigned int sk_ll_usec;
    unsigned int sk_napi_id;
    int sk_rcvbuf;
    struct sk_filter *sk_filter;
    struct socket_wq *sk_wq;
    struct socket_wq *sk_wq_raw;
    struct xfrm_policy * sk_policy[2];
    struct dst_entry *sk_rx_dst;
    struct dst_entry *sk_dst_cache;
    atomic_t sk_omem_alloc;
    int sk_sndbuf;
    int sk_wmem_queued;
    refcount_t sk_wmem_alloc;
    long unsigned int sk_tsq_flags;
    struct sk_buff *sk_send_head;
    struct rb_root tcp_rtx_queue;
    struct sk_buff_head sk_write_queue;
    __s32 sk_peek_off;
    int sk_write_pending;
    __u32 sk_dst_pending_confirm;
    u32 sk_pacing_status;
    long int sk_sndtimeo;
    struct timer_list sk_timer;
    __u32 sk_priority;
    __u32 sk_mark;
    u32 sk_pacing_rate;
    u32 sk_max_pacing_rate;
    struct page_frag sk_frag;
    netdev_features_t sk_route_caps;
    netdev_features_t sk_route_nocaps;
    int sk_gso_type;
    unsigned int sk_gso_max_size;
    gfp_t sk_allocation;
    __u32 sk_txhash;
    unsigned int __sk_flags_offset[0];
    unsigned int sk_padding;
    unsigned int sk_kern_sock;
    unsigned int sk_no_check_tx;
    unsigned int sk_no_check_rx;
    unsigned int sk_userlocks;
    unsigned int sk_protocol;
    unsigned int sk_type;
    u16 sk_gso_max_segs;
    u8 sk_pacing_shift;
    long unsigned int sk_lingertime;
    struct proto *sk_prot_creator;
    rwlock_t sk_callback_lock;
    int sk_err;
    int sk_err_soft;
    u32 sk_ack_backlog;
    u32 sk_max_ack_backlog;
    kuid_t sk_uid;
    struct pid *sk_peer_pid;
    const struct cred *sk_peer_cred;
    long int sk_rcvtimeo;
    ktime_t sk_stamp;
    u16 sk_tsflags;
    u8 sk_shutdown;
    u32 sk_tskey;
    atomic_t sk_zckey;
    struct socket *sk_socket;
    void *sk_user_data;
    void *sk_security;
    struct sock_cgroup_data sk_cgrp_data;
    struct mem_cgroup *sk_memcg;
    void (*sk_state_change)(struct sock *);
    void (*sk_data_ready)(struct sock *);
    void (*sk_write_space)(struct sock *);
    void (*sk_error_report)(struct sock *);
    int (*sk_backlog_rcv)(struct sock *, struct sk_buff *);
    void (*sk_destruct)(struct sock *);
    struct sock_reuseport *sk_reuseport_cb;
    struct callback_head sk_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct sock {
    struct sock_common __sk_common;
    socket_lock_t sk_lock;
    atomic_t sk_drops;
    int sk_rcvlowat;
    struct sk_buff_head sk_error_queue;
    struct sk_buff_head sk_receive_queue;
    struct (anon) sk_backlog;
    int sk_forward_alloc;
    unsigned int sk_ll_usec;
    unsigned int sk_napi_id;
    int sk_rcvbuf;
    struct sk_filter *sk_filter;
    struct socket_wq *sk_wq;
    struct socket_wq *sk_wq_raw;
    struct xfrm_policy * sk_policy[2];
    struct dst_entry *sk_rx_dst;
    struct dst_entry *sk_dst_cache;
    atomic_t sk_omem_alloc;
    int sk_sndbuf;
    int sk_wmem_queued;
    refcount_t sk_wmem_alloc;
    long unsigned int sk_tsq_flags;
    struct sk_buff *sk_send_head;
    struct rb_root tcp_rtx_queue;
    struct sk_buff_head sk_write_queue;
    __s32 sk_peek_off;
    int sk_write_pending;
    __u32 sk_dst_pending_confirm;
    u32 sk_pacing_status;
    long int sk_sndtimeo;
    struct timer_list sk_timer;
    __u32 sk_priority;
    __u32 sk_mark;
    u32 sk_pacing_rate;
    u32 sk_max_pacing_rate;
    struct page_frag sk_frag;
    netdev_features_t sk_route_caps;
    netdev_features_t sk_route_nocaps;
    netdev_features_t sk_route_forced_caps;
    int sk_gso_type;
    unsigned int sk_gso_max_size;
    gfp_t sk_allocation;
    __u32 sk_txhash;
    unsigned int __sk_flags_offset[0];
    unsigned int sk_padding;
    unsigned int sk_kern_sock;
    unsigned int sk_no_check_tx;
    unsigned int sk_no_check_rx;
    unsigned int sk_userlocks;
    unsigned int sk_protocol;
    unsigned int sk_type;
    u16 sk_gso_max_segs;
    u8 sk_pacing_shift;
    long unsigned int sk_lingertime;
    struct proto *sk_prot_creator;
    rwlock_t sk_callback_lock;
    int sk_err;
    int sk_err_soft;
    u32 sk_ack_backlog;
    u32 sk_max_ack_backlog;
    kuid_t sk_uid;
    struct pid *sk_peer_pid;
    const struct cred *sk_peer_cred;
    long int sk_rcvtimeo;
    ktime_t sk_stamp;
    u16 sk_tsflags;
    u8 sk_shutdown;
    u32 sk_tskey;
    atomic_t sk_zckey;
    struct socket *sk_socket;
    void *sk_user_data;
    void *sk_security;
    struct sock_cgroup_data sk_cgrp_data;
    struct mem_cgroup *sk_memcg;
    void (*sk_state_change)(struct sock *);
    void (*sk_data_ready)(struct sock *);
    void (*sk_write_space)(struct sock *);
    void (*sk_error_report)(struct sock *);
    int (*sk_backlog_rcv)(struct sock *, struct sk_buff *);
    struct sk_buff * (*sk_validate_xmit_skb)(struct sock *, struct net_device *, struct sk_buff *);
    void (*sk_destruct)(struct sock *);
    struct sock_reuseport *sk_reuseport_cb;
    struct callback_head sk_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct sock {
    struct sock_common __sk_common;
    socket_lock_t sk_lock;
    atomic_t sk_drops;
    int sk_rcvlowat;
    struct sk_buff_head sk_error_queue;
    struct sk_buff_head sk_receive_queue;
    struct (anon) sk_backlog;
    int sk_forward_alloc;
    unsigned int sk_ll_usec;
    unsigned int sk_napi_id;
    int sk_rcvbuf;
    struct sk_filter *sk_filter;
    struct socket_wq *sk_wq;
    struct socket_wq *sk_wq_raw;
    struct xfrm_policy * sk_policy[2];
    struct dst_entry *sk_rx_dst;
    struct dst_entry *sk_dst_cache;
    atomic_t sk_omem_alloc;
    int sk_sndbuf;
    int sk_wmem_queued;
    refcount_t sk_wmem_alloc;
    long unsigned int sk_tsq_flags;
    struct sk_buff *sk_send_head;
    struct rb_root tcp_rtx_queue;
    struct sk_buff_head sk_write_queue;
    __s32 sk_peek_off;
    int sk_write_pending;
    __u32 sk_dst_pending_confirm;
    u32 sk_pacing_status;
    long int sk_sndtimeo;
    struct timer_list sk_timer;
    __u32 sk_priority;
    __u32 sk_mark;
    long unsigned int sk_pacing_rate;
    long unsigned int sk_max_pacing_rate;
    struct page_frag sk_frag;
    netdev_features_t sk_route_caps;
    netdev_features_t sk_route_nocaps;
    netdev_features_t sk_route_forced_caps;
    int sk_gso_type;
    unsigned int sk_gso_max_size;
    gfp_t sk_allocation;
    __u32 sk_txhash;
    unsigned int __sk_flags_offset[0];
    unsigned int sk_padding;
    unsigned int sk_kern_sock;
    unsigned int sk_no_check_tx;
    unsigned int sk_no_check_rx;
    unsigned int sk_userlocks;
    unsigned int sk_protocol;
    unsigned int sk_type;
    u16 sk_gso_max_segs;
    u8 sk_pacing_shift;
    long unsigned int sk_lingertime;
    struct proto *sk_prot_creator;
    rwlock_t sk_callback_lock;
    int sk_err;
    int sk_err_soft;
    u32 sk_ack_backlog;
    u32 sk_max_ack_backlog;
    kuid_t sk_uid;
    struct pid *sk_peer_pid;
    const struct cred *sk_peer_cred;
    long int sk_rcvtimeo;
    ktime_t sk_stamp;
    u16 sk_tsflags;
    u8 sk_shutdown;
    u32 sk_tskey;
    atomic_t sk_zckey;
    u8 sk_clockid;
    u8 sk_txtime_deadline_mode;
    u8 sk_txtime_report_errors;
    u8 sk_txtime_unused;
    struct socket *sk_socket;
    void *sk_user_data;
    void *sk_security;
    struct sock_cgroup_data sk_cgrp_data;
    struct mem_cgroup *sk_memcg;
    void (*sk_state_change)(struct sock *);
    void (*sk_data_ready)(struct sock *);
    void (*sk_write_space)(struct sock *);
    void (*sk_error_report)(struct sock *);
    int (*sk_backlog_rcv)(struct sock *, struct sk_buff *);
    struct sk_buff * (*sk_validate_xmit_skb)(struct sock *, struct net_device *, struct sk_buff *);
    void (*sk_destruct)(struct sock *);
    struct sock_reuseport *sk_reuseport_cb;
    struct callback_head sk_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct sock {
    struct sock_common __sk_common;
    socket_lock_t sk_lock;
    atomic_t sk_drops;
    int sk_rcvlowat;
    struct sk_buff_head sk_error_queue;
    struct sk_buff *sk_rx_skb_cache;
    struct sk_buff_head sk_receive_queue;
    struct (anon) sk_backlog;
    int sk_forward_alloc;
    unsigned int sk_ll_usec;
    unsigned int sk_napi_id;
    int sk_rcvbuf;
    struct sk_filter *sk_filter;
    struct socket_wq *sk_wq;
    struct socket_wq *sk_wq_raw;
    struct xfrm_policy * sk_policy[2];
    struct dst_entry *sk_rx_dst;
    struct dst_entry *sk_dst_cache;
    atomic_t sk_omem_alloc;
    int sk_sndbuf;
    int sk_wmem_queued;
    refcount_t sk_wmem_alloc;
    long unsigned int sk_tsq_flags;
    struct sk_buff *sk_send_head;
    struct rb_root tcp_rtx_queue;
    struct sk_buff *sk_tx_skb_cache;
    struct sk_buff_head sk_write_queue;
    __s32 sk_peek_off;
    int sk_write_pending;
    __u32 sk_dst_pending_confirm;
    u32 sk_pacing_status;
    long int sk_sndtimeo;
    struct timer_list sk_timer;
    __u32 sk_priority;
    __u32 sk_mark;
    long unsigned int sk_pacing_rate;
    long unsigned int sk_max_pacing_rate;
    struct page_frag sk_frag;
    netdev_features_t sk_route_caps;
    netdev_features_t sk_route_nocaps;
    netdev_features_t sk_route_forced_caps;
    int sk_gso_type;
    unsigned int sk_gso_max_size;
    gfp_t sk_allocation;
    __u32 sk_txhash;
    unsigned int __sk_flags_offset[0];
    unsigned int sk_padding;
    unsigned int sk_kern_sock;
    unsigned int sk_no_check_tx;
    unsigned int sk_no_check_rx;
    unsigned int sk_userlocks;
    unsigned int sk_protocol;
    unsigned int sk_type;
    u16 sk_gso_max_segs;
    u8 sk_pacing_shift;
    long unsigned int sk_lingertime;
    struct proto *sk_prot_creator;
    rwlock_t sk_callback_lock;
    int sk_err;
    int sk_err_soft;
    u32 sk_ack_backlog;
    u32 sk_max_ack_backlog;
    kuid_t sk_uid;
    struct pid *sk_peer_pid;
    const struct cred *sk_peer_cred;
    long int sk_rcvtimeo;
    ktime_t sk_stamp;
    u16 sk_tsflags;
    u8 sk_shutdown;
    u32 sk_tskey;
    atomic_t sk_zckey;
    u8 sk_clockid;
    u8 sk_txtime_deadline_mode;
    u8 sk_txtime_report_errors;
    u8 sk_txtime_unused;
    struct socket *sk_socket;
    void *sk_user_data;
    void *sk_security;
    struct sock_cgroup_data sk_cgrp_data;
    struct mem_cgroup *sk_memcg;
    void (*sk_state_change)(struct sock *);
    void (*sk_data_ready)(struct sock *);
    void (*sk_write_space)(struct sock *);
    void (*sk_error_report)(struct sock *);
    int (*sk_backlog_rcv)(struct sock *, struct sk_buff *);
    struct sk_buff * (*sk_validate_xmit_skb)(struct sock *, struct net_device *, struct sk_buff *);
    void (*sk_destruct)(struct sock *);
    struct sock_reuseport *sk_reuseport_cb;
    struct bpf_sk_storage *sk_bpf_storage;
    struct callback_head sk_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct sock {
    struct sock_common __sk_common;
    socket_lock_t sk_lock;
    atomic_t sk_drops;
    int sk_rcvlowat;
    struct sk_buff_head sk_error_queue;
    struct sk_buff *sk_rx_skb_cache;
    struct sk_buff_head sk_receive_queue;
    struct (anon) sk_backlog;
    int sk_forward_alloc;
    unsigned int sk_ll_usec;
    unsigned int sk_napi_id;
    int sk_rcvbuf;
    struct sk_filter *sk_filter;
    struct socket_wq *sk_wq;
    struct socket_wq *sk_wq_raw;
    struct xfrm_policy * sk_policy[2];
    struct dst_entry *sk_rx_dst;
    struct dst_entry *sk_dst_cache;
    atomic_t sk_omem_alloc;
    int sk_sndbuf;
    int sk_wmem_queued;
    refcount_t sk_wmem_alloc;
    long unsigned int sk_tsq_flags;
    struct sk_buff *sk_send_head;
    struct rb_root tcp_rtx_queue;
    struct sk_buff *sk_tx_skb_cache;
    struct sk_buff_head sk_write_queue;
    __s32 sk_peek_off;
    int sk_write_pending;
    __u32 sk_dst_pending_confirm;
    u32 sk_pacing_status;
    long int sk_sndtimeo;
    struct timer_list sk_timer;
    __u32 sk_priority;
    __u32 sk_mark;
    long unsigned int sk_pacing_rate;
    long unsigned int sk_max_pacing_rate;
    struct page_frag sk_frag;
    netdev_features_t sk_route_caps;
    netdev_features_t sk_route_nocaps;
    netdev_features_t sk_route_forced_caps;
    int sk_gso_type;
    unsigned int sk_gso_max_size;
    gfp_t sk_allocation;
    __u32 sk_txhash;
    unsigned int __sk_flags_offset[0];
    unsigned int sk_padding;
    unsigned int sk_kern_sock;
    unsigned int sk_no_check_tx;
    unsigned int sk_no_check_rx;
    unsigned int sk_userlocks;
    unsigned int sk_protocol;
    unsigned int sk_type;
    u16 sk_gso_max_segs;
    u8 sk_pacing_shift;
    long unsigned int sk_lingertime;
    struct proto *sk_prot_creator;
    rwlock_t sk_callback_lock;
    int sk_err;
    int sk_err_soft;
    u32 sk_ack_backlog;
    u32 sk_max_ack_backlog;
    kuid_t sk_uid;
    struct pid *sk_peer_pid;
    const struct cred *sk_peer_cred;
    long int sk_rcvtimeo;
    ktime_t sk_stamp;
    u16 sk_tsflags;
    u8 sk_shutdown;
    u32 sk_tskey;
    atomic_t sk_zckey;
    u8 sk_clockid;
    u8 sk_txtime_deadline_mode;
    u8 sk_txtime_report_errors;
    u8 sk_txtime_unused;
    struct socket *sk_socket;
    void *sk_user_data;
    void *sk_security;
    struct sock_cgroup_data sk_cgrp_data;
    struct mem_cgroup *sk_memcg;
    void (*sk_state_change)(struct sock *);
    void (*sk_data_ready)(struct sock *);
    void (*sk_write_space)(struct sock *);
    void (*sk_error_report)(struct sock *);
    int (*sk_backlog_rcv)(struct sock *, struct sk_buff *);
    struct sk_buff * (*sk_validate_xmit_skb)(struct sock *, struct net_device *, struct sk_buff *);
    void (*sk_destruct)(struct sock *);
    struct sock_reuseport *sk_reuseport_cb;
    struct bpf_sk_storage *sk_bpf_storage;
    struct callback_head sk_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct sock {
    struct sock_common __sk_common;
    socket_lock_t sk_lock;
    atomic_t sk_drops;
    int sk_rcvlowat;
    struct sk_buff_head sk_error_queue;
    struct sk_buff *sk_rx_skb_cache;
    struct sk_buff_head sk_receive_queue;
    struct (anon) sk_backlog;
    int sk_forward_alloc;
    unsigned int sk_ll_usec;
    unsigned int sk_napi_id;
    int sk_rcvbuf;
    struct sk_filter *sk_filter;
    struct socket_wq *sk_wq;
    struct socket_wq *sk_wq_raw;
    struct xfrm_policy * sk_policy[2];
    struct dst_entry *sk_rx_dst;
    struct dst_entry *sk_dst_cache;
    atomic_t sk_omem_alloc;
    int sk_sndbuf;
    int sk_wmem_queued;
    refcount_t sk_wmem_alloc;
    long unsigned int sk_tsq_flags;
    struct sk_buff *sk_send_head;
    struct rb_root tcp_rtx_queue;
    struct sk_buff *sk_tx_skb_cache;
    struct sk_buff_head sk_write_queue;
    __s32 sk_peek_off;
    int sk_write_pending;
    __u32 sk_dst_pending_confirm;
    u32 sk_pacing_status;
    long int sk_sndtimeo;
    struct timer_list sk_timer;
    __u32 sk_priority;
    __u32 sk_mark;
    long unsigned int sk_pacing_rate;
    long unsigned int sk_max_pacing_rate;
    struct page_frag sk_frag;
    netdev_features_t sk_route_caps;
    netdev_features_t sk_route_nocaps;
    netdev_features_t sk_route_forced_caps;
    int sk_gso_type;
    unsigned int sk_gso_max_size;
    gfp_t sk_allocation;
    __u32 sk_txhash;
    u8 sk_padding;
    u8 sk_kern_sock;
    u8 sk_no_check_tx;
    u8 sk_no_check_rx;
    u8 sk_userlocks;
    u8 sk_pacing_shift;
    u16 sk_type;
    u16 sk_protocol;
    u16 sk_gso_max_segs;
    long unsigned int sk_lingertime;
    struct proto *sk_prot_creator;
    rwlock_t sk_callback_lock;
    int sk_err;
    int sk_err_soft;
    u32 sk_ack_backlog;
    u32 sk_max_ack_backlog;
    kuid_t sk_uid;
    struct pid *sk_peer_pid;
    const struct cred *sk_peer_cred;
    long int sk_rcvtimeo;
    ktime_t sk_stamp;
    u16 sk_tsflags;
    u8 sk_shutdown;
    u32 sk_tskey;
    atomic_t sk_zckey;
    u8 sk_clockid;
    u8 sk_txtime_deadline_mode;
    u8 sk_txtime_report_errors;
    u8 sk_txtime_unused;
    struct socket *sk_socket;
    void *sk_user_data;
    void *sk_security;
    struct sock_cgroup_data sk_cgrp_data;
    struct mem_cgroup *sk_memcg;
    void (*sk_state_change)(struct sock *);
    void (*sk_data_ready)(struct sock *);
    void (*sk_write_space)(struct sock *);
    void (*sk_error_report)(struct sock *);
    int (*sk_backlog_rcv)(struct sock *, struct sk_buff *);
    struct sk_buff * (*sk_validate_xmit_skb)(struct sock *, struct net_device *, struct sk_buff *);
    void (*sk_destruct)(struct sock *);
    struct sock_reuseport *sk_reuseport_cb;
    struct bpf_sk_storage *sk_bpf_storage;
    struct callback_head sk_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct sock {
    struct sock_common __sk_common;
    socket_lock_t sk_lock;
    atomic_t sk_drops;
    int sk_rcvlowat;
    struct sk_buff_head sk_error_queue;
    struct sk_buff *sk_rx_skb_cache;
    struct sk_buff_head sk_receive_queue;
    struct (anon) sk_backlog;
    int sk_forward_alloc;
    unsigned int sk_ll_usec;
    unsigned int sk_napi_id;
    int sk_rcvbuf;
    struct sk_filter *sk_filter;
    struct socket_wq *sk_wq;
    struct socket_wq *sk_wq_raw;
    struct xfrm_policy * sk_policy[2];
    struct dst_entry *sk_rx_dst;
    struct dst_entry *sk_dst_cache;
    atomic_t sk_omem_alloc;
    int sk_sndbuf;
    int sk_wmem_queued;
    refcount_t sk_wmem_alloc;
    long unsigned int sk_tsq_flags;
    struct sk_buff *sk_send_head;
    struct rb_root tcp_rtx_queue;
    struct sk_buff *sk_tx_skb_cache;
    struct sk_buff_head sk_write_queue;
    __s32 sk_peek_off;
    int sk_write_pending;
    __u32 sk_dst_pending_confirm;
    u32 sk_pacing_status;
    long int sk_sndtimeo;
    struct timer_list sk_timer;
    __u32 sk_priority;
    __u32 sk_mark;
    long unsigned int sk_pacing_rate;
    long unsigned int sk_max_pacing_rate;
    struct page_frag sk_frag;
    netdev_features_t sk_route_caps;
    netdev_features_t sk_route_nocaps;
    netdev_features_t sk_route_forced_caps;
    int sk_gso_type;
    unsigned int sk_gso_max_size;
    gfp_t sk_allocation;
    __u32 sk_txhash;
    u8 sk_padding;
    u8 sk_kern_sock;
    u8 sk_no_check_tx;
    u8 sk_no_check_rx;
    u8 sk_userlocks;
    u8 sk_pacing_shift;
    u16 sk_type;
    u16 sk_protocol;
    u16 sk_gso_max_segs;
    long unsigned int sk_lingertime;
    struct proto *sk_prot_creator;
    rwlock_t sk_callback_lock;
    int sk_err;
    int sk_err_soft;
    u32 sk_ack_backlog;
    u32 sk_max_ack_backlog;
    kuid_t sk_uid;
    u8 sk_prefer_busy_poll;
    u16 sk_busy_poll_budget;
    struct pid *sk_peer_pid;
    const struct cred *sk_peer_cred;
    long int sk_rcvtimeo;
    ktime_t sk_stamp;
    u16 sk_tsflags;
    u8 sk_shutdown;
    u32 sk_tskey;
    atomic_t sk_zckey;
    u8 sk_clockid;
    u8 sk_txtime_deadline_mode;
    u8 sk_txtime_report_errors;
    u8 sk_txtime_unused;
    struct socket *sk_socket;
    void *sk_user_data;
    void *sk_security;
    struct sock_cgroup_data sk_cgrp_data;
    struct mem_cgroup *sk_memcg;
    void (*sk_state_change)(struct sock *);
    void (*sk_data_ready)(struct sock *);
    void (*sk_write_space)(struct sock *);
    void (*sk_error_report)(struct sock *);
    int (*sk_backlog_rcv)(struct sock *, struct sk_buff *);
    struct sk_buff * (*sk_validate_xmit_skb)(struct sock *, struct net_device *, struct sk_buff *);
    void (*sk_destruct)(struct sock *);
    struct sock_reuseport *sk_reuseport_cb;
    struct bpf_local_storage *sk_bpf_storage;
    struct callback_head sk_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct sock {
    struct sock_common __sk_common;
    socket_lock_t sk_lock;
    atomic_t sk_drops;
    int sk_rcvlowat;
    struct sk_buff_head sk_error_queue;
    struct sk_buff *sk_rx_skb_cache;
    struct sk_buff_head sk_receive_queue;
    struct (anon) sk_backlog;
    int sk_forward_alloc;
    unsigned int sk_ll_usec;
    unsigned int sk_napi_id;
    int sk_rcvbuf;
    struct sk_filter *sk_filter;
    struct socket_wq *sk_wq;
    struct socket_wq *sk_wq_raw;
    struct xfrm_policy * sk_policy[2];
    struct dst_entry *sk_rx_dst;
    struct dst_entry *sk_dst_cache;
    atomic_t sk_omem_alloc;
    int sk_sndbuf;
    int sk_wmem_queued;
    refcount_t sk_wmem_alloc;
    long unsigned int sk_tsq_flags;
    struct sk_buff *sk_send_head;
    struct rb_root tcp_rtx_queue;
    struct sk_buff *sk_tx_skb_cache;
    struct sk_buff_head sk_write_queue;
    __s32 sk_peek_off;
    int sk_write_pending;
    __u32 sk_dst_pending_confirm;
    u32 sk_pacing_status;
    long int sk_sndtimeo;
    struct timer_list sk_timer;
    __u32 sk_priority;
    __u32 sk_mark;
    long unsigned int sk_pacing_rate;
    long unsigned int sk_max_pacing_rate;
    struct page_frag sk_frag;
    netdev_features_t sk_route_caps;
    netdev_features_t sk_route_nocaps;
    netdev_features_t sk_route_forced_caps;
    int sk_gso_type;
    unsigned int sk_gso_max_size;
    gfp_t sk_allocation;
    __u32 sk_txhash;
    u8 sk_padding;
    u8 sk_kern_sock;
    u8 sk_no_check_tx;
    u8 sk_no_check_rx;
    u8 sk_userlocks;
    u8 sk_pacing_shift;
    u16 sk_type;
    u16 sk_protocol;
    u16 sk_gso_max_segs;
    long unsigned int sk_lingertime;
    struct proto *sk_prot_creator;
    rwlock_t sk_callback_lock;
    int sk_err;
    int sk_err_soft;
    u32 sk_ack_backlog;
    u32 sk_max_ack_backlog;
    kuid_t sk_uid;
    u8 sk_prefer_busy_poll;
    u16 sk_busy_poll_budget;
    struct pid *sk_peer_pid;
    const struct cred *sk_peer_cred;
    long int sk_rcvtimeo;
    ktime_t sk_stamp;
    u16 sk_tsflags;
    u8 sk_shutdown;
    u32 sk_tskey;
    atomic_t sk_zckey;
    u8 sk_clockid;
    u8 sk_txtime_deadline_mode;
    u8 sk_txtime_report_errors;
    u8 sk_txtime_unused;
    struct socket *sk_socket;
    void *sk_user_data;
    void *sk_security;
    struct sock_cgroup_data sk_cgrp_data;
    struct mem_cgroup *sk_memcg;
    void (*sk_state_change)(struct sock *);
    void (*sk_data_ready)(struct sock *);
    void (*sk_write_space)(struct sock *);
    void (*sk_error_report)(struct sock *);
    int (*sk_backlog_rcv)(struct sock *, struct sk_buff *);
    struct sk_buff * (*sk_validate_xmit_skb)(struct sock *, struct net_device *, struct sk_buff *);
    void (*sk_destruct)(struct sock *);
    struct sock_reuseport *sk_reuseport_cb;
    struct bpf_local_storage *sk_bpf_storage;
    struct callback_head sk_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct sock {
    struct sock_common __sk_common;
    socket_lock_t sk_lock;
    atomic_t sk_drops;
    int sk_rcvlowat;
    struct sk_buff_head sk_error_queue;
    struct sk_buff *sk_rx_skb_cache;
    struct sk_buff_head sk_receive_queue;
    struct (anon) sk_backlog;
    int sk_forward_alloc;
    unsigned int sk_ll_usec;
    unsigned int sk_napi_id;
    int sk_rcvbuf;
    struct sk_filter *sk_filter;
    struct socket_wq *sk_wq;
    struct socket_wq *sk_wq_raw;
    struct xfrm_policy * sk_policy[2];
    struct dst_entry *sk_rx_dst;
    int sk_rx_dst_ifindex;
    u32 sk_rx_dst_cookie;
    struct dst_entry *sk_dst_cache;
    atomic_t sk_omem_alloc;
    int sk_sndbuf;
    int sk_wmem_queued;
    refcount_t sk_wmem_alloc;
    long unsigned int sk_tsq_flags;
    struct sk_buff *sk_send_head;
    struct rb_root tcp_rtx_queue;
    struct sk_buff *sk_tx_skb_cache;
    struct sk_buff_head sk_write_queue;
    __s32 sk_peek_off;
    int sk_write_pending;
    __u32 sk_dst_pending_confirm;
    u32 sk_pacing_status;
    long int sk_sndtimeo;
    struct timer_list sk_timer;
    __u32 sk_priority;
    __u32 sk_mark;
    long unsigned int sk_pacing_rate;
    long unsigned int sk_max_pacing_rate;
    struct page_frag sk_frag;
    netdev_features_t sk_route_caps;
    netdev_features_t sk_route_nocaps;
    netdev_features_t sk_route_forced_caps;
    int sk_gso_type;
    unsigned int sk_gso_max_size;
    gfp_t sk_allocation;
    __u32 sk_txhash;
    u8 sk_padding;
    u8 sk_kern_sock;
    u8 sk_no_check_tx;
    u8 sk_no_check_rx;
    u8 sk_userlocks;
    u8 sk_pacing_shift;
    u16 sk_type;
    u16 sk_protocol;
    u16 sk_gso_max_segs;
    long unsigned int sk_lingertime;
    struct proto *sk_prot_creator;
    rwlock_t sk_callback_lock;
    int sk_err;
    int sk_err_soft;
    u32 sk_ack_backlog;
    u32 sk_max_ack_backlog;
    kuid_t sk_uid;
    u8 sk_prefer_busy_poll;
    u16 sk_busy_poll_budget;
    spinlock_t sk_peer_lock;
    struct pid *sk_peer_pid;
    const struct cred *sk_peer_cred;
    long int sk_rcvtimeo;
    ktime_t sk_stamp;
    u16 sk_tsflags;
    int sk_bind_phc;
    u8 sk_shutdown;
    atomic_t sk_tskey;
    atomic_t sk_zckey;
    u8 sk_clockid;
    u8 sk_txtime_deadline_mode;
    u8 sk_txtime_report_errors;
    u8 sk_txtime_unused;
    struct socket *sk_socket;
    void *sk_user_data;
    void *sk_security;
    struct sock_cgroup_data sk_cgrp_data;
    struct mem_cgroup *sk_memcg;
    void (*sk_state_change)(struct sock *);
    void (*sk_data_ready)(struct sock *);
    void (*sk_write_space)(struct sock *);
    void (*sk_error_report)(struct sock *);
    int (*sk_backlog_rcv)(struct sock *, struct sk_buff *);
    struct sk_buff * (*sk_validate_xmit_skb)(struct sock *, struct net_device *, struct sk_buff *);
    void (*sk_destruct)(struct sock *);
    struct sock_reuseport *sk_reuseport_cb;
    struct bpf_local_storage *sk_bpf_storage;
    struct callback_head sk_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct sock {
    struct sock_common __sk_common;
    struct dst_entry *sk_rx_dst;
    int sk_rx_dst_ifindex;
    u32 sk_rx_dst_cookie;
    socket_lock_t sk_lock;
    atomic_t sk_drops;
    int sk_rcvlowat;
    struct sk_buff_head sk_error_queue;
    struct sk_buff_head sk_receive_queue;
    struct (anon) sk_backlog;
    int sk_forward_alloc;
    u32 sk_reserved_mem;
    unsigned int sk_ll_usec;
    unsigned int sk_napi_id;
    int sk_rcvbuf;
    struct sk_filter *sk_filter;
    struct socket_wq *sk_wq;
    struct socket_wq *sk_wq_raw;
    struct xfrm_policy * sk_policy[2];
    struct dst_entry *sk_dst_cache;
    atomic_t sk_omem_alloc;
    int sk_sndbuf;
    int sk_wmem_queued;
    refcount_t sk_wmem_alloc;
    long unsigned int sk_tsq_flags;
    struct sk_buff *sk_send_head;
    struct rb_root tcp_rtx_queue;
    struct sk_buff_head sk_write_queue;
    __s32 sk_peek_off;
    int sk_write_pending;
    __u32 sk_dst_pending_confirm;
    u32 sk_pacing_status;
    long int sk_sndtimeo;
    struct timer_list sk_timer;
    __u32 sk_priority;
    __u32 sk_mark;
    long unsigned int sk_pacing_rate;
    long unsigned int sk_max_pacing_rate;
    struct page_frag sk_frag;
    netdev_features_t sk_route_caps;
    int sk_gso_type;
    unsigned int sk_gso_max_size;
    gfp_t sk_allocation;
    __u32 sk_txhash;
    u8 sk_gso_disabled;
    u8 sk_kern_sock;
    u8 sk_no_check_tx;
    u8 sk_no_check_rx;
    u8 sk_userlocks;
    u8 sk_pacing_shift;
    u16 sk_type;
    u16 sk_protocol;
    u16 sk_gso_max_segs;
    long unsigned int sk_lingertime;
    struct proto *sk_prot_creator;
    rwlock_t sk_callback_lock;
    int sk_err;
    int sk_err_soft;
    u32 sk_ack_backlog;
    u32 sk_max_ack_backlog;
    kuid_t sk_uid;
    u8 sk_txrehash;
    u8 sk_prefer_busy_poll;
    u16 sk_busy_poll_budget;
    spinlock_t sk_peer_lock;
    int sk_bind_phc;
    struct pid *sk_peer_pid;
    const struct cred *sk_peer_cred;
    long int sk_rcvtimeo;
    ktime_t sk_stamp;
    u16 sk_tsflags;
    u8 sk_shutdown;
    atomic_t sk_tskey;
    atomic_t sk_zckey;
    u8 sk_clockid;
    u8 sk_txtime_deadline_mode;
    u8 sk_txtime_report_errors;
    u8 sk_txtime_unused;
    struct socket *sk_socket;
    void *sk_user_data;
    void *sk_security;
    struct sock_cgroup_data sk_cgrp_data;
    struct mem_cgroup *sk_memcg;
    void (*sk_state_change)(struct sock *);
    void (*sk_data_ready)(struct sock *);
    void (*sk_write_space)(struct sock *);
    void (*sk_error_report)(struct sock *);
    int (*sk_backlog_rcv)(struct sock *, struct sk_buff *);
    struct sk_buff * (*sk_validate_xmit_skb)(struct sock *, struct net_device *, struct sk_buff *);
    void (*sk_destruct)(struct sock *);
    struct sock_reuseport *sk_reuseport_cb;
    struct bpf_local_storage *sk_bpf_storage;
    struct callback_head sk_rcu;
    netns_tracker ns_tracker;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct sock {
    struct sock_common __sk_common;
    struct dst_entry *sk_rx_dst;
    int sk_rx_dst_ifindex;
    u32 sk_rx_dst_cookie;
    socket_lock_t sk_lock;
    atomic_t sk_drops;
    int sk_rcvlowat;
    struct sk_buff_head sk_error_queue;
    struct sk_buff_head sk_receive_queue;
    struct (anon) sk_backlog;
    int sk_forward_alloc;
    u32 sk_reserved_mem;
    unsigned int sk_ll_usec;
    unsigned int sk_napi_id;
    int sk_rcvbuf;
    struct sk_filter *sk_filter;
    struct socket_wq *sk_wq;
    struct socket_wq *sk_wq_raw;
    struct xfrm_policy * sk_policy[2];
    struct dst_entry *sk_dst_cache;
    atomic_t sk_omem_alloc;
    int sk_sndbuf;
    int sk_wmem_queued;
    refcount_t sk_wmem_alloc;
    long unsigned int sk_tsq_flags;
    struct sk_buff *sk_send_head;
    struct rb_root tcp_rtx_queue;
    struct sk_buff_head sk_write_queue;
    __s32 sk_peek_off;
    int sk_write_pending;
    __u32 sk_dst_pending_confirm;
    u32 sk_pacing_status;
    long int sk_sndtimeo;
    struct timer_list sk_timer;
    __u32 sk_priority;
    __u32 sk_mark;
    long unsigned int sk_pacing_rate;
    long unsigned int sk_max_pacing_rate;
    struct page_frag sk_frag;
    netdev_features_t sk_route_caps;
    int sk_gso_type;
    unsigned int sk_gso_max_size;
    gfp_t sk_allocation;
    __u32 sk_txhash;
    u8 sk_gso_disabled;
    u8 sk_kern_sock;
    u8 sk_no_check_tx;
    u8 sk_no_check_rx;
    u8 sk_userlocks;
    u8 sk_pacing_shift;
    u16 sk_type;
    u16 sk_protocol;
    u16 sk_gso_max_segs;
    long unsigned int sk_lingertime;
    struct proto *sk_prot_creator;
    rwlock_t sk_callback_lock;
    int sk_err;
    int sk_err_soft;
    u32 sk_ack_backlog;
    u32 sk_max_ack_backlog;
    kuid_t sk_uid;
    u8 sk_txrehash;
    u8 sk_prefer_busy_poll;
    u16 sk_busy_poll_budget;
    spinlock_t sk_peer_lock;
    int sk_bind_phc;
    struct pid *sk_peer_pid;
    const struct cred *sk_peer_cred;
    long int sk_rcvtimeo;
    ktime_t sk_stamp;
    atomic_t sk_tskey;
    atomic_t sk_zckey;
    u32 sk_tsflags;
    u8 sk_shutdown;
    u8 sk_clockid;
    u8 sk_txtime_deadline_mode;
    u8 sk_txtime_report_errors;
    u8 sk_txtime_unused;
    bool sk_use_task_frag;
    struct socket *sk_socket;
    void *sk_user_data;
    void *sk_security;
    struct sock_cgroup_data sk_cgrp_data;
    struct mem_cgroup *sk_memcg;
    void (*sk_state_change)(struct sock *);
    void (*sk_data_ready)(struct sock *);
    void (*sk_write_space)(struct sock *);
    void (*sk_error_report)(struct sock *);
    int (*sk_backlog_rcv)(struct sock *, struct sk_buff *);
    struct sk_buff * (*sk_validate_xmit_skb)(struct sock *, struct net_device *, struct sk_buff *);
    void (*sk_destruct)(struct sock *);
    struct sock_reuseport *sk_reuseport_cb;
    struct bpf_local_storage *sk_bpf_storage;
    struct callback_head sk_rcu;
    netns_tracker ns_tracker;
    struct hlist_node sk_bind2_node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct sock {
    struct sock_common __sk_common;
    struct dst_entry *sk_rx_dst;
    int sk_rx_dst_ifindex;
    u32 sk_rx_dst_cookie;
    socket_lock_t sk_lock;
    atomic_t sk_drops;
    int sk_rcvlowat;
    struct sk_buff_head sk_error_queue;
    struct sk_buff_head sk_receive_queue;
    struct (anon) sk_backlog;
    int sk_forward_alloc;
    u32 sk_reserved_mem;
    unsigned int sk_ll_usec;
    unsigned int sk_napi_id;
    int sk_rcvbuf;
    int sk_wait_pending;
    struct sk_filter *sk_filter;
    struct socket_wq *sk_wq;
    struct socket_wq *sk_wq_raw;
    struct xfrm_policy * sk_policy[2];
    struct dst_entry *sk_dst_cache;
    atomic_t sk_omem_alloc;
    int sk_sndbuf;
    int sk_wmem_queued;
    refcount_t sk_wmem_alloc;
    long unsigned int sk_tsq_flags;
    struct sk_buff *sk_send_head;
    struct rb_root tcp_rtx_queue;
    struct sk_buff_head sk_write_queue;
    __s32 sk_peek_off;
    int sk_write_pending;
    __u32 sk_dst_pending_confirm;
    u32 sk_pacing_status;
    long int sk_sndtimeo;
    struct timer_list sk_timer;
    __u32 sk_priority;
    __u32 sk_mark;
    long unsigned int sk_pacing_rate;
    long unsigned int sk_max_pacing_rate;
    struct page_frag sk_frag;
    netdev_features_t sk_route_caps;
    int sk_gso_type;
    unsigned int sk_gso_max_size;
    gfp_t sk_allocation;
    __u32 sk_txhash;
    u8 sk_gso_disabled;
    u8 sk_kern_sock;
    u8 sk_no_check_tx;
    u8 sk_no_check_rx;
    u8 sk_userlocks;
    u8 sk_pacing_shift;
    u16 sk_type;
    u16 sk_protocol;
    u16 sk_gso_max_segs;
    long unsigned int sk_lingertime;
    struct proto *sk_prot_creator;
    rwlock_t sk_callback_lock;
    int sk_err;
    int sk_err_soft;
    u32 sk_ack_backlog;
    u32 sk_max_ack_backlog;
    kuid_t sk_uid;
    u8 sk_txrehash;
    u8 sk_prefer_busy_poll;
    u16 sk_busy_poll_budget;
    spinlock_t sk_peer_lock;
    int sk_bind_phc;
    struct pid *sk_peer_pid;
    const struct cred *sk_peer_cred;
    long int sk_rcvtimeo;
    ktime_t sk_stamp;
    atomic_t sk_tskey;
    atomic_t sk_zckey;
    u32 sk_tsflags;
    u8 sk_shutdown;
    u8 sk_clockid;
    u8 sk_txtime_deadline_mode;
    u8 sk_txtime_report_errors;
    u8 sk_txtime_unused;
    bool sk_use_task_frag;
    struct socket *sk_socket;
    void *sk_user_data;
    void *sk_security;
    struct sock_cgroup_data sk_cgrp_data;
    struct mem_cgroup *sk_memcg;
    void (*sk_state_change)(struct sock *);
    void (*sk_data_ready)(struct sock *);
    void (*sk_write_space)(struct sock *);
    void (*sk_error_report)(struct sock *);
    int (*sk_backlog_rcv)(struct sock *, struct sk_buff *);
    struct sk_buff * (*sk_validate_xmit_skb)(struct sock *, struct net_device *, struct sk_buff *);
    void (*sk_destruct)(struct sock *);
    struct sock_reuseport *sk_reuseport_cb;
    struct bpf_local_storage *sk_bpf_storage;
    struct callback_head sk_rcu;
    netns_tracker ns_tracker;
    struct hlist_node sk_bind2_node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct sock {
    struct sock_common __sk_common;
    struct dst_entry *sk_rx_dst;
    int sk_rx_dst_ifindex;
    u32 sk_rx_dst_cookie;
    socket_lock_t sk_lock;
    atomic_t sk_drops;
    int sk_rcvlowat;
    struct sk_buff_head sk_error_queue;
    struct sk_buff_head sk_receive_queue;
    struct (anon) sk_backlog;
    int sk_forward_alloc;
    u32 sk_reserved_mem;
    unsigned int sk_ll_usec;
    unsigned int sk_napi_id;
    int sk_rcvbuf;
    int sk_disconnects;
    struct sk_filter *sk_filter;
    struct socket_wq *sk_wq;
    struct socket_wq *sk_wq_raw;
    struct xfrm_policy * sk_policy[2];
    struct dst_entry *sk_dst_cache;
    atomic_t sk_omem_alloc;
    int sk_sndbuf;
    int sk_wmem_queued;
    refcount_t sk_wmem_alloc;
    long unsigned int sk_tsq_flags;
    struct sk_buff *sk_send_head;
    struct rb_root tcp_rtx_queue;
    struct sk_buff_head sk_write_queue;
    __s32 sk_peek_off;
    int sk_write_pending;
    __u32 sk_dst_pending_confirm;
    u32 sk_pacing_status;
    long int sk_sndtimeo;
    struct timer_list sk_timer;
    __u32 sk_priority;
    __u32 sk_mark;
    long unsigned int sk_pacing_rate;
    long unsigned int sk_max_pacing_rate;
    struct page_frag sk_frag;
    netdev_features_t sk_route_caps;
    int sk_gso_type;
    unsigned int sk_gso_max_size;
    gfp_t sk_allocation;
    __u32 sk_txhash;
    u8 sk_gso_disabled;
    u8 sk_kern_sock;
    u8 sk_no_check_tx;
    u8 sk_no_check_rx;
    u8 sk_userlocks;
    u8 sk_pacing_shift;
    u16 sk_type;
    u16 sk_protocol;
    u16 sk_gso_max_segs;
    long unsigned int sk_lingertime;
    struct proto *sk_prot_creator;
    rwlock_t sk_callback_lock;
    int sk_err;
    int sk_err_soft;
    u32 sk_ack_backlog;
    u32 sk_max_ack_backlog;
    kuid_t sk_uid;
    u8 sk_txrehash;
    u8 sk_prefer_busy_poll;
    u16 sk_busy_poll_budget;
    spinlock_t sk_peer_lock;
    int sk_bind_phc;
    struct pid *sk_peer_pid;
    const struct cred *sk_peer_cred;
    long int sk_rcvtimeo;
    ktime_t sk_stamp;
    atomic_t sk_tskey;
    atomic_t sk_zckey;
    u32 sk_tsflags;
    u8 sk_shutdown;
    u8 sk_clockid;
    u8 sk_txtime_deadline_mode;
    u8 sk_txtime_report_errors;
    u8 sk_txtime_unused;
    bool sk_use_task_frag;
    struct socket *sk_socket;
    void *sk_user_data;
    void *sk_security;
    struct sock_cgroup_data sk_cgrp_data;
    struct mem_cgroup *sk_memcg;
    void (*sk_state_change)(struct sock *);
    void (*sk_data_ready)(struct sock *);
    void (*sk_write_space)(struct sock *);
    void (*sk_error_report)(struct sock *);
    int (*sk_backlog_rcv)(struct sock *, struct sk_buff *);
    struct sk_buff * (*sk_validate_xmit_skb)(struct sock *, struct net_device *, struct sk_buff *);
    void (*sk_destruct)(struct sock *);
    struct sock_reuseport *sk_reuseport_cb;
    struct bpf_local_storage *sk_bpf_storage;
    struct callback_head sk_rcu;
    netns_tracker ns_tracker;
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
struct sock {
    struct sock_common __sk_common;
    socket_lock_t sk_lock;
    atomic_t sk_drops;
    int sk_rcvlowat;
    struct sk_buff_head sk_error_queue;
    struct sk_buff *sk_rx_skb_cache;
    struct sk_buff_head sk_receive_queue;
    struct (anon) sk_backlog;
    int sk_forward_alloc;
    unsigned int sk_ll_usec;
    unsigned int sk_napi_id;
    int sk_rcvbuf;
    struct sk_filter *sk_filter;
    struct socket_wq *sk_wq;
    struct socket_wq *sk_wq_raw;
    struct xfrm_policy * sk_policy[2];
    struct dst_entry *sk_rx_dst;
    struct dst_entry *sk_dst_cache;
    atomic_t sk_omem_alloc;
    int sk_sndbuf;
    int sk_wmem_queued;
    refcount_t sk_wmem_alloc;
    long unsigned int sk_tsq_flags;
    struct sk_buff *sk_send_head;
    struct rb_root tcp_rtx_queue;
    struct sk_buff *sk_tx_skb_cache;
    struct sk_buff_head sk_write_queue;
    __s32 sk_peek_off;
    int sk_write_pending;
    __u32 sk_dst_pending_confirm;
    u32 sk_pacing_status;
    long int sk_sndtimeo;
    struct timer_list sk_timer;
    __u32 sk_priority;
    __u32 sk_mark;
    long unsigned int sk_pacing_rate;
    long unsigned int sk_max_pacing_rate;
    struct page_frag sk_frag;
    netdev_features_t sk_route_caps;
    netdev_features_t sk_route_nocaps;
    netdev_features_t sk_route_forced_caps;
    int sk_gso_type;
    unsigned int sk_gso_max_size;
    gfp_t sk_allocation;
    __u32 sk_txhash;
    unsigned int __sk_flags_offset[0];
    unsigned int sk_padding;
    unsigned int sk_kern_sock;
    unsigned int sk_no_check_tx;
    unsigned int sk_no_check_rx;
    unsigned int sk_userlocks;
    unsigned int sk_protocol;
    unsigned int sk_type;
    u16 sk_gso_max_segs;
    u8 sk_pacing_shift;
    long unsigned int sk_lingertime;
    struct proto *sk_prot_creator;
    rwlock_t sk_callback_lock;
    int sk_err;
    int sk_err_soft;
    u32 sk_ack_backlog;
    u32 sk_max_ack_backlog;
    kuid_t sk_uid;
    struct pid *sk_peer_pid;
    const struct cred *sk_peer_cred;
    long int sk_rcvtimeo;
    ktime_t sk_stamp;
    u16 sk_tsflags;
    u8 sk_shutdown;
    u32 sk_tskey;
    atomic_t sk_zckey;
    u8 sk_clockid;
    u8 sk_txtime_deadline_mode;
    u8 sk_txtime_report_errors;
    u8 sk_txtime_unused;
    struct socket *sk_socket;
    void *sk_user_data;
    void *sk_security;
    struct sock_cgroup_data sk_cgrp_data;
    struct mem_cgroup *sk_memcg;
    void (*sk_state_change)(struct sock *);
    void (*sk_data_ready)(struct sock *);
    void (*sk_write_space)(struct sock *);
    void (*sk_error_report)(struct sock *);
    int (*sk_backlog_rcv)(struct sock *, struct sk_buff *);
    struct sk_buff * (*sk_validate_xmit_skb)(struct sock *, struct net_device *, struct sk_buff *);
    void (*sk_destruct)(struct sock *);
    struct sock_reuseport *sk_reuseport_cb;
    struct bpf_sk_storage *sk_bpf_storage;
    struct callback_head sk_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct sock {
    struct sock_common __sk_common;
    socket_lock_t sk_lock;
    atomic_t sk_drops;
    int sk_rcvlowat;
    struct sk_buff_head sk_error_queue;
    struct sk_buff *sk_rx_skb_cache;
    struct sk_buff_head sk_receive_queue;
    struct (anon) sk_backlog;
    int sk_forward_alloc;
    unsigned int sk_ll_usec;
    unsigned int sk_napi_id;
    int sk_rcvbuf;
    struct sk_filter *sk_filter;
    struct socket_wq *sk_wq;
    struct socket_wq *sk_wq_raw;
    struct xfrm_policy * sk_policy[2];
    struct dst_entry *sk_rx_dst;
    struct dst_entry *sk_dst_cache;
    atomic_t sk_omem_alloc;
    int sk_sndbuf;
    int sk_wmem_queued;
    refcount_t sk_wmem_alloc;
    long unsigned int sk_tsq_flags;
    struct sk_buff *sk_send_head;
    struct rb_root tcp_rtx_queue;
    struct sk_buff *sk_tx_skb_cache;
    struct sk_buff_head sk_write_queue;
    __s32 sk_peek_off;
    int sk_write_pending;
    __u32 sk_dst_pending_confirm;
    u32 sk_pacing_status;
    long int sk_sndtimeo;
    struct timer_list sk_timer;
    __u32 sk_priority;
    __u32 sk_mark;
    long unsigned int sk_pacing_rate;
    long unsigned int sk_max_pacing_rate;
    struct page_frag sk_frag;
    netdev_features_t sk_route_caps;
    netdev_features_t sk_route_nocaps;
    netdev_features_t sk_route_forced_caps;
    int sk_gso_type;
    unsigned int sk_gso_max_size;
    gfp_t sk_allocation;
    __u32 sk_txhash;
    unsigned int __sk_flags_offset[0];
    unsigned int sk_padding;
    unsigned int sk_kern_sock;
    unsigned int sk_no_check_tx;
    unsigned int sk_no_check_rx;
    unsigned int sk_userlocks;
    unsigned int sk_protocol;
    unsigned int sk_type;
    u16 sk_gso_max_segs;
    u8 sk_pacing_shift;
    long unsigned int sk_lingertime;
    struct proto *sk_prot_creator;
    rwlock_t sk_callback_lock;
    int sk_err;
    int sk_err_soft;
    u32 sk_ack_backlog;
    u32 sk_max_ack_backlog;
    kuid_t sk_uid;
    struct pid *sk_peer_pid;
    const struct cred *sk_peer_cred;
    long int sk_rcvtimeo;
    ktime_t sk_stamp;
    seqlock_t sk_stamp_seq;
    u16 sk_tsflags;
    u8 sk_shutdown;
    u32 sk_tskey;
    atomic_t sk_zckey;
    u8 sk_clockid;
    u8 sk_txtime_deadline_mode;
    u8 sk_txtime_report_errors;
    u8 sk_txtime_unused;
    struct socket *sk_socket;
    void *sk_user_data;
    void *sk_security;
    struct sock_cgroup_data sk_cgrp_data;
    struct mem_cgroup *sk_memcg;
    void (*sk_state_change)(struct sock *);
    void (*sk_data_ready)(struct sock *);
    void (*sk_write_space)(struct sock *);
    void (*sk_error_report)(struct sock *);
    int (*sk_backlog_rcv)(struct sock *, struct sk_buff *);
    struct sk_buff * (*sk_validate_xmit_skb)(struct sock *, struct net_device *, struct sk_buff *);
    void (*sk_destruct)(struct sock *);
    struct sock_reuseport *sk_reuseport_cb;
    struct bpf_sk_storage *sk_bpf_storage;
    struct callback_head sk_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct sock {
    struct sock_common __sk_common;
    socket_lock_t sk_lock;
    atomic_t sk_drops;
    int sk_rcvlowat;
    struct sk_buff_head sk_error_queue;
    struct sk_buff *sk_rx_skb_cache;
    struct sk_buff_head sk_receive_queue;
    struct (anon) sk_backlog;
    int sk_forward_alloc;
    unsigned int sk_ll_usec;
    unsigned int sk_napi_id;
    int sk_rcvbuf;
    struct sk_filter *sk_filter;
    struct socket_wq *sk_wq;
    struct socket_wq *sk_wq_raw;
    struct xfrm_policy * sk_policy[2];
    struct dst_entry *sk_rx_dst;
    struct dst_entry *sk_dst_cache;
    atomic_t sk_omem_alloc;
    int sk_sndbuf;
    int sk_wmem_queued;
    refcount_t sk_wmem_alloc;
    long unsigned int sk_tsq_flags;
    struct sk_buff *sk_send_head;
    struct rb_root tcp_rtx_queue;
    struct sk_buff *sk_tx_skb_cache;
    struct sk_buff_head sk_write_queue;
    __s32 sk_peek_off;
    int sk_write_pending;
    __u32 sk_dst_pending_confirm;
    u32 sk_pacing_status;
    long int sk_sndtimeo;
    struct timer_list sk_timer;
    __u32 sk_priority;
    __u32 sk_mark;
    long unsigned int sk_pacing_rate;
    long unsigned int sk_max_pacing_rate;
    struct page_frag sk_frag;
    netdev_features_t sk_route_caps;
    netdev_features_t sk_route_nocaps;
    netdev_features_t sk_route_forced_caps;
    int sk_gso_type;
    unsigned int sk_gso_max_size;
    gfp_t sk_allocation;
    __u32 sk_txhash;
    unsigned int __sk_flags_offset[0];
    unsigned int sk_padding;
    unsigned int sk_kern_sock;
    unsigned int sk_no_check_tx;
    unsigned int sk_no_check_rx;
    unsigned int sk_userlocks;
    unsigned int sk_protocol;
    unsigned int sk_type;
    u16 sk_gso_max_segs;
    u8 sk_pacing_shift;
    long unsigned int sk_lingertime;
    struct proto *sk_prot_creator;
    rwlock_t sk_callback_lock;
    int sk_err;
    int sk_err_soft;
    u32 sk_ack_backlog;
    u32 sk_max_ack_backlog;
    kuid_t sk_uid;
    struct pid *sk_peer_pid;
    const struct cred *sk_peer_cred;
    long int sk_rcvtimeo;
    ktime_t sk_stamp;
    u16 sk_tsflags;
    u8 sk_shutdown;
    u32 sk_tskey;
    atomic_t sk_zckey;
    u8 sk_clockid;
    u8 sk_txtime_deadline_mode;
    u8 sk_txtime_report_errors;
    u8 sk_txtime_unused;
    struct socket *sk_socket;
    void *sk_user_data;
    void *sk_security;
    struct sock_cgroup_data sk_cgrp_data;
    struct mem_cgroup *sk_memcg;
    void (*sk_state_change)(struct sock *);
    void (*sk_data_ready)(struct sock *);
    void (*sk_write_space)(struct sock *);
    void (*sk_error_report)(struct sock *);
    int (*sk_backlog_rcv)(struct sock *, struct sk_buff *);
    struct sk_buff * (*sk_validate_xmit_skb)(struct sock *, struct net_device *, struct sk_buff *);
    void (*sk_destruct)(struct sock *);
    struct sock_reuseport *sk_reuseport_cb;
    struct bpf_sk_storage *sk_bpf_storage;
    struct callback_head sk_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct sock {
    struct sock_common __sk_common;
    socket_lock_t sk_lock;
    atomic_t sk_drops;
    int sk_rcvlowat;
    struct sk_buff_head sk_error_queue;
    struct sk_buff *sk_rx_skb_cache;
    struct sk_buff_head sk_receive_queue;
    struct (anon) sk_backlog;
    int sk_forward_alloc;
    unsigned int sk_ll_usec;
    unsigned int sk_napi_id;
    int sk_rcvbuf;
    struct sk_filter *sk_filter;
    struct socket_wq *sk_wq;
    struct socket_wq *sk_wq_raw;
    struct xfrm_policy * sk_policy[2];
    struct dst_entry *sk_rx_dst;
    struct dst_entry *sk_dst_cache;
    atomic_t sk_omem_alloc;
    int sk_sndbuf;
    int sk_wmem_queued;
    refcount_t sk_wmem_alloc;
    long unsigned int sk_tsq_flags;
    struct sk_buff *sk_send_head;
    struct rb_root tcp_rtx_queue;
    struct sk_buff *sk_tx_skb_cache;
    struct sk_buff_head sk_write_queue;
    __s32 sk_peek_off;
    int sk_write_pending;
    __u32 sk_dst_pending_confirm;
    u32 sk_pacing_status;
    long int sk_sndtimeo;
    struct timer_list sk_timer;
    __u32 sk_priority;
    __u32 sk_mark;
    long unsigned int sk_pacing_rate;
    long unsigned int sk_max_pacing_rate;
    struct page_frag sk_frag;
    netdev_features_t sk_route_caps;
    netdev_features_t sk_route_nocaps;
    netdev_features_t sk_route_forced_caps;
    int sk_gso_type;
    unsigned int sk_gso_max_size;
    gfp_t sk_allocation;
    __u32 sk_txhash;
    unsigned int __sk_flags_offset[0];
    unsigned int sk_padding;
    unsigned int sk_kern_sock;
    unsigned int sk_no_check_tx;
    unsigned int sk_no_check_rx;
    unsigned int sk_userlocks;
    unsigned int sk_protocol;
    unsigned int sk_type;
    u16 sk_gso_max_segs;
    u8 sk_pacing_shift;
    long unsigned int sk_lingertime;
    struct proto *sk_prot_creator;
    rwlock_t sk_callback_lock;
    int sk_err;
    int sk_err_soft;
    u32 sk_ack_backlog;
    u32 sk_max_ack_backlog;
    kuid_t sk_uid;
    struct pid *sk_peer_pid;
    const struct cred *sk_peer_cred;
    long int sk_rcvtimeo;
    ktime_t sk_stamp;
    u16 sk_tsflags;
    u8 sk_shutdown;
    u32 sk_tskey;
    atomic_t sk_zckey;
    u8 sk_clockid;
    u8 sk_txtime_deadline_mode;
    u8 sk_txtime_report_errors;
    u8 sk_txtime_unused;
    struct socket *sk_socket;
    void *sk_user_data;
    void *sk_security;
    struct sock_cgroup_data sk_cgrp_data;
    struct mem_cgroup *sk_memcg;
    void (*sk_state_change)(struct sock *);
    void (*sk_data_ready)(struct sock *);
    void (*sk_write_space)(struct sock *);
    void (*sk_error_report)(struct sock *);
    int (*sk_backlog_rcv)(struct sock *, struct sk_buff *);
    struct sk_buff * (*sk_validate_xmit_skb)(struct sock *, struct net_device *, struct sk_buff *);
    void (*sk_destruct)(struct sock *);
    struct sock_reuseport *sk_reuseport_cb;
    struct bpf_sk_storage *sk_bpf_storage;
    struct callback_head sk_rcu;
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
struct sock {
    struct sock_common __sk_common;
    socket_lock_t sk_lock;
    atomic_t sk_drops;
    int sk_rcvlowat;
    struct sk_buff_head sk_error_queue;
    struct sk_buff *sk_rx_skb_cache;
    struct sk_buff_head sk_receive_queue;
    struct (anon) sk_backlog;
    int sk_forward_alloc;
    unsigned int sk_ll_usec;
    unsigned int sk_napi_id;
    int sk_rcvbuf;
    struct sk_filter *sk_filter;
    struct socket_wq *sk_wq;
    struct socket_wq *sk_wq_raw;
    struct xfrm_policy * sk_policy[2];
    struct dst_entry *sk_rx_dst;
    struct dst_entry *sk_dst_cache;
    atomic_t sk_omem_alloc;
    int sk_sndbuf;
    int sk_wmem_queued;
    refcount_t sk_wmem_alloc;
    long unsigned int sk_tsq_flags;
    struct sk_buff *sk_send_head;
    struct rb_root tcp_rtx_queue;
    struct sk_buff *sk_tx_skb_cache;
    struct sk_buff_head sk_write_queue;
    __s32 sk_peek_off;
    int sk_write_pending;
    __u32 sk_dst_pending_confirm;
    u32 sk_pacing_status;
    long int sk_sndtimeo;
    struct timer_list sk_timer;
    __u32 sk_priority;
    __u32 sk_mark;
    long unsigned int sk_pacing_rate;
    long unsigned int sk_max_pacing_rate;
    struct page_frag sk_frag;
    netdev_features_t sk_route_caps;
    netdev_features_t sk_route_nocaps;
    netdev_features_t sk_route_forced_caps;
    int sk_gso_type;
    unsigned int sk_gso_max_size;
    gfp_t sk_allocation;
    __u32 sk_txhash;
    unsigned int __sk_flags_offset[0];
    unsigned int sk_padding;
    unsigned int sk_kern_sock;
    unsigned int sk_no_check_tx;
    unsigned int sk_no_check_rx;
    unsigned int sk_userlocks;
    unsigned int sk_protocol;
    unsigned int sk_type;
    u16 sk_gso_max_segs;
    u8 sk_pacing_shift;
    long unsigned int sk_lingertime;
    struct proto *sk_prot_creator;
    rwlock_t sk_callback_lock;
    int sk_err;
    int sk_err_soft;
    u32 sk_ack_backlog;
    u32 sk_max_ack_backlog;
    kuid_t sk_uid;
    struct pid *sk_peer_pid;
    const struct cred *sk_peer_cred;
    long int sk_rcvtimeo;
    ktime_t sk_stamp;
    u16 sk_tsflags;
    u8 sk_shutdown;
    u32 sk_tskey;
    atomic_t sk_zckey;
    u8 sk_clockid;
    u8 sk_txtime_deadline_mode;
    u8 sk_txtime_report_errors;
    u8 sk_txtime_unused;
    struct socket *sk_socket;
    void *sk_user_data;
    void *sk_security;
    struct sock_cgroup_data sk_cgrp_data;
    struct mem_cgroup *sk_memcg;
    void (*sk_state_change)(struct sock *);
    void (*sk_data_ready)(struct sock *);
    void (*sk_write_space)(struct sock *);
    void (*sk_error_report)(struct sock *);
    int (*sk_backlog_rcv)(struct sock *, struct sk_buff *);
    struct sk_buff * (*sk_validate_xmit_skb)(struct sock *, struct net_device *, struct sk_buff *);
    void (*sk_destruct)(struct sock *);
    struct sock_reuseport *sk_reuseport_cb;
    struct bpf_sk_storage *sk_bpf_storage;
    struct callback_head sk_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct sock {
    struct sock_common __sk_common;
    socket_lock_t sk_lock;
    atomic_t sk_drops;
    int sk_rcvlowat;
    struct sk_buff_head sk_error_queue;
    struct sk_buff *sk_rx_skb_cache;
    struct sk_buff_head sk_receive_queue;
    struct (anon) sk_backlog;
    int sk_forward_alloc;
    unsigned int sk_ll_usec;
    unsigned int sk_napi_id;
    int sk_rcvbuf;
    struct sk_filter *sk_filter;
    struct socket_wq *sk_wq;
    struct socket_wq *sk_wq_raw;
    struct xfrm_policy * sk_policy[2];
    struct dst_entry *sk_rx_dst;
    struct dst_entry *sk_dst_cache;
    atomic_t sk_omem_alloc;
    int sk_sndbuf;
    int sk_wmem_queued;
    refcount_t sk_wmem_alloc;
    long unsigned int sk_tsq_flags;
    struct sk_buff *sk_send_head;
    struct rb_root tcp_rtx_queue;
    struct sk_buff *sk_tx_skb_cache;
    struct sk_buff_head sk_write_queue;
    __s32 sk_peek_off;
    int sk_write_pending;
    __u32 sk_dst_pending_confirm;
    u32 sk_pacing_status;
    long int sk_sndtimeo;
    struct timer_list sk_timer;
    __u32 sk_priority;
    __u32 sk_mark;
    long unsigned int sk_pacing_rate;
    long unsigned int sk_max_pacing_rate;
    struct page_frag sk_frag;
    netdev_features_t sk_route_caps;
    netdev_features_t sk_route_nocaps;
    netdev_features_t sk_route_forced_caps;
    int sk_gso_type;
    unsigned int sk_gso_max_size;
    gfp_t sk_allocation;
    __u32 sk_txhash;
    unsigned int __sk_flags_offset[0];
    unsigned int sk_padding;
    unsigned int sk_kern_sock;
    unsigned int sk_no_check_tx;
    unsigned int sk_no_check_rx;
    unsigned int sk_userlocks;
    unsigned int sk_protocol;
    unsigned int sk_type;
    u16 sk_gso_max_segs;
    u8 sk_pacing_shift;
    long unsigned int sk_lingertime;
    struct proto *sk_prot_creator;
    rwlock_t sk_callback_lock;
    int sk_err;
    int sk_err_soft;
    u32 sk_ack_backlog;
    u32 sk_max_ack_backlog;
    kuid_t sk_uid;
    struct pid *sk_peer_pid;
    const struct cred *sk_peer_cred;
    long int sk_rcvtimeo;
    ktime_t sk_stamp;
    u16 sk_tsflags;
    u8 sk_shutdown;
    u32 sk_tskey;
    atomic_t sk_zckey;
    u8 sk_clockid;
    u8 sk_txtime_deadline_mode;
    u8 sk_txtime_report_errors;
    u8 sk_txtime_unused;
    struct socket *sk_socket;
    void *sk_user_data;
    void *sk_security;
    struct sock_cgroup_data sk_cgrp_data;
    struct mem_cgroup *sk_memcg;
    void (*sk_state_change)(struct sock *);
    void (*sk_data_ready)(struct sock *);
    void (*sk_write_space)(struct sock *);
    void (*sk_error_report)(struct sock *);
    int (*sk_backlog_rcv)(struct sock *, struct sk_buff *);
    struct sk_buff * (*sk_validate_xmit_skb)(struct sock *, struct net_device *, struct sk_buff *);
    void (*sk_destruct)(struct sock *);
    struct sock_reuseport *sk_reuseport_cb;
    struct bpf_sk_storage *sk_bpf_storage;
    struct callback_head sk_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct sock {
    struct sock_common __sk_common;
    socket_lock_t sk_lock;
    atomic_t sk_drops;
    int sk_rcvlowat;
    struct sk_buff_head sk_error_queue;
    struct sk_buff *sk_rx_skb_cache;
    struct sk_buff_head sk_receive_queue;
    struct (anon) sk_backlog;
    int sk_forward_alloc;
    unsigned int sk_ll_usec;
    unsigned int sk_napi_id;
    int sk_rcvbuf;
    struct sk_filter *sk_filter;
    struct socket_wq *sk_wq;
    struct socket_wq *sk_wq_raw;
    struct xfrm_policy * sk_policy[2];
    struct dst_entry *sk_rx_dst;
    struct dst_entry *sk_dst_cache;
    atomic_t sk_omem_alloc;
    int sk_sndbuf;
    int sk_wmem_queued;
    refcount_t sk_wmem_alloc;
    long unsigned int sk_tsq_flags;
    struct sk_buff *sk_send_head;
    struct rb_root tcp_rtx_queue;
    struct sk_buff *sk_tx_skb_cache;
    struct sk_buff_head sk_write_queue;
    __s32 sk_peek_off;
    int sk_write_pending;
    __u32 sk_dst_pending_confirm;
    u32 sk_pacing_status;
    long int sk_sndtimeo;
    struct timer_list sk_timer;
    __u32 sk_priority;
    __u32 sk_mark;
    long unsigned int sk_pacing_rate;
    long unsigned int sk_max_pacing_rate;
    struct page_frag sk_frag;
    netdev_features_t sk_route_caps;
    netdev_features_t sk_route_nocaps;
    netdev_features_t sk_route_forced_caps;
    int sk_gso_type;
    unsigned int sk_gso_max_size;
    gfp_t sk_allocation;
    __u32 sk_txhash;
    unsigned int __sk_flags_offset[0];
    unsigned int sk_padding;
    unsigned int sk_kern_sock;
    unsigned int sk_no_check_tx;
    unsigned int sk_no_check_rx;
    unsigned int sk_userlocks;
    unsigned int sk_protocol;
    unsigned int sk_type;
    u16 sk_gso_max_segs;
    u8 sk_pacing_shift;
    long unsigned int sk_lingertime;
    struct proto *sk_prot_creator;
    rwlock_t sk_callback_lock;
    int sk_err;
    int sk_err_soft;
    u32 sk_ack_backlog;
    u32 sk_max_ack_backlog;
    kuid_t sk_uid;
    struct pid *sk_peer_pid;
    const struct cred *sk_peer_cred;
    long int sk_rcvtimeo;
    ktime_t sk_stamp;
    u16 sk_tsflags;
    u8 sk_shutdown;
    u32 sk_tskey;
    atomic_t sk_zckey;
    u8 sk_clockid;
    u8 sk_txtime_deadline_mode;
    u8 sk_txtime_report_errors;
    u8 sk_txtime_unused;
    struct socket *sk_socket;
    void *sk_user_data;
    void *sk_security;
    struct sock_cgroup_data sk_cgrp_data;
    struct mem_cgroup *sk_memcg;
    void (*sk_state_change)(struct sock *);
    void (*sk_data_ready)(struct sock *);
    void (*sk_write_space)(struct sock *);
    void (*sk_error_report)(struct sock *);
    int (*sk_backlog_rcv)(struct sock *, struct sk_buff *);
    struct sk_buff * (*sk_validate_xmit_skb)(struct sock *, struct net_device *, struct sk_buff *);
    void (*sk_destruct)(struct sock *);
    struct sock_reuseport *sk_reuseport_cb;
    struct bpf_sk_storage *sk_bpf_storage;
    struct callback_head sk_rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct sock {
    struct sock_common __sk_common;
    socket_lock_t sk_lock;
    atomic_t sk_drops;
    int sk_rcvlowat;
    struct sk_buff_head sk_error_queue;
    struct sk_buff *sk_rx_skb_cache;
    struct sk_buff_head sk_receive_queue;
    struct (anon) sk_backlog;
    int sk_forward_alloc;
    unsigned int sk_ll_usec;
    unsigned int sk_napi_id;
    int sk_rcvbuf;
    struct sk_filter *sk_filter;
    struct socket_wq *sk_wq;
    struct socket_wq *sk_wq_raw;
    struct xfrm_policy * sk_policy[2];
    struct dst_entry *sk_rx_dst;
    struct dst_entry *sk_dst_cache;
    atomic_t sk_omem_alloc;
    int sk_sndbuf;
    int sk_wmem_queued;
    refcount_t sk_wmem_alloc;
    long unsigned int sk_tsq_flags;
    struct sk_buff *sk_send_head;
    struct rb_root tcp_rtx_queue;
    struct sk_buff *sk_tx_skb_cache;
    struct sk_buff_head sk_write_queue;
    __s32 sk_peek_off;
    int sk_write_pending;
    __u32 sk_dst_pending_confirm;
    u32 sk_pacing_status;
    long int sk_sndtimeo;
    struct timer_list sk_timer;
    __u32 sk_priority;
    __u32 sk_mark;
    long unsigned int sk_pacing_rate;
    long unsigned int sk_max_pacing_rate;
    struct page_frag sk_frag;
    netdev_features_t sk_route_caps;
    netdev_features_t sk_route_nocaps;
    netdev_features_t sk_route_forced_caps;
    int sk_gso_type;
    unsigned int sk_gso_max_size;
    gfp_t sk_allocation;
    __u32 sk_txhash;
    unsigned int __sk_flags_offset[0];
    unsigned int sk_padding;
    unsigned int sk_kern_sock;
    unsigned int sk_no_check_tx;
    unsigned int sk_no_check_rx;
    unsigned int sk_userlocks;
    unsigned int sk_protocol;
    unsigned int sk_type;
    u16 sk_gso_max_segs;
    u8 sk_pacing_shift;
    long unsigned int sk_lingertime;
    struct proto *sk_prot_creator;
    rwlock_t sk_callback_lock;
    int sk_err;
    int sk_err_soft;
    u32 sk_ack_backlog;
    u32 sk_max_ack_backlog;
    kuid_t sk_uid;
    struct pid *sk_peer_pid;
    const struct cred *sk_peer_cred;
    long int sk_rcvtimeo;
    ktime_t sk_stamp;
    u16 sk_tsflags;
    u8 sk_shutdown;
    u32 sk_tskey;
    atomic_t sk_zckey;
    u8 sk_clockid;
    u8 sk_txtime_deadline_mode;
    u8 sk_txtime_report_errors;
    u8 sk_txtime_unused;
    struct socket *sk_socket;
    void *sk_user_data;
    void *sk_security;
    struct sock_cgroup_data sk_cgrp_data;
    struct mem_cgroup *sk_memcg;
    void (*sk_state_change)(struct sock *);
    void (*sk_data_ready)(struct sock *);
    void (*sk_write_space)(struct sock *);
    void (*sk_error_report)(struct sock *);
    int (*sk_backlog_rcv)(struct sock *, struct sk_buff *);
    struct sk_buff * (*sk_validate_xmit_skb)(struct sock *, struct net_device *, struct sk_buff *);
    void (*sk_destruct)(struct sock *);
    struct sock_reuseport *sk_reuseport_cb;
    struct bpf_sk_storage *sk_bpf_storage;
    struct callback_head sk_rcu;
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
<b>Field added. </b>
<code>unsigned int sk_padding</code>
</li>
<li>
<b>Field added. </b>
<code>struct sock_cgroup_data sk_cgrp_data</code>
</li>
<li>
<b>Field added. </b>
<code>struct mem_cgroup *sk_memcg</code>
</li>
<li>
<b>Field added. </b>
<code>struct sock_reuseport *sk_reuseport_cb</code>
</li>
<li>
<b>Field added. </b>
<code>struct callback_head sk_rcu</code>
</li>
<li>
<b>Field removed. </b>
<code>__u32 sk_cgrp_prioidx</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 sk_classid</code>
</li>
<li>
<b>Field removed. </b>
<code>struct cg_proto *sk_cgrp</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int sk_shutdown</code> ➡️ <code>u8 sk_shutdown</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int sk_tsq_flags</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int __sk_flags_offset[0]</code>
</li>
<li>
<b>Field added. </b>
<code>kuid_t sk_uid</code>
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
<code>__u32 sk_dst_pending_confirm</code>
</li>
<li>
<b>Field added. </b>
<code>u32 sk_pacing_status</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int sk_kern_sock</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_t sk_wmem_alloc</code> ➡️ <code>refcount_t sk_wmem_alloc</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct rb_root tcp_rtx_queue</code>
</li>
<li>
<b>Field added. </b>
<code>u8 sk_pacing_shift</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t sk_zckey</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>netdev_features_t sk_route_forced_caps</code>
</li>
<li>
<b>Field added. </b>
<code>struct sk_buff * (*sk_validate_xmit_skb)(struct sock *, struct net_device *, struct sk_buff *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 sk_clockid</code>
</li>
<li>
<b>Field added. </b>
<code>u8 sk_txtime_deadline_mode</code>
</li>
<li>
<b>Field added. </b>
<code>u8 sk_txtime_report_errors</code>
</li>
<li>
<b>Field added. </b>
<code>u8 sk_txtime_unused</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 sk_pacing_rate</code> ➡️ <code>long unsigned int sk_pacing_rate</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 sk_max_pacing_rate</code> ➡️ <code>long unsigned int sk_max_pacing_rate</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct sk_buff *sk_rx_skb_cache</code>
</li>
<li>
<b>Field added. </b>
<code>struct sk_buff *sk_tx_skb_cache</code>
</li>
<li>
<b>Field added. </b>
<code>struct bpf_sk_storage *sk_bpf_storage</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned int __sk_flags_offset[0]</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int sk_padding</code> ➡️ <code>u8 sk_padding</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int sk_kern_sock</code> ➡️ <code>u8 sk_kern_sock</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int sk_no_check_tx</code> ➡️ <code>u8 sk_no_check_tx</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int sk_no_check_rx</code> ➡️ <code>u8 sk_no_check_rx</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int sk_userlocks</code> ➡️ <code>u8 sk_userlocks</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int sk_protocol</code> ➡️ <code>u16 sk_protocol</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int sk_type</code> ➡️ <code>u16 sk_type</code>
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
<code>u8 sk_prefer_busy_poll</code>
</li>
<li>
<b>Field added. </b>
<code>u16 sk_busy_poll_budget</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct bpf_sk_storage *sk_bpf_storage</code> ➡️ <code>struct bpf_local_storage *sk_bpf_storage</code>
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
<code>int sk_rx_dst_ifindex</code>
</li>
<li>
<b>Field added. </b>
<code>u32 sk_rx_dst_cookie</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t sk_peer_lock</code>
</li>
<li>
<b>Field added. </b>
<code>int sk_bind_phc</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 sk_tskey</code> ➡️ <code>atomic_t sk_tskey</code>
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
<code>u32 sk_reserved_mem</code>
</li>
<li>
<b>Field added. </b>
<code>u8 sk_gso_disabled</code>
</li>
<li>
<b>Field added. </b>
<code>u8 sk_txrehash</code>
</li>
<li>
<b>Field added. </b>
<code>netns_tracker ns_tracker</code>
</li>
<li>
<b>Field removed. </b>
<code>struct sk_buff *sk_rx_skb_cache</code>
</li>
<li>
<b>Field removed. </b>
<code>struct sk_buff *sk_tx_skb_cache</code>
</li>
<li>
<b>Field removed. </b>
<code>netdev_features_t sk_route_nocaps</code>
</li>
<li>
<b>Field removed. </b>
<code>netdev_features_t sk_route_forced_caps</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 sk_padding</code>
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
<code>bool sk_use_task_frag</code>
</li>
<li>
<b>Field added. </b>
<code>struct hlist_node sk_bind2_node</code>
</li>
<li>
<b>Field type changed. </b>
<code>u16 sk_tsflags</code> ➡️ <code>u32 sk_tsflags</code>
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
<code>int sk_wait_pending</code>
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
<code>int sk_disconnects</code>
</li>
<li>
<b>Field removed. </b>
<code>int sk_wait_pending</code>
</li>
<li>
<b>Field removed. </b>
<code>struct hlist_node sk_bind2_node</code>
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
<b>Field added. </b>
<code>seqlock_t sk_stamp_seq</code>
</li>
</ul>
</details>
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
