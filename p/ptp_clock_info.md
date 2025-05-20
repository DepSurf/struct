# Struct: <code>ptp_clock_info</code>

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
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ptp_clock_info {
    struct module *owner;
    char name[16];
    s32 max_adj;
    int n_alarm;
    int n_ext_ts;
    int n_per_out;
    int n_pins;
    int pps;
    struct ptp_pin_desc *pin_config;
    int (*adjfine)(struct ptp_clock_info *, long int);
    int (*adjfreq)(struct ptp_clock_info *, s32);
    int (*adjtime)(struct ptp_clock_info *, s64);
    int (*gettime64)(struct ptp_clock_info *, struct timespec64 *);
    int (*getcrosststamp)(struct ptp_clock_info *, struct system_device_crosststamp *);
    int (*settime64)(struct ptp_clock_info *, const struct timespec64 *);
    int (*enable)(struct ptp_clock_info *, struct ptp_clock_request *, int);
    int (*verify)(struct ptp_clock_info *, unsigned int, enum ptp_pin_function, unsigned int);
    long int (*do_aux_work)(struct ptp_clock_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ptp_clock_info {
    struct module *owner;
    char name[16];
    s32 max_adj;
    int n_alarm;
    int n_ext_ts;
    int n_per_out;
    int n_pins;
    int pps;
    struct ptp_pin_desc *pin_config;
    int (*adjfine)(struct ptp_clock_info *, long int);
    int (*adjfreq)(struct ptp_clock_info *, s32);
    int (*adjtime)(struct ptp_clock_info *, s64);
    int (*gettime64)(struct ptp_clock_info *, struct timespec64 *);
    int (*gettimex64)(struct ptp_clock_info *, struct timespec64 *, struct ptp_system_timestamp *);
    int (*getcrosststamp)(struct ptp_clock_info *, struct system_device_crosststamp *);
    int (*settime64)(struct ptp_clock_info *, const struct timespec64 *);
    int (*enable)(struct ptp_clock_info *, struct ptp_clock_request *, int);
    int (*verify)(struct ptp_clock_info *, unsigned int, enum ptp_pin_function, unsigned int);
    long int (*do_aux_work)(struct ptp_clock_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ptp_clock_info {
    struct module *owner;
    char name[16];
    s32 max_adj;
    int n_alarm;
    int n_ext_ts;
    int n_per_out;
    int n_pins;
    int pps;
    struct ptp_pin_desc *pin_config;
    int (*adjfine)(struct ptp_clock_info *, long int);
    int (*adjfreq)(struct ptp_clock_info *, s32);
    int (*adjtime)(struct ptp_clock_info *, s64);
    int (*gettime64)(struct ptp_clock_info *, struct timespec64 *);
    int (*gettimex64)(struct ptp_clock_info *, struct timespec64 *, struct ptp_system_timestamp *);
    int (*getcrosststamp)(struct ptp_clock_info *, struct system_device_crosststamp *);
    int (*settime64)(struct ptp_clock_info *, const struct timespec64 *);
    int (*enable)(struct ptp_clock_info *, struct ptp_clock_request *, int);
    int (*verify)(struct ptp_clock_info *, unsigned int, enum ptp_pin_function, unsigned int);
    long int (*do_aux_work)(struct ptp_clock_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ptp_clock_info {
    struct module *owner;
    char name[16];
    s32 max_adj;
    int n_alarm;
    int n_ext_ts;
    int n_per_out;
    int n_pins;
    int pps;
    struct ptp_pin_desc *pin_config;
    int (*adjfine)(struct ptp_clock_info *, long int);
    int (*adjfreq)(struct ptp_clock_info *, s32);
    int (*adjtime)(struct ptp_clock_info *, s64);
    int (*gettime64)(struct ptp_clock_info *, struct timespec64 *);
    int (*gettimex64)(struct ptp_clock_info *, struct timespec64 *, struct ptp_system_timestamp *);
    int (*getcrosststamp)(struct ptp_clock_info *, struct system_device_crosststamp *);
    int (*settime64)(struct ptp_clock_info *, const struct timespec64 *);
    int (*enable)(struct ptp_clock_info *, struct ptp_clock_request *, int);
    int (*verify)(struct ptp_clock_info *, unsigned int, enum ptp_pin_function, unsigned int);
    long int (*do_aux_work)(struct ptp_clock_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ptp_clock_info {
    struct module *owner;
    char name[16];
    s32 max_adj;
    int n_alarm;
    int n_ext_ts;
    int n_per_out;
    int n_pins;
    int pps;
    struct ptp_pin_desc *pin_config;
    int (*adjfine)(struct ptp_clock_info *, long int);
    int (*adjfreq)(struct ptp_clock_info *, s32);
    int (*adjphase)(struct ptp_clock_info *, s32);
    int (*adjtime)(struct ptp_clock_info *, s64);
    int (*gettime64)(struct ptp_clock_info *, struct timespec64 *);
    int (*gettimex64)(struct ptp_clock_info *, struct timespec64 *, struct ptp_system_timestamp *);
    int (*getcrosststamp)(struct ptp_clock_info *, struct system_device_crosststamp *);
    int (*settime64)(struct ptp_clock_info *, const struct timespec64 *);
    int (*enable)(struct ptp_clock_info *, struct ptp_clock_request *, int);
    int (*verify)(struct ptp_clock_info *, unsigned int, enum ptp_pin_function, unsigned int);
    long int (*do_aux_work)(struct ptp_clock_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ptp_clock_info {
    struct module *owner;
    char name[16];
    s32 max_adj;
    int n_alarm;
    int n_ext_ts;
    int n_per_out;
    int n_pins;
    int pps;
    struct ptp_pin_desc *pin_config;
    int (*adjfine)(struct ptp_clock_info *, long int);
    int (*adjfreq)(struct ptp_clock_info *, s32);
    int (*adjphase)(struct ptp_clock_info *, s32);
    int (*adjtime)(struct ptp_clock_info *, s64);
    int (*gettime64)(struct ptp_clock_info *, struct timespec64 *);
    int (*gettimex64)(struct ptp_clock_info *, struct timespec64 *, struct ptp_system_timestamp *);
    int (*getcrosststamp)(struct ptp_clock_info *, struct system_device_crosststamp *);
    int (*settime64)(struct ptp_clock_info *, const struct timespec64 *);
    int (*enable)(struct ptp_clock_info *, struct ptp_clock_request *, int);
    int (*verify)(struct ptp_clock_info *, unsigned int, enum ptp_pin_function, unsigned int);
    long int (*do_aux_work)(struct ptp_clock_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ptp_clock_info {
    struct module *owner;
    char name[16];
    s32 max_adj;
    int n_alarm;
    int n_ext_ts;
    int n_per_out;
    int n_pins;
    int pps;
    struct ptp_pin_desc *pin_config;
    int (*adjfine)(struct ptp_clock_info *, long int);
    int (*adjfreq)(struct ptp_clock_info *, s32);
    int (*adjphase)(struct ptp_clock_info *, s32);
    int (*adjtime)(struct ptp_clock_info *, s64);
    int (*gettime64)(struct ptp_clock_info *, struct timespec64 *);
    int (*gettimex64)(struct ptp_clock_info *, struct timespec64 *, struct ptp_system_timestamp *);
    int (*getcrosststamp)(struct ptp_clock_info *, struct system_device_crosststamp *);
    int (*settime64)(struct ptp_clock_info *, const struct timespec64 *);
    int (*enable)(struct ptp_clock_info *, struct ptp_clock_request *, int);
    int (*verify)(struct ptp_clock_info *, unsigned int, enum ptp_pin_function, unsigned int);
    long int (*do_aux_work)(struct ptp_clock_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ptp_clock_info {
    struct module *owner;
    char name[32];
    s32 max_adj;
    int n_alarm;
    int n_ext_ts;
    int n_per_out;
    int n_pins;
    int pps;
    struct ptp_pin_desc *pin_config;
    int (*adjfine)(struct ptp_clock_info *, long int);
    int (*adjfreq)(struct ptp_clock_info *, s32);
    int (*adjphase)(struct ptp_clock_info *, s32);
    int (*adjtime)(struct ptp_clock_info *, s64);
    int (*gettime64)(struct ptp_clock_info *, struct timespec64 *);
    int (*gettimex64)(struct ptp_clock_info *, struct timespec64 *, struct ptp_system_timestamp *);
    int (*getcrosststamp)(struct ptp_clock_info *, struct system_device_crosststamp *);
    int (*settime64)(struct ptp_clock_info *, const struct timespec64 *);
    int (*enable)(struct ptp_clock_info *, struct ptp_clock_request *, int);
    int (*verify)(struct ptp_clock_info *, unsigned int, enum ptp_pin_function, unsigned int);
    long int (*do_aux_work)(struct ptp_clock_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ptp_clock_info {
    struct module *owner;
    char name[32];
    s32 max_adj;
    int n_alarm;
    int n_ext_ts;
    int n_per_out;
    int n_pins;
    int pps;
    struct ptp_pin_desc *pin_config;
    int (*adjfine)(struct ptp_clock_info *, long int);
    int (*adjfreq)(struct ptp_clock_info *, s32);
    int (*adjphase)(struct ptp_clock_info *, s32);
    int (*adjtime)(struct ptp_clock_info *, s64);
    int (*gettime64)(struct ptp_clock_info *, struct timespec64 *);
    int (*gettimex64)(struct ptp_clock_info *, struct timespec64 *, struct ptp_system_timestamp *);
    int (*getcrosststamp)(struct ptp_clock_info *, struct system_device_crosststamp *);
    int (*settime64)(struct ptp_clock_info *, const struct timespec64 *);
    int (*getcycles64)(struct ptp_clock_info *, struct timespec64 *);
    int (*getcyclesx64)(struct ptp_clock_info *, struct timespec64 *, struct ptp_system_timestamp *);
    int (*getcrosscycles)(struct ptp_clock_info *, struct system_device_crosststamp *);
    int (*enable)(struct ptp_clock_info *, struct ptp_clock_request *, int);
    int (*verify)(struct ptp_clock_info *, unsigned int, enum ptp_pin_function, unsigned int);
    long int (*do_aux_work)(struct ptp_clock_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ptp_clock_info {
    struct module *owner;
    char name[32];
    s32 max_adj;
    int n_alarm;
    int n_ext_ts;
    int n_per_out;
    int n_pins;
    int pps;
    struct ptp_pin_desc *pin_config;
    int (*adjfine)(struct ptp_clock_info *, long int);
    int (*adjphase)(struct ptp_clock_info *, s32);
    int (*adjtime)(struct ptp_clock_info *, s64);
    int (*gettime64)(struct ptp_clock_info *, struct timespec64 *);
    int (*gettimex64)(struct ptp_clock_info *, struct timespec64 *, struct ptp_system_timestamp *);
    int (*getcrosststamp)(struct ptp_clock_info *, struct system_device_crosststamp *);
    int (*settime64)(struct ptp_clock_info *, const struct timespec64 *);
    int (*getcycles64)(struct ptp_clock_info *, struct timespec64 *);
    int (*getcyclesx64)(struct ptp_clock_info *, struct timespec64 *, struct ptp_system_timestamp *);
    int (*getcrosscycles)(struct ptp_clock_info *, struct system_device_crosststamp *);
    int (*enable)(struct ptp_clock_info *, struct ptp_clock_request *, int);
    int (*verify)(struct ptp_clock_info *, unsigned int, enum ptp_pin_function, unsigned int);
    long int (*do_aux_work)(struct ptp_clock_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ptp_clock_info {
    struct module *owner;
    char name[32];
    s32 max_adj;
    int n_alarm;
    int n_ext_ts;
    int n_per_out;
    int n_pins;
    int pps;
    struct ptp_pin_desc *pin_config;
    int (*adjfine)(struct ptp_clock_info *, long int);
    int (*adjphase)(struct ptp_clock_info *, s32);
    s32 (*getmaxphase)(struct ptp_clock_info *);
    int (*adjtime)(struct ptp_clock_info *, s64);
    int (*gettime64)(struct ptp_clock_info *, struct timespec64 *);
    int (*gettimex64)(struct ptp_clock_info *, struct timespec64 *, struct ptp_system_timestamp *);
    int (*getcrosststamp)(struct ptp_clock_info *, struct system_device_crosststamp *);
    int (*settime64)(struct ptp_clock_info *, const struct timespec64 *);
    int (*getcycles64)(struct ptp_clock_info *, struct timespec64 *);
    int (*getcyclesx64)(struct ptp_clock_info *, struct timespec64 *, struct ptp_system_timestamp *);
    int (*getcrosscycles)(struct ptp_clock_info *, struct system_device_crosststamp *);
    int (*enable)(struct ptp_clock_info *, struct ptp_clock_request *, int);
    int (*verify)(struct ptp_clock_info *, unsigned int, enum ptp_pin_function, unsigned int);
    long int (*do_aux_work)(struct ptp_clock_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ptp_clock_info {
    struct module *owner;
    char name[32];
    s32 max_adj;
    int n_alarm;
    int n_ext_ts;
    int n_per_out;
    int n_pins;
    int pps;
    struct ptp_pin_desc *pin_config;
    int (*adjfine)(struct ptp_clock_info *, long int);
    int (*adjphase)(struct ptp_clock_info *, s32);
    s32 (*getmaxphase)(struct ptp_clock_info *);
    int (*adjtime)(struct ptp_clock_info *, s64);
    int (*gettime64)(struct ptp_clock_info *, struct timespec64 *);
    int (*gettimex64)(struct ptp_clock_info *, struct timespec64 *, struct ptp_system_timestamp *);
    int (*getcrosststamp)(struct ptp_clock_info *, struct system_device_crosststamp *);
    int (*settime64)(struct ptp_clock_info *, const struct timespec64 *);
    int (*getcycles64)(struct ptp_clock_info *, struct timespec64 *);
    int (*getcyclesx64)(struct ptp_clock_info *, struct timespec64 *, struct ptp_system_timestamp *);
    int (*getcrosscycles)(struct ptp_clock_info *, struct system_device_crosststamp *);
    int (*enable)(struct ptp_clock_info *, struct ptp_clock_request *, int);
    int (*verify)(struct ptp_clock_info *, unsigned int, enum ptp_pin_function, unsigned int);
    long int (*do_aux_work)(struct ptp_clock_info *);
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
struct ptp_clock_info {
    struct module *owner;
    char name[16];
    s32 max_adj;
    int n_alarm;
    int n_ext_ts;
    int n_per_out;
    int n_pins;
    int pps;
    struct ptp_pin_desc *pin_config;
    int (*adjfine)(struct ptp_clock_info *, long int);
    int (*adjfreq)(struct ptp_clock_info *, s32);
    int (*adjtime)(struct ptp_clock_info *, s64);
    int (*gettime64)(struct ptp_clock_info *, struct timespec64 *);
    int (*gettimex64)(struct ptp_clock_info *, struct timespec64 *, struct ptp_system_timestamp *);
    int (*getcrosststamp)(struct ptp_clock_info *, struct system_device_crosststamp *);
    int (*settime64)(struct ptp_clock_info *, const struct timespec64 *);
    int (*enable)(struct ptp_clock_info *, struct ptp_clock_request *, int);
    int (*verify)(struct ptp_clock_info *, unsigned int, enum ptp_pin_function, unsigned int);
    long int (*do_aux_work)(struct ptp_clock_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ptp_clock_info {
    struct module *owner;
    char name[16];
    s32 max_adj;
    int n_alarm;
    int n_ext_ts;
    int n_per_out;
    int n_pins;
    int pps;
    struct ptp_pin_desc *pin_config;
    int (*adjfine)(struct ptp_clock_info *, long int);
    int (*adjfreq)(struct ptp_clock_info *, s32);
    int (*adjtime)(struct ptp_clock_info *, s64);
    int (*gettime64)(struct ptp_clock_info *, struct timespec64 *);
    int (*gettimex64)(struct ptp_clock_info *, struct timespec64 *, struct ptp_system_timestamp *);
    int (*getcrosststamp)(struct ptp_clock_info *, struct system_device_crosststamp *);
    int (*settime64)(struct ptp_clock_info *, const struct timespec64 *);
    int (*enable)(struct ptp_clock_info *, struct ptp_clock_request *, int);
    int (*verify)(struct ptp_clock_info *, unsigned int, enum ptp_pin_function, unsigned int);
    long int (*do_aux_work)(struct ptp_clock_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ptp_clock_info {
    struct module *owner;
    char name[16];
    s32 max_adj;
    int n_alarm;
    int n_ext_ts;
    int n_per_out;
    int n_pins;
    int pps;
    struct ptp_pin_desc *pin_config;
    int (*adjfine)(struct ptp_clock_info *, long int);
    int (*adjfreq)(struct ptp_clock_info *, s32);
    int (*adjtime)(struct ptp_clock_info *, s64);
    int (*gettime64)(struct ptp_clock_info *, struct timespec64 *);
    int (*gettimex64)(struct ptp_clock_info *, struct timespec64 *, struct ptp_system_timestamp *);
    int (*getcrosststamp)(struct ptp_clock_info *, struct system_device_crosststamp *);
    int (*settime64)(struct ptp_clock_info *, const struct timespec64 *);
    int (*enable)(struct ptp_clock_info *, struct ptp_clock_request *, int);
    int (*verify)(struct ptp_clock_info *, unsigned int, enum ptp_pin_function, unsigned int);
    long int (*do_aux_work)(struct ptp_clock_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ptp_clock_info {
    struct module *owner;
    char name[16];
    s32 max_adj;
    int n_alarm;
    int n_ext_ts;
    int n_per_out;
    int n_pins;
    int pps;
    struct ptp_pin_desc *pin_config;
    int (*adjfine)(struct ptp_clock_info *, long int);
    int (*adjfreq)(struct ptp_clock_info *, s32);
    int (*adjtime)(struct ptp_clock_info *, s64);
    int (*gettime64)(struct ptp_clock_info *, struct timespec64 *);
    int (*gettimex64)(struct ptp_clock_info *, struct timespec64 *, struct ptp_system_timestamp *);
    int (*getcrosststamp)(struct ptp_clock_info *, struct system_device_crosststamp *);
    int (*settime64)(struct ptp_clock_info *, const struct timespec64 *);
    int (*enable)(struct ptp_clock_info *, struct ptp_clock_request *, int);
    int (*verify)(struct ptp_clock_info *, unsigned int, enum ptp_pin_function, unsigned int);
    long int (*do_aux_work)(struct ptp_clock_info *);
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
struct ptp_clock_info {
    struct module *owner;
    char name[16];
    s32 max_adj;
    int n_alarm;
    int n_ext_ts;
    int n_per_out;
    int n_pins;
    int pps;
    struct ptp_pin_desc *pin_config;
    int (*adjfine)(struct ptp_clock_info *, long int);
    int (*adjfreq)(struct ptp_clock_info *, s32);
    int (*adjtime)(struct ptp_clock_info *, s64);
    int (*gettime64)(struct ptp_clock_info *, struct timespec64 *);
    int (*gettimex64)(struct ptp_clock_info *, struct timespec64 *, struct ptp_system_timestamp *);
    int (*getcrosststamp)(struct ptp_clock_info *, struct system_device_crosststamp *);
    int (*settime64)(struct ptp_clock_info *, const struct timespec64 *);
    int (*enable)(struct ptp_clock_info *, struct ptp_clock_request *, int);
    int (*verify)(struct ptp_clock_info *, unsigned int, enum ptp_pin_function, unsigned int);
    long int (*do_aux_work)(struct ptp_clock_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ptp_clock_info {
    struct module *owner;
    char name[16];
    s32 max_adj;
    int n_alarm;
    int n_ext_ts;
    int n_per_out;
    int n_pins;
    int pps;
    struct ptp_pin_desc *pin_config;
    int (*adjfine)(struct ptp_clock_info *, long int);
    int (*adjfreq)(struct ptp_clock_info *, s32);
    int (*adjtime)(struct ptp_clock_info *, s64);
    int (*gettime64)(struct ptp_clock_info *, struct timespec64 *);
    int (*gettimex64)(struct ptp_clock_info *, struct timespec64 *, struct ptp_system_timestamp *);
    int (*getcrosststamp)(struct ptp_clock_info *, struct system_device_crosststamp *);
    int (*settime64)(struct ptp_clock_info *, const struct timespec64 *);
    int (*enable)(struct ptp_clock_info *, struct ptp_clock_request *, int);
    int (*verify)(struct ptp_clock_info *, unsigned int, enum ptp_pin_function, unsigned int);
    long int (*do_aux_work)(struct ptp_clock_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ptp_clock_info {
    struct module *owner;
    char name[16];
    s32 max_adj;
    int n_alarm;
    int n_ext_ts;
    int n_per_out;
    int n_pins;
    int pps;
    struct ptp_pin_desc *pin_config;
    int (*adjfine)(struct ptp_clock_info *, long int);
    int (*adjfreq)(struct ptp_clock_info *, s32);
    int (*adjtime)(struct ptp_clock_info *, s64);
    int (*gettime64)(struct ptp_clock_info *, struct timespec64 *);
    int (*gettimex64)(struct ptp_clock_info *, struct timespec64 *, struct ptp_system_timestamp *);
    int (*getcrosststamp)(struct ptp_clock_info *, struct system_device_crosststamp *);
    int (*settime64)(struct ptp_clock_info *, const struct timespec64 *);
    int (*enable)(struct ptp_clock_info *, struct ptp_clock_request *, int);
    int (*verify)(struct ptp_clock_info *, unsigned int, enum ptp_pin_function, unsigned int);
    long int (*do_aux_work)(struct ptp_clock_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ptp_clock_info {
    struct module *owner;
    char name[16];
    s32 max_adj;
    int n_alarm;
    int n_ext_ts;
    int n_per_out;
    int n_pins;
    int pps;
    struct ptp_pin_desc *pin_config;
    int (*adjfine)(struct ptp_clock_info *, long int);
    int (*adjfreq)(struct ptp_clock_info *, s32);
    int (*adjtime)(struct ptp_clock_info *, s64);
    int (*gettime64)(struct ptp_clock_info *, struct timespec64 *);
    int (*gettimex64)(struct ptp_clock_info *, struct timespec64 *, struct ptp_system_timestamp *);
    int (*getcrosststamp)(struct ptp_clock_info *, struct system_device_crosststamp *);
    int (*settime64)(struct ptp_clock_info *, const struct timespec64 *);
    int (*enable)(struct ptp_clock_info *, struct ptp_clock_request *, int);
    int (*verify)(struct ptp_clock_info *, unsigned int, enum ptp_pin_function, unsigned int);
    long int (*do_aux_work)(struct ptp_clock_info *);
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
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*gettimex64)(struct ptp_clock_info *, struct timespec64 *, struct ptp_system_timestamp *)</code>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*adjphase)(struct ptp_clock_info *, s32)</code>
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
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>char name[16]</code> ➡️ <code>char name[32]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*getcycles64)(struct ptp_clock_info *, struct timespec64 *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*getcyclesx64)(struct ptp_clock_info *, struct timespec64 *, struct ptp_system_timestamp *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*getcrosscycles)(struct ptp_clock_info *, struct system_device_crosststamp *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*adjfreq)(struct ptp_clock_info *, s32)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>s32 (*getmaxphase)(struct ptp_clock_info *)</code>
</li>
</ul>
</details>
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
