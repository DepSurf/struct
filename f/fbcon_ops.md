# Struct: <code>fbcon_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct fbcon_ops {
    void (*bmove)(struct vc_data *, struct fb_info *, int, int, int, int, int, int);
    void (*clear)(struct vc_data *, struct fb_info *, int, int, int, int);
    void (*putcs)(struct vc_data *, struct fb_info *, const short unsigned int *, int, int, int, int, int);
    void (*clear_margins)(struct vc_data *, struct fb_info *, int);
    void (*cursor)(struct vc_data *, struct fb_info *, int, int, int, int);
    int (*update_start)(struct fb_info *);
    int (*rotate_font)(struct fb_info *, struct vc_data *);
    struct fb_var_screeninfo var;
    struct timer_list cursor_timer;
    struct fb_cursor cursor_state;
    struct display *p;
    int currcon;
    int cur_blink_jiffies;
    int cursor_flash;
    int cursor_reset;
    int blank_state;
    int graphics;
    int save_graphics;
    int flags;
    int rotate;
    int cur_rotate;
    char *cursor_data;
    u8 *fontbuffer;
    u8 *fontdata;
    u8 *cursor_src;
    u32 cursor_size;
    u32 fd_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct fbcon_ops {
    void (*bmove)(struct vc_data *, struct fb_info *, int, int, int, int, int, int);
    void (*clear)(struct vc_data *, struct fb_info *, int, int, int, int);
    void (*putcs)(struct vc_data *, struct fb_info *, const short unsigned int *, int, int, int, int, int);
    void (*clear_margins)(struct vc_data *, struct fb_info *, int);
    void (*cursor)(struct vc_data *, struct fb_info *, int, int, int, int);
    int (*update_start)(struct fb_info *);
    int (*rotate_font)(struct fb_info *, struct vc_data *);
    struct fb_var_screeninfo var;
    struct timer_list cursor_timer;
    struct fb_cursor cursor_state;
    struct display *p;
    int currcon;
    int cur_blink_jiffies;
    int cursor_flash;
    int cursor_reset;
    int blank_state;
    int graphics;
    int save_graphics;
    int flags;
    int rotate;
    int cur_rotate;
    char *cursor_data;
    u8 *fontbuffer;
    u8 *fontdata;
    u8 *cursor_src;
    u32 cursor_size;
    u32 fd_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct fbcon_ops {
    void (*bmove)(struct vc_data *, struct fb_info *, int, int, int, int, int, int);
    void (*clear)(struct vc_data *, struct fb_info *, int, int, int, int);
    void (*putcs)(struct vc_data *, struct fb_info *, const short unsigned int *, int, int, int, int, int);
    void (*clear_margins)(struct vc_data *, struct fb_info *, int);
    void (*cursor)(struct vc_data *, struct fb_info *, int, int, int, int);
    int (*update_start)(struct fb_info *);
    int (*rotate_font)(struct fb_info *, struct vc_data *);
    struct fb_var_screeninfo var;
    struct timer_list cursor_timer;
    struct fb_cursor cursor_state;
    struct display *p;
    int currcon;
    int cur_blink_jiffies;
    int cursor_flash;
    int cursor_reset;
    int blank_state;
    int graphics;
    int save_graphics;
    int flags;
    int rotate;
    int cur_rotate;
    char *cursor_data;
    u8 *fontbuffer;
    u8 *fontdata;
    u8 *cursor_src;
    u32 cursor_size;
    u32 fd_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct fbcon_ops {
    void (*bmove)(struct vc_data *, struct fb_info *, int, int, int, int, int, int);
    void (*clear)(struct vc_data *, struct fb_info *, int, int, int, int);
    void (*putcs)(struct vc_data *, struct fb_info *, const short unsigned int *, int, int, int, int, int);
    void (*clear_margins)(struct vc_data *, struct fb_info *, int);
    void (*cursor)(struct vc_data *, struct fb_info *, int, int, int, int);
    int (*update_start)(struct fb_info *);
    int (*rotate_font)(struct fb_info *, struct vc_data *);
    struct fb_var_screeninfo var;
    struct timer_list cursor_timer;
    struct fb_cursor cursor_state;
    struct display *p;
    int currcon;
    int cur_blink_jiffies;
    int cursor_flash;
    int cursor_reset;
    int blank_state;
    int graphics;
    int save_graphics;
    int flags;
    int rotate;
    int cur_rotate;
    char *cursor_data;
    u8 *fontbuffer;
    u8 *fontdata;
    u8 *cursor_src;
    u32 cursor_size;
    u32 fd_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct fbcon_ops {
    void (*bmove)(struct vc_data *, struct fb_info *, int, int, int, int, int, int);
    void (*clear)(struct vc_data *, struct fb_info *, int, int, int, int);
    void (*putcs)(struct vc_data *, struct fb_info *, const short unsigned int *, int, int, int, int, int);
    void (*clear_margins)(struct vc_data *, struct fb_info *, int, int);
    void (*cursor)(struct vc_data *, struct fb_info *, int, int, int, int);
    int (*update_start)(struct fb_info *);
    int (*rotate_font)(struct fb_info *, struct vc_data *);
    struct fb_var_screeninfo var;
    struct timer_list cursor_timer;
    struct fb_cursor cursor_state;
    struct display *p;
    struct fb_info *info;
    int currcon;
    int cur_blink_jiffies;
    int cursor_flash;
    int cursor_reset;
    int blank_state;
    int graphics;
    int save_graphics;
    int flags;
    int rotate;
    int cur_rotate;
    char *cursor_data;
    u8 *fontbuffer;
    u8 *fontdata;
    u8 *cursor_src;
    u32 cursor_size;
    u32 fd_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct fbcon_ops {
    void (*bmove)(struct vc_data *, struct fb_info *, int, int, int, int, int, int);
    void (*clear)(struct vc_data *, struct fb_info *, int, int, int, int);
    void (*putcs)(struct vc_data *, struct fb_info *, const short unsigned int *, int, int, int, int, int);
    void (*clear_margins)(struct vc_data *, struct fb_info *, int, int);
    void (*cursor)(struct vc_data *, struct fb_info *, int, int, int, int);
    int (*update_start)(struct fb_info *);
    int (*rotate_font)(struct fb_info *, struct vc_data *);
    struct fb_var_screeninfo var;
    struct timer_list cursor_timer;
    struct fb_cursor cursor_state;
    struct display *p;
    struct fb_info *info;
    int currcon;
    int cur_blink_jiffies;
    int cursor_flash;
    int cursor_reset;
    int blank_state;
    int graphics;
    int save_graphics;
    int flags;
    int rotate;
    int cur_rotate;
    char *cursor_data;
    u8 *fontbuffer;
    u8 *fontdata;
    u8 *cursor_src;
    u32 cursor_size;
    u32 fd_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct fbcon_ops {
    void (*bmove)(struct vc_data *, struct fb_info *, int, int, int, int, int, int);
    void (*clear)(struct vc_data *, struct fb_info *, int, int, int, int);
    void (*putcs)(struct vc_data *, struct fb_info *, const short unsigned int *, int, int, int, int, int);
    void (*clear_margins)(struct vc_data *, struct fb_info *, int, int);
    void (*cursor)(struct vc_data *, struct fb_info *, int, int, int, int);
    int (*update_start)(struct fb_info *);
    int (*rotate_font)(struct fb_info *, struct vc_data *);
    struct fb_var_screeninfo var;
    struct timer_list cursor_timer;
    struct fb_cursor cursor_state;
    struct display *p;
    struct fb_info *info;
    int currcon;
    int cur_blink_jiffies;
    int cursor_flash;
    int cursor_reset;
    int blank_state;
    int graphics;
    int save_graphics;
    int flags;
    int rotate;
    int cur_rotate;
    char *cursor_data;
    u8 *fontbuffer;
    u8 *fontdata;
    u8 *cursor_src;
    u32 cursor_size;
    u32 fd_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct fbcon_ops {
    void (*bmove)(struct vc_data *, struct fb_info *, int, int, int, int, int, int);
    void (*clear)(struct vc_data *, struct fb_info *, int, int, int, int);
    void (*putcs)(struct vc_data *, struct fb_info *, const short unsigned int *, int, int, int, int, int);
    void (*clear_margins)(struct vc_data *, struct fb_info *, int, int);
    void (*cursor)(struct vc_data *, struct fb_info *, int, int, int, int);
    int (*update_start)(struct fb_info *);
    int (*rotate_font)(struct fb_info *, struct vc_data *);
    struct fb_var_screeninfo var;
    struct timer_list cursor_timer;
    struct fb_cursor cursor_state;
    struct fbcon_display *p;
    struct fb_info *info;
    int currcon;
    int cur_blink_jiffies;
    int cursor_flash;
    int cursor_reset;
    int blank_state;
    int graphics;
    int save_graphics;
    int flags;
    int rotate;
    int cur_rotate;
    char *cursor_data;
    u8 *fontbuffer;
    u8 *fontdata;
    u8 *cursor_src;
    u32 cursor_size;
    u32 fd_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct fbcon_ops {
    void (*bmove)(struct vc_data *, struct fb_info *, int, int, int, int, int, int);
    void (*clear)(struct vc_data *, struct fb_info *, int, int, int, int);
    void (*putcs)(struct vc_data *, struct fb_info *, const short unsigned int *, int, int, int, int, int);
    void (*clear_margins)(struct vc_data *, struct fb_info *, int, int);
    void (*cursor)(struct vc_data *, struct fb_info *, int, int, int, int);
    int (*update_start)(struct fb_info *);
    int (*rotate_font)(struct fb_info *, struct vc_data *);
    struct fb_var_screeninfo var;
    struct timer_list cursor_timer;
    struct fb_cursor cursor_state;
    struct fbcon_display *p;
    struct fb_info *info;
    int currcon;
    int cur_blink_jiffies;
    int cursor_flash;
    int cursor_reset;
    int blank_state;
    int graphics;
    int save_graphics;
    int flags;
    int rotate;
    int cur_rotate;
    char *cursor_data;
    u8 *fontbuffer;
    u8 *fontdata;
    u8 *cursor_src;
    u32 cursor_size;
    u32 fd_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct fbcon_ops {
    void (*bmove)(struct vc_data *, struct fb_info *, int, int, int, int, int, int);
    void (*clear)(struct vc_data *, struct fb_info *, int, int, int, int);
    void (*putcs)(struct vc_data *, struct fb_info *, const short unsigned int *, int, int, int, int, int);
    void (*clear_margins)(struct vc_data *, struct fb_info *, int, int);
    void (*cursor)(struct vc_data *, struct fb_info *, int, int, int);
    int (*update_start)(struct fb_info *);
    int (*rotate_font)(struct fb_info *, struct vc_data *);
    struct fb_var_screeninfo var;
    struct timer_list cursor_timer;
    struct fb_cursor cursor_state;
    struct fbcon_display *p;
    struct fb_info *info;
    int currcon;
    int cur_blink_jiffies;
    int cursor_flash;
    int cursor_reset;
    int blank_state;
    int graphics;
    int save_graphics;
    int flags;
    int rotate;
    int cur_rotate;
    char *cursor_data;
    u8 *fontbuffer;
    u8 *fontdata;
    u8 *cursor_src;
    u32 cursor_size;
    u32 fd_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct fbcon_ops {
    void (*bmove)(struct vc_data *, struct fb_info *, int, int, int, int, int, int);
    void (*clear)(struct vc_data *, struct fb_info *, int, int, int, int);
    void (*putcs)(struct vc_data *, struct fb_info *, const short unsigned int *, int, int, int, int, int);
    void (*clear_margins)(struct vc_data *, struct fb_info *, int, int);
    void (*cursor)(struct vc_data *, struct fb_info *, int, int, int);
    int (*update_start)(struct fb_info *);
    int (*rotate_font)(struct fb_info *, struct vc_data *);
    struct fb_var_screeninfo var;
    struct timer_list cursor_timer;
    struct fb_cursor cursor_state;
    struct fbcon_display *p;
    struct fb_info *info;
    int currcon;
    int cur_blink_jiffies;
    int cursor_flash;
    int cursor_reset;
    int blank_state;
    int graphics;
    int save_graphics;
    int flags;
    int rotate;
    int cur_rotate;
    char *cursor_data;
    u8 *fontbuffer;
    u8 *fontdata;
    u8 *cursor_src;
    u32 cursor_size;
    u32 fd_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct fbcon_ops {
    void (*bmove)(struct vc_data *, struct fb_info *, int, int, int, int, int, int);
    void (*clear)(struct vc_data *, struct fb_info *, int, int, int, int);
    void (*putcs)(struct vc_data *, struct fb_info *, const short unsigned int *, int, int, int, int, int);
    void (*clear_margins)(struct vc_data *, struct fb_info *, int, int);
    void (*cursor)(struct vc_data *, struct fb_info *, int, int, int);
    int (*update_start)(struct fb_info *);
    int (*rotate_font)(struct fb_info *, struct vc_data *);
    struct fb_var_screeninfo var;
    struct timer_list cursor_timer;
    struct fb_cursor cursor_state;
    struct fbcon_display *p;
    struct fb_info *info;
    int currcon;
    int cur_blink_jiffies;
    int cursor_flash;
    int cursor_reset;
    int blank_state;
    int graphics;
    int save_graphics;
    int flags;
    int rotate;
    int cur_rotate;
    char *cursor_data;
    u8 *fontbuffer;
    u8 *fontdata;
    u8 *cursor_src;
    u32 cursor_size;
    u32 fd_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct fbcon_ops {
    void (*bmove)(struct vc_data *, struct fb_info *, int, int, int, int, int, int);
    void (*clear)(struct vc_data *, struct fb_info *, int, int, int, int);
    void (*putcs)(struct vc_data *, struct fb_info *, const short unsigned int *, int, int, int, int, int);
    void (*clear_margins)(struct vc_data *, struct fb_info *, int, int);
    void (*cursor)(struct vc_data *, struct fb_info *, int, int, int);
    int (*update_start)(struct fb_info *);
    int (*rotate_font)(struct fb_info *, struct vc_data *);
    struct fb_var_screeninfo var;
    struct timer_list cursor_timer;
    struct fb_cursor cursor_state;
    struct fbcon_display *p;
    struct fb_info *info;
    int currcon;
    int cur_blink_jiffies;
    int cursor_flash;
    int cursor_reset;
    int blank_state;
    int graphics;
    int save_graphics;
    int flags;
    int rotate;
    int cur_rotate;
    char *cursor_data;
    u8 *fontbuffer;
    u8 *fontdata;
    u8 *cursor_src;
    u32 cursor_size;
    u32 fd_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct fbcon_ops {
    void (*bmove)(struct vc_data *, struct fb_info *, int, int, int, int, int, int);
    void (*clear)(struct vc_data *, struct fb_info *, int, int, int, int);
    void (*putcs)(struct vc_data *, struct fb_info *, const short unsigned int *, int, int, int, int, int);
    void (*clear_margins)(struct vc_data *, struct fb_info *, int, int);
    void (*cursor)(struct vc_data *, struct fb_info *, int, int, int);
    int (*update_start)(struct fb_info *);
    int (*rotate_font)(struct fb_info *, struct vc_data *);
    struct fb_var_screeninfo var;
    struct delayed_work cursor_work;
    struct fb_cursor cursor_state;
    struct fbcon_display *p;
    struct fb_info *info;
    int currcon;
    int cur_blink_jiffies;
    int cursor_flash;
    int cursor_reset;
    int blank_state;
    int graphics;
    int save_graphics;
    bool initialized;
    int rotate;
    int cur_rotate;
    char *cursor_data;
    u8 *fontbuffer;
    u8 *fontdata;
    u8 *cursor_src;
    u32 cursor_size;
    u32 fd_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct fbcon_ops {
    void (*bmove)(struct vc_data *, struct fb_info *, int, int, int, int, int, int);
    void (*clear)(struct vc_data *, struct fb_info *, int, int, int, int);
    void (*putcs)(struct vc_data *, struct fb_info *, const short unsigned int *, int, int, int, int, int);
    void (*clear_margins)(struct vc_data *, struct fb_info *, int, int);
    void (*cursor)(struct vc_data *, struct fb_info *, int, int, int);
    int (*update_start)(struct fb_info *);
    int (*rotate_font)(struct fb_info *, struct vc_data *);
    struct fb_var_screeninfo var;
    struct delayed_work cursor_work;
    struct fb_cursor cursor_state;
    struct fbcon_display *p;
    struct fb_info *info;
    int currcon;
    int cur_blink_jiffies;
    int cursor_flash;
    int cursor_reset;
    int blank_state;
    int graphics;
    int save_graphics;
    bool initialized;
    int rotate;
    int cur_rotate;
    char *cursor_data;
    u8 *fontbuffer;
    u8 *fontdata;
    u8 *cursor_src;
    u32 cursor_size;
    u32 fd_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct fbcon_ops {
    void (*bmove)(struct vc_data *, struct fb_info *, int, int, int, int, int, int);
    void (*clear)(struct vc_data *, struct fb_info *, int, int, int, int);
    void (*putcs)(struct vc_data *, struct fb_info *, const short unsigned int *, int, int, int, int, int);
    void (*clear_margins)(struct vc_data *, struct fb_info *, int, int);
    void (*cursor)(struct vc_data *, struct fb_info *, int, int, int);
    int (*update_start)(struct fb_info *);
    int (*rotate_font)(struct fb_info *, struct vc_data *);
    struct fb_var_screeninfo var;
    struct delayed_work cursor_work;
    struct fb_cursor cursor_state;
    struct fbcon_display *p;
    struct fb_info *info;
    int currcon;
    int cur_blink_jiffies;
    int cursor_flash;
    int cursor_reset;
    int blank_state;
    int graphics;
    int save_graphics;
    bool initialized;
    int rotate;
    int cur_rotate;
    char *cursor_data;
    u8 *fontbuffer;
    u8 *fontdata;
    u8 *cursor_src;
    u32 cursor_size;
    u32 fd_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct fbcon_ops {
    void (*bmove)(struct vc_data *, struct fb_info *, int, int, int, int, int, int);
    void (*clear)(struct vc_data *, struct fb_info *, int, int, int, int);
    void (*putcs)(struct vc_data *, struct fb_info *, const short unsigned int *, int, int, int, int, int);
    void (*clear_margins)(struct vc_data *, struct fb_info *, int, int);
    void (*cursor)(struct vc_data *, struct fb_info *, int, int, int);
    int (*update_start)(struct fb_info *);
    int (*rotate_font)(struct fb_info *, struct vc_data *);
    struct fb_var_screeninfo var;
    struct delayed_work cursor_work;
    struct fb_cursor cursor_state;
    struct fbcon_display *p;
    struct fb_info *info;
    int currcon;
    int cur_blink_jiffies;
    int cursor_flash;
    int cursor_reset;
    int blank_state;
    int graphics;
    int save_graphics;
    bool initialized;
    int rotate;
    int cur_rotate;
    char *cursor_data;
    u8 *fontbuffer;
    u8 *fontdata;
    u8 *cursor_src;
    u32 cursor_size;
    u32 fd_size;
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
struct fbcon_ops {
    void (*bmove)(struct vc_data *, struct fb_info *, int, int, int, int, int, int);
    void (*clear)(struct vc_data *, struct fb_info *, int, int, int, int);
    void (*putcs)(struct vc_data *, struct fb_info *, const short unsigned int *, int, int, int, int, int);
    void (*clear_margins)(struct vc_data *, struct fb_info *, int, int);
    void (*cursor)(struct vc_data *, struct fb_info *, int, int, int, int);
    int (*update_start)(struct fb_info *);
    int (*rotate_font)(struct fb_info *, struct vc_data *);
    struct fb_var_screeninfo var;
    struct timer_list cursor_timer;
    struct fb_cursor cursor_state;
    struct fbcon_display *p;
    struct fb_info *info;
    int currcon;
    int cur_blink_jiffies;
    int cursor_flash;
    int cursor_reset;
    int blank_state;
    int graphics;
    int save_graphics;
    int flags;
    int rotate;
    int cur_rotate;
    char *cursor_data;
    u8 *fontbuffer;
    u8 *fontdata;
    u8 *cursor_src;
    u32 cursor_size;
    u32 fd_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct fbcon_ops {
    void (*bmove)(struct vc_data *, struct fb_info *, int, int, int, int, int, int);
    void (*clear)(struct vc_data *, struct fb_info *, int, int, int, int);
    void (*putcs)(struct vc_data *, struct fb_info *, const short unsigned int *, int, int, int, int, int);
    void (*clear_margins)(struct vc_data *, struct fb_info *, int, int);
    void (*cursor)(struct vc_data *, struct fb_info *, int, int, int, int);
    int (*update_start)(struct fb_info *);
    int (*rotate_font)(struct fb_info *, struct vc_data *);
    struct fb_var_screeninfo var;
    struct timer_list cursor_timer;
    struct fb_cursor cursor_state;
    struct fbcon_display *p;
    struct fb_info *info;
    int currcon;
    int cur_blink_jiffies;
    int cursor_flash;
    int cursor_reset;
    int blank_state;
    int graphics;
    int save_graphics;
    int flags;
    int rotate;
    int cur_rotate;
    char *cursor_data;
    u8 *fontbuffer;
    u8 *fontdata;
    u8 *cursor_src;
    u32 cursor_size;
    u32 fd_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct fbcon_ops {
    void (*bmove)(struct vc_data *, struct fb_info *, int, int, int, int, int, int);
    void (*clear)(struct vc_data *, struct fb_info *, int, int, int, int);
    void (*putcs)(struct vc_data *, struct fb_info *, const short unsigned int *, int, int, int, int, int);
    void (*clear_margins)(struct vc_data *, struct fb_info *, int, int);
    void (*cursor)(struct vc_data *, struct fb_info *, int, int, int, int);
    int (*update_start)(struct fb_info *);
    int (*rotate_font)(struct fb_info *, struct vc_data *);
    struct fb_var_screeninfo var;
    struct timer_list cursor_timer;
    struct fb_cursor cursor_state;
    struct fbcon_display *p;
    struct fb_info *info;
    int currcon;
    int cur_blink_jiffies;
    int cursor_flash;
    int cursor_reset;
    int blank_state;
    int graphics;
    int save_graphics;
    int flags;
    int rotate;
    int cur_rotate;
    char *cursor_data;
    u8 *fontbuffer;
    u8 *fontdata;
    u8 *cursor_src;
    u32 cursor_size;
    u32 fd_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct fbcon_ops {
    void (*bmove)(struct vc_data *, struct fb_info *, int, int, int, int, int, int);
    void (*clear)(struct vc_data *, struct fb_info *, int, int, int, int);
    void (*putcs)(struct vc_data *, struct fb_info *, const short unsigned int *, int, int, int, int, int);
    void (*clear_margins)(struct vc_data *, struct fb_info *, int, int);
    void (*cursor)(struct vc_data *, struct fb_info *, int, int, int, int);
    int (*update_start)(struct fb_info *);
    int (*rotate_font)(struct fb_info *, struct vc_data *);
    struct fb_var_screeninfo var;
    struct timer_list cursor_timer;
    struct fb_cursor cursor_state;
    struct fbcon_display *p;
    struct fb_info *info;
    int currcon;
    int cur_blink_jiffies;
    int cursor_flash;
    int cursor_reset;
    int blank_state;
    int graphics;
    int save_graphics;
    int flags;
    int rotate;
    int cur_rotate;
    char *cursor_data;
    u8 *fontbuffer;
    u8 *fontdata;
    u8 *cursor_src;
    u32 cursor_size;
    u32 fd_size;
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
struct fbcon_ops {
    void (*bmove)(struct vc_data *, struct fb_info *, int, int, int, int, int, int);
    void (*clear)(struct vc_data *, struct fb_info *, int, int, int, int);
    void (*putcs)(struct vc_data *, struct fb_info *, const short unsigned int *, int, int, int, int, int);
    void (*clear_margins)(struct vc_data *, struct fb_info *, int, int);
    void (*cursor)(struct vc_data *, struct fb_info *, int, int, int, int);
    int (*update_start)(struct fb_info *);
    int (*rotate_font)(struct fb_info *, struct vc_data *);
    struct fb_var_screeninfo var;
    struct timer_list cursor_timer;
    struct fb_cursor cursor_state;
    struct fbcon_display *p;
    struct fb_info *info;
    int currcon;
    int cur_blink_jiffies;
    int cursor_flash;
    int cursor_reset;
    int blank_state;
    int graphics;
    int save_graphics;
    int flags;
    int rotate;
    int cur_rotate;
    char *cursor_data;
    u8 *fontbuffer;
    u8 *fontdata;
    u8 *cursor_src;
    u32 cursor_size;
    u32 fd_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct fbcon_ops {
    void (*bmove)(struct vc_data *, struct fb_info *, int, int, int, int, int, int);
    void (*clear)(struct vc_data *, struct fb_info *, int, int, int, int);
    void (*putcs)(struct vc_data *, struct fb_info *, const short unsigned int *, int, int, int, int, int);
    void (*clear_margins)(struct vc_data *, struct fb_info *, int, int);
    void (*cursor)(struct vc_data *, struct fb_info *, int, int, int, int);
    int (*update_start)(struct fb_info *);
    int (*rotate_font)(struct fb_info *, struct vc_data *);
    struct fb_var_screeninfo var;
    struct timer_list cursor_timer;
    struct fb_cursor cursor_state;
    struct fbcon_display *p;
    struct fb_info *info;
    int currcon;
    int cur_blink_jiffies;
    int cursor_flash;
    int cursor_reset;
    int blank_state;
    int graphics;
    int save_graphics;
    int flags;
    int rotate;
    int cur_rotate;
    char *cursor_data;
    u8 *fontbuffer;
    u8 *fontdata;
    u8 *cursor_src;
    u32 cursor_size;
    u32 fd_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct fbcon_ops {
    void (*bmove)(struct vc_data *, struct fb_info *, int, int, int, int, int, int);
    void (*clear)(struct vc_data *, struct fb_info *, int, int, int, int);
    void (*putcs)(struct vc_data *, struct fb_info *, const short unsigned int *, int, int, int, int, int);
    void (*clear_margins)(struct vc_data *, struct fb_info *, int, int);
    void (*cursor)(struct vc_data *, struct fb_info *, int, int, int, int);
    int (*update_start)(struct fb_info *);
    int (*rotate_font)(struct fb_info *, struct vc_data *);
    struct fb_var_screeninfo var;
    struct timer_list cursor_timer;
    struct fb_cursor cursor_state;
    struct fbcon_display *p;
    struct fb_info *info;
    int currcon;
    int cur_blink_jiffies;
    int cursor_flash;
    int cursor_reset;
    int blank_state;
    int graphics;
    int save_graphics;
    int flags;
    int rotate;
    int cur_rotate;
    char *cursor_data;
    u8 *fontbuffer;
    u8 *fontdata;
    u8 *cursor_src;
    u32 cursor_size;
    u32 fd_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct fbcon_ops {
    void (*bmove)(struct vc_data *, struct fb_info *, int, int, int, int, int, int);
    void (*clear)(struct vc_data *, struct fb_info *, int, int, int, int);
    void (*putcs)(struct vc_data *, struct fb_info *, const short unsigned int *, int, int, int, int, int);
    void (*clear_margins)(struct vc_data *, struct fb_info *, int, int);
    void (*cursor)(struct vc_data *, struct fb_info *, int, int, int, int);
    int (*update_start)(struct fb_info *);
    int (*rotate_font)(struct fb_info *, struct vc_data *);
    struct fb_var_screeninfo var;
    struct timer_list cursor_timer;
    struct fb_cursor cursor_state;
    struct fbcon_display *p;
    struct fb_info *info;
    int currcon;
    int cur_blink_jiffies;
    int cursor_flash;
    int cursor_reset;
    int blank_state;
    int graphics;
    int save_graphics;
    int flags;
    int rotate;
    int cur_rotate;
    char *cursor_data;
    u8 *fontbuffer;
    u8 *fontdata;
    u8 *cursor_src;
    u32 cursor_size;
    u32 fd_size;
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
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct fb_info *info</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*clear_margins)(struct vc_data *, struct fb_info *, int)</code> ➡️ <code>void (*clear_margins)(struct vc_data *, struct fb_info *, int, int)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct display *p</code> ➡️ <code>struct fbcon_display *p</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>void (*cursor)(struct vc_data *, struct fb_info *, int, int, int, int)</code> ➡️ <code>void (*cursor)(struct vc_data *, struct fb_info *, int, int, int)</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct delayed_work cursor_work</code>
</li>
<li>
<b>Field added. </b>
<code>bool initialized</code>
</li>
<li>
<b>Field removed. </b>
<code>struct timer_list cursor_timer</code>
</li>
<li>
<b>Field removed. </b>
<code>int flags</code>
</li>
</ul>
</details>
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
