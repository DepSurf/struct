# Struct: <code>drm_cmdline_mode</code>

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
struct drm_cmdline_mode {
    char name[32];
    bool specified;
    bool refresh_specified;
    bool bpp_specified;
    int xres;
    int yres;
    int bpp;
    int refresh;
    bool rb;
    bool interlace;
    bool cvt;
    bool margins;
    enum drm_connector_force force;
    unsigned int rotation_reflection;
    struct drm_connector_tv_margins tv_margins;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct drm_cmdline_mode {
    char name[32];
    bool specified;
    bool refresh_specified;
    bool bpp_specified;
    int xres;
    int yres;
    int bpp;
    int refresh;
    bool rb;
    bool interlace;
    bool cvt;
    bool margins;
    enum drm_connector_force force;
    unsigned int rotation_reflection;
    struct drm_connector_tv_margins tv_margins;
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
struct drm_cmdline_mode {
    char name[32];
    bool specified;
    bool refresh_specified;
    bool bpp_specified;
    unsigned int pixel_clock;
    int xres;
    int yres;
    int bpp;
    int refresh;
    bool rb;
    bool interlace;
    bool cvt;
    bool margins;
    enum drm_connector_force force;
    unsigned int rotation_reflection;
    enum drm_panel_orientation panel_orientation;
    struct drm_connector_tv_margins tv_margins;
    enum drm_connector_tv_mode tv_mode;
    bool tv_mode_specified;
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
struct drm_cmdline_mode {
    char name[32];
    bool specified;
    bool refresh_specified;
    bool bpp_specified;
    int xres;
    int yres;
    int bpp;
    int refresh;
    bool rb;
    bool interlace;
    bool cvt;
    bool margins;
    enum drm_connector_force force;
    unsigned int rotation_reflection;
    struct drm_connector_tv_margins tv_margins;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct drm_cmdline_mode {
    char name[32];
    bool specified;
    bool refresh_specified;
    bool bpp_specified;
    int xres;
    int yres;
    int bpp;
    int refresh;
    bool rb;
    bool interlace;
    bool cvt;
    bool margins;
    enum drm_connector_force force;
    unsigned int rotation_reflection;
    struct drm_connector_tv_margins tv_margins;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct drm_cmdline_mode {
    char name[32];
    bool specified;
    bool refresh_specified;
    bool bpp_specified;
    int xres;
    int yres;
    int bpp;
    int refresh;
    bool rb;
    bool interlace;
    bool cvt;
    bool margins;
    enum drm_connector_force force;
    unsigned int rotation_reflection;
    struct drm_connector_tv_margins tv_margins;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct drm_cmdline_mode {
    char name[32];
    bool specified;
    bool refresh_specified;
    bool bpp_specified;
    int xres;
    int yres;
    int bpp;
    int refresh;
    bool rb;
    bool interlace;
    bool cvt;
    bool margins;
    enum drm_connector_force force;
    unsigned int rotation_reflection;
    struct drm_connector_tv_margins tv_margins;
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
struct drm_cmdline_mode {
    char name[32];
    bool specified;
    bool refresh_specified;
    bool bpp_specified;
    int xres;
    int yres;
    int bpp;
    int refresh;
    bool rb;
    bool interlace;
    bool cvt;
    bool margins;
    enum drm_connector_force force;
    unsigned int rotation_reflection;
    struct drm_connector_tv_margins tv_margins;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct drm_cmdline_mode {
    char name[32];
    bool specified;
    bool refresh_specified;
    bool bpp_specified;
    int xres;
    int yres;
    int bpp;
    int refresh;
    bool rb;
    bool interlace;
    bool cvt;
    bool margins;
    enum drm_connector_force force;
    unsigned int rotation_reflection;
    struct drm_connector_tv_margins tv_margins;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct drm_cmdline_mode {
    char name[32];
    bool specified;
    bool refresh_specified;
    bool bpp_specified;
    int xres;
    int yres;
    int bpp;
    int refresh;
    bool rb;
    bool interlace;
    bool cvt;
    bool margins;
    enum drm_connector_force force;
    unsigned int rotation_reflection;
    struct drm_connector_tv_margins tv_margins;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct drm_cmdline_mode {
    char name[32];
    bool specified;
    bool refresh_specified;
    bool bpp_specified;
    int xres;
    int yres;
    int bpp;
    int refresh;
    bool rb;
    bool interlace;
    bool cvt;
    bool margins;
    enum drm_connector_force force;
    unsigned int rotation_reflection;
    struct drm_connector_tv_margins tv_margins;
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
