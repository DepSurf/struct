# Struct: <code>net_bridge_vlan</code>

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
struct net_bridge_vlan {
    struct rhash_head vnode;
    struct rhash_head tnode;
    u16 vid;
    u16 flags;
    u16 priv_flags;
    u8 state;
    struct pcpu_sw_netstats *stats;
    struct net_bridge *br;
    struct net_bridge_port *port;
    refcount_t refcnt;
    struct net_bridge_vlan *brvlan;
    struct br_tunnel_info tinfo;
    struct net_bridge_mcast br_mcast_ctx;
    struct net_bridge_mcast_port port_mcast_ctx;
    struct list_head vlist;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct net_bridge_vlan {
    struct rhash_head vnode;
    struct rhash_head tnode;
    u16 vid;
    u16 flags;
    u16 priv_flags;
    u8 state;
    struct pcpu_sw_netstats *stats;
    struct net_bridge *br;
    struct net_bridge_port *port;
    refcount_t refcnt;
    struct net_bridge_vlan *brvlan;
    struct br_tunnel_info tinfo;
    struct net_bridge_mcast br_mcast_ctx;
    struct net_bridge_mcast_port port_mcast_ctx;
    u16 msti;
    struct list_head vlist;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct net_bridge_vlan {
    struct rhash_head vnode;
    struct rhash_head tnode;
    u16 vid;
    u16 flags;
    u16 priv_flags;
    u8 state;
    struct pcpu_sw_netstats *stats;
    struct net_bridge *br;
    struct net_bridge_port *port;
    refcount_t refcnt;
    struct net_bridge_vlan *brvlan;
    struct br_tunnel_info tinfo;
    struct net_bridge_mcast br_mcast_ctx;
    struct net_bridge_mcast_port port_mcast_ctx;
    u16 msti;
    struct list_head vlist;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct net_bridge_vlan {
    struct rhash_head vnode;
    struct rhash_head tnode;
    u16 vid;
    u16 flags;
    u16 priv_flags;
    u8 state;
    struct pcpu_sw_netstats *stats;
    struct net_bridge *br;
    struct net_bridge_port *port;
    refcount_t refcnt;
    struct net_bridge_vlan *brvlan;
    struct br_tunnel_info tinfo;
    struct net_bridge_mcast br_mcast_ctx;
    struct net_bridge_mcast_port port_mcast_ctx;
    u16 msti;
    struct list_head vlist;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct net_bridge_vlan {
    struct rhash_head vnode;
    struct rhash_head tnode;
    u16 vid;
    u16 flags;
    u16 priv_flags;
    u8 state;
    struct pcpu_sw_netstats *stats;
    struct net_bridge *br;
    struct net_bridge_port *port;
    refcount_t refcnt;
    struct net_bridge_vlan *brvlan;
    struct br_tunnel_info tinfo;
    struct net_bridge_mcast br_mcast_ctx;
    struct net_bridge_mcast_port port_mcast_ctx;
    u16 msti;
    struct list_head vlist;
    struct callback_head rcu;
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 msti</code>
</li>
</ul>
</details>
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
