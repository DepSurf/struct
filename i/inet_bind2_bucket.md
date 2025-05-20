# Struct: <code>inet_bind2_bucket</code>

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
In <code>4.18</code>: Absent ⚠️
</li>
<li>
In <code>5.0</code>: Absent ⚠️
</li>
<li>
In <code>5.3</code>: Absent ⚠️
</li>
<li>
In <code>5.4</code>: Absent ⚠️
</li>
<li>
In <code>5.8</code>: Absent ⚠️
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
In <code>5.19</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct inet_bind2_bucket {
    possible_net_t ib_net;
    int l3mdev;
    short unsigned int port;
    short unsigned int family;
    struct in6_addr v6_rcv_saddr;
    __be32 rcv_saddr;
    struct hlist_node node;
    struct hlist_head owners;
    struct hlist_head deathrow;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct inet_bind2_bucket {
    possible_net_t ib_net;
    int l3mdev;
    short unsigned int port;
    short unsigned int family;
    struct in6_addr v6_rcv_saddr;
    __be32 rcv_saddr;
    struct hlist_node node;
    struct hlist_head owners;
    struct hlist_head deathrow;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct inet_bind2_bucket {
    possible_net_t ib_net;
    int l3mdev;
    short unsigned int port;
    short unsigned int addr_type;
    struct in6_addr v6_rcv_saddr;
    struct hlist_node node;
    struct hlist_node bhash_node;
    struct hlist_head owners;
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
In <code>arm64</code>: Absent ⚠️
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
</li>
<li>
In <code>riscv64</code>: Absent ⚠️
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
In <code>aws</code>: Absent ⚠️
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>short unsigned int addr_type</code>
</li>
<li>
<b>Field added. </b>
<code>struct hlist_node bhash_node</code>
</li>
<li>
<b>Field removed. </b>
<code>short unsigned int family</code>
</li>
<li>
<b>Field removed. </b>
<code>__be32 rcv_saddr</code>
</li>
<li>
<b>Field removed. </b>
<code>struct hlist_head deathrow</code>
</li>
</ul>
</details>
</li>
</ul>
