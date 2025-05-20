# Struct: <code>xfrm_mode</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct xfrm_mode {
    int (*input2)(struct xfrm_state *, struct sk_buff *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output2)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    struct xfrm_state_afinfo *afinfo;
    struct module *owner;
    unsigned int encap;
    int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct xfrm_mode {
    int (*input2)(struct xfrm_state *, struct sk_buff *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output2)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    struct xfrm_state_afinfo *afinfo;
    struct module *owner;
    unsigned int encap;
    int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct xfrm_mode {
    int (*input2)(struct xfrm_state *, struct sk_buff *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output2)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    struct xfrm_state_afinfo *afinfo;
    struct module *owner;
    unsigned int encap;
    int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct xfrm_mode {
    int (*input2)(struct xfrm_state *, struct sk_buff *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output2)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    struct sk_buff * (*gso_segment)(struct xfrm_state *, struct sk_buff *, netdev_features_t);
    void (*xmit)(struct xfrm_state *, struct sk_buff *);
    struct xfrm_state_afinfo *afinfo;
    struct module *owner;
    unsigned int encap;
    int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct xfrm_mode {
    int (*input2)(struct xfrm_state *, struct sk_buff *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output2)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    struct sk_buff * (*gso_segment)(struct xfrm_state *, struct sk_buff *, netdev_features_t);
    void (*xmit)(struct xfrm_state *, struct sk_buff *);
    struct xfrm_state_afinfo *afinfo;
    struct module *owner;
    unsigned int encap;
    int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct xfrm_mode {
    int (*input2)(struct xfrm_state *, struct sk_buff *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output2)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    struct sk_buff * (*gso_segment)(struct xfrm_state *, struct sk_buff *, netdev_features_t);
    void (*xmit)(struct xfrm_state *, struct sk_buff *);
    struct xfrm_state_afinfo *afinfo;
    struct module *owner;
    unsigned int encap;
    int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct xfrm_mode {
    int (*input2)(struct xfrm_state *, struct sk_buff *);
    int (*input)(struct xfrm_state *, struct sk_buff *);
    int (*output2)(struct xfrm_state *, struct sk_buff *);
    int (*output)(struct xfrm_state *, struct sk_buff *);
    struct sk_buff * (*gso_segment)(struct xfrm_state *, struct sk_buff *, netdev_features_t);
    void (*xmit)(struct xfrm_state *, struct sk_buff *);
    struct xfrm_state_afinfo *afinfo;
    struct module *owner;
    unsigned int encap;
    int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct xfrm_mode {
    u8 encap;
    u8 family;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct xfrm_mode {
    u8 encap;
    u8 family;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct xfrm_mode {
    u8 encap;
    u8 family;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct xfrm_mode {
    u8 encap;
    u8 family;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct xfrm_mode {
    u8 encap;
    u8 family;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct xfrm_mode {
    u8 encap;
    u8 family;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct xfrm_mode {
    u8 encap;
    u8 family;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct xfrm_mode {
    u8 encap;
    u8 family;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct xfrm_mode {
    u8 encap;
    u8 family;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct xfrm_mode {
    u8 encap;
    u8 family;
    u8 flags;
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
struct xfrm_mode {
    u8 encap;
    u8 family;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct xfrm_mode {
    u8 encap;
    u8 family;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct xfrm_mode {
    u8 encap;
    u8 family;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct xfrm_mode {
    u8 encap;
    u8 family;
    u8 flags;
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
struct xfrm_mode {
    u8 encap;
    u8 family;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct xfrm_mode {
    u8 encap;
    u8 family;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct xfrm_mode {
    u8 encap;
    u8 family;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct xfrm_mode {
    u8 encap;
    u8 family;
    u8 flags;
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
<code>struct sk_buff * (*gso_segment)(struct xfrm_state *, struct sk_buff *, netdev_features_t)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*xmit)(struct xfrm_state *, struct sk_buff *)</code>
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 family</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*input2)(struct xfrm_state *, struct sk_buff *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*input)(struct xfrm_state *, struct sk_buff *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*output2)(struct xfrm_state *, struct sk_buff *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*output)(struct xfrm_state *, struct sk_buff *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct sk_buff * (*gso_segment)(struct xfrm_state *, struct sk_buff *, netdev_features_t)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*xmit)(struct xfrm_state *, struct sk_buff *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct xfrm_state_afinfo *afinfo</code>
</li>
<li>
<b>Field removed. </b>
<code>struct module *owner</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int encap</code> ➡️ <code>u8 encap</code>
</li>
<li>
<b>Field type changed. </b>
<code>int flags</code> ➡️ <code>u8 flags</code>
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
