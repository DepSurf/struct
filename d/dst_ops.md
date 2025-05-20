# Struct: <code>dst_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct dst_ops {
    short unsigned int family;
    unsigned int gc_thresh;
    int (*gc)(struct dst_ops *);
    struct dst_entry * (*check)(struct dst_entry *, __u32);
    unsigned int (*default_advmss)(const struct dst_entry *);
    unsigned int (*mtu)(const struct dst_entry *);
    u32 * (*cow_metrics)(struct dst_entry *, long unsigned int);
    void (*destroy)(struct dst_entry *);
    void (*ifdown)(struct dst_entry *, struct net_device *, int);
    struct dst_entry * (*negative_advice)(struct dst_entry *);
    void (*link_failure)(struct sk_buff *);
    void (*update_pmtu)(struct dst_entry *, struct sock *, struct sk_buff *, u32);
    void (*redirect)(struct dst_entry *, struct sock *, struct sk_buff *);
    int (*local_out)(struct net *, struct sock *, struct sk_buff *);
    struct neighbour * (*neigh_lookup)(const struct dst_entry *, struct sk_buff *, const void *);
    struct kmem_cache *kmem_cachep;
    struct percpu_counter pcpuc_entries;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct dst_ops {
    short unsigned int family;
    unsigned int gc_thresh;
    int (*gc)(struct dst_ops *);
    struct dst_entry * (*check)(struct dst_entry *, __u32);
    unsigned int (*default_advmss)(const struct dst_entry *);
    unsigned int (*mtu)(const struct dst_entry *);
    u32 * (*cow_metrics)(struct dst_entry *, long unsigned int);
    void (*destroy)(struct dst_entry *);
    void (*ifdown)(struct dst_entry *, struct net_device *, int);
    struct dst_entry * (*negative_advice)(struct dst_entry *);
    void (*link_failure)(struct sk_buff *);
    void (*update_pmtu)(struct dst_entry *, struct sock *, struct sk_buff *, u32);
    void (*redirect)(struct dst_entry *, struct sock *, struct sk_buff *);
    int (*local_out)(struct net *, struct sock *, struct sk_buff *);
    struct neighbour * (*neigh_lookup)(const struct dst_entry *, struct sk_buff *, const void *);
    struct kmem_cache *kmem_cachep;
    struct percpu_counter pcpuc_entries;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct dst_ops {
    short unsigned int family;
    unsigned int gc_thresh;
    int (*gc)(struct dst_ops *);
    struct dst_entry * (*check)(struct dst_entry *, __u32);
    unsigned int (*default_advmss)(const struct dst_entry *);
    unsigned int (*mtu)(const struct dst_entry *);
    u32 * (*cow_metrics)(struct dst_entry *, long unsigned int);
    void (*destroy)(struct dst_entry *);
    void (*ifdown)(struct dst_entry *, struct net_device *, int);
    struct dst_entry * (*negative_advice)(struct dst_entry *);
    void (*link_failure)(struct sk_buff *);
    void (*update_pmtu)(struct dst_entry *, struct sock *, struct sk_buff *, u32);
    void (*redirect)(struct dst_entry *, struct sock *, struct sk_buff *);
    int (*local_out)(struct net *, struct sock *, struct sk_buff *);
    struct neighbour * (*neigh_lookup)(const struct dst_entry *, struct sk_buff *, const void *);
    struct kmem_cache *kmem_cachep;
    struct percpu_counter pcpuc_entries;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct dst_ops {
    short unsigned int family;
    unsigned int gc_thresh;
    int (*gc)(struct dst_ops *);
    struct dst_entry * (*check)(struct dst_entry *, __u32);
    unsigned int (*default_advmss)(const struct dst_entry *);
    unsigned int (*mtu)(const struct dst_entry *);
    u32 * (*cow_metrics)(struct dst_entry *, long unsigned int);
    void (*destroy)(struct dst_entry *);
    void (*ifdown)(struct dst_entry *, struct net_device *, int);
    struct dst_entry * (*negative_advice)(struct dst_entry *);
    void (*link_failure)(struct sk_buff *);
    void (*update_pmtu)(struct dst_entry *, struct sock *, struct sk_buff *, u32);
    void (*redirect)(struct dst_entry *, struct sock *, struct sk_buff *);
    int (*local_out)(struct net *, struct sock *, struct sk_buff *);
    struct neighbour * (*neigh_lookup)(const struct dst_entry *, struct sk_buff *, const void *);
    void (*confirm_neigh)(const struct dst_entry *, const void *);
    struct kmem_cache *kmem_cachep;
    struct percpu_counter pcpuc_entries;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dst_ops {
    short unsigned int family;
    unsigned int gc_thresh;
    int (*gc)(struct dst_ops *);
    struct dst_entry * (*check)(struct dst_entry *, __u32);
    unsigned int (*default_advmss)(const struct dst_entry *);
    unsigned int (*mtu)(const struct dst_entry *);
    u32 * (*cow_metrics)(struct dst_entry *, long unsigned int);
    void (*destroy)(struct dst_entry *);
    void (*ifdown)(struct dst_entry *, struct net_device *, int);
    struct dst_entry * (*negative_advice)(struct dst_entry *);
    void (*link_failure)(struct sk_buff *);
    void (*update_pmtu)(struct dst_entry *, struct sock *, struct sk_buff *, u32);
    void (*redirect)(struct dst_entry *, struct sock *, struct sk_buff *);
    int (*local_out)(struct net *, struct sock *, struct sk_buff *);
    struct neighbour * (*neigh_lookup)(const struct dst_entry *, struct sk_buff *, const void *);
    void (*confirm_neigh)(const struct dst_entry *, const void *);
    struct kmem_cache *kmem_cachep;
    struct percpu_counter pcpuc_entries;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dst_ops {
    short unsigned int family;
    unsigned int gc_thresh;
    int (*gc)(struct dst_ops *);
    struct dst_entry * (*check)(struct dst_entry *, __u32);
    unsigned int (*default_advmss)(const struct dst_entry *);
    unsigned int (*mtu)(const struct dst_entry *);
    u32 * (*cow_metrics)(struct dst_entry *, long unsigned int);
    void (*destroy)(struct dst_entry *);
    void (*ifdown)(struct dst_entry *, struct net_device *, int);
    struct dst_entry * (*negative_advice)(struct dst_entry *);
    void (*link_failure)(struct sk_buff *);
    void (*update_pmtu)(struct dst_entry *, struct sock *, struct sk_buff *, u32);
    void (*redirect)(struct dst_entry *, struct sock *, struct sk_buff *);
    int (*local_out)(struct net *, struct sock *, struct sk_buff *);
    struct neighbour * (*neigh_lookup)(const struct dst_entry *, struct sk_buff *, const void *);
    void (*confirm_neigh)(const struct dst_entry *, const void *);
    struct kmem_cache *kmem_cachep;
    struct percpu_counter pcpuc_entries;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dst_ops {
    short unsigned int family;
    unsigned int gc_thresh;
    int (*gc)(struct dst_ops *);
    struct dst_entry * (*check)(struct dst_entry *, __u32);
    unsigned int (*default_advmss)(const struct dst_entry *);
    unsigned int (*mtu)(const struct dst_entry *);
    u32 * (*cow_metrics)(struct dst_entry *, long unsigned int);
    void (*destroy)(struct dst_entry *);
    void (*ifdown)(struct dst_entry *, struct net_device *, int);
    struct dst_entry * (*negative_advice)(struct dst_entry *);
    void (*link_failure)(struct sk_buff *);
    void (*update_pmtu)(struct dst_entry *, struct sock *, struct sk_buff *, u32);
    void (*redirect)(struct dst_entry *, struct sock *, struct sk_buff *);
    int (*local_out)(struct net *, struct sock *, struct sk_buff *);
    struct neighbour * (*neigh_lookup)(const struct dst_entry *, struct sk_buff *, const void *);
    void (*confirm_neigh)(const struct dst_entry *, const void *);
    struct kmem_cache *kmem_cachep;
    struct percpu_counter pcpuc_entries;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dst_ops {
    short unsigned int family;
    unsigned int gc_thresh;
    int (*gc)(struct dst_ops *);
    struct dst_entry * (*check)(struct dst_entry *, __u32);
    unsigned int (*default_advmss)(const struct dst_entry *);
    unsigned int (*mtu)(const struct dst_entry *);
    u32 * (*cow_metrics)(struct dst_entry *, long unsigned int);
    void (*destroy)(struct dst_entry *);
    void (*ifdown)(struct dst_entry *, struct net_device *, int);
    struct dst_entry * (*negative_advice)(struct dst_entry *);
    void (*link_failure)(struct sk_buff *);
    void (*update_pmtu)(struct dst_entry *, struct sock *, struct sk_buff *, u32);
    void (*redirect)(struct dst_entry *, struct sock *, struct sk_buff *);
    int (*local_out)(struct net *, struct sock *, struct sk_buff *);
    struct neighbour * (*neigh_lookup)(const struct dst_entry *, struct sk_buff *, const void *);
    void (*confirm_neigh)(const struct dst_entry *, const void *);
    struct kmem_cache *kmem_cachep;
    struct percpu_counter pcpuc_entries;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dst_ops {
    short unsigned int family;
    unsigned int gc_thresh;
    int (*gc)(struct dst_ops *);
    struct dst_entry * (*check)(struct dst_entry *, __u32);
    unsigned int (*default_advmss)(const struct dst_entry *);
    unsigned int (*mtu)(const struct dst_entry *);
    u32 * (*cow_metrics)(struct dst_entry *, long unsigned int);
    void (*destroy)(struct dst_entry *);
    void (*ifdown)(struct dst_entry *, struct net_device *, int);
    struct dst_entry * (*negative_advice)(struct dst_entry *);
    void (*link_failure)(struct sk_buff *);
    void (*update_pmtu)(struct dst_entry *, struct sock *, struct sk_buff *, u32, bool);
    void (*redirect)(struct dst_entry *, struct sock *, struct sk_buff *);
    int (*local_out)(struct net *, struct sock *, struct sk_buff *);
    struct neighbour * (*neigh_lookup)(const struct dst_entry *, struct sk_buff *, const void *);
    void (*confirm_neigh)(const struct dst_entry *, const void *);
    struct kmem_cache *kmem_cachep;
    struct percpu_counter pcpuc_entries;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dst_ops {
    short unsigned int family;
    unsigned int gc_thresh;
    int (*gc)(struct dst_ops *);
    struct dst_entry * (*check)(struct dst_entry *, __u32);
    unsigned int (*default_advmss)(const struct dst_entry *);
    unsigned int (*mtu)(const struct dst_entry *);
    u32 * (*cow_metrics)(struct dst_entry *, long unsigned int);
    void (*destroy)(struct dst_entry *);
    void (*ifdown)(struct dst_entry *, struct net_device *, int);
    struct dst_entry * (*negative_advice)(struct dst_entry *);
    void (*link_failure)(struct sk_buff *);
    void (*update_pmtu)(struct dst_entry *, struct sock *, struct sk_buff *, u32, bool);
    void (*redirect)(struct dst_entry *, struct sock *, struct sk_buff *);
    int (*local_out)(struct net *, struct sock *, struct sk_buff *);
    struct neighbour * (*neigh_lookup)(const struct dst_entry *, struct sk_buff *, const void *);
    void (*confirm_neigh)(const struct dst_entry *, const void *);
    struct kmem_cache *kmem_cachep;
    struct percpu_counter pcpuc_entries;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dst_ops {
    short unsigned int family;
    unsigned int gc_thresh;
    int (*gc)(struct dst_ops *);
    struct dst_entry * (*check)(struct dst_entry *, __u32);
    unsigned int (*default_advmss)(const struct dst_entry *);
    unsigned int (*mtu)(const struct dst_entry *);
    u32 * (*cow_metrics)(struct dst_entry *, long unsigned int);
    void (*destroy)(struct dst_entry *);
    void (*ifdown)(struct dst_entry *, struct net_device *, int);
    struct dst_entry * (*negative_advice)(struct dst_entry *);
    void (*link_failure)(struct sk_buff *);
    void (*update_pmtu)(struct dst_entry *, struct sock *, struct sk_buff *, u32, bool);
    void (*redirect)(struct dst_entry *, struct sock *, struct sk_buff *);
    int (*local_out)(struct net *, struct sock *, struct sk_buff *);
    struct neighbour * (*neigh_lookup)(const struct dst_entry *, struct sk_buff *, const void *);
    void (*confirm_neigh)(const struct dst_entry *, const void *);
    struct kmem_cache *kmem_cachep;
    struct percpu_counter pcpuc_entries;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dst_ops {
    short unsigned int family;
    unsigned int gc_thresh;
    int (*gc)(struct dst_ops *);
    struct dst_entry * (*check)(struct dst_entry *, __u32);
    unsigned int (*default_advmss)(const struct dst_entry *);
    unsigned int (*mtu)(const struct dst_entry *);
    u32 * (*cow_metrics)(struct dst_entry *, long unsigned int);
    void (*destroy)(struct dst_entry *);
    void (*ifdown)(struct dst_entry *, struct net_device *, int);
    struct dst_entry * (*negative_advice)(struct dst_entry *);
    void (*link_failure)(struct sk_buff *);
    void (*update_pmtu)(struct dst_entry *, struct sock *, struct sk_buff *, u32, bool);
    void (*redirect)(struct dst_entry *, struct sock *, struct sk_buff *);
    int (*local_out)(struct net *, struct sock *, struct sk_buff *);
    struct neighbour * (*neigh_lookup)(const struct dst_entry *, struct sk_buff *, const void *);
    void (*confirm_neigh)(const struct dst_entry *, const void *);
    struct kmem_cache *kmem_cachep;
    struct percpu_counter pcpuc_entries;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dst_ops {
    short unsigned int family;
    unsigned int gc_thresh;
    int (*gc)(struct dst_ops *);
    struct dst_entry * (*check)(struct dst_entry *, __u32);
    unsigned int (*default_advmss)(const struct dst_entry *);
    unsigned int (*mtu)(const struct dst_entry *);
    u32 * (*cow_metrics)(struct dst_entry *, long unsigned int);
    void (*destroy)(struct dst_entry *);
    void (*ifdown)(struct dst_entry *, struct net_device *, int);
    struct dst_entry * (*negative_advice)(struct dst_entry *);
    void (*link_failure)(struct sk_buff *);
    void (*update_pmtu)(struct dst_entry *, struct sock *, struct sk_buff *, u32, bool);
    void (*redirect)(struct dst_entry *, struct sock *, struct sk_buff *);
    int (*local_out)(struct net *, struct sock *, struct sk_buff *);
    struct neighbour * (*neigh_lookup)(const struct dst_entry *, struct sk_buff *, const void *);
    void (*confirm_neigh)(const struct dst_entry *, const void *);
    struct kmem_cache *kmem_cachep;
    struct percpu_counter pcpuc_entries;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dst_ops {
    short unsigned int family;
    unsigned int gc_thresh;
    int (*gc)(struct dst_ops *);
    struct dst_entry * (*check)(struct dst_entry *, __u32);
    unsigned int (*default_advmss)(const struct dst_entry *);
    unsigned int (*mtu)(const struct dst_entry *);
    u32 * (*cow_metrics)(struct dst_entry *, long unsigned int);
    void (*destroy)(struct dst_entry *);
    void (*ifdown)(struct dst_entry *, struct net_device *, int);
    struct dst_entry * (*negative_advice)(struct dst_entry *);
    void (*link_failure)(struct sk_buff *);
    void (*update_pmtu)(struct dst_entry *, struct sock *, struct sk_buff *, u32, bool);
    void (*redirect)(struct dst_entry *, struct sock *, struct sk_buff *);
    int (*local_out)(struct net *, struct sock *, struct sk_buff *);
    struct neighbour * (*neigh_lookup)(const struct dst_entry *, struct sk_buff *, const void *);
    void (*confirm_neigh)(const struct dst_entry *, const void *);
    struct kmem_cache *kmem_cachep;
    struct percpu_counter pcpuc_entries;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dst_ops {
    short unsigned int family;
    unsigned int gc_thresh;
    int (*gc)(struct dst_ops *);
    struct dst_entry * (*check)(struct dst_entry *, __u32);
    unsigned int (*default_advmss)(const struct dst_entry *);
    unsigned int (*mtu)(const struct dst_entry *);
    u32 * (*cow_metrics)(struct dst_entry *, long unsigned int);
    void (*destroy)(struct dst_entry *);
    void (*ifdown)(struct dst_entry *, struct net_device *, int);
    struct dst_entry * (*negative_advice)(struct dst_entry *);
    void (*link_failure)(struct sk_buff *);
    void (*update_pmtu)(struct dst_entry *, struct sock *, struct sk_buff *, u32, bool);
    void (*redirect)(struct dst_entry *, struct sock *, struct sk_buff *);
    int (*local_out)(struct net *, struct sock *, struct sk_buff *);
    struct neighbour * (*neigh_lookup)(const struct dst_entry *, struct sk_buff *, const void *);
    void (*confirm_neigh)(const struct dst_entry *, const void *);
    struct kmem_cache *kmem_cachep;
    struct percpu_counter pcpuc_entries;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dst_ops {
    short unsigned int family;
    unsigned int gc_thresh;
    void (*gc)(struct dst_ops *);
    struct dst_entry * (*check)(struct dst_entry *, __u32);
    unsigned int (*default_advmss)(const struct dst_entry *);
    unsigned int (*mtu)(const struct dst_entry *);
    u32 * (*cow_metrics)(struct dst_entry *, long unsigned int);
    void (*destroy)(struct dst_entry *);
    void (*ifdown)(struct dst_entry *, struct net_device *, int);
    struct dst_entry * (*negative_advice)(struct dst_entry *);
    void (*link_failure)(struct sk_buff *);
    void (*update_pmtu)(struct dst_entry *, struct sock *, struct sk_buff *, u32, bool);
    void (*redirect)(struct dst_entry *, struct sock *, struct sk_buff *);
    int (*local_out)(struct net *, struct sock *, struct sk_buff *);
    struct neighbour * (*neigh_lookup)(const struct dst_entry *, struct sk_buff *, const void *);
    void (*confirm_neigh)(const struct dst_entry *, const void *);
    struct kmem_cache *kmem_cachep;
    struct percpu_counter pcpuc_entries;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dst_ops {
    short unsigned int family;
    unsigned int gc_thresh;
    void (*gc)(struct dst_ops *);
    struct dst_entry * (*check)(struct dst_entry *, __u32);
    unsigned int (*default_advmss)(const struct dst_entry *);
    unsigned int (*mtu)(const struct dst_entry *);
    u32 * (*cow_metrics)(struct dst_entry *, long unsigned int);
    void (*destroy)(struct dst_entry *);
    void (*ifdown)(struct dst_entry *, struct net_device *);
    struct dst_entry * (*negative_advice)(struct dst_entry *);
    void (*link_failure)(struct sk_buff *);
    void (*update_pmtu)(struct dst_entry *, struct sock *, struct sk_buff *, u32, bool);
    void (*redirect)(struct dst_entry *, struct sock *, struct sk_buff *);
    int (*local_out)(struct net *, struct sock *, struct sk_buff *);
    struct neighbour * (*neigh_lookup)(const struct dst_entry *, struct sk_buff *, const void *);
    void (*confirm_neigh)(const struct dst_entry *, const void *);
    struct kmem_cache *kmem_cachep;
    struct percpu_counter pcpuc_entries;
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
struct dst_ops {
    short unsigned int family;
    unsigned int gc_thresh;
    int (*gc)(struct dst_ops *);
    struct dst_entry * (*check)(struct dst_entry *, __u32);
    unsigned int (*default_advmss)(const struct dst_entry *);
    unsigned int (*mtu)(const struct dst_entry *);
    u32 * (*cow_metrics)(struct dst_entry *, long unsigned int);
    void (*destroy)(struct dst_entry *);
    void (*ifdown)(struct dst_entry *, struct net_device *, int);
    struct dst_entry * (*negative_advice)(struct dst_entry *);
    void (*link_failure)(struct sk_buff *);
    void (*update_pmtu)(struct dst_entry *, struct sock *, struct sk_buff *, u32, bool);
    void (*redirect)(struct dst_entry *, struct sock *, struct sk_buff *);
    int (*local_out)(struct net *, struct sock *, struct sk_buff *);
    struct neighbour * (*neigh_lookup)(const struct dst_entry *, struct sk_buff *, const void *);
    void (*confirm_neigh)(const struct dst_entry *, const void *);
    struct kmem_cache *kmem_cachep;
    struct percpu_counter pcpuc_entries;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dst_ops {
    short unsigned int family;
    unsigned int gc_thresh;
    int (*gc)(struct dst_ops *);
    struct dst_entry * (*check)(struct dst_entry *, __u32);
    unsigned int (*default_advmss)(const struct dst_entry *);
    unsigned int (*mtu)(const struct dst_entry *);
    u32 * (*cow_metrics)(struct dst_entry *, long unsigned int);
    void (*destroy)(struct dst_entry *);
    void (*ifdown)(struct dst_entry *, struct net_device *, int);
    struct dst_entry * (*negative_advice)(struct dst_entry *);
    void (*link_failure)(struct sk_buff *);
    void (*update_pmtu)(struct dst_entry *, struct sock *, struct sk_buff *, u32, bool);
    void (*redirect)(struct dst_entry *, struct sock *, struct sk_buff *);
    int (*local_out)(struct net *, struct sock *, struct sk_buff *);
    struct neighbour * (*neigh_lookup)(const struct dst_entry *, struct sk_buff *, const void *);
    void (*confirm_neigh)(const struct dst_entry *, const void *);
    struct kmem_cache *kmem_cachep;
    struct percpu_counter pcpuc_entries;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dst_ops {
    short unsigned int family;
    unsigned int gc_thresh;
    int (*gc)(struct dst_ops *);
    struct dst_entry * (*check)(struct dst_entry *, __u32);
    unsigned int (*default_advmss)(const struct dst_entry *);
    unsigned int (*mtu)(const struct dst_entry *);
    u32 * (*cow_metrics)(struct dst_entry *, long unsigned int);
    void (*destroy)(struct dst_entry *);
    void (*ifdown)(struct dst_entry *, struct net_device *, int);
    struct dst_entry * (*negative_advice)(struct dst_entry *);
    void (*link_failure)(struct sk_buff *);
    void (*update_pmtu)(struct dst_entry *, struct sock *, struct sk_buff *, u32, bool);
    void (*redirect)(struct dst_entry *, struct sock *, struct sk_buff *);
    int (*local_out)(struct net *, struct sock *, struct sk_buff *);
    struct neighbour * (*neigh_lookup)(const struct dst_entry *, struct sk_buff *, const void *);
    void (*confirm_neigh)(const struct dst_entry *, const void *);
    struct kmem_cache *kmem_cachep;
    struct percpu_counter pcpuc_entries;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dst_ops {
    short unsigned int family;
    unsigned int gc_thresh;
    int (*gc)(struct dst_ops *);
    struct dst_entry * (*check)(struct dst_entry *, __u32);
    unsigned int (*default_advmss)(const struct dst_entry *);
    unsigned int (*mtu)(const struct dst_entry *);
    u32 * (*cow_metrics)(struct dst_entry *, long unsigned int);
    void (*destroy)(struct dst_entry *);
    void (*ifdown)(struct dst_entry *, struct net_device *, int);
    struct dst_entry * (*negative_advice)(struct dst_entry *);
    void (*link_failure)(struct sk_buff *);
    void (*update_pmtu)(struct dst_entry *, struct sock *, struct sk_buff *, u32, bool);
    void (*redirect)(struct dst_entry *, struct sock *, struct sk_buff *);
    int (*local_out)(struct net *, struct sock *, struct sk_buff *);
    struct neighbour * (*neigh_lookup)(const struct dst_entry *, struct sk_buff *, const void *);
    void (*confirm_neigh)(const struct dst_entry *, const void *);
    struct kmem_cache *kmem_cachep;
    struct percpu_counter pcpuc_entries;
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
struct dst_ops {
    short unsigned int family;
    unsigned int gc_thresh;
    int (*gc)(struct dst_ops *);
    struct dst_entry * (*check)(struct dst_entry *, __u32);
    unsigned int (*default_advmss)(const struct dst_entry *);
    unsigned int (*mtu)(const struct dst_entry *);
    u32 * (*cow_metrics)(struct dst_entry *, long unsigned int);
    void (*destroy)(struct dst_entry *);
    void (*ifdown)(struct dst_entry *, struct net_device *, int);
    struct dst_entry * (*negative_advice)(struct dst_entry *);
    void (*link_failure)(struct sk_buff *);
    void (*update_pmtu)(struct dst_entry *, struct sock *, struct sk_buff *, u32, bool);
    void (*redirect)(struct dst_entry *, struct sock *, struct sk_buff *);
    int (*local_out)(struct net *, struct sock *, struct sk_buff *);
    struct neighbour * (*neigh_lookup)(const struct dst_entry *, struct sk_buff *, const void *);
    void (*confirm_neigh)(const struct dst_entry *, const void *);
    struct kmem_cache *kmem_cachep;
    struct percpu_counter pcpuc_entries;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dst_ops {
    short unsigned int family;
    unsigned int gc_thresh;
    int (*gc)(struct dst_ops *);
    struct dst_entry * (*check)(struct dst_entry *, __u32);
    unsigned int (*default_advmss)(const struct dst_entry *);
    unsigned int (*mtu)(const struct dst_entry *);
    u32 * (*cow_metrics)(struct dst_entry *, long unsigned int);
    void (*destroy)(struct dst_entry *);
    void (*ifdown)(struct dst_entry *, struct net_device *, int);
    struct dst_entry * (*negative_advice)(struct dst_entry *);
    void (*link_failure)(struct sk_buff *);
    void (*update_pmtu)(struct dst_entry *, struct sock *, struct sk_buff *, u32, bool);
    void (*redirect)(struct dst_entry *, struct sock *, struct sk_buff *);
    int (*local_out)(struct net *, struct sock *, struct sk_buff *);
    struct neighbour * (*neigh_lookup)(const struct dst_entry *, struct sk_buff *, const void *);
    void (*confirm_neigh)(const struct dst_entry *, const void *);
    struct kmem_cache *kmem_cachep;
    struct percpu_counter pcpuc_entries;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dst_ops {
    short unsigned int family;
    unsigned int gc_thresh;
    int (*gc)(struct dst_ops *);
    struct dst_entry * (*check)(struct dst_entry *, __u32);
    unsigned int (*default_advmss)(const struct dst_entry *);
    unsigned int (*mtu)(const struct dst_entry *);
    u32 * (*cow_metrics)(struct dst_entry *, long unsigned int);
    void (*destroy)(struct dst_entry *);
    void (*ifdown)(struct dst_entry *, struct net_device *, int);
    struct dst_entry * (*negative_advice)(struct dst_entry *);
    void (*link_failure)(struct sk_buff *);
    void (*update_pmtu)(struct dst_entry *, struct sock *, struct sk_buff *, u32, bool);
    void (*redirect)(struct dst_entry *, struct sock *, struct sk_buff *);
    int (*local_out)(struct net *, struct sock *, struct sk_buff *);
    struct neighbour * (*neigh_lookup)(const struct dst_entry *, struct sk_buff *, const void *);
    void (*confirm_neigh)(const struct dst_entry *, const void *);
    struct kmem_cache *kmem_cachep;
    struct percpu_counter pcpuc_entries;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dst_ops {
    short unsigned int family;
    unsigned int gc_thresh;
    int (*gc)(struct dst_ops *);
    struct dst_entry * (*check)(struct dst_entry *, __u32);
    unsigned int (*default_advmss)(const struct dst_entry *);
    unsigned int (*mtu)(const struct dst_entry *);
    u32 * (*cow_metrics)(struct dst_entry *, long unsigned int);
    void (*destroy)(struct dst_entry *);
    void (*ifdown)(struct dst_entry *, struct net_device *, int);
    struct dst_entry * (*negative_advice)(struct dst_entry *);
    void (*link_failure)(struct sk_buff *);
    void (*update_pmtu)(struct dst_entry *, struct sock *, struct sk_buff *, u32, bool);
    void (*redirect)(struct dst_entry *, struct sock *, struct sk_buff *);
    int (*local_out)(struct net *, struct sock *, struct sk_buff *);
    struct neighbour * (*neigh_lookup)(const struct dst_entry *, struct sk_buff *, const void *);
    void (*confirm_neigh)(const struct dst_entry *, const void *);
    struct kmem_cache *kmem_cachep;
    struct percpu_counter pcpuc_entries;
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
<code>void (*confirm_neigh)(const struct dst_entry *, const void *)</code>
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
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>void (*update_pmtu)(struct dst_entry *, struct sock *, struct sk_buff *, u32)</code> ➡️ <code>void (*update_pmtu)(struct dst_entry *, struct sock *, struct sk_buff *, u32, bool)</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*gc)(struct dst_ops *)</code> ➡️ <code>void (*gc)(struct dst_ops *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>void (*ifdown)(struct dst_entry *, struct net_device *, int)</code> ➡️ <code>void (*ifdown)(struct dst_entry *, struct net_device *)</code>
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
