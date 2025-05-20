# Struct: <code>wpan_phy</code>

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
struct wpan_phy {
    const void *privid;
    u32 flags;
    u8 current_channel;
    u8 current_page;
    struct wpan_phy_supported supported;
    s32 transmit_power;
    struct wpan_phy_cca cca;
    __le64 perm_extended_addr;
    s32 cca_ed_level;
    u8 symbol_duration;
    u16 lifs_period;
    u16 sifs_period;
    struct device dev;
    possible_net_t _net;
    char priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct wpan_phy {
    const void *privid;
    u32 flags;
    u8 current_channel;
    u8 current_page;
    struct wpan_phy_supported supported;
    s32 transmit_power;
    struct wpan_phy_cca cca;
    __le64 perm_extended_addr;
    s32 cca_ed_level;
    u8 symbol_duration;
    u16 lifs_period;
    u16 sifs_period;
    struct device dev;
    possible_net_t _net;
    char priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct wpan_phy {
    const void *privid;
    u32 flags;
    u8 current_channel;
    u8 current_page;
    struct wpan_phy_supported supported;
    s32 transmit_power;
    struct wpan_phy_cca cca;
    __le64 perm_extended_addr;
    s32 cca_ed_level;
    u8 symbol_duration;
    u16 lifs_period;
    u16 sifs_period;
    struct device dev;
    possible_net_t _net;
    char priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct wpan_phy {
    const void *privid;
    u32 flags;
    u8 current_channel;
    u8 current_page;
    struct wpan_phy_supported supported;
    s32 transmit_power;
    struct wpan_phy_cca cca;
    __le64 perm_extended_addr;
    s32 cca_ed_level;
    u8 symbol_duration;
    u16 lifs_period;
    u16 sifs_period;
    struct device dev;
    possible_net_t _net;
    char priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct wpan_phy {
    const void *privid;
    u32 flags;
    u8 current_channel;
    u8 current_page;
    struct wpan_phy_supported supported;
    s32 transmit_power;
    struct wpan_phy_cca cca;
    __le64 perm_extended_addr;
    s32 cca_ed_level;
    u8 symbol_duration;
    u16 lifs_period;
    u16 sifs_period;
    struct device dev;
    possible_net_t _net;
    char priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct wpan_phy {
    const void *privid;
    u32 flags;
    u8 current_channel;
    u8 current_page;
    struct wpan_phy_supported supported;
    s32 transmit_power;
    struct wpan_phy_cca cca;
    __le64 perm_extended_addr;
    s32 cca_ed_level;
    u8 symbol_duration;
    u16 lifs_period;
    u16 sifs_period;
    struct device dev;
    possible_net_t _net;
    char priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct wpan_phy {
    const void *privid;
    u32 flags;
    u8 current_channel;
    u8 current_page;
    struct wpan_phy_supported supported;
    s32 transmit_power;
    struct wpan_phy_cca cca;
    __le64 perm_extended_addr;
    s32 cca_ed_level;
    u8 symbol_duration;
    u16 lifs_period;
    u16 sifs_period;
    struct device dev;
    possible_net_t _net;
    char priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct wpan_phy {
    const void *privid;
    u32 flags;
    u8 current_channel;
    u8 current_page;
    struct wpan_phy_supported supported;
    s32 transmit_power;
    struct wpan_phy_cca cca;
    __le64 perm_extended_addr;
    s32 cca_ed_level;
    u8 symbol_duration;
    u16 lifs_period;
    u16 sifs_period;
    struct device dev;
    possible_net_t _net;
    char priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct wpan_phy {
    const void *privid;
    u32 flags;
    u8 current_channel;
    u8 current_page;
    struct wpan_phy_supported supported;
    s32 transmit_power;
    struct wpan_phy_cca cca;
    __le64 perm_extended_addr;
    s32 cca_ed_level;
    u8 symbol_duration;
    u16 lifs_period;
    u16 sifs_period;
    struct device dev;
    possible_net_t _net;
    char priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct wpan_phy {
    const void *privid;
    u32 flags;
    u8 current_channel;
    u8 current_page;
    struct wpan_phy_supported supported;
    s32 transmit_power;
    struct wpan_phy_cca cca;
    __le64 perm_extended_addr;
    s32 cca_ed_level;
    u8 symbol_duration;
    u16 lifs_period;
    u16 sifs_period;
    struct device dev;
    possible_net_t _net;
    char priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct wpan_phy {
    const void *privid;
    u32 flags;
    u8 current_channel;
    u8 current_page;
    struct wpan_phy_supported supported;
    s32 transmit_power;
    struct wpan_phy_cca cca;
    __le64 perm_extended_addr;
    s32 cca_ed_level;
    u8 symbol_duration;
    u16 lifs_period;
    u16 sifs_period;
    struct device dev;
    possible_net_t _net;
    char priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct wpan_phy {
    const void *privid;
    u32 flags;
    u8 current_channel;
    u8 current_page;
    struct wpan_phy_supported supported;
    s32 transmit_power;
    struct wpan_phy_cca cca;
    __le64 perm_extended_addr;
    s32 cca_ed_level;
    u8 symbol_duration;
    u16 lifs_period;
    u16 sifs_period;
    struct device dev;
    possible_net_t _net;
    char priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct wpan_phy {
    const void *privid;
    u32 flags;
    u8 current_channel;
    u8 current_page;
    struct wpan_phy_supported supported;
    s32 transmit_power;
    struct wpan_phy_cca cca;
    __le64 perm_extended_addr;
    s32 cca_ed_level;
    u32 symbol_duration;
    u16 lifs_period;
    u16 sifs_period;
    struct device dev;
    possible_net_t _net;
    char priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct wpan_phy {
    const void *privid;
    long unsigned int flags;
    u8 current_channel;
    u8 current_page;
    struct wpan_phy_supported supported;
    s32 transmit_power;
    struct wpan_phy_cca cca;
    __le64 perm_extended_addr;
    s32 cca_ed_level;
    u32 symbol_duration;
    u16 lifs_period;
    u16 sifs_period;
    struct device dev;
    possible_net_t _net;
    spinlock_t queue_lock;
    atomic_t ongoing_txs;
    atomic_t hold_txs;
    wait_queue_head_t sync_txq;
    enum ieee802154_filtering_level filtering;
    char priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct wpan_phy {
    const void *privid;
    long unsigned int flags;
    u8 current_channel;
    u8 current_page;
    struct wpan_phy_supported supported;
    s32 transmit_power;
    struct wpan_phy_cca cca;
    __le64 perm_extended_addr;
    s32 cca_ed_level;
    u32 symbol_duration;
    u16 lifs_period;
    u16 sifs_period;
    struct device dev;
    possible_net_t _net;
    spinlock_t queue_lock;
    atomic_t ongoing_txs;
    atomic_t hold_txs;
    wait_queue_head_t sync_txq;
    enum ieee802154_filtering_level filtering;
    char priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct wpan_phy {
    const void *privid;
    long unsigned int flags;
    u8 current_channel;
    u8 current_page;
    struct wpan_phy_supported supported;
    s32 transmit_power;
    struct wpan_phy_cca cca;
    __le64 perm_extended_addr;
    s32 cca_ed_level;
    u32 symbol_duration;
    u16 lifs_period;
    u16 sifs_period;
    struct device dev;
    possible_net_t _net;
    spinlock_t queue_lock;
    atomic_t ongoing_txs;
    atomic_t hold_txs;
    wait_queue_head_t sync_txq;
    enum ieee802154_filtering_level filtering;
    char priv[0];
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
struct wpan_phy {
    const void *privid;
    u32 flags;
    u8 current_channel;
    u8 current_page;
    struct wpan_phy_supported supported;
    s32 transmit_power;
    struct wpan_phy_cca cca;
    __le64 perm_extended_addr;
    s32 cca_ed_level;
    u8 symbol_duration;
    u16 lifs_period;
    u16 sifs_period;
    struct device dev;
    possible_net_t _net;
    char priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct wpan_phy {
    const void *privid;
    u32 flags;
    u8 current_channel;
    u8 current_page;
    struct wpan_phy_supported supported;
    s32 transmit_power;
    struct wpan_phy_cca cca;
    __le64 perm_extended_addr;
    s32 cca_ed_level;
    u8 symbol_duration;
    u16 lifs_period;
    u16 sifs_period;
    struct device dev;
    possible_net_t _net;
    char priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct wpan_phy {
    const void *privid;
    u32 flags;
    u8 current_channel;
    u8 current_page;
    struct wpan_phy_supported supported;
    s32 transmit_power;
    struct wpan_phy_cca cca;
    __le64 perm_extended_addr;
    s32 cca_ed_level;
    u8 symbol_duration;
    u16 lifs_period;
    u16 sifs_period;
    struct device dev;
    possible_net_t _net;
    char priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct wpan_phy {
    const void *privid;
    u32 flags;
    u8 current_channel;
    u8 current_page;
    struct wpan_phy_supported supported;
    s32 transmit_power;
    struct wpan_phy_cca cca;
    __le64 perm_extended_addr;
    s32 cca_ed_level;
    u8 symbol_duration;
    u16 lifs_period;
    u16 sifs_period;
    struct device dev;
    possible_net_t _net;
    char priv[0];
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
struct wpan_phy {
    const void *privid;
    u32 flags;
    u8 current_channel;
    u8 current_page;
    struct wpan_phy_supported supported;
    s32 transmit_power;
    struct wpan_phy_cca cca;
    __le64 perm_extended_addr;
    s32 cca_ed_level;
    u8 symbol_duration;
    u16 lifs_period;
    u16 sifs_period;
    struct device dev;
    possible_net_t _net;
    char priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct wpan_phy {
    const void *privid;
    u32 flags;
    u8 current_channel;
    u8 current_page;
    struct wpan_phy_supported supported;
    s32 transmit_power;
    struct wpan_phy_cca cca;
    __le64 perm_extended_addr;
    s32 cca_ed_level;
    u8 symbol_duration;
    u16 lifs_period;
    u16 sifs_period;
    struct device dev;
    possible_net_t _net;
    char priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct wpan_phy {
    const void *privid;
    u32 flags;
    u8 current_channel;
    u8 current_page;
    struct wpan_phy_supported supported;
    s32 transmit_power;
    struct wpan_phy_cca cca;
    __le64 perm_extended_addr;
    s32 cca_ed_level;
    u8 symbol_duration;
    u16 lifs_period;
    u16 sifs_period;
    struct device dev;
    possible_net_t _net;
    char priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct wpan_phy {
    const void *privid;
    u32 flags;
    u8 current_channel;
    u8 current_page;
    struct wpan_phy_supported supported;
    s32 transmit_power;
    struct wpan_phy_cca cca;
    __le64 perm_extended_addr;
    s32 cca_ed_level;
    u8 symbol_duration;
    u16 lifs_period;
    u16 sifs_period;
    struct device dev;
    possible_net_t _net;
    char priv[0];
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>u8 symbol_duration</code> ➡️ <code>u32 symbol_duration</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>spinlock_t queue_lock</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t ongoing_txs</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t hold_txs</code>
</li>
<li>
<b>Field added. </b>
<code>wait_queue_head_t sync_txq</code>
</li>
<li>
<b>Field added. </b>
<code>enum ieee802154_filtering_level filtering</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 flags</code> ➡️ <code>long unsigned int flags</code>
</li>
</ul>
</details>
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
