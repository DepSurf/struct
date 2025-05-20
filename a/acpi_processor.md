# Struct: <code>acpi_processor</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct acpi_processor {
    acpi_handle handle;
    u32 acpi_id;
    phys_cpuid_t phys_id;
    u32 id;
    u32 pblk;
    int performance_platform_limit;
    int throttling_platform_limit;
    struct acpi_processor_flags flags;
    struct acpi_processor_power power;
    struct acpi_processor_performance *performance;
    struct acpi_processor_throttling throttling;
    struct acpi_processor_limit limit;
    struct thermal_cooling_device *cdev;
    struct device *dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct acpi_processor {
    acpi_handle handle;
    u32 acpi_id;
    phys_cpuid_t phys_id;
    u32 id;
    u32 pblk;
    int performance_platform_limit;
    int throttling_platform_limit;
    struct acpi_processor_flags flags;
    struct acpi_processor_power power;
    struct acpi_processor_performance *performance;
    struct acpi_processor_throttling throttling;
    struct acpi_processor_limit limit;
    struct thermal_cooling_device *cdev;
    struct device *dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct acpi_processor {
    acpi_handle handle;
    u32 acpi_id;
    phys_cpuid_t phys_id;
    u32 id;
    u32 pblk;
    int performance_platform_limit;
    int throttling_platform_limit;
    struct acpi_processor_flags flags;
    struct acpi_processor_power power;
    struct acpi_processor_performance *performance;
    struct acpi_processor_throttling throttling;
    struct acpi_processor_limit limit;
    struct thermal_cooling_device *cdev;
    struct device *dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct acpi_processor {
    acpi_handle handle;
    u32 acpi_id;
    phys_cpuid_t phys_id;
    u32 id;
    u32 pblk;
    int performance_platform_limit;
    int throttling_platform_limit;
    struct acpi_processor_flags flags;
    struct acpi_processor_power power;
    struct acpi_processor_performance *performance;
    struct acpi_processor_throttling throttling;
    struct acpi_processor_limit limit;
    struct thermal_cooling_device *cdev;
    struct device *dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct acpi_processor {
    acpi_handle handle;
    u32 acpi_id;
    phys_cpuid_t phys_id;
    u32 id;
    u32 pblk;
    int performance_platform_limit;
    int throttling_platform_limit;
    struct acpi_processor_flags flags;
    struct acpi_processor_power power;
    struct acpi_processor_performance *performance;
    struct acpi_processor_throttling throttling;
    struct acpi_processor_limit limit;
    struct thermal_cooling_device *cdev;
    struct device *dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct acpi_processor {
    acpi_handle handle;
    u32 acpi_id;
    phys_cpuid_t phys_id;
    u32 id;
    u32 pblk;
    int performance_platform_limit;
    int throttling_platform_limit;
    struct acpi_processor_flags flags;
    struct acpi_processor_power power;
    struct acpi_processor_performance *performance;
    struct acpi_processor_throttling throttling;
    struct acpi_processor_limit limit;
    struct thermal_cooling_device *cdev;
    struct device *dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct acpi_processor {
    acpi_handle handle;
    u32 acpi_id;
    phys_cpuid_t phys_id;
    u32 id;
    u32 pblk;
    int performance_platform_limit;
    int throttling_platform_limit;
    struct acpi_processor_flags flags;
    struct acpi_processor_power power;
    struct acpi_processor_performance *performance;
    struct acpi_processor_throttling throttling;
    struct acpi_processor_limit limit;
    struct thermal_cooling_device *cdev;
    struct device *dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct acpi_processor {
    acpi_handle handle;
    u32 acpi_id;
    phys_cpuid_t phys_id;
    u32 id;
    u32 pblk;
    int performance_platform_limit;
    int throttling_platform_limit;
    struct acpi_processor_flags flags;
    struct acpi_processor_power power;
    struct acpi_processor_performance *performance;
    struct acpi_processor_throttling throttling;
    struct acpi_processor_limit limit;
    struct thermal_cooling_device *cdev;
    struct device *dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct acpi_processor {
    acpi_handle handle;
    u32 acpi_id;
    phys_cpuid_t phys_id;
    u32 id;
    u32 pblk;
    int performance_platform_limit;
    int throttling_platform_limit;
    struct acpi_processor_flags flags;
    struct acpi_processor_power power;
    struct acpi_processor_performance *performance;
    struct acpi_processor_throttling throttling;
    struct acpi_processor_limit limit;
    struct thermal_cooling_device *cdev;
    struct device *dev;
    struct freq_qos_request perflib_req;
    struct freq_qos_request thermal_req;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct acpi_processor {
    acpi_handle handle;
    u32 acpi_id;
    phys_cpuid_t phys_id;
    u32 id;
    u32 pblk;
    int performance_platform_limit;
    int throttling_platform_limit;
    struct acpi_processor_flags flags;
    struct acpi_processor_power power;
    struct acpi_processor_performance *performance;
    struct acpi_processor_throttling throttling;
    struct acpi_processor_limit limit;
    struct thermal_cooling_device *cdev;
    struct device *dev;
    struct freq_qos_request perflib_req;
    struct freq_qos_request thermal_req;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct acpi_processor {
    acpi_handle handle;
    u32 acpi_id;
    phys_cpuid_t phys_id;
    u32 id;
    u32 pblk;
    int performance_platform_limit;
    int throttling_platform_limit;
    struct acpi_processor_flags flags;
    struct acpi_processor_power power;
    struct acpi_processor_performance *performance;
    struct acpi_processor_throttling throttling;
    struct acpi_processor_limit limit;
    struct thermal_cooling_device *cdev;
    struct device *dev;
    struct freq_qos_request perflib_req;
    struct freq_qos_request thermal_req;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct acpi_processor {
    acpi_handle handle;
    u32 acpi_id;
    phys_cpuid_t phys_id;
    u32 id;
    u32 pblk;
    int performance_platform_limit;
    int throttling_platform_limit;
    struct acpi_processor_flags flags;
    struct acpi_processor_power power;
    struct acpi_processor_performance *performance;
    struct acpi_processor_throttling throttling;
    struct acpi_processor_limit limit;
    struct thermal_cooling_device *cdev;
    struct device *dev;
    struct freq_qos_request perflib_req;
    struct freq_qos_request thermal_req;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct acpi_processor {
    acpi_handle handle;
    u32 acpi_id;
    phys_cpuid_t phys_id;
    u32 id;
    u32 pblk;
    int performance_platform_limit;
    int throttling_platform_limit;
    struct acpi_processor_flags flags;
    struct acpi_processor_power power;
    struct acpi_processor_performance *performance;
    struct acpi_processor_throttling throttling;
    struct acpi_processor_limit limit;
    struct thermal_cooling_device *cdev;
    struct device *dev;
    struct freq_qos_request perflib_req;
    struct freq_qos_request thermal_req;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct acpi_processor {
    acpi_handle handle;
    u32 acpi_id;
    phys_cpuid_t phys_id;
    u32 id;
    u32 pblk;
    int performance_platform_limit;
    int throttling_platform_limit;
    struct acpi_processor_flags flags;
    struct acpi_processor_power power;
    struct acpi_processor_performance *performance;
    struct acpi_processor_throttling throttling;
    struct acpi_processor_limit limit;
    struct thermal_cooling_device *cdev;
    struct device *dev;
    struct freq_qos_request perflib_req;
    struct freq_qos_request thermal_req;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct acpi_processor {
    acpi_handle handle;
    u32 acpi_id;
    phys_cpuid_t phys_id;
    u32 id;
    u32 pblk;
    int performance_platform_limit;
    int throttling_platform_limit;
    struct acpi_processor_flags flags;
    struct acpi_processor_power power;
    struct acpi_processor_performance *performance;
    struct acpi_processor_throttling throttling;
    struct acpi_processor_limit limit;
    struct thermal_cooling_device *cdev;
    struct device *dev;
    struct freq_qos_request perflib_req;
    struct freq_qos_request thermal_req;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct acpi_processor {
    acpi_handle handle;
    u32 acpi_id;
    phys_cpuid_t phys_id;
    u32 id;
    u32 pblk;
    int performance_platform_limit;
    int throttling_platform_limit;
    struct acpi_processor_flags flags;
    struct acpi_processor_power power;
    struct acpi_processor_performance *performance;
    struct acpi_processor_throttling throttling;
    struct acpi_processor_limit limit;
    struct thermal_cooling_device *cdev;
    struct device *dev;
    struct freq_qos_request perflib_req;
    struct freq_qos_request thermal_req;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct acpi_processor {
    acpi_handle handle;
    u32 acpi_id;
    phys_cpuid_t phys_id;
    u32 id;
    u32 pblk;
    int performance_platform_limit;
    int throttling_platform_limit;
    struct acpi_processor_flags flags;
    struct acpi_processor_power power;
    struct acpi_processor_performance *performance;
    struct acpi_processor_throttling throttling;
    struct acpi_processor_limit limit;
    struct thermal_cooling_device *cdev;
    struct device *dev;
    struct freq_qos_request perflib_req;
    struct freq_qos_request thermal_req;
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
struct acpi_processor {
    acpi_handle handle;
    u32 acpi_id;
    phys_cpuid_t phys_id;
    u32 id;
    u32 pblk;
    int performance_platform_limit;
    int throttling_platform_limit;
    struct acpi_processor_flags flags;
    struct acpi_processor_power power;
    struct acpi_processor_performance *performance;
    struct acpi_processor_throttling throttling;
    struct acpi_processor_limit limit;
    struct thermal_cooling_device *cdev;
    struct device *dev;
    struct freq_qos_request perflib_req;
    struct freq_qos_request thermal_req;
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct acpi_processor {
    acpi_handle handle;
    u32 acpi_id;
    phys_cpuid_t phys_id;
    u32 id;
    u32 pblk;
    int performance_platform_limit;
    int throttling_platform_limit;
    struct acpi_processor_flags flags;
    struct acpi_processor_power power;
    struct acpi_processor_performance *performance;
    struct acpi_processor_throttling throttling;
    struct acpi_processor_limit limit;
    struct thermal_cooling_device *cdev;
    struct device *dev;
    struct freq_qos_request perflib_req;
    struct freq_qos_request thermal_req;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct acpi_processor {
    acpi_handle handle;
    u32 acpi_id;
    phys_cpuid_t phys_id;
    u32 id;
    u32 pblk;
    int performance_platform_limit;
    int throttling_platform_limit;
    struct acpi_processor_flags flags;
    struct acpi_processor_power power;
    struct acpi_processor_performance *performance;
    struct acpi_processor_throttling throttling;
    struct acpi_processor_limit limit;
    struct thermal_cooling_device *cdev;
    struct device *dev;
    struct freq_qos_request perflib_req;
    struct freq_qos_request thermal_req;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct acpi_processor {
    acpi_handle handle;
    u32 acpi_id;
    phys_cpuid_t phys_id;
    u32 id;
    u32 pblk;
    int performance_platform_limit;
    int throttling_platform_limit;
    struct acpi_processor_flags flags;
    struct acpi_processor_power power;
    struct acpi_processor_performance *performance;
    struct acpi_processor_throttling throttling;
    struct acpi_processor_limit limit;
    struct thermal_cooling_device *cdev;
    struct device *dev;
    struct freq_qos_request perflib_req;
    struct freq_qos_request thermal_req;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct acpi_processor {
    acpi_handle handle;
    u32 acpi_id;
    phys_cpuid_t phys_id;
    u32 id;
    u32 pblk;
    int performance_platform_limit;
    int throttling_platform_limit;
    struct acpi_processor_flags flags;
    struct acpi_processor_power power;
    struct acpi_processor_performance *performance;
    struct acpi_processor_throttling throttling;
    struct acpi_processor_limit limit;
    struct thermal_cooling_device *cdev;
    struct device *dev;
    struct freq_qos_request perflib_req;
    struct freq_qos_request thermal_req;
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
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct freq_qos_request perflib_req</code>
</li>
<li>
<b>Field added. </b>
<code>struct freq_qos_request thermal_req</code>
</li>
</ul>
</details>
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
