# Struct: <code>bpf_fib_lookup</code>

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
struct bpf_fib_lookup {
    __u8 family;
    __u8 l4_protocol;
    __be16 sport;
    __be16 dport;
    __u16 tot_len;
    __u32 ifindex;
    __u8 tos;
    __be32 flowinfo;
    __u32 rt_metric;
    __be32 ipv4_src;
    __u32 ipv6_src[4];
    __be32 ipv4_dst;
    __u32 ipv6_dst[4];
    __be16 h_vlan_proto;
    __be16 h_vlan_TCI;
    __u8 smac[6];
    __u8 dmac[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct bpf_fib_lookup {
    __u8 family;
    __u8 l4_protocol;
    __be16 sport;
    __be16 dport;
    __u16 tot_len;
    __u32 ifindex;
    __u8 tos;
    __be32 flowinfo;
    __u32 rt_metric;
    __be32 ipv4_src;
    __u32 ipv6_src[4];
    __be32 ipv4_dst;
    __u32 ipv6_dst[4];
    __be16 h_vlan_proto;
    __be16 h_vlan_TCI;
    __u8 smac[6];
    __u8 dmac[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct bpf_fib_lookup {
    __u8 family;
    __u8 l4_protocol;
    __be16 sport;
    __be16 dport;
    __u16 tot_len;
    __u32 ifindex;
    __u8 tos;
    __be32 flowinfo;
    __u32 rt_metric;
    __be32 ipv4_src;
    __u32 ipv6_src[4];
    __be32 ipv4_dst;
    __u32 ipv6_dst[4];
    __be16 h_vlan_proto;
    __be16 h_vlan_TCI;
    __u8 smac[6];
    __u8 dmac[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct bpf_fib_lookup {
    __u8 family;
    __u8 l4_protocol;
    __be16 sport;
    __be16 dport;
    __u16 tot_len;
    __u32 ifindex;
    __u8 tos;
    __be32 flowinfo;
    __u32 rt_metric;
    __be32 ipv4_src;
    __u32 ipv6_src[4];
    __be32 ipv4_dst;
    __u32 ipv6_dst[4];
    __be16 h_vlan_proto;
    __be16 h_vlan_TCI;
    __u8 smac[6];
    __u8 dmac[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct bpf_fib_lookup {
    __u8 family;
    __u8 l4_protocol;
    __be16 sport;
    __be16 dport;
    __u16 tot_len;
    __u32 ifindex;
    __u8 tos;
    __be32 flowinfo;
    __u32 rt_metric;
    __be32 ipv4_src;
    __u32 ipv6_src[4];
    __be32 ipv4_dst;
    __u32 ipv6_dst[4];
    __be16 h_vlan_proto;
    __be16 h_vlan_TCI;
    __u8 smac[6];
    __u8 dmac[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct bpf_fib_lookup {
    __u8 family;
    __u8 l4_protocol;
    __be16 sport;
    __be16 dport;
    __u16 tot_len;
    __u32 ifindex;
    __u8 tos;
    __be32 flowinfo;
    __u32 rt_metric;
    __be32 ipv4_src;
    __u32 ipv6_src[4];
    __be32 ipv4_dst;
    __u32 ipv6_dst[4];
    __be16 h_vlan_proto;
    __be16 h_vlan_TCI;
    __u8 smac[6];
    __u8 dmac[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct bpf_fib_lookup {
    __u8 family;
    __u8 l4_protocol;
    __be16 sport;
    __be16 dport;
    __u16 tot_len;
    __u16 mtu_result;
    __u32 ifindex;
    __u8 tos;
    __be32 flowinfo;
    __u32 rt_metric;
    __be32 ipv4_src;
    __u32 ipv6_src[4];
    __be32 ipv4_dst;
    __u32 ipv6_dst[4];
    __be16 h_vlan_proto;
    __be16 h_vlan_TCI;
    __u8 smac[6];
    __u8 dmac[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct bpf_fib_lookup {
    __u8 family;
    __u8 l4_protocol;
    __be16 sport;
    __be16 dport;
    __u16 tot_len;
    __u16 mtu_result;
    __u32 ifindex;
    __u8 tos;
    __be32 flowinfo;
    __u32 rt_metric;
    __be32 ipv4_src;
    __u32 ipv6_src[4];
    __be32 ipv4_dst;
    __u32 ipv6_dst[4];
    __be16 h_vlan_proto;
    __be16 h_vlan_TCI;
    __u8 smac[6];
    __u8 dmac[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct bpf_fib_lookup {
    __u8 family;
    __u8 l4_protocol;
    __be16 sport;
    __be16 dport;
    __u16 tot_len;
    __u16 mtu_result;
    __u32 ifindex;
    __u8 tos;
    __be32 flowinfo;
    __u32 rt_metric;
    __be32 ipv4_src;
    __u32 ipv6_src[4];
    __be32 ipv4_dst;
    __u32 ipv6_dst[4];
    __be16 h_vlan_proto;
    __be16 h_vlan_TCI;
    __u8 smac[6];
    __u8 dmac[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct bpf_fib_lookup {
    __u8 family;
    __u8 l4_protocol;
    __be16 sport;
    __be16 dport;
    __u16 tot_len;
    __u16 mtu_result;
    __u32 ifindex;
    __u8 tos;
    __be32 flowinfo;
    __u32 rt_metric;
    __be32 ipv4_src;
    __u32 ipv6_src[4];
    __be32 ipv4_dst;
    __u32 ipv6_dst[4];
    __be16 h_vlan_proto;
    __be16 h_vlan_TCI;
    __u8 smac[6];
    __u8 dmac[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct bpf_fib_lookup {
    __u8 family;
    __u8 l4_protocol;
    __be16 sport;
    __be16 dport;
    __u16 tot_len;
    __u16 mtu_result;
    __u32 ifindex;
    __u8 tos;
    __be32 flowinfo;
    __u32 rt_metric;
    __be32 ipv4_src;
    __u32 ipv6_src[4];
    __be32 ipv4_dst;
    __u32 ipv6_dst[4];
    __be16 h_vlan_proto;
    __be16 h_vlan_TCI;
    __u32 tbid;
    __u8 smac[6];
    __u8 dmac[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct bpf_fib_lookup {
    __u8 family;
    __u8 l4_protocol;
    __be16 sport;
    __be16 dport;
    __u16 tot_len;
    __u16 mtu_result;
    __u32 ifindex;
    __u8 tos;
    __be32 flowinfo;
    __u32 rt_metric;
    __be32 ipv4_src;
    __u32 ipv6_src[4];
    __be32 ipv4_dst;
    __u32 ipv6_dst[4];
    __be16 h_vlan_proto;
    __be16 h_vlan_TCI;
    __u32 tbid;
    __u8 smac[6];
    __u8 dmac[6];
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
struct bpf_fib_lookup {
    __u8 family;
    __u8 l4_protocol;
    __be16 sport;
    __be16 dport;
    __u16 tot_len;
    __u32 ifindex;
    __u8 tos;
    __be32 flowinfo;
    __u32 rt_metric;
    __be32 ipv4_src;
    __u32 ipv6_src[4];
    __be32 ipv4_dst;
    __u32 ipv6_dst[4];
    __be16 h_vlan_proto;
    __be16 h_vlan_TCI;
    __u8 smac[6];
    __u8 dmac[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct bpf_fib_lookup {
    __u8 family;
    __u8 l4_protocol;
    __be16 sport;
    __be16 dport;
    __u16 tot_len;
    __u32 ifindex;
    __u8 tos;
    __be32 flowinfo;
    __u32 rt_metric;
    __be32 ipv4_src;
    __u32 ipv6_src[4];
    __be32 ipv4_dst;
    __u32 ipv6_dst[4];
    __be16 h_vlan_proto;
    __be16 h_vlan_TCI;
    __u8 smac[6];
    __u8 dmac[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct bpf_fib_lookup {
    __u8 family;
    __u8 l4_protocol;
    __be16 sport;
    __be16 dport;
    __u16 tot_len;
    __u32 ifindex;
    __u8 tos;
    __be32 flowinfo;
    __u32 rt_metric;
    __be32 ipv4_src;
    __u32 ipv6_src[4];
    __be32 ipv4_dst;
    __u32 ipv6_dst[4];
    __be16 h_vlan_proto;
    __be16 h_vlan_TCI;
    __u8 smac[6];
    __u8 dmac[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct bpf_fib_lookup {
    __u8 family;
    __u8 l4_protocol;
    __be16 sport;
    __be16 dport;
    __u16 tot_len;
    __u32 ifindex;
    __u8 tos;
    __be32 flowinfo;
    __u32 rt_metric;
    __be32 ipv4_src;
    __u32 ipv6_src[4];
    __be32 ipv4_dst;
    __u32 ipv6_dst[4];
    __be16 h_vlan_proto;
    __be16 h_vlan_TCI;
    __u8 smac[6];
    __u8 dmac[6];
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
struct bpf_fib_lookup {
    __u8 family;
    __u8 l4_protocol;
    __be16 sport;
    __be16 dport;
    __u16 tot_len;
    __u32 ifindex;
    __u8 tos;
    __be32 flowinfo;
    __u32 rt_metric;
    __be32 ipv4_src;
    __u32 ipv6_src[4];
    __be32 ipv4_dst;
    __u32 ipv6_dst[4];
    __be16 h_vlan_proto;
    __be16 h_vlan_TCI;
    __u8 smac[6];
    __u8 dmac[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct bpf_fib_lookup {
    __u8 family;
    __u8 l4_protocol;
    __be16 sport;
    __be16 dport;
    __u16 tot_len;
    __u32 ifindex;
    __u8 tos;
    __be32 flowinfo;
    __u32 rt_metric;
    __be32 ipv4_src;
    __u32 ipv6_src[4];
    __be32 ipv4_dst;
    __u32 ipv6_dst[4];
    __be16 h_vlan_proto;
    __be16 h_vlan_TCI;
    __u8 smac[6];
    __u8 dmac[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct bpf_fib_lookup {
    __u8 family;
    __u8 l4_protocol;
    __be16 sport;
    __be16 dport;
    __u16 tot_len;
    __u32 ifindex;
    __u8 tos;
    __be32 flowinfo;
    __u32 rt_metric;
    __be32 ipv4_src;
    __u32 ipv6_src[4];
    __be32 ipv4_dst;
    __u32 ipv6_dst[4];
    __be16 h_vlan_proto;
    __be16 h_vlan_TCI;
    __u8 smac[6];
    __u8 dmac[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct bpf_fib_lookup {
    __u8 family;
    __u8 l4_protocol;
    __be16 sport;
    __be16 dport;
    __u16 tot_len;
    __u32 ifindex;
    __u8 tos;
    __be32 flowinfo;
    __u32 rt_metric;
    __be32 ipv4_src;
    __u32 ipv6_src[4];
    __be32 ipv4_dst;
    __u32 ipv6_dst[4];
    __be16 h_vlan_proto;
    __be16 h_vlan_TCI;
    __u8 smac[6];
    __u8 dmac[6];
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
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u16 mtu_result</code>
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
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u32 tbid</code>
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
