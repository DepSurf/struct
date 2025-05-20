# Struct: <code>in_ifaddr</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct in_ifaddr {
    struct hlist_node hash;
    struct in_ifaddr *ifa_next;
    struct in_device *ifa_dev;
    struct callback_head callback_head;
    __be32 ifa_local;
    __be32 ifa_address;
    __be32 ifa_mask;
    __be32 ifa_broadcast;
    unsigned char ifa_scope;
    unsigned char ifa_prefixlen;
    __u32 ifa_flags;
    char ifa_label[16];
    __u32 ifa_valid_lft;
    __u32 ifa_preferred_lft;
    long unsigned int ifa_cstamp;
    long unsigned int ifa_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct in_ifaddr {
    struct hlist_node hash;
    struct in_ifaddr *ifa_next;
    struct in_device *ifa_dev;
    struct callback_head callback_head;
    __be32 ifa_local;
    __be32 ifa_address;
    __be32 ifa_mask;
    __be32 ifa_broadcast;
    unsigned char ifa_scope;
    unsigned char ifa_prefixlen;
    __u32 ifa_flags;
    char ifa_label[16];
    __u32 ifa_valid_lft;
    __u32 ifa_preferred_lft;
    long unsigned int ifa_cstamp;
    long unsigned int ifa_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct in_ifaddr {
    struct hlist_node hash;
    struct in_ifaddr *ifa_next;
    struct in_device *ifa_dev;
    struct callback_head callback_head;
    __be32 ifa_local;
    __be32 ifa_address;
    __be32 ifa_mask;
    __be32 ifa_broadcast;
    unsigned char ifa_scope;
    unsigned char ifa_prefixlen;
    __u32 ifa_flags;
    char ifa_label[16];
    __u32 ifa_valid_lft;
    __u32 ifa_preferred_lft;
    long unsigned int ifa_cstamp;
    long unsigned int ifa_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct in_ifaddr {
    struct hlist_node hash;
    struct in_ifaddr *ifa_next;
    struct in_device *ifa_dev;
    struct callback_head callback_head;
    __be32 ifa_local;
    __be32 ifa_address;
    __be32 ifa_mask;
    __be32 ifa_broadcast;
    unsigned char ifa_scope;
    unsigned char ifa_prefixlen;
    __u32 ifa_flags;
    char ifa_label[16];
    __u32 ifa_valid_lft;
    __u32 ifa_preferred_lft;
    long unsigned int ifa_cstamp;
    long unsigned int ifa_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct in_ifaddr {
    struct hlist_node hash;
    struct in_ifaddr *ifa_next;
    struct in_device *ifa_dev;
    struct callback_head callback_head;
    __be32 ifa_local;
    __be32 ifa_address;
    __be32 ifa_mask;
    __be32 ifa_broadcast;
    unsigned char ifa_scope;
    unsigned char ifa_prefixlen;
    __u32 ifa_flags;
    char ifa_label[16];
    __u32 ifa_valid_lft;
    __u32 ifa_preferred_lft;
    long unsigned int ifa_cstamp;
    long unsigned int ifa_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct in_ifaddr {
    struct hlist_node hash;
    struct in_ifaddr *ifa_next;
    struct in_device *ifa_dev;
    struct callback_head callback_head;
    __be32 ifa_local;
    __be32 ifa_address;
    __be32 ifa_mask;
    __u32 ifa_rt_priority;
    __be32 ifa_broadcast;
    unsigned char ifa_scope;
    unsigned char ifa_prefixlen;
    __u32 ifa_flags;
    char ifa_label[16];
    __u32 ifa_valid_lft;
    __u32 ifa_preferred_lft;
    long unsigned int ifa_cstamp;
    long unsigned int ifa_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct in_ifaddr {
    struct hlist_node hash;
    struct in_ifaddr *ifa_next;
    struct in_device *ifa_dev;
    struct callback_head callback_head;
    __be32 ifa_local;
    __be32 ifa_address;
    __be32 ifa_mask;
    __u32 ifa_rt_priority;
    __be32 ifa_broadcast;
    unsigned char ifa_scope;
    unsigned char ifa_prefixlen;
    __u32 ifa_flags;
    char ifa_label[16];
    __u32 ifa_valid_lft;
    __u32 ifa_preferred_lft;
    long unsigned int ifa_cstamp;
    long unsigned int ifa_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct in_ifaddr {
    struct hlist_node hash;
    struct in_ifaddr *ifa_next;
    struct in_device *ifa_dev;
    struct callback_head callback_head;
    __be32 ifa_local;
    __be32 ifa_address;
    __be32 ifa_mask;
    __u32 ifa_rt_priority;
    __be32 ifa_broadcast;
    unsigned char ifa_scope;
    unsigned char ifa_prefixlen;
    __u32 ifa_flags;
    char ifa_label[16];
    __u32 ifa_valid_lft;
    __u32 ifa_preferred_lft;
    long unsigned int ifa_cstamp;
    long unsigned int ifa_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct in_ifaddr {
    struct hlist_node hash;
    struct in_ifaddr *ifa_next;
    struct in_device *ifa_dev;
    struct callback_head callback_head;
    __be32 ifa_local;
    __be32 ifa_address;
    __be32 ifa_mask;
    __u32 ifa_rt_priority;
    __be32 ifa_broadcast;
    unsigned char ifa_scope;
    unsigned char ifa_prefixlen;
    __u32 ifa_flags;
    char ifa_label[16];
    __u32 ifa_valid_lft;
    __u32 ifa_preferred_lft;
    long unsigned int ifa_cstamp;
    long unsigned int ifa_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct in_ifaddr {
    struct hlist_node hash;
    struct in_ifaddr *ifa_next;
    struct in_device *ifa_dev;
    struct callback_head callback_head;
    __be32 ifa_local;
    __be32 ifa_address;
    __be32 ifa_mask;
    __u32 ifa_rt_priority;
    __be32 ifa_broadcast;
    unsigned char ifa_scope;
    unsigned char ifa_prefixlen;
    __u32 ifa_flags;
    char ifa_label[16];
    __u32 ifa_valid_lft;
    __u32 ifa_preferred_lft;
    long unsigned int ifa_cstamp;
    long unsigned int ifa_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct in_ifaddr {
    struct hlist_node hash;
    struct in_ifaddr *ifa_next;
    struct in_device *ifa_dev;
    struct callback_head callback_head;
    __be32 ifa_local;
    __be32 ifa_address;
    __be32 ifa_mask;
    __u32 ifa_rt_priority;
    __be32 ifa_broadcast;
    unsigned char ifa_scope;
    unsigned char ifa_prefixlen;
    __u32 ifa_flags;
    char ifa_label[16];
    __u32 ifa_valid_lft;
    __u32 ifa_preferred_lft;
    long unsigned int ifa_cstamp;
    long unsigned int ifa_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct in_ifaddr {
    struct hlist_node hash;
    struct in_ifaddr *ifa_next;
    struct in_device *ifa_dev;
    struct callback_head callback_head;
    __be32 ifa_local;
    __be32 ifa_address;
    __be32 ifa_mask;
    __u32 ifa_rt_priority;
    __be32 ifa_broadcast;
    unsigned char ifa_scope;
    unsigned char ifa_prefixlen;
    __u32 ifa_flags;
    char ifa_label[16];
    __u32 ifa_valid_lft;
    __u32 ifa_preferred_lft;
    long unsigned int ifa_cstamp;
    long unsigned int ifa_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct in_ifaddr {
    struct hlist_node hash;
    struct in_ifaddr *ifa_next;
    struct in_device *ifa_dev;
    struct callback_head callback_head;
    __be32 ifa_local;
    __be32 ifa_address;
    __be32 ifa_mask;
    __u32 ifa_rt_priority;
    __be32 ifa_broadcast;
    unsigned char ifa_scope;
    unsigned char ifa_prefixlen;
    __u32 ifa_flags;
    char ifa_label[16];
    __u32 ifa_valid_lft;
    __u32 ifa_preferred_lft;
    long unsigned int ifa_cstamp;
    long unsigned int ifa_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct in_ifaddr {
    struct hlist_node hash;
    struct in_ifaddr *ifa_next;
    struct in_device *ifa_dev;
    struct callback_head callback_head;
    __be32 ifa_local;
    __be32 ifa_address;
    __be32 ifa_mask;
    __u32 ifa_rt_priority;
    __be32 ifa_broadcast;
    unsigned char ifa_scope;
    unsigned char ifa_prefixlen;
    unsigned char ifa_proto;
    __u32 ifa_flags;
    char ifa_label[16];
    __u32 ifa_valid_lft;
    __u32 ifa_preferred_lft;
    long unsigned int ifa_cstamp;
    long unsigned int ifa_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct in_ifaddr {
    struct hlist_node hash;
    struct in_ifaddr *ifa_next;
    struct in_device *ifa_dev;
    struct callback_head callback_head;
    __be32 ifa_local;
    __be32 ifa_address;
    __be32 ifa_mask;
    __u32 ifa_rt_priority;
    __be32 ifa_broadcast;
    unsigned char ifa_scope;
    unsigned char ifa_prefixlen;
    unsigned char ifa_proto;
    __u32 ifa_flags;
    char ifa_label[16];
    __u32 ifa_valid_lft;
    __u32 ifa_preferred_lft;
    long unsigned int ifa_cstamp;
    long unsigned int ifa_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct in_ifaddr {
    struct hlist_node hash;
    struct in_ifaddr *ifa_next;
    struct in_device *ifa_dev;
    struct callback_head callback_head;
    __be32 ifa_local;
    __be32 ifa_address;
    __be32 ifa_mask;
    __u32 ifa_rt_priority;
    __be32 ifa_broadcast;
    unsigned char ifa_scope;
    unsigned char ifa_prefixlen;
    unsigned char ifa_proto;
    __u32 ifa_flags;
    char ifa_label[16];
    __u32 ifa_valid_lft;
    __u32 ifa_preferred_lft;
    long unsigned int ifa_cstamp;
    long unsigned int ifa_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct in_ifaddr {
    struct hlist_node hash;
    struct in_ifaddr *ifa_next;
    struct in_device *ifa_dev;
    struct callback_head callback_head;
    __be32 ifa_local;
    __be32 ifa_address;
    __be32 ifa_mask;
    __u32 ifa_rt_priority;
    __be32 ifa_broadcast;
    unsigned char ifa_scope;
    unsigned char ifa_prefixlen;
    unsigned char ifa_proto;
    __u32 ifa_flags;
    char ifa_label[16];
    __u32 ifa_valid_lft;
    __u32 ifa_preferred_lft;
    long unsigned int ifa_cstamp;
    long unsigned int ifa_tstamp;
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
struct in_ifaddr {
    struct hlist_node hash;
    struct in_ifaddr *ifa_next;
    struct in_device *ifa_dev;
    struct callback_head callback_head;
    __be32 ifa_local;
    __be32 ifa_address;
    __be32 ifa_mask;
    __u32 ifa_rt_priority;
    __be32 ifa_broadcast;
    unsigned char ifa_scope;
    unsigned char ifa_prefixlen;
    __u32 ifa_flags;
    char ifa_label[16];
    __u32 ifa_valid_lft;
    __u32 ifa_preferred_lft;
    long unsigned int ifa_cstamp;
    long unsigned int ifa_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct in_ifaddr {
    struct hlist_node hash;
    struct in_ifaddr *ifa_next;
    struct in_device *ifa_dev;
    struct callback_head callback_head;
    __be32 ifa_local;
    __be32 ifa_address;
    __be32 ifa_mask;
    __u32 ifa_rt_priority;
    __be32 ifa_broadcast;
    unsigned char ifa_scope;
    unsigned char ifa_prefixlen;
    __u32 ifa_flags;
    char ifa_label[16];
    __u32 ifa_valid_lft;
    __u32 ifa_preferred_lft;
    long unsigned int ifa_cstamp;
    long unsigned int ifa_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct in_ifaddr {
    struct hlist_node hash;
    struct in_ifaddr *ifa_next;
    struct in_device *ifa_dev;
    struct callback_head callback_head;
    __be32 ifa_local;
    __be32 ifa_address;
    __be32 ifa_mask;
    __u32 ifa_rt_priority;
    __be32 ifa_broadcast;
    unsigned char ifa_scope;
    unsigned char ifa_prefixlen;
    __u32 ifa_flags;
    char ifa_label[16];
    __u32 ifa_valid_lft;
    __u32 ifa_preferred_lft;
    long unsigned int ifa_cstamp;
    long unsigned int ifa_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct in_ifaddr {
    struct hlist_node hash;
    struct in_ifaddr *ifa_next;
    struct in_device *ifa_dev;
    struct callback_head callback_head;
    __be32 ifa_local;
    __be32 ifa_address;
    __be32 ifa_mask;
    __u32 ifa_rt_priority;
    __be32 ifa_broadcast;
    unsigned char ifa_scope;
    unsigned char ifa_prefixlen;
    __u32 ifa_flags;
    char ifa_label[16];
    __u32 ifa_valid_lft;
    __u32 ifa_preferred_lft;
    long unsigned int ifa_cstamp;
    long unsigned int ifa_tstamp;
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
struct in_ifaddr {
    struct hlist_node hash;
    struct in_ifaddr *ifa_next;
    struct in_device *ifa_dev;
    struct callback_head callback_head;
    __be32 ifa_local;
    __be32 ifa_address;
    __be32 ifa_mask;
    __u32 ifa_rt_priority;
    __be32 ifa_broadcast;
    unsigned char ifa_scope;
    unsigned char ifa_prefixlen;
    __u32 ifa_flags;
    char ifa_label[16];
    __u32 ifa_valid_lft;
    __u32 ifa_preferred_lft;
    long unsigned int ifa_cstamp;
    long unsigned int ifa_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct in_ifaddr {
    struct hlist_node hash;
    struct in_ifaddr *ifa_next;
    struct in_device *ifa_dev;
    struct callback_head callback_head;
    __be32 ifa_local;
    __be32 ifa_address;
    __be32 ifa_mask;
    __u32 ifa_rt_priority;
    __be32 ifa_broadcast;
    unsigned char ifa_scope;
    unsigned char ifa_prefixlen;
    __u32 ifa_flags;
    char ifa_label[16];
    __u32 ifa_valid_lft;
    __u32 ifa_preferred_lft;
    long unsigned int ifa_cstamp;
    long unsigned int ifa_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct in_ifaddr {
    struct hlist_node hash;
    struct in_ifaddr *ifa_next;
    struct in_device *ifa_dev;
    struct callback_head callback_head;
    __be32 ifa_local;
    __be32 ifa_address;
    __be32 ifa_mask;
    __u32 ifa_rt_priority;
    __be32 ifa_broadcast;
    unsigned char ifa_scope;
    unsigned char ifa_prefixlen;
    __u32 ifa_flags;
    char ifa_label[16];
    __u32 ifa_valid_lft;
    __u32 ifa_preferred_lft;
    long unsigned int ifa_cstamp;
    long unsigned int ifa_tstamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct in_ifaddr {
    struct hlist_node hash;
    struct in_ifaddr *ifa_next;
    struct in_device *ifa_dev;
    struct callback_head callback_head;
    __be32 ifa_local;
    __be32 ifa_address;
    __be32 ifa_mask;
    __u32 ifa_rt_priority;
    __be32 ifa_broadcast;
    unsigned char ifa_scope;
    unsigned char ifa_prefixlen;
    __u32 ifa_flags;
    char ifa_label[16];
    __u32 ifa_valid_lft;
    __u32 ifa_preferred_lft;
    long unsigned int ifa_cstamp;
    long unsigned int ifa_tstamp;
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
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u32 ifa_rt_priority</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned char ifa_proto</code>
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
