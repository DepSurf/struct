# Struct: <code>fuse_inode</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct fuse_inode {
    struct inode inode;
    u64 nodeid;
    u64 nlookup;
    struct fuse_forget_link *forget;
    u64 i_time;
    umode_t orig_i_mode;
    u64 orig_ino;
    u64 attr_version;
    struct list_head write_files;
    struct list_head queued_writes;
    int writectr;
    wait_queue_head_t page_waitq;
    struct list_head writepages;
    long unsigned int state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct fuse_inode {
    struct inode inode;
    u64 nodeid;
    u64 nlookup;
    struct fuse_forget_link *forget;
    u64 i_time;
    umode_t orig_i_mode;
    u64 orig_ino;
    u64 attr_version;
    struct list_head write_files;
    struct list_head queued_writes;
    int writectr;
    wait_queue_head_t page_waitq;
    struct list_head writepages;
    long unsigned int state;
    struct mutex mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct fuse_inode {
    struct inode inode;
    u64 nodeid;
    u64 nlookup;
    struct fuse_forget_link *forget;
    u64 i_time;
    umode_t orig_i_mode;
    u64 orig_ino;
    u64 attr_version;
    struct list_head write_files;
    struct list_head queued_writes;
    int writectr;
    wait_queue_head_t page_waitq;
    struct list_head writepages;
    long unsigned int state;
    struct mutex mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct fuse_inode {
    struct inode inode;
    u64 nodeid;
    u64 nlookup;
    struct fuse_forget_link *forget;
    u64 i_time;
    umode_t orig_i_mode;
    u64 orig_ino;
    u64 attr_version;
    struct list_head write_files;
    struct list_head queued_writes;
    int writectr;
    wait_queue_head_t page_waitq;
    struct list_head writepages;
    long unsigned int state;
    struct mutex mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct fuse_inode {
    struct inode inode;
    u64 nodeid;
    u64 nlookup;
    struct fuse_forget_link *forget;
    u64 i_time;
    umode_t orig_i_mode;
    u64 orig_ino;
    u64 attr_version;
    struct list_head write_files;
    struct list_head queued_writes;
    int writectr;
    wait_queue_head_t page_waitq;
    struct list_head writepages;
    long unsigned int state;
    struct mutex mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct fuse_inode {
    struct inode inode;
    u64 nodeid;
    u64 nlookup;
    struct fuse_forget_link *forget;
    u64 i_time;
    umode_t orig_i_mode;
    u64 orig_ino;
    u64 attr_version;
    struct list_head write_files;
    struct list_head queued_writes;
    int writectr;
    wait_queue_head_t page_waitq;
    struct list_head writepages;
    long unsigned int state;
    struct mutex mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct fuse_inode {
    struct inode inode;
    u64 nodeid;
    u64 nlookup;
    struct fuse_forget_link *forget;
    u64 i_time;
    u32 inval_mask;
    umode_t orig_i_mode;
    u64 orig_ino;
    u64 attr_version;
    struct list_head write_files;
    struct list_head queued_writes;
    int writectr;
    wait_queue_head_t page_waitq;
    struct list_head writepages;
    struct (anon) rdc;
    long unsigned int state;
    struct mutex mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct fuse_inode {
    struct inode inode;
    u64 nodeid;
    u64 nlookup;
    struct fuse_forget_link *forget;
    u64 i_time;
    u32 inval_mask;
    umode_t orig_i_mode;
    u64 orig_ino;
    u64 attr_version;
    struct list_head write_files;
    struct list_head queued_writes;
    int writectr;
    wait_queue_head_t page_waitq;
    struct list_head writepages;
    struct (anon) rdc;
    long unsigned int state;
    struct mutex mutex;
    spinlock_t lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct fuse_inode {
    struct inode inode;
    u64 nodeid;
    u64 nlookup;
    struct fuse_forget_link *forget;
    u64 i_time;
    u32 inval_mask;
    umode_t orig_i_mode;
    u64 orig_ino;
    u64 attr_version;
    struct list_head write_files;
    struct list_head queued_writes;
    int writectr;
    wait_queue_head_t page_waitq;
    struct list_head writepages;
    struct (anon) rdc;
    long unsigned int state;
    struct mutex mutex;
    spinlock_t lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct fuse_inode {
    struct inode inode;
    u64 nodeid;
    u64 nlookup;
    struct fuse_forget_link *forget;
    u64 i_time;
    u32 inval_mask;
    umode_t orig_i_mode;
    u64 orig_ino;
    u64 attr_version;
    struct list_head write_files;
    struct list_head queued_writes;
    int writectr;
    wait_queue_head_t page_waitq;
    struct rb_root writepages;
    struct (anon) rdc;
    long unsigned int state;
    struct mutex mutex;
    spinlock_t lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct fuse_inode {
    struct inode inode;
    u64 nodeid;
    u64 nlookup;
    struct fuse_forget_link *forget;
    u64 i_time;
    u32 inval_mask;
    umode_t orig_i_mode;
    u64 orig_ino;
    u64 attr_version;
    struct list_head write_files;
    struct list_head queued_writes;
    int writectr;
    wait_queue_head_t page_waitq;
    struct rb_root writepages;
    struct (anon) rdc;
    long unsigned int state;
    struct mutex mutex;
    spinlock_t lock;
    struct rw_semaphore i_mmap_sem;
    struct fuse_inode_dax *dax;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct fuse_inode {
    struct inode inode;
    u64 nodeid;
    u64 nlookup;
    struct fuse_forget_link *forget;
    u64 i_time;
    u32 inval_mask;
    umode_t orig_i_mode;
    u64 orig_ino;
    u64 attr_version;
    struct list_head write_files;
    struct list_head queued_writes;
    int writectr;
    wait_queue_head_t page_waitq;
    struct rb_root writepages;
    struct (anon) rdc;
    long unsigned int state;
    struct mutex mutex;
    spinlock_t lock;
    struct rw_semaphore i_mmap_sem;
    struct fuse_inode_dax *dax;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct fuse_inode {
    struct inode inode;
    u64 nodeid;
    u64 nlookup;
    struct fuse_forget_link *forget;
    u64 i_time;
    u32 inval_mask;
    umode_t orig_i_mode;
    u64 orig_ino;
    u64 attr_version;
    struct list_head write_files;
    struct list_head queued_writes;
    int writectr;
    wait_queue_head_t page_waitq;
    struct rb_root writepages;
    struct (anon) rdc;
    long unsigned int state;
    struct mutex mutex;
    spinlock_t lock;
    struct fuse_inode_dax *dax;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct fuse_inode {
    struct inode inode;
    u64 nodeid;
    u64 nlookup;
    struct fuse_forget_link *forget;
    u64 i_time;
    u32 inval_mask;
    umode_t orig_i_mode;
    u64 orig_ino;
    u64 attr_version;
    struct list_head write_files;
    struct list_head queued_writes;
    int writectr;
    wait_queue_head_t page_waitq;
    struct rb_root writepages;
    struct (anon) rdc;
    long unsigned int state;
    struct mutex mutex;
    spinlock_t lock;
    struct fuse_inode_dax *dax;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct fuse_inode {
    struct inode inode;
    u64 nodeid;
    u64 nlookup;
    struct fuse_forget_link *forget;
    u64 i_time;
    u32 inval_mask;
    umode_t orig_i_mode;
    u64 orig_ino;
    u64 attr_version;
    struct list_head write_files;
    struct list_head queued_writes;
    int writectr;
    wait_queue_head_t page_waitq;
    struct rb_root writepages;
    struct (anon) rdc;
    long unsigned int state;
    struct mutex mutex;
    spinlock_t lock;
    struct fuse_inode_dax *dax;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct fuse_inode {
    struct inode inode;
    u64 nodeid;
    u64 nlookup;
    struct fuse_forget_link *forget;
    u64 i_time;
    u32 inval_mask;
    umode_t orig_i_mode;
    u64 orig_ino;
    u64 attr_version;
    struct list_head write_files;
    struct list_head queued_writes;
    int writectr;
    wait_queue_head_t page_waitq;
    struct rb_root writepages;
    struct (anon) rdc;
    long unsigned int state;
    struct mutex mutex;
    spinlock_t lock;
    struct fuse_inode_dax *dax;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct fuse_inode {
    struct inode inode;
    u64 nodeid;
    u64 nlookup;
    struct fuse_forget_link *forget;
    u64 i_time;
    u32 inval_mask;
    umode_t orig_i_mode;
    struct timespec64 i_btime;
    u64 orig_ino;
    u64 attr_version;
    struct list_head write_files;
    struct list_head queued_writes;
    int writectr;
    wait_queue_head_t page_waitq;
    struct rb_root writepages;
    struct (anon) rdc;
    long unsigned int state;
    struct mutex mutex;
    spinlock_t lock;
    struct fuse_inode_dax *dax;
    struct fuse_submount_lookup *submount_lookup;
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
struct fuse_inode {
    struct inode inode;
    u64 nodeid;
    u64 nlookup;
    struct fuse_forget_link *forget;
    u64 i_time;
    u32 inval_mask;
    umode_t orig_i_mode;
    u64 orig_ino;
    u64 attr_version;
    struct list_head write_files;
    struct list_head queued_writes;
    int writectr;
    wait_queue_head_t page_waitq;
    struct list_head writepages;
    struct (anon) rdc;
    long unsigned int state;
    struct mutex mutex;
    spinlock_t lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct fuse_inode {
    struct inode inode;
    u64 nodeid;
    u64 nlookup;
    struct fuse_forget_link *forget;
    u64 i_time;
    u32 inval_mask;
    umode_t orig_i_mode;
    u64 orig_ino;
    u64 attr_version;
    struct list_head write_files;
    struct list_head queued_writes;
    int writectr;
    wait_queue_head_t page_waitq;
    struct list_head writepages;
    struct (anon) rdc;
    long unsigned int state;
    struct mutex mutex;
    spinlock_t lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct fuse_inode {
    struct inode inode;
    u64 nodeid;
    u64 nlookup;
    struct fuse_forget_link *forget;
    u64 i_time;
    u32 inval_mask;
    umode_t orig_i_mode;
    u64 orig_ino;
    u64 attr_version;
    struct list_head write_files;
    struct list_head queued_writes;
    int writectr;
    wait_queue_head_t page_waitq;
    struct list_head writepages;
    struct (anon) rdc;
    long unsigned int state;
    struct mutex mutex;
    spinlock_t lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct fuse_inode {
    struct inode inode;
    u64 nodeid;
    u64 nlookup;
    struct fuse_forget_link *forget;
    u64 i_time;
    u32 inval_mask;
    umode_t orig_i_mode;
    u64 orig_ino;
    u64 attr_version;
    struct list_head write_files;
    struct list_head queued_writes;
    int writectr;
    wait_queue_head_t page_waitq;
    struct list_head writepages;
    struct (anon) rdc;
    long unsigned int state;
    struct mutex mutex;
    spinlock_t lock;
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
struct fuse_inode {
    struct inode inode;
    u64 nodeid;
    u64 nlookup;
    struct fuse_forget_link *forget;
    u64 i_time;
    u32 inval_mask;
    umode_t orig_i_mode;
    u64 orig_ino;
    u64 attr_version;
    struct list_head write_files;
    struct list_head queued_writes;
    int writectr;
    wait_queue_head_t page_waitq;
    struct list_head writepages;
    struct (anon) rdc;
    long unsigned int state;
    struct mutex mutex;
    spinlock_t lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct fuse_inode {
    struct inode inode;
    u64 nodeid;
    u64 nlookup;
    struct fuse_forget_link *forget;
    u64 i_time;
    u32 inval_mask;
    umode_t orig_i_mode;
    u64 orig_ino;
    u64 attr_version;
    struct list_head write_files;
    struct list_head queued_writes;
    int writectr;
    wait_queue_head_t page_waitq;
    struct list_head writepages;
    struct (anon) rdc;
    long unsigned int state;
    struct mutex mutex;
    spinlock_t lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct fuse_inode {
    struct inode inode;
    u64 nodeid;
    u64 nlookup;
    struct fuse_forget_link *forget;
    u64 i_time;
    u32 inval_mask;
    umode_t orig_i_mode;
    u64 orig_ino;
    u64 attr_version;
    struct list_head write_files;
    struct list_head queued_writes;
    int writectr;
    wait_queue_head_t page_waitq;
    struct list_head writepages;
    struct (anon) rdc;
    long unsigned int state;
    struct mutex mutex;
    spinlock_t lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct fuse_inode {
    struct inode inode;
    u64 nodeid;
    u64 nlookup;
    struct fuse_forget_link *forget;
    u64 i_time;
    u32 inval_mask;
    umode_t orig_i_mode;
    u64 orig_ino;
    u64 attr_version;
    struct list_head write_files;
    struct list_head queued_writes;
    int writectr;
    wait_queue_head_t page_waitq;
    struct list_head writepages;
    struct (anon) rdc;
    long unsigned int state;
    struct mutex mutex;
    spinlock_t lock;
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
<code>struct mutex mutex</code>
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
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 inval_mask</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) rdc</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>spinlock_t lock</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct list_head writepages</code> ➡️ <code>struct rb_root writepages</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct rw_semaphore i_mmap_sem</code>
</li>
<li>
<b>Field added. </b>
<code>struct fuse_inode_dax *dax</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct rw_semaphore i_mmap_sem</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct timespec64 i_btime</code>
</li>
<li>
<b>Field added. </b>
<code>struct fuse_submount_lookup *submount_lookup</code>
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
