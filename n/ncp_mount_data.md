# Struct: <code>ncp_mount_data</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct ncp_mount_data {
    int version;
    unsigned int ncp_fd;
    __kernel_uid_t mounted_uid;
    __kernel_pid_t wdog_pid;
    unsigned char mounted_vol[17];
    unsigned int time_out;
    unsigned int retry_count;
    unsigned int flags;
    __kernel_uid_t uid;
    __kernel_gid_t gid;
    __kernel_mode_t file_mode;
    __kernel_mode_t dir_mode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ncp_mount_data {
    int version;
    unsigned int ncp_fd;
    __kernel_uid_t mounted_uid;
    __kernel_pid_t wdog_pid;
    unsigned char mounted_vol[17];
    unsigned int time_out;
    unsigned int retry_count;
    unsigned int flags;
    __kernel_uid_t uid;
    __kernel_gid_t gid;
    __kernel_mode_t file_mode;
    __kernel_mode_t dir_mode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ncp_mount_data {
    int version;
    unsigned int ncp_fd;
    __kernel_uid_t mounted_uid;
    __kernel_pid_t wdog_pid;
    unsigned char mounted_vol[17];
    unsigned int time_out;
    unsigned int retry_count;
    unsigned int flags;
    __kernel_uid_t uid;
    __kernel_gid_t gid;
    __kernel_mode_t file_mode;
    __kernel_mode_t dir_mode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ncp_mount_data {
    int version;
    unsigned int ncp_fd;
    __kernel_uid_t mounted_uid;
    __kernel_pid_t wdog_pid;
    unsigned char mounted_vol[17];
    unsigned int time_out;
    unsigned int retry_count;
    unsigned int flags;
    __kernel_uid_t uid;
    __kernel_gid_t gid;
    __kernel_mode_t file_mode;
    __kernel_mode_t dir_mode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ncp_mount_data {
    int version;
    unsigned int ncp_fd;
    __kernel_uid_t mounted_uid;
    __kernel_pid_t wdog_pid;
    unsigned char mounted_vol[17];
    unsigned int time_out;
    unsigned int retry_count;
    unsigned int flags;
    __kernel_uid_t uid;
    __kernel_gid_t gid;
    __kernel_mode_t file_mode;
    __kernel_mode_t dir_mode;
};
```
</details>
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
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
In <code>5.19</code>: Absent ⚠️
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
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
</ul>
