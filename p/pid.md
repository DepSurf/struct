# Struct: <code>pid</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct pid {
    atomic_t count;
    unsigned int level;
    struct hlist_head tasks[3];
    struct callback_head rcu;
    struct upid numbers[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct pid {
    atomic_t count;
    unsigned int level;
    struct hlist_head tasks[3];
    struct callback_head rcu;
    struct upid numbers[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct pid {
    atomic_t count;
    unsigned int level;
    struct hlist_head tasks[3];
    struct callback_head rcu;
    struct upid numbers[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct pid {
    atomic_t count;
    unsigned int level;
    struct hlist_head tasks[3];
    struct callback_head rcu;
    struct upid numbers[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct pid {
    atomic_t count;
    unsigned int level;
    struct hlist_head tasks[3];
    struct callback_head rcu;
    struct upid numbers[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct pid {
    atomic_t count;
    unsigned int level;
    struct hlist_head tasks[3];
    struct callback_head rcu;
    struct upid numbers[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct pid {
    atomic_t count;
    unsigned int level;
    struct hlist_head tasks[4];
    struct callback_head rcu;
    struct upid numbers[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct pid {
    refcount_t count;
    unsigned int level;
    struct hlist_head tasks[4];
    wait_queue_head_t wait_pidfd;
    struct callback_head rcu;
    struct upid numbers[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct pid {
    refcount_t count;
    unsigned int level;
    struct hlist_head tasks[4];
    wait_queue_head_t wait_pidfd;
    struct callback_head rcu;
    struct upid numbers[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct pid {
    refcount_t count;
    unsigned int level;
    spinlock_t lock;
    struct hlist_head tasks[4];
    struct hlist_head inodes;
    wait_queue_head_t wait_pidfd;
    struct callback_head rcu;
    struct upid numbers[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct pid {
    refcount_t count;
    unsigned int level;
    spinlock_t lock;
    struct hlist_head tasks[4];
    struct hlist_head inodes;
    wait_queue_head_t wait_pidfd;
    struct callback_head rcu;
    struct upid numbers[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct pid {
    refcount_t count;
    unsigned int level;
    spinlock_t lock;
    struct hlist_head tasks[4];
    struct hlist_head inodes;
    wait_queue_head_t wait_pidfd;
    struct callback_head rcu;
    struct upid numbers[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct pid {
    refcount_t count;
    unsigned int level;
    spinlock_t lock;
    struct hlist_head tasks[4];
    struct hlist_head inodes;
    wait_queue_head_t wait_pidfd;
    struct callback_head rcu;
    struct upid numbers[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct pid {
    refcount_t count;
    unsigned int level;
    spinlock_t lock;
    struct hlist_head tasks[4];
    struct hlist_head inodes;
    wait_queue_head_t wait_pidfd;
    struct callback_head rcu;
    struct upid numbers[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct pid {
    refcount_t count;
    unsigned int level;
    spinlock_t lock;
    struct hlist_head tasks[4];
    struct hlist_head inodes;
    wait_queue_head_t wait_pidfd;
    struct callback_head rcu;
    struct upid numbers[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct pid {
    refcount_t count;
    unsigned int level;
    spinlock_t lock;
    struct hlist_head tasks[4];
    struct hlist_head inodes;
    wait_queue_head_t wait_pidfd;
    struct callback_head rcu;
    struct upid numbers[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct pid {
    refcount_t count;
    unsigned int level;
    spinlock_t lock;
    struct hlist_head tasks[4];
    struct hlist_head inodes;
    wait_queue_head_t wait_pidfd;
    struct callback_head rcu;
    struct upid numbers[0];
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
struct pid {
    refcount_t count;
    unsigned int level;
    struct hlist_head tasks[4];
    wait_queue_head_t wait_pidfd;
    struct callback_head rcu;
    struct upid numbers[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct pid {
    refcount_t count;
    unsigned int level;
    struct hlist_head tasks[4];
    wait_queue_head_t wait_pidfd;
    struct callback_head rcu;
    struct upid numbers[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct pid {
    refcount_t count;
    unsigned int level;
    struct hlist_head tasks[4];
    wait_queue_head_t wait_pidfd;
    struct callback_head rcu;
    struct upid numbers[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct pid {
    refcount_t count;
    unsigned int level;
    struct hlist_head tasks[4];
    wait_queue_head_t wait_pidfd;
    struct callback_head rcu;
    struct upid numbers[1];
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
struct pid {
    refcount_t count;
    unsigned int level;
    struct hlist_head tasks[4];
    wait_queue_head_t wait_pidfd;
    struct callback_head rcu;
    struct upid numbers[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct pid {
    refcount_t count;
    unsigned int level;
    struct hlist_head tasks[4];
    wait_queue_head_t wait_pidfd;
    struct callback_head rcu;
    struct upid numbers[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct pid {
    refcount_t count;
    unsigned int level;
    struct hlist_head tasks[4];
    wait_queue_head_t wait_pidfd;
    struct callback_head rcu;
    struct upid numbers[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct pid {
    refcount_t count;
    unsigned int level;
    struct hlist_head tasks[4];
    wait_queue_head_t wait_pidfd;
    struct callback_head rcu;
    struct upid numbers[1];
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
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct hlist_head tasks[3]</code> ➡️ <code>struct hlist_head tasks[4]</code>
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
<code>wait_queue_head_t wait_pidfd</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_t count</code> ➡️ <code>refcount_t count</code>
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
<code>spinlock_t lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct hlist_head inodes</code>
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
<b>Field type changed. </b>
<code>struct upid numbers[1]</code> ➡️ <code>struct upid numbers[0]</code>
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
