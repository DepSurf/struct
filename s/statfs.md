# Struct: <code>statfs</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct statfs {
    __kernel_long_t f_type;
    __kernel_long_t f_bsize;
    __kernel_long_t f_blocks;
    __kernel_long_t f_bfree;
    __kernel_long_t f_bavail;
    __kernel_long_t f_files;
    __kernel_long_t f_ffree;
    __kernel_fsid_t f_fsid;
    __kernel_long_t f_namelen;
    __kernel_long_t f_frsize;
    __kernel_long_t f_flags;
    __kernel_long_t f_spare[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct statfs {
    __kernel_long_t f_type;
    __kernel_long_t f_bsize;
    __kernel_long_t f_blocks;
    __kernel_long_t f_bfree;
    __kernel_long_t f_bavail;
    __kernel_long_t f_files;
    __kernel_long_t f_ffree;
    __kernel_fsid_t f_fsid;
    __kernel_long_t f_namelen;
    __kernel_long_t f_frsize;
    __kernel_long_t f_flags;
    __kernel_long_t f_spare[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct statfs {
    __kernel_long_t f_type;
    __kernel_long_t f_bsize;
    __kernel_long_t f_blocks;
    __kernel_long_t f_bfree;
    __kernel_long_t f_bavail;
    __kernel_long_t f_files;
    __kernel_long_t f_ffree;
    __kernel_fsid_t f_fsid;
    __kernel_long_t f_namelen;
    __kernel_long_t f_frsize;
    __kernel_long_t f_flags;
    __kernel_long_t f_spare[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct statfs {
    __kernel_long_t f_type;
    __kernel_long_t f_bsize;
    __kernel_long_t f_blocks;
    __kernel_long_t f_bfree;
    __kernel_long_t f_bavail;
    __kernel_long_t f_files;
    __kernel_long_t f_ffree;
    __kernel_fsid_t f_fsid;
    __kernel_long_t f_namelen;
    __kernel_long_t f_frsize;
    __kernel_long_t f_flags;
    __kernel_long_t f_spare[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct statfs {
    __kernel_long_t f_type;
    __kernel_long_t f_bsize;
    __kernel_long_t f_blocks;
    __kernel_long_t f_bfree;
    __kernel_long_t f_bavail;
    __kernel_long_t f_files;
    __kernel_long_t f_ffree;
    __kernel_fsid_t f_fsid;
    __kernel_long_t f_namelen;
    __kernel_long_t f_frsize;
    __kernel_long_t f_flags;
    __kernel_long_t f_spare[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct statfs {
    __kernel_long_t f_type;
    __kernel_long_t f_bsize;
    __kernel_long_t f_blocks;
    __kernel_long_t f_bfree;
    __kernel_long_t f_bavail;
    __kernel_long_t f_files;
    __kernel_long_t f_ffree;
    __kernel_fsid_t f_fsid;
    __kernel_long_t f_namelen;
    __kernel_long_t f_frsize;
    __kernel_long_t f_flags;
    __kernel_long_t f_spare[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct statfs {
    __kernel_long_t f_type;
    __kernel_long_t f_bsize;
    __kernel_long_t f_blocks;
    __kernel_long_t f_bfree;
    __kernel_long_t f_bavail;
    __kernel_long_t f_files;
    __kernel_long_t f_ffree;
    __kernel_fsid_t f_fsid;
    __kernel_long_t f_namelen;
    __kernel_long_t f_frsize;
    __kernel_long_t f_flags;
    __kernel_long_t f_spare[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct statfs {
    __kernel_long_t f_type;
    __kernel_long_t f_bsize;
    __kernel_long_t f_blocks;
    __kernel_long_t f_bfree;
    __kernel_long_t f_bavail;
    __kernel_long_t f_files;
    __kernel_long_t f_ffree;
    __kernel_fsid_t f_fsid;
    __kernel_long_t f_namelen;
    __kernel_long_t f_frsize;
    __kernel_long_t f_flags;
    __kernel_long_t f_spare[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct statfs {
    __kernel_long_t f_type;
    __kernel_long_t f_bsize;
    __kernel_long_t f_blocks;
    __kernel_long_t f_bfree;
    __kernel_long_t f_bavail;
    __kernel_long_t f_files;
    __kernel_long_t f_ffree;
    __kernel_fsid_t f_fsid;
    __kernel_long_t f_namelen;
    __kernel_long_t f_frsize;
    __kernel_long_t f_flags;
    __kernel_long_t f_spare[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct statfs {
    __kernel_long_t f_type;
    __kernel_long_t f_bsize;
    __kernel_long_t f_blocks;
    __kernel_long_t f_bfree;
    __kernel_long_t f_bavail;
    __kernel_long_t f_files;
    __kernel_long_t f_ffree;
    __kernel_fsid_t f_fsid;
    __kernel_long_t f_namelen;
    __kernel_long_t f_frsize;
    __kernel_long_t f_flags;
    __kernel_long_t f_spare[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct statfs {
    __kernel_long_t f_type;
    __kernel_long_t f_bsize;
    __kernel_long_t f_blocks;
    __kernel_long_t f_bfree;
    __kernel_long_t f_bavail;
    __kernel_long_t f_files;
    __kernel_long_t f_ffree;
    __kernel_fsid_t f_fsid;
    __kernel_long_t f_namelen;
    __kernel_long_t f_frsize;
    __kernel_long_t f_flags;
    __kernel_long_t f_spare[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct statfs {
    __kernel_long_t f_type;
    __kernel_long_t f_bsize;
    __kernel_long_t f_blocks;
    __kernel_long_t f_bfree;
    __kernel_long_t f_bavail;
    __kernel_long_t f_files;
    __kernel_long_t f_ffree;
    __kernel_fsid_t f_fsid;
    __kernel_long_t f_namelen;
    __kernel_long_t f_frsize;
    __kernel_long_t f_flags;
    __kernel_long_t f_spare[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct statfs {
    __kernel_long_t f_type;
    __kernel_long_t f_bsize;
    __kernel_long_t f_blocks;
    __kernel_long_t f_bfree;
    __kernel_long_t f_bavail;
    __kernel_long_t f_files;
    __kernel_long_t f_ffree;
    __kernel_fsid_t f_fsid;
    __kernel_long_t f_namelen;
    __kernel_long_t f_frsize;
    __kernel_long_t f_flags;
    __kernel_long_t f_spare[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct statfs {
    __kernel_long_t f_type;
    __kernel_long_t f_bsize;
    __kernel_long_t f_blocks;
    __kernel_long_t f_bfree;
    __kernel_long_t f_bavail;
    __kernel_long_t f_files;
    __kernel_long_t f_ffree;
    __kernel_fsid_t f_fsid;
    __kernel_long_t f_namelen;
    __kernel_long_t f_frsize;
    __kernel_long_t f_flags;
    __kernel_long_t f_spare[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct statfs {
    __kernel_long_t f_type;
    __kernel_long_t f_bsize;
    __kernel_long_t f_blocks;
    __kernel_long_t f_bfree;
    __kernel_long_t f_bavail;
    __kernel_long_t f_files;
    __kernel_long_t f_ffree;
    __kernel_fsid_t f_fsid;
    __kernel_long_t f_namelen;
    __kernel_long_t f_frsize;
    __kernel_long_t f_flags;
    __kernel_long_t f_spare[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct statfs {
    __kernel_long_t f_type;
    __kernel_long_t f_bsize;
    __kernel_long_t f_blocks;
    __kernel_long_t f_bfree;
    __kernel_long_t f_bavail;
    __kernel_long_t f_files;
    __kernel_long_t f_ffree;
    __kernel_fsid_t f_fsid;
    __kernel_long_t f_namelen;
    __kernel_long_t f_frsize;
    __kernel_long_t f_flags;
    __kernel_long_t f_spare[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct statfs {
    __kernel_long_t f_type;
    __kernel_long_t f_bsize;
    __kernel_long_t f_blocks;
    __kernel_long_t f_bfree;
    __kernel_long_t f_bavail;
    __kernel_long_t f_files;
    __kernel_long_t f_ffree;
    __kernel_fsid_t f_fsid;
    __kernel_long_t f_namelen;
    __kernel_long_t f_frsize;
    __kernel_long_t f_flags;
    __kernel_long_t f_spare[4];
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
struct statfs {
    __kernel_long_t f_type;
    __kernel_long_t f_bsize;
    __kernel_long_t f_blocks;
    __kernel_long_t f_bfree;
    __kernel_long_t f_bavail;
    __kernel_long_t f_files;
    __kernel_long_t f_ffree;
    __kernel_fsid_t f_fsid;
    __kernel_long_t f_namelen;
    __kernel_long_t f_frsize;
    __kernel_long_t f_flags;
    __kernel_long_t f_spare[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct statfs {
    __u32 f_type;
    __u32 f_bsize;
    __u32 f_blocks;
    __u32 f_bfree;
    __u32 f_bavail;
    __u32 f_files;
    __u32 f_ffree;
    __kernel_fsid_t f_fsid;
    __u32 f_namelen;
    __u32 f_frsize;
    __u32 f_flags;
    __u32 f_spare[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct statfs {
    __kernel_long_t f_type;
    __kernel_long_t f_bsize;
    __kernel_long_t f_blocks;
    __kernel_long_t f_bfree;
    __kernel_long_t f_bavail;
    __kernel_long_t f_files;
    __kernel_long_t f_ffree;
    __kernel_fsid_t f_fsid;
    __kernel_long_t f_namelen;
    __kernel_long_t f_frsize;
    __kernel_long_t f_flags;
    __kernel_long_t f_spare[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct statfs {
    __kernel_long_t f_type;
    __kernel_long_t f_bsize;
    __kernel_long_t f_blocks;
    __kernel_long_t f_bfree;
    __kernel_long_t f_bavail;
    __kernel_long_t f_files;
    __kernel_long_t f_ffree;
    __kernel_fsid_t f_fsid;
    __kernel_long_t f_namelen;
    __kernel_long_t f_frsize;
    __kernel_long_t f_flags;
    __kernel_long_t f_spare[4];
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
struct statfs {
    __kernel_long_t f_type;
    __kernel_long_t f_bsize;
    __kernel_long_t f_blocks;
    __kernel_long_t f_bfree;
    __kernel_long_t f_bavail;
    __kernel_long_t f_files;
    __kernel_long_t f_ffree;
    __kernel_fsid_t f_fsid;
    __kernel_long_t f_namelen;
    __kernel_long_t f_frsize;
    __kernel_long_t f_flags;
    __kernel_long_t f_spare[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct statfs {
    __kernel_long_t f_type;
    __kernel_long_t f_bsize;
    __kernel_long_t f_blocks;
    __kernel_long_t f_bfree;
    __kernel_long_t f_bavail;
    __kernel_long_t f_files;
    __kernel_long_t f_ffree;
    __kernel_fsid_t f_fsid;
    __kernel_long_t f_namelen;
    __kernel_long_t f_frsize;
    __kernel_long_t f_flags;
    __kernel_long_t f_spare[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct statfs {
    __kernel_long_t f_type;
    __kernel_long_t f_bsize;
    __kernel_long_t f_blocks;
    __kernel_long_t f_bfree;
    __kernel_long_t f_bavail;
    __kernel_long_t f_files;
    __kernel_long_t f_ffree;
    __kernel_fsid_t f_fsid;
    __kernel_long_t f_namelen;
    __kernel_long_t f_frsize;
    __kernel_long_t f_flags;
    __kernel_long_t f_spare[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct statfs {
    __kernel_long_t f_type;
    __kernel_long_t f_bsize;
    __kernel_long_t f_blocks;
    __kernel_long_t f_bfree;
    __kernel_long_t f_bavail;
    __kernel_long_t f_files;
    __kernel_long_t f_ffree;
    __kernel_fsid_t f_fsid;
    __kernel_long_t f_namelen;
    __kernel_long_t f_frsize;
    __kernel_long_t f_flags;
    __kernel_long_t f_spare[4];
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
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>__kernel_long_t f_type</code> ➡️ <code>__u32 f_type</code>
</li>
<li>
<b>Field type changed. </b>
<code>__kernel_long_t f_bsize</code> ➡️ <code>__u32 f_bsize</code>
</li>
<li>
<b>Field type changed. </b>
<code>__kernel_long_t f_blocks</code> ➡️ <code>__u32 f_blocks</code>
</li>
<li>
<b>Field type changed. </b>
<code>__kernel_long_t f_bfree</code> ➡️ <code>__u32 f_bfree</code>
</li>
<li>
<b>Field type changed. </b>
<code>__kernel_long_t f_bavail</code> ➡️ <code>__u32 f_bavail</code>
</li>
<li>
<b>Field type changed. </b>
<code>__kernel_long_t f_files</code> ➡️ <code>__u32 f_files</code>
</li>
<li>
<b>Field type changed. </b>
<code>__kernel_long_t f_ffree</code> ➡️ <code>__u32 f_ffree</code>
</li>
<li>
<b>Field type changed. </b>
<code>__kernel_long_t f_namelen</code> ➡️ <code>__u32 f_namelen</code>
</li>
<li>
<b>Field type changed. </b>
<code>__kernel_long_t f_frsize</code> ➡️ <code>__u32 f_frsize</code>
</li>
<li>
<b>Field type changed. </b>
<code>__kernel_long_t f_flags</code> ➡️ <code>__u32 f_flags</code>
</li>
<li>
<b>Field type changed. </b>
<code>__kernel_long_t f_spare[4]</code> ➡️ <code>__u32 f_spare[4]</code>
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
