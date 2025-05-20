# Struct: <code>net_device_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct net_device_ops {
    int (*ndo_init)(struct net_device *);
    void (*ndo_uninit)(struct net_device *);
    int (*ndo_open)(struct net_device *);
    int (*ndo_stop)(struct net_device *);
    netdev_tx_t (*ndo_start_xmit)(struct sk_buff *, struct net_device *);
    u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, void *, select_queue_fallback_t);
    void (*ndo_change_rx_flags)(struct net_device *, int);
    void (*ndo_set_rx_mode)(struct net_device *);
    int (*ndo_set_mac_address)(struct net_device *, void *);
    int (*ndo_validate_addr)(struct net_device *);
    int (*ndo_do_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_set_config)(struct net_device *, struct ifmap *);
    int (*ndo_change_mtu)(struct net_device *, int);
    int (*ndo_neigh_setup)(struct net_device *, struct neigh_parms *);
    void (*ndo_tx_timeout)(struct net_device *);
    struct rtnl_link_stats64 * (*ndo_get_stats64)(struct net_device *, struct rtnl_link_stats64 *);
    struct net_device_stats * (*ndo_get_stats)(struct net_device *);
    int (*ndo_vlan_rx_add_vid)(struct net_device *, __be16, u16);
    int (*ndo_vlan_rx_kill_vid)(struct net_device *, __be16, u16);
    void (*ndo_poll_controller)(struct net_device *);
    int (*ndo_netpoll_setup)(struct net_device *, struct netpoll_info *);
    void (*ndo_netpoll_cleanup)(struct net_device *);
    int (*ndo_busy_poll)(struct napi_struct *);
    int (*ndo_set_vf_mac)(struct net_device *, int, u8 *);
    int (*ndo_set_vf_vlan)(struct net_device *, int, u16, u8);
    int (*ndo_set_vf_rate)(struct net_device *, int, int, int);
    int (*ndo_set_vf_spoofchk)(struct net_device *, int, bool);
    int (*ndo_set_vf_trust)(struct net_device *, int, bool);
    int (*ndo_get_vf_config)(struct net_device *, int, struct ifla_vf_info *);
    int (*ndo_set_vf_link_state)(struct net_device *, int, int);
    int (*ndo_get_vf_stats)(struct net_device *, int, struct ifla_vf_stats *);
    int (*ndo_set_vf_port)(struct net_device *, int, struct nlattr **);
    int (*ndo_get_vf_port)(struct net_device *, int, struct sk_buff *);
    int (*ndo_set_vf_rss_query_en)(struct net_device *, int, bool);
    int (*ndo_setup_tc)(struct net_device *, u32, __be16, struct tc_to_netdev *);
    int (*ndo_fcoe_enable)(struct net_device *);
    int (*ndo_fcoe_disable)(struct net_device *);
    int (*ndo_fcoe_ddp_setup)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_ddp_done)(struct net_device *, u16);
    int (*ndo_fcoe_ddp_target)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_get_hbainfo)(struct net_device *, struct netdev_fcoe_hbainfo *);
    int (*ndo_fcoe_get_wwn)(struct net_device *, u64 *, int);
    int (*ndo_rx_flow_steer)(struct net_device *, const struct sk_buff *, u16, u32);
    int (*ndo_add_slave)(struct net_device *, struct net_device *);
    int (*ndo_del_slave)(struct net_device *, struct net_device *);
    netdev_features_t (*ndo_fix_features)(struct net_device *, netdev_features_t);
    int (*ndo_set_features)(struct net_device *, netdev_features_t);
    int (*ndo_neigh_construct)(struct neighbour *);
    void (*ndo_neigh_destroy)(struct neighbour *);
    int (*ndo_fdb_add)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, u16);
    int (*ndo_fdb_del)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16);
    int (*ndo_fdb_dump)(struct sk_buff *, struct netlink_callback *, struct net_device *, struct net_device *, int);
    int (*ndo_bridge_setlink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_bridge_getlink)(struct sk_buff *, u32, u32, struct net_device *, u32, int);
    int (*ndo_bridge_dellink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_change_carrier)(struct net_device *, bool);
    int (*ndo_get_phys_port_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_phys_port_name)(struct net_device *, char *, size_t);
    void (*ndo_add_vxlan_port)(struct net_device *, sa_family_t, __be16);
    void (*ndo_del_vxlan_port)(struct net_device *, sa_family_t, __be16);
    void (*ndo_add_geneve_port)(struct net_device *, sa_family_t, __be16);
    void (*ndo_del_geneve_port)(struct net_device *, sa_family_t, __be16);
    void * (*ndo_dfwd_add_station)(struct net_device *, struct net_device *);
    void (*ndo_dfwd_del_station)(struct net_device *, void *);
    netdev_tx_t (*ndo_dfwd_start_xmit)(struct sk_buff *, struct net_device *, void *);
    int (*ndo_get_lock_subclass)(struct net_device *);
    netdev_features_t (*ndo_features_check)(struct sk_buff *, struct net_device *, netdev_features_t);
    int (*ndo_set_tx_maxrate)(struct net_device *, int, u32);
    int (*ndo_get_iflink)(const struct net_device *);
    int (*ndo_change_proto_down)(struct net_device *, bool);
    int (*ndo_fill_metadata_dst)(struct net_device *, struct sk_buff *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct net_device_ops {
    int (*ndo_init)(struct net_device *);
    void (*ndo_uninit)(struct net_device *);
    int (*ndo_open)(struct net_device *);
    int (*ndo_stop)(struct net_device *);
    netdev_tx_t (*ndo_start_xmit)(struct sk_buff *, struct net_device *);
    netdev_features_t (*ndo_features_check)(struct sk_buff *, struct net_device *, netdev_features_t);
    u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, void *, select_queue_fallback_t);
    void (*ndo_change_rx_flags)(struct net_device *, int);
    void (*ndo_set_rx_mode)(struct net_device *);
    int (*ndo_set_mac_address)(struct net_device *, void *);
    int (*ndo_validate_addr)(struct net_device *);
    int (*ndo_do_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_set_config)(struct net_device *, struct ifmap *);
    int (*ndo_change_mtu)(struct net_device *, int);
    int (*ndo_neigh_setup)(struct net_device *, struct neigh_parms *);
    void (*ndo_tx_timeout)(struct net_device *);
    struct rtnl_link_stats64 * (*ndo_get_stats64)(struct net_device *, struct rtnl_link_stats64 *);
    struct net_device_stats * (*ndo_get_stats)(struct net_device *);
    int (*ndo_vlan_rx_add_vid)(struct net_device *, __be16, u16);
    int (*ndo_vlan_rx_kill_vid)(struct net_device *, __be16, u16);
    void (*ndo_poll_controller)(struct net_device *);
    int (*ndo_netpoll_setup)(struct net_device *, struct netpoll_info *);
    void (*ndo_netpoll_cleanup)(struct net_device *);
    int (*ndo_busy_poll)(struct napi_struct *);
    int (*ndo_set_vf_mac)(struct net_device *, int, u8 *);
    int (*ndo_set_vf_vlan)(struct net_device *, int, u16, u8);
    int (*ndo_set_vf_rate)(struct net_device *, int, int, int);
    int (*ndo_set_vf_spoofchk)(struct net_device *, int, bool);
    int (*ndo_set_vf_trust)(struct net_device *, int, bool);
    int (*ndo_get_vf_config)(struct net_device *, int, struct ifla_vf_info *);
    int (*ndo_set_vf_link_state)(struct net_device *, int, int);
    int (*ndo_get_vf_stats)(struct net_device *, int, struct ifla_vf_stats *);
    int (*ndo_set_vf_port)(struct net_device *, int, struct nlattr **);
    int (*ndo_get_vf_port)(struct net_device *, int, struct sk_buff *);
    int (*ndo_set_vf_guid)(struct net_device *, int, u64, int);
    int (*ndo_set_vf_rss_query_en)(struct net_device *, int, bool);
    int (*ndo_setup_tc)(struct net_device *, u32, __be16, struct tc_to_netdev *);
    int (*ndo_fcoe_enable)(struct net_device *);
    int (*ndo_fcoe_disable)(struct net_device *);
    int (*ndo_fcoe_ddp_setup)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_ddp_done)(struct net_device *, u16);
    int (*ndo_fcoe_ddp_target)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_get_hbainfo)(struct net_device *, struct netdev_fcoe_hbainfo *);
    int (*ndo_fcoe_get_wwn)(struct net_device *, u64 *, int);
    int (*ndo_rx_flow_steer)(struct net_device *, const struct sk_buff *, u16, u32);
    int (*ndo_add_slave)(struct net_device *, struct net_device *);
    int (*ndo_del_slave)(struct net_device *, struct net_device *);
    netdev_features_t (*ndo_fix_features)(struct net_device *, netdev_features_t);
    int (*ndo_set_features)(struct net_device *, netdev_features_t);
    int (*ndo_neigh_construct)(struct net_device *, struct neighbour *);
    void (*ndo_neigh_destroy)(struct net_device *, struct neighbour *);
    int (*ndo_fdb_add)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, u16);
    int (*ndo_fdb_del)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16);
    int (*ndo_fdb_dump)(struct sk_buff *, struct netlink_callback *, struct net_device *, struct net_device *, int);
    int (*ndo_bridge_setlink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_bridge_getlink)(struct sk_buff *, u32, u32, struct net_device *, u32, int);
    int (*ndo_bridge_dellink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_change_carrier)(struct net_device *, bool);
    int (*ndo_get_phys_port_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_phys_port_name)(struct net_device *, char *, size_t);
    void (*ndo_udp_tunnel_add)(struct net_device *, struct udp_tunnel_info *);
    void (*ndo_udp_tunnel_del)(struct net_device *, struct udp_tunnel_info *);
    void * (*ndo_dfwd_add_station)(struct net_device *, struct net_device *);
    void (*ndo_dfwd_del_station)(struct net_device *, void *);
    netdev_tx_t (*ndo_dfwd_start_xmit)(struct sk_buff *, struct net_device *, void *);
    int (*ndo_get_lock_subclass)(struct net_device *);
    int (*ndo_set_tx_maxrate)(struct net_device *, int, u32);
    int (*ndo_get_iflink)(const struct net_device *);
    int (*ndo_change_proto_down)(struct net_device *, bool);
    int (*ndo_fill_metadata_dst)(struct net_device *, struct sk_buff *);
    void (*ndo_set_rx_headroom)(struct net_device *, int);
    int (*ndo_xdp)(struct net_device *, struct netdev_xdp *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct net_device_ops {
    int (*ndo_init)(struct net_device *);
    void (*ndo_uninit)(struct net_device *);
    int (*ndo_open)(struct net_device *);
    int (*ndo_stop)(struct net_device *);
    netdev_tx_t (*ndo_start_xmit)(struct sk_buff *, struct net_device *);
    netdev_features_t (*ndo_features_check)(struct sk_buff *, struct net_device *, netdev_features_t);
    u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, void *, select_queue_fallback_t);
    void (*ndo_change_rx_flags)(struct net_device *, int);
    void (*ndo_set_rx_mode)(struct net_device *);
    int (*ndo_set_mac_address)(struct net_device *, void *);
    int (*ndo_validate_addr)(struct net_device *);
    int (*ndo_do_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_set_config)(struct net_device *, struct ifmap *);
    int (*ndo_change_mtu)(struct net_device *, int);
    int (*ndo_neigh_setup)(struct net_device *, struct neigh_parms *);
    void (*ndo_tx_timeout)(struct net_device *);
    struct rtnl_link_stats64 * (*ndo_get_stats64)(struct net_device *, struct rtnl_link_stats64 *);
    bool (*ndo_has_offload_stats)(const struct net_device *, int);
    int (*ndo_get_offload_stats)(int, const struct net_device *, void *);
    struct net_device_stats * (*ndo_get_stats)(struct net_device *);
    int (*ndo_vlan_rx_add_vid)(struct net_device *, __be16, u16);
    int (*ndo_vlan_rx_kill_vid)(struct net_device *, __be16, u16);
    void (*ndo_poll_controller)(struct net_device *);
    int (*ndo_netpoll_setup)(struct net_device *, struct netpoll_info *);
    void (*ndo_netpoll_cleanup)(struct net_device *);
    int (*ndo_busy_poll)(struct napi_struct *);
    int (*ndo_set_vf_mac)(struct net_device *, int, u8 *);
    int (*ndo_set_vf_vlan)(struct net_device *, int, u16, u8, __be16);
    int (*ndo_set_vf_rate)(struct net_device *, int, int, int);
    int (*ndo_set_vf_spoofchk)(struct net_device *, int, bool);
    int (*ndo_set_vf_trust)(struct net_device *, int, bool);
    int (*ndo_get_vf_config)(struct net_device *, int, struct ifla_vf_info *);
    int (*ndo_set_vf_link_state)(struct net_device *, int, int);
    int (*ndo_get_vf_stats)(struct net_device *, int, struct ifla_vf_stats *);
    int (*ndo_set_vf_port)(struct net_device *, int, struct nlattr **);
    int (*ndo_get_vf_port)(struct net_device *, int, struct sk_buff *);
    int (*ndo_set_vf_guid)(struct net_device *, int, u64, int);
    int (*ndo_set_vf_rss_query_en)(struct net_device *, int, bool);
    int (*ndo_setup_tc)(struct net_device *, u32, __be16, struct tc_to_netdev *);
    int (*ndo_fcoe_enable)(struct net_device *);
    int (*ndo_fcoe_disable)(struct net_device *);
    int (*ndo_fcoe_ddp_setup)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_ddp_done)(struct net_device *, u16);
    int (*ndo_fcoe_ddp_target)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_get_hbainfo)(struct net_device *, struct netdev_fcoe_hbainfo *);
    int (*ndo_fcoe_get_wwn)(struct net_device *, u64 *, int);
    int (*ndo_rx_flow_steer)(struct net_device *, const struct sk_buff *, u16, u32);
    int (*ndo_add_slave)(struct net_device *, struct net_device *);
    int (*ndo_del_slave)(struct net_device *, struct net_device *);
    netdev_features_t (*ndo_fix_features)(struct net_device *, netdev_features_t);
    int (*ndo_set_features)(struct net_device *, netdev_features_t);
    int (*ndo_neigh_construct)(struct net_device *, struct neighbour *);
    void (*ndo_neigh_destroy)(struct net_device *, struct neighbour *);
    int (*ndo_fdb_add)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, u16);
    int (*ndo_fdb_del)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16);
    int (*ndo_fdb_dump)(struct sk_buff *, struct netlink_callback *, struct net_device *, struct net_device *, int *);
    int (*ndo_bridge_setlink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_bridge_getlink)(struct sk_buff *, u32, u32, struct net_device *, u32, int);
    int (*ndo_bridge_dellink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_change_carrier)(struct net_device *, bool);
    int (*ndo_get_phys_port_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_phys_port_name)(struct net_device *, char *, size_t);
    void (*ndo_udp_tunnel_add)(struct net_device *, struct udp_tunnel_info *);
    void (*ndo_udp_tunnel_del)(struct net_device *, struct udp_tunnel_info *);
    void * (*ndo_dfwd_add_station)(struct net_device *, struct net_device *);
    void (*ndo_dfwd_del_station)(struct net_device *, void *);
    netdev_tx_t (*ndo_dfwd_start_xmit)(struct sk_buff *, struct net_device *, void *);
    int (*ndo_get_lock_subclass)(struct net_device *);
    int (*ndo_set_tx_maxrate)(struct net_device *, int, u32);
    int (*ndo_get_iflink)(const struct net_device *);
    int (*ndo_change_proto_down)(struct net_device *, bool);
    int (*ndo_fill_metadata_dst)(struct net_device *, struct sk_buff *);
    void (*ndo_set_rx_headroom)(struct net_device *, int);
    int (*ndo_xdp)(struct net_device *, struct netdev_xdp *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct net_device_ops {
    int (*ndo_init)(struct net_device *);
    void (*ndo_uninit)(struct net_device *);
    int (*ndo_open)(struct net_device *);
    int (*ndo_stop)(struct net_device *);
    netdev_tx_t (*ndo_start_xmit)(struct sk_buff *, struct net_device *);
    netdev_features_t (*ndo_features_check)(struct sk_buff *, struct net_device *, netdev_features_t);
    u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, void *, select_queue_fallback_t);
    void (*ndo_change_rx_flags)(struct net_device *, int);
    void (*ndo_set_rx_mode)(struct net_device *);
    int (*ndo_set_mac_address)(struct net_device *, void *);
    int (*ndo_validate_addr)(struct net_device *);
    int (*ndo_do_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_set_config)(struct net_device *, struct ifmap *);
    int (*ndo_change_mtu)(struct net_device *, int);
    int (*ndo_neigh_setup)(struct net_device *, struct neigh_parms *);
    void (*ndo_tx_timeout)(struct net_device *);
    void (*ndo_get_stats64)(struct net_device *, struct rtnl_link_stats64 *);
    bool (*ndo_has_offload_stats)(const struct net_device *, int);
    int (*ndo_get_offload_stats)(int, const struct net_device *, void *);
    struct net_device_stats * (*ndo_get_stats)(struct net_device *);
    int (*ndo_vlan_rx_add_vid)(struct net_device *, __be16, u16);
    int (*ndo_vlan_rx_kill_vid)(struct net_device *, __be16, u16);
    void (*ndo_poll_controller)(struct net_device *);
    int (*ndo_netpoll_setup)(struct net_device *, struct netpoll_info *);
    void (*ndo_netpoll_cleanup)(struct net_device *);
    int (*ndo_set_vf_mac)(struct net_device *, int, u8 *);
    int (*ndo_set_vf_vlan)(struct net_device *, int, u16, u8, __be16);
    int (*ndo_set_vf_rate)(struct net_device *, int, int, int);
    int (*ndo_set_vf_spoofchk)(struct net_device *, int, bool);
    int (*ndo_set_vf_trust)(struct net_device *, int, bool);
    int (*ndo_get_vf_config)(struct net_device *, int, struct ifla_vf_info *);
    int (*ndo_set_vf_link_state)(struct net_device *, int, int);
    int (*ndo_get_vf_stats)(struct net_device *, int, struct ifla_vf_stats *);
    int (*ndo_set_vf_port)(struct net_device *, int, struct nlattr **);
    int (*ndo_get_vf_port)(struct net_device *, int, struct sk_buff *);
    int (*ndo_set_vf_guid)(struct net_device *, int, u64, int);
    int (*ndo_set_vf_rss_query_en)(struct net_device *, int, bool);
    int (*ndo_setup_tc)(struct net_device *, u32, u32, __be16, struct tc_to_netdev *);
    int (*ndo_fcoe_enable)(struct net_device *);
    int (*ndo_fcoe_disable)(struct net_device *);
    int (*ndo_fcoe_ddp_setup)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_ddp_done)(struct net_device *, u16);
    int (*ndo_fcoe_ddp_target)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_get_hbainfo)(struct net_device *, struct netdev_fcoe_hbainfo *);
    int (*ndo_fcoe_get_wwn)(struct net_device *, u64 *, int);
    int (*ndo_rx_flow_steer)(struct net_device *, const struct sk_buff *, u16, u32);
    int (*ndo_add_slave)(struct net_device *, struct net_device *);
    int (*ndo_del_slave)(struct net_device *, struct net_device *);
    netdev_features_t (*ndo_fix_features)(struct net_device *, netdev_features_t);
    int (*ndo_set_features)(struct net_device *, netdev_features_t);
    int (*ndo_neigh_construct)(struct net_device *, struct neighbour *);
    void (*ndo_neigh_destroy)(struct net_device *, struct neighbour *);
    int (*ndo_fdb_add)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, u16);
    int (*ndo_fdb_del)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16);
    int (*ndo_fdb_dump)(struct sk_buff *, struct netlink_callback *, struct net_device *, struct net_device *, int *);
    int (*ndo_bridge_setlink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_bridge_getlink)(struct sk_buff *, u32, u32, struct net_device *, u32, int);
    int (*ndo_bridge_dellink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_change_carrier)(struct net_device *, bool);
    int (*ndo_get_phys_port_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_phys_port_name)(struct net_device *, char *, size_t);
    void (*ndo_udp_tunnel_add)(struct net_device *, struct udp_tunnel_info *);
    void (*ndo_udp_tunnel_del)(struct net_device *, struct udp_tunnel_info *);
    void * (*ndo_dfwd_add_station)(struct net_device *, struct net_device *);
    void (*ndo_dfwd_del_station)(struct net_device *, void *);
    int (*ndo_get_lock_subclass)(struct net_device *);
    int (*ndo_set_tx_maxrate)(struct net_device *, int, u32);
    int (*ndo_get_iflink)(const struct net_device *);
    int (*ndo_change_proto_down)(struct net_device *, bool);
    int (*ndo_fill_metadata_dst)(struct net_device *, struct sk_buff *);
    void (*ndo_set_rx_headroom)(struct net_device *, int);
    int (*ndo_xdp)(struct net_device *, struct netdev_xdp *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct net_device_ops {
    int (*ndo_init)(struct net_device *);
    void (*ndo_uninit)(struct net_device *);
    int (*ndo_open)(struct net_device *);
    int (*ndo_stop)(struct net_device *);
    netdev_tx_t (*ndo_start_xmit)(struct sk_buff *, struct net_device *);
    netdev_features_t (*ndo_features_check)(struct sk_buff *, struct net_device *, netdev_features_t);
    u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, void *, select_queue_fallback_t);
    void (*ndo_change_rx_flags)(struct net_device *, int);
    void (*ndo_set_rx_mode)(struct net_device *);
    int (*ndo_set_mac_address)(struct net_device *, void *);
    int (*ndo_validate_addr)(struct net_device *);
    int (*ndo_do_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_set_config)(struct net_device *, struct ifmap *);
    int (*ndo_change_mtu)(struct net_device *, int);
    int (*ndo_neigh_setup)(struct net_device *, struct neigh_parms *);
    void (*ndo_tx_timeout)(struct net_device *);
    void (*ndo_get_stats64)(struct net_device *, struct rtnl_link_stats64 *);
    bool (*ndo_has_offload_stats)(const struct net_device *, int);
    int (*ndo_get_offload_stats)(int, const struct net_device *, void *);
    struct net_device_stats * (*ndo_get_stats)(struct net_device *);
    int (*ndo_vlan_rx_add_vid)(struct net_device *, __be16, u16);
    int (*ndo_vlan_rx_kill_vid)(struct net_device *, __be16, u16);
    void (*ndo_poll_controller)(struct net_device *);
    int (*ndo_netpoll_setup)(struct net_device *, struct netpoll_info *);
    void (*ndo_netpoll_cleanup)(struct net_device *);
    int (*ndo_set_vf_mac)(struct net_device *, int, u8 *);
    int (*ndo_set_vf_vlan)(struct net_device *, int, u16, u8, __be16);
    int (*ndo_set_vf_rate)(struct net_device *, int, int, int);
    int (*ndo_set_vf_spoofchk)(struct net_device *, int, bool);
    int (*ndo_set_vf_trust)(struct net_device *, int, bool);
    int (*ndo_get_vf_config)(struct net_device *, int, struct ifla_vf_info *);
    int (*ndo_set_vf_link_state)(struct net_device *, int, int);
    int (*ndo_get_vf_stats)(struct net_device *, int, struct ifla_vf_stats *);
    int (*ndo_set_vf_port)(struct net_device *, int, struct nlattr **);
    int (*ndo_get_vf_port)(struct net_device *, int, struct sk_buff *);
    int (*ndo_set_vf_guid)(struct net_device *, int, u64, int);
    int (*ndo_set_vf_rss_query_en)(struct net_device *, int, bool);
    int (*ndo_setup_tc)(struct net_device *, enum tc_setup_type, void *);
    int (*ndo_fcoe_enable)(struct net_device *);
    int (*ndo_fcoe_disable)(struct net_device *);
    int (*ndo_fcoe_ddp_setup)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_ddp_done)(struct net_device *, u16);
    int (*ndo_fcoe_ddp_target)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_get_hbainfo)(struct net_device *, struct netdev_fcoe_hbainfo *);
    int (*ndo_fcoe_get_wwn)(struct net_device *, u64 *, int);
    int (*ndo_rx_flow_steer)(struct net_device *, const struct sk_buff *, u16, u32);
    int (*ndo_add_slave)(struct net_device *, struct net_device *, struct netlink_ext_ack *);
    int (*ndo_del_slave)(struct net_device *, struct net_device *);
    netdev_features_t (*ndo_fix_features)(struct net_device *, netdev_features_t);
    int (*ndo_set_features)(struct net_device *, netdev_features_t);
    int (*ndo_neigh_construct)(struct net_device *, struct neighbour *);
    void (*ndo_neigh_destroy)(struct net_device *, struct neighbour *);
    int (*ndo_fdb_add)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, u16);
    int (*ndo_fdb_del)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16);
    int (*ndo_fdb_dump)(struct sk_buff *, struct netlink_callback *, struct net_device *, struct net_device *, int *);
    int (*ndo_bridge_setlink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_bridge_getlink)(struct sk_buff *, u32, u32, struct net_device *, u32, int);
    int (*ndo_bridge_dellink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_change_carrier)(struct net_device *, bool);
    int (*ndo_get_phys_port_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_phys_port_name)(struct net_device *, char *, size_t);
    void (*ndo_udp_tunnel_add)(struct net_device *, struct udp_tunnel_info *);
    void (*ndo_udp_tunnel_del)(struct net_device *, struct udp_tunnel_info *);
    void * (*ndo_dfwd_add_station)(struct net_device *, struct net_device *);
    void (*ndo_dfwd_del_station)(struct net_device *, void *);
    int (*ndo_get_lock_subclass)(struct net_device *);
    int (*ndo_set_tx_maxrate)(struct net_device *, int, u32);
    int (*ndo_get_iflink)(const struct net_device *);
    int (*ndo_change_proto_down)(struct net_device *, bool);
    int (*ndo_fill_metadata_dst)(struct net_device *, struct sk_buff *);
    void (*ndo_set_rx_headroom)(struct net_device *, int);
    int (*ndo_bpf)(struct net_device *, struct netdev_bpf *);
    int (*ndo_xdp_xmit)(struct net_device *, struct xdp_buff *);
    void (*ndo_xdp_flush)(struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct net_device_ops {
    int (*ndo_init)(struct net_device *);
    void (*ndo_uninit)(struct net_device *);
    int (*ndo_open)(struct net_device *);
    int (*ndo_stop)(struct net_device *);
    netdev_tx_t (*ndo_start_xmit)(struct sk_buff *, struct net_device *);
    netdev_features_t (*ndo_features_check)(struct sk_buff *, struct net_device *, netdev_features_t);
    u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, void *, select_queue_fallback_t);
    void (*ndo_change_rx_flags)(struct net_device *, int);
    void (*ndo_set_rx_mode)(struct net_device *);
    int (*ndo_set_mac_address)(struct net_device *, void *);
    int (*ndo_validate_addr)(struct net_device *);
    int (*ndo_do_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_set_config)(struct net_device *, struct ifmap *);
    int (*ndo_change_mtu)(struct net_device *, int);
    int (*ndo_neigh_setup)(struct net_device *, struct neigh_parms *);
    void (*ndo_tx_timeout)(struct net_device *);
    void (*ndo_get_stats64)(struct net_device *, struct rtnl_link_stats64 *);
    bool (*ndo_has_offload_stats)(const struct net_device *, int);
    int (*ndo_get_offload_stats)(int, const struct net_device *, void *);
    struct net_device_stats * (*ndo_get_stats)(struct net_device *);
    int (*ndo_vlan_rx_add_vid)(struct net_device *, __be16, u16);
    int (*ndo_vlan_rx_kill_vid)(struct net_device *, __be16, u16);
    void (*ndo_poll_controller)(struct net_device *);
    int (*ndo_netpoll_setup)(struct net_device *, struct netpoll_info *);
    void (*ndo_netpoll_cleanup)(struct net_device *);
    int (*ndo_set_vf_mac)(struct net_device *, int, u8 *);
    int (*ndo_set_vf_vlan)(struct net_device *, int, u16, u8, __be16);
    int (*ndo_set_vf_rate)(struct net_device *, int, int, int);
    int (*ndo_set_vf_spoofchk)(struct net_device *, int, bool);
    int (*ndo_set_vf_trust)(struct net_device *, int, bool);
    int (*ndo_get_vf_config)(struct net_device *, int, struct ifla_vf_info *);
    int (*ndo_set_vf_link_state)(struct net_device *, int, int);
    int (*ndo_get_vf_stats)(struct net_device *, int, struct ifla_vf_stats *);
    int (*ndo_set_vf_port)(struct net_device *, int, struct nlattr **);
    int (*ndo_get_vf_port)(struct net_device *, int, struct sk_buff *);
    int (*ndo_set_vf_guid)(struct net_device *, int, u64, int);
    int (*ndo_set_vf_rss_query_en)(struct net_device *, int, bool);
    int (*ndo_setup_tc)(struct net_device *, enum tc_setup_type, void *);
    int (*ndo_fcoe_enable)(struct net_device *);
    int (*ndo_fcoe_disable)(struct net_device *);
    int (*ndo_fcoe_ddp_setup)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_ddp_done)(struct net_device *, u16);
    int (*ndo_fcoe_ddp_target)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_get_hbainfo)(struct net_device *, struct netdev_fcoe_hbainfo *);
    int (*ndo_fcoe_get_wwn)(struct net_device *, u64 *, int);
    int (*ndo_rx_flow_steer)(struct net_device *, const struct sk_buff *, u16, u32);
    int (*ndo_add_slave)(struct net_device *, struct net_device *, struct netlink_ext_ack *);
    int (*ndo_del_slave)(struct net_device *, struct net_device *);
    netdev_features_t (*ndo_fix_features)(struct net_device *, netdev_features_t);
    int (*ndo_set_features)(struct net_device *, netdev_features_t);
    int (*ndo_neigh_construct)(struct net_device *, struct neighbour *);
    void (*ndo_neigh_destroy)(struct net_device *, struct neighbour *);
    int (*ndo_fdb_add)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, u16);
    int (*ndo_fdb_del)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16);
    int (*ndo_fdb_dump)(struct sk_buff *, struct netlink_callback *, struct net_device *, struct net_device *, int *);
    int (*ndo_bridge_setlink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_bridge_getlink)(struct sk_buff *, u32, u32, struct net_device *, u32, int);
    int (*ndo_bridge_dellink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_change_carrier)(struct net_device *, bool);
    int (*ndo_get_phys_port_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_phys_port_name)(struct net_device *, char *, size_t);
    void (*ndo_udp_tunnel_add)(struct net_device *, struct udp_tunnel_info *);
    void (*ndo_udp_tunnel_del)(struct net_device *, struct udp_tunnel_info *);
    void * (*ndo_dfwd_add_station)(struct net_device *, struct net_device *);
    void (*ndo_dfwd_del_station)(struct net_device *, void *);
    int (*ndo_get_lock_subclass)(struct net_device *);
    int (*ndo_set_tx_maxrate)(struct net_device *, int, u32);
    int (*ndo_get_iflink)(const struct net_device *);
    int (*ndo_change_proto_down)(struct net_device *, bool);
    int (*ndo_fill_metadata_dst)(struct net_device *, struct sk_buff *);
    void (*ndo_set_rx_headroom)(struct net_device *, int);
    int (*ndo_bpf)(struct net_device *, struct netdev_bpf *);
    int (*ndo_xdp_xmit)(struct net_device *, int, struct xdp_frame **, u32);
    int (*ndo_xsk_async_xmit)(struct net_device *, u32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct net_device_ops {
    int (*ndo_init)(struct net_device *);
    void (*ndo_uninit)(struct net_device *);
    int (*ndo_open)(struct net_device *);
    int (*ndo_stop)(struct net_device *);
    netdev_tx_t (*ndo_start_xmit)(struct sk_buff *, struct net_device *);
    netdev_features_t (*ndo_features_check)(struct sk_buff *, struct net_device *, netdev_features_t);
    u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, struct net_device *, select_queue_fallback_t);
    void (*ndo_change_rx_flags)(struct net_device *, int);
    void (*ndo_set_rx_mode)(struct net_device *);
    int (*ndo_set_mac_address)(struct net_device *, void *);
    int (*ndo_validate_addr)(struct net_device *);
    int (*ndo_do_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_set_config)(struct net_device *, struct ifmap *);
    int (*ndo_change_mtu)(struct net_device *, int);
    int (*ndo_neigh_setup)(struct net_device *, struct neigh_parms *);
    void (*ndo_tx_timeout)(struct net_device *);
    void (*ndo_get_stats64)(struct net_device *, struct rtnl_link_stats64 *);
    bool (*ndo_has_offload_stats)(const struct net_device *, int);
    int (*ndo_get_offload_stats)(int, const struct net_device *, void *);
    struct net_device_stats * (*ndo_get_stats)(struct net_device *);
    int (*ndo_vlan_rx_add_vid)(struct net_device *, __be16, u16);
    int (*ndo_vlan_rx_kill_vid)(struct net_device *, __be16, u16);
    void (*ndo_poll_controller)(struct net_device *);
    int (*ndo_netpoll_setup)(struct net_device *, struct netpoll_info *);
    void (*ndo_netpoll_cleanup)(struct net_device *);
    int (*ndo_set_vf_mac)(struct net_device *, int, u8 *);
    int (*ndo_set_vf_vlan)(struct net_device *, int, u16, u8, __be16);
    int (*ndo_set_vf_rate)(struct net_device *, int, int, int);
    int (*ndo_set_vf_spoofchk)(struct net_device *, int, bool);
    int (*ndo_set_vf_trust)(struct net_device *, int, bool);
    int (*ndo_get_vf_config)(struct net_device *, int, struct ifla_vf_info *);
    int (*ndo_set_vf_link_state)(struct net_device *, int, int);
    int (*ndo_get_vf_stats)(struct net_device *, int, struct ifla_vf_stats *);
    int (*ndo_set_vf_port)(struct net_device *, int, struct nlattr **);
    int (*ndo_get_vf_port)(struct net_device *, int, struct sk_buff *);
    int (*ndo_set_vf_guid)(struct net_device *, int, u64, int);
    int (*ndo_set_vf_rss_query_en)(struct net_device *, int, bool);
    int (*ndo_setup_tc)(struct net_device *, enum tc_setup_type, void *);
    int (*ndo_fcoe_enable)(struct net_device *);
    int (*ndo_fcoe_disable)(struct net_device *);
    int (*ndo_fcoe_ddp_setup)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_ddp_done)(struct net_device *, u16);
    int (*ndo_fcoe_ddp_target)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_get_hbainfo)(struct net_device *, struct netdev_fcoe_hbainfo *);
    int (*ndo_fcoe_get_wwn)(struct net_device *, u64 *, int);
    int (*ndo_rx_flow_steer)(struct net_device *, const struct sk_buff *, u16, u32);
    int (*ndo_add_slave)(struct net_device *, struct net_device *, struct netlink_ext_ack *);
    int (*ndo_del_slave)(struct net_device *, struct net_device *);
    netdev_features_t (*ndo_fix_features)(struct net_device *, netdev_features_t);
    int (*ndo_set_features)(struct net_device *, netdev_features_t);
    int (*ndo_neigh_construct)(struct net_device *, struct neighbour *);
    void (*ndo_neigh_destroy)(struct net_device *, struct neighbour *);
    int (*ndo_fdb_add)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, u16);
    int (*ndo_fdb_del)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16);
    int (*ndo_fdb_dump)(struct sk_buff *, struct netlink_callback *, struct net_device *, struct net_device *, int *);
    int (*ndo_fdb_get)(struct sk_buff *, struct nlattr **, struct net_device *, const unsigned char *, u16, u32, u32, struct netlink_ext_ack *);
    int (*ndo_bridge_setlink)(struct net_device *, struct nlmsghdr *, u16, struct netlink_ext_ack *);
    int (*ndo_bridge_getlink)(struct sk_buff *, u32, u32, struct net_device *, u32, int);
    int (*ndo_bridge_dellink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_change_carrier)(struct net_device *, bool);
    int (*ndo_get_phys_port_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_phys_port_name)(struct net_device *, char *, size_t);
    void (*ndo_udp_tunnel_add)(struct net_device *, struct udp_tunnel_info *);
    void (*ndo_udp_tunnel_del)(struct net_device *, struct udp_tunnel_info *);
    void * (*ndo_dfwd_add_station)(struct net_device *, struct net_device *);
    void (*ndo_dfwd_del_station)(struct net_device *, void *);
    int (*ndo_get_lock_subclass)(struct net_device *);
    int (*ndo_set_tx_maxrate)(struct net_device *, int, u32);
    int (*ndo_get_iflink)(const struct net_device *);
    int (*ndo_change_proto_down)(struct net_device *, bool);
    int (*ndo_fill_metadata_dst)(struct net_device *, struct sk_buff *);
    void (*ndo_set_rx_headroom)(struct net_device *, int);
    int (*ndo_bpf)(struct net_device *, struct netdev_bpf *);
    int (*ndo_xdp_xmit)(struct net_device *, int, struct xdp_frame **, u32);
    int (*ndo_xsk_async_xmit)(struct net_device *, u32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct net_device_ops {
    int (*ndo_init)(struct net_device *);
    void (*ndo_uninit)(struct net_device *);
    int (*ndo_open)(struct net_device *);
    int (*ndo_stop)(struct net_device *);
    netdev_tx_t (*ndo_start_xmit)(struct sk_buff *, struct net_device *);
    netdev_features_t (*ndo_features_check)(struct sk_buff *, struct net_device *, netdev_features_t);
    u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, struct net_device *);
    void (*ndo_change_rx_flags)(struct net_device *, int);
    void (*ndo_set_rx_mode)(struct net_device *);
    int (*ndo_set_mac_address)(struct net_device *, void *);
    int (*ndo_validate_addr)(struct net_device *);
    int (*ndo_do_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_set_config)(struct net_device *, struct ifmap *);
    int (*ndo_change_mtu)(struct net_device *, int);
    int (*ndo_neigh_setup)(struct net_device *, struct neigh_parms *);
    void (*ndo_tx_timeout)(struct net_device *);
    void (*ndo_get_stats64)(struct net_device *, struct rtnl_link_stats64 *);
    bool (*ndo_has_offload_stats)(const struct net_device *, int);
    int (*ndo_get_offload_stats)(int, const struct net_device *, void *);
    struct net_device_stats * (*ndo_get_stats)(struct net_device *);
    int (*ndo_vlan_rx_add_vid)(struct net_device *, __be16, u16);
    int (*ndo_vlan_rx_kill_vid)(struct net_device *, __be16, u16);
    void (*ndo_poll_controller)(struct net_device *);
    int (*ndo_netpoll_setup)(struct net_device *, struct netpoll_info *);
    void (*ndo_netpoll_cleanup)(struct net_device *);
    int (*ndo_set_vf_mac)(struct net_device *, int, u8 *);
    int (*ndo_set_vf_vlan)(struct net_device *, int, u16, u8, __be16);
    int (*ndo_set_vf_rate)(struct net_device *, int, int, int);
    int (*ndo_set_vf_spoofchk)(struct net_device *, int, bool);
    int (*ndo_set_vf_trust)(struct net_device *, int, bool);
    int (*ndo_get_vf_config)(struct net_device *, int, struct ifla_vf_info *);
    int (*ndo_set_vf_link_state)(struct net_device *, int, int);
    int (*ndo_get_vf_stats)(struct net_device *, int, struct ifla_vf_stats *);
    int (*ndo_set_vf_port)(struct net_device *, int, struct nlattr **);
    int (*ndo_get_vf_port)(struct net_device *, int, struct sk_buff *);
    int (*ndo_set_vf_guid)(struct net_device *, int, u64, int);
    int (*ndo_set_vf_rss_query_en)(struct net_device *, int, bool);
    int (*ndo_setup_tc)(struct net_device *, enum tc_setup_type, void *);
    int (*ndo_fcoe_enable)(struct net_device *);
    int (*ndo_fcoe_disable)(struct net_device *);
    int (*ndo_fcoe_ddp_setup)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_ddp_done)(struct net_device *, u16);
    int (*ndo_fcoe_ddp_target)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_get_hbainfo)(struct net_device *, struct netdev_fcoe_hbainfo *);
    int (*ndo_fcoe_get_wwn)(struct net_device *, u64 *, int);
    int (*ndo_rx_flow_steer)(struct net_device *, const struct sk_buff *, u16, u32);
    int (*ndo_add_slave)(struct net_device *, struct net_device *, struct netlink_ext_ack *);
    int (*ndo_del_slave)(struct net_device *, struct net_device *);
    netdev_features_t (*ndo_fix_features)(struct net_device *, netdev_features_t);
    int (*ndo_set_features)(struct net_device *, netdev_features_t);
    int (*ndo_neigh_construct)(struct net_device *, struct neighbour *);
    void (*ndo_neigh_destroy)(struct net_device *, struct neighbour *);
    int (*ndo_fdb_add)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, u16, struct netlink_ext_ack *);
    int (*ndo_fdb_del)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16);
    int (*ndo_fdb_dump)(struct sk_buff *, struct netlink_callback *, struct net_device *, struct net_device *, int *);
    int (*ndo_fdb_get)(struct sk_buff *, struct nlattr **, struct net_device *, const unsigned char *, u16, u32, u32, struct netlink_ext_ack *);
    int (*ndo_bridge_setlink)(struct net_device *, struct nlmsghdr *, u16, struct netlink_ext_ack *);
    int (*ndo_bridge_getlink)(struct sk_buff *, u32, u32, struct net_device *, u32, int);
    int (*ndo_bridge_dellink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_change_carrier)(struct net_device *, bool);
    int (*ndo_get_phys_port_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_port_parent_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_phys_port_name)(struct net_device *, char *, size_t);
    void (*ndo_udp_tunnel_add)(struct net_device *, struct udp_tunnel_info *);
    void (*ndo_udp_tunnel_del)(struct net_device *, struct udp_tunnel_info *);
    void * (*ndo_dfwd_add_station)(struct net_device *, struct net_device *);
    void (*ndo_dfwd_del_station)(struct net_device *, void *);
    int (*ndo_get_lock_subclass)(struct net_device *);
    int (*ndo_set_tx_maxrate)(struct net_device *, int, u32);
    int (*ndo_get_iflink)(const struct net_device *);
    int (*ndo_change_proto_down)(struct net_device *, bool);
    int (*ndo_fill_metadata_dst)(struct net_device *, struct sk_buff *);
    void (*ndo_set_rx_headroom)(struct net_device *, int);
    int (*ndo_bpf)(struct net_device *, struct netdev_bpf *);
    int (*ndo_xdp_xmit)(struct net_device *, int, struct xdp_frame **, u32);
    int (*ndo_xsk_async_xmit)(struct net_device *, u32);
    struct devlink_port * (*ndo_get_devlink_port)(struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct net_device_ops {
    int (*ndo_init)(struct net_device *);
    void (*ndo_uninit)(struct net_device *);
    int (*ndo_open)(struct net_device *);
    int (*ndo_stop)(struct net_device *);
    netdev_tx_t (*ndo_start_xmit)(struct sk_buff *, struct net_device *);
    netdev_features_t (*ndo_features_check)(struct sk_buff *, struct net_device *, netdev_features_t);
    u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, struct net_device *);
    void (*ndo_change_rx_flags)(struct net_device *, int);
    void (*ndo_set_rx_mode)(struct net_device *);
    int (*ndo_set_mac_address)(struct net_device *, void *);
    int (*ndo_validate_addr)(struct net_device *);
    int (*ndo_do_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_set_config)(struct net_device *, struct ifmap *);
    int (*ndo_change_mtu)(struct net_device *, int);
    int (*ndo_neigh_setup)(struct net_device *, struct neigh_parms *);
    void (*ndo_tx_timeout)(struct net_device *);
    void (*ndo_get_stats64)(struct net_device *, struct rtnl_link_stats64 *);
    bool (*ndo_has_offload_stats)(const struct net_device *, int);
    int (*ndo_get_offload_stats)(int, const struct net_device *, void *);
    struct net_device_stats * (*ndo_get_stats)(struct net_device *);
    int (*ndo_vlan_rx_add_vid)(struct net_device *, __be16, u16);
    int (*ndo_vlan_rx_kill_vid)(struct net_device *, __be16, u16);
    void (*ndo_poll_controller)(struct net_device *);
    int (*ndo_netpoll_setup)(struct net_device *, struct netpoll_info *);
    void (*ndo_netpoll_cleanup)(struct net_device *);
    int (*ndo_set_vf_mac)(struct net_device *, int, u8 *);
    int (*ndo_set_vf_vlan)(struct net_device *, int, u16, u8, __be16);
    int (*ndo_set_vf_rate)(struct net_device *, int, int, int);
    int (*ndo_set_vf_spoofchk)(struct net_device *, int, bool);
    int (*ndo_set_vf_trust)(struct net_device *, int, bool);
    int (*ndo_get_vf_config)(struct net_device *, int, struct ifla_vf_info *);
    int (*ndo_set_vf_link_state)(struct net_device *, int, int);
    int (*ndo_get_vf_stats)(struct net_device *, int, struct ifla_vf_stats *);
    int (*ndo_set_vf_port)(struct net_device *, int, struct nlattr **);
    int (*ndo_get_vf_port)(struct net_device *, int, struct sk_buff *);
    int (*ndo_set_vf_guid)(struct net_device *, int, u64, int);
    int (*ndo_set_vf_rss_query_en)(struct net_device *, int, bool);
    int (*ndo_setup_tc)(struct net_device *, enum tc_setup_type, void *);
    int (*ndo_fcoe_enable)(struct net_device *);
    int (*ndo_fcoe_disable)(struct net_device *);
    int (*ndo_fcoe_ddp_setup)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_ddp_done)(struct net_device *, u16);
    int (*ndo_fcoe_ddp_target)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_get_hbainfo)(struct net_device *, struct netdev_fcoe_hbainfo *);
    int (*ndo_fcoe_get_wwn)(struct net_device *, u64 *, int);
    int (*ndo_rx_flow_steer)(struct net_device *, const struct sk_buff *, u16, u32);
    int (*ndo_add_slave)(struct net_device *, struct net_device *, struct netlink_ext_ack *);
    int (*ndo_del_slave)(struct net_device *, struct net_device *);
    netdev_features_t (*ndo_fix_features)(struct net_device *, netdev_features_t);
    int (*ndo_set_features)(struct net_device *, netdev_features_t);
    int (*ndo_neigh_construct)(struct net_device *, struct neighbour *);
    void (*ndo_neigh_destroy)(struct net_device *, struct neighbour *);
    int (*ndo_fdb_add)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, u16, struct netlink_ext_ack *);
    int (*ndo_fdb_del)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16);
    int (*ndo_fdb_dump)(struct sk_buff *, struct netlink_callback *, struct net_device *, struct net_device *, int *);
    int (*ndo_fdb_get)(struct sk_buff *, struct nlattr **, struct net_device *, const unsigned char *, u16, u32, u32, struct netlink_ext_ack *);
    int (*ndo_bridge_setlink)(struct net_device *, struct nlmsghdr *, u16, struct netlink_ext_ack *);
    int (*ndo_bridge_getlink)(struct sk_buff *, u32, u32, struct net_device *, u32, int);
    int (*ndo_bridge_dellink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_change_carrier)(struct net_device *, bool);
    int (*ndo_get_phys_port_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_port_parent_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_phys_port_name)(struct net_device *, char *, size_t);
    void (*ndo_udp_tunnel_add)(struct net_device *, struct udp_tunnel_info *);
    void (*ndo_udp_tunnel_del)(struct net_device *, struct udp_tunnel_info *);
    void * (*ndo_dfwd_add_station)(struct net_device *, struct net_device *);
    void (*ndo_dfwd_del_station)(struct net_device *, void *);
    int (*ndo_set_tx_maxrate)(struct net_device *, int, u32);
    int (*ndo_get_iflink)(const struct net_device *);
    int (*ndo_change_proto_down)(struct net_device *, bool);
    int (*ndo_fill_metadata_dst)(struct net_device *, struct sk_buff *);
    void (*ndo_set_rx_headroom)(struct net_device *, int);
    int (*ndo_bpf)(struct net_device *, struct netdev_bpf *);
    int (*ndo_xdp_xmit)(struct net_device *, int, struct xdp_frame **, u32);
    int (*ndo_xsk_wakeup)(struct net_device *, u32, u32);
    struct devlink_port * (*ndo_get_devlink_port)(struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct net_device_ops {
    int (*ndo_init)(struct net_device *);
    void (*ndo_uninit)(struct net_device *);
    int (*ndo_open)(struct net_device *);
    int (*ndo_stop)(struct net_device *);
    netdev_tx_t (*ndo_start_xmit)(struct sk_buff *, struct net_device *);
    netdev_features_t (*ndo_features_check)(struct sk_buff *, struct net_device *, netdev_features_t);
    u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, struct net_device *);
    void (*ndo_change_rx_flags)(struct net_device *, int);
    void (*ndo_set_rx_mode)(struct net_device *);
    int (*ndo_set_mac_address)(struct net_device *, void *);
    int (*ndo_validate_addr)(struct net_device *);
    int (*ndo_do_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_set_config)(struct net_device *, struct ifmap *);
    int (*ndo_change_mtu)(struct net_device *, int);
    int (*ndo_neigh_setup)(struct net_device *, struct neigh_parms *);
    void (*ndo_tx_timeout)(struct net_device *, unsigned int);
    void (*ndo_get_stats64)(struct net_device *, struct rtnl_link_stats64 *);
    bool (*ndo_has_offload_stats)(const struct net_device *, int);
    int (*ndo_get_offload_stats)(int, const struct net_device *, void *);
    struct net_device_stats * (*ndo_get_stats)(struct net_device *);
    int (*ndo_vlan_rx_add_vid)(struct net_device *, __be16, u16);
    int (*ndo_vlan_rx_kill_vid)(struct net_device *, __be16, u16);
    void (*ndo_poll_controller)(struct net_device *);
    int (*ndo_netpoll_setup)(struct net_device *, struct netpoll_info *);
    void (*ndo_netpoll_cleanup)(struct net_device *);
    int (*ndo_set_vf_mac)(struct net_device *, int, u8 *);
    int (*ndo_set_vf_vlan)(struct net_device *, int, u16, u8, __be16);
    int (*ndo_set_vf_rate)(struct net_device *, int, int, int);
    int (*ndo_set_vf_spoofchk)(struct net_device *, int, bool);
    int (*ndo_set_vf_trust)(struct net_device *, int, bool);
    int (*ndo_get_vf_config)(struct net_device *, int, struct ifla_vf_info *);
    int (*ndo_set_vf_link_state)(struct net_device *, int, int);
    int (*ndo_get_vf_stats)(struct net_device *, int, struct ifla_vf_stats *);
    int (*ndo_set_vf_port)(struct net_device *, int, struct nlattr **);
    int (*ndo_get_vf_port)(struct net_device *, int, struct sk_buff *);
    int (*ndo_get_vf_guid)(struct net_device *, int, struct ifla_vf_guid *, struct ifla_vf_guid *);
    int (*ndo_set_vf_guid)(struct net_device *, int, u64, int);
    int (*ndo_set_vf_rss_query_en)(struct net_device *, int, bool);
    int (*ndo_setup_tc)(struct net_device *, enum tc_setup_type, void *);
    int (*ndo_fcoe_enable)(struct net_device *);
    int (*ndo_fcoe_disable)(struct net_device *);
    int (*ndo_fcoe_ddp_setup)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_ddp_done)(struct net_device *, u16);
    int (*ndo_fcoe_ddp_target)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_get_hbainfo)(struct net_device *, struct netdev_fcoe_hbainfo *);
    int (*ndo_fcoe_get_wwn)(struct net_device *, u64 *, int);
    int (*ndo_rx_flow_steer)(struct net_device *, const struct sk_buff *, u16, u32);
    int (*ndo_add_slave)(struct net_device *, struct net_device *, struct netlink_ext_ack *);
    int (*ndo_del_slave)(struct net_device *, struct net_device *);
    struct net_device * (*ndo_get_xmit_slave)(struct net_device *, struct sk_buff *, bool);
    netdev_features_t (*ndo_fix_features)(struct net_device *, netdev_features_t);
    int (*ndo_set_features)(struct net_device *, netdev_features_t);
    int (*ndo_neigh_construct)(struct net_device *, struct neighbour *);
    void (*ndo_neigh_destroy)(struct net_device *, struct neighbour *);
    int (*ndo_fdb_add)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, u16, struct netlink_ext_ack *);
    int (*ndo_fdb_del)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16);
    int (*ndo_fdb_dump)(struct sk_buff *, struct netlink_callback *, struct net_device *, struct net_device *, int *);
    int (*ndo_fdb_get)(struct sk_buff *, struct nlattr **, struct net_device *, const unsigned char *, u16, u32, u32, struct netlink_ext_ack *);
    int (*ndo_bridge_setlink)(struct net_device *, struct nlmsghdr *, u16, struct netlink_ext_ack *);
    int (*ndo_bridge_getlink)(struct sk_buff *, u32, u32, struct net_device *, u32, int);
    int (*ndo_bridge_dellink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_change_carrier)(struct net_device *, bool);
    int (*ndo_get_phys_port_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_port_parent_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_phys_port_name)(struct net_device *, char *, size_t);
    void (*ndo_udp_tunnel_add)(struct net_device *, struct udp_tunnel_info *);
    void (*ndo_udp_tunnel_del)(struct net_device *, struct udp_tunnel_info *);
    void * (*ndo_dfwd_add_station)(struct net_device *, struct net_device *);
    void (*ndo_dfwd_del_station)(struct net_device *, void *);
    int (*ndo_set_tx_maxrate)(struct net_device *, int, u32);
    int (*ndo_get_iflink)(const struct net_device *);
    int (*ndo_change_proto_down)(struct net_device *, bool);
    int (*ndo_fill_metadata_dst)(struct net_device *, struct sk_buff *);
    void (*ndo_set_rx_headroom)(struct net_device *, int);
    int (*ndo_bpf)(struct net_device *, struct netdev_bpf *);
    int (*ndo_xdp_xmit)(struct net_device *, int, struct xdp_frame **, u32);
    int (*ndo_xsk_wakeup)(struct net_device *, u32, u32);
    struct devlink_port * (*ndo_get_devlink_port)(struct net_device *);
    int (*ndo_tunnel_ctl)(struct net_device *, struct ip_tunnel_parm *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct net_device_ops {
    int (*ndo_init)(struct net_device *);
    void (*ndo_uninit)(struct net_device *);
    int (*ndo_open)(struct net_device *);
    int (*ndo_stop)(struct net_device *);
    netdev_tx_t (*ndo_start_xmit)(struct sk_buff *, struct net_device *);
    netdev_features_t (*ndo_features_check)(struct sk_buff *, struct net_device *, netdev_features_t);
    u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, struct net_device *);
    void (*ndo_change_rx_flags)(struct net_device *, int);
    void (*ndo_set_rx_mode)(struct net_device *);
    int (*ndo_set_mac_address)(struct net_device *, void *);
    int (*ndo_validate_addr)(struct net_device *);
    int (*ndo_do_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_set_config)(struct net_device *, struct ifmap *);
    int (*ndo_change_mtu)(struct net_device *, int);
    int (*ndo_neigh_setup)(struct net_device *, struct neigh_parms *);
    void (*ndo_tx_timeout)(struct net_device *, unsigned int);
    void (*ndo_get_stats64)(struct net_device *, struct rtnl_link_stats64 *);
    bool (*ndo_has_offload_stats)(const struct net_device *, int);
    int (*ndo_get_offload_stats)(int, const struct net_device *, void *);
    struct net_device_stats * (*ndo_get_stats)(struct net_device *);
    int (*ndo_vlan_rx_add_vid)(struct net_device *, __be16, u16);
    int (*ndo_vlan_rx_kill_vid)(struct net_device *, __be16, u16);
    void (*ndo_poll_controller)(struct net_device *);
    int (*ndo_netpoll_setup)(struct net_device *, struct netpoll_info *);
    void (*ndo_netpoll_cleanup)(struct net_device *);
    int (*ndo_set_vf_mac)(struct net_device *, int, u8 *);
    int (*ndo_set_vf_vlan)(struct net_device *, int, u16, u8, __be16);
    int (*ndo_set_vf_rate)(struct net_device *, int, int, int);
    int (*ndo_set_vf_spoofchk)(struct net_device *, int, bool);
    int (*ndo_set_vf_trust)(struct net_device *, int, bool);
    int (*ndo_get_vf_config)(struct net_device *, int, struct ifla_vf_info *);
    int (*ndo_set_vf_link_state)(struct net_device *, int, int);
    int (*ndo_get_vf_stats)(struct net_device *, int, struct ifla_vf_stats *);
    int (*ndo_set_vf_port)(struct net_device *, int, struct nlattr **);
    int (*ndo_get_vf_port)(struct net_device *, int, struct sk_buff *);
    int (*ndo_get_vf_guid)(struct net_device *, int, struct ifla_vf_guid *, struct ifla_vf_guid *);
    int (*ndo_set_vf_guid)(struct net_device *, int, u64, int);
    int (*ndo_set_vf_rss_query_en)(struct net_device *, int, bool);
    int (*ndo_setup_tc)(struct net_device *, enum tc_setup_type, void *);
    int (*ndo_fcoe_enable)(struct net_device *);
    int (*ndo_fcoe_disable)(struct net_device *);
    int (*ndo_fcoe_ddp_setup)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_ddp_done)(struct net_device *, u16);
    int (*ndo_fcoe_ddp_target)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_get_hbainfo)(struct net_device *, struct netdev_fcoe_hbainfo *);
    int (*ndo_fcoe_get_wwn)(struct net_device *, u64 *, int);
    int (*ndo_rx_flow_steer)(struct net_device *, const struct sk_buff *, u16, u32);
    int (*ndo_add_slave)(struct net_device *, struct net_device *, struct netlink_ext_ack *);
    int (*ndo_del_slave)(struct net_device *, struct net_device *);
    struct net_device * (*ndo_get_xmit_slave)(struct net_device *, struct sk_buff *, bool);
    struct net_device * (*ndo_sk_get_lower_dev)(struct net_device *, struct sock *);
    netdev_features_t (*ndo_fix_features)(struct net_device *, netdev_features_t);
    int (*ndo_set_features)(struct net_device *, netdev_features_t);
    int (*ndo_neigh_construct)(struct net_device *, struct neighbour *);
    void (*ndo_neigh_destroy)(struct net_device *, struct neighbour *);
    int (*ndo_fdb_add)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, u16, struct netlink_ext_ack *);
    int (*ndo_fdb_del)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16);
    int (*ndo_fdb_dump)(struct sk_buff *, struct netlink_callback *, struct net_device *, struct net_device *, int *);
    int (*ndo_fdb_get)(struct sk_buff *, struct nlattr **, struct net_device *, const unsigned char *, u16, u32, u32, struct netlink_ext_ack *);
    int (*ndo_bridge_setlink)(struct net_device *, struct nlmsghdr *, u16, struct netlink_ext_ack *);
    int (*ndo_bridge_getlink)(struct sk_buff *, u32, u32, struct net_device *, u32, int);
    int (*ndo_bridge_dellink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_change_carrier)(struct net_device *, bool);
    int (*ndo_get_phys_port_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_port_parent_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_phys_port_name)(struct net_device *, char *, size_t);
    void (*ndo_udp_tunnel_add)(struct net_device *, struct udp_tunnel_info *);
    void (*ndo_udp_tunnel_del)(struct net_device *, struct udp_tunnel_info *);
    void * (*ndo_dfwd_add_station)(struct net_device *, struct net_device *);
    void (*ndo_dfwd_del_station)(struct net_device *, void *);
    int (*ndo_set_tx_maxrate)(struct net_device *, int, u32);
    int (*ndo_get_iflink)(const struct net_device *);
    int (*ndo_change_proto_down)(struct net_device *, bool);
    int (*ndo_fill_metadata_dst)(struct net_device *, struct sk_buff *);
    void (*ndo_set_rx_headroom)(struct net_device *, int);
    int (*ndo_bpf)(struct net_device *, struct netdev_bpf *);
    int (*ndo_xdp_xmit)(struct net_device *, int, struct xdp_frame **, u32);
    int (*ndo_xsk_wakeup)(struct net_device *, u32, u32);
    struct devlink_port * (*ndo_get_devlink_port)(struct net_device *);
    int (*ndo_tunnel_ctl)(struct net_device *, struct ip_tunnel_parm *, int);
    struct net_device * (*ndo_get_peer_dev)(struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct net_device_ops {
    int (*ndo_init)(struct net_device *);
    void (*ndo_uninit)(struct net_device *);
    int (*ndo_open)(struct net_device *);
    int (*ndo_stop)(struct net_device *);
    netdev_tx_t (*ndo_start_xmit)(struct sk_buff *, struct net_device *);
    netdev_features_t (*ndo_features_check)(struct sk_buff *, struct net_device *, netdev_features_t);
    u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, struct net_device *);
    void (*ndo_change_rx_flags)(struct net_device *, int);
    void (*ndo_set_rx_mode)(struct net_device *);
    int (*ndo_set_mac_address)(struct net_device *, void *);
    int (*ndo_validate_addr)(struct net_device *);
    int (*ndo_do_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_set_config)(struct net_device *, struct ifmap *);
    int (*ndo_change_mtu)(struct net_device *, int);
    int (*ndo_neigh_setup)(struct net_device *, struct neigh_parms *);
    void (*ndo_tx_timeout)(struct net_device *, unsigned int);
    void (*ndo_get_stats64)(struct net_device *, struct rtnl_link_stats64 *);
    bool (*ndo_has_offload_stats)(const struct net_device *, int);
    int (*ndo_get_offload_stats)(int, const struct net_device *, void *);
    struct net_device_stats * (*ndo_get_stats)(struct net_device *);
    int (*ndo_vlan_rx_add_vid)(struct net_device *, __be16, u16);
    int (*ndo_vlan_rx_kill_vid)(struct net_device *, __be16, u16);
    void (*ndo_poll_controller)(struct net_device *);
    int (*ndo_netpoll_setup)(struct net_device *, struct netpoll_info *);
    void (*ndo_netpoll_cleanup)(struct net_device *);
    int (*ndo_set_vf_mac)(struct net_device *, int, u8 *);
    int (*ndo_set_vf_vlan)(struct net_device *, int, u16, u8, __be16);
    int (*ndo_set_vf_rate)(struct net_device *, int, int, int);
    int (*ndo_set_vf_spoofchk)(struct net_device *, int, bool);
    int (*ndo_set_vf_trust)(struct net_device *, int, bool);
    int (*ndo_get_vf_config)(struct net_device *, int, struct ifla_vf_info *);
    int (*ndo_set_vf_link_state)(struct net_device *, int, int);
    int (*ndo_get_vf_stats)(struct net_device *, int, struct ifla_vf_stats *);
    int (*ndo_set_vf_port)(struct net_device *, int, struct nlattr **);
    int (*ndo_get_vf_port)(struct net_device *, int, struct sk_buff *);
    int (*ndo_get_vf_guid)(struct net_device *, int, struct ifla_vf_guid *, struct ifla_vf_guid *);
    int (*ndo_set_vf_guid)(struct net_device *, int, u64, int);
    int (*ndo_set_vf_rss_query_en)(struct net_device *, int, bool);
    int (*ndo_setup_tc)(struct net_device *, enum tc_setup_type, void *);
    int (*ndo_fcoe_enable)(struct net_device *);
    int (*ndo_fcoe_disable)(struct net_device *);
    int (*ndo_fcoe_ddp_setup)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_ddp_done)(struct net_device *, u16);
    int (*ndo_fcoe_ddp_target)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_get_hbainfo)(struct net_device *, struct netdev_fcoe_hbainfo *);
    int (*ndo_fcoe_get_wwn)(struct net_device *, u64 *, int);
    int (*ndo_rx_flow_steer)(struct net_device *, const struct sk_buff *, u16, u32);
    int (*ndo_add_slave)(struct net_device *, struct net_device *, struct netlink_ext_ack *);
    int (*ndo_del_slave)(struct net_device *, struct net_device *);
    struct net_device * (*ndo_get_xmit_slave)(struct net_device *, struct sk_buff *, bool);
    struct net_device * (*ndo_sk_get_lower_dev)(struct net_device *, struct sock *);
    netdev_features_t (*ndo_fix_features)(struct net_device *, netdev_features_t);
    int (*ndo_set_features)(struct net_device *, netdev_features_t);
    int (*ndo_neigh_construct)(struct net_device *, struct neighbour *);
    void (*ndo_neigh_destroy)(struct net_device *, struct neighbour *);
    int (*ndo_fdb_add)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, u16, struct netlink_ext_ack *);
    int (*ndo_fdb_del)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16);
    int (*ndo_fdb_dump)(struct sk_buff *, struct netlink_callback *, struct net_device *, struct net_device *, int *);
    int (*ndo_fdb_get)(struct sk_buff *, struct nlattr **, struct net_device *, const unsigned char *, u16, u32, u32, struct netlink_ext_ack *);
    int (*ndo_bridge_setlink)(struct net_device *, struct nlmsghdr *, u16, struct netlink_ext_ack *);
    int (*ndo_bridge_getlink)(struct sk_buff *, u32, u32, struct net_device *, u32, int);
    int (*ndo_bridge_dellink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_change_carrier)(struct net_device *, bool);
    int (*ndo_get_phys_port_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_port_parent_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_phys_port_name)(struct net_device *, char *, size_t);
    void * (*ndo_dfwd_add_station)(struct net_device *, struct net_device *);
    void (*ndo_dfwd_del_station)(struct net_device *, void *);
    int (*ndo_set_tx_maxrate)(struct net_device *, int, u32);
    int (*ndo_get_iflink)(const struct net_device *);
    int (*ndo_change_proto_down)(struct net_device *, bool);
    int (*ndo_fill_metadata_dst)(struct net_device *, struct sk_buff *);
    void (*ndo_set_rx_headroom)(struct net_device *, int);
    int (*ndo_bpf)(struct net_device *, struct netdev_bpf *);
    int (*ndo_xdp_xmit)(struct net_device *, int, struct xdp_frame **, u32);
    int (*ndo_xsk_wakeup)(struct net_device *, u32, u32);
    struct devlink_port * (*ndo_get_devlink_port)(struct net_device *);
    int (*ndo_tunnel_ctl)(struct net_device *, struct ip_tunnel_parm *, int);
    struct net_device * (*ndo_get_peer_dev)(struct net_device *);
    int (*ndo_fill_forward_path)(struct net_device_path_ctx *, struct net_device_path *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct net_device_ops {
    int (*ndo_init)(struct net_device *);
    void (*ndo_uninit)(struct net_device *);
    int (*ndo_open)(struct net_device *);
    int (*ndo_stop)(struct net_device *);
    netdev_tx_t (*ndo_start_xmit)(struct sk_buff *, struct net_device *);
    netdev_features_t (*ndo_features_check)(struct sk_buff *, struct net_device *, netdev_features_t);
    u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, struct net_device *);
    void (*ndo_change_rx_flags)(struct net_device *, int);
    void (*ndo_set_rx_mode)(struct net_device *);
    int (*ndo_set_mac_address)(struct net_device *, void *);
    int (*ndo_validate_addr)(struct net_device *);
    int (*ndo_do_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_eth_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_siocbond)(struct net_device *, struct ifreq *, int);
    int (*ndo_siocwandev)(struct net_device *, struct if_settings *);
    int (*ndo_siocdevprivate)(struct net_device *, struct ifreq *, void *, int);
    int (*ndo_set_config)(struct net_device *, struct ifmap *);
    int (*ndo_change_mtu)(struct net_device *, int);
    int (*ndo_neigh_setup)(struct net_device *, struct neigh_parms *);
    void (*ndo_tx_timeout)(struct net_device *, unsigned int);
    void (*ndo_get_stats64)(struct net_device *, struct rtnl_link_stats64 *);
    bool (*ndo_has_offload_stats)(const struct net_device *, int);
    int (*ndo_get_offload_stats)(int, const struct net_device *, void *);
    struct net_device_stats * (*ndo_get_stats)(struct net_device *);
    int (*ndo_vlan_rx_add_vid)(struct net_device *, __be16, u16);
    int (*ndo_vlan_rx_kill_vid)(struct net_device *, __be16, u16);
    void (*ndo_poll_controller)(struct net_device *);
    int (*ndo_netpoll_setup)(struct net_device *, struct netpoll_info *);
    void (*ndo_netpoll_cleanup)(struct net_device *);
    int (*ndo_set_vf_mac)(struct net_device *, int, u8 *);
    int (*ndo_set_vf_vlan)(struct net_device *, int, u16, u8, __be16);
    int (*ndo_set_vf_rate)(struct net_device *, int, int, int);
    int (*ndo_set_vf_spoofchk)(struct net_device *, int, bool);
    int (*ndo_set_vf_trust)(struct net_device *, int, bool);
    int (*ndo_get_vf_config)(struct net_device *, int, struct ifla_vf_info *);
    int (*ndo_set_vf_link_state)(struct net_device *, int, int);
    int (*ndo_get_vf_stats)(struct net_device *, int, struct ifla_vf_stats *);
    int (*ndo_set_vf_port)(struct net_device *, int, struct nlattr **);
    int (*ndo_get_vf_port)(struct net_device *, int, struct sk_buff *);
    int (*ndo_get_vf_guid)(struct net_device *, int, struct ifla_vf_guid *, struct ifla_vf_guid *);
    int (*ndo_set_vf_guid)(struct net_device *, int, u64, int);
    int (*ndo_set_vf_rss_query_en)(struct net_device *, int, bool);
    int (*ndo_setup_tc)(struct net_device *, enum tc_setup_type, void *);
    int (*ndo_fcoe_enable)(struct net_device *);
    int (*ndo_fcoe_disable)(struct net_device *);
    int (*ndo_fcoe_ddp_setup)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_ddp_done)(struct net_device *, u16);
    int (*ndo_fcoe_ddp_target)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_get_hbainfo)(struct net_device *, struct netdev_fcoe_hbainfo *);
    int (*ndo_fcoe_get_wwn)(struct net_device *, u64 *, int);
    int (*ndo_rx_flow_steer)(struct net_device *, const struct sk_buff *, u16, u32);
    int (*ndo_add_slave)(struct net_device *, struct net_device *, struct netlink_ext_ack *);
    int (*ndo_del_slave)(struct net_device *, struct net_device *);
    struct net_device * (*ndo_get_xmit_slave)(struct net_device *, struct sk_buff *, bool);
    struct net_device * (*ndo_sk_get_lower_dev)(struct net_device *, struct sock *);
    netdev_features_t (*ndo_fix_features)(struct net_device *, netdev_features_t);
    int (*ndo_set_features)(struct net_device *, netdev_features_t);
    int (*ndo_neigh_construct)(struct net_device *, struct neighbour *);
    void (*ndo_neigh_destroy)(struct net_device *, struct neighbour *);
    int (*ndo_fdb_add)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, u16, struct netlink_ext_ack *);
    int (*ndo_fdb_del)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16);
    int (*ndo_fdb_dump)(struct sk_buff *, struct netlink_callback *, struct net_device *, struct net_device *, int *);
    int (*ndo_fdb_get)(struct sk_buff *, struct nlattr **, struct net_device *, const unsigned char *, u16, u32, u32, struct netlink_ext_ack *);
    int (*ndo_bridge_setlink)(struct net_device *, struct nlmsghdr *, u16, struct netlink_ext_ack *);
    int (*ndo_bridge_getlink)(struct sk_buff *, u32, u32, struct net_device *, u32, int);
    int (*ndo_bridge_dellink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_change_carrier)(struct net_device *, bool);
    int (*ndo_get_phys_port_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_port_parent_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_phys_port_name)(struct net_device *, char *, size_t);
    void * (*ndo_dfwd_add_station)(struct net_device *, struct net_device *);
    void (*ndo_dfwd_del_station)(struct net_device *, void *);
    int (*ndo_set_tx_maxrate)(struct net_device *, int, u32);
    int (*ndo_get_iflink)(const struct net_device *);
    int (*ndo_change_proto_down)(struct net_device *, bool);
    int (*ndo_fill_metadata_dst)(struct net_device *, struct sk_buff *);
    void (*ndo_set_rx_headroom)(struct net_device *, int);
    int (*ndo_bpf)(struct net_device *, struct netdev_bpf *);
    int (*ndo_xdp_xmit)(struct net_device *, int, struct xdp_frame **, u32);
    struct net_device * (*ndo_xdp_get_xmit_slave)(struct net_device *, struct xdp_buff *);
    int (*ndo_xsk_wakeup)(struct net_device *, u32, u32);
    struct devlink_port * (*ndo_get_devlink_port)(struct net_device *);
    int (*ndo_tunnel_ctl)(struct net_device *, struct ip_tunnel_parm *, int);
    struct net_device * (*ndo_get_peer_dev)(struct net_device *);
    int (*ndo_fill_forward_path)(struct net_device_path_ctx *, struct net_device_path *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct net_device_ops {
    int (*ndo_init)(struct net_device *);
    void (*ndo_uninit)(struct net_device *);
    int (*ndo_open)(struct net_device *);
    int (*ndo_stop)(struct net_device *);
    netdev_tx_t (*ndo_start_xmit)(struct sk_buff *, struct net_device *);
    netdev_features_t (*ndo_features_check)(struct sk_buff *, struct net_device *, netdev_features_t);
    u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, struct net_device *);
    void (*ndo_change_rx_flags)(struct net_device *, int);
    void (*ndo_set_rx_mode)(struct net_device *);
    int (*ndo_set_mac_address)(struct net_device *, void *);
    int (*ndo_validate_addr)(struct net_device *);
    int (*ndo_do_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_eth_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_siocbond)(struct net_device *, struct ifreq *, int);
    int (*ndo_siocwandev)(struct net_device *, struct if_settings *);
    int (*ndo_siocdevprivate)(struct net_device *, struct ifreq *, void *, int);
    int (*ndo_set_config)(struct net_device *, struct ifmap *);
    int (*ndo_change_mtu)(struct net_device *, int);
    int (*ndo_neigh_setup)(struct net_device *, struct neigh_parms *);
    void (*ndo_tx_timeout)(struct net_device *, unsigned int);
    void (*ndo_get_stats64)(struct net_device *, struct rtnl_link_stats64 *);
    bool (*ndo_has_offload_stats)(const struct net_device *, int);
    int (*ndo_get_offload_stats)(int, const struct net_device *, void *);
    struct net_device_stats * (*ndo_get_stats)(struct net_device *);
    int (*ndo_vlan_rx_add_vid)(struct net_device *, __be16, u16);
    int (*ndo_vlan_rx_kill_vid)(struct net_device *, __be16, u16);
    void (*ndo_poll_controller)(struct net_device *);
    int (*ndo_netpoll_setup)(struct net_device *, struct netpoll_info *);
    void (*ndo_netpoll_cleanup)(struct net_device *);
    int (*ndo_set_vf_mac)(struct net_device *, int, u8 *);
    int (*ndo_set_vf_vlan)(struct net_device *, int, u16, u8, __be16);
    int (*ndo_set_vf_rate)(struct net_device *, int, int, int);
    int (*ndo_set_vf_spoofchk)(struct net_device *, int, bool);
    int (*ndo_set_vf_trust)(struct net_device *, int, bool);
    int (*ndo_get_vf_config)(struct net_device *, int, struct ifla_vf_info *);
    int (*ndo_set_vf_link_state)(struct net_device *, int, int);
    int (*ndo_get_vf_stats)(struct net_device *, int, struct ifla_vf_stats *);
    int (*ndo_set_vf_port)(struct net_device *, int, struct nlattr **);
    int (*ndo_get_vf_port)(struct net_device *, int, struct sk_buff *);
    int (*ndo_get_vf_guid)(struct net_device *, int, struct ifla_vf_guid *, struct ifla_vf_guid *);
    int (*ndo_set_vf_guid)(struct net_device *, int, u64, int);
    int (*ndo_set_vf_rss_query_en)(struct net_device *, int, bool);
    int (*ndo_setup_tc)(struct net_device *, enum tc_setup_type, void *);
    int (*ndo_fcoe_enable)(struct net_device *);
    int (*ndo_fcoe_disable)(struct net_device *);
    int (*ndo_fcoe_ddp_setup)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_ddp_done)(struct net_device *, u16);
    int (*ndo_fcoe_ddp_target)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_get_hbainfo)(struct net_device *, struct netdev_fcoe_hbainfo *);
    int (*ndo_fcoe_get_wwn)(struct net_device *, u64 *, int);
    int (*ndo_rx_flow_steer)(struct net_device *, const struct sk_buff *, u16, u32);
    int (*ndo_add_slave)(struct net_device *, struct net_device *, struct netlink_ext_ack *);
    int (*ndo_del_slave)(struct net_device *, struct net_device *);
    struct net_device * (*ndo_get_xmit_slave)(struct net_device *, struct sk_buff *, bool);
    struct net_device * (*ndo_sk_get_lower_dev)(struct net_device *, struct sock *);
    netdev_features_t (*ndo_fix_features)(struct net_device *, netdev_features_t);
    int (*ndo_set_features)(struct net_device *, netdev_features_t);
    int (*ndo_neigh_construct)(struct net_device *, struct neighbour *);
    void (*ndo_neigh_destroy)(struct net_device *, struct neighbour *);
    int (*ndo_fdb_add)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, u16, struct netlink_ext_ack *);
    int (*ndo_fdb_del)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, struct netlink_ext_ack *);
    int (*ndo_fdb_del_bulk)(struct ndmsg *, struct nlattr **, struct net_device *, u16, struct netlink_ext_ack *);
    int (*ndo_fdb_dump)(struct sk_buff *, struct netlink_callback *, struct net_device *, struct net_device *, int *);
    int (*ndo_fdb_get)(struct sk_buff *, struct nlattr **, struct net_device *, const unsigned char *, u16, u32, u32, struct netlink_ext_ack *);
    int (*ndo_bridge_setlink)(struct net_device *, struct nlmsghdr *, u16, struct netlink_ext_ack *);
    int (*ndo_bridge_getlink)(struct sk_buff *, u32, u32, struct net_device *, u32, int);
    int (*ndo_bridge_dellink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_change_carrier)(struct net_device *, bool);
    int (*ndo_get_phys_port_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_port_parent_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_phys_port_name)(struct net_device *, char *, size_t);
    void * (*ndo_dfwd_add_station)(struct net_device *, struct net_device *);
    void (*ndo_dfwd_del_station)(struct net_device *, void *);
    int (*ndo_set_tx_maxrate)(struct net_device *, int, u32);
    int (*ndo_get_iflink)(const struct net_device *);
    int (*ndo_fill_metadata_dst)(struct net_device *, struct sk_buff *);
    void (*ndo_set_rx_headroom)(struct net_device *, int);
    int (*ndo_bpf)(struct net_device *, struct netdev_bpf *);
    int (*ndo_xdp_xmit)(struct net_device *, int, struct xdp_frame **, u32);
    struct net_device * (*ndo_xdp_get_xmit_slave)(struct net_device *, struct xdp_buff *);
    int (*ndo_xsk_wakeup)(struct net_device *, u32, u32);
    struct devlink_port * (*ndo_get_devlink_port)(struct net_device *);
    int (*ndo_tunnel_ctl)(struct net_device *, struct ip_tunnel_parm *, int);
    struct net_device * (*ndo_get_peer_dev)(struct net_device *);
    int (*ndo_fill_forward_path)(struct net_device_path_ctx *, struct net_device_path *);
    ktime_t (*ndo_get_tstamp)(struct net_device *, const struct skb_shared_hwtstamps *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct net_device_ops {
    int (*ndo_init)(struct net_device *);
    void (*ndo_uninit)(struct net_device *);
    int (*ndo_open)(struct net_device *);
    int (*ndo_stop)(struct net_device *);
    netdev_tx_t (*ndo_start_xmit)(struct sk_buff *, struct net_device *);
    netdev_features_t (*ndo_features_check)(struct sk_buff *, struct net_device *, netdev_features_t);
    u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, struct net_device *);
    void (*ndo_change_rx_flags)(struct net_device *, int);
    void (*ndo_set_rx_mode)(struct net_device *);
    int (*ndo_set_mac_address)(struct net_device *, void *);
    int (*ndo_validate_addr)(struct net_device *);
    int (*ndo_do_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_eth_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_siocbond)(struct net_device *, struct ifreq *, int);
    int (*ndo_siocwandev)(struct net_device *, struct if_settings *);
    int (*ndo_siocdevprivate)(struct net_device *, struct ifreq *, void *, int);
    int (*ndo_set_config)(struct net_device *, struct ifmap *);
    int (*ndo_change_mtu)(struct net_device *, int);
    int (*ndo_neigh_setup)(struct net_device *, struct neigh_parms *);
    void (*ndo_tx_timeout)(struct net_device *, unsigned int);
    void (*ndo_get_stats64)(struct net_device *, struct rtnl_link_stats64 *);
    bool (*ndo_has_offload_stats)(const struct net_device *, int);
    int (*ndo_get_offload_stats)(int, const struct net_device *, void *);
    struct net_device_stats * (*ndo_get_stats)(struct net_device *);
    int (*ndo_vlan_rx_add_vid)(struct net_device *, __be16, u16);
    int (*ndo_vlan_rx_kill_vid)(struct net_device *, __be16, u16);
    void (*ndo_poll_controller)(struct net_device *);
    int (*ndo_netpoll_setup)(struct net_device *, struct netpoll_info *);
    void (*ndo_netpoll_cleanup)(struct net_device *);
    int (*ndo_set_vf_mac)(struct net_device *, int, u8 *);
    int (*ndo_set_vf_vlan)(struct net_device *, int, u16, u8, __be16);
    int (*ndo_set_vf_rate)(struct net_device *, int, int, int);
    int (*ndo_set_vf_spoofchk)(struct net_device *, int, bool);
    int (*ndo_set_vf_trust)(struct net_device *, int, bool);
    int (*ndo_get_vf_config)(struct net_device *, int, struct ifla_vf_info *);
    int (*ndo_set_vf_link_state)(struct net_device *, int, int);
    int (*ndo_get_vf_stats)(struct net_device *, int, struct ifla_vf_stats *);
    int (*ndo_set_vf_port)(struct net_device *, int, struct nlattr **);
    int (*ndo_get_vf_port)(struct net_device *, int, struct sk_buff *);
    int (*ndo_get_vf_guid)(struct net_device *, int, struct ifla_vf_guid *, struct ifla_vf_guid *);
    int (*ndo_set_vf_guid)(struct net_device *, int, u64, int);
    int (*ndo_set_vf_rss_query_en)(struct net_device *, int, bool);
    int (*ndo_setup_tc)(struct net_device *, enum tc_setup_type, void *);
    int (*ndo_fcoe_enable)(struct net_device *);
    int (*ndo_fcoe_disable)(struct net_device *);
    int (*ndo_fcoe_ddp_setup)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_ddp_done)(struct net_device *, u16);
    int (*ndo_fcoe_ddp_target)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_get_hbainfo)(struct net_device *, struct netdev_fcoe_hbainfo *);
    int (*ndo_fcoe_get_wwn)(struct net_device *, u64 *, int);
    int (*ndo_rx_flow_steer)(struct net_device *, const struct sk_buff *, u16, u32);
    int (*ndo_add_slave)(struct net_device *, struct net_device *, struct netlink_ext_ack *);
    int (*ndo_del_slave)(struct net_device *, struct net_device *);
    struct net_device * (*ndo_get_xmit_slave)(struct net_device *, struct sk_buff *, bool);
    struct net_device * (*ndo_sk_get_lower_dev)(struct net_device *, struct sock *);
    netdev_features_t (*ndo_fix_features)(struct net_device *, netdev_features_t);
    int (*ndo_set_features)(struct net_device *, netdev_features_t);
    int (*ndo_neigh_construct)(struct net_device *, struct neighbour *);
    void (*ndo_neigh_destroy)(struct net_device *, struct neighbour *);
    int (*ndo_fdb_add)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, u16, struct netlink_ext_ack *);
    int (*ndo_fdb_del)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, struct netlink_ext_ack *);
    int (*ndo_fdb_del_bulk)(struct ndmsg *, struct nlattr **, struct net_device *, u16, struct netlink_ext_ack *);
    int (*ndo_fdb_dump)(struct sk_buff *, struct netlink_callback *, struct net_device *, struct net_device *, int *);
    int (*ndo_fdb_get)(struct sk_buff *, struct nlattr **, struct net_device *, const unsigned char *, u16, u32, u32, struct netlink_ext_ack *);
    int (*ndo_bridge_setlink)(struct net_device *, struct nlmsghdr *, u16, struct netlink_ext_ack *);
    int (*ndo_bridge_getlink)(struct sk_buff *, u32, u32, struct net_device *, u32, int);
    int (*ndo_bridge_dellink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_change_carrier)(struct net_device *, bool);
    int (*ndo_get_phys_port_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_port_parent_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_phys_port_name)(struct net_device *, char *, size_t);
    void * (*ndo_dfwd_add_station)(struct net_device *, struct net_device *);
    void (*ndo_dfwd_del_station)(struct net_device *, void *);
    int (*ndo_set_tx_maxrate)(struct net_device *, int, u32);
    int (*ndo_get_iflink)(const struct net_device *);
    int (*ndo_fill_metadata_dst)(struct net_device *, struct sk_buff *);
    void (*ndo_set_rx_headroom)(struct net_device *, int);
    int (*ndo_bpf)(struct net_device *, struct netdev_bpf *);
    int (*ndo_xdp_xmit)(struct net_device *, int, struct xdp_frame **, u32);
    struct net_device * (*ndo_xdp_get_xmit_slave)(struct net_device *, struct xdp_buff *);
    int (*ndo_xsk_wakeup)(struct net_device *, u32, u32);
    int (*ndo_tunnel_ctl)(struct net_device *, struct ip_tunnel_parm *, int);
    struct net_device * (*ndo_get_peer_dev)(struct net_device *);
    int (*ndo_fill_forward_path)(struct net_device_path_ctx *, struct net_device_path *);
    ktime_t (*ndo_get_tstamp)(struct net_device *, const struct skb_shared_hwtstamps *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct net_device_ops {
    int (*ndo_init)(struct net_device *);
    void (*ndo_uninit)(struct net_device *);
    int (*ndo_open)(struct net_device *);
    int (*ndo_stop)(struct net_device *);
    netdev_tx_t (*ndo_start_xmit)(struct sk_buff *, struct net_device *);
    netdev_features_t (*ndo_features_check)(struct sk_buff *, struct net_device *, netdev_features_t);
    u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, struct net_device *);
    void (*ndo_change_rx_flags)(struct net_device *, int);
    void (*ndo_set_rx_mode)(struct net_device *);
    int (*ndo_set_mac_address)(struct net_device *, void *);
    int (*ndo_validate_addr)(struct net_device *);
    int (*ndo_do_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_eth_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_siocbond)(struct net_device *, struct ifreq *, int);
    int (*ndo_siocwandev)(struct net_device *, struct if_settings *);
    int (*ndo_siocdevprivate)(struct net_device *, struct ifreq *, void *, int);
    int (*ndo_set_config)(struct net_device *, struct ifmap *);
    int (*ndo_change_mtu)(struct net_device *, int);
    int (*ndo_neigh_setup)(struct net_device *, struct neigh_parms *);
    void (*ndo_tx_timeout)(struct net_device *, unsigned int);
    void (*ndo_get_stats64)(struct net_device *, struct rtnl_link_stats64 *);
    bool (*ndo_has_offload_stats)(const struct net_device *, int);
    int (*ndo_get_offload_stats)(int, const struct net_device *, void *);
    struct net_device_stats * (*ndo_get_stats)(struct net_device *);
    int (*ndo_vlan_rx_add_vid)(struct net_device *, __be16, u16);
    int (*ndo_vlan_rx_kill_vid)(struct net_device *, __be16, u16);
    void (*ndo_poll_controller)(struct net_device *);
    int (*ndo_netpoll_setup)(struct net_device *, struct netpoll_info *);
    void (*ndo_netpoll_cleanup)(struct net_device *);
    int (*ndo_set_vf_mac)(struct net_device *, int, u8 *);
    int (*ndo_set_vf_vlan)(struct net_device *, int, u16, u8, __be16);
    int (*ndo_set_vf_rate)(struct net_device *, int, int, int);
    int (*ndo_set_vf_spoofchk)(struct net_device *, int, bool);
    int (*ndo_set_vf_trust)(struct net_device *, int, bool);
    int (*ndo_get_vf_config)(struct net_device *, int, struct ifla_vf_info *);
    int (*ndo_set_vf_link_state)(struct net_device *, int, int);
    int (*ndo_get_vf_stats)(struct net_device *, int, struct ifla_vf_stats *);
    int (*ndo_set_vf_port)(struct net_device *, int, struct nlattr **);
    int (*ndo_get_vf_port)(struct net_device *, int, struct sk_buff *);
    int (*ndo_get_vf_guid)(struct net_device *, int, struct ifla_vf_guid *, struct ifla_vf_guid *);
    int (*ndo_set_vf_guid)(struct net_device *, int, u64, int);
    int (*ndo_set_vf_rss_query_en)(struct net_device *, int, bool);
    int (*ndo_setup_tc)(struct net_device *, enum tc_setup_type, void *);
    int (*ndo_fcoe_enable)(struct net_device *);
    int (*ndo_fcoe_disable)(struct net_device *);
    int (*ndo_fcoe_ddp_setup)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_ddp_done)(struct net_device *, u16);
    int (*ndo_fcoe_ddp_target)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_get_hbainfo)(struct net_device *, struct netdev_fcoe_hbainfo *);
    int (*ndo_fcoe_get_wwn)(struct net_device *, u64 *, int);
    int (*ndo_rx_flow_steer)(struct net_device *, const struct sk_buff *, u16, u32);
    int (*ndo_add_slave)(struct net_device *, struct net_device *, struct netlink_ext_ack *);
    int (*ndo_del_slave)(struct net_device *, struct net_device *);
    struct net_device * (*ndo_get_xmit_slave)(struct net_device *, struct sk_buff *, bool);
    struct net_device * (*ndo_sk_get_lower_dev)(struct net_device *, struct sock *);
    netdev_features_t (*ndo_fix_features)(struct net_device *, netdev_features_t);
    int (*ndo_set_features)(struct net_device *, netdev_features_t);
    int (*ndo_neigh_construct)(struct net_device *, struct neighbour *);
    void (*ndo_neigh_destroy)(struct net_device *, struct neighbour *);
    int (*ndo_fdb_add)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, u16, struct netlink_ext_ack *);
    int (*ndo_fdb_del)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, struct netlink_ext_ack *);
    int (*ndo_fdb_del_bulk)(struct ndmsg *, struct nlattr **, struct net_device *, u16, struct netlink_ext_ack *);
    int (*ndo_fdb_dump)(struct sk_buff *, struct netlink_callback *, struct net_device *, struct net_device *, int *);
    int (*ndo_fdb_get)(struct sk_buff *, struct nlattr **, struct net_device *, const unsigned char *, u16, u32, u32, struct netlink_ext_ack *);
    int (*ndo_mdb_add)(struct net_device *, struct nlattr **, u16, struct netlink_ext_ack *);
    int (*ndo_mdb_del)(struct net_device *, struct nlattr **, struct netlink_ext_ack *);
    int (*ndo_mdb_dump)(struct net_device *, struct sk_buff *, struct netlink_callback *);
    int (*ndo_bridge_setlink)(struct net_device *, struct nlmsghdr *, u16, struct netlink_ext_ack *);
    int (*ndo_bridge_getlink)(struct sk_buff *, u32, u32, struct net_device *, u32, int);
    int (*ndo_bridge_dellink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_change_carrier)(struct net_device *, bool);
    int (*ndo_get_phys_port_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_port_parent_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_phys_port_name)(struct net_device *, char *, size_t);
    void * (*ndo_dfwd_add_station)(struct net_device *, struct net_device *);
    void (*ndo_dfwd_del_station)(struct net_device *, void *);
    int (*ndo_set_tx_maxrate)(struct net_device *, int, u32);
    int (*ndo_get_iflink)(const struct net_device *);
    int (*ndo_fill_metadata_dst)(struct net_device *, struct sk_buff *);
    void (*ndo_set_rx_headroom)(struct net_device *, int);
    int (*ndo_bpf)(struct net_device *, struct netdev_bpf *);
    int (*ndo_xdp_xmit)(struct net_device *, int, struct xdp_frame **, u32);
    struct net_device * (*ndo_xdp_get_xmit_slave)(struct net_device *, struct xdp_buff *);
    int (*ndo_xsk_wakeup)(struct net_device *, u32, u32);
    int (*ndo_tunnel_ctl)(struct net_device *, struct ip_tunnel_parm *, int);
    struct net_device * (*ndo_get_peer_dev)(struct net_device *);
    int (*ndo_fill_forward_path)(struct net_device_path_ctx *, struct net_device_path *);
    ktime_t (*ndo_get_tstamp)(struct net_device *, const struct skb_shared_hwtstamps *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct net_device_ops {
    int (*ndo_init)(struct net_device *);
    void (*ndo_uninit)(struct net_device *);
    int (*ndo_open)(struct net_device *);
    int (*ndo_stop)(struct net_device *);
    netdev_tx_t (*ndo_start_xmit)(struct sk_buff *, struct net_device *);
    netdev_features_t (*ndo_features_check)(struct sk_buff *, struct net_device *, netdev_features_t);
    u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, struct net_device *);
    void (*ndo_change_rx_flags)(struct net_device *, int);
    void (*ndo_set_rx_mode)(struct net_device *);
    int (*ndo_set_mac_address)(struct net_device *, void *);
    int (*ndo_validate_addr)(struct net_device *);
    int (*ndo_do_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_eth_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_siocbond)(struct net_device *, struct ifreq *, int);
    int (*ndo_siocwandev)(struct net_device *, struct if_settings *);
    int (*ndo_siocdevprivate)(struct net_device *, struct ifreq *, void *, int);
    int (*ndo_set_config)(struct net_device *, struct ifmap *);
    int (*ndo_change_mtu)(struct net_device *, int);
    int (*ndo_neigh_setup)(struct net_device *, struct neigh_parms *);
    void (*ndo_tx_timeout)(struct net_device *, unsigned int);
    void (*ndo_get_stats64)(struct net_device *, struct rtnl_link_stats64 *);
    bool (*ndo_has_offload_stats)(const struct net_device *, int);
    int (*ndo_get_offload_stats)(int, const struct net_device *, void *);
    struct net_device_stats * (*ndo_get_stats)(struct net_device *);
    int (*ndo_vlan_rx_add_vid)(struct net_device *, __be16, u16);
    int (*ndo_vlan_rx_kill_vid)(struct net_device *, __be16, u16);
    void (*ndo_poll_controller)(struct net_device *);
    int (*ndo_netpoll_setup)(struct net_device *, struct netpoll_info *);
    void (*ndo_netpoll_cleanup)(struct net_device *);
    int (*ndo_set_vf_mac)(struct net_device *, int, u8 *);
    int (*ndo_set_vf_vlan)(struct net_device *, int, u16, u8, __be16);
    int (*ndo_set_vf_rate)(struct net_device *, int, int, int);
    int (*ndo_set_vf_spoofchk)(struct net_device *, int, bool);
    int (*ndo_set_vf_trust)(struct net_device *, int, bool);
    int (*ndo_get_vf_config)(struct net_device *, int, struct ifla_vf_info *);
    int (*ndo_set_vf_link_state)(struct net_device *, int, int);
    int (*ndo_get_vf_stats)(struct net_device *, int, struct ifla_vf_stats *);
    int (*ndo_set_vf_port)(struct net_device *, int, struct nlattr **);
    int (*ndo_get_vf_port)(struct net_device *, int, struct sk_buff *);
    int (*ndo_get_vf_guid)(struct net_device *, int, struct ifla_vf_guid *, struct ifla_vf_guid *);
    int (*ndo_set_vf_guid)(struct net_device *, int, u64, int);
    int (*ndo_set_vf_rss_query_en)(struct net_device *, int, bool);
    int (*ndo_setup_tc)(struct net_device *, enum tc_setup_type, void *);
    int (*ndo_fcoe_enable)(struct net_device *);
    int (*ndo_fcoe_disable)(struct net_device *);
    int (*ndo_fcoe_ddp_setup)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_ddp_done)(struct net_device *, u16);
    int (*ndo_fcoe_ddp_target)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_get_hbainfo)(struct net_device *, struct netdev_fcoe_hbainfo *);
    int (*ndo_fcoe_get_wwn)(struct net_device *, u64 *, int);
    int (*ndo_rx_flow_steer)(struct net_device *, const struct sk_buff *, u16, u32);
    int (*ndo_add_slave)(struct net_device *, struct net_device *, struct netlink_ext_ack *);
    int (*ndo_del_slave)(struct net_device *, struct net_device *);
    struct net_device * (*ndo_get_xmit_slave)(struct net_device *, struct sk_buff *, bool);
    struct net_device * (*ndo_sk_get_lower_dev)(struct net_device *, struct sock *);
    netdev_features_t (*ndo_fix_features)(struct net_device *, netdev_features_t);
    int (*ndo_set_features)(struct net_device *, netdev_features_t);
    int (*ndo_neigh_construct)(struct net_device *, struct neighbour *);
    void (*ndo_neigh_destroy)(struct net_device *, struct neighbour *);
    int (*ndo_fdb_add)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, u16, struct netlink_ext_ack *);
    int (*ndo_fdb_del)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, struct netlink_ext_ack *);
    int (*ndo_fdb_del_bulk)(struct nlmsghdr *, struct net_device *, struct netlink_ext_ack *);
    int (*ndo_fdb_dump)(struct sk_buff *, struct netlink_callback *, struct net_device *, struct net_device *, int *);
    int (*ndo_fdb_get)(struct sk_buff *, struct nlattr **, struct net_device *, const unsigned char *, u16, u32, u32, struct netlink_ext_ack *);
    int (*ndo_mdb_add)(struct net_device *, struct nlattr **, u16, struct netlink_ext_ack *);
    int (*ndo_mdb_del)(struct net_device *, struct nlattr **, struct netlink_ext_ack *);
    int (*ndo_mdb_del_bulk)(struct net_device *, struct nlattr **, struct netlink_ext_ack *);
    int (*ndo_mdb_dump)(struct net_device *, struct sk_buff *, struct netlink_callback *);
    int (*ndo_mdb_get)(struct net_device *, struct nlattr **, u32, u32, struct netlink_ext_ack *);
    int (*ndo_bridge_setlink)(struct net_device *, struct nlmsghdr *, u16, struct netlink_ext_ack *);
    int (*ndo_bridge_getlink)(struct sk_buff *, u32, u32, struct net_device *, u32, int);
    int (*ndo_bridge_dellink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_change_carrier)(struct net_device *, bool);
    int (*ndo_get_phys_port_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_port_parent_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_phys_port_name)(struct net_device *, char *, size_t);
    void * (*ndo_dfwd_add_station)(struct net_device *, struct net_device *);
    void (*ndo_dfwd_del_station)(struct net_device *, void *);
    int (*ndo_set_tx_maxrate)(struct net_device *, int, u32);
    int (*ndo_get_iflink)(const struct net_device *);
    int (*ndo_fill_metadata_dst)(struct net_device *, struct sk_buff *);
    void (*ndo_set_rx_headroom)(struct net_device *, int);
    int (*ndo_bpf)(struct net_device *, struct netdev_bpf *);
    int (*ndo_xdp_xmit)(struct net_device *, int, struct xdp_frame **, u32);
    struct net_device * (*ndo_xdp_get_xmit_slave)(struct net_device *, struct xdp_buff *);
    int (*ndo_xsk_wakeup)(struct net_device *, u32, u32);
    int (*ndo_tunnel_ctl)(struct net_device *, struct ip_tunnel_parm *, int);
    struct net_device * (*ndo_get_peer_dev)(struct net_device *);
    int (*ndo_fill_forward_path)(struct net_device_path_ctx *, struct net_device_path *);
    ktime_t (*ndo_get_tstamp)(struct net_device *, const struct skb_shared_hwtstamps *, bool);
    int (*ndo_hwtstamp_get)(struct net_device *, struct kernel_hwtstamp_config *);
    int (*ndo_hwtstamp_set)(struct net_device *, struct kernel_hwtstamp_config *, struct netlink_ext_ack *);
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
struct net_device_ops {
    int (*ndo_init)(struct net_device *);
    void (*ndo_uninit)(struct net_device *);
    int (*ndo_open)(struct net_device *);
    int (*ndo_stop)(struct net_device *);
    netdev_tx_t (*ndo_start_xmit)(struct sk_buff *, struct net_device *);
    netdev_features_t (*ndo_features_check)(struct sk_buff *, struct net_device *, netdev_features_t);
    u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, struct net_device *);
    void (*ndo_change_rx_flags)(struct net_device *, int);
    void (*ndo_set_rx_mode)(struct net_device *);
    int (*ndo_set_mac_address)(struct net_device *, void *);
    int (*ndo_validate_addr)(struct net_device *);
    int (*ndo_do_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_set_config)(struct net_device *, struct ifmap *);
    int (*ndo_change_mtu)(struct net_device *, int);
    int (*ndo_neigh_setup)(struct net_device *, struct neigh_parms *);
    void (*ndo_tx_timeout)(struct net_device *);
    void (*ndo_get_stats64)(struct net_device *, struct rtnl_link_stats64 *);
    bool (*ndo_has_offload_stats)(const struct net_device *, int);
    int (*ndo_get_offload_stats)(int, const struct net_device *, void *);
    struct net_device_stats * (*ndo_get_stats)(struct net_device *);
    int (*ndo_vlan_rx_add_vid)(struct net_device *, __be16, u16);
    int (*ndo_vlan_rx_kill_vid)(struct net_device *, __be16, u16);
    void (*ndo_poll_controller)(struct net_device *);
    int (*ndo_netpoll_setup)(struct net_device *, struct netpoll_info *);
    void (*ndo_netpoll_cleanup)(struct net_device *);
    int (*ndo_set_vf_mac)(struct net_device *, int, u8 *);
    int (*ndo_set_vf_vlan)(struct net_device *, int, u16, u8, __be16);
    int (*ndo_set_vf_rate)(struct net_device *, int, int, int);
    int (*ndo_set_vf_spoofchk)(struct net_device *, int, bool);
    int (*ndo_set_vf_trust)(struct net_device *, int, bool);
    int (*ndo_get_vf_config)(struct net_device *, int, struct ifla_vf_info *);
    int (*ndo_set_vf_link_state)(struct net_device *, int, int);
    int (*ndo_get_vf_stats)(struct net_device *, int, struct ifla_vf_stats *);
    int (*ndo_set_vf_port)(struct net_device *, int, struct nlattr **);
    int (*ndo_get_vf_port)(struct net_device *, int, struct sk_buff *);
    int (*ndo_set_vf_guid)(struct net_device *, int, u64, int);
    int (*ndo_set_vf_rss_query_en)(struct net_device *, int, bool);
    int (*ndo_setup_tc)(struct net_device *, enum tc_setup_type, void *);
    int (*ndo_fcoe_enable)(struct net_device *);
    int (*ndo_fcoe_disable)(struct net_device *);
    int (*ndo_fcoe_ddp_setup)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_ddp_done)(struct net_device *, u16);
    int (*ndo_fcoe_ddp_target)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_get_hbainfo)(struct net_device *, struct netdev_fcoe_hbainfo *);
    int (*ndo_fcoe_get_wwn)(struct net_device *, u64 *, int);
    int (*ndo_rx_flow_steer)(struct net_device *, const struct sk_buff *, u16, u32);
    int (*ndo_add_slave)(struct net_device *, struct net_device *, struct netlink_ext_ack *);
    int (*ndo_del_slave)(struct net_device *, struct net_device *);
    netdev_features_t (*ndo_fix_features)(struct net_device *, netdev_features_t);
    int (*ndo_set_features)(struct net_device *, netdev_features_t);
    int (*ndo_neigh_construct)(struct net_device *, struct neighbour *);
    void (*ndo_neigh_destroy)(struct net_device *, struct neighbour *);
    int (*ndo_fdb_add)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, u16, struct netlink_ext_ack *);
    int (*ndo_fdb_del)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16);
    int (*ndo_fdb_dump)(struct sk_buff *, struct netlink_callback *, struct net_device *, struct net_device *, int *);
    int (*ndo_fdb_get)(struct sk_buff *, struct nlattr **, struct net_device *, const unsigned char *, u16, u32, u32, struct netlink_ext_ack *);
    int (*ndo_bridge_setlink)(struct net_device *, struct nlmsghdr *, u16, struct netlink_ext_ack *);
    int (*ndo_bridge_getlink)(struct sk_buff *, u32, u32, struct net_device *, u32, int);
    int (*ndo_bridge_dellink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_change_carrier)(struct net_device *, bool);
    int (*ndo_get_phys_port_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_port_parent_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_phys_port_name)(struct net_device *, char *, size_t);
    void (*ndo_udp_tunnel_add)(struct net_device *, struct udp_tunnel_info *);
    void (*ndo_udp_tunnel_del)(struct net_device *, struct udp_tunnel_info *);
    void * (*ndo_dfwd_add_station)(struct net_device *, struct net_device *);
    void (*ndo_dfwd_del_station)(struct net_device *, void *);
    int (*ndo_set_tx_maxrate)(struct net_device *, int, u32);
    int (*ndo_get_iflink)(const struct net_device *);
    int (*ndo_change_proto_down)(struct net_device *, bool);
    int (*ndo_fill_metadata_dst)(struct net_device *, struct sk_buff *);
    void (*ndo_set_rx_headroom)(struct net_device *, int);
    int (*ndo_bpf)(struct net_device *, struct netdev_bpf *);
    int (*ndo_xdp_xmit)(struct net_device *, int, struct xdp_frame **, u32);
    int (*ndo_xsk_wakeup)(struct net_device *, u32, u32);
    struct devlink_port * (*ndo_get_devlink_port)(struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct net_device_ops {
    int (*ndo_init)(struct net_device *);
    void (*ndo_uninit)(struct net_device *);
    int (*ndo_open)(struct net_device *);
    int (*ndo_stop)(struct net_device *);
    netdev_tx_t (*ndo_start_xmit)(struct sk_buff *, struct net_device *);
    netdev_features_t (*ndo_features_check)(struct sk_buff *, struct net_device *, netdev_features_t);
    u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, struct net_device *);
    void (*ndo_change_rx_flags)(struct net_device *, int);
    void (*ndo_set_rx_mode)(struct net_device *);
    int (*ndo_set_mac_address)(struct net_device *, void *);
    int (*ndo_validate_addr)(struct net_device *);
    int (*ndo_do_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_set_config)(struct net_device *, struct ifmap *);
    int (*ndo_change_mtu)(struct net_device *, int);
    int (*ndo_neigh_setup)(struct net_device *, struct neigh_parms *);
    void (*ndo_tx_timeout)(struct net_device *);
    void (*ndo_get_stats64)(struct net_device *, struct rtnl_link_stats64 *);
    bool (*ndo_has_offload_stats)(const struct net_device *, int);
    int (*ndo_get_offload_stats)(int, const struct net_device *, void *);
    struct net_device_stats * (*ndo_get_stats)(struct net_device *);
    int (*ndo_vlan_rx_add_vid)(struct net_device *, __be16, u16);
    int (*ndo_vlan_rx_kill_vid)(struct net_device *, __be16, u16);
    void (*ndo_poll_controller)(struct net_device *);
    int (*ndo_netpoll_setup)(struct net_device *, struct netpoll_info *);
    void (*ndo_netpoll_cleanup)(struct net_device *);
    int (*ndo_set_vf_mac)(struct net_device *, int, u8 *);
    int (*ndo_set_vf_vlan)(struct net_device *, int, u16, u8, __be16);
    int (*ndo_set_vf_rate)(struct net_device *, int, int, int);
    int (*ndo_set_vf_spoofchk)(struct net_device *, int, bool);
    int (*ndo_set_vf_trust)(struct net_device *, int, bool);
    int (*ndo_get_vf_config)(struct net_device *, int, struct ifla_vf_info *);
    int (*ndo_set_vf_link_state)(struct net_device *, int, int);
    int (*ndo_get_vf_stats)(struct net_device *, int, struct ifla_vf_stats *);
    int (*ndo_set_vf_port)(struct net_device *, int, struct nlattr **);
    int (*ndo_get_vf_port)(struct net_device *, int, struct sk_buff *);
    int (*ndo_set_vf_guid)(struct net_device *, int, u64, int);
    int (*ndo_set_vf_rss_query_en)(struct net_device *, int, bool);
    int (*ndo_setup_tc)(struct net_device *, enum tc_setup_type, void *);
    int (*ndo_fcoe_enable)(struct net_device *);
    int (*ndo_fcoe_disable)(struct net_device *);
    int (*ndo_fcoe_ddp_setup)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_ddp_done)(struct net_device *, u16);
    int (*ndo_fcoe_ddp_target)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_get_hbainfo)(struct net_device *, struct netdev_fcoe_hbainfo *);
    int (*ndo_fcoe_get_wwn)(struct net_device *, u64 *, int);
    int (*ndo_rx_flow_steer)(struct net_device *, const struct sk_buff *, u16, u32);
    int (*ndo_add_slave)(struct net_device *, struct net_device *, struct netlink_ext_ack *);
    int (*ndo_del_slave)(struct net_device *, struct net_device *);
    netdev_features_t (*ndo_fix_features)(struct net_device *, netdev_features_t);
    int (*ndo_set_features)(struct net_device *, netdev_features_t);
    int (*ndo_neigh_construct)(struct net_device *, struct neighbour *);
    void (*ndo_neigh_destroy)(struct net_device *, struct neighbour *);
    int (*ndo_fdb_add)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, u16, struct netlink_ext_ack *);
    int (*ndo_fdb_del)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16);
    int (*ndo_fdb_dump)(struct sk_buff *, struct netlink_callback *, struct net_device *, struct net_device *, int *);
    int (*ndo_fdb_get)(struct sk_buff *, struct nlattr **, struct net_device *, const unsigned char *, u16, u32, u32, struct netlink_ext_ack *);
    int (*ndo_bridge_setlink)(struct net_device *, struct nlmsghdr *, u16, struct netlink_ext_ack *);
    int (*ndo_bridge_getlink)(struct sk_buff *, u32, u32, struct net_device *, u32, int);
    int (*ndo_bridge_dellink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_change_carrier)(struct net_device *, bool);
    int (*ndo_get_phys_port_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_port_parent_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_phys_port_name)(struct net_device *, char *, size_t);
    void (*ndo_udp_tunnel_add)(struct net_device *, struct udp_tunnel_info *);
    void (*ndo_udp_tunnel_del)(struct net_device *, struct udp_tunnel_info *);
    void * (*ndo_dfwd_add_station)(struct net_device *, struct net_device *);
    void (*ndo_dfwd_del_station)(struct net_device *, void *);
    int (*ndo_set_tx_maxrate)(struct net_device *, int, u32);
    int (*ndo_get_iflink)(const struct net_device *);
    int (*ndo_change_proto_down)(struct net_device *, bool);
    int (*ndo_fill_metadata_dst)(struct net_device *, struct sk_buff *);
    void (*ndo_set_rx_headroom)(struct net_device *, int);
    int (*ndo_bpf)(struct net_device *, struct netdev_bpf *);
    int (*ndo_xdp_xmit)(struct net_device *, int, struct xdp_frame **, u32);
    int (*ndo_xsk_wakeup)(struct net_device *, u32, u32);
    struct devlink_port * (*ndo_get_devlink_port)(struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct net_device_ops {
    int (*ndo_init)(struct net_device *);
    void (*ndo_uninit)(struct net_device *);
    int (*ndo_open)(struct net_device *);
    int (*ndo_stop)(struct net_device *);
    netdev_tx_t (*ndo_start_xmit)(struct sk_buff *, struct net_device *);
    netdev_features_t (*ndo_features_check)(struct sk_buff *, struct net_device *, netdev_features_t);
    u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, struct net_device *);
    void (*ndo_change_rx_flags)(struct net_device *, int);
    void (*ndo_set_rx_mode)(struct net_device *);
    int (*ndo_set_mac_address)(struct net_device *, void *);
    int (*ndo_validate_addr)(struct net_device *);
    int (*ndo_do_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_set_config)(struct net_device *, struct ifmap *);
    int (*ndo_change_mtu)(struct net_device *, int);
    int (*ndo_neigh_setup)(struct net_device *, struct neigh_parms *);
    void (*ndo_tx_timeout)(struct net_device *);
    void (*ndo_get_stats64)(struct net_device *, struct rtnl_link_stats64 *);
    bool (*ndo_has_offload_stats)(const struct net_device *, int);
    int (*ndo_get_offload_stats)(int, const struct net_device *, void *);
    struct net_device_stats * (*ndo_get_stats)(struct net_device *);
    int (*ndo_vlan_rx_add_vid)(struct net_device *, __be16, u16);
    int (*ndo_vlan_rx_kill_vid)(struct net_device *, __be16, u16);
    void (*ndo_poll_controller)(struct net_device *);
    int (*ndo_netpoll_setup)(struct net_device *, struct netpoll_info *);
    void (*ndo_netpoll_cleanup)(struct net_device *);
    int (*ndo_set_vf_mac)(struct net_device *, int, u8 *);
    int (*ndo_set_vf_vlan)(struct net_device *, int, u16, u8, __be16);
    int (*ndo_set_vf_rate)(struct net_device *, int, int, int);
    int (*ndo_set_vf_spoofchk)(struct net_device *, int, bool);
    int (*ndo_set_vf_trust)(struct net_device *, int, bool);
    int (*ndo_get_vf_config)(struct net_device *, int, struct ifla_vf_info *);
    int (*ndo_set_vf_link_state)(struct net_device *, int, int);
    int (*ndo_get_vf_stats)(struct net_device *, int, struct ifla_vf_stats *);
    int (*ndo_set_vf_port)(struct net_device *, int, struct nlattr **);
    int (*ndo_get_vf_port)(struct net_device *, int, struct sk_buff *);
    int (*ndo_set_vf_guid)(struct net_device *, int, u64, int);
    int (*ndo_set_vf_rss_query_en)(struct net_device *, int, bool);
    int (*ndo_setup_tc)(struct net_device *, enum tc_setup_type, void *);
    int (*ndo_fcoe_enable)(struct net_device *);
    int (*ndo_fcoe_disable)(struct net_device *);
    int (*ndo_fcoe_ddp_setup)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_ddp_done)(struct net_device *, u16);
    int (*ndo_fcoe_ddp_target)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_get_hbainfo)(struct net_device *, struct netdev_fcoe_hbainfo *);
    int (*ndo_fcoe_get_wwn)(struct net_device *, u64 *, int);
    int (*ndo_rx_flow_steer)(struct net_device *, const struct sk_buff *, u16, u32);
    int (*ndo_add_slave)(struct net_device *, struct net_device *, struct netlink_ext_ack *);
    int (*ndo_del_slave)(struct net_device *, struct net_device *);
    netdev_features_t (*ndo_fix_features)(struct net_device *, netdev_features_t);
    int (*ndo_set_features)(struct net_device *, netdev_features_t);
    int (*ndo_neigh_construct)(struct net_device *, struct neighbour *);
    void (*ndo_neigh_destroy)(struct net_device *, struct neighbour *);
    int (*ndo_fdb_add)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, u16, struct netlink_ext_ack *);
    int (*ndo_fdb_del)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16);
    int (*ndo_fdb_dump)(struct sk_buff *, struct netlink_callback *, struct net_device *, struct net_device *, int *);
    int (*ndo_fdb_get)(struct sk_buff *, struct nlattr **, struct net_device *, const unsigned char *, u16, u32, u32, struct netlink_ext_ack *);
    int (*ndo_bridge_setlink)(struct net_device *, struct nlmsghdr *, u16, struct netlink_ext_ack *);
    int (*ndo_bridge_getlink)(struct sk_buff *, u32, u32, struct net_device *, u32, int);
    int (*ndo_bridge_dellink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_change_carrier)(struct net_device *, bool);
    int (*ndo_get_phys_port_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_port_parent_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_phys_port_name)(struct net_device *, char *, size_t);
    void (*ndo_udp_tunnel_add)(struct net_device *, struct udp_tunnel_info *);
    void (*ndo_udp_tunnel_del)(struct net_device *, struct udp_tunnel_info *);
    void * (*ndo_dfwd_add_station)(struct net_device *, struct net_device *);
    void (*ndo_dfwd_del_station)(struct net_device *, void *);
    int (*ndo_set_tx_maxrate)(struct net_device *, int, u32);
    int (*ndo_get_iflink)(const struct net_device *);
    int (*ndo_change_proto_down)(struct net_device *, bool);
    int (*ndo_fill_metadata_dst)(struct net_device *, struct sk_buff *);
    void (*ndo_set_rx_headroom)(struct net_device *, int);
    int (*ndo_bpf)(struct net_device *, struct netdev_bpf *);
    int (*ndo_xdp_xmit)(struct net_device *, int, struct xdp_frame **, u32);
    int (*ndo_xsk_wakeup)(struct net_device *, u32, u32);
    struct devlink_port * (*ndo_get_devlink_port)(struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct net_device_ops {
    int (*ndo_init)(struct net_device *);
    void (*ndo_uninit)(struct net_device *);
    int (*ndo_open)(struct net_device *);
    int (*ndo_stop)(struct net_device *);
    netdev_tx_t (*ndo_start_xmit)(struct sk_buff *, struct net_device *);
    netdev_features_t (*ndo_features_check)(struct sk_buff *, struct net_device *, netdev_features_t);
    u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, struct net_device *);
    void (*ndo_change_rx_flags)(struct net_device *, int);
    void (*ndo_set_rx_mode)(struct net_device *);
    int (*ndo_set_mac_address)(struct net_device *, void *);
    int (*ndo_validate_addr)(struct net_device *);
    int (*ndo_do_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_set_config)(struct net_device *, struct ifmap *);
    int (*ndo_change_mtu)(struct net_device *, int);
    int (*ndo_neigh_setup)(struct net_device *, struct neigh_parms *);
    void (*ndo_tx_timeout)(struct net_device *);
    void (*ndo_get_stats64)(struct net_device *, struct rtnl_link_stats64 *);
    bool (*ndo_has_offload_stats)(const struct net_device *, int);
    int (*ndo_get_offload_stats)(int, const struct net_device *, void *);
    struct net_device_stats * (*ndo_get_stats)(struct net_device *);
    int (*ndo_vlan_rx_add_vid)(struct net_device *, __be16, u16);
    int (*ndo_vlan_rx_kill_vid)(struct net_device *, __be16, u16);
    void (*ndo_poll_controller)(struct net_device *);
    int (*ndo_netpoll_setup)(struct net_device *, struct netpoll_info *);
    void (*ndo_netpoll_cleanup)(struct net_device *);
    int (*ndo_set_vf_mac)(struct net_device *, int, u8 *);
    int (*ndo_set_vf_vlan)(struct net_device *, int, u16, u8, __be16);
    int (*ndo_set_vf_rate)(struct net_device *, int, int, int);
    int (*ndo_set_vf_spoofchk)(struct net_device *, int, bool);
    int (*ndo_set_vf_trust)(struct net_device *, int, bool);
    int (*ndo_get_vf_config)(struct net_device *, int, struct ifla_vf_info *);
    int (*ndo_set_vf_link_state)(struct net_device *, int, int);
    int (*ndo_get_vf_stats)(struct net_device *, int, struct ifla_vf_stats *);
    int (*ndo_set_vf_port)(struct net_device *, int, struct nlattr **);
    int (*ndo_get_vf_port)(struct net_device *, int, struct sk_buff *);
    int (*ndo_set_vf_guid)(struct net_device *, int, u64, int);
    int (*ndo_set_vf_rss_query_en)(struct net_device *, int, bool);
    int (*ndo_setup_tc)(struct net_device *, enum tc_setup_type, void *);
    int (*ndo_fcoe_enable)(struct net_device *);
    int (*ndo_fcoe_disable)(struct net_device *);
    int (*ndo_fcoe_ddp_setup)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_ddp_done)(struct net_device *, u16);
    int (*ndo_fcoe_ddp_target)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_get_hbainfo)(struct net_device *, struct netdev_fcoe_hbainfo *);
    int (*ndo_fcoe_get_wwn)(struct net_device *, u64 *, int);
    int (*ndo_rx_flow_steer)(struct net_device *, const struct sk_buff *, u16, u32);
    int (*ndo_add_slave)(struct net_device *, struct net_device *, struct netlink_ext_ack *);
    int (*ndo_del_slave)(struct net_device *, struct net_device *);
    netdev_features_t (*ndo_fix_features)(struct net_device *, netdev_features_t);
    int (*ndo_set_features)(struct net_device *, netdev_features_t);
    int (*ndo_neigh_construct)(struct net_device *, struct neighbour *);
    void (*ndo_neigh_destroy)(struct net_device *, struct neighbour *);
    int (*ndo_fdb_add)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, u16, struct netlink_ext_ack *);
    int (*ndo_fdb_del)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16);
    int (*ndo_fdb_dump)(struct sk_buff *, struct netlink_callback *, struct net_device *, struct net_device *, int *);
    int (*ndo_fdb_get)(struct sk_buff *, struct nlattr **, struct net_device *, const unsigned char *, u16, u32, u32, struct netlink_ext_ack *);
    int (*ndo_bridge_setlink)(struct net_device *, struct nlmsghdr *, u16, struct netlink_ext_ack *);
    int (*ndo_bridge_getlink)(struct sk_buff *, u32, u32, struct net_device *, u32, int);
    int (*ndo_bridge_dellink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_change_carrier)(struct net_device *, bool);
    int (*ndo_get_phys_port_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_port_parent_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_phys_port_name)(struct net_device *, char *, size_t);
    void (*ndo_udp_tunnel_add)(struct net_device *, struct udp_tunnel_info *);
    void (*ndo_udp_tunnel_del)(struct net_device *, struct udp_tunnel_info *);
    void * (*ndo_dfwd_add_station)(struct net_device *, struct net_device *);
    void (*ndo_dfwd_del_station)(struct net_device *, void *);
    int (*ndo_set_tx_maxrate)(struct net_device *, int, u32);
    int (*ndo_get_iflink)(const struct net_device *);
    int (*ndo_change_proto_down)(struct net_device *, bool);
    int (*ndo_fill_metadata_dst)(struct net_device *, struct sk_buff *);
    void (*ndo_set_rx_headroom)(struct net_device *, int);
    int (*ndo_bpf)(struct net_device *, struct netdev_bpf *);
    int (*ndo_xdp_xmit)(struct net_device *, int, struct xdp_frame **, u32);
    int (*ndo_xsk_wakeup)(struct net_device *, u32, u32);
    struct devlink_port * (*ndo_get_devlink_port)(struct net_device *);
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
struct net_device_ops {
    int (*ndo_init)(struct net_device *);
    void (*ndo_uninit)(struct net_device *);
    int (*ndo_open)(struct net_device *);
    int (*ndo_stop)(struct net_device *);
    netdev_tx_t (*ndo_start_xmit)(struct sk_buff *, struct net_device *);
    netdev_features_t (*ndo_features_check)(struct sk_buff *, struct net_device *, netdev_features_t);
    u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, struct net_device *);
    void (*ndo_change_rx_flags)(struct net_device *, int);
    void (*ndo_set_rx_mode)(struct net_device *);
    int (*ndo_set_mac_address)(struct net_device *, void *);
    int (*ndo_validate_addr)(struct net_device *);
    int (*ndo_do_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_set_config)(struct net_device *, struct ifmap *);
    int (*ndo_change_mtu)(struct net_device *, int);
    int (*ndo_neigh_setup)(struct net_device *, struct neigh_parms *);
    void (*ndo_tx_timeout)(struct net_device *);
    void (*ndo_get_stats64)(struct net_device *, struct rtnl_link_stats64 *);
    bool (*ndo_has_offload_stats)(const struct net_device *, int);
    int (*ndo_get_offload_stats)(int, const struct net_device *, void *);
    struct net_device_stats * (*ndo_get_stats)(struct net_device *);
    int (*ndo_vlan_rx_add_vid)(struct net_device *, __be16, u16);
    int (*ndo_vlan_rx_kill_vid)(struct net_device *, __be16, u16);
    void (*ndo_poll_controller)(struct net_device *);
    int (*ndo_netpoll_setup)(struct net_device *, struct netpoll_info *);
    void (*ndo_netpoll_cleanup)(struct net_device *);
    int (*ndo_set_vf_mac)(struct net_device *, int, u8 *);
    int (*ndo_set_vf_vlan)(struct net_device *, int, u16, u8, __be16);
    int (*ndo_set_vf_rate)(struct net_device *, int, int, int);
    int (*ndo_set_vf_spoofchk)(struct net_device *, int, bool);
    int (*ndo_set_vf_trust)(struct net_device *, int, bool);
    int (*ndo_get_vf_config)(struct net_device *, int, struct ifla_vf_info *);
    int (*ndo_set_vf_link_state)(struct net_device *, int, int);
    int (*ndo_get_vf_stats)(struct net_device *, int, struct ifla_vf_stats *);
    int (*ndo_set_vf_port)(struct net_device *, int, struct nlattr **);
    int (*ndo_get_vf_port)(struct net_device *, int, struct sk_buff *);
    int (*ndo_set_vf_guid)(struct net_device *, int, u64, int);
    int (*ndo_set_vf_rss_query_en)(struct net_device *, int, bool);
    int (*ndo_setup_tc)(struct net_device *, enum tc_setup_type, void *);
    int (*ndo_fcoe_enable)(struct net_device *);
    int (*ndo_fcoe_disable)(struct net_device *);
    int (*ndo_fcoe_ddp_setup)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_ddp_done)(struct net_device *, u16);
    int (*ndo_fcoe_ddp_target)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_get_hbainfo)(struct net_device *, struct netdev_fcoe_hbainfo *);
    int (*ndo_fcoe_get_wwn)(struct net_device *, u64 *, int);
    int (*ndo_rx_flow_steer)(struct net_device *, const struct sk_buff *, u16, u32);
    int (*ndo_add_slave)(struct net_device *, struct net_device *, struct netlink_ext_ack *);
    int (*ndo_del_slave)(struct net_device *, struct net_device *);
    netdev_features_t (*ndo_fix_features)(struct net_device *, netdev_features_t);
    int (*ndo_set_features)(struct net_device *, netdev_features_t);
    int (*ndo_neigh_construct)(struct net_device *, struct neighbour *);
    void (*ndo_neigh_destroy)(struct net_device *, struct neighbour *);
    int (*ndo_fdb_add)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, u16, struct netlink_ext_ack *);
    int (*ndo_fdb_del)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16);
    int (*ndo_fdb_dump)(struct sk_buff *, struct netlink_callback *, struct net_device *, struct net_device *, int *);
    int (*ndo_fdb_get)(struct sk_buff *, struct nlattr **, struct net_device *, const unsigned char *, u16, u32, u32, struct netlink_ext_ack *);
    int (*ndo_bridge_setlink)(struct net_device *, struct nlmsghdr *, u16, struct netlink_ext_ack *);
    int (*ndo_bridge_getlink)(struct sk_buff *, u32, u32, struct net_device *, u32, int);
    int (*ndo_bridge_dellink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_change_carrier)(struct net_device *, bool);
    int (*ndo_get_phys_port_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_port_parent_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_phys_port_name)(struct net_device *, char *, size_t);
    void (*ndo_udp_tunnel_add)(struct net_device *, struct udp_tunnel_info *);
    void (*ndo_udp_tunnel_del)(struct net_device *, struct udp_tunnel_info *);
    void * (*ndo_dfwd_add_station)(struct net_device *, struct net_device *);
    void (*ndo_dfwd_del_station)(struct net_device *, void *);
    int (*ndo_set_tx_maxrate)(struct net_device *, int, u32);
    int (*ndo_get_iflink)(const struct net_device *);
    int (*ndo_change_proto_down)(struct net_device *, bool);
    int (*ndo_fill_metadata_dst)(struct net_device *, struct sk_buff *);
    void (*ndo_set_rx_headroom)(struct net_device *, int);
    int (*ndo_bpf)(struct net_device *, struct netdev_bpf *);
    int (*ndo_xdp_xmit)(struct net_device *, int, struct xdp_frame **, u32);
    int (*ndo_xsk_wakeup)(struct net_device *, u32, u32);
    struct devlink_port * (*ndo_get_devlink_port)(struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct net_device_ops {
    int (*ndo_init)(struct net_device *);
    void (*ndo_uninit)(struct net_device *);
    int (*ndo_open)(struct net_device *);
    int (*ndo_stop)(struct net_device *);
    netdev_tx_t (*ndo_start_xmit)(struct sk_buff *, struct net_device *);
    netdev_features_t (*ndo_features_check)(struct sk_buff *, struct net_device *, netdev_features_t);
    u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, struct net_device *);
    void (*ndo_change_rx_flags)(struct net_device *, int);
    void (*ndo_set_rx_mode)(struct net_device *);
    int (*ndo_set_mac_address)(struct net_device *, void *);
    int (*ndo_validate_addr)(struct net_device *);
    int (*ndo_do_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_set_config)(struct net_device *, struct ifmap *);
    int (*ndo_change_mtu)(struct net_device *, int);
    int (*ndo_neigh_setup)(struct net_device *, struct neigh_parms *);
    void (*ndo_tx_timeout)(struct net_device *);
    void (*ndo_get_stats64)(struct net_device *, struct rtnl_link_stats64 *);
    bool (*ndo_has_offload_stats)(const struct net_device *, int);
    int (*ndo_get_offload_stats)(int, const struct net_device *, void *);
    struct net_device_stats * (*ndo_get_stats)(struct net_device *);
    int (*ndo_vlan_rx_add_vid)(struct net_device *, __be16, u16);
    int (*ndo_vlan_rx_kill_vid)(struct net_device *, __be16, u16);
    void (*ndo_poll_controller)(struct net_device *);
    int (*ndo_netpoll_setup)(struct net_device *, struct netpoll_info *);
    void (*ndo_netpoll_cleanup)(struct net_device *);
    int (*ndo_set_vf_mac)(struct net_device *, int, u8 *);
    int (*ndo_set_vf_vlan)(struct net_device *, int, u16, u8, __be16);
    int (*ndo_set_vf_rate)(struct net_device *, int, int, int);
    int (*ndo_set_vf_spoofchk)(struct net_device *, int, bool);
    int (*ndo_set_vf_trust)(struct net_device *, int, bool);
    int (*ndo_get_vf_config)(struct net_device *, int, struct ifla_vf_info *);
    int (*ndo_set_vf_link_state)(struct net_device *, int, int);
    int (*ndo_get_vf_stats)(struct net_device *, int, struct ifla_vf_stats *);
    int (*ndo_set_vf_port)(struct net_device *, int, struct nlattr **);
    int (*ndo_get_vf_port)(struct net_device *, int, struct sk_buff *);
    int (*ndo_set_vf_guid)(struct net_device *, int, u64, int);
    int (*ndo_set_vf_rss_query_en)(struct net_device *, int, bool);
    int (*ndo_setup_tc)(struct net_device *, enum tc_setup_type, void *);
    int (*ndo_rx_flow_steer)(struct net_device *, const struct sk_buff *, u16, u32);
    int (*ndo_add_slave)(struct net_device *, struct net_device *, struct netlink_ext_ack *);
    int (*ndo_del_slave)(struct net_device *, struct net_device *);
    netdev_features_t (*ndo_fix_features)(struct net_device *, netdev_features_t);
    int (*ndo_set_features)(struct net_device *, netdev_features_t);
    int (*ndo_neigh_construct)(struct net_device *, struct neighbour *);
    void (*ndo_neigh_destroy)(struct net_device *, struct neighbour *);
    int (*ndo_fdb_add)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, u16, struct netlink_ext_ack *);
    int (*ndo_fdb_del)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16);
    int (*ndo_fdb_dump)(struct sk_buff *, struct netlink_callback *, struct net_device *, struct net_device *, int *);
    int (*ndo_fdb_get)(struct sk_buff *, struct nlattr **, struct net_device *, const unsigned char *, u16, u32, u32, struct netlink_ext_ack *);
    int (*ndo_bridge_setlink)(struct net_device *, struct nlmsghdr *, u16, struct netlink_ext_ack *);
    int (*ndo_bridge_getlink)(struct sk_buff *, u32, u32, struct net_device *, u32, int);
    int (*ndo_bridge_dellink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_change_carrier)(struct net_device *, bool);
    int (*ndo_get_phys_port_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_port_parent_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_phys_port_name)(struct net_device *, char *, size_t);
    void (*ndo_udp_tunnel_add)(struct net_device *, struct udp_tunnel_info *);
    void (*ndo_udp_tunnel_del)(struct net_device *, struct udp_tunnel_info *);
    void * (*ndo_dfwd_add_station)(struct net_device *, struct net_device *);
    void (*ndo_dfwd_del_station)(struct net_device *, void *);
    int (*ndo_set_tx_maxrate)(struct net_device *, int, u32);
    int (*ndo_get_iflink)(const struct net_device *);
    int (*ndo_change_proto_down)(struct net_device *, bool);
    int (*ndo_fill_metadata_dst)(struct net_device *, struct sk_buff *);
    void (*ndo_set_rx_headroom)(struct net_device *, int);
    int (*ndo_bpf)(struct net_device *, struct netdev_bpf *);
    int (*ndo_xdp_xmit)(struct net_device *, int, struct xdp_frame **, u32);
    int (*ndo_xsk_wakeup)(struct net_device *, u32, u32);
    struct devlink_port * (*ndo_get_devlink_port)(struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct net_device_ops {
    int (*ndo_init)(struct net_device *);
    void (*ndo_uninit)(struct net_device *);
    int (*ndo_open)(struct net_device *);
    int (*ndo_stop)(struct net_device *);
    netdev_tx_t (*ndo_start_xmit)(struct sk_buff *, struct net_device *);
    netdev_features_t (*ndo_features_check)(struct sk_buff *, struct net_device *, netdev_features_t);
    u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, struct net_device *);
    void (*ndo_change_rx_flags)(struct net_device *, int);
    void (*ndo_set_rx_mode)(struct net_device *);
    int (*ndo_set_mac_address)(struct net_device *, void *);
    int (*ndo_validate_addr)(struct net_device *);
    int (*ndo_do_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_set_config)(struct net_device *, struct ifmap *);
    int (*ndo_change_mtu)(struct net_device *, int);
    int (*ndo_neigh_setup)(struct net_device *, struct neigh_parms *);
    void (*ndo_tx_timeout)(struct net_device *);
    void (*ndo_get_stats64)(struct net_device *, struct rtnl_link_stats64 *);
    bool (*ndo_has_offload_stats)(const struct net_device *, int);
    int (*ndo_get_offload_stats)(int, const struct net_device *, void *);
    struct net_device_stats * (*ndo_get_stats)(struct net_device *);
    int (*ndo_vlan_rx_add_vid)(struct net_device *, __be16, u16);
    int (*ndo_vlan_rx_kill_vid)(struct net_device *, __be16, u16);
    void (*ndo_poll_controller)(struct net_device *);
    int (*ndo_netpoll_setup)(struct net_device *, struct netpoll_info *);
    void (*ndo_netpoll_cleanup)(struct net_device *);
    int (*ndo_set_vf_mac)(struct net_device *, int, u8 *);
    int (*ndo_set_vf_vlan)(struct net_device *, int, u16, u8, __be16);
    int (*ndo_set_vf_rate)(struct net_device *, int, int, int);
    int (*ndo_set_vf_spoofchk)(struct net_device *, int, bool);
    int (*ndo_set_vf_trust)(struct net_device *, int, bool);
    int (*ndo_get_vf_config)(struct net_device *, int, struct ifla_vf_info *);
    int (*ndo_set_vf_link_state)(struct net_device *, int, int);
    int (*ndo_get_vf_stats)(struct net_device *, int, struct ifla_vf_stats *);
    int (*ndo_set_vf_port)(struct net_device *, int, struct nlattr **);
    int (*ndo_get_vf_port)(struct net_device *, int, struct sk_buff *);
    int (*ndo_set_vf_guid)(struct net_device *, int, u64, int);
    int (*ndo_set_vf_rss_query_en)(struct net_device *, int, bool);
    int (*ndo_setup_tc)(struct net_device *, enum tc_setup_type, void *);
    int (*ndo_fcoe_enable)(struct net_device *);
    int (*ndo_fcoe_disable)(struct net_device *);
    int (*ndo_fcoe_ddp_setup)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_ddp_done)(struct net_device *, u16);
    int (*ndo_fcoe_ddp_target)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_get_hbainfo)(struct net_device *, struct netdev_fcoe_hbainfo *);
    int (*ndo_fcoe_get_wwn)(struct net_device *, u64 *, int);
    int (*ndo_rx_flow_steer)(struct net_device *, const struct sk_buff *, u16, u32);
    int (*ndo_add_slave)(struct net_device *, struct net_device *, struct netlink_ext_ack *);
    int (*ndo_del_slave)(struct net_device *, struct net_device *);
    netdev_features_t (*ndo_fix_features)(struct net_device *, netdev_features_t);
    int (*ndo_set_features)(struct net_device *, netdev_features_t);
    int (*ndo_neigh_construct)(struct net_device *, struct neighbour *);
    void (*ndo_neigh_destroy)(struct net_device *, struct neighbour *);
    int (*ndo_fdb_add)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, u16, struct netlink_ext_ack *);
    int (*ndo_fdb_del)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16);
    int (*ndo_fdb_dump)(struct sk_buff *, struct netlink_callback *, struct net_device *, struct net_device *, int *);
    int (*ndo_fdb_get)(struct sk_buff *, struct nlattr **, struct net_device *, const unsigned char *, u16, u32, u32, struct netlink_ext_ack *);
    int (*ndo_bridge_setlink)(struct net_device *, struct nlmsghdr *, u16, struct netlink_ext_ack *);
    int (*ndo_bridge_getlink)(struct sk_buff *, u32, u32, struct net_device *, u32, int);
    int (*ndo_bridge_dellink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_change_carrier)(struct net_device *, bool);
    int (*ndo_get_phys_port_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_port_parent_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_phys_port_name)(struct net_device *, char *, size_t);
    void (*ndo_udp_tunnel_add)(struct net_device *, struct udp_tunnel_info *);
    void (*ndo_udp_tunnel_del)(struct net_device *, struct udp_tunnel_info *);
    void * (*ndo_dfwd_add_station)(struct net_device *, struct net_device *);
    void (*ndo_dfwd_del_station)(struct net_device *, void *);
    int (*ndo_set_tx_maxrate)(struct net_device *, int, u32);
    int (*ndo_get_iflink)(const struct net_device *);
    int (*ndo_change_proto_down)(struct net_device *, bool);
    int (*ndo_fill_metadata_dst)(struct net_device *, struct sk_buff *);
    void (*ndo_set_rx_headroom)(struct net_device *, int);
    int (*ndo_bpf)(struct net_device *, struct netdev_bpf *);
    int (*ndo_xdp_xmit)(struct net_device *, int, struct xdp_frame **, u32);
    int (*ndo_xsk_wakeup)(struct net_device *, u32, u32);
    struct devlink_port * (*ndo_get_devlink_port)(struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct net_device_ops {
    int (*ndo_init)(struct net_device *);
    void (*ndo_uninit)(struct net_device *);
    int (*ndo_open)(struct net_device *);
    int (*ndo_stop)(struct net_device *);
    netdev_tx_t (*ndo_start_xmit)(struct sk_buff *, struct net_device *);
    netdev_features_t (*ndo_features_check)(struct sk_buff *, struct net_device *, netdev_features_t);
    u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, struct net_device *);
    void (*ndo_change_rx_flags)(struct net_device *, int);
    void (*ndo_set_rx_mode)(struct net_device *);
    int (*ndo_set_mac_address)(struct net_device *, void *);
    int (*ndo_validate_addr)(struct net_device *);
    int (*ndo_do_ioctl)(struct net_device *, struct ifreq *, int);
    int (*ndo_set_config)(struct net_device *, struct ifmap *);
    int (*ndo_change_mtu)(struct net_device *, int);
    int (*ndo_neigh_setup)(struct net_device *, struct neigh_parms *);
    void (*ndo_tx_timeout)(struct net_device *);
    void (*ndo_get_stats64)(struct net_device *, struct rtnl_link_stats64 *);
    bool (*ndo_has_offload_stats)(const struct net_device *, int);
    int (*ndo_get_offload_stats)(int, const struct net_device *, void *);
    struct net_device_stats * (*ndo_get_stats)(struct net_device *);
    int (*ndo_vlan_rx_add_vid)(struct net_device *, __be16, u16);
    int (*ndo_vlan_rx_kill_vid)(struct net_device *, __be16, u16);
    void (*ndo_poll_controller)(struct net_device *);
    int (*ndo_netpoll_setup)(struct net_device *, struct netpoll_info *);
    void (*ndo_netpoll_cleanup)(struct net_device *);
    int (*ndo_set_vf_mac)(struct net_device *, int, u8 *);
    int (*ndo_set_vf_vlan)(struct net_device *, int, u16, u8, __be16);
    int (*ndo_set_vf_rate)(struct net_device *, int, int, int);
    int (*ndo_set_vf_spoofchk)(struct net_device *, int, bool);
    int (*ndo_set_vf_trust)(struct net_device *, int, bool);
    int (*ndo_get_vf_config)(struct net_device *, int, struct ifla_vf_info *);
    int (*ndo_set_vf_link_state)(struct net_device *, int, int);
    int (*ndo_get_vf_stats)(struct net_device *, int, struct ifla_vf_stats *);
    int (*ndo_set_vf_port)(struct net_device *, int, struct nlattr **);
    int (*ndo_get_vf_port)(struct net_device *, int, struct sk_buff *);
    int (*ndo_set_vf_guid)(struct net_device *, int, u64, int);
    int (*ndo_set_vf_rss_query_en)(struct net_device *, int, bool);
    int (*ndo_setup_tc)(struct net_device *, enum tc_setup_type, void *);
    int (*ndo_fcoe_enable)(struct net_device *);
    int (*ndo_fcoe_disable)(struct net_device *);
    int (*ndo_fcoe_ddp_setup)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_ddp_done)(struct net_device *, u16);
    int (*ndo_fcoe_ddp_target)(struct net_device *, u16, struct scatterlist *, unsigned int);
    int (*ndo_fcoe_get_hbainfo)(struct net_device *, struct netdev_fcoe_hbainfo *);
    int (*ndo_fcoe_get_wwn)(struct net_device *, u64 *, int);
    int (*ndo_rx_flow_steer)(struct net_device *, const struct sk_buff *, u16, u32);
    int (*ndo_add_slave)(struct net_device *, struct net_device *, struct netlink_ext_ack *);
    int (*ndo_del_slave)(struct net_device *, struct net_device *);
    netdev_features_t (*ndo_fix_features)(struct net_device *, netdev_features_t);
    int (*ndo_set_features)(struct net_device *, netdev_features_t);
    int (*ndo_neigh_construct)(struct net_device *, struct neighbour *);
    void (*ndo_neigh_destroy)(struct net_device *, struct neighbour *);
    int (*ndo_fdb_add)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, u16, struct netlink_ext_ack *);
    int (*ndo_fdb_del)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16);
    int (*ndo_fdb_dump)(struct sk_buff *, struct netlink_callback *, struct net_device *, struct net_device *, int *);
    int (*ndo_fdb_get)(struct sk_buff *, struct nlattr **, struct net_device *, const unsigned char *, u16, u32, u32, struct netlink_ext_ack *);
    int (*ndo_bridge_setlink)(struct net_device *, struct nlmsghdr *, u16, struct netlink_ext_ack *);
    int (*ndo_bridge_getlink)(struct sk_buff *, u32, u32, struct net_device *, u32, int);
    int (*ndo_bridge_dellink)(struct net_device *, struct nlmsghdr *, u16);
    int (*ndo_change_carrier)(struct net_device *, bool);
    int (*ndo_get_phys_port_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_port_parent_id)(struct net_device *, struct netdev_phys_item_id *);
    int (*ndo_get_phys_port_name)(struct net_device *, char *, size_t);
    void (*ndo_udp_tunnel_add)(struct net_device *, struct udp_tunnel_info *);
    void (*ndo_udp_tunnel_del)(struct net_device *, struct udp_tunnel_info *);
    void * (*ndo_dfwd_add_station)(struct net_device *, struct net_device *);
    void (*ndo_dfwd_del_station)(struct net_device *, void *);
    int (*ndo_set_tx_maxrate)(struct net_device *, int, u32);
    int (*ndo_get_iflink)(const struct net_device *);
    int (*ndo_change_proto_down)(struct net_device *, bool);
    int (*ndo_fill_metadata_dst)(struct net_device *, struct sk_buff *);
    void (*ndo_set_rx_headroom)(struct net_device *, int);
    int (*ndo_bpf)(struct net_device *, struct netdev_bpf *);
    int (*ndo_xdp_xmit)(struct net_device *, int, struct xdp_frame **, u32);
    int (*ndo_xsk_wakeup)(struct net_device *, u32, u32);
    struct devlink_port * (*ndo_get_devlink_port)(struct net_device *);
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*ndo_set_vf_guid)(struct net_device *, int, u64, int)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*ndo_udp_tunnel_add)(struct net_device *, struct udp_tunnel_info *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*ndo_udp_tunnel_del)(struct net_device *, struct udp_tunnel_info *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*ndo_set_rx_headroom)(struct net_device *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*ndo_xdp)(struct net_device *, struct netdev_xdp *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*ndo_add_vxlan_port)(struct net_device *, sa_family_t, __be16)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*ndo_del_vxlan_port)(struct net_device *, sa_family_t, __be16)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*ndo_add_geneve_port)(struct net_device *, sa_family_t, __be16)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*ndo_del_geneve_port)(struct net_device *, sa_family_t, __be16)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*ndo_neigh_construct)(struct neighbour *)</code> ➡️ <code>int (*ndo_neigh_construct)(struct net_device *, struct neighbour *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*ndo_neigh_destroy)(struct neighbour *)</code> ➡️ <code>void (*ndo_neigh_destroy)(struct net_device *, struct neighbour *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool (*ndo_has_offload_stats)(const struct net_device *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*ndo_get_offload_stats)(int, const struct net_device *, void *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*ndo_set_vf_vlan)(struct net_device *, int, u16, u8)</code> ➡️ <code>int (*ndo_set_vf_vlan)(struct net_device *, int, u16, u8, __be16)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*ndo_fdb_dump)(struct sk_buff *, struct netlink_callback *, struct net_device *, struct net_device *, int)</code> ➡️ <code>int (*ndo_fdb_dump)(struct sk_buff *, struct netlink_callback *, struct net_device *, struct net_device *, int *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*ndo_busy_poll)(struct napi_struct *)</code>
</li>
<li>
<b>Field removed. </b>
<code>netdev_tx_t (*ndo_dfwd_start_xmit)(struct sk_buff *, struct net_device *, void *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct rtnl_link_stats64 * (*ndo_get_stats64)(struct net_device *, struct rtnl_link_stats64 *)</code> ➡️ <code>void (*ndo_get_stats64)(struct net_device *, struct rtnl_link_stats64 *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*ndo_setup_tc)(struct net_device *, u32, __be16, struct tc_to_netdev *)</code> ➡️ <code>int (*ndo_setup_tc)(struct net_device *, u32, u32, __be16, struct tc_to_netdev *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*ndo_bpf)(struct net_device *, struct netdev_bpf *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*ndo_xdp_xmit)(struct net_device *, struct xdp_buff *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*ndo_xdp_flush)(struct net_device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*ndo_xdp)(struct net_device *, struct netdev_xdp *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*ndo_setup_tc)(struct net_device *, u32, u32, __be16, struct tc_to_netdev *)</code> ➡️ <code>int (*ndo_setup_tc)(struct net_device *, enum tc_setup_type, void *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*ndo_add_slave)(struct net_device *, struct net_device *)</code> ➡️ <code>int (*ndo_add_slave)(struct net_device *, struct net_device *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*ndo_udp_tunnel_add)(struct net_device *, struct udp_tunnel_info *)</code> ➡️ <code>void (*ndo_udp_tunnel_add)(struct net_device *, struct udp_tunnel_info *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*ndo_udp_tunnel_del)(struct net_device *, struct udp_tunnel_info *)</code> ➡️ <code>void (*ndo_udp_tunnel_del)(struct net_device *, struct udp_tunnel_info *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*ndo_xsk_async_xmit)(struct net_device *, u32)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*ndo_xdp_flush)(struct net_device *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*ndo_xdp_xmit)(struct net_device *, struct xdp_buff *)</code> ➡️ <code>int (*ndo_xdp_xmit)(struct net_device *, int, struct xdp_frame **, u32)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*ndo_fdb_get)(struct sk_buff *, struct nlattr **, struct net_device *, const unsigned char *, u16, u32, u32, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, void *, select_queue_fallback_t)</code> ➡️ <code>u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, struct net_device *, select_queue_fallback_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*ndo_bridge_setlink)(struct net_device *, struct nlmsghdr *, u16)</code> ➡️ <code>int (*ndo_bridge_setlink)(struct net_device *, struct nlmsghdr *, u16, struct netlink_ext_ack *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*ndo_get_port_parent_id)(struct net_device *, struct netdev_phys_item_id *)</code>
</li>
<li>
<b>Field added. </b>
<code>struct devlink_port * (*ndo_get_devlink_port)(struct net_device *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, struct net_device *, select_queue_fallback_t)</code> ➡️ <code>u16 (*ndo_select_queue)(struct net_device *, struct sk_buff *, struct net_device *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*ndo_fdb_add)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, u16)</code> ➡️ <code>int (*ndo_fdb_add)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, u16, struct netlink_ext_ack *)</code>
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
<code>int (*ndo_xsk_wakeup)(struct net_device *, u32, u32)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*ndo_get_lock_subclass)(struct net_device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*ndo_xsk_async_xmit)(struct net_device *, u32)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*ndo_get_vf_guid)(struct net_device *, int, struct ifla_vf_guid *, struct ifla_vf_guid *)</code>
</li>
<li>
<b>Field added. </b>
<code>struct net_device * (*ndo_get_xmit_slave)(struct net_device *, struct sk_buff *, bool)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*ndo_tunnel_ctl)(struct net_device *, struct ip_tunnel_parm *, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*ndo_tx_timeout)(struct net_device *)</code> ➡️ <code>void (*ndo_tx_timeout)(struct net_device *, unsigned int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct net_device * (*ndo_sk_get_lower_dev)(struct net_device *, struct sock *)</code>
</li>
<li>
<b>Field added. </b>
<code>struct net_device * (*ndo_get_peer_dev)(struct net_device *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*ndo_fill_forward_path)(struct net_device_path_ctx *, struct net_device_path *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*ndo_udp_tunnel_add)(struct net_device *, struct udp_tunnel_info *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*ndo_udp_tunnel_del)(struct net_device *, struct udp_tunnel_info *)</code>
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
<code>int (*ndo_eth_ioctl)(struct net_device *, struct ifreq *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*ndo_siocbond)(struct net_device *, struct ifreq *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*ndo_siocwandev)(struct net_device *, struct if_settings *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*ndo_siocdevprivate)(struct net_device *, struct ifreq *, void *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>struct net_device * (*ndo_xdp_get_xmit_slave)(struct net_device *, struct xdp_buff *)</code>
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
<code>int (*ndo_fdb_del_bulk)(struct ndmsg *, struct nlattr **, struct net_device *, u16, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>ktime_t (*ndo_get_tstamp)(struct net_device *, const struct skb_shared_hwtstamps *, bool)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*ndo_change_proto_down)(struct net_device *, bool)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*ndo_fdb_del)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16)</code> ➡️ <code>int (*ndo_fdb_del)(struct ndmsg *, struct nlattr **, struct net_device *, const unsigned char *, u16, struct netlink_ext_ack *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct devlink_port * (*ndo_get_devlink_port)(struct net_device *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*ndo_mdb_add)(struct net_device *, struct nlattr **, u16, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*ndo_mdb_del)(struct net_device *, struct nlattr **, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*ndo_mdb_dump)(struct net_device *, struct sk_buff *, struct netlink_callback *)</code>
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
<code>int (*ndo_mdb_del_bulk)(struct net_device *, struct nlattr **, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*ndo_mdb_get)(struct net_device *, struct nlattr **, u32, u32, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*ndo_hwtstamp_get)(struct net_device *, struct kernel_hwtstamp_config *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*ndo_hwtstamp_set)(struct net_device *, struct kernel_hwtstamp_config *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*ndo_fdb_del_bulk)(struct ndmsg *, struct nlattr **, struct net_device *, u16, struct netlink_ext_ack *)</code> ➡️ <code>int (*ndo_fdb_del_bulk)(struct nlmsghdr *, struct net_device *, struct netlink_ext_ack *)</code>
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
<details>
<summary>Changed between <code>generic</code> and <code>azure</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*ndo_fcoe_enable)(struct net_device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*ndo_fcoe_disable)(struct net_device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*ndo_fcoe_ddp_setup)(struct net_device *, u16, struct scatterlist *, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*ndo_fcoe_ddp_done)(struct net_device *, u16)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*ndo_fcoe_ddp_target)(struct net_device *, u16, struct scatterlist *, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*ndo_fcoe_get_hbainfo)(struct net_device *, struct netdev_fcoe_hbainfo *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*ndo_fcoe_get_wwn)(struct net_device *, u64 *, int)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
