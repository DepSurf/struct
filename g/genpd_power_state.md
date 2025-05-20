# Struct: <code>genpd_power_state</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct genpd_power_state {
    s64 power_off_latency_ns;
    s64 power_on_latency_ns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct genpd_power_state {
    s64 power_off_latency_ns;
    s64 power_on_latency_ns;
    s64 residency_ns;
    struct fwnode_handle *fwnode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct genpd_power_state {
    s64 power_off_latency_ns;
    s64 power_on_latency_ns;
    s64 residency_ns;
    struct fwnode_handle *fwnode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct genpd_power_state {
    s64 power_off_latency_ns;
    s64 power_on_latency_ns;
    s64 residency_ns;
    struct fwnode_handle *fwnode;
    ktime_t idle_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct genpd_power_state {
    s64 power_off_latency_ns;
    s64 power_on_latency_ns;
    s64 residency_ns;
    struct fwnode_handle *fwnode;
    ktime_t idle_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct genpd_power_state {
    s64 power_off_latency_ns;
    s64 power_on_latency_ns;
    s64 residency_ns;
    struct fwnode_handle *fwnode;
    ktime_t idle_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct genpd_power_state {
    s64 power_off_latency_ns;
    s64 power_on_latency_ns;
    s64 residency_ns;
    struct fwnode_handle *fwnode;
    ktime_t idle_time;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct genpd_power_state {
    s64 power_off_latency_ns;
    s64 power_on_latency_ns;
    s64 residency_ns;
    struct fwnode_handle *fwnode;
    ktime_t idle_time;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct genpd_power_state {
    s64 power_off_latency_ns;
    s64 power_on_latency_ns;
    s64 residency_ns;
    struct fwnode_handle *fwnode;
    ktime_t idle_time;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct genpd_power_state {
    s64 power_off_latency_ns;
    s64 power_on_latency_ns;
    s64 residency_ns;
    u64 usage;
    u64 rejected;
    struct fwnode_handle *fwnode;
    ktime_t idle_time;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct genpd_power_state {
    s64 power_off_latency_ns;
    s64 power_on_latency_ns;
    s64 residency_ns;
    u64 usage;
    u64 rejected;
    struct fwnode_handle *fwnode;
    ktime_t idle_time;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct genpd_power_state {
    s64 power_off_latency_ns;
    s64 power_on_latency_ns;
    s64 residency_ns;
    u64 usage;
    u64 rejected;
    struct fwnode_handle *fwnode;
    ktime_t idle_time;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct genpd_power_state {
    s64 power_off_latency_ns;
    s64 power_on_latency_ns;
    s64 residency_ns;
    u64 usage;
    u64 rejected;
    struct fwnode_handle *fwnode;
    u64 idle_time;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct genpd_power_state {
    s64 power_off_latency_ns;
    s64 power_on_latency_ns;
    s64 residency_ns;
    u64 usage;
    u64 rejected;
    struct fwnode_handle *fwnode;
    u64 idle_time;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct genpd_power_state {
    s64 power_off_latency_ns;
    s64 power_on_latency_ns;
    s64 residency_ns;
    u64 usage;
    u64 rejected;
    struct fwnode_handle *fwnode;
    u64 idle_time;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct genpd_power_state {
    s64 power_off_latency_ns;
    s64 power_on_latency_ns;
    s64 residency_ns;
    u64 usage;
    u64 rejected;
    struct fwnode_handle *fwnode;
    u64 idle_time;
    void *data;
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
struct genpd_power_state {
    s64 power_off_latency_ns;
    s64 power_on_latency_ns;
    s64 residency_ns;
    struct fwnode_handle *fwnode;
    ktime_t idle_time;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct genpd_power_state {
    s64 power_off_latency_ns;
    s64 power_on_latency_ns;
    s64 residency_ns;
    struct fwnode_handle *fwnode;
    ktime_t idle_time;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct genpd_power_state {
    s64 power_off_latency_ns;
    s64 power_on_latency_ns;
    s64 residency_ns;
    struct fwnode_handle *fwnode;
    ktime_t idle_time;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct genpd_power_state {
    s64 power_off_latency_ns;
    s64 power_on_latency_ns;
    s64 residency_ns;
    struct fwnode_handle *fwnode;
    ktime_t idle_time;
    void *data;
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
struct genpd_power_state {
    s64 power_off_latency_ns;
    s64 power_on_latency_ns;
    s64 residency_ns;
    struct fwnode_handle *fwnode;
    ktime_t idle_time;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct genpd_power_state {
    s64 power_off_latency_ns;
    s64 power_on_latency_ns;
    s64 residency_ns;
    struct fwnode_handle *fwnode;
    ktime_t idle_time;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct genpd_power_state {
    s64 power_off_latency_ns;
    s64 power_on_latency_ns;
    s64 residency_ns;
    struct fwnode_handle *fwnode;
    ktime_t idle_time;
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct genpd_power_state {
    s64 power_off_latency_ns;
    s64 power_on_latency_ns;
    s64 residency_ns;
    struct fwnode_handle *fwnode;
    ktime_t idle_time;
    void *data;
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
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>s64 residency_ns</code>
</li>
<li>
<b>Field added. </b>
<code>struct fwnode_handle *fwnode</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>ktime_t idle_time</code>
</li>
</ul>
</details>
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
<code>void *data</code>
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
<code>u64 usage</code>
</li>
<li>
<b>Field added. </b>
<code>u64 rejected</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>ktime_t idle_time</code> ➡️ <code>u64 idle_time</code>
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
