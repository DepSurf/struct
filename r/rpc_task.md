# Struct: <code>rpc_task</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct rpc_task {
    atomic_t tk_count;
    int tk_status;
    struct list_head tk_task;
    void (*tk_callback)(struct rpc_task *);
    void (*tk_action)(struct rpc_task *);
    long unsigned int tk_timeout;
    long unsigned int tk_runstate;
    struct rpc_wait_queue *tk_waitqueue;
    union (anon) u;
    struct rpc_message tk_msg;
    void *tk_calldata;
    const struct rpc_call_ops *tk_ops;
    struct rpc_clnt *tk_client;
    struct rpc_xprt *tk_xprt;
    struct rpc_rqst *tk_rqstp;
    struct workqueue_struct *tk_workqueue;
    ktime_t tk_start;
    pid_t tk_owner;
    short unsigned int tk_flags;
    short unsigned int tk_timeouts;
    short unsigned int tk_pid;
    unsigned char tk_priority;
    unsigned char tk_garb_retry;
    unsigned char tk_cred_retry;
    unsigned char tk_rebind_retry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rpc_task {
    atomic_t tk_count;
    int tk_status;
    struct list_head tk_task;
    void (*tk_callback)(struct rpc_task *);
    void (*tk_action)(struct rpc_task *);
    long unsigned int tk_timeout;
    long unsigned int tk_runstate;
    struct rpc_wait_queue *tk_waitqueue;
    union (anon) u;
    struct rpc_message tk_msg;
    void *tk_calldata;
    const struct rpc_call_ops *tk_ops;
    struct rpc_clnt *tk_client;
    struct rpc_xprt *tk_xprt;
    struct rpc_rqst *tk_rqstp;
    struct workqueue_struct *tk_workqueue;
    ktime_t tk_start;
    pid_t tk_owner;
    short unsigned int tk_flags;
    short unsigned int tk_timeouts;
    short unsigned int tk_pid;
    unsigned char tk_priority;
    unsigned char tk_garb_retry;
    unsigned char tk_cred_retry;
    unsigned char tk_rebind_retry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rpc_task {
    atomic_t tk_count;
    int tk_status;
    struct list_head tk_task;
    void (*tk_callback)(struct rpc_task *);
    void (*tk_action)(struct rpc_task *);
    long unsigned int tk_timeout;
    long unsigned int tk_runstate;
    struct rpc_wait_queue *tk_waitqueue;
    union (anon) u;
    struct rpc_message tk_msg;
    void *tk_calldata;
    const struct rpc_call_ops *tk_ops;
    struct rpc_clnt *tk_client;
    struct rpc_xprt *tk_xprt;
    struct rpc_rqst *tk_rqstp;
    struct workqueue_struct *tk_workqueue;
    ktime_t tk_start;
    pid_t tk_owner;
    short unsigned int tk_flags;
    short unsigned int tk_timeouts;
    short unsigned int tk_pid;
    unsigned char tk_priority;
    unsigned char tk_garb_retry;
    unsigned char tk_cred_retry;
    unsigned char tk_rebind_retry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rpc_task {
    atomic_t tk_count;
    int tk_status;
    struct list_head tk_task;
    void (*tk_callback)(struct rpc_task *);
    void (*tk_action)(struct rpc_task *);
    long unsigned int tk_timeout;
    long unsigned int tk_runstate;
    struct rpc_wait_queue *tk_waitqueue;
    union (anon) u;
    struct rpc_message tk_msg;
    void *tk_calldata;
    const struct rpc_call_ops *tk_ops;
    struct rpc_clnt *tk_client;
    struct rpc_xprt *tk_xprt;
    struct rpc_rqst *tk_rqstp;
    struct workqueue_struct *tk_workqueue;
    ktime_t tk_start;
    pid_t tk_owner;
    short unsigned int tk_flags;
    short unsigned int tk_timeouts;
    short unsigned int tk_pid;
    unsigned char tk_priority;
    unsigned char tk_garb_retry;
    unsigned char tk_cred_retry;
    unsigned char tk_rebind_retry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rpc_task {
    atomic_t tk_count;
    int tk_status;
    struct list_head tk_task;
    void (*tk_callback)(struct rpc_task *);
    void (*tk_action)(struct rpc_task *);
    long unsigned int tk_timeout;
    long unsigned int tk_runstate;
    struct rpc_wait_queue *tk_waitqueue;
    union (anon) u;
    struct rpc_message tk_msg;
    void *tk_calldata;
    const struct rpc_call_ops *tk_ops;
    struct rpc_clnt *tk_client;
    struct rpc_xprt *tk_xprt;
    struct rpc_rqst *tk_rqstp;
    struct workqueue_struct *tk_workqueue;
    ktime_t tk_start;
    pid_t tk_owner;
    short unsigned int tk_flags;
    short unsigned int tk_timeouts;
    short unsigned int tk_pid;
    unsigned char tk_priority;
    unsigned char tk_garb_retry;
    unsigned char tk_cred_retry;
    unsigned char tk_rebind_retry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rpc_task {
    atomic_t tk_count;
    int tk_status;
    struct list_head tk_task;
    void (*tk_callback)(struct rpc_task *);
    void (*tk_action)(struct rpc_task *);
    long unsigned int tk_timeout;
    long unsigned int tk_runstate;
    struct rpc_wait_queue *tk_waitqueue;
    union (anon) u;
    struct rpc_message tk_msg;
    void *tk_calldata;
    const struct rpc_call_ops *tk_ops;
    struct rpc_clnt *tk_client;
    struct rpc_xprt *tk_xprt;
    struct rpc_cred *tk_op_cred;
    struct rpc_rqst *tk_rqstp;
    struct workqueue_struct *tk_workqueue;
    ktime_t tk_start;
    pid_t tk_owner;
    short unsigned int tk_flags;
    short unsigned int tk_timeouts;
    short unsigned int tk_pid;
    unsigned char tk_priority;
    unsigned char tk_garb_retry;
    unsigned char tk_cred_retry;
    unsigned char tk_rebind_retry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rpc_task {
    atomic_t tk_count;
    int tk_status;
    struct list_head tk_task;
    void (*tk_callback)(struct rpc_task *);
    void (*tk_action)(struct rpc_task *);
    long unsigned int tk_timeout;
    long unsigned int tk_runstate;
    struct rpc_wait_queue *tk_waitqueue;
    union (anon) u;
    int tk_rpc_status;
    struct rpc_message tk_msg;
    void *tk_calldata;
    const struct rpc_call_ops *tk_ops;
    struct rpc_clnt *tk_client;
    struct rpc_xprt *tk_xprt;
    struct rpc_cred *tk_op_cred;
    struct rpc_rqst *tk_rqstp;
    struct workqueue_struct *tk_workqueue;
    ktime_t tk_start;
    pid_t tk_owner;
    short unsigned int tk_flags;
    short unsigned int tk_timeouts;
    short unsigned int tk_pid;
    unsigned char tk_priority;
    unsigned char tk_garb_retry;
    unsigned char tk_cred_retry;
    unsigned char tk_rebind_retry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rpc_task {
    atomic_t tk_count;
    int tk_status;
    struct list_head tk_task;
    void (*tk_callback)(struct rpc_task *);
    void (*tk_action)(struct rpc_task *);
    long unsigned int tk_timeout;
    long unsigned int tk_runstate;
    struct rpc_wait_queue *tk_waitqueue;
    union (anon) u;
    int tk_rpc_status;
    struct rpc_message tk_msg;
    void *tk_calldata;
    const struct rpc_call_ops *tk_ops;
    struct rpc_clnt *tk_client;
    struct rpc_xprt *tk_xprt;
    struct rpc_cred *tk_op_cred;
    struct rpc_rqst *tk_rqstp;
    struct workqueue_struct *tk_workqueue;
    ktime_t tk_start;
    pid_t tk_owner;
    short unsigned int tk_flags;
    short unsigned int tk_timeouts;
    short unsigned int tk_pid;
    unsigned char tk_priority;
    unsigned char tk_garb_retry;
    unsigned char tk_cred_retry;
    unsigned char tk_rebind_retry;
};
```
</details>
</li>
<li>
In <code>5.8</code>: Absent ⚠️
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rpc_task {
    atomic_t tk_count;
    int tk_status;
    struct list_head tk_task;
    void (*tk_callback)(struct rpc_task *);
    void (*tk_action)(struct rpc_task *);
    long unsigned int tk_timeout;
    long unsigned int tk_runstate;
    struct rpc_wait_queue *tk_waitqueue;
    union (anon) u;
    int tk_rpc_status;
    struct rpc_message tk_msg;
    void *tk_calldata;
    const struct rpc_call_ops *tk_ops;
    struct rpc_clnt *tk_client;
    struct rpc_xprt *tk_xprt;
    struct rpc_cred *tk_op_cred;
    struct rpc_rqst *tk_rqstp;
    struct workqueue_struct *tk_workqueue;
    ktime_t tk_start;
    pid_t tk_owner;
    short unsigned int tk_flags;
    short unsigned int tk_timeouts;
    short unsigned int tk_pid;
    unsigned char tk_priority;
    unsigned char tk_garb_retry;
    unsigned char tk_cred_retry;
    unsigned char tk_rebind_retry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rpc_task {
    atomic_t tk_count;
    int tk_status;
    struct list_head tk_task;
    void (*tk_callback)(struct rpc_task *);
    void (*tk_action)(struct rpc_task *);
    long unsigned int tk_timeout;
    long unsigned int tk_runstate;
    struct rpc_wait_queue *tk_waitqueue;
    union (anon) u;
    int tk_rpc_status;
    struct rpc_message tk_msg;
    void *tk_calldata;
    const struct rpc_call_ops *tk_ops;
    struct rpc_clnt *tk_client;
    struct rpc_xprt *tk_xprt;
    struct rpc_cred *tk_op_cred;
    struct rpc_rqst *tk_rqstp;
    struct workqueue_struct *tk_workqueue;
    ktime_t tk_start;
    pid_t tk_owner;
    short unsigned int tk_flags;
    short unsigned int tk_timeouts;
    short unsigned int tk_pid;
    unsigned char tk_priority;
    unsigned char tk_garb_retry;
    unsigned char tk_cred_retry;
    unsigned char tk_rebind_retry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rpc_task {
    atomic_t tk_count;
    int tk_status;
    struct list_head tk_task;
    void (*tk_callback)(struct rpc_task *);
    void (*tk_action)(struct rpc_task *);
    long unsigned int tk_timeout;
    long unsigned int tk_runstate;
    struct rpc_wait_queue *tk_waitqueue;
    union (anon) u;
    int tk_rpc_status;
    struct rpc_message tk_msg;
    void *tk_calldata;
    const struct rpc_call_ops *tk_ops;
    struct rpc_clnt *tk_client;
    struct rpc_xprt *tk_xprt;
    struct rpc_cred *tk_op_cred;
    struct rpc_rqst *tk_rqstp;
    struct workqueue_struct *tk_workqueue;
    ktime_t tk_start;
    pid_t tk_owner;
    short unsigned int tk_flags;
    short unsigned int tk_timeouts;
    short unsigned int tk_pid;
    unsigned char tk_priority;
    unsigned char tk_garb_retry;
    unsigned char tk_cred_retry;
    unsigned char tk_rebind_retry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rpc_task {
    atomic_t tk_count;
    int tk_status;
    struct list_head tk_task;
    void (*tk_callback)(struct rpc_task *);
    void (*tk_action)(struct rpc_task *);
    long unsigned int tk_timeout;
    long unsigned int tk_runstate;
    struct rpc_wait_queue *tk_waitqueue;
    union (anon) u;
    struct rpc_message tk_msg;
    void *tk_calldata;
    const struct rpc_call_ops *tk_ops;
    struct rpc_clnt *tk_client;
    struct rpc_xprt *tk_xprt;
    struct rpc_cred *tk_op_cred;
    struct rpc_rqst *tk_rqstp;
    struct workqueue_struct *tk_workqueue;
    ktime_t tk_start;
    pid_t tk_owner;
    int tk_rpc_status;
    short unsigned int tk_flags;
    short unsigned int tk_timeouts;
    short unsigned int tk_pid;
    unsigned char tk_priority;
    unsigned char tk_garb_retry;
    unsigned char tk_cred_retry;
    unsigned char tk_rebind_retry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rpc_task {
    atomic_t tk_count;
    int tk_status;
    struct list_head tk_task;
    void (*tk_callback)(struct rpc_task *);
    void (*tk_action)(struct rpc_task *);
    long unsigned int tk_timeout;
    long unsigned int tk_runstate;
    struct rpc_wait_queue *tk_waitqueue;
    union (anon) u;
    struct rpc_message tk_msg;
    void *tk_calldata;
    const struct rpc_call_ops *tk_ops;
    struct rpc_clnt *tk_client;
    struct rpc_xprt *tk_xprt;
    struct rpc_cred *tk_op_cred;
    struct rpc_rqst *tk_rqstp;
    struct workqueue_struct *tk_workqueue;
    ktime_t tk_start;
    pid_t tk_owner;
    int tk_rpc_status;
    short unsigned int tk_flags;
    short unsigned int tk_timeouts;
    short unsigned int tk_pid;
    unsigned char tk_priority;
    unsigned char tk_garb_retry;
    unsigned char tk_cred_retry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rpc_task {
    atomic_t tk_count;
    int tk_status;
    struct list_head tk_task;
    void (*tk_callback)(struct rpc_task *);
    void (*tk_action)(struct rpc_task *);
    long unsigned int tk_timeout;
    long unsigned int tk_runstate;
    struct rpc_wait_queue *tk_waitqueue;
    union (anon) u;
    struct rpc_message tk_msg;
    void *tk_calldata;
    const struct rpc_call_ops *tk_ops;
    struct rpc_clnt *tk_client;
    struct rpc_xprt *tk_xprt;
    struct rpc_cred *tk_op_cred;
    struct rpc_rqst *tk_rqstp;
    struct workqueue_struct *tk_workqueue;
    ktime_t tk_start;
    pid_t tk_owner;
    int tk_rpc_status;
    short unsigned int tk_flags;
    short unsigned int tk_timeouts;
    short unsigned int tk_pid;
    unsigned char tk_priority;
    unsigned char tk_garb_retry;
    unsigned char tk_cred_retry;
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
struct rpc_task {
    atomic_t tk_count;
    int tk_status;
    struct list_head tk_task;
    void (*tk_callback)(struct rpc_task *);
    void (*tk_action)(struct rpc_task *);
    long unsigned int tk_timeout;
    long unsigned int tk_runstate;
    struct rpc_wait_queue *tk_waitqueue;
    union (anon) u;
    int tk_rpc_status;
    struct rpc_message tk_msg;
    void *tk_calldata;
    const struct rpc_call_ops *tk_ops;
    struct rpc_clnt *tk_client;
    struct rpc_xprt *tk_xprt;
    struct rpc_cred *tk_op_cred;
    struct rpc_rqst *tk_rqstp;
    struct workqueue_struct *tk_workqueue;
    ktime_t tk_start;
    pid_t tk_owner;
    short unsigned int tk_flags;
    short unsigned int tk_timeouts;
    short unsigned int tk_pid;
    unsigned char tk_priority;
    unsigned char tk_garb_retry;
    unsigned char tk_cred_retry;
    unsigned char tk_rebind_retry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rpc_task {
    atomic_t tk_count;
    int tk_status;
    struct list_head tk_task;
    void (*tk_callback)(struct rpc_task *);
    void (*tk_action)(struct rpc_task *);
    long unsigned int tk_timeout;
    long unsigned int tk_runstate;
    struct rpc_wait_queue *tk_waitqueue;
    union (anon) u;
    int tk_rpc_status;
    struct rpc_message tk_msg;
    void *tk_calldata;
    const struct rpc_call_ops *tk_ops;
    struct rpc_clnt *tk_client;
    struct rpc_xprt *tk_xprt;
    struct rpc_cred *tk_op_cred;
    struct rpc_rqst *tk_rqstp;
    struct workqueue_struct *tk_workqueue;
    ktime_t tk_start;
    pid_t tk_owner;
    short unsigned int tk_flags;
    short unsigned int tk_timeouts;
    short unsigned int tk_pid;
    unsigned char tk_priority;
    unsigned char tk_garb_retry;
    unsigned char tk_cred_retry;
    unsigned char tk_rebind_retry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rpc_task {
    atomic_t tk_count;
    int tk_status;
    struct list_head tk_task;
    void (*tk_callback)(struct rpc_task *);
    void (*tk_action)(struct rpc_task *);
    long unsigned int tk_timeout;
    long unsigned int tk_runstate;
    struct rpc_wait_queue *tk_waitqueue;
    union (anon) u;
    int tk_rpc_status;
    struct rpc_message tk_msg;
    void *tk_calldata;
    const struct rpc_call_ops *tk_ops;
    struct rpc_clnt *tk_client;
    struct rpc_xprt *tk_xprt;
    struct rpc_cred *tk_op_cred;
    struct rpc_rqst *tk_rqstp;
    struct workqueue_struct *tk_workqueue;
    ktime_t tk_start;
    pid_t tk_owner;
    short unsigned int tk_flags;
    short unsigned int tk_timeouts;
    short unsigned int tk_pid;
    unsigned char tk_priority;
    unsigned char tk_garb_retry;
    unsigned char tk_cred_retry;
    unsigned char tk_rebind_retry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct rpc_task {
    atomic_t tk_count;
    int tk_status;
    struct list_head tk_task;
    void (*tk_callback)(struct rpc_task *);
    void (*tk_action)(struct rpc_task *);
    long unsigned int tk_timeout;
    long unsigned int tk_runstate;
    struct rpc_wait_queue *tk_waitqueue;
    union (anon) u;
    int tk_rpc_status;
    struct rpc_message tk_msg;
    void *tk_calldata;
    const struct rpc_call_ops *tk_ops;
    struct rpc_clnt *tk_client;
    struct rpc_xprt *tk_xprt;
    struct rpc_cred *tk_op_cred;
    struct rpc_rqst *tk_rqstp;
    struct workqueue_struct *tk_workqueue;
    ktime_t tk_start;
    pid_t tk_owner;
    short unsigned int tk_flags;
    short unsigned int tk_timeouts;
    short unsigned int tk_pid;
    unsigned char tk_priority;
    unsigned char tk_garb_retry;
    unsigned char tk_cred_retry;
    unsigned char tk_rebind_retry;
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
struct rpc_task {
    atomic_t tk_count;
    int tk_status;
    struct list_head tk_task;
    void (*tk_callback)(struct rpc_task *);
    void (*tk_action)(struct rpc_task *);
    long unsigned int tk_timeout;
    long unsigned int tk_runstate;
    struct rpc_wait_queue *tk_waitqueue;
    union (anon) u;
    int tk_rpc_status;
    struct rpc_message tk_msg;
    void *tk_calldata;
    const struct rpc_call_ops *tk_ops;
    struct rpc_clnt *tk_client;
    struct rpc_xprt *tk_xprt;
    struct rpc_cred *tk_op_cred;
    struct rpc_rqst *tk_rqstp;
    struct workqueue_struct *tk_workqueue;
    ktime_t tk_start;
    pid_t tk_owner;
    short unsigned int tk_flags;
    short unsigned int tk_timeouts;
    short unsigned int tk_pid;
    unsigned char tk_priority;
    unsigned char tk_garb_retry;
    unsigned char tk_cred_retry;
    unsigned char tk_rebind_retry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rpc_task {
    atomic_t tk_count;
    int tk_status;
    struct list_head tk_task;
    void (*tk_callback)(struct rpc_task *);
    void (*tk_action)(struct rpc_task *);
    long unsigned int tk_timeout;
    long unsigned int tk_runstate;
    struct rpc_wait_queue *tk_waitqueue;
    union (anon) u;
    int tk_rpc_status;
    struct rpc_message tk_msg;
    void *tk_calldata;
    const struct rpc_call_ops *tk_ops;
    struct rpc_clnt *tk_client;
    struct rpc_xprt *tk_xprt;
    struct rpc_cred *tk_op_cred;
    struct rpc_rqst *tk_rqstp;
    struct workqueue_struct *tk_workqueue;
    ktime_t tk_start;
    pid_t tk_owner;
    short unsigned int tk_flags;
    short unsigned int tk_timeouts;
    short unsigned int tk_pid;
    unsigned char tk_priority;
    unsigned char tk_garb_retry;
    unsigned char tk_cred_retry;
    unsigned char tk_rebind_retry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rpc_task {
    atomic_t tk_count;
    int tk_status;
    struct list_head tk_task;
    void (*tk_callback)(struct rpc_task *);
    void (*tk_action)(struct rpc_task *);
    long unsigned int tk_timeout;
    long unsigned int tk_runstate;
    struct rpc_wait_queue *tk_waitqueue;
    union (anon) u;
    int tk_rpc_status;
    struct rpc_message tk_msg;
    void *tk_calldata;
    const struct rpc_call_ops *tk_ops;
    struct rpc_clnt *tk_client;
    struct rpc_xprt *tk_xprt;
    struct rpc_cred *tk_op_cred;
    struct rpc_rqst *tk_rqstp;
    struct workqueue_struct *tk_workqueue;
    ktime_t tk_start;
    pid_t tk_owner;
    short unsigned int tk_flags;
    short unsigned int tk_timeouts;
    short unsigned int tk_pid;
    unsigned char tk_priority;
    unsigned char tk_garb_retry;
    unsigned char tk_cred_retry;
    unsigned char tk_rebind_retry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rpc_task {
    atomic_t tk_count;
    int tk_status;
    struct list_head tk_task;
    void (*tk_callback)(struct rpc_task *);
    void (*tk_action)(struct rpc_task *);
    long unsigned int tk_timeout;
    long unsigned int tk_runstate;
    struct rpc_wait_queue *tk_waitqueue;
    union (anon) u;
    int tk_rpc_status;
    struct rpc_message tk_msg;
    void *tk_calldata;
    const struct rpc_call_ops *tk_ops;
    struct rpc_clnt *tk_client;
    struct rpc_xprt *tk_xprt;
    struct rpc_cred *tk_op_cred;
    struct rpc_rqst *tk_rqstp;
    struct workqueue_struct *tk_workqueue;
    ktime_t tk_start;
    pid_t tk_owner;
    short unsigned int tk_flags;
    short unsigned int tk_timeouts;
    short unsigned int tk_pid;
    unsigned char tk_priority;
    unsigned char tk_garb_retry;
    unsigned char tk_cred_retry;
    unsigned char tk_rebind_retry;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
<b>Field added. </b>
<code>struct rpc_cred *tk_op_cred</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int tk_rpc_status</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
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
<code>unsigned char tk_rebind_retry</code>
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
