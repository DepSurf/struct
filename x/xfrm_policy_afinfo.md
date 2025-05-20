# Struct: <code>xfrm_policy_afinfo</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct xfrm_policy_afinfo {
    short unsigned int family;
    struct dst_ops *dst_ops;
    void (*garbage_collect)(struct net *);
    struct dst_entry * (*dst_lookup)(struct net *, int, int, const xfrm_address_t *, const xfrm_address_t *);
    int (*get_saddr)(struct net *, int, xfrm_address_t *, xfrm_address_t *);
    void (*decode_session)(struct sk_buff *, struct flowi *, int);
    int (*get_tos)(const struct flowi *);
    int (*init_path)(struct xfrm_dst *, struct dst_entry *, int);
    int (*fill_dst)(struct xfrm_dst *, struct net_device *, const struct flowi *);
    struct dst_entry * (*blackhole_route)(struct net *, struct dst_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct xfrm_policy_afinfo {
    short unsigned int family;
    struct dst_ops *dst_ops;
    void (*garbage_collect)(struct net *);
    struct dst_entry * (*dst_lookup)(struct net *, int, int, const xfrm_address_t *, const xfrm_address_t *);
    int (*get_saddr)(struct net *, int, xfrm_address_t *, xfrm_address_t *);
    void (*decode_session)(struct sk_buff *, struct flowi *, int);
    int (*get_tos)(const struct flowi *);
    int (*init_path)(struct xfrm_dst *, struct dst_entry *, int);
    int (*fill_dst)(struct xfrm_dst *, struct net_device *, const struct flowi *);
    struct dst_entry * (*blackhole_route)(struct net *, struct dst_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct xfrm_policy_afinfo {
    short unsigned int family;
    struct dst_ops *dst_ops;
    void (*garbage_collect)(struct net *);
    struct dst_entry * (*dst_lookup)(struct net *, int, int, const xfrm_address_t *, const xfrm_address_t *);
    int (*get_saddr)(struct net *, int, xfrm_address_t *, xfrm_address_t *);
    void (*decode_session)(struct sk_buff *, struct flowi *, int);
    int (*get_tos)(const struct flowi *);
    int (*init_path)(struct xfrm_dst *, struct dst_entry *, int);
    int (*fill_dst)(struct xfrm_dst *, struct net_device *, const struct flowi *);
    struct dst_entry * (*blackhole_route)(struct net *, struct dst_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct xfrm_policy_afinfo {
    struct dst_ops *dst_ops;
    struct dst_entry * (*dst_lookup)(struct net *, int, int, const xfrm_address_t *, const xfrm_address_t *);
    int (*get_saddr)(struct net *, int, xfrm_address_t *, xfrm_address_t *);
    void (*decode_session)(struct sk_buff *, struct flowi *, int);
    int (*get_tos)(const struct flowi *);
    int (*init_path)(struct xfrm_dst *, struct dst_entry *, int);
    int (*fill_dst)(struct xfrm_dst *, struct net_device *, const struct flowi *);
    struct dst_entry * (*blackhole_route)(struct net *, struct dst_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct xfrm_policy_afinfo {
    struct dst_ops *dst_ops;
    struct dst_entry * (*dst_lookup)(struct net *, int, int, const xfrm_address_t *, const xfrm_address_t *, u32);
    int (*get_saddr)(struct net *, int, xfrm_address_t *, xfrm_address_t *, u32);
    void (*decode_session)(struct sk_buff *, struct flowi *, int);
    int (*get_tos)(const struct flowi *);
    int (*init_path)(struct xfrm_dst *, struct dst_entry *, int);
    int (*fill_dst)(struct xfrm_dst *, struct net_device *, const struct flowi *);
    struct dst_entry * (*blackhole_route)(struct net *, struct dst_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct xfrm_policy_afinfo {
    struct dst_ops *dst_ops;
    struct dst_entry * (*dst_lookup)(struct net *, int, int, const xfrm_address_t *, const xfrm_address_t *, u32);
    int (*get_saddr)(struct net *, int, xfrm_address_t *, xfrm_address_t *, u32);
    void (*decode_session)(struct sk_buff *, struct flowi *, int);
    int (*get_tos)(const struct flowi *);
    int (*init_path)(struct xfrm_dst *, struct dst_entry *, int);
    int (*fill_dst)(struct xfrm_dst *, struct net_device *, const struct flowi *);
    struct dst_entry * (*blackhole_route)(struct net *, struct dst_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct xfrm_policy_afinfo {
    struct dst_ops *dst_ops;
    struct dst_entry * (*dst_lookup)(struct net *, int, int, const xfrm_address_t *, const xfrm_address_t *, u32);
    int (*get_saddr)(struct net *, int, xfrm_address_t *, xfrm_address_t *, u32);
    void (*decode_session)(struct sk_buff *, struct flowi *, int);
    int (*get_tos)(const struct flowi *);
    int (*init_path)(struct xfrm_dst *, struct dst_entry *, int);
    int (*fill_dst)(struct xfrm_dst *, struct net_device *, const struct flowi *);
    struct dst_entry * (*blackhole_route)(struct net *, struct dst_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct xfrm_policy_afinfo {
    struct dst_ops *dst_ops;
    struct dst_entry * (*dst_lookup)(struct net *, int, int, const xfrm_address_t *, const xfrm_address_t *, u32);
    int (*get_saddr)(struct net *, int, xfrm_address_t *, xfrm_address_t *, u32);
    int (*fill_dst)(struct xfrm_dst *, struct net_device *, const struct flowi *);
    struct dst_entry * (*blackhole_route)(struct net *, struct dst_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct xfrm_policy_afinfo {
    struct dst_ops *dst_ops;
    struct dst_entry * (*dst_lookup)(struct net *, int, int, const xfrm_address_t *, const xfrm_address_t *, u32);
    int (*get_saddr)(struct net *, int, xfrm_address_t *, xfrm_address_t *, u32);
    int (*fill_dst)(struct xfrm_dst *, struct net_device *, const struct flowi *);
    struct dst_entry * (*blackhole_route)(struct net *, struct dst_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct xfrm_policy_afinfo {
    struct dst_ops *dst_ops;
    struct dst_entry * (*dst_lookup)(struct net *, int, int, const xfrm_address_t *, const xfrm_address_t *, u32);
    int (*get_saddr)(struct net *, int, xfrm_address_t *, xfrm_address_t *, u32);
    int (*fill_dst)(struct xfrm_dst *, struct net_device *, const struct flowi *);
    struct dst_entry * (*blackhole_route)(struct net *, struct dst_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct xfrm_policy_afinfo {
    struct dst_ops *dst_ops;
    struct dst_entry * (*dst_lookup)(struct net *, int, int, const xfrm_address_t *, const xfrm_address_t *, u32);
    int (*get_saddr)(struct net *, int, xfrm_address_t *, xfrm_address_t *, u32);
    int (*fill_dst)(struct xfrm_dst *, struct net_device *, const struct flowi *);
    struct dst_entry * (*blackhole_route)(struct net *, struct dst_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct xfrm_policy_afinfo {
    struct dst_ops *dst_ops;
    struct dst_entry * (*dst_lookup)(struct net *, int, int, const xfrm_address_t *, const xfrm_address_t *, u32);
    int (*get_saddr)(struct net *, int, xfrm_address_t *, xfrm_address_t *, u32);
    int (*fill_dst)(struct xfrm_dst *, struct net_device *, const struct flowi *);
    struct dst_entry * (*blackhole_route)(struct net *, struct dst_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct xfrm_policy_afinfo {
    struct dst_ops *dst_ops;
    struct dst_entry * (*dst_lookup)(struct net *, int, int, const xfrm_address_t *, const xfrm_address_t *, u32);
    int (*get_saddr)(struct net *, int, xfrm_address_t *, xfrm_address_t *, u32);
    int (*fill_dst)(struct xfrm_dst *, struct net_device *, const struct flowi *);
    struct dst_entry * (*blackhole_route)(struct net *, struct dst_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct xfrm_policy_afinfo {
    struct dst_ops *dst_ops;
    struct dst_entry * (*dst_lookup)(struct net *, int, int, const xfrm_address_t *, const xfrm_address_t *, u32);
    int (*get_saddr)(struct net *, int, xfrm_address_t *, xfrm_address_t *, u32);
    int (*fill_dst)(struct xfrm_dst *, struct net_device *, const struct flowi *);
    struct dst_entry * (*blackhole_route)(struct net *, struct dst_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct xfrm_policy_afinfo {
    struct dst_ops *dst_ops;
    struct dst_entry * (*dst_lookup)(struct net *, int, int, const xfrm_address_t *, const xfrm_address_t *, u32);
    int (*get_saddr)(struct net *, int, xfrm_address_t *, xfrm_address_t *, u32);
    int (*fill_dst)(struct xfrm_dst *, struct net_device *, const struct flowi *);
    struct dst_entry * (*blackhole_route)(struct net *, struct dst_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct xfrm_policy_afinfo {
    struct dst_ops *dst_ops;
    struct dst_entry * (*dst_lookup)(struct net *, int, int, const xfrm_address_t *, const xfrm_address_t *, u32);
    int (*get_saddr)(struct net *, int, xfrm_address_t *, xfrm_address_t *, u32);
    int (*fill_dst)(struct xfrm_dst *, struct net_device *, const struct flowi *);
    struct dst_entry * (*blackhole_route)(struct net *, struct dst_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct xfrm_policy_afinfo {
    struct dst_ops *dst_ops;
    struct dst_entry * (*dst_lookup)(struct net *, int, int, const xfrm_address_t *, const xfrm_address_t *, u32);
    int (*get_saddr)(struct net *, int, xfrm_address_t *, xfrm_address_t *, u32);
    int (*fill_dst)(struct xfrm_dst *, struct net_device *, const struct flowi *);
    struct dst_entry * (*blackhole_route)(struct net *, struct dst_entry *);
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
struct xfrm_policy_afinfo {
    struct dst_ops *dst_ops;
    struct dst_entry * (*dst_lookup)(struct net *, int, int, const xfrm_address_t *, const xfrm_address_t *, u32);
    int (*get_saddr)(struct net *, int, xfrm_address_t *, xfrm_address_t *, u32);
    int (*fill_dst)(struct xfrm_dst *, struct net_device *, const struct flowi *);
    struct dst_entry * (*blackhole_route)(struct net *, struct dst_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct xfrm_policy_afinfo {
    struct dst_ops *dst_ops;
    struct dst_entry * (*dst_lookup)(struct net *, int, int, const xfrm_address_t *, const xfrm_address_t *, u32);
    int (*get_saddr)(struct net *, int, xfrm_address_t *, xfrm_address_t *, u32);
    int (*fill_dst)(struct xfrm_dst *, struct net_device *, const struct flowi *);
    struct dst_entry * (*blackhole_route)(struct net *, struct dst_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct xfrm_policy_afinfo {
    struct dst_ops *dst_ops;
    struct dst_entry * (*dst_lookup)(struct net *, int, int, const xfrm_address_t *, const xfrm_address_t *, u32);
    int (*get_saddr)(struct net *, int, xfrm_address_t *, xfrm_address_t *, u32);
    int (*fill_dst)(struct xfrm_dst *, struct net_device *, const struct flowi *);
    struct dst_entry * (*blackhole_route)(struct net *, struct dst_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct xfrm_policy_afinfo {
    struct dst_ops *dst_ops;
    struct dst_entry * (*dst_lookup)(struct net *, int, int, const xfrm_address_t *, const xfrm_address_t *, u32);
    int (*get_saddr)(struct net *, int, xfrm_address_t *, xfrm_address_t *, u32);
    int (*fill_dst)(struct xfrm_dst *, struct net_device *, const struct flowi *);
    struct dst_entry * (*blackhole_route)(struct net *, struct dst_entry *);
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
struct xfrm_policy_afinfo {
    struct dst_ops *dst_ops;
    struct dst_entry * (*dst_lookup)(struct net *, int, int, const xfrm_address_t *, const xfrm_address_t *, u32);
    int (*get_saddr)(struct net *, int, xfrm_address_t *, xfrm_address_t *, u32);
    int (*fill_dst)(struct xfrm_dst *, struct net_device *, const struct flowi *);
    struct dst_entry * (*blackhole_route)(struct net *, struct dst_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct xfrm_policy_afinfo {
    struct dst_ops *dst_ops;
    struct dst_entry * (*dst_lookup)(struct net *, int, int, const xfrm_address_t *, const xfrm_address_t *, u32);
    int (*get_saddr)(struct net *, int, xfrm_address_t *, xfrm_address_t *, u32);
    int (*fill_dst)(struct xfrm_dst *, struct net_device *, const struct flowi *);
    struct dst_entry * (*blackhole_route)(struct net *, struct dst_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct xfrm_policy_afinfo {
    struct dst_ops *dst_ops;
    struct dst_entry * (*dst_lookup)(struct net *, int, int, const xfrm_address_t *, const xfrm_address_t *, u32);
    int (*get_saddr)(struct net *, int, xfrm_address_t *, xfrm_address_t *, u32);
    int (*fill_dst)(struct xfrm_dst *, struct net_device *, const struct flowi *);
    struct dst_entry * (*blackhole_route)(struct net *, struct dst_entry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct xfrm_policy_afinfo {
    struct dst_ops *dst_ops;
    struct dst_entry * (*dst_lookup)(struct net *, int, int, const xfrm_address_t *, const xfrm_address_t *, u32);
    int (*get_saddr)(struct net *, int, xfrm_address_t *, xfrm_address_t *, u32);
    int (*fill_dst)(struct xfrm_dst *, struct net_device *, const struct flowi *);
    struct dst_entry * (*blackhole_route)(struct net *, struct dst_entry *);
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
<b>Field removed. </b>
<code>short unsigned int family</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*garbage_collect)(struct net *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct dst_entry * (*dst_lookup)(struct net *, int, int, const xfrm_address_t *, const xfrm_address_t *)</code> ➡️ <code>struct dst_entry * (*dst_lookup)(struct net *, int, int, const xfrm_address_t *, const xfrm_address_t *, u32)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*get_saddr)(struct net *, int, xfrm_address_t *, xfrm_address_t *)</code> ➡️ <code>int (*get_saddr)(struct net *, int, xfrm_address_t *, xfrm_address_t *, u32)</code>
</li>
</ul>
</details>
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
<code>void (*decode_session)(struct sk_buff *, struct flowi *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*get_tos)(const struct flowi *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*init_path)(struct xfrm_dst *, struct dst_entry *, int)</code>
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
