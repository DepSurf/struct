# Struct: <code>nh_config</code>

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
struct nh_config {
    u32 nh_id;
    u8 nh_family;
    u8 nh_protocol;
    u8 nh_blackhole;
    u32 nh_flags;
    int nh_ifindex;
    struct net_device *dev;
    union (anon) gw;
    struct nlattr *nh_grp;
    u16 nh_grp_type;
    struct nlattr *nh_encap;
    u16 nh_encap_type;
    u32 nlflags;
    struct nl_info nlinfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct nh_config {
    u32 nh_id;
    u8 nh_family;
    u8 nh_protocol;
    u8 nh_blackhole;
    u32 nh_flags;
    int nh_ifindex;
    struct net_device *dev;
    union (anon) gw;
    struct nlattr *nh_grp;
    u16 nh_grp_type;
    struct nlattr *nh_encap;
    u16 nh_encap_type;
    u32 nlflags;
    struct nl_info nlinfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct nh_config {
    u32 nh_id;
    u8 nh_family;
    u8 nh_protocol;
    u8 nh_blackhole;
    u8 nh_fdb;
    u32 nh_flags;
    int nh_ifindex;
    struct net_device *dev;
    union (anon) gw;
    struct nlattr *nh_grp;
    u16 nh_grp_type;
    struct nlattr *nh_encap;
    u16 nh_encap_type;
    u32 nlflags;
    struct nl_info nlinfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct nh_config {
    u32 nh_id;
    u8 nh_family;
    u8 nh_protocol;
    u8 nh_blackhole;
    u8 nh_fdb;
    u32 nh_flags;
    int nh_ifindex;
    struct net_device *dev;
    union (anon) gw;
    struct nlattr *nh_grp;
    u16 nh_grp_type;
    struct nlattr *nh_encap;
    u16 nh_encap_type;
    u32 nlflags;
    struct nl_info nlinfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct nh_config {
    u32 nh_id;
    u8 nh_family;
    u8 nh_protocol;
    u8 nh_blackhole;
    u8 nh_fdb;
    u32 nh_flags;
    int nh_ifindex;
    struct net_device *dev;
    union (anon) gw;
    struct nlattr *nh_grp;
    u16 nh_grp_type;
    u16 nh_grp_res_num_buckets;
    long unsigned int nh_grp_res_idle_timer;
    long unsigned int nh_grp_res_unbalanced_timer;
    bool nh_grp_res_has_num_buckets;
    bool nh_grp_res_has_idle_timer;
    bool nh_grp_res_has_unbalanced_timer;
    struct nlattr *nh_encap;
    u16 nh_encap_type;
    u32 nlflags;
    struct nl_info nlinfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct nh_config {
    u32 nh_id;
    u8 nh_family;
    u8 nh_protocol;
    u8 nh_blackhole;
    u8 nh_fdb;
    u32 nh_flags;
    int nh_ifindex;
    struct net_device *dev;
    union (anon) gw;
    struct nlattr *nh_grp;
    u16 nh_grp_type;
    u16 nh_grp_res_num_buckets;
    long unsigned int nh_grp_res_idle_timer;
    long unsigned int nh_grp_res_unbalanced_timer;
    bool nh_grp_res_has_num_buckets;
    bool nh_grp_res_has_idle_timer;
    bool nh_grp_res_has_unbalanced_timer;
    struct nlattr *nh_encap;
    u16 nh_encap_type;
    u32 nlflags;
    struct nl_info nlinfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct nh_config {
    u32 nh_id;
    u8 nh_family;
    u8 nh_protocol;
    u8 nh_blackhole;
    u8 nh_fdb;
    u32 nh_flags;
    int nh_ifindex;
    struct net_device *dev;
    union (anon) gw;
    struct nlattr *nh_grp;
    u16 nh_grp_type;
    u16 nh_grp_res_num_buckets;
    long unsigned int nh_grp_res_idle_timer;
    long unsigned int nh_grp_res_unbalanced_timer;
    bool nh_grp_res_has_num_buckets;
    bool nh_grp_res_has_idle_timer;
    bool nh_grp_res_has_unbalanced_timer;
    struct nlattr *nh_encap;
    u16 nh_encap_type;
    u32 nlflags;
    struct nl_info nlinfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct nh_config {
    u32 nh_id;
    u8 nh_family;
    u8 nh_protocol;
    u8 nh_blackhole;
    u8 nh_fdb;
    u32 nh_flags;
    int nh_ifindex;
    struct net_device *dev;
    union (anon) gw;
    struct nlattr *nh_grp;
    u16 nh_grp_type;
    u16 nh_grp_res_num_buckets;
    long unsigned int nh_grp_res_idle_timer;
    long unsigned int nh_grp_res_unbalanced_timer;
    bool nh_grp_res_has_num_buckets;
    bool nh_grp_res_has_idle_timer;
    bool nh_grp_res_has_unbalanced_timer;
    struct nlattr *nh_encap;
    u16 nh_encap_type;
    u32 nlflags;
    struct nl_info nlinfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct nh_config {
    u32 nh_id;
    u8 nh_family;
    u8 nh_protocol;
    u8 nh_blackhole;
    u8 nh_fdb;
    u32 nh_flags;
    int nh_ifindex;
    struct net_device *dev;
    union (anon) gw;
    struct nlattr *nh_grp;
    u16 nh_grp_type;
    u16 nh_grp_res_num_buckets;
    long unsigned int nh_grp_res_idle_timer;
    long unsigned int nh_grp_res_unbalanced_timer;
    bool nh_grp_res_has_num_buckets;
    bool nh_grp_res_has_idle_timer;
    bool nh_grp_res_has_unbalanced_timer;
    struct nlattr *nh_encap;
    u16 nh_encap_type;
    u32 nlflags;
    struct nl_info nlinfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct nh_config {
    u32 nh_id;
    u8 nh_family;
    u8 nh_protocol;
    u8 nh_blackhole;
    u8 nh_fdb;
    u32 nh_flags;
    int nh_ifindex;
    struct net_device *dev;
    union (anon) gw;
    struct nlattr *nh_grp;
    u16 nh_grp_type;
    u16 nh_grp_res_num_buckets;
    long unsigned int nh_grp_res_idle_timer;
    long unsigned int nh_grp_res_unbalanced_timer;
    bool nh_grp_res_has_num_buckets;
    bool nh_grp_res_has_idle_timer;
    bool nh_grp_res_has_unbalanced_timer;
    struct nlattr *nh_encap;
    u16 nh_encap_type;
    u32 nlflags;
    struct nl_info nlinfo;
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
struct nh_config {
    u32 nh_id;
    u8 nh_family;
    u8 nh_protocol;
    u8 nh_blackhole;
    u32 nh_flags;
    int nh_ifindex;
    struct net_device *dev;
    union (anon) gw;
    struct nlattr *nh_grp;
    u16 nh_grp_type;
    struct nlattr *nh_encap;
    u16 nh_encap_type;
    u32 nlflags;
    struct nl_info nlinfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct nh_config {
    u32 nh_id;
    u8 nh_family;
    u8 nh_protocol;
    u8 nh_blackhole;
    u32 nh_flags;
    int nh_ifindex;
    struct net_device *dev;
    union (anon) gw;
    struct nlattr *nh_grp;
    u16 nh_grp_type;
    struct nlattr *nh_encap;
    u16 nh_encap_type;
    u32 nlflags;
    struct nl_info nlinfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct nh_config {
    u32 nh_id;
    u8 nh_family;
    u8 nh_protocol;
    u8 nh_blackhole;
    u32 nh_flags;
    int nh_ifindex;
    struct net_device *dev;
    union (anon) gw;
    struct nlattr *nh_grp;
    u16 nh_grp_type;
    struct nlattr *nh_encap;
    u16 nh_encap_type;
    u32 nlflags;
    struct nl_info nlinfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct nh_config {
    u32 nh_id;
    u8 nh_family;
    u8 nh_protocol;
    u8 nh_blackhole;
    u32 nh_flags;
    int nh_ifindex;
    struct net_device *dev;
    union (anon) gw;
    struct nlattr *nh_grp;
    u16 nh_grp_type;
    struct nlattr *nh_encap;
    u16 nh_encap_type;
    u32 nlflags;
    struct nl_info nlinfo;
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
struct nh_config {
    u32 nh_id;
    u8 nh_family;
    u8 nh_protocol;
    u8 nh_blackhole;
    u32 nh_flags;
    int nh_ifindex;
    struct net_device *dev;
    union (anon) gw;
    struct nlattr *nh_grp;
    u16 nh_grp_type;
    struct nlattr *nh_encap;
    u16 nh_encap_type;
    u32 nlflags;
    struct nl_info nlinfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct nh_config {
    u32 nh_id;
    u8 nh_family;
    u8 nh_protocol;
    u8 nh_blackhole;
    u32 nh_flags;
    int nh_ifindex;
    struct net_device *dev;
    union (anon) gw;
    struct nlattr *nh_grp;
    u16 nh_grp_type;
    struct nlattr *nh_encap;
    u16 nh_encap_type;
    u32 nlflags;
    struct nl_info nlinfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct nh_config {
    u32 nh_id;
    u8 nh_family;
    u8 nh_protocol;
    u8 nh_blackhole;
    u32 nh_flags;
    int nh_ifindex;
    struct net_device *dev;
    union (anon) gw;
    struct nlattr *nh_grp;
    u16 nh_grp_type;
    struct nlattr *nh_encap;
    u16 nh_encap_type;
    u32 nlflags;
    struct nl_info nlinfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct nh_config {
    u32 nh_id;
    u8 nh_family;
    u8 nh_protocol;
    u8 nh_blackhole;
    u32 nh_flags;
    int nh_ifindex;
    struct net_device *dev;
    union (anon) gw;
    struct nlattr *nh_grp;
    u16 nh_grp_type;
    struct nlattr *nh_encap;
    u16 nh_encap_type;
    u32 nlflags;
    struct nl_info nlinfo;
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 nh_fdb</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 nh_grp_res_num_buckets</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int nh_grp_res_idle_timer</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int nh_grp_res_unbalanced_timer</code>
</li>
<li>
<b>Field added. </b>
<code>bool nh_grp_res_has_num_buckets</code>
</li>
<li>
<b>Field added. </b>
<code>bool nh_grp_res_has_idle_timer</code>
</li>
<li>
<b>Field added. </b>
<code>bool nh_grp_res_has_unbalanced_timer</code>
</li>
</ul>
</details>
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
