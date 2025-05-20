# Struct: <code>netlink_callback</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct netlink_callback {
    struct sk_buff *skb;
    const struct nlmsghdr *nlh;
    int (*dump)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    void *data;
    struct module *module;
    u16 family;
    u16 min_dump_alloc;
    unsigned int prev_seq;
    unsigned int seq;
    long int args[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct netlink_callback {
    struct sk_buff *skb;
    const struct nlmsghdr *nlh;
    int (*start)(struct netlink_callback *);
    int (*dump)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    void *data;
    struct module *module;
    u16 family;
    u16 min_dump_alloc;
    unsigned int prev_seq;
    unsigned int seq;
    long int args[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct netlink_callback {
    struct sk_buff *skb;
    const struct nlmsghdr *nlh;
    int (*start)(struct netlink_callback *);
    int (*dump)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    void *data;
    struct module *module;
    u16 family;
    u16 min_dump_alloc;
    unsigned int prev_seq;
    unsigned int seq;
    long int args[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct netlink_callback {
    struct sk_buff *skb;
    const struct nlmsghdr *nlh;
    int (*start)(struct netlink_callback *);
    int (*dump)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    void *data;
    struct module *module;
    u16 family;
    u16 min_dump_alloc;
    unsigned int prev_seq;
    unsigned int seq;
    long int args[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct netlink_callback {
    struct sk_buff *skb;
    const struct nlmsghdr *nlh;
    int (*start)(struct netlink_callback *);
    int (*dump)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    void *data;
    struct module *module;
    u16 family;
    u16 min_dump_alloc;
    unsigned int prev_seq;
    unsigned int seq;
    long int args[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct netlink_callback {
    struct sk_buff *skb;
    const struct nlmsghdr *nlh;
    int (*start)(struct netlink_callback *);
    int (*dump)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    void *data;
    struct module *module;
    u16 family;
    u16 min_dump_alloc;
    unsigned int prev_seq;
    unsigned int seq;
    long int args[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct netlink_callback {
    struct sk_buff *skb;
    const struct nlmsghdr *nlh;
    int (*dump)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    void *data;
    struct module *module;
    struct netlink_ext_ack *extack;
    u16 family;
    u16 min_dump_alloc;
    bool strict_check;
    u16 answer_flags;
    unsigned int prev_seq;
    unsigned int seq;
    long int args[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct netlink_callback {
    struct sk_buff *skb;
    const struct nlmsghdr *nlh;
    int (*dump)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    void *data;
    struct module *module;
    struct netlink_ext_ack *extack;
    u16 family;
    u16 min_dump_alloc;
    bool strict_check;
    u16 answer_flags;
    unsigned int prev_seq;
    unsigned int seq;
    u8 ctx[48];
    long int args[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct netlink_callback {
    struct sk_buff *skb;
    const struct nlmsghdr *nlh;
    int (*dump)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    void *data;
    struct module *module;
    struct netlink_ext_ack *extack;
    u16 family;
    u16 min_dump_alloc;
    bool strict_check;
    u16 answer_flags;
    unsigned int prev_seq;
    unsigned int seq;
    u8 ctx[48];
    long int args[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct netlink_callback {
    struct sk_buff *skb;
    const struct nlmsghdr *nlh;
    int (*dump)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    void *data;
    struct module *module;
    struct netlink_ext_ack *extack;
    u16 family;
    u16 answer_flags;
    u32 min_dump_alloc;
    unsigned int prev_seq;
    unsigned int seq;
    bool strict_check;
    u8 ctx[48];
    long int args[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct netlink_callback {
    struct sk_buff *skb;
    const struct nlmsghdr *nlh;
    int (*dump)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    void *data;
    struct module *module;
    struct netlink_ext_ack *extack;
    u16 family;
    u16 answer_flags;
    u32 min_dump_alloc;
    unsigned int prev_seq;
    unsigned int seq;
    bool strict_check;
    u8 ctx[48];
    long int args[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct netlink_callback {
    struct sk_buff *skb;
    const struct nlmsghdr *nlh;
    int (*dump)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    void *data;
    struct module *module;
    struct netlink_ext_ack *extack;
    u16 family;
    u16 answer_flags;
    u32 min_dump_alloc;
    unsigned int prev_seq;
    unsigned int seq;
    bool strict_check;
    u8 ctx[48];
    long int args[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct netlink_callback {
    struct sk_buff *skb;
    const struct nlmsghdr *nlh;
    int (*dump)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    void *data;
    struct module *module;
    struct netlink_ext_ack *extack;
    u16 family;
    u16 answer_flags;
    u32 min_dump_alloc;
    unsigned int prev_seq;
    unsigned int seq;
    bool strict_check;
    u8 ctx[48];
    long int args[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct netlink_callback {
    struct sk_buff *skb;
    const struct nlmsghdr *nlh;
    int (*dump)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    void *data;
    struct module *module;
    struct netlink_ext_ack *extack;
    u16 family;
    u16 answer_flags;
    u32 min_dump_alloc;
    unsigned int prev_seq;
    unsigned int seq;
    bool strict_check;
    u8 ctx[48];
    long int args[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct netlink_callback {
    struct sk_buff *skb;
    const struct nlmsghdr *nlh;
    int (*dump)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    void *data;
    struct module *module;
    struct netlink_ext_ack *extack;
    u16 family;
    u16 answer_flags;
    u32 min_dump_alloc;
    unsigned int prev_seq;
    unsigned int seq;
    bool strict_check;
    u8 ctx[48];
    long int args[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct netlink_callback {
    struct sk_buff *skb;
    const struct nlmsghdr *nlh;
    int (*dump)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    void *data;
    struct module *module;
    struct netlink_ext_ack *extack;
    u16 family;
    u16 answer_flags;
    u32 min_dump_alloc;
    unsigned int prev_seq;
    unsigned int seq;
    bool strict_check;
    u8 ctx[48];
    long int args[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct netlink_callback {
    struct sk_buff *skb;
    const struct nlmsghdr *nlh;
    int (*dump)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    void *data;
    struct module *module;
    struct netlink_ext_ack *extack;
    u16 family;
    u16 answer_flags;
    u32 min_dump_alloc;
    unsigned int prev_seq;
    unsigned int seq;
    bool strict_check;
    u8 ctx[48];
    long int args[6];
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
struct netlink_callback {
    struct sk_buff *skb;
    const struct nlmsghdr *nlh;
    int (*dump)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    void *data;
    struct module *module;
    struct netlink_ext_ack *extack;
    u16 family;
    u16 min_dump_alloc;
    bool strict_check;
    u16 answer_flags;
    unsigned int prev_seq;
    unsigned int seq;
    u8 ctx[48];
    long int args[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct netlink_callback {
    struct sk_buff *skb;
    const struct nlmsghdr *nlh;
    int (*dump)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    void *data;
    struct module *module;
    struct netlink_ext_ack *extack;
    u16 family;
    u16 min_dump_alloc;
    bool strict_check;
    u16 answer_flags;
    unsigned int prev_seq;
    unsigned int seq;
    u8 ctx[48];
    long int args[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct netlink_callback {
    struct sk_buff *skb;
    const struct nlmsghdr *nlh;
    int (*dump)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    void *data;
    struct module *module;
    struct netlink_ext_ack *extack;
    u16 family;
    u16 min_dump_alloc;
    bool strict_check;
    u16 answer_flags;
    unsigned int prev_seq;
    unsigned int seq;
    u8 ctx[48];
    long int args[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct netlink_callback {
    struct sk_buff *skb;
    const struct nlmsghdr *nlh;
    int (*dump)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    void *data;
    struct module *module;
    struct netlink_ext_ack *extack;
    u16 family;
    u16 min_dump_alloc;
    bool strict_check;
    u16 answer_flags;
    unsigned int prev_seq;
    unsigned int seq;
    u8 ctx[48];
    long int args[6];
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
struct netlink_callback {
    struct sk_buff *skb;
    const struct nlmsghdr *nlh;
    int (*dump)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    void *data;
    struct module *module;
    struct netlink_ext_ack *extack;
    u16 family;
    u16 min_dump_alloc;
    bool strict_check;
    u16 answer_flags;
    unsigned int prev_seq;
    unsigned int seq;
    u8 ctx[48];
    long int args[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct netlink_callback {
    struct sk_buff *skb;
    const struct nlmsghdr *nlh;
    int (*dump)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    void *data;
    struct module *module;
    struct netlink_ext_ack *extack;
    u16 family;
    u16 min_dump_alloc;
    bool strict_check;
    u16 answer_flags;
    unsigned int prev_seq;
    unsigned int seq;
    u8 ctx[48];
    long int args[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct netlink_callback {
    struct sk_buff *skb;
    const struct nlmsghdr *nlh;
    int (*dump)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    void *data;
    struct module *module;
    struct netlink_ext_ack *extack;
    u16 family;
    u16 min_dump_alloc;
    bool strict_check;
    u16 answer_flags;
    unsigned int prev_seq;
    unsigned int seq;
    u8 ctx[48];
    long int args[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct netlink_callback {
    struct sk_buff *skb;
    const struct nlmsghdr *nlh;
    int (*dump)(struct sk_buff *, struct netlink_callback *);
    int (*done)(struct netlink_callback *);
    void *data;
    struct module *module;
    struct netlink_ext_ack *extack;
    u16 family;
    u16 min_dump_alloc;
    bool strict_check;
    u16 answer_flags;
    unsigned int prev_seq;
    unsigned int seq;
    u8 ctx[48];
    long int args[6];
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
<code>int (*start)(struct netlink_callback *)</code>
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
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct netlink_ext_ack *extack</code>
</li>
<li>
<b>Field added. </b>
<code>bool strict_check</code>
</li>
<li>
<b>Field added. </b>
<code>u16 answer_flags</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*start)(struct netlink_callback *)</code>
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
<code>u8 ctx[48]</code>
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
<b>Field type changed. </b>
<code>u16 min_dump_alloc</code> ➡️ <code>u32 min_dump_alloc</code>
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
