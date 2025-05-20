# Struct: <code>fib6_config</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct fib6_config {
    u32 fc_table;
    u32 fc_metric;
    int fc_dst_len;
    int fc_src_len;
    int fc_ifindex;
    u32 fc_flags;
    u32 fc_protocol;
    u32 fc_type;
    struct in6_addr fc_dst;
    struct in6_addr fc_src;
    struct in6_addr fc_prefsrc;
    struct in6_addr fc_gateway;
    long unsigned int fc_expires;
    struct nlattr *fc_mx;
    int fc_mx_len;
    int fc_mp_len;
    struct nlattr *fc_mp;
    struct nl_info fc_nlinfo;
    struct nlattr *fc_encap;
    u16 fc_encap_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct fib6_config {
    u32 fc_table;
    u32 fc_metric;
    int fc_dst_len;
    int fc_src_len;
    int fc_ifindex;
    u32 fc_flags;
    u32 fc_protocol;
    u32 fc_type;
    struct in6_addr fc_dst;
    struct in6_addr fc_src;
    struct in6_addr fc_prefsrc;
    struct in6_addr fc_gateway;
    long unsigned int fc_expires;
    struct nlattr *fc_mx;
    int fc_mx_len;
    int fc_mp_len;
    struct nlattr *fc_mp;
    struct nl_info fc_nlinfo;
    struct nlattr *fc_encap;
    u16 fc_encap_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct fib6_config {
    u32 fc_table;
    u32 fc_metric;
    int fc_dst_len;
    int fc_src_len;
    int fc_ifindex;
    u32 fc_flags;
    u32 fc_protocol;
    u32 fc_type;
    struct in6_addr fc_dst;
    struct in6_addr fc_src;
    struct in6_addr fc_prefsrc;
    struct in6_addr fc_gateway;
    long unsigned int fc_expires;
    struct nlattr *fc_mx;
    int fc_mx_len;
    int fc_mp_len;
    struct nlattr *fc_mp;
    struct nl_info fc_nlinfo;
    struct nlattr *fc_encap;
    u16 fc_encap_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct fib6_config {
    u32 fc_table;
    u32 fc_metric;
    int fc_dst_len;
    int fc_src_len;
    int fc_ifindex;
    u32 fc_flags;
    u32 fc_protocol;
    u16 fc_type;
    u16 fc_delete_all_nh;
    u16 __unused;
    struct in6_addr fc_dst;
    struct in6_addr fc_src;
    struct in6_addr fc_prefsrc;
    struct in6_addr fc_gateway;
    long unsigned int fc_expires;
    struct nlattr *fc_mx;
    int fc_mx_len;
    int fc_mp_len;
    struct nlattr *fc_mp;
    struct nl_info fc_nlinfo;
    struct nlattr *fc_encap;
    u16 fc_encap_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct fib6_config {
    u32 fc_table;
    u32 fc_metric;
    int fc_dst_len;
    int fc_src_len;
    int fc_ifindex;
    u32 fc_flags;
    u32 fc_protocol;
    u16 fc_type;
    u16 fc_delete_all_nh;
    u16 __unused;
    struct in6_addr fc_dst;
    struct in6_addr fc_src;
    struct in6_addr fc_prefsrc;
    struct in6_addr fc_gateway;
    long unsigned int fc_expires;
    struct nlattr *fc_mx;
    int fc_mx_len;
    int fc_mp_len;
    struct nlattr *fc_mp;
    struct nl_info fc_nlinfo;
    struct nlattr *fc_encap;
    u16 fc_encap_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct fib6_config {
    u32 fc_table;
    u32 fc_metric;
    int fc_dst_len;
    int fc_src_len;
    int fc_ifindex;
    u32 fc_flags;
    u32 fc_protocol;
    u16 fc_type;
    u16 fc_delete_all_nh;
    u16 __unused;
    struct in6_addr fc_dst;
    struct in6_addr fc_src;
    struct in6_addr fc_prefsrc;
    struct in6_addr fc_gateway;
    long unsigned int fc_expires;
    struct nlattr *fc_mx;
    int fc_mx_len;
    int fc_mp_len;
    struct nlattr *fc_mp;
    struct nl_info fc_nlinfo;
    struct nlattr *fc_encap;
    u16 fc_encap_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct fib6_config {
    u32 fc_table;
    u32 fc_metric;
    int fc_dst_len;
    int fc_src_len;
    int fc_ifindex;
    u32 fc_flags;
    u32 fc_protocol;
    u16 fc_type;
    u16 fc_delete_all_nh;
    u16 __unused;
    struct in6_addr fc_dst;
    struct in6_addr fc_src;
    struct in6_addr fc_prefsrc;
    struct in6_addr fc_gateway;
    long unsigned int fc_expires;
    struct nlattr *fc_mx;
    int fc_mx_len;
    int fc_mp_len;
    struct nlattr *fc_mp;
    struct nl_info fc_nlinfo;
    struct nlattr *fc_encap;
    u16 fc_encap_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct fib6_config {
    u32 fc_table;
    u32 fc_metric;
    int fc_dst_len;
    int fc_src_len;
    int fc_ifindex;
    u32 fc_flags;
    u32 fc_protocol;
    u16 fc_type;
    u16 fc_delete_all_nh;
    u16 fc_ignore_dev_down;
    u16 __unused;
    u32 fc_nh_id;
    struct in6_addr fc_dst;
    struct in6_addr fc_src;
    struct in6_addr fc_prefsrc;
    struct in6_addr fc_gateway;
    long unsigned int fc_expires;
    struct nlattr *fc_mx;
    int fc_mx_len;
    int fc_mp_len;
    struct nlattr *fc_mp;
    struct nl_info fc_nlinfo;
    struct nlattr *fc_encap;
    u16 fc_encap_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct fib6_config {
    u32 fc_table;
    u32 fc_metric;
    int fc_dst_len;
    int fc_src_len;
    int fc_ifindex;
    u32 fc_flags;
    u32 fc_protocol;
    u16 fc_type;
    u16 fc_delete_all_nh;
    u16 fc_ignore_dev_down;
    u16 __unused;
    u32 fc_nh_id;
    struct in6_addr fc_dst;
    struct in6_addr fc_src;
    struct in6_addr fc_prefsrc;
    struct in6_addr fc_gateway;
    long unsigned int fc_expires;
    struct nlattr *fc_mx;
    int fc_mx_len;
    int fc_mp_len;
    struct nlattr *fc_mp;
    struct nl_info fc_nlinfo;
    struct nlattr *fc_encap;
    u16 fc_encap_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct fib6_config {
    u32 fc_table;
    u32 fc_metric;
    int fc_dst_len;
    int fc_src_len;
    int fc_ifindex;
    u32 fc_flags;
    u32 fc_protocol;
    u16 fc_type;
    u16 fc_delete_all_nh;
    u16 fc_ignore_dev_down;
    u16 __unused;
    u32 fc_nh_id;
    struct in6_addr fc_dst;
    struct in6_addr fc_src;
    struct in6_addr fc_prefsrc;
    struct in6_addr fc_gateway;
    long unsigned int fc_expires;
    struct nlattr *fc_mx;
    int fc_mx_len;
    int fc_mp_len;
    struct nlattr *fc_mp;
    struct nl_info fc_nlinfo;
    struct nlattr *fc_encap;
    u16 fc_encap_type;
    bool fc_is_fdb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct fib6_config {
    u32 fc_table;
    u32 fc_metric;
    int fc_dst_len;
    int fc_src_len;
    int fc_ifindex;
    u32 fc_flags;
    u32 fc_protocol;
    u16 fc_type;
    u16 fc_delete_all_nh;
    u16 fc_ignore_dev_down;
    u16 __unused;
    u32 fc_nh_id;
    struct in6_addr fc_dst;
    struct in6_addr fc_src;
    struct in6_addr fc_prefsrc;
    struct in6_addr fc_gateway;
    long unsigned int fc_expires;
    struct nlattr *fc_mx;
    int fc_mx_len;
    int fc_mp_len;
    struct nlattr *fc_mp;
    struct nl_info fc_nlinfo;
    struct nlattr *fc_encap;
    u16 fc_encap_type;
    bool fc_is_fdb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct fib6_config {
    u32 fc_table;
    u32 fc_metric;
    int fc_dst_len;
    int fc_src_len;
    int fc_ifindex;
    u32 fc_flags;
    u32 fc_protocol;
    u16 fc_type;
    u16 fc_delete_all_nh;
    u16 fc_ignore_dev_down;
    u16 __unused;
    u32 fc_nh_id;
    struct in6_addr fc_dst;
    struct in6_addr fc_src;
    struct in6_addr fc_prefsrc;
    struct in6_addr fc_gateway;
    long unsigned int fc_expires;
    struct nlattr *fc_mx;
    int fc_mx_len;
    int fc_mp_len;
    struct nlattr *fc_mp;
    struct nl_info fc_nlinfo;
    struct nlattr *fc_encap;
    u16 fc_encap_type;
    bool fc_is_fdb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct fib6_config {
    u32 fc_table;
    u32 fc_metric;
    int fc_dst_len;
    int fc_src_len;
    int fc_ifindex;
    u32 fc_flags;
    u32 fc_protocol;
    u16 fc_type;
    u16 fc_delete_all_nh;
    u16 fc_ignore_dev_down;
    u16 __unused;
    u32 fc_nh_id;
    struct in6_addr fc_dst;
    struct in6_addr fc_src;
    struct in6_addr fc_prefsrc;
    struct in6_addr fc_gateway;
    long unsigned int fc_expires;
    struct nlattr *fc_mx;
    int fc_mx_len;
    int fc_mp_len;
    struct nlattr *fc_mp;
    struct nl_info fc_nlinfo;
    struct nlattr *fc_encap;
    u16 fc_encap_type;
    bool fc_is_fdb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct fib6_config {
    u32 fc_table;
    u32 fc_metric;
    int fc_dst_len;
    int fc_src_len;
    int fc_ifindex;
    u32 fc_flags;
    u32 fc_protocol;
    u16 fc_type;
    u16 fc_delete_all_nh;
    u16 fc_ignore_dev_down;
    u16 __unused;
    u32 fc_nh_id;
    struct in6_addr fc_dst;
    struct in6_addr fc_src;
    struct in6_addr fc_prefsrc;
    struct in6_addr fc_gateway;
    long unsigned int fc_expires;
    struct nlattr *fc_mx;
    int fc_mx_len;
    int fc_mp_len;
    struct nlattr *fc_mp;
    struct nl_info fc_nlinfo;
    struct nlattr *fc_encap;
    u16 fc_encap_type;
    bool fc_is_fdb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct fib6_config {
    u32 fc_table;
    u32 fc_metric;
    int fc_dst_len;
    int fc_src_len;
    int fc_ifindex;
    u32 fc_flags;
    u32 fc_protocol;
    u16 fc_type;
    u16 fc_delete_all_nh;
    u16 fc_ignore_dev_down;
    u16 __unused;
    u32 fc_nh_id;
    struct in6_addr fc_dst;
    struct in6_addr fc_src;
    struct in6_addr fc_prefsrc;
    struct in6_addr fc_gateway;
    long unsigned int fc_expires;
    struct nlattr *fc_mx;
    int fc_mx_len;
    int fc_mp_len;
    struct nlattr *fc_mp;
    struct nl_info fc_nlinfo;
    struct nlattr *fc_encap;
    u16 fc_encap_type;
    bool fc_is_fdb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct fib6_config {
    u32 fc_table;
    u32 fc_metric;
    int fc_dst_len;
    int fc_src_len;
    int fc_ifindex;
    u32 fc_flags;
    u32 fc_protocol;
    u16 fc_type;
    u16 fc_delete_all_nh;
    u16 fc_ignore_dev_down;
    u16 __unused;
    u32 fc_nh_id;
    struct in6_addr fc_dst;
    struct in6_addr fc_src;
    struct in6_addr fc_prefsrc;
    struct in6_addr fc_gateway;
    long unsigned int fc_expires;
    struct nlattr *fc_mx;
    int fc_mx_len;
    int fc_mp_len;
    struct nlattr *fc_mp;
    struct nl_info fc_nlinfo;
    struct nlattr *fc_encap;
    u16 fc_encap_type;
    bool fc_is_fdb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct fib6_config {
    u32 fc_table;
    u32 fc_metric;
    int fc_dst_len;
    int fc_src_len;
    int fc_ifindex;
    u32 fc_flags;
    u32 fc_protocol;
    u16 fc_type;
    u16 fc_delete_all_nh;
    u16 fc_ignore_dev_down;
    u16 __unused;
    u32 fc_nh_id;
    struct in6_addr fc_dst;
    struct in6_addr fc_src;
    struct in6_addr fc_prefsrc;
    struct in6_addr fc_gateway;
    long unsigned int fc_expires;
    struct nlattr *fc_mx;
    int fc_mx_len;
    int fc_mp_len;
    struct nlattr *fc_mp;
    struct nl_info fc_nlinfo;
    struct nlattr *fc_encap;
    u16 fc_encap_type;
    bool fc_is_fdb;
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
struct fib6_config {
    u32 fc_table;
    u32 fc_metric;
    int fc_dst_len;
    int fc_src_len;
    int fc_ifindex;
    u32 fc_flags;
    u32 fc_protocol;
    u16 fc_type;
    u16 fc_delete_all_nh;
    u16 fc_ignore_dev_down;
    u16 __unused;
    u32 fc_nh_id;
    struct in6_addr fc_dst;
    struct in6_addr fc_src;
    struct in6_addr fc_prefsrc;
    struct in6_addr fc_gateway;
    long unsigned int fc_expires;
    struct nlattr *fc_mx;
    int fc_mx_len;
    int fc_mp_len;
    struct nlattr *fc_mp;
    struct nl_info fc_nlinfo;
    struct nlattr *fc_encap;
    u16 fc_encap_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct fib6_config {
    u32 fc_table;
    u32 fc_metric;
    int fc_dst_len;
    int fc_src_len;
    int fc_ifindex;
    u32 fc_flags;
    u32 fc_protocol;
    u16 fc_type;
    u16 fc_delete_all_nh;
    u16 fc_ignore_dev_down;
    u16 __unused;
    u32 fc_nh_id;
    struct in6_addr fc_dst;
    struct in6_addr fc_src;
    struct in6_addr fc_prefsrc;
    struct in6_addr fc_gateway;
    long unsigned int fc_expires;
    struct nlattr *fc_mx;
    int fc_mx_len;
    int fc_mp_len;
    struct nlattr *fc_mp;
    struct nl_info fc_nlinfo;
    struct nlattr *fc_encap;
    u16 fc_encap_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct fib6_config {
    u32 fc_table;
    u32 fc_metric;
    int fc_dst_len;
    int fc_src_len;
    int fc_ifindex;
    u32 fc_flags;
    u32 fc_protocol;
    u16 fc_type;
    u16 fc_delete_all_nh;
    u16 fc_ignore_dev_down;
    u16 __unused;
    u32 fc_nh_id;
    struct in6_addr fc_dst;
    struct in6_addr fc_src;
    struct in6_addr fc_prefsrc;
    struct in6_addr fc_gateway;
    long unsigned int fc_expires;
    struct nlattr *fc_mx;
    int fc_mx_len;
    int fc_mp_len;
    struct nlattr *fc_mp;
    struct nl_info fc_nlinfo;
    struct nlattr *fc_encap;
    u16 fc_encap_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct fib6_config {
    u32 fc_table;
    u32 fc_metric;
    int fc_dst_len;
    int fc_src_len;
    int fc_ifindex;
    u32 fc_flags;
    u32 fc_protocol;
    u16 fc_type;
    u16 fc_delete_all_nh;
    u16 fc_ignore_dev_down;
    u16 __unused;
    u32 fc_nh_id;
    struct in6_addr fc_dst;
    struct in6_addr fc_src;
    struct in6_addr fc_prefsrc;
    struct in6_addr fc_gateway;
    long unsigned int fc_expires;
    struct nlattr *fc_mx;
    int fc_mx_len;
    int fc_mp_len;
    struct nlattr *fc_mp;
    struct nl_info fc_nlinfo;
    struct nlattr *fc_encap;
    u16 fc_encap_type;
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
struct fib6_config {
    u32 fc_table;
    u32 fc_metric;
    int fc_dst_len;
    int fc_src_len;
    int fc_ifindex;
    u32 fc_flags;
    u32 fc_protocol;
    u16 fc_type;
    u16 fc_delete_all_nh;
    u16 fc_ignore_dev_down;
    u16 __unused;
    u32 fc_nh_id;
    struct in6_addr fc_dst;
    struct in6_addr fc_src;
    struct in6_addr fc_prefsrc;
    struct in6_addr fc_gateway;
    long unsigned int fc_expires;
    struct nlattr *fc_mx;
    int fc_mx_len;
    int fc_mp_len;
    struct nlattr *fc_mp;
    struct nl_info fc_nlinfo;
    struct nlattr *fc_encap;
    u16 fc_encap_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct fib6_config {
    u32 fc_table;
    u32 fc_metric;
    int fc_dst_len;
    int fc_src_len;
    int fc_ifindex;
    u32 fc_flags;
    u32 fc_protocol;
    u16 fc_type;
    u16 fc_delete_all_nh;
    u16 fc_ignore_dev_down;
    u16 __unused;
    u32 fc_nh_id;
    struct in6_addr fc_dst;
    struct in6_addr fc_src;
    struct in6_addr fc_prefsrc;
    struct in6_addr fc_gateway;
    long unsigned int fc_expires;
    struct nlattr *fc_mx;
    int fc_mx_len;
    int fc_mp_len;
    struct nlattr *fc_mp;
    struct nl_info fc_nlinfo;
    struct nlattr *fc_encap;
    u16 fc_encap_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct fib6_config {
    u32 fc_table;
    u32 fc_metric;
    int fc_dst_len;
    int fc_src_len;
    int fc_ifindex;
    u32 fc_flags;
    u32 fc_protocol;
    u16 fc_type;
    u16 fc_delete_all_nh;
    u16 fc_ignore_dev_down;
    u16 __unused;
    u32 fc_nh_id;
    struct in6_addr fc_dst;
    struct in6_addr fc_src;
    struct in6_addr fc_prefsrc;
    struct in6_addr fc_gateway;
    long unsigned int fc_expires;
    struct nlattr *fc_mx;
    int fc_mx_len;
    int fc_mp_len;
    struct nlattr *fc_mp;
    struct nl_info fc_nlinfo;
    struct nlattr *fc_encap;
    u16 fc_encap_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct fib6_config {
    u32 fc_table;
    u32 fc_metric;
    int fc_dst_len;
    int fc_src_len;
    int fc_ifindex;
    u32 fc_flags;
    u32 fc_protocol;
    u16 fc_type;
    u16 fc_delete_all_nh;
    u16 fc_ignore_dev_down;
    u16 __unused;
    u32 fc_nh_id;
    struct in6_addr fc_dst;
    struct in6_addr fc_src;
    struct in6_addr fc_prefsrc;
    struct in6_addr fc_gateway;
    long unsigned int fc_expires;
    struct nlattr *fc_mx;
    int fc_mx_len;
    int fc_mp_len;
    struct nlattr *fc_mp;
    struct nl_info fc_nlinfo;
    struct nlattr *fc_encap;
    u16 fc_encap_type;
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
<code>u16 fc_delete_all_nh</code>
</li>
<li>
<b>Field added. </b>
<code>u16 __unused</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 fc_type</code> ➡️ <code>u16 fc_type</code>
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
<code>u16 fc_ignore_dev_down</code>
</li>
<li>
<b>Field added. </b>
<code>u32 fc_nh_id</code>
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
<b>Field added. </b>
<code>bool fc_is_fdb</code>
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
