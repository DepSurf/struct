# Struct: <code>compat_msqid_ds</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct compat_msqid_ds {
    struct compat_ipc_perm msg_perm;
    compat_uptr_t msg_first;
    compat_uptr_t msg_last;
    compat_time_t msg_stime;
    compat_time_t msg_rtime;
    compat_time_t msg_ctime;
    compat_ulong_t msg_lcbytes;
    compat_ulong_t msg_lqbytes;
    short unsigned int msg_cbytes;
    short unsigned int msg_qnum;
    short unsigned int msg_qbytes;
    compat_ipc_pid_t msg_lspid;
    compat_ipc_pid_t msg_lrpid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct compat_msqid_ds {
    struct compat_ipc_perm msg_perm;
    compat_uptr_t msg_first;
    compat_uptr_t msg_last;
    compat_time_t msg_stime;
    compat_time_t msg_rtime;
    compat_time_t msg_ctime;
    compat_ulong_t msg_lcbytes;
    compat_ulong_t msg_lqbytes;
    short unsigned int msg_cbytes;
    short unsigned int msg_qnum;
    short unsigned int msg_qbytes;
    compat_ipc_pid_t msg_lspid;
    compat_ipc_pid_t msg_lrpid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct compat_msqid_ds {
    struct compat_ipc_perm msg_perm;
    compat_uptr_t msg_first;
    compat_uptr_t msg_last;
    compat_time_t msg_stime;
    compat_time_t msg_rtime;
    compat_time_t msg_ctime;
    compat_ulong_t msg_lcbytes;
    compat_ulong_t msg_lqbytes;
    short unsigned int msg_cbytes;
    short unsigned int msg_qnum;
    short unsigned int msg_qbytes;
    compat_ipc_pid_t msg_lspid;
    compat_ipc_pid_t msg_lrpid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct compat_msqid_ds {
    struct compat_ipc_perm msg_perm;
    compat_uptr_t msg_first;
    compat_uptr_t msg_last;
    compat_time_t msg_stime;
    compat_time_t msg_rtime;
    compat_time_t msg_ctime;
    compat_ulong_t msg_lcbytes;
    compat_ulong_t msg_lqbytes;
    short unsigned int msg_cbytes;
    short unsigned int msg_qnum;
    short unsigned int msg_qbytes;
    compat_ipc_pid_t msg_lspid;
    compat_ipc_pid_t msg_lrpid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct compat_msqid_ds {
    struct compat_ipc_perm msg_perm;
    compat_uptr_t msg_first;
    compat_uptr_t msg_last;
    compat_time_t msg_stime;
    compat_time_t msg_rtime;
    compat_time_t msg_ctime;
    compat_ulong_t msg_lcbytes;
    compat_ulong_t msg_lqbytes;
    short unsigned int msg_cbytes;
    short unsigned int msg_qnum;
    short unsigned int msg_qbytes;
    compat_ipc_pid_t msg_lspid;
    compat_ipc_pid_t msg_lrpid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct compat_msqid_ds {
    struct compat_ipc_perm msg_perm;
    compat_uptr_t msg_first;
    compat_uptr_t msg_last;
    compat_time_t msg_stime;
    compat_time_t msg_rtime;
    compat_time_t msg_ctime;
    compat_ulong_t msg_lcbytes;
    compat_ulong_t msg_lqbytes;
    short unsigned int msg_cbytes;
    short unsigned int msg_qnum;
    short unsigned int msg_qbytes;
    compat_ipc_pid_t msg_lspid;
    compat_ipc_pid_t msg_lrpid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct compat_msqid_ds {
    struct compat_ipc_perm msg_perm;
    compat_uptr_t msg_first;
    compat_uptr_t msg_last;
    old_time32_t msg_stime;
    old_time32_t msg_rtime;
    old_time32_t msg_ctime;
    compat_ulong_t msg_lcbytes;
    compat_ulong_t msg_lqbytes;
    short unsigned int msg_cbytes;
    short unsigned int msg_qnum;
    short unsigned int msg_qbytes;
    compat_ipc_pid_t msg_lspid;
    compat_ipc_pid_t msg_lrpid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct compat_msqid_ds {
    struct compat_ipc_perm msg_perm;
    compat_uptr_t msg_first;
    compat_uptr_t msg_last;
    old_time32_t msg_stime;
    old_time32_t msg_rtime;
    old_time32_t msg_ctime;
    compat_ulong_t msg_lcbytes;
    compat_ulong_t msg_lqbytes;
    short unsigned int msg_cbytes;
    short unsigned int msg_qnum;
    short unsigned int msg_qbytes;
    compat_ipc_pid_t msg_lspid;
    compat_ipc_pid_t msg_lrpid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct compat_msqid_ds {
    struct compat_ipc_perm msg_perm;
    compat_uptr_t msg_first;
    compat_uptr_t msg_last;
    old_time32_t msg_stime;
    old_time32_t msg_rtime;
    old_time32_t msg_ctime;
    compat_ulong_t msg_lcbytes;
    compat_ulong_t msg_lqbytes;
    short unsigned int msg_cbytes;
    short unsigned int msg_qnum;
    short unsigned int msg_qbytes;
    compat_ipc_pid_t msg_lspid;
    compat_ipc_pid_t msg_lrpid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct compat_msqid_ds {
    struct compat_ipc_perm msg_perm;
    compat_uptr_t msg_first;
    compat_uptr_t msg_last;
    old_time32_t msg_stime;
    old_time32_t msg_rtime;
    old_time32_t msg_ctime;
    compat_ulong_t msg_lcbytes;
    compat_ulong_t msg_lqbytes;
    short unsigned int msg_cbytes;
    short unsigned int msg_qnum;
    short unsigned int msg_qbytes;
    compat_ipc_pid_t msg_lspid;
    compat_ipc_pid_t msg_lrpid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct compat_msqid_ds {
    struct compat_ipc_perm msg_perm;
    compat_uptr_t msg_first;
    compat_uptr_t msg_last;
    old_time32_t msg_stime;
    old_time32_t msg_rtime;
    old_time32_t msg_ctime;
    compat_ulong_t msg_lcbytes;
    compat_ulong_t msg_lqbytes;
    short unsigned int msg_cbytes;
    short unsigned int msg_qnum;
    short unsigned int msg_qbytes;
    compat_ipc_pid_t msg_lspid;
    compat_ipc_pid_t msg_lrpid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct compat_msqid_ds {
    struct compat_ipc_perm msg_perm;
    compat_uptr_t msg_first;
    compat_uptr_t msg_last;
    old_time32_t msg_stime;
    old_time32_t msg_rtime;
    old_time32_t msg_ctime;
    compat_ulong_t msg_lcbytes;
    compat_ulong_t msg_lqbytes;
    short unsigned int msg_cbytes;
    short unsigned int msg_qnum;
    short unsigned int msg_qbytes;
    compat_ipc_pid_t msg_lspid;
    compat_ipc_pid_t msg_lrpid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct compat_msqid_ds {
    struct compat_ipc_perm msg_perm;
    compat_uptr_t msg_first;
    compat_uptr_t msg_last;
    old_time32_t msg_stime;
    old_time32_t msg_rtime;
    old_time32_t msg_ctime;
    compat_ulong_t msg_lcbytes;
    compat_ulong_t msg_lqbytes;
    short unsigned int msg_cbytes;
    short unsigned int msg_qnum;
    short unsigned int msg_qbytes;
    compat_ipc_pid_t msg_lspid;
    compat_ipc_pid_t msg_lrpid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct compat_msqid_ds {
    struct compat_ipc_perm msg_perm;
    compat_uptr_t msg_first;
    compat_uptr_t msg_last;
    old_time32_t msg_stime;
    old_time32_t msg_rtime;
    old_time32_t msg_ctime;
    compat_ulong_t msg_lcbytes;
    compat_ulong_t msg_lqbytes;
    short unsigned int msg_cbytes;
    short unsigned int msg_qnum;
    short unsigned int msg_qbytes;
    compat_ipc_pid_t msg_lspid;
    compat_ipc_pid_t msg_lrpid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct compat_msqid_ds {
    struct compat_ipc_perm msg_perm;
    compat_uptr_t msg_first;
    compat_uptr_t msg_last;
    old_time32_t msg_stime;
    old_time32_t msg_rtime;
    old_time32_t msg_ctime;
    compat_ulong_t msg_lcbytes;
    compat_ulong_t msg_lqbytes;
    short unsigned int msg_cbytes;
    short unsigned int msg_qnum;
    short unsigned int msg_qbytes;
    compat_ipc_pid_t msg_lspid;
    compat_ipc_pid_t msg_lrpid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct compat_msqid_ds {
    struct compat_ipc_perm msg_perm;
    compat_uptr_t msg_first;
    compat_uptr_t msg_last;
    old_time32_t msg_stime;
    old_time32_t msg_rtime;
    old_time32_t msg_ctime;
    compat_ulong_t msg_lcbytes;
    compat_ulong_t msg_lqbytes;
    short unsigned int msg_cbytes;
    short unsigned int msg_qnum;
    short unsigned int msg_qbytes;
    compat_ipc_pid_t msg_lspid;
    compat_ipc_pid_t msg_lrpid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct compat_msqid_ds {
    struct compat_ipc_perm msg_perm;
    compat_uptr_t msg_first;
    compat_uptr_t msg_last;
    old_time32_t msg_stime;
    old_time32_t msg_rtime;
    old_time32_t msg_ctime;
    compat_ulong_t msg_lcbytes;
    compat_ulong_t msg_lqbytes;
    short unsigned int msg_cbytes;
    short unsigned int msg_qnum;
    short unsigned int msg_qbytes;
    compat_ipc_pid_t msg_lspid;
    compat_ipc_pid_t msg_lrpid;
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
struct compat_msqid_ds {
    struct compat_ipc_perm msg_perm;
    compat_uptr_t msg_first;
    compat_uptr_t msg_last;
    old_time32_t msg_stime;
    old_time32_t msg_rtime;
    old_time32_t msg_ctime;
    compat_ulong_t msg_lcbytes;
    compat_ulong_t msg_lqbytes;
    short unsigned int msg_cbytes;
    short unsigned int msg_qnum;
    short unsigned int msg_qbytes;
    compat_ipc_pid_t msg_lspid;
    compat_ipc_pid_t msg_lrpid;
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
struct compat_msqid_ds {
    struct compat_ipc_perm msg_perm;
    compat_uptr_t msg_first;
    compat_uptr_t msg_last;
    old_time32_t msg_stime;
    old_time32_t msg_rtime;
    old_time32_t msg_ctime;
    compat_ulong_t msg_lcbytes;
    compat_ulong_t msg_lqbytes;
    short unsigned int msg_cbytes;
    short unsigned int msg_qnum;
    short unsigned int msg_qbytes;
    compat_ipc_pid_t msg_lspid;
    compat_ipc_pid_t msg_lrpid;
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
struct compat_msqid_ds {
    struct compat_ipc_perm msg_perm;
    compat_uptr_t msg_first;
    compat_uptr_t msg_last;
    old_time32_t msg_stime;
    old_time32_t msg_rtime;
    old_time32_t msg_ctime;
    compat_ulong_t msg_lcbytes;
    compat_ulong_t msg_lqbytes;
    short unsigned int msg_cbytes;
    short unsigned int msg_qnum;
    short unsigned int msg_qbytes;
    compat_ipc_pid_t msg_lspid;
    compat_ipc_pid_t msg_lrpid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct compat_msqid_ds {
    struct compat_ipc_perm msg_perm;
    compat_uptr_t msg_first;
    compat_uptr_t msg_last;
    old_time32_t msg_stime;
    old_time32_t msg_rtime;
    old_time32_t msg_ctime;
    compat_ulong_t msg_lcbytes;
    compat_ulong_t msg_lqbytes;
    short unsigned int msg_cbytes;
    short unsigned int msg_qnum;
    short unsigned int msg_qbytes;
    compat_ipc_pid_t msg_lspid;
    compat_ipc_pid_t msg_lrpid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct compat_msqid_ds {
    struct compat_ipc_perm msg_perm;
    compat_uptr_t msg_first;
    compat_uptr_t msg_last;
    old_time32_t msg_stime;
    old_time32_t msg_rtime;
    old_time32_t msg_ctime;
    compat_ulong_t msg_lcbytes;
    compat_ulong_t msg_lqbytes;
    short unsigned int msg_cbytes;
    short unsigned int msg_qnum;
    short unsigned int msg_qbytes;
    compat_ipc_pid_t msg_lspid;
    compat_ipc_pid_t msg_lrpid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct compat_msqid_ds {
    struct compat_ipc_perm msg_perm;
    compat_uptr_t msg_first;
    compat_uptr_t msg_last;
    old_time32_t msg_stime;
    old_time32_t msg_rtime;
    old_time32_t msg_ctime;
    compat_ulong_t msg_lcbytes;
    compat_ulong_t msg_lqbytes;
    short unsigned int msg_cbytes;
    short unsigned int msg_qnum;
    short unsigned int msg_qbytes;
    compat_ipc_pid_t msg_lspid;
    compat_ipc_pid_t msg_lrpid;
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
<code>compat_time_t msg_stime</code> ➡️ <code>old_time32_t msg_stime</code>
</li>
<li>
<b>Field type changed. </b>
<code>compat_time_t msg_rtime</code> ➡️ <code>old_time32_t msg_rtime</code>
</li>
<li>
<b>Field type changed. </b>
<code>compat_time_t msg_ctime</code> ➡️ <code>old_time32_t msg_ctime</code>
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
