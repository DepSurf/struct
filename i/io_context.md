# Struct: <code>io_context</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct io_context {
    atomic_long_t refcount;
    atomic_t active_ref;
    atomic_t nr_tasks;
    spinlock_t lock;
    short unsigned int ioprio;
    int nr_batch_requests;
    long unsigned int last_waited;
    struct radix_tree_root icq_tree;
    struct io_cq *icq_hint;
    struct hlist_head icq_list;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct io_context {
    atomic_long_t refcount;
    atomic_t active_ref;
    atomic_t nr_tasks;
    spinlock_t lock;
    short unsigned int ioprio;
    int nr_batch_requests;
    long unsigned int last_waited;
    struct radix_tree_root icq_tree;
    struct io_cq *icq_hint;
    struct hlist_head icq_list;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct io_context {
    atomic_long_t refcount;
    atomic_t active_ref;
    atomic_t nr_tasks;
    spinlock_t lock;
    short unsigned int ioprio;
    int nr_batch_requests;
    long unsigned int last_waited;
    struct radix_tree_root icq_tree;
    struct io_cq *icq_hint;
    struct hlist_head icq_list;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct io_context {
    atomic_long_t refcount;
    atomic_t active_ref;
    atomic_t nr_tasks;
    spinlock_t lock;
    short unsigned int ioprio;
    int nr_batch_requests;
    long unsigned int last_waited;
    struct radix_tree_root icq_tree;
    struct io_cq *icq_hint;
    struct hlist_head icq_list;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct io_context {
    atomic_long_t refcount;
    atomic_t active_ref;
    atomic_t nr_tasks;
    spinlock_t lock;
    short unsigned int ioprio;
    int nr_batch_requests;
    long unsigned int last_waited;
    struct radix_tree_root icq_tree;
    struct io_cq *icq_hint;
    struct hlist_head icq_list;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct io_context {
    atomic_long_t refcount;
    atomic_t active_ref;
    atomic_t nr_tasks;
    spinlock_t lock;
    short unsigned int ioprio;
    int nr_batch_requests;
    long unsigned int last_waited;
    struct radix_tree_root icq_tree;
    struct io_cq *icq_hint;
    struct hlist_head icq_list;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct io_context {
    atomic_long_t refcount;
    atomic_t active_ref;
    atomic_t nr_tasks;
    spinlock_t lock;
    short unsigned int ioprio;
    int nr_batch_requests;
    long unsigned int last_waited;
    struct xarray icq_tree;
    struct io_cq *icq_hint;
    struct hlist_head icq_list;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct io_context {
    atomic_long_t refcount;
    atomic_t active_ref;
    atomic_t nr_tasks;
    spinlock_t lock;
    short unsigned int ioprio;
    int nr_batch_requests;
    long unsigned int last_waited;
    struct xarray icq_tree;
    struct io_cq *icq_hint;
    struct hlist_head icq_list;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct io_context {
    atomic_long_t refcount;
    atomic_t active_ref;
    atomic_t nr_tasks;
    spinlock_t lock;
    short unsigned int ioprio;
    int nr_batch_requests;
    long unsigned int last_waited;
    struct xarray icq_tree;
    struct io_cq *icq_hint;
    struct hlist_head icq_list;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct io_context {
    atomic_long_t refcount;
    atomic_t active_ref;
    atomic_t nr_tasks;
    spinlock_t lock;
    short unsigned int ioprio;
    int nr_batch_requests;
    long unsigned int last_waited;
    struct xarray icq_tree;
    struct io_cq *icq_hint;
    struct hlist_head icq_list;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct io_context {
    atomic_long_t refcount;
    atomic_t active_ref;
    atomic_t nr_tasks;
    spinlock_t lock;
    short unsigned int ioprio;
    struct xarray icq_tree;
    struct io_cq *icq_hint;
    struct hlist_head icq_list;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct io_context {
    atomic_long_t refcount;
    atomic_t active_ref;
    atomic_t nr_tasks;
    spinlock_t lock;
    short unsigned int ioprio;
    struct xarray icq_tree;
    struct io_cq *icq_hint;
    struct hlist_head icq_list;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct io_context {
    atomic_long_t refcount;
    atomic_t active_ref;
    atomic_t nr_tasks;
    spinlock_t lock;
    short unsigned int ioprio;
    struct xarray icq_tree;
    struct io_cq *icq_hint;
    struct hlist_head icq_list;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct io_context {
    atomic_long_t refcount;
    atomic_t active_ref;
    short unsigned int ioprio;
    spinlock_t lock;
    struct xarray icq_tree;
    struct io_cq *icq_hint;
    struct hlist_head icq_list;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct io_context {
    atomic_long_t refcount;
    atomic_t active_ref;
    short unsigned int ioprio;
    spinlock_t lock;
    struct xarray icq_tree;
    struct io_cq *icq_hint;
    struct hlist_head icq_list;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct io_context {
    atomic_long_t refcount;
    atomic_t active_ref;
    short unsigned int ioprio;
    spinlock_t lock;
    struct xarray icq_tree;
    struct io_cq *icq_hint;
    struct hlist_head icq_list;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct io_context {
    atomic_long_t refcount;
    atomic_t active_ref;
    short unsigned int ioprio;
    spinlock_t lock;
    struct xarray icq_tree;
    struct io_cq *icq_hint;
    struct hlist_head icq_list;
    struct work_struct release_work;
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
struct io_context {
    atomic_long_t refcount;
    atomic_t active_ref;
    atomic_t nr_tasks;
    spinlock_t lock;
    short unsigned int ioprio;
    int nr_batch_requests;
    long unsigned int last_waited;
    struct xarray icq_tree;
    struct io_cq *icq_hint;
    struct hlist_head icq_list;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct io_context {
    atomic_long_t refcount;
    atomic_t active_ref;
    atomic_t nr_tasks;
    spinlock_t lock;
    short unsigned int ioprio;
    int nr_batch_requests;
    long unsigned int last_waited;
    struct xarray icq_tree;
    struct io_cq *icq_hint;
    struct hlist_head icq_list;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct io_context {
    atomic_long_t refcount;
    atomic_t active_ref;
    atomic_t nr_tasks;
    spinlock_t lock;
    short unsigned int ioprio;
    int nr_batch_requests;
    long unsigned int last_waited;
    struct xarray icq_tree;
    struct io_cq *icq_hint;
    struct hlist_head icq_list;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct io_context {
    atomic_long_t refcount;
    atomic_t active_ref;
    atomic_t nr_tasks;
    spinlock_t lock;
    short unsigned int ioprio;
    int nr_batch_requests;
    long unsigned int last_waited;
    struct xarray icq_tree;
    struct io_cq *icq_hint;
    struct hlist_head icq_list;
    struct work_struct release_work;
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
struct io_context {
    atomic_long_t refcount;
    atomic_t active_ref;
    atomic_t nr_tasks;
    spinlock_t lock;
    short unsigned int ioprio;
    int nr_batch_requests;
    long unsigned int last_waited;
    struct xarray icq_tree;
    struct io_cq *icq_hint;
    struct hlist_head icq_list;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct io_context {
    atomic_long_t refcount;
    atomic_t active_ref;
    atomic_t nr_tasks;
    spinlock_t lock;
    short unsigned int ioprio;
    int nr_batch_requests;
    long unsigned int last_waited;
    struct xarray icq_tree;
    struct io_cq *icq_hint;
    struct hlist_head icq_list;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct io_context {
    atomic_long_t refcount;
    atomic_t active_ref;
    atomic_t nr_tasks;
    spinlock_t lock;
    short unsigned int ioprio;
    int nr_batch_requests;
    long unsigned int last_waited;
    struct xarray icq_tree;
    struct io_cq *icq_hint;
    struct hlist_head icq_list;
    struct work_struct release_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct io_context {
    atomic_long_t refcount;
    atomic_t active_ref;
    atomic_t nr_tasks;
    spinlock_t lock;
    short unsigned int ioprio;
    int nr_batch_requests;
    long unsigned int last_waited;
    struct xarray icq_tree;
    struct io_cq *icq_hint;
    struct hlist_head icq_list;
    struct work_struct release_work;
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
<code>struct radix_tree_root icq_tree</code> ➡️ <code>struct xarray icq_tree</code>
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
<b>Field removed. </b>
<code>int nr_batch_requests</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int last_waited</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>atomic_t nr_tasks</code>
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
