# Struct: <code>nf_ipv6_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct nf_ipv6_ops {
    int (*chk_addr)(struct net *, const struct in6_addr *, const struct net_device *, int);
    void (*route_input)(struct sk_buff *);
    int (*fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct nf_ipv6_ops {
    int (*chk_addr)(struct net *, const struct in6_addr *, const struct net_device *, int);
    void (*route_input)(struct sk_buff *);
    int (*fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct nf_ipv6_ops {
    int (*chk_addr)(struct net *, const struct in6_addr *, const struct net_device *, int);
    void (*route_input)(struct sk_buff *);
    int (*fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct nf_ipv6_ops {
    int (*chk_addr)(struct net *, const struct in6_addr *, const struct net_device *, int);
    void (*route_input)(struct sk_buff *);
    int (*fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct nf_ipv6_ops {
    int (*chk_addr)(struct net *, const struct in6_addr *, const struct net_device *, int);
    void (*route_input)(struct sk_buff *);
    int (*fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct nf_ipv6_ops {
    int (*chk_addr)(struct net *, const struct in6_addr *, const struct net_device *, int);
    void (*route_input)(struct sk_buff *);
    int (*fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
    __sum16 (*checksum)(struct sk_buff *, unsigned int, unsigned int, u_int8_t);
    __sum16 (*checksum_partial)(struct sk_buff *, unsigned int, unsigned int, unsigned int, u_int8_t);
    int (*route)(struct net *, struct dst_entry **, struct flowi *, bool);
    int (*reroute)(struct sk_buff *, const struct nf_queue_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct nf_ipv6_ops {
    int (*chk_addr)(struct net *, const struct in6_addr *, const struct net_device *, int);
    void (*route_input)(struct sk_buff *);
    int (*fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
    int (*route)(struct net *, struct dst_entry **, struct flowi *, bool);
    int (*reroute)(struct sk_buff *, const struct nf_queue_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct nf_ipv6_ops {
    void (*route_input)(struct sk_buff *);
    int (*fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
    int (*reroute)(struct sk_buff *, const struct nf_queue_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct nf_ipv6_ops {
    void (*route_input)(struct sk_buff *);
    int (*fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
    int (*reroute)(struct sk_buff *, const struct nf_queue_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct nf_ipv6_ops {
    void (*route_input)(struct sk_buff *);
    int (*fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
    int (*reroute)(struct sk_buff *, const struct nf_queue_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct nf_ipv6_ops {
    void (*route_input)(struct sk_buff *);
    int (*fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
    int (*reroute)(struct sk_buff *, const struct nf_queue_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct nf_ipv6_ops {
    void (*route_input)(struct sk_buff *);
    int (*fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
    int (*reroute)(struct sk_buff *, const struct nf_queue_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct nf_ipv6_ops {
    void (*route_input)(struct sk_buff *);
    int (*fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
    int (*reroute)(struct sk_buff *, const struct nf_queue_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct nf_ipv6_ops {
    void (*route_input)(struct sk_buff *);
    int (*fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
    int (*reroute)(struct sk_buff *, const struct nf_queue_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct nf_ipv6_ops {
    void (*route_input)(struct sk_buff *);
    int (*fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
    int (*reroute)(struct sk_buff *, const struct nf_queue_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct nf_ipv6_ops {
    void (*route_input)(struct sk_buff *);
    int (*fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
    int (*reroute)(struct sk_buff *, const struct nf_queue_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct nf_ipv6_ops {
    void (*route_input)(struct sk_buff *);
    int (*fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
    int (*reroute)(struct sk_buff *, const struct nf_queue_entry *);
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
struct nf_ipv6_ops {
    void (*route_input)(struct sk_buff *);
    int (*fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
    int (*reroute)(struct sk_buff *, const struct nf_queue_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct nf_ipv6_ops {
    void (*route_input)(struct sk_buff *);
    int (*fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
    int (*reroute)(struct sk_buff *, const struct nf_queue_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct nf_ipv6_ops {
    void (*route_input)(struct sk_buff *);
    int (*fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
    int (*reroute)(struct sk_buff *, const struct nf_queue_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct nf_ipv6_ops {
    void (*route_input)(struct sk_buff *);
    int (*fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
    int (*reroute)(struct sk_buff *, const struct nf_queue_entry *);
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
struct nf_ipv6_ops {
    void (*route_input)(struct sk_buff *);
    int (*fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
    int (*reroute)(struct sk_buff *, const struct nf_queue_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct nf_ipv6_ops {
    void (*route_input)(struct sk_buff *);
    int (*fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
    int (*reroute)(struct sk_buff *, const struct nf_queue_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct nf_ipv6_ops {
    void (*route_input)(struct sk_buff *);
    int (*fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
    int (*reroute)(struct sk_buff *, const struct nf_queue_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct nf_ipv6_ops {
    void (*route_input)(struct sk_buff *);
    int (*fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
    int (*reroute)(struct sk_buff *, const struct nf_queue_entry *);
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
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__sum16 (*checksum)(struct sk_buff *, unsigned int, unsigned int, u_int8_t)</code>
</li>
<li>
<b>Field added. </b>
<code>__sum16 (*checksum_partial)(struct sk_buff *, unsigned int, unsigned int, unsigned int, u_int8_t)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*route)(struct net *, struct dst_entry **, struct flowi *, bool)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*reroute)(struct sk_buff *, const struct nf_queue_entry *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>__sum16 (*checksum)(struct sk_buff *, unsigned int, unsigned int, u_int8_t)</code>
</li>
<li>
<b>Field removed. </b>
<code>__sum16 (*checksum_partial)(struct sk_buff *, unsigned int, unsigned int, unsigned int, u_int8_t)</code>
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
<code>int (*chk_addr)(struct net *, const struct in6_addr *, const struct net_device *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*route)(struct net *, struct dst_entry **, struct flowi *, bool)</code>
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
