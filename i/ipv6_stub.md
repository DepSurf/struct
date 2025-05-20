# Struct: <code>ipv6_stub</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct ipv6_stub {
    int (*ipv6_sock_mc_join)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_sock_mc_drop)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_dst_lookup)(struct net *, struct sock *, struct dst_entry **, struct flowi6 *);
    void (*udpv6_encap_enable)();
    void (*ndisc_send_na)(struct net_device *, const struct in6_addr *, const struct in6_addr *, bool, bool, bool, bool);
    struct neigh_table *nd_tbl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ipv6_stub {
    int (*ipv6_sock_mc_join)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_sock_mc_drop)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_dst_lookup)(struct net *, struct sock *, struct dst_entry **, struct flowi6 *);
    void (*udpv6_encap_enable)();
    void (*ndisc_send_na)(struct net_device *, const struct in6_addr *, const struct in6_addr *, bool, bool, bool, bool);
    struct neigh_table *nd_tbl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ipv6_stub {
    int (*ipv6_sock_mc_join)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_sock_mc_drop)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_dst_lookup)(struct net *, struct sock *, struct dst_entry **, struct flowi6 *);
    void (*udpv6_encap_enable)();
    void (*ndisc_send_na)(struct net_device *, const struct in6_addr *, const struct in6_addr *, bool, bool, bool, bool);
    struct neigh_table *nd_tbl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ipv6_stub {
    int (*ipv6_sock_mc_join)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_sock_mc_drop)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_dst_lookup)(struct net *, struct sock *, struct dst_entry **, struct flowi6 *);
    void (*udpv6_encap_enable)();
    void (*ndisc_send_na)(struct net_device *, const struct in6_addr *, const struct in6_addr *, bool, bool, bool, bool);
    struct neigh_table *nd_tbl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ipv6_stub {
    int (*ipv6_sock_mc_join)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_sock_mc_drop)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_dst_lookup)(struct net *, struct sock *, struct dst_entry **, struct flowi6 *);
    void (*udpv6_encap_enable)();
    void (*ndisc_send_na)(struct net_device *, const struct in6_addr *, const struct in6_addr *, bool, bool, bool, bool);
    struct neigh_table *nd_tbl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ipv6_stub {
    int (*ipv6_sock_mc_join)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_sock_mc_drop)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_dst_lookup)(struct net *, struct sock *, struct dst_entry **, struct flowi6 *);
    struct fib6_table * (*fib6_get_table)(struct net *, u32);
    struct fib6_info * (*fib6_lookup)(struct net *, int, struct flowi6 *, int);
    struct fib6_info * (*fib6_table_lookup)(struct net *, struct fib6_table *, int, struct flowi6 *, int);
    struct fib6_info * (*fib6_multipath_select)(const struct net *, struct fib6_info *, struct flowi6 *, int, const struct sk_buff *, int);
    u32 (*ip6_mtu_from_fib6)(struct fib6_info *, struct in6_addr *, struct in6_addr *);
    void (*udpv6_encap_enable)();
    void (*ndisc_send_na)(struct net_device *, const struct in6_addr *, const struct in6_addr *, bool, bool, bool, bool);
    struct neigh_table *nd_tbl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ipv6_stub {
    int (*ipv6_sock_mc_join)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_sock_mc_drop)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_dst_lookup)(struct net *, struct sock *, struct dst_entry **, struct flowi6 *);
    struct fib6_table * (*fib6_get_table)(struct net *, u32);
    struct fib6_info * (*fib6_lookup)(struct net *, int, struct flowi6 *, int);
    struct fib6_info * (*fib6_table_lookup)(struct net *, struct fib6_table *, int, struct flowi6 *, int);
    struct fib6_info * (*fib6_multipath_select)(const struct net *, struct fib6_info *, struct flowi6 *, int, const struct sk_buff *, int);
    u32 (*ip6_mtu_from_fib6)(struct fib6_info *, struct in6_addr *, struct in6_addr *);
    void (*udpv6_encap_enable)();
    void (*ndisc_send_na)(struct net_device *, const struct in6_addr *, const struct in6_addr *, bool, bool, bool, bool);
    struct neigh_table *nd_tbl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ipv6_stub {
    int (*ipv6_sock_mc_join)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_sock_mc_drop)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_dst_lookup)(struct net *, struct sock *, struct dst_entry **, struct flowi6 *);
    int (*ipv6_route_input)(struct sk_buff *);
    struct fib6_table * (*fib6_get_table)(struct net *, u32);
    int (*fib6_lookup)(struct net *, int, struct flowi6 *, struct fib6_result *, int);
    int (*fib6_table_lookup)(struct net *, struct fib6_table *, int, struct flowi6 *, struct fib6_result *, int);
    void (*fib6_select_path)(const struct net *, struct fib6_result *, struct flowi6 *, int, bool, const struct sk_buff *, int);
    u32 (*ip6_mtu_from_fib6)(const struct fib6_result *, const struct in6_addr *, const struct in6_addr *);
    int (*fib6_nh_init)(struct net *, struct fib6_nh *, struct fib6_config *, gfp_t, struct netlink_ext_ack *);
    void (*fib6_nh_release)(struct fib6_nh *);
    void (*fib6_update_sernum)(struct net *, struct fib6_info *);
    int (*ip6_del_rt)(struct net *, struct fib6_info *);
    void (*fib6_rt_update)(struct net *, struct fib6_info *, struct nl_info *);
    void (*udpv6_encap_enable)();
    void (*ndisc_send_na)(struct net_device *, const struct in6_addr *, const struct in6_addr *, bool, bool, bool, bool);
    struct neigh_table *nd_tbl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ipv6_stub {
    int (*ipv6_sock_mc_join)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_sock_mc_drop)(struct sock *, int, const struct in6_addr *);
    struct dst_entry * (*ipv6_dst_lookup_flow)(struct net *, const struct sock *, struct flowi6 *, const struct in6_addr *);
    int (*ipv6_route_input)(struct sk_buff *);
    struct fib6_table * (*fib6_get_table)(struct net *, u32);
    int (*fib6_lookup)(struct net *, int, struct flowi6 *, struct fib6_result *, int);
    int (*fib6_table_lookup)(struct net *, struct fib6_table *, int, struct flowi6 *, struct fib6_result *, int);
    void (*fib6_select_path)(const struct net *, struct fib6_result *, struct flowi6 *, int, bool, const struct sk_buff *, int);
    u32 (*ip6_mtu_from_fib6)(const struct fib6_result *, const struct in6_addr *, const struct in6_addr *);
    int (*fib6_nh_init)(struct net *, struct fib6_nh *, struct fib6_config *, gfp_t, struct netlink_ext_ack *);
    void (*fib6_nh_release)(struct fib6_nh *);
    void (*fib6_update_sernum)(struct net *, struct fib6_info *);
    int (*ip6_del_rt)(struct net *, struct fib6_info *);
    void (*fib6_rt_update)(struct net *, struct fib6_info *, struct nl_info *);
    void (*udpv6_encap_enable)();
    void (*ndisc_send_na)(struct net_device *, const struct in6_addr *, const struct in6_addr *, bool, bool, bool, bool);
    struct neigh_table *nd_tbl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ipv6_stub {
    int (*ipv6_sock_mc_join)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_sock_mc_drop)(struct sock *, int, const struct in6_addr *);
    struct dst_entry * (*ipv6_dst_lookup_flow)(struct net *, const struct sock *, struct flowi6 *, const struct in6_addr *);
    int (*ipv6_route_input)(struct sk_buff *);
    struct fib6_table * (*fib6_get_table)(struct net *, u32);
    int (*fib6_lookup)(struct net *, int, struct flowi6 *, struct fib6_result *, int);
    int (*fib6_table_lookup)(struct net *, struct fib6_table *, int, struct flowi6 *, struct fib6_result *, int);
    void (*fib6_select_path)(const struct net *, struct fib6_result *, struct flowi6 *, int, bool, const struct sk_buff *, int);
    u32 (*ip6_mtu_from_fib6)(const struct fib6_result *, const struct in6_addr *, const struct in6_addr *);
    int (*fib6_nh_init)(struct net *, struct fib6_nh *, struct fib6_config *, gfp_t, struct netlink_ext_ack *);
    void (*fib6_nh_release)(struct fib6_nh *);
    void (*fib6_update_sernum)(struct net *, struct fib6_info *);
    int (*ip6_del_rt)(struct net *, struct fib6_info *, bool);
    void (*fib6_rt_update)(struct net *, struct fib6_info *, struct nl_info *);
    void (*udpv6_encap_enable)();
    void (*ndisc_send_na)(struct net_device *, const struct in6_addr *, const struct in6_addr *, bool, bool, bool, bool);
    void (*xfrm6_local_rxpmtu)(struct sk_buff *, u32);
    int (*xfrm6_udp_encap_rcv)(struct sock *, struct sk_buff *);
    int (*xfrm6_rcv_encap)(struct sk_buff *, int, __be32, int);
    struct neigh_table *nd_tbl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ipv6_stub {
    int (*ipv6_sock_mc_join)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_sock_mc_drop)(struct sock *, int, const struct in6_addr *);
    struct dst_entry * (*ipv6_dst_lookup_flow)(struct net *, const struct sock *, struct flowi6 *, const struct in6_addr *);
    int (*ipv6_route_input)(struct sk_buff *);
    struct fib6_table * (*fib6_get_table)(struct net *, u32);
    int (*fib6_lookup)(struct net *, int, struct flowi6 *, struct fib6_result *, int);
    int (*fib6_table_lookup)(struct net *, struct fib6_table *, int, struct flowi6 *, struct fib6_result *, int);
    void (*fib6_select_path)(const struct net *, struct fib6_result *, struct flowi6 *, int, bool, const struct sk_buff *, int);
    u32 (*ip6_mtu_from_fib6)(const struct fib6_result *, const struct in6_addr *, const struct in6_addr *);
    int (*fib6_nh_init)(struct net *, struct fib6_nh *, struct fib6_config *, gfp_t, struct netlink_ext_ack *);
    void (*fib6_nh_release)(struct fib6_nh *);
    void (*fib6_update_sernum)(struct net *, struct fib6_info *);
    int (*ip6_del_rt)(struct net *, struct fib6_info *, bool);
    void (*fib6_rt_update)(struct net *, struct fib6_info *, struct nl_info *);
    void (*udpv6_encap_enable)();
    void (*ndisc_send_na)(struct net_device *, const struct in6_addr *, const struct in6_addr *, bool, bool, bool, bool);
    void (*xfrm6_local_rxpmtu)(struct sk_buff *, u32);
    int (*xfrm6_udp_encap_rcv)(struct sock *, struct sk_buff *);
    int (*xfrm6_rcv_encap)(struct sk_buff *, int, __be32, int);
    struct neigh_table *nd_tbl;
    int (*ipv6_fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ipv6_stub {
    int (*ipv6_sock_mc_join)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_sock_mc_drop)(struct sock *, int, const struct in6_addr *);
    struct dst_entry * (*ipv6_dst_lookup_flow)(struct net *, const struct sock *, struct flowi6 *, const struct in6_addr *);
    int (*ipv6_route_input)(struct sk_buff *);
    struct fib6_table * (*fib6_get_table)(struct net *, u32);
    int (*fib6_lookup)(struct net *, int, struct flowi6 *, struct fib6_result *, int);
    int (*fib6_table_lookup)(struct net *, struct fib6_table *, int, struct flowi6 *, struct fib6_result *, int);
    void (*fib6_select_path)(const struct net *, struct fib6_result *, struct flowi6 *, int, bool, const struct sk_buff *, int);
    u32 (*ip6_mtu_from_fib6)(const struct fib6_result *, const struct in6_addr *, const struct in6_addr *);
    int (*fib6_nh_init)(struct net *, struct fib6_nh *, struct fib6_config *, gfp_t, struct netlink_ext_ack *);
    void (*fib6_nh_release)(struct fib6_nh *);
    void (*fib6_update_sernum)(struct net *, struct fib6_info *);
    int (*ip6_del_rt)(struct net *, struct fib6_info *, bool);
    void (*fib6_rt_update)(struct net *, struct fib6_info *, struct nl_info *);
    void (*udpv6_encap_enable)();
    void (*ndisc_send_na)(struct net_device *, const struct in6_addr *, const struct in6_addr *, bool, bool, bool, bool);
    void (*xfrm6_local_rxpmtu)(struct sk_buff *, u32);
    int (*xfrm6_udp_encap_rcv)(struct sock *, struct sk_buff *);
    int (*xfrm6_rcv_encap)(struct sk_buff *, int, __be32, int);
    struct neigh_table *nd_tbl;
    int (*ipv6_fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
    struct net_device * (*ipv6_dev_find)(struct net *, const struct in6_addr *, struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ipv6_stub {
    int (*ipv6_sock_mc_join)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_sock_mc_drop)(struct sock *, int, const struct in6_addr *);
    struct dst_entry * (*ipv6_dst_lookup_flow)(struct net *, const struct sock *, struct flowi6 *, const struct in6_addr *);
    int (*ipv6_route_input)(struct sk_buff *);
    struct fib6_table * (*fib6_get_table)(struct net *, u32);
    int (*fib6_lookup)(struct net *, int, struct flowi6 *, struct fib6_result *, int);
    int (*fib6_table_lookup)(struct net *, struct fib6_table *, int, struct flowi6 *, struct fib6_result *, int);
    void (*fib6_select_path)(const struct net *, struct fib6_result *, struct flowi6 *, int, bool, const struct sk_buff *, int);
    u32 (*ip6_mtu_from_fib6)(const struct fib6_result *, const struct in6_addr *, const struct in6_addr *);
    int (*fib6_nh_init)(struct net *, struct fib6_nh *, struct fib6_config *, gfp_t, struct netlink_ext_ack *);
    void (*fib6_nh_release)(struct fib6_nh *);
    void (*fib6_nh_release_dsts)(struct fib6_nh *);
    void (*fib6_update_sernum)(struct net *, struct fib6_info *);
    int (*ip6_del_rt)(struct net *, struct fib6_info *, bool);
    void (*fib6_rt_update)(struct net *, struct fib6_info *, struct nl_info *);
    void (*udpv6_encap_enable)();
    void (*ndisc_send_na)(struct net_device *, const struct in6_addr *, const struct in6_addr *, bool, bool, bool, bool);
    void (*xfrm6_local_rxpmtu)(struct sk_buff *, u32);
    int (*xfrm6_udp_encap_rcv)(struct sock *, struct sk_buff *);
    int (*xfrm6_rcv_encap)(struct sk_buff *, int, __be32, int);
    struct neigh_table *nd_tbl;
    int (*ipv6_fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
    struct net_device * (*ipv6_dev_find)(struct net *, const struct in6_addr *, struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ipv6_stub {
    int (*ipv6_sock_mc_join)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_sock_mc_drop)(struct sock *, int, const struct in6_addr *);
    struct dst_entry * (*ipv6_dst_lookup_flow)(struct net *, const struct sock *, struct flowi6 *, const struct in6_addr *);
    int (*ipv6_route_input)(struct sk_buff *);
    struct fib6_table * (*fib6_get_table)(struct net *, u32);
    int (*fib6_lookup)(struct net *, int, struct flowi6 *, struct fib6_result *, int);
    int (*fib6_table_lookup)(struct net *, struct fib6_table *, int, struct flowi6 *, struct fib6_result *, int);
    void (*fib6_select_path)(const struct net *, struct fib6_result *, struct flowi6 *, int, bool, const struct sk_buff *, int);
    u32 (*ip6_mtu_from_fib6)(const struct fib6_result *, const struct in6_addr *, const struct in6_addr *);
    int (*fib6_nh_init)(struct net *, struct fib6_nh *, struct fib6_config *, gfp_t, struct netlink_ext_ack *);
    void (*fib6_nh_release)(struct fib6_nh *);
    void (*fib6_nh_release_dsts)(struct fib6_nh *);
    void (*fib6_update_sernum)(struct net *, struct fib6_info *);
    int (*ip6_del_rt)(struct net *, struct fib6_info *, bool);
    void (*fib6_rt_update)(struct net *, struct fib6_info *, struct nl_info *);
    void (*udpv6_encap_enable)();
    void (*ndisc_send_na)(struct net_device *, const struct in6_addr *, const struct in6_addr *, bool, bool, bool, bool);
    void (*xfrm6_local_rxpmtu)(struct sk_buff *, u32);
    int (*xfrm6_udp_encap_rcv)(struct sock *, struct sk_buff *);
    int (*xfrm6_rcv_encap)(struct sk_buff *, int, __be32, int);
    struct neigh_table *nd_tbl;
    int (*ipv6_fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
    struct net_device * (*ipv6_dev_find)(struct net *, const struct in6_addr *, struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ipv6_stub {
    int (*ipv6_sock_mc_join)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_sock_mc_drop)(struct sock *, int, const struct in6_addr *);
    struct dst_entry * (*ipv6_dst_lookup_flow)(struct net *, const struct sock *, struct flowi6 *, const struct in6_addr *);
    int (*ipv6_route_input)(struct sk_buff *);
    struct fib6_table * (*fib6_get_table)(struct net *, u32);
    int (*fib6_lookup)(struct net *, int, struct flowi6 *, struct fib6_result *, int);
    int (*fib6_table_lookup)(struct net *, struct fib6_table *, int, struct flowi6 *, struct fib6_result *, int);
    void (*fib6_select_path)(const struct net *, struct fib6_result *, struct flowi6 *, int, bool, const struct sk_buff *, int);
    u32 (*ip6_mtu_from_fib6)(const struct fib6_result *, const struct in6_addr *, const struct in6_addr *);
    int (*fib6_nh_init)(struct net *, struct fib6_nh *, struct fib6_config *, gfp_t, struct netlink_ext_ack *);
    void (*fib6_nh_release)(struct fib6_nh *);
    void (*fib6_nh_release_dsts)(struct fib6_nh *);
    void (*fib6_update_sernum)(struct net *, struct fib6_info *);
    int (*ip6_del_rt)(struct net *, struct fib6_info *, bool);
    void (*fib6_rt_update)(struct net *, struct fib6_info *, struct nl_info *);
    void (*udpv6_encap_enable)();
    void (*ndisc_send_na)(struct net_device *, const struct in6_addr *, const struct in6_addr *, bool, bool, bool, bool);
    void (*xfrm6_local_rxpmtu)(struct sk_buff *, u32);
    int (*xfrm6_udp_encap_rcv)(struct sock *, struct sk_buff *);
    int (*xfrm6_rcv_encap)(struct sk_buff *, int, __be32, int);
    struct neigh_table *nd_tbl;
    int (*ipv6_fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
    struct net_device * (*ipv6_dev_find)(struct net *, const struct in6_addr *, struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ipv6_stub {
    int (*ipv6_sock_mc_join)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_sock_mc_drop)(struct sock *, int, const struct in6_addr *);
    struct dst_entry * (*ipv6_dst_lookup_flow)(struct net *, const struct sock *, struct flowi6 *, const struct in6_addr *);
    int (*ipv6_route_input)(struct sk_buff *);
    struct fib6_table * (*fib6_get_table)(struct net *, u32);
    int (*fib6_lookup)(struct net *, int, struct flowi6 *, struct fib6_result *, int);
    int (*fib6_table_lookup)(struct net *, struct fib6_table *, int, struct flowi6 *, struct fib6_result *, int);
    void (*fib6_select_path)(const struct net *, struct fib6_result *, struct flowi6 *, int, bool, const struct sk_buff *, int);
    u32 (*ip6_mtu_from_fib6)(const struct fib6_result *, const struct in6_addr *, const struct in6_addr *);
    int (*fib6_nh_init)(struct net *, struct fib6_nh *, struct fib6_config *, gfp_t, struct netlink_ext_ack *);
    void (*fib6_nh_release)(struct fib6_nh *);
    void (*fib6_nh_release_dsts)(struct fib6_nh *);
    void (*fib6_update_sernum)(struct net *, struct fib6_info *);
    int (*ip6_del_rt)(struct net *, struct fib6_info *, bool);
    void (*fib6_rt_update)(struct net *, struct fib6_info *, struct nl_info *);
    void (*udpv6_encap_enable)();
    void (*ndisc_send_na)(struct net_device *, const struct in6_addr *, const struct in6_addr *, bool, bool, bool, bool);
    void (*xfrm6_local_rxpmtu)(struct sk_buff *, u32);
    int (*xfrm6_udp_encap_rcv)(struct sock *, struct sk_buff *);
    int (*xfrm6_rcv_encap)(struct sk_buff *, int, __be32, int);
    struct neigh_table *nd_tbl;
    int (*ipv6_fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
    struct net_device * (*ipv6_dev_find)(struct net *, const struct in6_addr *, struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ipv6_stub {
    int (*ipv6_sock_mc_join)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_sock_mc_drop)(struct sock *, int, const struct in6_addr *);
    struct dst_entry * (*ipv6_dst_lookup_flow)(struct net *, const struct sock *, struct flowi6 *, const struct in6_addr *);
    int (*ipv6_route_input)(struct sk_buff *);
    struct fib6_table * (*fib6_get_table)(struct net *, u32);
    int (*fib6_lookup)(struct net *, int, struct flowi6 *, struct fib6_result *, int);
    int (*fib6_table_lookup)(struct net *, struct fib6_table *, int, struct flowi6 *, struct fib6_result *, int);
    void (*fib6_select_path)(const struct net *, struct fib6_result *, struct flowi6 *, int, bool, const struct sk_buff *, int);
    u32 (*ip6_mtu_from_fib6)(const struct fib6_result *, const struct in6_addr *, const struct in6_addr *);
    int (*fib6_nh_init)(struct net *, struct fib6_nh *, struct fib6_config *, gfp_t, struct netlink_ext_ack *);
    void (*fib6_nh_release)(struct fib6_nh *);
    void (*fib6_nh_release_dsts)(struct fib6_nh *);
    void (*fib6_update_sernum)(struct net *, struct fib6_info *);
    int (*ip6_del_rt)(struct net *, struct fib6_info *, bool);
    void (*fib6_rt_update)(struct net *, struct fib6_info *, struct nl_info *);
    void (*udpv6_encap_enable)();
    void (*ndisc_send_na)(struct net_device *, const struct in6_addr *, const struct in6_addr *, bool, bool, bool, bool);
    void (*xfrm6_local_rxpmtu)(struct sk_buff *, u32);
    int (*xfrm6_udp_encap_rcv)(struct sock *, struct sk_buff *);
    struct sk_buff * (*xfrm6_gro_udp_encap_rcv)(struct sock *, struct list_head *, struct sk_buff *);
    int (*xfrm6_rcv_encap)(struct sk_buff *, int, __be32, int);
    struct neigh_table *nd_tbl;
    int (*ipv6_fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *));
    struct net_device * (*ipv6_dev_find)(struct net *, const struct in6_addr *, struct net_device *);
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
struct ipv6_stub {
    int (*ipv6_sock_mc_join)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_sock_mc_drop)(struct sock *, int, const struct in6_addr *);
    struct dst_entry * (*ipv6_dst_lookup_flow)(struct net *, const struct sock *, struct flowi6 *, const struct in6_addr *);
    int (*ipv6_route_input)(struct sk_buff *);
    struct fib6_table * (*fib6_get_table)(struct net *, u32);
    int (*fib6_lookup)(struct net *, int, struct flowi6 *, struct fib6_result *, int);
    int (*fib6_table_lookup)(struct net *, struct fib6_table *, int, struct flowi6 *, struct fib6_result *, int);
    void (*fib6_select_path)(const struct net *, struct fib6_result *, struct flowi6 *, int, bool, const struct sk_buff *, int);
    u32 (*ip6_mtu_from_fib6)(const struct fib6_result *, const struct in6_addr *, const struct in6_addr *);
    int (*fib6_nh_init)(struct net *, struct fib6_nh *, struct fib6_config *, gfp_t, struct netlink_ext_ack *);
    void (*fib6_nh_release)(struct fib6_nh *);
    void (*fib6_update_sernum)(struct net *, struct fib6_info *);
    int (*ip6_del_rt)(struct net *, struct fib6_info *);
    void (*fib6_rt_update)(struct net *, struct fib6_info *, struct nl_info *);
    void (*udpv6_encap_enable)();
    void (*ndisc_send_na)(struct net_device *, const struct in6_addr *, const struct in6_addr *, bool, bool, bool, bool);
    struct neigh_table *nd_tbl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ipv6_stub {
    int (*ipv6_sock_mc_join)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_sock_mc_drop)(struct sock *, int, const struct in6_addr *);
    struct dst_entry * (*ipv6_dst_lookup_flow)(struct net *, const struct sock *, struct flowi6 *, const struct in6_addr *);
    int (*ipv6_route_input)(struct sk_buff *);
    struct fib6_table * (*fib6_get_table)(struct net *, u32);
    int (*fib6_lookup)(struct net *, int, struct flowi6 *, struct fib6_result *, int);
    int (*fib6_table_lookup)(struct net *, struct fib6_table *, int, struct flowi6 *, struct fib6_result *, int);
    void (*fib6_select_path)(const struct net *, struct fib6_result *, struct flowi6 *, int, bool, const struct sk_buff *, int);
    u32 (*ip6_mtu_from_fib6)(const struct fib6_result *, const struct in6_addr *, const struct in6_addr *);
    int (*fib6_nh_init)(struct net *, struct fib6_nh *, struct fib6_config *, gfp_t, struct netlink_ext_ack *);
    void (*fib6_nh_release)(struct fib6_nh *);
    void (*fib6_update_sernum)(struct net *, struct fib6_info *);
    int (*ip6_del_rt)(struct net *, struct fib6_info *);
    void (*fib6_rt_update)(struct net *, struct fib6_info *, struct nl_info *);
    void (*udpv6_encap_enable)();
    void (*ndisc_send_na)(struct net_device *, const struct in6_addr *, const struct in6_addr *, bool, bool, bool, bool);
    struct neigh_table *nd_tbl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ipv6_stub {
    int (*ipv6_sock_mc_join)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_sock_mc_drop)(struct sock *, int, const struct in6_addr *);
    struct dst_entry * (*ipv6_dst_lookup_flow)(struct net *, const struct sock *, struct flowi6 *, const struct in6_addr *);
    int (*ipv6_route_input)(struct sk_buff *);
    struct fib6_table * (*fib6_get_table)(struct net *, u32);
    int (*fib6_lookup)(struct net *, int, struct flowi6 *, struct fib6_result *, int);
    int (*fib6_table_lookup)(struct net *, struct fib6_table *, int, struct flowi6 *, struct fib6_result *, int);
    void (*fib6_select_path)(const struct net *, struct fib6_result *, struct flowi6 *, int, bool, const struct sk_buff *, int);
    u32 (*ip6_mtu_from_fib6)(const struct fib6_result *, const struct in6_addr *, const struct in6_addr *);
    int (*fib6_nh_init)(struct net *, struct fib6_nh *, struct fib6_config *, gfp_t, struct netlink_ext_ack *);
    void (*fib6_nh_release)(struct fib6_nh *);
    void (*fib6_update_sernum)(struct net *, struct fib6_info *);
    int (*ip6_del_rt)(struct net *, struct fib6_info *);
    void (*fib6_rt_update)(struct net *, struct fib6_info *, struct nl_info *);
    void (*udpv6_encap_enable)();
    void (*ndisc_send_na)(struct net_device *, const struct in6_addr *, const struct in6_addr *, bool, bool, bool, bool);
    struct neigh_table *nd_tbl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ipv6_stub {
    int (*ipv6_sock_mc_join)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_sock_mc_drop)(struct sock *, int, const struct in6_addr *);
    struct dst_entry * (*ipv6_dst_lookup_flow)(struct net *, const struct sock *, struct flowi6 *, const struct in6_addr *);
    int (*ipv6_route_input)(struct sk_buff *);
    struct fib6_table * (*fib6_get_table)(struct net *, u32);
    int (*fib6_lookup)(struct net *, int, struct flowi6 *, struct fib6_result *, int);
    int (*fib6_table_lookup)(struct net *, struct fib6_table *, int, struct flowi6 *, struct fib6_result *, int);
    void (*fib6_select_path)(const struct net *, struct fib6_result *, struct flowi6 *, int, bool, const struct sk_buff *, int);
    u32 (*ip6_mtu_from_fib6)(const struct fib6_result *, const struct in6_addr *, const struct in6_addr *);
    int (*fib6_nh_init)(struct net *, struct fib6_nh *, struct fib6_config *, gfp_t, struct netlink_ext_ack *);
    void (*fib6_nh_release)(struct fib6_nh *);
    void (*fib6_update_sernum)(struct net *, struct fib6_info *);
    int (*ip6_del_rt)(struct net *, struct fib6_info *);
    void (*fib6_rt_update)(struct net *, struct fib6_info *, struct nl_info *);
    void (*udpv6_encap_enable)();
    void (*ndisc_send_na)(struct net_device *, const struct in6_addr *, const struct in6_addr *, bool, bool, bool, bool);
    struct neigh_table *nd_tbl;
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
struct ipv6_stub {
    int (*ipv6_sock_mc_join)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_sock_mc_drop)(struct sock *, int, const struct in6_addr *);
    struct dst_entry * (*ipv6_dst_lookup_flow)(struct net *, const struct sock *, struct flowi6 *, const struct in6_addr *);
    int (*ipv6_route_input)(struct sk_buff *);
    struct fib6_table * (*fib6_get_table)(struct net *, u32);
    int (*fib6_lookup)(struct net *, int, struct flowi6 *, struct fib6_result *, int);
    int (*fib6_table_lookup)(struct net *, struct fib6_table *, int, struct flowi6 *, struct fib6_result *, int);
    void (*fib6_select_path)(const struct net *, struct fib6_result *, struct flowi6 *, int, bool, const struct sk_buff *, int);
    u32 (*ip6_mtu_from_fib6)(const struct fib6_result *, const struct in6_addr *, const struct in6_addr *);
    int (*fib6_nh_init)(struct net *, struct fib6_nh *, struct fib6_config *, gfp_t, struct netlink_ext_ack *);
    void (*fib6_nh_release)(struct fib6_nh *);
    void (*fib6_update_sernum)(struct net *, struct fib6_info *);
    int (*ip6_del_rt)(struct net *, struct fib6_info *);
    void (*fib6_rt_update)(struct net *, struct fib6_info *, struct nl_info *);
    void (*udpv6_encap_enable)();
    void (*ndisc_send_na)(struct net_device *, const struct in6_addr *, const struct in6_addr *, bool, bool, bool, bool);
    struct neigh_table *nd_tbl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ipv6_stub {
    int (*ipv6_sock_mc_join)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_sock_mc_drop)(struct sock *, int, const struct in6_addr *);
    struct dst_entry * (*ipv6_dst_lookup_flow)(struct net *, const struct sock *, struct flowi6 *, const struct in6_addr *);
    int (*ipv6_route_input)(struct sk_buff *);
    struct fib6_table * (*fib6_get_table)(struct net *, u32);
    int (*fib6_lookup)(struct net *, int, struct flowi6 *, struct fib6_result *, int);
    int (*fib6_table_lookup)(struct net *, struct fib6_table *, int, struct flowi6 *, struct fib6_result *, int);
    void (*fib6_select_path)(const struct net *, struct fib6_result *, struct flowi6 *, int, bool, const struct sk_buff *, int);
    u32 (*ip6_mtu_from_fib6)(const struct fib6_result *, const struct in6_addr *, const struct in6_addr *);
    int (*fib6_nh_init)(struct net *, struct fib6_nh *, struct fib6_config *, gfp_t, struct netlink_ext_ack *);
    void (*fib6_nh_release)(struct fib6_nh *);
    void (*fib6_update_sernum)(struct net *, struct fib6_info *);
    int (*ip6_del_rt)(struct net *, struct fib6_info *);
    void (*fib6_rt_update)(struct net *, struct fib6_info *, struct nl_info *);
    void (*udpv6_encap_enable)();
    void (*ndisc_send_na)(struct net_device *, const struct in6_addr *, const struct in6_addr *, bool, bool, bool, bool);
    struct neigh_table *nd_tbl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ipv6_stub {
    int (*ipv6_sock_mc_join)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_sock_mc_drop)(struct sock *, int, const struct in6_addr *);
    struct dst_entry * (*ipv6_dst_lookup_flow)(struct net *, const struct sock *, struct flowi6 *, const struct in6_addr *);
    int (*ipv6_route_input)(struct sk_buff *);
    struct fib6_table * (*fib6_get_table)(struct net *, u32);
    int (*fib6_lookup)(struct net *, int, struct flowi6 *, struct fib6_result *, int);
    int (*fib6_table_lookup)(struct net *, struct fib6_table *, int, struct flowi6 *, struct fib6_result *, int);
    void (*fib6_select_path)(const struct net *, struct fib6_result *, struct flowi6 *, int, bool, const struct sk_buff *, int);
    u32 (*ip6_mtu_from_fib6)(const struct fib6_result *, const struct in6_addr *, const struct in6_addr *);
    int (*fib6_nh_init)(struct net *, struct fib6_nh *, struct fib6_config *, gfp_t, struct netlink_ext_ack *);
    void (*fib6_nh_release)(struct fib6_nh *);
    void (*fib6_update_sernum)(struct net *, struct fib6_info *);
    int (*ip6_del_rt)(struct net *, struct fib6_info *);
    void (*fib6_rt_update)(struct net *, struct fib6_info *, struct nl_info *);
    void (*udpv6_encap_enable)();
    void (*ndisc_send_na)(struct net_device *, const struct in6_addr *, const struct in6_addr *, bool, bool, bool, bool);
    struct neigh_table *nd_tbl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ipv6_stub {
    int (*ipv6_sock_mc_join)(struct sock *, int, const struct in6_addr *);
    int (*ipv6_sock_mc_drop)(struct sock *, int, const struct in6_addr *);
    struct dst_entry * (*ipv6_dst_lookup_flow)(struct net *, const struct sock *, struct flowi6 *, const struct in6_addr *);
    int (*ipv6_route_input)(struct sk_buff *);
    struct fib6_table * (*fib6_get_table)(struct net *, u32);
    int (*fib6_lookup)(struct net *, int, struct flowi6 *, struct fib6_result *, int);
    int (*fib6_table_lookup)(struct net *, struct fib6_table *, int, struct flowi6 *, struct fib6_result *, int);
    void (*fib6_select_path)(const struct net *, struct fib6_result *, struct flowi6 *, int, bool, const struct sk_buff *, int);
    u32 (*ip6_mtu_from_fib6)(const struct fib6_result *, const struct in6_addr *, const struct in6_addr *);
    int (*fib6_nh_init)(struct net *, struct fib6_nh *, struct fib6_config *, gfp_t, struct netlink_ext_ack *);
    void (*fib6_nh_release)(struct fib6_nh *);
    void (*fib6_update_sernum)(struct net *, struct fib6_info *);
    int (*ip6_del_rt)(struct net *, struct fib6_info *);
    void (*fib6_rt_update)(struct net *, struct fib6_info *, struct nl_info *);
    void (*udpv6_encap_enable)();
    void (*ndisc_send_na)(struct net_device *, const struct in6_addr *, const struct in6_addr *, bool, bool, bool, bool);
    struct neigh_table *nd_tbl;
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
<code>struct fib6_table * (*fib6_get_table)(struct net *, u32)</code>
</li>
<li>
<b>Field added. </b>
<code>struct fib6_info * (*fib6_lookup)(struct net *, int, struct flowi6 *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>struct fib6_info * (*fib6_table_lookup)(struct net *, struct fib6_table *, int, struct flowi6 *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>struct fib6_info * (*fib6_multipath_select)(const struct net *, struct fib6_info *, struct flowi6 *, int, const struct sk_buff *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>u32 (*ip6_mtu_from_fib6)(struct fib6_info *, struct in6_addr *, struct in6_addr *)</code>
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
<code>int (*ipv6_route_input)(struct sk_buff *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*fib6_select_path)(const struct net *, struct fib6_result *, struct flowi6 *, int, bool, const struct sk_buff *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*fib6_nh_init)(struct net *, struct fib6_nh *, struct fib6_config *, gfp_t, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*fib6_nh_release)(struct fib6_nh *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*fib6_update_sernum)(struct net *, struct fib6_info *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*ip6_del_rt)(struct net *, struct fib6_info *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*fib6_rt_update)(struct net *, struct fib6_info *, struct nl_info *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct fib6_info * (*fib6_multipath_select)(const struct net *, struct fib6_info *, struct flowi6 *, int, const struct sk_buff *, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct fib6_info * (*fib6_lookup)(struct net *, int, struct flowi6 *, int)</code> ➡️ <code>int (*fib6_lookup)(struct net *, int, struct flowi6 *, struct fib6_result *, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct fib6_info * (*fib6_table_lookup)(struct net *, struct fib6_table *, int, struct flowi6 *, int)</code> ➡️ <code>int (*fib6_table_lookup)(struct net *, struct fib6_table *, int, struct flowi6 *, struct fib6_result *, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 (*ip6_mtu_from_fib6)(struct fib6_info *, struct in6_addr *, struct in6_addr *)</code> ➡️ <code>u32 (*ip6_mtu_from_fib6)(const struct fib6_result *, const struct in6_addr *, const struct in6_addr *)</code>
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
<code>struct dst_entry * (*ipv6_dst_lookup_flow)(struct net *, const struct sock *, struct flowi6 *, const struct in6_addr *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*ipv6_dst_lookup)(struct net *, struct sock *, struct dst_entry **, struct flowi6 *)</code>
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
<code>void (*xfrm6_local_rxpmtu)(struct sk_buff *, u32)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*xfrm6_udp_encap_rcv)(struct sock *, struct sk_buff *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*xfrm6_rcv_encap)(struct sk_buff *, int, __be32, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*ip6_del_rt)(struct net *, struct fib6_info *)</code> ➡️ <code>int (*ip6_del_rt)(struct net *, struct fib6_info *, bool)</code>
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
<code>int (*ipv6_fragment)(struct net *, struct sock *, struct sk_buff *, int(*)(struct net *, struct sock *, struct sk_buff *))</code>
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
<code>struct net_device * (*ipv6_dev_find)(struct net *, const struct in6_addr *, struct net_device *)</code>
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
<code>void (*fib6_nh_release_dsts)(struct fib6_nh *)</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct sk_buff * (*xfrm6_gro_udp_encap_rcv)(struct sock *, struct list_head *, struct sk_buff *)</code>
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
