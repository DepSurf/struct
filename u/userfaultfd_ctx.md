# Struct: <code>userfaultfd_ctx</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct userfaultfd_ctx {
    wait_queue_head_t fault_pending_wqh;
    wait_queue_head_t fault_wqh;
    wait_queue_head_t fd_wqh;
    struct seqcount refile_seq;
    atomic_t refcount;
    unsigned int flags;
    enum userfaultfd_state state;
    bool released;
    struct mm_struct *mm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct userfaultfd_ctx {
    wait_queue_head_t fault_pending_wqh;
    wait_queue_head_t fault_wqh;
    wait_queue_head_t fd_wqh;
    struct seqcount refile_seq;
    atomic_t refcount;
    unsigned int flags;
    enum userfaultfd_state state;
    bool released;
    struct mm_struct *mm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct userfaultfd_ctx {
    wait_queue_head_t fault_pending_wqh;
    wait_queue_head_t fault_wqh;
    wait_queue_head_t fd_wqh;
    struct seqcount refile_seq;
    atomic_t refcount;
    unsigned int flags;
    enum userfaultfd_state state;
    bool released;
    struct mm_struct *mm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct userfaultfd_ctx {
    wait_queue_head_t fault_pending_wqh;
    wait_queue_head_t fault_wqh;
    wait_queue_head_t fd_wqh;
    wait_queue_head_t event_wqh;
    struct seqcount refile_seq;
    atomic_t refcount;
    unsigned int flags;
    unsigned int features;
    enum userfaultfd_state state;
    bool released;
    struct mm_struct *mm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct userfaultfd_ctx {
    wait_queue_head_t fault_pending_wqh;
    wait_queue_head_t fault_wqh;
    wait_queue_head_t fd_wqh;
    wait_queue_head_t event_wqh;
    struct seqcount refile_seq;
    atomic_t refcount;
    unsigned int flags;
    unsigned int features;
    enum userfaultfd_state state;
    bool released;
    struct mm_struct *mm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct userfaultfd_ctx {
    wait_queue_head_t fault_pending_wqh;
    wait_queue_head_t fault_wqh;
    wait_queue_head_t fd_wqh;
    wait_queue_head_t event_wqh;
    struct seqcount refile_seq;
    atomic_t refcount;
    unsigned int flags;
    unsigned int features;
    enum userfaultfd_state state;
    bool released;
    bool mmap_changing;
    struct mm_struct *mm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct userfaultfd_ctx {
    wait_queue_head_t fault_pending_wqh;
    wait_queue_head_t fault_wqh;
    wait_queue_head_t fd_wqh;
    wait_queue_head_t event_wqh;
    struct seqcount refile_seq;
    refcount_t refcount;
    unsigned int flags;
    unsigned int features;
    enum userfaultfd_state state;
    bool released;
    bool mmap_changing;
    struct mm_struct *mm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct userfaultfd_ctx {
    wait_queue_head_t fault_pending_wqh;
    wait_queue_head_t fault_wqh;
    wait_queue_head_t fd_wqh;
    wait_queue_head_t event_wqh;
    struct seqcount refile_seq;
    refcount_t refcount;
    unsigned int flags;
    unsigned int features;
    enum userfaultfd_state state;
    bool released;
    bool mmap_changing;
    struct mm_struct *mm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct userfaultfd_ctx {
    wait_queue_head_t fault_pending_wqh;
    wait_queue_head_t fault_wqh;
    wait_queue_head_t fd_wqh;
    wait_queue_head_t event_wqh;
    struct seqcount refile_seq;
    refcount_t refcount;
    unsigned int flags;
    unsigned int features;
    enum userfaultfd_state state;
    bool released;
    bool mmap_changing;
    struct mm_struct *mm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct userfaultfd_ctx {
    wait_queue_head_t fault_pending_wqh;
    wait_queue_head_t fault_wqh;
    wait_queue_head_t fd_wqh;
    wait_queue_head_t event_wqh;
    struct seqcount refile_seq;
    refcount_t refcount;
    unsigned int flags;
    unsigned int features;
    enum userfaultfd_state state;
    bool released;
    bool mmap_changing;
    struct mm_struct *mm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct userfaultfd_ctx {
    wait_queue_head_t fault_pending_wqh;
    wait_queue_head_t fault_wqh;
    wait_queue_head_t fd_wqh;
    wait_queue_head_t event_wqh;
    seqcount_spinlock_t refile_seq;
    refcount_t refcount;
    unsigned int flags;
    unsigned int features;
    enum userfaultfd_state state;
    bool released;
    bool mmap_changing;
    struct mm_struct *mm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct userfaultfd_ctx {
    wait_queue_head_t fault_pending_wqh;
    wait_queue_head_t fault_wqh;
    wait_queue_head_t fd_wqh;
    wait_queue_head_t event_wqh;
    seqcount_spinlock_t refile_seq;
    refcount_t refcount;
    unsigned int flags;
    unsigned int features;
    enum userfaultfd_state state;
    bool released;
    bool mmap_changing;
    struct mm_struct *mm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct userfaultfd_ctx {
    wait_queue_head_t fault_pending_wqh;
    wait_queue_head_t fault_wqh;
    wait_queue_head_t fd_wqh;
    wait_queue_head_t event_wqh;
    seqcount_spinlock_t refile_seq;
    refcount_t refcount;
    unsigned int flags;
    unsigned int features;
    bool released;
    atomic_t mmap_changing;
    struct mm_struct *mm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct userfaultfd_ctx {
    wait_queue_head_t fault_pending_wqh;
    wait_queue_head_t fault_wqh;
    wait_queue_head_t fd_wqh;
    wait_queue_head_t event_wqh;
    seqcount_spinlock_t refile_seq;
    refcount_t refcount;
    unsigned int flags;
    unsigned int features;
    bool released;
    atomic_t mmap_changing;
    struct mm_struct *mm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct userfaultfd_ctx {
    wait_queue_head_t fault_pending_wqh;
    wait_queue_head_t fault_wqh;
    wait_queue_head_t fd_wqh;
    wait_queue_head_t event_wqh;
    seqcount_spinlock_t refile_seq;
    refcount_t refcount;
    unsigned int flags;
    unsigned int features;
    bool released;
    atomic_t mmap_changing;
    struct mm_struct *mm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct userfaultfd_ctx {
    wait_queue_head_t fault_pending_wqh;
    wait_queue_head_t fault_wqh;
    wait_queue_head_t fd_wqh;
    wait_queue_head_t event_wqh;
    seqcount_spinlock_t refile_seq;
    refcount_t refcount;
    unsigned int flags;
    unsigned int features;
    bool released;
    atomic_t mmap_changing;
    struct mm_struct *mm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct userfaultfd_ctx {
    wait_queue_head_t fault_pending_wqh;
    wait_queue_head_t fault_wqh;
    wait_queue_head_t fd_wqh;
    wait_queue_head_t event_wqh;
    seqcount_spinlock_t refile_seq;
    refcount_t refcount;
    unsigned int flags;
    unsigned int features;
    bool released;
    atomic_t mmap_changing;
    struct mm_struct *mm;
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
struct userfaultfd_ctx {
    wait_queue_head_t fault_pending_wqh;
    wait_queue_head_t fault_wqh;
    wait_queue_head_t fd_wqh;
    wait_queue_head_t event_wqh;
    struct seqcount refile_seq;
    refcount_t refcount;
    unsigned int flags;
    unsigned int features;
    enum userfaultfd_state state;
    bool released;
    bool mmap_changing;
    struct mm_struct *mm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct userfaultfd_ctx {
    wait_queue_head_t fault_pending_wqh;
    wait_queue_head_t fault_wqh;
    wait_queue_head_t fd_wqh;
    wait_queue_head_t event_wqh;
    struct seqcount refile_seq;
    refcount_t refcount;
    unsigned int flags;
    unsigned int features;
    enum userfaultfd_state state;
    bool released;
    bool mmap_changing;
    struct mm_struct *mm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct userfaultfd_ctx {
    wait_queue_head_t fault_pending_wqh;
    wait_queue_head_t fault_wqh;
    wait_queue_head_t fd_wqh;
    wait_queue_head_t event_wqh;
    struct seqcount refile_seq;
    refcount_t refcount;
    unsigned int flags;
    unsigned int features;
    enum userfaultfd_state state;
    bool released;
    bool mmap_changing;
    struct mm_struct *mm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct userfaultfd_ctx {
    wait_queue_head_t fault_pending_wqh;
    wait_queue_head_t fault_wqh;
    wait_queue_head_t fd_wqh;
    wait_queue_head_t event_wqh;
    struct seqcount refile_seq;
    refcount_t refcount;
    unsigned int flags;
    unsigned int features;
    enum userfaultfd_state state;
    bool released;
    bool mmap_changing;
    struct mm_struct *mm;
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
struct userfaultfd_ctx {
    wait_queue_head_t fault_pending_wqh;
    wait_queue_head_t fault_wqh;
    wait_queue_head_t fd_wqh;
    wait_queue_head_t event_wqh;
    struct seqcount refile_seq;
    refcount_t refcount;
    unsigned int flags;
    unsigned int features;
    enum userfaultfd_state state;
    bool released;
    bool mmap_changing;
    struct mm_struct *mm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct userfaultfd_ctx {
    wait_queue_head_t fault_pending_wqh;
    wait_queue_head_t fault_wqh;
    wait_queue_head_t fd_wqh;
    wait_queue_head_t event_wqh;
    struct seqcount refile_seq;
    refcount_t refcount;
    unsigned int flags;
    unsigned int features;
    enum userfaultfd_state state;
    bool released;
    bool mmap_changing;
    struct mm_struct *mm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct userfaultfd_ctx {
    wait_queue_head_t fault_pending_wqh;
    wait_queue_head_t fault_wqh;
    wait_queue_head_t fd_wqh;
    wait_queue_head_t event_wqh;
    struct seqcount refile_seq;
    refcount_t refcount;
    unsigned int flags;
    unsigned int features;
    enum userfaultfd_state state;
    bool released;
    bool mmap_changing;
    struct mm_struct *mm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct userfaultfd_ctx {
    wait_queue_head_t fault_pending_wqh;
    wait_queue_head_t fault_wqh;
    wait_queue_head_t fd_wqh;
    wait_queue_head_t event_wqh;
    struct seqcount refile_seq;
    refcount_t refcount;
    unsigned int flags;
    unsigned int features;
    enum userfaultfd_state state;
    bool released;
    bool mmap_changing;
    struct mm_struct *mm;
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
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>wait_queue_head_t event_wqh</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int features</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool mmap_changing</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>atomic_t refcount</code> ➡️ <code>refcount_t refcount</code>
</li>
</ul>
</details>
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
<code>struct seqcount refile_seq</code> ➡️ <code>seqcount_spinlock_t refile_seq</code>
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
<code>enum userfaultfd_state state</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool mmap_changing</code> ➡️ <code>atomic_t mmap_changing</code>
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
