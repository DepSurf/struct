# Struct: <code>sctp_sock</code>

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
struct sctp_sock {
    struct inet_sock inet;
    enum sctp_socket_type type;
    struct sctp_pf *pf;
    struct crypto_shash *hmac;
    char *sctp_hmac_alg;
    struct sctp_endpoint *ep;
    struct sctp_bind_bucket *bind_hash;
    __u16 default_stream;
    __u32 default_ppid;
    __u16 default_flags;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    int max_burst;
    __u32 hbinterval;
    __u16 pathmaxrxt;
    __u32 pathmtu;
    __u32 sackdelay;
    __u32 sackfreq;
    __u32 param_flags;
    struct sctp_rtoinfo rtoinfo;
    struct sctp_paddrparams paddrparam;
    struct sctp_assocparams assocparams;
    struct sctp_event_subscribe subscribe;
    struct sctp_initmsg initmsg;
    int user_frag;
    __u32 autoclose;
    __u32 adaptation_ind;
    __u32 pd_point;
    __u16 nodelay;
    __u16 disable_fragments;
    __u16 v4mapped;
    __u16 frag_interleave;
    __u16 strm_interleave;
    __u16 recvrcvinfo;
    __u16 recvnxtinfo;
    __u16 data_ready_signalled;
    atomic_t pd_mode;
    struct sk_buff_head pd_lobby;
    struct list_head auto_asconf_list;
    int do_auto_asconf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct sctp_sock {
    struct inet_sock inet;
    enum sctp_socket_type type;
    struct sctp_pf *pf;
    struct crypto_shash *hmac;
    char *sctp_hmac_alg;
    struct sctp_endpoint *ep;
    struct sctp_bind_bucket *bind_hash;
    __u16 default_stream;
    __u32 default_ppid;
    __u16 default_flags;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    int max_burst;
    __u32 hbinterval;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u32 pathmtu;
    __u32 sackdelay;
    __u32 sackfreq;
    __u32 param_flags;
    struct sctp_rtoinfo rtoinfo;
    struct sctp_paddrparams paddrparam;
    struct sctp_assocparams assocparams;
    __u16 subscribe;
    struct sctp_initmsg initmsg;
    int user_frag;
    __u32 autoclose;
    __u32 adaptation_ind;
    __u32 pd_point;
    __u16 nodelay;
    __u16 reuse;
    __u16 disable_fragments;
    __u16 v4mapped;
    __u16 frag_interleave;
    __u16 strm_interleave;
    __u16 recvrcvinfo;
    __u16 recvnxtinfo;
    __u16 data_ready_signalled;
    atomic_t pd_mode;
    struct sk_buff_head pd_lobby;
    struct list_head auto_asconf_list;
    int do_auto_asconf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct sctp_sock {
    struct inet_sock inet;
    enum sctp_socket_type type;
    struct sctp_pf *pf;
    struct crypto_shash *hmac;
    char *sctp_hmac_alg;
    struct sctp_endpoint *ep;
    struct sctp_bind_bucket *bind_hash;
    __u16 default_stream;
    __u32 default_ppid;
    __u16 default_flags;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    int max_burst;
    __u32 hbinterval;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    int pf_retrans;
    __u32 pathmtu;
    __u32 sackdelay;
    __u32 sackfreq;
    __u32 param_flags;
    __u32 default_ss;
    struct sctp_rtoinfo rtoinfo;
    struct sctp_paddrparams paddrparam;
    struct sctp_assocparams assocparams;
    __u16 subscribe;
    struct sctp_initmsg initmsg;
    int user_frag;
    __u32 autoclose;
    __u32 adaptation_ind;
    __u32 pd_point;
    __u16 nodelay;
    __u16 reuse;
    __u16 disable_fragments;
    __u16 v4mapped;
    __u16 frag_interleave;
    __u16 recvrcvinfo;
    __u16 recvnxtinfo;
    __u16 data_ready_signalled;
    atomic_t pd_mode;
    struct sk_buff_head pd_lobby;
    struct list_head auto_asconf_list;
    int do_auto_asconf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct sctp_sock {
    struct inet_sock inet;
    enum sctp_socket_type type;
    struct sctp_pf *pf;
    struct crypto_shash *hmac;
    char *sctp_hmac_alg;
    struct sctp_endpoint *ep;
    struct sctp_bind_bucket *bind_hash;
    __u16 default_stream;
    __u32 default_ppid;
    __u16 default_flags;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    int max_burst;
    __u32 hbinterval;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    int pf_retrans;
    __u32 pathmtu;
    __u32 sackdelay;
    __u32 sackfreq;
    __u32 param_flags;
    __u32 default_ss;
    struct sctp_rtoinfo rtoinfo;
    struct sctp_paddrparams paddrparam;
    struct sctp_assocparams assocparams;
    __u16 subscribe;
    struct sctp_initmsg initmsg;
    int user_frag;
    __u32 autoclose;
    __u32 adaptation_ind;
    __u32 pd_point;
    __u16 nodelay;
    __u16 reuse;
    __u16 disable_fragments;
    __u16 v4mapped;
    __u16 frag_interleave;
    __u16 recvrcvinfo;
    __u16 recvnxtinfo;
    __u16 data_ready_signalled;
    atomic_t pd_mode;
    struct sk_buff_head pd_lobby;
    struct list_head auto_asconf_list;
    int do_auto_asconf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct sctp_sock {
    struct inet_sock inet;
    enum sctp_socket_type type;
    struct sctp_pf *pf;
    struct crypto_shash *hmac;
    char *sctp_hmac_alg;
    struct sctp_endpoint *ep;
    struct sctp_bind_bucket *bind_hash;
    __u16 default_stream;
    __u32 default_ppid;
    __u16 default_flags;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    int max_burst;
    __u32 hbinterval;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u16 pf_retrans;
    __u16 ps_retrans;
    __u32 pathmtu;
    __u32 sackdelay;
    __u32 sackfreq;
    __u32 param_flags;
    __u32 default_ss;
    struct sctp_rtoinfo rtoinfo;
    struct sctp_paddrparams paddrparam;
    struct sctp_assocparams assocparams;
    __u16 subscribe;
    struct sctp_initmsg initmsg;
    int user_frag;
    __u32 autoclose;
    __u32 adaptation_ind;
    __u32 pd_point;
    __u16 nodelay;
    __u16 pf_expose;
    __u16 reuse;
    __u16 disable_fragments;
    __u16 v4mapped;
    __u16 frag_interleave;
    __u16 recvrcvinfo;
    __u16 recvnxtinfo;
    __u16 data_ready_signalled;
    atomic_t pd_mode;
    struct sk_buff_head pd_lobby;
    struct list_head auto_asconf_list;
    int do_auto_asconf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct sctp_sock {
    struct inet_sock inet;
    enum sctp_socket_type type;
    struct sctp_pf *pf;
    struct crypto_shash *hmac;
    char *sctp_hmac_alg;
    struct sctp_endpoint *ep;
    struct sctp_bind_bucket *bind_hash;
    __u16 default_stream;
    __u32 default_ppid;
    __u16 default_flags;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    int max_burst;
    __u32 hbinterval;
    __be16 udp_port;
    __be16 encap_port;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u16 pf_retrans;
    __u16 ps_retrans;
    __u32 pathmtu;
    __u32 sackdelay;
    __u32 sackfreq;
    __u32 param_flags;
    __u32 default_ss;
    struct sctp_rtoinfo rtoinfo;
    struct sctp_paddrparams paddrparam;
    struct sctp_assocparams assocparams;
    __u16 subscribe;
    struct sctp_initmsg initmsg;
    int user_frag;
    __u32 autoclose;
    __u32 adaptation_ind;
    __u32 pd_point;
    __u16 nodelay;
    __u16 pf_expose;
    __u16 reuse;
    __u16 disable_fragments;
    __u16 v4mapped;
    __u16 frag_interleave;
    __u16 recvrcvinfo;
    __u16 recvnxtinfo;
    __u16 data_ready_signalled;
    atomic_t pd_mode;
    struct sk_buff_head pd_lobby;
    struct list_head auto_asconf_list;
    int do_auto_asconf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct sctp_sock {
    struct inet_sock inet;
    enum sctp_socket_type type;
    struct sctp_pf *pf;
    struct crypto_shash *hmac;
    char *sctp_hmac_alg;
    struct sctp_endpoint *ep;
    struct sctp_bind_bucket *bind_hash;
    __u16 default_stream;
    __u32 default_ppid;
    __u16 default_flags;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    int max_burst;
    __u32 hbinterval;
    __be16 udp_port;
    __be16 encap_port;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u16 pf_retrans;
    __u16 ps_retrans;
    __u32 pathmtu;
    __u32 sackdelay;
    __u32 sackfreq;
    __u32 param_flags;
    __u32 default_ss;
    struct sctp_rtoinfo rtoinfo;
    struct sctp_paddrparams paddrparam;
    struct sctp_assocparams assocparams;
    __u16 subscribe;
    struct sctp_initmsg initmsg;
    int user_frag;
    __u32 autoclose;
    __u32 adaptation_ind;
    __u32 pd_point;
    __u16 nodelay;
    __u16 pf_expose;
    __u16 reuse;
    __u16 disable_fragments;
    __u16 v4mapped;
    __u16 frag_interleave;
    __u16 recvrcvinfo;
    __u16 recvnxtinfo;
    __u16 data_ready_signalled;
    atomic_t pd_mode;
    struct sk_buff_head pd_lobby;
    struct list_head auto_asconf_list;
    int do_auto_asconf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct sctp_sock {
    struct inet_sock inet;
    enum sctp_socket_type type;
    struct sctp_pf *pf;
    struct crypto_shash *hmac;
    char *sctp_hmac_alg;
    struct sctp_endpoint *ep;
    struct sctp_bind_bucket *bind_hash;
    __u16 default_stream;
    __u32 default_ppid;
    __u16 default_flags;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    int max_burst;
    __u32 hbinterval;
    __u32 probe_interval;
    __be16 udp_port;
    __be16 encap_port;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u16 pf_retrans;
    __u16 ps_retrans;
    __u32 pathmtu;
    __u32 sackdelay;
    __u32 sackfreq;
    __u32 param_flags;
    __u32 default_ss;
    struct sctp_rtoinfo rtoinfo;
    struct sctp_paddrparams paddrparam;
    struct sctp_assocparams assocparams;
    __u16 subscribe;
    struct sctp_initmsg initmsg;
    int user_frag;
    __u32 autoclose;
    __u32 adaptation_ind;
    __u32 pd_point;
    __u16 nodelay;
    __u16 pf_expose;
    __u16 reuse;
    __u16 disable_fragments;
    __u16 v4mapped;
    __u16 frag_interleave;
    __u16 recvrcvinfo;
    __u16 recvnxtinfo;
    __u16 data_ready_signalled;
    atomic_t pd_mode;
    struct sk_buff_head pd_lobby;
    struct list_head auto_asconf_list;
    int do_auto_asconf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct sctp_sock {
    struct inet_sock inet;
    enum sctp_socket_type type;
    struct sctp_pf *pf;
    struct crypto_shash *hmac;
    char *sctp_hmac_alg;
    struct sctp_endpoint *ep;
    struct sctp_bind_bucket *bind_hash;
    __u16 default_stream;
    __u32 default_ppid;
    __u16 default_flags;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    int max_burst;
    __u32 hbinterval;
    __u32 probe_interval;
    __be16 udp_port;
    __be16 encap_port;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u16 pf_retrans;
    __u16 ps_retrans;
    __u32 pathmtu;
    __u32 sackdelay;
    __u32 sackfreq;
    __u32 param_flags;
    __u32 default_ss;
    struct sctp_rtoinfo rtoinfo;
    struct sctp_paddrparams paddrparam;
    struct sctp_assocparams assocparams;
    __u16 subscribe;
    struct sctp_initmsg initmsg;
    int user_frag;
    __u32 autoclose;
    __u32 adaptation_ind;
    __u32 pd_point;
    __u16 nodelay;
    __u16 pf_expose;
    __u16 reuse;
    __u16 disable_fragments;
    __u16 v4mapped;
    __u16 frag_interleave;
    __u16 recvrcvinfo;
    __u16 recvnxtinfo;
    __u16 data_ready_signalled;
    atomic_t pd_mode;
    struct sk_buff_head pd_lobby;
    struct list_head auto_asconf_list;
    int do_auto_asconf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct sctp_sock {
    struct inet_sock inet;
    enum sctp_socket_type type;
    struct sctp_pf *pf;
    struct crypto_shash *hmac;
    char *sctp_hmac_alg;
    struct sctp_endpoint *ep;
    struct sctp_bind_bucket *bind_hash;
    __u16 default_stream;
    __u32 default_ppid;
    __u16 default_flags;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    int max_burst;
    __u32 hbinterval;
    __u32 probe_interval;
    __be16 udp_port;
    __be16 encap_port;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u16 pf_retrans;
    __u16 ps_retrans;
    __u32 pathmtu;
    __u32 sackdelay;
    __u32 sackfreq;
    __u32 param_flags;
    __u32 default_ss;
    struct sctp_rtoinfo rtoinfo;
    struct sctp_paddrparams paddrparam;
    struct sctp_assocparams assocparams;
    __u16 subscribe;
    struct sctp_initmsg initmsg;
    int user_frag;
    __u32 autoclose;
    __u32 adaptation_ind;
    __u32 pd_point;
    __u16 nodelay;
    __u16 pf_expose;
    __u16 reuse;
    __u16 disable_fragments;
    __u16 v4mapped;
    __u16 frag_interleave;
    __u16 recvrcvinfo;
    __u16 recvnxtinfo;
    __u16 data_ready_signalled;
    atomic_t pd_mode;
    struct sk_buff_head pd_lobby;
    struct list_head auto_asconf_list;
    int do_auto_asconf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct sctp_sock {
    struct inet_sock inet;
    enum sctp_socket_type type;
    struct sctp_pf *pf;
    struct crypto_shash *hmac;
    char *sctp_hmac_alg;
    struct sctp_endpoint *ep;
    struct sctp_bind_bucket *bind_hash;
    __u16 default_stream;
    __u32 default_ppid;
    __u16 default_flags;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    int max_burst;
    __u32 hbinterval;
    __u32 probe_interval;
    __be16 udp_port;
    __be16 encap_port;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u16 pf_retrans;
    __u16 ps_retrans;
    __u32 pathmtu;
    __u32 sackdelay;
    __u32 sackfreq;
    __u32 param_flags;
    __u32 default_ss;
    struct sctp_rtoinfo rtoinfo;
    struct sctp_paddrparams paddrparam;
    struct sctp_assocparams assocparams;
    __u16 subscribe;
    struct sctp_initmsg initmsg;
    int user_frag;
    __u32 autoclose;
    __u32 adaptation_ind;
    __u32 pd_point;
    __u16 nodelay;
    __u16 pf_expose;
    __u16 reuse;
    __u16 disable_fragments;
    __u16 v4mapped;
    __u16 frag_interleave;
    __u16 recvrcvinfo;
    __u16 recvnxtinfo;
    __u16 data_ready_signalled;
    atomic_t pd_mode;
    struct sk_buff_head pd_lobby;
    struct list_head auto_asconf_list;
    int do_auto_asconf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct sctp_sock {
    struct inet_sock inet;
    enum sctp_socket_type type;
    struct sctp_pf *pf;
    struct crypto_shash *hmac;
    char *sctp_hmac_alg;
    struct sctp_endpoint *ep;
    struct sctp_bind_bucket *bind_hash;
    __u16 default_stream;
    __u32 default_ppid;
    __u16 default_flags;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    int max_burst;
    __u32 hbinterval;
    __u32 probe_interval;
    __be16 udp_port;
    __be16 encap_port;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    __u16 pf_retrans;
    __u16 ps_retrans;
    __u32 pathmtu;
    __u32 sackdelay;
    __u32 sackfreq;
    __u32 param_flags;
    __u32 default_ss;
    struct sctp_rtoinfo rtoinfo;
    struct sctp_paddrparams paddrparam;
    struct sctp_assocparams assocparams;
    __u16 subscribe;
    struct sctp_initmsg initmsg;
    int user_frag;
    __u32 autoclose;
    __u32 adaptation_ind;
    __u32 pd_point;
    __u16 nodelay;
    __u16 pf_expose;
    __u16 reuse;
    __u16 disable_fragments;
    __u16 v4mapped;
    __u16 frag_interleave;
    __u16 recvrcvinfo;
    __u16 recvnxtinfo;
    __u16 data_ready_signalled;
    atomic_t pd_mode;
    struct sk_buff_head pd_lobby;
    struct list_head auto_asconf_list;
    int do_auto_asconf;
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
struct sctp_sock {
    struct inet_sock inet;
    enum sctp_socket_type type;
    struct sctp_pf *pf;
    struct crypto_shash *hmac;
    char *sctp_hmac_alg;
    struct sctp_endpoint *ep;
    struct sctp_bind_bucket *bind_hash;
    __u16 default_stream;
    __u32 default_ppid;
    __u16 default_flags;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    int max_burst;
    __u32 hbinterval;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    int pf_retrans;
    __u32 pathmtu;
    __u32 sackdelay;
    __u32 sackfreq;
    __u32 param_flags;
    __u32 default_ss;
    struct sctp_rtoinfo rtoinfo;
    struct sctp_paddrparams paddrparam;
    struct sctp_assocparams assocparams;
    __u16 subscribe;
    struct sctp_initmsg initmsg;
    int user_frag;
    __u32 autoclose;
    __u32 adaptation_ind;
    __u32 pd_point;
    __u16 nodelay;
    __u16 reuse;
    __u16 disable_fragments;
    __u16 v4mapped;
    __u16 frag_interleave;
    __u16 recvrcvinfo;
    __u16 recvnxtinfo;
    __u16 data_ready_signalled;
    atomic_t pd_mode;
    struct sk_buff_head pd_lobby;
    struct list_head auto_asconf_list;
    int do_auto_asconf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct sctp_sock {
    struct inet_sock inet;
    enum sctp_socket_type type;
    struct sctp_pf *pf;
    struct crypto_shash *hmac;
    char *sctp_hmac_alg;
    struct sctp_endpoint *ep;
    struct sctp_bind_bucket *bind_hash;
    __u16 default_stream;
    __u32 default_ppid;
    __u16 default_flags;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    int max_burst;
    __u32 hbinterval;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    int pf_retrans;
    __u32 pathmtu;
    __u32 sackdelay;
    __u32 sackfreq;
    __u32 param_flags;
    __u32 default_ss;
    struct sctp_rtoinfo rtoinfo;
    struct sctp_paddrparams paddrparam;
    struct sctp_assocparams assocparams;
    __u16 subscribe;
    struct sctp_initmsg initmsg;
    int user_frag;
    __u32 autoclose;
    __u32 adaptation_ind;
    __u32 pd_point;
    __u16 nodelay;
    __u16 reuse;
    __u16 disable_fragments;
    __u16 v4mapped;
    __u16 frag_interleave;
    __u16 recvrcvinfo;
    __u16 recvnxtinfo;
    __u16 data_ready_signalled;
    atomic_t pd_mode;
    struct sk_buff_head pd_lobby;
    struct list_head auto_asconf_list;
    int do_auto_asconf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct sctp_sock {
    struct inet_sock inet;
    enum sctp_socket_type type;
    struct sctp_pf *pf;
    struct crypto_shash *hmac;
    char *sctp_hmac_alg;
    struct sctp_endpoint *ep;
    struct sctp_bind_bucket *bind_hash;
    __u16 default_stream;
    __u32 default_ppid;
    __u16 default_flags;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    int max_burst;
    __u32 hbinterval;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    int pf_retrans;
    __u32 pathmtu;
    __u32 sackdelay;
    __u32 sackfreq;
    __u32 param_flags;
    __u32 default_ss;
    struct sctp_rtoinfo rtoinfo;
    struct sctp_paddrparams paddrparam;
    struct sctp_assocparams assocparams;
    __u16 subscribe;
    struct sctp_initmsg initmsg;
    int user_frag;
    __u32 autoclose;
    __u32 adaptation_ind;
    __u32 pd_point;
    __u16 nodelay;
    __u16 reuse;
    __u16 disable_fragments;
    __u16 v4mapped;
    __u16 frag_interleave;
    __u16 recvrcvinfo;
    __u16 recvnxtinfo;
    __u16 data_ready_signalled;
    atomic_t pd_mode;
    struct sk_buff_head pd_lobby;
    struct list_head auto_asconf_list;
    int do_auto_asconf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct sctp_sock {
    struct inet_sock inet;
    enum sctp_socket_type type;
    struct sctp_pf *pf;
    struct crypto_shash *hmac;
    char *sctp_hmac_alg;
    struct sctp_endpoint *ep;
    struct sctp_bind_bucket *bind_hash;
    __u16 default_stream;
    __u32 default_ppid;
    __u16 default_flags;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    int max_burst;
    __u32 hbinterval;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    int pf_retrans;
    __u32 pathmtu;
    __u32 sackdelay;
    __u32 sackfreq;
    __u32 param_flags;
    __u32 default_ss;
    struct sctp_rtoinfo rtoinfo;
    struct sctp_paddrparams paddrparam;
    struct sctp_assocparams assocparams;
    __u16 subscribe;
    struct sctp_initmsg initmsg;
    int user_frag;
    __u32 autoclose;
    __u32 adaptation_ind;
    __u32 pd_point;
    __u16 nodelay;
    __u16 reuse;
    __u16 disable_fragments;
    __u16 v4mapped;
    __u16 frag_interleave;
    __u16 recvrcvinfo;
    __u16 recvnxtinfo;
    __u16 data_ready_signalled;
    atomic_t pd_mode;
    struct sk_buff_head pd_lobby;
    struct list_head auto_asconf_list;
    int do_auto_asconf;
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
struct sctp_sock {
    struct inet_sock inet;
    enum sctp_socket_type type;
    struct sctp_pf *pf;
    struct crypto_shash *hmac;
    char *sctp_hmac_alg;
    struct sctp_endpoint *ep;
    struct sctp_bind_bucket *bind_hash;
    __u16 default_stream;
    __u32 default_ppid;
    __u16 default_flags;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    int max_burst;
    __u32 hbinterval;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    int pf_retrans;
    __u32 pathmtu;
    __u32 sackdelay;
    __u32 sackfreq;
    __u32 param_flags;
    __u32 default_ss;
    struct sctp_rtoinfo rtoinfo;
    struct sctp_paddrparams paddrparam;
    struct sctp_assocparams assocparams;
    __u16 subscribe;
    struct sctp_initmsg initmsg;
    int user_frag;
    __u32 autoclose;
    __u32 adaptation_ind;
    __u32 pd_point;
    __u16 nodelay;
    __u16 reuse;
    __u16 disable_fragments;
    __u16 v4mapped;
    __u16 frag_interleave;
    __u16 recvrcvinfo;
    __u16 recvnxtinfo;
    __u16 data_ready_signalled;
    atomic_t pd_mode;
    struct sk_buff_head pd_lobby;
    struct list_head auto_asconf_list;
    int do_auto_asconf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct sctp_sock {
    struct inet_sock inet;
    enum sctp_socket_type type;
    struct sctp_pf *pf;
    struct crypto_shash *hmac;
    char *sctp_hmac_alg;
    struct sctp_endpoint *ep;
    struct sctp_bind_bucket *bind_hash;
    __u16 default_stream;
    __u32 default_ppid;
    __u16 default_flags;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    int max_burst;
    __u32 hbinterval;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    int pf_retrans;
    __u32 pathmtu;
    __u32 sackdelay;
    __u32 sackfreq;
    __u32 param_flags;
    __u32 default_ss;
    struct sctp_rtoinfo rtoinfo;
    struct sctp_paddrparams paddrparam;
    struct sctp_assocparams assocparams;
    __u16 subscribe;
    struct sctp_initmsg initmsg;
    int user_frag;
    __u32 autoclose;
    __u32 adaptation_ind;
    __u32 pd_point;
    __u16 nodelay;
    __u16 reuse;
    __u16 disable_fragments;
    __u16 v4mapped;
    __u16 frag_interleave;
    __u16 recvrcvinfo;
    __u16 recvnxtinfo;
    __u16 data_ready_signalled;
    atomic_t pd_mode;
    struct sk_buff_head pd_lobby;
    struct list_head auto_asconf_list;
    int do_auto_asconf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct sctp_sock {
    struct inet_sock inet;
    enum sctp_socket_type type;
    struct sctp_pf *pf;
    struct crypto_shash *hmac;
    char *sctp_hmac_alg;
    struct sctp_endpoint *ep;
    struct sctp_bind_bucket *bind_hash;
    __u16 default_stream;
    __u32 default_ppid;
    __u16 default_flags;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    int max_burst;
    __u32 hbinterval;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    int pf_retrans;
    __u32 pathmtu;
    __u32 sackdelay;
    __u32 sackfreq;
    __u32 param_flags;
    __u32 default_ss;
    struct sctp_rtoinfo rtoinfo;
    struct sctp_paddrparams paddrparam;
    struct sctp_assocparams assocparams;
    __u16 subscribe;
    struct sctp_initmsg initmsg;
    int user_frag;
    __u32 autoclose;
    __u32 adaptation_ind;
    __u32 pd_point;
    __u16 nodelay;
    __u16 reuse;
    __u16 disable_fragments;
    __u16 v4mapped;
    __u16 frag_interleave;
    __u16 recvrcvinfo;
    __u16 recvnxtinfo;
    __u16 data_ready_signalled;
    atomic_t pd_mode;
    struct sk_buff_head pd_lobby;
    struct list_head auto_asconf_list;
    int do_auto_asconf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct sctp_sock {
    struct inet_sock inet;
    enum sctp_socket_type type;
    struct sctp_pf *pf;
    struct crypto_shash *hmac;
    char *sctp_hmac_alg;
    struct sctp_endpoint *ep;
    struct sctp_bind_bucket *bind_hash;
    __u16 default_stream;
    __u32 default_ppid;
    __u16 default_flags;
    __u32 default_context;
    __u32 default_timetolive;
    __u32 default_rcv_context;
    int max_burst;
    __u32 hbinterval;
    __u16 pathmaxrxt;
    __u32 flowlabel;
    __u8 dscp;
    int pf_retrans;
    __u32 pathmtu;
    __u32 sackdelay;
    __u32 sackfreq;
    __u32 param_flags;
    __u32 default_ss;
    struct sctp_rtoinfo rtoinfo;
    struct sctp_paddrparams paddrparam;
    struct sctp_assocparams assocparams;
    __u16 subscribe;
    struct sctp_initmsg initmsg;
    int user_frag;
    __u32 autoclose;
    __u32 adaptation_ind;
    __u32 pd_point;
    __u16 nodelay;
    __u16 reuse;
    __u16 disable_fragments;
    __u16 v4mapped;
    __u16 frag_interleave;
    __u16 recvrcvinfo;
    __u16 recvnxtinfo;
    __u16 data_ready_signalled;
    atomic_t pd_mode;
    struct sk_buff_head pd_lobby;
    struct list_head auto_asconf_list;
    int do_auto_asconf;
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
<code>__u16 reuse</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct sctp_event_subscribe subscribe</code> ➡️ <code>__u16 subscribe</code>
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
<code>int pf_retrans</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 default_ss</code>
</li>
<li>
<b>Field removed. </b>
<code>__u16 strm_interleave</code>
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
<code>__u16 pf_expose</code>
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
<code>__be16 udp_port</code>
</li>
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
<code>__u32 probe_interval</code>
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
