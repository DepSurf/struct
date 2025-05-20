# Struct: <code>worker_pool</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct worker_pool {
    spinlock_t lock;
    int cpu;
    int node;
    int id;
    unsigned int flags;
    struct list_head worklist;
    int nr_workers;
    int nr_idle;
    struct list_head idle_list;
    struct timer_list idle_timer;
    struct timer_list mayday_timer;
    struct hlist_head busy_hash[64];
    struct mutex manager_arb;
    struct worker *manager;
    struct mutex attach_mutex;
    struct list_head workers;
    struct completion *detach_completion;
    struct ida worker_ida;
    struct workqueue_attrs *attrs;
    struct hlist_node hash_node;
    int refcnt;
    atomic_t nr_running;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct worker_pool {
    spinlock_t lock;
    int cpu;
    int node;
    int id;
    unsigned int flags;
    long unsigned int watchdog_ts;
    struct list_head worklist;
    int nr_workers;
    int nr_idle;
    struct list_head idle_list;
    struct timer_list idle_timer;
    struct timer_list mayday_timer;
    struct hlist_head busy_hash[64];
    struct mutex manager_arb;
    struct worker *manager;
    struct mutex attach_mutex;
    struct list_head workers;
    struct completion *detach_completion;
    struct ida worker_ida;
    struct workqueue_attrs *attrs;
    struct hlist_node hash_node;
    int refcnt;
    atomic_t nr_running;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct worker_pool {
    spinlock_t lock;
    int cpu;
    int node;
    int id;
    unsigned int flags;
    long unsigned int watchdog_ts;
    struct list_head worklist;
    int nr_workers;
    int nr_idle;
    struct list_head idle_list;
    struct timer_list idle_timer;
    struct timer_list mayday_timer;
    struct hlist_head busy_hash[64];
    struct mutex manager_arb;
    struct worker *manager;
    struct mutex attach_mutex;
    struct list_head workers;
    struct completion *detach_completion;
    struct ida worker_ida;
    struct workqueue_attrs *attrs;
    struct hlist_node hash_node;
    int refcnt;
    atomic_t nr_running;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct worker_pool {
    spinlock_t lock;
    int cpu;
    int node;
    int id;
    unsigned int flags;
    long unsigned int watchdog_ts;
    struct list_head worklist;
    int nr_workers;
    int nr_idle;
    struct list_head idle_list;
    struct timer_list idle_timer;
    struct timer_list mayday_timer;
    struct hlist_head busy_hash[64];
    struct mutex manager_arb;
    struct worker *manager;
    struct mutex attach_mutex;
    struct list_head workers;
    struct completion *detach_completion;
    struct ida worker_ida;
    struct workqueue_attrs *attrs;
    struct hlist_node hash_node;
    int refcnt;
    atomic_t nr_running;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct worker_pool {
    spinlock_t lock;
    int cpu;
    int node;
    int id;
    unsigned int flags;
    long unsigned int watchdog_ts;
    struct list_head worklist;
    int nr_workers;
    int nr_idle;
    struct list_head idle_list;
    struct timer_list idle_timer;
    struct timer_list mayday_timer;
    struct hlist_head busy_hash[64];
    struct worker *manager;
    struct mutex attach_mutex;
    struct list_head workers;
    struct completion *detach_completion;
    struct ida worker_ida;
    struct workqueue_attrs *attrs;
    struct hlist_node hash_node;
    int refcnt;
    atomic_t nr_running;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct worker_pool {
    spinlock_t lock;
    int cpu;
    int node;
    int id;
    unsigned int flags;
    long unsigned int watchdog_ts;
    struct list_head worklist;
    int nr_workers;
    int nr_idle;
    struct list_head idle_list;
    struct timer_list idle_timer;
    struct timer_list mayday_timer;
    struct hlist_head busy_hash[64];
    struct worker *manager;
    struct list_head workers;
    struct completion *detach_completion;
    struct ida worker_ida;
    struct workqueue_attrs *attrs;
    struct hlist_node hash_node;
    int refcnt;
    atomic_t nr_running;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct worker_pool {
    spinlock_t lock;
    int cpu;
    int node;
    int id;
    unsigned int flags;
    long unsigned int watchdog_ts;
    struct list_head worklist;
    int nr_workers;
    int nr_idle;
    struct list_head idle_list;
    struct timer_list idle_timer;
    struct timer_list mayday_timer;
    struct hlist_head busy_hash[64];
    struct worker *manager;
    struct list_head workers;
    struct completion *detach_completion;
    struct ida worker_ida;
    struct workqueue_attrs *attrs;
    struct hlist_node hash_node;
    int refcnt;
    atomic_t nr_running;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct worker_pool {
    spinlock_t lock;
    int cpu;
    int node;
    int id;
    unsigned int flags;
    long unsigned int watchdog_ts;
    struct list_head worklist;
    int nr_workers;
    int nr_idle;
    struct list_head idle_list;
    struct timer_list idle_timer;
    struct timer_list mayday_timer;
    struct hlist_head busy_hash[64];
    struct worker *manager;
    struct list_head workers;
    struct completion *detach_completion;
    struct ida worker_ida;
    struct workqueue_attrs *attrs;
    struct hlist_node hash_node;
    int refcnt;
    atomic_t nr_running;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct worker_pool {
    spinlock_t lock;
    int cpu;
    int node;
    int id;
    unsigned int flags;
    long unsigned int watchdog_ts;
    struct list_head worklist;
    int nr_workers;
    int nr_idle;
    struct list_head idle_list;
    struct timer_list idle_timer;
    struct timer_list mayday_timer;
    struct hlist_head busy_hash[64];
    struct worker *manager;
    struct list_head workers;
    struct completion *detach_completion;
    struct ida worker_ida;
    struct workqueue_attrs *attrs;
    struct hlist_node hash_node;
    int refcnt;
    atomic_t nr_running;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct worker_pool {
    raw_spinlock_t lock;
    int cpu;
    int node;
    int id;
    unsigned int flags;
    long unsigned int watchdog_ts;
    struct list_head worklist;
    int nr_workers;
    int nr_idle;
    struct list_head idle_list;
    struct timer_list idle_timer;
    struct timer_list mayday_timer;
    struct hlist_head busy_hash[64];
    struct worker *manager;
    struct list_head workers;
    struct completion *detach_completion;
    struct ida worker_ida;
    struct workqueue_attrs *attrs;
    struct hlist_node hash_node;
    int refcnt;
    atomic_t nr_running;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct worker_pool {
    raw_spinlock_t lock;
    int cpu;
    int node;
    int id;
    unsigned int flags;
    long unsigned int watchdog_ts;
    struct list_head worklist;
    int nr_workers;
    int nr_idle;
    struct list_head idle_list;
    struct timer_list idle_timer;
    struct timer_list mayday_timer;
    struct hlist_head busy_hash[64];
    struct worker *manager;
    struct list_head workers;
    struct completion *detach_completion;
    struct ida worker_ida;
    struct workqueue_attrs *attrs;
    struct hlist_node hash_node;
    int refcnt;
    atomic_t nr_running;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct worker_pool {
    raw_spinlock_t lock;
    int cpu;
    int node;
    int id;
    unsigned int flags;
    long unsigned int watchdog_ts;
    struct list_head worklist;
    int nr_workers;
    int nr_idle;
    struct list_head idle_list;
    struct timer_list idle_timer;
    struct timer_list mayday_timer;
    struct hlist_head busy_hash[64];
    struct worker *manager;
    struct list_head workers;
    struct completion *detach_completion;
    struct ida worker_ida;
    struct workqueue_attrs *attrs;
    struct hlist_node hash_node;
    int refcnt;
    atomic_t nr_running;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct worker_pool {
    raw_spinlock_t lock;
    int cpu;
    int node;
    int id;
    unsigned int flags;
    long unsigned int watchdog_ts;
    struct list_head worklist;
    int nr_workers;
    int nr_idle;
    struct list_head idle_list;
    struct timer_list idle_timer;
    struct timer_list mayday_timer;
    struct hlist_head busy_hash[64];
    struct worker *manager;
    struct list_head workers;
    struct completion *detach_completion;
    struct ida worker_ida;
    struct workqueue_attrs *attrs;
    struct hlist_node hash_node;
    int refcnt;
    atomic_t nr_running;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct worker_pool {
    raw_spinlock_t lock;
    int cpu;
    int node;
    int id;
    unsigned int flags;
    long unsigned int watchdog_ts;
    int nr_running;
    struct list_head worklist;
    int nr_workers;
    int nr_idle;
    struct list_head idle_list;
    struct timer_list idle_timer;
    struct timer_list mayday_timer;
    struct hlist_head busy_hash[64];
    struct worker *manager;
    struct list_head workers;
    struct completion *detach_completion;
    struct ida worker_ida;
    struct workqueue_attrs *attrs;
    struct hlist_node hash_node;
    int refcnt;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct worker_pool {
    raw_spinlock_t lock;
    int cpu;
    int node;
    int id;
    unsigned int flags;
    long unsigned int watchdog_ts;
    int nr_running;
    struct list_head worklist;
    int nr_workers;
    int nr_idle;
    struct list_head idle_list;
    struct timer_list idle_timer;
    struct timer_list mayday_timer;
    struct hlist_head busy_hash[64];
    struct worker *manager;
    struct list_head workers;
    struct completion *detach_completion;
    struct ida worker_ida;
    struct workqueue_attrs *attrs;
    struct hlist_node hash_node;
    int refcnt;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct worker_pool {
    raw_spinlock_t lock;
    int cpu;
    int node;
    int id;
    unsigned int flags;
    long unsigned int watchdog_ts;
    bool cpu_stall;
    int nr_running;
    struct list_head worklist;
    int nr_workers;
    int nr_idle;
    struct list_head idle_list;
    struct timer_list idle_timer;
    struct work_struct idle_cull_work;
    struct timer_list mayday_timer;
    struct hlist_head busy_hash[64];
    struct worker *manager;
    struct list_head workers;
    struct list_head dying_workers;
    struct completion *detach_completion;
    struct ida worker_ida;
    struct workqueue_attrs *attrs;
    struct hlist_node hash_node;
    int refcnt;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct worker_pool {
    raw_spinlock_t lock;
    int cpu;
    int node;
    int id;
    unsigned int flags;
    long unsigned int watchdog_ts;
    bool cpu_stall;
    int nr_running;
    struct list_head worklist;
    int nr_workers;
    int nr_idle;
    struct list_head idle_list;
    struct timer_list idle_timer;
    struct work_struct idle_cull_work;
    struct timer_list mayday_timer;
    struct hlist_head busy_hash[64];
    struct worker *manager;
    struct list_head workers;
    struct list_head dying_workers;
    struct completion *detach_completion;
    struct ida worker_ida;
    struct workqueue_attrs *attrs;
    struct hlist_node hash_node;
    int refcnt;
    struct callback_head rcu;
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
struct worker_pool {
    spinlock_t lock;
    int cpu;
    int node;
    int id;
    unsigned int flags;
    long unsigned int watchdog_ts;
    struct list_head worklist;
    int nr_workers;
    int nr_idle;
    struct list_head idle_list;
    struct timer_list idle_timer;
    struct timer_list mayday_timer;
    struct hlist_head busy_hash[64];
    struct worker *manager;
    struct list_head workers;
    struct completion *detach_completion;
    struct ida worker_ida;
    struct workqueue_attrs *attrs;
    struct hlist_node hash_node;
    int refcnt;
    atomic_t nr_running;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct worker_pool {
    spinlock_t lock;
    int cpu;
    int node;
    int id;
    unsigned int flags;
    long unsigned int watchdog_ts;
    struct list_head worklist;
    int nr_workers;
    int nr_idle;
    struct list_head idle_list;
    struct timer_list idle_timer;
    struct timer_list mayday_timer;
    struct hlist_head busy_hash[64];
    struct worker *manager;
    struct list_head workers;
    struct completion *detach_completion;
    struct ida worker_ida;
    struct workqueue_attrs *attrs;
    struct hlist_node hash_node;
    int refcnt;
    atomic_t nr_running;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct worker_pool {
    spinlock_t lock;
    int cpu;
    int node;
    int id;
    unsigned int flags;
    long unsigned int watchdog_ts;
    struct list_head worklist;
    int nr_workers;
    int nr_idle;
    struct list_head idle_list;
    struct timer_list idle_timer;
    struct timer_list mayday_timer;
    struct hlist_head busy_hash[64];
    struct worker *manager;
    struct list_head workers;
    struct completion *detach_completion;
    struct ida worker_ida;
    struct workqueue_attrs *attrs;
    struct hlist_node hash_node;
    int refcnt;
    atomic_t nr_running;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct worker_pool {
    spinlock_t lock;
    int cpu;
    int node;
    int id;
    unsigned int flags;
    long unsigned int watchdog_ts;
    struct list_head worklist;
    int nr_workers;
    int nr_idle;
    struct list_head idle_list;
    struct timer_list idle_timer;
    struct timer_list mayday_timer;
    struct hlist_head busy_hash[64];
    struct worker *manager;
    struct list_head workers;
    struct completion *detach_completion;
    struct ida worker_ida;
    struct workqueue_attrs *attrs;
    struct hlist_node hash_node;
    int refcnt;
    atomic_t nr_running;
    struct callback_head rcu;
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
struct worker_pool {
    spinlock_t lock;
    int cpu;
    int node;
    int id;
    unsigned int flags;
    long unsigned int watchdog_ts;
    struct list_head worklist;
    int nr_workers;
    int nr_idle;
    struct list_head idle_list;
    struct timer_list idle_timer;
    struct timer_list mayday_timer;
    struct hlist_head busy_hash[64];
    struct worker *manager;
    struct list_head workers;
    struct completion *detach_completion;
    struct ida worker_ida;
    struct workqueue_attrs *attrs;
    struct hlist_node hash_node;
    int refcnt;
    atomic_t nr_running;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct worker_pool {
    spinlock_t lock;
    int cpu;
    int node;
    int id;
    unsigned int flags;
    long unsigned int watchdog_ts;
    struct list_head worklist;
    int nr_workers;
    int nr_idle;
    struct list_head idle_list;
    struct timer_list idle_timer;
    struct timer_list mayday_timer;
    struct hlist_head busy_hash[64];
    struct worker *manager;
    struct list_head workers;
    struct completion *detach_completion;
    struct ida worker_ida;
    struct workqueue_attrs *attrs;
    struct hlist_node hash_node;
    int refcnt;
    atomic_t nr_running;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct worker_pool {
    spinlock_t lock;
    int cpu;
    int node;
    int id;
    unsigned int flags;
    long unsigned int watchdog_ts;
    struct list_head worklist;
    int nr_workers;
    int nr_idle;
    struct list_head idle_list;
    struct timer_list idle_timer;
    struct timer_list mayday_timer;
    struct hlist_head busy_hash[64];
    struct worker *manager;
    struct list_head workers;
    struct completion *detach_completion;
    struct ida worker_ida;
    struct workqueue_attrs *attrs;
    struct hlist_node hash_node;
    int refcnt;
    atomic_t nr_running;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct worker_pool {
    spinlock_t lock;
    int cpu;
    int node;
    int id;
    unsigned int flags;
    long unsigned int watchdog_ts;
    struct list_head worklist;
    int nr_workers;
    int nr_idle;
    struct list_head idle_list;
    struct timer_list idle_timer;
    struct timer_list mayday_timer;
    struct hlist_head busy_hash[64];
    struct worker *manager;
    struct list_head workers;
    struct completion *detach_completion;
    struct ida worker_ida;
    struct workqueue_attrs *attrs;
    struct hlist_node hash_node;
    int refcnt;
    atomic_t nr_running;
    struct callback_head rcu;
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
<code>long unsigned int watchdog_ts</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct mutex manager_arb</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct mutex attach_mutex</code>
</li>
</ul>
</details>
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
<b>Field type changed. </b>
<code>spinlock_t lock</code> ➡️ <code>raw_spinlock_t lock</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>atomic_t nr_running</code> ➡️ <code>int nr_running</code>
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
<code>bool cpu_stall</code>
</li>
<li>
<b>Field added. </b>
<code>struct work_struct idle_cull_work</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head dying_workers</code>
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
