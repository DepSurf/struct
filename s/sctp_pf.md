# Struct: <code>sctp_pf</code>

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
struct sctp_pf {
    void (*event_msgname)(struct sctp_ulpevent *, char *, int *);
    void (*skb_msgname)(struct sk_buff *, char *, int *);
    int (*af_supported)(sa_family_t, struct sctp_sock *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *, struct sctp_sock *);
    int (*bind_verify)(struct sctp_sock *, union sctp_addr *);
    int (*send_verify)(struct sctp_sock *, union sctp_addr *);
    int (*supported_addrs)(const struct sctp_sock *, __be16 *);
    struct sock * (*create_accept_sk)(struct sock *, struct sctp_association *, bool);
    int (*addr_to_user)(struct sctp_sock *, union sctp_addr *);
    void (*to_sk_saddr)(union sctp_addr *, struct sock *);
    void (*to_sk_daddr)(union sctp_addr *, struct sock *);
    void (*copy_ip_options)(struct sock *, struct sock *);
    struct sctp_af *af;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct sctp_pf {
    void (*event_msgname)(struct sctp_ulpevent *, char *, int *);
    void (*skb_msgname)(struct sk_buff *, char *, int *);
    int (*af_supported)(sa_family_t, struct sctp_sock *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *, struct sctp_sock *);
    int (*bind_verify)(struct sctp_sock *, union sctp_addr *);
    int (*send_verify)(struct sctp_sock *, union sctp_addr *);
    int (*supported_addrs)(const struct sctp_sock *, __be16 *);
    struct sock * (*create_accept_sk)(struct sock *, struct sctp_association *, bool);
    int (*addr_to_user)(struct sctp_sock *, union sctp_addr *);
    void (*to_sk_saddr)(union sctp_addr *, struct sock *);
    void (*to_sk_daddr)(union sctp_addr *, struct sock *);
    void (*copy_ip_options)(struct sock *, struct sock *);
    struct sctp_af *af;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct sctp_pf {
    void (*event_msgname)(struct sctp_ulpevent *, char *, int *);
    void (*skb_msgname)(struct sk_buff *, char *, int *);
    int (*af_supported)(sa_family_t, struct sctp_sock *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *, struct sctp_sock *);
    int (*bind_verify)(struct sctp_sock *, union sctp_addr *);
    int (*send_verify)(struct sctp_sock *, union sctp_addr *);
    int (*supported_addrs)(const struct sctp_sock *, __be16 *);
    struct sock * (*create_accept_sk)(struct sock *, struct sctp_association *, bool);
    int (*addr_to_user)(struct sctp_sock *, union sctp_addr *);
    void (*to_sk_saddr)(union sctp_addr *, struct sock *);
    void (*to_sk_daddr)(union sctp_addr *, struct sock *);
    void (*copy_ip_options)(struct sock *, struct sock *);
    struct sctp_af *af;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct sctp_pf {
    void (*event_msgname)(struct sctp_ulpevent *, char *, int *);
    void (*skb_msgname)(struct sk_buff *, char *, int *);
    int (*af_supported)(sa_family_t, struct sctp_sock *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *, struct sctp_sock *);
    int (*bind_verify)(struct sctp_sock *, union sctp_addr *);
    int (*send_verify)(struct sctp_sock *, union sctp_addr *);
    int (*supported_addrs)(const struct sctp_sock *, __be16 *);
    struct sock * (*create_accept_sk)(struct sock *, struct sctp_association *, bool);
    int (*addr_to_user)(struct sctp_sock *, union sctp_addr *);
    void (*to_sk_saddr)(union sctp_addr *, struct sock *);
    void (*to_sk_daddr)(union sctp_addr *, struct sock *);
    void (*copy_ip_options)(struct sock *, struct sock *);
    struct sctp_af *af;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct sctp_pf {
    void (*event_msgname)(struct sctp_ulpevent *, char *, int *);
    void (*skb_msgname)(struct sk_buff *, char *, int *);
    int (*af_supported)(sa_family_t, struct sctp_sock *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *, struct sctp_sock *);
    int (*bind_verify)(struct sctp_sock *, union sctp_addr *);
    int (*send_verify)(struct sctp_sock *, union sctp_addr *);
    int (*supported_addrs)(const struct sctp_sock *, __be16 *);
    struct sock * (*create_accept_sk)(struct sock *, struct sctp_association *, bool);
    int (*addr_to_user)(struct sctp_sock *, union sctp_addr *);
    void (*to_sk_saddr)(union sctp_addr *, struct sock *);
    void (*to_sk_daddr)(union sctp_addr *, struct sock *);
    void (*copy_ip_options)(struct sock *, struct sock *);
    struct sctp_af *af;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct sctp_pf {
    void (*event_msgname)(struct sctp_ulpevent *, char *, int *);
    void (*skb_msgname)(struct sk_buff *, char *, int *);
    int (*af_supported)(sa_family_t, struct sctp_sock *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *, struct sctp_sock *);
    int (*bind_verify)(struct sctp_sock *, union sctp_addr *);
    int (*send_verify)(struct sctp_sock *, union sctp_addr *);
    int (*supported_addrs)(const struct sctp_sock *, __be16 *);
    struct sock * (*create_accept_sk)(struct sock *, struct sctp_association *, bool);
    int (*addr_to_user)(struct sctp_sock *, union sctp_addr *);
    void (*to_sk_saddr)(union sctp_addr *, struct sock *);
    void (*to_sk_daddr)(union sctp_addr *, struct sock *);
    void (*copy_ip_options)(struct sock *, struct sock *);
    struct sctp_af *af;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct sctp_pf {
    void (*event_msgname)(struct sctp_ulpevent *, char *, int *);
    void (*skb_msgname)(struct sk_buff *, char *, int *);
    int (*af_supported)(sa_family_t, struct sctp_sock *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *, struct sctp_sock *);
    int (*bind_verify)(struct sctp_sock *, union sctp_addr *);
    int (*send_verify)(struct sctp_sock *, union sctp_addr *);
    int (*supported_addrs)(const struct sctp_sock *, __be16 *);
    struct sock * (*create_accept_sk)(struct sock *, struct sctp_association *, bool);
    int (*addr_to_user)(struct sctp_sock *, union sctp_addr *);
    void (*to_sk_saddr)(union sctp_addr *, struct sock *);
    void (*to_sk_daddr)(union sctp_addr *, struct sock *);
    void (*copy_ip_options)(struct sock *, struct sock *);
    struct sctp_af *af;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct sctp_pf {
    void (*event_msgname)(struct sctp_ulpevent *, char *, int *);
    void (*skb_msgname)(struct sk_buff *, char *, int *);
    int (*af_supported)(sa_family_t, struct sctp_sock *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *, struct sctp_sock *);
    int (*bind_verify)(struct sctp_sock *, union sctp_addr *);
    int (*send_verify)(struct sctp_sock *, union sctp_addr *);
    int (*supported_addrs)(const struct sctp_sock *, __be16 *);
    struct sock * (*create_accept_sk)(struct sock *, struct sctp_association *, bool);
    int (*addr_to_user)(struct sctp_sock *, union sctp_addr *);
    void (*to_sk_saddr)(union sctp_addr *, struct sock *);
    void (*to_sk_daddr)(union sctp_addr *, struct sock *);
    void (*copy_ip_options)(struct sock *, struct sock *);
    struct sctp_af *af;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct sctp_pf {
    void (*event_msgname)(struct sctp_ulpevent *, char *, int *);
    void (*skb_msgname)(struct sk_buff *, char *, int *);
    int (*af_supported)(sa_family_t, struct sctp_sock *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *, struct sctp_sock *);
    int (*bind_verify)(struct sctp_sock *, union sctp_addr *);
    int (*send_verify)(struct sctp_sock *, union sctp_addr *);
    int (*supported_addrs)(const struct sctp_sock *, __be16 *);
    struct sock * (*create_accept_sk)(struct sock *, struct sctp_association *, bool);
    int (*addr_to_user)(struct sctp_sock *, union sctp_addr *);
    void (*to_sk_saddr)(union sctp_addr *, struct sock *);
    void (*to_sk_daddr)(union sctp_addr *, struct sock *);
    void (*copy_ip_options)(struct sock *, struct sock *);
    struct sctp_af *af;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct sctp_pf {
    void (*event_msgname)(struct sctp_ulpevent *, char *, int *);
    void (*skb_msgname)(struct sk_buff *, char *, int *);
    int (*af_supported)(sa_family_t, struct sctp_sock *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *, struct sctp_sock *);
    int (*bind_verify)(struct sctp_sock *, union sctp_addr *);
    int (*send_verify)(struct sctp_sock *, union sctp_addr *);
    int (*supported_addrs)(const struct sctp_sock *, __be16 *);
    struct sock * (*create_accept_sk)(struct sock *, struct sctp_association *, bool);
    int (*addr_to_user)(struct sctp_sock *, union sctp_addr *);
    void (*to_sk_saddr)(union sctp_addr *, struct sock *);
    void (*to_sk_daddr)(union sctp_addr *, struct sock *);
    void (*copy_ip_options)(struct sock *, struct sock *);
    struct sctp_af *af;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct sctp_pf {
    void (*event_msgname)(struct sctp_ulpevent *, char *, int *);
    void (*skb_msgname)(struct sk_buff *, char *, int *);
    int (*af_supported)(sa_family_t, struct sctp_sock *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *, struct sctp_sock *);
    int (*bind_verify)(struct sctp_sock *, union sctp_addr *);
    int (*send_verify)(struct sctp_sock *, union sctp_addr *);
    int (*supported_addrs)(const struct sctp_sock *, __be16 *);
    struct sock * (*create_accept_sk)(struct sock *, struct sctp_association *, bool);
    int (*addr_to_user)(struct sctp_sock *, union sctp_addr *);
    void (*to_sk_saddr)(union sctp_addr *, struct sock *);
    void (*to_sk_daddr)(union sctp_addr *, struct sock *);
    void (*copy_ip_options)(struct sock *, struct sock *);
    struct sctp_af *af;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct sctp_pf {
    void (*event_msgname)(struct sctp_ulpevent *, char *, int *);
    void (*skb_msgname)(struct sk_buff *, char *, int *);
    int (*af_supported)(sa_family_t, struct sctp_sock *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *, struct sctp_sock *);
    int (*bind_verify)(struct sctp_sock *, union sctp_addr *);
    int (*send_verify)(struct sctp_sock *, union sctp_addr *);
    int (*supported_addrs)(const struct sctp_sock *, __be16 *);
    struct sock * (*create_accept_sk)(struct sock *, struct sctp_association *, bool);
    int (*addr_to_user)(struct sctp_sock *, union sctp_addr *);
    void (*to_sk_saddr)(union sctp_addr *, struct sock *);
    void (*to_sk_daddr)(union sctp_addr *, struct sock *);
    void (*copy_ip_options)(struct sock *, struct sock *);
    struct sctp_af *af;
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
struct sctp_pf {
    void (*event_msgname)(struct sctp_ulpevent *, char *, int *);
    void (*skb_msgname)(struct sk_buff *, char *, int *);
    int (*af_supported)(sa_family_t, struct sctp_sock *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *, struct sctp_sock *);
    int (*bind_verify)(struct sctp_sock *, union sctp_addr *);
    int (*send_verify)(struct sctp_sock *, union sctp_addr *);
    int (*supported_addrs)(const struct sctp_sock *, __be16 *);
    struct sock * (*create_accept_sk)(struct sock *, struct sctp_association *, bool);
    int (*addr_to_user)(struct sctp_sock *, union sctp_addr *);
    void (*to_sk_saddr)(union sctp_addr *, struct sock *);
    void (*to_sk_daddr)(union sctp_addr *, struct sock *);
    void (*copy_ip_options)(struct sock *, struct sock *);
    struct sctp_af *af;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct sctp_pf {
    void (*event_msgname)(struct sctp_ulpevent *, char *, int *);
    void (*skb_msgname)(struct sk_buff *, char *, int *);
    int (*af_supported)(sa_family_t, struct sctp_sock *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *, struct sctp_sock *);
    int (*bind_verify)(struct sctp_sock *, union sctp_addr *);
    int (*send_verify)(struct sctp_sock *, union sctp_addr *);
    int (*supported_addrs)(const struct sctp_sock *, __be16 *);
    struct sock * (*create_accept_sk)(struct sock *, struct sctp_association *, bool);
    int (*addr_to_user)(struct sctp_sock *, union sctp_addr *);
    void (*to_sk_saddr)(union sctp_addr *, struct sock *);
    void (*to_sk_daddr)(union sctp_addr *, struct sock *);
    void (*copy_ip_options)(struct sock *, struct sock *);
    struct sctp_af *af;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct sctp_pf {
    void (*event_msgname)(struct sctp_ulpevent *, char *, int *);
    void (*skb_msgname)(struct sk_buff *, char *, int *);
    int (*af_supported)(sa_family_t, struct sctp_sock *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *, struct sctp_sock *);
    int (*bind_verify)(struct sctp_sock *, union sctp_addr *);
    int (*send_verify)(struct sctp_sock *, union sctp_addr *);
    int (*supported_addrs)(const struct sctp_sock *, __be16 *);
    struct sock * (*create_accept_sk)(struct sock *, struct sctp_association *, bool);
    int (*addr_to_user)(struct sctp_sock *, union sctp_addr *);
    void (*to_sk_saddr)(union sctp_addr *, struct sock *);
    void (*to_sk_daddr)(union sctp_addr *, struct sock *);
    void (*copy_ip_options)(struct sock *, struct sock *);
    struct sctp_af *af;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct sctp_pf {
    void (*event_msgname)(struct sctp_ulpevent *, char *, int *);
    void (*skb_msgname)(struct sk_buff *, char *, int *);
    int (*af_supported)(sa_family_t, struct sctp_sock *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *, struct sctp_sock *);
    int (*bind_verify)(struct sctp_sock *, union sctp_addr *);
    int (*send_verify)(struct sctp_sock *, union sctp_addr *);
    int (*supported_addrs)(const struct sctp_sock *, __be16 *);
    struct sock * (*create_accept_sk)(struct sock *, struct sctp_association *, bool);
    int (*addr_to_user)(struct sctp_sock *, union sctp_addr *);
    void (*to_sk_saddr)(union sctp_addr *, struct sock *);
    void (*to_sk_daddr)(union sctp_addr *, struct sock *);
    void (*copy_ip_options)(struct sock *, struct sock *);
    struct sctp_af *af;
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
struct sctp_pf {
    void (*event_msgname)(struct sctp_ulpevent *, char *, int *);
    void (*skb_msgname)(struct sk_buff *, char *, int *);
    int (*af_supported)(sa_family_t, struct sctp_sock *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *, struct sctp_sock *);
    int (*bind_verify)(struct sctp_sock *, union sctp_addr *);
    int (*send_verify)(struct sctp_sock *, union sctp_addr *);
    int (*supported_addrs)(const struct sctp_sock *, __be16 *);
    struct sock * (*create_accept_sk)(struct sock *, struct sctp_association *, bool);
    int (*addr_to_user)(struct sctp_sock *, union sctp_addr *);
    void (*to_sk_saddr)(union sctp_addr *, struct sock *);
    void (*to_sk_daddr)(union sctp_addr *, struct sock *);
    void (*copy_ip_options)(struct sock *, struct sock *);
    struct sctp_af *af;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct sctp_pf {
    void (*event_msgname)(struct sctp_ulpevent *, char *, int *);
    void (*skb_msgname)(struct sk_buff *, char *, int *);
    int (*af_supported)(sa_family_t, struct sctp_sock *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *, struct sctp_sock *);
    int (*bind_verify)(struct sctp_sock *, union sctp_addr *);
    int (*send_verify)(struct sctp_sock *, union sctp_addr *);
    int (*supported_addrs)(const struct sctp_sock *, __be16 *);
    struct sock * (*create_accept_sk)(struct sock *, struct sctp_association *, bool);
    int (*addr_to_user)(struct sctp_sock *, union sctp_addr *);
    void (*to_sk_saddr)(union sctp_addr *, struct sock *);
    void (*to_sk_daddr)(union sctp_addr *, struct sock *);
    void (*copy_ip_options)(struct sock *, struct sock *);
    struct sctp_af *af;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct sctp_pf {
    void (*event_msgname)(struct sctp_ulpevent *, char *, int *);
    void (*skb_msgname)(struct sk_buff *, char *, int *);
    int (*af_supported)(sa_family_t, struct sctp_sock *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *, struct sctp_sock *);
    int (*bind_verify)(struct sctp_sock *, union sctp_addr *);
    int (*send_verify)(struct sctp_sock *, union sctp_addr *);
    int (*supported_addrs)(const struct sctp_sock *, __be16 *);
    struct sock * (*create_accept_sk)(struct sock *, struct sctp_association *, bool);
    int (*addr_to_user)(struct sctp_sock *, union sctp_addr *);
    void (*to_sk_saddr)(union sctp_addr *, struct sock *);
    void (*to_sk_daddr)(union sctp_addr *, struct sock *);
    void (*copy_ip_options)(struct sock *, struct sock *);
    struct sctp_af *af;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct sctp_pf {
    void (*event_msgname)(struct sctp_ulpevent *, char *, int *);
    void (*skb_msgname)(struct sk_buff *, char *, int *);
    int (*af_supported)(sa_family_t, struct sctp_sock *);
    int (*cmp_addr)(const union sctp_addr *, const union sctp_addr *, struct sctp_sock *);
    int (*bind_verify)(struct sctp_sock *, union sctp_addr *);
    int (*send_verify)(struct sctp_sock *, union sctp_addr *);
    int (*supported_addrs)(const struct sctp_sock *, __be16 *);
    struct sock * (*create_accept_sk)(struct sock *, struct sctp_association *, bool);
    int (*addr_to_user)(struct sctp_sock *, union sctp_addr *);
    void (*to_sk_saddr)(union sctp_addr *, struct sock *);
    void (*to_sk_daddr)(union sctp_addr *, struct sock *);
    void (*copy_ip_options)(struct sock *, struct sock *);
    struct sctp_af *af;
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
