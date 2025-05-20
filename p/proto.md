# Struct: <code>proto</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct proto {
    void (*close)(struct sock *, long int);
    int (*connect)(struct sock *, struct sockaddr *, int);
    int (*disconnect)(struct sock *, int);
    struct sock * (*accept)(struct sock *, int, int *);
    int (*ioctl)(struct sock *, int, long unsigned int);
    int (*init)(struct sock *);
    void (*destroy)(struct sock *);
    void (*shutdown)(struct sock *, int);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_ioctl)(struct sock *, unsigned int, long unsigned int);
    int (*sendmsg)(struct sock *, struct msghdr *, size_t);
    int (*recvmsg)(struct sock *, struct msghdr *, size_t, int, int, int *);
    int (*sendpage)(struct sock *, struct page *, int, size_t, int);
    int (*bind)(struct sock *, struct sockaddr *, int);
    int (*backlog_rcv)(struct sock *, struct sk_buff *);
    void (*release_cb)(struct sock *);
    void (*hash)(struct sock *);
    void (*unhash)(struct sock *);
    void (*rehash)(struct sock *);
    int (*get_port)(struct sock *, short unsigned int);
    void (*clear_sk)(struct sock *, int);
    unsigned int inuse_idx;
    bool (*stream_memory_free)(const struct sock *);
    void (*enter_memory_pressure)(struct sock *);
    atomic_long_t *memory_allocated;
    struct percpu_counter *sockets_allocated;
    int *memory_pressure;
    long int *sysctl_mem;
    int *sysctl_wmem;
    int *sysctl_rmem;
    int max_header;
    bool no_autobind;
    struct kmem_cache *slab;
    unsigned int obj_size;
    int slab_flags;
    struct percpu_counter *orphan_count;
    struct request_sock_ops *rsk_prot;
    struct timewait_sock_ops *twsk_prot;
    union (anon) h;
    struct module *owner;
    char name[32];
    struct list_head node;
    int (*init_cgroup)(struct mem_cgroup *, struct cgroup_subsys *);
    void (*destroy_cgroup)(struct mem_cgroup *);
    struct cg_proto * (*proto_cgroup)(struct mem_cgroup *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct proto {
    void (*close)(struct sock *, long int);
    int (*connect)(struct sock *, struct sockaddr *, int);
    int (*disconnect)(struct sock *, int);
    struct sock * (*accept)(struct sock *, int, int *);
    int (*ioctl)(struct sock *, int, long unsigned int);
    int (*init)(struct sock *);
    void (*destroy)(struct sock *);
    void (*shutdown)(struct sock *, int);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_ioctl)(struct sock *, unsigned int, long unsigned int);
    int (*sendmsg)(struct sock *, struct msghdr *, size_t);
    int (*recvmsg)(struct sock *, struct msghdr *, size_t, int, int, int *);
    int (*sendpage)(struct sock *, struct page *, int, size_t, int);
    int (*bind)(struct sock *, struct sockaddr *, int);
    int (*backlog_rcv)(struct sock *, struct sk_buff *);
    void (*release_cb)(struct sock *);
    int (*hash)(struct sock *);
    void (*unhash)(struct sock *);
    void (*rehash)(struct sock *);
    int (*get_port)(struct sock *, short unsigned int);
    void (*clear_sk)(struct sock *, int);
    unsigned int inuse_idx;
    bool (*stream_memory_free)(const struct sock *);
    void (*enter_memory_pressure)(struct sock *);
    atomic_long_t *memory_allocated;
    struct percpu_counter *sockets_allocated;
    int *memory_pressure;
    long int *sysctl_mem;
    int *sysctl_wmem;
    int *sysctl_rmem;
    int max_header;
    bool no_autobind;
    struct kmem_cache *slab;
    unsigned int obj_size;
    int slab_flags;
    struct percpu_counter *orphan_count;
    struct request_sock_ops *rsk_prot;
    struct timewait_sock_ops *twsk_prot;
    union (anon) h;
    struct module *owner;
    char name[32];
    struct list_head node;
    int (*diag_destroy)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct proto {
    void (*close)(struct sock *, long int);
    int (*connect)(struct sock *, struct sockaddr *, int);
    int (*disconnect)(struct sock *, int);
    struct sock * (*accept)(struct sock *, int, int *);
    int (*ioctl)(struct sock *, int, long unsigned int);
    int (*init)(struct sock *);
    void (*destroy)(struct sock *);
    void (*shutdown)(struct sock *, int);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_ioctl)(struct sock *, unsigned int, long unsigned int);
    int (*sendmsg)(struct sock *, struct msghdr *, size_t);
    int (*recvmsg)(struct sock *, struct msghdr *, size_t, int, int, int *);
    int (*sendpage)(struct sock *, struct page *, int, size_t, int);
    int (*bind)(struct sock *, struct sockaddr *, int);
    int (*backlog_rcv)(struct sock *, struct sk_buff *);
    void (*release_cb)(struct sock *);
    int (*hash)(struct sock *);
    void (*unhash)(struct sock *);
    void (*rehash)(struct sock *);
    int (*get_port)(struct sock *, short unsigned int);
    unsigned int inuse_idx;
    bool (*stream_memory_free)(const struct sock *);
    void (*enter_memory_pressure)(struct sock *);
    atomic_long_t *memory_allocated;
    struct percpu_counter *sockets_allocated;
    int *memory_pressure;
    long int *sysctl_mem;
    int *sysctl_wmem;
    int *sysctl_rmem;
    int max_header;
    bool no_autobind;
    struct kmem_cache *slab;
    unsigned int obj_size;
    int slab_flags;
    struct percpu_counter *orphan_count;
    struct request_sock_ops *rsk_prot;
    struct timewait_sock_ops *twsk_prot;
    union (anon) h;
    struct module *owner;
    char name[32];
    struct list_head node;
    int (*diag_destroy)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct proto {
    void (*close)(struct sock *, long int);
    int (*connect)(struct sock *, struct sockaddr *, int);
    int (*disconnect)(struct sock *, int);
    struct sock * (*accept)(struct sock *, int, int *, bool);
    int (*ioctl)(struct sock *, int, long unsigned int);
    int (*init)(struct sock *);
    void (*destroy)(struct sock *);
    void (*shutdown)(struct sock *, int);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*keepalive)(struct sock *, int);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_ioctl)(struct sock *, unsigned int, long unsigned int);
    int (*sendmsg)(struct sock *, struct msghdr *, size_t);
    int (*recvmsg)(struct sock *, struct msghdr *, size_t, int, int, int *);
    int (*sendpage)(struct sock *, struct page *, int, size_t, int);
    int (*bind)(struct sock *, struct sockaddr *, int);
    int (*backlog_rcv)(struct sock *, struct sk_buff *);
    void (*release_cb)(struct sock *);
    int (*hash)(struct sock *);
    void (*unhash)(struct sock *);
    void (*rehash)(struct sock *);
    int (*get_port)(struct sock *, short unsigned int);
    unsigned int inuse_idx;
    bool (*stream_memory_free)(const struct sock *);
    void (*enter_memory_pressure)(struct sock *);
    void (*leave_memory_pressure)(struct sock *);
    atomic_long_t *memory_allocated;
    struct percpu_counter *sockets_allocated;
    long unsigned int *memory_pressure;
    long int *sysctl_mem;
    int *sysctl_wmem;
    int *sysctl_rmem;
    int max_header;
    bool no_autobind;
    struct kmem_cache *slab;
    unsigned int obj_size;
    int slab_flags;
    struct percpu_counter *orphan_count;
    struct request_sock_ops *rsk_prot;
    struct timewait_sock_ops *twsk_prot;
    union (anon) h;
    struct module *owner;
    char name[32];
    struct list_head node;
    int (*diag_destroy)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct proto {
    void (*close)(struct sock *, long int);
    int (*connect)(struct sock *, struct sockaddr *, int);
    int (*disconnect)(struct sock *, int);
    struct sock * (*accept)(struct sock *, int, int *, bool);
    int (*ioctl)(struct sock *, int, long unsigned int);
    int (*init)(struct sock *);
    void (*destroy)(struct sock *);
    void (*shutdown)(struct sock *, int);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*keepalive)(struct sock *, int);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_ioctl)(struct sock *, unsigned int, long unsigned int);
    int (*sendmsg)(struct sock *, struct msghdr *, size_t);
    int (*recvmsg)(struct sock *, struct msghdr *, size_t, int, int, int *);
    int (*sendpage)(struct sock *, struct page *, int, size_t, int);
    int (*bind)(struct sock *, struct sockaddr *, int);
    int (*backlog_rcv)(struct sock *, struct sk_buff *);
    void (*release_cb)(struct sock *);
    int (*hash)(struct sock *);
    void (*unhash)(struct sock *);
    void (*rehash)(struct sock *);
    int (*get_port)(struct sock *, short unsigned int);
    unsigned int inuse_idx;
    bool (*stream_memory_free)(const struct sock *);
    void (*enter_memory_pressure)(struct sock *);
    void (*leave_memory_pressure)(struct sock *);
    atomic_long_t *memory_allocated;
    struct percpu_counter *sockets_allocated;
    long unsigned int *memory_pressure;
    long int *sysctl_mem;
    int *sysctl_wmem;
    int *sysctl_rmem;
    u32 sysctl_wmem_offset;
    u32 sysctl_rmem_offset;
    int max_header;
    bool no_autobind;
    struct kmem_cache *slab;
    unsigned int obj_size;
    slab_flags_t slab_flags;
    struct percpu_counter *orphan_count;
    struct request_sock_ops *rsk_prot;
    struct timewait_sock_ops *twsk_prot;
    union (anon) h;
    struct module *owner;
    char name[32];
    struct list_head node;
    int (*diag_destroy)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct proto {
    void (*close)(struct sock *, long int);
    int (*pre_connect)(struct sock *, struct sockaddr *, int);
    int (*connect)(struct sock *, struct sockaddr *, int);
    int (*disconnect)(struct sock *, int);
    struct sock * (*accept)(struct sock *, int, int *, bool);
    int (*ioctl)(struct sock *, int, long unsigned int);
    int (*init)(struct sock *);
    void (*destroy)(struct sock *);
    void (*shutdown)(struct sock *, int);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*keepalive)(struct sock *, int);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_ioctl)(struct sock *, unsigned int, long unsigned int);
    int (*sendmsg)(struct sock *, struct msghdr *, size_t);
    int (*recvmsg)(struct sock *, struct msghdr *, size_t, int, int, int *);
    int (*sendpage)(struct sock *, struct page *, int, size_t, int);
    int (*bind)(struct sock *, struct sockaddr *, int);
    int (*backlog_rcv)(struct sock *, struct sk_buff *);
    void (*release_cb)(struct sock *);
    int (*hash)(struct sock *);
    void (*unhash)(struct sock *);
    void (*rehash)(struct sock *);
    int (*get_port)(struct sock *, short unsigned int);
    unsigned int inuse_idx;
    bool (*stream_memory_free)(const struct sock *);
    bool (*stream_memory_read)(const struct sock *);
    void (*enter_memory_pressure)(struct sock *);
    void (*leave_memory_pressure)(struct sock *);
    atomic_long_t *memory_allocated;
    struct percpu_counter *sockets_allocated;
    long unsigned int *memory_pressure;
    long int *sysctl_mem;
    int *sysctl_wmem;
    int *sysctl_rmem;
    u32 sysctl_wmem_offset;
    u32 sysctl_rmem_offset;
    int max_header;
    bool no_autobind;
    struct kmem_cache *slab;
    unsigned int obj_size;
    slab_flags_t slab_flags;
    unsigned int useroffset;
    unsigned int usersize;
    struct percpu_counter *orphan_count;
    struct request_sock_ops *rsk_prot;
    struct timewait_sock_ops *twsk_prot;
    union (anon) h;
    struct module *owner;
    char name[32];
    struct list_head node;
    int (*diag_destroy)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct proto {
    void (*close)(struct sock *, long int);
    int (*pre_connect)(struct sock *, struct sockaddr *, int);
    int (*connect)(struct sock *, struct sockaddr *, int);
    int (*disconnect)(struct sock *, int);
    struct sock * (*accept)(struct sock *, int, int *, bool);
    int (*ioctl)(struct sock *, int, long unsigned int);
    int (*init)(struct sock *);
    void (*destroy)(struct sock *);
    void (*shutdown)(struct sock *, int);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*keepalive)(struct sock *, int);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_ioctl)(struct sock *, unsigned int, long unsigned int);
    int (*sendmsg)(struct sock *, struct msghdr *, size_t);
    int (*recvmsg)(struct sock *, struct msghdr *, size_t, int, int, int *);
    int (*sendpage)(struct sock *, struct page *, int, size_t, int);
    int (*bind)(struct sock *, struct sockaddr *, int);
    int (*backlog_rcv)(struct sock *, struct sk_buff *);
    void (*release_cb)(struct sock *);
    int (*hash)(struct sock *);
    void (*unhash)(struct sock *);
    void (*rehash)(struct sock *);
    int (*get_port)(struct sock *, short unsigned int);
    unsigned int inuse_idx;
    bool (*stream_memory_free)(const struct sock *, int);
    bool (*stream_memory_read)(const struct sock *);
    void (*enter_memory_pressure)(struct sock *);
    void (*leave_memory_pressure)(struct sock *);
    atomic_long_t *memory_allocated;
    struct percpu_counter *sockets_allocated;
    long unsigned int *memory_pressure;
    long int *sysctl_mem;
    int *sysctl_wmem;
    int *sysctl_rmem;
    u32 sysctl_wmem_offset;
    u32 sysctl_rmem_offset;
    int max_header;
    bool no_autobind;
    struct kmem_cache *slab;
    unsigned int obj_size;
    slab_flags_t slab_flags;
    unsigned int useroffset;
    unsigned int usersize;
    struct percpu_counter *orphan_count;
    struct request_sock_ops *rsk_prot;
    struct timewait_sock_ops *twsk_prot;
    union (anon) h;
    struct module *owner;
    char name[32];
    struct list_head node;
    int (*diag_destroy)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct proto {
    void (*close)(struct sock *, long int);
    int (*pre_connect)(struct sock *, struct sockaddr *, int);
    int (*connect)(struct sock *, struct sockaddr *, int);
    int (*disconnect)(struct sock *, int);
    struct sock * (*accept)(struct sock *, int, int *, bool);
    int (*ioctl)(struct sock *, int, long unsigned int);
    int (*init)(struct sock *);
    void (*destroy)(struct sock *);
    void (*shutdown)(struct sock *, int);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*keepalive)(struct sock *, int);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_ioctl)(struct sock *, unsigned int, long unsigned int);
    int (*sendmsg)(struct sock *, struct msghdr *, size_t);
    int (*recvmsg)(struct sock *, struct msghdr *, size_t, int, int, int *);
    int (*sendpage)(struct sock *, struct page *, int, size_t, int);
    int (*bind)(struct sock *, struct sockaddr *, int);
    int (*backlog_rcv)(struct sock *, struct sk_buff *);
    void (*release_cb)(struct sock *);
    int (*hash)(struct sock *);
    void (*unhash)(struct sock *);
    void (*rehash)(struct sock *);
    int (*get_port)(struct sock *, short unsigned int);
    unsigned int inuse_idx;
    bool (*stream_memory_free)(const struct sock *, int);
    bool (*stream_memory_read)(const struct sock *);
    void (*enter_memory_pressure)(struct sock *);
    void (*leave_memory_pressure)(struct sock *);
    atomic_long_t *memory_allocated;
    struct percpu_counter *sockets_allocated;
    long unsigned int *memory_pressure;
    long int *sysctl_mem;
    int *sysctl_wmem;
    int *sysctl_rmem;
    u32 sysctl_wmem_offset;
    u32 sysctl_rmem_offset;
    int max_header;
    bool no_autobind;
    struct kmem_cache *slab;
    unsigned int obj_size;
    slab_flags_t slab_flags;
    unsigned int useroffset;
    unsigned int usersize;
    struct percpu_counter *orphan_count;
    struct request_sock_ops *rsk_prot;
    struct timewait_sock_ops *twsk_prot;
    union (anon) h;
    struct module *owner;
    char name[32];
    struct list_head node;
    int (*diag_destroy)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct proto {
    void (*close)(struct sock *, long int);
    int (*pre_connect)(struct sock *, struct sockaddr *, int);
    int (*connect)(struct sock *, struct sockaddr *, int);
    int (*disconnect)(struct sock *, int);
    struct sock * (*accept)(struct sock *, int, int *, bool);
    int (*ioctl)(struct sock *, int, long unsigned int);
    int (*init)(struct sock *);
    void (*destroy)(struct sock *);
    void (*shutdown)(struct sock *, int);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*keepalive)(struct sock *, int);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_ioctl)(struct sock *, unsigned int, long unsigned int);
    int (*sendmsg)(struct sock *, struct msghdr *, size_t);
    int (*recvmsg)(struct sock *, struct msghdr *, size_t, int, int, int *);
    int (*sendpage)(struct sock *, struct page *, int, size_t, int);
    int (*bind)(struct sock *, struct sockaddr *, int);
    int (*backlog_rcv)(struct sock *, struct sk_buff *);
    void (*release_cb)(struct sock *);
    int (*hash)(struct sock *);
    void (*unhash)(struct sock *);
    void (*rehash)(struct sock *);
    int (*get_port)(struct sock *, short unsigned int);
    unsigned int inuse_idx;
    bool (*stream_memory_free)(const struct sock *, int);
    bool (*stream_memory_read)(const struct sock *);
    void (*enter_memory_pressure)(struct sock *);
    void (*leave_memory_pressure)(struct sock *);
    atomic_long_t *memory_allocated;
    struct percpu_counter *sockets_allocated;
    long unsigned int *memory_pressure;
    long int *sysctl_mem;
    int *sysctl_wmem;
    int *sysctl_rmem;
    u32 sysctl_wmem_offset;
    u32 sysctl_rmem_offset;
    int max_header;
    bool no_autobind;
    struct kmem_cache *slab;
    unsigned int obj_size;
    slab_flags_t slab_flags;
    unsigned int useroffset;
    unsigned int usersize;
    struct percpu_counter *orphan_count;
    struct request_sock_ops *rsk_prot;
    struct timewait_sock_ops *twsk_prot;
    union (anon) h;
    struct module *owner;
    char name[32];
    struct list_head node;
    int (*diag_destroy)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct proto {
    void (*close)(struct sock *, long int);
    int (*pre_connect)(struct sock *, struct sockaddr *, int);
    int (*connect)(struct sock *, struct sockaddr *, int);
    int (*disconnect)(struct sock *, int);
    struct sock * (*accept)(struct sock *, int, int *, bool);
    int (*ioctl)(struct sock *, int, long unsigned int);
    int (*init)(struct sock *);
    void (*destroy)(struct sock *);
    void (*shutdown)(struct sock *, int);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*keepalive)(struct sock *, int);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_ioctl)(struct sock *, unsigned int, long unsigned int);
    int (*sendmsg)(struct sock *, struct msghdr *, size_t);
    int (*recvmsg)(struct sock *, struct msghdr *, size_t, int, int, int *);
    int (*sendpage)(struct sock *, struct page *, int, size_t, int);
    int (*bind)(struct sock *, struct sockaddr *, int);
    int (*bind_add)(struct sock *, struct sockaddr *, int);
    int (*backlog_rcv)(struct sock *, struct sk_buff *);
    void (*release_cb)(struct sock *);
    int (*hash)(struct sock *);
    void (*unhash)(struct sock *);
    void (*rehash)(struct sock *);
    int (*get_port)(struct sock *, short unsigned int);
    unsigned int inuse_idx;
    bool (*stream_memory_free)(const struct sock *, int);
    bool (*stream_memory_read)(const struct sock *);
    void (*enter_memory_pressure)(struct sock *);
    void (*leave_memory_pressure)(struct sock *);
    atomic_long_t *memory_allocated;
    struct percpu_counter *sockets_allocated;
    long unsigned int *memory_pressure;
    long int *sysctl_mem;
    int *sysctl_wmem;
    int *sysctl_rmem;
    u32 sysctl_wmem_offset;
    u32 sysctl_rmem_offset;
    int max_header;
    bool no_autobind;
    struct kmem_cache *slab;
    unsigned int obj_size;
    slab_flags_t slab_flags;
    unsigned int useroffset;
    unsigned int usersize;
    struct percpu_counter *orphan_count;
    struct request_sock_ops *rsk_prot;
    struct timewait_sock_ops *twsk_prot;
    union (anon) h;
    struct module *owner;
    char name[32];
    struct list_head node;
    int (*diag_destroy)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct proto {
    void (*close)(struct sock *, long int);
    int (*pre_connect)(struct sock *, struct sockaddr *, int);
    int (*connect)(struct sock *, struct sockaddr *, int);
    int (*disconnect)(struct sock *, int);
    struct sock * (*accept)(struct sock *, int, int *, bool);
    int (*ioctl)(struct sock *, int, long unsigned int);
    int (*init)(struct sock *);
    void (*destroy)(struct sock *);
    void (*shutdown)(struct sock *, int);
    int (*setsockopt)(struct sock *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*keepalive)(struct sock *, int);
    int (*compat_ioctl)(struct sock *, unsigned int, long unsigned int);
    int (*sendmsg)(struct sock *, struct msghdr *, size_t);
    int (*recvmsg)(struct sock *, struct msghdr *, size_t, int, int, int *);
    int (*sendpage)(struct sock *, struct page *, int, size_t, int);
    int (*bind)(struct sock *, struct sockaddr *, int);
    int (*bind_add)(struct sock *, struct sockaddr *, int);
    int (*backlog_rcv)(struct sock *, struct sk_buff *);
    void (*release_cb)(struct sock *);
    int (*hash)(struct sock *);
    void (*unhash)(struct sock *);
    void (*rehash)(struct sock *);
    int (*get_port)(struct sock *, short unsigned int);
    unsigned int inuse_idx;
    bool (*stream_memory_free)(const struct sock *, int);
    bool (*stream_memory_read)(const struct sock *);
    void (*enter_memory_pressure)(struct sock *);
    void (*leave_memory_pressure)(struct sock *);
    atomic_long_t *memory_allocated;
    struct percpu_counter *sockets_allocated;
    long unsigned int *memory_pressure;
    long int *sysctl_mem;
    int *sysctl_wmem;
    int *sysctl_rmem;
    u32 sysctl_wmem_offset;
    u32 sysctl_rmem_offset;
    int max_header;
    bool no_autobind;
    struct kmem_cache *slab;
    unsigned int obj_size;
    slab_flags_t slab_flags;
    unsigned int useroffset;
    unsigned int usersize;
    struct percpu_counter *orphan_count;
    struct request_sock_ops *rsk_prot;
    struct timewait_sock_ops *twsk_prot;
    union (anon) h;
    struct module *owner;
    char name[32];
    struct list_head node;
    int (*diag_destroy)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct proto {
    void (*close)(struct sock *, long int);
    int (*pre_connect)(struct sock *, struct sockaddr *, int);
    int (*connect)(struct sock *, struct sockaddr *, int);
    int (*disconnect)(struct sock *, int);
    struct sock * (*accept)(struct sock *, int, int *, bool);
    int (*ioctl)(struct sock *, int, long unsigned int);
    int (*init)(struct sock *);
    void (*destroy)(struct sock *);
    void (*shutdown)(struct sock *, int);
    int (*setsockopt)(struct sock *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*keepalive)(struct sock *, int);
    int (*compat_ioctl)(struct sock *, unsigned int, long unsigned int);
    int (*sendmsg)(struct sock *, struct msghdr *, size_t);
    int (*recvmsg)(struct sock *, struct msghdr *, size_t, int, int, int *);
    int (*sendpage)(struct sock *, struct page *, int, size_t, int);
    int (*bind)(struct sock *, struct sockaddr *, int);
    int (*bind_add)(struct sock *, struct sockaddr *, int);
    int (*backlog_rcv)(struct sock *, struct sk_buff *);
    bool (*bpf_bypass_getsockopt)(int, int);
    void (*release_cb)(struct sock *);
    int (*hash)(struct sock *);
    void (*unhash)(struct sock *);
    void (*rehash)(struct sock *);
    int (*get_port)(struct sock *, short unsigned int);
    int (*psock_update_sk_prot)(struct sock *, struct sk_psock *, bool);
    unsigned int inuse_idx;
    bool (*stream_memory_free)(const struct sock *, int);
    bool (*stream_memory_read)(const struct sock *);
    void (*enter_memory_pressure)(struct sock *);
    void (*leave_memory_pressure)(struct sock *);
    atomic_long_t *memory_allocated;
    struct percpu_counter *sockets_allocated;
    long unsigned int *memory_pressure;
    long int *sysctl_mem;
    int *sysctl_wmem;
    int *sysctl_rmem;
    u32 sysctl_wmem_offset;
    u32 sysctl_rmem_offset;
    int max_header;
    bool no_autobind;
    struct kmem_cache *slab;
    unsigned int obj_size;
    slab_flags_t slab_flags;
    unsigned int useroffset;
    unsigned int usersize;
    struct percpu_counter *orphan_count;
    struct request_sock_ops *rsk_prot;
    struct timewait_sock_ops *twsk_prot;
    union (anon) h;
    struct module *owner;
    char name[32];
    struct list_head node;
    int (*diag_destroy)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct proto {
    void (*close)(struct sock *, long int);
    int (*pre_connect)(struct sock *, struct sockaddr *, int);
    int (*connect)(struct sock *, struct sockaddr *, int);
    int (*disconnect)(struct sock *, int);
    struct sock * (*accept)(struct sock *, int, int *, bool);
    int (*ioctl)(struct sock *, int, long unsigned int);
    int (*init)(struct sock *);
    void (*destroy)(struct sock *);
    void (*shutdown)(struct sock *, int);
    int (*setsockopt)(struct sock *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*keepalive)(struct sock *, int);
    int (*compat_ioctl)(struct sock *, unsigned int, long unsigned int);
    int (*sendmsg)(struct sock *, struct msghdr *, size_t);
    int (*recvmsg)(struct sock *, struct msghdr *, size_t, int, int, int *);
    int (*sendpage)(struct sock *, struct page *, int, size_t, int);
    int (*bind)(struct sock *, struct sockaddr *, int);
    int (*bind_add)(struct sock *, struct sockaddr *, int);
    int (*backlog_rcv)(struct sock *, struct sk_buff *);
    bool (*bpf_bypass_getsockopt)(int, int);
    void (*release_cb)(struct sock *);
    int (*hash)(struct sock *);
    void (*unhash)(struct sock *);
    void (*rehash)(struct sock *);
    int (*get_port)(struct sock *, short unsigned int);
    int (*psock_update_sk_prot)(struct sock *, struct sk_psock *, bool);
    unsigned int inuse_idx;
    bool (*stream_memory_free)(const struct sock *, int);
    bool (*sock_is_readable)(struct sock *);
    void (*enter_memory_pressure)(struct sock *);
    void (*leave_memory_pressure)(struct sock *);
    atomic_long_t *memory_allocated;
    struct percpu_counter *sockets_allocated;
    long unsigned int *memory_pressure;
    long int *sysctl_mem;
    int *sysctl_wmem;
    int *sysctl_rmem;
    u32 sysctl_wmem_offset;
    u32 sysctl_rmem_offset;
    int max_header;
    bool no_autobind;
    struct kmem_cache *slab;
    unsigned int obj_size;
    slab_flags_t slab_flags;
    unsigned int useroffset;
    unsigned int usersize;
    unsigned int *orphan_count;
    struct request_sock_ops *rsk_prot;
    struct timewait_sock_ops *twsk_prot;
    union (anon) h;
    struct module *owner;
    char name[32];
    struct list_head node;
    int (*diag_destroy)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct proto {
    void (*close)(struct sock *, long int);
    int (*pre_connect)(struct sock *, struct sockaddr *, int);
    int (*connect)(struct sock *, struct sockaddr *, int);
    int (*disconnect)(struct sock *, int);
    struct sock * (*accept)(struct sock *, int, int *, bool);
    int (*ioctl)(struct sock *, int, long unsigned int);
    int (*init)(struct sock *);
    void (*destroy)(struct sock *);
    void (*shutdown)(struct sock *, int);
    int (*setsockopt)(struct sock *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*keepalive)(struct sock *, int);
    int (*compat_ioctl)(struct sock *, unsigned int, long unsigned int);
    int (*sendmsg)(struct sock *, struct msghdr *, size_t);
    int (*recvmsg)(struct sock *, struct msghdr *, size_t, int, int *);
    int (*sendpage)(struct sock *, struct page *, int, size_t, int);
    int (*bind)(struct sock *, struct sockaddr *, int);
    int (*bind_add)(struct sock *, struct sockaddr *, int);
    int (*backlog_rcv)(struct sock *, struct sk_buff *);
    bool (*bpf_bypass_getsockopt)(int, int);
    void (*release_cb)(struct sock *);
    int (*hash)(struct sock *);
    void (*unhash)(struct sock *);
    void (*rehash)(struct sock *);
    int (*get_port)(struct sock *, short unsigned int);
    void (*put_port)(struct sock *);
    int (*psock_update_sk_prot)(struct sock *, struct sk_psock *, bool);
    unsigned int inuse_idx;
    int (*forward_alloc_get)(const struct sock *);
    bool (*stream_memory_free)(const struct sock *, int);
    bool (*sock_is_readable)(struct sock *);
    void (*enter_memory_pressure)(struct sock *);
    void (*leave_memory_pressure)(struct sock *);
    atomic_long_t *memory_allocated;
    struct percpu_counter *sockets_allocated;
    long unsigned int *memory_pressure;
    long int *sysctl_mem;
    int *sysctl_wmem;
    int *sysctl_rmem;
    u32 sysctl_wmem_offset;
    u32 sysctl_rmem_offset;
    int max_header;
    bool no_autobind;
    struct kmem_cache *slab;
    unsigned int obj_size;
    slab_flags_t slab_flags;
    unsigned int useroffset;
    unsigned int usersize;
    unsigned int *orphan_count;
    struct request_sock_ops *rsk_prot;
    struct timewait_sock_ops *twsk_prot;
    union (anon) h;
    struct module *owner;
    char name[32];
    struct list_head node;
    int (*diag_destroy)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct proto {
    void (*close)(struct sock *, long int);
    int (*pre_connect)(struct sock *, struct sockaddr *, int);
    int (*connect)(struct sock *, struct sockaddr *, int);
    int (*disconnect)(struct sock *, int);
    struct sock * (*accept)(struct sock *, int, int *, bool);
    int (*ioctl)(struct sock *, int, long unsigned int);
    int (*init)(struct sock *);
    void (*destroy)(struct sock *);
    void (*shutdown)(struct sock *, int);
    int (*setsockopt)(struct sock *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*keepalive)(struct sock *, int);
    int (*compat_ioctl)(struct sock *, unsigned int, long unsigned int);
    int (*sendmsg)(struct sock *, struct msghdr *, size_t);
    int (*recvmsg)(struct sock *, struct msghdr *, size_t, int, int *);
    int (*sendpage)(struct sock *, struct page *, int, size_t, int);
    int (*bind)(struct sock *, struct sockaddr *, int);
    int (*bind_add)(struct sock *, struct sockaddr *, int);
    int (*backlog_rcv)(struct sock *, struct sk_buff *);
    bool (*bpf_bypass_getsockopt)(int, int);
    void (*release_cb)(struct sock *);
    int (*hash)(struct sock *);
    void (*unhash)(struct sock *);
    void (*rehash)(struct sock *);
    int (*get_port)(struct sock *, short unsigned int);
    void (*put_port)(struct sock *);
    int (*psock_update_sk_prot)(struct sock *, struct sk_psock *, bool);
    unsigned int inuse_idx;
    int (*forward_alloc_get)(const struct sock *);
    bool (*stream_memory_free)(const struct sock *, int);
    bool (*sock_is_readable)(struct sock *);
    void (*enter_memory_pressure)(struct sock *);
    void (*leave_memory_pressure)(struct sock *);
    atomic_long_t *memory_allocated;
    int *per_cpu_fw_alloc;
    struct percpu_counter *sockets_allocated;
    long unsigned int *memory_pressure;
    long int *sysctl_mem;
    int *sysctl_wmem;
    int *sysctl_rmem;
    u32 sysctl_wmem_offset;
    u32 sysctl_rmem_offset;
    int max_header;
    bool no_autobind;
    struct kmem_cache *slab;
    unsigned int obj_size;
    slab_flags_t slab_flags;
    unsigned int useroffset;
    unsigned int usersize;
    unsigned int *orphan_count;
    struct request_sock_ops *rsk_prot;
    struct timewait_sock_ops *twsk_prot;
    union (anon) h;
    struct module *owner;
    char name[32];
    struct list_head node;
    int (*diag_destroy)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct proto {
    void (*close)(struct sock *, long int);
    int (*pre_connect)(struct sock *, struct sockaddr *, int);
    int (*connect)(struct sock *, struct sockaddr *, int);
    int (*disconnect)(struct sock *, int);
    struct sock * (*accept)(struct sock *, int, int *, bool);
    int (*ioctl)(struct sock *, int, int *);
    int (*init)(struct sock *);
    void (*destroy)(struct sock *);
    void (*shutdown)(struct sock *, int);
    int (*setsockopt)(struct sock *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*keepalive)(struct sock *, int);
    int (*compat_ioctl)(struct sock *, unsigned int, long unsigned int);
    int (*sendmsg)(struct sock *, struct msghdr *, size_t);
    int (*recvmsg)(struct sock *, struct msghdr *, size_t, int, int *);
    void (*splice_eof)(struct socket *);
    int (*bind)(struct sock *, struct sockaddr *, int);
    int (*bind_add)(struct sock *, struct sockaddr *, int);
    int (*backlog_rcv)(struct sock *, struct sk_buff *);
    bool (*bpf_bypass_getsockopt)(int, int);
    void (*release_cb)(struct sock *);
    int (*hash)(struct sock *);
    void (*unhash)(struct sock *);
    void (*rehash)(struct sock *);
    int (*get_port)(struct sock *, short unsigned int);
    void (*put_port)(struct sock *);
    int (*psock_update_sk_prot)(struct sock *, struct sk_psock *, bool);
    unsigned int inuse_idx;
    int (*forward_alloc_get)(const struct sock *);
    bool (*stream_memory_free)(const struct sock *, int);
    bool (*sock_is_readable)(struct sock *);
    void (*enter_memory_pressure)(struct sock *);
    void (*leave_memory_pressure)(struct sock *);
    atomic_long_t *memory_allocated;
    int *per_cpu_fw_alloc;
    struct percpu_counter *sockets_allocated;
    long unsigned int *memory_pressure;
    long int *sysctl_mem;
    int *sysctl_wmem;
    int *sysctl_rmem;
    u32 sysctl_wmem_offset;
    u32 sysctl_rmem_offset;
    int max_header;
    bool no_autobind;
    struct kmem_cache *slab;
    unsigned int obj_size;
    unsigned int ipv6_pinfo_offset;
    slab_flags_t slab_flags;
    unsigned int useroffset;
    unsigned int usersize;
    unsigned int *orphan_count;
    struct request_sock_ops *rsk_prot;
    struct timewait_sock_ops *twsk_prot;
    union (anon) h;
    struct module *owner;
    char name[32];
    struct list_head node;
    int (*diag_destroy)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct proto {
    void (*close)(struct sock *, long int);
    int (*pre_connect)(struct sock *, struct sockaddr *, int);
    int (*connect)(struct sock *, struct sockaddr *, int);
    int (*disconnect)(struct sock *, int);
    struct sock * (*accept)(struct sock *, int, int *, bool);
    int (*ioctl)(struct sock *, int, int *);
    int (*init)(struct sock *);
    void (*destroy)(struct sock *);
    void (*shutdown)(struct sock *, int);
    int (*setsockopt)(struct sock *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*keepalive)(struct sock *, int);
    int (*compat_ioctl)(struct sock *, unsigned int, long unsigned int);
    int (*sendmsg)(struct sock *, struct msghdr *, size_t);
    int (*recvmsg)(struct sock *, struct msghdr *, size_t, int, int *);
    void (*splice_eof)(struct socket *);
    int (*bind)(struct sock *, struct sockaddr *, int);
    int (*bind_add)(struct sock *, struct sockaddr *, int);
    int (*backlog_rcv)(struct sock *, struct sk_buff *);
    bool (*bpf_bypass_getsockopt)(int, int);
    void (*release_cb)(struct sock *);
    int (*hash)(struct sock *);
    void (*unhash)(struct sock *);
    void (*rehash)(struct sock *);
    int (*get_port)(struct sock *, short unsigned int);
    void (*put_port)(struct sock *);
    int (*psock_update_sk_prot)(struct sock *, struct sk_psock *, bool);
    unsigned int inuse_idx;
    int (*forward_alloc_get)(const struct sock *);
    bool (*stream_memory_free)(const struct sock *, int);
    bool (*sock_is_readable)(struct sock *);
    void (*enter_memory_pressure)(struct sock *);
    void (*leave_memory_pressure)(struct sock *);
    atomic_long_t *memory_allocated;
    int *per_cpu_fw_alloc;
    struct percpu_counter *sockets_allocated;
    long unsigned int *memory_pressure;
    long int *sysctl_mem;
    int *sysctl_wmem;
    int *sysctl_rmem;
    u32 sysctl_wmem_offset;
    u32 sysctl_rmem_offset;
    int max_header;
    bool no_autobind;
    struct kmem_cache *slab;
    unsigned int obj_size;
    unsigned int ipv6_pinfo_offset;
    slab_flags_t slab_flags;
    unsigned int useroffset;
    unsigned int usersize;
    unsigned int *orphan_count;
    struct request_sock_ops *rsk_prot;
    struct timewait_sock_ops *twsk_prot;
    union (anon) h;
    struct module *owner;
    char name[32];
    struct list_head node;
    int (*diag_destroy)(struct sock *, int);
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
struct proto {
    void (*close)(struct sock *, long int);
    int (*pre_connect)(struct sock *, struct sockaddr *, int);
    int (*connect)(struct sock *, struct sockaddr *, int);
    int (*disconnect)(struct sock *, int);
    struct sock * (*accept)(struct sock *, int, int *, bool);
    int (*ioctl)(struct sock *, int, long unsigned int);
    int (*init)(struct sock *);
    void (*destroy)(struct sock *);
    void (*shutdown)(struct sock *, int);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*keepalive)(struct sock *, int);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_ioctl)(struct sock *, unsigned int, long unsigned int);
    int (*sendmsg)(struct sock *, struct msghdr *, size_t);
    int (*recvmsg)(struct sock *, struct msghdr *, size_t, int, int, int *);
    int (*sendpage)(struct sock *, struct page *, int, size_t, int);
    int (*bind)(struct sock *, struct sockaddr *, int);
    int (*backlog_rcv)(struct sock *, struct sk_buff *);
    void (*release_cb)(struct sock *);
    int (*hash)(struct sock *);
    void (*unhash)(struct sock *);
    void (*rehash)(struct sock *);
    int (*get_port)(struct sock *, short unsigned int);
    unsigned int inuse_idx;
    bool (*stream_memory_free)(const struct sock *, int);
    bool (*stream_memory_read)(const struct sock *);
    void (*enter_memory_pressure)(struct sock *);
    void (*leave_memory_pressure)(struct sock *);
    atomic_long_t *memory_allocated;
    struct percpu_counter *sockets_allocated;
    long unsigned int *memory_pressure;
    long int *sysctl_mem;
    int *sysctl_wmem;
    int *sysctl_rmem;
    u32 sysctl_wmem_offset;
    u32 sysctl_rmem_offset;
    int max_header;
    bool no_autobind;
    struct kmem_cache *slab;
    unsigned int obj_size;
    slab_flags_t slab_flags;
    unsigned int useroffset;
    unsigned int usersize;
    struct percpu_counter *orphan_count;
    struct request_sock_ops *rsk_prot;
    struct timewait_sock_ops *twsk_prot;
    union (anon) h;
    struct module *owner;
    char name[32];
    struct list_head node;
    int (*diag_destroy)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct proto {
    void (*close)(struct sock *, long int);
    int (*pre_connect)(struct sock *, struct sockaddr *, int);
    int (*connect)(struct sock *, struct sockaddr *, int);
    int (*disconnect)(struct sock *, int);
    struct sock * (*accept)(struct sock *, int, int *, bool);
    int (*ioctl)(struct sock *, int, long unsigned int);
    int (*init)(struct sock *);
    void (*destroy)(struct sock *);
    void (*shutdown)(struct sock *, int);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*keepalive)(struct sock *, int);
    int (*sendmsg)(struct sock *, struct msghdr *, size_t);
    int (*recvmsg)(struct sock *, struct msghdr *, size_t, int, int, int *);
    int (*sendpage)(struct sock *, struct page *, int, size_t, int);
    int (*bind)(struct sock *, struct sockaddr *, int);
    int (*backlog_rcv)(struct sock *, struct sk_buff *);
    void (*release_cb)(struct sock *);
    int (*hash)(struct sock *);
    void (*unhash)(struct sock *);
    void (*rehash)(struct sock *);
    int (*get_port)(struct sock *, short unsigned int);
    unsigned int inuse_idx;
    bool (*stream_memory_free)(const struct sock *, int);
    bool (*stream_memory_read)(const struct sock *);
    void (*enter_memory_pressure)(struct sock *);
    void (*leave_memory_pressure)(struct sock *);
    atomic_long_t *memory_allocated;
    struct percpu_counter *sockets_allocated;
    long unsigned int *memory_pressure;
    long int *sysctl_mem;
    int *sysctl_wmem;
    int *sysctl_rmem;
    u32 sysctl_wmem_offset;
    u32 sysctl_rmem_offset;
    int max_header;
    bool no_autobind;
    struct kmem_cache *slab;
    unsigned int obj_size;
    slab_flags_t slab_flags;
    unsigned int useroffset;
    unsigned int usersize;
    struct percpu_counter *orphan_count;
    struct request_sock_ops *rsk_prot;
    struct timewait_sock_ops *twsk_prot;
    union (anon) h;
    struct module *owner;
    char name[32];
    struct list_head node;
    int (*diag_destroy)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct proto {
    void (*close)(struct sock *, long int);
    int (*pre_connect)(struct sock *, struct sockaddr *, int);
    int (*connect)(struct sock *, struct sockaddr *, int);
    int (*disconnect)(struct sock *, int);
    struct sock * (*accept)(struct sock *, int, int *, bool);
    int (*ioctl)(struct sock *, int, long unsigned int);
    int (*init)(struct sock *);
    void (*destroy)(struct sock *);
    void (*shutdown)(struct sock *, int);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*keepalive)(struct sock *, int);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_ioctl)(struct sock *, unsigned int, long unsigned int);
    int (*sendmsg)(struct sock *, struct msghdr *, size_t);
    int (*recvmsg)(struct sock *, struct msghdr *, size_t, int, int, int *);
    int (*sendpage)(struct sock *, struct page *, int, size_t, int);
    int (*bind)(struct sock *, struct sockaddr *, int);
    int (*backlog_rcv)(struct sock *, struct sk_buff *);
    void (*release_cb)(struct sock *);
    int (*hash)(struct sock *);
    void (*unhash)(struct sock *);
    void (*rehash)(struct sock *);
    int (*get_port)(struct sock *, short unsigned int);
    unsigned int inuse_idx;
    bool (*stream_memory_free)(const struct sock *, int);
    bool (*stream_memory_read)(const struct sock *);
    void (*enter_memory_pressure)(struct sock *);
    void (*leave_memory_pressure)(struct sock *);
    atomic_long_t *memory_allocated;
    struct percpu_counter *sockets_allocated;
    long unsigned int *memory_pressure;
    long int *sysctl_mem;
    int *sysctl_wmem;
    int *sysctl_rmem;
    u32 sysctl_wmem_offset;
    u32 sysctl_rmem_offset;
    int max_header;
    bool no_autobind;
    struct kmem_cache *slab;
    unsigned int obj_size;
    slab_flags_t slab_flags;
    unsigned int useroffset;
    unsigned int usersize;
    struct percpu_counter *orphan_count;
    struct request_sock_ops *rsk_prot;
    struct timewait_sock_ops *twsk_prot;
    union (anon) h;
    struct module *owner;
    char name[32];
    struct list_head node;
    int (*diag_destroy)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct proto {
    void (*close)(struct sock *, long int);
    int (*pre_connect)(struct sock *, struct sockaddr *, int);
    int (*connect)(struct sock *, struct sockaddr *, int);
    int (*disconnect)(struct sock *, int);
    struct sock * (*accept)(struct sock *, int, int *, bool);
    int (*ioctl)(struct sock *, int, long unsigned int);
    int (*init)(struct sock *);
    void (*destroy)(struct sock *);
    void (*shutdown)(struct sock *, int);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*keepalive)(struct sock *, int);
    int (*sendmsg)(struct sock *, struct msghdr *, size_t);
    int (*recvmsg)(struct sock *, struct msghdr *, size_t, int, int, int *);
    int (*sendpage)(struct sock *, struct page *, int, size_t, int);
    int (*bind)(struct sock *, struct sockaddr *, int);
    int (*backlog_rcv)(struct sock *, struct sk_buff *);
    void (*release_cb)(struct sock *);
    int (*hash)(struct sock *);
    void (*unhash)(struct sock *);
    void (*rehash)(struct sock *);
    int (*get_port)(struct sock *, short unsigned int);
    unsigned int inuse_idx;
    bool (*stream_memory_free)(const struct sock *, int);
    bool (*stream_memory_read)(const struct sock *);
    void (*enter_memory_pressure)(struct sock *);
    void (*leave_memory_pressure)(struct sock *);
    atomic_long_t *memory_allocated;
    struct percpu_counter *sockets_allocated;
    long unsigned int *memory_pressure;
    long int *sysctl_mem;
    int *sysctl_wmem;
    int *sysctl_rmem;
    u32 sysctl_wmem_offset;
    u32 sysctl_rmem_offset;
    int max_header;
    bool no_autobind;
    struct kmem_cache *slab;
    unsigned int obj_size;
    slab_flags_t slab_flags;
    unsigned int useroffset;
    unsigned int usersize;
    struct percpu_counter *orphan_count;
    struct request_sock_ops *rsk_prot;
    struct timewait_sock_ops *twsk_prot;
    union (anon) h;
    struct module *owner;
    char name[32];
    struct list_head node;
    int (*diag_destroy)(struct sock *, int);
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
struct proto {
    void (*close)(struct sock *, long int);
    int (*pre_connect)(struct sock *, struct sockaddr *, int);
    int (*connect)(struct sock *, struct sockaddr *, int);
    int (*disconnect)(struct sock *, int);
    struct sock * (*accept)(struct sock *, int, int *, bool);
    int (*ioctl)(struct sock *, int, long unsigned int);
    int (*init)(struct sock *);
    void (*destroy)(struct sock *);
    void (*shutdown)(struct sock *, int);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*keepalive)(struct sock *, int);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_ioctl)(struct sock *, unsigned int, long unsigned int);
    int (*sendmsg)(struct sock *, struct msghdr *, size_t);
    int (*recvmsg)(struct sock *, struct msghdr *, size_t, int, int, int *);
    int (*sendpage)(struct sock *, struct page *, int, size_t, int);
    int (*bind)(struct sock *, struct sockaddr *, int);
    int (*backlog_rcv)(struct sock *, struct sk_buff *);
    void (*release_cb)(struct sock *);
    int (*hash)(struct sock *);
    void (*unhash)(struct sock *);
    void (*rehash)(struct sock *);
    int (*get_port)(struct sock *, short unsigned int);
    unsigned int inuse_idx;
    bool (*stream_memory_free)(const struct sock *, int);
    bool (*stream_memory_read)(const struct sock *);
    void (*enter_memory_pressure)(struct sock *);
    void (*leave_memory_pressure)(struct sock *);
    atomic_long_t *memory_allocated;
    struct percpu_counter *sockets_allocated;
    long unsigned int *memory_pressure;
    long int *sysctl_mem;
    int *sysctl_wmem;
    int *sysctl_rmem;
    u32 sysctl_wmem_offset;
    u32 sysctl_rmem_offset;
    int max_header;
    bool no_autobind;
    struct kmem_cache *slab;
    unsigned int obj_size;
    slab_flags_t slab_flags;
    unsigned int useroffset;
    unsigned int usersize;
    struct percpu_counter *orphan_count;
    struct request_sock_ops *rsk_prot;
    struct timewait_sock_ops *twsk_prot;
    union (anon) h;
    struct module *owner;
    char name[32];
    struct list_head node;
    int (*diag_destroy)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct proto {
    void (*close)(struct sock *, long int);
    int (*pre_connect)(struct sock *, struct sockaddr *, int);
    int (*connect)(struct sock *, struct sockaddr *, int);
    int (*disconnect)(struct sock *, int);
    struct sock * (*accept)(struct sock *, int, int *, bool);
    int (*ioctl)(struct sock *, int, long unsigned int);
    int (*init)(struct sock *);
    void (*destroy)(struct sock *);
    void (*shutdown)(struct sock *, int);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*keepalive)(struct sock *, int);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_ioctl)(struct sock *, unsigned int, long unsigned int);
    int (*sendmsg)(struct sock *, struct msghdr *, size_t);
    int (*recvmsg)(struct sock *, struct msghdr *, size_t, int, int, int *);
    int (*sendpage)(struct sock *, struct page *, int, size_t, int);
    int (*bind)(struct sock *, struct sockaddr *, int);
    int (*backlog_rcv)(struct sock *, struct sk_buff *);
    void (*release_cb)(struct sock *);
    int (*hash)(struct sock *);
    void (*unhash)(struct sock *);
    void (*rehash)(struct sock *);
    int (*get_port)(struct sock *, short unsigned int);
    unsigned int inuse_idx;
    bool (*stream_memory_free)(const struct sock *, int);
    bool (*stream_memory_read)(const struct sock *);
    void (*enter_memory_pressure)(struct sock *);
    void (*leave_memory_pressure)(struct sock *);
    atomic_long_t *memory_allocated;
    struct percpu_counter *sockets_allocated;
    long unsigned int *memory_pressure;
    long int *sysctl_mem;
    int *sysctl_wmem;
    int *sysctl_rmem;
    u32 sysctl_wmem_offset;
    u32 sysctl_rmem_offset;
    int max_header;
    bool no_autobind;
    struct kmem_cache *slab;
    unsigned int obj_size;
    slab_flags_t slab_flags;
    unsigned int useroffset;
    unsigned int usersize;
    struct percpu_counter *orphan_count;
    struct request_sock_ops *rsk_prot;
    struct timewait_sock_ops *twsk_prot;
    union (anon) h;
    struct module *owner;
    char name[32];
    struct list_head node;
    int (*diag_destroy)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct proto {
    void (*close)(struct sock *, long int);
    int (*pre_connect)(struct sock *, struct sockaddr *, int);
    int (*connect)(struct sock *, struct sockaddr *, int);
    int (*disconnect)(struct sock *, int);
    struct sock * (*accept)(struct sock *, int, int *, bool);
    int (*ioctl)(struct sock *, int, long unsigned int);
    int (*init)(struct sock *);
    void (*destroy)(struct sock *);
    void (*shutdown)(struct sock *, int);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*keepalive)(struct sock *, int);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_ioctl)(struct sock *, unsigned int, long unsigned int);
    int (*sendmsg)(struct sock *, struct msghdr *, size_t);
    int (*recvmsg)(struct sock *, struct msghdr *, size_t, int, int, int *);
    int (*sendpage)(struct sock *, struct page *, int, size_t, int);
    int (*bind)(struct sock *, struct sockaddr *, int);
    int (*backlog_rcv)(struct sock *, struct sk_buff *);
    void (*release_cb)(struct sock *);
    int (*hash)(struct sock *);
    void (*unhash)(struct sock *);
    void (*rehash)(struct sock *);
    int (*get_port)(struct sock *, short unsigned int);
    unsigned int inuse_idx;
    bool (*stream_memory_free)(const struct sock *, int);
    bool (*stream_memory_read)(const struct sock *);
    void (*enter_memory_pressure)(struct sock *);
    void (*leave_memory_pressure)(struct sock *);
    atomic_long_t *memory_allocated;
    struct percpu_counter *sockets_allocated;
    long unsigned int *memory_pressure;
    long int *sysctl_mem;
    int *sysctl_wmem;
    int *sysctl_rmem;
    u32 sysctl_wmem_offset;
    u32 sysctl_rmem_offset;
    int max_header;
    bool no_autobind;
    struct kmem_cache *slab;
    unsigned int obj_size;
    slab_flags_t slab_flags;
    unsigned int useroffset;
    unsigned int usersize;
    struct percpu_counter *orphan_count;
    struct request_sock_ops *rsk_prot;
    struct timewait_sock_ops *twsk_prot;
    union (anon) h;
    struct module *owner;
    char name[32];
    struct list_head node;
    int (*diag_destroy)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct proto {
    void (*close)(struct sock *, long int);
    int (*pre_connect)(struct sock *, struct sockaddr *, int);
    int (*connect)(struct sock *, struct sockaddr *, int);
    int (*disconnect)(struct sock *, int);
    struct sock * (*accept)(struct sock *, int, int *, bool);
    int (*ioctl)(struct sock *, int, long unsigned int);
    int (*init)(struct sock *);
    void (*destroy)(struct sock *);
    void (*shutdown)(struct sock *, int);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    void (*keepalive)(struct sock *, int);
    int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct sock *, int, int, char *, int *);
    int (*compat_ioctl)(struct sock *, unsigned int, long unsigned int);
    int (*sendmsg)(struct sock *, struct msghdr *, size_t);
    int (*recvmsg)(struct sock *, struct msghdr *, size_t, int, int, int *);
    int (*sendpage)(struct sock *, struct page *, int, size_t, int);
    int (*bind)(struct sock *, struct sockaddr *, int);
    int (*backlog_rcv)(struct sock *, struct sk_buff *);
    void (*release_cb)(struct sock *);
    int (*hash)(struct sock *);
    void (*unhash)(struct sock *);
    void (*rehash)(struct sock *);
    int (*get_port)(struct sock *, short unsigned int);
    unsigned int inuse_idx;
    bool (*stream_memory_free)(const struct sock *, int);
    bool (*stream_memory_read)(const struct sock *);
    void (*enter_memory_pressure)(struct sock *);
    void (*leave_memory_pressure)(struct sock *);
    atomic_long_t *memory_allocated;
    struct percpu_counter *sockets_allocated;
    long unsigned int *memory_pressure;
    long int *sysctl_mem;
    int *sysctl_wmem;
    int *sysctl_rmem;
    u32 sysctl_wmem_offset;
    u32 sysctl_rmem_offset;
    int max_header;
    bool no_autobind;
    struct kmem_cache *slab;
    unsigned int obj_size;
    slab_flags_t slab_flags;
    unsigned int useroffset;
    unsigned int usersize;
    struct percpu_counter *orphan_count;
    struct request_sock_ops *rsk_prot;
    struct timewait_sock_ops *twsk_prot;
    union (anon) h;
    struct module *owner;
    char name[32];
    struct list_head node;
    int (*diag_destroy)(struct sock *, int);
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
<code>int (*diag_destroy)(struct sock *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*init_cgroup)(struct mem_cgroup *, struct cgroup_subsys *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*destroy_cgroup)(struct mem_cgroup *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct cg_proto * (*proto_cgroup)(struct mem_cgroup *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*hash)(struct sock *)</code> ➡️ <code>int (*hash)(struct sock *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>void (*clear_sk)(struct sock *, int)</code>
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
<code>void (*keepalive)(struct sock *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*leave_memory_pressure)(struct sock *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct sock * (*accept)(struct sock *, int, int *)</code> ➡️ <code>struct sock * (*accept)(struct sock *, int, int *, bool)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int *memory_pressure</code> ➡️ <code>long unsigned int *memory_pressure</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 sysctl_wmem_offset</code>
</li>
<li>
<b>Field added. </b>
<code>u32 sysctl_rmem_offset</code>
</li>
<li>
<b>Field type changed. </b>
<code>int slab_flags</code> ➡️ <code>slab_flags_t slab_flags</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*pre_connect)(struct sock *, struct sockaddr *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>bool (*stream_memory_read)(const struct sock *)</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int useroffset</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int usersize</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>bool (*stream_memory_free)(const struct sock *)</code> ➡️ <code>bool (*stream_memory_free)(const struct sock *, int)</code>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*bind_add)(struct sock *, struct sockaddr *, int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*compat_getsockopt)(struct sock *, int, int, char *, int *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*setsockopt)(struct sock *, int, int, char *, unsigned int)</code> ➡️ <code>int (*setsockopt)(struct sock *, int, int, sockptr_t, unsigned int)</code>
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
<code>bool (*bpf_bypass_getsockopt)(int, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*psock_update_sk_prot)(struct sock *, struct sk_psock *, bool)</code>
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
<code>bool (*sock_is_readable)(struct sock *)</code>
</li>
<li>
<b>Field removed. </b>
<code>bool (*stream_memory_read)(const struct sock *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct percpu_counter *orphan_count</code> ➡️ <code>unsigned int *orphan_count</code>
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
<code>void (*put_port)(struct sock *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*forward_alloc_get)(const struct sock *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*recvmsg)(struct sock *, struct msghdr *, size_t, int, int, int *)</code> ➡️ <code>int (*recvmsg)(struct sock *, struct msghdr *, size_t, int, int *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int *per_cpu_fw_alloc</code>
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
<code>void (*splice_eof)(struct socket *)</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int ipv6_pinfo_offset</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*sendpage)(struct sock *, struct page *, int, size_t, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*ioctl)(struct sock *, int, long unsigned int)</code> ➡️ <code>int (*ioctl)(struct sock *, int, int *)</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*compat_getsockopt)(struct sock *, int, int, char *, int *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*compat_ioctl)(struct sock *, unsigned int, long unsigned int)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*compat_setsockopt)(struct sock *, int, int, char *, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*compat_getsockopt)(struct sock *, int, int, char *, int *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*compat_ioctl)(struct sock *, unsigned int, long unsigned int)</code>
</li>
</ul>
</details>
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
