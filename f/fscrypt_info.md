# Struct: <code>fscrypt_info</code>

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
struct fscrypt_info {
    u8 ci_data_mode;
    u8 ci_filename_mode;
    u8 ci_flags;
    struct crypto_skcipher *ci_ctfm;
    struct key *ci_keyring_key;
    u8 ci_master_key[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct fscrypt_info {
    u8 ci_data_mode;
    u8 ci_filename_mode;
    u8 ci_flags;
    struct crypto_skcipher *ci_ctfm;
    u8 ci_master_key[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct fscrypt_info {
    u8 ci_data_mode;
    u8 ci_filename_mode;
    u8 ci_flags;
    struct crypto_skcipher *ci_ctfm;
    struct crypto_cipher *ci_essiv_tfm;
    u8 ci_master_key[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct fscrypt_info {
    u8 ci_data_mode;
    u8 ci_filename_mode;
    u8 ci_flags;
    struct crypto_skcipher *ci_ctfm;
    struct crypto_cipher *ci_essiv_tfm;
    u8 ci_master_key[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct fscrypt_info {
    u8 ci_data_mode;
    u8 ci_filename_mode;
    u8 ci_flags;
    struct crypto_skcipher *ci_ctfm;
    struct crypto_cipher *ci_essiv_tfm;
    u8 ci_master_key[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct fscrypt_info {
    struct crypto_skcipher *ci_ctfm;
    struct crypto_cipher *ci_essiv_tfm;
    struct fscrypt_mode *ci_mode;
    struct fscrypt_master_key *ci_master_key;
    u8 ci_data_mode;
    u8 ci_filename_mode;
    u8 ci_flags;
    u8 ci_master_key_descriptor[8];
    u8 ci_nonce[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct fscrypt_info {
    struct crypto_skcipher *ci_ctfm;
    struct crypto_cipher *ci_essiv_tfm;
    struct fscrypt_mode *ci_mode;
    struct fscrypt_master_key *ci_master_key;
    u8 ci_data_mode;
    u8 ci_filename_mode;
    u8 ci_flags;
    u8 ci_master_key_descriptor[8];
    u8 ci_nonce[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct fscrypt_info {
    struct crypto_skcipher *ci_ctfm;
    struct crypto_cipher *ci_essiv_tfm;
    struct fscrypt_mode *ci_mode;
    struct inode *ci_inode;
    struct key *ci_master_key;
    struct list_head ci_master_key_link;
    struct fscrypt_direct_key *ci_direct_key;
    union fscrypt_policy ci_policy;
    u8 ci_nonce[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct fscrypt_info {
    struct crypto_skcipher *ci_ctfm;
    bool ci_owns_key;
    struct fscrypt_mode *ci_mode;
    struct inode *ci_inode;
    struct key *ci_master_key;
    struct list_head ci_master_key_link;
    struct fscrypt_direct_key *ci_direct_key;
    siphash_key_t ci_dirhash_key;
    bool ci_dirhash_key_initialized;
    union fscrypt_policy ci_policy;
    u8 ci_nonce[16];
    u32 ci_hashed_ino;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct fscrypt_info {
    struct fscrypt_prepared_key ci_enc_key;
    bool ci_owns_key;
    bool ci_inlinecrypt;
    struct fscrypt_mode *ci_mode;
    struct inode *ci_inode;
    struct key *ci_master_key;
    struct list_head ci_master_key_link;
    struct fscrypt_direct_key *ci_direct_key;
    siphash_key_t ci_dirhash_key;
    bool ci_dirhash_key_initialized;
    union fscrypt_policy ci_policy;
    u8 ci_nonce[16];
    u32 ci_hashed_ino;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct fscrypt_info {
    struct fscrypt_prepared_key ci_enc_key;
    bool ci_owns_key;
    bool ci_inlinecrypt;
    struct fscrypt_mode *ci_mode;
    struct inode *ci_inode;
    struct key *ci_master_key;
    struct list_head ci_master_key_link;
    struct fscrypt_direct_key *ci_direct_key;
    siphash_key_t ci_dirhash_key;
    bool ci_dirhash_key_initialized;
    union fscrypt_policy ci_policy;
    u8 ci_nonce[16];
    u32 ci_hashed_ino;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct fscrypt_info {
    struct fscrypt_prepared_key ci_enc_key;
    bool ci_owns_key;
    bool ci_inlinecrypt;
    struct fscrypt_mode *ci_mode;
    struct inode *ci_inode;
    struct key *ci_master_key;
    struct list_head ci_master_key_link;
    struct fscrypt_direct_key *ci_direct_key;
    siphash_key_t ci_dirhash_key;
    bool ci_dirhash_key_initialized;
    union fscrypt_policy ci_policy;
    u8 ci_nonce[16];
    u32 ci_hashed_ino;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct fscrypt_info {
    struct fscrypt_prepared_key ci_enc_key;
    bool ci_owns_key;
    bool ci_inlinecrypt;
    struct fscrypt_mode *ci_mode;
    struct inode *ci_inode;
    struct key *ci_master_key;
    struct list_head ci_master_key_link;
    struct fscrypt_direct_key *ci_direct_key;
    siphash_key_t ci_dirhash_key;
    bool ci_dirhash_key_initialized;
    union fscrypt_policy ci_policy;
    u8 ci_nonce[16];
    u32 ci_hashed_ino;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct fscrypt_info {
    struct fscrypt_prepared_key ci_enc_key;
    bool ci_owns_key;
    bool ci_inlinecrypt;
    struct fscrypt_mode *ci_mode;
    struct inode *ci_inode;
    struct fscrypt_master_key *ci_master_key;
    struct list_head ci_master_key_link;
    struct fscrypt_direct_key *ci_direct_key;
    siphash_key_t ci_dirhash_key;
    bool ci_dirhash_key_initialized;
    union fscrypt_policy ci_policy;
    u8 ci_nonce[16];
    u32 ci_hashed_ino;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct fscrypt_info {
    struct fscrypt_prepared_key ci_enc_key;
    bool ci_owns_key;
    bool ci_inlinecrypt;
    struct fscrypt_mode *ci_mode;
    struct inode *ci_inode;
    struct fscrypt_master_key *ci_master_key;
    struct list_head ci_master_key_link;
    struct fscrypt_direct_key *ci_direct_key;
    siphash_key_t ci_dirhash_key;
    bool ci_dirhash_key_initialized;
    union fscrypt_policy ci_policy;
    u8 ci_nonce[16];
    u32 ci_hashed_ino;
};
```
</details>
</li>
<li>
In <code>6.8</code>: Absent ⚠️
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct fscrypt_info {
    struct crypto_skcipher *ci_ctfm;
    struct crypto_cipher *ci_essiv_tfm;
    struct fscrypt_mode *ci_mode;
    struct inode *ci_inode;
    struct key *ci_master_key;
    struct list_head ci_master_key_link;
    struct fscrypt_direct_key *ci_direct_key;
    union fscrypt_policy ci_policy;
    u8 ci_nonce[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct fscrypt_info {
    struct crypto_skcipher *ci_ctfm;
    struct crypto_cipher *ci_essiv_tfm;
    struct fscrypt_mode *ci_mode;
    struct inode *ci_inode;
    struct key *ci_master_key;
    struct list_head ci_master_key_link;
    struct fscrypt_direct_key *ci_direct_key;
    union fscrypt_policy ci_policy;
    u8 ci_nonce[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct fscrypt_info {
    struct crypto_skcipher *ci_ctfm;
    struct crypto_cipher *ci_essiv_tfm;
    struct fscrypt_mode *ci_mode;
    struct inode *ci_inode;
    struct key *ci_master_key;
    struct list_head ci_master_key_link;
    struct fscrypt_direct_key *ci_direct_key;
    union fscrypt_policy ci_policy;
    u8 ci_nonce[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct fscrypt_info {
    struct crypto_skcipher *ci_ctfm;
    struct crypto_cipher *ci_essiv_tfm;
    struct fscrypt_mode *ci_mode;
    struct inode *ci_inode;
    struct key *ci_master_key;
    struct list_head ci_master_key_link;
    struct fscrypt_direct_key *ci_direct_key;
    union fscrypt_policy ci_policy;
    u8 ci_nonce[16];
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
struct fscrypt_info {
    struct crypto_skcipher *ci_ctfm;
    struct crypto_cipher *ci_essiv_tfm;
    struct fscrypt_mode *ci_mode;
    struct inode *ci_inode;
    struct key *ci_master_key;
    struct list_head ci_master_key_link;
    struct fscrypt_direct_key *ci_direct_key;
    union fscrypt_policy ci_policy;
    u8 ci_nonce[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct fscrypt_info {
    struct crypto_skcipher *ci_ctfm;
    struct crypto_cipher *ci_essiv_tfm;
    struct fscrypt_mode *ci_mode;
    struct inode *ci_inode;
    struct key *ci_master_key;
    struct list_head ci_master_key_link;
    struct fscrypt_direct_key *ci_direct_key;
    union fscrypt_policy ci_policy;
    u8 ci_nonce[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct fscrypt_info {
    struct crypto_skcipher *ci_ctfm;
    struct crypto_cipher *ci_essiv_tfm;
    struct fscrypt_mode *ci_mode;
    struct inode *ci_inode;
    struct key *ci_master_key;
    struct list_head ci_master_key_link;
    struct fscrypt_direct_key *ci_direct_key;
    union fscrypt_policy ci_policy;
    u8 ci_nonce[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct fscrypt_info {
    struct crypto_skcipher *ci_ctfm;
    struct crypto_cipher *ci_essiv_tfm;
    struct fscrypt_mode *ci_mode;
    struct inode *ci_inode;
    struct key *ci_master_key;
    struct list_head ci_master_key_link;
    struct fscrypt_direct_key *ci_direct_key;
    union fscrypt_policy ci_policy;
    u8 ci_nonce[16];
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
<b>Field removed. </b>
<code>struct key *ci_keyring_key</code>
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
<code>struct crypto_cipher *ci_essiv_tfm</code>
</li>
</ul>
</details>
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
<code>struct fscrypt_mode *ci_mode</code>
</li>
<li>
<b>Field added. </b>
<code>u8 ci_master_key_descriptor[8]</code>
</li>
<li>
<b>Field added. </b>
<code>u8 ci_nonce[16]</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 ci_master_key[8]</code> ➡️ <code>struct fscrypt_master_key *ci_master_key</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct inode *ci_inode</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head ci_master_key_link</code>
</li>
<li>
<b>Field added. </b>
<code>struct fscrypt_direct_key *ci_direct_key</code>
</li>
<li>
<b>Field added. </b>
<code>union fscrypt_policy ci_policy</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 ci_data_mode</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 ci_filename_mode</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 ci_flags</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 ci_master_key_descriptor[8]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct fscrypt_master_key *ci_master_key</code> ➡️ <code>struct key *ci_master_key</code>
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
<code>bool ci_owns_key</code>
</li>
<li>
<b>Field added. </b>
<code>siphash_key_t ci_dirhash_key</code>
</li>
<li>
<b>Field added. </b>
<code>bool ci_dirhash_key_initialized</code>
</li>
<li>
<b>Field added. </b>
<code>u32 ci_hashed_ino</code>
</li>
<li>
<b>Field removed. </b>
<code>struct crypto_cipher *ci_essiv_tfm</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct fscrypt_prepared_key ci_enc_key</code>
</li>
<li>
<b>Field added. </b>
<code>bool ci_inlinecrypt</code>
</li>
<li>
<b>Field removed. </b>
<code>struct crypto_skcipher *ci_ctfm</code>
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
<b>Field type changed. </b>
<code>struct key *ci_master_key</code> ➡️ <code>struct fscrypt_master_key *ci_master_key</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
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
