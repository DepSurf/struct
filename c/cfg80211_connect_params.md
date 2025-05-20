# Struct: <code>cfg80211_connect_params</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct cfg80211_connect_params {
    struct ieee80211_channel *channel;
    struct ieee80211_channel *channel_hint;
    const u8 *bssid;
    const u8 *bssid_hint;
    const u8 *ssid;
    size_t ssid_len;
    enum nl80211_auth_type auth_type;
    const u8 *ie;
    size_t ie_len;
    bool privacy;
    enum nl80211_mfp mfp;
    struct cfg80211_crypto_settings crypto;
    const u8 *key;
    u8 key_len;
    u8 key_idx;
    u32 flags;
    int bg_scan_period;
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct ieee80211_vht_cap vht_capa;
    struct ieee80211_vht_cap vht_capa_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct cfg80211_connect_params {
    struct ieee80211_channel *channel;
    struct ieee80211_channel *channel_hint;
    const u8 *bssid;
    const u8 *bssid_hint;
    const u8 *ssid;
    size_t ssid_len;
    enum nl80211_auth_type auth_type;
    const u8 *ie;
    size_t ie_len;
    bool privacy;
    enum nl80211_mfp mfp;
    struct cfg80211_crypto_settings crypto;
    const u8 *key;
    u8 key_len;
    u8 key_idx;
    u32 flags;
    int bg_scan_period;
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct ieee80211_vht_cap vht_capa;
    struct ieee80211_vht_cap vht_capa_mask;
    bool pbss;
    struct cfg80211_bss_selection bss_select;
    const u8 *prev_bssid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct cfg80211_connect_params {
    struct ieee80211_channel *channel;
    struct ieee80211_channel *channel_hint;
    const u8 *bssid;
    const u8 *bssid_hint;
    const u8 *ssid;
    size_t ssid_len;
    enum nl80211_auth_type auth_type;
    const u8 *ie;
    size_t ie_len;
    bool privacy;
    enum nl80211_mfp mfp;
    struct cfg80211_crypto_settings crypto;
    const u8 *key;
    u8 key_len;
    u8 key_idx;
    u32 flags;
    int bg_scan_period;
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct ieee80211_vht_cap vht_capa;
    struct ieee80211_vht_cap vht_capa_mask;
    bool pbss;
    struct cfg80211_bss_selection bss_select;
    const u8 *prev_bssid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct cfg80211_connect_params {
    struct ieee80211_channel *channel;
    struct ieee80211_channel *channel_hint;
    const u8 *bssid;
    const u8 *bssid_hint;
    const u8 *ssid;
    size_t ssid_len;
    enum nl80211_auth_type auth_type;
    const u8 *ie;
    size_t ie_len;
    bool privacy;
    enum nl80211_mfp mfp;
    struct cfg80211_crypto_settings crypto;
    const u8 *key;
    u8 key_len;
    u8 key_idx;
    u32 flags;
    int bg_scan_period;
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct ieee80211_vht_cap vht_capa;
    struct ieee80211_vht_cap vht_capa_mask;
    bool pbss;
    struct cfg80211_bss_selection bss_select;
    const u8 *prev_bssid;
    const u8 *fils_erp_username;
    size_t fils_erp_username_len;
    const u8 *fils_erp_realm;
    size_t fils_erp_realm_len;
    u16 fils_erp_next_seq_num;
    const u8 *fils_erp_rrk;
    size_t fils_erp_rrk_len;
    bool want_1x;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct cfg80211_connect_params {
    struct ieee80211_channel *channel;
    struct ieee80211_channel *channel_hint;
    const u8 *bssid;
    const u8 *bssid_hint;
    const u8 *ssid;
    size_t ssid_len;
    enum nl80211_auth_type auth_type;
    const u8 *ie;
    size_t ie_len;
    bool privacy;
    enum nl80211_mfp mfp;
    struct cfg80211_crypto_settings crypto;
    const u8 *key;
    u8 key_len;
    u8 key_idx;
    u32 flags;
    int bg_scan_period;
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct ieee80211_vht_cap vht_capa;
    struct ieee80211_vht_cap vht_capa_mask;
    bool pbss;
    struct cfg80211_bss_selection bss_select;
    const u8 *prev_bssid;
    const u8 *fils_erp_username;
    size_t fils_erp_username_len;
    const u8 *fils_erp_realm;
    size_t fils_erp_realm_len;
    u16 fils_erp_next_seq_num;
    const u8 *fils_erp_rrk;
    size_t fils_erp_rrk_len;
    bool want_1x;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct cfg80211_connect_params {
    struct ieee80211_channel *channel;
    struct ieee80211_channel *channel_hint;
    const u8 *bssid;
    const u8 *bssid_hint;
    const u8 *ssid;
    size_t ssid_len;
    enum nl80211_auth_type auth_type;
    const u8 *ie;
    size_t ie_len;
    bool privacy;
    enum nl80211_mfp mfp;
    struct cfg80211_crypto_settings crypto;
    const u8 *key;
    u8 key_len;
    u8 key_idx;
    u32 flags;
    int bg_scan_period;
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct ieee80211_vht_cap vht_capa;
    struct ieee80211_vht_cap vht_capa_mask;
    bool pbss;
    struct cfg80211_bss_selection bss_select;
    const u8 *prev_bssid;
    const u8 *fils_erp_username;
    size_t fils_erp_username_len;
    const u8 *fils_erp_realm;
    size_t fils_erp_realm_len;
    u16 fils_erp_next_seq_num;
    const u8 *fils_erp_rrk;
    size_t fils_erp_rrk_len;
    bool want_1x;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct cfg80211_connect_params {
    struct ieee80211_channel *channel;
    struct ieee80211_channel *channel_hint;
    const u8 *bssid;
    const u8 *bssid_hint;
    const u8 *ssid;
    size_t ssid_len;
    enum nl80211_auth_type auth_type;
    const u8 *ie;
    size_t ie_len;
    bool privacy;
    enum nl80211_mfp mfp;
    struct cfg80211_crypto_settings crypto;
    const u8 *key;
    u8 key_len;
    u8 key_idx;
    u32 flags;
    int bg_scan_period;
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct ieee80211_vht_cap vht_capa;
    struct ieee80211_vht_cap vht_capa_mask;
    bool pbss;
    struct cfg80211_bss_selection bss_select;
    const u8 *prev_bssid;
    const u8 *fils_erp_username;
    size_t fils_erp_username_len;
    const u8 *fils_erp_realm;
    size_t fils_erp_realm_len;
    u16 fils_erp_next_seq_num;
    const u8 *fils_erp_rrk;
    size_t fils_erp_rrk_len;
    bool want_1x;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct cfg80211_connect_params {
    struct ieee80211_channel *channel;
    struct ieee80211_channel *channel_hint;
    const u8 *bssid;
    const u8 *bssid_hint;
    const u8 *ssid;
    size_t ssid_len;
    enum nl80211_auth_type auth_type;
    const u8 *ie;
    size_t ie_len;
    bool privacy;
    enum nl80211_mfp mfp;
    struct cfg80211_crypto_settings crypto;
    const u8 *key;
    u8 key_len;
    u8 key_idx;
    u32 flags;
    int bg_scan_period;
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct ieee80211_vht_cap vht_capa;
    struct ieee80211_vht_cap vht_capa_mask;
    bool pbss;
    struct cfg80211_bss_selection bss_select;
    const u8 *prev_bssid;
    const u8 *fils_erp_username;
    size_t fils_erp_username_len;
    const u8 *fils_erp_realm;
    size_t fils_erp_realm_len;
    u16 fils_erp_next_seq_num;
    const u8 *fils_erp_rrk;
    size_t fils_erp_rrk_len;
    bool want_1x;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct cfg80211_connect_params {
    struct ieee80211_channel *channel;
    struct ieee80211_channel *channel_hint;
    const u8 *bssid;
    const u8 *bssid_hint;
    const u8 *ssid;
    size_t ssid_len;
    enum nl80211_auth_type auth_type;
    const u8 *ie;
    size_t ie_len;
    bool privacy;
    enum nl80211_mfp mfp;
    struct cfg80211_crypto_settings crypto;
    const u8 *key;
    u8 key_len;
    u8 key_idx;
    u32 flags;
    int bg_scan_period;
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct ieee80211_vht_cap vht_capa;
    struct ieee80211_vht_cap vht_capa_mask;
    bool pbss;
    struct cfg80211_bss_selection bss_select;
    const u8 *prev_bssid;
    const u8 *fils_erp_username;
    size_t fils_erp_username_len;
    const u8 *fils_erp_realm;
    size_t fils_erp_realm_len;
    u16 fils_erp_next_seq_num;
    const u8 *fils_erp_rrk;
    size_t fils_erp_rrk_len;
    bool want_1x;
    struct ieee80211_edmg edmg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct cfg80211_connect_params {
    struct ieee80211_channel *channel;
    struct ieee80211_channel *channel_hint;
    const u8 *bssid;
    const u8 *bssid_hint;
    const u8 *ssid;
    size_t ssid_len;
    enum nl80211_auth_type auth_type;
    const u8 *ie;
    size_t ie_len;
    bool privacy;
    enum nl80211_mfp mfp;
    struct cfg80211_crypto_settings crypto;
    const u8 *key;
    u8 key_len;
    u8 key_idx;
    u32 flags;
    int bg_scan_period;
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct ieee80211_vht_cap vht_capa;
    struct ieee80211_vht_cap vht_capa_mask;
    bool pbss;
    struct cfg80211_bss_selection bss_select;
    const u8 *prev_bssid;
    const u8 *fils_erp_username;
    size_t fils_erp_username_len;
    const u8 *fils_erp_realm;
    size_t fils_erp_realm_len;
    u16 fils_erp_next_seq_num;
    const u8 *fils_erp_rrk;
    size_t fils_erp_rrk_len;
    bool want_1x;
    struct ieee80211_edmg edmg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct cfg80211_connect_params {
    struct ieee80211_channel *channel;
    struct ieee80211_channel *channel_hint;
    const u8 *bssid;
    const u8 *bssid_hint;
    const u8 *ssid;
    size_t ssid_len;
    enum nl80211_auth_type auth_type;
    const u8 *ie;
    size_t ie_len;
    bool privacy;
    enum nl80211_mfp mfp;
    struct cfg80211_crypto_settings crypto;
    const u8 *key;
    u8 key_len;
    u8 key_idx;
    u32 flags;
    int bg_scan_period;
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct ieee80211_vht_cap vht_capa;
    struct ieee80211_vht_cap vht_capa_mask;
    bool pbss;
    struct cfg80211_bss_selection bss_select;
    const u8 *prev_bssid;
    const u8 *fils_erp_username;
    size_t fils_erp_username_len;
    const u8 *fils_erp_realm;
    size_t fils_erp_realm_len;
    u16 fils_erp_next_seq_num;
    const u8 *fils_erp_rrk;
    size_t fils_erp_rrk_len;
    bool want_1x;
    struct ieee80211_edmg edmg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct cfg80211_connect_params {
    struct ieee80211_channel *channel;
    struct ieee80211_channel *channel_hint;
    const u8 *bssid;
    const u8 *bssid_hint;
    const u8 *ssid;
    size_t ssid_len;
    enum nl80211_auth_type auth_type;
    const u8 *ie;
    size_t ie_len;
    bool privacy;
    enum nl80211_mfp mfp;
    struct cfg80211_crypto_settings crypto;
    const u8 *key;
    u8 key_len;
    u8 key_idx;
    u32 flags;
    int bg_scan_period;
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct ieee80211_vht_cap vht_capa;
    struct ieee80211_vht_cap vht_capa_mask;
    bool pbss;
    struct cfg80211_bss_selection bss_select;
    const u8 *prev_bssid;
    const u8 *fils_erp_username;
    size_t fils_erp_username_len;
    const u8 *fils_erp_realm;
    size_t fils_erp_realm_len;
    u16 fils_erp_next_seq_num;
    const u8 *fils_erp_rrk;
    size_t fils_erp_rrk_len;
    bool want_1x;
    struct ieee80211_edmg edmg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct cfg80211_connect_params {
    struct ieee80211_channel *channel;
    struct ieee80211_channel *channel_hint;
    const u8 *bssid;
    const u8 *bssid_hint;
    const u8 *ssid;
    size_t ssid_len;
    enum nl80211_auth_type auth_type;
    const u8 *ie;
    size_t ie_len;
    bool privacy;
    enum nl80211_mfp mfp;
    struct cfg80211_crypto_settings crypto;
    const u8 *key;
    u8 key_len;
    u8 key_idx;
    u32 flags;
    int bg_scan_period;
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct ieee80211_vht_cap vht_capa;
    struct ieee80211_vht_cap vht_capa_mask;
    bool pbss;
    struct cfg80211_bss_selection bss_select;
    const u8 *prev_bssid;
    const u8 *fils_erp_username;
    size_t fils_erp_username_len;
    const u8 *fils_erp_realm;
    size_t fils_erp_realm_len;
    u16 fils_erp_next_seq_num;
    const u8 *fils_erp_rrk;
    size_t fils_erp_rrk_len;
    bool want_1x;
    struct ieee80211_edmg edmg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct cfg80211_connect_params {
    struct ieee80211_channel *channel;
    struct ieee80211_channel *channel_hint;
    const u8 *bssid;
    const u8 *bssid_hint;
    const u8 *ssid;
    size_t ssid_len;
    enum nl80211_auth_type auth_type;
    const u8 *ie;
    size_t ie_len;
    bool privacy;
    enum nl80211_mfp mfp;
    struct cfg80211_crypto_settings crypto;
    const u8 *key;
    u8 key_len;
    u8 key_idx;
    u32 flags;
    int bg_scan_period;
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct ieee80211_vht_cap vht_capa;
    struct ieee80211_vht_cap vht_capa_mask;
    bool pbss;
    struct cfg80211_bss_selection bss_select;
    const u8 *prev_bssid;
    const u8 *fils_erp_username;
    size_t fils_erp_username_len;
    const u8 *fils_erp_realm;
    size_t fils_erp_realm_len;
    u16 fils_erp_next_seq_num;
    const u8 *fils_erp_rrk;
    size_t fils_erp_rrk_len;
    bool want_1x;
    struct ieee80211_edmg edmg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct cfg80211_connect_params {
    struct ieee80211_channel *channel;
    struct ieee80211_channel *channel_hint;
    const u8 *bssid;
    const u8 *bssid_hint;
    const u8 *ssid;
    size_t ssid_len;
    enum nl80211_auth_type auth_type;
    const u8 *ie;
    size_t ie_len;
    bool privacy;
    enum nl80211_mfp mfp;
    struct cfg80211_crypto_settings crypto;
    const u8 *key;
    u8 key_len;
    u8 key_idx;
    u32 flags;
    int bg_scan_period;
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct ieee80211_vht_cap vht_capa;
    struct ieee80211_vht_cap vht_capa_mask;
    bool pbss;
    struct cfg80211_bss_selection bss_select;
    const u8 *prev_bssid;
    const u8 *fils_erp_username;
    size_t fils_erp_username_len;
    const u8 *fils_erp_realm;
    size_t fils_erp_realm_len;
    u16 fils_erp_next_seq_num;
    const u8 *fils_erp_rrk;
    size_t fils_erp_rrk_len;
    bool want_1x;
    struct ieee80211_edmg edmg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct cfg80211_connect_params {
    struct ieee80211_channel *channel;
    struct ieee80211_channel *channel_hint;
    const u8 *bssid;
    const u8 *bssid_hint;
    const u8 *ssid;
    size_t ssid_len;
    enum nl80211_auth_type auth_type;
    const u8 *ie;
    size_t ie_len;
    bool privacy;
    enum nl80211_mfp mfp;
    struct cfg80211_crypto_settings crypto;
    const u8 *key;
    u8 key_len;
    u8 key_idx;
    u32 flags;
    int bg_scan_period;
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct ieee80211_vht_cap vht_capa;
    struct ieee80211_vht_cap vht_capa_mask;
    bool pbss;
    struct cfg80211_bss_selection bss_select;
    const u8 *prev_bssid;
    const u8 *fils_erp_username;
    size_t fils_erp_username_len;
    const u8 *fils_erp_realm;
    size_t fils_erp_realm_len;
    u16 fils_erp_next_seq_num;
    const u8 *fils_erp_rrk;
    size_t fils_erp_rrk_len;
    bool want_1x;
    struct ieee80211_edmg edmg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct cfg80211_connect_params {
    struct ieee80211_channel *channel;
    struct ieee80211_channel *channel_hint;
    const u8 *bssid;
    const u8 *bssid_hint;
    const u8 *ssid;
    size_t ssid_len;
    enum nl80211_auth_type auth_type;
    const u8 *ie;
    size_t ie_len;
    bool privacy;
    enum nl80211_mfp mfp;
    struct cfg80211_crypto_settings crypto;
    const u8 *key;
    u8 key_len;
    u8 key_idx;
    u32 flags;
    int bg_scan_period;
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct ieee80211_vht_cap vht_capa;
    struct ieee80211_vht_cap vht_capa_mask;
    bool pbss;
    struct cfg80211_bss_selection bss_select;
    const u8 *prev_bssid;
    const u8 *fils_erp_username;
    size_t fils_erp_username_len;
    const u8 *fils_erp_realm;
    size_t fils_erp_realm_len;
    u16 fils_erp_next_seq_num;
    const u8 *fils_erp_rrk;
    size_t fils_erp_rrk_len;
    bool want_1x;
    struct ieee80211_edmg edmg;
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
struct cfg80211_connect_params {
    struct ieee80211_channel *channel;
    struct ieee80211_channel *channel_hint;
    const u8 *bssid;
    const u8 *bssid_hint;
    const u8 *ssid;
    size_t ssid_len;
    enum nl80211_auth_type auth_type;
    const u8 *ie;
    size_t ie_len;
    bool privacy;
    enum nl80211_mfp mfp;
    struct cfg80211_crypto_settings crypto;
    const u8 *key;
    u8 key_len;
    u8 key_idx;
    u32 flags;
    int bg_scan_period;
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct ieee80211_vht_cap vht_capa;
    struct ieee80211_vht_cap vht_capa_mask;
    bool pbss;
    struct cfg80211_bss_selection bss_select;
    const u8 *prev_bssid;
    const u8 *fils_erp_username;
    size_t fils_erp_username_len;
    const u8 *fils_erp_realm;
    size_t fils_erp_realm_len;
    u16 fils_erp_next_seq_num;
    const u8 *fils_erp_rrk;
    size_t fils_erp_rrk_len;
    bool want_1x;
    struct ieee80211_edmg edmg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct cfg80211_connect_params {
    struct ieee80211_channel *channel;
    struct ieee80211_channel *channel_hint;
    const u8 *bssid;
    const u8 *bssid_hint;
    const u8 *ssid;
    size_t ssid_len;
    enum nl80211_auth_type auth_type;
    const u8 *ie;
    size_t ie_len;
    bool privacy;
    enum nl80211_mfp mfp;
    struct cfg80211_crypto_settings crypto;
    const u8 *key;
    u8 key_len;
    u8 key_idx;
    u32 flags;
    int bg_scan_period;
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct ieee80211_vht_cap vht_capa;
    struct ieee80211_vht_cap vht_capa_mask;
    bool pbss;
    struct cfg80211_bss_selection bss_select;
    const u8 *prev_bssid;
    const u8 *fils_erp_username;
    size_t fils_erp_username_len;
    const u8 *fils_erp_realm;
    size_t fils_erp_realm_len;
    u16 fils_erp_next_seq_num;
    const u8 *fils_erp_rrk;
    size_t fils_erp_rrk_len;
    bool want_1x;
    struct ieee80211_edmg edmg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct cfg80211_connect_params {
    struct ieee80211_channel *channel;
    struct ieee80211_channel *channel_hint;
    const u8 *bssid;
    const u8 *bssid_hint;
    const u8 *ssid;
    size_t ssid_len;
    enum nl80211_auth_type auth_type;
    const u8 *ie;
    size_t ie_len;
    bool privacy;
    enum nl80211_mfp mfp;
    struct cfg80211_crypto_settings crypto;
    const u8 *key;
    u8 key_len;
    u8 key_idx;
    u32 flags;
    int bg_scan_period;
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct ieee80211_vht_cap vht_capa;
    struct ieee80211_vht_cap vht_capa_mask;
    bool pbss;
    struct cfg80211_bss_selection bss_select;
    const u8 *prev_bssid;
    const u8 *fils_erp_username;
    size_t fils_erp_username_len;
    const u8 *fils_erp_realm;
    size_t fils_erp_realm_len;
    u16 fils_erp_next_seq_num;
    const u8 *fils_erp_rrk;
    size_t fils_erp_rrk_len;
    bool want_1x;
    struct ieee80211_edmg edmg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct cfg80211_connect_params {
    struct ieee80211_channel *channel;
    struct ieee80211_channel *channel_hint;
    const u8 *bssid;
    const u8 *bssid_hint;
    const u8 *ssid;
    size_t ssid_len;
    enum nl80211_auth_type auth_type;
    const u8 *ie;
    size_t ie_len;
    bool privacy;
    enum nl80211_mfp mfp;
    struct cfg80211_crypto_settings crypto;
    const u8 *key;
    u8 key_len;
    u8 key_idx;
    u32 flags;
    int bg_scan_period;
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct ieee80211_vht_cap vht_capa;
    struct ieee80211_vht_cap vht_capa_mask;
    bool pbss;
    struct cfg80211_bss_selection bss_select;
    const u8 *prev_bssid;
    const u8 *fils_erp_username;
    size_t fils_erp_username_len;
    const u8 *fils_erp_realm;
    size_t fils_erp_realm_len;
    u16 fils_erp_next_seq_num;
    const u8 *fils_erp_rrk;
    size_t fils_erp_rrk_len;
    bool want_1x;
    struct ieee80211_edmg edmg;
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
struct cfg80211_connect_params {
    struct ieee80211_channel *channel;
    struct ieee80211_channel *channel_hint;
    const u8 *bssid;
    const u8 *bssid_hint;
    const u8 *ssid;
    size_t ssid_len;
    enum nl80211_auth_type auth_type;
    const u8 *ie;
    size_t ie_len;
    bool privacy;
    enum nl80211_mfp mfp;
    struct cfg80211_crypto_settings crypto;
    const u8 *key;
    u8 key_len;
    u8 key_idx;
    u32 flags;
    int bg_scan_period;
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct ieee80211_vht_cap vht_capa;
    struct ieee80211_vht_cap vht_capa_mask;
    bool pbss;
    struct cfg80211_bss_selection bss_select;
    const u8 *prev_bssid;
    const u8 *fils_erp_username;
    size_t fils_erp_username_len;
    const u8 *fils_erp_realm;
    size_t fils_erp_realm_len;
    u16 fils_erp_next_seq_num;
    const u8 *fils_erp_rrk;
    size_t fils_erp_rrk_len;
    bool want_1x;
    struct ieee80211_edmg edmg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct cfg80211_connect_params {
    struct ieee80211_channel *channel;
    struct ieee80211_channel *channel_hint;
    const u8 *bssid;
    const u8 *bssid_hint;
    const u8 *ssid;
    size_t ssid_len;
    enum nl80211_auth_type auth_type;
    const u8 *ie;
    size_t ie_len;
    bool privacy;
    enum nl80211_mfp mfp;
    struct cfg80211_crypto_settings crypto;
    const u8 *key;
    u8 key_len;
    u8 key_idx;
    u32 flags;
    int bg_scan_period;
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct ieee80211_vht_cap vht_capa;
    struct ieee80211_vht_cap vht_capa_mask;
    bool pbss;
    struct cfg80211_bss_selection bss_select;
    const u8 *prev_bssid;
    const u8 *fils_erp_username;
    size_t fils_erp_username_len;
    const u8 *fils_erp_realm;
    size_t fils_erp_realm_len;
    u16 fils_erp_next_seq_num;
    const u8 *fils_erp_rrk;
    size_t fils_erp_rrk_len;
    bool want_1x;
    struct ieee80211_edmg edmg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct cfg80211_connect_params {
    struct ieee80211_channel *channel;
    struct ieee80211_channel *channel_hint;
    const u8 *bssid;
    const u8 *bssid_hint;
    const u8 *ssid;
    size_t ssid_len;
    enum nl80211_auth_type auth_type;
    const u8 *ie;
    size_t ie_len;
    bool privacy;
    enum nl80211_mfp mfp;
    struct cfg80211_crypto_settings crypto;
    const u8 *key;
    u8 key_len;
    u8 key_idx;
    u32 flags;
    int bg_scan_period;
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct ieee80211_vht_cap vht_capa;
    struct ieee80211_vht_cap vht_capa_mask;
    bool pbss;
    struct cfg80211_bss_selection bss_select;
    const u8 *prev_bssid;
    const u8 *fils_erp_username;
    size_t fils_erp_username_len;
    const u8 *fils_erp_realm;
    size_t fils_erp_realm_len;
    u16 fils_erp_next_seq_num;
    const u8 *fils_erp_rrk;
    size_t fils_erp_rrk_len;
    bool want_1x;
    struct ieee80211_edmg edmg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cfg80211_connect_params {
    struct ieee80211_channel *channel;
    struct ieee80211_channel *channel_hint;
    const u8 *bssid;
    const u8 *bssid_hint;
    const u8 *ssid;
    size_t ssid_len;
    enum nl80211_auth_type auth_type;
    const u8 *ie;
    size_t ie_len;
    bool privacy;
    enum nl80211_mfp mfp;
    struct cfg80211_crypto_settings crypto;
    const u8 *key;
    u8 key_len;
    u8 key_idx;
    u32 flags;
    int bg_scan_period;
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct ieee80211_vht_cap vht_capa;
    struct ieee80211_vht_cap vht_capa_mask;
    bool pbss;
    struct cfg80211_bss_selection bss_select;
    const u8 *prev_bssid;
    const u8 *fils_erp_username;
    size_t fils_erp_username_len;
    const u8 *fils_erp_realm;
    size_t fils_erp_realm_len;
    u16 fils_erp_next_seq_num;
    const u8 *fils_erp_rrk;
    size_t fils_erp_rrk_len;
    bool want_1x;
    struct ieee80211_edmg edmg;
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
<code>bool pbss</code>
</li>
<li>
<b>Field added. </b>
<code>struct cfg80211_bss_selection bss_select</code>
</li>
<li>
<b>Field added. </b>
<code>const u8 *prev_bssid</code>
</li>
</ul>
</details>
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
<code>const u8 *fils_erp_username</code>
</li>
<li>
<b>Field added. </b>
<code>size_t fils_erp_username_len</code>
</li>
<li>
<b>Field added. </b>
<code>const u8 *fils_erp_realm</code>
</li>
<li>
<b>Field added. </b>
<code>size_t fils_erp_realm_len</code>
</li>
<li>
<b>Field added. </b>
<code>u16 fils_erp_next_seq_num</code>
</li>
<li>
<b>Field added. </b>
<code>const u8 *fils_erp_rrk</code>
</li>
<li>
<b>Field added. </b>
<code>size_t fils_erp_rrk_len</code>
</li>
<li>
<b>Field added. </b>
<code>bool want_1x</code>
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
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct ieee80211_edmg edmg</code>
</li>
</ul>
</details>
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
