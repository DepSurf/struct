# Struct: <code>cfg80211_sched_scan_request</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct cfg80211_sched_scan_request {
    struct cfg80211_ssid *ssids;
    int n_ssids;
    u32 n_channels;
    enum nl80211_bss_scan_width scan_width;
    const u8 *ie;
    size_t ie_len;
    u32 flags;
    struct cfg80211_match_set *match_sets;
    int n_match_sets;
    s32 min_rssi_thold;
    u32 delay;
    struct cfg80211_sched_scan_plan *scan_plans;
    int n_scan_plans;
    u8 mac_addr[6];
    u8 mac_addr_mask[6];
    struct wiphy *wiphy;
    struct net_device *dev;
    long unsigned int scan_start;
    struct callback_head callback_head;
    u32 owner_nlportid;
    struct ieee80211_channel * channels[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct cfg80211_sched_scan_request {
    struct cfg80211_ssid *ssids;
    int n_ssids;
    u32 n_channels;
    enum nl80211_bss_scan_width scan_width;
    const u8 *ie;
    size_t ie_len;
    u32 flags;
    struct cfg80211_match_set *match_sets;
    int n_match_sets;
    s32 min_rssi_thold;
    u32 delay;
    struct cfg80211_sched_scan_plan *scan_plans;
    int n_scan_plans;
    u8 mac_addr[6];
    u8 mac_addr_mask[6];
    struct wiphy *wiphy;
    struct net_device *dev;
    long unsigned int scan_start;
    struct callback_head callback_head;
    u32 owner_nlportid;
    struct ieee80211_channel * channels[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct cfg80211_sched_scan_request {
    struct cfg80211_ssid *ssids;
    int n_ssids;
    u32 n_channels;
    enum nl80211_bss_scan_width scan_width;
    const u8 *ie;
    size_t ie_len;
    u32 flags;
    struct cfg80211_match_set *match_sets;
    int n_match_sets;
    s32 min_rssi_thold;
    u32 delay;
    struct cfg80211_sched_scan_plan *scan_plans;
    int n_scan_plans;
    u8 mac_addr[6];
    u8 mac_addr_mask[6];
    struct wiphy *wiphy;
    struct net_device *dev;
    long unsigned int scan_start;
    struct callback_head callback_head;
    u32 owner_nlportid;
    struct ieee80211_channel * channels[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct cfg80211_sched_scan_request {
    u64 reqid;
    struct cfg80211_ssid *ssids;
    int n_ssids;
    u32 n_channels;
    enum nl80211_bss_scan_width scan_width;
    const u8 *ie;
    size_t ie_len;
    u32 flags;
    struct cfg80211_match_set *match_sets;
    int n_match_sets;
    s32 min_rssi_thold;
    u32 delay;
    struct cfg80211_sched_scan_plan *scan_plans;
    int n_scan_plans;
    u8 mac_addr[6];
    u8 mac_addr_mask[6];
    bool relative_rssi_set;
    s8 relative_rssi;
    struct cfg80211_bss_select_adjust rssi_adjust;
    struct wiphy *wiphy;
    struct net_device *dev;
    long unsigned int scan_start;
    bool report_results;
    struct callback_head callback_head;
    u32 owner_nlportid;
    bool nl_owner_dead;
    struct list_head list;
    struct ieee80211_channel * channels[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct cfg80211_sched_scan_request {
    u64 reqid;
    struct cfg80211_ssid *ssids;
    int n_ssids;
    u32 n_channels;
    enum nl80211_bss_scan_width scan_width;
    const u8 *ie;
    size_t ie_len;
    u32 flags;
    struct cfg80211_match_set *match_sets;
    int n_match_sets;
    s32 min_rssi_thold;
    u32 delay;
    struct cfg80211_sched_scan_plan *scan_plans;
    int n_scan_plans;
    u8 mac_addr[6];
    u8 mac_addr_mask[6];
    bool relative_rssi_set;
    s8 relative_rssi;
    struct cfg80211_bss_select_adjust rssi_adjust;
    struct wiphy *wiphy;
    struct net_device *dev;
    long unsigned int scan_start;
    bool report_results;
    struct callback_head callback_head;
    u32 owner_nlportid;
    bool nl_owner_dead;
    struct list_head list;
    struct ieee80211_channel * channels[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct cfg80211_sched_scan_request {
    u64 reqid;
    struct cfg80211_ssid *ssids;
    int n_ssids;
    u32 n_channels;
    enum nl80211_bss_scan_width scan_width;
    const u8 *ie;
    size_t ie_len;
    u32 flags;
    struct cfg80211_match_set *match_sets;
    int n_match_sets;
    s32 min_rssi_thold;
    u32 delay;
    struct cfg80211_sched_scan_plan *scan_plans;
    int n_scan_plans;
    u8 mac_addr[6];
    u8 mac_addr_mask[6];
    bool relative_rssi_set;
    s8 relative_rssi;
    struct cfg80211_bss_select_adjust rssi_adjust;
    struct wiphy *wiphy;
    struct net_device *dev;
    long unsigned int scan_start;
    bool report_results;
    struct callback_head callback_head;
    u32 owner_nlportid;
    bool nl_owner_dead;
    struct list_head list;
    struct ieee80211_channel * channels[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct cfg80211_sched_scan_request {
    u64 reqid;
    struct cfg80211_ssid *ssids;
    int n_ssids;
    u32 n_channels;
    enum nl80211_bss_scan_width scan_width;
    const u8 *ie;
    size_t ie_len;
    u32 flags;
    struct cfg80211_match_set *match_sets;
    int n_match_sets;
    s32 min_rssi_thold;
    u32 delay;
    struct cfg80211_sched_scan_plan *scan_plans;
    int n_scan_plans;
    u8 mac_addr[6];
    u8 mac_addr_mask[6];
    bool relative_rssi_set;
    s8 relative_rssi;
    struct cfg80211_bss_select_adjust rssi_adjust;
    struct wiphy *wiphy;
    struct net_device *dev;
    long unsigned int scan_start;
    bool report_results;
    struct callback_head callback_head;
    u32 owner_nlportid;
    bool nl_owner_dead;
    struct list_head list;
    struct ieee80211_channel * channels[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct cfg80211_sched_scan_request {
    u64 reqid;
    struct cfg80211_ssid *ssids;
    int n_ssids;
    u32 n_channels;
    enum nl80211_bss_scan_width scan_width;
    const u8 *ie;
    size_t ie_len;
    u32 flags;
    struct cfg80211_match_set *match_sets;
    int n_match_sets;
    s32 min_rssi_thold;
    u32 delay;
    struct cfg80211_sched_scan_plan *scan_plans;
    int n_scan_plans;
    u8 mac_addr[6];
    u8 mac_addr_mask[6];
    bool relative_rssi_set;
    s8 relative_rssi;
    struct cfg80211_bss_select_adjust rssi_adjust;
    struct wiphy *wiphy;
    struct net_device *dev;
    long unsigned int scan_start;
    bool report_results;
    struct callback_head callback_head;
    u32 owner_nlportid;
    bool nl_owner_dead;
    struct list_head list;
    struct ieee80211_channel * channels[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct cfg80211_sched_scan_request {
    u64 reqid;
    struct cfg80211_ssid *ssids;
    int n_ssids;
    u32 n_channels;
    enum nl80211_bss_scan_width scan_width;
    const u8 *ie;
    size_t ie_len;
    u32 flags;
    struct cfg80211_match_set *match_sets;
    int n_match_sets;
    s32 min_rssi_thold;
    u32 delay;
    struct cfg80211_sched_scan_plan *scan_plans;
    int n_scan_plans;
    u8 mac_addr[6];
    u8 mac_addr_mask[6];
    bool relative_rssi_set;
    s8 relative_rssi;
    struct cfg80211_bss_select_adjust rssi_adjust;
    struct wiphy *wiphy;
    struct net_device *dev;
    long unsigned int scan_start;
    bool report_results;
    struct callback_head callback_head;
    u32 owner_nlportid;
    bool nl_owner_dead;
    struct list_head list;
    struct ieee80211_channel * channels[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct cfg80211_sched_scan_request {
    u64 reqid;
    struct cfg80211_ssid *ssids;
    int n_ssids;
    u32 n_channels;
    enum nl80211_bss_scan_width scan_width;
    const u8 *ie;
    size_t ie_len;
    u32 flags;
    struct cfg80211_match_set *match_sets;
    int n_match_sets;
    s32 min_rssi_thold;
    u32 delay;
    struct cfg80211_sched_scan_plan *scan_plans;
    int n_scan_plans;
    u8 mac_addr[6];
    u8 mac_addr_mask[6];
    bool relative_rssi_set;
    s8 relative_rssi;
    struct cfg80211_bss_select_adjust rssi_adjust;
    struct wiphy *wiphy;
    struct net_device *dev;
    long unsigned int scan_start;
    bool report_results;
    struct callback_head callback_head;
    u32 owner_nlportid;
    bool nl_owner_dead;
    struct list_head list;
    struct ieee80211_channel * channels[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct cfg80211_sched_scan_request {
    u64 reqid;
    struct cfg80211_ssid *ssids;
    int n_ssids;
    u32 n_channels;
    enum nl80211_bss_scan_width scan_width;
    const u8 *ie;
    size_t ie_len;
    u32 flags;
    struct cfg80211_match_set *match_sets;
    int n_match_sets;
    s32 min_rssi_thold;
    u32 delay;
    struct cfg80211_sched_scan_plan *scan_plans;
    int n_scan_plans;
    u8 mac_addr[6];
    u8 mac_addr_mask[6];
    bool relative_rssi_set;
    s8 relative_rssi;
    struct cfg80211_bss_select_adjust rssi_adjust;
    struct wiphy *wiphy;
    struct net_device *dev;
    long unsigned int scan_start;
    bool report_results;
    struct callback_head callback_head;
    u32 owner_nlportid;
    bool nl_owner_dead;
    struct list_head list;
    struct ieee80211_channel * channels[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct cfg80211_sched_scan_request {
    u64 reqid;
    struct cfg80211_ssid *ssids;
    int n_ssids;
    u32 n_channels;
    enum nl80211_bss_scan_width scan_width;
    const u8 *ie;
    size_t ie_len;
    u32 flags;
    struct cfg80211_match_set *match_sets;
    int n_match_sets;
    s32 min_rssi_thold;
    u32 delay;
    struct cfg80211_sched_scan_plan *scan_plans;
    int n_scan_plans;
    u8 mac_addr[6];
    u8 mac_addr_mask[6];
    bool relative_rssi_set;
    s8 relative_rssi;
    struct cfg80211_bss_select_adjust rssi_adjust;
    struct wiphy *wiphy;
    struct net_device *dev;
    long unsigned int scan_start;
    bool report_results;
    struct callback_head callback_head;
    u32 owner_nlportid;
    bool nl_owner_dead;
    struct list_head list;
    struct ieee80211_channel * channels[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct cfg80211_sched_scan_request {
    u64 reqid;
    struct cfg80211_ssid *ssids;
    int n_ssids;
    u32 n_channels;
    enum nl80211_bss_scan_width scan_width;
    const u8 *ie;
    size_t ie_len;
    u32 flags;
    struct cfg80211_match_set *match_sets;
    int n_match_sets;
    s32 min_rssi_thold;
    u32 delay;
    struct cfg80211_sched_scan_plan *scan_plans;
    int n_scan_plans;
    u8 mac_addr[6];
    u8 mac_addr_mask[6];
    bool relative_rssi_set;
    s8 relative_rssi;
    struct cfg80211_bss_select_adjust rssi_adjust;
    struct wiphy *wiphy;
    struct net_device *dev;
    long unsigned int scan_start;
    bool report_results;
    struct callback_head callback_head;
    u32 owner_nlportid;
    bool nl_owner_dead;
    struct list_head list;
    struct ieee80211_channel * channels[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct cfg80211_sched_scan_request {
    u64 reqid;
    struct cfg80211_ssid *ssids;
    int n_ssids;
    u32 n_channels;
    enum nl80211_bss_scan_width scan_width;
    const u8 *ie;
    size_t ie_len;
    u32 flags;
    struct cfg80211_match_set *match_sets;
    int n_match_sets;
    s32 min_rssi_thold;
    u32 delay;
    struct cfg80211_sched_scan_plan *scan_plans;
    int n_scan_plans;
    u8 mac_addr[6];
    u8 mac_addr_mask[6];
    bool relative_rssi_set;
    s8 relative_rssi;
    struct cfg80211_bss_select_adjust rssi_adjust;
    struct wiphy *wiphy;
    struct net_device *dev;
    long unsigned int scan_start;
    bool report_results;
    struct callback_head callback_head;
    u32 owner_nlportid;
    bool nl_owner_dead;
    struct list_head list;
    struct ieee80211_channel * channels[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct cfg80211_sched_scan_request {
    u64 reqid;
    struct cfg80211_ssid *ssids;
    int n_ssids;
    u32 n_channels;
    enum nl80211_bss_scan_width scan_width;
    const u8 *ie;
    size_t ie_len;
    u32 flags;
    struct cfg80211_match_set *match_sets;
    int n_match_sets;
    s32 min_rssi_thold;
    u32 delay;
    struct cfg80211_sched_scan_plan *scan_plans;
    int n_scan_plans;
    u8 mac_addr[6];
    u8 mac_addr_mask[6];
    bool relative_rssi_set;
    s8 relative_rssi;
    struct cfg80211_bss_select_adjust rssi_adjust;
    struct wiphy *wiphy;
    struct net_device *dev;
    long unsigned int scan_start;
    bool report_results;
    struct callback_head callback_head;
    u32 owner_nlportid;
    bool nl_owner_dead;
    struct list_head list;
    struct ieee80211_channel * channels[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct cfg80211_sched_scan_request {
    u64 reqid;
    struct cfg80211_ssid *ssids;
    int n_ssids;
    u32 n_channels;
    enum nl80211_bss_scan_width scan_width;
    const u8 *ie;
    size_t ie_len;
    u32 flags;
    struct cfg80211_match_set *match_sets;
    int n_match_sets;
    s32 min_rssi_thold;
    u32 delay;
    struct cfg80211_sched_scan_plan *scan_plans;
    int n_scan_plans;
    u8 mac_addr[6];
    u8 mac_addr_mask[6];
    bool relative_rssi_set;
    s8 relative_rssi;
    struct cfg80211_bss_select_adjust rssi_adjust;
    struct wiphy *wiphy;
    struct net_device *dev;
    long unsigned int scan_start;
    bool report_results;
    struct callback_head callback_head;
    u32 owner_nlportid;
    bool nl_owner_dead;
    struct list_head list;
    struct ieee80211_channel * channels[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct cfg80211_sched_scan_request {
    u64 reqid;
    struct cfg80211_ssid *ssids;
    int n_ssids;
    u32 n_channels;
    const u8 *ie;
    size_t ie_len;
    u32 flags;
    struct cfg80211_match_set *match_sets;
    int n_match_sets;
    s32 min_rssi_thold;
    u32 delay;
    struct cfg80211_sched_scan_plan *scan_plans;
    int n_scan_plans;
    u8 mac_addr[6];
    u8 mac_addr_mask[6];
    bool relative_rssi_set;
    s8 relative_rssi;
    struct cfg80211_bss_select_adjust rssi_adjust;
    struct wiphy *wiphy;
    struct net_device *dev;
    long unsigned int scan_start;
    bool report_results;
    struct callback_head callback_head;
    u32 owner_nlportid;
    bool nl_owner_dead;
    struct list_head list;
    struct ieee80211_channel * channels[0];
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
struct cfg80211_sched_scan_request {
    u64 reqid;
    struct cfg80211_ssid *ssids;
    int n_ssids;
    u32 n_channels;
    enum nl80211_bss_scan_width scan_width;
    const u8 *ie;
    size_t ie_len;
    u32 flags;
    struct cfg80211_match_set *match_sets;
    int n_match_sets;
    s32 min_rssi_thold;
    u32 delay;
    struct cfg80211_sched_scan_plan *scan_plans;
    int n_scan_plans;
    u8 mac_addr[6];
    u8 mac_addr_mask[6];
    bool relative_rssi_set;
    s8 relative_rssi;
    struct cfg80211_bss_select_adjust rssi_adjust;
    struct wiphy *wiphy;
    struct net_device *dev;
    long unsigned int scan_start;
    bool report_results;
    struct callback_head callback_head;
    u32 owner_nlportid;
    bool nl_owner_dead;
    struct list_head list;
    struct ieee80211_channel * channels[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct cfg80211_sched_scan_request {
    u64 reqid;
    struct cfg80211_ssid *ssids;
    int n_ssids;
    u32 n_channels;
    enum nl80211_bss_scan_width scan_width;
    const u8 *ie;
    size_t ie_len;
    u32 flags;
    struct cfg80211_match_set *match_sets;
    int n_match_sets;
    s32 min_rssi_thold;
    u32 delay;
    struct cfg80211_sched_scan_plan *scan_plans;
    int n_scan_plans;
    u8 mac_addr[6];
    u8 mac_addr_mask[6];
    bool relative_rssi_set;
    s8 relative_rssi;
    struct cfg80211_bss_select_adjust rssi_adjust;
    struct wiphy *wiphy;
    struct net_device *dev;
    long unsigned int scan_start;
    bool report_results;
    struct callback_head callback_head;
    u32 owner_nlportid;
    bool nl_owner_dead;
    struct list_head list;
    struct ieee80211_channel * channels[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct cfg80211_sched_scan_request {
    u64 reqid;
    struct cfg80211_ssid *ssids;
    int n_ssids;
    u32 n_channels;
    enum nl80211_bss_scan_width scan_width;
    const u8 *ie;
    size_t ie_len;
    u32 flags;
    struct cfg80211_match_set *match_sets;
    int n_match_sets;
    s32 min_rssi_thold;
    u32 delay;
    struct cfg80211_sched_scan_plan *scan_plans;
    int n_scan_plans;
    u8 mac_addr[6];
    u8 mac_addr_mask[6];
    bool relative_rssi_set;
    s8 relative_rssi;
    struct cfg80211_bss_select_adjust rssi_adjust;
    struct wiphy *wiphy;
    struct net_device *dev;
    long unsigned int scan_start;
    bool report_results;
    struct callback_head callback_head;
    u32 owner_nlportid;
    bool nl_owner_dead;
    struct list_head list;
    struct ieee80211_channel * channels[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct cfg80211_sched_scan_request {
    u64 reqid;
    struct cfg80211_ssid *ssids;
    int n_ssids;
    u32 n_channels;
    enum nl80211_bss_scan_width scan_width;
    const u8 *ie;
    size_t ie_len;
    u32 flags;
    struct cfg80211_match_set *match_sets;
    int n_match_sets;
    s32 min_rssi_thold;
    u32 delay;
    struct cfg80211_sched_scan_plan *scan_plans;
    int n_scan_plans;
    u8 mac_addr[6];
    u8 mac_addr_mask[6];
    bool relative_rssi_set;
    s8 relative_rssi;
    struct cfg80211_bss_select_adjust rssi_adjust;
    struct wiphy *wiphy;
    struct net_device *dev;
    long unsigned int scan_start;
    bool report_results;
    struct callback_head callback_head;
    u32 owner_nlportid;
    bool nl_owner_dead;
    struct list_head list;
    struct ieee80211_channel * channels[0];
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
struct cfg80211_sched_scan_request {
    u64 reqid;
    struct cfg80211_ssid *ssids;
    int n_ssids;
    u32 n_channels;
    enum nl80211_bss_scan_width scan_width;
    const u8 *ie;
    size_t ie_len;
    u32 flags;
    struct cfg80211_match_set *match_sets;
    int n_match_sets;
    s32 min_rssi_thold;
    u32 delay;
    struct cfg80211_sched_scan_plan *scan_plans;
    int n_scan_plans;
    u8 mac_addr[6];
    u8 mac_addr_mask[6];
    bool relative_rssi_set;
    s8 relative_rssi;
    struct cfg80211_bss_select_adjust rssi_adjust;
    struct wiphy *wiphy;
    struct net_device *dev;
    long unsigned int scan_start;
    bool report_results;
    struct callback_head callback_head;
    u32 owner_nlportid;
    bool nl_owner_dead;
    struct list_head list;
    struct ieee80211_channel * channels[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct cfg80211_sched_scan_request {
    u64 reqid;
    struct cfg80211_ssid *ssids;
    int n_ssids;
    u32 n_channels;
    enum nl80211_bss_scan_width scan_width;
    const u8 *ie;
    size_t ie_len;
    u32 flags;
    struct cfg80211_match_set *match_sets;
    int n_match_sets;
    s32 min_rssi_thold;
    u32 delay;
    struct cfg80211_sched_scan_plan *scan_plans;
    int n_scan_plans;
    u8 mac_addr[6];
    u8 mac_addr_mask[6];
    bool relative_rssi_set;
    s8 relative_rssi;
    struct cfg80211_bss_select_adjust rssi_adjust;
    struct wiphy *wiphy;
    struct net_device *dev;
    long unsigned int scan_start;
    bool report_results;
    struct callback_head callback_head;
    u32 owner_nlportid;
    bool nl_owner_dead;
    struct list_head list;
    struct ieee80211_channel * channels[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct cfg80211_sched_scan_request {
    u64 reqid;
    struct cfg80211_ssid *ssids;
    int n_ssids;
    u32 n_channels;
    enum nl80211_bss_scan_width scan_width;
    const u8 *ie;
    size_t ie_len;
    u32 flags;
    struct cfg80211_match_set *match_sets;
    int n_match_sets;
    s32 min_rssi_thold;
    u32 delay;
    struct cfg80211_sched_scan_plan *scan_plans;
    int n_scan_plans;
    u8 mac_addr[6];
    u8 mac_addr_mask[6];
    bool relative_rssi_set;
    s8 relative_rssi;
    struct cfg80211_bss_select_adjust rssi_adjust;
    struct wiphy *wiphy;
    struct net_device *dev;
    long unsigned int scan_start;
    bool report_results;
    struct callback_head callback_head;
    u32 owner_nlportid;
    bool nl_owner_dead;
    struct list_head list;
    struct ieee80211_channel * channels[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cfg80211_sched_scan_request {
    u64 reqid;
    struct cfg80211_ssid *ssids;
    int n_ssids;
    u32 n_channels;
    enum nl80211_bss_scan_width scan_width;
    const u8 *ie;
    size_t ie_len;
    u32 flags;
    struct cfg80211_match_set *match_sets;
    int n_match_sets;
    s32 min_rssi_thold;
    u32 delay;
    struct cfg80211_sched_scan_plan *scan_plans;
    int n_scan_plans;
    u8 mac_addr[6];
    u8 mac_addr_mask[6];
    bool relative_rssi_set;
    s8 relative_rssi;
    struct cfg80211_bss_select_adjust rssi_adjust;
    struct wiphy *wiphy;
    struct net_device *dev;
    long unsigned int scan_start;
    bool report_results;
    struct callback_head callback_head;
    u32 owner_nlportid;
    bool nl_owner_dead;
    struct list_head list;
    struct ieee80211_channel * channels[0];
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
<code>u64 reqid</code>
</li>
<li>
<b>Field added. </b>
<code>bool relative_rssi_set</code>
</li>
<li>
<b>Field added. </b>
<code>s8 relative_rssi</code>
</li>
<li>
<b>Field added. </b>
<code>struct cfg80211_bss_select_adjust rssi_adjust</code>
</li>
<li>
<b>Field added. </b>
<code>bool report_results</code>
</li>
<li>
<b>Field added. </b>
<code>bool nl_owner_dead</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head list</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>enum nl80211_bss_scan_width scan_width</code>
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
