# Struct: <code>compat_shmid64_ds</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct compat_shmid64_ds {
    struct compat_ipc64_perm shm_perm;
    compat_size_t shm_segsz;
    compat_time_t shm_atime;
    compat_ulong_t __unused1;
    compat_time_t shm_dtime;
    compat_ulong_t __unused2;
    compat_time_t shm_ctime;
    compat_ulong_t __unused3;
    compat_pid_t shm_cpid;
    compat_pid_t shm_lpid;
    compat_ulong_t shm_nattch;
    compat_ulong_t __unused4;
    compat_ulong_t __unused5;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct compat_shmid64_ds {
    struct compat_ipc64_perm shm_perm;
    compat_size_t shm_segsz;
    compat_time_t shm_atime;
    compat_ulong_t __unused1;
    compat_time_t shm_dtime;
    compat_ulong_t __unused2;
    compat_time_t shm_ctime;
    compat_ulong_t __unused3;
    compat_pid_t shm_cpid;
    compat_pid_t shm_lpid;
    compat_ulong_t shm_nattch;
    compat_ulong_t __unused4;
    compat_ulong_t __unused5;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct compat_shmid64_ds {
    struct compat_ipc64_perm shm_perm;
    compat_size_t shm_segsz;
    compat_time_t shm_atime;
    compat_ulong_t __unused1;
    compat_time_t shm_dtime;
    compat_ulong_t __unused2;
    compat_time_t shm_ctime;
    compat_ulong_t __unused3;
    compat_pid_t shm_cpid;
    compat_pid_t shm_lpid;
    compat_ulong_t shm_nattch;
    compat_ulong_t __unused4;
    compat_ulong_t __unused5;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct compat_shmid64_ds {
    struct compat_ipc64_perm shm_perm;
    compat_size_t shm_segsz;
    compat_time_t shm_atime;
    compat_ulong_t __unused1;
    compat_time_t shm_dtime;
    compat_ulong_t __unused2;
    compat_time_t shm_ctime;
    compat_ulong_t __unused3;
    compat_pid_t shm_cpid;
    compat_pid_t shm_lpid;
    compat_ulong_t shm_nattch;
    compat_ulong_t __unused4;
    compat_ulong_t __unused5;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct compat_shmid64_ds {
    struct compat_ipc64_perm shm_perm;
    compat_size_t shm_segsz;
    compat_time_t shm_atime;
    compat_ulong_t __unused1;
    compat_time_t shm_dtime;
    compat_ulong_t __unused2;
    compat_time_t shm_ctime;
    compat_ulong_t __unused3;
    compat_pid_t shm_cpid;
    compat_pid_t shm_lpid;
    compat_ulong_t shm_nattch;
    compat_ulong_t __unused4;
    compat_ulong_t __unused5;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct compat_shmid64_ds {
    struct compat_ipc64_perm shm_perm;
    compat_size_t shm_segsz;
    compat_ulong_t shm_atime;
    compat_ulong_t shm_atime_high;
    compat_ulong_t shm_dtime;
    compat_ulong_t shm_dtime_high;
    compat_ulong_t shm_ctime;
    compat_ulong_t shm_ctime_high;
    compat_pid_t shm_cpid;
    compat_pid_t shm_lpid;
    compat_ulong_t shm_nattch;
    compat_ulong_t __unused4;
    compat_ulong_t __unused5;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct compat_shmid64_ds {
    struct compat_ipc64_perm shm_perm;
    compat_size_t shm_segsz;
    compat_ulong_t shm_atime;
    compat_ulong_t shm_atime_high;
    compat_ulong_t shm_dtime;
    compat_ulong_t shm_dtime_high;
    compat_ulong_t shm_ctime;
    compat_ulong_t shm_ctime_high;
    compat_pid_t shm_cpid;
    compat_pid_t shm_lpid;
    compat_ulong_t shm_nattch;
    compat_ulong_t __unused4;
    compat_ulong_t __unused5;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct compat_shmid64_ds {
    struct compat_ipc64_perm shm_perm;
    compat_size_t shm_segsz;
    compat_ulong_t shm_atime;
    compat_ulong_t shm_atime_high;
    compat_ulong_t shm_dtime;
    compat_ulong_t shm_dtime_high;
    compat_ulong_t shm_ctime;
    compat_ulong_t shm_ctime_high;
    compat_pid_t shm_cpid;
    compat_pid_t shm_lpid;
    compat_ulong_t shm_nattch;
    compat_ulong_t __unused4;
    compat_ulong_t __unused5;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct compat_shmid64_ds {
    struct compat_ipc64_perm shm_perm;
    compat_size_t shm_segsz;
    compat_ulong_t shm_atime;
    compat_ulong_t shm_atime_high;
    compat_ulong_t shm_dtime;
    compat_ulong_t shm_dtime_high;
    compat_ulong_t shm_ctime;
    compat_ulong_t shm_ctime_high;
    compat_pid_t shm_cpid;
    compat_pid_t shm_lpid;
    compat_ulong_t shm_nattch;
    compat_ulong_t __unused4;
    compat_ulong_t __unused5;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct compat_shmid64_ds {
    struct compat_ipc64_perm shm_perm;
    compat_size_t shm_segsz;
    compat_ulong_t shm_atime;
    compat_ulong_t shm_atime_high;
    compat_ulong_t shm_dtime;
    compat_ulong_t shm_dtime_high;
    compat_ulong_t shm_ctime;
    compat_ulong_t shm_ctime_high;
    compat_pid_t shm_cpid;
    compat_pid_t shm_lpid;
    compat_ulong_t shm_nattch;
    compat_ulong_t __unused4;
    compat_ulong_t __unused5;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct compat_shmid64_ds {
    struct compat_ipc64_perm shm_perm;
    compat_size_t shm_segsz;
    compat_ulong_t shm_atime;
    compat_ulong_t shm_atime_high;
    compat_ulong_t shm_dtime;
    compat_ulong_t shm_dtime_high;
    compat_ulong_t shm_ctime;
    compat_ulong_t shm_ctime_high;
    compat_pid_t shm_cpid;
    compat_pid_t shm_lpid;
    compat_ulong_t shm_nattch;
    compat_ulong_t __unused4;
    compat_ulong_t __unused5;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct compat_shmid64_ds {
    struct compat_ipc64_perm shm_perm;
    compat_size_t shm_segsz;
    compat_ulong_t shm_atime;
    compat_ulong_t shm_atime_high;
    compat_ulong_t shm_dtime;
    compat_ulong_t shm_dtime_high;
    compat_ulong_t shm_ctime;
    compat_ulong_t shm_ctime_high;
    compat_pid_t shm_cpid;
    compat_pid_t shm_lpid;
    compat_ulong_t shm_nattch;
    compat_ulong_t __unused4;
    compat_ulong_t __unused5;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct compat_shmid64_ds {
    struct compat_ipc64_perm shm_perm;
    compat_size_t shm_segsz;
    compat_ulong_t shm_atime;
    compat_ulong_t shm_atime_high;
    compat_ulong_t shm_dtime;
    compat_ulong_t shm_dtime_high;
    compat_ulong_t shm_ctime;
    compat_ulong_t shm_ctime_high;
    compat_pid_t shm_cpid;
    compat_pid_t shm_lpid;
    compat_ulong_t shm_nattch;
    compat_ulong_t __unused4;
    compat_ulong_t __unused5;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct compat_shmid64_ds {
    struct compat_ipc64_perm shm_perm;
    compat_size_t shm_segsz;
    compat_ulong_t shm_atime;
    compat_ulong_t shm_atime_high;
    compat_ulong_t shm_dtime;
    compat_ulong_t shm_dtime_high;
    compat_ulong_t shm_ctime;
    compat_ulong_t shm_ctime_high;
    compat_pid_t shm_cpid;
    compat_pid_t shm_lpid;
    compat_ulong_t shm_nattch;
    compat_ulong_t __unused4;
    compat_ulong_t __unused5;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct compat_shmid64_ds {
    struct compat_ipc64_perm shm_perm;
    compat_size_t shm_segsz;
    compat_ulong_t shm_atime;
    compat_ulong_t shm_atime_high;
    compat_ulong_t shm_dtime;
    compat_ulong_t shm_dtime_high;
    compat_ulong_t shm_ctime;
    compat_ulong_t shm_ctime_high;
    compat_pid_t shm_cpid;
    compat_pid_t shm_lpid;
    compat_ulong_t shm_nattch;
    compat_ulong_t __unused4;
    compat_ulong_t __unused5;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct compat_shmid64_ds {
    struct compat_ipc64_perm shm_perm;
    compat_size_t shm_segsz;
    compat_ulong_t shm_atime;
    compat_ulong_t shm_atime_high;
    compat_ulong_t shm_dtime;
    compat_ulong_t shm_dtime_high;
    compat_ulong_t shm_ctime;
    compat_ulong_t shm_ctime_high;
    compat_pid_t shm_cpid;
    compat_pid_t shm_lpid;
    compat_ulong_t shm_nattch;
    compat_ulong_t __unused4;
    compat_ulong_t __unused5;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct compat_shmid64_ds {
    struct compat_ipc64_perm shm_perm;
    compat_size_t shm_segsz;
    compat_ulong_t shm_atime;
    compat_ulong_t shm_atime_high;
    compat_ulong_t shm_dtime;
    compat_ulong_t shm_dtime_high;
    compat_ulong_t shm_ctime;
    compat_ulong_t shm_ctime_high;
    compat_pid_t shm_cpid;
    compat_pid_t shm_lpid;
    compat_ulong_t shm_nattch;
    compat_ulong_t __unused4;
    compat_ulong_t __unused5;
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
struct compat_shmid64_ds {
    struct compat_ipc64_perm shm_perm;
    compat_size_t shm_segsz;
    compat_ulong_t shm_atime;
    compat_ulong_t shm_atime_high;
    compat_ulong_t shm_dtime;
    compat_ulong_t shm_dtime_high;
    compat_ulong_t shm_ctime;
    compat_ulong_t shm_ctime_high;
    compat_pid_t shm_cpid;
    compat_pid_t shm_lpid;
    compat_ulong_t shm_nattch;
    compat_ulong_t __unused4;
    compat_ulong_t __unused5;
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
struct compat_shmid64_ds {
    struct compat_ipc64_perm shm_perm;
    unsigned int shm_atime_high;
    unsigned int shm_atime;
    unsigned int shm_dtime_high;
    unsigned int shm_dtime;
    unsigned int shm_ctime_high;
    unsigned int shm_ctime;
    unsigned int __unused4;
    compat_size_t shm_segsz;
    compat_pid_t shm_cpid;
    compat_pid_t shm_lpid;
    compat_ulong_t shm_nattch;
    compat_ulong_t __unused5;
    compat_ulong_t __unused6;
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
struct compat_shmid64_ds {
    struct compat_ipc64_perm shm_perm;
    compat_size_t shm_segsz;
    compat_ulong_t shm_atime;
    compat_ulong_t shm_atime_high;
    compat_ulong_t shm_dtime;
    compat_ulong_t shm_dtime_high;
    compat_ulong_t shm_ctime;
    compat_ulong_t shm_ctime_high;
    compat_pid_t shm_cpid;
    compat_pid_t shm_lpid;
    compat_ulong_t shm_nattch;
    compat_ulong_t __unused4;
    compat_ulong_t __unused5;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct compat_shmid64_ds {
    struct compat_ipc64_perm shm_perm;
    compat_size_t shm_segsz;
    compat_ulong_t shm_atime;
    compat_ulong_t shm_atime_high;
    compat_ulong_t shm_dtime;
    compat_ulong_t shm_dtime_high;
    compat_ulong_t shm_ctime;
    compat_ulong_t shm_ctime_high;
    compat_pid_t shm_cpid;
    compat_pid_t shm_lpid;
    compat_ulong_t shm_nattch;
    compat_ulong_t __unused4;
    compat_ulong_t __unused5;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct compat_shmid64_ds {
    struct compat_ipc64_perm shm_perm;
    compat_size_t shm_segsz;
    compat_ulong_t shm_atime;
    compat_ulong_t shm_atime_high;
    compat_ulong_t shm_dtime;
    compat_ulong_t shm_dtime_high;
    compat_ulong_t shm_ctime;
    compat_ulong_t shm_ctime_high;
    compat_pid_t shm_cpid;
    compat_pid_t shm_lpid;
    compat_ulong_t shm_nattch;
    compat_ulong_t __unused4;
    compat_ulong_t __unused5;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct compat_shmid64_ds {
    struct compat_ipc64_perm shm_perm;
    compat_size_t shm_segsz;
    compat_ulong_t shm_atime;
    compat_ulong_t shm_atime_high;
    compat_ulong_t shm_dtime;
    compat_ulong_t shm_dtime_high;
    compat_ulong_t shm_ctime;
    compat_ulong_t shm_ctime_high;
    compat_pid_t shm_cpid;
    compat_pid_t shm_lpid;
    compat_ulong_t shm_nattch;
    compat_ulong_t __unused4;
    compat_ulong_t __unused5;
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
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>compat_ulong_t shm_atime_high</code>
</li>
<li>
<b>Field added. </b>
<code>compat_ulong_t shm_dtime_high</code>
</li>
<li>
<b>Field added. </b>
<code>compat_ulong_t shm_ctime_high</code>
</li>
<li>
<b>Field removed. </b>
<code>compat_ulong_t __unused1</code>
</li>
<li>
<b>Field removed. </b>
<code>compat_ulong_t __unused2</code>
</li>
<li>
<b>Field removed. </b>
<code>compat_ulong_t __unused3</code>
</li>
<li>
<b>Field type changed. </b>
<code>compat_time_t shm_atime</code> ➡️ <code>compat_ulong_t shm_atime</code>
</li>
<li>
<b>Field type changed. </b>
<code>compat_time_t shm_dtime</code> ➡️ <code>compat_ulong_t shm_dtime</code>
</li>
<li>
<b>Field type changed. </b>
<code>compat_time_t shm_ctime</code> ➡️ <code>compat_ulong_t shm_ctime</code>
</li>
</ul>
</details>
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
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>compat_ulong_t __unused6</code>
</li>
<li>
<b>Field type changed. </b>
<code>compat_ulong_t shm_atime</code> ➡️ <code>unsigned int shm_atime</code>
</li>
<li>
<b>Field type changed. </b>
<code>compat_ulong_t shm_atime_high</code> ➡️ <code>unsigned int shm_atime_high</code>
</li>
<li>
<b>Field type changed. </b>
<code>compat_ulong_t shm_dtime</code> ➡️ <code>unsigned int shm_dtime</code>
</li>
<li>
<b>Field type changed. </b>
<code>compat_ulong_t shm_dtime_high</code> ➡️ <code>unsigned int shm_dtime_high</code>
</li>
<li>
<b>Field type changed. </b>
<code>compat_ulong_t shm_ctime</code> ➡️ <code>unsigned int shm_ctime</code>
</li>
<li>
<b>Field type changed. </b>
<code>compat_ulong_t shm_ctime_high</code> ➡️ <code>unsigned int shm_ctime_high</code>
</li>
<li>
<b>Field type changed. </b>
<code>compat_ulong_t __unused4</code> ➡️ <code>unsigned int __unused4</code>
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
