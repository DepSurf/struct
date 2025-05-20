# Struct: <code>io_wqe</code>

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
In <code>4.13</code>: Absent ⚠️
</li>
<li>
In <code>4.15</code>: Absent ⚠️
</li>
<li>
In <code>4.18</code>: Absent ⚠️
</li>
<li>
In <code>5.0</code>: Absent ⚠️
</li>
<li>
In <code>5.3</code>: Absent ⚠️
</li>
<li>
In <code>5.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct io_wqe {
    spinlock_t lock;
    struct io_wq_work_list work_list;
    long unsigned int hash_map;
    unsigned int flags;
    int node;
    struct io_wqe_acct acct[2];
    struct hlist_nulls_head free_list;
    struct list_head all_list;
    struct io_wq *wq;
    struct io_wq_work * hash_tail[64];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct io_wqe {
    raw_spinlock_t lock;
    struct io_wq_work_list work_list;
    long unsigned int hash_map;
    unsigned int flags;
    int node;
    struct io_wqe_acct acct[2];
    struct hlist_nulls_head free_list;
    struct list_head all_list;
    struct io_wq *wq;
    struct io_wq_work * hash_tail[64];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct io_wqe {
    raw_spinlock_t lock;
    struct io_wq_work_list work_list;
    unsigned int flags;
    int node;
    struct io_wqe_acct acct[2];
    struct hlist_nulls_head free_list;
    struct list_head all_list;
    struct wait_queue_entry wait;
    struct io_wq *wq;
    struct io_wq_work * hash_tail[64];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct io_wqe {
    raw_spinlock_t lock;
    struct io_wqe_acct acct[2];
    int node;
    struct hlist_nulls_head free_list;
    struct list_head all_list;
    struct wait_queue_entry wait;
    struct io_wq *wq;
    struct io_wq_work * hash_tail[64];
    cpumask_var_t cpu_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct io_wqe {
    raw_spinlock_t lock;
    struct io_wqe_acct acct[2];
    int node;
    struct hlist_nulls_head free_list;
    struct list_head all_list;
    struct wait_queue_entry wait;
    struct io_wq *wq;
    struct io_wq_work * hash_tail[64];
    cpumask_var_t cpu_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct io_wqe {
    raw_spinlock_t lock;
    struct io_wqe_acct acct[2];
    int node;
    struct hlist_nulls_head free_list;
    struct list_head all_list;
    struct wait_queue_entry wait;
    struct io_wq *wq;
    struct io_wq_work * hash_tail[64];
    cpumask_var_t cpu_mask;
};
```
</details>
</li>
<li>
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
</li>
</ul>
<b>Arch</b>
<ul>
<li>
In <code>arm64</code>: Absent ⚠️
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
</li>
<li>
In <code>riscv64</code>: Absent ⚠️
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
In <code>aws</code>: Absent ⚠️
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>spinlock_t lock</code> ➡️ <code>raw_spinlock_t lock</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct wait_queue_entry wait</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int hash_map</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>cpumask_var_t cpu_mask</code>
</li>
<li>
<b>Field removed. </b>
<code>struct io_wq_work_list work_list</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int flags</code>
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
</ul>
