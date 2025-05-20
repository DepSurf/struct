# Struct: <code>trace_event_raw_thermal_power_cpu_get_power</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct trace_event_raw_thermal_power_cpu_get_power {
    struct trace_entry ent;
    u32 __data_loc_cpumask;
    long unsigned int freq;
    u32 __data_loc_load;
    size_t load_len;
    u32 dynamic_power;
    u32 static_power;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct trace_event_raw_thermal_power_cpu_get_power {
    struct trace_entry ent;
    u32 __data_loc_cpumask;
    long unsigned int freq;
    u32 __data_loc_load;
    size_t load_len;
    u32 dynamic_power;
    u32 static_power;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct trace_event_raw_thermal_power_cpu_get_power {
    struct trace_entry ent;
    u32 __data_loc_cpumask;
    long unsigned int freq;
    u32 __data_loc_load;
    size_t load_len;
    u32 dynamic_power;
    u32 static_power;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct trace_event_raw_thermal_power_cpu_get_power {
    struct trace_entry ent;
    u32 __data_loc_cpumask;
    long unsigned int freq;
    u32 __data_loc_load;
    size_t load_len;
    u32 dynamic_power;
    u32 static_power;
    char __data[0];
};
```
</details>
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
In <code>5.8</code>: Absent ⚠️
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
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
struct trace_event_raw_thermal_power_cpu_get_power {
    struct trace_entry ent;
    u32 __data_loc_cpumask;
    long unsigned int freq;
    u32 __data_loc_load;
    size_t load_len;
    u32 dynamic_power;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct trace_event_raw_thermal_power_cpu_get_power {
    struct trace_entry ent;
    u32 __data_loc_cpumask;
    long unsigned int freq;
    u32 __data_loc_load;
    size_t load_len;
    u32 dynamic_power;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct trace_event_raw_thermal_power_cpu_get_power {
    struct trace_entry ent;
    u32 __data_loc_cpumask;
    long unsigned int freq;
    u32 __data_loc_load;
    size_t load_len;
    u32 dynamic_power;
    char __data[0];
};
```
</details>
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
No changes between <code>4.4</code> and <code>4.8</code> ✅
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
</ul>
<b>Arch</b>
<ul>
</ul>
