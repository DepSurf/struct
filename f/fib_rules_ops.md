# Struct: <code>fib_rules_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct fib_rules_ops {
    int family;
    struct list_head list;
    int rule_size;
    int addr_size;
    int unresolved_rules;
    int nr_goto_rules;
    int (*action)(struct fib_rule *, struct flowi *, int, struct fib_lookup_arg *);
    bool (*suppress)(struct fib_rule *, struct fib_lookup_arg *);
    int (*match)(struct fib_rule *, struct flowi *, int);
    int (*configure)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *, struct nlattr **);
    int (*delete)(struct fib_rule *);
    int (*compare)(struct fib_rule *, struct fib_rule_hdr *, struct nlattr **);
    int (*fill)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *);
    size_t (*nlmsg_payload)(struct fib_rule *);
    void (*flush_cache)(struct fib_rules_ops *);
    int nlgroup;
    const struct nla_policy *policy;
    struct list_head rules_list;
    struct module *owner;
    struct net *fro_net;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct fib_rules_ops {
    int family;
    struct list_head list;
    int rule_size;
    int addr_size;
    int unresolved_rules;
    int nr_goto_rules;
    int (*action)(struct fib_rule *, struct flowi *, int, struct fib_lookup_arg *);
    bool (*suppress)(struct fib_rule *, struct fib_lookup_arg *);
    int (*match)(struct fib_rule *, struct flowi *, int);
    int (*configure)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *, struct nlattr **);
    int (*delete)(struct fib_rule *);
    int (*compare)(struct fib_rule *, struct fib_rule_hdr *, struct nlattr **);
    int (*fill)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *);
    size_t (*nlmsg_payload)(struct fib_rule *);
    void (*flush_cache)(struct fib_rules_ops *);
    int nlgroup;
    const struct nla_policy *policy;
    struct list_head rules_list;
    struct module *owner;
    struct net *fro_net;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct fib_rules_ops {
    int family;
    struct list_head list;
    int rule_size;
    int addr_size;
    int unresolved_rules;
    int nr_goto_rules;
    int (*action)(struct fib_rule *, struct flowi *, int, struct fib_lookup_arg *);
    bool (*suppress)(struct fib_rule *, struct fib_lookup_arg *);
    int (*match)(struct fib_rule *, struct flowi *, int);
    int (*configure)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *, struct nlattr **);
    int (*delete)(struct fib_rule *);
    int (*compare)(struct fib_rule *, struct fib_rule_hdr *, struct nlattr **);
    int (*fill)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *);
    size_t (*nlmsg_payload)(struct fib_rule *);
    void (*flush_cache)(struct fib_rules_ops *);
    int nlgroup;
    const struct nla_policy *policy;
    struct list_head rules_list;
    struct module *owner;
    struct net *fro_net;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct fib_rules_ops {
    int family;
    struct list_head list;
    int rule_size;
    int addr_size;
    int unresolved_rules;
    int nr_goto_rules;
    int (*action)(struct fib_rule *, struct flowi *, int, struct fib_lookup_arg *);
    bool (*suppress)(struct fib_rule *, struct fib_lookup_arg *);
    int (*match)(struct fib_rule *, struct flowi *, int);
    int (*configure)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *, struct nlattr **);
    int (*delete)(struct fib_rule *);
    int (*compare)(struct fib_rule *, struct fib_rule_hdr *, struct nlattr **);
    int (*fill)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *);
    size_t (*nlmsg_payload)(struct fib_rule *);
    void (*flush_cache)(struct fib_rules_ops *);
    int nlgroup;
    const struct nla_policy *policy;
    struct list_head rules_list;
    struct module *owner;
    struct net *fro_net;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct fib_rules_ops {
    int family;
    struct list_head list;
    int rule_size;
    int addr_size;
    int unresolved_rules;
    int nr_goto_rules;
    unsigned int fib_rules_seq;
    int (*action)(struct fib_rule *, struct flowi *, int, struct fib_lookup_arg *);
    bool (*suppress)(struct fib_rule *, struct fib_lookup_arg *);
    int (*match)(struct fib_rule *, struct flowi *, int);
    int (*configure)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *, struct nlattr **);
    int (*delete)(struct fib_rule *);
    int (*compare)(struct fib_rule *, struct fib_rule_hdr *, struct nlattr **);
    int (*fill)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *);
    size_t (*nlmsg_payload)(struct fib_rule *);
    void (*flush_cache)(struct fib_rules_ops *);
    int nlgroup;
    const struct nla_policy *policy;
    struct list_head rules_list;
    struct module *owner;
    struct net *fro_net;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct fib_rules_ops {
    int family;
    struct list_head list;
    int rule_size;
    int addr_size;
    int unresolved_rules;
    int nr_goto_rules;
    unsigned int fib_rules_seq;
    int (*action)(struct fib_rule *, struct flowi *, int, struct fib_lookup_arg *);
    bool (*suppress)(struct fib_rule *, struct fib_lookup_arg *);
    int (*match)(struct fib_rule *, struct flowi *, int);
    int (*configure)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *, struct nlattr **, struct netlink_ext_ack *);
    int (*delete)(struct fib_rule *);
    int (*compare)(struct fib_rule *, struct fib_rule_hdr *, struct nlattr **);
    int (*fill)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *);
    size_t (*nlmsg_payload)(struct fib_rule *);
    void (*flush_cache)(struct fib_rules_ops *);
    int nlgroup;
    const struct nla_policy *policy;
    struct list_head rules_list;
    struct module *owner;
    struct net *fro_net;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct fib_rules_ops {
    int family;
    struct list_head list;
    int rule_size;
    int addr_size;
    int unresolved_rules;
    int nr_goto_rules;
    unsigned int fib_rules_seq;
    int (*action)(struct fib_rule *, struct flowi *, int, struct fib_lookup_arg *);
    bool (*suppress)(struct fib_rule *, struct fib_lookup_arg *);
    int (*match)(struct fib_rule *, struct flowi *, int);
    int (*configure)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *, struct nlattr **, struct netlink_ext_ack *);
    int (*delete)(struct fib_rule *);
    int (*compare)(struct fib_rule *, struct fib_rule_hdr *, struct nlattr **);
    int (*fill)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *);
    size_t (*nlmsg_payload)(struct fib_rule *);
    void (*flush_cache)(struct fib_rules_ops *);
    int nlgroup;
    const struct nla_policy *policy;
    struct list_head rules_list;
    struct module *owner;
    struct net *fro_net;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct fib_rules_ops {
    int family;
    struct list_head list;
    int rule_size;
    int addr_size;
    int unresolved_rules;
    int nr_goto_rules;
    unsigned int fib_rules_seq;
    int (*action)(struct fib_rule *, struct flowi *, int, struct fib_lookup_arg *);
    bool (*suppress)(struct fib_rule *, struct fib_lookup_arg *);
    int (*match)(struct fib_rule *, struct flowi *, int);
    int (*configure)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *, struct nlattr **, struct netlink_ext_ack *);
    int (*delete)(struct fib_rule *);
    int (*compare)(struct fib_rule *, struct fib_rule_hdr *, struct nlattr **);
    int (*fill)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *);
    size_t (*nlmsg_payload)(struct fib_rule *);
    void (*flush_cache)(struct fib_rules_ops *);
    int nlgroup;
    const struct nla_policy *policy;
    struct list_head rules_list;
    struct module *owner;
    struct net *fro_net;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct fib_rules_ops {
    int family;
    struct list_head list;
    int rule_size;
    int addr_size;
    int unresolved_rules;
    int nr_goto_rules;
    unsigned int fib_rules_seq;
    int (*action)(struct fib_rule *, struct flowi *, int, struct fib_lookup_arg *);
    bool (*suppress)(struct fib_rule *, struct fib_lookup_arg *);
    int (*match)(struct fib_rule *, struct flowi *, int);
    int (*configure)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *, struct nlattr **, struct netlink_ext_ack *);
    int (*delete)(struct fib_rule *);
    int (*compare)(struct fib_rule *, struct fib_rule_hdr *, struct nlattr **);
    int (*fill)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *);
    size_t (*nlmsg_payload)(struct fib_rule *);
    void (*flush_cache)(struct fib_rules_ops *);
    int nlgroup;
    const struct nla_policy *policy;
    struct list_head rules_list;
    struct module *owner;
    struct net *fro_net;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct fib_rules_ops {
    int family;
    struct list_head list;
    int rule_size;
    int addr_size;
    int unresolved_rules;
    int nr_goto_rules;
    unsigned int fib_rules_seq;
    int (*action)(struct fib_rule *, struct flowi *, int, struct fib_lookup_arg *);
    bool (*suppress)(struct fib_rule *, struct fib_lookup_arg *);
    int (*match)(struct fib_rule *, struct flowi *, int);
    int (*configure)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *, struct nlattr **, struct netlink_ext_ack *);
    int (*delete)(struct fib_rule *);
    int (*compare)(struct fib_rule *, struct fib_rule_hdr *, struct nlattr **);
    int (*fill)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *);
    size_t (*nlmsg_payload)(struct fib_rule *);
    void (*flush_cache)(struct fib_rules_ops *);
    int nlgroup;
    const struct nla_policy *policy;
    struct list_head rules_list;
    struct module *owner;
    struct net *fro_net;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct fib_rules_ops {
    int family;
    struct list_head list;
    int rule_size;
    int addr_size;
    int unresolved_rules;
    int nr_goto_rules;
    unsigned int fib_rules_seq;
    int (*action)(struct fib_rule *, struct flowi *, int, struct fib_lookup_arg *);
    bool (*suppress)(struct fib_rule *, struct fib_lookup_arg *);
    int (*match)(struct fib_rule *, struct flowi *, int);
    int (*configure)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *, struct nlattr **, struct netlink_ext_ack *);
    int (*delete)(struct fib_rule *);
    int (*compare)(struct fib_rule *, struct fib_rule_hdr *, struct nlattr **);
    int (*fill)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *);
    size_t (*nlmsg_payload)(struct fib_rule *);
    void (*flush_cache)(struct fib_rules_ops *);
    int nlgroup;
    const struct nla_policy *policy;
    struct list_head rules_list;
    struct module *owner;
    struct net *fro_net;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct fib_rules_ops {
    int family;
    struct list_head list;
    int rule_size;
    int addr_size;
    int unresolved_rules;
    int nr_goto_rules;
    unsigned int fib_rules_seq;
    int (*action)(struct fib_rule *, struct flowi *, int, struct fib_lookup_arg *);
    bool (*suppress)(struct fib_rule *, struct fib_lookup_arg *);
    int (*match)(struct fib_rule *, struct flowi *, int);
    int (*configure)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *, struct nlattr **, struct netlink_ext_ack *);
    int (*delete)(struct fib_rule *);
    int (*compare)(struct fib_rule *, struct fib_rule_hdr *, struct nlattr **);
    int (*fill)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *);
    size_t (*nlmsg_payload)(struct fib_rule *);
    void (*flush_cache)(struct fib_rules_ops *);
    int nlgroup;
    const struct nla_policy *policy;
    struct list_head rules_list;
    struct module *owner;
    struct net *fro_net;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct fib_rules_ops {
    int family;
    struct list_head list;
    int rule_size;
    int addr_size;
    int unresolved_rules;
    int nr_goto_rules;
    unsigned int fib_rules_seq;
    int (*action)(struct fib_rule *, struct flowi *, int, struct fib_lookup_arg *);
    bool (*suppress)(struct fib_rule *, int, struct fib_lookup_arg *);
    int (*match)(struct fib_rule *, struct flowi *, int);
    int (*configure)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *, struct nlattr **, struct netlink_ext_ack *);
    int (*delete)(struct fib_rule *);
    int (*compare)(struct fib_rule *, struct fib_rule_hdr *, struct nlattr **);
    int (*fill)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *);
    size_t (*nlmsg_payload)(struct fib_rule *);
    void (*flush_cache)(struct fib_rules_ops *);
    int nlgroup;
    const struct nla_policy *policy;
    struct list_head rules_list;
    struct module *owner;
    struct net *fro_net;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct fib_rules_ops {
    int family;
    struct list_head list;
    int rule_size;
    int addr_size;
    int unresolved_rules;
    int nr_goto_rules;
    unsigned int fib_rules_seq;
    int (*action)(struct fib_rule *, struct flowi *, int, struct fib_lookup_arg *);
    bool (*suppress)(struct fib_rule *, int, struct fib_lookup_arg *);
    int (*match)(struct fib_rule *, struct flowi *, int);
    int (*configure)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *, struct nlattr **, struct netlink_ext_ack *);
    int (*delete)(struct fib_rule *);
    int (*compare)(struct fib_rule *, struct fib_rule_hdr *, struct nlattr **);
    int (*fill)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *);
    size_t (*nlmsg_payload)(struct fib_rule *);
    void (*flush_cache)(struct fib_rules_ops *);
    int nlgroup;
    struct list_head rules_list;
    struct module *owner;
    struct net *fro_net;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct fib_rules_ops {
    int family;
    struct list_head list;
    int rule_size;
    int addr_size;
    int unresolved_rules;
    int nr_goto_rules;
    unsigned int fib_rules_seq;
    int (*action)(struct fib_rule *, struct flowi *, int, struct fib_lookup_arg *);
    bool (*suppress)(struct fib_rule *, int, struct fib_lookup_arg *);
    int (*match)(struct fib_rule *, struct flowi *, int);
    int (*configure)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *, struct nlattr **, struct netlink_ext_ack *);
    int (*delete)(struct fib_rule *);
    int (*compare)(struct fib_rule *, struct fib_rule_hdr *, struct nlattr **);
    int (*fill)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *);
    size_t (*nlmsg_payload)(struct fib_rule *);
    void (*flush_cache)(struct fib_rules_ops *);
    int nlgroup;
    struct list_head rules_list;
    struct module *owner;
    struct net *fro_net;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct fib_rules_ops {
    int family;
    struct list_head list;
    int rule_size;
    int addr_size;
    int unresolved_rules;
    int nr_goto_rules;
    unsigned int fib_rules_seq;
    int (*action)(struct fib_rule *, struct flowi *, int, struct fib_lookup_arg *);
    bool (*suppress)(struct fib_rule *, int, struct fib_lookup_arg *);
    int (*match)(struct fib_rule *, struct flowi *, int);
    int (*configure)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *, struct nlattr **, struct netlink_ext_ack *);
    int (*delete)(struct fib_rule *);
    int (*compare)(struct fib_rule *, struct fib_rule_hdr *, struct nlattr **);
    int (*fill)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *);
    size_t (*nlmsg_payload)(struct fib_rule *);
    void (*flush_cache)(struct fib_rules_ops *);
    int nlgroup;
    struct list_head rules_list;
    struct module *owner;
    struct net *fro_net;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct fib_rules_ops {
    int family;
    struct list_head list;
    int rule_size;
    int addr_size;
    int unresolved_rules;
    int nr_goto_rules;
    unsigned int fib_rules_seq;
    int (*action)(struct fib_rule *, struct flowi *, int, struct fib_lookup_arg *);
    bool (*suppress)(struct fib_rule *, int, struct fib_lookup_arg *);
    int (*match)(struct fib_rule *, struct flowi *, int);
    int (*configure)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *, struct nlattr **, struct netlink_ext_ack *);
    int (*delete)(struct fib_rule *);
    int (*compare)(struct fib_rule *, struct fib_rule_hdr *, struct nlattr **);
    int (*fill)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *);
    size_t (*nlmsg_payload)(struct fib_rule *);
    void (*flush_cache)(struct fib_rules_ops *);
    int nlgroup;
    struct list_head rules_list;
    struct module *owner;
    struct net *fro_net;
    struct callback_head rcu;
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
struct fib_rules_ops {
    int family;
    struct list_head list;
    int rule_size;
    int addr_size;
    int unresolved_rules;
    int nr_goto_rules;
    unsigned int fib_rules_seq;
    int (*action)(struct fib_rule *, struct flowi *, int, struct fib_lookup_arg *);
    bool (*suppress)(struct fib_rule *, struct fib_lookup_arg *);
    int (*match)(struct fib_rule *, struct flowi *, int);
    int (*configure)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *, struct nlattr **, struct netlink_ext_ack *);
    int (*delete)(struct fib_rule *);
    int (*compare)(struct fib_rule *, struct fib_rule_hdr *, struct nlattr **);
    int (*fill)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *);
    size_t (*nlmsg_payload)(struct fib_rule *);
    void (*flush_cache)(struct fib_rules_ops *);
    int nlgroup;
    const struct nla_policy *policy;
    struct list_head rules_list;
    struct module *owner;
    struct net *fro_net;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct fib_rules_ops {
    int family;
    struct list_head list;
    int rule_size;
    int addr_size;
    int unresolved_rules;
    int nr_goto_rules;
    unsigned int fib_rules_seq;
    int (*action)(struct fib_rule *, struct flowi *, int, struct fib_lookup_arg *);
    bool (*suppress)(struct fib_rule *, struct fib_lookup_arg *);
    int (*match)(struct fib_rule *, struct flowi *, int);
    int (*configure)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *, struct nlattr **, struct netlink_ext_ack *);
    int (*delete)(struct fib_rule *);
    int (*compare)(struct fib_rule *, struct fib_rule_hdr *, struct nlattr **);
    int (*fill)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *);
    size_t (*nlmsg_payload)(struct fib_rule *);
    void (*flush_cache)(struct fib_rules_ops *);
    int nlgroup;
    const struct nla_policy *policy;
    struct list_head rules_list;
    struct module *owner;
    struct net *fro_net;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct fib_rules_ops {
    int family;
    struct list_head list;
    int rule_size;
    int addr_size;
    int unresolved_rules;
    int nr_goto_rules;
    unsigned int fib_rules_seq;
    int (*action)(struct fib_rule *, struct flowi *, int, struct fib_lookup_arg *);
    bool (*suppress)(struct fib_rule *, struct fib_lookup_arg *);
    int (*match)(struct fib_rule *, struct flowi *, int);
    int (*configure)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *, struct nlattr **, struct netlink_ext_ack *);
    int (*delete)(struct fib_rule *);
    int (*compare)(struct fib_rule *, struct fib_rule_hdr *, struct nlattr **);
    int (*fill)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *);
    size_t (*nlmsg_payload)(struct fib_rule *);
    void (*flush_cache)(struct fib_rules_ops *);
    int nlgroup;
    const struct nla_policy *policy;
    struct list_head rules_list;
    struct module *owner;
    struct net *fro_net;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct fib_rules_ops {
    int family;
    struct list_head list;
    int rule_size;
    int addr_size;
    int unresolved_rules;
    int nr_goto_rules;
    unsigned int fib_rules_seq;
    int (*action)(struct fib_rule *, struct flowi *, int, struct fib_lookup_arg *);
    bool (*suppress)(struct fib_rule *, struct fib_lookup_arg *);
    int (*match)(struct fib_rule *, struct flowi *, int);
    int (*configure)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *, struct nlattr **, struct netlink_ext_ack *);
    int (*delete)(struct fib_rule *);
    int (*compare)(struct fib_rule *, struct fib_rule_hdr *, struct nlattr **);
    int (*fill)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *);
    size_t (*nlmsg_payload)(struct fib_rule *);
    void (*flush_cache)(struct fib_rules_ops *);
    int nlgroup;
    const struct nla_policy *policy;
    struct list_head rules_list;
    struct module *owner;
    struct net *fro_net;
    struct callback_head rcu;
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
struct fib_rules_ops {
    int family;
    struct list_head list;
    int rule_size;
    int addr_size;
    int unresolved_rules;
    int nr_goto_rules;
    unsigned int fib_rules_seq;
    int (*action)(struct fib_rule *, struct flowi *, int, struct fib_lookup_arg *);
    bool (*suppress)(struct fib_rule *, struct fib_lookup_arg *);
    int (*match)(struct fib_rule *, struct flowi *, int);
    int (*configure)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *, struct nlattr **, struct netlink_ext_ack *);
    int (*delete)(struct fib_rule *);
    int (*compare)(struct fib_rule *, struct fib_rule_hdr *, struct nlattr **);
    int (*fill)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *);
    size_t (*nlmsg_payload)(struct fib_rule *);
    void (*flush_cache)(struct fib_rules_ops *);
    int nlgroup;
    const struct nla_policy *policy;
    struct list_head rules_list;
    struct module *owner;
    struct net *fro_net;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct fib_rules_ops {
    int family;
    struct list_head list;
    int rule_size;
    int addr_size;
    int unresolved_rules;
    int nr_goto_rules;
    unsigned int fib_rules_seq;
    int (*action)(struct fib_rule *, struct flowi *, int, struct fib_lookup_arg *);
    bool (*suppress)(struct fib_rule *, struct fib_lookup_arg *);
    int (*match)(struct fib_rule *, struct flowi *, int);
    int (*configure)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *, struct nlattr **, struct netlink_ext_ack *);
    int (*delete)(struct fib_rule *);
    int (*compare)(struct fib_rule *, struct fib_rule_hdr *, struct nlattr **);
    int (*fill)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *);
    size_t (*nlmsg_payload)(struct fib_rule *);
    void (*flush_cache)(struct fib_rules_ops *);
    int nlgroup;
    const struct nla_policy *policy;
    struct list_head rules_list;
    struct module *owner;
    struct net *fro_net;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct fib_rules_ops {
    int family;
    struct list_head list;
    int rule_size;
    int addr_size;
    int unresolved_rules;
    int nr_goto_rules;
    unsigned int fib_rules_seq;
    int (*action)(struct fib_rule *, struct flowi *, int, struct fib_lookup_arg *);
    bool (*suppress)(struct fib_rule *, struct fib_lookup_arg *);
    int (*match)(struct fib_rule *, struct flowi *, int);
    int (*configure)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *, struct nlattr **, struct netlink_ext_ack *);
    int (*delete)(struct fib_rule *);
    int (*compare)(struct fib_rule *, struct fib_rule_hdr *, struct nlattr **);
    int (*fill)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *);
    size_t (*nlmsg_payload)(struct fib_rule *);
    void (*flush_cache)(struct fib_rules_ops *);
    int nlgroup;
    const struct nla_policy *policy;
    struct list_head rules_list;
    struct module *owner;
    struct net *fro_net;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct fib_rules_ops {
    int family;
    struct list_head list;
    int rule_size;
    int addr_size;
    int unresolved_rules;
    int nr_goto_rules;
    unsigned int fib_rules_seq;
    int (*action)(struct fib_rule *, struct flowi *, int, struct fib_lookup_arg *);
    bool (*suppress)(struct fib_rule *, struct fib_lookup_arg *);
    int (*match)(struct fib_rule *, struct flowi *, int);
    int (*configure)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *, struct nlattr **, struct netlink_ext_ack *);
    int (*delete)(struct fib_rule *);
    int (*compare)(struct fib_rule *, struct fib_rule_hdr *, struct nlattr **);
    int (*fill)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *);
    size_t (*nlmsg_payload)(struct fib_rule *);
    void (*flush_cache)(struct fib_rules_ops *);
    int nlgroup;
    const struct nla_policy *policy;
    struct list_head rules_list;
    struct module *owner;
    struct net *fro_net;
    struct callback_head rcu;
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
<code>unsigned int fib_rules_seq</code>
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
<code>int (*configure)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *, struct nlattr **)</code> ➡️ <code>int (*configure)(struct fib_rule *, struct sk_buff *, struct fib_rule_hdr *, struct nlattr **, struct netlink_ext_ack *)</code>
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
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>bool (*suppress)(struct fib_rule *, struct fib_lookup_arg *)</code> ➡️ <code>bool (*suppress)(struct fib_rule *, int, struct fib_lookup_arg *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>const struct nla_policy *policy</code>
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
