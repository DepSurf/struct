# Struct: <code>percpu_rw_semaphore</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct percpu_rw_semaphore {
    struct rcu_sync rss;
    unsigned int *fast_read_ctr;
    struct rw_semaphore rw_sem;
    atomic_t slow_read_ctr;
    wait_queue_head_t write_waitq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct percpu_rw_semaphore {
    struct rcu_sync rss;
    unsigned int *fast_read_ctr;
    struct rw_semaphore rw_sem;
    atomic_t slow_read_ctr;
    wait_queue_head_t write_waitq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct percpu_rw_semaphore {
    struct rcu_sync rss;
    unsigned int *read_count;
    struct rw_semaphore rw_sem;
    wait_queue_head_t writer;
    int readers_block;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct percpu_rw_semaphore {
    struct rcu_sync rss;
    unsigned int *read_count;
    struct rw_semaphore rw_sem;
    struct rcuwait writer;
    int readers_block;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct percpu_rw_semaphore {
    struct rcu_sync rss;
    unsigned int *read_count;
    struct rw_semaphore rw_sem;
    struct rcuwait writer;
    int readers_block;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct percpu_rw_semaphore {
    struct rcu_sync rss;
    unsigned int *read_count;
    struct rw_semaphore rw_sem;
    struct rcuwait writer;
    int readers_block;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct percpu_rw_semaphore {
    struct rcu_sync rss;
    unsigned int *read_count;
    struct rw_semaphore rw_sem;
    struct rcuwait writer;
    int readers_block;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct percpu_rw_semaphore {
    struct rcu_sync rss;
    unsigned int *read_count;
    struct rw_semaphore rw_sem;
    struct rcuwait writer;
    int readers_block;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct percpu_rw_semaphore {
    struct rcu_sync rss;
    unsigned int *read_count;
    struct rw_semaphore rw_sem;
    struct rcuwait writer;
    int readers_block;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct percpu_rw_semaphore {
    struct rcu_sync rss;
    unsigned int *read_count;
    struct rcuwait writer;
    wait_queue_head_t waiters;
    atomic_t block;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct percpu_rw_semaphore {
    struct rcu_sync rss;
    unsigned int *read_count;
    struct rcuwait writer;
    wait_queue_head_t waiters;
    atomic_t block;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct percpu_rw_semaphore {
    struct rcu_sync rss;
    unsigned int *read_count;
    struct rcuwait writer;
    wait_queue_head_t waiters;
    atomic_t block;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct percpu_rw_semaphore {
    struct rcu_sync rss;
    unsigned int *read_count;
    struct rcuwait writer;
    wait_queue_head_t waiters;
    atomic_t block;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct percpu_rw_semaphore {
    struct rcu_sync rss;
    unsigned int *read_count;
    struct rcuwait writer;
    wait_queue_head_t waiters;
    atomic_t block;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct percpu_rw_semaphore {
    struct rcu_sync rss;
    unsigned int *read_count;
    struct rcuwait writer;
    wait_queue_head_t waiters;
    atomic_t block;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct percpu_rw_semaphore {
    struct rcu_sync rss;
    unsigned int *read_count;
    struct rcuwait writer;
    wait_queue_head_t waiters;
    atomic_t block;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct percpu_rw_semaphore {
    struct rcu_sync rss;
    unsigned int *read_count;
    struct rcuwait writer;
    wait_queue_head_t waiters;
    atomic_t block;
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
struct percpu_rw_semaphore {
    struct rcu_sync rss;
    unsigned int *read_count;
    struct rw_semaphore rw_sem;
    struct rcuwait writer;
    int readers_block;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct percpu_rw_semaphore {
    struct rcu_sync rss;
    unsigned int *read_count;
    struct rw_semaphore rw_sem;
    struct rcuwait writer;
    int readers_block;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct percpu_rw_semaphore {
    struct rcu_sync rss;
    unsigned int *read_count;
    struct rw_semaphore rw_sem;
    struct rcuwait writer;
    int readers_block;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct percpu_rw_semaphore {
    struct rcu_sync rss;
    unsigned int *read_count;
    struct rw_semaphore rw_sem;
    struct rcuwait writer;
    int readers_block;
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
struct percpu_rw_semaphore {
    struct rcu_sync rss;
    unsigned int *read_count;
    struct rw_semaphore rw_sem;
    struct rcuwait writer;
    int readers_block;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct percpu_rw_semaphore {
    struct rcu_sync rss;
    unsigned int *read_count;
    struct rw_semaphore rw_sem;
    struct rcuwait writer;
    int readers_block;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct percpu_rw_semaphore {
    struct rcu_sync rss;
    unsigned int *read_count;
    struct rw_semaphore rw_sem;
    struct rcuwait writer;
    int readers_block;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct percpu_rw_semaphore {
    struct rcu_sync rss;
    unsigned int *read_count;
    struct rw_semaphore rw_sem;
    struct rcuwait writer;
    int readers_block;
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
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int *read_count</code>
</li>
<li>
<b>Field added. </b>
<code>wait_queue_head_t writer</code>
</li>
<li>
<b>Field added. </b>
<code>int readers_block</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int *fast_read_ctr</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t slow_read_ctr</code>
</li>
<li>
<b>Field removed. </b>
<code>wait_queue_head_t write_waitq</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>wait_queue_head_t writer</code> ➡️ <code>struct rcuwait writer</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>wait_queue_head_t waiters</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t block</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rw_semaphore rw_sem</code>
</li>
<li>
<b>Field removed. </b>
<code>int readers_block</code>
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
