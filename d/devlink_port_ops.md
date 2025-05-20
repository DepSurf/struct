# Struct: <code>devlink_port_ops</code>

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
In <code>6.2</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct devlink_port_ops {
    int (*port_split)(struct devlink *, struct devlink_port *, unsigned int, struct netlink_ext_ack *);
    int (*port_unsplit)(struct devlink *, struct devlink_port *, struct netlink_ext_ack *);
    int (*port_type_set)(struct devlink_port *, enum devlink_port_type);
    int (*port_del)(struct devlink *, struct devlink_port *, struct netlink_ext_ack *);
    int (*port_fn_hw_addr_get)(struct devlink_port *, u8 *, int *, struct netlink_ext_ack *);
    int (*port_fn_hw_addr_set)(struct devlink_port *, const u8 *, int, struct netlink_ext_ack *);
    int (*port_fn_roce_get)(struct devlink_port *, bool *, struct netlink_ext_ack *);
    int (*port_fn_roce_set)(struct devlink_port *, bool, struct netlink_ext_ack *);
    int (*port_fn_migratable_get)(struct devlink_port *, bool *, struct netlink_ext_ack *);
    int (*port_fn_migratable_set)(struct devlink_port *, bool, struct netlink_ext_ack *);
    int (*port_fn_state_get)(struct devlink_port *, enum devlink_port_fn_state *, enum devlink_port_fn_opstate *, struct netlink_ext_ack *);
    int (*port_fn_state_set)(struct devlink_port *, enum devlink_port_fn_state, struct netlink_ext_ack *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct devlink_port_ops {
    int (*port_split)(struct devlink *, struct devlink_port *, unsigned int, struct netlink_ext_ack *);
    int (*port_unsplit)(struct devlink *, struct devlink_port *, struct netlink_ext_ack *);
    int (*port_type_set)(struct devlink_port *, enum devlink_port_type);
    int (*port_del)(struct devlink *, struct devlink_port *, struct netlink_ext_ack *);
    int (*port_fn_hw_addr_get)(struct devlink_port *, u8 *, int *, struct netlink_ext_ack *);
    int (*port_fn_hw_addr_set)(struct devlink_port *, const u8 *, int, struct netlink_ext_ack *);
    int (*port_fn_roce_get)(struct devlink_port *, bool *, struct netlink_ext_ack *);
    int (*port_fn_roce_set)(struct devlink_port *, bool, struct netlink_ext_ack *);
    int (*port_fn_migratable_get)(struct devlink_port *, bool *, struct netlink_ext_ack *);
    int (*port_fn_migratable_set)(struct devlink_port *, bool, struct netlink_ext_ack *);
    int (*port_fn_state_get)(struct devlink_port *, enum devlink_port_fn_state *, enum devlink_port_fn_opstate *, struct netlink_ext_ack *);
    int (*port_fn_state_set)(struct devlink_port *, enum devlink_port_fn_state, struct netlink_ext_ack *);
    int (*port_fn_ipsec_crypto_get)(struct devlink_port *, bool *, struct netlink_ext_ack *);
    int (*port_fn_ipsec_crypto_set)(struct devlink_port *, bool, struct netlink_ext_ack *);
    int (*port_fn_ipsec_packet_get)(struct devlink_port *, bool *, struct netlink_ext_ack *);
    int (*port_fn_ipsec_packet_set)(struct devlink_port *, bool, struct netlink_ext_ack *);
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
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*port_fn_ipsec_crypto_get)(struct devlink_port *, bool *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_fn_ipsec_crypto_set)(struct devlink_port *, bool, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_fn_ipsec_packet_get)(struct devlink_port *, bool *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_fn_ipsec_packet_set)(struct devlink_port *, bool, struct netlink_ext_ack *)</code>
</li>
</ul>
</details>
</li>
</ul>
