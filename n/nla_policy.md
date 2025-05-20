# Struct: <code>nla_policy</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct nla_policy {
    u16 type;
    u16 len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct nla_policy {
    u16 type;
    u16 len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct nla_policy {
    u16 type;
    u16 len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct nla_policy {
    u16 type;
    u16 len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct nla_policy {
    u16 type;
    u16 len;
    void *validation_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct nla_policy {
    u16 type;
    u16 len;
    void *validation_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct nla_policy {
    u8 type;
    u8 validation_type;
    u16 len;
    const void *validation_data;
    s16 min;
    s16 max;
    int (*validate)(const struct nlattr *, struct netlink_ext_ack *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct nla_policy {
    u8 type;
    u8 validation_type;
    u16 len;
    const void *validation_data;
    s16 min;
    s16 max;
    int (*validate)(const struct nlattr *, struct netlink_ext_ack *);
    u16 strict_start_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct nla_policy {
    u8 type;
    u8 validation_type;
    u16 len;
    const void *validation_data;
    s16 min;
    s16 max;
    int (*validate)(const struct nlattr *, struct netlink_ext_ack *);
    u16 strict_start_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct nla_policy {
    u8 type;
    u8 validation_type;
    u16 len;
    const u32 bitfield32_valid;
    const char *reject_message;
    const struct nla_policy *nested_policy;
    struct netlink_range_validation *range;
    struct netlink_range_validation_signed *range_signed;
    s16 min;
    s16 max;
    int (*validate)(const struct nlattr *, struct netlink_ext_ack *);
    u16 strict_start_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct nla_policy {
    u8 type;
    u8 validation_type;
    u16 len;
    const u32 bitfield32_valid;
    const u32 mask;
    const char *reject_message;
    const struct nla_policy *nested_policy;
    struct netlink_range_validation *range;
    struct netlink_range_validation_signed *range_signed;
    s16 min;
    s16 max;
    int (*validate)(const struct nlattr *, struct netlink_ext_ack *);
    u16 strict_start_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct nla_policy {
    u8 type;
    u8 validation_type;
    u16 len;
    const u32 bitfield32_valid;
    const u32 mask;
    const char *reject_message;
    const struct nla_policy *nested_policy;
    struct netlink_range_validation *range;
    struct netlink_range_validation_signed *range_signed;
    s16 min;
    s16 max;
    int (*validate)(const struct nlattr *, struct netlink_ext_ack *);
    u16 strict_start_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct nla_policy {
    u8 type;
    u8 validation_type;
    u16 len;
    const u32 bitfield32_valid;
    const u32 mask;
    const char *reject_message;
    const struct nla_policy *nested_policy;
    struct netlink_range_validation *range;
    struct netlink_range_validation_signed *range_signed;
    s16 min;
    s16 max;
    int (*validate)(const struct nlattr *, struct netlink_ext_ack *);
    u16 strict_start_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct nla_policy {
    u8 type;
    u8 validation_type;
    u16 len;
    const u32 bitfield32_valid;
    const u32 mask;
    const char *reject_message;
    const struct nla_policy *nested_policy;
    struct netlink_range_validation *range;
    struct netlink_range_validation_signed *range_signed;
    s16 min;
    s16 max;
    int (*validate)(const struct nlattr *, struct netlink_ext_ack *);
    u16 strict_start_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct nla_policy {
    u8 type;
    u8 validation_type;
    u16 len;
    u16 strict_start_type;
    const u32 bitfield32_valid;
    const u32 mask;
    const char *reject_message;
    const struct nla_policy *nested_policy;
    struct netlink_range_validation *range;
    struct netlink_range_validation_signed *range_signed;
    s16 min;
    s16 max;
    int (*validate)(const struct nlattr *, struct netlink_ext_ack *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct nla_policy {
    u8 type;
    u8 validation_type;
    u16 len;
    u16 strict_start_type;
    const u32 bitfield32_valid;
    const u32 mask;
    const char *reject_message;
    const struct nla_policy *nested_policy;
    struct netlink_range_validation *range;
    struct netlink_range_validation_signed *range_signed;
    s16 min;
    s16 max;
    int (*validate)(const struct nlattr *, struct netlink_ext_ack *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct nla_policy {
    u8 type;
    u8 validation_type;
    u16 len;
    u16 strict_start_type;
    const u32 bitfield32_valid;
    const u32 mask;
    const char *reject_message;
    const struct nla_policy *nested_policy;
    const struct netlink_range_validation *range;
    const struct netlink_range_validation_signed *range_signed;
    s16 min;
    s16 max;
    int (*validate)(const struct nlattr *, struct netlink_ext_ack *);
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
struct nla_policy {
    u8 type;
    u8 validation_type;
    u16 len;
    const void *validation_data;
    s16 min;
    s16 max;
    int (*validate)(const struct nlattr *, struct netlink_ext_ack *);
    u16 strict_start_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct nla_policy {
    u8 type;
    u8 validation_type;
    u16 len;
    const void *validation_data;
    s16 min;
    s16 max;
    int (*validate)(const struct nlattr *, struct netlink_ext_ack *);
    u16 strict_start_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct nla_policy {
    u8 type;
    u8 validation_type;
    u16 len;
    const void *validation_data;
    s16 min;
    s16 max;
    int (*validate)(const struct nlattr *, struct netlink_ext_ack *);
    u16 strict_start_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct nla_policy {
    u8 type;
    u8 validation_type;
    u16 len;
    const void *validation_data;
    s16 min;
    s16 max;
    int (*validate)(const struct nlattr *, struct netlink_ext_ack *);
    u16 strict_start_type;
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
struct nla_policy {
    u8 type;
    u8 validation_type;
    u16 len;
    const void *validation_data;
    s16 min;
    s16 max;
    int (*validate)(const struct nlattr *, struct netlink_ext_ack *);
    u16 strict_start_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct nla_policy {
    u8 type;
    u8 validation_type;
    u16 len;
    const void *validation_data;
    s16 min;
    s16 max;
    int (*validate)(const struct nlattr *, struct netlink_ext_ack *);
    u16 strict_start_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct nla_policy {
    u8 type;
    u8 validation_type;
    u16 len;
    const void *validation_data;
    s16 min;
    s16 max;
    int (*validate)(const struct nlattr *, struct netlink_ext_ack *);
    u16 strict_start_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct nla_policy {
    u8 type;
    u8 validation_type;
    u16 len;
    const void *validation_data;
    s16 min;
    s16 max;
    int (*validate)(const struct nlattr *, struct netlink_ext_ack *);
    u16 strict_start_type;
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
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void *validation_data</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 validation_type</code>
</li>
<li>
<b>Field added. </b>
<code>s16 min</code>
</li>
<li>
<b>Field added. </b>
<code>s16 max</code>
</li>
<li>
<b>Field added. </b>
<code>int (*validate)(const struct nlattr *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>u16 type</code> ➡️ <code>u8 type</code>
</li>
<li>
<b>Field type changed. </b>
<code>void *validation_data</code> ➡️ <code>const void *validation_data</code>
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
<code>u16 strict_start_type</code>
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
<code>const u32 bitfield32_valid</code>
</li>
<li>
<b>Field added. </b>
<code>const char *reject_message</code>
</li>
<li>
<b>Field added. </b>
<code>const struct nla_policy *nested_policy</code>
</li>
<li>
<b>Field added. </b>
<code>struct netlink_range_validation *range</code>
</li>
<li>
<b>Field added. </b>
<code>struct netlink_range_validation_signed *range_signed</code>
</li>
<li>
<b>Field removed. </b>
<code>const void *validation_data</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const u32 mask</code>
</li>
</ul>
</details>
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
<code>struct netlink_range_validation *range</code> ➡️ <code>const struct netlink_range_validation *range</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct netlink_range_validation_signed *range_signed</code> ➡️ <code>const struct netlink_range_validation_signed *range_signed</code>
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
