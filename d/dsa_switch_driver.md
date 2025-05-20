# Struct: <code>dsa_switch_driver</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct dsa_switch_driver {
    struct list_head list;
    enum dsa_tag_protocol tag_protocol;
    const char * (*probe)(struct device *, struct device *, int, void **);
    int (*setup)(struct dsa_switch *);
    int (*set_addr)(struct dsa_switch *, u8 *);
    u32 (*get_phy_flags)(struct dsa_switch *, int);
    int (*phy_read)(struct dsa_switch *, int, int);
    int (*phy_write)(struct dsa_switch *, int, int, u16);
    void (*adjust_link)(struct dsa_switch *, int, struct phy_device *);
    void (*fixed_link_update)(struct dsa_switch *, int, struct fixed_phy_status *);
    void (*get_strings)(struct dsa_switch *, int, uint8_t *);
    void (*get_ethtool_stats)(struct dsa_switch *, int, uint64_t *);
    int (*get_sset_count)(struct dsa_switch *);
    void (*get_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*set_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*suspend)(struct dsa_switch *);
    int (*resume)(struct dsa_switch *);
    int (*port_enable)(struct dsa_switch *, int, struct phy_device *);
    void (*port_disable)(struct dsa_switch *, int, struct phy_device *);
    int (*set_eee)(struct dsa_switch *, int, struct phy_device *, struct ethtool_eee *);
    int (*get_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_temp)(struct dsa_switch *, int *);
    int (*get_temp_limit)(struct dsa_switch *, int *);
    int (*set_temp_limit)(struct dsa_switch *, int);
    int (*get_temp_alarm)(struct dsa_switch *, bool *);
    int (*get_eeprom_len)(struct dsa_switch *);
    int (*get_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*get_regs_len)(struct dsa_switch *, int);
    void (*get_regs)(struct dsa_switch *, int, struct ethtool_regs *, void *);
    int (*set_ageing_time)(struct dsa_switch *, unsigned int);
    int (*port_bridge_join)(struct dsa_switch *, int, struct net_device *);
    void (*port_bridge_leave)(struct dsa_switch *, int);
    void (*port_stp_state_set)(struct dsa_switch *, int, u8);
    int (*port_vlan_filtering)(struct dsa_switch *, int, bool);
    int (*port_vlan_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *, struct switchdev_trans *);
    void (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *, struct switchdev_trans *);
    int (*port_vlan_del)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_vlan_dump)(struct dsa_switch *, int, struct switchdev_obj_port_vlan *, int(*)(struct switchdev_obj *));
    int (*port_fdb_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_fdb *, struct switchdev_trans *);
    void (*port_fdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_fdb *, struct switchdev_trans *);
    int (*port_fdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_fdb *);
    int (*port_fdb_dump)(struct dsa_switch *, int, struct switchdev_obj_port_fdb *, int(*)(struct switchdev_obj *));
};
```
</details>
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
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
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
</ul>
