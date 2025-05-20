# Struct: <code>ecryptfs_parse_tag_70_packet_silly_stack</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct ecryptfs_parse_tag_70_packet_silly_stack {
    u8 cipher_code;
    size_t max_packet_size;
    size_t packet_size_len;
    size_t parsed_tag_70_packet_size;
    size_t block_aligned_filename_size;
    size_t block_size;
    size_t i;
    struct mutex *tfm_mutex;
    char *decrypted_filename;
    struct ecryptfs_auth_tok *auth_tok;
    struct scatterlist src_sg[2];
    struct scatterlist dst_sg[2];
    struct blkcipher_desc desc;
    char fnek_sig_hex[17];
    char iv[16];
    char cipher_string[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ecryptfs_parse_tag_70_packet_silly_stack {
    u8 cipher_code;
    size_t max_packet_size;
    size_t packet_size_len;
    size_t parsed_tag_70_packet_size;
    size_t block_aligned_filename_size;
    size_t block_size;
    size_t i;
    struct mutex *tfm_mutex;
    char *decrypted_filename;
    struct ecryptfs_auth_tok *auth_tok;
    struct scatterlist src_sg[2];
    struct scatterlist dst_sg[2];
    struct crypto_skcipher *skcipher_tfm;
    struct skcipher_request *skcipher_req;
    char fnek_sig_hex[17];
    char iv[16];
    char cipher_string[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ecryptfs_parse_tag_70_packet_silly_stack {
    u8 cipher_code;
    size_t max_packet_size;
    size_t packet_size_len;
    size_t parsed_tag_70_packet_size;
    size_t block_aligned_filename_size;
    size_t block_size;
    size_t i;
    struct mutex *tfm_mutex;
    char *decrypted_filename;
    struct ecryptfs_auth_tok *auth_tok;
    struct scatterlist src_sg[2];
    struct scatterlist dst_sg[2];
    struct crypto_skcipher *skcipher_tfm;
    struct skcipher_request *skcipher_req;
    char fnek_sig_hex[17];
    char iv[16];
    char cipher_string[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ecryptfs_parse_tag_70_packet_silly_stack {
    u8 cipher_code;
    size_t max_packet_size;
    size_t packet_size_len;
    size_t parsed_tag_70_packet_size;
    size_t block_aligned_filename_size;
    size_t block_size;
    size_t i;
    struct mutex *tfm_mutex;
    char *decrypted_filename;
    struct ecryptfs_auth_tok *auth_tok;
    struct scatterlist src_sg[2];
    struct scatterlist dst_sg[2];
    struct crypto_skcipher *skcipher_tfm;
    struct skcipher_request *skcipher_req;
    char fnek_sig_hex[17];
    char iv[16];
    char cipher_string[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ecryptfs_parse_tag_70_packet_silly_stack {
    u8 cipher_code;
    size_t max_packet_size;
    size_t packet_size_len;
    size_t parsed_tag_70_packet_size;
    size_t block_aligned_filename_size;
    size_t block_size;
    size_t i;
    struct mutex *tfm_mutex;
    char *decrypted_filename;
    struct ecryptfs_auth_tok *auth_tok;
    struct scatterlist src_sg[2];
    struct scatterlist dst_sg[2];
    struct crypto_skcipher *skcipher_tfm;
    struct skcipher_request *skcipher_req;
    char fnek_sig_hex[17];
    char iv[16];
    char cipher_string[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ecryptfs_parse_tag_70_packet_silly_stack {
    u8 cipher_code;
    size_t max_packet_size;
    size_t packet_size_len;
    size_t parsed_tag_70_packet_size;
    size_t block_aligned_filename_size;
    size_t block_size;
    size_t i;
    struct mutex *tfm_mutex;
    char *decrypted_filename;
    struct ecryptfs_auth_tok *auth_tok;
    struct scatterlist src_sg[2];
    struct scatterlist dst_sg[2];
    struct crypto_skcipher *skcipher_tfm;
    struct skcipher_request *skcipher_req;
    char fnek_sig_hex[17];
    char iv[16];
    char cipher_string[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ecryptfs_parse_tag_70_packet_silly_stack {
    u8 cipher_code;
    size_t max_packet_size;
    size_t packet_size_len;
    size_t parsed_tag_70_packet_size;
    size_t block_aligned_filename_size;
    size_t block_size;
    size_t i;
    struct mutex *tfm_mutex;
    char *decrypted_filename;
    struct ecryptfs_auth_tok *auth_tok;
    struct scatterlist src_sg[2];
    struct scatterlist dst_sg[2];
    struct crypto_skcipher *skcipher_tfm;
    struct skcipher_request *skcipher_req;
    char fnek_sig_hex[17];
    char iv[16];
    char cipher_string[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ecryptfs_parse_tag_70_packet_silly_stack {
    u8 cipher_code;
    size_t max_packet_size;
    size_t packet_size_len;
    size_t parsed_tag_70_packet_size;
    size_t block_aligned_filename_size;
    size_t block_size;
    size_t i;
    struct mutex *tfm_mutex;
    char *decrypted_filename;
    struct ecryptfs_auth_tok *auth_tok;
    struct scatterlist src_sg[2];
    struct scatterlist dst_sg[2];
    struct crypto_skcipher *skcipher_tfm;
    struct skcipher_request *skcipher_req;
    char fnek_sig_hex[17];
    char iv[16];
    char cipher_string[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ecryptfs_parse_tag_70_packet_silly_stack {
    u8 cipher_code;
    size_t max_packet_size;
    size_t packet_size_len;
    size_t parsed_tag_70_packet_size;
    size_t block_aligned_filename_size;
    size_t block_size;
    size_t i;
    struct mutex *tfm_mutex;
    char *decrypted_filename;
    struct ecryptfs_auth_tok *auth_tok;
    struct scatterlist src_sg[2];
    struct scatterlist dst_sg[2];
    struct crypto_skcipher *skcipher_tfm;
    struct skcipher_request *skcipher_req;
    char fnek_sig_hex[17];
    char iv[16];
    char cipher_string[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ecryptfs_parse_tag_70_packet_silly_stack {
    u8 cipher_code;
    size_t max_packet_size;
    size_t packet_size_len;
    size_t parsed_tag_70_packet_size;
    size_t block_aligned_filename_size;
    size_t block_size;
    size_t i;
    struct mutex *tfm_mutex;
    char *decrypted_filename;
    struct ecryptfs_auth_tok *auth_tok;
    struct scatterlist src_sg[2];
    struct scatterlist dst_sg[2];
    struct crypto_skcipher *skcipher_tfm;
    struct skcipher_request *skcipher_req;
    char fnek_sig_hex[17];
    char iv[16];
    char cipher_string[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ecryptfs_parse_tag_70_packet_silly_stack {
    u8 cipher_code;
    size_t max_packet_size;
    size_t packet_size_len;
    size_t parsed_tag_70_packet_size;
    size_t block_aligned_filename_size;
    size_t block_size;
    size_t i;
    struct mutex *tfm_mutex;
    char *decrypted_filename;
    struct ecryptfs_auth_tok *auth_tok;
    struct scatterlist src_sg[2];
    struct scatterlist dst_sg[2];
    struct crypto_skcipher *skcipher_tfm;
    struct skcipher_request *skcipher_req;
    char fnek_sig_hex[17];
    char iv[16];
    char cipher_string[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ecryptfs_parse_tag_70_packet_silly_stack {
    u8 cipher_code;
    size_t max_packet_size;
    size_t packet_size_len;
    size_t parsed_tag_70_packet_size;
    size_t block_aligned_filename_size;
    size_t block_size;
    size_t i;
    struct mutex *tfm_mutex;
    char *decrypted_filename;
    struct ecryptfs_auth_tok *auth_tok;
    struct scatterlist src_sg[2];
    struct scatterlist dst_sg[2];
    struct crypto_skcipher *skcipher_tfm;
    struct skcipher_request *skcipher_req;
    char fnek_sig_hex[17];
    char iv[16];
    char cipher_string[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ecryptfs_parse_tag_70_packet_silly_stack {
    u8 cipher_code;
    size_t max_packet_size;
    size_t packet_size_len;
    size_t parsed_tag_70_packet_size;
    size_t block_aligned_filename_size;
    size_t block_size;
    size_t i;
    struct mutex *tfm_mutex;
    char *decrypted_filename;
    struct ecryptfs_auth_tok *auth_tok;
    struct scatterlist src_sg[2];
    struct scatterlist dst_sg[2];
    struct crypto_skcipher *skcipher_tfm;
    struct skcipher_request *skcipher_req;
    char fnek_sig_hex[17];
    char iv[16];
    char cipher_string[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ecryptfs_parse_tag_70_packet_silly_stack {
    u8 cipher_code;
    size_t max_packet_size;
    size_t packet_size_len;
    size_t parsed_tag_70_packet_size;
    size_t block_aligned_filename_size;
    size_t block_size;
    size_t i;
    struct mutex *tfm_mutex;
    char *decrypted_filename;
    struct ecryptfs_auth_tok *auth_tok;
    struct scatterlist src_sg[2];
    struct scatterlist dst_sg[2];
    struct crypto_skcipher *skcipher_tfm;
    struct skcipher_request *skcipher_req;
    char fnek_sig_hex[17];
    char iv[16];
    char cipher_string[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ecryptfs_parse_tag_70_packet_silly_stack {
    u8 cipher_code;
    size_t max_packet_size;
    size_t packet_size_len;
    size_t parsed_tag_70_packet_size;
    size_t block_aligned_filename_size;
    size_t block_size;
    size_t i;
    struct mutex *tfm_mutex;
    char *decrypted_filename;
    struct ecryptfs_auth_tok *auth_tok;
    struct scatterlist src_sg[2];
    struct scatterlist dst_sg[2];
    struct crypto_skcipher *skcipher_tfm;
    struct skcipher_request *skcipher_req;
    char fnek_sig_hex[17];
    char iv[16];
    char cipher_string[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ecryptfs_parse_tag_70_packet_silly_stack {
    u8 cipher_code;
    size_t max_packet_size;
    size_t packet_size_len;
    size_t parsed_tag_70_packet_size;
    size_t block_aligned_filename_size;
    size_t block_size;
    size_t i;
    struct mutex *tfm_mutex;
    char *decrypted_filename;
    struct ecryptfs_auth_tok *auth_tok;
    struct scatterlist src_sg[2];
    struct scatterlist dst_sg[2];
    struct crypto_skcipher *skcipher_tfm;
    struct skcipher_request *skcipher_req;
    char fnek_sig_hex[17];
    char iv[16];
    char cipher_string[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ecryptfs_parse_tag_70_packet_silly_stack {
    u8 cipher_code;
    size_t max_packet_size;
    size_t packet_size_len;
    size_t parsed_tag_70_packet_size;
    size_t block_aligned_filename_size;
    size_t block_size;
    size_t i;
    struct mutex *tfm_mutex;
    char *decrypted_filename;
    struct ecryptfs_auth_tok *auth_tok;
    struct scatterlist src_sg[2];
    struct scatterlist dst_sg[2];
    struct crypto_skcipher *skcipher_tfm;
    struct skcipher_request *skcipher_req;
    char fnek_sig_hex[17];
    char iv[16];
    char cipher_string[32];
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
struct ecryptfs_parse_tag_70_packet_silly_stack {
    u8 cipher_code;
    size_t max_packet_size;
    size_t packet_size_len;
    size_t parsed_tag_70_packet_size;
    size_t block_aligned_filename_size;
    size_t block_size;
    size_t i;
    struct mutex *tfm_mutex;
    char *decrypted_filename;
    struct ecryptfs_auth_tok *auth_tok;
    struct scatterlist src_sg[2];
    struct scatterlist dst_sg[2];
    struct crypto_skcipher *skcipher_tfm;
    struct skcipher_request *skcipher_req;
    char fnek_sig_hex[17];
    char iv[16];
    char cipher_string[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ecryptfs_parse_tag_70_packet_silly_stack {
    u8 cipher_code;
    size_t max_packet_size;
    size_t packet_size_len;
    size_t parsed_tag_70_packet_size;
    size_t block_aligned_filename_size;
    size_t block_size;
    size_t i;
    struct mutex *tfm_mutex;
    char *decrypted_filename;
    struct ecryptfs_auth_tok *auth_tok;
    struct scatterlist src_sg[2];
    struct scatterlist dst_sg[2];
    struct crypto_skcipher *skcipher_tfm;
    struct skcipher_request *skcipher_req;
    char fnek_sig_hex[17];
    char iv[16];
    char cipher_string[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ecryptfs_parse_tag_70_packet_silly_stack {
    u8 cipher_code;
    size_t max_packet_size;
    size_t packet_size_len;
    size_t parsed_tag_70_packet_size;
    size_t block_aligned_filename_size;
    size_t block_size;
    size_t i;
    struct mutex *tfm_mutex;
    char *decrypted_filename;
    struct ecryptfs_auth_tok *auth_tok;
    struct scatterlist src_sg[2];
    struct scatterlist dst_sg[2];
    struct crypto_skcipher *skcipher_tfm;
    struct skcipher_request *skcipher_req;
    char fnek_sig_hex[17];
    char iv[16];
    char cipher_string[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ecryptfs_parse_tag_70_packet_silly_stack {
    u8 cipher_code;
    size_t max_packet_size;
    size_t packet_size_len;
    size_t parsed_tag_70_packet_size;
    size_t block_aligned_filename_size;
    size_t block_size;
    size_t i;
    struct mutex *tfm_mutex;
    char *decrypted_filename;
    struct ecryptfs_auth_tok *auth_tok;
    struct scatterlist src_sg[2];
    struct scatterlist dst_sg[2];
    struct crypto_skcipher *skcipher_tfm;
    struct skcipher_request *skcipher_req;
    char fnek_sig_hex[17];
    char iv[16];
    char cipher_string[32];
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
struct ecryptfs_parse_tag_70_packet_silly_stack {
    u8 cipher_code;
    size_t max_packet_size;
    size_t packet_size_len;
    size_t parsed_tag_70_packet_size;
    size_t block_aligned_filename_size;
    size_t block_size;
    size_t i;
    struct mutex *tfm_mutex;
    char *decrypted_filename;
    struct ecryptfs_auth_tok *auth_tok;
    struct scatterlist src_sg[2];
    struct scatterlist dst_sg[2];
    struct crypto_skcipher *skcipher_tfm;
    struct skcipher_request *skcipher_req;
    char fnek_sig_hex[17];
    char iv[16];
    char cipher_string[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ecryptfs_parse_tag_70_packet_silly_stack {
    u8 cipher_code;
    size_t max_packet_size;
    size_t packet_size_len;
    size_t parsed_tag_70_packet_size;
    size_t block_aligned_filename_size;
    size_t block_size;
    size_t i;
    struct mutex *tfm_mutex;
    char *decrypted_filename;
    struct ecryptfs_auth_tok *auth_tok;
    struct scatterlist src_sg[2];
    struct scatterlist dst_sg[2];
    struct crypto_skcipher *skcipher_tfm;
    struct skcipher_request *skcipher_req;
    char fnek_sig_hex[17];
    char iv[16];
    char cipher_string[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ecryptfs_parse_tag_70_packet_silly_stack {
    u8 cipher_code;
    size_t max_packet_size;
    size_t packet_size_len;
    size_t parsed_tag_70_packet_size;
    size_t block_aligned_filename_size;
    size_t block_size;
    size_t i;
    struct mutex *tfm_mutex;
    char *decrypted_filename;
    struct ecryptfs_auth_tok *auth_tok;
    struct scatterlist src_sg[2];
    struct scatterlist dst_sg[2];
    struct crypto_skcipher *skcipher_tfm;
    struct skcipher_request *skcipher_req;
    char fnek_sig_hex[17];
    char iv[16];
    char cipher_string[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ecryptfs_parse_tag_70_packet_silly_stack {
    u8 cipher_code;
    size_t max_packet_size;
    size_t packet_size_len;
    size_t parsed_tag_70_packet_size;
    size_t block_aligned_filename_size;
    size_t block_size;
    size_t i;
    struct mutex *tfm_mutex;
    char *decrypted_filename;
    struct ecryptfs_auth_tok *auth_tok;
    struct scatterlist src_sg[2];
    struct scatterlist dst_sg[2];
    struct crypto_skcipher *skcipher_tfm;
    struct skcipher_request *skcipher_req;
    char fnek_sig_hex[17];
    char iv[16];
    char cipher_string[32];
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
<code>struct crypto_skcipher *skcipher_tfm</code>
</li>
<li>
<b>Field added. </b>
<code>struct skcipher_request *skcipher_req</code>
</li>
<li>
<b>Field removed. </b>
<code>struct blkcipher_desc desc</code>
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
