# Struct: <code>drm_crtc_helper_funcs</code>

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
struct drm_crtc_helper_funcs {
    void (*dpms)(struct drm_crtc *, int);
    void (*prepare)(struct drm_crtc *);
    void (*commit)(struct drm_crtc *);
    enum drm_mode_status (*mode_valid)(struct drm_crtc *, const struct drm_display_mode *);
    bool (*mode_fixup)(struct drm_crtc *, const struct drm_display_mode *, struct drm_display_mode *);
    int (*mode_set)(struct drm_crtc *, struct drm_display_mode *, struct drm_display_mode *, int, int, struct drm_framebuffer *);
    void (*mode_set_nofb)(struct drm_crtc *);
    int (*mode_set_base)(struct drm_crtc *, int, int, struct drm_framebuffer *);
    int (*mode_set_base_atomic)(struct drm_crtc *, struct drm_framebuffer *, int, int, enum mode_set_atomic);
    void (*disable)(struct drm_crtc *);
    int (*atomic_check)(struct drm_crtc *, struct drm_atomic_state *);
    void (*atomic_begin)(struct drm_crtc *, struct drm_atomic_state *);
    void (*atomic_flush)(struct drm_crtc *, struct drm_atomic_state *);
    void (*atomic_enable)(struct drm_crtc *, struct drm_atomic_state *);
    void (*atomic_disable)(struct drm_crtc *, struct drm_atomic_state *);
    bool (*get_scanout_position)(struct drm_crtc *, bool, int *, int *, ktime_t *, ktime_t *, const struct drm_display_mode *);
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
