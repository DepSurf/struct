# Struct: <code>drm_connector_helper_funcs</code>

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
struct drm_connector_helper_funcs {
    int (*get_modes)(struct drm_connector *);
    int (*detect_ctx)(struct drm_connector *, struct drm_modeset_acquire_ctx *, bool);
    enum drm_mode_status (*mode_valid)(struct drm_connector *, struct drm_display_mode *);
    int (*mode_valid_ctx)(struct drm_connector *, struct drm_display_mode *, struct drm_modeset_acquire_ctx *, enum drm_mode_status *);
    struct drm_encoder * (*best_encoder)(struct drm_connector *);
    struct drm_encoder * (*atomic_best_encoder)(struct drm_connector *, struct drm_atomic_state *);
    int (*atomic_check)(struct drm_connector *, struct drm_atomic_state *);
    void (*atomic_commit)(struct drm_connector *, struct drm_atomic_state *);
    int (*prepare_writeback_job)(struct drm_writeback_connector *, struct drm_writeback_job *);
    void (*cleanup_writeback_job)(struct drm_writeback_connector *, struct drm_writeback_job *);
    void (*enable_hpd)(struct drm_connector *);
    void (*disable_hpd)(struct drm_connector *);
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
