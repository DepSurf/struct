# Struct: <code>statx</code>

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
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct statx {
    __u32 stx_mask;
    __u32 stx_blksize;
    __u64 stx_attributes;
    __u32 stx_nlink;
    __u32 stx_uid;
    __u32 stx_gid;
    __u16 stx_mode;
    __u16 __spare0[1];
    __u64 stx_ino;
    __u64 stx_size;
    __u64 stx_blocks;
    __u64 stx_attributes_mask;
    struct statx_timestamp stx_atime;
    struct statx_timestamp stx_btime;
    struct statx_timestamp stx_ctime;
    struct statx_timestamp stx_mtime;
    __u32 stx_rdev_major;
    __u32 stx_rdev_minor;
    __u32 stx_dev_major;
    __u32 stx_dev_minor;
    __u64 __spare2[14];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct statx {
    __u32 stx_mask;
    __u32 stx_blksize;
    __u64 stx_attributes;
    __u32 stx_nlink;
    __u32 stx_uid;
    __u32 stx_gid;
    __u16 stx_mode;
    __u16 __spare0[1];
    __u64 stx_ino;
    __u64 stx_size;
    __u64 stx_blocks;
    __u64 stx_attributes_mask;
    struct statx_timestamp stx_atime;
    struct statx_timestamp stx_btime;
    struct statx_timestamp stx_ctime;
    struct statx_timestamp stx_mtime;
    __u32 stx_rdev_major;
    __u32 stx_rdev_minor;
    __u32 stx_dev_major;
    __u32 stx_dev_minor;
    __u64 __spare2[14];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct statx {
    __u32 stx_mask;
    __u32 stx_blksize;
    __u64 stx_attributes;
    __u32 stx_nlink;
    __u32 stx_uid;
    __u32 stx_gid;
    __u16 stx_mode;
    __u16 __spare0[1];
    __u64 stx_ino;
    __u64 stx_size;
    __u64 stx_blocks;
    __u64 stx_attributes_mask;
    struct statx_timestamp stx_atime;
    struct statx_timestamp stx_btime;
    struct statx_timestamp stx_ctime;
    struct statx_timestamp stx_mtime;
    __u32 stx_rdev_major;
    __u32 stx_rdev_minor;
    __u32 stx_dev_major;
    __u32 stx_dev_minor;
    __u64 __spare2[14];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct statx {
    __u32 stx_mask;
    __u32 stx_blksize;
    __u64 stx_attributes;
    __u32 stx_nlink;
    __u32 stx_uid;
    __u32 stx_gid;
    __u16 stx_mode;
    __u16 __spare0[1];
    __u64 stx_ino;
    __u64 stx_size;
    __u64 stx_blocks;
    __u64 stx_attributes_mask;
    struct statx_timestamp stx_atime;
    struct statx_timestamp stx_btime;
    struct statx_timestamp stx_ctime;
    struct statx_timestamp stx_mtime;
    __u32 stx_rdev_major;
    __u32 stx_rdev_minor;
    __u32 stx_dev_major;
    __u32 stx_dev_minor;
    __u64 __spare2[14];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct statx {
    __u32 stx_mask;
    __u32 stx_blksize;
    __u64 stx_attributes;
    __u32 stx_nlink;
    __u32 stx_uid;
    __u32 stx_gid;
    __u16 stx_mode;
    __u16 __spare0[1];
    __u64 stx_ino;
    __u64 stx_size;
    __u64 stx_blocks;
    __u64 stx_attributes_mask;
    struct statx_timestamp stx_atime;
    struct statx_timestamp stx_btime;
    struct statx_timestamp stx_ctime;
    struct statx_timestamp stx_mtime;
    __u32 stx_rdev_major;
    __u32 stx_rdev_minor;
    __u32 stx_dev_major;
    __u32 stx_dev_minor;
    __u64 __spare2[14];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct statx {
    __u32 stx_mask;
    __u32 stx_blksize;
    __u64 stx_attributes;
    __u32 stx_nlink;
    __u32 stx_uid;
    __u32 stx_gid;
    __u16 stx_mode;
    __u16 __spare0[1];
    __u64 stx_ino;
    __u64 stx_size;
    __u64 stx_blocks;
    __u64 stx_attributes_mask;
    struct statx_timestamp stx_atime;
    struct statx_timestamp stx_btime;
    struct statx_timestamp stx_ctime;
    struct statx_timestamp stx_mtime;
    __u32 stx_rdev_major;
    __u32 stx_rdev_minor;
    __u32 stx_dev_major;
    __u32 stx_dev_minor;
    __u64 __spare2[14];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct statx {
    __u32 stx_mask;
    __u32 stx_blksize;
    __u64 stx_attributes;
    __u32 stx_nlink;
    __u32 stx_uid;
    __u32 stx_gid;
    __u16 stx_mode;
    __u16 __spare0[1];
    __u64 stx_ino;
    __u64 stx_size;
    __u64 stx_blocks;
    __u64 stx_attributes_mask;
    struct statx_timestamp stx_atime;
    struct statx_timestamp stx_btime;
    struct statx_timestamp stx_ctime;
    struct statx_timestamp stx_mtime;
    __u32 stx_rdev_major;
    __u32 stx_rdev_minor;
    __u32 stx_dev_major;
    __u32 stx_dev_minor;
    __u64 stx_mnt_id;
    __u64 __spare2;
    __u64 __spare3[12];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct statx {
    __u32 stx_mask;
    __u32 stx_blksize;
    __u64 stx_attributes;
    __u32 stx_nlink;
    __u32 stx_uid;
    __u32 stx_gid;
    __u16 stx_mode;
    __u16 __spare0[1];
    __u64 stx_ino;
    __u64 stx_size;
    __u64 stx_blocks;
    __u64 stx_attributes_mask;
    struct statx_timestamp stx_atime;
    struct statx_timestamp stx_btime;
    struct statx_timestamp stx_ctime;
    struct statx_timestamp stx_mtime;
    __u32 stx_rdev_major;
    __u32 stx_rdev_minor;
    __u32 stx_dev_major;
    __u32 stx_dev_minor;
    __u64 stx_mnt_id;
    __u64 __spare2;
    __u64 __spare3[12];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct statx {
    __u32 stx_mask;
    __u32 stx_blksize;
    __u64 stx_attributes;
    __u32 stx_nlink;
    __u32 stx_uid;
    __u32 stx_gid;
    __u16 stx_mode;
    __u16 __spare0[1];
    __u64 stx_ino;
    __u64 stx_size;
    __u64 stx_blocks;
    __u64 stx_attributes_mask;
    struct statx_timestamp stx_atime;
    struct statx_timestamp stx_btime;
    struct statx_timestamp stx_ctime;
    struct statx_timestamp stx_mtime;
    __u32 stx_rdev_major;
    __u32 stx_rdev_minor;
    __u32 stx_dev_major;
    __u32 stx_dev_minor;
    __u64 stx_mnt_id;
    __u64 __spare2;
    __u64 __spare3[12];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct statx {
    __u32 stx_mask;
    __u32 stx_blksize;
    __u64 stx_attributes;
    __u32 stx_nlink;
    __u32 stx_uid;
    __u32 stx_gid;
    __u16 stx_mode;
    __u16 __spare0[1];
    __u64 stx_ino;
    __u64 stx_size;
    __u64 stx_blocks;
    __u64 stx_attributes_mask;
    struct statx_timestamp stx_atime;
    struct statx_timestamp stx_btime;
    struct statx_timestamp stx_ctime;
    struct statx_timestamp stx_mtime;
    __u32 stx_rdev_major;
    __u32 stx_rdev_minor;
    __u32 stx_dev_major;
    __u32 stx_dev_minor;
    __u64 stx_mnt_id;
    __u64 __spare2;
    __u64 __spare3[12];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct statx {
    __u32 stx_mask;
    __u32 stx_blksize;
    __u64 stx_attributes;
    __u32 stx_nlink;
    __u32 stx_uid;
    __u32 stx_gid;
    __u16 stx_mode;
    __u16 __spare0[1];
    __u64 stx_ino;
    __u64 stx_size;
    __u64 stx_blocks;
    __u64 stx_attributes_mask;
    struct statx_timestamp stx_atime;
    struct statx_timestamp stx_btime;
    struct statx_timestamp stx_ctime;
    struct statx_timestamp stx_mtime;
    __u32 stx_rdev_major;
    __u32 stx_rdev_minor;
    __u32 stx_dev_major;
    __u32 stx_dev_minor;
    __u64 stx_mnt_id;
    __u64 __spare2;
    __u64 __spare3[12];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct statx {
    __u32 stx_mask;
    __u32 stx_blksize;
    __u64 stx_attributes;
    __u32 stx_nlink;
    __u32 stx_uid;
    __u32 stx_gid;
    __u16 stx_mode;
    __u16 __spare0[1];
    __u64 stx_ino;
    __u64 stx_size;
    __u64 stx_blocks;
    __u64 stx_attributes_mask;
    struct statx_timestamp stx_atime;
    struct statx_timestamp stx_btime;
    struct statx_timestamp stx_ctime;
    struct statx_timestamp stx_mtime;
    __u32 stx_rdev_major;
    __u32 stx_rdev_minor;
    __u32 stx_dev_major;
    __u32 stx_dev_minor;
    __u64 stx_mnt_id;
    __u32 stx_dio_mem_align;
    __u32 stx_dio_offset_align;
    __u64 __spare3[12];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct statx {
    __u32 stx_mask;
    __u32 stx_blksize;
    __u64 stx_attributes;
    __u32 stx_nlink;
    __u32 stx_uid;
    __u32 stx_gid;
    __u16 stx_mode;
    __u16 __spare0[1];
    __u64 stx_ino;
    __u64 stx_size;
    __u64 stx_blocks;
    __u64 stx_attributes_mask;
    struct statx_timestamp stx_atime;
    struct statx_timestamp stx_btime;
    struct statx_timestamp stx_ctime;
    struct statx_timestamp stx_mtime;
    __u32 stx_rdev_major;
    __u32 stx_rdev_minor;
    __u32 stx_dev_major;
    __u32 stx_dev_minor;
    __u64 stx_mnt_id;
    __u32 stx_dio_mem_align;
    __u32 stx_dio_offset_align;
    __u64 __spare3[12];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct statx {
    __u32 stx_mask;
    __u32 stx_blksize;
    __u64 stx_attributes;
    __u32 stx_nlink;
    __u32 stx_uid;
    __u32 stx_gid;
    __u16 stx_mode;
    __u16 __spare0[1];
    __u64 stx_ino;
    __u64 stx_size;
    __u64 stx_blocks;
    __u64 stx_attributes_mask;
    struct statx_timestamp stx_atime;
    struct statx_timestamp stx_btime;
    struct statx_timestamp stx_ctime;
    struct statx_timestamp stx_mtime;
    __u32 stx_rdev_major;
    __u32 stx_rdev_minor;
    __u32 stx_dev_major;
    __u32 stx_dev_minor;
    __u64 stx_mnt_id;
    __u32 stx_dio_mem_align;
    __u32 stx_dio_offset_align;
    __u64 __spare3[12];
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
struct statx {
    __u32 stx_mask;
    __u32 stx_blksize;
    __u64 stx_attributes;
    __u32 stx_nlink;
    __u32 stx_uid;
    __u32 stx_gid;
    __u16 stx_mode;
    __u16 __spare0[1];
    __u64 stx_ino;
    __u64 stx_size;
    __u64 stx_blocks;
    __u64 stx_attributes_mask;
    struct statx_timestamp stx_atime;
    struct statx_timestamp stx_btime;
    struct statx_timestamp stx_ctime;
    struct statx_timestamp stx_mtime;
    __u32 stx_rdev_major;
    __u32 stx_rdev_minor;
    __u32 stx_dev_major;
    __u32 stx_dev_minor;
    __u64 __spare2[14];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct statx {
    __u32 stx_mask;
    __u32 stx_blksize;
    __u64 stx_attributes;
    __u32 stx_nlink;
    __u32 stx_uid;
    __u32 stx_gid;
    __u16 stx_mode;
    __u16 __spare0[1];
    __u64 stx_ino;
    __u64 stx_size;
    __u64 stx_blocks;
    __u64 stx_attributes_mask;
    struct statx_timestamp stx_atime;
    struct statx_timestamp stx_btime;
    struct statx_timestamp stx_ctime;
    struct statx_timestamp stx_mtime;
    __u32 stx_rdev_major;
    __u32 stx_rdev_minor;
    __u32 stx_dev_major;
    __u32 stx_dev_minor;
    __u64 __spare2[14];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct statx {
    __u32 stx_mask;
    __u32 stx_blksize;
    __u64 stx_attributes;
    __u32 stx_nlink;
    __u32 stx_uid;
    __u32 stx_gid;
    __u16 stx_mode;
    __u16 __spare0[1];
    __u64 stx_ino;
    __u64 stx_size;
    __u64 stx_blocks;
    __u64 stx_attributes_mask;
    struct statx_timestamp stx_atime;
    struct statx_timestamp stx_btime;
    struct statx_timestamp stx_ctime;
    struct statx_timestamp stx_mtime;
    __u32 stx_rdev_major;
    __u32 stx_rdev_minor;
    __u32 stx_dev_major;
    __u32 stx_dev_minor;
    __u64 __spare2[14];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct statx {
    __u32 stx_mask;
    __u32 stx_blksize;
    __u64 stx_attributes;
    __u32 stx_nlink;
    __u32 stx_uid;
    __u32 stx_gid;
    __u16 stx_mode;
    __u16 __spare0[1];
    __u64 stx_ino;
    __u64 stx_size;
    __u64 stx_blocks;
    __u64 stx_attributes_mask;
    struct statx_timestamp stx_atime;
    struct statx_timestamp stx_btime;
    struct statx_timestamp stx_ctime;
    struct statx_timestamp stx_mtime;
    __u32 stx_rdev_major;
    __u32 stx_rdev_minor;
    __u32 stx_dev_major;
    __u32 stx_dev_minor;
    __u64 __spare2[14];
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
struct statx {
    __u32 stx_mask;
    __u32 stx_blksize;
    __u64 stx_attributes;
    __u32 stx_nlink;
    __u32 stx_uid;
    __u32 stx_gid;
    __u16 stx_mode;
    __u16 __spare0[1];
    __u64 stx_ino;
    __u64 stx_size;
    __u64 stx_blocks;
    __u64 stx_attributes_mask;
    struct statx_timestamp stx_atime;
    struct statx_timestamp stx_btime;
    struct statx_timestamp stx_ctime;
    struct statx_timestamp stx_mtime;
    __u32 stx_rdev_major;
    __u32 stx_rdev_minor;
    __u32 stx_dev_major;
    __u32 stx_dev_minor;
    __u64 __spare2[14];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct statx {
    __u32 stx_mask;
    __u32 stx_blksize;
    __u64 stx_attributes;
    __u32 stx_nlink;
    __u32 stx_uid;
    __u32 stx_gid;
    __u16 stx_mode;
    __u16 __spare0[1];
    __u64 stx_ino;
    __u64 stx_size;
    __u64 stx_blocks;
    __u64 stx_attributes_mask;
    struct statx_timestamp stx_atime;
    struct statx_timestamp stx_btime;
    struct statx_timestamp stx_ctime;
    struct statx_timestamp stx_mtime;
    __u32 stx_rdev_major;
    __u32 stx_rdev_minor;
    __u32 stx_dev_major;
    __u32 stx_dev_minor;
    __u64 __spare2[14];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct statx {
    __u32 stx_mask;
    __u32 stx_blksize;
    __u64 stx_attributes;
    __u32 stx_nlink;
    __u32 stx_uid;
    __u32 stx_gid;
    __u16 stx_mode;
    __u16 __spare0[1];
    __u64 stx_ino;
    __u64 stx_size;
    __u64 stx_blocks;
    __u64 stx_attributes_mask;
    struct statx_timestamp stx_atime;
    struct statx_timestamp stx_btime;
    struct statx_timestamp stx_ctime;
    struct statx_timestamp stx_mtime;
    __u32 stx_rdev_major;
    __u32 stx_rdev_minor;
    __u32 stx_dev_major;
    __u32 stx_dev_minor;
    __u64 __spare2[14];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct statx {
    __u32 stx_mask;
    __u32 stx_blksize;
    __u64 stx_attributes;
    __u32 stx_nlink;
    __u32 stx_uid;
    __u32 stx_gid;
    __u16 stx_mode;
    __u16 __spare0[1];
    __u64 stx_ino;
    __u64 stx_size;
    __u64 stx_blocks;
    __u64 stx_attributes_mask;
    struct statx_timestamp stx_atime;
    struct statx_timestamp stx_btime;
    struct statx_timestamp stx_ctime;
    struct statx_timestamp stx_mtime;
    __u32 stx_rdev_major;
    __u32 stx_rdev_minor;
    __u32 stx_dev_major;
    __u32 stx_dev_minor;
    __u64 __spare2[14];
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
<b>Field added. </b>
<code>__u64 stx_mnt_id</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 __spare3[12]</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u64 __spare2[14]</code> ➡️ <code>__u64 __spare2</code>
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
<code>__u32 stx_dio_mem_align</code>
</li>
<li>
<b>Field added. </b>
<code>__u32 stx_dio_offset_align</code>
</li>
<li>
<b>Field removed. </b>
<code>__u64 __spare2</code>
</li>
</ul>
</details>
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
