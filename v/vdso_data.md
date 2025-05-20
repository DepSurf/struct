# Struct: <code>vdso_data</code>

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
struct vdso_data {
    u32 seq;
    s32 clock_mode;
    u64 cycle_last;
    u64 mask;
    u32 mult;
    u32 shift;
    struct vdso_timestamp basetime[12];
    s32 tz_minuteswest;
    s32 tz_dsttime;
    u32 hrtimer_res;
    u32 __unused;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct vdso_data {
    u32 seq;
    s32 clock_mode;
    u64 cycle_last;
    u64 mask;
    u32 mult;
    u32 shift;
    struct vdso_timestamp basetime[12];
    s32 tz_minuteswest;
    s32 tz_dsttime;
    u32 hrtimer_res;
    u32 __unused;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct vdso_data {
    u32 seq;
    s32 clock_mode;
    u64 cycle_last;
    u64 mask;
    u32 mult;
    u32 shift;
    struct vdso_timestamp basetime[12];
    struct timens_offset offset[12];
    s32 tz_minuteswest;
    s32 tz_dsttime;
    u32 hrtimer_res;
    u32 __unused;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct vdso_data {
    u32 seq;
    s32 clock_mode;
    u64 cycle_last;
    u64 mask;
    u32 mult;
    u32 shift;
    struct vdso_timestamp basetime[12];
    struct timens_offset offset[12];
    s32 tz_minuteswest;
    s32 tz_dsttime;
    u32 hrtimer_res;
    u32 __unused;
    struct arch_vdso_data arch_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct vdso_data {
    u32 seq;
    s32 clock_mode;
    u64 cycle_last;
    u64 mask;
    u32 mult;
    u32 shift;
    struct vdso_timestamp basetime[12];
    struct timens_offset offset[12];
    s32 tz_minuteswest;
    s32 tz_dsttime;
    u32 hrtimer_res;
    u32 __unused;
    struct arch_vdso_data arch_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct vdso_data {
    u32 seq;
    s32 clock_mode;
    u64 cycle_last;
    u64 mask;
    u32 mult;
    u32 shift;
    struct vdso_timestamp basetime[12];
    struct timens_offset offset[12];
    s32 tz_minuteswest;
    s32 tz_dsttime;
    u32 hrtimer_res;
    u32 __unused;
    struct arch_vdso_data arch_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct vdso_data {
    u32 seq;
    s32 clock_mode;
    u64 cycle_last;
    u64 mask;
    u32 mult;
    u32 shift;
    struct vdso_timestamp basetime[12];
    struct timens_offset offset[12];
    s32 tz_minuteswest;
    s32 tz_dsttime;
    u32 hrtimer_res;
    u32 __unused;
    struct arch_vdso_data arch_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct vdso_data {
    u32 seq;
    s32 clock_mode;
    u64 cycle_last;
    u64 mask;
    u32 mult;
    u32 shift;
    struct vdso_timestamp basetime[12];
    struct timens_offset offset[12];
    s32 tz_minuteswest;
    s32 tz_dsttime;
    u32 hrtimer_res;
    u32 __unused;
    struct arch_vdso_data arch_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct vdso_data {
    u32 seq;
    s32 clock_mode;
    u64 cycle_last;
    u64 mask;
    u32 mult;
    u32 shift;
    struct vdso_timestamp basetime[12];
    struct timens_offset offset[12];
    s32 tz_minuteswest;
    s32 tz_dsttime;
    u32 hrtimer_res;
    u32 __unused;
    struct arch_vdso_data arch_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct vdso_data {
    u32 seq;
    s32 clock_mode;
    u64 cycle_last;
    u64 mask;
    u32 mult;
    u32 shift;
    struct vdso_timestamp basetime[12];
    struct timens_offset offset[12];
    s32 tz_minuteswest;
    s32 tz_dsttime;
    u32 hrtimer_res;
    u32 __unused;
    struct arch_vdso_data arch_data;
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
struct vdso_data {
    u32 seq;
    s32 clock_mode;
    u64 cycle_last;
    u64 mask;
    u32 mult;
    u32 shift;
    struct vdso_timestamp basetime[12];
    s32 tz_minuteswest;
    s32 tz_dsttime;
    u32 hrtimer_res;
    u32 __unused;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct vdso_data {
    u32 seq_count;
    u16 tk_is_cntvct;
    u16 cs_shift;
    u32 xtime_coarse_sec;
    u32 xtime_coarse_nsec;
    u32 wtm_clock_sec;
    u32 wtm_clock_nsec;
    u32 xtime_clock_sec;
    u32 cs_mult;
    u64 cs_cycle_last;
    u64 cs_mask;
    u64 xtime_clock_snsec;
    u32 tz_minuteswest;
    u32 tz_dsttime;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct vdso_data {
    __u8 eye_catcher[16];
    struct (anon) version;
    __u32 platform;
    __u32 processor;
    __u64 processorCount;
    __u64 physicalMemorySize;
    __u64 tb_orig_stamp;
    __u64 tb_ticks_per_sec;
    __u64 tb_to_xs;
    __u64 stamp_xsec;
    __u64 tb_update_count;
    __u32 tz_minuteswest;
    __u32 tz_dsttime;
    __u32 dcache_size;
    __u32 dcache_line_size;
    __u32 icache_size;
    __u32 icache_line_size;
    __u32 dcache_block_size;
    __u32 icache_block_size;
    __u32 dcache_log_block_size;
    __u32 icache_log_block_size;
    __u32 stamp_sec_fraction;
    __s32 wtom_clock_nsec;
    __s64 wtom_clock_sec;
    struct timespec stamp_xtime;
    __u32 hrtimer_res;
    __u32 syscall_map_64[14];
    __u32 syscall_map_32[14];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct vdso_data {
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
struct vdso_data {
    u32 seq;
    s32 clock_mode;
    u64 cycle_last;
    u64 mask;
    u32 mult;
    u32 shift;
    struct vdso_timestamp basetime[12];
    s32 tz_minuteswest;
    s32 tz_dsttime;
    u32 hrtimer_res;
    u32 __unused;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct vdso_data {
    u32 seq;
    s32 clock_mode;
    u64 cycle_last;
    u64 mask;
    u32 mult;
    u32 shift;
    struct vdso_timestamp basetime[12];
    s32 tz_minuteswest;
    s32 tz_dsttime;
    u32 hrtimer_res;
    u32 __unused;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct vdso_data {
    u32 seq;
    s32 clock_mode;
    u64 cycle_last;
    u64 mask;
    u32 mult;
    u32 shift;
    struct vdso_timestamp basetime[12];
    s32 tz_minuteswest;
    s32 tz_dsttime;
    u32 hrtimer_res;
    u32 __unused;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct vdso_data {
    u32 seq;
    s32 clock_mode;
    u64 cycle_last;
    u64 mask;
    u32 mult;
    u32 shift;
    struct vdso_timestamp basetime[12];
    s32 tz_minuteswest;
    s32 tz_dsttime;
    u32 hrtimer_res;
    u32 __unused;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct timens_offset offset[12]</code>
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
<code>struct arch_vdso_data arch_data</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 seq_count</code>
</li>
<li>
<b>Field added. </b>
<code>u16 tk_is_cntvct</code>
</li>
<li>
<b>Field added. </b>
<code>u16 cs_shift</code>
</li>
<li>
<b>Field added. </b>
<code>u32 xtime_coarse_sec</code>
</li>
<li>
<b>Field added. </b>
<code>u32 xtime_coarse_nsec</code>
</li>
<li>
<b>Field added. </b>
<code>u32 wtm_clock_sec</code>
</li>
<li>
<b>Field added. </b>
<code>u32 wtm_clock_nsec</code>
</li>
<li>
<b>Field added. </b>
<code>u32 xtime_clock_sec</code>
</li>
<li>
<b>Field added. </b>
<code>u32 cs_mult</code>
</li>
<li>
<b>Field added. </b>
<code>u64 cs_cycle_last</code>
</li>
<li>
<b>Field added. </b>
<code>u64 cs_mask</code>
</li>
<li>
<b>Field added. </b>
<code>u64 xtime_clock_snsec</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 seq</code>
</li>
<li>
<b>Field removed. </b>
<code>s32 clock_mode</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 cycle_last</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 mask</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 mult</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 shift</code>
</li>
<li>
<b>Field removed. </b>
<code>struct vdso_timestamp basetime[12]</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 hrtimer_res</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 __unused</code>
</li>
<li>
<b>Field type changed. </b>
<code>s32 tz_minuteswest</code> ➡️ <code>u32 tz_minuteswest</code>
</li>
<li>
<b>Field type changed. </b>
<code>s32 tz_dsttime</code> ➡️ <code>u32 tz_dsttime</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u8 eye_catcher[16]</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) version</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 platform</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 processor</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 processorCount</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 physicalMemorySize</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 tb_orig_stamp</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 tb_ticks_per_sec</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 tb_to_xs</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 stamp_xsec</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 tb_update_count</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 dcache_size</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 dcache_line_size</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 icache_size</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 icache_line_size</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 dcache_block_size</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 icache_block_size</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 dcache_log_block_size</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 icache_log_block_size</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 stamp_sec_fraction</code>
</li>
<li>
<b>Field added. </b>
<code>__s32 wtom_clock_nsec</code>
</li>
<li>
<b>Field added. </b>
<code>__s64 wtom_clock_sec</code>
</li>
<li>
<b>Field added. </b>
<code>struct timespec stamp_xtime</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 syscall_map_64[14]</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 syscall_map_32[14]</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 seq</code>
</li>
<li>
<b>Field removed. </b>
<code>s32 clock_mode</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 cycle_last</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 mask</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 mult</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 shift</code>
</li>
<li>
<b>Field removed. </b>
<code>struct vdso_timestamp basetime[12]</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 __unused</code>
</li>
<li>
<b>Field type changed. </b>
<code>s32 tz_minuteswest</code> ➡️ <code>__u32 tz_minuteswest</code>
</li>
<li>
<b>Field type changed. </b>
<code>s32 tz_dsttime</code> ➡️ <code>__u32 tz_dsttime</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 hrtimer_res</code> ➡️ <code>__u32 hrtimer_res</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>u32 seq</code>
</li>
<li>
<b>Field removed. </b>
<code>s32 clock_mode</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 cycle_last</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 mask</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 mult</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 shift</code>
</li>
<li>
<b>Field removed. </b>
<code>struct vdso_timestamp basetime[12]</code>
</li>
<li>
<b>Field removed. </b>
<code>s32 tz_minuteswest</code>
</li>
<li>
<b>Field removed. </b>
<code>s32 tz_dsttime</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 hrtimer_res</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 __unused</code>
</li>
</ul>
</details>
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
