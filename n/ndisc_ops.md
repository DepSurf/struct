# Struct: <code>ndisc_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ndisc_ops {
    int (*is_useropt)(u8);
    int (*parse_options)(const struct net_device *, struct nd_opt_hdr *, struct ndisc_options *);
    void (*update)(const struct net_device *, struct neighbour *, u32, u8, const struct ndisc_options *);
    int (*opt_addr_space)(const struct net_device *, u8, struct neighbour *, u8 *, u8 **);
    void (*fill_addr_option)(const struct net_device *, struct sk_buff *, u8, const u8 *);
    void (*prefix_rcv_add_addr)(struct net *, struct net_device *, const struct prefix_info *, struct inet6_dev *, struct in6_addr *, int, u32, bool, bool, __u32, u32, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ndisc_ops {
    int (*is_useropt)(u8);
    int (*parse_options)(const struct net_device *, struct nd_opt_hdr *, struct ndisc_options *);
    void (*update)(const struct net_device *, struct neighbour *, u32, u8, const struct ndisc_options *);
    int (*opt_addr_space)(const struct net_device *, u8, struct neighbour *, u8 *, u8 **);
    void (*fill_addr_option)(const struct net_device *, struct sk_buff *, u8, const u8 *);
    void (*prefix_rcv_add_addr)(struct net *, struct net_device *, const struct prefix_info *, struct inet6_dev *, struct in6_addr *, int, u32, bool, bool, __u32, u32, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ndisc_ops {
    int (*is_useropt)(u8);
    int (*parse_options)(const struct net_device *, struct nd_opt_hdr *, struct ndisc_options *);
    void (*update)(const struct net_device *, struct neighbour *, u32, u8, const struct ndisc_options *);
    int (*opt_addr_space)(const struct net_device *, u8, struct neighbour *, u8 *, u8 **);
    void (*fill_addr_option)(const struct net_device *, struct sk_buff *, u8, const u8 *);
    void (*prefix_rcv_add_addr)(struct net *, struct net_device *, const struct prefix_info *, struct inet6_dev *, struct in6_addr *, int, u32, bool, bool, __u32, u32, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ndisc_ops {
    int (*is_useropt)(u8);
    int (*parse_options)(const struct net_device *, struct nd_opt_hdr *, struct ndisc_options *);
    void (*update)(const struct net_device *, struct neighbour *, u32, u8, const struct ndisc_options *);
    int (*opt_addr_space)(const struct net_device *, u8, struct neighbour *, u8 *, u8 **);
    void (*fill_addr_option)(const struct net_device *, struct sk_buff *, u8, const u8 *);
    void (*prefix_rcv_add_addr)(struct net *, struct net_device *, const struct prefix_info *, struct inet6_dev *, struct in6_addr *, int, u32, bool, bool, __u32, u32, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ndisc_ops {
    int (*is_useropt)(u8);
    int (*parse_options)(const struct net_device *, struct nd_opt_hdr *, struct ndisc_options *);
    void (*update)(const struct net_device *, struct neighbour *, u32, u8, const struct ndisc_options *);
    int (*opt_addr_space)(const struct net_device *, u8, struct neighbour *, u8 *, u8 **);
    void (*fill_addr_option)(const struct net_device *, struct sk_buff *, u8, const u8 *);
    void (*prefix_rcv_add_addr)(struct net *, struct net_device *, const struct prefix_info *, struct inet6_dev *, struct in6_addr *, int, u32, bool, bool, __u32, u32, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ndisc_ops {
    int (*is_useropt)(u8);
    int (*parse_options)(const struct net_device *, struct nd_opt_hdr *, struct ndisc_options *);
    void (*update)(const struct net_device *, struct neighbour *, u32, u8, const struct ndisc_options *);
    int (*opt_addr_space)(const struct net_device *, u8, struct neighbour *, u8 *, u8 **);
    void (*fill_addr_option)(const struct net_device *, struct sk_buff *, u8, const u8 *);
    void (*prefix_rcv_add_addr)(struct net *, struct net_device *, const struct prefix_info *, struct inet6_dev *, struct in6_addr *, int, u32, bool, bool, __u32, u32, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ndisc_ops {
    int (*is_useropt)(u8);
    int (*parse_options)(const struct net_device *, struct nd_opt_hdr *, struct ndisc_options *);
    void (*update)(const struct net_device *, struct neighbour *, u32, u8, const struct ndisc_options *);
    int (*opt_addr_space)(const struct net_device *, u8, struct neighbour *, u8 *, u8 **);
    void (*fill_addr_option)(const struct net_device *, struct sk_buff *, u8, const u8 *);
    void (*prefix_rcv_add_addr)(struct net *, struct net_device *, const struct prefix_info *, struct inet6_dev *, struct in6_addr *, int, u32, bool, bool, __u32, u32, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ndisc_ops {
    int (*is_useropt)(u8);
    int (*parse_options)(const struct net_device *, struct nd_opt_hdr *, struct ndisc_options *);
    void (*update)(const struct net_device *, struct neighbour *, u32, u8, const struct ndisc_options *);
    int (*opt_addr_space)(const struct net_device *, u8, struct neighbour *, u8 *, u8 **);
    void (*fill_addr_option)(const struct net_device *, struct sk_buff *, u8, const u8 *);
    void (*prefix_rcv_add_addr)(struct net *, struct net_device *, const struct prefix_info *, struct inet6_dev *, struct in6_addr *, int, u32, bool, bool, __u32, u32, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ndisc_ops {
    int (*is_useropt)(u8);
    int (*parse_options)(const struct net_device *, struct nd_opt_hdr *, struct ndisc_options *);
    void (*update)(const struct net_device *, struct neighbour *, u32, u8, const struct ndisc_options *);
    int (*opt_addr_space)(const struct net_device *, u8, struct neighbour *, u8 *, u8 **);
    void (*fill_addr_option)(const struct net_device *, struct sk_buff *, u8, const u8 *);
    void (*prefix_rcv_add_addr)(struct net *, struct net_device *, const struct prefix_info *, struct inet6_dev *, struct in6_addr *, int, u32, bool, bool, __u32, u32, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ndisc_ops {
    int (*is_useropt)(u8);
    int (*parse_options)(const struct net_device *, struct nd_opt_hdr *, struct ndisc_options *);
    void (*update)(const struct net_device *, struct neighbour *, u32, u8, const struct ndisc_options *);
    int (*opt_addr_space)(const struct net_device *, u8, struct neighbour *, u8 *, u8 **);
    void (*fill_addr_option)(const struct net_device *, struct sk_buff *, u8, const u8 *);
    void (*prefix_rcv_add_addr)(struct net *, struct net_device *, const struct prefix_info *, struct inet6_dev *, struct in6_addr *, int, u32, bool, bool, __u32, u32, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ndisc_ops {
    int (*is_useropt)(u8);
    int (*parse_options)(const struct net_device *, struct nd_opt_hdr *, struct ndisc_options *);
    void (*update)(const struct net_device *, struct neighbour *, u32, u8, const struct ndisc_options *);
    int (*opt_addr_space)(const struct net_device *, u8, struct neighbour *, u8 *, u8 **);
    void (*fill_addr_option)(const struct net_device *, struct sk_buff *, u8, const u8 *);
    void (*prefix_rcv_add_addr)(struct net *, struct net_device *, const struct prefix_info *, struct inet6_dev *, struct in6_addr *, int, u32, bool, bool, __u32, u32, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ndisc_ops {
    int (*is_useropt)(u8);
    int (*parse_options)(const struct net_device *, struct nd_opt_hdr *, struct ndisc_options *);
    void (*update)(const struct net_device *, struct neighbour *, u32, u8, const struct ndisc_options *);
    int (*opt_addr_space)(const struct net_device *, u8, struct neighbour *, u8 *, u8 **);
    void (*fill_addr_option)(const struct net_device *, struct sk_buff *, u8, const u8 *);
    void (*prefix_rcv_add_addr)(struct net *, struct net_device *, const struct prefix_info *, struct inet6_dev *, struct in6_addr *, int, u32, bool, bool, __u32, u32, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ndisc_ops {
    int (*is_useropt)(u8);
    int (*parse_options)(const struct net_device *, struct nd_opt_hdr *, struct ndisc_options *);
    void (*update)(const struct net_device *, struct neighbour *, u32, u8, const struct ndisc_options *);
    int (*opt_addr_space)(const struct net_device *, u8, struct neighbour *, u8 *, u8 **);
    void (*fill_addr_option)(const struct net_device *, struct sk_buff *, u8, const u8 *);
    void (*prefix_rcv_add_addr)(struct net *, struct net_device *, const struct prefix_info *, struct inet6_dev *, struct in6_addr *, int, u32, bool, bool, __u32, u32, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ndisc_ops {
    int (*is_useropt)(u8);
    int (*parse_options)(const struct net_device *, struct nd_opt_hdr *, struct ndisc_options *);
    void (*update)(const struct net_device *, struct neighbour *, u32, u8, const struct ndisc_options *);
    int (*opt_addr_space)(const struct net_device *, u8, struct neighbour *, u8 *, u8 **);
    void (*fill_addr_option)(const struct net_device *, struct sk_buff *, u8, const u8 *);
    void (*prefix_rcv_add_addr)(struct net *, struct net_device *, const struct prefix_info *, struct inet6_dev *, struct in6_addr *, int, u32, bool, bool, __u32, u32, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ndisc_ops {
    int (*is_useropt)(u8);
    int (*parse_options)(const struct net_device *, struct nd_opt_hdr *, struct ndisc_options *);
    void (*update)(const struct net_device *, struct neighbour *, u32, u8, const struct ndisc_options *);
    int (*opt_addr_space)(const struct net_device *, u8, struct neighbour *, u8 *, u8 **);
    void (*fill_addr_option)(const struct net_device *, struct sk_buff *, u8, const u8 *);
    void (*prefix_rcv_add_addr)(struct net *, struct net_device *, const struct prefix_info *, struct inet6_dev *, struct in6_addr *, int, u32, bool, bool, __u32, u32, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ndisc_ops {
    int (*is_useropt)(u8);
    int (*parse_options)(const struct net_device *, struct nd_opt_hdr *, struct ndisc_options *);
    void (*update)(const struct net_device *, struct neighbour *, u32, u8, const struct ndisc_options *);
    int (*opt_addr_space)(const struct net_device *, u8, struct neighbour *, u8 *, u8 **);
    void (*fill_addr_option)(const struct net_device *, struct sk_buff *, u8, const u8 *);
    void (*prefix_rcv_add_addr)(struct net *, struct net_device *, const struct prefix_info *, struct inet6_dev *, struct in6_addr *, int, u32, bool, bool, __u32, u32, bool);
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
struct ndisc_ops {
    int (*is_useropt)(u8);
    int (*parse_options)(const struct net_device *, struct nd_opt_hdr *, struct ndisc_options *);
    void (*update)(const struct net_device *, struct neighbour *, u32, u8, const struct ndisc_options *);
    int (*opt_addr_space)(const struct net_device *, u8, struct neighbour *, u8 *, u8 **);
    void (*fill_addr_option)(const struct net_device *, struct sk_buff *, u8, const u8 *);
    void (*prefix_rcv_add_addr)(struct net *, struct net_device *, const struct prefix_info *, struct inet6_dev *, struct in6_addr *, int, u32, bool, bool, __u32, u32, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ndisc_ops {
    int (*is_useropt)(u8);
    int (*parse_options)(const struct net_device *, struct nd_opt_hdr *, struct ndisc_options *);
    void (*update)(const struct net_device *, struct neighbour *, u32, u8, const struct ndisc_options *);
    int (*opt_addr_space)(const struct net_device *, u8, struct neighbour *, u8 *, u8 **);
    void (*fill_addr_option)(const struct net_device *, struct sk_buff *, u8, const u8 *);
    void (*prefix_rcv_add_addr)(struct net *, struct net_device *, const struct prefix_info *, struct inet6_dev *, struct in6_addr *, int, u32, bool, bool, __u32, u32, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ndisc_ops {
    int (*is_useropt)(u8);
    int (*parse_options)(const struct net_device *, struct nd_opt_hdr *, struct ndisc_options *);
    void (*update)(const struct net_device *, struct neighbour *, u32, u8, const struct ndisc_options *);
    int (*opt_addr_space)(const struct net_device *, u8, struct neighbour *, u8 *, u8 **);
    void (*fill_addr_option)(const struct net_device *, struct sk_buff *, u8, const u8 *);
    void (*prefix_rcv_add_addr)(struct net *, struct net_device *, const struct prefix_info *, struct inet6_dev *, struct in6_addr *, int, u32, bool, bool, __u32, u32, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ndisc_ops {
    int (*is_useropt)(u8);
    int (*parse_options)(const struct net_device *, struct nd_opt_hdr *, struct ndisc_options *);
    void (*update)(const struct net_device *, struct neighbour *, u32, u8, const struct ndisc_options *);
    int (*opt_addr_space)(const struct net_device *, u8, struct neighbour *, u8 *, u8 **);
    void (*fill_addr_option)(const struct net_device *, struct sk_buff *, u8, const u8 *);
    void (*prefix_rcv_add_addr)(struct net *, struct net_device *, const struct prefix_info *, struct inet6_dev *, struct in6_addr *, int, u32, bool, bool, __u32, u32, bool);
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
struct ndisc_ops {
    int (*is_useropt)(u8);
    int (*parse_options)(const struct net_device *, struct nd_opt_hdr *, struct ndisc_options *);
    void (*update)(const struct net_device *, struct neighbour *, u32, u8, const struct ndisc_options *);
    int (*opt_addr_space)(const struct net_device *, u8, struct neighbour *, u8 *, u8 **);
    void (*fill_addr_option)(const struct net_device *, struct sk_buff *, u8, const u8 *);
    void (*prefix_rcv_add_addr)(struct net *, struct net_device *, const struct prefix_info *, struct inet6_dev *, struct in6_addr *, int, u32, bool, bool, __u32, u32, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ndisc_ops {
    int (*is_useropt)(u8);
    int (*parse_options)(const struct net_device *, struct nd_opt_hdr *, struct ndisc_options *);
    void (*update)(const struct net_device *, struct neighbour *, u32, u8, const struct ndisc_options *);
    int (*opt_addr_space)(const struct net_device *, u8, struct neighbour *, u8 *, u8 **);
    void (*fill_addr_option)(const struct net_device *, struct sk_buff *, u8, const u8 *);
    void (*prefix_rcv_add_addr)(struct net *, struct net_device *, const struct prefix_info *, struct inet6_dev *, struct in6_addr *, int, u32, bool, bool, __u32, u32, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ndisc_ops {
    int (*is_useropt)(u8);
    int (*parse_options)(const struct net_device *, struct nd_opt_hdr *, struct ndisc_options *);
    void (*update)(const struct net_device *, struct neighbour *, u32, u8, const struct ndisc_options *);
    int (*opt_addr_space)(const struct net_device *, u8, struct neighbour *, u8 *, u8 **);
    void (*fill_addr_option)(const struct net_device *, struct sk_buff *, u8, const u8 *);
    void (*prefix_rcv_add_addr)(struct net *, struct net_device *, const struct prefix_info *, struct inet6_dev *, struct in6_addr *, int, u32, bool, bool, __u32, u32, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ndisc_ops {
    int (*is_useropt)(u8);
    int (*parse_options)(const struct net_device *, struct nd_opt_hdr *, struct ndisc_options *);
    void (*update)(const struct net_device *, struct neighbour *, u32, u8, const struct ndisc_options *);
    int (*opt_addr_space)(const struct net_device *, u8, struct neighbour *, u8 *, u8 **);
    void (*fill_addr_option)(const struct net_device *, struct sk_buff *, u8, const u8 *);
    void (*prefix_rcv_add_addr)(struct net *, struct net_device *, const struct prefix_info *, struct inet6_dev *, struct in6_addr *, int, u32, bool, bool, __u32, u32, bool);
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
