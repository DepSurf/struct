# Struct: <code>hrtimer_cpu_base</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct hrtimer_cpu_base {
    raw_spinlock_t lock;
    seqcount_t seq;
    struct hrtimer *running;
    unsigned int cpu;
    unsigned int active_bases;
    unsigned int clock_was_set_seq;
    bool migration_enabled;
    bool nohz_active;
    unsigned int in_hrtirq;
    unsigned int hres_active;
    unsigned int hang_detected;
    ktime_t expires_next;
    struct hrtimer *next_timer;
    unsigned int nr_events;
    unsigned int nr_retries;
    unsigned int nr_hangs;
    unsigned int max_hang_time;
    struct hrtimer_clock_base clock_base[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct hrtimer_cpu_base {
    raw_spinlock_t lock;
    seqcount_t seq;
    struct hrtimer *running;
    unsigned int cpu;
    unsigned int active_bases;
    unsigned int clock_was_set_seq;
    bool migration_enabled;
    bool nohz_active;
    unsigned int in_hrtirq;
    unsigned int hres_active;
    unsigned int hang_detected;
    ktime_t expires_next;
    struct hrtimer *next_timer;
    unsigned int nr_events;
    unsigned int nr_retries;
    unsigned int nr_hangs;
    unsigned int max_hang_time;
    struct hrtimer_clock_base clock_base[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct hrtimer_cpu_base {
    raw_spinlock_t lock;
    seqcount_t seq;
    struct hrtimer *running;
    unsigned int cpu;
    unsigned int active_bases;
    unsigned int clock_was_set_seq;
    bool migration_enabled;
    bool nohz_active;
    unsigned int in_hrtirq;
    unsigned int hres_active;
    unsigned int hang_detected;
    ktime_t expires_next;
    struct hrtimer *next_timer;
    unsigned int nr_events;
    unsigned int nr_retries;
    unsigned int nr_hangs;
    unsigned int max_hang_time;
    struct hrtimer_clock_base clock_base[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct hrtimer_cpu_base {
    raw_spinlock_t lock;
    seqcount_t seq;
    struct hrtimer *running;
    unsigned int cpu;
    unsigned int active_bases;
    unsigned int clock_was_set_seq;
    bool migration_enabled;
    bool nohz_active;
    unsigned int in_hrtirq;
    unsigned int hres_active;
    unsigned int hang_detected;
    ktime_t expires_next;
    struct hrtimer *next_timer;
    unsigned int nr_events;
    unsigned int nr_retries;
    unsigned int nr_hangs;
    unsigned int max_hang_time;
    struct hrtimer_clock_base clock_base[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct hrtimer_cpu_base {
    raw_spinlock_t lock;
    seqcount_t seq;
    struct hrtimer *running;
    unsigned int cpu;
    unsigned int active_bases;
    unsigned int clock_was_set_seq;
    bool migration_enabled;
    bool nohz_active;
    unsigned int in_hrtirq;
    unsigned int hres_active;
    unsigned int hang_detected;
    ktime_t expires_next;
    struct hrtimer *next_timer;
    unsigned int nr_events;
    unsigned int nr_retries;
    unsigned int nr_hangs;
    unsigned int max_hang_time;
    struct hrtimer_clock_base clock_base[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct hrtimer_cpu_base {
    raw_spinlock_t lock;
    unsigned int cpu;
    unsigned int active_bases;
    unsigned int clock_was_set_seq;
    unsigned int hres_active;
    unsigned int in_hrtirq;
    unsigned int hang_detected;
    unsigned int softirq_activated;
    unsigned int nr_events;
    short unsigned int nr_retries;
    short unsigned int nr_hangs;
    unsigned int max_hang_time;
    ktime_t expires_next;
    struct hrtimer *next_timer;
    ktime_t softirq_expires_next;
    struct hrtimer *softirq_next_timer;
    struct hrtimer_clock_base clock_base[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct hrtimer_cpu_base {
    raw_spinlock_t lock;
    unsigned int cpu;
    unsigned int active_bases;
    unsigned int clock_was_set_seq;
    unsigned int hres_active;
    unsigned int in_hrtirq;
    unsigned int hang_detected;
    unsigned int softirq_activated;
    unsigned int nr_events;
    short unsigned int nr_retries;
    short unsigned int nr_hangs;
    unsigned int max_hang_time;
    ktime_t expires_next;
    struct hrtimer *next_timer;
    ktime_t softirq_expires_next;
    struct hrtimer *softirq_next_timer;
    struct hrtimer_clock_base clock_base[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct hrtimer_cpu_base {
    raw_spinlock_t lock;
    unsigned int cpu;
    unsigned int active_bases;
    unsigned int clock_was_set_seq;
    unsigned int hres_active;
    unsigned int in_hrtirq;
    unsigned int hang_detected;
    unsigned int softirq_activated;
    unsigned int nr_events;
    short unsigned int nr_retries;
    short unsigned int nr_hangs;
    unsigned int max_hang_time;
    ktime_t expires_next;
    struct hrtimer *next_timer;
    ktime_t softirq_expires_next;
    struct hrtimer *softirq_next_timer;
    struct hrtimer_clock_base clock_base[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct hrtimer_cpu_base {
    raw_spinlock_t lock;
    unsigned int cpu;
    unsigned int active_bases;
    unsigned int clock_was_set_seq;
    unsigned int hres_active;
    unsigned int in_hrtirq;
    unsigned int hang_detected;
    unsigned int softirq_activated;
    unsigned int nr_events;
    short unsigned int nr_retries;
    short unsigned int nr_hangs;
    unsigned int max_hang_time;
    ktime_t expires_next;
    struct hrtimer *next_timer;
    ktime_t softirq_expires_next;
    struct hrtimer *softirq_next_timer;
    struct hrtimer_clock_base clock_base[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct hrtimer_cpu_base {
    raw_spinlock_t lock;
    unsigned int cpu;
    unsigned int active_bases;
    unsigned int clock_was_set_seq;
    unsigned int hres_active;
    unsigned int in_hrtirq;
    unsigned int hang_detected;
    unsigned int softirq_activated;
    unsigned int nr_events;
    short unsigned int nr_retries;
    short unsigned int nr_hangs;
    unsigned int max_hang_time;
    ktime_t expires_next;
    struct hrtimer *next_timer;
    ktime_t softirq_expires_next;
    struct hrtimer *softirq_next_timer;
    struct hrtimer_clock_base clock_base[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct hrtimer_cpu_base {
    raw_spinlock_t lock;
    unsigned int cpu;
    unsigned int active_bases;
    unsigned int clock_was_set_seq;
    unsigned int hres_active;
    unsigned int in_hrtirq;
    unsigned int hang_detected;
    unsigned int softirq_activated;
    unsigned int nr_events;
    short unsigned int nr_retries;
    short unsigned int nr_hangs;
    unsigned int max_hang_time;
    ktime_t expires_next;
    struct hrtimer *next_timer;
    ktime_t softirq_expires_next;
    struct hrtimer *softirq_next_timer;
    struct hrtimer_clock_base clock_base[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct hrtimer_cpu_base {
    raw_spinlock_t lock;
    unsigned int cpu;
    unsigned int active_bases;
    unsigned int clock_was_set_seq;
    unsigned int hres_active;
    unsigned int in_hrtirq;
    unsigned int hang_detected;
    unsigned int softirq_activated;
    unsigned int nr_events;
    short unsigned int nr_retries;
    short unsigned int nr_hangs;
    unsigned int max_hang_time;
    ktime_t expires_next;
    struct hrtimer *next_timer;
    ktime_t softirq_expires_next;
    struct hrtimer *softirq_next_timer;
    struct hrtimer_clock_base clock_base[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct hrtimer_cpu_base {
    raw_spinlock_t lock;
    unsigned int cpu;
    unsigned int active_bases;
    unsigned int clock_was_set_seq;
    unsigned int hres_active;
    unsigned int in_hrtirq;
    unsigned int hang_detected;
    unsigned int softirq_activated;
    unsigned int nr_events;
    short unsigned int nr_retries;
    short unsigned int nr_hangs;
    unsigned int max_hang_time;
    ktime_t expires_next;
    struct hrtimer *next_timer;
    ktime_t softirq_expires_next;
    struct hrtimer *softirq_next_timer;
    struct hrtimer_clock_base clock_base[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct hrtimer_cpu_base {
    raw_spinlock_t lock;
    unsigned int cpu;
    unsigned int active_bases;
    unsigned int clock_was_set_seq;
    unsigned int hres_active;
    unsigned int in_hrtirq;
    unsigned int hang_detected;
    unsigned int softirq_activated;
    unsigned int nr_events;
    short unsigned int nr_retries;
    short unsigned int nr_hangs;
    unsigned int max_hang_time;
    ktime_t expires_next;
    struct hrtimer *next_timer;
    ktime_t softirq_expires_next;
    struct hrtimer *softirq_next_timer;
    struct hrtimer_clock_base clock_base[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct hrtimer_cpu_base {
    raw_spinlock_t lock;
    unsigned int cpu;
    unsigned int active_bases;
    unsigned int clock_was_set_seq;
    unsigned int hres_active;
    unsigned int in_hrtirq;
    unsigned int hang_detected;
    unsigned int softirq_activated;
    unsigned int nr_events;
    short unsigned int nr_retries;
    short unsigned int nr_hangs;
    unsigned int max_hang_time;
    ktime_t expires_next;
    struct hrtimer *next_timer;
    ktime_t softirq_expires_next;
    struct hrtimer *softirq_next_timer;
    struct hrtimer_clock_base clock_base[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct hrtimer_cpu_base {
    raw_spinlock_t lock;
    unsigned int cpu;
    unsigned int active_bases;
    unsigned int clock_was_set_seq;
    unsigned int hres_active;
    unsigned int in_hrtirq;
    unsigned int hang_detected;
    unsigned int softirq_activated;
    unsigned int nr_events;
    short unsigned int nr_retries;
    short unsigned int nr_hangs;
    unsigned int max_hang_time;
    ktime_t expires_next;
    struct hrtimer *next_timer;
    ktime_t softirq_expires_next;
    struct hrtimer *softirq_next_timer;
    struct hrtimer_clock_base clock_base[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct hrtimer_cpu_base {
    raw_spinlock_t lock;
    unsigned int cpu;
    unsigned int active_bases;
    unsigned int clock_was_set_seq;
    unsigned int hres_active;
    unsigned int in_hrtirq;
    unsigned int hang_detected;
    unsigned int softirq_activated;
    unsigned int online;
    unsigned int nr_events;
    short unsigned int nr_retries;
    short unsigned int nr_hangs;
    unsigned int max_hang_time;
    ktime_t expires_next;
    struct hrtimer *next_timer;
    ktime_t softirq_expires_next;
    struct hrtimer *softirq_next_timer;
    struct hrtimer_clock_base clock_base[8];
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
struct hrtimer_cpu_base {
    raw_spinlock_t lock;
    unsigned int cpu;
    unsigned int active_bases;
    unsigned int clock_was_set_seq;
    unsigned int hres_active;
    unsigned int in_hrtirq;
    unsigned int hang_detected;
    unsigned int softirq_activated;
    unsigned int nr_events;
    short unsigned int nr_retries;
    short unsigned int nr_hangs;
    unsigned int max_hang_time;
    ktime_t expires_next;
    struct hrtimer *next_timer;
    ktime_t softirq_expires_next;
    struct hrtimer *softirq_next_timer;
    struct hrtimer_clock_base clock_base[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct hrtimer_cpu_base {
    raw_spinlock_t lock;
    unsigned int cpu;
    unsigned int active_bases;
    unsigned int clock_was_set_seq;
    unsigned int hres_active;
    unsigned int in_hrtirq;
    unsigned int hang_detected;
    unsigned int softirq_activated;
    unsigned int nr_events;
    short unsigned int nr_retries;
    short unsigned int nr_hangs;
    unsigned int max_hang_time;
    ktime_t expires_next;
    struct hrtimer *next_timer;
    ktime_t softirq_expires_next;
    struct hrtimer *softirq_next_timer;
    struct hrtimer_clock_base clock_base[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct hrtimer_cpu_base {
    raw_spinlock_t lock;
    unsigned int cpu;
    unsigned int active_bases;
    unsigned int clock_was_set_seq;
    unsigned int hres_active;
    unsigned int in_hrtirq;
    unsigned int hang_detected;
    unsigned int softirq_activated;
    unsigned int nr_events;
    short unsigned int nr_retries;
    short unsigned int nr_hangs;
    unsigned int max_hang_time;
    ktime_t expires_next;
    struct hrtimer *next_timer;
    ktime_t softirq_expires_next;
    struct hrtimer *softirq_next_timer;
    struct hrtimer_clock_base clock_base[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct hrtimer_cpu_base {
    raw_spinlock_t lock;
    unsigned int cpu;
    unsigned int active_bases;
    unsigned int clock_was_set_seq;
    unsigned int hres_active;
    unsigned int in_hrtirq;
    unsigned int hang_detected;
    unsigned int softirq_activated;
    unsigned int nr_events;
    short unsigned int nr_retries;
    short unsigned int nr_hangs;
    unsigned int max_hang_time;
    ktime_t expires_next;
    struct hrtimer *next_timer;
    ktime_t softirq_expires_next;
    struct hrtimer *softirq_next_timer;
    struct hrtimer_clock_base clock_base[8];
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
struct hrtimer_cpu_base {
    raw_spinlock_t lock;
    unsigned int cpu;
    unsigned int active_bases;
    unsigned int clock_was_set_seq;
    unsigned int hres_active;
    unsigned int in_hrtirq;
    unsigned int hang_detected;
    unsigned int softirq_activated;
    unsigned int nr_events;
    short unsigned int nr_retries;
    short unsigned int nr_hangs;
    unsigned int max_hang_time;
    ktime_t expires_next;
    struct hrtimer *next_timer;
    ktime_t softirq_expires_next;
    struct hrtimer *softirq_next_timer;
    struct hrtimer_clock_base clock_base[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct hrtimer_cpu_base {
    raw_spinlock_t lock;
    unsigned int cpu;
    unsigned int active_bases;
    unsigned int clock_was_set_seq;
    unsigned int hres_active;
    unsigned int in_hrtirq;
    unsigned int hang_detected;
    unsigned int softirq_activated;
    unsigned int nr_events;
    short unsigned int nr_retries;
    short unsigned int nr_hangs;
    unsigned int max_hang_time;
    ktime_t expires_next;
    struct hrtimer *next_timer;
    ktime_t softirq_expires_next;
    struct hrtimer *softirq_next_timer;
    struct hrtimer_clock_base clock_base[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct hrtimer_cpu_base {
    raw_spinlock_t lock;
    unsigned int cpu;
    unsigned int active_bases;
    unsigned int clock_was_set_seq;
    unsigned int hres_active;
    unsigned int in_hrtirq;
    unsigned int hang_detected;
    unsigned int softirq_activated;
    unsigned int nr_events;
    short unsigned int nr_retries;
    short unsigned int nr_hangs;
    unsigned int max_hang_time;
    ktime_t expires_next;
    struct hrtimer *next_timer;
    ktime_t softirq_expires_next;
    struct hrtimer *softirq_next_timer;
    struct hrtimer_clock_base clock_base[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct hrtimer_cpu_base {
    raw_spinlock_t lock;
    unsigned int cpu;
    unsigned int active_bases;
    unsigned int clock_was_set_seq;
    unsigned int hres_active;
    unsigned int in_hrtirq;
    unsigned int hang_detected;
    unsigned int softirq_activated;
    unsigned int nr_events;
    short unsigned int nr_retries;
    short unsigned int nr_hangs;
    unsigned int max_hang_time;
    ktime_t expires_next;
    struct hrtimer *next_timer;
    ktime_t softirq_expires_next;
    struct hrtimer *softirq_next_timer;
    struct hrtimer_clock_base clock_base[8];
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
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int softirq_activated</code>
</li>
<li>
<b>Field added. </b>
<code>ktime_t softirq_expires_next</code>
</li>
<li>
<b>Field added. </b>
<code>struct hrtimer *softirq_next_timer</code>
</li>
<li>
<b>Field removed. </b>
<code>seqcount_t seq</code>
</li>
<li>
<b>Field removed. </b>
<code>struct hrtimer *running</code>
</li>
<li>
<b>Field removed. </b>
<code>bool migration_enabled</code>
</li>
<li>
<b>Field removed. </b>
<code>bool nohz_active</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int nr_retries</code> ➡️ <code>short unsigned int nr_retries</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int nr_hangs</code> ➡️ <code>short unsigned int nr_hangs</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct hrtimer_clock_base clock_base[4]</code> ➡️ <code>struct hrtimer_clock_base clock_base[8]</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int online</code>
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
