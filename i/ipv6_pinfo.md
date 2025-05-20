# Struct: <code>ipv6_pinfo</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct ipv6_pinfo {
    struct in6_addr saddr;
    struct in6_pktinfo sticky_pktinfo;
    const struct in6_addr *daddr_cache;
    const struct in6_addr *saddr_cache;
    __be32 flow_label;
    __u32 frag_size;
    __u16 __unused_1;
    __s16 hop_limit;
    __u16 mc_loop;
    __u16 __unused_2;
    __s16 mcast_hops;
    int ucast_oif;
    int mcast_oif;
    union (anon) rxopt;
    __u16 recverr;
    __u16 sndflow;
    __u16 repflow;
    __u16 pmtudisc;
    __u16 padding;
    __u16 srcprefs;
    __u16 dontfrag;
    __u16 autoflowlabel;
    __u8 min_hopcount;
    __u8 tclass;
    __be32 rcv_flowinfo;
    __u32 dst_cookie;
    __u32 rx_dst_cookie;
    struct ipv6_mc_socklist *ipv6_mc_list;
    struct ipv6_ac_socklist *ipv6_ac_list;
    struct ipv6_fl_socklist *ipv6_fl_list;
    struct ipv6_txoptions *opt;
    struct sk_buff *pktoptions;
    struct sk_buff *rxpmtu;
    struct inet6_cork cork;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ipv6_pinfo {
    struct in6_addr saddr;
    struct in6_pktinfo sticky_pktinfo;
    const struct in6_addr *daddr_cache;
    const struct in6_addr *saddr_cache;
    __be32 flow_label;
    __u32 frag_size;
    __u16 __unused_1;
    __s16 hop_limit;
    __u16 mc_loop;
    __u16 __unused_2;
    __s16 mcast_hops;
    int ucast_oif;
    int mcast_oif;
    union (anon) rxopt;
    __u16 recverr;
    __u16 sndflow;
    __u16 repflow;
    __u16 pmtudisc;
    __u16 padding;
    __u16 srcprefs;
    __u16 dontfrag;
    __u16 autoflowlabel;
    __u8 min_hopcount;
    __u8 tclass;
    __be32 rcv_flowinfo;
    __u32 dst_cookie;
    __u32 rx_dst_cookie;
    struct ipv6_mc_socklist *ipv6_mc_list;
    struct ipv6_ac_socklist *ipv6_ac_list;
    struct ipv6_fl_socklist *ipv6_fl_list;
    struct ipv6_txoptions *opt;
    struct sk_buff *pktoptions;
    struct sk_buff *rxpmtu;
    struct inet6_cork cork;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ipv6_pinfo {
    struct in6_addr saddr;
    struct in6_pktinfo sticky_pktinfo;
    const struct in6_addr *daddr_cache;
    const struct in6_addr *saddr_cache;
    __be32 flow_label;
    __u32 frag_size;
    __u16 __unused_1;
    __s16 hop_limit;
    __u16 mc_loop;
    __u16 __unused_2;
    __s16 mcast_hops;
    int ucast_oif;
    int mcast_oif;
    union (anon) rxopt;
    __u16 recverr;
    __u16 sndflow;
    __u16 repflow;
    __u16 pmtudisc;
    __u16 padding;
    __u16 srcprefs;
    __u16 dontfrag;
    __u16 autoflowlabel;
    __u8 min_hopcount;
    __u8 tclass;
    __be32 rcv_flowinfo;
    __u32 dst_cookie;
    __u32 rx_dst_cookie;
    struct ipv6_mc_socklist *ipv6_mc_list;
    struct ipv6_ac_socklist *ipv6_ac_list;
    struct ipv6_fl_socklist *ipv6_fl_list;
    struct ipv6_txoptions *opt;
    struct sk_buff *pktoptions;
    struct sk_buff *rxpmtu;
    struct inet6_cork cork;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ipv6_pinfo {
    struct in6_addr saddr;
    struct in6_pktinfo sticky_pktinfo;
    const struct in6_addr *daddr_cache;
    const struct in6_addr *saddr_cache;
    __be32 flow_label;
    __u32 frag_size;
    __u16 __unused_1;
    __s16 hop_limit;
    __u16 mc_loop;
    __u16 __unused_2;
    __s16 mcast_hops;
    int ucast_oif;
    int mcast_oif;
    union (anon) rxopt;
    __u16 recverr;
    __u16 sndflow;
    __u16 repflow;
    __u16 pmtudisc;
    __u16 padding;
    __u16 srcprefs;
    __u16 dontfrag;
    __u16 autoflowlabel;
    __u8 min_hopcount;
    __u8 tclass;
    __be32 rcv_flowinfo;
    __u32 dst_cookie;
    __u32 rx_dst_cookie;
    struct ipv6_mc_socklist *ipv6_mc_list;
    struct ipv6_ac_socklist *ipv6_ac_list;
    struct ipv6_fl_socklist *ipv6_fl_list;
    struct ipv6_txoptions *opt;
    struct sk_buff *pktoptions;
    struct sk_buff *rxpmtu;
    struct inet6_cork cork;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ipv6_pinfo {
    struct in6_addr saddr;
    struct in6_pktinfo sticky_pktinfo;
    const struct in6_addr *daddr_cache;
    const struct in6_addr *saddr_cache;
    __be32 flow_label;
    __u32 frag_size;
    __u16 __unused_1;
    __s16 hop_limit;
    __u16 mc_loop;
    __u16 __unused_2;
    __s16 mcast_hops;
    int ucast_oif;
    int mcast_oif;
    union (anon) rxopt;
    __u16 recverr;
    __u16 sndflow;
    __u16 repflow;
    __u16 pmtudisc;
    __u16 padding;
    __u16 srcprefs;
    __u16 dontfrag;
    __u16 autoflowlabel;
    __u16 autoflowlabel_set;
    __u8 min_hopcount;
    __u8 tclass;
    __be32 rcv_flowinfo;
    __u32 dst_cookie;
    __u32 rx_dst_cookie;
    struct ipv6_mc_socklist *ipv6_mc_list;
    struct ipv6_ac_socklist *ipv6_ac_list;
    struct ipv6_fl_socklist *ipv6_fl_list;
    struct ipv6_txoptions *opt;
    struct sk_buff *pktoptions;
    struct sk_buff *rxpmtu;
    struct inet6_cork cork;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ipv6_pinfo {
    struct in6_addr saddr;
    struct in6_pktinfo sticky_pktinfo;
    const struct in6_addr *daddr_cache;
    const struct in6_addr *saddr_cache;
    __be32 flow_label;
    __u32 frag_size;
    __u16 __unused_1;
    __s16 hop_limit;
    __u16 mc_loop;
    __u16 __unused_2;
    __s16 mcast_hops;
    int ucast_oif;
    int mcast_oif;
    union (anon) rxopt;
    __u16 recverr;
    __u16 sndflow;
    __u16 repflow;
    __u16 pmtudisc;
    __u16 padding;
    __u16 srcprefs;
    __u16 dontfrag;
    __u16 autoflowlabel;
    __u16 autoflowlabel_set;
    __u8 min_hopcount;
    __u8 tclass;
    __be32 rcv_flowinfo;
    __u32 dst_cookie;
    __u32 rx_dst_cookie;
    struct ipv6_mc_socklist *ipv6_mc_list;
    struct ipv6_ac_socklist *ipv6_ac_list;
    struct ipv6_fl_socklist *ipv6_fl_list;
    struct ipv6_txoptions *opt;
    struct sk_buff *pktoptions;
    struct sk_buff *rxpmtu;
    struct inet6_cork cork;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ipv6_pinfo {
    struct in6_addr saddr;
    struct in6_pktinfo sticky_pktinfo;
    const struct in6_addr *daddr_cache;
    const struct in6_addr *saddr_cache;
    __be32 flow_label;
    __u32 frag_size;
    __u16 __unused_1;
    __s16 hop_limit;
    __u16 mc_loop;
    __u16 __unused_2;
    __s16 mcast_hops;
    int ucast_oif;
    int mcast_oif;
    union (anon) rxopt;
    __u16 recverr;
    __u16 sndflow;
    __u16 repflow;
    __u16 pmtudisc;
    __u16 padding;
    __u16 srcprefs;
    __u16 dontfrag;
    __u16 autoflowlabel;
    __u16 autoflowlabel_set;
    __u16 mc_all;
    __u8 min_hopcount;
    __u8 tclass;
    __be32 rcv_flowinfo;
    __u32 dst_cookie;
    __u32 rx_dst_cookie;
    struct ipv6_mc_socklist *ipv6_mc_list;
    struct ipv6_ac_socklist *ipv6_ac_list;
    struct ipv6_fl_socklist *ipv6_fl_list;
    struct ipv6_txoptions *opt;
    struct sk_buff *pktoptions;
    struct sk_buff *rxpmtu;
    struct inet6_cork cork;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ipv6_pinfo {
    struct in6_addr saddr;
    struct in6_pktinfo sticky_pktinfo;
    const struct in6_addr *daddr_cache;
    const struct in6_addr *saddr_cache;
    __be32 flow_label;
    __u32 frag_size;
    __u16 __unused_1;
    __s16 hop_limit;
    __u16 mc_loop;
    __u16 __unused_2;
    __s16 mcast_hops;
    int ucast_oif;
    int mcast_oif;
    union (anon) rxopt;
    __u16 recverr;
    __u16 sndflow;
    __u16 repflow;
    __u16 pmtudisc;
    __u16 padding;
    __u16 srcprefs;
    __u16 dontfrag;
    __u16 autoflowlabel;
    __u16 autoflowlabel_set;
    __u16 mc_all;
    __u16 rtalert_isolate;
    __u8 min_hopcount;
    __u8 tclass;
    __be32 rcv_flowinfo;
    __u32 dst_cookie;
    __u32 rx_dst_cookie;
    struct ipv6_mc_socklist *ipv6_mc_list;
    struct ipv6_ac_socklist *ipv6_ac_list;
    struct ipv6_fl_socklist *ipv6_fl_list;
    struct ipv6_txoptions *opt;
    struct sk_buff *pktoptions;
    struct sk_buff *rxpmtu;
    struct inet6_cork cork;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ipv6_pinfo {
    struct in6_addr saddr;
    struct in6_pktinfo sticky_pktinfo;
    const struct in6_addr *daddr_cache;
    const struct in6_addr *saddr_cache;
    __be32 flow_label;
    __u32 frag_size;
    __u16 __unused_1;
    __s16 hop_limit;
    __u16 mc_loop;
    __u16 __unused_2;
    __s16 mcast_hops;
    int ucast_oif;
    int mcast_oif;
    union (anon) rxopt;
    __u16 recverr;
    __u16 sndflow;
    __u16 repflow;
    __u16 pmtudisc;
    __u16 padding;
    __u16 srcprefs;
    __u16 dontfrag;
    __u16 autoflowlabel;
    __u16 autoflowlabel_set;
    __u16 mc_all;
    __u16 rtalert_isolate;
    __u8 min_hopcount;
    __u8 tclass;
    __be32 rcv_flowinfo;
    __u32 dst_cookie;
    __u32 rx_dst_cookie;
    struct ipv6_mc_socklist *ipv6_mc_list;
    struct ipv6_ac_socklist *ipv6_ac_list;
    struct ipv6_fl_socklist *ipv6_fl_list;
    struct ipv6_txoptions *opt;
    struct sk_buff *pktoptions;
    struct sk_buff *rxpmtu;
    struct inet6_cork cork;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ipv6_pinfo {
    struct in6_addr saddr;
    struct in6_pktinfo sticky_pktinfo;
    const struct in6_addr *daddr_cache;
    const struct in6_addr *saddr_cache;
    __be32 flow_label;
    __u32 frag_size;
    __u16 __unused_1;
    __s16 hop_limit;
    __u16 mc_loop;
    __u16 __unused_2;
    __s16 mcast_hops;
    int ucast_oif;
    int mcast_oif;
    union (anon) rxopt;
    __u16 recverr;
    __u16 sndflow;
    __u16 repflow;
    __u16 pmtudisc;
    __u16 padding;
    __u16 srcprefs;
    __u16 dontfrag;
    __u16 autoflowlabel;
    __u16 autoflowlabel_set;
    __u16 mc_all;
    __u16 rtalert_isolate;
    __u8 min_hopcount;
    __u8 tclass;
    __be32 rcv_flowinfo;
    __u32 dst_cookie;
    __u32 rx_dst_cookie;
    struct ipv6_mc_socklist *ipv6_mc_list;
    struct ipv6_ac_socklist *ipv6_ac_list;
    struct ipv6_fl_socklist *ipv6_fl_list;
    struct ipv6_txoptions *opt;
    struct sk_buff *pktoptions;
    struct sk_buff *rxpmtu;
    struct inet6_cork cork;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ipv6_pinfo {
    struct in6_addr saddr;
    struct in6_pktinfo sticky_pktinfo;
    const struct in6_addr *daddr_cache;
    const struct in6_addr *saddr_cache;
    __be32 flow_label;
    __u32 frag_size;
    __u16 __unused_1;
    __s16 hop_limit;
    __u16 mc_loop;
    __u16 __unused_2;
    __s16 mcast_hops;
    int ucast_oif;
    int mcast_oif;
    union (anon) rxopt;
    __u16 recverr;
    __u16 sndflow;
    __u16 repflow;
    __u16 pmtudisc;
    __u16 padding;
    __u16 srcprefs;
    __u16 dontfrag;
    __u16 autoflowlabel;
    __u16 autoflowlabel_set;
    __u16 mc_all;
    __u16 recverr_rfc4884;
    __u16 rtalert_isolate;
    __u8 min_hopcount;
    __u8 tclass;
    __be32 rcv_flowinfo;
    __u32 dst_cookie;
    __u32 rx_dst_cookie;
    struct ipv6_mc_socklist *ipv6_mc_list;
    struct ipv6_ac_socklist *ipv6_ac_list;
    struct ipv6_fl_socklist *ipv6_fl_list;
    struct ipv6_txoptions *opt;
    struct sk_buff *pktoptions;
    struct sk_buff *rxpmtu;
    struct inet6_cork cork;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ipv6_pinfo {
    struct in6_addr saddr;
    struct in6_pktinfo sticky_pktinfo;
    const struct in6_addr *daddr_cache;
    const struct in6_addr *saddr_cache;
    __be32 flow_label;
    __u32 frag_size;
    __u16 __unused_1;
    __s16 hop_limit;
    __u16 mc_loop;
    __u16 __unused_2;
    __s16 mcast_hops;
    int ucast_oif;
    int mcast_oif;
    union (anon) rxopt;
    __u16 recverr;
    __u16 sndflow;
    __u16 repflow;
    __u16 pmtudisc;
    __u16 padding;
    __u16 srcprefs;
    __u16 dontfrag;
    __u16 autoflowlabel;
    __u16 autoflowlabel_set;
    __u16 mc_all;
    __u16 recverr_rfc4884;
    __u16 rtalert_isolate;
    __u8 min_hopcount;
    __u8 tclass;
    __be32 rcv_flowinfo;
    __u32 dst_cookie;
    __u32 rx_dst_cookie;
    struct ipv6_mc_socklist *ipv6_mc_list;
    struct ipv6_ac_socklist *ipv6_ac_list;
    struct ipv6_fl_socklist *ipv6_fl_list;
    struct ipv6_txoptions *opt;
    struct sk_buff *pktoptions;
    struct sk_buff *rxpmtu;
    struct inet6_cork cork;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ipv6_pinfo {
    struct in6_addr saddr;
    struct in6_pktinfo sticky_pktinfo;
    const struct in6_addr *daddr_cache;
    const struct in6_addr *saddr_cache;
    __be32 flow_label;
    __u32 frag_size;
    __u16 __unused_1;
    __s16 hop_limit;
    __u16 mc_loop;
    __u16 __unused_2;
    __s16 mcast_hops;
    int ucast_oif;
    int mcast_oif;
    union (anon) rxopt;
    __u16 recverr;
    __u16 sndflow;
    __u16 repflow;
    __u16 pmtudisc;
    __u16 padding;
    __u16 srcprefs;
    __u16 dontfrag;
    __u16 autoflowlabel;
    __u16 autoflowlabel_set;
    __u16 mc_all;
    __u16 recverr_rfc4884;
    __u16 rtalert_isolate;
    __u8 min_hopcount;
    __u8 tclass;
    __be32 rcv_flowinfo;
    __u32 dst_cookie;
    struct ipv6_mc_socklist *ipv6_mc_list;
    struct ipv6_ac_socklist *ipv6_ac_list;
    struct ipv6_fl_socklist *ipv6_fl_list;
    struct ipv6_txoptions *opt;
    struct sk_buff *pktoptions;
    struct sk_buff *rxpmtu;
    struct inet6_cork cork;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ipv6_pinfo {
    struct in6_addr saddr;
    struct in6_pktinfo sticky_pktinfo;
    const struct in6_addr *daddr_cache;
    const struct in6_addr *saddr_cache;
    __be32 flow_label;
    __u32 frag_size;
    __u16 __unused_1;
    __s16 hop_limit;
    __u16 mc_loop;
    __u16 __unused_2;
    __s16 mcast_hops;
    int ucast_oif;
    int mcast_oif;
    union (anon) rxopt;
    __u16 recverr;
    __u16 sndflow;
    __u16 repflow;
    __u16 pmtudisc;
    __u16 padding;
    __u16 srcprefs;
    __u16 dontfrag;
    __u16 autoflowlabel;
    __u16 autoflowlabel_set;
    __u16 mc_all;
    __u16 recverr_rfc4884;
    __u16 rtalert_isolate;
    __u8 min_hopcount;
    __u8 tclass;
    __be32 rcv_flowinfo;
    __u32 dst_cookie;
    struct ipv6_mc_socklist *ipv6_mc_list;
    struct ipv6_ac_socklist *ipv6_ac_list;
    struct ipv6_fl_socklist *ipv6_fl_list;
    struct ipv6_txoptions *opt;
    struct sk_buff *pktoptions;
    struct sk_buff *rxpmtu;
    struct inet6_cork cork;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ipv6_pinfo {
    struct in6_addr saddr;
    struct in6_pktinfo sticky_pktinfo;
    const struct in6_addr *daddr_cache;
    const struct in6_addr *saddr_cache;
    __be32 flow_label;
    __u32 frag_size;
    __u16 __unused_1;
    __s16 hop_limit;
    __u16 mc_loop;
    __u16 __unused_2;
    __s16 mcast_hops;
    int ucast_oif;
    int mcast_oif;
    union (anon) rxopt;
    __u16 recverr;
    __u16 sndflow;
    __u16 repflow;
    __u16 pmtudisc;
    __u16 padding;
    __u16 srcprefs;
    __u16 dontfrag;
    __u16 autoflowlabel;
    __u16 autoflowlabel_set;
    __u16 mc_all;
    __u16 recverr_rfc4884;
    __u16 rtalert_isolate;
    __u8 min_hopcount;
    __u8 tclass;
    __be32 rcv_flowinfo;
    __u32 dst_cookie;
    struct ipv6_mc_socklist *ipv6_mc_list;
    struct ipv6_ac_socklist *ipv6_ac_list;
    struct ipv6_fl_socklist *ipv6_fl_list;
    struct ipv6_txoptions *opt;
    struct sk_buff *pktoptions;
    struct sk_buff *rxpmtu;
    struct inet6_cork cork;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ipv6_pinfo {
    struct in6_addr saddr;
    struct in6_pktinfo sticky_pktinfo;
    const struct in6_addr *daddr_cache;
    const struct in6_addr *saddr_cache;
    __be32 flow_label;
    __u32 frag_size;
    __u16 __unused_1;
    __s16 hop_limit;
    __u16 mc_loop;
    __u16 __unused_2;
    __s16 mcast_hops;
    int ucast_oif;
    int mcast_oif;
    union (anon) rxopt;
    __u16 recverr;
    __u16 sndflow;
    __u16 repflow;
    __u16 pmtudisc;
    __u16 padding;
    __u16 srcprefs;
    __u16 dontfrag;
    __u16 autoflowlabel;
    __u16 autoflowlabel_set;
    __u16 mc_all;
    __u16 recverr_rfc4884;
    __u16 rtalert_isolate;
    __u8 min_hopcount;
    __u8 tclass;
    __be32 rcv_flowinfo;
    __u32 dst_cookie;
    struct ipv6_mc_socklist *ipv6_mc_list;
    struct ipv6_ac_socklist *ipv6_ac_list;
    struct ipv6_fl_socklist *ipv6_fl_list;
    struct ipv6_txoptions *opt;
    struct sk_buff *pktoptions;
    struct sk_buff *rxpmtu;
    struct inet6_cork cork;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ipv6_pinfo {
    struct in6_addr saddr;
    struct in6_pktinfo sticky_pktinfo;
    const struct in6_addr *daddr_cache;
    const struct in6_addr *saddr_cache;
    __be32 flow_label;
    __u32 frag_size;
    s16 hop_limit;
    u8 mcast_hops;
    int ucast_oif;
    int mcast_oif;
    union (anon) rxopt;
    __u8 srcprefs;
    __u8 pmtudisc;
    __u8 min_hopcount;
    __u8 tclass;
    __be32 rcv_flowinfo;
    __u32 dst_cookie;
    struct ipv6_mc_socklist *ipv6_mc_list;
    struct ipv6_ac_socklist *ipv6_ac_list;
    struct ipv6_fl_socklist *ipv6_fl_list;
    struct ipv6_txoptions *opt;
    struct sk_buff *pktoptions;
    struct sk_buff *rxpmtu;
    struct inet6_cork cork;
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
struct ipv6_pinfo {
    struct in6_addr saddr;
    struct in6_pktinfo sticky_pktinfo;
    const struct in6_addr *daddr_cache;
    const struct in6_addr *saddr_cache;
    __be32 flow_label;
    __u32 frag_size;
    __u16 __unused_1;
    __s16 hop_limit;
    __u16 mc_loop;
    __u16 __unused_2;
    __s16 mcast_hops;
    int ucast_oif;
    int mcast_oif;
    union (anon) rxopt;
    __u16 recverr;
    __u16 sndflow;
    __u16 repflow;
    __u16 pmtudisc;
    __u16 padding;
    __u16 srcprefs;
    __u16 dontfrag;
    __u16 autoflowlabel;
    __u16 autoflowlabel_set;
    __u16 mc_all;
    __u16 rtalert_isolate;
    __u8 min_hopcount;
    __u8 tclass;
    __be32 rcv_flowinfo;
    __u32 dst_cookie;
    __u32 rx_dst_cookie;
    struct ipv6_mc_socklist *ipv6_mc_list;
    struct ipv6_ac_socklist *ipv6_ac_list;
    struct ipv6_fl_socklist *ipv6_fl_list;
    struct ipv6_txoptions *opt;
    struct sk_buff *pktoptions;
    struct sk_buff *rxpmtu;
    struct inet6_cork cork;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ipv6_pinfo {
    struct in6_addr saddr;
    struct in6_pktinfo sticky_pktinfo;
    const struct in6_addr *daddr_cache;
    const struct in6_addr *saddr_cache;
    __be32 flow_label;
    __u32 frag_size;
    __u16 __unused_1;
    __s16 hop_limit;
    __u16 mc_loop;
    __u16 __unused_2;
    __s16 mcast_hops;
    int ucast_oif;
    int mcast_oif;
    union (anon) rxopt;
    __u16 recverr;
    __u16 sndflow;
    __u16 repflow;
    __u16 pmtudisc;
    __u16 padding;
    __u16 srcprefs;
    __u16 dontfrag;
    __u16 autoflowlabel;
    __u16 autoflowlabel_set;
    __u16 mc_all;
    __u16 rtalert_isolate;
    __u8 min_hopcount;
    __u8 tclass;
    __be32 rcv_flowinfo;
    __u32 dst_cookie;
    __u32 rx_dst_cookie;
    struct ipv6_mc_socklist *ipv6_mc_list;
    struct ipv6_ac_socklist *ipv6_ac_list;
    struct ipv6_fl_socklist *ipv6_fl_list;
    struct ipv6_txoptions *opt;
    struct sk_buff *pktoptions;
    struct sk_buff *rxpmtu;
    struct inet6_cork cork;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ipv6_pinfo {
    struct in6_addr saddr;
    struct in6_pktinfo sticky_pktinfo;
    const struct in6_addr *daddr_cache;
    const struct in6_addr *saddr_cache;
    __be32 flow_label;
    __u32 frag_size;
    __u16 __unused_1;
    __s16 hop_limit;
    __u16 mc_loop;
    __u16 __unused_2;
    __s16 mcast_hops;
    int ucast_oif;
    int mcast_oif;
    union (anon) rxopt;
    __u16 recverr;
    __u16 sndflow;
    __u16 repflow;
    __u16 pmtudisc;
    __u16 padding;
    __u16 srcprefs;
    __u16 dontfrag;
    __u16 autoflowlabel;
    __u16 autoflowlabel_set;
    __u16 mc_all;
    __u16 rtalert_isolate;
    __u8 min_hopcount;
    __u8 tclass;
    __be32 rcv_flowinfo;
    __u32 dst_cookie;
    __u32 rx_dst_cookie;
    struct ipv6_mc_socklist *ipv6_mc_list;
    struct ipv6_ac_socklist *ipv6_ac_list;
    struct ipv6_fl_socklist *ipv6_fl_list;
    struct ipv6_txoptions *opt;
    struct sk_buff *pktoptions;
    struct sk_buff *rxpmtu;
    struct inet6_cork cork;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ipv6_pinfo {
    struct in6_addr saddr;
    struct in6_pktinfo sticky_pktinfo;
    const struct in6_addr *daddr_cache;
    const struct in6_addr *saddr_cache;
    __be32 flow_label;
    __u32 frag_size;
    __u16 __unused_1;
    __s16 hop_limit;
    __u16 mc_loop;
    __u16 __unused_2;
    __s16 mcast_hops;
    int ucast_oif;
    int mcast_oif;
    union (anon) rxopt;
    __u16 recverr;
    __u16 sndflow;
    __u16 repflow;
    __u16 pmtudisc;
    __u16 padding;
    __u16 srcprefs;
    __u16 dontfrag;
    __u16 autoflowlabel;
    __u16 autoflowlabel_set;
    __u16 mc_all;
    __u16 rtalert_isolate;
    __u8 min_hopcount;
    __u8 tclass;
    __be32 rcv_flowinfo;
    __u32 dst_cookie;
    __u32 rx_dst_cookie;
    struct ipv6_mc_socklist *ipv6_mc_list;
    struct ipv6_ac_socklist *ipv6_ac_list;
    struct ipv6_fl_socklist *ipv6_fl_list;
    struct ipv6_txoptions *opt;
    struct sk_buff *pktoptions;
    struct sk_buff *rxpmtu;
    struct inet6_cork cork;
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
struct ipv6_pinfo {
    struct in6_addr saddr;
    struct in6_pktinfo sticky_pktinfo;
    const struct in6_addr *daddr_cache;
    const struct in6_addr *saddr_cache;
    __be32 flow_label;
    __u32 frag_size;
    __u16 __unused_1;
    __s16 hop_limit;
    __u16 mc_loop;
    __u16 __unused_2;
    __s16 mcast_hops;
    int ucast_oif;
    int mcast_oif;
    union (anon) rxopt;
    __u16 recverr;
    __u16 sndflow;
    __u16 repflow;
    __u16 pmtudisc;
    __u16 padding;
    __u16 srcprefs;
    __u16 dontfrag;
    __u16 autoflowlabel;
    __u16 autoflowlabel_set;
    __u16 mc_all;
    __u16 rtalert_isolate;
    __u8 min_hopcount;
    __u8 tclass;
    __be32 rcv_flowinfo;
    __u32 dst_cookie;
    __u32 rx_dst_cookie;
    struct ipv6_mc_socklist *ipv6_mc_list;
    struct ipv6_ac_socklist *ipv6_ac_list;
    struct ipv6_fl_socklist *ipv6_fl_list;
    struct ipv6_txoptions *opt;
    struct sk_buff *pktoptions;
    struct sk_buff *rxpmtu;
    struct inet6_cork cork;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ipv6_pinfo {
    struct in6_addr saddr;
    struct in6_pktinfo sticky_pktinfo;
    const struct in6_addr *daddr_cache;
    const struct in6_addr *saddr_cache;
    __be32 flow_label;
    __u32 frag_size;
    __u16 __unused_1;
    __s16 hop_limit;
    __u16 mc_loop;
    __u16 __unused_2;
    __s16 mcast_hops;
    int ucast_oif;
    int mcast_oif;
    union (anon) rxopt;
    __u16 recverr;
    __u16 sndflow;
    __u16 repflow;
    __u16 pmtudisc;
    __u16 padding;
    __u16 srcprefs;
    __u16 dontfrag;
    __u16 autoflowlabel;
    __u16 autoflowlabel_set;
    __u16 mc_all;
    __u16 rtalert_isolate;
    __u8 min_hopcount;
    __u8 tclass;
    __be32 rcv_flowinfo;
    __u32 dst_cookie;
    __u32 rx_dst_cookie;
    struct ipv6_mc_socklist *ipv6_mc_list;
    struct ipv6_ac_socklist *ipv6_ac_list;
    struct ipv6_fl_socklist *ipv6_fl_list;
    struct ipv6_txoptions *opt;
    struct sk_buff *pktoptions;
    struct sk_buff *rxpmtu;
    struct inet6_cork cork;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ipv6_pinfo {
    struct in6_addr saddr;
    struct in6_pktinfo sticky_pktinfo;
    const struct in6_addr *daddr_cache;
    const struct in6_addr *saddr_cache;
    __be32 flow_label;
    __u32 frag_size;
    __u16 __unused_1;
    __s16 hop_limit;
    __u16 mc_loop;
    __u16 __unused_2;
    __s16 mcast_hops;
    int ucast_oif;
    int mcast_oif;
    union (anon) rxopt;
    __u16 recverr;
    __u16 sndflow;
    __u16 repflow;
    __u16 pmtudisc;
    __u16 padding;
    __u16 srcprefs;
    __u16 dontfrag;
    __u16 autoflowlabel;
    __u16 autoflowlabel_set;
    __u16 mc_all;
    __u16 rtalert_isolate;
    __u8 min_hopcount;
    __u8 tclass;
    __be32 rcv_flowinfo;
    __u32 dst_cookie;
    __u32 rx_dst_cookie;
    struct ipv6_mc_socklist *ipv6_mc_list;
    struct ipv6_ac_socklist *ipv6_ac_list;
    struct ipv6_fl_socklist *ipv6_fl_list;
    struct ipv6_txoptions *opt;
    struct sk_buff *pktoptions;
    struct sk_buff *rxpmtu;
    struct inet6_cork cork;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ipv6_pinfo {
    struct in6_addr saddr;
    struct in6_pktinfo sticky_pktinfo;
    const struct in6_addr *daddr_cache;
    const struct in6_addr *saddr_cache;
    __be32 flow_label;
    __u32 frag_size;
    __u16 __unused_1;
    __s16 hop_limit;
    __u16 mc_loop;
    __u16 __unused_2;
    __s16 mcast_hops;
    int ucast_oif;
    int mcast_oif;
    union (anon) rxopt;
    __u16 recverr;
    __u16 sndflow;
    __u16 repflow;
    __u16 pmtudisc;
    __u16 padding;
    __u16 srcprefs;
    __u16 dontfrag;
    __u16 autoflowlabel;
    __u16 autoflowlabel_set;
    __u16 mc_all;
    __u16 rtalert_isolate;
    __u8 min_hopcount;
    __u8 tclass;
    __be32 rcv_flowinfo;
    __u32 dst_cookie;
    __u32 rx_dst_cookie;
    struct ipv6_mc_socklist *ipv6_mc_list;
    struct ipv6_ac_socklist *ipv6_ac_list;
    struct ipv6_fl_socklist *ipv6_fl_list;
    struct ipv6_txoptions *opt;
    struct sk_buff *pktoptions;
    struct sk_buff *rxpmtu;
    struct inet6_cork cork;
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
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u16 autoflowlabel_set</code>
</li>
</ul>
</details>
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
<code>__u16 mc_all</code>
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
<code>__u16 rtalert_isolate</code>
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
<code>__u16 recverr_rfc4884</code>
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
<b>Field removed. </b>
<code>__u32 rx_dst_cookie</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>__u16 __unused_1</code>
</li>
<li>
<b>Field removed. </b>
<code>__u16 mc_loop</code>
</li>
<li>
<b>Field removed. </b>
<code>__u16 __unused_2</code>
</li>
<li>
<b>Field removed. </b>
<code>__u16 recverr</code>
</li>
<li>
<b>Field removed. </b>
<code>__u16 sndflow</code>
</li>
<li>
<b>Field removed. </b>
<code>__u16 repflow</code>
</li>
<li>
<b>Field removed. </b>
<code>__u16 padding</code>
</li>
<li>
<b>Field removed. </b>
<code>__u16 dontfrag</code>
</li>
<li>
<b>Field removed. </b>
<code>__u16 autoflowlabel</code>
</li>
<li>
<b>Field removed. </b>
<code>__u16 autoflowlabel_set</code>
</li>
<li>
<b>Field removed. </b>
<code>__u16 mc_all</code>
</li>
<li>
<b>Field removed. </b>
<code>__u16 recverr_rfc4884</code>
</li>
<li>
<b>Field removed. </b>
<code>__u16 rtalert_isolate</code>
</li>
<li>
<b>Field type changed. </b>
<code>__s16 hop_limit</code> ➡️ <code>s16 hop_limit</code>
</li>
<li>
<b>Field type changed. </b>
<code>__s16 mcast_hops</code> ➡️ <code>u8 mcast_hops</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u16 pmtudisc</code> ➡️ <code>__u8 pmtudisc</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u16 srcprefs</code> ➡️ <code>__u8 srcprefs</code>
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
