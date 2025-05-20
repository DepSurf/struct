# Struct: <code>tcp_sock_af_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct tcp_sock_af_ops {
    struct tcp_md5sig_key * (*md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    int (*md5_parse)(struct sock *, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct tcp_sock_af_ops {
    struct tcp_md5sig_key * (*md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    int (*md5_parse)(struct sock *, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct tcp_sock_af_ops {
    struct tcp_md5sig_key * (*md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    int (*md5_parse)(struct sock *, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct tcp_sock_af_ops {
    struct tcp_md5sig_key * (*md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    int (*md5_parse)(struct sock *, int, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct tcp_sock_af_ops {
    struct tcp_md5sig_key * (*md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    int (*md5_parse)(struct sock *, int, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct tcp_sock_af_ops {
    struct tcp_md5sig_key * (*md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    int (*md5_parse)(struct sock *, int, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct tcp_sock_af_ops {
    struct tcp_md5sig_key * (*md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    int (*md5_parse)(struct sock *, int, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct tcp_sock_af_ops {
    struct tcp_md5sig_key * (*md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    int (*md5_parse)(struct sock *, int, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct tcp_sock_af_ops {
    struct tcp_md5sig_key * (*md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    int (*md5_parse)(struct sock *, int, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct tcp_sock_af_ops {
    struct tcp_md5sig_key * (*md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    int (*md5_parse)(struct sock *, int, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct tcp_sock_af_ops {
    struct tcp_md5sig_key * (*md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    int (*md5_parse)(struct sock *, int, sockptr_t, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct tcp_sock_af_ops {
    struct tcp_md5sig_key * (*md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    int (*md5_parse)(struct sock *, int, sockptr_t, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct tcp_sock_af_ops {
    struct tcp_md5sig_key * (*md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    int (*md5_parse)(struct sock *, int, sockptr_t, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct tcp_sock_af_ops {
    struct tcp_md5sig_key * (*md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    int (*md5_parse)(struct sock *, int, sockptr_t, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct tcp_sock_af_ops {
    struct tcp_md5sig_key * (*md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    int (*md5_parse)(struct sock *, int, sockptr_t, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct tcp_sock_af_ops {
    struct tcp_md5sig_key * (*md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    int (*md5_parse)(struct sock *, int, sockptr_t, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct tcp_sock_af_ops {
    struct tcp_md5sig_key * (*md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    int (*md5_parse)(struct sock *, int, sockptr_t, int);
    int (*ao_parse)(struct sock *, int, sockptr_t, int);
    struct tcp_ao_key * (*ao_lookup)(const struct sock *, struct sock *, int, int);
    int (*ao_calc_key_sk)(struct tcp_ao_key *, u8 *, const struct sock *, __be32, __be32, bool);
    int (*calc_ao_hash)(char *, struct tcp_ao_key *, const struct sock *, const struct sk_buff *, const u8 *, int, u32);
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
struct tcp_sock_af_ops {
    struct tcp_md5sig_key * (*md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    int (*md5_parse)(struct sock *, int, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct tcp_sock_af_ops {
    struct tcp_md5sig_key * (*md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    int (*md5_parse)(struct sock *, int, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct tcp_sock_af_ops {
    struct tcp_md5sig_key * (*md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    int (*md5_parse)(struct sock *, int, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct tcp_sock_af_ops {
    struct tcp_md5sig_key * (*md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    int (*md5_parse)(struct sock *, int, char *, int);
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
struct tcp_sock_af_ops {
    struct tcp_md5sig_key * (*md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    int (*md5_parse)(struct sock *, int, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct tcp_sock_af_ops {
    struct tcp_md5sig_key * (*md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    int (*md5_parse)(struct sock *, int, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct tcp_sock_af_ops {
    struct tcp_md5sig_key * (*md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    int (*md5_parse)(struct sock *, int, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct tcp_sock_af_ops {
    struct tcp_md5sig_key * (*md5_lookup)(const struct sock *, const struct sock *);
    int (*calc_md5_hash)(char *, const struct tcp_md5sig_key *, const struct sock *, const struct sk_buff *);
    int (*md5_parse)(struct sock *, int, char *, int);
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.4</code> and <code>4.8</code> ✅
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*md5_parse)(struct sock *, char *, int)</code> ➡️ <code>int (*md5_parse)(struct sock *, int, char *, int)</code>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*md5_parse)(struct sock *, int, char *, int)</code> ➡️ <code>int (*md5_parse)(struct sock *, int, sockptr_t, int)</code>
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
No changes between <code>5.19</code> and <code>6.2</code> ✅
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
<code>int (*ao_parse)(struct sock *, int, sockptr_t, int)</code>
</li>
<li>
<b>Field added. </b>
<code>struct tcp_ao_key * (*ao_lookup)(const struct sock *, struct sock *, int, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*ao_calc_key_sk)(struct tcp_ao_key *, u8 *, const struct sock *, __be32, __be32, bool)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*calc_ao_hash)(char *, struct tcp_ao_key *, const struct sock *, const struct sk_buff *, const u8 *, int, u32)</code>
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
