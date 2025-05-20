# Struct: <code>rpc_xprt_ops</code>

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
struct rpc_xprt_ops {
    void (*set_buffer_size)(struct rpc_xprt *, size_t, size_t);
    int (*reserve_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*release_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*alloc_slot)(struct rpc_xprt *, struct rpc_task *);
    void (*rpcbind)(struct rpc_task *);
    void (*set_port)(struct rpc_xprt *, short unsigned int);
    void (*connect)(struct rpc_xprt *, struct rpc_task *);
    void * (*buf_alloc)(struct rpc_task *, size_t);
    void (*buf_free)(void *);
    int (*send_request)(struct rpc_task *);
    void (*set_retrans_timeout)(struct rpc_task *);
    void (*timer)(struct rpc_xprt *, struct rpc_task *);
    void (*release_request)(struct rpc_task *);
    void (*close)(struct rpc_xprt *);
    void (*destroy)(struct rpc_xprt *);
    void (*print_stats)(struct rpc_xprt *, struct seq_file *);
    int (*enable_swap)(struct rpc_xprt *);
    void (*disable_swap)(struct rpc_xprt *);
    void (*inject_disconnect)(struct rpc_xprt *);
    int (*bc_setup)(struct rpc_xprt *, unsigned int);
    int (*bc_up)(struct svc_serv *, struct net *);
    size_t (*bc_maxpayload)(struct rpc_xprt *);
    void (*bc_free_rqst)(struct rpc_rqst *);
    void (*bc_destroy)(struct rpc_xprt *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rpc_xprt_ops {
    void (*set_buffer_size)(struct rpc_xprt *, size_t, size_t);
    int (*reserve_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*release_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*alloc_slot)(struct rpc_xprt *, struct rpc_task *);
    void (*rpcbind)(struct rpc_task *);
    void (*set_port)(struct rpc_xprt *, short unsigned int);
    void (*connect)(struct rpc_xprt *, struct rpc_task *);
    int (*buf_alloc)(struct rpc_task *);
    void (*buf_free)(struct rpc_task *);
    int (*send_request)(struct rpc_task *);
    void (*set_retrans_timeout)(struct rpc_task *);
    void (*timer)(struct rpc_xprt *, struct rpc_task *);
    void (*release_request)(struct rpc_task *);
    void (*close)(struct rpc_xprt *);
    void (*destroy)(struct rpc_xprt *);
    void (*print_stats)(struct rpc_xprt *, struct seq_file *);
    int (*enable_swap)(struct rpc_xprt *);
    void (*disable_swap)(struct rpc_xprt *);
    void (*inject_disconnect)(struct rpc_xprt *);
    int (*bc_setup)(struct rpc_xprt *, unsigned int);
    int (*bc_up)(struct svc_serv *, struct net *);
    size_t (*bc_maxpayload)(struct rpc_xprt *);
    void (*bc_free_rqst)(struct rpc_rqst *);
    void (*bc_destroy)(struct rpc_xprt *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rpc_xprt_ops {
    void (*set_buffer_size)(struct rpc_xprt *, size_t, size_t);
    int (*reserve_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*release_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*alloc_slot)(struct rpc_xprt *, struct rpc_task *);
    void (*rpcbind)(struct rpc_task *);
    void (*set_port)(struct rpc_xprt *, short unsigned int);
    void (*connect)(struct rpc_xprt *, struct rpc_task *);
    int (*buf_alloc)(struct rpc_task *);
    void (*buf_free)(struct rpc_task *);
    int (*send_request)(struct rpc_task *);
    void (*set_retrans_timeout)(struct rpc_task *);
    void (*timer)(struct rpc_xprt *, struct rpc_task *);
    void (*release_request)(struct rpc_task *);
    void (*close)(struct rpc_xprt *);
    void (*destroy)(struct rpc_xprt *);
    void (*set_connect_timeout)(struct rpc_xprt *, long unsigned int, long unsigned int);
    void (*print_stats)(struct rpc_xprt *, struct seq_file *);
    int (*enable_swap)(struct rpc_xprt *);
    void (*disable_swap)(struct rpc_xprt *);
    void (*inject_disconnect)(struct rpc_xprt *);
    int (*bc_setup)(struct rpc_xprt *, unsigned int);
    int (*bc_up)(struct svc_serv *, struct net *);
    size_t (*bc_maxpayload)(struct rpc_xprt *);
    void (*bc_free_rqst)(struct rpc_rqst *);
    void (*bc_destroy)(struct rpc_xprt *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rpc_xprt_ops {
    void (*set_buffer_size)(struct rpc_xprt *, size_t, size_t);
    int (*reserve_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*release_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*alloc_slot)(struct rpc_xprt *, struct rpc_task *);
    void (*rpcbind)(struct rpc_task *);
    void (*set_port)(struct rpc_xprt *, short unsigned int);
    void (*connect)(struct rpc_xprt *, struct rpc_task *);
    int (*buf_alloc)(struct rpc_task *);
    void (*buf_free)(struct rpc_task *);
    int (*send_request)(struct rpc_task *);
    void (*set_retrans_timeout)(struct rpc_task *);
    void (*timer)(struct rpc_xprt *, struct rpc_task *);
    void (*release_request)(struct rpc_task *);
    void (*close)(struct rpc_xprt *);
    void (*destroy)(struct rpc_xprt *);
    void (*set_connect_timeout)(struct rpc_xprt *, long unsigned int, long unsigned int);
    void (*print_stats)(struct rpc_xprt *, struct seq_file *);
    int (*enable_swap)(struct rpc_xprt *);
    void (*disable_swap)(struct rpc_xprt *);
    void (*inject_disconnect)(struct rpc_xprt *);
    int (*bc_setup)(struct rpc_xprt *, unsigned int);
    int (*bc_up)(struct svc_serv *, struct net *);
    size_t (*bc_maxpayload)(struct rpc_xprt *);
    void (*bc_free_rqst)(struct rpc_rqst *);
    void (*bc_destroy)(struct rpc_xprt *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rpc_xprt_ops {
    void (*set_buffer_size)(struct rpc_xprt *, size_t, size_t);
    int (*reserve_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*release_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*alloc_slot)(struct rpc_xprt *, struct rpc_task *);
    void (*free_slot)(struct rpc_xprt *, struct rpc_rqst *);
    void (*rpcbind)(struct rpc_task *);
    void (*set_port)(struct rpc_xprt *, short unsigned int);
    void (*connect)(struct rpc_xprt *, struct rpc_task *);
    int (*buf_alloc)(struct rpc_task *);
    void (*buf_free)(struct rpc_task *);
    int (*send_request)(struct rpc_task *);
    void (*set_retrans_timeout)(struct rpc_task *);
    void (*timer)(struct rpc_xprt *, struct rpc_task *);
    void (*release_request)(struct rpc_task *);
    void (*close)(struct rpc_xprt *);
    void (*destroy)(struct rpc_xprt *);
    void (*set_connect_timeout)(struct rpc_xprt *, long unsigned int, long unsigned int);
    void (*print_stats)(struct rpc_xprt *, struct seq_file *);
    int (*enable_swap)(struct rpc_xprt *);
    void (*disable_swap)(struct rpc_xprt *);
    void (*inject_disconnect)(struct rpc_xprt *);
    int (*bc_setup)(struct rpc_xprt *, unsigned int);
    int (*bc_up)(struct svc_serv *, struct net *);
    size_t (*bc_maxpayload)(struct rpc_xprt *);
    void (*bc_free_rqst)(struct rpc_rqst *);
    void (*bc_destroy)(struct rpc_xprt *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rpc_xprt_ops {
    void (*set_buffer_size)(struct rpc_xprt *, size_t, size_t);
    int (*reserve_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*release_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*alloc_slot)(struct rpc_xprt *, struct rpc_task *);
    void (*free_slot)(struct rpc_xprt *, struct rpc_rqst *);
    void (*rpcbind)(struct rpc_task *);
    void (*set_port)(struct rpc_xprt *, short unsigned int);
    void (*connect)(struct rpc_xprt *, struct rpc_task *);
    int (*buf_alloc)(struct rpc_task *);
    void (*buf_free)(struct rpc_task *);
    void (*prepare_request)(struct rpc_rqst *);
    int (*send_request)(struct rpc_rqst *);
    void (*set_retrans_timeout)(struct rpc_task *);
    void (*timer)(struct rpc_xprt *, struct rpc_task *);
    void (*release_request)(struct rpc_task *);
    void (*close)(struct rpc_xprt *);
    void (*destroy)(struct rpc_xprt *);
    void (*set_connect_timeout)(struct rpc_xprt *, long unsigned int, long unsigned int);
    void (*print_stats)(struct rpc_xprt *, struct seq_file *);
    int (*enable_swap)(struct rpc_xprt *);
    void (*disable_swap)(struct rpc_xprt *);
    void (*inject_disconnect)(struct rpc_xprt *);
    int (*bc_setup)(struct rpc_xprt *, unsigned int);
    size_t (*bc_maxpayload)(struct rpc_xprt *);
    void (*bc_free_rqst)(struct rpc_rqst *);
    void (*bc_destroy)(struct rpc_xprt *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rpc_xprt_ops {
    void (*set_buffer_size)(struct rpc_xprt *, size_t, size_t);
    int (*reserve_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*release_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*alloc_slot)(struct rpc_xprt *, struct rpc_task *);
    void (*free_slot)(struct rpc_xprt *, struct rpc_rqst *);
    void (*rpcbind)(struct rpc_task *);
    void (*set_port)(struct rpc_xprt *, short unsigned int);
    void (*connect)(struct rpc_xprt *, struct rpc_task *);
    int (*buf_alloc)(struct rpc_task *);
    void (*buf_free)(struct rpc_task *);
    void (*prepare_request)(struct rpc_rqst *);
    int (*send_request)(struct rpc_rqst *);
    void (*wait_for_reply_request)(struct rpc_task *);
    void (*timer)(struct rpc_xprt *, struct rpc_task *);
    void (*release_request)(struct rpc_task *);
    void (*close)(struct rpc_xprt *);
    void (*destroy)(struct rpc_xprt *);
    void (*set_connect_timeout)(struct rpc_xprt *, long unsigned int, long unsigned int);
    void (*print_stats)(struct rpc_xprt *, struct seq_file *);
    int (*enable_swap)(struct rpc_xprt *);
    void (*disable_swap)(struct rpc_xprt *);
    void (*inject_disconnect)(struct rpc_xprt *);
    int (*bc_setup)(struct rpc_xprt *, unsigned int);
    size_t (*bc_maxpayload)(struct rpc_xprt *);
    unsigned int (*bc_num_slots)(struct rpc_xprt *);
    void (*bc_free_rqst)(struct rpc_rqst *);
    void (*bc_destroy)(struct rpc_xprt *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rpc_xprt_ops {
    void (*set_buffer_size)(struct rpc_xprt *, size_t, size_t);
    int (*reserve_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*release_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*alloc_slot)(struct rpc_xprt *, struct rpc_task *);
    void (*free_slot)(struct rpc_xprt *, struct rpc_rqst *);
    void (*rpcbind)(struct rpc_task *);
    void (*set_port)(struct rpc_xprt *, short unsigned int);
    void (*connect)(struct rpc_xprt *, struct rpc_task *);
    int (*buf_alloc)(struct rpc_task *);
    void (*buf_free)(struct rpc_task *);
    void (*prepare_request)(struct rpc_rqst *);
    int (*send_request)(struct rpc_rqst *);
    void (*wait_for_reply_request)(struct rpc_task *);
    void (*timer)(struct rpc_xprt *, struct rpc_task *);
    void (*release_request)(struct rpc_task *);
    void (*close)(struct rpc_xprt *);
    void (*destroy)(struct rpc_xprt *);
    void (*set_connect_timeout)(struct rpc_xprt *, long unsigned int, long unsigned int);
    void (*print_stats)(struct rpc_xprt *, struct seq_file *);
    int (*enable_swap)(struct rpc_xprt *);
    void (*disable_swap)(struct rpc_xprt *);
    void (*inject_disconnect)(struct rpc_xprt *);
    int (*bc_setup)(struct rpc_xprt *, unsigned int);
    size_t (*bc_maxpayload)(struct rpc_xprt *);
    unsigned int (*bc_num_slots)(struct rpc_xprt *);
    void (*bc_free_rqst)(struct rpc_rqst *);
    void (*bc_destroy)(struct rpc_xprt *, unsigned int);
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
struct rpc_xprt_ops {
    void (*set_buffer_size)(struct rpc_xprt *, size_t, size_t);
    int (*reserve_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*release_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*alloc_slot)(struct rpc_xprt *, struct rpc_task *);
    void (*free_slot)(struct rpc_xprt *, struct rpc_rqst *);
    void (*rpcbind)(struct rpc_task *);
    void (*set_port)(struct rpc_xprt *, short unsigned int);
    void (*connect)(struct rpc_xprt *, struct rpc_task *);
    int (*buf_alloc)(struct rpc_task *);
    void (*buf_free)(struct rpc_task *);
    void (*prepare_request)(struct rpc_rqst *);
    int (*send_request)(struct rpc_rqst *);
    void (*wait_for_reply_request)(struct rpc_task *);
    void (*timer)(struct rpc_xprt *, struct rpc_task *);
    void (*release_request)(struct rpc_task *);
    void (*close)(struct rpc_xprt *);
    void (*destroy)(struct rpc_xprt *);
    void (*set_connect_timeout)(struct rpc_xprt *, long unsigned int, long unsigned int);
    void (*print_stats)(struct rpc_xprt *, struct seq_file *);
    int (*enable_swap)(struct rpc_xprt *);
    void (*disable_swap)(struct rpc_xprt *);
    void (*inject_disconnect)(struct rpc_xprt *);
    int (*bc_setup)(struct rpc_xprt *, unsigned int);
    size_t (*bc_maxpayload)(struct rpc_xprt *);
    unsigned int (*bc_num_slots)(struct rpc_xprt *);
    void (*bc_free_rqst)(struct rpc_rqst *);
    void (*bc_destroy)(struct rpc_xprt *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rpc_xprt_ops {
    void (*set_buffer_size)(struct rpc_xprt *, size_t, size_t);
    int (*reserve_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*release_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*alloc_slot)(struct rpc_xprt *, struct rpc_task *);
    void (*free_slot)(struct rpc_xprt *, struct rpc_rqst *);
    void (*rpcbind)(struct rpc_task *);
    void (*set_port)(struct rpc_xprt *, short unsigned int);
    void (*connect)(struct rpc_xprt *, struct rpc_task *);
    int (*buf_alloc)(struct rpc_task *);
    void (*buf_free)(struct rpc_task *);
    void (*prepare_request)(struct rpc_rqst *);
    int (*send_request)(struct rpc_rqst *);
    void (*wait_for_reply_request)(struct rpc_task *);
    void (*timer)(struct rpc_xprt *, struct rpc_task *);
    void (*release_request)(struct rpc_task *);
    void (*close)(struct rpc_xprt *);
    void (*destroy)(struct rpc_xprt *);
    void (*set_connect_timeout)(struct rpc_xprt *, long unsigned int, long unsigned int);
    void (*print_stats)(struct rpc_xprt *, struct seq_file *);
    int (*enable_swap)(struct rpc_xprt *);
    void (*disable_swap)(struct rpc_xprt *);
    void (*inject_disconnect)(struct rpc_xprt *);
    int (*bc_setup)(struct rpc_xprt *, unsigned int);
    size_t (*bc_maxpayload)(struct rpc_xprt *);
    unsigned int (*bc_num_slots)(struct rpc_xprt *);
    void (*bc_free_rqst)(struct rpc_rqst *);
    void (*bc_destroy)(struct rpc_xprt *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rpc_xprt_ops {
    void (*set_buffer_size)(struct rpc_xprt *, size_t, size_t);
    int (*reserve_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*release_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*alloc_slot)(struct rpc_xprt *, struct rpc_task *);
    void (*free_slot)(struct rpc_xprt *, struct rpc_rqst *);
    void (*rpcbind)(struct rpc_task *);
    void (*set_port)(struct rpc_xprt *, short unsigned int);
    void (*connect)(struct rpc_xprt *, struct rpc_task *);
    int (*get_srcaddr)(struct rpc_xprt *, char *, size_t);
    short unsigned int (*get_srcport)(struct rpc_xprt *);
    int (*buf_alloc)(struct rpc_task *);
    void (*buf_free)(struct rpc_task *);
    int (*prepare_request)(struct rpc_rqst *, struct xdr_buf *);
    int (*send_request)(struct rpc_rqst *);
    void (*wait_for_reply_request)(struct rpc_task *);
    void (*timer)(struct rpc_xprt *, struct rpc_task *);
    void (*release_request)(struct rpc_task *);
    void (*close)(struct rpc_xprt *);
    void (*destroy)(struct rpc_xprt *);
    void (*set_connect_timeout)(struct rpc_xprt *, long unsigned int, long unsigned int);
    void (*print_stats)(struct rpc_xprt *, struct seq_file *);
    int (*enable_swap)(struct rpc_xprt *);
    void (*disable_swap)(struct rpc_xprt *);
    void (*inject_disconnect)(struct rpc_xprt *);
    int (*bc_setup)(struct rpc_xprt *, unsigned int);
    size_t (*bc_maxpayload)(struct rpc_xprt *);
    unsigned int (*bc_num_slots)(struct rpc_xprt *);
    void (*bc_free_rqst)(struct rpc_rqst *);
    void (*bc_destroy)(struct rpc_xprt *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rpc_xprt_ops {
    void (*set_buffer_size)(struct rpc_xprt *, size_t, size_t);
    int (*reserve_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*release_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*alloc_slot)(struct rpc_xprt *, struct rpc_task *);
    void (*free_slot)(struct rpc_xprt *, struct rpc_rqst *);
    void (*rpcbind)(struct rpc_task *);
    void (*set_port)(struct rpc_xprt *, short unsigned int);
    void (*connect)(struct rpc_xprt *, struct rpc_task *);
    int (*get_srcaddr)(struct rpc_xprt *, char *, size_t);
    short unsigned int (*get_srcport)(struct rpc_xprt *);
    int (*buf_alloc)(struct rpc_task *);
    void (*buf_free)(struct rpc_task *);
    int (*prepare_request)(struct rpc_rqst *, struct xdr_buf *);
    int (*send_request)(struct rpc_rqst *);
    void (*wait_for_reply_request)(struct rpc_task *);
    void (*timer)(struct rpc_xprt *, struct rpc_task *);
    void (*release_request)(struct rpc_task *);
    void (*close)(struct rpc_xprt *);
    void (*destroy)(struct rpc_xprt *);
    void (*set_connect_timeout)(struct rpc_xprt *, long unsigned int, long unsigned int);
    void (*print_stats)(struct rpc_xprt *, struct seq_file *);
    int (*enable_swap)(struct rpc_xprt *);
    void (*disable_swap)(struct rpc_xprt *);
    void (*inject_disconnect)(struct rpc_xprt *);
    int (*bc_setup)(struct rpc_xprt *, unsigned int);
    size_t (*bc_maxpayload)(struct rpc_xprt *);
    unsigned int (*bc_num_slots)(struct rpc_xprt *);
    void (*bc_free_rqst)(struct rpc_rqst *);
    void (*bc_destroy)(struct rpc_xprt *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rpc_xprt_ops {
    void (*set_buffer_size)(struct rpc_xprt *, size_t, size_t);
    int (*reserve_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*release_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*alloc_slot)(struct rpc_xprt *, struct rpc_task *);
    void (*free_slot)(struct rpc_xprt *, struct rpc_rqst *);
    void (*rpcbind)(struct rpc_task *);
    void (*set_port)(struct rpc_xprt *, short unsigned int);
    void (*connect)(struct rpc_xprt *, struct rpc_task *);
    int (*get_srcaddr)(struct rpc_xprt *, char *, size_t);
    short unsigned int (*get_srcport)(struct rpc_xprt *);
    int (*buf_alloc)(struct rpc_task *);
    void (*buf_free)(struct rpc_task *);
    int (*prepare_request)(struct rpc_rqst *, struct xdr_buf *);
    int (*send_request)(struct rpc_rqst *);
    void (*wait_for_reply_request)(struct rpc_task *);
    void (*timer)(struct rpc_xprt *, struct rpc_task *);
    void (*release_request)(struct rpc_task *);
    void (*close)(struct rpc_xprt *);
    void (*destroy)(struct rpc_xprt *);
    void (*set_connect_timeout)(struct rpc_xprt *, long unsigned int, long unsigned int);
    void (*print_stats)(struct rpc_xprt *, struct seq_file *);
    int (*enable_swap)(struct rpc_xprt *);
    void (*disable_swap)(struct rpc_xprt *);
    void (*inject_disconnect)(struct rpc_xprt *);
    int (*bc_setup)(struct rpc_xprt *, unsigned int);
    size_t (*bc_maxpayload)(struct rpc_xprt *);
    unsigned int (*bc_num_slots)(struct rpc_xprt *);
    void (*bc_free_rqst)(struct rpc_rqst *);
    void (*bc_destroy)(struct rpc_xprt *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rpc_xprt_ops {
    void (*set_buffer_size)(struct rpc_xprt *, size_t, size_t);
    int (*reserve_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*release_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*alloc_slot)(struct rpc_xprt *, struct rpc_task *);
    void (*free_slot)(struct rpc_xprt *, struct rpc_rqst *);
    void (*rpcbind)(struct rpc_task *);
    void (*set_port)(struct rpc_xprt *, short unsigned int);
    void (*connect)(struct rpc_xprt *, struct rpc_task *);
    int (*get_srcaddr)(struct rpc_xprt *, char *, size_t);
    short unsigned int (*get_srcport)(struct rpc_xprt *);
    int (*buf_alloc)(struct rpc_task *);
    void (*buf_free)(struct rpc_task *);
    int (*prepare_request)(struct rpc_rqst *, struct xdr_buf *);
    int (*send_request)(struct rpc_rqst *);
    void (*wait_for_reply_request)(struct rpc_task *);
    void (*timer)(struct rpc_xprt *, struct rpc_task *);
    void (*release_request)(struct rpc_task *);
    void (*close)(struct rpc_xprt *);
    void (*destroy)(struct rpc_xprt *);
    void (*set_connect_timeout)(struct rpc_xprt *, long unsigned int, long unsigned int);
    void (*print_stats)(struct rpc_xprt *, struct seq_file *);
    int (*enable_swap)(struct rpc_xprt *);
    void (*disable_swap)(struct rpc_xprt *);
    void (*inject_disconnect)(struct rpc_xprt *);
    int (*bc_setup)(struct rpc_xprt *, unsigned int);
    size_t (*bc_maxpayload)(struct rpc_xprt *);
    unsigned int (*bc_num_slots)(struct rpc_xprt *);
    void (*bc_free_rqst)(struct rpc_rqst *);
    void (*bc_destroy)(struct rpc_xprt *, unsigned int);
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
struct rpc_xprt_ops {
    void (*set_buffer_size)(struct rpc_xprt *, size_t, size_t);
    int (*reserve_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*release_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*alloc_slot)(struct rpc_xprt *, struct rpc_task *);
    void (*free_slot)(struct rpc_xprt *, struct rpc_rqst *);
    void (*rpcbind)(struct rpc_task *);
    void (*set_port)(struct rpc_xprt *, short unsigned int);
    void (*connect)(struct rpc_xprt *, struct rpc_task *);
    int (*buf_alloc)(struct rpc_task *);
    void (*buf_free)(struct rpc_task *);
    void (*prepare_request)(struct rpc_rqst *);
    int (*send_request)(struct rpc_rqst *);
    void (*wait_for_reply_request)(struct rpc_task *);
    void (*timer)(struct rpc_xprt *, struct rpc_task *);
    void (*release_request)(struct rpc_task *);
    void (*close)(struct rpc_xprt *);
    void (*destroy)(struct rpc_xprt *);
    void (*set_connect_timeout)(struct rpc_xprt *, long unsigned int, long unsigned int);
    void (*print_stats)(struct rpc_xprt *, struct seq_file *);
    int (*enable_swap)(struct rpc_xprt *);
    void (*disable_swap)(struct rpc_xprt *);
    void (*inject_disconnect)(struct rpc_xprt *);
    int (*bc_setup)(struct rpc_xprt *, unsigned int);
    size_t (*bc_maxpayload)(struct rpc_xprt *);
    unsigned int (*bc_num_slots)(struct rpc_xprt *);
    void (*bc_free_rqst)(struct rpc_rqst *);
    void (*bc_destroy)(struct rpc_xprt *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rpc_xprt_ops {
    void (*set_buffer_size)(struct rpc_xprt *, size_t, size_t);
    int (*reserve_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*release_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*alloc_slot)(struct rpc_xprt *, struct rpc_task *);
    void (*free_slot)(struct rpc_xprt *, struct rpc_rqst *);
    void (*rpcbind)(struct rpc_task *);
    void (*set_port)(struct rpc_xprt *, short unsigned int);
    void (*connect)(struct rpc_xprt *, struct rpc_task *);
    int (*buf_alloc)(struct rpc_task *);
    void (*buf_free)(struct rpc_task *);
    void (*prepare_request)(struct rpc_rqst *);
    int (*send_request)(struct rpc_rqst *);
    void (*wait_for_reply_request)(struct rpc_task *);
    void (*timer)(struct rpc_xprt *, struct rpc_task *);
    void (*release_request)(struct rpc_task *);
    void (*close)(struct rpc_xprt *);
    void (*destroy)(struct rpc_xprt *);
    void (*set_connect_timeout)(struct rpc_xprt *, long unsigned int, long unsigned int);
    void (*print_stats)(struct rpc_xprt *, struct seq_file *);
    int (*enable_swap)(struct rpc_xprt *);
    void (*disable_swap)(struct rpc_xprt *);
    void (*inject_disconnect)(struct rpc_xprt *);
    int (*bc_setup)(struct rpc_xprt *, unsigned int);
    size_t (*bc_maxpayload)(struct rpc_xprt *);
    unsigned int (*bc_num_slots)(struct rpc_xprt *);
    void (*bc_free_rqst)(struct rpc_rqst *);
    void (*bc_destroy)(struct rpc_xprt *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rpc_xprt_ops {
    void (*set_buffer_size)(struct rpc_xprt *, size_t, size_t);
    int (*reserve_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*release_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*alloc_slot)(struct rpc_xprt *, struct rpc_task *);
    void (*free_slot)(struct rpc_xprt *, struct rpc_rqst *);
    void (*rpcbind)(struct rpc_task *);
    void (*set_port)(struct rpc_xprt *, short unsigned int);
    void (*connect)(struct rpc_xprt *, struct rpc_task *);
    int (*buf_alloc)(struct rpc_task *);
    void (*buf_free)(struct rpc_task *);
    void (*prepare_request)(struct rpc_rqst *);
    int (*send_request)(struct rpc_rqst *);
    void (*wait_for_reply_request)(struct rpc_task *);
    void (*timer)(struct rpc_xprt *, struct rpc_task *);
    void (*release_request)(struct rpc_task *);
    void (*close)(struct rpc_xprt *);
    void (*destroy)(struct rpc_xprt *);
    void (*set_connect_timeout)(struct rpc_xprt *, long unsigned int, long unsigned int);
    void (*print_stats)(struct rpc_xprt *, struct seq_file *);
    int (*enable_swap)(struct rpc_xprt *);
    void (*disable_swap)(struct rpc_xprt *);
    void (*inject_disconnect)(struct rpc_xprt *);
    int (*bc_setup)(struct rpc_xprt *, unsigned int);
    size_t (*bc_maxpayload)(struct rpc_xprt *);
    unsigned int (*bc_num_slots)(struct rpc_xprt *);
    void (*bc_free_rqst)(struct rpc_rqst *);
    void (*bc_destroy)(struct rpc_xprt *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct rpc_xprt_ops {
    void (*set_buffer_size)(struct rpc_xprt *, size_t, size_t);
    int (*reserve_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*release_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*alloc_slot)(struct rpc_xprt *, struct rpc_task *);
    void (*free_slot)(struct rpc_xprt *, struct rpc_rqst *);
    void (*rpcbind)(struct rpc_task *);
    void (*set_port)(struct rpc_xprt *, short unsigned int);
    void (*connect)(struct rpc_xprt *, struct rpc_task *);
    int (*buf_alloc)(struct rpc_task *);
    void (*buf_free)(struct rpc_task *);
    void (*prepare_request)(struct rpc_rqst *);
    int (*send_request)(struct rpc_rqst *);
    void (*wait_for_reply_request)(struct rpc_task *);
    void (*timer)(struct rpc_xprt *, struct rpc_task *);
    void (*release_request)(struct rpc_task *);
    void (*close)(struct rpc_xprt *);
    void (*destroy)(struct rpc_xprt *);
    void (*set_connect_timeout)(struct rpc_xprt *, long unsigned int, long unsigned int);
    void (*print_stats)(struct rpc_xprt *, struct seq_file *);
    int (*enable_swap)(struct rpc_xprt *);
    void (*disable_swap)(struct rpc_xprt *);
    void (*inject_disconnect)(struct rpc_xprt *);
    int (*bc_setup)(struct rpc_xprt *, unsigned int);
    size_t (*bc_maxpayload)(struct rpc_xprt *);
    unsigned int (*bc_num_slots)(struct rpc_xprt *);
    void (*bc_free_rqst)(struct rpc_rqst *);
    void (*bc_destroy)(struct rpc_xprt *, unsigned int);
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
struct rpc_xprt_ops {
    void (*set_buffer_size)(struct rpc_xprt *, size_t, size_t);
    int (*reserve_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*release_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*alloc_slot)(struct rpc_xprt *, struct rpc_task *);
    void (*free_slot)(struct rpc_xprt *, struct rpc_rqst *);
    void (*rpcbind)(struct rpc_task *);
    void (*set_port)(struct rpc_xprt *, short unsigned int);
    void (*connect)(struct rpc_xprt *, struct rpc_task *);
    int (*buf_alloc)(struct rpc_task *);
    void (*buf_free)(struct rpc_task *);
    void (*prepare_request)(struct rpc_rqst *);
    int (*send_request)(struct rpc_rqst *);
    void (*wait_for_reply_request)(struct rpc_task *);
    void (*timer)(struct rpc_xprt *, struct rpc_task *);
    void (*release_request)(struct rpc_task *);
    void (*close)(struct rpc_xprt *);
    void (*destroy)(struct rpc_xprt *);
    void (*set_connect_timeout)(struct rpc_xprt *, long unsigned int, long unsigned int);
    void (*print_stats)(struct rpc_xprt *, struct seq_file *);
    int (*enable_swap)(struct rpc_xprt *);
    void (*disable_swap)(struct rpc_xprt *);
    void (*inject_disconnect)(struct rpc_xprt *);
    int (*bc_setup)(struct rpc_xprt *, unsigned int);
    size_t (*bc_maxpayload)(struct rpc_xprt *);
    unsigned int (*bc_num_slots)(struct rpc_xprt *);
    void (*bc_free_rqst)(struct rpc_rqst *);
    void (*bc_destroy)(struct rpc_xprt *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rpc_xprt_ops {
    void (*set_buffer_size)(struct rpc_xprt *, size_t, size_t);
    int (*reserve_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*release_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*alloc_slot)(struct rpc_xprt *, struct rpc_task *);
    void (*free_slot)(struct rpc_xprt *, struct rpc_rqst *);
    void (*rpcbind)(struct rpc_task *);
    void (*set_port)(struct rpc_xprt *, short unsigned int);
    void (*connect)(struct rpc_xprt *, struct rpc_task *);
    int (*buf_alloc)(struct rpc_task *);
    void (*buf_free)(struct rpc_task *);
    void (*prepare_request)(struct rpc_rqst *);
    int (*send_request)(struct rpc_rqst *);
    void (*wait_for_reply_request)(struct rpc_task *);
    void (*timer)(struct rpc_xprt *, struct rpc_task *);
    void (*release_request)(struct rpc_task *);
    void (*close)(struct rpc_xprt *);
    void (*destroy)(struct rpc_xprt *);
    void (*set_connect_timeout)(struct rpc_xprt *, long unsigned int, long unsigned int);
    void (*print_stats)(struct rpc_xprt *, struct seq_file *);
    int (*enable_swap)(struct rpc_xprt *);
    void (*disable_swap)(struct rpc_xprt *);
    void (*inject_disconnect)(struct rpc_xprt *);
    int (*bc_setup)(struct rpc_xprt *, unsigned int);
    size_t (*bc_maxpayload)(struct rpc_xprt *);
    unsigned int (*bc_num_slots)(struct rpc_xprt *);
    void (*bc_free_rqst)(struct rpc_rqst *);
    void (*bc_destroy)(struct rpc_xprt *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rpc_xprt_ops {
    void (*set_buffer_size)(struct rpc_xprt *, size_t, size_t);
    int (*reserve_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*release_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*alloc_slot)(struct rpc_xprt *, struct rpc_task *);
    void (*free_slot)(struct rpc_xprt *, struct rpc_rqst *);
    void (*rpcbind)(struct rpc_task *);
    void (*set_port)(struct rpc_xprt *, short unsigned int);
    void (*connect)(struct rpc_xprt *, struct rpc_task *);
    int (*buf_alloc)(struct rpc_task *);
    void (*buf_free)(struct rpc_task *);
    void (*prepare_request)(struct rpc_rqst *);
    int (*send_request)(struct rpc_rqst *);
    void (*wait_for_reply_request)(struct rpc_task *);
    void (*timer)(struct rpc_xprt *, struct rpc_task *);
    void (*release_request)(struct rpc_task *);
    void (*close)(struct rpc_xprt *);
    void (*destroy)(struct rpc_xprt *);
    void (*set_connect_timeout)(struct rpc_xprt *, long unsigned int, long unsigned int);
    void (*print_stats)(struct rpc_xprt *, struct seq_file *);
    int (*enable_swap)(struct rpc_xprt *);
    void (*disable_swap)(struct rpc_xprt *);
    void (*inject_disconnect)(struct rpc_xprt *);
    int (*bc_setup)(struct rpc_xprt *, unsigned int);
    size_t (*bc_maxpayload)(struct rpc_xprt *);
    unsigned int (*bc_num_slots)(struct rpc_xprt *);
    void (*bc_free_rqst)(struct rpc_rqst *);
    void (*bc_destroy)(struct rpc_xprt *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rpc_xprt_ops {
    void (*set_buffer_size)(struct rpc_xprt *, size_t, size_t);
    int (*reserve_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*release_xprt)(struct rpc_xprt *, struct rpc_task *);
    void (*alloc_slot)(struct rpc_xprt *, struct rpc_task *);
    void (*free_slot)(struct rpc_xprt *, struct rpc_rqst *);
    void (*rpcbind)(struct rpc_task *);
    void (*set_port)(struct rpc_xprt *, short unsigned int);
    void (*connect)(struct rpc_xprt *, struct rpc_task *);
    int (*buf_alloc)(struct rpc_task *);
    void (*buf_free)(struct rpc_task *);
    void (*prepare_request)(struct rpc_rqst *);
    int (*send_request)(struct rpc_rqst *);
    void (*wait_for_reply_request)(struct rpc_task *);
    void (*timer)(struct rpc_xprt *, struct rpc_task *);
    void (*release_request)(struct rpc_task *);
    void (*close)(struct rpc_xprt *);
    void (*destroy)(struct rpc_xprt *);
    void (*set_connect_timeout)(struct rpc_xprt *, long unsigned int, long unsigned int);
    void (*print_stats)(struct rpc_xprt *, struct seq_file *);
    int (*enable_swap)(struct rpc_xprt *);
    void (*disable_swap)(struct rpc_xprt *);
    void (*inject_disconnect)(struct rpc_xprt *);
    int (*bc_setup)(struct rpc_xprt *, unsigned int);
    size_t (*bc_maxpayload)(struct rpc_xprt *);
    unsigned int (*bc_num_slots)(struct rpc_xprt *);
    void (*bc_free_rqst)(struct rpc_rqst *);
    void (*bc_destroy)(struct rpc_xprt *, unsigned int);
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
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>void * (*buf_alloc)(struct rpc_task *, size_t)</code> ➡️ <code>int (*buf_alloc)(struct rpc_task *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*buf_free)(void *)</code> ➡️ <code>void (*buf_free)(struct rpc_task *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*set_connect_timeout)(struct rpc_xprt *, long unsigned int, long unsigned int)</code>
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
<b>Field added. </b>
<code>void (*free_slot)(struct rpc_xprt *, struct rpc_rqst *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*prepare_request)(struct rpc_rqst *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*bc_up)(struct svc_serv *, struct net *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*send_request)(struct rpc_task *)</code> ➡️ <code>int (*send_request)(struct rpc_rqst *)</code>
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
<code>void (*wait_for_reply_request)(struct rpc_task *)</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int (*bc_num_slots)(struct rpc_xprt *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*set_retrans_timeout)(struct rpc_task *)</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*get_srcaddr)(struct rpc_xprt *, char *, size_t)</code>
</li>
<li>
<b>Field added. </b>
<code>short unsigned int (*get_srcport)(struct rpc_xprt *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*prepare_request)(struct rpc_rqst *)</code> ➡️ <code>int (*prepare_request)(struct rpc_rqst *, struct xdr_buf *)</code>
</li>
</ul>
</details>
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
