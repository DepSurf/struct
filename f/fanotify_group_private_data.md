# Struct: <code>fanotify_group_private_data</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct fanotify_group_private_data {
    spinlock_t access_lock;
    struct list_head access_list;
    wait_queue_head_t access_waitq;
    atomic_t bypass_perm;
    int f_flags;
    unsigned int max_marks;
    struct user_struct *user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct fanotify_group_private_data {
    spinlock_t access_lock;
    struct list_head access_list;
    wait_queue_head_t access_waitq;
    int f_flags;
    unsigned int max_marks;
    struct user_struct *user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct fanotify_group_private_data {
    struct list_head access_list;
    wait_queue_head_t access_waitq;
    int f_flags;
    unsigned int max_marks;
    struct user_struct *user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct fanotify_group_private_data {
    struct list_head access_list;
    wait_queue_head_t access_waitq;
    int f_flags;
    unsigned int max_marks;
    struct user_struct *user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct fanotify_group_private_data {
    struct list_head access_list;
    wait_queue_head_t access_waitq;
    int f_flags;
    unsigned int max_marks;
    struct user_struct *user;
    bool audit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct fanotify_group_private_data {
    struct list_head access_list;
    wait_queue_head_t access_waitq;
    int f_flags;
    unsigned int max_marks;
    struct user_struct *user;
    bool audit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct fanotify_group_private_data {
    struct list_head access_list;
    wait_queue_head_t access_waitq;
    int flags;
    int f_flags;
    unsigned int max_marks;
    struct user_struct *user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct fanotify_group_private_data {
    struct list_head access_list;
    wait_queue_head_t access_waitq;
    int flags;
    int f_flags;
    unsigned int max_marks;
    struct user_struct *user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct fanotify_group_private_data {
    struct list_head access_list;
    wait_queue_head_t access_waitq;
    int flags;
    int f_flags;
    unsigned int max_marks;
    struct user_struct *user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct fanotify_group_private_data {
    struct list_head access_list;
    wait_queue_head_t access_waitq;
    int flags;
    int f_flags;
    unsigned int max_marks;
    struct user_struct *user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct fanotify_group_private_data {
    struct list_head access_list;
    wait_queue_head_t access_waitq;
    int flags;
    int f_flags;
    unsigned int max_marks;
    struct user_struct *user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct fanotify_group_private_data {
    struct hlist_head *merge_hash;
    struct list_head access_list;
    wait_queue_head_t access_waitq;
    int flags;
    int f_flags;
    struct ucounts *ucounts;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct fanotify_group_private_data {
    struct hlist_head *merge_hash;
    struct list_head access_list;
    wait_queue_head_t access_waitq;
    int flags;
    int f_flags;
    struct ucounts *ucounts;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct fanotify_group_private_data {
    struct hlist_head *merge_hash;
    struct list_head access_list;
    wait_queue_head_t access_waitq;
    int flags;
    int f_flags;
    struct ucounts *ucounts;
    mempool_t error_events_pool;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct fanotify_group_private_data {
    struct hlist_head *merge_hash;
    struct list_head access_list;
    wait_queue_head_t access_waitq;
    int flags;
    int f_flags;
    struct ucounts *ucounts;
    mempool_t error_events_pool;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct fanotify_group_private_data {
    struct hlist_head *merge_hash;
    struct list_head access_list;
    wait_queue_head_t access_waitq;
    int flags;
    int f_flags;
    struct ucounts *ucounts;
    mempool_t error_events_pool;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct fanotify_group_private_data {
    struct hlist_head *merge_hash;
    struct list_head access_list;
    wait_queue_head_t access_waitq;
    int flags;
    int f_flags;
    struct ucounts *ucounts;
    mempool_t error_events_pool;
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
struct fanotify_group_private_data {
    struct list_head access_list;
    wait_queue_head_t access_waitq;
    int flags;
    int f_flags;
    unsigned int max_marks;
    struct user_struct *user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct fanotify_group_private_data {
    struct list_head access_list;
    wait_queue_head_t access_waitq;
    int flags;
    int f_flags;
    unsigned int max_marks;
    struct user_struct *user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct fanotify_group_private_data {
    struct list_head access_list;
    wait_queue_head_t access_waitq;
    int flags;
    int f_flags;
    unsigned int max_marks;
    struct user_struct *user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct fanotify_group_private_data {
    struct list_head access_list;
    wait_queue_head_t access_waitq;
    int flags;
    int f_flags;
    unsigned int max_marks;
    struct user_struct *user;
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
struct fanotify_group_private_data {
    struct list_head access_list;
    wait_queue_head_t access_waitq;
    int flags;
    int f_flags;
    unsigned int max_marks;
    struct user_struct *user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct fanotify_group_private_data {
    struct list_head access_list;
    wait_queue_head_t access_waitq;
    int flags;
    int f_flags;
    unsigned int max_marks;
    struct user_struct *user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct fanotify_group_private_data {
    struct list_head access_list;
    wait_queue_head_t access_waitq;
    int flags;
    int f_flags;
    unsigned int max_marks;
    struct user_struct *user;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct fanotify_group_private_data {
    struct list_head access_list;
    wait_queue_head_t access_waitq;
    int flags;
    int f_flags;
    unsigned int max_marks;
    struct user_struct *user;
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
<b>Field removed. </b>
<code>atomic_t bypass_perm</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>spinlock_t access_lock</code>
</li>
</ul>
</details>
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
<code>bool audit</code>
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
<code>int flags</code>
</li>
<li>
<b>Field removed. </b>
<code>bool audit</code>
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
<b>Field added. </b>
<code>struct hlist_head *merge_hash</code>
</li>
<li>
<b>Field added. </b>
<code>struct ucounts *ucounts</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int max_marks</code>
</li>
<li>
<b>Field removed. </b>
<code>struct user_struct *user</code>
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
<code>mempool_t error_events_pool</code>
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
