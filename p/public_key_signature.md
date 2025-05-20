# Struct: <code>public_key_signature</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct public_key_signature {
    u8 *digest;
    u8 digest_size;
    u8 nr_mpi;
    enum pkey_algo pkey_algo;
    enum hash_algo pkey_hash_algo;
    MPI mpi[2];
    struct (anon) rsa;
    struct (anon) dsa;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct public_key_signature {
    struct asymmetric_key_id * auth_ids[2];
    u8 *s;
    u32 s_size;
    u8 *digest;
    u8 digest_size;
    const char *pkey_algo;
    const char *hash_algo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct public_key_signature {
    struct asymmetric_key_id * auth_ids[2];
    u8 *s;
    u32 s_size;
    u8 *digest;
    u8 digest_size;
    const char *pkey_algo;
    const char *hash_algo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct public_key_signature {
    struct asymmetric_key_id * auth_ids[2];
    u8 *s;
    u32 s_size;
    u8 *digest;
    u8 digest_size;
    const char *pkey_algo;
    const char *hash_algo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct public_key_signature {
    struct asymmetric_key_id * auth_ids[2];
    u8 *s;
    u32 s_size;
    u8 *digest;
    u8 digest_size;
    const char *pkey_algo;
    const char *hash_algo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct public_key_signature {
    struct asymmetric_key_id * auth_ids[2];
    u8 *s;
    u32 s_size;
    u8 *digest;
    u8 digest_size;
    const char *pkey_algo;
    const char *hash_algo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct public_key_signature {
    struct asymmetric_key_id * auth_ids[2];
    u8 *s;
    u32 s_size;
    u8 *digest;
    u8 digest_size;
    const char *pkey_algo;
    const char *hash_algo;
    const char *encoding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct public_key_signature {
    struct asymmetric_key_id * auth_ids[2];
    u8 *s;
    u32 s_size;
    u8 *digest;
    u8 digest_size;
    const char *pkey_algo;
    const char *hash_algo;
    const char *encoding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct public_key_signature {
    struct asymmetric_key_id * auth_ids[2];
    u8 *s;
    u32 s_size;
    u8 *digest;
    u8 digest_size;
    const char *pkey_algo;
    const char *hash_algo;
    const char *encoding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct public_key_signature {
    struct asymmetric_key_id * auth_ids[2];
    u8 *s;
    u32 s_size;
    u8 *digest;
    u8 digest_size;
    const char *pkey_algo;
    const char *hash_algo;
    const char *encoding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct public_key_signature {
    struct asymmetric_key_id * auth_ids[2];
    u8 *s;
    u32 s_size;
    u8 *digest;
    u8 digest_size;
    const char *pkey_algo;
    const char *hash_algo;
    const char *encoding;
    const void *data;
    unsigned int data_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct public_key_signature {
    struct asymmetric_key_id * auth_ids[2];
    u8 *s;
    u32 s_size;
    u8 *digest;
    u8 digest_size;
    const char *pkey_algo;
    const char *hash_algo;
    const char *encoding;
    const void *data;
    unsigned int data_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct public_key_signature {
    struct asymmetric_key_id * auth_ids[2];
    u8 *s;
    u8 *digest;
    u32 s_size;
    u32 digest_size;
    const char *pkey_algo;
    const char *hash_algo;
    const char *encoding;
    const void *data;
    unsigned int data_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct public_key_signature {
    struct asymmetric_key_id * auth_ids[3];
    u8 *s;
    u8 *digest;
    u32 s_size;
    u32 digest_size;
    const char *pkey_algo;
    const char *hash_algo;
    const char *encoding;
    const void *data;
    unsigned int data_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct public_key_signature {
    struct asymmetric_key_id * auth_ids[3];
    u8 *s;
    u8 *digest;
    u32 s_size;
    u32 digest_size;
    const char *pkey_algo;
    const char *hash_algo;
    const char *encoding;
    const void *data;
    unsigned int data_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct public_key_signature {
    struct asymmetric_key_id * auth_ids[3];
    u8 *s;
    u8 *digest;
    u32 s_size;
    u32 digest_size;
    const char *pkey_algo;
    const char *hash_algo;
    const char *encoding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct public_key_signature {
    struct asymmetric_key_id * auth_ids[3];
    u8 *s;
    u8 *digest;
    u32 s_size;
    u32 digest_size;
    const char *pkey_algo;
    const char *hash_algo;
    const char *encoding;
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
struct public_key_signature {
    struct asymmetric_key_id * auth_ids[2];
    u8 *s;
    u32 s_size;
    u8 *digest;
    u8 digest_size;
    const char *pkey_algo;
    const char *hash_algo;
    const char *encoding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct public_key_signature {
    struct asymmetric_key_id * auth_ids[2];
    u8 *s;
    u32 s_size;
    u8 *digest;
    u8 digest_size;
    const char *pkey_algo;
    const char *hash_algo;
    const char *encoding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct public_key_signature {
    struct asymmetric_key_id * auth_ids[2];
    u8 *s;
    u32 s_size;
    u8 *digest;
    u8 digest_size;
    const char *pkey_algo;
    const char *hash_algo;
    const char *encoding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct public_key_signature {
    struct asymmetric_key_id * auth_ids[2];
    u8 *s;
    u32 s_size;
    u8 *digest;
    u8 digest_size;
    const char *pkey_algo;
    const char *hash_algo;
    const char *encoding;
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
struct public_key_signature {
    struct asymmetric_key_id * auth_ids[2];
    u8 *s;
    u32 s_size;
    u8 *digest;
    u8 digest_size;
    const char *pkey_algo;
    const char *hash_algo;
    const char *encoding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct public_key_signature {
    struct asymmetric_key_id * auth_ids[2];
    u8 *s;
    u32 s_size;
    u8 *digest;
    u8 digest_size;
    const char *pkey_algo;
    const char *hash_algo;
    const char *encoding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct public_key_signature {
    struct asymmetric_key_id * auth_ids[2];
    u8 *s;
    u32 s_size;
    u8 *digest;
    u8 digest_size;
    const char *pkey_algo;
    const char *hash_algo;
    const char *encoding;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct public_key_signature {
    struct asymmetric_key_id * auth_ids[2];
    u8 *s;
    u32 s_size;
    u8 *digest;
    u8 digest_size;
    const char *pkey_algo;
    const char *hash_algo;
    const char *encoding;
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
<code>struct asymmetric_key_id * auth_ids[2]</code>
</li>
<li>
<b>Field added. </b>
<code>u8 *s</code>
</li>
<li>
<b>Field added. </b>
<code>u32 s_size</code>
</li>
<li>
<b>Field added. </b>
<code>const char *hash_algo</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 nr_mpi</code>
</li>
<li>
<b>Field removed. </b>
<code>enum hash_algo pkey_hash_algo</code>
</li>
<li>
<b>Field removed. </b>
<code>MPI mpi[2]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct (anon) rsa</code>
</li>
<li>
<b>Field removed. </b>
<code>struct (anon) dsa</code>
</li>
<li>
<b>Field type changed. </b>
<code>enum pkey_algo pkey_algo</code> ➡️ <code>const char *pkey_algo</code>
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
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const char *encoding</code>
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
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const void *data</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int data_size</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>u8 digest_size</code> ➡️ <code>u32 digest_size</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct asymmetric_key_id * auth_ids[2]</code> ➡️ <code>struct asymmetric_key_id * auth_ids[3]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>const void *data</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int data_size</code>
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
