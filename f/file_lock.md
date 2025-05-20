# Struct: <code>file_lock</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct file_lock {
    struct file_lock *fl_next;
    struct list_head fl_list;
    struct hlist_node fl_link;
    struct list_head fl_block;
    fl_owner_t fl_owner;
    unsigned int fl_flags;
    unsigned char fl_type;
    unsigned int fl_pid;
    int fl_link_cpu;
    struct pid *fl_nspid;
    wait_queue_head_t fl_wait;
    struct file *fl_file;
    loff_t fl_start;
    loff_t fl_end;
    struct fasync_struct *fl_fasync;
    long unsigned int fl_break_time;
    long unsigned int fl_downgrade_time;
    const struct file_lock_operations *fl_ops;
    const struct lock_manager_operations *fl_lmops;
    union (anon) fl_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct file_lock {
    struct file_lock *fl_next;
    struct list_head fl_list;
    struct hlist_node fl_link;
    struct list_head fl_block;
    fl_owner_t fl_owner;
    unsigned int fl_flags;
    unsigned char fl_type;
    unsigned int fl_pid;
    int fl_link_cpu;
    struct pid *fl_nspid;
    wait_queue_head_t fl_wait;
    struct file *fl_file;
    loff_t fl_start;
    loff_t fl_end;
    struct fasync_struct *fl_fasync;
    long unsigned int fl_break_time;
    long unsigned int fl_downgrade_time;
    const struct file_lock_operations *fl_ops;
    const struct lock_manager_operations *fl_lmops;
    union (anon) fl_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct file_lock {
    struct file_lock *fl_next;
    struct list_head fl_list;
    struct hlist_node fl_link;
    struct list_head fl_block;
    fl_owner_t fl_owner;
    unsigned int fl_flags;
    unsigned char fl_type;
    unsigned int fl_pid;
    int fl_link_cpu;
    struct pid *fl_nspid;
    wait_queue_head_t fl_wait;
    struct file *fl_file;
    loff_t fl_start;
    loff_t fl_end;
    struct fasync_struct *fl_fasync;
    long unsigned int fl_break_time;
    long unsigned int fl_downgrade_time;
    const struct file_lock_operations *fl_ops;
    const struct lock_manager_operations *fl_lmops;
    union (anon) fl_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct file_lock {
    struct file_lock *fl_next;
    struct list_head fl_list;
    struct hlist_node fl_link;
    struct list_head fl_block;
    fl_owner_t fl_owner;
    unsigned int fl_flags;
    unsigned char fl_type;
    unsigned int fl_pid;
    int fl_link_cpu;
    struct pid *fl_nspid;
    wait_queue_head_t fl_wait;
    struct file *fl_file;
    loff_t fl_start;
    loff_t fl_end;
    struct fasync_struct *fl_fasync;
    long unsigned int fl_break_time;
    long unsigned int fl_downgrade_time;
    const struct file_lock_operations *fl_ops;
    const struct lock_manager_operations *fl_lmops;
    union (anon) fl_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct file_lock {
    struct file_lock *fl_next;
    struct list_head fl_list;
    struct hlist_node fl_link;
    struct list_head fl_block;
    fl_owner_t fl_owner;
    unsigned int fl_flags;
    unsigned char fl_type;
    unsigned int fl_pid;
    int fl_link_cpu;
    wait_queue_head_t fl_wait;
    struct file *fl_file;
    loff_t fl_start;
    loff_t fl_end;
    struct fasync_struct *fl_fasync;
    long unsigned int fl_break_time;
    long unsigned int fl_downgrade_time;
    const struct file_lock_operations *fl_ops;
    const struct lock_manager_operations *fl_lmops;
    union (anon) fl_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct file_lock {
    struct file_lock *fl_next;
    struct list_head fl_list;
    struct hlist_node fl_link;
    struct list_head fl_block;
    fl_owner_t fl_owner;
    unsigned int fl_flags;
    unsigned char fl_type;
    unsigned int fl_pid;
    int fl_link_cpu;
    wait_queue_head_t fl_wait;
    struct file *fl_file;
    loff_t fl_start;
    loff_t fl_end;
    struct fasync_struct *fl_fasync;
    long unsigned int fl_break_time;
    long unsigned int fl_downgrade_time;
    const struct file_lock_operations *fl_ops;
    const struct lock_manager_operations *fl_lmops;
    union (anon) fl_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct file_lock {
    struct file_lock *fl_blocker;
    struct list_head fl_list;
    struct hlist_node fl_link;
    struct list_head fl_blocked_requests;
    struct list_head fl_blocked_member;
    fl_owner_t fl_owner;
    unsigned int fl_flags;
    unsigned char fl_type;
    unsigned int fl_pid;
    int fl_link_cpu;
    wait_queue_head_t fl_wait;
    struct file *fl_file;
    loff_t fl_start;
    loff_t fl_end;
    struct fasync_struct *fl_fasync;
    long unsigned int fl_break_time;
    long unsigned int fl_downgrade_time;
    const struct file_lock_operations *fl_ops;
    const struct lock_manager_operations *fl_lmops;
    union (anon) fl_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct file_lock {
    struct file_lock *fl_blocker;
    struct list_head fl_list;
    struct hlist_node fl_link;
    struct list_head fl_blocked_requests;
    struct list_head fl_blocked_member;
    fl_owner_t fl_owner;
    unsigned int fl_flags;
    unsigned char fl_type;
    unsigned int fl_pid;
    int fl_link_cpu;
    wait_queue_head_t fl_wait;
    struct file *fl_file;
    loff_t fl_start;
    loff_t fl_end;
    struct fasync_struct *fl_fasync;
    long unsigned int fl_break_time;
    long unsigned int fl_downgrade_time;
    const struct file_lock_operations *fl_ops;
    const struct lock_manager_operations *fl_lmops;
    union (anon) fl_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct file_lock {
    struct file_lock *fl_blocker;
    struct list_head fl_list;
    struct hlist_node fl_link;
    struct list_head fl_blocked_requests;
    struct list_head fl_blocked_member;
    fl_owner_t fl_owner;
    unsigned int fl_flags;
    unsigned char fl_type;
    unsigned int fl_pid;
    int fl_link_cpu;
    wait_queue_head_t fl_wait;
    struct file *fl_file;
    loff_t fl_start;
    loff_t fl_end;
    struct fasync_struct *fl_fasync;
    long unsigned int fl_break_time;
    long unsigned int fl_downgrade_time;
    const struct file_lock_operations *fl_ops;
    const struct lock_manager_operations *fl_lmops;
    union (anon) fl_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct file_lock {
    struct file_lock *fl_blocker;
    struct list_head fl_list;
    struct hlist_node fl_link;
    struct list_head fl_blocked_requests;
    struct list_head fl_blocked_member;
    fl_owner_t fl_owner;
    unsigned int fl_flags;
    unsigned char fl_type;
    unsigned int fl_pid;
    int fl_link_cpu;
    wait_queue_head_t fl_wait;
    struct file *fl_file;
    loff_t fl_start;
    loff_t fl_end;
    struct fasync_struct *fl_fasync;
    long unsigned int fl_break_time;
    long unsigned int fl_downgrade_time;
    const struct file_lock_operations *fl_ops;
    const struct lock_manager_operations *fl_lmops;
    union (anon) fl_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct file_lock {
    struct file_lock *fl_blocker;
    struct list_head fl_list;
    struct hlist_node fl_link;
    struct list_head fl_blocked_requests;
    struct list_head fl_blocked_member;
    fl_owner_t fl_owner;
    unsigned int fl_flags;
    unsigned char fl_type;
    unsigned int fl_pid;
    int fl_link_cpu;
    wait_queue_head_t fl_wait;
    struct file *fl_file;
    loff_t fl_start;
    loff_t fl_end;
    struct fasync_struct *fl_fasync;
    long unsigned int fl_break_time;
    long unsigned int fl_downgrade_time;
    const struct file_lock_operations *fl_ops;
    const struct lock_manager_operations *fl_lmops;
    union (anon) fl_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct file_lock {
    struct file_lock *fl_blocker;
    struct list_head fl_list;
    struct hlist_node fl_link;
    struct list_head fl_blocked_requests;
    struct list_head fl_blocked_member;
    fl_owner_t fl_owner;
    unsigned int fl_flags;
    unsigned char fl_type;
    unsigned int fl_pid;
    int fl_link_cpu;
    wait_queue_head_t fl_wait;
    struct file *fl_file;
    loff_t fl_start;
    loff_t fl_end;
    struct fasync_struct *fl_fasync;
    long unsigned int fl_break_time;
    long unsigned int fl_downgrade_time;
    const struct file_lock_operations *fl_ops;
    const struct lock_manager_operations *fl_lmops;
    union (anon) fl_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct file_lock {
    struct file_lock *fl_blocker;
    struct list_head fl_list;
    struct hlist_node fl_link;
    struct list_head fl_blocked_requests;
    struct list_head fl_blocked_member;
    fl_owner_t fl_owner;
    unsigned int fl_flags;
    unsigned char fl_type;
    unsigned int fl_pid;
    int fl_link_cpu;
    wait_queue_head_t fl_wait;
    struct file *fl_file;
    loff_t fl_start;
    loff_t fl_end;
    struct fasync_struct *fl_fasync;
    long unsigned int fl_break_time;
    long unsigned int fl_downgrade_time;
    const struct file_lock_operations *fl_ops;
    const struct lock_manager_operations *fl_lmops;
    union (anon) fl_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct file_lock {
    struct file_lock *fl_blocker;
    struct list_head fl_list;
    struct hlist_node fl_link;
    struct list_head fl_blocked_requests;
    struct list_head fl_blocked_member;
    fl_owner_t fl_owner;
    unsigned int fl_flags;
    unsigned char fl_type;
    unsigned int fl_pid;
    int fl_link_cpu;
    wait_queue_head_t fl_wait;
    struct file *fl_file;
    loff_t fl_start;
    loff_t fl_end;
    struct fasync_struct *fl_fasync;
    long unsigned int fl_break_time;
    long unsigned int fl_downgrade_time;
    const struct file_lock_operations *fl_ops;
    const struct lock_manager_operations *fl_lmops;
    union (anon) fl_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct file_lock {
    struct file_lock *fl_blocker;
    struct list_head fl_list;
    struct hlist_node fl_link;
    struct list_head fl_blocked_requests;
    struct list_head fl_blocked_member;
    fl_owner_t fl_owner;
    unsigned int fl_flags;
    unsigned char fl_type;
    unsigned int fl_pid;
    int fl_link_cpu;
    wait_queue_head_t fl_wait;
    struct file *fl_file;
    loff_t fl_start;
    loff_t fl_end;
    struct fasync_struct *fl_fasync;
    long unsigned int fl_break_time;
    long unsigned int fl_downgrade_time;
    const struct file_lock_operations *fl_ops;
    const struct lock_manager_operations *fl_lmops;
    union (anon) fl_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct file_lock {
    struct file_lock *fl_blocker;
    struct list_head fl_list;
    struct hlist_node fl_link;
    struct list_head fl_blocked_requests;
    struct list_head fl_blocked_member;
    fl_owner_t fl_owner;
    unsigned int fl_flags;
    unsigned char fl_type;
    unsigned int fl_pid;
    int fl_link_cpu;
    wait_queue_head_t fl_wait;
    struct file *fl_file;
    loff_t fl_start;
    loff_t fl_end;
    struct fasync_struct *fl_fasync;
    long unsigned int fl_break_time;
    long unsigned int fl_downgrade_time;
    const struct file_lock_operations *fl_ops;
    const struct lock_manager_operations *fl_lmops;
    union (anon) fl_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct file_lock {
    struct file_lock *fl_blocker;
    struct list_head fl_list;
    struct hlist_node fl_link;
    struct list_head fl_blocked_requests;
    struct list_head fl_blocked_member;
    fl_owner_t fl_owner;
    unsigned int fl_flags;
    unsigned char fl_type;
    unsigned int fl_pid;
    int fl_link_cpu;
    wait_queue_head_t fl_wait;
    struct file *fl_file;
    loff_t fl_start;
    loff_t fl_end;
    struct fasync_struct *fl_fasync;
    long unsigned int fl_break_time;
    long unsigned int fl_downgrade_time;
    const struct file_lock_operations *fl_ops;
    const struct lock_manager_operations *fl_lmops;
    union (anon) fl_u;
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
struct file_lock {
    struct file_lock *fl_blocker;
    struct list_head fl_list;
    struct hlist_node fl_link;
    struct list_head fl_blocked_requests;
    struct list_head fl_blocked_member;
    fl_owner_t fl_owner;
    unsigned int fl_flags;
    unsigned char fl_type;
    unsigned int fl_pid;
    int fl_link_cpu;
    wait_queue_head_t fl_wait;
    struct file *fl_file;
    loff_t fl_start;
    loff_t fl_end;
    struct fasync_struct *fl_fasync;
    long unsigned int fl_break_time;
    long unsigned int fl_downgrade_time;
    const struct file_lock_operations *fl_ops;
    const struct lock_manager_operations *fl_lmops;
    union (anon) fl_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct file_lock {
    struct file_lock *fl_blocker;
    struct list_head fl_list;
    struct hlist_node fl_link;
    struct list_head fl_blocked_requests;
    struct list_head fl_blocked_member;
    fl_owner_t fl_owner;
    unsigned int fl_flags;
    unsigned char fl_type;
    unsigned int fl_pid;
    int fl_link_cpu;
    wait_queue_head_t fl_wait;
    struct file *fl_file;
    loff_t fl_start;
    loff_t fl_end;
    struct fasync_struct *fl_fasync;
    long unsigned int fl_break_time;
    long unsigned int fl_downgrade_time;
    const struct file_lock_operations *fl_ops;
    const struct lock_manager_operations *fl_lmops;
    union (anon) fl_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct file_lock {
    struct file_lock *fl_blocker;
    struct list_head fl_list;
    struct hlist_node fl_link;
    struct list_head fl_blocked_requests;
    struct list_head fl_blocked_member;
    fl_owner_t fl_owner;
    unsigned int fl_flags;
    unsigned char fl_type;
    unsigned int fl_pid;
    int fl_link_cpu;
    wait_queue_head_t fl_wait;
    struct file *fl_file;
    loff_t fl_start;
    loff_t fl_end;
    struct fasync_struct *fl_fasync;
    long unsigned int fl_break_time;
    long unsigned int fl_downgrade_time;
    const struct file_lock_operations *fl_ops;
    const struct lock_manager_operations *fl_lmops;
    union (anon) fl_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct file_lock {
    struct file_lock *fl_blocker;
    struct list_head fl_list;
    struct hlist_node fl_link;
    struct list_head fl_blocked_requests;
    struct list_head fl_blocked_member;
    fl_owner_t fl_owner;
    unsigned int fl_flags;
    unsigned char fl_type;
    unsigned int fl_pid;
    int fl_link_cpu;
    wait_queue_head_t fl_wait;
    struct file *fl_file;
    loff_t fl_start;
    loff_t fl_end;
    struct fasync_struct *fl_fasync;
    long unsigned int fl_break_time;
    long unsigned int fl_downgrade_time;
    const struct file_lock_operations *fl_ops;
    const struct lock_manager_operations *fl_lmops;
    union (anon) fl_u;
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
struct file_lock {
    struct file_lock *fl_blocker;
    struct list_head fl_list;
    struct hlist_node fl_link;
    struct list_head fl_blocked_requests;
    struct list_head fl_blocked_member;
    fl_owner_t fl_owner;
    unsigned int fl_flags;
    unsigned char fl_type;
    unsigned int fl_pid;
    int fl_link_cpu;
    wait_queue_head_t fl_wait;
    struct file *fl_file;
    loff_t fl_start;
    loff_t fl_end;
    struct fasync_struct *fl_fasync;
    long unsigned int fl_break_time;
    long unsigned int fl_downgrade_time;
    const struct file_lock_operations *fl_ops;
    const struct lock_manager_operations *fl_lmops;
    union (anon) fl_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct file_lock {
    struct file_lock *fl_blocker;
    struct list_head fl_list;
    struct hlist_node fl_link;
    struct list_head fl_blocked_requests;
    struct list_head fl_blocked_member;
    fl_owner_t fl_owner;
    unsigned int fl_flags;
    unsigned char fl_type;
    unsigned int fl_pid;
    int fl_link_cpu;
    wait_queue_head_t fl_wait;
    struct file *fl_file;
    loff_t fl_start;
    loff_t fl_end;
    struct fasync_struct *fl_fasync;
    long unsigned int fl_break_time;
    long unsigned int fl_downgrade_time;
    const struct file_lock_operations *fl_ops;
    const struct lock_manager_operations *fl_lmops;
    union (anon) fl_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct file_lock {
    struct file_lock *fl_blocker;
    struct list_head fl_list;
    struct hlist_node fl_link;
    struct list_head fl_blocked_requests;
    struct list_head fl_blocked_member;
    fl_owner_t fl_owner;
    unsigned int fl_flags;
    unsigned char fl_type;
    unsigned int fl_pid;
    int fl_link_cpu;
    wait_queue_head_t fl_wait;
    struct file *fl_file;
    loff_t fl_start;
    loff_t fl_end;
    struct fasync_struct *fl_fasync;
    long unsigned int fl_break_time;
    long unsigned int fl_downgrade_time;
    const struct file_lock_operations *fl_ops;
    const struct lock_manager_operations *fl_lmops;
    union (anon) fl_u;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct file_lock {
    struct file_lock *fl_blocker;
    struct list_head fl_list;
    struct hlist_node fl_link;
    struct list_head fl_blocked_requests;
    struct list_head fl_blocked_member;
    fl_owner_t fl_owner;
    unsigned int fl_flags;
    unsigned char fl_type;
    unsigned int fl_pid;
    int fl_link_cpu;
    wait_queue_head_t fl_wait;
    struct file *fl_file;
    loff_t fl_start;
    loff_t fl_end;
    struct fasync_struct *fl_fasync;
    long unsigned int fl_break_time;
    long unsigned int fl_downgrade_time;
    const struct file_lock_operations *fl_ops;
    const struct lock_manager_operations *fl_lmops;
    union (anon) fl_u;
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
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct pid *fl_nspid</code>
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
<code>struct file_lock *fl_blocker</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head fl_blocked_requests</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head fl_blocked_member</code>
</li>
<li>
<b>Field removed. </b>
<code>struct file_lock *fl_next</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head fl_block</code>
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
