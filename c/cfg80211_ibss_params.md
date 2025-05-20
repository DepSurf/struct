# Struct: <code>cfg80211_ibss_params</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct cfg80211_ibss_params {
    const u8 *ssid;
    const u8 *bssid;
    struct cfg80211_chan_def chandef;
    const u8 *ie;
    u8 ssid_len;
    u8 ie_len;
    u16 beacon_interval;
    u32 basic_rates;
    bool channel_fixed;
    bool privacy;
    bool control_port;
    bool userspace_handles_dfs;
    int mcast_rate[3];
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct cfg80211_ibss_params {
    const u8 *ssid;
    const u8 *bssid;
    struct cfg80211_chan_def chandef;
    const u8 *ie;
    u8 ssid_len;
    u8 ie_len;
    u16 beacon_interval;
    u32 basic_rates;
    bool channel_fixed;
    bool privacy;
    bool control_port;
    bool userspace_handles_dfs;
    int mcast_rate[3];
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct cfg80211_ibss_params {
    const u8 *ssid;
    const u8 *bssid;
    struct cfg80211_chan_def chandef;
    const u8 *ie;
    u8 ssid_len;
    u8 ie_len;
    u16 beacon_interval;
    u32 basic_rates;
    bool channel_fixed;
    bool privacy;
    bool control_port;
    bool userspace_handles_dfs;
    int mcast_rate[3];
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct cfg80211_ibss_params {
    const u8 *ssid;
    const u8 *bssid;
    struct cfg80211_chan_def chandef;
    const u8 *ie;
    u8 ssid_len;
    u8 ie_len;
    u16 beacon_interval;
    u32 basic_rates;
    bool channel_fixed;
    bool privacy;
    bool control_port;
    bool userspace_handles_dfs;
    int mcast_rate[3];
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct cfg80211_ibss_params {
    const u8 *ssid;
    const u8 *bssid;
    struct cfg80211_chan_def chandef;
    const u8 *ie;
    u8 ssid_len;
    u8 ie_len;
    u16 beacon_interval;
    u32 basic_rates;
    bool channel_fixed;
    bool privacy;
    bool control_port;
    bool userspace_handles_dfs;
    int mcast_rate[3];
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct cfg80211_ibss_params {
    const u8 *ssid;
    const u8 *bssid;
    struct cfg80211_chan_def chandef;
    const u8 *ie;
    u8 ssid_len;
    u8 ie_len;
    u16 beacon_interval;
    u32 basic_rates;
    bool channel_fixed;
    bool privacy;
    bool control_port;
    bool control_port_over_nl80211;
    bool userspace_handles_dfs;
    int mcast_rate[3];
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct key_params *wep_keys;
    int wep_tx_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct cfg80211_ibss_params {
    const u8 *ssid;
    const u8 *bssid;
    struct cfg80211_chan_def chandef;
    const u8 *ie;
    u8 ssid_len;
    u8 ie_len;
    u16 beacon_interval;
    u32 basic_rates;
    bool channel_fixed;
    bool privacy;
    bool control_port;
    bool control_port_over_nl80211;
    bool userspace_handles_dfs;
    int mcast_rate[3];
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct key_params *wep_keys;
    int wep_tx_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct cfg80211_ibss_params {
    const u8 *ssid;
    const u8 *bssid;
    struct cfg80211_chan_def chandef;
    const u8 *ie;
    u8 ssid_len;
    u8 ie_len;
    u16 beacon_interval;
    u32 basic_rates;
    bool channel_fixed;
    bool privacy;
    bool control_port;
    bool control_port_over_nl80211;
    bool userspace_handles_dfs;
    int mcast_rate[3];
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct key_params *wep_keys;
    int wep_tx_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct cfg80211_ibss_params {
    const u8 *ssid;
    const u8 *bssid;
    struct cfg80211_chan_def chandef;
    const u8 *ie;
    u8 ssid_len;
    u8 ie_len;
    u16 beacon_interval;
    u32 basic_rates;
    bool channel_fixed;
    bool privacy;
    bool control_port;
    bool control_port_over_nl80211;
    bool userspace_handles_dfs;
    int mcast_rate[4];
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct key_params *wep_keys;
    int wep_tx_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct cfg80211_ibss_params {
    const u8 *ssid;
    const u8 *bssid;
    struct cfg80211_chan_def chandef;
    const u8 *ie;
    u8 ssid_len;
    u8 ie_len;
    u16 beacon_interval;
    u32 basic_rates;
    bool channel_fixed;
    bool privacy;
    bool control_port;
    bool control_port_over_nl80211;
    bool userspace_handles_dfs;
    int mcast_rate[4];
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct key_params *wep_keys;
    int wep_tx_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct cfg80211_ibss_params {
    const u8 *ssid;
    const u8 *bssid;
    struct cfg80211_chan_def chandef;
    const u8 *ie;
    u8 ssid_len;
    u8 ie_len;
    u16 beacon_interval;
    u32 basic_rates;
    bool channel_fixed;
    bool privacy;
    bool control_port;
    bool control_port_over_nl80211;
    bool userspace_handles_dfs;
    int mcast_rate[5];
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct key_params *wep_keys;
    int wep_tx_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct cfg80211_ibss_params {
    const u8 *ssid;
    const u8 *bssid;
    struct cfg80211_chan_def chandef;
    const u8 *ie;
    u8 ssid_len;
    u8 ie_len;
    u16 beacon_interval;
    u32 basic_rates;
    bool channel_fixed;
    bool privacy;
    bool control_port;
    bool control_port_over_nl80211;
    bool userspace_handles_dfs;
    int mcast_rate[5];
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct key_params *wep_keys;
    int wep_tx_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct cfg80211_ibss_params {
    const u8 *ssid;
    const u8 *bssid;
    struct cfg80211_chan_def chandef;
    const u8 *ie;
    u8 ssid_len;
    u8 ie_len;
    u16 beacon_interval;
    u32 basic_rates;
    bool channel_fixed;
    bool privacy;
    bool control_port;
    bool control_port_over_nl80211;
    bool userspace_handles_dfs;
    int mcast_rate[5];
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct key_params *wep_keys;
    int wep_tx_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct cfg80211_ibss_params {
    const u8 *ssid;
    const u8 *bssid;
    struct cfg80211_chan_def chandef;
    const u8 *ie;
    u8 ssid_len;
    u8 ie_len;
    u16 beacon_interval;
    u32 basic_rates;
    bool channel_fixed;
    bool privacy;
    bool control_port;
    bool control_port_over_nl80211;
    bool userspace_handles_dfs;
    int mcast_rate[6];
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct key_params *wep_keys;
    int wep_tx_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct cfg80211_ibss_params {
    const u8 *ssid;
    const u8 *bssid;
    struct cfg80211_chan_def chandef;
    const u8 *ie;
    u8 ssid_len;
    u8 ie_len;
    u16 beacon_interval;
    u32 basic_rates;
    bool channel_fixed;
    bool privacy;
    bool control_port;
    bool control_port_over_nl80211;
    bool userspace_handles_dfs;
    int mcast_rate[6];
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct key_params *wep_keys;
    int wep_tx_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct cfg80211_ibss_params {
    const u8 *ssid;
    const u8 *bssid;
    struct cfg80211_chan_def chandef;
    const u8 *ie;
    u8 ssid_len;
    u8 ie_len;
    u16 beacon_interval;
    u32 basic_rates;
    bool channel_fixed;
    bool privacy;
    bool control_port;
    bool control_port_over_nl80211;
    bool userspace_handles_dfs;
    int mcast_rate[6];
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct key_params *wep_keys;
    int wep_tx_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct cfg80211_ibss_params {
    const u8 *ssid;
    const u8 *bssid;
    struct cfg80211_chan_def chandef;
    const u8 *ie;
    u8 ssid_len;
    u8 ie_len;
    u16 beacon_interval;
    u32 basic_rates;
    bool channel_fixed;
    bool privacy;
    bool control_port;
    bool control_port_over_nl80211;
    bool userspace_handles_dfs;
    int mcast_rate[6];
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct key_params *wep_keys;
    int wep_tx_key;
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
struct cfg80211_ibss_params {
    const u8 *ssid;
    const u8 *bssid;
    struct cfg80211_chan_def chandef;
    const u8 *ie;
    u8 ssid_len;
    u8 ie_len;
    u16 beacon_interval;
    u32 basic_rates;
    bool channel_fixed;
    bool privacy;
    bool control_port;
    bool control_port_over_nl80211;
    bool userspace_handles_dfs;
    int mcast_rate[4];
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct key_params *wep_keys;
    int wep_tx_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct cfg80211_ibss_params {
    const u8 *ssid;
    const u8 *bssid;
    struct cfg80211_chan_def chandef;
    const u8 *ie;
    u8 ssid_len;
    u8 ie_len;
    u16 beacon_interval;
    u32 basic_rates;
    bool channel_fixed;
    bool privacy;
    bool control_port;
    bool control_port_over_nl80211;
    bool userspace_handles_dfs;
    int mcast_rate[4];
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct key_params *wep_keys;
    int wep_tx_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct cfg80211_ibss_params {
    const u8 *ssid;
    const u8 *bssid;
    struct cfg80211_chan_def chandef;
    const u8 *ie;
    u8 ssid_len;
    u8 ie_len;
    u16 beacon_interval;
    u32 basic_rates;
    bool channel_fixed;
    bool privacy;
    bool control_port;
    bool control_port_over_nl80211;
    bool userspace_handles_dfs;
    int mcast_rate[4];
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct key_params *wep_keys;
    int wep_tx_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct cfg80211_ibss_params {
    const u8 *ssid;
    const u8 *bssid;
    struct cfg80211_chan_def chandef;
    const u8 *ie;
    u8 ssid_len;
    u8 ie_len;
    u16 beacon_interval;
    u32 basic_rates;
    bool channel_fixed;
    bool privacy;
    bool control_port;
    bool control_port_over_nl80211;
    bool userspace_handles_dfs;
    int mcast_rate[4];
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct key_params *wep_keys;
    int wep_tx_key;
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
struct cfg80211_ibss_params {
    const u8 *ssid;
    const u8 *bssid;
    struct cfg80211_chan_def chandef;
    const u8 *ie;
    u8 ssid_len;
    u8 ie_len;
    u16 beacon_interval;
    u32 basic_rates;
    bool channel_fixed;
    bool privacy;
    bool control_port;
    bool control_port_over_nl80211;
    bool userspace_handles_dfs;
    int mcast_rate[4];
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct key_params *wep_keys;
    int wep_tx_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct cfg80211_ibss_params {
    const u8 *ssid;
    const u8 *bssid;
    struct cfg80211_chan_def chandef;
    const u8 *ie;
    u8 ssid_len;
    u8 ie_len;
    u16 beacon_interval;
    u32 basic_rates;
    bool channel_fixed;
    bool privacy;
    bool control_port;
    bool control_port_over_nl80211;
    bool userspace_handles_dfs;
    int mcast_rate[4];
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct key_params *wep_keys;
    int wep_tx_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct cfg80211_ibss_params {
    const u8 *ssid;
    const u8 *bssid;
    struct cfg80211_chan_def chandef;
    const u8 *ie;
    u8 ssid_len;
    u8 ie_len;
    u16 beacon_interval;
    u32 basic_rates;
    bool channel_fixed;
    bool privacy;
    bool control_port;
    bool control_port_over_nl80211;
    bool userspace_handles_dfs;
    int mcast_rate[4];
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct key_params *wep_keys;
    int wep_tx_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cfg80211_ibss_params {
    const u8 *ssid;
    const u8 *bssid;
    struct cfg80211_chan_def chandef;
    const u8 *ie;
    u8 ssid_len;
    u8 ie_len;
    u16 beacon_interval;
    u32 basic_rates;
    bool channel_fixed;
    bool privacy;
    bool control_port;
    bool control_port_over_nl80211;
    bool userspace_handles_dfs;
    int mcast_rate[4];
    struct ieee80211_ht_cap ht_capa;
    struct ieee80211_ht_cap ht_capa_mask;
    struct key_params *wep_keys;
    int wep_tx_key;
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
<code>bool control_port_over_nl80211</code>
</li>
<li>
<b>Field added. </b>
<code>struct key_params *wep_keys</code>
</li>
<li>
<b>Field added. </b>
<code>int wep_tx_key</code>
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
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int mcast_rate[3]</code> ➡️ <code>int mcast_rate[4]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int mcast_rate[4]</code> ➡️ <code>int mcast_rate[5]</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int mcast_rate[5]</code> ➡️ <code>int mcast_rate[6]</code>
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
