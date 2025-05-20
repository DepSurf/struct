# Struct: <code>net_bridge_port</code>

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
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct net_bridge_port {
    struct net_bridge *br;
    struct net_device *dev;
    struct list_head list;
    long unsigned int flags;
    struct net_bridge_vlan_group *vlgrp;
    u8 priority;
    u8 state;
    u16 port_no;
    unsigned char topology_change_ack;
    unsigned char config_pending;
    port_id port_id;
    port_id designated_port;
    bridge_id designated_root;
    bridge_id designated_bridge;
    u32 path_cost;
    u32 designated_cost;
    long unsigned int designated_age;
    struct timer_list forward_delay_timer;
    struct timer_list hold_timer;
    struct timer_list message_age_timer;
    struct kobject kobj;
    struct callback_head rcu;
    struct bridge_mcast_own_query ip4_own_query;
    struct bridge_mcast_own_query ip6_own_query;
    unsigned char multicast_router;
    struct bridge_mcast_stats *mcast_stats;
    struct timer_list multicast_router_timer;
    struct hlist_head mglist;
    struct hlist_node rlist;
    char sysfs_name[16];
    struct netpoll *np;
    int offload_fwd_mark;
    u16 group_fwd_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct net_bridge_port {
    struct net_bridge *br;
    struct net_device *dev;
    struct list_head list;
    long unsigned int flags;
    struct net_bridge_vlan_group *vlgrp;
    u8 priority;
    u8 state;
    u16 port_no;
    unsigned char topology_change_ack;
    unsigned char config_pending;
    port_id port_id;
    port_id designated_port;
    bridge_id designated_root;
    bridge_id designated_bridge;
    u32 path_cost;
    u32 designated_cost;
    long unsigned int designated_age;
    struct timer_list forward_delay_timer;
    struct timer_list hold_timer;
    struct timer_list message_age_timer;
    struct kobject kobj;
    struct callback_head rcu;
    struct bridge_mcast_own_query ip4_own_query;
    struct bridge_mcast_own_query ip6_own_query;
    unsigned char multicast_router;
    struct bridge_mcast_stats *mcast_stats;
    struct timer_list multicast_router_timer;
    struct hlist_head mglist;
    struct hlist_node rlist;
    char sysfs_name[16];
    struct netpoll *np;
    int offload_fwd_mark;
    u16 group_fwd_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct net_bridge_port {
    struct net_bridge *br;
    struct net_device *dev;
    struct list_head list;
    long unsigned int flags;
    struct net_bridge_vlan_group *vlgrp;
    struct net_bridge_port *backup_port;
    u8 priority;
    u8 state;
    u16 port_no;
    unsigned char topology_change_ack;
    unsigned char config_pending;
    port_id port_id;
    port_id designated_port;
    bridge_id designated_root;
    bridge_id designated_bridge;
    u32 path_cost;
    u32 designated_cost;
    long unsigned int designated_age;
    struct timer_list forward_delay_timer;
    struct timer_list hold_timer;
    struct timer_list message_age_timer;
    struct kobject kobj;
    struct callback_head rcu;
    struct bridge_mcast_own_query ip4_own_query;
    struct bridge_mcast_own_query ip6_own_query;
    unsigned char multicast_router;
    struct bridge_mcast_stats *mcast_stats;
    struct timer_list multicast_router_timer;
    struct hlist_head mglist;
    struct hlist_node rlist;
    char sysfs_name[16];
    struct netpoll *np;
    int offload_fwd_mark;
    u16 group_fwd_mask;
    u16 backup_redirected_cnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct net_bridge_port {
    struct net_bridge *br;
    struct net_device *dev;
    struct list_head list;
    long unsigned int flags;
    struct net_bridge_vlan_group *vlgrp;
    struct net_bridge_port *backup_port;
    u8 priority;
    u8 state;
    u16 port_no;
    unsigned char topology_change_ack;
    unsigned char config_pending;
    port_id port_id;
    port_id designated_port;
    bridge_id designated_root;
    bridge_id designated_bridge;
    u32 path_cost;
    u32 designated_cost;
    long unsigned int designated_age;
    struct timer_list forward_delay_timer;
    struct timer_list hold_timer;
    struct timer_list message_age_timer;
    struct kobject kobj;
    struct callback_head rcu;
    struct bridge_mcast_own_query ip4_own_query;
    struct bridge_mcast_own_query ip6_own_query;
    unsigned char multicast_router;
    struct bridge_mcast_stats *mcast_stats;
    struct timer_list multicast_router_timer;
    struct hlist_head mglist;
    struct hlist_node rlist;
    char sysfs_name[16];
    struct netpoll *np;
    int offload_fwd_mark;
    u16 group_fwd_mask;
    u16 backup_redirected_cnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct net_bridge_port {
    struct net_bridge *br;
    struct net_device *dev;
    struct list_head list;
    long unsigned int flags;
    struct net_bridge_vlan_group *vlgrp;
    struct net_bridge_port *backup_port;
    u8 priority;
    u8 state;
    u16 port_no;
    unsigned char topology_change_ack;
    unsigned char config_pending;
    port_id port_id;
    port_id designated_port;
    bridge_id designated_root;
    bridge_id designated_bridge;
    u32 path_cost;
    u32 designated_cost;
    long unsigned int designated_age;
    struct timer_list forward_delay_timer;
    struct timer_list hold_timer;
    struct timer_list message_age_timer;
    struct kobject kobj;
    struct callback_head rcu;
    struct bridge_mcast_own_query ip4_own_query;
    struct bridge_mcast_own_query ip6_own_query;
    unsigned char multicast_router;
    struct bridge_mcast_stats *mcast_stats;
    struct timer_list multicast_router_timer;
    struct hlist_head mglist;
    struct hlist_node rlist;
    char sysfs_name[16];
    struct netpoll *np;
    int offload_fwd_mark;
    u16 group_fwd_mask;
    u16 backup_redirected_cnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct net_bridge_port {
    struct net_bridge *br;
    struct net_device *dev;
    struct list_head list;
    long unsigned int flags;
    struct net_bridge_vlan_group *vlgrp;
    struct net_bridge_port *backup_port;
    u8 priority;
    u8 state;
    u16 port_no;
    unsigned char topology_change_ack;
    unsigned char config_pending;
    port_id port_id;
    port_id designated_port;
    bridge_id designated_root;
    bridge_id designated_bridge;
    u32 path_cost;
    u32 designated_cost;
    long unsigned int designated_age;
    struct timer_list forward_delay_timer;
    struct timer_list hold_timer;
    struct timer_list message_age_timer;
    struct kobject kobj;
    struct callback_head rcu;
    struct bridge_mcast_own_query ip4_own_query;
    struct bridge_mcast_own_query ip6_own_query;
    unsigned char multicast_router;
    struct bridge_mcast_stats *mcast_stats;
    struct timer_list multicast_router_timer;
    struct hlist_head mglist;
    struct hlist_node rlist;
    char sysfs_name[16];
    struct netpoll *np;
    int offload_fwd_mark;
    u16 group_fwd_mask;
    u16 backup_redirected_cnt;
    struct bridge_stp_xstats stp_xstats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct net_bridge_port {
    struct net_bridge *br;
    struct net_device *dev;
    struct list_head list;
    long unsigned int flags;
    struct net_bridge_vlan_group *vlgrp;
    struct net_bridge_port *backup_port;
    u8 priority;
    u8 state;
    u16 port_no;
    unsigned char topology_change_ack;
    unsigned char config_pending;
    port_id port_id;
    port_id designated_port;
    bridge_id designated_root;
    bridge_id designated_bridge;
    u32 path_cost;
    u32 designated_cost;
    long unsigned int designated_age;
    struct timer_list forward_delay_timer;
    struct timer_list hold_timer;
    struct timer_list message_age_timer;
    struct kobject kobj;
    struct callback_head rcu;
    struct bridge_mcast_own_query ip4_own_query;
    struct bridge_mcast_own_query ip6_own_query;
    unsigned char multicast_router;
    struct bridge_mcast_stats *mcast_stats;
    struct timer_list multicast_router_timer;
    struct hlist_head mglist;
    struct hlist_node rlist;
    char sysfs_name[16];
    struct netpoll *np;
    int offload_fwd_mark;
    u16 group_fwd_mask;
    u16 backup_redirected_cnt;
    struct bridge_stp_xstats stp_xstats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct net_bridge_port {
    struct net_bridge *br;
    struct net_device *dev;
    struct list_head list;
    long unsigned int flags;
    struct net_bridge_vlan_group *vlgrp;
    struct net_bridge_port *backup_port;
    u8 priority;
    u8 state;
    u16 port_no;
    unsigned char topology_change_ack;
    unsigned char config_pending;
    port_id port_id;
    port_id designated_port;
    bridge_id designated_root;
    bridge_id designated_bridge;
    u32 path_cost;
    u32 designated_cost;
    long unsigned int designated_age;
    struct timer_list forward_delay_timer;
    struct timer_list hold_timer;
    struct timer_list message_age_timer;
    struct kobject kobj;
    struct callback_head rcu;
    struct bridge_mcast_own_query ip4_own_query;
    struct bridge_mcast_own_query ip6_own_query;
    u32 multicast_eht_hosts_limit;
    u32 multicast_eht_hosts_cnt;
    unsigned char multicast_router;
    struct bridge_mcast_stats *mcast_stats;
    struct timer_list multicast_router_timer;
    struct hlist_head mglist;
    struct hlist_node rlist;
    char sysfs_name[16];
    struct netpoll *np;
    int offload_fwd_mark;
    u16 group_fwd_mask;
    u16 backup_redirected_cnt;
    struct bridge_stp_xstats stp_xstats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct net_bridge_port {
    struct net_bridge *br;
    struct net_device *dev;
    struct list_head list;
    long unsigned int flags;
    struct net_bridge_vlan_group *vlgrp;
    struct net_bridge_port *backup_port;
    u8 priority;
    u8 state;
    u16 port_no;
    unsigned char topology_change_ack;
    unsigned char config_pending;
    port_id port_id;
    port_id designated_port;
    bridge_id designated_root;
    bridge_id designated_bridge;
    u32 path_cost;
    u32 designated_cost;
    long unsigned int designated_age;
    struct timer_list forward_delay_timer;
    struct timer_list hold_timer;
    struct timer_list message_age_timer;
    struct kobject kobj;
    struct callback_head rcu;
    struct net_bridge_mcast_port multicast_ctx;
    struct bridge_mcast_stats *mcast_stats;
    u32 multicast_eht_hosts_limit;
    u32 multicast_eht_hosts_cnt;
    struct hlist_head mglist;
    char sysfs_name[16];
    struct netpoll *np;
    int hwdom;
    int offload_count;
    struct netdev_phys_item_id ppid;
    u16 group_fwd_mask;
    u16 backup_redirected_cnt;
    struct bridge_stp_xstats stp_xstats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct net_bridge_port {
    struct net_bridge *br;
    struct net_device *dev;
    netdevice_tracker dev_tracker;
    struct list_head list;
    long unsigned int flags;
    struct net_bridge_vlan_group *vlgrp;
    struct net_bridge_port *backup_port;
    u8 priority;
    u8 state;
    u16 port_no;
    unsigned char topology_change_ack;
    unsigned char config_pending;
    port_id port_id;
    port_id designated_port;
    bridge_id designated_root;
    bridge_id designated_bridge;
    u32 path_cost;
    u32 designated_cost;
    long unsigned int designated_age;
    struct timer_list forward_delay_timer;
    struct timer_list hold_timer;
    struct timer_list message_age_timer;
    struct kobject kobj;
    struct callback_head rcu;
    struct net_bridge_mcast_port multicast_ctx;
    struct bridge_mcast_stats *mcast_stats;
    u32 multicast_eht_hosts_limit;
    u32 multicast_eht_hosts_cnt;
    struct hlist_head mglist;
    char sysfs_name[16];
    struct netpoll *np;
    int hwdom;
    int offload_count;
    struct netdev_phys_item_id ppid;
    u16 group_fwd_mask;
    u16 backup_redirected_cnt;
    struct bridge_stp_xstats stp_xstats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct net_bridge_port {
    struct net_bridge *br;
    struct net_device *dev;
    netdevice_tracker dev_tracker;
    struct list_head list;
    long unsigned int flags;
    struct net_bridge_vlan_group *vlgrp;
    struct net_bridge_port *backup_port;
    u8 priority;
    u8 state;
    u16 port_no;
    unsigned char topology_change_ack;
    unsigned char config_pending;
    port_id port_id;
    port_id designated_port;
    bridge_id designated_root;
    bridge_id designated_bridge;
    u32 path_cost;
    u32 designated_cost;
    long unsigned int designated_age;
    struct timer_list forward_delay_timer;
    struct timer_list hold_timer;
    struct timer_list message_age_timer;
    struct kobject kobj;
    struct callback_head rcu;
    struct net_bridge_mcast_port multicast_ctx;
    struct bridge_mcast_stats *mcast_stats;
    u32 multicast_eht_hosts_limit;
    u32 multicast_eht_hosts_cnt;
    struct hlist_head mglist;
    char sysfs_name[16];
    struct netpoll *np;
    int hwdom;
    int offload_count;
    struct netdev_phys_item_id ppid;
    u16 group_fwd_mask;
    u16 backup_redirected_cnt;
    struct bridge_stp_xstats stp_xstats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct net_bridge_port {
    struct net_bridge *br;
    struct net_device *dev;
    netdevice_tracker dev_tracker;
    struct list_head list;
    long unsigned int flags;
    struct net_bridge_vlan_group *vlgrp;
    struct net_bridge_port *backup_port;
    u8 priority;
    u8 state;
    u16 port_no;
    unsigned char topology_change_ack;
    unsigned char config_pending;
    port_id port_id;
    port_id designated_port;
    bridge_id designated_root;
    bridge_id designated_bridge;
    u32 path_cost;
    u32 designated_cost;
    long unsigned int designated_age;
    struct timer_list forward_delay_timer;
    struct timer_list hold_timer;
    struct timer_list message_age_timer;
    struct kobject kobj;
    struct callback_head rcu;
    struct net_bridge_mcast_port multicast_ctx;
    struct bridge_mcast_stats *mcast_stats;
    u32 multicast_eht_hosts_limit;
    u32 multicast_eht_hosts_cnt;
    struct hlist_head mglist;
    char sysfs_name[16];
    struct netpoll *np;
    int hwdom;
    int offload_count;
    struct netdev_phys_item_id ppid;
    u16 group_fwd_mask;
    u16 backup_redirected_cnt;
    struct bridge_stp_xstats stp_xstats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct net_bridge_port {
    struct net_bridge *br;
    struct net_device *dev;
    netdevice_tracker dev_tracker;
    struct list_head list;
    long unsigned int flags;
    struct net_bridge_vlan_group *vlgrp;
    struct net_bridge_port *backup_port;
    u32 backup_nhid;
    u8 priority;
    u8 state;
    u16 port_no;
    unsigned char topology_change_ack;
    unsigned char config_pending;
    port_id port_id;
    port_id designated_port;
    bridge_id designated_root;
    bridge_id designated_bridge;
    u32 path_cost;
    u32 designated_cost;
    long unsigned int designated_age;
    struct timer_list forward_delay_timer;
    struct timer_list hold_timer;
    struct timer_list message_age_timer;
    struct kobject kobj;
    struct callback_head rcu;
    struct net_bridge_mcast_port multicast_ctx;
    struct bridge_mcast_stats *mcast_stats;
    u32 multicast_eht_hosts_limit;
    u32 multicast_eht_hosts_cnt;
    struct hlist_head mglist;
    char sysfs_name[16];
    struct netpoll *np;
    int hwdom;
    int offload_count;
    struct netdev_phys_item_id ppid;
    u16 group_fwd_mask;
    u16 backup_redirected_cnt;
    struct bridge_stp_xstats stp_xstats;
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
struct net_bridge_port {
    struct net_bridge *br;
    struct net_device *dev;
    struct list_head list;
    long unsigned int flags;
    struct net_bridge_vlan_group *vlgrp;
    struct net_bridge_port *backup_port;
    u8 priority;
    u8 state;
    u16 port_no;
    unsigned char topology_change_ack;
    unsigned char config_pending;
    port_id port_id;
    port_id designated_port;
    bridge_id designated_root;
    bridge_id designated_bridge;
    u32 path_cost;
    u32 designated_cost;
    long unsigned int designated_age;
    struct timer_list forward_delay_timer;
    struct timer_list hold_timer;
    struct timer_list message_age_timer;
    struct kobject kobj;
    struct callback_head rcu;
    struct bridge_mcast_own_query ip4_own_query;
    struct bridge_mcast_own_query ip6_own_query;
    unsigned char multicast_router;
    struct bridge_mcast_stats *mcast_stats;
    struct timer_list multicast_router_timer;
    struct hlist_head mglist;
    struct hlist_node rlist;
    char sysfs_name[16];
    struct netpoll *np;
    int offload_fwd_mark;
    u16 group_fwd_mask;
    u16 backup_redirected_cnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct net_bridge_port {
    struct net_bridge *br;
    struct net_device *dev;
    struct list_head list;
    long unsigned int flags;
    struct net_bridge_vlan_group *vlgrp;
    struct net_bridge_port *backup_port;
    u8 priority;
    u8 state;
    u16 port_no;
    unsigned char topology_change_ack;
    unsigned char config_pending;
    port_id port_id;
    port_id designated_port;
    bridge_id designated_root;
    bridge_id designated_bridge;
    u32 path_cost;
    u32 designated_cost;
    long unsigned int designated_age;
    struct timer_list forward_delay_timer;
    struct timer_list hold_timer;
    struct timer_list message_age_timer;
    struct kobject kobj;
    struct callback_head rcu;
    struct bridge_mcast_own_query ip4_own_query;
    struct bridge_mcast_own_query ip6_own_query;
    unsigned char multicast_router;
    struct bridge_mcast_stats *mcast_stats;
    struct timer_list multicast_router_timer;
    struct hlist_head mglist;
    struct hlist_node rlist;
    char sysfs_name[16];
    struct netpoll *np;
    int offload_fwd_mark;
    u16 group_fwd_mask;
    u16 backup_redirected_cnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct net_bridge_port {
    struct net_bridge *br;
    struct net_device *dev;
    struct list_head list;
    long unsigned int flags;
    struct net_bridge_vlan_group *vlgrp;
    struct net_bridge_port *backup_port;
    u8 priority;
    u8 state;
    u16 port_no;
    unsigned char topology_change_ack;
    unsigned char config_pending;
    port_id port_id;
    port_id designated_port;
    bridge_id designated_root;
    bridge_id designated_bridge;
    u32 path_cost;
    u32 designated_cost;
    long unsigned int designated_age;
    struct timer_list forward_delay_timer;
    struct timer_list hold_timer;
    struct timer_list message_age_timer;
    struct kobject kobj;
    struct callback_head rcu;
    struct bridge_mcast_own_query ip4_own_query;
    struct bridge_mcast_own_query ip6_own_query;
    unsigned char multicast_router;
    struct bridge_mcast_stats *mcast_stats;
    struct timer_list multicast_router_timer;
    struct hlist_head mglist;
    struct hlist_node rlist;
    char sysfs_name[16];
    struct netpoll *np;
    int offload_fwd_mark;
    u16 group_fwd_mask;
    u16 backup_redirected_cnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct net_bridge_port {
    struct net_bridge *br;
    struct net_device *dev;
    struct list_head list;
    long unsigned int flags;
    struct net_bridge_vlan_group *vlgrp;
    struct net_bridge_port *backup_port;
    u8 priority;
    u8 state;
    u16 port_no;
    unsigned char topology_change_ack;
    unsigned char config_pending;
    port_id port_id;
    port_id designated_port;
    bridge_id designated_root;
    bridge_id designated_bridge;
    u32 path_cost;
    u32 designated_cost;
    long unsigned int designated_age;
    struct timer_list forward_delay_timer;
    struct timer_list hold_timer;
    struct timer_list message_age_timer;
    struct kobject kobj;
    struct callback_head rcu;
    struct bridge_mcast_own_query ip4_own_query;
    struct bridge_mcast_own_query ip6_own_query;
    unsigned char multicast_router;
    struct bridge_mcast_stats *mcast_stats;
    struct timer_list multicast_router_timer;
    struct hlist_head mglist;
    struct hlist_node rlist;
    char sysfs_name[16];
    struct netpoll *np;
    int offload_fwd_mark;
    u16 group_fwd_mask;
    u16 backup_redirected_cnt;
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
struct net_bridge_port {
    struct net_bridge *br;
    struct net_device *dev;
    struct list_head list;
    long unsigned int flags;
    struct net_bridge_vlan_group *vlgrp;
    struct net_bridge_port *backup_port;
    u8 priority;
    u8 state;
    u16 port_no;
    unsigned char topology_change_ack;
    unsigned char config_pending;
    port_id port_id;
    port_id designated_port;
    bridge_id designated_root;
    bridge_id designated_bridge;
    u32 path_cost;
    u32 designated_cost;
    long unsigned int designated_age;
    struct timer_list forward_delay_timer;
    struct timer_list hold_timer;
    struct timer_list message_age_timer;
    struct kobject kobj;
    struct callback_head rcu;
    struct bridge_mcast_own_query ip4_own_query;
    struct bridge_mcast_own_query ip6_own_query;
    unsigned char multicast_router;
    struct bridge_mcast_stats *mcast_stats;
    struct timer_list multicast_router_timer;
    struct hlist_head mglist;
    struct hlist_node rlist;
    char sysfs_name[16];
    struct netpoll *np;
    int offload_fwd_mark;
    u16 group_fwd_mask;
    u16 backup_redirected_cnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct net_bridge_port {
    struct net_bridge *br;
    struct net_device *dev;
    struct list_head list;
    long unsigned int flags;
    struct net_bridge_vlan_group *vlgrp;
    struct net_bridge_port *backup_port;
    u8 priority;
    u8 state;
    u16 port_no;
    unsigned char topology_change_ack;
    unsigned char config_pending;
    port_id port_id;
    port_id designated_port;
    bridge_id designated_root;
    bridge_id designated_bridge;
    u32 path_cost;
    u32 designated_cost;
    long unsigned int designated_age;
    struct timer_list forward_delay_timer;
    struct timer_list hold_timer;
    struct timer_list message_age_timer;
    struct kobject kobj;
    struct callback_head rcu;
    struct bridge_mcast_own_query ip4_own_query;
    struct bridge_mcast_own_query ip6_own_query;
    unsigned char multicast_router;
    struct bridge_mcast_stats *mcast_stats;
    struct timer_list multicast_router_timer;
    struct hlist_head mglist;
    struct hlist_node rlist;
    char sysfs_name[16];
    struct netpoll *np;
    int offload_fwd_mark;
    u16 group_fwd_mask;
    u16 backup_redirected_cnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct net_bridge_port {
    struct net_bridge *br;
    struct net_device *dev;
    struct list_head list;
    long unsigned int flags;
    struct net_bridge_vlan_group *vlgrp;
    struct net_bridge_port *backup_port;
    u8 priority;
    u8 state;
    u16 port_no;
    unsigned char topology_change_ack;
    unsigned char config_pending;
    port_id port_id;
    port_id designated_port;
    bridge_id designated_root;
    bridge_id designated_bridge;
    u32 path_cost;
    u32 designated_cost;
    long unsigned int designated_age;
    struct timer_list forward_delay_timer;
    struct timer_list hold_timer;
    struct timer_list message_age_timer;
    struct kobject kobj;
    struct callback_head rcu;
    struct bridge_mcast_own_query ip4_own_query;
    struct bridge_mcast_own_query ip6_own_query;
    unsigned char multicast_router;
    struct bridge_mcast_stats *mcast_stats;
    struct timer_list multicast_router_timer;
    struct hlist_head mglist;
    struct hlist_node rlist;
    char sysfs_name[16];
    struct netpoll *np;
    int offload_fwd_mark;
    u16 group_fwd_mask;
    u16 backup_redirected_cnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct net_bridge_port {
    struct net_bridge *br;
    struct net_device *dev;
    struct list_head list;
    long unsigned int flags;
    struct net_bridge_vlan_group *vlgrp;
    struct net_bridge_port *backup_port;
    u8 priority;
    u8 state;
    u16 port_no;
    unsigned char topology_change_ack;
    unsigned char config_pending;
    port_id port_id;
    port_id designated_port;
    bridge_id designated_root;
    bridge_id designated_bridge;
    u32 path_cost;
    u32 designated_cost;
    long unsigned int designated_age;
    struct timer_list forward_delay_timer;
    struct timer_list hold_timer;
    struct timer_list message_age_timer;
    struct kobject kobj;
    struct callback_head rcu;
    struct bridge_mcast_own_query ip4_own_query;
    struct bridge_mcast_own_query ip6_own_query;
    unsigned char multicast_router;
    struct bridge_mcast_stats *mcast_stats;
    struct timer_list multicast_router_timer;
    struct hlist_head mglist;
    struct hlist_node rlist;
    char sysfs_name[16];
    struct netpoll *np;
    int offload_fwd_mark;
    u16 group_fwd_mask;
    u16 backup_redirected_cnt;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct net_bridge_port *backup_port</code>
</li>
<li>
<b>Field added. </b>
<code>u16 backup_redirected_cnt</code>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct bridge_stp_xstats stp_xstats</code>
</li>
</ul>
</details>
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
<code>u32 multicast_eht_hosts_limit</code>
</li>
<li>
<b>Field added. </b>
<code>u32 multicast_eht_hosts_cnt</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct net_bridge_mcast_port multicast_ctx</code>
</li>
<li>
<b>Field added. </b>
<code>int hwdom</code>
</li>
<li>
<b>Field added. </b>
<code>int offload_count</code>
</li>
<li>
<b>Field added. </b>
<code>struct netdev_phys_item_id ppid</code>
</li>
<li>
<b>Field removed. </b>
<code>struct bridge_mcast_own_query ip4_own_query</code>
</li>
<li>
<b>Field removed. </b>
<code>struct bridge_mcast_own_query ip6_own_query</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned char multicast_router</code>
</li>
<li>
<b>Field removed. </b>
<code>struct timer_list multicast_router_timer</code>
</li>
<li>
<b>Field removed. </b>
<code>struct hlist_node rlist</code>
</li>
<li>
<b>Field removed. </b>
<code>int offload_fwd_mark</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>netdevice_tracker dev_tracker</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 backup_nhid</code>
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
