# Struct: <code>timer_base</code>

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
struct timer_base {
    spinlock_t lock;
    struct timer_list *running_timer;
    long unsigned int clk;
    long unsigned int next_expiry;
    unsigned int cpu;
    bool migration_enabled;
    bool nohz_active;
    bool is_idle;
    long unsigned int pending_map[9];
    struct hlist_head vectors[576];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct timer_base {
    spinlock_t lock;
    struct timer_list *running_timer;
    long unsigned int clk;
    long unsigned int next_expiry;
    unsigned int cpu;
    bool migration_enabled;
    bool nohz_active;
    bool is_idle;
    long unsigned int pending_map[9];
    struct hlist_head vectors[576];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct timer_base {
    raw_spinlock_t lock;
    struct timer_list *running_timer;
    long unsigned int clk;
    long unsigned int next_expiry;
    unsigned int cpu;
    bool migration_enabled;
    bool nohz_active;
    bool is_idle;
    bool must_forward_clk;
    long unsigned int pending_map[9];
    struct hlist_head vectors[576];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct timer_base {
    raw_spinlock_t lock;
    struct timer_list *running_timer;
    long unsigned int clk;
    long unsigned int next_expiry;
    unsigned int cpu;
    bool migration_enabled;
    bool nohz_active;
    bool is_idle;
    bool must_forward_clk;
    long unsigned int pending_map[9];
    struct hlist_head vectors[576];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct timer_base {
    raw_spinlock_t lock;
    struct timer_list *running_timer;
    long unsigned int clk;
    long unsigned int next_expiry;
    unsigned int cpu;
    bool is_idle;
    bool must_forward_clk;
    long unsigned int pending_map[9];
    struct hlist_head vectors[576];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct timer_base {
    raw_spinlock_t lock;
    struct timer_list *running_timer;
    long unsigned int clk;
    long unsigned int next_expiry;
    unsigned int cpu;
    bool is_idle;
    bool must_forward_clk;
    long unsigned int pending_map[9];
    struct hlist_head vectors[576];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct timer_base {
    raw_spinlock_t lock;
    struct timer_list *running_timer;
    long unsigned int clk;
    long unsigned int next_expiry;
    unsigned int cpu;
    bool is_idle;
    bool must_forward_clk;
    long unsigned int pending_map[9];
    struct hlist_head vectors[576];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct timer_base {
    raw_spinlock_t lock;
    struct timer_list *running_timer;
    long unsigned int clk;
    long unsigned int next_expiry;
    unsigned int cpu;
    bool is_idle;
    bool must_forward_clk;
    long unsigned int pending_map[9];
    struct hlist_head vectors[576];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct timer_base {
    raw_spinlock_t lock;
    struct timer_list *running_timer;
    long unsigned int clk;
    long unsigned int next_expiry;
    unsigned int cpu;
    bool is_idle;
    bool must_forward_clk;
    long unsigned int pending_map[9];
    struct hlist_head vectors[576];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct timer_base {
    raw_spinlock_t lock;
    struct timer_list *running_timer;
    long unsigned int clk;
    long unsigned int next_expiry;
    unsigned int cpu;
    bool next_expiry_recalc;
    bool is_idle;
    long unsigned int pending_map[9];
    struct hlist_head vectors[576];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct timer_base {
    raw_spinlock_t lock;
    struct timer_list *running_timer;
    long unsigned int clk;
    long unsigned int next_expiry;
    unsigned int cpu;
    bool next_expiry_recalc;
    bool is_idle;
    bool timers_pending;
    long unsigned int pending_map[9];
    struct hlist_head vectors[576];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct timer_base {
    raw_spinlock_t lock;
    struct timer_list *running_timer;
    long unsigned int clk;
    long unsigned int next_expiry;
    unsigned int cpu;
    bool next_expiry_recalc;
    bool is_idle;
    bool timers_pending;
    long unsigned int pending_map[9];
    struct hlist_head vectors[576];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct timer_base {
    raw_spinlock_t lock;
    struct timer_list *running_timer;
    long unsigned int clk;
    long unsigned int next_expiry;
    unsigned int cpu;
    bool next_expiry_recalc;
    bool is_idle;
    bool timers_pending;
    long unsigned int pending_map[9];
    struct hlist_head vectors[576];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct timer_base {
    raw_spinlock_t lock;
    struct timer_list *running_timer;
    long unsigned int clk;
    long unsigned int next_expiry;
    unsigned int cpu;
    bool next_expiry_recalc;
    bool is_idle;
    bool timers_pending;
    long unsigned int pending_map[9];
    struct hlist_head vectors[576];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct timer_base {
    raw_spinlock_t lock;
    struct timer_list *running_timer;
    long unsigned int clk;
    long unsigned int next_expiry;
    unsigned int cpu;
    bool next_expiry_recalc;
    bool is_idle;
    bool timers_pending;
    long unsigned int pending_map[9];
    struct hlist_head vectors[576];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct timer_base {
    raw_spinlock_t lock;
    struct timer_list *running_timer;
    long unsigned int clk;
    long unsigned int next_expiry;
    unsigned int cpu;
    bool next_expiry_recalc;
    bool is_idle;
    bool timers_pending;
    long unsigned int pending_map[9];
    struct hlist_head vectors[576];
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
struct timer_base {
    raw_spinlock_t lock;
    struct timer_list *running_timer;
    long unsigned int clk;
    long unsigned int next_expiry;
    unsigned int cpu;
    bool is_idle;
    bool must_forward_clk;
    long unsigned int pending_map[9];
    struct hlist_head vectors[576];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct timer_base {
    raw_spinlock_t lock;
    struct timer_list *running_timer;
    long unsigned int clk;
    long unsigned int next_expiry;
    unsigned int cpu;
    bool is_idle;
    bool must_forward_clk;
    long unsigned int pending_map[18];
    struct hlist_head vectors[576];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct timer_base {
    raw_spinlock_t lock;
    struct timer_list *running_timer;
    long unsigned int clk;
    long unsigned int next_expiry;
    unsigned int cpu;
    bool is_idle;
    bool must_forward_clk;
    long unsigned int pending_map[9];
    struct hlist_head vectors[576];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct timer_base {
    raw_spinlock_t lock;
    struct timer_list *running_timer;
    long unsigned int clk;
    long unsigned int next_expiry;
    unsigned int cpu;
    bool is_idle;
    bool must_forward_clk;
    long unsigned int pending_map[9];
    struct hlist_head vectors[576];
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
struct timer_base {
    raw_spinlock_t lock;
    struct timer_list *running_timer;
    long unsigned int clk;
    long unsigned int next_expiry;
    unsigned int cpu;
    bool is_idle;
    bool must_forward_clk;
    long unsigned int pending_map[9];
    struct hlist_head vectors[576];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct timer_base {
    raw_spinlock_t lock;
    struct timer_list *running_timer;
    long unsigned int clk;
    long unsigned int next_expiry;
    unsigned int cpu;
    bool is_idle;
    bool must_forward_clk;
    long unsigned int pending_map[9];
    struct hlist_head vectors[576];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct timer_base {
    raw_spinlock_t lock;
    struct timer_list *running_timer;
    long unsigned int clk;
    long unsigned int next_expiry;
    unsigned int cpu;
    bool is_idle;
    bool must_forward_clk;
    long unsigned int pending_map[9];
    struct hlist_head vectors[576];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct timer_base {
    raw_spinlock_t lock;
    struct timer_list *running_timer;
    long unsigned int clk;
    long unsigned int next_expiry;
    unsigned int cpu;
    bool is_idle;
    bool must_forward_clk;
    long unsigned int pending_map[9];
    struct hlist_head vectors[576];
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool must_forward_clk</code>
</li>
<li>
<b>Field type changed. </b>
<code>spinlock_t lock</code> ➡️ <code>raw_spinlock_t lock</code>
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
<b>Field removed. </b>
<code>bool migration_enabled</code>
</li>
<li>
<b>Field removed. </b>
<code>bool nohz_active</code>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool next_expiry_recalc</code>
</li>
<li>
<b>Field removed. </b>
<code>bool must_forward_clk</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool timers_pending</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long unsigned int pending_map[9]</code> ➡️ <code>long unsigned int pending_map[18]</code>
</li>
</ul>
</details>
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
