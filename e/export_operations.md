# Struct: <code>export_operations</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct export_operations {
    int (*encode_fh)(struct inode *, __u32 *, int *, struct inode *);
    struct dentry * (*fh_to_dentry)(struct super_block *, struct fid *, int, int);
    struct dentry * (*fh_to_parent)(struct super_block *, struct fid *, int, int);
    int (*get_name)(struct dentry *, char *, struct dentry *);
    struct dentry * (*get_parent)(struct dentry *);
    int (*commit_metadata)(struct inode *);
    int (*get_uuid)(struct super_block *, u8 *, u32 *, u64 *);
    int (*map_blocks)(struct inode *, loff_t, u64, struct iomap *, bool, u32 *);
    int (*commit_blocks)(struct inode *, struct iomap *, int, struct iattr *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct export_operations {
    int (*encode_fh)(struct inode *, __u32 *, int *, struct inode *);
    struct dentry * (*fh_to_dentry)(struct super_block *, struct fid *, int, int);
    struct dentry * (*fh_to_parent)(struct super_block *, struct fid *, int, int);
    int (*get_name)(struct dentry *, char *, struct dentry *);
    struct dentry * (*get_parent)(struct dentry *);
    int (*commit_metadata)(struct inode *);
    int (*get_uuid)(struct super_block *, u8 *, u32 *, u64 *);
    int (*map_blocks)(struct inode *, loff_t, u64, struct iomap *, bool, u32 *);
    int (*commit_blocks)(struct inode *, struct iomap *, int, struct iattr *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct export_operations {
    int (*encode_fh)(struct inode *, __u32 *, int *, struct inode *);
    struct dentry * (*fh_to_dentry)(struct super_block *, struct fid *, int, int);
    struct dentry * (*fh_to_parent)(struct super_block *, struct fid *, int, int);
    int (*get_name)(struct dentry *, char *, struct dentry *);
    struct dentry * (*get_parent)(struct dentry *);
    int (*commit_metadata)(struct inode *);
    int (*get_uuid)(struct super_block *, u8 *, u32 *, u64 *);
    int (*map_blocks)(struct inode *, loff_t, u64, struct iomap *, bool, u32 *);
    int (*commit_blocks)(struct inode *, struct iomap *, int, struct iattr *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct export_operations {
    int (*encode_fh)(struct inode *, __u32 *, int *, struct inode *);
    struct dentry * (*fh_to_dentry)(struct super_block *, struct fid *, int, int);
    struct dentry * (*fh_to_parent)(struct super_block *, struct fid *, int, int);
    int (*get_name)(struct dentry *, char *, struct dentry *);
    struct dentry * (*get_parent)(struct dentry *);
    int (*commit_metadata)(struct inode *);
    int (*get_uuid)(struct super_block *, u8 *, u32 *, u64 *);
    int (*map_blocks)(struct inode *, loff_t, u64, struct iomap *, bool, u32 *);
    int (*commit_blocks)(struct inode *, struct iomap *, int, struct iattr *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct export_operations {
    int (*encode_fh)(struct inode *, __u32 *, int *, struct inode *);
    struct dentry * (*fh_to_dentry)(struct super_block *, struct fid *, int, int);
    struct dentry * (*fh_to_parent)(struct super_block *, struct fid *, int, int);
    int (*get_name)(struct dentry *, char *, struct dentry *);
    struct dentry * (*get_parent)(struct dentry *);
    int (*commit_metadata)(struct inode *);
    int (*get_uuid)(struct super_block *, u8 *, u32 *, u64 *);
    int (*map_blocks)(struct inode *, loff_t, u64, struct iomap *, bool, u32 *);
    int (*commit_blocks)(struct inode *, struct iomap *, int, struct iattr *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct export_operations {
    int (*encode_fh)(struct inode *, __u32 *, int *, struct inode *);
    struct dentry * (*fh_to_dentry)(struct super_block *, struct fid *, int, int);
    struct dentry * (*fh_to_parent)(struct super_block *, struct fid *, int, int);
    int (*get_name)(struct dentry *, char *, struct dentry *);
    struct dentry * (*get_parent)(struct dentry *);
    int (*commit_metadata)(struct inode *);
    int (*get_uuid)(struct super_block *, u8 *, u32 *, u64 *);
    int (*map_blocks)(struct inode *, loff_t, u64, struct iomap *, bool, u32 *);
    int (*commit_blocks)(struct inode *, struct iomap *, int, struct iattr *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct export_operations {
    int (*encode_fh)(struct inode *, __u32 *, int *, struct inode *);
    struct dentry * (*fh_to_dentry)(struct super_block *, struct fid *, int, int);
    struct dentry * (*fh_to_parent)(struct super_block *, struct fid *, int, int);
    int (*get_name)(struct dentry *, char *, struct dentry *);
    struct dentry * (*get_parent)(struct dentry *);
    int (*commit_metadata)(struct inode *);
    int (*get_uuid)(struct super_block *, u8 *, u32 *, u64 *);
    int (*map_blocks)(struct inode *, loff_t, u64, struct iomap *, bool, u32 *);
    int (*commit_blocks)(struct inode *, struct iomap *, int, struct iattr *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct export_operations {
    int (*encode_fh)(struct inode *, __u32 *, int *, struct inode *);
    struct dentry * (*fh_to_dentry)(struct super_block *, struct fid *, int, int);
    struct dentry * (*fh_to_parent)(struct super_block *, struct fid *, int, int);
    int (*get_name)(struct dentry *, char *, struct dentry *);
    struct dentry * (*get_parent)(struct dentry *);
    int (*commit_metadata)(struct inode *);
    int (*get_uuid)(struct super_block *, u8 *, u32 *, u64 *);
    int (*map_blocks)(struct inode *, loff_t, u64, struct iomap *, bool, u32 *);
    int (*commit_blocks)(struct inode *, struct iomap *, int, struct iattr *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct export_operations {
    int (*encode_fh)(struct inode *, __u32 *, int *, struct inode *);
    struct dentry * (*fh_to_dentry)(struct super_block *, struct fid *, int, int);
    struct dentry * (*fh_to_parent)(struct super_block *, struct fid *, int, int);
    int (*get_name)(struct dentry *, char *, struct dentry *);
    struct dentry * (*get_parent)(struct dentry *);
    int (*commit_metadata)(struct inode *);
    int (*get_uuid)(struct super_block *, u8 *, u32 *, u64 *);
    int (*map_blocks)(struct inode *, loff_t, u64, struct iomap *, bool, u32 *);
    int (*commit_blocks)(struct inode *, struct iomap *, int, struct iattr *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct export_operations {
    int (*encode_fh)(struct inode *, __u32 *, int *, struct inode *);
    struct dentry * (*fh_to_dentry)(struct super_block *, struct fid *, int, int);
    struct dentry * (*fh_to_parent)(struct super_block *, struct fid *, int, int);
    int (*get_name)(struct dentry *, char *, struct dentry *);
    struct dentry * (*get_parent)(struct dentry *);
    int (*commit_metadata)(struct inode *);
    int (*get_uuid)(struct super_block *, u8 *, u32 *, u64 *);
    int (*map_blocks)(struct inode *, loff_t, u64, struct iomap *, bool, u32 *);
    int (*commit_blocks)(struct inode *, struct iomap *, int, struct iattr *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct export_operations {
    int (*encode_fh)(struct inode *, __u32 *, int *, struct inode *);
    struct dentry * (*fh_to_dentry)(struct super_block *, struct fid *, int, int);
    struct dentry * (*fh_to_parent)(struct super_block *, struct fid *, int, int);
    int (*get_name)(struct dentry *, char *, struct dentry *);
    struct dentry * (*get_parent)(struct dentry *);
    int (*commit_metadata)(struct inode *);
    int (*get_uuid)(struct super_block *, u8 *, u32 *, u64 *);
    int (*map_blocks)(struct inode *, loff_t, u64, struct iomap *, bool, u32 *);
    int (*commit_blocks)(struct inode *, struct iomap *, int, struct iattr *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct export_operations {
    int (*encode_fh)(struct inode *, __u32 *, int *, struct inode *);
    struct dentry * (*fh_to_dentry)(struct super_block *, struct fid *, int, int);
    struct dentry * (*fh_to_parent)(struct super_block *, struct fid *, int, int);
    int (*get_name)(struct dentry *, char *, struct dentry *);
    struct dentry * (*get_parent)(struct dentry *);
    int (*commit_metadata)(struct inode *);
    int (*get_uuid)(struct super_block *, u8 *, u32 *, u64 *);
    int (*map_blocks)(struct inode *, loff_t, u64, struct iomap *, bool, u32 *);
    int (*commit_blocks)(struct inode *, struct iomap *, int, struct iattr *);
    u64 (*fetch_iversion)(struct inode *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct export_operations {
    int (*encode_fh)(struct inode *, __u32 *, int *, struct inode *);
    struct dentry * (*fh_to_dentry)(struct super_block *, struct fid *, int, int);
    struct dentry * (*fh_to_parent)(struct super_block *, struct fid *, int, int);
    int (*get_name)(struct dentry *, char *, struct dentry *);
    struct dentry * (*get_parent)(struct dentry *);
    int (*commit_metadata)(struct inode *);
    int (*get_uuid)(struct super_block *, u8 *, u32 *, u64 *);
    int (*map_blocks)(struct inode *, loff_t, u64, struct iomap *, bool, u32 *);
    int (*commit_blocks)(struct inode *, struct iomap *, int, struct iattr *);
    u64 (*fetch_iversion)(struct inode *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct export_operations {
    int (*encode_fh)(struct inode *, __u32 *, int *, struct inode *);
    struct dentry * (*fh_to_dentry)(struct super_block *, struct fid *, int, int);
    struct dentry * (*fh_to_parent)(struct super_block *, struct fid *, int, int);
    int (*get_name)(struct dentry *, char *, struct dentry *);
    struct dentry * (*get_parent)(struct dentry *);
    int (*commit_metadata)(struct inode *);
    int (*get_uuid)(struct super_block *, u8 *, u32 *, u64 *);
    int (*map_blocks)(struct inode *, loff_t, u64, struct iomap *, bool, u32 *);
    int (*commit_blocks)(struct inode *, struct iomap *, int, struct iattr *);
    u64 (*fetch_iversion)(struct inode *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct export_operations {
    int (*encode_fh)(struct inode *, __u32 *, int *, struct inode *);
    struct dentry * (*fh_to_dentry)(struct super_block *, struct fid *, int, int);
    struct dentry * (*fh_to_parent)(struct super_block *, struct fid *, int, int);
    int (*get_name)(struct dentry *, char *, struct dentry *);
    struct dentry * (*get_parent)(struct dentry *);
    int (*commit_metadata)(struct inode *);
    int (*get_uuid)(struct super_block *, u8 *, u32 *, u64 *);
    int (*map_blocks)(struct inode *, loff_t, u64, struct iomap *, bool, u32 *);
    int (*commit_blocks)(struct inode *, struct iomap *, int, struct iattr *);
    u64 (*fetch_iversion)(struct inode *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct export_operations {
    int (*encode_fh)(struct inode *, __u32 *, int *, struct inode *);
    struct dentry * (*fh_to_dentry)(struct super_block *, struct fid *, int, int);
    struct dentry * (*fh_to_parent)(struct super_block *, struct fid *, int, int);
    int (*get_name)(struct dentry *, char *, struct dentry *);
    struct dentry * (*get_parent)(struct dentry *);
    int (*commit_metadata)(struct inode *);
    int (*get_uuid)(struct super_block *, u8 *, u32 *, u64 *);
    int (*map_blocks)(struct inode *, loff_t, u64, struct iomap *, bool, u32 *);
    int (*commit_blocks)(struct inode *, struct iomap *, int, struct iattr *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct export_operations {
    int (*encode_fh)(struct inode *, __u32 *, int *, struct inode *);
    struct dentry * (*fh_to_dentry)(struct super_block *, struct fid *, int, int);
    struct dentry * (*fh_to_parent)(struct super_block *, struct fid *, int, int);
    int (*get_name)(struct dentry *, char *, struct dentry *);
    struct dentry * (*get_parent)(struct dentry *);
    int (*commit_metadata)(struct inode *);
    int (*get_uuid)(struct super_block *, u8 *, u32 *, u64 *);
    int (*map_blocks)(struct inode *, loff_t, u64, struct iomap *, bool, u32 *);
    int (*commit_blocks)(struct inode *, struct iomap *, int, struct iattr *);
    long unsigned int flags;
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
struct export_operations {
    int (*encode_fh)(struct inode *, __u32 *, int *, struct inode *);
    struct dentry * (*fh_to_dentry)(struct super_block *, struct fid *, int, int);
    struct dentry * (*fh_to_parent)(struct super_block *, struct fid *, int, int);
    int (*get_name)(struct dentry *, char *, struct dentry *);
    struct dentry * (*get_parent)(struct dentry *);
    int (*commit_metadata)(struct inode *);
    int (*get_uuid)(struct super_block *, u8 *, u32 *, u64 *);
    int (*map_blocks)(struct inode *, loff_t, u64, struct iomap *, bool, u32 *);
    int (*commit_blocks)(struct inode *, struct iomap *, int, struct iattr *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct export_operations {
    int (*encode_fh)(struct inode *, __u32 *, int *, struct inode *);
    struct dentry * (*fh_to_dentry)(struct super_block *, struct fid *, int, int);
    struct dentry * (*fh_to_parent)(struct super_block *, struct fid *, int, int);
    int (*get_name)(struct dentry *, char *, struct dentry *);
    struct dentry * (*get_parent)(struct dentry *);
    int (*commit_metadata)(struct inode *);
    int (*get_uuid)(struct super_block *, u8 *, u32 *, u64 *);
    int (*map_blocks)(struct inode *, loff_t, u64, struct iomap *, bool, u32 *);
    int (*commit_blocks)(struct inode *, struct iomap *, int, struct iattr *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct export_operations {
    int (*encode_fh)(struct inode *, __u32 *, int *, struct inode *);
    struct dentry * (*fh_to_dentry)(struct super_block *, struct fid *, int, int);
    struct dentry * (*fh_to_parent)(struct super_block *, struct fid *, int, int);
    int (*get_name)(struct dentry *, char *, struct dentry *);
    struct dentry * (*get_parent)(struct dentry *);
    int (*commit_metadata)(struct inode *);
    int (*get_uuid)(struct super_block *, u8 *, u32 *, u64 *);
    int (*map_blocks)(struct inode *, loff_t, u64, struct iomap *, bool, u32 *);
    int (*commit_blocks)(struct inode *, struct iomap *, int, struct iattr *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct export_operations {
    int (*encode_fh)(struct inode *, __u32 *, int *, struct inode *);
    struct dentry * (*fh_to_dentry)(struct super_block *, struct fid *, int, int);
    struct dentry * (*fh_to_parent)(struct super_block *, struct fid *, int, int);
    int (*get_name)(struct dentry *, char *, struct dentry *);
    struct dentry * (*get_parent)(struct dentry *);
    int (*commit_metadata)(struct inode *);
    int (*get_uuid)(struct super_block *, u8 *, u32 *, u64 *);
    int (*map_blocks)(struct inode *, loff_t, u64, struct iomap *, bool, u32 *);
    int (*commit_blocks)(struct inode *, struct iomap *, int, struct iattr *);
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
struct export_operations {
    int (*encode_fh)(struct inode *, __u32 *, int *, struct inode *);
    struct dentry * (*fh_to_dentry)(struct super_block *, struct fid *, int, int);
    struct dentry * (*fh_to_parent)(struct super_block *, struct fid *, int, int);
    int (*get_name)(struct dentry *, char *, struct dentry *);
    struct dentry * (*get_parent)(struct dentry *);
    int (*commit_metadata)(struct inode *);
    int (*get_uuid)(struct super_block *, u8 *, u32 *, u64 *);
    int (*map_blocks)(struct inode *, loff_t, u64, struct iomap *, bool, u32 *);
    int (*commit_blocks)(struct inode *, struct iomap *, int, struct iattr *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct export_operations {
    int (*encode_fh)(struct inode *, __u32 *, int *, struct inode *);
    struct dentry * (*fh_to_dentry)(struct super_block *, struct fid *, int, int);
    struct dentry * (*fh_to_parent)(struct super_block *, struct fid *, int, int);
    int (*get_name)(struct dentry *, char *, struct dentry *);
    struct dentry * (*get_parent)(struct dentry *);
    int (*commit_metadata)(struct inode *);
    int (*get_uuid)(struct super_block *, u8 *, u32 *, u64 *);
    int (*map_blocks)(struct inode *, loff_t, u64, struct iomap *, bool, u32 *);
    int (*commit_blocks)(struct inode *, struct iomap *, int, struct iattr *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct export_operations {
    int (*encode_fh)(struct inode *, __u32 *, int *, struct inode *);
    struct dentry * (*fh_to_dentry)(struct super_block *, struct fid *, int, int);
    struct dentry * (*fh_to_parent)(struct super_block *, struct fid *, int, int);
    int (*get_name)(struct dentry *, char *, struct dentry *);
    struct dentry * (*get_parent)(struct dentry *);
    int (*commit_metadata)(struct inode *);
    int (*get_uuid)(struct super_block *, u8 *, u32 *, u64 *);
    int (*map_blocks)(struct inode *, loff_t, u64, struct iomap *, bool, u32 *);
    int (*commit_blocks)(struct inode *, struct iomap *, int, struct iattr *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct export_operations {
    int (*encode_fh)(struct inode *, __u32 *, int *, struct inode *);
    struct dentry * (*fh_to_dentry)(struct super_block *, struct fid *, int, int);
    struct dentry * (*fh_to_parent)(struct super_block *, struct fid *, int, int);
    int (*get_name)(struct dentry *, char *, struct dentry *);
    struct dentry * (*get_parent)(struct dentry *);
    int (*commit_metadata)(struct inode *);
    int (*get_uuid)(struct super_block *, u8 *, u32 *, u64 *);
    int (*map_blocks)(struct inode *, loff_t, u64, struct iomap *, bool, u32 *);
    int (*commit_blocks)(struct inode *, struct iomap *, int, struct iattr *);
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int flags</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 (*fetch_iversion)(struct inode *)</code>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>u64 (*fetch_iversion)(struct inode *)</code>
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
