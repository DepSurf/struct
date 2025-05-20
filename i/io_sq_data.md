# Struct: <code>io_sq_data</code>

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
In <code>4.10</code>: Absent ⚠️
</li>
<li>
In <code>4.13</code>: Absent ⚠️
</li>
<li>
In <code>4.15</code>: Absent ⚠️
</li>
<li>
In <code>4.18</code>: Absent ⚠️
</li>
<li>
In <code>5.0</code>: Absent ⚠️
</li>
<li>
In <code>5.3</code>: Absent ⚠️
</li>
<li>
In <code>5.4</code>: Absent ⚠️
</li>
<li>
In <code>5.8</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct io_sq_data {
    refcount_t refs;
    struct mutex lock;
    struct list_head ctx_list;
    struct list_head ctx_new_list;
    struct mutex ctx_lock;
    struct task_struct *thread;
    struct wait_queue_head wait;
    unsigned int sq_thread_idle;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct io_sq_data {
    refcount_t refs;
    atomic_t park_pending;
    struct mutex lock;
    struct list_head ctx_list;
    struct task_struct *thread;
    struct wait_queue_head wait;
    unsigned int sq_thread_idle;
    int sq_cpu;
    pid_t task_pid;
    pid_t task_tgid;
    long unsigned int state;
    struct completion exited;
    struct callback_head *park_task_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct io_sq_data {
    refcount_t refs;
    atomic_t park_pending;
    struct mutex lock;
    struct list_head ctx_list;
    struct task_struct *thread;
    struct wait_queue_head wait;
    unsigned int sq_thread_idle;
    int sq_cpu;
    pid_t task_pid;
    pid_t task_tgid;
    long unsigned int state;
    struct completion exited;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct io_sq_data {
    refcount_t refs;
    atomic_t park_pending;
    struct mutex lock;
    struct list_head ctx_list;
    struct task_struct *thread;
    struct wait_queue_head wait;
    unsigned int sq_thread_idle;
    int sq_cpu;
    pid_t task_pid;
    pid_t task_tgid;
    long unsigned int state;
    struct completion exited;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct io_sq_data {
    refcount_t refs;
    atomic_t park_pending;
    struct mutex lock;
    struct list_head ctx_list;
    struct task_struct *thread;
    struct wait_queue_head wait;
    unsigned int sq_thread_idle;
    int sq_cpu;
    pid_t task_pid;
    pid_t task_tgid;
    long unsigned int state;
    struct completion exited;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct io_sq_data {
    refcount_t refs;
    atomic_t park_pending;
    struct mutex lock;
    struct list_head ctx_list;
    struct task_struct *thread;
    struct wait_queue_head wait;
    unsigned int sq_thread_idle;
    int sq_cpu;
    pid_t task_pid;
    pid_t task_tgid;
    long unsigned int state;
    struct completion exited;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct io_sq_data {
    refcount_t refs;
    atomic_t park_pending;
    struct mutex lock;
    struct list_head ctx_list;
    struct task_struct *thread;
    struct wait_queue_head wait;
    unsigned int sq_thread_idle;
    int sq_cpu;
    pid_t task_pid;
    pid_t task_tgid;
    long unsigned int state;
    struct completion exited;
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
In <code>arm64</code>: Absent ⚠️
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
</li>
<li>
In <code>riscv64</code>: Absent ⚠️
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
In <code>aws</code>: Absent ⚠️
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>atomic_t park_pending</code>
</li>
<li>
<b>Field added. </b>
<code>int sq_cpu</code>
</li>
<li>
<b>Field added. </b>
<code>pid_t task_pid</code>
</li>
<li>
<b>Field added. </b>
<code>pid_t task_tgid</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int state</code>
</li>
<li>
<b>Field added. </b>
<code>struct completion exited</code>
</li>
<li>
<b>Field added. </b>
<code>struct callback_head *park_task_work</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head ctx_new_list</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mutex ctx_lock</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct callback_head *park_task_work</code>
</li>
</ul>
</details>
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
