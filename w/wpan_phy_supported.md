# Struct: <code>wpan_phy_supported</code>

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
struct wpan_phy_supported {
    u32 channels[32];
    u32 cca_modes;
    u32 cca_opts;
    u32 iftypes;
    enum nl802154_supported_bool_states lbt;
    u8 min_minbe;
    u8 max_minbe;
    u8 min_maxbe;
    u8 max_maxbe;
    u8 min_csma_backoffs;
    u8 max_csma_backoffs;
    s8 min_frame_retries;
    s8 max_frame_retries;
    size_t tx_powers_size;
    size_t cca_ed_levels_size;
    const s32 *tx_powers;
    const s32 *cca_ed_levels;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct wpan_phy_supported {
    u32 channels[32];
    u32 cca_modes;
    u32 cca_opts;
    u32 iftypes;
    enum nl802154_supported_bool_states lbt;
    u8 min_minbe;
    u8 max_minbe;
    u8 min_maxbe;
    u8 max_maxbe;
    u8 min_csma_backoffs;
    u8 max_csma_backoffs;
    s8 min_frame_retries;
    s8 max_frame_retries;
    size_t tx_powers_size;
    size_t cca_ed_levels_size;
    const s32 *tx_powers;
    const s32 *cca_ed_levels;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct wpan_phy_supported {
    u32 channels[32];
    u32 cca_modes;
    u32 cca_opts;
    u32 iftypes;
    enum nl802154_supported_bool_states lbt;
    u8 min_minbe;
    u8 max_minbe;
    u8 min_maxbe;
    u8 max_maxbe;
    u8 min_csma_backoffs;
    u8 max_csma_backoffs;
    s8 min_frame_retries;
    s8 max_frame_retries;
    size_t tx_powers_size;
    size_t cca_ed_levels_size;
    const s32 *tx_powers;
    const s32 *cca_ed_levels;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct wpan_phy_supported {
    u32 channels[32];
    u32 cca_modes;
    u32 cca_opts;
    u32 iftypes;
    enum nl802154_supported_bool_states lbt;
    u8 min_minbe;
    u8 max_minbe;
    u8 min_maxbe;
    u8 max_maxbe;
    u8 min_csma_backoffs;
    u8 max_csma_backoffs;
    s8 min_frame_retries;
    s8 max_frame_retries;
    size_t tx_powers_size;
    size_t cca_ed_levels_size;
    const s32 *tx_powers;
    const s32 *cca_ed_levels;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct wpan_phy_supported {
    u32 channels[32];
    u32 cca_modes;
    u32 cca_opts;
    u32 iftypes;
    enum nl802154_supported_bool_states lbt;
    u8 min_minbe;
    u8 max_minbe;
    u8 min_maxbe;
    u8 max_maxbe;
    u8 min_csma_backoffs;
    u8 max_csma_backoffs;
    s8 min_frame_retries;
    s8 max_frame_retries;
    size_t tx_powers_size;
    size_t cca_ed_levels_size;
    const s32 *tx_powers;
    const s32 *cca_ed_levels;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct wpan_phy_supported {
    u32 channels[32];
    u32 cca_modes;
    u32 cca_opts;
    u32 iftypes;
    enum nl802154_supported_bool_states lbt;
    u8 min_minbe;
    u8 max_minbe;
    u8 min_maxbe;
    u8 max_maxbe;
    u8 min_csma_backoffs;
    u8 max_csma_backoffs;
    s8 min_frame_retries;
    s8 max_frame_retries;
    size_t tx_powers_size;
    size_t cca_ed_levels_size;
    const s32 *tx_powers;
    const s32 *cca_ed_levels;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct wpan_phy_supported {
    u32 channels[32];
    u32 cca_modes;
    u32 cca_opts;
    u32 iftypes;
    enum nl802154_supported_bool_states lbt;
    u8 min_minbe;
    u8 max_minbe;
    u8 min_maxbe;
    u8 max_maxbe;
    u8 min_csma_backoffs;
    u8 max_csma_backoffs;
    s8 min_frame_retries;
    s8 max_frame_retries;
    size_t tx_powers_size;
    size_t cca_ed_levels_size;
    const s32 *tx_powers;
    const s32 *cca_ed_levels;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct wpan_phy_supported {
    u32 channels[32];
    u32 cca_modes;
    u32 cca_opts;
    u32 iftypes;
    enum nl802154_supported_bool_states lbt;
    u8 min_minbe;
    u8 max_minbe;
    u8 min_maxbe;
    u8 max_maxbe;
    u8 min_csma_backoffs;
    u8 max_csma_backoffs;
    s8 min_frame_retries;
    s8 max_frame_retries;
    size_t tx_powers_size;
    size_t cca_ed_levels_size;
    const s32 *tx_powers;
    const s32 *cca_ed_levels;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct wpan_phy_supported {
    u32 channels[32];
    u32 cca_modes;
    u32 cca_opts;
    u32 iftypes;
    enum nl802154_supported_bool_states lbt;
    u8 min_minbe;
    u8 max_minbe;
    u8 min_maxbe;
    u8 max_maxbe;
    u8 min_csma_backoffs;
    u8 max_csma_backoffs;
    s8 min_frame_retries;
    s8 max_frame_retries;
    size_t tx_powers_size;
    size_t cca_ed_levels_size;
    const s32 *tx_powers;
    const s32 *cca_ed_levels;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct wpan_phy_supported {
    u32 channels[32];
    u32 cca_modes;
    u32 cca_opts;
    u32 iftypes;
    enum nl802154_supported_bool_states lbt;
    u8 min_minbe;
    u8 max_minbe;
    u8 min_maxbe;
    u8 max_maxbe;
    u8 min_csma_backoffs;
    u8 max_csma_backoffs;
    s8 min_frame_retries;
    s8 max_frame_retries;
    size_t tx_powers_size;
    size_t cca_ed_levels_size;
    const s32 *tx_powers;
    const s32 *cca_ed_levels;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct wpan_phy_supported {
    u32 channels[32];
    u32 cca_modes;
    u32 cca_opts;
    u32 iftypes;
    enum nl802154_supported_bool_states lbt;
    u8 min_minbe;
    u8 max_minbe;
    u8 min_maxbe;
    u8 max_maxbe;
    u8 min_csma_backoffs;
    u8 max_csma_backoffs;
    s8 min_frame_retries;
    s8 max_frame_retries;
    size_t tx_powers_size;
    size_t cca_ed_levels_size;
    const s32 *tx_powers;
    const s32 *cca_ed_levels;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct wpan_phy_supported {
    u32 channels[32];
    u32 cca_modes;
    u32 cca_opts;
    u32 iftypes;
    enum nl802154_supported_bool_states lbt;
    u8 min_minbe;
    u8 max_minbe;
    u8 min_maxbe;
    u8 max_maxbe;
    u8 min_csma_backoffs;
    u8 max_csma_backoffs;
    s8 min_frame_retries;
    s8 max_frame_retries;
    size_t tx_powers_size;
    size_t cca_ed_levels_size;
    const s32 *tx_powers;
    const s32 *cca_ed_levels;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct wpan_phy_supported {
    u32 channels[32];
    u32 cca_modes;
    u32 cca_opts;
    u32 iftypes;
    enum nl802154_supported_bool_states lbt;
    u8 min_minbe;
    u8 max_minbe;
    u8 min_maxbe;
    u8 max_maxbe;
    u8 min_csma_backoffs;
    u8 max_csma_backoffs;
    s8 min_frame_retries;
    s8 max_frame_retries;
    size_t tx_powers_size;
    size_t cca_ed_levels_size;
    const s32 *tx_powers;
    const s32 *cca_ed_levels;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct wpan_phy_supported {
    u32 channels[32];
    u32 cca_modes;
    u32 cca_opts;
    u32 iftypes;
    enum nl802154_supported_bool_states lbt;
    u8 min_minbe;
    u8 max_minbe;
    u8 min_maxbe;
    u8 max_maxbe;
    u8 min_csma_backoffs;
    u8 max_csma_backoffs;
    s8 min_frame_retries;
    s8 max_frame_retries;
    size_t tx_powers_size;
    size_t cca_ed_levels_size;
    const s32 *tx_powers;
    const s32 *cca_ed_levels;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct wpan_phy_supported {
    u32 channels[32];
    u32 cca_modes;
    u32 cca_opts;
    u32 iftypes;
    enum nl802154_supported_bool_states lbt;
    u8 min_minbe;
    u8 max_minbe;
    u8 min_maxbe;
    u8 max_maxbe;
    u8 min_csma_backoffs;
    u8 max_csma_backoffs;
    s8 min_frame_retries;
    s8 max_frame_retries;
    size_t tx_powers_size;
    size_t cca_ed_levels_size;
    const s32 *tx_powers;
    const s32 *cca_ed_levels;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct wpan_phy_supported {
    u32 channels[32];
    u32 cca_modes;
    u32 cca_opts;
    u32 iftypes;
    enum nl802154_supported_bool_states lbt;
    u8 min_minbe;
    u8 max_minbe;
    u8 min_maxbe;
    u8 max_maxbe;
    u8 min_csma_backoffs;
    u8 max_csma_backoffs;
    s8 min_frame_retries;
    s8 max_frame_retries;
    size_t tx_powers_size;
    size_t cca_ed_levels_size;
    const s32 *tx_powers;
    const s32 *cca_ed_levels;
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
struct wpan_phy_supported {
    u32 channels[32];
    u32 cca_modes;
    u32 cca_opts;
    u32 iftypes;
    enum nl802154_supported_bool_states lbt;
    u8 min_minbe;
    u8 max_minbe;
    u8 min_maxbe;
    u8 max_maxbe;
    u8 min_csma_backoffs;
    u8 max_csma_backoffs;
    s8 min_frame_retries;
    s8 max_frame_retries;
    size_t tx_powers_size;
    size_t cca_ed_levels_size;
    const s32 *tx_powers;
    const s32 *cca_ed_levels;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct wpan_phy_supported {
    u32 channels[32];
    u32 cca_modes;
    u32 cca_opts;
    u32 iftypes;
    enum nl802154_supported_bool_states lbt;
    u8 min_minbe;
    u8 max_minbe;
    u8 min_maxbe;
    u8 max_maxbe;
    u8 min_csma_backoffs;
    u8 max_csma_backoffs;
    s8 min_frame_retries;
    s8 max_frame_retries;
    size_t tx_powers_size;
    size_t cca_ed_levels_size;
    const s32 *tx_powers;
    const s32 *cca_ed_levels;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct wpan_phy_supported {
    u32 channels[32];
    u32 cca_modes;
    u32 cca_opts;
    u32 iftypes;
    enum nl802154_supported_bool_states lbt;
    u8 min_minbe;
    u8 max_minbe;
    u8 min_maxbe;
    u8 max_maxbe;
    u8 min_csma_backoffs;
    u8 max_csma_backoffs;
    s8 min_frame_retries;
    s8 max_frame_retries;
    size_t tx_powers_size;
    size_t cca_ed_levels_size;
    const s32 *tx_powers;
    const s32 *cca_ed_levels;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct wpan_phy_supported {
    u32 channels[32];
    u32 cca_modes;
    u32 cca_opts;
    u32 iftypes;
    enum nl802154_supported_bool_states lbt;
    u8 min_minbe;
    u8 max_minbe;
    u8 min_maxbe;
    u8 max_maxbe;
    u8 min_csma_backoffs;
    u8 max_csma_backoffs;
    s8 min_frame_retries;
    s8 max_frame_retries;
    size_t tx_powers_size;
    size_t cca_ed_levels_size;
    const s32 *tx_powers;
    const s32 *cca_ed_levels;
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
struct wpan_phy_supported {
    u32 channels[32];
    u32 cca_modes;
    u32 cca_opts;
    u32 iftypes;
    enum nl802154_supported_bool_states lbt;
    u8 min_minbe;
    u8 max_minbe;
    u8 min_maxbe;
    u8 max_maxbe;
    u8 min_csma_backoffs;
    u8 max_csma_backoffs;
    s8 min_frame_retries;
    s8 max_frame_retries;
    size_t tx_powers_size;
    size_t cca_ed_levels_size;
    const s32 *tx_powers;
    const s32 *cca_ed_levels;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct wpan_phy_supported {
    u32 channels[32];
    u32 cca_modes;
    u32 cca_opts;
    u32 iftypes;
    enum nl802154_supported_bool_states lbt;
    u8 min_minbe;
    u8 max_minbe;
    u8 min_maxbe;
    u8 max_maxbe;
    u8 min_csma_backoffs;
    u8 max_csma_backoffs;
    s8 min_frame_retries;
    s8 max_frame_retries;
    size_t tx_powers_size;
    size_t cca_ed_levels_size;
    const s32 *tx_powers;
    const s32 *cca_ed_levels;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct wpan_phy_supported {
    u32 channels[32];
    u32 cca_modes;
    u32 cca_opts;
    u32 iftypes;
    enum nl802154_supported_bool_states lbt;
    u8 min_minbe;
    u8 max_minbe;
    u8 min_maxbe;
    u8 max_maxbe;
    u8 min_csma_backoffs;
    u8 max_csma_backoffs;
    s8 min_frame_retries;
    s8 max_frame_retries;
    size_t tx_powers_size;
    size_t cca_ed_levels_size;
    const s32 *tx_powers;
    const s32 *cca_ed_levels;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct wpan_phy_supported {
    u32 channels[32];
    u32 cca_modes;
    u32 cca_opts;
    u32 iftypes;
    enum nl802154_supported_bool_states lbt;
    u8 min_minbe;
    u8 max_minbe;
    u8 min_maxbe;
    u8 max_maxbe;
    u8 min_csma_backoffs;
    u8 max_csma_backoffs;
    s8 min_frame_retries;
    s8 max_frame_retries;
    size_t tx_powers_size;
    size_t cca_ed_levels_size;
    const s32 *tx_powers;
    const s32 *cca_ed_levels;
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
