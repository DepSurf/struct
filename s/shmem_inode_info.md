# Struct: <code>shmem_inode_info</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct shmem_inode_info {
    spinlock_t lock;
    unsigned int seals;
    long unsigned int flags;
    long unsigned int alloced;
    long unsigned int swapped;
    struct shared_policy policy;
    struct list_head swaplist;
    struct simple_xattrs xattrs;
    struct inode vfs_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct shmem_inode_info {
    spinlock_t lock;
    unsigned int seals;
    long unsigned int flags;
    long unsigned int alloced;
    long unsigned int swapped;
    struct list_head shrinklist;
    struct list_head swaplist;
    struct shared_policy policy;
    struct simple_xattrs xattrs;
    struct inode vfs_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct shmem_inode_info {
    spinlock_t lock;
    unsigned int seals;
    long unsigned int flags;
    long unsigned int alloced;
    long unsigned int swapped;
    struct list_head shrinklist;
    struct list_head swaplist;
    struct shared_policy policy;
    struct simple_xattrs xattrs;
    struct inode vfs_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct shmem_inode_info {
    spinlock_t lock;
    unsigned int seals;
    long unsigned int flags;
    long unsigned int alloced;
    long unsigned int swapped;
    struct list_head shrinklist;
    struct list_head swaplist;
    struct shared_policy policy;
    struct simple_xattrs xattrs;
    struct inode vfs_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct shmem_inode_info {
    spinlock_t lock;
    unsigned int seals;
    long unsigned int flags;
    long unsigned int alloced;
    long unsigned int swapped;
    struct list_head shrinklist;
    struct list_head swaplist;
    struct shared_policy policy;
    struct simple_xattrs xattrs;
    struct inode vfs_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct shmem_inode_info {
    spinlock_t lock;
    unsigned int seals;
    long unsigned int flags;
    long unsigned int alloced;
    long unsigned int swapped;
    struct list_head shrinklist;
    struct list_head swaplist;
    struct shared_policy policy;
    struct simple_xattrs xattrs;
    struct inode vfs_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct shmem_inode_info {
    spinlock_t lock;
    unsigned int seals;
    long unsigned int flags;
    long unsigned int alloced;
    long unsigned int swapped;
    struct list_head shrinklist;
    struct list_head swaplist;
    struct shared_policy policy;
    struct simple_xattrs xattrs;
    struct inode vfs_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct shmem_inode_info {
    spinlock_t lock;
    unsigned int seals;
    long unsigned int flags;
    long unsigned int alloced;
    long unsigned int swapped;
    struct list_head shrinklist;
    struct list_head swaplist;
    struct shared_policy policy;
    struct simple_xattrs xattrs;
    atomic_t stop_eviction;
    struct inode vfs_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct shmem_inode_info {
    spinlock_t lock;
    unsigned int seals;
    long unsigned int flags;
    long unsigned int alloced;
    long unsigned int swapped;
    struct list_head shrinklist;
    struct list_head swaplist;
    struct shared_policy policy;
    struct simple_xattrs xattrs;
    atomic_t stop_eviction;
    struct inode vfs_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct shmem_inode_info {
    spinlock_t lock;
    unsigned int seals;
    long unsigned int flags;
    long unsigned int alloced;
    long unsigned int swapped;
    struct list_head shrinklist;
    struct list_head swaplist;
    struct shared_policy policy;
    struct simple_xattrs xattrs;
    atomic_t stop_eviction;
    struct inode vfs_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct shmem_inode_info {
    spinlock_t lock;
    unsigned int seals;
    long unsigned int flags;
    long unsigned int alloced;
    long unsigned int swapped;
    struct list_head shrinklist;
    struct list_head swaplist;
    struct shared_policy policy;
    struct simple_xattrs xattrs;
    atomic_t stop_eviction;
    struct inode vfs_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct shmem_inode_info {
    spinlock_t lock;
    unsigned int seals;
    long unsigned int flags;
    long unsigned int alloced;
    long unsigned int swapped;
    struct list_head shrinklist;
    struct list_head swaplist;
    struct shared_policy policy;
    struct simple_xattrs xattrs;
    atomic_t stop_eviction;
    struct inode vfs_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct shmem_inode_info {
    spinlock_t lock;
    unsigned int seals;
    long unsigned int flags;
    long unsigned int alloced;
    long unsigned int swapped;
    long unsigned int fallocend;
    struct list_head shrinklist;
    struct list_head swaplist;
    struct shared_policy policy;
    struct simple_xattrs xattrs;
    atomic_t stop_eviction;
    struct inode vfs_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct shmem_inode_info {
    spinlock_t lock;
    unsigned int seals;
    long unsigned int flags;
    long unsigned int alloced;
    long unsigned int swapped;
    long unsigned int fallocend;
    struct list_head shrinklist;
    struct list_head swaplist;
    struct shared_policy policy;
    struct simple_xattrs xattrs;
    atomic_t stop_eviction;
    struct timespec64 i_crtime;
    struct inode vfs_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct shmem_inode_info {
    spinlock_t lock;
    unsigned int seals;
    long unsigned int flags;
    long unsigned int alloced;
    long unsigned int swapped;
    long unsigned int fallocend;
    struct list_head shrinklist;
    struct list_head swaplist;
    struct shared_policy policy;
    struct simple_xattrs xattrs;
    atomic_t stop_eviction;
    struct timespec64 i_crtime;
    unsigned int fsflags;
    struct inode vfs_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct shmem_inode_info {
    spinlock_t lock;
    unsigned int seals;
    long unsigned int flags;
    long unsigned int alloced;
    long unsigned int swapped;
    long unsigned int fallocend;
    struct list_head shrinklist;
    struct list_head swaplist;
    struct shared_policy policy;
    struct simple_xattrs xattrs;
    atomic_t stop_eviction;
    struct timespec64 i_crtime;
    unsigned int fsflags;
    struct inode vfs_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct shmem_inode_info {
    spinlock_t lock;
    unsigned int seals;
    long unsigned int flags;
    long unsigned int alloced;
    long unsigned int swapped;
    struct offset_ctx dir_offsets;
    struct list_head shrinklist;
    struct list_head swaplist;
    struct timespec64 i_crtime;
    struct shared_policy policy;
    struct simple_xattrs xattrs;
    long unsigned int fallocend;
    unsigned int fsflags;
    atomic_t stop_eviction;
    struct dquot * i_dquot[3];
    struct inode vfs_inode;
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
struct shmem_inode_info {
    spinlock_t lock;
    unsigned int seals;
    long unsigned int flags;
    long unsigned int alloced;
    long unsigned int swapped;
    struct list_head shrinklist;
    struct list_head swaplist;
    struct shared_policy policy;
    struct simple_xattrs xattrs;
    atomic_t stop_eviction;
    struct inode vfs_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct shmem_inode_info {
    spinlock_t lock;
    unsigned int seals;
    long unsigned int flags;
    long unsigned int alloced;
    long unsigned int swapped;
    struct list_head shrinklist;
    struct list_head swaplist;
    struct shared_policy policy;
    struct simple_xattrs xattrs;
    atomic_t stop_eviction;
    struct inode vfs_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct shmem_inode_info {
    spinlock_t lock;
    unsigned int seals;
    long unsigned int flags;
    long unsigned int alloced;
    long unsigned int swapped;
    struct list_head shrinklist;
    struct list_head swaplist;
    struct shared_policy policy;
    struct simple_xattrs xattrs;
    atomic_t stop_eviction;
    struct inode vfs_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct shmem_inode_info {
    spinlock_t lock;
    unsigned int seals;
    long unsigned int flags;
    long unsigned int alloced;
    long unsigned int swapped;
    struct list_head shrinklist;
    struct list_head swaplist;
    struct shared_policy policy;
    struct simple_xattrs xattrs;
    atomic_t stop_eviction;
    struct inode vfs_inode;
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
struct shmem_inode_info {
    spinlock_t lock;
    unsigned int seals;
    long unsigned int flags;
    long unsigned int alloced;
    long unsigned int swapped;
    struct list_head shrinklist;
    struct list_head swaplist;
    struct shared_policy policy;
    struct simple_xattrs xattrs;
    atomic_t stop_eviction;
    struct inode vfs_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct shmem_inode_info {
    spinlock_t lock;
    unsigned int seals;
    long unsigned int flags;
    long unsigned int alloced;
    long unsigned int swapped;
    struct list_head shrinklist;
    struct list_head swaplist;
    struct shared_policy policy;
    struct simple_xattrs xattrs;
    atomic_t stop_eviction;
    struct inode vfs_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct shmem_inode_info {
    spinlock_t lock;
    unsigned int seals;
    long unsigned int flags;
    long unsigned int alloced;
    long unsigned int swapped;
    struct list_head shrinklist;
    struct list_head swaplist;
    struct shared_policy policy;
    struct simple_xattrs xattrs;
    atomic_t stop_eviction;
    struct inode vfs_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct shmem_inode_info {
    spinlock_t lock;
    unsigned int seals;
    long unsigned int flags;
    long unsigned int alloced;
    long unsigned int swapped;
    struct list_head shrinklist;
    struct list_head swaplist;
    struct shared_policy policy;
    struct simple_xattrs xattrs;
    atomic_t stop_eviction;
    struct inode vfs_inode;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head shrinklist</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>atomic_t stop_eviction</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int fallocend</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct timespec64 i_crtime</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int fsflags</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct offset_ctx dir_offsets</code>
</li>
<li>
<b>Field added. </b>
<code>struct dquot * i_dquot[3]</code>
</li>
</ul>
</details>
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
