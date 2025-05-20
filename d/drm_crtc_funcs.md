# Struct: <code>drm_crtc_funcs</code>

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
struct drm_crtc_funcs {
    void (*reset)(struct drm_crtc *);
    int (*cursor_set)(struct drm_crtc *, struct drm_file *, uint32_t, uint32_t, uint32_t);
    int (*cursor_set2)(struct drm_crtc *, struct drm_file *, uint32_t, uint32_t, uint32_t, int32_t, int32_t);
    int (*cursor_move)(struct drm_crtc *, int, int);
    int (*gamma_set)(struct drm_crtc *, u16 *, u16 *, u16 *, uint32_t, struct drm_modeset_acquire_ctx *);
    void (*destroy)(struct drm_crtc *);
    int (*set_config)(struct drm_mode_set *, struct drm_modeset_acquire_ctx *);
    int (*page_flip)(struct drm_crtc *, struct drm_framebuffer *, struct drm_pending_vblank_event *, uint32_t, struct drm_modeset_acquire_ctx *);
    int (*page_flip_target)(struct drm_crtc *, struct drm_framebuffer *, struct drm_pending_vblank_event *, uint32_t, uint32_t, struct drm_modeset_acquire_ctx *);
    int (*set_property)(struct drm_crtc *, struct drm_property *, uint64_t);
    struct drm_crtc_state * (*atomic_duplicate_state)(struct drm_crtc *);
    void (*atomic_destroy_state)(struct drm_crtc *, struct drm_crtc_state *);
    int (*atomic_set_property)(struct drm_crtc *, struct drm_crtc_state *, struct drm_property *, uint64_t);
    int (*atomic_get_property)(struct drm_crtc *, const struct drm_crtc_state *, struct drm_property *, uint64_t *);
    int (*late_register)(struct drm_crtc *);
    void (*early_unregister)(struct drm_crtc *);
    int (*set_crc_source)(struct drm_crtc *, const char *);
    int (*verify_crc_source)(struct drm_crtc *, const char *, size_t *);
    const const char * * (*get_crc_sources)(struct drm_crtc *, size_t *);
    void (*atomic_print_state)(struct drm_printer *, const struct drm_crtc_state *);
    u32 (*get_vblank_counter)(struct drm_crtc *);
    int (*enable_vblank)(struct drm_crtc *);
    void (*disable_vblank)(struct drm_crtc *);
    bool (*get_vblank_timestamp)(struct drm_crtc *, int *, ktime_t *, bool);
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
