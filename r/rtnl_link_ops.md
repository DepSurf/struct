# Struct: <code>rtnl_link_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct rtnl_link_ops {
    struct list_head list;
    const char *kind;
    size_t priv_size;
    void (*setup)(struct net_device *);
    int maxtype;
    const struct nla_policy *policy;
    int (*validate)(struct nlattr **, struct nlattr **);
    int (*newlink)(struct net *, struct net_device *, struct nlattr **, struct nlattr **);
    int (*changelink)(struct net_device *, struct nlattr **, struct nlattr **);
    void (*dellink)(struct net_device *, struct list_head *);
    size_t (*get_size)(const struct net_device *);
    int (*fill_info)(struct sk_buff *, const struct net_device *);
    size_t (*get_xstats_size)(const struct net_device *);
    int (*fill_xstats)(struct sk_buff *, const struct net_device *);
    unsigned int (*get_num_tx_queues)();
    unsigned int (*get_num_rx_queues)();
    int slave_maxtype;
    const struct nla_policy *slave_policy;
    int (*slave_validate)(struct nlattr **, struct nlattr **);
    int (*slave_changelink)(struct net_device *, struct net_device *, struct nlattr **, struct nlattr **);
    size_t (*get_slave_size)(const struct net_device *, const struct net_device *);
    int (*fill_slave_info)(struct sk_buff *, const struct net_device *, const struct net_device *);
    struct net * (*get_link_net)(const struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct rtnl_link_ops {
    struct list_head list;
    const char *kind;
    size_t priv_size;
    void (*setup)(struct net_device *);
    int maxtype;
    const struct nla_policy *policy;
    int (*validate)(struct nlattr **, struct nlattr **);
    int (*newlink)(struct net *, struct net_device *, struct nlattr **, struct nlattr **);
    int (*changelink)(struct net_device *, struct nlattr **, struct nlattr **);
    void (*dellink)(struct net_device *, struct list_head *);
    size_t (*get_size)(const struct net_device *);
    int (*fill_info)(struct sk_buff *, const struct net_device *);
    size_t (*get_xstats_size)(const struct net_device *);
    int (*fill_xstats)(struct sk_buff *, const struct net_device *);
    unsigned int (*get_num_tx_queues)();
    unsigned int (*get_num_rx_queues)();
    int slave_maxtype;
    const struct nla_policy *slave_policy;
    int (*slave_validate)(struct nlattr **, struct nlattr **);
    int (*slave_changelink)(struct net_device *, struct net_device *, struct nlattr **, struct nlattr **);
    size_t (*get_slave_size)(const struct net_device *, const struct net_device *);
    int (*fill_slave_info)(struct sk_buff *, const struct net_device *, const struct net_device *);
    struct net * (*get_link_net)(const struct net_device *);
    size_t (*get_linkxstats_size)(const struct net_device *, int);
    int (*fill_linkxstats)(struct sk_buff *, const struct net_device *, int *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rtnl_link_ops {
    struct list_head list;
    const char *kind;
    size_t priv_size;
    void (*setup)(struct net_device *);
    int maxtype;
    const struct nla_policy *policy;
    int (*validate)(struct nlattr **, struct nlattr **);
    int (*newlink)(struct net *, struct net_device *, struct nlattr **, struct nlattr **);
    int (*changelink)(struct net_device *, struct nlattr **, struct nlattr **);
    void (*dellink)(struct net_device *, struct list_head *);
    size_t (*get_size)(const struct net_device *);
    int (*fill_info)(struct sk_buff *, const struct net_device *);
    size_t (*get_xstats_size)(const struct net_device *);
    int (*fill_xstats)(struct sk_buff *, const struct net_device *);
    unsigned int (*get_num_tx_queues)();
    unsigned int (*get_num_rx_queues)();
    int slave_maxtype;
    const struct nla_policy *slave_policy;
    int (*slave_validate)(struct nlattr **, struct nlattr **);
    int (*slave_changelink)(struct net_device *, struct net_device *, struct nlattr **, struct nlattr **);
    size_t (*get_slave_size)(const struct net_device *, const struct net_device *);
    int (*fill_slave_info)(struct sk_buff *, const struct net_device *, const struct net_device *);
    struct net * (*get_link_net)(const struct net_device *);
    size_t (*get_linkxstats_size)(const struct net_device *, int);
    int (*fill_linkxstats)(struct sk_buff *, const struct net_device *, int *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rtnl_link_ops {
    struct list_head list;
    const char *kind;
    size_t priv_size;
    void (*setup)(struct net_device *);
    int maxtype;
    const struct nla_policy *policy;
    int (*validate)(struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*newlink)(struct net *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*changelink)(struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    void (*dellink)(struct net_device *, struct list_head *);
    size_t (*get_size)(const struct net_device *);
    int (*fill_info)(struct sk_buff *, const struct net_device *);
    size_t (*get_xstats_size)(const struct net_device *);
    int (*fill_xstats)(struct sk_buff *, const struct net_device *);
    unsigned int (*get_num_tx_queues)();
    unsigned int (*get_num_rx_queues)();
    int slave_maxtype;
    const struct nla_policy *slave_policy;
    int (*slave_validate)(struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*slave_changelink)(struct net_device *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    size_t (*get_slave_size)(const struct net_device *, const struct net_device *);
    int (*fill_slave_info)(struct sk_buff *, const struct net_device *, const struct net_device *);
    struct net * (*get_link_net)(const struct net_device *);
    size_t (*get_linkxstats_size)(const struct net_device *, int);
    int (*fill_linkxstats)(struct sk_buff *, const struct net_device *, int *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rtnl_link_ops {
    struct list_head list;
    const char *kind;
    size_t priv_size;
    void (*setup)(struct net_device *);
    int maxtype;
    const struct nla_policy *policy;
    int (*validate)(struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*newlink)(struct net *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*changelink)(struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    void (*dellink)(struct net_device *, struct list_head *);
    size_t (*get_size)(const struct net_device *);
    int (*fill_info)(struct sk_buff *, const struct net_device *);
    size_t (*get_xstats_size)(const struct net_device *);
    int (*fill_xstats)(struct sk_buff *, const struct net_device *);
    unsigned int (*get_num_tx_queues)();
    unsigned int (*get_num_rx_queues)();
    int slave_maxtype;
    const struct nla_policy *slave_policy;
    int (*slave_changelink)(struct net_device *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    size_t (*get_slave_size)(const struct net_device *, const struct net_device *);
    int (*fill_slave_info)(struct sk_buff *, const struct net_device *, const struct net_device *);
    struct net * (*get_link_net)(const struct net_device *);
    size_t (*get_linkxstats_size)(const struct net_device *, int);
    int (*fill_linkxstats)(struct sk_buff *, const struct net_device *, int *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rtnl_link_ops {
    struct list_head list;
    const char *kind;
    size_t priv_size;
    void (*setup)(struct net_device *);
    unsigned int maxtype;
    const struct nla_policy *policy;
    int (*validate)(struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*newlink)(struct net *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*changelink)(struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    void (*dellink)(struct net_device *, struct list_head *);
    size_t (*get_size)(const struct net_device *);
    int (*fill_info)(struct sk_buff *, const struct net_device *);
    size_t (*get_xstats_size)(const struct net_device *);
    int (*fill_xstats)(struct sk_buff *, const struct net_device *);
    unsigned int (*get_num_tx_queues)();
    unsigned int (*get_num_rx_queues)();
    unsigned int slave_maxtype;
    const struct nla_policy *slave_policy;
    int (*slave_changelink)(struct net_device *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    size_t (*get_slave_size)(const struct net_device *, const struct net_device *);
    int (*fill_slave_info)(struct sk_buff *, const struct net_device *, const struct net_device *);
    struct net * (*get_link_net)(const struct net_device *);
    size_t (*get_linkxstats_size)(const struct net_device *, int);
    int (*fill_linkxstats)(struct sk_buff *, const struct net_device *, int *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rtnl_link_ops {
    struct list_head list;
    const char *kind;
    size_t priv_size;
    void (*setup)(struct net_device *);
    unsigned int maxtype;
    const struct nla_policy *policy;
    int (*validate)(struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*newlink)(struct net *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*changelink)(struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    void (*dellink)(struct net_device *, struct list_head *);
    size_t (*get_size)(const struct net_device *);
    int (*fill_info)(struct sk_buff *, const struct net_device *);
    size_t (*get_xstats_size)(const struct net_device *);
    int (*fill_xstats)(struct sk_buff *, const struct net_device *);
    unsigned int (*get_num_tx_queues)();
    unsigned int (*get_num_rx_queues)();
    unsigned int slave_maxtype;
    const struct nla_policy *slave_policy;
    int (*slave_changelink)(struct net_device *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    size_t (*get_slave_size)(const struct net_device *, const struct net_device *);
    int (*fill_slave_info)(struct sk_buff *, const struct net_device *, const struct net_device *);
    struct net * (*get_link_net)(const struct net_device *);
    size_t (*get_linkxstats_size)(const struct net_device *, int);
    int (*fill_linkxstats)(struct sk_buff *, const struct net_device *, int *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rtnl_link_ops {
    struct list_head list;
    const char *kind;
    size_t priv_size;
    void (*setup)(struct net_device *);
    unsigned int maxtype;
    const struct nla_policy *policy;
    int (*validate)(struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*newlink)(struct net *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*changelink)(struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    void (*dellink)(struct net_device *, struct list_head *);
    size_t (*get_size)(const struct net_device *);
    int (*fill_info)(struct sk_buff *, const struct net_device *);
    size_t (*get_xstats_size)(const struct net_device *);
    int (*fill_xstats)(struct sk_buff *, const struct net_device *);
    unsigned int (*get_num_tx_queues)();
    unsigned int (*get_num_rx_queues)();
    unsigned int slave_maxtype;
    const struct nla_policy *slave_policy;
    int (*slave_changelink)(struct net_device *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    size_t (*get_slave_size)(const struct net_device *, const struct net_device *);
    int (*fill_slave_info)(struct sk_buff *, const struct net_device *, const struct net_device *);
    struct net * (*get_link_net)(const struct net_device *);
    size_t (*get_linkxstats_size)(const struct net_device *, int);
    int (*fill_linkxstats)(struct sk_buff *, const struct net_device *, int *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rtnl_link_ops {
    struct list_head list;
    const char *kind;
    size_t priv_size;
    void (*setup)(struct net_device *);
    unsigned int maxtype;
    const struct nla_policy *policy;
    int (*validate)(struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*newlink)(struct net *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*changelink)(struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    void (*dellink)(struct net_device *, struct list_head *);
    size_t (*get_size)(const struct net_device *);
    int (*fill_info)(struct sk_buff *, const struct net_device *);
    size_t (*get_xstats_size)(const struct net_device *);
    int (*fill_xstats)(struct sk_buff *, const struct net_device *);
    unsigned int (*get_num_tx_queues)();
    unsigned int (*get_num_rx_queues)();
    unsigned int slave_maxtype;
    const struct nla_policy *slave_policy;
    int (*slave_changelink)(struct net_device *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    size_t (*get_slave_size)(const struct net_device *, const struct net_device *);
    int (*fill_slave_info)(struct sk_buff *, const struct net_device *, const struct net_device *);
    struct net * (*get_link_net)(const struct net_device *);
    size_t (*get_linkxstats_size)(const struct net_device *, int);
    int (*fill_linkxstats)(struct sk_buff *, const struct net_device *, int *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct rtnl_link_ops {
    struct list_head list;
    const char *kind;
    size_t priv_size;
    void (*setup)(struct net_device *);
    unsigned int maxtype;
    const struct nla_policy *policy;
    int (*validate)(struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*newlink)(struct net *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*changelink)(struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    void (*dellink)(struct net_device *, struct list_head *);
    size_t (*get_size)(const struct net_device *);
    int (*fill_info)(struct sk_buff *, const struct net_device *);
    size_t (*get_xstats_size)(const struct net_device *);
    int (*fill_xstats)(struct sk_buff *, const struct net_device *);
    unsigned int (*get_num_tx_queues)();
    unsigned int (*get_num_rx_queues)();
    unsigned int slave_maxtype;
    const struct nla_policy *slave_policy;
    int (*slave_changelink)(struct net_device *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    size_t (*get_slave_size)(const struct net_device *, const struct net_device *);
    int (*fill_slave_info)(struct sk_buff *, const struct net_device *, const struct net_device *);
    struct net * (*get_link_net)(const struct net_device *);
    size_t (*get_linkxstats_size)(const struct net_device *, int);
    int (*fill_linkxstats)(struct sk_buff *, const struct net_device *, int *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct rtnl_link_ops {
    struct list_head list;
    const char *kind;
    size_t priv_size;
    void (*setup)(struct net_device *);
    bool netns_refund;
    unsigned int maxtype;
    const struct nla_policy *policy;
    int (*validate)(struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*newlink)(struct net *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*changelink)(struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    void (*dellink)(struct net_device *, struct list_head *);
    size_t (*get_size)(const struct net_device *);
    int (*fill_info)(struct sk_buff *, const struct net_device *);
    size_t (*get_xstats_size)(const struct net_device *);
    int (*fill_xstats)(struct sk_buff *, const struct net_device *);
    unsigned int (*get_num_tx_queues)();
    unsigned int (*get_num_rx_queues)();
    unsigned int slave_maxtype;
    const struct nla_policy *slave_policy;
    int (*slave_changelink)(struct net_device *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    size_t (*get_slave_size)(const struct net_device *, const struct net_device *);
    int (*fill_slave_info)(struct sk_buff *, const struct net_device *, const struct net_device *);
    struct net * (*get_link_net)(const struct net_device *);
    size_t (*get_linkxstats_size)(const struct net_device *, int);
    int (*fill_linkxstats)(struct sk_buff *, const struct net_device *, int *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rtnl_link_ops {
    struct list_head list;
    const char *kind;
    size_t priv_size;
    void (*setup)(struct net_device *);
    bool netns_refund;
    unsigned int maxtype;
    const struct nla_policy *policy;
    int (*validate)(struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*newlink)(struct net *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*changelink)(struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    void (*dellink)(struct net_device *, struct list_head *);
    size_t (*get_size)(const struct net_device *);
    int (*fill_info)(struct sk_buff *, const struct net_device *);
    size_t (*get_xstats_size)(const struct net_device *);
    int (*fill_xstats)(struct sk_buff *, const struct net_device *);
    unsigned int (*get_num_tx_queues)();
    unsigned int (*get_num_rx_queues)();
    unsigned int slave_maxtype;
    const struct nla_policy *slave_policy;
    int (*slave_changelink)(struct net_device *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    size_t (*get_slave_size)(const struct net_device *, const struct net_device *);
    int (*fill_slave_info)(struct sk_buff *, const struct net_device *, const struct net_device *);
    struct net * (*get_link_net)(const struct net_device *);
    size_t (*get_linkxstats_size)(const struct net_device *, int);
    int (*fill_linkxstats)(struct sk_buff *, const struct net_device *, int *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rtnl_link_ops {
    struct list_head list;
    const char *kind;
    size_t priv_size;
    struct net_device * (*alloc)(struct nlattr **, const char *, unsigned char, unsigned int, unsigned int);
    void (*setup)(struct net_device *);
    bool netns_refund;
    unsigned int maxtype;
    const struct nla_policy *policy;
    int (*validate)(struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*newlink)(struct net *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*changelink)(struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    void (*dellink)(struct net_device *, struct list_head *);
    size_t (*get_size)(const struct net_device *);
    int (*fill_info)(struct sk_buff *, const struct net_device *);
    size_t (*get_xstats_size)(const struct net_device *);
    int (*fill_xstats)(struct sk_buff *, const struct net_device *);
    unsigned int (*get_num_tx_queues)();
    unsigned int (*get_num_rx_queues)();
    unsigned int slave_maxtype;
    const struct nla_policy *slave_policy;
    int (*slave_changelink)(struct net_device *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    size_t (*get_slave_size)(const struct net_device *, const struct net_device *);
    int (*fill_slave_info)(struct sk_buff *, const struct net_device *, const struct net_device *);
    struct net * (*get_link_net)(const struct net_device *);
    size_t (*get_linkxstats_size)(const struct net_device *, int);
    int (*fill_linkxstats)(struct sk_buff *, const struct net_device *, int *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rtnl_link_ops {
    struct list_head list;
    const char *kind;
    size_t priv_size;
    struct net_device * (*alloc)(struct nlattr **, const char *, unsigned char, unsigned int, unsigned int);
    void (*setup)(struct net_device *);
    bool netns_refund;
    unsigned int maxtype;
    const struct nla_policy *policy;
    int (*validate)(struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*newlink)(struct net *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*changelink)(struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    void (*dellink)(struct net_device *, struct list_head *);
    size_t (*get_size)(const struct net_device *);
    int (*fill_info)(struct sk_buff *, const struct net_device *);
    size_t (*get_xstats_size)(const struct net_device *);
    int (*fill_xstats)(struct sk_buff *, const struct net_device *);
    unsigned int (*get_num_tx_queues)();
    unsigned int (*get_num_rx_queues)();
    unsigned int slave_maxtype;
    const struct nla_policy *slave_policy;
    int (*slave_changelink)(struct net_device *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    size_t (*get_slave_size)(const struct net_device *, const struct net_device *);
    int (*fill_slave_info)(struct sk_buff *, const struct net_device *, const struct net_device *);
    struct net * (*get_link_net)(const struct net_device *);
    size_t (*get_linkxstats_size)(const struct net_device *, int);
    int (*fill_linkxstats)(struct sk_buff *, const struct net_device *, int *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rtnl_link_ops {
    struct list_head list;
    const char *kind;
    size_t priv_size;
    struct net_device * (*alloc)(struct nlattr **, const char *, unsigned char, unsigned int, unsigned int);
    void (*setup)(struct net_device *);
    bool netns_refund;
    unsigned int maxtype;
    const struct nla_policy *policy;
    int (*validate)(struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*newlink)(struct net *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*changelink)(struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    void (*dellink)(struct net_device *, struct list_head *);
    size_t (*get_size)(const struct net_device *);
    int (*fill_info)(struct sk_buff *, const struct net_device *);
    size_t (*get_xstats_size)(const struct net_device *);
    int (*fill_xstats)(struct sk_buff *, const struct net_device *);
    unsigned int (*get_num_tx_queues)();
    unsigned int (*get_num_rx_queues)();
    unsigned int slave_maxtype;
    const struct nla_policy *slave_policy;
    int (*slave_changelink)(struct net_device *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    size_t (*get_slave_size)(const struct net_device *, const struct net_device *);
    int (*fill_slave_info)(struct sk_buff *, const struct net_device *, const struct net_device *);
    struct net * (*get_link_net)(const struct net_device *);
    size_t (*get_linkxstats_size)(const struct net_device *, int);
    int (*fill_linkxstats)(struct sk_buff *, const struct net_device *, int *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rtnl_link_ops {
    struct list_head list;
    const char *kind;
    size_t priv_size;
    struct net_device * (*alloc)(struct nlattr **, const char *, unsigned char, unsigned int, unsigned int);
    void (*setup)(struct net_device *);
    bool netns_refund;
    unsigned int maxtype;
    const struct nla_policy *policy;
    int (*validate)(struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*newlink)(struct net *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*changelink)(struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    void (*dellink)(struct net_device *, struct list_head *);
    size_t (*get_size)(const struct net_device *);
    int (*fill_info)(struct sk_buff *, const struct net_device *);
    size_t (*get_xstats_size)(const struct net_device *);
    int (*fill_xstats)(struct sk_buff *, const struct net_device *);
    unsigned int (*get_num_tx_queues)();
    unsigned int (*get_num_rx_queues)();
    unsigned int slave_maxtype;
    const struct nla_policy *slave_policy;
    int (*slave_changelink)(struct net_device *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    size_t (*get_slave_size)(const struct net_device *, const struct net_device *);
    int (*fill_slave_info)(struct sk_buff *, const struct net_device *, const struct net_device *);
    struct net * (*get_link_net)(const struct net_device *);
    size_t (*get_linkxstats_size)(const struct net_device *, int);
    int (*fill_linkxstats)(struct sk_buff *, const struct net_device *, int *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rtnl_link_ops {
    struct list_head list;
    const char *kind;
    size_t priv_size;
    struct net_device * (*alloc)(struct nlattr **, const char *, unsigned char, unsigned int, unsigned int);
    void (*setup)(struct net_device *);
    bool netns_refund;
    unsigned int maxtype;
    const struct nla_policy *policy;
    int (*validate)(struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*newlink)(struct net *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*changelink)(struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    void (*dellink)(struct net_device *, struct list_head *);
    size_t (*get_size)(const struct net_device *);
    int (*fill_info)(struct sk_buff *, const struct net_device *);
    size_t (*get_xstats_size)(const struct net_device *);
    int (*fill_xstats)(struct sk_buff *, const struct net_device *);
    unsigned int (*get_num_tx_queues)();
    unsigned int (*get_num_rx_queues)();
    unsigned int slave_maxtype;
    const struct nla_policy *slave_policy;
    int (*slave_changelink)(struct net_device *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    size_t (*get_slave_size)(const struct net_device *, const struct net_device *);
    int (*fill_slave_info)(struct sk_buff *, const struct net_device *, const struct net_device *);
    struct net * (*get_link_net)(const struct net_device *);
    size_t (*get_linkxstats_size)(const struct net_device *, int);
    int (*fill_linkxstats)(struct sk_buff *, const struct net_device *, int *, int);
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
struct rtnl_link_ops {
    struct list_head list;
    const char *kind;
    size_t priv_size;
    void (*setup)(struct net_device *);
    unsigned int maxtype;
    const struct nla_policy *policy;
    int (*validate)(struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*newlink)(struct net *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*changelink)(struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    void (*dellink)(struct net_device *, struct list_head *);
    size_t (*get_size)(const struct net_device *);
    int (*fill_info)(struct sk_buff *, const struct net_device *);
    size_t (*get_xstats_size)(const struct net_device *);
    int (*fill_xstats)(struct sk_buff *, const struct net_device *);
    unsigned int (*get_num_tx_queues)();
    unsigned int (*get_num_rx_queues)();
    unsigned int slave_maxtype;
    const struct nla_policy *slave_policy;
    int (*slave_changelink)(struct net_device *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    size_t (*get_slave_size)(const struct net_device *, const struct net_device *);
    int (*fill_slave_info)(struct sk_buff *, const struct net_device *, const struct net_device *);
    struct net * (*get_link_net)(const struct net_device *);
    size_t (*get_linkxstats_size)(const struct net_device *, int);
    int (*fill_linkxstats)(struct sk_buff *, const struct net_device *, int *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rtnl_link_ops {
    struct list_head list;
    const char *kind;
    size_t priv_size;
    void (*setup)(struct net_device *);
    unsigned int maxtype;
    const struct nla_policy *policy;
    int (*validate)(struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*newlink)(struct net *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*changelink)(struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    void (*dellink)(struct net_device *, struct list_head *);
    size_t (*get_size)(const struct net_device *);
    int (*fill_info)(struct sk_buff *, const struct net_device *);
    size_t (*get_xstats_size)(const struct net_device *);
    int (*fill_xstats)(struct sk_buff *, const struct net_device *);
    unsigned int (*get_num_tx_queues)();
    unsigned int (*get_num_rx_queues)();
    unsigned int slave_maxtype;
    const struct nla_policy *slave_policy;
    int (*slave_changelink)(struct net_device *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    size_t (*get_slave_size)(const struct net_device *, const struct net_device *);
    int (*fill_slave_info)(struct sk_buff *, const struct net_device *, const struct net_device *);
    struct net * (*get_link_net)(const struct net_device *);
    size_t (*get_linkxstats_size)(const struct net_device *, int);
    int (*fill_linkxstats)(struct sk_buff *, const struct net_device *, int *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rtnl_link_ops {
    struct list_head list;
    const char *kind;
    size_t priv_size;
    void (*setup)(struct net_device *);
    unsigned int maxtype;
    const struct nla_policy *policy;
    int (*validate)(struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*newlink)(struct net *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*changelink)(struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    void (*dellink)(struct net_device *, struct list_head *);
    size_t (*get_size)(const struct net_device *);
    int (*fill_info)(struct sk_buff *, const struct net_device *);
    size_t (*get_xstats_size)(const struct net_device *);
    int (*fill_xstats)(struct sk_buff *, const struct net_device *);
    unsigned int (*get_num_tx_queues)();
    unsigned int (*get_num_rx_queues)();
    unsigned int slave_maxtype;
    const struct nla_policy *slave_policy;
    int (*slave_changelink)(struct net_device *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    size_t (*get_slave_size)(const struct net_device *, const struct net_device *);
    int (*fill_slave_info)(struct sk_buff *, const struct net_device *, const struct net_device *);
    struct net * (*get_link_net)(const struct net_device *);
    size_t (*get_linkxstats_size)(const struct net_device *, int);
    int (*fill_linkxstats)(struct sk_buff *, const struct net_device *, int *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct rtnl_link_ops {
    struct list_head list;
    const char *kind;
    size_t priv_size;
    void (*setup)(struct net_device *);
    unsigned int maxtype;
    const struct nla_policy *policy;
    int (*validate)(struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*newlink)(struct net *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*changelink)(struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    void (*dellink)(struct net_device *, struct list_head *);
    size_t (*get_size)(const struct net_device *);
    int (*fill_info)(struct sk_buff *, const struct net_device *);
    size_t (*get_xstats_size)(const struct net_device *);
    int (*fill_xstats)(struct sk_buff *, const struct net_device *);
    unsigned int (*get_num_tx_queues)();
    unsigned int (*get_num_rx_queues)();
    unsigned int slave_maxtype;
    const struct nla_policy *slave_policy;
    int (*slave_changelink)(struct net_device *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    size_t (*get_slave_size)(const struct net_device *, const struct net_device *);
    int (*fill_slave_info)(struct sk_buff *, const struct net_device *, const struct net_device *);
    struct net * (*get_link_net)(const struct net_device *);
    size_t (*get_linkxstats_size)(const struct net_device *, int);
    int (*fill_linkxstats)(struct sk_buff *, const struct net_device *, int *, int);
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
struct rtnl_link_ops {
    struct list_head list;
    const char *kind;
    size_t priv_size;
    void (*setup)(struct net_device *);
    unsigned int maxtype;
    const struct nla_policy *policy;
    int (*validate)(struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*newlink)(struct net *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*changelink)(struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    void (*dellink)(struct net_device *, struct list_head *);
    size_t (*get_size)(const struct net_device *);
    int (*fill_info)(struct sk_buff *, const struct net_device *);
    size_t (*get_xstats_size)(const struct net_device *);
    int (*fill_xstats)(struct sk_buff *, const struct net_device *);
    unsigned int (*get_num_tx_queues)();
    unsigned int (*get_num_rx_queues)();
    unsigned int slave_maxtype;
    const struct nla_policy *slave_policy;
    int (*slave_changelink)(struct net_device *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    size_t (*get_slave_size)(const struct net_device *, const struct net_device *);
    int (*fill_slave_info)(struct sk_buff *, const struct net_device *, const struct net_device *);
    struct net * (*get_link_net)(const struct net_device *);
    size_t (*get_linkxstats_size)(const struct net_device *, int);
    int (*fill_linkxstats)(struct sk_buff *, const struct net_device *, int *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rtnl_link_ops {
    struct list_head list;
    const char *kind;
    size_t priv_size;
    void (*setup)(struct net_device *);
    unsigned int maxtype;
    const struct nla_policy *policy;
    int (*validate)(struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*newlink)(struct net *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*changelink)(struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    void (*dellink)(struct net_device *, struct list_head *);
    size_t (*get_size)(const struct net_device *);
    int (*fill_info)(struct sk_buff *, const struct net_device *);
    size_t (*get_xstats_size)(const struct net_device *);
    int (*fill_xstats)(struct sk_buff *, const struct net_device *);
    unsigned int (*get_num_tx_queues)();
    unsigned int (*get_num_rx_queues)();
    unsigned int slave_maxtype;
    const struct nla_policy *slave_policy;
    int (*slave_changelink)(struct net_device *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    size_t (*get_slave_size)(const struct net_device *, const struct net_device *);
    int (*fill_slave_info)(struct sk_buff *, const struct net_device *, const struct net_device *);
    struct net * (*get_link_net)(const struct net_device *);
    size_t (*get_linkxstats_size)(const struct net_device *, int);
    int (*fill_linkxstats)(struct sk_buff *, const struct net_device *, int *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rtnl_link_ops {
    struct list_head list;
    const char *kind;
    size_t priv_size;
    void (*setup)(struct net_device *);
    unsigned int maxtype;
    const struct nla_policy *policy;
    int (*validate)(struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*newlink)(struct net *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*changelink)(struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    void (*dellink)(struct net_device *, struct list_head *);
    size_t (*get_size)(const struct net_device *);
    int (*fill_info)(struct sk_buff *, const struct net_device *);
    size_t (*get_xstats_size)(const struct net_device *);
    int (*fill_xstats)(struct sk_buff *, const struct net_device *);
    unsigned int (*get_num_tx_queues)();
    unsigned int (*get_num_rx_queues)();
    unsigned int slave_maxtype;
    const struct nla_policy *slave_policy;
    int (*slave_changelink)(struct net_device *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    size_t (*get_slave_size)(const struct net_device *, const struct net_device *);
    int (*fill_slave_info)(struct sk_buff *, const struct net_device *, const struct net_device *);
    struct net * (*get_link_net)(const struct net_device *);
    size_t (*get_linkxstats_size)(const struct net_device *, int);
    int (*fill_linkxstats)(struct sk_buff *, const struct net_device *, int *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rtnl_link_ops {
    struct list_head list;
    const char *kind;
    size_t priv_size;
    void (*setup)(struct net_device *);
    unsigned int maxtype;
    const struct nla_policy *policy;
    int (*validate)(struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*newlink)(struct net *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    int (*changelink)(struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    void (*dellink)(struct net_device *, struct list_head *);
    size_t (*get_size)(const struct net_device *);
    int (*fill_info)(struct sk_buff *, const struct net_device *);
    size_t (*get_xstats_size)(const struct net_device *);
    int (*fill_xstats)(struct sk_buff *, const struct net_device *);
    unsigned int (*get_num_tx_queues)();
    unsigned int (*get_num_rx_queues)();
    unsigned int slave_maxtype;
    const struct nla_policy *slave_policy;
    int (*slave_changelink)(struct net_device *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *);
    size_t (*get_slave_size)(const struct net_device *, const struct net_device *);
    int (*fill_slave_info)(struct sk_buff *, const struct net_device *, const struct net_device *);
    struct net * (*get_link_net)(const struct net_device *);
    size_t (*get_linkxstats_size)(const struct net_device *, int);
    int (*fill_linkxstats)(struct sk_buff *, const struct net_device *, int *, int);
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>size_t (*get_linkxstats_size)(const struct net_device *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*fill_linkxstats)(struct sk_buff *, const struct net_device *, int *, int)</code>
</li>
</ul>
</details>
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
<code>int (*validate)(struct nlattr **, struct nlattr **)</code> ➡️ <code>int (*validate)(struct nlattr **, struct nlattr **, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*newlink)(struct net *, struct net_device *, struct nlattr **, struct nlattr **)</code> ➡️ <code>int (*newlink)(struct net *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*changelink)(struct net_device *, struct nlattr **, struct nlattr **)</code> ➡️ <code>int (*changelink)(struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*slave_validate)(struct nlattr **, struct nlattr **)</code> ➡️ <code>int (*slave_validate)(struct nlattr **, struct nlattr **, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*slave_changelink)(struct net_device *, struct net_device *, struct nlattr **, struct nlattr **)</code> ➡️ <code>int (*slave_changelink)(struct net_device *, struct net_device *, struct nlattr **, struct nlattr **, struct netlink_ext_ack *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*slave_validate)(struct nlattr **, struct nlattr **, struct netlink_ext_ack *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int maxtype</code> ➡️ <code>unsigned int maxtype</code>
</li>
<li>
<b>Field type changed. </b>
<code>int slave_maxtype</code> ➡️ <code>unsigned int slave_maxtype</code>
</li>
</ul>
</details>
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
<b>Field added. </b>
<code>bool netns_refund</code>
</li>
</ul>
</details>
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
<code>struct net_device * (*alloc)(struct nlattr **, const char *, unsigned char, unsigned int, unsigned int)</code>
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
