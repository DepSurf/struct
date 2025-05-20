# Struct: <code>mqueue_inode_info</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct mqueue_inode_info {
    spinlock_t lock;
    struct inode vfs_inode;
    wait_queue_head_t wait_q;
    struct rb_root msg_tree;
    struct posix_msg_tree_node *node_cache;
    struct mq_attr attr;
    struct sigevent notify;
    struct pid *notify_owner;
    struct user_namespace *notify_user_ns;
    struct user_struct *user;
    struct sock *notify_sock;
    struct sk_buff *notify_cookie;
    struct ext_wait_queue e_wait_q[2];
    long unsigned int qsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct mqueue_inode_info {
    spinlock_t lock;
    struct inode vfs_inode;
    wait_queue_head_t wait_q;
    struct rb_root msg_tree;
    struct posix_msg_tree_node *node_cache;
    struct mq_attr attr;
    struct sigevent notify;
    struct pid *notify_owner;
    struct user_namespace *notify_user_ns;
    struct user_struct *user;
    struct sock *notify_sock;
    struct sk_buff *notify_cookie;
    struct ext_wait_queue e_wait_q[2];
    long unsigned int qsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct mqueue_inode_info {
    spinlock_t lock;
    struct inode vfs_inode;
    wait_queue_head_t wait_q;
    struct rb_root msg_tree;
    struct posix_msg_tree_node *node_cache;
    struct mq_attr attr;
    struct sigevent notify;
    struct pid *notify_owner;
    struct user_namespace *notify_user_ns;
    struct user_struct *user;
    struct sock *notify_sock;
    struct sk_buff *notify_cookie;
    struct ext_wait_queue e_wait_q[2];
    long unsigned int qsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct mqueue_inode_info {
    spinlock_t lock;
    struct inode vfs_inode;
    wait_queue_head_t wait_q;
    struct rb_root msg_tree;
    struct posix_msg_tree_node *node_cache;
    struct mq_attr attr;
    struct sigevent notify;
    struct pid *notify_owner;
    struct user_namespace *notify_user_ns;
    struct user_struct *user;
    struct sock *notify_sock;
    struct sk_buff *notify_cookie;
    struct ext_wait_queue e_wait_q[2];
    long unsigned int qsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct mqueue_inode_info {
    spinlock_t lock;
    struct inode vfs_inode;
    wait_queue_head_t wait_q;
    struct rb_root msg_tree;
    struct posix_msg_tree_node *node_cache;
    struct mq_attr attr;
    struct sigevent notify;
    struct pid *notify_owner;
    struct user_namespace *notify_user_ns;
    struct user_struct *user;
    struct sock *notify_sock;
    struct sk_buff *notify_cookie;
    struct ext_wait_queue e_wait_q[2];
    long unsigned int qsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct mqueue_inode_info {
    spinlock_t lock;
    struct inode vfs_inode;
    wait_queue_head_t wait_q;
    struct rb_root msg_tree;
    struct posix_msg_tree_node *node_cache;
    struct mq_attr attr;
    struct sigevent notify;
    struct pid *notify_owner;
    struct user_namespace *notify_user_ns;
    struct user_struct *user;
    struct sock *notify_sock;
    struct sk_buff *notify_cookie;
    struct ext_wait_queue e_wait_q[2];
    long unsigned int qsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct mqueue_inode_info {
    spinlock_t lock;
    struct inode vfs_inode;
    wait_queue_head_t wait_q;
    struct rb_root msg_tree;
    struct posix_msg_tree_node *node_cache;
    struct mq_attr attr;
    struct sigevent notify;
    struct pid *notify_owner;
    struct user_namespace *notify_user_ns;
    struct user_struct *user;
    struct sock *notify_sock;
    struct sk_buff *notify_cookie;
    struct ext_wait_queue e_wait_q[2];
    long unsigned int qsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct mqueue_inode_info {
    spinlock_t lock;
    struct inode vfs_inode;
    wait_queue_head_t wait_q;
    struct rb_root msg_tree;
    struct rb_node *msg_tree_rightmost;
    struct posix_msg_tree_node *node_cache;
    struct mq_attr attr;
    struct sigevent notify;
    struct pid *notify_owner;
    struct user_namespace *notify_user_ns;
    struct user_struct *user;
    struct sock *notify_sock;
    struct sk_buff *notify_cookie;
    struct ext_wait_queue e_wait_q[2];
    long unsigned int qsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct mqueue_inode_info {
    spinlock_t lock;
    struct inode vfs_inode;
    wait_queue_head_t wait_q;
    struct rb_root msg_tree;
    struct rb_node *msg_tree_rightmost;
    struct posix_msg_tree_node *node_cache;
    struct mq_attr attr;
    struct sigevent notify;
    struct pid *notify_owner;
    struct user_namespace *notify_user_ns;
    struct user_struct *user;
    struct sock *notify_sock;
    struct sk_buff *notify_cookie;
    struct ext_wait_queue e_wait_q[2];
    long unsigned int qsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct mqueue_inode_info {
    spinlock_t lock;
    struct inode vfs_inode;
    wait_queue_head_t wait_q;
    struct rb_root msg_tree;
    struct rb_node *msg_tree_rightmost;
    struct posix_msg_tree_node *node_cache;
    struct mq_attr attr;
    struct sigevent notify;
    struct pid *notify_owner;
    u32 notify_self_exec_id;
    struct user_namespace *notify_user_ns;
    struct user_struct *user;
    struct sock *notify_sock;
    struct sk_buff *notify_cookie;
    struct ext_wait_queue e_wait_q[2];
    long unsigned int qsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mqueue_inode_info {
    spinlock_t lock;
    struct inode vfs_inode;
    wait_queue_head_t wait_q;
    struct rb_root msg_tree;
    struct rb_node *msg_tree_rightmost;
    struct posix_msg_tree_node *node_cache;
    struct mq_attr attr;
    struct sigevent notify;
    struct pid *notify_owner;
    u32 notify_self_exec_id;
    struct user_namespace *notify_user_ns;
    struct user_struct *user;
    struct sock *notify_sock;
    struct sk_buff *notify_cookie;
    struct ext_wait_queue e_wait_q[2];
    long unsigned int qsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mqueue_inode_info {
    spinlock_t lock;
    struct inode vfs_inode;
    wait_queue_head_t wait_q;
    struct rb_root msg_tree;
    struct rb_node *msg_tree_rightmost;
    struct posix_msg_tree_node *node_cache;
    struct mq_attr attr;
    struct sigevent notify;
    struct pid *notify_owner;
    u32 notify_self_exec_id;
    struct user_namespace *notify_user_ns;
    struct user_struct *user;
    struct sock *notify_sock;
    struct sk_buff *notify_cookie;
    struct ext_wait_queue e_wait_q[2];
    long unsigned int qsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mqueue_inode_info {
    spinlock_t lock;
    struct inode vfs_inode;
    wait_queue_head_t wait_q;
    struct rb_root msg_tree;
    struct rb_node *msg_tree_rightmost;
    struct posix_msg_tree_node *node_cache;
    struct mq_attr attr;
    struct sigevent notify;
    struct pid *notify_owner;
    u32 notify_self_exec_id;
    struct user_namespace *notify_user_ns;
    struct ucounts *ucounts;
    struct sock *notify_sock;
    struct sk_buff *notify_cookie;
    struct ext_wait_queue e_wait_q[2];
    long unsigned int qsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mqueue_inode_info {
    spinlock_t lock;
    struct inode vfs_inode;
    wait_queue_head_t wait_q;
    struct rb_root msg_tree;
    struct rb_node *msg_tree_rightmost;
    struct posix_msg_tree_node *node_cache;
    struct mq_attr attr;
    struct sigevent notify;
    struct pid *notify_owner;
    u32 notify_self_exec_id;
    struct user_namespace *notify_user_ns;
    struct ucounts *ucounts;
    struct sock *notify_sock;
    struct sk_buff *notify_cookie;
    struct ext_wait_queue e_wait_q[2];
    long unsigned int qsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mqueue_inode_info {
    spinlock_t lock;
    struct inode vfs_inode;
    wait_queue_head_t wait_q;
    struct rb_root msg_tree;
    struct rb_node *msg_tree_rightmost;
    struct posix_msg_tree_node *node_cache;
    struct mq_attr attr;
    struct sigevent notify;
    struct pid *notify_owner;
    u32 notify_self_exec_id;
    struct user_namespace *notify_user_ns;
    struct ucounts *ucounts;
    struct sock *notify_sock;
    struct sk_buff *notify_cookie;
    struct ext_wait_queue e_wait_q[2];
    long unsigned int qsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mqueue_inode_info {
    spinlock_t lock;
    struct inode vfs_inode;
    wait_queue_head_t wait_q;
    struct rb_root msg_tree;
    struct rb_node *msg_tree_rightmost;
    struct posix_msg_tree_node *node_cache;
    struct mq_attr attr;
    struct sigevent notify;
    struct pid *notify_owner;
    u32 notify_self_exec_id;
    struct user_namespace *notify_user_ns;
    struct ucounts *ucounts;
    struct sock *notify_sock;
    struct sk_buff *notify_cookie;
    struct ext_wait_queue e_wait_q[2];
    long unsigned int qsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mqueue_inode_info {
    spinlock_t lock;
    struct inode vfs_inode;
    wait_queue_head_t wait_q;
    struct rb_root msg_tree;
    struct rb_node *msg_tree_rightmost;
    struct posix_msg_tree_node *node_cache;
    struct mq_attr attr;
    struct sigevent notify;
    struct pid *notify_owner;
    u32 notify_self_exec_id;
    struct user_namespace *notify_user_ns;
    struct ucounts *ucounts;
    struct sock *notify_sock;
    struct sk_buff *notify_cookie;
    struct ext_wait_queue e_wait_q[2];
    long unsigned int qsize;
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
struct mqueue_inode_info {
    spinlock_t lock;
    struct inode vfs_inode;
    wait_queue_head_t wait_q;
    struct rb_root msg_tree;
    struct rb_node *msg_tree_rightmost;
    struct posix_msg_tree_node *node_cache;
    struct mq_attr attr;
    struct sigevent notify;
    struct pid *notify_owner;
    struct user_namespace *notify_user_ns;
    struct user_struct *user;
    struct sock *notify_sock;
    struct sk_buff *notify_cookie;
    struct ext_wait_queue e_wait_q[2];
    long unsigned int qsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mqueue_inode_info {
    spinlock_t lock;
    struct inode vfs_inode;
    wait_queue_head_t wait_q;
    struct rb_root msg_tree;
    struct rb_node *msg_tree_rightmost;
    struct posix_msg_tree_node *node_cache;
    struct mq_attr attr;
    struct sigevent notify;
    struct pid *notify_owner;
    struct user_namespace *notify_user_ns;
    struct user_struct *user;
    struct sock *notify_sock;
    struct sk_buff *notify_cookie;
    struct ext_wait_queue e_wait_q[2];
    long unsigned int qsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct mqueue_inode_info {
    spinlock_t lock;
    struct inode vfs_inode;
    wait_queue_head_t wait_q;
    struct rb_root msg_tree;
    struct rb_node *msg_tree_rightmost;
    struct posix_msg_tree_node *node_cache;
    struct mq_attr attr;
    struct sigevent notify;
    struct pid *notify_owner;
    struct user_namespace *notify_user_ns;
    struct user_struct *user;
    struct sock *notify_sock;
    struct sk_buff *notify_cookie;
    struct ext_wait_queue e_wait_q[2];
    long unsigned int qsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct mqueue_inode_info {
    spinlock_t lock;
    struct inode vfs_inode;
    wait_queue_head_t wait_q;
    struct rb_root msg_tree;
    struct rb_node *msg_tree_rightmost;
    struct posix_msg_tree_node *node_cache;
    struct mq_attr attr;
    struct sigevent notify;
    struct pid *notify_owner;
    struct user_namespace *notify_user_ns;
    struct user_struct *user;
    struct sock *notify_sock;
    struct sk_buff *notify_cookie;
    struct ext_wait_queue e_wait_q[2];
    long unsigned int qsize;
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
struct mqueue_inode_info {
    spinlock_t lock;
    struct inode vfs_inode;
    wait_queue_head_t wait_q;
    struct rb_root msg_tree;
    struct rb_node *msg_tree_rightmost;
    struct posix_msg_tree_node *node_cache;
    struct mq_attr attr;
    struct sigevent notify;
    struct pid *notify_owner;
    struct user_namespace *notify_user_ns;
    struct user_struct *user;
    struct sock *notify_sock;
    struct sk_buff *notify_cookie;
    struct ext_wait_queue e_wait_q[2];
    long unsigned int qsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct mqueue_inode_info {
    spinlock_t lock;
    struct inode vfs_inode;
    wait_queue_head_t wait_q;
    struct rb_root msg_tree;
    struct rb_node *msg_tree_rightmost;
    struct posix_msg_tree_node *node_cache;
    struct mq_attr attr;
    struct sigevent notify;
    struct pid *notify_owner;
    struct user_namespace *notify_user_ns;
    struct user_struct *user;
    struct sock *notify_sock;
    struct sk_buff *notify_cookie;
    struct ext_wait_queue e_wait_q[2];
    long unsigned int qsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct mqueue_inode_info {
    spinlock_t lock;
    struct inode vfs_inode;
    wait_queue_head_t wait_q;
    struct rb_root msg_tree;
    struct rb_node *msg_tree_rightmost;
    struct posix_msg_tree_node *node_cache;
    struct mq_attr attr;
    struct sigevent notify;
    struct pid *notify_owner;
    struct user_namespace *notify_user_ns;
    struct user_struct *user;
    struct sock *notify_sock;
    struct sk_buff *notify_cookie;
    struct ext_wait_queue e_wait_q[2];
    long unsigned int qsize;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct mqueue_inode_info {
    spinlock_t lock;
    struct inode vfs_inode;
    wait_queue_head_t wait_q;
    struct rb_root msg_tree;
    struct rb_node *msg_tree_rightmost;
    struct posix_msg_tree_node *node_cache;
    struct mq_attr attr;
    struct sigevent notify;
    struct pid *notify_owner;
    struct user_namespace *notify_user_ns;
    struct user_struct *user;
    struct sock *notify_sock;
    struct sk_buff *notify_cookie;
    struct ext_wait_queue e_wait_q[2];
    long unsigned int qsize;
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct rb_node *msg_tree_rightmost</code>
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
<code>u32 notify_self_exec_id</code>
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
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct ucounts *ucounts</code>
</li>
<li>
<b>Field removed. </b>
<code>struct user_struct *user</code>
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
