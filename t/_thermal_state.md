# Struct: <code>_thermal_state</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct _thermal_state {
    bool new_event;
    int event;
    u64 next_check;
    long unsigned int count;
    long unsigned int last_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct _thermal_state {
    bool new_event;
    int event;
    u64 next_check;
    long unsigned int count;
    long unsigned int last_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct _thermal_state {
    bool new_event;
    int event;
    u64 next_check;
    long unsigned int count;
    long unsigned int last_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct _thermal_state {
    bool new_event;
    int event;
    u64 next_check;
    long unsigned int count;
    long unsigned int last_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct _thermal_state {
    bool new_event;
    int event;
    u64 next_check;
    long unsigned int count;
    long unsigned int last_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct _thermal_state {
    bool new_event;
    int event;
    u64 next_check;
    long unsigned int count;
    long unsigned int last_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct _thermal_state {
    bool new_event;
    int event;
    u64 next_check;
    long unsigned int count;
    long unsigned int last_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct _thermal_state {
    bool new_event;
    int event;
    u64 next_check;
    long unsigned int count;
    long unsigned int last_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct _thermal_state {
    bool new_event;
    int event;
    u64 next_check;
    long unsigned int count;
    long unsigned int last_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct _thermal_state {
    u64 next_check;
    u64 last_interrupt_time;
    struct delayed_work therm_work;
    long unsigned int count;
    long unsigned int last_count;
    long unsigned int max_time_ms;
    long unsigned int total_time_ms;
    bool rate_control_active;
    bool new_event;
    u8 level;
    u8 sample_index;
    u8 sample_count;
    u8 average;
    u8 baseline_temp;
    u8 temp_samples[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct _thermal_state {
    u64 next_check;
    u64 last_interrupt_time;
    struct delayed_work therm_work;
    long unsigned int count;
    long unsigned int last_count;
    long unsigned int max_time_ms;
    long unsigned int total_time_ms;
    bool rate_control_active;
    bool new_event;
    u8 level;
    u8 sample_index;
    u8 sample_count;
    u8 average;
    u8 baseline_temp;
    u8 temp_samples[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct _thermal_state {
    u64 next_check;
    u64 last_interrupt_time;
    struct delayed_work therm_work;
    long unsigned int count;
    long unsigned int last_count;
    long unsigned int max_time_ms;
    long unsigned int total_time_ms;
    bool rate_control_active;
    bool new_event;
    u8 level;
    u8 sample_index;
    u8 sample_count;
    u8 average;
    u8 baseline_temp;
    u8 temp_samples[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct _thermal_state {
    u64 next_check;
    u64 last_interrupt_time;
    struct delayed_work therm_work;
    long unsigned int count;
    long unsigned int last_count;
    long unsigned int max_time_ms;
    long unsigned int total_time_ms;
    bool rate_control_active;
    bool new_event;
    u8 level;
    u8 sample_index;
    u8 sample_count;
    u8 average;
    u8 baseline_temp;
    u8 temp_samples[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct _thermal_state {
    u64 next_check;
    u64 last_interrupt_time;
    struct delayed_work therm_work;
    long unsigned int count;
    long unsigned int last_count;
    long unsigned int max_time_ms;
    long unsigned int total_time_ms;
    bool rate_control_active;
    bool new_event;
    u8 level;
    u8 sample_index;
    u8 sample_count;
    u8 average;
    u8 baseline_temp;
    u8 temp_samples[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct _thermal_state {
    u64 next_check;
    u64 last_interrupt_time;
    struct delayed_work therm_work;
    long unsigned int count;
    long unsigned int last_count;
    long unsigned int max_time_ms;
    long unsigned int total_time_ms;
    bool rate_control_active;
    bool new_event;
    u8 level;
    u8 sample_index;
    u8 sample_count;
    u8 average;
    u8 baseline_temp;
    u8 temp_samples[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct _thermal_state {
    u64 next_check;
    u64 last_interrupt_time;
    struct delayed_work therm_work;
    long unsigned int count;
    long unsigned int last_count;
    long unsigned int max_time_ms;
    long unsigned int total_time_ms;
    bool rate_control_active;
    bool new_event;
    u8 level;
    u8 sample_index;
    u8 sample_count;
    u8 average;
    u8 baseline_temp;
    u8 temp_samples[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct _thermal_state {
    u64 next_check;
    u64 last_interrupt_time;
    struct delayed_work therm_work;
    long unsigned int count;
    long unsigned int last_count;
    long unsigned int max_time_ms;
    long unsigned int total_time_ms;
    bool rate_control_active;
    bool new_event;
    u8 level;
    u8 sample_index;
    u8 sample_count;
    u8 average;
    u8 baseline_temp;
    u8 temp_samples[3];
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct _thermal_state {
    bool new_event;
    int event;
    u64 next_check;
    long unsigned int count;
    long unsigned int last_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct _thermal_state {
    bool new_event;
    int event;
    u64 next_check;
    long unsigned int count;
    long unsigned int last_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct _thermal_state {
    bool new_event;
    int event;
    u64 next_check;
    long unsigned int count;
    long unsigned int last_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct _thermal_state {
    bool new_event;
    int event;
    u64 next_check;
    long unsigned int count;
    long unsigned int last_count;
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 last_interrupt_time</code>
</li>
<li>
<b>Field added. </b>
<code>struct delayed_work therm_work</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int max_time_ms</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int total_time_ms</code>
</li>
<li>
<b>Field added. </b>
<code>bool rate_control_active</code>
</li>
<li>
<b>Field added. </b>
<code>u8 level</code>
</li>
<li>
<b>Field added. </b>
<code>u8 sample_index</code>
</li>
<li>
<b>Field added. </b>
<code>u8 sample_count</code>
</li>
<li>
<b>Field added. </b>
<code>u8 average</code>
</li>
<li>
<b>Field added. </b>
<code>u8 baseline_temp</code>
</li>
<li>
<b>Field added. </b>
<code>u8 temp_samples[3]</code>
</li>
<li>
<b>Field removed. </b>
<code>int event</code>
</li>
</ul>
</details>
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
