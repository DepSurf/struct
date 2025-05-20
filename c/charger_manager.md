# Struct: <code>charger_manager</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct charger_manager {
    struct list_head entry;
    struct device *dev;
    struct charger_desc *desc;
    struct thermal_zone_device *tzd_batt;
    bool charger_enabled;
    long unsigned int fullbatt_vchk_jiffies_at;
    struct delayed_work fullbatt_vchk_work;
    int emergency_stop;
    char psy_name_buf[31];
    struct power_supply_desc charger_psy_desc;
    struct power_supply *charger_psy;
    u64 charging_start_time;
    u64 charging_end_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct charger_manager {
    struct list_head entry;
    struct device *dev;
    struct charger_desc *desc;
    struct thermal_zone_device *tzd_batt;
    bool charger_enabled;
    long unsigned int fullbatt_vchk_jiffies_at;
    struct delayed_work fullbatt_vchk_work;
    int emergency_stop;
    char psy_name_buf[31];
    struct power_supply_desc charger_psy_desc;
    struct power_supply *charger_psy;
    u64 charging_start_time;
    u64 charging_end_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct charger_manager {
    struct list_head entry;
    struct device *dev;
    struct charger_desc *desc;
    struct thermal_zone_device *tzd_batt;
    bool charger_enabled;
    long unsigned int fullbatt_vchk_jiffies_at;
    struct delayed_work fullbatt_vchk_work;
    int emergency_stop;
    char psy_name_buf[31];
    struct power_supply_desc charger_psy_desc;
    struct power_supply *charger_psy;
    u64 charging_start_time;
    u64 charging_end_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct charger_manager {
    struct list_head entry;
    struct device *dev;
    struct charger_desc *desc;
    struct thermal_zone_device *tzd_batt;
    bool charger_enabled;
    long unsigned int fullbatt_vchk_jiffies_at;
    struct delayed_work fullbatt_vchk_work;
    int emergency_stop;
    char psy_name_buf[31];
    struct power_supply_desc charger_psy_desc;
    struct power_supply *charger_psy;
    u64 charging_start_time;
    u64 charging_end_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct charger_manager {
    struct list_head entry;
    struct device *dev;
    struct charger_desc *desc;
    struct thermal_zone_device *tzd_batt;
    bool charger_enabled;
    long unsigned int fullbatt_vchk_jiffies_at;
    struct delayed_work fullbatt_vchk_work;
    int emergency_stop;
    char psy_name_buf[31];
    struct power_supply_desc charger_psy_desc;
    struct power_supply *charger_psy;
    u64 charging_start_time;
    u64 charging_end_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct charger_manager {
    struct list_head entry;
    struct device *dev;
    struct charger_desc *desc;
    struct thermal_zone_device *tzd_batt;
    bool charger_enabled;
    long unsigned int fullbatt_vchk_jiffies_at;
    struct delayed_work fullbatt_vchk_work;
    int emergency_stop;
    char psy_name_buf[31];
    struct power_supply_desc charger_psy_desc;
    struct power_supply *charger_psy;
    u64 charging_start_time;
    u64 charging_end_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct charger_manager {
    struct list_head entry;
    struct device *dev;
    struct charger_desc *desc;
    struct thermal_zone_device *tzd_batt;
    bool charger_enabled;
    long unsigned int fullbatt_vchk_jiffies_at;
    struct delayed_work fullbatt_vchk_work;
    int emergency_stop;
    char psy_name_buf[31];
    struct power_supply_desc charger_psy_desc;
    struct power_supply *charger_psy;
    u64 charging_start_time;
    u64 charging_end_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct charger_manager {
    struct list_head entry;
    struct device *dev;
    struct charger_desc *desc;
    struct thermal_zone_device *tzd_batt;
    bool charger_enabled;
    long unsigned int fullbatt_vchk_jiffies_at;
    struct delayed_work fullbatt_vchk_work;
    int emergency_stop;
    char psy_name_buf[31];
    struct power_supply_desc charger_psy_desc;
    struct power_supply *charger_psy;
    u64 charging_start_time;
    u64 charging_end_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct charger_manager {
    struct list_head entry;
    struct device *dev;
    struct charger_desc *desc;
    struct thermal_zone_device *tzd_batt;
    bool charger_enabled;
    long unsigned int fullbatt_vchk_jiffies_at;
    struct delayed_work fullbatt_vchk_work;
    int emergency_stop;
    char psy_name_buf[31];
    struct power_supply_desc charger_psy_desc;
    struct power_supply *charger_psy;
    u64 charging_start_time;
    u64 charging_end_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct charger_manager {
    struct list_head entry;
    struct device *dev;
    struct charger_desc *desc;
    struct thermal_zone_device *tzd_batt;
    bool charger_enabled;
    long unsigned int fullbatt_vchk_jiffies_at;
    struct delayed_work fullbatt_vchk_work;
    int emergency_stop;
    char psy_name_buf[31];
    struct power_supply_desc charger_psy_desc;
    struct power_supply *charger_psy;
    u64 charging_start_time;
    u64 charging_end_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct charger_manager {
    struct list_head entry;
    struct device *dev;
    struct charger_desc *desc;
    struct thermal_zone_device *tzd_batt;
    bool charger_enabled;
    int emergency_stop;
    char psy_name_buf[31];
    struct power_supply_desc charger_psy_desc;
    struct power_supply *charger_psy;
    u64 charging_start_time;
    u64 charging_end_time;
    int battery_status;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct charger_manager {
    struct list_head entry;
    struct device *dev;
    struct charger_desc *desc;
    struct thermal_zone_device *tzd_batt;
    bool charger_enabled;
    int emergency_stop;
    char psy_name_buf[31];
    struct power_supply_desc charger_psy_desc;
    struct power_supply *charger_psy;
    u64 charging_start_time;
    u64 charging_end_time;
    int battery_status;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct charger_manager {
    struct list_head entry;
    struct device *dev;
    struct charger_desc *desc;
    struct thermal_zone_device *tzd_batt;
    bool charger_enabled;
    int emergency_stop;
    char psy_name_buf[31];
    struct power_supply_desc charger_psy_desc;
    struct power_supply *charger_psy;
    u64 charging_start_time;
    u64 charging_end_time;
    int battery_status;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct charger_manager {
    struct list_head entry;
    struct device *dev;
    struct charger_desc *desc;
    struct thermal_zone_device *tzd_batt;
    bool charger_enabled;
    int emergency_stop;
    char psy_name_buf[31];
    struct power_supply_desc charger_psy_desc;
    struct power_supply *charger_psy;
    u64 charging_start_time;
    u64 charging_end_time;
    int battery_status;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct charger_manager {
    struct list_head entry;
    struct device *dev;
    struct charger_desc *desc;
    struct thermal_zone_device *tzd_batt;
    bool charger_enabled;
    int emergency_stop;
    char psy_name_buf[31];
    struct power_supply_desc charger_psy_desc;
    struct power_supply *charger_psy;
    u64 charging_start_time;
    u64 charging_end_time;
    int battery_status;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct charger_manager {
    struct list_head entry;
    struct device *dev;
    struct charger_desc *desc;
    struct thermal_zone_device *tzd_batt;
    bool charger_enabled;
    int emergency_stop;
    char psy_name_buf[31];
    struct power_supply_desc charger_psy_desc;
    struct power_supply *charger_psy;
    u64 charging_start_time;
    u64 charging_end_time;
    int battery_status;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct charger_manager {
    struct list_head entry;
    struct device *dev;
    struct charger_desc *desc;
    struct thermal_zone_device *tzd_batt;
    bool charger_enabled;
    int emergency_stop;
    char psy_name_buf[31];
    struct power_supply_desc charger_psy_desc;
    struct power_supply *charger_psy;
    u64 charging_start_time;
    u64 charging_end_time;
    int battery_status;
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
struct charger_manager {
    struct list_head entry;
    struct device *dev;
    struct charger_desc *desc;
    struct thermal_zone_device *tzd_batt;
    bool charger_enabled;
    long unsigned int fullbatt_vchk_jiffies_at;
    struct delayed_work fullbatt_vchk_work;
    int emergency_stop;
    char psy_name_buf[31];
    struct power_supply_desc charger_psy_desc;
    struct power_supply *charger_psy;
    u64 charging_start_time;
    u64 charging_end_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct charger_manager {
    struct list_head entry;
    struct device *dev;
    struct charger_desc *desc;
    struct thermal_zone_device *tzd_batt;
    bool charger_enabled;
    long unsigned int fullbatt_vchk_jiffies_at;
    struct delayed_work fullbatt_vchk_work;
    int emergency_stop;
    char psy_name_buf[31];
    struct power_supply_desc charger_psy_desc;
    struct power_supply *charger_psy;
    u64 charging_start_time;
    u64 charging_end_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct charger_manager {
    struct list_head entry;
    struct device *dev;
    struct charger_desc *desc;
    struct thermal_zone_device *tzd_batt;
    bool charger_enabled;
    long unsigned int fullbatt_vchk_jiffies_at;
    struct delayed_work fullbatt_vchk_work;
    int emergency_stop;
    char psy_name_buf[31];
    struct power_supply_desc charger_psy_desc;
    struct power_supply *charger_psy;
    u64 charging_start_time;
    u64 charging_end_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct charger_manager {
    struct list_head entry;
    struct device *dev;
    struct charger_desc *desc;
    struct thermal_zone_device *tzd_batt;
    bool charger_enabled;
    long unsigned int fullbatt_vchk_jiffies_at;
    struct delayed_work fullbatt_vchk_work;
    int emergency_stop;
    char psy_name_buf[31];
    struct power_supply_desc charger_psy_desc;
    struct power_supply *charger_psy;
    u64 charging_start_time;
    u64 charging_end_time;
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
struct charger_manager {
    struct list_head entry;
    struct device *dev;
    struct charger_desc *desc;
    struct thermal_zone_device *tzd_batt;
    bool charger_enabled;
    long unsigned int fullbatt_vchk_jiffies_at;
    struct delayed_work fullbatt_vchk_work;
    int emergency_stop;
    char psy_name_buf[31];
    struct power_supply_desc charger_psy_desc;
    struct power_supply *charger_psy;
    u64 charging_start_time;
    u64 charging_end_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct charger_manager {
    struct list_head entry;
    struct device *dev;
    struct charger_desc *desc;
    struct thermal_zone_device *tzd_batt;
    bool charger_enabled;
    long unsigned int fullbatt_vchk_jiffies_at;
    struct delayed_work fullbatt_vchk_work;
    int emergency_stop;
    char psy_name_buf[31];
    struct power_supply_desc charger_psy_desc;
    struct power_supply *charger_psy;
    u64 charging_start_time;
    u64 charging_end_time;
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
No changes between <code>4.18</code> and <code>5.0</code> ✅
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
<b>Field added. </b>
<code>int battery_status</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int fullbatt_vchk_jiffies_at</code>
</li>
<li>
<b>Field removed. </b>
<code>struct delayed_work fullbatt_vchk_work</code>
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
