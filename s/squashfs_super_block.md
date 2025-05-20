# Struct: <code>squashfs_super_block</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct squashfs_super_block {
    __le32 s_magic;
    __le32 inodes;
    __le32 mkfs_time;
    __le32 block_size;
    __le32 fragments;
    __le16 compression;
    __le16 block_log;
    __le16 flags;
    __le16 no_ids;
    __le16 s_major;
    __le16 s_minor;
    __le64 root_inode;
    __le64 bytes_used;
    __le64 id_table_start;
    __le64 xattr_id_table_start;
    __le64 inode_table_start;
    __le64 directory_table_start;
    __le64 fragment_table_start;
    __le64 lookup_table_start;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct squashfs_super_block {
    __le32 s_magic;
    __le32 inodes;
    __le32 mkfs_time;
    __le32 block_size;
    __le32 fragments;
    __le16 compression;
    __le16 block_log;
    __le16 flags;
    __le16 no_ids;
    __le16 s_major;
    __le16 s_minor;
    __le64 root_inode;
    __le64 bytes_used;
    __le64 id_table_start;
    __le64 xattr_id_table_start;
    __le64 inode_table_start;
    __le64 directory_table_start;
    __le64 fragment_table_start;
    __le64 lookup_table_start;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct squashfs_super_block {
    __le32 s_magic;
    __le32 inodes;
    __le32 mkfs_time;
    __le32 block_size;
    __le32 fragments;
    __le16 compression;
    __le16 block_log;
    __le16 flags;
    __le16 no_ids;
    __le16 s_major;
    __le16 s_minor;
    __le64 root_inode;
    __le64 bytes_used;
    __le64 id_table_start;
    __le64 xattr_id_table_start;
    __le64 inode_table_start;
    __le64 directory_table_start;
    __le64 fragment_table_start;
    __le64 lookup_table_start;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct squashfs_super_block {
    __le32 s_magic;
    __le32 inodes;
    __le32 mkfs_time;
    __le32 block_size;
    __le32 fragments;
    __le16 compression;
    __le16 block_log;
    __le16 flags;
    __le16 no_ids;
    __le16 s_major;
    __le16 s_minor;
    __le64 root_inode;
    __le64 bytes_used;
    __le64 id_table_start;
    __le64 xattr_id_table_start;
    __le64 inode_table_start;
    __le64 directory_table_start;
    __le64 fragment_table_start;
    __le64 lookup_table_start;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct squashfs_super_block {
    __le32 s_magic;
    __le32 inodes;
    __le32 mkfs_time;
    __le32 block_size;
    __le32 fragments;
    __le16 compression;
    __le16 block_log;
    __le16 flags;
    __le16 no_ids;
    __le16 s_major;
    __le16 s_minor;
    __le64 root_inode;
    __le64 bytes_used;
    __le64 id_table_start;
    __le64 xattr_id_table_start;
    __le64 inode_table_start;
    __le64 directory_table_start;
    __le64 fragment_table_start;
    __le64 lookup_table_start;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct squashfs_super_block {
    __le32 s_magic;
    __le32 inodes;
    __le32 mkfs_time;
    __le32 block_size;
    __le32 fragments;
    __le16 compression;
    __le16 block_log;
    __le16 flags;
    __le16 no_ids;
    __le16 s_major;
    __le16 s_minor;
    __le64 root_inode;
    __le64 bytes_used;
    __le64 id_table_start;
    __le64 xattr_id_table_start;
    __le64 inode_table_start;
    __le64 directory_table_start;
    __le64 fragment_table_start;
    __le64 lookup_table_start;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct squashfs_super_block {
    __le32 s_magic;
    __le32 inodes;
    __le32 mkfs_time;
    __le32 block_size;
    __le32 fragments;
    __le16 compression;
    __le16 block_log;
    __le16 flags;
    __le16 no_ids;
    __le16 s_major;
    __le16 s_minor;
    __le64 root_inode;
    __le64 bytes_used;
    __le64 id_table_start;
    __le64 xattr_id_table_start;
    __le64 inode_table_start;
    __le64 directory_table_start;
    __le64 fragment_table_start;
    __le64 lookup_table_start;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct squashfs_super_block {
    __le32 s_magic;
    __le32 inodes;
    __le32 mkfs_time;
    __le32 block_size;
    __le32 fragments;
    __le16 compression;
    __le16 block_log;
    __le16 flags;
    __le16 no_ids;
    __le16 s_major;
    __le16 s_minor;
    __le64 root_inode;
    __le64 bytes_used;
    __le64 id_table_start;
    __le64 xattr_id_table_start;
    __le64 inode_table_start;
    __le64 directory_table_start;
    __le64 fragment_table_start;
    __le64 lookup_table_start;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct squashfs_super_block {
    __le32 s_magic;
    __le32 inodes;
    __le32 mkfs_time;
    __le32 block_size;
    __le32 fragments;
    __le16 compression;
    __le16 block_log;
    __le16 flags;
    __le16 no_ids;
    __le16 s_major;
    __le16 s_minor;
    __le64 root_inode;
    __le64 bytes_used;
    __le64 id_table_start;
    __le64 xattr_id_table_start;
    __le64 inode_table_start;
    __le64 directory_table_start;
    __le64 fragment_table_start;
    __le64 lookup_table_start;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct squashfs_super_block {
    __le32 s_magic;
    __le32 inodes;
    __le32 mkfs_time;
    __le32 block_size;
    __le32 fragments;
    __le16 compression;
    __le16 block_log;
    __le16 flags;
    __le16 no_ids;
    __le16 s_major;
    __le16 s_minor;
    __le64 root_inode;
    __le64 bytes_used;
    __le64 id_table_start;
    __le64 xattr_id_table_start;
    __le64 inode_table_start;
    __le64 directory_table_start;
    __le64 fragment_table_start;
    __le64 lookup_table_start;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct squashfs_super_block {
    __le32 s_magic;
    __le32 inodes;
    __le32 mkfs_time;
    __le32 block_size;
    __le32 fragments;
    __le16 compression;
    __le16 block_log;
    __le16 flags;
    __le16 no_ids;
    __le16 s_major;
    __le16 s_minor;
    __le64 root_inode;
    __le64 bytes_used;
    __le64 id_table_start;
    __le64 xattr_id_table_start;
    __le64 inode_table_start;
    __le64 directory_table_start;
    __le64 fragment_table_start;
    __le64 lookup_table_start;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct squashfs_super_block {
    __le32 s_magic;
    __le32 inodes;
    __le32 mkfs_time;
    __le32 block_size;
    __le32 fragments;
    __le16 compression;
    __le16 block_log;
    __le16 flags;
    __le16 no_ids;
    __le16 s_major;
    __le16 s_minor;
    __le64 root_inode;
    __le64 bytes_used;
    __le64 id_table_start;
    __le64 xattr_id_table_start;
    __le64 inode_table_start;
    __le64 directory_table_start;
    __le64 fragment_table_start;
    __le64 lookup_table_start;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct squashfs_super_block {
    __le32 s_magic;
    __le32 inodes;
    __le32 mkfs_time;
    __le32 block_size;
    __le32 fragments;
    __le16 compression;
    __le16 block_log;
    __le16 flags;
    __le16 no_ids;
    __le16 s_major;
    __le16 s_minor;
    __le64 root_inode;
    __le64 bytes_used;
    __le64 id_table_start;
    __le64 xattr_id_table_start;
    __le64 inode_table_start;
    __le64 directory_table_start;
    __le64 fragment_table_start;
    __le64 lookup_table_start;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct squashfs_super_block {
    __le32 s_magic;
    __le32 inodes;
    __le32 mkfs_time;
    __le32 block_size;
    __le32 fragments;
    __le16 compression;
    __le16 block_log;
    __le16 flags;
    __le16 no_ids;
    __le16 s_major;
    __le16 s_minor;
    __le64 root_inode;
    __le64 bytes_used;
    __le64 id_table_start;
    __le64 xattr_id_table_start;
    __le64 inode_table_start;
    __le64 directory_table_start;
    __le64 fragment_table_start;
    __le64 lookup_table_start;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct squashfs_super_block {
    __le32 s_magic;
    __le32 inodes;
    __le32 mkfs_time;
    __le32 block_size;
    __le32 fragments;
    __le16 compression;
    __le16 block_log;
    __le16 flags;
    __le16 no_ids;
    __le16 s_major;
    __le16 s_minor;
    __le64 root_inode;
    __le64 bytes_used;
    __le64 id_table_start;
    __le64 xattr_id_table_start;
    __le64 inode_table_start;
    __le64 directory_table_start;
    __le64 fragment_table_start;
    __le64 lookup_table_start;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct squashfs_super_block {
    __le32 s_magic;
    __le32 inodes;
    __le32 mkfs_time;
    __le32 block_size;
    __le32 fragments;
    __le16 compression;
    __le16 block_log;
    __le16 flags;
    __le16 no_ids;
    __le16 s_major;
    __le16 s_minor;
    __le64 root_inode;
    __le64 bytes_used;
    __le64 id_table_start;
    __le64 xattr_id_table_start;
    __le64 inode_table_start;
    __le64 directory_table_start;
    __le64 fragment_table_start;
    __le64 lookup_table_start;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct squashfs_super_block {
    __le32 s_magic;
    __le32 inodes;
    __le32 mkfs_time;
    __le32 block_size;
    __le32 fragments;
    __le16 compression;
    __le16 block_log;
    __le16 flags;
    __le16 no_ids;
    __le16 s_major;
    __le16 s_minor;
    __le64 root_inode;
    __le64 bytes_used;
    __le64 id_table_start;
    __le64 xattr_id_table_start;
    __le64 inode_table_start;
    __le64 directory_table_start;
    __le64 fragment_table_start;
    __le64 lookup_table_start;
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
struct squashfs_super_block {
    __le32 s_magic;
    __le32 inodes;
    __le32 mkfs_time;
    __le32 block_size;
    __le32 fragments;
    __le16 compression;
    __le16 block_log;
    __le16 flags;
    __le16 no_ids;
    __le16 s_major;
    __le16 s_minor;
    __le64 root_inode;
    __le64 bytes_used;
    __le64 id_table_start;
    __le64 xattr_id_table_start;
    __le64 inode_table_start;
    __le64 directory_table_start;
    __le64 fragment_table_start;
    __le64 lookup_table_start;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct squashfs_super_block {
    __le32 s_magic;
    __le32 inodes;
    __le32 mkfs_time;
    __le32 block_size;
    __le32 fragments;
    __le16 compression;
    __le16 block_log;
    __le16 flags;
    __le16 no_ids;
    __le16 s_major;
    __le16 s_minor;
    __le64 root_inode;
    __le64 bytes_used;
    __le64 id_table_start;
    __le64 xattr_id_table_start;
    __le64 inode_table_start;
    __le64 directory_table_start;
    __le64 fragment_table_start;
    __le64 lookup_table_start;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct squashfs_super_block {
    __le32 s_magic;
    __le32 inodes;
    __le32 mkfs_time;
    __le32 block_size;
    __le32 fragments;
    __le16 compression;
    __le16 block_log;
    __le16 flags;
    __le16 no_ids;
    __le16 s_major;
    __le16 s_minor;
    __le64 root_inode;
    __le64 bytes_used;
    __le64 id_table_start;
    __le64 xattr_id_table_start;
    __le64 inode_table_start;
    __le64 directory_table_start;
    __le64 fragment_table_start;
    __le64 lookup_table_start;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct squashfs_super_block {
    __le32 s_magic;
    __le32 inodes;
    __le32 mkfs_time;
    __le32 block_size;
    __le32 fragments;
    __le16 compression;
    __le16 block_log;
    __le16 flags;
    __le16 no_ids;
    __le16 s_major;
    __le16 s_minor;
    __le64 root_inode;
    __le64 bytes_used;
    __le64 id_table_start;
    __le64 xattr_id_table_start;
    __le64 inode_table_start;
    __le64 directory_table_start;
    __le64 fragment_table_start;
    __le64 lookup_table_start;
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
struct squashfs_super_block {
    __le32 s_magic;
    __le32 inodes;
    __le32 mkfs_time;
    __le32 block_size;
    __le32 fragments;
    __le16 compression;
    __le16 block_log;
    __le16 flags;
    __le16 no_ids;
    __le16 s_major;
    __le16 s_minor;
    __le64 root_inode;
    __le64 bytes_used;
    __le64 id_table_start;
    __le64 xattr_id_table_start;
    __le64 inode_table_start;
    __le64 directory_table_start;
    __le64 fragment_table_start;
    __le64 lookup_table_start;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct squashfs_super_block {
    __le32 s_magic;
    __le32 inodes;
    __le32 mkfs_time;
    __le32 block_size;
    __le32 fragments;
    __le16 compression;
    __le16 block_log;
    __le16 flags;
    __le16 no_ids;
    __le16 s_major;
    __le16 s_minor;
    __le64 root_inode;
    __le64 bytes_used;
    __le64 id_table_start;
    __le64 xattr_id_table_start;
    __le64 inode_table_start;
    __le64 directory_table_start;
    __le64 fragment_table_start;
    __le64 lookup_table_start;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct squashfs_super_block {
    __le32 s_magic;
    __le32 inodes;
    __le32 mkfs_time;
    __le32 block_size;
    __le32 fragments;
    __le16 compression;
    __le16 block_log;
    __le16 flags;
    __le16 no_ids;
    __le16 s_major;
    __le16 s_minor;
    __le64 root_inode;
    __le64 bytes_used;
    __le64 id_table_start;
    __le64 xattr_id_table_start;
    __le64 inode_table_start;
    __le64 directory_table_start;
    __le64 fragment_table_start;
    __le64 lookup_table_start;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct squashfs_super_block {
    __le32 s_magic;
    __le32 inodes;
    __le32 mkfs_time;
    __le32 block_size;
    __le32 fragments;
    __le16 compression;
    __le16 block_log;
    __le16 flags;
    __le16 no_ids;
    __le16 s_major;
    __le16 s_minor;
    __le64 root_inode;
    __le64 bytes_used;
    __le64 id_table_start;
    __le64 xattr_id_table_start;
    __le64 inode_table_start;
    __le64 directory_table_start;
    __le64 fragment_table_start;
    __le64 lookup_table_start;
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
