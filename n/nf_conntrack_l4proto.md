# Struct: <code>nf_conntrack_l4proto</code>

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
In <code>5.0</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct nf_conntrack_l4proto {
    u_int8_t l4proto;
    bool allow_clash;
    u16 nlattr_size;
    bool (*can_early_drop)(const struct nf_conn *);
    int (*to_nlattr)(struct sk_buff *, struct nlattr *, struct nf_conn *);
    int (*from_nlattr)(struct nlattr **, struct nf_conn *);
    int (*tuple_to_nlattr)(struct sk_buff *, const struct nf_conntrack_tuple *);
    unsigned int (*nlattr_tuple_size)();
    int (*nlattr_to_tuple)(struct nlattr **, struct nf_conntrack_tuple *);
    const struct nla_policy *nla_policy;
    struct (anon) ctnl_timeout;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct nf_conntrack_l4proto {
    u_int8_t l4proto;
    bool allow_clash;
    u16 nlattr_size;
    bool (*can_early_drop)(const struct nf_conn *);
    int (*to_nlattr)(struct sk_buff *, struct nlattr *, struct nf_conn *);
    int (*from_nlattr)(struct nlattr **, struct nf_conn *);
    int (*tuple_to_nlattr)(struct sk_buff *, const struct nf_conntrack_tuple *);
    unsigned int (*nlattr_tuple_size)();
    int (*nlattr_to_tuple)(struct nlattr **, struct nf_conntrack_tuple *);
    const struct nla_policy *nla_policy;
    struct (anon) ctnl_timeout;
};
```
</details>
</li>
<li>
In <code>5.8</code>: Absent ⚠️
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
In <code>5.19</code>: Absent ⚠️
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
struct nf_conntrack_l4proto {
    u_int8_t l4proto;
    bool allow_clash;
    u16 nlattr_size;
    bool (*can_early_drop)(const struct nf_conn *);
    int (*to_nlattr)(struct sk_buff *, struct nlattr *, struct nf_conn *);
    int (*from_nlattr)(struct nlattr **, struct nf_conn *);
    int (*tuple_to_nlattr)(struct sk_buff *, const struct nf_conntrack_tuple *);
    unsigned int (*nlattr_tuple_size)();
    int (*nlattr_to_tuple)(struct nlattr **, struct nf_conntrack_tuple *);
    const struct nla_policy *nla_policy;
    struct (anon) ctnl_timeout;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct nf_conntrack_l4proto {
    u_int8_t l4proto;
    bool allow_clash;
    u16 nlattr_size;
    bool (*can_early_drop)(const struct nf_conn *);
    int (*to_nlattr)(struct sk_buff *, struct nlattr *, struct nf_conn *);
    int (*from_nlattr)(struct nlattr **, struct nf_conn *);
    int (*tuple_to_nlattr)(struct sk_buff *, const struct nf_conntrack_tuple *);
    unsigned int (*nlattr_tuple_size)();
    int (*nlattr_to_tuple)(struct nlattr **, struct nf_conntrack_tuple *);
    const struct nla_policy *nla_policy;
    struct (anon) ctnl_timeout;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct nf_conntrack_l4proto {
    u_int8_t l4proto;
    bool allow_clash;
    u16 nlattr_size;
    bool (*can_early_drop)(const struct nf_conn *);
    int (*to_nlattr)(struct sk_buff *, struct nlattr *, struct nf_conn *);
    int (*from_nlattr)(struct nlattr **, struct nf_conn *);
    int (*tuple_to_nlattr)(struct sk_buff *, const struct nf_conntrack_tuple *);
    unsigned int (*nlattr_tuple_size)();
    int (*nlattr_to_tuple)(struct nlattr **, struct nf_conntrack_tuple *);
    const struct nla_policy *nla_policy;
    struct (anon) ctnl_timeout;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct nf_conntrack_l4proto {
    u_int8_t l4proto;
    bool allow_clash;
    u16 nlattr_size;
    bool (*can_early_drop)(const struct nf_conn *);
    int (*to_nlattr)(struct sk_buff *, struct nlattr *, struct nf_conn *);
    int (*from_nlattr)(struct nlattr **, struct nf_conn *);
    int (*tuple_to_nlattr)(struct sk_buff *, const struct nf_conntrack_tuple *);
    unsigned int (*nlattr_tuple_size)();
    int (*nlattr_to_tuple)(struct nlattr **, struct nf_conntrack_tuple *);
    const struct nla_policy *nla_policy;
    struct (anon) ctnl_timeout;
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
struct nf_conntrack_l4proto {
    u_int8_t l4proto;
    bool allow_clash;
    u16 nlattr_size;
    bool (*can_early_drop)(const struct nf_conn *);
    int (*to_nlattr)(struct sk_buff *, struct nlattr *, struct nf_conn *);
    int (*from_nlattr)(struct nlattr **, struct nf_conn *);
    int (*tuple_to_nlattr)(struct sk_buff *, const struct nf_conntrack_tuple *);
    unsigned int (*nlattr_tuple_size)();
    int (*nlattr_to_tuple)(struct nlattr **, struct nf_conntrack_tuple *);
    const struct nla_policy *nla_policy;
    struct (anon) ctnl_timeout;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct nf_conntrack_l4proto {
    u_int8_t l4proto;
    bool allow_clash;
    u16 nlattr_size;
    bool (*can_early_drop)(const struct nf_conn *);
    int (*to_nlattr)(struct sk_buff *, struct nlattr *, struct nf_conn *);
    int (*from_nlattr)(struct nlattr **, struct nf_conn *);
    int (*tuple_to_nlattr)(struct sk_buff *, const struct nf_conntrack_tuple *);
    unsigned int (*nlattr_tuple_size)();
    int (*nlattr_to_tuple)(struct nlattr **, struct nf_conntrack_tuple *);
    const struct nla_policy *nla_policy;
    struct (anon) ctnl_timeout;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct nf_conntrack_l4proto {
    u_int8_t l4proto;
    bool allow_clash;
    u16 nlattr_size;
    bool (*can_early_drop)(const struct nf_conn *);
    int (*to_nlattr)(struct sk_buff *, struct nlattr *, struct nf_conn *);
    int (*from_nlattr)(struct nlattr **, struct nf_conn *);
    int (*tuple_to_nlattr)(struct sk_buff *, const struct nf_conntrack_tuple *);
    unsigned int (*nlattr_tuple_size)();
    int (*nlattr_to_tuple)(struct nlattr **, struct nf_conntrack_tuple *);
    const struct nla_policy *nla_policy;
    struct (anon) ctnl_timeout;
    void (*print_conntrack)(struct seq_file *, struct nf_conn *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct nf_conntrack_l4proto {
    u_int8_t l4proto;
    bool allow_clash;
    u16 nlattr_size;
    bool (*can_early_drop)(const struct nf_conn *);
    int (*to_nlattr)(struct sk_buff *, struct nlattr *, struct nf_conn *);
    int (*from_nlattr)(struct nlattr **, struct nf_conn *);
    int (*tuple_to_nlattr)(struct sk_buff *, const struct nf_conntrack_tuple *);
    unsigned int (*nlattr_tuple_size)();
    int (*nlattr_to_tuple)(struct nlattr **, struct nf_conntrack_tuple *);
    const struct nla_policy *nla_policy;
    struct (anon) ctnl_timeout;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
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
<details>
<summary>Changed between <code>generic</code> and <code>gcp</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*print_conntrack)(struct seq_file *, struct nf_conn *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
