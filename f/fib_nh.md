# Struct: <code>fib_nh</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct fib_nh {
    struct net_device *nh_dev;
    struct hlist_node nh_hash;
    struct fib_info *nh_parent;
    unsigned int nh_flags;
    unsigned char nh_scope;
    int nh_weight;
    atomic_t nh_upper_bound;
    __u32 nh_tclassid;
    int nh_oif;
    __be32 nh_gw;
    __be32 nh_saddr;
    int nh_saddr_genid;
    struct rtable **nh_pcpu_rth_output;
    struct rtable *nh_rth_input;
    struct fnhe_hash_bucket *nh_exceptions;
    struct lwtunnel_state *nh_lwtstate;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct fib_nh {
    struct net_device *nh_dev;
    struct hlist_node nh_hash;
    struct fib_info *nh_parent;
    unsigned int nh_flags;
    unsigned char nh_scope;
    int nh_weight;
    atomic_t nh_upper_bound;
    __u32 nh_tclassid;
    int nh_oif;
    __be32 nh_gw;
    __be32 nh_saddr;
    int nh_saddr_genid;
    struct rtable **nh_pcpu_rth_output;
    struct rtable *nh_rth_input;
    struct fnhe_hash_bucket *nh_exceptions;
    struct lwtunnel_state *nh_lwtstate;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct fib_nh {
    struct net_device *nh_dev;
    struct hlist_node nh_hash;
    struct fib_info *nh_parent;
    unsigned int nh_flags;
    unsigned char nh_scope;
    int nh_weight;
    atomic_t nh_upper_bound;
    __u32 nh_tclassid;
    int nh_oif;
    __be32 nh_gw;
    __be32 nh_saddr;
    int nh_saddr_genid;
    struct rtable **nh_pcpu_rth_output;
    struct rtable *nh_rth_input;
    struct fnhe_hash_bucket *nh_exceptions;
    struct lwtunnel_state *nh_lwtstate;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct fib_nh {
    struct net_device *nh_dev;
    struct hlist_node nh_hash;
    struct fib_info *nh_parent;
    unsigned int nh_flags;
    unsigned char nh_scope;
    int nh_weight;
    atomic_t nh_upper_bound;
    __u32 nh_tclassid;
    int nh_oif;
    __be32 nh_gw;
    __be32 nh_saddr;
    int nh_saddr_genid;
    struct rtable **nh_pcpu_rth_output;
    struct rtable *nh_rth_input;
    struct fnhe_hash_bucket *nh_exceptions;
    struct lwtunnel_state *nh_lwtstate;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct fib_nh {
    struct net_device *nh_dev;
    struct hlist_node nh_hash;
    struct fib_info *nh_parent;
    unsigned int nh_flags;
    unsigned char nh_scope;
    int nh_weight;
    atomic_t nh_upper_bound;
    __u32 nh_tclassid;
    int nh_oif;
    __be32 nh_gw;
    __be32 nh_saddr;
    int nh_saddr_genid;
    struct rtable **nh_pcpu_rth_output;
    struct rtable *nh_rth_input;
    struct fnhe_hash_bucket *nh_exceptions;
    struct lwtunnel_state *nh_lwtstate;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct fib_nh {
    struct net_device *nh_dev;
    struct hlist_node nh_hash;
    struct fib_info *nh_parent;
    unsigned int nh_flags;
    unsigned char nh_scope;
    int nh_weight;
    atomic_t nh_upper_bound;
    __u32 nh_tclassid;
    int nh_oif;
    __be32 nh_gw;
    __be32 nh_saddr;
    int nh_saddr_genid;
    struct rtable **nh_pcpu_rth_output;
    struct rtable *nh_rth_input;
    struct fnhe_hash_bucket *nh_exceptions;
    struct lwtunnel_state *nh_lwtstate;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct fib_nh {
    struct net_device *nh_dev;
    struct hlist_node nh_hash;
    struct fib_info *nh_parent;
    unsigned int nh_flags;
    unsigned char nh_scope;
    int nh_weight;
    atomic_t nh_upper_bound;
    __u32 nh_tclassid;
    int nh_oif;
    __be32 nh_gw;
    __be32 nh_saddr;
    int nh_saddr_genid;
    struct rtable **nh_pcpu_rth_output;
    struct rtable *nh_rth_input;
    struct fnhe_hash_bucket *nh_exceptions;
    struct lwtunnel_state *nh_lwtstate;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct fib_nh {
    struct fib_nh_common nh_common;
    struct hlist_node nh_hash;
    struct fib_info *nh_parent;
    __u32 nh_tclassid;
    __be32 nh_saddr;
    int nh_saddr_genid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct fib_nh {
    struct fib_nh_common nh_common;
    struct hlist_node nh_hash;
    struct fib_info *nh_parent;
    __u32 nh_tclassid;
    __be32 nh_saddr;
    int nh_saddr_genid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct fib_nh {
    struct fib_nh_common nh_common;
    struct hlist_node nh_hash;
    struct fib_info *nh_parent;
    __u32 nh_tclassid;
    __be32 nh_saddr;
    int nh_saddr_genid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct fib_nh {
    struct fib_nh_common nh_common;
    struct hlist_node nh_hash;
    struct fib_info *nh_parent;
    __u32 nh_tclassid;
    __be32 nh_saddr;
    int nh_saddr_genid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct fib_nh {
    struct fib_nh_common nh_common;
    struct hlist_node nh_hash;
    struct fib_info *nh_parent;
    __u32 nh_tclassid;
    __be32 nh_saddr;
    int nh_saddr_genid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct fib_nh {
    struct fib_nh_common nh_common;
    struct hlist_node nh_hash;
    struct fib_info *nh_parent;
    __u32 nh_tclassid;
    __be32 nh_saddr;
    int nh_saddr_genid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct fib_nh {
    struct fib_nh_common nh_common;
    struct hlist_node nh_hash;
    struct fib_info *nh_parent;
    __u32 nh_tclassid;
    __be32 nh_saddr;
    int nh_saddr_genid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct fib_nh {
    struct fib_nh_common nh_common;
    struct hlist_node nh_hash;
    struct fib_info *nh_parent;
    __u32 nh_tclassid;
    __be32 nh_saddr;
    int nh_saddr_genid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct fib_nh {
    struct fib_nh_common nh_common;
    struct hlist_node nh_hash;
    struct fib_info *nh_parent;
    __u32 nh_tclassid;
    __be32 nh_saddr;
    int nh_saddr_genid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct fib_nh {
    struct fib_nh_common nh_common;
    struct hlist_node nh_hash;
    struct fib_info *nh_parent;
    __u32 nh_tclassid;
    __be32 nh_saddr;
    int nh_saddr_genid;
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
struct fib_nh {
    struct fib_nh_common nh_common;
    struct hlist_node nh_hash;
    struct fib_info *nh_parent;
    __u32 nh_tclassid;
    __be32 nh_saddr;
    int nh_saddr_genid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct fib_nh {
    struct fib_nh_common nh_common;
    struct hlist_node nh_hash;
    struct fib_info *nh_parent;
    __u32 nh_tclassid;
    __be32 nh_saddr;
    int nh_saddr_genid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct fib_nh {
    struct fib_nh_common nh_common;
    struct hlist_node nh_hash;
    struct fib_info *nh_parent;
    __u32 nh_tclassid;
    __be32 nh_saddr;
    int nh_saddr_genid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct fib_nh {
    struct fib_nh_common nh_common;
    struct hlist_node nh_hash;
    struct fib_info *nh_parent;
    __u32 nh_tclassid;
    __be32 nh_saddr;
    int nh_saddr_genid;
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
struct fib_nh {
    struct fib_nh_common nh_common;
    struct hlist_node nh_hash;
    struct fib_info *nh_parent;
    __u32 nh_tclassid;
    __be32 nh_saddr;
    int nh_saddr_genid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct fib_nh {
    struct fib_nh_common nh_common;
    struct hlist_node nh_hash;
    struct fib_info *nh_parent;
    __u32 nh_tclassid;
    __be32 nh_saddr;
    int nh_saddr_genid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct fib_nh {
    struct fib_nh_common nh_common;
    struct hlist_node nh_hash;
    struct fib_info *nh_parent;
    __u32 nh_tclassid;
    __be32 nh_saddr;
    int nh_saddr_genid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct fib_nh {
    struct fib_nh_common nh_common;
    struct hlist_node nh_hash;
    struct fib_info *nh_parent;
    __u32 nh_tclassid;
    __be32 nh_saddr;
    int nh_saddr_genid;
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
<b>Field added. </b>
<code>struct fib_nh_common nh_common</code>
</li>
<li>
<b>Field removed. </b>
<code>struct net_device *nh_dev</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int nh_flags</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned char nh_scope</code>
</li>
<li>
<b>Field removed. </b>
<code>int nh_weight</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t nh_upper_bound</code>
</li>
<li>
<b>Field removed. </b>
<code>int nh_oif</code>
</li>
<li>
<b>Field removed. </b>
<code>__be32 nh_gw</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rtable **nh_pcpu_rth_output</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rtable *nh_rth_input</code>
</li>
<li>
<b>Field removed. </b>
<code>struct fnhe_hash_bucket *nh_exceptions</code>
</li>
<li>
<b>Field removed. </b>
<code>struct lwtunnel_state *nh_lwtstate</code>
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
