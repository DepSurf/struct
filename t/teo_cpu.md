# Struct: <code>teo_cpu</code>

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
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct teo_cpu {
    u64 time_span_ns;
    u64 sleep_length_ns;
    struct teo_idle_state states[10];
    int last_state;
    int interval_idx;
    unsigned int intervals[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct teo_cpu {
    u64 time_span_ns;
    u64 sleep_length_ns;
    struct teo_idle_state states[10];
    int interval_idx;
    unsigned int intervals[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct teo_cpu {
    u64 time_span_ns;
    u64 sleep_length_ns;
    struct teo_idle_state states[10];
    int interval_idx;
    u64 intervals[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct teo_cpu {
    u64 time_span_ns;
    u64 sleep_length_ns;
    struct teo_idle_state states[10];
    int interval_idx;
    u64 intervals[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct teo_cpu {
    s64 time_span_ns;
    s64 sleep_length_ns;
    struct teo_idle_state states[10];
    int interval_idx;
    u64 intervals[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct teo_cpu {
    s64 time_span_ns;
    s64 sleep_length_ns;
    struct teo_bin state_bins[10];
    unsigned int total;
    int next_recent_idx;
    int recent_idx[9];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct teo_cpu {
    s64 time_span_ns;
    s64 sleep_length_ns;
    struct teo_bin state_bins[10];
    unsigned int total;
    int next_recent_idx;
    int recent_idx[9];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct teo_cpu {
    s64 time_span_ns;
    s64 sleep_length_ns;
    struct teo_bin state_bins[10];
    unsigned int total;
    int next_recent_idx;
    int recent_idx[9];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct teo_cpu {
    s64 time_span_ns;
    s64 sleep_length_ns;
    struct teo_bin state_bins[10];
    unsigned int total;
    int next_recent_idx;
    int recent_idx[9];
    long unsigned int util_threshold;
    bool utilized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct teo_cpu {
    s64 time_span_ns;
    s64 sleep_length_ns;
    struct teo_bin state_bins[10];
    unsigned int total;
    int next_recent_idx;
    int recent_idx[9];
    unsigned int tick_hits;
    long unsigned int util_threshold;
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
struct teo_cpu {
    u64 time_span_ns;
    u64 sleep_length_ns;
    struct teo_idle_state states[10];
    int interval_idx;
    unsigned int intervals[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct teo_cpu {
    u64 time_span_ns;
    u64 sleep_length_ns;
    struct teo_idle_state states[10];
    int interval_idx;
    unsigned int intervals[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct teo_cpu {
    u64 time_span_ns;
    u64 sleep_length_ns;
    struct teo_idle_state states[10];
    int interval_idx;
    unsigned int intervals[8];
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct teo_cpu {
    u64 time_span_ns;
    u64 sleep_length_ns;
    struct teo_idle_state states[10];
    int interval_idx;
    unsigned int intervals[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct teo_cpu {
    u64 time_span_ns;
    u64 sleep_length_ns;
    struct teo_idle_state states[10];
    int interval_idx;
    unsigned int intervals[8];
};
```
</details>
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct teo_cpu {
    u64 time_span_ns;
    u64 sleep_length_ns;
    struct teo_idle_state states[10];
    int interval_idx;
    unsigned int intervals[8];
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
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int last_state</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>unsigned int intervals[8]</code> ➡️ <code>u64 intervals[8]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>u64 time_span_ns</code> ➡️ <code>s64 time_span_ns</code>
</li>
<li>
<b>Field type changed. </b>
<code>u64 sleep_length_ns</code> ➡️ <code>s64 sleep_length_ns</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct teo_bin state_bins[10]</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int total</code>
</li>
<li>
<b>Field added. </b>
<code>int next_recent_idx</code>
</li>
<li>
<b>Field added. </b>
<code>int recent_idx[9]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct teo_idle_state states[10]</code>
</li>
<li>
<b>Field removed. </b>
<code>int interval_idx</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 intervals[8]</code>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int util_threshold</code>
</li>
<li>
<b>Field added. </b>
<code>bool utilized</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int tick_hits</code>
</li>
<li>
<b>Field removed. </b>
<code>bool utilized</code>
</li>
</ul>
</details>
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
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
