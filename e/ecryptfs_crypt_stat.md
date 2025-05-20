# Struct: <code>ecryptfs_crypt_stat</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct ecryptfs_crypt_stat {
    u32 flags;
    unsigned int file_version;
    size_t iv_bytes;
    size_t metadata_size;
    size_t extent_size;
    size_t key_size;
    size_t extent_shift;
    unsigned int extent_mask;
    struct ecryptfs_mount_crypt_stat *mount_crypt_stat;
    struct crypto_ablkcipher *tfm;
    struct crypto_hash *hash_tfm;
    unsigned char cipher[32];
    unsigned char key[64];
    unsigned char root_iv[16];
    struct list_head keysig_list;
    struct mutex keysig_list_mutex;
    struct mutex cs_tfm_mutex;
    struct mutex cs_hash_tfm_mutex;
    struct mutex cs_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ecryptfs_crypt_stat {
    u32 flags;
    unsigned int file_version;
    size_t iv_bytes;
    size_t metadata_size;
    size_t extent_size;
    size_t key_size;
    size_t extent_shift;
    unsigned int extent_mask;
    struct ecryptfs_mount_crypt_stat *mount_crypt_stat;
    struct crypto_skcipher *tfm;
    struct crypto_shash *hash_tfm;
    unsigned char cipher[32];
    unsigned char key[64];
    unsigned char root_iv[16];
    struct list_head keysig_list;
    struct mutex keysig_list_mutex;
    struct mutex cs_tfm_mutex;
    struct mutex cs_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ecryptfs_crypt_stat {
    u32 flags;
    unsigned int file_version;
    size_t iv_bytes;
    size_t metadata_size;
    size_t extent_size;
    size_t key_size;
    size_t extent_shift;
    unsigned int extent_mask;
    struct ecryptfs_mount_crypt_stat *mount_crypt_stat;
    struct crypto_skcipher *tfm;
    struct crypto_shash *hash_tfm;
    unsigned char cipher[32];
    unsigned char key[64];
    unsigned char root_iv[16];
    struct list_head keysig_list;
    struct mutex keysig_list_mutex;
    struct mutex cs_tfm_mutex;
    struct mutex cs_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ecryptfs_crypt_stat {
    u32 flags;
    unsigned int file_version;
    size_t iv_bytes;
    size_t metadata_size;
    size_t extent_size;
    size_t key_size;
    size_t extent_shift;
    unsigned int extent_mask;
    struct ecryptfs_mount_crypt_stat *mount_crypt_stat;
    struct crypto_skcipher *tfm;
    struct crypto_shash *hash_tfm;
    unsigned char cipher[32];
    unsigned char key[64];
    unsigned char root_iv[16];
    struct list_head keysig_list;
    struct mutex keysig_list_mutex;
    struct mutex cs_tfm_mutex;
    struct mutex cs_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ecryptfs_crypt_stat {
    u32 flags;
    unsigned int file_version;
    size_t iv_bytes;
    size_t metadata_size;
    size_t extent_size;
    size_t key_size;
    size_t extent_shift;
    unsigned int extent_mask;
    struct ecryptfs_mount_crypt_stat *mount_crypt_stat;
    struct crypto_skcipher *tfm;
    struct crypto_shash *hash_tfm;
    unsigned char cipher[32];
    unsigned char key[64];
    unsigned char root_iv[16];
    struct list_head keysig_list;
    struct mutex keysig_list_mutex;
    struct mutex cs_tfm_mutex;
    struct mutex cs_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ecryptfs_crypt_stat {
    u32 flags;
    unsigned int file_version;
    size_t iv_bytes;
    size_t metadata_size;
    size_t extent_size;
    size_t key_size;
    size_t extent_shift;
    unsigned int extent_mask;
    struct ecryptfs_mount_crypt_stat *mount_crypt_stat;
    struct crypto_skcipher *tfm;
    struct crypto_shash *hash_tfm;
    unsigned char cipher[32];
    unsigned char key[64];
    unsigned char root_iv[16];
    struct list_head keysig_list;
    struct mutex keysig_list_mutex;
    struct mutex cs_tfm_mutex;
    struct mutex cs_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ecryptfs_crypt_stat {
    u32 flags;
    unsigned int file_version;
    size_t iv_bytes;
    size_t metadata_size;
    size_t extent_size;
    size_t key_size;
    size_t extent_shift;
    unsigned int extent_mask;
    struct ecryptfs_mount_crypt_stat *mount_crypt_stat;
    struct crypto_skcipher *tfm;
    struct crypto_shash *hash_tfm;
    unsigned char cipher[32];
    unsigned char key[64];
    unsigned char root_iv[16];
    struct list_head keysig_list;
    struct mutex keysig_list_mutex;
    struct mutex cs_tfm_mutex;
    struct mutex cs_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ecryptfs_crypt_stat {
    u32 flags;
    unsigned int file_version;
    size_t iv_bytes;
    size_t metadata_size;
    size_t extent_size;
    size_t key_size;
    size_t extent_shift;
    unsigned int extent_mask;
    struct ecryptfs_mount_crypt_stat *mount_crypt_stat;
    struct crypto_skcipher *tfm;
    struct crypto_shash *hash_tfm;
    unsigned char cipher[32];
    unsigned char key[64];
    unsigned char root_iv[16];
    struct list_head keysig_list;
    struct mutex keysig_list_mutex;
    struct mutex cs_tfm_mutex;
    struct mutex cs_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ecryptfs_crypt_stat {
    u32 flags;
    unsigned int file_version;
    size_t iv_bytes;
    size_t metadata_size;
    size_t extent_size;
    size_t key_size;
    size_t extent_shift;
    unsigned int extent_mask;
    struct ecryptfs_mount_crypt_stat *mount_crypt_stat;
    struct crypto_skcipher *tfm;
    struct crypto_shash *hash_tfm;
    unsigned char cipher[32];
    unsigned char key[64];
    unsigned char root_iv[16];
    struct list_head keysig_list;
    struct mutex keysig_list_mutex;
    struct mutex cs_tfm_mutex;
    struct mutex cs_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ecryptfs_crypt_stat {
    u32 flags;
    unsigned int file_version;
    size_t iv_bytes;
    size_t metadata_size;
    size_t extent_size;
    size_t key_size;
    size_t extent_shift;
    unsigned int extent_mask;
    struct ecryptfs_mount_crypt_stat *mount_crypt_stat;
    struct crypto_skcipher *tfm;
    struct crypto_shash *hash_tfm;
    unsigned char cipher[32];
    unsigned char key[64];
    unsigned char root_iv[16];
    struct list_head keysig_list;
    struct mutex keysig_list_mutex;
    struct mutex cs_tfm_mutex;
    struct mutex cs_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ecryptfs_crypt_stat {
    u32 flags;
    unsigned int file_version;
    size_t iv_bytes;
    size_t metadata_size;
    size_t extent_size;
    size_t key_size;
    size_t extent_shift;
    unsigned int extent_mask;
    struct ecryptfs_mount_crypt_stat *mount_crypt_stat;
    struct crypto_skcipher *tfm;
    struct crypto_shash *hash_tfm;
    unsigned char cipher[32];
    unsigned char key[64];
    unsigned char root_iv[16];
    struct list_head keysig_list;
    struct mutex keysig_list_mutex;
    struct mutex cs_tfm_mutex;
    struct mutex cs_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ecryptfs_crypt_stat {
    u32 flags;
    unsigned int file_version;
    size_t iv_bytes;
    size_t metadata_size;
    size_t extent_size;
    size_t key_size;
    size_t extent_shift;
    unsigned int extent_mask;
    struct ecryptfs_mount_crypt_stat *mount_crypt_stat;
    struct crypto_skcipher *tfm;
    struct crypto_shash *hash_tfm;
    unsigned char cipher[32];
    unsigned char key[64];
    unsigned char root_iv[16];
    struct list_head keysig_list;
    struct mutex keysig_list_mutex;
    struct mutex cs_tfm_mutex;
    struct mutex cs_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ecryptfs_crypt_stat {
    u32 flags;
    unsigned int file_version;
    size_t iv_bytes;
    size_t metadata_size;
    size_t extent_size;
    size_t key_size;
    size_t extent_shift;
    unsigned int extent_mask;
    struct ecryptfs_mount_crypt_stat *mount_crypt_stat;
    struct crypto_skcipher *tfm;
    struct crypto_shash *hash_tfm;
    unsigned char cipher[32];
    unsigned char key[64];
    unsigned char root_iv[16];
    struct list_head keysig_list;
    struct mutex keysig_list_mutex;
    struct mutex cs_tfm_mutex;
    struct mutex cs_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ecryptfs_crypt_stat {
    u32 flags;
    unsigned int file_version;
    size_t iv_bytes;
    size_t metadata_size;
    size_t extent_size;
    size_t key_size;
    size_t extent_shift;
    unsigned int extent_mask;
    struct ecryptfs_mount_crypt_stat *mount_crypt_stat;
    struct crypto_skcipher *tfm;
    struct crypto_shash *hash_tfm;
    unsigned char cipher[32];
    unsigned char key[64];
    unsigned char root_iv[16];
    struct list_head keysig_list;
    struct mutex keysig_list_mutex;
    struct mutex cs_tfm_mutex;
    struct mutex cs_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ecryptfs_crypt_stat {
    u32 flags;
    unsigned int file_version;
    size_t iv_bytes;
    size_t metadata_size;
    size_t extent_size;
    size_t key_size;
    size_t extent_shift;
    unsigned int extent_mask;
    struct ecryptfs_mount_crypt_stat *mount_crypt_stat;
    struct crypto_skcipher *tfm;
    struct crypto_shash *hash_tfm;
    unsigned char cipher[32];
    unsigned char key[64];
    unsigned char root_iv[16];
    struct list_head keysig_list;
    struct mutex keysig_list_mutex;
    struct mutex cs_tfm_mutex;
    struct mutex cs_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ecryptfs_crypt_stat {
    u32 flags;
    unsigned int file_version;
    size_t iv_bytes;
    size_t metadata_size;
    size_t extent_size;
    size_t key_size;
    size_t extent_shift;
    unsigned int extent_mask;
    struct ecryptfs_mount_crypt_stat *mount_crypt_stat;
    struct crypto_skcipher *tfm;
    struct crypto_shash *hash_tfm;
    unsigned char cipher[32];
    unsigned char key[64];
    unsigned char root_iv[16];
    struct list_head keysig_list;
    struct mutex keysig_list_mutex;
    struct mutex cs_tfm_mutex;
    struct mutex cs_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ecryptfs_crypt_stat {
    u32 flags;
    unsigned int file_version;
    size_t iv_bytes;
    size_t metadata_size;
    size_t extent_size;
    size_t key_size;
    size_t extent_shift;
    unsigned int extent_mask;
    struct ecryptfs_mount_crypt_stat *mount_crypt_stat;
    struct crypto_skcipher *tfm;
    struct crypto_shash *hash_tfm;
    unsigned char cipher[32];
    unsigned char key[64];
    unsigned char root_iv[16];
    struct list_head keysig_list;
    struct mutex keysig_list_mutex;
    struct mutex cs_tfm_mutex;
    struct mutex cs_mutex;
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
struct ecryptfs_crypt_stat {
    u32 flags;
    unsigned int file_version;
    size_t iv_bytes;
    size_t metadata_size;
    size_t extent_size;
    size_t key_size;
    size_t extent_shift;
    unsigned int extent_mask;
    struct ecryptfs_mount_crypt_stat *mount_crypt_stat;
    struct crypto_skcipher *tfm;
    struct crypto_shash *hash_tfm;
    unsigned char cipher[32];
    unsigned char key[64];
    unsigned char root_iv[16];
    struct list_head keysig_list;
    struct mutex keysig_list_mutex;
    struct mutex cs_tfm_mutex;
    struct mutex cs_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ecryptfs_crypt_stat {
    u32 flags;
    unsigned int file_version;
    size_t iv_bytes;
    size_t metadata_size;
    size_t extent_size;
    size_t key_size;
    size_t extent_shift;
    unsigned int extent_mask;
    struct ecryptfs_mount_crypt_stat *mount_crypt_stat;
    struct crypto_skcipher *tfm;
    struct crypto_shash *hash_tfm;
    unsigned char cipher[32];
    unsigned char key[64];
    unsigned char root_iv[16];
    struct list_head keysig_list;
    struct mutex keysig_list_mutex;
    struct mutex cs_tfm_mutex;
    struct mutex cs_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ecryptfs_crypt_stat {
    u32 flags;
    unsigned int file_version;
    size_t iv_bytes;
    size_t metadata_size;
    size_t extent_size;
    size_t key_size;
    size_t extent_shift;
    unsigned int extent_mask;
    struct ecryptfs_mount_crypt_stat *mount_crypt_stat;
    struct crypto_skcipher *tfm;
    struct crypto_shash *hash_tfm;
    unsigned char cipher[32];
    unsigned char key[64];
    unsigned char root_iv[16];
    struct list_head keysig_list;
    struct mutex keysig_list_mutex;
    struct mutex cs_tfm_mutex;
    struct mutex cs_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ecryptfs_crypt_stat {
    u32 flags;
    unsigned int file_version;
    size_t iv_bytes;
    size_t metadata_size;
    size_t extent_size;
    size_t key_size;
    size_t extent_shift;
    unsigned int extent_mask;
    struct ecryptfs_mount_crypt_stat *mount_crypt_stat;
    struct crypto_skcipher *tfm;
    struct crypto_shash *hash_tfm;
    unsigned char cipher[32];
    unsigned char key[64];
    unsigned char root_iv[16];
    struct list_head keysig_list;
    struct mutex keysig_list_mutex;
    struct mutex cs_tfm_mutex;
    struct mutex cs_mutex;
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
struct ecryptfs_crypt_stat {
    u32 flags;
    unsigned int file_version;
    size_t iv_bytes;
    size_t metadata_size;
    size_t extent_size;
    size_t key_size;
    size_t extent_shift;
    unsigned int extent_mask;
    struct ecryptfs_mount_crypt_stat *mount_crypt_stat;
    struct crypto_skcipher *tfm;
    struct crypto_shash *hash_tfm;
    unsigned char cipher[32];
    unsigned char key[64];
    unsigned char root_iv[16];
    struct list_head keysig_list;
    struct mutex keysig_list_mutex;
    struct mutex cs_tfm_mutex;
    struct mutex cs_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ecryptfs_crypt_stat {
    u32 flags;
    unsigned int file_version;
    size_t iv_bytes;
    size_t metadata_size;
    size_t extent_size;
    size_t key_size;
    size_t extent_shift;
    unsigned int extent_mask;
    struct ecryptfs_mount_crypt_stat *mount_crypt_stat;
    struct crypto_skcipher *tfm;
    struct crypto_shash *hash_tfm;
    unsigned char cipher[32];
    unsigned char key[64];
    unsigned char root_iv[16];
    struct list_head keysig_list;
    struct mutex keysig_list_mutex;
    struct mutex cs_tfm_mutex;
    struct mutex cs_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ecryptfs_crypt_stat {
    u32 flags;
    unsigned int file_version;
    size_t iv_bytes;
    size_t metadata_size;
    size_t extent_size;
    size_t key_size;
    size_t extent_shift;
    unsigned int extent_mask;
    struct ecryptfs_mount_crypt_stat *mount_crypt_stat;
    struct crypto_skcipher *tfm;
    struct crypto_shash *hash_tfm;
    unsigned char cipher[32];
    unsigned char key[64];
    unsigned char root_iv[16];
    struct list_head keysig_list;
    struct mutex keysig_list_mutex;
    struct mutex cs_tfm_mutex;
    struct mutex cs_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ecryptfs_crypt_stat {
    u32 flags;
    unsigned int file_version;
    size_t iv_bytes;
    size_t metadata_size;
    size_t extent_size;
    size_t key_size;
    size_t extent_shift;
    unsigned int extent_mask;
    struct ecryptfs_mount_crypt_stat *mount_crypt_stat;
    struct crypto_skcipher *tfm;
    struct crypto_shash *hash_tfm;
    unsigned char cipher[32];
    unsigned char key[64];
    unsigned char root_iv[16];
    struct list_head keysig_list;
    struct mutex keysig_list_mutex;
    struct mutex cs_tfm_mutex;
    struct mutex cs_mutex;
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
<b>Field removed. </b>
<code>struct mutex cs_hash_tfm_mutex</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct crypto_ablkcipher *tfm</code> ➡️ <code>struct crypto_skcipher *tfm</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct crypto_hash *hash_tfm</code> ➡️ <code>struct crypto_shash *hash_tfm</code>
</li>
</ul>
</details>
</li>
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
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
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
No changes between <code>5.11</code> and <code>5.13</code> ✅
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
