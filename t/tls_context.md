# Struct: <code>tls_context</code>

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
struct tls_context {
    union tls_crypto_context crypto_send;
    union tls_crypto_context crypto_recv;
    struct list_head list;
    struct net_device *netdev;
    refcount_t refcount;
    void *priv_ctx_tx;
    void *priv_ctx_rx;
    u8 tx_conf;
    u8 rx_conf;
    struct cipher_context tx;
    struct cipher_context rx;
    struct scatterlist *partially_sent_record;
    u16 partially_sent_offset;
    long unsigned int flags;
    bool in_tcp_sendpages;
    bool pending_open_record_frags;
    int (*push_pending_record)(struct sock *, int);
    void (*sk_write_space)(struct sock *);
    void (*sk_destruct)(struct sock *);
    void (*sk_proto_close)(struct sock *, long int);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*hash)(struct sock *);
    void (*unhash)(struct sock *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct tls_context {
    struct tls_prot_info prot_info;
    u8 tx_conf;
    u8 rx_conf;
    int (*push_pending_record)(struct sock *, int);
    void (*sk_write_space)(struct sock *);
    void *priv_ctx_tx;
    void *priv_ctx_rx;
    struct net_device *netdev;
    struct cipher_context tx;
    struct cipher_context rx;
    struct scatterlist *partially_sent_record;
    u16 partially_sent_offset;
    bool in_tcp_sendpages;
    bool pending_open_record_frags;
    long unsigned int flags;
    struct proto *sk_proto;
    void (*sk_destruct)(struct sock *);
    void (*sk_proto_close)(struct sock *, long int);
    int (*setsockopt)(struct sock *, int, int, char *, unsigned int);
    int (*getsockopt)(struct sock *, int, int, char *, int *);
    int (*hash)(struct sock *);
    void (*unhash)(struct sock *);
    union tls_crypto_context crypto_send;
    union tls_crypto_context crypto_recv;
    struct list_head list;
    refcount_t refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct tls_context {
    struct tls_prot_info prot_info;
    u8 tx_conf;
    u8 rx_conf;
    int (*push_pending_record)(struct sock *, int);
    void (*sk_write_space)(struct sock *);
    void *priv_ctx_tx;
    void *priv_ctx_rx;
    struct net_device *netdev;
    struct cipher_context tx;
    struct cipher_context rx;
    struct scatterlist *partially_sent_record;
    u16 partially_sent_offset;
    bool in_tcp_sendpages;
    bool pending_open_record_frags;
    struct mutex tx_lock;
    long unsigned int flags;
    struct proto *sk_proto;
    void (*sk_destruct)(struct sock *);
    union tls_crypto_context crypto_send;
    union tls_crypto_context crypto_recv;
    struct list_head list;
    refcount_t refcount;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct tls_context {
    struct tls_prot_info prot_info;
    u8 tx_conf;
    u8 rx_conf;
    int (*push_pending_record)(struct sock *, int);
    void (*sk_write_space)(struct sock *);
    void *priv_ctx_tx;
    void *priv_ctx_rx;
    struct net_device *netdev;
    struct cipher_context tx;
    struct cipher_context rx;
    struct scatterlist *partially_sent_record;
    u16 partially_sent_offset;
    bool in_tcp_sendpages;
    bool pending_open_record_frags;
    struct mutex tx_lock;
    long unsigned int flags;
    struct proto *sk_proto;
    void (*sk_destruct)(struct sock *);
    union tls_crypto_context crypto_send;
    union tls_crypto_context crypto_recv;
    struct list_head list;
    refcount_t refcount;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct tls_context {
    struct tls_prot_info prot_info;
    u8 tx_conf;
    u8 rx_conf;
    int (*push_pending_record)(struct sock *, int);
    void (*sk_write_space)(struct sock *);
    void *priv_ctx_tx;
    void *priv_ctx_rx;
    struct net_device *netdev;
    struct cipher_context tx;
    struct cipher_context rx;
    struct scatterlist *partially_sent_record;
    u16 partially_sent_offset;
    bool in_tcp_sendpages;
    bool pending_open_record_frags;
    struct mutex tx_lock;
    long unsigned int flags;
    struct proto *sk_proto;
    void (*sk_destruct)(struct sock *);
    union tls_crypto_context crypto_send;
    union tls_crypto_context crypto_recv;
    struct list_head list;
    refcount_t refcount;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct tls_context {
    struct tls_prot_info prot_info;
    u8 tx_conf;
    u8 rx_conf;
    int (*push_pending_record)(struct sock *, int);
    void (*sk_write_space)(struct sock *);
    void *priv_ctx_tx;
    void *priv_ctx_rx;
    struct net_device *netdev;
    struct cipher_context tx;
    struct cipher_context rx;
    struct scatterlist *partially_sent_record;
    u16 partially_sent_offset;
    bool in_tcp_sendpages;
    bool pending_open_record_frags;
    struct mutex tx_lock;
    long unsigned int flags;
    struct proto *sk_proto;
    struct sock *sk;
    void (*sk_destruct)(struct sock *);
    union tls_crypto_context crypto_send;
    union tls_crypto_context crypto_recv;
    struct list_head list;
    refcount_t refcount;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct tls_context {
    struct tls_prot_info prot_info;
    u8 tx_conf;
    u8 rx_conf;
    int (*push_pending_record)(struct sock *, int);
    void (*sk_write_space)(struct sock *);
    void *priv_ctx_tx;
    void *priv_ctx_rx;
    struct net_device *netdev;
    struct cipher_context tx;
    struct cipher_context rx;
    struct scatterlist *partially_sent_record;
    u16 partially_sent_offset;
    bool in_tcp_sendpages;
    bool pending_open_record_frags;
    struct mutex tx_lock;
    long unsigned int flags;
    struct proto *sk_proto;
    struct sock *sk;
    void (*sk_destruct)(struct sock *);
    union tls_crypto_context crypto_send;
    union tls_crypto_context crypto_recv;
    struct list_head list;
    refcount_t refcount;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct tls_context {
    struct tls_prot_info prot_info;
    u8 tx_conf;
    u8 rx_conf;
    u8 zerocopy_sendfile;
    int (*push_pending_record)(struct sock *, int);
    void (*sk_write_space)(struct sock *);
    void *priv_ctx_tx;
    void *priv_ctx_rx;
    struct net_device *netdev;
    struct cipher_context tx;
    struct cipher_context rx;
    struct scatterlist *partially_sent_record;
    u16 partially_sent_offset;
    bool in_tcp_sendpages;
    bool pending_open_record_frags;
    struct mutex tx_lock;
    long unsigned int flags;
    struct proto *sk_proto;
    struct sock *sk;
    void (*sk_destruct)(struct sock *);
    union tls_crypto_context crypto_send;
    union tls_crypto_context crypto_recv;
    struct list_head list;
    refcount_t refcount;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct tls_context {
    struct tls_prot_info prot_info;
    u8 tx_conf;
    u8 rx_conf;
    u8 zerocopy_sendfile;
    u8 rx_no_pad;
    int (*push_pending_record)(struct sock *, int);
    void (*sk_write_space)(struct sock *);
    void *priv_ctx_tx;
    void *priv_ctx_rx;
    struct net_device *netdev;
    struct cipher_context tx;
    struct cipher_context rx;
    struct scatterlist *partially_sent_record;
    u16 partially_sent_offset;
    bool in_tcp_sendpages;
    bool pending_open_record_frags;
    struct mutex tx_lock;
    long unsigned int flags;
    struct proto *sk_proto;
    struct sock *sk;
    void (*sk_destruct)(struct sock *);
    union tls_crypto_context crypto_send;
    union tls_crypto_context crypto_recv;
    struct list_head list;
    refcount_t refcount;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct tls_context {
    struct tls_prot_info prot_info;
    u8 tx_conf;
    u8 rx_conf;
    u8 zerocopy_sendfile;
    u8 rx_no_pad;
    int (*push_pending_record)(struct sock *, int);
    void (*sk_write_space)(struct sock *);
    void *priv_ctx_tx;
    void *priv_ctx_rx;
    struct net_device *netdev;
    struct cipher_context tx;
    struct cipher_context rx;
    struct scatterlist *partially_sent_record;
    u16 partially_sent_offset;
    bool splicing_pages;
    bool pending_open_record_frags;
    struct mutex tx_lock;
    long unsigned int flags;
    struct proto *sk_proto;
    struct sock *sk;
    void (*sk_destruct)(struct sock *);
    union tls_crypto_context crypto_send;
    union tls_crypto_context crypto_recv;
    struct list_head list;
    refcount_t refcount;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct tls_context {
    struct tls_prot_info prot_info;
    u8 tx_conf;
    u8 rx_conf;
    u8 zerocopy_sendfile;
    u8 rx_no_pad;
    int (*push_pending_record)(struct sock *, int);
    void (*sk_write_space)(struct sock *);
    void *priv_ctx_tx;
    void *priv_ctx_rx;
    struct net_device *netdev;
    struct cipher_context tx;
    struct cipher_context rx;
    struct scatterlist *partially_sent_record;
    u16 partially_sent_offset;
    bool splicing_pages;
    bool pending_open_record_frags;
    struct mutex tx_lock;
    long unsigned int flags;
    struct proto *sk_proto;
    struct sock *sk;
    void (*sk_destruct)(struct sock *);
    union tls_crypto_context crypto_send;
    union tls_crypto_context crypto_recv;
    struct list_head list;
    refcount_t refcount;
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
struct tls_context {
    struct tls_prot_info prot_info;
    u8 tx_conf;
    u8 rx_conf;
    int (*push_pending_record)(struct sock *, int);
    void (*sk_write_space)(struct sock *);
    void *priv_ctx_tx;
    void *priv_ctx_rx;
    struct net_device *netdev;
    struct cipher_context tx;
    struct cipher_context rx;
    struct scatterlist *partially_sent_record;
    u16 partially_sent_offset;
    bool in_tcp_sendpages;
    bool pending_open_record_frags;
    struct mutex tx_lock;
    long unsigned int flags;
    struct proto *sk_proto;
    void (*sk_destruct)(struct sock *);
    union tls_crypto_context crypto_send;
    union tls_crypto_context crypto_recv;
    struct list_head list;
    refcount_t refcount;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct tls_context {
    struct tls_prot_info prot_info;
    u8 tx_conf;
    u8 rx_conf;
    int (*push_pending_record)(struct sock *, int);
    void (*sk_write_space)(struct sock *);
    void *priv_ctx_tx;
    void *priv_ctx_rx;
    struct net_device *netdev;
    struct cipher_context tx;
    struct cipher_context rx;
    struct scatterlist *partially_sent_record;
    u16 partially_sent_offset;
    bool in_tcp_sendpages;
    bool pending_open_record_frags;
    struct mutex tx_lock;
    long unsigned int flags;
    struct proto *sk_proto;
    void (*sk_destruct)(struct sock *);
    union tls_crypto_context crypto_send;
    union tls_crypto_context crypto_recv;
    struct list_head list;
    refcount_t refcount;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct tls_context {
    struct tls_prot_info prot_info;
    u8 tx_conf;
    u8 rx_conf;
    int (*push_pending_record)(struct sock *, int);
    void (*sk_write_space)(struct sock *);
    void *priv_ctx_tx;
    void *priv_ctx_rx;
    struct net_device *netdev;
    struct cipher_context tx;
    struct cipher_context rx;
    struct scatterlist *partially_sent_record;
    u16 partially_sent_offset;
    bool in_tcp_sendpages;
    bool pending_open_record_frags;
    struct mutex tx_lock;
    long unsigned int flags;
    struct proto *sk_proto;
    void (*sk_destruct)(struct sock *);
    union tls_crypto_context crypto_send;
    union tls_crypto_context crypto_recv;
    struct list_head list;
    refcount_t refcount;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct tls_context {
    struct tls_prot_info prot_info;
    u8 tx_conf;
    u8 rx_conf;
    int (*push_pending_record)(struct sock *, int);
    void (*sk_write_space)(struct sock *);
    void *priv_ctx_tx;
    void *priv_ctx_rx;
    struct net_device *netdev;
    struct cipher_context tx;
    struct cipher_context rx;
    struct scatterlist *partially_sent_record;
    u16 partially_sent_offset;
    bool in_tcp_sendpages;
    bool pending_open_record_frags;
    struct mutex tx_lock;
    long unsigned int flags;
    struct proto *sk_proto;
    void (*sk_destruct)(struct sock *);
    union tls_crypto_context crypto_send;
    union tls_crypto_context crypto_recv;
    struct list_head list;
    refcount_t refcount;
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
struct tls_context {
    struct tls_prot_info prot_info;
    u8 tx_conf;
    u8 rx_conf;
    int (*push_pending_record)(struct sock *, int);
    void (*sk_write_space)(struct sock *);
    void *priv_ctx_tx;
    void *priv_ctx_rx;
    struct net_device *netdev;
    struct cipher_context tx;
    struct cipher_context rx;
    struct scatterlist *partially_sent_record;
    u16 partially_sent_offset;
    bool in_tcp_sendpages;
    bool pending_open_record_frags;
    struct mutex tx_lock;
    long unsigned int flags;
    struct proto *sk_proto;
    void (*sk_destruct)(struct sock *);
    union tls_crypto_context crypto_send;
    union tls_crypto_context crypto_recv;
    struct list_head list;
    refcount_t refcount;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct tls_context {
    struct tls_prot_info prot_info;
    u8 tx_conf;
    u8 rx_conf;
    int (*push_pending_record)(struct sock *, int);
    void (*sk_write_space)(struct sock *);
    void *priv_ctx_tx;
    void *priv_ctx_rx;
    struct net_device *netdev;
    struct cipher_context tx;
    struct cipher_context rx;
    struct scatterlist *partially_sent_record;
    u16 partially_sent_offset;
    bool in_tcp_sendpages;
    bool pending_open_record_frags;
    struct mutex tx_lock;
    long unsigned int flags;
    struct proto *sk_proto;
    void (*sk_destruct)(struct sock *);
    union tls_crypto_context crypto_send;
    union tls_crypto_context crypto_recv;
    struct list_head list;
    refcount_t refcount;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct tls_context {
    struct tls_prot_info prot_info;
    u8 tx_conf;
    u8 rx_conf;
    int (*push_pending_record)(struct sock *, int);
    void (*sk_write_space)(struct sock *);
    void *priv_ctx_tx;
    void *priv_ctx_rx;
    struct net_device *netdev;
    struct cipher_context tx;
    struct cipher_context rx;
    struct scatterlist *partially_sent_record;
    u16 partially_sent_offset;
    bool in_tcp_sendpages;
    bool pending_open_record_frags;
    struct mutex tx_lock;
    long unsigned int flags;
    struct proto *sk_proto;
    void (*sk_destruct)(struct sock *);
    union tls_crypto_context crypto_send;
    union tls_crypto_context crypto_recv;
    struct list_head list;
    refcount_t refcount;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct tls_context {
    struct tls_prot_info prot_info;
    u8 tx_conf;
    u8 rx_conf;
    int (*push_pending_record)(struct sock *, int);
    void (*sk_write_space)(struct sock *);
    void *priv_ctx_tx;
    void *priv_ctx_rx;
    struct net_device *netdev;
    struct cipher_context tx;
    struct cipher_context rx;
    struct scatterlist *partially_sent_record;
    u16 partially_sent_offset;
    bool in_tcp_sendpages;
    bool pending_open_record_frags;
    struct mutex tx_lock;
    long unsigned int flags;
    struct proto *sk_proto;
    void (*sk_destruct)(struct sock *);
    union tls_crypto_context crypto_send;
    union tls_crypto_context crypto_recv;
    struct list_head list;
    refcount_t refcount;
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
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct tls_prot_info prot_info</code>
</li>
<li>
<b>Field added. </b>
<code>struct proto *sk_proto</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct mutex tx_lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct callback_head rcu</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*sk_proto_close)(struct sock *, long int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*setsockopt)(struct sock *, int, int, char *, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*getsockopt)(struct sock *, int, int, char *, int *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*hash)(struct sock *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*unhash)(struct sock *)</code>
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
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct sock *sk</code>
</li>
</ul>
</details>
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
<code>u8 zerocopy_sendfile</code>
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
<code>u8 rx_no_pad</code>
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
<code>bool splicing_pages</code>
</li>
<li>
<b>Field removed. </b>
<code>bool in_tcp_sendpages</code>
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
