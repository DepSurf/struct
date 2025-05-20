# Struct: <code>timekeeper</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct timekeeper {
    struct tk_read_base tkr_mono;
    struct tk_read_base tkr_raw;
    u64 xtime_sec;
    long unsigned int ktime_sec;
    struct timespec wall_to_monotonic;
    ktime_t offs_real;
    ktime_t offs_boot;
    ktime_t offs_tai;
    s32 tai_offset;
    unsigned int clock_was_set_seq;
    u8 cs_was_changed_seq;
    ktime_t next_leap_ktime;
    struct timespec raw_time;
    cycle_t cycle_interval;
    u64 xtime_interval;
    s64 xtime_remainder;
    u32 raw_interval;
    u64 ntp_tick;
    s64 ntp_error;
    u32 ntp_error_shift;
    u32 ntp_err_mult;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct timekeeper {
    struct tk_read_base tkr_mono;
    struct tk_read_base tkr_raw;
    u64 xtime_sec;
    long unsigned int ktime_sec;
    struct timespec wall_to_monotonic;
    ktime_t offs_real;
    ktime_t offs_boot;
    ktime_t offs_tai;
    s32 tai_offset;
    unsigned int clock_was_set_seq;
    u8 cs_was_changed_seq;
    ktime_t next_leap_ktime;
    struct timespec raw_time;
    cycle_t cycle_interval;
    u64 xtime_interval;
    s64 xtime_remainder;
    u32 raw_interval;
    u64 ntp_tick;
    s64 ntp_error;
    u32 ntp_error_shift;
    u32 ntp_err_mult;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct timekeeper {
    struct tk_read_base tkr_mono;
    struct tk_read_base tkr_raw;
    u64 xtime_sec;
    long unsigned int ktime_sec;
    struct timespec wall_to_monotonic;
    ktime_t offs_real;
    ktime_t offs_boot;
    ktime_t offs_tai;
    s32 tai_offset;
    unsigned int clock_was_set_seq;
    u8 cs_was_changed_seq;
    ktime_t next_leap_ktime;
    struct timespec raw_time;
    u64 cycle_interval;
    u64 xtime_interval;
    s64 xtime_remainder;
    u32 raw_interval;
    u64 ntp_tick;
    s64 ntp_error;
    u32 ntp_error_shift;
    u32 ntp_err_mult;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct timekeeper {
    struct tk_read_base tkr_mono;
    struct tk_read_base tkr_raw;
    u64 xtime_sec;
    long unsigned int ktime_sec;
    struct timespec wall_to_monotonic;
    ktime_t offs_real;
    ktime_t offs_boot;
    ktime_t offs_tai;
    s32 tai_offset;
    unsigned int clock_was_set_seq;
    u8 cs_was_changed_seq;
    ktime_t next_leap_ktime;
    u64 raw_sec;
    u64 cycle_interval;
    u64 xtime_interval;
    s64 xtime_remainder;
    u64 raw_interval;
    u64 ntp_tick;
    s64 ntp_error;
    u32 ntp_error_shift;
    u32 ntp_err_mult;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct timekeeper {
    struct tk_read_base tkr_mono;
    struct tk_read_base tkr_raw;
    u64 xtime_sec;
    long unsigned int ktime_sec;
    struct timespec wall_to_monotonic;
    ktime_t offs_real;
    ktime_t offs_boot;
    ktime_t offs_tai;
    s32 tai_offset;
    unsigned int clock_was_set_seq;
    u8 cs_was_changed_seq;
    ktime_t next_leap_ktime;
    u64 raw_sec;
    u64 cycle_interval;
    u64 xtime_interval;
    s64 xtime_remainder;
    u64 raw_interval;
    u64 ntp_tick;
    s64 ntp_error;
    u32 ntp_error_shift;
    u32 ntp_err_mult;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct timekeeper {
    struct tk_read_base tkr_mono;
    struct tk_read_base tkr_raw;
    u64 xtime_sec;
    long unsigned int ktime_sec;
    struct timespec64 wall_to_monotonic;
    ktime_t offs_real;
    ktime_t offs_boot;
    ktime_t offs_tai;
    s32 tai_offset;
    unsigned int clock_was_set_seq;
    u8 cs_was_changed_seq;
    ktime_t next_leap_ktime;
    u64 raw_sec;
    u64 cycle_interval;
    u64 xtime_interval;
    s64 xtime_remainder;
    u64 raw_interval;
    u64 ntp_tick;
    s64 ntp_error;
    u32 ntp_error_shift;
    u32 ntp_err_mult;
    u32 skip_second_overflow;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct timekeeper {
    struct tk_read_base tkr_mono;
    struct tk_read_base tkr_raw;
    u64 xtime_sec;
    long unsigned int ktime_sec;
    struct timespec64 wall_to_monotonic;
    ktime_t offs_real;
    ktime_t offs_boot;
    ktime_t offs_tai;
    s32 tai_offset;
    unsigned int clock_was_set_seq;
    u8 cs_was_changed_seq;
    ktime_t next_leap_ktime;
    u64 raw_sec;
    u64 cycle_interval;
    u64 xtime_interval;
    s64 xtime_remainder;
    u64 raw_interval;
    u64 ntp_tick;
    s64 ntp_error;
    u32 ntp_error_shift;
    u32 ntp_err_mult;
    u32 skip_second_overflow;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct timekeeper {
    struct tk_read_base tkr_mono;
    struct tk_read_base tkr_raw;
    u64 xtime_sec;
    long unsigned int ktime_sec;
    struct timespec64 wall_to_monotonic;
    ktime_t offs_real;
    ktime_t offs_boot;
    ktime_t offs_tai;
    s32 tai_offset;
    unsigned int clock_was_set_seq;
    u8 cs_was_changed_seq;
    ktime_t next_leap_ktime;
    u64 raw_sec;
    struct timespec64 monotonic_to_boot;
    u64 cycle_interval;
    u64 xtime_interval;
    s64 xtime_remainder;
    u64 raw_interval;
    u64 ntp_tick;
    s64 ntp_error;
    u32 ntp_error_shift;
    u32 ntp_err_mult;
    u32 skip_second_overflow;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct timekeeper {
    struct tk_read_base tkr_mono;
    struct tk_read_base tkr_raw;
    u64 xtime_sec;
    long unsigned int ktime_sec;
    struct timespec64 wall_to_monotonic;
    ktime_t offs_real;
    ktime_t offs_boot;
    ktime_t offs_tai;
    s32 tai_offset;
    unsigned int clock_was_set_seq;
    u8 cs_was_changed_seq;
    ktime_t next_leap_ktime;
    u64 raw_sec;
    struct timespec64 monotonic_to_boot;
    u64 cycle_interval;
    u64 xtime_interval;
    s64 xtime_remainder;
    u64 raw_interval;
    u64 ntp_tick;
    s64 ntp_error;
    u32 ntp_error_shift;
    u32 ntp_err_mult;
    u32 skip_second_overflow;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct timekeeper {
    struct tk_read_base tkr_mono;
    struct tk_read_base tkr_raw;
    u64 xtime_sec;
    long unsigned int ktime_sec;
    struct timespec64 wall_to_monotonic;
    ktime_t offs_real;
    ktime_t offs_boot;
    ktime_t offs_tai;
    s32 tai_offset;
    unsigned int clock_was_set_seq;
    u8 cs_was_changed_seq;
    ktime_t next_leap_ktime;
    u64 raw_sec;
    struct timespec64 monotonic_to_boot;
    u64 cycle_interval;
    u64 xtime_interval;
    s64 xtime_remainder;
    u64 raw_interval;
    u64 ntp_tick;
    s64 ntp_error;
    u32 ntp_error_shift;
    u32 ntp_err_mult;
    u32 skip_second_overflow;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct timekeeper {
    struct tk_read_base tkr_mono;
    struct tk_read_base tkr_raw;
    u64 xtime_sec;
    long unsigned int ktime_sec;
    struct timespec64 wall_to_monotonic;
    ktime_t offs_real;
    ktime_t offs_boot;
    ktime_t offs_tai;
    s32 tai_offset;
    unsigned int clock_was_set_seq;
    u8 cs_was_changed_seq;
    ktime_t next_leap_ktime;
    u64 raw_sec;
    struct timespec64 monotonic_to_boot;
    u64 cycle_interval;
    u64 xtime_interval;
    s64 xtime_remainder;
    u64 raw_interval;
    u64 ntp_tick;
    s64 ntp_error;
    u32 ntp_error_shift;
    u32 ntp_err_mult;
    u32 skip_second_overflow;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct timekeeper {
    struct tk_read_base tkr_mono;
    struct tk_read_base tkr_raw;
    u64 xtime_sec;
    long unsigned int ktime_sec;
    struct timespec64 wall_to_monotonic;
    ktime_t offs_real;
    ktime_t offs_boot;
    ktime_t offs_tai;
    s32 tai_offset;
    unsigned int clock_was_set_seq;
    u8 cs_was_changed_seq;
    ktime_t next_leap_ktime;
    u64 raw_sec;
    struct timespec64 monotonic_to_boot;
    u64 cycle_interval;
    u64 xtime_interval;
    s64 xtime_remainder;
    u64 raw_interval;
    u64 ntp_tick;
    s64 ntp_error;
    u32 ntp_error_shift;
    u32 ntp_err_mult;
    u32 skip_second_overflow;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct timekeeper {
    struct tk_read_base tkr_mono;
    struct tk_read_base tkr_raw;
    u64 xtime_sec;
    long unsigned int ktime_sec;
    struct timespec64 wall_to_monotonic;
    ktime_t offs_real;
    ktime_t offs_boot;
    ktime_t offs_tai;
    s32 tai_offset;
    unsigned int clock_was_set_seq;
    u8 cs_was_changed_seq;
    ktime_t next_leap_ktime;
    u64 raw_sec;
    struct timespec64 monotonic_to_boot;
    u64 cycle_interval;
    u64 xtime_interval;
    s64 xtime_remainder;
    u64 raw_interval;
    u64 ntp_tick;
    s64 ntp_error;
    u32 ntp_error_shift;
    u32 ntp_err_mult;
    u32 skip_second_overflow;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct timekeeper {
    struct tk_read_base tkr_mono;
    struct tk_read_base tkr_raw;
    u64 xtime_sec;
    long unsigned int ktime_sec;
    struct timespec64 wall_to_monotonic;
    ktime_t offs_real;
    ktime_t offs_boot;
    ktime_t offs_tai;
    s32 tai_offset;
    unsigned int clock_was_set_seq;
    u8 cs_was_changed_seq;
    ktime_t next_leap_ktime;
    u64 raw_sec;
    struct timespec64 monotonic_to_boot;
    u64 cycle_interval;
    u64 xtime_interval;
    s64 xtime_remainder;
    u64 raw_interval;
    u64 ntp_tick;
    s64 ntp_error;
    u32 ntp_error_shift;
    u32 ntp_err_mult;
    u32 skip_second_overflow;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct timekeeper {
    struct tk_read_base tkr_mono;
    struct tk_read_base tkr_raw;
    u64 xtime_sec;
    long unsigned int ktime_sec;
    struct timespec64 wall_to_monotonic;
    ktime_t offs_real;
    ktime_t offs_boot;
    ktime_t offs_tai;
    s32 tai_offset;
    unsigned int clock_was_set_seq;
    u8 cs_was_changed_seq;
    ktime_t next_leap_ktime;
    u64 raw_sec;
    struct timespec64 monotonic_to_boot;
    u64 cycle_interval;
    u64 xtime_interval;
    s64 xtime_remainder;
    u64 raw_interval;
    u64 ntp_tick;
    s64 ntp_error;
    u32 ntp_error_shift;
    u32 ntp_err_mult;
    u32 skip_second_overflow;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct timekeeper {
    struct tk_read_base tkr_mono;
    struct tk_read_base tkr_raw;
    u64 xtime_sec;
    long unsigned int ktime_sec;
    struct timespec64 wall_to_monotonic;
    ktime_t offs_real;
    ktime_t offs_boot;
    ktime_t offs_tai;
    s32 tai_offset;
    unsigned int clock_was_set_seq;
    u8 cs_was_changed_seq;
    ktime_t next_leap_ktime;
    u64 raw_sec;
    struct timespec64 monotonic_to_boot;
    u64 cycle_interval;
    u64 xtime_interval;
    s64 xtime_remainder;
    u64 raw_interval;
    u64 ntp_tick;
    s64 ntp_error;
    u32 ntp_error_shift;
    u32 ntp_err_mult;
    u32 skip_second_overflow;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct timekeeper {
    struct tk_read_base tkr_mono;
    struct tk_read_base tkr_raw;
    u64 xtime_sec;
    long unsigned int ktime_sec;
    struct timespec64 wall_to_monotonic;
    ktime_t offs_real;
    ktime_t offs_boot;
    ktime_t offs_tai;
    s32 tai_offset;
    unsigned int clock_was_set_seq;
    u8 cs_was_changed_seq;
    ktime_t next_leap_ktime;
    u64 raw_sec;
    struct timespec64 monotonic_to_boot;
    u64 cycle_interval;
    u64 xtime_interval;
    s64 xtime_remainder;
    u64 raw_interval;
    u64 ntp_tick;
    s64 ntp_error;
    u32 ntp_error_shift;
    u32 ntp_err_mult;
    u32 skip_second_overflow;
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
struct timekeeper {
    struct tk_read_base tkr_mono;
    struct tk_read_base tkr_raw;
    u64 xtime_sec;
    long unsigned int ktime_sec;
    struct timespec64 wall_to_monotonic;
    ktime_t offs_real;
    ktime_t offs_boot;
    ktime_t offs_tai;
    s32 tai_offset;
    unsigned int clock_was_set_seq;
    u8 cs_was_changed_seq;
    ktime_t next_leap_ktime;
    u64 raw_sec;
    struct timespec64 monotonic_to_boot;
    u64 cycle_interval;
    u64 xtime_interval;
    s64 xtime_remainder;
    u64 raw_interval;
    u64 ntp_tick;
    s64 ntp_error;
    u32 ntp_error_shift;
    u32 ntp_err_mult;
    u32 skip_second_overflow;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct timekeeper {
    struct tk_read_base tkr_mono;
    struct tk_read_base tkr_raw;
    u64 xtime_sec;
    long unsigned int ktime_sec;
    struct timespec64 wall_to_monotonic;
    ktime_t offs_real;
    ktime_t offs_boot;
    ktime_t offs_tai;
    s32 tai_offset;
    unsigned int clock_was_set_seq;
    u8 cs_was_changed_seq;
    ktime_t next_leap_ktime;
    u64 raw_sec;
    struct timespec64 monotonic_to_boot;
    u64 cycle_interval;
    u64 xtime_interval;
    s64 xtime_remainder;
    u64 raw_interval;
    u64 ntp_tick;
    s64 ntp_error;
    u32 ntp_error_shift;
    u32 ntp_err_mult;
    u32 skip_second_overflow;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct timekeeper {
    struct tk_read_base tkr_mono;
    struct tk_read_base tkr_raw;
    u64 xtime_sec;
    long unsigned int ktime_sec;
    struct timespec64 wall_to_monotonic;
    ktime_t offs_real;
    ktime_t offs_boot;
    ktime_t offs_tai;
    s32 tai_offset;
    unsigned int clock_was_set_seq;
    u8 cs_was_changed_seq;
    ktime_t next_leap_ktime;
    u64 raw_sec;
    struct timespec64 monotonic_to_boot;
    u64 cycle_interval;
    u64 xtime_interval;
    s64 xtime_remainder;
    u64 raw_interval;
    u64 ntp_tick;
    s64 ntp_error;
    u32 ntp_error_shift;
    u32 ntp_err_mult;
    u32 skip_second_overflow;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct timekeeper {
    struct tk_read_base tkr_mono;
    struct tk_read_base tkr_raw;
    u64 xtime_sec;
    long unsigned int ktime_sec;
    struct timespec64 wall_to_monotonic;
    ktime_t offs_real;
    ktime_t offs_boot;
    ktime_t offs_tai;
    s32 tai_offset;
    unsigned int clock_was_set_seq;
    u8 cs_was_changed_seq;
    ktime_t next_leap_ktime;
    u64 raw_sec;
    struct timespec64 monotonic_to_boot;
    u64 cycle_interval;
    u64 xtime_interval;
    s64 xtime_remainder;
    u64 raw_interval;
    u64 ntp_tick;
    s64 ntp_error;
    u32 ntp_error_shift;
    u32 ntp_err_mult;
    u32 skip_second_overflow;
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
struct timekeeper {
    struct tk_read_base tkr_mono;
    struct tk_read_base tkr_raw;
    u64 xtime_sec;
    long unsigned int ktime_sec;
    struct timespec64 wall_to_monotonic;
    ktime_t offs_real;
    ktime_t offs_boot;
    ktime_t offs_tai;
    s32 tai_offset;
    unsigned int clock_was_set_seq;
    u8 cs_was_changed_seq;
    ktime_t next_leap_ktime;
    u64 raw_sec;
    struct timespec64 monotonic_to_boot;
    u64 cycle_interval;
    u64 xtime_interval;
    s64 xtime_remainder;
    u64 raw_interval;
    u64 ntp_tick;
    s64 ntp_error;
    u32 ntp_error_shift;
    u32 ntp_err_mult;
    u32 skip_second_overflow;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct timekeeper {
    struct tk_read_base tkr_mono;
    struct tk_read_base tkr_raw;
    u64 xtime_sec;
    long unsigned int ktime_sec;
    struct timespec64 wall_to_monotonic;
    ktime_t offs_real;
    ktime_t offs_boot;
    ktime_t offs_tai;
    s32 tai_offset;
    unsigned int clock_was_set_seq;
    u8 cs_was_changed_seq;
    ktime_t next_leap_ktime;
    u64 raw_sec;
    struct timespec64 monotonic_to_boot;
    u64 cycle_interval;
    u64 xtime_interval;
    s64 xtime_remainder;
    u64 raw_interval;
    u64 ntp_tick;
    s64 ntp_error;
    u32 ntp_error_shift;
    u32 ntp_err_mult;
    u32 skip_second_overflow;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct timekeeper {
    struct tk_read_base tkr_mono;
    struct tk_read_base tkr_raw;
    u64 xtime_sec;
    long unsigned int ktime_sec;
    struct timespec64 wall_to_monotonic;
    ktime_t offs_real;
    ktime_t offs_boot;
    ktime_t offs_tai;
    s32 tai_offset;
    unsigned int clock_was_set_seq;
    u8 cs_was_changed_seq;
    ktime_t next_leap_ktime;
    u64 raw_sec;
    struct timespec64 monotonic_to_boot;
    u64 cycle_interval;
    u64 xtime_interval;
    s64 xtime_remainder;
    u64 raw_interval;
    u64 ntp_tick;
    s64 ntp_error;
    u32 ntp_error_shift;
    u32 ntp_err_mult;
    u32 skip_second_overflow;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct timekeeper {
    struct tk_read_base tkr_mono;
    struct tk_read_base tkr_raw;
    u64 xtime_sec;
    long unsigned int ktime_sec;
    struct timespec64 wall_to_monotonic;
    ktime_t offs_real;
    ktime_t offs_boot;
    ktime_t offs_tai;
    s32 tai_offset;
    unsigned int clock_was_set_seq;
    u8 cs_was_changed_seq;
    ktime_t next_leap_ktime;
    u64 raw_sec;
    struct timespec64 monotonic_to_boot;
    u64 cycle_interval;
    u64 xtime_interval;
    s64 xtime_remainder;
    u64 raw_interval;
    u64 ntp_tick;
    s64 ntp_error;
    u32 ntp_error_shift;
    u32 ntp_err_mult;
    u32 skip_second_overflow;
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
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>cycle_t cycle_interval</code> ➡️ <code>u64 cycle_interval</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 raw_sec</code>
</li>
<li>
<b>Field removed. </b>
<code>struct timespec raw_time</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 raw_interval</code> ➡️ <code>u64 raw_interval</code>
</li>
</ul>
</details>
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
<code>u32 skip_second_overflow</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct timespec wall_to_monotonic</code> ➡️ <code>struct timespec64 wall_to_monotonic</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct timespec64 monotonic_to_boot</code>
</li>
</ul>
</details>
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
