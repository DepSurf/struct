# Struct: <code>fb_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct fb_ops {
    struct module *owner;
    int (*fb_open)(struct fb_info *, int);
    int (*fb_release)(struct fb_info *, int);
    ssize_t (*fb_read)(struct fb_info *, char *, size_t, loff_t *);
    ssize_t (*fb_write)(struct fb_info *, const char *, size_t, loff_t *);
    int (*fb_check_var)(struct fb_var_screeninfo *, struct fb_info *);
    int (*fb_set_par)(struct fb_info *);
    int (*fb_setcolreg)(unsigned int, unsigned int, unsigned int, unsigned int, unsigned int, struct fb_info *);
    int (*fb_setcmap)(struct fb_cmap *, struct fb_info *);
    int (*fb_blank)(int, struct fb_info *);
    int (*fb_pan_display)(struct fb_var_screeninfo *, struct fb_info *);
    void (*fb_fillrect)(struct fb_info *, const struct fb_fillrect *);
    void (*fb_copyarea)(struct fb_info *, const struct fb_copyarea *);
    void (*fb_imageblit)(struct fb_info *, const struct fb_image *);
    int (*fb_cursor)(struct fb_info *, struct fb_cursor *);
    void (*fb_rotate)(struct fb_info *, int);
    int (*fb_sync)(struct fb_info *);
    int (*fb_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_compat_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_mmap)(struct fb_info *, struct vm_area_struct *);
    void (*fb_get_caps)(struct fb_info *, struct fb_blit_caps *, struct fb_var_screeninfo *);
    void (*fb_destroy)(struct fb_info *);
    int (*fb_debug_enter)(struct fb_info *);
    int (*fb_debug_leave)(struct fb_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct fb_ops {
    struct module *owner;
    int (*fb_open)(struct fb_info *, int);
    int (*fb_release)(struct fb_info *, int);
    ssize_t (*fb_read)(struct fb_info *, char *, size_t, loff_t *);
    ssize_t (*fb_write)(struct fb_info *, const char *, size_t, loff_t *);
    int (*fb_check_var)(struct fb_var_screeninfo *, struct fb_info *);
    int (*fb_set_par)(struct fb_info *);
    int (*fb_setcolreg)(unsigned int, unsigned int, unsigned int, unsigned int, unsigned int, struct fb_info *);
    int (*fb_setcmap)(struct fb_cmap *, struct fb_info *);
    int (*fb_blank)(int, struct fb_info *);
    int (*fb_pan_display)(struct fb_var_screeninfo *, struct fb_info *);
    void (*fb_fillrect)(struct fb_info *, const struct fb_fillrect *);
    void (*fb_copyarea)(struct fb_info *, const struct fb_copyarea *);
    void (*fb_imageblit)(struct fb_info *, const struct fb_image *);
    int (*fb_cursor)(struct fb_info *, struct fb_cursor *);
    int (*fb_sync)(struct fb_info *);
    int (*fb_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_compat_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_mmap)(struct fb_info *, struct vm_area_struct *);
    void (*fb_get_caps)(struct fb_info *, struct fb_blit_caps *, struct fb_var_screeninfo *);
    void (*fb_destroy)(struct fb_info *);
    int (*fb_debug_enter)(struct fb_info *);
    int (*fb_debug_leave)(struct fb_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct fb_ops {
    struct module *owner;
    int (*fb_open)(struct fb_info *, int);
    int (*fb_release)(struct fb_info *, int);
    ssize_t (*fb_read)(struct fb_info *, char *, size_t, loff_t *);
    ssize_t (*fb_write)(struct fb_info *, const char *, size_t, loff_t *);
    int (*fb_check_var)(struct fb_var_screeninfo *, struct fb_info *);
    int (*fb_set_par)(struct fb_info *);
    int (*fb_setcolreg)(unsigned int, unsigned int, unsigned int, unsigned int, unsigned int, struct fb_info *);
    int (*fb_setcmap)(struct fb_cmap *, struct fb_info *);
    int (*fb_blank)(int, struct fb_info *);
    int (*fb_pan_display)(struct fb_var_screeninfo *, struct fb_info *);
    void (*fb_fillrect)(struct fb_info *, const struct fb_fillrect *);
    void (*fb_copyarea)(struct fb_info *, const struct fb_copyarea *);
    void (*fb_imageblit)(struct fb_info *, const struct fb_image *);
    int (*fb_cursor)(struct fb_info *, struct fb_cursor *);
    int (*fb_sync)(struct fb_info *);
    int (*fb_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_compat_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_mmap)(struct fb_info *, struct vm_area_struct *);
    void (*fb_get_caps)(struct fb_info *, struct fb_blit_caps *, struct fb_var_screeninfo *);
    void (*fb_destroy)(struct fb_info *);
    int (*fb_debug_enter)(struct fb_info *);
    int (*fb_debug_leave)(struct fb_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct fb_ops {
    struct module *owner;
    int (*fb_open)(struct fb_info *, int);
    int (*fb_release)(struct fb_info *, int);
    ssize_t (*fb_read)(struct fb_info *, char *, size_t, loff_t *);
    ssize_t (*fb_write)(struct fb_info *, const char *, size_t, loff_t *);
    int (*fb_check_var)(struct fb_var_screeninfo *, struct fb_info *);
    int (*fb_set_par)(struct fb_info *);
    int (*fb_setcolreg)(unsigned int, unsigned int, unsigned int, unsigned int, unsigned int, struct fb_info *);
    int (*fb_setcmap)(struct fb_cmap *, struct fb_info *);
    int (*fb_blank)(int, struct fb_info *);
    int (*fb_pan_display)(struct fb_var_screeninfo *, struct fb_info *);
    void (*fb_fillrect)(struct fb_info *, const struct fb_fillrect *);
    void (*fb_copyarea)(struct fb_info *, const struct fb_copyarea *);
    void (*fb_imageblit)(struct fb_info *, const struct fb_image *);
    int (*fb_cursor)(struct fb_info *, struct fb_cursor *);
    int (*fb_sync)(struct fb_info *);
    int (*fb_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_compat_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_mmap)(struct fb_info *, struct vm_area_struct *);
    void (*fb_get_caps)(struct fb_info *, struct fb_blit_caps *, struct fb_var_screeninfo *);
    void (*fb_destroy)(struct fb_info *);
    int (*fb_debug_enter)(struct fb_info *);
    int (*fb_debug_leave)(struct fb_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct fb_ops {
    struct module *owner;
    int (*fb_open)(struct fb_info *, int);
    int (*fb_release)(struct fb_info *, int);
    ssize_t (*fb_read)(struct fb_info *, char *, size_t, loff_t *);
    ssize_t (*fb_write)(struct fb_info *, const char *, size_t, loff_t *);
    int (*fb_check_var)(struct fb_var_screeninfo *, struct fb_info *);
    int (*fb_set_par)(struct fb_info *);
    int (*fb_setcolreg)(unsigned int, unsigned int, unsigned int, unsigned int, unsigned int, struct fb_info *);
    int (*fb_setcmap)(struct fb_cmap *, struct fb_info *);
    int (*fb_blank)(int, struct fb_info *);
    int (*fb_pan_display)(struct fb_var_screeninfo *, struct fb_info *);
    void (*fb_fillrect)(struct fb_info *, const struct fb_fillrect *);
    void (*fb_copyarea)(struct fb_info *, const struct fb_copyarea *);
    void (*fb_imageblit)(struct fb_info *, const struct fb_image *);
    int (*fb_cursor)(struct fb_info *, struct fb_cursor *);
    int (*fb_sync)(struct fb_info *);
    int (*fb_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_compat_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_mmap)(struct fb_info *, struct vm_area_struct *);
    void (*fb_get_caps)(struct fb_info *, struct fb_blit_caps *, struct fb_var_screeninfo *);
    void (*fb_destroy)(struct fb_info *);
    int (*fb_debug_enter)(struct fb_info *);
    int (*fb_debug_leave)(struct fb_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct fb_ops {
    struct module *owner;
    int (*fb_open)(struct fb_info *, int);
    int (*fb_release)(struct fb_info *, int);
    ssize_t (*fb_read)(struct fb_info *, char *, size_t, loff_t *);
    ssize_t (*fb_write)(struct fb_info *, const char *, size_t, loff_t *);
    int (*fb_check_var)(struct fb_var_screeninfo *, struct fb_info *);
    int (*fb_set_par)(struct fb_info *);
    int (*fb_setcolreg)(unsigned int, unsigned int, unsigned int, unsigned int, unsigned int, struct fb_info *);
    int (*fb_setcmap)(struct fb_cmap *, struct fb_info *);
    int (*fb_blank)(int, struct fb_info *);
    int (*fb_pan_display)(struct fb_var_screeninfo *, struct fb_info *);
    void (*fb_fillrect)(struct fb_info *, const struct fb_fillrect *);
    void (*fb_copyarea)(struct fb_info *, const struct fb_copyarea *);
    void (*fb_imageblit)(struct fb_info *, const struct fb_image *);
    int (*fb_cursor)(struct fb_info *, struct fb_cursor *);
    int (*fb_sync)(struct fb_info *);
    int (*fb_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_compat_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_mmap)(struct fb_info *, struct vm_area_struct *);
    void (*fb_get_caps)(struct fb_info *, struct fb_blit_caps *, struct fb_var_screeninfo *);
    void (*fb_destroy)(struct fb_info *);
    int (*fb_debug_enter)(struct fb_info *);
    int (*fb_debug_leave)(struct fb_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct fb_ops {
    struct module *owner;
    int (*fb_open)(struct fb_info *, int);
    int (*fb_release)(struct fb_info *, int);
    ssize_t (*fb_read)(struct fb_info *, char *, size_t, loff_t *);
    ssize_t (*fb_write)(struct fb_info *, const char *, size_t, loff_t *);
    int (*fb_check_var)(struct fb_var_screeninfo *, struct fb_info *);
    int (*fb_set_par)(struct fb_info *);
    int (*fb_setcolreg)(unsigned int, unsigned int, unsigned int, unsigned int, unsigned int, struct fb_info *);
    int (*fb_setcmap)(struct fb_cmap *, struct fb_info *);
    int (*fb_blank)(int, struct fb_info *);
    int (*fb_pan_display)(struct fb_var_screeninfo *, struct fb_info *);
    void (*fb_fillrect)(struct fb_info *, const struct fb_fillrect *);
    void (*fb_copyarea)(struct fb_info *, const struct fb_copyarea *);
    void (*fb_imageblit)(struct fb_info *, const struct fb_image *);
    int (*fb_cursor)(struct fb_info *, struct fb_cursor *);
    int (*fb_sync)(struct fb_info *);
    int (*fb_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_compat_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_mmap)(struct fb_info *, struct vm_area_struct *);
    void (*fb_get_caps)(struct fb_info *, struct fb_blit_caps *, struct fb_var_screeninfo *);
    void (*fb_destroy)(struct fb_info *);
    int (*fb_debug_enter)(struct fb_info *);
    int (*fb_debug_leave)(struct fb_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct fb_ops {
    struct module *owner;
    int (*fb_open)(struct fb_info *, int);
    int (*fb_release)(struct fb_info *, int);
    ssize_t (*fb_read)(struct fb_info *, char *, size_t, loff_t *);
    ssize_t (*fb_write)(struct fb_info *, const char *, size_t, loff_t *);
    int (*fb_check_var)(struct fb_var_screeninfo *, struct fb_info *);
    int (*fb_set_par)(struct fb_info *);
    int (*fb_setcolreg)(unsigned int, unsigned int, unsigned int, unsigned int, unsigned int, struct fb_info *);
    int (*fb_setcmap)(struct fb_cmap *, struct fb_info *);
    int (*fb_blank)(int, struct fb_info *);
    int (*fb_pan_display)(struct fb_var_screeninfo *, struct fb_info *);
    void (*fb_fillrect)(struct fb_info *, const struct fb_fillrect *);
    void (*fb_copyarea)(struct fb_info *, const struct fb_copyarea *);
    void (*fb_imageblit)(struct fb_info *, const struct fb_image *);
    int (*fb_cursor)(struct fb_info *, struct fb_cursor *);
    int (*fb_sync)(struct fb_info *);
    int (*fb_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_compat_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_mmap)(struct fb_info *, struct vm_area_struct *);
    void (*fb_get_caps)(struct fb_info *, struct fb_blit_caps *, struct fb_var_screeninfo *);
    void (*fb_destroy)(struct fb_info *);
    int (*fb_debug_enter)(struct fb_info *);
    int (*fb_debug_leave)(struct fb_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct fb_ops {
    struct module *owner;
    int (*fb_open)(struct fb_info *, int);
    int (*fb_release)(struct fb_info *, int);
    ssize_t (*fb_read)(struct fb_info *, char *, size_t, loff_t *);
    ssize_t (*fb_write)(struct fb_info *, const char *, size_t, loff_t *);
    int (*fb_check_var)(struct fb_var_screeninfo *, struct fb_info *);
    int (*fb_set_par)(struct fb_info *);
    int (*fb_setcolreg)(unsigned int, unsigned int, unsigned int, unsigned int, unsigned int, struct fb_info *);
    int (*fb_setcmap)(struct fb_cmap *, struct fb_info *);
    int (*fb_blank)(int, struct fb_info *);
    int (*fb_pan_display)(struct fb_var_screeninfo *, struct fb_info *);
    void (*fb_fillrect)(struct fb_info *, const struct fb_fillrect *);
    void (*fb_copyarea)(struct fb_info *, const struct fb_copyarea *);
    void (*fb_imageblit)(struct fb_info *, const struct fb_image *);
    int (*fb_cursor)(struct fb_info *, struct fb_cursor *);
    int (*fb_sync)(struct fb_info *);
    int (*fb_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_compat_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_mmap)(struct fb_info *, struct vm_area_struct *);
    void (*fb_get_caps)(struct fb_info *, struct fb_blit_caps *, struct fb_var_screeninfo *);
    void (*fb_destroy)(struct fb_info *);
    int (*fb_debug_enter)(struct fb_info *);
    int (*fb_debug_leave)(struct fb_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct fb_ops {
    struct module *owner;
    int (*fb_open)(struct fb_info *, int);
    int (*fb_release)(struct fb_info *, int);
    ssize_t (*fb_read)(struct fb_info *, char *, size_t, loff_t *);
    ssize_t (*fb_write)(struct fb_info *, const char *, size_t, loff_t *);
    int (*fb_check_var)(struct fb_var_screeninfo *, struct fb_info *);
    int (*fb_set_par)(struct fb_info *);
    int (*fb_setcolreg)(unsigned int, unsigned int, unsigned int, unsigned int, unsigned int, struct fb_info *);
    int (*fb_setcmap)(struct fb_cmap *, struct fb_info *);
    int (*fb_blank)(int, struct fb_info *);
    int (*fb_pan_display)(struct fb_var_screeninfo *, struct fb_info *);
    void (*fb_fillrect)(struct fb_info *, const struct fb_fillrect *);
    void (*fb_copyarea)(struct fb_info *, const struct fb_copyarea *);
    void (*fb_imageblit)(struct fb_info *, const struct fb_image *);
    int (*fb_cursor)(struct fb_info *, struct fb_cursor *);
    int (*fb_sync)(struct fb_info *);
    int (*fb_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_compat_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_mmap)(struct fb_info *, struct vm_area_struct *);
    void (*fb_get_caps)(struct fb_info *, struct fb_blit_caps *, struct fb_var_screeninfo *);
    void (*fb_destroy)(struct fb_info *);
    int (*fb_debug_enter)(struct fb_info *);
    int (*fb_debug_leave)(struct fb_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct fb_ops {
    struct module *owner;
    int (*fb_open)(struct fb_info *, int);
    int (*fb_release)(struct fb_info *, int);
    ssize_t (*fb_read)(struct fb_info *, char *, size_t, loff_t *);
    ssize_t (*fb_write)(struct fb_info *, const char *, size_t, loff_t *);
    int (*fb_check_var)(struct fb_var_screeninfo *, struct fb_info *);
    int (*fb_set_par)(struct fb_info *);
    int (*fb_setcolreg)(unsigned int, unsigned int, unsigned int, unsigned int, unsigned int, struct fb_info *);
    int (*fb_setcmap)(struct fb_cmap *, struct fb_info *);
    int (*fb_blank)(int, struct fb_info *);
    int (*fb_pan_display)(struct fb_var_screeninfo *, struct fb_info *);
    void (*fb_fillrect)(struct fb_info *, const struct fb_fillrect *);
    void (*fb_copyarea)(struct fb_info *, const struct fb_copyarea *);
    void (*fb_imageblit)(struct fb_info *, const struct fb_image *);
    int (*fb_cursor)(struct fb_info *, struct fb_cursor *);
    int (*fb_sync)(struct fb_info *);
    int (*fb_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_compat_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_mmap)(struct fb_info *, struct vm_area_struct *);
    void (*fb_get_caps)(struct fb_info *, struct fb_blit_caps *, struct fb_var_screeninfo *);
    void (*fb_destroy)(struct fb_info *);
    int (*fb_debug_enter)(struct fb_info *);
    int (*fb_debug_leave)(struct fb_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct fb_ops {
    struct module *owner;
    int (*fb_open)(struct fb_info *, int);
    int (*fb_release)(struct fb_info *, int);
    ssize_t (*fb_read)(struct fb_info *, char *, size_t, loff_t *);
    ssize_t (*fb_write)(struct fb_info *, const char *, size_t, loff_t *);
    int (*fb_check_var)(struct fb_var_screeninfo *, struct fb_info *);
    int (*fb_set_par)(struct fb_info *);
    int (*fb_setcolreg)(unsigned int, unsigned int, unsigned int, unsigned int, unsigned int, struct fb_info *);
    int (*fb_setcmap)(struct fb_cmap *, struct fb_info *);
    int (*fb_blank)(int, struct fb_info *);
    int (*fb_pan_display)(struct fb_var_screeninfo *, struct fb_info *);
    void (*fb_fillrect)(struct fb_info *, const struct fb_fillrect *);
    void (*fb_copyarea)(struct fb_info *, const struct fb_copyarea *);
    void (*fb_imageblit)(struct fb_info *, const struct fb_image *);
    int (*fb_cursor)(struct fb_info *, struct fb_cursor *);
    int (*fb_sync)(struct fb_info *);
    int (*fb_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_compat_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_mmap)(struct fb_info *, struct vm_area_struct *);
    void (*fb_get_caps)(struct fb_info *, struct fb_blit_caps *, struct fb_var_screeninfo *);
    void (*fb_destroy)(struct fb_info *);
    int (*fb_debug_enter)(struct fb_info *);
    int (*fb_debug_leave)(struct fb_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct fb_ops {
    struct module *owner;
    int (*fb_open)(struct fb_info *, int);
    int (*fb_release)(struct fb_info *, int);
    ssize_t (*fb_read)(struct fb_info *, char *, size_t, loff_t *);
    ssize_t (*fb_write)(struct fb_info *, const char *, size_t, loff_t *);
    int (*fb_check_var)(struct fb_var_screeninfo *, struct fb_info *);
    int (*fb_set_par)(struct fb_info *);
    int (*fb_setcolreg)(unsigned int, unsigned int, unsigned int, unsigned int, unsigned int, struct fb_info *);
    int (*fb_setcmap)(struct fb_cmap *, struct fb_info *);
    int (*fb_blank)(int, struct fb_info *);
    int (*fb_pan_display)(struct fb_var_screeninfo *, struct fb_info *);
    void (*fb_fillrect)(struct fb_info *, const struct fb_fillrect *);
    void (*fb_copyarea)(struct fb_info *, const struct fb_copyarea *);
    void (*fb_imageblit)(struct fb_info *, const struct fb_image *);
    int (*fb_cursor)(struct fb_info *, struct fb_cursor *);
    int (*fb_sync)(struct fb_info *);
    int (*fb_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_compat_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_mmap)(struct fb_info *, struct vm_area_struct *);
    void (*fb_get_caps)(struct fb_info *, struct fb_blit_caps *, struct fb_var_screeninfo *);
    void (*fb_destroy)(struct fb_info *);
    int (*fb_debug_enter)(struct fb_info *);
    int (*fb_debug_leave)(struct fb_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct fb_ops {
    struct module *owner;
    int (*fb_open)(struct fb_info *, int);
    int (*fb_release)(struct fb_info *, int);
    ssize_t (*fb_read)(struct fb_info *, char *, size_t, loff_t *);
    ssize_t (*fb_write)(struct fb_info *, const char *, size_t, loff_t *);
    int (*fb_check_var)(struct fb_var_screeninfo *, struct fb_info *);
    int (*fb_set_par)(struct fb_info *);
    int (*fb_setcolreg)(unsigned int, unsigned int, unsigned int, unsigned int, unsigned int, struct fb_info *);
    int (*fb_setcmap)(struct fb_cmap *, struct fb_info *);
    int (*fb_blank)(int, struct fb_info *);
    int (*fb_pan_display)(struct fb_var_screeninfo *, struct fb_info *);
    void (*fb_fillrect)(struct fb_info *, const struct fb_fillrect *);
    void (*fb_copyarea)(struct fb_info *, const struct fb_copyarea *);
    void (*fb_imageblit)(struct fb_info *, const struct fb_image *);
    int (*fb_cursor)(struct fb_info *, struct fb_cursor *);
    int (*fb_sync)(struct fb_info *);
    int (*fb_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_compat_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_mmap)(struct fb_info *, struct vm_area_struct *);
    void (*fb_get_caps)(struct fb_info *, struct fb_blit_caps *, struct fb_var_screeninfo *);
    void (*fb_destroy)(struct fb_info *);
    int (*fb_debug_enter)(struct fb_info *);
    int (*fb_debug_leave)(struct fb_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct fb_ops {
    struct module *owner;
    int (*fb_open)(struct fb_info *, int);
    int (*fb_release)(struct fb_info *, int);
    ssize_t (*fb_read)(struct fb_info *, char *, size_t, loff_t *);
    ssize_t (*fb_write)(struct fb_info *, const char *, size_t, loff_t *);
    int (*fb_check_var)(struct fb_var_screeninfo *, struct fb_info *);
    int (*fb_set_par)(struct fb_info *);
    int (*fb_setcolreg)(unsigned int, unsigned int, unsigned int, unsigned int, unsigned int, struct fb_info *);
    int (*fb_setcmap)(struct fb_cmap *, struct fb_info *);
    int (*fb_blank)(int, struct fb_info *);
    int (*fb_pan_display)(struct fb_var_screeninfo *, struct fb_info *);
    void (*fb_fillrect)(struct fb_info *, const struct fb_fillrect *);
    void (*fb_copyarea)(struct fb_info *, const struct fb_copyarea *);
    void (*fb_imageblit)(struct fb_info *, const struct fb_image *);
    int (*fb_cursor)(struct fb_info *, struct fb_cursor *);
    int (*fb_sync)(struct fb_info *);
    int (*fb_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_compat_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_mmap)(struct fb_info *, struct vm_area_struct *);
    void (*fb_get_caps)(struct fb_info *, struct fb_blit_caps *, struct fb_var_screeninfo *);
    void (*fb_destroy)(struct fb_info *);
    int (*fb_debug_enter)(struct fb_info *);
    int (*fb_debug_leave)(struct fb_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct fb_ops {
    struct module *owner;
    int (*fb_open)(struct fb_info *, int);
    int (*fb_release)(struct fb_info *, int);
    ssize_t (*fb_read)(struct fb_info *, char *, size_t, loff_t *);
    ssize_t (*fb_write)(struct fb_info *, const char *, size_t, loff_t *);
    int (*fb_check_var)(struct fb_var_screeninfo *, struct fb_info *);
    int (*fb_set_par)(struct fb_info *);
    int (*fb_setcolreg)(unsigned int, unsigned int, unsigned int, unsigned int, unsigned int, struct fb_info *);
    int (*fb_setcmap)(struct fb_cmap *, struct fb_info *);
    int (*fb_blank)(int, struct fb_info *);
    int (*fb_pan_display)(struct fb_var_screeninfo *, struct fb_info *);
    void (*fb_fillrect)(struct fb_info *, const struct fb_fillrect *);
    void (*fb_copyarea)(struct fb_info *, const struct fb_copyarea *);
    void (*fb_imageblit)(struct fb_info *, const struct fb_image *);
    int (*fb_cursor)(struct fb_info *, struct fb_cursor *);
    int (*fb_sync)(struct fb_info *);
    int (*fb_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_compat_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_mmap)(struct fb_info *, struct vm_area_struct *);
    void (*fb_get_caps)(struct fb_info *, struct fb_blit_caps *, struct fb_var_screeninfo *);
    void (*fb_destroy)(struct fb_info *);
    int (*fb_debug_enter)(struct fb_info *);
    int (*fb_debug_leave)(struct fb_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct fb_ops {
    struct module *owner;
    int (*fb_open)(struct fb_info *, int);
    int (*fb_release)(struct fb_info *, int);
    ssize_t (*fb_read)(struct fb_info *, char *, size_t, loff_t *);
    ssize_t (*fb_write)(struct fb_info *, const char *, size_t, loff_t *);
    int (*fb_check_var)(struct fb_var_screeninfo *, struct fb_info *);
    int (*fb_set_par)(struct fb_info *);
    int (*fb_setcolreg)(unsigned int, unsigned int, unsigned int, unsigned int, unsigned int, struct fb_info *);
    int (*fb_setcmap)(struct fb_cmap *, struct fb_info *);
    int (*fb_blank)(int, struct fb_info *);
    int (*fb_pan_display)(struct fb_var_screeninfo *, struct fb_info *);
    void (*fb_fillrect)(struct fb_info *, const struct fb_fillrect *);
    void (*fb_copyarea)(struct fb_info *, const struct fb_copyarea *);
    void (*fb_imageblit)(struct fb_info *, const struct fb_image *);
    int (*fb_cursor)(struct fb_info *, struct fb_cursor *);
    int (*fb_sync)(struct fb_info *);
    int (*fb_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_compat_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_mmap)(struct fb_info *, struct vm_area_struct *);
    void (*fb_get_caps)(struct fb_info *, struct fb_blit_caps *, struct fb_var_screeninfo *);
    void (*fb_destroy)(struct fb_info *);
    int (*fb_debug_enter)(struct fb_info *);
    int (*fb_debug_leave)(struct fb_info *);
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
struct fb_ops {
    struct module *owner;
    int (*fb_open)(struct fb_info *, int);
    int (*fb_release)(struct fb_info *, int);
    ssize_t (*fb_read)(struct fb_info *, char *, size_t, loff_t *);
    ssize_t (*fb_write)(struct fb_info *, const char *, size_t, loff_t *);
    int (*fb_check_var)(struct fb_var_screeninfo *, struct fb_info *);
    int (*fb_set_par)(struct fb_info *);
    int (*fb_setcolreg)(unsigned int, unsigned int, unsigned int, unsigned int, unsigned int, struct fb_info *);
    int (*fb_setcmap)(struct fb_cmap *, struct fb_info *);
    int (*fb_blank)(int, struct fb_info *);
    int (*fb_pan_display)(struct fb_var_screeninfo *, struct fb_info *);
    void (*fb_fillrect)(struct fb_info *, const struct fb_fillrect *);
    void (*fb_copyarea)(struct fb_info *, const struct fb_copyarea *);
    void (*fb_imageblit)(struct fb_info *, const struct fb_image *);
    int (*fb_cursor)(struct fb_info *, struct fb_cursor *);
    int (*fb_sync)(struct fb_info *);
    int (*fb_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_compat_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_mmap)(struct fb_info *, struct vm_area_struct *);
    void (*fb_get_caps)(struct fb_info *, struct fb_blit_caps *, struct fb_var_screeninfo *);
    void (*fb_destroy)(struct fb_info *);
    int (*fb_debug_enter)(struct fb_info *);
    int (*fb_debug_leave)(struct fb_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct fb_ops {
    struct module *owner;
    int (*fb_open)(struct fb_info *, int);
    int (*fb_release)(struct fb_info *, int);
    ssize_t (*fb_read)(struct fb_info *, char *, size_t, loff_t *);
    ssize_t (*fb_write)(struct fb_info *, const char *, size_t, loff_t *);
    int (*fb_check_var)(struct fb_var_screeninfo *, struct fb_info *);
    int (*fb_set_par)(struct fb_info *);
    int (*fb_setcolreg)(unsigned int, unsigned int, unsigned int, unsigned int, unsigned int, struct fb_info *);
    int (*fb_setcmap)(struct fb_cmap *, struct fb_info *);
    int (*fb_blank)(int, struct fb_info *);
    int (*fb_pan_display)(struct fb_var_screeninfo *, struct fb_info *);
    void (*fb_fillrect)(struct fb_info *, const struct fb_fillrect *);
    void (*fb_copyarea)(struct fb_info *, const struct fb_copyarea *);
    void (*fb_imageblit)(struct fb_info *, const struct fb_image *);
    int (*fb_cursor)(struct fb_info *, struct fb_cursor *);
    int (*fb_sync)(struct fb_info *);
    int (*fb_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_compat_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_mmap)(struct fb_info *, struct vm_area_struct *);
    void (*fb_get_caps)(struct fb_info *, struct fb_blit_caps *, struct fb_var_screeninfo *);
    void (*fb_destroy)(struct fb_info *);
    int (*fb_debug_enter)(struct fb_info *);
    int (*fb_debug_leave)(struct fb_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct fb_ops {
    struct module *owner;
    int (*fb_open)(struct fb_info *, int);
    int (*fb_release)(struct fb_info *, int);
    ssize_t (*fb_read)(struct fb_info *, char *, size_t, loff_t *);
    ssize_t (*fb_write)(struct fb_info *, const char *, size_t, loff_t *);
    int (*fb_check_var)(struct fb_var_screeninfo *, struct fb_info *);
    int (*fb_set_par)(struct fb_info *);
    int (*fb_setcolreg)(unsigned int, unsigned int, unsigned int, unsigned int, unsigned int, struct fb_info *);
    int (*fb_setcmap)(struct fb_cmap *, struct fb_info *);
    int (*fb_blank)(int, struct fb_info *);
    int (*fb_pan_display)(struct fb_var_screeninfo *, struct fb_info *);
    void (*fb_fillrect)(struct fb_info *, const struct fb_fillrect *);
    void (*fb_copyarea)(struct fb_info *, const struct fb_copyarea *);
    void (*fb_imageblit)(struct fb_info *, const struct fb_image *);
    int (*fb_cursor)(struct fb_info *, struct fb_cursor *);
    int (*fb_sync)(struct fb_info *);
    int (*fb_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_compat_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_mmap)(struct fb_info *, struct vm_area_struct *);
    void (*fb_get_caps)(struct fb_info *, struct fb_blit_caps *, struct fb_var_screeninfo *);
    void (*fb_destroy)(struct fb_info *);
    int (*fb_debug_enter)(struct fb_info *);
    int (*fb_debug_leave)(struct fb_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct fb_ops {
    struct module *owner;
    int (*fb_open)(struct fb_info *, int);
    int (*fb_release)(struct fb_info *, int);
    ssize_t (*fb_read)(struct fb_info *, char *, size_t, loff_t *);
    ssize_t (*fb_write)(struct fb_info *, const char *, size_t, loff_t *);
    int (*fb_check_var)(struct fb_var_screeninfo *, struct fb_info *);
    int (*fb_set_par)(struct fb_info *);
    int (*fb_setcolreg)(unsigned int, unsigned int, unsigned int, unsigned int, unsigned int, struct fb_info *);
    int (*fb_setcmap)(struct fb_cmap *, struct fb_info *);
    int (*fb_blank)(int, struct fb_info *);
    int (*fb_pan_display)(struct fb_var_screeninfo *, struct fb_info *);
    void (*fb_fillrect)(struct fb_info *, const struct fb_fillrect *);
    void (*fb_copyarea)(struct fb_info *, const struct fb_copyarea *);
    void (*fb_imageblit)(struct fb_info *, const struct fb_image *);
    int (*fb_cursor)(struct fb_info *, struct fb_cursor *);
    int (*fb_sync)(struct fb_info *);
    int (*fb_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_compat_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_mmap)(struct fb_info *, struct vm_area_struct *);
    void (*fb_get_caps)(struct fb_info *, struct fb_blit_caps *, struct fb_var_screeninfo *);
    void (*fb_destroy)(struct fb_info *);
    int (*fb_debug_enter)(struct fb_info *);
    int (*fb_debug_leave)(struct fb_info *);
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
struct fb_ops {
    struct module *owner;
    int (*fb_open)(struct fb_info *, int);
    int (*fb_release)(struct fb_info *, int);
    ssize_t (*fb_read)(struct fb_info *, char *, size_t, loff_t *);
    ssize_t (*fb_write)(struct fb_info *, const char *, size_t, loff_t *);
    int (*fb_check_var)(struct fb_var_screeninfo *, struct fb_info *);
    int (*fb_set_par)(struct fb_info *);
    int (*fb_setcolreg)(unsigned int, unsigned int, unsigned int, unsigned int, unsigned int, struct fb_info *);
    int (*fb_setcmap)(struct fb_cmap *, struct fb_info *);
    int (*fb_blank)(int, struct fb_info *);
    int (*fb_pan_display)(struct fb_var_screeninfo *, struct fb_info *);
    void (*fb_fillrect)(struct fb_info *, const struct fb_fillrect *);
    void (*fb_copyarea)(struct fb_info *, const struct fb_copyarea *);
    void (*fb_imageblit)(struct fb_info *, const struct fb_image *);
    int (*fb_cursor)(struct fb_info *, struct fb_cursor *);
    int (*fb_sync)(struct fb_info *);
    int (*fb_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_compat_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_mmap)(struct fb_info *, struct vm_area_struct *);
    void (*fb_get_caps)(struct fb_info *, struct fb_blit_caps *, struct fb_var_screeninfo *);
    void (*fb_destroy)(struct fb_info *);
    int (*fb_debug_enter)(struct fb_info *);
    int (*fb_debug_leave)(struct fb_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct fb_ops {
    struct module *owner;
    int (*fb_open)(struct fb_info *, int);
    int (*fb_release)(struct fb_info *, int);
    ssize_t (*fb_read)(struct fb_info *, char *, size_t, loff_t *);
    ssize_t (*fb_write)(struct fb_info *, const char *, size_t, loff_t *);
    int (*fb_check_var)(struct fb_var_screeninfo *, struct fb_info *);
    int (*fb_set_par)(struct fb_info *);
    int (*fb_setcolreg)(unsigned int, unsigned int, unsigned int, unsigned int, unsigned int, struct fb_info *);
    int (*fb_setcmap)(struct fb_cmap *, struct fb_info *);
    int (*fb_blank)(int, struct fb_info *);
    int (*fb_pan_display)(struct fb_var_screeninfo *, struct fb_info *);
    void (*fb_fillrect)(struct fb_info *, const struct fb_fillrect *);
    void (*fb_copyarea)(struct fb_info *, const struct fb_copyarea *);
    void (*fb_imageblit)(struct fb_info *, const struct fb_image *);
    int (*fb_cursor)(struct fb_info *, struct fb_cursor *);
    int (*fb_sync)(struct fb_info *);
    int (*fb_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_compat_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_mmap)(struct fb_info *, struct vm_area_struct *);
    void (*fb_get_caps)(struct fb_info *, struct fb_blit_caps *, struct fb_var_screeninfo *);
    void (*fb_destroy)(struct fb_info *);
    int (*fb_debug_enter)(struct fb_info *);
    int (*fb_debug_leave)(struct fb_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct fb_ops {
    struct module *owner;
    int (*fb_open)(struct fb_info *, int);
    int (*fb_release)(struct fb_info *, int);
    ssize_t (*fb_read)(struct fb_info *, char *, size_t, loff_t *);
    ssize_t (*fb_write)(struct fb_info *, const char *, size_t, loff_t *);
    int (*fb_check_var)(struct fb_var_screeninfo *, struct fb_info *);
    int (*fb_set_par)(struct fb_info *);
    int (*fb_setcolreg)(unsigned int, unsigned int, unsigned int, unsigned int, unsigned int, struct fb_info *);
    int (*fb_setcmap)(struct fb_cmap *, struct fb_info *);
    int (*fb_blank)(int, struct fb_info *);
    int (*fb_pan_display)(struct fb_var_screeninfo *, struct fb_info *);
    void (*fb_fillrect)(struct fb_info *, const struct fb_fillrect *);
    void (*fb_copyarea)(struct fb_info *, const struct fb_copyarea *);
    void (*fb_imageblit)(struct fb_info *, const struct fb_image *);
    int (*fb_cursor)(struct fb_info *, struct fb_cursor *);
    int (*fb_sync)(struct fb_info *);
    int (*fb_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_compat_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_mmap)(struct fb_info *, struct vm_area_struct *);
    void (*fb_get_caps)(struct fb_info *, struct fb_blit_caps *, struct fb_var_screeninfo *);
    void (*fb_destroy)(struct fb_info *);
    int (*fb_debug_enter)(struct fb_info *);
    int (*fb_debug_leave)(struct fb_info *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct fb_ops {
    struct module *owner;
    int (*fb_open)(struct fb_info *, int);
    int (*fb_release)(struct fb_info *, int);
    ssize_t (*fb_read)(struct fb_info *, char *, size_t, loff_t *);
    ssize_t (*fb_write)(struct fb_info *, const char *, size_t, loff_t *);
    int (*fb_check_var)(struct fb_var_screeninfo *, struct fb_info *);
    int (*fb_set_par)(struct fb_info *);
    int (*fb_setcolreg)(unsigned int, unsigned int, unsigned int, unsigned int, unsigned int, struct fb_info *);
    int (*fb_setcmap)(struct fb_cmap *, struct fb_info *);
    int (*fb_blank)(int, struct fb_info *);
    int (*fb_pan_display)(struct fb_var_screeninfo *, struct fb_info *);
    void (*fb_fillrect)(struct fb_info *, const struct fb_fillrect *);
    void (*fb_copyarea)(struct fb_info *, const struct fb_copyarea *);
    void (*fb_imageblit)(struct fb_info *, const struct fb_image *);
    int (*fb_cursor)(struct fb_info *, struct fb_cursor *);
    int (*fb_sync)(struct fb_info *);
    int (*fb_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_compat_ioctl)(struct fb_info *, unsigned int, long unsigned int);
    int (*fb_mmap)(struct fb_info *, struct vm_area_struct *);
    void (*fb_get_caps)(struct fb_info *, struct fb_blit_caps *, struct fb_var_screeninfo *);
    void (*fb_destroy)(struct fb_info *);
    int (*fb_debug_enter)(struct fb_info *);
    int (*fb_debug_leave)(struct fb_info *);
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
<b>Field removed. </b>
<code>void (*fb_rotate)(struct fb_info *, int)</code>
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
