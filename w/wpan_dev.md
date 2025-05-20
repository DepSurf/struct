# Struct: <code>wpan_dev</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct wpan_dev {
    struct wpan_phy *wpan_phy;
    int iftype;
    struct list_head list;
    struct net_device *netdev;
    const struct wpan_dev_header_ops *header_ops;
    struct net_device *lowpan_dev;
    u32 identifier;
    __le16 pan_id;
    __le16 short_addr;
    __le64 extended_addr;
    atomic_t bsn;
    atomic_t dsn;
    u8 min_be;
    u8 max_be;
    u8 csma_retries;
    s8 frame_retries;
    bool lbt;
    bool promiscuous_mode;
    bool ackreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct wpan_dev {
    struct wpan_phy *wpan_phy;
    int iftype;
    struct list_head list;
    struct net_device *netdev;
    const struct wpan_dev_header_ops *header_ops;
    struct net_device *lowpan_dev;
    u32 identifier;
    __le16 pan_id;
    __le16 short_addr;
    __le64 extended_addr;
    atomic_t bsn;
    atomic_t dsn;
    u8 min_be;
    u8 max_be;
    u8 csma_retries;
    s8 frame_retries;
    bool lbt;
    bool promiscuous_mode;
    bool ackreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct wpan_dev {
    struct wpan_phy *wpan_phy;
    int iftype;
    struct list_head list;
    struct net_device *netdev;
    const struct wpan_dev_header_ops *header_ops;
    struct net_device *lowpan_dev;
    u32 identifier;
    __le16 pan_id;
    __le16 short_addr;
    __le64 extended_addr;
    atomic_t bsn;
    atomic_t dsn;
    u8 min_be;
    u8 max_be;
    u8 csma_retries;
    s8 frame_retries;
    bool lbt;
    bool promiscuous_mode;
    bool ackreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct wpan_dev {
    struct wpan_phy *wpan_phy;
    int iftype;
    struct list_head list;
    struct net_device *netdev;
    const struct wpan_dev_header_ops *header_ops;
    struct net_device *lowpan_dev;
    u32 identifier;
    __le16 pan_id;
    __le16 short_addr;
    __le64 extended_addr;
    atomic_t bsn;
    atomic_t dsn;
    u8 min_be;
    u8 max_be;
    u8 csma_retries;
    s8 frame_retries;
    bool lbt;
    bool promiscuous_mode;
    bool ackreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct wpan_dev {
    struct wpan_phy *wpan_phy;
    int iftype;
    struct list_head list;
    struct net_device *netdev;
    const struct wpan_dev_header_ops *header_ops;
    struct net_device *lowpan_dev;
    u32 identifier;
    __le16 pan_id;
    __le16 short_addr;
    __le64 extended_addr;
    atomic_t bsn;
    atomic_t dsn;
    u8 min_be;
    u8 max_be;
    u8 csma_retries;
    s8 frame_retries;
    bool lbt;
    bool promiscuous_mode;
    bool ackreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct wpan_dev {
    struct wpan_phy *wpan_phy;
    int iftype;
    struct list_head list;
    struct net_device *netdev;
    const struct wpan_dev_header_ops *header_ops;
    struct net_device *lowpan_dev;
    u32 identifier;
    __le16 pan_id;
    __le16 short_addr;
    __le64 extended_addr;
    atomic_t bsn;
    atomic_t dsn;
    u8 min_be;
    u8 max_be;
    u8 csma_retries;
    s8 frame_retries;
    bool lbt;
    bool promiscuous_mode;
    bool ackreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct wpan_dev {
    struct wpan_phy *wpan_phy;
    int iftype;
    struct list_head list;
    struct net_device *netdev;
    const struct wpan_dev_header_ops *header_ops;
    struct net_device *lowpan_dev;
    u32 identifier;
    __le16 pan_id;
    __le16 short_addr;
    __le64 extended_addr;
    atomic_t bsn;
    atomic_t dsn;
    u8 min_be;
    u8 max_be;
    u8 csma_retries;
    s8 frame_retries;
    bool lbt;
    bool promiscuous_mode;
    bool ackreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct wpan_dev {
    struct wpan_phy *wpan_phy;
    int iftype;
    struct list_head list;
    struct net_device *netdev;
    const struct wpan_dev_header_ops *header_ops;
    struct net_device *lowpan_dev;
    u32 identifier;
    __le16 pan_id;
    __le16 short_addr;
    __le64 extended_addr;
    atomic_t bsn;
    atomic_t dsn;
    u8 min_be;
    u8 max_be;
    u8 csma_retries;
    s8 frame_retries;
    bool lbt;
    bool promiscuous_mode;
    bool ackreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct wpan_dev {
    struct wpan_phy *wpan_phy;
    int iftype;
    struct list_head list;
    struct net_device *netdev;
    const struct wpan_dev_header_ops *header_ops;
    struct net_device *lowpan_dev;
    u32 identifier;
    __le16 pan_id;
    __le16 short_addr;
    __le64 extended_addr;
    atomic_t bsn;
    atomic_t dsn;
    u8 min_be;
    u8 max_be;
    u8 csma_retries;
    s8 frame_retries;
    bool lbt;
    bool promiscuous_mode;
    bool ackreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct wpan_dev {
    struct wpan_phy *wpan_phy;
    int iftype;
    struct list_head list;
    struct net_device *netdev;
    const struct wpan_dev_header_ops *header_ops;
    struct net_device *lowpan_dev;
    u32 identifier;
    __le16 pan_id;
    __le16 short_addr;
    __le64 extended_addr;
    atomic_t bsn;
    atomic_t dsn;
    u8 min_be;
    u8 max_be;
    u8 csma_retries;
    s8 frame_retries;
    bool lbt;
    bool promiscuous_mode;
    bool ackreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct wpan_dev {
    struct wpan_phy *wpan_phy;
    int iftype;
    struct list_head list;
    struct net_device *netdev;
    const struct wpan_dev_header_ops *header_ops;
    struct net_device *lowpan_dev;
    u32 identifier;
    __le16 pan_id;
    __le16 short_addr;
    __le64 extended_addr;
    atomic_t bsn;
    atomic_t dsn;
    u8 min_be;
    u8 max_be;
    u8 csma_retries;
    s8 frame_retries;
    bool lbt;
    bool promiscuous_mode;
    bool ackreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct wpan_dev {
    struct wpan_phy *wpan_phy;
    int iftype;
    struct list_head list;
    struct net_device *netdev;
    const struct wpan_dev_header_ops *header_ops;
    struct net_device *lowpan_dev;
    u32 identifier;
    __le16 pan_id;
    __le16 short_addr;
    __le64 extended_addr;
    atomic_t bsn;
    atomic_t dsn;
    u8 min_be;
    u8 max_be;
    u8 csma_retries;
    s8 frame_retries;
    bool lbt;
    bool promiscuous_mode;
    bool ackreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct wpan_dev {
    struct wpan_phy *wpan_phy;
    int iftype;
    struct list_head list;
    struct net_device *netdev;
    const struct wpan_dev_header_ops *header_ops;
    struct net_device *lowpan_dev;
    u32 identifier;
    __le16 pan_id;
    __le16 short_addr;
    __le64 extended_addr;
    atomic_t bsn;
    atomic_t dsn;
    u8 min_be;
    u8 max_be;
    u8 csma_retries;
    s8 frame_retries;
    bool lbt;
    bool promiscuous_mode;
    bool ackreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct wpan_dev {
    struct wpan_phy *wpan_phy;
    int iftype;
    struct list_head list;
    struct net_device *netdev;
    const struct wpan_dev_header_ops *header_ops;
    struct net_device *lowpan_dev;
    u32 identifier;
    __le16 pan_id;
    __le16 short_addr;
    __le64 extended_addr;
    atomic_t bsn;
    atomic_t dsn;
    u8 min_be;
    u8 max_be;
    u8 csma_retries;
    s8 frame_retries;
    bool lbt;
    bool ackreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct wpan_dev {
    struct wpan_phy *wpan_phy;
    int iftype;
    struct list_head list;
    struct net_device *netdev;
    const struct wpan_dev_header_ops *header_ops;
    struct net_device *lowpan_dev;
    u32 identifier;
    __le16 pan_id;
    __le16 short_addr;
    __le64 extended_addr;
    atomic_t bsn;
    atomic_t dsn;
    u8 min_be;
    u8 max_be;
    u8 csma_retries;
    s8 frame_retries;
    bool lbt;
    bool ackreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct wpan_dev {
    struct wpan_phy *wpan_phy;
    int iftype;
    struct list_head list;
    struct net_device *netdev;
    const struct wpan_dev_header_ops *header_ops;
    struct net_device *lowpan_dev;
    u32 identifier;
    __le16 pan_id;
    __le16 short_addr;
    __le64 extended_addr;
    atomic_t bsn;
    atomic_t dsn;
    u8 min_be;
    u8 max_be;
    u8 csma_retries;
    s8 frame_retries;
    bool lbt;
    bool ackreq;
    struct mutex association_lock;
    struct ieee802154_pan_device *parent;
    struct list_head children;
    unsigned int max_associations;
    unsigned int nchildren;
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
struct wpan_dev {
    struct wpan_phy *wpan_phy;
    int iftype;
    struct list_head list;
    struct net_device *netdev;
    const struct wpan_dev_header_ops *header_ops;
    struct net_device *lowpan_dev;
    u32 identifier;
    __le16 pan_id;
    __le16 short_addr;
    __le64 extended_addr;
    atomic_t bsn;
    atomic_t dsn;
    u8 min_be;
    u8 max_be;
    u8 csma_retries;
    s8 frame_retries;
    bool lbt;
    bool promiscuous_mode;
    bool ackreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct wpan_dev {
    struct wpan_phy *wpan_phy;
    int iftype;
    struct list_head list;
    struct net_device *netdev;
    const struct wpan_dev_header_ops *header_ops;
    struct net_device *lowpan_dev;
    u32 identifier;
    __le16 pan_id;
    __le16 short_addr;
    __le64 extended_addr;
    atomic_t bsn;
    atomic_t dsn;
    u8 min_be;
    u8 max_be;
    u8 csma_retries;
    s8 frame_retries;
    bool lbt;
    bool promiscuous_mode;
    bool ackreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct wpan_dev {
    struct wpan_phy *wpan_phy;
    int iftype;
    struct list_head list;
    struct net_device *netdev;
    const struct wpan_dev_header_ops *header_ops;
    struct net_device *lowpan_dev;
    u32 identifier;
    __le16 pan_id;
    __le16 short_addr;
    __le64 extended_addr;
    atomic_t bsn;
    atomic_t dsn;
    u8 min_be;
    u8 max_be;
    u8 csma_retries;
    s8 frame_retries;
    bool lbt;
    bool promiscuous_mode;
    bool ackreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct wpan_dev {
    struct wpan_phy *wpan_phy;
    int iftype;
    struct list_head list;
    struct net_device *netdev;
    const struct wpan_dev_header_ops *header_ops;
    struct net_device *lowpan_dev;
    u32 identifier;
    __le16 pan_id;
    __le16 short_addr;
    __le64 extended_addr;
    atomic_t bsn;
    atomic_t dsn;
    u8 min_be;
    u8 max_be;
    u8 csma_retries;
    s8 frame_retries;
    bool lbt;
    bool promiscuous_mode;
    bool ackreq;
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
struct wpan_dev {
    struct wpan_phy *wpan_phy;
    int iftype;
    struct list_head list;
    struct net_device *netdev;
    const struct wpan_dev_header_ops *header_ops;
    struct net_device *lowpan_dev;
    u32 identifier;
    __le16 pan_id;
    __le16 short_addr;
    __le64 extended_addr;
    atomic_t bsn;
    atomic_t dsn;
    u8 min_be;
    u8 max_be;
    u8 csma_retries;
    s8 frame_retries;
    bool lbt;
    bool promiscuous_mode;
    bool ackreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct wpan_dev {
    struct wpan_phy *wpan_phy;
    int iftype;
    struct list_head list;
    struct net_device *netdev;
    const struct wpan_dev_header_ops *header_ops;
    struct net_device *lowpan_dev;
    u32 identifier;
    __le16 pan_id;
    __le16 short_addr;
    __le64 extended_addr;
    atomic_t bsn;
    atomic_t dsn;
    u8 min_be;
    u8 max_be;
    u8 csma_retries;
    s8 frame_retries;
    bool lbt;
    bool promiscuous_mode;
    bool ackreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct wpan_dev {
    struct wpan_phy *wpan_phy;
    int iftype;
    struct list_head list;
    struct net_device *netdev;
    const struct wpan_dev_header_ops *header_ops;
    struct net_device *lowpan_dev;
    u32 identifier;
    __le16 pan_id;
    __le16 short_addr;
    __le64 extended_addr;
    atomic_t bsn;
    atomic_t dsn;
    u8 min_be;
    u8 max_be;
    u8 csma_retries;
    s8 frame_retries;
    bool lbt;
    bool promiscuous_mode;
    bool ackreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct wpan_dev {
    struct wpan_phy *wpan_phy;
    int iftype;
    struct list_head list;
    struct net_device *netdev;
    const struct wpan_dev_header_ops *header_ops;
    struct net_device *lowpan_dev;
    u32 identifier;
    __le16 pan_id;
    __le16 short_addr;
    __le64 extended_addr;
    atomic_t bsn;
    atomic_t dsn;
    u8 min_be;
    u8 max_be;
    u8 csma_retries;
    s8 frame_retries;
    bool lbt;
    bool promiscuous_mode;
    bool ackreq;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>bool promiscuous_mode</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct mutex association_lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct ieee802154_pan_device *parent</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head children</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int max_associations</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int nchildren</code>
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
