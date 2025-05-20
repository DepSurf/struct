# Struct: <code>xfrm_type</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct xfrm_type {
    char *description;
    struct module *owner;
    u8 proto;
    u8 flags;
    int (*init_state)(struct xfrm_state *);
    void (*destructor)(struct xfrm_state *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    int (*reject)(struct xfrm_state *, struct sk_buff *, const struct flowi *);
    int (*hdr_offset)(struct xfrm_state *, struct sk_buff *, u8 **);
    u32 (*get_mtu)(struct xfrm_state *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct xfrm_type {
    char *description;
    struct module *owner;
    u8 proto;
    u8 flags;
    int (*init_state)(struct xfrm_state *);
    void (*destructor)(struct xfrm_state *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    int (*reject)(struct xfrm_state *, struct sk_buff *, const struct flowi *);
    int (*hdr_offset)(struct xfrm_state *, struct sk_buff *, u8 **);
    u32 (*get_mtu)(struct xfrm_state *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct xfrm_type {
    char *description;
    struct module *owner;
    u8 proto;
    u8 flags;
    int (*init_state)(struct xfrm_state *);
    void (*destructor)(struct xfrm_state *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    int (*reject)(struct xfrm_state *, struct sk_buff *, const struct flowi *);
    int (*hdr_offset)(struct xfrm_state *, struct sk_buff *, u8 **);
    u32 (*get_mtu)(struct xfrm_state *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct xfrm_type {
    char *description;
    struct module *owner;
    u8 proto;
    u8 flags;
    int (*init_state)(struct xfrm_state *);
    void (*destructor)(struct xfrm_state *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    int (*reject)(struct xfrm_state *, struct sk_buff *, const struct flowi *);
    int (*hdr_offset)(struct xfrm_state *, struct sk_buff *, u8 **);
    u32 (*get_mtu)(struct xfrm_state *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct xfrm_type {
    char *description;
    struct module *owner;
    u8 proto;
    u8 flags;
    int (*init_state)(struct xfrm_state *);
    void (*destructor)(struct xfrm_state *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    int (*reject)(struct xfrm_state *, struct sk_buff *, const struct flowi *);
    int (*hdr_offset)(struct xfrm_state *, struct sk_buff *, u8 **);
    u32 (*get_mtu)(struct xfrm_state *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct xfrm_type {
    char *description;
    struct module *owner;
    u8 proto;
    u8 flags;
    int (*init_state)(struct xfrm_state *);
    void (*destructor)(struct xfrm_state *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    int (*reject)(struct xfrm_state *, struct sk_buff *, const struct flowi *);
    int (*hdr_offset)(struct xfrm_state *, struct sk_buff *, u8 **);
    u32 (*get_mtu)(struct xfrm_state *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct xfrm_type {
    char *description;
    struct module *owner;
    u8 proto;
    u8 flags;
    int (*init_state)(struct xfrm_state *);
    void (*destructor)(struct xfrm_state *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    int (*reject)(struct xfrm_state *, struct sk_buff *, const struct flowi *);
    int (*hdr_offset)(struct xfrm_state *, struct sk_buff *, u8 **);
    u32 (*get_mtu)(struct xfrm_state *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct xfrm_type {
    char *description;
    struct module *owner;
    u8 proto;
    u8 flags;
    int (*init_state)(struct xfrm_state *);
    void (*destructor)(struct xfrm_state *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    int (*reject)(struct xfrm_state *, struct sk_buff *, const struct flowi *);
    int (*hdr_offset)(struct xfrm_state *, struct sk_buff *, u8 **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct xfrm_type {
    char *description;
    struct module *owner;
    u8 proto;
    u8 flags;
    int (*init_state)(struct xfrm_state *);
    void (*destructor)(struct xfrm_state *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    int (*reject)(struct xfrm_state *, struct sk_buff *, const struct flowi *);
    int (*hdr_offset)(struct xfrm_state *, struct sk_buff *, u8 **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct xfrm_type {
    char *description;
    struct module *owner;
    u8 proto;
    u8 flags;
    int (*init_state)(struct xfrm_state *);
    void (*destructor)(struct xfrm_state *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    int (*reject)(struct xfrm_state *, struct sk_buff *, const struct flowi *);
    int (*hdr_offset)(struct xfrm_state *, struct sk_buff *, u8 **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct xfrm_type {
    char *description;
    struct module *owner;
    u8 proto;
    u8 flags;
    int (*init_state)(struct xfrm_state *);
    void (*destructor)(struct xfrm_state *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    int (*reject)(struct xfrm_state *, struct sk_buff *, const struct flowi *);
    int (*hdr_offset)(struct xfrm_state *, struct sk_buff *, u8 **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct xfrm_type {
    char *description;
    struct module *owner;
    u8 proto;
    u8 flags;
    int (*init_state)(struct xfrm_state *);
    void (*destructor)(struct xfrm_state *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    int (*reject)(struct xfrm_state *, struct sk_buff *, const struct flowi *);
    int (*hdr_offset)(struct xfrm_state *, struct sk_buff *, u8 **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct xfrm_type {
    struct module *owner;
    u8 proto;
    u8 flags;
    int (*init_state)(struct xfrm_state *);
    void (*destructor)(struct xfrm_state *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    int (*reject)(struct xfrm_state *, struct sk_buff *, const struct flowi *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct xfrm_type {
    struct module *owner;
    u8 proto;
    u8 flags;
    int (*init_state)(struct xfrm_state *);
    void (*destructor)(struct xfrm_state *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    int (*reject)(struct xfrm_state *, struct sk_buff *, const struct flowi *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct xfrm_type {
    struct module *owner;
    u8 proto;
    u8 flags;
    int (*init_state)(struct xfrm_state *, struct netlink_ext_ack *);
    void (*destructor)(struct xfrm_state *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    int (*reject)(struct xfrm_state *, struct sk_buff *, const struct flowi *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct xfrm_type {
    struct module *owner;
    u8 proto;
    u8 flags;
    int (*init_state)(struct xfrm_state *, struct netlink_ext_ack *);
    void (*destructor)(struct xfrm_state *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    int (*reject)(struct xfrm_state *, struct sk_buff *, const struct flowi *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct xfrm_type {
    struct module *owner;
    u8 proto;
    u8 flags;
    int (*init_state)(struct xfrm_state *, struct netlink_ext_ack *);
    void (*destructor)(struct xfrm_state *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    int (*reject)(struct xfrm_state *, struct sk_buff *, const struct flowi *);
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
struct xfrm_type {
    char *description;
    struct module *owner;
    u8 proto;
    u8 flags;
    int (*init_state)(struct xfrm_state *);
    void (*destructor)(struct xfrm_state *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    int (*reject)(struct xfrm_state *, struct sk_buff *, const struct flowi *);
    int (*hdr_offset)(struct xfrm_state *, struct sk_buff *, u8 **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct xfrm_type {
    char *description;
    struct module *owner;
    u8 proto;
    u8 flags;
    int (*init_state)(struct xfrm_state *);
    void (*destructor)(struct xfrm_state *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    int (*reject)(struct xfrm_state *, struct sk_buff *, const struct flowi *);
    int (*hdr_offset)(struct xfrm_state *, struct sk_buff *, u8 **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct xfrm_type {
    char *description;
    struct module *owner;
    u8 proto;
    u8 flags;
    int (*init_state)(struct xfrm_state *);
    void (*destructor)(struct xfrm_state *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    int (*reject)(struct xfrm_state *, struct sk_buff *, const struct flowi *);
    int (*hdr_offset)(struct xfrm_state *, struct sk_buff *, u8 **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct xfrm_type {
    char *description;
    struct module *owner;
    u8 proto;
    u8 flags;
    int (*init_state)(struct xfrm_state *);
    void (*destructor)(struct xfrm_state *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    int (*reject)(struct xfrm_state *, struct sk_buff *, const struct flowi *);
    int (*hdr_offset)(struct xfrm_state *, struct sk_buff *, u8 **);
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
struct xfrm_type {
    char *description;
    struct module *owner;
    u8 proto;
    u8 flags;
    int (*init_state)(struct xfrm_state *);
    void (*destructor)(struct xfrm_state *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    int (*reject)(struct xfrm_state *, struct sk_buff *, const struct flowi *);
    int (*hdr_offset)(struct xfrm_state *, struct sk_buff *, u8 **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct xfrm_type {
    char *description;
    struct module *owner;
    u8 proto;
    u8 flags;
    int (*init_state)(struct xfrm_state *);
    void (*destructor)(struct xfrm_state *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    int (*reject)(struct xfrm_state *, struct sk_buff *, const struct flowi *);
    int (*hdr_offset)(struct xfrm_state *, struct sk_buff *, u8 **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct xfrm_type {
    char *description;
    struct module *owner;
    u8 proto;
    u8 flags;
    int (*init_state)(struct xfrm_state *);
    void (*destructor)(struct xfrm_state *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    int (*reject)(struct xfrm_state *, struct sk_buff *, const struct flowi *);
    int (*hdr_offset)(struct xfrm_state *, struct sk_buff *, u8 **);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct xfrm_type {
    char *description;
    struct module *owner;
    u8 proto;
    u8 flags;
    int (*init_state)(struct xfrm_state *);
    void (*destructor)(struct xfrm_state *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    int (*reject)(struct xfrm_state *, struct sk_buff *, const struct flowi *);
    int (*hdr_offset)(struct xfrm_state *, struct sk_buff *, u8 **);
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
<b>Field removed. </b>
<code>u32 (*get_mtu)(struct xfrm_state *, int)</code>
</li>
</ul>
</details>
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
<b>Field removed. </b>
<code>char *description</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*hdr_offset)(struct xfrm_state *, struct sk_buff *, u8 **)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*init_state)(struct xfrm_state *)</code> ➡️ <code>int (*init_state)(struct xfrm_state *, struct netlink_ext_ack *)</code>
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
