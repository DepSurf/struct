# Struct: <code>net_bridge_mcast_port</code>

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
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct net_bridge_mcast_port {
    struct net_bridge_port *port;
    struct net_bridge_vlan *vlan;
    struct bridge_mcast_own_query ip4_own_query;
    struct timer_list ip4_mc_router_timer;
    struct hlist_node ip4_rlist;
    struct bridge_mcast_own_query ip6_own_query;
    struct timer_list ip6_mc_router_timer;
    struct hlist_node ip6_rlist;
    unsigned char multicast_router;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct net_bridge_mcast_port {
    struct net_bridge_port *port;
    struct net_bridge_vlan *vlan;
    struct bridge_mcast_own_query ip4_own_query;
    struct timer_list ip4_mc_router_timer;
    struct hlist_node ip4_rlist;
    struct bridge_mcast_own_query ip6_own_query;
    struct timer_list ip6_mc_router_timer;
    struct hlist_node ip6_rlist;
    unsigned char multicast_router;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct net_bridge_mcast_port {
    struct net_bridge_port *port;
    struct net_bridge_vlan *vlan;
    struct bridge_mcast_own_query ip4_own_query;
    struct timer_list ip4_mc_router_timer;
    struct hlist_node ip4_rlist;
    struct bridge_mcast_own_query ip6_own_query;
    struct timer_list ip6_mc_router_timer;
    struct hlist_node ip6_rlist;
    unsigned char multicast_router;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct net_bridge_mcast_port {
    struct net_bridge_port *port;
    struct net_bridge_vlan *vlan;
    struct bridge_mcast_own_query ip4_own_query;
    struct timer_list ip4_mc_router_timer;
    struct hlist_node ip4_rlist;
    struct bridge_mcast_own_query ip6_own_query;
    struct timer_list ip6_mc_router_timer;
    struct hlist_node ip6_rlist;
    unsigned char multicast_router;
    u32 mdb_n_entries;
    u32 mdb_max_entries;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct net_bridge_mcast_port {
    struct net_bridge_port *port;
    struct net_bridge_vlan *vlan;
    struct bridge_mcast_own_query ip4_own_query;
    struct timer_list ip4_mc_router_timer;
    struct hlist_node ip4_rlist;
    struct bridge_mcast_own_query ip6_own_query;
    struct timer_list ip6_mc_router_timer;
    struct hlist_node ip6_rlist;
    unsigned char multicast_router;
    u32 mdb_n_entries;
    u32 mdb_max_entries;
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
<code>u32 mdb_n_entries</code>
</li>
<li>
<b>Field added. </b>
<code>u32 mdb_max_entries</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
