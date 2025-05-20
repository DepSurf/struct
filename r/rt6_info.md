# Struct: <code>rt6_info</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct rt6_info {
    struct dst_entry dst;
    struct fib6_table *rt6i_table;
    struct fib6_node *rt6i_node;
    struct in6_addr rt6i_gateway;
    struct list_head rt6i_siblings;
    unsigned int rt6i_nsiblings;
    atomic_t rt6i_ref;
    struct rt6key rt6i_dst;
    u32 rt6i_flags;
    struct rt6key rt6i_src;
    struct rt6key rt6i_prefsrc;
    struct list_head rt6i_uncached;
    struct uncached_list *rt6i_uncached_list;
    struct inet6_dev *rt6i_idev;
    struct rt6_info **rt6i_pcpu;
    u32 rt6i_metric;
    u32 rt6i_pmtu;
    short unsigned int rt6i_nfheader_len;
    u8 rt6i_protocol;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct rt6_info {
    struct dst_entry dst;
    struct fib6_table *rt6i_table;
    struct fib6_node *rt6i_node;
    struct in6_addr rt6i_gateway;
    struct list_head rt6i_siblings;
    unsigned int rt6i_nsiblings;
    atomic_t rt6i_ref;
    struct rt6key rt6i_dst;
    u32 rt6i_flags;
    struct rt6key rt6i_src;
    struct rt6key rt6i_prefsrc;
    struct list_head rt6i_uncached;
    struct uncached_list *rt6i_uncached_list;
    struct inet6_dev *rt6i_idev;
    struct rt6_info **rt6i_pcpu;
    u32 rt6i_metric;
    u32 rt6i_pmtu;
    short unsigned int rt6i_nfheader_len;
    u8 rt6i_protocol;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rt6_info {
    struct dst_entry dst;
    struct fib6_table *rt6i_table;
    struct fib6_node *rt6i_node;
    struct in6_addr rt6i_gateway;
    struct list_head rt6i_siblings;
    unsigned int rt6i_nsiblings;
    atomic_t rt6i_ref;
    struct rt6key rt6i_dst;
    u32 rt6i_flags;
    struct rt6key rt6i_src;
    struct rt6key rt6i_prefsrc;
    struct list_head rt6i_uncached;
    struct uncached_list *rt6i_uncached_list;
    struct inet6_dev *rt6i_idev;
    struct rt6_info **rt6i_pcpu;
    u32 rt6i_metric;
    u32 rt6i_pmtu;
    short unsigned int rt6i_nfheader_len;
    u8 rt6i_protocol;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rt6_info {
    struct dst_entry dst;
    struct fib6_table *rt6i_table;
    struct fib6_node *rt6i_node;
    struct in6_addr rt6i_gateway;
    struct list_head rt6i_siblings;
    unsigned int rt6i_nsiblings;
    atomic_t rt6i_ref;
    struct rt6key rt6i_dst;
    u32 rt6i_flags;
    struct rt6key rt6i_src;
    struct rt6key rt6i_prefsrc;
    struct list_head rt6i_uncached;
    struct uncached_list *rt6i_uncached_list;
    struct inet6_dev *rt6i_idev;
    struct rt6_info **rt6i_pcpu;
    u32 rt6i_metric;
    u32 rt6i_pmtu;
    short unsigned int rt6i_nfheader_len;
    u8 rt6i_protocol;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rt6_info {
    struct dst_entry dst;
    struct fib6_table *rt6i_table;
    struct fib6_node *rt6i_node;
    struct in6_addr rt6i_gateway;
    struct list_head rt6i_siblings;
    unsigned int rt6i_nsiblings;
    atomic_t rt6i_ref;
    unsigned int rt6i_nh_flags;
    struct rt6key rt6i_dst;
    u32 rt6i_flags;
    struct rt6key rt6i_src;
    struct rt6key rt6i_prefsrc;
    struct list_head rt6i_uncached;
    struct uncached_list *rt6i_uncached_list;
    struct inet6_dev *rt6i_idev;
    struct rt6_info **rt6i_pcpu;
    struct rt6_exception_bucket *rt6i_exception_bucket;
    u32 rt6i_metric;
    u32 rt6i_pmtu;
    short unsigned int rt6i_nfheader_len;
    u8 rt6i_protocol;
    u8 exception_bucket_flushed;
    u8 unused;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rt6_info {
    struct dst_entry dst;
    struct fib6_info *from;
    struct rt6key rt6i_dst;
    struct rt6key rt6i_src;
    struct in6_addr rt6i_gateway;
    struct inet6_dev *rt6i_idev;
    u32 rt6i_flags;
    struct rt6key rt6i_prefsrc;
    struct list_head rt6i_uncached;
    struct uncached_list *rt6i_uncached_list;
    short unsigned int rt6i_nfheader_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rt6_info {
    struct dst_entry dst;
    struct fib6_info *from;
    struct rt6key rt6i_dst;
    struct rt6key rt6i_src;
    struct in6_addr rt6i_gateway;
    struct inet6_dev *rt6i_idev;
    u32 rt6i_flags;
    struct list_head rt6i_uncached;
    struct uncached_list *rt6i_uncached_list;
    short unsigned int rt6i_nfheader_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rt6_info {
    struct dst_entry dst;
    struct fib6_info *from;
    struct rt6key rt6i_dst;
    struct rt6key rt6i_src;
    struct in6_addr rt6i_gateway;
    struct inet6_dev *rt6i_idev;
    u32 rt6i_flags;
    struct list_head rt6i_uncached;
    struct uncached_list *rt6i_uncached_list;
    short unsigned int rt6i_nfheader_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rt6_info {
    struct dst_entry dst;
    struct fib6_info *from;
    struct rt6key rt6i_dst;
    struct rt6key rt6i_src;
    struct in6_addr rt6i_gateway;
    struct inet6_dev *rt6i_idev;
    u32 rt6i_flags;
    struct list_head rt6i_uncached;
    struct uncached_list *rt6i_uncached_list;
    short unsigned int rt6i_nfheader_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct rt6_info {
    struct dst_entry dst;
    struct fib6_info *from;
    int sernum;
    struct rt6key rt6i_dst;
    struct rt6key rt6i_src;
    struct in6_addr rt6i_gateway;
    struct inet6_dev *rt6i_idev;
    u32 rt6i_flags;
    struct list_head rt6i_uncached;
    struct uncached_list *rt6i_uncached_list;
    short unsigned int rt6i_nfheader_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct rt6_info {
    struct dst_entry dst;
    struct fib6_info *from;
    int sernum;
    struct rt6key rt6i_dst;
    struct rt6key rt6i_src;
    struct in6_addr rt6i_gateway;
    struct inet6_dev *rt6i_idev;
    u32 rt6i_flags;
    struct list_head rt6i_uncached;
    struct uncached_list *rt6i_uncached_list;
    short unsigned int rt6i_nfheader_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rt6_info {
    struct dst_entry dst;
    struct fib6_info *from;
    int sernum;
    struct rt6key rt6i_dst;
    struct rt6key rt6i_src;
    struct in6_addr rt6i_gateway;
    struct inet6_dev *rt6i_idev;
    u32 rt6i_flags;
    struct list_head rt6i_uncached;
    struct uncached_list *rt6i_uncached_list;
    short unsigned int rt6i_nfheader_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rt6_info {
    struct dst_entry dst;
    struct fib6_info *from;
    int sernum;
    struct rt6key rt6i_dst;
    struct rt6key rt6i_src;
    struct in6_addr rt6i_gateway;
    struct inet6_dev *rt6i_idev;
    u32 rt6i_flags;
    struct list_head rt6i_uncached;
    struct uncached_list *rt6i_uncached_list;
    short unsigned int rt6i_nfheader_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rt6_info {
    struct dst_entry dst;
    struct fib6_info *from;
    int sernum;
    struct rt6key rt6i_dst;
    struct rt6key rt6i_src;
    struct in6_addr rt6i_gateway;
    struct inet6_dev *rt6i_idev;
    u32 rt6i_flags;
    struct list_head rt6i_uncached;
    struct uncached_list *rt6i_uncached_list;
    short unsigned int rt6i_nfheader_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rt6_info {
    struct dst_entry dst;
    struct fib6_info *from;
    int sernum;
    struct rt6key rt6i_dst;
    struct rt6key rt6i_src;
    struct in6_addr rt6i_gateway;
    struct inet6_dev *rt6i_idev;
    u32 rt6i_flags;
    struct list_head rt6i_uncached;
    struct uncached_list *rt6i_uncached_list;
    short unsigned int rt6i_nfheader_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rt6_info {
    struct dst_entry dst;
    struct fib6_info *from;
    int sernum;
    struct rt6key rt6i_dst;
    struct rt6key rt6i_src;
    struct in6_addr rt6i_gateway;
    struct inet6_dev *rt6i_idev;
    u32 rt6i_flags;
    short unsigned int rt6i_nfheader_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rt6_info {
    struct dst_entry dst;
    struct fib6_info *from;
    int sernum;
    struct rt6key rt6i_dst;
    struct rt6key rt6i_src;
    struct in6_addr rt6i_gateway;
    struct inet6_dev *rt6i_idev;
    u32 rt6i_flags;
    short unsigned int rt6i_nfheader_len;
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
struct rt6_info {
    struct dst_entry dst;
    struct fib6_info *from;
    struct rt6key rt6i_dst;
    struct rt6key rt6i_src;
    struct in6_addr rt6i_gateway;
    struct inet6_dev *rt6i_idev;
    u32 rt6i_flags;
    struct list_head rt6i_uncached;
    struct uncached_list *rt6i_uncached_list;
    short unsigned int rt6i_nfheader_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rt6_info {
    struct dst_entry dst;
    struct fib6_info *from;
    struct rt6key rt6i_dst;
    struct rt6key rt6i_src;
    struct in6_addr rt6i_gateway;
    struct inet6_dev *rt6i_idev;
    u32 rt6i_flags;
    struct list_head rt6i_uncached;
    struct uncached_list *rt6i_uncached_list;
    short unsigned int rt6i_nfheader_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rt6_info {
    struct dst_entry dst;
    struct fib6_info *from;
    struct rt6key rt6i_dst;
    struct rt6key rt6i_src;
    struct in6_addr rt6i_gateway;
    struct inet6_dev *rt6i_idev;
    u32 rt6i_flags;
    struct list_head rt6i_uncached;
    struct uncached_list *rt6i_uncached_list;
    short unsigned int rt6i_nfheader_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct rt6_info {
    struct dst_entry dst;
    struct fib6_info *from;
    struct rt6key rt6i_dst;
    struct rt6key rt6i_src;
    struct in6_addr rt6i_gateway;
    struct inet6_dev *rt6i_idev;
    u32 rt6i_flags;
    struct list_head rt6i_uncached;
    struct uncached_list *rt6i_uncached_list;
    short unsigned int rt6i_nfheader_len;
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
struct rt6_info {
    struct dst_entry dst;
    struct fib6_info *from;
    struct rt6key rt6i_dst;
    struct rt6key rt6i_src;
    struct in6_addr rt6i_gateway;
    struct inet6_dev *rt6i_idev;
    u32 rt6i_flags;
    struct list_head rt6i_uncached;
    struct uncached_list *rt6i_uncached_list;
    short unsigned int rt6i_nfheader_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rt6_info {
    struct dst_entry dst;
    struct fib6_info *from;
    struct rt6key rt6i_dst;
    struct rt6key rt6i_src;
    struct in6_addr rt6i_gateway;
    struct inet6_dev *rt6i_idev;
    u32 rt6i_flags;
    struct list_head rt6i_uncached;
    struct uncached_list *rt6i_uncached_list;
    short unsigned int rt6i_nfheader_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rt6_info {
    struct dst_entry dst;
    struct fib6_info *from;
    struct rt6key rt6i_dst;
    struct rt6key rt6i_src;
    struct in6_addr rt6i_gateway;
    struct inet6_dev *rt6i_idev;
    u32 rt6i_flags;
    struct list_head rt6i_uncached;
    struct uncached_list *rt6i_uncached_list;
    short unsigned int rt6i_nfheader_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rt6_info {
    struct dst_entry dst;
    struct fib6_info *from;
    struct rt6key rt6i_dst;
    struct rt6key rt6i_src;
    struct in6_addr rt6i_gateway;
    struct inet6_dev *rt6i_idev;
    u32 rt6i_flags;
    struct list_head rt6i_uncached;
    struct uncached_list *rt6i_uncached_list;
    short unsigned int rt6i_nfheader_len;
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
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int rt6i_nh_flags</code>
</li>
<li>
<b>Field added. </b>
<code>struct rt6_exception_bucket *rt6i_exception_bucket</code>
</li>
<li>
<b>Field added. </b>
<code>u8 exception_bucket_flushed</code>
</li>
<li>
<b>Field added. </b>
<code>u8 unused</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct fib6_info *from</code>
</li>
<li>
<b>Field removed. </b>
<code>struct fib6_table *rt6i_table</code>
</li>
<li>
<b>Field removed. </b>
<code>struct fib6_node *rt6i_node</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head rt6i_siblings</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int rt6i_nsiblings</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t rt6i_ref</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int rt6i_nh_flags</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rt6_info **rt6i_pcpu</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rt6_exception_bucket *rt6i_exception_bucket</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 rt6i_metric</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 rt6i_pmtu</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 rt6i_protocol</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 exception_bucket_flushed</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 unused</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct rt6key rt6i_prefsrc</code>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int sernum</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct list_head rt6i_uncached</code>
</li>
<li>
<b>Field removed. </b>
<code>struct uncached_list *rt6i_uncached_list</code>
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
