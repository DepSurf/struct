# Struct: <code>eventpoll</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct eventpoll {
    spinlock_t lock;
    struct mutex mtx;
    wait_queue_head_t wq;
    wait_queue_head_t poll_wait;
    struct list_head rdllist;
    struct rb_root rbr;
    struct epitem *ovflist;
    struct wakeup_source *ws;
    struct user_struct *user;
    struct file *file;
    int visited;
    struct list_head visited_list_link;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct eventpoll {
    spinlock_t lock;
    struct mutex mtx;
    wait_queue_head_t wq;
    wait_queue_head_t poll_wait;
    struct list_head rdllist;
    struct rb_root rbr;
    struct epitem *ovflist;
    struct wakeup_source *ws;
    struct user_struct *user;
    struct file *file;
    int visited;
    struct list_head visited_list_link;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct eventpoll {
    spinlock_t lock;
    struct mutex mtx;
    wait_queue_head_t wq;
    wait_queue_head_t poll_wait;
    struct list_head rdllist;
    struct rb_root rbr;
    struct epitem *ovflist;
    struct wakeup_source *ws;
    struct user_struct *user;
    struct file *file;
    int visited;
    struct list_head visited_list_link;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct eventpoll {
    spinlock_t lock;
    struct mutex mtx;
    wait_queue_head_t wq;
    wait_queue_head_t poll_wait;
    struct list_head rdllist;
    struct rb_root rbr;
    struct epitem *ovflist;
    struct wakeup_source *ws;
    struct user_struct *user;
    struct file *file;
    int visited;
    struct list_head visited_list_link;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct eventpoll {
    spinlock_t lock;
    struct mutex mtx;
    wait_queue_head_t wq;
    wait_queue_head_t poll_wait;
    struct list_head rdllist;
    struct rb_root_cached rbr;
    struct epitem *ovflist;
    struct wakeup_source *ws;
    struct user_struct *user;
    struct file *file;
    int visited;
    struct list_head visited_list_link;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct eventpoll {
    spinlock_t lock;
    struct mutex mtx;
    wait_queue_head_t wq;
    wait_queue_head_t poll_wait;
    struct list_head rdllist;
    struct rb_root_cached rbr;
    struct epitem *ovflist;
    struct wakeup_source *ws;
    struct user_struct *user;
    struct file *file;
    int visited;
    struct list_head visited_list_link;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct eventpoll {
    struct mutex mtx;
    wait_queue_head_t wq;
    wait_queue_head_t poll_wait;
    struct list_head rdllist;
    struct rb_root_cached rbr;
    struct epitem *ovflist;
    struct wakeup_source *ws;
    struct user_struct *user;
    struct file *file;
    int visited;
    struct list_head visited_list_link;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct eventpoll {
    struct mutex mtx;
    wait_queue_head_t wq;
    wait_queue_head_t poll_wait;
    struct list_head rdllist;
    rwlock_t lock;
    struct rb_root_cached rbr;
    struct epitem *ovflist;
    struct wakeup_source *ws;
    struct user_struct *user;
    struct file *file;
    int visited;
    struct list_head visited_list_link;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct eventpoll {
    struct mutex mtx;
    wait_queue_head_t wq;
    wait_queue_head_t poll_wait;
    struct list_head rdllist;
    rwlock_t lock;
    struct rb_root_cached rbr;
    struct epitem *ovflist;
    struct wakeup_source *ws;
    struct user_struct *user;
    struct file *file;
    int visited;
    struct list_head visited_list_link;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct eventpoll {
    struct mutex mtx;
    wait_queue_head_t wq;
    wait_queue_head_t poll_wait;
    struct list_head rdllist;
    rwlock_t lock;
    struct rb_root_cached rbr;
    struct epitem *ovflist;
    struct wakeup_source *ws;
    struct user_struct *user;
    struct file *file;
    u64 gen;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct eventpoll {
    struct mutex mtx;
    wait_queue_head_t wq;
    wait_queue_head_t poll_wait;
    struct list_head rdllist;
    rwlock_t lock;
    struct rb_root_cached rbr;
    struct epitem *ovflist;
    struct wakeup_source *ws;
    struct user_struct *user;
    struct file *file;
    u64 gen;
    struct hlist_head refs;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct eventpoll {
    struct mutex mtx;
    wait_queue_head_t wq;
    wait_queue_head_t poll_wait;
    struct list_head rdllist;
    rwlock_t lock;
    struct rb_root_cached rbr;
    struct epitem *ovflist;
    struct wakeup_source *ws;
    struct user_struct *user;
    struct file *file;
    u64 gen;
    struct hlist_head refs;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct eventpoll {
    struct mutex mtx;
    wait_queue_head_t wq;
    wait_queue_head_t poll_wait;
    struct list_head rdllist;
    rwlock_t lock;
    struct rb_root_cached rbr;
    struct epitem *ovflist;
    struct wakeup_source *ws;
    struct user_struct *user;
    struct file *file;
    u64 gen;
    struct hlist_head refs;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct eventpoll {
    struct mutex mtx;
    wait_queue_head_t wq;
    wait_queue_head_t poll_wait;
    struct list_head rdllist;
    rwlock_t lock;
    struct rb_root_cached rbr;
    struct epitem *ovflist;
    struct wakeup_source *ws;
    struct user_struct *user;
    struct file *file;
    u64 gen;
    struct hlist_head refs;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct eventpoll {
    struct mutex mtx;
    wait_queue_head_t wq;
    wait_queue_head_t poll_wait;
    struct list_head rdllist;
    rwlock_t lock;
    struct rb_root_cached rbr;
    struct epitem *ovflist;
    struct wakeup_source *ws;
    struct user_struct *user;
    struct file *file;
    u64 gen;
    struct hlist_head refs;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct eventpoll {
    struct mutex mtx;
    wait_queue_head_t wq;
    wait_queue_head_t poll_wait;
    struct list_head rdllist;
    rwlock_t lock;
    struct rb_root_cached rbr;
    struct epitem *ovflist;
    struct wakeup_source *ws;
    struct user_struct *user;
    struct file *file;
    u64 gen;
    struct hlist_head refs;
    refcount_t refcount;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct eventpoll {
    struct mutex mtx;
    wait_queue_head_t wq;
    wait_queue_head_t poll_wait;
    struct list_head rdllist;
    rwlock_t lock;
    struct rb_root_cached rbr;
    struct epitem *ovflist;
    struct wakeup_source *ws;
    struct user_struct *user;
    struct file *file;
    u64 gen;
    struct hlist_head refs;
    refcount_t refcount;
    unsigned int napi_id;
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
struct eventpoll {
    struct mutex mtx;
    wait_queue_head_t wq;
    wait_queue_head_t poll_wait;
    struct list_head rdllist;
    rwlock_t lock;
    struct rb_root_cached rbr;
    struct epitem *ovflist;
    struct wakeup_source *ws;
    struct user_struct *user;
    struct file *file;
    int visited;
    struct list_head visited_list_link;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct eventpoll {
    struct mutex mtx;
    wait_queue_head_t wq;
    wait_queue_head_t poll_wait;
    struct list_head rdllist;
    rwlock_t lock;
    struct rb_root_cached rbr;
    struct epitem *ovflist;
    struct wakeup_source *ws;
    struct user_struct *user;
    struct file *file;
    int visited;
    struct list_head visited_list_link;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct eventpoll {
    struct mutex mtx;
    wait_queue_head_t wq;
    wait_queue_head_t poll_wait;
    struct list_head rdllist;
    rwlock_t lock;
    struct rb_root_cached rbr;
    struct epitem *ovflist;
    struct wakeup_source *ws;
    struct user_struct *user;
    struct file *file;
    int visited;
    struct list_head visited_list_link;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct eventpoll {
    struct mutex mtx;
    wait_queue_head_t wq;
    wait_queue_head_t poll_wait;
    struct list_head rdllist;
    rwlock_t lock;
    struct rb_root_cached rbr;
    struct epitem *ovflist;
    struct wakeup_source *ws;
    struct user_struct *user;
    struct file *file;
    int visited;
    struct list_head visited_list_link;
    unsigned int napi_id;
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
struct eventpoll {
    struct mutex mtx;
    wait_queue_head_t wq;
    wait_queue_head_t poll_wait;
    struct list_head rdllist;
    rwlock_t lock;
    struct rb_root_cached rbr;
    struct epitem *ovflist;
    struct wakeup_source *ws;
    struct user_struct *user;
    struct file *file;
    int visited;
    struct list_head visited_list_link;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct eventpoll {
    struct mutex mtx;
    wait_queue_head_t wq;
    wait_queue_head_t poll_wait;
    struct list_head rdllist;
    rwlock_t lock;
    struct rb_root_cached rbr;
    struct epitem *ovflist;
    struct wakeup_source *ws;
    struct user_struct *user;
    struct file *file;
    int visited;
    struct list_head visited_list_link;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct eventpoll {
    struct mutex mtx;
    wait_queue_head_t wq;
    wait_queue_head_t poll_wait;
    struct list_head rdllist;
    rwlock_t lock;
    struct rb_root_cached rbr;
    struct epitem *ovflist;
    struct wakeup_source *ws;
    struct user_struct *user;
    struct file *file;
    int visited;
    struct list_head visited_list_link;
    unsigned int napi_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct eventpoll {
    struct mutex mtx;
    wait_queue_head_t wq;
    wait_queue_head_t poll_wait;
    struct list_head rdllist;
    rwlock_t lock;
    struct rb_root_cached rbr;
    struct epitem *ovflist;
    struct wakeup_source *ws;
    struct user_struct *user;
    struct file *file;
    int visited;
    struct list_head visited_list_link;
    unsigned int napi_id;
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
<code>unsigned int napi_id</code>
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
<code>struct rb_root rbr</code> ➡️ <code>struct rb_root_cached rbr</code>
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
<b>Field removed. </b>
<code>spinlock_t lock</code>
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
<code>rwlock_t lock</code>
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
<b>Field added. </b>
<code>u64 gen</code>
</li>
<li>
<b>Field removed. </b>
<code>int visited</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head visited_list_link</code>
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
<code>struct hlist_head refs</code>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>refcount_t refcount</code>
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
