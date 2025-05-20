# Struct: <code>compat_elf_prstatus</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct compat_elf_prstatus {
    struct compat_elf_siginfo pr_info;
    short int pr_cursig;
    compat_ulong_t pr_sigpend;
    compat_ulong_t pr_sighold;
    compat_pid_t pr_pid;
    compat_pid_t pr_ppid;
    compat_pid_t pr_pgrp;
    compat_pid_t pr_sid;
    struct compat_timeval pr_utime;
    struct compat_timeval pr_stime;
    struct compat_timeval pr_cutime;
    struct compat_timeval pr_cstime;
    compat_elf_gregset_t pr_reg;
    compat_int_t pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct compat_elf_prstatus {
    struct compat_elf_siginfo pr_info;
    short int pr_cursig;
    compat_ulong_t pr_sigpend;
    compat_ulong_t pr_sighold;
    compat_pid_t pr_pid;
    compat_pid_t pr_ppid;
    compat_pid_t pr_pgrp;
    compat_pid_t pr_sid;
    struct compat_timeval pr_utime;
    struct compat_timeval pr_stime;
    struct compat_timeval pr_cutime;
    struct compat_timeval pr_cstime;
    compat_elf_gregset_t pr_reg;
    compat_int_t pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct compat_elf_prstatus {
    struct compat_elf_siginfo pr_info;
    short int pr_cursig;
    compat_ulong_t pr_sigpend;
    compat_ulong_t pr_sighold;
    compat_pid_t pr_pid;
    compat_pid_t pr_ppid;
    compat_pid_t pr_pgrp;
    compat_pid_t pr_sid;
    struct compat_timeval pr_utime;
    struct compat_timeval pr_stime;
    struct compat_timeval pr_cutime;
    struct compat_timeval pr_cstime;
    compat_elf_gregset_t pr_reg;
    compat_int_t pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct compat_elf_prstatus {
    struct compat_elf_siginfo pr_info;
    short int pr_cursig;
    compat_ulong_t pr_sigpend;
    compat_ulong_t pr_sighold;
    compat_pid_t pr_pid;
    compat_pid_t pr_ppid;
    compat_pid_t pr_pgrp;
    compat_pid_t pr_sid;
    struct compat_timeval pr_utime;
    struct compat_timeval pr_stime;
    struct compat_timeval pr_cutime;
    struct compat_timeval pr_cstime;
    compat_elf_gregset_t pr_reg;
    compat_int_t pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct compat_elf_prstatus {
    struct compat_elf_siginfo pr_info;
    short int pr_cursig;
    compat_ulong_t pr_sigpend;
    compat_ulong_t pr_sighold;
    compat_pid_t pr_pid;
    compat_pid_t pr_ppid;
    compat_pid_t pr_pgrp;
    compat_pid_t pr_sid;
    struct compat_timeval pr_utime;
    struct compat_timeval pr_stime;
    struct compat_timeval pr_cutime;
    struct compat_timeval pr_cstime;
    compat_elf_gregset_t pr_reg;
    compat_int_t pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct compat_elf_prstatus {
    struct compat_elf_siginfo pr_info;
    short int pr_cursig;
    compat_ulong_t pr_sigpend;
    compat_ulong_t pr_sighold;
    compat_pid_t pr_pid;
    compat_pid_t pr_ppid;
    compat_pid_t pr_pgrp;
    compat_pid_t pr_sid;
    struct compat_timeval pr_utime;
    struct compat_timeval pr_stime;
    struct compat_timeval pr_cutime;
    struct compat_timeval pr_cstime;
    compat_elf_gregset_t pr_reg;
    compat_int_t pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct compat_elf_prstatus {
    struct compat_elf_siginfo pr_info;
    short int pr_cursig;
    compat_ulong_t pr_sigpend;
    compat_ulong_t pr_sighold;
    compat_pid_t pr_pid;
    compat_pid_t pr_ppid;
    compat_pid_t pr_pgrp;
    compat_pid_t pr_sid;
    struct old_timeval32 pr_utime;
    struct old_timeval32 pr_stime;
    struct old_timeval32 pr_cutime;
    struct old_timeval32 pr_cstime;
    compat_elf_gregset_t pr_reg;
    compat_int_t pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct compat_elf_prstatus {
    struct compat_elf_siginfo pr_info;
    short int pr_cursig;
    compat_ulong_t pr_sigpend;
    compat_ulong_t pr_sighold;
    compat_pid_t pr_pid;
    compat_pid_t pr_ppid;
    compat_pid_t pr_pgrp;
    compat_pid_t pr_sid;
    struct old_timeval32 pr_utime;
    struct old_timeval32 pr_stime;
    struct old_timeval32 pr_cutime;
    struct old_timeval32 pr_cstime;
    compat_elf_gregset_t pr_reg;
    compat_int_t pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct compat_elf_prstatus {
    struct compat_elf_siginfo pr_info;
    short int pr_cursig;
    compat_ulong_t pr_sigpend;
    compat_ulong_t pr_sighold;
    compat_pid_t pr_pid;
    compat_pid_t pr_ppid;
    compat_pid_t pr_pgrp;
    compat_pid_t pr_sid;
    struct old_timeval32 pr_utime;
    struct old_timeval32 pr_stime;
    struct old_timeval32 pr_cutime;
    struct old_timeval32 pr_cstime;
    compat_elf_gregset_t pr_reg;
    compat_int_t pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct compat_elf_prstatus {
    struct compat_elf_siginfo pr_info;
    short int pr_cursig;
    compat_ulong_t pr_sigpend;
    compat_ulong_t pr_sighold;
    compat_pid_t pr_pid;
    compat_pid_t pr_ppid;
    compat_pid_t pr_pgrp;
    compat_pid_t pr_sid;
    struct old_timeval32 pr_utime;
    struct old_timeval32 pr_stime;
    struct old_timeval32 pr_cutime;
    struct old_timeval32 pr_cstime;
    compat_elf_gregset_t pr_reg;
    compat_int_t pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct compat_elf_prstatus {
    struct compat_elf_siginfo pr_info;
    short int pr_cursig;
    compat_ulong_t pr_sigpend;
    compat_ulong_t pr_sighold;
    compat_pid_t pr_pid;
    compat_pid_t pr_ppid;
    compat_pid_t pr_pgrp;
    compat_pid_t pr_sid;
    struct old_timeval32 pr_utime;
    struct old_timeval32 pr_stime;
    struct old_timeval32 pr_cutime;
    struct old_timeval32 pr_cstime;
    compat_elf_gregset_t pr_reg;
    compat_int_t pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct compat_elf_prstatus {
    struct compat_elf_prstatus_common common;
    compat_elf_gregset_t pr_reg;
    compat_int_t pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct compat_elf_prstatus {
    struct compat_elf_prstatus_common common;
    compat_elf_gregset_t pr_reg;
    compat_int_t pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct compat_elf_prstatus {
    struct compat_elf_prstatus_common common;
    compat_elf_gregset_t pr_reg;
    compat_int_t pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct compat_elf_prstatus {
    struct compat_elf_prstatus_common common;
    compat_elf_gregset_t pr_reg;
    compat_int_t pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct compat_elf_prstatus {
    struct compat_elf_prstatus_common common;
    compat_elf_gregset_t pr_reg;
    compat_int_t pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct compat_elf_prstatus {
    struct compat_elf_prstatus_common common;
    compat_elf_gregset_t pr_reg;
    compat_int_t pr_fpvalid;
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
struct compat_elf_prstatus {
    struct compat_elf_siginfo pr_info;
    short int pr_cursig;
    compat_ulong_t pr_sigpend;
    compat_ulong_t pr_sighold;
    compat_pid_t pr_pid;
    compat_pid_t pr_ppid;
    compat_pid_t pr_pgrp;
    compat_pid_t pr_sid;
    struct old_timeval32 pr_utime;
    struct old_timeval32 pr_stime;
    struct old_timeval32 pr_cutime;
    struct old_timeval32 pr_cstime;
    compat_elf_gregset_t pr_reg;
    compat_int_t pr_fpvalid;
};
```
</details>
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct compat_elf_prstatus {
    struct compat_elf_siginfo pr_info;
    short int pr_cursig;
    compat_ulong_t pr_sigpend;
    compat_ulong_t pr_sighold;
    compat_pid_t pr_pid;
    compat_pid_t pr_ppid;
    compat_pid_t pr_pgrp;
    compat_pid_t pr_sid;
    struct old_timeval32 pr_utime;
    struct old_timeval32 pr_stime;
    struct old_timeval32 pr_cutime;
    struct old_timeval32 pr_cstime;
    compat_elf_gregset_t pr_reg;
    compat_int_t pr_fpvalid;
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
struct compat_elf_prstatus {
    struct compat_elf_siginfo pr_info;
    short int pr_cursig;
    compat_ulong_t pr_sigpend;
    compat_ulong_t pr_sighold;
    compat_pid_t pr_pid;
    compat_pid_t pr_ppid;
    compat_pid_t pr_pgrp;
    compat_pid_t pr_sid;
    struct old_timeval32 pr_utime;
    struct old_timeval32 pr_stime;
    struct old_timeval32 pr_cutime;
    struct old_timeval32 pr_cstime;
    compat_elf_gregset_t pr_reg;
    compat_int_t pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct compat_elf_prstatus {
    struct compat_elf_siginfo pr_info;
    short int pr_cursig;
    compat_ulong_t pr_sigpend;
    compat_ulong_t pr_sighold;
    compat_pid_t pr_pid;
    compat_pid_t pr_ppid;
    compat_pid_t pr_pgrp;
    compat_pid_t pr_sid;
    struct old_timeval32 pr_utime;
    struct old_timeval32 pr_stime;
    struct old_timeval32 pr_cutime;
    struct old_timeval32 pr_cstime;
    compat_elf_gregset_t pr_reg;
    compat_int_t pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct compat_elf_prstatus {
    struct compat_elf_siginfo pr_info;
    short int pr_cursig;
    compat_ulong_t pr_sigpend;
    compat_ulong_t pr_sighold;
    compat_pid_t pr_pid;
    compat_pid_t pr_ppid;
    compat_pid_t pr_pgrp;
    compat_pid_t pr_sid;
    struct old_timeval32 pr_utime;
    struct old_timeval32 pr_stime;
    struct old_timeval32 pr_cutime;
    struct old_timeval32 pr_cstime;
    compat_elf_gregset_t pr_reg;
    compat_int_t pr_fpvalid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct compat_elf_prstatus {
    struct compat_elf_siginfo pr_info;
    short int pr_cursig;
    compat_ulong_t pr_sigpend;
    compat_ulong_t pr_sighold;
    compat_pid_t pr_pid;
    compat_pid_t pr_ppid;
    compat_pid_t pr_pgrp;
    compat_pid_t pr_sid;
    struct old_timeval32 pr_utime;
    struct old_timeval32 pr_stime;
    struct old_timeval32 pr_cutime;
    struct old_timeval32 pr_cstime;
    compat_elf_gregset_t pr_reg;
    compat_int_t pr_fpvalid;
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
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct compat_timeval pr_utime</code> ➡️ <code>struct old_timeval32 pr_utime</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct compat_timeval pr_stime</code> ➡️ <code>struct old_timeval32 pr_stime</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct compat_timeval pr_cutime</code> ➡️ <code>struct old_timeval32 pr_cutime</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct compat_timeval pr_cstime</code> ➡️ <code>struct old_timeval32 pr_cstime</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct compat_elf_prstatus_common common</code>
</li>
<li>
<b>Field removed. </b>
<code>struct compat_elf_siginfo pr_info</code>
</li>
<li>
<b>Field removed. </b>
<code>short int pr_cursig</code>
</li>
<li>
<b>Field removed. </b>
<code>compat_ulong_t pr_sigpend</code>
</li>
<li>
<b>Field removed. </b>
<code>compat_ulong_t pr_sighold</code>
</li>
<li>
<b>Field removed. </b>
<code>compat_pid_t pr_pid</code>
</li>
<li>
<b>Field removed. </b>
<code>compat_pid_t pr_ppid</code>
</li>
<li>
<b>Field removed. </b>
<code>compat_pid_t pr_pgrp</code>
</li>
<li>
<b>Field removed. </b>
<code>compat_pid_t pr_sid</code>
</li>
<li>
<b>Field removed. </b>
<code>struct old_timeval32 pr_utime</code>
</li>
<li>
<b>Field removed. </b>
<code>struct old_timeval32 pr_stime</code>
</li>
<li>
<b>Field removed. </b>
<code>struct old_timeval32 pr_cutime</code>
</li>
<li>
<b>Field removed. </b>
<code>struct old_timeval32 pr_cstime</code>
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
