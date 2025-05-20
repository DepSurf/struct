# Struct: <code>rtable</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct rtable {
    struct dst_entry dst;
    int rt_genid;
    unsigned int rt_flags;
    __u16 rt_type;
    __u8 rt_is_input;
    __u8 rt_uses_gateway;
    int rt_iif;
    __be32 rt_gateway;
    u32 rt_pmtu;
    u32 rt_table_id;
    struct list_head rt_uncached;
    struct uncached_list *rt_uncached_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct rtable {
    struct dst_entry dst;
    int rt_genid;
    unsigned int rt_flags;
    __u16 rt_type;
    __u8 rt_is_input;
    __u8 rt_uses_gateway;
    int rt_iif;
    __be32 rt_gateway;
    u32 rt_pmtu;
    u32 rt_table_id;
    struct list_head rt_uncached;
    struct uncached_list *rt_uncached_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rtable {
    struct dst_entry dst;
    int rt_genid;
    unsigned int rt_flags;
    __u16 rt_type;
    __u8 rt_is_input;
    __u8 rt_uses_gateway;
    int rt_iif;
    __be32 rt_gateway;
    u32 rt_pmtu;
    u32 rt_table_id;
    struct list_head rt_uncached;
    struct uncached_list *rt_uncached_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rtable {
    struct dst_entry dst;
    int rt_genid;
    unsigned int rt_flags;
    __u16 rt_type;
    __u8 rt_is_input;
    __u8 rt_uses_gateway;
    int rt_iif;
    __be32 rt_gateway;
    u32 rt_pmtu;
    u32 rt_table_id;
    struct list_head rt_uncached;
    struct uncached_list *rt_uncached_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rtable {
    struct dst_entry dst;
    int rt_genid;
    unsigned int rt_flags;
    __u16 rt_type;
    __u8 rt_is_input;
    __u8 rt_uses_gateway;
    int rt_iif;
    __be32 rt_gateway;
    u32 rt_pmtu;
    u32 rt_table_id;
    struct list_head rt_uncached;
    struct uncached_list *rt_uncached_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rtable {
    struct dst_entry dst;
    int rt_genid;
    unsigned int rt_flags;
    __u16 rt_type;
    __u8 rt_is_input;
    __u8 rt_uses_gateway;
    int rt_iif;
    __be32 rt_gateway;
    u32 rt_mtu_locked;
    u32 rt_pmtu;
    struct list_head rt_uncached;
    struct uncached_list *rt_uncached_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rtable {
    struct dst_entry dst;
    int rt_genid;
    unsigned int rt_flags;
    __u16 rt_type;
    __u8 rt_is_input;
    __u8 rt_uses_gateway;
    int rt_iif;
    __be32 rt_gateway;
    u32 rt_mtu_locked;
    u32 rt_pmtu;
    struct list_head rt_uncached;
    struct uncached_list *rt_uncached_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rtable {
    struct dst_entry dst;
    int rt_genid;
    unsigned int rt_flags;
    __u16 rt_type;
    __u8 rt_is_input;
    u8 rt_gw_family;
    int rt_iif;
    __be32 rt_gw4;
    struct in6_addr rt_gw6;
    u32 rt_mtu_locked;
    u32 rt_pmtu;
    struct list_head rt_uncached;
    struct uncached_list *rt_uncached_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rtable {
    struct dst_entry dst;
    int rt_genid;
    unsigned int rt_flags;
    __u16 rt_type;
    __u8 rt_is_input;
    __u8 rt_uses_gateway;
    int rt_iif;
    u8 rt_gw_family;
    __be32 rt_gw4;
    struct in6_addr rt_gw6;
    u32 rt_mtu_locked;
    u32 rt_pmtu;
    struct list_head rt_uncached;
    struct uncached_list *rt_uncached_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct rtable {
    struct dst_entry dst;
    int rt_genid;
    unsigned int rt_flags;
    __u16 rt_type;
    __u8 rt_is_input;
    __u8 rt_uses_gateway;
    int rt_iif;
    u8 rt_gw_family;
    __be32 rt_gw4;
    struct in6_addr rt_gw6;
    u32 rt_mtu_locked;
    u32 rt_pmtu;
    struct list_head rt_uncached;
    struct uncached_list *rt_uncached_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct rtable {
    struct dst_entry dst;
    int rt_genid;
    unsigned int rt_flags;
    __u16 rt_type;
    __u8 rt_is_input;
    __u8 rt_uses_gateway;
    int rt_iif;
    u8 rt_gw_family;
    __be32 rt_gw4;
    struct in6_addr rt_gw6;
    u32 rt_mtu_locked;
    u32 rt_pmtu;
    struct list_head rt_uncached;
    struct uncached_list *rt_uncached_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rtable {
    struct dst_entry dst;
    int rt_genid;
    unsigned int rt_flags;
    __u16 rt_type;
    __u8 rt_is_input;
    __u8 rt_uses_gateway;
    int rt_iif;
    u8 rt_gw_family;
    __be32 rt_gw4;
    struct in6_addr rt_gw6;
    u32 rt_mtu_locked;
    u32 rt_pmtu;
    struct list_head rt_uncached;
    struct uncached_list *rt_uncached_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rtable {
    struct dst_entry dst;
    int rt_genid;
    unsigned int rt_flags;
    __u16 rt_type;
    __u8 rt_is_input;
    __u8 rt_uses_gateway;
    int rt_iif;
    u8 rt_gw_family;
    __be32 rt_gw4;
    struct in6_addr rt_gw6;
    u32 rt_mtu_locked;
    u32 rt_pmtu;
    struct list_head rt_uncached;
    struct uncached_list *rt_uncached_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rtable {
    struct dst_entry dst;
    int rt_genid;
    unsigned int rt_flags;
    __u16 rt_type;
    __u8 rt_is_input;
    __u8 rt_uses_gateway;
    int rt_iif;
    u8 rt_gw_family;
    __be32 rt_gw4;
    struct in6_addr rt_gw6;
    u32 rt_mtu_locked;
    u32 rt_pmtu;
    struct list_head rt_uncached;
    struct uncached_list *rt_uncached_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rtable {
    struct dst_entry dst;
    int rt_genid;
    unsigned int rt_flags;
    __u16 rt_type;
    __u8 rt_is_input;
    __u8 rt_uses_gateway;
    int rt_iif;
    u8 rt_gw_family;
    __be32 rt_gw4;
    struct in6_addr rt_gw6;
    u32 rt_mtu_locked;
    u32 rt_pmtu;
    struct list_head rt_uncached;
    struct uncached_list *rt_uncached_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rtable {
    struct dst_entry dst;
    int rt_genid;
    unsigned int rt_flags;
    __u16 rt_type;
    __u8 rt_is_input;
    __u8 rt_uses_gateway;
    int rt_iif;
    u8 rt_gw_family;
    __be32 rt_gw4;
    struct in6_addr rt_gw6;
    u32 rt_mtu_locked;
    u32 rt_pmtu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rtable {
    struct dst_entry dst;
    int rt_genid;
    unsigned int rt_flags;
    __u16 rt_type;
    __u8 rt_is_input;
    __u8 rt_uses_gateway;
    int rt_iif;
    u8 rt_gw_family;
    __be32 rt_gw4;
    struct in6_addr rt_gw6;
    u32 rt_mtu_locked;
    u32 rt_pmtu;
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
struct rtable {
    struct dst_entry dst;
    int rt_genid;
    unsigned int rt_flags;
    __u16 rt_type;
    __u8 rt_is_input;
    __u8 rt_uses_gateway;
    int rt_iif;
    u8 rt_gw_family;
    __be32 rt_gw4;
    struct in6_addr rt_gw6;
    u32 rt_mtu_locked;
    u32 rt_pmtu;
    struct list_head rt_uncached;
    struct uncached_list *rt_uncached_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rtable {
    struct dst_entry dst;
    int rt_genid;
    unsigned int rt_flags;
    __u16 rt_type;
    __u8 rt_is_input;
    __u8 rt_uses_gateway;
    int rt_iif;
    u8 rt_gw_family;
    __be32 rt_gw4;
    struct in6_addr rt_gw6;
    u32 rt_mtu_locked;
    u32 rt_pmtu;
    struct list_head rt_uncached;
    struct uncached_list *rt_uncached_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rtable {
    struct dst_entry dst;
    int rt_genid;
    unsigned int rt_flags;
    __u16 rt_type;
    __u8 rt_is_input;
    __u8 rt_uses_gateway;
    int rt_iif;
    u8 rt_gw_family;
    __be32 rt_gw4;
    struct in6_addr rt_gw6;
    u32 rt_mtu_locked;
    u32 rt_pmtu;
    struct list_head rt_uncached;
    struct uncached_list *rt_uncached_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct rtable {
    struct dst_entry dst;
    int rt_genid;
    unsigned int rt_flags;
    __u16 rt_type;
    __u8 rt_is_input;
    __u8 rt_uses_gateway;
    int rt_iif;
    u8 rt_gw_family;
    __be32 rt_gw4;
    struct in6_addr rt_gw6;
    u32 rt_mtu_locked;
    u32 rt_pmtu;
    struct list_head rt_uncached;
    struct uncached_list *rt_uncached_list;
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
struct rtable {
    struct dst_entry dst;
    int rt_genid;
    unsigned int rt_flags;
    __u16 rt_type;
    __u8 rt_is_input;
    __u8 rt_uses_gateway;
    int rt_iif;
    u8 rt_gw_family;
    __be32 rt_gw4;
    struct in6_addr rt_gw6;
    u32 rt_mtu_locked;
    u32 rt_pmtu;
    struct list_head rt_uncached;
    struct uncached_list *rt_uncached_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rtable {
    struct dst_entry dst;
    int rt_genid;
    unsigned int rt_flags;
    __u16 rt_type;
    __u8 rt_is_input;
    __u8 rt_uses_gateway;
    int rt_iif;
    u8 rt_gw_family;
    __be32 rt_gw4;
    struct in6_addr rt_gw6;
    u32 rt_mtu_locked;
    u32 rt_pmtu;
    struct list_head rt_uncached;
    struct uncached_list *rt_uncached_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rtable {
    struct dst_entry dst;
    int rt_genid;
    unsigned int rt_flags;
    __u16 rt_type;
    __u8 rt_is_input;
    __u8 rt_uses_gateway;
    int rt_iif;
    u8 rt_gw_family;
    __be32 rt_gw4;
    struct in6_addr rt_gw6;
    u32 rt_mtu_locked;
    u32 rt_pmtu;
    struct list_head rt_uncached;
    struct uncached_list *rt_uncached_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rtable {
    struct dst_entry dst;
    int rt_genid;
    unsigned int rt_flags;
    __u16 rt_type;
    __u8 rt_is_input;
    __u8 rt_uses_gateway;
    int rt_iif;
    u8 rt_gw_family;
    __be32 rt_gw4;
    struct in6_addr rt_gw6;
    u32 rt_mtu_locked;
    u32 rt_pmtu;
    struct list_head rt_uncached;
    struct uncached_list *rt_uncached_list;
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
<code>u32 rt_mtu_locked</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 rt_table_id</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 rt_gw_family</code>
</li>
<li>
<b>Field added. </b>
<code>__be32 rt_gw4</code>
</li>
<li>
<b>Field added. </b>
<code>struct in6_addr rt_gw6</code>
</li>
<li>
<b>Field removed. </b>
<code>__u8 rt_uses_gateway</code>
</li>
<li>
<b>Field removed. </b>
<code>__be32 rt_gateway</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u8 rt_uses_gateway</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct list_head rt_uncached</code>
</li>
<li>
<b>Field removed. </b>
<code>struct uncached_list *rt_uncached_list</code>
</li>
</ul>
</details>
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
