# Struct: <code>tls_rec</code>

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
struct tls_rec {
    struct list_head list;
    int tx_ready;
    int tx_flags;
    int inplace_crypto;
    struct sk_msg msg_plaintext;
    struct sk_msg msg_encrypted;
    struct scatterlist sg_aead_in[2];
    struct scatterlist sg_aead_out[2];
    char aad_space[13];
    u8 iv_data[12];
    struct aead_request aead_req;
    u8 aead_req_ctx[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct tls_rec {
    struct list_head list;
    int tx_ready;
    int tx_flags;
    int inplace_crypto;
    struct sk_msg msg_plaintext;
    struct sk_msg msg_encrypted;
    struct scatterlist sg_aead_in[2];
    struct scatterlist sg_aead_out[2];
    char content_type;
    struct scatterlist sg_content_type;
    char aad_space[13];
    u8 iv_data[16];
    struct aead_request aead_req;
    u8 aead_req_ctx[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct tls_rec {
    struct list_head list;
    int tx_ready;
    int tx_flags;
    struct sk_msg msg_plaintext;
    struct sk_msg msg_encrypted;
    struct scatterlist sg_aead_in[2];
    struct scatterlist sg_aead_out[2];
    char content_type;
    struct scatterlist sg_content_type;
    char aad_space[13];
    u8 iv_data[16];
    struct aead_request aead_req;
    u8 aead_req_ctx[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct tls_rec {
    struct list_head list;
    int tx_ready;
    int tx_flags;
    struct sk_msg msg_plaintext;
    struct sk_msg msg_encrypted;
    struct scatterlist sg_aead_in[2];
    struct scatterlist sg_aead_out[2];
    char content_type;
    struct scatterlist sg_content_type;
    char aad_space[13];
    u8 iv_data[16];
    struct aead_request aead_req;
    u8 aead_req_ctx[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct tls_rec {
    struct list_head list;
    int tx_ready;
    int tx_flags;
    struct sk_msg msg_plaintext;
    struct sk_msg msg_encrypted;
    struct scatterlist sg_aead_in[2];
    struct scatterlist sg_aead_out[2];
    char content_type;
    struct scatterlist sg_content_type;
    char aad_space[13];
    u8 iv_data[16];
    struct aead_request aead_req;
    u8 aead_req_ctx[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct tls_rec {
    struct list_head list;
    int tx_ready;
    int tx_flags;
    struct sk_msg msg_plaintext;
    struct sk_msg msg_encrypted;
    struct scatterlist sg_aead_in[2];
    struct scatterlist sg_aead_out[2];
    char content_type;
    struct scatterlist sg_content_type;
    char aad_space[13];
    u8 iv_data[16];
    struct aead_request aead_req;
    u8 aead_req_ctx[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct tls_rec {
    struct list_head list;
    int tx_ready;
    int tx_flags;
    struct sk_msg msg_plaintext;
    struct sk_msg msg_encrypted;
    struct scatterlist sg_aead_in[2];
    struct scatterlist sg_aead_out[2];
    char content_type;
    struct scatterlist sg_content_type;
    char aad_space[13];
    u8 iv_data[16];
    struct aead_request aead_req;
    u8 aead_req_ctx[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct tls_rec {
    struct list_head list;
    int tx_ready;
    int tx_flags;
    struct sk_msg msg_plaintext;
    struct sk_msg msg_encrypted;
    struct scatterlist sg_aead_in[2];
    struct scatterlist sg_aead_out[2];
    char content_type;
    struct scatterlist sg_content_type;
    char aad_space[13];
    u8 iv_data[16];
    struct aead_request aead_req;
    u8 aead_req_ctx[0];
};
```
</details>
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
In <code>6.5</code>: Absent ⚠️
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
struct tls_rec {
    struct list_head list;
    int tx_ready;
    int tx_flags;
    struct sk_msg msg_plaintext;
    struct sk_msg msg_encrypted;
    struct scatterlist sg_aead_in[2];
    struct scatterlist sg_aead_out[2];
    char content_type;
    struct scatterlist sg_content_type;
    char aad_space[13];
    u8 iv_data[16];
    struct aead_request aead_req;
    u8 aead_req_ctx[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct tls_rec {
    struct list_head list;
    int tx_ready;
    int tx_flags;
    struct sk_msg msg_plaintext;
    struct sk_msg msg_encrypted;
    struct scatterlist sg_aead_in[2];
    struct scatterlist sg_aead_out[2];
    char content_type;
    struct scatterlist sg_content_type;
    char aad_space[13];
    u8 iv_data[16];
    struct aead_request aead_req;
    u8 aead_req_ctx[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct tls_rec {
    struct list_head list;
    int tx_ready;
    int tx_flags;
    struct sk_msg msg_plaintext;
    struct sk_msg msg_encrypted;
    struct scatterlist sg_aead_in[2];
    struct scatterlist sg_aead_out[2];
    char content_type;
    struct scatterlist sg_content_type;
    char aad_space[13];
    u8 iv_data[16];
    struct aead_request aead_req;
    u8 aead_req_ctx[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct tls_rec {
    struct list_head list;
    int tx_ready;
    int tx_flags;
    struct sk_msg msg_plaintext;
    struct sk_msg msg_encrypted;
    struct scatterlist sg_aead_in[2];
    struct scatterlist sg_aead_out[2];
    char content_type;
    struct scatterlist sg_content_type;
    char aad_space[13];
    u8 iv_data[16];
    struct aead_request aead_req;
    u8 aead_req_ctx[0];
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
struct tls_rec {
    struct list_head list;
    int tx_ready;
    int tx_flags;
    struct sk_msg msg_plaintext;
    struct sk_msg msg_encrypted;
    struct scatterlist sg_aead_in[2];
    struct scatterlist sg_aead_out[2];
    char content_type;
    struct scatterlist sg_content_type;
    char aad_space[13];
    u8 iv_data[16];
    struct aead_request aead_req;
    u8 aead_req_ctx[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct tls_rec {
    struct list_head list;
    int tx_ready;
    int tx_flags;
    struct sk_msg msg_plaintext;
    struct sk_msg msg_encrypted;
    struct scatterlist sg_aead_in[2];
    struct scatterlist sg_aead_out[2];
    char content_type;
    struct scatterlist sg_content_type;
    char aad_space[13];
    u8 iv_data[16];
    struct aead_request aead_req;
    u8 aead_req_ctx[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct tls_rec {
    struct list_head list;
    int tx_ready;
    int tx_flags;
    struct sk_msg msg_plaintext;
    struct sk_msg msg_encrypted;
    struct scatterlist sg_aead_in[2];
    struct scatterlist sg_aead_out[2];
    char content_type;
    struct scatterlist sg_content_type;
    char aad_space[13];
    u8 iv_data[16];
    struct aead_request aead_req;
    u8 aead_req_ctx[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct tls_rec {
    struct list_head list;
    int tx_ready;
    int tx_flags;
    struct sk_msg msg_plaintext;
    struct sk_msg msg_encrypted;
    struct scatterlist sg_aead_in[2];
    struct scatterlist sg_aead_out[2];
    char content_type;
    struct scatterlist sg_content_type;
    char aad_space[13];
    u8 iv_data[16];
    struct aead_request aead_req;
    u8 aead_req_ctx[0];
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
<code>char content_type</code>
</li>
<li>
<b>Field added. </b>
<code>struct scatterlist sg_content_type</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 iv_data[12]</code> ➡️ <code>u8 iv_data[16]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int inplace_crypto</code>
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
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
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
