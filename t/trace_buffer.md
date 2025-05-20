# Struct: <code>trace_buffer</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct trace_buffer {
    struct trace_array *tr;
    struct ring_buffer *buffer;
    struct trace_array_cpu *data;
    cycle_t time_start;
    int cpu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct trace_buffer {
    struct trace_array *tr;
    struct ring_buffer *buffer;
    struct trace_array_cpu *data;
    cycle_t time_start;
    int cpu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct trace_buffer {
    struct trace_array *tr;
    struct ring_buffer *buffer;
    struct trace_array_cpu *data;
    u64 time_start;
    int cpu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct trace_buffer {
    struct trace_array *tr;
    struct ring_buffer *buffer;
    struct trace_array_cpu *data;
    u64 time_start;
    int cpu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct trace_buffer {
    struct trace_array *tr;
    struct ring_buffer *buffer;
    struct trace_array_cpu *data;
    u64 time_start;
    int cpu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct trace_buffer {
    struct trace_array *tr;
    struct ring_buffer *buffer;
    struct trace_array_cpu *data;
    u64 time_start;
    int cpu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct trace_buffer {
    struct trace_array *tr;
    struct ring_buffer *buffer;
    struct trace_array_cpu *data;
    u64 time_start;
    int cpu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct trace_buffer {
    struct trace_array *tr;
    struct ring_buffer *buffer;
    struct trace_array_cpu *data;
    u64 time_start;
    int cpu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct trace_buffer {
    struct trace_array *tr;
    struct ring_buffer *buffer;
    struct trace_array_cpu *data;
    u64 time_start;
    int cpu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct trace_buffer {
    unsigned int flags;
    int cpus;
    atomic_t record_disabled;
    cpumask_var_t cpumask;
    struct lock_class_key *reader_lock_key;
    struct mutex mutex;
    struct ring_buffer_per_cpu **buffers;
    struct hlist_node node;
    u64 (*clock)();
    struct rb_irq_work irq_work;
    bool time_stamp_abs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct trace_buffer {
    unsigned int flags;
    int cpus;
    atomic_t record_disabled;
    cpumask_var_t cpumask;
    struct lock_class_key *reader_lock_key;
    struct mutex mutex;
    struct ring_buffer_per_cpu **buffers;
    struct hlist_node node;
    u64 (*clock)();
    struct rb_irq_work irq_work;
    bool time_stamp_abs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct trace_buffer {
    unsigned int flags;
    int cpus;
    atomic_t record_disabled;
    cpumask_var_t cpumask;
    struct lock_class_key *reader_lock_key;
    struct mutex mutex;
    struct ring_buffer_per_cpu **buffers;
    struct hlist_node node;
    u64 (*clock)();
    struct rb_irq_work irq_work;
    bool time_stamp_abs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct trace_buffer {
    unsigned int flags;
    int cpus;
    atomic_t record_disabled;
    cpumask_var_t cpumask;
    struct lock_class_key *reader_lock_key;
    struct mutex mutex;
    struct ring_buffer_per_cpu **buffers;
    struct hlist_node node;
    u64 (*clock)();
    struct rb_irq_work irq_work;
    bool time_stamp_abs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct trace_buffer {
    unsigned int flags;
    int cpus;
    atomic_t record_disabled;
    cpumask_var_t cpumask;
    struct lock_class_key *reader_lock_key;
    struct mutex mutex;
    struct ring_buffer_per_cpu **buffers;
    struct hlist_node node;
    u64 (*clock)();
    struct rb_irq_work irq_work;
    bool time_stamp_abs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct trace_buffer {
    unsigned int flags;
    int cpus;
    atomic_t record_disabled;
    cpumask_var_t cpumask;
    struct lock_class_key *reader_lock_key;
    struct mutex mutex;
    struct ring_buffer_per_cpu **buffers;
    struct hlist_node node;
    u64 (*clock)();
    struct rb_irq_work irq_work;
    bool time_stamp_abs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct trace_buffer {
    unsigned int flags;
    int cpus;
    atomic_t record_disabled;
    atomic_t resizing;
    cpumask_var_t cpumask;
    struct lock_class_key *reader_lock_key;
    struct mutex mutex;
    struct ring_buffer_per_cpu **buffers;
    struct hlist_node node;
    u64 (*clock)();
    struct rb_irq_work irq_work;
    bool time_stamp_abs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct trace_buffer {
    unsigned int flags;
    int cpus;
    atomic_t record_disabled;
    atomic_t resizing;
    cpumask_var_t cpumask;
    struct lock_class_key *reader_lock_key;
    struct mutex mutex;
    struct ring_buffer_per_cpu **buffers;
    struct hlist_node node;
    u64 (*clock)();
    struct rb_irq_work irq_work;
    bool time_stamp_abs;
    unsigned int subbuf_size;
    unsigned int subbuf_order;
    unsigned int max_data_size;
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
struct trace_buffer {
    struct trace_array *tr;
    struct ring_buffer *buffer;
    struct trace_array_cpu *data;
    u64 time_start;
    int cpu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct trace_buffer {
    struct trace_array *tr;
    struct ring_buffer *buffer;
    struct trace_array_cpu *data;
    u64 time_start;
    int cpu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct trace_buffer {
    struct trace_array *tr;
    struct ring_buffer *buffer;
    struct trace_array_cpu *data;
    u64 time_start;
    int cpu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct trace_buffer {
    struct trace_array *tr;
    struct ring_buffer *buffer;
    struct trace_array_cpu *data;
    u64 time_start;
    int cpu;
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
struct trace_buffer {
    struct trace_array *tr;
    struct ring_buffer *buffer;
    struct trace_array_cpu *data;
    u64 time_start;
    int cpu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct trace_buffer {
    struct trace_array *tr;
    struct ring_buffer *buffer;
    struct trace_array_cpu *data;
    u64 time_start;
    int cpu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct trace_buffer {
    struct trace_array *tr;
    struct ring_buffer *buffer;
    struct trace_array_cpu *data;
    u64 time_start;
    int cpu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct trace_buffer {
    struct trace_array *tr;
    struct ring_buffer *buffer;
    struct trace_array_cpu *data;
    u64 time_start;
    int cpu;
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
<b>Field type changed. </b>
<code>cycle_t time_start</code> ➡️ <code>u64 time_start</code>
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
<code>unsigned int flags</code>
</li>
<li>
<b>Field added. </b>
<code>int cpus</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t record_disabled</code>
</li>
<li>
<b>Field added. </b>
<code>cpumask_var_t cpumask</code>
</li>
<li>
<b>Field added. </b>
<code>struct lock_class_key *reader_lock_key</code>
</li>
<li>
<b>Field added. </b>
<code>struct mutex mutex</code>
</li>
<li>
<b>Field added. </b>
<code>struct ring_buffer_per_cpu **buffers</code>
</li>
<li>
<b>Field added. </b>
<code>struct hlist_node node</code>
</li>
<li>
<b>Field added. </b>
<code>u64 (*clock)()</code>
</li>
<li>
<b>Field added. </b>
<code>struct rb_irq_work irq_work</code>
</li>
<li>
<b>Field added. </b>
<code>bool time_stamp_abs</code>
</li>
<li>
<b>Field removed. </b>
<code>struct trace_array *tr</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ring_buffer *buffer</code>
</li>
<li>
<b>Field removed. </b>
<code>struct trace_array_cpu *data</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 time_start</code>
</li>
<li>
<b>Field removed. </b>
<code>int cpu</code>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>atomic_t resizing</code>
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
<code>unsigned int subbuf_size</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int subbuf_order</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int max_data_size</code>
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
