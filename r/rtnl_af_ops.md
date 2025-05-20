# Struct: <code>rtnl_af_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct rtnl_af_ops {
    struct list_head list;
    int family;
    int (*fill_link_af)(struct sk_buff *, const struct net_device *, u32);
    size_t (*get_link_af_size)(const struct net_device *, u32);
    int (*validate_link_af)(const struct net_device *, const struct nlattr *);
    int (*set_link_af)(struct net_device *, const struct nlattr *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct rtnl_af_ops {
    struct list_head list;
    int family;
    int (*fill_link_af)(struct sk_buff *, const struct net_device *, u32);
    size_t (*get_link_af_size)(const struct net_device *, u32);
    int (*validate_link_af)(const struct net_device *, const struct nlattr *);
    int (*set_link_af)(struct net_device *, const struct nlattr *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rtnl_af_ops {
    struct list_head list;
    int family;
    int (*fill_link_af)(struct sk_buff *, const struct net_device *, u32);
    size_t (*get_link_af_size)(const struct net_device *, u32);
    int (*validate_link_af)(const struct net_device *, const struct nlattr *);
    int (*set_link_af)(struct net_device *, const struct nlattr *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rtnl_af_ops {
    struct list_head list;
    int family;
    int (*fill_link_af)(struct sk_buff *, const struct net_device *, u32);
    size_t (*get_link_af_size)(const struct net_device *, u32);
    int (*validate_link_af)(const struct net_device *, const struct nlattr *);
    int (*set_link_af)(struct net_device *, const struct nlattr *);
    int (*fill_stats_af)(struct sk_buff *, const struct net_device *);
    size_t (*get_stats_af_size)(const struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rtnl_af_ops {
    struct list_head list;
    int family;
    int (*fill_link_af)(struct sk_buff *, const struct net_device *, u32);
    size_t (*get_link_af_size)(const struct net_device *, u32);
    int (*validate_link_af)(const struct net_device *, const struct nlattr *);
    int (*set_link_af)(struct net_device *, const struct nlattr *);
    int (*fill_stats_af)(struct sk_buff *, const struct net_device *);
    size_t (*get_stats_af_size)(const struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rtnl_af_ops {
    struct list_head list;
    int family;
    int (*fill_link_af)(struct sk_buff *, const struct net_device *, u32);
    size_t (*get_link_af_size)(const struct net_device *, u32);
    int (*validate_link_af)(const struct net_device *, const struct nlattr *);
    int (*set_link_af)(struct net_device *, const struct nlattr *);
    int (*fill_stats_af)(struct sk_buff *, const struct net_device *);
    size_t (*get_stats_af_size)(const struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rtnl_af_ops {
    struct list_head list;
    int family;
    int (*fill_link_af)(struct sk_buff *, const struct net_device *, u32);
    size_t (*get_link_af_size)(const struct net_device *, u32);
    int (*validate_link_af)(const struct net_device *, const struct nlattr *);
    int (*set_link_af)(struct net_device *, const struct nlattr *);
    int (*fill_stats_af)(struct sk_buff *, const struct net_device *);
    size_t (*get_stats_af_size)(const struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rtnl_af_ops {
    struct list_head list;
    int family;
    int (*fill_link_af)(struct sk_buff *, const struct net_device *, u32);
    size_t (*get_link_af_size)(const struct net_device *, u32);
    int (*validate_link_af)(const struct net_device *, const struct nlattr *);
    int (*set_link_af)(struct net_device *, const struct nlattr *);
    int (*fill_stats_af)(struct sk_buff *, const struct net_device *);
    size_t (*get_stats_af_size)(const struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rtnl_af_ops {
    struct list_head list;
    int family;
    int (*fill_link_af)(struct sk_buff *, const struct net_device *, u32);
    size_t (*get_link_af_size)(const struct net_device *, u32);
    int (*validate_link_af)(const struct net_device *, const struct nlattr *);
    int (*set_link_af)(struct net_device *, const struct nlattr *);
    int (*fill_stats_af)(struct sk_buff *, const struct net_device *);
    size_t (*get_stats_af_size)(const struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct rtnl_af_ops {
    struct list_head list;
    int family;
    int (*fill_link_af)(struct sk_buff *, const struct net_device *, u32);
    size_t (*get_link_af_size)(const struct net_device *, u32);
    int (*validate_link_af)(const struct net_device *, const struct nlattr *);
    int (*set_link_af)(struct net_device *, const struct nlattr *);
    int (*fill_stats_af)(struct sk_buff *, const struct net_device *);
    size_t (*get_stats_af_size)(const struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct rtnl_af_ops {
    struct list_head list;
    int family;
    int (*fill_link_af)(struct sk_buff *, const struct net_device *, u32);
    size_t (*get_link_af_size)(const struct net_device *, u32);
    int (*validate_link_af)(const struct net_device *, const struct nlattr *);
    int (*set_link_af)(struct net_device *, const struct nlattr *);
    int (*fill_stats_af)(struct sk_buff *, const struct net_device *);
    size_t (*get_stats_af_size)(const struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rtnl_af_ops {
    struct list_head list;
    int family;
    int (*fill_link_af)(struct sk_buff *, const struct net_device *, u32);
    size_t (*get_link_af_size)(const struct net_device *, u32);
    int (*validate_link_af)(const struct net_device *, const struct nlattr *);
    int (*set_link_af)(struct net_device *, const struct nlattr *, struct netlink_ext_ack *);
    int (*fill_stats_af)(struct sk_buff *, const struct net_device *);
    size_t (*get_stats_af_size)(const struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rtnl_af_ops {
    struct list_head list;
    int family;
    int (*fill_link_af)(struct sk_buff *, const struct net_device *, u32);
    size_t (*get_link_af_size)(const struct net_device *, u32);
    int (*validate_link_af)(const struct net_device *, const struct nlattr *, struct netlink_ext_ack *);
    int (*set_link_af)(struct net_device *, const struct nlattr *, struct netlink_ext_ack *);
    int (*fill_stats_af)(struct sk_buff *, const struct net_device *);
    size_t (*get_stats_af_size)(const struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rtnl_af_ops {
    struct list_head list;
    int family;
    int (*fill_link_af)(struct sk_buff *, const struct net_device *, u32);
    size_t (*get_link_af_size)(const struct net_device *, u32);
    int (*validate_link_af)(const struct net_device *, const struct nlattr *, struct netlink_ext_ack *);
    int (*set_link_af)(struct net_device *, const struct nlattr *, struct netlink_ext_ack *);
    int (*fill_stats_af)(struct sk_buff *, const struct net_device *);
    size_t (*get_stats_af_size)(const struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rtnl_af_ops {
    struct list_head list;
    int family;
    int (*fill_link_af)(struct sk_buff *, const struct net_device *, u32);
    size_t (*get_link_af_size)(const struct net_device *, u32);
    int (*validate_link_af)(const struct net_device *, const struct nlattr *, struct netlink_ext_ack *);
    int (*set_link_af)(struct net_device *, const struct nlattr *, struct netlink_ext_ack *);
    int (*fill_stats_af)(struct sk_buff *, const struct net_device *);
    size_t (*get_stats_af_size)(const struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rtnl_af_ops {
    struct list_head list;
    int family;
    int (*fill_link_af)(struct sk_buff *, const struct net_device *, u32);
    size_t (*get_link_af_size)(const struct net_device *, u32);
    int (*validate_link_af)(const struct net_device *, const struct nlattr *, struct netlink_ext_ack *);
    int (*set_link_af)(struct net_device *, const struct nlattr *, struct netlink_ext_ack *);
    int (*fill_stats_af)(struct sk_buff *, const struct net_device *);
    size_t (*get_stats_af_size)(const struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rtnl_af_ops {
    struct list_head list;
    int family;
    int (*fill_link_af)(struct sk_buff *, const struct net_device *, u32);
    size_t (*get_link_af_size)(const struct net_device *, u32);
    int (*validate_link_af)(const struct net_device *, const struct nlattr *, struct netlink_ext_ack *);
    int (*set_link_af)(struct net_device *, const struct nlattr *, struct netlink_ext_ack *);
    int (*fill_stats_af)(struct sk_buff *, const struct net_device *);
    size_t (*get_stats_af_size)(const struct net_device *);
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
struct rtnl_af_ops {
    struct list_head list;
    int family;
    int (*fill_link_af)(struct sk_buff *, const struct net_device *, u32);
    size_t (*get_link_af_size)(const struct net_device *, u32);
    int (*validate_link_af)(const struct net_device *, const struct nlattr *);
    int (*set_link_af)(struct net_device *, const struct nlattr *);
    int (*fill_stats_af)(struct sk_buff *, const struct net_device *);
    size_t (*get_stats_af_size)(const struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rtnl_af_ops {
    struct list_head list;
    int family;
    int (*fill_link_af)(struct sk_buff *, const struct net_device *, u32);
    size_t (*get_link_af_size)(const struct net_device *, u32);
    int (*validate_link_af)(const struct net_device *, const struct nlattr *);
    int (*set_link_af)(struct net_device *, const struct nlattr *);
    int (*fill_stats_af)(struct sk_buff *, const struct net_device *);
    size_t (*get_stats_af_size)(const struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rtnl_af_ops {
    struct list_head list;
    int family;
    int (*fill_link_af)(struct sk_buff *, const struct net_device *, u32);
    size_t (*get_link_af_size)(const struct net_device *, u32);
    int (*validate_link_af)(const struct net_device *, const struct nlattr *);
    int (*set_link_af)(struct net_device *, const struct nlattr *);
    int (*fill_stats_af)(struct sk_buff *, const struct net_device *);
    size_t (*get_stats_af_size)(const struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct rtnl_af_ops {
    struct list_head list;
    int family;
    int (*fill_link_af)(struct sk_buff *, const struct net_device *, u32);
    size_t (*get_link_af_size)(const struct net_device *, u32);
    int (*validate_link_af)(const struct net_device *, const struct nlattr *);
    int (*set_link_af)(struct net_device *, const struct nlattr *);
    int (*fill_stats_af)(struct sk_buff *, const struct net_device *);
    size_t (*get_stats_af_size)(const struct net_device *);
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
struct rtnl_af_ops {
    struct list_head list;
    int family;
    int (*fill_link_af)(struct sk_buff *, const struct net_device *, u32);
    size_t (*get_link_af_size)(const struct net_device *, u32);
    int (*validate_link_af)(const struct net_device *, const struct nlattr *);
    int (*set_link_af)(struct net_device *, const struct nlattr *);
    int (*fill_stats_af)(struct sk_buff *, const struct net_device *);
    size_t (*get_stats_af_size)(const struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rtnl_af_ops {
    struct list_head list;
    int family;
    int (*fill_link_af)(struct sk_buff *, const struct net_device *, u32);
    size_t (*get_link_af_size)(const struct net_device *, u32);
    int (*validate_link_af)(const struct net_device *, const struct nlattr *);
    int (*set_link_af)(struct net_device *, const struct nlattr *);
    int (*fill_stats_af)(struct sk_buff *, const struct net_device *);
    size_t (*get_stats_af_size)(const struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rtnl_af_ops {
    struct list_head list;
    int family;
    int (*fill_link_af)(struct sk_buff *, const struct net_device *, u32);
    size_t (*get_link_af_size)(const struct net_device *, u32);
    int (*validate_link_af)(const struct net_device *, const struct nlattr *);
    int (*set_link_af)(struct net_device *, const struct nlattr *);
    int (*fill_stats_af)(struct sk_buff *, const struct net_device *);
    size_t (*get_stats_af_size)(const struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rtnl_af_ops {
    struct list_head list;
    int family;
    int (*fill_link_af)(struct sk_buff *, const struct net_device *, u32);
    size_t (*get_link_af_size)(const struct net_device *, u32);
    int (*validate_link_af)(const struct net_device *, const struct nlattr *);
    int (*set_link_af)(struct net_device *, const struct nlattr *);
    int (*fill_stats_af)(struct sk_buff *, const struct net_device *);
    size_t (*get_stats_af_size)(const struct net_device *);
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
<code>int (*fill_stats_af)(struct sk_buff *, const struct net_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>size_t (*get_stats_af_size)(const struct net_device *)</code>
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
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*set_link_af)(struct net_device *, const struct nlattr *)</code> ➡️ <code>int (*set_link_af)(struct net_device *, const struct nlattr *, struct netlink_ext_ack *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*validate_link_af)(const struct net_device *, const struct nlattr *)</code> ➡️ <code>int (*validate_link_af)(const struct net_device *, const struct nlattr *, struct netlink_ext_ack *)</code>
</li>
</ul>
</details>
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
