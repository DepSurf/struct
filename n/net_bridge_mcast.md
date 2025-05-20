# Struct: <code>net_bridge_mcast</code>

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
struct net_bridge_mcast {
    struct net_bridge *br;
    struct net_bridge_vlan *vlan;
    u32 multicast_last_member_count;
    u32 multicast_startup_query_count;
    u8 multicast_querier;
    u8 multicast_igmp_version;
    u8 multicast_router;
    u8 multicast_mld_version;
    long unsigned int multicast_last_member_interval;
    long unsigned int multicast_membership_interval;
    long unsigned int multicast_querier_interval;
    long unsigned int multicast_query_interval;
    long unsigned int multicast_query_response_interval;
    long unsigned int multicast_startup_query_interval;
    struct hlist_head ip4_mc_router_list;
    struct timer_list ip4_mc_router_timer;
    struct bridge_mcast_other_query ip4_other_query;
    struct bridge_mcast_own_query ip4_own_query;
    struct bridge_mcast_querier ip4_querier;
    struct hlist_head ip6_mc_router_list;
    struct timer_list ip6_mc_router_timer;
    struct bridge_mcast_other_query ip6_other_query;
    struct bridge_mcast_own_query ip6_own_query;
    struct bridge_mcast_querier ip6_querier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct net_bridge_mcast {
    struct net_bridge *br;
    struct net_bridge_vlan *vlan;
    u32 multicast_last_member_count;
    u32 multicast_startup_query_count;
    u8 multicast_querier;
    u8 multicast_igmp_version;
    u8 multicast_router;
    u8 multicast_mld_version;
    long unsigned int multicast_last_member_interval;
    long unsigned int multicast_membership_interval;
    long unsigned int multicast_querier_interval;
    long unsigned int multicast_query_interval;
    long unsigned int multicast_query_response_interval;
    long unsigned int multicast_startup_query_interval;
    struct hlist_head ip4_mc_router_list;
    struct timer_list ip4_mc_router_timer;
    struct bridge_mcast_other_query ip4_other_query;
    struct bridge_mcast_own_query ip4_own_query;
    struct bridge_mcast_querier ip4_querier;
    struct hlist_head ip6_mc_router_list;
    struct timer_list ip6_mc_router_timer;
    struct bridge_mcast_other_query ip6_other_query;
    struct bridge_mcast_own_query ip6_own_query;
    struct bridge_mcast_querier ip6_querier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct net_bridge_mcast {
    struct net_bridge *br;
    struct net_bridge_vlan *vlan;
    u32 multicast_last_member_count;
    u32 multicast_startup_query_count;
    u8 multicast_querier;
    u8 multicast_igmp_version;
    u8 multicast_router;
    u8 multicast_mld_version;
    long unsigned int multicast_last_member_interval;
    long unsigned int multicast_membership_interval;
    long unsigned int multicast_querier_interval;
    long unsigned int multicast_query_interval;
    long unsigned int multicast_query_response_interval;
    long unsigned int multicast_startup_query_interval;
    struct hlist_head ip4_mc_router_list;
    struct timer_list ip4_mc_router_timer;
    struct bridge_mcast_other_query ip4_other_query;
    struct bridge_mcast_own_query ip4_own_query;
    struct bridge_mcast_querier ip4_querier;
    struct hlist_head ip6_mc_router_list;
    struct timer_list ip6_mc_router_timer;
    struct bridge_mcast_other_query ip6_other_query;
    struct bridge_mcast_own_query ip6_own_query;
    struct bridge_mcast_querier ip6_querier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct net_bridge_mcast {
    struct net_bridge *br;
    struct net_bridge_vlan *vlan;
    u32 multicast_last_member_count;
    u32 multicast_startup_query_count;
    u8 multicast_querier;
    u8 multicast_igmp_version;
    u8 multicast_router;
    u8 multicast_mld_version;
    long unsigned int multicast_last_member_interval;
    long unsigned int multicast_membership_interval;
    long unsigned int multicast_querier_interval;
    long unsigned int multicast_query_interval;
    long unsigned int multicast_query_response_interval;
    long unsigned int multicast_startup_query_interval;
    struct hlist_head ip4_mc_router_list;
    struct timer_list ip4_mc_router_timer;
    struct bridge_mcast_other_query ip4_other_query;
    struct bridge_mcast_own_query ip4_own_query;
    struct bridge_mcast_querier ip4_querier;
    struct hlist_head ip6_mc_router_list;
    struct timer_list ip6_mc_router_timer;
    struct bridge_mcast_other_query ip6_other_query;
    struct bridge_mcast_own_query ip6_own_query;
    struct bridge_mcast_querier ip6_querier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct net_bridge_mcast {
    struct net_bridge *br;
    struct net_bridge_vlan *vlan;
    u32 multicast_last_member_count;
    u32 multicast_startup_query_count;
    u8 multicast_querier;
    u8 multicast_igmp_version;
    u8 multicast_router;
    u8 multicast_mld_version;
    long unsigned int multicast_last_member_interval;
    long unsigned int multicast_membership_interval;
    long unsigned int multicast_querier_interval;
    long unsigned int multicast_query_interval;
    long unsigned int multicast_query_response_interval;
    long unsigned int multicast_startup_query_interval;
    struct hlist_head ip4_mc_router_list;
    struct timer_list ip4_mc_router_timer;
    struct bridge_mcast_other_query ip4_other_query;
    struct bridge_mcast_own_query ip4_own_query;
    struct bridge_mcast_querier ip4_querier;
    struct hlist_head ip6_mc_router_list;
    struct timer_list ip6_mc_router_timer;
    struct bridge_mcast_other_query ip6_other_query;
    struct bridge_mcast_own_query ip6_own_query;
    struct bridge_mcast_querier ip6_querier;
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
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
