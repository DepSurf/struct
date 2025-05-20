# Struct: <code>cpuidle_device</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct cpuidle_device {
    unsigned int registered;
    unsigned int enabled;
    unsigned int cpu;
    int last_residency;
    struct cpuidle_state_usage states_usage[10];
    struct cpuidle_state_kobj * kobjs[10];
    struct cpuidle_driver_kobj *kobj_driver;
    struct cpuidle_device_kobj *kobj_dev;
    struct list_head device_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct cpuidle_device {
    unsigned int registered;
    unsigned int enabled;
    unsigned int cpu;
    int last_residency;
    struct cpuidle_state_usage states_usage[10];
    struct cpuidle_state_kobj * kobjs[10];
    struct cpuidle_driver_kobj *kobj_driver;
    struct cpuidle_device_kobj *kobj_dev;
    struct list_head device_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct cpuidle_device {
    unsigned int registered;
    unsigned int enabled;
    unsigned int use_deepest_state;
    unsigned int cpu;
    int last_residency;
    struct cpuidle_state_usage states_usage[10];
    struct cpuidle_state_kobj * kobjs[10];
    struct cpuidle_driver_kobj *kobj_driver;
    struct cpuidle_device_kobj *kobj_dev;
    struct list_head device_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct cpuidle_device {
    unsigned int registered;
    unsigned int enabled;
    unsigned int use_deepest_state;
    unsigned int cpu;
    int last_residency;
    struct cpuidle_state_usage states_usage[10];
    struct cpuidle_state_kobj * kobjs[10];
    struct cpuidle_driver_kobj *kobj_driver;
    struct cpuidle_device_kobj *kobj_dev;
    struct list_head device_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct cpuidle_device {
    unsigned int registered;
    unsigned int enabled;
    unsigned int use_deepest_state;
    unsigned int cpu;
    int last_residency;
    struct cpuidle_state_usage states_usage[10];
    struct cpuidle_state_kobj * kobjs[10];
    struct cpuidle_driver_kobj *kobj_driver;
    struct cpuidle_device_kobj *kobj_dev;
    struct list_head device_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct cpuidle_device {
    unsigned int registered;
    unsigned int enabled;
    unsigned int use_deepest_state;
    unsigned int cpu;
    int last_residency;
    struct cpuidle_state_usage states_usage[10];
    struct cpuidle_state_kobj * kobjs[10];
    struct cpuidle_driver_kobj *kobj_driver;
    struct cpuidle_device_kobj *kobj_dev;
    struct list_head device_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct cpuidle_device {
    unsigned int registered;
    unsigned int enabled;
    unsigned int use_deepest_state;
    unsigned int poll_time_limit;
    unsigned int cpu;
    int last_residency;
    struct cpuidle_state_usage states_usage[10];
    struct cpuidle_state_kobj * kobjs[10];
    struct cpuidle_driver_kobj *kobj_driver;
    struct cpuidle_device_kobj *kobj_dev;
    struct list_head device_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct cpuidle_device {
    unsigned int registered;
    unsigned int enabled;
    unsigned int use_deepest_state;
    unsigned int poll_time_limit;
    unsigned int cpu;
    ktime_t next_hrtimer;
    int last_residency;
    struct cpuidle_state_usage states_usage[10];
    struct cpuidle_state_kobj * kobjs[10];
    struct cpuidle_driver_kobj *kobj_driver;
    struct cpuidle_device_kobj *kobj_dev;
    struct list_head device_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct cpuidle_device {
    unsigned int registered;
    unsigned int enabled;
    unsigned int use_deepest_state;
    unsigned int poll_time_limit;
    unsigned int cpu;
    ktime_t next_hrtimer;
    int last_state_idx;
    int last_residency;
    u64 poll_limit_ns;
    struct cpuidle_state_usage states_usage[10];
    struct cpuidle_state_kobj * kobjs[10];
    struct cpuidle_driver_kobj *kobj_driver;
    struct cpuidle_device_kobj *kobj_dev;
    struct list_head device_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct cpuidle_device {
    unsigned int registered;
    unsigned int enabled;
    unsigned int poll_time_limit;
    unsigned int cpu;
    ktime_t next_hrtimer;
    int last_state_idx;
    u64 last_residency_ns;
    u64 poll_limit_ns;
    u64 forced_idle_latency_limit_ns;
    struct cpuidle_state_usage states_usage[10];
    struct cpuidle_state_kobj * kobjs[10];
    struct cpuidle_driver_kobj *kobj_driver;
    struct cpuidle_device_kobj *kobj_dev;
    struct list_head device_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct cpuidle_device {
    unsigned int registered;
    unsigned int enabled;
    unsigned int poll_time_limit;
    unsigned int cpu;
    ktime_t next_hrtimer;
    int last_state_idx;
    u64 last_residency_ns;
    u64 poll_limit_ns;
    u64 forced_idle_latency_limit_ns;
    struct cpuidle_state_usage states_usage[10];
    struct cpuidle_state_kobj * kobjs[10];
    struct cpuidle_driver_kobj *kobj_driver;
    struct cpuidle_device_kobj *kobj_dev;
    struct list_head device_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct cpuidle_device {
    unsigned int registered;
    unsigned int enabled;
    unsigned int poll_time_limit;
    unsigned int cpu;
    ktime_t next_hrtimer;
    int last_state_idx;
    u64 last_residency_ns;
    u64 poll_limit_ns;
    u64 forced_idle_latency_limit_ns;
    struct cpuidle_state_usage states_usage[10];
    struct cpuidle_state_kobj * kobjs[10];
    struct cpuidle_driver_kobj *kobj_driver;
    struct cpuidle_device_kobj *kobj_dev;
    struct list_head device_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct cpuidle_device {
    unsigned int registered;
    unsigned int enabled;
    unsigned int poll_time_limit;
    unsigned int cpu;
    ktime_t next_hrtimer;
    int last_state_idx;
    u64 last_residency_ns;
    u64 poll_limit_ns;
    u64 forced_idle_latency_limit_ns;
    struct cpuidle_state_usage states_usage[10];
    struct cpuidle_state_kobj * kobjs[10];
    struct cpuidle_driver_kobj *kobj_driver;
    struct cpuidle_device_kobj *kobj_dev;
    struct list_head device_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct cpuidle_device {
    unsigned int registered;
    unsigned int enabled;
    unsigned int poll_time_limit;
    unsigned int cpu;
    ktime_t next_hrtimer;
    int last_state_idx;
    u64 last_residency_ns;
    u64 poll_limit_ns;
    u64 forced_idle_latency_limit_ns;
    struct cpuidle_state_usage states_usage[10];
    struct cpuidle_state_kobj * kobjs[10];
    struct cpuidle_driver_kobj *kobj_driver;
    struct cpuidle_device_kobj *kobj_dev;
    struct list_head device_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct cpuidle_device {
    unsigned int registered;
    unsigned int enabled;
    unsigned int poll_time_limit;
    unsigned int cpu;
    ktime_t next_hrtimer;
    int last_state_idx;
    u64 last_residency_ns;
    u64 poll_limit_ns;
    u64 forced_idle_latency_limit_ns;
    struct cpuidle_state_usage states_usage[10];
    struct cpuidle_state_kobj * kobjs[10];
    struct cpuidle_driver_kobj *kobj_driver;
    struct cpuidle_device_kobj *kobj_dev;
    struct list_head device_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct cpuidle_device {
    unsigned int registered;
    unsigned int enabled;
    unsigned int poll_time_limit;
    unsigned int cpu;
    ktime_t next_hrtimer;
    int last_state_idx;
    u64 last_residency_ns;
    u64 poll_limit_ns;
    u64 forced_idle_latency_limit_ns;
    struct cpuidle_state_usage states_usage[10];
    struct cpuidle_state_kobj * kobjs[10];
    struct cpuidle_driver_kobj *kobj_driver;
    struct cpuidle_device_kobj *kobj_dev;
    struct list_head device_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct cpuidle_device {
    unsigned int registered;
    unsigned int enabled;
    unsigned int poll_time_limit;
    unsigned int cpu;
    ktime_t next_hrtimer;
    int last_state_idx;
    u64 last_residency_ns;
    u64 poll_limit_ns;
    u64 forced_idle_latency_limit_ns;
    struct cpuidle_state_usage states_usage[10];
    struct cpuidle_state_kobj * kobjs[10];
    struct cpuidle_driver_kobj *kobj_driver;
    struct cpuidle_device_kobj *kobj_dev;
    struct list_head device_list;
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
struct cpuidle_device {
    unsigned int registered;
    unsigned int enabled;
    unsigned int use_deepest_state;
    unsigned int poll_time_limit;
    unsigned int cpu;
    ktime_t next_hrtimer;
    int last_state_idx;
    int last_residency;
    u64 poll_limit_ns;
    struct cpuidle_state_usage states_usage[10];
    struct cpuidle_state_kobj * kobjs[10];
    struct cpuidle_driver_kobj *kobj_driver;
    struct cpuidle_device_kobj *kobj_dev;
    struct list_head device_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct cpuidle_device {
    unsigned int registered;
    unsigned int enabled;
    unsigned int use_deepest_state;
    unsigned int poll_time_limit;
    unsigned int cpu;
    ktime_t next_hrtimer;
    int last_state_idx;
    int last_residency;
    u64 poll_limit_ns;
    struct cpuidle_state_usage states_usage[10];
    struct cpuidle_state_kobj * kobjs[10];
    struct cpuidle_driver_kobj *kobj_driver;
    struct cpuidle_device_kobj *kobj_dev;
    struct list_head device_list;
    cpumask_t coupled_cpus;
    struct cpuidle_coupled *coupled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct cpuidle_device {
    unsigned int registered;
    unsigned int enabled;
    unsigned int use_deepest_state;
    unsigned int poll_time_limit;
    unsigned int cpu;
    ktime_t next_hrtimer;
    int last_state_idx;
    int last_residency;
    u64 poll_limit_ns;
    struct cpuidle_state_usage states_usage[10];
    struct cpuidle_state_kobj * kobjs[10];
    struct cpuidle_driver_kobj *kobj_driver;
    struct cpuidle_device_kobj *kobj_dev;
    struct list_head device_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct cpuidle_device {
    unsigned int registered;
    unsigned int enabled;
    unsigned int use_deepest_state;
    unsigned int poll_time_limit;
    unsigned int cpu;
    ktime_t next_hrtimer;
    int last_state_idx;
    int last_residency;
    u64 poll_limit_ns;
    struct cpuidle_state_usage states_usage[10];
    struct cpuidle_state_kobj * kobjs[10];
    struct cpuidle_driver_kobj *kobj_driver;
    struct cpuidle_device_kobj *kobj_dev;
    struct list_head device_list;
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
struct cpuidle_device {
    unsigned int registered;
    unsigned int enabled;
    unsigned int use_deepest_state;
    unsigned int poll_time_limit;
    unsigned int cpu;
    ktime_t next_hrtimer;
    int last_state_idx;
    int last_residency;
    u64 poll_limit_ns;
    struct cpuidle_state_usage states_usage[10];
    struct cpuidle_state_kobj * kobjs[10];
    struct cpuidle_driver_kobj *kobj_driver;
    struct cpuidle_device_kobj *kobj_dev;
    struct list_head device_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct cpuidle_device {
    unsigned int registered;
    unsigned int enabled;
    unsigned int use_deepest_state;
    unsigned int poll_time_limit;
    unsigned int cpu;
    ktime_t next_hrtimer;
    int last_state_idx;
    int last_residency;
    u64 poll_limit_ns;
    struct cpuidle_state_usage states_usage[10];
    struct cpuidle_state_kobj * kobjs[10];
    struct cpuidle_driver_kobj *kobj_driver;
    struct cpuidle_device_kobj *kobj_dev;
    struct list_head device_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct cpuidle_device {
    unsigned int registered;
    unsigned int enabled;
    unsigned int use_deepest_state;
    unsigned int poll_time_limit;
    unsigned int cpu;
    ktime_t next_hrtimer;
    int last_state_idx;
    int last_residency;
    u64 poll_limit_ns;
    struct cpuidle_state_usage states_usage[10];
    struct cpuidle_state_kobj * kobjs[10];
    struct cpuidle_driver_kobj *kobj_driver;
    struct cpuidle_device_kobj *kobj_dev;
    struct list_head device_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cpuidle_device {
    unsigned int registered;
    unsigned int enabled;
    unsigned int use_deepest_state;
    unsigned int poll_time_limit;
    unsigned int cpu;
    ktime_t next_hrtimer;
    int last_state_idx;
    int last_residency;
    u64 poll_limit_ns;
    struct cpuidle_state_usage states_usage[10];
    struct cpuidle_state_kobj * kobjs[10];
    struct cpuidle_driver_kobj *kobj_driver;
    struct cpuidle_device_kobj *kobj_dev;
    struct list_head device_list;
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
<b>Field added. </b>
<code>unsigned int use_deepest_state</code>
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
<code>unsigned int poll_time_limit</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>ktime_t next_hrtimer</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int last_state_idx</code>
</li>
<li>
<b>Field added. </b>
<code>u64 poll_limit_ns</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 last_residency_ns</code>
</li>
<li>
<b>Field added. </b>
<code>u64 forced_idle_latency_limit_ns</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int use_deepest_state</code>
</li>
<li>
<b>Field removed. </b>
<code>int last_residency</code>
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
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>arm64</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct cpuidle_driver_kobj *kobj_driver</code> ➡️ <code>struct cpuidle_driver_kobj *kobj_driver</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>cpumask_t coupled_cpus</code>
</li>
<li>
<b>Field added. </b>
<code>struct cpuidle_coupled *coupled</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct cpuidle_driver_kobj *kobj_driver</code> ➡️ <code>struct cpuidle_driver_kobj *kobj_driver</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct cpuidle_state_kobj * kobjs[10]</code> ➡️ <code>struct cpuidle_state_kobj * kobjs[10]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct cpuidle_device_kobj *kobj_dev</code> ➡️ <code>struct cpuidle_device_kobj *kobj_dev</code>
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
