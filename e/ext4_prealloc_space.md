# Struct: <code>ext4_prealloc_space</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct ext4_prealloc_space {
    struct list_head pa_inode_list;
    struct list_head pa_group_list;
    union (anon) u;
    spinlock_t pa_lock;
    atomic_t pa_count;
    unsigned int pa_deleted;
    ext4_fsblk_t pa_pstart;
    ext4_lblk_t pa_lstart;
    ext4_grpblk_t pa_len;
    ext4_grpblk_t pa_free;
    short unsigned int pa_type;
    spinlock_t *pa_obj_lock;
    struct inode *pa_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ext4_prealloc_space {
    struct list_head pa_inode_list;
    struct list_head pa_group_list;
    union (anon) u;
    spinlock_t pa_lock;
    atomic_t pa_count;
    unsigned int pa_deleted;
    ext4_fsblk_t pa_pstart;
    ext4_lblk_t pa_lstart;
    ext4_grpblk_t pa_len;
    ext4_grpblk_t pa_free;
    short unsigned int pa_type;
    spinlock_t *pa_obj_lock;
    struct inode *pa_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ext4_prealloc_space {
    struct list_head pa_inode_list;
    struct list_head pa_group_list;
    union (anon) u;
    spinlock_t pa_lock;
    atomic_t pa_count;
    unsigned int pa_deleted;
    ext4_fsblk_t pa_pstart;
    ext4_lblk_t pa_lstart;
    ext4_grpblk_t pa_len;
    ext4_grpblk_t pa_free;
    short unsigned int pa_type;
    spinlock_t *pa_obj_lock;
    struct inode *pa_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ext4_prealloc_space {
    struct list_head pa_inode_list;
    struct list_head pa_group_list;
    union (anon) u;
    spinlock_t pa_lock;
    atomic_t pa_count;
    unsigned int pa_deleted;
    ext4_fsblk_t pa_pstart;
    ext4_lblk_t pa_lstart;
    ext4_grpblk_t pa_len;
    ext4_grpblk_t pa_free;
    short unsigned int pa_type;
    spinlock_t *pa_obj_lock;
    struct inode *pa_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ext4_prealloc_space {
    struct list_head pa_inode_list;
    struct list_head pa_group_list;
    union (anon) u;
    spinlock_t pa_lock;
    atomic_t pa_count;
    unsigned int pa_deleted;
    ext4_fsblk_t pa_pstart;
    ext4_lblk_t pa_lstart;
    ext4_grpblk_t pa_len;
    ext4_grpblk_t pa_free;
    short unsigned int pa_type;
    spinlock_t *pa_obj_lock;
    struct inode *pa_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ext4_prealloc_space {
    struct list_head pa_inode_list;
    struct list_head pa_group_list;
    union (anon) u;
    spinlock_t pa_lock;
    atomic_t pa_count;
    unsigned int pa_deleted;
    ext4_fsblk_t pa_pstart;
    ext4_lblk_t pa_lstart;
    ext4_grpblk_t pa_len;
    ext4_grpblk_t pa_free;
    short unsigned int pa_type;
    spinlock_t *pa_obj_lock;
    struct inode *pa_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ext4_prealloc_space {
    struct list_head pa_inode_list;
    struct list_head pa_group_list;
    union (anon) u;
    spinlock_t pa_lock;
    atomic_t pa_count;
    unsigned int pa_deleted;
    ext4_fsblk_t pa_pstart;
    ext4_lblk_t pa_lstart;
    ext4_grpblk_t pa_len;
    ext4_grpblk_t pa_free;
    short unsigned int pa_type;
    spinlock_t *pa_obj_lock;
    struct inode *pa_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ext4_prealloc_space {
    struct list_head pa_inode_list;
    struct list_head pa_group_list;
    union (anon) u;
    spinlock_t pa_lock;
    atomic_t pa_count;
    unsigned int pa_deleted;
    ext4_fsblk_t pa_pstart;
    ext4_lblk_t pa_lstart;
    ext4_grpblk_t pa_len;
    ext4_grpblk_t pa_free;
    short unsigned int pa_type;
    spinlock_t *pa_obj_lock;
    struct inode *pa_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ext4_prealloc_space {
    struct list_head pa_inode_list;
    struct list_head pa_group_list;
    union (anon) u;
    spinlock_t pa_lock;
    atomic_t pa_count;
    unsigned int pa_deleted;
    ext4_fsblk_t pa_pstart;
    ext4_lblk_t pa_lstart;
    ext4_grpblk_t pa_len;
    ext4_grpblk_t pa_free;
    short unsigned int pa_type;
    spinlock_t *pa_obj_lock;
    struct inode *pa_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ext4_prealloc_space {
    struct list_head pa_inode_list;
    struct list_head pa_group_list;
    union (anon) u;
    spinlock_t pa_lock;
    atomic_t pa_count;
    unsigned int pa_deleted;
    ext4_fsblk_t pa_pstart;
    ext4_lblk_t pa_lstart;
    ext4_grpblk_t pa_len;
    ext4_grpblk_t pa_free;
    short unsigned int pa_type;
    spinlock_t *pa_obj_lock;
    struct inode *pa_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ext4_prealloc_space {
    struct list_head pa_inode_list;
    struct list_head pa_group_list;
    union (anon) u;
    spinlock_t pa_lock;
    atomic_t pa_count;
    unsigned int pa_deleted;
    ext4_fsblk_t pa_pstart;
    ext4_lblk_t pa_lstart;
    ext4_grpblk_t pa_len;
    ext4_grpblk_t pa_free;
    short unsigned int pa_type;
    spinlock_t *pa_obj_lock;
    struct inode *pa_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ext4_prealloc_space {
    struct list_head pa_inode_list;
    struct list_head pa_group_list;
    union (anon) u;
    spinlock_t pa_lock;
    atomic_t pa_count;
    unsigned int pa_deleted;
    ext4_fsblk_t pa_pstart;
    ext4_lblk_t pa_lstart;
    ext4_grpblk_t pa_len;
    ext4_grpblk_t pa_free;
    short unsigned int pa_type;
    spinlock_t *pa_obj_lock;
    struct inode *pa_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ext4_prealloc_space {
    struct list_head pa_inode_list;
    struct list_head pa_group_list;
    union (anon) u;
    spinlock_t pa_lock;
    atomic_t pa_count;
    unsigned int pa_deleted;
    ext4_fsblk_t pa_pstart;
    ext4_lblk_t pa_lstart;
    ext4_grpblk_t pa_len;
    ext4_grpblk_t pa_free;
    short unsigned int pa_type;
    spinlock_t *pa_obj_lock;
    struct inode *pa_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ext4_prealloc_space {
    struct list_head pa_inode_list;
    struct list_head pa_group_list;
    union (anon) u;
    spinlock_t pa_lock;
    atomic_t pa_count;
    unsigned int pa_deleted;
    ext4_fsblk_t pa_pstart;
    ext4_lblk_t pa_lstart;
    ext4_grpblk_t pa_len;
    ext4_grpblk_t pa_free;
    short unsigned int pa_type;
    spinlock_t *pa_obj_lock;
    struct inode *pa_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ext4_prealloc_space {
    struct list_head pa_inode_list;
    struct list_head pa_group_list;
    union (anon) u;
    spinlock_t pa_lock;
    atomic_t pa_count;
    unsigned int pa_deleted;
    ext4_fsblk_t pa_pstart;
    ext4_lblk_t pa_lstart;
    ext4_grpblk_t pa_len;
    ext4_grpblk_t pa_free;
    short unsigned int pa_type;
    spinlock_t *pa_obj_lock;
    struct inode *pa_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ext4_prealloc_space {
    union (anon) pa_node;
    struct list_head pa_group_list;
    union (anon) u;
    spinlock_t pa_lock;
    atomic_t pa_count;
    unsigned int pa_deleted;
    ext4_fsblk_t pa_pstart;
    ext4_lblk_t pa_lstart;
    ext4_grpblk_t pa_len;
    ext4_grpblk_t pa_free;
    short unsigned int pa_type;
    union (anon) pa_node_lock;
    struct inode *pa_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ext4_prealloc_space {
    union (anon) pa_node;
    struct list_head pa_group_list;
    union (anon) u;
    spinlock_t pa_lock;
    atomic_t pa_count;
    unsigned int pa_deleted;
    ext4_fsblk_t pa_pstart;
    ext4_lblk_t pa_lstart;
    ext4_grpblk_t pa_len;
    ext4_grpblk_t pa_free;
    short unsigned int pa_type;
    union (anon) pa_node_lock;
    struct inode *pa_inode;
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
struct ext4_prealloc_space {
    struct list_head pa_inode_list;
    struct list_head pa_group_list;
    union (anon) u;
    spinlock_t pa_lock;
    atomic_t pa_count;
    unsigned int pa_deleted;
    ext4_fsblk_t pa_pstart;
    ext4_lblk_t pa_lstart;
    ext4_grpblk_t pa_len;
    ext4_grpblk_t pa_free;
    short unsigned int pa_type;
    spinlock_t *pa_obj_lock;
    struct inode *pa_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ext4_prealloc_space {
    struct list_head pa_inode_list;
    struct list_head pa_group_list;
    union (anon) u;
    spinlock_t pa_lock;
    atomic_t pa_count;
    unsigned int pa_deleted;
    ext4_fsblk_t pa_pstart;
    ext4_lblk_t pa_lstart;
    ext4_grpblk_t pa_len;
    ext4_grpblk_t pa_free;
    short unsigned int pa_type;
    spinlock_t *pa_obj_lock;
    struct inode *pa_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ext4_prealloc_space {
    struct list_head pa_inode_list;
    struct list_head pa_group_list;
    union (anon) u;
    spinlock_t pa_lock;
    atomic_t pa_count;
    unsigned int pa_deleted;
    ext4_fsblk_t pa_pstart;
    ext4_lblk_t pa_lstart;
    ext4_grpblk_t pa_len;
    ext4_grpblk_t pa_free;
    short unsigned int pa_type;
    spinlock_t *pa_obj_lock;
    struct inode *pa_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ext4_prealloc_space {
    struct list_head pa_inode_list;
    struct list_head pa_group_list;
    union (anon) u;
    spinlock_t pa_lock;
    atomic_t pa_count;
    unsigned int pa_deleted;
    ext4_fsblk_t pa_pstart;
    ext4_lblk_t pa_lstart;
    ext4_grpblk_t pa_len;
    ext4_grpblk_t pa_free;
    short unsigned int pa_type;
    spinlock_t *pa_obj_lock;
    struct inode *pa_inode;
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
struct ext4_prealloc_space {
    struct list_head pa_inode_list;
    struct list_head pa_group_list;
    union (anon) u;
    spinlock_t pa_lock;
    atomic_t pa_count;
    unsigned int pa_deleted;
    ext4_fsblk_t pa_pstart;
    ext4_lblk_t pa_lstart;
    ext4_grpblk_t pa_len;
    ext4_grpblk_t pa_free;
    short unsigned int pa_type;
    spinlock_t *pa_obj_lock;
    struct inode *pa_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ext4_prealloc_space {
    struct list_head pa_inode_list;
    struct list_head pa_group_list;
    union (anon) u;
    spinlock_t pa_lock;
    atomic_t pa_count;
    unsigned int pa_deleted;
    ext4_fsblk_t pa_pstart;
    ext4_lblk_t pa_lstart;
    ext4_grpblk_t pa_len;
    ext4_grpblk_t pa_free;
    short unsigned int pa_type;
    spinlock_t *pa_obj_lock;
    struct inode *pa_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ext4_prealloc_space {
    struct list_head pa_inode_list;
    struct list_head pa_group_list;
    union (anon) u;
    spinlock_t pa_lock;
    atomic_t pa_count;
    unsigned int pa_deleted;
    ext4_fsblk_t pa_pstart;
    ext4_lblk_t pa_lstart;
    ext4_grpblk_t pa_len;
    ext4_grpblk_t pa_free;
    short unsigned int pa_type;
    spinlock_t *pa_obj_lock;
    struct inode *pa_inode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ext4_prealloc_space {
    struct list_head pa_inode_list;
    struct list_head pa_group_list;
    union (anon) u;
    spinlock_t pa_lock;
    atomic_t pa_count;
    unsigned int pa_deleted;
    ext4_fsblk_t pa_pstart;
    ext4_lblk_t pa_lstart;
    ext4_grpblk_t pa_len;
    ext4_grpblk_t pa_free;
    short unsigned int pa_type;
    spinlock_t *pa_obj_lock;
    struct inode *pa_inode;
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>union (anon) pa_node</code>
</li>
<li>
<b>Field added. </b>
<code>union (anon) pa_node_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head pa_inode_list</code>
</li>
<li>
<b>Field removed. </b>
<code>spinlock_t *pa_obj_lock</code>
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
