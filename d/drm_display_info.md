# Struct: <code>drm_display_info</code>

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
struct drm_display_info {
    unsigned int width_mm;
    unsigned int height_mm;
    unsigned int bpc;
    enum subpixel_order subpixel_order;
    int panel_orientation;
    u32 color_formats;
    const u32 *bus_formats;
    unsigned int num_bus_formats;
    u32 bus_flags;
    int max_tmds_clock;
    bool dvi_dual;
    bool has_hdmi_infoframe;
    bool rgb_quant_range_selectable;
    u8 edid_hdmi_dc_modes;
    u8 cea_rev;
    struct drm_hdmi_info hdmi;
    bool non_desktop;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct drm_display_info {
    unsigned int width_mm;
    unsigned int height_mm;
    unsigned int bpc;
    enum subpixel_order subpixel_order;
    int panel_orientation;
    u32 color_formats;
    const u32 *bus_formats;
    unsigned int num_bus_formats;
    u32 bus_flags;
    int max_tmds_clock;
    bool dvi_dual;
    bool has_hdmi_infoframe;
    bool rgb_quant_range_selectable;
    u8 edid_hdmi_dc_modes;
    u8 cea_rev;
    struct drm_hdmi_info hdmi;
    bool non_desktop;
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
struct drm_display_info {
    unsigned int width_mm;
    unsigned int height_mm;
    unsigned int bpc;
    enum subpixel_order subpixel_order;
    int panel_orientation;
    u32 color_formats;
    const u32 *bus_formats;
    unsigned int num_bus_formats;
    u32 bus_flags;
    int max_tmds_clock;
    bool dvi_dual;
    bool is_hdmi;
    bool has_audio;
    bool has_hdmi_infoframe;
    bool rgb_quant_range_selectable;
    u8 edid_hdmi_rgb444_dc_modes;
    u8 edid_hdmi_ycbcr444_dc_modes;
    u8 cea_rev;
    struct drm_hdmi_info hdmi;
    bool non_desktop;
    struct drm_monitor_range_info monitor_range;
    struct drm_luminance_range_info luminance_range;
    u8 mso_stream_count;
    u8 mso_pixel_overlap;
    u32 max_dsc_bpp;
    u8 *vics;
    int vics_len;
    u32 quirks;
    u16 source_physical_address;
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
struct drm_display_info {
    unsigned int width_mm;
    unsigned int height_mm;
    unsigned int bpc;
    enum subpixel_order subpixel_order;
    int panel_orientation;
    u32 color_formats;
    const u32 *bus_formats;
    unsigned int num_bus_formats;
    u32 bus_flags;
    int max_tmds_clock;
    bool dvi_dual;
    bool has_hdmi_infoframe;
    bool rgb_quant_range_selectable;
    u8 edid_hdmi_dc_modes;
    u8 cea_rev;
    struct drm_hdmi_info hdmi;
    bool non_desktop;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct drm_display_info {
    unsigned int width_mm;
    unsigned int height_mm;
    unsigned int bpc;
    enum subpixel_order subpixel_order;
    int panel_orientation;
    u32 color_formats;
    const u32 *bus_formats;
    unsigned int num_bus_formats;
    u32 bus_flags;
    int max_tmds_clock;
    bool dvi_dual;
    bool has_hdmi_infoframe;
    bool rgb_quant_range_selectable;
    u8 edid_hdmi_dc_modes;
    u8 cea_rev;
    struct drm_hdmi_info hdmi;
    bool non_desktop;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct drm_display_info {
    unsigned int width_mm;
    unsigned int height_mm;
    unsigned int bpc;
    enum subpixel_order subpixel_order;
    int panel_orientation;
    u32 color_formats;
    const u32 *bus_formats;
    unsigned int num_bus_formats;
    u32 bus_flags;
    int max_tmds_clock;
    bool dvi_dual;
    bool has_hdmi_infoframe;
    bool rgb_quant_range_selectable;
    u8 edid_hdmi_dc_modes;
    u8 cea_rev;
    struct drm_hdmi_info hdmi;
    bool non_desktop;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct drm_display_info {
    unsigned int width_mm;
    unsigned int height_mm;
    unsigned int bpc;
    enum subpixel_order subpixel_order;
    int panel_orientation;
    u32 color_formats;
    const u32 *bus_formats;
    unsigned int num_bus_formats;
    u32 bus_flags;
    int max_tmds_clock;
    bool dvi_dual;
    bool has_hdmi_infoframe;
    bool rgb_quant_range_selectable;
    u8 edid_hdmi_dc_modes;
    u8 cea_rev;
    struct drm_hdmi_info hdmi;
    bool non_desktop;
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
struct drm_display_info {
    unsigned int width_mm;
    unsigned int height_mm;
    unsigned int bpc;
    enum subpixel_order subpixel_order;
    int panel_orientation;
    u32 color_formats;
    const u32 *bus_formats;
    unsigned int num_bus_formats;
    u32 bus_flags;
    int max_tmds_clock;
    bool dvi_dual;
    bool has_hdmi_infoframe;
    bool rgb_quant_range_selectable;
    u8 edid_hdmi_dc_modes;
    u8 cea_rev;
    struct drm_hdmi_info hdmi;
    bool non_desktop;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct drm_display_info {
    unsigned int width_mm;
    unsigned int height_mm;
    unsigned int bpc;
    enum subpixel_order subpixel_order;
    int panel_orientation;
    u32 color_formats;
    const u32 *bus_formats;
    unsigned int num_bus_formats;
    u32 bus_flags;
    int max_tmds_clock;
    bool dvi_dual;
    bool has_hdmi_infoframe;
    bool rgb_quant_range_selectable;
    u8 edid_hdmi_dc_modes;
    u8 cea_rev;
    struct drm_hdmi_info hdmi;
    bool non_desktop;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct drm_display_info {
    unsigned int width_mm;
    unsigned int height_mm;
    unsigned int bpc;
    enum subpixel_order subpixel_order;
    int panel_orientation;
    u32 color_formats;
    const u32 *bus_formats;
    unsigned int num_bus_formats;
    u32 bus_flags;
    int max_tmds_clock;
    bool dvi_dual;
    bool has_hdmi_infoframe;
    bool rgb_quant_range_selectable;
    u8 edid_hdmi_dc_modes;
    u8 cea_rev;
    struct drm_hdmi_info hdmi;
    bool non_desktop;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct drm_display_info {
    unsigned int width_mm;
    unsigned int height_mm;
    unsigned int bpc;
    enum subpixel_order subpixel_order;
    int panel_orientation;
    u32 color_formats;
    const u32 *bus_formats;
    unsigned int num_bus_formats;
    u32 bus_flags;
    int max_tmds_clock;
    bool dvi_dual;
    bool has_hdmi_infoframe;
    bool rgb_quant_range_selectable;
    u8 edid_hdmi_dc_modes;
    u8 cea_rev;
    struct drm_hdmi_info hdmi;
    bool non_desktop;
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
