# Struct: <code>trace_pid_list</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct trace_pid_list {
    unsigned int nr_pids;
    int order;
    pid_t *pids;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct trace_pid_list {
    int pid_max;
    long unsigned int *pids;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct trace_pid_list {
    int pid_max;
    long unsigned int *pids;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct trace_pid_list {
    int pid_max;
    long unsigned int *pids;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct trace_pid_list {
    int pid_max;
    long unsigned int *pids;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct trace_pid_list {
    int pid_max;
    long unsigned int *pids;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct trace_pid_list {
    int pid_max;
    long unsigned int *pids;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct trace_pid_list {
    int pid_max;
    long unsigned int *pids;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct trace_pid_list {
    int pid_max;
    long unsigned int *pids;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct trace_pid_list {
    int pid_max;
    long unsigned int *pids;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct trace_pid_list {
    int pid_max;
    long unsigned int *pids;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct trace_pid_list {
    int pid_max;
    long unsigned int *pids;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct trace_pid_list {
    int pid_max;
    long unsigned int *pids;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct trace_pid_list {
    raw_spinlock_t lock;
    struct irq_work refill_irqwork;
    union upper_chunk * upper[256];
    union upper_chunk *upper_list;
    union lower_chunk *lower_list;
    int free_upper_chunks;
    int free_lower_chunks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct trace_pid_list {
    raw_spinlock_t lock;
    struct irq_work refill_irqwork;
    union upper_chunk * upper[256];
    union upper_chunk *upper_list;
    union lower_chunk *lower_list;
    int free_upper_chunks;
    int free_lower_chunks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct trace_pid_list {
    raw_spinlock_t lock;
    struct irq_work refill_irqwork;
    union upper_chunk * upper[256];
    union upper_chunk *upper_list;
    union lower_chunk *lower_list;
    int free_upper_chunks;
    int free_lower_chunks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct trace_pid_list {
    raw_spinlock_t lock;
    struct irq_work refill_irqwork;
    union upper_chunk * upper[256];
    union upper_chunk *upper_list;
    union lower_chunk *lower_list;
    int free_upper_chunks;
    int free_lower_chunks;
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
struct trace_pid_list {
    int pid_max;
    long unsigned int *pids;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct trace_pid_list {
    int pid_max;
    long unsigned int *pids;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct trace_pid_list {
    int pid_max;
    long unsigned int *pids;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct trace_pid_list {
    int pid_max;
    long unsigned int *pids;
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
struct trace_pid_list {
    int pid_max;
    long unsigned int *pids;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct trace_pid_list {
    int pid_max;
    long unsigned int *pids;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct trace_pid_list {
    int pid_max;
    long unsigned int *pids;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct trace_pid_list {
    int pid_max;
    long unsigned int *pids;
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
<code>int pid_max</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int nr_pids</code>
</li>
<li>
<b>Field removed. </b>
<code>int order</code>
</li>
<li>
<b>Field type changed. </b>
<code>pid_t *pids</code> ➡️ <code>long unsigned int *pids</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>raw_spinlock_t lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct irq_work refill_irqwork</code>
</li>
<li>
<b>Field added. </b>
<code>union upper_chunk * upper[256]</code>
</li>
<li>
<b>Field added. </b>
<code>union upper_chunk *upper_list</code>
</li>
<li>
<b>Field added. </b>
<code>union lower_chunk *lower_list</code>
</li>
<li>
<b>Field added. </b>
<code>int free_upper_chunks</code>
</li>
<li>
<b>Field added. </b>
<code>int free_lower_chunks</code>
</li>
<li>
<b>Field removed. </b>
<code>int pid_max</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int *pids</code>
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
