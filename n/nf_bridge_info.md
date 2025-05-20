# Struct: <code>nf_bridge_info</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct nf_bridge_info {
    atomic_t use;
    enum (anon) orig_proto;
    u8 pkt_otherhost;
    u8 in_prerouting;
    u8 bridged_dnat;
    __u16 frag_max_size;
    struct net_device *physindev;
    struct net_device *physoutdev;
    __be32 ipv4_daddr;
    struct in6_addr ipv6_daddr;
    char neigh_header[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct nf_bridge_info {
    atomic_t use;
    enum (anon) orig_proto;
    u8 pkt_otherhost;
    u8 in_prerouting;
    u8 bridged_dnat;
    __u16 frag_max_size;
    struct net_device *physindev;
    struct net_device *physoutdev;
    __be32 ipv4_daddr;
    struct in6_addr ipv6_daddr;
    char neigh_header[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct nf_bridge_info {
    atomic_t use;
    enum (anon) orig_proto;
    u8 pkt_otherhost;
    u8 in_prerouting;
    u8 bridged_dnat;
    __u16 frag_max_size;
    struct net_device *physindev;
    struct net_device *physoutdev;
    __be32 ipv4_daddr;
    struct in6_addr ipv6_daddr;
    char neigh_header[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct nf_bridge_info {
    refcount_t use;
    enum (anon) orig_proto;
    u8 pkt_otherhost;
    u8 in_prerouting;
    u8 bridged_dnat;
    __u16 frag_max_size;
    struct net_device *physindev;
    struct net_device *physoutdev;
    __be32 ipv4_daddr;
    struct in6_addr ipv6_daddr;
    char neigh_header[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct nf_bridge_info {
    refcount_t use;
    enum (anon) orig_proto;
    u8 pkt_otherhost;
    u8 in_prerouting;
    u8 bridged_dnat;
    __u16 frag_max_size;
    struct net_device *physindev;
    struct net_device *physoutdev;
    __be32 ipv4_daddr;
    struct in6_addr ipv6_daddr;
    char neigh_header[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct nf_bridge_info {
    refcount_t use;
    enum (anon) orig_proto;
    u8 pkt_otherhost;
    u8 in_prerouting;
    u8 bridged_dnat;
    __u16 frag_max_size;
    struct net_device *physindev;
    struct net_device *physoutdev;
    __be32 ipv4_daddr;
    struct in6_addr ipv6_daddr;
    char neigh_header[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct nf_bridge_info {
    enum (anon) orig_proto;
    u8 pkt_otherhost;
    u8 in_prerouting;
    u8 bridged_dnat;
    __u16 frag_max_size;
    struct net_device *physindev;
    struct net_device *physoutdev;
    __be32 ipv4_daddr;
    struct in6_addr ipv6_daddr;
    char neigh_header[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct nf_bridge_info {
    enum (anon) orig_proto;
    u8 pkt_otherhost;
    u8 in_prerouting;
    u8 bridged_dnat;
    __u16 frag_max_size;
    struct net_device *physindev;
    struct net_device *physoutdev;
    __be32 ipv4_daddr;
    struct in6_addr ipv6_daddr;
    char neigh_header[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct nf_bridge_info {
    enum (anon) orig_proto;
    u8 pkt_otherhost;
    u8 in_prerouting;
    u8 bridged_dnat;
    __u16 frag_max_size;
    struct net_device *physindev;
    struct net_device *physoutdev;
    __be32 ipv4_daddr;
    struct in6_addr ipv6_daddr;
    char neigh_header[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct nf_bridge_info {
    enum (anon) orig_proto;
    u8 pkt_otherhost;
    u8 in_prerouting;
    u8 bridged_dnat;
    __u16 frag_max_size;
    struct net_device *physindev;
    struct net_device *physoutdev;
    __be32 ipv4_daddr;
    struct in6_addr ipv6_daddr;
    char neigh_header[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct nf_bridge_info {
    enum (anon) orig_proto;
    u8 pkt_otherhost;
    u8 in_prerouting;
    u8 bridged_dnat;
    __u16 frag_max_size;
    struct net_device *physindev;
    struct net_device *physoutdev;
    __be32 ipv4_daddr;
    struct in6_addr ipv6_daddr;
    char neigh_header[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct nf_bridge_info {
    enum (anon) orig_proto;
    u8 pkt_otherhost;
    u8 in_prerouting;
    u8 bridged_dnat;
    __u16 frag_max_size;
    struct net_device *physindev;
    struct net_device *physoutdev;
    __be32 ipv4_daddr;
    struct in6_addr ipv6_daddr;
    char neigh_header[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct nf_bridge_info {
    enum (anon) orig_proto;
    u8 pkt_otherhost;
    u8 in_prerouting;
    u8 bridged_dnat;
    __u16 frag_max_size;
    struct net_device *physindev;
    struct net_device *physoutdev;
    __be32 ipv4_daddr;
    struct in6_addr ipv6_daddr;
    char neigh_header[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct nf_bridge_info {
    enum (anon) orig_proto;
    u8 pkt_otherhost;
    u8 in_prerouting;
    u8 bridged_dnat;
    __u16 frag_max_size;
    struct net_device *physindev;
    struct net_device *physoutdev;
    __be32 ipv4_daddr;
    struct in6_addr ipv6_daddr;
    char neigh_header[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct nf_bridge_info {
    enum (anon) orig_proto;
    u8 pkt_otherhost;
    u8 in_prerouting;
    u8 bridged_dnat;
    __u16 frag_max_size;
    struct net_device *physindev;
    struct net_device *physoutdev;
    __be32 ipv4_daddr;
    struct in6_addr ipv6_daddr;
    char neigh_header[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct nf_bridge_info {
    enum (anon) orig_proto;
    u8 pkt_otherhost;
    u8 in_prerouting;
    u8 bridged_dnat;
    u8 sabotage_in_done;
    __u16 frag_max_size;
    struct net_device *physindev;
    struct net_device *physoutdev;
    __be32 ipv4_daddr;
    struct in6_addr ipv6_daddr;
    char neigh_header[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct nf_bridge_info {
    enum (anon) orig_proto;
    u8 pkt_otherhost;
    u8 in_prerouting;
    u8 bridged_dnat;
    u8 sabotage_in_done;
    __u16 frag_max_size;
    int physinif;
    struct net_device *physoutdev;
    __be32 ipv4_daddr;
    struct in6_addr ipv6_daddr;
    char neigh_header[8];
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
struct nf_bridge_info {
    enum (anon) orig_proto;
    u8 pkt_otherhost;
    u8 in_prerouting;
    u8 bridged_dnat;
    __u16 frag_max_size;
    struct net_device *physindev;
    struct net_device *physoutdev;
    __be32 ipv4_daddr;
    struct in6_addr ipv6_daddr;
    char neigh_header[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct nf_bridge_info {
    enum (anon) orig_proto;
    u8 pkt_otherhost;
    u8 in_prerouting;
    u8 bridged_dnat;
    __u16 frag_max_size;
    struct net_device *physindev;
    struct net_device *physoutdev;
    __be32 ipv4_daddr;
    struct in6_addr ipv6_daddr;
    char neigh_header[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct nf_bridge_info {
    enum (anon) orig_proto;
    u8 pkt_otherhost;
    u8 in_prerouting;
    u8 bridged_dnat;
    __u16 frag_max_size;
    struct net_device *physindev;
    struct net_device *physoutdev;
    __be32 ipv4_daddr;
    struct in6_addr ipv6_daddr;
    char neigh_header[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct nf_bridge_info {
    enum (anon) orig_proto;
    u8 pkt_otherhost;
    u8 in_prerouting;
    u8 bridged_dnat;
    __u16 frag_max_size;
    struct net_device *physindev;
    struct net_device *physoutdev;
    __be32 ipv4_daddr;
    struct in6_addr ipv6_daddr;
    char neigh_header[8];
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
struct nf_bridge_info {
    enum (anon) orig_proto;
    u8 pkt_otherhost;
    u8 in_prerouting;
    u8 bridged_dnat;
    __u16 frag_max_size;
    struct net_device *physindev;
    struct net_device *physoutdev;
    __be32 ipv4_daddr;
    struct in6_addr ipv6_daddr;
    char neigh_header[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct nf_bridge_info {
    enum (anon) orig_proto;
    u8 pkt_otherhost;
    u8 in_prerouting;
    u8 bridged_dnat;
    __u16 frag_max_size;
    struct net_device *physindev;
    struct net_device *physoutdev;
    __be32 ipv4_daddr;
    struct in6_addr ipv6_daddr;
    char neigh_header[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct nf_bridge_info {
    enum (anon) orig_proto;
    u8 pkt_otherhost;
    u8 in_prerouting;
    u8 bridged_dnat;
    __u16 frag_max_size;
    struct net_device *physindev;
    struct net_device *physoutdev;
    __be32 ipv4_daddr;
    struct in6_addr ipv6_daddr;
    char neigh_header[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct nf_bridge_info {
    enum (anon) orig_proto;
    u8 pkt_otherhost;
    u8 in_prerouting;
    u8 bridged_dnat;
    __u16 frag_max_size;
    struct net_device *physindev;
    struct net_device *physoutdev;
    __be32 ipv4_daddr;
    struct in6_addr ipv6_daddr;
    char neigh_header[8];
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
<b>Field type changed. </b>
<code>atomic_t use</code> ➡️ <code>refcount_t use</code>
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
<b>Field removed. </b>
<code>refcount_t use</code>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 sabotage_in_done</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int physinif</code>
</li>
<li>
<b>Field removed. </b>
<code>struct net_device *physindev</code>
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
