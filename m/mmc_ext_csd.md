# Struct: <code>mmc_ext_csd</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct mmc_ext_csd {
    u8 rev;
    u8 erase_group_def;
    u8 sec_feature_support;
    u8 rel_sectors;
    u8 rel_param;
    u8 part_config;
    u8 cache_ctrl;
    u8 rst_n_function;
    u8 max_packed_writes;
    u8 max_packed_reads;
    u8 packed_event_en;
    unsigned int part_time;
    unsigned int sa_timeout;
    unsigned int generic_cmd6_time;
    unsigned int power_off_longtime;
    u8 power_off_notification;
    unsigned int hs_max_dtr;
    unsigned int hs200_max_dtr;
    unsigned int sectors;
    unsigned int hc_erase_size;
    unsigned int hc_erase_timeout;
    unsigned int sec_trim_mult;
    unsigned int sec_erase_mult;
    unsigned int trim_timeout;
    bool partition_setting_completed;
    long long unsigned int enhanced_area_offset;
    unsigned int enhanced_area_size;
    unsigned int cache_size;
    bool hpi_en;
    bool hpi;
    unsigned int hpi_cmd;
    bool bkops;
    bool man_bkops_en;
    unsigned int data_sector_size;
    unsigned int data_tag_unit_size;
    unsigned int boot_ro_lock;
    bool boot_ro_lockable;
    bool ffu_capable;
    u8 fwrev[8];
    u8 raw_exception_status;
    u8 raw_partition_support;
    u8 raw_rpmb_size_mult;
    u8 raw_erased_mem_count;
    u8 raw_ext_csd_structure;
    u8 raw_card_type;
    u8 raw_driver_strength;
    u8 out_of_int_time;
    u8 raw_pwr_cl_52_195;
    u8 raw_pwr_cl_26_195;
    u8 raw_pwr_cl_52_360;
    u8 raw_pwr_cl_26_360;
    u8 raw_s_a_timeout;
    u8 raw_hc_erase_gap_size;
    u8 raw_erase_timeout_mult;
    u8 raw_hc_erase_grp_size;
    u8 raw_sec_trim_mult;
    u8 raw_sec_erase_mult;
    u8 raw_sec_feature_support;
    u8 raw_trim_mult;
    u8 raw_pwr_cl_200_195;
    u8 raw_pwr_cl_200_360;
    u8 raw_pwr_cl_ddr_52_195;
    u8 raw_pwr_cl_ddr_52_360;
    u8 raw_pwr_cl_ddr_200_360;
    u8 raw_bkops_status;
    u8 raw_sectors[4];
    unsigned int feature_support;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct mmc_ext_csd {
    u8 rev;
    u8 erase_group_def;
    u8 sec_feature_support;
    u8 rel_sectors;
    u8 rel_param;
    u8 part_config;
    u8 cache_ctrl;
    u8 rst_n_function;
    u8 max_packed_writes;
    u8 max_packed_reads;
    u8 packed_event_en;
    unsigned int part_time;
    unsigned int sa_timeout;
    unsigned int generic_cmd6_time;
    unsigned int power_off_longtime;
    u8 power_off_notification;
    unsigned int hs_max_dtr;
    unsigned int hs200_max_dtr;
    unsigned int sectors;
    unsigned int hc_erase_size;
    unsigned int hc_erase_timeout;
    unsigned int sec_trim_mult;
    unsigned int sec_erase_mult;
    unsigned int trim_timeout;
    bool partition_setting_completed;
    long long unsigned int enhanced_area_offset;
    unsigned int enhanced_area_size;
    unsigned int cache_size;
    bool hpi_en;
    bool hpi;
    unsigned int hpi_cmd;
    bool bkops;
    bool man_bkops_en;
    unsigned int data_sector_size;
    unsigned int data_tag_unit_size;
    unsigned int boot_ro_lock;
    bool boot_ro_lockable;
    bool ffu_capable;
    u8 fwrev[8];
    u8 raw_exception_status;
    u8 raw_partition_support;
    u8 raw_rpmb_size_mult;
    u8 raw_erased_mem_count;
    u8 strobe_support;
    u8 raw_ext_csd_structure;
    u8 raw_card_type;
    u8 raw_driver_strength;
    u8 out_of_int_time;
    u8 raw_pwr_cl_52_195;
    u8 raw_pwr_cl_26_195;
    u8 raw_pwr_cl_52_360;
    u8 raw_pwr_cl_26_360;
    u8 raw_s_a_timeout;
    u8 raw_hc_erase_gap_size;
    u8 raw_erase_timeout_mult;
    u8 raw_hc_erase_grp_size;
    u8 raw_sec_trim_mult;
    u8 raw_sec_erase_mult;
    u8 raw_sec_feature_support;
    u8 raw_trim_mult;
    u8 raw_pwr_cl_200_195;
    u8 raw_pwr_cl_200_360;
    u8 raw_pwr_cl_ddr_52_195;
    u8 raw_pwr_cl_ddr_52_360;
    u8 raw_pwr_cl_ddr_200_360;
    u8 raw_bkops_status;
    u8 raw_sectors[4];
    unsigned int feature_support;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct mmc_ext_csd {
    u8 rev;
    u8 erase_group_def;
    u8 sec_feature_support;
    u8 rel_sectors;
    u8 rel_param;
    u8 part_config;
    u8 cache_ctrl;
    u8 rst_n_function;
    u8 max_packed_writes;
    u8 max_packed_reads;
    u8 packed_event_en;
    unsigned int part_time;
    unsigned int sa_timeout;
    unsigned int generic_cmd6_time;
    unsigned int power_off_longtime;
    u8 power_off_notification;
    unsigned int hs_max_dtr;
    unsigned int hs200_max_dtr;
    unsigned int sectors;
    unsigned int hc_erase_size;
    unsigned int hc_erase_timeout;
    unsigned int sec_trim_mult;
    unsigned int sec_erase_mult;
    unsigned int trim_timeout;
    bool partition_setting_completed;
    long long unsigned int enhanced_area_offset;
    unsigned int enhanced_area_size;
    unsigned int cache_size;
    bool hpi_en;
    bool hpi;
    unsigned int hpi_cmd;
    bool bkops;
    bool man_bkops_en;
    unsigned int data_sector_size;
    unsigned int data_tag_unit_size;
    unsigned int boot_ro_lock;
    bool boot_ro_lockable;
    bool ffu_capable;
    bool cmdq_support;
    unsigned int cmdq_depth;
    u8 fwrev[8];
    u8 raw_exception_status;
    u8 raw_partition_support;
    u8 raw_rpmb_size_mult;
    u8 raw_erased_mem_count;
    u8 strobe_support;
    u8 raw_ext_csd_structure;
    u8 raw_card_type;
    u8 raw_driver_strength;
    u8 out_of_int_time;
    u8 raw_pwr_cl_52_195;
    u8 raw_pwr_cl_26_195;
    u8 raw_pwr_cl_52_360;
    u8 raw_pwr_cl_26_360;
    u8 raw_s_a_timeout;
    u8 raw_hc_erase_gap_size;
    u8 raw_erase_timeout_mult;
    u8 raw_hc_erase_grp_size;
    u8 raw_sec_trim_mult;
    u8 raw_sec_erase_mult;
    u8 raw_sec_feature_support;
    u8 raw_trim_mult;
    u8 raw_pwr_cl_200_195;
    u8 raw_pwr_cl_200_360;
    u8 raw_pwr_cl_ddr_52_195;
    u8 raw_pwr_cl_ddr_52_360;
    u8 raw_pwr_cl_ddr_200_360;
    u8 raw_bkops_status;
    u8 raw_sectors[4];
    unsigned int feature_support;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct mmc_ext_csd {
    u8 rev;
    u8 erase_group_def;
    u8 sec_feature_support;
    u8 rel_sectors;
    u8 rel_param;
    u8 part_config;
    u8 cache_ctrl;
    u8 rst_n_function;
    u8 max_packed_writes;
    u8 max_packed_reads;
    u8 packed_event_en;
    unsigned int part_time;
    unsigned int sa_timeout;
    unsigned int generic_cmd6_time;
    unsigned int power_off_longtime;
    u8 power_off_notification;
    unsigned int hs_max_dtr;
    unsigned int hs200_max_dtr;
    unsigned int sectors;
    unsigned int hc_erase_size;
    unsigned int hc_erase_timeout;
    unsigned int sec_trim_mult;
    unsigned int sec_erase_mult;
    unsigned int trim_timeout;
    bool partition_setting_completed;
    long long unsigned int enhanced_area_offset;
    unsigned int enhanced_area_size;
    unsigned int cache_size;
    bool hpi_en;
    bool hpi;
    unsigned int hpi_cmd;
    bool bkops;
    bool man_bkops_en;
    bool auto_bkops_en;
    unsigned int data_sector_size;
    unsigned int data_tag_unit_size;
    unsigned int boot_ro_lock;
    bool boot_ro_lockable;
    bool ffu_capable;
    bool cmdq_en;
    bool cmdq_support;
    unsigned int cmdq_depth;
    u8 fwrev[8];
    u8 raw_exception_status;
    u8 raw_partition_support;
    u8 raw_rpmb_size_mult;
    u8 raw_erased_mem_count;
    u8 strobe_support;
    u8 raw_ext_csd_structure;
    u8 raw_card_type;
    u8 raw_driver_strength;
    u8 out_of_int_time;
    u8 raw_pwr_cl_52_195;
    u8 raw_pwr_cl_26_195;
    u8 raw_pwr_cl_52_360;
    u8 raw_pwr_cl_26_360;
    u8 raw_s_a_timeout;
    u8 raw_hc_erase_gap_size;
    u8 raw_erase_timeout_mult;
    u8 raw_hc_erase_grp_size;
    u8 raw_sec_trim_mult;
    u8 raw_sec_erase_mult;
    u8 raw_sec_feature_support;
    u8 raw_trim_mult;
    u8 raw_pwr_cl_200_195;
    u8 raw_pwr_cl_200_360;
    u8 raw_pwr_cl_ddr_52_195;
    u8 raw_pwr_cl_ddr_52_360;
    u8 raw_pwr_cl_ddr_200_360;
    u8 raw_bkops_status;
    u8 raw_sectors[4];
    u8 pre_eol_info;
    u8 device_life_time_est_typ_a;
    u8 device_life_time_est_typ_b;
    unsigned int feature_support;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct mmc_ext_csd {
    u8 rev;
    u8 erase_group_def;
    u8 sec_feature_support;
    u8 rel_sectors;
    u8 rel_param;
    u8 part_config;
    u8 cache_ctrl;
    u8 rst_n_function;
    u8 max_packed_writes;
    u8 max_packed_reads;
    u8 packed_event_en;
    unsigned int part_time;
    unsigned int sa_timeout;
    unsigned int generic_cmd6_time;
    unsigned int power_off_longtime;
    u8 power_off_notification;
    unsigned int hs_max_dtr;
    unsigned int hs200_max_dtr;
    unsigned int sectors;
    unsigned int hc_erase_size;
    unsigned int hc_erase_timeout;
    unsigned int sec_trim_mult;
    unsigned int sec_erase_mult;
    unsigned int trim_timeout;
    bool partition_setting_completed;
    long long unsigned int enhanced_area_offset;
    unsigned int enhanced_area_size;
    unsigned int cache_size;
    bool hpi_en;
    bool hpi;
    unsigned int hpi_cmd;
    bool bkops;
    bool man_bkops_en;
    bool auto_bkops_en;
    unsigned int data_sector_size;
    unsigned int data_tag_unit_size;
    unsigned int boot_ro_lock;
    bool boot_ro_lockable;
    bool ffu_capable;
    bool cmdq_en;
    bool cmdq_support;
    unsigned int cmdq_depth;
    u8 fwrev[8];
    u8 raw_exception_status;
    u8 raw_partition_support;
    u8 raw_rpmb_size_mult;
    u8 raw_erased_mem_count;
    u8 strobe_support;
    u8 raw_ext_csd_structure;
    u8 raw_card_type;
    u8 raw_driver_strength;
    u8 out_of_int_time;
    u8 raw_pwr_cl_52_195;
    u8 raw_pwr_cl_26_195;
    u8 raw_pwr_cl_52_360;
    u8 raw_pwr_cl_26_360;
    u8 raw_s_a_timeout;
    u8 raw_hc_erase_gap_size;
    u8 raw_erase_timeout_mult;
    u8 raw_hc_erase_grp_size;
    u8 raw_sec_trim_mult;
    u8 raw_sec_erase_mult;
    u8 raw_sec_feature_support;
    u8 raw_trim_mult;
    u8 raw_pwr_cl_200_195;
    u8 raw_pwr_cl_200_360;
    u8 raw_pwr_cl_ddr_52_195;
    u8 raw_pwr_cl_ddr_52_360;
    u8 raw_pwr_cl_ddr_200_360;
    u8 raw_bkops_status;
    u8 raw_sectors[4];
    u8 pre_eol_info;
    u8 device_life_time_est_typ_a;
    u8 device_life_time_est_typ_b;
    unsigned int feature_support;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct mmc_ext_csd {
    u8 rev;
    u8 erase_group_def;
    u8 sec_feature_support;
    u8 rel_sectors;
    u8 rel_param;
    u8 part_config;
    u8 cache_ctrl;
    u8 rst_n_function;
    u8 max_packed_writes;
    u8 max_packed_reads;
    u8 packed_event_en;
    unsigned int part_time;
    unsigned int sa_timeout;
    unsigned int generic_cmd6_time;
    unsigned int power_off_longtime;
    u8 power_off_notification;
    unsigned int hs_max_dtr;
    unsigned int hs200_max_dtr;
    unsigned int sectors;
    unsigned int hc_erase_size;
    unsigned int hc_erase_timeout;
    unsigned int sec_trim_mult;
    unsigned int sec_erase_mult;
    unsigned int trim_timeout;
    bool partition_setting_completed;
    long long unsigned int enhanced_area_offset;
    unsigned int enhanced_area_size;
    unsigned int cache_size;
    bool hpi_en;
    bool hpi;
    unsigned int hpi_cmd;
    bool bkops;
    bool man_bkops_en;
    bool auto_bkops_en;
    unsigned int data_sector_size;
    unsigned int data_tag_unit_size;
    unsigned int boot_ro_lock;
    bool boot_ro_lockable;
    bool ffu_capable;
    bool cmdq_en;
    bool cmdq_support;
    unsigned int cmdq_depth;
    u8 fwrev[8];
    u8 raw_exception_status;
    u8 raw_partition_support;
    u8 raw_rpmb_size_mult;
    u8 raw_erased_mem_count;
    u8 strobe_support;
    u8 raw_ext_csd_structure;
    u8 raw_card_type;
    u8 raw_driver_strength;
    u8 out_of_int_time;
    u8 raw_pwr_cl_52_195;
    u8 raw_pwr_cl_26_195;
    u8 raw_pwr_cl_52_360;
    u8 raw_pwr_cl_26_360;
    u8 raw_s_a_timeout;
    u8 raw_hc_erase_gap_size;
    u8 raw_erase_timeout_mult;
    u8 raw_hc_erase_grp_size;
    u8 raw_sec_trim_mult;
    u8 raw_sec_erase_mult;
    u8 raw_sec_feature_support;
    u8 raw_trim_mult;
    u8 raw_pwr_cl_200_195;
    u8 raw_pwr_cl_200_360;
    u8 raw_pwr_cl_ddr_52_195;
    u8 raw_pwr_cl_ddr_52_360;
    u8 raw_pwr_cl_ddr_200_360;
    u8 raw_bkops_status;
    u8 raw_sectors[4];
    u8 pre_eol_info;
    u8 device_life_time_est_typ_a;
    u8 device_life_time_est_typ_b;
    unsigned int feature_support;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct mmc_ext_csd {
    u8 rev;
    u8 erase_group_def;
    u8 sec_feature_support;
    u8 rel_sectors;
    u8 rel_param;
    u8 part_config;
    u8 cache_ctrl;
    u8 rst_n_function;
    u8 max_packed_writes;
    u8 max_packed_reads;
    u8 packed_event_en;
    unsigned int part_time;
    unsigned int sa_timeout;
    unsigned int generic_cmd6_time;
    unsigned int power_off_longtime;
    u8 power_off_notification;
    unsigned int hs_max_dtr;
    unsigned int hs200_max_dtr;
    unsigned int sectors;
    unsigned int hc_erase_size;
    unsigned int hc_erase_timeout;
    unsigned int sec_trim_mult;
    unsigned int sec_erase_mult;
    unsigned int trim_timeout;
    bool partition_setting_completed;
    long long unsigned int enhanced_area_offset;
    unsigned int enhanced_area_size;
    unsigned int cache_size;
    bool hpi_en;
    bool hpi;
    unsigned int hpi_cmd;
    bool bkops;
    bool man_bkops_en;
    bool auto_bkops_en;
    unsigned int data_sector_size;
    unsigned int data_tag_unit_size;
    unsigned int boot_ro_lock;
    bool boot_ro_lockable;
    bool ffu_capable;
    bool cmdq_en;
    bool cmdq_support;
    unsigned int cmdq_depth;
    u8 fwrev[8];
    u8 raw_exception_status;
    u8 raw_partition_support;
    u8 raw_rpmb_size_mult;
    u8 raw_erased_mem_count;
    u8 strobe_support;
    u8 raw_ext_csd_structure;
    u8 raw_card_type;
    u8 raw_driver_strength;
    u8 out_of_int_time;
    u8 raw_pwr_cl_52_195;
    u8 raw_pwr_cl_26_195;
    u8 raw_pwr_cl_52_360;
    u8 raw_pwr_cl_26_360;
    u8 raw_s_a_timeout;
    u8 raw_hc_erase_gap_size;
    u8 raw_erase_timeout_mult;
    u8 raw_hc_erase_grp_size;
    u8 raw_sec_trim_mult;
    u8 raw_sec_erase_mult;
    u8 raw_sec_feature_support;
    u8 raw_trim_mult;
    u8 raw_pwr_cl_200_195;
    u8 raw_pwr_cl_200_360;
    u8 raw_pwr_cl_ddr_52_195;
    u8 raw_pwr_cl_ddr_52_360;
    u8 raw_pwr_cl_ddr_200_360;
    u8 raw_bkops_status;
    u8 raw_sectors[4];
    u8 pre_eol_info;
    u8 device_life_time_est_typ_a;
    u8 device_life_time_est_typ_b;
    unsigned int feature_support;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct mmc_ext_csd {
    u8 rev;
    u8 erase_group_def;
    u8 sec_feature_support;
    u8 rel_sectors;
    u8 rel_param;
    u8 part_config;
    u8 cache_ctrl;
    u8 rst_n_function;
    u8 max_packed_writes;
    u8 max_packed_reads;
    u8 packed_event_en;
    unsigned int part_time;
    unsigned int sa_timeout;
    unsigned int generic_cmd6_time;
    unsigned int power_off_longtime;
    u8 power_off_notification;
    unsigned int hs_max_dtr;
    unsigned int hs200_max_dtr;
    unsigned int sectors;
    unsigned int hc_erase_size;
    unsigned int hc_erase_timeout;
    unsigned int sec_trim_mult;
    unsigned int sec_erase_mult;
    unsigned int trim_timeout;
    bool partition_setting_completed;
    long long unsigned int enhanced_area_offset;
    unsigned int enhanced_area_size;
    unsigned int cache_size;
    bool hpi_en;
    bool hpi;
    unsigned int hpi_cmd;
    bool bkops;
    bool man_bkops_en;
    bool auto_bkops_en;
    unsigned int data_sector_size;
    unsigned int data_tag_unit_size;
    unsigned int boot_ro_lock;
    bool boot_ro_lockable;
    bool ffu_capable;
    bool cmdq_en;
    bool cmdq_support;
    unsigned int cmdq_depth;
    u8 fwrev[8];
    u8 raw_exception_status;
    u8 raw_partition_support;
    u8 raw_rpmb_size_mult;
    u8 raw_erased_mem_count;
    u8 strobe_support;
    u8 raw_ext_csd_structure;
    u8 raw_card_type;
    u8 raw_driver_strength;
    u8 out_of_int_time;
    u8 raw_pwr_cl_52_195;
    u8 raw_pwr_cl_26_195;
    u8 raw_pwr_cl_52_360;
    u8 raw_pwr_cl_26_360;
    u8 raw_s_a_timeout;
    u8 raw_hc_erase_gap_size;
    u8 raw_erase_timeout_mult;
    u8 raw_hc_erase_grp_size;
    u8 raw_sec_trim_mult;
    u8 raw_sec_erase_mult;
    u8 raw_sec_feature_support;
    u8 raw_trim_mult;
    u8 raw_pwr_cl_200_195;
    u8 raw_pwr_cl_200_360;
    u8 raw_pwr_cl_ddr_52_195;
    u8 raw_pwr_cl_ddr_52_360;
    u8 raw_pwr_cl_ddr_200_360;
    u8 raw_bkops_status;
    u8 raw_sectors[4];
    u8 pre_eol_info;
    u8 device_life_time_est_typ_a;
    u8 device_life_time_est_typ_b;
    unsigned int feature_support;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct mmc_ext_csd {
    u8 rev;
    u8 erase_group_def;
    u8 sec_feature_support;
    u8 rel_sectors;
    u8 rel_param;
    u8 part_config;
    u8 cache_ctrl;
    u8 rst_n_function;
    u8 max_packed_writes;
    u8 max_packed_reads;
    u8 packed_event_en;
    unsigned int part_time;
    unsigned int sa_timeout;
    unsigned int generic_cmd6_time;
    unsigned int power_off_longtime;
    u8 power_off_notification;
    unsigned int hs_max_dtr;
    unsigned int hs200_max_dtr;
    unsigned int sectors;
    unsigned int hc_erase_size;
    unsigned int hc_erase_timeout;
    unsigned int sec_trim_mult;
    unsigned int sec_erase_mult;
    unsigned int trim_timeout;
    bool partition_setting_completed;
    long long unsigned int enhanced_area_offset;
    unsigned int enhanced_area_size;
    unsigned int cache_size;
    bool hpi_en;
    bool hpi;
    unsigned int hpi_cmd;
    bool bkops;
    bool man_bkops_en;
    bool auto_bkops_en;
    unsigned int data_sector_size;
    unsigned int data_tag_unit_size;
    unsigned int boot_ro_lock;
    bool boot_ro_lockable;
    bool ffu_capable;
    bool cmdq_en;
    bool cmdq_support;
    unsigned int cmdq_depth;
    u8 fwrev[8];
    u8 raw_exception_status;
    u8 raw_partition_support;
    u8 raw_rpmb_size_mult;
    u8 raw_erased_mem_count;
    u8 strobe_support;
    u8 raw_ext_csd_structure;
    u8 raw_card_type;
    u8 raw_driver_strength;
    u8 out_of_int_time;
    u8 raw_pwr_cl_52_195;
    u8 raw_pwr_cl_26_195;
    u8 raw_pwr_cl_52_360;
    u8 raw_pwr_cl_26_360;
    u8 raw_s_a_timeout;
    u8 raw_hc_erase_gap_size;
    u8 raw_erase_timeout_mult;
    u8 raw_hc_erase_grp_size;
    u8 raw_sec_trim_mult;
    u8 raw_sec_erase_mult;
    u8 raw_sec_feature_support;
    u8 raw_trim_mult;
    u8 raw_pwr_cl_200_195;
    u8 raw_pwr_cl_200_360;
    u8 raw_pwr_cl_ddr_52_195;
    u8 raw_pwr_cl_ddr_52_360;
    u8 raw_pwr_cl_ddr_200_360;
    u8 raw_bkops_status;
    u8 raw_sectors[4];
    u8 pre_eol_info;
    u8 device_life_time_est_typ_a;
    u8 device_life_time_est_typ_b;
    unsigned int feature_support;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct mmc_ext_csd {
    u8 rev;
    u8 erase_group_def;
    u8 sec_feature_support;
    u8 rel_sectors;
    u8 rel_param;
    bool enhanced_rpmb_supported;
    u8 part_config;
    u8 cache_ctrl;
    u8 rst_n_function;
    u8 max_packed_writes;
    u8 max_packed_reads;
    u8 packed_event_en;
    unsigned int part_time;
    unsigned int sa_timeout;
    unsigned int generic_cmd6_time;
    unsigned int power_off_longtime;
    u8 power_off_notification;
    unsigned int hs_max_dtr;
    unsigned int hs200_max_dtr;
    unsigned int sectors;
    unsigned int hc_erase_size;
    unsigned int hc_erase_timeout;
    unsigned int sec_trim_mult;
    unsigned int sec_erase_mult;
    unsigned int trim_timeout;
    bool partition_setting_completed;
    long long unsigned int enhanced_area_offset;
    unsigned int enhanced_area_size;
    unsigned int cache_size;
    bool hpi_en;
    bool hpi;
    unsigned int hpi_cmd;
    bool bkops;
    bool man_bkops_en;
    bool auto_bkops_en;
    unsigned int data_sector_size;
    unsigned int data_tag_unit_size;
    unsigned int boot_ro_lock;
    bool boot_ro_lockable;
    bool ffu_capable;
    bool cmdq_en;
    bool cmdq_support;
    unsigned int cmdq_depth;
    u8 fwrev[8];
    u8 raw_exception_status;
    u8 raw_partition_support;
    u8 raw_rpmb_size_mult;
    u8 raw_erased_mem_count;
    u8 strobe_support;
    u8 raw_ext_csd_structure;
    u8 raw_card_type;
    u8 raw_driver_strength;
    u8 out_of_int_time;
    u8 raw_pwr_cl_52_195;
    u8 raw_pwr_cl_26_195;
    u8 raw_pwr_cl_52_360;
    u8 raw_pwr_cl_26_360;
    u8 raw_s_a_timeout;
    u8 raw_hc_erase_gap_size;
    u8 raw_erase_timeout_mult;
    u8 raw_hc_erase_grp_size;
    u8 raw_sec_trim_mult;
    u8 raw_sec_erase_mult;
    u8 raw_sec_feature_support;
    u8 raw_trim_mult;
    u8 raw_pwr_cl_200_195;
    u8 raw_pwr_cl_200_360;
    u8 raw_pwr_cl_ddr_52_195;
    u8 raw_pwr_cl_ddr_52_360;
    u8 raw_pwr_cl_ddr_200_360;
    u8 raw_bkops_status;
    u8 raw_sectors[4];
    u8 pre_eol_info;
    u8 device_life_time_est_typ_a;
    u8 device_life_time_est_typ_b;
    unsigned int feature_support;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mmc_ext_csd {
    u8 rev;
    u8 erase_group_def;
    u8 sec_feature_support;
    u8 rel_sectors;
    u8 rel_param;
    bool enhanced_rpmb_supported;
    u8 part_config;
    u8 cache_ctrl;
    u8 rst_n_function;
    u8 max_packed_writes;
    u8 max_packed_reads;
    u8 packed_event_en;
    unsigned int part_time;
    unsigned int sa_timeout;
    unsigned int generic_cmd6_time;
    unsigned int power_off_longtime;
    u8 power_off_notification;
    unsigned int hs_max_dtr;
    unsigned int hs200_max_dtr;
    unsigned int sectors;
    unsigned int hc_erase_size;
    unsigned int hc_erase_timeout;
    unsigned int sec_trim_mult;
    unsigned int sec_erase_mult;
    unsigned int trim_timeout;
    bool partition_setting_completed;
    long long unsigned int enhanced_area_offset;
    unsigned int enhanced_area_size;
    unsigned int cache_size;
    bool hpi_en;
    bool hpi;
    unsigned int hpi_cmd;
    bool bkops;
    bool man_bkops_en;
    bool auto_bkops_en;
    unsigned int data_sector_size;
    unsigned int data_tag_unit_size;
    unsigned int boot_ro_lock;
    bool boot_ro_lockable;
    bool ffu_capable;
    bool cmdq_en;
    bool cmdq_support;
    unsigned int cmdq_depth;
    u8 fwrev[8];
    u8 raw_exception_status;
    u8 raw_partition_support;
    u8 raw_rpmb_size_mult;
    u8 raw_erased_mem_count;
    u8 strobe_support;
    u8 raw_ext_csd_structure;
    u8 raw_card_type;
    u8 raw_driver_strength;
    u8 out_of_int_time;
    u8 raw_pwr_cl_52_195;
    u8 raw_pwr_cl_26_195;
    u8 raw_pwr_cl_52_360;
    u8 raw_pwr_cl_26_360;
    u8 raw_s_a_timeout;
    u8 raw_hc_erase_gap_size;
    u8 raw_erase_timeout_mult;
    u8 raw_hc_erase_grp_size;
    u8 raw_sec_trim_mult;
    u8 raw_sec_erase_mult;
    u8 raw_sec_feature_support;
    u8 raw_trim_mult;
    u8 raw_pwr_cl_200_195;
    u8 raw_pwr_cl_200_360;
    u8 raw_pwr_cl_ddr_52_195;
    u8 raw_pwr_cl_ddr_52_360;
    u8 raw_pwr_cl_ddr_200_360;
    u8 raw_bkops_status;
    u8 raw_sectors[4];
    u8 pre_eol_info;
    u8 device_life_time_est_typ_a;
    u8 device_life_time_est_typ_b;
    unsigned int feature_support;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mmc_ext_csd {
    u8 rev;
    u8 erase_group_def;
    u8 sec_feature_support;
    u8 rel_sectors;
    u8 rel_param;
    bool enhanced_rpmb_supported;
    u8 part_config;
    u8 cache_ctrl;
    u8 rst_n_function;
    u8 max_packed_writes;
    u8 max_packed_reads;
    u8 packed_event_en;
    unsigned int part_time;
    unsigned int sa_timeout;
    unsigned int generic_cmd6_time;
    unsigned int power_off_longtime;
    u8 power_off_notification;
    unsigned int hs_max_dtr;
    unsigned int hs200_max_dtr;
    unsigned int sectors;
    unsigned int hc_erase_size;
    unsigned int hc_erase_timeout;
    unsigned int sec_trim_mult;
    unsigned int sec_erase_mult;
    unsigned int trim_timeout;
    bool partition_setting_completed;
    long long unsigned int enhanced_area_offset;
    unsigned int enhanced_area_size;
    unsigned int cache_size;
    bool hpi_en;
    bool hpi;
    unsigned int hpi_cmd;
    bool bkops;
    bool man_bkops_en;
    bool auto_bkops_en;
    unsigned int data_sector_size;
    unsigned int data_tag_unit_size;
    unsigned int boot_ro_lock;
    bool boot_ro_lockable;
    bool ffu_capable;
    bool cmdq_en;
    bool cmdq_support;
    unsigned int cmdq_depth;
    u8 fwrev[8];
    u8 raw_exception_status;
    u8 raw_partition_support;
    u8 raw_rpmb_size_mult;
    u8 raw_erased_mem_count;
    u8 strobe_support;
    u8 raw_ext_csd_structure;
    u8 raw_card_type;
    u8 raw_driver_strength;
    u8 out_of_int_time;
    u8 raw_pwr_cl_52_195;
    u8 raw_pwr_cl_26_195;
    u8 raw_pwr_cl_52_360;
    u8 raw_pwr_cl_26_360;
    u8 raw_s_a_timeout;
    u8 raw_hc_erase_gap_size;
    u8 raw_erase_timeout_mult;
    u8 raw_hc_erase_grp_size;
    u8 raw_sec_trim_mult;
    u8 raw_sec_erase_mult;
    u8 raw_sec_feature_support;
    u8 raw_trim_mult;
    u8 raw_pwr_cl_200_195;
    u8 raw_pwr_cl_200_360;
    u8 raw_pwr_cl_ddr_52_195;
    u8 raw_pwr_cl_ddr_52_360;
    u8 raw_pwr_cl_ddr_200_360;
    u8 raw_bkops_status;
    u8 raw_sectors[4];
    u8 pre_eol_info;
    u8 device_life_time_est_typ_a;
    u8 device_life_time_est_typ_b;
    unsigned int feature_support;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mmc_ext_csd {
    u8 rev;
    u8 erase_group_def;
    u8 sec_feature_support;
    u8 rel_sectors;
    u8 rel_param;
    bool enhanced_rpmb_supported;
    u8 part_config;
    u8 cache_ctrl;
    u8 rst_n_function;
    u8 max_packed_writes;
    u8 max_packed_reads;
    u8 packed_event_en;
    unsigned int part_time;
    unsigned int sa_timeout;
    unsigned int generic_cmd6_time;
    unsigned int power_off_longtime;
    u8 power_off_notification;
    unsigned int hs_max_dtr;
    unsigned int hs200_max_dtr;
    unsigned int sectors;
    unsigned int hc_erase_size;
    unsigned int hc_erase_timeout;
    unsigned int sec_trim_mult;
    unsigned int sec_erase_mult;
    unsigned int trim_timeout;
    bool partition_setting_completed;
    long long unsigned int enhanced_area_offset;
    unsigned int enhanced_area_size;
    unsigned int cache_size;
    bool hpi_en;
    bool hpi;
    unsigned int hpi_cmd;
    bool bkops;
    bool man_bkops_en;
    bool auto_bkops_en;
    unsigned int data_sector_size;
    unsigned int data_tag_unit_size;
    unsigned int boot_ro_lock;
    bool boot_ro_lockable;
    bool ffu_capable;
    bool cmdq_en;
    bool cmdq_support;
    unsigned int cmdq_depth;
    u8 fwrev[8];
    u8 raw_exception_status;
    u8 raw_partition_support;
    u8 raw_rpmb_size_mult;
    u8 raw_erased_mem_count;
    u8 strobe_support;
    u8 raw_ext_csd_structure;
    u8 raw_card_type;
    u8 raw_driver_strength;
    u8 out_of_int_time;
    u8 raw_pwr_cl_52_195;
    u8 raw_pwr_cl_26_195;
    u8 raw_pwr_cl_52_360;
    u8 raw_pwr_cl_26_360;
    u8 raw_s_a_timeout;
    u8 raw_hc_erase_gap_size;
    u8 raw_erase_timeout_mult;
    u8 raw_hc_erase_grp_size;
    u8 raw_boot_mult;
    u8 raw_sec_trim_mult;
    u8 raw_sec_erase_mult;
    u8 raw_sec_feature_support;
    u8 raw_trim_mult;
    u8 raw_pwr_cl_200_195;
    u8 raw_pwr_cl_200_360;
    u8 raw_pwr_cl_ddr_52_195;
    u8 raw_pwr_cl_ddr_52_360;
    u8 raw_pwr_cl_ddr_200_360;
    u8 raw_bkops_status;
    u8 raw_sectors[4];
    u8 pre_eol_info;
    u8 device_life_time_est_typ_a;
    u8 device_life_time_est_typ_b;
    unsigned int feature_support;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mmc_ext_csd {
    u8 rev;
    u8 erase_group_def;
    u8 sec_feature_support;
    u8 rel_sectors;
    u8 rel_param;
    bool enhanced_rpmb_supported;
    u8 part_config;
    u8 cache_ctrl;
    u8 rst_n_function;
    u8 max_packed_writes;
    u8 max_packed_reads;
    u8 packed_event_en;
    unsigned int part_time;
    unsigned int sa_timeout;
    unsigned int generic_cmd6_time;
    unsigned int power_off_longtime;
    u8 power_off_notification;
    unsigned int hs_max_dtr;
    unsigned int hs200_max_dtr;
    unsigned int sectors;
    unsigned int hc_erase_size;
    unsigned int hc_erase_timeout;
    unsigned int sec_trim_mult;
    unsigned int sec_erase_mult;
    unsigned int trim_timeout;
    bool partition_setting_completed;
    long long unsigned int enhanced_area_offset;
    unsigned int enhanced_area_size;
    unsigned int cache_size;
    bool hpi_en;
    bool hpi;
    unsigned int hpi_cmd;
    bool bkops;
    bool man_bkops_en;
    bool auto_bkops_en;
    unsigned int data_sector_size;
    unsigned int data_tag_unit_size;
    unsigned int boot_ro_lock;
    bool boot_ro_lockable;
    bool ffu_capable;
    bool cmdq_en;
    bool cmdq_support;
    unsigned int cmdq_depth;
    u8 fwrev[8];
    u8 raw_exception_status;
    u8 raw_partition_support;
    u8 raw_rpmb_size_mult;
    u8 raw_erased_mem_count;
    u8 strobe_support;
    u8 raw_ext_csd_structure;
    u8 raw_card_type;
    u8 raw_driver_strength;
    u8 out_of_int_time;
    u8 raw_pwr_cl_52_195;
    u8 raw_pwr_cl_26_195;
    u8 raw_pwr_cl_52_360;
    u8 raw_pwr_cl_26_360;
    u8 raw_s_a_timeout;
    u8 raw_hc_erase_gap_size;
    u8 raw_erase_timeout_mult;
    u8 raw_hc_erase_grp_size;
    u8 raw_boot_mult;
    u8 raw_sec_trim_mult;
    u8 raw_sec_erase_mult;
    u8 raw_sec_feature_support;
    u8 raw_trim_mult;
    u8 raw_pwr_cl_200_195;
    u8 raw_pwr_cl_200_360;
    u8 raw_pwr_cl_ddr_52_195;
    u8 raw_pwr_cl_ddr_52_360;
    u8 raw_pwr_cl_ddr_200_360;
    u8 raw_bkops_status;
    u8 raw_sectors[4];
    u8 pre_eol_info;
    u8 device_life_time_est_typ_a;
    u8 device_life_time_est_typ_b;
    unsigned int feature_support;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mmc_ext_csd {
    u8 rev;
    u8 erase_group_def;
    u8 sec_feature_support;
    u8 rel_sectors;
    u8 rel_param;
    bool enhanced_rpmb_supported;
    u8 part_config;
    u8 cache_ctrl;
    u8 rst_n_function;
    u8 max_packed_writes;
    u8 max_packed_reads;
    u8 packed_event_en;
    unsigned int part_time;
    unsigned int sa_timeout;
    unsigned int generic_cmd6_time;
    unsigned int power_off_longtime;
    u8 power_off_notification;
    unsigned int hs_max_dtr;
    unsigned int hs200_max_dtr;
    unsigned int sectors;
    unsigned int hc_erase_size;
    unsigned int hc_erase_timeout;
    unsigned int sec_trim_mult;
    unsigned int sec_erase_mult;
    unsigned int trim_timeout;
    bool partition_setting_completed;
    long long unsigned int enhanced_area_offset;
    unsigned int enhanced_area_size;
    unsigned int cache_size;
    bool hpi_en;
    bool hpi;
    unsigned int hpi_cmd;
    bool bkops;
    bool man_bkops_en;
    bool auto_bkops_en;
    unsigned int data_sector_size;
    unsigned int data_tag_unit_size;
    unsigned int boot_ro_lock;
    bool boot_ro_lockable;
    bool ffu_capable;
    bool cmdq_en;
    bool cmdq_support;
    unsigned int cmdq_depth;
    u8 fwrev[8];
    u8 raw_exception_status;
    u8 raw_partition_support;
    u8 raw_rpmb_size_mult;
    u8 raw_erased_mem_count;
    u8 strobe_support;
    u8 raw_ext_csd_structure;
    u8 raw_card_type;
    u8 raw_driver_strength;
    u8 out_of_int_time;
    u8 raw_pwr_cl_52_195;
    u8 raw_pwr_cl_26_195;
    u8 raw_pwr_cl_52_360;
    u8 raw_pwr_cl_26_360;
    u8 raw_s_a_timeout;
    u8 raw_hc_erase_gap_size;
    u8 raw_erase_timeout_mult;
    u8 raw_hc_erase_grp_size;
    u8 raw_boot_mult;
    u8 raw_sec_trim_mult;
    u8 raw_sec_erase_mult;
    u8 raw_sec_feature_support;
    u8 raw_trim_mult;
    u8 raw_pwr_cl_200_195;
    u8 raw_pwr_cl_200_360;
    u8 raw_pwr_cl_ddr_52_195;
    u8 raw_pwr_cl_ddr_52_360;
    u8 raw_pwr_cl_ddr_200_360;
    u8 raw_bkops_status;
    u8 raw_sectors[4];
    u8 pre_eol_info;
    u8 device_life_time_est_typ_a;
    u8 device_life_time_est_typ_b;
    unsigned int feature_support;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mmc_ext_csd {
    u8 rev;
    u8 erase_group_def;
    u8 sec_feature_support;
    u8 rel_sectors;
    u8 rel_param;
    bool enhanced_rpmb_supported;
    u8 part_config;
    u8 cache_ctrl;
    u8 rst_n_function;
    u8 max_packed_writes;
    u8 max_packed_reads;
    u8 packed_event_en;
    unsigned int part_time;
    unsigned int sa_timeout;
    unsigned int generic_cmd6_time;
    unsigned int power_off_longtime;
    u8 power_off_notification;
    unsigned int hs_max_dtr;
    unsigned int hs200_max_dtr;
    unsigned int sectors;
    unsigned int hc_erase_size;
    unsigned int hc_erase_timeout;
    unsigned int sec_trim_mult;
    unsigned int sec_erase_mult;
    unsigned int trim_timeout;
    bool partition_setting_completed;
    long long unsigned int enhanced_area_offset;
    unsigned int enhanced_area_size;
    unsigned int cache_size;
    bool hpi_en;
    bool hpi;
    unsigned int hpi_cmd;
    bool bkops;
    bool man_bkops_en;
    bool auto_bkops_en;
    unsigned int data_sector_size;
    unsigned int data_tag_unit_size;
    unsigned int boot_ro_lock;
    bool boot_ro_lockable;
    bool ffu_capable;
    bool cmdq_en;
    bool cmdq_support;
    unsigned int cmdq_depth;
    u8 fwrev[8];
    u8 raw_exception_status;
    u8 raw_partition_support;
    u8 raw_rpmb_size_mult;
    u8 raw_erased_mem_count;
    u8 strobe_support;
    u8 raw_ext_csd_structure;
    u8 raw_card_type;
    u8 raw_driver_strength;
    u8 out_of_int_time;
    u8 raw_pwr_cl_52_195;
    u8 raw_pwr_cl_26_195;
    u8 raw_pwr_cl_52_360;
    u8 raw_pwr_cl_26_360;
    u8 raw_s_a_timeout;
    u8 raw_hc_erase_gap_size;
    u8 raw_erase_timeout_mult;
    u8 raw_hc_erase_grp_size;
    u8 raw_boot_mult;
    u8 raw_sec_trim_mult;
    u8 raw_sec_erase_mult;
    u8 raw_sec_feature_support;
    u8 raw_trim_mult;
    u8 raw_pwr_cl_200_195;
    u8 raw_pwr_cl_200_360;
    u8 raw_pwr_cl_ddr_52_195;
    u8 raw_pwr_cl_ddr_52_360;
    u8 raw_pwr_cl_ddr_200_360;
    u8 raw_bkops_status;
    u8 raw_sectors[4];
    u8 pre_eol_info;
    u8 device_life_time_est_typ_a;
    u8 device_life_time_est_typ_b;
    unsigned int feature_support;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mmc_ext_csd {
    u8 rev;
    u8 erase_group_def;
    u8 sec_feature_support;
    u8 rel_sectors;
    u8 rel_param;
    bool enhanced_rpmb_supported;
    u8 part_config;
    u8 cache_ctrl;
    u8 rst_n_function;
    unsigned int part_time;
    unsigned int sa_timeout;
    unsigned int generic_cmd6_time;
    unsigned int power_off_longtime;
    u8 power_off_notification;
    unsigned int hs_max_dtr;
    unsigned int hs200_max_dtr;
    unsigned int sectors;
    unsigned int hc_erase_size;
    unsigned int hc_erase_timeout;
    unsigned int sec_trim_mult;
    unsigned int sec_erase_mult;
    unsigned int trim_timeout;
    bool partition_setting_completed;
    long long unsigned int enhanced_area_offset;
    unsigned int enhanced_area_size;
    unsigned int cache_size;
    bool hpi_en;
    bool hpi;
    unsigned int hpi_cmd;
    bool bkops;
    bool man_bkops_en;
    bool auto_bkops_en;
    unsigned int data_sector_size;
    unsigned int data_tag_unit_size;
    unsigned int boot_ro_lock;
    bool boot_ro_lockable;
    bool ffu_capable;
    bool cmdq_en;
    bool cmdq_support;
    unsigned int cmdq_depth;
    u8 fwrev[8];
    u8 raw_exception_status;
    u8 raw_partition_support;
    u8 raw_rpmb_size_mult;
    u8 raw_erased_mem_count;
    u8 strobe_support;
    u8 raw_ext_csd_structure;
    u8 raw_card_type;
    u8 raw_driver_strength;
    u8 out_of_int_time;
    u8 raw_pwr_cl_52_195;
    u8 raw_pwr_cl_26_195;
    u8 raw_pwr_cl_52_360;
    u8 raw_pwr_cl_26_360;
    u8 raw_s_a_timeout;
    u8 raw_hc_erase_gap_size;
    u8 raw_erase_timeout_mult;
    u8 raw_hc_erase_grp_size;
    u8 raw_boot_mult;
    u8 raw_sec_trim_mult;
    u8 raw_sec_erase_mult;
    u8 raw_sec_feature_support;
    u8 raw_trim_mult;
    u8 raw_pwr_cl_200_195;
    u8 raw_pwr_cl_200_360;
    u8 raw_pwr_cl_ddr_52_195;
    u8 raw_pwr_cl_ddr_52_360;
    u8 raw_pwr_cl_ddr_200_360;
    u8 raw_bkops_status;
    u8 raw_sectors[4];
    u8 pre_eol_info;
    u8 device_life_time_est_typ_a;
    u8 device_life_time_est_typ_b;
    unsigned int feature_support;
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
struct mmc_ext_csd {
    u8 rev;
    u8 erase_group_def;
    u8 sec_feature_support;
    u8 rel_sectors;
    u8 rel_param;
    u8 part_config;
    u8 cache_ctrl;
    u8 rst_n_function;
    u8 max_packed_writes;
    u8 max_packed_reads;
    u8 packed_event_en;
    unsigned int part_time;
    unsigned int sa_timeout;
    unsigned int generic_cmd6_time;
    unsigned int power_off_longtime;
    u8 power_off_notification;
    unsigned int hs_max_dtr;
    unsigned int hs200_max_dtr;
    unsigned int sectors;
    unsigned int hc_erase_size;
    unsigned int hc_erase_timeout;
    unsigned int sec_trim_mult;
    unsigned int sec_erase_mult;
    unsigned int trim_timeout;
    bool partition_setting_completed;
    long long unsigned int enhanced_area_offset;
    unsigned int enhanced_area_size;
    unsigned int cache_size;
    bool hpi_en;
    bool hpi;
    unsigned int hpi_cmd;
    bool bkops;
    bool man_bkops_en;
    bool auto_bkops_en;
    unsigned int data_sector_size;
    unsigned int data_tag_unit_size;
    unsigned int boot_ro_lock;
    bool boot_ro_lockable;
    bool ffu_capable;
    bool cmdq_en;
    bool cmdq_support;
    unsigned int cmdq_depth;
    u8 fwrev[8];
    u8 raw_exception_status;
    u8 raw_partition_support;
    u8 raw_rpmb_size_mult;
    u8 raw_erased_mem_count;
    u8 strobe_support;
    u8 raw_ext_csd_structure;
    u8 raw_card_type;
    u8 raw_driver_strength;
    u8 out_of_int_time;
    u8 raw_pwr_cl_52_195;
    u8 raw_pwr_cl_26_195;
    u8 raw_pwr_cl_52_360;
    u8 raw_pwr_cl_26_360;
    u8 raw_s_a_timeout;
    u8 raw_hc_erase_gap_size;
    u8 raw_erase_timeout_mult;
    u8 raw_hc_erase_grp_size;
    u8 raw_sec_trim_mult;
    u8 raw_sec_erase_mult;
    u8 raw_sec_feature_support;
    u8 raw_trim_mult;
    u8 raw_pwr_cl_200_195;
    u8 raw_pwr_cl_200_360;
    u8 raw_pwr_cl_ddr_52_195;
    u8 raw_pwr_cl_ddr_52_360;
    u8 raw_pwr_cl_ddr_200_360;
    u8 raw_bkops_status;
    u8 raw_sectors[4];
    u8 pre_eol_info;
    u8 device_life_time_est_typ_a;
    u8 device_life_time_est_typ_b;
    unsigned int feature_support;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mmc_ext_csd {
    u8 rev;
    u8 erase_group_def;
    u8 sec_feature_support;
    u8 rel_sectors;
    u8 rel_param;
    u8 part_config;
    u8 cache_ctrl;
    u8 rst_n_function;
    u8 max_packed_writes;
    u8 max_packed_reads;
    u8 packed_event_en;
    unsigned int part_time;
    unsigned int sa_timeout;
    unsigned int generic_cmd6_time;
    unsigned int power_off_longtime;
    u8 power_off_notification;
    unsigned int hs_max_dtr;
    unsigned int hs200_max_dtr;
    unsigned int sectors;
    unsigned int hc_erase_size;
    unsigned int hc_erase_timeout;
    unsigned int sec_trim_mult;
    unsigned int sec_erase_mult;
    unsigned int trim_timeout;
    bool partition_setting_completed;
    long long unsigned int enhanced_area_offset;
    unsigned int enhanced_area_size;
    unsigned int cache_size;
    bool hpi_en;
    bool hpi;
    unsigned int hpi_cmd;
    bool bkops;
    bool man_bkops_en;
    bool auto_bkops_en;
    unsigned int data_sector_size;
    unsigned int data_tag_unit_size;
    unsigned int boot_ro_lock;
    bool boot_ro_lockable;
    bool ffu_capable;
    bool cmdq_en;
    bool cmdq_support;
    unsigned int cmdq_depth;
    u8 fwrev[8];
    u8 raw_exception_status;
    u8 raw_partition_support;
    u8 raw_rpmb_size_mult;
    u8 raw_erased_mem_count;
    u8 strobe_support;
    u8 raw_ext_csd_structure;
    u8 raw_card_type;
    u8 raw_driver_strength;
    u8 out_of_int_time;
    u8 raw_pwr_cl_52_195;
    u8 raw_pwr_cl_26_195;
    u8 raw_pwr_cl_52_360;
    u8 raw_pwr_cl_26_360;
    u8 raw_s_a_timeout;
    u8 raw_hc_erase_gap_size;
    u8 raw_erase_timeout_mult;
    u8 raw_hc_erase_grp_size;
    u8 raw_sec_trim_mult;
    u8 raw_sec_erase_mult;
    u8 raw_sec_feature_support;
    u8 raw_trim_mult;
    u8 raw_pwr_cl_200_195;
    u8 raw_pwr_cl_200_360;
    u8 raw_pwr_cl_ddr_52_195;
    u8 raw_pwr_cl_ddr_52_360;
    u8 raw_pwr_cl_ddr_200_360;
    u8 raw_bkops_status;
    u8 raw_sectors[4];
    u8 pre_eol_info;
    u8 device_life_time_est_typ_a;
    u8 device_life_time_est_typ_b;
    unsigned int feature_support;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct mmc_ext_csd {
    u8 rev;
    u8 erase_group_def;
    u8 sec_feature_support;
    u8 rel_sectors;
    u8 rel_param;
    u8 part_config;
    u8 cache_ctrl;
    u8 rst_n_function;
    u8 max_packed_writes;
    u8 max_packed_reads;
    u8 packed_event_en;
    unsigned int part_time;
    unsigned int sa_timeout;
    unsigned int generic_cmd6_time;
    unsigned int power_off_longtime;
    u8 power_off_notification;
    unsigned int hs_max_dtr;
    unsigned int hs200_max_dtr;
    unsigned int sectors;
    unsigned int hc_erase_size;
    unsigned int hc_erase_timeout;
    unsigned int sec_trim_mult;
    unsigned int sec_erase_mult;
    unsigned int trim_timeout;
    bool partition_setting_completed;
    long long unsigned int enhanced_area_offset;
    unsigned int enhanced_area_size;
    unsigned int cache_size;
    bool hpi_en;
    bool hpi;
    unsigned int hpi_cmd;
    bool bkops;
    bool man_bkops_en;
    bool auto_bkops_en;
    unsigned int data_sector_size;
    unsigned int data_tag_unit_size;
    unsigned int boot_ro_lock;
    bool boot_ro_lockable;
    bool ffu_capable;
    bool cmdq_en;
    bool cmdq_support;
    unsigned int cmdq_depth;
    u8 fwrev[8];
    u8 raw_exception_status;
    u8 raw_partition_support;
    u8 raw_rpmb_size_mult;
    u8 raw_erased_mem_count;
    u8 strobe_support;
    u8 raw_ext_csd_structure;
    u8 raw_card_type;
    u8 raw_driver_strength;
    u8 out_of_int_time;
    u8 raw_pwr_cl_52_195;
    u8 raw_pwr_cl_26_195;
    u8 raw_pwr_cl_52_360;
    u8 raw_pwr_cl_26_360;
    u8 raw_s_a_timeout;
    u8 raw_hc_erase_gap_size;
    u8 raw_erase_timeout_mult;
    u8 raw_hc_erase_grp_size;
    u8 raw_sec_trim_mult;
    u8 raw_sec_erase_mult;
    u8 raw_sec_feature_support;
    u8 raw_trim_mult;
    u8 raw_pwr_cl_200_195;
    u8 raw_pwr_cl_200_360;
    u8 raw_pwr_cl_ddr_52_195;
    u8 raw_pwr_cl_ddr_52_360;
    u8 raw_pwr_cl_ddr_200_360;
    u8 raw_bkops_status;
    u8 raw_sectors[4];
    u8 pre_eol_info;
    u8 device_life_time_est_typ_a;
    u8 device_life_time_est_typ_b;
    unsigned int feature_support;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct mmc_ext_csd {
    u8 rev;
    u8 erase_group_def;
    u8 sec_feature_support;
    u8 rel_sectors;
    u8 rel_param;
    u8 part_config;
    u8 cache_ctrl;
    u8 rst_n_function;
    u8 max_packed_writes;
    u8 max_packed_reads;
    u8 packed_event_en;
    unsigned int part_time;
    unsigned int sa_timeout;
    unsigned int generic_cmd6_time;
    unsigned int power_off_longtime;
    u8 power_off_notification;
    unsigned int hs_max_dtr;
    unsigned int hs200_max_dtr;
    unsigned int sectors;
    unsigned int hc_erase_size;
    unsigned int hc_erase_timeout;
    unsigned int sec_trim_mult;
    unsigned int sec_erase_mult;
    unsigned int trim_timeout;
    bool partition_setting_completed;
    long long unsigned int enhanced_area_offset;
    unsigned int enhanced_area_size;
    unsigned int cache_size;
    bool hpi_en;
    bool hpi;
    unsigned int hpi_cmd;
    bool bkops;
    bool man_bkops_en;
    bool auto_bkops_en;
    unsigned int data_sector_size;
    unsigned int data_tag_unit_size;
    unsigned int boot_ro_lock;
    bool boot_ro_lockable;
    bool ffu_capable;
    bool cmdq_en;
    bool cmdq_support;
    unsigned int cmdq_depth;
    u8 fwrev[8];
    u8 raw_exception_status;
    u8 raw_partition_support;
    u8 raw_rpmb_size_mult;
    u8 raw_erased_mem_count;
    u8 strobe_support;
    u8 raw_ext_csd_structure;
    u8 raw_card_type;
    u8 raw_driver_strength;
    u8 out_of_int_time;
    u8 raw_pwr_cl_52_195;
    u8 raw_pwr_cl_26_195;
    u8 raw_pwr_cl_52_360;
    u8 raw_pwr_cl_26_360;
    u8 raw_s_a_timeout;
    u8 raw_hc_erase_gap_size;
    u8 raw_erase_timeout_mult;
    u8 raw_hc_erase_grp_size;
    u8 raw_sec_trim_mult;
    u8 raw_sec_erase_mult;
    u8 raw_sec_feature_support;
    u8 raw_trim_mult;
    u8 raw_pwr_cl_200_195;
    u8 raw_pwr_cl_200_360;
    u8 raw_pwr_cl_ddr_52_195;
    u8 raw_pwr_cl_ddr_52_360;
    u8 raw_pwr_cl_ddr_200_360;
    u8 raw_bkops_status;
    u8 raw_sectors[4];
    u8 pre_eol_info;
    u8 device_life_time_est_typ_a;
    u8 device_life_time_est_typ_b;
    unsigned int feature_support;
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
struct mmc_ext_csd {
    u8 rev;
    u8 erase_group_def;
    u8 sec_feature_support;
    u8 rel_sectors;
    u8 rel_param;
    u8 part_config;
    u8 cache_ctrl;
    u8 rst_n_function;
    u8 max_packed_writes;
    u8 max_packed_reads;
    u8 packed_event_en;
    unsigned int part_time;
    unsigned int sa_timeout;
    unsigned int generic_cmd6_time;
    unsigned int power_off_longtime;
    u8 power_off_notification;
    unsigned int hs_max_dtr;
    unsigned int hs200_max_dtr;
    unsigned int sectors;
    unsigned int hc_erase_size;
    unsigned int hc_erase_timeout;
    unsigned int sec_trim_mult;
    unsigned int sec_erase_mult;
    unsigned int trim_timeout;
    bool partition_setting_completed;
    long long unsigned int enhanced_area_offset;
    unsigned int enhanced_area_size;
    unsigned int cache_size;
    bool hpi_en;
    bool hpi;
    unsigned int hpi_cmd;
    bool bkops;
    bool man_bkops_en;
    bool auto_bkops_en;
    unsigned int data_sector_size;
    unsigned int data_tag_unit_size;
    unsigned int boot_ro_lock;
    bool boot_ro_lockable;
    bool ffu_capable;
    bool cmdq_en;
    bool cmdq_support;
    unsigned int cmdq_depth;
    u8 fwrev[8];
    u8 raw_exception_status;
    u8 raw_partition_support;
    u8 raw_rpmb_size_mult;
    u8 raw_erased_mem_count;
    u8 strobe_support;
    u8 raw_ext_csd_structure;
    u8 raw_card_type;
    u8 raw_driver_strength;
    u8 out_of_int_time;
    u8 raw_pwr_cl_52_195;
    u8 raw_pwr_cl_26_195;
    u8 raw_pwr_cl_52_360;
    u8 raw_pwr_cl_26_360;
    u8 raw_s_a_timeout;
    u8 raw_hc_erase_gap_size;
    u8 raw_erase_timeout_mult;
    u8 raw_hc_erase_grp_size;
    u8 raw_sec_trim_mult;
    u8 raw_sec_erase_mult;
    u8 raw_sec_feature_support;
    u8 raw_trim_mult;
    u8 raw_pwr_cl_200_195;
    u8 raw_pwr_cl_200_360;
    u8 raw_pwr_cl_ddr_52_195;
    u8 raw_pwr_cl_ddr_52_360;
    u8 raw_pwr_cl_ddr_200_360;
    u8 raw_bkops_status;
    u8 raw_sectors[4];
    u8 pre_eol_info;
    u8 device_life_time_est_typ_a;
    u8 device_life_time_est_typ_b;
    unsigned int feature_support;
};
```
</details>
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct mmc_ext_csd {
    u8 rev;
    u8 erase_group_def;
    u8 sec_feature_support;
    u8 rel_sectors;
    u8 rel_param;
    u8 part_config;
    u8 cache_ctrl;
    u8 rst_n_function;
    u8 max_packed_writes;
    u8 max_packed_reads;
    u8 packed_event_en;
    unsigned int part_time;
    unsigned int sa_timeout;
    unsigned int generic_cmd6_time;
    unsigned int power_off_longtime;
    u8 power_off_notification;
    unsigned int hs_max_dtr;
    unsigned int hs200_max_dtr;
    unsigned int sectors;
    unsigned int hc_erase_size;
    unsigned int hc_erase_timeout;
    unsigned int sec_trim_mult;
    unsigned int sec_erase_mult;
    unsigned int trim_timeout;
    bool partition_setting_completed;
    long long unsigned int enhanced_area_offset;
    unsigned int enhanced_area_size;
    unsigned int cache_size;
    bool hpi_en;
    bool hpi;
    unsigned int hpi_cmd;
    bool bkops;
    bool man_bkops_en;
    bool auto_bkops_en;
    unsigned int data_sector_size;
    unsigned int data_tag_unit_size;
    unsigned int boot_ro_lock;
    bool boot_ro_lockable;
    bool ffu_capable;
    bool cmdq_en;
    bool cmdq_support;
    unsigned int cmdq_depth;
    u8 fwrev[8];
    u8 raw_exception_status;
    u8 raw_partition_support;
    u8 raw_rpmb_size_mult;
    u8 raw_erased_mem_count;
    u8 strobe_support;
    u8 raw_ext_csd_structure;
    u8 raw_card_type;
    u8 raw_driver_strength;
    u8 out_of_int_time;
    u8 raw_pwr_cl_52_195;
    u8 raw_pwr_cl_26_195;
    u8 raw_pwr_cl_52_360;
    u8 raw_pwr_cl_26_360;
    u8 raw_s_a_timeout;
    u8 raw_hc_erase_gap_size;
    u8 raw_erase_timeout_mult;
    u8 raw_hc_erase_grp_size;
    u8 raw_sec_trim_mult;
    u8 raw_sec_erase_mult;
    u8 raw_sec_feature_support;
    u8 raw_trim_mult;
    u8 raw_pwr_cl_200_195;
    u8 raw_pwr_cl_200_360;
    u8 raw_pwr_cl_ddr_52_195;
    u8 raw_pwr_cl_ddr_52_360;
    u8 raw_pwr_cl_ddr_200_360;
    u8 raw_bkops_status;
    u8 raw_sectors[4];
    u8 pre_eol_info;
    u8 device_life_time_est_typ_a;
    u8 device_life_time_est_typ_b;
    unsigned int feature_support;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct mmc_ext_csd {
    u8 rev;
    u8 erase_group_def;
    u8 sec_feature_support;
    u8 rel_sectors;
    u8 rel_param;
    u8 part_config;
    u8 cache_ctrl;
    u8 rst_n_function;
    u8 max_packed_writes;
    u8 max_packed_reads;
    u8 packed_event_en;
    unsigned int part_time;
    unsigned int sa_timeout;
    unsigned int generic_cmd6_time;
    unsigned int power_off_longtime;
    u8 power_off_notification;
    unsigned int hs_max_dtr;
    unsigned int hs200_max_dtr;
    unsigned int sectors;
    unsigned int hc_erase_size;
    unsigned int hc_erase_timeout;
    unsigned int sec_trim_mult;
    unsigned int sec_erase_mult;
    unsigned int trim_timeout;
    bool partition_setting_completed;
    long long unsigned int enhanced_area_offset;
    unsigned int enhanced_area_size;
    unsigned int cache_size;
    bool hpi_en;
    bool hpi;
    unsigned int hpi_cmd;
    bool bkops;
    bool man_bkops_en;
    bool auto_bkops_en;
    unsigned int data_sector_size;
    unsigned int data_tag_unit_size;
    unsigned int boot_ro_lock;
    bool boot_ro_lockable;
    bool ffu_capable;
    bool cmdq_en;
    bool cmdq_support;
    unsigned int cmdq_depth;
    u8 fwrev[8];
    u8 raw_exception_status;
    u8 raw_partition_support;
    u8 raw_rpmb_size_mult;
    u8 raw_erased_mem_count;
    u8 strobe_support;
    u8 raw_ext_csd_structure;
    u8 raw_card_type;
    u8 raw_driver_strength;
    u8 out_of_int_time;
    u8 raw_pwr_cl_52_195;
    u8 raw_pwr_cl_26_195;
    u8 raw_pwr_cl_52_360;
    u8 raw_pwr_cl_26_360;
    u8 raw_s_a_timeout;
    u8 raw_hc_erase_gap_size;
    u8 raw_erase_timeout_mult;
    u8 raw_hc_erase_grp_size;
    u8 raw_sec_trim_mult;
    u8 raw_sec_erase_mult;
    u8 raw_sec_feature_support;
    u8 raw_trim_mult;
    u8 raw_pwr_cl_200_195;
    u8 raw_pwr_cl_200_360;
    u8 raw_pwr_cl_ddr_52_195;
    u8 raw_pwr_cl_ddr_52_360;
    u8 raw_pwr_cl_ddr_200_360;
    u8 raw_bkops_status;
    u8 raw_sectors[4];
    u8 pre_eol_info;
    u8 device_life_time_est_typ_a;
    u8 device_life_time_est_typ_b;
    unsigned int feature_support;
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
<code>u8 strobe_support</code>
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
<code>bool cmdq_support</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int cmdq_depth</code>
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
<code>bool auto_bkops_en</code>
</li>
<li>
<b>Field added. </b>
<code>bool cmdq_en</code>
</li>
<li>
<b>Field added. </b>
<code>u8 pre_eol_info</code>
</li>
<li>
<b>Field added. </b>
<code>u8 device_life_time_est_typ_a</code>
</li>
<li>
<b>Field added. </b>
<code>u8 device_life_time_est_typ_b</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
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
<code>bool enhanced_rpmb_supported</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 raw_boot_mult</code>
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
<b>Field removed. </b>
<code>u8 max_packed_writes</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 max_packed_reads</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 packed_event_en</code>
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
