# Struct: <code>drm_mode_config_funcs</code>

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
struct drm_mode_config_funcs {
    struct drm_framebuffer * (*fb_create)(struct drm_device *, struct drm_file *, const struct drm_mode_fb_cmd2 *);
    const struct drm_format_info * (*get_format_info)(const struct drm_mode_fb_cmd2 *);
    void (*output_poll_changed)(struct drm_device *);
    enum drm_mode_status (*mode_valid)(struct drm_device *, const struct drm_display_mode *);
    int (*atomic_check)(struct drm_device *, struct drm_atomic_state *);
    int (*atomic_commit)(struct drm_device *, struct drm_atomic_state *, bool);
    struct drm_atomic_state * (*atomic_state_alloc)(struct drm_device *);
    void (*atomic_state_clear)(struct drm_atomic_state *);
    void (*atomic_state_free)(struct drm_atomic_state *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct drm_mode_config_funcs {
    struct drm_framebuffer * (*fb_create)(struct drm_device *, struct drm_file *, const struct drm_mode_fb_cmd2 *);
    const struct drm_format_info * (*get_format_info)(const struct drm_mode_fb_cmd2 *);
    void (*output_poll_changed)(struct drm_device *);
    enum drm_mode_status (*mode_valid)(struct drm_device *, const struct drm_display_mode *);
    int (*atomic_check)(struct drm_device *, struct drm_atomic_state *);
    int (*atomic_commit)(struct drm_device *, struct drm_atomic_state *, bool);
    struct drm_atomic_state * (*atomic_state_alloc)(struct drm_device *);
    void (*atomic_state_clear)(struct drm_atomic_state *);
    void (*atomic_state_free)(struct drm_atomic_state *);
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
struct drm_mode_config_funcs {
    struct drm_framebuffer * (*fb_create)(struct drm_device *, struct drm_file *, const struct drm_mode_fb_cmd2 *);
    const struct drm_format_info * (*get_format_info)(const struct drm_mode_fb_cmd2 *);
    void (*output_poll_changed)(struct drm_device *);
    enum drm_mode_status (*mode_valid)(struct drm_device *, const struct drm_display_mode *);
    int (*atomic_check)(struct drm_device *, struct drm_atomic_state *);
    int (*atomic_commit)(struct drm_device *, struct drm_atomic_state *, bool);
    struct drm_atomic_state * (*atomic_state_alloc)(struct drm_device *);
    void (*atomic_state_clear)(struct drm_atomic_state *);
    void (*atomic_state_free)(struct drm_atomic_state *);
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
struct drm_mode_config_funcs {
    struct drm_framebuffer * (*fb_create)(struct drm_device *, struct drm_file *, const struct drm_mode_fb_cmd2 *);
    const struct drm_format_info * (*get_format_info)(const struct drm_mode_fb_cmd2 *);
    void (*output_poll_changed)(struct drm_device *);
    enum drm_mode_status (*mode_valid)(struct drm_device *, const struct drm_display_mode *);
    int (*atomic_check)(struct drm_device *, struct drm_atomic_state *);
    int (*atomic_commit)(struct drm_device *, struct drm_atomic_state *, bool);
    struct drm_atomic_state * (*atomic_state_alloc)(struct drm_device *);
    void (*atomic_state_clear)(struct drm_atomic_state *);
    void (*atomic_state_free)(struct drm_atomic_state *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct drm_mode_config_funcs {
    struct drm_framebuffer * (*fb_create)(struct drm_device *, struct drm_file *, const struct drm_mode_fb_cmd2 *);
    const struct drm_format_info * (*get_format_info)(const struct drm_mode_fb_cmd2 *);
    void (*output_poll_changed)(struct drm_device *);
    enum drm_mode_status (*mode_valid)(struct drm_device *, const struct drm_display_mode *);
    int (*atomic_check)(struct drm_device *, struct drm_atomic_state *);
    int (*atomic_commit)(struct drm_device *, struct drm_atomic_state *, bool);
    struct drm_atomic_state * (*atomic_state_alloc)(struct drm_device *);
    void (*atomic_state_clear)(struct drm_atomic_state *);
    void (*atomic_state_free)(struct drm_atomic_state *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct drm_mode_config_funcs {
    struct drm_framebuffer * (*fb_create)(struct drm_device *, struct drm_file *, const struct drm_mode_fb_cmd2 *);
    const struct drm_format_info * (*get_format_info)(const struct drm_mode_fb_cmd2 *);
    void (*output_poll_changed)(struct drm_device *);
    enum drm_mode_status (*mode_valid)(struct drm_device *, const struct drm_display_mode *);
    int (*atomic_check)(struct drm_device *, struct drm_atomic_state *);
    int (*atomic_commit)(struct drm_device *, struct drm_atomic_state *, bool);
    struct drm_atomic_state * (*atomic_state_alloc)(struct drm_device *);
    void (*atomic_state_clear)(struct drm_atomic_state *);
    void (*atomic_state_free)(struct drm_atomic_state *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct drm_mode_config_funcs {
    struct drm_framebuffer * (*fb_create)(struct drm_device *, struct drm_file *, const struct drm_mode_fb_cmd2 *);
    const struct drm_format_info * (*get_format_info)(const struct drm_mode_fb_cmd2 *);
    void (*output_poll_changed)(struct drm_device *);
    enum drm_mode_status (*mode_valid)(struct drm_device *, const struct drm_display_mode *);
    int (*atomic_check)(struct drm_device *, struct drm_atomic_state *);
    int (*atomic_commit)(struct drm_device *, struct drm_atomic_state *, bool);
    struct drm_atomic_state * (*atomic_state_alloc)(struct drm_device *);
    void (*atomic_state_clear)(struct drm_atomic_state *);
    void (*atomic_state_free)(struct drm_atomic_state *);
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
struct drm_mode_config_funcs {
    struct drm_framebuffer * (*fb_create)(struct drm_device *, struct drm_file *, const struct drm_mode_fb_cmd2 *);
    const struct drm_format_info * (*get_format_info)(const struct drm_mode_fb_cmd2 *);
    void (*output_poll_changed)(struct drm_device *);
    enum drm_mode_status (*mode_valid)(struct drm_device *, const struct drm_display_mode *);
    int (*atomic_check)(struct drm_device *, struct drm_atomic_state *);
    int (*atomic_commit)(struct drm_device *, struct drm_atomic_state *, bool);
    struct drm_atomic_state * (*atomic_state_alloc)(struct drm_device *);
    void (*atomic_state_clear)(struct drm_atomic_state *);
    void (*atomic_state_free)(struct drm_atomic_state *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct drm_mode_config_funcs {
    struct drm_framebuffer * (*fb_create)(struct drm_device *, struct drm_file *, const struct drm_mode_fb_cmd2 *);
    const struct drm_format_info * (*get_format_info)(const struct drm_mode_fb_cmd2 *);
    void (*output_poll_changed)(struct drm_device *);
    enum drm_mode_status (*mode_valid)(struct drm_device *, const struct drm_display_mode *);
    int (*atomic_check)(struct drm_device *, struct drm_atomic_state *);
    int (*atomic_commit)(struct drm_device *, struct drm_atomic_state *, bool);
    struct drm_atomic_state * (*atomic_state_alloc)(struct drm_device *);
    void (*atomic_state_clear)(struct drm_atomic_state *);
    void (*atomic_state_free)(struct drm_atomic_state *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct drm_mode_config_funcs {
    struct drm_framebuffer * (*fb_create)(struct drm_device *, struct drm_file *, const struct drm_mode_fb_cmd2 *);
    const struct drm_format_info * (*get_format_info)(const struct drm_mode_fb_cmd2 *);
    void (*output_poll_changed)(struct drm_device *);
    enum drm_mode_status (*mode_valid)(struct drm_device *, const struct drm_display_mode *);
    int (*atomic_check)(struct drm_device *, struct drm_atomic_state *);
    int (*atomic_commit)(struct drm_device *, struct drm_atomic_state *, bool);
    struct drm_atomic_state * (*atomic_state_alloc)(struct drm_device *);
    void (*atomic_state_clear)(struct drm_atomic_state *);
    void (*atomic_state_free)(struct drm_atomic_state *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct drm_mode_config_funcs {
    struct drm_framebuffer * (*fb_create)(struct drm_device *, struct drm_file *, const struct drm_mode_fb_cmd2 *);
    const struct drm_format_info * (*get_format_info)(const struct drm_mode_fb_cmd2 *);
    void (*output_poll_changed)(struct drm_device *);
    enum drm_mode_status (*mode_valid)(struct drm_device *, const struct drm_display_mode *);
    int (*atomic_check)(struct drm_device *, struct drm_atomic_state *);
    int (*atomic_commit)(struct drm_device *, struct drm_atomic_state *, bool);
    struct drm_atomic_state * (*atomic_state_alloc)(struct drm_device *);
    void (*atomic_state_clear)(struct drm_atomic_state *);
    void (*atomic_state_free)(struct drm_atomic_state *);
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
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
