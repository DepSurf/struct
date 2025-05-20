# Struct: <code>intel_pmic_opregion_data</code>

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
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct intel_pmic_opregion_data {
    int (*get_power)(struct regmap *, int, int, u64 *);
    int (*update_power)(struct regmap *, int, int, bool);
    int (*get_raw_temp)(struct regmap *, int);
    int (*update_aux)(struct regmap *, int, int);
    int (*get_policy)(struct regmap *, int, int, u64 *);
    int (*update_policy)(struct regmap *, int, int, int);
    int (*exec_mipi_pmic_seq_element)(struct regmap *, u16, u32, u32, u32);
    struct pmic_table *power_table;
    int power_table_count;
    struct pmic_table *thermal_table;
    int thermal_table_count;
    int pmic_i2c_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct intel_pmic_opregion_data {
    int (*get_power)(struct regmap *, int, int, u64 *);
    int (*update_power)(struct regmap *, int, int, bool);
    int (*get_raw_temp)(struct regmap *, int);
    int (*update_aux)(struct regmap *, int, int);
    int (*get_policy)(struct regmap *, int, int, u64 *);
    int (*update_policy)(struct regmap *, int, int, int);
    int (*exec_mipi_pmic_seq_element)(struct regmap *, u16, u32, u32, u32);
    struct pmic_table *power_table;
    int power_table_count;
    struct pmic_table *thermal_table;
    int thermal_table_count;
    int pmic_i2c_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct intel_pmic_opregion_data {
    int (*get_power)(struct regmap *, int, int, u64 *);
    int (*update_power)(struct regmap *, int, int, bool);
    int (*get_raw_temp)(struct regmap *, int);
    int (*update_aux)(struct regmap *, int, int);
    int (*get_policy)(struct regmap *, int, int, u64 *);
    int (*update_policy)(struct regmap *, int, int, int);
    int (*exec_mipi_pmic_seq_element)(struct regmap *, u16, u32, u32, u32);
    struct pmic_table *power_table;
    int power_table_count;
    struct pmic_table *thermal_table;
    int thermal_table_count;
    int pmic_i2c_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct intel_pmic_opregion_data {
    int (*get_power)(struct regmap *, int, int, u64 *);
    int (*update_power)(struct regmap *, int, int, bool);
    int (*get_raw_temp)(struct regmap *, int);
    int (*update_aux)(struct regmap *, int, int);
    int (*get_policy)(struct regmap *, int, int, u64 *);
    int (*update_policy)(struct regmap *, int, int, int);
    int (*exec_mipi_pmic_seq_element)(struct regmap *, u16, u32, u32, u32);
    struct pmic_table *power_table;
    int power_table_count;
    struct pmic_table *thermal_table;
    int thermal_table_count;
    int pmic_i2c_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct intel_pmic_opregion_data {
    int (*get_power)(struct regmap *, int, int, u64 *);
    int (*update_power)(struct regmap *, int, int, bool);
    int (*get_raw_temp)(struct regmap *, int);
    int (*update_aux)(struct regmap *, int, int);
    int (*get_policy)(struct regmap *, int, int, u64 *);
    int (*update_policy)(struct regmap *, int, int, int);
    int (*exec_mipi_pmic_seq_element)(struct regmap *, u16, u32, u32, u32);
    int (*lpat_raw_to_temp)(struct acpi_lpat_conversion_table *, int);
    struct pmic_table *power_table;
    int power_table_count;
    struct pmic_table *thermal_table;
    int thermal_table_count;
    int pmic_i2c_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct intel_pmic_opregion_data {
    int (*get_power)(struct regmap *, int, int, u64 *);
    int (*update_power)(struct regmap *, int, int, bool);
    int (*get_raw_temp)(struct regmap *, int);
    int (*update_aux)(struct regmap *, int, int);
    int (*get_policy)(struct regmap *, int, int, u64 *);
    int (*update_policy)(struct regmap *, int, int, int);
    int (*exec_mipi_pmic_seq_element)(struct regmap *, u16, u32, u32, u32);
    int (*lpat_raw_to_temp)(struct acpi_lpat_conversion_table *, int);
    struct pmic_table *power_table;
    int power_table_count;
    struct pmic_table *thermal_table;
    int thermal_table_count;
    int pmic_i2c_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct intel_pmic_opregion_data {
    int (*get_power)(struct regmap *, int, int, u64 *);
    int (*update_power)(struct regmap *, int, int, bool);
    int (*get_raw_temp)(struct regmap *, int);
    int (*update_aux)(struct regmap *, int, int);
    int (*get_policy)(struct regmap *, int, int, u64 *);
    int (*update_policy)(struct regmap *, int, int, int);
    int (*exec_mipi_pmic_seq_element)(struct regmap *, u16, u32, u32, u32);
    int (*lpat_raw_to_temp)(struct acpi_lpat_conversion_table *, int);
    struct pmic_table *power_table;
    int power_table_count;
    struct pmic_table *thermal_table;
    int thermal_table_count;
    int pmic_i2c_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct intel_pmic_opregion_data {
    int (*get_power)(struct regmap *, int, int, u64 *);
    int (*update_power)(struct regmap *, int, int, bool);
    int (*get_raw_temp)(struct regmap *, int);
    int (*update_aux)(struct regmap *, int, int);
    int (*get_policy)(struct regmap *, int, int, u64 *);
    int (*update_policy)(struct regmap *, int, int, int);
    int (*exec_mipi_pmic_seq_element)(struct regmap *, u16, u32, u32, u32);
    int (*lpat_raw_to_temp)(struct acpi_lpat_conversion_table *, int);
    struct pmic_table *power_table;
    int power_table_count;
    struct pmic_table *thermal_table;
    int thermal_table_count;
    int pmic_i2c_address;
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
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*lpat_raw_to_temp)(struct acpi_lpat_conversion_table *, int)</code>
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
