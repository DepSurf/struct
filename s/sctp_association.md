# Struct: <code>sctp_association</code>

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
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct sctp_association {
    struct sctp_ep_common base;
    struct list_head asocs;
    sctp_assoc_t assoc_id;
    struct sctp_endpoint *ep;
    struct sctp_cookie c;
    struct (anon) peer;
    enum sctp_state state;
    int overall_error_count;
    ktime_t cookie_life;
    long unsigned int rto_initial;
    long unsigned int rto_max;
    long unsigned int rto_min;
    int max_burst;
    int max_retrans;
    int pf_retrans;
    __u16 max_init_attempts;
    __u16 init_retries;
    long unsigned int max_init_timeo;
    long unsigned int hbinterval;
    __u16 pathmaxrxt;
    __u8 pmtu_pending;
    __u32 pathmtu;
    __u32 param_flags;
    __u32 sackfreq;
    long unsigned int sackdelay;
    long unsigned int timeouts[11];
    struct timer_list timers[11];
    struct sctp_transport *shutdown_last_sent_to;
    struct sctp_transport *init_last_sent_to;
    int shutdown_retries;
    __u32 next_tsn;
    __u32 ctsn_ack_point;
    __u32 adv_peer_ack_point;
    __u32 highest_sacked;
    __u32 fast_recovery_exit;
    __u8 fast_recovery;
    __u16 unack_data;
    __u32 rtx_data_chunks;
    __u32 rwnd;
    __u32 a_rwnd;
    __u32 rwnd_over;
    __u32 rwnd_press;
    int sndbuf_used;
    atomic_t rmem_alloc;
    wait_queue_head_t wait;
    __u32 frag_point;
    __u32 user_frag;
    int init_err_counter;
    int init_cycle;
    __u16 default_stream;
    __u16 default_flags;
    __u32 default_ppid;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    struct sctp_stream stream;
    struct sctp_outq outqueue;
    struct sctp_ulpq ulpq;
    __u32 last_ecne_tsn;
    __u32 last_cwr_tsn;
    int numduptsns;
    struct sctp_chunk *addip_last_asconf;
    struct list_head asconf_ack_list;
    struct list_head addip_chunk_list;
    __u32 addip_serial;
    int src_out_of_asoc_ok;
    union sctp_addr *asconf_addr_del_pending;
    struct sctp_transport *new_transport;
    struct list_head endpoint_shared_keys;
    struct sctp_auth_bytes *asoc_shared_key;
    struct sctp_shared_key *shkey;
    __u16 default_hmac_id;
    __u16 active_key_id;
    __u8 need_ecne;
    __u8 temp;
    __u8 force_delay;
    __u8 intl_enable;
    __u8 prsctp_enable;
    __u8 reconf_enable;
    __u8 strreset_enable;
    __u8 strreset_outstanding;
    __u32 strreset_outseq;
    __u32 strreset_inseq;
    __u32 strreset_result[2];
    struct sctp_chunk *strreset_chunk;
    struct sctp_priv_assoc_stats stats;
    int sent_cnt_removable;
    __u64 abandoned_unsent[3];
    __u64 abandoned_sent[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct sctp_association {
    struct sctp_ep_common base;
    struct list_head asocs;
    sctp_assoc_t assoc_id;
    struct sctp_endpoint *ep;
    struct sctp_cookie c;
    struct (anon) peer;
    enum sctp_state state;
    int overall_error_count;
    ktime_t cookie_life;
    long unsigned int rto_initial;
    long unsigned int rto_max;
    long unsigned int rto_min;
    int max_burst;
    int max_retrans;
    int pf_retrans;
    __u16 max_init_attempts;
    __u16 init_retries;
    long unsigned int max_init_timeo;
    long unsigned int hbinterval;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u8 pmtu_pending;
    __u32 pathmtu;
    __u32 param_flags;
    __u32 sackfreq;
    long unsigned int sackdelay;
    long unsigned int timeouts[11];
    struct timer_list timers[11];
    struct sctp_transport *shutdown_last_sent_to;
    struct sctp_transport *init_last_sent_to;
    int shutdown_retries;
    __u32 next_tsn;
    __u32 ctsn_ack_point;
    __u32 adv_peer_ack_point;
    __u32 highest_sacked;
    __u32 fast_recovery_exit;
    __u8 fast_recovery;
    __u16 unack_data;
    __u32 rtx_data_chunks;
    __u32 rwnd;
    __u32 a_rwnd;
    __u32 rwnd_over;
    __u32 rwnd_press;
    int sndbuf_used;
    atomic_t rmem_alloc;
    wait_queue_head_t wait;
    __u32 frag_point;
    __u32 user_frag;
    int init_err_counter;
    int init_cycle;
    __u16 default_stream;
    __u16 default_flags;
    __u32 default_ppid;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    struct sctp_stream stream;
    struct sctp_outq outqueue;
    struct sctp_ulpq ulpq;
    __u32 last_ecne_tsn;
    __u32 last_cwr_tsn;
    int numduptsns;
    struct sctp_chunk *addip_last_asconf;
    struct list_head asconf_ack_list;
    struct list_head addip_chunk_list;
    __u32 addip_serial;
    int src_out_of_asoc_ok;
    union sctp_addr *asconf_addr_del_pending;
    struct sctp_transport *new_transport;
    struct list_head endpoint_shared_keys;
    struct sctp_auth_bytes *asoc_shared_key;
    struct sctp_shared_key *shkey;
    __u16 default_hmac_id;
    __u16 active_key_id;
    __u8 need_ecne;
    __u8 temp;
    __u8 force_delay;
    __u8 intl_enable;
    __u8 prsctp_enable;
    __u8 reconf_enable;
    __u8 strreset_enable;
    __u8 strreset_outstanding;
    __u32 strreset_outseq;
    __u32 strreset_inseq;
    __u32 strreset_result[2];
    struct sctp_chunk *strreset_chunk;
    struct sctp_priv_assoc_stats stats;
    int sent_cnt_removable;
    __u16 subscribe;
    __u64 abandoned_unsent[3];
    __u64 abandoned_sent[3];
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct sctp_association {
    struct sctp_ep_common base;
    struct list_head asocs;
    sctp_assoc_t assoc_id;
    struct sctp_endpoint *ep;
    struct sctp_cookie c;
    struct (anon) peer;
    enum sctp_state state;
    int overall_error_count;
    ktime_t cookie_life;
    long unsigned int rto_initial;
    long unsigned int rto_max;
    long unsigned int rto_min;
    int max_burst;
    int max_retrans;
    int pf_retrans;
    __u16 max_init_attempts;
    __u16 init_retries;
    long unsigned int max_init_timeo;
    long unsigned int hbinterval;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u8 pmtu_pending;
    __u32 pathmtu;
    __u32 param_flags;
    __u32 sackfreq;
    long unsigned int sackdelay;
    long unsigned int timeouts[11];
    struct timer_list timers[11];
    struct sctp_transport *shutdown_last_sent_to;
    struct sctp_transport *init_last_sent_to;
    int shutdown_retries;
    __u32 next_tsn;
    __u32 ctsn_ack_point;
    __u32 adv_peer_ack_point;
    __u32 highest_sacked;
    __u32 fast_recovery_exit;
    __u8 fast_recovery;
    __u16 unack_data;
    __u32 rtx_data_chunks;
    __u32 rwnd;
    __u32 a_rwnd;
    __u32 rwnd_over;
    __u32 rwnd_press;
    int sndbuf_used;
    atomic_t rmem_alloc;
    wait_queue_head_t wait;
    __u32 frag_point;
    __u32 user_frag;
    int init_err_counter;
    int init_cycle;
    __u16 default_stream;
    __u16 default_flags;
    __u32 default_ppid;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    struct sctp_stream stream;
    struct sctp_outq outqueue;
    struct sctp_ulpq ulpq;
    __u32 last_ecne_tsn;
    __u32 last_cwr_tsn;
    int numduptsns;
    struct sctp_chunk *addip_last_asconf;
    struct list_head asconf_ack_list;
    struct list_head addip_chunk_list;
    __u32 addip_serial;
    int src_out_of_asoc_ok;
    union sctp_addr *asconf_addr_del_pending;
    struct sctp_transport *new_transport;
    struct list_head endpoint_shared_keys;
    struct sctp_auth_bytes *asoc_shared_key;
    struct sctp_shared_key *shkey;
    __u16 default_hmac_id;
    __u16 active_key_id;
    __u8 need_ecne;
    __u8 temp;
    __u8 force_delay;
    __u8 strreset_enable;
    __u8 strreset_outstanding;
    __u32 strreset_outseq;
    __u32 strreset_inseq;
    __u32 strreset_result[2];
    struct sctp_chunk *strreset_chunk;
    struct sctp_priv_assoc_stats stats;
    int sent_cnt_removable;
    __u16 subscribe;
    __u64 abandoned_unsent[3];
    __u64 abandoned_sent[3];
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct sctp_association {
    struct sctp_ep_common base;
    struct list_head asocs;
    sctp_assoc_t assoc_id;
    struct sctp_endpoint *ep;
    struct sctp_cookie c;
    struct (anon) peer;
    enum sctp_state state;
    int overall_error_count;
    ktime_t cookie_life;
    long unsigned int rto_initial;
    long unsigned int rto_max;
    long unsigned int rto_min;
    int max_burst;
    int max_retrans;
    int pf_retrans;
    __u16 max_init_attempts;
    __u16 init_retries;
    long unsigned int max_init_timeo;
    long unsigned int hbinterval;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u8 pmtu_pending;
    __u32 pathmtu;
    __u32 param_flags;
    __u32 sackfreq;
    long unsigned int sackdelay;
    long unsigned int timeouts[11];
    struct timer_list timers[11];
    struct sctp_transport *shutdown_last_sent_to;
    struct sctp_transport *init_last_sent_to;
    int shutdown_retries;
    __u32 next_tsn;
    __u32 ctsn_ack_point;
    __u32 adv_peer_ack_point;
    __u32 highest_sacked;
    __u32 fast_recovery_exit;
    __u8 fast_recovery;
    __u16 unack_data;
    __u32 rtx_data_chunks;
    __u32 rwnd;
    __u32 a_rwnd;
    __u32 rwnd_over;
    __u32 rwnd_press;
    int sndbuf_used;
    atomic_t rmem_alloc;
    wait_queue_head_t wait;
    __u32 frag_point;
    __u32 user_frag;
    int init_err_counter;
    int init_cycle;
    __u16 default_stream;
    __u16 default_flags;
    __u32 default_ppid;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    struct sctp_stream stream;
    struct sctp_outq outqueue;
    struct sctp_ulpq ulpq;
    __u32 last_ecne_tsn;
    __u32 last_cwr_tsn;
    int numduptsns;
    struct sctp_chunk *addip_last_asconf;
    struct list_head asconf_ack_list;
    struct list_head addip_chunk_list;
    __u32 addip_serial;
    int src_out_of_asoc_ok;
    union sctp_addr *asconf_addr_del_pending;
    struct sctp_transport *new_transport;
    struct list_head endpoint_shared_keys;
    struct sctp_auth_bytes *asoc_shared_key;
    struct sctp_shared_key *shkey;
    __u16 default_hmac_id;
    __u16 active_key_id;
    __u8 need_ecne;
    __u8 temp;
    __u8 force_delay;
    __u8 strreset_enable;
    __u8 strreset_outstanding;
    __u32 strreset_outseq;
    __u32 strreset_inseq;
    __u32 strreset_result[2];
    struct sctp_chunk *strreset_chunk;
    struct sctp_priv_assoc_stats stats;
    int sent_cnt_removable;
    __u16 subscribe;
    __u64 abandoned_unsent[3];
    __u64 abandoned_sent[3];
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct sctp_association {
    struct sctp_ep_common base;
    struct list_head asocs;
    sctp_assoc_t assoc_id;
    struct sctp_endpoint *ep;
    struct sctp_cookie c;
    struct (anon) peer;
    enum sctp_state state;
    int overall_error_count;
    ktime_t cookie_life;
    long unsigned int rto_initial;
    long unsigned int rto_max;
    long unsigned int rto_min;
    int max_burst;
    int max_retrans;
    __u16 pf_retrans;
    __u16 ps_retrans;
    __u16 max_init_attempts;
    __u16 init_retries;
    long unsigned int max_init_timeo;
    long unsigned int hbinterval;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u8 pmtu_pending;
    __u32 pathmtu;
    __u32 param_flags;
    __u32 sackfreq;
    long unsigned int sackdelay;
    long unsigned int timeouts[11];
    struct timer_list timers[11];
    struct sctp_transport *shutdown_last_sent_to;
    struct sctp_transport *init_last_sent_to;
    int shutdown_retries;
    __u32 next_tsn;
    __u32 ctsn_ack_point;
    __u32 adv_peer_ack_point;
    __u32 highest_sacked;
    __u32 fast_recovery_exit;
    __u8 fast_recovery;
    __u16 unack_data;
    __u32 rtx_data_chunks;
    __u32 rwnd;
    __u32 a_rwnd;
    __u32 rwnd_over;
    __u32 rwnd_press;
    int sndbuf_used;
    atomic_t rmem_alloc;
    wait_queue_head_t wait;
    __u32 frag_point;
    __u32 user_frag;
    int init_err_counter;
    int init_cycle;
    __u16 default_stream;
    __u16 default_flags;
    __u32 default_ppid;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    struct sctp_stream stream;
    struct sctp_outq outqueue;
    struct sctp_ulpq ulpq;
    __u32 last_ecne_tsn;
    __u32 last_cwr_tsn;
    int numduptsns;
    struct sctp_chunk *addip_last_asconf;
    struct list_head asconf_ack_list;
    struct list_head addip_chunk_list;
    __u32 addip_serial;
    int src_out_of_asoc_ok;
    union sctp_addr *asconf_addr_del_pending;
    struct sctp_transport *new_transport;
    struct list_head endpoint_shared_keys;
    struct sctp_auth_bytes *asoc_shared_key;
    struct sctp_shared_key *shkey;
    __u16 default_hmac_id;
    __u16 active_key_id;
    __u8 need_ecne;
    __u8 temp;
    __u8 pf_expose;
    __u8 force_delay;
    __u8 strreset_enable;
    __u8 strreset_outstanding;
    __u32 strreset_outseq;
    __u32 strreset_inseq;
    __u32 strreset_result[2];
    struct sctp_chunk *strreset_chunk;
    struct sctp_priv_assoc_stats stats;
    int sent_cnt_removable;
    __u16 subscribe;
    __u64 abandoned_unsent[3];
    __u64 abandoned_sent[3];
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct sctp_association {
    struct sctp_ep_common base;
    struct list_head asocs;
    sctp_assoc_t assoc_id;
    struct sctp_endpoint *ep;
    struct sctp_cookie c;
    struct (anon) peer;
    enum sctp_state state;
    int overall_error_count;
    ktime_t cookie_life;
    long unsigned int rto_initial;
    long unsigned int rto_max;
    long unsigned int rto_min;
    int max_burst;
    int max_retrans;
    __u16 pf_retrans;
    __u16 ps_retrans;
    __u16 max_init_attempts;
    __u16 init_retries;
    long unsigned int max_init_timeo;
    long unsigned int hbinterval;
    __be16 encap_port;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u8 pmtu_pending;
    __u32 pathmtu;
    __u32 param_flags;
    __u32 sackfreq;
    long unsigned int sackdelay;
    long unsigned int timeouts[11];
    struct timer_list timers[11];
    struct sctp_transport *shutdown_last_sent_to;
    struct sctp_transport *init_last_sent_to;
    int shutdown_retries;
    __u32 next_tsn;
    __u32 ctsn_ack_point;
    __u32 adv_peer_ack_point;
    __u32 highest_sacked;
    __u32 fast_recovery_exit;
    __u8 fast_recovery;
    __u16 unack_data;
    __u32 rtx_data_chunks;
    __u32 rwnd;
    __u32 a_rwnd;
    __u32 rwnd_over;
    __u32 rwnd_press;
    int sndbuf_used;
    atomic_t rmem_alloc;
    wait_queue_head_t wait;
    __u32 frag_point;
    __u32 user_frag;
    int init_err_counter;
    int init_cycle;
    __u16 default_stream;
    __u16 default_flags;
    __u32 default_ppid;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    struct sctp_stream stream;
    struct sctp_outq outqueue;
    struct sctp_ulpq ulpq;
    __u32 last_ecne_tsn;
    __u32 last_cwr_tsn;
    int numduptsns;
    struct sctp_chunk *addip_last_asconf;
    struct list_head asconf_ack_list;
    struct list_head addip_chunk_list;
    __u32 addip_serial;
    int src_out_of_asoc_ok;
    union sctp_addr *asconf_addr_del_pending;
    struct sctp_transport *new_transport;
    struct list_head endpoint_shared_keys;
    struct sctp_auth_bytes *asoc_shared_key;
    struct sctp_shared_key *shkey;
    __u16 default_hmac_id;
    __u16 active_key_id;
    __u8 need_ecne;
    __u8 temp;
    __u8 pf_expose;
    __u8 force_delay;
    __u8 strreset_enable;
    __u8 strreset_outstanding;
    __u32 strreset_outseq;
    __u32 strreset_inseq;
    __u32 strreset_result[2];
    struct sctp_chunk *strreset_chunk;
    struct sctp_priv_assoc_stats stats;
    int sent_cnt_removable;
    __u16 subscribe;
    __u64 abandoned_unsent[3];
    __u64 abandoned_sent[3];
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct sctp_association {
    struct sctp_ep_common base;
    struct list_head asocs;
    sctp_assoc_t assoc_id;
    struct sctp_endpoint *ep;
    struct sctp_cookie c;
    struct (anon) peer;
    enum sctp_state state;
    int overall_error_count;
    ktime_t cookie_life;
    long unsigned int rto_initial;
    long unsigned int rto_max;
    long unsigned int rto_min;
    int max_burst;
    int max_retrans;
    __u16 pf_retrans;
    __u16 ps_retrans;
    __u16 max_init_attempts;
    __u16 init_retries;
    long unsigned int max_init_timeo;
    long unsigned int hbinterval;
    __be16 encap_port;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u8 pmtu_pending;
    __u32 pathmtu;
    __u32 param_flags;
    __u32 sackfreq;
    long unsigned int sackdelay;
    long unsigned int timeouts[11];
    struct timer_list timers[11];
    struct sctp_transport *shutdown_last_sent_to;
    struct sctp_transport *init_last_sent_to;
    int shutdown_retries;
    __u32 next_tsn;
    __u32 ctsn_ack_point;
    __u32 adv_peer_ack_point;
    __u32 highest_sacked;
    __u32 fast_recovery_exit;
    __u8 fast_recovery;
    __u16 unack_data;
    __u32 rtx_data_chunks;
    __u32 rwnd;
    __u32 a_rwnd;
    __u32 rwnd_over;
    __u32 rwnd_press;
    int sndbuf_used;
    atomic_t rmem_alloc;
    wait_queue_head_t wait;
    __u32 frag_point;
    __u32 user_frag;
    int init_err_counter;
    int init_cycle;
    __u16 default_stream;
    __u16 default_flags;
    __u32 default_ppid;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    struct sctp_stream stream;
    struct sctp_outq outqueue;
    struct sctp_ulpq ulpq;
    __u32 last_ecne_tsn;
    __u32 last_cwr_tsn;
    int numduptsns;
    struct sctp_chunk *addip_last_asconf;
    struct list_head asconf_ack_list;
    struct list_head addip_chunk_list;
    __u32 addip_serial;
    int src_out_of_asoc_ok;
    union sctp_addr *asconf_addr_del_pending;
    struct sctp_transport *new_transport;
    struct list_head endpoint_shared_keys;
    struct sctp_auth_bytes *asoc_shared_key;
    struct sctp_shared_key *shkey;
    __u16 default_hmac_id;
    __u16 active_key_id;
    __u8 need_ecne;
    __u8 temp;
    __u8 pf_expose;
    __u8 force_delay;
    __u8 strreset_enable;
    __u8 strreset_outstanding;
    __u32 strreset_outseq;
    __u32 strreset_inseq;
    __u32 strreset_result[2];
    struct sctp_chunk *strreset_chunk;
    struct sctp_priv_assoc_stats stats;
    int sent_cnt_removable;
    __u16 subscribe;
    __u64 abandoned_unsent[3];
    __u64 abandoned_sent[3];
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct sctp_association {
    struct sctp_ep_common base;
    struct list_head asocs;
    sctp_assoc_t assoc_id;
    struct sctp_endpoint *ep;
    struct sctp_cookie c;
    struct (anon) peer;
    enum sctp_state state;
    int overall_error_count;
    ktime_t cookie_life;
    long unsigned int rto_initial;
    long unsigned int rto_max;
    long unsigned int rto_min;
    int max_burst;
    int max_retrans;
    __u16 pf_retrans;
    __u16 ps_retrans;
    __u16 max_init_attempts;
    __u16 init_retries;
    long unsigned int max_init_timeo;
    long unsigned int hbinterval;
    long unsigned int probe_interval;
    __be16 encap_port;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u8 pmtu_pending;
    __u32 pathmtu;
    __u32 param_flags;
    __u32 sackfreq;
    long unsigned int sackdelay;
    long unsigned int timeouts[12];
    struct timer_list timers[12];
    struct sctp_transport *shutdown_last_sent_to;
    struct sctp_transport *init_last_sent_to;
    int shutdown_retries;
    __u32 next_tsn;
    __u32 ctsn_ack_point;
    __u32 adv_peer_ack_point;
    __u32 highest_sacked;
    __u32 fast_recovery_exit;
    __u8 fast_recovery;
    __u16 unack_data;
    __u32 rtx_data_chunks;
    __u32 rwnd;
    __u32 a_rwnd;
    __u32 rwnd_over;
    __u32 rwnd_press;
    int sndbuf_used;
    atomic_t rmem_alloc;
    wait_queue_head_t wait;
    __u32 frag_point;
    __u32 user_frag;
    int init_err_counter;
    int init_cycle;
    __u16 default_stream;
    __u16 default_flags;
    __u32 default_ppid;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    struct sctp_stream stream;
    struct sctp_outq outqueue;
    struct sctp_ulpq ulpq;
    __u32 last_ecne_tsn;
    __u32 last_cwr_tsn;
    int numduptsns;
    struct sctp_chunk *addip_last_asconf;
    struct list_head asconf_ack_list;
    struct list_head addip_chunk_list;
    __u32 addip_serial;
    int src_out_of_asoc_ok;
    union sctp_addr *asconf_addr_del_pending;
    struct sctp_transport *new_transport;
    struct list_head endpoint_shared_keys;
    struct sctp_auth_bytes *asoc_shared_key;
    struct sctp_shared_key *shkey;
    __u16 default_hmac_id;
    __u16 active_key_id;
    __u8 need_ecne;
    __u8 temp;
    __u8 pf_expose;
    __u8 force_delay;
    __u8 strreset_enable;
    __u8 strreset_outstanding;
    __u32 strreset_outseq;
    __u32 strreset_inseq;
    __u32 strreset_result[2];
    struct sctp_chunk *strreset_chunk;
    struct sctp_priv_assoc_stats stats;
    int sent_cnt_removable;
    __u16 subscribe;
    __u64 abandoned_unsent[3];
    __u64 abandoned_sent[3];
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct sctp_association {
    struct sctp_ep_common base;
    struct list_head asocs;
    sctp_assoc_t assoc_id;
    struct sctp_endpoint *ep;
    struct sctp_cookie c;
    struct (anon) peer;
    enum sctp_state state;
    int overall_error_count;
    ktime_t cookie_life;
    long unsigned int rto_initial;
    long unsigned int rto_max;
    long unsigned int rto_min;
    int max_burst;
    int max_retrans;
    __u16 pf_retrans;
    __u16 ps_retrans;
    __u16 max_init_attempts;
    __u16 init_retries;
    long unsigned int max_init_timeo;
    long unsigned int hbinterval;
    long unsigned int probe_interval;
    __be16 encap_port;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u8 pmtu_pending;
    __u32 pathmtu;
    __u32 param_flags;
    __u32 sackfreq;
    long unsigned int sackdelay;
    long unsigned int timeouts[12];
    struct timer_list timers[12];
    struct sctp_transport *shutdown_last_sent_to;
    struct sctp_transport *init_last_sent_to;
    int shutdown_retries;
    __u32 next_tsn;
    __u32 ctsn_ack_point;
    __u32 adv_peer_ack_point;
    __u32 highest_sacked;
    __u32 fast_recovery_exit;
    __u8 fast_recovery;
    __u16 unack_data;
    __u32 rtx_data_chunks;
    __u32 rwnd;
    __u32 a_rwnd;
    __u32 rwnd_over;
    __u32 rwnd_press;
    int sndbuf_used;
    atomic_t rmem_alloc;
    wait_queue_head_t wait;
    __u32 frag_point;
    __u32 user_frag;
    int init_err_counter;
    int init_cycle;
    __u16 default_stream;
    __u16 default_flags;
    __u32 default_ppid;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    struct sctp_stream stream;
    struct sctp_outq outqueue;
    struct sctp_ulpq ulpq;
    __u32 last_ecne_tsn;
    __u32 last_cwr_tsn;
    int numduptsns;
    struct sctp_chunk *addip_last_asconf;
    struct list_head asconf_ack_list;
    struct list_head addip_chunk_list;
    __u32 addip_serial;
    int src_out_of_asoc_ok;
    union sctp_addr *asconf_addr_del_pending;
    struct sctp_transport *new_transport;
    struct list_head endpoint_shared_keys;
    struct sctp_auth_bytes *asoc_shared_key;
    struct sctp_shared_key *shkey;
    __u16 default_hmac_id;
    __u16 active_key_id;
    __u8 need_ecne;
    __u8 temp;
    __u8 pf_expose;
    __u8 force_delay;
    __u8 strreset_enable;
    __u8 strreset_outstanding;
    __u32 strreset_outseq;
    __u32 strreset_inseq;
    __u32 strreset_result[2];
    struct sctp_chunk *strreset_chunk;
    struct sctp_priv_assoc_stats stats;
    int sent_cnt_removable;
    __u16 subscribe;
    __u64 abandoned_unsent[3];
    __u64 abandoned_sent[3];
    u32 secid;
    u32 peer_secid;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct sctp_association {
    struct sctp_ep_common base;
    struct list_head asocs;
    sctp_assoc_t assoc_id;
    struct sctp_endpoint *ep;
    struct sctp_cookie c;
    struct (anon) peer;
    enum sctp_state state;
    int overall_error_count;
    ktime_t cookie_life;
    long unsigned int rto_initial;
    long unsigned int rto_max;
    long unsigned int rto_min;
    int max_burst;
    int max_retrans;
    __u16 pf_retrans;
    __u16 ps_retrans;
    __u16 max_init_attempts;
    __u16 init_retries;
    long unsigned int max_init_timeo;
    long unsigned int hbinterval;
    long unsigned int probe_interval;
    __be16 encap_port;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u8 pmtu_pending;
    __u32 pathmtu;
    __u32 param_flags;
    __u32 sackfreq;
    long unsigned int sackdelay;
    long unsigned int timeouts[12];
    struct timer_list timers[12];
    struct sctp_transport *shutdown_last_sent_to;
    struct sctp_transport *init_last_sent_to;
    int shutdown_retries;
    __u32 next_tsn;
    __u32 ctsn_ack_point;
    __u32 adv_peer_ack_point;
    __u32 highest_sacked;
    __u32 fast_recovery_exit;
    __u8 fast_recovery;
    __u16 unack_data;
    __u32 rtx_data_chunks;
    __u32 rwnd;
    __u32 a_rwnd;
    __u32 rwnd_over;
    __u32 rwnd_press;
    int sndbuf_used;
    atomic_t rmem_alloc;
    wait_queue_head_t wait;
    __u32 frag_point;
    __u32 user_frag;
    int init_err_counter;
    int init_cycle;
    __u16 default_stream;
    __u16 default_flags;
    __u32 default_ppid;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    struct sctp_stream stream;
    struct sctp_outq outqueue;
    struct sctp_ulpq ulpq;
    __u32 last_ecne_tsn;
    __u32 last_cwr_tsn;
    int numduptsns;
    struct sctp_chunk *addip_last_asconf;
    struct list_head asconf_ack_list;
    struct list_head addip_chunk_list;
    __u32 addip_serial;
    int src_out_of_asoc_ok;
    union sctp_addr *asconf_addr_del_pending;
    struct sctp_transport *new_transport;
    struct list_head endpoint_shared_keys;
    struct sctp_auth_bytes *asoc_shared_key;
    struct sctp_shared_key *shkey;
    __u16 default_hmac_id;
    __u16 active_key_id;
    __u8 need_ecne;
    __u8 temp;
    __u8 pf_expose;
    __u8 force_delay;
    __u8 strreset_enable;
    __u8 strreset_outstanding;
    __u32 strreset_outseq;
    __u32 strreset_inseq;
    __u32 strreset_result[2];
    struct sctp_chunk *strreset_chunk;
    struct sctp_priv_assoc_stats stats;
    int sent_cnt_removable;
    __u16 subscribe;
    __u64 abandoned_unsent[3];
    __u64 abandoned_sent[3];
    u32 secid;
    u32 peer_secid;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct sctp_association {
    struct sctp_ep_common base;
    struct list_head asocs;
    sctp_assoc_t assoc_id;
    struct sctp_endpoint *ep;
    struct sctp_cookie c;
    struct (anon) peer;
    enum sctp_state state;
    int overall_error_count;
    ktime_t cookie_life;
    long unsigned int rto_initial;
    long unsigned int rto_max;
    long unsigned int rto_min;
    int max_burst;
    int max_retrans;
    __u16 pf_retrans;
    __u16 ps_retrans;
    __u16 max_init_attempts;
    __u16 init_retries;
    long unsigned int max_init_timeo;
    long unsigned int hbinterval;
    long unsigned int probe_interval;
    __be16 encap_port;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u8 pmtu_pending;
    __u32 pathmtu;
    __u32 param_flags;
    __u32 sackfreq;
    long unsigned int sackdelay;
    long unsigned int timeouts[12];
    struct timer_list timers[12];
    struct sctp_transport *shutdown_last_sent_to;
    struct sctp_transport *init_last_sent_to;
    int shutdown_retries;
    __u32 next_tsn;
    __u32 ctsn_ack_point;
    __u32 adv_peer_ack_point;
    __u32 highest_sacked;
    __u32 fast_recovery_exit;
    __u8 fast_recovery;
    __u16 unack_data;
    __u32 rtx_data_chunks;
    __u32 rwnd;
    __u32 a_rwnd;
    __u32 rwnd_over;
    __u32 rwnd_press;
    int sndbuf_used;
    atomic_t rmem_alloc;
    wait_queue_head_t wait;
    __u32 frag_point;
    __u32 user_frag;
    int init_err_counter;
    int init_cycle;
    __u16 default_stream;
    __u16 default_flags;
    __u32 default_ppid;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    struct sctp_stream stream;
    struct sctp_outq outqueue;
    struct sctp_ulpq ulpq;
    __u32 last_ecne_tsn;
    __u32 last_cwr_tsn;
    int numduptsns;
    struct sctp_chunk *addip_last_asconf;
    struct list_head asconf_ack_list;
    struct list_head addip_chunk_list;
    __u32 addip_serial;
    int src_out_of_asoc_ok;
    union sctp_addr *asconf_addr_del_pending;
    struct sctp_transport *new_transport;
    struct list_head endpoint_shared_keys;
    struct sctp_auth_bytes *asoc_shared_key;
    struct sctp_shared_key *shkey;
    __u16 default_hmac_id;
    __u16 active_key_id;
    __u8 need_ecne;
    __u8 temp;
    __u8 pf_expose;
    __u8 force_delay;
    __u8 strreset_enable;
    __u8 strreset_outstanding;
    __u32 strreset_outseq;
    __u32 strreset_inseq;
    __u32 strreset_result[2];
    struct sctp_chunk *strreset_chunk;
    struct sctp_priv_assoc_stats stats;
    int sent_cnt_removable;
    __u16 subscribe;
    __u64 abandoned_unsent[3];
    __u64 abandoned_sent[3];
    u32 secid;
    u32 peer_secid;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct sctp_association {
    struct sctp_ep_common base;
    struct list_head asocs;
    sctp_assoc_t assoc_id;
    struct sctp_endpoint *ep;
    struct sctp_cookie c;
    struct (anon) peer;
    enum sctp_state state;
    int overall_error_count;
    ktime_t cookie_life;
    long unsigned int rto_initial;
    long unsigned int rto_max;
    long unsigned int rto_min;
    int max_burst;
    int max_retrans;
    __u16 pf_retrans;
    __u16 ps_retrans;
    __u16 max_init_attempts;
    __u16 init_retries;
    long unsigned int max_init_timeo;
    long unsigned int hbinterval;
    long unsigned int probe_interval;
    __be16 encap_port;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u8 pmtu_pending;
    __u32 pathmtu;
    __u32 param_flags;
    __u32 sackfreq;
    long unsigned int sackdelay;
    long unsigned int timeouts[12];
    struct timer_list timers[12];
    struct sctp_transport *shutdown_last_sent_to;
    struct sctp_transport *init_last_sent_to;
    int shutdown_retries;
    __u32 next_tsn;
    __u32 ctsn_ack_point;
    __u32 adv_peer_ack_point;
    __u32 highest_sacked;
    __u32 fast_recovery_exit;
    __u8 fast_recovery;
    __u16 unack_data;
    __u32 rtx_data_chunks;
    __u32 rwnd;
    __u32 a_rwnd;
    __u32 rwnd_over;
    __u32 rwnd_press;
    int sndbuf_used;
    atomic_t rmem_alloc;
    wait_queue_head_t wait;
    __u32 frag_point;
    __u32 user_frag;
    int init_err_counter;
    int init_cycle;
    __u16 default_stream;
    __u16 default_flags;
    __u32 default_ppid;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    struct sctp_stream stream;
    struct sctp_outq outqueue;
    struct sctp_ulpq ulpq;
    __u32 last_ecne_tsn;
    __u32 last_cwr_tsn;
    int numduptsns;
    struct sctp_chunk *addip_last_asconf;
    struct list_head asconf_ack_list;
    struct list_head addip_chunk_list;
    __u32 addip_serial;
    int src_out_of_asoc_ok;
    union sctp_addr *asconf_addr_del_pending;
    struct sctp_transport *new_transport;
    struct list_head endpoint_shared_keys;
    struct sctp_auth_bytes *asoc_shared_key;
    struct sctp_shared_key *shkey;
    __u16 default_hmac_id;
    __u16 active_key_id;
    __u8 need_ecne;
    __u8 temp;
    __u8 pf_expose;
    __u8 force_delay;
    __u8 strreset_enable;
    __u8 strreset_outstanding;
    __u32 strreset_outseq;
    __u32 strreset_inseq;
    __u32 strreset_result[2];
    struct sctp_chunk *strreset_chunk;
    struct sctp_priv_assoc_stats stats;
    int sent_cnt_removable;
    __u16 subscribe;
    __u64 abandoned_unsent[3];
    __u64 abandoned_sent[3];
    u32 secid;
    u32 peer_secid;
    struct callback_head rcu;
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
struct sctp_association {
    struct sctp_ep_common base;
    struct list_head asocs;
    sctp_assoc_t assoc_id;
    struct sctp_endpoint *ep;
    struct sctp_cookie c;
    struct (anon) peer;
    enum sctp_state state;
    int overall_error_count;
    ktime_t cookie_life;
    long unsigned int rto_initial;
    long unsigned int rto_max;
    long unsigned int rto_min;
    int max_burst;
    int max_retrans;
    int pf_retrans;
    __u16 max_init_attempts;
    __u16 init_retries;
    long unsigned int max_init_timeo;
    long unsigned int hbinterval;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u8 pmtu_pending;
    __u32 pathmtu;
    __u32 param_flags;
    __u32 sackfreq;
    long unsigned int sackdelay;
    long unsigned int timeouts[11];
    struct timer_list timers[11];
    struct sctp_transport *shutdown_last_sent_to;
    struct sctp_transport *init_last_sent_to;
    int shutdown_retries;
    __u32 next_tsn;
    __u32 ctsn_ack_point;
    __u32 adv_peer_ack_point;
    __u32 highest_sacked;
    __u32 fast_recovery_exit;
    __u8 fast_recovery;
    __u16 unack_data;
    __u32 rtx_data_chunks;
    __u32 rwnd;
    __u32 a_rwnd;
    __u32 rwnd_over;
    __u32 rwnd_press;
    int sndbuf_used;
    atomic_t rmem_alloc;
    wait_queue_head_t wait;
    __u32 frag_point;
    __u32 user_frag;
    int init_err_counter;
    int init_cycle;
    __u16 default_stream;
    __u16 default_flags;
    __u32 default_ppid;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    struct sctp_stream stream;
    struct sctp_outq outqueue;
    struct sctp_ulpq ulpq;
    __u32 last_ecne_tsn;
    __u32 last_cwr_tsn;
    int numduptsns;
    struct sctp_chunk *addip_last_asconf;
    struct list_head asconf_ack_list;
    struct list_head addip_chunk_list;
    __u32 addip_serial;
    int src_out_of_asoc_ok;
    union sctp_addr *asconf_addr_del_pending;
    struct sctp_transport *new_transport;
    struct list_head endpoint_shared_keys;
    struct sctp_auth_bytes *asoc_shared_key;
    struct sctp_shared_key *shkey;
    __u16 default_hmac_id;
    __u16 active_key_id;
    __u8 need_ecne;
    __u8 temp;
    __u8 force_delay;
    __u8 strreset_enable;
    __u8 strreset_outstanding;
    __u32 strreset_outseq;
    __u32 strreset_inseq;
    __u32 strreset_result[2];
    struct sctp_chunk *strreset_chunk;
    struct sctp_priv_assoc_stats stats;
    int sent_cnt_removable;
    __u16 subscribe;
    __u64 abandoned_unsent[3];
    __u64 abandoned_sent[3];
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct sctp_association {
    struct sctp_ep_common base;
    struct list_head asocs;
    sctp_assoc_t assoc_id;
    struct sctp_endpoint *ep;
    struct sctp_cookie c;
    struct (anon) peer;
    enum sctp_state state;
    int overall_error_count;
    ktime_t cookie_life;
    long unsigned int rto_initial;
    long unsigned int rto_max;
    long unsigned int rto_min;
    int max_burst;
    int max_retrans;
    int pf_retrans;
    __u16 max_init_attempts;
    __u16 init_retries;
    long unsigned int max_init_timeo;
    long unsigned int hbinterval;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u8 pmtu_pending;
    __u32 pathmtu;
    __u32 param_flags;
    __u32 sackfreq;
    long unsigned int sackdelay;
    long unsigned int timeouts[11];
    struct timer_list timers[11];
    struct sctp_transport *shutdown_last_sent_to;
    struct sctp_transport *init_last_sent_to;
    int shutdown_retries;
    __u32 next_tsn;
    __u32 ctsn_ack_point;
    __u32 adv_peer_ack_point;
    __u32 highest_sacked;
    __u32 fast_recovery_exit;
    __u8 fast_recovery;
    __u16 unack_data;
    __u32 rtx_data_chunks;
    __u32 rwnd;
    __u32 a_rwnd;
    __u32 rwnd_over;
    __u32 rwnd_press;
    int sndbuf_used;
    atomic_t rmem_alloc;
    wait_queue_head_t wait;
    __u32 frag_point;
    __u32 user_frag;
    int init_err_counter;
    int init_cycle;
    __u16 default_stream;
    __u16 default_flags;
    __u32 default_ppid;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    struct sctp_stream stream;
    struct sctp_outq outqueue;
    struct sctp_ulpq ulpq;
    __u32 last_ecne_tsn;
    __u32 last_cwr_tsn;
    int numduptsns;
    struct sctp_chunk *addip_last_asconf;
    struct list_head asconf_ack_list;
    struct list_head addip_chunk_list;
    __u32 addip_serial;
    int src_out_of_asoc_ok;
    union sctp_addr *asconf_addr_del_pending;
    struct sctp_transport *new_transport;
    struct list_head endpoint_shared_keys;
    struct sctp_auth_bytes *asoc_shared_key;
    struct sctp_shared_key *shkey;
    __u16 default_hmac_id;
    __u16 active_key_id;
    __u8 need_ecne;
    __u8 temp;
    __u8 force_delay;
    __u8 strreset_enable;
    __u8 strreset_outstanding;
    __u32 strreset_outseq;
    __u32 strreset_inseq;
    __u32 strreset_result[2];
    struct sctp_chunk *strreset_chunk;
    struct sctp_priv_assoc_stats stats;
    int sent_cnt_removable;
    __u16 subscribe;
    __u64 abandoned_unsent[3];
    __u64 abandoned_sent[3];
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct sctp_association {
    struct sctp_ep_common base;
    struct list_head asocs;
    sctp_assoc_t assoc_id;
    struct sctp_endpoint *ep;
    struct sctp_cookie c;
    struct (anon) peer;
    enum sctp_state state;
    int overall_error_count;
    ktime_t cookie_life;
    long unsigned int rto_initial;
    long unsigned int rto_max;
    long unsigned int rto_min;
    int max_burst;
    int max_retrans;
    int pf_retrans;
    __u16 max_init_attempts;
    __u16 init_retries;
    long unsigned int max_init_timeo;
    long unsigned int hbinterval;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u8 pmtu_pending;
    __u32 pathmtu;
    __u32 param_flags;
    __u32 sackfreq;
    long unsigned int sackdelay;
    long unsigned int timeouts[11];
    struct timer_list timers[11];
    struct sctp_transport *shutdown_last_sent_to;
    struct sctp_transport *init_last_sent_to;
    int shutdown_retries;
    __u32 next_tsn;
    __u32 ctsn_ack_point;
    __u32 adv_peer_ack_point;
    __u32 highest_sacked;
    __u32 fast_recovery_exit;
    __u8 fast_recovery;
    __u16 unack_data;
    __u32 rtx_data_chunks;
    __u32 rwnd;
    __u32 a_rwnd;
    __u32 rwnd_over;
    __u32 rwnd_press;
    int sndbuf_used;
    atomic_t rmem_alloc;
    wait_queue_head_t wait;
    __u32 frag_point;
    __u32 user_frag;
    int init_err_counter;
    int init_cycle;
    __u16 default_stream;
    __u16 default_flags;
    __u32 default_ppid;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    struct sctp_stream stream;
    struct sctp_outq outqueue;
    struct sctp_ulpq ulpq;
    __u32 last_ecne_tsn;
    __u32 last_cwr_tsn;
    int numduptsns;
    struct sctp_chunk *addip_last_asconf;
    struct list_head asconf_ack_list;
    struct list_head addip_chunk_list;
    __u32 addip_serial;
    int src_out_of_asoc_ok;
    union sctp_addr *asconf_addr_del_pending;
    struct sctp_transport *new_transport;
    struct list_head endpoint_shared_keys;
    struct sctp_auth_bytes *asoc_shared_key;
    struct sctp_shared_key *shkey;
    __u16 default_hmac_id;
    __u16 active_key_id;
    __u8 need_ecne;
    __u8 temp;
    __u8 force_delay;
    __u8 strreset_enable;
    __u8 strreset_outstanding;
    __u32 strreset_outseq;
    __u32 strreset_inseq;
    __u32 strreset_result[2];
    struct sctp_chunk *strreset_chunk;
    struct sctp_priv_assoc_stats stats;
    int sent_cnt_removable;
    __u16 subscribe;
    __u64 abandoned_unsent[3];
    __u64 abandoned_sent[3];
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct sctp_association {
    struct sctp_ep_common base;
    struct list_head asocs;
    sctp_assoc_t assoc_id;
    struct sctp_endpoint *ep;
    struct sctp_cookie c;
    struct (anon) peer;
    enum sctp_state state;
    int overall_error_count;
    ktime_t cookie_life;
    long unsigned int rto_initial;
    long unsigned int rto_max;
    long unsigned int rto_min;
    int max_burst;
    int max_retrans;
    int pf_retrans;
    __u16 max_init_attempts;
    __u16 init_retries;
    long unsigned int max_init_timeo;
    long unsigned int hbinterval;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u8 pmtu_pending;
    __u32 pathmtu;
    __u32 param_flags;
    __u32 sackfreq;
    long unsigned int sackdelay;
    long unsigned int timeouts[11];
    struct timer_list timers[11];
    struct sctp_transport *shutdown_last_sent_to;
    struct sctp_transport *init_last_sent_to;
    int shutdown_retries;
    __u32 next_tsn;
    __u32 ctsn_ack_point;
    __u32 adv_peer_ack_point;
    __u32 highest_sacked;
    __u32 fast_recovery_exit;
    __u8 fast_recovery;
    __u16 unack_data;
    __u32 rtx_data_chunks;
    __u32 rwnd;
    __u32 a_rwnd;
    __u32 rwnd_over;
    __u32 rwnd_press;
    int sndbuf_used;
    atomic_t rmem_alloc;
    wait_queue_head_t wait;
    __u32 frag_point;
    __u32 user_frag;
    int init_err_counter;
    int init_cycle;
    __u16 default_stream;
    __u16 default_flags;
    __u32 default_ppid;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    struct sctp_stream stream;
    struct sctp_outq outqueue;
    struct sctp_ulpq ulpq;
    __u32 last_ecne_tsn;
    __u32 last_cwr_tsn;
    int numduptsns;
    struct sctp_chunk *addip_last_asconf;
    struct list_head asconf_ack_list;
    struct list_head addip_chunk_list;
    __u32 addip_serial;
    int src_out_of_asoc_ok;
    union sctp_addr *asconf_addr_del_pending;
    struct sctp_transport *new_transport;
    struct list_head endpoint_shared_keys;
    struct sctp_auth_bytes *asoc_shared_key;
    struct sctp_shared_key *shkey;
    __u16 default_hmac_id;
    __u16 active_key_id;
    __u8 need_ecne;
    __u8 temp;
    __u8 force_delay;
    __u8 strreset_enable;
    __u8 strreset_outstanding;
    __u32 strreset_outseq;
    __u32 strreset_inseq;
    __u32 strreset_result[2];
    struct sctp_chunk *strreset_chunk;
    struct sctp_priv_assoc_stats stats;
    int sent_cnt_removable;
    __u16 subscribe;
    __u64 abandoned_unsent[3];
    __u64 abandoned_sent[3];
    struct callback_head rcu;
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
struct sctp_association {
    struct sctp_ep_common base;
    struct list_head asocs;
    sctp_assoc_t assoc_id;
    struct sctp_endpoint *ep;
    struct sctp_cookie c;
    struct (anon) peer;
    enum sctp_state state;
    int overall_error_count;
    ktime_t cookie_life;
    long unsigned int rto_initial;
    long unsigned int rto_max;
    long unsigned int rto_min;
    int max_burst;
    int max_retrans;
    int pf_retrans;
    __u16 max_init_attempts;
    __u16 init_retries;
    long unsigned int max_init_timeo;
    long unsigned int hbinterval;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u8 pmtu_pending;
    __u32 pathmtu;
    __u32 param_flags;
    __u32 sackfreq;
    long unsigned int sackdelay;
    long unsigned int timeouts[11];
    struct timer_list timers[11];
    struct sctp_transport *shutdown_last_sent_to;
    struct sctp_transport *init_last_sent_to;
    int shutdown_retries;
    __u32 next_tsn;
    __u32 ctsn_ack_point;
    __u32 adv_peer_ack_point;
    __u32 highest_sacked;
    __u32 fast_recovery_exit;
    __u8 fast_recovery;
    __u16 unack_data;
    __u32 rtx_data_chunks;
    __u32 rwnd;
    __u32 a_rwnd;
    __u32 rwnd_over;
    __u32 rwnd_press;
    int sndbuf_used;
    atomic_t rmem_alloc;
    wait_queue_head_t wait;
    __u32 frag_point;
    __u32 user_frag;
    int init_err_counter;
    int init_cycle;
    __u16 default_stream;
    __u16 default_flags;
    __u32 default_ppid;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    struct sctp_stream stream;
    struct sctp_outq outqueue;
    struct sctp_ulpq ulpq;
    __u32 last_ecne_tsn;
    __u32 last_cwr_tsn;
    int numduptsns;
    struct sctp_chunk *addip_last_asconf;
    struct list_head asconf_ack_list;
    struct list_head addip_chunk_list;
    __u32 addip_serial;
    int src_out_of_asoc_ok;
    union sctp_addr *asconf_addr_del_pending;
    struct sctp_transport *new_transport;
    struct list_head endpoint_shared_keys;
    struct sctp_auth_bytes *asoc_shared_key;
    struct sctp_shared_key *shkey;
    __u16 default_hmac_id;
    __u16 active_key_id;
    __u8 need_ecne;
    __u8 temp;
    __u8 force_delay;
    __u8 strreset_enable;
    __u8 strreset_outstanding;
    __u32 strreset_outseq;
    __u32 strreset_inseq;
    __u32 strreset_result[2];
    struct sctp_chunk *strreset_chunk;
    struct sctp_priv_assoc_stats stats;
    int sent_cnt_removable;
    __u16 subscribe;
    __u64 abandoned_unsent[3];
    __u64 abandoned_sent[3];
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct sctp_association {
    struct sctp_ep_common base;
    struct list_head asocs;
    sctp_assoc_t assoc_id;
    struct sctp_endpoint *ep;
    struct sctp_cookie c;
    struct (anon) peer;
    enum sctp_state state;
    int overall_error_count;
    ktime_t cookie_life;
    long unsigned int rto_initial;
    long unsigned int rto_max;
    long unsigned int rto_min;
    int max_burst;
    int max_retrans;
    int pf_retrans;
    __u16 max_init_attempts;
    __u16 init_retries;
    long unsigned int max_init_timeo;
    long unsigned int hbinterval;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u8 pmtu_pending;
    __u32 pathmtu;
    __u32 param_flags;
    __u32 sackfreq;
    long unsigned int sackdelay;
    long unsigned int timeouts[11];
    struct timer_list timers[11];
    struct sctp_transport *shutdown_last_sent_to;
    struct sctp_transport *init_last_sent_to;
    int shutdown_retries;
    __u32 next_tsn;
    __u32 ctsn_ack_point;
    __u32 adv_peer_ack_point;
    __u32 highest_sacked;
    __u32 fast_recovery_exit;
    __u8 fast_recovery;
    __u16 unack_data;
    __u32 rtx_data_chunks;
    __u32 rwnd;
    __u32 a_rwnd;
    __u32 rwnd_over;
    __u32 rwnd_press;
    int sndbuf_used;
    atomic_t rmem_alloc;
    wait_queue_head_t wait;
    __u32 frag_point;
    __u32 user_frag;
    int init_err_counter;
    int init_cycle;
    __u16 default_stream;
    __u16 default_flags;
    __u32 default_ppid;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    struct sctp_stream stream;
    struct sctp_outq outqueue;
    struct sctp_ulpq ulpq;
    __u32 last_ecne_tsn;
    __u32 last_cwr_tsn;
    int numduptsns;
    struct sctp_chunk *addip_last_asconf;
    struct list_head asconf_ack_list;
    struct list_head addip_chunk_list;
    __u32 addip_serial;
    int src_out_of_asoc_ok;
    union sctp_addr *asconf_addr_del_pending;
    struct sctp_transport *new_transport;
    struct list_head endpoint_shared_keys;
    struct sctp_auth_bytes *asoc_shared_key;
    struct sctp_shared_key *shkey;
    __u16 default_hmac_id;
    __u16 active_key_id;
    __u8 need_ecne;
    __u8 temp;
    __u8 force_delay;
    __u8 strreset_enable;
    __u8 strreset_outstanding;
    __u32 strreset_outseq;
    __u32 strreset_inseq;
    __u32 strreset_result[2];
    struct sctp_chunk *strreset_chunk;
    struct sctp_priv_assoc_stats stats;
    int sent_cnt_removable;
    __u16 subscribe;
    __u64 abandoned_unsent[3];
    __u64 abandoned_sent[3];
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct sctp_association {
    struct sctp_ep_common base;
    struct list_head asocs;
    sctp_assoc_t assoc_id;
    struct sctp_endpoint *ep;
    struct sctp_cookie c;
    struct (anon) peer;
    enum sctp_state state;
    int overall_error_count;
    ktime_t cookie_life;
    long unsigned int rto_initial;
    long unsigned int rto_max;
    long unsigned int rto_min;
    int max_burst;
    int max_retrans;
    int pf_retrans;
    __u16 max_init_attempts;
    __u16 init_retries;
    long unsigned int max_init_timeo;
    long unsigned int hbinterval;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u8 pmtu_pending;
    __u32 pathmtu;
    __u32 param_flags;
    __u32 sackfreq;
    long unsigned int sackdelay;
    long unsigned int timeouts[11];
    struct timer_list timers[11];
    struct sctp_transport *shutdown_last_sent_to;
    struct sctp_transport *init_last_sent_to;
    int shutdown_retries;
    __u32 next_tsn;
    __u32 ctsn_ack_point;
    __u32 adv_peer_ack_point;
    __u32 highest_sacked;
    __u32 fast_recovery_exit;
    __u8 fast_recovery;
    __u16 unack_data;
    __u32 rtx_data_chunks;
    __u32 rwnd;
    __u32 a_rwnd;
    __u32 rwnd_over;
    __u32 rwnd_press;
    int sndbuf_used;
    atomic_t rmem_alloc;
    wait_queue_head_t wait;
    __u32 frag_point;
    __u32 user_frag;
    int init_err_counter;
    int init_cycle;
    __u16 default_stream;
    __u16 default_flags;
    __u32 default_ppid;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    struct sctp_stream stream;
    struct sctp_outq outqueue;
    struct sctp_ulpq ulpq;
    __u32 last_ecne_tsn;
    __u32 last_cwr_tsn;
    int numduptsns;
    struct sctp_chunk *addip_last_asconf;
    struct list_head asconf_ack_list;
    struct list_head addip_chunk_list;
    __u32 addip_serial;
    int src_out_of_asoc_ok;
    union sctp_addr *asconf_addr_del_pending;
    struct sctp_transport *new_transport;
    struct list_head endpoint_shared_keys;
    struct sctp_auth_bytes *asoc_shared_key;
    struct sctp_shared_key *shkey;
    __u16 default_hmac_id;
    __u16 active_key_id;
    __u8 need_ecne;
    __u8 temp;
    __u8 force_delay;
    __u8 strreset_enable;
    __u8 strreset_outstanding;
    __u32 strreset_outseq;
    __u32 strreset_inseq;
    __u32 strreset_result[2];
    struct sctp_chunk *strreset_chunk;
    struct sctp_priv_assoc_stats stats;
    int sent_cnt_removable;
    __u16 subscribe;
    __u64 abandoned_unsent[3];
    __u64 abandoned_sent[3];
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct sctp_association {
    struct sctp_ep_common base;
    struct list_head asocs;
    sctp_assoc_t assoc_id;
    struct sctp_endpoint *ep;
    struct sctp_cookie c;
    struct (anon) peer;
    enum sctp_state state;
    int overall_error_count;
    ktime_t cookie_life;
    long unsigned int rto_initial;
    long unsigned int rto_max;
    long unsigned int rto_min;
    int max_burst;
    int max_retrans;
    int pf_retrans;
    __u16 max_init_attempts;
    __u16 init_retries;
    long unsigned int max_init_timeo;
    long unsigned int hbinterval;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u8 pmtu_pending;
    __u32 pathmtu;
    __u32 param_flags;
    __u32 sackfreq;
    long unsigned int sackdelay;
    long unsigned int timeouts[11];
    struct timer_list timers[11];
    struct sctp_transport *shutdown_last_sent_to;
    struct sctp_transport *init_last_sent_to;
    int shutdown_retries;
    __u32 next_tsn;
    __u32 ctsn_ack_point;
    __u32 adv_peer_ack_point;
    __u32 highest_sacked;
    __u32 fast_recovery_exit;
    __u8 fast_recovery;
    __u16 unack_data;
    __u32 rtx_data_chunks;
    __u32 rwnd;
    __u32 a_rwnd;
    __u32 rwnd_over;
    __u32 rwnd_press;
    int sndbuf_used;
    atomic_t rmem_alloc;
    wait_queue_head_t wait;
    __u32 frag_point;
    __u32 user_frag;
    int init_err_counter;
    int init_cycle;
    __u16 default_stream;
    __u16 default_flags;
    __u32 default_ppid;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    struct sctp_stream stream;
    struct sctp_outq outqueue;
    struct sctp_ulpq ulpq;
    __u32 last_ecne_tsn;
    __u32 last_cwr_tsn;
    int numduptsns;
    struct sctp_chunk *addip_last_asconf;
    struct list_head asconf_ack_list;
    struct list_head addip_chunk_list;
    __u32 addip_serial;
    int src_out_of_asoc_ok;
    union sctp_addr *asconf_addr_del_pending;
    struct sctp_transport *new_transport;
    struct list_head endpoint_shared_keys;
    struct sctp_auth_bytes *asoc_shared_key;
    struct sctp_shared_key *shkey;
    __u16 default_hmac_id;
    __u16 active_key_id;
    __u8 need_ecne;
    __u8 temp;
    __u8 force_delay;
    __u8 strreset_enable;
    __u8 strreset_outstanding;
    __u32 strreset_outseq;
    __u32 strreset_inseq;
    __u32 strreset_result[2];
    struct sctp_chunk *strreset_chunk;
    struct sctp_priv_assoc_stats stats;
    int sent_cnt_removable;
    __u16 subscribe;
    __u64 abandoned_unsent[3];
    __u64 abandoned_sent[3];
    struct callback_head rcu;
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
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u32 flowlabel</code>
</li>
<li>
<b>Field added. </b>
<code>__u8 dscp</code>
</li>
<li>
<b>Field added. </b>
<code>__u16 subscribe</code>
</li>
<li>
<b>Field added. </b>
<code>struct callback_head rcu</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>__u8 intl_enable</code>
</li>
<li>
<b>Field removed. </b>
<code>__u8 prsctp_enable</code>
</li>
<li>
<b>Field removed. </b>
<code>__u8 reconf_enable</code>
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
<b>Field added. </b>
<code>__u16 ps_retrans</code>
</li>
<li>
<b>Field added. </b>
<code>__u8 pf_expose</code>
</li>
<li>
<b>Field type changed. </b>
<code>int pf_retrans</code> ➡️ <code>__u16 pf_retrans</code>
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
<code>__be16 encap_port</code>
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
<code>long unsigned int probe_interval</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int timeouts[11]</code> ➡️ <code>long unsigned int timeouts[12]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct timer_list timers[11]</code> ➡️ <code>struct timer_list timers[12]</code>
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
<code>u32 secid</code>
</li>
<li>
<b>Field added. </b>
<code>u32 peer_secid</code>
</li>
</ul>
</details>
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
