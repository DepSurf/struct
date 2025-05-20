# Struct: <code>sec_platform_data</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct sec_platform_data {
    struct sec_regulator_data *regulators;
    struct sec_opmode_data *opmode;
    int device_type;
    int num_regulators;
    int irq_base;
    int (*cfg_pmic_irq)();
    bool wakeup;
    bool buck_voltage_lock;
    int buck_gpios[3];
    int buck_ds[3];
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck3_voltage[8];
    bool buck3_gpiodvs;
    unsigned int buck4_voltage[8];
    bool buck4_gpiodvs;
    int buck_set1;
    int buck_set2;
    int buck_set3;
    int buck2_enable;
    int buck3_enable;
    int buck4_enable;
    int buck_default_idx;
    int buck2_default_idx;
    int buck3_default_idx;
    int buck4_default_idx;
    int buck_ramp_delay;
    int buck2_ramp_delay;
    int buck34_ramp_delay;
    int buck5_ramp_delay;
    int buck16_ramp_delay;
    int buck7810_ramp_delay;
    int buck9_ramp_delay;
    int buck24_ramp_delay;
    int buck3_ramp_delay;
    int buck7_ramp_delay;
    int buck8910_ramp_delay;
    bool buck1_ramp_enable;
    bool buck2_ramp_enable;
    bool buck3_ramp_enable;
    bool buck4_ramp_enable;
    bool buck6_ramp_enable;
    int buck2_init;
    int buck3_init;
    int buck4_init;
    bool manual_poweroff;
    bool disable_wrstbi;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct sec_platform_data {
    struct sec_regulator_data *regulators;
    struct sec_opmode_data *opmode;
    int device_type;
    int num_regulators;
    int irq_base;
    int (*cfg_pmic_irq)();
    bool wakeup;
    bool buck_voltage_lock;
    int buck_gpios[3];
    int buck_ds[3];
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck3_voltage[8];
    bool buck3_gpiodvs;
    unsigned int buck4_voltage[8];
    bool buck4_gpiodvs;
    int buck_set1;
    int buck_set2;
    int buck_set3;
    int buck2_enable;
    int buck3_enable;
    int buck4_enable;
    int buck_default_idx;
    int buck2_default_idx;
    int buck3_default_idx;
    int buck4_default_idx;
    int buck_ramp_delay;
    int buck2_ramp_delay;
    int buck34_ramp_delay;
    int buck5_ramp_delay;
    int buck16_ramp_delay;
    int buck7810_ramp_delay;
    int buck9_ramp_delay;
    int buck24_ramp_delay;
    int buck3_ramp_delay;
    int buck7_ramp_delay;
    int buck8910_ramp_delay;
    bool buck1_ramp_enable;
    bool buck2_ramp_enable;
    bool buck3_ramp_enable;
    bool buck4_ramp_enable;
    bool buck6_ramp_enable;
    int buck2_init;
    int buck3_init;
    int buck4_init;
    bool manual_poweroff;
    bool disable_wrstbi;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct sec_platform_data {
    struct sec_regulator_data *regulators;
    struct sec_opmode_data *opmode;
    int device_type;
    int num_regulators;
    int irq_base;
    int (*cfg_pmic_irq)();
    bool wakeup;
    bool buck_voltage_lock;
    int buck_gpios[3];
    int buck_ds[3];
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck3_voltage[8];
    bool buck3_gpiodvs;
    unsigned int buck4_voltage[8];
    bool buck4_gpiodvs;
    int buck_set1;
    int buck_set2;
    int buck_set3;
    int buck2_enable;
    int buck3_enable;
    int buck4_enable;
    int buck_default_idx;
    int buck2_default_idx;
    int buck3_default_idx;
    int buck4_default_idx;
    int buck_ramp_delay;
    int buck2_ramp_delay;
    int buck34_ramp_delay;
    int buck5_ramp_delay;
    int buck16_ramp_delay;
    int buck7810_ramp_delay;
    int buck9_ramp_delay;
    int buck24_ramp_delay;
    int buck3_ramp_delay;
    int buck7_ramp_delay;
    int buck8910_ramp_delay;
    bool buck1_ramp_enable;
    bool buck2_ramp_enable;
    bool buck3_ramp_enable;
    bool buck4_ramp_enable;
    bool buck6_ramp_enable;
    int buck2_init;
    int buck3_init;
    int buck4_init;
    bool manual_poweroff;
    bool disable_wrstbi;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct sec_platform_data {
    struct sec_regulator_data *regulators;
    struct sec_opmode_data *opmode;
    int device_type;
    int num_regulators;
    int irq_base;
    int (*cfg_pmic_irq)();
    bool wakeup;
    bool buck_voltage_lock;
    int buck_gpios[3];
    int buck_ds[3];
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck3_voltage[8];
    bool buck3_gpiodvs;
    unsigned int buck4_voltage[8];
    bool buck4_gpiodvs;
    int buck_set1;
    int buck_set2;
    int buck_set3;
    int buck2_enable;
    int buck3_enable;
    int buck4_enable;
    int buck_default_idx;
    int buck2_default_idx;
    int buck3_default_idx;
    int buck4_default_idx;
    int buck_ramp_delay;
    int buck2_ramp_delay;
    int buck34_ramp_delay;
    int buck5_ramp_delay;
    int buck16_ramp_delay;
    int buck7810_ramp_delay;
    int buck9_ramp_delay;
    int buck24_ramp_delay;
    int buck3_ramp_delay;
    int buck7_ramp_delay;
    int buck8910_ramp_delay;
    bool buck1_ramp_enable;
    bool buck2_ramp_enable;
    bool buck3_ramp_enable;
    bool buck4_ramp_enable;
    bool buck6_ramp_enable;
    int buck2_init;
    int buck3_init;
    int buck4_init;
    bool manual_poweroff;
    bool disable_wrstbi;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct sec_platform_data {
    struct sec_regulator_data *regulators;
    struct sec_opmode_data *opmode;
    int device_type;
    int num_regulators;
    int irq_base;
    int (*cfg_pmic_irq)();
    bool wakeup;
    bool buck_voltage_lock;
    int buck_gpios[3];
    int buck_ds[3];
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck3_voltage[8];
    bool buck3_gpiodvs;
    unsigned int buck4_voltage[8];
    bool buck4_gpiodvs;
    int buck_set1;
    int buck_set2;
    int buck_set3;
    int buck2_enable;
    int buck3_enable;
    int buck4_enable;
    int buck_default_idx;
    int buck2_default_idx;
    int buck3_default_idx;
    int buck4_default_idx;
    int buck_ramp_delay;
    int buck2_ramp_delay;
    int buck34_ramp_delay;
    int buck5_ramp_delay;
    int buck16_ramp_delay;
    int buck7810_ramp_delay;
    int buck9_ramp_delay;
    int buck24_ramp_delay;
    int buck3_ramp_delay;
    int buck7_ramp_delay;
    int buck8910_ramp_delay;
    bool buck1_ramp_enable;
    bool buck2_ramp_enable;
    bool buck3_ramp_enable;
    bool buck4_ramp_enable;
    bool buck6_ramp_enable;
    int buck2_init;
    int buck3_init;
    int buck4_init;
    bool manual_poweroff;
    bool disable_wrstbi;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct sec_platform_data {
    struct sec_regulator_data *regulators;
    struct sec_opmode_data *opmode;
    int device_type;
    int num_regulators;
    int irq_base;
    int (*cfg_pmic_irq)();
    bool wakeup;
    bool buck_voltage_lock;
    int buck_gpios[3];
    int buck_ds[3];
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck3_voltage[8];
    bool buck3_gpiodvs;
    unsigned int buck4_voltage[8];
    bool buck4_gpiodvs;
    int buck_set1;
    int buck_set2;
    int buck_set3;
    int buck2_enable;
    int buck3_enable;
    int buck4_enable;
    int buck_default_idx;
    int buck2_default_idx;
    int buck3_default_idx;
    int buck4_default_idx;
    int buck_ramp_delay;
    int buck2_ramp_delay;
    int buck34_ramp_delay;
    int buck5_ramp_delay;
    int buck16_ramp_delay;
    int buck7810_ramp_delay;
    int buck9_ramp_delay;
    int buck24_ramp_delay;
    int buck3_ramp_delay;
    int buck7_ramp_delay;
    int buck8910_ramp_delay;
    bool buck1_ramp_enable;
    bool buck2_ramp_enable;
    bool buck3_ramp_enable;
    bool buck4_ramp_enable;
    bool buck6_ramp_enable;
    int buck2_init;
    int buck3_init;
    int buck4_init;
    bool manual_poweroff;
    bool disable_wrstbi;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct sec_platform_data {
    struct sec_regulator_data *regulators;
    struct sec_opmode_data *opmode;
    int device_type;
    int num_regulators;
    int irq_base;
    int (*cfg_pmic_irq)();
    bool wakeup;
    bool buck_voltage_lock;
    int buck_gpios[3];
    int buck_ds[3];
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck3_voltage[8];
    bool buck3_gpiodvs;
    unsigned int buck4_voltage[8];
    bool buck4_gpiodvs;
    int buck_set1;
    int buck_set2;
    int buck_set3;
    int buck2_enable;
    int buck3_enable;
    int buck4_enable;
    int buck_default_idx;
    int buck2_default_idx;
    int buck3_default_idx;
    int buck4_default_idx;
    int buck_ramp_delay;
    int buck2_ramp_delay;
    int buck34_ramp_delay;
    int buck5_ramp_delay;
    int buck16_ramp_delay;
    int buck7810_ramp_delay;
    int buck9_ramp_delay;
    int buck24_ramp_delay;
    int buck3_ramp_delay;
    int buck7_ramp_delay;
    int buck8910_ramp_delay;
    bool buck1_ramp_enable;
    bool buck2_ramp_enable;
    bool buck3_ramp_enable;
    bool buck4_ramp_enable;
    bool buck6_ramp_enable;
    int buck2_init;
    int buck3_init;
    int buck4_init;
    bool manual_poweroff;
    bool disable_wrstbi;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct sec_platform_data {
    struct sec_regulator_data *regulators;
    struct sec_opmode_data *opmode;
    int device_type;
    int num_regulators;
    int irq_base;
    int (*cfg_pmic_irq)();
    bool wakeup;
    bool buck_voltage_lock;
    int buck_gpios[3];
    int buck_ds[3];
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck3_voltage[8];
    bool buck3_gpiodvs;
    unsigned int buck4_voltage[8];
    bool buck4_gpiodvs;
    int buck_set1;
    int buck_set2;
    int buck_set3;
    int buck2_enable;
    int buck3_enable;
    int buck4_enable;
    int buck_default_idx;
    int buck2_default_idx;
    int buck3_default_idx;
    int buck4_default_idx;
    int buck_ramp_delay;
    int buck2_ramp_delay;
    int buck34_ramp_delay;
    int buck5_ramp_delay;
    int buck16_ramp_delay;
    int buck7810_ramp_delay;
    int buck9_ramp_delay;
    int buck24_ramp_delay;
    int buck3_ramp_delay;
    int buck7_ramp_delay;
    int buck8910_ramp_delay;
    bool buck1_ramp_enable;
    bool buck2_ramp_enable;
    bool buck3_ramp_enable;
    bool buck4_ramp_enable;
    bool buck6_ramp_enable;
    int buck2_init;
    int buck3_init;
    int buck4_init;
    bool manual_poweroff;
    bool disable_wrstbi;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct sec_platform_data {
    struct sec_regulator_data *regulators;
    struct sec_opmode_data *opmode;
    int device_type;
    int num_regulators;
    int irq_base;
    int (*cfg_pmic_irq)();
    bool wakeup;
    bool buck_voltage_lock;
    int buck_gpios[3];
    int buck_ds[3];
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck3_voltage[8];
    bool buck3_gpiodvs;
    unsigned int buck4_voltage[8];
    bool buck4_gpiodvs;
    int buck_set1;
    int buck_set2;
    int buck_set3;
    int buck2_enable;
    int buck3_enable;
    int buck4_enable;
    int buck_default_idx;
    int buck2_default_idx;
    int buck3_default_idx;
    int buck4_default_idx;
    int buck_ramp_delay;
    int buck2_ramp_delay;
    int buck34_ramp_delay;
    int buck5_ramp_delay;
    int buck16_ramp_delay;
    int buck7810_ramp_delay;
    int buck9_ramp_delay;
    int buck24_ramp_delay;
    int buck3_ramp_delay;
    int buck7_ramp_delay;
    int buck8910_ramp_delay;
    bool buck1_ramp_enable;
    bool buck2_ramp_enable;
    bool buck3_ramp_enable;
    bool buck4_ramp_enable;
    bool buck6_ramp_enable;
    int buck2_init;
    int buck3_init;
    int buck4_init;
    bool manual_poweroff;
    bool disable_wrstbi;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct sec_platform_data {
    struct sec_regulator_data *regulators;
    struct sec_opmode_data *opmode;
    int device_type;
    int num_regulators;
    int irq_base;
    int (*cfg_pmic_irq)();
    bool wakeup;
    bool buck_voltage_lock;
    int buck_gpios[3];
    int buck_ds[3];
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck3_voltage[8];
    bool buck3_gpiodvs;
    unsigned int buck4_voltage[8];
    bool buck4_gpiodvs;
    int buck_set1;
    int buck_set2;
    int buck_set3;
    int buck2_enable;
    int buck3_enable;
    int buck4_enable;
    int buck_default_idx;
    int buck2_default_idx;
    int buck3_default_idx;
    int buck4_default_idx;
    int buck_ramp_delay;
    int buck2_ramp_delay;
    int buck34_ramp_delay;
    int buck5_ramp_delay;
    int buck16_ramp_delay;
    int buck7810_ramp_delay;
    int buck9_ramp_delay;
    int buck24_ramp_delay;
    int buck3_ramp_delay;
    int buck7_ramp_delay;
    int buck8910_ramp_delay;
    bool buck1_ramp_enable;
    bool buck2_ramp_enable;
    bool buck3_ramp_enable;
    bool buck4_ramp_enable;
    bool buck6_ramp_enable;
    int buck2_init;
    int buck3_init;
    int buck4_init;
    bool manual_poweroff;
    bool disable_wrstbi;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct sec_platform_data {
    struct sec_regulator_data *regulators;
    struct sec_opmode_data *opmode;
    int device_type;
    int num_regulators;
    int irq_base;
    int (*cfg_pmic_irq)();
    bool wakeup;
    bool buck_voltage_lock;
    int buck_gpios[3];
    int buck_ds[3];
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck3_voltage[8];
    bool buck3_gpiodvs;
    unsigned int buck4_voltage[8];
    bool buck4_gpiodvs;
    int buck_set1;
    int buck_set2;
    int buck_set3;
    int buck2_enable;
    int buck3_enable;
    int buck4_enable;
    int buck_default_idx;
    int buck2_default_idx;
    int buck3_default_idx;
    int buck4_default_idx;
    int buck_ramp_delay;
    int buck2_ramp_delay;
    int buck34_ramp_delay;
    int buck5_ramp_delay;
    int buck16_ramp_delay;
    int buck7810_ramp_delay;
    int buck9_ramp_delay;
    int buck24_ramp_delay;
    int buck3_ramp_delay;
    int buck7_ramp_delay;
    int buck8910_ramp_delay;
    bool buck1_ramp_enable;
    bool buck2_ramp_enable;
    bool buck3_ramp_enable;
    bool buck4_ramp_enable;
    bool buck6_ramp_enable;
    int buck2_init;
    int buck3_init;
    int buck4_init;
    bool manual_poweroff;
    bool disable_wrstbi;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct sec_platform_data {
    struct sec_regulator_data *regulators;
    struct sec_opmode_data *opmode;
    int device_type;
    int num_regulators;
    int irq_base;
    int (*cfg_pmic_irq)();
    bool wakeup;
    bool buck_voltage_lock;
    int buck_gpios[3];
    int buck_ds[3];
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck3_voltage[8];
    bool buck3_gpiodvs;
    unsigned int buck4_voltage[8];
    bool buck4_gpiodvs;
    int buck_set1;
    int buck_set2;
    int buck_set3;
    int buck2_enable;
    int buck3_enable;
    int buck4_enable;
    int buck_default_idx;
    int buck2_default_idx;
    int buck3_default_idx;
    int buck4_default_idx;
    int buck_ramp_delay;
    int buck2_ramp_delay;
    int buck34_ramp_delay;
    int buck5_ramp_delay;
    int buck16_ramp_delay;
    int buck7810_ramp_delay;
    int buck9_ramp_delay;
    int buck24_ramp_delay;
    int buck3_ramp_delay;
    int buck7_ramp_delay;
    int buck8910_ramp_delay;
    bool buck1_ramp_enable;
    bool buck2_ramp_enable;
    bool buck3_ramp_enable;
    bool buck4_ramp_enable;
    bool buck6_ramp_enable;
    int buck2_init;
    int buck3_init;
    int buck4_init;
    bool manual_poweroff;
    bool disable_wrstbi;
};
```
</details>
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
In <code>5.19</code>: Absent ⚠️
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct sec_platform_data {
    struct sec_regulator_data *regulators;
    struct sec_opmode_data *opmode;
    int device_type;
    int num_regulators;
    int irq_base;
    int (*cfg_pmic_irq)();
    bool wakeup;
    bool buck_voltage_lock;
    int buck_gpios[3];
    int buck_ds[3];
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck3_voltage[8];
    bool buck3_gpiodvs;
    unsigned int buck4_voltage[8];
    bool buck4_gpiodvs;
    int buck_set1;
    int buck_set2;
    int buck_set3;
    int buck2_enable;
    int buck3_enable;
    int buck4_enable;
    int buck_default_idx;
    int buck2_default_idx;
    int buck3_default_idx;
    int buck4_default_idx;
    int buck_ramp_delay;
    int buck2_ramp_delay;
    int buck34_ramp_delay;
    int buck5_ramp_delay;
    int buck16_ramp_delay;
    int buck7810_ramp_delay;
    int buck9_ramp_delay;
    int buck24_ramp_delay;
    int buck3_ramp_delay;
    int buck7_ramp_delay;
    int buck8910_ramp_delay;
    bool buck1_ramp_enable;
    bool buck2_ramp_enable;
    bool buck3_ramp_enable;
    bool buck4_ramp_enable;
    bool buck6_ramp_enable;
    int buck2_init;
    int buck3_init;
    int buck4_init;
    bool manual_poweroff;
    bool disable_wrstbi;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct sec_platform_data {
    struct sec_regulator_data *regulators;
    struct sec_opmode_data *opmode;
    int device_type;
    int num_regulators;
    int irq_base;
    int (*cfg_pmic_irq)();
    bool wakeup;
    bool buck_voltage_lock;
    int buck_gpios[3];
    int buck_ds[3];
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck3_voltage[8];
    bool buck3_gpiodvs;
    unsigned int buck4_voltage[8];
    bool buck4_gpiodvs;
    int buck_set1;
    int buck_set2;
    int buck_set3;
    int buck2_enable;
    int buck3_enable;
    int buck4_enable;
    int buck_default_idx;
    int buck2_default_idx;
    int buck3_default_idx;
    int buck4_default_idx;
    int buck_ramp_delay;
    int buck2_ramp_delay;
    int buck34_ramp_delay;
    int buck5_ramp_delay;
    int buck16_ramp_delay;
    int buck7810_ramp_delay;
    int buck9_ramp_delay;
    int buck24_ramp_delay;
    int buck3_ramp_delay;
    int buck7_ramp_delay;
    int buck8910_ramp_delay;
    bool buck1_ramp_enable;
    bool buck2_ramp_enable;
    bool buck3_ramp_enable;
    bool buck4_ramp_enable;
    bool buck6_ramp_enable;
    int buck2_init;
    int buck3_init;
    int buck4_init;
    bool manual_poweroff;
    bool disable_wrstbi;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct sec_platform_data {
    struct sec_regulator_data *regulators;
    struct sec_opmode_data *opmode;
    int device_type;
    int num_regulators;
    int irq_base;
    int (*cfg_pmic_irq)();
    bool wakeup;
    bool buck_voltage_lock;
    int buck_gpios[3];
    int buck_ds[3];
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck3_voltage[8];
    bool buck3_gpiodvs;
    unsigned int buck4_voltage[8];
    bool buck4_gpiodvs;
    int buck_set1;
    int buck_set2;
    int buck_set3;
    int buck2_enable;
    int buck3_enable;
    int buck4_enable;
    int buck_default_idx;
    int buck2_default_idx;
    int buck3_default_idx;
    int buck4_default_idx;
    int buck_ramp_delay;
    int buck2_ramp_delay;
    int buck34_ramp_delay;
    int buck5_ramp_delay;
    int buck16_ramp_delay;
    int buck7810_ramp_delay;
    int buck9_ramp_delay;
    int buck24_ramp_delay;
    int buck3_ramp_delay;
    int buck7_ramp_delay;
    int buck8910_ramp_delay;
    bool buck1_ramp_enable;
    bool buck2_ramp_enable;
    bool buck3_ramp_enable;
    bool buck4_ramp_enable;
    bool buck6_ramp_enable;
    int buck2_init;
    int buck3_init;
    int buck4_init;
    bool manual_poweroff;
    bool disable_wrstbi;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct sec_platform_data {
    struct sec_regulator_data *regulators;
    struct sec_opmode_data *opmode;
    int device_type;
    int num_regulators;
    int irq_base;
    int (*cfg_pmic_irq)();
    bool wakeup;
    bool buck_voltage_lock;
    int buck_gpios[3];
    int buck_ds[3];
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck3_voltage[8];
    bool buck3_gpiodvs;
    unsigned int buck4_voltage[8];
    bool buck4_gpiodvs;
    int buck_set1;
    int buck_set2;
    int buck_set3;
    int buck2_enable;
    int buck3_enable;
    int buck4_enable;
    int buck_default_idx;
    int buck2_default_idx;
    int buck3_default_idx;
    int buck4_default_idx;
    int buck_ramp_delay;
    int buck2_ramp_delay;
    int buck34_ramp_delay;
    int buck5_ramp_delay;
    int buck16_ramp_delay;
    int buck7810_ramp_delay;
    int buck9_ramp_delay;
    int buck24_ramp_delay;
    int buck3_ramp_delay;
    int buck7_ramp_delay;
    int buck8910_ramp_delay;
    bool buck1_ramp_enable;
    bool buck2_ramp_enable;
    bool buck3_ramp_enable;
    bool buck4_ramp_enable;
    bool buck6_ramp_enable;
    int buck2_init;
    int buck3_init;
    int buck4_init;
    bool manual_poweroff;
    bool disable_wrstbi;
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
struct sec_platform_data {
    struct sec_regulator_data *regulators;
    struct sec_opmode_data *opmode;
    int device_type;
    int num_regulators;
    int irq_base;
    int (*cfg_pmic_irq)();
    bool wakeup;
    bool buck_voltage_lock;
    int buck_gpios[3];
    int buck_ds[3];
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck3_voltage[8];
    bool buck3_gpiodvs;
    unsigned int buck4_voltage[8];
    bool buck4_gpiodvs;
    int buck_set1;
    int buck_set2;
    int buck_set3;
    int buck2_enable;
    int buck3_enable;
    int buck4_enable;
    int buck_default_idx;
    int buck2_default_idx;
    int buck3_default_idx;
    int buck4_default_idx;
    int buck_ramp_delay;
    int buck2_ramp_delay;
    int buck34_ramp_delay;
    int buck5_ramp_delay;
    int buck16_ramp_delay;
    int buck7810_ramp_delay;
    int buck9_ramp_delay;
    int buck24_ramp_delay;
    int buck3_ramp_delay;
    int buck7_ramp_delay;
    int buck8910_ramp_delay;
    bool buck1_ramp_enable;
    bool buck2_ramp_enable;
    bool buck3_ramp_enable;
    bool buck4_ramp_enable;
    bool buck6_ramp_enable;
    int buck2_init;
    int buck3_init;
    int buck4_init;
    bool manual_poweroff;
    bool disable_wrstbi;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct sec_platform_data {
    struct sec_regulator_data *regulators;
    struct sec_opmode_data *opmode;
    int device_type;
    int num_regulators;
    int irq_base;
    int (*cfg_pmic_irq)();
    bool wakeup;
    bool buck_voltage_lock;
    int buck_gpios[3];
    int buck_ds[3];
    unsigned int buck2_voltage[8];
    bool buck2_gpiodvs;
    unsigned int buck3_voltage[8];
    bool buck3_gpiodvs;
    unsigned int buck4_voltage[8];
    bool buck4_gpiodvs;
    int buck_set1;
    int buck_set2;
    int buck_set3;
    int buck2_enable;
    int buck3_enable;
    int buck4_enable;
    int buck_default_idx;
    int buck2_default_idx;
    int buck3_default_idx;
    int buck4_default_idx;
    int buck_ramp_delay;
    int buck2_ramp_delay;
    int buck34_ramp_delay;
    int buck5_ramp_delay;
    int buck16_ramp_delay;
    int buck7810_ramp_delay;
    int buck9_ramp_delay;
    int buck24_ramp_delay;
    int buck3_ramp_delay;
    int buck7_ramp_delay;
    int buck8910_ramp_delay;
    bool buck1_ramp_enable;
    bool buck2_ramp_enable;
    bool buck3_ramp_enable;
    bool buck4_ramp_enable;
    bool buck6_ramp_enable;
    int buck2_init;
    int buck3_init;
    int buck4_init;
    bool manual_poweroff;
    bool disable_wrstbi;
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
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
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
