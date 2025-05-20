# Struct: <code>rpc_rqst</code>

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
struct rpc_rqst {
    struct rpc_xprt *rq_xprt;
    struct xdr_buf rq_snd_buf;
    struct xdr_buf rq_rcv_buf;
    struct rpc_task *rq_task;
    struct rpc_cred *rq_cred;
    __be32 rq_xid;
    int rq_cong;
    u32 rq_seqno;
    int rq_enc_pages_num;
    struct page **rq_enc_pages;
    void (*rq_release_snd_buf)(struct rpc_rqst *);
    struct list_head rq_list;
    __u32 *rq_buffer;
    size_t rq_callsize;
    size_t rq_rcvsize;
    size_t rq_xmit_bytes_sent;
    size_t rq_reply_bytes_recvd;
    struct xdr_buf rq_private_buf;
    long unsigned int rq_majortimeo;
    long unsigned int rq_timeout;
    ktime_t rq_rtt;
    unsigned int rq_retries;
    unsigned int rq_connect_cookie;
    u32 rq_bytes_sent;
    ktime_t rq_xtime;
    int rq_ntrans;
    struct list_head rq_bc_list;
    long unsigned int rq_bc_pa_state;
    struct list_head rq_bc_pa_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rpc_rqst {
    struct rpc_xprt *rq_xprt;
    struct xdr_buf rq_snd_buf;
    struct xdr_buf rq_rcv_buf;
    struct rpc_task *rq_task;
    struct rpc_cred *rq_cred;
    __be32 rq_xid;
    int rq_cong;
    u32 rq_seqno;
    int rq_enc_pages_num;
    struct page **rq_enc_pages;
    void (*rq_release_snd_buf)(struct rpc_rqst *);
    struct list_head rq_list;
    void *rq_xprtdata;
    void *rq_buffer;
    size_t rq_callsize;
    void *rq_rbuffer;
    size_t rq_rcvsize;
    size_t rq_xmit_bytes_sent;
    size_t rq_reply_bytes_recvd;
    struct xdr_buf rq_private_buf;
    long unsigned int rq_majortimeo;
    long unsigned int rq_timeout;
    ktime_t rq_rtt;
    unsigned int rq_retries;
    unsigned int rq_connect_cookie;
    u32 rq_bytes_sent;
    ktime_t rq_xtime;
    int rq_ntrans;
    struct list_head rq_bc_list;
    long unsigned int rq_bc_pa_state;
    struct list_head rq_bc_pa_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rpc_rqst {
    struct rpc_xprt *rq_xprt;
    struct xdr_buf rq_snd_buf;
    struct xdr_buf rq_rcv_buf;
    struct rpc_task *rq_task;
    struct rpc_cred *rq_cred;
    __be32 rq_xid;
    int rq_cong;
    u32 rq_seqno;
    int rq_enc_pages_num;
    struct page **rq_enc_pages;
    void (*rq_release_snd_buf)(struct rpc_rqst *);
    struct list_head rq_list;
    void *rq_xprtdata;
    void *rq_buffer;
    size_t rq_callsize;
    void *rq_rbuffer;
    size_t rq_rcvsize;
    size_t rq_xmit_bytes_sent;
    size_t rq_reply_bytes_recvd;
    struct xdr_buf rq_private_buf;
    long unsigned int rq_majortimeo;
    long unsigned int rq_timeout;
    ktime_t rq_rtt;
    unsigned int rq_retries;
    unsigned int rq_connect_cookie;
    u32 rq_bytes_sent;
    ktime_t rq_xtime;
    int rq_ntrans;
    struct list_head rq_bc_list;
    long unsigned int rq_bc_pa_state;
    struct list_head rq_bc_pa_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rpc_rqst {
    struct rpc_xprt *rq_xprt;
    struct xdr_buf rq_snd_buf;
    struct xdr_buf rq_rcv_buf;
    struct rpc_task *rq_task;
    struct rpc_cred *rq_cred;
    __be32 rq_xid;
    int rq_cong;
    u32 rq_seqno;
    int rq_enc_pages_num;
    struct page **rq_enc_pages;
    void (*rq_release_snd_buf)(struct rpc_rqst *);
    struct list_head rq_list;
    void *rq_xprtdata;
    void *rq_buffer;
    size_t rq_callsize;
    void *rq_rbuffer;
    size_t rq_rcvsize;
    size_t rq_xmit_bytes_sent;
    size_t rq_reply_bytes_recvd;
    struct xdr_buf rq_private_buf;
    long unsigned int rq_majortimeo;
    long unsigned int rq_timeout;
    ktime_t rq_rtt;
    unsigned int rq_retries;
    unsigned int rq_connect_cookie;
    u32 rq_bytes_sent;
    ktime_t rq_xtime;
    int rq_ntrans;
    struct list_head rq_bc_list;
    long unsigned int rq_bc_pa_state;
    struct list_head rq_bc_pa_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rpc_rqst {
    struct rpc_xprt *rq_xprt;
    struct xdr_buf rq_snd_buf;
    struct xdr_buf rq_rcv_buf;
    struct rpc_task *rq_task;
    struct rpc_cred *rq_cred;
    __be32 rq_xid;
    int rq_cong;
    u32 rq_seqno;
    int rq_enc_pages_num;
    struct page **rq_enc_pages;
    void (*rq_release_snd_buf)(struct rpc_rqst *);
    struct list_head rq_list;
    void *rq_buffer;
    size_t rq_callsize;
    void *rq_rbuffer;
    size_t rq_rcvsize;
    size_t rq_xmit_bytes_sent;
    size_t rq_reply_bytes_recvd;
    struct xdr_buf rq_private_buf;
    long unsigned int rq_majortimeo;
    long unsigned int rq_timeout;
    ktime_t rq_rtt;
    unsigned int rq_retries;
    unsigned int rq_connect_cookie;
    u32 rq_bytes_sent;
    ktime_t rq_xtime;
    int rq_ntrans;
    struct list_head rq_bc_list;
    long unsigned int rq_bc_pa_state;
    struct list_head rq_bc_pa_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rpc_rqst {
    struct rpc_xprt *rq_xprt;
    struct xdr_buf rq_snd_buf;
    struct xdr_buf rq_rcv_buf;
    struct rpc_task *rq_task;
    struct rpc_cred *rq_cred;
    __be32 rq_xid;
    int rq_cong;
    u32 rq_seqno;
    int rq_enc_pages_num;
    struct page **rq_enc_pages;
    void (*rq_release_snd_buf)(struct rpc_rqst *);
    struct list_head rq_list;
    struct rb_node rq_recv;
    struct list_head rq_xmit;
    struct list_head rq_xmit2;
    void *rq_buffer;
    size_t rq_callsize;
    void *rq_rbuffer;
    size_t rq_rcvsize;
    size_t rq_xmit_bytes_sent;
    size_t rq_reply_bytes_recvd;
    struct xdr_buf rq_private_buf;
    long unsigned int rq_majortimeo;
    long unsigned int rq_timeout;
    ktime_t rq_rtt;
    unsigned int rq_retries;
    unsigned int rq_connect_cookie;
    atomic_t rq_pin;
    u32 rq_bytes_sent;
    ktime_t rq_xtime;
    int rq_ntrans;
    struct list_head rq_bc_list;
    long unsigned int rq_bc_pa_state;
    struct list_head rq_bc_pa_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rpc_rqst {
    struct rpc_xprt *rq_xprt;
    struct xdr_buf rq_snd_buf;
    struct xdr_buf rq_rcv_buf;
    struct rpc_task *rq_task;
    struct rpc_cred *rq_cred;
    __be32 rq_xid;
    int rq_cong;
    u32 rq_seqno;
    int rq_enc_pages_num;
    struct page **rq_enc_pages;
    void (*rq_release_snd_buf)(struct rpc_rqst *);
    struct list_head rq_list;
    struct rb_node rq_recv;
    struct list_head rq_xmit;
    struct list_head rq_xmit2;
    void *rq_buffer;
    size_t rq_callsize;
    void *rq_rbuffer;
    size_t rq_rcvsize;
    size_t rq_xmit_bytes_sent;
    size_t rq_reply_bytes_recvd;
    struct xdr_buf rq_private_buf;
    long unsigned int rq_majortimeo;
    long unsigned int rq_timeout;
    ktime_t rq_rtt;
    unsigned int rq_retries;
    unsigned int rq_connect_cookie;
    atomic_t rq_pin;
    u32 rq_bytes_sent;
    ktime_t rq_xtime;
    int rq_ntrans;
    struct list_head rq_bc_list;
    long unsigned int rq_bc_pa_state;
    struct list_head rq_bc_pa_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rpc_rqst {
    struct rpc_xprt *rq_xprt;
    struct xdr_buf rq_snd_buf;
    struct xdr_buf rq_rcv_buf;
    struct rpc_task *rq_task;
    struct rpc_cred *rq_cred;
    __be32 rq_xid;
    int rq_cong;
    u32 rq_seqno;
    int rq_enc_pages_num;
    struct page **rq_enc_pages;
    void (*rq_release_snd_buf)(struct rpc_rqst *);
    struct list_head rq_list;
    struct rb_node rq_recv;
    struct list_head rq_xmit;
    struct list_head rq_xmit2;
    void *rq_buffer;
    size_t rq_callsize;
    void *rq_rbuffer;
    size_t rq_rcvsize;
    size_t rq_xmit_bytes_sent;
    size_t rq_reply_bytes_recvd;
    struct xdr_buf rq_private_buf;
    long unsigned int rq_majortimeo;
    long unsigned int rq_timeout;
    ktime_t rq_rtt;
    unsigned int rq_retries;
    unsigned int rq_connect_cookie;
    atomic_t rq_pin;
    u32 rq_bytes_sent;
    ktime_t rq_xtime;
    int rq_ntrans;
    struct list_head rq_bc_list;
    long unsigned int rq_bc_pa_state;
    struct list_head rq_bc_pa_list;
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
struct rpc_rqst {
    struct rpc_xprt *rq_xprt;
    struct xdr_buf rq_snd_buf;
    struct xdr_buf rq_rcv_buf;
    struct rpc_task *rq_task;
    struct rpc_cred *rq_cred;
    __be32 rq_xid;
    int rq_cong;
    u32 rq_seqno;
    int rq_enc_pages_num;
    struct page **rq_enc_pages;
    void (*rq_release_snd_buf)(struct rpc_rqst *);
    struct list_head rq_list;
    struct rb_node rq_recv;
    struct list_head rq_xmit;
    struct list_head rq_xmit2;
    void *rq_buffer;
    size_t rq_callsize;
    void *rq_rbuffer;
    size_t rq_rcvsize;
    size_t rq_xmit_bytes_sent;
    size_t rq_reply_bytes_recvd;
    struct xdr_buf rq_private_buf;
    long unsigned int rq_majortimeo;
    long unsigned int rq_minortimeo;
    long unsigned int rq_timeout;
    ktime_t rq_rtt;
    unsigned int rq_retries;
    unsigned int rq_connect_cookie;
    atomic_t rq_pin;
    u32 rq_bytes_sent;
    ktime_t rq_xtime;
    int rq_ntrans;
    struct list_head rq_bc_list;
    long unsigned int rq_bc_pa_state;
    struct list_head rq_bc_pa_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rpc_rqst {
    struct rpc_xprt *rq_xprt;
    struct xdr_buf rq_snd_buf;
    struct xdr_buf rq_rcv_buf;
    struct rpc_task *rq_task;
    struct rpc_cred *rq_cred;
    __be32 rq_xid;
    int rq_cong;
    u32 rq_seqno;
    int rq_enc_pages_num;
    struct page **rq_enc_pages;
    void (*rq_release_snd_buf)(struct rpc_rqst *);
    struct list_head rq_list;
    struct rb_node rq_recv;
    struct list_head rq_xmit;
    struct list_head rq_xmit2;
    void *rq_buffer;
    size_t rq_callsize;
    void *rq_rbuffer;
    size_t rq_rcvsize;
    size_t rq_xmit_bytes_sent;
    size_t rq_reply_bytes_recvd;
    struct xdr_buf rq_private_buf;
    long unsigned int rq_majortimeo;
    long unsigned int rq_minortimeo;
    long unsigned int rq_timeout;
    ktime_t rq_rtt;
    unsigned int rq_retries;
    unsigned int rq_connect_cookie;
    atomic_t rq_pin;
    u32 rq_bytes_sent;
    ktime_t rq_xtime;
    int rq_ntrans;
    struct list_head rq_bc_list;
    long unsigned int rq_bc_pa_state;
    struct list_head rq_bc_pa_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rpc_rqst {
    struct rpc_xprt *rq_xprt;
    struct xdr_buf rq_snd_buf;
    struct xdr_buf rq_rcv_buf;
    struct rpc_task *rq_task;
    struct rpc_cred *rq_cred;
    __be32 rq_xid;
    int rq_cong;
    u32 rq_seqno;
    int rq_enc_pages_num;
    struct page **rq_enc_pages;
    void (*rq_release_snd_buf)(struct rpc_rqst *);
    struct list_head rq_list;
    struct rb_node rq_recv;
    struct list_head rq_xmit;
    struct list_head rq_xmit2;
    void *rq_buffer;
    size_t rq_callsize;
    void *rq_rbuffer;
    size_t rq_rcvsize;
    size_t rq_xmit_bytes_sent;
    size_t rq_reply_bytes_recvd;
    struct xdr_buf rq_private_buf;
    long unsigned int rq_majortimeo;
    long unsigned int rq_minortimeo;
    long unsigned int rq_timeout;
    ktime_t rq_rtt;
    unsigned int rq_retries;
    unsigned int rq_connect_cookie;
    atomic_t rq_pin;
    u32 rq_bytes_sent;
    ktime_t rq_xtime;
    int rq_ntrans;
    struct list_head rq_bc_list;
    long unsigned int rq_bc_pa_state;
    struct list_head rq_bc_pa_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rpc_rqst {
    struct rpc_xprt *rq_xprt;
    struct xdr_buf rq_snd_buf;
    struct xdr_buf rq_rcv_buf;
    struct rpc_task *rq_task;
    struct rpc_cred *rq_cred;
    __be32 rq_xid;
    int rq_cong;
    u32 rq_seqno;
    int rq_enc_pages_num;
    struct page **rq_enc_pages;
    void (*rq_release_snd_buf)(struct rpc_rqst *);
    struct list_head rq_list;
    struct rb_node rq_recv;
    struct list_head rq_xmit;
    struct list_head rq_xmit2;
    void *rq_buffer;
    size_t rq_callsize;
    void *rq_rbuffer;
    size_t rq_rcvsize;
    size_t rq_xmit_bytes_sent;
    size_t rq_reply_bytes_recvd;
    struct xdr_buf rq_private_buf;
    long unsigned int rq_majortimeo;
    long unsigned int rq_minortimeo;
    long unsigned int rq_timeout;
    ktime_t rq_rtt;
    unsigned int rq_retries;
    unsigned int rq_connect_cookie;
    atomic_t rq_pin;
    u32 rq_bytes_sent;
    ktime_t rq_xtime;
    int rq_ntrans;
    struct list_head rq_bc_list;
    long unsigned int rq_bc_pa_state;
    struct list_head rq_bc_pa_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rpc_rqst {
    struct rpc_xprt *rq_xprt;
    struct xdr_buf rq_snd_buf;
    struct xdr_buf rq_rcv_buf;
    struct rpc_task *rq_task;
    struct rpc_cred *rq_cred;
    __be32 rq_xid;
    int rq_cong;
    u32 rq_seqno;
    int rq_enc_pages_num;
    struct page **rq_enc_pages;
    void (*rq_release_snd_buf)(struct rpc_rqst *);
    struct list_head rq_list;
    struct rb_node rq_recv;
    struct list_head rq_xmit;
    struct list_head rq_xmit2;
    void *rq_buffer;
    size_t rq_callsize;
    void *rq_rbuffer;
    size_t rq_rcvsize;
    size_t rq_xmit_bytes_sent;
    size_t rq_reply_bytes_recvd;
    struct xdr_buf rq_private_buf;
    long unsigned int rq_majortimeo;
    long unsigned int rq_minortimeo;
    long unsigned int rq_timeout;
    ktime_t rq_rtt;
    unsigned int rq_retries;
    unsigned int rq_connect_cookie;
    atomic_t rq_pin;
    u32 rq_bytes_sent;
    ktime_t rq_xtime;
    int rq_ntrans;
    struct list_head rq_bc_list;
    long unsigned int rq_bc_pa_state;
    struct list_head rq_bc_pa_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rpc_rqst {
    struct rpc_xprt *rq_xprt;
    struct xdr_buf rq_snd_buf;
    struct xdr_buf rq_rcv_buf;
    struct rpc_task *rq_task;
    struct rpc_cred *rq_cred;
    __be32 rq_xid;
    int rq_cong;
    u32 rq_seqno;
    int rq_enc_pages_num;
    struct page **rq_enc_pages;
    void (*rq_release_snd_buf)(struct rpc_rqst *);
    struct list_head rq_list;
    struct rb_node rq_recv;
    struct list_head rq_xmit;
    struct list_head rq_xmit2;
    void *rq_buffer;
    size_t rq_callsize;
    void *rq_rbuffer;
    size_t rq_rcvsize;
    size_t rq_xmit_bytes_sent;
    size_t rq_reply_bytes_recvd;
    struct xdr_buf rq_private_buf;
    long unsigned int rq_majortimeo;
    long unsigned int rq_minortimeo;
    long unsigned int rq_timeout;
    ktime_t rq_rtt;
    unsigned int rq_retries;
    unsigned int rq_connect_cookie;
    atomic_t rq_pin;
    u32 rq_bytes_sent;
    ktime_t rq_xtime;
    int rq_ntrans;
    struct lwq_node rq_bc_list;
    long unsigned int rq_bc_pa_state;
    struct list_head rq_bc_pa_list;
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
struct rpc_rqst {
    struct rpc_xprt *rq_xprt;
    struct xdr_buf rq_snd_buf;
    struct xdr_buf rq_rcv_buf;
    struct rpc_task *rq_task;
    struct rpc_cred *rq_cred;
    __be32 rq_xid;
    int rq_cong;
    u32 rq_seqno;
    int rq_enc_pages_num;
    struct page **rq_enc_pages;
    void (*rq_release_snd_buf)(struct rpc_rqst *);
    struct list_head rq_list;
    struct rb_node rq_recv;
    struct list_head rq_xmit;
    struct list_head rq_xmit2;
    void *rq_buffer;
    size_t rq_callsize;
    void *rq_rbuffer;
    size_t rq_rcvsize;
    size_t rq_xmit_bytes_sent;
    size_t rq_reply_bytes_recvd;
    struct xdr_buf rq_private_buf;
    long unsigned int rq_majortimeo;
    long unsigned int rq_timeout;
    ktime_t rq_rtt;
    unsigned int rq_retries;
    unsigned int rq_connect_cookie;
    atomic_t rq_pin;
    u32 rq_bytes_sent;
    ktime_t rq_xtime;
    int rq_ntrans;
    struct list_head rq_bc_list;
    long unsigned int rq_bc_pa_state;
    struct list_head rq_bc_pa_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rpc_rqst {
    struct rpc_xprt *rq_xprt;
    struct xdr_buf rq_snd_buf;
    struct xdr_buf rq_rcv_buf;
    struct rpc_task *rq_task;
    struct rpc_cred *rq_cred;
    __be32 rq_xid;
    int rq_cong;
    u32 rq_seqno;
    int rq_enc_pages_num;
    struct page **rq_enc_pages;
    void (*rq_release_snd_buf)(struct rpc_rqst *);
    struct list_head rq_list;
    struct rb_node rq_recv;
    struct list_head rq_xmit;
    struct list_head rq_xmit2;
    void *rq_buffer;
    size_t rq_callsize;
    void *rq_rbuffer;
    size_t rq_rcvsize;
    size_t rq_xmit_bytes_sent;
    size_t rq_reply_bytes_recvd;
    struct xdr_buf rq_private_buf;
    long unsigned int rq_majortimeo;
    long unsigned int rq_timeout;
    ktime_t rq_rtt;
    unsigned int rq_retries;
    unsigned int rq_connect_cookie;
    atomic_t rq_pin;
    u32 rq_bytes_sent;
    ktime_t rq_xtime;
    int rq_ntrans;
    struct list_head rq_bc_list;
    long unsigned int rq_bc_pa_state;
    struct list_head rq_bc_pa_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rpc_rqst {
    struct rpc_xprt *rq_xprt;
    struct xdr_buf rq_snd_buf;
    struct xdr_buf rq_rcv_buf;
    struct rpc_task *rq_task;
    struct rpc_cred *rq_cred;
    __be32 rq_xid;
    int rq_cong;
    u32 rq_seqno;
    int rq_enc_pages_num;
    struct page **rq_enc_pages;
    void (*rq_release_snd_buf)(struct rpc_rqst *);
    struct list_head rq_list;
    struct rb_node rq_recv;
    struct list_head rq_xmit;
    struct list_head rq_xmit2;
    void *rq_buffer;
    size_t rq_callsize;
    void *rq_rbuffer;
    size_t rq_rcvsize;
    size_t rq_xmit_bytes_sent;
    size_t rq_reply_bytes_recvd;
    struct xdr_buf rq_private_buf;
    long unsigned int rq_majortimeo;
    long unsigned int rq_timeout;
    ktime_t rq_rtt;
    unsigned int rq_retries;
    unsigned int rq_connect_cookie;
    atomic_t rq_pin;
    u32 rq_bytes_sent;
    ktime_t rq_xtime;
    int rq_ntrans;
    struct list_head rq_bc_list;
    long unsigned int rq_bc_pa_state;
    struct list_head rq_bc_pa_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct rpc_rqst {
    struct rpc_xprt *rq_xprt;
    struct xdr_buf rq_snd_buf;
    struct xdr_buf rq_rcv_buf;
    struct rpc_task *rq_task;
    struct rpc_cred *rq_cred;
    __be32 rq_xid;
    int rq_cong;
    u32 rq_seqno;
    int rq_enc_pages_num;
    struct page **rq_enc_pages;
    void (*rq_release_snd_buf)(struct rpc_rqst *);
    struct list_head rq_list;
    struct rb_node rq_recv;
    struct list_head rq_xmit;
    struct list_head rq_xmit2;
    void *rq_buffer;
    size_t rq_callsize;
    void *rq_rbuffer;
    size_t rq_rcvsize;
    size_t rq_xmit_bytes_sent;
    size_t rq_reply_bytes_recvd;
    struct xdr_buf rq_private_buf;
    long unsigned int rq_majortimeo;
    long unsigned int rq_timeout;
    ktime_t rq_rtt;
    unsigned int rq_retries;
    unsigned int rq_connect_cookie;
    atomic_t rq_pin;
    u32 rq_bytes_sent;
    ktime_t rq_xtime;
    int rq_ntrans;
    struct list_head rq_bc_list;
    long unsigned int rq_bc_pa_state;
    struct list_head rq_bc_pa_list;
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
struct rpc_rqst {
    struct rpc_xprt *rq_xprt;
    struct xdr_buf rq_snd_buf;
    struct xdr_buf rq_rcv_buf;
    struct rpc_task *rq_task;
    struct rpc_cred *rq_cred;
    __be32 rq_xid;
    int rq_cong;
    u32 rq_seqno;
    int rq_enc_pages_num;
    struct page **rq_enc_pages;
    void (*rq_release_snd_buf)(struct rpc_rqst *);
    struct list_head rq_list;
    struct rb_node rq_recv;
    struct list_head rq_xmit;
    struct list_head rq_xmit2;
    void *rq_buffer;
    size_t rq_callsize;
    void *rq_rbuffer;
    size_t rq_rcvsize;
    size_t rq_xmit_bytes_sent;
    size_t rq_reply_bytes_recvd;
    struct xdr_buf rq_private_buf;
    long unsigned int rq_majortimeo;
    long unsigned int rq_timeout;
    ktime_t rq_rtt;
    unsigned int rq_retries;
    unsigned int rq_connect_cookie;
    atomic_t rq_pin;
    u32 rq_bytes_sent;
    ktime_t rq_xtime;
    int rq_ntrans;
    struct list_head rq_bc_list;
    long unsigned int rq_bc_pa_state;
    struct list_head rq_bc_pa_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rpc_rqst {
    struct rpc_xprt *rq_xprt;
    struct xdr_buf rq_snd_buf;
    struct xdr_buf rq_rcv_buf;
    struct rpc_task *rq_task;
    struct rpc_cred *rq_cred;
    __be32 rq_xid;
    int rq_cong;
    u32 rq_seqno;
    int rq_enc_pages_num;
    struct page **rq_enc_pages;
    void (*rq_release_snd_buf)(struct rpc_rqst *);
    struct list_head rq_list;
    struct rb_node rq_recv;
    struct list_head rq_xmit;
    struct list_head rq_xmit2;
    void *rq_buffer;
    size_t rq_callsize;
    void *rq_rbuffer;
    size_t rq_rcvsize;
    size_t rq_xmit_bytes_sent;
    size_t rq_reply_bytes_recvd;
    struct xdr_buf rq_private_buf;
    long unsigned int rq_majortimeo;
    long unsigned int rq_timeout;
    ktime_t rq_rtt;
    unsigned int rq_retries;
    unsigned int rq_connect_cookie;
    atomic_t rq_pin;
    u32 rq_bytes_sent;
    ktime_t rq_xtime;
    int rq_ntrans;
    struct list_head rq_bc_list;
    long unsigned int rq_bc_pa_state;
    struct list_head rq_bc_pa_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rpc_rqst {
    struct rpc_xprt *rq_xprt;
    struct xdr_buf rq_snd_buf;
    struct xdr_buf rq_rcv_buf;
    struct rpc_task *rq_task;
    struct rpc_cred *rq_cred;
    __be32 rq_xid;
    int rq_cong;
    u32 rq_seqno;
    int rq_enc_pages_num;
    struct page **rq_enc_pages;
    void (*rq_release_snd_buf)(struct rpc_rqst *);
    struct list_head rq_list;
    struct rb_node rq_recv;
    struct list_head rq_xmit;
    struct list_head rq_xmit2;
    void *rq_buffer;
    size_t rq_callsize;
    void *rq_rbuffer;
    size_t rq_rcvsize;
    size_t rq_xmit_bytes_sent;
    size_t rq_reply_bytes_recvd;
    struct xdr_buf rq_private_buf;
    long unsigned int rq_majortimeo;
    long unsigned int rq_timeout;
    ktime_t rq_rtt;
    unsigned int rq_retries;
    unsigned int rq_connect_cookie;
    atomic_t rq_pin;
    u32 rq_bytes_sent;
    ktime_t rq_xtime;
    int rq_ntrans;
    struct list_head rq_bc_list;
    long unsigned int rq_bc_pa_state;
    struct list_head rq_bc_pa_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rpc_rqst {
    struct rpc_xprt *rq_xprt;
    struct xdr_buf rq_snd_buf;
    struct xdr_buf rq_rcv_buf;
    struct rpc_task *rq_task;
    struct rpc_cred *rq_cred;
    __be32 rq_xid;
    int rq_cong;
    u32 rq_seqno;
    int rq_enc_pages_num;
    struct page **rq_enc_pages;
    void (*rq_release_snd_buf)(struct rpc_rqst *);
    struct list_head rq_list;
    struct rb_node rq_recv;
    struct list_head rq_xmit;
    struct list_head rq_xmit2;
    void *rq_buffer;
    size_t rq_callsize;
    void *rq_rbuffer;
    size_t rq_rcvsize;
    size_t rq_xmit_bytes_sent;
    size_t rq_reply_bytes_recvd;
    struct xdr_buf rq_private_buf;
    long unsigned int rq_majortimeo;
    long unsigned int rq_timeout;
    ktime_t rq_rtt;
    unsigned int rq_retries;
    unsigned int rq_connect_cookie;
    atomic_t rq_pin;
    u32 rq_bytes_sent;
    ktime_t rq_xtime;
    int rq_ntrans;
    struct list_head rq_bc_list;
    long unsigned int rq_bc_pa_state;
    struct list_head rq_bc_pa_list;
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
<b>Field added. </b>
<code>void *rq_xprtdata</code>
</li>
<li>
<b>Field added. </b>
<code>void *rq_rbuffer</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u32 *rq_buffer</code> ➡️ <code>void *rq_buffer</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>void *rq_xprtdata</code>
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
<code>struct rb_node rq_recv</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head rq_xmit</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head rq_xmit2</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t rq_pin</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct list_head rq_bc_list</code> ➡️ <code>struct lwq_node rq_bc_list</code>
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
