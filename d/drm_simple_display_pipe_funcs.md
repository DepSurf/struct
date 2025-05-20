# Struct: <code>drm_simple_display_pipe_funcs</code>

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
struct drm_simple_display_pipe_funcs {
    enum drm_mode_status (*mode_valid)(struct drm_simple_display_pipe *, const struct drm_display_mode *);
    void (*enable)(struct drm_simple_display_pipe *, struct drm_crtc_state *, struct drm_plane_state *);
    void (*disable)(struct drm_simple_display_pipe *);
    int (*check)(struct drm_simple_display_pipe *, struct drm_plane_state *, struct drm_crtc_state *);
    void (*update)(struct drm_simple_display_pipe *, struct drm_plane_state *);
    int (*prepare_fb)(struct drm_simple_display_pipe *, struct drm_plane_state *);
    void (*cleanup_fb)(struct drm_simple_display_pipe *, struct drm_plane_state *);
    int (*begin_fb_access)(struct drm_simple_display_pipe *, struct drm_plane_state *);
    void (*end_fb_access)(struct drm_simple_display_pipe *, struct drm_plane_state *);
    int (*enable_vblank)(struct drm_simple_display_pipe *);
    void (*disable_vblank)(struct drm_simple_display_pipe *);
    void (*reset_crtc)(struct drm_simple_display_pipe *);
    struct drm_crtc_state * (*duplicate_crtc_state)(struct drm_simple_display_pipe *);
    void (*destroy_crtc_state)(struct drm_simple_display_pipe *, struct drm_crtc_state *);
    void (*reset_plane)(struct drm_simple_display_pipe *);
    struct drm_plane_state * (*duplicate_plane_state)(struct drm_simple_display_pipe *);
    void (*destroy_plane_state)(struct drm_simple_display_pipe *, struct drm_plane_state *);
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
