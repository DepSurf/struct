# Struct: <code>netns_mib</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct netns_mib {
    struct tcp_mib *tcp_statistics;
    struct ipstats_mib *ip_statistics;
    struct linux_mib *net_statistics;
    struct udp_mib *udp_statistics;
    struct udp_mib *udplite_statistics;
    struct icmp_mib *icmp_statistics;
    struct icmpmsg_mib *icmpmsg_statistics;
    struct proc_dir_entry *proc_net_devsnmp6;
    struct udp_mib *udp_stats_in6;
    struct udp_mib *udplite_stats_in6;
    struct ipstats_mib *ipv6_statistics;
    struct icmpv6_mib *icmpv6_statistics;
    struct icmpv6msg_mib *icmpv6msg_statistics;
    struct linux_xfrm_mib *xfrm_statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct netns_mib {
    struct tcp_mib *tcp_statistics;
    struct ipstats_mib *ip_statistics;
    struct linux_mib *net_statistics;
    struct udp_mib *udp_statistics;
    struct udp_mib *udplite_statistics;
    struct icmp_mib *icmp_statistics;
    struct icmpmsg_mib *icmpmsg_statistics;
    struct proc_dir_entry *proc_net_devsnmp6;
    struct udp_mib *udp_stats_in6;
    struct udp_mib *udplite_stats_in6;
    struct ipstats_mib *ipv6_statistics;
    struct icmpv6_mib *icmpv6_statistics;
    struct icmpv6msg_mib *icmpv6msg_statistics;
    struct linux_xfrm_mib *xfrm_statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct netns_mib {
    struct tcp_mib *tcp_statistics;
    struct ipstats_mib *ip_statistics;
    struct linux_mib *net_statistics;
    struct udp_mib *udp_statistics;
    struct udp_mib *udplite_statistics;
    struct icmp_mib *icmp_statistics;
    struct icmpmsg_mib *icmpmsg_statistics;
    struct proc_dir_entry *proc_net_devsnmp6;
    struct udp_mib *udp_stats_in6;
    struct udp_mib *udplite_stats_in6;
    struct ipstats_mib *ipv6_statistics;
    struct icmpv6_mib *icmpv6_statistics;
    struct icmpv6msg_mib *icmpv6msg_statistics;
    struct linux_xfrm_mib *xfrm_statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct netns_mib {
    struct tcp_mib *tcp_statistics;
    struct ipstats_mib *ip_statistics;
    struct linux_mib *net_statistics;
    struct udp_mib *udp_statistics;
    struct udp_mib *udplite_statistics;
    struct icmp_mib *icmp_statistics;
    struct icmpmsg_mib *icmpmsg_statistics;
    struct proc_dir_entry *proc_net_devsnmp6;
    struct udp_mib *udp_stats_in6;
    struct udp_mib *udplite_stats_in6;
    struct ipstats_mib *ipv6_statistics;
    struct icmpv6_mib *icmpv6_statistics;
    struct icmpv6msg_mib *icmpv6msg_statistics;
    struct linux_xfrm_mib *xfrm_statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct netns_mib {
    struct tcp_mib *tcp_statistics;
    struct ipstats_mib *ip_statistics;
    struct linux_mib *net_statistics;
    struct udp_mib *udp_statistics;
    struct udp_mib *udplite_statistics;
    struct icmp_mib *icmp_statistics;
    struct icmpmsg_mib *icmpmsg_statistics;
    struct proc_dir_entry *proc_net_devsnmp6;
    struct udp_mib *udp_stats_in6;
    struct udp_mib *udplite_stats_in6;
    struct ipstats_mib *ipv6_statistics;
    struct icmpv6_mib *icmpv6_statistics;
    struct icmpv6msg_mib *icmpv6msg_statistics;
    struct linux_xfrm_mib *xfrm_statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct netns_mib {
    struct tcp_mib *tcp_statistics;
    struct ipstats_mib *ip_statistics;
    struct linux_mib *net_statistics;
    struct udp_mib *udp_statistics;
    struct udp_mib *udplite_statistics;
    struct icmp_mib *icmp_statistics;
    struct icmpmsg_mib *icmpmsg_statistics;
    struct proc_dir_entry *proc_net_devsnmp6;
    struct udp_mib *udp_stats_in6;
    struct udp_mib *udplite_stats_in6;
    struct ipstats_mib *ipv6_statistics;
    struct icmpv6_mib *icmpv6_statistics;
    struct icmpv6msg_mib *icmpv6msg_statistics;
    struct linux_xfrm_mib *xfrm_statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct netns_mib {
    struct tcp_mib *tcp_statistics;
    struct ipstats_mib *ip_statistics;
    struct linux_mib *net_statistics;
    struct udp_mib *udp_statistics;
    struct udp_mib *udplite_statistics;
    struct icmp_mib *icmp_statistics;
    struct icmpmsg_mib *icmpmsg_statistics;
    struct proc_dir_entry *proc_net_devsnmp6;
    struct udp_mib *udp_stats_in6;
    struct udp_mib *udplite_stats_in6;
    struct ipstats_mib *ipv6_statistics;
    struct icmpv6_mib *icmpv6_statistics;
    struct icmpv6msg_mib *icmpv6msg_statistics;
    struct linux_xfrm_mib *xfrm_statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct netns_mib {
    struct tcp_mib *tcp_statistics;
    struct ipstats_mib *ip_statistics;
    struct linux_mib *net_statistics;
    struct udp_mib *udp_statistics;
    struct udp_mib *udplite_statistics;
    struct icmp_mib *icmp_statistics;
    struct icmpmsg_mib *icmpmsg_statistics;
    struct proc_dir_entry *proc_net_devsnmp6;
    struct udp_mib *udp_stats_in6;
    struct udp_mib *udplite_stats_in6;
    struct ipstats_mib *ipv6_statistics;
    struct icmpv6_mib *icmpv6_statistics;
    struct icmpv6msg_mib *icmpv6msg_statistics;
    struct linux_xfrm_mib *xfrm_statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct netns_mib {
    struct tcp_mib *tcp_statistics;
    struct ipstats_mib *ip_statistics;
    struct linux_mib *net_statistics;
    struct udp_mib *udp_statistics;
    struct udp_mib *udplite_statistics;
    struct icmp_mib *icmp_statistics;
    struct icmpmsg_mib *icmpmsg_statistics;
    struct proc_dir_entry *proc_net_devsnmp6;
    struct udp_mib *udp_stats_in6;
    struct udp_mib *udplite_stats_in6;
    struct ipstats_mib *ipv6_statistics;
    struct icmpv6_mib *icmpv6_statistics;
    struct icmpv6msg_mib *icmpv6msg_statistics;
    struct linux_xfrm_mib *xfrm_statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct netns_mib {
    struct tcp_mib *tcp_statistics;
    struct ipstats_mib *ip_statistics;
    struct linux_mib *net_statistics;
    struct udp_mib *udp_statistics;
    struct udp_mib *udplite_statistics;
    struct icmp_mib *icmp_statistics;
    struct icmpmsg_mib *icmpmsg_statistics;
    struct proc_dir_entry *proc_net_devsnmp6;
    struct udp_mib *udp_stats_in6;
    struct udp_mib *udplite_stats_in6;
    struct ipstats_mib *ipv6_statistics;
    struct icmpv6_mib *icmpv6_statistics;
    struct icmpv6msg_mib *icmpv6msg_statistics;
    struct linux_xfrm_mib *xfrm_statistics;
    struct linux_tls_mib *tls_statistics;
    struct mptcp_mib *mptcp_statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct netns_mib {
    struct tcp_mib *tcp_statistics;
    struct ipstats_mib *ip_statistics;
    struct linux_mib *net_statistics;
    struct udp_mib *udp_statistics;
    struct udp_mib *udplite_statistics;
    struct icmp_mib *icmp_statistics;
    struct icmpmsg_mib *icmpmsg_statistics;
    struct proc_dir_entry *proc_net_devsnmp6;
    struct udp_mib *udp_stats_in6;
    struct udp_mib *udplite_stats_in6;
    struct ipstats_mib *ipv6_statistics;
    struct icmpv6_mib *icmpv6_statistics;
    struct icmpv6msg_mib *icmpv6msg_statistics;
    struct linux_xfrm_mib *xfrm_statistics;
    struct linux_tls_mib *tls_statistics;
    struct mptcp_mib *mptcp_statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct netns_mib {
    struct ipstats_mib *ip_statistics;
    struct ipstats_mib *ipv6_statistics;
    struct tcp_mib *tcp_statistics;
    struct linux_mib *net_statistics;
    struct udp_mib *udp_statistics;
    struct udp_mib *udp_stats_in6;
    struct linux_xfrm_mib *xfrm_statistics;
    struct linux_tls_mib *tls_statistics;
    struct mptcp_mib *mptcp_statistics;
    struct udp_mib *udplite_statistics;
    struct udp_mib *udplite_stats_in6;
    struct icmp_mib *icmp_statistics;
    struct icmpmsg_mib *icmpmsg_statistics;
    struct icmpv6_mib *icmpv6_statistics;
    struct icmpv6msg_mib *icmpv6msg_statistics;
    struct proc_dir_entry *proc_net_devsnmp6;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct netns_mib {
    struct ipstats_mib *ip_statistics;
    struct ipstats_mib *ipv6_statistics;
    struct tcp_mib *tcp_statistics;
    struct linux_mib *net_statistics;
    struct udp_mib *udp_statistics;
    struct udp_mib *udp_stats_in6;
    struct linux_xfrm_mib *xfrm_statistics;
    struct linux_tls_mib *tls_statistics;
    struct mptcp_mib *mptcp_statistics;
    struct udp_mib *udplite_statistics;
    struct udp_mib *udplite_stats_in6;
    struct icmp_mib *icmp_statistics;
    struct icmpmsg_mib *icmpmsg_statistics;
    struct icmpv6_mib *icmpv6_statistics;
    struct icmpv6msg_mib *icmpv6msg_statistics;
    struct proc_dir_entry *proc_net_devsnmp6;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct netns_mib {
    struct ipstats_mib *ip_statistics;
    struct ipstats_mib *ipv6_statistics;
    struct tcp_mib *tcp_statistics;
    struct linux_mib *net_statistics;
    struct udp_mib *udp_statistics;
    struct udp_mib *udp_stats_in6;
    struct linux_xfrm_mib *xfrm_statistics;
    struct linux_tls_mib *tls_statistics;
    struct mptcp_mib *mptcp_statistics;
    struct udp_mib *udplite_statistics;
    struct udp_mib *udplite_stats_in6;
    struct icmp_mib *icmp_statistics;
    struct icmpmsg_mib *icmpmsg_statistics;
    struct icmpv6_mib *icmpv6_statistics;
    struct icmpv6msg_mib *icmpv6msg_statistics;
    struct proc_dir_entry *proc_net_devsnmp6;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct netns_mib {
    struct ipstats_mib *ip_statistics;
    struct ipstats_mib *ipv6_statistics;
    struct tcp_mib *tcp_statistics;
    struct linux_mib *net_statistics;
    struct udp_mib *udp_statistics;
    struct udp_mib *udp_stats_in6;
    struct linux_xfrm_mib *xfrm_statistics;
    struct linux_tls_mib *tls_statistics;
    struct mptcp_mib *mptcp_statistics;
    struct udp_mib *udplite_statistics;
    struct udp_mib *udplite_stats_in6;
    struct icmp_mib *icmp_statistics;
    struct icmpmsg_mib *icmpmsg_statistics;
    struct icmpv6_mib *icmpv6_statistics;
    struct icmpv6msg_mib *icmpv6msg_statistics;
    struct proc_dir_entry *proc_net_devsnmp6;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct netns_mib {
    struct ipstats_mib *ip_statistics;
    struct ipstats_mib *ipv6_statistics;
    struct tcp_mib *tcp_statistics;
    struct linux_mib *net_statistics;
    struct udp_mib *udp_statistics;
    struct udp_mib *udp_stats_in6;
    struct linux_xfrm_mib *xfrm_statistics;
    struct linux_tls_mib *tls_statistics;
    struct mptcp_mib *mptcp_statistics;
    struct udp_mib *udplite_statistics;
    struct udp_mib *udplite_stats_in6;
    struct icmp_mib *icmp_statistics;
    struct icmpmsg_mib *icmpmsg_statistics;
    struct icmpv6_mib *icmpv6_statistics;
    struct icmpv6msg_mib *icmpv6msg_statistics;
    struct proc_dir_entry *proc_net_devsnmp6;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct netns_mib {
    struct ipstats_mib *ip_statistics;
    struct ipstats_mib *ipv6_statistics;
    struct tcp_mib *tcp_statistics;
    struct linux_mib *net_statistics;
    struct udp_mib *udp_statistics;
    struct udp_mib *udp_stats_in6;
    struct linux_xfrm_mib *xfrm_statistics;
    struct linux_tls_mib *tls_statistics;
    struct mptcp_mib *mptcp_statistics;
    struct udp_mib *udplite_statistics;
    struct udp_mib *udplite_stats_in6;
    struct icmp_mib *icmp_statistics;
    struct icmpmsg_mib *icmpmsg_statistics;
    struct icmpv6_mib *icmpv6_statistics;
    struct icmpv6msg_mib *icmpv6msg_statistics;
    struct proc_dir_entry *proc_net_devsnmp6;
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
struct netns_mib {
    struct tcp_mib *tcp_statistics;
    struct ipstats_mib *ip_statistics;
    struct linux_mib *net_statistics;
    struct udp_mib *udp_statistics;
    struct udp_mib *udplite_statistics;
    struct icmp_mib *icmp_statistics;
    struct icmpmsg_mib *icmpmsg_statistics;
    struct proc_dir_entry *proc_net_devsnmp6;
    struct udp_mib *udp_stats_in6;
    struct udp_mib *udplite_stats_in6;
    struct ipstats_mib *ipv6_statistics;
    struct icmpv6_mib *icmpv6_statistics;
    struct icmpv6msg_mib *icmpv6msg_statistics;
    struct linux_xfrm_mib *xfrm_statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct netns_mib {
    struct tcp_mib *tcp_statistics;
    struct ipstats_mib *ip_statistics;
    struct linux_mib *net_statistics;
    struct udp_mib *udp_statistics;
    struct udp_mib *udplite_statistics;
    struct icmp_mib *icmp_statistics;
    struct icmpmsg_mib *icmpmsg_statistics;
    struct proc_dir_entry *proc_net_devsnmp6;
    struct udp_mib *udp_stats_in6;
    struct udp_mib *udplite_stats_in6;
    struct ipstats_mib *ipv6_statistics;
    struct icmpv6_mib *icmpv6_statistics;
    struct icmpv6msg_mib *icmpv6msg_statistics;
    struct linux_xfrm_mib *xfrm_statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct netns_mib {
    struct tcp_mib *tcp_statistics;
    struct ipstats_mib *ip_statistics;
    struct linux_mib *net_statistics;
    struct udp_mib *udp_statistics;
    struct udp_mib *udplite_statistics;
    struct icmp_mib *icmp_statistics;
    struct icmpmsg_mib *icmpmsg_statistics;
    struct proc_dir_entry *proc_net_devsnmp6;
    struct udp_mib *udp_stats_in6;
    struct udp_mib *udplite_stats_in6;
    struct ipstats_mib *ipv6_statistics;
    struct icmpv6_mib *icmpv6_statistics;
    struct icmpv6msg_mib *icmpv6msg_statistics;
    struct linux_xfrm_mib *xfrm_statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct netns_mib {
    struct tcp_mib *tcp_statistics;
    struct ipstats_mib *ip_statistics;
    struct linux_mib *net_statistics;
    struct udp_mib *udp_statistics;
    struct udp_mib *udplite_statistics;
    struct icmp_mib *icmp_statistics;
    struct icmpmsg_mib *icmpmsg_statistics;
    struct proc_dir_entry *proc_net_devsnmp6;
    struct udp_mib *udp_stats_in6;
    struct udp_mib *udplite_stats_in6;
    struct ipstats_mib *ipv6_statistics;
    struct icmpv6_mib *icmpv6_statistics;
    struct icmpv6msg_mib *icmpv6msg_statistics;
    struct linux_xfrm_mib *xfrm_statistics;
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
struct netns_mib {
    struct tcp_mib *tcp_statistics;
    struct ipstats_mib *ip_statistics;
    struct linux_mib *net_statistics;
    struct udp_mib *udp_statistics;
    struct udp_mib *udplite_statistics;
    struct icmp_mib *icmp_statistics;
    struct icmpmsg_mib *icmpmsg_statistics;
    struct proc_dir_entry *proc_net_devsnmp6;
    struct udp_mib *udp_stats_in6;
    struct udp_mib *udplite_stats_in6;
    struct ipstats_mib *ipv6_statistics;
    struct icmpv6_mib *icmpv6_statistics;
    struct icmpv6msg_mib *icmpv6msg_statistics;
    struct linux_xfrm_mib *xfrm_statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct netns_mib {
    struct tcp_mib *tcp_statistics;
    struct ipstats_mib *ip_statistics;
    struct linux_mib *net_statistics;
    struct udp_mib *udp_statistics;
    struct udp_mib *udplite_statistics;
    struct icmp_mib *icmp_statistics;
    struct icmpmsg_mib *icmpmsg_statistics;
    struct proc_dir_entry *proc_net_devsnmp6;
    struct udp_mib *udp_stats_in6;
    struct udp_mib *udplite_stats_in6;
    struct ipstats_mib *ipv6_statistics;
    struct icmpv6_mib *icmpv6_statistics;
    struct icmpv6msg_mib *icmpv6msg_statistics;
    struct linux_xfrm_mib *xfrm_statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct netns_mib {
    struct tcp_mib *tcp_statistics;
    struct ipstats_mib *ip_statistics;
    struct linux_mib *net_statistics;
    struct udp_mib *udp_statistics;
    struct udp_mib *udplite_statistics;
    struct icmp_mib *icmp_statistics;
    struct icmpmsg_mib *icmpmsg_statistics;
    struct proc_dir_entry *proc_net_devsnmp6;
    struct udp_mib *udp_stats_in6;
    struct udp_mib *udplite_stats_in6;
    struct ipstats_mib *ipv6_statistics;
    struct icmpv6_mib *icmpv6_statistics;
    struct icmpv6msg_mib *icmpv6msg_statistics;
    struct linux_xfrm_mib *xfrm_statistics;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct netns_mib {
    struct tcp_mib *tcp_statistics;
    struct ipstats_mib *ip_statistics;
    struct linux_mib *net_statistics;
    struct udp_mib *udp_statistics;
    struct udp_mib *udplite_statistics;
    struct icmp_mib *icmp_statistics;
    struct icmpmsg_mib *icmpmsg_statistics;
    struct proc_dir_entry *proc_net_devsnmp6;
    struct udp_mib *udp_stats_in6;
    struct udp_mib *udplite_stats_in6;
    struct ipstats_mib *ipv6_statistics;
    struct icmpv6_mib *icmpv6_statistics;
    struct icmpv6msg_mib *icmpv6msg_statistics;
    struct linux_xfrm_mib *xfrm_statistics;
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct linux_tls_mib *tls_statistics</code>
</li>
<li>
<b>Field added. </b>
<code>struct mptcp_mib *mptcp_statistics</code>
</li>
</ul>
</details>
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
