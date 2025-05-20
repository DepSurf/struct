# Struct: <code>io_worker</code>

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
struct io_worker {
    refcount_t ref;
    unsigned int flags;
    struct hlist_nulls_node nulls_node;
    struct list_head all_list;
    struct task_struct *task;
    struct io_wqe *wqe;
    struct io_wq_work *cur_work;
    spinlock_t lock;
    struct callback_head rcu;
    struct mm_struct *mm;
    const struct cred *cur_creds;
    const struct cred *saved_creds;
    struct files_struct *restore_files;
    struct fs_struct *restore_fs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct io_worker {
    refcount_t ref;
    unsigned int flags;
    struct hlist_nulls_node nulls_node;
    struct list_head all_list;
    struct task_struct *task;
    struct io_wqe *wqe;
    struct io_wq_work *cur_work;
    spinlock_t lock;
    struct callback_head rcu;
    struct mm_struct *mm;
    struct cgroup_subsys_state *blkcg_css;
    const struct cred *cur_creds;
    const struct cred *saved_creds;
    struct files_struct *restore_files;
    struct nsproxy *restore_nsproxy;
    struct fs_struct *restore_fs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct io_worker {
    refcount_t ref;
    unsigned int flags;
    struct hlist_nulls_node nulls_node;
    struct list_head all_list;
    struct task_struct *task;
    struct io_wqe *wqe;
    struct io_wq_work *cur_work;
    spinlock_t lock;
    struct completion ref_done;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct io_worker {
    refcount_t ref;
    unsigned int flags;
    struct hlist_nulls_node nulls_node;
    struct list_head all_list;
    struct task_struct *task;
    struct io_wqe *wqe;
    struct io_wq_work *cur_work;
    spinlock_t lock;
    struct completion ref_done;
    long unsigned int create_state;
    struct callback_head create_work;
    int create_index;
    struct callback_head rcu;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct io_worker {
    refcount_t ref;
    unsigned int flags;
    struct hlist_nulls_node nulls_node;
    struct list_head all_list;
    struct task_struct *task;
    struct io_wqe *wqe;
    struct io_wq_work *cur_work;
    struct io_wq_work *next_work;
    raw_spinlock_t lock;
    struct completion ref_done;
    long unsigned int create_state;
    struct callback_head create_work;
    int create_index;
    struct callback_head rcu;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct io_worker {
    refcount_t ref;
    unsigned int flags;
    struct hlist_nulls_node nulls_node;
    struct list_head all_list;
    struct task_struct *task;
    struct io_wqe *wqe;
    struct io_wq_work *cur_work;
    struct io_wq_work *next_work;
    raw_spinlock_t lock;
    struct completion ref_done;
    long unsigned int create_state;
    struct callback_head create_work;
    int create_index;
    struct callback_head rcu;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct io_worker {
    refcount_t ref;
    unsigned int flags;
    struct hlist_nulls_node nulls_node;
    struct list_head all_list;
    struct task_struct *task;
    struct io_wq *wq;
    struct io_wq_work *cur_work;
    struct io_wq_work *next_work;
    raw_spinlock_t lock;
    struct completion ref_done;
    long unsigned int create_state;
    struct callback_head create_work;
    int create_index;
    struct callback_head rcu;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct io_worker {
    refcount_t ref;
    unsigned int flags;
    struct hlist_nulls_node nulls_node;
    struct list_head all_list;
    struct task_struct *task;
    struct io_wq *wq;
    struct io_wq_work *cur_work;
    struct io_wq_work *next_work;
    raw_spinlock_t lock;
    struct completion ref_done;
    long unsigned int create_state;
    struct callback_head create_work;
    int create_index;
    struct callback_head rcu;
    struct work_struct work;
};
```
</details>
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
<b>Field added. </b>
<code>struct cgroup_subsys_state *blkcg_css</code>
</li>
<li>
<b>Field added. </b>
<code>struct nsproxy *restore_nsproxy</code>
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
<code>struct completion ref_done</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mm_struct *mm</code>
</li>
<li>
<b>Field removed. </b>
<code>struct cgroup_subsys_state *blkcg_css</code>
</li>
<li>
<b>Field removed. </b>
<code>const struct cred *cur_creds</code>
</li>
<li>
<b>Field removed. </b>
<code>const struct cred *saved_creds</code>
</li>
<li>
<b>Field removed. </b>
<code>struct files_struct *restore_files</code>
</li>
<li>
<b>Field removed. </b>
<code>struct nsproxy *restore_nsproxy</code>
</li>
<li>
<b>Field removed. </b>
<code>struct fs_struct *restore_fs</code>
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
<code>long unsigned int create_state</code>
</li>
<li>
<b>Field added. </b>
<code>struct callback_head create_work</code>
</li>
<li>
<b>Field added. </b>
<code>int create_index</code>
</li>
<li>
<b>Field added. </b>
<code>struct work_struct work</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct io_wq_work *next_work</code>
</li>
<li>
<b>Field type changed. </b>
<code>spinlock_t lock</code> ➡️ <code>raw_spinlock_t lock</code>
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
<code>struct io_wq *wq</code>
</li>
<li>
<b>Field removed. </b>
<code>struct io_wqe *wqe</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
