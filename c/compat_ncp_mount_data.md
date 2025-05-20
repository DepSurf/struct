# Struct: <code>compat_ncp_mount_data</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct compat_ncp_mount_data {
    compat_int_t version;
    compat_uint_t ncp_fd;
    __compat_uid_t mounted_uid;
    compat_pid_t wdog_pid;
    unsigned char mounted_vol[17];
    compat_uint_t time_out;
    compat_uint_t retry_count;
    compat_uint_t flags;
    __compat_uid_t uid;
    __compat_gid_t gid;
    compat_mode_t file_mode;
    compat_mode_t dir_mode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct compat_ncp_mount_data {
    compat_int_t version;
    compat_uint_t ncp_fd;
    __compat_uid_t mounted_uid;
    compat_pid_t wdog_pid;
    unsigned char mounted_vol[17];
    compat_uint_t time_out;
    compat_uint_t retry_count;
    compat_uint_t flags;
    __compat_uid_t uid;
    __compat_gid_t gid;
    compat_mode_t file_mode;
    compat_mode_t dir_mode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct compat_ncp_mount_data {
    compat_int_t version;
    compat_uint_t ncp_fd;
    __compat_uid_t mounted_uid;
    compat_pid_t wdog_pid;
    unsigned char mounted_vol[17];
    compat_uint_t time_out;
    compat_uint_t retry_count;
    compat_uint_t flags;
    __compat_uid_t uid;
    __compat_gid_t gid;
    compat_mode_t file_mode;
    compat_mode_t dir_mode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct compat_ncp_mount_data {
    compat_int_t version;
    compat_uint_t ncp_fd;
    __compat_uid_t mounted_uid;
    compat_pid_t wdog_pid;
    unsigned char mounted_vol[17];
    compat_uint_t time_out;
    compat_uint_t retry_count;
    compat_uint_t flags;
    __compat_uid_t uid;
    __compat_gid_t gid;
    compat_mode_t file_mode;
    compat_mode_t dir_mode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct compat_ncp_mount_data {
    compat_int_t version;
    compat_uint_t ncp_fd;
    __compat_uid_t mounted_uid;
    compat_pid_t wdog_pid;
    unsigned char mounted_vol[17];
    compat_uint_t time_out;
    compat_uint_t retry_count;
    compat_uint_t flags;
    __compat_uid_t uid;
    __compat_gid_t gid;
    compat_mode_t file_mode;
    compat_mode_t dir_mode;
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
