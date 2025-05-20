# Struct: <code>fsnotify_mark_connector</code>

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
struct fsnotify_mark_connector {
    spinlock_t lock;
    unsigned int flags;
    struct inode *inode;
    struct vfsmount *mnt;
    struct hlist_head list;
    struct fsnotify_mark_connector *destroy_next;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct fsnotify_mark_connector {
    spinlock_t lock;
    unsigned int flags;
    struct inode *inode;
    struct vfsmount *mnt;
    struct hlist_head list;
    struct fsnotify_mark_connector *destroy_next;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct fsnotify_mark_connector {
    spinlock_t lock;
    unsigned int type;
    struct inode *inode;
    struct vfsmount *mnt;
    struct fsnotify_mark_connector *destroy_next;
    struct hlist_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct fsnotify_mark_connector {
    spinlock_t lock;
    unsigned int type;
    fsnotify_connp_t *obj;
    struct fsnotify_mark_connector *destroy_next;
    struct hlist_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct fsnotify_mark_connector {
    spinlock_t lock;
    short unsigned int type;
    short unsigned int flags;
    __kernel_fsid_t fsid;
    fsnotify_connp_t *obj;
    struct fsnotify_mark_connector *destroy_next;
    struct hlist_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct fsnotify_mark_connector {
    spinlock_t lock;
    short unsigned int type;
    short unsigned int flags;
    __kernel_fsid_t fsid;
    fsnotify_connp_t *obj;
    struct fsnotify_mark_connector *destroy_next;
    struct hlist_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct fsnotify_mark_connector {
    spinlock_t lock;
    short unsigned int type;
    short unsigned int flags;
    __kernel_fsid_t fsid;
    fsnotify_connp_t *obj;
    struct fsnotify_mark_connector *destroy_next;
    struct hlist_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct fsnotify_mark_connector {
    spinlock_t lock;
    short unsigned int type;
    short unsigned int flags;
    __kernel_fsid_t fsid;
    fsnotify_connp_t *obj;
    struct fsnotify_mark_connector *destroy_next;
    struct hlist_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct fsnotify_mark_connector {
    spinlock_t lock;
    short unsigned int type;
    short unsigned int flags;
    __kernel_fsid_t fsid;
    fsnotify_connp_t *obj;
    struct fsnotify_mark_connector *destroy_next;
    struct hlist_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct fsnotify_mark_connector {
    spinlock_t lock;
    short unsigned int type;
    short unsigned int flags;
    __kernel_fsid_t fsid;
    fsnotify_connp_t *obj;
    struct fsnotify_mark_connector *destroy_next;
    struct hlist_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct fsnotify_mark_connector {
    spinlock_t lock;
    short unsigned int type;
    short unsigned int flags;
    __kernel_fsid_t fsid;
    fsnotify_connp_t *obj;
    struct fsnotify_mark_connector *destroy_next;
    struct hlist_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct fsnotify_mark_connector {
    spinlock_t lock;
    short unsigned int type;
    short unsigned int flags;
    __kernel_fsid_t fsid;
    fsnotify_connp_t *obj;
    struct fsnotify_mark_connector *destroy_next;
    struct hlist_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct fsnotify_mark_connector {
    spinlock_t lock;
    short unsigned int type;
    short unsigned int flags;
    __kernel_fsid_t fsid;
    fsnotify_connp_t *obj;
    struct fsnotify_mark_connector *destroy_next;
    struct hlist_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct fsnotify_mark_connector {
    spinlock_t lock;
    short unsigned int type;
    short unsigned int flags;
    fsnotify_connp_t *obj;
    struct fsnotify_mark_connector *destroy_next;
    struct hlist_head list;
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
struct fsnotify_mark_connector {
    spinlock_t lock;
    short unsigned int type;
    short unsigned int flags;
    __kernel_fsid_t fsid;
    fsnotify_connp_t *obj;
    struct fsnotify_mark_connector *destroy_next;
    struct hlist_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct fsnotify_mark_connector {
    spinlock_t lock;
    short unsigned int type;
    short unsigned int flags;
    __kernel_fsid_t fsid;
    fsnotify_connp_t *obj;
    struct fsnotify_mark_connector *destroy_next;
    struct hlist_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct fsnotify_mark_connector {
    spinlock_t lock;
    short unsigned int type;
    short unsigned int flags;
    __kernel_fsid_t fsid;
    fsnotify_connp_t *obj;
    struct fsnotify_mark_connector *destroy_next;
    struct hlist_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct fsnotify_mark_connector {
    spinlock_t lock;
    short unsigned int type;
    short unsigned int flags;
    __kernel_fsid_t fsid;
    fsnotify_connp_t *obj;
    struct fsnotify_mark_connector *destroy_next;
    struct hlist_head list;
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
struct fsnotify_mark_connector {
    spinlock_t lock;
    short unsigned int type;
    short unsigned int flags;
    __kernel_fsid_t fsid;
    fsnotify_connp_t *obj;
    struct fsnotify_mark_connector *destroy_next;
    struct hlist_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct fsnotify_mark_connector {
    spinlock_t lock;
    short unsigned int type;
    short unsigned int flags;
    __kernel_fsid_t fsid;
    fsnotify_connp_t *obj;
    struct fsnotify_mark_connector *destroy_next;
    struct hlist_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct fsnotify_mark_connector {
    spinlock_t lock;
    short unsigned int type;
    short unsigned int flags;
    __kernel_fsid_t fsid;
    fsnotify_connp_t *obj;
    struct fsnotify_mark_connector *destroy_next;
    struct hlist_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct fsnotify_mark_connector {
    spinlock_t lock;
    short unsigned int type;
    short unsigned int flags;
    __kernel_fsid_t fsid;
    fsnotify_connp_t *obj;
    struct fsnotify_mark_connector *destroy_next;
    struct hlist_head list;
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
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int type</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int flags</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>fsnotify_connp_t *obj</code>
</li>
<li>
<b>Field removed. </b>
<code>struct inode *inode</code>
</li>
<li>
<b>Field removed. </b>
<code>struct vfsmount *mnt</code>
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
<code>short unsigned int flags</code>
</li>
<li>
<b>Field added. </b>
<code>__kernel_fsid_t fsid</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int type</code> ➡️ <code>short unsigned int type</code>
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
<b>Field removed. </b>
<code>__kernel_fsid_t fsid</code>
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
