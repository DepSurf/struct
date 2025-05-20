# Struct: <code>genl_family</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct genl_family {
    unsigned int id;
    unsigned int hdrsize;
    char name[16];
    unsigned int version;
    unsigned int maxattr;
    bool netnsok;
    bool parallel_ops;
    int (*pre_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    int (*mcast_bind)(struct net *, int);
    void (*mcast_unbind)(struct net *, int);
    struct nlattr **attrbuf;
    const struct genl_ops *ops;
    const struct genl_multicast_group *mcgrps;
    unsigned int n_ops;
    unsigned int n_mcgrps;
    unsigned int mcgrp_offset;
    struct list_head family_list;
    struct module *module;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct genl_family {
    unsigned int id;
    unsigned int hdrsize;
    char name[16];
    unsigned int version;
    unsigned int maxattr;
    bool netnsok;
    bool parallel_ops;
    int (*pre_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    int (*mcast_bind)(struct net *, int);
    void (*mcast_unbind)(struct net *, int);
    struct nlattr **attrbuf;
    const struct genl_ops *ops;
    const struct genl_multicast_group *mcgrps;
    unsigned int n_ops;
    unsigned int n_mcgrps;
    unsigned int mcgrp_offset;
    struct list_head family_list;
    struct module *module;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct genl_family {
    int id;
    unsigned int hdrsize;
    char name[16];
    unsigned int version;
    unsigned int maxattr;
    bool netnsok;
    bool parallel_ops;
    int (*pre_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    int (*mcast_bind)(struct net *, int);
    void (*mcast_unbind)(struct net *, int);
    struct nlattr **attrbuf;
    const struct genl_ops *ops;
    const struct genl_multicast_group *mcgrps;
    unsigned int n_ops;
    unsigned int n_mcgrps;
    unsigned int mcgrp_offset;
    struct module *module;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct genl_family {
    int id;
    unsigned int hdrsize;
    char name[16];
    unsigned int version;
    unsigned int maxattr;
    bool netnsok;
    bool parallel_ops;
    int (*pre_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    int (*mcast_bind)(struct net *, int);
    void (*mcast_unbind)(struct net *, int);
    struct nlattr **attrbuf;
    const struct genl_ops *ops;
    const struct genl_multicast_group *mcgrps;
    unsigned int n_ops;
    unsigned int n_mcgrps;
    unsigned int mcgrp_offset;
    struct module *module;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct genl_family {
    int id;
    unsigned int hdrsize;
    char name[16];
    unsigned int version;
    unsigned int maxattr;
    bool netnsok;
    bool parallel_ops;
    int (*pre_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    int (*mcast_bind)(struct net *, int);
    void (*mcast_unbind)(struct net *, int);
    struct nlattr **attrbuf;
    const struct genl_ops *ops;
    const struct genl_multicast_group *mcgrps;
    unsigned int n_ops;
    unsigned int n_mcgrps;
    unsigned int mcgrp_offset;
    struct module *module;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct genl_family {
    int id;
    unsigned int hdrsize;
    char name[16];
    unsigned int version;
    unsigned int maxattr;
    bool netnsok;
    bool parallel_ops;
    int (*pre_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    int (*mcast_bind)(struct net *, int);
    void (*mcast_unbind)(struct net *, int);
    struct nlattr **attrbuf;
    const struct genl_ops *ops;
    const struct genl_multicast_group *mcgrps;
    unsigned int n_ops;
    unsigned int n_mcgrps;
    unsigned int mcgrp_offset;
    struct module *module;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct genl_family {
    int id;
    unsigned int hdrsize;
    char name[16];
    unsigned int version;
    unsigned int maxattr;
    bool netnsok;
    bool parallel_ops;
    int (*pre_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    int (*mcast_bind)(struct net *, int);
    void (*mcast_unbind)(struct net *, int);
    struct nlattr **attrbuf;
    const struct genl_ops *ops;
    const struct genl_multicast_group *mcgrps;
    unsigned int n_ops;
    unsigned int n_mcgrps;
    unsigned int mcgrp_offset;
    struct module *module;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct genl_family {
    int id;
    unsigned int hdrsize;
    char name[16];
    unsigned int version;
    unsigned int maxattr;
    bool netnsok;
    bool parallel_ops;
    const struct nla_policy *policy;
    int (*pre_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    int (*mcast_bind)(struct net *, int);
    void (*mcast_unbind)(struct net *, int);
    struct nlattr **attrbuf;
    const struct genl_ops *ops;
    const struct genl_multicast_group *mcgrps;
    unsigned int n_ops;
    unsigned int n_mcgrps;
    unsigned int mcgrp_offset;
    struct module *module;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct genl_family {
    int id;
    unsigned int hdrsize;
    char name[16];
    unsigned int version;
    unsigned int maxattr;
    bool netnsok;
    bool parallel_ops;
    const struct nla_policy *policy;
    int (*pre_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    int (*mcast_bind)(struct net *, int);
    void (*mcast_unbind)(struct net *, int);
    struct nlattr **attrbuf;
    const struct genl_ops *ops;
    const struct genl_multicast_group *mcgrps;
    unsigned int n_ops;
    unsigned int n_mcgrps;
    unsigned int mcgrp_offset;
    struct module *module;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct genl_family {
    int id;
    unsigned int hdrsize;
    char name[16];
    unsigned int version;
    unsigned int maxattr;
    bool netnsok;
    bool parallel_ops;
    const struct nla_policy *policy;
    int (*pre_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    const struct genl_ops *ops;
    const struct genl_multicast_group *mcgrps;
    unsigned int n_ops;
    unsigned int n_mcgrps;
    unsigned int mcgrp_offset;
    struct module *module;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct genl_family {
    int id;
    unsigned int hdrsize;
    char name[16];
    unsigned int version;
    unsigned int maxattr;
    unsigned int mcgrp_offset;
    u8 netnsok;
    u8 parallel_ops;
    u8 n_ops;
    u8 n_small_ops;
    u8 n_mcgrps;
    const struct nla_policy *policy;
    int (*pre_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    const struct genl_ops *ops;
    const struct genl_small_ops *small_ops;
    const struct genl_multicast_group *mcgrps;
    struct module *module;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct genl_family {
    int id;
    unsigned int hdrsize;
    char name[16];
    unsigned int version;
    unsigned int maxattr;
    unsigned int mcgrp_offset;
    u8 netnsok;
    u8 parallel_ops;
    u8 n_ops;
    u8 n_small_ops;
    u8 n_mcgrps;
    const struct nla_policy *policy;
    int (*pre_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    const struct genl_ops *ops;
    const struct genl_small_ops *small_ops;
    const struct genl_multicast_group *mcgrps;
    struct module *module;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct genl_family {
    int id;
    unsigned int hdrsize;
    char name[16];
    unsigned int version;
    unsigned int maxattr;
    unsigned int mcgrp_offset;
    u8 netnsok;
    u8 parallel_ops;
    u8 n_ops;
    u8 n_small_ops;
    u8 n_mcgrps;
    const struct nla_policy *policy;
    int (*pre_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    const struct genl_ops *ops;
    const struct genl_small_ops *small_ops;
    const struct genl_multicast_group *mcgrps;
    struct module *module;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct genl_family {
    int id;
    unsigned int hdrsize;
    char name[16];
    unsigned int version;
    unsigned int maxattr;
    unsigned int mcgrp_offset;
    u8 netnsok;
    u8 parallel_ops;
    u8 n_ops;
    u8 n_small_ops;
    u8 n_mcgrps;
    const struct nla_policy *policy;
    int (*pre_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    const struct genl_ops *ops;
    const struct genl_small_ops *small_ops;
    const struct genl_multicast_group *mcgrps;
    struct module *module;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct genl_family {
    unsigned int hdrsize;
    char name[16];
    unsigned int version;
    unsigned int maxattr;
    u8 netnsok;
    u8 parallel_ops;
    u8 n_ops;
    u8 n_small_ops;
    u8 n_split_ops;
    u8 n_mcgrps;
    u8 resv_start_op;
    const struct nla_policy *policy;
    int (*pre_doit)(const struct genl_split_ops *, struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_split_ops *, struct sk_buff *, struct genl_info *);
    const struct genl_ops *ops;
    const struct genl_small_ops *small_ops;
    const struct genl_split_ops *split_ops;
    const struct genl_multicast_group *mcgrps;
    struct module *module;
    int id;
    unsigned int mcgrp_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct genl_family {
    unsigned int hdrsize;
    char name[16];
    unsigned int version;
    unsigned int maxattr;
    u8 netnsok;
    u8 parallel_ops;
    u8 n_ops;
    u8 n_small_ops;
    u8 n_split_ops;
    u8 n_mcgrps;
    u8 resv_start_op;
    const struct nla_policy *policy;
    int (*pre_doit)(const struct genl_split_ops *, struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_split_ops *, struct sk_buff *, struct genl_info *);
    const struct genl_ops *ops;
    const struct genl_small_ops *small_ops;
    const struct genl_split_ops *split_ops;
    const struct genl_multicast_group *mcgrps;
    struct module *module;
    int id;
    unsigned int mcgrp_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct genl_family {
    unsigned int hdrsize;
    char name[16];
    unsigned int version;
    unsigned int maxattr;
    u8 netnsok;
    u8 parallel_ops;
    u8 n_ops;
    u8 n_small_ops;
    u8 n_split_ops;
    u8 n_mcgrps;
    u8 resv_start_op;
    const struct nla_policy *policy;
    int (*pre_doit)(const struct genl_split_ops *, struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_split_ops *, struct sk_buff *, struct genl_info *);
    const struct genl_ops *ops;
    const struct genl_small_ops *small_ops;
    const struct genl_split_ops *split_ops;
    const struct genl_multicast_group *mcgrps;
    struct module *module;
    size_t sock_priv_size;
    void (*sock_priv_init)(void *);
    void (*sock_priv_destroy)(void *);
    int id;
    unsigned int mcgrp_offset;
    struct xarray *sock_privs;
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
struct genl_family {
    int id;
    unsigned int hdrsize;
    char name[16];
    unsigned int version;
    unsigned int maxattr;
    bool netnsok;
    bool parallel_ops;
    const struct nla_policy *policy;
    int (*pre_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    int (*mcast_bind)(struct net *, int);
    void (*mcast_unbind)(struct net *, int);
    struct nlattr **attrbuf;
    const struct genl_ops *ops;
    const struct genl_multicast_group *mcgrps;
    unsigned int n_ops;
    unsigned int n_mcgrps;
    unsigned int mcgrp_offset;
    struct module *module;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct genl_family {
    int id;
    unsigned int hdrsize;
    char name[16];
    unsigned int version;
    unsigned int maxattr;
    bool netnsok;
    bool parallel_ops;
    const struct nla_policy *policy;
    int (*pre_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    int (*mcast_bind)(struct net *, int);
    void (*mcast_unbind)(struct net *, int);
    struct nlattr **attrbuf;
    const struct genl_ops *ops;
    const struct genl_multicast_group *mcgrps;
    unsigned int n_ops;
    unsigned int n_mcgrps;
    unsigned int mcgrp_offset;
    struct module *module;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct genl_family {
    int id;
    unsigned int hdrsize;
    char name[16];
    unsigned int version;
    unsigned int maxattr;
    bool netnsok;
    bool parallel_ops;
    const struct nla_policy *policy;
    int (*pre_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    int (*mcast_bind)(struct net *, int);
    void (*mcast_unbind)(struct net *, int);
    struct nlattr **attrbuf;
    const struct genl_ops *ops;
    const struct genl_multicast_group *mcgrps;
    unsigned int n_ops;
    unsigned int n_mcgrps;
    unsigned int mcgrp_offset;
    struct module *module;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct genl_family {
    int id;
    unsigned int hdrsize;
    char name[16];
    unsigned int version;
    unsigned int maxattr;
    bool netnsok;
    bool parallel_ops;
    const struct nla_policy *policy;
    int (*pre_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    int (*mcast_bind)(struct net *, int);
    void (*mcast_unbind)(struct net *, int);
    struct nlattr **attrbuf;
    const struct genl_ops *ops;
    const struct genl_multicast_group *mcgrps;
    unsigned int n_ops;
    unsigned int n_mcgrps;
    unsigned int mcgrp_offset;
    struct module *module;
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
struct genl_family {
    int id;
    unsigned int hdrsize;
    char name[16];
    unsigned int version;
    unsigned int maxattr;
    bool netnsok;
    bool parallel_ops;
    const struct nla_policy *policy;
    int (*pre_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    int (*mcast_bind)(struct net *, int);
    void (*mcast_unbind)(struct net *, int);
    struct nlattr **attrbuf;
    const struct genl_ops *ops;
    const struct genl_multicast_group *mcgrps;
    unsigned int n_ops;
    unsigned int n_mcgrps;
    unsigned int mcgrp_offset;
    struct module *module;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct genl_family {
    int id;
    unsigned int hdrsize;
    char name[16];
    unsigned int version;
    unsigned int maxattr;
    bool netnsok;
    bool parallel_ops;
    const struct nla_policy *policy;
    int (*pre_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    int (*mcast_bind)(struct net *, int);
    void (*mcast_unbind)(struct net *, int);
    struct nlattr **attrbuf;
    const struct genl_ops *ops;
    const struct genl_multicast_group *mcgrps;
    unsigned int n_ops;
    unsigned int n_mcgrps;
    unsigned int mcgrp_offset;
    struct module *module;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct genl_family {
    int id;
    unsigned int hdrsize;
    char name[16];
    unsigned int version;
    unsigned int maxattr;
    bool netnsok;
    bool parallel_ops;
    const struct nla_policy *policy;
    int (*pre_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    int (*mcast_bind)(struct net *, int);
    void (*mcast_unbind)(struct net *, int);
    struct nlattr **attrbuf;
    const struct genl_ops *ops;
    const struct genl_multicast_group *mcgrps;
    unsigned int n_ops;
    unsigned int n_mcgrps;
    unsigned int mcgrp_offset;
    struct module *module;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct genl_family {
    int id;
    unsigned int hdrsize;
    char name[16];
    unsigned int version;
    unsigned int maxattr;
    bool netnsok;
    bool parallel_ops;
    const struct nla_policy *policy;
    int (*pre_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *);
    int (*mcast_bind)(struct net *, int);
    void (*mcast_unbind)(struct net *, int);
    struct nlattr **attrbuf;
    const struct genl_ops *ops;
    const struct genl_multicast_group *mcgrps;
    unsigned int n_ops;
    unsigned int n_mcgrps;
    unsigned int mcgrp_offset;
    struct module *module;
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
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct list_head family_list</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int id</code> ➡️ <code>int id</code>
</li>
</ul>
</details>
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
<code>const struct nla_policy *policy</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*mcast_bind)(struct net *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*mcast_unbind)(struct net *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct nlattr **attrbuf</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 n_small_ops</code>
</li>
<li>
<b>Field added. </b>
<code>const struct genl_small_ops *small_ops</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool netnsok</code> ➡️ <code>u8 netnsok</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool parallel_ops</code> ➡️ <code>u8 parallel_ops</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int n_ops</code> ➡️ <code>u8 n_ops</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int n_mcgrps</code> ➡️ <code>u8 n_mcgrps</code>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 n_split_ops</code>
</li>
<li>
<b>Field added. </b>
<code>u8 resv_start_op</code>
</li>
<li>
<b>Field added. </b>
<code>const struct genl_split_ops *split_ops</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*pre_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *)</code> ➡️ <code>int (*pre_doit)(const struct genl_split_ops *, struct sk_buff *, struct genl_info *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*post_doit)(const struct genl_ops *, struct sk_buff *, struct genl_info *)</code> ➡️ <code>void (*post_doit)(const struct genl_split_ops *, struct sk_buff *, struct genl_info *)</code>
</li>
</ul>
</details>
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
<code>size_t sock_priv_size</code>
</li>
<li>
<b>Field added. </b>
<code>void (*sock_priv_init)(void *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*sock_priv_destroy)(void *)</code>
</li>
<li>
<b>Field added. </b>
<code>struct xarray *sock_privs</code>
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
