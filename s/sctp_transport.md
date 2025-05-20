# Struct: <code>sctp_transport</code>

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
struct sctp_transport {
    struct list_head transports;
    struct rhlist_head node;
    refcount_t refcnt;
    __u32 rto_pending;
    __u32 hb_sent;
    __u32 pmtu_pending;
    __u32 dst_pending_confirm;
    __u32 sack_generation;
    u32 dst_cookie;
    struct flowi fl;
    union sctp_addr ipaddr;
    struct sctp_af *af_specific;
    struct sctp_association *asoc;
    long unsigned int rto;
    __u32 rtt;
    __u32 rttvar;
    __u32 srtt;
    __u32 cwnd;
    __u32 ssthresh;
    __u32 partial_bytes_acked;
    __u32 flight_size;
    __u32 burst_limited;
    struct dst_entry *dst;
    union sctp_addr saddr;
    long unsigned int hbinterval;
    long unsigned int sackdelay;
    __u32 sackfreq;
    ktime_t last_time_heard;
    long unsigned int last_time_sent;
    long unsigned int last_time_ecne_reduced;
    __u16 pathmaxrxt;
    int pf_retrans;
    __u32 pathmtu;
    __u32 param_flags;
    int init_sent_count;
    int state;
    short unsigned int error_count;
    struct timer_list T3_rtx_timer;
    struct timer_list hb_timer;
    struct timer_list proto_unreach_timer;
    struct timer_list reconf_timer;
    struct list_head transmitted;
    struct sctp_packet packet;
    struct list_head send_ready;
    struct (anon) cacc;
    __u64 hb_nonce;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct sctp_transport {
    struct list_head transports;
    struct rhlist_head node;
    refcount_t refcnt;
    __u32 rto_pending;
    __u32 hb_sent;
    __u32 pmtu_pending;
    __u32 dst_pending_confirm;
    __u32 sack_generation;
    u32 dst_cookie;
    struct flowi fl;
    union sctp_addr ipaddr;
    struct sctp_af *af_specific;
    struct sctp_association *asoc;
    long unsigned int rto;
    __u32 rtt;
    __u32 rttvar;
    __u32 srtt;
    __u32 cwnd;
    __u32 ssthresh;
    __u32 partial_bytes_acked;
    __u32 flight_size;
    __u32 burst_limited;
    struct dst_entry *dst;
    union sctp_addr saddr;
    long unsigned int hbinterval;
    long unsigned int sackdelay;
    __u32 sackfreq;
    atomic_t mtu_info;
    ktime_t last_time_heard;
    long unsigned int last_time_sent;
    long unsigned int last_time_ecne_reduced;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    int pf_retrans;
    __u32 pathmtu;
    __u32 param_flags;
    int init_sent_count;
    int state;
    short unsigned int error_count;
    struct timer_list T3_rtx_timer;
    struct timer_list hb_timer;
    struct timer_list proto_unreach_timer;
    struct timer_list reconf_timer;
    struct list_head transmitted;
    struct sctp_packet packet;
    struct list_head send_ready;
    struct (anon) cacc;
    __u64 hb_nonce;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct sctp_transport {
    struct list_head transports;
    struct rhlist_head node;
    refcount_t refcnt;
    __u32 rto_pending;
    __u32 hb_sent;
    __u32 pmtu_pending;
    __u32 dst_pending_confirm;
    __u32 sack_generation;
    u32 dst_cookie;
    struct flowi fl;
    union sctp_addr ipaddr;
    struct sctp_af *af_specific;
    struct sctp_association *asoc;
    long unsigned int rto;
    __u32 rtt;
    __u32 rttvar;
    __u32 srtt;
    __u32 cwnd;
    __u32 ssthresh;
    __u32 partial_bytes_acked;
    __u32 flight_size;
    __u32 burst_limited;
    struct dst_entry *dst;
    union sctp_addr saddr;
    long unsigned int hbinterval;
    long unsigned int sackdelay;
    __u32 sackfreq;
    atomic_t mtu_info;
    ktime_t last_time_heard;
    long unsigned int last_time_sent;
    long unsigned int last_time_ecne_reduced;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    int pf_retrans;
    __u32 pathmtu;
    __u32 param_flags;
    int init_sent_count;
    int state;
    short unsigned int error_count;
    struct timer_list T3_rtx_timer;
    struct timer_list hb_timer;
    struct timer_list proto_unreach_timer;
    struct timer_list reconf_timer;
    struct list_head transmitted;
    struct sctp_packet packet;
    struct list_head send_ready;
    struct (anon) cacc;
    __u64 hb_nonce;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct sctp_transport {
    struct list_head transports;
    struct rhlist_head node;
    refcount_t refcnt;
    __u32 rto_pending;
    __u32 hb_sent;
    __u32 pmtu_pending;
    __u32 dst_pending_confirm;
    __u32 sack_generation;
    u32 dst_cookie;
    struct flowi fl;
    union sctp_addr ipaddr;
    struct sctp_af *af_specific;
    struct sctp_association *asoc;
    long unsigned int rto;
    __u32 rtt;
    __u32 rttvar;
    __u32 srtt;
    __u32 cwnd;
    __u32 ssthresh;
    __u32 partial_bytes_acked;
    __u32 flight_size;
    __u32 burst_limited;
    struct dst_entry *dst;
    union sctp_addr saddr;
    long unsigned int hbinterval;
    long unsigned int sackdelay;
    __u32 sackfreq;
    atomic_t mtu_info;
    ktime_t last_time_heard;
    long unsigned int last_time_sent;
    long unsigned int last_time_ecne_reduced;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    int pf_retrans;
    __u32 pathmtu;
    __u32 param_flags;
    int init_sent_count;
    int state;
    short unsigned int error_count;
    struct timer_list T3_rtx_timer;
    struct timer_list hb_timer;
    struct timer_list proto_unreach_timer;
    struct timer_list reconf_timer;
    struct list_head transmitted;
    struct sctp_packet packet;
    struct list_head send_ready;
    struct (anon) cacc;
    __u64 hb_nonce;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct sctp_transport {
    struct list_head transports;
    struct rhlist_head node;
    refcount_t refcnt;
    __u32 rto_pending;
    __u32 hb_sent;
    __u32 pmtu_pending;
    __u32 dst_pending_confirm;
    __u32 sack_generation;
    u32 dst_cookie;
    struct flowi fl;
    union sctp_addr ipaddr;
    struct sctp_af *af_specific;
    struct sctp_association *asoc;
    long unsigned int rto;
    __u32 rtt;
    __u32 rttvar;
    __u32 srtt;
    __u32 cwnd;
    __u32 ssthresh;
    __u32 partial_bytes_acked;
    __u32 flight_size;
    __u32 burst_limited;
    struct dst_entry *dst;
    union sctp_addr saddr;
    long unsigned int hbinterval;
    long unsigned int sackdelay;
    __u32 sackfreq;
    atomic_t mtu_info;
    ktime_t last_time_heard;
    long unsigned int last_time_sent;
    long unsigned int last_time_ecne_reduced;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u16 pf_retrans;
    __u16 ps_retrans;
    __u32 pathmtu;
    __u32 param_flags;
    int init_sent_count;
    int state;
    short unsigned int error_count;
    struct timer_list T3_rtx_timer;
    struct timer_list hb_timer;
    struct timer_list proto_unreach_timer;
    struct timer_list reconf_timer;
    struct list_head transmitted;
    struct sctp_packet packet;
    struct list_head send_ready;
    struct (anon) cacc;
    __u64 hb_nonce;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct sctp_transport {
    struct list_head transports;
    struct rhlist_head node;
    refcount_t refcnt;
    __u32 rto_pending;
    __u32 hb_sent;
    __u32 pmtu_pending;
    __u32 dst_pending_confirm;
    __u32 sack_generation;
    u32 dst_cookie;
    struct flowi fl;
    union sctp_addr ipaddr;
    struct sctp_af *af_specific;
    struct sctp_association *asoc;
    long unsigned int rto;
    __u32 rtt;
    __u32 rttvar;
    __u32 srtt;
    __u32 cwnd;
    __u32 ssthresh;
    __u32 partial_bytes_acked;
    __u32 flight_size;
    __u32 burst_limited;
    struct dst_entry *dst;
    union sctp_addr saddr;
    long unsigned int hbinterval;
    long unsigned int sackdelay;
    __u32 sackfreq;
    atomic_t mtu_info;
    ktime_t last_time_heard;
    long unsigned int last_time_sent;
    long unsigned int last_time_ecne_reduced;
    __be16 encap_port;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u16 pf_retrans;
    __u16 ps_retrans;
    __u32 pathmtu;
    __u32 param_flags;
    int init_sent_count;
    int state;
    short unsigned int error_count;
    struct timer_list T3_rtx_timer;
    struct timer_list hb_timer;
    struct timer_list proto_unreach_timer;
    struct timer_list reconf_timer;
    struct list_head transmitted;
    struct sctp_packet packet;
    struct list_head send_ready;
    struct (anon) cacc;
    __u64 hb_nonce;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct sctp_transport {
    struct list_head transports;
    struct rhlist_head node;
    refcount_t refcnt;
    __u32 rto_pending;
    __u32 hb_sent;
    __u32 pmtu_pending;
    __u32 dst_pending_confirm;
    __u32 sack_generation;
    u32 dst_cookie;
    struct flowi fl;
    union sctp_addr ipaddr;
    struct sctp_af *af_specific;
    struct sctp_association *asoc;
    long unsigned int rto;
    __u32 rtt;
    __u32 rttvar;
    __u32 srtt;
    __u32 cwnd;
    __u32 ssthresh;
    __u32 partial_bytes_acked;
    __u32 flight_size;
    __u32 burst_limited;
    struct dst_entry *dst;
    union sctp_addr saddr;
    long unsigned int hbinterval;
    long unsigned int sackdelay;
    __u32 sackfreq;
    atomic_t mtu_info;
    ktime_t last_time_heard;
    long unsigned int last_time_sent;
    long unsigned int last_time_ecne_reduced;
    __be16 encap_port;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u16 pf_retrans;
    __u16 ps_retrans;
    __u32 pathmtu;
    __u32 param_flags;
    int init_sent_count;
    int state;
    short unsigned int error_count;
    struct timer_list T3_rtx_timer;
    struct timer_list hb_timer;
    struct timer_list proto_unreach_timer;
    struct timer_list reconf_timer;
    struct list_head transmitted;
    struct sctp_packet packet;
    struct list_head send_ready;
    struct (anon) cacc;
    __u64 hb_nonce;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct sctp_transport {
    struct list_head transports;
    struct rhlist_head node;
    refcount_t refcnt;
    __u32 rto_pending;
    __u32 hb_sent;
    __u32 pmtu_pending;
    __u32 dst_pending_confirm;
    __u32 sack_generation;
    u32 dst_cookie;
    struct flowi fl;
    union sctp_addr ipaddr;
    struct sctp_af *af_specific;
    struct sctp_association *asoc;
    long unsigned int rto;
    __u32 rtt;
    __u32 rttvar;
    __u32 srtt;
    __u32 cwnd;
    __u32 ssthresh;
    __u32 partial_bytes_acked;
    __u32 flight_size;
    __u32 burst_limited;
    struct dst_entry *dst;
    union sctp_addr saddr;
    long unsigned int hbinterval;
    long unsigned int probe_interval;
    long unsigned int sackdelay;
    __u32 sackfreq;
    atomic_t mtu_info;
    ktime_t last_time_heard;
    long unsigned int last_time_sent;
    long unsigned int last_time_ecne_reduced;
    __be16 encap_port;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u16 pf_retrans;
    __u16 ps_retrans;
    __u32 pathmtu;
    __u32 param_flags;
    int init_sent_count;
    int state;
    short unsigned int error_count;
    struct timer_list T3_rtx_timer;
    struct timer_list hb_timer;
    struct timer_list proto_unreach_timer;
    struct timer_list reconf_timer;
    struct timer_list probe_timer;
    struct list_head transmitted;
    struct sctp_packet packet;
    struct list_head send_ready;
    struct (anon) cacc;
    struct (anon) pl;
    __u64 hb_nonce;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct sctp_transport {
    struct list_head transports;
    struct rhlist_head node;
    refcount_t refcnt;
    __u32 rto_pending;
    __u32 hb_sent;
    __u32 pmtu_pending;
    __u32 dst_pending_confirm;
    __u32 sack_generation;
    u32 dst_cookie;
    struct flowi fl;
    union sctp_addr ipaddr;
    struct sctp_af *af_specific;
    struct sctp_association *asoc;
    long unsigned int rto;
    __u32 rtt;
    __u32 rttvar;
    __u32 srtt;
    __u32 cwnd;
    __u32 ssthresh;
    __u32 partial_bytes_acked;
    __u32 flight_size;
    __u32 burst_limited;
    struct dst_entry *dst;
    union sctp_addr saddr;
    long unsigned int hbinterval;
    long unsigned int probe_interval;
    long unsigned int sackdelay;
    __u32 sackfreq;
    atomic_t mtu_info;
    ktime_t last_time_heard;
    long unsigned int last_time_sent;
    long unsigned int last_time_ecne_reduced;
    __be16 encap_port;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u16 pf_retrans;
    __u16 ps_retrans;
    __u32 pathmtu;
    __u32 param_flags;
    int init_sent_count;
    int state;
    short unsigned int error_count;
    struct timer_list T3_rtx_timer;
    struct timer_list hb_timer;
    struct timer_list proto_unreach_timer;
    struct timer_list reconf_timer;
    struct timer_list probe_timer;
    struct list_head transmitted;
    struct sctp_packet packet;
    struct list_head send_ready;
    struct (anon) cacc;
    struct (anon) pl;
    __u64 hb_nonce;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct sctp_transport {
    struct list_head transports;
    struct rhlist_head node;
    refcount_t refcnt;
    __u32 rto_pending;
    __u32 hb_sent;
    __u32 pmtu_pending;
    __u32 dst_pending_confirm;
    __u32 sack_generation;
    u32 dst_cookie;
    struct flowi fl;
    union sctp_addr ipaddr;
    struct sctp_af *af_specific;
    struct sctp_association *asoc;
    long unsigned int rto;
    __u32 rtt;
    __u32 rttvar;
    __u32 srtt;
    __u32 cwnd;
    __u32 ssthresh;
    __u32 partial_bytes_acked;
    __u32 flight_size;
    __u32 burst_limited;
    struct dst_entry *dst;
    union sctp_addr saddr;
    long unsigned int hbinterval;
    long unsigned int probe_interval;
    long unsigned int sackdelay;
    __u32 sackfreq;
    atomic_t mtu_info;
    ktime_t last_time_heard;
    long unsigned int last_time_sent;
    long unsigned int last_time_ecne_reduced;
    __be16 encap_port;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u16 pf_retrans;
    __u16 ps_retrans;
    __u32 pathmtu;
    __u32 param_flags;
    int init_sent_count;
    int state;
    short unsigned int error_count;
    struct timer_list T3_rtx_timer;
    struct timer_list hb_timer;
    struct timer_list proto_unreach_timer;
    struct timer_list reconf_timer;
    struct timer_list probe_timer;
    struct list_head transmitted;
    struct sctp_packet packet;
    struct list_head send_ready;
    struct (anon) cacc;
    struct (anon) pl;
    __u64 hb_nonce;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct sctp_transport {
    struct list_head transports;
    struct rhlist_head node;
    refcount_t refcnt;
    __u32 rto_pending;
    __u32 hb_sent;
    __u32 pmtu_pending;
    __u32 dst_pending_confirm;
    __u32 sack_generation;
    u32 dst_cookie;
    struct flowi fl;
    union sctp_addr ipaddr;
    struct sctp_af *af_specific;
    struct sctp_association *asoc;
    long unsigned int rto;
    __u32 rtt;
    __u32 rttvar;
    __u32 srtt;
    __u32 cwnd;
    __u32 ssthresh;
    __u32 partial_bytes_acked;
    __u32 flight_size;
    __u32 burst_limited;
    struct dst_entry *dst;
    union sctp_addr saddr;
    long unsigned int hbinterval;
    long unsigned int probe_interval;
    long unsigned int sackdelay;
    __u32 sackfreq;
    atomic_t mtu_info;
    ktime_t last_time_heard;
    long unsigned int last_time_sent;
    long unsigned int last_time_ecne_reduced;
    __be16 encap_port;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u16 pf_retrans;
    __u16 ps_retrans;
    __u32 pathmtu;
    __u32 param_flags;
    int init_sent_count;
    int state;
    short unsigned int error_count;
    struct timer_list T3_rtx_timer;
    struct timer_list hb_timer;
    struct timer_list proto_unreach_timer;
    struct timer_list reconf_timer;
    struct timer_list probe_timer;
    struct list_head transmitted;
    struct sctp_packet packet;
    struct list_head send_ready;
    struct (anon) cacc;
    struct (anon) pl;
    __u64 hb_nonce;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct sctp_transport {
    struct list_head transports;
    struct rhlist_head node;
    refcount_t refcnt;
    __u32 rto_pending;
    __u32 hb_sent;
    __u32 pmtu_pending;
    __u32 dst_pending_confirm;
    __u32 sack_generation;
    u32 dst_cookie;
    struct flowi fl;
    union sctp_addr ipaddr;
    struct sctp_af *af_specific;
    struct sctp_association *asoc;
    long unsigned int rto;
    __u32 rtt;
    __u32 rttvar;
    __u32 srtt;
    __u32 cwnd;
    __u32 ssthresh;
    __u32 partial_bytes_acked;
    __u32 flight_size;
    __u32 burst_limited;
    struct dst_entry *dst;
    union sctp_addr saddr;
    long unsigned int hbinterval;
    long unsigned int probe_interval;
    long unsigned int sackdelay;
    __u32 sackfreq;
    atomic_t mtu_info;
    ktime_t last_time_heard;
    long unsigned int last_time_sent;
    long unsigned int last_time_ecne_reduced;
    __be16 encap_port;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u16 pf_retrans;
    __u16 ps_retrans;
    __u32 pathmtu;
    __u32 param_flags;
    int init_sent_count;
    int state;
    short unsigned int error_count;
    struct timer_list T3_rtx_timer;
    struct timer_list hb_timer;
    struct timer_list proto_unreach_timer;
    struct timer_list reconf_timer;
    struct timer_list probe_timer;
    struct list_head transmitted;
    struct sctp_packet packet;
    struct list_head send_ready;
    struct (anon) cacc;
    struct (anon) pl;
    __u64 hb_nonce;
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
struct sctp_transport {
    struct list_head transports;
    struct rhlist_head node;
    refcount_t refcnt;
    __u32 rto_pending;
    __u32 hb_sent;
    __u32 pmtu_pending;
    __u32 dst_pending_confirm;
    __u32 sack_generation;
    u32 dst_cookie;
    struct flowi fl;
    union sctp_addr ipaddr;
    struct sctp_af *af_specific;
    struct sctp_association *asoc;
    long unsigned int rto;
    __u32 rtt;
    __u32 rttvar;
    __u32 srtt;
    __u32 cwnd;
    __u32 ssthresh;
    __u32 partial_bytes_acked;
    __u32 flight_size;
    __u32 burst_limited;
    struct dst_entry *dst;
    union sctp_addr saddr;
    long unsigned int hbinterval;
    long unsigned int sackdelay;
    __u32 sackfreq;
    atomic_t mtu_info;
    ktime_t last_time_heard;
    long unsigned int last_time_sent;
    long unsigned int last_time_ecne_reduced;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    int pf_retrans;
    __u32 pathmtu;
    __u32 param_flags;
    int init_sent_count;
    int state;
    short unsigned int error_count;
    struct timer_list T3_rtx_timer;
    struct timer_list hb_timer;
    struct timer_list proto_unreach_timer;
    struct timer_list reconf_timer;
    struct list_head transmitted;
    struct sctp_packet packet;
    struct list_head send_ready;
    struct (anon) cacc;
    __u64 hb_nonce;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct sctp_transport {
    struct list_head transports;
    struct rhlist_head node;
    refcount_t refcnt;
    __u32 rto_pending;
    __u32 hb_sent;
    __u32 pmtu_pending;
    __u32 dst_pending_confirm;
    __u32 sack_generation;
    u32 dst_cookie;
    struct flowi fl;
    union sctp_addr ipaddr;
    struct sctp_af *af_specific;
    struct sctp_association *asoc;
    long unsigned int rto;
    __u32 rtt;
    __u32 rttvar;
    __u32 srtt;
    __u32 cwnd;
    __u32 ssthresh;
    __u32 partial_bytes_acked;
    __u32 flight_size;
    __u32 burst_limited;
    struct dst_entry *dst;
    union sctp_addr saddr;
    long unsigned int hbinterval;
    long unsigned int sackdelay;
    __u32 sackfreq;
    atomic_t mtu_info;
    ktime_t last_time_heard;
    long unsigned int last_time_sent;
    long unsigned int last_time_ecne_reduced;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    int pf_retrans;
    __u32 pathmtu;
    __u32 param_flags;
    int init_sent_count;
    int state;
    short unsigned int error_count;
    struct timer_list T3_rtx_timer;
    struct timer_list hb_timer;
    struct timer_list proto_unreach_timer;
    struct timer_list reconf_timer;
    struct list_head transmitted;
    struct sctp_packet packet;
    struct list_head send_ready;
    struct (anon) cacc;
    __u64 hb_nonce;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct sctp_transport {
    struct list_head transports;
    struct rhlist_head node;
    refcount_t refcnt;
    __u32 rto_pending;
    __u32 hb_sent;
    __u32 pmtu_pending;
    __u32 dst_pending_confirm;
    __u32 sack_generation;
    u32 dst_cookie;
    struct flowi fl;
    union sctp_addr ipaddr;
    struct sctp_af *af_specific;
    struct sctp_association *asoc;
    long unsigned int rto;
    __u32 rtt;
    __u32 rttvar;
    __u32 srtt;
    __u32 cwnd;
    __u32 ssthresh;
    __u32 partial_bytes_acked;
    __u32 flight_size;
    __u32 burst_limited;
    struct dst_entry *dst;
    union sctp_addr saddr;
    long unsigned int hbinterval;
    long unsigned int sackdelay;
    __u32 sackfreq;
    atomic_t mtu_info;
    ktime_t last_time_heard;
    long unsigned int last_time_sent;
    long unsigned int last_time_ecne_reduced;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    int pf_retrans;
    __u32 pathmtu;
    __u32 param_flags;
    int init_sent_count;
    int state;
    short unsigned int error_count;
    struct timer_list T3_rtx_timer;
    struct timer_list hb_timer;
    struct timer_list proto_unreach_timer;
    struct timer_list reconf_timer;
    struct list_head transmitted;
    struct sctp_packet packet;
    struct list_head send_ready;
    struct (anon) cacc;
    __u64 hb_nonce;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct sctp_transport {
    struct list_head transports;
    struct rhlist_head node;
    refcount_t refcnt;
    __u32 rto_pending;
    __u32 hb_sent;
    __u32 pmtu_pending;
    __u32 dst_pending_confirm;
    __u32 sack_generation;
    u32 dst_cookie;
    struct flowi fl;
    union sctp_addr ipaddr;
    struct sctp_af *af_specific;
    struct sctp_association *asoc;
    long unsigned int rto;
    __u32 rtt;
    __u32 rttvar;
    __u32 srtt;
    __u32 cwnd;
    __u32 ssthresh;
    __u32 partial_bytes_acked;
    __u32 flight_size;
    __u32 burst_limited;
    struct dst_entry *dst;
    union sctp_addr saddr;
    long unsigned int hbinterval;
    long unsigned int sackdelay;
    __u32 sackfreq;
    atomic_t mtu_info;
    ktime_t last_time_heard;
    long unsigned int last_time_sent;
    long unsigned int last_time_ecne_reduced;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    int pf_retrans;
    __u32 pathmtu;
    __u32 param_flags;
    int init_sent_count;
    int state;
    short unsigned int error_count;
    struct timer_list T3_rtx_timer;
    struct timer_list hb_timer;
    struct timer_list proto_unreach_timer;
    struct timer_list reconf_timer;
    struct list_head transmitted;
    struct sctp_packet packet;
    struct list_head send_ready;
    struct (anon) cacc;
    __u64 hb_nonce;
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
struct sctp_transport {
    struct list_head transports;
    struct rhlist_head node;
    refcount_t refcnt;
    __u32 rto_pending;
    __u32 hb_sent;
    __u32 pmtu_pending;
    __u32 dst_pending_confirm;
    __u32 sack_generation;
    u32 dst_cookie;
    struct flowi fl;
    union sctp_addr ipaddr;
    struct sctp_af *af_specific;
    struct sctp_association *asoc;
    long unsigned int rto;
    __u32 rtt;
    __u32 rttvar;
    __u32 srtt;
    __u32 cwnd;
    __u32 ssthresh;
    __u32 partial_bytes_acked;
    __u32 flight_size;
    __u32 burst_limited;
    struct dst_entry *dst;
    union sctp_addr saddr;
    long unsigned int hbinterval;
    long unsigned int sackdelay;
    __u32 sackfreq;
    atomic_t mtu_info;
    ktime_t last_time_heard;
    long unsigned int last_time_sent;
    long unsigned int last_time_ecne_reduced;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    int pf_retrans;
    __u32 pathmtu;
    __u32 param_flags;
    int init_sent_count;
    int state;
    short unsigned int error_count;
    struct timer_list T3_rtx_timer;
    struct timer_list hb_timer;
    struct timer_list proto_unreach_timer;
    struct timer_list reconf_timer;
    struct list_head transmitted;
    struct sctp_packet packet;
    struct list_head send_ready;
    struct (anon) cacc;
    __u64 hb_nonce;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct sctp_transport {
    struct list_head transports;
    struct rhlist_head node;
    refcount_t refcnt;
    __u32 rto_pending;
    __u32 hb_sent;
    __u32 pmtu_pending;
    __u32 dst_pending_confirm;
    __u32 sack_generation;
    u32 dst_cookie;
    struct flowi fl;
    union sctp_addr ipaddr;
    struct sctp_af *af_specific;
    struct sctp_association *asoc;
    long unsigned int rto;
    __u32 rtt;
    __u32 rttvar;
    __u32 srtt;
    __u32 cwnd;
    __u32 ssthresh;
    __u32 partial_bytes_acked;
    __u32 flight_size;
    __u32 burst_limited;
    struct dst_entry *dst;
    union sctp_addr saddr;
    long unsigned int hbinterval;
    long unsigned int sackdelay;
    __u32 sackfreq;
    atomic_t mtu_info;
    ktime_t last_time_heard;
    long unsigned int last_time_sent;
    long unsigned int last_time_ecne_reduced;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    int pf_retrans;
    __u32 pathmtu;
    __u32 param_flags;
    int init_sent_count;
    int state;
    short unsigned int error_count;
    struct timer_list T3_rtx_timer;
    struct timer_list hb_timer;
    struct timer_list proto_unreach_timer;
    struct timer_list reconf_timer;
    struct list_head transmitted;
    struct sctp_packet packet;
    struct list_head send_ready;
    struct (anon) cacc;
    __u64 hb_nonce;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct sctp_transport {
    struct list_head transports;
    struct rhlist_head node;
    refcount_t refcnt;
    __u32 rto_pending;
    __u32 hb_sent;
    __u32 pmtu_pending;
    __u32 dst_pending_confirm;
    __u32 sack_generation;
    u32 dst_cookie;
    struct flowi fl;
    union sctp_addr ipaddr;
    struct sctp_af *af_specific;
    struct sctp_association *asoc;
    long unsigned int rto;
    __u32 rtt;
    __u32 rttvar;
    __u32 srtt;
    __u32 cwnd;
    __u32 ssthresh;
    __u32 partial_bytes_acked;
    __u32 flight_size;
    __u32 burst_limited;
    struct dst_entry *dst;
    union sctp_addr saddr;
    long unsigned int hbinterval;
    long unsigned int sackdelay;
    __u32 sackfreq;
    atomic_t mtu_info;
    ktime_t last_time_heard;
    long unsigned int last_time_sent;
    long unsigned int last_time_ecne_reduced;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    int pf_retrans;
    __u32 pathmtu;
    __u32 param_flags;
    int init_sent_count;
    int state;
    short unsigned int error_count;
    struct timer_list T3_rtx_timer;
    struct timer_list hb_timer;
    struct timer_list proto_unreach_timer;
    struct timer_list reconf_timer;
    struct list_head transmitted;
    struct sctp_packet packet;
    struct list_head send_ready;
    struct (anon) cacc;
    __u64 hb_nonce;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct sctp_transport {
    struct list_head transports;
    struct rhlist_head node;
    refcount_t refcnt;
    __u32 rto_pending;
    __u32 hb_sent;
    __u32 pmtu_pending;
    __u32 dst_pending_confirm;
    __u32 sack_generation;
    u32 dst_cookie;
    struct flowi fl;
    union sctp_addr ipaddr;
    struct sctp_af *af_specific;
    struct sctp_association *asoc;
    long unsigned int rto;
    __u32 rtt;
    __u32 rttvar;
    __u32 srtt;
    __u32 cwnd;
    __u32 ssthresh;
    __u32 partial_bytes_acked;
    __u32 flight_size;
    __u32 burst_limited;
    struct dst_entry *dst;
    union sctp_addr saddr;
    long unsigned int hbinterval;
    long unsigned int sackdelay;
    __u32 sackfreq;
    atomic_t mtu_info;
    ktime_t last_time_heard;
    long unsigned int last_time_sent;
    long unsigned int last_time_ecne_reduced;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    int pf_retrans;
    __u32 pathmtu;
    __u32 param_flags;
    int init_sent_count;
    int state;
    short unsigned int error_count;
    struct timer_list T3_rtx_timer;
    struct timer_list hb_timer;
    struct timer_list proto_unreach_timer;
    struct timer_list reconf_timer;
    struct list_head transmitted;
    struct sctp_packet packet;
    struct list_head send_ready;
    struct (anon) cacc;
    __u64 hb_nonce;
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
<code>atomic_t mtu_info</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 flowlabel</code>
</li>
<li>
<b>Field added. </b>
<code>__u8 dscp</code>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u16 ps_retrans</code>
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
<b>Field added. </b>
<code>struct timer_list probe_timer</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) pl</code>
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
