# Struct: <code>xfrm_mgr</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct xfrm_mgr {
    struct list_head list;
    char *id;
    int (*notify)(struct xfrm_state *, const struct km_event *);
    int (*acquire)(struct xfrm_state *, struct xfrm_tmpl *, struct xfrm_policy *);
    struct xfrm_policy * (*compile_policy)(struct sock *, int, u8 *, int, int *);
    int (*new_mapping)(struct xfrm_state *, xfrm_address_t *, __be16);
    int (*notify_policy)(struct xfrm_policy *, int, const struct km_event *);
    int (*report)(struct net *, u8, struct xfrm_selector *, xfrm_address_t *);
    int (*migrate)(const struct xfrm_selector *, u8, u8, const struct xfrm_migrate *, int, const struct xfrm_kmaddress *);
    bool (*is_alive)(const struct km_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct xfrm_mgr {
    struct list_head list;
    char *id;
    int (*notify)(struct xfrm_state *, const struct km_event *);
    int (*acquire)(struct xfrm_state *, struct xfrm_tmpl *, struct xfrm_policy *);
    struct xfrm_policy * (*compile_policy)(struct sock *, int, u8 *, int, int *);
    int (*new_mapping)(struct xfrm_state *, xfrm_address_t *, __be16);
    int (*notify_policy)(struct xfrm_policy *, int, const struct km_event *);
    int (*report)(struct net *, u8, struct xfrm_selector *, xfrm_address_t *);
    int (*migrate)(const struct xfrm_selector *, u8, u8, const struct xfrm_migrate *, int, const struct xfrm_kmaddress *);
    bool (*is_alive)(const struct km_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct xfrm_mgr {
    struct list_head list;
    char *id;
    int (*notify)(struct xfrm_state *, const struct km_event *);
    int (*acquire)(struct xfrm_state *, struct xfrm_tmpl *, struct xfrm_policy *);
    struct xfrm_policy * (*compile_policy)(struct sock *, int, u8 *, int, int *);
    int (*new_mapping)(struct xfrm_state *, xfrm_address_t *, __be16);
    int (*notify_policy)(struct xfrm_policy *, int, const struct km_event *);
    int (*report)(struct net *, u8, struct xfrm_selector *, xfrm_address_t *);
    int (*migrate)(const struct xfrm_selector *, u8, u8, const struct xfrm_migrate *, int, const struct xfrm_kmaddress *);
    bool (*is_alive)(const struct km_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct xfrm_mgr {
    struct list_head list;
    int (*notify)(struct xfrm_state *, const struct km_event *);
    int (*acquire)(struct xfrm_state *, struct xfrm_tmpl *, struct xfrm_policy *);
    struct xfrm_policy * (*compile_policy)(struct sock *, int, u8 *, int, int *);
    int (*new_mapping)(struct xfrm_state *, xfrm_address_t *, __be16);
    int (*notify_policy)(struct xfrm_policy *, int, const struct km_event *);
    int (*report)(struct net *, u8, struct xfrm_selector *, xfrm_address_t *);
    int (*migrate)(const struct xfrm_selector *, u8, u8, const struct xfrm_migrate *, int, const struct xfrm_kmaddress *, const struct xfrm_encap_tmpl *);
    bool (*is_alive)(const struct km_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct xfrm_mgr {
    struct list_head list;
    int (*notify)(struct xfrm_state *, const struct km_event *);
    int (*acquire)(struct xfrm_state *, struct xfrm_tmpl *, struct xfrm_policy *);
    struct xfrm_policy * (*compile_policy)(struct sock *, int, u8 *, int, int *);
    int (*new_mapping)(struct xfrm_state *, xfrm_address_t *, __be16);
    int (*notify_policy)(struct xfrm_policy *, int, const struct km_event *);
    int (*report)(struct net *, u8, struct xfrm_selector *, xfrm_address_t *);
    int (*migrate)(const struct xfrm_selector *, u8, u8, const struct xfrm_migrate *, int, const struct xfrm_kmaddress *, const struct xfrm_encap_tmpl *);
    bool (*is_alive)(const struct km_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct xfrm_mgr {
    struct list_head list;
    int (*notify)(struct xfrm_state *, const struct km_event *);
    int (*acquire)(struct xfrm_state *, struct xfrm_tmpl *, struct xfrm_policy *);
    struct xfrm_policy * (*compile_policy)(struct sock *, int, u8 *, int, int *);
    int (*new_mapping)(struct xfrm_state *, xfrm_address_t *, __be16);
    int (*notify_policy)(struct xfrm_policy *, int, const struct km_event *);
    int (*report)(struct net *, u8, struct xfrm_selector *, xfrm_address_t *);
    int (*migrate)(const struct xfrm_selector *, u8, u8, const struct xfrm_migrate *, int, const struct xfrm_kmaddress *, const struct xfrm_encap_tmpl *);
    bool (*is_alive)(const struct km_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct xfrm_mgr {
    struct list_head list;
    int (*notify)(struct xfrm_state *, const struct km_event *);
    int (*acquire)(struct xfrm_state *, struct xfrm_tmpl *, struct xfrm_policy *);
    struct xfrm_policy * (*compile_policy)(struct sock *, int, u8 *, int, int *);
    int (*new_mapping)(struct xfrm_state *, xfrm_address_t *, __be16);
    int (*notify_policy)(struct xfrm_policy *, int, const struct km_event *);
    int (*report)(struct net *, u8, struct xfrm_selector *, xfrm_address_t *);
    int (*migrate)(const struct xfrm_selector *, u8, u8, const struct xfrm_migrate *, int, const struct xfrm_kmaddress *, const struct xfrm_encap_tmpl *);
    bool (*is_alive)(const struct km_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct xfrm_mgr {
    struct list_head list;
    int (*notify)(struct xfrm_state *, const struct km_event *);
    int (*acquire)(struct xfrm_state *, struct xfrm_tmpl *, struct xfrm_policy *);
    struct xfrm_policy * (*compile_policy)(struct sock *, int, u8 *, int, int *);
    int (*new_mapping)(struct xfrm_state *, xfrm_address_t *, __be16);
    int (*notify_policy)(struct xfrm_policy *, int, const struct km_event *);
    int (*report)(struct net *, u8, struct xfrm_selector *, xfrm_address_t *);
    int (*migrate)(const struct xfrm_selector *, u8, u8, const struct xfrm_migrate *, int, const struct xfrm_kmaddress *, const struct xfrm_encap_tmpl *);
    bool (*is_alive)(const struct km_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct xfrm_mgr {
    struct list_head list;
    int (*notify)(struct xfrm_state *, const struct km_event *);
    int (*acquire)(struct xfrm_state *, struct xfrm_tmpl *, struct xfrm_policy *);
    struct xfrm_policy * (*compile_policy)(struct sock *, int, u8 *, int, int *);
    int (*new_mapping)(struct xfrm_state *, xfrm_address_t *, __be16);
    int (*notify_policy)(struct xfrm_policy *, int, const struct km_event *);
    int (*report)(struct net *, u8, struct xfrm_selector *, xfrm_address_t *);
    int (*migrate)(const struct xfrm_selector *, u8, u8, const struct xfrm_migrate *, int, const struct xfrm_kmaddress *, const struct xfrm_encap_tmpl *);
    bool (*is_alive)(const struct km_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct xfrm_mgr {
    struct list_head list;
    int (*notify)(struct xfrm_state *, const struct km_event *);
    int (*acquire)(struct xfrm_state *, struct xfrm_tmpl *, struct xfrm_policy *);
    struct xfrm_policy * (*compile_policy)(struct sock *, int, u8 *, int, int *);
    int (*new_mapping)(struct xfrm_state *, xfrm_address_t *, __be16);
    int (*notify_policy)(struct xfrm_policy *, int, const struct km_event *);
    int (*report)(struct net *, u8, struct xfrm_selector *, xfrm_address_t *);
    int (*migrate)(const struct xfrm_selector *, u8, u8, const struct xfrm_migrate *, int, const struct xfrm_kmaddress *, const struct xfrm_encap_tmpl *);
    bool (*is_alive)(const struct km_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct xfrm_mgr {
    struct list_head list;
    int (*notify)(struct xfrm_state *, const struct km_event *);
    int (*acquire)(struct xfrm_state *, struct xfrm_tmpl *, struct xfrm_policy *);
    struct xfrm_policy * (*compile_policy)(struct sock *, int, u8 *, int, int *);
    int (*new_mapping)(struct xfrm_state *, xfrm_address_t *, __be16);
    int (*notify_policy)(struct xfrm_policy *, int, const struct km_event *);
    int (*report)(struct net *, u8, struct xfrm_selector *, xfrm_address_t *);
    int (*migrate)(const struct xfrm_selector *, u8, u8, const struct xfrm_migrate *, int, const struct xfrm_kmaddress *, const struct xfrm_encap_tmpl *);
    bool (*is_alive)(const struct km_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct xfrm_mgr {
    struct list_head list;
    int (*notify)(struct xfrm_state *, const struct km_event *);
    int (*acquire)(struct xfrm_state *, struct xfrm_tmpl *, struct xfrm_policy *);
    struct xfrm_policy * (*compile_policy)(struct sock *, int, u8 *, int, int *);
    int (*new_mapping)(struct xfrm_state *, xfrm_address_t *, __be16);
    int (*notify_policy)(struct xfrm_policy *, int, const struct km_event *);
    int (*report)(struct net *, u8, struct xfrm_selector *, xfrm_address_t *);
    int (*migrate)(const struct xfrm_selector *, u8, u8, const struct xfrm_migrate *, int, const struct xfrm_kmaddress *, const struct xfrm_encap_tmpl *);
    bool (*is_alive)(const struct km_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct xfrm_mgr {
    struct list_head list;
    int (*notify)(struct xfrm_state *, const struct km_event *);
    int (*acquire)(struct xfrm_state *, struct xfrm_tmpl *, struct xfrm_policy *);
    struct xfrm_policy * (*compile_policy)(struct sock *, int, u8 *, int, int *);
    int (*new_mapping)(struct xfrm_state *, xfrm_address_t *, __be16);
    int (*notify_policy)(struct xfrm_policy *, int, const struct km_event *);
    int (*report)(struct net *, u8, struct xfrm_selector *, xfrm_address_t *);
    int (*migrate)(const struct xfrm_selector *, u8, u8, const struct xfrm_migrate *, int, const struct xfrm_kmaddress *, const struct xfrm_encap_tmpl *);
    bool (*is_alive)(const struct km_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct xfrm_mgr {
    struct list_head list;
    int (*notify)(struct xfrm_state *, const struct km_event *);
    int (*acquire)(struct xfrm_state *, struct xfrm_tmpl *, struct xfrm_policy *);
    struct xfrm_policy * (*compile_policy)(struct sock *, int, u8 *, int, int *);
    int (*new_mapping)(struct xfrm_state *, xfrm_address_t *, __be16);
    int (*notify_policy)(struct xfrm_policy *, int, const struct km_event *);
    int (*report)(struct net *, u8, struct xfrm_selector *, xfrm_address_t *);
    int (*migrate)(const struct xfrm_selector *, u8, u8, const struct xfrm_migrate *, int, const struct xfrm_kmaddress *, const struct xfrm_encap_tmpl *);
    bool (*is_alive)(const struct km_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct xfrm_mgr {
    struct list_head list;
    int (*notify)(struct xfrm_state *, const struct km_event *);
    int (*acquire)(struct xfrm_state *, struct xfrm_tmpl *, struct xfrm_policy *);
    struct xfrm_policy * (*compile_policy)(struct sock *, int, u8 *, int, int *);
    int (*new_mapping)(struct xfrm_state *, xfrm_address_t *, __be16);
    int (*notify_policy)(struct xfrm_policy *, int, const struct km_event *);
    int (*report)(struct net *, u8, struct xfrm_selector *, xfrm_address_t *);
    int (*migrate)(const struct xfrm_selector *, u8, u8, const struct xfrm_migrate *, int, const struct xfrm_kmaddress *, const struct xfrm_encap_tmpl *);
    bool (*is_alive)(const struct km_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct xfrm_mgr {
    struct list_head list;
    int (*notify)(struct xfrm_state *, const struct km_event *);
    int (*acquire)(struct xfrm_state *, struct xfrm_tmpl *, struct xfrm_policy *);
    struct xfrm_policy * (*compile_policy)(struct sock *, int, u8 *, int, int *);
    int (*new_mapping)(struct xfrm_state *, xfrm_address_t *, __be16);
    int (*notify_policy)(struct xfrm_policy *, int, const struct km_event *);
    int (*report)(struct net *, u8, struct xfrm_selector *, xfrm_address_t *);
    int (*migrate)(const struct xfrm_selector *, u8, u8, const struct xfrm_migrate *, int, const struct xfrm_kmaddress *, const struct xfrm_encap_tmpl *);
    bool (*is_alive)(const struct km_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct xfrm_mgr {
    struct list_head list;
    int (*notify)(struct xfrm_state *, const struct km_event *);
    int (*acquire)(struct xfrm_state *, struct xfrm_tmpl *, struct xfrm_policy *);
    struct xfrm_policy * (*compile_policy)(struct sock *, int, u8 *, int, int *);
    int (*new_mapping)(struct xfrm_state *, xfrm_address_t *, __be16);
    int (*notify_policy)(struct xfrm_policy *, int, const struct km_event *);
    int (*report)(struct net *, u8, struct xfrm_selector *, xfrm_address_t *);
    int (*migrate)(const struct xfrm_selector *, u8, u8, const struct xfrm_migrate *, int, const struct xfrm_kmaddress *, const struct xfrm_encap_tmpl *);
    bool (*is_alive)(const struct km_event *);
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
struct xfrm_mgr {
    struct list_head list;
    int (*notify)(struct xfrm_state *, const struct km_event *);
    int (*acquire)(struct xfrm_state *, struct xfrm_tmpl *, struct xfrm_policy *);
    struct xfrm_policy * (*compile_policy)(struct sock *, int, u8 *, int, int *);
    int (*new_mapping)(struct xfrm_state *, xfrm_address_t *, __be16);
    int (*notify_policy)(struct xfrm_policy *, int, const struct km_event *);
    int (*report)(struct net *, u8, struct xfrm_selector *, xfrm_address_t *);
    int (*migrate)(const struct xfrm_selector *, u8, u8, const struct xfrm_migrate *, int, const struct xfrm_kmaddress *, const struct xfrm_encap_tmpl *);
    bool (*is_alive)(const struct km_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct xfrm_mgr {
    struct list_head list;
    int (*notify)(struct xfrm_state *, const struct km_event *);
    int (*acquire)(struct xfrm_state *, struct xfrm_tmpl *, struct xfrm_policy *);
    struct xfrm_policy * (*compile_policy)(struct sock *, int, u8 *, int, int *);
    int (*new_mapping)(struct xfrm_state *, xfrm_address_t *, __be16);
    int (*notify_policy)(struct xfrm_policy *, int, const struct km_event *);
    int (*report)(struct net *, u8, struct xfrm_selector *, xfrm_address_t *);
    int (*migrate)(const struct xfrm_selector *, u8, u8, const struct xfrm_migrate *, int, const struct xfrm_kmaddress *, const struct xfrm_encap_tmpl *);
    bool (*is_alive)(const struct km_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct xfrm_mgr {
    struct list_head list;
    int (*notify)(struct xfrm_state *, const struct km_event *);
    int (*acquire)(struct xfrm_state *, struct xfrm_tmpl *, struct xfrm_policy *);
    struct xfrm_policy * (*compile_policy)(struct sock *, int, u8 *, int, int *);
    int (*new_mapping)(struct xfrm_state *, xfrm_address_t *, __be16);
    int (*notify_policy)(struct xfrm_policy *, int, const struct km_event *);
    int (*report)(struct net *, u8, struct xfrm_selector *, xfrm_address_t *);
    int (*migrate)(const struct xfrm_selector *, u8, u8, const struct xfrm_migrate *, int, const struct xfrm_kmaddress *, const struct xfrm_encap_tmpl *);
    bool (*is_alive)(const struct km_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct xfrm_mgr {
    struct list_head list;
    int (*notify)(struct xfrm_state *, const struct km_event *);
    int (*acquire)(struct xfrm_state *, struct xfrm_tmpl *, struct xfrm_policy *);
    struct xfrm_policy * (*compile_policy)(struct sock *, int, u8 *, int, int *);
    int (*new_mapping)(struct xfrm_state *, xfrm_address_t *, __be16);
    int (*notify_policy)(struct xfrm_policy *, int, const struct km_event *);
    int (*report)(struct net *, u8, struct xfrm_selector *, xfrm_address_t *);
    int (*migrate)(const struct xfrm_selector *, u8, u8, const struct xfrm_migrate *, int, const struct xfrm_kmaddress *, const struct xfrm_encap_tmpl *);
    bool (*is_alive)(const struct km_event *);
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
struct xfrm_mgr {
    struct list_head list;
    int (*notify)(struct xfrm_state *, const struct km_event *);
    int (*acquire)(struct xfrm_state *, struct xfrm_tmpl *, struct xfrm_policy *);
    struct xfrm_policy * (*compile_policy)(struct sock *, int, u8 *, int, int *);
    int (*new_mapping)(struct xfrm_state *, xfrm_address_t *, __be16);
    int (*notify_policy)(struct xfrm_policy *, int, const struct km_event *);
    int (*report)(struct net *, u8, struct xfrm_selector *, xfrm_address_t *);
    int (*migrate)(const struct xfrm_selector *, u8, u8, const struct xfrm_migrate *, int, const struct xfrm_kmaddress *, const struct xfrm_encap_tmpl *);
    bool (*is_alive)(const struct km_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct xfrm_mgr {
    struct list_head list;
    int (*notify)(struct xfrm_state *, const struct km_event *);
    int (*acquire)(struct xfrm_state *, struct xfrm_tmpl *, struct xfrm_policy *);
    struct xfrm_policy * (*compile_policy)(struct sock *, int, u8 *, int, int *);
    int (*new_mapping)(struct xfrm_state *, xfrm_address_t *, __be16);
    int (*notify_policy)(struct xfrm_policy *, int, const struct km_event *);
    int (*report)(struct net *, u8, struct xfrm_selector *, xfrm_address_t *);
    int (*migrate)(const struct xfrm_selector *, u8, u8, const struct xfrm_migrate *, int, const struct xfrm_kmaddress *, const struct xfrm_encap_tmpl *);
    bool (*is_alive)(const struct km_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct xfrm_mgr {
    struct list_head list;
    int (*notify)(struct xfrm_state *, const struct km_event *);
    int (*acquire)(struct xfrm_state *, struct xfrm_tmpl *, struct xfrm_policy *);
    struct xfrm_policy * (*compile_policy)(struct sock *, int, u8 *, int, int *);
    int (*new_mapping)(struct xfrm_state *, xfrm_address_t *, __be16);
    int (*notify_policy)(struct xfrm_policy *, int, const struct km_event *);
    int (*report)(struct net *, u8, struct xfrm_selector *, xfrm_address_t *);
    int (*migrate)(const struct xfrm_selector *, u8, u8, const struct xfrm_migrate *, int, const struct xfrm_kmaddress *, const struct xfrm_encap_tmpl *);
    bool (*is_alive)(const struct km_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct xfrm_mgr {
    struct list_head list;
    int (*notify)(struct xfrm_state *, const struct km_event *);
    int (*acquire)(struct xfrm_state *, struct xfrm_tmpl *, struct xfrm_policy *);
    struct xfrm_policy * (*compile_policy)(struct sock *, int, u8 *, int, int *);
    int (*new_mapping)(struct xfrm_state *, xfrm_address_t *, __be16);
    int (*notify_policy)(struct xfrm_policy *, int, const struct km_event *);
    int (*report)(struct net *, u8, struct xfrm_selector *, xfrm_address_t *);
    int (*migrate)(const struct xfrm_selector *, u8, u8, const struct xfrm_migrate *, int, const struct xfrm_kmaddress *, const struct xfrm_encap_tmpl *);
    bool (*is_alive)(const struct km_event *);
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
<code>char *id</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*migrate)(const struct xfrm_selector *, u8, u8, const struct xfrm_migrate *, int, const struct xfrm_kmaddress *)</code> ➡️ <code>int (*migrate)(const struct xfrm_selector *, u8, u8, const struct xfrm_migrate *, int, const struct xfrm_kmaddress *, const struct xfrm_encap_tmpl *)</code>
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
