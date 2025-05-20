# Struct: <code>tcp_ulp_ops</code>

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
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct tcp_ulp_ops {
    struct list_head list;
    int (*init)(struct sock *);
    void (*release)(struct sock *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct tcp_ulp_ops {
    struct list_head list;
    int (*init)(struct sock *);
    void (*release)(struct sock *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct tcp_ulp_ops {
    struct list_head list;
    int (*init)(struct sock *);
    void (*release)(struct sock *);
    int uid;
    char name[16];
    bool user_visible;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct tcp_ulp_ops {
    struct list_head list;
    int (*init)(struct sock *);
    void (*release)(struct sock *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct tcp_ulp_ops {
    struct list_head list;
    int (*init)(struct sock *);
    void (*update)(struct sock *, struct proto *);
    void (*release)(struct sock *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct tcp_ulp_ops {
    struct list_head list;
    int (*init)(struct sock *);
    void (*update)(struct sock *, struct proto *, void(*)(struct sock *));
    void (*release)(struct sock *);
    int (*get_info)(const struct sock *, struct sk_buff *);
    size_t (*get_info_size)(const struct sock *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct tcp_ulp_ops {
    struct list_head list;
    int (*init)(struct sock *);
    void (*update)(struct sock *, struct proto *, void(*)(struct sock *));
    void (*release)(struct sock *);
    int (*get_info)(const struct sock *, struct sk_buff *);
    size_t (*get_info_size)(const struct sock *);
    void (*clone)(const struct request_sock *, struct sock *, const gfp_t);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct tcp_ulp_ops {
    struct list_head list;
    int (*init)(struct sock *);
    void (*update)(struct sock *, struct proto *, void(*)(struct sock *));
    void (*release)(struct sock *);
    int (*get_info)(const struct sock *, struct sk_buff *);
    size_t (*get_info_size)(const struct sock *);
    void (*clone)(const struct request_sock *, struct sock *, const gfp_t);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct tcp_ulp_ops {
    struct list_head list;
    int (*init)(struct sock *);
    void (*update)(struct sock *, struct proto *, void(*)(struct sock *));
    void (*release)(struct sock *);
    int (*get_info)(const struct sock *, struct sk_buff *);
    size_t (*get_info_size)(const struct sock *);
    void (*clone)(const struct request_sock *, struct sock *, const gfp_t);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct tcp_ulp_ops {
    struct list_head list;
    int (*init)(struct sock *);
    void (*update)(struct sock *, struct proto *, void(*)(struct sock *));
    void (*release)(struct sock *);
    int (*get_info)(const struct sock *, struct sk_buff *);
    size_t (*get_info_size)(const struct sock *);
    void (*clone)(const struct request_sock *, struct sock *, const gfp_t);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct tcp_ulp_ops {
    struct list_head list;
    int (*init)(struct sock *);
    void (*update)(struct sock *, struct proto *, void(*)(struct sock *));
    void (*release)(struct sock *);
    int (*get_info)(const struct sock *, struct sk_buff *);
    size_t (*get_info_size)(const struct sock *);
    void (*clone)(const struct request_sock *, struct sock *, const gfp_t);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct tcp_ulp_ops {
    struct list_head list;
    int (*init)(struct sock *);
    void (*update)(struct sock *, struct proto *, void(*)(struct sock *));
    void (*release)(struct sock *);
    int (*get_info)(const struct sock *, struct sk_buff *);
    size_t (*get_info_size)(const struct sock *);
    void (*clone)(const struct request_sock *, struct sock *, const gfp_t);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct tcp_ulp_ops {
    struct list_head list;
    int (*init)(struct sock *);
    void (*update)(struct sock *, struct proto *, void(*)(struct sock *));
    void (*release)(struct sock *);
    int (*get_info)(const struct sock *, struct sk_buff *);
    size_t (*get_info_size)(const struct sock *);
    void (*clone)(const struct request_sock *, struct sock *, const gfp_t);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct tcp_ulp_ops {
    struct list_head list;
    int (*init)(struct sock *);
    void (*update)(struct sock *, struct proto *, void(*)(struct sock *));
    void (*release)(struct sock *);
    int (*get_info)(struct sock *, struct sk_buff *);
    size_t (*get_info_size)(const struct sock *);
    void (*clone)(const struct request_sock *, struct sock *, const gfp_t);
    char name[16];
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
struct tcp_ulp_ops {
    struct list_head list;
    int (*init)(struct sock *);
    void (*update)(struct sock *, struct proto *, void(*)(struct sock *));
    void (*release)(struct sock *);
    int (*get_info)(const struct sock *, struct sk_buff *);
    size_t (*get_info_size)(const struct sock *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct tcp_ulp_ops {
    struct list_head list;
    int (*init)(struct sock *);
    void (*update)(struct sock *, struct proto *, void(*)(struct sock *));
    void (*release)(struct sock *);
    int (*get_info)(const struct sock *, struct sk_buff *);
    size_t (*get_info_size)(const struct sock *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct tcp_ulp_ops {
    struct list_head list;
    int (*init)(struct sock *);
    void (*update)(struct sock *, struct proto *, void(*)(struct sock *));
    void (*release)(struct sock *);
    int (*get_info)(const struct sock *, struct sk_buff *);
    size_t (*get_info_size)(const struct sock *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct tcp_ulp_ops {
    struct list_head list;
    int (*init)(struct sock *);
    void (*update)(struct sock *, struct proto *, void(*)(struct sock *));
    void (*release)(struct sock *);
    int (*get_info)(const struct sock *, struct sk_buff *);
    size_t (*get_info_size)(const struct sock *);
    char name[16];
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
struct tcp_ulp_ops {
    struct list_head list;
    int (*init)(struct sock *);
    void (*update)(struct sock *, struct proto *, void(*)(struct sock *));
    void (*release)(struct sock *);
    int (*get_info)(const struct sock *, struct sk_buff *);
    size_t (*get_info_size)(const struct sock *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct tcp_ulp_ops {
    struct list_head list;
    int (*init)(struct sock *);
    void (*update)(struct sock *, struct proto *, void(*)(struct sock *));
    void (*release)(struct sock *);
    int (*get_info)(const struct sock *, struct sk_buff *);
    size_t (*get_info_size)(const struct sock *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct tcp_ulp_ops {
    struct list_head list;
    int (*init)(struct sock *);
    void (*update)(struct sock *, struct proto *, void(*)(struct sock *));
    void (*release)(struct sock *);
    int (*get_info)(const struct sock *, struct sk_buff *);
    size_t (*get_info_size)(const struct sock *);
    char name[16];
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct tcp_ulp_ops {
    struct list_head list;
    int (*init)(struct sock *);
    void (*update)(struct sock *, struct proto *, void(*)(struct sock *));
    void (*release)(struct sock *);
    int (*get_info)(const struct sock *, struct sk_buff *);
    size_t (*get_info_size)(const struct sock *);
    char name[16];
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
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int uid</code>
</li>
<li>
<b>Field added. </b>
<code>bool user_visible</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int uid</code>
</li>
<li>
<b>Field removed. </b>
<code>bool user_visible</code>
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
<code>void (*update)(struct sock *, struct proto *)</code>
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
<code>int (*get_info)(const struct sock *, struct sk_buff *)</code>
</li>
<li>
<b>Field added. </b>
<code>size_t (*get_info_size)(const struct sock *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*update)(struct sock *, struct proto *)</code> ➡️ <code>void (*update)(struct sock *, struct proto *, void(*)(struct sock *))</code>
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
<code>void (*clone)(const struct request_sock *, struct sock *, const gfp_t)</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*get_info)(const struct sock *, struct sk_buff *)</code> ➡️ <code>int (*get_info)(struct sock *, struct sk_buff *)</code>
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
