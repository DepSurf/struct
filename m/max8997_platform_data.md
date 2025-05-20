# Struct: <code>max8997_platform_data</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct max8997_platform_data {
    int ono;
    int wakeup;
    struct max8997_regulator_data *regulators;
    int num_regulators;
    bool ignore_gpiodvs_side_effect;
    int buck125_gpios[3];
    int buck125_default_idx;
    unsigned int buck1_voltage[8];
    bool buck1_gpiodvs;
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck5_voltage[8];
    bool buck5_gpiodvs;
    int eoc_mA;
    int timeout;
    struct max8997_muic_platform_data *muic_pdata;
    struct max8997_haptic_platform_data *haptic_pdata;
    struct max8997_led_platform_data *led_pdata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct max8997_platform_data {
    int ono;
    int wakeup;
    struct max8997_regulator_data *regulators;
    int num_regulators;
    bool ignore_gpiodvs_side_effect;
    int buck125_gpios[3];
    int buck125_default_idx;
    unsigned int buck1_voltage[8];
    bool buck1_gpiodvs;
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck5_voltage[8];
    bool buck5_gpiodvs;
    int eoc_mA;
    int timeout;
    struct max8997_muic_platform_data *muic_pdata;
    struct max8997_haptic_platform_data *haptic_pdata;
    struct max8997_led_platform_data *led_pdata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct max8997_platform_data {
    int ono;
    int wakeup;
    struct max8997_regulator_data *regulators;
    int num_regulators;
    bool ignore_gpiodvs_side_effect;
    int buck125_gpios[3];
    int buck125_default_idx;
    unsigned int buck1_voltage[8];
    bool buck1_gpiodvs;
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck5_voltage[8];
    bool buck5_gpiodvs;
    int eoc_mA;
    int timeout;
    struct max8997_muic_platform_data *muic_pdata;
    struct max8997_haptic_platform_data *haptic_pdata;
    struct max8997_led_platform_data *led_pdata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct max8997_platform_data {
    int ono;
    int wakeup;
    struct max8997_regulator_data *regulators;
    int num_regulators;
    bool ignore_gpiodvs_side_effect;
    int buck125_gpios[3];
    int buck125_default_idx;
    unsigned int buck1_voltage[8];
    bool buck1_gpiodvs;
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck5_voltage[8];
    bool buck5_gpiodvs;
    int eoc_mA;
    int timeout;
    struct max8997_muic_platform_data *muic_pdata;
    struct max8997_haptic_platform_data *haptic_pdata;
    struct max8997_led_platform_data *led_pdata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct max8997_platform_data {
    int ono;
    int wakeup;
    struct max8997_regulator_data *regulators;
    int num_regulators;
    bool ignore_gpiodvs_side_effect;
    int buck125_gpios[3];
    int buck125_default_idx;
    unsigned int buck1_voltage[8];
    bool buck1_gpiodvs;
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck5_voltage[8];
    bool buck5_gpiodvs;
    int eoc_mA;
    int timeout;
    struct max8997_muic_platform_data *muic_pdata;
    struct max8997_haptic_platform_data *haptic_pdata;
    struct max8997_led_platform_data *led_pdata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct max8997_platform_data {
    int ono;
    int wakeup;
    struct max8997_regulator_data *regulators;
    int num_regulators;
    bool ignore_gpiodvs_side_effect;
    int buck125_gpios[3];
    int buck125_default_idx;
    unsigned int buck1_voltage[8];
    bool buck1_gpiodvs;
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck5_voltage[8];
    bool buck5_gpiodvs;
    int eoc_mA;
    int timeout;
    struct max8997_muic_platform_data *muic_pdata;
    struct max8997_haptic_platform_data *haptic_pdata;
    struct max8997_led_platform_data *led_pdata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct max8997_platform_data {
    int ono;
    struct max8997_regulator_data *regulators;
    int num_regulators;
    bool ignore_gpiodvs_side_effect;
    int buck125_gpios[3];
    int buck125_default_idx;
    unsigned int buck1_voltage[8];
    bool buck1_gpiodvs;
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck5_voltage[8];
    bool buck5_gpiodvs;
    int eoc_mA;
    int timeout;
    struct max8997_muic_platform_data *muic_pdata;
    struct max8997_haptic_platform_data *haptic_pdata;
    struct max8997_led_platform_data *led_pdata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct max8997_platform_data {
    int ono;
    struct max8997_regulator_data *regulators;
    int num_regulators;
    bool ignore_gpiodvs_side_effect;
    int buck125_gpios[3];
    int buck125_default_idx;
    unsigned int buck1_voltage[8];
    bool buck1_gpiodvs;
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck5_voltage[8];
    bool buck5_gpiodvs;
    int eoc_mA;
    int timeout;
    struct max8997_muic_platform_data *muic_pdata;
    struct max8997_haptic_platform_data *haptic_pdata;
    struct max8997_led_platform_data *led_pdata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct max8997_platform_data {
    int ono;
    struct max8997_regulator_data *regulators;
    int num_regulators;
    bool ignore_gpiodvs_side_effect;
    int buck125_gpios[3];
    int buck125_default_idx;
    unsigned int buck1_voltage[8];
    bool buck1_gpiodvs;
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck5_voltage[8];
    bool buck5_gpiodvs;
    int eoc_mA;
    int timeout;
    struct max8997_muic_platform_data *muic_pdata;
    struct max8997_haptic_platform_data *haptic_pdata;
    struct max8997_led_platform_data *led_pdata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct max8997_platform_data {
    int ono;
    struct max8997_regulator_data *regulators;
    int num_regulators;
    bool ignore_gpiodvs_side_effect;
    int buck125_gpios[3];
    int buck125_default_idx;
    unsigned int buck1_voltage[8];
    bool buck1_gpiodvs;
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck5_voltage[8];
    bool buck5_gpiodvs;
    int eoc_mA;
    int timeout;
    struct max8997_muic_platform_data *muic_pdata;
    struct max8997_haptic_platform_data *haptic_pdata;
    struct max8997_led_platform_data *led_pdata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct max8997_platform_data {
    int ono;
    struct max8997_regulator_data *regulators;
    int num_regulators;
    bool ignore_gpiodvs_side_effect;
    int buck125_gpios[3];
    int buck125_default_idx;
    unsigned int buck1_voltage[8];
    bool buck1_gpiodvs;
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck5_voltage[8];
    bool buck5_gpiodvs;
    int eoc_mA;
    int timeout;
    struct max8997_muic_platform_data *muic_pdata;
    struct max8997_haptic_platform_data *haptic_pdata;
    struct max8997_led_platform_data *led_pdata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct max8997_platform_data {
    int ono;
    struct max8997_regulator_data *regulators;
    int num_regulators;
    bool ignore_gpiodvs_side_effect;
    int buck125_gpios[3];
    int buck125_default_idx;
    unsigned int buck1_voltage[8];
    bool buck1_gpiodvs;
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck5_voltage[8];
    bool buck5_gpiodvs;
    int eoc_mA;
    int timeout;
    struct max8997_muic_platform_data *muic_pdata;
    struct max8997_haptic_platform_data *haptic_pdata;
    struct max8997_led_platform_data *led_pdata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct max8997_platform_data {
    int ono;
    struct max8997_regulator_data *regulators;
    int num_regulators;
    bool ignore_gpiodvs_side_effect;
    int buck125_gpios[3];
    int buck125_default_idx;
    unsigned int buck1_voltage[8];
    bool buck1_gpiodvs;
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck5_voltage[8];
    bool buck5_gpiodvs;
    int eoc_mA;
    int timeout;
    struct max8997_muic_platform_data *muic_pdata;
    struct max8997_haptic_platform_data *haptic_pdata;
    struct max8997_led_platform_data *led_pdata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct max8997_platform_data {
    int ono;
    struct max8997_regulator_data *regulators;
    int num_regulators;
    bool ignore_gpiodvs_side_effect;
    int buck125_gpios[3];
    int buck125_default_idx;
    unsigned int buck1_voltage[8];
    bool buck1_gpiodvs;
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck5_voltage[8];
    bool buck5_gpiodvs;
    int eoc_mA;
    int timeout;
    struct max8997_muic_platform_data *muic_pdata;
    struct max8997_haptic_platform_data *haptic_pdata;
    struct max8997_led_platform_data *led_pdata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct max8997_platform_data {
    int ono;
    struct max8997_regulator_data *regulators;
    int num_regulators;
    bool ignore_gpiodvs_side_effect;
    int buck125_gpios[3];
    int buck125_default_idx;
    unsigned int buck1_voltage[8];
    bool buck1_gpiodvs;
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck5_voltage[8];
    bool buck5_gpiodvs;
    int eoc_mA;
    int timeout;
    struct max8997_muic_platform_data *muic_pdata;
    struct max8997_haptic_platform_data *haptic_pdata;
    struct max8997_led_platform_data *led_pdata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct max8997_platform_data {
    int ono;
    struct max8997_regulator_data *regulators;
    int num_regulators;
    bool ignore_gpiodvs_side_effect;
    int buck125_gpios[3];
    int buck125_default_idx;
    unsigned int buck1_voltage[8];
    bool buck1_gpiodvs;
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck5_voltage[8];
    bool buck5_gpiodvs;
    int eoc_mA;
    int timeout;
    struct max8997_muic_platform_data *muic_pdata;
    struct max8997_haptic_platform_data *haptic_pdata;
    struct max8997_led_platform_data *led_pdata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct max8997_platform_data {
    int ono;
    struct max8997_regulator_data *regulators;
    int num_regulators;
    bool ignore_gpiodvs_side_effect;
    int buck125_gpios[3];
    int buck125_default_idx;
    unsigned int buck1_voltage[8];
    bool buck1_gpiodvs;
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck5_voltage[8];
    bool buck5_gpiodvs;
    int eoc_mA;
    int timeout;
    struct max8997_muic_platform_data *muic_pdata;
    struct max8997_haptic_platform_data *haptic_pdata;
    struct max8997_led_platform_data *led_pdata;
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
struct max8997_platform_data {
    int ono;
    struct max8997_regulator_data *regulators;
    int num_regulators;
    bool ignore_gpiodvs_side_effect;
    int buck125_gpios[3];
    int buck125_default_idx;
    unsigned int buck1_voltage[8];
    bool buck1_gpiodvs;
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck5_voltage[8];
    bool buck5_gpiodvs;
    int eoc_mA;
    int timeout;
    struct max8997_muic_platform_data *muic_pdata;
    struct max8997_haptic_platform_data *haptic_pdata;
    struct max8997_led_platform_data *led_pdata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct max8997_platform_data {
    int ono;
    struct max8997_regulator_data *regulators;
    int num_regulators;
    bool ignore_gpiodvs_side_effect;
    int buck125_gpios[3];
    int buck125_default_idx;
    unsigned int buck1_voltage[8];
    bool buck1_gpiodvs;
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck5_voltage[8];
    bool buck5_gpiodvs;
    int eoc_mA;
    int timeout;
    struct max8997_muic_platform_data *muic_pdata;
    struct max8997_haptic_platform_data *haptic_pdata;
    struct max8997_led_platform_data *led_pdata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct max8997_platform_data {
    int ono;
    struct max8997_regulator_data *regulators;
    int num_regulators;
    bool ignore_gpiodvs_side_effect;
    int buck125_gpios[3];
    int buck125_default_idx;
    unsigned int buck1_voltage[8];
    bool buck1_gpiodvs;
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck5_voltage[8];
    bool buck5_gpiodvs;
    int eoc_mA;
    int timeout;
    struct max8997_muic_platform_data *muic_pdata;
    struct max8997_haptic_platform_data *haptic_pdata;
    struct max8997_led_platform_data *led_pdata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct max8997_platform_data {
    int ono;
    struct max8997_regulator_data *regulators;
    int num_regulators;
    bool ignore_gpiodvs_side_effect;
    int buck125_gpios[3];
    int buck125_default_idx;
    unsigned int buck1_voltage[8];
    bool buck1_gpiodvs;
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck5_voltage[8];
    bool buck5_gpiodvs;
    int eoc_mA;
    int timeout;
    struct max8997_muic_platform_data *muic_pdata;
    struct max8997_haptic_platform_data *haptic_pdata;
    struct max8997_led_platform_data *led_pdata;
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
struct max8997_platform_data {
    int ono;
    struct max8997_regulator_data *regulators;
    int num_regulators;
    bool ignore_gpiodvs_side_effect;
    int buck125_gpios[3];
    int buck125_default_idx;
    unsigned int buck1_voltage[8];
    bool buck1_gpiodvs;
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck5_voltage[8];
    bool buck5_gpiodvs;
    int eoc_mA;
    int timeout;
    struct max8997_muic_platform_data *muic_pdata;
    struct max8997_haptic_platform_data *haptic_pdata;
    struct max8997_led_platform_data *led_pdata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct max8997_platform_data {
    int ono;
    struct max8997_regulator_data *regulators;
    int num_regulators;
    bool ignore_gpiodvs_side_effect;
    int buck125_gpios[3];
    int buck125_default_idx;
    unsigned int buck1_voltage[8];
    bool buck1_gpiodvs;
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck5_voltage[8];
    bool buck5_gpiodvs;
    int eoc_mA;
    int timeout;
    struct max8997_muic_platform_data *muic_pdata;
    struct max8997_haptic_platform_data *haptic_pdata;
    struct max8997_led_platform_data *led_pdata;
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
<b>Field removed. </b>
<code>int wakeup</code>
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
