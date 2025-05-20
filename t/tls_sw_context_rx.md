# Struct: <code>tls_sw_context_rx</code>

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
In <code>5.0</code>: Absent ⚠️
</li>
<li>
In <code>5.3</code>: Absent ⚠️
</li>
<li>
In <code>5.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct tls_sw_context_rx {
    struct crypto_aead *aead_recv;
    struct crypto_wait async_wait;
    struct strparser strp;
    struct sk_buff_head rx_list;
    void (*saved_data_ready)(struct sock *);
    struct sk_buff *recv_pkt;
    u8 control;
    u8 async_capable;
    u8 decrypted;
    atomic_t decrypt_pending;
    spinlock_t decrypt_compl_lock;
    bool async_notify;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct tls_sw_context_rx {
    struct crypto_aead *aead_recv;
    struct crypto_wait async_wait;
    struct strparser strp;
    struct sk_buff_head rx_list;
    void (*saved_data_ready)(struct sock *);
    struct sk_buff *recv_pkt;
    u8 control;
    u8 async_capable;
    u8 decrypted;
    atomic_t decrypt_pending;
    spinlock_t decrypt_compl_lock;
    bool async_notify;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct tls_sw_context_rx {
    struct crypto_aead *aead_recv;
    struct crypto_wait async_wait;
    struct strparser strp;
    struct sk_buff_head rx_list;
    void (*saved_data_ready)(struct sock *);
    struct sk_buff *recv_pkt;
    u8 control;
    u8 async_capable;
    u8 decrypted;
    atomic_t decrypt_pending;
    spinlock_t decrypt_compl_lock;
    bool async_notify;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct tls_sw_context_rx {
    struct crypto_aead *aead_recv;
    struct crypto_wait async_wait;
    struct strparser strp;
    struct sk_buff_head rx_list;
    void (*saved_data_ready)(struct sock *);
    struct sk_buff *recv_pkt;
    u8 control;
    u8 async_capable;
    u8 decrypted;
    atomic_t decrypt_pending;
    spinlock_t decrypt_compl_lock;
    bool async_notify;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct tls_sw_context_rx {
    struct crypto_aead *aead_recv;
    struct crypto_wait async_wait;
    struct strparser strp;
    struct sk_buff_head rx_list;
    void (*saved_data_ready)(struct sock *);
    struct sk_buff *recv_pkt;
    u8 async_capable;
    atomic_t decrypt_pending;
    spinlock_t decrypt_compl_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct tls_sw_context_rx {
    struct crypto_aead *aead_recv;
    struct crypto_wait async_wait;
    struct sk_buff_head rx_list;
    void (*saved_data_ready)(struct sock *);
    u8 reader_present;
    u8 async_capable;
    u8 zc_capable;
    u8 reader_contended;
    struct tls_strparser strp;
    atomic_t decrypt_pending;
    spinlock_t decrypt_compl_lock;
    struct sk_buff_head async_hold;
    struct wait_queue_head wq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct tls_sw_context_rx {
    struct crypto_aead *aead_recv;
    struct crypto_wait async_wait;
    struct sk_buff_head rx_list;
    void (*saved_data_ready)(struct sock *);
    u8 reader_present;
    u8 async_capable;
    u8 zc_capable;
    u8 reader_contended;
    struct tls_strparser strp;
    atomic_t decrypt_pending;
    spinlock_t decrypt_compl_lock;
    struct sk_buff_head async_hold;
    struct wait_queue_head wq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct tls_sw_context_rx {
    struct crypto_aead *aead_recv;
    struct crypto_wait async_wait;
    struct sk_buff_head rx_list;
    void (*saved_data_ready)(struct sock *);
    u8 reader_present;
    u8 async_capable;
    u8 zc_capable;
    u8 reader_contended;
    struct tls_strparser strp;
    atomic_t decrypt_pending;
    struct sk_buff_head async_hold;
    struct wait_queue_head wq;
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
In <code>arm64</code>: Absent ⚠️
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
</li>
<li>
In <code>riscv64</code>: Absent ⚠️
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
In <code>aws</code>: Absent ⚠️
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>u8 control</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 decrypted</code>
</li>
<li>
<b>Field removed. </b>
<code>bool async_notify</code>
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
<code>u8 reader_present</code>
</li>
<li>
<b>Field added. </b>
<code>u8 zc_capable</code>
</li>
<li>
<b>Field added. </b>
<code>u8 reader_contended</code>
</li>
<li>
<b>Field added. </b>
<code>struct sk_buff_head async_hold</code>
</li>
<li>
<b>Field added. </b>
<code>struct wait_queue_head wq</code>
</li>
<li>
<b>Field removed. </b>
<code>struct sk_buff *recv_pkt</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct strparser strp</code> ➡️ <code>struct tls_strparser strp</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>spinlock_t decrypt_compl_lock</code>
</li>
</ul>
</details>
</li>
</ul>
