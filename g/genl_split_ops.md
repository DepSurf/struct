# Struct: <code>genl_split_ops</code>

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
In <code>5.3</code>: Absent ⚠️
</li>
<li>
In <code>5.4</code>: Absent ⚠️
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
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct genl_split_ops {
    int (*pre_doit)(const struct genl_split_ops *, struct sk_buff *, struct genl_info *);
    int (*doit)(struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_split_ops *, struct sk_buff *, struct genl_info *);
    int (*start)(struct netlink_callback *);
    int (*dumpit)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    const struct nla_policy *policy;
    unsigned int maxattr;
    u8 cmd;
    u8 internal_flags;
    u8 flags;
    u8 validate;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct genl_split_ops {
    int (*pre_doit)(const struct genl_split_ops *, struct sk_buff *, struct genl_info *);
    int (*doit)(struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_split_ops *, struct sk_buff *, struct genl_info *);
    int (*start)(struct netlink_callback *);
    int (*dumpit)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    const struct nla_policy *policy;
    unsigned int maxattr;
    u8 cmd;
    u8 internal_flags;
    u8 flags;
    u8 validate;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct genl_split_ops {
    int (*pre_doit)(const struct genl_split_ops *, struct sk_buff *, struct genl_info *);
    int (*doit)(struct sk_buff *, struct genl_info *);
    void (*post_doit)(const struct genl_split_ops *, struct sk_buff *, struct genl_info *);
    int (*start)(struct netlink_callback *);
    int (*dumpit)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    const struct nla_policy *policy;
    unsigned int maxattr;
    u8 cmd;
    u8 internal_flags;
    u8 flags;
    u8 validate;
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
In <code>arm64</code>: Absent ⚠️
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
</li>
<li>
In <code>riscv64</code>: Absent ⚠️
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
In <code>aws</code>: Absent ⚠️
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
