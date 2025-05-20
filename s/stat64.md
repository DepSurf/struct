# Struct: <code>stat64</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct stat64 {
    long long unsigned int st_dev;
    unsigned char __pad0[4];
    unsigned int __st_ino;
    unsigned int st_mode;
    unsigned int st_nlink;
    unsigned int st_uid;
    unsigned int st_gid;
    long long unsigned int st_rdev;
    unsigned char __pad3[4];
    long long int st_size;
    unsigned int st_blksize;
    long long int st_blocks;
    unsigned int st_atime;
    unsigned int st_atime_nsec;
    unsigned int st_mtime;
    unsigned int st_mtime_nsec;
    unsigned int st_ctime;
    unsigned int st_ctime_nsec;
    long long unsigned int st_ino;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct stat64 {
    long long unsigned int st_dev;
    unsigned char __pad0[4];
    unsigned int __st_ino;
    unsigned int st_mode;
    unsigned int st_nlink;
    unsigned int st_uid;
    unsigned int st_gid;
    long long unsigned int st_rdev;
    unsigned char __pad3[4];
    long long int st_size;
    unsigned int st_blksize;
    long long int st_blocks;
    unsigned int st_atime;
    unsigned int st_atime_nsec;
    unsigned int st_mtime;
    unsigned int st_mtime_nsec;
    unsigned int st_ctime;
    unsigned int st_ctime_nsec;
    long long unsigned int st_ino;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct stat64 {
    long long unsigned int st_dev;
    unsigned char __pad0[4];
    unsigned int __st_ino;
    unsigned int st_mode;
    unsigned int st_nlink;
    unsigned int st_uid;
    unsigned int st_gid;
    long long unsigned int st_rdev;
    unsigned char __pad3[4];
    long long int st_size;
    unsigned int st_blksize;
    long long int st_blocks;
    unsigned int st_atime;
    unsigned int st_atime_nsec;
    unsigned int st_mtime;
    unsigned int st_mtime_nsec;
    unsigned int st_ctime;
    unsigned int st_ctime_nsec;
    long long unsigned int st_ino;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct stat64 {
    long long unsigned int st_dev;
    unsigned char __pad0[4];
    unsigned int __st_ino;
    unsigned int st_mode;
    unsigned int st_nlink;
    unsigned int st_uid;
    unsigned int st_gid;
    long long unsigned int st_rdev;
    unsigned char __pad3[4];
    long long int st_size;
    unsigned int st_blksize;
    long long int st_blocks;
    unsigned int st_atime;
    unsigned int st_atime_nsec;
    unsigned int st_mtime;
    unsigned int st_mtime_nsec;
    unsigned int st_ctime;
    unsigned int st_ctime_nsec;
    long long unsigned int st_ino;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct stat64 {
    long long unsigned int st_dev;
    unsigned char __pad0[4];
    unsigned int __st_ino;
    unsigned int st_mode;
    unsigned int st_nlink;
    unsigned int st_uid;
    unsigned int st_gid;
    long long unsigned int st_rdev;
    unsigned char __pad3[4];
    long long int st_size;
    unsigned int st_blksize;
    long long int st_blocks;
    unsigned int st_atime;
    unsigned int st_atime_nsec;
    unsigned int st_mtime;
    unsigned int st_mtime_nsec;
    unsigned int st_ctime;
    unsigned int st_ctime_nsec;
    long long unsigned int st_ino;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct stat64 {
    long long unsigned int st_dev;
    unsigned char __pad0[4];
    unsigned int __st_ino;
    unsigned int st_mode;
    unsigned int st_nlink;
    unsigned int st_uid;
    unsigned int st_gid;
    long long unsigned int st_rdev;
    unsigned char __pad3[4];
    long long int st_size;
    unsigned int st_blksize;
    long long int st_blocks;
    unsigned int st_atime;
    unsigned int st_atime_nsec;
    unsigned int st_mtime;
    unsigned int st_mtime_nsec;
    unsigned int st_ctime;
    unsigned int st_ctime_nsec;
    long long unsigned int st_ino;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct stat64 {
    long long unsigned int st_dev;
    unsigned char __pad0[4];
    unsigned int __st_ino;
    unsigned int st_mode;
    unsigned int st_nlink;
    unsigned int st_uid;
    unsigned int st_gid;
    long long unsigned int st_rdev;
    unsigned char __pad3[4];
    long long int st_size;
    unsigned int st_blksize;
    long long int st_blocks;
    unsigned int st_atime;
    unsigned int st_atime_nsec;
    unsigned int st_mtime;
    unsigned int st_mtime_nsec;
    unsigned int st_ctime;
    unsigned int st_ctime_nsec;
    long long unsigned int st_ino;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct stat64 {
    long long unsigned int st_dev;
    unsigned char __pad0[4];
    unsigned int __st_ino;
    unsigned int st_mode;
    unsigned int st_nlink;
    unsigned int st_uid;
    unsigned int st_gid;
    long long unsigned int st_rdev;
    unsigned char __pad3[4];
    long long int st_size;
    unsigned int st_blksize;
    long long int st_blocks;
    unsigned int st_atime;
    unsigned int st_atime_nsec;
    unsigned int st_mtime;
    unsigned int st_mtime_nsec;
    unsigned int st_ctime;
    unsigned int st_ctime_nsec;
    long long unsigned int st_ino;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct stat64 {
    long long unsigned int st_dev;
    unsigned char __pad0[4];
    unsigned int __st_ino;
    unsigned int st_mode;
    unsigned int st_nlink;
    unsigned int st_uid;
    unsigned int st_gid;
    long long unsigned int st_rdev;
    unsigned char __pad3[4];
    long long int st_size;
    unsigned int st_blksize;
    long long int st_blocks;
    unsigned int st_atime;
    unsigned int st_atime_nsec;
    unsigned int st_mtime;
    unsigned int st_mtime_nsec;
    unsigned int st_ctime;
    unsigned int st_ctime_nsec;
    long long unsigned int st_ino;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct stat64 {
    long long unsigned int st_dev;
    unsigned char __pad0[4];
    unsigned int __st_ino;
    unsigned int st_mode;
    unsigned int st_nlink;
    unsigned int st_uid;
    unsigned int st_gid;
    long long unsigned int st_rdev;
    unsigned char __pad3[4];
    long long int st_size;
    unsigned int st_blksize;
    long long int st_blocks;
    unsigned int st_atime;
    unsigned int st_atime_nsec;
    unsigned int st_mtime;
    unsigned int st_mtime_nsec;
    unsigned int st_ctime;
    unsigned int st_ctime_nsec;
    long long unsigned int st_ino;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct stat64 {
    long long unsigned int st_dev;
    unsigned char __pad0[4];
    unsigned int __st_ino;
    unsigned int st_mode;
    unsigned int st_nlink;
    unsigned int st_uid;
    unsigned int st_gid;
    long long unsigned int st_rdev;
    unsigned char __pad3[4];
    long long int st_size;
    unsigned int st_blksize;
    long long int st_blocks;
    unsigned int st_atime;
    unsigned int st_atime_nsec;
    unsigned int st_mtime;
    unsigned int st_mtime_nsec;
    unsigned int st_ctime;
    unsigned int st_ctime_nsec;
    long long unsigned int st_ino;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct stat64 {
    long long unsigned int st_dev;
    unsigned char __pad0[4];
    unsigned int __st_ino;
    unsigned int st_mode;
    unsigned int st_nlink;
    unsigned int st_uid;
    unsigned int st_gid;
    long long unsigned int st_rdev;
    unsigned char __pad3[4];
    long long int st_size;
    unsigned int st_blksize;
    long long int st_blocks;
    unsigned int st_atime;
    unsigned int st_atime_nsec;
    unsigned int st_mtime;
    unsigned int st_mtime_nsec;
    unsigned int st_ctime;
    unsigned int st_ctime_nsec;
    long long unsigned int st_ino;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct stat64 {
    long long unsigned int st_dev;
    unsigned char __pad0[4];
    unsigned int __st_ino;
    unsigned int st_mode;
    unsigned int st_nlink;
    unsigned int st_uid;
    unsigned int st_gid;
    long long unsigned int st_rdev;
    unsigned char __pad3[4];
    long long int st_size;
    unsigned int st_blksize;
    long long int st_blocks;
    unsigned int st_atime;
    unsigned int st_atime_nsec;
    unsigned int st_mtime;
    unsigned int st_mtime_nsec;
    unsigned int st_ctime;
    unsigned int st_ctime_nsec;
    long long unsigned int st_ino;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct stat64 {
    long long unsigned int st_dev;
    unsigned char __pad0[4];
    unsigned int __st_ino;
    unsigned int st_mode;
    unsigned int st_nlink;
    unsigned int st_uid;
    unsigned int st_gid;
    long long unsigned int st_rdev;
    unsigned char __pad3[4];
    long long int st_size;
    unsigned int st_blksize;
    long long int st_blocks;
    unsigned int st_atime;
    unsigned int st_atime_nsec;
    unsigned int st_mtime;
    unsigned int st_mtime_nsec;
    unsigned int st_ctime;
    unsigned int st_ctime_nsec;
    long long unsigned int st_ino;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct stat64 {
    long long unsigned int st_dev;
    unsigned char __pad0[4];
    unsigned int __st_ino;
    unsigned int st_mode;
    unsigned int st_nlink;
    unsigned int st_uid;
    unsigned int st_gid;
    long long unsigned int st_rdev;
    unsigned char __pad3[4];
    long long int st_size;
    unsigned int st_blksize;
    long long int st_blocks;
    unsigned int st_atime;
    unsigned int st_atime_nsec;
    unsigned int st_mtime;
    unsigned int st_mtime_nsec;
    unsigned int st_ctime;
    unsigned int st_ctime_nsec;
    long long unsigned int st_ino;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct stat64 {
    long long unsigned int st_dev;
    unsigned char __pad0[4];
    unsigned int __st_ino;
    unsigned int st_mode;
    unsigned int st_nlink;
    unsigned int st_uid;
    unsigned int st_gid;
    long long unsigned int st_rdev;
    unsigned char __pad3[4];
    long long int st_size;
    unsigned int st_blksize;
    long long int st_blocks;
    unsigned int st_atime;
    unsigned int st_atime_nsec;
    unsigned int st_mtime;
    unsigned int st_mtime_nsec;
    unsigned int st_ctime;
    unsigned int st_ctime_nsec;
    long long unsigned int st_ino;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct stat64 {
    long long unsigned int st_dev;
    unsigned char __pad0[4];
    unsigned int __st_ino;
    unsigned int st_mode;
    unsigned int st_nlink;
    unsigned int st_uid;
    unsigned int st_gid;
    long long unsigned int st_rdev;
    unsigned char __pad3[4];
    long long int st_size;
    unsigned int st_blksize;
    long long int st_blocks;
    unsigned int st_atime;
    unsigned int st_atime_nsec;
    unsigned int st_mtime;
    unsigned int st_mtime_nsec;
    unsigned int st_ctime;
    unsigned int st_ctime_nsec;
    long long unsigned int st_ino;
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
struct stat64 {
    compat_u64 st_dev;
    unsigned char __pad0[4];
    compat_ulong_t __st_ino;
    compat_uint_t st_mode;
    compat_uint_t st_nlink;
    compat_ulong_t st_uid;
    compat_ulong_t st_gid;
    compat_u64 st_rdev;
    unsigned char __pad3[4];
    compat_s64 st_size;
    compat_ulong_t st_blksize;
    compat_u64 st_blocks;
    compat_ulong_t st_atime;
    compat_ulong_t st_atime_nsec;
    compat_ulong_t st_mtime;
    compat_ulong_t st_mtime_nsec;
    compat_ulong_t st_ctime;
    compat_ulong_t st_ctime_nsec;
    compat_u64 st_ino;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct stat64 {
    long long unsigned int st_dev;
    unsigned char __pad0[4];
    long unsigned int __st_ino;
    unsigned int st_mode;
    unsigned int st_nlink;
    long unsigned int st_uid;
    long unsigned int st_gid;
    long long unsigned int st_rdev;
    unsigned char __pad3[4];
    long long int st_size;
    long unsigned int st_blksize;
    long long unsigned int st_blocks;
    long unsigned int st_atime;
    long unsigned int st_atime_nsec;
    long unsigned int st_mtime;
    long unsigned int st_mtime_nsec;
    long unsigned int st_ctime;
    long unsigned int st_ctime_nsec;
    long long unsigned int st_ino;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct stat64 {
    long long unsigned int st_dev;
    long long unsigned int st_ino;
    unsigned int st_mode;
    unsigned int st_nlink;
    unsigned int st_uid;
    unsigned int st_gid;
    long long unsigned int st_rdev;
    short unsigned int __pad2;
    long long int st_size;
    int st_blksize;
    long long int st_blocks;
    int st_atime;
    unsigned int st_atime_nsec;
    int st_mtime;
    unsigned int st_mtime_nsec;
    int st_ctime;
    unsigned int st_ctime_nsec;
    unsigned int __unused4;
    unsigned int __unused5;
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
struct stat64 {
    long long unsigned int st_dev;
    unsigned char __pad0[4];
    unsigned int __st_ino;
    unsigned int st_mode;
    unsigned int st_nlink;
    unsigned int st_uid;
    unsigned int st_gid;
    long long unsigned int st_rdev;
    unsigned char __pad3[4];
    long long int st_size;
    unsigned int st_blksize;
    long long int st_blocks;
    unsigned int st_atime;
    unsigned int st_atime_nsec;
    unsigned int st_mtime;
    unsigned int st_mtime_nsec;
    unsigned int st_ctime;
    unsigned int st_ctime_nsec;
    long long unsigned int st_ino;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct stat64 {
    long long unsigned int st_dev;
    unsigned char __pad0[4];
    unsigned int __st_ino;
    unsigned int st_mode;
    unsigned int st_nlink;
    unsigned int st_uid;
    unsigned int st_gid;
    long long unsigned int st_rdev;
    unsigned char __pad3[4];
    long long int st_size;
    unsigned int st_blksize;
    long long int st_blocks;
    unsigned int st_atime;
    unsigned int st_atime_nsec;
    unsigned int st_mtime;
    unsigned int st_mtime_nsec;
    unsigned int st_ctime;
    unsigned int st_ctime_nsec;
    long long unsigned int st_ino;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct stat64 {
    long long unsigned int st_dev;
    unsigned char __pad0[4];
    unsigned int __st_ino;
    unsigned int st_mode;
    unsigned int st_nlink;
    unsigned int st_uid;
    unsigned int st_gid;
    long long unsigned int st_rdev;
    unsigned char __pad3[4];
    long long int st_size;
    unsigned int st_blksize;
    long long int st_blocks;
    unsigned int st_atime;
    unsigned int st_atime_nsec;
    unsigned int st_mtime;
    unsigned int st_mtime_nsec;
    unsigned int st_ctime;
    unsigned int st_ctime_nsec;
    long long unsigned int st_ino;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct stat64 {
    long long unsigned int st_dev;
    unsigned char __pad0[4];
    unsigned int __st_ino;
    unsigned int st_mode;
    unsigned int st_nlink;
    unsigned int st_uid;
    unsigned int st_gid;
    long long unsigned int st_rdev;
    unsigned char __pad3[4];
    long long int st_size;
    unsigned int st_blksize;
    long long int st_blocks;
    unsigned int st_atime;
    unsigned int st_atime_nsec;
    unsigned int st_mtime;
    unsigned int st_mtime_nsec;
    unsigned int st_ctime;
    unsigned int st_ctime_nsec;
    long long unsigned int st_ino;
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
<details>
<summary>Changed between <code>amd64</code> and <code>arm64</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long long unsigned int st_dev</code> ➡️ <code>compat_u64 st_dev</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int __st_ino</code> ➡️ <code>compat_ulong_t __st_ino</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int st_mode</code> ➡️ <code>compat_uint_t st_mode</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int st_nlink</code> ➡️ <code>compat_uint_t st_nlink</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int st_uid</code> ➡️ <code>compat_ulong_t st_uid</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int st_gid</code> ➡️ <code>compat_ulong_t st_gid</code>
</li>
<li>
<b>Field type changed. </b>
<code>long long unsigned int st_rdev</code> ➡️ <code>compat_u64 st_rdev</code>
</li>
<li>
<b>Field type changed. </b>
<code>long long int st_size</code> ➡️ <code>compat_s64 st_size</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int st_blksize</code> ➡️ <code>compat_ulong_t st_blksize</code>
</li>
<li>
<b>Field type changed. </b>
<code>long long int st_blocks</code> ➡️ <code>compat_u64 st_blocks</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int st_atime</code> ➡️ <code>compat_ulong_t st_atime</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int st_atime_nsec</code> ➡️ <code>compat_ulong_t st_atime_nsec</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int st_mtime</code> ➡️ <code>compat_ulong_t st_mtime</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int st_mtime_nsec</code> ➡️ <code>compat_ulong_t st_mtime_nsec</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int st_ctime</code> ➡️ <code>compat_ulong_t st_ctime</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int st_ctime_nsec</code> ➡️ <code>compat_ulong_t st_ctime_nsec</code>
</li>
<li>
<b>Field type changed. </b>
<code>long long unsigned int st_ino</code> ➡️ <code>compat_u64 st_ino</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>unsigned int __st_ino</code> ➡️ <code>long unsigned int __st_ino</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int st_uid</code> ➡️ <code>long unsigned int st_uid</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int st_gid</code> ➡️ <code>long unsigned int st_gid</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int st_blksize</code> ➡️ <code>long unsigned int st_blksize</code>
</li>
<li>
<b>Field type changed. </b>
<code>long long int st_blocks</code> ➡️ <code>long long unsigned int st_blocks</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int st_atime</code> ➡️ <code>long unsigned int st_atime</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int st_atime_nsec</code> ➡️ <code>long unsigned int st_atime_nsec</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int st_mtime</code> ➡️ <code>long unsigned int st_mtime</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int st_mtime_nsec</code> ➡️ <code>long unsigned int st_mtime_nsec</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int st_ctime</code> ➡️ <code>long unsigned int st_ctime</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int st_ctime_nsec</code> ➡️ <code>long unsigned int st_ctime_nsec</code>
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
<code>short unsigned int __pad2</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int __unused4</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int __unused5</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned char __pad0[4]</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int __st_ino</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned char __pad3[4]</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int st_blksize</code> ➡️ <code>int st_blksize</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int st_atime</code> ➡️ <code>int st_atime</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int st_mtime</code> ➡️ <code>int st_mtime</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int st_ctime</code> ➡️ <code>int st_ctime</code>
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
