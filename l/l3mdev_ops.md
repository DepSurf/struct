# Struct: <code>l3mdev_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct l3mdev_ops {
    u32 (*l3mdev_fib_table)(const struct net_device *);
    struct rtable * (*l3mdev_get_rtable)(const struct net_device *, const struct flowi4 *);
    int (*l3mdev_get_saddr)(struct net_device *, struct flowi4 *);
    struct dst_entry * (*l3mdev_get_rt6_dst)(const struct net_device *, const struct flowi6 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct l3mdev_ops {
    u32 (*l3mdev_fib_table)(const struct net_device *);
    struct sk_buff * (*l3mdev_l3_rcv)(struct net_device *, struct sk_buff *, u16);
    struct rtable * (*l3mdev_get_rtable)(const struct net_device *, const struct flowi4 *);
    int (*l3mdev_get_saddr)(struct net_device *, struct flowi4 *);
    struct dst_entry * (*l3mdev_get_rt6_dst)(const struct net_device *, struct flowi6 *);
    int (*l3mdev_get_saddr6)(struct net_device *, const struct sock *, struct flowi6 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct l3mdev_ops {
    u32 (*l3mdev_fib_table)(const struct net_device *);
    struct sk_buff * (*l3mdev_l3_rcv)(struct net_device *, struct sk_buff *, u16);
    struct sk_buff * (*l3mdev_l3_out)(struct net_device *, struct sock *, struct sk_buff *, u16);
    struct dst_entry * (*l3mdev_link_scope_lookup)(const struct net_device *, struct flowi6 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct l3mdev_ops {
    u32 (*l3mdev_fib_table)(const struct net_device *);
    struct sk_buff * (*l3mdev_l3_rcv)(struct net_device *, struct sk_buff *, u16);
    struct sk_buff * (*l3mdev_l3_out)(struct net_device *, struct sock *, struct sk_buff *, u16);
    struct dst_entry * (*l3mdev_link_scope_lookup)(const struct net_device *, struct flowi6 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct l3mdev_ops {
    u32 (*l3mdev_fib_table)(const struct net_device *);
    struct sk_buff * (*l3mdev_l3_rcv)(struct net_device *, struct sk_buff *, u16);
    struct sk_buff * (*l3mdev_l3_out)(struct net_device *, struct sock *, struct sk_buff *, u16);
    struct dst_entry * (*l3mdev_link_scope_lookup)(const struct net_device *, struct flowi6 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct l3mdev_ops {
    u32 (*l3mdev_fib_table)(const struct net_device *);
    struct sk_buff * (*l3mdev_l3_rcv)(struct net_device *, struct sk_buff *, u16);
    struct sk_buff * (*l3mdev_l3_out)(struct net_device *, struct sock *, struct sk_buff *, u16);
    struct dst_entry * (*l3mdev_link_scope_lookup)(const struct net_device *, struct flowi6 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct l3mdev_ops {
    u32 (*l3mdev_fib_table)(const struct net_device *);
    struct sk_buff * (*l3mdev_l3_rcv)(struct net_device *, struct sk_buff *, u16);
    struct sk_buff * (*l3mdev_l3_out)(struct net_device *, struct sock *, struct sk_buff *, u16);
    struct dst_entry * (*l3mdev_link_scope_lookup)(const struct net_device *, struct flowi6 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct l3mdev_ops {
    u32 (*l3mdev_fib_table)(const struct net_device *);
    struct sk_buff * (*l3mdev_l3_rcv)(struct net_device *, struct sk_buff *, u16);
    struct sk_buff * (*l3mdev_l3_out)(struct net_device *, struct sock *, struct sk_buff *, u16);
    struct dst_entry * (*l3mdev_link_scope_lookup)(const struct net_device *, struct flowi6 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct l3mdev_ops {
    u32 (*l3mdev_fib_table)(const struct net_device *);
    struct sk_buff * (*l3mdev_l3_rcv)(struct net_device *, struct sk_buff *, u16);
    struct sk_buff * (*l3mdev_l3_out)(struct net_device *, struct sock *, struct sk_buff *, u16);
    struct dst_entry * (*l3mdev_link_scope_lookup)(const struct net_device *, struct flowi6 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct l3mdev_ops {
    u32 (*l3mdev_fib_table)(const struct net_device *);
    struct sk_buff * (*l3mdev_l3_rcv)(struct net_device *, struct sk_buff *, u16);
    struct sk_buff * (*l3mdev_l3_out)(struct net_device *, struct sock *, struct sk_buff *, u16);
    struct dst_entry * (*l3mdev_link_scope_lookup)(const struct net_device *, struct flowi6 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct l3mdev_ops {
    u32 (*l3mdev_fib_table)(const struct net_device *);
    struct sk_buff * (*l3mdev_l3_rcv)(struct net_device *, struct sk_buff *, u16);
    struct sk_buff * (*l3mdev_l3_out)(struct net_device *, struct sock *, struct sk_buff *, u16);
    struct dst_entry * (*l3mdev_link_scope_lookup)(const struct net_device *, struct flowi6 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct l3mdev_ops {
    u32 (*l3mdev_fib_table)(const struct net_device *);
    struct sk_buff * (*l3mdev_l3_rcv)(struct net_device *, struct sk_buff *, u16);
    struct sk_buff * (*l3mdev_l3_out)(struct net_device *, struct sock *, struct sk_buff *, u16);
    struct dst_entry * (*l3mdev_link_scope_lookup)(const struct net_device *, struct flowi6 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct l3mdev_ops {
    u32 (*l3mdev_fib_table)(const struct net_device *);
    struct sk_buff * (*l3mdev_l3_rcv)(struct net_device *, struct sk_buff *, u16);
    struct sk_buff * (*l3mdev_l3_out)(struct net_device *, struct sock *, struct sk_buff *, u16);
    struct dst_entry * (*l3mdev_link_scope_lookup)(const struct net_device *, struct flowi6 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct l3mdev_ops {
    u32 (*l3mdev_fib_table)(const struct net_device *);
    struct sk_buff * (*l3mdev_l3_rcv)(struct net_device *, struct sk_buff *, u16);
    struct sk_buff * (*l3mdev_l3_out)(struct net_device *, struct sock *, struct sk_buff *, u16);
    struct dst_entry * (*l3mdev_link_scope_lookup)(const struct net_device *, struct flowi6 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct l3mdev_ops {
    u32 (*l3mdev_fib_table)(const struct net_device *);
    struct sk_buff * (*l3mdev_l3_rcv)(struct net_device *, struct sk_buff *, u16);
    struct sk_buff * (*l3mdev_l3_out)(struct net_device *, struct sock *, struct sk_buff *, u16);
    struct dst_entry * (*l3mdev_link_scope_lookup)(const struct net_device *, struct flowi6 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct l3mdev_ops {
    u32 (*l3mdev_fib_table)(const struct net_device *);
    struct sk_buff * (*l3mdev_l3_rcv)(struct net_device *, struct sk_buff *, u16);
    struct sk_buff * (*l3mdev_l3_out)(struct net_device *, struct sock *, struct sk_buff *, u16);
    struct dst_entry * (*l3mdev_link_scope_lookup)(const struct net_device *, struct flowi6 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct l3mdev_ops {
    u32 (*l3mdev_fib_table)(const struct net_device *);
    struct sk_buff * (*l3mdev_l3_rcv)(struct net_device *, struct sk_buff *, u16);
    struct sk_buff * (*l3mdev_l3_out)(struct net_device *, struct sock *, struct sk_buff *, u16);
    struct dst_entry * (*l3mdev_link_scope_lookup)(const struct net_device *, struct flowi6 *);
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
struct l3mdev_ops {
    u32 (*l3mdev_fib_table)(const struct net_device *);
    struct sk_buff * (*l3mdev_l3_rcv)(struct net_device *, struct sk_buff *, u16);
    struct sk_buff * (*l3mdev_l3_out)(struct net_device *, struct sock *, struct sk_buff *, u16);
    struct dst_entry * (*l3mdev_link_scope_lookup)(const struct net_device *, struct flowi6 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct l3mdev_ops {
    u32 (*l3mdev_fib_table)(const struct net_device *);
    struct sk_buff * (*l3mdev_l3_rcv)(struct net_device *, struct sk_buff *, u16);
    struct sk_buff * (*l3mdev_l3_out)(struct net_device *, struct sock *, struct sk_buff *, u16);
    struct dst_entry * (*l3mdev_link_scope_lookup)(const struct net_device *, struct flowi6 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct l3mdev_ops {
    u32 (*l3mdev_fib_table)(const struct net_device *);
    struct sk_buff * (*l3mdev_l3_rcv)(struct net_device *, struct sk_buff *, u16);
    struct sk_buff * (*l3mdev_l3_out)(struct net_device *, struct sock *, struct sk_buff *, u16);
    struct dst_entry * (*l3mdev_link_scope_lookup)(const struct net_device *, struct flowi6 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct l3mdev_ops {
    u32 (*l3mdev_fib_table)(const struct net_device *);
    struct sk_buff * (*l3mdev_l3_rcv)(struct net_device *, struct sk_buff *, u16);
    struct sk_buff * (*l3mdev_l3_out)(struct net_device *, struct sock *, struct sk_buff *, u16);
    struct dst_entry * (*l3mdev_link_scope_lookup)(const struct net_device *, struct flowi6 *);
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
struct l3mdev_ops {
    u32 (*l3mdev_fib_table)(const struct net_device *);
    struct sk_buff * (*l3mdev_l3_rcv)(struct net_device *, struct sk_buff *, u16);
    struct sk_buff * (*l3mdev_l3_out)(struct net_device *, struct sock *, struct sk_buff *, u16);
    struct dst_entry * (*l3mdev_link_scope_lookup)(const struct net_device *, struct flowi6 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct l3mdev_ops {
    u32 (*l3mdev_fib_table)(const struct net_device *);
    struct sk_buff * (*l3mdev_l3_rcv)(struct net_device *, struct sk_buff *, u16);
    struct sk_buff * (*l3mdev_l3_out)(struct net_device *, struct sock *, struct sk_buff *, u16);
    struct dst_entry * (*l3mdev_link_scope_lookup)(const struct net_device *, struct flowi6 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct l3mdev_ops {
    u32 (*l3mdev_fib_table)(const struct net_device *);
    struct sk_buff * (*l3mdev_l3_rcv)(struct net_device *, struct sk_buff *, u16);
    struct sk_buff * (*l3mdev_l3_out)(struct net_device *, struct sock *, struct sk_buff *, u16);
    struct dst_entry * (*l3mdev_link_scope_lookup)(const struct net_device *, struct flowi6 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct l3mdev_ops {
    u32 (*l3mdev_fib_table)(const struct net_device *);
    struct sk_buff * (*l3mdev_l3_rcv)(struct net_device *, struct sk_buff *, u16);
    struct sk_buff * (*l3mdev_l3_out)(struct net_device *, struct sock *, struct sk_buff *, u16);
    struct dst_entry * (*l3mdev_link_scope_lookup)(const struct net_device *, struct flowi6 *);
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
<code>struct sk_buff * (*l3mdev_l3_rcv)(struct net_device *, struct sk_buff *, u16)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*l3mdev_get_saddr6)(struct net_device *, const struct sock *, struct flowi6 *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct dst_entry * (*l3mdev_get_rt6_dst)(const struct net_device *, const struct flowi6 *)</code> ➡️ <code>struct dst_entry * (*l3mdev_get_rt6_dst)(const struct net_device *, struct flowi6 *)</code>
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
<code>struct sk_buff * (*l3mdev_l3_out)(struct net_device *, struct sock *, struct sk_buff *, u16)</code>
</li>
<li>
<b>Field added. </b>
<code>struct dst_entry * (*l3mdev_link_scope_lookup)(const struct net_device *, struct flowi6 *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rtable * (*l3mdev_get_rtable)(const struct net_device *, const struct flowi4 *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*l3mdev_get_saddr)(struct net_device *, struct flowi4 *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct dst_entry * (*l3mdev_get_rt6_dst)(const struct net_device *, struct flowi6 *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*l3mdev_get_saddr6)(struct net_device *, const struct sock *, struct flowi6 *)</code>
</li>
</ul>
</details>
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
