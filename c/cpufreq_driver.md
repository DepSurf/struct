# Struct: <code>cpufreq_driver</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct cpufreq_driver {
    char name[16];
    u8 flags;
    void *driver_data;
    int (*init)(struct cpufreq_policy *);
    int (*verify)(struct cpufreq_policy *);
    int (*setpolicy)(struct cpufreq_policy *);
    int (*target)(struct cpufreq_policy *, unsigned int, unsigned int);
    int (*target_index)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get_intermediate)(struct cpufreq_policy *, unsigned int);
    int (*target_intermediate)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get)(unsigned int);
    int (*bios_limit)(int, unsigned int *);
    int (*exit)(struct cpufreq_policy *);
    void (*stop_cpu)(struct cpufreq_policy *);
    int (*suspend)(struct cpufreq_policy *);
    int (*resume)(struct cpufreq_policy *);
    void (*ready)(struct cpufreq_policy *);
    struct freq_attr **attr;
    bool boost_supported;
    bool boost_enabled;
    int (*set_boost)(int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct cpufreq_driver {
    char name[16];
    u8 flags;
    void *driver_data;
    int (*init)(struct cpufreq_policy *);
    int (*verify)(struct cpufreq_policy *);
    int (*setpolicy)(struct cpufreq_policy *);
    int (*target)(struct cpufreq_policy *, unsigned int, unsigned int);
    int (*target_index)(struct cpufreq_policy *, unsigned int);
    unsigned int (*fast_switch)(struct cpufreq_policy *, unsigned int);
    unsigned int (*resolve_freq)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get_intermediate)(struct cpufreq_policy *, unsigned int);
    int (*target_intermediate)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get)(unsigned int);
    int (*bios_limit)(int, unsigned int *);
    int (*exit)(struct cpufreq_policy *);
    void (*stop_cpu)(struct cpufreq_policy *);
    int (*suspend)(struct cpufreq_policy *);
    int (*resume)(struct cpufreq_policy *);
    void (*ready)(struct cpufreq_policy *);
    struct freq_attr **attr;
    bool boost_enabled;
    int (*set_boost)(int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct cpufreq_driver {
    char name[16];
    u8 flags;
    void *driver_data;
    int (*init)(struct cpufreq_policy *);
    int (*verify)(struct cpufreq_policy *);
    int (*setpolicy)(struct cpufreq_policy *);
    int (*target)(struct cpufreq_policy *, unsigned int, unsigned int);
    int (*target_index)(struct cpufreq_policy *, unsigned int);
    unsigned int (*fast_switch)(struct cpufreq_policy *, unsigned int);
    unsigned int (*resolve_freq)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get_intermediate)(struct cpufreq_policy *, unsigned int);
    int (*target_intermediate)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get)(unsigned int);
    int (*bios_limit)(int, unsigned int *);
    int (*exit)(struct cpufreq_policy *);
    void (*stop_cpu)(struct cpufreq_policy *);
    int (*suspend)(struct cpufreq_policy *);
    int (*resume)(struct cpufreq_policy *);
    void (*ready)(struct cpufreq_policy *);
    struct freq_attr **attr;
    bool boost_enabled;
    int (*set_boost)(int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct cpufreq_driver {
    char name[16];
    u8 flags;
    void *driver_data;
    int (*init)(struct cpufreq_policy *);
    int (*verify)(struct cpufreq_policy *);
    int (*setpolicy)(struct cpufreq_policy *);
    int (*target)(struct cpufreq_policy *, unsigned int, unsigned int);
    int (*target_index)(struct cpufreq_policy *, unsigned int);
    unsigned int (*fast_switch)(struct cpufreq_policy *, unsigned int);
    unsigned int (*resolve_freq)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get_intermediate)(struct cpufreq_policy *, unsigned int);
    int (*target_intermediate)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get)(unsigned int);
    int (*bios_limit)(int, unsigned int *);
    int (*exit)(struct cpufreq_policy *);
    void (*stop_cpu)(struct cpufreq_policy *);
    int (*suspend)(struct cpufreq_policy *);
    int (*resume)(struct cpufreq_policy *);
    void (*ready)(struct cpufreq_policy *);
    struct freq_attr **attr;
    bool boost_enabled;
    int (*set_boost)(int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct cpufreq_driver {
    char name[16];
    u8 flags;
    void *driver_data;
    int (*init)(struct cpufreq_policy *);
    int (*verify)(struct cpufreq_policy *);
    int (*setpolicy)(struct cpufreq_policy *);
    int (*target)(struct cpufreq_policy *, unsigned int, unsigned int);
    int (*target_index)(struct cpufreq_policy *, unsigned int);
    unsigned int (*fast_switch)(struct cpufreq_policy *, unsigned int);
    unsigned int (*resolve_freq)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get_intermediate)(struct cpufreq_policy *, unsigned int);
    int (*target_intermediate)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get)(unsigned int);
    int (*bios_limit)(int, unsigned int *);
    int (*exit)(struct cpufreq_policy *);
    void (*stop_cpu)(struct cpufreq_policy *);
    int (*suspend)(struct cpufreq_policy *);
    int (*resume)(struct cpufreq_policy *);
    void (*ready)(struct cpufreq_policy *);
    struct freq_attr **attr;
    bool boost_enabled;
    int (*set_boost)(int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct cpufreq_driver {
    char name[16];
    u8 flags;
    void *driver_data;
    int (*init)(struct cpufreq_policy *);
    int (*verify)(struct cpufreq_policy *);
    int (*setpolicy)(struct cpufreq_policy *);
    int (*target)(struct cpufreq_policy *, unsigned int, unsigned int);
    int (*target_index)(struct cpufreq_policy *, unsigned int);
    unsigned int (*fast_switch)(struct cpufreq_policy *, unsigned int);
    unsigned int (*resolve_freq)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get_intermediate)(struct cpufreq_policy *, unsigned int);
    int (*target_intermediate)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get)(unsigned int);
    int (*bios_limit)(int, unsigned int *);
    int (*exit)(struct cpufreq_policy *);
    void (*stop_cpu)(struct cpufreq_policy *);
    int (*suspend)(struct cpufreq_policy *);
    int (*resume)(struct cpufreq_policy *);
    void (*ready)(struct cpufreq_policy *);
    struct freq_attr **attr;
    bool boost_enabled;
    int (*set_boost)(int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct cpufreq_driver {
    char name[16];
    u8 flags;
    void *driver_data;
    int (*init)(struct cpufreq_policy *);
    int (*verify)(struct cpufreq_policy *);
    int (*setpolicy)(struct cpufreq_policy *);
    int (*target)(struct cpufreq_policy *, unsigned int, unsigned int);
    int (*target_index)(struct cpufreq_policy *, unsigned int);
    unsigned int (*fast_switch)(struct cpufreq_policy *, unsigned int);
    unsigned int (*resolve_freq)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get_intermediate)(struct cpufreq_policy *, unsigned int);
    int (*target_intermediate)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get)(unsigned int);
    int (*bios_limit)(int, unsigned int *);
    int (*exit)(struct cpufreq_policy *);
    void (*stop_cpu)(struct cpufreq_policy *);
    int (*suspend)(struct cpufreq_policy *);
    int (*resume)(struct cpufreq_policy *);
    void (*ready)(struct cpufreq_policy *);
    struct freq_attr **attr;
    bool boost_enabled;
    int (*set_boost)(int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct cpufreq_driver {
    char name[16];
    u8 flags;
    void *driver_data;
    int (*init)(struct cpufreq_policy *);
    int (*verify)(struct cpufreq_policy *);
    int (*setpolicy)(struct cpufreq_policy *);
    int (*target)(struct cpufreq_policy *, unsigned int, unsigned int);
    int (*target_index)(struct cpufreq_policy *, unsigned int);
    unsigned int (*fast_switch)(struct cpufreq_policy *, unsigned int);
    unsigned int (*resolve_freq)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get_intermediate)(struct cpufreq_policy *, unsigned int);
    int (*target_intermediate)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get)(unsigned int);
    void (*update_limits)(unsigned int);
    int (*bios_limit)(int, unsigned int *);
    int (*online)(struct cpufreq_policy *);
    int (*offline)(struct cpufreq_policy *);
    int (*exit)(struct cpufreq_policy *);
    void (*stop_cpu)(struct cpufreq_policy *);
    int (*suspend)(struct cpufreq_policy *);
    int (*resume)(struct cpufreq_policy *);
    void (*ready)(struct cpufreq_policy *);
    struct freq_attr **attr;
    bool boost_enabled;
    int (*set_boost)(int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct cpufreq_driver {
    char name[16];
    u8 flags;
    void *driver_data;
    int (*init)(struct cpufreq_policy *);
    int (*verify)(struct cpufreq_policy_data *);
    int (*setpolicy)(struct cpufreq_policy *);
    int (*target)(struct cpufreq_policy *, unsigned int, unsigned int);
    int (*target_index)(struct cpufreq_policy *, unsigned int);
    unsigned int (*fast_switch)(struct cpufreq_policy *, unsigned int);
    unsigned int (*resolve_freq)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get_intermediate)(struct cpufreq_policy *, unsigned int);
    int (*target_intermediate)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get)(unsigned int);
    void (*update_limits)(unsigned int);
    int (*bios_limit)(int, unsigned int *);
    int (*online)(struct cpufreq_policy *);
    int (*offline)(struct cpufreq_policy *);
    int (*exit)(struct cpufreq_policy *);
    void (*stop_cpu)(struct cpufreq_policy *);
    int (*suspend)(struct cpufreq_policy *);
    int (*resume)(struct cpufreq_policy *);
    void (*ready)(struct cpufreq_policy *);
    struct freq_attr **attr;
    bool boost_enabled;
    int (*set_boost)(int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct cpufreq_driver {
    char name[16];
    u8 flags;
    void *driver_data;
    int (*init)(struct cpufreq_policy *);
    int (*verify)(struct cpufreq_policy_data *);
    int (*setpolicy)(struct cpufreq_policy *);
    int (*target)(struct cpufreq_policy *, unsigned int, unsigned int);
    int (*target_index)(struct cpufreq_policy *, unsigned int);
    unsigned int (*fast_switch)(struct cpufreq_policy *, unsigned int);
    unsigned int (*resolve_freq)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get_intermediate)(struct cpufreq_policy *, unsigned int);
    int (*target_intermediate)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get)(unsigned int);
    void (*update_limits)(unsigned int);
    int (*bios_limit)(int, unsigned int *);
    int (*online)(struct cpufreq_policy *);
    int (*offline)(struct cpufreq_policy *);
    int (*exit)(struct cpufreq_policy *);
    void (*stop_cpu)(struct cpufreq_policy *);
    int (*suspend)(struct cpufreq_policy *);
    int (*resume)(struct cpufreq_policy *);
    void (*ready)(struct cpufreq_policy *);
    struct freq_attr **attr;
    bool boost_enabled;
    int (*set_boost)(struct cpufreq_policy *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct cpufreq_driver {
    char name[16];
    u16 flags;
    void *driver_data;
    int (*init)(struct cpufreq_policy *);
    int (*verify)(struct cpufreq_policy_data *);
    int (*setpolicy)(struct cpufreq_policy *);
    int (*target)(struct cpufreq_policy *, unsigned int, unsigned int);
    int (*target_index)(struct cpufreq_policy *, unsigned int);
    unsigned int (*fast_switch)(struct cpufreq_policy *, unsigned int);
    void (*adjust_perf)(unsigned int, long unsigned int, long unsigned int, long unsigned int);
    unsigned int (*resolve_freq)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get_intermediate)(struct cpufreq_policy *, unsigned int);
    int (*target_intermediate)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get)(unsigned int);
    void (*update_limits)(unsigned int);
    int (*bios_limit)(int, unsigned int *);
    int (*online)(struct cpufreq_policy *);
    int (*offline)(struct cpufreq_policy *);
    int (*exit)(struct cpufreq_policy *);
    void (*stop_cpu)(struct cpufreq_policy *);
    int (*suspend)(struct cpufreq_policy *);
    int (*resume)(struct cpufreq_policy *);
    void (*ready)(struct cpufreq_policy *);
    struct freq_attr **attr;
    bool boost_enabled;
    int (*set_boost)(struct cpufreq_policy *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct cpufreq_driver {
    char name[16];
    u16 flags;
    void *driver_data;
    int (*init)(struct cpufreq_policy *);
    int (*verify)(struct cpufreq_policy_data *);
    int (*setpolicy)(struct cpufreq_policy *);
    int (*target)(struct cpufreq_policy *, unsigned int, unsigned int);
    int (*target_index)(struct cpufreq_policy *, unsigned int);
    unsigned int (*fast_switch)(struct cpufreq_policy *, unsigned int);
    void (*adjust_perf)(unsigned int, long unsigned int, long unsigned int, long unsigned int);
    unsigned int (*resolve_freq)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get_intermediate)(struct cpufreq_policy *, unsigned int);
    int (*target_intermediate)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get)(unsigned int);
    void (*update_limits)(unsigned int);
    int (*bios_limit)(int, unsigned int *);
    int (*online)(struct cpufreq_policy *);
    int (*offline)(struct cpufreq_policy *);
    int (*exit)(struct cpufreq_policy *);
    void (*stop_cpu)(struct cpufreq_policy *);
    int (*suspend)(struct cpufreq_policy *);
    int (*resume)(struct cpufreq_policy *);
    void (*ready)(struct cpufreq_policy *);
    struct freq_attr **attr;
    bool boost_enabled;
    int (*set_boost)(struct cpufreq_policy *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct cpufreq_driver {
    char name[16];
    u16 flags;
    void *driver_data;
    int (*init)(struct cpufreq_policy *);
    int (*verify)(struct cpufreq_policy_data *);
    int (*setpolicy)(struct cpufreq_policy *);
    int (*target)(struct cpufreq_policy *, unsigned int, unsigned int);
    int (*target_index)(struct cpufreq_policy *, unsigned int);
    unsigned int (*fast_switch)(struct cpufreq_policy *, unsigned int);
    void (*adjust_perf)(unsigned int, long unsigned int, long unsigned int, long unsigned int);
    unsigned int (*get_intermediate)(struct cpufreq_policy *, unsigned int);
    int (*target_intermediate)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get)(unsigned int);
    void (*update_limits)(unsigned int);
    int (*bios_limit)(int, unsigned int *);
    int (*online)(struct cpufreq_policy *);
    int (*offline)(struct cpufreq_policy *);
    int (*exit)(struct cpufreq_policy *);
    int (*suspend)(struct cpufreq_policy *);
    int (*resume)(struct cpufreq_policy *);
    struct freq_attr **attr;
    bool boost_enabled;
    int (*set_boost)(struct cpufreq_policy *, int);
    void (*register_em)(struct cpufreq_policy *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct cpufreq_driver {
    char name[16];
    u16 flags;
    void *driver_data;
    int (*init)(struct cpufreq_policy *);
    int (*verify)(struct cpufreq_policy_data *);
    int (*setpolicy)(struct cpufreq_policy *);
    int (*target)(struct cpufreq_policy *, unsigned int, unsigned int);
    int (*target_index)(struct cpufreq_policy *, unsigned int);
    unsigned int (*fast_switch)(struct cpufreq_policy *, unsigned int);
    void (*adjust_perf)(unsigned int, long unsigned int, long unsigned int, long unsigned int);
    unsigned int (*get_intermediate)(struct cpufreq_policy *, unsigned int);
    int (*target_intermediate)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get)(unsigned int);
    void (*update_limits)(unsigned int);
    int (*bios_limit)(int, unsigned int *);
    int (*online)(struct cpufreq_policy *);
    int (*offline)(struct cpufreq_policy *);
    int (*exit)(struct cpufreq_policy *);
    int (*suspend)(struct cpufreq_policy *);
    int (*resume)(struct cpufreq_policy *);
    void (*ready)(struct cpufreq_policy *);
    struct freq_attr **attr;
    bool boost_enabled;
    int (*set_boost)(struct cpufreq_policy *, int);
    void (*register_em)(struct cpufreq_policy *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct cpufreq_driver {
    char name[16];
    u16 flags;
    void *driver_data;
    int (*init)(struct cpufreq_policy *);
    int (*verify)(struct cpufreq_policy_data *);
    int (*setpolicy)(struct cpufreq_policy *);
    int (*target)(struct cpufreq_policy *, unsigned int, unsigned int);
    int (*target_index)(struct cpufreq_policy *, unsigned int);
    unsigned int (*fast_switch)(struct cpufreq_policy *, unsigned int);
    void (*adjust_perf)(unsigned int, long unsigned int, long unsigned int, long unsigned int);
    unsigned int (*get_intermediate)(struct cpufreq_policy *, unsigned int);
    int (*target_intermediate)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get)(unsigned int);
    void (*update_limits)(unsigned int);
    int (*bios_limit)(int, unsigned int *);
    int (*online)(struct cpufreq_policy *);
    int (*offline)(struct cpufreq_policy *);
    int (*exit)(struct cpufreq_policy *);
    int (*suspend)(struct cpufreq_policy *);
    int (*resume)(struct cpufreq_policy *);
    void (*ready)(struct cpufreq_policy *);
    struct freq_attr **attr;
    bool boost_enabled;
    int (*set_boost)(struct cpufreq_policy *, int);
    void (*register_em)(struct cpufreq_policy *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct cpufreq_driver {
    char name[16];
    u16 flags;
    void *driver_data;
    int (*init)(struct cpufreq_policy *);
    int (*verify)(struct cpufreq_policy_data *);
    int (*setpolicy)(struct cpufreq_policy *);
    int (*target)(struct cpufreq_policy *, unsigned int, unsigned int);
    int (*target_index)(struct cpufreq_policy *, unsigned int);
    unsigned int (*fast_switch)(struct cpufreq_policy *, unsigned int);
    void (*adjust_perf)(unsigned int, long unsigned int, long unsigned int, long unsigned int);
    unsigned int (*get_intermediate)(struct cpufreq_policy *, unsigned int);
    int (*target_intermediate)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get)(unsigned int);
    void (*update_limits)(unsigned int);
    int (*bios_limit)(int, unsigned int *);
    int (*online)(struct cpufreq_policy *);
    int (*offline)(struct cpufreq_policy *);
    int (*exit)(struct cpufreq_policy *);
    int (*suspend)(struct cpufreq_policy *);
    int (*resume)(struct cpufreq_policy *);
    void (*ready)(struct cpufreq_policy *);
    struct freq_attr **attr;
    bool boost_enabled;
    int (*set_boost)(struct cpufreq_policy *, int);
    void (*register_em)(struct cpufreq_policy *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct cpufreq_driver {
    char name[16];
    u16 flags;
    void *driver_data;
    int (*init)(struct cpufreq_policy *);
    int (*verify)(struct cpufreq_policy_data *);
    int (*setpolicy)(struct cpufreq_policy *);
    int (*target)(struct cpufreq_policy *, unsigned int, unsigned int);
    int (*target_index)(struct cpufreq_policy *, unsigned int);
    unsigned int (*fast_switch)(struct cpufreq_policy *, unsigned int);
    void (*adjust_perf)(unsigned int, long unsigned int, long unsigned int, long unsigned int);
    unsigned int (*get_intermediate)(struct cpufreq_policy *, unsigned int);
    int (*target_intermediate)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get)(unsigned int);
    void (*update_limits)(unsigned int);
    int (*bios_limit)(int, unsigned int *);
    int (*online)(struct cpufreq_policy *);
    int (*offline)(struct cpufreq_policy *);
    int (*exit)(struct cpufreq_policy *);
    int (*suspend)(struct cpufreq_policy *);
    int (*resume)(struct cpufreq_policy *);
    void (*ready)(struct cpufreq_policy *);
    struct freq_attr **attr;
    bool boost_enabled;
    int (*set_boost)(struct cpufreq_policy *, int);
    void (*register_em)(struct cpufreq_policy *);
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
struct cpufreq_driver {
    char name[16];
    u8 flags;
    void *driver_data;
    int (*init)(struct cpufreq_policy *);
    int (*verify)(struct cpufreq_policy_data *);
    int (*setpolicy)(struct cpufreq_policy *);
    int (*target)(struct cpufreq_policy *, unsigned int, unsigned int);
    int (*target_index)(struct cpufreq_policy *, unsigned int);
    unsigned int (*fast_switch)(struct cpufreq_policy *, unsigned int);
    unsigned int (*resolve_freq)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get_intermediate)(struct cpufreq_policy *, unsigned int);
    int (*target_intermediate)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get)(unsigned int);
    void (*update_limits)(unsigned int);
    int (*bios_limit)(int, unsigned int *);
    int (*online)(struct cpufreq_policy *);
    int (*offline)(struct cpufreq_policy *);
    int (*exit)(struct cpufreq_policy *);
    void (*stop_cpu)(struct cpufreq_policy *);
    int (*suspend)(struct cpufreq_policy *);
    int (*resume)(struct cpufreq_policy *);
    void (*ready)(struct cpufreq_policy *);
    struct freq_attr **attr;
    bool boost_enabled;
    int (*set_boost)(int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct cpufreq_driver {
    char name[16];
    u8 flags;
    void *driver_data;
    int (*init)(struct cpufreq_policy *);
    int (*verify)(struct cpufreq_policy_data *);
    int (*setpolicy)(struct cpufreq_policy *);
    int (*target)(struct cpufreq_policy *, unsigned int, unsigned int);
    int (*target_index)(struct cpufreq_policy *, unsigned int);
    unsigned int (*fast_switch)(struct cpufreq_policy *, unsigned int);
    unsigned int (*resolve_freq)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get_intermediate)(struct cpufreq_policy *, unsigned int);
    int (*target_intermediate)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get)(unsigned int);
    void (*update_limits)(unsigned int);
    int (*bios_limit)(int, unsigned int *);
    int (*online)(struct cpufreq_policy *);
    int (*offline)(struct cpufreq_policy *);
    int (*exit)(struct cpufreq_policy *);
    void (*stop_cpu)(struct cpufreq_policy *);
    int (*suspend)(struct cpufreq_policy *);
    int (*resume)(struct cpufreq_policy *);
    void (*ready)(struct cpufreq_policy *);
    struct freq_attr **attr;
    bool boost_enabled;
    int (*set_boost)(int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct cpufreq_driver {
    char name[16];
    u8 flags;
    void *driver_data;
    int (*init)(struct cpufreq_policy *);
    int (*verify)(struct cpufreq_policy_data *);
    int (*setpolicy)(struct cpufreq_policy *);
    int (*target)(struct cpufreq_policy *, unsigned int, unsigned int);
    int (*target_index)(struct cpufreq_policy *, unsigned int);
    unsigned int (*fast_switch)(struct cpufreq_policy *, unsigned int);
    unsigned int (*resolve_freq)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get_intermediate)(struct cpufreq_policy *, unsigned int);
    int (*target_intermediate)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get)(unsigned int);
    void (*update_limits)(unsigned int);
    int (*bios_limit)(int, unsigned int *);
    int (*online)(struct cpufreq_policy *);
    int (*offline)(struct cpufreq_policy *);
    int (*exit)(struct cpufreq_policy *);
    void (*stop_cpu)(struct cpufreq_policy *);
    int (*suspend)(struct cpufreq_policy *);
    int (*resume)(struct cpufreq_policy *);
    void (*ready)(struct cpufreq_policy *);
    struct freq_attr **attr;
    bool boost_enabled;
    int (*set_boost)(int);
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
struct cpufreq_driver {
    char name[16];
    u8 flags;
    void *driver_data;
    int (*init)(struct cpufreq_policy *);
    int (*verify)(struct cpufreq_policy_data *);
    int (*setpolicy)(struct cpufreq_policy *);
    int (*target)(struct cpufreq_policy *, unsigned int, unsigned int);
    int (*target_index)(struct cpufreq_policy *, unsigned int);
    unsigned int (*fast_switch)(struct cpufreq_policy *, unsigned int);
    unsigned int (*resolve_freq)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get_intermediate)(struct cpufreq_policy *, unsigned int);
    int (*target_intermediate)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get)(unsigned int);
    void (*update_limits)(unsigned int);
    int (*bios_limit)(int, unsigned int *);
    int (*online)(struct cpufreq_policy *);
    int (*offline)(struct cpufreq_policy *);
    int (*exit)(struct cpufreq_policy *);
    void (*stop_cpu)(struct cpufreq_policy *);
    int (*suspend)(struct cpufreq_policy *);
    int (*resume)(struct cpufreq_policy *);
    void (*ready)(struct cpufreq_policy *);
    struct freq_attr **attr;
    bool boost_enabled;
    int (*set_boost)(int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct cpufreq_driver {
    char name[16];
    u8 flags;
    void *driver_data;
    int (*init)(struct cpufreq_policy *);
    int (*verify)(struct cpufreq_policy_data *);
    int (*setpolicy)(struct cpufreq_policy *);
    int (*target)(struct cpufreq_policy *, unsigned int, unsigned int);
    int (*target_index)(struct cpufreq_policy *, unsigned int);
    unsigned int (*fast_switch)(struct cpufreq_policy *, unsigned int);
    unsigned int (*resolve_freq)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get_intermediate)(struct cpufreq_policy *, unsigned int);
    int (*target_intermediate)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get)(unsigned int);
    void (*update_limits)(unsigned int);
    int (*bios_limit)(int, unsigned int *);
    int (*online)(struct cpufreq_policy *);
    int (*offline)(struct cpufreq_policy *);
    int (*exit)(struct cpufreq_policy *);
    void (*stop_cpu)(struct cpufreq_policy *);
    int (*suspend)(struct cpufreq_policy *);
    int (*resume)(struct cpufreq_policy *);
    void (*ready)(struct cpufreq_policy *);
    struct freq_attr **attr;
    bool boost_enabled;
    int (*set_boost)(int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct cpufreq_driver {
    char name[16];
    u8 flags;
    void *driver_data;
    int (*init)(struct cpufreq_policy *);
    int (*verify)(struct cpufreq_policy_data *);
    int (*setpolicy)(struct cpufreq_policy *);
    int (*target)(struct cpufreq_policy *, unsigned int, unsigned int);
    int (*target_index)(struct cpufreq_policy *, unsigned int);
    unsigned int (*fast_switch)(struct cpufreq_policy *, unsigned int);
    unsigned int (*resolve_freq)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get_intermediate)(struct cpufreq_policy *, unsigned int);
    int (*target_intermediate)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get)(unsigned int);
    void (*update_limits)(unsigned int);
    int (*bios_limit)(int, unsigned int *);
    int (*online)(struct cpufreq_policy *);
    int (*offline)(struct cpufreq_policy *);
    int (*exit)(struct cpufreq_policy *);
    void (*stop_cpu)(struct cpufreq_policy *);
    int (*suspend)(struct cpufreq_policy *);
    int (*resume)(struct cpufreq_policy *);
    void (*ready)(struct cpufreq_policy *);
    struct freq_attr **attr;
    bool boost_enabled;
    int (*set_boost)(int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cpufreq_driver {
    char name[16];
    u8 flags;
    void *driver_data;
    int (*init)(struct cpufreq_policy *);
    int (*verify)(struct cpufreq_policy_data *);
    int (*setpolicy)(struct cpufreq_policy *);
    int (*target)(struct cpufreq_policy *, unsigned int, unsigned int);
    int (*target_index)(struct cpufreq_policy *, unsigned int);
    unsigned int (*fast_switch)(struct cpufreq_policy *, unsigned int);
    unsigned int (*resolve_freq)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get_intermediate)(struct cpufreq_policy *, unsigned int);
    int (*target_intermediate)(struct cpufreq_policy *, unsigned int);
    unsigned int (*get)(unsigned int);
    void (*update_limits)(unsigned int);
    int (*bios_limit)(int, unsigned int *);
    int (*online)(struct cpufreq_policy *);
    int (*offline)(struct cpufreq_policy *);
    int (*exit)(struct cpufreq_policy *);
    void (*stop_cpu)(struct cpufreq_policy *);
    int (*suspend)(struct cpufreq_policy *);
    int (*resume)(struct cpufreq_policy *);
    void (*ready)(struct cpufreq_policy *);
    struct freq_attr **attr;
    bool boost_enabled;
    int (*set_boost)(int);
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
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int (*fast_switch)(struct cpufreq_policy *, unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int (*resolve_freq)(struct cpufreq_policy *, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>bool boost_supported</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*update_limits)(unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*online)(struct cpufreq_policy *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*offline)(struct cpufreq_policy *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*verify)(struct cpufreq_policy *)</code> ➡️ <code>int (*verify)(struct cpufreq_policy_data *)</code>
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
<code>int (*set_boost)(int)</code> ➡️ <code>int (*set_boost)(struct cpufreq_policy *, int)</code>
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
<code>void (*adjust_perf)(unsigned int, long unsigned int, long unsigned int, long unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 flags</code> ➡️ <code>u16 flags</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*register_em)(struct cpufreq_policy *)</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int (*resolve_freq)(struct cpufreq_policy *, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*stop_cpu)(struct cpufreq_policy *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*ready)(struct cpufreq_policy *)</code>
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
<code>void (*ready)(struct cpufreq_policy *)</code>
</li>
</ul>
</details>
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
