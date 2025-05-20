# Struct: <code>power_supply_battery_info</code>

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
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct power_supply_battery_info {
    int energy_full_design_uwh;
    int charge_full_design_uah;
    int voltage_min_design_uv;
    int precharge_current_ua;
    int charge_term_current_ua;
    int constant_charge_current_max_ua;
    int constant_charge_voltage_max_uv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct power_supply_battery_info {
    int energy_full_design_uwh;
    int charge_full_design_uah;
    int voltage_min_design_uv;
    int precharge_current_ua;
    int charge_term_current_ua;
    int constant_charge_current_max_ua;
    int constant_charge_voltage_max_uv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct power_supply_battery_info {
    int energy_full_design_uwh;
    int charge_full_design_uah;
    int voltage_min_design_uv;
    int precharge_current_ua;
    int charge_term_current_ua;
    int constant_charge_current_max_ua;
    int constant_charge_voltage_max_uv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct power_supply_battery_info {
    int energy_full_design_uwh;
    int charge_full_design_uah;
    int voltage_min_design_uv;
    int precharge_current_ua;
    int charge_term_current_ua;
    int constant_charge_current_max_ua;
    int constant_charge_voltage_max_uv;
    int factory_internal_resistance_uohm;
    int ocv_temp[20];
    struct power_supply_battery_ocv_table * ocv_table[20];
    int ocv_table_size[20];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct power_supply_battery_info {
    int energy_full_design_uwh;
    int charge_full_design_uah;
    int voltage_min_design_uv;
    int voltage_max_design_uv;
    int precharge_current_ua;
    int charge_term_current_ua;
    int constant_charge_current_max_ua;
    int constant_charge_voltage_max_uv;
    int factory_internal_resistance_uohm;
    int ocv_temp[20];
    struct power_supply_battery_ocv_table * ocv_table[20];
    int ocv_table_size[20];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct power_supply_battery_info {
    int energy_full_design_uwh;
    int charge_full_design_uah;
    int voltage_min_design_uv;
    int voltage_max_design_uv;
    int precharge_current_ua;
    int charge_term_current_ua;
    int constant_charge_current_max_ua;
    int constant_charge_voltage_max_uv;
    int factory_internal_resistance_uohm;
    int ocv_temp[20];
    struct power_supply_battery_ocv_table * ocv_table[20];
    int ocv_table_size[20];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct power_supply_battery_info {
    int energy_full_design_uwh;
    int charge_full_design_uah;
    int voltage_min_design_uv;
    int voltage_max_design_uv;
    int tricklecharge_current_ua;
    int precharge_current_ua;
    int precharge_voltage_max_uv;
    int charge_term_current_ua;
    int charge_restart_voltage_uv;
    int overvoltage_limit_uv;
    int constant_charge_current_max_ua;
    int constant_charge_voltage_max_uv;
    int factory_internal_resistance_uohm;
    int ocv_temp[20];
    struct power_supply_battery_ocv_table * ocv_table[20];
    int ocv_table_size[20];
    struct power_supply_resistance_temp_table *resist_table;
    int resist_table_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct power_supply_battery_info {
    int energy_full_design_uwh;
    int charge_full_design_uah;
    int voltage_min_design_uv;
    int voltage_max_design_uv;
    int tricklecharge_current_ua;
    int precharge_current_ua;
    int precharge_voltage_max_uv;
    int charge_term_current_ua;
    int charge_restart_voltage_uv;
    int overvoltage_limit_uv;
    int constant_charge_current_max_ua;
    int constant_charge_voltage_max_uv;
    int factory_internal_resistance_uohm;
    int ocv_temp[20];
    int temp_ambient_alert_min;
    int temp_ambient_alert_max;
    int temp_alert_min;
    int temp_alert_max;
    int temp_min;
    int temp_max;
    struct power_supply_battery_ocv_table * ocv_table[20];
    int ocv_table_size[20];
    struct power_supply_resistance_temp_table *resist_table;
    int resist_table_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct power_supply_battery_info {
    int energy_full_design_uwh;
    int charge_full_design_uah;
    int voltage_min_design_uv;
    int voltage_max_design_uv;
    int tricklecharge_current_ua;
    int precharge_current_ua;
    int precharge_voltage_max_uv;
    int charge_term_current_ua;
    int charge_restart_voltage_uv;
    int overvoltage_limit_uv;
    int constant_charge_current_max_ua;
    int constant_charge_voltage_max_uv;
    int factory_internal_resistance_uohm;
    int ocv_temp[20];
    int temp_ambient_alert_min;
    int temp_ambient_alert_max;
    int temp_alert_min;
    int temp_alert_max;
    int temp_min;
    int temp_max;
    struct power_supply_battery_ocv_table * ocv_table[20];
    int ocv_table_size[20];
    struct power_supply_resistance_temp_table *resist_table;
    int resist_table_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct power_supply_battery_info {
    unsigned int technology;
    int energy_full_design_uwh;
    int charge_full_design_uah;
    int voltage_min_design_uv;
    int voltage_max_design_uv;
    int tricklecharge_current_ua;
    int precharge_current_ua;
    int precharge_voltage_max_uv;
    int charge_term_current_ua;
    int charge_restart_voltage_uv;
    int overvoltage_limit_uv;
    int constant_charge_current_max_ua;
    int constant_charge_voltage_max_uv;
    int factory_internal_resistance_uohm;
    int ocv_temp[20];
    int temp_ambient_alert_min;
    int temp_ambient_alert_max;
    int temp_alert_min;
    int temp_alert_max;
    int temp_min;
    int temp_max;
    struct power_supply_battery_ocv_table * ocv_table[20];
    int ocv_table_size[20];
    struct power_supply_resistance_temp_table *resist_table;
    int resist_table_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct power_supply_battery_info {
    unsigned int technology;
    int energy_full_design_uwh;
    int charge_full_design_uah;
    int voltage_min_design_uv;
    int voltage_max_design_uv;
    int tricklecharge_current_ua;
    int precharge_current_ua;
    int precharge_voltage_max_uv;
    int charge_term_current_ua;
    int charge_restart_voltage_uv;
    int overvoltage_limit_uv;
    int constant_charge_current_max_ua;
    int constant_charge_voltage_max_uv;
    struct power_supply_maintenance_charge_table *maintenance_charge;
    int maintenance_charge_size;
    int alert_low_temp_charge_current_ua;
    int alert_low_temp_charge_voltage_uv;
    int alert_high_temp_charge_current_ua;
    int alert_high_temp_charge_voltage_uv;
    int factory_internal_resistance_uohm;
    int factory_internal_resistance_charging_uohm;
    int ocv_temp[20];
    int temp_ambient_alert_min;
    int temp_ambient_alert_max;
    int temp_alert_min;
    int temp_alert_max;
    int temp_min;
    int temp_max;
    struct power_supply_battery_ocv_table * ocv_table[20];
    int ocv_table_size[20];
    struct power_supply_resistance_temp_table *resist_table;
    int resist_table_size;
    struct power_supply_vbat_ri_table *vbat2ri_discharging;
    int vbat2ri_discharging_size;
    struct power_supply_vbat_ri_table *vbat2ri_charging;
    int vbat2ri_charging_size;
    int bti_resistance_ohm;
    int bti_resistance_tolerance;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct power_supply_battery_info {
    unsigned int technology;
    int energy_full_design_uwh;
    int charge_full_design_uah;
    int voltage_min_design_uv;
    int voltage_max_design_uv;
    int tricklecharge_current_ua;
    int precharge_current_ua;
    int precharge_voltage_max_uv;
    int charge_term_current_ua;
    int charge_restart_voltage_uv;
    int overvoltage_limit_uv;
    int constant_charge_current_max_ua;
    int constant_charge_voltage_max_uv;
    struct power_supply_maintenance_charge_table *maintenance_charge;
    int maintenance_charge_size;
    int alert_low_temp_charge_current_ua;
    int alert_low_temp_charge_voltage_uv;
    int alert_high_temp_charge_current_ua;
    int alert_high_temp_charge_voltage_uv;
    int factory_internal_resistance_uohm;
    int factory_internal_resistance_charging_uohm;
    int ocv_temp[20];
    int temp_ambient_alert_min;
    int temp_ambient_alert_max;
    int temp_alert_min;
    int temp_alert_max;
    int temp_min;
    int temp_max;
    struct power_supply_battery_ocv_table * ocv_table[20];
    int ocv_table_size[20];
    struct power_supply_resistance_temp_table *resist_table;
    int resist_table_size;
    struct power_supply_vbat_ri_table *vbat2ri_discharging;
    int vbat2ri_discharging_size;
    struct power_supply_vbat_ri_table *vbat2ri_charging;
    int vbat2ri_charging_size;
    int bti_resistance_ohm;
    int bti_resistance_tolerance;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct power_supply_battery_info {
    unsigned int technology;
    int energy_full_design_uwh;
    int charge_full_design_uah;
    int voltage_min_design_uv;
    int voltage_max_design_uv;
    int tricklecharge_current_ua;
    int precharge_current_ua;
    int precharge_voltage_max_uv;
    int charge_term_current_ua;
    int charge_restart_voltage_uv;
    int overvoltage_limit_uv;
    int constant_charge_current_max_ua;
    int constant_charge_voltage_max_uv;
    struct power_supply_maintenance_charge_table *maintenance_charge;
    int maintenance_charge_size;
    int alert_low_temp_charge_current_ua;
    int alert_low_temp_charge_voltage_uv;
    int alert_high_temp_charge_current_ua;
    int alert_high_temp_charge_voltage_uv;
    int factory_internal_resistance_uohm;
    int factory_internal_resistance_charging_uohm;
    int ocv_temp[20];
    int temp_ambient_alert_min;
    int temp_ambient_alert_max;
    int temp_alert_min;
    int temp_alert_max;
    int temp_min;
    int temp_max;
    struct power_supply_battery_ocv_table * ocv_table[20];
    int ocv_table_size[20];
    struct power_supply_resistance_temp_table *resist_table;
    int resist_table_size;
    struct power_supply_vbat_ri_table *vbat2ri_discharging;
    int vbat2ri_discharging_size;
    struct power_supply_vbat_ri_table *vbat2ri_charging;
    int vbat2ri_charging_size;
    int bti_resistance_ohm;
    int bti_resistance_tolerance;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct power_supply_battery_info {
    unsigned int technology;
    int energy_full_design_uwh;
    int charge_full_design_uah;
    int voltage_min_design_uv;
    int voltage_max_design_uv;
    int tricklecharge_current_ua;
    int precharge_current_ua;
    int precharge_voltage_max_uv;
    int charge_term_current_ua;
    int charge_restart_voltage_uv;
    int overvoltage_limit_uv;
    int constant_charge_current_max_ua;
    int constant_charge_voltage_max_uv;
    struct power_supply_maintenance_charge_table *maintenance_charge;
    int maintenance_charge_size;
    int alert_low_temp_charge_current_ua;
    int alert_low_temp_charge_voltage_uv;
    int alert_high_temp_charge_current_ua;
    int alert_high_temp_charge_voltage_uv;
    int factory_internal_resistance_uohm;
    int factory_internal_resistance_charging_uohm;
    int ocv_temp[20];
    int temp_ambient_alert_min;
    int temp_ambient_alert_max;
    int temp_alert_min;
    int temp_alert_max;
    int temp_min;
    int temp_max;
    struct power_supply_battery_ocv_table * ocv_table[20];
    int ocv_table_size[20];
    struct power_supply_resistance_temp_table *resist_table;
    int resist_table_size;
    struct power_supply_vbat_ri_table *vbat2ri_discharging;
    int vbat2ri_discharging_size;
    struct power_supply_vbat_ri_table *vbat2ri_charging;
    int vbat2ri_charging_size;
    int bti_resistance_ohm;
    int bti_resistance_tolerance;
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
struct power_supply_battery_info {
    int energy_full_design_uwh;
    int charge_full_design_uah;
    int voltage_min_design_uv;
    int voltage_max_design_uv;
    int precharge_current_ua;
    int charge_term_current_ua;
    int constant_charge_current_max_ua;
    int constant_charge_voltage_max_uv;
    int factory_internal_resistance_uohm;
    int ocv_temp[20];
    struct power_supply_battery_ocv_table * ocv_table[20];
    int ocv_table_size[20];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct power_supply_battery_info {
    int energy_full_design_uwh;
    int charge_full_design_uah;
    int voltage_min_design_uv;
    int voltage_max_design_uv;
    int precharge_current_ua;
    int charge_term_current_ua;
    int constant_charge_current_max_ua;
    int constant_charge_voltage_max_uv;
    int factory_internal_resistance_uohm;
    int ocv_temp[20];
    struct power_supply_battery_ocv_table * ocv_table[20];
    int ocv_table_size[20];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct power_supply_battery_info {
    int energy_full_design_uwh;
    int charge_full_design_uah;
    int voltage_min_design_uv;
    int voltage_max_design_uv;
    int precharge_current_ua;
    int charge_term_current_ua;
    int constant_charge_current_max_ua;
    int constant_charge_voltage_max_uv;
    int factory_internal_resistance_uohm;
    int ocv_temp[20];
    struct power_supply_battery_ocv_table * ocv_table[20];
    int ocv_table_size[20];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct power_supply_battery_info {
    int energy_full_design_uwh;
    int charge_full_design_uah;
    int voltage_min_design_uv;
    int voltage_max_design_uv;
    int precharge_current_ua;
    int charge_term_current_ua;
    int constant_charge_current_max_ua;
    int constant_charge_voltage_max_uv;
    int factory_internal_resistance_uohm;
    int ocv_temp[20];
    struct power_supply_battery_ocv_table * ocv_table[20];
    int ocv_table_size[20];
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
struct power_supply_battery_info {
    int energy_full_design_uwh;
    int charge_full_design_uah;
    int voltage_min_design_uv;
    int voltage_max_design_uv;
    int precharge_current_ua;
    int charge_term_current_ua;
    int constant_charge_current_max_ua;
    int constant_charge_voltage_max_uv;
    int factory_internal_resistance_uohm;
    int ocv_temp[20];
    struct power_supply_battery_ocv_table * ocv_table[20];
    int ocv_table_size[20];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct power_supply_battery_info {
    int energy_full_design_uwh;
    int charge_full_design_uah;
    int voltage_min_design_uv;
    int voltage_max_design_uv;
    int precharge_current_ua;
    int charge_term_current_ua;
    int constant_charge_current_max_ua;
    int constant_charge_voltage_max_uv;
    int factory_internal_resistance_uohm;
    int ocv_temp[20];
    struct power_supply_battery_ocv_table * ocv_table[20];
    int ocv_table_size[20];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct power_supply_battery_info {
    int energy_full_design_uwh;
    int charge_full_design_uah;
    int voltage_min_design_uv;
    int voltage_max_design_uv;
    int precharge_current_ua;
    int charge_term_current_ua;
    int constant_charge_current_max_ua;
    int constant_charge_voltage_max_uv;
    int factory_internal_resistance_uohm;
    int ocv_temp[20];
    struct power_supply_battery_ocv_table * ocv_table[20];
    int ocv_table_size[20];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct power_supply_battery_info {
    int energy_full_design_uwh;
    int charge_full_design_uah;
    int voltage_min_design_uv;
    int voltage_max_design_uv;
    int precharge_current_ua;
    int charge_term_current_ua;
    int constant_charge_current_max_ua;
    int constant_charge_voltage_max_uv;
    int factory_internal_resistance_uohm;
    int ocv_temp[20];
    struct power_supply_battery_ocv_table * ocv_table[20];
    int ocv_table_size[20];
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
<code>int factory_internal_resistance_uohm</code>
</li>
<li>
<b>Field added. </b>
<code>int ocv_temp[20]</code>
</li>
<li>
<b>Field added. </b>
<code>struct power_supply_battery_ocv_table * ocv_table[20]</code>
</li>
<li>
<b>Field added. </b>
<code>int ocv_table_size[20]</code>
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
<code>int voltage_max_design_uv</code>
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
<code>int tricklecharge_current_ua</code>
</li>
<li>
<b>Field added. </b>
<code>int precharge_voltage_max_uv</code>
</li>
<li>
<b>Field added. </b>
<code>int charge_restart_voltage_uv</code>
</li>
<li>
<b>Field added. </b>
<code>int overvoltage_limit_uv</code>
</li>
<li>
<b>Field added. </b>
<code>struct power_supply_resistance_temp_table *resist_table</code>
</li>
<li>
<b>Field added. </b>
<code>int resist_table_size</code>
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
<code>int temp_ambient_alert_min</code>
</li>
<li>
<b>Field added. </b>
<code>int temp_ambient_alert_max</code>
</li>
<li>
<b>Field added. </b>
<code>int temp_alert_min</code>
</li>
<li>
<b>Field added. </b>
<code>int temp_alert_max</code>
</li>
<li>
<b>Field added. </b>
<code>int temp_min</code>
</li>
<li>
<b>Field added. </b>
<code>int temp_max</code>
</li>
</ul>
</details>
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
<code>unsigned int technology</code>
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
<code>struct power_supply_maintenance_charge_table *maintenance_charge</code>
</li>
<li>
<b>Field added. </b>
<code>int maintenance_charge_size</code>
</li>
<li>
<b>Field added. </b>
<code>int alert_low_temp_charge_current_ua</code>
</li>
<li>
<b>Field added. </b>
<code>int alert_low_temp_charge_voltage_uv</code>
</li>
<li>
<b>Field added. </b>
<code>int alert_high_temp_charge_current_ua</code>
</li>
<li>
<b>Field added. </b>
<code>int alert_high_temp_charge_voltage_uv</code>
</li>
<li>
<b>Field added. </b>
<code>int factory_internal_resistance_charging_uohm</code>
</li>
<li>
<b>Field added. </b>
<code>struct power_supply_vbat_ri_table *vbat2ri_discharging</code>
</li>
<li>
<b>Field added. </b>
<code>int vbat2ri_discharging_size</code>
</li>
<li>
<b>Field added. </b>
<code>struct power_supply_vbat_ri_table *vbat2ri_charging</code>
</li>
<li>
<b>Field added. </b>
<code>int vbat2ri_charging_size</code>
</li>
<li>
<b>Field added. </b>
<code>int bti_resistance_ohm</code>
</li>
<li>
<b>Field added. </b>
<code>int bti_resistance_tolerance</code>
</li>
</ul>
</details>
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
