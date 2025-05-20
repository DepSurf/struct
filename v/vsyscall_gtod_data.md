# Struct: <code>vsyscall_gtod_data</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct vsyscall_gtod_data {
    unsigned int seq;
    int vclock_mode;
    cycle_t cycle_last;
    cycle_t mask;
    u32 mult;
    u32 shift;
    u64 wall_time_snsec;
    gtod_long_t wall_time_sec;
    gtod_long_t monotonic_time_sec;
    u64 monotonic_time_snsec;
    gtod_long_t wall_time_coarse_sec;
    gtod_long_t wall_time_coarse_nsec;
    gtod_long_t monotonic_time_coarse_sec;
    gtod_long_t monotonic_time_coarse_nsec;
    int tz_minuteswest;
    int tz_dsttime;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct vsyscall_gtod_data {
    unsigned int seq;
    int vclock_mode;
    cycle_t cycle_last;
    cycle_t mask;
    u32 mult;
    u32 shift;
    u64 wall_time_snsec;
    gtod_long_t wall_time_sec;
    gtod_long_t monotonic_time_sec;
    u64 monotonic_time_snsec;
    gtod_long_t wall_time_coarse_sec;
    gtod_long_t wall_time_coarse_nsec;
    gtod_long_t monotonic_time_coarse_sec;
    gtod_long_t monotonic_time_coarse_nsec;
    int tz_minuteswest;
    int tz_dsttime;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct vsyscall_gtod_data {
    unsigned int seq;
    int vclock_mode;
    u64 cycle_last;
    u64 mask;
    u32 mult;
    u32 shift;
    u64 wall_time_snsec;
    gtod_long_t wall_time_sec;
    gtod_long_t monotonic_time_sec;
    u64 monotonic_time_snsec;
    gtod_long_t wall_time_coarse_sec;
    gtod_long_t wall_time_coarse_nsec;
    gtod_long_t monotonic_time_coarse_sec;
    gtod_long_t monotonic_time_coarse_nsec;
    int tz_minuteswest;
    int tz_dsttime;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct vsyscall_gtod_data {
    unsigned int seq;
    int vclock_mode;
    u64 cycle_last;
    u64 mask;
    u32 mult;
    u32 shift;
    u64 wall_time_snsec;
    gtod_long_t wall_time_sec;
    gtod_long_t monotonic_time_sec;
    u64 monotonic_time_snsec;
    gtod_long_t wall_time_coarse_sec;
    gtod_long_t wall_time_coarse_nsec;
    gtod_long_t monotonic_time_coarse_sec;
    gtod_long_t monotonic_time_coarse_nsec;
    int tz_minuteswest;
    int tz_dsttime;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct vsyscall_gtod_data {
    unsigned int seq;
    int vclock_mode;
    u64 cycle_last;
    u64 mask;
    u32 mult;
    u32 shift;
    u64 wall_time_snsec;
    gtod_long_t wall_time_sec;
    gtod_long_t monotonic_time_sec;
    u64 monotonic_time_snsec;
    gtod_long_t wall_time_coarse_sec;
    gtod_long_t wall_time_coarse_nsec;
    gtod_long_t monotonic_time_coarse_sec;
    gtod_long_t monotonic_time_coarse_nsec;
    int tz_minuteswest;
    int tz_dsttime;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct vsyscall_gtod_data {
    unsigned int seq;
    int vclock_mode;
    u64 cycle_last;
    u64 mask;
    u32 mult;
    u32 shift;
    u64 wall_time_snsec;
    gtod_long_t wall_time_sec;
    gtod_long_t monotonic_time_sec;
    u64 monotonic_time_snsec;
    gtod_long_t wall_time_coarse_sec;
    gtod_long_t wall_time_coarse_nsec;
    gtod_long_t monotonic_time_coarse_sec;
    gtod_long_t monotonic_time_coarse_nsec;
    int tz_minuteswest;
    int tz_dsttime;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct vsyscall_gtod_data {
    unsigned int seq;
    int vclock_mode;
    u64 cycle_last;
    u64 mask;
    u32 mult;
    u32 shift;
    struct vgtod_ts basetime[12];
    int tz_minuteswest;
    int tz_dsttime;
};
```
</details>
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
No changes between <code>4.4</code> and <code>4.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>cycle_t cycle_last</code> ➡️ <code>u64 cycle_last</code>
</li>
<li>
<b>Field type changed. </b>
<code>cycle_t mask</code> ➡️ <code>u64 mask</code>
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
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct vgtod_ts basetime[12]</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 wall_time_snsec</code>
</li>
<li>
<b>Field removed. </b>
<code>gtod_long_t wall_time_sec</code>
</li>
<li>
<b>Field removed. </b>
<code>gtod_long_t monotonic_time_sec</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 monotonic_time_snsec</code>
</li>
<li>
<b>Field removed. </b>
<code>gtod_long_t wall_time_coarse_sec</code>
</li>
<li>
<b>Field removed. </b>
<code>gtod_long_t wall_time_coarse_nsec</code>
</li>
<li>
<b>Field removed. </b>
<code>gtod_long_t monotonic_time_coarse_sec</code>
</li>
<li>
<b>Field removed. </b>
<code>gtod_long_t monotonic_time_coarse_nsec</code>
</li>
</ul>
</details>
</li>
</ul>
