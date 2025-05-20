# Struct: <code>kfree_rcu_cpu</code>

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
struct kfree_rcu_cpu {
    struct callback_head *head;
    struct kfree_rcu_bulk_data *bhead;
    struct kfree_rcu_bulk_data *bcached;
    struct kfree_rcu_cpu_work krw_arr[2];
    spinlock_t lock;
    struct delayed_work monitor_work;
    bool monitor_todo;
    bool initialized;
    int count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct kfree_rcu_cpu {
    struct callback_head *head;
    struct kvfree_rcu_bulk_data * bkvhead[2];
    struct kfree_rcu_cpu_work krw_arr[2];
    raw_spinlock_t lock;
    struct delayed_work monitor_work;
    bool monitor_todo;
    bool initialized;
    int count;
    struct work_struct page_cache_work;
    atomic_t work_in_progress;
    struct hrtimer hrtimer;
    struct llist_head bkvcache;
    int nr_bkv_objs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kfree_rcu_cpu {
    struct callback_head *head;
    struct kvfree_rcu_bulk_data * bkvhead[2];
    struct kfree_rcu_cpu_work krw_arr[2];
    raw_spinlock_t lock;
    struct delayed_work monitor_work;
    bool monitor_todo;
    bool initialized;
    int count;
    struct work_struct page_cache_work;
    atomic_t work_in_progress;
    struct hrtimer hrtimer;
    struct llist_head bkvcache;
    int nr_bkv_objs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kfree_rcu_cpu {
    struct callback_head *head;
    struct kvfree_rcu_bulk_data * bkvhead[2];
    struct kfree_rcu_cpu_work krw_arr[2];
    raw_spinlock_t lock;
    struct delayed_work monitor_work;
    bool monitor_todo;
    bool initialized;
    int count;
    struct delayed_work page_cache_work;
    atomic_t backoff_page_cache_fill;
    atomic_t work_in_progress;
    struct hrtimer hrtimer;
    struct llist_head bkvcache;
    int nr_bkv_objs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kfree_rcu_cpu {
    struct callback_head *head;
    struct kvfree_rcu_bulk_data * bkvhead[2];
    struct kfree_rcu_cpu_work krw_arr[2];
    raw_spinlock_t lock;
    struct delayed_work monitor_work;
    bool monitor_todo;
    bool initialized;
    int count;
    struct delayed_work page_cache_work;
    atomic_t backoff_page_cache_fill;
    atomic_t work_in_progress;
    struct hrtimer hrtimer;
    struct llist_head bkvcache;
    int nr_bkv_objs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kfree_rcu_cpu {
    struct callback_head *head;
    struct kvfree_rcu_bulk_data * bkvhead[2];
    struct kfree_rcu_cpu_work krw_arr[2];
    raw_spinlock_t lock;
    struct delayed_work monitor_work;
    bool initialized;
    int count;
    struct delayed_work page_cache_work;
    atomic_t backoff_page_cache_fill;
    atomic_t work_in_progress;
    struct hrtimer hrtimer;
    struct llist_head bkvcache;
    int nr_bkv_objs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kfree_rcu_cpu {
    struct callback_head *head;
    long unsigned int head_gp_snap;
    atomic_t head_count;
    struct list_head bulk_head[2];
    atomic_t bulk_count[2];
    struct kfree_rcu_cpu_work krw_arr[2];
    raw_spinlock_t lock;
    struct delayed_work monitor_work;
    bool initialized;
    struct delayed_work page_cache_work;
    atomic_t backoff_page_cache_fill;
    atomic_t work_in_progress;
    struct hrtimer hrtimer;
    struct llist_head bkvcache;
    int nr_bkv_objs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kfree_rcu_cpu {
    struct callback_head *head;
    long unsigned int head_gp_snap;
    atomic_t head_count;
    struct list_head bulk_head[2];
    atomic_t bulk_count[2];
    struct kfree_rcu_cpu_work krw_arr[2];
    raw_spinlock_t lock;
    struct delayed_work monitor_work;
    bool initialized;
    struct delayed_work page_cache_work;
    atomic_t backoff_page_cache_fill;
    atomic_t work_in_progress;
    struct hrtimer hrtimer;
    struct llist_head bkvcache;
    int nr_bkv_objs;
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
<code>struct kvfree_rcu_bulk_data * bkvhead[2]</code>
</li>
<li>
<b>Field added. </b>
<code>struct work_struct page_cache_work</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t work_in_progress</code>
</li>
<li>
<b>Field added. </b>
<code>struct hrtimer hrtimer</code>
</li>
<li>
<b>Field added. </b>
<code>struct llist_head bkvcache</code>
</li>
<li>
<b>Field added. </b>
<code>int nr_bkv_objs</code>
</li>
<li>
<b>Field removed. </b>
<code>struct kfree_rcu_bulk_data *bhead</code>
</li>
<li>
<b>Field removed. </b>
<code>struct kfree_rcu_bulk_data *bcached</code>
</li>
<li>
<b>Field type changed. </b>
<code>spinlock_t lock</code> ➡️ <code>raw_spinlock_t lock</code>
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
<b>Field added. </b>
<code>atomic_t backoff_page_cache_fill</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct work_struct page_cache_work</code> ➡️ <code>struct delayed_work page_cache_work</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>bool monitor_todo</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int head_gp_snap</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t head_count</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head bulk_head[2]</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t bulk_count[2]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct kvfree_rcu_bulk_data * bkvhead[2]</code>
</li>
<li>
<b>Field removed. </b>
<code>int count</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
