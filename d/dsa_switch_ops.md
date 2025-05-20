# Struct: <code>dsa_switch_ops</code>

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
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct dsa_switch_ops {
    struct list_head list;
    const char * (*probe)(struct device *, struct device *, int, void **);
    enum dsa_tag_protocol (*get_tag_protocol)(struct dsa_switch *);
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
    void (*port_fast_age)(struct dsa_switch *, int);
    int (*port_vlan_filtering)(struct dsa_switch *, int, bool);
    int (*port_vlan_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *, struct switchdev_trans *);
    void (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *, struct switchdev_trans *);
    int (*port_vlan_del)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_vlan_dump)(struct dsa_switch *, int, struct switchdev_obj_port_vlan *, int(*)(struct switchdev_obj *));
    int (*port_fdb_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_fdb *, struct switchdev_trans *);
    void (*port_fdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_fdb *, struct switchdev_trans *);
    int (*port_fdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_fdb *);
    int (*port_fdb_dump)(struct dsa_switch *, int, struct switchdev_obj_port_fdb *, int(*)(struct switchdev_obj *));
    int (*port_mdb_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *, struct switchdev_trans *);
    void (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *, struct switchdev_trans *);
    int (*port_mdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*port_mdb_dump)(struct dsa_switch *, int, struct switchdev_obj_port_mdb *, int(*)(struct switchdev_obj *));
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct dsa_switch_ops {
    const char * (*probe)(struct device *, struct device *, int, void **);
    enum dsa_tag_protocol (*get_tag_protocol)(struct dsa_switch *);
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
    int (*get_eeprom_len)(struct dsa_switch *);
    int (*get_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*get_regs_len)(struct dsa_switch *, int);
    void (*get_regs)(struct dsa_switch *, int, struct ethtool_regs *, void *);
    int (*set_ageing_time)(struct dsa_switch *, unsigned int);
    int (*port_bridge_join)(struct dsa_switch *, int, struct net_device *);
    void (*port_bridge_leave)(struct dsa_switch *, int, struct net_device *);
    void (*port_stp_state_set)(struct dsa_switch *, int, u8);
    void (*port_fast_age)(struct dsa_switch *, int);
    int (*port_vlan_filtering)(struct dsa_switch *, int, bool);
    int (*port_vlan_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *, struct switchdev_trans *);
    void (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *, struct switchdev_trans *);
    int (*port_vlan_del)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_vlan_dump)(struct dsa_switch *, int, struct switchdev_obj_port_vlan *, switchdev_obj_dump_cb_t *);
    int (*port_fdb_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_fdb *, struct switchdev_trans *);
    void (*port_fdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_fdb *, struct switchdev_trans *);
    int (*port_fdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_fdb *);
    int (*port_fdb_dump)(struct dsa_switch *, int, struct switchdev_obj_port_fdb *, switchdev_obj_dump_cb_t *);
    int (*port_mdb_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *, struct switchdev_trans *);
    void (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *, struct switchdev_trans *);
    int (*port_mdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*port_mdb_dump)(struct dsa_switch *, int, struct switchdev_obj_port_mdb *, switchdev_obj_dump_cb_t *);
    int (*get_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *);
    int (*port_mirror_add)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *, bool);
    void (*port_mirror_del)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *);
    int (*crosschip_bridge_join)(struct dsa_switch *, int, int, struct net_device *);
    void (*crosschip_bridge_leave)(struct dsa_switch *, int, int, struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dsa_switch_ops {
    const char * (*probe)(struct device *, struct device *, int, void **);
    enum dsa_tag_protocol (*get_tag_protocol)(struct dsa_switch *, int);
    int (*setup)(struct dsa_switch *);
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
    int (*set_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_eeprom_len)(struct dsa_switch *);
    int (*get_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*get_regs_len)(struct dsa_switch *, int);
    void (*get_regs)(struct dsa_switch *, int, struct ethtool_regs *, void *);
    int (*set_ageing_time)(struct dsa_switch *, unsigned int);
    int (*port_bridge_join)(struct dsa_switch *, int, struct net_device *);
    void (*port_bridge_leave)(struct dsa_switch *, int, struct net_device *);
    void (*port_stp_state_set)(struct dsa_switch *, int, u8);
    void (*port_fast_age)(struct dsa_switch *, int);
    int (*port_vlan_filtering)(struct dsa_switch *, int, bool);
    int (*port_vlan_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *, struct switchdev_trans *);
    void (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *, struct switchdev_trans *);
    int (*port_vlan_del)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_fdb_add)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_del)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_dump)(struct dsa_switch *, int, dsa_fdb_dump_cb_t *, void *);
    int (*port_mdb_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *, struct switchdev_trans *);
    void (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *, struct switchdev_trans *);
    int (*port_mdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*get_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *);
    int (*port_mirror_add)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *, bool);
    void (*port_mirror_del)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *);
    int (*crosschip_bridge_join)(struct dsa_switch *, int, int, struct net_device *);
    void (*crosschip_bridge_leave)(struct dsa_switch *, int, int, struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dsa_switch_ops {
    const char * (*probe)(struct device *, struct device *, int, void **);
    enum dsa_tag_protocol (*get_tag_protocol)(struct dsa_switch *, int);
    int (*setup)(struct dsa_switch *);
    u32 (*get_phy_flags)(struct dsa_switch *, int);
    int (*phy_read)(struct dsa_switch *, int, int);
    int (*phy_write)(struct dsa_switch *, int, int, u16);
    void (*adjust_link)(struct dsa_switch *, int, struct phy_device *);
    void (*fixed_link_update)(struct dsa_switch *, int, struct fixed_phy_status *);
    void (*phylink_validate)(struct dsa_switch *, int, long unsigned int *, struct phylink_link_state *);
    int (*phylink_mac_link_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*phylink_mac_config)(struct dsa_switch *, int, unsigned int, const struct phylink_link_state *);
    void (*phylink_mac_an_restart)(struct dsa_switch *, int);
    void (*phylink_mac_link_down)(struct dsa_switch *, int, unsigned int, phy_interface_t);
    void (*phylink_mac_link_up)(struct dsa_switch *, int, unsigned int, phy_interface_t, struct phy_device *);
    void (*phylink_fixed_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*get_strings)(struct dsa_switch *, int, u32, uint8_t *);
    void (*get_ethtool_stats)(struct dsa_switch *, int, uint64_t *);
    int (*get_sset_count)(struct dsa_switch *, int, int);
    void (*get_ethtool_phy_stats)(struct dsa_switch *, int, uint64_t *);
    void (*get_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*set_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*get_ts_info)(struct dsa_switch *, int, struct ethtool_ts_info *);
    int (*suspend)(struct dsa_switch *);
    int (*resume)(struct dsa_switch *);
    int (*port_enable)(struct dsa_switch *, int, struct phy_device *);
    void (*port_disable)(struct dsa_switch *, int, struct phy_device *);
    int (*set_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_eeprom_len)(struct dsa_switch *);
    int (*get_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*get_regs_len)(struct dsa_switch *, int);
    void (*get_regs)(struct dsa_switch *, int, struct ethtool_regs *, void *);
    int (*set_ageing_time)(struct dsa_switch *, unsigned int);
    int (*port_bridge_join)(struct dsa_switch *, int, struct net_device *);
    void (*port_bridge_leave)(struct dsa_switch *, int, struct net_device *);
    void (*port_stp_state_set)(struct dsa_switch *, int, u8);
    void (*port_fast_age)(struct dsa_switch *, int);
    int (*port_vlan_filtering)(struct dsa_switch *, int, bool);
    int (*port_vlan_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    void (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_vlan_del)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_fdb_add)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_del)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_dump)(struct dsa_switch *, int, dsa_fdb_dump_cb_t *, void *);
    int (*port_mdb_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    void (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*port_mdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*get_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *);
    int (*port_mirror_add)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *, bool);
    void (*port_mirror_del)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *);
    int (*crosschip_bridge_join)(struct dsa_switch *, int, int, struct net_device *);
    void (*crosschip_bridge_leave)(struct dsa_switch *, int, int, struct net_device *);
    int (*port_hwtstamp_get)(struct dsa_switch *, int, struct ifreq *);
    int (*port_hwtstamp_set)(struct dsa_switch *, int, struct ifreq *);
    bool (*port_txtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    bool (*port_rxtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dsa_switch_ops {
    const char * (*probe)(struct device *, struct device *, int, void **);
    enum dsa_tag_protocol (*get_tag_protocol)(struct dsa_switch *, int);
    int (*setup)(struct dsa_switch *);
    u32 (*get_phy_flags)(struct dsa_switch *, int);
    int (*phy_read)(struct dsa_switch *, int, int);
    int (*phy_write)(struct dsa_switch *, int, int, u16);
    void (*adjust_link)(struct dsa_switch *, int, struct phy_device *);
    void (*fixed_link_update)(struct dsa_switch *, int, struct fixed_phy_status *);
    void (*phylink_validate)(struct dsa_switch *, int, long unsigned int *, struct phylink_link_state *);
    int (*phylink_mac_link_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*phylink_mac_config)(struct dsa_switch *, int, unsigned int, const struct phylink_link_state *);
    void (*phylink_mac_an_restart)(struct dsa_switch *, int);
    void (*phylink_mac_link_down)(struct dsa_switch *, int, unsigned int, phy_interface_t);
    void (*phylink_mac_link_up)(struct dsa_switch *, int, unsigned int, phy_interface_t, struct phy_device *);
    void (*phylink_fixed_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*get_strings)(struct dsa_switch *, int, u32, uint8_t *);
    void (*get_ethtool_stats)(struct dsa_switch *, int, uint64_t *);
    int (*get_sset_count)(struct dsa_switch *, int, int);
    void (*get_ethtool_phy_stats)(struct dsa_switch *, int, uint64_t *);
    void (*get_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*set_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*get_ts_info)(struct dsa_switch *, int, struct ethtool_ts_info *);
    int (*suspend)(struct dsa_switch *);
    int (*resume)(struct dsa_switch *);
    int (*port_enable)(struct dsa_switch *, int, struct phy_device *);
    void (*port_disable)(struct dsa_switch *, int, struct phy_device *);
    int (*set_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_eeprom_len)(struct dsa_switch *);
    int (*get_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*get_regs_len)(struct dsa_switch *, int);
    void (*get_regs)(struct dsa_switch *, int, struct ethtool_regs *, void *);
    int (*set_ageing_time)(struct dsa_switch *, unsigned int);
    int (*port_bridge_join)(struct dsa_switch *, int, struct net_device *);
    void (*port_bridge_leave)(struct dsa_switch *, int, struct net_device *);
    void (*port_stp_state_set)(struct dsa_switch *, int, u8);
    void (*port_fast_age)(struct dsa_switch *, int);
    int (*port_vlan_filtering)(struct dsa_switch *, int, bool);
    int (*port_vlan_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    void (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_vlan_del)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_fdb_add)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_del)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_dump)(struct dsa_switch *, int, dsa_fdb_dump_cb_t *, void *);
    int (*port_mdb_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    void (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*port_mdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*get_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *);
    int (*port_mirror_add)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *, bool);
    void (*port_mirror_del)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *);
    int (*crosschip_bridge_join)(struct dsa_switch *, int, int, struct net_device *);
    void (*crosschip_bridge_leave)(struct dsa_switch *, int, int, struct net_device *);
    int (*port_hwtstamp_get)(struct dsa_switch *, int, struct ifreq *);
    int (*port_hwtstamp_set)(struct dsa_switch *, int, struct ifreq *);
    bool (*port_txtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    bool (*port_rxtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dsa_switch_ops {
    enum dsa_tag_protocol (*get_tag_protocol)(struct dsa_switch *, int);
    int (*setup)(struct dsa_switch *);
    void (*teardown)(struct dsa_switch *);
    u32 (*get_phy_flags)(struct dsa_switch *, int);
    int (*phy_read)(struct dsa_switch *, int, int);
    int (*phy_write)(struct dsa_switch *, int, int, u16);
    void (*adjust_link)(struct dsa_switch *, int, struct phy_device *);
    void (*fixed_link_update)(struct dsa_switch *, int, struct fixed_phy_status *);
    void (*phylink_validate)(struct dsa_switch *, int, long unsigned int *, struct phylink_link_state *);
    int (*phylink_mac_link_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*phylink_mac_config)(struct dsa_switch *, int, unsigned int, const struct phylink_link_state *);
    void (*phylink_mac_an_restart)(struct dsa_switch *, int);
    void (*phylink_mac_link_down)(struct dsa_switch *, int, unsigned int, phy_interface_t);
    void (*phylink_mac_link_up)(struct dsa_switch *, int, unsigned int, phy_interface_t, struct phy_device *);
    void (*phylink_fixed_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*get_strings)(struct dsa_switch *, int, u32, uint8_t *);
    void (*get_ethtool_stats)(struct dsa_switch *, int, uint64_t *);
    int (*get_sset_count)(struct dsa_switch *, int, int);
    void (*get_ethtool_phy_stats)(struct dsa_switch *, int, uint64_t *);
    void (*get_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*set_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*get_ts_info)(struct dsa_switch *, int, struct ethtool_ts_info *);
    int (*suspend)(struct dsa_switch *);
    int (*resume)(struct dsa_switch *);
    int (*port_enable)(struct dsa_switch *, int, struct phy_device *);
    void (*port_disable)(struct dsa_switch *, int);
    int (*set_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_eeprom_len)(struct dsa_switch *);
    int (*get_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*get_regs_len)(struct dsa_switch *, int);
    void (*get_regs)(struct dsa_switch *, int, struct ethtool_regs *, void *);
    int (*set_ageing_time)(struct dsa_switch *, unsigned int);
    int (*port_bridge_join)(struct dsa_switch *, int, struct net_device *);
    void (*port_bridge_leave)(struct dsa_switch *, int, struct net_device *);
    void (*port_stp_state_set)(struct dsa_switch *, int, u8);
    void (*port_fast_age)(struct dsa_switch *, int);
    int (*port_egress_floods)(struct dsa_switch *, int, bool, bool);
    int (*port_vlan_filtering)(struct dsa_switch *, int, bool);
    int (*port_vlan_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    void (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_vlan_del)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_fdb_add)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_del)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_dump)(struct dsa_switch *, int, dsa_fdb_dump_cb_t *, void *);
    int (*port_mdb_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    void (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*port_mdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*get_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *);
    int (*port_mirror_add)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *, bool);
    void (*port_mirror_del)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *);
    int (*crosschip_bridge_join)(struct dsa_switch *, int, int, struct net_device *);
    void (*crosschip_bridge_leave)(struct dsa_switch *, int, int, struct net_device *);
    int (*port_hwtstamp_get)(struct dsa_switch *, int, struct ifreq *);
    int (*port_hwtstamp_set)(struct dsa_switch *, int, struct ifreq *);
    bool (*port_txtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    bool (*port_rxtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    netdev_tx_t (*port_deferred_xmit)(struct dsa_switch *, int, struct sk_buff *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dsa_switch_ops {
    enum dsa_tag_protocol (*get_tag_protocol)(struct dsa_switch *, int);
    int (*setup)(struct dsa_switch *);
    void (*teardown)(struct dsa_switch *);
    u32 (*get_phy_flags)(struct dsa_switch *, int);
    int (*phy_read)(struct dsa_switch *, int, int);
    int (*phy_write)(struct dsa_switch *, int, int, u16);
    void (*adjust_link)(struct dsa_switch *, int, struct phy_device *);
    void (*fixed_link_update)(struct dsa_switch *, int, struct fixed_phy_status *);
    void (*phylink_validate)(struct dsa_switch *, int, long unsigned int *, struct phylink_link_state *);
    int (*phylink_mac_link_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*phylink_mac_config)(struct dsa_switch *, int, unsigned int, const struct phylink_link_state *);
    void (*phylink_mac_an_restart)(struct dsa_switch *, int);
    void (*phylink_mac_link_down)(struct dsa_switch *, int, unsigned int, phy_interface_t);
    void (*phylink_mac_link_up)(struct dsa_switch *, int, unsigned int, phy_interface_t, struct phy_device *);
    void (*phylink_fixed_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*get_strings)(struct dsa_switch *, int, u32, uint8_t *);
    void (*get_ethtool_stats)(struct dsa_switch *, int, uint64_t *);
    int (*get_sset_count)(struct dsa_switch *, int, int);
    void (*get_ethtool_phy_stats)(struct dsa_switch *, int, uint64_t *);
    void (*get_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*set_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*get_ts_info)(struct dsa_switch *, int, struct ethtool_ts_info *);
    int (*suspend)(struct dsa_switch *);
    int (*resume)(struct dsa_switch *);
    int (*port_enable)(struct dsa_switch *, int, struct phy_device *);
    void (*port_disable)(struct dsa_switch *, int);
    int (*set_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_eeprom_len)(struct dsa_switch *);
    int (*get_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*get_regs_len)(struct dsa_switch *, int);
    void (*get_regs)(struct dsa_switch *, int, struct ethtool_regs *, void *);
    int (*set_ageing_time)(struct dsa_switch *, unsigned int);
    int (*port_bridge_join)(struct dsa_switch *, int, struct net_device *);
    void (*port_bridge_leave)(struct dsa_switch *, int, struct net_device *);
    void (*port_stp_state_set)(struct dsa_switch *, int, u8);
    void (*port_fast_age)(struct dsa_switch *, int);
    int (*port_egress_floods)(struct dsa_switch *, int, bool, bool);
    int (*port_vlan_filtering)(struct dsa_switch *, int, bool);
    int (*port_vlan_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    void (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_vlan_del)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_fdb_add)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_del)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_dump)(struct dsa_switch *, int, dsa_fdb_dump_cb_t *, void *);
    int (*port_mdb_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    void (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*port_mdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*get_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *);
    int (*port_mirror_add)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *, bool);
    void (*port_mirror_del)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *);
    int (*port_setup_tc)(struct dsa_switch *, int, enum tc_setup_type, void *);
    int (*crosschip_bridge_join)(struct dsa_switch *, int, int, struct net_device *);
    void (*crosschip_bridge_leave)(struct dsa_switch *, int, int, struct net_device *);
    int (*port_hwtstamp_get)(struct dsa_switch *, int, struct ifreq *);
    int (*port_hwtstamp_set)(struct dsa_switch *, int, struct ifreq *);
    bool (*port_txtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    bool (*port_rxtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    netdev_tx_t (*port_deferred_xmit)(struct dsa_switch *, int, struct sk_buff *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dsa_switch_ops {
    enum dsa_tag_protocol (*get_tag_protocol)(struct dsa_switch *, int, enum dsa_tag_protocol);
    int (*setup)(struct dsa_switch *);
    void (*teardown)(struct dsa_switch *);
    u32 (*get_phy_flags)(struct dsa_switch *, int);
    int (*phy_read)(struct dsa_switch *, int, int);
    int (*phy_write)(struct dsa_switch *, int, int, u16);
    void (*adjust_link)(struct dsa_switch *, int, struct phy_device *);
    void (*fixed_link_update)(struct dsa_switch *, int, struct fixed_phy_status *);
    void (*phylink_validate)(struct dsa_switch *, int, long unsigned int *, struct phylink_link_state *);
    int (*phylink_mac_link_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*phylink_mac_config)(struct dsa_switch *, int, unsigned int, const struct phylink_link_state *);
    void (*phylink_mac_an_restart)(struct dsa_switch *, int);
    void (*phylink_mac_link_down)(struct dsa_switch *, int, unsigned int, phy_interface_t);
    void (*phylink_mac_link_up)(struct dsa_switch *, int, unsigned int, phy_interface_t, struct phy_device *, int, int, bool, bool);
    void (*phylink_fixed_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*get_strings)(struct dsa_switch *, int, u32, uint8_t *);
    void (*get_ethtool_stats)(struct dsa_switch *, int, uint64_t *);
    int (*get_sset_count)(struct dsa_switch *, int, int);
    void (*get_ethtool_phy_stats)(struct dsa_switch *, int, uint64_t *);
    void (*get_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*set_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*get_ts_info)(struct dsa_switch *, int, struct ethtool_ts_info *);
    int (*suspend)(struct dsa_switch *);
    int (*resume)(struct dsa_switch *);
    int (*port_enable)(struct dsa_switch *, int, struct phy_device *);
    void (*port_disable)(struct dsa_switch *, int);
    int (*set_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_eeprom_len)(struct dsa_switch *);
    int (*get_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*get_regs_len)(struct dsa_switch *, int);
    void (*get_regs)(struct dsa_switch *, int, struct ethtool_regs *, void *);
    int (*set_ageing_time)(struct dsa_switch *, unsigned int);
    int (*port_bridge_join)(struct dsa_switch *, int, struct net_device *);
    void (*port_bridge_leave)(struct dsa_switch *, int, struct net_device *);
    void (*port_stp_state_set)(struct dsa_switch *, int, u8);
    void (*port_fast_age)(struct dsa_switch *, int);
    int (*port_egress_floods)(struct dsa_switch *, int, bool, bool);
    int (*port_vlan_filtering)(struct dsa_switch *, int, bool);
    int (*port_vlan_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    void (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_vlan_del)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_fdb_add)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_del)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_dump)(struct dsa_switch *, int, dsa_fdb_dump_cb_t *, void *);
    int (*port_mdb_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    void (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*port_mdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*get_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *);
    int (*cls_flower_add)(struct dsa_switch *, int, struct flow_cls_offload *, bool);
    int (*cls_flower_del)(struct dsa_switch *, int, struct flow_cls_offload *, bool);
    int (*cls_flower_stats)(struct dsa_switch *, int, struct flow_cls_offload *, bool);
    int (*port_mirror_add)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *, bool);
    void (*port_mirror_del)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *);
    int (*port_policer_add)(struct dsa_switch *, int, struct dsa_mall_policer_tc_entry *);
    void (*port_policer_del)(struct dsa_switch *, int);
    int (*port_setup_tc)(struct dsa_switch *, int, enum tc_setup_type, void *);
    int (*crosschip_bridge_join)(struct dsa_switch *, int, int, int, struct net_device *);
    void (*crosschip_bridge_leave)(struct dsa_switch *, int, int, int, struct net_device *);
    int (*port_hwtstamp_get)(struct dsa_switch *, int, struct ifreq *);
    int (*port_hwtstamp_set)(struct dsa_switch *, int, struct ifreq *);
    bool (*port_txtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    bool (*port_rxtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    int (*devlink_param_get)(struct dsa_switch *, u32, struct devlink_param_gset_ctx *);
    int (*devlink_param_set)(struct dsa_switch *, u32, struct devlink_param_gset_ctx *);
    int (*port_change_mtu)(struct dsa_switch *, int, int);
    int (*port_max_mtu)(struct dsa_switch *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dsa_switch_ops {
    enum dsa_tag_protocol (*get_tag_protocol)(struct dsa_switch *, int, enum dsa_tag_protocol);
    int (*setup)(struct dsa_switch *);
    void (*teardown)(struct dsa_switch *);
    u32 (*get_phy_flags)(struct dsa_switch *, int);
    int (*phy_read)(struct dsa_switch *, int, int);
    int (*phy_write)(struct dsa_switch *, int, int, u16);
    void (*adjust_link)(struct dsa_switch *, int, struct phy_device *);
    void (*fixed_link_update)(struct dsa_switch *, int, struct fixed_phy_status *);
    void (*phylink_validate)(struct dsa_switch *, int, long unsigned int *, struct phylink_link_state *);
    int (*phylink_mac_link_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*phylink_mac_config)(struct dsa_switch *, int, unsigned int, const struct phylink_link_state *);
    void (*phylink_mac_an_restart)(struct dsa_switch *, int);
    void (*phylink_mac_link_down)(struct dsa_switch *, int, unsigned int, phy_interface_t);
    void (*phylink_mac_link_up)(struct dsa_switch *, int, unsigned int, phy_interface_t, struct phy_device *, int, int, bool, bool);
    void (*phylink_fixed_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*get_strings)(struct dsa_switch *, int, u32, uint8_t *);
    void (*get_ethtool_stats)(struct dsa_switch *, int, uint64_t *);
    int (*get_sset_count)(struct dsa_switch *, int, int);
    void (*get_ethtool_phy_stats)(struct dsa_switch *, int, uint64_t *);
    void (*get_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*set_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*get_ts_info)(struct dsa_switch *, int, struct ethtool_ts_info *);
    int (*suspend)(struct dsa_switch *);
    int (*resume)(struct dsa_switch *);
    int (*port_enable)(struct dsa_switch *, int, struct phy_device *);
    void (*port_disable)(struct dsa_switch *, int);
    int (*set_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_eeprom_len)(struct dsa_switch *);
    int (*get_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*get_regs_len)(struct dsa_switch *, int);
    void (*get_regs)(struct dsa_switch *, int, struct ethtool_regs *, void *);
    int (*port_prechangeupper)(struct dsa_switch *, int, struct netdev_notifier_changeupper_info *);
    int (*set_ageing_time)(struct dsa_switch *, unsigned int);
    int (*port_bridge_join)(struct dsa_switch *, int, struct net_device *);
    void (*port_bridge_leave)(struct dsa_switch *, int, struct net_device *);
    void (*port_stp_state_set)(struct dsa_switch *, int, u8);
    void (*port_fast_age)(struct dsa_switch *, int);
    int (*port_egress_floods)(struct dsa_switch *, int, bool, bool);
    int (*port_vlan_filtering)(struct dsa_switch *, int, bool, struct switchdev_trans *);
    int (*port_vlan_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    void (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_vlan_del)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_fdb_add)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_del)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_dump)(struct dsa_switch *, int, dsa_fdb_dump_cb_t *, void *);
    int (*port_mdb_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    void (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*port_mdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*get_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *);
    int (*cls_flower_add)(struct dsa_switch *, int, struct flow_cls_offload *, bool);
    int (*cls_flower_del)(struct dsa_switch *, int, struct flow_cls_offload *, bool);
    int (*cls_flower_stats)(struct dsa_switch *, int, struct flow_cls_offload *, bool);
    int (*port_mirror_add)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *, bool);
    void (*port_mirror_del)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *);
    int (*port_policer_add)(struct dsa_switch *, int, struct dsa_mall_policer_tc_entry *);
    void (*port_policer_del)(struct dsa_switch *, int);
    int (*port_setup_tc)(struct dsa_switch *, int, enum tc_setup_type, void *);
    int (*crosschip_bridge_join)(struct dsa_switch *, int, int, int, struct net_device *);
    void (*crosschip_bridge_leave)(struct dsa_switch *, int, int, int, struct net_device *);
    int (*port_hwtstamp_get)(struct dsa_switch *, int, struct ifreq *);
    int (*port_hwtstamp_set)(struct dsa_switch *, int, struct ifreq *);
    bool (*port_txtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    bool (*port_rxtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    int (*devlink_param_get)(struct dsa_switch *, u32, struct devlink_param_gset_ctx *);
    int (*devlink_param_set)(struct dsa_switch *, u32, struct devlink_param_gset_ctx *);
    int (*devlink_info_get)(struct dsa_switch *, struct devlink_info_req *, struct netlink_ext_ack *);
    int (*port_change_mtu)(struct dsa_switch *, int, int);
    int (*port_max_mtu)(struct dsa_switch *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dsa_switch_ops {
    enum dsa_tag_protocol (*get_tag_protocol)(struct dsa_switch *, int, enum dsa_tag_protocol);
    int (*change_tag_protocol)(struct dsa_switch *, int, enum dsa_tag_protocol);
    int (*setup)(struct dsa_switch *);
    void (*teardown)(struct dsa_switch *);
    u32 (*get_phy_flags)(struct dsa_switch *, int);
    int (*phy_read)(struct dsa_switch *, int, int);
    int (*phy_write)(struct dsa_switch *, int, int, u16);
    void (*adjust_link)(struct dsa_switch *, int, struct phy_device *);
    void (*fixed_link_update)(struct dsa_switch *, int, struct fixed_phy_status *);
    void (*phylink_validate)(struct dsa_switch *, int, long unsigned int *, struct phylink_link_state *);
    int (*phylink_mac_link_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*phylink_mac_config)(struct dsa_switch *, int, unsigned int, const struct phylink_link_state *);
    void (*phylink_mac_an_restart)(struct dsa_switch *, int);
    void (*phylink_mac_link_down)(struct dsa_switch *, int, unsigned int, phy_interface_t);
    void (*phylink_mac_link_up)(struct dsa_switch *, int, unsigned int, phy_interface_t, struct phy_device *, int, int, bool, bool);
    void (*phylink_fixed_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*get_strings)(struct dsa_switch *, int, u32, uint8_t *);
    void (*get_ethtool_stats)(struct dsa_switch *, int, uint64_t *);
    int (*get_sset_count)(struct dsa_switch *, int, int);
    void (*get_ethtool_phy_stats)(struct dsa_switch *, int, uint64_t *);
    void (*get_stats64)(struct dsa_switch *, int, struct rtnl_link_stats64 *);
    void (*self_test)(struct dsa_switch *, int, struct ethtool_test *, u64 *);
    void (*get_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*set_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*get_ts_info)(struct dsa_switch *, int, struct ethtool_ts_info *);
    int (*suspend)(struct dsa_switch *);
    int (*resume)(struct dsa_switch *);
    int (*port_enable)(struct dsa_switch *, int, struct phy_device *);
    void (*port_disable)(struct dsa_switch *, int);
    int (*set_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_eeprom_len)(struct dsa_switch *);
    int (*get_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*get_regs_len)(struct dsa_switch *, int);
    void (*get_regs)(struct dsa_switch *, int, struct ethtool_regs *, void *);
    int (*port_prechangeupper)(struct dsa_switch *, int, struct netdev_notifier_changeupper_info *);
    int (*set_ageing_time)(struct dsa_switch *, unsigned int);
    int (*port_bridge_join)(struct dsa_switch *, int, struct net_device *);
    void (*port_bridge_leave)(struct dsa_switch *, int, struct net_device *);
    void (*port_stp_state_set)(struct dsa_switch *, int, u8);
    void (*port_fast_age)(struct dsa_switch *, int);
    int (*port_pre_bridge_flags)(struct dsa_switch *, int, struct switchdev_brport_flags, struct netlink_ext_ack *);
    int (*port_bridge_flags)(struct dsa_switch *, int, struct switchdev_brport_flags, struct netlink_ext_ack *);
    int (*port_set_mrouter)(struct dsa_switch *, int, bool, struct netlink_ext_ack *);
    int (*port_vlan_filtering)(struct dsa_switch *, int, bool, struct netlink_ext_ack *);
    int (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *, struct netlink_ext_ack *);
    int (*port_vlan_del)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_fdb_add)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_del)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_dump)(struct dsa_switch *, int, dsa_fdb_dump_cb_t *, void *);
    int (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*port_mdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*get_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *);
    int (*cls_flower_add)(struct dsa_switch *, int, struct flow_cls_offload *, bool);
    int (*cls_flower_del)(struct dsa_switch *, int, struct flow_cls_offload *, bool);
    int (*cls_flower_stats)(struct dsa_switch *, int, struct flow_cls_offload *, bool);
    int (*port_mirror_add)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *, bool);
    void (*port_mirror_del)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *);
    int (*port_policer_add)(struct dsa_switch *, int, struct dsa_mall_policer_tc_entry *);
    void (*port_policer_del)(struct dsa_switch *, int);
    int (*port_setup_tc)(struct dsa_switch *, int, enum tc_setup_type, void *);
    int (*crosschip_bridge_join)(struct dsa_switch *, int, int, int, struct net_device *);
    void (*crosschip_bridge_leave)(struct dsa_switch *, int, int, int, struct net_device *);
    int (*crosschip_lag_change)(struct dsa_switch *, int, int);
    int (*crosschip_lag_join)(struct dsa_switch *, int, int, struct net_device *, struct netdev_lag_upper_info *);
    int (*crosschip_lag_leave)(struct dsa_switch *, int, int, struct net_device *);
    int (*port_hwtstamp_get)(struct dsa_switch *, int, struct ifreq *);
    int (*port_hwtstamp_set)(struct dsa_switch *, int, struct ifreq *);
    void (*port_txtstamp)(struct dsa_switch *, int, struct sk_buff *);
    bool (*port_rxtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    int (*devlink_param_get)(struct dsa_switch *, u32, struct devlink_param_gset_ctx *);
    int (*devlink_param_set)(struct dsa_switch *, u32, struct devlink_param_gset_ctx *);
    int (*devlink_info_get)(struct dsa_switch *, struct devlink_info_req *, struct netlink_ext_ack *);
    int (*devlink_sb_pool_get)(struct dsa_switch *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*devlink_sb_pool_set)(struct dsa_switch *, unsigned int, u16, u32, enum devlink_sb_threshold_type, struct netlink_ext_ack *);
    int (*devlink_sb_port_pool_get)(struct dsa_switch *, int, unsigned int, u16, u32 *);
    int (*devlink_sb_port_pool_set)(struct dsa_switch *, int, unsigned int, u16, u32, struct netlink_ext_ack *);
    int (*devlink_sb_tc_pool_bind_get)(struct dsa_switch *, int, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*devlink_sb_tc_pool_bind_set)(struct dsa_switch *, int, unsigned int, u16, enum devlink_sb_pool_type, u16, u32, struct netlink_ext_ack *);
    int (*devlink_sb_occ_snapshot)(struct dsa_switch *, unsigned int);
    int (*devlink_sb_occ_max_clear)(struct dsa_switch *, unsigned int);
    int (*devlink_sb_occ_port_pool_get)(struct dsa_switch *, int, unsigned int, u16, u32 *, u32 *);
    int (*devlink_sb_occ_tc_port_bind_get)(struct dsa_switch *, int, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*port_change_mtu)(struct dsa_switch *, int, int);
    int (*port_max_mtu)(struct dsa_switch *, int);
    int (*port_lag_change)(struct dsa_switch *, int);
    int (*port_lag_join)(struct dsa_switch *, int, struct net_device *, struct netdev_lag_upper_info *);
    int (*port_lag_leave)(struct dsa_switch *, int, struct net_device *);
    int (*port_hsr_join)(struct dsa_switch *, int, struct net_device *);
    int (*port_hsr_leave)(struct dsa_switch *, int, struct net_device *);
    int (*port_mrp_add)(struct dsa_switch *, int, const struct switchdev_obj_mrp *);
    int (*port_mrp_del)(struct dsa_switch *, int, const struct switchdev_obj_mrp *);
    int (*port_mrp_add_ring_role)(struct dsa_switch *, int, const struct switchdev_obj_ring_role_mrp *);
    int (*port_mrp_del_ring_role)(struct dsa_switch *, int, const struct switchdev_obj_ring_role_mrp *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dsa_switch_ops {
    enum dsa_tag_protocol (*get_tag_protocol)(struct dsa_switch *, int, enum dsa_tag_protocol);
    int (*change_tag_protocol)(struct dsa_switch *, int, enum dsa_tag_protocol);
    int (*setup)(struct dsa_switch *);
    void (*teardown)(struct dsa_switch *);
    int (*port_setup)(struct dsa_switch *, int);
    void (*port_teardown)(struct dsa_switch *, int);
    u32 (*get_phy_flags)(struct dsa_switch *, int);
    int (*phy_read)(struct dsa_switch *, int, int);
    int (*phy_write)(struct dsa_switch *, int, int, u16);
    void (*adjust_link)(struct dsa_switch *, int, struct phy_device *);
    void (*fixed_link_update)(struct dsa_switch *, int, struct fixed_phy_status *);
    void (*phylink_validate)(struct dsa_switch *, int, long unsigned int *, struct phylink_link_state *);
    int (*phylink_mac_link_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*phylink_mac_config)(struct dsa_switch *, int, unsigned int, const struct phylink_link_state *);
    void (*phylink_mac_an_restart)(struct dsa_switch *, int);
    void (*phylink_mac_link_down)(struct dsa_switch *, int, unsigned int, phy_interface_t);
    void (*phylink_mac_link_up)(struct dsa_switch *, int, unsigned int, phy_interface_t, struct phy_device *, int, int, bool, bool);
    void (*phylink_fixed_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*get_strings)(struct dsa_switch *, int, u32, uint8_t *);
    void (*get_ethtool_stats)(struct dsa_switch *, int, uint64_t *);
    int (*get_sset_count)(struct dsa_switch *, int, int);
    void (*get_ethtool_phy_stats)(struct dsa_switch *, int, uint64_t *);
    void (*get_stats64)(struct dsa_switch *, int, struct rtnl_link_stats64 *);
    void (*self_test)(struct dsa_switch *, int, struct ethtool_test *, u64 *);
    void (*get_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*set_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*get_ts_info)(struct dsa_switch *, int, struct ethtool_ts_info *);
    int (*suspend)(struct dsa_switch *);
    int (*resume)(struct dsa_switch *);
    int (*port_enable)(struct dsa_switch *, int, struct phy_device *);
    void (*port_disable)(struct dsa_switch *, int);
    int (*set_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_eeprom_len)(struct dsa_switch *);
    int (*get_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*get_regs_len)(struct dsa_switch *, int);
    void (*get_regs)(struct dsa_switch *, int, struct ethtool_regs *, void *);
    int (*port_prechangeupper)(struct dsa_switch *, int, struct netdev_notifier_changeupper_info *);
    int (*set_ageing_time)(struct dsa_switch *, unsigned int);
    int (*port_bridge_join)(struct dsa_switch *, int, struct net_device *);
    void (*port_bridge_leave)(struct dsa_switch *, int, struct net_device *);
    int (*port_bridge_tx_fwd_offload)(struct dsa_switch *, int, struct net_device *, int);
    void (*port_bridge_tx_fwd_unoffload)(struct dsa_switch *, int, struct net_device *, int);
    void (*port_stp_state_set)(struct dsa_switch *, int, u8);
    void (*port_fast_age)(struct dsa_switch *, int);
    int (*port_pre_bridge_flags)(struct dsa_switch *, int, struct switchdev_brport_flags, struct netlink_ext_ack *);
    int (*port_bridge_flags)(struct dsa_switch *, int, struct switchdev_brport_flags, struct netlink_ext_ack *);
    int (*port_vlan_filtering)(struct dsa_switch *, int, bool, struct netlink_ext_ack *);
    int (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *, struct netlink_ext_ack *);
    int (*port_vlan_del)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_fdb_add)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_del)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_dump)(struct dsa_switch *, int, dsa_fdb_dump_cb_t *, void *);
    int (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*port_mdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*get_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *);
    int (*cls_flower_add)(struct dsa_switch *, int, struct flow_cls_offload *, bool);
    int (*cls_flower_del)(struct dsa_switch *, int, struct flow_cls_offload *, bool);
    int (*cls_flower_stats)(struct dsa_switch *, int, struct flow_cls_offload *, bool);
    int (*port_mirror_add)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *, bool);
    void (*port_mirror_del)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *);
    int (*port_policer_add)(struct dsa_switch *, int, struct dsa_mall_policer_tc_entry *);
    void (*port_policer_del)(struct dsa_switch *, int);
    int (*port_setup_tc)(struct dsa_switch *, int, enum tc_setup_type, void *);
    int (*crosschip_bridge_join)(struct dsa_switch *, int, int, int, struct net_device *);
    void (*crosschip_bridge_leave)(struct dsa_switch *, int, int, int, struct net_device *);
    int (*crosschip_lag_change)(struct dsa_switch *, int, int);
    int (*crosschip_lag_join)(struct dsa_switch *, int, int, struct net_device *, struct netdev_lag_upper_info *);
    int (*crosschip_lag_leave)(struct dsa_switch *, int, int, struct net_device *);
    int (*port_hwtstamp_get)(struct dsa_switch *, int, struct ifreq *);
    int (*port_hwtstamp_set)(struct dsa_switch *, int, struct ifreq *);
    void (*port_txtstamp)(struct dsa_switch *, int, struct sk_buff *);
    bool (*port_rxtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    int (*devlink_param_get)(struct dsa_switch *, u32, struct devlink_param_gset_ctx *);
    int (*devlink_param_set)(struct dsa_switch *, u32, struct devlink_param_gset_ctx *);
    int (*devlink_info_get)(struct dsa_switch *, struct devlink_info_req *, struct netlink_ext_ack *);
    int (*devlink_sb_pool_get)(struct dsa_switch *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*devlink_sb_pool_set)(struct dsa_switch *, unsigned int, u16, u32, enum devlink_sb_threshold_type, struct netlink_ext_ack *);
    int (*devlink_sb_port_pool_get)(struct dsa_switch *, int, unsigned int, u16, u32 *);
    int (*devlink_sb_port_pool_set)(struct dsa_switch *, int, unsigned int, u16, u32, struct netlink_ext_ack *);
    int (*devlink_sb_tc_pool_bind_get)(struct dsa_switch *, int, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*devlink_sb_tc_pool_bind_set)(struct dsa_switch *, int, unsigned int, u16, enum devlink_sb_pool_type, u16, u32, struct netlink_ext_ack *);
    int (*devlink_sb_occ_snapshot)(struct dsa_switch *, unsigned int);
    int (*devlink_sb_occ_max_clear)(struct dsa_switch *, unsigned int);
    int (*devlink_sb_occ_port_pool_get)(struct dsa_switch *, int, unsigned int, u16, u32 *, u32 *);
    int (*devlink_sb_occ_tc_port_bind_get)(struct dsa_switch *, int, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*port_change_mtu)(struct dsa_switch *, int, int);
    int (*port_max_mtu)(struct dsa_switch *, int);
    int (*port_lag_change)(struct dsa_switch *, int);
    int (*port_lag_join)(struct dsa_switch *, int, struct net_device *, struct netdev_lag_upper_info *);
    int (*port_lag_leave)(struct dsa_switch *, int, struct net_device *);
    int (*port_hsr_join)(struct dsa_switch *, int, struct net_device *);
    int (*port_hsr_leave)(struct dsa_switch *, int, struct net_device *);
    int (*port_mrp_add)(struct dsa_switch *, int, const struct switchdev_obj_mrp *);
    int (*port_mrp_del)(struct dsa_switch *, int, const struct switchdev_obj_mrp *);
    int (*port_mrp_add_ring_role)(struct dsa_switch *, int, const struct switchdev_obj_ring_role_mrp *);
    int (*port_mrp_del_ring_role)(struct dsa_switch *, int, const struct switchdev_obj_ring_role_mrp *);
    int (*tag_8021q_vlan_add)(struct dsa_switch *, int, u16, u16);
    int (*tag_8021q_vlan_del)(struct dsa_switch *, int, u16);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dsa_switch_ops {
    enum dsa_tag_protocol (*get_tag_protocol)(struct dsa_switch *, int, enum dsa_tag_protocol);
    int (*change_tag_protocol)(struct dsa_switch *, enum dsa_tag_protocol);
    int (*connect_tag_protocol)(struct dsa_switch *, enum dsa_tag_protocol);
    int (*setup)(struct dsa_switch *);
    void (*teardown)(struct dsa_switch *);
    int (*port_setup)(struct dsa_switch *, int);
    void (*port_teardown)(struct dsa_switch *, int);
    u32 (*get_phy_flags)(struct dsa_switch *, int);
    int (*phy_read)(struct dsa_switch *, int, int);
    int (*phy_write)(struct dsa_switch *, int, int, u16);
    void (*adjust_link)(struct dsa_switch *, int, struct phy_device *);
    void (*fixed_link_update)(struct dsa_switch *, int, struct fixed_phy_status *);
    void (*phylink_get_caps)(struct dsa_switch *, int, struct phylink_config *);
    void (*phylink_validate)(struct dsa_switch *, int, long unsigned int *, struct phylink_link_state *);
    struct phylink_pcs * (*phylink_mac_select_pcs)(struct dsa_switch *, int, phy_interface_t);
    int (*phylink_mac_link_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*phylink_mac_config)(struct dsa_switch *, int, unsigned int, const struct phylink_link_state *);
    void (*phylink_mac_an_restart)(struct dsa_switch *, int);
    void (*phylink_mac_link_down)(struct dsa_switch *, int, unsigned int, phy_interface_t);
    void (*phylink_mac_link_up)(struct dsa_switch *, int, unsigned int, phy_interface_t, struct phy_device *, int, int, bool, bool);
    void (*phylink_fixed_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*get_strings)(struct dsa_switch *, int, u32, uint8_t *);
    void (*get_ethtool_stats)(struct dsa_switch *, int, uint64_t *);
    int (*get_sset_count)(struct dsa_switch *, int, int);
    void (*get_ethtool_phy_stats)(struct dsa_switch *, int, uint64_t *);
    void (*get_eth_phy_stats)(struct dsa_switch *, int, struct ethtool_eth_phy_stats *);
    void (*get_eth_mac_stats)(struct dsa_switch *, int, struct ethtool_eth_mac_stats *);
    void (*get_eth_ctrl_stats)(struct dsa_switch *, int, struct ethtool_eth_ctrl_stats *);
    void (*get_stats64)(struct dsa_switch *, int, struct rtnl_link_stats64 *);
    void (*self_test)(struct dsa_switch *, int, struct ethtool_test *, u64 *);
    void (*get_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*set_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*get_ts_info)(struct dsa_switch *, int, struct ethtool_ts_info *);
    int (*port_get_default_prio)(struct dsa_switch *, int);
    int (*port_set_default_prio)(struct dsa_switch *, int, u8);
    int (*port_get_dscp_prio)(struct dsa_switch *, int, u8);
    int (*port_add_dscp_prio)(struct dsa_switch *, int, u8, u8);
    int (*port_del_dscp_prio)(struct dsa_switch *, int, u8, u8);
    int (*suspend)(struct dsa_switch *);
    int (*resume)(struct dsa_switch *);
    int (*port_enable)(struct dsa_switch *, int, struct phy_device *);
    void (*port_disable)(struct dsa_switch *, int);
    int (*set_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_eeprom_len)(struct dsa_switch *);
    int (*get_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*get_regs_len)(struct dsa_switch *, int);
    void (*get_regs)(struct dsa_switch *, int, struct ethtool_regs *, void *);
    int (*port_prechangeupper)(struct dsa_switch *, int, struct netdev_notifier_changeupper_info *);
    int (*set_ageing_time)(struct dsa_switch *, unsigned int);
    int (*port_bridge_join)(struct dsa_switch *, int, struct dsa_bridge, bool *, struct netlink_ext_ack *);
    void (*port_bridge_leave)(struct dsa_switch *, int, struct dsa_bridge);
    void (*port_stp_state_set)(struct dsa_switch *, int, u8);
    int (*port_mst_state_set)(struct dsa_switch *, int, const struct switchdev_mst_state *);
    void (*port_fast_age)(struct dsa_switch *, int);
    int (*port_vlan_fast_age)(struct dsa_switch *, int, u16);
    int (*port_pre_bridge_flags)(struct dsa_switch *, int, struct switchdev_brport_flags, struct netlink_ext_ack *);
    int (*port_bridge_flags)(struct dsa_switch *, int, struct switchdev_brport_flags, struct netlink_ext_ack *);
    void (*port_set_host_flood)(struct dsa_switch *, int, bool, bool);
    int (*port_vlan_filtering)(struct dsa_switch *, int, bool, struct netlink_ext_ack *);
    int (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *, struct netlink_ext_ack *);
    int (*port_vlan_del)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*vlan_msti_set)(struct dsa_switch *, struct dsa_bridge, const struct switchdev_vlan_msti *);
    int (*port_fdb_add)(struct dsa_switch *, int, const unsigned char *, u16, struct dsa_db);
    int (*port_fdb_del)(struct dsa_switch *, int, const unsigned char *, u16, struct dsa_db);
    int (*port_fdb_dump)(struct dsa_switch *, int, dsa_fdb_dump_cb_t *, void *);
    int (*lag_fdb_add)(struct dsa_switch *, struct dsa_lag, const unsigned char *, u16, struct dsa_db);
    int (*lag_fdb_del)(struct dsa_switch *, struct dsa_lag, const unsigned char *, u16, struct dsa_db);
    int (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *, struct dsa_db);
    int (*port_mdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *, struct dsa_db);
    int (*get_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *);
    int (*cls_flower_add)(struct dsa_switch *, int, struct flow_cls_offload *, bool);
    int (*cls_flower_del)(struct dsa_switch *, int, struct flow_cls_offload *, bool);
    int (*cls_flower_stats)(struct dsa_switch *, int, struct flow_cls_offload *, bool);
    int (*port_mirror_add)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *, bool, struct netlink_ext_ack *);
    void (*port_mirror_del)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *);
    int (*port_policer_add)(struct dsa_switch *, int, struct dsa_mall_policer_tc_entry *);
    void (*port_policer_del)(struct dsa_switch *, int);
    int (*port_setup_tc)(struct dsa_switch *, int, enum tc_setup_type, void *);
    int (*crosschip_bridge_join)(struct dsa_switch *, int, int, int, struct dsa_bridge, struct netlink_ext_ack *);
    void (*crosschip_bridge_leave)(struct dsa_switch *, int, int, int, struct dsa_bridge);
    int (*crosschip_lag_change)(struct dsa_switch *, int, int);
    int (*crosschip_lag_join)(struct dsa_switch *, int, int, struct dsa_lag, struct netdev_lag_upper_info *);
    int (*crosschip_lag_leave)(struct dsa_switch *, int, int, struct dsa_lag);
    int (*port_hwtstamp_get)(struct dsa_switch *, int, struct ifreq *);
    int (*port_hwtstamp_set)(struct dsa_switch *, int, struct ifreq *);
    void (*port_txtstamp)(struct dsa_switch *, int, struct sk_buff *);
    bool (*port_rxtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    int (*devlink_param_get)(struct dsa_switch *, u32, struct devlink_param_gset_ctx *);
    int (*devlink_param_set)(struct dsa_switch *, u32, struct devlink_param_gset_ctx *);
    int (*devlink_info_get)(struct dsa_switch *, struct devlink_info_req *, struct netlink_ext_ack *);
    int (*devlink_sb_pool_get)(struct dsa_switch *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*devlink_sb_pool_set)(struct dsa_switch *, unsigned int, u16, u32, enum devlink_sb_threshold_type, struct netlink_ext_ack *);
    int (*devlink_sb_port_pool_get)(struct dsa_switch *, int, unsigned int, u16, u32 *);
    int (*devlink_sb_port_pool_set)(struct dsa_switch *, int, unsigned int, u16, u32, struct netlink_ext_ack *);
    int (*devlink_sb_tc_pool_bind_get)(struct dsa_switch *, int, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*devlink_sb_tc_pool_bind_set)(struct dsa_switch *, int, unsigned int, u16, enum devlink_sb_pool_type, u16, u32, struct netlink_ext_ack *);
    int (*devlink_sb_occ_snapshot)(struct dsa_switch *, unsigned int);
    int (*devlink_sb_occ_max_clear)(struct dsa_switch *, unsigned int);
    int (*devlink_sb_occ_port_pool_get)(struct dsa_switch *, int, unsigned int, u16, u32 *, u32 *);
    int (*devlink_sb_occ_tc_port_bind_get)(struct dsa_switch *, int, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*port_change_mtu)(struct dsa_switch *, int, int);
    int (*port_max_mtu)(struct dsa_switch *, int);
    int (*port_lag_change)(struct dsa_switch *, int);
    int (*port_lag_join)(struct dsa_switch *, int, struct dsa_lag, struct netdev_lag_upper_info *);
    int (*port_lag_leave)(struct dsa_switch *, int, struct dsa_lag);
    int (*port_hsr_join)(struct dsa_switch *, int, struct net_device *);
    int (*port_hsr_leave)(struct dsa_switch *, int, struct net_device *);
    int (*port_mrp_add)(struct dsa_switch *, int, const struct switchdev_obj_mrp *);
    int (*port_mrp_del)(struct dsa_switch *, int, const struct switchdev_obj_mrp *);
    int (*port_mrp_add_ring_role)(struct dsa_switch *, int, const struct switchdev_obj_ring_role_mrp *);
    int (*port_mrp_del_ring_role)(struct dsa_switch *, int, const struct switchdev_obj_ring_role_mrp *);
    int (*tag_8021q_vlan_add)(struct dsa_switch *, int, u16, u16);
    int (*tag_8021q_vlan_del)(struct dsa_switch *, int, u16);
    void (*master_state_change)(struct dsa_switch *, const struct net_device *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dsa_switch_ops {
    enum dsa_tag_protocol (*get_tag_protocol)(struct dsa_switch *, int, enum dsa_tag_protocol);
    int (*change_tag_protocol)(struct dsa_switch *, enum dsa_tag_protocol);
    int (*connect_tag_protocol)(struct dsa_switch *, enum dsa_tag_protocol);
    int (*port_change_master)(struct dsa_switch *, int, struct net_device *, struct netlink_ext_ack *);
    int (*setup)(struct dsa_switch *);
    void (*teardown)(struct dsa_switch *);
    int (*port_setup)(struct dsa_switch *, int);
    void (*port_teardown)(struct dsa_switch *, int);
    u32 (*get_phy_flags)(struct dsa_switch *, int);
    int (*phy_read)(struct dsa_switch *, int, int);
    int (*phy_write)(struct dsa_switch *, int, int, u16);
    void (*adjust_link)(struct dsa_switch *, int, struct phy_device *);
    void (*fixed_link_update)(struct dsa_switch *, int, struct fixed_phy_status *);
    void (*phylink_get_caps)(struct dsa_switch *, int, struct phylink_config *);
    struct phylink_pcs * (*phylink_mac_select_pcs)(struct dsa_switch *, int, phy_interface_t);
    int (*phylink_mac_link_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*phylink_mac_config)(struct dsa_switch *, int, unsigned int, const struct phylink_link_state *);
    void (*phylink_mac_an_restart)(struct dsa_switch *, int);
    void (*phylink_mac_link_down)(struct dsa_switch *, int, unsigned int, phy_interface_t);
    void (*phylink_mac_link_up)(struct dsa_switch *, int, unsigned int, phy_interface_t, struct phy_device *, int, int, bool, bool);
    void (*phylink_fixed_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*get_strings)(struct dsa_switch *, int, u32, uint8_t *);
    void (*get_ethtool_stats)(struct dsa_switch *, int, uint64_t *);
    int (*get_sset_count)(struct dsa_switch *, int, int);
    void (*get_ethtool_phy_stats)(struct dsa_switch *, int, uint64_t *);
    void (*get_eth_phy_stats)(struct dsa_switch *, int, struct ethtool_eth_phy_stats *);
    void (*get_eth_mac_stats)(struct dsa_switch *, int, struct ethtool_eth_mac_stats *);
    void (*get_eth_ctrl_stats)(struct dsa_switch *, int, struct ethtool_eth_ctrl_stats *);
    void (*get_rmon_stats)(struct dsa_switch *, int, struct ethtool_rmon_stats *, const struct ethtool_rmon_hist_range **);
    void (*get_stats64)(struct dsa_switch *, int, struct rtnl_link_stats64 *);
    void (*get_pause_stats)(struct dsa_switch *, int, struct ethtool_pause_stats *);
    void (*self_test)(struct dsa_switch *, int, struct ethtool_test *, u64 *);
    void (*get_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*set_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*get_ts_info)(struct dsa_switch *, int, struct ethtool_ts_info *);
    int (*port_get_default_prio)(struct dsa_switch *, int);
    int (*port_set_default_prio)(struct dsa_switch *, int, u8);
    int (*port_get_dscp_prio)(struct dsa_switch *, int, u8);
    int (*port_add_dscp_prio)(struct dsa_switch *, int, u8, u8);
    int (*port_del_dscp_prio)(struct dsa_switch *, int, u8, u8);
    int (*suspend)(struct dsa_switch *);
    int (*resume)(struct dsa_switch *);
    int (*port_enable)(struct dsa_switch *, int, struct phy_device *);
    void (*port_disable)(struct dsa_switch *, int);
    int (*set_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_eeprom_len)(struct dsa_switch *);
    int (*get_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*get_regs_len)(struct dsa_switch *, int);
    void (*get_regs)(struct dsa_switch *, int, struct ethtool_regs *, void *);
    int (*port_prechangeupper)(struct dsa_switch *, int, struct netdev_notifier_changeupper_info *);
    int (*set_ageing_time)(struct dsa_switch *, unsigned int);
    int (*port_bridge_join)(struct dsa_switch *, int, struct dsa_bridge, bool *, struct netlink_ext_ack *);
    void (*port_bridge_leave)(struct dsa_switch *, int, struct dsa_bridge);
    void (*port_stp_state_set)(struct dsa_switch *, int, u8);
    int (*port_mst_state_set)(struct dsa_switch *, int, const struct switchdev_mst_state *);
    void (*port_fast_age)(struct dsa_switch *, int);
    int (*port_vlan_fast_age)(struct dsa_switch *, int, u16);
    int (*port_pre_bridge_flags)(struct dsa_switch *, int, struct switchdev_brport_flags, struct netlink_ext_ack *);
    int (*port_bridge_flags)(struct dsa_switch *, int, struct switchdev_brport_flags, struct netlink_ext_ack *);
    void (*port_set_host_flood)(struct dsa_switch *, int, bool, bool);
    int (*port_vlan_filtering)(struct dsa_switch *, int, bool, struct netlink_ext_ack *);
    int (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *, struct netlink_ext_ack *);
    int (*port_vlan_del)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*vlan_msti_set)(struct dsa_switch *, struct dsa_bridge, const struct switchdev_vlan_msti *);
    int (*port_fdb_add)(struct dsa_switch *, int, const unsigned char *, u16, struct dsa_db);
    int (*port_fdb_del)(struct dsa_switch *, int, const unsigned char *, u16, struct dsa_db);
    int (*port_fdb_dump)(struct dsa_switch *, int, dsa_fdb_dump_cb_t *, void *);
    int (*lag_fdb_add)(struct dsa_switch *, struct dsa_lag, const unsigned char *, u16, struct dsa_db);
    int (*lag_fdb_del)(struct dsa_switch *, struct dsa_lag, const unsigned char *, u16, struct dsa_db);
    int (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *, struct dsa_db);
    int (*port_mdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *, struct dsa_db);
    int (*get_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *);
    int (*cls_flower_add)(struct dsa_switch *, int, struct flow_cls_offload *, bool);
    int (*cls_flower_del)(struct dsa_switch *, int, struct flow_cls_offload *, bool);
    int (*cls_flower_stats)(struct dsa_switch *, int, struct flow_cls_offload *, bool);
    int (*port_mirror_add)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *, bool, struct netlink_ext_ack *);
    void (*port_mirror_del)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *);
    int (*port_policer_add)(struct dsa_switch *, int, struct dsa_mall_policer_tc_entry *);
    void (*port_policer_del)(struct dsa_switch *, int);
    int (*port_setup_tc)(struct dsa_switch *, int, enum tc_setup_type, void *);
    int (*crosschip_bridge_join)(struct dsa_switch *, int, int, int, struct dsa_bridge, struct netlink_ext_ack *);
    void (*crosschip_bridge_leave)(struct dsa_switch *, int, int, int, struct dsa_bridge);
    int (*crosschip_lag_change)(struct dsa_switch *, int, int);
    int (*crosschip_lag_join)(struct dsa_switch *, int, int, struct dsa_lag, struct netdev_lag_upper_info *, struct netlink_ext_ack *);
    int (*crosschip_lag_leave)(struct dsa_switch *, int, int, struct dsa_lag);
    int (*port_hwtstamp_get)(struct dsa_switch *, int, struct ifreq *);
    int (*port_hwtstamp_set)(struct dsa_switch *, int, struct ifreq *);
    void (*port_txtstamp)(struct dsa_switch *, int, struct sk_buff *);
    bool (*port_rxtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    int (*devlink_param_get)(struct dsa_switch *, u32, struct devlink_param_gset_ctx *);
    int (*devlink_param_set)(struct dsa_switch *, u32, struct devlink_param_gset_ctx *);
    int (*devlink_info_get)(struct dsa_switch *, struct devlink_info_req *, struct netlink_ext_ack *);
    int (*devlink_sb_pool_get)(struct dsa_switch *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*devlink_sb_pool_set)(struct dsa_switch *, unsigned int, u16, u32, enum devlink_sb_threshold_type, struct netlink_ext_ack *);
    int (*devlink_sb_port_pool_get)(struct dsa_switch *, int, unsigned int, u16, u32 *);
    int (*devlink_sb_port_pool_set)(struct dsa_switch *, int, unsigned int, u16, u32, struct netlink_ext_ack *);
    int (*devlink_sb_tc_pool_bind_get)(struct dsa_switch *, int, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*devlink_sb_tc_pool_bind_set)(struct dsa_switch *, int, unsigned int, u16, enum devlink_sb_pool_type, u16, u32, struct netlink_ext_ack *);
    int (*devlink_sb_occ_snapshot)(struct dsa_switch *, unsigned int);
    int (*devlink_sb_occ_max_clear)(struct dsa_switch *, unsigned int);
    int (*devlink_sb_occ_port_pool_get)(struct dsa_switch *, int, unsigned int, u16, u32 *, u32 *);
    int (*devlink_sb_occ_tc_port_bind_get)(struct dsa_switch *, int, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*port_change_mtu)(struct dsa_switch *, int, int);
    int (*port_max_mtu)(struct dsa_switch *, int);
    int (*port_lag_change)(struct dsa_switch *, int);
    int (*port_lag_join)(struct dsa_switch *, int, struct dsa_lag, struct netdev_lag_upper_info *, struct netlink_ext_ack *);
    int (*port_lag_leave)(struct dsa_switch *, int, struct dsa_lag);
    int (*port_hsr_join)(struct dsa_switch *, int, struct net_device *);
    int (*port_hsr_leave)(struct dsa_switch *, int, struct net_device *);
    int (*port_mrp_add)(struct dsa_switch *, int, const struct switchdev_obj_mrp *);
    int (*port_mrp_del)(struct dsa_switch *, int, const struct switchdev_obj_mrp *);
    int (*port_mrp_add_ring_role)(struct dsa_switch *, int, const struct switchdev_obj_ring_role_mrp *);
    int (*port_mrp_del_ring_role)(struct dsa_switch *, int, const struct switchdev_obj_ring_role_mrp *);
    int (*tag_8021q_vlan_add)(struct dsa_switch *, int, u16, u16);
    int (*tag_8021q_vlan_del)(struct dsa_switch *, int, u16);
    void (*master_state_change)(struct dsa_switch *, const struct net_device *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dsa_switch_ops {
    enum dsa_tag_protocol (*get_tag_protocol)(struct dsa_switch *, int, enum dsa_tag_protocol);
    int (*change_tag_protocol)(struct dsa_switch *, enum dsa_tag_protocol);
    int (*connect_tag_protocol)(struct dsa_switch *, enum dsa_tag_protocol);
    int (*port_change_master)(struct dsa_switch *, int, struct net_device *, struct netlink_ext_ack *);
    int (*setup)(struct dsa_switch *);
    void (*teardown)(struct dsa_switch *);
    int (*port_setup)(struct dsa_switch *, int);
    void (*port_teardown)(struct dsa_switch *, int);
    u32 (*get_phy_flags)(struct dsa_switch *, int);
    int (*phy_read)(struct dsa_switch *, int, int);
    int (*phy_write)(struct dsa_switch *, int, int, u16);
    void (*adjust_link)(struct dsa_switch *, int, struct phy_device *);
    void (*fixed_link_update)(struct dsa_switch *, int, struct fixed_phy_status *);
    void (*phylink_get_caps)(struct dsa_switch *, int, struct phylink_config *);
    struct phylink_pcs * (*phylink_mac_select_pcs)(struct dsa_switch *, int, phy_interface_t);
    int (*phylink_mac_link_state)(struct dsa_switch *, int, struct phylink_link_state *);
    int (*phylink_mac_prepare)(struct dsa_switch *, int, unsigned int, phy_interface_t);
    void (*phylink_mac_config)(struct dsa_switch *, int, unsigned int, const struct phylink_link_state *);
    int (*phylink_mac_finish)(struct dsa_switch *, int, unsigned int, phy_interface_t);
    void (*phylink_mac_an_restart)(struct dsa_switch *, int);
    void (*phylink_mac_link_down)(struct dsa_switch *, int, unsigned int, phy_interface_t);
    void (*phylink_mac_link_up)(struct dsa_switch *, int, unsigned int, phy_interface_t, struct phy_device *, int, int, bool, bool);
    void (*phylink_fixed_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*get_strings)(struct dsa_switch *, int, u32, uint8_t *);
    void (*get_ethtool_stats)(struct dsa_switch *, int, uint64_t *);
    int (*get_sset_count)(struct dsa_switch *, int, int);
    void (*get_ethtool_phy_stats)(struct dsa_switch *, int, uint64_t *);
    void (*get_eth_phy_stats)(struct dsa_switch *, int, struct ethtool_eth_phy_stats *);
    void (*get_eth_mac_stats)(struct dsa_switch *, int, struct ethtool_eth_mac_stats *);
    void (*get_eth_ctrl_stats)(struct dsa_switch *, int, struct ethtool_eth_ctrl_stats *);
    void (*get_rmon_stats)(struct dsa_switch *, int, struct ethtool_rmon_stats *, const struct ethtool_rmon_hist_range **);
    void (*get_stats64)(struct dsa_switch *, int, struct rtnl_link_stats64 *);
    void (*get_pause_stats)(struct dsa_switch *, int, struct ethtool_pause_stats *);
    void (*self_test)(struct dsa_switch *, int, struct ethtool_test *, u64 *);
    void (*get_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*set_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*get_ts_info)(struct dsa_switch *, int, struct ethtool_ts_info *);
    int (*get_mm)(struct dsa_switch *, int, struct ethtool_mm_state *);
    int (*set_mm)(struct dsa_switch *, int, struct ethtool_mm_cfg *, struct netlink_ext_ack *);
    void (*get_mm_stats)(struct dsa_switch *, int, struct ethtool_mm_stats *);
    int (*port_get_default_prio)(struct dsa_switch *, int);
    int (*port_set_default_prio)(struct dsa_switch *, int, u8);
    int (*port_get_dscp_prio)(struct dsa_switch *, int, u8);
    int (*port_add_dscp_prio)(struct dsa_switch *, int, u8, u8);
    int (*port_del_dscp_prio)(struct dsa_switch *, int, u8, u8);
    int (*suspend)(struct dsa_switch *);
    int (*resume)(struct dsa_switch *);
    int (*port_enable)(struct dsa_switch *, int, struct phy_device *);
    void (*port_disable)(struct dsa_switch *, int);
    struct dsa_port * (*preferred_default_local_cpu_port)(struct dsa_switch *);
    int (*set_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_eeprom_len)(struct dsa_switch *);
    int (*get_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*get_regs_len)(struct dsa_switch *, int);
    void (*get_regs)(struct dsa_switch *, int, struct ethtool_regs *, void *);
    int (*port_prechangeupper)(struct dsa_switch *, int, struct netdev_notifier_changeupper_info *);
    int (*set_ageing_time)(struct dsa_switch *, unsigned int);
    int (*port_bridge_join)(struct dsa_switch *, int, struct dsa_bridge, bool *, struct netlink_ext_ack *);
    void (*port_bridge_leave)(struct dsa_switch *, int, struct dsa_bridge);
    void (*port_stp_state_set)(struct dsa_switch *, int, u8);
    int (*port_mst_state_set)(struct dsa_switch *, int, const struct switchdev_mst_state *);
    void (*port_fast_age)(struct dsa_switch *, int);
    int (*port_vlan_fast_age)(struct dsa_switch *, int, u16);
    int (*port_pre_bridge_flags)(struct dsa_switch *, int, struct switchdev_brport_flags, struct netlink_ext_ack *);
    int (*port_bridge_flags)(struct dsa_switch *, int, struct switchdev_brport_flags, struct netlink_ext_ack *);
    void (*port_set_host_flood)(struct dsa_switch *, int, bool, bool);
    int (*port_vlan_filtering)(struct dsa_switch *, int, bool, struct netlink_ext_ack *);
    int (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *, struct netlink_ext_ack *);
    int (*port_vlan_del)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*vlan_msti_set)(struct dsa_switch *, struct dsa_bridge, const struct switchdev_vlan_msti *);
    int (*port_fdb_add)(struct dsa_switch *, int, const unsigned char *, u16, struct dsa_db);
    int (*port_fdb_del)(struct dsa_switch *, int, const unsigned char *, u16, struct dsa_db);
    int (*port_fdb_dump)(struct dsa_switch *, int, dsa_fdb_dump_cb_t *, void *);
    int (*lag_fdb_add)(struct dsa_switch *, struct dsa_lag, const unsigned char *, u16, struct dsa_db);
    int (*lag_fdb_del)(struct dsa_switch *, struct dsa_lag, const unsigned char *, u16, struct dsa_db);
    int (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *, struct dsa_db);
    int (*port_mdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *, struct dsa_db);
    int (*get_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *);
    int (*cls_flower_add)(struct dsa_switch *, int, struct flow_cls_offload *, bool);
    int (*cls_flower_del)(struct dsa_switch *, int, struct flow_cls_offload *, bool);
    int (*cls_flower_stats)(struct dsa_switch *, int, struct flow_cls_offload *, bool);
    int (*port_mirror_add)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *, bool, struct netlink_ext_ack *);
    void (*port_mirror_del)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *);
    int (*port_policer_add)(struct dsa_switch *, int, struct dsa_mall_policer_tc_entry *);
    void (*port_policer_del)(struct dsa_switch *, int);
    int (*port_setup_tc)(struct dsa_switch *, int, enum tc_setup_type, void *);
    int (*crosschip_bridge_join)(struct dsa_switch *, int, int, int, struct dsa_bridge, struct netlink_ext_ack *);
    void (*crosschip_bridge_leave)(struct dsa_switch *, int, int, int, struct dsa_bridge);
    int (*crosschip_lag_change)(struct dsa_switch *, int, int);
    int (*crosschip_lag_join)(struct dsa_switch *, int, int, struct dsa_lag, struct netdev_lag_upper_info *, struct netlink_ext_ack *);
    int (*crosschip_lag_leave)(struct dsa_switch *, int, int, struct dsa_lag);
    int (*port_hwtstamp_get)(struct dsa_switch *, int, struct ifreq *);
    int (*port_hwtstamp_set)(struct dsa_switch *, int, struct ifreq *);
    void (*port_txtstamp)(struct dsa_switch *, int, struct sk_buff *);
    bool (*port_rxtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    int (*devlink_param_get)(struct dsa_switch *, u32, struct devlink_param_gset_ctx *);
    int (*devlink_param_set)(struct dsa_switch *, u32, struct devlink_param_gset_ctx *);
    int (*devlink_info_get)(struct dsa_switch *, struct devlink_info_req *, struct netlink_ext_ack *);
    int (*devlink_sb_pool_get)(struct dsa_switch *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*devlink_sb_pool_set)(struct dsa_switch *, unsigned int, u16, u32, enum devlink_sb_threshold_type, struct netlink_ext_ack *);
    int (*devlink_sb_port_pool_get)(struct dsa_switch *, int, unsigned int, u16, u32 *);
    int (*devlink_sb_port_pool_set)(struct dsa_switch *, int, unsigned int, u16, u32, struct netlink_ext_ack *);
    int (*devlink_sb_tc_pool_bind_get)(struct dsa_switch *, int, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*devlink_sb_tc_pool_bind_set)(struct dsa_switch *, int, unsigned int, u16, enum devlink_sb_pool_type, u16, u32, struct netlink_ext_ack *);
    int (*devlink_sb_occ_snapshot)(struct dsa_switch *, unsigned int);
    int (*devlink_sb_occ_max_clear)(struct dsa_switch *, unsigned int);
    int (*devlink_sb_occ_port_pool_get)(struct dsa_switch *, int, unsigned int, u16, u32 *, u32 *);
    int (*devlink_sb_occ_tc_port_bind_get)(struct dsa_switch *, int, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*port_change_mtu)(struct dsa_switch *, int, int);
    int (*port_max_mtu)(struct dsa_switch *, int);
    int (*port_lag_change)(struct dsa_switch *, int);
    int (*port_lag_join)(struct dsa_switch *, int, struct dsa_lag, struct netdev_lag_upper_info *, struct netlink_ext_ack *);
    int (*port_lag_leave)(struct dsa_switch *, int, struct dsa_lag);
    int (*port_hsr_join)(struct dsa_switch *, int, struct net_device *);
    int (*port_hsr_leave)(struct dsa_switch *, int, struct net_device *);
    int (*port_mrp_add)(struct dsa_switch *, int, const struct switchdev_obj_mrp *);
    int (*port_mrp_del)(struct dsa_switch *, int, const struct switchdev_obj_mrp *);
    int (*port_mrp_add_ring_role)(struct dsa_switch *, int, const struct switchdev_obj_ring_role_mrp *);
    int (*port_mrp_del_ring_role)(struct dsa_switch *, int, const struct switchdev_obj_ring_role_mrp *);
    int (*tag_8021q_vlan_add)(struct dsa_switch *, int, u16, u16);
    int (*tag_8021q_vlan_del)(struct dsa_switch *, int, u16);
    void (*master_state_change)(struct dsa_switch *, const struct net_device *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dsa_switch_ops {
    enum dsa_tag_protocol (*get_tag_protocol)(struct dsa_switch *, int, enum dsa_tag_protocol);
    int (*change_tag_protocol)(struct dsa_switch *, enum dsa_tag_protocol);
    int (*connect_tag_protocol)(struct dsa_switch *, enum dsa_tag_protocol);
    int (*port_change_conduit)(struct dsa_switch *, int, struct net_device *, struct netlink_ext_ack *);
    int (*setup)(struct dsa_switch *);
    void (*teardown)(struct dsa_switch *);
    int (*port_setup)(struct dsa_switch *, int);
    void (*port_teardown)(struct dsa_switch *, int);
    u32 (*get_phy_flags)(struct dsa_switch *, int);
    int (*phy_read)(struct dsa_switch *, int, int);
    int (*phy_write)(struct dsa_switch *, int, int, u16);
    void (*adjust_link)(struct dsa_switch *, int, struct phy_device *);
    void (*fixed_link_update)(struct dsa_switch *, int, struct fixed_phy_status *);
    void (*phylink_get_caps)(struct dsa_switch *, int, struct phylink_config *);
    struct phylink_pcs * (*phylink_mac_select_pcs)(struct dsa_switch *, int, phy_interface_t);
    int (*phylink_mac_prepare)(struct dsa_switch *, int, unsigned int, phy_interface_t);
    void (*phylink_mac_config)(struct dsa_switch *, int, unsigned int, const struct phylink_link_state *);
    int (*phylink_mac_finish)(struct dsa_switch *, int, unsigned int, phy_interface_t);
    void (*phylink_mac_link_down)(struct dsa_switch *, int, unsigned int, phy_interface_t);
    void (*phylink_mac_link_up)(struct dsa_switch *, int, unsigned int, phy_interface_t, struct phy_device *, int, int, bool, bool);
    void (*phylink_fixed_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*get_strings)(struct dsa_switch *, int, u32, uint8_t *);
    void (*get_ethtool_stats)(struct dsa_switch *, int, uint64_t *);
    int (*get_sset_count)(struct dsa_switch *, int, int);
    void (*get_ethtool_phy_stats)(struct dsa_switch *, int, uint64_t *);
    void (*get_eth_phy_stats)(struct dsa_switch *, int, struct ethtool_eth_phy_stats *);
    void (*get_eth_mac_stats)(struct dsa_switch *, int, struct ethtool_eth_mac_stats *);
    void (*get_eth_ctrl_stats)(struct dsa_switch *, int, struct ethtool_eth_ctrl_stats *);
    void (*get_rmon_stats)(struct dsa_switch *, int, struct ethtool_rmon_stats *, const struct ethtool_rmon_hist_range **);
    void (*get_stats64)(struct dsa_switch *, int, struct rtnl_link_stats64 *);
    void (*get_pause_stats)(struct dsa_switch *, int, struct ethtool_pause_stats *);
    void (*self_test)(struct dsa_switch *, int, struct ethtool_test *, u64 *);
    void (*get_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*set_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*get_ts_info)(struct dsa_switch *, int, struct ethtool_ts_info *);
    int (*get_mm)(struct dsa_switch *, int, struct ethtool_mm_state *);
    int (*set_mm)(struct dsa_switch *, int, struct ethtool_mm_cfg *, struct netlink_ext_ack *);
    void (*get_mm_stats)(struct dsa_switch *, int, struct ethtool_mm_stats *);
    int (*port_get_default_prio)(struct dsa_switch *, int);
    int (*port_set_default_prio)(struct dsa_switch *, int, u8);
    int (*port_get_dscp_prio)(struct dsa_switch *, int, u8);
    int (*port_add_dscp_prio)(struct dsa_switch *, int, u8, u8);
    int (*port_del_dscp_prio)(struct dsa_switch *, int, u8, u8);
    int (*suspend)(struct dsa_switch *);
    int (*resume)(struct dsa_switch *);
    int (*port_enable)(struct dsa_switch *, int, struct phy_device *);
    void (*port_disable)(struct dsa_switch *, int);
    int (*port_set_mac_address)(struct dsa_switch *, int, const unsigned char *);
    struct dsa_port * (*preferred_default_local_cpu_port)(struct dsa_switch *);
    int (*set_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_eeprom_len)(struct dsa_switch *);
    int (*get_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*get_regs_len)(struct dsa_switch *, int);
    void (*get_regs)(struct dsa_switch *, int, struct ethtool_regs *, void *);
    int (*port_prechangeupper)(struct dsa_switch *, int, struct netdev_notifier_changeupper_info *);
    int (*set_ageing_time)(struct dsa_switch *, unsigned int);
    int (*port_bridge_join)(struct dsa_switch *, int, struct dsa_bridge, bool *, struct netlink_ext_ack *);
    void (*port_bridge_leave)(struct dsa_switch *, int, struct dsa_bridge);
    void (*port_stp_state_set)(struct dsa_switch *, int, u8);
    int (*port_mst_state_set)(struct dsa_switch *, int, const struct switchdev_mst_state *);
    void (*port_fast_age)(struct dsa_switch *, int);
    int (*port_vlan_fast_age)(struct dsa_switch *, int, u16);
    int (*port_pre_bridge_flags)(struct dsa_switch *, int, struct switchdev_brport_flags, struct netlink_ext_ack *);
    int (*port_bridge_flags)(struct dsa_switch *, int, struct switchdev_brport_flags, struct netlink_ext_ack *);
    void (*port_set_host_flood)(struct dsa_switch *, int, bool, bool);
    int (*port_vlan_filtering)(struct dsa_switch *, int, bool, struct netlink_ext_ack *);
    int (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *, struct netlink_ext_ack *);
    int (*port_vlan_del)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*vlan_msti_set)(struct dsa_switch *, struct dsa_bridge, const struct switchdev_vlan_msti *);
    int (*port_fdb_add)(struct dsa_switch *, int, const unsigned char *, u16, struct dsa_db);
    int (*port_fdb_del)(struct dsa_switch *, int, const unsigned char *, u16, struct dsa_db);
    int (*port_fdb_dump)(struct dsa_switch *, int, dsa_fdb_dump_cb_t *, void *);
    int (*lag_fdb_add)(struct dsa_switch *, struct dsa_lag, const unsigned char *, u16, struct dsa_db);
    int (*lag_fdb_del)(struct dsa_switch *, struct dsa_lag, const unsigned char *, u16, struct dsa_db);
    int (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *, struct dsa_db);
    int (*port_mdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *, struct dsa_db);
    int (*get_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *);
    int (*cls_flower_add)(struct dsa_switch *, int, struct flow_cls_offload *, bool);
    int (*cls_flower_del)(struct dsa_switch *, int, struct flow_cls_offload *, bool);
    int (*cls_flower_stats)(struct dsa_switch *, int, struct flow_cls_offload *, bool);
    int (*port_mirror_add)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *, bool, struct netlink_ext_ack *);
    void (*port_mirror_del)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *);
    int (*port_policer_add)(struct dsa_switch *, int, struct dsa_mall_policer_tc_entry *);
    void (*port_policer_del)(struct dsa_switch *, int);
    int (*port_setup_tc)(struct dsa_switch *, int, enum tc_setup_type, void *);
    int (*crosschip_bridge_join)(struct dsa_switch *, int, int, int, struct dsa_bridge, struct netlink_ext_ack *);
    void (*crosschip_bridge_leave)(struct dsa_switch *, int, int, int, struct dsa_bridge);
    int (*crosschip_lag_change)(struct dsa_switch *, int, int);
    int (*crosschip_lag_join)(struct dsa_switch *, int, int, struct dsa_lag, struct netdev_lag_upper_info *, struct netlink_ext_ack *);
    int (*crosschip_lag_leave)(struct dsa_switch *, int, int, struct dsa_lag);
    int (*port_hwtstamp_get)(struct dsa_switch *, int, struct ifreq *);
    int (*port_hwtstamp_set)(struct dsa_switch *, int, struct ifreq *);
    void (*port_txtstamp)(struct dsa_switch *, int, struct sk_buff *);
    bool (*port_rxtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    int (*devlink_param_get)(struct dsa_switch *, u32, struct devlink_param_gset_ctx *);
    int (*devlink_param_set)(struct dsa_switch *, u32, struct devlink_param_gset_ctx *);
    int (*devlink_info_get)(struct dsa_switch *, struct devlink_info_req *, struct netlink_ext_ack *);
    int (*devlink_sb_pool_get)(struct dsa_switch *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*devlink_sb_pool_set)(struct dsa_switch *, unsigned int, u16, u32, enum devlink_sb_threshold_type, struct netlink_ext_ack *);
    int (*devlink_sb_port_pool_get)(struct dsa_switch *, int, unsigned int, u16, u32 *);
    int (*devlink_sb_port_pool_set)(struct dsa_switch *, int, unsigned int, u16, u32, struct netlink_ext_ack *);
    int (*devlink_sb_tc_pool_bind_get)(struct dsa_switch *, int, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*devlink_sb_tc_pool_bind_set)(struct dsa_switch *, int, unsigned int, u16, enum devlink_sb_pool_type, u16, u32, struct netlink_ext_ack *);
    int (*devlink_sb_occ_snapshot)(struct dsa_switch *, unsigned int);
    int (*devlink_sb_occ_max_clear)(struct dsa_switch *, unsigned int);
    int (*devlink_sb_occ_port_pool_get)(struct dsa_switch *, int, unsigned int, u16, u32 *, u32 *);
    int (*devlink_sb_occ_tc_port_bind_get)(struct dsa_switch *, int, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*port_change_mtu)(struct dsa_switch *, int, int);
    int (*port_max_mtu)(struct dsa_switch *, int);
    int (*port_lag_change)(struct dsa_switch *, int);
    int (*port_lag_join)(struct dsa_switch *, int, struct dsa_lag, struct netdev_lag_upper_info *, struct netlink_ext_ack *);
    int (*port_lag_leave)(struct dsa_switch *, int, struct dsa_lag);
    int (*port_hsr_join)(struct dsa_switch *, int, struct net_device *, struct netlink_ext_ack *);
    int (*port_hsr_leave)(struct dsa_switch *, int, struct net_device *);
    int (*port_mrp_add)(struct dsa_switch *, int, const struct switchdev_obj_mrp *);
    int (*port_mrp_del)(struct dsa_switch *, int, const struct switchdev_obj_mrp *);
    int (*port_mrp_add_ring_role)(struct dsa_switch *, int, const struct switchdev_obj_ring_role_mrp *);
    int (*port_mrp_del_ring_role)(struct dsa_switch *, int, const struct switchdev_obj_ring_role_mrp *);
    int (*tag_8021q_vlan_add)(struct dsa_switch *, int, u16, u16);
    int (*tag_8021q_vlan_del)(struct dsa_switch *, int, u16);
    void (*conduit_state_change)(struct dsa_switch *, const struct net_device *, bool);
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
struct dsa_switch_ops {
    enum dsa_tag_protocol (*get_tag_protocol)(struct dsa_switch *, int);
    int (*setup)(struct dsa_switch *);
    void (*teardown)(struct dsa_switch *);
    u32 (*get_phy_flags)(struct dsa_switch *, int);
    int (*phy_read)(struct dsa_switch *, int, int);
    int (*phy_write)(struct dsa_switch *, int, int, u16);
    void (*adjust_link)(struct dsa_switch *, int, struct phy_device *);
    void (*fixed_link_update)(struct dsa_switch *, int, struct fixed_phy_status *);
    void (*phylink_validate)(struct dsa_switch *, int, long unsigned int *, struct phylink_link_state *);
    int (*phylink_mac_link_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*phylink_mac_config)(struct dsa_switch *, int, unsigned int, const struct phylink_link_state *);
    void (*phylink_mac_an_restart)(struct dsa_switch *, int);
    void (*phylink_mac_link_down)(struct dsa_switch *, int, unsigned int, phy_interface_t);
    void (*phylink_mac_link_up)(struct dsa_switch *, int, unsigned int, phy_interface_t, struct phy_device *);
    void (*phylink_fixed_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*get_strings)(struct dsa_switch *, int, u32, uint8_t *);
    void (*get_ethtool_stats)(struct dsa_switch *, int, uint64_t *);
    int (*get_sset_count)(struct dsa_switch *, int, int);
    void (*get_ethtool_phy_stats)(struct dsa_switch *, int, uint64_t *);
    void (*get_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*set_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*get_ts_info)(struct dsa_switch *, int, struct ethtool_ts_info *);
    int (*suspend)(struct dsa_switch *);
    int (*resume)(struct dsa_switch *);
    int (*port_enable)(struct dsa_switch *, int, struct phy_device *);
    void (*port_disable)(struct dsa_switch *, int);
    int (*set_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_eeprom_len)(struct dsa_switch *);
    int (*get_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*get_regs_len)(struct dsa_switch *, int);
    void (*get_regs)(struct dsa_switch *, int, struct ethtool_regs *, void *);
    int (*set_ageing_time)(struct dsa_switch *, unsigned int);
    int (*port_bridge_join)(struct dsa_switch *, int, struct net_device *);
    void (*port_bridge_leave)(struct dsa_switch *, int, struct net_device *);
    void (*port_stp_state_set)(struct dsa_switch *, int, u8);
    void (*port_fast_age)(struct dsa_switch *, int);
    int (*port_egress_floods)(struct dsa_switch *, int, bool, bool);
    int (*port_vlan_filtering)(struct dsa_switch *, int, bool);
    int (*port_vlan_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    void (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_vlan_del)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_fdb_add)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_del)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_dump)(struct dsa_switch *, int, dsa_fdb_dump_cb_t *, void *);
    int (*port_mdb_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    void (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*port_mdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*get_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *);
    int (*port_mirror_add)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *, bool);
    void (*port_mirror_del)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *);
    int (*port_setup_tc)(struct dsa_switch *, int, enum tc_setup_type, void *);
    int (*crosschip_bridge_join)(struct dsa_switch *, int, int, struct net_device *);
    void (*crosschip_bridge_leave)(struct dsa_switch *, int, int, struct net_device *);
    int (*port_hwtstamp_get)(struct dsa_switch *, int, struct ifreq *);
    int (*port_hwtstamp_set)(struct dsa_switch *, int, struct ifreq *);
    bool (*port_txtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    bool (*port_rxtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    netdev_tx_t (*port_deferred_xmit)(struct dsa_switch *, int, struct sk_buff *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dsa_switch_ops {
    enum dsa_tag_protocol (*get_tag_protocol)(struct dsa_switch *, int);
    int (*setup)(struct dsa_switch *);
    void (*teardown)(struct dsa_switch *);
    u32 (*get_phy_flags)(struct dsa_switch *, int);
    int (*phy_read)(struct dsa_switch *, int, int);
    int (*phy_write)(struct dsa_switch *, int, int, u16);
    void (*adjust_link)(struct dsa_switch *, int, struct phy_device *);
    void (*fixed_link_update)(struct dsa_switch *, int, struct fixed_phy_status *);
    void (*phylink_validate)(struct dsa_switch *, int, long unsigned int *, struct phylink_link_state *);
    int (*phylink_mac_link_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*phylink_mac_config)(struct dsa_switch *, int, unsigned int, const struct phylink_link_state *);
    void (*phylink_mac_an_restart)(struct dsa_switch *, int);
    void (*phylink_mac_link_down)(struct dsa_switch *, int, unsigned int, phy_interface_t);
    void (*phylink_mac_link_up)(struct dsa_switch *, int, unsigned int, phy_interface_t, struct phy_device *);
    void (*phylink_fixed_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*get_strings)(struct dsa_switch *, int, u32, uint8_t *);
    void (*get_ethtool_stats)(struct dsa_switch *, int, uint64_t *);
    int (*get_sset_count)(struct dsa_switch *, int, int);
    void (*get_ethtool_phy_stats)(struct dsa_switch *, int, uint64_t *);
    void (*get_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*set_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*get_ts_info)(struct dsa_switch *, int, struct ethtool_ts_info *);
    int (*suspend)(struct dsa_switch *);
    int (*resume)(struct dsa_switch *);
    int (*port_enable)(struct dsa_switch *, int, struct phy_device *);
    void (*port_disable)(struct dsa_switch *, int);
    int (*set_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_eeprom_len)(struct dsa_switch *);
    int (*get_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*get_regs_len)(struct dsa_switch *, int);
    void (*get_regs)(struct dsa_switch *, int, struct ethtool_regs *, void *);
    int (*set_ageing_time)(struct dsa_switch *, unsigned int);
    int (*port_bridge_join)(struct dsa_switch *, int, struct net_device *);
    void (*port_bridge_leave)(struct dsa_switch *, int, struct net_device *);
    void (*port_stp_state_set)(struct dsa_switch *, int, u8);
    void (*port_fast_age)(struct dsa_switch *, int);
    int (*port_egress_floods)(struct dsa_switch *, int, bool, bool);
    int (*port_vlan_filtering)(struct dsa_switch *, int, bool);
    int (*port_vlan_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    void (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_vlan_del)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_fdb_add)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_del)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_dump)(struct dsa_switch *, int, dsa_fdb_dump_cb_t *, void *);
    int (*port_mdb_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    void (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*port_mdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*get_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *);
    int (*port_mirror_add)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *, bool);
    void (*port_mirror_del)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *);
    int (*port_setup_tc)(struct dsa_switch *, int, enum tc_setup_type, void *);
    int (*crosschip_bridge_join)(struct dsa_switch *, int, int, struct net_device *);
    void (*crosschip_bridge_leave)(struct dsa_switch *, int, int, struct net_device *);
    int (*port_hwtstamp_get)(struct dsa_switch *, int, struct ifreq *);
    int (*port_hwtstamp_set)(struct dsa_switch *, int, struct ifreq *);
    bool (*port_txtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    bool (*port_rxtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    netdev_tx_t (*port_deferred_xmit)(struct dsa_switch *, int, struct sk_buff *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dsa_switch_ops {
    enum dsa_tag_protocol (*get_tag_protocol)(struct dsa_switch *, int);
    int (*setup)(struct dsa_switch *);
    void (*teardown)(struct dsa_switch *);
    u32 (*get_phy_flags)(struct dsa_switch *, int);
    int (*phy_read)(struct dsa_switch *, int, int);
    int (*phy_write)(struct dsa_switch *, int, int, u16);
    void (*adjust_link)(struct dsa_switch *, int, struct phy_device *);
    void (*fixed_link_update)(struct dsa_switch *, int, struct fixed_phy_status *);
    void (*phylink_validate)(struct dsa_switch *, int, long unsigned int *, struct phylink_link_state *);
    int (*phylink_mac_link_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*phylink_mac_config)(struct dsa_switch *, int, unsigned int, const struct phylink_link_state *);
    void (*phylink_mac_an_restart)(struct dsa_switch *, int);
    void (*phylink_mac_link_down)(struct dsa_switch *, int, unsigned int, phy_interface_t);
    void (*phylink_mac_link_up)(struct dsa_switch *, int, unsigned int, phy_interface_t, struct phy_device *);
    void (*phylink_fixed_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*get_strings)(struct dsa_switch *, int, u32, uint8_t *);
    void (*get_ethtool_stats)(struct dsa_switch *, int, uint64_t *);
    int (*get_sset_count)(struct dsa_switch *, int, int);
    void (*get_ethtool_phy_stats)(struct dsa_switch *, int, uint64_t *);
    void (*get_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*set_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*get_ts_info)(struct dsa_switch *, int, struct ethtool_ts_info *);
    int (*suspend)(struct dsa_switch *);
    int (*resume)(struct dsa_switch *);
    int (*port_enable)(struct dsa_switch *, int, struct phy_device *);
    void (*port_disable)(struct dsa_switch *, int);
    int (*set_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_eeprom_len)(struct dsa_switch *);
    int (*get_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*get_regs_len)(struct dsa_switch *, int);
    void (*get_regs)(struct dsa_switch *, int, struct ethtool_regs *, void *);
    int (*set_ageing_time)(struct dsa_switch *, unsigned int);
    int (*port_bridge_join)(struct dsa_switch *, int, struct net_device *);
    void (*port_bridge_leave)(struct dsa_switch *, int, struct net_device *);
    void (*port_stp_state_set)(struct dsa_switch *, int, u8);
    void (*port_fast_age)(struct dsa_switch *, int);
    int (*port_egress_floods)(struct dsa_switch *, int, bool, bool);
    int (*port_vlan_filtering)(struct dsa_switch *, int, bool);
    int (*port_vlan_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    void (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_vlan_del)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_fdb_add)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_del)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_dump)(struct dsa_switch *, int, dsa_fdb_dump_cb_t *, void *);
    int (*port_mdb_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    void (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*port_mdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*get_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *);
    int (*port_mirror_add)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *, bool);
    void (*port_mirror_del)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *);
    int (*port_setup_tc)(struct dsa_switch *, int, enum tc_setup_type, void *);
    int (*crosschip_bridge_join)(struct dsa_switch *, int, int, struct net_device *);
    void (*crosschip_bridge_leave)(struct dsa_switch *, int, int, struct net_device *);
    int (*port_hwtstamp_get)(struct dsa_switch *, int, struct ifreq *);
    int (*port_hwtstamp_set)(struct dsa_switch *, int, struct ifreq *);
    bool (*port_txtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    bool (*port_rxtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    netdev_tx_t (*port_deferred_xmit)(struct dsa_switch *, int, struct sk_buff *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dsa_switch_ops {
    enum dsa_tag_protocol (*get_tag_protocol)(struct dsa_switch *, int);
    int (*setup)(struct dsa_switch *);
    void (*teardown)(struct dsa_switch *);
    u32 (*get_phy_flags)(struct dsa_switch *, int);
    int (*phy_read)(struct dsa_switch *, int, int);
    int (*phy_write)(struct dsa_switch *, int, int, u16);
    void (*adjust_link)(struct dsa_switch *, int, struct phy_device *);
    void (*fixed_link_update)(struct dsa_switch *, int, struct fixed_phy_status *);
    void (*phylink_validate)(struct dsa_switch *, int, long unsigned int *, struct phylink_link_state *);
    int (*phylink_mac_link_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*phylink_mac_config)(struct dsa_switch *, int, unsigned int, const struct phylink_link_state *);
    void (*phylink_mac_an_restart)(struct dsa_switch *, int);
    void (*phylink_mac_link_down)(struct dsa_switch *, int, unsigned int, phy_interface_t);
    void (*phylink_mac_link_up)(struct dsa_switch *, int, unsigned int, phy_interface_t, struct phy_device *);
    void (*phylink_fixed_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*get_strings)(struct dsa_switch *, int, u32, uint8_t *);
    void (*get_ethtool_stats)(struct dsa_switch *, int, uint64_t *);
    int (*get_sset_count)(struct dsa_switch *, int, int);
    void (*get_ethtool_phy_stats)(struct dsa_switch *, int, uint64_t *);
    void (*get_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*set_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*get_ts_info)(struct dsa_switch *, int, struct ethtool_ts_info *);
    int (*suspend)(struct dsa_switch *);
    int (*resume)(struct dsa_switch *);
    int (*port_enable)(struct dsa_switch *, int, struct phy_device *);
    void (*port_disable)(struct dsa_switch *, int);
    int (*set_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_eeprom_len)(struct dsa_switch *);
    int (*get_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*get_regs_len)(struct dsa_switch *, int);
    void (*get_regs)(struct dsa_switch *, int, struct ethtool_regs *, void *);
    int (*set_ageing_time)(struct dsa_switch *, unsigned int);
    int (*port_bridge_join)(struct dsa_switch *, int, struct net_device *);
    void (*port_bridge_leave)(struct dsa_switch *, int, struct net_device *);
    void (*port_stp_state_set)(struct dsa_switch *, int, u8);
    void (*port_fast_age)(struct dsa_switch *, int);
    int (*port_egress_floods)(struct dsa_switch *, int, bool, bool);
    int (*port_vlan_filtering)(struct dsa_switch *, int, bool);
    int (*port_vlan_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    void (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_vlan_del)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_fdb_add)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_del)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_dump)(struct dsa_switch *, int, dsa_fdb_dump_cb_t *, void *);
    int (*port_mdb_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    void (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*port_mdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*get_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *);
    int (*port_mirror_add)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *, bool);
    void (*port_mirror_del)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *);
    int (*port_setup_tc)(struct dsa_switch *, int, enum tc_setup_type, void *);
    int (*crosschip_bridge_join)(struct dsa_switch *, int, int, struct net_device *);
    void (*crosschip_bridge_leave)(struct dsa_switch *, int, int, struct net_device *);
    int (*port_hwtstamp_get)(struct dsa_switch *, int, struct ifreq *);
    int (*port_hwtstamp_set)(struct dsa_switch *, int, struct ifreq *);
    bool (*port_txtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    bool (*port_rxtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    netdev_tx_t (*port_deferred_xmit)(struct dsa_switch *, int, struct sk_buff *);
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
struct dsa_switch_ops {
    enum dsa_tag_protocol (*get_tag_protocol)(struct dsa_switch *, int);
    int (*setup)(struct dsa_switch *);
    void (*teardown)(struct dsa_switch *);
    u32 (*get_phy_flags)(struct dsa_switch *, int);
    int (*phy_read)(struct dsa_switch *, int, int);
    int (*phy_write)(struct dsa_switch *, int, int, u16);
    void (*adjust_link)(struct dsa_switch *, int, struct phy_device *);
    void (*fixed_link_update)(struct dsa_switch *, int, struct fixed_phy_status *);
    void (*phylink_validate)(struct dsa_switch *, int, long unsigned int *, struct phylink_link_state *);
    int (*phylink_mac_link_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*phylink_mac_config)(struct dsa_switch *, int, unsigned int, const struct phylink_link_state *);
    void (*phylink_mac_an_restart)(struct dsa_switch *, int);
    void (*phylink_mac_link_down)(struct dsa_switch *, int, unsigned int, phy_interface_t);
    void (*phylink_mac_link_up)(struct dsa_switch *, int, unsigned int, phy_interface_t, struct phy_device *);
    void (*phylink_fixed_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*get_strings)(struct dsa_switch *, int, u32, uint8_t *);
    void (*get_ethtool_stats)(struct dsa_switch *, int, uint64_t *);
    int (*get_sset_count)(struct dsa_switch *, int, int);
    void (*get_ethtool_phy_stats)(struct dsa_switch *, int, uint64_t *);
    void (*get_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*set_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*get_ts_info)(struct dsa_switch *, int, struct ethtool_ts_info *);
    int (*suspend)(struct dsa_switch *);
    int (*resume)(struct dsa_switch *);
    int (*port_enable)(struct dsa_switch *, int, struct phy_device *);
    void (*port_disable)(struct dsa_switch *, int);
    int (*set_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_eeprom_len)(struct dsa_switch *);
    int (*get_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*get_regs_len)(struct dsa_switch *, int);
    void (*get_regs)(struct dsa_switch *, int, struct ethtool_regs *, void *);
    int (*set_ageing_time)(struct dsa_switch *, unsigned int);
    int (*port_bridge_join)(struct dsa_switch *, int, struct net_device *);
    void (*port_bridge_leave)(struct dsa_switch *, int, struct net_device *);
    void (*port_stp_state_set)(struct dsa_switch *, int, u8);
    void (*port_fast_age)(struct dsa_switch *, int);
    int (*port_egress_floods)(struct dsa_switch *, int, bool, bool);
    int (*port_vlan_filtering)(struct dsa_switch *, int, bool);
    int (*port_vlan_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    void (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_vlan_del)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_fdb_add)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_del)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_dump)(struct dsa_switch *, int, dsa_fdb_dump_cb_t *, void *);
    int (*port_mdb_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    void (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*port_mdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*get_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *);
    int (*port_mirror_add)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *, bool);
    void (*port_mirror_del)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *);
    int (*port_setup_tc)(struct dsa_switch *, int, enum tc_setup_type, void *);
    int (*crosschip_bridge_join)(struct dsa_switch *, int, int, struct net_device *);
    void (*crosschip_bridge_leave)(struct dsa_switch *, int, int, struct net_device *);
    int (*port_hwtstamp_get)(struct dsa_switch *, int, struct ifreq *);
    int (*port_hwtstamp_set)(struct dsa_switch *, int, struct ifreq *);
    bool (*port_txtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    bool (*port_rxtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    netdev_tx_t (*port_deferred_xmit)(struct dsa_switch *, int, struct sk_buff *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dsa_switch_ops {
    enum dsa_tag_protocol (*get_tag_protocol)(struct dsa_switch *, int);
    int (*setup)(struct dsa_switch *);
    void (*teardown)(struct dsa_switch *);
    u32 (*get_phy_flags)(struct dsa_switch *, int);
    int (*phy_read)(struct dsa_switch *, int, int);
    int (*phy_write)(struct dsa_switch *, int, int, u16);
    void (*adjust_link)(struct dsa_switch *, int, struct phy_device *);
    void (*fixed_link_update)(struct dsa_switch *, int, struct fixed_phy_status *);
    void (*phylink_validate)(struct dsa_switch *, int, long unsigned int *, struct phylink_link_state *);
    int (*phylink_mac_link_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*phylink_mac_config)(struct dsa_switch *, int, unsigned int, const struct phylink_link_state *);
    void (*phylink_mac_an_restart)(struct dsa_switch *, int);
    void (*phylink_mac_link_down)(struct dsa_switch *, int, unsigned int, phy_interface_t);
    void (*phylink_mac_link_up)(struct dsa_switch *, int, unsigned int, phy_interface_t, struct phy_device *);
    void (*phylink_fixed_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*get_strings)(struct dsa_switch *, int, u32, uint8_t *);
    void (*get_ethtool_stats)(struct dsa_switch *, int, uint64_t *);
    int (*get_sset_count)(struct dsa_switch *, int, int);
    void (*get_ethtool_phy_stats)(struct dsa_switch *, int, uint64_t *);
    void (*get_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*set_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*get_ts_info)(struct dsa_switch *, int, struct ethtool_ts_info *);
    int (*suspend)(struct dsa_switch *);
    int (*resume)(struct dsa_switch *);
    int (*port_enable)(struct dsa_switch *, int, struct phy_device *);
    void (*port_disable)(struct dsa_switch *, int);
    int (*set_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_eeprom_len)(struct dsa_switch *);
    int (*get_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*get_regs_len)(struct dsa_switch *, int);
    void (*get_regs)(struct dsa_switch *, int, struct ethtool_regs *, void *);
    int (*set_ageing_time)(struct dsa_switch *, unsigned int);
    int (*port_bridge_join)(struct dsa_switch *, int, struct net_device *);
    void (*port_bridge_leave)(struct dsa_switch *, int, struct net_device *);
    void (*port_stp_state_set)(struct dsa_switch *, int, u8);
    void (*port_fast_age)(struct dsa_switch *, int);
    int (*port_egress_floods)(struct dsa_switch *, int, bool, bool);
    int (*port_vlan_filtering)(struct dsa_switch *, int, bool);
    int (*port_vlan_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    void (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_vlan_del)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_fdb_add)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_del)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_dump)(struct dsa_switch *, int, dsa_fdb_dump_cb_t *, void *);
    int (*port_mdb_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    void (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*port_mdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*get_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *);
    int (*port_mirror_add)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *, bool);
    void (*port_mirror_del)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *);
    int (*port_setup_tc)(struct dsa_switch *, int, enum tc_setup_type, void *);
    int (*crosschip_bridge_join)(struct dsa_switch *, int, int, struct net_device *);
    void (*crosschip_bridge_leave)(struct dsa_switch *, int, int, struct net_device *);
    int (*port_hwtstamp_get)(struct dsa_switch *, int, struct ifreq *);
    int (*port_hwtstamp_set)(struct dsa_switch *, int, struct ifreq *);
    bool (*port_txtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    bool (*port_rxtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    netdev_tx_t (*port_deferred_xmit)(struct dsa_switch *, int, struct sk_buff *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dsa_switch_ops {
    enum dsa_tag_protocol (*get_tag_protocol)(struct dsa_switch *, int);
    int (*setup)(struct dsa_switch *);
    void (*teardown)(struct dsa_switch *);
    u32 (*get_phy_flags)(struct dsa_switch *, int);
    int (*phy_read)(struct dsa_switch *, int, int);
    int (*phy_write)(struct dsa_switch *, int, int, u16);
    void (*adjust_link)(struct dsa_switch *, int, struct phy_device *);
    void (*fixed_link_update)(struct dsa_switch *, int, struct fixed_phy_status *);
    void (*phylink_validate)(struct dsa_switch *, int, long unsigned int *, struct phylink_link_state *);
    int (*phylink_mac_link_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*phylink_mac_config)(struct dsa_switch *, int, unsigned int, const struct phylink_link_state *);
    void (*phylink_mac_an_restart)(struct dsa_switch *, int);
    void (*phylink_mac_link_down)(struct dsa_switch *, int, unsigned int, phy_interface_t);
    void (*phylink_mac_link_up)(struct dsa_switch *, int, unsigned int, phy_interface_t, struct phy_device *);
    void (*phylink_fixed_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*get_strings)(struct dsa_switch *, int, u32, uint8_t *);
    void (*get_ethtool_stats)(struct dsa_switch *, int, uint64_t *);
    int (*get_sset_count)(struct dsa_switch *, int, int);
    void (*get_ethtool_phy_stats)(struct dsa_switch *, int, uint64_t *);
    void (*get_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*set_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*get_ts_info)(struct dsa_switch *, int, struct ethtool_ts_info *);
    int (*suspend)(struct dsa_switch *);
    int (*resume)(struct dsa_switch *);
    int (*port_enable)(struct dsa_switch *, int, struct phy_device *);
    void (*port_disable)(struct dsa_switch *, int);
    int (*set_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_eeprom_len)(struct dsa_switch *);
    int (*get_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*get_regs_len)(struct dsa_switch *, int);
    void (*get_regs)(struct dsa_switch *, int, struct ethtool_regs *, void *);
    int (*set_ageing_time)(struct dsa_switch *, unsigned int);
    int (*port_bridge_join)(struct dsa_switch *, int, struct net_device *);
    void (*port_bridge_leave)(struct dsa_switch *, int, struct net_device *);
    void (*port_stp_state_set)(struct dsa_switch *, int, u8);
    void (*port_fast_age)(struct dsa_switch *, int);
    int (*port_egress_floods)(struct dsa_switch *, int, bool, bool);
    int (*port_vlan_filtering)(struct dsa_switch *, int, bool);
    int (*port_vlan_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    void (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_vlan_del)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_fdb_add)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_del)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_dump)(struct dsa_switch *, int, dsa_fdb_dump_cb_t *, void *);
    int (*port_mdb_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    void (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*port_mdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*get_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *);
    int (*port_mirror_add)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *, bool);
    void (*port_mirror_del)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *);
    int (*port_setup_tc)(struct dsa_switch *, int, enum tc_setup_type, void *);
    int (*crosschip_bridge_join)(struct dsa_switch *, int, int, struct net_device *);
    void (*crosschip_bridge_leave)(struct dsa_switch *, int, int, struct net_device *);
    int (*port_hwtstamp_get)(struct dsa_switch *, int, struct ifreq *);
    int (*port_hwtstamp_set)(struct dsa_switch *, int, struct ifreq *);
    bool (*port_txtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    bool (*port_rxtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    netdev_tx_t (*port_deferred_xmit)(struct dsa_switch *, int, struct sk_buff *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dsa_switch_ops {
    enum dsa_tag_protocol (*get_tag_protocol)(struct dsa_switch *, int);
    int (*setup)(struct dsa_switch *);
    void (*teardown)(struct dsa_switch *);
    u32 (*get_phy_flags)(struct dsa_switch *, int);
    int (*phy_read)(struct dsa_switch *, int, int);
    int (*phy_write)(struct dsa_switch *, int, int, u16);
    void (*adjust_link)(struct dsa_switch *, int, struct phy_device *);
    void (*fixed_link_update)(struct dsa_switch *, int, struct fixed_phy_status *);
    void (*phylink_validate)(struct dsa_switch *, int, long unsigned int *, struct phylink_link_state *);
    int (*phylink_mac_link_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*phylink_mac_config)(struct dsa_switch *, int, unsigned int, const struct phylink_link_state *);
    void (*phylink_mac_an_restart)(struct dsa_switch *, int);
    void (*phylink_mac_link_down)(struct dsa_switch *, int, unsigned int, phy_interface_t);
    void (*phylink_mac_link_up)(struct dsa_switch *, int, unsigned int, phy_interface_t, struct phy_device *);
    void (*phylink_fixed_state)(struct dsa_switch *, int, struct phylink_link_state *);
    void (*get_strings)(struct dsa_switch *, int, u32, uint8_t *);
    void (*get_ethtool_stats)(struct dsa_switch *, int, uint64_t *);
    int (*get_sset_count)(struct dsa_switch *, int, int);
    void (*get_ethtool_phy_stats)(struct dsa_switch *, int, uint64_t *);
    void (*get_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*set_wol)(struct dsa_switch *, int, struct ethtool_wolinfo *);
    int (*get_ts_info)(struct dsa_switch *, int, struct ethtool_ts_info *);
    int (*suspend)(struct dsa_switch *);
    int (*resume)(struct dsa_switch *);
    int (*port_enable)(struct dsa_switch *, int, struct phy_device *);
    void (*port_disable)(struct dsa_switch *, int);
    int (*set_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *);
    int (*get_eeprom_len)(struct dsa_switch *);
    int (*get_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct dsa_switch *, struct ethtool_eeprom *, u8 *);
    int (*get_regs_len)(struct dsa_switch *, int);
    void (*get_regs)(struct dsa_switch *, int, struct ethtool_regs *, void *);
    int (*set_ageing_time)(struct dsa_switch *, unsigned int);
    int (*port_bridge_join)(struct dsa_switch *, int, struct net_device *);
    void (*port_bridge_leave)(struct dsa_switch *, int, struct net_device *);
    void (*port_stp_state_set)(struct dsa_switch *, int, u8);
    void (*port_fast_age)(struct dsa_switch *, int);
    int (*port_egress_floods)(struct dsa_switch *, int, bool, bool);
    int (*port_vlan_filtering)(struct dsa_switch *, int, bool);
    int (*port_vlan_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    void (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_vlan_del)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *);
    int (*port_fdb_add)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_del)(struct dsa_switch *, int, const unsigned char *, u16);
    int (*port_fdb_dump)(struct dsa_switch *, int, dsa_fdb_dump_cb_t *, void *);
    int (*port_mdb_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    void (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*port_mdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *);
    int (*get_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *);
    int (*port_mirror_add)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *, bool);
    void (*port_mirror_del)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *);
    int (*port_setup_tc)(struct dsa_switch *, int, enum tc_setup_type, void *);
    int (*crosschip_bridge_join)(struct dsa_switch *, int, int, struct net_device *);
    void (*crosschip_bridge_leave)(struct dsa_switch *, int, int, struct net_device *);
    int (*port_hwtstamp_get)(struct dsa_switch *, int, struct ifreq *);
    int (*port_hwtstamp_set)(struct dsa_switch *, int, struct ifreq *);
    bool (*port_txtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    bool (*port_rxtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int);
    netdev_tx_t (*port_deferred_xmit)(struct dsa_switch *, int, struct sk_buff *);
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
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*get_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *, u32 *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_rxnfc)(struct dsa_switch *, int, struct ethtool_rxnfc *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_mirror_add)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *, bool)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*port_mirror_del)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*crosschip_bridge_join)(struct dsa_switch *, int, int, struct net_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*crosschip_bridge_leave)(struct dsa_switch *, int, int, struct net_device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head list</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*get_temp)(struct dsa_switch *, int *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*get_temp_limit)(struct dsa_switch *, int *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*set_temp_limit)(struct dsa_switch *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*get_temp_alarm)(struct dsa_switch *, bool *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*port_bridge_leave)(struct dsa_switch *, int)</code> ➡️ <code>void (*port_bridge_leave)(struct dsa_switch *, int, struct net_device *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*port_vlan_dump)(struct dsa_switch *, int, struct switchdev_obj_port_vlan *, int(*)(struct switchdev_obj *))</code> ➡️ <code>int (*port_vlan_dump)(struct dsa_switch *, int, struct switchdev_obj_port_vlan *, switchdev_obj_dump_cb_t *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*port_fdb_dump)(struct dsa_switch *, int, struct switchdev_obj_port_fdb *, int(*)(struct switchdev_obj *))</code> ➡️ <code>int (*port_fdb_dump)(struct dsa_switch *, int, struct switchdev_obj_port_fdb *, switchdev_obj_dump_cb_t *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*port_mdb_dump)(struct dsa_switch *, int, struct switchdev_obj_port_mdb *, int(*)(struct switchdev_obj *))</code> ➡️ <code>int (*port_mdb_dump)(struct dsa_switch *, int, struct switchdev_obj_port_mdb *, switchdev_obj_dump_cb_t *)</code>
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
<code>int (*set_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*get_mac_eee)(struct dsa_switch *, int, struct ethtool_eee *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*set_addr)(struct dsa_switch *, u8 *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*set_eee)(struct dsa_switch *, int, struct phy_device *, struct ethtool_eee *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*get_eee)(struct dsa_switch *, int, struct ethtool_eee *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*port_vlan_dump)(struct dsa_switch *, int, struct switchdev_obj_port_vlan *, switchdev_obj_dump_cb_t *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*port_fdb_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_fdb *, struct switchdev_trans *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*port_mdb_dump)(struct dsa_switch *, int, struct switchdev_obj_port_mdb *, switchdev_obj_dump_cb_t *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>enum dsa_tag_protocol (*get_tag_protocol)(struct dsa_switch *)</code> ➡️ <code>enum dsa_tag_protocol (*get_tag_protocol)(struct dsa_switch *, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*port_fdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_fdb *, struct switchdev_trans *)</code> ➡️ <code>int (*port_fdb_add)(struct dsa_switch *, int, const unsigned char *, u16)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*port_fdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_fdb *)</code> ➡️ <code>int (*port_fdb_del)(struct dsa_switch *, int, const unsigned char *, u16)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*port_fdb_dump)(struct dsa_switch *, int, struct switchdev_obj_port_fdb *, switchdev_obj_dump_cb_t *)</code> ➡️ <code>int (*port_fdb_dump)(struct dsa_switch *, int, dsa_fdb_dump_cb_t *, void *)</code>
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
<code>void (*phylink_validate)(struct dsa_switch *, int, long unsigned int *, struct phylink_link_state *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*phylink_mac_link_state)(struct dsa_switch *, int, struct phylink_link_state *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*phylink_mac_config)(struct dsa_switch *, int, unsigned int, const struct phylink_link_state *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*phylink_mac_an_restart)(struct dsa_switch *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*phylink_mac_link_down)(struct dsa_switch *, int, unsigned int, phy_interface_t)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*phylink_mac_link_up)(struct dsa_switch *, int, unsigned int, phy_interface_t, struct phy_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*phylink_fixed_state)(struct dsa_switch *, int, struct phylink_link_state *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*get_ethtool_phy_stats)(struct dsa_switch *, int, uint64_t *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*get_ts_info)(struct dsa_switch *, int, struct ethtool_ts_info *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_hwtstamp_get)(struct dsa_switch *, int, struct ifreq *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_hwtstamp_set)(struct dsa_switch *, int, struct ifreq *)</code>
</li>
<li>
<b>Field added. </b>
<code>bool (*port_txtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>bool (*port_rxtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*get_strings)(struct dsa_switch *, int, uint8_t *)</code> ➡️ <code>void (*get_strings)(struct dsa_switch *, int, u32, uint8_t *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*get_sset_count)(struct dsa_switch *)</code> ➡️ <code>int (*get_sset_count)(struct dsa_switch *, int, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*port_vlan_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *, struct switchdev_trans *)</code> ➡️ <code>int (*port_vlan_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *, struct switchdev_trans *)</code> ➡️ <code>void (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*port_mdb_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *, struct switchdev_trans *)</code> ➡️ <code>int (*port_mdb_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *, struct switchdev_trans *)</code> ➡️ <code>void (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *)</code>
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
<code>void (*teardown)(struct dsa_switch *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_egress_floods)(struct dsa_switch *, int, bool, bool)</code>
</li>
<li>
<b>Field added. </b>
<code>netdev_tx_t (*port_deferred_xmit)(struct dsa_switch *, int, struct sk_buff *)</code>
</li>
<li>
<b>Field removed. </b>
<code>const char * (*probe)(struct device *, struct device *, int, void **)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*phylink_validate)(struct dsa_switch *, int, long unsigned int *, struct phylink_link_state *)</code> ➡️ <code>void (*phylink_validate)(struct dsa_switch *, int, long unsigned int *, struct phylink_link_state *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*phylink_mac_link_state)(struct dsa_switch *, int, struct phylink_link_state *)</code> ➡️ <code>int (*phylink_mac_link_state)(struct dsa_switch *, int, struct phylink_link_state *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*phylink_mac_config)(struct dsa_switch *, int, unsigned int, const struct phylink_link_state *)</code> ➡️ <code>void (*phylink_mac_config)(struct dsa_switch *, int, unsigned int, const struct phylink_link_state *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*phylink_fixed_state)(struct dsa_switch *, int, struct phylink_link_state *)</code> ➡️ <code>void (*phylink_fixed_state)(struct dsa_switch *, int, struct phylink_link_state *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*port_disable)(struct dsa_switch *, int, struct phy_device *)</code> ➡️ <code>void (*port_disable)(struct dsa_switch *, int)</code>
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
<code>int (*port_setup_tc)(struct dsa_switch *, int, enum tc_setup_type, void *)</code>
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
<code>int (*cls_flower_add)(struct dsa_switch *, int, struct flow_cls_offload *, bool)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*cls_flower_del)(struct dsa_switch *, int, struct flow_cls_offload *, bool)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*cls_flower_stats)(struct dsa_switch *, int, struct flow_cls_offload *, bool)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_policer_add)(struct dsa_switch *, int, struct dsa_mall_policer_tc_entry *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*port_policer_del)(struct dsa_switch *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*devlink_param_get)(struct dsa_switch *, u32, struct devlink_param_gset_ctx *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*devlink_param_set)(struct dsa_switch *, u32, struct devlink_param_gset_ctx *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_change_mtu)(struct dsa_switch *, int, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_max_mtu)(struct dsa_switch *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>netdev_tx_t (*port_deferred_xmit)(struct dsa_switch *, int, struct sk_buff *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>enum dsa_tag_protocol (*get_tag_protocol)(struct dsa_switch *, int)</code> ➡️ <code>enum dsa_tag_protocol (*get_tag_protocol)(struct dsa_switch *, int, enum dsa_tag_protocol)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*phylink_mac_link_up)(struct dsa_switch *, int, unsigned int, phy_interface_t, struct phy_device *)</code> ➡️ <code>void (*phylink_mac_link_up)(struct dsa_switch *, int, unsigned int, phy_interface_t, struct phy_device *, int, int, bool, bool)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*crosschip_bridge_join)(struct dsa_switch *, int, int, struct net_device *)</code> ➡️ <code>int (*crosschip_bridge_join)(struct dsa_switch *, int, int, int, struct net_device *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*crosschip_bridge_leave)(struct dsa_switch *, int, int, struct net_device *)</code> ➡️ <code>void (*crosschip_bridge_leave)(struct dsa_switch *, int, int, int, struct net_device *)</code>
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
<code>int (*port_prechangeupper)(struct dsa_switch *, int, struct netdev_notifier_changeupper_info *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*devlink_info_get)(struct dsa_switch *, struct devlink_info_req *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*port_vlan_filtering)(struct dsa_switch *, int, bool)</code> ➡️ <code>int (*port_vlan_filtering)(struct dsa_switch *, int, bool, struct switchdev_trans *)</code>
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
<code>int (*change_tag_protocol)(struct dsa_switch *, int, enum dsa_tag_protocol)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*get_stats64)(struct dsa_switch *, int, struct rtnl_link_stats64 *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*self_test)(struct dsa_switch *, int, struct ethtool_test *, u64 *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_pre_bridge_flags)(struct dsa_switch *, int, struct switchdev_brport_flags, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_bridge_flags)(struct dsa_switch *, int, struct switchdev_brport_flags, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_set_mrouter)(struct dsa_switch *, int, bool, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*crosschip_lag_change)(struct dsa_switch *, int, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*crosschip_lag_join)(struct dsa_switch *, int, int, struct net_device *, struct netdev_lag_upper_info *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*crosschip_lag_leave)(struct dsa_switch *, int, int, struct net_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*devlink_sb_pool_get)(struct dsa_switch *, unsigned int, u16, struct devlink_sb_pool_info *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*devlink_sb_pool_set)(struct dsa_switch *, unsigned int, u16, u32, enum devlink_sb_threshold_type, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*devlink_sb_port_pool_get)(struct dsa_switch *, int, unsigned int, u16, u32 *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*devlink_sb_port_pool_set)(struct dsa_switch *, int, unsigned int, u16, u32, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*devlink_sb_tc_pool_bind_get)(struct dsa_switch *, int, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*devlink_sb_tc_pool_bind_set)(struct dsa_switch *, int, unsigned int, u16, enum devlink_sb_pool_type, u16, u32, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*devlink_sb_occ_snapshot)(struct dsa_switch *, unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*devlink_sb_occ_max_clear)(struct dsa_switch *, unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*devlink_sb_occ_port_pool_get)(struct dsa_switch *, int, unsigned int, u16, u32 *, u32 *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*devlink_sb_occ_tc_port_bind_get)(struct dsa_switch *, int, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_lag_change)(struct dsa_switch *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_lag_join)(struct dsa_switch *, int, struct net_device *, struct netdev_lag_upper_info *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_lag_leave)(struct dsa_switch *, int, struct net_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_hsr_join)(struct dsa_switch *, int, struct net_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_hsr_leave)(struct dsa_switch *, int, struct net_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_mrp_add)(struct dsa_switch *, int, const struct switchdev_obj_mrp *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_mrp_del)(struct dsa_switch *, int, const struct switchdev_obj_mrp *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_mrp_add_ring_role)(struct dsa_switch *, int, const struct switchdev_obj_ring_role_mrp *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_mrp_del_ring_role)(struct dsa_switch *, int, const struct switchdev_obj_ring_role_mrp *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*port_egress_floods)(struct dsa_switch *, int, bool, bool)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*port_vlan_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*port_mdb_prepare)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*port_vlan_filtering)(struct dsa_switch *, int, bool, struct switchdev_trans *)</code> ➡️ <code>int (*port_vlan_filtering)(struct dsa_switch *, int, bool, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *)</code> ➡️ <code>int (*port_vlan_add)(struct dsa_switch *, int, const struct switchdev_obj_port_vlan *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *)</code> ➡️ <code>int (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool (*port_txtstamp)(struct dsa_switch *, int, struct sk_buff *, unsigned int)</code> ➡️ <code>void (*port_txtstamp)(struct dsa_switch *, int, struct sk_buff *)</code>
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
<code>int (*port_setup)(struct dsa_switch *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*port_teardown)(struct dsa_switch *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_bridge_tx_fwd_offload)(struct dsa_switch *, int, struct net_device *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*port_bridge_tx_fwd_unoffload)(struct dsa_switch *, int, struct net_device *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*tag_8021q_vlan_add)(struct dsa_switch *, int, u16, u16)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*tag_8021q_vlan_del)(struct dsa_switch *, int, u16)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*port_set_mrouter)(struct dsa_switch *, int, bool, struct netlink_ext_ack *)</code>
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
<code>int (*connect_tag_protocol)(struct dsa_switch *, enum dsa_tag_protocol)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*phylink_get_caps)(struct dsa_switch *, int, struct phylink_config *)</code>
</li>
<li>
<b>Field added. </b>
<code>struct phylink_pcs * (*phylink_mac_select_pcs)(struct dsa_switch *, int, phy_interface_t)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*get_eth_phy_stats)(struct dsa_switch *, int, struct ethtool_eth_phy_stats *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*get_eth_mac_stats)(struct dsa_switch *, int, struct ethtool_eth_mac_stats *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*get_eth_ctrl_stats)(struct dsa_switch *, int, struct ethtool_eth_ctrl_stats *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_get_default_prio)(struct dsa_switch *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_set_default_prio)(struct dsa_switch *, int, u8)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_get_dscp_prio)(struct dsa_switch *, int, u8)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_add_dscp_prio)(struct dsa_switch *, int, u8, u8)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_del_dscp_prio)(struct dsa_switch *, int, u8, u8)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_mst_state_set)(struct dsa_switch *, int, const struct switchdev_mst_state *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_vlan_fast_age)(struct dsa_switch *, int, u16)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*port_set_host_flood)(struct dsa_switch *, int, bool, bool)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*vlan_msti_set)(struct dsa_switch *, struct dsa_bridge, const struct switchdev_vlan_msti *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*lag_fdb_add)(struct dsa_switch *, struct dsa_lag, const unsigned char *, u16, struct dsa_db)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*lag_fdb_del)(struct dsa_switch *, struct dsa_lag, const unsigned char *, u16, struct dsa_db)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*master_state_change)(struct dsa_switch *, const struct net_device *, bool)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*port_bridge_tx_fwd_offload)(struct dsa_switch *, int, struct net_device *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*port_bridge_tx_fwd_unoffload)(struct dsa_switch *, int, struct net_device *, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*change_tag_protocol)(struct dsa_switch *, int, enum dsa_tag_protocol)</code> ➡️ <code>int (*change_tag_protocol)(struct dsa_switch *, enum dsa_tag_protocol)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*port_bridge_join)(struct dsa_switch *, int, struct net_device *)</code> ➡️ <code>int (*port_bridge_join)(struct dsa_switch *, int, struct dsa_bridge, bool *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*port_bridge_leave)(struct dsa_switch *, int, struct net_device *)</code> ➡️ <code>void (*port_bridge_leave)(struct dsa_switch *, int, struct dsa_bridge)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*port_fdb_add)(struct dsa_switch *, int, const unsigned char *, u16)</code> ➡️ <code>int (*port_fdb_add)(struct dsa_switch *, int, const unsigned char *, u16, struct dsa_db)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*port_fdb_del)(struct dsa_switch *, int, const unsigned char *, u16)</code> ➡️ <code>int (*port_fdb_del)(struct dsa_switch *, int, const unsigned char *, u16, struct dsa_db)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *)</code> ➡️ <code>int (*port_mdb_add)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *, struct dsa_db)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*port_mdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *)</code> ➡️ <code>int (*port_mdb_del)(struct dsa_switch *, int, const struct switchdev_obj_port_mdb *, struct dsa_db)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*port_mirror_add)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *, bool)</code> ➡️ <code>int (*port_mirror_add)(struct dsa_switch *, int, struct dsa_mall_mirror_tc_entry *, bool, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*crosschip_bridge_join)(struct dsa_switch *, int, int, int, struct net_device *)</code> ➡️ <code>int (*crosschip_bridge_join)(struct dsa_switch *, int, int, int, struct dsa_bridge, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*crosschip_bridge_leave)(struct dsa_switch *, int, int, int, struct net_device *)</code> ➡️ <code>void (*crosschip_bridge_leave)(struct dsa_switch *, int, int, int, struct dsa_bridge)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*crosschip_lag_join)(struct dsa_switch *, int, int, struct net_device *, struct netdev_lag_upper_info *)</code> ➡️ <code>int (*crosschip_lag_join)(struct dsa_switch *, int, int, struct dsa_lag, struct netdev_lag_upper_info *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*crosschip_lag_leave)(struct dsa_switch *, int, int, struct net_device *)</code> ➡️ <code>int (*crosschip_lag_leave)(struct dsa_switch *, int, int, struct dsa_lag)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*port_lag_join)(struct dsa_switch *, int, struct net_device *, struct netdev_lag_upper_info *)</code> ➡️ <code>int (*port_lag_join)(struct dsa_switch *, int, struct dsa_lag, struct netdev_lag_upper_info *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*port_lag_leave)(struct dsa_switch *, int, struct net_device *)</code> ➡️ <code>int (*port_lag_leave)(struct dsa_switch *, int, struct dsa_lag)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*port_change_master)(struct dsa_switch *, int, struct net_device *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*get_rmon_stats)(struct dsa_switch *, int, struct ethtool_rmon_stats *, const struct ethtool_rmon_hist_range **)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*get_pause_stats)(struct dsa_switch *, int, struct ethtool_pause_stats *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*phylink_validate)(struct dsa_switch *, int, long unsigned int *, struct phylink_link_state *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*crosschip_lag_join)(struct dsa_switch *, int, int, struct dsa_lag, struct netdev_lag_upper_info *)</code> ➡️ <code>int (*crosschip_lag_join)(struct dsa_switch *, int, int, struct dsa_lag, struct netdev_lag_upper_info *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*port_lag_join)(struct dsa_switch *, int, struct dsa_lag, struct netdev_lag_upper_info *)</code> ➡️ <code>int (*port_lag_join)(struct dsa_switch *, int, struct dsa_lag, struct netdev_lag_upper_info *, struct netlink_ext_ack *)</code>
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
<code>int (*phylink_mac_prepare)(struct dsa_switch *, int, unsigned int, phy_interface_t)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*phylink_mac_finish)(struct dsa_switch *, int, unsigned int, phy_interface_t)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*get_mm)(struct dsa_switch *, int, struct ethtool_mm_state *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_mm)(struct dsa_switch *, int, struct ethtool_mm_cfg *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*get_mm_stats)(struct dsa_switch *, int, struct ethtool_mm_stats *)</code>
</li>
<li>
<b>Field added. </b>
<code>struct dsa_port * (*preferred_default_local_cpu_port)(struct dsa_switch *)</code>
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
<code>int (*port_change_conduit)(struct dsa_switch *, int, struct net_device *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_set_mac_address)(struct dsa_switch *, int, const unsigned char *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*conduit_state_change)(struct dsa_switch *, const struct net_device *, bool)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*port_change_master)(struct dsa_switch *, int, struct net_device *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*phylink_mac_link_state)(struct dsa_switch *, int, struct phylink_link_state *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*phylink_mac_an_restart)(struct dsa_switch *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*master_state_change)(struct dsa_switch *, const struct net_device *, bool)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*port_hsr_join)(struct dsa_switch *, int, struct net_device *)</code> ➡️ <code>int (*port_hsr_join)(struct dsa_switch *, int, struct net_device *, struct netlink_ext_ack *)</code>
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
