# Struct: <code>cpuidle_state</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct cpuidle_state {
    char name[16];
    char desc[32];
    unsigned int flags;
    unsigned int exit_latency;
    int power_usage;
    unsigned int target_residency;
    bool disabled;
    int (*enter)(struct cpuidle_device *, struct cpuidle_driver *, int);
    int (*enter_dead)(struct cpuidle_device *, int);
    void (*enter_freeze)(struct cpuidle_device *, struct cpuidle_driver *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct cpuidle_state {
    char name[16];
    char desc[32];
    unsigned int flags;
    unsigned int exit_latency;
    int power_usage;
    unsigned int target_residency;
    bool disabled;
    int (*enter)(struct cpuidle_device *, struct cpuidle_driver *, int);
    int (*enter_dead)(struct cpuidle_device *, int);
    void (*enter_freeze)(struct cpuidle_device *, struct cpuidle_driver *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct cpuidle_state {
    char name[16];
    char desc[32];
    unsigned int flags;
    unsigned int exit_latency;
    int power_usage;
    unsigned int target_residency;
    bool disabled;
    int (*enter)(struct cpuidle_device *, struct cpuidle_driver *, int);
    int (*enter_dead)(struct cpuidle_device *, int);
    void (*enter_freeze)(struct cpuidle_device *, struct cpuidle_driver *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct cpuidle_state {
    char name[16];
    char desc[32];
    unsigned int flags;
    unsigned int exit_latency;
    int power_usage;
    unsigned int target_residency;
    bool disabled;
    int (*enter)(struct cpuidle_device *, struct cpuidle_driver *, int);
    int (*enter_dead)(struct cpuidle_device *, int);
    void (*enter_freeze)(struct cpuidle_device *, struct cpuidle_driver *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct cpuidle_state {
    char name[16];
    char desc[32];
    unsigned int flags;
    unsigned int exit_latency;
    int power_usage;
    unsigned int target_residency;
    bool disabled;
    int (*enter)(struct cpuidle_device *, struct cpuidle_driver *, int);
    int (*enter_dead)(struct cpuidle_device *, int);
    void (*enter_s2idle)(struct cpuidle_device *, struct cpuidle_driver *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct cpuidle_state {
    char name[16];
    char desc[32];
    unsigned int flags;
    unsigned int exit_latency;
    int power_usage;
    unsigned int target_residency;
    bool disabled;
    int (*enter)(struct cpuidle_device *, struct cpuidle_driver *, int);
    int (*enter_dead)(struct cpuidle_device *, int);
    void (*enter_s2idle)(struct cpuidle_device *, struct cpuidle_driver *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct cpuidle_state {
    char name[16];
    char desc[32];
    unsigned int flags;
    unsigned int exit_latency;
    int power_usage;
    unsigned int target_residency;
    bool disabled;
    int (*enter)(struct cpuidle_device *, struct cpuidle_driver *, int);
    int (*enter_dead)(struct cpuidle_device *, int);
    void (*enter_s2idle)(struct cpuidle_device *, struct cpuidle_driver *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct cpuidle_state {
    char name[16];
    char desc[32];
    unsigned int flags;
    unsigned int exit_latency;
    int power_usage;
    unsigned int target_residency;
    bool disabled;
    int (*enter)(struct cpuidle_device *, struct cpuidle_driver *, int);
    int (*enter_dead)(struct cpuidle_device *, int);
    void (*enter_s2idle)(struct cpuidle_device *, struct cpuidle_driver *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct cpuidle_state {
    char name[16];
    char desc[32];
    unsigned int flags;
    unsigned int exit_latency;
    int power_usage;
    unsigned int target_residency;
    bool disabled;
    int (*enter)(struct cpuidle_device *, struct cpuidle_driver *, int);
    int (*enter_dead)(struct cpuidle_device *, int);
    void (*enter_s2idle)(struct cpuidle_device *, struct cpuidle_driver *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct cpuidle_state {
    char name[16];
    char desc[32];
    u64 exit_latency_ns;
    u64 target_residency_ns;
    unsigned int flags;
    unsigned int exit_latency;
    int power_usage;
    unsigned int target_residency;
    int (*enter)(struct cpuidle_device *, struct cpuidle_driver *, int);
    int (*enter_dead)(struct cpuidle_device *, int);
    void (*enter_s2idle)(struct cpuidle_device *, struct cpuidle_driver *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct cpuidle_state {
    char name[16];
    char desc[32];
    u64 exit_latency_ns;
    u64 target_residency_ns;
    unsigned int flags;
    unsigned int exit_latency;
    int power_usage;
    unsigned int target_residency;
    int (*enter)(struct cpuidle_device *, struct cpuidle_driver *, int);
    int (*enter_dead)(struct cpuidle_device *, int);
    int (*enter_s2idle)(struct cpuidle_device *, struct cpuidle_driver *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct cpuidle_state {
    char name[16];
    char desc[32];
    s64 exit_latency_ns;
    s64 target_residency_ns;
    unsigned int flags;
    unsigned int exit_latency;
    int power_usage;
    unsigned int target_residency;
    int (*enter)(struct cpuidle_device *, struct cpuidle_driver *, int);
    int (*enter_dead)(struct cpuidle_device *, int);
    int (*enter_s2idle)(struct cpuidle_device *, struct cpuidle_driver *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct cpuidle_state {
    char name[16];
    char desc[32];
    s64 exit_latency_ns;
    s64 target_residency_ns;
    unsigned int flags;
    unsigned int exit_latency;
    int power_usage;
    unsigned int target_residency;
    int (*enter)(struct cpuidle_device *, struct cpuidle_driver *, int);
    int (*enter_dead)(struct cpuidle_device *, int);
    int (*enter_s2idle)(struct cpuidle_device *, struct cpuidle_driver *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct cpuidle_state {
    char name[16];
    char desc[32];
    s64 exit_latency_ns;
    s64 target_residency_ns;
    unsigned int flags;
    unsigned int exit_latency;
    int power_usage;
    unsigned int target_residency;
    int (*enter)(struct cpuidle_device *, struct cpuidle_driver *, int);
    int (*enter_dead)(struct cpuidle_device *, int);
    int (*enter_s2idle)(struct cpuidle_device *, struct cpuidle_driver *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct cpuidle_state {
    char name[16];
    char desc[32];
    s64 exit_latency_ns;
    s64 target_residency_ns;
    unsigned int flags;
    unsigned int exit_latency;
    int power_usage;
    unsigned int target_residency;
    int (*enter)(struct cpuidle_device *, struct cpuidle_driver *, int);
    int (*enter_dead)(struct cpuidle_device *, int);
    int (*enter_s2idle)(struct cpuidle_device *, struct cpuidle_driver *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct cpuidle_state {
    char name[16];
    char desc[32];
    s64 exit_latency_ns;
    s64 target_residency_ns;
    unsigned int flags;
    unsigned int exit_latency;
    int power_usage;
    unsigned int target_residency;
    int (*enter)(struct cpuidle_device *, struct cpuidle_driver *, int);
    int (*enter_dead)(struct cpuidle_device *, int);
    int (*enter_s2idle)(struct cpuidle_device *, struct cpuidle_driver *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct cpuidle_state {
    char name[16];
    char desc[32];
    s64 exit_latency_ns;
    s64 target_residency_ns;
    unsigned int flags;
    unsigned int exit_latency;
    int power_usage;
    unsigned int target_residency;
    int (*enter)(struct cpuidle_device *, struct cpuidle_driver *, int);
    int (*enter_dead)(struct cpuidle_device *, int);
    int (*enter_s2idle)(struct cpuidle_device *, struct cpuidle_driver *, int);
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
struct cpuidle_state {
    char name[16];
    char desc[32];
    unsigned int flags;
    unsigned int exit_latency;
    int power_usage;
    unsigned int target_residency;
    bool disabled;
    int (*enter)(struct cpuidle_device *, struct cpuidle_driver *, int);
    int (*enter_dead)(struct cpuidle_device *, int);
    void (*enter_s2idle)(struct cpuidle_device *, struct cpuidle_driver *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct cpuidle_state {
    char name[16];
    char desc[32];
    unsigned int flags;
    unsigned int exit_latency;
    int power_usage;
    unsigned int target_residency;
    bool disabled;
    int (*enter)(struct cpuidle_device *, struct cpuidle_driver *, int);
    int (*enter_dead)(struct cpuidle_device *, int);
    void (*enter_s2idle)(struct cpuidle_device *, struct cpuidle_driver *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct cpuidle_state {
    char name[16];
    char desc[32];
    unsigned int flags;
    unsigned int exit_latency;
    int power_usage;
    unsigned int target_residency;
    bool disabled;
    int (*enter)(struct cpuidle_device *, struct cpuidle_driver *, int);
    int (*enter_dead)(struct cpuidle_device *, int);
    void (*enter_s2idle)(struct cpuidle_device *, struct cpuidle_driver *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct cpuidle_state {
    char name[16];
    char desc[32];
    unsigned int flags;
    unsigned int exit_latency;
    int power_usage;
    unsigned int target_residency;
    bool disabled;
    int (*enter)(struct cpuidle_device *, struct cpuidle_driver *, int);
    int (*enter_dead)(struct cpuidle_device *, int);
    void (*enter_s2idle)(struct cpuidle_device *, struct cpuidle_driver *, int);
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
struct cpuidle_state {
    char name[16];
    char desc[32];
    unsigned int flags;
    unsigned int exit_latency;
    int power_usage;
    unsigned int target_residency;
    bool disabled;
    int (*enter)(struct cpuidle_device *, struct cpuidle_driver *, int);
    int (*enter_dead)(struct cpuidle_device *, int);
    void (*enter_s2idle)(struct cpuidle_device *, struct cpuidle_driver *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct cpuidle_state {
    char name[16];
    char desc[32];
    unsigned int flags;
    unsigned int exit_latency;
    int power_usage;
    unsigned int target_residency;
    bool disabled;
    int (*enter)(struct cpuidle_device *, struct cpuidle_driver *, int);
    int (*enter_dead)(struct cpuidle_device *, int);
    void (*enter_s2idle)(struct cpuidle_device *, struct cpuidle_driver *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct cpuidle_state {
    char name[16];
    char desc[32];
    unsigned int flags;
    unsigned int exit_latency;
    int power_usage;
    unsigned int target_residency;
    bool disabled;
    int (*enter)(struct cpuidle_device *, struct cpuidle_driver *, int);
    int (*enter_dead)(struct cpuidle_device *, int);
    void (*enter_s2idle)(struct cpuidle_device *, struct cpuidle_driver *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cpuidle_state {
    char name[16];
    char desc[32];
    unsigned int flags;
    unsigned int exit_latency;
    int power_usage;
    unsigned int target_residency;
    bool disabled;
    int (*enter)(struct cpuidle_device *, struct cpuidle_driver *, int);
    int (*enter_dead)(struct cpuidle_device *, int);
    void (*enter_s2idle)(struct cpuidle_device *, struct cpuidle_driver *, int);
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
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*enter_s2idle)(struct cpuidle_device *, struct cpuidle_driver *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*enter_freeze)(struct cpuidle_device *, struct cpuidle_driver *, int)</code>
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
<code>u64 exit_latency_ns</code>
</li>
<li>
<b>Field added. </b>
<code>u64 target_residency_ns</code>
</li>
<li>
<b>Field removed. </b>
<code>bool disabled</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>void (*enter_s2idle)(struct cpuidle_device *, struct cpuidle_driver *, int)</code> ➡️ <code>int (*enter_s2idle)(struct cpuidle_device *, struct cpuidle_driver *, int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>u64 exit_latency_ns</code> ➡️ <code>s64 exit_latency_ns</code>
</li>
<li>
<b>Field type changed. </b>
<code>u64 target_residency_ns</code> ➡️ <code>s64 target_residency_ns</code>
</li>
</ul>
</details>
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
