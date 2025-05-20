# Struct: <code>sugov_cpu</code>

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
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct sugov_cpu {
    struct update_util_data update_util;
    struct sugov_policy *sg_policy;
    unsigned int cached_raw_freq;
    long unsigned int iowait_boost;
    long unsigned int iowait_boost_max;
    u64 last_update;
    long unsigned int util;
    long unsigned int max;
    unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct sugov_cpu {
    struct update_util_data update_util;
    struct sugov_policy *sg_policy;
    long unsigned int iowait_boost;
    long unsigned int iowait_boost_max;
    u64 last_update;
    long unsigned int util;
    long unsigned int max;
    unsigned int flags;
    long unsigned int saved_idle_calls;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct sugov_cpu {
    struct update_util_data update_util;
    struct sugov_policy *sg_policy;
    unsigned int cpu;
    bool iowait_boost_pending;
    unsigned int iowait_boost;
    unsigned int iowait_boost_max;
    u64 last_update;
    long unsigned int util;
    long unsigned int max;
    unsigned int flags;
    long unsigned int saved_idle_calls;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct sugov_cpu {
    struct update_util_data update_util;
    struct sugov_policy *sg_policy;
    unsigned int cpu;
    bool iowait_boost_pending;
    unsigned int iowait_boost;
    unsigned int iowait_boost_max;
    u64 last_update;
    long unsigned int util_cfs;
    long unsigned int util_dl;
    long unsigned int max;
    long unsigned int saved_idle_calls;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct sugov_cpu {
    struct update_util_data update_util;
    struct sugov_policy *sg_policy;
    unsigned int cpu;
    bool iowait_boost_pending;
    unsigned int iowait_boost;
    unsigned int iowait_boost_max;
    u64 last_update;
    long unsigned int bw_dl;
    long unsigned int max;
    long unsigned int saved_idle_calls;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct sugov_cpu {
    struct update_util_data update_util;
    struct sugov_policy *sg_policy;
    unsigned int cpu;
    bool iowait_boost_pending;
    unsigned int iowait_boost;
    u64 last_update;
    long unsigned int bw_dl;
    long unsigned int max;
    long unsigned int saved_idle_calls;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct sugov_cpu {
    struct update_util_data update_util;
    struct sugov_policy *sg_policy;
    unsigned int cpu;
    bool iowait_boost_pending;
    unsigned int iowait_boost;
    u64 last_update;
    long unsigned int bw_dl;
    long unsigned int max;
    long unsigned int saved_idle_calls;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct sugov_cpu {
    struct update_util_data update_util;
    struct sugov_policy *sg_policy;
    unsigned int cpu;
    bool iowait_boost_pending;
    unsigned int iowait_boost;
    u64 last_update;
    long unsigned int bw_dl;
    long unsigned int max;
    long unsigned int saved_idle_calls;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct sugov_cpu {
    struct update_util_data update_util;
    struct sugov_policy *sg_policy;
    unsigned int cpu;
    bool iowait_boost_pending;
    unsigned int iowait_boost;
    u64 last_update;
    long unsigned int util;
    long unsigned int bw_dl;
    long unsigned int max;
    long unsigned int saved_idle_calls;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct sugov_cpu {
    struct update_util_data update_util;
    struct sugov_policy *sg_policy;
    unsigned int cpu;
    bool iowait_boost_pending;
    unsigned int iowait_boost;
    u64 last_update;
    long unsigned int util;
    long unsigned int bw_dl;
    long unsigned int max;
    long unsigned int saved_idle_calls;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct sugov_cpu {
    struct update_util_data update_util;
    struct sugov_policy *sg_policy;
    unsigned int cpu;
    bool iowait_boost_pending;
    unsigned int iowait_boost;
    u64 last_update;
    long unsigned int util;
    long unsigned int bw_dl;
    long unsigned int max;
    long unsigned int saved_idle_calls;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct sugov_cpu {
    struct update_util_data update_util;
    struct sugov_policy *sg_policy;
    unsigned int cpu;
    bool iowait_boost_pending;
    unsigned int iowait_boost;
    u64 last_update;
    long unsigned int util;
    long unsigned int bw_dl;
    long unsigned int max;
    long unsigned int saved_idle_calls;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct sugov_cpu {
    struct update_util_data update_util;
    struct sugov_policy *sg_policy;
    unsigned int cpu;
    bool iowait_boost_pending;
    unsigned int iowait_boost;
    u64 last_update;
    long unsigned int util;
    long unsigned int bw_dl;
    long unsigned int max;
    long unsigned int saved_idle_calls;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct sugov_cpu {
    struct update_util_data update_util;
    struct sugov_policy *sg_policy;
    unsigned int cpu;
    bool iowait_boost_pending;
    unsigned int iowait_boost;
    u64 last_update;
    long unsigned int util;
    long unsigned int bw_dl;
    long unsigned int saved_idle_calls;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct sugov_cpu {
    struct update_util_data update_util;
    struct sugov_policy *sg_policy;
    unsigned int cpu;
    bool iowait_boost_pending;
    unsigned int iowait_boost;
    u64 last_update;
    long unsigned int util;
    long unsigned int bw_min;
    long unsigned int saved_idle_calls;
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
struct sugov_cpu {
    struct update_util_data update_util;
    struct sugov_policy *sg_policy;
    unsigned int cpu;
    bool iowait_boost_pending;
    unsigned int iowait_boost;
    u64 last_update;
    long unsigned int bw_dl;
    long unsigned int max;
    long unsigned int saved_idle_calls;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct sugov_cpu {
    struct update_util_data update_util;
    struct sugov_policy *sg_policy;
    unsigned int cpu;
    bool iowait_boost_pending;
    unsigned int iowait_boost;
    u64 last_update;
    long unsigned int bw_dl;
    long unsigned int max;
    long unsigned int saved_idle_calls;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct sugov_cpu {
    struct update_util_data update_util;
    struct sugov_policy *sg_policy;
    unsigned int cpu;
    bool iowait_boost_pending;
    unsigned int iowait_boost;
    u64 last_update;
    long unsigned int bw_dl;
    long unsigned int max;
    long unsigned int saved_idle_calls;
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
struct sugov_cpu {
    struct update_util_data update_util;
    struct sugov_policy *sg_policy;
    unsigned int cpu;
    bool iowait_boost_pending;
    unsigned int iowait_boost;
    u64 last_update;
    long unsigned int bw_dl;
    long unsigned int max;
    long unsigned int saved_idle_calls;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct sugov_cpu {
    struct update_util_data update_util;
    struct sugov_policy *sg_policy;
    unsigned int cpu;
    bool iowait_boost_pending;
    unsigned int iowait_boost;
    u64 last_update;
    long unsigned int bw_dl;
    long unsigned int max;
    long unsigned int saved_idle_calls;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct sugov_cpu {
    struct update_util_data update_util;
    struct sugov_policy *sg_policy;
    unsigned int cpu;
    bool iowait_boost_pending;
    unsigned int iowait_boost;
    u64 last_update;
    long unsigned int bw_dl;
    long unsigned int max;
    long unsigned int saved_idle_calls;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct sugov_cpu {
    struct update_util_data update_util;
    struct sugov_policy *sg_policy;
    unsigned int cpu;
    bool iowait_boost_pending;
    unsigned int iowait_boost;
    u64 last_update;
    long unsigned int bw_dl;
    long unsigned int max;
    long unsigned int saved_idle_calls;
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
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int saved_idle_calls</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int cached_raw_freq</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int cpu</code>
</li>
<li>
<b>Field added. </b>
<code>bool iowait_boost_pending</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int iowait_boost</code> ➡️ <code>unsigned int iowait_boost</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int iowait_boost_max</code> ➡️ <code>unsigned int iowait_boost_max</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int util_cfs</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int util_dl</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int util</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int flags</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int bw_dl</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int util_cfs</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int util_dl</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned int iowait_boost_max</code>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int util</code>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>long unsigned int max</code>
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
<code>long unsigned int bw_min</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int bw_dl</code>
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
