# Struct: <code>regulator_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct regulator_ops {
    int (*list_voltage)(struct regulator_dev *, unsigned int);
    int (*set_voltage)(struct regulator_dev *, int, int, unsigned int *);
    int (*map_voltage)(struct regulator_dev *, int, int);
    int (*set_voltage_sel)(struct regulator_dev *, unsigned int);
    int (*get_voltage)(struct regulator_dev *);
    int (*get_voltage_sel)(struct regulator_dev *);
    int (*set_current_limit)(struct regulator_dev *, int, int);
    int (*get_current_limit)(struct regulator_dev *);
    int (*set_input_current_limit)(struct regulator_dev *, int);
    int (*set_over_current_protection)(struct regulator_dev *);
    int (*enable)(struct regulator_dev *);
    int (*disable)(struct regulator_dev *);
    int (*is_enabled)(struct regulator_dev *);
    int (*set_mode)(struct regulator_dev *, unsigned int);
    unsigned int (*get_mode)(struct regulator_dev *);
    int (*enable_time)(struct regulator_dev *);
    int (*set_ramp_delay)(struct regulator_dev *, int);
    int (*set_voltage_time_sel)(struct regulator_dev *, unsigned int, unsigned int);
    int (*set_soft_start)(struct regulator_dev *);
    int (*get_status)(struct regulator_dev *);
    unsigned int (*get_optimum_mode)(struct regulator_dev *, int, int, int);
    int (*set_load)(struct regulator_dev *, int);
    int (*set_bypass)(struct regulator_dev *, bool);
    int (*get_bypass)(struct regulator_dev *, bool *);
    int (*set_suspend_voltage)(struct regulator_dev *, int);
    int (*set_suspend_enable)(struct regulator_dev *);
    int (*set_suspend_disable)(struct regulator_dev *);
    int (*set_suspend_mode)(struct regulator_dev *, unsigned int);
    int (*set_pull_down)(struct regulator_dev *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct regulator_ops {
    int (*list_voltage)(struct regulator_dev *, unsigned int);
    int (*set_voltage)(struct regulator_dev *, int, int, unsigned int *);
    int (*map_voltage)(struct regulator_dev *, int, int);
    int (*set_voltage_sel)(struct regulator_dev *, unsigned int);
    int (*get_voltage)(struct regulator_dev *);
    int (*get_voltage_sel)(struct regulator_dev *);
    int (*set_current_limit)(struct regulator_dev *, int, int);
    int (*get_current_limit)(struct regulator_dev *);
    int (*set_input_current_limit)(struct regulator_dev *, int);
    int (*set_over_current_protection)(struct regulator_dev *);
    int (*set_active_discharge)(struct regulator_dev *, bool);
    int (*enable)(struct regulator_dev *);
    int (*disable)(struct regulator_dev *);
    int (*is_enabled)(struct regulator_dev *);
    int (*set_mode)(struct regulator_dev *, unsigned int);
    unsigned int (*get_mode)(struct regulator_dev *);
    int (*enable_time)(struct regulator_dev *);
    int (*set_ramp_delay)(struct regulator_dev *, int);
    int (*set_voltage_time_sel)(struct regulator_dev *, unsigned int, unsigned int);
    int (*set_soft_start)(struct regulator_dev *);
    int (*get_status)(struct regulator_dev *);
    unsigned int (*get_optimum_mode)(struct regulator_dev *, int, int, int);
    int (*set_load)(struct regulator_dev *, int);
    int (*set_bypass)(struct regulator_dev *, bool);
    int (*get_bypass)(struct regulator_dev *, bool *);
    int (*set_suspend_voltage)(struct regulator_dev *, int);
    int (*set_suspend_enable)(struct regulator_dev *);
    int (*set_suspend_disable)(struct regulator_dev *);
    int (*set_suspend_mode)(struct regulator_dev *, unsigned int);
    int (*set_pull_down)(struct regulator_dev *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct regulator_ops {
    int (*list_voltage)(struct regulator_dev *, unsigned int);
    int (*set_voltage)(struct regulator_dev *, int, int, unsigned int *);
    int (*map_voltage)(struct regulator_dev *, int, int);
    int (*set_voltage_sel)(struct regulator_dev *, unsigned int);
    int (*get_voltage)(struct regulator_dev *);
    int (*get_voltage_sel)(struct regulator_dev *);
    int (*set_current_limit)(struct regulator_dev *, int, int);
    int (*get_current_limit)(struct regulator_dev *);
    int (*set_input_current_limit)(struct regulator_dev *, int);
    int (*set_over_current_protection)(struct regulator_dev *);
    int (*set_active_discharge)(struct regulator_dev *, bool);
    int (*enable)(struct regulator_dev *);
    int (*disable)(struct regulator_dev *);
    int (*is_enabled)(struct regulator_dev *);
    int (*set_mode)(struct regulator_dev *, unsigned int);
    unsigned int (*get_mode)(struct regulator_dev *);
    int (*get_error_flags)(struct regulator_dev *, unsigned int *);
    int (*enable_time)(struct regulator_dev *);
    int (*set_ramp_delay)(struct regulator_dev *, int);
    int (*set_voltage_time)(struct regulator_dev *, int, int);
    int (*set_voltage_time_sel)(struct regulator_dev *, unsigned int, unsigned int);
    int (*set_soft_start)(struct regulator_dev *);
    int (*get_status)(struct regulator_dev *);
    unsigned int (*get_optimum_mode)(struct regulator_dev *, int, int, int);
    int (*set_load)(struct regulator_dev *, int);
    int (*set_bypass)(struct regulator_dev *, bool);
    int (*get_bypass)(struct regulator_dev *, bool *);
    int (*set_suspend_voltage)(struct regulator_dev *, int);
    int (*set_suspend_enable)(struct regulator_dev *);
    int (*set_suspend_disable)(struct regulator_dev *);
    int (*set_suspend_mode)(struct regulator_dev *, unsigned int);
    int (*set_pull_down)(struct regulator_dev *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct regulator_ops {
    int (*list_voltage)(struct regulator_dev *, unsigned int);
    int (*set_voltage)(struct regulator_dev *, int, int, unsigned int *);
    int (*map_voltage)(struct regulator_dev *, int, int);
    int (*set_voltage_sel)(struct regulator_dev *, unsigned int);
    int (*get_voltage)(struct regulator_dev *);
    int (*get_voltage_sel)(struct regulator_dev *);
    int (*set_current_limit)(struct regulator_dev *, int, int);
    int (*get_current_limit)(struct regulator_dev *);
    int (*set_input_current_limit)(struct regulator_dev *, int);
    int (*set_over_current_protection)(struct regulator_dev *);
    int (*set_active_discharge)(struct regulator_dev *, bool);
    int (*enable)(struct regulator_dev *);
    int (*disable)(struct regulator_dev *);
    int (*is_enabled)(struct regulator_dev *);
    int (*set_mode)(struct regulator_dev *, unsigned int);
    unsigned int (*get_mode)(struct regulator_dev *);
    int (*get_error_flags)(struct regulator_dev *, unsigned int *);
    int (*enable_time)(struct regulator_dev *);
    int (*set_ramp_delay)(struct regulator_dev *, int);
    int (*set_voltage_time)(struct regulator_dev *, int, int);
    int (*set_voltage_time_sel)(struct regulator_dev *, unsigned int, unsigned int);
    int (*set_soft_start)(struct regulator_dev *);
    int (*get_status)(struct regulator_dev *);
    unsigned int (*get_optimum_mode)(struct regulator_dev *, int, int, int);
    int (*set_load)(struct regulator_dev *, int);
    int (*set_bypass)(struct regulator_dev *, bool);
    int (*get_bypass)(struct regulator_dev *, bool *);
    int (*set_suspend_voltage)(struct regulator_dev *, int);
    int (*set_suspend_enable)(struct regulator_dev *);
    int (*set_suspend_disable)(struct regulator_dev *);
    int (*set_suspend_mode)(struct regulator_dev *, unsigned int);
    int (*set_pull_down)(struct regulator_dev *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct regulator_ops {
    int (*list_voltage)(struct regulator_dev *, unsigned int);
    int (*set_voltage)(struct regulator_dev *, int, int, unsigned int *);
    int (*map_voltage)(struct regulator_dev *, int, int);
    int (*set_voltage_sel)(struct regulator_dev *, unsigned int);
    int (*get_voltage)(struct regulator_dev *);
    int (*get_voltage_sel)(struct regulator_dev *);
    int (*set_current_limit)(struct regulator_dev *, int, int);
    int (*get_current_limit)(struct regulator_dev *);
    int (*set_input_current_limit)(struct regulator_dev *, int);
    int (*set_over_current_protection)(struct regulator_dev *);
    int (*set_active_discharge)(struct regulator_dev *, bool);
    int (*enable)(struct regulator_dev *);
    int (*disable)(struct regulator_dev *);
    int (*is_enabled)(struct regulator_dev *);
    int (*set_mode)(struct regulator_dev *, unsigned int);
    unsigned int (*get_mode)(struct regulator_dev *);
    int (*get_error_flags)(struct regulator_dev *, unsigned int *);
    int (*enable_time)(struct regulator_dev *);
    int (*set_ramp_delay)(struct regulator_dev *, int);
    int (*set_voltage_time)(struct regulator_dev *, int, int);
    int (*set_voltage_time_sel)(struct regulator_dev *, unsigned int, unsigned int);
    int (*set_soft_start)(struct regulator_dev *);
    int (*get_status)(struct regulator_dev *);
    unsigned int (*get_optimum_mode)(struct regulator_dev *, int, int, int);
    int (*set_load)(struct regulator_dev *, int);
    int (*set_bypass)(struct regulator_dev *, bool);
    int (*get_bypass)(struct regulator_dev *, bool *);
    int (*set_suspend_voltage)(struct regulator_dev *, int);
    int (*set_suspend_enable)(struct regulator_dev *);
    int (*set_suspend_disable)(struct regulator_dev *);
    int (*set_suspend_mode)(struct regulator_dev *, unsigned int);
    int (*set_pull_down)(struct regulator_dev *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct regulator_ops {
    int (*list_voltage)(struct regulator_dev *, unsigned int);
    int (*set_voltage)(struct regulator_dev *, int, int, unsigned int *);
    int (*map_voltage)(struct regulator_dev *, int, int);
    int (*set_voltage_sel)(struct regulator_dev *, unsigned int);
    int (*get_voltage)(struct regulator_dev *);
    int (*get_voltage_sel)(struct regulator_dev *);
    int (*set_current_limit)(struct regulator_dev *, int, int);
    int (*get_current_limit)(struct regulator_dev *);
    int (*set_input_current_limit)(struct regulator_dev *, int);
    int (*set_over_current_protection)(struct regulator_dev *);
    int (*set_active_discharge)(struct regulator_dev *, bool);
    int (*enable)(struct regulator_dev *);
    int (*disable)(struct regulator_dev *);
    int (*is_enabled)(struct regulator_dev *);
    int (*set_mode)(struct regulator_dev *, unsigned int);
    unsigned int (*get_mode)(struct regulator_dev *);
    int (*get_error_flags)(struct regulator_dev *, unsigned int *);
    int (*enable_time)(struct regulator_dev *);
    int (*set_ramp_delay)(struct regulator_dev *, int);
    int (*set_voltage_time)(struct regulator_dev *, int, int);
    int (*set_voltage_time_sel)(struct regulator_dev *, unsigned int, unsigned int);
    int (*set_soft_start)(struct regulator_dev *);
    int (*get_status)(struct regulator_dev *);
    unsigned int (*get_optimum_mode)(struct regulator_dev *, int, int, int);
    int (*set_load)(struct regulator_dev *, int);
    int (*set_bypass)(struct regulator_dev *, bool);
    int (*get_bypass)(struct regulator_dev *, bool *);
    int (*set_suspend_voltage)(struct regulator_dev *, int);
    int (*set_suspend_enable)(struct regulator_dev *);
    int (*set_suspend_disable)(struct regulator_dev *);
    int (*set_suspend_mode)(struct regulator_dev *, unsigned int);
    int (*resume_early)(struct regulator_dev *);
    int (*set_pull_down)(struct regulator_dev *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct regulator_ops {
    int (*list_voltage)(struct regulator_dev *, unsigned int);
    int (*set_voltage)(struct regulator_dev *, int, int, unsigned int *);
    int (*map_voltage)(struct regulator_dev *, int, int);
    int (*set_voltage_sel)(struct regulator_dev *, unsigned int);
    int (*get_voltage)(struct regulator_dev *);
    int (*get_voltage_sel)(struct regulator_dev *);
    int (*set_current_limit)(struct regulator_dev *, int, int);
    int (*get_current_limit)(struct regulator_dev *);
    int (*set_input_current_limit)(struct regulator_dev *, int);
    int (*set_over_current_protection)(struct regulator_dev *);
    int (*set_active_discharge)(struct regulator_dev *, bool);
    int (*enable)(struct regulator_dev *);
    int (*disable)(struct regulator_dev *);
    int (*is_enabled)(struct regulator_dev *);
    int (*set_mode)(struct regulator_dev *, unsigned int);
    unsigned int (*get_mode)(struct regulator_dev *);
    int (*get_error_flags)(struct regulator_dev *, unsigned int *);
    int (*enable_time)(struct regulator_dev *);
    int (*set_ramp_delay)(struct regulator_dev *, int);
    int (*set_voltage_time)(struct regulator_dev *, int, int);
    int (*set_voltage_time_sel)(struct regulator_dev *, unsigned int, unsigned int);
    int (*set_soft_start)(struct regulator_dev *);
    int (*get_status)(struct regulator_dev *);
    unsigned int (*get_optimum_mode)(struct regulator_dev *, int, int, int);
    int (*set_load)(struct regulator_dev *, int);
    int (*set_bypass)(struct regulator_dev *, bool);
    int (*get_bypass)(struct regulator_dev *, bool *);
    int (*set_suspend_voltage)(struct regulator_dev *, int);
    int (*set_suspend_enable)(struct regulator_dev *);
    int (*set_suspend_disable)(struct regulator_dev *);
    int (*set_suspend_mode)(struct regulator_dev *, unsigned int);
    int (*resume)(struct regulator_dev *);
    int (*set_pull_down)(struct regulator_dev *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct regulator_ops {
    int (*list_voltage)(struct regulator_dev *, unsigned int);
    int (*set_voltage)(struct regulator_dev *, int, int, unsigned int *);
    int (*map_voltage)(struct regulator_dev *, int, int);
    int (*set_voltage_sel)(struct regulator_dev *, unsigned int);
    int (*get_voltage)(struct regulator_dev *);
    int (*get_voltage_sel)(struct regulator_dev *);
    int (*set_current_limit)(struct regulator_dev *, int, int);
    int (*get_current_limit)(struct regulator_dev *);
    int (*set_input_current_limit)(struct regulator_dev *, int);
    int (*set_over_current_protection)(struct regulator_dev *);
    int (*set_active_discharge)(struct regulator_dev *, bool);
    int (*enable)(struct regulator_dev *);
    int (*disable)(struct regulator_dev *);
    int (*is_enabled)(struct regulator_dev *);
    int (*set_mode)(struct regulator_dev *, unsigned int);
    unsigned int (*get_mode)(struct regulator_dev *);
    int (*get_error_flags)(struct regulator_dev *, unsigned int *);
    int (*enable_time)(struct regulator_dev *);
    int (*set_ramp_delay)(struct regulator_dev *, int);
    int (*set_voltage_time)(struct regulator_dev *, int, int);
    int (*set_voltage_time_sel)(struct regulator_dev *, unsigned int, unsigned int);
    int (*set_soft_start)(struct regulator_dev *);
    int (*get_status)(struct regulator_dev *);
    unsigned int (*get_optimum_mode)(struct regulator_dev *, int, int, int);
    int (*set_load)(struct regulator_dev *, int);
    int (*set_bypass)(struct regulator_dev *, bool);
    int (*get_bypass)(struct regulator_dev *, bool *);
    int (*set_suspend_voltage)(struct regulator_dev *, int);
    int (*set_suspend_enable)(struct regulator_dev *);
    int (*set_suspend_disable)(struct regulator_dev *);
    int (*set_suspend_mode)(struct regulator_dev *, unsigned int);
    int (*resume)(struct regulator_dev *);
    int (*set_pull_down)(struct regulator_dev *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct regulator_ops {
    int (*list_voltage)(struct regulator_dev *, unsigned int);
    int (*set_voltage)(struct regulator_dev *, int, int, unsigned int *);
    int (*map_voltage)(struct regulator_dev *, int, int);
    int (*set_voltage_sel)(struct regulator_dev *, unsigned int);
    int (*get_voltage)(struct regulator_dev *);
    int (*get_voltage_sel)(struct regulator_dev *);
    int (*set_current_limit)(struct regulator_dev *, int, int);
    int (*get_current_limit)(struct regulator_dev *);
    int (*set_input_current_limit)(struct regulator_dev *, int);
    int (*set_over_current_protection)(struct regulator_dev *);
    int (*set_active_discharge)(struct regulator_dev *, bool);
    int (*enable)(struct regulator_dev *);
    int (*disable)(struct regulator_dev *);
    int (*is_enabled)(struct regulator_dev *);
    int (*set_mode)(struct regulator_dev *, unsigned int);
    unsigned int (*get_mode)(struct regulator_dev *);
    int (*get_error_flags)(struct regulator_dev *, unsigned int *);
    int (*enable_time)(struct regulator_dev *);
    int (*set_ramp_delay)(struct regulator_dev *, int);
    int (*set_voltage_time)(struct regulator_dev *, int, int);
    int (*set_voltage_time_sel)(struct regulator_dev *, unsigned int, unsigned int);
    int (*set_soft_start)(struct regulator_dev *);
    int (*get_status)(struct regulator_dev *);
    unsigned int (*get_optimum_mode)(struct regulator_dev *, int, int, int);
    int (*set_load)(struct regulator_dev *, int);
    int (*set_bypass)(struct regulator_dev *, bool);
    int (*get_bypass)(struct regulator_dev *, bool *);
    int (*set_suspend_voltage)(struct regulator_dev *, int);
    int (*set_suspend_enable)(struct regulator_dev *);
    int (*set_suspend_disable)(struct regulator_dev *);
    int (*set_suspend_mode)(struct regulator_dev *, unsigned int);
    int (*resume)(struct regulator_dev *);
    int (*set_pull_down)(struct regulator_dev *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct regulator_ops {
    int (*list_voltage)(struct regulator_dev *, unsigned int);
    int (*set_voltage)(struct regulator_dev *, int, int, unsigned int *);
    int (*map_voltage)(struct regulator_dev *, int, int);
    int (*set_voltage_sel)(struct regulator_dev *, unsigned int);
    int (*get_voltage)(struct regulator_dev *);
    int (*get_voltage_sel)(struct regulator_dev *);
    int (*set_current_limit)(struct regulator_dev *, int, int);
    int (*get_current_limit)(struct regulator_dev *);
    int (*set_input_current_limit)(struct regulator_dev *, int);
    int (*set_over_current_protection)(struct regulator_dev *);
    int (*set_active_discharge)(struct regulator_dev *, bool);
    int (*enable)(struct regulator_dev *);
    int (*disable)(struct regulator_dev *);
    int (*is_enabled)(struct regulator_dev *);
    int (*set_mode)(struct regulator_dev *, unsigned int);
    unsigned int (*get_mode)(struct regulator_dev *);
    int (*get_error_flags)(struct regulator_dev *, unsigned int *);
    int (*enable_time)(struct regulator_dev *);
    int (*set_ramp_delay)(struct regulator_dev *, int);
    int (*set_voltage_time)(struct regulator_dev *, int, int);
    int (*set_voltage_time_sel)(struct regulator_dev *, unsigned int, unsigned int);
    int (*set_soft_start)(struct regulator_dev *);
    int (*get_status)(struct regulator_dev *);
    unsigned int (*get_optimum_mode)(struct regulator_dev *, int, int, int);
    int (*set_load)(struct regulator_dev *, int);
    int (*set_bypass)(struct regulator_dev *, bool);
    int (*get_bypass)(struct regulator_dev *, bool *);
    int (*set_suspend_voltage)(struct regulator_dev *, int);
    int (*set_suspend_enable)(struct regulator_dev *);
    int (*set_suspend_disable)(struct regulator_dev *);
    int (*set_suspend_mode)(struct regulator_dev *, unsigned int);
    int (*resume)(struct regulator_dev *);
    int (*set_pull_down)(struct regulator_dev *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct regulator_ops {
    int (*list_voltage)(struct regulator_dev *, unsigned int);
    int (*set_voltage)(struct regulator_dev *, int, int, unsigned int *);
    int (*map_voltage)(struct regulator_dev *, int, int);
    int (*set_voltage_sel)(struct regulator_dev *, unsigned int);
    int (*get_voltage)(struct regulator_dev *);
    int (*get_voltage_sel)(struct regulator_dev *);
    int (*set_current_limit)(struct regulator_dev *, int, int);
    int (*get_current_limit)(struct regulator_dev *);
    int (*set_input_current_limit)(struct regulator_dev *, int);
    int (*set_over_current_protection)(struct regulator_dev *);
    int (*set_active_discharge)(struct regulator_dev *, bool);
    int (*enable)(struct regulator_dev *);
    int (*disable)(struct regulator_dev *);
    int (*is_enabled)(struct regulator_dev *);
    int (*set_mode)(struct regulator_dev *, unsigned int);
    unsigned int (*get_mode)(struct regulator_dev *);
    int (*get_error_flags)(struct regulator_dev *, unsigned int *);
    int (*enable_time)(struct regulator_dev *);
    int (*set_ramp_delay)(struct regulator_dev *, int);
    int (*set_voltage_time)(struct regulator_dev *, int, int);
    int (*set_voltage_time_sel)(struct regulator_dev *, unsigned int, unsigned int);
    int (*set_soft_start)(struct regulator_dev *);
    int (*get_status)(struct regulator_dev *);
    unsigned int (*get_optimum_mode)(struct regulator_dev *, int, int, int);
    int (*set_load)(struct regulator_dev *, int);
    int (*set_bypass)(struct regulator_dev *, bool);
    int (*get_bypass)(struct regulator_dev *, bool *);
    int (*set_suspend_voltage)(struct regulator_dev *, int);
    int (*set_suspend_enable)(struct regulator_dev *);
    int (*set_suspend_disable)(struct regulator_dev *);
    int (*set_suspend_mode)(struct regulator_dev *, unsigned int);
    int (*resume)(struct regulator_dev *);
    int (*set_pull_down)(struct regulator_dev *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct regulator_ops {
    int (*list_voltage)(struct regulator_dev *, unsigned int);
    int (*set_voltage)(struct regulator_dev *, int, int, unsigned int *);
    int (*map_voltage)(struct regulator_dev *, int, int);
    int (*set_voltage_sel)(struct regulator_dev *, unsigned int);
    int (*get_voltage)(struct regulator_dev *);
    int (*get_voltage_sel)(struct regulator_dev *);
    int (*set_current_limit)(struct regulator_dev *, int, int);
    int (*get_current_limit)(struct regulator_dev *);
    int (*set_input_current_limit)(struct regulator_dev *, int);
    int (*set_over_current_protection)(struct regulator_dev *);
    int (*set_active_discharge)(struct regulator_dev *, bool);
    int (*enable)(struct regulator_dev *);
    int (*disable)(struct regulator_dev *);
    int (*is_enabled)(struct regulator_dev *);
    int (*set_mode)(struct regulator_dev *, unsigned int);
    unsigned int (*get_mode)(struct regulator_dev *);
    int (*get_error_flags)(struct regulator_dev *, unsigned int *);
    int (*enable_time)(struct regulator_dev *);
    int (*set_ramp_delay)(struct regulator_dev *, int);
    int (*set_voltage_time)(struct regulator_dev *, int, int);
    int (*set_voltage_time_sel)(struct regulator_dev *, unsigned int, unsigned int);
    int (*set_soft_start)(struct regulator_dev *);
    int (*get_status)(struct regulator_dev *);
    unsigned int (*get_optimum_mode)(struct regulator_dev *, int, int, int);
    int (*set_load)(struct regulator_dev *, int);
    int (*set_bypass)(struct regulator_dev *, bool);
    int (*get_bypass)(struct regulator_dev *, bool *);
    int (*set_suspend_voltage)(struct regulator_dev *, int);
    int (*set_suspend_enable)(struct regulator_dev *);
    int (*set_suspend_disable)(struct regulator_dev *);
    int (*set_suspend_mode)(struct regulator_dev *, unsigned int);
    int (*resume)(struct regulator_dev *);
    int (*set_pull_down)(struct regulator_dev *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct regulator_ops {
    int (*list_voltage)(struct regulator_dev *, unsigned int);
    int (*set_voltage)(struct regulator_dev *, int, int, unsigned int *);
    int (*map_voltage)(struct regulator_dev *, int, int);
    int (*set_voltage_sel)(struct regulator_dev *, unsigned int);
    int (*get_voltage)(struct regulator_dev *);
    int (*get_voltage_sel)(struct regulator_dev *);
    int (*set_current_limit)(struct regulator_dev *, int, int);
    int (*get_current_limit)(struct regulator_dev *);
    int (*set_input_current_limit)(struct regulator_dev *, int);
    int (*set_over_current_protection)(struct regulator_dev *, int, int, bool);
    int (*set_over_voltage_protection)(struct regulator_dev *, int, int, bool);
    int (*set_under_voltage_protection)(struct regulator_dev *, int, int, bool);
    int (*set_thermal_protection)(struct regulator_dev *, int, int, bool);
    int (*set_active_discharge)(struct regulator_dev *, bool);
    int (*enable)(struct regulator_dev *);
    int (*disable)(struct regulator_dev *);
    int (*is_enabled)(struct regulator_dev *);
    int (*set_mode)(struct regulator_dev *, unsigned int);
    unsigned int (*get_mode)(struct regulator_dev *);
    int (*get_error_flags)(struct regulator_dev *, unsigned int *);
    int (*enable_time)(struct regulator_dev *);
    int (*set_ramp_delay)(struct regulator_dev *, int);
    int (*set_voltage_time)(struct regulator_dev *, int, int);
    int (*set_voltage_time_sel)(struct regulator_dev *, unsigned int, unsigned int);
    int (*set_soft_start)(struct regulator_dev *);
    int (*get_status)(struct regulator_dev *);
    unsigned int (*get_optimum_mode)(struct regulator_dev *, int, int, int);
    int (*set_load)(struct regulator_dev *, int);
    int (*set_bypass)(struct regulator_dev *, bool);
    int (*get_bypass)(struct regulator_dev *, bool *);
    int (*set_suspend_voltage)(struct regulator_dev *, int);
    int (*set_suspend_enable)(struct regulator_dev *);
    int (*set_suspend_disable)(struct regulator_dev *);
    int (*set_suspend_mode)(struct regulator_dev *, unsigned int);
    int (*resume)(struct regulator_dev *);
    int (*set_pull_down)(struct regulator_dev *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct regulator_ops {
    int (*list_voltage)(struct regulator_dev *, unsigned int);
    int (*set_voltage)(struct regulator_dev *, int, int, unsigned int *);
    int (*map_voltage)(struct regulator_dev *, int, int);
    int (*set_voltage_sel)(struct regulator_dev *, unsigned int);
    int (*get_voltage)(struct regulator_dev *);
    int (*get_voltage_sel)(struct regulator_dev *);
    int (*set_current_limit)(struct regulator_dev *, int, int);
    int (*get_current_limit)(struct regulator_dev *);
    int (*set_input_current_limit)(struct regulator_dev *, int);
    int (*set_over_current_protection)(struct regulator_dev *, int, int, bool);
    int (*set_over_voltage_protection)(struct regulator_dev *, int, int, bool);
    int (*set_under_voltage_protection)(struct regulator_dev *, int, int, bool);
    int (*set_thermal_protection)(struct regulator_dev *, int, int, bool);
    int (*set_active_discharge)(struct regulator_dev *, bool);
    int (*enable)(struct regulator_dev *);
    int (*disable)(struct regulator_dev *);
    int (*is_enabled)(struct regulator_dev *);
    int (*set_mode)(struct regulator_dev *, unsigned int);
    unsigned int (*get_mode)(struct regulator_dev *);
    int (*get_error_flags)(struct regulator_dev *, unsigned int *);
    int (*enable_time)(struct regulator_dev *);
    int (*set_ramp_delay)(struct regulator_dev *, int);
    int (*set_voltage_time)(struct regulator_dev *, int, int);
    int (*set_voltage_time_sel)(struct regulator_dev *, unsigned int, unsigned int);
    int (*set_soft_start)(struct regulator_dev *);
    int (*get_status)(struct regulator_dev *);
    unsigned int (*get_optimum_mode)(struct regulator_dev *, int, int, int);
    int (*set_load)(struct regulator_dev *, int);
    int (*set_bypass)(struct regulator_dev *, bool);
    int (*get_bypass)(struct regulator_dev *, bool *);
    int (*set_suspend_voltage)(struct regulator_dev *, int);
    int (*set_suspend_enable)(struct regulator_dev *);
    int (*set_suspend_disable)(struct regulator_dev *);
    int (*set_suspend_mode)(struct regulator_dev *, unsigned int);
    int (*resume)(struct regulator_dev *);
    int (*set_pull_down)(struct regulator_dev *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct regulator_ops {
    int (*list_voltage)(struct regulator_dev *, unsigned int);
    int (*set_voltage)(struct regulator_dev *, int, int, unsigned int *);
    int (*map_voltage)(struct regulator_dev *, int, int);
    int (*set_voltage_sel)(struct regulator_dev *, unsigned int);
    int (*get_voltage)(struct regulator_dev *);
    int (*get_voltage_sel)(struct regulator_dev *);
    int (*set_current_limit)(struct regulator_dev *, int, int);
    int (*get_current_limit)(struct regulator_dev *);
    int (*set_input_current_limit)(struct regulator_dev *, int);
    int (*set_over_current_protection)(struct regulator_dev *, int, int, bool);
    int (*set_over_voltage_protection)(struct regulator_dev *, int, int, bool);
    int (*set_under_voltage_protection)(struct regulator_dev *, int, int, bool);
    int (*set_thermal_protection)(struct regulator_dev *, int, int, bool);
    int (*set_active_discharge)(struct regulator_dev *, bool);
    int (*enable)(struct regulator_dev *);
    int (*disable)(struct regulator_dev *);
    int (*is_enabled)(struct regulator_dev *);
    int (*set_mode)(struct regulator_dev *, unsigned int);
    unsigned int (*get_mode)(struct regulator_dev *);
    int (*get_error_flags)(struct regulator_dev *, unsigned int *);
    int (*enable_time)(struct regulator_dev *);
    int (*set_ramp_delay)(struct regulator_dev *, int);
    int (*set_voltage_time)(struct regulator_dev *, int, int);
    int (*set_voltage_time_sel)(struct regulator_dev *, unsigned int, unsigned int);
    int (*set_soft_start)(struct regulator_dev *);
    int (*get_status)(struct regulator_dev *);
    unsigned int (*get_optimum_mode)(struct regulator_dev *, int, int, int);
    int (*set_load)(struct regulator_dev *, int);
    int (*set_bypass)(struct regulator_dev *, bool);
    int (*get_bypass)(struct regulator_dev *, bool *);
    int (*set_suspend_voltage)(struct regulator_dev *, int);
    int (*set_suspend_enable)(struct regulator_dev *);
    int (*set_suspend_disable)(struct regulator_dev *);
    int (*set_suspend_mode)(struct regulator_dev *, unsigned int);
    int (*resume)(struct regulator_dev *);
    int (*set_pull_down)(struct regulator_dev *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct regulator_ops {
    int (*list_voltage)(struct regulator_dev *, unsigned int);
    int (*set_voltage)(struct regulator_dev *, int, int, unsigned int *);
    int (*map_voltage)(struct regulator_dev *, int, int);
    int (*set_voltage_sel)(struct regulator_dev *, unsigned int);
    int (*get_voltage)(struct regulator_dev *);
    int (*get_voltage_sel)(struct regulator_dev *);
    int (*set_current_limit)(struct regulator_dev *, int, int);
    int (*get_current_limit)(struct regulator_dev *);
    int (*set_input_current_limit)(struct regulator_dev *, int);
    int (*set_over_current_protection)(struct regulator_dev *, int, int, bool);
    int (*set_over_voltage_protection)(struct regulator_dev *, int, int, bool);
    int (*set_under_voltage_protection)(struct regulator_dev *, int, int, bool);
    int (*set_thermal_protection)(struct regulator_dev *, int, int, bool);
    int (*set_active_discharge)(struct regulator_dev *, bool);
    int (*enable)(struct regulator_dev *);
    int (*disable)(struct regulator_dev *);
    int (*is_enabled)(struct regulator_dev *);
    int (*set_mode)(struct regulator_dev *, unsigned int);
    unsigned int (*get_mode)(struct regulator_dev *);
    int (*get_error_flags)(struct regulator_dev *, unsigned int *);
    int (*enable_time)(struct regulator_dev *);
    int (*set_ramp_delay)(struct regulator_dev *, int);
    int (*set_voltage_time)(struct regulator_dev *, int, int);
    int (*set_voltage_time_sel)(struct regulator_dev *, unsigned int, unsigned int);
    int (*set_soft_start)(struct regulator_dev *);
    int (*get_status)(struct regulator_dev *);
    unsigned int (*get_optimum_mode)(struct regulator_dev *, int, int, int);
    int (*set_load)(struct regulator_dev *, int);
    int (*set_bypass)(struct regulator_dev *, bool);
    int (*get_bypass)(struct regulator_dev *, bool *);
    int (*set_suspend_voltage)(struct regulator_dev *, int);
    int (*set_suspend_enable)(struct regulator_dev *);
    int (*set_suspend_disable)(struct regulator_dev *);
    int (*set_suspend_mode)(struct regulator_dev *, unsigned int);
    int (*resume)(struct regulator_dev *);
    int (*set_pull_down)(struct regulator_dev *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct regulator_ops {
    int (*list_voltage)(struct regulator_dev *, unsigned int);
    int (*set_voltage)(struct regulator_dev *, int, int, unsigned int *);
    int (*map_voltage)(struct regulator_dev *, int, int);
    int (*set_voltage_sel)(struct regulator_dev *, unsigned int);
    int (*get_voltage)(struct regulator_dev *);
    int (*get_voltage_sel)(struct regulator_dev *);
    int (*set_current_limit)(struct regulator_dev *, int, int);
    int (*get_current_limit)(struct regulator_dev *);
    int (*set_input_current_limit)(struct regulator_dev *, int);
    int (*set_over_current_protection)(struct regulator_dev *, int, int, bool);
    int (*set_over_voltage_protection)(struct regulator_dev *, int, int, bool);
    int (*set_under_voltage_protection)(struct regulator_dev *, int, int, bool);
    int (*set_thermal_protection)(struct regulator_dev *, int, int, bool);
    int (*set_active_discharge)(struct regulator_dev *, bool);
    int (*enable)(struct regulator_dev *);
    int (*disable)(struct regulator_dev *);
    int (*is_enabled)(struct regulator_dev *);
    int (*set_mode)(struct regulator_dev *, unsigned int);
    unsigned int (*get_mode)(struct regulator_dev *);
    int (*get_error_flags)(struct regulator_dev *, unsigned int *);
    int (*enable_time)(struct regulator_dev *);
    int (*set_ramp_delay)(struct regulator_dev *, int);
    int (*set_voltage_time)(struct regulator_dev *, int, int);
    int (*set_voltage_time_sel)(struct regulator_dev *, unsigned int, unsigned int);
    int (*set_soft_start)(struct regulator_dev *);
    int (*get_status)(struct regulator_dev *);
    unsigned int (*get_optimum_mode)(struct regulator_dev *, int, int, int);
    int (*set_load)(struct regulator_dev *, int);
    int (*set_bypass)(struct regulator_dev *, bool);
    int (*get_bypass)(struct regulator_dev *, bool *);
    int (*set_suspend_voltage)(struct regulator_dev *, int);
    int (*set_suspend_enable)(struct regulator_dev *);
    int (*set_suspend_disable)(struct regulator_dev *);
    int (*set_suspend_mode)(struct regulator_dev *, unsigned int);
    int (*resume)(struct regulator_dev *);
    int (*set_pull_down)(struct regulator_dev *);
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
struct regulator_ops {
    int (*list_voltage)(struct regulator_dev *, unsigned int);
    int (*set_voltage)(struct regulator_dev *, int, int, unsigned int *);
    int (*map_voltage)(struct regulator_dev *, int, int);
    int (*set_voltage_sel)(struct regulator_dev *, unsigned int);
    int (*get_voltage)(struct regulator_dev *);
    int (*get_voltage_sel)(struct regulator_dev *);
    int (*set_current_limit)(struct regulator_dev *, int, int);
    int (*get_current_limit)(struct regulator_dev *);
    int (*set_input_current_limit)(struct regulator_dev *, int);
    int (*set_over_current_protection)(struct regulator_dev *);
    int (*set_active_discharge)(struct regulator_dev *, bool);
    int (*enable)(struct regulator_dev *);
    int (*disable)(struct regulator_dev *);
    int (*is_enabled)(struct regulator_dev *);
    int (*set_mode)(struct regulator_dev *, unsigned int);
    unsigned int (*get_mode)(struct regulator_dev *);
    int (*get_error_flags)(struct regulator_dev *, unsigned int *);
    int (*enable_time)(struct regulator_dev *);
    int (*set_ramp_delay)(struct regulator_dev *, int);
    int (*set_voltage_time)(struct regulator_dev *, int, int);
    int (*set_voltage_time_sel)(struct regulator_dev *, unsigned int, unsigned int);
    int (*set_soft_start)(struct regulator_dev *);
    int (*get_status)(struct regulator_dev *);
    unsigned int (*get_optimum_mode)(struct regulator_dev *, int, int, int);
    int (*set_load)(struct regulator_dev *, int);
    int (*set_bypass)(struct regulator_dev *, bool);
    int (*get_bypass)(struct regulator_dev *, bool *);
    int (*set_suspend_voltage)(struct regulator_dev *, int);
    int (*set_suspend_enable)(struct regulator_dev *);
    int (*set_suspend_disable)(struct regulator_dev *);
    int (*set_suspend_mode)(struct regulator_dev *, unsigned int);
    int (*resume)(struct regulator_dev *);
    int (*set_pull_down)(struct regulator_dev *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct regulator_ops {
    int (*list_voltage)(struct regulator_dev *, unsigned int);
    int (*set_voltage)(struct regulator_dev *, int, int, unsigned int *);
    int (*map_voltage)(struct regulator_dev *, int, int);
    int (*set_voltage_sel)(struct regulator_dev *, unsigned int);
    int (*get_voltage)(struct regulator_dev *);
    int (*get_voltage_sel)(struct regulator_dev *);
    int (*set_current_limit)(struct regulator_dev *, int, int);
    int (*get_current_limit)(struct regulator_dev *);
    int (*set_input_current_limit)(struct regulator_dev *, int);
    int (*set_over_current_protection)(struct regulator_dev *);
    int (*set_active_discharge)(struct regulator_dev *, bool);
    int (*enable)(struct regulator_dev *);
    int (*disable)(struct regulator_dev *);
    int (*is_enabled)(struct regulator_dev *);
    int (*set_mode)(struct regulator_dev *, unsigned int);
    unsigned int (*get_mode)(struct regulator_dev *);
    int (*get_error_flags)(struct regulator_dev *, unsigned int *);
    int (*enable_time)(struct regulator_dev *);
    int (*set_ramp_delay)(struct regulator_dev *, int);
    int (*set_voltage_time)(struct regulator_dev *, int, int);
    int (*set_voltage_time_sel)(struct regulator_dev *, unsigned int, unsigned int);
    int (*set_soft_start)(struct regulator_dev *);
    int (*get_status)(struct regulator_dev *);
    unsigned int (*get_optimum_mode)(struct regulator_dev *, int, int, int);
    int (*set_load)(struct regulator_dev *, int);
    int (*set_bypass)(struct regulator_dev *, bool);
    int (*get_bypass)(struct regulator_dev *, bool *);
    int (*set_suspend_voltage)(struct regulator_dev *, int);
    int (*set_suspend_enable)(struct regulator_dev *);
    int (*set_suspend_disable)(struct regulator_dev *);
    int (*set_suspend_mode)(struct regulator_dev *, unsigned int);
    int (*resume)(struct regulator_dev *);
    int (*set_pull_down)(struct regulator_dev *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct regulator_ops {
    int (*list_voltage)(struct regulator_dev *, unsigned int);
    int (*set_voltage)(struct regulator_dev *, int, int, unsigned int *);
    int (*map_voltage)(struct regulator_dev *, int, int);
    int (*set_voltage_sel)(struct regulator_dev *, unsigned int);
    int (*get_voltage)(struct regulator_dev *);
    int (*get_voltage_sel)(struct regulator_dev *);
    int (*set_current_limit)(struct regulator_dev *, int, int);
    int (*get_current_limit)(struct regulator_dev *);
    int (*set_input_current_limit)(struct regulator_dev *, int);
    int (*set_over_current_protection)(struct regulator_dev *);
    int (*set_active_discharge)(struct regulator_dev *, bool);
    int (*enable)(struct regulator_dev *);
    int (*disable)(struct regulator_dev *);
    int (*is_enabled)(struct regulator_dev *);
    int (*set_mode)(struct regulator_dev *, unsigned int);
    unsigned int (*get_mode)(struct regulator_dev *);
    int (*get_error_flags)(struct regulator_dev *, unsigned int *);
    int (*enable_time)(struct regulator_dev *);
    int (*set_ramp_delay)(struct regulator_dev *, int);
    int (*set_voltage_time)(struct regulator_dev *, int, int);
    int (*set_voltage_time_sel)(struct regulator_dev *, unsigned int, unsigned int);
    int (*set_soft_start)(struct regulator_dev *);
    int (*get_status)(struct regulator_dev *);
    unsigned int (*get_optimum_mode)(struct regulator_dev *, int, int, int);
    int (*set_load)(struct regulator_dev *, int);
    int (*set_bypass)(struct regulator_dev *, bool);
    int (*get_bypass)(struct regulator_dev *, bool *);
    int (*set_suspend_voltage)(struct regulator_dev *, int);
    int (*set_suspend_enable)(struct regulator_dev *);
    int (*set_suspend_disable)(struct regulator_dev *);
    int (*set_suspend_mode)(struct regulator_dev *, unsigned int);
    int (*resume)(struct regulator_dev *);
    int (*set_pull_down)(struct regulator_dev *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct regulator_ops {
    int (*list_voltage)(struct regulator_dev *, unsigned int);
    int (*set_voltage)(struct regulator_dev *, int, int, unsigned int *);
    int (*map_voltage)(struct regulator_dev *, int, int);
    int (*set_voltage_sel)(struct regulator_dev *, unsigned int);
    int (*get_voltage)(struct regulator_dev *);
    int (*get_voltage_sel)(struct regulator_dev *);
    int (*set_current_limit)(struct regulator_dev *, int, int);
    int (*get_current_limit)(struct regulator_dev *);
    int (*set_input_current_limit)(struct regulator_dev *, int);
    int (*set_over_current_protection)(struct regulator_dev *);
    int (*set_active_discharge)(struct regulator_dev *, bool);
    int (*enable)(struct regulator_dev *);
    int (*disable)(struct regulator_dev *);
    int (*is_enabled)(struct regulator_dev *);
    int (*set_mode)(struct regulator_dev *, unsigned int);
    unsigned int (*get_mode)(struct regulator_dev *);
    int (*get_error_flags)(struct regulator_dev *, unsigned int *);
    int (*enable_time)(struct regulator_dev *);
    int (*set_ramp_delay)(struct regulator_dev *, int);
    int (*set_voltage_time)(struct regulator_dev *, int, int);
    int (*set_voltage_time_sel)(struct regulator_dev *, unsigned int, unsigned int);
    int (*set_soft_start)(struct regulator_dev *);
    int (*get_status)(struct regulator_dev *);
    unsigned int (*get_optimum_mode)(struct regulator_dev *, int, int, int);
    int (*set_load)(struct regulator_dev *, int);
    int (*set_bypass)(struct regulator_dev *, bool);
    int (*get_bypass)(struct regulator_dev *, bool *);
    int (*set_suspend_voltage)(struct regulator_dev *, int);
    int (*set_suspend_enable)(struct regulator_dev *);
    int (*set_suspend_disable)(struct regulator_dev *);
    int (*set_suspend_mode)(struct regulator_dev *, unsigned int);
    int (*resume)(struct regulator_dev *);
    int (*set_pull_down)(struct regulator_dev *);
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
struct regulator_ops {
    int (*list_voltage)(struct regulator_dev *, unsigned int);
    int (*set_voltage)(struct regulator_dev *, int, int, unsigned int *);
    int (*map_voltage)(struct regulator_dev *, int, int);
    int (*set_voltage_sel)(struct regulator_dev *, unsigned int);
    int (*get_voltage)(struct regulator_dev *);
    int (*get_voltage_sel)(struct regulator_dev *);
    int (*set_current_limit)(struct regulator_dev *, int, int);
    int (*get_current_limit)(struct regulator_dev *);
    int (*set_input_current_limit)(struct regulator_dev *, int);
    int (*set_over_current_protection)(struct regulator_dev *);
    int (*set_active_discharge)(struct regulator_dev *, bool);
    int (*enable)(struct regulator_dev *);
    int (*disable)(struct regulator_dev *);
    int (*is_enabled)(struct regulator_dev *);
    int (*set_mode)(struct regulator_dev *, unsigned int);
    unsigned int (*get_mode)(struct regulator_dev *);
    int (*get_error_flags)(struct regulator_dev *, unsigned int *);
    int (*enable_time)(struct regulator_dev *);
    int (*set_ramp_delay)(struct regulator_dev *, int);
    int (*set_voltage_time)(struct regulator_dev *, int, int);
    int (*set_voltage_time_sel)(struct regulator_dev *, unsigned int, unsigned int);
    int (*set_soft_start)(struct regulator_dev *);
    int (*get_status)(struct regulator_dev *);
    unsigned int (*get_optimum_mode)(struct regulator_dev *, int, int, int);
    int (*set_load)(struct regulator_dev *, int);
    int (*set_bypass)(struct regulator_dev *, bool);
    int (*get_bypass)(struct regulator_dev *, bool *);
    int (*set_suspend_voltage)(struct regulator_dev *, int);
    int (*set_suspend_enable)(struct regulator_dev *);
    int (*set_suspend_disable)(struct regulator_dev *);
    int (*set_suspend_mode)(struct regulator_dev *, unsigned int);
    int (*resume)(struct regulator_dev *);
    int (*set_pull_down)(struct regulator_dev *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct regulator_ops {
    int (*list_voltage)(struct regulator_dev *, unsigned int);
    int (*set_voltage)(struct regulator_dev *, int, int, unsigned int *);
    int (*map_voltage)(struct regulator_dev *, int, int);
    int (*set_voltage_sel)(struct regulator_dev *, unsigned int);
    int (*get_voltage)(struct regulator_dev *);
    int (*get_voltage_sel)(struct regulator_dev *);
    int (*set_current_limit)(struct regulator_dev *, int, int);
    int (*get_current_limit)(struct regulator_dev *);
    int (*set_input_current_limit)(struct regulator_dev *, int);
    int (*set_over_current_protection)(struct regulator_dev *);
    int (*set_active_discharge)(struct regulator_dev *, bool);
    int (*enable)(struct regulator_dev *);
    int (*disable)(struct regulator_dev *);
    int (*is_enabled)(struct regulator_dev *);
    int (*set_mode)(struct regulator_dev *, unsigned int);
    unsigned int (*get_mode)(struct regulator_dev *);
    int (*get_error_flags)(struct regulator_dev *, unsigned int *);
    int (*enable_time)(struct regulator_dev *);
    int (*set_ramp_delay)(struct regulator_dev *, int);
    int (*set_voltage_time)(struct regulator_dev *, int, int);
    int (*set_voltage_time_sel)(struct regulator_dev *, unsigned int, unsigned int);
    int (*set_soft_start)(struct regulator_dev *);
    int (*get_status)(struct regulator_dev *);
    unsigned int (*get_optimum_mode)(struct regulator_dev *, int, int, int);
    int (*set_load)(struct regulator_dev *, int);
    int (*set_bypass)(struct regulator_dev *, bool);
    int (*get_bypass)(struct regulator_dev *, bool *);
    int (*set_suspend_voltage)(struct regulator_dev *, int);
    int (*set_suspend_enable)(struct regulator_dev *);
    int (*set_suspend_disable)(struct regulator_dev *);
    int (*set_suspend_mode)(struct regulator_dev *, unsigned int);
    int (*resume)(struct regulator_dev *);
    int (*set_pull_down)(struct regulator_dev *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct regulator_ops {
    int (*list_voltage)(struct regulator_dev *, unsigned int);
    int (*set_voltage)(struct regulator_dev *, int, int, unsigned int *);
    int (*map_voltage)(struct regulator_dev *, int, int);
    int (*set_voltage_sel)(struct regulator_dev *, unsigned int);
    int (*get_voltage)(struct regulator_dev *);
    int (*get_voltage_sel)(struct regulator_dev *);
    int (*set_current_limit)(struct regulator_dev *, int, int);
    int (*get_current_limit)(struct regulator_dev *);
    int (*set_input_current_limit)(struct regulator_dev *, int);
    int (*set_over_current_protection)(struct regulator_dev *);
    int (*set_active_discharge)(struct regulator_dev *, bool);
    int (*enable)(struct regulator_dev *);
    int (*disable)(struct regulator_dev *);
    int (*is_enabled)(struct regulator_dev *);
    int (*set_mode)(struct regulator_dev *, unsigned int);
    unsigned int (*get_mode)(struct regulator_dev *);
    int (*get_error_flags)(struct regulator_dev *, unsigned int *);
    int (*enable_time)(struct regulator_dev *);
    int (*set_ramp_delay)(struct regulator_dev *, int);
    int (*set_voltage_time)(struct regulator_dev *, int, int);
    int (*set_voltage_time_sel)(struct regulator_dev *, unsigned int, unsigned int);
    int (*set_soft_start)(struct regulator_dev *);
    int (*get_status)(struct regulator_dev *);
    unsigned int (*get_optimum_mode)(struct regulator_dev *, int, int, int);
    int (*set_load)(struct regulator_dev *, int);
    int (*set_bypass)(struct regulator_dev *, bool);
    int (*get_bypass)(struct regulator_dev *, bool *);
    int (*set_suspend_voltage)(struct regulator_dev *, int);
    int (*set_suspend_enable)(struct regulator_dev *);
    int (*set_suspend_disable)(struct regulator_dev *);
    int (*set_suspend_mode)(struct regulator_dev *, unsigned int);
    int (*resume)(struct regulator_dev *);
    int (*set_pull_down)(struct regulator_dev *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct regulator_ops {
    int (*list_voltage)(struct regulator_dev *, unsigned int);
    int (*set_voltage)(struct regulator_dev *, int, int, unsigned int *);
    int (*map_voltage)(struct regulator_dev *, int, int);
    int (*set_voltage_sel)(struct regulator_dev *, unsigned int);
    int (*get_voltage)(struct regulator_dev *);
    int (*get_voltage_sel)(struct regulator_dev *);
    int (*set_current_limit)(struct regulator_dev *, int, int);
    int (*get_current_limit)(struct regulator_dev *);
    int (*set_input_current_limit)(struct regulator_dev *, int);
    int (*set_over_current_protection)(struct regulator_dev *);
    int (*set_active_discharge)(struct regulator_dev *, bool);
    int (*enable)(struct regulator_dev *);
    int (*disable)(struct regulator_dev *);
    int (*is_enabled)(struct regulator_dev *);
    int (*set_mode)(struct regulator_dev *, unsigned int);
    unsigned int (*get_mode)(struct regulator_dev *);
    int (*get_error_flags)(struct regulator_dev *, unsigned int *);
    int (*enable_time)(struct regulator_dev *);
    int (*set_ramp_delay)(struct regulator_dev *, int);
    int (*set_voltage_time)(struct regulator_dev *, int, int);
    int (*set_voltage_time_sel)(struct regulator_dev *, unsigned int, unsigned int);
    int (*set_soft_start)(struct regulator_dev *);
    int (*get_status)(struct regulator_dev *);
    unsigned int (*get_optimum_mode)(struct regulator_dev *, int, int, int);
    int (*set_load)(struct regulator_dev *, int);
    int (*set_bypass)(struct regulator_dev *, bool);
    int (*get_bypass)(struct regulator_dev *, bool *);
    int (*set_suspend_voltage)(struct regulator_dev *, int);
    int (*set_suspend_enable)(struct regulator_dev *);
    int (*set_suspend_disable)(struct regulator_dev *);
    int (*set_suspend_mode)(struct regulator_dev *, unsigned int);
    int (*resume)(struct regulator_dev *);
    int (*set_pull_down)(struct regulator_dev *);
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
<code>int (*set_active_discharge)(struct regulator_dev *, bool)</code>
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
<code>int (*get_error_flags)(struct regulator_dev *, unsigned int *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_voltage_time)(struct regulator_dev *, int, int)</code>
</li>
</ul>
</details>
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
<code>int (*resume_early)(struct regulator_dev *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*resume)(struct regulator_dev *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*resume_early)(struct regulator_dev *)</code>
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
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*set_over_voltage_protection)(struct regulator_dev *, int, int, bool)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_under_voltage_protection)(struct regulator_dev *, int, int, bool)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_thermal_protection)(struct regulator_dev *, int, int, bool)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*set_over_current_protection)(struct regulator_dev *)</code> ➡️ <code>int (*set_over_current_protection)(struct regulator_dev *, int, int, bool)</code>
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
