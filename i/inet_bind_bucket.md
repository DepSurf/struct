# Struct: <code>inet_bind_bucket</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct inet_bind_bucket {
    possible_net_t ib_net;
    short unsigned int port;
    signed char fastreuse;
    signed char fastreuseport;
    kuid_t fastuid;
    int num_owners;
    struct hlist_node node;
    struct hlist_head owners;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct inet_bind_bucket {
    possible_net_t ib_net;
    short unsigned int port;
    signed char fastreuse;
    signed char fastreuseport;
    kuid_t fastuid;
    int num_owners;
    struct hlist_node node;
    struct hlist_head owners;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct inet_bind_bucket {
    possible_net_t ib_net;
    short unsigned int port;
    signed char fastreuse;
    signed char fastreuseport;
    kuid_t fastuid;
    int num_owners;
    struct hlist_node node;
    struct hlist_head owners;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct inet_bind_bucket {
    possible_net_t ib_net;
    short unsigned int port;
    signed char fastreuse;
    signed char fastreuseport;
    kuid_t fastuid;
    struct in6_addr fast_v6_rcv_saddr;
    __be32 fast_rcv_saddr;
    short unsigned int fast_sk_family;
    bool fast_ipv6_only;
    struct hlist_node node;
    struct hlist_head owners;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct inet_bind_bucket {
    possible_net_t ib_net;
    short unsigned int port;
    signed char fastreuse;
    signed char fastreuseport;
    kuid_t fastuid;
    struct in6_addr fast_v6_rcv_saddr;
    __be32 fast_rcv_saddr;
    short unsigned int fast_sk_family;
    bool fast_ipv6_only;
    struct hlist_node node;
    struct hlist_head owners;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct inet_bind_bucket {
    possible_net_t ib_net;
    short unsigned int port;
    signed char fastreuse;
    signed char fastreuseport;
    kuid_t fastuid;
    struct in6_addr fast_v6_rcv_saddr;
    __be32 fast_rcv_saddr;
    short unsigned int fast_sk_family;
    bool fast_ipv6_only;
    struct hlist_node node;
    struct hlist_head owners;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct inet_bind_bucket {
    possible_net_t ib_net;
    int l3mdev;
    short unsigned int port;
    signed char fastreuse;
    signed char fastreuseport;
    kuid_t fastuid;
    struct in6_addr fast_v6_rcv_saddr;
    __be32 fast_rcv_saddr;
    short unsigned int fast_sk_family;
    bool fast_ipv6_only;
    struct hlist_node node;
    struct hlist_head owners;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct inet_bind_bucket {
    possible_net_t ib_net;
    int l3mdev;
    short unsigned int port;
    signed char fastreuse;
    signed char fastreuseport;
    kuid_t fastuid;
    struct in6_addr fast_v6_rcv_saddr;
    __be32 fast_rcv_saddr;
    short unsigned int fast_sk_family;
    bool fast_ipv6_only;
    struct hlist_node node;
    struct hlist_head owners;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct inet_bind_bucket {
    possible_net_t ib_net;
    int l3mdev;
    short unsigned int port;
    signed char fastreuse;
    signed char fastreuseport;
    kuid_t fastuid;
    struct in6_addr fast_v6_rcv_saddr;
    __be32 fast_rcv_saddr;
    short unsigned int fast_sk_family;
    bool fast_ipv6_only;
    struct hlist_node node;
    struct hlist_head owners;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct inet_bind_bucket {
    possible_net_t ib_net;
    int l3mdev;
    short unsigned int port;
    signed char fastreuse;
    signed char fastreuseport;
    kuid_t fastuid;
    struct in6_addr fast_v6_rcv_saddr;
    __be32 fast_rcv_saddr;
    short unsigned int fast_sk_family;
    bool fast_ipv6_only;
    struct hlist_node node;
    struct hlist_head owners;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct inet_bind_bucket {
    possible_net_t ib_net;
    int l3mdev;
    short unsigned int port;
    signed char fastreuse;
    signed char fastreuseport;
    kuid_t fastuid;
    struct in6_addr fast_v6_rcv_saddr;
    __be32 fast_rcv_saddr;
    short unsigned int fast_sk_family;
    bool fast_ipv6_only;
    struct hlist_node node;
    struct hlist_head owners;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct inet_bind_bucket {
    possible_net_t ib_net;
    int l3mdev;
    short unsigned int port;
    signed char fastreuse;
    signed char fastreuseport;
    kuid_t fastuid;
    struct in6_addr fast_v6_rcv_saddr;
    __be32 fast_rcv_saddr;
    short unsigned int fast_sk_family;
    bool fast_ipv6_only;
    struct hlist_node node;
    struct hlist_head owners;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct inet_bind_bucket {
    possible_net_t ib_net;
    int l3mdev;
    short unsigned int port;
    signed char fastreuse;
    signed char fastreuseport;
    kuid_t fastuid;
    struct in6_addr fast_v6_rcv_saddr;
    __be32 fast_rcv_saddr;
    short unsigned int fast_sk_family;
    bool fast_ipv6_only;
    struct hlist_node node;
    struct hlist_head owners;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct inet_bind_bucket {
    possible_net_t ib_net;
    int l3mdev;
    short unsigned int port;
    signed char fastreuse;
    signed char fastreuseport;
    kuid_t fastuid;
    struct in6_addr fast_v6_rcv_saddr;
    __be32 fast_rcv_saddr;
    short unsigned int fast_sk_family;
    bool fast_ipv6_only;
    struct hlist_node node;
    struct hlist_head owners;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct inet_bind_bucket {
    possible_net_t ib_net;
    int l3mdev;
    short unsigned int port;
    signed char fastreuse;
    signed char fastreuseport;
    kuid_t fastuid;
    struct in6_addr fast_v6_rcv_saddr;
    __be32 fast_rcv_saddr;
    short unsigned int fast_sk_family;
    bool fast_ipv6_only;
    struct hlist_node node;
    struct hlist_head owners;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct inet_bind_bucket {
    possible_net_t ib_net;
    int l3mdev;
    short unsigned int port;
    signed char fastreuse;
    signed char fastreuseport;
    kuid_t fastuid;
    struct in6_addr fast_v6_rcv_saddr;
    __be32 fast_rcv_saddr;
    short unsigned int fast_sk_family;
    bool fast_ipv6_only;
    struct hlist_node node;
    struct hlist_head owners;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct inet_bind_bucket {
    possible_net_t ib_net;
    int l3mdev;
    short unsigned int port;
    signed char fastreuse;
    signed char fastreuseport;
    kuid_t fastuid;
    struct in6_addr fast_v6_rcv_saddr;
    __be32 fast_rcv_saddr;
    short unsigned int fast_sk_family;
    bool fast_ipv6_only;
    struct hlist_node node;
    struct hlist_head bhash2;
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
struct inet_bind_bucket {
    possible_net_t ib_net;
    int l3mdev;
    short unsigned int port;
    signed char fastreuse;
    signed char fastreuseport;
    kuid_t fastuid;
    struct in6_addr fast_v6_rcv_saddr;
    __be32 fast_rcv_saddr;
    short unsigned int fast_sk_family;
    bool fast_ipv6_only;
    struct hlist_node node;
    struct hlist_head owners;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct inet_bind_bucket {
    possible_net_t ib_net;
    int l3mdev;
    short unsigned int port;
    signed char fastreuse;
    signed char fastreuseport;
    kuid_t fastuid;
    struct in6_addr fast_v6_rcv_saddr;
    __be32 fast_rcv_saddr;
    short unsigned int fast_sk_family;
    bool fast_ipv6_only;
    struct hlist_node node;
    struct hlist_head owners;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct inet_bind_bucket {
    possible_net_t ib_net;
    int l3mdev;
    short unsigned int port;
    signed char fastreuse;
    signed char fastreuseport;
    kuid_t fastuid;
    struct in6_addr fast_v6_rcv_saddr;
    __be32 fast_rcv_saddr;
    short unsigned int fast_sk_family;
    bool fast_ipv6_only;
    struct hlist_node node;
    struct hlist_head owners;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct inet_bind_bucket {
    possible_net_t ib_net;
    int l3mdev;
    short unsigned int port;
    signed char fastreuse;
    signed char fastreuseport;
    kuid_t fastuid;
    struct in6_addr fast_v6_rcv_saddr;
    __be32 fast_rcv_saddr;
    short unsigned int fast_sk_family;
    bool fast_ipv6_only;
    struct hlist_node node;
    struct hlist_head owners;
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
struct inet_bind_bucket {
    possible_net_t ib_net;
    int l3mdev;
    short unsigned int port;
    signed char fastreuse;
    signed char fastreuseport;
    kuid_t fastuid;
    struct in6_addr fast_v6_rcv_saddr;
    __be32 fast_rcv_saddr;
    short unsigned int fast_sk_family;
    bool fast_ipv6_only;
    struct hlist_node node;
    struct hlist_head owners;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct inet_bind_bucket {
    possible_net_t ib_net;
    int l3mdev;
    short unsigned int port;
    signed char fastreuse;
    signed char fastreuseport;
    kuid_t fastuid;
    struct in6_addr fast_v6_rcv_saddr;
    __be32 fast_rcv_saddr;
    short unsigned int fast_sk_family;
    bool fast_ipv6_only;
    struct hlist_node node;
    struct hlist_head owners;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct inet_bind_bucket {
    possible_net_t ib_net;
    int l3mdev;
    short unsigned int port;
    signed char fastreuse;
    signed char fastreuseport;
    kuid_t fastuid;
    struct in6_addr fast_v6_rcv_saddr;
    __be32 fast_rcv_saddr;
    short unsigned int fast_sk_family;
    bool fast_ipv6_only;
    struct hlist_node node;
    struct hlist_head owners;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct inet_bind_bucket {
    possible_net_t ib_net;
    int l3mdev;
    short unsigned int port;
    signed char fastreuse;
    signed char fastreuseport;
    kuid_t fastuid;
    struct in6_addr fast_v6_rcv_saddr;
    __be32 fast_rcv_saddr;
    short unsigned int fast_sk_family;
    bool fast_ipv6_only;
    struct hlist_node node;
    struct hlist_head owners;
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
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct in6_addr fast_v6_rcv_saddr</code>
</li>
<li>
<b>Field added. </b>
<code>__be32 fast_rcv_saddr</code>
</li>
<li>
<b>Field added. </b>
<code>short unsigned int fast_sk_family</code>
</li>
<li>
<b>Field added. </b>
<code>bool fast_ipv6_only</code>
</li>
<li>
<b>Field removed. </b>
<code>int num_owners</code>
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
<code>int l3mdev</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct hlist_head bhash2</code>
</li>
<li>
<b>Field removed. </b>
<code>struct hlist_head owners</code>
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
