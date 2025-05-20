# Struct: <code>kernfs_root</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct kernfs_root {
    struct kernfs_node *kn;
    unsigned int flags;
    struct ida ino_ida;
    struct kernfs_syscall_ops *syscall_ops;
    struct list_head supers;
    wait_queue_head_t deactivate_waitq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct kernfs_root {
    struct kernfs_node *kn;
    unsigned int flags;
    struct ida ino_ida;
    struct kernfs_syscall_ops *syscall_ops;
    struct list_head supers;
    wait_queue_head_t deactivate_waitq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct kernfs_root {
    struct kernfs_node *kn;
    unsigned int flags;
    struct ida ino_ida;
    struct kernfs_syscall_ops *syscall_ops;
    struct list_head supers;
    wait_queue_head_t deactivate_waitq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct kernfs_root {
    struct kernfs_node *kn;
    unsigned int flags;
    struct ida ino_ida;
    struct kernfs_syscall_ops *syscall_ops;
    struct list_head supers;
    wait_queue_head_t deactivate_waitq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct kernfs_root {
    struct kernfs_node *kn;
    unsigned int flags;
    struct idr ino_idr;
    u32 next_generation;
    struct kernfs_syscall_ops *syscall_ops;
    struct list_head supers;
    wait_queue_head_t deactivate_waitq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct kernfs_root {
    struct kernfs_node *kn;
    unsigned int flags;
    struct idr ino_idr;
    u32 next_generation;
    struct kernfs_syscall_ops *syscall_ops;
    struct list_head supers;
    wait_queue_head_t deactivate_waitq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct kernfs_root {
    struct kernfs_node *kn;
    unsigned int flags;
    struct idr ino_idr;
    u32 next_generation;
    struct kernfs_syscall_ops *syscall_ops;
    struct list_head supers;
    wait_queue_head_t deactivate_waitq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct kernfs_root {
    struct kernfs_node *kn;
    unsigned int flags;
    struct idr ino_idr;
    u32 next_generation;
    struct kernfs_syscall_ops *syscall_ops;
    struct list_head supers;
    wait_queue_head_t deactivate_waitq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct kernfs_root {
    struct kernfs_node *kn;
    unsigned int flags;
    struct idr ino_idr;
    u32 last_ino;
    u32 next_generation;
    struct kernfs_syscall_ops *syscall_ops;
    struct list_head supers;
    wait_queue_head_t deactivate_waitq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct kernfs_root {
    struct kernfs_node *kn;
    unsigned int flags;
    struct idr ino_idr;
    u32 last_id_lowbits;
    u32 id_highbits;
    struct kernfs_syscall_ops *syscall_ops;
    struct list_head supers;
    wait_queue_head_t deactivate_waitq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct kernfs_root {
    struct kernfs_node *kn;
    unsigned int flags;
    struct idr ino_idr;
    u32 last_id_lowbits;
    u32 id_highbits;
    struct kernfs_syscall_ops *syscall_ops;
    struct list_head supers;
    wait_queue_head_t deactivate_waitq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kernfs_root {
    struct kernfs_node *kn;
    unsigned int flags;
    struct idr ino_idr;
    u32 last_id_lowbits;
    u32 id_highbits;
    struct kernfs_syscall_ops *syscall_ops;
    struct list_head supers;
    wait_queue_head_t deactivate_waitq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kernfs_root {
    struct kernfs_node *kn;
    unsigned int flags;
    struct idr ino_idr;
    u32 last_id_lowbits;
    u32 id_highbits;
    struct kernfs_syscall_ops *syscall_ops;
    struct list_head supers;
    wait_queue_head_t deactivate_waitq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kernfs_root {
    struct kernfs_node *kn;
    unsigned int flags;
    struct idr ino_idr;
    u32 last_id_lowbits;
    u32 id_highbits;
    struct kernfs_syscall_ops *syscall_ops;
    struct list_head supers;
    wait_queue_head_t deactivate_waitq;
    struct rw_semaphore kernfs_rwsem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kernfs_root {
    struct kernfs_node *kn;
    unsigned int flags;
    struct idr ino_idr;
    u32 last_id_lowbits;
    u32 id_highbits;
    struct kernfs_syscall_ops *syscall_ops;
    struct list_head supers;
    wait_queue_head_t deactivate_waitq;
    struct rw_semaphore kernfs_rwsem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kernfs_root {
    struct kernfs_node *kn;
    unsigned int flags;
    struct idr ino_idr;
    u32 last_id_lowbits;
    u32 id_highbits;
    struct kernfs_syscall_ops *syscall_ops;
    struct list_head supers;
    wait_queue_head_t deactivate_waitq;
    struct rw_semaphore kernfs_rwsem;
    struct rw_semaphore kernfs_iattr_rwsem;
    struct rw_semaphore kernfs_supers_rwsem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kernfs_root {
    struct kernfs_node *kn;
    unsigned int flags;
    struct idr ino_idr;
    u32 last_id_lowbits;
    u32 id_highbits;
    struct kernfs_syscall_ops *syscall_ops;
    struct list_head supers;
    wait_queue_head_t deactivate_waitq;
    struct rw_semaphore kernfs_rwsem;
    struct rw_semaphore kernfs_iattr_rwsem;
    struct rw_semaphore kernfs_supers_rwsem;
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
struct kernfs_root {
    struct kernfs_node *kn;
    unsigned int flags;
    struct idr ino_idr;
    u32 last_ino;
    u32 next_generation;
    struct kernfs_syscall_ops *syscall_ops;
    struct list_head supers;
    wait_queue_head_t deactivate_waitq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct kernfs_root {
    struct kernfs_node *kn;
    unsigned int flags;
    struct idr ino_idr;
    u32 last_ino;
    u32 next_generation;
    struct kernfs_syscall_ops *syscall_ops;
    struct list_head supers;
    wait_queue_head_t deactivate_waitq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct kernfs_root {
    struct kernfs_node *kn;
    unsigned int flags;
    struct idr ino_idr;
    u32 last_ino;
    u32 next_generation;
    struct kernfs_syscall_ops *syscall_ops;
    struct list_head supers;
    wait_queue_head_t deactivate_waitq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct kernfs_root {
    struct kernfs_node *kn;
    unsigned int flags;
    struct idr ino_idr;
    u32 last_ino;
    u32 next_generation;
    struct kernfs_syscall_ops *syscall_ops;
    struct list_head supers;
    wait_queue_head_t deactivate_waitq;
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
struct kernfs_root {
    struct kernfs_node *kn;
    unsigned int flags;
    struct idr ino_idr;
    u32 last_ino;
    u32 next_generation;
    struct kernfs_syscall_ops *syscall_ops;
    struct list_head supers;
    wait_queue_head_t deactivate_waitq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct kernfs_root {
    struct kernfs_node *kn;
    unsigned int flags;
    struct idr ino_idr;
    u32 last_ino;
    u32 next_generation;
    struct kernfs_syscall_ops *syscall_ops;
    struct list_head supers;
    wait_queue_head_t deactivate_waitq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct kernfs_root {
    struct kernfs_node *kn;
    unsigned int flags;
    struct idr ino_idr;
    u32 last_ino;
    u32 next_generation;
    struct kernfs_syscall_ops *syscall_ops;
    struct list_head supers;
    wait_queue_head_t deactivate_waitq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct kernfs_root {
    struct kernfs_node *kn;
    unsigned int flags;
    struct idr ino_idr;
    u32 last_ino;
    u32 next_generation;
    struct kernfs_syscall_ops *syscall_ops;
    struct list_head supers;
    wait_queue_head_t deactivate_waitq;
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
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct idr ino_idr</code>
</li>
<li>
<b>Field added. </b>
<code>u32 next_generation</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ida ino_ida</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 last_ino</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 last_id_lowbits</code>
</li>
<li>
<b>Field added. </b>
<code>u32 id_highbits</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 last_ino</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 next_generation</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct rw_semaphore kernfs_rwsem</code>
</li>
</ul>
</details>
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
<code>struct rw_semaphore kernfs_iattr_rwsem</code>
</li>
<li>
<b>Field added. </b>
<code>struct rw_semaphore kernfs_supers_rwsem</code>
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
