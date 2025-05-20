# Struct: <code>thread_info</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct thread_info {
    struct task_struct *task;
    __u32 flags;
    __u32 status;
    __u32 cpu;
    mm_segment_t addr_limit;
    unsigned int sig_on_uaccess_error;
    unsigned int uaccess_err;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct thread_info {
    struct task_struct *task;
    __u32 flags;
    __u32 status;
    __u32 cpu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct thread_info {
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct thread_info {
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct thread_info {
    long unsigned int flags;
    u32 status;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct thread_info {
    long unsigned int flags;
    u32 status;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct thread_info {
    long unsigned int flags;
    u32 status;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct thread_info {
    long unsigned int flags;
    u32 status;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct thread_info {
    long unsigned int flags;
    u32 status;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct thread_info {
    long unsigned int flags;
    u32 status;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct thread_info {
    long unsigned int flags;
    long unsigned int syscall_work;
    u32 status;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct thread_info {
    long unsigned int flags;
    long unsigned int syscall_work;
    u32 status;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct thread_info {
    long unsigned int flags;
    long unsigned int syscall_work;
    u32 status;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct thread_info {
    long unsigned int flags;
    long unsigned int syscall_work;
    u32 status;
    u32 cpu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct thread_info {
    long unsigned int flags;
    long unsigned int syscall_work;
    u32 status;
    u32 cpu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct thread_info {
    long unsigned int flags;
    long unsigned int syscall_work;
    u32 status;
    u32 cpu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct thread_info {
    long unsigned int flags;
    long unsigned int syscall_work;
    u32 status;
    u32 cpu;
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
struct thread_info {
    long unsigned int flags;
    mm_segment_t addr_limit;
    u64 ttbr0;
    u64 preempt_count;
    struct (anon) preempt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct thread_info {
    long unsigned int flags;
    int preempt_count;
    mm_segment_t addr_limit;
    struct task_struct *task;
    __u32 cpu;
    __u32 cpu_domain;
    struct cpu_context_save cpu_context;
    __u32 syscall;
    __u8 used_cp[16];
    long unsigned int tp_value[2];
    union fp_state fpstate;
    union vfp_state vfpstate;
    long unsigned int thumbee_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct thread_info {
    int preempt_count;
    long unsigned int local_flags;
    long unsigned int *livepatch_sp;
    unsigned char slb_preload_nr;
    unsigned char slb_preload_tail;
    u32 slb_preload_esid[16];
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct thread_info {
    long unsigned int flags;
    int preempt_count;
    mm_segment_t addr_limit;
    long int kernel_sp;
    long int user_sp;
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
struct thread_info {
    long unsigned int flags;
    u32 status;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct thread_info {
    long unsigned int flags;
    u32 status;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct thread_info {
    long unsigned int flags;
    u32 status;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct thread_info {
    long unsigned int flags;
    u32 status;
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
<b>Field removed. </b>
<code>mm_segment_t addr_limit</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int sig_on_uaccess_error</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int uaccess_err</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct task_struct *task</code>
</li>
<li>
<b>Field removed. </b>
<code>__u32 status</code>
</li>
<li>
<b>Field removed. </b>
<code>__u32 cpu</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u32 flags</code> ➡️ <code>long unsigned int flags</code>
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
<code>u32 status</code>
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
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int syscall_work</code>
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
<b>Field added. </b>
<code>u32 cpu</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>arm64</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>mm_segment_t addr_limit</code>
</li>
<li>
<b>Field added. </b>
<code>u64 ttbr0</code>
</li>
<li>
<b>Field added. </b>
<code>u64 preempt_count</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) preempt</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 status</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int preempt_count</code>
</li>
<li>
<b>Field added. </b>
<code>mm_segment_t addr_limit</code>
</li>
<li>
<b>Field added. </b>
<code>struct task_struct *task</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 cpu</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 cpu_domain</code>
</li>
<li>
<b>Field added. </b>
<code>struct cpu_context_save cpu_context</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 syscall</code>
</li>
<li>
<b>Field added. </b>
<code>__u8 used_cp[16]</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int tp_value[2]</code>
</li>
<li>
<b>Field added. </b>
<code>union fp_state fpstate</code>
</li>
<li>
<b>Field added. </b>
<code>union vfp_state vfpstate</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int thumbee_state</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 status</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int preempt_count</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int local_flags</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int *livepatch_sp</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned char slb_preload_nr</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned char slb_preload_tail</code>
</li>
<li>
<b>Field added. </b>
<code>u32 slb_preload_esid[16]</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 status</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int preempt_count</code>
</li>
<li>
<b>Field added. </b>
<code>mm_segment_t addr_limit</code>
</li>
<li>
<b>Field added. </b>
<code>long int kernel_sp</code>
</li>
<li>
<b>Field added. </b>
<code>long int user_sp</code>
</li>
<li>
<b>Field added. </b>
<code>int cpu</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 status</code>
</li>
</ul>
</details>
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
