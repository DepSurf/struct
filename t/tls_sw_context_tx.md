# Struct: <code>tls_sw_context_tx</code>

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
struct tls_sw_context_tx {
    struct crypto_aead *aead_send;
    struct crypto_wait async_wait;
    struct tx_work tx_work;
    struct tls_rec *open_rec;
    struct list_head tx_list;
    atomic_t encrypt_pending;
    int async_notify;
    long unsigned int tx_bitmask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct tls_sw_context_tx {
    struct crypto_aead *aead_send;
    struct crypto_wait async_wait;
    struct tx_work tx_work;
    struct tls_rec *open_rec;
    struct list_head tx_list;
    atomic_t encrypt_pending;
    int async_notify;
    int async_capable;
    long unsigned int tx_bitmask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct tls_sw_context_tx {
    struct crypto_aead *aead_send;
    struct crypto_wait async_wait;
    struct tx_work tx_work;
    struct tls_rec *open_rec;
    struct list_head tx_list;
    atomic_t encrypt_pending;
    int async_notify;
    int async_capable;
    long unsigned int tx_bitmask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct tls_sw_context_tx {
    struct crypto_aead *aead_send;
    struct crypto_wait async_wait;
    struct tx_work tx_work;
    struct tls_rec *open_rec;
    struct list_head tx_list;
    atomic_t encrypt_pending;
    spinlock_t encrypt_compl_lock;
    int async_notify;
    u8 async_capable;
    long unsigned int tx_bitmask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct tls_sw_context_tx {
    struct crypto_aead *aead_send;
    struct crypto_wait async_wait;
    struct tx_work tx_work;
    struct tls_rec *open_rec;
    struct list_head tx_list;
    atomic_t encrypt_pending;
    spinlock_t encrypt_compl_lock;
    int async_notify;
    u8 async_capable;
    long unsigned int tx_bitmask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct tls_sw_context_tx {
    struct crypto_aead *aead_send;
    struct crypto_wait async_wait;
    struct tx_work tx_work;
    struct tls_rec *open_rec;
    struct list_head tx_list;
    atomic_t encrypt_pending;
    spinlock_t encrypt_compl_lock;
    int async_notify;
    u8 async_capable;
    long unsigned int tx_bitmask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct tls_sw_context_tx {
    struct crypto_aead *aead_send;
    struct crypto_wait async_wait;
    struct tx_work tx_work;
    struct tls_rec *open_rec;
    struct list_head tx_list;
    atomic_t encrypt_pending;
    spinlock_t encrypt_compl_lock;
    int async_notify;
    u8 async_capable;
    long unsigned int tx_bitmask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct tls_sw_context_tx {
    struct crypto_aead *aead_send;
    struct crypto_wait async_wait;
    struct tx_work tx_work;
    struct tls_rec *open_rec;
    struct list_head tx_list;
    atomic_t encrypt_pending;
    spinlock_t encrypt_compl_lock;
    int async_notify;
    u8 async_capable;
    long unsigned int tx_bitmask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct tls_sw_context_tx {
    struct crypto_aead *aead_send;
    struct crypto_wait async_wait;
    struct tx_work tx_work;
    struct tls_rec *open_rec;
    struct list_head tx_list;
    atomic_t encrypt_pending;
    spinlock_t encrypt_compl_lock;
    int async_notify;
    u8 async_capable;
    long unsigned int tx_bitmask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct tls_sw_context_tx {
    struct crypto_aead *aead_send;
    struct crypto_wait async_wait;
    struct tx_work tx_work;
    struct tls_rec *open_rec;
    struct list_head tx_list;
    atomic_t encrypt_pending;
    spinlock_t encrypt_compl_lock;
    int async_notify;
    u8 async_capable;
    long unsigned int tx_bitmask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct tls_sw_context_tx {
    struct crypto_aead *aead_send;
    struct crypto_wait async_wait;
    struct tx_work tx_work;
    struct tls_rec *open_rec;
    struct list_head tx_list;
    atomic_t encrypt_pending;
    u8 async_capable;
    long unsigned int tx_bitmask;
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
struct tls_sw_context_tx {
    struct crypto_aead *aead_send;
    struct crypto_wait async_wait;
    struct tx_work tx_work;
    struct tls_rec *open_rec;
    struct list_head tx_list;
    atomic_t encrypt_pending;
    int async_notify;
    int async_capable;
    long unsigned int tx_bitmask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct tls_sw_context_tx {
    struct crypto_aead *aead_send;
    struct crypto_wait async_wait;
    struct tx_work tx_work;
    struct tls_rec *open_rec;
    struct list_head tx_list;
    atomic_t encrypt_pending;
    int async_notify;
    int async_capable;
    long unsigned int tx_bitmask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct tls_sw_context_tx {
    struct crypto_aead *aead_send;
    struct crypto_wait async_wait;
    struct tx_work tx_work;
    struct tls_rec *open_rec;
    struct list_head tx_list;
    atomic_t encrypt_pending;
    int async_notify;
    int async_capable;
    long unsigned int tx_bitmask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct tls_sw_context_tx {
    struct crypto_aead *aead_send;
    struct crypto_wait async_wait;
    struct tx_work tx_work;
    struct tls_rec *open_rec;
    struct list_head tx_list;
    atomic_t encrypt_pending;
    int async_notify;
    int async_capable;
    long unsigned int tx_bitmask;
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
struct tls_sw_context_tx {
    struct crypto_aead *aead_send;
    struct crypto_wait async_wait;
    struct tx_work tx_work;
    struct tls_rec *open_rec;
    struct list_head tx_list;
    atomic_t encrypt_pending;
    int async_notify;
    int async_capable;
    long unsigned int tx_bitmask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct tls_sw_context_tx {
    struct crypto_aead *aead_send;
    struct crypto_wait async_wait;
    struct tx_work tx_work;
    struct tls_rec *open_rec;
    struct list_head tx_list;
    atomic_t encrypt_pending;
    int async_notify;
    int async_capable;
    long unsigned int tx_bitmask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct tls_sw_context_tx {
    struct crypto_aead *aead_send;
    struct crypto_wait async_wait;
    struct tx_work tx_work;
    struct tls_rec *open_rec;
    struct list_head tx_list;
    atomic_t encrypt_pending;
    int async_notify;
    int async_capable;
    long unsigned int tx_bitmask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct tls_sw_context_tx {
    struct crypto_aead *aead_send;
    struct crypto_wait async_wait;
    struct tx_work tx_work;
    struct tls_rec *open_rec;
    struct list_head tx_list;
    atomic_t encrypt_pending;
    int async_notify;
    int async_capable;
    long unsigned int tx_bitmask;
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
<code>int async_capable</code>
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
<code>spinlock_t encrypt_compl_lock</code>
</li>
<li>
<b>Field type changed. </b>
<code>int async_capable</code> ➡️ <code>u8 async_capable</code>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct tls_rec *open_rec</code> ➡️ <code>struct tls_rec *open_rec</code>
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
<code>spinlock_t encrypt_compl_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>int async_notify</code>
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
