# Struct: <code>acpi_battery</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct acpi_battery {
    struct mutex lock;
    struct mutex sysfs_lock;
    struct power_supply *bat;
    struct power_supply_desc bat_desc;
    struct acpi_device *device;
    struct notifier_block pm_nb;
    long unsigned int update_time;
    int revision;
    int rate_now;
    int capacity_now;
    int voltage_now;
    int design_capacity;
    int full_charge_capacity;
    int technology;
    int design_voltage;
    int design_capacity_warning;
    int design_capacity_low;
    int cycle_count;
    int measurement_accuracy;
    int max_sampling_time;
    int min_sampling_time;
    int max_averaging_interval;
    int min_averaging_interval;
    int capacity_granularity_1;
    int capacity_granularity_2;
    int alarm;
    char model_number[32];
    char serial_number[32];
    char type[32];
    char oem_info[32];
    int state;
    int power_unit;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct acpi_battery {
    struct mutex lock;
    struct mutex sysfs_lock;
    struct power_supply *bat;
    struct power_supply_desc bat_desc;
    struct acpi_device *device;
    struct notifier_block pm_nb;
    long unsigned int update_time;
    int revision;
    int rate_now;
    int capacity_now;
    int voltage_now;
    int design_capacity;
    int full_charge_capacity;
    int technology;
    int design_voltage;
    int design_capacity_warning;
    int design_capacity_low;
    int cycle_count;
    int measurement_accuracy;
    int max_sampling_time;
    int min_sampling_time;
    int max_averaging_interval;
    int min_averaging_interval;
    int capacity_granularity_1;
    int capacity_granularity_2;
    int alarm;
    char model_number[32];
    char serial_number[32];
    char type[32];
    char oem_info[32];
    int state;
    int power_unit;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct acpi_battery {
    struct mutex lock;
    struct mutex sysfs_lock;
    struct power_supply *bat;
    struct power_supply_desc bat_desc;
    struct acpi_device *device;
    struct notifier_block pm_nb;
    long unsigned int update_time;
    int revision;
    int rate_now;
    int capacity_now;
    int voltage_now;
    int design_capacity;
    int full_charge_capacity;
    int technology;
    int design_voltage;
    int design_capacity_warning;
    int design_capacity_low;
    int cycle_count;
    int measurement_accuracy;
    int max_sampling_time;
    int min_sampling_time;
    int max_averaging_interval;
    int min_averaging_interval;
    int capacity_granularity_1;
    int capacity_granularity_2;
    int alarm;
    char model_number[32];
    char serial_number[32];
    char type[32];
    char oem_info[32];
    int state;
    int power_unit;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct acpi_battery {
    struct mutex lock;
    struct mutex sysfs_lock;
    struct power_supply *bat;
    struct power_supply_desc bat_desc;
    struct acpi_device *device;
    struct notifier_block pm_nb;
    long unsigned int update_time;
    int revision;
    int rate_now;
    int capacity_now;
    int voltage_now;
    int design_capacity;
    int full_charge_capacity;
    int technology;
    int design_voltage;
    int design_capacity_warning;
    int design_capacity_low;
    int cycle_count;
    int measurement_accuracy;
    int max_sampling_time;
    int min_sampling_time;
    int max_averaging_interval;
    int min_averaging_interval;
    int capacity_granularity_1;
    int capacity_granularity_2;
    int alarm;
    char model_number[32];
    char serial_number[32];
    char type[32];
    char oem_info[32];
    int state;
    int power_unit;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct acpi_battery {
    struct mutex lock;
    struct mutex sysfs_lock;
    struct power_supply *bat;
    struct power_supply_desc bat_desc;
    struct acpi_device *device;
    struct notifier_block pm_nb;
    long unsigned int update_time;
    int revision;
    int rate_now;
    int capacity_now;
    int voltage_now;
    int design_capacity;
    int full_charge_capacity;
    int technology;
    int design_voltage;
    int design_capacity_warning;
    int design_capacity_low;
    int cycle_count;
    int measurement_accuracy;
    int max_sampling_time;
    int min_sampling_time;
    int max_averaging_interval;
    int min_averaging_interval;
    int capacity_granularity_1;
    int capacity_granularity_2;
    int alarm;
    char model_number[32];
    char serial_number[32];
    char type[32];
    char oem_info[32];
    int state;
    int power_unit;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct acpi_battery {
    struct mutex lock;
    struct mutex sysfs_lock;
    struct power_supply *bat;
    struct power_supply_desc bat_desc;
    struct acpi_device *device;
    struct notifier_block pm_nb;
    struct list_head list;
    long unsigned int update_time;
    int revision;
    int rate_now;
    int capacity_now;
    int voltage_now;
    int design_capacity;
    int full_charge_capacity;
    int technology;
    int design_voltage;
    int design_capacity_warning;
    int design_capacity_low;
    int cycle_count;
    int measurement_accuracy;
    int max_sampling_time;
    int min_sampling_time;
    int max_averaging_interval;
    int min_averaging_interval;
    int capacity_granularity_1;
    int capacity_granularity_2;
    int alarm;
    char model_number[32];
    char serial_number[32];
    char type[32];
    char oem_info[32];
    int state;
    int power_unit;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct acpi_battery {
    struct mutex lock;
    struct mutex sysfs_lock;
    struct power_supply *bat;
    struct power_supply_desc bat_desc;
    struct acpi_device *device;
    struct notifier_block pm_nb;
    struct list_head list;
    long unsigned int update_time;
    int revision;
    int rate_now;
    int capacity_now;
    int voltage_now;
    int design_capacity;
    int full_charge_capacity;
    int technology;
    int design_voltage;
    int design_capacity_warning;
    int design_capacity_low;
    int cycle_count;
    int measurement_accuracy;
    int max_sampling_time;
    int min_sampling_time;
    int max_averaging_interval;
    int min_averaging_interval;
    int capacity_granularity_1;
    int capacity_granularity_2;
    int alarm;
    char model_number[32];
    char serial_number[32];
    char type[32];
    char oem_info[32];
    int state;
    int power_unit;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct acpi_battery {
    struct mutex lock;
    struct mutex sysfs_lock;
    struct power_supply *bat;
    struct power_supply_desc bat_desc;
    struct acpi_device *device;
    struct notifier_block pm_nb;
    struct list_head list;
    long unsigned int update_time;
    int revision;
    int rate_now;
    int capacity_now;
    int voltage_now;
    int design_capacity;
    int full_charge_capacity;
    int technology;
    int design_voltage;
    int design_capacity_warning;
    int design_capacity_low;
    int cycle_count;
    int measurement_accuracy;
    int max_sampling_time;
    int min_sampling_time;
    int max_averaging_interval;
    int min_averaging_interval;
    int capacity_granularity_1;
    int capacity_granularity_2;
    int alarm;
    char model_number[32];
    char serial_number[32];
    char type[32];
    char oem_info[32];
    int state;
    int power_unit;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct acpi_battery {
    struct mutex lock;
    struct mutex sysfs_lock;
    struct power_supply *bat;
    struct power_supply_desc bat_desc;
    struct acpi_device *device;
    struct notifier_block pm_nb;
    struct list_head list;
    long unsigned int update_time;
    int revision;
    int rate_now;
    int capacity_now;
    int voltage_now;
    int design_capacity;
    int full_charge_capacity;
    int technology;
    int design_voltage;
    int design_capacity_warning;
    int design_capacity_low;
    int cycle_count;
    int measurement_accuracy;
    int max_sampling_time;
    int min_sampling_time;
    int max_averaging_interval;
    int min_averaging_interval;
    int capacity_granularity_1;
    int capacity_granularity_2;
    int alarm;
    char model_number[32];
    char serial_number[32];
    char type[32];
    char oem_info[32];
    int state;
    int power_unit;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct acpi_battery {
    struct mutex lock;
    struct mutex sysfs_lock;
    struct power_supply *bat;
    struct power_supply_desc bat_desc;
    struct acpi_device *device;
    struct notifier_block pm_nb;
    struct list_head list;
    long unsigned int update_time;
    int revision;
    int rate_now;
    int capacity_now;
    int voltage_now;
    int design_capacity;
    int full_charge_capacity;
    int technology;
    int design_voltage;
    int design_capacity_warning;
    int design_capacity_low;
    int cycle_count;
    int measurement_accuracy;
    int max_sampling_time;
    int min_sampling_time;
    int max_averaging_interval;
    int min_averaging_interval;
    int capacity_granularity_1;
    int capacity_granularity_2;
    int alarm;
    char model_number[32];
    char serial_number[32];
    char type[32];
    char oem_info[32];
    int state;
    int power_unit;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct acpi_battery {
    struct mutex lock;
    struct mutex sysfs_lock;
    struct power_supply *bat;
    struct power_supply_desc bat_desc;
    struct acpi_device *device;
    struct notifier_block pm_nb;
    struct list_head list;
    long unsigned int update_time;
    int revision;
    int rate_now;
    int capacity_now;
    int voltage_now;
    int design_capacity;
    int full_charge_capacity;
    int technology;
    int design_voltage;
    int design_capacity_warning;
    int design_capacity_low;
    int cycle_count;
    int measurement_accuracy;
    int max_sampling_time;
    int min_sampling_time;
    int max_averaging_interval;
    int min_averaging_interval;
    int capacity_granularity_1;
    int capacity_granularity_2;
    int alarm;
    char model_number[32];
    char serial_number[32];
    char type[32];
    char oem_info[32];
    int state;
    int power_unit;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct acpi_battery {
    struct mutex lock;
    struct mutex sysfs_lock;
    struct power_supply *bat;
    struct power_supply_desc bat_desc;
    struct acpi_device *device;
    struct notifier_block pm_nb;
    struct list_head list;
    long unsigned int update_time;
    int revision;
    int rate_now;
    int capacity_now;
    int voltage_now;
    int design_capacity;
    int full_charge_capacity;
    int technology;
    int design_voltage;
    int design_capacity_warning;
    int design_capacity_low;
    int cycle_count;
    int measurement_accuracy;
    int max_sampling_time;
    int min_sampling_time;
    int max_averaging_interval;
    int min_averaging_interval;
    int capacity_granularity_1;
    int capacity_granularity_2;
    int alarm;
    char model_number[32];
    char serial_number[32];
    char type[32];
    char oem_info[32];
    int state;
    int power_unit;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct acpi_battery {
    struct mutex lock;
    struct mutex sysfs_lock;
    struct power_supply *bat;
    struct power_supply_desc bat_desc;
    struct acpi_device *device;
    struct notifier_block pm_nb;
    struct list_head list;
    long unsigned int update_time;
    int revision;
    int rate_now;
    int capacity_now;
    int voltage_now;
    int design_capacity;
    int full_charge_capacity;
    int technology;
    int design_voltage;
    int design_capacity_warning;
    int design_capacity_low;
    int cycle_count;
    int measurement_accuracy;
    int max_sampling_time;
    int min_sampling_time;
    int max_averaging_interval;
    int min_averaging_interval;
    int capacity_granularity_1;
    int capacity_granularity_2;
    int alarm;
    char model_number[32];
    char serial_number[32];
    char type[32];
    char oem_info[32];
    int state;
    int power_unit;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct acpi_battery {
    struct mutex lock;
    struct mutex sysfs_lock;
    struct power_supply *bat;
    struct power_supply_desc bat_desc;
    struct acpi_device *device;
    struct notifier_block pm_nb;
    struct list_head list;
    long unsigned int update_time;
    int revision;
    int rate_now;
    int capacity_now;
    int voltage_now;
    int design_capacity;
    int full_charge_capacity;
    int technology;
    int design_voltage;
    int design_capacity_warning;
    int design_capacity_low;
    int cycle_count;
    int measurement_accuracy;
    int max_sampling_time;
    int min_sampling_time;
    int max_averaging_interval;
    int min_averaging_interval;
    int capacity_granularity_1;
    int capacity_granularity_2;
    int alarm;
    char model_number[32];
    char serial_number[32];
    char type[32];
    char oem_info[32];
    int state;
    int power_unit;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct acpi_battery {
    struct mutex lock;
    struct mutex sysfs_lock;
    struct power_supply *bat;
    struct power_supply_desc bat_desc;
    struct acpi_device *device;
    struct notifier_block pm_nb;
    struct list_head list;
    long unsigned int update_time;
    int revision;
    int rate_now;
    int capacity_now;
    int voltage_now;
    int design_capacity;
    int full_charge_capacity;
    int technology;
    int design_voltage;
    int design_capacity_warning;
    int design_capacity_low;
    int cycle_count;
    int measurement_accuracy;
    int max_sampling_time;
    int min_sampling_time;
    int max_averaging_interval;
    int min_averaging_interval;
    int capacity_granularity_1;
    int capacity_granularity_2;
    int alarm;
    char model_number[32];
    char serial_number[32];
    char type[32];
    char oem_info[32];
    int state;
    int power_unit;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct acpi_battery {
    struct mutex lock;
    struct mutex sysfs_lock;
    struct power_supply *bat;
    struct power_supply_desc bat_desc;
    struct acpi_device *device;
    struct notifier_block pm_nb;
    struct list_head list;
    long unsigned int update_time;
    int revision;
    int rate_now;
    int capacity_now;
    int voltage_now;
    int design_capacity;
    int full_charge_capacity;
    int technology;
    int design_voltage;
    int design_capacity_warning;
    int design_capacity_low;
    int cycle_count;
    int measurement_accuracy;
    int max_sampling_time;
    int min_sampling_time;
    int max_averaging_interval;
    int min_averaging_interval;
    int capacity_granularity_1;
    int capacity_granularity_2;
    int alarm;
    char model_number[64];
    char serial_number[64];
    char type[64];
    char oem_info[64];
    int state;
    int power_unit;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct acpi_battery {
    struct mutex lock;
    struct mutex sysfs_lock;
    struct power_supply *bat;
    struct power_supply_desc bat_desc;
    struct acpi_device *device;
    struct notifier_block pm_nb;
    struct list_head list;
    long unsigned int update_time;
    int revision;
    int rate_now;
    int capacity_now;
    int voltage_now;
    int design_capacity;
    int full_charge_capacity;
    int technology;
    int design_voltage;
    int design_capacity_warning;
    int design_capacity_low;
    int cycle_count;
    int measurement_accuracy;
    int max_sampling_time;
    int min_sampling_time;
    int max_averaging_interval;
    int min_averaging_interval;
    int capacity_granularity_1;
    int capacity_granularity_2;
    int alarm;
    char model_number[64];
    char serial_number[64];
    char type[64];
    char oem_info[64];
    int state;
    int power_unit;
    long unsigned int flags;
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
struct acpi_battery {
    struct mutex lock;
    struct mutex sysfs_lock;
    struct power_supply *bat;
    struct power_supply_desc bat_desc;
    struct acpi_device *device;
    struct notifier_block pm_nb;
    struct list_head list;
    long unsigned int update_time;
    int revision;
    int rate_now;
    int capacity_now;
    int voltage_now;
    int design_capacity;
    int full_charge_capacity;
    int technology;
    int design_voltage;
    int design_capacity_warning;
    int design_capacity_low;
    int cycle_count;
    int measurement_accuracy;
    int max_sampling_time;
    int min_sampling_time;
    int max_averaging_interval;
    int min_averaging_interval;
    int capacity_granularity_1;
    int capacity_granularity_2;
    int alarm;
    char model_number[32];
    char serial_number[32];
    char type[32];
    char oem_info[32];
    int state;
    int power_unit;
    long unsigned int flags;
};
```
</details>
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
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct acpi_battery {
    struct mutex lock;
    struct mutex sysfs_lock;
    struct power_supply *bat;
    struct power_supply_desc bat_desc;
    struct acpi_device *device;
    struct notifier_block pm_nb;
    struct list_head list;
    long unsigned int update_time;
    int revision;
    int rate_now;
    int capacity_now;
    int voltage_now;
    int design_capacity;
    int full_charge_capacity;
    int technology;
    int design_voltage;
    int design_capacity_warning;
    int design_capacity_low;
    int cycle_count;
    int measurement_accuracy;
    int max_sampling_time;
    int min_sampling_time;
    int max_averaging_interval;
    int min_averaging_interval;
    int capacity_granularity_1;
    int capacity_granularity_2;
    int alarm;
    char model_number[32];
    char serial_number[32];
    char type[32];
    char oem_info[32];
    int state;
    int power_unit;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct acpi_battery {
    struct mutex lock;
    struct mutex sysfs_lock;
    struct power_supply *bat;
    struct power_supply_desc bat_desc;
    struct acpi_device *device;
    struct notifier_block pm_nb;
    struct list_head list;
    long unsigned int update_time;
    int revision;
    int rate_now;
    int capacity_now;
    int voltage_now;
    int design_capacity;
    int full_charge_capacity;
    int technology;
    int design_voltage;
    int design_capacity_warning;
    int design_capacity_low;
    int cycle_count;
    int measurement_accuracy;
    int max_sampling_time;
    int min_sampling_time;
    int max_averaging_interval;
    int min_averaging_interval;
    int capacity_granularity_1;
    int capacity_granularity_2;
    int alarm;
    char model_number[32];
    char serial_number[32];
    char type[32];
    char oem_info[32];
    int state;
    int power_unit;
    long unsigned int flags;
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
<code>struct list_head list</code>
</li>
</ul>
</details>
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
No changes between <code>5.8</code> and <code>5.11</code> ✅
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>char model_number[32]</code> ➡️ <code>char model_number[64]</code>
</li>
<li>
<b>Field type changed. </b>
<code>char serial_number[32]</code> ➡️ <code>char serial_number[64]</code>
</li>
<li>
<b>Field type changed. </b>
<code>char type[32]</code> ➡️ <code>char type[64]</code>
</li>
<li>
<b>Field type changed. </b>
<code>char oem_info[32]</code> ➡️ <code>char oem_info[64]</code>
</li>
</ul>
</details>
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
