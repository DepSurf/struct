# Struct: <code>sctp_endpoint</code>

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
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct sctp_endpoint {
    struct sctp_ep_common base;
    struct list_head asocs;
    __u8 secret_key[32];
    __u8 *digest;
    __u32 sndbuf_policy;
    __u32 rcvbuf_policy;
    struct crypto_shash **auth_hmacs;
    struct sctp_hmac_algo_param *auth_hmacs_list;
    struct sctp_chunks_param *auth_chunk_list;
    struct list_head endpoint_shared_keys;
    __u16 active_key_id;
    __u8 auth_enable;
    __u8 prsctp_enable;
    __u8 reconf_enable;
    __u8 strreset_enable;
    u32 secid;
    u32 peer_secid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct sctp_endpoint {
    struct sctp_ep_common base;
    struct list_head asocs;
    __u8 secret_key[32];
    __u8 *digest;
    __u32 sndbuf_policy;
    __u32 rcvbuf_policy;
    struct crypto_shash **auth_hmacs;
    struct sctp_hmac_algo_param *auth_hmacs_list;
    struct sctp_chunks_param *auth_chunk_list;
    struct list_head endpoint_shared_keys;
    __u16 active_key_id;
    __u8 auth_enable;
    __u8 prsctp_enable;
    __u8 reconf_enable;
    __u8 strreset_enable;
    u32 secid;
    u32 peer_secid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct sctp_endpoint {
    struct sctp_ep_common base;
    struct list_head asocs;
    __u8 secret_key[32];
    __u8 *digest;
    __u32 sndbuf_policy;
    __u32 rcvbuf_policy;
    struct crypto_shash **auth_hmacs;
    struct sctp_hmac_algo_param *auth_hmacs_list;
    struct sctp_chunks_param *auth_chunk_list;
    struct list_head endpoint_shared_keys;
    __u16 active_key_id;
    __u8 auth_enable;
    __u8 intl_enable;
    __u8 prsctp_enable;
    __u8 reconf_enable;
    __u8 strreset_enable;
    u32 secid;
    u32 peer_secid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct sctp_endpoint {
    struct sctp_ep_common base;
    struct list_head asocs;
    __u8 secret_key[32];
    __u8 *digest;
    __u32 sndbuf_policy;
    __u32 rcvbuf_policy;
    struct crypto_shash **auth_hmacs;
    struct sctp_hmac_algo_param *auth_hmacs_list;
    struct sctp_chunks_param *auth_chunk_list;
    struct list_head endpoint_shared_keys;
    __u16 active_key_id;
    __u8 ecn_enable;
    __u8 auth_enable;
    __u8 intl_enable;
    __u8 prsctp_enable;
    __u8 asconf_enable;
    __u8 reconf_enable;
    __u8 strreset_enable;
    u32 secid;
    u32 peer_secid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct sctp_endpoint {
    struct sctp_ep_common base;
    struct list_head asocs;
    __u8 secret_key[32];
    __u8 *digest;
    __u32 sndbuf_policy;
    __u32 rcvbuf_policy;
    struct crypto_shash **auth_hmacs;
    struct sctp_hmac_algo_param *auth_hmacs_list;
    struct sctp_chunks_param *auth_chunk_list;
    struct list_head endpoint_shared_keys;
    __u16 active_key_id;
    __u8 ecn_enable;
    __u8 auth_enable;
    __u8 intl_enable;
    __u8 prsctp_enable;
    __u8 asconf_enable;
    __u8 reconf_enable;
    __u8 strreset_enable;
    u32 secid;
    u32 peer_secid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct sctp_endpoint {
    struct sctp_ep_common base;
    struct list_head asocs;
    __u8 secret_key[32];
    __u8 *digest;
    __u32 sndbuf_policy;
    __u32 rcvbuf_policy;
    struct crypto_shash **auth_hmacs;
    struct sctp_hmac_algo_param *auth_hmacs_list;
    struct sctp_chunks_param *auth_chunk_list;
    struct list_head endpoint_shared_keys;
    __u16 active_key_id;
    __u8 ecn_enable;
    __u8 auth_enable;
    __u8 intl_enable;
    __u8 prsctp_enable;
    __u8 asconf_enable;
    __u8 reconf_enable;
    __u8 strreset_enable;
    u32 secid;
    u32 peer_secid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct sctp_endpoint {
    struct sctp_ep_common base;
    struct list_head asocs;
    __u8 secret_key[32];
    __u8 *digest;
    __u32 sndbuf_policy;
    __u32 rcvbuf_policy;
    struct crypto_shash **auth_hmacs;
    struct sctp_hmac_algo_param *auth_hmacs_list;
    struct sctp_chunks_param *auth_chunk_list;
    struct list_head endpoint_shared_keys;
    __u16 active_key_id;
    __u8 ecn_enable;
    __u8 auth_enable;
    __u8 intl_enable;
    __u8 prsctp_enable;
    __u8 asconf_enable;
    __u8 reconf_enable;
    __u8 strreset_enable;
    u32 secid;
    u32 peer_secid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct sctp_endpoint {
    struct sctp_ep_common base;
    struct list_head asocs;
    __u8 secret_key[32];
    __u8 *digest;
    __u32 sndbuf_policy;
    __u32 rcvbuf_policy;
    struct crypto_shash **auth_hmacs;
    struct sctp_hmac_algo_param *auth_hmacs_list;
    struct sctp_chunks_param *auth_chunk_list;
    struct list_head endpoint_shared_keys;
    __u16 active_key_id;
    __u8 ecn_enable;
    __u8 auth_enable;
    __u8 intl_enable;
    __u8 prsctp_enable;
    __u8 asconf_enable;
    __u8 reconf_enable;
    __u8 strreset_enable;
    u32 secid;
    u32 peer_secid;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct sctp_endpoint {
    struct sctp_ep_common base;
    struct hlist_node node;
    int hashent;
    struct list_head asocs;
    __u8 secret_key[32];
    __u8 *digest;
    __u32 sndbuf_policy;
    __u32 rcvbuf_policy;
    struct crypto_shash **auth_hmacs;
    struct sctp_hmac_algo_param *auth_hmacs_list;
    struct sctp_chunks_param *auth_chunk_list;
    struct list_head endpoint_shared_keys;
    __u16 active_key_id;
    __u8 ecn_enable;
    __u8 auth_enable;
    __u8 intl_enable;
    __u8 prsctp_enable;
    __u8 asconf_enable;
    __u8 reconf_enable;
    __u8 strreset_enable;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct sctp_endpoint {
    struct sctp_ep_common base;
    struct hlist_node node;
    int hashent;
    struct list_head asocs;
    __u8 secret_key[32];
    __u8 *digest;
    __u32 sndbuf_policy;
    __u32 rcvbuf_policy;
    struct crypto_shash **auth_hmacs;
    struct sctp_hmac_algo_param *auth_hmacs_list;
    struct sctp_chunks_param *auth_chunk_list;
    struct list_head endpoint_shared_keys;
    __u16 active_key_id;
    __u8 ecn_enable;
    __u8 auth_enable;
    __u8 intl_enable;
    __u8 prsctp_enable;
    __u8 asconf_enable;
    __u8 reconf_enable;
    __u8 strreset_enable;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct sctp_endpoint {
    struct sctp_ep_common base;
    struct hlist_node node;
    int hashent;
    struct list_head asocs;
    __u8 secret_key[32];
    __u8 *digest;
    __u32 sndbuf_policy;
    __u32 rcvbuf_policy;
    struct crypto_shash **auth_hmacs;
    struct sctp_hmac_algo_param *auth_hmacs_list;
    struct sctp_chunks_param *auth_chunk_list;
    struct list_head endpoint_shared_keys;
    __u16 active_key_id;
    __u8 ecn_enable;
    __u8 auth_enable;
    __u8 intl_enable;
    __u8 prsctp_enable;
    __u8 asconf_enable;
    __u8 reconf_enable;
    __u8 strreset_enable;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct sctp_endpoint {
    struct sctp_ep_common base;
    struct hlist_node node;
    int hashent;
    struct list_head asocs;
    __u8 secret_key[32];
    __u8 *digest;
    __u32 sndbuf_policy;
    __u32 rcvbuf_policy;
    struct crypto_shash **auth_hmacs;
    struct sctp_hmac_algo_param *auth_hmacs_list;
    struct sctp_chunks_param *auth_chunk_list;
    struct list_head endpoint_shared_keys;
    __u16 active_key_id;
    __u8 ecn_enable;
    __u8 auth_enable;
    __u8 intl_enable;
    __u8 prsctp_enable;
    __u8 asconf_enable;
    __u8 reconf_enable;
    __u8 strreset_enable;
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
struct sctp_endpoint {
    struct sctp_ep_common base;
    struct list_head asocs;
    __u8 secret_key[32];
    __u8 *digest;
    __u32 sndbuf_policy;
    __u32 rcvbuf_policy;
    struct crypto_shash **auth_hmacs;
    struct sctp_hmac_algo_param *auth_hmacs_list;
    struct sctp_chunks_param *auth_chunk_list;
    struct list_head endpoint_shared_keys;
    __u16 active_key_id;
    __u8 ecn_enable;
    __u8 auth_enable;
    __u8 intl_enable;
    __u8 prsctp_enable;
    __u8 asconf_enable;
    __u8 reconf_enable;
    __u8 strreset_enable;
    u32 secid;
    u32 peer_secid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct sctp_endpoint {
    struct sctp_ep_common base;
    struct list_head asocs;
    __u8 secret_key[32];
    __u8 *digest;
    __u32 sndbuf_policy;
    __u32 rcvbuf_policy;
    struct crypto_shash **auth_hmacs;
    struct sctp_hmac_algo_param *auth_hmacs_list;
    struct sctp_chunks_param *auth_chunk_list;
    struct list_head endpoint_shared_keys;
    __u16 active_key_id;
    __u8 ecn_enable;
    __u8 auth_enable;
    __u8 intl_enable;
    __u8 prsctp_enable;
    __u8 asconf_enable;
    __u8 reconf_enable;
    __u8 strreset_enable;
    u32 secid;
    u32 peer_secid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct sctp_endpoint {
    struct sctp_ep_common base;
    struct list_head asocs;
    __u8 secret_key[32];
    __u8 *digest;
    __u32 sndbuf_policy;
    __u32 rcvbuf_policy;
    struct crypto_shash **auth_hmacs;
    struct sctp_hmac_algo_param *auth_hmacs_list;
    struct sctp_chunks_param *auth_chunk_list;
    struct list_head endpoint_shared_keys;
    __u16 active_key_id;
    __u8 ecn_enable;
    __u8 auth_enable;
    __u8 intl_enable;
    __u8 prsctp_enable;
    __u8 asconf_enable;
    __u8 reconf_enable;
    __u8 strreset_enable;
    u32 secid;
    u32 peer_secid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct sctp_endpoint {
    struct sctp_ep_common base;
    struct list_head asocs;
    __u8 secret_key[32];
    __u8 *digest;
    __u32 sndbuf_policy;
    __u32 rcvbuf_policy;
    struct crypto_shash **auth_hmacs;
    struct sctp_hmac_algo_param *auth_hmacs_list;
    struct sctp_chunks_param *auth_chunk_list;
    struct list_head endpoint_shared_keys;
    __u16 active_key_id;
    __u8 ecn_enable;
    __u8 auth_enable;
    __u8 intl_enable;
    __u8 prsctp_enable;
    __u8 asconf_enable;
    __u8 reconf_enable;
    __u8 strreset_enable;
    u32 secid;
    u32 peer_secid;
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
struct sctp_endpoint {
    struct sctp_ep_common base;
    struct list_head asocs;
    __u8 secret_key[32];
    __u8 *digest;
    __u32 sndbuf_policy;
    __u32 rcvbuf_policy;
    struct crypto_shash **auth_hmacs;
    struct sctp_hmac_algo_param *auth_hmacs_list;
    struct sctp_chunks_param *auth_chunk_list;
    struct list_head endpoint_shared_keys;
    __u16 active_key_id;
    __u8 ecn_enable;
    __u8 auth_enable;
    __u8 intl_enable;
    __u8 prsctp_enable;
    __u8 asconf_enable;
    __u8 reconf_enable;
    __u8 strreset_enable;
    u32 secid;
    u32 peer_secid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct sctp_endpoint {
    struct sctp_ep_common base;
    struct list_head asocs;
    __u8 secret_key[32];
    __u8 *digest;
    __u32 sndbuf_policy;
    __u32 rcvbuf_policy;
    struct crypto_shash **auth_hmacs;
    struct sctp_hmac_algo_param *auth_hmacs_list;
    struct sctp_chunks_param *auth_chunk_list;
    struct list_head endpoint_shared_keys;
    __u16 active_key_id;
    __u8 ecn_enable;
    __u8 auth_enable;
    __u8 intl_enable;
    __u8 prsctp_enable;
    __u8 asconf_enable;
    __u8 reconf_enable;
    __u8 strreset_enable;
    u32 secid;
    u32 peer_secid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct sctp_endpoint {
    struct sctp_ep_common base;
    struct list_head asocs;
    __u8 secret_key[32];
    __u8 *digest;
    __u32 sndbuf_policy;
    __u32 rcvbuf_policy;
    struct crypto_shash **auth_hmacs;
    struct sctp_hmac_algo_param *auth_hmacs_list;
    struct sctp_chunks_param *auth_chunk_list;
    struct list_head endpoint_shared_keys;
    __u16 active_key_id;
    __u8 ecn_enable;
    __u8 auth_enable;
    __u8 intl_enable;
    __u8 prsctp_enable;
    __u8 asconf_enable;
    __u8 reconf_enable;
    __u8 strreset_enable;
    u32 secid;
    u32 peer_secid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct sctp_endpoint {
    struct sctp_ep_common base;
    struct list_head asocs;
    __u8 secret_key[32];
    __u8 *digest;
    __u32 sndbuf_policy;
    __u32 rcvbuf_policy;
    struct crypto_shash **auth_hmacs;
    struct sctp_hmac_algo_param *auth_hmacs_list;
    struct sctp_chunks_param *auth_chunk_list;
    struct list_head endpoint_shared_keys;
    __u16 active_key_id;
    __u8 ecn_enable;
    __u8 auth_enable;
    __u8 intl_enable;
    __u8 prsctp_enable;
    __u8 asconf_enable;
    __u8 reconf_enable;
    __u8 strreset_enable;
    u32 secid;
    u32 peer_secid;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u8 intl_enable</code>
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
<code>__u8 ecn_enable</code>
</li>
<li>
<b>Field added. </b>
<code>__u8 asconf_enable</code>
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
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct callback_head rcu</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct hlist_node node</code>
</li>
<li>
<b>Field added. </b>
<code>int hashent</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 secid</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 peer_secid</code>
</li>
</ul>
</details>
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
