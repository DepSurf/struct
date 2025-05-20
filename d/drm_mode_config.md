# Struct: <code>drm_mode_config</code>

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
struct drm_mode_config {
    struct mutex mutex;
    struct drm_modeset_lock connection_mutex;
    struct drm_modeset_acquire_ctx *acquire_ctx;
    struct mutex idr_mutex;
    struct idr object_idr;
    struct idr tile_idr;
    struct mutex fb_lock;
    int num_fb;
    struct list_head fb_list;
    spinlock_t connector_list_lock;
    int num_connector;
    struct ida connector_ida;
    struct list_head connector_list;
    struct llist_head connector_free_list;
    struct work_struct connector_free_work;
    int num_encoder;
    struct list_head encoder_list;
    int num_total_plane;
    struct list_head plane_list;
    int num_crtc;
    struct list_head crtc_list;
    struct list_head property_list;
    struct list_head privobj_list;
    int min_width;
    int min_height;
    int max_width;
    int max_height;
    const struct drm_mode_config_funcs *funcs;
    resource_size_t fb_base;
    bool poll_enabled;
    bool poll_running;
    bool delayed_event;
    struct delayed_work output_poll_work;
    struct mutex blob_lock;
    struct list_head property_blob_list;
    struct drm_property *edid_property;
    struct drm_property *dpms_property;
    struct drm_property *path_property;
    struct drm_property *tile_property;
    struct drm_property *link_status_property;
    struct drm_property *plane_type_property;
    struct drm_property *prop_src_x;
    struct drm_property *prop_src_y;
    struct drm_property *prop_src_w;
    struct drm_property *prop_src_h;
    struct drm_property *prop_crtc_x;
    struct drm_property *prop_crtc_y;
    struct drm_property *prop_crtc_w;
    struct drm_property *prop_crtc_h;
    struct drm_property *prop_fb_id;
    struct drm_property *prop_in_fence_fd;
    struct drm_property *prop_out_fence_ptr;
    struct drm_property *prop_crtc_id;
    struct drm_property *prop_fb_damage_clips;
    struct drm_property *prop_active;
    struct drm_property *prop_mode_id;
    struct drm_property *prop_vrr_enabled;
    struct drm_property *dvi_i_subconnector_property;
    struct drm_property *dvi_i_select_subconnector_property;
    struct drm_property *tv_subconnector_property;
    struct drm_property *tv_select_subconnector_property;
    struct drm_property *tv_mode_property;
    struct drm_property *tv_left_margin_property;
    struct drm_property *tv_right_margin_property;
    struct drm_property *tv_top_margin_property;
    struct drm_property *tv_bottom_margin_property;
    struct drm_property *tv_brightness_property;
    struct drm_property *tv_contrast_property;
    struct drm_property *tv_flicker_reduction_property;
    struct drm_property *tv_overscan_property;
    struct drm_property *tv_saturation_property;
    struct drm_property *tv_hue_property;
    struct drm_property *scaling_mode_property;
    struct drm_property *aspect_ratio_property;
    struct drm_property *content_type_property;
    struct drm_property *degamma_lut_property;
    struct drm_property *degamma_lut_size_property;
    struct drm_property *ctm_property;
    struct drm_property *gamma_lut_property;
    struct drm_property *gamma_lut_size_property;
    struct drm_property *suggested_x_property;
    struct drm_property *suggested_y_property;
    struct drm_property *non_desktop_property;
    struct drm_property *panel_orientation_property;
    struct drm_property *writeback_fb_id_property;
    struct drm_property *writeback_pixel_formats_property;
    struct drm_property *writeback_out_fence_ptr_property;
    struct drm_property *hdr_output_metadata_property;
    struct drm_property *content_protection_property;
    uint32_t preferred_depth;
    uint32_t prefer_shadow;
    bool prefer_shadow_fbdev;
    bool quirk_addfb_prefer_xbgr_30bpp;
    bool quirk_addfb_prefer_host_byte_order;
    bool async_page_flip;
    bool allow_fb_modifiers;
    bool normalize_zpos;
    struct drm_property *modifiers_property;
    uint32_t cursor_width;
    uint32_t cursor_height;
    struct drm_atomic_state *suspend_state;
    const struct drm_mode_config_helper_funcs *helper_private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct drm_mode_config {
    struct mutex mutex;
    struct drm_modeset_lock connection_mutex;
    struct drm_modeset_acquire_ctx *acquire_ctx;
    struct mutex idr_mutex;
    struct idr object_idr;
    struct idr tile_idr;
    struct mutex fb_lock;
    int num_fb;
    struct list_head fb_list;
    spinlock_t connector_list_lock;
    int num_connector;
    struct ida connector_ida;
    struct list_head connector_list;
    struct llist_head connector_free_list;
    struct work_struct connector_free_work;
    int num_encoder;
    struct list_head encoder_list;
    int num_total_plane;
    struct list_head plane_list;
    int num_crtc;
    struct list_head crtc_list;
    struct list_head property_list;
    struct list_head privobj_list;
    int min_width;
    int min_height;
    int max_width;
    int max_height;
    const struct drm_mode_config_funcs *funcs;
    resource_size_t fb_base;
    bool poll_enabled;
    bool poll_running;
    bool delayed_event;
    struct delayed_work output_poll_work;
    struct mutex blob_lock;
    struct list_head property_blob_list;
    struct drm_property *edid_property;
    struct drm_property *dpms_property;
    struct drm_property *path_property;
    struct drm_property *tile_property;
    struct drm_property *link_status_property;
    struct drm_property *plane_type_property;
    struct drm_property *prop_src_x;
    struct drm_property *prop_src_y;
    struct drm_property *prop_src_w;
    struct drm_property *prop_src_h;
    struct drm_property *prop_crtc_x;
    struct drm_property *prop_crtc_y;
    struct drm_property *prop_crtc_w;
    struct drm_property *prop_crtc_h;
    struct drm_property *prop_fb_id;
    struct drm_property *prop_in_fence_fd;
    struct drm_property *prop_out_fence_ptr;
    struct drm_property *prop_crtc_id;
    struct drm_property *prop_fb_damage_clips;
    struct drm_property *prop_active;
    struct drm_property *prop_mode_id;
    struct drm_property *prop_vrr_enabled;
    struct drm_property *dvi_i_subconnector_property;
    struct drm_property *dvi_i_select_subconnector_property;
    struct drm_property *tv_subconnector_property;
    struct drm_property *tv_select_subconnector_property;
    struct drm_property *tv_mode_property;
    struct drm_property *tv_left_margin_property;
    struct drm_property *tv_right_margin_property;
    struct drm_property *tv_top_margin_property;
    struct drm_property *tv_bottom_margin_property;
    struct drm_property *tv_brightness_property;
    struct drm_property *tv_contrast_property;
    struct drm_property *tv_flicker_reduction_property;
    struct drm_property *tv_overscan_property;
    struct drm_property *tv_saturation_property;
    struct drm_property *tv_hue_property;
    struct drm_property *scaling_mode_property;
    struct drm_property *aspect_ratio_property;
    struct drm_property *content_type_property;
    struct drm_property *degamma_lut_property;
    struct drm_property *degamma_lut_size_property;
    struct drm_property *ctm_property;
    struct drm_property *gamma_lut_property;
    struct drm_property *gamma_lut_size_property;
    struct drm_property *suggested_x_property;
    struct drm_property *suggested_y_property;
    struct drm_property *non_desktop_property;
    struct drm_property *panel_orientation_property;
    struct drm_property *writeback_fb_id_property;
    struct drm_property *writeback_pixel_formats_property;
    struct drm_property *writeback_out_fence_ptr_property;
    struct drm_property *hdr_output_metadata_property;
    struct drm_property *content_protection_property;
    struct drm_property *hdcp_content_type_property;
    uint32_t preferred_depth;
    uint32_t prefer_shadow;
    bool prefer_shadow_fbdev;
    bool quirk_addfb_prefer_xbgr_30bpp;
    bool quirk_addfb_prefer_host_byte_order;
    bool async_page_flip;
    bool allow_fb_modifiers;
    bool normalize_zpos;
    struct drm_property *modifiers_property;
    uint32_t cursor_width;
    uint32_t cursor_height;
    struct drm_atomic_state *suspend_state;
    const struct drm_mode_config_helper_funcs *helper_private;
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
struct drm_mode_config {
    struct mutex mutex;
    struct drm_modeset_lock connection_mutex;
    struct drm_modeset_acquire_ctx *acquire_ctx;
    struct mutex idr_mutex;
    struct idr object_idr;
    struct idr tile_idr;
    struct mutex fb_lock;
    int num_fb;
    struct list_head fb_list;
    spinlock_t connector_list_lock;
    int num_connector;
    struct ida connector_ida;
    struct list_head connector_list;
    struct llist_head connector_free_list;
    struct work_struct connector_free_work;
    int num_encoder;
    struct list_head encoder_list;
    int num_total_plane;
    struct list_head plane_list;
    int num_crtc;
    struct list_head crtc_list;
    struct list_head property_list;
    struct list_head privobj_list;
    int min_width;
    int min_height;
    int max_width;
    int max_height;
    const struct drm_mode_config_funcs *funcs;
    bool poll_enabled;
    bool poll_running;
    bool delayed_event;
    struct delayed_work output_poll_work;
    struct mutex blob_lock;
    struct list_head property_blob_list;
    struct drm_property *edid_property;
    struct drm_property *dpms_property;
    struct drm_property *path_property;
    struct drm_property *tile_property;
    struct drm_property *link_status_property;
    struct drm_property *plane_type_property;
    struct drm_property *prop_src_x;
    struct drm_property *prop_src_y;
    struct drm_property *prop_src_w;
    struct drm_property *prop_src_h;
    struct drm_property *prop_crtc_x;
    struct drm_property *prop_crtc_y;
    struct drm_property *prop_crtc_w;
    struct drm_property *prop_crtc_h;
    struct drm_property *prop_fb_id;
    struct drm_property *prop_in_fence_fd;
    struct drm_property *prop_out_fence_ptr;
    struct drm_property *prop_crtc_id;
    struct drm_property *prop_fb_damage_clips;
    struct drm_property *prop_active;
    struct drm_property *prop_mode_id;
    struct drm_property *prop_vrr_enabled;
    struct drm_property *dvi_i_subconnector_property;
    struct drm_property *dvi_i_select_subconnector_property;
    struct drm_property *dp_subconnector_property;
    struct drm_property *tv_subconnector_property;
    struct drm_property *tv_select_subconnector_property;
    struct drm_property *legacy_tv_mode_property;
    struct drm_property *tv_mode_property;
    struct drm_property *tv_left_margin_property;
    struct drm_property *tv_right_margin_property;
    struct drm_property *tv_top_margin_property;
    struct drm_property *tv_bottom_margin_property;
    struct drm_property *tv_brightness_property;
    struct drm_property *tv_contrast_property;
    struct drm_property *tv_flicker_reduction_property;
    struct drm_property *tv_overscan_property;
    struct drm_property *tv_saturation_property;
    struct drm_property *tv_hue_property;
    struct drm_property *scaling_mode_property;
    struct drm_property *aspect_ratio_property;
    struct drm_property *content_type_property;
    struct drm_property *degamma_lut_property;
    struct drm_property *degamma_lut_size_property;
    struct drm_property *ctm_property;
    struct drm_property *gamma_lut_property;
    struct drm_property *gamma_lut_size_property;
    struct drm_property *suggested_x_property;
    struct drm_property *suggested_y_property;
    struct drm_property *non_desktop_property;
    struct drm_property *panel_orientation_property;
    struct drm_property *writeback_fb_id_property;
    struct drm_property *writeback_pixel_formats_property;
    struct drm_property *writeback_out_fence_ptr_property;
    struct drm_property *hdr_output_metadata_property;
    struct drm_property *content_protection_property;
    struct drm_property *hdcp_content_type_property;
    uint32_t preferred_depth;
    uint32_t prefer_shadow;
    bool quirk_addfb_prefer_xbgr_30bpp;
    bool quirk_addfb_prefer_host_byte_order;
    bool async_page_flip;
    bool fb_modifiers_not_supported;
    bool normalize_zpos;
    struct drm_property *modifiers_property;
    uint32_t cursor_width;
    uint32_t cursor_height;
    struct drm_atomic_state *suspend_state;
    const struct drm_mode_config_helper_funcs *helper_private;
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
struct drm_mode_config {
    struct mutex mutex;
    struct drm_modeset_lock connection_mutex;
    struct drm_modeset_acquire_ctx *acquire_ctx;
    struct mutex idr_mutex;
    struct idr object_idr;
    struct idr tile_idr;
    struct mutex fb_lock;
    int num_fb;
    struct list_head fb_list;
    spinlock_t connector_list_lock;
    int num_connector;
    struct ida connector_ida;
    struct list_head connector_list;
    struct llist_head connector_free_list;
    struct work_struct connector_free_work;
    int num_encoder;
    struct list_head encoder_list;
    int num_total_plane;
    struct list_head plane_list;
    int num_crtc;
    struct list_head crtc_list;
    struct list_head property_list;
    struct list_head privobj_list;
    int min_width;
    int min_height;
    int max_width;
    int max_height;
    const struct drm_mode_config_funcs *funcs;
    resource_size_t fb_base;
    bool poll_enabled;
    bool poll_running;
    bool delayed_event;
    struct delayed_work output_poll_work;
    struct mutex blob_lock;
    struct list_head property_blob_list;
    struct drm_property *edid_property;
    struct drm_property *dpms_property;
    struct drm_property *path_property;
    struct drm_property *tile_property;
    struct drm_property *link_status_property;
    struct drm_property *plane_type_property;
    struct drm_property *prop_src_x;
    struct drm_property *prop_src_y;
    struct drm_property *prop_src_w;
    struct drm_property *prop_src_h;
    struct drm_property *prop_crtc_x;
    struct drm_property *prop_crtc_y;
    struct drm_property *prop_crtc_w;
    struct drm_property *prop_crtc_h;
    struct drm_property *prop_fb_id;
    struct drm_property *prop_in_fence_fd;
    struct drm_property *prop_out_fence_ptr;
    struct drm_property *prop_crtc_id;
    struct drm_property *prop_fb_damage_clips;
    struct drm_property *prop_active;
    struct drm_property *prop_mode_id;
    struct drm_property *prop_vrr_enabled;
    struct drm_property *dvi_i_subconnector_property;
    struct drm_property *dvi_i_select_subconnector_property;
    struct drm_property *tv_subconnector_property;
    struct drm_property *tv_select_subconnector_property;
    struct drm_property *tv_mode_property;
    struct drm_property *tv_left_margin_property;
    struct drm_property *tv_right_margin_property;
    struct drm_property *tv_top_margin_property;
    struct drm_property *tv_bottom_margin_property;
    struct drm_property *tv_brightness_property;
    struct drm_property *tv_contrast_property;
    struct drm_property *tv_flicker_reduction_property;
    struct drm_property *tv_overscan_property;
    struct drm_property *tv_saturation_property;
    struct drm_property *tv_hue_property;
    struct drm_property *scaling_mode_property;
    struct drm_property *aspect_ratio_property;
    struct drm_property *content_type_property;
    struct drm_property *degamma_lut_property;
    struct drm_property *degamma_lut_size_property;
    struct drm_property *ctm_property;
    struct drm_property *gamma_lut_property;
    struct drm_property *gamma_lut_size_property;
    struct drm_property *suggested_x_property;
    struct drm_property *suggested_y_property;
    struct drm_property *non_desktop_property;
    struct drm_property *panel_orientation_property;
    struct drm_property *writeback_fb_id_property;
    struct drm_property *writeback_pixel_formats_property;
    struct drm_property *writeback_out_fence_ptr_property;
    struct drm_property *hdr_output_metadata_property;
    struct drm_property *content_protection_property;
    struct drm_property *hdcp_content_type_property;
    uint32_t preferred_depth;
    uint32_t prefer_shadow;
    bool prefer_shadow_fbdev;
    bool quirk_addfb_prefer_xbgr_30bpp;
    bool quirk_addfb_prefer_host_byte_order;
    bool async_page_flip;
    bool allow_fb_modifiers;
    bool normalize_zpos;
    struct drm_property *modifiers_property;
    uint32_t cursor_width;
    uint32_t cursor_height;
    struct drm_atomic_state *suspend_state;
    const struct drm_mode_config_helper_funcs *helper_private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct drm_mode_config {
    struct mutex mutex;
    struct drm_modeset_lock connection_mutex;
    struct drm_modeset_acquire_ctx *acquire_ctx;
    struct mutex idr_mutex;
    struct idr object_idr;
    struct idr tile_idr;
    struct mutex fb_lock;
    int num_fb;
    struct list_head fb_list;
    spinlock_t connector_list_lock;
    int num_connector;
    struct ida connector_ida;
    struct list_head connector_list;
    struct llist_head connector_free_list;
    struct work_struct connector_free_work;
    int num_encoder;
    struct list_head encoder_list;
    int num_total_plane;
    struct list_head plane_list;
    int num_crtc;
    struct list_head crtc_list;
    struct list_head property_list;
    struct list_head privobj_list;
    int min_width;
    int min_height;
    int max_width;
    int max_height;
    const struct drm_mode_config_funcs *funcs;
    resource_size_t fb_base;
    bool poll_enabled;
    bool poll_running;
    bool delayed_event;
    struct delayed_work output_poll_work;
    struct mutex blob_lock;
    struct list_head property_blob_list;
    struct drm_property *edid_property;
    struct drm_property *dpms_property;
    struct drm_property *path_property;
    struct drm_property *tile_property;
    struct drm_property *link_status_property;
    struct drm_property *plane_type_property;
    struct drm_property *prop_src_x;
    struct drm_property *prop_src_y;
    struct drm_property *prop_src_w;
    struct drm_property *prop_src_h;
    struct drm_property *prop_crtc_x;
    struct drm_property *prop_crtc_y;
    struct drm_property *prop_crtc_w;
    struct drm_property *prop_crtc_h;
    struct drm_property *prop_fb_id;
    struct drm_property *prop_in_fence_fd;
    struct drm_property *prop_out_fence_ptr;
    struct drm_property *prop_crtc_id;
    struct drm_property *prop_fb_damage_clips;
    struct drm_property *prop_active;
    struct drm_property *prop_mode_id;
    struct drm_property *prop_vrr_enabled;
    struct drm_property *dvi_i_subconnector_property;
    struct drm_property *dvi_i_select_subconnector_property;
    struct drm_property *tv_subconnector_property;
    struct drm_property *tv_select_subconnector_property;
    struct drm_property *tv_mode_property;
    struct drm_property *tv_left_margin_property;
    struct drm_property *tv_right_margin_property;
    struct drm_property *tv_top_margin_property;
    struct drm_property *tv_bottom_margin_property;
    struct drm_property *tv_brightness_property;
    struct drm_property *tv_contrast_property;
    struct drm_property *tv_flicker_reduction_property;
    struct drm_property *tv_overscan_property;
    struct drm_property *tv_saturation_property;
    struct drm_property *tv_hue_property;
    struct drm_property *scaling_mode_property;
    struct drm_property *aspect_ratio_property;
    struct drm_property *content_type_property;
    struct drm_property *degamma_lut_property;
    struct drm_property *degamma_lut_size_property;
    struct drm_property *ctm_property;
    struct drm_property *gamma_lut_property;
    struct drm_property *gamma_lut_size_property;
    struct drm_property *suggested_x_property;
    struct drm_property *suggested_y_property;
    struct drm_property *non_desktop_property;
    struct drm_property *panel_orientation_property;
    struct drm_property *writeback_fb_id_property;
    struct drm_property *writeback_pixel_formats_property;
    struct drm_property *writeback_out_fence_ptr_property;
    struct drm_property *hdr_output_metadata_property;
    struct drm_property *content_protection_property;
    struct drm_property *hdcp_content_type_property;
    uint32_t preferred_depth;
    uint32_t prefer_shadow;
    bool prefer_shadow_fbdev;
    bool quirk_addfb_prefer_xbgr_30bpp;
    bool quirk_addfb_prefer_host_byte_order;
    bool async_page_flip;
    bool allow_fb_modifiers;
    bool normalize_zpos;
    struct drm_property *modifiers_property;
    uint32_t cursor_width;
    uint32_t cursor_height;
    struct drm_atomic_state *suspend_state;
    const struct drm_mode_config_helper_funcs *helper_private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct drm_mode_config {
    struct mutex mutex;
    struct drm_modeset_lock connection_mutex;
    struct drm_modeset_acquire_ctx *acquire_ctx;
    struct mutex idr_mutex;
    struct idr object_idr;
    struct idr tile_idr;
    struct mutex fb_lock;
    int num_fb;
    struct list_head fb_list;
    spinlock_t connector_list_lock;
    int num_connector;
    struct ida connector_ida;
    struct list_head connector_list;
    struct llist_head connector_free_list;
    struct work_struct connector_free_work;
    int num_encoder;
    struct list_head encoder_list;
    int num_total_plane;
    struct list_head plane_list;
    int num_crtc;
    struct list_head crtc_list;
    struct list_head property_list;
    struct list_head privobj_list;
    int min_width;
    int min_height;
    int max_width;
    int max_height;
    const struct drm_mode_config_funcs *funcs;
    resource_size_t fb_base;
    bool poll_enabled;
    bool poll_running;
    bool delayed_event;
    struct delayed_work output_poll_work;
    struct mutex blob_lock;
    struct list_head property_blob_list;
    struct drm_property *edid_property;
    struct drm_property *dpms_property;
    struct drm_property *path_property;
    struct drm_property *tile_property;
    struct drm_property *link_status_property;
    struct drm_property *plane_type_property;
    struct drm_property *prop_src_x;
    struct drm_property *prop_src_y;
    struct drm_property *prop_src_w;
    struct drm_property *prop_src_h;
    struct drm_property *prop_crtc_x;
    struct drm_property *prop_crtc_y;
    struct drm_property *prop_crtc_w;
    struct drm_property *prop_crtc_h;
    struct drm_property *prop_fb_id;
    struct drm_property *prop_in_fence_fd;
    struct drm_property *prop_out_fence_ptr;
    struct drm_property *prop_crtc_id;
    struct drm_property *prop_fb_damage_clips;
    struct drm_property *prop_active;
    struct drm_property *prop_mode_id;
    struct drm_property *prop_vrr_enabled;
    struct drm_property *dvi_i_subconnector_property;
    struct drm_property *dvi_i_select_subconnector_property;
    struct drm_property *tv_subconnector_property;
    struct drm_property *tv_select_subconnector_property;
    struct drm_property *tv_mode_property;
    struct drm_property *tv_left_margin_property;
    struct drm_property *tv_right_margin_property;
    struct drm_property *tv_top_margin_property;
    struct drm_property *tv_bottom_margin_property;
    struct drm_property *tv_brightness_property;
    struct drm_property *tv_contrast_property;
    struct drm_property *tv_flicker_reduction_property;
    struct drm_property *tv_overscan_property;
    struct drm_property *tv_saturation_property;
    struct drm_property *tv_hue_property;
    struct drm_property *scaling_mode_property;
    struct drm_property *aspect_ratio_property;
    struct drm_property *content_type_property;
    struct drm_property *degamma_lut_property;
    struct drm_property *degamma_lut_size_property;
    struct drm_property *ctm_property;
    struct drm_property *gamma_lut_property;
    struct drm_property *gamma_lut_size_property;
    struct drm_property *suggested_x_property;
    struct drm_property *suggested_y_property;
    struct drm_property *non_desktop_property;
    struct drm_property *panel_orientation_property;
    struct drm_property *writeback_fb_id_property;
    struct drm_property *writeback_pixel_formats_property;
    struct drm_property *writeback_out_fence_ptr_property;
    struct drm_property *hdr_output_metadata_property;
    struct drm_property *content_protection_property;
    struct drm_property *hdcp_content_type_property;
    uint32_t preferred_depth;
    uint32_t prefer_shadow;
    bool prefer_shadow_fbdev;
    bool quirk_addfb_prefer_xbgr_30bpp;
    bool quirk_addfb_prefer_host_byte_order;
    bool async_page_flip;
    bool allow_fb_modifiers;
    bool normalize_zpos;
    struct drm_property *modifiers_property;
    uint32_t cursor_width;
    uint32_t cursor_height;
    struct drm_atomic_state *suspend_state;
    const struct drm_mode_config_helper_funcs *helper_private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct drm_mode_config {
    struct mutex mutex;
    struct drm_modeset_lock connection_mutex;
    struct drm_modeset_acquire_ctx *acquire_ctx;
    struct mutex idr_mutex;
    struct idr object_idr;
    struct idr tile_idr;
    struct mutex fb_lock;
    int num_fb;
    struct list_head fb_list;
    spinlock_t connector_list_lock;
    int num_connector;
    struct ida connector_ida;
    struct list_head connector_list;
    struct llist_head connector_free_list;
    struct work_struct connector_free_work;
    int num_encoder;
    struct list_head encoder_list;
    int num_total_plane;
    struct list_head plane_list;
    int num_crtc;
    struct list_head crtc_list;
    struct list_head property_list;
    struct list_head privobj_list;
    int min_width;
    int min_height;
    int max_width;
    int max_height;
    const struct drm_mode_config_funcs *funcs;
    resource_size_t fb_base;
    bool poll_enabled;
    bool poll_running;
    bool delayed_event;
    struct delayed_work output_poll_work;
    struct mutex blob_lock;
    struct list_head property_blob_list;
    struct drm_property *edid_property;
    struct drm_property *dpms_property;
    struct drm_property *path_property;
    struct drm_property *tile_property;
    struct drm_property *link_status_property;
    struct drm_property *plane_type_property;
    struct drm_property *prop_src_x;
    struct drm_property *prop_src_y;
    struct drm_property *prop_src_w;
    struct drm_property *prop_src_h;
    struct drm_property *prop_crtc_x;
    struct drm_property *prop_crtc_y;
    struct drm_property *prop_crtc_w;
    struct drm_property *prop_crtc_h;
    struct drm_property *prop_fb_id;
    struct drm_property *prop_in_fence_fd;
    struct drm_property *prop_out_fence_ptr;
    struct drm_property *prop_crtc_id;
    struct drm_property *prop_fb_damage_clips;
    struct drm_property *prop_active;
    struct drm_property *prop_mode_id;
    struct drm_property *prop_vrr_enabled;
    struct drm_property *dvi_i_subconnector_property;
    struct drm_property *dvi_i_select_subconnector_property;
    struct drm_property *tv_subconnector_property;
    struct drm_property *tv_select_subconnector_property;
    struct drm_property *tv_mode_property;
    struct drm_property *tv_left_margin_property;
    struct drm_property *tv_right_margin_property;
    struct drm_property *tv_top_margin_property;
    struct drm_property *tv_bottom_margin_property;
    struct drm_property *tv_brightness_property;
    struct drm_property *tv_contrast_property;
    struct drm_property *tv_flicker_reduction_property;
    struct drm_property *tv_overscan_property;
    struct drm_property *tv_saturation_property;
    struct drm_property *tv_hue_property;
    struct drm_property *scaling_mode_property;
    struct drm_property *aspect_ratio_property;
    struct drm_property *content_type_property;
    struct drm_property *degamma_lut_property;
    struct drm_property *degamma_lut_size_property;
    struct drm_property *ctm_property;
    struct drm_property *gamma_lut_property;
    struct drm_property *gamma_lut_size_property;
    struct drm_property *suggested_x_property;
    struct drm_property *suggested_y_property;
    struct drm_property *non_desktop_property;
    struct drm_property *panel_orientation_property;
    struct drm_property *writeback_fb_id_property;
    struct drm_property *writeback_pixel_formats_property;
    struct drm_property *writeback_out_fence_ptr_property;
    struct drm_property *hdr_output_metadata_property;
    struct drm_property *content_protection_property;
    struct drm_property *hdcp_content_type_property;
    uint32_t preferred_depth;
    uint32_t prefer_shadow;
    bool prefer_shadow_fbdev;
    bool quirk_addfb_prefer_xbgr_30bpp;
    bool quirk_addfb_prefer_host_byte_order;
    bool async_page_flip;
    bool allow_fb_modifiers;
    bool normalize_zpos;
    struct drm_property *modifiers_property;
    uint32_t cursor_width;
    uint32_t cursor_height;
    struct drm_atomic_state *suspend_state;
    const struct drm_mode_config_helper_funcs *helper_private;
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
struct drm_mode_config {
    struct mutex mutex;
    struct drm_modeset_lock connection_mutex;
    struct drm_modeset_acquire_ctx *acquire_ctx;
    struct mutex idr_mutex;
    struct idr object_idr;
    struct idr tile_idr;
    struct mutex fb_lock;
    int num_fb;
    struct list_head fb_list;
    spinlock_t connector_list_lock;
    int num_connector;
    struct ida connector_ida;
    struct list_head connector_list;
    struct llist_head connector_free_list;
    struct work_struct connector_free_work;
    int num_encoder;
    struct list_head encoder_list;
    int num_total_plane;
    struct list_head plane_list;
    int num_crtc;
    struct list_head crtc_list;
    struct list_head property_list;
    struct list_head privobj_list;
    int min_width;
    int min_height;
    int max_width;
    int max_height;
    const struct drm_mode_config_funcs *funcs;
    resource_size_t fb_base;
    bool poll_enabled;
    bool poll_running;
    bool delayed_event;
    struct delayed_work output_poll_work;
    struct mutex blob_lock;
    struct list_head property_blob_list;
    struct drm_property *edid_property;
    struct drm_property *dpms_property;
    struct drm_property *path_property;
    struct drm_property *tile_property;
    struct drm_property *link_status_property;
    struct drm_property *plane_type_property;
    struct drm_property *prop_src_x;
    struct drm_property *prop_src_y;
    struct drm_property *prop_src_w;
    struct drm_property *prop_src_h;
    struct drm_property *prop_crtc_x;
    struct drm_property *prop_crtc_y;
    struct drm_property *prop_crtc_w;
    struct drm_property *prop_crtc_h;
    struct drm_property *prop_fb_id;
    struct drm_property *prop_in_fence_fd;
    struct drm_property *prop_out_fence_ptr;
    struct drm_property *prop_crtc_id;
    struct drm_property *prop_fb_damage_clips;
    struct drm_property *prop_active;
    struct drm_property *prop_mode_id;
    struct drm_property *prop_vrr_enabled;
    struct drm_property *dvi_i_subconnector_property;
    struct drm_property *dvi_i_select_subconnector_property;
    struct drm_property *tv_subconnector_property;
    struct drm_property *tv_select_subconnector_property;
    struct drm_property *tv_mode_property;
    struct drm_property *tv_left_margin_property;
    struct drm_property *tv_right_margin_property;
    struct drm_property *tv_top_margin_property;
    struct drm_property *tv_bottom_margin_property;
    struct drm_property *tv_brightness_property;
    struct drm_property *tv_contrast_property;
    struct drm_property *tv_flicker_reduction_property;
    struct drm_property *tv_overscan_property;
    struct drm_property *tv_saturation_property;
    struct drm_property *tv_hue_property;
    struct drm_property *scaling_mode_property;
    struct drm_property *aspect_ratio_property;
    struct drm_property *content_type_property;
    struct drm_property *degamma_lut_property;
    struct drm_property *degamma_lut_size_property;
    struct drm_property *ctm_property;
    struct drm_property *gamma_lut_property;
    struct drm_property *gamma_lut_size_property;
    struct drm_property *suggested_x_property;
    struct drm_property *suggested_y_property;
    struct drm_property *non_desktop_property;
    struct drm_property *panel_orientation_property;
    struct drm_property *writeback_fb_id_property;
    struct drm_property *writeback_pixel_formats_property;
    struct drm_property *writeback_out_fence_ptr_property;
    struct drm_property *hdr_output_metadata_property;
    struct drm_property *content_protection_property;
    struct drm_property *hdcp_content_type_property;
    uint32_t preferred_depth;
    uint32_t prefer_shadow;
    bool prefer_shadow_fbdev;
    bool quirk_addfb_prefer_xbgr_30bpp;
    bool quirk_addfb_prefer_host_byte_order;
    bool async_page_flip;
    bool allow_fb_modifiers;
    bool normalize_zpos;
    struct drm_property *modifiers_property;
    uint32_t cursor_width;
    uint32_t cursor_height;
    struct drm_atomic_state *suspend_state;
    const struct drm_mode_config_helper_funcs *helper_private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct drm_mode_config {
    struct mutex mutex;
    struct drm_modeset_lock connection_mutex;
    struct drm_modeset_acquire_ctx *acquire_ctx;
    struct mutex idr_mutex;
    struct idr object_idr;
    struct idr tile_idr;
    struct mutex fb_lock;
    int num_fb;
    struct list_head fb_list;
    spinlock_t connector_list_lock;
    int num_connector;
    struct ida connector_ida;
    struct list_head connector_list;
    struct llist_head connector_free_list;
    struct work_struct connector_free_work;
    int num_encoder;
    struct list_head encoder_list;
    int num_total_plane;
    struct list_head plane_list;
    int num_crtc;
    struct list_head crtc_list;
    struct list_head property_list;
    struct list_head privobj_list;
    int min_width;
    int min_height;
    int max_width;
    int max_height;
    const struct drm_mode_config_funcs *funcs;
    resource_size_t fb_base;
    bool poll_enabled;
    bool poll_running;
    bool delayed_event;
    struct delayed_work output_poll_work;
    struct mutex blob_lock;
    struct list_head property_blob_list;
    struct drm_property *edid_property;
    struct drm_property *dpms_property;
    struct drm_property *path_property;
    struct drm_property *tile_property;
    struct drm_property *link_status_property;
    struct drm_property *plane_type_property;
    struct drm_property *prop_src_x;
    struct drm_property *prop_src_y;
    struct drm_property *prop_src_w;
    struct drm_property *prop_src_h;
    struct drm_property *prop_crtc_x;
    struct drm_property *prop_crtc_y;
    struct drm_property *prop_crtc_w;
    struct drm_property *prop_crtc_h;
    struct drm_property *prop_fb_id;
    struct drm_property *prop_in_fence_fd;
    struct drm_property *prop_out_fence_ptr;
    struct drm_property *prop_crtc_id;
    struct drm_property *prop_fb_damage_clips;
    struct drm_property *prop_active;
    struct drm_property *prop_mode_id;
    struct drm_property *prop_vrr_enabled;
    struct drm_property *dvi_i_subconnector_property;
    struct drm_property *dvi_i_select_subconnector_property;
    struct drm_property *tv_subconnector_property;
    struct drm_property *tv_select_subconnector_property;
    struct drm_property *tv_mode_property;
    struct drm_property *tv_left_margin_property;
    struct drm_property *tv_right_margin_property;
    struct drm_property *tv_top_margin_property;
    struct drm_property *tv_bottom_margin_property;
    struct drm_property *tv_brightness_property;
    struct drm_property *tv_contrast_property;
    struct drm_property *tv_flicker_reduction_property;
    struct drm_property *tv_overscan_property;
    struct drm_property *tv_saturation_property;
    struct drm_property *tv_hue_property;
    struct drm_property *scaling_mode_property;
    struct drm_property *aspect_ratio_property;
    struct drm_property *content_type_property;
    struct drm_property *degamma_lut_property;
    struct drm_property *degamma_lut_size_property;
    struct drm_property *ctm_property;
    struct drm_property *gamma_lut_property;
    struct drm_property *gamma_lut_size_property;
    struct drm_property *suggested_x_property;
    struct drm_property *suggested_y_property;
    struct drm_property *non_desktop_property;
    struct drm_property *panel_orientation_property;
    struct drm_property *writeback_fb_id_property;
    struct drm_property *writeback_pixel_formats_property;
    struct drm_property *writeback_out_fence_ptr_property;
    struct drm_property *hdr_output_metadata_property;
    struct drm_property *content_protection_property;
    struct drm_property *hdcp_content_type_property;
    uint32_t preferred_depth;
    uint32_t prefer_shadow;
    bool prefer_shadow_fbdev;
    bool quirk_addfb_prefer_xbgr_30bpp;
    bool quirk_addfb_prefer_host_byte_order;
    bool async_page_flip;
    bool allow_fb_modifiers;
    bool normalize_zpos;
    struct drm_property *modifiers_property;
    uint32_t cursor_width;
    uint32_t cursor_height;
    struct drm_atomic_state *suspend_state;
    const struct drm_mode_config_helper_funcs *helper_private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct drm_mode_config {
    struct mutex mutex;
    struct drm_modeset_lock connection_mutex;
    struct drm_modeset_acquire_ctx *acquire_ctx;
    struct mutex idr_mutex;
    struct idr object_idr;
    struct idr tile_idr;
    struct mutex fb_lock;
    int num_fb;
    struct list_head fb_list;
    spinlock_t connector_list_lock;
    int num_connector;
    struct ida connector_ida;
    struct list_head connector_list;
    struct llist_head connector_free_list;
    struct work_struct connector_free_work;
    int num_encoder;
    struct list_head encoder_list;
    int num_total_plane;
    struct list_head plane_list;
    int num_crtc;
    struct list_head crtc_list;
    struct list_head property_list;
    struct list_head privobj_list;
    int min_width;
    int min_height;
    int max_width;
    int max_height;
    const struct drm_mode_config_funcs *funcs;
    resource_size_t fb_base;
    bool poll_enabled;
    bool poll_running;
    bool delayed_event;
    struct delayed_work output_poll_work;
    struct mutex blob_lock;
    struct list_head property_blob_list;
    struct drm_property *edid_property;
    struct drm_property *dpms_property;
    struct drm_property *path_property;
    struct drm_property *tile_property;
    struct drm_property *link_status_property;
    struct drm_property *plane_type_property;
    struct drm_property *prop_src_x;
    struct drm_property *prop_src_y;
    struct drm_property *prop_src_w;
    struct drm_property *prop_src_h;
    struct drm_property *prop_crtc_x;
    struct drm_property *prop_crtc_y;
    struct drm_property *prop_crtc_w;
    struct drm_property *prop_crtc_h;
    struct drm_property *prop_fb_id;
    struct drm_property *prop_in_fence_fd;
    struct drm_property *prop_out_fence_ptr;
    struct drm_property *prop_crtc_id;
    struct drm_property *prop_fb_damage_clips;
    struct drm_property *prop_active;
    struct drm_property *prop_mode_id;
    struct drm_property *prop_vrr_enabled;
    struct drm_property *dvi_i_subconnector_property;
    struct drm_property *dvi_i_select_subconnector_property;
    struct drm_property *tv_subconnector_property;
    struct drm_property *tv_select_subconnector_property;
    struct drm_property *tv_mode_property;
    struct drm_property *tv_left_margin_property;
    struct drm_property *tv_right_margin_property;
    struct drm_property *tv_top_margin_property;
    struct drm_property *tv_bottom_margin_property;
    struct drm_property *tv_brightness_property;
    struct drm_property *tv_contrast_property;
    struct drm_property *tv_flicker_reduction_property;
    struct drm_property *tv_overscan_property;
    struct drm_property *tv_saturation_property;
    struct drm_property *tv_hue_property;
    struct drm_property *scaling_mode_property;
    struct drm_property *aspect_ratio_property;
    struct drm_property *content_type_property;
    struct drm_property *degamma_lut_property;
    struct drm_property *degamma_lut_size_property;
    struct drm_property *ctm_property;
    struct drm_property *gamma_lut_property;
    struct drm_property *gamma_lut_size_property;
    struct drm_property *suggested_x_property;
    struct drm_property *suggested_y_property;
    struct drm_property *non_desktop_property;
    struct drm_property *panel_orientation_property;
    struct drm_property *writeback_fb_id_property;
    struct drm_property *writeback_pixel_formats_property;
    struct drm_property *writeback_out_fence_ptr_property;
    struct drm_property *hdr_output_metadata_property;
    struct drm_property *content_protection_property;
    struct drm_property *hdcp_content_type_property;
    uint32_t preferred_depth;
    uint32_t prefer_shadow;
    bool prefer_shadow_fbdev;
    bool quirk_addfb_prefer_xbgr_30bpp;
    bool quirk_addfb_prefer_host_byte_order;
    bool async_page_flip;
    bool allow_fb_modifiers;
    bool normalize_zpos;
    struct drm_property *modifiers_property;
    uint32_t cursor_width;
    uint32_t cursor_height;
    struct drm_atomic_state *suspend_state;
    const struct drm_mode_config_helper_funcs *helper_private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct drm_mode_config {
    struct mutex mutex;
    struct drm_modeset_lock connection_mutex;
    struct drm_modeset_acquire_ctx *acquire_ctx;
    struct mutex idr_mutex;
    struct idr object_idr;
    struct idr tile_idr;
    struct mutex fb_lock;
    int num_fb;
    struct list_head fb_list;
    spinlock_t connector_list_lock;
    int num_connector;
    struct ida connector_ida;
    struct list_head connector_list;
    struct llist_head connector_free_list;
    struct work_struct connector_free_work;
    int num_encoder;
    struct list_head encoder_list;
    int num_total_plane;
    struct list_head plane_list;
    int num_crtc;
    struct list_head crtc_list;
    struct list_head property_list;
    struct list_head privobj_list;
    int min_width;
    int min_height;
    int max_width;
    int max_height;
    const struct drm_mode_config_funcs *funcs;
    resource_size_t fb_base;
    bool poll_enabled;
    bool poll_running;
    bool delayed_event;
    struct delayed_work output_poll_work;
    struct mutex blob_lock;
    struct list_head property_blob_list;
    struct drm_property *edid_property;
    struct drm_property *dpms_property;
    struct drm_property *path_property;
    struct drm_property *tile_property;
    struct drm_property *link_status_property;
    struct drm_property *plane_type_property;
    struct drm_property *prop_src_x;
    struct drm_property *prop_src_y;
    struct drm_property *prop_src_w;
    struct drm_property *prop_src_h;
    struct drm_property *prop_crtc_x;
    struct drm_property *prop_crtc_y;
    struct drm_property *prop_crtc_w;
    struct drm_property *prop_crtc_h;
    struct drm_property *prop_fb_id;
    struct drm_property *prop_in_fence_fd;
    struct drm_property *prop_out_fence_ptr;
    struct drm_property *prop_crtc_id;
    struct drm_property *prop_fb_damage_clips;
    struct drm_property *prop_active;
    struct drm_property *prop_mode_id;
    struct drm_property *prop_vrr_enabled;
    struct drm_property *dvi_i_subconnector_property;
    struct drm_property *dvi_i_select_subconnector_property;
    struct drm_property *tv_subconnector_property;
    struct drm_property *tv_select_subconnector_property;
    struct drm_property *tv_mode_property;
    struct drm_property *tv_left_margin_property;
    struct drm_property *tv_right_margin_property;
    struct drm_property *tv_top_margin_property;
    struct drm_property *tv_bottom_margin_property;
    struct drm_property *tv_brightness_property;
    struct drm_property *tv_contrast_property;
    struct drm_property *tv_flicker_reduction_property;
    struct drm_property *tv_overscan_property;
    struct drm_property *tv_saturation_property;
    struct drm_property *tv_hue_property;
    struct drm_property *scaling_mode_property;
    struct drm_property *aspect_ratio_property;
    struct drm_property *content_type_property;
    struct drm_property *degamma_lut_property;
    struct drm_property *degamma_lut_size_property;
    struct drm_property *ctm_property;
    struct drm_property *gamma_lut_property;
    struct drm_property *gamma_lut_size_property;
    struct drm_property *suggested_x_property;
    struct drm_property *suggested_y_property;
    struct drm_property *non_desktop_property;
    struct drm_property *panel_orientation_property;
    struct drm_property *writeback_fb_id_property;
    struct drm_property *writeback_pixel_formats_property;
    struct drm_property *writeback_out_fence_ptr_property;
    struct drm_property *hdr_output_metadata_property;
    struct drm_property *content_protection_property;
    struct drm_property *hdcp_content_type_property;
    uint32_t preferred_depth;
    uint32_t prefer_shadow;
    bool prefer_shadow_fbdev;
    bool quirk_addfb_prefer_xbgr_30bpp;
    bool quirk_addfb_prefer_host_byte_order;
    bool async_page_flip;
    bool allow_fb_modifiers;
    bool normalize_zpos;
    struct drm_property *modifiers_property;
    uint32_t cursor_width;
    uint32_t cursor_height;
    struct drm_atomic_state *suspend_state;
    const struct drm_mode_config_helper_funcs *helper_private;
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
<code>struct drm_property *hdcp_content_type_property</code>
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
