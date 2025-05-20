# Struct: <code>drm_connector_state</code>

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
struct drm_connector_state {
    struct drm_connector *connector;
    struct drm_crtc *crtc;
    struct drm_encoder *best_encoder;
    enum drm_link_status link_status;
    struct drm_atomic_state *state;
    struct drm_crtc_commit *commit;
    struct drm_tv_connector_state tv;
    bool self_refresh_aware;
    enum hdmi_picture_aspect picture_aspect_ratio;
    unsigned int content_type;
    unsigned int scaling_mode;
    unsigned int content_protection;
    u32 colorspace;
    struct drm_writeback_job *writeback_job;
    u8 max_requested_bpc;
    u8 max_bpc;
    struct drm_property_blob *hdr_output_metadata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct drm_connector_state {
    struct drm_connector *connector;
    struct drm_crtc *crtc;
    struct drm_encoder *best_encoder;
    enum drm_link_status link_status;
    struct drm_atomic_state *state;
    struct drm_crtc_commit *commit;
    struct drm_tv_connector_state tv;
    bool self_refresh_aware;
    enum hdmi_picture_aspect picture_aspect_ratio;
    unsigned int content_type;
    unsigned int hdcp_content_type;
    unsigned int scaling_mode;
    unsigned int content_protection;
    u32 colorspace;
    struct drm_writeback_job *writeback_job;
    u8 max_requested_bpc;
    u8 max_bpc;
    struct drm_property_blob *hdr_output_metadata;
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
struct drm_connector_state {
    struct drm_connector *connector;
    struct drm_crtc *crtc;
    struct drm_encoder *best_encoder;
    enum drm_link_status link_status;
    struct drm_atomic_state *state;
    struct drm_crtc_commit *commit;
    struct drm_tv_connector_state tv;
    bool self_refresh_aware;
    enum hdmi_picture_aspect picture_aspect_ratio;
    unsigned int content_type;
    unsigned int hdcp_content_type;
    unsigned int scaling_mode;
    unsigned int content_protection;
    enum drm_colorspace colorspace;
    struct drm_writeback_job *writeback_job;
    u8 max_requested_bpc;
    u8 max_bpc;
    enum drm_privacy_screen_status privacy_screen_sw_state;
    struct drm_property_blob *hdr_output_metadata;
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
struct drm_connector_state {
    struct drm_connector *connector;
    struct drm_crtc *crtc;
    struct drm_encoder *best_encoder;
    enum drm_link_status link_status;
    struct drm_atomic_state *state;
    struct drm_crtc_commit *commit;
    struct drm_tv_connector_state tv;
    bool self_refresh_aware;
    enum hdmi_picture_aspect picture_aspect_ratio;
    unsigned int content_type;
    unsigned int hdcp_content_type;
    unsigned int scaling_mode;
    unsigned int content_protection;
    u32 colorspace;
    struct drm_writeback_job *writeback_job;
    u8 max_requested_bpc;
    u8 max_bpc;
    struct drm_property_blob *hdr_output_metadata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct drm_connector_state {
    struct drm_connector *connector;
    struct drm_crtc *crtc;
    struct drm_encoder *best_encoder;
    enum drm_link_status link_status;
    struct drm_atomic_state *state;
    struct drm_crtc_commit *commit;
    struct drm_tv_connector_state tv;
    bool self_refresh_aware;
    enum hdmi_picture_aspect picture_aspect_ratio;
    unsigned int content_type;
    unsigned int hdcp_content_type;
    unsigned int scaling_mode;
    unsigned int content_protection;
    u32 colorspace;
    struct drm_writeback_job *writeback_job;
    u8 max_requested_bpc;
    u8 max_bpc;
    struct drm_property_blob *hdr_output_metadata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct drm_connector_state {
    struct drm_connector *connector;
    struct drm_crtc *crtc;
    struct drm_encoder *best_encoder;
    enum drm_link_status link_status;
    struct drm_atomic_state *state;
    struct drm_crtc_commit *commit;
    struct drm_tv_connector_state tv;
    bool self_refresh_aware;
    enum hdmi_picture_aspect picture_aspect_ratio;
    unsigned int content_type;
    unsigned int hdcp_content_type;
    unsigned int scaling_mode;
    unsigned int content_protection;
    u32 colorspace;
    struct drm_writeback_job *writeback_job;
    u8 max_requested_bpc;
    u8 max_bpc;
    struct drm_property_blob *hdr_output_metadata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct drm_connector_state {
    struct drm_connector *connector;
    struct drm_crtc *crtc;
    struct drm_encoder *best_encoder;
    enum drm_link_status link_status;
    struct drm_atomic_state *state;
    struct drm_crtc_commit *commit;
    struct drm_tv_connector_state tv;
    bool self_refresh_aware;
    enum hdmi_picture_aspect picture_aspect_ratio;
    unsigned int content_type;
    unsigned int hdcp_content_type;
    unsigned int scaling_mode;
    unsigned int content_protection;
    u32 colorspace;
    struct drm_writeback_job *writeback_job;
    u8 max_requested_bpc;
    u8 max_bpc;
    struct drm_property_blob *hdr_output_metadata;
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
struct drm_connector_state {
    struct drm_connector *connector;
    struct drm_crtc *crtc;
    struct drm_encoder *best_encoder;
    enum drm_link_status link_status;
    struct drm_atomic_state *state;
    struct drm_crtc_commit *commit;
    struct drm_tv_connector_state tv;
    bool self_refresh_aware;
    enum hdmi_picture_aspect picture_aspect_ratio;
    unsigned int content_type;
    unsigned int hdcp_content_type;
    unsigned int scaling_mode;
    unsigned int content_protection;
    u32 colorspace;
    struct drm_writeback_job *writeback_job;
    u8 max_requested_bpc;
    u8 max_bpc;
    struct drm_property_blob *hdr_output_metadata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct drm_connector_state {
    struct drm_connector *connector;
    struct drm_crtc *crtc;
    struct drm_encoder *best_encoder;
    enum drm_link_status link_status;
    struct drm_atomic_state *state;
    struct drm_crtc_commit *commit;
    struct drm_tv_connector_state tv;
    bool self_refresh_aware;
    enum hdmi_picture_aspect picture_aspect_ratio;
    unsigned int content_type;
    unsigned int hdcp_content_type;
    unsigned int scaling_mode;
    unsigned int content_protection;
    u32 colorspace;
    struct drm_writeback_job *writeback_job;
    u8 max_requested_bpc;
    u8 max_bpc;
    struct drm_property_blob *hdr_output_metadata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct drm_connector_state {
    struct drm_connector *connector;
    struct drm_crtc *crtc;
    struct drm_encoder *best_encoder;
    enum drm_link_status link_status;
    struct drm_atomic_state *state;
    struct drm_crtc_commit *commit;
    struct drm_tv_connector_state tv;
    bool self_refresh_aware;
    enum hdmi_picture_aspect picture_aspect_ratio;
    unsigned int content_type;
    unsigned int hdcp_content_type;
    unsigned int scaling_mode;
    unsigned int content_protection;
    u32 colorspace;
    struct drm_writeback_job *writeback_job;
    u8 max_requested_bpc;
    u8 max_bpc;
    struct drm_property_blob *hdr_output_metadata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct drm_connector_state {
    struct drm_connector *connector;
    struct drm_crtc *crtc;
    struct drm_encoder *best_encoder;
    enum drm_link_status link_status;
    struct drm_atomic_state *state;
    struct drm_crtc_commit *commit;
    struct drm_tv_connector_state tv;
    bool self_refresh_aware;
    enum hdmi_picture_aspect picture_aspect_ratio;
    unsigned int content_type;
    unsigned int hdcp_content_type;
    unsigned int scaling_mode;
    unsigned int content_protection;
    u32 colorspace;
    struct drm_writeback_job *writeback_job;
    u8 max_requested_bpc;
    u8 max_bpc;
    struct drm_property_blob *hdr_output_metadata;
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
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int hdcp_content_type</code>
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
