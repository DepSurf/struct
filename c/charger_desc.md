# Struct: <code>charger_desc</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct charger_desc {
    const char *psy_name;
    enum polling_modes polling_mode;
    unsigned int polling_interval_ms;
    unsigned int fullbatt_vchkdrop_ms;
    unsigned int fullbatt_vchkdrop_uV;
    unsigned int fullbatt_uV;
    unsigned int fullbatt_soc;
    unsigned int fullbatt_full_capacity;
    enum data_source battery_present;
    const char **psy_charger_stat;
    int num_charger_regulators;
    struct charger_regulator *charger_regulators;
    const char *psy_fuel_gauge;
    const char *thermal_zone;
    int temp_min;
    int temp_max;
    int temp_diff;
    bool measure_battery_temp;
    u32 charging_max_duration_ms;
    u32 discharging_max_duration_ms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct charger_desc {
    const char *psy_name;
    enum polling_modes polling_mode;
    unsigned int polling_interval_ms;
    unsigned int fullbatt_vchkdrop_ms;
    unsigned int fullbatt_vchkdrop_uV;
    unsigned int fullbatt_uV;
    unsigned int fullbatt_soc;
    unsigned int fullbatt_full_capacity;
    enum data_source battery_present;
    const char **psy_charger_stat;
    int num_charger_regulators;
    struct charger_regulator *charger_regulators;
    const char *psy_fuel_gauge;
    const char *thermal_zone;
    int temp_min;
    int temp_max;
    int temp_diff;
    bool measure_battery_temp;
    u32 charging_max_duration_ms;
    u32 discharging_max_duration_ms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct charger_desc {
    const char *psy_name;
    enum polling_modes polling_mode;
    unsigned int polling_interval_ms;
    unsigned int fullbatt_vchkdrop_ms;
    unsigned int fullbatt_vchkdrop_uV;
    unsigned int fullbatt_uV;
    unsigned int fullbatt_soc;
    unsigned int fullbatt_full_capacity;
    enum data_source battery_present;
    const char **psy_charger_stat;
    int num_charger_regulators;
    struct charger_regulator *charger_regulators;
    const char *psy_fuel_gauge;
    const char *thermal_zone;
    int temp_min;
    int temp_max;
    int temp_diff;
    bool measure_battery_temp;
    u32 charging_max_duration_ms;
    u32 discharging_max_duration_ms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct charger_desc {
    const char *psy_name;
    enum polling_modes polling_mode;
    unsigned int polling_interval_ms;
    unsigned int fullbatt_vchkdrop_ms;
    unsigned int fullbatt_vchkdrop_uV;
    unsigned int fullbatt_uV;
    unsigned int fullbatt_soc;
    unsigned int fullbatt_full_capacity;
    enum data_source battery_present;
    const char **psy_charger_stat;
    int num_charger_regulators;
    struct charger_regulator *charger_regulators;
    const char *psy_fuel_gauge;
    const char *thermal_zone;
    int temp_min;
    int temp_max;
    int temp_diff;
    bool measure_battery_temp;
    u32 charging_max_duration_ms;
    u32 discharging_max_duration_ms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct charger_desc {
    const char *psy_name;
    enum polling_modes polling_mode;
    unsigned int polling_interval_ms;
    unsigned int fullbatt_vchkdrop_ms;
    unsigned int fullbatt_vchkdrop_uV;
    unsigned int fullbatt_uV;
    unsigned int fullbatt_soc;
    unsigned int fullbatt_full_capacity;
    enum data_source battery_present;
    const char **psy_charger_stat;
    int num_charger_regulators;
    struct charger_regulator *charger_regulators;
    const char *psy_fuel_gauge;
    const char *thermal_zone;
    int temp_min;
    int temp_max;
    int temp_diff;
    bool measure_battery_temp;
    u32 charging_max_duration_ms;
    u32 discharging_max_duration_ms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct charger_desc {
    const char *psy_name;
    enum polling_modes polling_mode;
    unsigned int polling_interval_ms;
    unsigned int fullbatt_vchkdrop_ms;
    unsigned int fullbatt_vchkdrop_uV;
    unsigned int fullbatt_uV;
    unsigned int fullbatt_soc;
    unsigned int fullbatt_full_capacity;
    enum data_source battery_present;
    const char **psy_charger_stat;
    int num_charger_regulators;
    struct charger_regulator *charger_regulators;
    const char *psy_fuel_gauge;
    const char *thermal_zone;
    int temp_min;
    int temp_max;
    int temp_diff;
    bool measure_battery_temp;
    u32 charging_max_duration_ms;
    u32 discharging_max_duration_ms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct charger_desc {
    const char *psy_name;
    enum polling_modes polling_mode;
    unsigned int polling_interval_ms;
    unsigned int fullbatt_vchkdrop_ms;
    unsigned int fullbatt_vchkdrop_uV;
    unsigned int fullbatt_uV;
    unsigned int fullbatt_soc;
    unsigned int fullbatt_full_capacity;
    enum data_source battery_present;
    const char **psy_charger_stat;
    int num_charger_regulators;
    struct charger_regulator *charger_regulators;
    const struct attribute_group **sysfs_groups;
    const char *psy_fuel_gauge;
    const char *thermal_zone;
    int temp_min;
    int temp_max;
    int temp_diff;
    bool measure_battery_temp;
    u32 charging_max_duration_ms;
    u32 discharging_max_duration_ms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct charger_desc {
    const char *psy_name;
    enum polling_modes polling_mode;
    unsigned int polling_interval_ms;
    unsigned int fullbatt_vchkdrop_ms;
    unsigned int fullbatt_vchkdrop_uV;
    unsigned int fullbatt_uV;
    unsigned int fullbatt_soc;
    unsigned int fullbatt_full_capacity;
    enum data_source battery_present;
    const char **psy_charger_stat;
    int num_charger_regulators;
    struct charger_regulator *charger_regulators;
    const struct attribute_group **sysfs_groups;
    const char *psy_fuel_gauge;
    const char *thermal_zone;
    int temp_min;
    int temp_max;
    int temp_diff;
    bool measure_battery_temp;
    u32 charging_max_duration_ms;
    u32 discharging_max_duration_ms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct charger_desc {
    const char *psy_name;
    enum polling_modes polling_mode;
    unsigned int polling_interval_ms;
    unsigned int fullbatt_vchkdrop_ms;
    unsigned int fullbatt_vchkdrop_uV;
    unsigned int fullbatt_uV;
    unsigned int fullbatt_soc;
    unsigned int fullbatt_full_capacity;
    enum data_source battery_present;
    const char **psy_charger_stat;
    int num_charger_regulators;
    struct charger_regulator *charger_regulators;
    const struct attribute_group **sysfs_groups;
    const char *psy_fuel_gauge;
    const char *thermal_zone;
    int temp_min;
    int temp_max;
    int temp_diff;
    bool measure_battery_temp;
    u32 charging_max_duration_ms;
    u32 discharging_max_duration_ms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct charger_desc {
    const char *psy_name;
    enum polling_modes polling_mode;
    unsigned int polling_interval_ms;
    unsigned int fullbatt_vchkdrop_ms;
    unsigned int fullbatt_vchkdrop_uV;
    unsigned int fullbatt_uV;
    unsigned int fullbatt_soc;
    unsigned int fullbatt_full_capacity;
    enum data_source battery_present;
    const char **psy_charger_stat;
    int num_charger_regulators;
    struct charger_regulator *charger_regulators;
    const struct attribute_group **sysfs_groups;
    const char *psy_fuel_gauge;
    const char *thermal_zone;
    int temp_min;
    int temp_max;
    int temp_diff;
    bool measure_battery_temp;
    u32 charging_max_duration_ms;
    u32 discharging_max_duration_ms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct charger_desc {
    const char *psy_name;
    enum polling_modes polling_mode;
    unsigned int polling_interval_ms;
    unsigned int fullbatt_vchkdrop_uV;
    unsigned int fullbatt_uV;
    unsigned int fullbatt_soc;
    unsigned int fullbatt_full_capacity;
    enum data_source battery_present;
    const char **psy_charger_stat;
    int num_charger_regulators;
    struct charger_regulator *charger_regulators;
    const struct attribute_group **sysfs_groups;
    const char *psy_fuel_gauge;
    const char *thermal_zone;
    int temp_min;
    int temp_max;
    int temp_diff;
    bool measure_battery_temp;
    u32 charging_max_duration_ms;
    u32 discharging_max_duration_ms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct charger_desc {
    const char *psy_name;
    enum polling_modes polling_mode;
    unsigned int polling_interval_ms;
    unsigned int fullbatt_vchkdrop_uV;
    unsigned int fullbatt_uV;
    unsigned int fullbatt_soc;
    unsigned int fullbatt_full_capacity;
    enum data_source battery_present;
    const char **psy_charger_stat;
    int num_charger_regulators;
    struct charger_regulator *charger_regulators;
    const struct attribute_group **sysfs_groups;
    const char *psy_fuel_gauge;
    const char *thermal_zone;
    int temp_min;
    int temp_max;
    int temp_diff;
    bool measure_battery_temp;
    u32 charging_max_duration_ms;
    u32 discharging_max_duration_ms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct charger_desc {
    const char *psy_name;
    enum polling_modes polling_mode;
    unsigned int polling_interval_ms;
    unsigned int fullbatt_vchkdrop_uV;
    unsigned int fullbatt_uV;
    unsigned int fullbatt_soc;
    unsigned int fullbatt_full_capacity;
    enum data_source battery_present;
    const char **psy_charger_stat;
    int num_charger_regulators;
    struct charger_regulator *charger_regulators;
    const struct attribute_group **sysfs_groups;
    const char *psy_fuel_gauge;
    const char *thermal_zone;
    int temp_min;
    int temp_max;
    int temp_diff;
    bool measure_battery_temp;
    u32 charging_max_duration_ms;
    u32 discharging_max_duration_ms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct charger_desc {
    const char *psy_name;
    enum polling_modes polling_mode;
    unsigned int polling_interval_ms;
    unsigned int fullbatt_vchkdrop_uV;
    unsigned int fullbatt_uV;
    unsigned int fullbatt_soc;
    unsigned int fullbatt_full_capacity;
    enum data_source battery_present;
    const char **psy_charger_stat;
    int num_charger_regulators;
    struct charger_regulator *charger_regulators;
    const struct attribute_group **sysfs_groups;
    const char *psy_fuel_gauge;
    const char *thermal_zone;
    int temp_min;
    int temp_max;
    int temp_diff;
    bool measure_battery_temp;
    u32 charging_max_duration_ms;
    u32 discharging_max_duration_ms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct charger_desc {
    const char *psy_name;
    enum polling_modes polling_mode;
    unsigned int polling_interval_ms;
    unsigned int fullbatt_vchkdrop_uV;
    unsigned int fullbatt_uV;
    unsigned int fullbatt_soc;
    unsigned int fullbatt_full_capacity;
    enum data_source battery_present;
    const char **psy_charger_stat;
    int num_charger_regulators;
    struct charger_regulator *charger_regulators;
    const struct attribute_group **sysfs_groups;
    const char *psy_fuel_gauge;
    const char *thermal_zone;
    int temp_min;
    int temp_max;
    int temp_diff;
    bool measure_battery_temp;
    u32 charging_max_duration_ms;
    u32 discharging_max_duration_ms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct charger_desc {
    const char *psy_name;
    enum polling_modes polling_mode;
    unsigned int polling_interval_ms;
    unsigned int fullbatt_vchkdrop_uV;
    unsigned int fullbatt_uV;
    unsigned int fullbatt_soc;
    unsigned int fullbatt_full_capacity;
    enum data_source battery_present;
    const char **psy_charger_stat;
    int num_charger_regulators;
    struct charger_regulator *charger_regulators;
    const struct attribute_group **sysfs_groups;
    const char *psy_fuel_gauge;
    const char *thermal_zone;
    int temp_min;
    int temp_max;
    int temp_diff;
    bool measure_battery_temp;
    u32 charging_max_duration_ms;
    u32 discharging_max_duration_ms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct charger_desc {
    const char *psy_name;
    enum polling_modes polling_mode;
    unsigned int polling_interval_ms;
    unsigned int fullbatt_vchkdrop_uV;
    unsigned int fullbatt_uV;
    unsigned int fullbatt_soc;
    unsigned int fullbatt_full_capacity;
    enum data_source battery_present;
    const char **psy_charger_stat;
    int num_charger_regulators;
    struct charger_regulator *charger_regulators;
    const struct attribute_group **sysfs_groups;
    const char *psy_fuel_gauge;
    const char *thermal_zone;
    int temp_min;
    int temp_max;
    int temp_diff;
    bool measure_battery_temp;
    u32 charging_max_duration_ms;
    u32 discharging_max_duration_ms;
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
struct charger_desc {
    const char *psy_name;
    enum polling_modes polling_mode;
    unsigned int polling_interval_ms;
    unsigned int fullbatt_vchkdrop_ms;
    unsigned int fullbatt_vchkdrop_uV;
    unsigned int fullbatt_uV;
    unsigned int fullbatt_soc;
    unsigned int fullbatt_full_capacity;
    enum data_source battery_present;
    const char **psy_charger_stat;
    int num_charger_regulators;
    struct charger_regulator *charger_regulators;
    const struct attribute_group **sysfs_groups;
    const char *psy_fuel_gauge;
    const char *thermal_zone;
    int temp_min;
    int temp_max;
    int temp_diff;
    bool measure_battery_temp;
    u32 charging_max_duration_ms;
    u32 discharging_max_duration_ms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct charger_desc {
    const char *psy_name;
    enum polling_modes polling_mode;
    unsigned int polling_interval_ms;
    unsigned int fullbatt_vchkdrop_ms;
    unsigned int fullbatt_vchkdrop_uV;
    unsigned int fullbatt_uV;
    unsigned int fullbatt_soc;
    unsigned int fullbatt_full_capacity;
    enum data_source battery_present;
    const char **psy_charger_stat;
    int num_charger_regulators;
    struct charger_regulator *charger_regulators;
    const struct attribute_group **sysfs_groups;
    const char *psy_fuel_gauge;
    const char *thermal_zone;
    int temp_min;
    int temp_max;
    int temp_diff;
    bool measure_battery_temp;
    u32 charging_max_duration_ms;
    u32 discharging_max_duration_ms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct charger_desc {
    const char *psy_name;
    enum polling_modes polling_mode;
    unsigned int polling_interval_ms;
    unsigned int fullbatt_vchkdrop_ms;
    unsigned int fullbatt_vchkdrop_uV;
    unsigned int fullbatt_uV;
    unsigned int fullbatt_soc;
    unsigned int fullbatt_full_capacity;
    enum data_source battery_present;
    const char **psy_charger_stat;
    int num_charger_regulators;
    struct charger_regulator *charger_regulators;
    const struct attribute_group **sysfs_groups;
    const char *psy_fuel_gauge;
    const char *thermal_zone;
    int temp_min;
    int temp_max;
    int temp_diff;
    bool measure_battery_temp;
    u32 charging_max_duration_ms;
    u32 discharging_max_duration_ms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct charger_desc {
    const char *psy_name;
    enum polling_modes polling_mode;
    unsigned int polling_interval_ms;
    unsigned int fullbatt_vchkdrop_ms;
    unsigned int fullbatt_vchkdrop_uV;
    unsigned int fullbatt_uV;
    unsigned int fullbatt_soc;
    unsigned int fullbatt_full_capacity;
    enum data_source battery_present;
    const char **psy_charger_stat;
    int num_charger_regulators;
    struct charger_regulator *charger_regulators;
    const struct attribute_group **sysfs_groups;
    const char *psy_fuel_gauge;
    const char *thermal_zone;
    int temp_min;
    int temp_max;
    int temp_diff;
    bool measure_battery_temp;
    u32 charging_max_duration_ms;
    u32 discharging_max_duration_ms;
};
```
</details>
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
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct charger_desc {
    const char *psy_name;
    enum polling_modes polling_mode;
    unsigned int polling_interval_ms;
    unsigned int fullbatt_vchkdrop_ms;
    unsigned int fullbatt_vchkdrop_uV;
    unsigned int fullbatt_uV;
    unsigned int fullbatt_soc;
    unsigned int fullbatt_full_capacity;
    enum data_source battery_present;
    const char **psy_charger_stat;
    int num_charger_regulators;
    struct charger_regulator *charger_regulators;
    const struct attribute_group **sysfs_groups;
    const char *psy_fuel_gauge;
    const char *thermal_zone;
    int temp_min;
    int temp_max;
    int temp_diff;
    bool measure_battery_temp;
    u32 charging_max_duration_ms;
    u32 discharging_max_duration_ms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct charger_desc {
    const char *psy_name;
    enum polling_modes polling_mode;
    unsigned int polling_interval_ms;
    unsigned int fullbatt_vchkdrop_ms;
    unsigned int fullbatt_vchkdrop_uV;
    unsigned int fullbatt_uV;
    unsigned int fullbatt_soc;
    unsigned int fullbatt_full_capacity;
    enum data_source battery_present;
    const char **psy_charger_stat;
    int num_charger_regulators;
    struct charger_regulator *charger_regulators;
    const struct attribute_group **sysfs_groups;
    const char *psy_fuel_gauge;
    const char *thermal_zone;
    int temp_min;
    int temp_max;
    int temp_diff;
    bool measure_battery_temp;
    u32 charging_max_duration_ms;
    u32 discharging_max_duration_ms;
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
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const struct attribute_group **sysfs_groups</code>
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
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned int fullbatt_vchkdrop_ms</code>
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
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
