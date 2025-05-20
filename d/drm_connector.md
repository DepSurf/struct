# Struct: <code>drm_connector</code>

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
struct drm_connector {
    struct drm_device *dev;
    struct device *kdev;
    struct device_attribute *attr;
    struct list_head head;
    struct drm_mode_object base;
    char *name;
    struct mutex mutex;
    unsigned int index;
    int connector_type;
    int connector_type_id;
    bool interlace_allowed;
    bool doublescan_allowed;
    bool stereo_allowed;
    bool ycbcr_420_allowed;
    enum drm_connector_registration_state registration_state;
    struct list_head modes;
    enum drm_connector_status status;
    struct list_head probed_modes;
    struct drm_display_info display_info;
    const struct drm_connector_funcs *funcs;
    struct drm_property_blob *edid_blob_ptr;
    struct drm_object_properties properties;
    struct drm_property *scaling_mode_property;
    struct drm_property *vrr_capable_property;
    struct drm_property *colorspace_property;
    struct drm_property_blob *path_blob_ptr;
    struct drm_property *max_bpc_property;
    uint8_t polled;
    int dpms;
    const struct drm_connector_helper_funcs *helper_private;
    struct drm_cmdline_mode cmdline_mode;
    enum drm_connector_force force;
    bool override_edid;
    uint32_t encoder_ids[3];
    struct drm_encoder *encoder;
    uint8_t eld[128];
    bool latency_present[2];
    int video_latency[2];
    int audio_latency[2];
    int null_edid_counter;
    unsigned int bad_edid_counter;
    bool edid_corrupt;
    struct dentry *debugfs_entry;
    struct drm_connector_state *state;
    struct drm_property_blob *tile_blob_ptr;
    bool has_tile;
    struct drm_tile_group *tile_group;
    bool tile_is_single_monitor;
    uint8_t num_h_tile;
    uint8_t num_v_tile;
    uint8_t tile_h_loc;
    uint8_t tile_v_loc;
    uint16_t tile_h_size;
    uint16_t tile_v_size;
    struct llist_node free_node;
    struct hdr_sink_metadata hdr_sink_metadata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct drm_connector {
    struct drm_device *dev;
    struct device *kdev;
    struct device_attribute *attr;
    struct list_head head;
    struct drm_mode_object base;
    char *name;
    struct mutex mutex;
    unsigned int index;
    int connector_type;
    int connector_type_id;
    bool interlace_allowed;
    bool doublescan_allowed;
    bool stereo_allowed;
    bool ycbcr_420_allowed;
    enum drm_connector_registration_state registration_state;
    struct list_head modes;
    enum drm_connector_status status;
    struct list_head probed_modes;
    struct drm_display_info display_info;
    const struct drm_connector_funcs *funcs;
    struct drm_property_blob *edid_blob_ptr;
    struct drm_object_properties properties;
    struct drm_property *scaling_mode_property;
    struct drm_property *vrr_capable_property;
    struct drm_property *colorspace_property;
    struct drm_property_blob *path_blob_ptr;
    struct drm_property *max_bpc_property;
    uint8_t polled;
    int dpms;
    const struct drm_connector_helper_funcs *helper_private;
    struct drm_cmdline_mode cmdline_mode;
    enum drm_connector_force force;
    bool override_edid;
    uint32_t encoder_ids[3];
    struct drm_encoder *encoder;
    uint8_t eld[128];
    bool latency_present[2];
    int video_latency[2];
    int audio_latency[2];
    struct i2c_adapter *ddc;
    int null_edid_counter;
    unsigned int bad_edid_counter;
    bool edid_corrupt;
    struct dentry *debugfs_entry;
    struct drm_connector_state *state;
    struct drm_property_blob *tile_blob_ptr;
    bool has_tile;
    struct drm_tile_group *tile_group;
    bool tile_is_single_monitor;
    uint8_t num_h_tile;
    uint8_t num_v_tile;
    uint8_t tile_h_loc;
    uint8_t tile_v_loc;
    uint16_t tile_h_size;
    uint16_t tile_v_size;
    struct llist_node free_node;
    struct hdr_sink_metadata hdr_sink_metadata;
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
struct drm_connector {
    struct drm_device *dev;
    struct device *kdev;
    struct device_attribute *attr;
    struct fwnode_handle *fwnode;
    struct list_head head;
    struct list_head global_connector_list_entry;
    struct drm_mode_object base;
    char *name;
    struct mutex mutex;
    unsigned int index;
    int connector_type;
    int connector_type_id;
    bool interlace_allowed;
    bool doublescan_allowed;
    bool stereo_allowed;
    bool ycbcr_420_allowed;
    enum drm_connector_registration_state registration_state;
    struct list_head modes;
    enum drm_connector_status status;
    struct list_head probed_modes;
    struct drm_display_info display_info;
    const struct drm_connector_funcs *funcs;
    struct drm_property_blob *edid_blob_ptr;
    struct drm_object_properties properties;
    struct drm_property *scaling_mode_property;
    struct drm_property *vrr_capable_property;
    struct drm_property *colorspace_property;
    struct drm_property_blob *path_blob_ptr;
    struct drm_property *max_bpc_property;
    struct drm_privacy_screen *privacy_screen;
    struct notifier_block privacy_screen_notifier;
    struct drm_property *privacy_screen_sw_state_property;
    struct drm_property *privacy_screen_hw_state_property;
    uint8_t polled;
    int dpms;
    const struct drm_connector_helper_funcs *helper_private;
    struct drm_cmdline_mode cmdline_mode;
    enum drm_connector_force force;
    const struct drm_edid *edid_override;
    struct mutex edid_override_mutex;
    u64 epoch_counter;
    u32 possible_encoders;
    struct drm_encoder *encoder;
    uint8_t eld[128];
    bool latency_present[2];
    int video_latency[2];
    int audio_latency[2];
    struct i2c_adapter *ddc;
    int null_edid_counter;
    unsigned int bad_edid_counter;
    bool edid_corrupt;
    u8 real_edid_checksum;
    struct dentry *debugfs_entry;
    struct drm_connector_state *state;
    struct drm_property_blob *tile_blob_ptr;
    bool has_tile;
    struct drm_tile_group *tile_group;
    bool tile_is_single_monitor;
    uint8_t num_h_tile;
    uint8_t num_v_tile;
    uint8_t tile_h_loc;
    uint8_t tile_v_loc;
    uint16_t tile_h_size;
    uint16_t tile_v_size;
    struct llist_node free_node;
    struct hdr_sink_metadata hdr_sink_metadata;
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
struct drm_connector {
    struct drm_device *dev;
    struct device *kdev;
    struct device_attribute *attr;
    struct list_head head;
    struct drm_mode_object base;
    char *name;
    struct mutex mutex;
    unsigned int index;
    int connector_type;
    int connector_type_id;
    bool interlace_allowed;
    bool doublescan_allowed;
    bool stereo_allowed;
    bool ycbcr_420_allowed;
    enum drm_connector_registration_state registration_state;
    struct list_head modes;
    enum drm_connector_status status;
    struct list_head probed_modes;
    struct drm_display_info display_info;
    const struct drm_connector_funcs *funcs;
    struct drm_property_blob *edid_blob_ptr;
    struct drm_object_properties properties;
    struct drm_property *scaling_mode_property;
    struct drm_property *vrr_capable_property;
    struct drm_property *colorspace_property;
    struct drm_property_blob *path_blob_ptr;
    struct drm_property *max_bpc_property;
    uint8_t polled;
    int dpms;
    const struct drm_connector_helper_funcs *helper_private;
    struct drm_cmdline_mode cmdline_mode;
    enum drm_connector_force force;
    bool override_edid;
    uint32_t encoder_ids[3];
    struct drm_encoder *encoder;
    uint8_t eld[128];
    bool latency_present[2];
    int video_latency[2];
    int audio_latency[2];
    struct i2c_adapter *ddc;
    int null_edid_counter;
    unsigned int bad_edid_counter;
    bool edid_corrupt;
    struct dentry *debugfs_entry;
    struct drm_connector_state *state;
    struct drm_property_blob *tile_blob_ptr;
    bool has_tile;
    struct drm_tile_group *tile_group;
    bool tile_is_single_monitor;
    uint8_t num_h_tile;
    uint8_t num_v_tile;
    uint8_t tile_h_loc;
    uint8_t tile_v_loc;
    uint16_t tile_h_size;
    uint16_t tile_v_size;
    struct llist_node free_node;
    struct hdr_sink_metadata hdr_sink_metadata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct drm_connector {
    struct drm_device *dev;
    struct device *kdev;
    struct device_attribute *attr;
    struct list_head head;
    struct drm_mode_object base;
    char *name;
    struct mutex mutex;
    unsigned int index;
    int connector_type;
    int connector_type_id;
    bool interlace_allowed;
    bool doublescan_allowed;
    bool stereo_allowed;
    bool ycbcr_420_allowed;
    enum drm_connector_registration_state registration_state;
    struct list_head modes;
    enum drm_connector_status status;
    struct list_head probed_modes;
    struct drm_display_info display_info;
    const struct drm_connector_funcs *funcs;
    struct drm_property_blob *edid_blob_ptr;
    struct drm_object_properties properties;
    struct drm_property *scaling_mode_property;
    struct drm_property *vrr_capable_property;
    struct drm_property *colorspace_property;
    struct drm_property_blob *path_blob_ptr;
    struct drm_property *max_bpc_property;
    uint8_t polled;
    int dpms;
    const struct drm_connector_helper_funcs *helper_private;
    struct drm_cmdline_mode cmdline_mode;
    enum drm_connector_force force;
    bool override_edid;
    uint32_t encoder_ids[3];
    struct drm_encoder *encoder;
    uint8_t eld[128];
    bool latency_present[2];
    int video_latency[2];
    int audio_latency[2];
    struct i2c_adapter *ddc;
    int null_edid_counter;
    unsigned int bad_edid_counter;
    bool edid_corrupt;
    struct dentry *debugfs_entry;
    struct drm_connector_state *state;
    struct drm_property_blob *tile_blob_ptr;
    bool has_tile;
    struct drm_tile_group *tile_group;
    bool tile_is_single_monitor;
    uint8_t num_h_tile;
    uint8_t num_v_tile;
    uint8_t tile_h_loc;
    uint8_t tile_v_loc;
    uint16_t tile_h_size;
    uint16_t tile_v_size;
    struct llist_node free_node;
    struct hdr_sink_metadata hdr_sink_metadata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct drm_connector {
    struct drm_device *dev;
    struct device *kdev;
    struct device_attribute *attr;
    struct list_head head;
    struct drm_mode_object base;
    char *name;
    struct mutex mutex;
    unsigned int index;
    int connector_type;
    int connector_type_id;
    bool interlace_allowed;
    bool doublescan_allowed;
    bool stereo_allowed;
    bool ycbcr_420_allowed;
    enum drm_connector_registration_state registration_state;
    struct list_head modes;
    enum drm_connector_status status;
    struct list_head probed_modes;
    struct drm_display_info display_info;
    const struct drm_connector_funcs *funcs;
    struct drm_property_blob *edid_blob_ptr;
    struct drm_object_properties properties;
    struct drm_property *scaling_mode_property;
    struct drm_property *vrr_capable_property;
    struct drm_property *colorspace_property;
    struct drm_property_blob *path_blob_ptr;
    struct drm_property *max_bpc_property;
    uint8_t polled;
    int dpms;
    const struct drm_connector_helper_funcs *helper_private;
    struct drm_cmdline_mode cmdline_mode;
    enum drm_connector_force force;
    bool override_edid;
    uint32_t encoder_ids[3];
    struct drm_encoder *encoder;
    uint8_t eld[128];
    bool latency_present[2];
    int video_latency[2];
    int audio_latency[2];
    struct i2c_adapter *ddc;
    int null_edid_counter;
    unsigned int bad_edid_counter;
    bool edid_corrupt;
    struct dentry *debugfs_entry;
    struct drm_connector_state *state;
    struct drm_property_blob *tile_blob_ptr;
    bool has_tile;
    struct drm_tile_group *tile_group;
    bool tile_is_single_monitor;
    uint8_t num_h_tile;
    uint8_t num_v_tile;
    uint8_t tile_h_loc;
    uint8_t tile_v_loc;
    uint16_t tile_h_size;
    uint16_t tile_v_size;
    struct llist_node free_node;
    struct hdr_sink_metadata hdr_sink_metadata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct drm_connector {
    struct drm_device *dev;
    struct device *kdev;
    struct device_attribute *attr;
    struct list_head head;
    struct drm_mode_object base;
    char *name;
    struct mutex mutex;
    unsigned int index;
    int connector_type;
    int connector_type_id;
    bool interlace_allowed;
    bool doublescan_allowed;
    bool stereo_allowed;
    bool ycbcr_420_allowed;
    enum drm_connector_registration_state registration_state;
    struct list_head modes;
    enum drm_connector_status status;
    struct list_head probed_modes;
    struct drm_display_info display_info;
    const struct drm_connector_funcs *funcs;
    struct drm_property_blob *edid_blob_ptr;
    struct drm_object_properties properties;
    struct drm_property *scaling_mode_property;
    struct drm_property *vrr_capable_property;
    struct drm_property *colorspace_property;
    struct drm_property_blob *path_blob_ptr;
    struct drm_property *max_bpc_property;
    uint8_t polled;
    int dpms;
    const struct drm_connector_helper_funcs *helper_private;
    struct drm_cmdline_mode cmdline_mode;
    enum drm_connector_force force;
    bool override_edid;
    uint32_t encoder_ids[3];
    struct drm_encoder *encoder;
    uint8_t eld[128];
    bool latency_present[2];
    int video_latency[2];
    int audio_latency[2];
    struct i2c_adapter *ddc;
    int null_edid_counter;
    unsigned int bad_edid_counter;
    bool edid_corrupt;
    struct dentry *debugfs_entry;
    struct drm_connector_state *state;
    struct drm_property_blob *tile_blob_ptr;
    bool has_tile;
    struct drm_tile_group *tile_group;
    bool tile_is_single_monitor;
    uint8_t num_h_tile;
    uint8_t num_v_tile;
    uint8_t tile_h_loc;
    uint8_t tile_v_loc;
    uint16_t tile_h_size;
    uint16_t tile_v_size;
    struct llist_node free_node;
    struct hdr_sink_metadata hdr_sink_metadata;
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
struct drm_connector {
    struct drm_device *dev;
    struct device *kdev;
    struct device_attribute *attr;
    struct list_head head;
    struct drm_mode_object base;
    char *name;
    struct mutex mutex;
    unsigned int index;
    int connector_type;
    int connector_type_id;
    bool interlace_allowed;
    bool doublescan_allowed;
    bool stereo_allowed;
    bool ycbcr_420_allowed;
    enum drm_connector_registration_state registration_state;
    struct list_head modes;
    enum drm_connector_status status;
    struct list_head probed_modes;
    struct drm_display_info display_info;
    const struct drm_connector_funcs *funcs;
    struct drm_property_blob *edid_blob_ptr;
    struct drm_object_properties properties;
    struct drm_property *scaling_mode_property;
    struct drm_property *vrr_capable_property;
    struct drm_property *colorspace_property;
    struct drm_property_blob *path_blob_ptr;
    struct drm_property *max_bpc_property;
    uint8_t polled;
    int dpms;
    const struct drm_connector_helper_funcs *helper_private;
    struct drm_cmdline_mode cmdline_mode;
    enum drm_connector_force force;
    bool override_edid;
    uint32_t encoder_ids[3];
    struct drm_encoder *encoder;
    uint8_t eld[128];
    bool latency_present[2];
    int video_latency[2];
    int audio_latency[2];
    struct i2c_adapter *ddc;
    int null_edid_counter;
    unsigned int bad_edid_counter;
    bool edid_corrupt;
    struct dentry *debugfs_entry;
    struct drm_connector_state *state;
    struct drm_property_blob *tile_blob_ptr;
    bool has_tile;
    struct drm_tile_group *tile_group;
    bool tile_is_single_monitor;
    uint8_t num_h_tile;
    uint8_t num_v_tile;
    uint8_t tile_h_loc;
    uint8_t tile_v_loc;
    uint16_t tile_h_size;
    uint16_t tile_v_size;
    struct llist_node free_node;
    struct hdr_sink_metadata hdr_sink_metadata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct drm_connector {
    struct drm_device *dev;
    struct device *kdev;
    struct device_attribute *attr;
    struct list_head head;
    struct drm_mode_object base;
    char *name;
    struct mutex mutex;
    unsigned int index;
    int connector_type;
    int connector_type_id;
    bool interlace_allowed;
    bool doublescan_allowed;
    bool stereo_allowed;
    bool ycbcr_420_allowed;
    enum drm_connector_registration_state registration_state;
    struct list_head modes;
    enum drm_connector_status status;
    struct list_head probed_modes;
    struct drm_display_info display_info;
    const struct drm_connector_funcs *funcs;
    struct drm_property_blob *edid_blob_ptr;
    struct drm_object_properties properties;
    struct drm_property *scaling_mode_property;
    struct drm_property *vrr_capable_property;
    struct drm_property *colorspace_property;
    struct drm_property_blob *path_blob_ptr;
    struct drm_property *max_bpc_property;
    uint8_t polled;
    int dpms;
    const struct drm_connector_helper_funcs *helper_private;
    struct drm_cmdline_mode cmdline_mode;
    enum drm_connector_force force;
    bool override_edid;
    uint32_t encoder_ids[3];
    struct drm_encoder *encoder;
    uint8_t eld[128];
    bool latency_present[2];
    int video_latency[2];
    int audio_latency[2];
    struct i2c_adapter *ddc;
    int null_edid_counter;
    unsigned int bad_edid_counter;
    bool edid_corrupt;
    struct dentry *debugfs_entry;
    struct drm_connector_state *state;
    struct drm_property_blob *tile_blob_ptr;
    bool has_tile;
    struct drm_tile_group *tile_group;
    bool tile_is_single_monitor;
    uint8_t num_h_tile;
    uint8_t num_v_tile;
    uint8_t tile_h_loc;
    uint8_t tile_v_loc;
    uint16_t tile_h_size;
    uint16_t tile_v_size;
    struct llist_node free_node;
    struct hdr_sink_metadata hdr_sink_metadata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct drm_connector {
    struct drm_device *dev;
    struct device *kdev;
    struct device_attribute *attr;
    struct list_head head;
    struct drm_mode_object base;
    char *name;
    struct mutex mutex;
    unsigned int index;
    int connector_type;
    int connector_type_id;
    bool interlace_allowed;
    bool doublescan_allowed;
    bool stereo_allowed;
    bool ycbcr_420_allowed;
    enum drm_connector_registration_state registration_state;
    struct list_head modes;
    enum drm_connector_status status;
    struct list_head probed_modes;
    struct drm_display_info display_info;
    const struct drm_connector_funcs *funcs;
    struct drm_property_blob *edid_blob_ptr;
    struct drm_object_properties properties;
    struct drm_property *scaling_mode_property;
    struct drm_property *vrr_capable_property;
    struct drm_property *colorspace_property;
    struct drm_property_blob *path_blob_ptr;
    struct drm_property *max_bpc_property;
    uint8_t polled;
    int dpms;
    const struct drm_connector_helper_funcs *helper_private;
    struct drm_cmdline_mode cmdline_mode;
    enum drm_connector_force force;
    bool override_edid;
    uint32_t encoder_ids[3];
    struct drm_encoder *encoder;
    uint8_t eld[128];
    bool latency_present[2];
    int video_latency[2];
    int audio_latency[2];
    struct i2c_adapter *ddc;
    int null_edid_counter;
    unsigned int bad_edid_counter;
    bool edid_corrupt;
    struct dentry *debugfs_entry;
    struct drm_connector_state *state;
    struct drm_property_blob *tile_blob_ptr;
    bool has_tile;
    struct drm_tile_group *tile_group;
    bool tile_is_single_monitor;
    uint8_t num_h_tile;
    uint8_t num_v_tile;
    uint8_t tile_h_loc;
    uint8_t tile_v_loc;
    uint16_t tile_h_size;
    uint16_t tile_v_size;
    struct llist_node free_node;
    struct hdr_sink_metadata hdr_sink_metadata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct drm_connector {
    struct drm_device *dev;
    struct device *kdev;
    struct device_attribute *attr;
    struct list_head head;
    struct drm_mode_object base;
    char *name;
    struct mutex mutex;
    unsigned int index;
    int connector_type;
    int connector_type_id;
    bool interlace_allowed;
    bool doublescan_allowed;
    bool stereo_allowed;
    bool ycbcr_420_allowed;
    enum drm_connector_registration_state registration_state;
    struct list_head modes;
    enum drm_connector_status status;
    struct list_head probed_modes;
    struct drm_display_info display_info;
    const struct drm_connector_funcs *funcs;
    struct drm_property_blob *edid_blob_ptr;
    struct drm_object_properties properties;
    struct drm_property *scaling_mode_property;
    struct drm_property *vrr_capable_property;
    struct drm_property *colorspace_property;
    struct drm_property_blob *path_blob_ptr;
    struct drm_property *max_bpc_property;
    uint8_t polled;
    int dpms;
    const struct drm_connector_helper_funcs *helper_private;
    struct drm_cmdline_mode cmdline_mode;
    enum drm_connector_force force;
    bool override_edid;
    uint32_t encoder_ids[3];
    struct drm_encoder *encoder;
    uint8_t eld[128];
    bool latency_present[2];
    int video_latency[2];
    int audio_latency[2];
    struct i2c_adapter *ddc;
    int null_edid_counter;
    unsigned int bad_edid_counter;
    bool edid_corrupt;
    struct dentry *debugfs_entry;
    struct drm_connector_state *state;
    struct drm_property_blob *tile_blob_ptr;
    bool has_tile;
    struct drm_tile_group *tile_group;
    bool tile_is_single_monitor;
    uint8_t num_h_tile;
    uint8_t num_v_tile;
    uint8_t tile_h_loc;
    uint8_t tile_v_loc;
    uint16_t tile_h_size;
    uint16_t tile_v_size;
    struct llist_node free_node;
    struct hdr_sink_metadata hdr_sink_metadata;
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
<code>struct i2c_adapter *ddc</code>
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
<details>
<summary>Changed between <code>generic</code> and <code>aws</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct i2c_adapter *ddc</code> ➡️ <code>struct i2c_adapter *ddc</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>generic</code> and <code>azure</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct i2c_adapter *ddc</code> ➡️ <code>struct i2c_adapter *ddc</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
