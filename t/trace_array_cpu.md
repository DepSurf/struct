# Struct: <code>trace_array_cpu</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct trace_array_cpu {
    atomic_t disabled;
    void *buffer_page;
    long unsigned int entries;
    long unsigned int saved_latency;
    long unsigned int critical_start;
    long unsigned int critical_end;
    long unsigned int critical_sequence;
    long unsigned int nice;
    long unsigned int policy;
    long unsigned int rt_priority;
    long unsigned int skipped_entries;
    cycle_t preempt_timestamp;
    pid_t pid;
    kuid_t uid;
    char comm[16];
    bool ignore_pid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct trace_array_cpu {
    atomic_t disabled;
    void *buffer_page;
    long unsigned int entries;
    long unsigned int saved_latency;
    long unsigned int critical_start;
    long unsigned int critical_end;
    long unsigned int critical_sequence;
    long unsigned int nice;
    long unsigned int policy;
    long unsigned int rt_priority;
    long unsigned int skipped_entries;
    cycle_t preempt_timestamp;
    pid_t pid;
    kuid_t uid;
    char comm[16];
    bool ignore_pid;
    bool ftrace_ignore_pid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct trace_array_cpu {
    atomic_t disabled;
    void *buffer_page;
    long unsigned int entries;
    long unsigned int saved_latency;
    long unsigned int critical_start;
    long unsigned int critical_end;
    long unsigned int critical_sequence;
    long unsigned int nice;
    long unsigned int policy;
    long unsigned int rt_priority;
    long unsigned int skipped_entries;
    u64 preempt_timestamp;
    pid_t pid;
    kuid_t uid;
    char comm[16];
    bool ignore_pid;
    bool ftrace_ignore_pid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct trace_array_cpu {
    atomic_t disabled;
    void *buffer_page;
    long unsigned int entries;
    long unsigned int saved_latency;
    long unsigned int critical_start;
    long unsigned int critical_end;
    long unsigned int critical_sequence;
    long unsigned int nice;
    long unsigned int policy;
    long unsigned int rt_priority;
    long unsigned int skipped_entries;
    u64 preempt_timestamp;
    pid_t pid;
    kuid_t uid;
    char comm[16];
    bool ignore_pid;
    bool ftrace_ignore_pid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct trace_array_cpu {
    atomic_t disabled;
    void *buffer_page;
    long unsigned int entries;
    long unsigned int saved_latency;
    long unsigned int critical_start;
    long unsigned int critical_end;
    long unsigned int critical_sequence;
    long unsigned int nice;
    long unsigned int policy;
    long unsigned int rt_priority;
    long unsigned int skipped_entries;
    u64 preempt_timestamp;
    pid_t pid;
    kuid_t uid;
    char comm[16];
    bool ignore_pid;
    bool ftrace_ignore_pid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct trace_array_cpu {
    atomic_t disabled;
    void *buffer_page;
    long unsigned int entries;
    long unsigned int saved_latency;
    long unsigned int critical_start;
    long unsigned int critical_end;
    long unsigned int critical_sequence;
    long unsigned int nice;
    long unsigned int policy;
    long unsigned int rt_priority;
    long unsigned int skipped_entries;
    u64 preempt_timestamp;
    pid_t pid;
    kuid_t uid;
    char comm[16];
    bool ignore_pid;
    bool ftrace_ignore_pid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct trace_array_cpu {
    atomic_t disabled;
    void *buffer_page;
    long unsigned int entries;
    long unsigned int saved_latency;
    long unsigned int critical_start;
    long unsigned int critical_end;
    long unsigned int critical_sequence;
    long unsigned int nice;
    long unsigned int policy;
    long unsigned int rt_priority;
    long unsigned int skipped_entries;
    u64 preempt_timestamp;
    pid_t pid;
    kuid_t uid;
    char comm[16];
    bool ignore_pid;
    bool ftrace_ignore_pid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct trace_array_cpu {
    atomic_t disabled;
    void *buffer_page;
    long unsigned int entries;
    long unsigned int saved_latency;
    long unsigned int critical_start;
    long unsigned int critical_end;
    long unsigned int critical_sequence;
    long unsigned int nice;
    long unsigned int policy;
    long unsigned int rt_priority;
    long unsigned int skipped_entries;
    u64 preempt_timestamp;
    pid_t pid;
    kuid_t uid;
    char comm[16];
    bool ignore_pid;
    bool ftrace_ignore_pid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct trace_array_cpu {
    atomic_t disabled;
    void *buffer_page;
    long unsigned int entries;
    long unsigned int saved_latency;
    long unsigned int critical_start;
    long unsigned int critical_end;
    long unsigned int critical_sequence;
    long unsigned int nice;
    long unsigned int policy;
    long unsigned int rt_priority;
    long unsigned int skipped_entries;
    u64 preempt_timestamp;
    pid_t pid;
    kuid_t uid;
    char comm[16];
    bool ignore_pid;
    bool ftrace_ignore_pid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct trace_array_cpu {
    atomic_t disabled;
    void *buffer_page;
    long unsigned int entries;
    long unsigned int saved_latency;
    long unsigned int critical_start;
    long unsigned int critical_end;
    long unsigned int critical_sequence;
    long unsigned int nice;
    long unsigned int policy;
    long unsigned int rt_priority;
    long unsigned int skipped_entries;
    u64 preempt_timestamp;
    pid_t pid;
    kuid_t uid;
    char comm[16];
    int ftrace_ignore_pid;
    bool ignore_pid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct trace_array_cpu {
    atomic_t disabled;
    void *buffer_page;
    long unsigned int entries;
    long unsigned int saved_latency;
    long unsigned int critical_start;
    long unsigned int critical_end;
    long unsigned int critical_sequence;
    long unsigned int nice;
    long unsigned int policy;
    long unsigned int rt_priority;
    long unsigned int skipped_entries;
    u64 preempt_timestamp;
    pid_t pid;
    kuid_t uid;
    char comm[16];
    int ftrace_ignore_pid;
    bool ignore_pid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct trace_array_cpu {
    atomic_t disabled;
    void *buffer_page;
    long unsigned int entries;
    long unsigned int saved_latency;
    long unsigned int critical_start;
    long unsigned int critical_end;
    long unsigned int critical_sequence;
    long unsigned int nice;
    long unsigned int policy;
    long unsigned int rt_priority;
    long unsigned int skipped_entries;
    u64 preempt_timestamp;
    pid_t pid;
    kuid_t uid;
    char comm[16];
    int ftrace_ignore_pid;
    bool ignore_pid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct trace_array_cpu {
    atomic_t disabled;
    void *buffer_page;
    long unsigned int entries;
    long unsigned int saved_latency;
    long unsigned int critical_start;
    long unsigned int critical_end;
    long unsigned int critical_sequence;
    long unsigned int nice;
    long unsigned int policy;
    long unsigned int rt_priority;
    long unsigned int skipped_entries;
    u64 preempt_timestamp;
    pid_t pid;
    kuid_t uid;
    char comm[16];
    int ftrace_ignore_pid;
    bool ignore_pid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct trace_array_cpu {
    atomic_t disabled;
    void *buffer_page;
    long unsigned int entries;
    long unsigned int saved_latency;
    long unsigned int critical_start;
    long unsigned int critical_end;
    long unsigned int critical_sequence;
    long unsigned int nice;
    long unsigned int policy;
    long unsigned int rt_priority;
    long unsigned int skipped_entries;
    u64 preempt_timestamp;
    pid_t pid;
    kuid_t uid;
    char comm[16];
    int ftrace_ignore_pid;
    bool ignore_pid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct trace_array_cpu {
    atomic_t disabled;
    void *buffer_page;
    long unsigned int entries;
    long unsigned int saved_latency;
    long unsigned int critical_start;
    long unsigned int critical_end;
    long unsigned int critical_sequence;
    long unsigned int nice;
    long unsigned int policy;
    long unsigned int rt_priority;
    long unsigned int skipped_entries;
    u64 preempt_timestamp;
    pid_t pid;
    kuid_t uid;
    char comm[16];
    int ftrace_ignore_pid;
    bool ignore_pid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct trace_array_cpu {
    atomic_t disabled;
    void *buffer_page;
    long unsigned int entries;
    long unsigned int saved_latency;
    long unsigned int critical_start;
    long unsigned int critical_end;
    long unsigned int critical_sequence;
    long unsigned int nice;
    long unsigned int policy;
    long unsigned int rt_priority;
    long unsigned int skipped_entries;
    u64 preempt_timestamp;
    pid_t pid;
    kuid_t uid;
    char comm[16];
    int ftrace_ignore_pid;
    bool ignore_pid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct trace_array_cpu {
    atomic_t disabled;
    void *buffer_page;
    long unsigned int entries;
    long unsigned int saved_latency;
    long unsigned int critical_start;
    long unsigned int critical_end;
    long unsigned int critical_sequence;
    long unsigned int nice;
    long unsigned int policy;
    long unsigned int rt_priority;
    long unsigned int skipped_entries;
    u64 preempt_timestamp;
    pid_t pid;
    kuid_t uid;
    char comm[16];
    int ftrace_ignore_pid;
    bool ignore_pid;
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
struct trace_array_cpu {
    atomic_t disabled;
    void *buffer_page;
    long unsigned int entries;
    long unsigned int saved_latency;
    long unsigned int critical_start;
    long unsigned int critical_end;
    long unsigned int critical_sequence;
    long unsigned int nice;
    long unsigned int policy;
    long unsigned int rt_priority;
    long unsigned int skipped_entries;
    u64 preempt_timestamp;
    pid_t pid;
    kuid_t uid;
    char comm[16];
    bool ignore_pid;
    bool ftrace_ignore_pid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct trace_array_cpu {
    atomic_t disabled;
    void *buffer_page;
    long unsigned int entries;
    long unsigned int saved_latency;
    long unsigned int critical_start;
    long unsigned int critical_end;
    long unsigned int critical_sequence;
    long unsigned int nice;
    long unsigned int policy;
    long unsigned int rt_priority;
    long unsigned int skipped_entries;
    u64 preempt_timestamp;
    pid_t pid;
    kuid_t uid;
    char comm[16];
    bool ignore_pid;
    bool ftrace_ignore_pid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct trace_array_cpu {
    atomic_t disabled;
    void *buffer_page;
    long unsigned int entries;
    long unsigned int saved_latency;
    long unsigned int critical_start;
    long unsigned int critical_end;
    long unsigned int critical_sequence;
    long unsigned int nice;
    long unsigned int policy;
    long unsigned int rt_priority;
    long unsigned int skipped_entries;
    u64 preempt_timestamp;
    pid_t pid;
    kuid_t uid;
    char comm[16];
    bool ignore_pid;
    bool ftrace_ignore_pid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct trace_array_cpu {
    atomic_t disabled;
    void *buffer_page;
    long unsigned int entries;
    long unsigned int saved_latency;
    long unsigned int critical_start;
    long unsigned int critical_end;
    long unsigned int critical_sequence;
    long unsigned int nice;
    long unsigned int policy;
    long unsigned int rt_priority;
    long unsigned int skipped_entries;
    u64 preempt_timestamp;
    pid_t pid;
    kuid_t uid;
    char comm[16];
    bool ignore_pid;
    bool ftrace_ignore_pid;
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
struct trace_array_cpu {
    atomic_t disabled;
    void *buffer_page;
    long unsigned int entries;
    long unsigned int saved_latency;
    long unsigned int critical_start;
    long unsigned int critical_end;
    long unsigned int critical_sequence;
    long unsigned int nice;
    long unsigned int policy;
    long unsigned int rt_priority;
    long unsigned int skipped_entries;
    u64 preempt_timestamp;
    pid_t pid;
    kuid_t uid;
    char comm[16];
    bool ignore_pid;
    bool ftrace_ignore_pid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct trace_array_cpu {
    atomic_t disabled;
    void *buffer_page;
    long unsigned int entries;
    long unsigned int saved_latency;
    long unsigned int critical_start;
    long unsigned int critical_end;
    long unsigned int critical_sequence;
    long unsigned int nice;
    long unsigned int policy;
    long unsigned int rt_priority;
    long unsigned int skipped_entries;
    u64 preempt_timestamp;
    pid_t pid;
    kuid_t uid;
    char comm[16];
    bool ignore_pid;
    bool ftrace_ignore_pid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct trace_array_cpu {
    atomic_t disabled;
    void *buffer_page;
    long unsigned int entries;
    long unsigned int saved_latency;
    long unsigned int critical_start;
    long unsigned int critical_end;
    long unsigned int critical_sequence;
    long unsigned int nice;
    long unsigned int policy;
    long unsigned int rt_priority;
    long unsigned int skipped_entries;
    u64 preempt_timestamp;
    pid_t pid;
    kuid_t uid;
    char comm[16];
    bool ignore_pid;
    bool ftrace_ignore_pid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct trace_array_cpu {
    atomic_t disabled;
    void *buffer_page;
    long unsigned int entries;
    long unsigned int saved_latency;
    long unsigned int critical_start;
    long unsigned int critical_end;
    long unsigned int critical_sequence;
    long unsigned int nice;
    long unsigned int policy;
    long unsigned int rt_priority;
    long unsigned int skipped_entries;
    u64 preempt_timestamp;
    pid_t pid;
    kuid_t uid;
    char comm[16];
    bool ignore_pid;
    bool ftrace_ignore_pid;
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
<code>bool ftrace_ignore_pid</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>cycle_t preempt_timestamp</code> ➡️ <code>u64 preempt_timestamp</code>
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
<b>Field type changed. </b>
<code>bool ftrace_ignore_pid</code> ➡️ <code>int ftrace_ignore_pid</code>
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
