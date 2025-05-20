# Struct: <code>phy_driver</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct phy_driver {
    u32 phy_id;
    char *name;
    unsigned int phy_id_mask;
    u32 features;
    u32 flags;
    const void *driver_data;
    int (*soft_reset)(struct phy_device *);
    int (*config_init)(struct phy_device *);
    int (*probe)(struct phy_device *);
    int (*suspend)(struct phy_device *);
    int (*resume)(struct phy_device *);
    int (*config_aneg)(struct phy_device *);
    int (*aneg_done)(struct phy_device *);
    int (*read_status)(struct phy_device *);
    int (*ack_interrupt)(struct phy_device *);
    int (*config_intr)(struct phy_device *);
    int (*did_interrupt)(struct phy_device *);
    void (*remove)(struct phy_device *);
    int (*match_phy_device)(struct phy_device *);
    int (*ts_info)(struct phy_device *, struct ethtool_ts_info *);
    int (*hwtstamp)(struct phy_device *, struct ifreq *);
    bool (*rxtstamp)(struct phy_device *, struct sk_buff *, int);
    void (*txtstamp)(struct phy_device *, struct sk_buff *, int);
    int (*set_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*get_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*link_change_notify)(struct phy_device *);
    int (*read_mmd_indirect)(struct phy_device *, int, int, int);
    void (*write_mmd_indirect)(struct phy_device *, int, int, int, u32);
    int (*module_info)(struct phy_device *, struct ethtool_modinfo *);
    int (*module_eeprom)(struct phy_device *, struct ethtool_eeprom *, u8 *);
    struct device_driver driver;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct phy_driver {
    struct mdio_driver_common mdiodrv;
    u32 phy_id;
    char *name;
    unsigned int phy_id_mask;
    u32 features;
    u32 flags;
    const void *driver_data;
    int (*soft_reset)(struct phy_device *);
    int (*config_init)(struct phy_device *);
    int (*probe)(struct phy_device *);
    int (*suspend)(struct phy_device *);
    int (*resume)(struct phy_device *);
    int (*config_aneg)(struct phy_device *);
    int (*aneg_done)(struct phy_device *);
    int (*read_status)(struct phy_device *);
    int (*ack_interrupt)(struct phy_device *);
    int (*config_intr)(struct phy_device *);
    int (*did_interrupt)(struct phy_device *);
    void (*remove)(struct phy_device *);
    int (*match_phy_device)(struct phy_device *);
    int (*ts_info)(struct phy_device *, struct ethtool_ts_info *);
    int (*hwtstamp)(struct phy_device *, struct ifreq *);
    bool (*rxtstamp)(struct phy_device *, struct sk_buff *, int);
    void (*txtstamp)(struct phy_device *, struct sk_buff *, int);
    int (*set_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*get_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*link_change_notify)(struct phy_device *);
    int (*read_mmd_indirect)(struct phy_device *, int, int, int);
    void (*write_mmd_indirect)(struct phy_device *, int, int, int, u32);
    int (*module_info)(struct phy_device *, struct ethtool_modinfo *);
    int (*module_eeprom)(struct phy_device *, struct ethtool_eeprom *, u8 *);
    int (*get_sset_count)(struct phy_device *);
    void (*get_strings)(struct phy_device *, u8 *);
    void (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct phy_driver {
    struct mdio_driver_common mdiodrv;
    u32 phy_id;
    char *name;
    unsigned int phy_id_mask;
    u32 features;
    u32 flags;
    const void *driver_data;
    int (*soft_reset)(struct phy_device *);
    int (*config_init)(struct phy_device *);
    int (*probe)(struct phy_device *);
    int (*suspend)(struct phy_device *);
    int (*resume)(struct phy_device *);
    int (*config_aneg)(struct phy_device *);
    int (*aneg_done)(struct phy_device *);
    int (*read_status)(struct phy_device *);
    int (*ack_interrupt)(struct phy_device *);
    int (*config_intr)(struct phy_device *);
    int (*did_interrupt)(struct phy_device *);
    void (*remove)(struct phy_device *);
    int (*match_phy_device)(struct phy_device *);
    int (*ts_info)(struct phy_device *, struct ethtool_ts_info *);
    int (*hwtstamp)(struct phy_device *, struct ifreq *);
    bool (*rxtstamp)(struct phy_device *, struct sk_buff *, int);
    void (*txtstamp)(struct phy_device *, struct sk_buff *, int);
    int (*set_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*get_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*link_change_notify)(struct phy_device *);
    int (*read_mmd_indirect)(struct phy_device *, int, int, int);
    void (*write_mmd_indirect)(struct phy_device *, int, int, int, u32);
    int (*module_info)(struct phy_device *, struct ethtool_modinfo *);
    int (*module_eeprom)(struct phy_device *, struct ethtool_eeprom *, u8 *);
    int (*get_sset_count)(struct phy_device *);
    void (*get_strings)(struct phy_device *, u8 *);
    void (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*get_tunable)(struct phy_device *, struct ethtool_tunable *, void *);
    int (*set_tunable)(struct phy_device *, struct ethtool_tunable *, const void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct phy_driver {
    struct mdio_driver_common mdiodrv;
    u32 phy_id;
    char *name;
    unsigned int phy_id_mask;
    u32 features;
    u32 flags;
    const void *driver_data;
    int (*soft_reset)(struct phy_device *);
    int (*config_init)(struct phy_device *);
    int (*probe)(struct phy_device *);
    int (*suspend)(struct phy_device *);
    int (*resume)(struct phy_device *);
    int (*config_aneg)(struct phy_device *);
    int (*aneg_done)(struct phy_device *);
    int (*read_status)(struct phy_device *);
    int (*ack_interrupt)(struct phy_device *);
    int (*config_intr)(struct phy_device *);
    int (*did_interrupt)(struct phy_device *);
    void (*remove)(struct phy_device *);
    int (*match_phy_device)(struct phy_device *);
    int (*ts_info)(struct phy_device *, struct ethtool_ts_info *);
    int (*hwtstamp)(struct phy_device *, struct ifreq *);
    bool (*rxtstamp)(struct phy_device *, struct sk_buff *, int);
    void (*txtstamp)(struct phy_device *, struct sk_buff *, int);
    int (*set_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*get_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*link_change_notify)(struct phy_device *);
    int (*read_mmd)(struct phy_device *, int, u16);
    int (*write_mmd)(struct phy_device *, int, u16, u16);
    int (*module_info)(struct phy_device *, struct ethtool_modinfo *);
    int (*module_eeprom)(struct phy_device *, struct ethtool_eeprom *, u8 *);
    int (*get_sset_count)(struct phy_device *);
    void (*get_strings)(struct phy_device *, u8 *);
    void (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*get_tunable)(struct phy_device *, struct ethtool_tunable *, void *);
    int (*set_tunable)(struct phy_device *, struct ethtool_tunable *, const void *);
    int (*set_loopback)(struct phy_device *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct phy_driver {
    struct mdio_driver_common mdiodrv;
    u32 phy_id;
    char *name;
    unsigned int phy_id_mask;
    u32 features;
    u32 flags;
    const void *driver_data;
    int (*soft_reset)(struct phy_device *);
    int (*config_init)(struct phy_device *);
    int (*probe)(struct phy_device *);
    int (*suspend)(struct phy_device *);
    int (*resume)(struct phy_device *);
    int (*config_aneg)(struct phy_device *);
    int (*aneg_done)(struct phy_device *);
    int (*read_status)(struct phy_device *);
    int (*ack_interrupt)(struct phy_device *);
    int (*config_intr)(struct phy_device *);
    int (*did_interrupt)(struct phy_device *);
    void (*remove)(struct phy_device *);
    int (*match_phy_device)(struct phy_device *);
    int (*ts_info)(struct phy_device *, struct ethtool_ts_info *);
    int (*hwtstamp)(struct phy_device *, struct ifreq *);
    bool (*rxtstamp)(struct phy_device *, struct sk_buff *, int);
    void (*txtstamp)(struct phy_device *, struct sk_buff *, int);
    int (*set_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*get_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*link_change_notify)(struct phy_device *);
    int (*read_mmd)(struct phy_device *, int, u16);
    int (*write_mmd)(struct phy_device *, int, u16, u16);
    int (*module_info)(struct phy_device *, struct ethtool_modinfo *);
    int (*module_eeprom)(struct phy_device *, struct ethtool_eeprom *, u8 *);
    int (*get_sset_count)(struct phy_device *);
    void (*get_strings)(struct phy_device *, u8 *);
    void (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*get_tunable)(struct phy_device *, struct ethtool_tunable *, void *);
    int (*set_tunable)(struct phy_device *, struct ethtool_tunable *, const void *);
    int (*set_loopback)(struct phy_device *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct phy_driver {
    struct mdio_driver_common mdiodrv;
    u32 phy_id;
    char *name;
    u32 phy_id_mask;
    u32 features;
    u32 flags;
    const void *driver_data;
    int (*soft_reset)(struct phy_device *);
    int (*config_init)(struct phy_device *);
    int (*probe)(struct phy_device *);
    int (*suspend)(struct phy_device *);
    int (*resume)(struct phy_device *);
    int (*config_aneg)(struct phy_device *);
    int (*aneg_done)(struct phy_device *);
    int (*read_status)(struct phy_device *);
    int (*ack_interrupt)(struct phy_device *);
    int (*config_intr)(struct phy_device *);
    int (*did_interrupt)(struct phy_device *);
    void (*remove)(struct phy_device *);
    int (*match_phy_device)(struct phy_device *);
    int (*ts_info)(struct phy_device *, struct ethtool_ts_info *);
    int (*hwtstamp)(struct phy_device *, struct ifreq *);
    bool (*rxtstamp)(struct phy_device *, struct sk_buff *, int);
    void (*txtstamp)(struct phy_device *, struct sk_buff *, int);
    int (*set_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*get_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*link_change_notify)(struct phy_device *);
    int (*read_mmd)(struct phy_device *, int, u16);
    int (*write_mmd)(struct phy_device *, int, u16, u16);
    int (*read_page)(struct phy_device *);
    int (*write_page)(struct phy_device *, int);
    int (*module_info)(struct phy_device *, struct ethtool_modinfo *);
    int (*module_eeprom)(struct phy_device *, struct ethtool_eeprom *, u8 *);
    int (*get_sset_count)(struct phy_device *);
    void (*get_strings)(struct phy_device *, u8 *);
    void (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*get_tunable)(struct phy_device *, struct ethtool_tunable *, void *);
    int (*set_tunable)(struct phy_device *, struct ethtool_tunable *, const void *);
    int (*set_loopback)(struct phy_device *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct phy_driver {
    struct mdio_driver_common mdiodrv;
    u32 phy_id;
    char *name;
    u32 phy_id_mask;
    const const long unsigned int * features;
    u32 flags;
    const void *driver_data;
    int (*soft_reset)(struct phy_device *);
    int (*config_init)(struct phy_device *);
    int (*probe)(struct phy_device *);
    int (*suspend)(struct phy_device *);
    int (*resume)(struct phy_device *);
    int (*config_aneg)(struct phy_device *);
    int (*aneg_done)(struct phy_device *);
    int (*read_status)(struct phy_device *);
    int (*ack_interrupt)(struct phy_device *);
    int (*config_intr)(struct phy_device *);
    int (*did_interrupt)(struct phy_device *);
    void (*remove)(struct phy_device *);
    int (*match_phy_device)(struct phy_device *);
    int (*ts_info)(struct phy_device *, struct ethtool_ts_info *);
    int (*hwtstamp)(struct phy_device *, struct ifreq *);
    bool (*rxtstamp)(struct phy_device *, struct sk_buff *, int);
    void (*txtstamp)(struct phy_device *, struct sk_buff *, int);
    int (*set_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*get_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*link_change_notify)(struct phy_device *);
    int (*read_mmd)(struct phy_device *, int, u16);
    int (*write_mmd)(struct phy_device *, int, u16, u16);
    int (*read_page)(struct phy_device *);
    int (*write_page)(struct phy_device *, int);
    int (*module_info)(struct phy_device *, struct ethtool_modinfo *);
    int (*module_eeprom)(struct phy_device *, struct ethtool_eeprom *, u8 *);
    int (*get_sset_count)(struct phy_device *);
    void (*get_strings)(struct phy_device *, u8 *);
    void (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*get_tunable)(struct phy_device *, struct ethtool_tunable *, void *);
    int (*set_tunable)(struct phy_device *, struct ethtool_tunable *, const void *);
    int (*set_loopback)(struct phy_device *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct phy_driver {
    struct mdio_driver_common mdiodrv;
    u32 phy_id;
    char *name;
    u32 phy_id_mask;
    const const long unsigned int * features;
    u32 flags;
    const void *driver_data;
    int (*soft_reset)(struct phy_device *);
    int (*config_init)(struct phy_device *);
    int (*probe)(struct phy_device *);
    int (*get_features)(struct phy_device *);
    int (*suspend)(struct phy_device *);
    int (*resume)(struct phy_device *);
    int (*config_aneg)(struct phy_device *);
    int (*aneg_done)(struct phy_device *);
    int (*read_status)(struct phy_device *);
    int (*ack_interrupt)(struct phy_device *);
    int (*config_intr)(struct phy_device *);
    int (*did_interrupt)(struct phy_device *);
    int (*handle_interrupt)(struct phy_device *);
    void (*remove)(struct phy_device *);
    int (*match_phy_device)(struct phy_device *);
    int (*ts_info)(struct phy_device *, struct ethtool_ts_info *);
    int (*hwtstamp)(struct phy_device *, struct ifreq *);
    bool (*rxtstamp)(struct phy_device *, struct sk_buff *, int);
    void (*txtstamp)(struct phy_device *, struct sk_buff *, int);
    int (*set_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*get_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*link_change_notify)(struct phy_device *);
    int (*read_mmd)(struct phy_device *, int, u16);
    int (*write_mmd)(struct phy_device *, int, u16, u16);
    int (*read_page)(struct phy_device *);
    int (*write_page)(struct phy_device *, int);
    int (*module_info)(struct phy_device *, struct ethtool_modinfo *);
    int (*module_eeprom)(struct phy_device *, struct ethtool_eeprom *, u8 *);
    int (*get_sset_count)(struct phy_device *);
    void (*get_strings)(struct phy_device *, u8 *);
    void (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*get_tunable)(struct phy_device *, struct ethtool_tunable *, void *);
    int (*set_tunable)(struct phy_device *, struct ethtool_tunable *, const void *);
    int (*set_loopback)(struct phy_device *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct phy_driver {
    struct mdio_driver_common mdiodrv;
    u32 phy_id;
    char *name;
    u32 phy_id_mask;
    const const long unsigned int * features;
    u32 flags;
    const void *driver_data;
    int (*soft_reset)(struct phy_device *);
    int (*config_init)(struct phy_device *);
    int (*probe)(struct phy_device *);
    int (*get_features)(struct phy_device *);
    int (*suspend)(struct phy_device *);
    int (*resume)(struct phy_device *);
    int (*config_aneg)(struct phy_device *);
    int (*aneg_done)(struct phy_device *);
    int (*read_status)(struct phy_device *);
    int (*ack_interrupt)(struct phy_device *);
    int (*config_intr)(struct phy_device *);
    int (*did_interrupt)(struct phy_device *);
    int (*handle_interrupt)(struct phy_device *);
    void (*remove)(struct phy_device *);
    int (*match_phy_device)(struct phy_device *);
    int (*ts_info)(struct phy_device *, struct ethtool_ts_info *);
    int (*hwtstamp)(struct phy_device *, struct ifreq *);
    bool (*rxtstamp)(struct phy_device *, struct sk_buff *, int);
    void (*txtstamp)(struct phy_device *, struct sk_buff *, int);
    int (*set_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*get_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*link_change_notify)(struct phy_device *);
    int (*read_mmd)(struct phy_device *, int, u16);
    int (*write_mmd)(struct phy_device *, int, u16, u16);
    int (*read_page)(struct phy_device *);
    int (*write_page)(struct phy_device *, int);
    int (*module_info)(struct phy_device *, struct ethtool_modinfo *);
    int (*module_eeprom)(struct phy_device *, struct ethtool_eeprom *, u8 *);
    int (*get_sset_count)(struct phy_device *);
    void (*get_strings)(struct phy_device *, u8 *);
    void (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*get_tunable)(struct phy_device *, struct ethtool_tunable *, void *);
    int (*set_tunable)(struct phy_device *, struct ethtool_tunable *, const void *);
    int (*set_loopback)(struct phy_device *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct phy_driver {
    struct mdio_driver_common mdiodrv;
    u32 phy_id;
    char *name;
    u32 phy_id_mask;
    const const long unsigned int * features;
    u32 flags;
    const void *driver_data;
    int (*soft_reset)(struct phy_device *);
    int (*config_init)(struct phy_device *);
    int (*probe)(struct phy_device *);
    int (*get_features)(struct phy_device *);
    int (*suspend)(struct phy_device *);
    int (*resume)(struct phy_device *);
    int (*config_aneg)(struct phy_device *);
    int (*aneg_done)(struct phy_device *);
    int (*read_status)(struct phy_device *);
    int (*ack_interrupt)(struct phy_device *);
    int (*config_intr)(struct phy_device *);
    int (*did_interrupt)(struct phy_device *);
    irqreturn_t (*handle_interrupt)(struct phy_device *);
    void (*remove)(struct phy_device *);
    int (*match_phy_device)(struct phy_device *);
    int (*set_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*get_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*link_change_notify)(struct phy_device *);
    int (*read_mmd)(struct phy_device *, int, u16);
    int (*write_mmd)(struct phy_device *, int, u16, u16);
    int (*read_page)(struct phy_device *);
    int (*write_page)(struct phy_device *, int);
    int (*module_info)(struct phy_device *, struct ethtool_modinfo *);
    int (*module_eeprom)(struct phy_device *, struct ethtool_eeprom *, u8 *);
    int (*cable_test_start)(struct phy_device *);
    int (*cable_test_tdr_start)(struct phy_device *, const struct phy_tdr_config *);
    int (*cable_test_get_status)(struct phy_device *, bool *);
    int (*get_sset_count)(struct phy_device *);
    void (*get_strings)(struct phy_device *, u8 *);
    void (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*get_tunable)(struct phy_device *, struct ethtool_tunable *, void *);
    int (*set_tunable)(struct phy_device *, struct ethtool_tunable *, const void *);
    int (*set_loopback)(struct phy_device *, bool);
    int (*get_sqi)(struct phy_device *);
    int (*get_sqi_max)(struct phy_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct phy_driver {
    struct mdio_driver_common mdiodrv;
    u32 phy_id;
    char *name;
    u32 phy_id_mask;
    const const long unsigned int * features;
    u32 flags;
    const void *driver_data;
    int (*soft_reset)(struct phy_device *);
    int (*config_init)(struct phy_device *);
    int (*probe)(struct phy_device *);
    int (*get_features)(struct phy_device *);
    int (*suspend)(struct phy_device *);
    int (*resume)(struct phy_device *);
    int (*config_aneg)(struct phy_device *);
    int (*aneg_done)(struct phy_device *);
    int (*read_status)(struct phy_device *);
    int (*config_intr)(struct phy_device *);
    irqreturn_t (*handle_interrupt)(struct phy_device *);
    void (*remove)(struct phy_device *);
    int (*match_phy_device)(struct phy_device *);
    int (*set_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*get_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*link_change_notify)(struct phy_device *);
    int (*read_mmd)(struct phy_device *, int, u16);
    int (*write_mmd)(struct phy_device *, int, u16, u16);
    int (*read_page)(struct phy_device *);
    int (*write_page)(struct phy_device *, int);
    int (*module_info)(struct phy_device *, struct ethtool_modinfo *);
    int (*module_eeprom)(struct phy_device *, struct ethtool_eeprom *, u8 *);
    int (*cable_test_start)(struct phy_device *);
    int (*cable_test_tdr_start)(struct phy_device *, const struct phy_tdr_config *);
    int (*cable_test_get_status)(struct phy_device *, bool *);
    int (*get_sset_count)(struct phy_device *);
    void (*get_strings)(struct phy_device *, u8 *);
    void (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*get_tunable)(struct phy_device *, struct ethtool_tunable *, void *);
    int (*set_tunable)(struct phy_device *, struct ethtool_tunable *, const void *);
    int (*set_loopback)(struct phy_device *, bool);
    int (*get_sqi)(struct phy_device *);
    int (*get_sqi_max)(struct phy_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct phy_driver {
    struct mdio_driver_common mdiodrv;
    u32 phy_id;
    char *name;
    u32 phy_id_mask;
    const const long unsigned int * features;
    u32 flags;
    const void *driver_data;
    int (*soft_reset)(struct phy_device *);
    int (*config_init)(struct phy_device *);
    int (*probe)(struct phy_device *);
    int (*get_features)(struct phy_device *);
    int (*suspend)(struct phy_device *);
    int (*resume)(struct phy_device *);
    int (*config_aneg)(struct phy_device *);
    int (*aneg_done)(struct phy_device *);
    int (*read_status)(struct phy_device *);
    int (*config_intr)(struct phy_device *);
    irqreturn_t (*handle_interrupt)(struct phy_device *);
    void (*remove)(struct phy_device *);
    int (*match_phy_device)(struct phy_device *);
    int (*set_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*get_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*link_change_notify)(struct phy_device *);
    int (*read_mmd)(struct phy_device *, int, u16);
    int (*write_mmd)(struct phy_device *, int, u16, u16);
    int (*read_page)(struct phy_device *);
    int (*write_page)(struct phy_device *, int);
    int (*module_info)(struct phy_device *, struct ethtool_modinfo *);
    int (*module_eeprom)(struct phy_device *, struct ethtool_eeprom *, u8 *);
    int (*cable_test_start)(struct phy_device *);
    int (*cable_test_tdr_start)(struct phy_device *, const struct phy_tdr_config *);
    int (*cable_test_get_status)(struct phy_device *, bool *);
    int (*get_sset_count)(struct phy_device *);
    void (*get_strings)(struct phy_device *, u8 *);
    void (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*get_tunable)(struct phy_device *, struct ethtool_tunable *, void *);
    int (*set_tunable)(struct phy_device *, struct ethtool_tunable *, const void *);
    int (*set_loopback)(struct phy_device *, bool);
    int (*get_sqi)(struct phy_device *);
    int (*get_sqi_max)(struct phy_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct phy_driver {
    struct mdio_driver_common mdiodrv;
    u32 phy_id;
    char *name;
    u32 phy_id_mask;
    const const long unsigned int * features;
    u32 flags;
    const void *driver_data;
    int (*soft_reset)(struct phy_device *);
    int (*config_init)(struct phy_device *);
    int (*probe)(struct phy_device *);
    int (*get_features)(struct phy_device *);
    int (*suspend)(struct phy_device *);
    int (*resume)(struct phy_device *);
    int (*config_aneg)(struct phy_device *);
    int (*aneg_done)(struct phy_device *);
    int (*read_status)(struct phy_device *);
    int (*config_intr)(struct phy_device *);
    irqreturn_t (*handle_interrupt)(struct phy_device *);
    void (*remove)(struct phy_device *);
    int (*match_phy_device)(struct phy_device *);
    int (*set_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*get_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*link_change_notify)(struct phy_device *);
    int (*read_mmd)(struct phy_device *, int, u16);
    int (*write_mmd)(struct phy_device *, int, u16, u16);
    int (*read_page)(struct phy_device *);
    int (*write_page)(struct phy_device *, int);
    int (*module_info)(struct phy_device *, struct ethtool_modinfo *);
    int (*module_eeprom)(struct phy_device *, struct ethtool_eeprom *, u8 *);
    int (*cable_test_start)(struct phy_device *);
    int (*cable_test_tdr_start)(struct phy_device *, const struct phy_tdr_config *);
    int (*cable_test_get_status)(struct phy_device *, bool *);
    int (*get_sset_count)(struct phy_device *);
    void (*get_strings)(struct phy_device *, u8 *);
    void (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*get_tunable)(struct phy_device *, struct ethtool_tunable *, void *);
    int (*set_tunable)(struct phy_device *, struct ethtool_tunable *, const void *);
    int (*set_loopback)(struct phy_device *, bool);
    int (*get_sqi)(struct phy_device *);
    int (*get_sqi_max)(struct phy_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct phy_driver {
    struct mdio_driver_common mdiodrv;
    u32 phy_id;
    char *name;
    u32 phy_id_mask;
    const const long unsigned int * features;
    u32 flags;
    const void *driver_data;
    int (*soft_reset)(struct phy_device *);
    int (*config_init)(struct phy_device *);
    int (*probe)(struct phy_device *);
    int (*get_features)(struct phy_device *);
    int (*suspend)(struct phy_device *);
    int (*resume)(struct phy_device *);
    int (*config_aneg)(struct phy_device *);
    int (*aneg_done)(struct phy_device *);
    int (*read_status)(struct phy_device *);
    int (*config_intr)(struct phy_device *);
    irqreturn_t (*handle_interrupt)(struct phy_device *);
    void (*remove)(struct phy_device *);
    int (*match_phy_device)(struct phy_device *);
    int (*set_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*get_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*link_change_notify)(struct phy_device *);
    int (*read_mmd)(struct phy_device *, int, u16);
    int (*write_mmd)(struct phy_device *, int, u16, u16);
    int (*read_page)(struct phy_device *);
    int (*write_page)(struct phy_device *, int);
    int (*module_info)(struct phy_device *, struct ethtool_modinfo *);
    int (*module_eeprom)(struct phy_device *, struct ethtool_eeprom *, u8 *);
    int (*cable_test_start)(struct phy_device *);
    int (*cable_test_tdr_start)(struct phy_device *, const struct phy_tdr_config *);
    int (*cable_test_get_status)(struct phy_device *, bool *);
    int (*get_sset_count)(struct phy_device *);
    void (*get_strings)(struct phy_device *, u8 *);
    void (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*get_tunable)(struct phy_device *, struct ethtool_tunable *, void *);
    int (*set_tunable)(struct phy_device *, struct ethtool_tunable *, const void *);
    int (*set_loopback)(struct phy_device *, bool);
    int (*get_sqi)(struct phy_device *);
    int (*get_sqi_max)(struct phy_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct phy_driver {
    struct mdio_driver_common mdiodrv;
    u32 phy_id;
    char *name;
    u32 phy_id_mask;
    const const long unsigned int * features;
    u32 flags;
    const void *driver_data;
    int (*soft_reset)(struct phy_device *);
    int (*config_init)(struct phy_device *);
    int (*probe)(struct phy_device *);
    int (*get_features)(struct phy_device *);
    int (*get_rate_matching)(struct phy_device *, phy_interface_t);
    int (*suspend)(struct phy_device *);
    int (*resume)(struct phy_device *);
    int (*config_aneg)(struct phy_device *);
    int (*aneg_done)(struct phy_device *);
    int (*read_status)(struct phy_device *);
    int (*config_intr)(struct phy_device *);
    irqreturn_t (*handle_interrupt)(struct phy_device *);
    void (*remove)(struct phy_device *);
    int (*match_phy_device)(struct phy_device *);
    int (*set_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*get_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*link_change_notify)(struct phy_device *);
    int (*read_mmd)(struct phy_device *, int, u16);
    int (*write_mmd)(struct phy_device *, int, u16, u16);
    int (*read_page)(struct phy_device *);
    int (*write_page)(struct phy_device *, int);
    int (*module_info)(struct phy_device *, struct ethtool_modinfo *);
    int (*module_eeprom)(struct phy_device *, struct ethtool_eeprom *, u8 *);
    int (*cable_test_start)(struct phy_device *);
    int (*cable_test_tdr_start)(struct phy_device *, const struct phy_tdr_config *);
    int (*cable_test_get_status)(struct phy_device *, bool *);
    int (*get_sset_count)(struct phy_device *);
    void (*get_strings)(struct phy_device *, u8 *);
    void (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*get_tunable)(struct phy_device *, struct ethtool_tunable *, void *);
    int (*set_tunable)(struct phy_device *, struct ethtool_tunable *, const void *);
    int (*set_loopback)(struct phy_device *, bool);
    int (*get_sqi)(struct phy_device *);
    int (*get_sqi_max)(struct phy_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct phy_driver {
    struct mdio_driver_common mdiodrv;
    u32 phy_id;
    char *name;
    u32 phy_id_mask;
    const const long unsigned int * features;
    u32 flags;
    const void *driver_data;
    int (*soft_reset)(struct phy_device *);
    int (*config_init)(struct phy_device *);
    int (*probe)(struct phy_device *);
    int (*get_features)(struct phy_device *);
    int (*get_rate_matching)(struct phy_device *, phy_interface_t);
    int (*suspend)(struct phy_device *);
    int (*resume)(struct phy_device *);
    int (*config_aneg)(struct phy_device *);
    int (*aneg_done)(struct phy_device *);
    int (*read_status)(struct phy_device *);
    int (*config_intr)(struct phy_device *);
    irqreturn_t (*handle_interrupt)(struct phy_device *);
    void (*remove)(struct phy_device *);
    int (*match_phy_device)(struct phy_device *);
    int (*set_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*get_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*link_change_notify)(struct phy_device *);
    int (*read_mmd)(struct phy_device *, int, u16);
    int (*write_mmd)(struct phy_device *, int, u16, u16);
    int (*read_page)(struct phy_device *);
    int (*write_page)(struct phy_device *, int);
    int (*module_info)(struct phy_device *, struct ethtool_modinfo *);
    int (*module_eeprom)(struct phy_device *, struct ethtool_eeprom *, u8 *);
    int (*cable_test_start)(struct phy_device *);
    int (*cable_test_tdr_start)(struct phy_device *, const struct phy_tdr_config *);
    int (*cable_test_get_status)(struct phy_device *, bool *);
    int (*get_sset_count)(struct phy_device *);
    void (*get_strings)(struct phy_device *, u8 *);
    void (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*get_tunable)(struct phy_device *, struct ethtool_tunable *, void *);
    int (*set_tunable)(struct phy_device *, struct ethtool_tunable *, const void *);
    int (*set_loopback)(struct phy_device *, bool);
    int (*get_sqi)(struct phy_device *);
    int (*get_sqi_max)(struct phy_device *);
    int (*get_plca_cfg)(struct phy_device *, struct phy_plca_cfg *);
    int (*set_plca_cfg)(struct phy_device *, const struct phy_plca_cfg *);
    int (*get_plca_status)(struct phy_device *, struct phy_plca_status *);
    int (*led_brightness_set)(struct phy_device *, u8, enum led_brightness);
    int (*led_blink_set)(struct phy_device *, u8, long unsigned int *, long unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct phy_driver {
    struct mdio_driver_common mdiodrv;
    u32 phy_id;
    char *name;
    u32 phy_id_mask;
    const const long unsigned int * features;
    u32 flags;
    const void *driver_data;
    int (*soft_reset)(struct phy_device *);
    int (*config_init)(struct phy_device *);
    int (*probe)(struct phy_device *);
    int (*get_features)(struct phy_device *);
    int (*get_rate_matching)(struct phy_device *, phy_interface_t);
    int (*suspend)(struct phy_device *);
    int (*resume)(struct phy_device *);
    int (*config_aneg)(struct phy_device *);
    int (*aneg_done)(struct phy_device *);
    int (*read_status)(struct phy_device *);
    int (*config_intr)(struct phy_device *);
    irqreturn_t (*handle_interrupt)(struct phy_device *);
    void (*remove)(struct phy_device *);
    int (*match_phy_device)(struct phy_device *);
    int (*set_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*get_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*link_change_notify)(struct phy_device *);
    int (*read_mmd)(struct phy_device *, int, u16);
    int (*write_mmd)(struct phy_device *, int, u16, u16);
    int (*read_page)(struct phy_device *);
    int (*write_page)(struct phy_device *, int);
    int (*module_info)(struct phy_device *, struct ethtool_modinfo *);
    int (*module_eeprom)(struct phy_device *, struct ethtool_eeprom *, u8 *);
    int (*cable_test_start)(struct phy_device *);
    int (*cable_test_tdr_start)(struct phy_device *, const struct phy_tdr_config *);
    int (*cable_test_get_status)(struct phy_device *, bool *);
    int (*get_sset_count)(struct phy_device *);
    void (*get_strings)(struct phy_device *, u8 *);
    void (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*get_tunable)(struct phy_device *, struct ethtool_tunable *, void *);
    int (*set_tunable)(struct phy_device *, struct ethtool_tunable *, const void *);
    int (*set_loopback)(struct phy_device *, bool);
    int (*get_sqi)(struct phy_device *);
    int (*get_sqi_max)(struct phy_device *);
    int (*get_plca_cfg)(struct phy_device *, struct phy_plca_cfg *);
    int (*set_plca_cfg)(struct phy_device *, const struct phy_plca_cfg *);
    int (*get_plca_status)(struct phy_device *, struct phy_plca_status *);
    int (*led_brightness_set)(struct phy_device *, u8, enum led_brightness);
    int (*led_blink_set)(struct phy_device *, u8, long unsigned int *, long unsigned int *);
    int (*led_hw_is_supported)(struct phy_device *, u8, long unsigned int);
    int (*led_hw_control_set)(struct phy_device *, u8, long unsigned int);
    int (*led_hw_control_get)(struct phy_device *, u8, long unsigned int *);
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
struct phy_driver {
    struct mdio_driver_common mdiodrv;
    u32 phy_id;
    char *name;
    u32 phy_id_mask;
    const const long unsigned int * features;
    u32 flags;
    const void *driver_data;
    int (*soft_reset)(struct phy_device *);
    int (*config_init)(struct phy_device *);
    int (*probe)(struct phy_device *);
    int (*get_features)(struct phy_device *);
    int (*suspend)(struct phy_device *);
    int (*resume)(struct phy_device *);
    int (*config_aneg)(struct phy_device *);
    int (*aneg_done)(struct phy_device *);
    int (*read_status)(struct phy_device *);
    int (*ack_interrupt)(struct phy_device *);
    int (*config_intr)(struct phy_device *);
    int (*did_interrupt)(struct phy_device *);
    int (*handle_interrupt)(struct phy_device *);
    void (*remove)(struct phy_device *);
    int (*match_phy_device)(struct phy_device *);
    int (*ts_info)(struct phy_device *, struct ethtool_ts_info *);
    int (*hwtstamp)(struct phy_device *, struct ifreq *);
    bool (*rxtstamp)(struct phy_device *, struct sk_buff *, int);
    void (*txtstamp)(struct phy_device *, struct sk_buff *, int);
    int (*set_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*get_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*link_change_notify)(struct phy_device *);
    int (*read_mmd)(struct phy_device *, int, u16);
    int (*write_mmd)(struct phy_device *, int, u16, u16);
    int (*read_page)(struct phy_device *);
    int (*write_page)(struct phy_device *, int);
    int (*module_info)(struct phy_device *, struct ethtool_modinfo *);
    int (*module_eeprom)(struct phy_device *, struct ethtool_eeprom *, u8 *);
    int (*get_sset_count)(struct phy_device *);
    void (*get_strings)(struct phy_device *, u8 *);
    void (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*get_tunable)(struct phy_device *, struct ethtool_tunable *, void *);
    int (*set_tunable)(struct phy_device *, struct ethtool_tunable *, const void *);
    int (*set_loopback)(struct phy_device *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct phy_driver {
    struct mdio_driver_common mdiodrv;
    u32 phy_id;
    char *name;
    u32 phy_id_mask;
    const const long unsigned int * features;
    u32 flags;
    const void *driver_data;
    int (*soft_reset)(struct phy_device *);
    int (*config_init)(struct phy_device *);
    int (*probe)(struct phy_device *);
    int (*get_features)(struct phy_device *);
    int (*suspend)(struct phy_device *);
    int (*resume)(struct phy_device *);
    int (*config_aneg)(struct phy_device *);
    int (*aneg_done)(struct phy_device *);
    int (*read_status)(struct phy_device *);
    int (*ack_interrupt)(struct phy_device *);
    int (*config_intr)(struct phy_device *);
    int (*did_interrupt)(struct phy_device *);
    int (*handle_interrupt)(struct phy_device *);
    void (*remove)(struct phy_device *);
    int (*match_phy_device)(struct phy_device *);
    int (*ts_info)(struct phy_device *, struct ethtool_ts_info *);
    int (*hwtstamp)(struct phy_device *, struct ifreq *);
    bool (*rxtstamp)(struct phy_device *, struct sk_buff *, int);
    void (*txtstamp)(struct phy_device *, struct sk_buff *, int);
    int (*set_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*get_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*link_change_notify)(struct phy_device *);
    int (*read_mmd)(struct phy_device *, int, u16);
    int (*write_mmd)(struct phy_device *, int, u16, u16);
    int (*read_page)(struct phy_device *);
    int (*write_page)(struct phy_device *, int);
    int (*module_info)(struct phy_device *, struct ethtool_modinfo *);
    int (*module_eeprom)(struct phy_device *, struct ethtool_eeprom *, u8 *);
    int (*get_sset_count)(struct phy_device *);
    void (*get_strings)(struct phy_device *, u8 *);
    void (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*get_tunable)(struct phy_device *, struct ethtool_tunable *, void *);
    int (*set_tunable)(struct phy_device *, struct ethtool_tunable *, const void *);
    int (*set_loopback)(struct phy_device *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct phy_driver {
    struct mdio_driver_common mdiodrv;
    u32 phy_id;
    char *name;
    u32 phy_id_mask;
    const const long unsigned int * features;
    u32 flags;
    const void *driver_data;
    int (*soft_reset)(struct phy_device *);
    int (*config_init)(struct phy_device *);
    int (*probe)(struct phy_device *);
    int (*get_features)(struct phy_device *);
    int (*suspend)(struct phy_device *);
    int (*resume)(struct phy_device *);
    int (*config_aneg)(struct phy_device *);
    int (*aneg_done)(struct phy_device *);
    int (*read_status)(struct phy_device *);
    int (*ack_interrupt)(struct phy_device *);
    int (*config_intr)(struct phy_device *);
    int (*did_interrupt)(struct phy_device *);
    int (*handle_interrupt)(struct phy_device *);
    void (*remove)(struct phy_device *);
    int (*match_phy_device)(struct phy_device *);
    int (*ts_info)(struct phy_device *, struct ethtool_ts_info *);
    int (*hwtstamp)(struct phy_device *, struct ifreq *);
    bool (*rxtstamp)(struct phy_device *, struct sk_buff *, int);
    void (*txtstamp)(struct phy_device *, struct sk_buff *, int);
    int (*set_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*get_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*link_change_notify)(struct phy_device *);
    int (*read_mmd)(struct phy_device *, int, u16);
    int (*write_mmd)(struct phy_device *, int, u16, u16);
    int (*read_page)(struct phy_device *);
    int (*write_page)(struct phy_device *, int);
    int (*module_info)(struct phy_device *, struct ethtool_modinfo *);
    int (*module_eeprom)(struct phy_device *, struct ethtool_eeprom *, u8 *);
    int (*get_sset_count)(struct phy_device *);
    void (*get_strings)(struct phy_device *, u8 *);
    void (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*get_tunable)(struct phy_device *, struct ethtool_tunable *, void *);
    int (*set_tunable)(struct phy_device *, struct ethtool_tunable *, const void *);
    int (*set_loopback)(struct phy_device *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct phy_driver {
    struct mdio_driver_common mdiodrv;
    u32 phy_id;
    char *name;
    u32 phy_id_mask;
    const const long unsigned int * features;
    u32 flags;
    const void *driver_data;
    int (*soft_reset)(struct phy_device *);
    int (*config_init)(struct phy_device *);
    int (*probe)(struct phy_device *);
    int (*get_features)(struct phy_device *);
    int (*suspend)(struct phy_device *);
    int (*resume)(struct phy_device *);
    int (*config_aneg)(struct phy_device *);
    int (*aneg_done)(struct phy_device *);
    int (*read_status)(struct phy_device *);
    int (*ack_interrupt)(struct phy_device *);
    int (*config_intr)(struct phy_device *);
    int (*did_interrupt)(struct phy_device *);
    int (*handle_interrupt)(struct phy_device *);
    void (*remove)(struct phy_device *);
    int (*match_phy_device)(struct phy_device *);
    int (*ts_info)(struct phy_device *, struct ethtool_ts_info *);
    int (*hwtstamp)(struct phy_device *, struct ifreq *);
    bool (*rxtstamp)(struct phy_device *, struct sk_buff *, int);
    void (*txtstamp)(struct phy_device *, struct sk_buff *, int);
    int (*set_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*get_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*link_change_notify)(struct phy_device *);
    int (*read_mmd)(struct phy_device *, int, u16);
    int (*write_mmd)(struct phy_device *, int, u16, u16);
    int (*read_page)(struct phy_device *);
    int (*write_page)(struct phy_device *, int);
    int (*module_info)(struct phy_device *, struct ethtool_modinfo *);
    int (*module_eeprom)(struct phy_device *, struct ethtool_eeprom *, u8 *);
    int (*get_sset_count)(struct phy_device *);
    void (*get_strings)(struct phy_device *, u8 *);
    void (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*get_tunable)(struct phy_device *, struct ethtool_tunable *, void *);
    int (*set_tunable)(struct phy_device *, struct ethtool_tunable *, const void *);
    int (*set_loopback)(struct phy_device *, bool);
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
struct phy_driver {
    struct mdio_driver_common mdiodrv;
    u32 phy_id;
    char *name;
    u32 phy_id_mask;
    const const long unsigned int * features;
    u32 flags;
    const void *driver_data;
    int (*soft_reset)(struct phy_device *);
    int (*config_init)(struct phy_device *);
    int (*probe)(struct phy_device *);
    int (*get_features)(struct phy_device *);
    int (*suspend)(struct phy_device *);
    int (*resume)(struct phy_device *);
    int (*config_aneg)(struct phy_device *);
    int (*aneg_done)(struct phy_device *);
    int (*read_status)(struct phy_device *);
    int (*ack_interrupt)(struct phy_device *);
    int (*config_intr)(struct phy_device *);
    int (*did_interrupt)(struct phy_device *);
    int (*handle_interrupt)(struct phy_device *);
    void (*remove)(struct phy_device *);
    int (*match_phy_device)(struct phy_device *);
    int (*ts_info)(struct phy_device *, struct ethtool_ts_info *);
    int (*hwtstamp)(struct phy_device *, struct ifreq *);
    bool (*rxtstamp)(struct phy_device *, struct sk_buff *, int);
    void (*txtstamp)(struct phy_device *, struct sk_buff *, int);
    int (*set_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*get_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*link_change_notify)(struct phy_device *);
    int (*read_mmd)(struct phy_device *, int, u16);
    int (*write_mmd)(struct phy_device *, int, u16, u16);
    int (*read_page)(struct phy_device *);
    int (*write_page)(struct phy_device *, int);
    int (*module_info)(struct phy_device *, struct ethtool_modinfo *);
    int (*module_eeprom)(struct phy_device *, struct ethtool_eeprom *, u8 *);
    int (*get_sset_count)(struct phy_device *);
    void (*get_strings)(struct phy_device *, u8 *);
    void (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*get_tunable)(struct phy_device *, struct ethtool_tunable *, void *);
    int (*set_tunable)(struct phy_device *, struct ethtool_tunable *, const void *);
    int (*set_loopback)(struct phy_device *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct phy_driver {
    struct mdio_driver_common mdiodrv;
    u32 phy_id;
    char *name;
    u32 phy_id_mask;
    const const long unsigned int * features;
    u32 flags;
    const void *driver_data;
    int (*soft_reset)(struct phy_device *);
    int (*config_init)(struct phy_device *);
    int (*probe)(struct phy_device *);
    int (*get_features)(struct phy_device *);
    int (*suspend)(struct phy_device *);
    int (*resume)(struct phy_device *);
    int (*config_aneg)(struct phy_device *);
    int (*aneg_done)(struct phy_device *);
    int (*read_status)(struct phy_device *);
    int (*ack_interrupt)(struct phy_device *);
    int (*config_intr)(struct phy_device *);
    int (*did_interrupt)(struct phy_device *);
    int (*handle_interrupt)(struct phy_device *);
    void (*remove)(struct phy_device *);
    int (*match_phy_device)(struct phy_device *);
    int (*ts_info)(struct phy_device *, struct ethtool_ts_info *);
    int (*hwtstamp)(struct phy_device *, struct ifreq *);
    bool (*rxtstamp)(struct phy_device *, struct sk_buff *, int);
    void (*txtstamp)(struct phy_device *, struct sk_buff *, int);
    int (*set_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*get_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*link_change_notify)(struct phy_device *);
    int (*read_mmd)(struct phy_device *, int, u16);
    int (*write_mmd)(struct phy_device *, int, u16, u16);
    int (*read_page)(struct phy_device *);
    int (*write_page)(struct phy_device *, int);
    int (*module_info)(struct phy_device *, struct ethtool_modinfo *);
    int (*module_eeprom)(struct phy_device *, struct ethtool_eeprom *, u8 *);
    int (*get_sset_count)(struct phy_device *);
    void (*get_strings)(struct phy_device *, u8 *);
    void (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*get_tunable)(struct phy_device *, struct ethtool_tunable *, void *);
    int (*set_tunable)(struct phy_device *, struct ethtool_tunable *, const void *);
    int (*set_loopback)(struct phy_device *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct phy_driver {
    struct mdio_driver_common mdiodrv;
    u32 phy_id;
    char *name;
    u32 phy_id_mask;
    const const long unsigned int * features;
    u32 flags;
    const void *driver_data;
    int (*soft_reset)(struct phy_device *);
    int (*config_init)(struct phy_device *);
    int (*probe)(struct phy_device *);
    int (*get_features)(struct phy_device *);
    int (*suspend)(struct phy_device *);
    int (*resume)(struct phy_device *);
    int (*config_aneg)(struct phy_device *);
    int (*aneg_done)(struct phy_device *);
    int (*read_status)(struct phy_device *);
    int (*ack_interrupt)(struct phy_device *);
    int (*config_intr)(struct phy_device *);
    int (*did_interrupt)(struct phy_device *);
    int (*handle_interrupt)(struct phy_device *);
    void (*remove)(struct phy_device *);
    int (*match_phy_device)(struct phy_device *);
    int (*ts_info)(struct phy_device *, struct ethtool_ts_info *);
    int (*hwtstamp)(struct phy_device *, struct ifreq *);
    bool (*rxtstamp)(struct phy_device *, struct sk_buff *, int);
    void (*txtstamp)(struct phy_device *, struct sk_buff *, int);
    int (*set_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*get_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*link_change_notify)(struct phy_device *);
    int (*read_mmd)(struct phy_device *, int, u16);
    int (*write_mmd)(struct phy_device *, int, u16, u16);
    int (*read_page)(struct phy_device *);
    int (*write_page)(struct phy_device *, int);
    int (*module_info)(struct phy_device *, struct ethtool_modinfo *);
    int (*module_eeprom)(struct phy_device *, struct ethtool_eeprom *, u8 *);
    int (*get_sset_count)(struct phy_device *);
    void (*get_strings)(struct phy_device *, u8 *);
    void (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*get_tunable)(struct phy_device *, struct ethtool_tunable *, void *);
    int (*set_tunable)(struct phy_device *, struct ethtool_tunable *, const void *);
    int (*set_loopback)(struct phy_device *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct phy_driver {
    struct mdio_driver_common mdiodrv;
    u32 phy_id;
    char *name;
    u32 phy_id_mask;
    const const long unsigned int * features;
    u32 flags;
    const void *driver_data;
    int (*soft_reset)(struct phy_device *);
    int (*config_init)(struct phy_device *);
    int (*probe)(struct phy_device *);
    int (*get_features)(struct phy_device *);
    int (*suspend)(struct phy_device *);
    int (*resume)(struct phy_device *);
    int (*config_aneg)(struct phy_device *);
    int (*aneg_done)(struct phy_device *);
    int (*read_status)(struct phy_device *);
    int (*ack_interrupt)(struct phy_device *);
    int (*config_intr)(struct phy_device *);
    int (*did_interrupt)(struct phy_device *);
    int (*handle_interrupt)(struct phy_device *);
    void (*remove)(struct phy_device *);
    int (*match_phy_device)(struct phy_device *);
    int (*ts_info)(struct phy_device *, struct ethtool_ts_info *);
    int (*hwtstamp)(struct phy_device *, struct ifreq *);
    bool (*rxtstamp)(struct phy_device *, struct sk_buff *, int);
    void (*txtstamp)(struct phy_device *, struct sk_buff *, int);
    int (*set_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*get_wol)(struct phy_device *, struct ethtool_wolinfo *);
    void (*link_change_notify)(struct phy_device *);
    int (*read_mmd)(struct phy_device *, int, u16);
    int (*write_mmd)(struct phy_device *, int, u16, u16);
    int (*read_page)(struct phy_device *);
    int (*write_page)(struct phy_device *, int);
    int (*module_info)(struct phy_device *, struct ethtool_modinfo *);
    int (*module_eeprom)(struct phy_device *, struct ethtool_eeprom *, u8 *);
    int (*get_sset_count)(struct phy_device *);
    void (*get_strings)(struct phy_device *, u8 *);
    void (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*get_tunable)(struct phy_device *, struct ethtool_tunable *, void *);
    int (*set_tunable)(struct phy_device *, struct ethtool_tunable *, const void *);
    int (*set_loopback)(struct phy_device *, bool);
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
<code>struct mdio_driver_common mdiodrv</code>
</li>
<li>
<b>Field added. </b>
<code>int (*get_sset_count)(struct phy_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*get_strings)(struct phy_device *, u8 *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct device_driver driver</code>
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
<code>int (*get_tunable)(struct phy_device *, struct ethtool_tunable *, void *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_tunable)(struct phy_device *, struct ethtool_tunable *, const void *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*read_mmd)(struct phy_device *, int, u16)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*write_mmd)(struct phy_device *, int, u16, u16)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_loopback)(struct phy_device *, bool)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*read_mmd_indirect)(struct phy_device *, int, int, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*write_mmd_indirect)(struct phy_device *, int, int, int, u32)</code>
</li>
</ul>
</details>
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
<code>int (*read_page)(struct phy_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*write_page)(struct phy_device *, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int phy_id_mask</code> ➡️ <code>u32 phy_id_mask</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>u32 features</code> ➡️ <code>const const long unsigned int * features</code>
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
<code>int (*get_features)(struct phy_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*handle_interrupt)(struct phy_device *)</code>
</li>
</ul>
</details>
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
<code>int (*cable_test_start)(struct phy_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*cable_test_tdr_start)(struct phy_device *, const struct phy_tdr_config *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*cable_test_get_status)(struct phy_device *, bool *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*get_sqi)(struct phy_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*get_sqi_max)(struct phy_device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*ts_info)(struct phy_device *, struct ethtool_ts_info *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*hwtstamp)(struct phy_device *, struct ifreq *)</code>
</li>
<li>
<b>Field removed. </b>
<code>bool (*rxtstamp)(struct phy_device *, struct sk_buff *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*txtstamp)(struct phy_device *, struct sk_buff *, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*handle_interrupt)(struct phy_device *)</code> ➡️ <code>irqreturn_t (*handle_interrupt)(struct phy_device *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*ack_interrupt)(struct phy_device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*did_interrupt)(struct phy_device *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*get_rate_matching)(struct phy_device *, phy_interface_t)</code>
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
<code>int (*get_plca_cfg)(struct phy_device *, struct phy_plca_cfg *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_plca_cfg)(struct phy_device *, const struct phy_plca_cfg *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*get_plca_status)(struct phy_device *, struct phy_plca_status *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*led_brightness_set)(struct phy_device *, u8, enum led_brightness)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*led_blink_set)(struct phy_device *, u8, long unsigned int *, long unsigned int *)</code>
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
<code>int (*led_hw_is_supported)(struct phy_device *, u8, long unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*led_hw_control_set)(struct phy_device *, u8, long unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*led_hw_control_get)(struct phy_device *, u8, long unsigned int *)</code>
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
