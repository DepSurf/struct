# Struct: <code>regulatory_request</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct regulatory_request {
    struct callback_head callback_head;
    int wiphy_idx;
    enum nl80211_reg_initiator initiator;
    enum nl80211_user_reg_hint_type user_reg_hint_type;
    char alpha2[2];
    enum nl80211_dfs_regions dfs_region;
    bool intersect;
    bool processed;
    enum environment_cap country_ie_env;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct regulatory_request {
    struct callback_head callback_head;
    int wiphy_idx;
    enum nl80211_reg_initiator initiator;
    enum nl80211_user_reg_hint_type user_reg_hint_type;
    char alpha2[2];
    enum nl80211_dfs_regions dfs_region;
    bool intersect;
    bool processed;
    enum environment_cap country_ie_env;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct regulatory_request {
    struct callback_head callback_head;
    int wiphy_idx;
    enum nl80211_reg_initiator initiator;
    enum nl80211_user_reg_hint_type user_reg_hint_type;
    char alpha2[2];
    enum nl80211_dfs_regions dfs_region;
    bool intersect;
    bool processed;
    enum environment_cap country_ie_env;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct regulatory_request {
    struct callback_head callback_head;
    int wiphy_idx;
    enum nl80211_reg_initiator initiator;
    enum nl80211_user_reg_hint_type user_reg_hint_type;
    char alpha2[2];
    enum nl80211_dfs_regions dfs_region;
    bool intersect;
    bool processed;
    enum environment_cap country_ie_env;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct regulatory_request {
    struct callback_head callback_head;
    int wiphy_idx;
    enum nl80211_reg_initiator initiator;
    enum nl80211_user_reg_hint_type user_reg_hint_type;
    char alpha2[2];
    enum nl80211_dfs_regions dfs_region;
    bool intersect;
    bool processed;
    enum environment_cap country_ie_env;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct regulatory_request {
    struct callback_head callback_head;
    int wiphy_idx;
    enum nl80211_reg_initiator initiator;
    enum nl80211_user_reg_hint_type user_reg_hint_type;
    char alpha2[3];
    enum nl80211_dfs_regions dfs_region;
    bool intersect;
    bool processed;
    enum environment_cap country_ie_env;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct regulatory_request {
    struct callback_head callback_head;
    int wiphy_idx;
    enum nl80211_reg_initiator initiator;
    enum nl80211_user_reg_hint_type user_reg_hint_type;
    char alpha2[3];
    enum nl80211_dfs_regions dfs_region;
    bool intersect;
    bool processed;
    enum environment_cap country_ie_env;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct regulatory_request {
    struct callback_head callback_head;
    int wiphy_idx;
    enum nl80211_reg_initiator initiator;
    enum nl80211_user_reg_hint_type user_reg_hint_type;
    char alpha2[3];
    enum nl80211_dfs_regions dfs_region;
    bool intersect;
    bool processed;
    enum environment_cap country_ie_env;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct regulatory_request {
    struct callback_head callback_head;
    int wiphy_idx;
    enum nl80211_reg_initiator initiator;
    enum nl80211_user_reg_hint_type user_reg_hint_type;
    char alpha2[3];
    enum nl80211_dfs_regions dfs_region;
    bool intersect;
    bool processed;
    enum environment_cap country_ie_env;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct regulatory_request {
    struct callback_head callback_head;
    int wiphy_idx;
    enum nl80211_reg_initiator initiator;
    enum nl80211_user_reg_hint_type user_reg_hint_type;
    char alpha2[3];
    enum nl80211_dfs_regions dfs_region;
    bool intersect;
    bool processed;
    enum environment_cap country_ie_env;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct regulatory_request {
    struct callback_head callback_head;
    int wiphy_idx;
    enum nl80211_reg_initiator initiator;
    enum nl80211_user_reg_hint_type user_reg_hint_type;
    char alpha2[3];
    enum nl80211_dfs_regions dfs_region;
    bool intersect;
    bool processed;
    enum environment_cap country_ie_env;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct regulatory_request {
    struct callback_head callback_head;
    int wiphy_idx;
    enum nl80211_reg_initiator initiator;
    enum nl80211_user_reg_hint_type user_reg_hint_type;
    char alpha2[3];
    enum nl80211_dfs_regions dfs_region;
    bool intersect;
    bool processed;
    enum environment_cap country_ie_env;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct regulatory_request {
    struct callback_head callback_head;
    int wiphy_idx;
    enum nl80211_reg_initiator initiator;
    enum nl80211_user_reg_hint_type user_reg_hint_type;
    char alpha2[3];
    enum nl80211_dfs_regions dfs_region;
    bool intersect;
    bool processed;
    enum environment_cap country_ie_env;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct regulatory_request {
    struct callback_head callback_head;
    int wiphy_idx;
    enum nl80211_reg_initiator initiator;
    enum nl80211_user_reg_hint_type user_reg_hint_type;
    char alpha2[3];
    enum nl80211_dfs_regions dfs_region;
    bool intersect;
    bool processed;
    enum environment_cap country_ie_env;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct regulatory_request {
    struct callback_head callback_head;
    int wiphy_idx;
    enum nl80211_reg_initiator initiator;
    enum nl80211_user_reg_hint_type user_reg_hint_type;
    char alpha2[3];
    enum nl80211_dfs_regions dfs_region;
    bool intersect;
    bool processed;
    enum environment_cap country_ie_env;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct regulatory_request {
    struct callback_head callback_head;
    int wiphy_idx;
    enum nl80211_reg_initiator initiator;
    enum nl80211_user_reg_hint_type user_reg_hint_type;
    char alpha2[3];
    enum nl80211_dfs_regions dfs_region;
    bool intersect;
    bool processed;
    enum environment_cap country_ie_env;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct regulatory_request {
    struct callback_head callback_head;
    int wiphy_idx;
    enum nl80211_reg_initiator initiator;
    enum nl80211_user_reg_hint_type user_reg_hint_type;
    char alpha2[3];
    enum nl80211_dfs_regions dfs_region;
    bool intersect;
    bool processed;
    enum environment_cap country_ie_env;
    struct list_head list;
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
struct regulatory_request {
    struct callback_head callback_head;
    int wiphy_idx;
    enum nl80211_reg_initiator initiator;
    enum nl80211_user_reg_hint_type user_reg_hint_type;
    char alpha2[3];
    enum nl80211_dfs_regions dfs_region;
    bool intersect;
    bool processed;
    enum environment_cap country_ie_env;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct regulatory_request {
    struct callback_head callback_head;
    int wiphy_idx;
    enum nl80211_reg_initiator initiator;
    enum nl80211_user_reg_hint_type user_reg_hint_type;
    char alpha2[3];
    enum nl80211_dfs_regions dfs_region;
    bool intersect;
    bool processed;
    enum environment_cap country_ie_env;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct regulatory_request {
    struct callback_head callback_head;
    int wiphy_idx;
    enum nl80211_reg_initiator initiator;
    enum nl80211_user_reg_hint_type user_reg_hint_type;
    char alpha2[3];
    enum nl80211_dfs_regions dfs_region;
    bool intersect;
    bool processed;
    enum environment_cap country_ie_env;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct regulatory_request {
    struct callback_head callback_head;
    int wiphy_idx;
    enum nl80211_reg_initiator initiator;
    enum nl80211_user_reg_hint_type user_reg_hint_type;
    char alpha2[3];
    enum nl80211_dfs_regions dfs_region;
    bool intersect;
    bool processed;
    enum environment_cap country_ie_env;
    struct list_head list;
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
struct regulatory_request {
    struct callback_head callback_head;
    int wiphy_idx;
    enum nl80211_reg_initiator initiator;
    enum nl80211_user_reg_hint_type user_reg_hint_type;
    char alpha2[3];
    enum nl80211_dfs_regions dfs_region;
    bool intersect;
    bool processed;
    enum environment_cap country_ie_env;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct regulatory_request {
    struct callback_head callback_head;
    int wiphy_idx;
    enum nl80211_reg_initiator initiator;
    enum nl80211_user_reg_hint_type user_reg_hint_type;
    char alpha2[3];
    enum nl80211_dfs_regions dfs_region;
    bool intersect;
    bool processed;
    enum environment_cap country_ie_env;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct regulatory_request {
    struct callback_head callback_head;
    int wiphy_idx;
    enum nl80211_reg_initiator initiator;
    enum nl80211_user_reg_hint_type user_reg_hint_type;
    char alpha2[3];
    enum nl80211_dfs_regions dfs_region;
    bool intersect;
    bool processed;
    enum environment_cap country_ie_env;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct regulatory_request {
    struct callback_head callback_head;
    int wiphy_idx;
    enum nl80211_reg_initiator initiator;
    enum nl80211_user_reg_hint_type user_reg_hint_type;
    char alpha2[3];
    enum nl80211_dfs_regions dfs_region;
    bool intersect;
    bool processed;
    enum environment_cap country_ie_env;
    struct list_head list;
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
<b>Field type changed. </b>
<code>char alpha2[2]</code> ➡️ <code>char alpha2[3]</code>
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
