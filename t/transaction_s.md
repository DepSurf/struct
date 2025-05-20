# Struct: <code>transaction_s</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct transaction_s {
    journal_t *t_journal;
    tid_t t_tid;
    enum (anon) t_state;
    long unsigned int t_log_start;
    int t_nr_buffers;
    struct journal_head *t_reserved_list;
    struct journal_head *t_buffers;
    struct journal_head *t_forget;
    struct journal_head *t_checkpoint_list;
    struct journal_head *t_checkpoint_io_list;
    struct journal_head *t_shadow_list;
    struct list_head t_inode_list;
    spinlock_t t_handle_lock;
    long unsigned int t_max_wait;
    long unsigned int t_start;
    long unsigned int t_requested;
    struct transaction_chp_stats_s t_chp_stats;
    atomic_t t_updates;
    atomic_t t_outstanding_credits;
    transaction_t *t_cpnext;
    transaction_t *t_cpprev;
    long unsigned int t_expires;
    ktime_t t_start_time;
    atomic_t t_handle_count;
    unsigned int t_synchronous_commit;
    int t_need_data_flush;
    struct list_head t_private_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct transaction_s {
    journal_t *t_journal;
    tid_t t_tid;
    enum (anon) t_state;
    long unsigned int t_log_start;
    int t_nr_buffers;
    struct journal_head *t_reserved_list;
    struct journal_head *t_buffers;
    struct journal_head *t_forget;
    struct journal_head *t_checkpoint_list;
    struct journal_head *t_checkpoint_io_list;
    struct journal_head *t_shadow_list;
    struct list_head t_inode_list;
    spinlock_t t_handle_lock;
    long unsigned int t_max_wait;
    long unsigned int t_start;
    long unsigned int t_requested;
    struct transaction_chp_stats_s t_chp_stats;
    atomic_t t_updates;
    atomic_t t_outstanding_credits;
    transaction_t *t_cpnext;
    transaction_t *t_cpprev;
    long unsigned int t_expires;
    ktime_t t_start_time;
    atomic_t t_handle_count;
    unsigned int t_synchronous_commit;
    int t_need_data_flush;
    struct list_head t_private_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct transaction_s {
    journal_t *t_journal;
    tid_t t_tid;
    enum (anon) t_state;
    long unsigned int t_log_start;
    int t_nr_buffers;
    struct journal_head *t_reserved_list;
    struct journal_head *t_buffers;
    struct journal_head *t_forget;
    struct journal_head *t_checkpoint_list;
    struct journal_head *t_checkpoint_io_list;
    struct journal_head *t_shadow_list;
    struct list_head t_inode_list;
    spinlock_t t_handle_lock;
    long unsigned int t_max_wait;
    long unsigned int t_start;
    long unsigned int t_requested;
    struct transaction_chp_stats_s t_chp_stats;
    atomic_t t_updates;
    atomic_t t_outstanding_credits;
    transaction_t *t_cpnext;
    transaction_t *t_cpprev;
    long unsigned int t_expires;
    ktime_t t_start_time;
    atomic_t t_handle_count;
    unsigned int t_synchronous_commit;
    int t_need_data_flush;
    struct list_head t_private_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct transaction_s {
    journal_t *t_journal;
    tid_t t_tid;
    enum (anon) t_state;
    long unsigned int t_log_start;
    int t_nr_buffers;
    struct journal_head *t_reserved_list;
    struct journal_head *t_buffers;
    struct journal_head *t_forget;
    struct journal_head *t_checkpoint_list;
    struct journal_head *t_checkpoint_io_list;
    struct journal_head *t_shadow_list;
    struct list_head t_inode_list;
    spinlock_t t_handle_lock;
    long unsigned int t_max_wait;
    long unsigned int t_start;
    long unsigned int t_requested;
    struct transaction_chp_stats_s t_chp_stats;
    atomic_t t_updates;
    atomic_t t_outstanding_credits;
    transaction_t *t_cpnext;
    transaction_t *t_cpprev;
    long unsigned int t_expires;
    ktime_t t_start_time;
    atomic_t t_handle_count;
    unsigned int t_synchronous_commit;
    int t_need_data_flush;
    struct list_head t_private_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct transaction_s {
    journal_t *t_journal;
    tid_t t_tid;
    enum (anon) t_state;
    long unsigned int t_log_start;
    int t_nr_buffers;
    struct journal_head *t_reserved_list;
    struct journal_head *t_buffers;
    struct journal_head *t_forget;
    struct journal_head *t_checkpoint_list;
    struct journal_head *t_checkpoint_io_list;
    struct journal_head *t_shadow_list;
    struct list_head t_inode_list;
    spinlock_t t_handle_lock;
    long unsigned int t_max_wait;
    long unsigned int t_start;
    long unsigned int t_requested;
    struct transaction_chp_stats_s t_chp_stats;
    atomic_t t_updates;
    atomic_t t_outstanding_credits;
    transaction_t *t_cpnext;
    transaction_t *t_cpprev;
    long unsigned int t_expires;
    ktime_t t_start_time;
    atomic_t t_handle_count;
    unsigned int t_synchronous_commit;
    int t_need_data_flush;
    struct list_head t_private_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct transaction_s {
    journal_t *t_journal;
    tid_t t_tid;
    enum (anon) t_state;
    long unsigned int t_log_start;
    int t_nr_buffers;
    struct journal_head *t_reserved_list;
    struct journal_head *t_buffers;
    struct journal_head *t_forget;
    struct journal_head *t_checkpoint_list;
    struct journal_head *t_checkpoint_io_list;
    struct journal_head *t_shadow_list;
    struct list_head t_inode_list;
    spinlock_t t_handle_lock;
    long unsigned int t_max_wait;
    long unsigned int t_start;
    long unsigned int t_requested;
    struct transaction_chp_stats_s t_chp_stats;
    atomic_t t_updates;
    atomic_t t_outstanding_credits;
    transaction_t *t_cpnext;
    transaction_t *t_cpprev;
    long unsigned int t_expires;
    ktime_t t_start_time;
    atomic_t t_handle_count;
    unsigned int t_synchronous_commit;
    int t_need_data_flush;
    struct list_head t_private_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct transaction_s {
    journal_t *t_journal;
    tid_t t_tid;
    enum (anon) t_state;
    long unsigned int t_log_start;
    int t_nr_buffers;
    struct journal_head *t_reserved_list;
    struct journal_head *t_buffers;
    struct journal_head *t_forget;
    struct journal_head *t_checkpoint_list;
    struct journal_head *t_checkpoint_io_list;
    struct journal_head *t_shadow_list;
    struct list_head t_inode_list;
    spinlock_t t_handle_lock;
    long unsigned int t_max_wait;
    long unsigned int t_start;
    long unsigned int t_requested;
    struct transaction_chp_stats_s t_chp_stats;
    atomic_t t_updates;
    atomic_t t_outstanding_credits;
    transaction_t *t_cpnext;
    transaction_t *t_cpprev;
    long unsigned int t_expires;
    ktime_t t_start_time;
    atomic_t t_handle_count;
    unsigned int t_synchronous_commit;
    int t_need_data_flush;
    struct list_head t_private_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct transaction_s {
    journal_t *t_journal;
    tid_t t_tid;
    enum (anon) t_state;
    long unsigned int t_log_start;
    int t_nr_buffers;
    struct journal_head *t_reserved_list;
    struct journal_head *t_buffers;
    struct journal_head *t_forget;
    struct journal_head *t_checkpoint_list;
    struct journal_head *t_checkpoint_io_list;
    struct journal_head *t_shadow_list;
    struct list_head t_inode_list;
    spinlock_t t_handle_lock;
    long unsigned int t_max_wait;
    long unsigned int t_start;
    long unsigned int t_requested;
    struct transaction_chp_stats_s t_chp_stats;
    atomic_t t_updates;
    atomic_t t_outstanding_credits;
    transaction_t *t_cpnext;
    transaction_t *t_cpprev;
    long unsigned int t_expires;
    ktime_t t_start_time;
    atomic_t t_handle_count;
    unsigned int t_synchronous_commit;
    int t_need_data_flush;
    struct list_head t_private_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct transaction_s {
    journal_t *t_journal;
    tid_t t_tid;
    enum (anon) t_state;
    long unsigned int t_log_start;
    int t_nr_buffers;
    struct journal_head *t_reserved_list;
    struct journal_head *t_buffers;
    struct journal_head *t_forget;
    struct journal_head *t_checkpoint_list;
    struct journal_head *t_checkpoint_io_list;
    struct journal_head *t_shadow_list;
    struct list_head t_inode_list;
    spinlock_t t_handle_lock;
    long unsigned int t_max_wait;
    long unsigned int t_start;
    long unsigned int t_requested;
    struct transaction_chp_stats_s t_chp_stats;
    atomic_t t_updates;
    atomic_t t_outstanding_credits;
    transaction_t *t_cpnext;
    transaction_t *t_cpprev;
    long unsigned int t_expires;
    ktime_t t_start_time;
    atomic_t t_handle_count;
    unsigned int t_synchronous_commit;
    int t_need_data_flush;
    struct list_head t_private_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct transaction_s {
    journal_t *t_journal;
    tid_t t_tid;
    enum (anon) t_state;
    long unsigned int t_log_start;
    int t_nr_buffers;
    struct journal_head *t_reserved_list;
    struct journal_head *t_buffers;
    struct journal_head *t_forget;
    struct journal_head *t_checkpoint_list;
    struct journal_head *t_checkpoint_io_list;
    struct journal_head *t_shadow_list;
    struct list_head t_inode_list;
    spinlock_t t_handle_lock;
    long unsigned int t_max_wait;
    long unsigned int t_start;
    long unsigned int t_requested;
    struct transaction_chp_stats_s t_chp_stats;
    atomic_t t_updates;
    atomic_t t_outstanding_credits;
    atomic_t t_outstanding_revokes;
    atomic_t t_handle_count;
    transaction_t *t_cpnext;
    transaction_t *t_cpprev;
    long unsigned int t_expires;
    ktime_t t_start_time;
    unsigned int t_synchronous_commit;
    int t_need_data_flush;
    struct list_head t_private_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct transaction_s {
    journal_t *t_journal;
    tid_t t_tid;
    enum (anon) t_state;
    long unsigned int t_log_start;
    int t_nr_buffers;
    struct journal_head *t_reserved_list;
    struct journal_head *t_buffers;
    struct journal_head *t_forget;
    struct journal_head *t_checkpoint_list;
    struct journal_head *t_checkpoint_io_list;
    struct journal_head *t_shadow_list;
    struct list_head t_inode_list;
    spinlock_t t_handle_lock;
    long unsigned int t_max_wait;
    long unsigned int t_start;
    long unsigned int t_requested;
    struct transaction_chp_stats_s t_chp_stats;
    atomic_t t_updates;
    atomic_t t_outstanding_credits;
    atomic_t t_outstanding_revokes;
    atomic_t t_handle_count;
    transaction_t *t_cpnext;
    transaction_t *t_cpprev;
    long unsigned int t_expires;
    ktime_t t_start_time;
    unsigned int t_synchronous_commit;
    int t_need_data_flush;
    struct list_head t_private_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct transaction_s {
    journal_t *t_journal;
    tid_t t_tid;
    enum (anon) t_state;
    long unsigned int t_log_start;
    int t_nr_buffers;
    struct journal_head *t_reserved_list;
    struct journal_head *t_buffers;
    struct journal_head *t_forget;
    struct journal_head *t_checkpoint_list;
    struct journal_head *t_checkpoint_io_list;
    struct journal_head *t_shadow_list;
    struct list_head t_inode_list;
    spinlock_t t_handle_lock;
    long unsigned int t_max_wait;
    long unsigned int t_start;
    long unsigned int t_requested;
    struct transaction_chp_stats_s t_chp_stats;
    atomic_t t_updates;
    atomic_t t_outstanding_credits;
    atomic_t t_outstanding_revokes;
    atomic_t t_handle_count;
    transaction_t *t_cpnext;
    transaction_t *t_cpprev;
    long unsigned int t_expires;
    ktime_t t_start_time;
    unsigned int t_synchronous_commit;
    int t_need_data_flush;
    struct list_head t_private_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct transaction_s {
    journal_t *t_journal;
    tid_t t_tid;
    enum (anon) t_state;
    long unsigned int t_log_start;
    int t_nr_buffers;
    struct journal_head *t_reserved_list;
    struct journal_head *t_buffers;
    struct journal_head *t_forget;
    struct journal_head *t_checkpoint_list;
    struct journal_head *t_checkpoint_io_list;
    struct journal_head *t_shadow_list;
    struct list_head t_inode_list;
    spinlock_t t_handle_lock;
    long unsigned int t_max_wait;
    long unsigned int t_start;
    long unsigned int t_requested;
    struct transaction_chp_stats_s t_chp_stats;
    atomic_t t_updates;
    atomic_t t_outstanding_credits;
    atomic_t t_outstanding_revokes;
    atomic_t t_handle_count;
    transaction_t *t_cpnext;
    transaction_t *t_cpprev;
    long unsigned int t_expires;
    ktime_t t_start_time;
    unsigned int t_synchronous_commit;
    int t_need_data_flush;
    struct list_head t_private_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct transaction_s {
    journal_t *t_journal;
    tid_t t_tid;
    enum (anon) t_state;
    long unsigned int t_log_start;
    int t_nr_buffers;
    struct journal_head *t_reserved_list;
    struct journal_head *t_buffers;
    struct journal_head *t_forget;
    struct journal_head *t_checkpoint_list;
    struct journal_head *t_checkpoint_io_list;
    struct journal_head *t_shadow_list;
    struct list_head t_inode_list;
    spinlock_t t_handle_lock;
    long unsigned int t_max_wait;
    long unsigned int t_start;
    long unsigned int t_requested;
    struct transaction_chp_stats_s t_chp_stats;
    atomic_t t_updates;
    atomic_t t_outstanding_credits;
    atomic_t t_outstanding_revokes;
    atomic_t t_handle_count;
    transaction_t *t_cpnext;
    transaction_t *t_cpprev;
    long unsigned int t_expires;
    ktime_t t_start_time;
    unsigned int t_synchronous_commit;
    int t_need_data_flush;
    struct list_head t_private_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct transaction_s {
    journal_t *t_journal;
    tid_t t_tid;
    enum (anon) t_state;
    long unsigned int t_log_start;
    int t_nr_buffers;
    struct journal_head *t_reserved_list;
    struct journal_head *t_buffers;
    struct journal_head *t_forget;
    struct journal_head *t_checkpoint_list;
    struct journal_head *t_checkpoint_io_list;
    struct journal_head *t_shadow_list;
    struct list_head t_inode_list;
    spinlock_t t_handle_lock;
    long unsigned int t_max_wait;
    long unsigned int t_start;
    long unsigned int t_requested;
    struct transaction_chp_stats_s t_chp_stats;
    atomic_t t_updates;
    atomic_t t_outstanding_credits;
    atomic_t t_outstanding_revokes;
    atomic_t t_handle_count;
    transaction_t *t_cpnext;
    transaction_t *t_cpprev;
    long unsigned int t_expires;
    ktime_t t_start_time;
    unsigned int t_synchronous_commit;
    int t_need_data_flush;
    struct list_head t_private_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct transaction_s {
    journal_t *t_journal;
    tid_t t_tid;
    enum (anon) t_state;
    long unsigned int t_log_start;
    int t_nr_buffers;
    struct journal_head *t_reserved_list;
    struct journal_head *t_buffers;
    struct journal_head *t_forget;
    struct journal_head *t_checkpoint_list;
    struct journal_head *t_shadow_list;
    struct list_head t_inode_list;
    spinlock_t t_handle_lock;
    long unsigned int t_max_wait;
    long unsigned int t_start;
    long unsigned int t_requested;
    struct transaction_chp_stats_s t_chp_stats;
    atomic_t t_updates;
    atomic_t t_outstanding_credits;
    atomic_t t_outstanding_revokes;
    atomic_t t_handle_count;
    transaction_t *t_cpnext;
    transaction_t *t_cpprev;
    long unsigned int t_expires;
    ktime_t t_start_time;
    unsigned int t_synchronous_commit;
    int t_need_data_flush;
    struct list_head t_private_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct transaction_s {
    journal_t *t_journal;
    tid_t t_tid;
    enum (anon) t_state;
    long unsigned int t_log_start;
    int t_nr_buffers;
    struct journal_head *t_reserved_list;
    struct journal_head *t_buffers;
    struct journal_head *t_forget;
    struct journal_head *t_checkpoint_list;
    struct journal_head *t_shadow_list;
    struct list_head t_inode_list;
    long unsigned int t_max_wait;
    long unsigned int t_start;
    long unsigned int t_requested;
    struct transaction_chp_stats_s t_chp_stats;
    atomic_t t_updates;
    atomic_t t_outstanding_credits;
    atomic_t t_outstanding_revokes;
    atomic_t t_handle_count;
    transaction_t *t_cpnext;
    transaction_t *t_cpprev;
    long unsigned int t_expires;
    ktime_t t_start_time;
    unsigned int t_synchronous_commit;
    int t_need_data_flush;
    struct list_head t_private_list;
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
struct transaction_s {
    journal_t *t_journal;
    tid_t t_tid;
    enum (anon) t_state;
    long unsigned int t_log_start;
    int t_nr_buffers;
    struct journal_head *t_reserved_list;
    struct journal_head *t_buffers;
    struct journal_head *t_forget;
    struct journal_head *t_checkpoint_list;
    struct journal_head *t_checkpoint_io_list;
    struct journal_head *t_shadow_list;
    struct list_head t_inode_list;
    spinlock_t t_handle_lock;
    long unsigned int t_max_wait;
    long unsigned int t_start;
    long unsigned int t_requested;
    struct transaction_chp_stats_s t_chp_stats;
    atomic_t t_updates;
    atomic_t t_outstanding_credits;
    transaction_t *t_cpnext;
    transaction_t *t_cpprev;
    long unsigned int t_expires;
    ktime_t t_start_time;
    atomic_t t_handle_count;
    unsigned int t_synchronous_commit;
    int t_need_data_flush;
    struct list_head t_private_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct transaction_s {
    journal_t *t_journal;
    tid_t t_tid;
    enum (anon) t_state;
    long unsigned int t_log_start;
    int t_nr_buffers;
    struct journal_head *t_reserved_list;
    struct journal_head *t_buffers;
    struct journal_head *t_forget;
    struct journal_head *t_checkpoint_list;
    struct journal_head *t_checkpoint_io_list;
    struct journal_head *t_shadow_list;
    struct list_head t_inode_list;
    spinlock_t t_handle_lock;
    long unsigned int t_max_wait;
    long unsigned int t_start;
    long unsigned int t_requested;
    struct transaction_chp_stats_s t_chp_stats;
    atomic_t t_updates;
    atomic_t t_outstanding_credits;
    transaction_t *t_cpnext;
    transaction_t *t_cpprev;
    long unsigned int t_expires;
    ktime_t t_start_time;
    atomic_t t_handle_count;
    unsigned int t_synchronous_commit;
    int t_need_data_flush;
    struct list_head t_private_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct transaction_s {
    journal_t *t_journal;
    tid_t t_tid;
    enum (anon) t_state;
    long unsigned int t_log_start;
    int t_nr_buffers;
    struct journal_head *t_reserved_list;
    struct journal_head *t_buffers;
    struct journal_head *t_forget;
    struct journal_head *t_checkpoint_list;
    struct journal_head *t_checkpoint_io_list;
    struct journal_head *t_shadow_list;
    struct list_head t_inode_list;
    spinlock_t t_handle_lock;
    long unsigned int t_max_wait;
    long unsigned int t_start;
    long unsigned int t_requested;
    struct transaction_chp_stats_s t_chp_stats;
    atomic_t t_updates;
    atomic_t t_outstanding_credits;
    transaction_t *t_cpnext;
    transaction_t *t_cpprev;
    long unsigned int t_expires;
    ktime_t t_start_time;
    atomic_t t_handle_count;
    unsigned int t_synchronous_commit;
    int t_need_data_flush;
    struct list_head t_private_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct transaction_s {
    journal_t *t_journal;
    tid_t t_tid;
    enum (anon) t_state;
    long unsigned int t_log_start;
    int t_nr_buffers;
    struct journal_head *t_reserved_list;
    struct journal_head *t_buffers;
    struct journal_head *t_forget;
    struct journal_head *t_checkpoint_list;
    struct journal_head *t_checkpoint_io_list;
    struct journal_head *t_shadow_list;
    struct list_head t_inode_list;
    spinlock_t t_handle_lock;
    long unsigned int t_max_wait;
    long unsigned int t_start;
    long unsigned int t_requested;
    struct transaction_chp_stats_s t_chp_stats;
    atomic_t t_updates;
    atomic_t t_outstanding_credits;
    transaction_t *t_cpnext;
    transaction_t *t_cpprev;
    long unsigned int t_expires;
    ktime_t t_start_time;
    atomic_t t_handle_count;
    unsigned int t_synchronous_commit;
    int t_need_data_flush;
    struct list_head t_private_list;
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
struct transaction_s {
    journal_t *t_journal;
    tid_t t_tid;
    enum (anon) t_state;
    long unsigned int t_log_start;
    int t_nr_buffers;
    struct journal_head *t_reserved_list;
    struct journal_head *t_buffers;
    struct journal_head *t_forget;
    struct journal_head *t_checkpoint_list;
    struct journal_head *t_checkpoint_io_list;
    struct journal_head *t_shadow_list;
    struct list_head t_inode_list;
    spinlock_t t_handle_lock;
    long unsigned int t_max_wait;
    long unsigned int t_start;
    long unsigned int t_requested;
    struct transaction_chp_stats_s t_chp_stats;
    atomic_t t_updates;
    atomic_t t_outstanding_credits;
    transaction_t *t_cpnext;
    transaction_t *t_cpprev;
    long unsigned int t_expires;
    ktime_t t_start_time;
    atomic_t t_handle_count;
    unsigned int t_synchronous_commit;
    int t_need_data_flush;
    struct list_head t_private_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct transaction_s {
    journal_t *t_journal;
    tid_t t_tid;
    enum (anon) t_state;
    long unsigned int t_log_start;
    int t_nr_buffers;
    struct journal_head *t_reserved_list;
    struct journal_head *t_buffers;
    struct journal_head *t_forget;
    struct journal_head *t_checkpoint_list;
    struct journal_head *t_checkpoint_io_list;
    struct journal_head *t_shadow_list;
    struct list_head t_inode_list;
    spinlock_t t_handle_lock;
    long unsigned int t_max_wait;
    long unsigned int t_start;
    long unsigned int t_requested;
    struct transaction_chp_stats_s t_chp_stats;
    atomic_t t_updates;
    atomic_t t_outstanding_credits;
    transaction_t *t_cpnext;
    transaction_t *t_cpprev;
    long unsigned int t_expires;
    ktime_t t_start_time;
    atomic_t t_handle_count;
    unsigned int t_synchronous_commit;
    int t_need_data_flush;
    struct list_head t_private_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct transaction_s {
    journal_t *t_journal;
    tid_t t_tid;
    enum (anon) t_state;
    long unsigned int t_log_start;
    int t_nr_buffers;
    struct journal_head *t_reserved_list;
    struct journal_head *t_buffers;
    struct journal_head *t_forget;
    struct journal_head *t_checkpoint_list;
    struct journal_head *t_checkpoint_io_list;
    struct journal_head *t_shadow_list;
    struct list_head t_inode_list;
    spinlock_t t_handle_lock;
    long unsigned int t_max_wait;
    long unsigned int t_start;
    long unsigned int t_requested;
    struct transaction_chp_stats_s t_chp_stats;
    atomic_t t_updates;
    atomic_t t_outstanding_credits;
    transaction_t *t_cpnext;
    transaction_t *t_cpprev;
    long unsigned int t_expires;
    ktime_t t_start_time;
    atomic_t t_handle_count;
    unsigned int t_synchronous_commit;
    int t_need_data_flush;
    struct list_head t_private_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct transaction_s {
    journal_t *t_journal;
    tid_t t_tid;
    enum (anon) t_state;
    long unsigned int t_log_start;
    int t_nr_buffers;
    struct journal_head *t_reserved_list;
    struct journal_head *t_buffers;
    struct journal_head *t_forget;
    struct journal_head *t_checkpoint_list;
    struct journal_head *t_checkpoint_io_list;
    struct journal_head *t_shadow_list;
    struct list_head t_inode_list;
    spinlock_t t_handle_lock;
    long unsigned int t_max_wait;
    long unsigned int t_start;
    long unsigned int t_requested;
    struct transaction_chp_stats_s t_chp_stats;
    atomic_t t_updates;
    atomic_t t_outstanding_credits;
    transaction_t *t_cpnext;
    transaction_t *t_cpprev;
    long unsigned int t_expires;
    ktime_t t_start_time;
    atomic_t t_handle_count;
    unsigned int t_synchronous_commit;
    int t_need_data_flush;
    struct list_head t_private_list;
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
<code>atomic_t t_outstanding_revokes</code>
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
<b>Field removed. </b>
<code>struct journal_head *t_checkpoint_io_list</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>spinlock_t t_handle_lock</code>
</li>
</ul>
</details>
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
