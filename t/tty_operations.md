# Struct: <code>tty_operations</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct tty_operations {
    struct tty_struct * (*lookup)(struct tty_driver *, struct inode *, int);
    int (*install)(struct tty_driver *, struct tty_struct *);
    void (*remove)(struct tty_driver *, struct tty_struct *);
    int (*open)(struct tty_struct *, struct file *);
    void (*close)(struct tty_struct *, struct file *);
    void (*shutdown)(struct tty_struct *);
    void (*cleanup)(struct tty_struct *);
    int (*write)(struct tty_struct *, const unsigned char *, int);
    int (*put_char)(struct tty_struct *, unsigned char);
    void (*flush_chars)(struct tty_struct *);
    int (*write_room)(struct tty_struct *);
    int (*chars_in_buffer)(struct tty_struct *);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    void (*throttle)(struct tty_struct *);
    void (*unthrottle)(struct tty_struct *);
    void (*stop)(struct tty_struct *);
    void (*start)(struct tty_struct *);
    void (*hangup)(struct tty_struct *);
    int (*break_ctl)(struct tty_struct *, int);
    void (*flush_buffer)(struct tty_struct *);
    void (*set_ldisc)(struct tty_struct *);
    void (*wait_until_sent)(struct tty_struct *, int);
    void (*send_xchar)(struct tty_struct *, char);
    int (*tiocmget)(struct tty_struct *);
    int (*tiocmset)(struct tty_struct *, unsigned int, unsigned int);
    int (*resize)(struct tty_struct *, struct winsize *);
    int (*set_termiox)(struct tty_struct *, struct termiox *);
    int (*get_icount)(struct tty_struct *, struct serial_icounter_struct *);
    int (*poll_init)(struct tty_driver *, int, char *);
    int (*poll_get_char)(struct tty_driver *, int);
    void (*poll_put_char)(struct tty_driver *, int, char);
    const struct file_operations *proc_fops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct tty_operations {
    struct tty_struct * (*lookup)(struct tty_driver *, struct file *, int);
    int (*install)(struct tty_driver *, struct tty_struct *);
    void (*remove)(struct tty_driver *, struct tty_struct *);
    int (*open)(struct tty_struct *, struct file *);
    void (*close)(struct tty_struct *, struct file *);
    void (*shutdown)(struct tty_struct *);
    void (*cleanup)(struct tty_struct *);
    int (*write)(struct tty_struct *, const unsigned char *, int);
    int (*put_char)(struct tty_struct *, unsigned char);
    void (*flush_chars)(struct tty_struct *);
    int (*write_room)(struct tty_struct *);
    int (*chars_in_buffer)(struct tty_struct *);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    void (*throttle)(struct tty_struct *);
    void (*unthrottle)(struct tty_struct *);
    void (*stop)(struct tty_struct *);
    void (*start)(struct tty_struct *);
    void (*hangup)(struct tty_struct *);
    int (*break_ctl)(struct tty_struct *, int);
    void (*flush_buffer)(struct tty_struct *);
    void (*set_ldisc)(struct tty_struct *);
    void (*wait_until_sent)(struct tty_struct *, int);
    void (*send_xchar)(struct tty_struct *, char);
    int (*tiocmget)(struct tty_struct *);
    int (*tiocmset)(struct tty_struct *, unsigned int, unsigned int);
    int (*resize)(struct tty_struct *, struct winsize *);
    int (*set_termiox)(struct tty_struct *, struct termiox *);
    int (*get_icount)(struct tty_struct *, struct serial_icounter_struct *);
    int (*poll_init)(struct tty_driver *, int, char *);
    int (*poll_get_char)(struct tty_driver *, int);
    void (*poll_put_char)(struct tty_driver *, int, char);
    const struct file_operations *proc_fops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct tty_operations {
    struct tty_struct * (*lookup)(struct tty_driver *, struct file *, int);
    int (*install)(struct tty_driver *, struct tty_struct *);
    void (*remove)(struct tty_driver *, struct tty_struct *);
    int (*open)(struct tty_struct *, struct file *);
    void (*close)(struct tty_struct *, struct file *);
    void (*shutdown)(struct tty_struct *);
    void (*cleanup)(struct tty_struct *);
    int (*write)(struct tty_struct *, const unsigned char *, int);
    int (*put_char)(struct tty_struct *, unsigned char);
    void (*flush_chars)(struct tty_struct *);
    int (*write_room)(struct tty_struct *);
    int (*chars_in_buffer)(struct tty_struct *);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    void (*throttle)(struct tty_struct *);
    void (*unthrottle)(struct tty_struct *);
    void (*stop)(struct tty_struct *);
    void (*start)(struct tty_struct *);
    void (*hangup)(struct tty_struct *);
    int (*break_ctl)(struct tty_struct *, int);
    void (*flush_buffer)(struct tty_struct *);
    void (*set_ldisc)(struct tty_struct *);
    void (*wait_until_sent)(struct tty_struct *, int);
    void (*send_xchar)(struct tty_struct *, char);
    int (*tiocmget)(struct tty_struct *);
    int (*tiocmset)(struct tty_struct *, unsigned int, unsigned int);
    int (*resize)(struct tty_struct *, struct winsize *);
    int (*set_termiox)(struct tty_struct *, struct termiox *);
    int (*get_icount)(struct tty_struct *, struct serial_icounter_struct *);
    int (*poll_init)(struct tty_driver *, int, char *);
    int (*poll_get_char)(struct tty_driver *, int);
    void (*poll_put_char)(struct tty_driver *, int, char);
    const struct file_operations *proc_fops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct tty_operations {
    struct tty_struct * (*lookup)(struct tty_driver *, struct file *, int);
    int (*install)(struct tty_driver *, struct tty_struct *);
    void (*remove)(struct tty_driver *, struct tty_struct *);
    int (*open)(struct tty_struct *, struct file *);
    void (*close)(struct tty_struct *, struct file *);
    void (*shutdown)(struct tty_struct *);
    void (*cleanup)(struct tty_struct *);
    int (*write)(struct tty_struct *, const unsigned char *, int);
    int (*put_char)(struct tty_struct *, unsigned char);
    void (*flush_chars)(struct tty_struct *);
    int (*write_room)(struct tty_struct *);
    int (*chars_in_buffer)(struct tty_struct *);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    void (*throttle)(struct tty_struct *);
    void (*unthrottle)(struct tty_struct *);
    void (*stop)(struct tty_struct *);
    void (*start)(struct tty_struct *);
    void (*hangup)(struct tty_struct *);
    int (*break_ctl)(struct tty_struct *, int);
    void (*flush_buffer)(struct tty_struct *);
    void (*set_ldisc)(struct tty_struct *);
    void (*wait_until_sent)(struct tty_struct *, int);
    void (*send_xchar)(struct tty_struct *, char);
    int (*tiocmget)(struct tty_struct *);
    int (*tiocmset)(struct tty_struct *, unsigned int, unsigned int);
    int (*resize)(struct tty_struct *, struct winsize *);
    int (*set_termiox)(struct tty_struct *, struct termiox *);
    int (*get_icount)(struct tty_struct *, struct serial_icounter_struct *);
    int (*poll_init)(struct tty_driver *, int, char *);
    int (*poll_get_char)(struct tty_driver *, int);
    void (*poll_put_char)(struct tty_driver *, int, char);
    const struct file_operations *proc_fops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct tty_operations {
    struct tty_struct * (*lookup)(struct tty_driver *, struct file *, int);
    int (*install)(struct tty_driver *, struct tty_struct *);
    void (*remove)(struct tty_driver *, struct tty_struct *);
    int (*open)(struct tty_struct *, struct file *);
    void (*close)(struct tty_struct *, struct file *);
    void (*shutdown)(struct tty_struct *);
    void (*cleanup)(struct tty_struct *);
    int (*write)(struct tty_struct *, const unsigned char *, int);
    int (*put_char)(struct tty_struct *, unsigned char);
    void (*flush_chars)(struct tty_struct *);
    int (*write_room)(struct tty_struct *);
    int (*chars_in_buffer)(struct tty_struct *);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    void (*throttle)(struct tty_struct *);
    void (*unthrottle)(struct tty_struct *);
    void (*stop)(struct tty_struct *);
    void (*start)(struct tty_struct *);
    void (*hangup)(struct tty_struct *);
    int (*break_ctl)(struct tty_struct *, int);
    void (*flush_buffer)(struct tty_struct *);
    void (*set_ldisc)(struct tty_struct *);
    void (*wait_until_sent)(struct tty_struct *, int);
    void (*send_xchar)(struct tty_struct *, char);
    int (*tiocmget)(struct tty_struct *);
    int (*tiocmset)(struct tty_struct *, unsigned int, unsigned int);
    int (*resize)(struct tty_struct *, struct winsize *);
    int (*set_termiox)(struct tty_struct *, struct termiox *);
    int (*get_icount)(struct tty_struct *, struct serial_icounter_struct *);
    void (*show_fdinfo)(struct tty_struct *, struct seq_file *);
    int (*poll_init)(struct tty_driver *, int, char *);
    int (*poll_get_char)(struct tty_driver *, int);
    void (*poll_put_char)(struct tty_driver *, int, char);
    const struct file_operations *proc_fops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct tty_operations {
    struct tty_struct * (*lookup)(struct tty_driver *, struct file *, int);
    int (*install)(struct tty_driver *, struct tty_struct *);
    void (*remove)(struct tty_driver *, struct tty_struct *);
    int (*open)(struct tty_struct *, struct file *);
    void (*close)(struct tty_struct *, struct file *);
    void (*shutdown)(struct tty_struct *);
    void (*cleanup)(struct tty_struct *);
    int (*write)(struct tty_struct *, const unsigned char *, int);
    int (*put_char)(struct tty_struct *, unsigned char);
    void (*flush_chars)(struct tty_struct *);
    int (*write_room)(struct tty_struct *);
    int (*chars_in_buffer)(struct tty_struct *);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    void (*throttle)(struct tty_struct *);
    void (*unthrottle)(struct tty_struct *);
    void (*stop)(struct tty_struct *);
    void (*start)(struct tty_struct *);
    void (*hangup)(struct tty_struct *);
    int (*break_ctl)(struct tty_struct *, int);
    void (*flush_buffer)(struct tty_struct *);
    void (*set_ldisc)(struct tty_struct *);
    void (*wait_until_sent)(struct tty_struct *, int);
    void (*send_xchar)(struct tty_struct *, char);
    int (*tiocmget)(struct tty_struct *);
    int (*tiocmset)(struct tty_struct *, unsigned int, unsigned int);
    int (*resize)(struct tty_struct *, struct winsize *);
    int (*set_termiox)(struct tty_struct *, struct termiox *);
    int (*get_icount)(struct tty_struct *, struct serial_icounter_struct *);
    void (*show_fdinfo)(struct tty_struct *, struct seq_file *);
    int (*poll_init)(struct tty_driver *, int, char *);
    int (*poll_get_char)(struct tty_driver *, int);
    void (*poll_put_char)(struct tty_driver *, int, char);
    int (*proc_show)(struct seq_file *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct tty_operations {
    struct tty_struct * (*lookup)(struct tty_driver *, struct file *, int);
    int (*install)(struct tty_driver *, struct tty_struct *);
    void (*remove)(struct tty_driver *, struct tty_struct *);
    int (*open)(struct tty_struct *, struct file *);
    void (*close)(struct tty_struct *, struct file *);
    void (*shutdown)(struct tty_struct *);
    void (*cleanup)(struct tty_struct *);
    int (*write)(struct tty_struct *, const unsigned char *, int);
    int (*put_char)(struct tty_struct *, unsigned char);
    void (*flush_chars)(struct tty_struct *);
    int (*write_room)(struct tty_struct *);
    int (*chars_in_buffer)(struct tty_struct *);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    void (*throttle)(struct tty_struct *);
    void (*unthrottle)(struct tty_struct *);
    void (*stop)(struct tty_struct *);
    void (*start)(struct tty_struct *);
    void (*hangup)(struct tty_struct *);
    int (*break_ctl)(struct tty_struct *, int);
    void (*flush_buffer)(struct tty_struct *);
    void (*set_ldisc)(struct tty_struct *);
    void (*wait_until_sent)(struct tty_struct *, int);
    void (*send_xchar)(struct tty_struct *, char);
    int (*tiocmget)(struct tty_struct *);
    int (*tiocmset)(struct tty_struct *, unsigned int, unsigned int);
    int (*resize)(struct tty_struct *, struct winsize *);
    int (*set_termiox)(struct tty_struct *, struct termiox *);
    int (*get_icount)(struct tty_struct *, struct serial_icounter_struct *);
    int (*get_serial)(struct tty_struct *, struct serial_struct *);
    int (*set_serial)(struct tty_struct *, struct serial_struct *);
    void (*show_fdinfo)(struct tty_struct *, struct seq_file *);
    int (*poll_init)(struct tty_driver *, int, char *);
    int (*poll_get_char)(struct tty_driver *, int);
    void (*poll_put_char)(struct tty_driver *, int, char);
    int (*proc_show)(struct seq_file *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct tty_operations {
    struct tty_struct * (*lookup)(struct tty_driver *, struct file *, int);
    int (*install)(struct tty_driver *, struct tty_struct *);
    void (*remove)(struct tty_driver *, struct tty_struct *);
    int (*open)(struct tty_struct *, struct file *);
    void (*close)(struct tty_struct *, struct file *);
    void (*shutdown)(struct tty_struct *);
    void (*cleanup)(struct tty_struct *);
    int (*write)(struct tty_struct *, const unsigned char *, int);
    int (*put_char)(struct tty_struct *, unsigned char);
    void (*flush_chars)(struct tty_struct *);
    int (*write_room)(struct tty_struct *);
    int (*chars_in_buffer)(struct tty_struct *);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    void (*throttle)(struct tty_struct *);
    void (*unthrottle)(struct tty_struct *);
    void (*stop)(struct tty_struct *);
    void (*start)(struct tty_struct *);
    void (*hangup)(struct tty_struct *);
    int (*break_ctl)(struct tty_struct *, int);
    void (*flush_buffer)(struct tty_struct *);
    void (*set_ldisc)(struct tty_struct *);
    void (*wait_until_sent)(struct tty_struct *, int);
    void (*send_xchar)(struct tty_struct *, char);
    int (*tiocmget)(struct tty_struct *);
    int (*tiocmset)(struct tty_struct *, unsigned int, unsigned int);
    int (*resize)(struct tty_struct *, struct winsize *);
    int (*set_termiox)(struct tty_struct *, struct termiox *);
    int (*get_icount)(struct tty_struct *, struct serial_icounter_struct *);
    int (*get_serial)(struct tty_struct *, struct serial_struct *);
    int (*set_serial)(struct tty_struct *, struct serial_struct *);
    void (*show_fdinfo)(struct tty_struct *, struct seq_file *);
    int (*poll_init)(struct tty_driver *, int, char *);
    int (*poll_get_char)(struct tty_driver *, int);
    void (*poll_put_char)(struct tty_driver *, int, char);
    int (*proc_show)(struct seq_file *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct tty_operations {
    struct tty_struct * (*lookup)(struct tty_driver *, struct file *, int);
    int (*install)(struct tty_driver *, struct tty_struct *);
    void (*remove)(struct tty_driver *, struct tty_struct *);
    int (*open)(struct tty_struct *, struct file *);
    void (*close)(struct tty_struct *, struct file *);
    void (*shutdown)(struct tty_struct *);
    void (*cleanup)(struct tty_struct *);
    int (*write)(struct tty_struct *, const unsigned char *, int);
    int (*put_char)(struct tty_struct *, unsigned char);
    void (*flush_chars)(struct tty_struct *);
    int (*write_room)(struct tty_struct *);
    int (*chars_in_buffer)(struct tty_struct *);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    void (*throttle)(struct tty_struct *);
    void (*unthrottle)(struct tty_struct *);
    void (*stop)(struct tty_struct *);
    void (*start)(struct tty_struct *);
    void (*hangup)(struct tty_struct *);
    int (*break_ctl)(struct tty_struct *, int);
    void (*flush_buffer)(struct tty_struct *);
    void (*set_ldisc)(struct tty_struct *);
    void (*wait_until_sent)(struct tty_struct *, int);
    void (*send_xchar)(struct tty_struct *, char);
    int (*tiocmget)(struct tty_struct *);
    int (*tiocmset)(struct tty_struct *, unsigned int, unsigned int);
    int (*resize)(struct tty_struct *, struct winsize *);
    int (*set_termiox)(struct tty_struct *, struct termiox *);
    int (*get_icount)(struct tty_struct *, struct serial_icounter_struct *);
    int (*get_serial)(struct tty_struct *, struct serial_struct *);
    int (*set_serial)(struct tty_struct *, struct serial_struct *);
    void (*show_fdinfo)(struct tty_struct *, struct seq_file *);
    int (*poll_init)(struct tty_driver *, int, char *);
    int (*poll_get_char)(struct tty_driver *, int);
    void (*poll_put_char)(struct tty_driver *, int, char);
    int (*proc_show)(struct seq_file *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct tty_operations {
    struct tty_struct * (*lookup)(struct tty_driver *, struct file *, int);
    int (*install)(struct tty_driver *, struct tty_struct *);
    void (*remove)(struct tty_driver *, struct tty_struct *);
    int (*open)(struct tty_struct *, struct file *);
    void (*close)(struct tty_struct *, struct file *);
    void (*shutdown)(struct tty_struct *);
    void (*cleanup)(struct tty_struct *);
    int (*write)(struct tty_struct *, const unsigned char *, int);
    int (*put_char)(struct tty_struct *, unsigned char);
    void (*flush_chars)(struct tty_struct *);
    int (*write_room)(struct tty_struct *);
    int (*chars_in_buffer)(struct tty_struct *);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    void (*throttle)(struct tty_struct *);
    void (*unthrottle)(struct tty_struct *);
    void (*stop)(struct tty_struct *);
    void (*start)(struct tty_struct *);
    void (*hangup)(struct tty_struct *);
    int (*break_ctl)(struct tty_struct *, int);
    void (*flush_buffer)(struct tty_struct *);
    void (*set_ldisc)(struct tty_struct *);
    void (*wait_until_sent)(struct tty_struct *, int);
    void (*send_xchar)(struct tty_struct *, char);
    int (*tiocmget)(struct tty_struct *);
    int (*tiocmset)(struct tty_struct *, unsigned int, unsigned int);
    int (*resize)(struct tty_struct *, struct winsize *);
    int (*set_termiox)(struct tty_struct *, struct termiox *);
    int (*get_icount)(struct tty_struct *, struct serial_icounter_struct *);
    int (*get_serial)(struct tty_struct *, struct serial_struct *);
    int (*set_serial)(struct tty_struct *, struct serial_struct *);
    void (*show_fdinfo)(struct tty_struct *, struct seq_file *);
    int (*poll_init)(struct tty_driver *, int, char *);
    int (*poll_get_char)(struct tty_driver *, int);
    void (*poll_put_char)(struct tty_driver *, int, char);
    int (*proc_show)(struct seq_file *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct tty_operations {
    struct tty_struct * (*lookup)(struct tty_driver *, struct file *, int);
    int (*install)(struct tty_driver *, struct tty_struct *);
    void (*remove)(struct tty_driver *, struct tty_struct *);
    int (*open)(struct tty_struct *, struct file *);
    void (*close)(struct tty_struct *, struct file *);
    void (*shutdown)(struct tty_struct *);
    void (*cleanup)(struct tty_struct *);
    int (*write)(struct tty_struct *, const unsigned char *, int);
    int (*put_char)(struct tty_struct *, unsigned char);
    void (*flush_chars)(struct tty_struct *);
    int (*write_room)(struct tty_struct *);
    int (*chars_in_buffer)(struct tty_struct *);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    void (*throttle)(struct tty_struct *);
    void (*unthrottle)(struct tty_struct *);
    void (*stop)(struct tty_struct *);
    void (*start)(struct tty_struct *);
    void (*hangup)(struct tty_struct *);
    int (*break_ctl)(struct tty_struct *, int);
    void (*flush_buffer)(struct tty_struct *);
    void (*set_ldisc)(struct tty_struct *);
    void (*wait_until_sent)(struct tty_struct *, int);
    void (*send_xchar)(struct tty_struct *, char);
    int (*tiocmget)(struct tty_struct *);
    int (*tiocmset)(struct tty_struct *, unsigned int, unsigned int);
    int (*resize)(struct tty_struct *, struct winsize *);
    int (*get_icount)(struct tty_struct *, struct serial_icounter_struct *);
    int (*get_serial)(struct tty_struct *, struct serial_struct *);
    int (*set_serial)(struct tty_struct *, struct serial_struct *);
    void (*show_fdinfo)(struct tty_struct *, struct seq_file *);
    int (*poll_init)(struct tty_driver *, int, char *);
    int (*poll_get_char)(struct tty_driver *, int);
    void (*poll_put_char)(struct tty_driver *, int, char);
    int (*proc_show)(struct seq_file *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct tty_operations {
    struct tty_struct * (*lookup)(struct tty_driver *, struct file *, int);
    int (*install)(struct tty_driver *, struct tty_struct *);
    void (*remove)(struct tty_driver *, struct tty_struct *);
    int (*open)(struct tty_struct *, struct file *);
    void (*close)(struct tty_struct *, struct file *);
    void (*shutdown)(struct tty_struct *);
    void (*cleanup)(struct tty_struct *);
    int (*write)(struct tty_struct *, const unsigned char *, int);
    int (*put_char)(struct tty_struct *, unsigned char);
    void (*flush_chars)(struct tty_struct *);
    int (*write_room)(struct tty_struct *);
    int (*chars_in_buffer)(struct tty_struct *);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    void (*throttle)(struct tty_struct *);
    void (*unthrottle)(struct tty_struct *);
    void (*stop)(struct tty_struct *);
    void (*start)(struct tty_struct *);
    void (*hangup)(struct tty_struct *);
    int (*break_ctl)(struct tty_struct *, int);
    void (*flush_buffer)(struct tty_struct *);
    void (*set_ldisc)(struct tty_struct *);
    void (*wait_until_sent)(struct tty_struct *, int);
    void (*send_xchar)(struct tty_struct *, char);
    int (*tiocmget)(struct tty_struct *);
    int (*tiocmset)(struct tty_struct *, unsigned int, unsigned int);
    int (*resize)(struct tty_struct *, struct winsize *);
    int (*get_icount)(struct tty_struct *, struct serial_icounter_struct *);
    int (*get_serial)(struct tty_struct *, struct serial_struct *);
    int (*set_serial)(struct tty_struct *, struct serial_struct *);
    void (*show_fdinfo)(struct tty_struct *, struct seq_file *);
    int (*poll_init)(struct tty_driver *, int, char *);
    int (*poll_get_char)(struct tty_driver *, int);
    void (*poll_put_char)(struct tty_driver *, int, char);
    int (*proc_show)(struct seq_file *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct tty_operations {
    struct tty_struct * (*lookup)(struct tty_driver *, struct file *, int);
    int (*install)(struct tty_driver *, struct tty_struct *);
    void (*remove)(struct tty_driver *, struct tty_struct *);
    int (*open)(struct tty_struct *, struct file *);
    void (*close)(struct tty_struct *, struct file *);
    void (*shutdown)(struct tty_struct *);
    void (*cleanup)(struct tty_struct *);
    int (*write)(struct tty_struct *, const unsigned char *, int);
    int (*put_char)(struct tty_struct *, unsigned char);
    void (*flush_chars)(struct tty_struct *);
    unsigned int (*write_room)(struct tty_struct *);
    unsigned int (*chars_in_buffer)(struct tty_struct *);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    void (*throttle)(struct tty_struct *);
    void (*unthrottle)(struct tty_struct *);
    void (*stop)(struct tty_struct *);
    void (*start)(struct tty_struct *);
    void (*hangup)(struct tty_struct *);
    int (*break_ctl)(struct tty_struct *, int);
    void (*flush_buffer)(struct tty_struct *);
    void (*set_ldisc)(struct tty_struct *);
    void (*wait_until_sent)(struct tty_struct *, int);
    void (*send_xchar)(struct tty_struct *, char);
    int (*tiocmget)(struct tty_struct *);
    int (*tiocmset)(struct tty_struct *, unsigned int, unsigned int);
    int (*resize)(struct tty_struct *, struct winsize *);
    int (*get_icount)(struct tty_struct *, struct serial_icounter_struct *);
    int (*get_serial)(struct tty_struct *, struct serial_struct *);
    int (*set_serial)(struct tty_struct *, struct serial_struct *);
    void (*show_fdinfo)(struct tty_struct *, struct seq_file *);
    int (*poll_init)(struct tty_driver *, int, char *);
    int (*poll_get_char)(struct tty_driver *, int);
    void (*poll_put_char)(struct tty_driver *, int, char);
    int (*proc_show)(struct seq_file *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct tty_operations {
    struct tty_struct * (*lookup)(struct tty_driver *, struct file *, int);
    int (*install)(struct tty_driver *, struct tty_struct *);
    void (*remove)(struct tty_driver *, struct tty_struct *);
    int (*open)(struct tty_struct *, struct file *);
    void (*close)(struct tty_struct *, struct file *);
    void (*shutdown)(struct tty_struct *);
    void (*cleanup)(struct tty_struct *);
    int (*write)(struct tty_struct *, const unsigned char *, int);
    int (*put_char)(struct tty_struct *, unsigned char);
    void (*flush_chars)(struct tty_struct *);
    unsigned int (*write_room)(struct tty_struct *);
    unsigned int (*chars_in_buffer)(struct tty_struct *);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    void (*throttle)(struct tty_struct *);
    void (*unthrottle)(struct tty_struct *);
    void (*stop)(struct tty_struct *);
    void (*start)(struct tty_struct *);
    void (*hangup)(struct tty_struct *);
    int (*break_ctl)(struct tty_struct *, int);
    void (*flush_buffer)(struct tty_struct *);
    void (*set_ldisc)(struct tty_struct *);
    void (*wait_until_sent)(struct tty_struct *, int);
    void (*send_xchar)(struct tty_struct *, char);
    int (*tiocmget)(struct tty_struct *);
    int (*tiocmset)(struct tty_struct *, unsigned int, unsigned int);
    int (*resize)(struct tty_struct *, struct winsize *);
    int (*get_icount)(struct tty_struct *, struct serial_icounter_struct *);
    int (*get_serial)(struct tty_struct *, struct serial_struct *);
    int (*set_serial)(struct tty_struct *, struct serial_struct *);
    void (*show_fdinfo)(struct tty_struct *, struct seq_file *);
    int (*poll_init)(struct tty_driver *, int, char *);
    int (*poll_get_char)(struct tty_driver *, int);
    void (*poll_put_char)(struct tty_driver *, int, char);
    int (*proc_show)(struct seq_file *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct tty_operations {
    struct tty_struct * (*lookup)(struct tty_driver *, struct file *, int);
    int (*install)(struct tty_driver *, struct tty_struct *);
    void (*remove)(struct tty_driver *, struct tty_struct *);
    int (*open)(struct tty_struct *, struct file *);
    void (*close)(struct tty_struct *, struct file *);
    void (*shutdown)(struct tty_struct *);
    void (*cleanup)(struct tty_struct *);
    int (*write)(struct tty_struct *, const unsigned char *, int);
    int (*put_char)(struct tty_struct *, unsigned char);
    void (*flush_chars)(struct tty_struct *);
    unsigned int (*write_room)(struct tty_struct *);
    unsigned int (*chars_in_buffer)(struct tty_struct *);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, const struct ktermios *);
    void (*throttle)(struct tty_struct *);
    void (*unthrottle)(struct tty_struct *);
    void (*stop)(struct tty_struct *);
    void (*start)(struct tty_struct *);
    void (*hangup)(struct tty_struct *);
    int (*break_ctl)(struct tty_struct *, int);
    void (*flush_buffer)(struct tty_struct *);
    void (*set_ldisc)(struct tty_struct *);
    void (*wait_until_sent)(struct tty_struct *, int);
    void (*send_xchar)(struct tty_struct *, char);
    int (*tiocmget)(struct tty_struct *);
    int (*tiocmset)(struct tty_struct *, unsigned int, unsigned int);
    int (*resize)(struct tty_struct *, struct winsize *);
    int (*get_icount)(struct tty_struct *, struct serial_icounter_struct *);
    int (*get_serial)(struct tty_struct *, struct serial_struct *);
    int (*set_serial)(struct tty_struct *, struct serial_struct *);
    void (*show_fdinfo)(struct tty_struct *, struct seq_file *);
    int (*poll_init)(struct tty_driver *, int, char *);
    int (*poll_get_char)(struct tty_driver *, int);
    void (*poll_put_char)(struct tty_driver *, int, char);
    int (*proc_show)(struct seq_file *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct tty_operations {
    struct tty_struct * (*lookup)(struct tty_driver *, struct file *, int);
    int (*install)(struct tty_driver *, struct tty_struct *);
    void (*remove)(struct tty_driver *, struct tty_struct *);
    int (*open)(struct tty_struct *, struct file *);
    void (*close)(struct tty_struct *, struct file *);
    void (*shutdown)(struct tty_struct *);
    void (*cleanup)(struct tty_struct *);
    int (*write)(struct tty_struct *, const unsigned char *, int);
    int (*put_char)(struct tty_struct *, unsigned char);
    void (*flush_chars)(struct tty_struct *);
    unsigned int (*write_room)(struct tty_struct *);
    unsigned int (*chars_in_buffer)(struct tty_struct *);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, const struct ktermios *);
    void (*throttle)(struct tty_struct *);
    void (*unthrottle)(struct tty_struct *);
    void (*stop)(struct tty_struct *);
    void (*start)(struct tty_struct *);
    void (*hangup)(struct tty_struct *);
    int (*break_ctl)(struct tty_struct *, int);
    void (*flush_buffer)(struct tty_struct *);
    void (*set_ldisc)(struct tty_struct *);
    void (*wait_until_sent)(struct tty_struct *, int);
    void (*send_xchar)(struct tty_struct *, char);
    int (*tiocmget)(struct tty_struct *);
    int (*tiocmset)(struct tty_struct *, unsigned int, unsigned int);
    int (*resize)(struct tty_struct *, struct winsize *);
    int (*get_icount)(struct tty_struct *, struct serial_icounter_struct *);
    int (*get_serial)(struct tty_struct *, struct serial_struct *);
    int (*set_serial)(struct tty_struct *, struct serial_struct *);
    void (*show_fdinfo)(struct tty_struct *, struct seq_file *);
    int (*poll_init)(struct tty_driver *, int, char *);
    int (*poll_get_char)(struct tty_driver *, int);
    void (*poll_put_char)(struct tty_driver *, int, char);
    int (*proc_show)(struct seq_file *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct tty_operations {
    struct tty_struct * (*lookup)(struct tty_driver *, struct file *, int);
    int (*install)(struct tty_driver *, struct tty_struct *);
    void (*remove)(struct tty_driver *, struct tty_struct *);
    int (*open)(struct tty_struct *, struct file *);
    void (*close)(struct tty_struct *, struct file *);
    void (*shutdown)(struct tty_struct *);
    void (*cleanup)(struct tty_struct *);
    ssize_t (*write)(struct tty_struct *, const u8 *, size_t);
    int (*put_char)(struct tty_struct *, u8);
    void (*flush_chars)(struct tty_struct *);
    unsigned int (*write_room)(struct tty_struct *);
    unsigned int (*chars_in_buffer)(struct tty_struct *);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, const struct ktermios *);
    void (*throttle)(struct tty_struct *);
    void (*unthrottle)(struct tty_struct *);
    void (*stop)(struct tty_struct *);
    void (*start)(struct tty_struct *);
    void (*hangup)(struct tty_struct *);
    int (*break_ctl)(struct tty_struct *, int);
    void (*flush_buffer)(struct tty_struct *);
    void (*set_ldisc)(struct tty_struct *);
    void (*wait_until_sent)(struct tty_struct *, int);
    void (*send_xchar)(struct tty_struct *, u8);
    int (*tiocmget)(struct tty_struct *);
    int (*tiocmset)(struct tty_struct *, unsigned int, unsigned int);
    int (*resize)(struct tty_struct *, struct winsize *);
    int (*get_icount)(struct tty_struct *, struct serial_icounter_struct *);
    int (*get_serial)(struct tty_struct *, struct serial_struct *);
    int (*set_serial)(struct tty_struct *, struct serial_struct *);
    void (*show_fdinfo)(struct tty_struct *, struct seq_file *);
    int (*poll_init)(struct tty_driver *, int, char *);
    int (*poll_get_char)(struct tty_driver *, int);
    void (*poll_put_char)(struct tty_driver *, int, char);
    int (*proc_show)(struct seq_file *, void *);
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
struct tty_operations {
    struct tty_struct * (*lookup)(struct tty_driver *, struct file *, int);
    int (*install)(struct tty_driver *, struct tty_struct *);
    void (*remove)(struct tty_driver *, struct tty_struct *);
    int (*open)(struct tty_struct *, struct file *);
    void (*close)(struct tty_struct *, struct file *);
    void (*shutdown)(struct tty_struct *);
    void (*cleanup)(struct tty_struct *);
    int (*write)(struct tty_struct *, const unsigned char *, int);
    int (*put_char)(struct tty_struct *, unsigned char);
    void (*flush_chars)(struct tty_struct *);
    int (*write_room)(struct tty_struct *);
    int (*chars_in_buffer)(struct tty_struct *);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    void (*throttle)(struct tty_struct *);
    void (*unthrottle)(struct tty_struct *);
    void (*stop)(struct tty_struct *);
    void (*start)(struct tty_struct *);
    void (*hangup)(struct tty_struct *);
    int (*break_ctl)(struct tty_struct *, int);
    void (*flush_buffer)(struct tty_struct *);
    void (*set_ldisc)(struct tty_struct *);
    void (*wait_until_sent)(struct tty_struct *, int);
    void (*send_xchar)(struct tty_struct *, char);
    int (*tiocmget)(struct tty_struct *);
    int (*tiocmset)(struct tty_struct *, unsigned int, unsigned int);
    int (*resize)(struct tty_struct *, struct winsize *);
    int (*set_termiox)(struct tty_struct *, struct termiox *);
    int (*get_icount)(struct tty_struct *, struct serial_icounter_struct *);
    int (*get_serial)(struct tty_struct *, struct serial_struct *);
    int (*set_serial)(struct tty_struct *, struct serial_struct *);
    void (*show_fdinfo)(struct tty_struct *, struct seq_file *);
    int (*poll_init)(struct tty_driver *, int, char *);
    int (*poll_get_char)(struct tty_driver *, int);
    void (*poll_put_char)(struct tty_driver *, int, char);
    int (*proc_show)(struct seq_file *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct tty_operations {
    struct tty_struct * (*lookup)(struct tty_driver *, struct file *, int);
    int (*install)(struct tty_driver *, struct tty_struct *);
    void (*remove)(struct tty_driver *, struct tty_struct *);
    int (*open)(struct tty_struct *, struct file *);
    void (*close)(struct tty_struct *, struct file *);
    void (*shutdown)(struct tty_struct *);
    void (*cleanup)(struct tty_struct *);
    int (*write)(struct tty_struct *, const unsigned char *, int);
    int (*put_char)(struct tty_struct *, unsigned char);
    void (*flush_chars)(struct tty_struct *);
    int (*write_room)(struct tty_struct *);
    int (*chars_in_buffer)(struct tty_struct *);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    void (*throttle)(struct tty_struct *);
    void (*unthrottle)(struct tty_struct *);
    void (*stop)(struct tty_struct *);
    void (*start)(struct tty_struct *);
    void (*hangup)(struct tty_struct *);
    int (*break_ctl)(struct tty_struct *, int);
    void (*flush_buffer)(struct tty_struct *);
    void (*set_ldisc)(struct tty_struct *);
    void (*wait_until_sent)(struct tty_struct *, int);
    void (*send_xchar)(struct tty_struct *, char);
    int (*tiocmget)(struct tty_struct *);
    int (*tiocmset)(struct tty_struct *, unsigned int, unsigned int);
    int (*resize)(struct tty_struct *, struct winsize *);
    int (*set_termiox)(struct tty_struct *, struct termiox *);
    int (*get_icount)(struct tty_struct *, struct serial_icounter_struct *);
    int (*get_serial)(struct tty_struct *, struct serial_struct *);
    int (*set_serial)(struct tty_struct *, struct serial_struct *);
    void (*show_fdinfo)(struct tty_struct *, struct seq_file *);
    int (*poll_init)(struct tty_driver *, int, char *);
    int (*poll_get_char)(struct tty_driver *, int);
    void (*poll_put_char)(struct tty_driver *, int, char);
    int (*proc_show)(struct seq_file *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct tty_operations {
    struct tty_struct * (*lookup)(struct tty_driver *, struct file *, int);
    int (*install)(struct tty_driver *, struct tty_struct *);
    void (*remove)(struct tty_driver *, struct tty_struct *);
    int (*open)(struct tty_struct *, struct file *);
    void (*close)(struct tty_struct *, struct file *);
    void (*shutdown)(struct tty_struct *);
    void (*cleanup)(struct tty_struct *);
    int (*write)(struct tty_struct *, const unsigned char *, int);
    int (*put_char)(struct tty_struct *, unsigned char);
    void (*flush_chars)(struct tty_struct *);
    int (*write_room)(struct tty_struct *);
    int (*chars_in_buffer)(struct tty_struct *);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    void (*throttle)(struct tty_struct *);
    void (*unthrottle)(struct tty_struct *);
    void (*stop)(struct tty_struct *);
    void (*start)(struct tty_struct *);
    void (*hangup)(struct tty_struct *);
    int (*break_ctl)(struct tty_struct *, int);
    void (*flush_buffer)(struct tty_struct *);
    void (*set_ldisc)(struct tty_struct *);
    void (*wait_until_sent)(struct tty_struct *, int);
    void (*send_xchar)(struct tty_struct *, char);
    int (*tiocmget)(struct tty_struct *);
    int (*tiocmset)(struct tty_struct *, unsigned int, unsigned int);
    int (*resize)(struct tty_struct *, struct winsize *);
    int (*set_termiox)(struct tty_struct *, struct termiox *);
    int (*get_icount)(struct tty_struct *, struct serial_icounter_struct *);
    int (*get_serial)(struct tty_struct *, struct serial_struct *);
    int (*set_serial)(struct tty_struct *, struct serial_struct *);
    void (*show_fdinfo)(struct tty_struct *, struct seq_file *);
    int (*poll_init)(struct tty_driver *, int, char *);
    int (*poll_get_char)(struct tty_driver *, int);
    void (*poll_put_char)(struct tty_driver *, int, char);
    int (*proc_show)(struct seq_file *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct tty_operations {
    struct tty_struct * (*lookup)(struct tty_driver *, struct file *, int);
    int (*install)(struct tty_driver *, struct tty_struct *);
    void (*remove)(struct tty_driver *, struct tty_struct *);
    int (*open)(struct tty_struct *, struct file *);
    void (*close)(struct tty_struct *, struct file *);
    void (*shutdown)(struct tty_struct *);
    void (*cleanup)(struct tty_struct *);
    int (*write)(struct tty_struct *, const unsigned char *, int);
    int (*put_char)(struct tty_struct *, unsigned char);
    void (*flush_chars)(struct tty_struct *);
    int (*write_room)(struct tty_struct *);
    int (*chars_in_buffer)(struct tty_struct *);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    void (*throttle)(struct tty_struct *);
    void (*unthrottle)(struct tty_struct *);
    void (*stop)(struct tty_struct *);
    void (*start)(struct tty_struct *);
    void (*hangup)(struct tty_struct *);
    int (*break_ctl)(struct tty_struct *, int);
    void (*flush_buffer)(struct tty_struct *);
    void (*set_ldisc)(struct tty_struct *);
    void (*wait_until_sent)(struct tty_struct *, int);
    void (*send_xchar)(struct tty_struct *, char);
    int (*tiocmget)(struct tty_struct *);
    int (*tiocmset)(struct tty_struct *, unsigned int, unsigned int);
    int (*resize)(struct tty_struct *, struct winsize *);
    int (*set_termiox)(struct tty_struct *, struct termiox *);
    int (*get_icount)(struct tty_struct *, struct serial_icounter_struct *);
    int (*get_serial)(struct tty_struct *, struct serial_struct *);
    int (*set_serial)(struct tty_struct *, struct serial_struct *);
    void (*show_fdinfo)(struct tty_struct *, struct seq_file *);
    int (*proc_show)(struct seq_file *, void *);
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
struct tty_operations {
    struct tty_struct * (*lookup)(struct tty_driver *, struct file *, int);
    int (*install)(struct tty_driver *, struct tty_struct *);
    void (*remove)(struct tty_driver *, struct tty_struct *);
    int (*open)(struct tty_struct *, struct file *);
    void (*close)(struct tty_struct *, struct file *);
    void (*shutdown)(struct tty_struct *);
    void (*cleanup)(struct tty_struct *);
    int (*write)(struct tty_struct *, const unsigned char *, int);
    int (*put_char)(struct tty_struct *, unsigned char);
    void (*flush_chars)(struct tty_struct *);
    int (*write_room)(struct tty_struct *);
    int (*chars_in_buffer)(struct tty_struct *);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    void (*throttle)(struct tty_struct *);
    void (*unthrottle)(struct tty_struct *);
    void (*stop)(struct tty_struct *);
    void (*start)(struct tty_struct *);
    void (*hangup)(struct tty_struct *);
    int (*break_ctl)(struct tty_struct *, int);
    void (*flush_buffer)(struct tty_struct *);
    void (*set_ldisc)(struct tty_struct *);
    void (*wait_until_sent)(struct tty_struct *, int);
    void (*send_xchar)(struct tty_struct *, char);
    int (*tiocmget)(struct tty_struct *);
    int (*tiocmset)(struct tty_struct *, unsigned int, unsigned int);
    int (*resize)(struct tty_struct *, struct winsize *);
    int (*set_termiox)(struct tty_struct *, struct termiox *);
    int (*get_icount)(struct tty_struct *, struct serial_icounter_struct *);
    int (*get_serial)(struct tty_struct *, struct serial_struct *);
    int (*set_serial)(struct tty_struct *, struct serial_struct *);
    void (*show_fdinfo)(struct tty_struct *, struct seq_file *);
    int (*poll_init)(struct tty_driver *, int, char *);
    int (*poll_get_char)(struct tty_driver *, int);
    void (*poll_put_char)(struct tty_driver *, int, char);
    int (*proc_show)(struct seq_file *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct tty_operations {
    struct tty_struct * (*lookup)(struct tty_driver *, struct file *, int);
    int (*install)(struct tty_driver *, struct tty_struct *);
    void (*remove)(struct tty_driver *, struct tty_struct *);
    int (*open)(struct tty_struct *, struct file *);
    void (*close)(struct tty_struct *, struct file *);
    void (*shutdown)(struct tty_struct *);
    void (*cleanup)(struct tty_struct *);
    int (*write)(struct tty_struct *, const unsigned char *, int);
    int (*put_char)(struct tty_struct *, unsigned char);
    void (*flush_chars)(struct tty_struct *);
    int (*write_room)(struct tty_struct *);
    int (*chars_in_buffer)(struct tty_struct *);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    void (*throttle)(struct tty_struct *);
    void (*unthrottle)(struct tty_struct *);
    void (*stop)(struct tty_struct *);
    void (*start)(struct tty_struct *);
    void (*hangup)(struct tty_struct *);
    int (*break_ctl)(struct tty_struct *, int);
    void (*flush_buffer)(struct tty_struct *);
    void (*set_ldisc)(struct tty_struct *);
    void (*wait_until_sent)(struct tty_struct *, int);
    void (*send_xchar)(struct tty_struct *, char);
    int (*tiocmget)(struct tty_struct *);
    int (*tiocmset)(struct tty_struct *, unsigned int, unsigned int);
    int (*resize)(struct tty_struct *, struct winsize *);
    int (*set_termiox)(struct tty_struct *, struct termiox *);
    int (*get_icount)(struct tty_struct *, struct serial_icounter_struct *);
    int (*get_serial)(struct tty_struct *, struct serial_struct *);
    int (*set_serial)(struct tty_struct *, struct serial_struct *);
    void (*show_fdinfo)(struct tty_struct *, struct seq_file *);
    int (*poll_init)(struct tty_driver *, int, char *);
    int (*poll_get_char)(struct tty_driver *, int);
    void (*poll_put_char)(struct tty_driver *, int, char);
    int (*proc_show)(struct seq_file *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct tty_operations {
    struct tty_struct * (*lookup)(struct tty_driver *, struct file *, int);
    int (*install)(struct tty_driver *, struct tty_struct *);
    void (*remove)(struct tty_driver *, struct tty_struct *);
    int (*open)(struct tty_struct *, struct file *);
    void (*close)(struct tty_struct *, struct file *);
    void (*shutdown)(struct tty_struct *);
    void (*cleanup)(struct tty_struct *);
    int (*write)(struct tty_struct *, const unsigned char *, int);
    int (*put_char)(struct tty_struct *, unsigned char);
    void (*flush_chars)(struct tty_struct *);
    int (*write_room)(struct tty_struct *);
    int (*chars_in_buffer)(struct tty_struct *);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    void (*throttle)(struct tty_struct *);
    void (*unthrottle)(struct tty_struct *);
    void (*stop)(struct tty_struct *);
    void (*start)(struct tty_struct *);
    void (*hangup)(struct tty_struct *);
    int (*break_ctl)(struct tty_struct *, int);
    void (*flush_buffer)(struct tty_struct *);
    void (*set_ldisc)(struct tty_struct *);
    void (*wait_until_sent)(struct tty_struct *, int);
    void (*send_xchar)(struct tty_struct *, char);
    int (*tiocmget)(struct tty_struct *);
    int (*tiocmset)(struct tty_struct *, unsigned int, unsigned int);
    int (*resize)(struct tty_struct *, struct winsize *);
    int (*set_termiox)(struct tty_struct *, struct termiox *);
    int (*get_icount)(struct tty_struct *, struct serial_icounter_struct *);
    int (*get_serial)(struct tty_struct *, struct serial_struct *);
    int (*set_serial)(struct tty_struct *, struct serial_struct *);
    void (*show_fdinfo)(struct tty_struct *, struct seq_file *);
    int (*poll_init)(struct tty_driver *, int, char *);
    int (*poll_get_char)(struct tty_driver *, int);
    void (*poll_put_char)(struct tty_driver *, int, char);
    int (*proc_show)(struct seq_file *, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct tty_operations {
    struct tty_struct * (*lookup)(struct tty_driver *, struct file *, int);
    int (*install)(struct tty_driver *, struct tty_struct *);
    void (*remove)(struct tty_driver *, struct tty_struct *);
    int (*open)(struct tty_struct *, struct file *);
    void (*close)(struct tty_struct *, struct file *);
    void (*shutdown)(struct tty_struct *);
    void (*cleanup)(struct tty_struct *);
    int (*write)(struct tty_struct *, const unsigned char *, int);
    int (*put_char)(struct tty_struct *, unsigned char);
    void (*flush_chars)(struct tty_struct *);
    int (*write_room)(struct tty_struct *);
    int (*chars_in_buffer)(struct tty_struct *);
    int (*ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    long int (*compat_ioctl)(struct tty_struct *, unsigned int, long unsigned int);
    void (*set_termios)(struct tty_struct *, struct ktermios *);
    void (*throttle)(struct tty_struct *);
    void (*unthrottle)(struct tty_struct *);
    void (*stop)(struct tty_struct *);
    void (*start)(struct tty_struct *);
    void (*hangup)(struct tty_struct *);
    int (*break_ctl)(struct tty_struct *, int);
    void (*flush_buffer)(struct tty_struct *);
    void (*set_ldisc)(struct tty_struct *);
    void (*wait_until_sent)(struct tty_struct *, int);
    void (*send_xchar)(struct tty_struct *, char);
    int (*tiocmget)(struct tty_struct *);
    int (*tiocmset)(struct tty_struct *, unsigned int, unsigned int);
    int (*resize)(struct tty_struct *, struct winsize *);
    int (*set_termiox)(struct tty_struct *, struct termiox *);
    int (*get_icount)(struct tty_struct *, struct serial_icounter_struct *);
    int (*get_serial)(struct tty_struct *, struct serial_struct *);
    int (*set_serial)(struct tty_struct *, struct serial_struct *);
    void (*show_fdinfo)(struct tty_struct *, struct seq_file *);
    int (*poll_init)(struct tty_driver *, int, char *);
    int (*poll_get_char)(struct tty_driver *, int);
    void (*poll_put_char)(struct tty_driver *, int, char);
    int (*proc_show)(struct seq_file *, void *);
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
<b>Field type changed. </b>
<code>struct tty_struct * (*lookup)(struct tty_driver *, struct inode *, int)</code> ➡️ <code>struct tty_struct * (*lookup)(struct tty_driver *, struct file *, int)</code>
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
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*show_fdinfo)(struct tty_struct *, struct seq_file *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*proc_show)(struct seq_file *, void *)</code>
</li>
<li>
<b>Field removed. </b>
<code>const struct file_operations *proc_fops</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*get_serial)(struct tty_struct *, struct serial_struct *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_serial)(struct tty_struct *, struct serial_struct *)</code>
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
<b>Field removed. </b>
<code>int (*set_termiox)(struct tty_struct *, struct termiox *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*write_room)(struct tty_struct *)</code> ➡️ <code>unsigned int (*write_room)(struct tty_struct *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*chars_in_buffer)(struct tty_struct *)</code> ➡️ <code>unsigned int (*chars_in_buffer)(struct tty_struct *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>void (*set_termios)(struct tty_struct *, struct ktermios *)</code> ➡️ <code>void (*set_termios)(struct tty_struct *, const struct ktermios *)</code>
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
<b>Field type changed. </b>
<code>int (*write)(struct tty_struct *, const unsigned char *, int)</code> ➡️ <code>ssize_t (*write)(struct tty_struct *, const u8 *, size_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*put_char)(struct tty_struct *, unsigned char)</code> ➡️ <code>int (*put_char)(struct tty_struct *, u8)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*send_xchar)(struct tty_struct *, char)</code> ➡️ <code>void (*send_xchar)(struct tty_struct *, u8)</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*poll_init)(struct tty_driver *, int, char *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*poll_get_char)(struct tty_driver *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*poll_put_char)(struct tty_driver *, int, char)</code>
</li>
</ul>
</details>
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
