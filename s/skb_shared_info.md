# Struct: <code>skb_shared_info</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct skb_shared_info {
    unsigned char nr_frags;
    __u8 tx_flags;
    short unsigned int gso_size;
    short unsigned int gso_segs;
    short unsigned int gso_type;
    struct sk_buff *frag_list;
    struct skb_shared_hwtstamps hwtstamps;
    u32 tskey;
    __be32 ip6_frag_id;
    atomic_t dataref;
    void *destructor_arg;
    skb_frag_t frags[17];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct skb_shared_info {
    unsigned char nr_frags;
    __u8 tx_flags;
    short unsigned int gso_size;
    short unsigned int gso_segs;
    short unsigned int gso_type;
    struct sk_buff *frag_list;
    struct skb_shared_hwtstamps hwtstamps;
    u32 tskey;
    __be32 ip6_frag_id;
    atomic_t dataref;
    void *destructor_arg;
    skb_frag_t frags[17];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct skb_shared_info {
    unsigned char nr_frags;
    __u8 tx_flags;
    short unsigned int gso_size;
    short unsigned int gso_segs;
    short unsigned int gso_type;
    struct sk_buff *frag_list;
    struct skb_shared_hwtstamps hwtstamps;
    u32 tskey;
    __be32 ip6_frag_id;
    atomic_t dataref;
    void *destructor_arg;
    skb_frag_t frags[17];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct skb_shared_info {
    short unsigned int _unused;
    unsigned char nr_frags;
    __u8 tx_flags;
    short unsigned int gso_size;
    short unsigned int gso_segs;
    struct sk_buff *frag_list;
    struct skb_shared_hwtstamps hwtstamps;
    unsigned int gso_type;
    u32 tskey;
    __be32 ip6_frag_id;
    atomic_t dataref;
    void *destructor_arg;
    skb_frag_t frags[17];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct skb_shared_info {
    __u8 __unused;
    __u8 meta_len;
    __u8 nr_frags;
    __u8 tx_flags;
    short unsigned int gso_size;
    short unsigned int gso_segs;
    struct sk_buff *frag_list;
    struct skb_shared_hwtstamps hwtstamps;
    unsigned int gso_type;
    u32 tskey;
    atomic_t dataref;
    void *destructor_arg;
    skb_frag_t frags[17];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct skb_shared_info {
    __u8 __unused;
    __u8 meta_len;
    __u8 nr_frags;
    __u8 tx_flags;
    short unsigned int gso_size;
    short unsigned int gso_segs;
    struct sk_buff *frag_list;
    struct skb_shared_hwtstamps hwtstamps;
    unsigned int gso_type;
    u32 tskey;
    atomic_t dataref;
    void *destructor_arg;
    skb_frag_t frags[17];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct skb_shared_info {
    __u8 __unused;
    __u8 meta_len;
    __u8 nr_frags;
    __u8 tx_flags;
    short unsigned int gso_size;
    short unsigned int gso_segs;
    struct sk_buff *frag_list;
    struct skb_shared_hwtstamps hwtstamps;
    unsigned int gso_type;
    u32 tskey;
    atomic_t dataref;
    void *destructor_arg;
    skb_frag_t frags[17];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct skb_shared_info {
    __u8 __unused;
    __u8 meta_len;
    __u8 nr_frags;
    __u8 tx_flags;
    short unsigned int gso_size;
    short unsigned int gso_segs;
    struct sk_buff *frag_list;
    struct skb_shared_hwtstamps hwtstamps;
    unsigned int gso_type;
    u32 tskey;
    atomic_t dataref;
    void *destructor_arg;
    skb_frag_t frags[17];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct skb_shared_info {
    __u8 __unused;
    __u8 meta_len;
    __u8 nr_frags;
    __u8 tx_flags;
    short unsigned int gso_size;
    short unsigned int gso_segs;
    struct sk_buff *frag_list;
    struct skb_shared_hwtstamps hwtstamps;
    unsigned int gso_type;
    u32 tskey;
    atomic_t dataref;
    void *destructor_arg;
    skb_frag_t frags[17];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct skb_shared_info {
    __u8 __unused;
    __u8 meta_len;
    __u8 nr_frags;
    __u8 tx_flags;
    short unsigned int gso_size;
    short unsigned int gso_segs;
    struct sk_buff *frag_list;
    struct skb_shared_hwtstamps hwtstamps;
    unsigned int gso_type;
    u32 tskey;
    atomic_t dataref;
    void *destructor_arg;
    skb_frag_t frags[17];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct skb_shared_info {
    __u8 __unused;
    __u8 meta_len;
    __u8 nr_frags;
    __u8 tx_flags;
    short unsigned int gso_size;
    short unsigned int gso_segs;
    struct sk_buff *frag_list;
    struct skb_shared_hwtstamps hwtstamps;
    unsigned int gso_type;
    u32 tskey;
    atomic_t dataref;
    void *destructor_arg;
    skb_frag_t frags[17];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct skb_shared_info {
    __u8 flags;
    __u8 meta_len;
    __u8 nr_frags;
    __u8 tx_flags;
    short unsigned int gso_size;
    short unsigned int gso_segs;
    struct sk_buff *frag_list;
    struct skb_shared_hwtstamps hwtstamps;
    unsigned int gso_type;
    u32 tskey;
    atomic_t dataref;
    void *destructor_arg;
    skb_frag_t frags[17];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct skb_shared_info {
    __u8 flags;
    __u8 meta_len;
    __u8 nr_frags;
    __u8 tx_flags;
    short unsigned int gso_size;
    short unsigned int gso_segs;
    struct sk_buff *frag_list;
    struct skb_shared_hwtstamps hwtstamps;
    unsigned int gso_type;
    u32 tskey;
    atomic_t dataref;
    void *destructor_arg;
    skb_frag_t frags[17];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct skb_shared_info {
    __u8 flags;
    __u8 meta_len;
    __u8 nr_frags;
    __u8 tx_flags;
    short unsigned int gso_size;
    short unsigned int gso_segs;
    struct sk_buff *frag_list;
    struct skb_shared_hwtstamps hwtstamps;
    unsigned int gso_type;
    u32 tskey;
    atomic_t dataref;
    unsigned int xdp_frags_size;
    void *destructor_arg;
    skb_frag_t frags[17];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct skb_shared_info {
    __u8 flags;
    __u8 meta_len;
    __u8 nr_frags;
    __u8 tx_flags;
    short unsigned int gso_size;
    short unsigned int gso_segs;
    struct sk_buff *frag_list;
    struct skb_shared_hwtstamps hwtstamps;
    unsigned int gso_type;
    u32 tskey;
    atomic_t dataref;
    unsigned int xdp_frags_size;
    void *destructor_arg;
    skb_frag_t frags[17];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct skb_shared_info {
    __u8 flags;
    __u8 meta_len;
    __u8 nr_frags;
    __u8 tx_flags;
    short unsigned int gso_size;
    short unsigned int gso_segs;
    struct sk_buff *frag_list;
    struct skb_shared_hwtstamps hwtstamps;
    unsigned int gso_type;
    u32 tskey;
    atomic_t dataref;
    unsigned int xdp_frags_size;
    void *destructor_arg;
    skb_frag_t frags[17];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct skb_shared_info {
    __u8 flags;
    __u8 meta_len;
    __u8 nr_frags;
    __u8 tx_flags;
    short unsigned int gso_size;
    short unsigned int gso_segs;
    struct sk_buff *frag_list;
    struct skb_shared_hwtstamps hwtstamps;
    struct xsk_tx_metadata_compl xsk_meta;
    unsigned int gso_type;
    u32 tskey;
    atomic_t dataref;
    unsigned int xdp_frags_size;
    void *destructor_arg;
    skb_frag_t frags[17];
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
struct skb_shared_info {
    __u8 __unused;
    __u8 meta_len;
    __u8 nr_frags;
    __u8 tx_flags;
    short unsigned int gso_size;
    short unsigned int gso_segs;
    struct sk_buff *frag_list;
    struct skb_shared_hwtstamps hwtstamps;
    unsigned int gso_type;
    u32 tskey;
    atomic_t dataref;
    void *destructor_arg;
    skb_frag_t frags[17];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct skb_shared_info {
    __u8 __unused;
    __u8 meta_len;
    __u8 nr_frags;
    __u8 tx_flags;
    short unsigned int gso_size;
    short unsigned int gso_segs;
    struct sk_buff *frag_list;
    struct skb_shared_hwtstamps hwtstamps;
    unsigned int gso_type;
    u32 tskey;
    atomic_t dataref;
    void *destructor_arg;
    skb_frag_t frags[17];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct skb_shared_info {
    __u8 __unused;
    __u8 meta_len;
    __u8 nr_frags;
    __u8 tx_flags;
    short unsigned int gso_size;
    short unsigned int gso_segs;
    struct sk_buff *frag_list;
    struct skb_shared_hwtstamps hwtstamps;
    unsigned int gso_type;
    u32 tskey;
    atomic_t dataref;
    void *destructor_arg;
    skb_frag_t frags[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct skb_shared_info {
    __u8 __unused;
    __u8 meta_len;
    __u8 nr_frags;
    __u8 tx_flags;
    short unsigned int gso_size;
    short unsigned int gso_segs;
    struct sk_buff *frag_list;
    struct skb_shared_hwtstamps hwtstamps;
    unsigned int gso_type;
    u32 tskey;
    atomic_t dataref;
    void *destructor_arg;
    skb_frag_t frags[17];
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
struct skb_shared_info {
    __u8 __unused;
    __u8 meta_len;
    __u8 nr_frags;
    __u8 tx_flags;
    short unsigned int gso_size;
    short unsigned int gso_segs;
    struct sk_buff *frag_list;
    struct skb_shared_hwtstamps hwtstamps;
    unsigned int gso_type;
    u32 tskey;
    atomic_t dataref;
    void *destructor_arg;
    skb_frag_t frags[17];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct skb_shared_info {
    __u8 __unused;
    __u8 meta_len;
    __u8 nr_frags;
    __u8 tx_flags;
    short unsigned int gso_size;
    short unsigned int gso_segs;
    struct sk_buff *frag_list;
    struct skb_shared_hwtstamps hwtstamps;
    unsigned int gso_type;
    u32 tskey;
    atomic_t dataref;
    void *destructor_arg;
    skb_frag_t frags[17];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct skb_shared_info {
    __u8 __unused;
    __u8 meta_len;
    __u8 nr_frags;
    __u8 tx_flags;
    short unsigned int gso_size;
    short unsigned int gso_segs;
    struct sk_buff *frag_list;
    struct skb_shared_hwtstamps hwtstamps;
    unsigned int gso_type;
    u32 tskey;
    atomic_t dataref;
    void *destructor_arg;
    skb_frag_t frags[17];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct skb_shared_info {
    __u8 __unused;
    __u8 meta_len;
    __u8 nr_frags;
    __u8 tx_flags;
    short unsigned int gso_size;
    short unsigned int gso_segs;
    struct sk_buff *frag_list;
    struct skb_shared_hwtstamps hwtstamps;
    unsigned int gso_type;
    u32 tskey;
    atomic_t dataref;
    void *destructor_arg;
    skb_frag_t frags[17];
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
<b>Field added. </b>
<code>short unsigned int _unused</code>
</li>
<li>
<b>Field type changed. </b>
<code>short unsigned int gso_type</code> ➡️ <code>unsigned int gso_type</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u8 __unused</code>
</li>
<li>
<b>Field added. </b>
<code>__u8 meta_len</code>
</li>
<li>
<b>Field removed. </b>
<code>short unsigned int _unused</code>
</li>
<li>
<b>Field removed. </b>
<code>__be32 ip6_frag_id</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned char nr_frags</code> ➡️ <code>__u8 nr_frags</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u8 flags</code>
</li>
<li>
<b>Field removed. </b>
<code>__u8 __unused</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int xdp_frags_size</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct xsk_tx_metadata_compl xsk_meta</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>skb_frag_t frags[17]</code> ➡️ <code>skb_frag_t frags[16]</code>
</li>
</ul>
</details>
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
