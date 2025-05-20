# Struct: <code>devfreq_cooling_device</code>

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
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct devfreq_cooling_device {
    int id;
    struct thermal_cooling_device *cdev;
    struct devfreq *devfreq;
    long unsigned int cooling_state;
    u32 *power_table;
    u32 *freq_table;
    size_t freq_table_size;
    struct devfreq_cooling_power *power_ops;
    u32 res_util;
    int capped_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct devfreq_cooling_device {
    int id;
    struct thermal_cooling_device *cdev;
    struct devfreq *devfreq;
    long unsigned int cooling_state;
    u32 *power_table;
    u32 *freq_table;
    size_t freq_table_size;
    struct devfreq_cooling_power *power_ops;
    u32 res_util;
    int capped_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct devfreq_cooling_device {
    int id;
    struct thermal_cooling_device *cdev;
    struct devfreq *devfreq;
    long unsigned int cooling_state;
    u32 *power_table;
    u32 *freq_table;
    size_t freq_table_size;
    struct devfreq_cooling_power *power_ops;
    u32 res_util;
    int capped_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct devfreq_cooling_device {
    int id;
    struct thermal_cooling_device *cdev;
    struct devfreq *devfreq;
    long unsigned int cooling_state;
    u32 *power_table;
    u32 *freq_table;
    size_t freq_table_size;
    struct devfreq_cooling_power *power_ops;
    u32 res_util;
    int capped_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct devfreq_cooling_device {
    int id;
    struct thermal_cooling_device *cdev;
    struct devfreq *devfreq;
    long unsigned int cooling_state;
    u32 *power_table;
    u32 *freq_table;
    size_t freq_table_size;
    struct devfreq_cooling_power *power_ops;
    u32 res_util;
    int capped_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct devfreq_cooling_device {
    int id;
    struct thermal_cooling_device *cdev;
    struct devfreq *devfreq;
    long unsigned int cooling_state;
    u32 *power_table;
    u32 *freq_table;
    size_t freq_table_size;
    struct devfreq_cooling_power *power_ops;
    u32 res_util;
    int capped_state;
    struct dev_pm_qos_request req_max_freq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct devfreq_cooling_device {
    int id;
    struct thermal_cooling_device *cdev;
    struct devfreq *devfreq;
    long unsigned int cooling_state;
    u32 *freq_table;
    size_t max_state;
    struct devfreq_cooling_power *power_ops;
    u32 res_util;
    int capped_state;
    struct dev_pm_qos_request req_max_freq;
    struct em_perf_domain *em_pd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct devfreq_cooling_device {
    struct thermal_cooling_device *cdev;
    struct devfreq *devfreq;
    long unsigned int cooling_state;
    u32 *freq_table;
    size_t max_state;
    struct devfreq_cooling_power *power_ops;
    u32 res_util;
    int capped_state;
    struct dev_pm_qos_request req_max_freq;
    struct em_perf_domain *em_pd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct devfreq_cooling_device {
    struct thermal_cooling_device *cdev;
    struct devfreq *devfreq;
    long unsigned int cooling_state;
    u32 *freq_table;
    size_t max_state;
    struct devfreq_cooling_power *power_ops;
    u32 res_util;
    int capped_state;
    struct dev_pm_qos_request req_max_freq;
    struct em_perf_domain *em_pd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct devfreq_cooling_device {
    struct thermal_cooling_device *cdev;
    struct devfreq *devfreq;
    long unsigned int cooling_state;
    u32 *freq_table;
    size_t max_state;
    struct devfreq_cooling_power *power_ops;
    u32 res_util;
    int capped_state;
    struct dev_pm_qos_request req_max_freq;
    struct em_perf_domain *em_pd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct devfreq_cooling_device {
    struct thermal_cooling_device *cdev;
    struct thermal_cooling_device_ops cooling_ops;
    struct devfreq *devfreq;
    long unsigned int cooling_state;
    u32 *freq_table;
    size_t max_state;
    struct devfreq_cooling_power *power_ops;
    u32 res_util;
    int capped_state;
    struct dev_pm_qos_request req_max_freq;
    struct em_perf_domain *em_pd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct devfreq_cooling_device {
    struct thermal_cooling_device *cdev;
    struct thermal_cooling_device_ops cooling_ops;
    struct devfreq *devfreq;
    long unsigned int cooling_state;
    u32 *freq_table;
    size_t max_state;
    struct devfreq_cooling_power *power_ops;
    u32 res_util;
    int capped_state;
    struct dev_pm_qos_request req_max_freq;
    struct em_perf_domain *em_pd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct devfreq_cooling_device {
    struct thermal_cooling_device *cdev;
    struct thermal_cooling_device_ops cooling_ops;
    struct devfreq *devfreq;
    long unsigned int cooling_state;
    u32 *freq_table;
    size_t max_state;
    struct devfreq_cooling_power *power_ops;
    u32 res_util;
    int capped_state;
    struct dev_pm_qos_request req_max_freq;
    struct em_perf_domain *em_pd;
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
struct devfreq_cooling_device {
    int id;
    struct thermal_cooling_device *cdev;
    struct devfreq *devfreq;
    long unsigned int cooling_state;
    u32 *power_table;
    u32 *freq_table;
    size_t freq_table_size;
    struct devfreq_cooling_power *power_ops;
    u32 res_util;
    int capped_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct devfreq_cooling_device {
    int id;
    struct thermal_cooling_device *cdev;
    struct devfreq *devfreq;
    long unsigned int cooling_state;
    u32 *power_table;
    u32 *freq_table;
    size_t freq_table_size;
    struct devfreq_cooling_power *power_ops;
    u32 res_util;
    int capped_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct devfreq_cooling_device {
    int id;
    struct thermal_cooling_device *cdev;
    struct devfreq *devfreq;
    long unsigned int cooling_state;
    u32 *power_table;
    u32 *freq_table;
    size_t freq_table_size;
    struct devfreq_cooling_power *power_ops;
    u32 res_util;
    int capped_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct devfreq_cooling_device {
    int id;
    struct thermal_cooling_device *cdev;
    struct devfreq *devfreq;
    long unsigned int cooling_state;
    u32 *power_table;
    u32 *freq_table;
    size_t freq_table_size;
    struct devfreq_cooling_power *power_ops;
    u32 res_util;
    int capped_state;
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
struct devfreq_cooling_device {
    int id;
    struct thermal_cooling_device *cdev;
    struct devfreq *devfreq;
    long unsigned int cooling_state;
    u32 *power_table;
    u32 *freq_table;
    size_t freq_table_size;
    struct devfreq_cooling_power *power_ops;
    u32 res_util;
    int capped_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct devfreq_cooling_device {
    int id;
    struct thermal_cooling_device *cdev;
    struct devfreq *devfreq;
    long unsigned int cooling_state;
    u32 *power_table;
    u32 *freq_table;
    size_t freq_table_size;
    struct devfreq_cooling_power *power_ops;
    u32 res_util;
    int capped_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct devfreq_cooling_device {
    int id;
    struct thermal_cooling_device *cdev;
    struct devfreq *devfreq;
    long unsigned int cooling_state;
    u32 *power_table;
    u32 *freq_table;
    size_t freq_table_size;
    struct devfreq_cooling_power *power_ops;
    u32 res_util;
    int capped_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct devfreq_cooling_device {
    int id;
    struct thermal_cooling_device *cdev;
    struct devfreq *devfreq;
    long unsigned int cooling_state;
    u32 *power_table;
    u32 *freq_table;
    size_t freq_table_size;
    struct devfreq_cooling_power *power_ops;
    u32 res_util;
    int capped_state;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
<code>struct dev_pm_qos_request req_max_freq</code>
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
<code>size_t max_state</code>
</li>
<li>
<b>Field added. </b>
<code>struct em_perf_domain *em_pd</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 *power_table</code>
</li>
<li>
<b>Field removed. </b>
<code>size_t freq_table_size</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int id</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct thermal_cooling_device_ops cooling_ops</code>
</li>
</ul>
</details>
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
