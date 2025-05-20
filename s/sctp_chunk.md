# Struct: <code>sctp_chunk</code>

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
struct sctp_chunk {
    struct list_head list;
    refcount_t refcnt;
    int sent_count;
    struct list_head transmitted_list;
    struct list_head stream_list;
    struct list_head frag_list;
    struct sk_buff *skb;
    struct sk_buff *head_skb;
    struct sctp_shared_key *shkey;
    union sctp_params param_hdr;
    union (anon) subh;
    __u8 *chunk_end;
    struct sctp_chunkhdr *chunk_hdr;
    struct sctphdr *sctp_hdr;
    struct sctp_sndrcvinfo sinfo;
    struct sctp_association *asoc;
    struct sctp_ep_common *rcvr;
    long unsigned int sent_at;
    union sctp_addr source;
    union sctp_addr dest;
    struct sctp_datamsg *msg;
    struct sctp_transport *transport;
    struct sk_buff *auth_chunk;
    __u16 rtt_in_progress;
    __u16 has_tsn;
    __u16 has_ssn;
    __u16 singleton;
    __u16 end_of_packet;
    __u16 ecn_ce_done;
    __u16 pdiscard;
    __u16 tsn_gap_acked;
    __u16 data_accepted;
    __u16 auth;
    __u16 has_asconf;
    __u16 tsn_missing_report;
    __u16 fast_retransmit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct sctp_chunk {
    struct list_head list;
    refcount_t refcnt;
    int sent_count;
    struct list_head transmitted_list;
    struct list_head stream_list;
    struct list_head frag_list;
    struct sk_buff *skb;
    struct sk_buff *head_skb;
    struct sctp_shared_key *shkey;
    union sctp_params param_hdr;
    union (anon) subh;
    __u8 *chunk_end;
    struct sctp_chunkhdr *chunk_hdr;
    struct sctphdr *sctp_hdr;
    struct sctp_sndrcvinfo sinfo;
    struct sctp_association *asoc;
    struct sctp_ep_common *rcvr;
    long unsigned int sent_at;
    union sctp_addr source;
    union sctp_addr dest;
    struct sctp_datamsg *msg;
    struct sctp_transport *transport;
    struct sk_buff *auth_chunk;
    __u16 rtt_in_progress;
    __u16 has_tsn;
    __u16 has_ssn;
    __u16 singleton;
    __u16 end_of_packet;
    __u16 ecn_ce_done;
    __u16 pdiscard;
    __u16 tsn_gap_acked;
    __u16 data_accepted;
    __u16 auth;
    __u16 has_asconf;
    __u16 tsn_missing_report;
    __u16 fast_retransmit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct sctp_chunk {
    struct list_head list;
    refcount_t refcnt;
    int sent_count;
    struct list_head transmitted_list;
    struct list_head stream_list;
    struct list_head frag_list;
    struct sk_buff *skb;
    struct sk_buff *head_skb;
    struct sctp_shared_key *shkey;
    union sctp_params param_hdr;
    union (anon) subh;
    __u8 *chunk_end;
    struct sctp_chunkhdr *chunk_hdr;
    struct sctphdr *sctp_hdr;
    struct sctp_sndrcvinfo sinfo;
    struct sctp_association *asoc;
    struct sctp_ep_common *rcvr;
    long unsigned int sent_at;
    union sctp_addr source;
    union sctp_addr dest;
    struct sctp_datamsg *msg;
    struct sctp_transport *transport;
    struct sk_buff *auth_chunk;
    __u16 rtt_in_progress;
    __u16 has_tsn;
    __u16 has_ssn;
    __u16 singleton;
    __u16 end_of_packet;
    __u16 ecn_ce_done;
    __u16 pdiscard;
    __u16 tsn_gap_acked;
    __u16 data_accepted;
    __u16 auth;
    __u16 has_asconf;
    __u16 tsn_missing_report;
    __u16 fast_retransmit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct sctp_chunk {
    struct list_head list;
    refcount_t refcnt;
    int sent_count;
    struct list_head transmitted_list;
    struct list_head stream_list;
    struct list_head frag_list;
    struct sk_buff *skb;
    struct sk_buff *head_skb;
    struct sctp_shared_key *shkey;
    union sctp_params param_hdr;
    union (anon) subh;
    __u8 *chunk_end;
    struct sctp_chunkhdr *chunk_hdr;
    struct sctphdr *sctp_hdr;
    struct sctp_sndrcvinfo sinfo;
    struct sctp_association *asoc;
    struct sctp_ep_common *rcvr;
    long unsigned int sent_at;
    union sctp_addr source;
    union sctp_addr dest;
    struct sctp_datamsg *msg;
    struct sctp_transport *transport;
    struct sk_buff *auth_chunk;
    __u16 rtt_in_progress;
    __u16 has_tsn;
    __u16 has_ssn;
    __u16 singleton;
    __u16 end_of_packet;
    __u16 ecn_ce_done;
    __u16 pdiscard;
    __u16 tsn_gap_acked;
    __u16 data_accepted;
    __u16 auth;
    __u16 has_asconf;
    __u16 tsn_missing_report;
    __u16 fast_retransmit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct sctp_chunk {
    struct list_head list;
    refcount_t refcnt;
    int sent_count;
    struct list_head transmitted_list;
    struct list_head stream_list;
    struct list_head frag_list;
    struct sk_buff *skb;
    struct sk_buff *head_skb;
    struct sctp_shared_key *shkey;
    union sctp_params param_hdr;
    union (anon) subh;
    __u8 *chunk_end;
    struct sctp_chunkhdr *chunk_hdr;
    struct sctphdr *sctp_hdr;
    struct sctp_sndrcvinfo sinfo;
    struct sctp_association *asoc;
    struct sctp_ep_common *rcvr;
    long unsigned int sent_at;
    union sctp_addr source;
    union sctp_addr dest;
    struct sctp_datamsg *msg;
    struct sctp_transport *transport;
    struct sk_buff *auth_chunk;
    __u16 rtt_in_progress;
    __u16 has_tsn;
    __u16 has_ssn;
    __u16 singleton;
    __u16 end_of_packet;
    __u16 ecn_ce_done;
    __u16 pdiscard;
    __u16 tsn_gap_acked;
    __u16 data_accepted;
    __u16 auth;
    __u16 has_asconf;
    __u16 tsn_missing_report;
    __u16 fast_retransmit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct sctp_chunk {
    struct list_head list;
    refcount_t refcnt;
    int sent_count;
    struct list_head transmitted_list;
    struct list_head stream_list;
    struct list_head frag_list;
    struct sk_buff *skb;
    struct sk_buff *head_skb;
    struct sctp_shared_key *shkey;
    union sctp_params param_hdr;
    union (anon) subh;
    __u8 *chunk_end;
    struct sctp_chunkhdr *chunk_hdr;
    struct sctphdr *sctp_hdr;
    struct sctp_sndrcvinfo sinfo;
    struct sctp_association *asoc;
    struct sctp_ep_common *rcvr;
    long unsigned int sent_at;
    union sctp_addr source;
    union sctp_addr dest;
    struct sctp_datamsg *msg;
    struct sctp_transport *transport;
    struct sk_buff *auth_chunk;
    __u16 rtt_in_progress;
    __u16 has_tsn;
    __u16 has_ssn;
    __u16 singleton;
    __u16 end_of_packet;
    __u16 ecn_ce_done;
    __u16 pdiscard;
    __u16 tsn_gap_acked;
    __u16 data_accepted;
    __u16 auth;
    __u16 has_asconf;
    __u16 tsn_missing_report;
    __u16 fast_retransmit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct sctp_chunk {
    struct list_head list;
    refcount_t refcnt;
    int sent_count;
    struct list_head transmitted_list;
    struct list_head stream_list;
    struct list_head frag_list;
    struct sk_buff *skb;
    struct sk_buff *head_skb;
    struct sctp_shared_key *shkey;
    union sctp_params param_hdr;
    union (anon) subh;
    __u8 *chunk_end;
    struct sctp_chunkhdr *chunk_hdr;
    struct sctphdr *sctp_hdr;
    struct sctp_sndrcvinfo sinfo;
    struct sctp_association *asoc;
    struct sctp_ep_common *rcvr;
    long unsigned int sent_at;
    union sctp_addr source;
    union sctp_addr dest;
    struct sctp_datamsg *msg;
    struct sctp_transport *transport;
    struct sk_buff *auth_chunk;
    __u16 rtt_in_progress;
    __u16 has_tsn;
    __u16 has_ssn;
    __u16 singleton;
    __u16 end_of_packet;
    __u16 ecn_ce_done;
    __u16 pdiscard;
    __u16 tsn_gap_acked;
    __u16 data_accepted;
    __u16 auth;
    __u16 has_asconf;
    __u16 tsn_missing_report;
    __u16 fast_retransmit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct sctp_chunk {
    struct list_head list;
    refcount_t refcnt;
    int sent_count;
    struct list_head transmitted_list;
    struct list_head stream_list;
    struct list_head frag_list;
    struct sk_buff *skb;
    struct sk_buff *head_skb;
    struct sctp_shared_key *shkey;
    union sctp_params param_hdr;
    union (anon) subh;
    __u8 *chunk_end;
    struct sctp_chunkhdr *chunk_hdr;
    struct sctphdr *sctp_hdr;
    struct sctp_sndrcvinfo sinfo;
    struct sctp_association *asoc;
    struct sctp_ep_common *rcvr;
    long unsigned int sent_at;
    union sctp_addr source;
    union sctp_addr dest;
    struct sctp_datamsg *msg;
    struct sctp_transport *transport;
    struct sk_buff *auth_chunk;
    __u16 rtt_in_progress;
    __u16 has_tsn;
    __u16 has_ssn;
    __u16 singleton;
    __u16 end_of_packet;
    __u16 ecn_ce_done;
    __u16 pdiscard;
    __u16 tsn_gap_acked;
    __u16 data_accepted;
    __u16 auth;
    __u16 has_asconf;
    __u16 pmtu_probe;
    __u16 tsn_missing_report;
    __u16 fast_retransmit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct sctp_chunk {
    struct list_head list;
    refcount_t refcnt;
    int sent_count;
    struct list_head transmitted_list;
    struct list_head stream_list;
    struct list_head frag_list;
    struct sk_buff *skb;
    struct sk_buff *head_skb;
    struct sctp_shared_key *shkey;
    union sctp_params param_hdr;
    union (anon) subh;
    __u8 *chunk_end;
    struct sctp_chunkhdr *chunk_hdr;
    struct sctphdr *sctp_hdr;
    struct sctp_sndrcvinfo sinfo;
    struct sctp_association *asoc;
    struct sctp_ep_common *rcvr;
    long unsigned int sent_at;
    union sctp_addr source;
    union sctp_addr dest;
    struct sctp_datamsg *msg;
    struct sctp_transport *transport;
    struct sk_buff *auth_chunk;
    __u16 rtt_in_progress;
    __u16 has_tsn;
    __u16 has_ssn;
    __u16 singleton;
    __u16 end_of_packet;
    __u16 ecn_ce_done;
    __u16 pdiscard;
    __u16 tsn_gap_acked;
    __u16 data_accepted;
    __u16 auth;
    __u16 has_asconf;
    __u16 pmtu_probe;
    __u16 tsn_missing_report;
    __u16 fast_retransmit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct sctp_chunk {
    struct list_head list;
    refcount_t refcnt;
    int sent_count;
    struct list_head transmitted_list;
    struct list_head stream_list;
    struct list_head frag_list;
    struct sk_buff *skb;
    struct sk_buff *head_skb;
    struct sctp_shared_key *shkey;
    union sctp_params param_hdr;
    union (anon) subh;
    __u8 *chunk_end;
    struct sctp_chunkhdr *chunk_hdr;
    struct sctphdr *sctp_hdr;
    struct sctp_sndrcvinfo sinfo;
    struct sctp_association *asoc;
    struct sctp_ep_common *rcvr;
    long unsigned int sent_at;
    union sctp_addr source;
    union sctp_addr dest;
    struct sctp_datamsg *msg;
    struct sctp_transport *transport;
    struct sk_buff *auth_chunk;
    __u16 rtt_in_progress;
    __u16 has_tsn;
    __u16 has_ssn;
    __u16 singleton;
    __u16 end_of_packet;
    __u16 ecn_ce_done;
    __u16 pdiscard;
    __u16 tsn_gap_acked;
    __u16 data_accepted;
    __u16 auth;
    __u16 has_asconf;
    __u16 pmtu_probe;
    __u16 tsn_missing_report;
    __u16 fast_retransmit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct sctp_chunk {
    struct list_head list;
    refcount_t refcnt;
    int sent_count;
    struct list_head transmitted_list;
    struct list_head stream_list;
    struct list_head frag_list;
    struct sk_buff *skb;
    struct sk_buff *head_skb;
    struct sctp_shared_key *shkey;
    union sctp_params param_hdr;
    union (anon) subh;
    __u8 *chunk_end;
    struct sctp_chunkhdr *chunk_hdr;
    struct sctphdr *sctp_hdr;
    struct sctp_sndrcvinfo sinfo;
    struct sctp_association *asoc;
    struct sctp_ep_common *rcvr;
    long unsigned int sent_at;
    union sctp_addr source;
    union sctp_addr dest;
    struct sctp_datamsg *msg;
    struct sctp_transport *transport;
    struct sk_buff *auth_chunk;
    __u16 rtt_in_progress;
    __u16 has_tsn;
    __u16 has_ssn;
    __u16 singleton;
    __u16 end_of_packet;
    __u16 ecn_ce_done;
    __u16 pdiscard;
    __u16 tsn_gap_acked;
    __u16 data_accepted;
    __u16 auth;
    __u16 has_asconf;
    __u16 pmtu_probe;
    __u16 tsn_missing_report;
    __u16 fast_retransmit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct sctp_chunk {
    struct list_head list;
    refcount_t refcnt;
    int sent_count;
    struct list_head transmitted_list;
    struct list_head stream_list;
    struct list_head frag_list;
    struct sk_buff *skb;
    struct sk_buff *head_skb;
    struct sctp_shared_key *shkey;
    union sctp_params param_hdr;
    union (anon) subh;
    __u8 *chunk_end;
    struct sctp_chunkhdr *chunk_hdr;
    struct sctphdr *sctp_hdr;
    struct sctp_sndrcvinfo sinfo;
    struct sctp_association *asoc;
    struct sctp_ep_common *rcvr;
    long unsigned int sent_at;
    union sctp_addr source;
    union sctp_addr dest;
    struct sctp_datamsg *msg;
    struct sctp_transport *transport;
    struct sk_buff *auth_chunk;
    __u16 rtt_in_progress;
    __u16 has_tsn;
    __u16 has_ssn;
    __u16 singleton;
    __u16 end_of_packet;
    __u16 ecn_ce_done;
    __u16 pdiscard;
    __u16 tsn_gap_acked;
    __u16 data_accepted;
    __u16 auth;
    __u16 has_asconf;
    __u16 pmtu_probe;
    __u16 tsn_missing_report;
    __u16 fast_retransmit;
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
struct sctp_chunk {
    struct list_head list;
    refcount_t refcnt;
    int sent_count;
    struct list_head transmitted_list;
    struct list_head stream_list;
    struct list_head frag_list;
    struct sk_buff *skb;
    struct sk_buff *head_skb;
    struct sctp_shared_key *shkey;
    union sctp_params param_hdr;
    union (anon) subh;
    __u8 *chunk_end;
    struct sctp_chunkhdr *chunk_hdr;
    struct sctphdr *sctp_hdr;
    struct sctp_sndrcvinfo sinfo;
    struct sctp_association *asoc;
    struct sctp_ep_common *rcvr;
    long unsigned int sent_at;
    union sctp_addr source;
    union sctp_addr dest;
    struct sctp_datamsg *msg;
    struct sctp_transport *transport;
    struct sk_buff *auth_chunk;
    __u16 rtt_in_progress;
    __u16 has_tsn;
    __u16 has_ssn;
    __u16 singleton;
    __u16 end_of_packet;
    __u16 ecn_ce_done;
    __u16 pdiscard;
    __u16 tsn_gap_acked;
    __u16 data_accepted;
    __u16 auth;
    __u16 has_asconf;
    __u16 tsn_missing_report;
    __u16 fast_retransmit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct sctp_chunk {
    struct list_head list;
    refcount_t refcnt;
    int sent_count;
    struct list_head transmitted_list;
    struct list_head stream_list;
    struct list_head frag_list;
    struct sk_buff *skb;
    struct sk_buff *head_skb;
    struct sctp_shared_key *shkey;
    union sctp_params param_hdr;
    union (anon) subh;
    __u8 *chunk_end;
    struct sctp_chunkhdr *chunk_hdr;
    struct sctphdr *sctp_hdr;
    struct sctp_sndrcvinfo sinfo;
    struct sctp_association *asoc;
    struct sctp_ep_common *rcvr;
    long unsigned int sent_at;
    union sctp_addr source;
    union sctp_addr dest;
    struct sctp_datamsg *msg;
    struct sctp_transport *transport;
    struct sk_buff *auth_chunk;
    __u16 rtt_in_progress;
    __u16 has_tsn;
    __u16 has_ssn;
    __u16 singleton;
    __u16 end_of_packet;
    __u16 ecn_ce_done;
    __u16 pdiscard;
    __u16 tsn_gap_acked;
    __u16 data_accepted;
    __u16 auth;
    __u16 has_asconf;
    __u16 tsn_missing_report;
    __u16 fast_retransmit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct sctp_chunk {
    struct list_head list;
    refcount_t refcnt;
    int sent_count;
    struct list_head transmitted_list;
    struct list_head stream_list;
    struct list_head frag_list;
    struct sk_buff *skb;
    struct sk_buff *head_skb;
    struct sctp_shared_key *shkey;
    union sctp_params param_hdr;
    union (anon) subh;
    __u8 *chunk_end;
    struct sctp_chunkhdr *chunk_hdr;
    struct sctphdr *sctp_hdr;
    struct sctp_sndrcvinfo sinfo;
    struct sctp_association *asoc;
    struct sctp_ep_common *rcvr;
    long unsigned int sent_at;
    union sctp_addr source;
    union sctp_addr dest;
    struct sctp_datamsg *msg;
    struct sctp_transport *transport;
    struct sk_buff *auth_chunk;
    __u16 rtt_in_progress;
    __u16 has_tsn;
    __u16 has_ssn;
    __u16 singleton;
    __u16 end_of_packet;
    __u16 ecn_ce_done;
    __u16 pdiscard;
    __u16 tsn_gap_acked;
    __u16 data_accepted;
    __u16 auth;
    __u16 has_asconf;
    __u16 tsn_missing_report;
    __u16 fast_retransmit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct sctp_chunk {
    struct list_head list;
    refcount_t refcnt;
    int sent_count;
    struct list_head transmitted_list;
    struct list_head stream_list;
    struct list_head frag_list;
    struct sk_buff *skb;
    struct sk_buff *head_skb;
    struct sctp_shared_key *shkey;
    union sctp_params param_hdr;
    union (anon) subh;
    __u8 *chunk_end;
    struct sctp_chunkhdr *chunk_hdr;
    struct sctphdr *sctp_hdr;
    struct sctp_sndrcvinfo sinfo;
    struct sctp_association *asoc;
    struct sctp_ep_common *rcvr;
    long unsigned int sent_at;
    union sctp_addr source;
    union sctp_addr dest;
    struct sctp_datamsg *msg;
    struct sctp_transport *transport;
    struct sk_buff *auth_chunk;
    __u16 rtt_in_progress;
    __u16 has_tsn;
    __u16 has_ssn;
    __u16 singleton;
    __u16 end_of_packet;
    __u16 ecn_ce_done;
    __u16 pdiscard;
    __u16 tsn_gap_acked;
    __u16 data_accepted;
    __u16 auth;
    __u16 has_asconf;
    __u16 tsn_missing_report;
    __u16 fast_retransmit;
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
struct sctp_chunk {
    struct list_head list;
    refcount_t refcnt;
    int sent_count;
    struct list_head transmitted_list;
    struct list_head stream_list;
    struct list_head frag_list;
    struct sk_buff *skb;
    struct sk_buff *head_skb;
    struct sctp_shared_key *shkey;
    union sctp_params param_hdr;
    union (anon) subh;
    __u8 *chunk_end;
    struct sctp_chunkhdr *chunk_hdr;
    struct sctphdr *sctp_hdr;
    struct sctp_sndrcvinfo sinfo;
    struct sctp_association *asoc;
    struct sctp_ep_common *rcvr;
    long unsigned int sent_at;
    union sctp_addr source;
    union sctp_addr dest;
    struct sctp_datamsg *msg;
    struct sctp_transport *transport;
    struct sk_buff *auth_chunk;
    __u16 rtt_in_progress;
    __u16 has_tsn;
    __u16 has_ssn;
    __u16 singleton;
    __u16 end_of_packet;
    __u16 ecn_ce_done;
    __u16 pdiscard;
    __u16 tsn_gap_acked;
    __u16 data_accepted;
    __u16 auth;
    __u16 has_asconf;
    __u16 tsn_missing_report;
    __u16 fast_retransmit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct sctp_chunk {
    struct list_head list;
    refcount_t refcnt;
    int sent_count;
    struct list_head transmitted_list;
    struct list_head stream_list;
    struct list_head frag_list;
    struct sk_buff *skb;
    struct sk_buff *head_skb;
    struct sctp_shared_key *shkey;
    union sctp_params param_hdr;
    union (anon) subh;
    __u8 *chunk_end;
    struct sctp_chunkhdr *chunk_hdr;
    struct sctphdr *sctp_hdr;
    struct sctp_sndrcvinfo sinfo;
    struct sctp_association *asoc;
    struct sctp_ep_common *rcvr;
    long unsigned int sent_at;
    union sctp_addr source;
    union sctp_addr dest;
    struct sctp_datamsg *msg;
    struct sctp_transport *transport;
    struct sk_buff *auth_chunk;
    __u16 rtt_in_progress;
    __u16 has_tsn;
    __u16 has_ssn;
    __u16 singleton;
    __u16 end_of_packet;
    __u16 ecn_ce_done;
    __u16 pdiscard;
    __u16 tsn_gap_acked;
    __u16 data_accepted;
    __u16 auth;
    __u16 has_asconf;
    __u16 tsn_missing_report;
    __u16 fast_retransmit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct sctp_chunk {
    struct list_head list;
    refcount_t refcnt;
    int sent_count;
    struct list_head transmitted_list;
    struct list_head stream_list;
    struct list_head frag_list;
    struct sk_buff *skb;
    struct sk_buff *head_skb;
    struct sctp_shared_key *shkey;
    union sctp_params param_hdr;
    union (anon) subh;
    __u8 *chunk_end;
    struct sctp_chunkhdr *chunk_hdr;
    struct sctphdr *sctp_hdr;
    struct sctp_sndrcvinfo sinfo;
    struct sctp_association *asoc;
    struct sctp_ep_common *rcvr;
    long unsigned int sent_at;
    union sctp_addr source;
    union sctp_addr dest;
    struct sctp_datamsg *msg;
    struct sctp_transport *transport;
    struct sk_buff *auth_chunk;
    __u16 rtt_in_progress;
    __u16 has_tsn;
    __u16 has_ssn;
    __u16 singleton;
    __u16 end_of_packet;
    __u16 ecn_ce_done;
    __u16 pdiscard;
    __u16 tsn_gap_acked;
    __u16 data_accepted;
    __u16 auth;
    __u16 has_asconf;
    __u16 tsn_missing_report;
    __u16 fast_retransmit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct sctp_chunk {
    struct list_head list;
    refcount_t refcnt;
    int sent_count;
    struct list_head transmitted_list;
    struct list_head stream_list;
    struct list_head frag_list;
    struct sk_buff *skb;
    struct sk_buff *head_skb;
    struct sctp_shared_key *shkey;
    union sctp_params param_hdr;
    union (anon) subh;
    __u8 *chunk_end;
    struct sctp_chunkhdr *chunk_hdr;
    struct sctphdr *sctp_hdr;
    struct sctp_sndrcvinfo sinfo;
    struct sctp_association *asoc;
    struct sctp_ep_common *rcvr;
    long unsigned int sent_at;
    union sctp_addr source;
    union sctp_addr dest;
    struct sctp_datamsg *msg;
    struct sctp_transport *transport;
    struct sk_buff *auth_chunk;
    __u16 rtt_in_progress;
    __u16 has_tsn;
    __u16 has_ssn;
    __u16 singleton;
    __u16 end_of_packet;
    __u16 ecn_ce_done;
    __u16 pdiscard;
    __u16 tsn_gap_acked;
    __u16 data_accepted;
    __u16 auth;
    __u16 has_asconf;
    __u16 tsn_missing_report;
    __u16 fast_retransmit;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
No changes between <code>5.8</code> and <code>5.11</code> ✅
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
<code>__u16 pmtu_probe</code>
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
