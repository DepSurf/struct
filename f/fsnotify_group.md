# Struct: <code>fsnotify_group</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct fsnotify_group {
    atomic_t refcnt;
    const struct fsnotify_ops *ops;
    struct mutex notification_mutex;
    struct list_head notification_list;
    wait_queue_head_t notification_waitq;
    unsigned int q_len;
    unsigned int max_events;
    unsigned int priority;
    struct mutex mark_mutex;
    atomic_t num_marks;
    struct list_head marks_list;
    struct fasync_struct *fsn_fa;
    struct fsnotify_event *overflow_event;
    void *private;
    struct inotify_group_private_data inotify_data;
    struct fanotify_group_private_data fanotify_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct fsnotify_group {
    atomic_t refcnt;
    const struct fsnotify_ops *ops;
    struct mutex notification_mutex;
    struct list_head notification_list;
    wait_queue_head_t notification_waitq;
    unsigned int q_len;
    unsigned int max_events;
    unsigned int priority;
    bool shutdown;
    struct mutex mark_mutex;
    atomic_t num_marks;
    struct list_head marks_list;
    struct fasync_struct *fsn_fa;
    struct fsnotify_event *overflow_event;
    void *private;
    struct inotify_group_private_data inotify_data;
    struct fanotify_group_private_data fanotify_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct fsnotify_group {
    atomic_t refcnt;
    const struct fsnotify_ops *ops;
    spinlock_t notification_lock;
    struct list_head notification_list;
    wait_queue_head_t notification_waitq;
    unsigned int q_len;
    unsigned int max_events;
    unsigned int priority;
    bool shutdown;
    struct mutex mark_mutex;
    atomic_t num_marks;
    struct list_head marks_list;
    struct fasync_struct *fsn_fa;
    struct fsnotify_event *overflow_event;
    void *private;
    struct inotify_group_private_data inotify_data;
    struct fanotify_group_private_data fanotify_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct fsnotify_group {
    atomic_t refcnt;
    const struct fsnotify_ops *ops;
    spinlock_t notification_lock;
    struct list_head notification_list;
    wait_queue_head_t notification_waitq;
    unsigned int q_len;
    unsigned int max_events;
    unsigned int priority;
    bool shutdown;
    struct mutex mark_mutex;
    atomic_t num_marks;
    struct list_head marks_list;
    struct fasync_struct *fsn_fa;
    struct fsnotify_event *overflow_event;
    atomic_t user_waits;
    void *private;
    struct inotify_group_private_data inotify_data;
    struct fanotify_group_private_data fanotify_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct fsnotify_group {
    refcount_t refcnt;
    const struct fsnotify_ops *ops;
    spinlock_t notification_lock;
    struct list_head notification_list;
    wait_queue_head_t notification_waitq;
    unsigned int q_len;
    unsigned int max_events;
    unsigned int priority;
    bool shutdown;
    struct mutex mark_mutex;
    atomic_t num_marks;
    struct list_head marks_list;
    struct fasync_struct *fsn_fa;
    struct fsnotify_event *overflow_event;
    atomic_t user_waits;
    void *private;
    struct inotify_group_private_data inotify_data;
    struct fanotify_group_private_data fanotify_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct fsnotify_group {
    refcount_t refcnt;
    const struct fsnotify_ops *ops;
    spinlock_t notification_lock;
    struct list_head notification_list;
    wait_queue_head_t notification_waitq;
    unsigned int q_len;
    unsigned int max_events;
    unsigned int priority;
    bool shutdown;
    struct mutex mark_mutex;
    atomic_t num_marks;
    struct list_head marks_list;
    struct fasync_struct *fsn_fa;
    struct fsnotify_event *overflow_event;
    atomic_t user_waits;
    void *private;
    struct inotify_group_private_data inotify_data;
    struct fanotify_group_private_data fanotify_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct fsnotify_group {
    const struct fsnotify_ops *ops;
    refcount_t refcnt;
    spinlock_t notification_lock;
    struct list_head notification_list;
    wait_queue_head_t notification_waitq;
    unsigned int q_len;
    unsigned int max_events;
    unsigned int priority;
    bool shutdown;
    struct mutex mark_mutex;
    atomic_t num_marks;
    atomic_t user_waits;
    struct list_head marks_list;
    struct fasync_struct *fsn_fa;
    struct fsnotify_event *overflow_event;
    struct mem_cgroup *memcg;
    void *private;
    struct inotify_group_private_data inotify_data;
    struct fanotify_group_private_data fanotify_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct fsnotify_group {
    const struct fsnotify_ops *ops;
    refcount_t refcnt;
    spinlock_t notification_lock;
    struct list_head notification_list;
    wait_queue_head_t notification_waitq;
    unsigned int q_len;
    unsigned int max_events;
    unsigned int priority;
    bool shutdown;
    struct mutex mark_mutex;
    atomic_t num_marks;
    atomic_t user_waits;
    struct list_head marks_list;
    struct fasync_struct *fsn_fa;
    struct fsnotify_event *overflow_event;
    struct mem_cgroup *memcg;
    void *private;
    struct inotify_group_private_data inotify_data;
    struct fanotify_group_private_data fanotify_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct fsnotify_group {
    const struct fsnotify_ops *ops;
    refcount_t refcnt;
    spinlock_t notification_lock;
    struct list_head notification_list;
    wait_queue_head_t notification_waitq;
    unsigned int q_len;
    unsigned int max_events;
    unsigned int priority;
    bool shutdown;
    struct mutex mark_mutex;
    atomic_t num_marks;
    atomic_t user_waits;
    struct list_head marks_list;
    struct fasync_struct *fsn_fa;
    struct fsnotify_event *overflow_event;
    struct mem_cgroup *memcg;
    void *private;
    struct inotify_group_private_data inotify_data;
    struct fanotify_group_private_data fanotify_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct fsnotify_group {
    const struct fsnotify_ops *ops;
    refcount_t refcnt;
    spinlock_t notification_lock;
    struct list_head notification_list;
    wait_queue_head_t notification_waitq;
    unsigned int q_len;
    unsigned int max_events;
    unsigned int priority;
    bool shutdown;
    struct mutex mark_mutex;
    atomic_t num_marks;
    atomic_t user_waits;
    struct list_head marks_list;
    struct fasync_struct *fsn_fa;
    struct fsnotify_event *overflow_event;
    struct mem_cgroup *memcg;
    void *private;
    struct inotify_group_private_data inotify_data;
    struct fanotify_group_private_data fanotify_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct fsnotify_group {
    const struct fsnotify_ops *ops;
    refcount_t refcnt;
    spinlock_t notification_lock;
    struct list_head notification_list;
    wait_queue_head_t notification_waitq;
    unsigned int q_len;
    unsigned int max_events;
    unsigned int priority;
    bool shutdown;
    struct mutex mark_mutex;
    atomic_t num_marks;
    atomic_t user_waits;
    struct list_head marks_list;
    struct fasync_struct *fsn_fa;
    struct fsnotify_event *overflow_event;
    struct mem_cgroup *memcg;
    void *private;
    struct inotify_group_private_data inotify_data;
    struct fanotify_group_private_data fanotify_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct fsnotify_group {
    const struct fsnotify_ops *ops;
    refcount_t refcnt;
    spinlock_t notification_lock;
    struct list_head notification_list;
    wait_queue_head_t notification_waitq;
    unsigned int q_len;
    unsigned int max_events;
    unsigned int priority;
    bool shutdown;
    struct mutex mark_mutex;
    atomic_t user_waits;
    struct list_head marks_list;
    struct fasync_struct *fsn_fa;
    struct fsnotify_event *overflow_event;
    struct mem_cgroup *memcg;
    void *private;
    struct inotify_group_private_data inotify_data;
    struct fanotify_group_private_data fanotify_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct fsnotify_group {
    const struct fsnotify_ops *ops;
    refcount_t refcnt;
    spinlock_t notification_lock;
    struct list_head notification_list;
    wait_queue_head_t notification_waitq;
    unsigned int q_len;
    unsigned int max_events;
    unsigned int priority;
    bool shutdown;
    struct mutex mark_mutex;
    atomic_t user_waits;
    struct list_head marks_list;
    struct fasync_struct *fsn_fa;
    struct fsnotify_event *overflow_event;
    struct mem_cgroup *memcg;
    void *private;
    struct inotify_group_private_data inotify_data;
    struct fanotify_group_private_data fanotify_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct fsnotify_group {
    const struct fsnotify_ops *ops;
    refcount_t refcnt;
    spinlock_t notification_lock;
    struct list_head notification_list;
    wait_queue_head_t notification_waitq;
    unsigned int q_len;
    unsigned int max_events;
    unsigned int priority;
    bool shutdown;
    int flags;
    unsigned int owner_flags;
    struct mutex mark_mutex;
    atomic_t user_waits;
    struct list_head marks_list;
    struct fasync_struct *fsn_fa;
    struct fsnotify_event *overflow_event;
    struct mem_cgroup *memcg;
    void *private;
    struct inotify_group_private_data inotify_data;
    struct fanotify_group_private_data fanotify_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct fsnotify_group {
    const struct fsnotify_ops *ops;
    refcount_t refcnt;
    spinlock_t notification_lock;
    struct list_head notification_list;
    wait_queue_head_t notification_waitq;
    unsigned int q_len;
    unsigned int max_events;
    unsigned int priority;
    bool shutdown;
    int flags;
    unsigned int owner_flags;
    struct mutex mark_mutex;
    atomic_t user_waits;
    struct list_head marks_list;
    struct fasync_struct *fsn_fa;
    struct fsnotify_event *overflow_event;
    struct mem_cgroup *memcg;
    void *private;
    struct inotify_group_private_data inotify_data;
    struct fanotify_group_private_data fanotify_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct fsnotify_group {
    const struct fsnotify_ops *ops;
    refcount_t refcnt;
    spinlock_t notification_lock;
    struct list_head notification_list;
    wait_queue_head_t notification_waitq;
    unsigned int q_len;
    unsigned int max_events;
    unsigned int priority;
    bool shutdown;
    int flags;
    unsigned int owner_flags;
    struct mutex mark_mutex;
    atomic_t user_waits;
    struct list_head marks_list;
    struct fasync_struct *fsn_fa;
    struct fsnotify_event *overflow_event;
    struct mem_cgroup *memcg;
    void *private;
    struct inotify_group_private_data inotify_data;
    struct fanotify_group_private_data fanotify_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct fsnotify_group {
    const struct fsnotify_ops *ops;
    refcount_t refcnt;
    spinlock_t notification_lock;
    struct list_head notification_list;
    wait_queue_head_t notification_waitq;
    unsigned int q_len;
    unsigned int max_events;
    unsigned int priority;
    bool shutdown;
    int flags;
    unsigned int owner_flags;
    struct mutex mark_mutex;
    atomic_t user_waits;
    struct list_head marks_list;
    struct fasync_struct *fsn_fa;
    struct fsnotify_event *overflow_event;
    struct mem_cgroup *memcg;
    void *private;
    struct inotify_group_private_data inotify_data;
    struct fanotify_group_private_data fanotify_data;
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
struct fsnotify_group {
    const struct fsnotify_ops *ops;
    refcount_t refcnt;
    spinlock_t notification_lock;
    struct list_head notification_list;
    wait_queue_head_t notification_waitq;
    unsigned int q_len;
    unsigned int max_events;
    unsigned int priority;
    bool shutdown;
    struct mutex mark_mutex;
    atomic_t num_marks;
    atomic_t user_waits;
    struct list_head marks_list;
    struct fasync_struct *fsn_fa;
    struct fsnotify_event *overflow_event;
    struct mem_cgroup *memcg;
    void *private;
    struct inotify_group_private_data inotify_data;
    struct fanotify_group_private_data fanotify_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct fsnotify_group {
    const struct fsnotify_ops *ops;
    refcount_t refcnt;
    spinlock_t notification_lock;
    struct list_head notification_list;
    wait_queue_head_t notification_waitq;
    unsigned int q_len;
    unsigned int max_events;
    unsigned int priority;
    bool shutdown;
    struct mutex mark_mutex;
    atomic_t num_marks;
    atomic_t user_waits;
    struct list_head marks_list;
    struct fasync_struct *fsn_fa;
    struct fsnotify_event *overflow_event;
    struct mem_cgroup *memcg;
    void *private;
    struct inotify_group_private_data inotify_data;
    struct fanotify_group_private_data fanotify_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct fsnotify_group {
    const struct fsnotify_ops *ops;
    refcount_t refcnt;
    spinlock_t notification_lock;
    struct list_head notification_list;
    wait_queue_head_t notification_waitq;
    unsigned int q_len;
    unsigned int max_events;
    unsigned int priority;
    bool shutdown;
    struct mutex mark_mutex;
    atomic_t num_marks;
    atomic_t user_waits;
    struct list_head marks_list;
    struct fasync_struct *fsn_fa;
    struct fsnotify_event *overflow_event;
    struct mem_cgroup *memcg;
    void *private;
    struct inotify_group_private_data inotify_data;
    struct fanotify_group_private_data fanotify_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct fsnotify_group {
    const struct fsnotify_ops *ops;
    refcount_t refcnt;
    spinlock_t notification_lock;
    struct list_head notification_list;
    wait_queue_head_t notification_waitq;
    unsigned int q_len;
    unsigned int max_events;
    unsigned int priority;
    bool shutdown;
    struct mutex mark_mutex;
    atomic_t num_marks;
    atomic_t user_waits;
    struct list_head marks_list;
    struct fasync_struct *fsn_fa;
    struct fsnotify_event *overflow_event;
    struct mem_cgroup *memcg;
    void *private;
    struct inotify_group_private_data inotify_data;
    struct fanotify_group_private_data fanotify_data;
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
struct fsnotify_group {
    const struct fsnotify_ops *ops;
    refcount_t refcnt;
    spinlock_t notification_lock;
    struct list_head notification_list;
    wait_queue_head_t notification_waitq;
    unsigned int q_len;
    unsigned int max_events;
    unsigned int priority;
    bool shutdown;
    struct mutex mark_mutex;
    atomic_t num_marks;
    atomic_t user_waits;
    struct list_head marks_list;
    struct fasync_struct *fsn_fa;
    struct fsnotify_event *overflow_event;
    struct mem_cgroup *memcg;
    void *private;
    struct inotify_group_private_data inotify_data;
    struct fanotify_group_private_data fanotify_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct fsnotify_group {
    const struct fsnotify_ops *ops;
    refcount_t refcnt;
    spinlock_t notification_lock;
    struct list_head notification_list;
    wait_queue_head_t notification_waitq;
    unsigned int q_len;
    unsigned int max_events;
    unsigned int priority;
    bool shutdown;
    struct mutex mark_mutex;
    atomic_t num_marks;
    atomic_t user_waits;
    struct list_head marks_list;
    struct fasync_struct *fsn_fa;
    struct fsnotify_event *overflow_event;
    struct mem_cgroup *memcg;
    void *private;
    struct inotify_group_private_data inotify_data;
    struct fanotify_group_private_data fanotify_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct fsnotify_group {
    const struct fsnotify_ops *ops;
    refcount_t refcnt;
    spinlock_t notification_lock;
    struct list_head notification_list;
    wait_queue_head_t notification_waitq;
    unsigned int q_len;
    unsigned int max_events;
    unsigned int priority;
    bool shutdown;
    struct mutex mark_mutex;
    atomic_t num_marks;
    atomic_t user_waits;
    struct list_head marks_list;
    struct fasync_struct *fsn_fa;
    struct fsnotify_event *overflow_event;
    struct mem_cgroup *memcg;
    void *private;
    struct inotify_group_private_data inotify_data;
    struct fanotify_group_private_data fanotify_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct fsnotify_group {
    const struct fsnotify_ops *ops;
    refcount_t refcnt;
    spinlock_t notification_lock;
    struct list_head notification_list;
    wait_queue_head_t notification_waitq;
    unsigned int q_len;
    unsigned int max_events;
    unsigned int priority;
    bool shutdown;
    struct mutex mark_mutex;
    atomic_t num_marks;
    atomic_t user_waits;
    struct list_head marks_list;
    struct fasync_struct *fsn_fa;
    struct fsnotify_event *overflow_event;
    struct mem_cgroup *memcg;
    void *private;
    struct inotify_group_private_data inotify_data;
    struct fanotify_group_private_data fanotify_data;
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
<code>bool shutdown</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>spinlock_t notification_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mutex notification_mutex</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>atomic_t user_waits</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>atomic_t refcnt</code> ➡️ <code>refcount_t refcnt</code>
</li>
</ul>
</details>
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
<code>struct mem_cgroup *memcg</code>
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
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>atomic_t num_marks</code>
</li>
</ul>
</details>
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
<code>int flags</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int owner_flags</code>
</li>
</ul>
</details>
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
