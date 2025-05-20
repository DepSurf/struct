# Struct: <code>mipi_dsi_device</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct mipi_dsi_device {
    struct mipi_dsi_host *host;
    struct device dev;
    unsigned int channel;
    unsigned int lanes;
    enum mipi_dsi_pixel_format format;
    long unsigned int mode_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct mipi_dsi_device {
    struct mipi_dsi_host *host;
    struct device dev;
    char name[20];
    unsigned int channel;
    unsigned int lanes;
    enum mipi_dsi_pixel_format format;
    long unsigned int mode_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct mipi_dsi_device {
    struct mipi_dsi_host *host;
    struct device dev;
    char name[20];
    unsigned int channel;
    unsigned int lanes;
    enum mipi_dsi_pixel_format format;
    long unsigned int mode_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct mipi_dsi_device {
    struct mipi_dsi_host *host;
    struct device dev;
    char name[20];
    unsigned int channel;
    unsigned int lanes;
    enum mipi_dsi_pixel_format format;
    long unsigned int mode_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct mipi_dsi_device {
    struct mipi_dsi_host *host;
    struct device dev;
    char name[20];
    unsigned int channel;
    unsigned int lanes;
    enum mipi_dsi_pixel_format format;
    long unsigned int mode_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct mipi_dsi_device {
    struct mipi_dsi_host *host;
    struct device dev;
    char name[20];
    unsigned int channel;
    unsigned int lanes;
    enum mipi_dsi_pixel_format format;
    long unsigned int mode_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct mipi_dsi_device {
    struct mipi_dsi_host *host;
    struct device dev;
    char name[20];
    unsigned int channel;
    unsigned int lanes;
    enum mipi_dsi_pixel_format format;
    long unsigned int mode_flags;
    long unsigned int hs_rate;
    long unsigned int lp_rate;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct mipi_dsi_device {
    struct mipi_dsi_host *host;
    struct device dev;
    char name[20];
    unsigned int channel;
    unsigned int lanes;
    enum mipi_dsi_pixel_format format;
    long unsigned int mode_flags;
    long unsigned int hs_rate;
    long unsigned int lp_rate;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct mipi_dsi_device {
    struct mipi_dsi_host *host;
    struct device dev;
    char name[20];
    unsigned int channel;
    unsigned int lanes;
    enum mipi_dsi_pixel_format format;
    long unsigned int mode_flags;
    long unsigned int hs_rate;
    long unsigned int lp_rate;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct mipi_dsi_device {
    struct mipi_dsi_host *host;
    struct device dev;
    char name[20];
    unsigned int channel;
    unsigned int lanes;
    enum mipi_dsi_pixel_format format;
    long unsigned int mode_flags;
    long unsigned int hs_rate;
    long unsigned int lp_rate;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mipi_dsi_device {
    struct mipi_dsi_host *host;
    struct device dev;
    char name[20];
    unsigned int channel;
    unsigned int lanes;
    enum mipi_dsi_pixel_format format;
    long unsigned int mode_flags;
    long unsigned int hs_rate;
    long unsigned int lp_rate;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mipi_dsi_device {
    struct mipi_dsi_host *host;
    struct device dev;
    char name[20];
    unsigned int channel;
    unsigned int lanes;
    enum mipi_dsi_pixel_format format;
    long unsigned int mode_flags;
    long unsigned int hs_rate;
    long unsigned int lp_rate;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mipi_dsi_device {
    struct mipi_dsi_host *host;
    struct device dev;
    char name[20];
    unsigned int channel;
    unsigned int lanes;
    enum mipi_dsi_pixel_format format;
    long unsigned int mode_flags;
    long unsigned int hs_rate;
    long unsigned int lp_rate;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mipi_dsi_device {
    struct mipi_dsi_host *host;
    struct device dev;
    char name[20];
    unsigned int channel;
    unsigned int lanes;
    enum mipi_dsi_pixel_format format;
    long unsigned int mode_flags;
    long unsigned int hs_rate;
    long unsigned int lp_rate;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mipi_dsi_device {
    struct mipi_dsi_host *host;
    struct device dev;
    char name[20];
    unsigned int channel;
    unsigned int lanes;
    enum mipi_dsi_pixel_format format;
    long unsigned int mode_flags;
    long unsigned int hs_rate;
    long unsigned int lp_rate;
    struct drm_dsc_config *dsc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mipi_dsi_device {
    struct mipi_dsi_host *host;
    struct device dev;
    char name[20];
    unsigned int channel;
    unsigned int lanes;
    enum mipi_dsi_pixel_format format;
    long unsigned int mode_flags;
    long unsigned int hs_rate;
    long unsigned int lp_rate;
    struct drm_dsc_config *dsc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mipi_dsi_device {
    struct mipi_dsi_host *host;
    struct device dev;
    bool attached;
    char name[20];
    unsigned int channel;
    unsigned int lanes;
    enum mipi_dsi_pixel_format format;
    long unsigned int mode_flags;
    long unsigned int hs_rate;
    long unsigned int lp_rate;
    struct drm_dsc_config *dsc;
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
struct mipi_dsi_device {
    struct mipi_dsi_host *host;
    struct device dev;
    char name[20];
    unsigned int channel;
    unsigned int lanes;
    enum mipi_dsi_pixel_format format;
    long unsigned int mode_flags;
    long unsigned int hs_rate;
    long unsigned int lp_rate;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mipi_dsi_device {
    struct mipi_dsi_host *host;
    struct device dev;
    char name[20];
    unsigned int channel;
    unsigned int lanes;
    enum mipi_dsi_pixel_format format;
    long unsigned int mode_flags;
    long unsigned int hs_rate;
    long unsigned int lp_rate;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct mipi_dsi_device {
    struct mipi_dsi_host *host;
    struct device dev;
    char name[20];
    unsigned int channel;
    unsigned int lanes;
    enum mipi_dsi_pixel_format format;
    long unsigned int mode_flags;
    long unsigned int hs_rate;
    long unsigned int lp_rate;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct mipi_dsi_device {
    struct mipi_dsi_host *host;
    struct device dev;
    char name[20];
    unsigned int channel;
    unsigned int lanes;
    enum mipi_dsi_pixel_format format;
    long unsigned int mode_flags;
    long unsigned int hs_rate;
    long unsigned int lp_rate;
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
struct mipi_dsi_device {
    struct mipi_dsi_host *host;
    struct device dev;
    char name[20];
    unsigned int channel;
    unsigned int lanes;
    enum mipi_dsi_pixel_format format;
    long unsigned int mode_flags;
    long unsigned int hs_rate;
    long unsigned int lp_rate;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct mipi_dsi_device {
    struct mipi_dsi_host *host;
    struct device dev;
    char name[20];
    unsigned int channel;
    unsigned int lanes;
    enum mipi_dsi_pixel_format format;
    long unsigned int mode_flags;
    long unsigned int hs_rate;
    long unsigned int lp_rate;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct mipi_dsi_device {
    struct mipi_dsi_host *host;
    struct device dev;
    char name[20];
    unsigned int channel;
    unsigned int lanes;
    enum mipi_dsi_pixel_format format;
    long unsigned int mode_flags;
    long unsigned int hs_rate;
    long unsigned int lp_rate;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct mipi_dsi_device {
    struct mipi_dsi_host *host;
    struct device dev;
    char name[20];
    unsigned int channel;
    unsigned int lanes;
    enum mipi_dsi_pixel_format format;
    long unsigned int mode_flags;
    long unsigned int hs_rate;
    long unsigned int lp_rate;
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
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>char name[20]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int hs_rate</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int lp_rate</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct drm_dsc_config *dsc</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool attached</code>
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
