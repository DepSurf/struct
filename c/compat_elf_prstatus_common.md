# Struct: <code>compat_elf_prstatus_common</code>

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
In <code>5.11</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct compat_elf_prstatus_common {
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
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct compat_elf_prstatus_common {
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
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct compat_elf_prstatus_common {
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
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct compat_elf_prstatus_common {
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
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct compat_elf_prstatus_common {
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
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct compat_elf_prstatus_common {
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
