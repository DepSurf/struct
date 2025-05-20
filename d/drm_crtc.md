# Struct: <code>drm_crtc</code>

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
In <code>5.3</code>: Absent ⚠️
</li>
<li>
In <code>5.4</code>: Absent ⚠️
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
struct drm_crtc {
    struct drm_device *dev;
    struct device_node *port;
    struct list_head head;
    char *name;
    struct drm_modeset_lock mutex;
    struct drm_mode_object base;
    struct drm_plane *primary;
    struct drm_plane *cursor;
    unsigned int index;
    int cursor_x;
    int cursor_y;
    bool enabled;
    struct drm_display_mode mode;
    struct drm_display_mode hwmode;
    int x;
    int y;
    const struct drm_crtc_funcs *funcs;
    uint32_t gamma_size;
    uint16_t *gamma_store;
    const struct drm_crtc_helper_funcs *helper_private;
    struct drm_object_properties properties;
    struct drm_property *scaling_filter_property;
    struct drm_crtc_state *state;
    struct list_head commit_list;
    spinlock_t commit_lock;
    struct dentry *debugfs_entry;
    struct drm_crtc_crc crc;
    unsigned int fence_context;
    spinlock_t fence_lock;
    long unsigned int fence_seqno;
    char timeline_name[32];
    struct drm_self_refresh_data *self_refresh_data;
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
In <code>arm64</code>: Absent ⚠️
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
</li>
<li>
In <code>riscv64</code>: Absent ⚠️
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
In <code>aws</code>: Absent ⚠️
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
</ul>
