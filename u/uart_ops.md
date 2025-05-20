# Struct: <code>uart_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct uart_ops {
    unsigned int (*tx_empty)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*stop_tx)(struct uart_port *);
    void (*start_tx)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    void (*send_xchar)(struct uart_port *, char);
    void (*stop_rx)(struct uart_port *);
    void (*enable_ms)(struct uart_port *);
    void (*break_ctl)(struct uart_port *, int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*flush_buffer)(struct uart_port *);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    const char * (*type)(struct uart_port *);
    void (*release_port)(struct uart_port *);
    int (*request_port)(struct uart_port *);
    void (*config_port)(struct uart_port *, int);
    int (*verify_port)(struct uart_port *, struct serial_struct *);
    int (*ioctl)(struct uart_port *, unsigned int, long unsigned int);
    int (*poll_init)(struct uart_port *);
    void (*poll_put_char)(struct uart_port *, unsigned char);
    int (*poll_get_char)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct uart_ops {
    unsigned int (*tx_empty)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*stop_tx)(struct uart_port *);
    void (*start_tx)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    void (*send_xchar)(struct uart_port *, char);
    void (*stop_rx)(struct uart_port *);
    void (*enable_ms)(struct uart_port *);
    void (*break_ctl)(struct uart_port *, int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*flush_buffer)(struct uart_port *);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    const char * (*type)(struct uart_port *);
    void (*release_port)(struct uart_port *);
    int (*request_port)(struct uart_port *);
    void (*config_port)(struct uart_port *, int);
    int (*verify_port)(struct uart_port *, struct serial_struct *);
    int (*ioctl)(struct uart_port *, unsigned int, long unsigned int);
    int (*poll_init)(struct uart_port *);
    void (*poll_put_char)(struct uart_port *, unsigned char);
    int (*poll_get_char)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct uart_ops {
    unsigned int (*tx_empty)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*stop_tx)(struct uart_port *);
    void (*start_tx)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    void (*send_xchar)(struct uart_port *, char);
    void (*stop_rx)(struct uart_port *);
    void (*enable_ms)(struct uart_port *);
    void (*break_ctl)(struct uart_port *, int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*flush_buffer)(struct uart_port *);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    const char * (*type)(struct uart_port *);
    void (*release_port)(struct uart_port *);
    int (*request_port)(struct uart_port *);
    void (*config_port)(struct uart_port *, int);
    int (*verify_port)(struct uart_port *, struct serial_struct *);
    int (*ioctl)(struct uart_port *, unsigned int, long unsigned int);
    int (*poll_init)(struct uart_port *);
    void (*poll_put_char)(struct uart_port *, unsigned char);
    int (*poll_get_char)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct uart_ops {
    unsigned int (*tx_empty)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*stop_tx)(struct uart_port *);
    void (*start_tx)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    void (*send_xchar)(struct uart_port *, char);
    void (*stop_rx)(struct uart_port *);
    void (*enable_ms)(struct uart_port *);
    void (*break_ctl)(struct uart_port *, int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*flush_buffer)(struct uart_port *);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    const char * (*type)(struct uart_port *);
    void (*release_port)(struct uart_port *);
    int (*request_port)(struct uart_port *);
    void (*config_port)(struct uart_port *, int);
    int (*verify_port)(struct uart_port *, struct serial_struct *);
    int (*ioctl)(struct uart_port *, unsigned int, long unsigned int);
    int (*poll_init)(struct uart_port *);
    void (*poll_put_char)(struct uart_port *, unsigned char);
    int (*poll_get_char)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct uart_ops {
    unsigned int (*tx_empty)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*stop_tx)(struct uart_port *);
    void (*start_tx)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    void (*send_xchar)(struct uart_port *, char);
    void (*stop_rx)(struct uart_port *);
    void (*enable_ms)(struct uart_port *);
    void (*break_ctl)(struct uart_port *, int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*flush_buffer)(struct uart_port *);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    const char * (*type)(struct uart_port *);
    void (*release_port)(struct uart_port *);
    int (*request_port)(struct uart_port *);
    void (*config_port)(struct uart_port *, int);
    int (*verify_port)(struct uart_port *, struct serial_struct *);
    int (*ioctl)(struct uart_port *, unsigned int, long unsigned int);
    int (*poll_init)(struct uart_port *);
    void (*poll_put_char)(struct uart_port *, unsigned char);
    int (*poll_get_char)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct uart_ops {
    unsigned int (*tx_empty)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*stop_tx)(struct uart_port *);
    void (*start_tx)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    void (*send_xchar)(struct uart_port *, char);
    void (*stop_rx)(struct uart_port *);
    void (*enable_ms)(struct uart_port *);
    void (*break_ctl)(struct uart_port *, int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*flush_buffer)(struct uart_port *);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    const char * (*type)(struct uart_port *);
    void (*release_port)(struct uart_port *);
    int (*request_port)(struct uart_port *);
    void (*config_port)(struct uart_port *, int);
    int (*verify_port)(struct uart_port *, struct serial_struct *);
    int (*ioctl)(struct uart_port *, unsigned int, long unsigned int);
    int (*poll_init)(struct uart_port *);
    void (*poll_put_char)(struct uart_port *, unsigned char);
    int (*poll_get_char)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct uart_ops {
    unsigned int (*tx_empty)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*stop_tx)(struct uart_port *);
    void (*start_tx)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    void (*send_xchar)(struct uart_port *, char);
    void (*stop_rx)(struct uart_port *);
    void (*enable_ms)(struct uart_port *);
    void (*break_ctl)(struct uart_port *, int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*flush_buffer)(struct uart_port *);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    const char * (*type)(struct uart_port *);
    void (*release_port)(struct uart_port *);
    int (*request_port)(struct uart_port *);
    void (*config_port)(struct uart_port *, int);
    int (*verify_port)(struct uart_port *, struct serial_struct *);
    int (*ioctl)(struct uart_port *, unsigned int, long unsigned int);
    int (*poll_init)(struct uart_port *);
    void (*poll_put_char)(struct uart_port *, unsigned char);
    int (*poll_get_char)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct uart_ops {
    unsigned int (*tx_empty)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*stop_tx)(struct uart_port *);
    void (*start_tx)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    void (*send_xchar)(struct uart_port *, char);
    void (*stop_rx)(struct uart_port *);
    void (*enable_ms)(struct uart_port *);
    void (*break_ctl)(struct uart_port *, int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*flush_buffer)(struct uart_port *);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    const char * (*type)(struct uart_port *);
    void (*release_port)(struct uart_port *);
    int (*request_port)(struct uart_port *);
    void (*config_port)(struct uart_port *, int);
    int (*verify_port)(struct uart_port *, struct serial_struct *);
    int (*ioctl)(struct uart_port *, unsigned int, long unsigned int);
    int (*poll_init)(struct uart_port *);
    void (*poll_put_char)(struct uart_port *, unsigned char);
    int (*poll_get_char)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct uart_ops {
    unsigned int (*tx_empty)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*stop_tx)(struct uart_port *);
    void (*start_tx)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    void (*send_xchar)(struct uart_port *, char);
    void (*stop_rx)(struct uart_port *);
    void (*enable_ms)(struct uart_port *);
    void (*break_ctl)(struct uart_port *, int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*flush_buffer)(struct uart_port *);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    const char * (*type)(struct uart_port *);
    void (*release_port)(struct uart_port *);
    int (*request_port)(struct uart_port *);
    void (*config_port)(struct uart_port *, int);
    int (*verify_port)(struct uart_port *, struct serial_struct *);
    int (*ioctl)(struct uart_port *, unsigned int, long unsigned int);
    int (*poll_init)(struct uart_port *);
    void (*poll_put_char)(struct uart_port *, unsigned char);
    int (*poll_get_char)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct uart_ops {
    unsigned int (*tx_empty)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*stop_tx)(struct uart_port *);
    void (*start_tx)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    void (*send_xchar)(struct uart_port *, char);
    void (*stop_rx)(struct uart_port *);
    void (*enable_ms)(struct uart_port *);
    void (*break_ctl)(struct uart_port *, int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*flush_buffer)(struct uart_port *);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    const char * (*type)(struct uart_port *);
    void (*release_port)(struct uart_port *);
    int (*request_port)(struct uart_port *);
    void (*config_port)(struct uart_port *, int);
    int (*verify_port)(struct uart_port *, struct serial_struct *);
    int (*ioctl)(struct uart_port *, unsigned int, long unsigned int);
    int (*poll_init)(struct uart_port *);
    void (*poll_put_char)(struct uart_port *, unsigned char);
    int (*poll_get_char)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct uart_ops {
    unsigned int (*tx_empty)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*stop_tx)(struct uart_port *);
    void (*start_tx)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    void (*send_xchar)(struct uart_port *, char);
    void (*stop_rx)(struct uart_port *);
    void (*enable_ms)(struct uart_port *);
    void (*break_ctl)(struct uart_port *, int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*flush_buffer)(struct uart_port *);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    const char * (*type)(struct uart_port *);
    void (*release_port)(struct uart_port *);
    int (*request_port)(struct uart_port *);
    void (*config_port)(struct uart_port *, int);
    int (*verify_port)(struct uart_port *, struct serial_struct *);
    int (*ioctl)(struct uart_port *, unsigned int, long unsigned int);
    int (*poll_init)(struct uart_port *);
    void (*poll_put_char)(struct uart_port *, unsigned char);
    int (*poll_get_char)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct uart_ops {
    unsigned int (*tx_empty)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*stop_tx)(struct uart_port *);
    void (*start_tx)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    void (*send_xchar)(struct uart_port *, char);
    void (*stop_rx)(struct uart_port *);
    void (*enable_ms)(struct uart_port *);
    void (*break_ctl)(struct uart_port *, int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*flush_buffer)(struct uart_port *);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    const char * (*type)(struct uart_port *);
    void (*release_port)(struct uart_port *);
    int (*request_port)(struct uart_port *);
    void (*config_port)(struct uart_port *, int);
    int (*verify_port)(struct uart_port *, struct serial_struct *);
    int (*ioctl)(struct uart_port *, unsigned int, long unsigned int);
    int (*poll_init)(struct uart_port *);
    void (*poll_put_char)(struct uart_port *, unsigned char);
    int (*poll_get_char)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct uart_ops {
    unsigned int (*tx_empty)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*stop_tx)(struct uart_port *);
    void (*start_tx)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    void (*send_xchar)(struct uart_port *, char);
    void (*stop_rx)(struct uart_port *);
    void (*enable_ms)(struct uart_port *);
    void (*break_ctl)(struct uart_port *, int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*flush_buffer)(struct uart_port *);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    const char * (*type)(struct uart_port *);
    void (*release_port)(struct uart_port *);
    int (*request_port)(struct uart_port *);
    void (*config_port)(struct uart_port *, int);
    int (*verify_port)(struct uart_port *, struct serial_struct *);
    int (*ioctl)(struct uart_port *, unsigned int, long unsigned int);
    int (*poll_init)(struct uart_port *);
    void (*poll_put_char)(struct uart_port *, unsigned char);
    int (*poll_get_char)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct uart_ops {
    unsigned int (*tx_empty)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*stop_tx)(struct uart_port *);
    void (*start_tx)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    void (*send_xchar)(struct uart_port *, char);
    void (*stop_rx)(struct uart_port *);
    void (*start_rx)(struct uart_port *);
    void (*enable_ms)(struct uart_port *);
    void (*break_ctl)(struct uart_port *, int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*flush_buffer)(struct uart_port *);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    const char * (*type)(struct uart_port *);
    void (*release_port)(struct uart_port *);
    int (*request_port)(struct uart_port *);
    void (*config_port)(struct uart_port *, int);
    int (*verify_port)(struct uart_port *, struct serial_struct *);
    int (*ioctl)(struct uart_port *, unsigned int, long unsigned int);
    int (*poll_init)(struct uart_port *);
    void (*poll_put_char)(struct uart_port *, unsigned char);
    int (*poll_get_char)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct uart_ops {
    unsigned int (*tx_empty)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*stop_tx)(struct uart_port *);
    void (*start_tx)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    void (*send_xchar)(struct uart_port *, char);
    void (*stop_rx)(struct uart_port *);
    void (*start_rx)(struct uart_port *);
    void (*enable_ms)(struct uart_port *);
    void (*break_ctl)(struct uart_port *, int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*flush_buffer)(struct uart_port *);
    void (*set_termios)(struct uart_port *, struct ktermios *, const struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    const char * (*type)(struct uart_port *);
    void (*release_port)(struct uart_port *);
    int (*request_port)(struct uart_port *);
    void (*config_port)(struct uart_port *, int);
    int (*verify_port)(struct uart_port *, struct serial_struct *);
    int (*ioctl)(struct uart_port *, unsigned int, long unsigned int);
    int (*poll_init)(struct uart_port *);
    void (*poll_put_char)(struct uart_port *, unsigned char);
    int (*poll_get_char)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct uart_ops {
    unsigned int (*tx_empty)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*stop_tx)(struct uart_port *);
    void (*start_tx)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    void (*send_xchar)(struct uart_port *, char);
    void (*stop_rx)(struct uart_port *);
    void (*start_rx)(struct uart_port *);
    void (*enable_ms)(struct uart_port *);
    void (*break_ctl)(struct uart_port *, int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*flush_buffer)(struct uart_port *);
    void (*set_termios)(struct uart_port *, struct ktermios *, const struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    const char * (*type)(struct uart_port *);
    void (*release_port)(struct uart_port *);
    int (*request_port)(struct uart_port *);
    void (*config_port)(struct uart_port *, int);
    int (*verify_port)(struct uart_port *, struct serial_struct *);
    int (*ioctl)(struct uart_port *, unsigned int, long unsigned int);
    int (*poll_init)(struct uart_port *);
    void (*poll_put_char)(struct uart_port *, unsigned char);
    int (*poll_get_char)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct uart_ops {
    unsigned int (*tx_empty)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*stop_tx)(struct uart_port *);
    void (*start_tx)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    void (*send_xchar)(struct uart_port *, char);
    void (*stop_rx)(struct uart_port *);
    void (*start_rx)(struct uart_port *);
    void (*enable_ms)(struct uart_port *);
    void (*break_ctl)(struct uart_port *, int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*flush_buffer)(struct uart_port *);
    void (*set_termios)(struct uart_port *, struct ktermios *, const struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    const char * (*type)(struct uart_port *);
    void (*release_port)(struct uart_port *);
    int (*request_port)(struct uart_port *);
    void (*config_port)(struct uart_port *, int);
    int (*verify_port)(struct uart_port *, struct serial_struct *);
    int (*ioctl)(struct uart_port *, unsigned int, long unsigned int);
    int (*poll_init)(struct uart_port *);
    void (*poll_put_char)(struct uart_port *, unsigned char);
    int (*poll_get_char)(struct uart_port *);
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
struct uart_ops {
    unsigned int (*tx_empty)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*stop_tx)(struct uart_port *);
    void (*start_tx)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    void (*send_xchar)(struct uart_port *, char);
    void (*stop_rx)(struct uart_port *);
    void (*enable_ms)(struct uart_port *);
    void (*break_ctl)(struct uart_port *, int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*flush_buffer)(struct uart_port *);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    const char * (*type)(struct uart_port *);
    void (*release_port)(struct uart_port *);
    int (*request_port)(struct uart_port *);
    void (*config_port)(struct uart_port *, int);
    int (*verify_port)(struct uart_port *, struct serial_struct *);
    int (*ioctl)(struct uart_port *, unsigned int, long unsigned int);
    int (*poll_init)(struct uart_port *);
    void (*poll_put_char)(struct uart_port *, unsigned char);
    int (*poll_get_char)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct uart_ops {
    unsigned int (*tx_empty)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*stop_tx)(struct uart_port *);
    void (*start_tx)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    void (*send_xchar)(struct uart_port *, char);
    void (*stop_rx)(struct uart_port *);
    void (*enable_ms)(struct uart_port *);
    void (*break_ctl)(struct uart_port *, int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*flush_buffer)(struct uart_port *);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    const char * (*type)(struct uart_port *);
    void (*release_port)(struct uart_port *);
    int (*request_port)(struct uart_port *);
    void (*config_port)(struct uart_port *, int);
    int (*verify_port)(struct uart_port *, struct serial_struct *);
    int (*ioctl)(struct uart_port *, unsigned int, long unsigned int);
    int (*poll_init)(struct uart_port *);
    void (*poll_put_char)(struct uart_port *, unsigned char);
    int (*poll_get_char)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct uart_ops {
    unsigned int (*tx_empty)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*stop_tx)(struct uart_port *);
    void (*start_tx)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    void (*send_xchar)(struct uart_port *, char);
    void (*stop_rx)(struct uart_port *);
    void (*enable_ms)(struct uart_port *);
    void (*break_ctl)(struct uart_port *, int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*flush_buffer)(struct uart_port *);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    const char * (*type)(struct uart_port *);
    void (*release_port)(struct uart_port *);
    int (*request_port)(struct uart_port *);
    void (*config_port)(struct uart_port *, int);
    int (*verify_port)(struct uart_port *, struct serial_struct *);
    int (*ioctl)(struct uart_port *, unsigned int, long unsigned int);
    int (*poll_init)(struct uart_port *);
    void (*poll_put_char)(struct uart_port *, unsigned char);
    int (*poll_get_char)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct uart_ops {
    unsigned int (*tx_empty)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*stop_tx)(struct uart_port *);
    void (*start_tx)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    void (*send_xchar)(struct uart_port *, char);
    void (*stop_rx)(struct uart_port *);
    void (*enable_ms)(struct uart_port *);
    void (*break_ctl)(struct uart_port *, int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*flush_buffer)(struct uart_port *);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    const char * (*type)(struct uart_port *);
    void (*release_port)(struct uart_port *);
    int (*request_port)(struct uart_port *);
    void (*config_port)(struct uart_port *, int);
    int (*verify_port)(struct uart_port *, struct serial_struct *);
    int (*ioctl)(struct uart_port *, unsigned int, long unsigned int);
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
struct uart_ops {
    unsigned int (*tx_empty)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*stop_tx)(struct uart_port *);
    void (*start_tx)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    void (*send_xchar)(struct uart_port *, char);
    void (*stop_rx)(struct uart_port *);
    void (*enable_ms)(struct uart_port *);
    void (*break_ctl)(struct uart_port *, int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*flush_buffer)(struct uart_port *);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    const char * (*type)(struct uart_port *);
    void (*release_port)(struct uart_port *);
    int (*request_port)(struct uart_port *);
    void (*config_port)(struct uart_port *, int);
    int (*verify_port)(struct uart_port *, struct serial_struct *);
    int (*ioctl)(struct uart_port *, unsigned int, long unsigned int);
    int (*poll_init)(struct uart_port *);
    void (*poll_put_char)(struct uart_port *, unsigned char);
    int (*poll_get_char)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct uart_ops {
    unsigned int (*tx_empty)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*stop_tx)(struct uart_port *);
    void (*start_tx)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    void (*send_xchar)(struct uart_port *, char);
    void (*stop_rx)(struct uart_port *);
    void (*enable_ms)(struct uart_port *);
    void (*break_ctl)(struct uart_port *, int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*flush_buffer)(struct uart_port *);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    const char * (*type)(struct uart_port *);
    void (*release_port)(struct uart_port *);
    int (*request_port)(struct uart_port *);
    void (*config_port)(struct uart_port *, int);
    int (*verify_port)(struct uart_port *, struct serial_struct *);
    int (*ioctl)(struct uart_port *, unsigned int, long unsigned int);
    int (*poll_init)(struct uart_port *);
    void (*poll_put_char)(struct uart_port *, unsigned char);
    int (*poll_get_char)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct uart_ops {
    unsigned int (*tx_empty)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*stop_tx)(struct uart_port *);
    void (*start_tx)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    void (*send_xchar)(struct uart_port *, char);
    void (*stop_rx)(struct uart_port *);
    void (*enable_ms)(struct uart_port *);
    void (*break_ctl)(struct uart_port *, int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*flush_buffer)(struct uart_port *);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    const char * (*type)(struct uart_port *);
    void (*release_port)(struct uart_port *);
    int (*request_port)(struct uart_port *);
    void (*config_port)(struct uart_port *, int);
    int (*verify_port)(struct uart_port *, struct serial_struct *);
    int (*ioctl)(struct uart_port *, unsigned int, long unsigned int);
    int (*poll_init)(struct uart_port *);
    void (*poll_put_char)(struct uart_port *, unsigned char);
    int (*poll_get_char)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct uart_ops {
    unsigned int (*tx_empty)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*stop_tx)(struct uart_port *);
    void (*start_tx)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    void (*send_xchar)(struct uart_port *, char);
    void (*stop_rx)(struct uart_port *);
    void (*enable_ms)(struct uart_port *);
    void (*break_ctl)(struct uart_port *, int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*flush_buffer)(struct uart_port *);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    const char * (*type)(struct uart_port *);
    void (*release_port)(struct uart_port *);
    int (*request_port)(struct uart_port *);
    void (*config_port)(struct uart_port *, int);
    int (*verify_port)(struct uart_port *, struct serial_struct *);
    int (*ioctl)(struct uart_port *, unsigned int, long unsigned int);
    int (*poll_init)(struct uart_port *);
    void (*poll_put_char)(struct uart_port *, unsigned char);
    int (*poll_get_char)(struct uart_port *);
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*start_rx)(struct uart_port *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *)</code> ➡️ <code>void (*set_termios)(struct uart_port *, struct ktermios *, const struct ktermios *)</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*poll_init)(struct uart_port *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*poll_put_char)(struct uart_port *, unsigned char)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*poll_get_char)(struct uart_port *)</code>
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
