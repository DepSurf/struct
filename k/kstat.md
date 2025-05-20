# Struct: <code>kstat</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct kstat {
    u64 ino;
    dev_t dev;
    umode_t mode;
    unsigned int nlink;
    kuid_t uid;
    kgid_t gid;
    dev_t rdev;
    loff_t size;
    struct timespec atime;
    struct timespec mtime;
    struct timespec ctime;
    long unsigned int blksize;
    long long unsigned int blocks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct kstat {
    u64 ino;
    dev_t dev;
    umode_t mode;
    unsigned int nlink;
    kuid_t uid;
    kgid_t gid;
    dev_t rdev;
    loff_t size;
    struct timespec atime;
    struct timespec mtime;
    struct timespec ctime;
    long unsigned int blksize;
    long long unsigned int blocks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct kstat {
    u64 ino;
    dev_t dev;
    umode_t mode;
    unsigned int nlink;
    kuid_t uid;
    kgid_t gid;
    dev_t rdev;
    loff_t size;
    struct timespec atime;
    struct timespec mtime;
    struct timespec ctime;
    long unsigned int blksize;
    long long unsigned int blocks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct kstat {
    u32 result_mask;
    umode_t mode;
    unsigned int nlink;
    uint32_t blksize;
    u64 attributes;
    u64 attributes_mask;
    u64 ino;
    dev_t dev;
    dev_t rdev;
    kuid_t uid;
    kgid_t gid;
    loff_t size;
    struct timespec atime;
    struct timespec mtime;
    struct timespec ctime;
    struct timespec btime;
    u64 blocks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct kstat {
    u32 result_mask;
    umode_t mode;
    unsigned int nlink;
    uint32_t blksize;
    u64 attributes;
    u64 attributes_mask;
    u64 ino;
    dev_t dev;
    dev_t rdev;
    kuid_t uid;
    kgid_t gid;
    loff_t size;
    struct timespec atime;
    struct timespec mtime;
    struct timespec ctime;
    struct timespec btime;
    u64 blocks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct kstat {
    u32 result_mask;
    umode_t mode;
    unsigned int nlink;
    uint32_t blksize;
    u64 attributes;
    u64 attributes_mask;
    u64 ino;
    dev_t dev;
    dev_t rdev;
    kuid_t uid;
    kgid_t gid;
    loff_t size;
    struct timespec64 atime;
    struct timespec64 mtime;
    struct timespec64 ctime;
    struct timespec64 btime;
    u64 blocks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct kstat {
    u32 result_mask;
    umode_t mode;
    unsigned int nlink;
    uint32_t blksize;
    u64 attributes;
    u64 attributes_mask;
    u64 ino;
    dev_t dev;
    dev_t rdev;
    kuid_t uid;
    kgid_t gid;
    loff_t size;
    struct timespec64 atime;
    struct timespec64 mtime;
    struct timespec64 ctime;
    struct timespec64 btime;
    u64 blocks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct kstat {
    u32 result_mask;
    umode_t mode;
    unsigned int nlink;
    uint32_t blksize;
    u64 attributes;
    u64 attributes_mask;
    u64 ino;
    dev_t dev;
    dev_t rdev;
    kuid_t uid;
    kgid_t gid;
    loff_t size;
    struct timespec64 atime;
    struct timespec64 mtime;
    struct timespec64 ctime;
    struct timespec64 btime;
    u64 blocks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct kstat {
    u32 result_mask;
    umode_t mode;
    unsigned int nlink;
    uint32_t blksize;
    u64 attributes;
    u64 attributes_mask;
    u64 ino;
    dev_t dev;
    dev_t rdev;
    kuid_t uid;
    kgid_t gid;
    loff_t size;
    struct timespec64 atime;
    struct timespec64 mtime;
    struct timespec64 ctime;
    struct timespec64 btime;
    u64 blocks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct kstat {
    u32 result_mask;
    umode_t mode;
    unsigned int nlink;
    uint32_t blksize;
    u64 attributes;
    u64 attributes_mask;
    u64 ino;
    dev_t dev;
    dev_t rdev;
    kuid_t uid;
    kgid_t gid;
    loff_t size;
    struct timespec64 atime;
    struct timespec64 mtime;
    struct timespec64 ctime;
    struct timespec64 btime;
    u64 blocks;
    u64 mnt_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct kstat {
    u32 result_mask;
    umode_t mode;
    unsigned int nlink;
    uint32_t blksize;
    u64 attributes;
    u64 attributes_mask;
    u64 ino;
    dev_t dev;
    dev_t rdev;
    kuid_t uid;
    kgid_t gid;
    loff_t size;
    struct timespec64 atime;
    struct timespec64 mtime;
    struct timespec64 ctime;
    struct timespec64 btime;
    u64 blocks;
    u64 mnt_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kstat {
    u32 result_mask;
    umode_t mode;
    unsigned int nlink;
    uint32_t blksize;
    u64 attributes;
    u64 attributes_mask;
    u64 ino;
    dev_t dev;
    dev_t rdev;
    kuid_t uid;
    kgid_t gid;
    loff_t size;
    struct timespec64 atime;
    struct timespec64 mtime;
    struct timespec64 ctime;
    struct timespec64 btime;
    u64 blocks;
    u64 mnt_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kstat {
    u32 result_mask;
    umode_t mode;
    unsigned int nlink;
    uint32_t blksize;
    u64 attributes;
    u64 attributes_mask;
    u64 ino;
    dev_t dev;
    dev_t rdev;
    kuid_t uid;
    kgid_t gid;
    loff_t size;
    struct timespec64 atime;
    struct timespec64 mtime;
    struct timespec64 ctime;
    struct timespec64 btime;
    u64 blocks;
    u64 mnt_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kstat {
    u32 result_mask;
    umode_t mode;
    unsigned int nlink;
    uint32_t blksize;
    u64 attributes;
    u64 attributes_mask;
    u64 ino;
    dev_t dev;
    dev_t rdev;
    kuid_t uid;
    kgid_t gid;
    loff_t size;
    struct timespec64 atime;
    struct timespec64 mtime;
    struct timespec64 ctime;
    struct timespec64 btime;
    u64 blocks;
    u64 mnt_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kstat {
    u32 result_mask;
    umode_t mode;
    unsigned int nlink;
    uint32_t blksize;
    u64 attributes;
    u64 attributes_mask;
    u64 ino;
    dev_t dev;
    dev_t rdev;
    kuid_t uid;
    kgid_t gid;
    loff_t size;
    struct timespec64 atime;
    struct timespec64 mtime;
    struct timespec64 ctime;
    struct timespec64 btime;
    u64 blocks;
    u64 mnt_id;
    u32 dio_mem_align;
    u32 dio_offset_align;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kstat {
    u32 result_mask;
    umode_t mode;
    unsigned int nlink;
    uint32_t blksize;
    u64 attributes;
    u64 attributes_mask;
    u64 ino;
    dev_t dev;
    dev_t rdev;
    kuid_t uid;
    kgid_t gid;
    loff_t size;
    struct timespec64 atime;
    struct timespec64 mtime;
    struct timespec64 ctime;
    struct timespec64 btime;
    u64 blocks;
    u64 mnt_id;
    u32 dio_mem_align;
    u32 dio_offset_align;
    u64 change_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kstat {
    u32 result_mask;
    umode_t mode;
    unsigned int nlink;
    uint32_t blksize;
    u64 attributes;
    u64 attributes_mask;
    u64 ino;
    dev_t dev;
    dev_t rdev;
    kuid_t uid;
    kgid_t gid;
    loff_t size;
    struct timespec64 atime;
    struct timespec64 mtime;
    struct timespec64 ctime;
    struct timespec64 btime;
    u64 blocks;
    u64 mnt_id;
    u32 dio_mem_align;
    u32 dio_offset_align;
    u64 change_cookie;
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
struct kstat {
    u32 result_mask;
    umode_t mode;
    unsigned int nlink;
    uint32_t blksize;
    u64 attributes;
    u64 attributes_mask;
    u64 ino;
    dev_t dev;
    dev_t rdev;
    kuid_t uid;
    kgid_t gid;
    loff_t size;
    struct timespec64 atime;
    struct timespec64 mtime;
    struct timespec64 ctime;
    struct timespec64 btime;
    u64 blocks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct kstat {
    u32 result_mask;
    umode_t mode;
    unsigned int nlink;
    uint32_t blksize;
    u64 attributes;
    u64 attributes_mask;
    u64 ino;
    dev_t dev;
    dev_t rdev;
    kuid_t uid;
    kgid_t gid;
    loff_t size;
    struct timespec64 atime;
    struct timespec64 mtime;
    struct timespec64 ctime;
    struct timespec64 btime;
    u64 blocks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct kstat {
    u32 result_mask;
    umode_t mode;
    unsigned int nlink;
    uint32_t blksize;
    u64 attributes;
    u64 attributes_mask;
    u64 ino;
    dev_t dev;
    dev_t rdev;
    kuid_t uid;
    kgid_t gid;
    loff_t size;
    struct timespec64 atime;
    struct timespec64 mtime;
    struct timespec64 ctime;
    struct timespec64 btime;
    u64 blocks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct kstat {
    u32 result_mask;
    umode_t mode;
    unsigned int nlink;
    uint32_t blksize;
    u64 attributes;
    u64 attributes_mask;
    u64 ino;
    dev_t dev;
    dev_t rdev;
    kuid_t uid;
    kgid_t gid;
    loff_t size;
    struct timespec64 atime;
    struct timespec64 mtime;
    struct timespec64 ctime;
    struct timespec64 btime;
    u64 blocks;
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
struct kstat {
    u32 result_mask;
    umode_t mode;
    unsigned int nlink;
    uint32_t blksize;
    u64 attributes;
    u64 attributes_mask;
    u64 ino;
    dev_t dev;
    dev_t rdev;
    kuid_t uid;
    kgid_t gid;
    loff_t size;
    struct timespec64 atime;
    struct timespec64 mtime;
    struct timespec64 ctime;
    struct timespec64 btime;
    u64 blocks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct kstat {
    u32 result_mask;
    umode_t mode;
    unsigned int nlink;
    uint32_t blksize;
    u64 attributes;
    u64 attributes_mask;
    u64 ino;
    dev_t dev;
    dev_t rdev;
    kuid_t uid;
    kgid_t gid;
    loff_t size;
    struct timespec64 atime;
    struct timespec64 mtime;
    struct timespec64 ctime;
    struct timespec64 btime;
    u64 blocks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct kstat {
    u32 result_mask;
    umode_t mode;
    unsigned int nlink;
    uint32_t blksize;
    u64 attributes;
    u64 attributes_mask;
    u64 ino;
    dev_t dev;
    dev_t rdev;
    kuid_t uid;
    kgid_t gid;
    loff_t size;
    struct timespec64 atime;
    struct timespec64 mtime;
    struct timespec64 ctime;
    struct timespec64 btime;
    u64 blocks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct kstat {
    u32 result_mask;
    umode_t mode;
    unsigned int nlink;
    uint32_t blksize;
    u64 attributes;
    u64 attributes_mask;
    u64 ino;
    dev_t dev;
    dev_t rdev;
    kuid_t uid;
    kgid_t gid;
    loff_t size;
    struct timespec64 atime;
    struct timespec64 mtime;
    struct timespec64 ctime;
    struct timespec64 btime;
    u64 blocks;
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
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 result_mask</code>
</li>
<li>
<b>Field added. </b>
<code>u64 attributes</code>
</li>
<li>
<b>Field added. </b>
<code>u64 attributes_mask</code>
</li>
<li>
<b>Field added. </b>
<code>struct timespec btime</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int blksize</code> ➡️ <code>uint32_t blksize</code>
</li>
<li>
<b>Field type changed. </b>
<code>long long unsigned int blocks</code> ➡️ <code>u64 blocks</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct timespec atime</code> ➡️ <code>struct timespec64 atime</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct timespec mtime</code> ➡️ <code>struct timespec64 mtime</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct timespec ctime</code> ➡️ <code>struct timespec64 ctime</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct timespec btime</code> ➡️ <code>struct timespec64 btime</code>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 mnt_id</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 dio_mem_align</code>
</li>
<li>
<b>Field added. </b>
<code>u32 dio_offset_align</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 change_cookie</code>
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
