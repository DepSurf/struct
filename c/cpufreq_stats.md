# Struct: <code>cpufreq_stats</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct cpufreq_stats {
    unsigned int total_trans;
    long long unsigned int last_time;
    unsigned int max_state;
    unsigned int state_num;
    unsigned int last_index;
    u64 *time_in_state;
    unsigned int *freq_table;
    unsigned int *trans_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct cpufreq_stats {
    unsigned int total_trans;
    long long unsigned int last_time;
    unsigned int max_state;
    unsigned int state_num;
    unsigned int last_index;
    u64 *time_in_state;
    unsigned int *freq_table;
    unsigned int *trans_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct cpufreq_stats {
    unsigned int total_trans;
    long long unsigned int last_time;
    unsigned int max_state;
    unsigned int state_num;
    unsigned int last_index;
    u64 *time_in_state;
    unsigned int *freq_table;
    unsigned int *trans_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct cpufreq_stats {
    unsigned int total_trans;
    long long unsigned int last_time;
    unsigned int max_state;
    unsigned int state_num;
    unsigned int last_index;
    u64 *time_in_state;
    unsigned int *freq_table;
    unsigned int *trans_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct cpufreq_stats {
    unsigned int total_trans;
    long long unsigned int last_time;
    unsigned int max_state;
    unsigned int state_num;
    unsigned int last_index;
    u64 *time_in_state;
    unsigned int *freq_table;
    unsigned int *trans_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct cpufreq_stats {
    unsigned int total_trans;
    long long unsigned int last_time;
    unsigned int max_state;
    unsigned int state_num;
    unsigned int last_index;
    u64 *time_in_state;
    unsigned int *freq_table;
    unsigned int *trans_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct cpufreq_stats {
    unsigned int total_trans;
    long long unsigned int last_time;
    unsigned int max_state;
    unsigned int state_num;
    unsigned int last_index;
    u64 *time_in_state;
    unsigned int *freq_table;
    unsigned int *trans_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct cpufreq_stats {
    unsigned int total_trans;
    long long unsigned int last_time;
    unsigned int max_state;
    unsigned int state_num;
    unsigned int last_index;
    u64 *time_in_state;
    spinlock_t lock;
    unsigned int *freq_table;
    unsigned int *trans_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct cpufreq_stats {
    unsigned int total_trans;
    long long unsigned int last_time;
    unsigned int max_state;
    unsigned int state_num;
    unsigned int last_index;
    u64 *time_in_state;
    spinlock_t lock;
    unsigned int *freq_table;
    unsigned int *trans_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct cpufreq_stats {
    unsigned int total_trans;
    long long unsigned int last_time;
    unsigned int max_state;
    unsigned int state_num;
    unsigned int last_index;
    u64 *time_in_state;
    spinlock_t lock;
    unsigned int *freq_table;
    unsigned int *trans_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct cpufreq_stats {
    unsigned int total_trans;
    long long unsigned int last_time;
    unsigned int max_state;
    unsigned int state_num;
    unsigned int last_index;
    u64 *time_in_state;
    unsigned int *freq_table;
    unsigned int *trans_table;
    unsigned int reset_pending;
    long long unsigned int reset_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct cpufreq_stats {
    unsigned int total_trans;
    long long unsigned int last_time;
    unsigned int max_state;
    unsigned int state_num;
    unsigned int last_index;
    u64 *time_in_state;
    unsigned int *freq_table;
    unsigned int *trans_table;
    unsigned int reset_pending;
    long long unsigned int reset_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct cpufreq_stats {
    unsigned int total_trans;
    long long unsigned int last_time;
    unsigned int max_state;
    unsigned int state_num;
    unsigned int last_index;
    u64 *time_in_state;
    unsigned int *freq_table;
    unsigned int *trans_table;
    unsigned int reset_pending;
    long long unsigned int reset_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct cpufreq_stats {
    unsigned int total_trans;
    long long unsigned int last_time;
    unsigned int max_state;
    unsigned int state_num;
    unsigned int last_index;
    u64 *time_in_state;
    unsigned int *freq_table;
    unsigned int *trans_table;
    unsigned int reset_pending;
    long long unsigned int reset_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct cpufreq_stats {
    unsigned int total_trans;
    long long unsigned int last_time;
    unsigned int max_state;
    unsigned int state_num;
    unsigned int last_index;
    u64 *time_in_state;
    unsigned int *freq_table;
    unsigned int *trans_table;
    unsigned int reset_pending;
    long long unsigned int reset_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct cpufreq_stats {
    unsigned int total_trans;
    long long unsigned int last_time;
    unsigned int max_state;
    unsigned int state_num;
    unsigned int last_index;
    u64 *time_in_state;
    unsigned int *freq_table;
    unsigned int *trans_table;
    unsigned int reset_pending;
    long long unsigned int reset_time;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct cpufreq_stats {
    unsigned int total_trans;
    long long unsigned int last_time;
    unsigned int max_state;
    unsigned int state_num;
    unsigned int last_index;
    u64 *time_in_state;
    unsigned int *freq_table;
    unsigned int *trans_table;
    unsigned int reset_pending;
    long long unsigned int reset_time;
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
struct cpufreq_stats {
    unsigned int total_trans;
    long long unsigned int last_time;
    unsigned int max_state;
    unsigned int state_num;
    unsigned int last_index;
    u64 *time_in_state;
    spinlock_t lock;
    unsigned int *freq_table;
    unsigned int *trans_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct cpufreq_stats {
    unsigned int total_trans;
    long long unsigned int last_time;
    unsigned int max_state;
    unsigned int state_num;
    unsigned int last_index;
    u64 *time_in_state;
    spinlock_t lock;
    unsigned int *freq_table;
    unsigned int *trans_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct cpufreq_stats {
    unsigned int total_trans;
    long long unsigned int last_time;
    unsigned int max_state;
    unsigned int state_num;
    unsigned int last_index;
    u64 *time_in_state;
    spinlock_t lock;
    unsigned int *freq_table;
    unsigned int *trans_table;
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
struct cpufreq_stats {
    unsigned int total_trans;
    long long unsigned int last_time;
    unsigned int max_state;
    unsigned int state_num;
    unsigned int last_index;
    u64 *time_in_state;
    spinlock_t lock;
    unsigned int *freq_table;
    unsigned int *trans_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct cpufreq_stats {
    unsigned int total_trans;
    long long unsigned int last_time;
    unsigned int max_state;
    unsigned int state_num;
    unsigned int last_index;
    u64 *time_in_state;
    spinlock_t lock;
    unsigned int *freq_table;
    unsigned int *trans_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct cpufreq_stats {
    unsigned int total_trans;
    long long unsigned int last_time;
    unsigned int max_state;
    unsigned int state_num;
    unsigned int last_index;
    u64 *time_in_state;
    spinlock_t lock;
    unsigned int *freq_table;
    unsigned int *trans_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cpufreq_stats {
    unsigned int total_trans;
    long long unsigned int last_time;
    unsigned int max_state;
    unsigned int state_num;
    unsigned int last_index;
    u64 *time_in_state;
    spinlock_t lock;
    unsigned int *freq_table;
    unsigned int *trans_table;
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>spinlock_t lock</code>
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
<code>unsigned int reset_pending</code>
</li>
<li>
<b>Field added. </b>
<code>long long unsigned int reset_time</code>
</li>
<li>
<b>Field removed. </b>
<code>spinlock_t lock</code>
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
