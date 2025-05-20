# Struct: <code>perf_event_mmap_page</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct perf_event_mmap_page {
    __u32 version;
    __u32 compat_version;
    __u32 lock;
    __u32 index;
    __s64 offset;
    __u64 time_enabled;
    __u64 time_running;
    __u64 capabilities;
    __u64 cap_bit0;
    __u64 cap_bit0_is_deprecated;
    __u64 cap_user_rdpmc;
    __u64 cap_user_time;
    __u64 cap_user_time_zero;
    __u64 cap_____res;
    __u16 pmc_width;
    __u16 time_shift;
    __u32 time_mult;
    __u64 time_offset;
    __u64 time_zero;
    __u32 size;
    __u8 __reserved[948];
    __u64 data_head;
    __u64 data_tail;
    __u64 data_offset;
    __u64 data_size;
    __u64 aux_head;
    __u64 aux_tail;
    __u64 aux_offset;
    __u64 aux_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct perf_event_mmap_page {
    __u32 version;
    __u32 compat_version;
    __u32 lock;
    __u32 index;
    __s64 offset;
    __u64 time_enabled;
    __u64 time_running;
    __u64 capabilities;
    __u64 cap_bit0;
    __u64 cap_bit0_is_deprecated;
    __u64 cap_user_rdpmc;
    __u64 cap_user_time;
    __u64 cap_user_time_zero;
    __u64 cap_____res;
    __u16 pmc_width;
    __u16 time_shift;
    __u32 time_mult;
    __u64 time_offset;
    __u64 time_zero;
    __u32 size;
    __u8 __reserved[948];
    __u64 data_head;
    __u64 data_tail;
    __u64 data_offset;
    __u64 data_size;
    __u64 aux_head;
    __u64 aux_tail;
    __u64 aux_offset;
    __u64 aux_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct perf_event_mmap_page {
    __u32 version;
    __u32 compat_version;
    __u32 lock;
    __u32 index;
    __s64 offset;
    __u64 time_enabled;
    __u64 time_running;
    __u64 capabilities;
    __u64 cap_bit0;
    __u64 cap_bit0_is_deprecated;
    __u64 cap_user_rdpmc;
    __u64 cap_user_time;
    __u64 cap_user_time_zero;
    __u64 cap_____res;
    __u16 pmc_width;
    __u16 time_shift;
    __u32 time_mult;
    __u64 time_offset;
    __u64 time_zero;
    __u32 size;
    __u8 __reserved[948];
    __u64 data_head;
    __u64 data_tail;
    __u64 data_offset;
    __u64 data_size;
    __u64 aux_head;
    __u64 aux_tail;
    __u64 aux_offset;
    __u64 aux_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct perf_event_mmap_page {
    __u32 version;
    __u32 compat_version;
    __u32 lock;
    __u32 index;
    __s64 offset;
    __u64 time_enabled;
    __u64 time_running;
    __u64 capabilities;
    __u64 cap_bit0;
    __u64 cap_bit0_is_deprecated;
    __u64 cap_user_rdpmc;
    __u64 cap_user_time;
    __u64 cap_user_time_zero;
    __u64 cap_____res;
    __u16 pmc_width;
    __u16 time_shift;
    __u32 time_mult;
    __u64 time_offset;
    __u64 time_zero;
    __u32 size;
    __u8 __reserved[948];
    __u64 data_head;
    __u64 data_tail;
    __u64 data_offset;
    __u64 data_size;
    __u64 aux_head;
    __u64 aux_tail;
    __u64 aux_offset;
    __u64 aux_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct perf_event_mmap_page {
    __u32 version;
    __u32 compat_version;
    __u32 lock;
    __u32 index;
    __s64 offset;
    __u64 time_enabled;
    __u64 time_running;
    __u64 capabilities;
    __u64 cap_bit0;
    __u64 cap_bit0_is_deprecated;
    __u64 cap_user_rdpmc;
    __u64 cap_user_time;
    __u64 cap_user_time_zero;
    __u64 cap_____res;
    __u16 pmc_width;
    __u16 time_shift;
    __u32 time_mult;
    __u64 time_offset;
    __u64 time_zero;
    __u32 size;
    __u8 __reserved[948];
    __u64 data_head;
    __u64 data_tail;
    __u64 data_offset;
    __u64 data_size;
    __u64 aux_head;
    __u64 aux_tail;
    __u64 aux_offset;
    __u64 aux_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct perf_event_mmap_page {
    __u32 version;
    __u32 compat_version;
    __u32 lock;
    __u32 index;
    __s64 offset;
    __u64 time_enabled;
    __u64 time_running;
    __u64 capabilities;
    __u64 cap_bit0;
    __u64 cap_bit0_is_deprecated;
    __u64 cap_user_rdpmc;
    __u64 cap_user_time;
    __u64 cap_user_time_zero;
    __u64 cap_____res;
    __u16 pmc_width;
    __u16 time_shift;
    __u32 time_mult;
    __u64 time_offset;
    __u64 time_zero;
    __u32 size;
    __u8 __reserved[948];
    __u64 data_head;
    __u64 data_tail;
    __u64 data_offset;
    __u64 data_size;
    __u64 aux_head;
    __u64 aux_tail;
    __u64 aux_offset;
    __u64 aux_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct perf_event_mmap_page {
    __u32 version;
    __u32 compat_version;
    __u32 lock;
    __u32 index;
    __s64 offset;
    __u64 time_enabled;
    __u64 time_running;
    __u64 capabilities;
    __u64 cap_bit0;
    __u64 cap_bit0_is_deprecated;
    __u64 cap_user_rdpmc;
    __u64 cap_user_time;
    __u64 cap_user_time_zero;
    __u64 cap_____res;
    __u16 pmc_width;
    __u16 time_shift;
    __u32 time_mult;
    __u64 time_offset;
    __u64 time_zero;
    __u32 size;
    __u8 __reserved[948];
    __u64 data_head;
    __u64 data_tail;
    __u64 data_offset;
    __u64 data_size;
    __u64 aux_head;
    __u64 aux_tail;
    __u64 aux_offset;
    __u64 aux_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct perf_event_mmap_page {
    __u32 version;
    __u32 compat_version;
    __u32 lock;
    __u32 index;
    __s64 offset;
    __u64 time_enabled;
    __u64 time_running;
    __u64 capabilities;
    __u64 cap_bit0;
    __u64 cap_bit0_is_deprecated;
    __u64 cap_user_rdpmc;
    __u64 cap_user_time;
    __u64 cap_user_time_zero;
    __u64 cap_____res;
    __u16 pmc_width;
    __u16 time_shift;
    __u32 time_mult;
    __u64 time_offset;
    __u64 time_zero;
    __u32 size;
    __u8 __reserved[948];
    __u64 data_head;
    __u64 data_tail;
    __u64 data_offset;
    __u64 data_size;
    __u64 aux_head;
    __u64 aux_tail;
    __u64 aux_offset;
    __u64 aux_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct perf_event_mmap_page {
    __u32 version;
    __u32 compat_version;
    __u32 lock;
    __u32 index;
    __s64 offset;
    __u64 time_enabled;
    __u64 time_running;
    __u64 capabilities;
    __u64 cap_bit0;
    __u64 cap_bit0_is_deprecated;
    __u64 cap_user_rdpmc;
    __u64 cap_user_time;
    __u64 cap_user_time_zero;
    __u64 cap_____res;
    __u16 pmc_width;
    __u16 time_shift;
    __u32 time_mult;
    __u64 time_offset;
    __u64 time_zero;
    __u32 size;
    __u8 __reserved[948];
    __u64 data_head;
    __u64 data_tail;
    __u64 data_offset;
    __u64 data_size;
    __u64 aux_head;
    __u64 aux_tail;
    __u64 aux_offset;
    __u64 aux_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct perf_event_mmap_page {
    __u32 version;
    __u32 compat_version;
    __u32 lock;
    __u32 index;
    __s64 offset;
    __u64 time_enabled;
    __u64 time_running;
    __u64 capabilities;
    __u64 cap_bit0;
    __u64 cap_bit0_is_deprecated;
    __u64 cap_user_rdpmc;
    __u64 cap_user_time;
    __u64 cap_user_time_zero;
    __u64 cap_____res;
    __u16 pmc_width;
    __u16 time_shift;
    __u32 time_mult;
    __u64 time_offset;
    __u64 time_zero;
    __u32 size;
    __u8 __reserved[948];
    __u64 data_head;
    __u64 data_tail;
    __u64 data_offset;
    __u64 data_size;
    __u64 aux_head;
    __u64 aux_tail;
    __u64 aux_offset;
    __u64 aux_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct perf_event_mmap_page {
    __u32 version;
    __u32 compat_version;
    __u32 lock;
    __u32 index;
    __s64 offset;
    __u64 time_enabled;
    __u64 time_running;
    __u64 capabilities;
    __u64 cap_bit0;
    __u64 cap_bit0_is_deprecated;
    __u64 cap_user_rdpmc;
    __u64 cap_user_time;
    __u64 cap_user_time_zero;
    __u64 cap_user_time_short;
    __u64 cap_____res;
    __u16 pmc_width;
    __u16 time_shift;
    __u32 time_mult;
    __u64 time_offset;
    __u64 time_zero;
    __u32 size;
    __u32 __reserved_1;
    __u64 time_cycles;
    __u64 time_mask;
    __u8 __reserved[928];
    __u64 data_head;
    __u64 data_tail;
    __u64 data_offset;
    __u64 data_size;
    __u64 aux_head;
    __u64 aux_tail;
    __u64 aux_offset;
    __u64 aux_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct perf_event_mmap_page {
    __u32 version;
    __u32 compat_version;
    __u32 lock;
    __u32 index;
    __s64 offset;
    __u64 time_enabled;
    __u64 time_running;
    __u64 capabilities;
    __u64 cap_bit0;
    __u64 cap_bit0_is_deprecated;
    __u64 cap_user_rdpmc;
    __u64 cap_user_time;
    __u64 cap_user_time_zero;
    __u64 cap_user_time_short;
    __u64 cap_____res;
    __u16 pmc_width;
    __u16 time_shift;
    __u32 time_mult;
    __u64 time_offset;
    __u64 time_zero;
    __u32 size;
    __u32 __reserved_1;
    __u64 time_cycles;
    __u64 time_mask;
    __u8 __reserved[928];
    __u64 data_head;
    __u64 data_tail;
    __u64 data_offset;
    __u64 data_size;
    __u64 aux_head;
    __u64 aux_tail;
    __u64 aux_offset;
    __u64 aux_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct perf_event_mmap_page {
    __u32 version;
    __u32 compat_version;
    __u32 lock;
    __u32 index;
    __s64 offset;
    __u64 time_enabled;
    __u64 time_running;
    __u64 capabilities;
    __u64 cap_bit0;
    __u64 cap_bit0_is_deprecated;
    __u64 cap_user_rdpmc;
    __u64 cap_user_time;
    __u64 cap_user_time_zero;
    __u64 cap_user_time_short;
    __u64 cap_____res;
    __u16 pmc_width;
    __u16 time_shift;
    __u32 time_mult;
    __u64 time_offset;
    __u64 time_zero;
    __u32 size;
    __u32 __reserved_1;
    __u64 time_cycles;
    __u64 time_mask;
    __u8 __reserved[928];
    __u64 data_head;
    __u64 data_tail;
    __u64 data_offset;
    __u64 data_size;
    __u64 aux_head;
    __u64 aux_tail;
    __u64 aux_offset;
    __u64 aux_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct perf_event_mmap_page {
    __u32 version;
    __u32 compat_version;
    __u32 lock;
    __u32 index;
    __s64 offset;
    __u64 time_enabled;
    __u64 time_running;
    __u64 capabilities;
    __u64 cap_bit0;
    __u64 cap_bit0_is_deprecated;
    __u64 cap_user_rdpmc;
    __u64 cap_user_time;
    __u64 cap_user_time_zero;
    __u64 cap_user_time_short;
    __u64 cap_____res;
    __u16 pmc_width;
    __u16 time_shift;
    __u32 time_mult;
    __u64 time_offset;
    __u64 time_zero;
    __u32 size;
    __u32 __reserved_1;
    __u64 time_cycles;
    __u64 time_mask;
    __u8 __reserved[928];
    __u64 data_head;
    __u64 data_tail;
    __u64 data_offset;
    __u64 data_size;
    __u64 aux_head;
    __u64 aux_tail;
    __u64 aux_offset;
    __u64 aux_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct perf_event_mmap_page {
    __u32 version;
    __u32 compat_version;
    __u32 lock;
    __u32 index;
    __s64 offset;
    __u64 time_enabled;
    __u64 time_running;
    __u64 capabilities;
    __u64 cap_bit0;
    __u64 cap_bit0_is_deprecated;
    __u64 cap_user_rdpmc;
    __u64 cap_user_time;
    __u64 cap_user_time_zero;
    __u64 cap_user_time_short;
    __u64 cap_____res;
    __u16 pmc_width;
    __u16 time_shift;
    __u32 time_mult;
    __u64 time_offset;
    __u64 time_zero;
    __u32 size;
    __u32 __reserved_1;
    __u64 time_cycles;
    __u64 time_mask;
    __u8 __reserved[928];
    __u64 data_head;
    __u64 data_tail;
    __u64 data_offset;
    __u64 data_size;
    __u64 aux_head;
    __u64 aux_tail;
    __u64 aux_offset;
    __u64 aux_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct perf_event_mmap_page {
    __u32 version;
    __u32 compat_version;
    __u32 lock;
    __u32 index;
    __s64 offset;
    __u64 time_enabled;
    __u64 time_running;
    __u64 capabilities;
    __u64 cap_bit0;
    __u64 cap_bit0_is_deprecated;
    __u64 cap_user_rdpmc;
    __u64 cap_user_time;
    __u64 cap_user_time_zero;
    __u64 cap_user_time_short;
    __u64 cap_____res;
    __u16 pmc_width;
    __u16 time_shift;
    __u32 time_mult;
    __u64 time_offset;
    __u64 time_zero;
    __u32 size;
    __u32 __reserved_1;
    __u64 time_cycles;
    __u64 time_mask;
    __u8 __reserved[928];
    __u64 data_head;
    __u64 data_tail;
    __u64 data_offset;
    __u64 data_size;
    __u64 aux_head;
    __u64 aux_tail;
    __u64 aux_offset;
    __u64 aux_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct perf_event_mmap_page {
    __u32 version;
    __u32 compat_version;
    __u32 lock;
    __u32 index;
    __s64 offset;
    __u64 time_enabled;
    __u64 time_running;
    __u64 capabilities;
    __u64 cap_bit0;
    __u64 cap_bit0_is_deprecated;
    __u64 cap_user_rdpmc;
    __u64 cap_user_time;
    __u64 cap_user_time_zero;
    __u64 cap_user_time_short;
    __u64 cap_____res;
    __u16 pmc_width;
    __u16 time_shift;
    __u32 time_mult;
    __u64 time_offset;
    __u64 time_zero;
    __u32 size;
    __u32 __reserved_1;
    __u64 time_cycles;
    __u64 time_mask;
    __u8 __reserved[928];
    __u64 data_head;
    __u64 data_tail;
    __u64 data_offset;
    __u64 data_size;
    __u64 aux_head;
    __u64 aux_tail;
    __u64 aux_offset;
    __u64 aux_size;
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
struct perf_event_mmap_page {
    __u32 version;
    __u32 compat_version;
    __u32 lock;
    __u32 index;
    __s64 offset;
    __u64 time_enabled;
    __u64 time_running;
    __u64 capabilities;
    __u64 cap_bit0;
    __u64 cap_bit0_is_deprecated;
    __u64 cap_user_rdpmc;
    __u64 cap_user_time;
    __u64 cap_user_time_zero;
    __u64 cap_____res;
    __u16 pmc_width;
    __u16 time_shift;
    __u32 time_mult;
    __u64 time_offset;
    __u64 time_zero;
    __u32 size;
    __u8 __reserved[948];
    __u64 data_head;
    __u64 data_tail;
    __u64 data_offset;
    __u64 data_size;
    __u64 aux_head;
    __u64 aux_tail;
    __u64 aux_offset;
    __u64 aux_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct perf_event_mmap_page {
    __u32 version;
    __u32 compat_version;
    __u32 lock;
    __u32 index;
    __s64 offset;
    __u64 time_enabled;
    __u64 time_running;
    __u64 capabilities;
    __u64 cap_bit0;
    __u64 cap_bit0_is_deprecated;
    __u64 cap_user_rdpmc;
    __u64 cap_user_time;
    __u64 cap_user_time_zero;
    __u64 cap_____res;
    __u16 pmc_width;
    __u16 time_shift;
    __u32 time_mult;
    __u64 time_offset;
    __u64 time_zero;
    __u32 size;
    __u8 __reserved[948];
    __u64 data_head;
    __u64 data_tail;
    __u64 data_offset;
    __u64 data_size;
    __u64 aux_head;
    __u64 aux_tail;
    __u64 aux_offset;
    __u64 aux_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct perf_event_mmap_page {
    __u32 version;
    __u32 compat_version;
    __u32 lock;
    __u32 index;
    __s64 offset;
    __u64 time_enabled;
    __u64 time_running;
    __u64 capabilities;
    __u64 cap_bit0;
    __u64 cap_bit0_is_deprecated;
    __u64 cap_user_rdpmc;
    __u64 cap_user_time;
    __u64 cap_user_time_zero;
    __u64 cap_____res;
    __u16 pmc_width;
    __u16 time_shift;
    __u32 time_mult;
    __u64 time_offset;
    __u64 time_zero;
    __u32 size;
    __u8 __reserved[948];
    __u64 data_head;
    __u64 data_tail;
    __u64 data_offset;
    __u64 data_size;
    __u64 aux_head;
    __u64 aux_tail;
    __u64 aux_offset;
    __u64 aux_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct perf_event_mmap_page {
    __u32 version;
    __u32 compat_version;
    __u32 lock;
    __u32 index;
    __s64 offset;
    __u64 time_enabled;
    __u64 time_running;
    __u64 capabilities;
    __u64 cap_bit0;
    __u64 cap_bit0_is_deprecated;
    __u64 cap_user_rdpmc;
    __u64 cap_user_time;
    __u64 cap_user_time_zero;
    __u64 cap_____res;
    __u16 pmc_width;
    __u16 time_shift;
    __u32 time_mult;
    __u64 time_offset;
    __u64 time_zero;
    __u32 size;
    __u8 __reserved[948];
    __u64 data_head;
    __u64 data_tail;
    __u64 data_offset;
    __u64 data_size;
    __u64 aux_head;
    __u64 aux_tail;
    __u64 aux_offset;
    __u64 aux_size;
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
struct perf_event_mmap_page {
    __u32 version;
    __u32 compat_version;
    __u32 lock;
    __u32 index;
    __s64 offset;
    __u64 time_enabled;
    __u64 time_running;
    __u64 capabilities;
    __u64 cap_bit0;
    __u64 cap_bit0_is_deprecated;
    __u64 cap_user_rdpmc;
    __u64 cap_user_time;
    __u64 cap_user_time_zero;
    __u64 cap_____res;
    __u16 pmc_width;
    __u16 time_shift;
    __u32 time_mult;
    __u64 time_offset;
    __u64 time_zero;
    __u32 size;
    __u8 __reserved[948];
    __u64 data_head;
    __u64 data_tail;
    __u64 data_offset;
    __u64 data_size;
    __u64 aux_head;
    __u64 aux_tail;
    __u64 aux_offset;
    __u64 aux_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct perf_event_mmap_page {
    __u32 version;
    __u32 compat_version;
    __u32 lock;
    __u32 index;
    __s64 offset;
    __u64 time_enabled;
    __u64 time_running;
    __u64 capabilities;
    __u64 cap_bit0;
    __u64 cap_bit0_is_deprecated;
    __u64 cap_user_rdpmc;
    __u64 cap_user_time;
    __u64 cap_user_time_zero;
    __u64 cap_____res;
    __u16 pmc_width;
    __u16 time_shift;
    __u32 time_mult;
    __u64 time_offset;
    __u64 time_zero;
    __u32 size;
    __u8 __reserved[948];
    __u64 data_head;
    __u64 data_tail;
    __u64 data_offset;
    __u64 data_size;
    __u64 aux_head;
    __u64 aux_tail;
    __u64 aux_offset;
    __u64 aux_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct perf_event_mmap_page {
    __u32 version;
    __u32 compat_version;
    __u32 lock;
    __u32 index;
    __s64 offset;
    __u64 time_enabled;
    __u64 time_running;
    __u64 capabilities;
    __u64 cap_bit0;
    __u64 cap_bit0_is_deprecated;
    __u64 cap_user_rdpmc;
    __u64 cap_user_time;
    __u64 cap_user_time_zero;
    __u64 cap_____res;
    __u16 pmc_width;
    __u16 time_shift;
    __u32 time_mult;
    __u64 time_offset;
    __u64 time_zero;
    __u32 size;
    __u8 __reserved[948];
    __u64 data_head;
    __u64 data_tail;
    __u64 data_offset;
    __u64 data_size;
    __u64 aux_head;
    __u64 aux_tail;
    __u64 aux_offset;
    __u64 aux_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct perf_event_mmap_page {
    __u32 version;
    __u32 compat_version;
    __u32 lock;
    __u32 index;
    __s64 offset;
    __u64 time_enabled;
    __u64 time_running;
    __u64 capabilities;
    __u64 cap_bit0;
    __u64 cap_bit0_is_deprecated;
    __u64 cap_user_rdpmc;
    __u64 cap_user_time;
    __u64 cap_user_time_zero;
    __u64 cap_____res;
    __u16 pmc_width;
    __u16 time_shift;
    __u32 time_mult;
    __u64 time_offset;
    __u64 time_zero;
    __u32 size;
    __u8 __reserved[948];
    __u64 data_head;
    __u64 data_tail;
    __u64 data_offset;
    __u64 data_size;
    __u64 aux_head;
    __u64 aux_tail;
    __u64 aux_offset;
    __u64 aux_size;
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u64 cap_user_time_short</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 __reserved_1</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 time_cycles</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 time_mask</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u8 __reserved[948]</code> ➡️ <code>__u8 __reserved[928]</code>
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
