# Struct: <code>fb_monspecs</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct fb_monspecs {
    struct fb_chroma chroma;
    struct fb_videomode *modedb;
    __u8 manufacturer[4];
    __u8 monitor[14];
    __u8 serial_no[14];
    __u8 ascii[14];
    __u32 modedb_len;
    __u32 model;
    __u32 serial;
    __u32 year;
    __u32 week;
    __u32 hfmin;
    __u32 hfmax;
    __u32 dclkmin;
    __u32 dclkmax;
    __u16 input;
    __u16 dpms;
    __u16 signal;
    __u16 vfmin;
    __u16 vfmax;
    __u16 gamma;
    __u16 gtf;
    __u16 misc;
    __u8 version;
    __u8 revision;
    __u8 max_x;
    __u8 max_y;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct fb_monspecs {
    struct fb_chroma chroma;
    struct fb_videomode *modedb;
    __u8 manufacturer[4];
    __u8 monitor[14];
    __u8 serial_no[14];
    __u8 ascii[14];
    __u32 modedb_len;
    __u32 model;
    __u32 serial;
    __u32 year;
    __u32 week;
    __u32 hfmin;
    __u32 hfmax;
    __u32 dclkmin;
    __u32 dclkmax;
    __u16 input;
    __u16 dpms;
    __u16 signal;
    __u16 vfmin;
    __u16 vfmax;
    __u16 gamma;
    __u16 gtf;
    __u16 misc;
    __u8 version;
    __u8 revision;
    __u8 max_x;
    __u8 max_y;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct fb_monspecs {
    struct fb_chroma chroma;
    struct fb_videomode *modedb;
    __u8 manufacturer[4];
    __u8 monitor[14];
    __u8 serial_no[14];
    __u8 ascii[14];
    __u32 modedb_len;
    __u32 model;
    __u32 serial;
    __u32 year;
    __u32 week;
    __u32 hfmin;
    __u32 hfmax;
    __u32 dclkmin;
    __u32 dclkmax;
    __u16 input;
    __u16 dpms;
    __u16 signal;
    __u16 vfmin;
    __u16 vfmax;
    __u16 gamma;
    __u16 gtf;
    __u16 misc;
    __u8 version;
    __u8 revision;
    __u8 max_x;
    __u8 max_y;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct fb_monspecs {
    struct fb_chroma chroma;
    struct fb_videomode *modedb;
    __u8 manufacturer[4];
    __u8 monitor[14];
    __u8 serial_no[14];
    __u8 ascii[14];
    __u32 modedb_len;
    __u32 model;
    __u32 serial;
    __u32 year;
    __u32 week;
    __u32 hfmin;
    __u32 hfmax;
    __u32 dclkmin;
    __u32 dclkmax;
    __u16 input;
    __u16 dpms;
    __u16 signal;
    __u16 vfmin;
    __u16 vfmax;
    __u16 gamma;
    __u16 gtf;
    __u16 misc;
    __u8 version;
    __u8 revision;
    __u8 max_x;
    __u8 max_y;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct fb_monspecs {
    struct fb_chroma chroma;
    struct fb_videomode *modedb;
    __u8 manufacturer[4];
    __u8 monitor[14];
    __u8 serial_no[14];
    __u8 ascii[14];
    __u32 modedb_len;
    __u32 model;
    __u32 serial;
    __u32 year;
    __u32 week;
    __u32 hfmin;
    __u32 hfmax;
    __u32 dclkmin;
    __u32 dclkmax;
    __u16 input;
    __u16 dpms;
    __u16 signal;
    __u16 vfmin;
    __u16 vfmax;
    __u16 gamma;
    __u16 gtf;
    __u16 misc;
    __u8 version;
    __u8 revision;
    __u8 max_x;
    __u8 max_y;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct fb_monspecs {
    struct fb_chroma chroma;
    struct fb_videomode *modedb;
    __u8 manufacturer[4];
    __u8 monitor[14];
    __u8 serial_no[14];
    __u8 ascii[14];
    __u32 modedb_len;
    __u32 model;
    __u32 serial;
    __u32 year;
    __u32 week;
    __u32 hfmin;
    __u32 hfmax;
    __u32 dclkmin;
    __u32 dclkmax;
    __u16 input;
    __u16 dpms;
    __u16 signal;
    __u16 vfmin;
    __u16 vfmax;
    __u16 gamma;
    __u16 gtf;
    __u16 misc;
    __u8 version;
    __u8 revision;
    __u8 max_x;
    __u8 max_y;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct fb_monspecs {
    struct fb_chroma chroma;
    struct fb_videomode *modedb;
    __u8 manufacturer[4];
    __u8 monitor[14];
    __u8 serial_no[14];
    __u8 ascii[14];
    __u32 modedb_len;
    __u32 model;
    __u32 serial;
    __u32 year;
    __u32 week;
    __u32 hfmin;
    __u32 hfmax;
    __u32 dclkmin;
    __u32 dclkmax;
    __u16 input;
    __u16 dpms;
    __u16 signal;
    __u16 vfmin;
    __u16 vfmax;
    __u16 gamma;
    __u16 gtf;
    __u16 misc;
    __u8 version;
    __u8 revision;
    __u8 max_x;
    __u8 max_y;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct fb_monspecs {
    struct fb_chroma chroma;
    struct fb_videomode *modedb;
    __u8 manufacturer[4];
    __u8 monitor[14];
    __u8 serial_no[14];
    __u8 ascii[14];
    __u32 modedb_len;
    __u32 model;
    __u32 serial;
    __u32 year;
    __u32 week;
    __u32 hfmin;
    __u32 hfmax;
    __u32 dclkmin;
    __u32 dclkmax;
    __u16 input;
    __u16 dpms;
    __u16 signal;
    __u16 vfmin;
    __u16 vfmax;
    __u16 gamma;
    __u16 gtf;
    __u16 misc;
    __u8 version;
    __u8 revision;
    __u8 max_x;
    __u8 max_y;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct fb_monspecs {
    struct fb_chroma chroma;
    struct fb_videomode *modedb;
    __u8 manufacturer[4];
    __u8 monitor[14];
    __u8 serial_no[14];
    __u8 ascii[14];
    __u32 modedb_len;
    __u32 model;
    __u32 serial;
    __u32 year;
    __u32 week;
    __u32 hfmin;
    __u32 hfmax;
    __u32 dclkmin;
    __u32 dclkmax;
    __u16 input;
    __u16 dpms;
    __u16 signal;
    __u16 vfmin;
    __u16 vfmax;
    __u16 gamma;
    __u16 gtf;
    __u16 misc;
    __u8 version;
    __u8 revision;
    __u8 max_x;
    __u8 max_y;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct fb_monspecs {
    struct fb_chroma chroma;
    struct fb_videomode *modedb;
    __u8 manufacturer[4];
    __u8 monitor[14];
    __u8 serial_no[14];
    __u8 ascii[14];
    __u32 modedb_len;
    __u32 model;
    __u32 serial;
    __u32 year;
    __u32 week;
    __u32 hfmin;
    __u32 hfmax;
    __u32 dclkmin;
    __u32 dclkmax;
    __u16 input;
    __u16 dpms;
    __u16 signal;
    __u16 vfmin;
    __u16 vfmax;
    __u16 gamma;
    __u16 gtf;
    __u16 misc;
    __u8 version;
    __u8 revision;
    __u8 max_x;
    __u8 max_y;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct fb_monspecs {
    struct fb_chroma chroma;
    struct fb_videomode *modedb;
    __u8 manufacturer[4];
    __u8 monitor[14];
    __u8 serial_no[14];
    __u8 ascii[14];
    __u32 modedb_len;
    __u32 model;
    __u32 serial;
    __u32 year;
    __u32 week;
    __u32 hfmin;
    __u32 hfmax;
    __u32 dclkmin;
    __u32 dclkmax;
    __u16 input;
    __u16 dpms;
    __u16 signal;
    __u16 vfmin;
    __u16 vfmax;
    __u16 gamma;
    __u16 gtf;
    __u16 misc;
    __u8 version;
    __u8 revision;
    __u8 max_x;
    __u8 max_y;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct fb_monspecs {
    struct fb_chroma chroma;
    struct fb_videomode *modedb;
    __u8 manufacturer[4];
    __u8 monitor[14];
    __u8 serial_no[14];
    __u8 ascii[14];
    __u32 modedb_len;
    __u32 model;
    __u32 serial;
    __u32 year;
    __u32 week;
    __u32 hfmin;
    __u32 hfmax;
    __u32 dclkmin;
    __u32 dclkmax;
    __u16 input;
    __u16 dpms;
    __u16 signal;
    __u16 vfmin;
    __u16 vfmax;
    __u16 gamma;
    __u16 gtf;
    __u16 misc;
    __u8 version;
    __u8 revision;
    __u8 max_x;
    __u8 max_y;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct fb_monspecs {
    struct fb_chroma chroma;
    struct fb_videomode *modedb;
    __u8 manufacturer[4];
    __u8 monitor[14];
    __u8 serial_no[14];
    __u8 ascii[14];
    __u32 modedb_len;
    __u32 model;
    __u32 serial;
    __u32 year;
    __u32 week;
    __u32 hfmin;
    __u32 hfmax;
    __u32 dclkmin;
    __u32 dclkmax;
    __u16 input;
    __u16 dpms;
    __u16 signal;
    __u16 vfmin;
    __u16 vfmax;
    __u16 gamma;
    __u16 gtf;
    __u16 misc;
    __u8 version;
    __u8 revision;
    __u8 max_x;
    __u8 max_y;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct fb_monspecs {
    struct fb_chroma chroma;
    struct fb_videomode *modedb;
    __u8 manufacturer[4];
    __u8 monitor[14];
    __u8 serial_no[14];
    __u8 ascii[14];
    __u32 modedb_len;
    __u32 model;
    __u32 serial;
    __u32 year;
    __u32 week;
    __u32 hfmin;
    __u32 hfmax;
    __u32 dclkmin;
    __u32 dclkmax;
    __u16 input;
    __u16 dpms;
    __u16 signal;
    __u16 vfmin;
    __u16 vfmax;
    __u16 gamma;
    __u16 gtf;
    __u16 misc;
    __u8 version;
    __u8 revision;
    __u8 max_x;
    __u8 max_y;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct fb_monspecs {
    struct fb_chroma chroma;
    struct fb_videomode *modedb;
    __u8 manufacturer[4];
    __u8 monitor[14];
    __u8 serial_no[14];
    __u8 ascii[14];
    __u32 modedb_len;
    __u32 model;
    __u32 serial;
    __u32 year;
    __u32 week;
    __u32 hfmin;
    __u32 hfmax;
    __u32 dclkmin;
    __u32 dclkmax;
    __u16 input;
    __u16 dpms;
    __u16 signal;
    __u16 vfmin;
    __u16 vfmax;
    __u16 gamma;
    __u16 gtf;
    __u16 misc;
    __u8 version;
    __u8 revision;
    __u8 max_x;
    __u8 max_y;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct fb_monspecs {
    struct fb_chroma chroma;
    struct fb_videomode *modedb;
    __u8 manufacturer[4];
    __u8 monitor[14];
    __u8 serial_no[14];
    __u8 ascii[14];
    __u32 modedb_len;
    __u32 model;
    __u32 serial;
    __u32 year;
    __u32 week;
    __u32 hfmin;
    __u32 hfmax;
    __u32 dclkmin;
    __u32 dclkmax;
    __u16 input;
    __u16 dpms;
    __u16 signal;
    __u16 vfmin;
    __u16 vfmax;
    __u16 gamma;
    __u16 gtf;
    __u16 misc;
    __u8 version;
    __u8 revision;
    __u8 max_x;
    __u8 max_y;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct fb_monspecs {
    struct fb_chroma chroma;
    struct fb_videomode *modedb;
    __u8 manufacturer[4];
    __u8 monitor[14];
    __u8 serial_no[14];
    __u8 ascii[14];
    __u32 modedb_len;
    __u32 model;
    __u32 serial;
    __u32 year;
    __u32 week;
    __u32 hfmin;
    __u32 hfmax;
    __u32 dclkmin;
    __u32 dclkmax;
    __u16 input;
    __u16 dpms;
    __u16 signal;
    __u16 vfmin;
    __u16 vfmax;
    __u16 gamma;
    __u16 gtf;
    __u16 misc;
    __u8 version;
    __u8 revision;
    __u8 max_x;
    __u8 max_y;
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
struct fb_monspecs {
    struct fb_chroma chroma;
    struct fb_videomode *modedb;
    __u8 manufacturer[4];
    __u8 monitor[14];
    __u8 serial_no[14];
    __u8 ascii[14];
    __u32 modedb_len;
    __u32 model;
    __u32 serial;
    __u32 year;
    __u32 week;
    __u32 hfmin;
    __u32 hfmax;
    __u32 dclkmin;
    __u32 dclkmax;
    __u16 input;
    __u16 dpms;
    __u16 signal;
    __u16 vfmin;
    __u16 vfmax;
    __u16 gamma;
    __u16 gtf;
    __u16 misc;
    __u8 version;
    __u8 revision;
    __u8 max_x;
    __u8 max_y;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct fb_monspecs {
    struct fb_chroma chroma;
    struct fb_videomode *modedb;
    __u8 manufacturer[4];
    __u8 monitor[14];
    __u8 serial_no[14];
    __u8 ascii[14];
    __u32 modedb_len;
    __u32 model;
    __u32 serial;
    __u32 year;
    __u32 week;
    __u32 hfmin;
    __u32 hfmax;
    __u32 dclkmin;
    __u32 dclkmax;
    __u16 input;
    __u16 dpms;
    __u16 signal;
    __u16 vfmin;
    __u16 vfmax;
    __u16 gamma;
    __u16 gtf;
    __u16 misc;
    __u8 version;
    __u8 revision;
    __u8 max_x;
    __u8 max_y;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct fb_monspecs {
    struct fb_chroma chroma;
    struct fb_videomode *modedb;
    __u8 manufacturer[4];
    __u8 monitor[14];
    __u8 serial_no[14];
    __u8 ascii[14];
    __u32 modedb_len;
    __u32 model;
    __u32 serial;
    __u32 year;
    __u32 week;
    __u32 hfmin;
    __u32 hfmax;
    __u32 dclkmin;
    __u32 dclkmax;
    __u16 input;
    __u16 dpms;
    __u16 signal;
    __u16 vfmin;
    __u16 vfmax;
    __u16 gamma;
    __u16 gtf;
    __u16 misc;
    __u8 version;
    __u8 revision;
    __u8 max_x;
    __u8 max_y;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct fb_monspecs {
    struct fb_chroma chroma;
    struct fb_videomode *modedb;
    __u8 manufacturer[4];
    __u8 monitor[14];
    __u8 serial_no[14];
    __u8 ascii[14];
    __u32 modedb_len;
    __u32 model;
    __u32 serial;
    __u32 year;
    __u32 week;
    __u32 hfmin;
    __u32 hfmax;
    __u32 dclkmin;
    __u32 dclkmax;
    __u16 input;
    __u16 dpms;
    __u16 signal;
    __u16 vfmin;
    __u16 vfmax;
    __u16 gamma;
    __u16 gtf;
    __u16 misc;
    __u8 version;
    __u8 revision;
    __u8 max_x;
    __u8 max_y;
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
struct fb_monspecs {
    struct fb_chroma chroma;
    struct fb_videomode *modedb;
    __u8 manufacturer[4];
    __u8 monitor[14];
    __u8 serial_no[14];
    __u8 ascii[14];
    __u32 modedb_len;
    __u32 model;
    __u32 serial;
    __u32 year;
    __u32 week;
    __u32 hfmin;
    __u32 hfmax;
    __u32 dclkmin;
    __u32 dclkmax;
    __u16 input;
    __u16 dpms;
    __u16 signal;
    __u16 vfmin;
    __u16 vfmax;
    __u16 gamma;
    __u16 gtf;
    __u16 misc;
    __u8 version;
    __u8 revision;
    __u8 max_x;
    __u8 max_y;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct fb_monspecs {
    struct fb_chroma chroma;
    struct fb_videomode *modedb;
    __u8 manufacturer[4];
    __u8 monitor[14];
    __u8 serial_no[14];
    __u8 ascii[14];
    __u32 modedb_len;
    __u32 model;
    __u32 serial;
    __u32 year;
    __u32 week;
    __u32 hfmin;
    __u32 hfmax;
    __u32 dclkmin;
    __u32 dclkmax;
    __u16 input;
    __u16 dpms;
    __u16 signal;
    __u16 vfmin;
    __u16 vfmax;
    __u16 gamma;
    __u16 gtf;
    __u16 misc;
    __u8 version;
    __u8 revision;
    __u8 max_x;
    __u8 max_y;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct fb_monspecs {
    struct fb_chroma chroma;
    struct fb_videomode *modedb;
    __u8 manufacturer[4];
    __u8 monitor[14];
    __u8 serial_no[14];
    __u8 ascii[14];
    __u32 modedb_len;
    __u32 model;
    __u32 serial;
    __u32 year;
    __u32 week;
    __u32 hfmin;
    __u32 hfmax;
    __u32 dclkmin;
    __u32 dclkmax;
    __u16 input;
    __u16 dpms;
    __u16 signal;
    __u16 vfmin;
    __u16 vfmax;
    __u16 gamma;
    __u16 gtf;
    __u16 misc;
    __u8 version;
    __u8 revision;
    __u8 max_x;
    __u8 max_y;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct fb_monspecs {
    struct fb_chroma chroma;
    struct fb_videomode *modedb;
    __u8 manufacturer[4];
    __u8 monitor[14];
    __u8 serial_no[14];
    __u8 ascii[14];
    __u32 modedb_len;
    __u32 model;
    __u32 serial;
    __u32 year;
    __u32 week;
    __u32 hfmin;
    __u32 hfmax;
    __u32 dclkmin;
    __u32 dclkmax;
    __u16 input;
    __u16 dpms;
    __u16 signal;
    __u16 vfmin;
    __u16 vfmax;
    __u16 gamma;
    __u16 gtf;
    __u16 misc;
    __u8 version;
    __u8 revision;
    __u8 max_x;
    __u8 max_y;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.4</code> and <code>4.8</code> ✅
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
No changes between <code>4.18</code> and <code>5.0</code> ✅
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
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
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
