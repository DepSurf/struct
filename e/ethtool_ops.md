# Struct: <code>ethtool_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct ethtool_ops {
    int (*get_settings)(struct net_device *, struct ethtool_cmd *);
    int (*set_settings)(struct net_device *, struct ethtool_cmd *);
    void (*get_drvinfo)(struct net_device *, struct ethtool_drvinfo *);
    int (*get_regs_len)(struct net_device *);
    void (*get_regs)(struct net_device *, struct ethtool_regs *, void *);
    void (*get_wol)(struct net_device *, struct ethtool_wolinfo *);
    int (*set_wol)(struct net_device *, struct ethtool_wolinfo *);
    u32 (*get_msglevel)(struct net_device *);
    void (*set_msglevel)(struct net_device *, u32);
    int (*nway_reset)(struct net_device *);
    u32 (*get_link)(struct net_device *);
    int (*get_eeprom_len)(struct net_device *);
    int (*get_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_coalesce)(struct net_device *, struct ethtool_coalesce *);
    int (*set_coalesce)(struct net_device *, struct ethtool_coalesce *);
    void (*get_ringparam)(struct net_device *, struct ethtool_ringparam *);
    int (*set_ringparam)(struct net_device *, struct ethtool_ringparam *);
    void (*get_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    int (*set_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    void (*self_test)(struct net_device *, struct ethtool_test *, u64 *);
    void (*get_strings)(struct net_device *, u32, u8 *);
    int (*set_phys_id)(struct net_device *, enum ethtool_phys_id_state);
    void (*get_ethtool_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*begin)(struct net_device *);
    void (*complete)(struct net_device *);
    u32 (*get_priv_flags)(struct net_device *);
    int (*set_priv_flags)(struct net_device *, u32);
    int (*get_sset_count)(struct net_device *, int);
    int (*get_rxnfc)(struct net_device *, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct net_device *, struct ethtool_rxnfc *);
    int (*flash_device)(struct net_device *, struct ethtool_flash *);
    int (*reset)(struct net_device *, u32 *);
    u32 (*get_rxfh_key_size)(struct net_device *);
    u32 (*get_rxfh_indir_size)(struct net_device *);
    int (*get_rxfh)(struct net_device *, u32 *, u8 *, u8 *);
    int (*set_rxfh)(struct net_device *, const u32 *, const u8 *, const u8);
    void (*get_channels)(struct net_device *, struct ethtool_channels *);
    int (*set_channels)(struct net_device *, struct ethtool_channels *);
    int (*get_dump_flag)(struct net_device *, struct ethtool_dump *);
    int (*get_dump_data)(struct net_device *, struct ethtool_dump *, void *);
    int (*set_dump)(struct net_device *, struct ethtool_dump *);
    int (*get_ts_info)(struct net_device *, struct ethtool_ts_info *);
    int (*get_module_info)(struct net_device *, struct ethtool_modinfo *);
    int (*get_module_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_eee)(struct net_device *, struct ethtool_eee *);
    int (*set_eee)(struct net_device *, struct ethtool_eee *);
    int (*get_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ethtool_ops {
    int (*get_settings)(struct net_device *, struct ethtool_cmd *);
    int (*set_settings)(struct net_device *, struct ethtool_cmd *);
    void (*get_drvinfo)(struct net_device *, struct ethtool_drvinfo *);
    int (*get_regs_len)(struct net_device *);
    void (*get_regs)(struct net_device *, struct ethtool_regs *, void *);
    void (*get_wol)(struct net_device *, struct ethtool_wolinfo *);
    int (*set_wol)(struct net_device *, struct ethtool_wolinfo *);
    u32 (*get_msglevel)(struct net_device *);
    void (*set_msglevel)(struct net_device *, u32);
    int (*nway_reset)(struct net_device *);
    u32 (*get_link)(struct net_device *);
    int (*get_eeprom_len)(struct net_device *);
    int (*get_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_coalesce)(struct net_device *, struct ethtool_coalesce *);
    int (*set_coalesce)(struct net_device *, struct ethtool_coalesce *);
    void (*get_ringparam)(struct net_device *, struct ethtool_ringparam *);
    int (*set_ringparam)(struct net_device *, struct ethtool_ringparam *);
    void (*get_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    int (*set_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    void (*self_test)(struct net_device *, struct ethtool_test *, u64 *);
    void (*get_strings)(struct net_device *, u32, u8 *);
    int (*set_phys_id)(struct net_device *, enum ethtool_phys_id_state);
    void (*get_ethtool_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*begin)(struct net_device *);
    void (*complete)(struct net_device *);
    u32 (*get_priv_flags)(struct net_device *);
    int (*set_priv_flags)(struct net_device *, u32);
    int (*get_sset_count)(struct net_device *, int);
    int (*get_rxnfc)(struct net_device *, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct net_device *, struct ethtool_rxnfc *);
    int (*flash_device)(struct net_device *, struct ethtool_flash *);
    int (*reset)(struct net_device *, u32 *);
    u32 (*get_rxfh_key_size)(struct net_device *);
    u32 (*get_rxfh_indir_size)(struct net_device *);
    int (*get_rxfh)(struct net_device *, u32 *, u8 *, u8 *);
    int (*set_rxfh)(struct net_device *, const u32 *, const u8 *, const u8);
    void (*get_channels)(struct net_device *, struct ethtool_channels *);
    int (*set_channels)(struct net_device *, struct ethtool_channels *);
    int (*get_dump_flag)(struct net_device *, struct ethtool_dump *);
    int (*get_dump_data)(struct net_device *, struct ethtool_dump *, void *);
    int (*set_dump)(struct net_device *, struct ethtool_dump *);
    int (*get_ts_info)(struct net_device *, struct ethtool_ts_info *);
    int (*get_module_info)(struct net_device *, struct ethtool_modinfo *);
    int (*get_module_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_eee)(struct net_device *, struct ethtool_eee *);
    int (*set_eee)(struct net_device *, struct ethtool_eee *);
    int (*get_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*set_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*get_link_ksettings)(struct net_device *, struct ethtool_link_ksettings *);
    int (*set_link_ksettings)(struct net_device *, const struct ethtool_link_ksettings *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ethtool_ops {
    int (*get_settings)(struct net_device *, struct ethtool_cmd *);
    int (*set_settings)(struct net_device *, struct ethtool_cmd *);
    void (*get_drvinfo)(struct net_device *, struct ethtool_drvinfo *);
    int (*get_regs_len)(struct net_device *);
    void (*get_regs)(struct net_device *, struct ethtool_regs *, void *);
    void (*get_wol)(struct net_device *, struct ethtool_wolinfo *);
    int (*set_wol)(struct net_device *, struct ethtool_wolinfo *);
    u32 (*get_msglevel)(struct net_device *);
    void (*set_msglevel)(struct net_device *, u32);
    int (*nway_reset)(struct net_device *);
    u32 (*get_link)(struct net_device *);
    int (*get_eeprom_len)(struct net_device *);
    int (*get_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_coalesce)(struct net_device *, struct ethtool_coalesce *);
    int (*set_coalesce)(struct net_device *, struct ethtool_coalesce *);
    void (*get_ringparam)(struct net_device *, struct ethtool_ringparam *);
    int (*set_ringparam)(struct net_device *, struct ethtool_ringparam *);
    void (*get_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    int (*set_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    void (*self_test)(struct net_device *, struct ethtool_test *, u64 *);
    void (*get_strings)(struct net_device *, u32, u8 *);
    int (*set_phys_id)(struct net_device *, enum ethtool_phys_id_state);
    void (*get_ethtool_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*begin)(struct net_device *);
    void (*complete)(struct net_device *);
    u32 (*get_priv_flags)(struct net_device *);
    int (*set_priv_flags)(struct net_device *, u32);
    int (*get_sset_count)(struct net_device *, int);
    int (*get_rxnfc)(struct net_device *, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct net_device *, struct ethtool_rxnfc *);
    int (*flash_device)(struct net_device *, struct ethtool_flash *);
    int (*reset)(struct net_device *, u32 *);
    u32 (*get_rxfh_key_size)(struct net_device *);
    u32 (*get_rxfh_indir_size)(struct net_device *);
    int (*get_rxfh)(struct net_device *, u32 *, u8 *, u8 *);
    int (*set_rxfh)(struct net_device *, const u32 *, const u8 *, const u8);
    void (*get_channels)(struct net_device *, struct ethtool_channels *);
    int (*set_channels)(struct net_device *, struct ethtool_channels *);
    int (*get_dump_flag)(struct net_device *, struct ethtool_dump *);
    int (*get_dump_data)(struct net_device *, struct ethtool_dump *, void *);
    int (*set_dump)(struct net_device *, struct ethtool_dump *);
    int (*get_ts_info)(struct net_device *, struct ethtool_ts_info *);
    int (*get_module_info)(struct net_device *, struct ethtool_modinfo *);
    int (*get_module_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_eee)(struct net_device *, struct ethtool_eee *);
    int (*set_eee)(struct net_device *, struct ethtool_eee *);
    int (*get_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*set_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*get_link_ksettings)(struct net_device *, struct ethtool_link_ksettings *);
    int (*set_link_ksettings)(struct net_device *, const struct ethtool_link_ksettings *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ethtool_ops {
    int (*get_settings)(struct net_device *, struct ethtool_cmd *);
    int (*set_settings)(struct net_device *, struct ethtool_cmd *);
    void (*get_drvinfo)(struct net_device *, struct ethtool_drvinfo *);
    int (*get_regs_len)(struct net_device *);
    void (*get_regs)(struct net_device *, struct ethtool_regs *, void *);
    void (*get_wol)(struct net_device *, struct ethtool_wolinfo *);
    int (*set_wol)(struct net_device *, struct ethtool_wolinfo *);
    u32 (*get_msglevel)(struct net_device *);
    void (*set_msglevel)(struct net_device *, u32);
    int (*nway_reset)(struct net_device *);
    u32 (*get_link)(struct net_device *);
    int (*get_eeprom_len)(struct net_device *);
    int (*get_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_coalesce)(struct net_device *, struct ethtool_coalesce *);
    int (*set_coalesce)(struct net_device *, struct ethtool_coalesce *);
    void (*get_ringparam)(struct net_device *, struct ethtool_ringparam *);
    int (*set_ringparam)(struct net_device *, struct ethtool_ringparam *);
    void (*get_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    int (*set_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    void (*self_test)(struct net_device *, struct ethtool_test *, u64 *);
    void (*get_strings)(struct net_device *, u32, u8 *);
    int (*set_phys_id)(struct net_device *, enum ethtool_phys_id_state);
    void (*get_ethtool_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*begin)(struct net_device *);
    void (*complete)(struct net_device *);
    u32 (*get_priv_flags)(struct net_device *);
    int (*set_priv_flags)(struct net_device *, u32);
    int (*get_sset_count)(struct net_device *, int);
    int (*get_rxnfc)(struct net_device *, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct net_device *, struct ethtool_rxnfc *);
    int (*flash_device)(struct net_device *, struct ethtool_flash *);
    int (*reset)(struct net_device *, u32 *);
    u32 (*get_rxfh_key_size)(struct net_device *);
    u32 (*get_rxfh_indir_size)(struct net_device *);
    int (*get_rxfh)(struct net_device *, u32 *, u8 *, u8 *);
    int (*set_rxfh)(struct net_device *, const u32 *, const u8 *, const u8);
    void (*get_channels)(struct net_device *, struct ethtool_channels *);
    int (*set_channels)(struct net_device *, struct ethtool_channels *);
    int (*get_dump_flag)(struct net_device *, struct ethtool_dump *);
    int (*get_dump_data)(struct net_device *, struct ethtool_dump *, void *);
    int (*set_dump)(struct net_device *, struct ethtool_dump *);
    int (*get_ts_info)(struct net_device *, struct ethtool_ts_info *);
    int (*get_module_info)(struct net_device *, struct ethtool_modinfo *);
    int (*get_module_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_eee)(struct net_device *, struct ethtool_eee *);
    int (*set_eee)(struct net_device *, struct ethtool_eee *);
    int (*get_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*set_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*get_link_ksettings)(struct net_device *, struct ethtool_link_ksettings *);
    int (*set_link_ksettings)(struct net_device *, const struct ethtool_link_ksettings *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ethtool_ops {
    int (*get_settings)(struct net_device *, struct ethtool_cmd *);
    int (*set_settings)(struct net_device *, struct ethtool_cmd *);
    void (*get_drvinfo)(struct net_device *, struct ethtool_drvinfo *);
    int (*get_regs_len)(struct net_device *);
    void (*get_regs)(struct net_device *, struct ethtool_regs *, void *);
    void (*get_wol)(struct net_device *, struct ethtool_wolinfo *);
    int (*set_wol)(struct net_device *, struct ethtool_wolinfo *);
    u32 (*get_msglevel)(struct net_device *);
    void (*set_msglevel)(struct net_device *, u32);
    int (*nway_reset)(struct net_device *);
    u32 (*get_link)(struct net_device *);
    int (*get_eeprom_len)(struct net_device *);
    int (*get_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_coalesce)(struct net_device *, struct ethtool_coalesce *);
    int (*set_coalesce)(struct net_device *, struct ethtool_coalesce *);
    void (*get_ringparam)(struct net_device *, struct ethtool_ringparam *);
    int (*set_ringparam)(struct net_device *, struct ethtool_ringparam *);
    void (*get_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    int (*set_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    void (*self_test)(struct net_device *, struct ethtool_test *, u64 *);
    void (*get_strings)(struct net_device *, u32, u8 *);
    int (*set_phys_id)(struct net_device *, enum ethtool_phys_id_state);
    void (*get_ethtool_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*begin)(struct net_device *);
    void (*complete)(struct net_device *);
    u32 (*get_priv_flags)(struct net_device *);
    int (*set_priv_flags)(struct net_device *, u32);
    int (*get_sset_count)(struct net_device *, int);
    int (*get_rxnfc)(struct net_device *, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct net_device *, struct ethtool_rxnfc *);
    int (*flash_device)(struct net_device *, struct ethtool_flash *);
    int (*reset)(struct net_device *, u32 *);
    u32 (*get_rxfh_key_size)(struct net_device *);
    u32 (*get_rxfh_indir_size)(struct net_device *);
    int (*get_rxfh)(struct net_device *, u32 *, u8 *, u8 *);
    int (*set_rxfh)(struct net_device *, const u32 *, const u8 *, const u8);
    void (*get_channels)(struct net_device *, struct ethtool_channels *);
    int (*set_channels)(struct net_device *, struct ethtool_channels *);
    int (*get_dump_flag)(struct net_device *, struct ethtool_dump *);
    int (*get_dump_data)(struct net_device *, struct ethtool_dump *, void *);
    int (*set_dump)(struct net_device *, struct ethtool_dump *);
    int (*get_ts_info)(struct net_device *, struct ethtool_ts_info *);
    int (*get_module_info)(struct net_device *, struct ethtool_modinfo *);
    int (*get_module_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_eee)(struct net_device *, struct ethtool_eee *);
    int (*set_eee)(struct net_device *, struct ethtool_eee *);
    int (*get_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*set_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*get_link_ksettings)(struct net_device *, struct ethtool_link_ksettings *);
    int (*set_link_ksettings)(struct net_device *, const struct ethtool_link_ksettings *);
    int (*get_fecparam)(struct net_device *, struct ethtool_fecparam *);
    int (*set_fecparam)(struct net_device *, struct ethtool_fecparam *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ethtool_ops {
    int (*get_settings)(struct net_device *, struct ethtool_cmd *);
    int (*set_settings)(struct net_device *, struct ethtool_cmd *);
    void (*get_drvinfo)(struct net_device *, struct ethtool_drvinfo *);
    int (*get_regs_len)(struct net_device *);
    void (*get_regs)(struct net_device *, struct ethtool_regs *, void *);
    void (*get_wol)(struct net_device *, struct ethtool_wolinfo *);
    int (*set_wol)(struct net_device *, struct ethtool_wolinfo *);
    u32 (*get_msglevel)(struct net_device *);
    void (*set_msglevel)(struct net_device *, u32);
    int (*nway_reset)(struct net_device *);
    u32 (*get_link)(struct net_device *);
    int (*get_eeprom_len)(struct net_device *);
    int (*get_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_coalesce)(struct net_device *, struct ethtool_coalesce *);
    int (*set_coalesce)(struct net_device *, struct ethtool_coalesce *);
    void (*get_ringparam)(struct net_device *, struct ethtool_ringparam *);
    int (*set_ringparam)(struct net_device *, struct ethtool_ringparam *);
    void (*get_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    int (*set_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    void (*self_test)(struct net_device *, struct ethtool_test *, u64 *);
    void (*get_strings)(struct net_device *, u32, u8 *);
    int (*set_phys_id)(struct net_device *, enum ethtool_phys_id_state);
    void (*get_ethtool_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*begin)(struct net_device *);
    void (*complete)(struct net_device *);
    u32 (*get_priv_flags)(struct net_device *);
    int (*set_priv_flags)(struct net_device *, u32);
    int (*get_sset_count)(struct net_device *, int);
    int (*get_rxnfc)(struct net_device *, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct net_device *, struct ethtool_rxnfc *);
    int (*flash_device)(struct net_device *, struct ethtool_flash *);
    int (*reset)(struct net_device *, u32 *);
    u32 (*get_rxfh_key_size)(struct net_device *);
    u32 (*get_rxfh_indir_size)(struct net_device *);
    int (*get_rxfh)(struct net_device *, u32 *, u8 *, u8 *);
    int (*set_rxfh)(struct net_device *, const u32 *, const u8 *, const u8);
    int (*get_rxfh_context)(struct net_device *, u32 *, u8 *, u8 *, u32);
    int (*set_rxfh_context)(struct net_device *, const u32 *, const u8 *, const u8, u32 *, bool);
    void (*get_channels)(struct net_device *, struct ethtool_channels *);
    int (*set_channels)(struct net_device *, struct ethtool_channels *);
    int (*get_dump_flag)(struct net_device *, struct ethtool_dump *);
    int (*get_dump_data)(struct net_device *, struct ethtool_dump *, void *);
    int (*set_dump)(struct net_device *, struct ethtool_dump *);
    int (*get_ts_info)(struct net_device *, struct ethtool_ts_info *);
    int (*get_module_info)(struct net_device *, struct ethtool_modinfo *);
    int (*get_module_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_eee)(struct net_device *, struct ethtool_eee *);
    int (*set_eee)(struct net_device *, struct ethtool_eee *);
    int (*get_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*set_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*get_link_ksettings)(struct net_device *, struct ethtool_link_ksettings *);
    int (*set_link_ksettings)(struct net_device *, const struct ethtool_link_ksettings *);
    int (*get_fecparam)(struct net_device *, struct ethtool_fecparam *);
    int (*set_fecparam)(struct net_device *, struct ethtool_fecparam *);
    void (*get_ethtool_phy_stats)(struct net_device *, struct ethtool_stats *, u64 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ethtool_ops {
    void (*get_drvinfo)(struct net_device *, struct ethtool_drvinfo *);
    int (*get_regs_len)(struct net_device *);
    void (*get_regs)(struct net_device *, struct ethtool_regs *, void *);
    void (*get_wol)(struct net_device *, struct ethtool_wolinfo *);
    int (*set_wol)(struct net_device *, struct ethtool_wolinfo *);
    u32 (*get_msglevel)(struct net_device *);
    void (*set_msglevel)(struct net_device *, u32);
    int (*nway_reset)(struct net_device *);
    u32 (*get_link)(struct net_device *);
    int (*get_eeprom_len)(struct net_device *);
    int (*get_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_coalesce)(struct net_device *, struct ethtool_coalesce *);
    int (*set_coalesce)(struct net_device *, struct ethtool_coalesce *);
    void (*get_ringparam)(struct net_device *, struct ethtool_ringparam *);
    int (*set_ringparam)(struct net_device *, struct ethtool_ringparam *);
    void (*get_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    int (*set_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    void (*self_test)(struct net_device *, struct ethtool_test *, u64 *);
    void (*get_strings)(struct net_device *, u32, u8 *);
    int (*set_phys_id)(struct net_device *, enum ethtool_phys_id_state);
    void (*get_ethtool_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*begin)(struct net_device *);
    void (*complete)(struct net_device *);
    u32 (*get_priv_flags)(struct net_device *);
    int (*set_priv_flags)(struct net_device *, u32);
    int (*get_sset_count)(struct net_device *, int);
    int (*get_rxnfc)(struct net_device *, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct net_device *, struct ethtool_rxnfc *);
    int (*flash_device)(struct net_device *, struct ethtool_flash *);
    int (*reset)(struct net_device *, u32 *);
    u32 (*get_rxfh_key_size)(struct net_device *);
    u32 (*get_rxfh_indir_size)(struct net_device *);
    int (*get_rxfh)(struct net_device *, u32 *, u8 *, u8 *);
    int (*set_rxfh)(struct net_device *, const u32 *, const u8 *, const u8);
    int (*get_rxfh_context)(struct net_device *, u32 *, u8 *, u8 *, u32);
    int (*set_rxfh_context)(struct net_device *, const u32 *, const u8 *, const u8, u32 *, bool);
    void (*get_channels)(struct net_device *, struct ethtool_channels *);
    int (*set_channels)(struct net_device *, struct ethtool_channels *);
    int (*get_dump_flag)(struct net_device *, struct ethtool_dump *);
    int (*get_dump_data)(struct net_device *, struct ethtool_dump *, void *);
    int (*set_dump)(struct net_device *, struct ethtool_dump *);
    int (*get_ts_info)(struct net_device *, struct ethtool_ts_info *);
    int (*get_module_info)(struct net_device *, struct ethtool_modinfo *);
    int (*get_module_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_eee)(struct net_device *, struct ethtool_eee *);
    int (*set_eee)(struct net_device *, struct ethtool_eee *);
    int (*get_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*set_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*get_link_ksettings)(struct net_device *, struct ethtool_link_ksettings *);
    int (*set_link_ksettings)(struct net_device *, const struct ethtool_link_ksettings *);
    int (*get_fecparam)(struct net_device *, struct ethtool_fecparam *);
    int (*set_fecparam)(struct net_device *, struct ethtool_fecparam *);
    void (*get_ethtool_phy_stats)(struct net_device *, struct ethtool_stats *, u64 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ethtool_ops {
    void (*get_drvinfo)(struct net_device *, struct ethtool_drvinfo *);
    int (*get_regs_len)(struct net_device *);
    void (*get_regs)(struct net_device *, struct ethtool_regs *, void *);
    void (*get_wol)(struct net_device *, struct ethtool_wolinfo *);
    int (*set_wol)(struct net_device *, struct ethtool_wolinfo *);
    u32 (*get_msglevel)(struct net_device *);
    void (*set_msglevel)(struct net_device *, u32);
    int (*nway_reset)(struct net_device *);
    u32 (*get_link)(struct net_device *);
    int (*get_eeprom_len)(struct net_device *);
    int (*get_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_coalesce)(struct net_device *, struct ethtool_coalesce *);
    int (*set_coalesce)(struct net_device *, struct ethtool_coalesce *);
    void (*get_ringparam)(struct net_device *, struct ethtool_ringparam *);
    int (*set_ringparam)(struct net_device *, struct ethtool_ringparam *);
    void (*get_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    int (*set_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    void (*self_test)(struct net_device *, struct ethtool_test *, u64 *);
    void (*get_strings)(struct net_device *, u32, u8 *);
    int (*set_phys_id)(struct net_device *, enum ethtool_phys_id_state);
    void (*get_ethtool_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*begin)(struct net_device *);
    void (*complete)(struct net_device *);
    u32 (*get_priv_flags)(struct net_device *);
    int (*set_priv_flags)(struct net_device *, u32);
    int (*get_sset_count)(struct net_device *, int);
    int (*get_rxnfc)(struct net_device *, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct net_device *, struct ethtool_rxnfc *);
    int (*flash_device)(struct net_device *, struct ethtool_flash *);
    int (*reset)(struct net_device *, u32 *);
    u32 (*get_rxfh_key_size)(struct net_device *);
    u32 (*get_rxfh_indir_size)(struct net_device *);
    int (*get_rxfh)(struct net_device *, u32 *, u8 *, u8 *);
    int (*set_rxfh)(struct net_device *, const u32 *, const u8 *, const u8);
    int (*get_rxfh_context)(struct net_device *, u32 *, u8 *, u8 *, u32);
    int (*set_rxfh_context)(struct net_device *, const u32 *, const u8 *, const u8, u32 *, bool);
    void (*get_channels)(struct net_device *, struct ethtool_channels *);
    int (*set_channels)(struct net_device *, struct ethtool_channels *);
    int (*get_dump_flag)(struct net_device *, struct ethtool_dump *);
    int (*get_dump_data)(struct net_device *, struct ethtool_dump *, void *);
    int (*set_dump)(struct net_device *, struct ethtool_dump *);
    int (*get_ts_info)(struct net_device *, struct ethtool_ts_info *);
    int (*get_module_info)(struct net_device *, struct ethtool_modinfo *);
    int (*get_module_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_eee)(struct net_device *, struct ethtool_eee *);
    int (*set_eee)(struct net_device *, struct ethtool_eee *);
    int (*get_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*set_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*get_link_ksettings)(struct net_device *, struct ethtool_link_ksettings *);
    int (*set_link_ksettings)(struct net_device *, const struct ethtool_link_ksettings *);
    int (*get_fecparam)(struct net_device *, struct ethtool_fecparam *);
    int (*set_fecparam)(struct net_device *, struct ethtool_fecparam *);
    void (*get_ethtool_phy_stats)(struct net_device *, struct ethtool_stats *, u64 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ethtool_ops {
    void (*get_drvinfo)(struct net_device *, struct ethtool_drvinfo *);
    int (*get_regs_len)(struct net_device *);
    void (*get_regs)(struct net_device *, struct ethtool_regs *, void *);
    void (*get_wol)(struct net_device *, struct ethtool_wolinfo *);
    int (*set_wol)(struct net_device *, struct ethtool_wolinfo *);
    u32 (*get_msglevel)(struct net_device *);
    void (*set_msglevel)(struct net_device *, u32);
    int (*nway_reset)(struct net_device *);
    u32 (*get_link)(struct net_device *);
    int (*get_eeprom_len)(struct net_device *);
    int (*get_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_coalesce)(struct net_device *, struct ethtool_coalesce *);
    int (*set_coalesce)(struct net_device *, struct ethtool_coalesce *);
    void (*get_ringparam)(struct net_device *, struct ethtool_ringparam *);
    int (*set_ringparam)(struct net_device *, struct ethtool_ringparam *);
    void (*get_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    int (*set_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    void (*self_test)(struct net_device *, struct ethtool_test *, u64 *);
    void (*get_strings)(struct net_device *, u32, u8 *);
    int (*set_phys_id)(struct net_device *, enum ethtool_phys_id_state);
    void (*get_ethtool_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*begin)(struct net_device *);
    void (*complete)(struct net_device *);
    u32 (*get_priv_flags)(struct net_device *);
    int (*set_priv_flags)(struct net_device *, u32);
    int (*get_sset_count)(struct net_device *, int);
    int (*get_rxnfc)(struct net_device *, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct net_device *, struct ethtool_rxnfc *);
    int (*flash_device)(struct net_device *, struct ethtool_flash *);
    int (*reset)(struct net_device *, u32 *);
    u32 (*get_rxfh_key_size)(struct net_device *);
    u32 (*get_rxfh_indir_size)(struct net_device *);
    int (*get_rxfh)(struct net_device *, u32 *, u8 *, u8 *);
    int (*set_rxfh)(struct net_device *, const u32 *, const u8 *, const u8);
    int (*get_rxfh_context)(struct net_device *, u32 *, u8 *, u8 *, u32);
    int (*set_rxfh_context)(struct net_device *, const u32 *, const u8 *, const u8, u32 *, bool);
    void (*get_channels)(struct net_device *, struct ethtool_channels *);
    int (*set_channels)(struct net_device *, struct ethtool_channels *);
    int (*get_dump_flag)(struct net_device *, struct ethtool_dump *);
    int (*get_dump_data)(struct net_device *, struct ethtool_dump *, void *);
    int (*set_dump)(struct net_device *, struct ethtool_dump *);
    int (*get_ts_info)(struct net_device *, struct ethtool_ts_info *);
    int (*get_module_info)(struct net_device *, struct ethtool_modinfo *);
    int (*get_module_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_eee)(struct net_device *, struct ethtool_eee *);
    int (*set_eee)(struct net_device *, struct ethtool_eee *);
    int (*get_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*set_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*get_link_ksettings)(struct net_device *, struct ethtool_link_ksettings *);
    int (*set_link_ksettings)(struct net_device *, const struct ethtool_link_ksettings *);
    int (*get_fecparam)(struct net_device *, struct ethtool_fecparam *);
    int (*set_fecparam)(struct net_device *, struct ethtool_fecparam *);
    void (*get_ethtool_phy_stats)(struct net_device *, struct ethtool_stats *, u64 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ethtool_ops {
    u32 supported_coalesce_params;
    void (*get_drvinfo)(struct net_device *, struct ethtool_drvinfo *);
    int (*get_regs_len)(struct net_device *);
    void (*get_regs)(struct net_device *, struct ethtool_regs *, void *);
    void (*get_wol)(struct net_device *, struct ethtool_wolinfo *);
    int (*set_wol)(struct net_device *, struct ethtool_wolinfo *);
    u32 (*get_msglevel)(struct net_device *);
    void (*set_msglevel)(struct net_device *, u32);
    int (*nway_reset)(struct net_device *);
    u32 (*get_link)(struct net_device *);
    int (*get_eeprom_len)(struct net_device *);
    int (*get_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_coalesce)(struct net_device *, struct ethtool_coalesce *);
    int (*set_coalesce)(struct net_device *, struct ethtool_coalesce *);
    void (*get_ringparam)(struct net_device *, struct ethtool_ringparam *);
    int (*set_ringparam)(struct net_device *, struct ethtool_ringparam *);
    void (*get_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    int (*set_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    void (*self_test)(struct net_device *, struct ethtool_test *, u64 *);
    void (*get_strings)(struct net_device *, u32, u8 *);
    int (*set_phys_id)(struct net_device *, enum ethtool_phys_id_state);
    void (*get_ethtool_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*begin)(struct net_device *);
    void (*complete)(struct net_device *);
    u32 (*get_priv_flags)(struct net_device *);
    int (*set_priv_flags)(struct net_device *, u32);
    int (*get_sset_count)(struct net_device *, int);
    int (*get_rxnfc)(struct net_device *, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct net_device *, struct ethtool_rxnfc *);
    int (*flash_device)(struct net_device *, struct ethtool_flash *);
    int (*reset)(struct net_device *, u32 *);
    u32 (*get_rxfh_key_size)(struct net_device *);
    u32 (*get_rxfh_indir_size)(struct net_device *);
    int (*get_rxfh)(struct net_device *, u32 *, u8 *, u8 *);
    int (*set_rxfh)(struct net_device *, const u32 *, const u8 *, const u8);
    int (*get_rxfh_context)(struct net_device *, u32 *, u8 *, u8 *, u32);
    int (*set_rxfh_context)(struct net_device *, const u32 *, const u8 *, const u8, u32 *, bool);
    void (*get_channels)(struct net_device *, struct ethtool_channels *);
    int (*set_channels)(struct net_device *, struct ethtool_channels *);
    int (*get_dump_flag)(struct net_device *, struct ethtool_dump *);
    int (*get_dump_data)(struct net_device *, struct ethtool_dump *, void *);
    int (*set_dump)(struct net_device *, struct ethtool_dump *);
    int (*get_ts_info)(struct net_device *, struct ethtool_ts_info *);
    int (*get_module_info)(struct net_device *, struct ethtool_modinfo *);
    int (*get_module_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_eee)(struct net_device *, struct ethtool_eee *);
    int (*set_eee)(struct net_device *, struct ethtool_eee *);
    int (*get_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*set_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*get_link_ksettings)(struct net_device *, struct ethtool_link_ksettings *);
    int (*set_link_ksettings)(struct net_device *, const struct ethtool_link_ksettings *);
    int (*get_fecparam)(struct net_device *, struct ethtool_fecparam *);
    int (*set_fecparam)(struct net_device *, struct ethtool_fecparam *);
    void (*get_ethtool_phy_stats)(struct net_device *, struct ethtool_stats *, u64 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ethtool_ops {
    u32 supported_coalesce_params;
    void (*get_drvinfo)(struct net_device *, struct ethtool_drvinfo *);
    int (*get_regs_len)(struct net_device *);
    void (*get_regs)(struct net_device *, struct ethtool_regs *, void *);
    void (*get_wol)(struct net_device *, struct ethtool_wolinfo *);
    int (*set_wol)(struct net_device *, struct ethtool_wolinfo *);
    u32 (*get_msglevel)(struct net_device *);
    void (*set_msglevel)(struct net_device *, u32);
    int (*nway_reset)(struct net_device *);
    u32 (*get_link)(struct net_device *);
    int (*get_link_ext_state)(struct net_device *, struct ethtool_link_ext_state_info *);
    int (*get_eeprom_len)(struct net_device *);
    int (*get_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_coalesce)(struct net_device *, struct ethtool_coalesce *);
    int (*set_coalesce)(struct net_device *, struct ethtool_coalesce *);
    void (*get_ringparam)(struct net_device *, struct ethtool_ringparam *);
    int (*set_ringparam)(struct net_device *, struct ethtool_ringparam *);
    void (*get_pause_stats)(struct net_device *, struct ethtool_pause_stats *);
    void (*get_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    int (*set_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    void (*self_test)(struct net_device *, struct ethtool_test *, u64 *);
    void (*get_strings)(struct net_device *, u32, u8 *);
    int (*set_phys_id)(struct net_device *, enum ethtool_phys_id_state);
    void (*get_ethtool_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*begin)(struct net_device *);
    void (*complete)(struct net_device *);
    u32 (*get_priv_flags)(struct net_device *);
    int (*set_priv_flags)(struct net_device *, u32);
    int (*get_sset_count)(struct net_device *, int);
    int (*get_rxnfc)(struct net_device *, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct net_device *, struct ethtool_rxnfc *);
    int (*flash_device)(struct net_device *, struct ethtool_flash *);
    int (*reset)(struct net_device *, u32 *);
    u32 (*get_rxfh_key_size)(struct net_device *);
    u32 (*get_rxfh_indir_size)(struct net_device *);
    int (*get_rxfh)(struct net_device *, u32 *, u8 *, u8 *);
    int (*set_rxfh)(struct net_device *, const u32 *, const u8 *, const u8);
    int (*get_rxfh_context)(struct net_device *, u32 *, u8 *, u8 *, u32);
    int (*set_rxfh_context)(struct net_device *, const u32 *, const u8 *, const u8, u32 *, bool);
    void (*get_channels)(struct net_device *, struct ethtool_channels *);
    int (*set_channels)(struct net_device *, struct ethtool_channels *);
    int (*get_dump_flag)(struct net_device *, struct ethtool_dump *);
    int (*get_dump_data)(struct net_device *, struct ethtool_dump *, void *);
    int (*set_dump)(struct net_device *, struct ethtool_dump *);
    int (*get_ts_info)(struct net_device *, struct ethtool_ts_info *);
    int (*get_module_info)(struct net_device *, struct ethtool_modinfo *);
    int (*get_module_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_eee)(struct net_device *, struct ethtool_eee *);
    int (*set_eee)(struct net_device *, struct ethtool_eee *);
    int (*get_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*set_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*get_link_ksettings)(struct net_device *, struct ethtool_link_ksettings *);
    int (*set_link_ksettings)(struct net_device *, const struct ethtool_link_ksettings *);
    int (*get_fecparam)(struct net_device *, struct ethtool_fecparam *);
    int (*set_fecparam)(struct net_device *, struct ethtool_fecparam *);
    void (*get_ethtool_phy_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*get_phy_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_phy_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ethtool_ops {
    u32 cap_link_lanes_supported;
    u32 supported_coalesce_params;
    void (*get_drvinfo)(struct net_device *, struct ethtool_drvinfo *);
    int (*get_regs_len)(struct net_device *);
    void (*get_regs)(struct net_device *, struct ethtool_regs *, void *);
    void (*get_wol)(struct net_device *, struct ethtool_wolinfo *);
    int (*set_wol)(struct net_device *, struct ethtool_wolinfo *);
    u32 (*get_msglevel)(struct net_device *);
    void (*set_msglevel)(struct net_device *, u32);
    int (*nway_reset)(struct net_device *);
    u32 (*get_link)(struct net_device *);
    int (*get_link_ext_state)(struct net_device *, struct ethtool_link_ext_state_info *);
    int (*get_eeprom_len)(struct net_device *);
    int (*get_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_coalesce)(struct net_device *, struct ethtool_coalesce *);
    int (*set_coalesce)(struct net_device *, struct ethtool_coalesce *);
    void (*get_ringparam)(struct net_device *, struct ethtool_ringparam *);
    int (*set_ringparam)(struct net_device *, struct ethtool_ringparam *);
    void (*get_pause_stats)(struct net_device *, struct ethtool_pause_stats *);
    void (*get_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    int (*set_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    void (*self_test)(struct net_device *, struct ethtool_test *, u64 *);
    void (*get_strings)(struct net_device *, u32, u8 *);
    int (*set_phys_id)(struct net_device *, enum ethtool_phys_id_state);
    void (*get_ethtool_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*begin)(struct net_device *);
    void (*complete)(struct net_device *);
    u32 (*get_priv_flags)(struct net_device *);
    int (*set_priv_flags)(struct net_device *, u32);
    int (*get_sset_count)(struct net_device *, int);
    int (*get_rxnfc)(struct net_device *, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct net_device *, struct ethtool_rxnfc *);
    int (*flash_device)(struct net_device *, struct ethtool_flash *);
    int (*reset)(struct net_device *, u32 *);
    u32 (*get_rxfh_key_size)(struct net_device *);
    u32 (*get_rxfh_indir_size)(struct net_device *);
    int (*get_rxfh)(struct net_device *, u32 *, u8 *, u8 *);
    int (*set_rxfh)(struct net_device *, const u32 *, const u8 *, const u8);
    int (*get_rxfh_context)(struct net_device *, u32 *, u8 *, u8 *, u32);
    int (*set_rxfh_context)(struct net_device *, const u32 *, const u8 *, const u8, u32 *, bool);
    void (*get_channels)(struct net_device *, struct ethtool_channels *);
    int (*set_channels)(struct net_device *, struct ethtool_channels *);
    int (*get_dump_flag)(struct net_device *, struct ethtool_dump *);
    int (*get_dump_data)(struct net_device *, struct ethtool_dump *, void *);
    int (*set_dump)(struct net_device *, struct ethtool_dump *);
    int (*get_ts_info)(struct net_device *, struct ethtool_ts_info *);
    int (*get_module_info)(struct net_device *, struct ethtool_modinfo *);
    int (*get_module_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_eee)(struct net_device *, struct ethtool_eee *);
    int (*set_eee)(struct net_device *, struct ethtool_eee *);
    int (*get_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*set_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*get_link_ksettings)(struct net_device *, struct ethtool_link_ksettings *);
    int (*set_link_ksettings)(struct net_device *, const struct ethtool_link_ksettings *);
    void (*get_fec_stats)(struct net_device *, struct ethtool_fec_stats *);
    int (*get_fecparam)(struct net_device *, struct ethtool_fecparam *);
    int (*set_fecparam)(struct net_device *, struct ethtool_fecparam *);
    void (*get_ethtool_phy_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*get_phy_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_phy_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_module_eeprom_by_page)(struct net_device *, const struct ethtool_module_eeprom *, struct netlink_ext_ack *);
    void (*get_eth_phy_stats)(struct net_device *, struct ethtool_eth_phy_stats *);
    void (*get_eth_mac_stats)(struct net_device *, struct ethtool_eth_mac_stats *);
    void (*get_eth_ctrl_stats)(struct net_device *, struct ethtool_eth_ctrl_stats *);
    void (*get_rmon_stats)(struct net_device *, struct ethtool_rmon_stats *, const struct ethtool_rmon_hist_range **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ethtool_ops {
    u32 cap_link_lanes_supported;
    u32 supported_coalesce_params;
    void (*get_drvinfo)(struct net_device *, struct ethtool_drvinfo *);
    int (*get_regs_len)(struct net_device *);
    void (*get_regs)(struct net_device *, struct ethtool_regs *, void *);
    void (*get_wol)(struct net_device *, struct ethtool_wolinfo *);
    int (*set_wol)(struct net_device *, struct ethtool_wolinfo *);
    u32 (*get_msglevel)(struct net_device *);
    void (*set_msglevel)(struct net_device *, u32);
    int (*nway_reset)(struct net_device *);
    u32 (*get_link)(struct net_device *);
    int (*get_link_ext_state)(struct net_device *, struct ethtool_link_ext_state_info *);
    int (*get_eeprom_len)(struct net_device *);
    int (*get_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_coalesce)(struct net_device *, struct ethtool_coalesce *, struct kernel_ethtool_coalesce *, struct netlink_ext_ack *);
    int (*set_coalesce)(struct net_device *, struct ethtool_coalesce *, struct kernel_ethtool_coalesce *, struct netlink_ext_ack *);
    void (*get_ringparam)(struct net_device *, struct ethtool_ringparam *);
    int (*set_ringparam)(struct net_device *, struct ethtool_ringparam *);
    void (*get_pause_stats)(struct net_device *, struct ethtool_pause_stats *);
    void (*get_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    int (*set_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    void (*self_test)(struct net_device *, struct ethtool_test *, u64 *);
    void (*get_strings)(struct net_device *, u32, u8 *);
    int (*set_phys_id)(struct net_device *, enum ethtool_phys_id_state);
    void (*get_ethtool_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*begin)(struct net_device *);
    void (*complete)(struct net_device *);
    u32 (*get_priv_flags)(struct net_device *);
    int (*set_priv_flags)(struct net_device *, u32);
    int (*get_sset_count)(struct net_device *, int);
    int (*get_rxnfc)(struct net_device *, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct net_device *, struct ethtool_rxnfc *);
    int (*flash_device)(struct net_device *, struct ethtool_flash *);
    int (*reset)(struct net_device *, u32 *);
    u32 (*get_rxfh_key_size)(struct net_device *);
    u32 (*get_rxfh_indir_size)(struct net_device *);
    int (*get_rxfh)(struct net_device *, u32 *, u8 *, u8 *);
    int (*set_rxfh)(struct net_device *, const u32 *, const u8 *, const u8);
    int (*get_rxfh_context)(struct net_device *, u32 *, u8 *, u8 *, u32);
    int (*set_rxfh_context)(struct net_device *, const u32 *, const u8 *, const u8, u32 *, bool);
    void (*get_channels)(struct net_device *, struct ethtool_channels *);
    int (*set_channels)(struct net_device *, struct ethtool_channels *);
    int (*get_dump_flag)(struct net_device *, struct ethtool_dump *);
    int (*get_dump_data)(struct net_device *, struct ethtool_dump *, void *);
    int (*set_dump)(struct net_device *, struct ethtool_dump *);
    int (*get_ts_info)(struct net_device *, struct ethtool_ts_info *);
    int (*get_module_info)(struct net_device *, struct ethtool_modinfo *);
    int (*get_module_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_eee)(struct net_device *, struct ethtool_eee *);
    int (*set_eee)(struct net_device *, struct ethtool_eee *);
    int (*get_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*set_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*get_link_ksettings)(struct net_device *, struct ethtool_link_ksettings *);
    int (*set_link_ksettings)(struct net_device *, const struct ethtool_link_ksettings *);
    void (*get_fec_stats)(struct net_device *, struct ethtool_fec_stats *);
    int (*get_fecparam)(struct net_device *, struct ethtool_fecparam *);
    int (*set_fecparam)(struct net_device *, struct ethtool_fecparam *);
    void (*get_ethtool_phy_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*get_phy_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_phy_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_module_eeprom_by_page)(struct net_device *, const struct ethtool_module_eeprom *, struct netlink_ext_ack *);
    void (*get_eth_phy_stats)(struct net_device *, struct ethtool_eth_phy_stats *);
    void (*get_eth_mac_stats)(struct net_device *, struct ethtool_eth_mac_stats *);
    void (*get_eth_ctrl_stats)(struct net_device *, struct ethtool_eth_ctrl_stats *);
    void (*get_rmon_stats)(struct net_device *, struct ethtool_rmon_stats *, const struct ethtool_rmon_hist_range **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ethtool_ops {
    u32 cap_link_lanes_supported;
    u32 supported_coalesce_params;
    u32 supported_ring_params;
    void (*get_drvinfo)(struct net_device *, struct ethtool_drvinfo *);
    int (*get_regs_len)(struct net_device *);
    void (*get_regs)(struct net_device *, struct ethtool_regs *, void *);
    void (*get_wol)(struct net_device *, struct ethtool_wolinfo *);
    int (*set_wol)(struct net_device *, struct ethtool_wolinfo *);
    u32 (*get_msglevel)(struct net_device *);
    void (*set_msglevel)(struct net_device *, u32);
    int (*nway_reset)(struct net_device *);
    u32 (*get_link)(struct net_device *);
    int (*get_link_ext_state)(struct net_device *, struct ethtool_link_ext_state_info *);
    int (*get_eeprom_len)(struct net_device *);
    int (*get_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_coalesce)(struct net_device *, struct ethtool_coalesce *, struct kernel_ethtool_coalesce *, struct netlink_ext_ack *);
    int (*set_coalesce)(struct net_device *, struct ethtool_coalesce *, struct kernel_ethtool_coalesce *, struct netlink_ext_ack *);
    void (*get_ringparam)(struct net_device *, struct ethtool_ringparam *, struct kernel_ethtool_ringparam *, struct netlink_ext_ack *);
    int (*set_ringparam)(struct net_device *, struct ethtool_ringparam *, struct kernel_ethtool_ringparam *, struct netlink_ext_ack *);
    void (*get_pause_stats)(struct net_device *, struct ethtool_pause_stats *);
    void (*get_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    int (*set_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    void (*self_test)(struct net_device *, struct ethtool_test *, u64 *);
    void (*get_strings)(struct net_device *, u32, u8 *);
    int (*set_phys_id)(struct net_device *, enum ethtool_phys_id_state);
    void (*get_ethtool_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*begin)(struct net_device *);
    void (*complete)(struct net_device *);
    u32 (*get_priv_flags)(struct net_device *);
    int (*set_priv_flags)(struct net_device *, u32);
    int (*get_sset_count)(struct net_device *, int);
    int (*get_rxnfc)(struct net_device *, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct net_device *, struct ethtool_rxnfc *);
    int (*flash_device)(struct net_device *, struct ethtool_flash *);
    int (*reset)(struct net_device *, u32 *);
    u32 (*get_rxfh_key_size)(struct net_device *);
    u32 (*get_rxfh_indir_size)(struct net_device *);
    int (*get_rxfh)(struct net_device *, u32 *, u8 *, u8 *);
    int (*set_rxfh)(struct net_device *, const u32 *, const u8 *, const u8);
    int (*get_rxfh_context)(struct net_device *, u32 *, u8 *, u8 *, u32);
    int (*set_rxfh_context)(struct net_device *, const u32 *, const u8 *, const u8, u32 *, bool);
    void (*get_channels)(struct net_device *, struct ethtool_channels *);
    int (*set_channels)(struct net_device *, struct ethtool_channels *);
    int (*get_dump_flag)(struct net_device *, struct ethtool_dump *);
    int (*get_dump_data)(struct net_device *, struct ethtool_dump *, void *);
    int (*set_dump)(struct net_device *, struct ethtool_dump *);
    int (*get_ts_info)(struct net_device *, struct ethtool_ts_info *);
    int (*get_module_info)(struct net_device *, struct ethtool_modinfo *);
    int (*get_module_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_eee)(struct net_device *, struct ethtool_eee *);
    int (*set_eee)(struct net_device *, struct ethtool_eee *);
    int (*get_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*set_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*get_link_ksettings)(struct net_device *, struct ethtool_link_ksettings *);
    int (*set_link_ksettings)(struct net_device *, const struct ethtool_link_ksettings *);
    void (*get_fec_stats)(struct net_device *, struct ethtool_fec_stats *);
    int (*get_fecparam)(struct net_device *, struct ethtool_fecparam *);
    int (*set_fecparam)(struct net_device *, struct ethtool_fecparam *);
    void (*get_ethtool_phy_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*get_phy_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_phy_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_module_eeprom_by_page)(struct net_device *, const struct ethtool_module_eeprom *, struct netlink_ext_ack *);
    void (*get_eth_phy_stats)(struct net_device *, struct ethtool_eth_phy_stats *);
    void (*get_eth_mac_stats)(struct net_device *, struct ethtool_eth_mac_stats *);
    void (*get_eth_ctrl_stats)(struct net_device *, struct ethtool_eth_ctrl_stats *);
    void (*get_rmon_stats)(struct net_device *, struct ethtool_rmon_stats *, const struct ethtool_rmon_hist_range **);
    int (*get_module_power_mode)(struct net_device *, struct ethtool_module_power_mode_params *, struct netlink_ext_ack *);
    int (*set_module_power_mode)(struct net_device *, const struct ethtool_module_power_mode_params *, struct netlink_ext_ack *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ethtool_ops {
    u32 cap_link_lanes_supported;
    u32 supported_coalesce_params;
    u32 supported_ring_params;
    void (*get_drvinfo)(struct net_device *, struct ethtool_drvinfo *);
    int (*get_regs_len)(struct net_device *);
    void (*get_regs)(struct net_device *, struct ethtool_regs *, void *);
    void (*get_wol)(struct net_device *, struct ethtool_wolinfo *);
    int (*set_wol)(struct net_device *, struct ethtool_wolinfo *);
    u32 (*get_msglevel)(struct net_device *);
    void (*set_msglevel)(struct net_device *, u32);
    int (*nway_reset)(struct net_device *);
    u32 (*get_link)(struct net_device *);
    int (*get_link_ext_state)(struct net_device *, struct ethtool_link_ext_state_info *);
    void (*get_link_ext_stats)(struct net_device *, struct ethtool_link_ext_stats *);
    int (*get_eeprom_len)(struct net_device *);
    int (*get_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_coalesce)(struct net_device *, struct ethtool_coalesce *, struct kernel_ethtool_coalesce *, struct netlink_ext_ack *);
    int (*set_coalesce)(struct net_device *, struct ethtool_coalesce *, struct kernel_ethtool_coalesce *, struct netlink_ext_ack *);
    void (*get_ringparam)(struct net_device *, struct ethtool_ringparam *, struct kernel_ethtool_ringparam *, struct netlink_ext_ack *);
    int (*set_ringparam)(struct net_device *, struct ethtool_ringparam *, struct kernel_ethtool_ringparam *, struct netlink_ext_ack *);
    void (*get_pause_stats)(struct net_device *, struct ethtool_pause_stats *);
    void (*get_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    int (*set_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    void (*self_test)(struct net_device *, struct ethtool_test *, u64 *);
    void (*get_strings)(struct net_device *, u32, u8 *);
    int (*set_phys_id)(struct net_device *, enum ethtool_phys_id_state);
    void (*get_ethtool_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*begin)(struct net_device *);
    void (*complete)(struct net_device *);
    u32 (*get_priv_flags)(struct net_device *);
    int (*set_priv_flags)(struct net_device *, u32);
    int (*get_sset_count)(struct net_device *, int);
    int (*get_rxnfc)(struct net_device *, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct net_device *, struct ethtool_rxnfc *);
    int (*flash_device)(struct net_device *, struct ethtool_flash *);
    int (*reset)(struct net_device *, u32 *);
    u32 (*get_rxfh_key_size)(struct net_device *);
    u32 (*get_rxfh_indir_size)(struct net_device *);
    int (*get_rxfh)(struct net_device *, u32 *, u8 *, u8 *);
    int (*set_rxfh)(struct net_device *, const u32 *, const u8 *, const u8);
    int (*get_rxfh_context)(struct net_device *, u32 *, u8 *, u8 *, u32);
    int (*set_rxfh_context)(struct net_device *, const u32 *, const u8 *, const u8, u32 *, bool);
    void (*get_channels)(struct net_device *, struct ethtool_channels *);
    int (*set_channels)(struct net_device *, struct ethtool_channels *);
    int (*get_dump_flag)(struct net_device *, struct ethtool_dump *);
    int (*get_dump_data)(struct net_device *, struct ethtool_dump *, void *);
    int (*set_dump)(struct net_device *, struct ethtool_dump *);
    int (*get_ts_info)(struct net_device *, struct ethtool_ts_info *);
    int (*get_module_info)(struct net_device *, struct ethtool_modinfo *);
    int (*get_module_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_eee)(struct net_device *, struct ethtool_eee *);
    int (*set_eee)(struct net_device *, struct ethtool_eee *);
    int (*get_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*set_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*get_link_ksettings)(struct net_device *, struct ethtool_link_ksettings *);
    int (*set_link_ksettings)(struct net_device *, const struct ethtool_link_ksettings *);
    void (*get_fec_stats)(struct net_device *, struct ethtool_fec_stats *);
    int (*get_fecparam)(struct net_device *, struct ethtool_fecparam *);
    int (*set_fecparam)(struct net_device *, struct ethtool_fecparam *);
    void (*get_ethtool_phy_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*get_phy_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_phy_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_module_eeprom_by_page)(struct net_device *, const struct ethtool_module_eeprom *, struct netlink_ext_ack *);
    void (*get_eth_phy_stats)(struct net_device *, struct ethtool_eth_phy_stats *);
    void (*get_eth_mac_stats)(struct net_device *, struct ethtool_eth_mac_stats *);
    void (*get_eth_ctrl_stats)(struct net_device *, struct ethtool_eth_ctrl_stats *);
    void (*get_rmon_stats)(struct net_device *, struct ethtool_rmon_stats *, const struct ethtool_rmon_hist_range **);
    int (*get_module_power_mode)(struct net_device *, struct ethtool_module_power_mode_params *, struct netlink_ext_ack *);
    int (*set_module_power_mode)(struct net_device *, const struct ethtool_module_power_mode_params *, struct netlink_ext_ack *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ethtool_ops {
    u32 cap_link_lanes_supported;
    u32 supported_coalesce_params;
    u32 supported_ring_params;
    void (*get_drvinfo)(struct net_device *, struct ethtool_drvinfo *);
    int (*get_regs_len)(struct net_device *);
    void (*get_regs)(struct net_device *, struct ethtool_regs *, void *);
    void (*get_wol)(struct net_device *, struct ethtool_wolinfo *);
    int (*set_wol)(struct net_device *, struct ethtool_wolinfo *);
    u32 (*get_msglevel)(struct net_device *);
    void (*set_msglevel)(struct net_device *, u32);
    int (*nway_reset)(struct net_device *);
    u32 (*get_link)(struct net_device *);
    int (*get_link_ext_state)(struct net_device *, struct ethtool_link_ext_state_info *);
    void (*get_link_ext_stats)(struct net_device *, struct ethtool_link_ext_stats *);
    int (*get_eeprom_len)(struct net_device *);
    int (*get_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_coalesce)(struct net_device *, struct ethtool_coalesce *, struct kernel_ethtool_coalesce *, struct netlink_ext_ack *);
    int (*set_coalesce)(struct net_device *, struct ethtool_coalesce *, struct kernel_ethtool_coalesce *, struct netlink_ext_ack *);
    void (*get_ringparam)(struct net_device *, struct ethtool_ringparam *, struct kernel_ethtool_ringparam *, struct netlink_ext_ack *);
    int (*set_ringparam)(struct net_device *, struct ethtool_ringparam *, struct kernel_ethtool_ringparam *, struct netlink_ext_ack *);
    void (*get_pause_stats)(struct net_device *, struct ethtool_pause_stats *);
    void (*get_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    int (*set_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    void (*self_test)(struct net_device *, struct ethtool_test *, u64 *);
    void (*get_strings)(struct net_device *, u32, u8 *);
    int (*set_phys_id)(struct net_device *, enum ethtool_phys_id_state);
    void (*get_ethtool_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*begin)(struct net_device *);
    void (*complete)(struct net_device *);
    u32 (*get_priv_flags)(struct net_device *);
    int (*set_priv_flags)(struct net_device *, u32);
    int (*get_sset_count)(struct net_device *, int);
    int (*get_rxnfc)(struct net_device *, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct net_device *, struct ethtool_rxnfc *);
    int (*flash_device)(struct net_device *, struct ethtool_flash *);
    int (*reset)(struct net_device *, u32 *);
    u32 (*get_rxfh_key_size)(struct net_device *);
    u32 (*get_rxfh_indir_size)(struct net_device *);
    int (*get_rxfh)(struct net_device *, u32 *, u8 *, u8 *);
    int (*set_rxfh)(struct net_device *, const u32 *, const u8 *, const u8);
    int (*get_rxfh_context)(struct net_device *, u32 *, u8 *, u8 *, u32);
    int (*set_rxfh_context)(struct net_device *, const u32 *, const u8 *, const u8, u32 *, bool);
    void (*get_channels)(struct net_device *, struct ethtool_channels *);
    int (*set_channels)(struct net_device *, struct ethtool_channels *);
    int (*get_dump_flag)(struct net_device *, struct ethtool_dump *);
    int (*get_dump_data)(struct net_device *, struct ethtool_dump *, void *);
    int (*set_dump)(struct net_device *, struct ethtool_dump *);
    int (*get_ts_info)(struct net_device *, struct ethtool_ts_info *);
    int (*get_module_info)(struct net_device *, struct ethtool_modinfo *);
    int (*get_module_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_eee)(struct net_device *, struct ethtool_eee *);
    int (*set_eee)(struct net_device *, struct ethtool_eee *);
    int (*get_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*set_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*get_link_ksettings)(struct net_device *, struct ethtool_link_ksettings *);
    int (*set_link_ksettings)(struct net_device *, const struct ethtool_link_ksettings *);
    void (*get_fec_stats)(struct net_device *, struct ethtool_fec_stats *);
    int (*get_fecparam)(struct net_device *, struct ethtool_fecparam *);
    int (*set_fecparam)(struct net_device *, struct ethtool_fecparam *);
    void (*get_ethtool_phy_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*get_phy_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_phy_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_module_eeprom_by_page)(struct net_device *, const struct ethtool_module_eeprom *, struct netlink_ext_ack *);
    void (*get_eth_phy_stats)(struct net_device *, struct ethtool_eth_phy_stats *);
    void (*get_eth_mac_stats)(struct net_device *, struct ethtool_eth_mac_stats *);
    void (*get_eth_ctrl_stats)(struct net_device *, struct ethtool_eth_ctrl_stats *);
    void (*get_rmon_stats)(struct net_device *, struct ethtool_rmon_stats *, const struct ethtool_rmon_hist_range **);
    int (*get_module_power_mode)(struct net_device *, struct ethtool_module_power_mode_params *, struct netlink_ext_ack *);
    int (*set_module_power_mode)(struct net_device *, const struct ethtool_module_power_mode_params *, struct netlink_ext_ack *);
    int (*get_mm)(struct net_device *, struct ethtool_mm_state *);
    int (*set_mm)(struct net_device *, struct ethtool_mm_cfg *, struct netlink_ext_ack *);
    void (*get_mm_stats)(struct net_device *, struct ethtool_mm_stats *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ethtool_ops {
    u32 cap_link_lanes_supported;
    u32 cap_rss_ctx_supported;
    u32 cap_rss_sym_xor_supported;
    u32 supported_coalesce_params;
    u32 supported_ring_params;
    void (*get_drvinfo)(struct net_device *, struct ethtool_drvinfo *);
    int (*get_regs_len)(struct net_device *);
    void (*get_regs)(struct net_device *, struct ethtool_regs *, void *);
    void (*get_wol)(struct net_device *, struct ethtool_wolinfo *);
    int (*set_wol)(struct net_device *, struct ethtool_wolinfo *);
    u32 (*get_msglevel)(struct net_device *);
    void (*set_msglevel)(struct net_device *, u32);
    int (*nway_reset)(struct net_device *);
    u32 (*get_link)(struct net_device *);
    int (*get_link_ext_state)(struct net_device *, struct ethtool_link_ext_state_info *);
    void (*get_link_ext_stats)(struct net_device *, struct ethtool_link_ext_stats *);
    int (*get_eeprom_len)(struct net_device *);
    int (*get_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_coalesce)(struct net_device *, struct ethtool_coalesce *, struct kernel_ethtool_coalesce *, struct netlink_ext_ack *);
    int (*set_coalesce)(struct net_device *, struct ethtool_coalesce *, struct kernel_ethtool_coalesce *, struct netlink_ext_ack *);
    void (*get_ringparam)(struct net_device *, struct ethtool_ringparam *, struct kernel_ethtool_ringparam *, struct netlink_ext_ack *);
    int (*set_ringparam)(struct net_device *, struct ethtool_ringparam *, struct kernel_ethtool_ringparam *, struct netlink_ext_ack *);
    void (*get_pause_stats)(struct net_device *, struct ethtool_pause_stats *);
    void (*get_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    int (*set_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    void (*self_test)(struct net_device *, struct ethtool_test *, u64 *);
    void (*get_strings)(struct net_device *, u32, u8 *);
    int (*set_phys_id)(struct net_device *, enum ethtool_phys_id_state);
    void (*get_ethtool_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*begin)(struct net_device *);
    void (*complete)(struct net_device *);
    u32 (*get_priv_flags)(struct net_device *);
    int (*set_priv_flags)(struct net_device *, u32);
    int (*get_sset_count)(struct net_device *, int);
    int (*get_rxnfc)(struct net_device *, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct net_device *, struct ethtool_rxnfc *);
    int (*flash_device)(struct net_device *, struct ethtool_flash *);
    int (*reset)(struct net_device *, u32 *);
    u32 (*get_rxfh_key_size)(struct net_device *);
    u32 (*get_rxfh_indir_size)(struct net_device *);
    int (*get_rxfh)(struct net_device *, struct ethtool_rxfh_param *);
    int (*set_rxfh)(struct net_device *, struct ethtool_rxfh_param *, struct netlink_ext_ack *);
    void (*get_channels)(struct net_device *, struct ethtool_channels *);
    int (*set_channels)(struct net_device *, struct ethtool_channels *);
    int (*get_dump_flag)(struct net_device *, struct ethtool_dump *);
    int (*get_dump_data)(struct net_device *, struct ethtool_dump *, void *);
    int (*set_dump)(struct net_device *, struct ethtool_dump *);
    int (*get_ts_info)(struct net_device *, struct ethtool_ts_info *);
    int (*get_module_info)(struct net_device *, struct ethtool_modinfo *);
    int (*get_module_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_eee)(struct net_device *, struct ethtool_eee *);
    int (*set_eee)(struct net_device *, struct ethtool_eee *);
    int (*get_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*set_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*get_link_ksettings)(struct net_device *, struct ethtool_link_ksettings *);
    int (*set_link_ksettings)(struct net_device *, const struct ethtool_link_ksettings *);
    void (*get_fec_stats)(struct net_device *, struct ethtool_fec_stats *);
    int (*get_fecparam)(struct net_device *, struct ethtool_fecparam *);
    int (*set_fecparam)(struct net_device *, struct ethtool_fecparam *);
    void (*get_ethtool_phy_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*get_phy_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_phy_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_module_eeprom_by_page)(struct net_device *, const struct ethtool_module_eeprom *, struct netlink_ext_ack *);
    void (*get_eth_phy_stats)(struct net_device *, struct ethtool_eth_phy_stats *);
    void (*get_eth_mac_stats)(struct net_device *, struct ethtool_eth_mac_stats *);
    void (*get_eth_ctrl_stats)(struct net_device *, struct ethtool_eth_ctrl_stats *);
    void (*get_rmon_stats)(struct net_device *, struct ethtool_rmon_stats *, const struct ethtool_rmon_hist_range **);
    int (*get_module_power_mode)(struct net_device *, struct ethtool_module_power_mode_params *, struct netlink_ext_ack *);
    int (*set_module_power_mode)(struct net_device *, const struct ethtool_module_power_mode_params *, struct netlink_ext_ack *);
    int (*get_mm)(struct net_device *, struct ethtool_mm_state *);
    int (*set_mm)(struct net_device *, struct ethtool_mm_cfg *, struct netlink_ext_ack *);
    void (*get_mm_stats)(struct net_device *, struct ethtool_mm_stats *);
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
struct ethtool_ops {
    void (*get_drvinfo)(struct net_device *, struct ethtool_drvinfo *);
    int (*get_regs_len)(struct net_device *);
    void (*get_regs)(struct net_device *, struct ethtool_regs *, void *);
    void (*get_wol)(struct net_device *, struct ethtool_wolinfo *);
    int (*set_wol)(struct net_device *, struct ethtool_wolinfo *);
    u32 (*get_msglevel)(struct net_device *);
    void (*set_msglevel)(struct net_device *, u32);
    int (*nway_reset)(struct net_device *);
    u32 (*get_link)(struct net_device *);
    int (*get_eeprom_len)(struct net_device *);
    int (*get_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_coalesce)(struct net_device *, struct ethtool_coalesce *);
    int (*set_coalesce)(struct net_device *, struct ethtool_coalesce *);
    void (*get_ringparam)(struct net_device *, struct ethtool_ringparam *);
    int (*set_ringparam)(struct net_device *, struct ethtool_ringparam *);
    void (*get_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    int (*set_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    void (*self_test)(struct net_device *, struct ethtool_test *, u64 *);
    void (*get_strings)(struct net_device *, u32, u8 *);
    int (*set_phys_id)(struct net_device *, enum ethtool_phys_id_state);
    void (*get_ethtool_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*begin)(struct net_device *);
    void (*complete)(struct net_device *);
    u32 (*get_priv_flags)(struct net_device *);
    int (*set_priv_flags)(struct net_device *, u32);
    int (*get_sset_count)(struct net_device *, int);
    int (*get_rxnfc)(struct net_device *, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct net_device *, struct ethtool_rxnfc *);
    int (*flash_device)(struct net_device *, struct ethtool_flash *);
    int (*reset)(struct net_device *, u32 *);
    u32 (*get_rxfh_key_size)(struct net_device *);
    u32 (*get_rxfh_indir_size)(struct net_device *);
    int (*get_rxfh)(struct net_device *, u32 *, u8 *, u8 *);
    int (*set_rxfh)(struct net_device *, const u32 *, const u8 *, const u8);
    int (*get_rxfh_context)(struct net_device *, u32 *, u8 *, u8 *, u32);
    int (*set_rxfh_context)(struct net_device *, const u32 *, const u8 *, const u8, u32 *, bool);
    void (*get_channels)(struct net_device *, struct ethtool_channels *);
    int (*set_channels)(struct net_device *, struct ethtool_channels *);
    int (*get_dump_flag)(struct net_device *, struct ethtool_dump *);
    int (*get_dump_data)(struct net_device *, struct ethtool_dump *, void *);
    int (*set_dump)(struct net_device *, struct ethtool_dump *);
    int (*get_ts_info)(struct net_device *, struct ethtool_ts_info *);
    int (*get_module_info)(struct net_device *, struct ethtool_modinfo *);
    int (*get_module_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_eee)(struct net_device *, struct ethtool_eee *);
    int (*set_eee)(struct net_device *, struct ethtool_eee *);
    int (*get_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*set_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*get_link_ksettings)(struct net_device *, struct ethtool_link_ksettings *);
    int (*set_link_ksettings)(struct net_device *, const struct ethtool_link_ksettings *);
    int (*get_fecparam)(struct net_device *, struct ethtool_fecparam *);
    int (*set_fecparam)(struct net_device *, struct ethtool_fecparam *);
    void (*get_ethtool_phy_stats)(struct net_device *, struct ethtool_stats *, u64 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ethtool_ops {
    void (*get_drvinfo)(struct net_device *, struct ethtool_drvinfo *);
    int (*get_regs_len)(struct net_device *);
    void (*get_regs)(struct net_device *, struct ethtool_regs *, void *);
    void (*get_wol)(struct net_device *, struct ethtool_wolinfo *);
    int (*set_wol)(struct net_device *, struct ethtool_wolinfo *);
    u32 (*get_msglevel)(struct net_device *);
    void (*set_msglevel)(struct net_device *, u32);
    int (*nway_reset)(struct net_device *);
    u32 (*get_link)(struct net_device *);
    int (*get_eeprom_len)(struct net_device *);
    int (*get_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_coalesce)(struct net_device *, struct ethtool_coalesce *);
    int (*set_coalesce)(struct net_device *, struct ethtool_coalesce *);
    void (*get_ringparam)(struct net_device *, struct ethtool_ringparam *);
    int (*set_ringparam)(struct net_device *, struct ethtool_ringparam *);
    void (*get_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    int (*set_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    void (*self_test)(struct net_device *, struct ethtool_test *, u64 *);
    void (*get_strings)(struct net_device *, u32, u8 *);
    int (*set_phys_id)(struct net_device *, enum ethtool_phys_id_state);
    void (*get_ethtool_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*begin)(struct net_device *);
    void (*complete)(struct net_device *);
    u32 (*get_priv_flags)(struct net_device *);
    int (*set_priv_flags)(struct net_device *, u32);
    int (*get_sset_count)(struct net_device *, int);
    int (*get_rxnfc)(struct net_device *, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct net_device *, struct ethtool_rxnfc *);
    int (*flash_device)(struct net_device *, struct ethtool_flash *);
    int (*reset)(struct net_device *, u32 *);
    u32 (*get_rxfh_key_size)(struct net_device *);
    u32 (*get_rxfh_indir_size)(struct net_device *);
    int (*get_rxfh)(struct net_device *, u32 *, u8 *, u8 *);
    int (*set_rxfh)(struct net_device *, const u32 *, const u8 *, const u8);
    int (*get_rxfh_context)(struct net_device *, u32 *, u8 *, u8 *, u32);
    int (*set_rxfh_context)(struct net_device *, const u32 *, const u8 *, const u8, u32 *, bool);
    void (*get_channels)(struct net_device *, struct ethtool_channels *);
    int (*set_channels)(struct net_device *, struct ethtool_channels *);
    int (*get_dump_flag)(struct net_device *, struct ethtool_dump *);
    int (*get_dump_data)(struct net_device *, struct ethtool_dump *, void *);
    int (*set_dump)(struct net_device *, struct ethtool_dump *);
    int (*get_ts_info)(struct net_device *, struct ethtool_ts_info *);
    int (*get_module_info)(struct net_device *, struct ethtool_modinfo *);
    int (*get_module_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_eee)(struct net_device *, struct ethtool_eee *);
    int (*set_eee)(struct net_device *, struct ethtool_eee *);
    int (*get_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*set_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*get_link_ksettings)(struct net_device *, struct ethtool_link_ksettings *);
    int (*set_link_ksettings)(struct net_device *, const struct ethtool_link_ksettings *);
    int (*get_fecparam)(struct net_device *, struct ethtool_fecparam *);
    int (*set_fecparam)(struct net_device *, struct ethtool_fecparam *);
    void (*get_ethtool_phy_stats)(struct net_device *, struct ethtool_stats *, u64 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ethtool_ops {
    void (*get_drvinfo)(struct net_device *, struct ethtool_drvinfo *);
    int (*get_regs_len)(struct net_device *);
    void (*get_regs)(struct net_device *, struct ethtool_regs *, void *);
    void (*get_wol)(struct net_device *, struct ethtool_wolinfo *);
    int (*set_wol)(struct net_device *, struct ethtool_wolinfo *);
    u32 (*get_msglevel)(struct net_device *);
    void (*set_msglevel)(struct net_device *, u32);
    int (*nway_reset)(struct net_device *);
    u32 (*get_link)(struct net_device *);
    int (*get_eeprom_len)(struct net_device *);
    int (*get_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_coalesce)(struct net_device *, struct ethtool_coalesce *);
    int (*set_coalesce)(struct net_device *, struct ethtool_coalesce *);
    void (*get_ringparam)(struct net_device *, struct ethtool_ringparam *);
    int (*set_ringparam)(struct net_device *, struct ethtool_ringparam *);
    void (*get_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    int (*set_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    void (*self_test)(struct net_device *, struct ethtool_test *, u64 *);
    void (*get_strings)(struct net_device *, u32, u8 *);
    int (*set_phys_id)(struct net_device *, enum ethtool_phys_id_state);
    void (*get_ethtool_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*begin)(struct net_device *);
    void (*complete)(struct net_device *);
    u32 (*get_priv_flags)(struct net_device *);
    int (*set_priv_flags)(struct net_device *, u32);
    int (*get_sset_count)(struct net_device *, int);
    int (*get_rxnfc)(struct net_device *, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct net_device *, struct ethtool_rxnfc *);
    int (*flash_device)(struct net_device *, struct ethtool_flash *);
    int (*reset)(struct net_device *, u32 *);
    u32 (*get_rxfh_key_size)(struct net_device *);
    u32 (*get_rxfh_indir_size)(struct net_device *);
    int (*get_rxfh)(struct net_device *, u32 *, u8 *, u8 *);
    int (*set_rxfh)(struct net_device *, const u32 *, const u8 *, const u8);
    int (*get_rxfh_context)(struct net_device *, u32 *, u8 *, u8 *, u32);
    int (*set_rxfh_context)(struct net_device *, const u32 *, const u8 *, const u8, u32 *, bool);
    void (*get_channels)(struct net_device *, struct ethtool_channels *);
    int (*set_channels)(struct net_device *, struct ethtool_channels *);
    int (*get_dump_flag)(struct net_device *, struct ethtool_dump *);
    int (*get_dump_data)(struct net_device *, struct ethtool_dump *, void *);
    int (*set_dump)(struct net_device *, struct ethtool_dump *);
    int (*get_ts_info)(struct net_device *, struct ethtool_ts_info *);
    int (*get_module_info)(struct net_device *, struct ethtool_modinfo *);
    int (*get_module_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_eee)(struct net_device *, struct ethtool_eee *);
    int (*set_eee)(struct net_device *, struct ethtool_eee *);
    int (*get_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*set_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*get_link_ksettings)(struct net_device *, struct ethtool_link_ksettings *);
    int (*set_link_ksettings)(struct net_device *, const struct ethtool_link_ksettings *);
    int (*get_fecparam)(struct net_device *, struct ethtool_fecparam *);
    int (*set_fecparam)(struct net_device *, struct ethtool_fecparam *);
    void (*get_ethtool_phy_stats)(struct net_device *, struct ethtool_stats *, u64 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ethtool_ops {
    void (*get_drvinfo)(struct net_device *, struct ethtool_drvinfo *);
    int (*get_regs_len)(struct net_device *);
    void (*get_regs)(struct net_device *, struct ethtool_regs *, void *);
    void (*get_wol)(struct net_device *, struct ethtool_wolinfo *);
    int (*set_wol)(struct net_device *, struct ethtool_wolinfo *);
    u32 (*get_msglevel)(struct net_device *);
    void (*set_msglevel)(struct net_device *, u32);
    int (*nway_reset)(struct net_device *);
    u32 (*get_link)(struct net_device *);
    int (*get_eeprom_len)(struct net_device *);
    int (*get_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_coalesce)(struct net_device *, struct ethtool_coalesce *);
    int (*set_coalesce)(struct net_device *, struct ethtool_coalesce *);
    void (*get_ringparam)(struct net_device *, struct ethtool_ringparam *);
    int (*set_ringparam)(struct net_device *, struct ethtool_ringparam *);
    void (*get_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    int (*set_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    void (*self_test)(struct net_device *, struct ethtool_test *, u64 *);
    void (*get_strings)(struct net_device *, u32, u8 *);
    int (*set_phys_id)(struct net_device *, enum ethtool_phys_id_state);
    void (*get_ethtool_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*begin)(struct net_device *);
    void (*complete)(struct net_device *);
    u32 (*get_priv_flags)(struct net_device *);
    int (*set_priv_flags)(struct net_device *, u32);
    int (*get_sset_count)(struct net_device *, int);
    int (*get_rxnfc)(struct net_device *, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct net_device *, struct ethtool_rxnfc *);
    int (*flash_device)(struct net_device *, struct ethtool_flash *);
    int (*reset)(struct net_device *, u32 *);
    u32 (*get_rxfh_key_size)(struct net_device *);
    u32 (*get_rxfh_indir_size)(struct net_device *);
    int (*get_rxfh)(struct net_device *, u32 *, u8 *, u8 *);
    int (*set_rxfh)(struct net_device *, const u32 *, const u8 *, const u8);
    int (*get_rxfh_context)(struct net_device *, u32 *, u8 *, u8 *, u32);
    int (*set_rxfh_context)(struct net_device *, const u32 *, const u8 *, const u8, u32 *, bool);
    void (*get_channels)(struct net_device *, struct ethtool_channels *);
    int (*set_channels)(struct net_device *, struct ethtool_channels *);
    int (*get_dump_flag)(struct net_device *, struct ethtool_dump *);
    int (*get_dump_data)(struct net_device *, struct ethtool_dump *, void *);
    int (*set_dump)(struct net_device *, struct ethtool_dump *);
    int (*get_ts_info)(struct net_device *, struct ethtool_ts_info *);
    int (*get_module_info)(struct net_device *, struct ethtool_modinfo *);
    int (*get_module_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_eee)(struct net_device *, struct ethtool_eee *);
    int (*set_eee)(struct net_device *, struct ethtool_eee *);
    int (*get_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*set_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*get_link_ksettings)(struct net_device *, struct ethtool_link_ksettings *);
    int (*set_link_ksettings)(struct net_device *, const struct ethtool_link_ksettings *);
    int (*get_fecparam)(struct net_device *, struct ethtool_fecparam *);
    int (*set_fecparam)(struct net_device *, struct ethtool_fecparam *);
    void (*get_ethtool_phy_stats)(struct net_device *, struct ethtool_stats *, u64 *);
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
struct ethtool_ops {
    void (*get_drvinfo)(struct net_device *, struct ethtool_drvinfo *);
    int (*get_regs_len)(struct net_device *);
    void (*get_regs)(struct net_device *, struct ethtool_regs *, void *);
    void (*get_wol)(struct net_device *, struct ethtool_wolinfo *);
    int (*set_wol)(struct net_device *, struct ethtool_wolinfo *);
    u32 (*get_msglevel)(struct net_device *);
    void (*set_msglevel)(struct net_device *, u32);
    int (*nway_reset)(struct net_device *);
    u32 (*get_link)(struct net_device *);
    int (*get_eeprom_len)(struct net_device *);
    int (*get_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_coalesce)(struct net_device *, struct ethtool_coalesce *);
    int (*set_coalesce)(struct net_device *, struct ethtool_coalesce *);
    void (*get_ringparam)(struct net_device *, struct ethtool_ringparam *);
    int (*set_ringparam)(struct net_device *, struct ethtool_ringparam *);
    void (*get_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    int (*set_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    void (*self_test)(struct net_device *, struct ethtool_test *, u64 *);
    void (*get_strings)(struct net_device *, u32, u8 *);
    int (*set_phys_id)(struct net_device *, enum ethtool_phys_id_state);
    void (*get_ethtool_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*begin)(struct net_device *);
    void (*complete)(struct net_device *);
    u32 (*get_priv_flags)(struct net_device *);
    int (*set_priv_flags)(struct net_device *, u32);
    int (*get_sset_count)(struct net_device *, int);
    int (*get_rxnfc)(struct net_device *, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct net_device *, struct ethtool_rxnfc *);
    int (*flash_device)(struct net_device *, struct ethtool_flash *);
    int (*reset)(struct net_device *, u32 *);
    u32 (*get_rxfh_key_size)(struct net_device *);
    u32 (*get_rxfh_indir_size)(struct net_device *);
    int (*get_rxfh)(struct net_device *, u32 *, u8 *, u8 *);
    int (*set_rxfh)(struct net_device *, const u32 *, const u8 *, const u8);
    int (*get_rxfh_context)(struct net_device *, u32 *, u8 *, u8 *, u32);
    int (*set_rxfh_context)(struct net_device *, const u32 *, const u8 *, const u8, u32 *, bool);
    void (*get_channels)(struct net_device *, struct ethtool_channels *);
    int (*set_channels)(struct net_device *, struct ethtool_channels *);
    int (*get_dump_flag)(struct net_device *, struct ethtool_dump *);
    int (*get_dump_data)(struct net_device *, struct ethtool_dump *, void *);
    int (*set_dump)(struct net_device *, struct ethtool_dump *);
    int (*get_ts_info)(struct net_device *, struct ethtool_ts_info *);
    int (*get_module_info)(struct net_device *, struct ethtool_modinfo *);
    int (*get_module_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_eee)(struct net_device *, struct ethtool_eee *);
    int (*set_eee)(struct net_device *, struct ethtool_eee *);
    int (*get_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*set_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*get_link_ksettings)(struct net_device *, struct ethtool_link_ksettings *);
    int (*set_link_ksettings)(struct net_device *, const struct ethtool_link_ksettings *);
    int (*get_fecparam)(struct net_device *, struct ethtool_fecparam *);
    int (*set_fecparam)(struct net_device *, struct ethtool_fecparam *);
    void (*get_ethtool_phy_stats)(struct net_device *, struct ethtool_stats *, u64 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ethtool_ops {
    void (*get_drvinfo)(struct net_device *, struct ethtool_drvinfo *);
    int (*get_regs_len)(struct net_device *);
    void (*get_regs)(struct net_device *, struct ethtool_regs *, void *);
    void (*get_wol)(struct net_device *, struct ethtool_wolinfo *);
    int (*set_wol)(struct net_device *, struct ethtool_wolinfo *);
    u32 (*get_msglevel)(struct net_device *);
    void (*set_msglevel)(struct net_device *, u32);
    int (*nway_reset)(struct net_device *);
    u32 (*get_link)(struct net_device *);
    int (*get_eeprom_len)(struct net_device *);
    int (*get_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_coalesce)(struct net_device *, struct ethtool_coalesce *);
    int (*set_coalesce)(struct net_device *, struct ethtool_coalesce *);
    void (*get_ringparam)(struct net_device *, struct ethtool_ringparam *);
    int (*set_ringparam)(struct net_device *, struct ethtool_ringparam *);
    void (*get_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    int (*set_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    void (*self_test)(struct net_device *, struct ethtool_test *, u64 *);
    void (*get_strings)(struct net_device *, u32, u8 *);
    int (*set_phys_id)(struct net_device *, enum ethtool_phys_id_state);
    void (*get_ethtool_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*begin)(struct net_device *);
    void (*complete)(struct net_device *);
    u32 (*get_priv_flags)(struct net_device *);
    int (*set_priv_flags)(struct net_device *, u32);
    int (*get_sset_count)(struct net_device *, int);
    int (*get_rxnfc)(struct net_device *, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct net_device *, struct ethtool_rxnfc *);
    int (*flash_device)(struct net_device *, struct ethtool_flash *);
    int (*reset)(struct net_device *, u32 *);
    u32 (*get_rxfh_key_size)(struct net_device *);
    u32 (*get_rxfh_indir_size)(struct net_device *);
    int (*get_rxfh)(struct net_device *, u32 *, u8 *, u8 *);
    int (*set_rxfh)(struct net_device *, const u32 *, const u8 *, const u8);
    int (*get_rxfh_context)(struct net_device *, u32 *, u8 *, u8 *, u32);
    int (*set_rxfh_context)(struct net_device *, const u32 *, const u8 *, const u8, u32 *, bool);
    void (*get_channels)(struct net_device *, struct ethtool_channels *);
    int (*set_channels)(struct net_device *, struct ethtool_channels *);
    int (*get_dump_flag)(struct net_device *, struct ethtool_dump *);
    int (*get_dump_data)(struct net_device *, struct ethtool_dump *, void *);
    int (*set_dump)(struct net_device *, struct ethtool_dump *);
    int (*get_ts_info)(struct net_device *, struct ethtool_ts_info *);
    int (*get_module_info)(struct net_device *, struct ethtool_modinfo *);
    int (*get_module_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_eee)(struct net_device *, struct ethtool_eee *);
    int (*set_eee)(struct net_device *, struct ethtool_eee *);
    int (*get_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*set_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*get_link_ksettings)(struct net_device *, struct ethtool_link_ksettings *);
    int (*set_link_ksettings)(struct net_device *, const struct ethtool_link_ksettings *);
    int (*get_fecparam)(struct net_device *, struct ethtool_fecparam *);
    int (*set_fecparam)(struct net_device *, struct ethtool_fecparam *);
    void (*get_ethtool_phy_stats)(struct net_device *, struct ethtool_stats *, u64 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ethtool_ops {
    void (*get_drvinfo)(struct net_device *, struct ethtool_drvinfo *);
    int (*get_regs_len)(struct net_device *);
    void (*get_regs)(struct net_device *, struct ethtool_regs *, void *);
    void (*get_wol)(struct net_device *, struct ethtool_wolinfo *);
    int (*set_wol)(struct net_device *, struct ethtool_wolinfo *);
    u32 (*get_msglevel)(struct net_device *);
    void (*set_msglevel)(struct net_device *, u32);
    int (*nway_reset)(struct net_device *);
    u32 (*get_link)(struct net_device *);
    int (*get_eeprom_len)(struct net_device *);
    int (*get_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_coalesce)(struct net_device *, struct ethtool_coalesce *);
    int (*set_coalesce)(struct net_device *, struct ethtool_coalesce *);
    void (*get_ringparam)(struct net_device *, struct ethtool_ringparam *);
    int (*set_ringparam)(struct net_device *, struct ethtool_ringparam *);
    void (*get_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    int (*set_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    void (*self_test)(struct net_device *, struct ethtool_test *, u64 *);
    void (*get_strings)(struct net_device *, u32, u8 *);
    int (*set_phys_id)(struct net_device *, enum ethtool_phys_id_state);
    void (*get_ethtool_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*begin)(struct net_device *);
    void (*complete)(struct net_device *);
    u32 (*get_priv_flags)(struct net_device *);
    int (*set_priv_flags)(struct net_device *, u32);
    int (*get_sset_count)(struct net_device *, int);
    int (*get_rxnfc)(struct net_device *, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct net_device *, struct ethtool_rxnfc *);
    int (*flash_device)(struct net_device *, struct ethtool_flash *);
    int (*reset)(struct net_device *, u32 *);
    u32 (*get_rxfh_key_size)(struct net_device *);
    u32 (*get_rxfh_indir_size)(struct net_device *);
    int (*get_rxfh)(struct net_device *, u32 *, u8 *, u8 *);
    int (*set_rxfh)(struct net_device *, const u32 *, const u8 *, const u8);
    int (*get_rxfh_context)(struct net_device *, u32 *, u8 *, u8 *, u32);
    int (*set_rxfh_context)(struct net_device *, const u32 *, const u8 *, const u8, u32 *, bool);
    void (*get_channels)(struct net_device *, struct ethtool_channels *);
    int (*set_channels)(struct net_device *, struct ethtool_channels *);
    int (*get_dump_flag)(struct net_device *, struct ethtool_dump *);
    int (*get_dump_data)(struct net_device *, struct ethtool_dump *, void *);
    int (*set_dump)(struct net_device *, struct ethtool_dump *);
    int (*get_ts_info)(struct net_device *, struct ethtool_ts_info *);
    int (*get_module_info)(struct net_device *, struct ethtool_modinfo *);
    int (*get_module_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_eee)(struct net_device *, struct ethtool_eee *);
    int (*set_eee)(struct net_device *, struct ethtool_eee *);
    int (*get_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*set_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*get_link_ksettings)(struct net_device *, struct ethtool_link_ksettings *);
    int (*set_link_ksettings)(struct net_device *, const struct ethtool_link_ksettings *);
    int (*get_fecparam)(struct net_device *, struct ethtool_fecparam *);
    int (*set_fecparam)(struct net_device *, struct ethtool_fecparam *);
    void (*get_ethtool_phy_stats)(struct net_device *, struct ethtool_stats *, u64 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ethtool_ops {
    void (*get_drvinfo)(struct net_device *, struct ethtool_drvinfo *);
    int (*get_regs_len)(struct net_device *);
    void (*get_regs)(struct net_device *, struct ethtool_regs *, void *);
    void (*get_wol)(struct net_device *, struct ethtool_wolinfo *);
    int (*set_wol)(struct net_device *, struct ethtool_wolinfo *);
    u32 (*get_msglevel)(struct net_device *);
    void (*set_msglevel)(struct net_device *, u32);
    int (*nway_reset)(struct net_device *);
    u32 (*get_link)(struct net_device *);
    int (*get_eeprom_len)(struct net_device *);
    int (*get_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*set_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_coalesce)(struct net_device *, struct ethtool_coalesce *);
    int (*set_coalesce)(struct net_device *, struct ethtool_coalesce *);
    void (*get_ringparam)(struct net_device *, struct ethtool_ringparam *);
    int (*set_ringparam)(struct net_device *, struct ethtool_ringparam *);
    void (*get_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    int (*set_pauseparam)(struct net_device *, struct ethtool_pauseparam *);
    void (*self_test)(struct net_device *, struct ethtool_test *, u64 *);
    void (*get_strings)(struct net_device *, u32, u8 *);
    int (*set_phys_id)(struct net_device *, enum ethtool_phys_id_state);
    void (*get_ethtool_stats)(struct net_device *, struct ethtool_stats *, u64 *);
    int (*begin)(struct net_device *);
    void (*complete)(struct net_device *);
    u32 (*get_priv_flags)(struct net_device *);
    int (*set_priv_flags)(struct net_device *, u32);
    int (*get_sset_count)(struct net_device *, int);
    int (*get_rxnfc)(struct net_device *, struct ethtool_rxnfc *, u32 *);
    int (*set_rxnfc)(struct net_device *, struct ethtool_rxnfc *);
    int (*flash_device)(struct net_device *, struct ethtool_flash *);
    int (*reset)(struct net_device *, u32 *);
    u32 (*get_rxfh_key_size)(struct net_device *);
    u32 (*get_rxfh_indir_size)(struct net_device *);
    int (*get_rxfh)(struct net_device *, u32 *, u8 *, u8 *);
    int (*set_rxfh)(struct net_device *, const u32 *, const u8 *, const u8);
    int (*get_rxfh_context)(struct net_device *, u32 *, u8 *, u8 *, u32);
    int (*set_rxfh_context)(struct net_device *, const u32 *, const u8 *, const u8, u32 *, bool);
    void (*get_channels)(struct net_device *, struct ethtool_channels *);
    int (*set_channels)(struct net_device *, struct ethtool_channels *);
    int (*get_dump_flag)(struct net_device *, struct ethtool_dump *);
    int (*get_dump_data)(struct net_device *, struct ethtool_dump *, void *);
    int (*set_dump)(struct net_device *, struct ethtool_dump *);
    int (*get_ts_info)(struct net_device *, struct ethtool_ts_info *);
    int (*get_module_info)(struct net_device *, struct ethtool_modinfo *);
    int (*get_module_eeprom)(struct net_device *, struct ethtool_eeprom *, u8 *);
    int (*get_eee)(struct net_device *, struct ethtool_eee *);
    int (*set_eee)(struct net_device *, struct ethtool_eee *);
    int (*get_tunable)(struct net_device *, const struct ethtool_tunable *, void *);
    int (*set_tunable)(struct net_device *, const struct ethtool_tunable *, const void *);
    int (*get_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*set_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *);
    int (*get_link_ksettings)(struct net_device *, struct ethtool_link_ksettings *);
    int (*set_link_ksettings)(struct net_device *, const struct ethtool_link_ksettings *);
    int (*get_fecparam)(struct net_device *, struct ethtool_fecparam *);
    int (*set_fecparam)(struct net_device *, struct ethtool_fecparam *);
    void (*get_ethtool_phy_stats)(struct net_device *, struct ethtool_stats *, u64 *);
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
<code>int (*get_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_per_queue_coalesce)(struct net_device *, u32, struct ethtool_coalesce *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*get_link_ksettings)(struct net_device *, struct ethtool_link_ksettings *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_link_ksettings)(struct net_device *, const struct ethtool_link_ksettings *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*get_fecparam)(struct net_device *, struct ethtool_fecparam *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_fecparam)(struct net_device *, struct ethtool_fecparam *)</code>
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
<code>int (*get_rxfh_context)(struct net_device *, u32 *, u8 *, u8 *, u32)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_rxfh_context)(struct net_device *, const u32 *, const u8 *, const u8, u32 *, bool)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*get_ethtool_phy_stats)(struct net_device *, struct ethtool_stats *, u64 *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*get_settings)(struct net_device *, struct ethtool_cmd *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*set_settings)(struct net_device *, struct ethtool_cmd *)</code>
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
<code>u32 supported_coalesce_params</code>
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
<code>int (*get_link_ext_state)(struct net_device *, struct ethtool_link_ext_state_info *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*get_pause_stats)(struct net_device *, struct ethtool_pause_stats *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*get_phy_tunable)(struct net_device *, const struct ethtool_tunable *, void *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_phy_tunable)(struct net_device *, const struct ethtool_tunable *, const void *)</code>
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
<code>u32 cap_link_lanes_supported</code>
</li>
<li>
<b>Field added. </b>
<code>void (*get_fec_stats)(struct net_device *, struct ethtool_fec_stats *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*get_module_eeprom_by_page)(struct net_device *, const struct ethtool_module_eeprom *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*get_eth_phy_stats)(struct net_device *, struct ethtool_eth_phy_stats *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*get_eth_mac_stats)(struct net_device *, struct ethtool_eth_mac_stats *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*get_eth_ctrl_stats)(struct net_device *, struct ethtool_eth_ctrl_stats *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*get_rmon_stats)(struct net_device *, struct ethtool_rmon_stats *, const struct ethtool_rmon_hist_range **)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*get_coalesce)(struct net_device *, struct ethtool_coalesce *)</code> ➡️ <code>int (*get_coalesce)(struct net_device *, struct ethtool_coalesce *, struct kernel_ethtool_coalesce *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*set_coalesce)(struct net_device *, struct ethtool_coalesce *)</code> ➡️ <code>int (*set_coalesce)(struct net_device *, struct ethtool_coalesce *, struct kernel_ethtool_coalesce *, struct netlink_ext_ack *)</code>
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
<code>u32 supported_ring_params</code>
</li>
<li>
<b>Field added. </b>
<code>int (*get_module_power_mode)(struct net_device *, struct ethtool_module_power_mode_params *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_module_power_mode)(struct net_device *, const struct ethtool_module_power_mode_params *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*get_ringparam)(struct net_device *, struct ethtool_ringparam *)</code> ➡️ <code>void (*get_ringparam)(struct net_device *, struct ethtool_ringparam *, struct kernel_ethtool_ringparam *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*set_ringparam)(struct net_device *, struct ethtool_ringparam *)</code> ➡️ <code>int (*set_ringparam)(struct net_device *, struct ethtool_ringparam *, struct kernel_ethtool_ringparam *, struct netlink_ext_ack *)</code>
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
<code>void (*get_link_ext_stats)(struct net_device *, struct ethtool_link_ext_stats *)</code>
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
<code>int (*get_mm)(struct net_device *, struct ethtool_mm_state *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_mm)(struct net_device *, struct ethtool_mm_cfg *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*get_mm_stats)(struct net_device *, struct ethtool_mm_stats *)</code>
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
<code>u32 cap_rss_ctx_supported</code>
</li>
<li>
<b>Field added. </b>
<code>u32 cap_rss_sym_xor_supported</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*get_rxfh_context)(struct net_device *, u32 *, u8 *, u8 *, u32)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*set_rxfh_context)(struct net_device *, const u32 *, const u8 *, const u8, u32 *, bool)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*get_rxfh)(struct net_device *, u32 *, u8 *, u8 *)</code> ➡️ <code>int (*get_rxfh)(struct net_device *, struct ethtool_rxfh_param *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*set_rxfh)(struct net_device *, const u32 *, const u8 *, const u8)</code> ➡️ <code>int (*set_rxfh)(struct net_device *, struct ethtool_rxfh_param *, struct netlink_ext_ack *)</code>
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
