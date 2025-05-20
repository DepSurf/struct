# Struct: <code>drm_plane_funcs</code>

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
struct drm_plane_funcs {
    int (*update_plane)(struct drm_plane *, struct drm_crtc *, struct drm_framebuffer *, int, int, unsigned int, unsigned int, uint32_t, uint32_t, uint32_t, uint32_t, struct drm_modeset_acquire_ctx *);
    int (*disable_plane)(struct drm_plane *, struct drm_modeset_acquire_ctx *);
    void (*destroy)(struct drm_plane *);
    void (*reset)(struct drm_plane *);
    int (*set_property)(struct drm_plane *, struct drm_property *, uint64_t);
    struct drm_plane_state * (*atomic_duplicate_state)(struct drm_plane *);
    void (*atomic_destroy_state)(struct drm_plane *, struct drm_plane_state *);
    int (*atomic_set_property)(struct drm_plane *, struct drm_plane_state *, struct drm_property *, uint64_t);
    int (*atomic_get_property)(struct drm_plane *, const struct drm_plane_state *, struct drm_property *, uint64_t *);
    int (*late_register)(struct drm_plane *);
    void (*early_unregister)(struct drm_plane *);
    void (*atomic_print_state)(struct drm_printer *, const struct drm_plane_state *);
    bool (*format_mod_supported)(struct drm_plane *, uint32_t, uint64_t);
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
