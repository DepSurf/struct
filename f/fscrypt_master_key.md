# Struct: <code>fscrypt_master_key</code>

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
struct fscrypt_master_key {
    struct hlist_node mk_node;
    refcount_t mk_refcount;
    const struct fscrypt_mode *mk_mode;
    struct crypto_skcipher *mk_ctfm;
    u8 mk_descriptor[8];
    u8 mk_raw[64];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct fscrypt_master_key {
    struct hlist_node mk_node;
    refcount_t mk_refcount;
    const struct fscrypt_mode *mk_mode;
    struct crypto_skcipher *mk_ctfm;
    u8 mk_descriptor[8];
    u8 mk_raw[64];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct fscrypt_master_key {
    struct fscrypt_master_key_secret mk_secret;
    struct rw_semaphore mk_secret_sem;
    struct fscrypt_key_specifier mk_spec;
    struct key *mk_users;
    refcount_t mk_refcount;
    struct list_head mk_decrypted_inodes;
    spinlock_t mk_decrypted_inodes_lock;
    struct crypto_skcipher * mk_mode_keys[10];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct fscrypt_master_key {
    struct fscrypt_master_key_secret mk_secret;
    struct rw_semaphore mk_secret_sem;
    struct fscrypt_key_specifier mk_spec;
    struct key *mk_users;
    refcount_t mk_refcount;
    struct list_head mk_decrypted_inodes;
    spinlock_t mk_decrypted_inodes_lock;
    struct crypto_skcipher * mk_direct_keys[10];
    struct crypto_skcipher * mk_iv_ino_lblk_64_keys[10];
    struct crypto_skcipher * mk_iv_ino_lblk_32_keys[10];
    siphash_key_t mk_ino_hash_key;
    bool mk_ino_hash_key_initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct fscrypt_master_key {
    struct fscrypt_master_key_secret mk_secret;
    struct fscrypt_key_specifier mk_spec;
    struct key *mk_users;
    refcount_t mk_refcount;
    struct list_head mk_decrypted_inodes;
    spinlock_t mk_decrypted_inodes_lock;
    struct fscrypt_prepared_key mk_direct_keys[10];
    struct fscrypt_prepared_key mk_iv_ino_lblk_64_keys[10];
    struct fscrypt_prepared_key mk_iv_ino_lblk_32_keys[10];
    siphash_key_t mk_ino_hash_key;
    bool mk_ino_hash_key_initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct fscrypt_master_key {
    struct fscrypt_master_key_secret mk_secret;
    struct fscrypt_key_specifier mk_spec;
    struct key *mk_users;
    refcount_t mk_refcount;
    struct list_head mk_decrypted_inodes;
    spinlock_t mk_decrypted_inodes_lock;
    struct fscrypt_prepared_key mk_direct_keys[10];
    struct fscrypt_prepared_key mk_iv_ino_lblk_64_keys[10];
    struct fscrypt_prepared_key mk_iv_ino_lblk_32_keys[10];
    siphash_key_t mk_ino_hash_key;
    bool mk_ino_hash_key_initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct fscrypt_master_key {
    struct fscrypt_master_key_secret mk_secret;
    struct fscrypt_key_specifier mk_spec;
    struct key *mk_users;
    refcount_t mk_refcount;
    struct list_head mk_decrypted_inodes;
    spinlock_t mk_decrypted_inodes_lock;
    struct fscrypt_prepared_key mk_direct_keys[10];
    struct fscrypt_prepared_key mk_iv_ino_lblk_64_keys[10];
    struct fscrypt_prepared_key mk_iv_ino_lblk_32_keys[10];
    siphash_key_t mk_ino_hash_key;
    bool mk_ino_hash_key_initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct fscrypt_master_key {
    struct fscrypt_master_key_secret mk_secret;
    struct fscrypt_key_specifier mk_spec;
    struct key *mk_users;
    refcount_t mk_refcount;
    struct list_head mk_decrypted_inodes;
    spinlock_t mk_decrypted_inodes_lock;
    struct fscrypt_prepared_key mk_direct_keys[10];
    struct fscrypt_prepared_key mk_iv_ino_lblk_64_keys[10];
    struct fscrypt_prepared_key mk_iv_ino_lblk_32_keys[10];
    siphash_key_t mk_ino_hash_key;
    bool mk_ino_hash_key_initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct fscrypt_master_key {
    struct hlist_node mk_node;
    struct rw_semaphore mk_sem;
    refcount_t mk_active_refs;
    refcount_t mk_struct_refs;
    struct callback_head mk_rcu_head;
    struct fscrypt_master_key_secret mk_secret;
    struct fscrypt_key_specifier mk_spec;
    struct key *mk_users;
    struct list_head mk_decrypted_inodes;
    spinlock_t mk_decrypted_inodes_lock;
    struct fscrypt_prepared_key mk_direct_keys[11];
    struct fscrypt_prepared_key mk_iv_ino_lblk_64_keys[11];
    struct fscrypt_prepared_key mk_iv_ino_lblk_32_keys[11];
    siphash_key_t mk_ino_hash_key;
    bool mk_ino_hash_key_initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct fscrypt_master_key {
    struct hlist_node mk_node;
    struct rw_semaphore mk_sem;
    refcount_t mk_active_refs;
    refcount_t mk_struct_refs;
    struct callback_head mk_rcu_head;
    struct fscrypt_master_key_secret mk_secret;
    struct fscrypt_key_specifier mk_spec;
    struct key *mk_users;
    struct list_head mk_decrypted_inodes;
    spinlock_t mk_decrypted_inodes_lock;
    struct fscrypt_prepared_key mk_direct_keys[11];
    struct fscrypt_prepared_key mk_iv_ino_lblk_64_keys[11];
    struct fscrypt_prepared_key mk_iv_ino_lblk_32_keys[11];
    siphash_key_t mk_ino_hash_key;
    bool mk_ino_hash_key_initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct fscrypt_master_key {
    struct hlist_node mk_node;
    struct rw_semaphore mk_sem;
    refcount_t mk_active_refs;
    refcount_t mk_struct_refs;
    struct callback_head mk_rcu_head;
    struct fscrypt_master_key_secret mk_secret;
    struct fscrypt_key_specifier mk_spec;
    struct key *mk_users;
    struct list_head mk_decrypted_inodes;
    spinlock_t mk_decrypted_inodes_lock;
    struct fscrypt_prepared_key mk_direct_keys[11];
    struct fscrypt_prepared_key mk_iv_ino_lblk_64_keys[11];
    struct fscrypt_prepared_key mk_iv_ino_lblk_32_keys[11];
    siphash_key_t mk_ino_hash_key;
    bool mk_ino_hash_key_initialized;
    bool mk_present;
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
struct fscrypt_master_key {
    struct fscrypt_master_key_secret mk_secret;
    struct rw_semaphore mk_secret_sem;
    struct fscrypt_key_specifier mk_spec;
    struct key *mk_users;
    refcount_t mk_refcount;
    struct list_head mk_decrypted_inodes;
    spinlock_t mk_decrypted_inodes_lock;
    struct crypto_skcipher * mk_mode_keys[10];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct fscrypt_master_key {
    struct fscrypt_master_key_secret mk_secret;
    struct rw_semaphore mk_secret_sem;
    struct fscrypt_key_specifier mk_spec;
    struct key *mk_users;
    refcount_t mk_refcount;
    struct list_head mk_decrypted_inodes;
    spinlock_t mk_decrypted_inodes_lock;
    struct crypto_skcipher * mk_mode_keys[10];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct fscrypt_master_key {
    struct fscrypt_master_key_secret mk_secret;
    struct rw_semaphore mk_secret_sem;
    struct fscrypt_key_specifier mk_spec;
    struct key *mk_users;
    refcount_t mk_refcount;
    struct list_head mk_decrypted_inodes;
    spinlock_t mk_decrypted_inodes_lock;
    struct crypto_skcipher * mk_mode_keys[10];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct fscrypt_master_key {
    struct fscrypt_master_key_secret mk_secret;
    struct rw_semaphore mk_secret_sem;
    struct fscrypt_key_specifier mk_spec;
    struct key *mk_users;
    refcount_t mk_refcount;
    struct list_head mk_decrypted_inodes;
    spinlock_t mk_decrypted_inodes_lock;
    struct crypto_skcipher * mk_mode_keys[10];
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
struct fscrypt_master_key {
    struct fscrypt_master_key_secret mk_secret;
    struct rw_semaphore mk_secret_sem;
    struct fscrypt_key_specifier mk_spec;
    struct key *mk_users;
    refcount_t mk_refcount;
    struct list_head mk_decrypted_inodes;
    spinlock_t mk_decrypted_inodes_lock;
    struct crypto_skcipher * mk_mode_keys[10];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct fscrypt_master_key {
    struct fscrypt_master_key_secret mk_secret;
    struct rw_semaphore mk_secret_sem;
    struct fscrypt_key_specifier mk_spec;
    struct key *mk_users;
    refcount_t mk_refcount;
    struct list_head mk_decrypted_inodes;
    spinlock_t mk_decrypted_inodes_lock;
    struct crypto_skcipher * mk_mode_keys[10];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct fscrypt_master_key {
    struct fscrypt_master_key_secret mk_secret;
    struct rw_semaphore mk_secret_sem;
    struct fscrypt_key_specifier mk_spec;
    struct key *mk_users;
    refcount_t mk_refcount;
    struct list_head mk_decrypted_inodes;
    spinlock_t mk_decrypted_inodes_lock;
    struct crypto_skcipher * mk_mode_keys[10];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct fscrypt_master_key {
    struct fscrypt_master_key_secret mk_secret;
    struct rw_semaphore mk_secret_sem;
    struct fscrypt_key_specifier mk_spec;
    struct key *mk_users;
    refcount_t mk_refcount;
    struct list_head mk_decrypted_inodes;
    spinlock_t mk_decrypted_inodes_lock;
    struct crypto_skcipher * mk_mode_keys[10];
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
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct fscrypt_master_key_secret mk_secret</code>
</li>
<li>
<b>Field added. </b>
<code>struct rw_semaphore mk_secret_sem</code>
</li>
<li>
<b>Field added. </b>
<code>struct fscrypt_key_specifier mk_spec</code>
</li>
<li>
<b>Field added. </b>
<code>struct key *mk_users</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head mk_decrypted_inodes</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t mk_decrypted_inodes_lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct crypto_skcipher * mk_mode_keys[10]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct hlist_node mk_node</code>
</li>
<li>
<b>Field removed. </b>
<code>const struct fscrypt_mode *mk_mode</code>
</li>
<li>
<b>Field removed. </b>
<code>struct crypto_skcipher *mk_ctfm</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 mk_descriptor[8]</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 mk_raw[64]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct crypto_skcipher * mk_direct_keys[10]</code>
</li>
<li>
<b>Field added. </b>
<code>struct crypto_skcipher * mk_iv_ino_lblk_64_keys[10]</code>
</li>
<li>
<b>Field added. </b>
<code>struct crypto_skcipher * mk_iv_ino_lblk_32_keys[10]</code>
</li>
<li>
<b>Field added. </b>
<code>siphash_key_t mk_ino_hash_key</code>
</li>
<li>
<b>Field added. </b>
<code>bool mk_ino_hash_key_initialized</code>
</li>
<li>
<b>Field removed. </b>
<code>struct crypto_skcipher * mk_mode_keys[10]</code>
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
<code>struct rw_semaphore mk_secret_sem</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct crypto_skcipher * mk_direct_keys[10]</code> ➡️ <code>struct fscrypt_prepared_key mk_direct_keys[10]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct crypto_skcipher * mk_iv_ino_lblk_64_keys[10]</code> ➡️ <code>struct fscrypt_prepared_key mk_iv_ino_lblk_64_keys[10]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct crypto_skcipher * mk_iv_ino_lblk_32_keys[10]</code> ➡️ <code>struct fscrypt_prepared_key mk_iv_ino_lblk_32_keys[10]</code>
</li>
</ul>
</details>
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
<b>Field added. </b>
<code>struct hlist_node mk_node</code>
</li>
<li>
<b>Field added. </b>
<code>struct rw_semaphore mk_sem</code>
</li>
<li>
<b>Field added. </b>
<code>refcount_t mk_active_refs</code>
</li>
<li>
<b>Field added. </b>
<code>refcount_t mk_struct_refs</code>
</li>
<li>
<b>Field added. </b>
<code>struct callback_head mk_rcu_head</code>
</li>
<li>
<b>Field removed. </b>
<code>refcount_t mk_refcount</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct fscrypt_prepared_key mk_direct_keys[10]</code> ➡️ <code>struct fscrypt_prepared_key mk_direct_keys[11]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct fscrypt_prepared_key mk_iv_ino_lblk_64_keys[10]</code> ➡️ <code>struct fscrypt_prepared_key mk_iv_ino_lblk_64_keys[11]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct fscrypt_prepared_key mk_iv_ino_lblk_32_keys[10]</code> ➡️ <code>struct fscrypt_prepared_key mk_iv_ino_lblk_32_keys[11]</code>
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
<b>Field added. </b>
<code>bool mk_present</code>
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
