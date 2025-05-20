# Struct: <code>fb_fix_screeninfo</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct fb_fix_screeninfo {
    char id[16];
    long unsigned int smem_start;
    __u32 smem_len;
    __u32 type;
    __u32 type_aux;
    __u32 visual;
    __u16 xpanstep;
    __u16 ypanstep;
    __u16 ywrapstep;
    __u32 line_length;
    long unsigned int mmio_start;
    __u32 mmio_len;
    __u32 accel;
    __u16 capabilities;
    __u16 reserved[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct fb_fix_screeninfo {
    char id[16];
    long unsigned int smem_start;
    __u32 smem_len;
    __u32 type;
    __u32 type_aux;
    __u32 visual;
    __u16 xpanstep;
    __u16 ypanstep;
    __u16 ywrapstep;
    __u32 line_length;
    long unsigned int mmio_start;
    __u32 mmio_len;
    __u32 accel;
    __u16 capabilities;
    __u16 reserved[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct fb_fix_screeninfo {
    char id[16];
    long unsigned int smem_start;
    __u32 smem_len;
    __u32 type;
    __u32 type_aux;
    __u32 visual;
    __u16 xpanstep;
    __u16 ypanstep;
    __u16 ywrapstep;
    __u32 line_length;
    long unsigned int mmio_start;
    __u32 mmio_len;
    __u32 accel;
    __u16 capabilities;
    __u16 reserved[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct fb_fix_screeninfo {
    char id[16];
    long unsigned int smem_start;
    __u32 smem_len;
    __u32 type;
    __u32 type_aux;
    __u32 visual;
    __u16 xpanstep;
    __u16 ypanstep;
    __u16 ywrapstep;
    __u32 line_length;
    long unsigned int mmio_start;
    __u32 mmio_len;
    __u32 accel;
    __u16 capabilities;
    __u16 reserved[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct fb_fix_screeninfo {
    char id[16];
    long unsigned int smem_start;
    __u32 smem_len;
    __u32 type;
    __u32 type_aux;
    __u32 visual;
    __u16 xpanstep;
    __u16 ypanstep;
    __u16 ywrapstep;
    __u32 line_length;
    long unsigned int mmio_start;
    __u32 mmio_len;
    __u32 accel;
    __u16 capabilities;
    __u16 reserved[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct fb_fix_screeninfo {
    char id[16];
    long unsigned int smem_start;
    __u32 smem_len;
    __u32 type;
    __u32 type_aux;
    __u32 visual;
    __u16 xpanstep;
    __u16 ypanstep;
    __u16 ywrapstep;
    __u32 line_length;
    long unsigned int mmio_start;
    __u32 mmio_len;
    __u32 accel;
    __u16 capabilities;
    __u16 reserved[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct fb_fix_screeninfo {
    char id[16];
    long unsigned int smem_start;
    __u32 smem_len;
    __u32 type;
    __u32 type_aux;
    __u32 visual;
    __u16 xpanstep;
    __u16 ypanstep;
    __u16 ywrapstep;
    __u32 line_length;
    long unsigned int mmio_start;
    __u32 mmio_len;
    __u32 accel;
    __u16 capabilities;
    __u16 reserved[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct fb_fix_screeninfo {
    char id[16];
    long unsigned int smem_start;
    __u32 smem_len;
    __u32 type;
    __u32 type_aux;
    __u32 visual;
    __u16 xpanstep;
    __u16 ypanstep;
    __u16 ywrapstep;
    __u32 line_length;
    long unsigned int mmio_start;
    __u32 mmio_len;
    __u32 accel;
    __u16 capabilities;
    __u16 reserved[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct fb_fix_screeninfo {
    char id[16];
    long unsigned int smem_start;
    __u32 smem_len;
    __u32 type;
    __u32 type_aux;
    __u32 visual;
    __u16 xpanstep;
    __u16 ypanstep;
    __u16 ywrapstep;
    __u32 line_length;
    long unsigned int mmio_start;
    __u32 mmio_len;
    __u32 accel;
    __u16 capabilities;
    __u16 reserved[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct fb_fix_screeninfo {
    char id[16];
    long unsigned int smem_start;
    __u32 smem_len;
    __u32 type;
    __u32 type_aux;
    __u32 visual;
    __u16 xpanstep;
    __u16 ypanstep;
    __u16 ywrapstep;
    __u32 line_length;
    long unsigned int mmio_start;
    __u32 mmio_len;
    __u32 accel;
    __u16 capabilities;
    __u16 reserved[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct fb_fix_screeninfo {
    char id[16];
    long unsigned int smem_start;
    __u32 smem_len;
    __u32 type;
    __u32 type_aux;
    __u32 visual;
    __u16 xpanstep;
    __u16 ypanstep;
    __u16 ywrapstep;
    __u32 line_length;
    long unsigned int mmio_start;
    __u32 mmio_len;
    __u32 accel;
    __u16 capabilities;
    __u16 reserved[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct fb_fix_screeninfo {
    char id[16];
    long unsigned int smem_start;
    __u32 smem_len;
    __u32 type;
    __u32 type_aux;
    __u32 visual;
    __u16 xpanstep;
    __u16 ypanstep;
    __u16 ywrapstep;
    __u32 line_length;
    long unsigned int mmio_start;
    __u32 mmio_len;
    __u32 accel;
    __u16 capabilities;
    __u16 reserved[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct fb_fix_screeninfo {
    char id[16];
    long unsigned int smem_start;
    __u32 smem_len;
    __u32 type;
    __u32 type_aux;
    __u32 visual;
    __u16 xpanstep;
    __u16 ypanstep;
    __u16 ywrapstep;
    __u32 line_length;
    long unsigned int mmio_start;
    __u32 mmio_len;
    __u32 accel;
    __u16 capabilities;
    __u16 reserved[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct fb_fix_screeninfo {
    char id[16];
    long unsigned int smem_start;
    __u32 smem_len;
    __u32 type;
    __u32 type_aux;
    __u32 visual;
    __u16 xpanstep;
    __u16 ypanstep;
    __u16 ywrapstep;
    __u32 line_length;
    long unsigned int mmio_start;
    __u32 mmio_len;
    __u32 accel;
    __u16 capabilities;
    __u16 reserved[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct fb_fix_screeninfo {
    char id[16];
    long unsigned int smem_start;
    __u32 smem_len;
    __u32 type;
    __u32 type_aux;
    __u32 visual;
    __u16 xpanstep;
    __u16 ypanstep;
    __u16 ywrapstep;
    __u32 line_length;
    long unsigned int mmio_start;
    __u32 mmio_len;
    __u32 accel;
    __u16 capabilities;
    __u16 reserved[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct fb_fix_screeninfo {
    char id[16];
    long unsigned int smem_start;
    __u32 smem_len;
    __u32 type;
    __u32 type_aux;
    __u32 visual;
    __u16 xpanstep;
    __u16 ypanstep;
    __u16 ywrapstep;
    __u32 line_length;
    long unsigned int mmio_start;
    __u32 mmio_len;
    __u32 accel;
    __u16 capabilities;
    __u16 reserved[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct fb_fix_screeninfo {
    char id[16];
    long unsigned int smem_start;
    __u32 smem_len;
    __u32 type;
    __u32 type_aux;
    __u32 visual;
    __u16 xpanstep;
    __u16 ypanstep;
    __u16 ywrapstep;
    __u32 line_length;
    long unsigned int mmio_start;
    __u32 mmio_len;
    __u32 accel;
    __u16 capabilities;
    __u16 reserved[2];
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
struct fb_fix_screeninfo {
    char id[16];
    long unsigned int smem_start;
    __u32 smem_len;
    __u32 type;
    __u32 type_aux;
    __u32 visual;
    __u16 xpanstep;
    __u16 ypanstep;
    __u16 ywrapstep;
    __u32 line_length;
    long unsigned int mmio_start;
    __u32 mmio_len;
    __u32 accel;
    __u16 capabilities;
    __u16 reserved[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct fb_fix_screeninfo {
    char id[16];
    long unsigned int smem_start;
    __u32 smem_len;
    __u32 type;
    __u32 type_aux;
    __u32 visual;
    __u16 xpanstep;
    __u16 ypanstep;
    __u16 ywrapstep;
    __u32 line_length;
    long unsigned int mmio_start;
    __u32 mmio_len;
    __u32 accel;
    __u16 capabilities;
    __u16 reserved[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct fb_fix_screeninfo {
    char id[16];
    long unsigned int smem_start;
    __u32 smem_len;
    __u32 type;
    __u32 type_aux;
    __u32 visual;
    __u16 xpanstep;
    __u16 ypanstep;
    __u16 ywrapstep;
    __u32 line_length;
    long unsigned int mmio_start;
    __u32 mmio_len;
    __u32 accel;
    __u16 capabilities;
    __u16 reserved[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct fb_fix_screeninfo {
    char id[16];
    long unsigned int smem_start;
    __u32 smem_len;
    __u32 type;
    __u32 type_aux;
    __u32 visual;
    __u16 xpanstep;
    __u16 ypanstep;
    __u16 ywrapstep;
    __u32 line_length;
    long unsigned int mmio_start;
    __u32 mmio_len;
    __u32 accel;
    __u16 capabilities;
    __u16 reserved[2];
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
struct fb_fix_screeninfo {
    char id[16];
    long unsigned int smem_start;
    __u32 smem_len;
    __u32 type;
    __u32 type_aux;
    __u32 visual;
    __u16 xpanstep;
    __u16 ypanstep;
    __u16 ywrapstep;
    __u32 line_length;
    long unsigned int mmio_start;
    __u32 mmio_len;
    __u32 accel;
    __u16 capabilities;
    __u16 reserved[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct fb_fix_screeninfo {
    char id[16];
    long unsigned int smem_start;
    __u32 smem_len;
    __u32 type;
    __u32 type_aux;
    __u32 visual;
    __u16 xpanstep;
    __u16 ypanstep;
    __u16 ywrapstep;
    __u32 line_length;
    long unsigned int mmio_start;
    __u32 mmio_len;
    __u32 accel;
    __u16 capabilities;
    __u16 reserved[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct fb_fix_screeninfo {
    char id[16];
    long unsigned int smem_start;
    __u32 smem_len;
    __u32 type;
    __u32 type_aux;
    __u32 visual;
    __u16 xpanstep;
    __u16 ypanstep;
    __u16 ywrapstep;
    __u32 line_length;
    long unsigned int mmio_start;
    __u32 mmio_len;
    __u32 accel;
    __u16 capabilities;
    __u16 reserved[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct fb_fix_screeninfo {
    char id[16];
    long unsigned int smem_start;
    __u32 smem_len;
    __u32 type;
    __u32 type_aux;
    __u32 visual;
    __u16 xpanstep;
    __u16 ypanstep;
    __u16 ywrapstep;
    __u32 line_length;
    long unsigned int mmio_start;
    __u32 mmio_len;
    __u32 accel;
    __u16 capabilities;
    __u16 reserved[2];
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
