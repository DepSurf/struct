# Struct: <code>dentry</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct dentry {
    unsigned int d_flags;
    seqcount_t d_seq;
    struct hlist_bl_node d_hash;
    struct dentry *d_parent;
    struct qstr d_name;
    struct inode *d_inode;
    unsigned char d_iname[32];
    struct lockref d_lockref;
    const struct dentry_operations *d_op;
    struct super_block *d_sb;
    long unsigned int d_time;
    void *d_fsdata;
    struct list_head d_lru;
    struct list_head d_child;
    struct list_head d_subdirs;
    union (anon) d_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct dentry {
    unsigned int d_flags;
    seqcount_t d_seq;
    struct hlist_bl_node d_hash;
    struct dentry *d_parent;
    struct qstr d_name;
    struct inode *d_inode;
    unsigned char d_iname[32];
    struct lockref d_lockref;
    const struct dentry_operations *d_op;
    struct super_block *d_sb;
    long unsigned int d_time;
    void *d_fsdata;
    struct list_head d_lru;
    wait_queue_head_t *d_wait;
    struct list_head d_child;
    struct list_head d_subdirs;
    union (anon) d_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct dentry {
    unsigned int d_flags;
    seqcount_t d_seq;
    struct hlist_bl_node d_hash;
    struct dentry *d_parent;
    struct qstr d_name;
    struct inode *d_inode;
    unsigned char d_iname[32];
    struct lockref d_lockref;
    const struct dentry_operations *d_op;
    struct super_block *d_sb;
    long unsigned int d_time;
    void *d_fsdata;
    struct list_head d_lru;
    wait_queue_head_t *d_wait;
    struct list_head d_child;
    struct list_head d_subdirs;
    union (anon) d_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct dentry {
    unsigned int d_flags;
    seqcount_t d_seq;
    struct hlist_bl_node d_hash;
    struct dentry *d_parent;
    struct qstr d_name;
    struct inode *d_inode;
    unsigned char d_iname[32];
    struct lockref d_lockref;
    const struct dentry_operations *d_op;
    struct super_block *d_sb;
    long unsigned int d_time;
    void *d_fsdata;
    struct list_head d_lru;
    wait_queue_head_t *d_wait;
    struct list_head d_child;
    struct list_head d_subdirs;
    union (anon) d_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dentry {
    unsigned int d_flags;
    seqcount_t d_seq;
    struct hlist_bl_node d_hash;
    struct dentry *d_parent;
    struct qstr d_name;
    struct inode *d_inode;
    unsigned char d_iname[32];
    struct lockref d_lockref;
    const struct dentry_operations *d_op;
    struct super_block *d_sb;
    long unsigned int d_time;
    void *d_fsdata;
    struct list_head d_lru;
    wait_queue_head_t *d_wait;
    struct list_head d_child;
    struct list_head d_subdirs;
    union (anon) d_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dentry {
    unsigned int d_flags;
    seqcount_t d_seq;
    struct hlist_bl_node d_hash;
    struct dentry *d_parent;
    struct qstr d_name;
    struct inode *d_inode;
    unsigned char d_iname[32];
    struct lockref d_lockref;
    const struct dentry_operations *d_op;
    struct super_block *d_sb;
    long unsigned int d_time;
    void *d_fsdata;
    struct list_head d_lru;
    wait_queue_head_t *d_wait;
    struct list_head d_child;
    struct list_head d_subdirs;
    union (anon) d_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dentry {
    unsigned int d_flags;
    seqcount_t d_seq;
    struct hlist_bl_node d_hash;
    struct dentry *d_parent;
    struct qstr d_name;
    struct inode *d_inode;
    unsigned char d_iname[32];
    struct lockref d_lockref;
    const struct dentry_operations *d_op;
    struct super_block *d_sb;
    long unsigned int d_time;
    void *d_fsdata;
    struct list_head d_lru;
    wait_queue_head_t *d_wait;
    struct list_head d_child;
    struct list_head d_subdirs;
    union (anon) d_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dentry {
    unsigned int d_flags;
    seqcount_t d_seq;
    struct hlist_bl_node d_hash;
    struct dentry *d_parent;
    struct qstr d_name;
    struct inode *d_inode;
    unsigned char d_iname[32];
    struct lockref d_lockref;
    const struct dentry_operations *d_op;
    struct super_block *d_sb;
    long unsigned int d_time;
    void *d_fsdata;
    struct list_head d_lru;
    wait_queue_head_t *d_wait;
    struct list_head d_child;
    struct list_head d_subdirs;
    union (anon) d_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dentry {
    unsigned int d_flags;
    seqcount_t d_seq;
    struct hlist_bl_node d_hash;
    struct dentry *d_parent;
    struct qstr d_name;
    struct inode *d_inode;
    unsigned char d_iname[32];
    struct lockref d_lockref;
    const struct dentry_operations *d_op;
    struct super_block *d_sb;
    long unsigned int d_time;
    void *d_fsdata;
    struct list_head d_lru;
    wait_queue_head_t *d_wait;
    struct list_head d_child;
    struct list_head d_subdirs;
    union (anon) d_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dentry {
    unsigned int d_flags;
    seqcount_t d_seq;
    struct hlist_bl_node d_hash;
    struct dentry *d_parent;
    struct qstr d_name;
    struct inode *d_inode;
    unsigned char d_iname[32];
    struct lockref d_lockref;
    const struct dentry_operations *d_op;
    struct super_block *d_sb;
    long unsigned int d_time;
    void *d_fsdata;
    struct list_head d_lru;
    wait_queue_head_t *d_wait;
    struct list_head d_child;
    struct list_head d_subdirs;
    union (anon) d_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dentry {
    unsigned int d_flags;
    seqcount_spinlock_t d_seq;
    struct hlist_bl_node d_hash;
    struct dentry *d_parent;
    struct qstr d_name;
    struct inode *d_inode;
    unsigned char d_iname[32];
    struct lockref d_lockref;
    const struct dentry_operations *d_op;
    struct super_block *d_sb;
    long unsigned int d_time;
    void *d_fsdata;
    struct list_head d_lru;
    wait_queue_head_t *d_wait;
    struct list_head d_child;
    struct list_head d_subdirs;
    union (anon) d_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dentry {
    unsigned int d_flags;
    seqcount_spinlock_t d_seq;
    struct hlist_bl_node d_hash;
    struct dentry *d_parent;
    struct qstr d_name;
    struct inode *d_inode;
    unsigned char d_iname[32];
    struct lockref d_lockref;
    const struct dentry_operations *d_op;
    struct super_block *d_sb;
    long unsigned int d_time;
    void *d_fsdata;
    struct list_head d_lru;
    wait_queue_head_t *d_wait;
    struct list_head d_child;
    struct list_head d_subdirs;
    union (anon) d_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dentry {
    unsigned int d_flags;
    seqcount_spinlock_t d_seq;
    struct hlist_bl_node d_hash;
    struct dentry *d_parent;
    struct qstr d_name;
    struct inode *d_inode;
    unsigned char d_iname[32];
    struct lockref d_lockref;
    const struct dentry_operations *d_op;
    struct super_block *d_sb;
    long unsigned int d_time;
    void *d_fsdata;
    struct list_head d_lru;
    wait_queue_head_t *d_wait;
    struct list_head d_child;
    struct list_head d_subdirs;
    union (anon) d_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dentry {
    unsigned int d_flags;
    seqcount_spinlock_t d_seq;
    struct hlist_bl_node d_hash;
    struct dentry *d_parent;
    struct qstr d_name;
    struct inode *d_inode;
    unsigned char d_iname[32];
    struct lockref d_lockref;
    const struct dentry_operations *d_op;
    struct super_block *d_sb;
    long unsigned int d_time;
    void *d_fsdata;
    struct list_head d_lru;
    wait_queue_head_t *d_wait;
    struct list_head d_child;
    struct list_head d_subdirs;
    union (anon) d_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dentry {
    unsigned int d_flags;
    seqcount_spinlock_t d_seq;
    struct hlist_bl_node d_hash;
    struct dentry *d_parent;
    struct qstr d_name;
    struct inode *d_inode;
    unsigned char d_iname[32];
    struct lockref d_lockref;
    const struct dentry_operations *d_op;
    struct super_block *d_sb;
    long unsigned int d_time;
    void *d_fsdata;
    struct list_head d_lru;
    wait_queue_head_t *d_wait;
    struct list_head d_child;
    struct list_head d_subdirs;
    union (anon) d_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dentry {
    unsigned int d_flags;
    seqcount_spinlock_t d_seq;
    struct hlist_bl_node d_hash;
    struct dentry *d_parent;
    struct qstr d_name;
    struct inode *d_inode;
    unsigned char d_iname[32];
    struct lockref d_lockref;
    const struct dentry_operations *d_op;
    struct super_block *d_sb;
    long unsigned int d_time;
    void *d_fsdata;
    struct list_head d_lru;
    wait_queue_head_t *d_wait;
    struct list_head d_child;
    struct list_head d_subdirs;
    union (anon) d_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dentry {
    unsigned int d_flags;
    seqcount_spinlock_t d_seq;
    struct hlist_bl_node d_hash;
    struct dentry *d_parent;
    struct qstr d_name;
    struct inode *d_inode;
    unsigned char d_iname[40];
    struct lockref d_lockref;
    const struct dentry_operations *d_op;
    struct super_block *d_sb;
    long unsigned int d_time;
    void *d_fsdata;
    struct list_head d_lru;
    wait_queue_head_t *d_wait;
    struct hlist_node d_sib;
    struct hlist_head d_children;
    union (anon) d_u;
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
struct dentry {
    unsigned int d_flags;
    seqcount_t d_seq;
    struct hlist_bl_node d_hash;
    struct dentry *d_parent;
    struct qstr d_name;
    struct inode *d_inode;
    unsigned char d_iname[32];
    struct lockref d_lockref;
    const struct dentry_operations *d_op;
    struct super_block *d_sb;
    long unsigned int d_time;
    void *d_fsdata;
    struct list_head d_lru;
    wait_queue_head_t *d_wait;
    struct list_head d_child;
    struct list_head d_subdirs;
    union (anon) d_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dentry {
    unsigned int d_flags;
    seqcount_t d_seq;
    struct hlist_bl_node d_hash;
    struct dentry *d_parent;
    struct qstr d_name;
    struct inode *d_inode;
    unsigned char d_iname[36];
    struct lockref d_lockref;
    const struct dentry_operations *d_op;
    struct super_block *d_sb;
    long unsigned int d_time;
    void *d_fsdata;
    struct list_head d_lru;
    wait_queue_head_t *d_wait;
    struct list_head d_child;
    struct list_head d_subdirs;
    union (anon) d_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dentry {
    unsigned int d_flags;
    seqcount_t d_seq;
    struct hlist_bl_node d_hash;
    struct dentry *d_parent;
    struct qstr d_name;
    struct inode *d_inode;
    unsigned char d_iname[32];
    struct lockref d_lockref;
    const struct dentry_operations *d_op;
    struct super_block *d_sb;
    long unsigned int d_time;
    void *d_fsdata;
    struct list_head d_lru;
    wait_queue_head_t *d_wait;
    struct list_head d_child;
    struct list_head d_subdirs;
    union (anon) d_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dentry {
    unsigned int d_flags;
    seqcount_t d_seq;
    struct hlist_bl_node d_hash;
    struct dentry *d_parent;
    struct qstr d_name;
    struct inode *d_inode;
    unsigned char d_iname[32];
    struct lockref d_lockref;
    const struct dentry_operations *d_op;
    struct super_block *d_sb;
    long unsigned int d_time;
    void *d_fsdata;
    struct list_head d_lru;
    wait_queue_head_t *d_wait;
    struct list_head d_child;
    struct list_head d_subdirs;
    union (anon) d_u;
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
struct dentry {
    unsigned int d_flags;
    seqcount_t d_seq;
    struct hlist_bl_node d_hash;
    struct dentry *d_parent;
    struct qstr d_name;
    struct inode *d_inode;
    unsigned char d_iname[32];
    struct lockref d_lockref;
    const struct dentry_operations *d_op;
    struct super_block *d_sb;
    long unsigned int d_time;
    void *d_fsdata;
    struct list_head d_lru;
    wait_queue_head_t *d_wait;
    struct list_head d_child;
    struct list_head d_subdirs;
    union (anon) d_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dentry {
    unsigned int d_flags;
    seqcount_t d_seq;
    struct hlist_bl_node d_hash;
    struct dentry *d_parent;
    struct qstr d_name;
    struct inode *d_inode;
    unsigned char d_iname[32];
    struct lockref d_lockref;
    const struct dentry_operations *d_op;
    struct super_block *d_sb;
    long unsigned int d_time;
    void *d_fsdata;
    struct list_head d_lru;
    wait_queue_head_t *d_wait;
    struct list_head d_child;
    struct list_head d_subdirs;
    union (anon) d_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dentry {
    unsigned int d_flags;
    seqcount_t d_seq;
    struct hlist_bl_node d_hash;
    struct dentry *d_parent;
    struct qstr d_name;
    struct inode *d_inode;
    unsigned char d_iname[32];
    struct lockref d_lockref;
    const struct dentry_operations *d_op;
    struct super_block *d_sb;
    long unsigned int d_time;
    void *d_fsdata;
    struct list_head d_lru;
    wait_queue_head_t *d_wait;
    struct list_head d_child;
    struct list_head d_subdirs;
    union (anon) d_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dentry {
    unsigned int d_flags;
    seqcount_t d_seq;
    struct hlist_bl_node d_hash;
    struct dentry *d_parent;
    struct qstr d_name;
    struct inode *d_inode;
    unsigned char d_iname[32];
    struct lockref d_lockref;
    const struct dentry_operations *d_op;
    struct super_block *d_sb;
    long unsigned int d_time;
    void *d_fsdata;
    struct list_head d_lru;
    wait_queue_head_t *d_wait;
    struct list_head d_child;
    struct list_head d_subdirs;
    union (anon) d_u;
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
<code>wait_queue_head_t *d_wait</code>
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
<b>Field type changed. </b>
<code>seqcount_t d_seq</code> ➡️ <code>seqcount_spinlock_t d_seq</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct hlist_node d_sib</code>
</li>
<li>
<b>Field added. </b>
<code>struct hlist_head d_children</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head d_child</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head d_subdirs</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned char d_iname[32]</code> ➡️ <code>unsigned char d_iname[40]</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>unsigned char d_iname[32]</code> ➡️ <code>unsigned char d_iname[36]</code>
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
