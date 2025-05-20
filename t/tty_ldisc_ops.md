# Struct: <code>tty_ldisc_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct tty_ldisc_ops {
    int magic;
    char *name;
    int num;
    int flags;
    int (*open)(struct tty_struct *);
    void (*close)(struct tty_struct *);
    void (*flush_buffer)(struct tty_struct *);
    ssize_t (*chars_in_buffer)(struct tty_struct *);
    ssize_t (*read)(struct tty_struct *, struct file *, unsigned char *, size_t);
    ssize_t (*write)(struct tty_struct *, struct file *, const unsigned char *, size_t);
    int (*ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    unsigned int (*poll)(struct tty_struct *, struct file *, struct poll_table_struct *);
    int (*hangup)(struct tty_struct *);
    void (*receive_buf)(struct tty_struct *, const unsigned char *, char *, int);
    void (*write_wakeup)(struct tty_struct *);
    void (*dcd_change)(struct tty_struct *, unsigned int);
    void (*fasync)(struct tty_struct *, int);
    int (*receive_buf2)(struct tty_struct *, const unsigned char *, char *, int);
    struct module *owner;
    int refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct tty_ldisc_ops {
    int magic;
    char *name;
    int num;
    int flags;
    int (*open)(struct tty_struct *);
    void (*close)(struct tty_struct *);
    void (*flush_buffer)(struct tty_struct *);
    ssize_t (*read)(struct tty_struct *, struct file *, unsigned char *, size_t);
    ssize_t (*write)(struct tty_struct *, struct file *, const unsigned char *, size_t);
    int (*ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    unsigned int (*poll)(struct tty_struct *, struct file *, struct poll_table_struct *);
    int (*hangup)(struct tty_struct *);
    void (*receive_buf)(struct tty_struct *, const unsigned char *, char *, int);
    void (*write_wakeup)(struct tty_struct *);
    void (*dcd_change)(struct tty_struct *, unsigned int);
    int (*receive_buf2)(struct tty_struct *, const unsigned char *, char *, int);
    struct module *owner;
    int refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct tty_ldisc_ops {
    int magic;
    char *name;
    int num;
    int flags;
    int (*open)(struct tty_struct *);
    void (*close)(struct tty_struct *);
    void (*flush_buffer)(struct tty_struct *);
    ssize_t (*read)(struct tty_struct *, struct file *, unsigned char *, size_t);
    ssize_t (*write)(struct tty_struct *, struct file *, const unsigned char *, size_t);
    int (*ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    unsigned int (*poll)(struct tty_struct *, struct file *, struct poll_table_struct *);
    int (*hangup)(struct tty_struct *);
    void (*receive_buf)(struct tty_struct *, const unsigned char *, char *, int);
    void (*write_wakeup)(struct tty_struct *);
    void (*dcd_change)(struct tty_struct *, unsigned int);
    int (*receive_buf2)(struct tty_struct *, const unsigned char *, char *, int);
    struct module *owner;
    int refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct tty_ldisc_ops {
    int magic;
    char *name;
    int num;
    int flags;
    int (*open)(struct tty_struct *);
    void (*close)(struct tty_struct *);
    void (*flush_buffer)(struct tty_struct *);
    ssize_t (*read)(struct tty_struct *, struct file *, unsigned char *, size_t);
    ssize_t (*write)(struct tty_struct *, struct file *, const unsigned char *, size_t);
    int (*ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    unsigned int (*poll)(struct tty_struct *, struct file *, struct poll_table_struct *);
    int (*hangup)(struct tty_struct *);
    void (*receive_buf)(struct tty_struct *, const unsigned char *, char *, int);
    void (*write_wakeup)(struct tty_struct *);
    void (*dcd_change)(struct tty_struct *, unsigned int);
    int (*receive_buf2)(struct tty_struct *, const unsigned char *, char *, int);
    struct module *owner;
    int refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct tty_ldisc_ops {
    int magic;
    char *name;
    int num;
    int flags;
    int (*open)(struct tty_struct *);
    void (*close)(struct tty_struct *);
    void (*flush_buffer)(struct tty_struct *);
    ssize_t (*read)(struct tty_struct *, struct file *, unsigned char *, size_t);
    ssize_t (*write)(struct tty_struct *, struct file *, const unsigned char *, size_t);
    int (*ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    unsigned int (*poll)(struct tty_struct *, struct file *, struct poll_table_struct *);
    int (*hangup)(struct tty_struct *);
    void (*receive_buf)(struct tty_struct *, const unsigned char *, char *, int);
    void (*write_wakeup)(struct tty_struct *);
    void (*dcd_change)(struct tty_struct *, unsigned int);
    int (*receive_buf2)(struct tty_struct *, const unsigned char *, char *, int);
    struct module *owner;
    int refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct tty_ldisc_ops {
    int magic;
    char *name;
    int num;
    int flags;
    int (*open)(struct tty_struct *);
    void (*close)(struct tty_struct *);
    void (*flush_buffer)(struct tty_struct *);
    ssize_t (*read)(struct tty_struct *, struct file *, unsigned char *, size_t);
    ssize_t (*write)(struct tty_struct *, struct file *, const unsigned char *, size_t);
    int (*ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    __poll_t (*poll)(struct tty_struct *, struct file *, struct poll_table_struct *);
    int (*hangup)(struct tty_struct *);
    void (*receive_buf)(struct tty_struct *, const unsigned char *, char *, int);
    void (*write_wakeup)(struct tty_struct *);
    void (*dcd_change)(struct tty_struct *, unsigned int);
    int (*receive_buf2)(struct tty_struct *, const unsigned char *, char *, int);
    struct module *owner;
    int refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct tty_ldisc_ops {
    int magic;
    char *name;
    int num;
    int flags;
    int (*open)(struct tty_struct *);
    void (*close)(struct tty_struct *);
    void (*flush_buffer)(struct tty_struct *);
    ssize_t (*read)(struct tty_struct *, struct file *, unsigned char *, size_t);
    ssize_t (*write)(struct tty_struct *, struct file *, const unsigned char *, size_t);
    int (*ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    __poll_t (*poll)(struct tty_struct *, struct file *, struct poll_table_struct *);
    int (*hangup)(struct tty_struct *);
    void (*receive_buf)(struct tty_struct *, const unsigned char *, char *, int);
    void (*write_wakeup)(struct tty_struct *);
    void (*dcd_change)(struct tty_struct *, unsigned int);
    int (*receive_buf2)(struct tty_struct *, const unsigned char *, char *, int);
    struct module *owner;
    int refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct tty_ldisc_ops {
    int magic;
    char *name;
    int num;
    int flags;
    int (*open)(struct tty_struct *);
    void (*close)(struct tty_struct *);
    void (*flush_buffer)(struct tty_struct *);
    ssize_t (*read)(struct tty_struct *, struct file *, unsigned char *, size_t);
    ssize_t (*write)(struct tty_struct *, struct file *, const unsigned char *, size_t);
    int (*ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    __poll_t (*poll)(struct tty_struct *, struct file *, struct poll_table_struct *);
    int (*hangup)(struct tty_struct *);
    void (*receive_buf)(struct tty_struct *, const unsigned char *, char *, int);
    void (*write_wakeup)(struct tty_struct *);
    void (*dcd_change)(struct tty_struct *, unsigned int);
    int (*receive_buf2)(struct tty_struct *, const unsigned char *, char *, int);
    struct module *owner;
    int refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct tty_ldisc_ops {
    int magic;
    char *name;
    int num;
    int flags;
    int (*open)(struct tty_struct *);
    void (*close)(struct tty_struct *);
    void (*flush_buffer)(struct tty_struct *);
    ssize_t (*read)(struct tty_struct *, struct file *, unsigned char *, size_t);
    ssize_t (*write)(struct tty_struct *, struct file *, const unsigned char *, size_t);
    int (*ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    __poll_t (*poll)(struct tty_struct *, struct file *, struct poll_table_struct *);
    int (*hangup)(struct tty_struct *);
    void (*receive_buf)(struct tty_struct *, const unsigned char *, char *, int);
    void (*write_wakeup)(struct tty_struct *);
    void (*dcd_change)(struct tty_struct *, unsigned int);
    int (*receive_buf2)(struct tty_struct *, const unsigned char *, char *, int);
    struct module *owner;
    int refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct tty_ldisc_ops {
    int magic;
    char *name;
    int num;
    int flags;
    int (*open)(struct tty_struct *);
    void (*close)(struct tty_struct *);
    void (*flush_buffer)(struct tty_struct *);
    ssize_t (*read)(struct tty_struct *, struct file *, unsigned char *, size_t);
    ssize_t (*write)(struct tty_struct *, struct file *, const unsigned char *, size_t);
    int (*ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    __poll_t (*poll)(struct tty_struct *, struct file *, struct poll_table_struct *);
    int (*hangup)(struct tty_struct *);
    void (*receive_buf)(struct tty_struct *, const unsigned char *, char *, int);
    void (*write_wakeup)(struct tty_struct *);
    void (*dcd_change)(struct tty_struct *, unsigned int);
    int (*receive_buf2)(struct tty_struct *, const unsigned char *, char *, int);
    struct module *owner;
    int refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct tty_ldisc_ops {
    int magic;
    char *name;
    int num;
    int flags;
    int (*open)(struct tty_struct *);
    void (*close)(struct tty_struct *);
    void (*flush_buffer)(struct tty_struct *);
    ssize_t (*read)(struct tty_struct *, struct file *, unsigned char *, size_t, void **, long unsigned int);
    ssize_t (*write)(struct tty_struct *, struct file *, const unsigned char *, size_t);
    int (*ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    __poll_t (*poll)(struct tty_struct *, struct file *, struct poll_table_struct *);
    int (*hangup)(struct tty_struct *);
    void (*receive_buf)(struct tty_struct *, const unsigned char *, char *, int);
    void (*write_wakeup)(struct tty_struct *);
    void (*dcd_change)(struct tty_struct *, unsigned int);
    int (*receive_buf2)(struct tty_struct *, const unsigned char *, char *, int);
    struct module *owner;
    int refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct tty_ldisc_ops {
    char *name;
    int num;
    int flags;
    int (*open)(struct tty_struct *);
    void (*close)(struct tty_struct *);
    void (*flush_buffer)(struct tty_struct *);
    ssize_t (*read)(struct tty_struct *, struct file *, unsigned char *, size_t, void **, long unsigned int);
    ssize_t (*write)(struct tty_struct *, struct file *, const unsigned char *, size_t);
    int (*ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    __poll_t (*poll)(struct tty_struct *, struct file *, struct poll_table_struct *);
    int (*hangup)(struct tty_struct *);
    void (*receive_buf)(struct tty_struct *, const unsigned char *, char *, int);
    void (*write_wakeup)(struct tty_struct *);
    void (*dcd_change)(struct tty_struct *, unsigned int);
    int (*receive_buf2)(struct tty_struct *, const unsigned char *, char *, int);
    struct module *owner;
    int refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct tty_ldisc_ops {
    char *name;
    int num;
    int flags;
    int (*open)(struct tty_struct *);
    void (*close)(struct tty_struct *);
    void (*flush_buffer)(struct tty_struct *);
    ssize_t (*read)(struct tty_struct *, struct file *, unsigned char *, size_t, void **, long unsigned int);
    ssize_t (*write)(struct tty_struct *, struct file *, const unsigned char *, size_t);
    int (*ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    __poll_t (*poll)(struct tty_struct *, struct file *, struct poll_table_struct *);
    int (*hangup)(struct tty_struct *);
    void (*receive_buf)(struct tty_struct *, const unsigned char *, const char *, int);
    void (*write_wakeup)(struct tty_struct *);
    void (*dcd_change)(struct tty_struct *, unsigned int);
    int (*receive_buf2)(struct tty_struct *, const unsigned char *, const char *, int);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct tty_ldisc_ops {
    char *name;
    int num;
    int (*open)(struct tty_struct *);
    void (*close)(struct tty_struct *);
    void (*flush_buffer)(struct tty_struct *);
    ssize_t (*read)(struct tty_struct *, struct file *, unsigned char *, size_t, void **, long unsigned int);
    ssize_t (*write)(struct tty_struct *, struct file *, const unsigned char *, size_t);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    __poll_t (*poll)(struct tty_struct *, struct file *, struct poll_table_struct *);
    void (*hangup)(struct tty_struct *);
    void (*receive_buf)(struct tty_struct *, const unsigned char *, const char *, int);
    void (*write_wakeup)(struct tty_struct *);
    void (*dcd_change)(struct tty_struct *, unsigned int);
    int (*receive_buf2)(struct tty_struct *, const unsigned char *, const char *, int);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct tty_ldisc_ops {
    char *name;
    int num;
    int (*open)(struct tty_struct *);
    void (*close)(struct tty_struct *);
    void (*flush_buffer)(struct tty_struct *);
    ssize_t (*read)(struct tty_struct *, struct file *, unsigned char *, size_t, void **, long unsigned int);
    ssize_t (*write)(struct tty_struct *, struct file *, const unsigned char *, size_t);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, const struct ktermios *);
    __poll_t (*poll)(struct tty_struct *, struct file *, struct poll_table_struct *);
    void (*hangup)(struct tty_struct *);
    void (*receive_buf)(struct tty_struct *, const unsigned char *, const char *, int);
    void (*write_wakeup)(struct tty_struct *);
    void (*dcd_change)(struct tty_struct *, unsigned int);
    int (*receive_buf2)(struct tty_struct *, const unsigned char *, const char *, int);
    void (*lookahead_buf)(struct tty_struct *, const unsigned char *, const unsigned char *, unsigned int);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct tty_ldisc_ops {
    char *name;
    int num;
    int (*open)(struct tty_struct *);
    void (*close)(struct tty_struct *);
    void (*flush_buffer)(struct tty_struct *);
    ssize_t (*read)(struct tty_struct *, struct file *, unsigned char *, size_t, void **, long unsigned int);
    ssize_t (*write)(struct tty_struct *, struct file *, const unsigned char *, size_t);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, const struct ktermios *);
    __poll_t (*poll)(struct tty_struct *, struct file *, struct poll_table_struct *);
    void (*hangup)(struct tty_struct *);
    void (*receive_buf)(struct tty_struct *, const unsigned char *, const char *, int);
    void (*write_wakeup)(struct tty_struct *);
    void (*dcd_change)(struct tty_struct *, bool);
    int (*receive_buf2)(struct tty_struct *, const unsigned char *, const char *, int);
    void (*lookahead_buf)(struct tty_struct *, const unsigned char *, const unsigned char *, unsigned int);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct tty_ldisc_ops {
    char *name;
    int num;
    int (*open)(struct tty_struct *);
    void (*close)(struct tty_struct *);
    void (*flush_buffer)(struct tty_struct *);
    ssize_t (*read)(struct tty_struct *, struct file *, u8 *, size_t, void **, long unsigned int);
    ssize_t (*write)(struct tty_struct *, struct file *, const u8 *, size_t);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, const struct ktermios *);
    __poll_t (*poll)(struct tty_struct *, struct file *, struct poll_table_struct *);
    void (*hangup)(struct tty_struct *);
    void (*receive_buf)(struct tty_struct *, const u8 *, const u8 *, size_t);
    void (*write_wakeup)(struct tty_struct *);
    void (*dcd_change)(struct tty_struct *, bool);
    size_t (*receive_buf2)(struct tty_struct *, const u8 *, const u8 *, size_t);
    void (*lookahead_buf)(struct tty_struct *, const u8 *, const u8 *, size_t);
    struct module *owner;
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
struct tty_ldisc_ops {
    int magic;
    char *name;
    int num;
    int flags;
    int (*open)(struct tty_struct *);
    void (*close)(struct tty_struct *);
    void (*flush_buffer)(struct tty_struct *);
    ssize_t (*read)(struct tty_struct *, struct file *, unsigned char *, size_t);
    ssize_t (*write)(struct tty_struct *, struct file *, const unsigned char *, size_t);
    int (*ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    __poll_t (*poll)(struct tty_struct *, struct file *, struct poll_table_struct *);
    int (*hangup)(struct tty_struct *);
    void (*receive_buf)(struct tty_struct *, const unsigned char *, char *, int);
    void (*write_wakeup)(struct tty_struct *);
    void (*dcd_change)(struct tty_struct *, unsigned int);
    int (*receive_buf2)(struct tty_struct *, const unsigned char *, char *, int);
    struct module *owner;
    int refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct tty_ldisc_ops {
    int magic;
    char *name;
    int num;
    int flags;
    int (*open)(struct tty_struct *);
    void (*close)(struct tty_struct *);
    void (*flush_buffer)(struct tty_struct *);
    ssize_t (*read)(struct tty_struct *, struct file *, unsigned char *, size_t);
    ssize_t (*write)(struct tty_struct *, struct file *, const unsigned char *, size_t);
    int (*ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    __poll_t (*poll)(struct tty_struct *, struct file *, struct poll_table_struct *);
    int (*hangup)(struct tty_struct *);
    void (*receive_buf)(struct tty_struct *, const unsigned char *, char *, int);
    void (*write_wakeup)(struct tty_struct *);
    void (*dcd_change)(struct tty_struct *, unsigned int);
    int (*receive_buf2)(struct tty_struct *, const unsigned char *, char *, int);
    struct module *owner;
    int refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct tty_ldisc_ops {
    int magic;
    char *name;
    int num;
    int flags;
    int (*open)(struct tty_struct *);
    void (*close)(struct tty_struct *);
    void (*flush_buffer)(struct tty_struct *);
    ssize_t (*read)(struct tty_struct *, struct file *, unsigned char *, size_t);
    ssize_t (*write)(struct tty_struct *, struct file *, const unsigned char *, size_t);
    int (*ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    __poll_t (*poll)(struct tty_struct *, struct file *, struct poll_table_struct *);
    int (*hangup)(struct tty_struct *);
    void (*receive_buf)(struct tty_struct *, const unsigned char *, char *, int);
    void (*write_wakeup)(struct tty_struct *);
    void (*dcd_change)(struct tty_struct *, unsigned int);
    int (*receive_buf2)(struct tty_struct *, const unsigned char *, char *, int);
    struct module *owner;
    int refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct tty_ldisc_ops {
    int magic;
    char *name;
    int num;
    int flags;
    int (*open)(struct tty_struct *);
    void (*close)(struct tty_struct *);
    void (*flush_buffer)(struct tty_struct *);
    ssize_t (*read)(struct tty_struct *, struct file *, unsigned char *, size_t);
    ssize_t (*write)(struct tty_struct *, struct file *, const unsigned char *, size_t);
    int (*ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    __poll_t (*poll)(struct tty_struct *, struct file *, struct poll_table_struct *);
    int (*hangup)(struct tty_struct *);
    void (*receive_buf)(struct tty_struct *, const unsigned char *, char *, int);
    void (*write_wakeup)(struct tty_struct *);
    void (*dcd_change)(struct tty_struct *, unsigned int);
    int (*receive_buf2)(struct tty_struct *, const unsigned char *, char *, int);
    struct module *owner;
    int refcount;
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
struct tty_ldisc_ops {
    int magic;
    char *name;
    int num;
    int flags;
    int (*open)(struct tty_struct *);
    void (*close)(struct tty_struct *);
    void (*flush_buffer)(struct tty_struct *);
    ssize_t (*read)(struct tty_struct *, struct file *, unsigned char *, size_t);
    ssize_t (*write)(struct tty_struct *, struct file *, const unsigned char *, size_t);
    int (*ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    __poll_t (*poll)(struct tty_struct *, struct file *, struct poll_table_struct *);
    int (*hangup)(struct tty_struct *);
    void (*receive_buf)(struct tty_struct *, const unsigned char *, char *, int);
    void (*write_wakeup)(struct tty_struct *);
    void (*dcd_change)(struct tty_struct *, unsigned int);
    int (*receive_buf2)(struct tty_struct *, const unsigned char *, char *, int);
    struct module *owner;
    int refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct tty_ldisc_ops {
    int magic;
    char *name;
    int num;
    int flags;
    int (*open)(struct tty_struct *);
    void (*close)(struct tty_struct *);
    void (*flush_buffer)(struct tty_struct *);
    ssize_t (*read)(struct tty_struct *, struct file *, unsigned char *, size_t);
    ssize_t (*write)(struct tty_struct *, struct file *, const unsigned char *, size_t);
    int (*ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    __poll_t (*poll)(struct tty_struct *, struct file *, struct poll_table_struct *);
    int (*hangup)(struct tty_struct *);
    void (*receive_buf)(struct tty_struct *, const unsigned char *, char *, int);
    void (*write_wakeup)(struct tty_struct *);
    void (*dcd_change)(struct tty_struct *, unsigned int);
    int (*receive_buf2)(struct tty_struct *, const unsigned char *, char *, int);
    struct module *owner;
    int refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct tty_ldisc_ops {
    int magic;
    char *name;
    int num;
    int flags;
    int (*open)(struct tty_struct *);
    void (*close)(struct tty_struct *);
    void (*flush_buffer)(struct tty_struct *);
    ssize_t (*read)(struct tty_struct *, struct file *, unsigned char *, size_t);
    ssize_t (*write)(struct tty_struct *, struct file *, const unsigned char *, size_t);
    int (*ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    __poll_t (*poll)(struct tty_struct *, struct file *, struct poll_table_struct *);
    int (*hangup)(struct tty_struct *);
    void (*receive_buf)(struct tty_struct *, const unsigned char *, char *, int);
    void (*write_wakeup)(struct tty_struct *);
    void (*dcd_change)(struct tty_struct *, unsigned int);
    int (*receive_buf2)(struct tty_struct *, const unsigned char *, char *, int);
    struct module *owner;
    int refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct tty_ldisc_ops {
    int magic;
    char *name;
    int num;
    int flags;
    int (*open)(struct tty_struct *);
    void (*close)(struct tty_struct *);
    void (*flush_buffer)(struct tty_struct *);
    ssize_t (*read)(struct tty_struct *, struct file *, unsigned char *, size_t);
    ssize_t (*write)(struct tty_struct *, struct file *, const unsigned char *, size_t);
    int (*ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    __poll_t (*poll)(struct tty_struct *, struct file *, struct poll_table_struct *);
    int (*hangup)(struct tty_struct *);
    void (*receive_buf)(struct tty_struct *, const unsigned char *, char *, int);
    void (*write_wakeup)(struct tty_struct *);
    void (*dcd_change)(struct tty_struct *, unsigned int);
    int (*receive_buf2)(struct tty_struct *, const unsigned char *, char *, int);
    struct module *owner;
    int refcount;
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
<code>ssize_t (*chars_in_buffer)(struct tty_struct *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*fasync)(struct tty_struct *, int)</code>
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
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>unsigned int (*poll)(struct tty_struct *, struct file *, struct poll_table_struct *)</code> ➡️ <code>__poll_t (*poll)(struct tty_struct *, struct file *, struct poll_table_struct *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long int (*compat_ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int)</code> ➡️ <code>int (*compat_ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int)</code>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>ssize_t (*read)(struct tty_struct *, struct file *, unsigned char *, size_t)</code> ➡️ <code>ssize_t (*read)(struct tty_struct *, struct file *, unsigned char *, size_t, void **, long unsigned int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int magic</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int refcount</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*receive_buf)(struct tty_struct *, const unsigned char *, char *, int)</code> ➡️ <code>void (*receive_buf)(struct tty_struct *, const unsigned char *, const char *, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*receive_buf2)(struct tty_struct *, const unsigned char *, char *, int)</code> ➡️ <code>int (*receive_buf2)(struct tty_struct *, const unsigned char *, const char *, int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int flags</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int)</code> ➡️ <code>int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*compat_ioctl)(struct tty_struct *, struct file *, unsigned int, long unsigned int)</code> ➡️ <code>int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*hangup)(struct tty_struct *)</code> ➡️ <code>void (*hangup)(struct tty_struct *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*lookahead_buf)(struct tty_struct *, const unsigned char *, const unsigned char *, unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*set_termios)(struct tty_struct *, struct ktermios *)</code> ➡️ <code>void (*set_termios)(struct tty_struct *, const struct ktermios *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>void (*dcd_change)(struct tty_struct *, unsigned int)</code> ➡️ <code>void (*dcd_change)(struct tty_struct *, bool)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>ssize_t (*read)(struct tty_struct *, struct file *, unsigned char *, size_t, void **, long unsigned int)</code> ➡️ <code>ssize_t (*read)(struct tty_struct *, struct file *, u8 *, size_t, void **, long unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>ssize_t (*write)(struct tty_struct *, struct file *, const unsigned char *, size_t)</code> ➡️ <code>ssize_t (*write)(struct tty_struct *, struct file *, const u8 *, size_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*receive_buf)(struct tty_struct *, const unsigned char *, const char *, int)</code> ➡️ <code>void (*receive_buf)(struct tty_struct *, const u8 *, const u8 *, size_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*receive_buf2)(struct tty_struct *, const unsigned char *, const char *, int)</code> ➡️ <code>size_t (*receive_buf2)(struct tty_struct *, const u8 *, const u8 *, size_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*lookahead_buf)(struct tty_struct *, const unsigned char *, const unsigned char *, unsigned int)</code> ➡️ <code>void (*lookahead_buf)(struct tty_struct *, const u8 *, const u8 *, size_t)</code>
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
