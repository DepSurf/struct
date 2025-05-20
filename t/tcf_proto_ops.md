# Struct: <code>tcf_proto_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct tcf_proto_ops {
    struct list_head head;
    char kind[16];
    int (*classify)(struct sk_buff *, const struct tcf_proto *, struct tcf_result *);
    int (*init)(struct tcf_proto *);
    bool (*destroy)(struct tcf_proto *, bool);
    long unsigned int (*get)(struct tcf_proto *, u32);
    int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, long unsigned int *, bool);
    int (*delete)(struct tcf_proto *, long unsigned int);
    void (*walk)(struct tcf_proto *, struct tcf_walker *);
    int (*dump)(struct net *, struct tcf_proto *, long unsigned int, struct sk_buff *, struct tcmsg *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct tcf_proto_ops {
    struct list_head head;
    char kind[16];
    int (*classify)(struct sk_buff *, const struct tcf_proto *, struct tcf_result *);
    int (*init)(struct tcf_proto *);
    bool (*destroy)(struct tcf_proto *, bool);
    long unsigned int (*get)(struct tcf_proto *, u32);
    int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, long unsigned int *, bool);
    int (*delete)(struct tcf_proto *, long unsigned int);
    void (*walk)(struct tcf_proto *, struct tcf_walker *);
    int (*dump)(struct net *, struct tcf_proto *, long unsigned int, struct sk_buff *, struct tcmsg *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct tcf_proto_ops {
    struct list_head head;
    char kind[16];
    int (*classify)(struct sk_buff *, const struct tcf_proto *, struct tcf_result *);
    int (*init)(struct tcf_proto *);
    bool (*destroy)(struct tcf_proto *, bool);
    long unsigned int (*get)(struct tcf_proto *, u32);
    int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, long unsigned int *, bool);
    int (*delete)(struct tcf_proto *, long unsigned int);
    void (*walk)(struct tcf_proto *, struct tcf_walker *);
    int (*dump)(struct net *, struct tcf_proto *, long unsigned int, struct sk_buff *, struct tcmsg *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct tcf_proto_ops {
    struct list_head head;
    char kind[16];
    int (*classify)(struct sk_buff *, const struct tcf_proto *, struct tcf_result *);
    int (*init)(struct tcf_proto *);
    void (*destroy)(struct tcf_proto *);
    long unsigned int (*get)(struct tcf_proto *, u32);
    int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, long unsigned int *, bool);
    int (*delete)(struct tcf_proto *, long unsigned int, bool *);
    void (*walk)(struct tcf_proto *, struct tcf_walker *);
    int (*dump)(struct net *, struct tcf_proto *, long unsigned int, struct sk_buff *, struct tcmsg *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct tcf_proto_ops {
    struct list_head head;
    char kind[16];
    int (*classify)(struct sk_buff *, const struct tcf_proto *, struct tcf_result *);
    int (*init)(struct tcf_proto *);
    void (*destroy)(struct tcf_proto *);
    void * (*get)(struct tcf_proto *, u32);
    int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, bool);
    int (*delete)(struct tcf_proto *, void *, bool *);
    void (*walk)(struct tcf_proto *, struct tcf_walker *);
    void (*bind_class)(void *, u32, long unsigned int);
    int (*dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct tcf_proto_ops {
    struct list_head head;
    char kind[16];
    int (*classify)(struct sk_buff *, const struct tcf_proto *, struct tcf_result *);
    int (*init)(struct tcf_proto *);
    void (*destroy)(struct tcf_proto *, struct netlink_ext_ack *);
    void * (*get)(struct tcf_proto *, u32);
    int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, bool, struct netlink_ext_ack *);
    int (*delete)(struct tcf_proto *, void *, bool *, struct netlink_ext_ack *);
    void (*walk)(struct tcf_proto *, struct tcf_walker *);
    void (*bind_class)(void *, u32, long unsigned int);
    int (*dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct tcf_proto_ops {
    struct list_head head;
    char kind[16];
    int (*classify)(struct sk_buff *, const struct tcf_proto *, struct tcf_result *);
    int (*init)(struct tcf_proto *);
    void (*destroy)(struct tcf_proto *, struct netlink_ext_ack *);
    void * (*get)(struct tcf_proto *, u32);
    int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, bool, struct netlink_ext_ack *);
    int (*delete)(struct tcf_proto *, void *, bool *, struct netlink_ext_ack *);
    void (*walk)(struct tcf_proto *, struct tcf_walker *);
    int (*reoffload)(struct tcf_proto *, bool, tc_setup_cb_t *, void *, struct netlink_ext_ack *);
    void (*bind_class)(void *, u32, long unsigned int);
    void * (*tmplt_create)(struct net *, struct tcf_chain *, struct nlattr **, struct netlink_ext_ack *);
    void (*tmplt_destroy)(void *);
    int (*dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *);
    int (*tmplt_dump)(struct sk_buff *, struct net *, void *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct tcf_proto_ops {
    struct list_head head;
    char kind[16];
    int (*classify)(struct sk_buff *, const struct tcf_proto *, struct tcf_result *);
    int (*init)(struct tcf_proto *);
    void (*destroy)(struct tcf_proto *, bool, struct netlink_ext_ack *);
    void * (*get)(struct tcf_proto *, u32);
    void (*put)(struct tcf_proto *, void *);
    int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, bool, bool, struct netlink_ext_ack *);
    int (*delete)(struct tcf_proto *, void *, bool *, bool, struct netlink_ext_ack *);
    void (*walk)(struct tcf_proto *, struct tcf_walker *, bool);
    int (*reoffload)(struct tcf_proto *, bool, flow_setup_cb_t *, void *, struct netlink_ext_ack *);
    void (*bind_class)(void *, u32, long unsigned int);
    void * (*tmplt_create)(struct net *, struct tcf_chain *, struct nlattr **, struct netlink_ext_ack *);
    void (*tmplt_destroy)(void *);
    int (*dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool);
    int (*tmplt_dump)(struct sk_buff *, struct net *, void *);
    struct module *owner;
    int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct tcf_proto_ops {
    struct list_head head;
    char kind[16];
    int (*classify)(struct sk_buff *, const struct tcf_proto *, struct tcf_result *);
    int (*init)(struct tcf_proto *);
    void (*destroy)(struct tcf_proto *, bool, struct netlink_ext_ack *);
    void * (*get)(struct tcf_proto *, u32);
    void (*put)(struct tcf_proto *, void *);
    int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, bool, bool, struct netlink_ext_ack *);
    int (*delete)(struct tcf_proto *, void *, bool *, bool, struct netlink_ext_ack *);
    bool (*delete_empty)(struct tcf_proto *);
    void (*walk)(struct tcf_proto *, struct tcf_walker *, bool);
    int (*reoffload)(struct tcf_proto *, bool, flow_setup_cb_t *, void *, struct netlink_ext_ack *);
    void (*hw_add)(struct tcf_proto *, void *);
    void (*hw_del)(struct tcf_proto *, void *);
    void (*bind_class)(void *, u32, long unsigned int, void *, long unsigned int);
    void * (*tmplt_create)(struct net *, struct tcf_chain *, struct nlattr **, struct netlink_ext_ack *);
    void (*tmplt_destroy)(void *);
    int (*dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool);
    int (*tmplt_dump)(struct sk_buff *, struct net *, void *);
    struct module *owner;
    int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct tcf_proto_ops {
    struct list_head head;
    char kind[16];
    int (*classify)(struct sk_buff *, const struct tcf_proto *, struct tcf_result *);
    int (*init)(struct tcf_proto *);
    void (*destroy)(struct tcf_proto *, bool, struct netlink_ext_ack *);
    void * (*get)(struct tcf_proto *, u32);
    void (*put)(struct tcf_proto *, void *);
    int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, bool, bool, struct netlink_ext_ack *);
    int (*delete)(struct tcf_proto *, void *, bool *, bool, struct netlink_ext_ack *);
    bool (*delete_empty)(struct tcf_proto *);
    void (*walk)(struct tcf_proto *, struct tcf_walker *, bool);
    int (*reoffload)(struct tcf_proto *, bool, flow_setup_cb_t *, void *, struct netlink_ext_ack *);
    void (*hw_add)(struct tcf_proto *, void *);
    void (*hw_del)(struct tcf_proto *, void *);
    void (*bind_class)(void *, u32, long unsigned int, void *, long unsigned int);
    void * (*tmplt_create)(struct net *, struct tcf_chain *, struct nlattr **, struct netlink_ext_ack *);
    void (*tmplt_destroy)(void *);
    int (*dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool);
    int (*terse_dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool);
    int (*tmplt_dump)(struct sk_buff *, struct net *, void *);
    struct module *owner;
    int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct tcf_proto_ops {
    struct list_head head;
    char kind[16];
    int (*classify)(struct sk_buff *, const struct tcf_proto *, struct tcf_result *);
    int (*init)(struct tcf_proto *);
    void (*destroy)(struct tcf_proto *, bool, struct netlink_ext_ack *);
    void * (*get)(struct tcf_proto *, u32);
    void (*put)(struct tcf_proto *, void *);
    int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, bool, bool, struct netlink_ext_ack *);
    int (*delete)(struct tcf_proto *, void *, bool *, bool, struct netlink_ext_ack *);
    bool (*delete_empty)(struct tcf_proto *);
    void (*walk)(struct tcf_proto *, struct tcf_walker *, bool);
    int (*reoffload)(struct tcf_proto *, bool, flow_setup_cb_t *, void *, struct netlink_ext_ack *);
    void (*hw_add)(struct tcf_proto *, void *);
    void (*hw_del)(struct tcf_proto *, void *);
    void (*bind_class)(void *, u32, long unsigned int, void *, long unsigned int);
    void * (*tmplt_create)(struct net *, struct tcf_chain *, struct nlattr **, struct netlink_ext_ack *);
    void (*tmplt_destroy)(void *);
    int (*dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool);
    int (*terse_dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool);
    int (*tmplt_dump)(struct sk_buff *, struct net *, void *);
    struct module *owner;
    int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct tcf_proto_ops {
    struct list_head head;
    char kind[16];
    int (*classify)(struct sk_buff *, const struct tcf_proto *, struct tcf_result *);
    int (*init)(struct tcf_proto *);
    void (*destroy)(struct tcf_proto *, bool, struct netlink_ext_ack *);
    void * (*get)(struct tcf_proto *, u32);
    void (*put)(struct tcf_proto *, void *);
    int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, bool, bool, struct netlink_ext_ack *);
    int (*delete)(struct tcf_proto *, void *, bool *, bool, struct netlink_ext_ack *);
    bool (*delete_empty)(struct tcf_proto *);
    void (*walk)(struct tcf_proto *, struct tcf_walker *, bool);
    int (*reoffload)(struct tcf_proto *, bool, flow_setup_cb_t *, void *, struct netlink_ext_ack *);
    void (*hw_add)(struct tcf_proto *, void *);
    void (*hw_del)(struct tcf_proto *, void *);
    void (*bind_class)(void *, u32, long unsigned int, void *, long unsigned int);
    void * (*tmplt_create)(struct net *, struct tcf_chain *, struct nlattr **, struct netlink_ext_ack *);
    void (*tmplt_destroy)(void *);
    int (*dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool);
    int (*terse_dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool);
    int (*tmplt_dump)(struct sk_buff *, struct net *, void *);
    struct module *owner;
    int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct tcf_proto_ops {
    struct list_head head;
    char kind[16];
    int (*classify)(struct sk_buff *, const struct tcf_proto *, struct tcf_result *);
    int (*init)(struct tcf_proto *);
    void (*destroy)(struct tcf_proto *, bool, struct netlink_ext_ack *);
    void * (*get)(struct tcf_proto *, u32);
    void (*put)(struct tcf_proto *, void *);
    int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, u32, struct netlink_ext_ack *);
    int (*delete)(struct tcf_proto *, void *, bool *, bool, struct netlink_ext_ack *);
    bool (*delete_empty)(struct tcf_proto *);
    void (*walk)(struct tcf_proto *, struct tcf_walker *, bool);
    int (*reoffload)(struct tcf_proto *, bool, flow_setup_cb_t *, void *, struct netlink_ext_ack *);
    void (*hw_add)(struct tcf_proto *, void *);
    void (*hw_del)(struct tcf_proto *, void *);
    void (*bind_class)(void *, u32, long unsigned int, void *, long unsigned int);
    void * (*tmplt_create)(struct net *, struct tcf_chain *, struct nlattr **, struct netlink_ext_ack *);
    void (*tmplt_destroy)(void *);
    int (*dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool);
    int (*terse_dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool);
    int (*tmplt_dump)(struct sk_buff *, struct net *, void *);
    struct module *owner;
    int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct tcf_proto_ops {
    struct list_head head;
    char kind[16];
    int (*classify)(struct sk_buff *, const struct tcf_proto *, struct tcf_result *);
    int (*init)(struct tcf_proto *);
    void (*destroy)(struct tcf_proto *, bool, struct netlink_ext_ack *);
    void * (*get)(struct tcf_proto *, u32);
    void (*put)(struct tcf_proto *, void *);
    int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, u32, struct netlink_ext_ack *);
    int (*delete)(struct tcf_proto *, void *, bool *, bool, struct netlink_ext_ack *);
    bool (*delete_empty)(struct tcf_proto *);
    void (*walk)(struct tcf_proto *, struct tcf_walker *, bool);
    int (*reoffload)(struct tcf_proto *, bool, flow_setup_cb_t *, void *, struct netlink_ext_ack *);
    void (*hw_add)(struct tcf_proto *, void *);
    void (*hw_del)(struct tcf_proto *, void *);
    void (*bind_class)(void *, u32, long unsigned int, void *, long unsigned int);
    void * (*tmplt_create)(struct net *, struct tcf_chain *, struct nlattr **, struct netlink_ext_ack *);
    void (*tmplt_destroy)(void *);
    int (*dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool);
    int (*terse_dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool);
    int (*tmplt_dump)(struct sk_buff *, struct net *, void *);
    struct module *owner;
    int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct tcf_proto_ops {
    struct list_head head;
    char kind[16];
    int (*classify)(struct sk_buff *, const struct tcf_proto *, struct tcf_result *);
    int (*init)(struct tcf_proto *);
    void (*destroy)(struct tcf_proto *, bool, struct netlink_ext_ack *);
    void * (*get)(struct tcf_proto *, u32);
    void (*put)(struct tcf_proto *, void *);
    int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, u32, struct netlink_ext_ack *);
    int (*delete)(struct tcf_proto *, void *, bool *, bool, struct netlink_ext_ack *);
    bool (*delete_empty)(struct tcf_proto *);
    void (*walk)(struct tcf_proto *, struct tcf_walker *, bool);
    int (*reoffload)(struct tcf_proto *, bool, flow_setup_cb_t *, void *, struct netlink_ext_ack *);
    void (*hw_add)(struct tcf_proto *, void *);
    void (*hw_del)(struct tcf_proto *, void *);
    void (*bind_class)(void *, u32, long unsigned int, void *, long unsigned int);
    void * (*tmplt_create)(struct net *, struct tcf_chain *, struct nlattr **, struct netlink_ext_ack *);
    void (*tmplt_destroy)(void *);
    int (*dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool);
    int (*terse_dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool);
    int (*tmplt_dump)(struct sk_buff *, struct net *, void *);
    struct module *owner;
    int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct tcf_proto_ops {
    struct list_head head;
    char kind[16];
    int (*classify)(struct sk_buff *, const struct tcf_proto *, struct tcf_result *);
    int (*init)(struct tcf_proto *);
    void (*destroy)(struct tcf_proto *, bool, struct netlink_ext_ack *);
    void * (*get)(struct tcf_proto *, u32);
    void (*put)(struct tcf_proto *, void *);
    int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, u32, struct netlink_ext_ack *);
    int (*delete)(struct tcf_proto *, void *, bool *, bool, struct netlink_ext_ack *);
    bool (*delete_empty)(struct tcf_proto *);
    void (*walk)(struct tcf_proto *, struct tcf_walker *, bool);
    int (*reoffload)(struct tcf_proto *, bool, flow_setup_cb_t *, void *, struct netlink_ext_ack *);
    void (*hw_add)(struct tcf_proto *, void *);
    void (*hw_del)(struct tcf_proto *, void *);
    void (*bind_class)(void *, u32, long unsigned int, void *, long unsigned int);
    void * (*tmplt_create)(struct net *, struct tcf_chain *, struct nlattr **, struct netlink_ext_ack *);
    void (*tmplt_destroy)(void *);
    struct tcf_exts * (*get_exts)(const struct tcf_proto *, u32);
    int (*dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool);
    int (*terse_dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool);
    int (*tmplt_dump)(struct sk_buff *, struct net *, void *);
    struct module *owner;
    int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct tcf_proto_ops {
    struct list_head head;
    char kind[16];
    int (*classify)(struct sk_buff *, const struct tcf_proto *, struct tcf_result *);
    int (*init)(struct tcf_proto *);
    void (*destroy)(struct tcf_proto *, bool, struct netlink_ext_ack *);
    void * (*get)(struct tcf_proto *, u32);
    void (*put)(struct tcf_proto *, void *);
    int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, u32, struct netlink_ext_ack *);
    int (*delete)(struct tcf_proto *, void *, bool *, bool, struct netlink_ext_ack *);
    bool (*delete_empty)(struct tcf_proto *);
    void (*walk)(struct tcf_proto *, struct tcf_walker *, bool);
    int (*reoffload)(struct tcf_proto *, bool, flow_setup_cb_t *, void *, struct netlink_ext_ack *);
    void (*hw_add)(struct tcf_proto *, void *);
    void (*hw_del)(struct tcf_proto *, void *);
    void (*bind_class)(void *, u32, long unsigned int, void *, long unsigned int);
    void * (*tmplt_create)(struct net *, struct tcf_chain *, struct nlattr **, struct netlink_ext_ack *);
    void (*tmplt_destroy)(void *);
    void (*tmplt_reoffload)(struct tcf_chain *, bool, flow_setup_cb_t *, void *);
    struct tcf_exts * (*get_exts)(const struct tcf_proto *, u32);
    int (*dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool);
    int (*terse_dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool);
    int (*tmplt_dump)(struct sk_buff *, struct net *, void *);
    struct module *owner;
    int flags;
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
struct tcf_proto_ops {
    struct list_head head;
    char kind[16];
    int (*classify)(struct sk_buff *, const struct tcf_proto *, struct tcf_result *);
    int (*init)(struct tcf_proto *);
    void (*destroy)(struct tcf_proto *, bool, struct netlink_ext_ack *);
    void * (*get)(struct tcf_proto *, u32);
    void (*put)(struct tcf_proto *, void *);
    int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, bool, bool, struct netlink_ext_ack *);
    int (*delete)(struct tcf_proto *, void *, bool *, bool, struct netlink_ext_ack *);
    bool (*delete_empty)(struct tcf_proto *);
    void (*walk)(struct tcf_proto *, struct tcf_walker *, bool);
    int (*reoffload)(struct tcf_proto *, bool, flow_setup_cb_t *, void *, struct netlink_ext_ack *);
    void (*hw_add)(struct tcf_proto *, void *);
    void (*hw_del)(struct tcf_proto *, void *);
    void (*bind_class)(void *, u32, long unsigned int, void *, long unsigned int);
    void * (*tmplt_create)(struct net *, struct tcf_chain *, struct nlattr **, struct netlink_ext_ack *);
    void (*tmplt_destroy)(void *);
    int (*dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool);
    int (*tmplt_dump)(struct sk_buff *, struct net *, void *);
    struct module *owner;
    int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct tcf_proto_ops {
    struct list_head head;
    char kind[16];
    int (*classify)(struct sk_buff *, const struct tcf_proto *, struct tcf_result *);
    int (*init)(struct tcf_proto *);
    void (*destroy)(struct tcf_proto *, bool, struct netlink_ext_ack *);
    void * (*get)(struct tcf_proto *, u32);
    void (*put)(struct tcf_proto *, void *);
    int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, bool, bool, struct netlink_ext_ack *);
    int (*delete)(struct tcf_proto *, void *, bool *, bool, struct netlink_ext_ack *);
    bool (*delete_empty)(struct tcf_proto *);
    void (*walk)(struct tcf_proto *, struct tcf_walker *, bool);
    int (*reoffload)(struct tcf_proto *, bool, flow_setup_cb_t *, void *, struct netlink_ext_ack *);
    void (*hw_add)(struct tcf_proto *, void *);
    void (*hw_del)(struct tcf_proto *, void *);
    void (*bind_class)(void *, u32, long unsigned int, void *, long unsigned int);
    void * (*tmplt_create)(struct net *, struct tcf_chain *, struct nlattr **, struct netlink_ext_ack *);
    void (*tmplt_destroy)(void *);
    int (*dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool);
    int (*tmplt_dump)(struct sk_buff *, struct net *, void *);
    struct module *owner;
    int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct tcf_proto_ops {
    struct list_head head;
    char kind[16];
    int (*classify)(struct sk_buff *, const struct tcf_proto *, struct tcf_result *);
    int (*init)(struct tcf_proto *);
    void (*destroy)(struct tcf_proto *, bool, struct netlink_ext_ack *);
    void * (*get)(struct tcf_proto *, u32);
    void (*put)(struct tcf_proto *, void *);
    int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, bool, bool, struct netlink_ext_ack *);
    int (*delete)(struct tcf_proto *, void *, bool *, bool, struct netlink_ext_ack *);
    bool (*delete_empty)(struct tcf_proto *);
    void (*walk)(struct tcf_proto *, struct tcf_walker *, bool);
    int (*reoffload)(struct tcf_proto *, bool, flow_setup_cb_t *, void *, struct netlink_ext_ack *);
    void (*hw_add)(struct tcf_proto *, void *);
    void (*hw_del)(struct tcf_proto *, void *);
    void (*bind_class)(void *, u32, long unsigned int, void *, long unsigned int);
    void * (*tmplt_create)(struct net *, struct tcf_chain *, struct nlattr **, struct netlink_ext_ack *);
    void (*tmplt_destroy)(void *);
    int (*dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool);
    int (*tmplt_dump)(struct sk_buff *, struct net *, void *);
    struct module *owner;
    int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct tcf_proto_ops {
    struct list_head head;
    char kind[16];
    int (*classify)(struct sk_buff *, const struct tcf_proto *, struct tcf_result *);
    int (*init)(struct tcf_proto *);
    void (*destroy)(struct tcf_proto *, bool, struct netlink_ext_ack *);
    void * (*get)(struct tcf_proto *, u32);
    void (*put)(struct tcf_proto *, void *);
    int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, bool, bool, struct netlink_ext_ack *);
    int (*delete)(struct tcf_proto *, void *, bool *, bool, struct netlink_ext_ack *);
    bool (*delete_empty)(struct tcf_proto *);
    void (*walk)(struct tcf_proto *, struct tcf_walker *, bool);
    int (*reoffload)(struct tcf_proto *, bool, flow_setup_cb_t *, void *, struct netlink_ext_ack *);
    void (*hw_add)(struct tcf_proto *, void *);
    void (*hw_del)(struct tcf_proto *, void *);
    void (*bind_class)(void *, u32, long unsigned int, void *, long unsigned int);
    void * (*tmplt_create)(struct net *, struct tcf_chain *, struct nlattr **, struct netlink_ext_ack *);
    void (*tmplt_destroy)(void *);
    int (*dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool);
    int (*tmplt_dump)(struct sk_buff *, struct net *, void *);
    struct module *owner;
    int flags;
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
struct tcf_proto_ops {
    struct list_head head;
    char kind[16];
    int (*classify)(struct sk_buff *, const struct tcf_proto *, struct tcf_result *);
    int (*init)(struct tcf_proto *);
    void (*destroy)(struct tcf_proto *, bool, struct netlink_ext_ack *);
    void * (*get)(struct tcf_proto *, u32);
    void (*put)(struct tcf_proto *, void *);
    int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, bool, bool, struct netlink_ext_ack *);
    int (*delete)(struct tcf_proto *, void *, bool *, bool, struct netlink_ext_ack *);
    bool (*delete_empty)(struct tcf_proto *);
    void (*walk)(struct tcf_proto *, struct tcf_walker *, bool);
    int (*reoffload)(struct tcf_proto *, bool, flow_setup_cb_t *, void *, struct netlink_ext_ack *);
    void (*hw_add)(struct tcf_proto *, void *);
    void (*hw_del)(struct tcf_proto *, void *);
    void (*bind_class)(void *, u32, long unsigned int, void *, long unsigned int);
    void * (*tmplt_create)(struct net *, struct tcf_chain *, struct nlattr **, struct netlink_ext_ack *);
    void (*tmplt_destroy)(void *);
    int (*dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool);
    int (*tmplt_dump)(struct sk_buff *, struct net *, void *);
    struct module *owner;
    int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct tcf_proto_ops {
    struct list_head head;
    char kind[16];
    int (*classify)(struct sk_buff *, const struct tcf_proto *, struct tcf_result *);
    int (*init)(struct tcf_proto *);
    void (*destroy)(struct tcf_proto *, bool, struct netlink_ext_ack *);
    void * (*get)(struct tcf_proto *, u32);
    void (*put)(struct tcf_proto *, void *);
    int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, bool, bool, struct netlink_ext_ack *);
    int (*delete)(struct tcf_proto *, void *, bool *, bool, struct netlink_ext_ack *);
    bool (*delete_empty)(struct tcf_proto *);
    void (*walk)(struct tcf_proto *, struct tcf_walker *, bool);
    int (*reoffload)(struct tcf_proto *, bool, flow_setup_cb_t *, void *, struct netlink_ext_ack *);
    void (*hw_add)(struct tcf_proto *, void *);
    void (*hw_del)(struct tcf_proto *, void *);
    void (*bind_class)(void *, u32, long unsigned int, void *, long unsigned int);
    void * (*tmplt_create)(struct net *, struct tcf_chain *, struct nlattr **, struct netlink_ext_ack *);
    void (*tmplt_destroy)(void *);
    int (*dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool);
    int (*tmplt_dump)(struct sk_buff *, struct net *, void *);
    struct module *owner;
    int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct tcf_proto_ops {
    struct list_head head;
    char kind[16];
    int (*classify)(struct sk_buff *, const struct tcf_proto *, struct tcf_result *);
    int (*init)(struct tcf_proto *);
    void (*destroy)(struct tcf_proto *, bool, struct netlink_ext_ack *);
    void * (*get)(struct tcf_proto *, u32);
    void (*put)(struct tcf_proto *, void *);
    int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, bool, bool, struct netlink_ext_ack *);
    int (*delete)(struct tcf_proto *, void *, bool *, bool, struct netlink_ext_ack *);
    bool (*delete_empty)(struct tcf_proto *);
    void (*walk)(struct tcf_proto *, struct tcf_walker *, bool);
    int (*reoffload)(struct tcf_proto *, bool, flow_setup_cb_t *, void *, struct netlink_ext_ack *);
    void (*hw_add)(struct tcf_proto *, void *);
    void (*hw_del)(struct tcf_proto *, void *);
    void (*bind_class)(void *, u32, long unsigned int, void *, long unsigned int);
    void * (*tmplt_create)(struct net *, struct tcf_chain *, struct nlattr **, struct netlink_ext_ack *);
    void (*tmplt_destroy)(void *);
    int (*dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool);
    int (*tmplt_dump)(struct sk_buff *, struct net *, void *);
    struct module *owner;
    int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct tcf_proto_ops {
    struct list_head head;
    char kind[16];
    int (*classify)(struct sk_buff *, const struct tcf_proto *, struct tcf_result *);
    int (*init)(struct tcf_proto *);
    void (*destroy)(struct tcf_proto *, bool, struct netlink_ext_ack *);
    void * (*get)(struct tcf_proto *, u32);
    void (*put)(struct tcf_proto *, void *);
    int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, bool, bool, struct netlink_ext_ack *);
    int (*delete)(struct tcf_proto *, void *, bool *, bool, struct netlink_ext_ack *);
    bool (*delete_empty)(struct tcf_proto *);
    void (*walk)(struct tcf_proto *, struct tcf_walker *, bool);
    int (*reoffload)(struct tcf_proto *, bool, flow_setup_cb_t *, void *, struct netlink_ext_ack *);
    void (*hw_add)(struct tcf_proto *, void *);
    void (*hw_del)(struct tcf_proto *, void *);
    void (*bind_class)(void *, u32, long unsigned int, void *, long unsigned int);
    void * (*tmplt_create)(struct net *, struct tcf_chain *, struct nlattr **, struct netlink_ext_ack *);
    void (*tmplt_destroy)(void *);
    int (*dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool);
    int (*tmplt_dump)(struct sk_buff *, struct net *, void *);
    struct module *owner;
    int flags;
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
<b>Field type changed. </b>
<code>bool (*destroy)(struct tcf_proto *, bool)</code> ➡️ <code>void (*destroy)(struct tcf_proto *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*delete)(struct tcf_proto *, long unsigned int)</code> ➡️ <code>int (*delete)(struct tcf_proto *, long unsigned int, bool *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*bind_class)(void *, u32, long unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int (*get)(struct tcf_proto *, u32)</code> ➡️ <code>void * (*get)(struct tcf_proto *, u32)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, long unsigned int *, bool)</code> ➡️ <code>int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, bool)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*delete)(struct tcf_proto *, long unsigned int, bool *)</code> ➡️ <code>int (*delete)(struct tcf_proto *, void *, bool *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*dump)(struct net *, struct tcf_proto *, long unsigned int, struct sk_buff *, struct tcmsg *)</code> ➡️ <code>int (*dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *)</code>
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
<code>void (*destroy)(struct tcf_proto *)</code> ➡️ <code>void (*destroy)(struct tcf_proto *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, bool)</code> ➡️ <code>int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, bool, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*delete)(struct tcf_proto *, void *, bool *)</code> ➡️ <code>int (*delete)(struct tcf_proto *, void *, bool *, struct netlink_ext_ack *)</code>
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
<code>int (*reoffload)(struct tcf_proto *, bool, tc_setup_cb_t *, void *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>void * (*tmplt_create)(struct net *, struct tcf_chain *, struct nlattr **, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*tmplt_destroy)(void *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*tmplt_dump)(struct sk_buff *, struct net *, void *)</code>
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
<code>void (*put)(struct tcf_proto *, void *)</code>
</li>
<li>
<b>Field added. </b>
<code>int flags</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*destroy)(struct tcf_proto *, struct netlink_ext_ack *)</code> ➡️ <code>void (*destroy)(struct tcf_proto *, bool, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, bool, struct netlink_ext_ack *)</code> ➡️ <code>int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, bool, bool, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*delete)(struct tcf_proto *, void *, bool *, struct netlink_ext_ack *)</code> ➡️ <code>int (*delete)(struct tcf_proto *, void *, bool *, bool, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*walk)(struct tcf_proto *, struct tcf_walker *)</code> ➡️ <code>void (*walk)(struct tcf_proto *, struct tcf_walker *, bool)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*reoffload)(struct tcf_proto *, bool, tc_setup_cb_t *, void *, struct netlink_ext_ack *)</code> ➡️ <code>int (*reoffload)(struct tcf_proto *, bool, flow_setup_cb_t *, void *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *)</code> ➡️ <code>int (*dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool)</code>
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
<code>bool (*delete_empty)(struct tcf_proto *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*hw_add)(struct tcf_proto *, void *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*hw_del)(struct tcf_proto *, void *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*bind_class)(void *, u32, long unsigned int)</code> ➡️ <code>void (*bind_class)(void *, u32, long unsigned int, void *, long unsigned int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*terse_dump)(struct net *, struct tcf_proto *, void *, struct sk_buff *, struct tcmsg *, bool)</code>
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
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, bool, bool, struct netlink_ext_ack *)</code> ➡️ <code>int (*change)(struct net *, struct sk_buff *, struct tcf_proto *, long unsigned int, u32, struct nlattr **, void **, u32, struct netlink_ext_ack *)</code>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct tcf_exts * (*get_exts)(const struct tcf_proto *, u32)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*tmplt_reoffload)(struct tcf_chain *, bool, flow_setup_cb_t *, void *)</code>
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
