# Struct: <code>tc_action_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct tc_action_ops {
    struct list_head head;
    struct tcf_hashinfo *hinfo;
    char kind[16];
    __u32 type;
    struct module *owner;
    int (*act)(struct sk_buff *, const struct tc_action *, struct tcf_result *);
    int (*dump)(struct sk_buff *, struct tc_action *, int, int);
    void (*cleanup)(struct tc_action *, int);
    int (*lookup)(struct tc_action *, u32);
    int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action *, int, int);
    int (*walk)(struct sk_buff *, struct netlink_callback *, int, struct tc_action *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct tc_action_ops {
    struct list_head head;
    char kind[16];
    __u32 type;
    size_t size;
    struct module *owner;
    int (*act)(struct sk_buff *, const struct tc_action *, struct tcf_result *);
    int (*dump)(struct sk_buff *, struct tc_action *, int, int);
    void (*cleanup)(struct tc_action *, int);
    int (*lookup)(struct net *, struct tc_action **, u32);
    int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int);
    int (*walk)(struct net *, struct sk_buff *, struct netlink_callback *, int, const struct tc_action_ops *);
    void (*stats_update)(struct tc_action *, u64, u32, u64);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct tc_action_ops {
    struct list_head head;
    char kind[16];
    __u32 type;
    size_t size;
    struct module *owner;
    int (*act)(struct sk_buff *, const struct tc_action *, struct tcf_result *);
    int (*dump)(struct sk_buff *, struct tc_action *, int, int);
    void (*cleanup)(struct tc_action *, int);
    int (*lookup)(struct net *, struct tc_action **, u32);
    int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int);
    int (*walk)(struct net *, struct sk_buff *, struct netlink_callback *, int, const struct tc_action_ops *);
    void (*stats_update)(struct tc_action *, u64, u32, u64);
    int (*get_dev)(const struct tc_action *, struct net *, struct net_device **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct tc_action_ops {
    struct list_head head;
    char kind[16];
    __u32 type;
    size_t size;
    struct module *owner;
    int (*act)(struct sk_buff *, const struct tc_action *, struct tcf_result *);
    int (*dump)(struct sk_buff *, struct tc_action *, int, int);
    void (*cleanup)(struct tc_action *, int);
    int (*lookup)(struct net *, struct tc_action **, u32);
    int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int);
    int (*walk)(struct net *, struct sk_buff *, struct netlink_callback *, int, const struct tc_action_ops *);
    void (*stats_update)(struct tc_action *, u64, u32, u64);
    int (*get_dev)(const struct tc_action *, struct net *, struct net_device **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct tc_action_ops {
    struct list_head head;
    char kind[16];
    __u32 type;
    size_t size;
    struct module *owner;
    int (*act)(struct sk_buff *, const struct tc_action *, struct tcf_result *);
    int (*dump)(struct sk_buff *, struct tc_action *, int, int);
    void (*cleanup)(struct tc_action *, int);
    int (*lookup)(struct net *, struct tc_action **, u32);
    int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int);
    int (*walk)(struct net *, struct sk_buff *, struct netlink_callback *, int, const struct tc_action_ops *);
    void (*stats_update)(struct tc_action *, u64, u32, u64);
    struct net_device * (*get_dev)(const struct tc_action *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct tc_action_ops {
    struct list_head head;
    char kind[16];
    __u32 type;
    size_t size;
    struct module *owner;
    int (*act)(struct sk_buff *, const struct tc_action *, struct tcf_result *);
    int (*dump)(struct sk_buff *, struct tc_action *, int, int);
    void (*cleanup)(struct tc_action *);
    int (*lookup)(struct net *, struct tc_action **, u32, struct netlink_ext_ack *);
    int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int, struct netlink_ext_ack *);
    int (*walk)(struct net *, struct sk_buff *, struct netlink_callback *, int, const struct tc_action_ops *, struct netlink_ext_ack *);
    void (*stats_update)(struct tc_action *, u64, u32, u64);
    size_t (*get_fill_size)(const struct tc_action *);
    struct net_device * (*get_dev)(const struct tc_action *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct tc_action_ops {
    struct list_head head;
    char kind[16];
    __u32 type;
    size_t size;
    struct module *owner;
    int (*act)(struct sk_buff *, const struct tc_action *, struct tcf_result *);
    int (*dump)(struct sk_buff *, struct tc_action *, int, int);
    void (*cleanup)(struct tc_action *);
    int (*lookup)(struct net *, struct tc_action **, u32);
    int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int, bool, struct netlink_ext_ack *);
    int (*walk)(struct net *, struct sk_buff *, struct netlink_callback *, int, const struct tc_action_ops *, struct netlink_ext_ack *);
    void (*stats_update)(struct tc_action *, u64, u32, u64, bool);
    size_t (*get_fill_size)(const struct tc_action *);
    struct net_device * (*get_dev)(const struct tc_action *);
    void (*put_dev)(struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct tc_action_ops {
    struct list_head head;
    char kind[16];
    enum tca_id id;
    size_t size;
    struct module *owner;
    int (*act)(struct sk_buff *, const struct tc_action *, struct tcf_result *);
    int (*dump)(struct sk_buff *, struct tc_action *, int, int);
    void (*cleanup)(struct tc_action *);
    int (*lookup)(struct net *, struct tc_action **, u32);
    int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int, bool, struct tcf_proto *, struct netlink_ext_ack *);
    int (*walk)(struct net *, struct sk_buff *, struct netlink_callback *, int, const struct tc_action_ops *, struct netlink_ext_ack *);
    void (*stats_update)(struct tc_action *, u64, u32, u64, bool);
    size_t (*get_fill_size)(const struct tc_action *);
    struct net_device * (*get_dev)(const struct tc_action *);
    void (*put_dev)(struct net_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct tc_action_ops {
    struct list_head head;
    char kind[16];
    enum tca_id id;
    size_t size;
    struct module *owner;
    int (*act)(struct sk_buff *, const struct tc_action *, struct tcf_result *);
    int (*dump)(struct sk_buff *, struct tc_action *, int, int);
    void (*cleanup)(struct tc_action *);
    int (*lookup)(struct net *, struct tc_action **, u32);
    int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int, bool, struct tcf_proto *, struct netlink_ext_ack *);
    int (*walk)(struct net *, struct sk_buff *, struct netlink_callback *, int, const struct tc_action_ops *, struct netlink_ext_ack *);
    void (*stats_update)(struct tc_action *, u64, u32, u64, bool);
    size_t (*get_fill_size)(const struct tc_action *);
    struct net_device * (*get_dev)(const struct tc_action *, tc_action_priv_destructor *);
    struct psample_group * (*get_psample_group)(const struct tc_action *, tc_action_priv_destructor *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct tc_action_ops {
    struct list_head head;
    char kind[16];
    enum tca_id id;
    size_t size;
    struct module *owner;
    int (*act)(struct sk_buff *, const struct tc_action *, struct tcf_result *);
    int (*dump)(struct sk_buff *, struct tc_action *, int, int);
    void (*cleanup)(struct tc_action *);
    int (*lookup)(struct net *, struct tc_action **, u32);
    int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int, bool, struct tcf_proto *, u32, struct netlink_ext_ack *);
    int (*walk)(struct net *, struct sk_buff *, struct netlink_callback *, int, const struct tc_action_ops *, struct netlink_ext_ack *);
    void (*stats_update)(struct tc_action *, u64, u32, u64, bool);
    size_t (*get_fill_size)(const struct tc_action *);
    struct net_device * (*get_dev)(const struct tc_action *, tc_action_priv_destructor *);
    struct psample_group * (*get_psample_group)(const struct tc_action *, tc_action_priv_destructor *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct tc_action_ops {
    struct list_head head;
    char kind[16];
    enum tca_id id;
    size_t size;
    struct module *owner;
    int (*act)(struct sk_buff *, const struct tc_action *, struct tcf_result *);
    int (*dump)(struct sk_buff *, struct tc_action *, int, int);
    void (*cleanup)(struct tc_action *);
    int (*lookup)(struct net *, struct tc_action **, u32);
    int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int, bool, struct tcf_proto *, u32, struct netlink_ext_ack *);
    int (*walk)(struct net *, struct sk_buff *, struct netlink_callback *, int, const struct tc_action_ops *, struct netlink_ext_ack *);
    void (*stats_update)(struct tc_action *, u64, u64, u64, u64, bool);
    size_t (*get_fill_size)(const struct tc_action *);
    struct net_device * (*get_dev)(const struct tc_action *, tc_action_priv_destructor *);
    struct psample_group * (*get_psample_group)(const struct tc_action *, tc_action_priv_destructor *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct tc_action_ops {
    struct list_head head;
    char kind[16];
    enum tca_id id;
    size_t size;
    struct module *owner;
    int (*act)(struct sk_buff *, const struct tc_action *, struct tcf_result *);
    int (*dump)(struct sk_buff *, struct tc_action *, int, int);
    void (*cleanup)(struct tc_action *);
    int (*lookup)(struct net *, struct tc_action **, u32);
    int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int, bool, struct tcf_proto *, u32, struct netlink_ext_ack *);
    int (*walk)(struct net *, struct sk_buff *, struct netlink_callback *, int, const struct tc_action_ops *, struct netlink_ext_ack *);
    void (*stats_update)(struct tc_action *, u64, u64, u64, u64, bool);
    size_t (*get_fill_size)(const struct tc_action *);
    struct net_device * (*get_dev)(const struct tc_action *, tc_action_priv_destructor *);
    struct psample_group * (*get_psample_group)(const struct tc_action *, tc_action_priv_destructor *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct tc_action_ops {
    struct list_head head;
    char kind[16];
    enum tca_id id;
    size_t size;
    struct module *owner;
    int (*act)(struct sk_buff *, const struct tc_action *, struct tcf_result *);
    int (*dump)(struct sk_buff *, struct tc_action *, int, int);
    void (*cleanup)(struct tc_action *);
    int (*lookup)(struct net *, struct tc_action **, u32);
    int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, struct tcf_proto *, u32, struct netlink_ext_ack *);
    int (*walk)(struct net *, struct sk_buff *, struct netlink_callback *, int, const struct tc_action_ops *, struct netlink_ext_ack *);
    void (*stats_update)(struct tc_action *, u64, u64, u64, u64, bool);
    size_t (*get_fill_size)(const struct tc_action *);
    struct net_device * (*get_dev)(const struct tc_action *, tc_action_priv_destructor *);
    struct psample_group * (*get_psample_group)(const struct tc_action *, tc_action_priv_destructor *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct tc_action_ops {
    struct list_head head;
    char kind[16];
    enum tca_id id;
    size_t size;
    struct module *owner;
    int (*act)(struct sk_buff *, const struct tc_action *, struct tcf_result *);
    int (*dump)(struct sk_buff *, struct tc_action *, int, int);
    void (*cleanup)(struct tc_action *);
    int (*lookup)(struct net *, struct tc_action **, u32);
    int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, struct tcf_proto *, u32, struct netlink_ext_ack *);
    int (*walk)(struct net *, struct sk_buff *, struct netlink_callback *, int, const struct tc_action_ops *, struct netlink_ext_ack *);
    void (*stats_update)(struct tc_action *, u64, u64, u64, u64, bool);
    size_t (*get_fill_size)(const struct tc_action *);
    struct net_device * (*get_dev)(const struct tc_action *, tc_action_priv_destructor *);
    struct psample_group * (*get_psample_group)(const struct tc_action *, tc_action_priv_destructor *);
    int (*offload_act_setup)(struct tc_action *, void *, u32 *, bool, struct netlink_ext_ack *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct tc_action_ops {
    struct list_head head;
    char kind[16];
    enum tca_id id;
    unsigned int net_id;
    size_t size;
    struct module *owner;
    int (*act)(struct sk_buff *, const struct tc_action *, struct tcf_result *);
    int (*dump)(struct sk_buff *, struct tc_action *, int, int);
    void (*cleanup)(struct tc_action *);
    int (*lookup)(struct net *, struct tc_action **, u32);
    int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, struct tcf_proto *, u32, struct netlink_ext_ack *);
    int (*walk)(struct net *, struct sk_buff *, struct netlink_callback *, int, const struct tc_action_ops *, struct netlink_ext_ack *);
    void (*stats_update)(struct tc_action *, u64, u64, u64, u64, bool);
    size_t (*get_fill_size)(const struct tc_action *);
    struct net_device * (*get_dev)(const struct tc_action *, tc_action_priv_destructor *);
    struct psample_group * (*get_psample_group)(const struct tc_action *, tc_action_priv_destructor *);
    int (*offload_act_setup)(struct tc_action *, void *, u32 *, bool, struct netlink_ext_ack *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct tc_action_ops {
    struct list_head head;
    char kind[16];
    enum tca_id id;
    unsigned int net_id;
    size_t size;
    struct module *owner;
    int (*act)(struct sk_buff *, const struct tc_action *, struct tcf_result *);
    int (*dump)(struct sk_buff *, struct tc_action *, int, int);
    void (*cleanup)(struct tc_action *);
    int (*lookup)(struct net *, struct tc_action **, u32);
    int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, struct tcf_proto *, u32, struct netlink_ext_ack *);
    int (*walk)(struct net *, struct sk_buff *, struct netlink_callback *, int, const struct tc_action_ops *, struct netlink_ext_ack *);
    void (*stats_update)(struct tc_action *, u64, u64, u64, u64, bool);
    size_t (*get_fill_size)(const struct tc_action *);
    struct net_device * (*get_dev)(const struct tc_action *, tc_action_priv_destructor *);
    struct psample_group * (*get_psample_group)(const struct tc_action *, tc_action_priv_destructor *);
    int (*offload_act_setup)(struct tc_action *, void *, u32 *, bool, struct netlink_ext_ack *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct tc_action_ops {
    struct list_head head;
    char kind[16];
    enum tca_id id;
    unsigned int net_id;
    size_t size;
    struct module *owner;
    int (*act)(struct sk_buff *, const struct tc_action *, struct tcf_result *);
    int (*dump)(struct sk_buff *, struct tc_action *, int, int);
    void (*cleanup)(struct tc_action *);
    int (*lookup)(struct net *, struct tc_action **, u32);
    int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, struct tcf_proto *, u32, struct netlink_ext_ack *);
    int (*walk)(struct net *, struct sk_buff *, struct netlink_callback *, int, const struct tc_action_ops *, struct netlink_ext_ack *);
    void (*stats_update)(struct tc_action *, u64, u64, u64, u64, bool);
    size_t (*get_fill_size)(const struct tc_action *);
    struct net_device * (*get_dev)(const struct tc_action *, tc_action_priv_destructor *);
    struct psample_group * (*get_psample_group)(const struct tc_action *, tc_action_priv_destructor *);
    int (*offload_act_setup)(struct tc_action *, void *, u32 *, bool, struct netlink_ext_ack *);
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
struct tc_action_ops {
    struct list_head head;
    char kind[16];
    enum tca_id id;
    size_t size;
    struct module *owner;
    int (*act)(struct sk_buff *, const struct tc_action *, struct tcf_result *);
    int (*dump)(struct sk_buff *, struct tc_action *, int, int);
    void (*cleanup)(struct tc_action *);
    int (*lookup)(struct net *, struct tc_action **, u32);
    int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int, bool, struct tcf_proto *, struct netlink_ext_ack *);
    int (*walk)(struct net *, struct sk_buff *, struct netlink_callback *, int, const struct tc_action_ops *, struct netlink_ext_ack *);
    void (*stats_update)(struct tc_action *, u64, u32, u64, bool);
    size_t (*get_fill_size)(const struct tc_action *);
    struct net_device * (*get_dev)(const struct tc_action *, tc_action_priv_destructor *);
    struct psample_group * (*get_psample_group)(const struct tc_action *, tc_action_priv_destructor *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct tc_action_ops {
    struct list_head head;
    char kind[16];
    enum tca_id id;
    size_t size;
    struct module *owner;
    int (*act)(struct sk_buff *, const struct tc_action *, struct tcf_result *);
    int (*dump)(struct sk_buff *, struct tc_action *, int, int);
    void (*cleanup)(struct tc_action *);
    int (*lookup)(struct net *, struct tc_action **, u32);
    int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int, bool, struct tcf_proto *, struct netlink_ext_ack *);
    int (*walk)(struct net *, struct sk_buff *, struct netlink_callback *, int, const struct tc_action_ops *, struct netlink_ext_ack *);
    void (*stats_update)(struct tc_action *, u64, u32, u64, bool);
    size_t (*get_fill_size)(const struct tc_action *);
    struct net_device * (*get_dev)(const struct tc_action *, tc_action_priv_destructor *);
    struct psample_group * (*get_psample_group)(const struct tc_action *, tc_action_priv_destructor *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct tc_action_ops {
    struct list_head head;
    char kind[16];
    enum tca_id id;
    size_t size;
    struct module *owner;
    int (*act)(struct sk_buff *, const struct tc_action *, struct tcf_result *);
    int (*dump)(struct sk_buff *, struct tc_action *, int, int);
    void (*cleanup)(struct tc_action *);
    int (*lookup)(struct net *, struct tc_action **, u32);
    int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int, bool, struct tcf_proto *, struct netlink_ext_ack *);
    int (*walk)(struct net *, struct sk_buff *, struct netlink_callback *, int, const struct tc_action_ops *, struct netlink_ext_ack *);
    void (*stats_update)(struct tc_action *, u64, u32, u64, bool);
    size_t (*get_fill_size)(const struct tc_action *);
    struct net_device * (*get_dev)(const struct tc_action *, tc_action_priv_destructor *);
    struct psample_group * (*get_psample_group)(const struct tc_action *, tc_action_priv_destructor *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct tc_action_ops {
    struct list_head head;
    char kind[16];
    enum tca_id id;
    size_t size;
    struct module *owner;
    int (*act)(struct sk_buff *, const struct tc_action *, struct tcf_result *);
    int (*dump)(struct sk_buff *, struct tc_action *, int, int);
    void (*cleanup)(struct tc_action *);
    int (*lookup)(struct net *, struct tc_action **, u32);
    int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int, bool, struct tcf_proto *, struct netlink_ext_ack *);
    int (*walk)(struct net *, struct sk_buff *, struct netlink_callback *, int, const struct tc_action_ops *, struct netlink_ext_ack *);
    void (*stats_update)(struct tc_action *, u64, u32, u64, bool);
    size_t (*get_fill_size)(const struct tc_action *);
    struct net_device * (*get_dev)(const struct tc_action *, tc_action_priv_destructor *);
    struct psample_group * (*get_psample_group)(const struct tc_action *, tc_action_priv_destructor *);
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
struct tc_action_ops {
    struct list_head head;
    char kind[16];
    enum tca_id id;
    size_t size;
    struct module *owner;
    int (*act)(struct sk_buff *, const struct tc_action *, struct tcf_result *);
    int (*dump)(struct sk_buff *, struct tc_action *, int, int);
    void (*cleanup)(struct tc_action *);
    int (*lookup)(struct net *, struct tc_action **, u32);
    int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int, bool, struct tcf_proto *, struct netlink_ext_ack *);
    int (*walk)(struct net *, struct sk_buff *, struct netlink_callback *, int, const struct tc_action_ops *, struct netlink_ext_ack *);
    void (*stats_update)(struct tc_action *, u64, u32, u64, bool);
    size_t (*get_fill_size)(const struct tc_action *);
    struct net_device * (*get_dev)(const struct tc_action *, tc_action_priv_destructor *);
    struct psample_group * (*get_psample_group)(const struct tc_action *, tc_action_priv_destructor *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct tc_action_ops {
    struct list_head head;
    char kind[16];
    enum tca_id id;
    size_t size;
    struct module *owner;
    int (*act)(struct sk_buff *, const struct tc_action *, struct tcf_result *);
    int (*dump)(struct sk_buff *, struct tc_action *, int, int);
    void (*cleanup)(struct tc_action *);
    int (*lookup)(struct net *, struct tc_action **, u32);
    int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int, bool, struct tcf_proto *, struct netlink_ext_ack *);
    int (*walk)(struct net *, struct sk_buff *, struct netlink_callback *, int, const struct tc_action_ops *, struct netlink_ext_ack *);
    void (*stats_update)(struct tc_action *, u64, u32, u64, bool);
    size_t (*get_fill_size)(const struct tc_action *);
    struct net_device * (*get_dev)(const struct tc_action *, tc_action_priv_destructor *);
    struct psample_group * (*get_psample_group)(const struct tc_action *, tc_action_priv_destructor *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct tc_action_ops {
    struct list_head head;
    char kind[16];
    enum tca_id id;
    size_t size;
    struct module *owner;
    int (*act)(struct sk_buff *, const struct tc_action *, struct tcf_result *);
    int (*dump)(struct sk_buff *, struct tc_action *, int, int);
    void (*cleanup)(struct tc_action *);
    int (*lookup)(struct net *, struct tc_action **, u32);
    int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int, bool, struct tcf_proto *, struct netlink_ext_ack *);
    int (*walk)(struct net *, struct sk_buff *, struct netlink_callback *, int, const struct tc_action_ops *, struct netlink_ext_ack *);
    void (*stats_update)(struct tc_action *, u64, u32, u64, bool);
    size_t (*get_fill_size)(const struct tc_action *);
    struct net_device * (*get_dev)(const struct tc_action *, tc_action_priv_destructor *);
    struct psample_group * (*get_psample_group)(const struct tc_action *, tc_action_priv_destructor *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct tc_action_ops {
    struct list_head head;
    char kind[16];
    enum tca_id id;
    size_t size;
    struct module *owner;
    int (*act)(struct sk_buff *, const struct tc_action *, struct tcf_result *);
    int (*dump)(struct sk_buff *, struct tc_action *, int, int);
    void (*cleanup)(struct tc_action *);
    int (*lookup)(struct net *, struct tc_action **, u32);
    int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int, bool, struct tcf_proto *, struct netlink_ext_ack *);
    int (*walk)(struct net *, struct sk_buff *, struct netlink_callback *, int, const struct tc_action_ops *, struct netlink_ext_ack *);
    void (*stats_update)(struct tc_action *, u64, u32, u64, bool);
    size_t (*get_fill_size)(const struct tc_action *);
    struct net_device * (*get_dev)(const struct tc_action *, tc_action_priv_destructor *);
    struct psample_group * (*get_psample_group)(const struct tc_action *, tc_action_priv_destructor *);
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
<code>size_t size</code>
</li>
<li>
<b>Field added. </b>
<code>void (*stats_update)(struct tc_action *, u64, u32, u64)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct tcf_hashinfo *hinfo</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*lookup)(struct tc_action *, u32)</code> ➡️ <code>int (*lookup)(struct net *, struct tc_action **, u32)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action *, int, int)</code> ➡️ <code>int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*walk)(struct sk_buff *, struct netlink_callback *, int, struct tc_action *)</code> ➡️ <code>int (*walk)(struct net *, struct sk_buff *, struct netlink_callback *, int, const struct tc_action_ops *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*get_dev)(const struct tc_action *, struct net *, struct net_device **)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*get_dev)(const struct tc_action *, struct net *, struct net_device **)</code> ➡️ <code>struct net_device * (*get_dev)(const struct tc_action *)</code>
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
<code>size_t (*get_fill_size)(const struct tc_action *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*cleanup)(struct tc_action *, int)</code> ➡️ <code>void (*cleanup)(struct tc_action *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*lookup)(struct net *, struct tc_action **, u32)</code> ➡️ <code>int (*lookup)(struct net *, struct tc_action **, u32, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int)</code> ➡️ <code>int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*walk)(struct net *, struct sk_buff *, struct netlink_callback *, int, const struct tc_action_ops *)</code> ➡️ <code>int (*walk)(struct net *, struct sk_buff *, struct netlink_callback *, int, const struct tc_action_ops *, struct netlink_ext_ack *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*put_dev)(struct net_device *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*lookup)(struct net *, struct tc_action **, u32, struct netlink_ext_ack *)</code> ➡️ <code>int (*lookup)(struct net *, struct tc_action **, u32)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int, struct netlink_ext_ack *)</code> ➡️ <code>int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int, bool, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*stats_update)(struct tc_action *, u64, u32, u64)</code> ➡️ <code>void (*stats_update)(struct tc_action *, u64, u32, u64, bool)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>enum tca_id id</code>
</li>
<li>
<b>Field removed. </b>
<code>__u32 type</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int, bool, struct netlink_ext_ack *)</code> ➡️ <code>int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int, bool, struct tcf_proto *, struct netlink_ext_ack *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct psample_group * (*get_psample_group)(const struct tc_action *, tc_action_priv_destructor *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*put_dev)(struct net_device *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct net_device * (*get_dev)(const struct tc_action *)</code> ➡️ <code>struct net_device * (*get_dev)(const struct tc_action *, tc_action_priv_destructor *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int, bool, struct tcf_proto *, struct netlink_ext_ack *)</code> ➡️ <code>int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int, bool, struct tcf_proto *, u32, struct netlink_ext_ack *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>void (*stats_update)(struct tc_action *, u64, u32, u64, bool)</code> ➡️ <code>void (*stats_update)(struct tc_action *, u64, u64, u64, u64, bool)</code>
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
<b>Field type changed. </b>
<code>int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, int, int, bool, struct tcf_proto *, u32, struct netlink_ext_ack *)</code> ➡️ <code>int (*init)(struct net *, struct nlattr *, struct nlattr *, struct tc_action **, struct tcf_proto *, u32, struct netlink_ext_ack *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*offload_act_setup)(struct tc_action *, void *, u32 *, bool, struct netlink_ext_ack *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int net_id</code>
</li>
</ul>
</details>
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
