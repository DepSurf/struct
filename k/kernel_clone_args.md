# Struct: <code>kernel_clone_args</code>

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
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct kernel_clone_args {
    u64 flags;
    int *pidfd;
    int *child_tid;
    int *parent_tid;
    int exit_signal;
    long unsigned int stack;
    long unsigned int stack_size;
    long unsigned int tls;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct kernel_clone_args {
    u64 flags;
    int *pidfd;
    int *child_tid;
    int *parent_tid;
    int exit_signal;
    long unsigned int stack;
    long unsigned int stack_size;
    long unsigned int tls;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct kernel_clone_args {
    u64 flags;
    int *pidfd;
    int *child_tid;
    int *parent_tid;
    int exit_signal;
    long unsigned int stack;
    long unsigned int stack_size;
    long unsigned int tls;
    pid_t *set_tid;
    size_t set_tid_size;
    int cgroup;
    struct cgroup *cgrp;
    struct css_set *cset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct kernel_clone_args {
    u64 flags;
    int *pidfd;
    int *child_tid;
    int *parent_tid;
    int exit_signal;
    long unsigned int stack;
    long unsigned int stack_size;
    long unsigned int tls;
    pid_t *set_tid;
    size_t set_tid_size;
    int cgroup;
    struct cgroup *cgrp;
    struct css_set *cset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kernel_clone_args {
    u64 flags;
    int *pidfd;
    int *child_tid;
    int *parent_tid;
    int exit_signal;
    long unsigned int stack;
    long unsigned int stack_size;
    long unsigned int tls;
    pid_t *set_tid;
    size_t set_tid_size;
    int cgroup;
    int io_thread;
    struct cgroup *cgrp;
    struct css_set *cset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kernel_clone_args {
    u64 flags;
    int *pidfd;
    int *child_tid;
    int *parent_tid;
    int exit_signal;
    long unsigned int stack;
    long unsigned int stack_size;
    long unsigned int tls;
    pid_t *set_tid;
    size_t set_tid_size;
    int cgroup;
    int io_thread;
    struct cgroup *cgrp;
    struct css_set *cset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kernel_clone_args {
    u64 flags;
    int *pidfd;
    int *child_tid;
    int *parent_tid;
    int exit_signal;
    long unsigned int stack;
    long unsigned int stack_size;
    long unsigned int tls;
    pid_t *set_tid;
    size_t set_tid_size;
    int cgroup;
    int io_thread;
    int kthread;
    int idle;
    int (*fn)(void *);
    void *fn_arg;
    struct cgroup *cgrp;
    struct css_set *cset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kernel_clone_args {
    u64 flags;
    int *pidfd;
    int *child_tid;
    int *parent_tid;
    int exit_signal;
    long unsigned int stack;
    long unsigned int stack_size;
    long unsigned int tls;
    pid_t *set_tid;
    size_t set_tid_size;
    int cgroup;
    int io_thread;
    int kthread;
    int idle;
    int (*fn)(void *);
    void *fn_arg;
    struct cgroup *cgrp;
    struct css_set *cset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kernel_clone_args {
    u64 flags;
    int *pidfd;
    int *child_tid;
    int *parent_tid;
    const char *name;
    int exit_signal;
    u32 kthread;
    u32 io_thread;
    u32 user_worker;
    u32 no_files;
    long unsigned int stack;
    long unsigned int stack_size;
    long unsigned int tls;
    pid_t *set_tid;
    size_t set_tid_size;
    int cgroup;
    int idle;
    int (*fn)(void *);
    void *fn_arg;
    struct cgroup *cgrp;
    struct css_set *cset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kernel_clone_args {
    u64 flags;
    int *pidfd;
    int *child_tid;
    int *parent_tid;
    const char *name;
    int exit_signal;
    u32 kthread;
    u32 io_thread;
    u32 user_worker;
    u32 no_files;
    long unsigned int stack;
    long unsigned int stack_size;
    long unsigned int tls;
    pid_t *set_tid;
    size_t set_tid_size;
    int cgroup;
    int idle;
    int (*fn)(void *);
    void *fn_arg;
    struct cgroup *cgrp;
    struct css_set *cset;
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
struct kernel_clone_args {
    u64 flags;
    int *pidfd;
    int *child_tid;
    int *parent_tid;
    int exit_signal;
    long unsigned int stack;
    long unsigned int stack_size;
    long unsigned int tls;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct kernel_clone_args {
    u64 flags;
    int *pidfd;
    int *child_tid;
    int *parent_tid;
    int exit_signal;
    long unsigned int stack;
    long unsigned int stack_size;
    long unsigned int tls;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct kernel_clone_args {
    u64 flags;
    int *pidfd;
    int *child_tid;
    int *parent_tid;
    int exit_signal;
    long unsigned int stack;
    long unsigned int stack_size;
    long unsigned int tls;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct kernel_clone_args {
    u64 flags;
    int *pidfd;
    int *child_tid;
    int *parent_tid;
    int exit_signal;
    long unsigned int stack;
    long unsigned int stack_size;
    long unsigned int tls;
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
struct kernel_clone_args {
    u64 flags;
    int *pidfd;
    int *child_tid;
    int *parent_tid;
    int exit_signal;
    long unsigned int stack;
    long unsigned int stack_size;
    long unsigned int tls;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct kernel_clone_args {
    u64 flags;
    int *pidfd;
    int *child_tid;
    int *parent_tid;
    int exit_signal;
    long unsigned int stack;
    long unsigned int stack_size;
    long unsigned int tls;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct kernel_clone_args {
    u64 flags;
    int *pidfd;
    int *child_tid;
    int *parent_tid;
    int exit_signal;
    long unsigned int stack;
    long unsigned int stack_size;
    long unsigned int tls;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct kernel_clone_args {
    u64 flags;
    int *pidfd;
    int *child_tid;
    int *parent_tid;
    int exit_signal;
    long unsigned int stack;
    long unsigned int stack_size;
    long unsigned int tls;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>pid_t *set_tid</code>
</li>
<li>
<b>Field added. </b>
<code>size_t set_tid_size</code>
</li>
<li>
<b>Field added. </b>
<code>int cgroup</code>
</li>
<li>
<b>Field added. </b>
<code>struct cgroup *cgrp</code>
</li>
<li>
<b>Field added. </b>
<code>struct css_set *cset</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int io_thread</code>
</li>
</ul>
</details>
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
<code>int kthread</code>
</li>
<li>
<b>Field added. </b>
<code>int idle</code>
</li>
<li>
<b>Field added. </b>
<code>int (*fn)(void *)</code>
</li>
<li>
<b>Field added. </b>
<code>void *fn_arg</code>
</li>
</ul>
</details>
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
<code>const char *name</code>
</li>
<li>
<b>Field added. </b>
<code>u32 user_worker</code>
</li>
<li>
<b>Field added. </b>
<code>u32 no_files</code>
</li>
<li>
<b>Field type changed. </b>
<code>int io_thread</code> ➡️ <code>u32 io_thread</code>
</li>
<li>
<b>Field type changed. </b>
<code>int kthread</code> ➡️ <code>u32 kthread</code>
</li>
</ul>
</details>
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
