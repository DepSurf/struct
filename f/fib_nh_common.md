# Struct: <code>fib_nh_common</code>

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
In <code>4.13</code>: Absent ⚠️
</li>
<li>
In <code>4.15</code>: Absent ⚠️
</li>
<li>
In <code>4.18</code>: Absent ⚠️
</li>
<li>
In <code>5.0</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct fib_nh_common {
    struct net_device *nhc_dev;
    int nhc_oif;
    unsigned char nhc_scope;
    u8 nhc_family;
    u8 nhc_gw_family;
    unsigned char nhc_flags;
    struct lwtunnel_state *nhc_lwtstate;
    union (anon) nhc_gw;
    int nhc_weight;
    atomic_t nhc_upper_bound;
    struct rtable **nhc_pcpu_rth_output;
    struct rtable *nhc_rth_input;
    struct fnhe_hash_bucket *nhc_exceptions;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct fib_nh_common {
    struct net_device *nhc_dev;
    int nhc_oif;
    unsigned char nhc_scope;
    u8 nhc_family;
    u8 nhc_gw_family;
    unsigned char nhc_flags;
    struct lwtunnel_state *nhc_lwtstate;
    union (anon) nhc_gw;
    int nhc_weight;
    atomic_t nhc_upper_bound;
    struct rtable **nhc_pcpu_rth_output;
    struct rtable *nhc_rth_input;
    struct fnhe_hash_bucket *nhc_exceptions;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct fib_nh_common {
    struct net_device *nhc_dev;
    int nhc_oif;
    unsigned char nhc_scope;
    u8 nhc_family;
    u8 nhc_gw_family;
    unsigned char nhc_flags;
    struct lwtunnel_state *nhc_lwtstate;
    union (anon) nhc_gw;
    int nhc_weight;
    atomic_t nhc_upper_bound;
    struct rtable **nhc_pcpu_rth_output;
    struct rtable *nhc_rth_input;
    struct fnhe_hash_bucket *nhc_exceptions;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct fib_nh_common {
    struct net_device *nhc_dev;
    int nhc_oif;
    unsigned char nhc_scope;
    u8 nhc_family;
    u8 nhc_gw_family;
    unsigned char nhc_flags;
    struct lwtunnel_state *nhc_lwtstate;
    union (anon) nhc_gw;
    int nhc_weight;
    atomic_t nhc_upper_bound;
    struct rtable **nhc_pcpu_rth_output;
    struct rtable *nhc_rth_input;
    struct fnhe_hash_bucket *nhc_exceptions;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct fib_nh_common {
    struct net_device *nhc_dev;
    int nhc_oif;
    unsigned char nhc_scope;
    u8 nhc_family;
    u8 nhc_gw_family;
    unsigned char nhc_flags;
    struct lwtunnel_state *nhc_lwtstate;
    union (anon) nhc_gw;
    int nhc_weight;
    atomic_t nhc_upper_bound;
    struct rtable **nhc_pcpu_rth_output;
    struct rtable *nhc_rth_input;
    struct fnhe_hash_bucket *nhc_exceptions;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct fib_nh_common {
    struct net_device *nhc_dev;
    int nhc_oif;
    unsigned char nhc_scope;
    u8 nhc_family;
    u8 nhc_gw_family;
    unsigned char nhc_flags;
    struct lwtunnel_state *nhc_lwtstate;
    union (anon) nhc_gw;
    int nhc_weight;
    atomic_t nhc_upper_bound;
    struct rtable **nhc_pcpu_rth_output;
    struct rtable *nhc_rth_input;
    struct fnhe_hash_bucket *nhc_exceptions;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct fib_nh_common {
    struct net_device *nhc_dev;
    netdevice_tracker nhc_dev_tracker;
    int nhc_oif;
    unsigned char nhc_scope;
    u8 nhc_family;
    u8 nhc_gw_family;
    unsigned char nhc_flags;
    struct lwtunnel_state *nhc_lwtstate;
    union (anon) nhc_gw;
    int nhc_weight;
    atomic_t nhc_upper_bound;
    struct rtable **nhc_pcpu_rth_output;
    struct rtable *nhc_rth_input;
    struct fnhe_hash_bucket *nhc_exceptions;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct fib_nh_common {
    struct net_device *nhc_dev;
    netdevice_tracker nhc_dev_tracker;
    int nhc_oif;
    unsigned char nhc_scope;
    u8 nhc_family;
    u8 nhc_gw_family;
    unsigned char nhc_flags;
    struct lwtunnel_state *nhc_lwtstate;
    union (anon) nhc_gw;
    int nhc_weight;
    atomic_t nhc_upper_bound;
    struct rtable **nhc_pcpu_rth_output;
    struct rtable *nhc_rth_input;
    struct fnhe_hash_bucket *nhc_exceptions;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct fib_nh_common {
    struct net_device *nhc_dev;
    netdevice_tracker nhc_dev_tracker;
    int nhc_oif;
    unsigned char nhc_scope;
    u8 nhc_family;
    u8 nhc_gw_family;
    unsigned char nhc_flags;
    struct lwtunnel_state *nhc_lwtstate;
    union (anon) nhc_gw;
    int nhc_weight;
    atomic_t nhc_upper_bound;
    struct rtable **nhc_pcpu_rth_output;
    struct rtable *nhc_rth_input;
    struct fnhe_hash_bucket *nhc_exceptions;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct fib_nh_common {
    struct net_device *nhc_dev;
    netdevice_tracker nhc_dev_tracker;
    int nhc_oif;
    unsigned char nhc_scope;
    u8 nhc_family;
    u8 nhc_gw_family;
    unsigned char nhc_flags;
    struct lwtunnel_state *nhc_lwtstate;
    union (anon) nhc_gw;
    int nhc_weight;
    atomic_t nhc_upper_bound;
    struct rtable **nhc_pcpu_rth_output;
    struct rtable *nhc_rth_input;
    struct fnhe_hash_bucket *nhc_exceptions;
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
struct fib_nh_common {
    struct net_device *nhc_dev;
    int nhc_oif;
    unsigned char nhc_scope;
    u8 nhc_family;
    u8 nhc_gw_family;
    unsigned char nhc_flags;
    struct lwtunnel_state *nhc_lwtstate;
    union (anon) nhc_gw;
    int nhc_weight;
    atomic_t nhc_upper_bound;
    struct rtable **nhc_pcpu_rth_output;
    struct rtable *nhc_rth_input;
    struct fnhe_hash_bucket *nhc_exceptions;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct fib_nh_common {
    struct net_device *nhc_dev;
    int nhc_oif;
    unsigned char nhc_scope;
    u8 nhc_family;
    u8 nhc_gw_family;
    unsigned char nhc_flags;
    struct lwtunnel_state *nhc_lwtstate;
    union (anon) nhc_gw;
    int nhc_weight;
    atomic_t nhc_upper_bound;
    struct rtable **nhc_pcpu_rth_output;
    struct rtable *nhc_rth_input;
    struct fnhe_hash_bucket *nhc_exceptions;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct fib_nh_common {
    struct net_device *nhc_dev;
    int nhc_oif;
    unsigned char nhc_scope;
    u8 nhc_family;
    u8 nhc_gw_family;
    unsigned char nhc_flags;
    struct lwtunnel_state *nhc_lwtstate;
    union (anon) nhc_gw;
    int nhc_weight;
    atomic_t nhc_upper_bound;
    struct rtable **nhc_pcpu_rth_output;
    struct rtable *nhc_rth_input;
    struct fnhe_hash_bucket *nhc_exceptions;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct fib_nh_common {
    struct net_device *nhc_dev;
    int nhc_oif;
    unsigned char nhc_scope;
    u8 nhc_family;
    u8 nhc_gw_family;
    unsigned char nhc_flags;
    struct lwtunnel_state *nhc_lwtstate;
    union (anon) nhc_gw;
    int nhc_weight;
    atomic_t nhc_upper_bound;
    struct rtable **nhc_pcpu_rth_output;
    struct rtable *nhc_rth_input;
    struct fnhe_hash_bucket *nhc_exceptions;
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
struct fib_nh_common {
    struct net_device *nhc_dev;
    int nhc_oif;
    unsigned char nhc_scope;
    u8 nhc_family;
    u8 nhc_gw_family;
    unsigned char nhc_flags;
    struct lwtunnel_state *nhc_lwtstate;
    union (anon) nhc_gw;
    int nhc_weight;
    atomic_t nhc_upper_bound;
    struct rtable **nhc_pcpu_rth_output;
    struct rtable *nhc_rth_input;
    struct fnhe_hash_bucket *nhc_exceptions;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct fib_nh_common {
    struct net_device *nhc_dev;
    int nhc_oif;
    unsigned char nhc_scope;
    u8 nhc_family;
    u8 nhc_gw_family;
    unsigned char nhc_flags;
    struct lwtunnel_state *nhc_lwtstate;
    union (anon) nhc_gw;
    int nhc_weight;
    atomic_t nhc_upper_bound;
    struct rtable **nhc_pcpu_rth_output;
    struct rtable *nhc_rth_input;
    struct fnhe_hash_bucket *nhc_exceptions;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct fib_nh_common {
    struct net_device *nhc_dev;
    int nhc_oif;
    unsigned char nhc_scope;
    u8 nhc_family;
    u8 nhc_gw_family;
    unsigned char nhc_flags;
    struct lwtunnel_state *nhc_lwtstate;
    union (anon) nhc_gw;
    int nhc_weight;
    atomic_t nhc_upper_bound;
    struct rtable **nhc_pcpu_rth_output;
    struct rtable *nhc_rth_input;
    struct fnhe_hash_bucket *nhc_exceptions;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct fib_nh_common {
    struct net_device *nhc_dev;
    int nhc_oif;
    unsigned char nhc_scope;
    u8 nhc_family;
    u8 nhc_gw_family;
    unsigned char nhc_flags;
    struct lwtunnel_state *nhc_lwtstate;
    union (anon) nhc_gw;
    int nhc_weight;
    atomic_t nhc_upper_bound;
    struct rtable **nhc_pcpu_rth_output;
    struct rtable *nhc_rth_input;
    struct fnhe_hash_bucket *nhc_exceptions;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>netdevice_tracker nhc_dev_tracker</code>
</li>
</ul>
</details>
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
