# Struct: <code>Qdisc_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct Qdisc_ops {
    struct Qdisc_ops *next;
    const struct Qdisc_class_ops *cl_ops;
    char id[16];
    int priv_size;
    int (*enqueue)(struct sk_buff *, struct Qdisc *);
    struct sk_buff * (*dequeue)(struct Qdisc *);
    struct sk_buff * (*peek)(struct Qdisc *);
    unsigned int (*drop)(struct Qdisc *);
    int (*init)(struct Qdisc *, struct nlattr *);
    void (*reset)(struct Qdisc *);
    void (*destroy)(struct Qdisc *);
    int (*change)(struct Qdisc *, struct nlattr *);
    void (*attach)(struct Qdisc *);
    int (*dump)(struct Qdisc *, struct sk_buff *);
    int (*dump_stats)(struct Qdisc *, struct gnet_dump *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct Qdisc_ops {
    struct Qdisc_ops *next;
    const struct Qdisc_class_ops *cl_ops;
    char id[16];
    int priv_size;
    int (*enqueue)(struct sk_buff *, struct Qdisc *, struct sk_buff **);
    struct sk_buff * (*dequeue)(struct Qdisc *);
    struct sk_buff * (*peek)(struct Qdisc *);
    int (*init)(struct Qdisc *, struct nlattr *);
    void (*reset)(struct Qdisc *);
    void (*destroy)(struct Qdisc *);
    int (*change)(struct Qdisc *, struct nlattr *);
    void (*attach)(struct Qdisc *);
    int (*dump)(struct Qdisc *, struct sk_buff *);
    int (*dump_stats)(struct Qdisc *, struct gnet_dump *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct Qdisc_ops {
    struct Qdisc_ops *next;
    const struct Qdisc_class_ops *cl_ops;
    char id[16];
    int priv_size;
    int (*enqueue)(struct sk_buff *, struct Qdisc *, struct sk_buff **);
    struct sk_buff * (*dequeue)(struct Qdisc *);
    struct sk_buff * (*peek)(struct Qdisc *);
    int (*init)(struct Qdisc *, struct nlattr *);
    void (*reset)(struct Qdisc *);
    void (*destroy)(struct Qdisc *);
    int (*change)(struct Qdisc *, struct nlattr *);
    void (*attach)(struct Qdisc *);
    int (*dump)(struct Qdisc *, struct sk_buff *);
    int (*dump_stats)(struct Qdisc *, struct gnet_dump *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct Qdisc_ops {
    struct Qdisc_ops *next;
    const struct Qdisc_class_ops *cl_ops;
    char id[16];
    int priv_size;
    int (*enqueue)(struct sk_buff *, struct Qdisc *, struct sk_buff **);
    struct sk_buff * (*dequeue)(struct Qdisc *);
    struct sk_buff * (*peek)(struct Qdisc *);
    int (*init)(struct Qdisc *, struct nlattr *);
    void (*reset)(struct Qdisc *);
    void (*destroy)(struct Qdisc *);
    int (*change)(struct Qdisc *, struct nlattr *);
    void (*attach)(struct Qdisc *);
    int (*dump)(struct Qdisc *, struct sk_buff *);
    int (*dump_stats)(struct Qdisc *, struct gnet_dump *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct Qdisc_ops {
    struct Qdisc_ops *next;
    const struct Qdisc_class_ops *cl_ops;
    char id[16];
    int priv_size;
    unsigned int static_flags;
    int (*enqueue)(struct sk_buff *, struct Qdisc *, struct sk_buff **);
    struct sk_buff * (*dequeue)(struct Qdisc *);
    struct sk_buff * (*peek)(struct Qdisc *);
    int (*init)(struct Qdisc *, struct nlattr *);
    void (*reset)(struct Qdisc *);
    void (*destroy)(struct Qdisc *);
    int (*change)(struct Qdisc *, struct nlattr *);
    void (*attach)(struct Qdisc *);
    int (*dump)(struct Qdisc *, struct sk_buff *);
    int (*dump_stats)(struct Qdisc *, struct gnet_dump *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct Qdisc_ops {
    struct Qdisc_ops *next;
    const struct Qdisc_class_ops *cl_ops;
    char id[16];
    int priv_size;
    unsigned int static_flags;
    int (*enqueue)(struct sk_buff *, struct Qdisc *, struct sk_buff **);
    struct sk_buff * (*dequeue)(struct Qdisc *);
    struct sk_buff * (*peek)(struct Qdisc *);
    int (*init)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*reset)(struct Qdisc *);
    void (*destroy)(struct Qdisc *);
    int (*change)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*attach)(struct Qdisc *);
    int (*change_tx_queue_len)(struct Qdisc *, unsigned int);
    int (*dump)(struct Qdisc *, struct sk_buff *);
    int (*dump_stats)(struct Qdisc *, struct gnet_dump *);
    void (*ingress_block_set)(struct Qdisc *, u32);
    void (*egress_block_set)(struct Qdisc *, u32);
    u32 (*ingress_block_get)(struct Qdisc *);
    u32 (*egress_block_get)(struct Qdisc *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct Qdisc_ops {
    struct Qdisc_ops *next;
    const struct Qdisc_class_ops *cl_ops;
    char id[16];
    int priv_size;
    unsigned int static_flags;
    int (*enqueue)(struct sk_buff *, struct Qdisc *, struct sk_buff **);
    struct sk_buff * (*dequeue)(struct Qdisc *);
    struct sk_buff * (*peek)(struct Qdisc *);
    int (*init)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*reset)(struct Qdisc *);
    void (*destroy)(struct Qdisc *);
    int (*change)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*attach)(struct Qdisc *);
    int (*change_tx_queue_len)(struct Qdisc *, unsigned int);
    int (*dump)(struct Qdisc *, struct sk_buff *);
    int (*dump_stats)(struct Qdisc *, struct gnet_dump *);
    void (*ingress_block_set)(struct Qdisc *, u32);
    void (*egress_block_set)(struct Qdisc *, u32);
    u32 (*ingress_block_get)(struct Qdisc *);
    u32 (*egress_block_get)(struct Qdisc *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct Qdisc_ops {
    struct Qdisc_ops *next;
    const struct Qdisc_class_ops *cl_ops;
    char id[16];
    int priv_size;
    unsigned int static_flags;
    int (*enqueue)(struct sk_buff *, struct Qdisc *, struct sk_buff **);
    struct sk_buff * (*dequeue)(struct Qdisc *);
    struct sk_buff * (*peek)(struct Qdisc *);
    int (*init)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*reset)(struct Qdisc *);
    void (*destroy)(struct Qdisc *);
    int (*change)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*attach)(struct Qdisc *);
    int (*change_tx_queue_len)(struct Qdisc *, unsigned int);
    int (*dump)(struct Qdisc *, struct sk_buff *);
    int (*dump_stats)(struct Qdisc *, struct gnet_dump *);
    void (*ingress_block_set)(struct Qdisc *, u32);
    void (*egress_block_set)(struct Qdisc *, u32);
    u32 (*ingress_block_get)(struct Qdisc *);
    u32 (*egress_block_get)(struct Qdisc *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct Qdisc_ops {
    struct Qdisc_ops *next;
    const struct Qdisc_class_ops *cl_ops;
    char id[16];
    int priv_size;
    unsigned int static_flags;
    int (*enqueue)(struct sk_buff *, struct Qdisc *, struct sk_buff **);
    struct sk_buff * (*dequeue)(struct Qdisc *);
    struct sk_buff * (*peek)(struct Qdisc *);
    int (*init)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*reset)(struct Qdisc *);
    void (*destroy)(struct Qdisc *);
    int (*change)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*attach)(struct Qdisc *);
    int (*change_tx_queue_len)(struct Qdisc *, unsigned int);
    int (*dump)(struct Qdisc *, struct sk_buff *);
    int (*dump_stats)(struct Qdisc *, struct gnet_dump *);
    void (*ingress_block_set)(struct Qdisc *, u32);
    void (*egress_block_set)(struct Qdisc *, u32);
    u32 (*ingress_block_get)(struct Qdisc *);
    u32 (*egress_block_get)(struct Qdisc *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct Qdisc_ops {
    struct Qdisc_ops *next;
    const struct Qdisc_class_ops *cl_ops;
    char id[16];
    int priv_size;
    unsigned int static_flags;
    int (*enqueue)(struct sk_buff *, struct Qdisc *, struct sk_buff **);
    struct sk_buff * (*dequeue)(struct Qdisc *);
    struct sk_buff * (*peek)(struct Qdisc *);
    int (*init)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*reset)(struct Qdisc *);
    void (*destroy)(struct Qdisc *);
    int (*change)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*attach)(struct Qdisc *);
    int (*change_tx_queue_len)(struct Qdisc *, unsigned int);
    int (*dump)(struct Qdisc *, struct sk_buff *);
    int (*dump_stats)(struct Qdisc *, struct gnet_dump *);
    void (*ingress_block_set)(struct Qdisc *, u32);
    void (*egress_block_set)(struct Qdisc *, u32);
    u32 (*ingress_block_get)(struct Qdisc *);
    u32 (*egress_block_get)(struct Qdisc *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct Qdisc_ops {
    struct Qdisc_ops *next;
    const struct Qdisc_class_ops *cl_ops;
    char id[16];
    int priv_size;
    unsigned int static_flags;
    int (*enqueue)(struct sk_buff *, struct Qdisc *, struct sk_buff **);
    struct sk_buff * (*dequeue)(struct Qdisc *);
    struct sk_buff * (*peek)(struct Qdisc *);
    int (*init)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*reset)(struct Qdisc *);
    void (*destroy)(struct Qdisc *);
    int (*change)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*attach)(struct Qdisc *);
    int (*change_tx_queue_len)(struct Qdisc *, unsigned int);
    int (*dump)(struct Qdisc *, struct sk_buff *);
    int (*dump_stats)(struct Qdisc *, struct gnet_dump *);
    void (*ingress_block_set)(struct Qdisc *, u32);
    void (*egress_block_set)(struct Qdisc *, u32);
    u32 (*ingress_block_get)(struct Qdisc *);
    u32 (*egress_block_get)(struct Qdisc *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct Qdisc_ops {
    struct Qdisc_ops *next;
    const struct Qdisc_class_ops *cl_ops;
    char id[16];
    int priv_size;
    unsigned int static_flags;
    int (*enqueue)(struct sk_buff *, struct Qdisc *, struct sk_buff **);
    struct sk_buff * (*dequeue)(struct Qdisc *);
    struct sk_buff * (*peek)(struct Qdisc *);
    int (*init)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*reset)(struct Qdisc *);
    void (*destroy)(struct Qdisc *);
    int (*change)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*attach)(struct Qdisc *);
    int (*change_tx_queue_len)(struct Qdisc *, unsigned int);
    int (*dump)(struct Qdisc *, struct sk_buff *);
    int (*dump_stats)(struct Qdisc *, struct gnet_dump *);
    void (*ingress_block_set)(struct Qdisc *, u32);
    void (*egress_block_set)(struct Qdisc *, u32);
    u32 (*ingress_block_get)(struct Qdisc *);
    u32 (*egress_block_get)(struct Qdisc *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct Qdisc_ops {
    struct Qdisc_ops *next;
    const struct Qdisc_class_ops *cl_ops;
    char id[16];
    int priv_size;
    unsigned int static_flags;
    int (*enqueue)(struct sk_buff *, struct Qdisc *, struct sk_buff **);
    struct sk_buff * (*dequeue)(struct Qdisc *);
    struct sk_buff * (*peek)(struct Qdisc *);
    int (*init)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*reset)(struct Qdisc *);
    void (*destroy)(struct Qdisc *);
    int (*change)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*attach)(struct Qdisc *);
    int (*change_tx_queue_len)(struct Qdisc *, unsigned int);
    void (*change_real_num_tx)(struct Qdisc *, unsigned int);
    int (*dump)(struct Qdisc *, struct sk_buff *);
    int (*dump_stats)(struct Qdisc *, struct gnet_dump *);
    void (*ingress_block_set)(struct Qdisc *, u32);
    void (*egress_block_set)(struct Qdisc *, u32);
    u32 (*ingress_block_get)(struct Qdisc *);
    u32 (*egress_block_get)(struct Qdisc *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct Qdisc_ops {
    struct Qdisc_ops *next;
    const struct Qdisc_class_ops *cl_ops;
    char id[16];
    int priv_size;
    unsigned int static_flags;
    int (*enqueue)(struct sk_buff *, struct Qdisc *, struct sk_buff **);
    struct sk_buff * (*dequeue)(struct Qdisc *);
    struct sk_buff * (*peek)(struct Qdisc *);
    int (*init)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*reset)(struct Qdisc *);
    void (*destroy)(struct Qdisc *);
    int (*change)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*attach)(struct Qdisc *);
    int (*change_tx_queue_len)(struct Qdisc *, unsigned int);
    void (*change_real_num_tx)(struct Qdisc *, unsigned int);
    int (*dump)(struct Qdisc *, struct sk_buff *);
    int (*dump_stats)(struct Qdisc *, struct gnet_dump *);
    void (*ingress_block_set)(struct Qdisc *, u32);
    void (*egress_block_set)(struct Qdisc *, u32);
    u32 (*ingress_block_get)(struct Qdisc *);
    u32 (*egress_block_get)(struct Qdisc *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct Qdisc_ops {
    struct Qdisc_ops *next;
    const struct Qdisc_class_ops *cl_ops;
    char id[16];
    int priv_size;
    unsigned int static_flags;
    int (*enqueue)(struct sk_buff *, struct Qdisc *, struct sk_buff **);
    struct sk_buff * (*dequeue)(struct Qdisc *);
    struct sk_buff * (*peek)(struct Qdisc *);
    int (*init)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*reset)(struct Qdisc *);
    void (*destroy)(struct Qdisc *);
    int (*change)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*attach)(struct Qdisc *);
    int (*change_tx_queue_len)(struct Qdisc *, unsigned int);
    void (*change_real_num_tx)(struct Qdisc *, unsigned int);
    int (*dump)(struct Qdisc *, struct sk_buff *);
    int (*dump_stats)(struct Qdisc *, struct gnet_dump *);
    void (*ingress_block_set)(struct Qdisc *, u32);
    void (*egress_block_set)(struct Qdisc *, u32);
    u32 (*ingress_block_get)(struct Qdisc *);
    u32 (*egress_block_get)(struct Qdisc *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct Qdisc_ops {
    struct Qdisc_ops *next;
    const struct Qdisc_class_ops *cl_ops;
    char id[16];
    int priv_size;
    unsigned int static_flags;
    int (*enqueue)(struct sk_buff *, struct Qdisc *, struct sk_buff **);
    struct sk_buff * (*dequeue)(struct Qdisc *);
    struct sk_buff * (*peek)(struct Qdisc *);
    int (*init)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*reset)(struct Qdisc *);
    void (*destroy)(struct Qdisc *);
    int (*change)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*attach)(struct Qdisc *);
    int (*change_tx_queue_len)(struct Qdisc *, unsigned int);
    void (*change_real_num_tx)(struct Qdisc *, unsigned int);
    int (*dump)(struct Qdisc *, struct sk_buff *);
    int (*dump_stats)(struct Qdisc *, struct gnet_dump *);
    void (*ingress_block_set)(struct Qdisc *, u32);
    void (*egress_block_set)(struct Qdisc *, u32);
    u32 (*ingress_block_get)(struct Qdisc *);
    u32 (*egress_block_get)(struct Qdisc *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct Qdisc_ops {
    struct Qdisc_ops *next;
    const struct Qdisc_class_ops *cl_ops;
    char id[16];
    int priv_size;
    unsigned int static_flags;
    int (*enqueue)(struct sk_buff *, struct Qdisc *, struct sk_buff **);
    struct sk_buff * (*dequeue)(struct Qdisc *);
    struct sk_buff * (*peek)(struct Qdisc *);
    int (*init)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*reset)(struct Qdisc *);
    void (*destroy)(struct Qdisc *);
    int (*change)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*attach)(struct Qdisc *);
    int (*change_tx_queue_len)(struct Qdisc *, unsigned int);
    void (*change_real_num_tx)(struct Qdisc *, unsigned int);
    int (*dump)(struct Qdisc *, struct sk_buff *);
    int (*dump_stats)(struct Qdisc *, struct gnet_dump *);
    void (*ingress_block_set)(struct Qdisc *, u32);
    void (*egress_block_set)(struct Qdisc *, u32);
    u32 (*ingress_block_get)(struct Qdisc *);
    u32 (*egress_block_get)(struct Qdisc *);
    struct module *owner;
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
struct Qdisc_ops {
    struct Qdisc_ops *next;
    const struct Qdisc_class_ops *cl_ops;
    char id[16];
    int priv_size;
    unsigned int static_flags;
    int (*enqueue)(struct sk_buff *, struct Qdisc *, struct sk_buff **);
    struct sk_buff * (*dequeue)(struct Qdisc *);
    struct sk_buff * (*peek)(struct Qdisc *);
    int (*init)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*reset)(struct Qdisc *);
    void (*destroy)(struct Qdisc *);
    int (*change)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*attach)(struct Qdisc *);
    int (*change_tx_queue_len)(struct Qdisc *, unsigned int);
    int (*dump)(struct Qdisc *, struct sk_buff *);
    int (*dump_stats)(struct Qdisc *, struct gnet_dump *);
    void (*ingress_block_set)(struct Qdisc *, u32);
    void (*egress_block_set)(struct Qdisc *, u32);
    u32 (*ingress_block_get)(struct Qdisc *);
    u32 (*egress_block_get)(struct Qdisc *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct Qdisc_ops {
    struct Qdisc_ops *next;
    const struct Qdisc_class_ops *cl_ops;
    char id[16];
    int priv_size;
    unsigned int static_flags;
    int (*enqueue)(struct sk_buff *, struct Qdisc *, struct sk_buff **);
    struct sk_buff * (*dequeue)(struct Qdisc *);
    struct sk_buff * (*peek)(struct Qdisc *);
    int (*init)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*reset)(struct Qdisc *);
    void (*destroy)(struct Qdisc *);
    int (*change)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*attach)(struct Qdisc *);
    int (*change_tx_queue_len)(struct Qdisc *, unsigned int);
    int (*dump)(struct Qdisc *, struct sk_buff *);
    int (*dump_stats)(struct Qdisc *, struct gnet_dump *);
    void (*ingress_block_set)(struct Qdisc *, u32);
    void (*egress_block_set)(struct Qdisc *, u32);
    u32 (*ingress_block_get)(struct Qdisc *);
    u32 (*egress_block_get)(struct Qdisc *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct Qdisc_ops {
    struct Qdisc_ops *next;
    const struct Qdisc_class_ops *cl_ops;
    char id[16];
    int priv_size;
    unsigned int static_flags;
    int (*enqueue)(struct sk_buff *, struct Qdisc *, struct sk_buff **);
    struct sk_buff * (*dequeue)(struct Qdisc *);
    struct sk_buff * (*peek)(struct Qdisc *);
    int (*init)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*reset)(struct Qdisc *);
    void (*destroy)(struct Qdisc *);
    int (*change)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*attach)(struct Qdisc *);
    int (*change_tx_queue_len)(struct Qdisc *, unsigned int);
    int (*dump)(struct Qdisc *, struct sk_buff *);
    int (*dump_stats)(struct Qdisc *, struct gnet_dump *);
    void (*ingress_block_set)(struct Qdisc *, u32);
    void (*egress_block_set)(struct Qdisc *, u32);
    u32 (*ingress_block_get)(struct Qdisc *);
    u32 (*egress_block_get)(struct Qdisc *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct Qdisc_ops {
    struct Qdisc_ops *next;
    const struct Qdisc_class_ops *cl_ops;
    char id[16];
    int priv_size;
    unsigned int static_flags;
    int (*enqueue)(struct sk_buff *, struct Qdisc *, struct sk_buff **);
    struct sk_buff * (*dequeue)(struct Qdisc *);
    struct sk_buff * (*peek)(struct Qdisc *);
    int (*init)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*reset)(struct Qdisc *);
    void (*destroy)(struct Qdisc *);
    int (*change)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*attach)(struct Qdisc *);
    int (*change_tx_queue_len)(struct Qdisc *, unsigned int);
    int (*dump)(struct Qdisc *, struct sk_buff *);
    int (*dump_stats)(struct Qdisc *, struct gnet_dump *);
    void (*ingress_block_set)(struct Qdisc *, u32);
    void (*egress_block_set)(struct Qdisc *, u32);
    u32 (*ingress_block_get)(struct Qdisc *);
    u32 (*egress_block_get)(struct Qdisc *);
    struct module *owner;
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
struct Qdisc_ops {
    struct Qdisc_ops *next;
    const struct Qdisc_class_ops *cl_ops;
    char id[16];
    int priv_size;
    unsigned int static_flags;
    int (*enqueue)(struct sk_buff *, struct Qdisc *, struct sk_buff **);
    struct sk_buff * (*dequeue)(struct Qdisc *);
    struct sk_buff * (*peek)(struct Qdisc *);
    int (*init)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*reset)(struct Qdisc *);
    void (*destroy)(struct Qdisc *);
    int (*change)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*attach)(struct Qdisc *);
    int (*change_tx_queue_len)(struct Qdisc *, unsigned int);
    int (*dump)(struct Qdisc *, struct sk_buff *);
    int (*dump_stats)(struct Qdisc *, struct gnet_dump *);
    void (*ingress_block_set)(struct Qdisc *, u32);
    void (*egress_block_set)(struct Qdisc *, u32);
    u32 (*ingress_block_get)(struct Qdisc *);
    u32 (*egress_block_get)(struct Qdisc *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct Qdisc_ops {
    struct Qdisc_ops *next;
    const struct Qdisc_class_ops *cl_ops;
    char id[16];
    int priv_size;
    unsigned int static_flags;
    int (*enqueue)(struct sk_buff *, struct Qdisc *, struct sk_buff **);
    struct sk_buff * (*dequeue)(struct Qdisc *);
    struct sk_buff * (*peek)(struct Qdisc *);
    int (*init)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*reset)(struct Qdisc *);
    void (*destroy)(struct Qdisc *);
    int (*change)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*attach)(struct Qdisc *);
    int (*change_tx_queue_len)(struct Qdisc *, unsigned int);
    int (*dump)(struct Qdisc *, struct sk_buff *);
    int (*dump_stats)(struct Qdisc *, struct gnet_dump *);
    void (*ingress_block_set)(struct Qdisc *, u32);
    void (*egress_block_set)(struct Qdisc *, u32);
    u32 (*ingress_block_get)(struct Qdisc *);
    u32 (*egress_block_get)(struct Qdisc *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct Qdisc_ops {
    struct Qdisc_ops *next;
    const struct Qdisc_class_ops *cl_ops;
    char id[16];
    int priv_size;
    unsigned int static_flags;
    int (*enqueue)(struct sk_buff *, struct Qdisc *, struct sk_buff **);
    struct sk_buff * (*dequeue)(struct Qdisc *);
    struct sk_buff * (*peek)(struct Qdisc *);
    int (*init)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*reset)(struct Qdisc *);
    void (*destroy)(struct Qdisc *);
    int (*change)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*attach)(struct Qdisc *);
    int (*change_tx_queue_len)(struct Qdisc *, unsigned int);
    int (*dump)(struct Qdisc *, struct sk_buff *);
    int (*dump_stats)(struct Qdisc *, struct gnet_dump *);
    void (*ingress_block_set)(struct Qdisc *, u32);
    void (*egress_block_set)(struct Qdisc *, u32);
    u32 (*ingress_block_get)(struct Qdisc *);
    u32 (*egress_block_get)(struct Qdisc *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct Qdisc_ops {
    struct Qdisc_ops *next;
    const struct Qdisc_class_ops *cl_ops;
    char id[16];
    int priv_size;
    unsigned int static_flags;
    int (*enqueue)(struct sk_buff *, struct Qdisc *, struct sk_buff **);
    struct sk_buff * (*dequeue)(struct Qdisc *);
    struct sk_buff * (*peek)(struct Qdisc *);
    int (*init)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*reset)(struct Qdisc *);
    void (*destroy)(struct Qdisc *);
    int (*change)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *);
    void (*attach)(struct Qdisc *);
    int (*change_tx_queue_len)(struct Qdisc *, unsigned int);
    int (*dump)(struct Qdisc *, struct sk_buff *);
    int (*dump_stats)(struct Qdisc *, struct gnet_dump *);
    void (*ingress_block_set)(struct Qdisc *, u32);
    void (*egress_block_set)(struct Qdisc *, u32);
    u32 (*ingress_block_get)(struct Qdisc *);
    u32 (*egress_block_get)(struct Qdisc *);
    struct module *owner;
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
<b>Field removed. </b>
<code>unsigned int (*drop)(struct Qdisc *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*enqueue)(struct sk_buff *, struct Qdisc *)</code> ➡️ <code>int (*enqueue)(struct sk_buff *, struct Qdisc *, struct sk_buff **)</code>
</li>
</ul>
</details>
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
<code>unsigned int static_flags</code>
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
<code>int (*change_tx_queue_len)(struct Qdisc *, unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*ingress_block_set)(struct Qdisc *, u32)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*egress_block_set)(struct Qdisc *, u32)</code>
</li>
<li>
<b>Field added. </b>
<code>u32 (*ingress_block_get)(struct Qdisc *)</code>
</li>
<li>
<b>Field added. </b>
<code>u32 (*egress_block_get)(struct Qdisc *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*init)(struct Qdisc *, struct nlattr *)</code> ➡️ <code>int (*init)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*change)(struct Qdisc *, struct nlattr *)</code> ➡️ <code>int (*change)(struct Qdisc *, struct nlattr *, struct netlink_ext_ack *)</code>
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
<b>Field added. </b>
<code>void (*change_real_num_tx)(struct Qdisc *, unsigned int)</code>
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
