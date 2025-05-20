# Struct: <code>drm_hdmi_info</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
In <code>4.8</code>: Absent ⚠️
</li>
<li>
In <code>4.10</code>: Absent ⚠️
</li>
<li>
In <code>4.13</code>: Absent ⚠️
</li>
<li>
In <code>4.15</code>: Absent ⚠️
</li>
<li>
In <code>4.18</code>: Absent ⚠️
</li>
<li>
In <code>5.0</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct drm_hdmi_info {
    struct drm_scdc scdc;
    long unsigned int y420_vdb_modes[2];
    long unsigned int y420_cmdb_modes[2];
    u64 y420_cmdb_map;
    u8 y420_dc_modes;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct drm_hdmi_info {
    struct drm_scdc scdc;
    long unsigned int y420_vdb_modes[2];
    long unsigned int y420_cmdb_modes[2];
    u64 y420_cmdb_map;
    u8 y420_dc_modes;
};
```
</details>
</li>
<li>
In <code>5.8</code>: Absent ⚠️
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
In <code>5.19</code>: Absent ⚠️
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
In <code>6.5</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct drm_hdmi_info {
    struct drm_scdc scdc;
    long unsigned int y420_vdb_modes[4];
    long unsigned int y420_cmdb_modes[4];
    u8 y420_dc_modes;
    u8 max_frl_rate_per_lane;
    u8 max_lanes;
    struct drm_hdmi_dsc_cap dsc_cap;
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
struct drm_hdmi_info {
    struct drm_scdc scdc;
    long unsigned int y420_vdb_modes[2];
    long unsigned int y420_cmdb_modes[2];
    u64 y420_cmdb_map;
    u8 y420_dc_modes;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct drm_hdmi_info {
    struct drm_scdc scdc;
    long unsigned int y420_vdb_modes[4];
    long unsigned int y420_cmdb_modes[4];
    u64 y420_cmdb_map;
    u8 y420_dc_modes;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct drm_hdmi_info {
    struct drm_scdc scdc;
    long unsigned int y420_vdb_modes[2];
    long unsigned int y420_cmdb_modes[2];
    u64 y420_cmdb_map;
    u8 y420_dc_modes;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct drm_hdmi_info {
    struct drm_scdc scdc;
    long unsigned int y420_vdb_modes[2];
    long unsigned int y420_cmdb_modes[2];
    u64 y420_cmdb_map;
    u8 y420_dc_modes;
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
struct drm_hdmi_info {
    struct drm_scdc scdc;
    long unsigned int y420_vdb_modes[2];
    long unsigned int y420_cmdb_modes[2];
    u64 y420_cmdb_map;
    u8 y420_dc_modes;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct drm_hdmi_info {
    struct drm_scdc scdc;
    long unsigned int y420_vdb_modes[2];
    long unsigned int y420_cmdb_modes[2];
    u64 y420_cmdb_map;
    u8 y420_dc_modes;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct drm_hdmi_info {
    struct drm_scdc scdc;
    long unsigned int y420_vdb_modes[2];
    long unsigned int y420_cmdb_modes[2];
    u64 y420_cmdb_map;
    u8 y420_dc_modes;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct drm_hdmi_info {
    struct drm_scdc scdc;
    long unsigned int y420_vdb_modes[2];
    long unsigned int y420_cmdb_modes[2];
    u64 y420_cmdb_map;
    u8 y420_dc_modes;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
</ul>
<b>Arch</b>
<ul>
<li>
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long unsigned int y420_vdb_modes[2]</code> ➡️ <code>long unsigned int y420_vdb_modes[4]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int y420_cmdb_modes[2]</code> ➡️ <code>long unsigned int y420_cmdb_modes[4]</code>
</li>
</ul>
</details>
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
