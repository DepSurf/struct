# Struct: <code>elf_prstatus</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct elf_prstatus {
    struct elf_siginfo pr_info;
    short int pr_cursig;
    long unsigned int pr_sigpend;
    long unsigned int pr_sighold;
    pid_t pr_pid;
    pid_t pr_ppid;
    pid_t pr_pgrp;
    pid_t pr_sid;
    struct timeval pr_utime;
    struct timeval pr_stime;
    struct timeval pr_cutime;
    struct timeval pr_cstime;
    elf_gregset_t pr_reg;
    int pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct elf_prstatus {
    struct elf_siginfo pr_info;
    short int pr_cursig;
    long unsigned int pr_sigpend;
    long unsigned int pr_sighold;
    pid_t pr_pid;
    pid_t pr_ppid;
    pid_t pr_pgrp;
    pid_t pr_sid;
    struct timeval pr_utime;
    struct timeval pr_stime;
    struct timeval pr_cutime;
    struct timeval pr_cstime;
    elf_gregset_t pr_reg;
    int pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct elf_prstatus {
    struct elf_siginfo pr_info;
    short int pr_cursig;
    long unsigned int pr_sigpend;
    long unsigned int pr_sighold;
    pid_t pr_pid;
    pid_t pr_ppid;
    pid_t pr_pgrp;
    pid_t pr_sid;
    struct timeval pr_utime;
    struct timeval pr_stime;
    struct timeval pr_cutime;
    struct timeval pr_cstime;
    elf_gregset_t pr_reg;
    int pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct elf_prstatus {
    struct elf_siginfo pr_info;
    short int pr_cursig;
    long unsigned int pr_sigpend;
    long unsigned int pr_sighold;
    pid_t pr_pid;
    pid_t pr_ppid;
    pid_t pr_pgrp;
    pid_t pr_sid;
    struct timeval pr_utime;
    struct timeval pr_stime;
    struct timeval pr_cutime;
    struct timeval pr_cstime;
    elf_gregset_t pr_reg;
    int pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct elf_prstatus {
    struct elf_siginfo pr_info;
    short int pr_cursig;
    long unsigned int pr_sigpend;
    long unsigned int pr_sighold;
    pid_t pr_pid;
    pid_t pr_ppid;
    pid_t pr_pgrp;
    pid_t pr_sid;
    struct timeval pr_utime;
    struct timeval pr_stime;
    struct timeval pr_cutime;
    struct timeval pr_cstime;
    elf_gregset_t pr_reg;
    int pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct elf_prstatus {
    struct elf_siginfo pr_info;
    short int pr_cursig;
    long unsigned int pr_sigpend;
    long unsigned int pr_sighold;
    pid_t pr_pid;
    pid_t pr_ppid;
    pid_t pr_pgrp;
    pid_t pr_sid;
    struct timeval pr_utime;
    struct timeval pr_stime;
    struct timeval pr_cutime;
    struct timeval pr_cstime;
    elf_gregset_t pr_reg;
    int pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct elf_prstatus {
    struct elf_siginfo pr_info;
    short int pr_cursig;
    long unsigned int pr_sigpend;
    long unsigned int pr_sighold;
    pid_t pr_pid;
    pid_t pr_ppid;
    pid_t pr_pgrp;
    pid_t pr_sid;
    struct timeval pr_utime;
    struct timeval pr_stime;
    struct timeval pr_cutime;
    struct timeval pr_cstime;
    elf_gregset_t pr_reg;
    int pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct elf_prstatus {
    struct elf_siginfo pr_info;
    short int pr_cursig;
    long unsigned int pr_sigpend;
    long unsigned int pr_sighold;
    pid_t pr_pid;
    pid_t pr_ppid;
    pid_t pr_pgrp;
    pid_t pr_sid;
    struct timeval pr_utime;
    struct timeval pr_stime;
    struct timeval pr_cutime;
    struct timeval pr_cstime;
    elf_gregset_t pr_reg;
    int pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct elf_prstatus {
    struct elf_siginfo pr_info;
    short int pr_cursig;
    long unsigned int pr_sigpend;
    long unsigned int pr_sighold;
    pid_t pr_pid;
    pid_t pr_ppid;
    pid_t pr_pgrp;
    pid_t pr_sid;
    struct timeval pr_utime;
    struct timeval pr_stime;
    struct timeval pr_cutime;
    struct timeval pr_cstime;
    elf_gregset_t pr_reg;
    int pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct elf_prstatus {
    struct elf_siginfo pr_info;
    short int pr_cursig;
    long unsigned int pr_sigpend;
    long unsigned int pr_sighold;
    pid_t pr_pid;
    pid_t pr_ppid;
    pid_t pr_pgrp;
    pid_t pr_sid;
    struct __kernel_old_timeval pr_utime;
    struct __kernel_old_timeval pr_stime;
    struct __kernel_old_timeval pr_cutime;
    struct __kernel_old_timeval pr_cstime;
    elf_gregset_t pr_reg;
    int pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct elf_prstatus {
    struct elf_siginfo pr_info;
    short int pr_cursig;
    long unsigned int pr_sigpend;
    long unsigned int pr_sighold;
    pid_t pr_pid;
    pid_t pr_ppid;
    pid_t pr_pgrp;
    pid_t pr_sid;
    struct __kernel_old_timeval pr_utime;
    struct __kernel_old_timeval pr_stime;
    struct __kernel_old_timeval pr_cutime;
    struct __kernel_old_timeval pr_cstime;
    elf_gregset_t pr_reg;
    int pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct elf_prstatus {
    struct elf_prstatus_common common;
    elf_gregset_t pr_reg;
    int pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct elf_prstatus {
    struct elf_prstatus_common common;
    elf_gregset_t pr_reg;
    int pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct elf_prstatus {
    struct elf_prstatus_common common;
    elf_gregset_t pr_reg;
    int pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct elf_prstatus {
    struct elf_prstatus_common common;
    elf_gregset_t pr_reg;
    int pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct elf_prstatus {
    struct elf_prstatus_common common;
    elf_gregset_t pr_reg;
    int pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct elf_prstatus {
    struct elf_prstatus_common common;
    elf_gregset_t pr_reg;
    int pr_fpvalid;
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
struct elf_prstatus {
    struct elf_siginfo pr_info;
    short int pr_cursig;
    long unsigned int pr_sigpend;
    long unsigned int pr_sighold;
    pid_t pr_pid;
    pid_t pr_ppid;
    pid_t pr_pgrp;
    pid_t pr_sid;
    struct timeval pr_utime;
    struct timeval pr_stime;
    struct timeval pr_cutime;
    struct timeval pr_cstime;
    elf_gregset_t pr_reg;
    int pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct elf_prstatus {
    struct elf_siginfo pr_info;
    short int pr_cursig;
    long unsigned int pr_sigpend;
    long unsigned int pr_sighold;
    pid_t pr_pid;
    pid_t pr_ppid;
    pid_t pr_pgrp;
    pid_t pr_sid;
    struct timeval pr_utime;
    struct timeval pr_stime;
    struct timeval pr_cutime;
    struct timeval pr_cstime;
    elf_gregset_t pr_reg;
    long unsigned int pr_exec_fdpic_loadmap;
    long unsigned int pr_interp_fdpic_loadmap;
    int pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct elf_prstatus {
    struct elf_siginfo pr_info;
    short int pr_cursig;
    long unsigned int pr_sigpend;
    long unsigned int pr_sighold;
    pid_t pr_pid;
    pid_t pr_ppid;
    pid_t pr_pgrp;
    pid_t pr_sid;
    struct timeval pr_utime;
    struct timeval pr_stime;
    struct timeval pr_cutime;
    struct timeval pr_cstime;
    elf_gregset_t pr_reg;
    int pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct elf_prstatus {
    struct elf_siginfo pr_info;
    short int pr_cursig;
    long unsigned int pr_sigpend;
    long unsigned int pr_sighold;
    pid_t pr_pid;
    pid_t pr_ppid;
    pid_t pr_pgrp;
    pid_t pr_sid;
    struct timeval pr_utime;
    struct timeval pr_stime;
    struct timeval pr_cutime;
    struct timeval pr_cstime;
    elf_gregset_t pr_reg;
    int pr_fpvalid;
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
struct elf_prstatus {
    struct elf_siginfo pr_info;
    short int pr_cursig;
    long unsigned int pr_sigpend;
    long unsigned int pr_sighold;
    pid_t pr_pid;
    pid_t pr_ppid;
    pid_t pr_pgrp;
    pid_t pr_sid;
    struct timeval pr_utime;
    struct timeval pr_stime;
    struct timeval pr_cutime;
    struct timeval pr_cstime;
    elf_gregset_t pr_reg;
    int pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct elf_prstatus {
    struct elf_siginfo pr_info;
    short int pr_cursig;
    long unsigned int pr_sigpend;
    long unsigned int pr_sighold;
    pid_t pr_pid;
    pid_t pr_ppid;
    pid_t pr_pgrp;
    pid_t pr_sid;
    struct timeval pr_utime;
    struct timeval pr_stime;
    struct timeval pr_cutime;
    struct timeval pr_cstime;
    elf_gregset_t pr_reg;
    int pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct elf_prstatus {
    struct elf_siginfo pr_info;
    short int pr_cursig;
    long unsigned int pr_sigpend;
    long unsigned int pr_sighold;
    pid_t pr_pid;
    pid_t pr_ppid;
    pid_t pr_pgrp;
    pid_t pr_sid;
    struct timeval pr_utime;
    struct timeval pr_stime;
    struct timeval pr_cutime;
    struct timeval pr_cstime;
    elf_gregset_t pr_reg;
    int pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct elf_prstatus {
    struct elf_siginfo pr_info;
    short int pr_cursig;
    long unsigned int pr_sigpend;
    long unsigned int pr_sighold;
    pid_t pr_pid;
    pid_t pr_ppid;
    pid_t pr_pgrp;
    pid_t pr_sid;
    struct timeval pr_utime;
    struct timeval pr_stime;
    struct timeval pr_cutime;
    struct timeval pr_cstime;
    elf_gregset_t pr_reg;
    int pr_fpvalid;
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
<code>struct timeval pr_utime</code> ➡️ <code>struct __kernel_old_timeval pr_utime</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct timeval pr_stime</code> ➡️ <code>struct __kernel_old_timeval pr_stime</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct timeval pr_cutime</code> ➡️ <code>struct __kernel_old_timeval pr_cutime</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct timeval pr_cstime</code> ➡️ <code>struct __kernel_old_timeval pr_cstime</code>
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
<code>struct elf_prstatus_common common</code>
</li>
<li>
<b>Field removed. </b>
<code>struct elf_siginfo pr_info</code>
</li>
<li>
<b>Field removed. </b>
<code>short int pr_cursig</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int pr_sigpend</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int pr_sighold</code>
</li>
<li>
<b>Field removed. </b>
<code>pid_t pr_pid</code>
</li>
<li>
<b>Field removed. </b>
<code>pid_t pr_ppid</code>
</li>
<li>
<b>Field removed. </b>
<code>pid_t pr_pgrp</code>
</li>
<li>
<b>Field removed. </b>
<code>pid_t pr_sid</code>
</li>
<li>
<b>Field removed. </b>
<code>struct __kernel_old_timeval pr_utime</code>
</li>
<li>
<b>Field removed. </b>
<code>struct __kernel_old_timeval pr_stime</code>
</li>
<li>
<b>Field removed. </b>
<code>struct __kernel_old_timeval pr_cutime</code>
</li>
<li>
<b>Field removed. </b>
<code>struct __kernel_old_timeval pr_cstime</code>
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
<b>Field added. </b>
<code>long unsigned int pr_exec_fdpic_loadmap</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int pr_interp_fdpic_loadmap</code>
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
