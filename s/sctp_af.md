# Struct: <code>sctp_af</code>

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
struct sctp_af {
    int (*sctp_xmit)(struct sk_buff *, struct sctp_transport *);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*get_dst)(struct sctp_transport *, union sctp_addr *, struct flowi *, struct sock *);
    void (*get_saddr)(struct sctp_sock *, struct sctp_transport *, struct flowi *);
    void (*copy_addrlist)(struct list_head *, struct net_device *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *);
    void (*addr_copy)(union sctp_addr *, union sctp_addr *);
    void (*from_skb)(union sctp_addr *, struct sk_buff *, int);
    void (*from_sk)(union sctp_addr *, struct sock *);
    void (*from_addr_param)(union sctp_addr *, union sctp_addr_param *, __be16, int);
    int (*to_addr_param)(const union sctp_addr *, union sctp_addr_param *);
    int (*addr_valid)(union sctp_addr *, struct sctp_sock *, const struct sk_buff *);
    enum sctp_scope (*scope)(union sctp_addr *);
    void (*inaddr_any)(union sctp_addr *, __be16);
    int (*is_any)(const union sctp_addr *);
    int (*available)(union sctp_addr *, struct sctp_sock *);
    int (*skb_iif)(const struct sk_buff *);
    int (*is_ce)(const struct sk_buff *);
    void (*seq_dump_addr)(struct seq_file *, union sctp_addr *);
    void (*ecn_capable)(struct sock *);
    __u16 net_header_len;
    int sockaddr_len;
    int (*ip_options_len)(struct sock *);
    sa_family_t sa_family;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct sctp_af {
    int (*sctp_xmit)(struct sk_buff *, struct sctp_transport *);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*get_dst)(struct sctp_transport *, union sctp_addr *, struct flowi *, struct sock *);
    void (*get_saddr)(struct sctp_sock *, struct sctp_transport *, struct flowi *);
    void (*copy_addrlist)(struct list_head *, struct net_device *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *);
    void (*addr_copy)(union sctp_addr *, union sctp_addr *);
    void (*from_skb)(union sctp_addr *, struct sk_buff *, int);
    void (*from_sk)(union sctp_addr *, struct sock *);
    void (*from_addr_param)(union sctp_addr *, union sctp_addr_param *, __be16, int);
    int (*to_addr_param)(const union sctp_addr *, union sctp_addr_param *);
    int (*addr_valid)(union sctp_addr *, struct sctp_sock *, const struct sk_buff *);
    enum sctp_scope (*scope)(union sctp_addr *);
    void (*inaddr_any)(union sctp_addr *, __be16);
    int (*is_any)(const union sctp_addr *);
    int (*available)(union sctp_addr *, struct sctp_sock *);
    int (*skb_iif)(const struct sk_buff *);
    int (*is_ce)(const struct sk_buff *);
    void (*seq_dump_addr)(struct seq_file *, union sctp_addr *);
    void (*ecn_capable)(struct sock *);
    __u16 net_header_len;
    int sockaddr_len;
    int (*ip_options_len)(struct sock *);
    sa_family_t sa_family;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct sctp_af {
    int (*sctp_xmit)(struct sk_buff *, struct sctp_transport *);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*get_dst)(struct sctp_transport *, union sctp_addr *, struct flowi *, struct sock *);
    void (*get_saddr)(struct sctp_sock *, struct sctp_transport *, struct flowi *);
    void (*copy_addrlist)(struct list_head *, struct net_device *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *);
    void (*addr_copy)(union sctp_addr *, union sctp_addr *);
    void (*from_skb)(union sctp_addr *, struct sk_buff *, int);
    void (*from_sk)(union sctp_addr *, struct sock *);
    void (*from_addr_param)(union sctp_addr *, union sctp_addr_param *, __be16, int);
    int (*to_addr_param)(const union sctp_addr *, union sctp_addr_param *);
    int (*addr_valid)(union sctp_addr *, struct sctp_sock *, const struct sk_buff *);
    enum sctp_scope (*scope)(union sctp_addr *);
    void (*inaddr_any)(union sctp_addr *, __be16);
    int (*is_any)(const union sctp_addr *);
    int (*available)(union sctp_addr *, struct sctp_sock *);
    int (*skb_iif)(const struct sk_buff *);
    int (*is_ce)(const struct sk_buff *);
    void (*seq_dump_addr)(struct seq_file *, union sctp_addr *);
    void (*ecn_capable)(struct sock *);
    __u16 net_header_len;
    int sockaddr_len;
    int (*ip_options_len)(struct sock *);
    sa_family_t sa_family;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct sctp_af {
    int (*sctp_xmit)(struct sk_buff *, struct sctp_transport *);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*get_dst)(struct sctp_transport *, union sctp_addr *, struct flowi *, struct sock *);
    void (*get_saddr)(struct sctp_sock *, struct sctp_transport *, struct flowi *);
    void (*copy_addrlist)(struct list_head *, struct net_device *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *);
    void (*addr_copy)(union sctp_addr *, union sctp_addr *);
    void (*from_skb)(union sctp_addr *, struct sk_buff *, int);
    void (*from_sk)(union sctp_addr *, struct sock *);
    void (*from_addr_param)(union sctp_addr *, union sctp_addr_param *, __be16, int);
    int (*to_addr_param)(const union sctp_addr *, union sctp_addr_param *);
    int (*addr_valid)(union sctp_addr *, struct sctp_sock *, const struct sk_buff *);
    enum sctp_scope (*scope)(union sctp_addr *);
    void (*inaddr_any)(union sctp_addr *, __be16);
    int (*is_any)(const union sctp_addr *);
    int (*available)(union sctp_addr *, struct sctp_sock *);
    int (*skb_iif)(const struct sk_buff *);
    int (*is_ce)(const struct sk_buff *);
    void (*seq_dump_addr)(struct seq_file *, union sctp_addr *);
    void (*ecn_capable)(struct sock *);
    __u16 net_header_len;
    int sockaddr_len;
    int (*ip_options_len)(struct sock *);
    sa_family_t sa_family;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct sctp_af {
    int (*sctp_xmit)(struct sk_buff *, struct sctp_transport *);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*get_dst)(struct sctp_transport *, union sctp_addr *, struct flowi *, struct sock *);
    void (*get_saddr)(struct sctp_sock *, struct sctp_transport *, struct flowi *);
    void (*copy_addrlist)(struct list_head *, struct net_device *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *);
    void (*addr_copy)(union sctp_addr *, union sctp_addr *);
    void (*from_skb)(union sctp_addr *, struct sk_buff *, int);
    void (*from_sk)(union sctp_addr *, struct sock *);
    void (*from_addr_param)(union sctp_addr *, union sctp_addr_param *, __be16, int);
    int (*to_addr_param)(const union sctp_addr *, union sctp_addr_param *);
    int (*addr_valid)(union sctp_addr *, struct sctp_sock *, const struct sk_buff *);
    enum sctp_scope (*scope)(union sctp_addr *);
    void (*inaddr_any)(union sctp_addr *, __be16);
    int (*is_any)(const union sctp_addr *);
    int (*available)(union sctp_addr *, struct sctp_sock *);
    int (*skb_iif)(const struct sk_buff *);
    int (*is_ce)(const struct sk_buff *);
    void (*seq_dump_addr)(struct seq_file *, union sctp_addr *);
    void (*ecn_capable)(struct sock *);
    __u16 net_header_len;
    int sockaddr_len;
    int (*ip_options_len)(struct sock *);
    sa_family_t sa_family;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct sctp_af {
    int (*sctp_xmit)(struct sk_buff *, struct sctp_transport *);
    int (*setsockopt)(struct sock *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*get_dst)(struct sctp_transport *, union sctp_addr *, struct flowi *, struct sock *);
    void (*get_saddr)(struct sctp_sock *, struct sctp_transport *, struct flowi *);
    void (*copy_addrlist)(struct list_head *, struct net_device *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *);
    void (*addr_copy)(union sctp_addr *, union sctp_addr *);
    void (*from_skb)(union sctp_addr *, struct sk_buff *, int);
    void (*from_sk)(union sctp_addr *, struct sock *);
    void (*from_addr_param)(union sctp_addr *, union sctp_addr_param *, __be16, int);
    int (*to_addr_param)(const union sctp_addr *, union sctp_addr_param *);
    int (*addr_valid)(union sctp_addr *, struct sctp_sock *, const struct sk_buff *);
    enum sctp_scope (*scope)(union sctp_addr *);
    void (*inaddr_any)(union sctp_addr *, __be16);
    int (*is_any)(const union sctp_addr *);
    int (*available)(union sctp_addr *, struct sctp_sock *);
    int (*skb_iif)(const struct sk_buff *);
    int (*is_ce)(const struct sk_buff *);
    void (*seq_dump_addr)(struct seq_file *, union sctp_addr *);
    void (*ecn_capable)(struct sock *);
    __u16 net_header_len;
    int sockaddr_len;
    int (*ip_options_len)(struct sock *);
    sa_family_t sa_family;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct sctp_af {
    int (*sctp_xmit)(struct sk_buff *, struct sctp_transport *);
    int (*setsockopt)(struct sock *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*get_dst)(struct sctp_transport *, union sctp_addr *, struct flowi *, struct sock *);
    void (*get_saddr)(struct sctp_sock *, struct sctp_transport *, struct flowi *);
    void (*copy_addrlist)(struct list_head *, struct net_device *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *);
    void (*addr_copy)(union sctp_addr *, union sctp_addr *);
    void (*from_skb)(union sctp_addr *, struct sk_buff *, int);
    void (*from_sk)(union sctp_addr *, struct sock *);
    bool (*from_addr_param)(union sctp_addr *, union sctp_addr_param *, __be16, int);
    int (*to_addr_param)(const union sctp_addr *, union sctp_addr_param *);
    int (*addr_valid)(union sctp_addr *, struct sctp_sock *, const struct sk_buff *);
    enum sctp_scope (*scope)(union sctp_addr *);
    void (*inaddr_any)(union sctp_addr *, __be16);
    int (*is_any)(const union sctp_addr *);
    int (*available)(union sctp_addr *, struct sctp_sock *);
    int (*skb_iif)(const struct sk_buff *);
    int (*is_ce)(const struct sk_buff *);
    void (*seq_dump_addr)(struct seq_file *, union sctp_addr *);
    void (*ecn_capable)(struct sock *);
    __u16 net_header_len;
    int sockaddr_len;
    int (*ip_options_len)(struct sock *);
    sa_family_t sa_family;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct sctp_af {
    int (*sctp_xmit)(struct sk_buff *, struct sctp_transport *);
    int (*setsockopt)(struct sock *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*get_dst)(struct sctp_transport *, union sctp_addr *, struct flowi *, struct sock *);
    void (*get_saddr)(struct sctp_sock *, struct sctp_transport *, struct flowi *);
    void (*copy_addrlist)(struct list_head *, struct net_device *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *);
    void (*addr_copy)(union sctp_addr *, union sctp_addr *);
    void (*from_skb)(union sctp_addr *, struct sk_buff *, int);
    void (*from_sk)(union sctp_addr *, struct sock *);
    bool (*from_addr_param)(union sctp_addr *, union sctp_addr_param *, __be16, int);
    int (*to_addr_param)(const union sctp_addr *, union sctp_addr_param *);
    int (*addr_valid)(union sctp_addr *, struct sctp_sock *, const struct sk_buff *);
    enum sctp_scope (*scope)(union sctp_addr *);
    void (*inaddr_any)(union sctp_addr *, __be16);
    int (*is_any)(const union sctp_addr *);
    int (*available)(union sctp_addr *, struct sctp_sock *);
    int (*skb_iif)(const struct sk_buff *);
    int (*is_ce)(const struct sk_buff *);
    void (*seq_dump_addr)(struct seq_file *, union sctp_addr *);
    void (*ecn_capable)(struct sock *);
    __u16 net_header_len;
    int sockaddr_len;
    int (*ip_options_len)(struct sock *);
    sa_family_t sa_family;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct sctp_af {
    int (*sctp_xmit)(struct sk_buff *, struct sctp_transport *);
    int (*setsockopt)(struct sock *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*get_dst)(struct sctp_transport *, union sctp_addr *, struct flowi *, struct sock *);
    void (*get_saddr)(struct sctp_sock *, struct sctp_transport *, struct flowi *);
    void (*copy_addrlist)(struct list_head *, struct net_device *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *);
    void (*addr_copy)(union sctp_addr *, union sctp_addr *);
    void (*from_skb)(union sctp_addr *, struct sk_buff *, int);
    void (*from_sk)(union sctp_addr *, struct sock *);
    bool (*from_addr_param)(union sctp_addr *, union sctp_addr_param *, __be16, int);
    int (*to_addr_param)(const union sctp_addr *, union sctp_addr_param *);
    int (*addr_valid)(union sctp_addr *, struct sctp_sock *, const struct sk_buff *);
    enum sctp_scope (*scope)(union sctp_addr *);
    void (*inaddr_any)(union sctp_addr *, __be16);
    int (*is_any)(const union sctp_addr *);
    int (*available)(union sctp_addr *, struct sctp_sock *);
    int (*skb_iif)(const struct sk_buff *);
    int (*is_ce)(const struct sk_buff *);
    void (*seq_dump_addr)(struct seq_file *, union sctp_addr *);
    void (*ecn_capable)(struct sock *);
    __u16 net_header_len;
    int sockaddr_len;
    int (*ip_options_len)(struct sock *);
    sa_family_t sa_family;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct sctp_af {
    int (*sctp_xmit)(struct sk_buff *, struct sctp_transport *);
    int (*setsockopt)(struct sock *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*get_dst)(struct sctp_transport *, union sctp_addr *, struct flowi *, struct sock *);
    void (*get_saddr)(struct sctp_sock *, struct sctp_transport *, struct flowi *);
    void (*copy_addrlist)(struct list_head *, struct net_device *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *);
    void (*addr_copy)(union sctp_addr *, union sctp_addr *);
    void (*from_skb)(union sctp_addr *, struct sk_buff *, int);
    void (*from_sk)(union sctp_addr *, struct sock *);
    bool (*from_addr_param)(union sctp_addr *, union sctp_addr_param *, __be16, int);
    int (*to_addr_param)(const union sctp_addr *, union sctp_addr_param *);
    int (*addr_valid)(union sctp_addr *, struct sctp_sock *, const struct sk_buff *);
    enum sctp_scope (*scope)(union sctp_addr *);
    void (*inaddr_any)(union sctp_addr *, __be16);
    int (*is_any)(const union sctp_addr *);
    int (*available)(union sctp_addr *, struct sctp_sock *);
    int (*skb_iif)(const struct sk_buff *);
    int (*skb_sdif)(const struct sk_buff *);
    int (*is_ce)(const struct sk_buff *);
    void (*seq_dump_addr)(struct seq_file *, union sctp_addr *);
    void (*ecn_capable)(struct sock *);
    __u16 net_header_len;
    int sockaddr_len;
    int (*ip_options_len)(struct sock *);
    sa_family_t sa_family;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct sctp_af {
    int (*sctp_xmit)(struct sk_buff *, struct sctp_transport *);
    int (*setsockopt)(struct sock *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*get_dst)(struct sctp_transport *, union sctp_addr *, struct flowi *, struct sock *);
    void (*get_saddr)(struct sctp_sock *, struct sctp_transport *, struct flowi *);
    void (*copy_addrlist)(struct list_head *, struct net_device *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *);
    void (*addr_copy)(union sctp_addr *, union sctp_addr *);
    void (*from_skb)(union sctp_addr *, struct sk_buff *, int);
    void (*from_sk)(union sctp_addr *, struct sock *);
    bool (*from_addr_param)(union sctp_addr *, union sctp_addr_param *, __be16, int);
    int (*to_addr_param)(const union sctp_addr *, union sctp_addr_param *);
    int (*addr_valid)(union sctp_addr *, struct sctp_sock *, const struct sk_buff *);
    enum sctp_scope (*scope)(union sctp_addr *);
    void (*inaddr_any)(union sctp_addr *, __be16);
    int (*is_any)(const union sctp_addr *);
    int (*available)(union sctp_addr *, struct sctp_sock *);
    int (*skb_iif)(const struct sk_buff *);
    int (*skb_sdif)(const struct sk_buff *);
    int (*is_ce)(const struct sk_buff *);
    void (*seq_dump_addr)(struct seq_file *, union sctp_addr *);
    void (*ecn_capable)(struct sock *);
    __u16 net_header_len;
    int sockaddr_len;
    int (*ip_options_len)(struct sock *);
    sa_family_t sa_family;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct sctp_af {
    int (*sctp_xmit)(struct sk_buff *, struct sctp_transport *);
    int (*setsockopt)(struct sock *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*get_dst)(struct sctp_transport *, union sctp_addr *, struct flowi *, struct sock *);
    void (*get_saddr)(struct sctp_sock *, struct sctp_transport *, struct flowi *);
    void (*copy_addrlist)(struct list_head *, struct net_device *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *);
    void (*addr_copy)(union sctp_addr *, union sctp_addr *);
    void (*from_skb)(union sctp_addr *, struct sk_buff *, int);
    void (*from_sk)(union sctp_addr *, struct sock *);
    bool (*from_addr_param)(union sctp_addr *, union sctp_addr_param *, __be16, int);
    int (*to_addr_param)(const union sctp_addr *, union sctp_addr_param *);
    int (*addr_valid)(union sctp_addr *, struct sctp_sock *, const struct sk_buff *);
    enum sctp_scope (*scope)(union sctp_addr *);
    void (*inaddr_any)(union sctp_addr *, __be16);
    int (*is_any)(const union sctp_addr *);
    int (*available)(union sctp_addr *, struct sctp_sock *);
    int (*skb_iif)(const struct sk_buff *);
    int (*skb_sdif)(const struct sk_buff *);
    int (*is_ce)(const struct sk_buff *);
    void (*seq_dump_addr)(struct seq_file *, union sctp_addr *);
    void (*ecn_capable)(struct sock *);
    __u16 net_header_len;
    int sockaddr_len;
    int (*ip_options_len)(struct sock *);
    sa_family_t sa_family;
    struct list_head list;
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
struct sctp_af {
    int (*sctp_xmit)(struct sk_buff *, struct sctp_transport *);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*get_dst)(struct sctp_transport *, union sctp_addr *, struct flowi *, struct sock *);
    void (*get_saddr)(struct sctp_sock *, struct sctp_transport *, struct flowi *);
    void (*copy_addrlist)(struct list_head *, struct net_device *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *);
    void (*addr_copy)(union sctp_addr *, union sctp_addr *);
    void (*from_skb)(union sctp_addr *, struct sk_buff *, int);
    void (*from_sk)(union sctp_addr *, struct sock *);
    void (*from_addr_param)(union sctp_addr *, union sctp_addr_param *, __be16, int);
    int (*to_addr_param)(const union sctp_addr *, union sctp_addr_param *);
    int (*addr_valid)(union sctp_addr *, struct sctp_sock *, const struct sk_buff *);
    enum sctp_scope (*scope)(union sctp_addr *);
    void (*inaddr_any)(union sctp_addr *, __be16);
    int (*is_any)(const union sctp_addr *);
    int (*available)(union sctp_addr *, struct sctp_sock *);
    int (*skb_iif)(const struct sk_buff *);
    int (*is_ce)(const struct sk_buff *);
    void (*seq_dump_addr)(struct seq_file *, union sctp_addr *);
    void (*ecn_capable)(struct sock *);
    __u16 net_header_len;
    int sockaddr_len;
    int (*ip_options_len)(struct sock *);
    sa_family_t sa_family;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct sctp_af {
    int (*sctp_xmit)(struct sk_buff *, struct sctp_transport *);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*get_dst)(struct sctp_transport *, union sctp_addr *, struct flowi *, struct sock *);
    void (*get_saddr)(struct sctp_sock *, struct sctp_transport *, struct flowi *);
    void (*copy_addrlist)(struct list_head *, struct net_device *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *);
    void (*addr_copy)(union sctp_addr *, union sctp_addr *);
    void (*from_skb)(union sctp_addr *, struct sk_buff *, int);
    void (*from_sk)(union sctp_addr *, struct sock *);
    void (*from_addr_param)(union sctp_addr *, union sctp_addr_param *, __be16, int);
    int (*to_addr_param)(const union sctp_addr *, union sctp_addr_param *);
    int (*addr_valid)(union sctp_addr *, struct sctp_sock *, const struct sk_buff *);
    enum sctp_scope (*scope)(union sctp_addr *);
    void (*inaddr_any)(union sctp_addr *, __be16);
    int (*is_any)(const union sctp_addr *);
    int (*available)(union sctp_addr *, struct sctp_sock *);
    int (*skb_iif)(const struct sk_buff *);
    int (*is_ce)(const struct sk_buff *);
    void (*seq_dump_addr)(struct seq_file *, union sctp_addr *);
    void (*ecn_capable)(struct sock *);
    __u16 net_header_len;
    int sockaddr_len;
    int (*ip_options_len)(struct sock *);
    sa_family_t sa_family;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct sctp_af {
    int (*sctp_xmit)(struct sk_buff *, struct sctp_transport *);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*get_dst)(struct sctp_transport *, union sctp_addr *, struct flowi *, struct sock *);
    void (*get_saddr)(struct sctp_sock *, struct sctp_transport *, struct flowi *);
    void (*copy_addrlist)(struct list_head *, struct net_device *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *);
    void (*addr_copy)(union sctp_addr *, union sctp_addr *);
    void (*from_skb)(union sctp_addr *, struct sk_buff *, int);
    void (*from_sk)(union sctp_addr *, struct sock *);
    void (*from_addr_param)(union sctp_addr *, union sctp_addr_param *, __be16, int);
    int (*to_addr_param)(const union sctp_addr *, union sctp_addr_param *);
    int (*addr_valid)(union sctp_addr *, struct sctp_sock *, const struct sk_buff *);
    enum sctp_scope (*scope)(union sctp_addr *);
    void (*inaddr_any)(union sctp_addr *, __be16);
    int (*is_any)(const union sctp_addr *);
    int (*available)(union sctp_addr *, struct sctp_sock *);
    int (*skb_iif)(const struct sk_buff *);
    int (*is_ce)(const struct sk_buff *);
    void (*seq_dump_addr)(struct seq_file *, union sctp_addr *);
    void (*ecn_capable)(struct sock *);
    __u16 net_header_len;
    int sockaddr_len;
    int (*ip_options_len)(struct sock *);
    sa_family_t sa_family;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct sctp_af {
    int (*sctp_xmit)(struct sk_buff *, struct sctp_transport *);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*get_dst)(struct sctp_transport *, union sctp_addr *, struct flowi *, struct sock *);
    void (*get_saddr)(struct sctp_sock *, struct sctp_transport *, struct flowi *);
    void (*copy_addrlist)(struct list_head *, struct net_device *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *);
    void (*addr_copy)(union sctp_addr *, union sctp_addr *);
    void (*from_skb)(union sctp_addr *, struct sk_buff *, int);
    void (*from_sk)(union sctp_addr *, struct sock *);
    void (*from_addr_param)(union sctp_addr *, union sctp_addr_param *, __be16, int);
    int (*to_addr_param)(const union sctp_addr *, union sctp_addr_param *);
    int (*addr_valid)(union sctp_addr *, struct sctp_sock *, const struct sk_buff *);
    enum sctp_scope (*scope)(union sctp_addr *);
    void (*inaddr_any)(union sctp_addr *, __be16);
    int (*is_any)(const union sctp_addr *);
    int (*available)(union sctp_addr *, struct sctp_sock *);
    int (*skb_iif)(const struct sk_buff *);
    int (*is_ce)(const struct sk_buff *);
    void (*seq_dump_addr)(struct seq_file *, union sctp_addr *);
    void (*ecn_capable)(struct sock *);
    __u16 net_header_len;
    int sockaddr_len;
    int (*ip_options_len)(struct sock *);
    sa_family_t sa_family;
    struct list_head list;
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
struct sctp_af {
    int (*sctp_xmit)(struct sk_buff *, struct sctp_transport *);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*get_dst)(struct sctp_transport *, union sctp_addr *, struct flowi *, struct sock *);
    void (*get_saddr)(struct sctp_sock *, struct sctp_transport *, struct flowi *);
    void (*copy_addrlist)(struct list_head *, struct net_device *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *);
    void (*addr_copy)(union sctp_addr *, union sctp_addr *);
    void (*from_skb)(union sctp_addr *, struct sk_buff *, int);
    void (*from_sk)(union sctp_addr *, struct sock *);
    void (*from_addr_param)(union sctp_addr *, union sctp_addr_param *, __be16, int);
    int (*to_addr_param)(const union sctp_addr *, union sctp_addr_param *);
    int (*addr_valid)(union sctp_addr *, struct sctp_sock *, const struct sk_buff *);
    enum sctp_scope (*scope)(union sctp_addr *);
    void (*inaddr_any)(union sctp_addr *, __be16);
    int (*is_any)(const union sctp_addr *);
    int (*available)(union sctp_addr *, struct sctp_sock *);
    int (*skb_iif)(const struct sk_buff *);
    int (*is_ce)(const struct sk_buff *);
    void (*seq_dump_addr)(struct seq_file *, union sctp_addr *);
    void (*ecn_capable)(struct sock *);
    __u16 net_header_len;
    int sockaddr_len;
    int (*ip_options_len)(struct sock *);
    sa_family_t sa_family;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct sctp_af {
    int (*sctp_xmit)(struct sk_buff *, struct sctp_transport *);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*get_dst)(struct sctp_transport *, union sctp_addr *, struct flowi *, struct sock *);
    void (*get_saddr)(struct sctp_sock *, struct sctp_transport *, struct flowi *);
    void (*copy_addrlist)(struct list_head *, struct net_device *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *);
    void (*addr_copy)(union sctp_addr *, union sctp_addr *);
    void (*from_skb)(union sctp_addr *, struct sk_buff *, int);
    void (*from_sk)(union sctp_addr *, struct sock *);
    void (*from_addr_param)(union sctp_addr *, union sctp_addr_param *, __be16, int);
    int (*to_addr_param)(const union sctp_addr *, union sctp_addr_param *);
    int (*addr_valid)(union sctp_addr *, struct sctp_sock *, const struct sk_buff *);
    enum sctp_scope (*scope)(union sctp_addr *);
    void (*inaddr_any)(union sctp_addr *, __be16);
    int (*is_any)(const union sctp_addr *);
    int (*available)(union sctp_addr *, struct sctp_sock *);
    int (*skb_iif)(const struct sk_buff *);
    int (*is_ce)(const struct sk_buff *);
    void (*seq_dump_addr)(struct seq_file *, union sctp_addr *);
    void (*ecn_capable)(struct sock *);
    __u16 net_header_len;
    int sockaddr_len;
    int (*ip_options_len)(struct sock *);
    sa_family_t sa_family;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct sctp_af {
    int (*sctp_xmit)(struct sk_buff *, struct sctp_transport *);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*get_dst)(struct sctp_transport *, union sctp_addr *, struct flowi *, struct sock *);
    void (*get_saddr)(struct sctp_sock *, struct sctp_transport *, struct flowi *);
    void (*copy_addrlist)(struct list_head *, struct net_device *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *);
    void (*addr_copy)(union sctp_addr *, union sctp_addr *);
    void (*from_skb)(union sctp_addr *, struct sk_buff *, int);
    void (*from_sk)(union sctp_addr *, struct sock *);
    void (*from_addr_param)(union sctp_addr *, union sctp_addr_param *, __be16, int);
    int (*to_addr_param)(const union sctp_addr *, union sctp_addr_param *);
    int (*addr_valid)(union sctp_addr *, struct sctp_sock *, const struct sk_buff *);
    enum sctp_scope (*scope)(union sctp_addr *);
    void (*inaddr_any)(union sctp_addr *, __be16);
    int (*is_any)(const union sctp_addr *);
    int (*available)(union sctp_addr *, struct sctp_sock *);
    int (*skb_iif)(const struct sk_buff *);
    int (*is_ce)(const struct sk_buff *);
    void (*seq_dump_addr)(struct seq_file *, union sctp_addr *);
    void (*ecn_capable)(struct sock *);
    __u16 net_header_len;
    int sockaddr_len;
    int (*ip_options_len)(struct sock *);
    sa_family_t sa_family;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct sctp_af {
    int (*sctp_xmit)(struct sk_buff *, struct sctp_transport *);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    void (*get_dst)(struct sctp_transport *, union sctp_addr *, struct flowi *, struct sock *);
    void (*get_saddr)(struct sctp_sock *, struct sctp_transport *, struct flowi *);
    void (*copy_addrlist)(struct list_head *, struct net_device *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *);
    void (*addr_copy)(union sctp_addr *, union sctp_addr *);
    void (*from_skb)(union sctp_addr *, struct sk_buff *, int);
    void (*from_sk)(union sctp_addr *, struct sock *);
    void (*from_addr_param)(union sctp_addr *, union sctp_addr_param *, __be16, int);
    int (*to_addr_param)(const union sctp_addr *, union sctp_addr_param *);
    int (*addr_valid)(union sctp_addr *, struct sctp_sock *, const struct sk_buff *);
    enum sctp_scope (*scope)(union sctp_addr *);
    void (*inaddr_any)(union sctp_addr *, __be16);
    int (*is_any)(const union sctp_addr *);
    int (*available)(union sctp_addr *, struct sctp_sock *);
    int (*skb_iif)(const struct sk_buff *);
    int (*is_ce)(const struct sk_buff *);
    void (*seq_dump_addr)(struct seq_file *, union sctp_addr *);
    void (*ecn_capable)(struct sock *);
    __u16 net_header_len;
    int sockaddr_len;
    int (*ip_options_len)(struct sock *);
    sa_family_t sa_family;
    struct list_head list;
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
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>void (*from_addr_param)(union sctp_addr *, union sctp_addr_param *, __be16, int)</code> ➡️ <code>bool (*from_addr_param)(union sctp_addr *, union sctp_addr_param *, __be16, int)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*skb_sdif)(const struct sk_buff *)</code>
</li>
</ul>
</details>
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
