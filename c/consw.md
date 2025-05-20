# Struct: <code>consw</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct consw {
    struct module *owner;
    const char * (*con_startup)();
    void (*con_init)(struct vc_data *, int);
    void (*con_deinit)(struct vc_data *);
    void (*con_clear)(struct vc_data *, int, int, int, int);
    void (*con_putc)(struct vc_data *, int, int, int);
    void (*con_putcs)(struct vc_data *, const short unsigned int *, int, int, int);
    void (*con_cursor)(struct vc_data *, int);
    int (*con_scroll)(struct vc_data *, int, int, int, int);
    void (*con_bmove)(struct vc_data *, int, int, int, int, int, int);
    int (*con_switch)(struct vc_data *);
    int (*con_blank)(struct vc_data *, int, int);
    int (*con_font_set)(struct vc_data *, struct console_font *, unsigned int);
    int (*con_font_get)(struct vc_data *, struct console_font *);
    int (*con_font_default)(struct vc_data *, struct console_font *, char *);
    int (*con_font_copy)(struct vc_data *, int);
    int (*con_resize)(struct vc_data *, unsigned int, unsigned int, unsigned int);
    int (*con_set_palette)(struct vc_data *, unsigned char *);
    int (*con_scrolldelta)(struct vc_data *, int);
    int (*con_set_origin)(struct vc_data *);
    void (*con_save_screen)(struct vc_data *);
    u8 (*con_build_attr)(struct vc_data *, u8, u8, u8, u8, u8, u8);
    void (*con_invert_region)(struct vc_data *, u16 *, int);
    u16 * (*con_screen_pos)(struct vc_data *, int);
    long unsigned int (*con_getxy)(struct vc_data *, long unsigned int, int *, int *);
    int (*con_debug_enter)(struct vc_data *);
    int (*con_debug_leave)(struct vc_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct consw {
    struct module *owner;
    const char * (*con_startup)();
    void (*con_init)(struct vc_data *, int);
    void (*con_deinit)(struct vc_data *);
    void (*con_clear)(struct vc_data *, int, int, int, int);
    void (*con_putc)(struct vc_data *, int, int, int);
    void (*con_putcs)(struct vc_data *, const short unsigned int *, int, int, int);
    void (*con_cursor)(struct vc_data *, int);
    int (*con_scroll)(struct vc_data *, int, int, int, int);
    int (*con_switch)(struct vc_data *);
    int (*con_blank)(struct vc_data *, int, int);
    int (*con_font_set)(struct vc_data *, struct console_font *, unsigned int);
    int (*con_font_get)(struct vc_data *, struct console_font *);
    int (*con_font_default)(struct vc_data *, struct console_font *, char *);
    int (*con_font_copy)(struct vc_data *, int);
    int (*con_resize)(struct vc_data *, unsigned int, unsigned int, unsigned int);
    void (*con_set_palette)(struct vc_data *, const unsigned char *);
    void (*con_scrolldelta)(struct vc_data *, int);
    int (*con_set_origin)(struct vc_data *);
    void (*con_save_screen)(struct vc_data *);
    u8 (*con_build_attr)(struct vc_data *, u8, u8, u8, u8, u8, u8);
    void (*con_invert_region)(struct vc_data *, u16 *, int);
    u16 * (*con_screen_pos)(struct vc_data *, int);
    long unsigned int (*con_getxy)(struct vc_data *, long unsigned int, int *, int *);
    int (*con_debug_enter)(struct vc_data *);
    int (*con_debug_leave)(struct vc_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct consw {
    struct module *owner;
    const char * (*con_startup)();
    void (*con_init)(struct vc_data *, int);
    void (*con_deinit)(struct vc_data *);
    void (*con_clear)(struct vc_data *, int, int, int, int);
    void (*con_putc)(struct vc_data *, int, int, int);
    void (*con_putcs)(struct vc_data *, const short unsigned int *, int, int, int);
    void (*con_cursor)(struct vc_data *, int);
    bool (*con_scroll)(struct vc_data *, unsigned int, unsigned int, enum con_scroll, unsigned int);
    int (*con_switch)(struct vc_data *);
    int (*con_blank)(struct vc_data *, int, int);
    int (*con_font_set)(struct vc_data *, struct console_font *, unsigned int);
    int (*con_font_get)(struct vc_data *, struct console_font *);
    int (*con_font_default)(struct vc_data *, struct console_font *, char *);
    int (*con_font_copy)(struct vc_data *, int);
    int (*con_resize)(struct vc_data *, unsigned int, unsigned int, unsigned int);
    void (*con_set_palette)(struct vc_data *, const unsigned char *);
    void (*con_scrolldelta)(struct vc_data *, int);
    int (*con_set_origin)(struct vc_data *);
    void (*con_save_screen)(struct vc_data *);
    u8 (*con_build_attr)(struct vc_data *, u8, u8, u8, u8, u8, u8);
    void (*con_invert_region)(struct vc_data *, u16 *, int);
    u16 * (*con_screen_pos)(struct vc_data *, int);
    long unsigned int (*con_getxy)(struct vc_data *, long unsigned int, int *, int *);
    int (*con_debug_enter)(struct vc_data *);
    int (*con_debug_leave)(struct vc_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct consw {
    struct module *owner;
    const char * (*con_startup)();
    void (*con_init)(struct vc_data *, int);
    void (*con_deinit)(struct vc_data *);
    void (*con_clear)(struct vc_data *, int, int, int, int);
    void (*con_putc)(struct vc_data *, int, int, int);
    void (*con_putcs)(struct vc_data *, const short unsigned int *, int, int, int);
    void (*con_cursor)(struct vc_data *, int);
    bool (*con_scroll)(struct vc_data *, unsigned int, unsigned int, enum con_scroll, unsigned int);
    int (*con_switch)(struct vc_data *);
    int (*con_blank)(struct vc_data *, int, int);
    int (*con_font_set)(struct vc_data *, struct console_font *, unsigned int);
    int (*con_font_get)(struct vc_data *, struct console_font *);
    int (*con_font_default)(struct vc_data *, struct console_font *, char *);
    int (*con_font_copy)(struct vc_data *, int);
    int (*con_resize)(struct vc_data *, unsigned int, unsigned int, unsigned int);
    void (*con_set_palette)(struct vc_data *, const unsigned char *);
    void (*con_scrolldelta)(struct vc_data *, int);
    int (*con_set_origin)(struct vc_data *);
    void (*con_save_screen)(struct vc_data *);
    u8 (*con_build_attr)(struct vc_data *, u8, u8, u8, u8, u8, u8);
    void (*con_invert_region)(struct vc_data *, u16 *, int);
    u16 * (*con_screen_pos)(struct vc_data *, int);
    long unsigned int (*con_getxy)(struct vc_data *, long unsigned int, int *, int *);
    void (*con_flush_scrollback)(struct vc_data *);
    int (*con_debug_enter)(struct vc_data *);
    int (*con_debug_leave)(struct vc_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct consw {
    struct module *owner;
    const char * (*con_startup)();
    void (*con_init)(struct vc_data *, int);
    void (*con_deinit)(struct vc_data *);
    void (*con_clear)(struct vc_data *, int, int, int, int);
    void (*con_putc)(struct vc_data *, int, int, int);
    void (*con_putcs)(struct vc_data *, const short unsigned int *, int, int, int);
    void (*con_cursor)(struct vc_data *, int);
    bool (*con_scroll)(struct vc_data *, unsigned int, unsigned int, enum con_scroll, unsigned int);
    int (*con_switch)(struct vc_data *);
    int (*con_blank)(struct vc_data *, int, int);
    int (*con_font_set)(struct vc_data *, struct console_font *, unsigned int);
    int (*con_font_get)(struct vc_data *, struct console_font *);
    int (*con_font_default)(struct vc_data *, struct console_font *, char *);
    int (*con_font_copy)(struct vc_data *, int);
    int (*con_resize)(struct vc_data *, unsigned int, unsigned int, unsigned int);
    void (*con_set_palette)(struct vc_data *, const unsigned char *);
    void (*con_scrolldelta)(struct vc_data *, int);
    int (*con_set_origin)(struct vc_data *);
    void (*con_save_screen)(struct vc_data *);
    u8 (*con_build_attr)(struct vc_data *, u8, u8, u8, u8, u8, u8);
    void (*con_invert_region)(struct vc_data *, u16 *, int);
    u16 * (*con_screen_pos)(struct vc_data *, int);
    long unsigned int (*con_getxy)(struct vc_data *, long unsigned int, int *, int *);
    void (*con_flush_scrollback)(struct vc_data *);
    int (*con_debug_enter)(struct vc_data *);
    int (*con_debug_leave)(struct vc_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct consw {
    struct module *owner;
    const char * (*con_startup)();
    void (*con_init)(struct vc_data *, int);
    void (*con_deinit)(struct vc_data *);
    void (*con_clear)(struct vc_data *, int, int, int, int);
    void (*con_putc)(struct vc_data *, int, int, int);
    void (*con_putcs)(struct vc_data *, const short unsigned int *, int, int, int);
    void (*con_cursor)(struct vc_data *, int);
    bool (*con_scroll)(struct vc_data *, unsigned int, unsigned int, enum con_scroll, unsigned int);
    int (*con_switch)(struct vc_data *);
    int (*con_blank)(struct vc_data *, int, int);
    int (*con_font_set)(struct vc_data *, struct console_font *, unsigned int);
    int (*con_font_get)(struct vc_data *, struct console_font *);
    int (*con_font_default)(struct vc_data *, struct console_font *, char *);
    int (*con_font_copy)(struct vc_data *, int);
    int (*con_resize)(struct vc_data *, unsigned int, unsigned int, unsigned int);
    void (*con_set_palette)(struct vc_data *, const unsigned char *);
    void (*con_scrolldelta)(struct vc_data *, int);
    int (*con_set_origin)(struct vc_data *);
    void (*con_save_screen)(struct vc_data *);
    u8 (*con_build_attr)(struct vc_data *, u8, u8, u8, u8, u8, u8);
    void (*con_invert_region)(struct vc_data *, u16 *, int);
    u16 * (*con_screen_pos)(struct vc_data *, int);
    long unsigned int (*con_getxy)(struct vc_data *, long unsigned int, int *, int *);
    void (*con_flush_scrollback)(struct vc_data *);
    int (*con_debug_enter)(struct vc_data *);
    int (*con_debug_leave)(struct vc_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct consw {
    struct module *owner;
    const char * (*con_startup)();
    void (*con_init)(struct vc_data *, int);
    void (*con_deinit)(struct vc_data *);
    void (*con_clear)(struct vc_data *, int, int, int, int);
    void (*con_putc)(struct vc_data *, int, int, int);
    void (*con_putcs)(struct vc_data *, const short unsigned int *, int, int, int);
    void (*con_cursor)(struct vc_data *, int);
    bool (*con_scroll)(struct vc_data *, unsigned int, unsigned int, enum con_scroll, unsigned int);
    int (*con_switch)(struct vc_data *);
    int (*con_blank)(struct vc_data *, int, int);
    int (*con_font_set)(struct vc_data *, struct console_font *, unsigned int);
    int (*con_font_get)(struct vc_data *, struct console_font *);
    int (*con_font_default)(struct vc_data *, struct console_font *, char *);
    int (*con_font_copy)(struct vc_data *, int);
    int (*con_resize)(struct vc_data *, unsigned int, unsigned int, unsigned int);
    void (*con_set_palette)(struct vc_data *, const unsigned char *);
    void (*con_scrolldelta)(struct vc_data *, int);
    int (*con_set_origin)(struct vc_data *);
    void (*con_save_screen)(struct vc_data *);
    u8 (*con_build_attr)(struct vc_data *, u8, u8, u8, u8, u8, u8);
    void (*con_invert_region)(struct vc_data *, u16 *, int);
    u16 * (*con_screen_pos)(struct vc_data *, int);
    long unsigned int (*con_getxy)(struct vc_data *, long unsigned int, int *, int *);
    void (*con_flush_scrollback)(struct vc_data *);
    int (*con_debug_enter)(struct vc_data *);
    int (*con_debug_leave)(struct vc_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct consw {
    struct module *owner;
    const char * (*con_startup)();
    void (*con_init)(struct vc_data *, int);
    void (*con_deinit)(struct vc_data *);
    void (*con_clear)(struct vc_data *, int, int, int, int);
    void (*con_putc)(struct vc_data *, int, int, int);
    void (*con_putcs)(struct vc_data *, const short unsigned int *, int, int, int);
    void (*con_cursor)(struct vc_data *, int);
    bool (*con_scroll)(struct vc_data *, unsigned int, unsigned int, enum con_scroll, unsigned int);
    int (*con_switch)(struct vc_data *);
    int (*con_blank)(struct vc_data *, int, int);
    int (*con_font_set)(struct vc_data *, struct console_font *, unsigned int);
    int (*con_font_get)(struct vc_data *, struct console_font *);
    int (*con_font_default)(struct vc_data *, struct console_font *, char *);
    int (*con_font_copy)(struct vc_data *, int);
    int (*con_resize)(struct vc_data *, unsigned int, unsigned int, unsigned int);
    void (*con_set_palette)(struct vc_data *, const unsigned char *);
    void (*con_scrolldelta)(struct vc_data *, int);
    int (*con_set_origin)(struct vc_data *);
    void (*con_save_screen)(struct vc_data *);
    u8 (*con_build_attr)(struct vc_data *, u8, u8, u8, u8, u8, u8);
    void (*con_invert_region)(struct vc_data *, u16 *, int);
    u16 * (*con_screen_pos)(struct vc_data *, int);
    long unsigned int (*con_getxy)(struct vc_data *, long unsigned int, int *, int *);
    void (*con_flush_scrollback)(struct vc_data *);
    int (*con_debug_enter)(struct vc_data *);
    int (*con_debug_leave)(struct vc_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct consw {
    struct module *owner;
    const char * (*con_startup)();
    void (*con_init)(struct vc_data *, int);
    void (*con_deinit)(struct vc_data *);
    void (*con_clear)(struct vc_data *, int, int, int, int);
    void (*con_putc)(struct vc_data *, int, int, int);
    void (*con_putcs)(struct vc_data *, const short unsigned int *, int, int, int);
    void (*con_cursor)(struct vc_data *, int);
    bool (*con_scroll)(struct vc_data *, unsigned int, unsigned int, enum con_scroll, unsigned int);
    int (*con_switch)(struct vc_data *);
    int (*con_blank)(struct vc_data *, int, int);
    int (*con_font_set)(struct vc_data *, struct console_font *, unsigned int);
    int (*con_font_get)(struct vc_data *, struct console_font *);
    int (*con_font_default)(struct vc_data *, struct console_font *, char *);
    int (*con_font_copy)(struct vc_data *, int);
    int (*con_resize)(struct vc_data *, unsigned int, unsigned int, unsigned int);
    void (*con_set_palette)(struct vc_data *, const unsigned char *);
    void (*con_scrolldelta)(struct vc_data *, int);
    int (*con_set_origin)(struct vc_data *);
    void (*con_save_screen)(struct vc_data *);
    u8 (*con_build_attr)(struct vc_data *, u8, u8, u8, u8, u8, u8);
    void (*con_invert_region)(struct vc_data *, u16 *, int);
    u16 * (*con_screen_pos)(struct vc_data *, int);
    long unsigned int (*con_getxy)(struct vc_data *, long unsigned int, int *, int *);
    void (*con_flush_scrollback)(struct vc_data *);
    int (*con_debug_enter)(struct vc_data *);
    int (*con_debug_leave)(struct vc_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct consw {
    struct module *owner;
    const char * (*con_startup)();
    void (*con_init)(struct vc_data *, int);
    void (*con_deinit)(struct vc_data *);
    void (*con_clear)(struct vc_data *, int, int, int, int);
    void (*con_putc)(struct vc_data *, int, int, int);
    void (*con_putcs)(struct vc_data *, const short unsigned int *, int, int, int);
    void (*con_cursor)(struct vc_data *, int);
    bool (*con_scroll)(struct vc_data *, unsigned int, unsigned int, enum con_scroll, unsigned int);
    int (*con_switch)(struct vc_data *);
    int (*con_blank)(struct vc_data *, int, int);
    int (*con_font_set)(struct vc_data *, struct console_font *, unsigned int);
    int (*con_font_get)(struct vc_data *, struct console_font *);
    int (*con_font_default)(struct vc_data *, struct console_font *, char *);
    int (*con_font_copy)(struct vc_data *, int);
    int (*con_resize)(struct vc_data *, unsigned int, unsigned int, unsigned int);
    void (*con_set_palette)(struct vc_data *, const unsigned char *);
    void (*con_scrolldelta)(struct vc_data *, int);
    int (*con_set_origin)(struct vc_data *);
    void (*con_save_screen)(struct vc_data *);
    u8 (*con_build_attr)(struct vc_data *, u8, u8, u8, u8, u8, u8);
    void (*con_invert_region)(struct vc_data *, u16 *, int);
    u16 * (*con_screen_pos)(struct vc_data *, int);
    long unsigned int (*con_getxy)(struct vc_data *, long unsigned int, int *, int *);
    void (*con_flush_scrollback)(struct vc_data *);
    int (*con_debug_enter)(struct vc_data *);
    int (*con_debug_leave)(struct vc_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct consw {
    struct module *owner;
    const char * (*con_startup)();
    void (*con_init)(struct vc_data *, int);
    void (*con_deinit)(struct vc_data *);
    void (*con_clear)(struct vc_data *, int, int, int, int);
    void (*con_putc)(struct vc_data *, int, int, int);
    void (*con_putcs)(struct vc_data *, const short unsigned int *, int, int, int);
    void (*con_cursor)(struct vc_data *, int);
    bool (*con_scroll)(struct vc_data *, unsigned int, unsigned int, enum con_scroll, unsigned int);
    int (*con_switch)(struct vc_data *);
    int (*con_blank)(struct vc_data *, int, int);
    int (*con_font_set)(struct vc_data *, struct console_font *, unsigned int);
    int (*con_font_get)(struct vc_data *, struct console_font *);
    int (*con_font_default)(struct vc_data *, struct console_font *, char *);
    int (*con_resize)(struct vc_data *, unsigned int, unsigned int, unsigned int);
    void (*con_set_palette)(struct vc_data *, const unsigned char *);
    void (*con_scrolldelta)(struct vc_data *, int);
    int (*con_set_origin)(struct vc_data *);
    void (*con_save_screen)(struct vc_data *);
    u8 (*con_build_attr)(struct vc_data *, u8, enum vc_intensity, bool, bool, bool, bool);
    void (*con_invert_region)(struct vc_data *, u16 *, int);
    u16 * (*con_screen_pos)(const struct vc_data *, int);
    long unsigned int (*con_getxy)(struct vc_data *, long unsigned int, int *, int *);
    void (*con_flush_scrollback)(struct vc_data *);
    int (*con_debug_enter)(struct vc_data *);
    int (*con_debug_leave)(struct vc_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct consw {
    struct module *owner;
    const char * (*con_startup)();
    void (*con_init)(struct vc_data *, int);
    void (*con_deinit)(struct vc_data *);
    void (*con_clear)(struct vc_data *, int, int, int, int);
    void (*con_putc)(struct vc_data *, int, int, int);
    void (*con_putcs)(struct vc_data *, const short unsigned int *, int, int, int);
    void (*con_cursor)(struct vc_data *, int);
    bool (*con_scroll)(struct vc_data *, unsigned int, unsigned int, enum con_scroll, unsigned int);
    int (*con_switch)(struct vc_data *);
    int (*con_blank)(struct vc_data *, int, int);
    int (*con_font_set)(struct vc_data *, struct console_font *, unsigned int);
    int (*con_font_get)(struct vc_data *, struct console_font *);
    int (*con_font_default)(struct vc_data *, struct console_font *, char *);
    int (*con_resize)(struct vc_data *, unsigned int, unsigned int, unsigned int);
    void (*con_set_palette)(struct vc_data *, const unsigned char *);
    void (*con_scrolldelta)(struct vc_data *, int);
    int (*con_set_origin)(struct vc_data *);
    void (*con_save_screen)(struct vc_data *);
    u8 (*con_build_attr)(struct vc_data *, u8, enum vc_intensity, bool, bool, bool, bool);
    void (*con_invert_region)(struct vc_data *, u16 *, int);
    u16 * (*con_screen_pos)(const struct vc_data *, int);
    long unsigned int (*con_getxy)(struct vc_data *, long unsigned int, int *, int *);
    void (*con_flush_scrollback)(struct vc_data *);
    int (*con_debug_enter)(struct vc_data *);
    int (*con_debug_leave)(struct vc_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct consw {
    struct module *owner;
    const char * (*con_startup)();
    void (*con_init)(struct vc_data *, int);
    void (*con_deinit)(struct vc_data *);
    void (*con_clear)(struct vc_data *, int, int, int, int);
    void (*con_putc)(struct vc_data *, int, int, int);
    void (*con_putcs)(struct vc_data *, const short unsigned int *, int, int, int);
    void (*con_cursor)(struct vc_data *, int);
    bool (*con_scroll)(struct vc_data *, unsigned int, unsigned int, enum con_scroll, unsigned int);
    int (*con_switch)(struct vc_data *);
    int (*con_blank)(struct vc_data *, int, int);
    int (*con_font_set)(struct vc_data *, struct console_font *, unsigned int);
    int (*con_font_get)(struct vc_data *, struct console_font *);
    int (*con_font_default)(struct vc_data *, struct console_font *, char *);
    int (*con_resize)(struct vc_data *, unsigned int, unsigned int, unsigned int);
    void (*con_set_palette)(struct vc_data *, const unsigned char *);
    void (*con_scrolldelta)(struct vc_data *, int);
    int (*con_set_origin)(struct vc_data *);
    void (*con_save_screen)(struct vc_data *);
    u8 (*con_build_attr)(struct vc_data *, u8, enum vc_intensity, bool, bool, bool, bool);
    void (*con_invert_region)(struct vc_data *, u16 *, int);
    u16 * (*con_screen_pos)(const struct vc_data *, int);
    long unsigned int (*con_getxy)(struct vc_data *, long unsigned int, int *, int *);
    void (*con_flush_scrollback)(struct vc_data *);
    int (*con_debug_enter)(struct vc_data *);
    int (*con_debug_leave)(struct vc_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct consw {
    struct module *owner;
    const char * (*con_startup)();
    void (*con_init)(struct vc_data *, int);
    void (*con_deinit)(struct vc_data *);
    void (*con_clear)(struct vc_data *, int, int, int, int);
    void (*con_putc)(struct vc_data *, int, int, int);
    void (*con_putcs)(struct vc_data *, const short unsigned int *, int, int, int);
    void (*con_cursor)(struct vc_data *, int);
    bool (*con_scroll)(struct vc_data *, unsigned int, unsigned int, enum con_scroll, unsigned int);
    int (*con_switch)(struct vc_data *);
    int (*con_blank)(struct vc_data *, int, int);
    int (*con_font_set)(struct vc_data *, struct console_font *, unsigned int);
    int (*con_font_get)(struct vc_data *, struct console_font *);
    int (*con_font_default)(struct vc_data *, struct console_font *, char *);
    int (*con_resize)(struct vc_data *, unsigned int, unsigned int, unsigned int);
    void (*con_set_palette)(struct vc_data *, const unsigned char *);
    void (*con_scrolldelta)(struct vc_data *, int);
    int (*con_set_origin)(struct vc_data *);
    void (*con_save_screen)(struct vc_data *);
    u8 (*con_build_attr)(struct vc_data *, u8, enum vc_intensity, bool, bool, bool, bool);
    void (*con_invert_region)(struct vc_data *, u16 *, int);
    u16 * (*con_screen_pos)(const struct vc_data *, int);
    long unsigned int (*con_getxy)(struct vc_data *, long unsigned int, int *, int *);
    void (*con_flush_scrollback)(struct vc_data *);
    int (*con_debug_enter)(struct vc_data *);
    int (*con_debug_leave)(struct vc_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct consw {
    struct module *owner;
    const char * (*con_startup)();
    void (*con_init)(struct vc_data *, int);
    void (*con_deinit)(struct vc_data *);
    void (*con_clear)(struct vc_data *, int, int, int, int);
    void (*con_putc)(struct vc_data *, int, int, int);
    void (*con_putcs)(struct vc_data *, const short unsigned int *, int, int, int);
    void (*con_cursor)(struct vc_data *, int);
    bool (*con_scroll)(struct vc_data *, unsigned int, unsigned int, enum con_scroll, unsigned int);
    int (*con_switch)(struct vc_data *);
    int (*con_blank)(struct vc_data *, int, int);
    int (*con_font_set)(struct vc_data *, struct console_font *, unsigned int);
    int (*con_font_get)(struct vc_data *, struct console_font *);
    int (*con_font_default)(struct vc_data *, struct console_font *, char *);
    int (*con_resize)(struct vc_data *, unsigned int, unsigned int, unsigned int);
    void (*con_set_palette)(struct vc_data *, const unsigned char *);
    void (*con_scrolldelta)(struct vc_data *, int);
    int (*con_set_origin)(struct vc_data *);
    void (*con_save_screen)(struct vc_data *);
    u8 (*con_build_attr)(struct vc_data *, u8, enum vc_intensity, bool, bool, bool, bool);
    void (*con_invert_region)(struct vc_data *, u16 *, int);
    u16 * (*con_screen_pos)(const struct vc_data *, int);
    long unsigned int (*con_getxy)(struct vc_data *, long unsigned int, int *, int *);
    void (*con_flush_scrollback)(struct vc_data *);
    int (*con_debug_enter)(struct vc_data *);
    int (*con_debug_leave)(struct vc_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct consw {
    struct module *owner;
    const char * (*con_startup)();
    void (*con_init)(struct vc_data *, int);
    void (*con_deinit)(struct vc_data *);
    void (*con_clear)(struct vc_data *, int, int, int, int);
    void (*con_putc)(struct vc_data *, int, int, int);
    void (*con_putcs)(struct vc_data *, const short unsigned int *, int, int, int);
    void (*con_cursor)(struct vc_data *, int);
    bool (*con_scroll)(struct vc_data *, unsigned int, unsigned int, enum con_scroll, unsigned int);
    int (*con_switch)(struct vc_data *);
    int (*con_blank)(struct vc_data *, int, int);
    int (*con_font_set)(struct vc_data *, struct console_font *, unsigned int, unsigned int);
    int (*con_font_get)(struct vc_data *, struct console_font *, unsigned int);
    int (*con_font_default)(struct vc_data *, struct console_font *, char *);
    int (*con_resize)(struct vc_data *, unsigned int, unsigned int, unsigned int);
    void (*con_set_palette)(struct vc_data *, const unsigned char *);
    void (*con_scrolldelta)(struct vc_data *, int);
    int (*con_set_origin)(struct vc_data *);
    void (*con_save_screen)(struct vc_data *);
    u8 (*con_build_attr)(struct vc_data *, u8, enum vc_intensity, bool, bool, bool, bool);
    void (*con_invert_region)(struct vc_data *, u16 *, int);
    u16 * (*con_screen_pos)(const struct vc_data *, int);
    long unsigned int (*con_getxy)(struct vc_data *, long unsigned int, int *, int *);
    void (*con_flush_scrollback)(struct vc_data *);
    int (*con_debug_enter)(struct vc_data *);
    int (*con_debug_leave)(struct vc_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct consw {
    struct module *owner;
    const char * (*con_startup)();
    void (*con_init)(struct vc_data *, int);
    void (*con_deinit)(struct vc_data *);
    void (*con_clear)(struct vc_data *, int, int, int, int);
    void (*con_putc)(struct vc_data *, int, int, int);
    void (*con_putcs)(struct vc_data *, const short unsigned int *, int, int, int);
    void (*con_cursor)(struct vc_data *, int);
    bool (*con_scroll)(struct vc_data *, unsigned int, unsigned int, enum con_scroll, unsigned int);
    int (*con_switch)(struct vc_data *);
    int (*con_blank)(struct vc_data *, int, int);
    int (*con_font_set)(struct vc_data *, struct console_font *, unsigned int, unsigned int);
    int (*con_font_get)(struct vc_data *, struct console_font *, unsigned int);
    int (*con_font_default)(struct vc_data *, struct console_font *, char *);
    int (*con_resize)(struct vc_data *, unsigned int, unsigned int, unsigned int);
    void (*con_set_palette)(struct vc_data *, const unsigned char *);
    void (*con_scrolldelta)(struct vc_data *, int);
    int (*con_set_origin)(struct vc_data *);
    void (*con_save_screen)(struct vc_data *);
    u8 (*con_build_attr)(struct vc_data *, u8, enum vc_intensity, bool, bool, bool, bool);
    void (*con_invert_region)(struct vc_data *, u16 *, int);
    u16 * (*con_screen_pos)(const struct vc_data *, int);
    long unsigned int (*con_getxy)(struct vc_data *, long unsigned int, int *, int *);
    void (*con_flush_scrollback)(struct vc_data *);
    int (*con_debug_enter)(struct vc_data *);
    int (*con_debug_leave)(struct vc_data *);
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
struct consw {
    struct module *owner;
    const char * (*con_startup)();
    void (*con_init)(struct vc_data *, int);
    void (*con_deinit)(struct vc_data *);
    void (*con_clear)(struct vc_data *, int, int, int, int);
    void (*con_putc)(struct vc_data *, int, int, int);
    void (*con_putcs)(struct vc_data *, const short unsigned int *, int, int, int);
    void (*con_cursor)(struct vc_data *, int);
    bool (*con_scroll)(struct vc_data *, unsigned int, unsigned int, enum con_scroll, unsigned int);
    int (*con_switch)(struct vc_data *);
    int (*con_blank)(struct vc_data *, int, int);
    int (*con_font_set)(struct vc_data *, struct console_font *, unsigned int);
    int (*con_font_get)(struct vc_data *, struct console_font *);
    int (*con_font_default)(struct vc_data *, struct console_font *, char *);
    int (*con_font_copy)(struct vc_data *, int);
    int (*con_resize)(struct vc_data *, unsigned int, unsigned int, unsigned int);
    void (*con_set_palette)(struct vc_data *, const unsigned char *);
    void (*con_scrolldelta)(struct vc_data *, int);
    int (*con_set_origin)(struct vc_data *);
    void (*con_save_screen)(struct vc_data *);
    u8 (*con_build_attr)(struct vc_data *, u8, u8, u8, u8, u8, u8);
    void (*con_invert_region)(struct vc_data *, u16 *, int);
    u16 * (*con_screen_pos)(struct vc_data *, int);
    long unsigned int (*con_getxy)(struct vc_data *, long unsigned int, int *, int *);
    void (*con_flush_scrollback)(struct vc_data *);
    int (*con_debug_enter)(struct vc_data *);
    int (*con_debug_leave)(struct vc_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct consw {
    struct module *owner;
    const char * (*con_startup)();
    void (*con_init)(struct vc_data *, int);
    void (*con_deinit)(struct vc_data *);
    void (*con_clear)(struct vc_data *, int, int, int, int);
    void (*con_putc)(struct vc_data *, int, int, int);
    void (*con_putcs)(struct vc_data *, const short unsigned int *, int, int, int);
    void (*con_cursor)(struct vc_data *, int);
    bool (*con_scroll)(struct vc_data *, unsigned int, unsigned int, enum con_scroll, unsigned int);
    int (*con_switch)(struct vc_data *);
    int (*con_blank)(struct vc_data *, int, int);
    int (*con_font_set)(struct vc_data *, struct console_font *, unsigned int);
    int (*con_font_get)(struct vc_data *, struct console_font *);
    int (*con_font_default)(struct vc_data *, struct console_font *, char *);
    int (*con_font_copy)(struct vc_data *, int);
    int (*con_resize)(struct vc_data *, unsigned int, unsigned int, unsigned int);
    void (*con_set_palette)(struct vc_data *, const unsigned char *);
    void (*con_scrolldelta)(struct vc_data *, int);
    int (*con_set_origin)(struct vc_data *);
    void (*con_save_screen)(struct vc_data *);
    u8 (*con_build_attr)(struct vc_data *, u8, u8, u8, u8, u8, u8);
    void (*con_invert_region)(struct vc_data *, u16 *, int);
    u16 * (*con_screen_pos)(struct vc_data *, int);
    long unsigned int (*con_getxy)(struct vc_data *, long unsigned int, int *, int *);
    void (*con_flush_scrollback)(struct vc_data *);
    int (*con_debug_enter)(struct vc_data *);
    int (*con_debug_leave)(struct vc_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct consw {
    struct module *owner;
    const char * (*con_startup)();
    void (*con_init)(struct vc_data *, int);
    void (*con_deinit)(struct vc_data *);
    void (*con_clear)(struct vc_data *, int, int, int, int);
    void (*con_putc)(struct vc_data *, int, int, int);
    void (*con_putcs)(struct vc_data *, const short unsigned int *, int, int, int);
    void (*con_cursor)(struct vc_data *, int);
    bool (*con_scroll)(struct vc_data *, unsigned int, unsigned int, enum con_scroll, unsigned int);
    int (*con_switch)(struct vc_data *);
    int (*con_blank)(struct vc_data *, int, int);
    int (*con_font_set)(struct vc_data *, struct console_font *, unsigned int);
    int (*con_font_get)(struct vc_data *, struct console_font *);
    int (*con_font_default)(struct vc_data *, struct console_font *, char *);
    int (*con_font_copy)(struct vc_data *, int);
    int (*con_resize)(struct vc_data *, unsigned int, unsigned int, unsigned int);
    void (*con_set_palette)(struct vc_data *, const unsigned char *);
    void (*con_scrolldelta)(struct vc_data *, int);
    int (*con_set_origin)(struct vc_data *);
    void (*con_save_screen)(struct vc_data *);
    u8 (*con_build_attr)(struct vc_data *, u8, u8, u8, u8, u8, u8);
    void (*con_invert_region)(struct vc_data *, u16 *, int);
    u16 * (*con_screen_pos)(struct vc_data *, int);
    long unsigned int (*con_getxy)(struct vc_data *, long unsigned int, int *, int *);
    void (*con_flush_scrollback)(struct vc_data *);
    int (*con_debug_enter)(struct vc_data *);
    int (*con_debug_leave)(struct vc_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct consw {
    struct module *owner;
    const char * (*con_startup)();
    void (*con_init)(struct vc_data *, int);
    void (*con_deinit)(struct vc_data *);
    void (*con_clear)(struct vc_data *, int, int, int, int);
    void (*con_putc)(struct vc_data *, int, int, int);
    void (*con_putcs)(struct vc_data *, const short unsigned int *, int, int, int);
    void (*con_cursor)(struct vc_data *, int);
    bool (*con_scroll)(struct vc_data *, unsigned int, unsigned int, enum con_scroll, unsigned int);
    int (*con_switch)(struct vc_data *);
    int (*con_blank)(struct vc_data *, int, int);
    int (*con_font_set)(struct vc_data *, struct console_font *, unsigned int);
    int (*con_font_get)(struct vc_data *, struct console_font *);
    int (*con_font_default)(struct vc_data *, struct console_font *, char *);
    int (*con_font_copy)(struct vc_data *, int);
    int (*con_resize)(struct vc_data *, unsigned int, unsigned int, unsigned int);
    void (*con_set_palette)(struct vc_data *, const unsigned char *);
    void (*con_scrolldelta)(struct vc_data *, int);
    int (*con_set_origin)(struct vc_data *);
    void (*con_save_screen)(struct vc_data *);
    u8 (*con_build_attr)(struct vc_data *, u8, u8, u8, u8, u8, u8);
    void (*con_invert_region)(struct vc_data *, u16 *, int);
    u16 * (*con_screen_pos)(struct vc_data *, int);
    long unsigned int (*con_getxy)(struct vc_data *, long unsigned int, int *, int *);
    void (*con_flush_scrollback)(struct vc_data *);
    int (*con_debug_enter)(struct vc_data *);
    int (*con_debug_leave)(struct vc_data *);
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
struct consw {
    struct module *owner;
    const char * (*con_startup)();
    void (*con_init)(struct vc_data *, int);
    void (*con_deinit)(struct vc_data *);
    void (*con_clear)(struct vc_data *, int, int, int, int);
    void (*con_putc)(struct vc_data *, int, int, int);
    void (*con_putcs)(struct vc_data *, const short unsigned int *, int, int, int);
    void (*con_cursor)(struct vc_data *, int);
    bool (*con_scroll)(struct vc_data *, unsigned int, unsigned int, enum con_scroll, unsigned int);
    int (*con_switch)(struct vc_data *);
    int (*con_blank)(struct vc_data *, int, int);
    int (*con_font_set)(struct vc_data *, struct console_font *, unsigned int);
    int (*con_font_get)(struct vc_data *, struct console_font *);
    int (*con_font_default)(struct vc_data *, struct console_font *, char *);
    int (*con_font_copy)(struct vc_data *, int);
    int (*con_resize)(struct vc_data *, unsigned int, unsigned int, unsigned int);
    void (*con_set_palette)(struct vc_data *, const unsigned char *);
    void (*con_scrolldelta)(struct vc_data *, int);
    int (*con_set_origin)(struct vc_data *);
    void (*con_save_screen)(struct vc_data *);
    u8 (*con_build_attr)(struct vc_data *, u8, u8, u8, u8, u8, u8);
    void (*con_invert_region)(struct vc_data *, u16 *, int);
    u16 * (*con_screen_pos)(struct vc_data *, int);
    long unsigned int (*con_getxy)(struct vc_data *, long unsigned int, int *, int *);
    void (*con_flush_scrollback)(struct vc_data *);
    int (*con_debug_enter)(struct vc_data *);
    int (*con_debug_leave)(struct vc_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct consw {
    struct module *owner;
    const char * (*con_startup)();
    void (*con_init)(struct vc_data *, int);
    void (*con_deinit)(struct vc_data *);
    void (*con_clear)(struct vc_data *, int, int, int, int);
    void (*con_putc)(struct vc_data *, int, int, int);
    void (*con_putcs)(struct vc_data *, const short unsigned int *, int, int, int);
    void (*con_cursor)(struct vc_data *, int);
    bool (*con_scroll)(struct vc_data *, unsigned int, unsigned int, enum con_scroll, unsigned int);
    int (*con_switch)(struct vc_data *);
    int (*con_blank)(struct vc_data *, int, int);
    int (*con_font_set)(struct vc_data *, struct console_font *, unsigned int);
    int (*con_font_get)(struct vc_data *, struct console_font *);
    int (*con_font_default)(struct vc_data *, struct console_font *, char *);
    int (*con_font_copy)(struct vc_data *, int);
    int (*con_resize)(struct vc_data *, unsigned int, unsigned int, unsigned int);
    void (*con_set_palette)(struct vc_data *, const unsigned char *);
    void (*con_scrolldelta)(struct vc_data *, int);
    int (*con_set_origin)(struct vc_data *);
    void (*con_save_screen)(struct vc_data *);
    u8 (*con_build_attr)(struct vc_data *, u8, u8, u8, u8, u8, u8);
    void (*con_invert_region)(struct vc_data *, u16 *, int);
    u16 * (*con_screen_pos)(struct vc_data *, int);
    long unsigned int (*con_getxy)(struct vc_data *, long unsigned int, int *, int *);
    void (*con_flush_scrollback)(struct vc_data *);
    int (*con_debug_enter)(struct vc_data *);
    int (*con_debug_leave)(struct vc_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct consw {
    struct module *owner;
    const char * (*con_startup)();
    void (*con_init)(struct vc_data *, int);
    void (*con_deinit)(struct vc_data *);
    void (*con_clear)(struct vc_data *, int, int, int, int);
    void (*con_putc)(struct vc_data *, int, int, int);
    void (*con_putcs)(struct vc_data *, const short unsigned int *, int, int, int);
    void (*con_cursor)(struct vc_data *, int);
    bool (*con_scroll)(struct vc_data *, unsigned int, unsigned int, enum con_scroll, unsigned int);
    int (*con_switch)(struct vc_data *);
    int (*con_blank)(struct vc_data *, int, int);
    int (*con_font_set)(struct vc_data *, struct console_font *, unsigned int);
    int (*con_font_get)(struct vc_data *, struct console_font *);
    int (*con_font_default)(struct vc_data *, struct console_font *, char *);
    int (*con_font_copy)(struct vc_data *, int);
    int (*con_resize)(struct vc_data *, unsigned int, unsigned int, unsigned int);
    void (*con_set_palette)(struct vc_data *, const unsigned char *);
    void (*con_scrolldelta)(struct vc_data *, int);
    int (*con_set_origin)(struct vc_data *);
    void (*con_save_screen)(struct vc_data *);
    u8 (*con_build_attr)(struct vc_data *, u8, u8, u8, u8, u8, u8);
    void (*con_invert_region)(struct vc_data *, u16 *, int);
    u16 * (*con_screen_pos)(struct vc_data *, int);
    long unsigned int (*con_getxy)(struct vc_data *, long unsigned int, int *, int *);
    void (*con_flush_scrollback)(struct vc_data *);
    int (*con_debug_enter)(struct vc_data *);
    int (*con_debug_leave)(struct vc_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct consw {
    struct module *owner;
    const char * (*con_startup)();
    void (*con_init)(struct vc_data *, int);
    void (*con_deinit)(struct vc_data *);
    void (*con_clear)(struct vc_data *, int, int, int, int);
    void (*con_putc)(struct vc_data *, int, int, int);
    void (*con_putcs)(struct vc_data *, const short unsigned int *, int, int, int);
    void (*con_cursor)(struct vc_data *, int);
    bool (*con_scroll)(struct vc_data *, unsigned int, unsigned int, enum con_scroll, unsigned int);
    int (*con_switch)(struct vc_data *);
    int (*con_blank)(struct vc_data *, int, int);
    int (*con_font_set)(struct vc_data *, struct console_font *, unsigned int);
    int (*con_font_get)(struct vc_data *, struct console_font *);
    int (*con_font_default)(struct vc_data *, struct console_font *, char *);
    int (*con_font_copy)(struct vc_data *, int);
    int (*con_resize)(struct vc_data *, unsigned int, unsigned int, unsigned int);
    void (*con_set_palette)(struct vc_data *, const unsigned char *);
    void (*con_scrolldelta)(struct vc_data *, int);
    int (*con_set_origin)(struct vc_data *);
    void (*con_save_screen)(struct vc_data *);
    u8 (*con_build_attr)(struct vc_data *, u8, u8, u8, u8, u8, u8);
    void (*con_invert_region)(struct vc_data *, u16 *, int);
    u16 * (*con_screen_pos)(struct vc_data *, int);
    long unsigned int (*con_getxy)(struct vc_data *, long unsigned int, int *, int *);
    void (*con_flush_scrollback)(struct vc_data *);
    int (*con_debug_enter)(struct vc_data *);
    int (*con_debug_leave)(struct vc_data *);
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
<code>void (*con_bmove)(struct vc_data *, int, int, int, int, int, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*con_set_palette)(struct vc_data *, unsigned char *)</code> ➡️ <code>void (*con_set_palette)(struct vc_data *, const unsigned char *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*con_scrolldelta)(struct vc_data *, int)</code> ➡️ <code>void (*con_scrolldelta)(struct vc_data *, int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*con_scroll)(struct vc_data *, int, int, int, int)</code> ➡️ <code>bool (*con_scroll)(struct vc_data *, unsigned int, unsigned int, enum con_scroll, unsigned int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*con_flush_scrollback)(struct vc_data *)</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*con_font_copy)(struct vc_data *, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 (*con_build_attr)(struct vc_data *, u8, u8, u8, u8, u8, u8)</code> ➡️ <code>u8 (*con_build_attr)(struct vc_data *, u8, enum vc_intensity, bool, bool, bool, bool)</code>
</li>
<li>
<b>Field type changed. </b>
<code>u16 * (*con_screen_pos)(struct vc_data *, int)</code> ➡️ <code>u16 * (*con_screen_pos)(const struct vc_data *, int)</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*con_font_set)(struct vc_data *, struct console_font *, unsigned int)</code> ➡️ <code>int (*con_font_set)(struct vc_data *, struct console_font *, unsigned int, unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*con_font_get)(struct vc_data *, struct console_font *)</code> ➡️ <code>int (*con_font_get)(struct vc_data *, struct console_font *, unsigned int)</code>
</li>
</ul>
</details>
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
