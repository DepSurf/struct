# Struct: <code>sk_psock</code>

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
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct sk_psock {
    struct sock *sk;
    struct sock *sk_redir;
    u32 apply_bytes;
    u32 cork_bytes;
    u32 eval;
    struct sk_msg *cork;
    struct sk_psock_progs progs;
    struct sk_psock_parser parser;
    struct sk_buff_head ingress_skb;
    struct list_head ingress_msg;
    long unsigned int state;
    struct list_head link;
    spinlock_t link_lock;
    refcount_t refcnt;
    void (*saved_unhash)(struct sock *);
    void (*saved_close)(struct sock *, long int);
    void (*saved_write_space)(struct sock *);
    struct proto *sk_proto;
    struct sk_psock_work_state work_state;
    struct work_struct work;
    struct callback_head rcu;
    struct work_struct gc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct sk_psock {
    struct sock *sk;
    struct sock *sk_redir;
    u32 apply_bytes;
    u32 cork_bytes;
    u32 eval;
    struct sk_msg *cork;
    struct sk_psock_progs progs;
    struct sk_psock_parser parser;
    struct sk_buff_head ingress_skb;
    struct list_head ingress_msg;
    long unsigned int state;
    struct list_head link;
    spinlock_t link_lock;
    refcount_t refcnt;
    void (*saved_unhash)(struct sock *);
    void (*saved_close)(struct sock *, long int);
    void (*saved_write_space)(struct sock *);
    struct proto *sk_proto;
    struct sk_psock_work_state work_state;
    struct work_struct work;
    struct callback_head rcu;
    struct work_struct gc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct sk_psock {
    struct sock *sk;
    struct sock *sk_redir;
    u32 apply_bytes;
    u32 cork_bytes;
    u32 eval;
    struct sk_msg *cork;
    struct sk_psock_progs progs;
    struct sk_psock_parser parser;
    struct sk_buff_head ingress_skb;
    struct list_head ingress_msg;
    long unsigned int state;
    struct list_head link;
    spinlock_t link_lock;
    refcount_t refcnt;
    void (*saved_unhash)(struct sock *);
    void (*saved_close)(struct sock *, long int);
    void (*saved_write_space)(struct sock *);
    struct proto *sk_proto;
    struct sk_psock_work_state work_state;
    struct work_struct work;
    struct callback_head rcu;
    struct work_struct gc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct sk_psock {
    struct sock *sk;
    struct sock *sk_redir;
    u32 apply_bytes;
    u32 cork_bytes;
    u32 eval;
    struct sk_msg *cork;
    struct sk_psock_progs progs;
    struct sk_psock_parser parser;
    struct sk_buff_head ingress_skb;
    struct list_head ingress_msg;
    long unsigned int state;
    struct list_head link;
    spinlock_t link_lock;
    refcount_t refcnt;
    void (*saved_unhash)(struct sock *);
    void (*saved_close)(struct sock *, long int);
    void (*saved_write_space)(struct sock *);
    struct proto *sk_proto;
    struct sk_psock_work_state work_state;
    struct work_struct work;
    struct callback_head rcu;
    struct work_struct gc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct sk_psock {
    struct sock *sk;
    struct sock *sk_redir;
    u32 apply_bytes;
    u32 cork_bytes;
    u32 eval;
    struct sk_msg *cork;
    struct sk_psock_progs progs;
    struct sk_psock_parser parser;
    struct sk_buff_head ingress_skb;
    struct list_head ingress_msg;
    long unsigned int state;
    struct list_head link;
    spinlock_t link_lock;
    refcount_t refcnt;
    void (*saved_unhash)(struct sock *);
    void (*saved_close)(struct sock *, long int);
    void (*saved_write_space)(struct sock *);
    struct proto *sk_proto;
    struct sk_psock_work_state work_state;
    struct work_struct work;
    struct callback_head rcu;
    struct work_struct gc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct sk_psock {
    struct sock *sk;
    struct sock *sk_redir;
    u32 apply_bytes;
    u32 cork_bytes;
    u32 eval;
    struct sk_msg *cork;
    struct sk_psock_progs progs;
    struct strparser strp;
    struct sk_buff_head ingress_skb;
    struct list_head ingress_msg;
    spinlock_t ingress_lock;
    long unsigned int state;
    struct list_head link;
    spinlock_t link_lock;
    refcount_t refcnt;
    void (*saved_unhash)(struct sock *);
    void (*saved_close)(struct sock *, long int);
    void (*saved_write_space)(struct sock *);
    void (*saved_data_ready)(struct sock *);
    int (*psock_update_sk_prot)(struct sock *, struct sk_psock *, bool);
    struct proto *sk_proto;
    struct mutex work_mutex;
    struct sk_psock_work_state work_state;
    struct work_struct work;
    struct rcu_work rwork;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct sk_psock {
    struct sock *sk;
    struct sock *sk_redir;
    u32 apply_bytes;
    u32 cork_bytes;
    u32 eval;
    struct sk_msg *cork;
    struct sk_psock_progs progs;
    struct strparser strp;
    struct sk_buff_head ingress_skb;
    struct list_head ingress_msg;
    spinlock_t ingress_lock;
    long unsigned int state;
    struct list_head link;
    spinlock_t link_lock;
    refcount_t refcnt;
    void (*saved_unhash)(struct sock *);
    void (*saved_close)(struct sock *, long int);
    void (*saved_write_space)(struct sock *);
    void (*saved_data_ready)(struct sock *);
    int (*psock_update_sk_prot)(struct sock *, struct sk_psock *, bool);
    struct proto *sk_proto;
    struct mutex work_mutex;
    struct sk_psock_work_state work_state;
    struct work_struct work;
    struct rcu_work rwork;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct sk_psock {
    struct sock *sk;
    struct sock *sk_redir;
    u32 apply_bytes;
    u32 cork_bytes;
    u32 eval;
    struct sk_msg *cork;
    struct sk_psock_progs progs;
    struct strparser strp;
    struct sk_buff_head ingress_skb;
    struct list_head ingress_msg;
    spinlock_t ingress_lock;
    long unsigned int state;
    struct list_head link;
    spinlock_t link_lock;
    refcount_t refcnt;
    void (*saved_unhash)(struct sock *);
    void (*saved_close)(struct sock *, long int);
    void (*saved_write_space)(struct sock *);
    void (*saved_data_ready)(struct sock *);
    int (*psock_update_sk_prot)(struct sock *, struct sk_psock *, bool);
    struct proto *sk_proto;
    struct mutex work_mutex;
    struct sk_psock_work_state work_state;
    struct work_struct work;
    struct rcu_work rwork;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct sk_psock {
    struct sock *sk;
    struct sock *sk_redir;
    u32 apply_bytes;
    u32 cork_bytes;
    u32 eval;
    bool redir_ingress;
    struct sk_msg *cork;
    struct sk_psock_progs progs;
    struct strparser strp;
    struct sk_buff_head ingress_skb;
    struct list_head ingress_msg;
    spinlock_t ingress_lock;
    long unsigned int state;
    struct list_head link;
    spinlock_t link_lock;
    refcount_t refcnt;
    void (*saved_unhash)(struct sock *);
    void (*saved_destroy)(struct sock *);
    void (*saved_close)(struct sock *, long int);
    void (*saved_write_space)(struct sock *);
    void (*saved_data_ready)(struct sock *);
    int (*psock_update_sk_prot)(struct sock *, struct sk_psock *, bool);
    struct proto *sk_proto;
    struct mutex work_mutex;
    struct sk_psock_work_state work_state;
    struct work_struct work;
    struct rcu_work rwork;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct sk_psock {
    struct sock *sk;
    struct sock *sk_redir;
    u32 apply_bytes;
    u32 cork_bytes;
    u32 eval;
    bool redir_ingress;
    struct sk_msg *cork;
    struct sk_psock_progs progs;
    struct strparser strp;
    struct sk_buff_head ingress_skb;
    struct list_head ingress_msg;
    spinlock_t ingress_lock;
    long unsigned int state;
    struct list_head link;
    spinlock_t link_lock;
    refcount_t refcnt;
    void (*saved_unhash)(struct sock *);
    void (*saved_destroy)(struct sock *);
    void (*saved_close)(struct sock *, long int);
    void (*saved_write_space)(struct sock *);
    void (*saved_data_ready)(struct sock *);
    int (*psock_update_sk_prot)(struct sock *, struct sk_psock *, bool);
    struct proto *sk_proto;
    struct mutex work_mutex;
    struct sk_psock_work_state work_state;
    struct delayed_work work;
    struct rcu_work rwork;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct sk_psock {
    struct sock *sk;
    struct sock *sk_redir;
    u32 apply_bytes;
    u32 cork_bytes;
    u32 eval;
    bool redir_ingress;
    struct sk_msg *cork;
    struct sk_psock_progs progs;
    struct strparser strp;
    struct sk_buff_head ingress_skb;
    struct list_head ingress_msg;
    spinlock_t ingress_lock;
    long unsigned int state;
    struct list_head link;
    spinlock_t link_lock;
    refcount_t refcnt;
    void (*saved_unhash)(struct sock *);
    void (*saved_destroy)(struct sock *);
    void (*saved_close)(struct sock *, long int);
    void (*saved_write_space)(struct sock *);
    void (*saved_data_ready)(struct sock *);
    int (*psock_update_sk_prot)(struct sock *, struct sk_psock *, bool);
    struct proto *sk_proto;
    struct mutex work_mutex;
    struct sk_psock_work_state work_state;
    struct delayed_work work;
    struct sock *sk_pair;
    struct rcu_work rwork;
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
struct sk_psock {
    struct sock *sk;
    struct sock *sk_redir;
    u32 apply_bytes;
    u32 cork_bytes;
    u32 eval;
    struct sk_msg *cork;
    struct sk_psock_progs progs;
    struct sk_psock_parser parser;
    struct sk_buff_head ingress_skb;
    struct list_head ingress_msg;
    long unsigned int state;
    struct list_head link;
    spinlock_t link_lock;
    refcount_t refcnt;
    void (*saved_unhash)(struct sock *);
    void (*saved_close)(struct sock *, long int);
    void (*saved_write_space)(struct sock *);
    struct proto *sk_proto;
    struct sk_psock_work_state work_state;
    struct work_struct work;
    struct callback_head rcu;
    struct work_struct gc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct sk_psock {
    struct sock *sk;
    struct sock *sk_redir;
    u32 apply_bytes;
    u32 cork_bytes;
    u32 eval;
    struct sk_msg *cork;
    struct sk_psock_progs progs;
    struct sk_psock_parser parser;
    struct sk_buff_head ingress_skb;
    struct list_head ingress_msg;
    long unsigned int state;
    struct list_head link;
    spinlock_t link_lock;
    refcount_t refcnt;
    void (*saved_unhash)(struct sock *);
    void (*saved_close)(struct sock *, long int);
    void (*saved_write_space)(struct sock *);
    struct proto *sk_proto;
    struct sk_psock_work_state work_state;
    struct work_struct work;
    struct callback_head rcu;
    struct work_struct gc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct sk_psock {
    struct sock *sk;
    struct sock *sk_redir;
    u32 apply_bytes;
    u32 cork_bytes;
    u32 eval;
    struct sk_msg *cork;
    struct sk_psock_progs progs;
    struct sk_psock_parser parser;
    struct sk_buff_head ingress_skb;
    struct list_head ingress_msg;
    long unsigned int state;
    struct list_head link;
    spinlock_t link_lock;
    refcount_t refcnt;
    void (*saved_unhash)(struct sock *);
    void (*saved_close)(struct sock *, long int);
    void (*saved_write_space)(struct sock *);
    struct proto *sk_proto;
    struct sk_psock_work_state work_state;
    struct work_struct work;
    struct callback_head rcu;
    struct work_struct gc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct sk_psock {
    struct sock *sk;
    struct sock *sk_redir;
    u32 apply_bytes;
    u32 cork_bytes;
    u32 eval;
    struct sk_msg *cork;
    struct sk_psock_progs progs;
    struct sk_psock_parser parser;
    struct sk_buff_head ingress_skb;
    struct list_head ingress_msg;
    long unsigned int state;
    struct list_head link;
    spinlock_t link_lock;
    refcount_t refcnt;
    void (*saved_unhash)(struct sock *);
    void (*saved_close)(struct sock *, long int);
    void (*saved_write_space)(struct sock *);
    struct proto *sk_proto;
    struct sk_psock_work_state work_state;
    struct work_struct work;
    struct callback_head rcu;
    struct work_struct gc;
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
struct sk_psock {
    struct sock *sk;
    struct sock *sk_redir;
    u32 apply_bytes;
    u32 cork_bytes;
    u32 eval;
    struct sk_msg *cork;
    struct sk_psock_progs progs;
    struct sk_psock_parser parser;
    struct sk_buff_head ingress_skb;
    struct list_head ingress_msg;
    long unsigned int state;
    struct list_head link;
    spinlock_t link_lock;
    refcount_t refcnt;
    void (*saved_unhash)(struct sock *);
    void (*saved_close)(struct sock *, long int);
    void (*saved_write_space)(struct sock *);
    struct proto *sk_proto;
    struct sk_psock_work_state work_state;
    struct work_struct work;
    struct callback_head rcu;
    struct work_struct gc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct sk_psock {
    struct sock *sk;
    struct sock *sk_redir;
    u32 apply_bytes;
    u32 cork_bytes;
    u32 eval;
    struct sk_msg *cork;
    struct sk_psock_progs progs;
    struct sk_psock_parser parser;
    struct sk_buff_head ingress_skb;
    struct list_head ingress_msg;
    long unsigned int state;
    struct list_head link;
    spinlock_t link_lock;
    refcount_t refcnt;
    void (*saved_unhash)(struct sock *);
    void (*saved_close)(struct sock *, long int);
    void (*saved_write_space)(struct sock *);
    struct proto *sk_proto;
    struct sk_psock_work_state work_state;
    struct work_struct work;
    struct callback_head rcu;
    struct work_struct gc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct sk_psock {
    struct sock *sk;
    struct sock *sk_redir;
    u32 apply_bytes;
    u32 cork_bytes;
    u32 eval;
    struct sk_msg *cork;
    struct sk_psock_progs progs;
    struct sk_psock_parser parser;
    struct sk_buff_head ingress_skb;
    struct list_head ingress_msg;
    long unsigned int state;
    struct list_head link;
    spinlock_t link_lock;
    refcount_t refcnt;
    void (*saved_unhash)(struct sock *);
    void (*saved_close)(struct sock *, long int);
    void (*saved_write_space)(struct sock *);
    struct proto *sk_proto;
    struct sk_psock_work_state work_state;
    struct work_struct work;
    struct callback_head rcu;
    struct work_struct gc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct sk_psock {
    struct sock *sk;
    struct sock *sk_redir;
    u32 apply_bytes;
    u32 cork_bytes;
    u32 eval;
    struct sk_msg *cork;
    struct sk_psock_progs progs;
    struct sk_psock_parser parser;
    struct sk_buff_head ingress_skb;
    struct list_head ingress_msg;
    long unsigned int state;
    struct list_head link;
    spinlock_t link_lock;
    refcount_t refcnt;
    void (*saved_unhash)(struct sock *);
    void (*saved_close)(struct sock *, long int);
    void (*saved_write_space)(struct sock *);
    struct proto *sk_proto;
    struct sk_psock_work_state work_state;
    struct work_struct work;
    struct callback_head rcu;
    struct work_struct gc;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct strparser strp</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t ingress_lock</code>
</li>
<li>
<b>Field added. </b>
<code>void (*saved_data_ready)(struct sock *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*psock_update_sk_prot)(struct sock *, struct sk_psock *, bool)</code>
</li>
<li>
<b>Field added. </b>
<code>struct mutex work_mutex</code>
</li>
<li>
<b>Field added. </b>
<code>struct rcu_work rwork</code>
</li>
<li>
<b>Field removed. </b>
<code>struct sk_psock_parser parser</code>
</li>
<li>
<b>Field removed. </b>
<code>struct callback_head rcu</code>
</li>
<li>
<b>Field removed. </b>
<code>struct work_struct gc</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool redir_ingress</code>
</li>
<li>
<b>Field added. </b>
<code>void (*saved_destroy)(struct sock *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct work_struct work</code> ➡️ <code>struct delayed_work work</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct sock *sk_pair</code>
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
