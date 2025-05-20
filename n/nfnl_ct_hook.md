# Struct: <code>nfnl_ct_hook</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct nfnl_ct_hook {
    struct nf_conn * (*get_ct)(const struct sk_buff *, enum ip_conntrack_info *);
    size_t (*build_size)(const struct nf_conn *);
    int (*build)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, u_int16_t, u_int16_t);
    int (*parse)(const struct nlattr *, struct nf_conn *);
    int (*attach_expect)(const struct nlattr *, struct nf_conn *, u32, u32);
    void (*seq_adjust)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, s32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct nfnl_ct_hook {
    struct nf_conn * (*get_ct)(const struct sk_buff *, enum ip_conntrack_info *);
    size_t (*build_size)(const struct nf_conn *);
    int (*build)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, u_int16_t, u_int16_t);
    int (*parse)(const struct nlattr *, struct nf_conn *);
    int (*attach_expect)(const struct nlattr *, struct nf_conn *, u32, u32);
    void (*seq_adjust)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, s32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct nfnl_ct_hook {
    struct nf_conn * (*get_ct)(const struct sk_buff *, enum ip_conntrack_info *);
    size_t (*build_size)(const struct nf_conn *);
    int (*build)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, u_int16_t, u_int16_t);
    int (*parse)(const struct nlattr *, struct nf_conn *);
    int (*attach_expect)(const struct nlattr *, struct nf_conn *, u32, u32);
    void (*seq_adjust)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, s32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct nfnl_ct_hook {
    struct nf_conn * (*get_ct)(const struct sk_buff *, enum ip_conntrack_info *);
    size_t (*build_size)(const struct nf_conn *);
    int (*build)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, u_int16_t, u_int16_t);
    int (*parse)(const struct nlattr *, struct nf_conn *);
    int (*attach_expect)(const struct nlattr *, struct nf_conn *, u32, u32);
    void (*seq_adjust)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, s32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct nfnl_ct_hook {
    struct nf_conn * (*get_ct)(const struct sk_buff *, enum ip_conntrack_info *);
    size_t (*build_size)(const struct nf_conn *);
    int (*build)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, u_int16_t, u_int16_t);
    int (*parse)(const struct nlattr *, struct nf_conn *);
    int (*attach_expect)(const struct nlattr *, struct nf_conn *, u32, u32);
    void (*seq_adjust)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, s32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct nfnl_ct_hook {
    struct nf_conn * (*get_ct)(const struct sk_buff *, enum ip_conntrack_info *);
    size_t (*build_size)(const struct nf_conn *);
    int (*build)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, u_int16_t, u_int16_t);
    int (*parse)(const struct nlattr *, struct nf_conn *);
    int (*attach_expect)(const struct nlattr *, struct nf_conn *, u32, u32);
    void (*seq_adjust)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, s32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct nfnl_ct_hook {
    struct nf_conn * (*get_ct)(const struct sk_buff *, enum ip_conntrack_info *);
    size_t (*build_size)(const struct nf_conn *);
    int (*build)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, u_int16_t, u_int16_t);
    int (*parse)(const struct nlattr *, struct nf_conn *);
    int (*attach_expect)(const struct nlattr *, struct nf_conn *, u32, u32);
    void (*seq_adjust)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, s32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct nfnl_ct_hook {
    struct nf_conn * (*get_ct)(const struct sk_buff *, enum ip_conntrack_info *);
    size_t (*build_size)(const struct nf_conn *);
    int (*build)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, u_int16_t, u_int16_t);
    int (*parse)(const struct nlattr *, struct nf_conn *);
    int (*attach_expect)(const struct nlattr *, struct nf_conn *, u32, u32);
    void (*seq_adjust)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, s32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct nfnl_ct_hook {
    struct nf_conn * (*get_ct)(const struct sk_buff *, enum ip_conntrack_info *);
    size_t (*build_size)(const struct nf_conn *);
    int (*build)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, u_int16_t, u_int16_t);
    int (*parse)(const struct nlattr *, struct nf_conn *);
    int (*attach_expect)(const struct nlattr *, struct nf_conn *, u32, u32);
    void (*seq_adjust)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, s32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct nfnl_ct_hook {
    struct nf_conn * (*get_ct)(const struct sk_buff *, enum ip_conntrack_info *);
    size_t (*build_size)(const struct nf_conn *);
    int (*build)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, u_int16_t, u_int16_t);
    int (*parse)(const struct nlattr *, struct nf_conn *);
    int (*attach_expect)(const struct nlattr *, struct nf_conn *, u32, u32);
    void (*seq_adjust)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, s32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct nfnl_ct_hook {
    struct nf_conn * (*get_ct)(const struct sk_buff *, enum ip_conntrack_info *);
    size_t (*build_size)(const struct nf_conn *);
    int (*build)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, u_int16_t, u_int16_t);
    int (*parse)(const struct nlattr *, struct nf_conn *);
    int (*attach_expect)(const struct nlattr *, struct nf_conn *, u32, u32);
    void (*seq_adjust)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, s32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct nfnl_ct_hook {
    size_t (*build_size)(const struct nf_conn *);
    int (*build)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, u_int16_t, u_int16_t);
    int (*parse)(const struct nlattr *, struct nf_conn *);
    int (*attach_expect)(const struct nlattr *, struct nf_conn *, u32, u32);
    void (*seq_adjust)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, s32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct nfnl_ct_hook {
    size_t (*build_size)(const struct nf_conn *);
    int (*build)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, u_int16_t, u_int16_t);
    int (*parse)(const struct nlattr *, struct nf_conn *);
    int (*attach_expect)(const struct nlattr *, struct nf_conn *, u32, u32);
    void (*seq_adjust)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, s32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct nfnl_ct_hook {
    size_t (*build_size)(const struct nf_conn *);
    int (*build)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, u_int16_t, u_int16_t);
    int (*parse)(const struct nlattr *, struct nf_conn *);
    int (*attach_expect)(const struct nlattr *, struct nf_conn *, u32, u32);
    void (*seq_adjust)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, s32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct nfnl_ct_hook {
    size_t (*build_size)(const struct nf_conn *);
    int (*build)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, u_int16_t, u_int16_t);
    int (*parse)(const struct nlattr *, struct nf_conn *);
    int (*attach_expect)(const struct nlattr *, struct nf_conn *, u32, u32);
    void (*seq_adjust)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, s32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct nfnl_ct_hook {
    size_t (*build_size)(const struct nf_conn *);
    int (*build)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, u_int16_t, u_int16_t);
    int (*parse)(const struct nlattr *, struct nf_conn *);
    int (*attach_expect)(const struct nlattr *, struct nf_conn *, u32, u32);
    void (*seq_adjust)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, s32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct nfnl_ct_hook {
    size_t (*build_size)(const struct nf_conn *);
    int (*build)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, u_int16_t, u_int16_t);
    int (*parse)(const struct nlattr *, struct nf_conn *);
    int (*attach_expect)(const struct nlattr *, struct nf_conn *, u32, u32);
    void (*seq_adjust)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, s32);
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
struct nfnl_ct_hook {
    struct nf_conn * (*get_ct)(const struct sk_buff *, enum ip_conntrack_info *);
    size_t (*build_size)(const struct nf_conn *);
    int (*build)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, u_int16_t, u_int16_t);
    int (*parse)(const struct nlattr *, struct nf_conn *);
    int (*attach_expect)(const struct nlattr *, struct nf_conn *, u32, u32);
    void (*seq_adjust)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, s32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct nfnl_ct_hook {
    struct nf_conn * (*get_ct)(const struct sk_buff *, enum ip_conntrack_info *);
    size_t (*build_size)(const struct nf_conn *);
    int (*build)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, u_int16_t, u_int16_t);
    int (*parse)(const struct nlattr *, struct nf_conn *);
    int (*attach_expect)(const struct nlattr *, struct nf_conn *, u32, u32);
    void (*seq_adjust)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, s32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct nfnl_ct_hook {
    struct nf_conn * (*get_ct)(const struct sk_buff *, enum ip_conntrack_info *);
    size_t (*build_size)(const struct nf_conn *);
    int (*build)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, u_int16_t, u_int16_t);
    int (*parse)(const struct nlattr *, struct nf_conn *);
    int (*attach_expect)(const struct nlattr *, struct nf_conn *, u32, u32);
    void (*seq_adjust)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, s32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct nfnl_ct_hook {
    struct nf_conn * (*get_ct)(const struct sk_buff *, enum ip_conntrack_info *);
    size_t (*build_size)(const struct nf_conn *);
    int (*build)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, u_int16_t, u_int16_t);
    int (*parse)(const struct nlattr *, struct nf_conn *);
    int (*attach_expect)(const struct nlattr *, struct nf_conn *, u32, u32);
    void (*seq_adjust)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, s32);
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
struct nfnl_ct_hook {
    struct nf_conn * (*get_ct)(const struct sk_buff *, enum ip_conntrack_info *);
    size_t (*build_size)(const struct nf_conn *);
    int (*build)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, u_int16_t, u_int16_t);
    int (*parse)(const struct nlattr *, struct nf_conn *);
    int (*attach_expect)(const struct nlattr *, struct nf_conn *, u32, u32);
    void (*seq_adjust)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, s32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct nfnl_ct_hook {
    struct nf_conn * (*get_ct)(const struct sk_buff *, enum ip_conntrack_info *);
    size_t (*build_size)(const struct nf_conn *);
    int (*build)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, u_int16_t, u_int16_t);
    int (*parse)(const struct nlattr *, struct nf_conn *);
    int (*attach_expect)(const struct nlattr *, struct nf_conn *, u32, u32);
    void (*seq_adjust)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, s32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct nfnl_ct_hook {
    struct nf_conn * (*get_ct)(const struct sk_buff *, enum ip_conntrack_info *);
    size_t (*build_size)(const struct nf_conn *);
    int (*build)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, u_int16_t, u_int16_t);
    int (*parse)(const struct nlattr *, struct nf_conn *);
    int (*attach_expect)(const struct nlattr *, struct nf_conn *, u32, u32);
    void (*seq_adjust)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, s32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct nfnl_ct_hook {
    struct nf_conn * (*get_ct)(const struct sk_buff *, enum ip_conntrack_info *);
    size_t (*build_size)(const struct nf_conn *);
    int (*build)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, u_int16_t, u_int16_t);
    int (*parse)(const struct nlattr *, struct nf_conn *);
    int (*attach_expect)(const struct nlattr *, struct nf_conn *, u32, u32);
    void (*seq_adjust)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, s32);
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct nf_conn * (*get_ct)(const struct sk_buff *, enum ip_conntrack_info *)</code> ➡️ <code>struct nf_conn * (*get_ct)(const struct sk_buff *, enum ip_conntrack_info *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>size_t (*build_size)(const struct nf_conn *)</code> ➡️ <code>size_t (*build_size)(const struct nf_conn *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*build)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, u_int16_t, u_int16_t)</code> ➡️ <code>int (*build)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, u_int16_t, u_int16_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*parse)(const struct nlattr *, struct nf_conn *)</code> ➡️ <code>int (*parse)(const struct nlattr *, struct nf_conn *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*attach_expect)(const struct nlattr *, struct nf_conn *, u32, u32)</code> ➡️ <code>int (*attach_expect)(const struct nlattr *, struct nf_conn *, u32, u32)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*seq_adjust)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, s32)</code> ➡️ <code>void (*seq_adjust)(struct sk_buff *, struct nf_conn *, enum ip_conntrack_info, s32)</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct nf_conn * (*get_ct)(const struct sk_buff *, enum ip_conntrack_info *)</code>
</li>
</ul>
</details>
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
