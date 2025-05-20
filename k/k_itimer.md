# Struct: <code>k_itimer</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct k_itimer {
    struct list_head list;
    struct hlist_node t_hash;
    spinlock_t it_lock;
    clockid_t it_clock;
    timer_t it_id;
    int it_overrun;
    int it_overrun_last;
    int it_requeue_pending;
    int it_sigev_notify;
    struct signal_struct *it_signal;
    struct pid *it_pid;
    struct task_struct *it_process;
    struct sigqueue *sigq;
    union (anon) it;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct k_itimer {
    struct list_head list;
    struct hlist_node t_hash;
    spinlock_t it_lock;
    clockid_t it_clock;
    timer_t it_id;
    int it_overrun;
    int it_overrun_last;
    int it_requeue_pending;
    int it_sigev_notify;
    struct signal_struct *it_signal;
    struct pid *it_pid;
    struct task_struct *it_process;
    struct sigqueue *sigq;
    union (anon) it;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct k_itimer {
    struct list_head list;
    struct hlist_node t_hash;
    spinlock_t it_lock;
    clockid_t it_clock;
    timer_t it_id;
    int it_overrun;
    int it_overrun_last;
    int it_requeue_pending;
    int it_sigev_notify;
    struct signal_struct *it_signal;
    struct pid *it_pid;
    struct task_struct *it_process;
    struct sigqueue *sigq;
    union (anon) it;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct k_itimer {
    struct list_head list;
    struct hlist_node t_hash;
    spinlock_t it_lock;
    const struct k_clock *kclock;
    clockid_t it_clock;
    timer_t it_id;
    int it_active;
    int it_overrun;
    int it_overrun_last;
    int it_requeue_pending;
    int it_sigev_notify;
    ktime_t it_interval;
    struct signal_struct *it_signal;
    struct pid *it_pid;
    struct task_struct *it_process;
    struct sigqueue *sigq;
    union (anon) it;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct k_itimer {
    struct list_head list;
    struct hlist_node t_hash;
    spinlock_t it_lock;
    const struct k_clock *kclock;
    clockid_t it_clock;
    timer_t it_id;
    int it_active;
    int it_overrun;
    int it_overrun_last;
    int it_requeue_pending;
    int it_sigev_notify;
    ktime_t it_interval;
    struct signal_struct *it_signal;
    struct pid *it_pid;
    struct task_struct *it_process;
    struct sigqueue *sigq;
    union (anon) it;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct k_itimer {
    struct list_head list;
    struct hlist_node t_hash;
    spinlock_t it_lock;
    const struct k_clock *kclock;
    clockid_t it_clock;
    timer_t it_id;
    int it_active;
    s64 it_overrun;
    s64 it_overrun_last;
    int it_requeue_pending;
    int it_sigev_notify;
    ktime_t it_interval;
    struct signal_struct *it_signal;
    struct pid *it_pid;
    struct task_struct *it_process;
    struct sigqueue *sigq;
    union (anon) it;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct k_itimer {
    struct list_head list;
    struct hlist_node t_hash;
    spinlock_t it_lock;
    const struct k_clock *kclock;
    clockid_t it_clock;
    timer_t it_id;
    int it_active;
    s64 it_overrun;
    s64 it_overrun_last;
    int it_requeue_pending;
    int it_sigev_notify;
    ktime_t it_interval;
    struct signal_struct *it_signal;
    struct pid *it_pid;
    struct task_struct *it_process;
    struct sigqueue *sigq;
    union (anon) it;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct k_itimer {
    struct list_head list;
    struct hlist_node t_hash;
    spinlock_t it_lock;
    const struct k_clock *kclock;
    clockid_t it_clock;
    timer_t it_id;
    int it_active;
    s64 it_overrun;
    s64 it_overrun_last;
    int it_requeue_pending;
    int it_sigev_notify;
    ktime_t it_interval;
    struct signal_struct *it_signal;
    struct pid *it_pid;
    struct task_struct *it_process;
    struct sigqueue *sigq;
    union (anon) it;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct k_itimer {
    struct list_head list;
    struct hlist_node t_hash;
    spinlock_t it_lock;
    const struct k_clock *kclock;
    clockid_t it_clock;
    timer_t it_id;
    int it_active;
    s64 it_overrun;
    s64 it_overrun_last;
    int it_requeue_pending;
    int it_sigev_notify;
    ktime_t it_interval;
    struct signal_struct *it_signal;
    struct pid *it_pid;
    struct task_struct *it_process;
    struct sigqueue *sigq;
    union (anon) it;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct k_itimer {
    struct list_head list;
    struct hlist_node t_hash;
    spinlock_t it_lock;
    const struct k_clock *kclock;
    clockid_t it_clock;
    timer_t it_id;
    int it_active;
    s64 it_overrun;
    s64 it_overrun_last;
    int it_requeue_pending;
    int it_sigev_notify;
    ktime_t it_interval;
    struct signal_struct *it_signal;
    struct pid *it_pid;
    struct task_struct *it_process;
    struct sigqueue *sigq;
    union (anon) it;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct k_itimer {
    struct list_head list;
    struct hlist_node t_hash;
    spinlock_t it_lock;
    const struct k_clock *kclock;
    clockid_t it_clock;
    timer_t it_id;
    int it_active;
    s64 it_overrun;
    s64 it_overrun_last;
    int it_requeue_pending;
    int it_sigev_notify;
    ktime_t it_interval;
    struct signal_struct *it_signal;
    struct pid *it_pid;
    struct task_struct *it_process;
    struct sigqueue *sigq;
    union (anon) it;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct k_itimer {
    struct list_head list;
    struct hlist_node t_hash;
    spinlock_t it_lock;
    const struct k_clock *kclock;
    clockid_t it_clock;
    timer_t it_id;
    int it_active;
    s64 it_overrun;
    s64 it_overrun_last;
    int it_requeue_pending;
    int it_sigev_notify;
    ktime_t it_interval;
    struct signal_struct *it_signal;
    struct pid *it_pid;
    struct task_struct *it_process;
    struct sigqueue *sigq;
    union (anon) it;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct k_itimer {
    struct list_head list;
    struct hlist_node t_hash;
    spinlock_t it_lock;
    const struct k_clock *kclock;
    clockid_t it_clock;
    timer_t it_id;
    int it_active;
    s64 it_overrun;
    s64 it_overrun_last;
    int it_requeue_pending;
    int it_sigev_notify;
    ktime_t it_interval;
    struct signal_struct *it_signal;
    struct pid *it_pid;
    struct task_struct *it_process;
    struct sigqueue *sigq;
    union (anon) it;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct k_itimer {
    struct list_head list;
    struct hlist_node t_hash;
    spinlock_t it_lock;
    const struct k_clock *kclock;
    clockid_t it_clock;
    timer_t it_id;
    int it_active;
    s64 it_overrun;
    s64 it_overrun_last;
    int it_requeue_pending;
    int it_sigev_notify;
    ktime_t it_interval;
    struct signal_struct *it_signal;
    struct pid *it_pid;
    struct task_struct *it_process;
    struct sigqueue *sigq;
    union (anon) it;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct k_itimer {
    struct list_head list;
    struct hlist_node t_hash;
    spinlock_t it_lock;
    const struct k_clock *kclock;
    clockid_t it_clock;
    timer_t it_id;
    int it_active;
    s64 it_overrun;
    s64 it_overrun_last;
    int it_requeue_pending;
    int it_sigev_notify;
    ktime_t it_interval;
    struct signal_struct *it_signal;
    struct pid *it_pid;
    struct task_struct *it_process;
    struct sigqueue *sigq;
    union (anon) it;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct k_itimer {
    struct list_head list;
    struct hlist_node t_hash;
    spinlock_t it_lock;
    const struct k_clock *kclock;
    clockid_t it_clock;
    timer_t it_id;
    int it_active;
    s64 it_overrun;
    s64 it_overrun_last;
    int it_requeue_pending;
    int it_sigev_notify;
    ktime_t it_interval;
    struct signal_struct *it_signal;
    struct pid *it_pid;
    struct task_struct *it_process;
    struct sigqueue *sigq;
    union (anon) it;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct k_itimer {
    struct list_head list;
    struct hlist_node t_hash;
    spinlock_t it_lock;
    const struct k_clock *kclock;
    clockid_t it_clock;
    timer_t it_id;
    int it_active;
    s64 it_overrun;
    s64 it_overrun_last;
    int it_requeue_pending;
    int it_sigev_notify;
    ktime_t it_interval;
    struct signal_struct *it_signal;
    struct pid *it_pid;
    struct task_struct *it_process;
    struct sigqueue *sigq;
    union (anon) it;
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
struct k_itimer {
    struct list_head list;
    struct hlist_node t_hash;
    spinlock_t it_lock;
    const struct k_clock *kclock;
    clockid_t it_clock;
    timer_t it_id;
    int it_active;
    s64 it_overrun;
    s64 it_overrun_last;
    int it_requeue_pending;
    int it_sigev_notify;
    ktime_t it_interval;
    struct signal_struct *it_signal;
    struct pid *it_pid;
    struct task_struct *it_process;
    struct sigqueue *sigq;
    union (anon) it;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct k_itimer {
    struct list_head list;
    struct hlist_node t_hash;
    spinlock_t it_lock;
    const struct k_clock *kclock;
    clockid_t it_clock;
    timer_t it_id;
    int it_active;
    s64 it_overrun;
    s64 it_overrun_last;
    int it_requeue_pending;
    int it_sigev_notify;
    ktime_t it_interval;
    struct signal_struct *it_signal;
    struct pid *it_pid;
    struct task_struct *it_process;
    struct sigqueue *sigq;
    union (anon) it;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct k_itimer {
    struct list_head list;
    struct hlist_node t_hash;
    spinlock_t it_lock;
    const struct k_clock *kclock;
    clockid_t it_clock;
    timer_t it_id;
    int it_active;
    s64 it_overrun;
    s64 it_overrun_last;
    int it_requeue_pending;
    int it_sigev_notify;
    ktime_t it_interval;
    struct signal_struct *it_signal;
    struct pid *it_pid;
    struct task_struct *it_process;
    struct sigqueue *sigq;
    union (anon) it;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct k_itimer {
    struct list_head list;
    struct hlist_node t_hash;
    spinlock_t it_lock;
    const struct k_clock *kclock;
    clockid_t it_clock;
    timer_t it_id;
    int it_active;
    s64 it_overrun;
    s64 it_overrun_last;
    int it_requeue_pending;
    int it_sigev_notify;
    ktime_t it_interval;
    struct signal_struct *it_signal;
    struct pid *it_pid;
    struct task_struct *it_process;
    struct sigqueue *sigq;
    union (anon) it;
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
struct k_itimer {
    struct list_head list;
    struct hlist_node t_hash;
    spinlock_t it_lock;
    const struct k_clock *kclock;
    clockid_t it_clock;
    timer_t it_id;
    int it_active;
    s64 it_overrun;
    s64 it_overrun_last;
    int it_requeue_pending;
    int it_sigev_notify;
    ktime_t it_interval;
    struct signal_struct *it_signal;
    struct pid *it_pid;
    struct task_struct *it_process;
    struct sigqueue *sigq;
    union (anon) it;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct k_itimer {
    struct list_head list;
    struct hlist_node t_hash;
    spinlock_t it_lock;
    const struct k_clock *kclock;
    clockid_t it_clock;
    timer_t it_id;
    int it_active;
    s64 it_overrun;
    s64 it_overrun_last;
    int it_requeue_pending;
    int it_sigev_notify;
    ktime_t it_interval;
    struct signal_struct *it_signal;
    struct pid *it_pid;
    struct task_struct *it_process;
    struct sigqueue *sigq;
    union (anon) it;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct k_itimer {
    struct list_head list;
    struct hlist_node t_hash;
    spinlock_t it_lock;
    const struct k_clock *kclock;
    clockid_t it_clock;
    timer_t it_id;
    int it_active;
    s64 it_overrun;
    s64 it_overrun_last;
    int it_requeue_pending;
    int it_sigev_notify;
    ktime_t it_interval;
    struct signal_struct *it_signal;
    struct pid *it_pid;
    struct task_struct *it_process;
    struct sigqueue *sigq;
    union (anon) it;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct k_itimer {
    struct list_head list;
    struct hlist_node t_hash;
    spinlock_t it_lock;
    const struct k_clock *kclock;
    clockid_t it_clock;
    timer_t it_id;
    int it_active;
    s64 it_overrun;
    s64 it_overrun_last;
    int it_requeue_pending;
    int it_sigev_notify;
    ktime_t it_interval;
    struct signal_struct *it_signal;
    struct pid *it_pid;
    struct task_struct *it_process;
    struct sigqueue *sigq;
    union (anon) it;
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
<code>const struct k_clock *kclock</code>
</li>
<li>
<b>Field added. </b>
<code>int it_active</code>
</li>
<li>
<b>Field added. </b>
<code>ktime_t it_interval</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int it_overrun</code> ➡️ <code>s64 it_overrun</code>
</li>
<li>
<b>Field type changed. </b>
<code>int it_overrun_last</code> ➡️ <code>s64 it_overrun_last</code>
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
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct callback_head rcu</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
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
