# Struct: <code>flowi_common</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct flowi_common {
    int flowic_oif;
    int flowic_iif;
    __u32 flowic_mark;
    __u8 flowic_tos;
    __u8 flowic_scope;
    __u8 flowic_proto;
    __u8 flowic_flags;
    __u32 flowic_secid;
    struct flowi_tunnel flowic_tun_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct flowi_common {
    int flowic_oif;
    int flowic_iif;
    __u32 flowic_mark;
    __u8 flowic_tos;
    __u8 flowic_scope;
    __u8 flowic_proto;
    __u8 flowic_flags;
    __u32 flowic_secid;
    struct flowi_tunnel flowic_tun_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct flowi_common {
    int flowic_oif;
    int flowic_iif;
    __u32 flowic_mark;
    __u8 flowic_tos;
    __u8 flowic_scope;
    __u8 flowic_proto;
    __u8 flowic_flags;
    __u32 flowic_secid;
    struct flowi_tunnel flowic_tun_key;
    kuid_t flowic_uid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct flowi_common {
    int flowic_oif;
    int flowic_iif;
    __u32 flowic_mark;
    __u8 flowic_tos;
    __u8 flowic_scope;
    __u8 flowic_proto;
    __u8 flowic_flags;
    __u32 flowic_secid;
    struct flowi_tunnel flowic_tun_key;
    kuid_t flowic_uid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct flowi_common {
    int flowic_oif;
    int flowic_iif;
    __u32 flowic_mark;
    __u8 flowic_tos;
    __u8 flowic_scope;
    __u8 flowic_proto;
    __u8 flowic_flags;
    __u32 flowic_secid;
    struct flowi_tunnel flowic_tun_key;
    kuid_t flowic_uid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct flowi_common {
    int flowic_oif;
    int flowic_iif;
    __u32 flowic_mark;
    __u8 flowic_tos;
    __u8 flowic_scope;
    __u8 flowic_proto;
    __u8 flowic_flags;
    __u32 flowic_secid;
    struct flowi_tunnel flowic_tun_key;
    kuid_t flowic_uid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct flowi_common {
    int flowic_oif;
    int flowic_iif;
    __u32 flowic_mark;
    __u8 flowic_tos;
    __u8 flowic_scope;
    __u8 flowic_proto;
    __u8 flowic_flags;
    __u32 flowic_secid;
    kuid_t flowic_uid;
    struct flowi_tunnel flowic_tun_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct flowi_common {
    int flowic_oif;
    int flowic_iif;
    __u32 flowic_mark;
    __u8 flowic_tos;
    __u8 flowic_scope;
    __u8 flowic_proto;
    __u8 flowic_flags;
    __u32 flowic_secid;
    kuid_t flowic_uid;
    struct flowi_tunnel flowic_tun_key;
    __u32 flowic_multipath_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct flowi_common {
    int flowic_oif;
    int flowic_iif;
    __u32 flowic_mark;
    __u8 flowic_tos;
    __u8 flowic_scope;
    __u8 flowic_proto;
    __u8 flowic_flags;
    __u32 flowic_secid;
    kuid_t flowic_uid;
    struct flowi_tunnel flowic_tun_key;
    __u32 flowic_multipath_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct flowi_common {
    int flowic_oif;
    int flowic_iif;
    __u32 flowic_mark;
    __u8 flowic_tos;
    __u8 flowic_scope;
    __u8 flowic_proto;
    __u8 flowic_flags;
    __u32 flowic_secid;
    kuid_t flowic_uid;
    struct flowi_tunnel flowic_tun_key;
    __u32 flowic_multipath_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct flowi_common {
    int flowic_oif;
    int flowic_iif;
    __u32 flowic_mark;
    __u8 flowic_tos;
    __u8 flowic_scope;
    __u8 flowic_proto;
    __u8 flowic_flags;
    __u32 flowic_secid;
    kuid_t flowic_uid;
    struct flowi_tunnel flowic_tun_key;
    __u32 flowic_multipath_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct flowi_common {
    int flowic_oif;
    int flowic_iif;
    __u32 flowic_mark;
    __u8 flowic_tos;
    __u8 flowic_scope;
    __u8 flowic_proto;
    __u8 flowic_flags;
    __u32 flowic_secid;
    kuid_t flowic_uid;
    struct flowi_tunnel flowic_tun_key;
    __u32 flowic_multipath_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct flowi_common {
    int flowic_oif;
    int flowic_iif;
    __u32 flowic_mark;
    __u8 flowic_tos;
    __u8 flowic_scope;
    __u8 flowic_proto;
    __u8 flowic_flags;
    __u32 flowic_secid;
    kuid_t flowic_uid;
    struct flowi_tunnel flowic_tun_key;
    __u32 flowic_multipath_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct flowi_common {
    int flowic_oif;
    int flowic_iif;
    int flowic_l3mdev;
    __u32 flowic_mark;
    __u8 flowic_tos;
    __u8 flowic_scope;
    __u8 flowic_proto;
    __u8 flowic_flags;
    __u32 flowic_secid;
    kuid_t flowic_uid;
    struct flowi_tunnel flowic_tun_key;
    __u32 flowic_multipath_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct flowi_common {
    int flowic_oif;
    int flowic_iif;
    int flowic_l3mdev;
    __u32 flowic_mark;
    __u8 flowic_tos;
    __u8 flowic_scope;
    __u8 flowic_proto;
    __u8 flowic_flags;
    __u32 flowic_secid;
    kuid_t flowic_uid;
    struct flowi_tunnel flowic_tun_key;
    __u32 flowic_multipath_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct flowi_common {
    int flowic_oif;
    int flowic_iif;
    int flowic_l3mdev;
    __u32 flowic_mark;
    __u8 flowic_tos;
    __u8 flowic_scope;
    __u8 flowic_proto;
    __u8 flowic_flags;
    __u32 flowic_secid;
    kuid_t flowic_uid;
    struct flowi_tunnel flowic_tun_key;
    __u32 flowic_multipath_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct flowi_common {
    int flowic_oif;
    int flowic_iif;
    int flowic_l3mdev;
    __u32 flowic_mark;
    __u8 flowic_tos;
    __u8 flowic_scope;
    __u8 flowic_proto;
    __u8 flowic_flags;
    __u32 flowic_secid;
    kuid_t flowic_uid;
    __u32 flowic_multipath_hash;
    struct flowi_tunnel flowic_tun_key;
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
struct flowi_common {
    int flowic_oif;
    int flowic_iif;
    __u32 flowic_mark;
    __u8 flowic_tos;
    __u8 flowic_scope;
    __u8 flowic_proto;
    __u8 flowic_flags;
    __u32 flowic_secid;
    kuid_t flowic_uid;
    struct flowi_tunnel flowic_tun_key;
    __u32 flowic_multipath_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct flowi_common {
    int flowic_oif;
    int flowic_iif;
    __u32 flowic_mark;
    __u8 flowic_tos;
    __u8 flowic_scope;
    __u8 flowic_proto;
    __u8 flowic_flags;
    __u32 flowic_secid;
    kuid_t flowic_uid;
    struct flowi_tunnel flowic_tun_key;
    __u32 flowic_multipath_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct flowi_common {
    int flowic_oif;
    int flowic_iif;
    __u32 flowic_mark;
    __u8 flowic_tos;
    __u8 flowic_scope;
    __u8 flowic_proto;
    __u8 flowic_flags;
    __u32 flowic_secid;
    kuid_t flowic_uid;
    struct flowi_tunnel flowic_tun_key;
    __u32 flowic_multipath_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct flowi_common {
    int flowic_oif;
    int flowic_iif;
    __u32 flowic_mark;
    __u8 flowic_tos;
    __u8 flowic_scope;
    __u8 flowic_proto;
    __u8 flowic_flags;
    __u32 flowic_secid;
    kuid_t flowic_uid;
    struct flowi_tunnel flowic_tun_key;
    __u32 flowic_multipath_hash;
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
struct flowi_common {
    int flowic_oif;
    int flowic_iif;
    __u32 flowic_mark;
    __u8 flowic_tos;
    __u8 flowic_scope;
    __u8 flowic_proto;
    __u8 flowic_flags;
    __u32 flowic_secid;
    kuid_t flowic_uid;
    struct flowi_tunnel flowic_tun_key;
    __u32 flowic_multipath_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct flowi_common {
    int flowic_oif;
    int flowic_iif;
    __u32 flowic_mark;
    __u8 flowic_tos;
    __u8 flowic_scope;
    __u8 flowic_proto;
    __u8 flowic_flags;
    __u32 flowic_secid;
    kuid_t flowic_uid;
    struct flowi_tunnel flowic_tun_key;
    __u32 flowic_multipath_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct flowi_common {
    int flowic_oif;
    int flowic_iif;
    __u32 flowic_mark;
    __u8 flowic_tos;
    __u8 flowic_scope;
    __u8 flowic_proto;
    __u8 flowic_flags;
    __u32 flowic_secid;
    kuid_t flowic_uid;
    struct flowi_tunnel flowic_tun_key;
    __u32 flowic_multipath_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct flowi_common {
    int flowic_oif;
    int flowic_iif;
    __u32 flowic_mark;
    __u8 flowic_tos;
    __u8 flowic_scope;
    __u8 flowic_proto;
    __u8 flowic_flags;
    __u32 flowic_secid;
    kuid_t flowic_uid;
    struct flowi_tunnel flowic_tun_key;
    __u32 flowic_multipath_hash;
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
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>kuid_t flowic_uid</code>
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u32 flowic_multipath_hash</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int flowic_l3mdev</code>
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
