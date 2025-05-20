# Struct: <code>drm_bridge_funcs</code>

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
struct drm_bridge_funcs {
    int (*attach)(struct drm_bridge *, enum drm_bridge_attach_flags);
    void (*detach)(struct drm_bridge *);
    enum drm_mode_status (*mode_valid)(struct drm_bridge *, const struct drm_display_info *, const struct drm_display_mode *);
    bool (*mode_fixup)(struct drm_bridge *, const struct drm_display_mode *, struct drm_display_mode *);
    void (*disable)(struct drm_bridge *);
    void (*post_disable)(struct drm_bridge *);
    void (*mode_set)(struct drm_bridge *, const struct drm_display_mode *, const struct drm_display_mode *);
    void (*pre_enable)(struct drm_bridge *);
    void (*enable)(struct drm_bridge *);
    void (*atomic_pre_enable)(struct drm_bridge *, struct drm_bridge_state *);
    void (*atomic_enable)(struct drm_bridge *, struct drm_bridge_state *);
    void (*atomic_disable)(struct drm_bridge *, struct drm_bridge_state *);
    void (*atomic_post_disable)(struct drm_bridge *, struct drm_bridge_state *);
    struct drm_bridge_state * (*atomic_duplicate_state)(struct drm_bridge *);
    void (*atomic_destroy_state)(struct drm_bridge *, struct drm_bridge_state *);
    u32 * (*atomic_get_output_bus_fmts)(struct drm_bridge *, struct drm_bridge_state *, struct drm_crtc_state *, struct drm_connector_state *, unsigned int *);
    u32 * (*atomic_get_input_bus_fmts)(struct drm_bridge *, struct drm_bridge_state *, struct drm_crtc_state *, struct drm_connector_state *, u32, unsigned int *);
    int (*atomic_check)(struct drm_bridge *, struct drm_bridge_state *, struct drm_crtc_state *, struct drm_connector_state *);
    struct drm_bridge_state * (*atomic_reset)(struct drm_bridge *);
    enum drm_connector_status (*detect)(struct drm_bridge *);
    int (*get_modes)(struct drm_bridge *, struct drm_connector *);
    struct edid * (*get_edid)(struct drm_bridge *, struct drm_connector *);
    void (*hpd_notify)(struct drm_bridge *, enum drm_connector_status);
    void (*hpd_enable)(struct drm_bridge *);
    void (*hpd_disable)(struct drm_bridge *);
    void (*debugfs_init)(struct drm_bridge *, struct dentry *);
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
