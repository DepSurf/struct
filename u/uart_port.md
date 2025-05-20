# Struct: <code>uart_port</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct uart_port {
    spinlock_t lock;
    long unsigned int iobase;
    unsigned char *membase;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
    int (*rs485_config)(struct uart_port *, struct serial_rs485 *);
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    unsigned int fifosize;
    unsigned char x_char;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char unused1;
    unsigned int read_status_mask;
    unsigned int ignore_status_mask;
    struct uart_state *state;
    struct uart_icount icount;
    struct console *cons;
    long unsigned int sysrq;
    upf_t flags;
    upstat_t status;
    int hw_stopped;
    unsigned int mctrl;
    unsigned int timeout;
    unsigned int type;
    const struct uart_ops *ops;
    unsigned int custom_divisor;
    unsigned int line;
    unsigned int minor;
    resource_size_t mapbase;
    resource_size_t mapsize;
    struct device *dev;
    unsigned char hub6;
    unsigned char suspended;
    unsigned char irq_wake;
    unsigned char unused[2];
    struct attribute_group *attr_group;
    const struct attribute_group **tty_groups;
    struct serial_rs485 rs485;
    void *private_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct uart_port {
    spinlock_t lock;
    long unsigned int iobase;
    unsigned char *membase;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
    int (*rs485_config)(struct uart_port *, struct serial_rs485 *);
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    unsigned int fifosize;
    unsigned char x_char;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char unused1;
    unsigned int read_status_mask;
    unsigned int ignore_status_mask;
    struct uart_state *state;
    struct uart_icount icount;
    struct console *cons;
    long unsigned int sysrq;
    upf_t flags;
    upstat_t status;
    int hw_stopped;
    unsigned int mctrl;
    unsigned int timeout;
    unsigned int type;
    const struct uart_ops *ops;
    unsigned int custom_divisor;
    unsigned int line;
    unsigned int minor;
    resource_size_t mapbase;
    resource_size_t mapsize;
    struct device *dev;
    unsigned char hub6;
    unsigned char suspended;
    unsigned char irq_wake;
    unsigned char unused[2];
    struct attribute_group *attr_group;
    const struct attribute_group **tty_groups;
    struct serial_rs485 rs485;
    void *private_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct uart_port {
    spinlock_t lock;
    long unsigned int iobase;
    unsigned char *membase;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
    int (*rs485_config)(struct uart_port *, struct serial_rs485 *);
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    unsigned int fifosize;
    unsigned char x_char;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char unused1;
    unsigned int read_status_mask;
    unsigned int ignore_status_mask;
    struct uart_state *state;
    struct uart_icount icount;
    struct console *cons;
    long unsigned int sysrq;
    upf_t flags;
    upstat_t status;
    int hw_stopped;
    unsigned int mctrl;
    unsigned int timeout;
    unsigned int type;
    const struct uart_ops *ops;
    unsigned int custom_divisor;
    unsigned int line;
    unsigned int minor;
    resource_size_t mapbase;
    resource_size_t mapsize;
    struct device *dev;
    unsigned char hub6;
    unsigned char suspended;
    unsigned char irq_wake;
    unsigned char unused[2];
    struct attribute_group *attr_group;
    const struct attribute_group **tty_groups;
    struct serial_rs485 rs485;
    void *private_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct uart_port {
    spinlock_t lock;
    long unsigned int iobase;
    unsigned char *membase;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
    int (*rs485_config)(struct uart_port *, struct serial_rs485 *);
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    unsigned int fifosize;
    unsigned char x_char;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char unused1;
    unsigned int read_status_mask;
    unsigned int ignore_status_mask;
    struct uart_state *state;
    struct uart_icount icount;
    struct console *cons;
    long unsigned int sysrq;
    upf_t flags;
    upstat_t status;
    int hw_stopped;
    unsigned int mctrl;
    unsigned int timeout;
    unsigned int type;
    const struct uart_ops *ops;
    unsigned int custom_divisor;
    unsigned int line;
    unsigned int minor;
    resource_size_t mapbase;
    resource_size_t mapsize;
    struct device *dev;
    unsigned char hub6;
    unsigned char suspended;
    unsigned char irq_wake;
    unsigned char unused[2];
    const char *name;
    struct attribute_group *attr_group;
    const struct attribute_group **tty_groups;
    struct serial_rs485 rs485;
    void *private_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct uart_port {
    spinlock_t lock;
    long unsigned int iobase;
    unsigned char *membase;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
    int (*rs485_config)(struct uart_port *, struct serial_rs485 *);
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    unsigned int fifosize;
    unsigned char x_char;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char quirks;
    unsigned int read_status_mask;
    unsigned int ignore_status_mask;
    struct uart_state *state;
    struct uart_icount icount;
    struct console *cons;
    long unsigned int sysrq;
    upf_t flags;
    upstat_t status;
    int hw_stopped;
    unsigned int mctrl;
    unsigned int timeout;
    unsigned int type;
    const struct uart_ops *ops;
    unsigned int custom_divisor;
    unsigned int line;
    unsigned int minor;
    resource_size_t mapbase;
    resource_size_t mapsize;
    struct device *dev;
    unsigned char hub6;
    unsigned char suspended;
    unsigned char unused[2];
    const char *name;
    struct attribute_group *attr_group;
    const struct attribute_group **tty_groups;
    struct serial_rs485 rs485;
    void *private_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct uart_port {
    spinlock_t lock;
    long unsigned int iobase;
    unsigned char *membase;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
    int (*rs485_config)(struct uart_port *, struct serial_rs485 *);
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    unsigned int fifosize;
    unsigned char x_char;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char quirks;
    unsigned int read_status_mask;
    unsigned int ignore_status_mask;
    struct uart_state *state;
    struct uart_icount icount;
    struct console *cons;
    long unsigned int sysrq;
    upf_t flags;
    upstat_t status;
    int hw_stopped;
    unsigned int mctrl;
    unsigned int timeout;
    unsigned int type;
    const struct uart_ops *ops;
    unsigned int custom_divisor;
    unsigned int line;
    unsigned int minor;
    resource_size_t mapbase;
    resource_size_t mapsize;
    struct device *dev;
    unsigned char hub6;
    unsigned char suspended;
    unsigned char unused[2];
    const char *name;
    struct attribute_group *attr_group;
    const struct attribute_group **tty_groups;
    struct serial_rs485 rs485;
    void *private_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct uart_port {
    spinlock_t lock;
    long unsigned int iobase;
    unsigned char *membase;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_divisor)(struct uart_port *, unsigned int, unsigned int *);
    void (*set_divisor)(struct uart_port *, unsigned int, unsigned int, unsigned int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
    int (*rs485_config)(struct uart_port *, struct serial_rs485 *);
    int (*iso7816_config)(struct uart_port *, struct serial_iso7816 *);
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    unsigned int fifosize;
    unsigned char x_char;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char quirks;
    unsigned int read_status_mask;
    unsigned int ignore_status_mask;
    struct uart_state *state;
    struct uart_icount icount;
    struct console *cons;
    long unsigned int sysrq;
    unsigned int sysrq_ch;
    upf_t flags;
    upstat_t status;
    int hw_stopped;
    unsigned int mctrl;
    unsigned int timeout;
    unsigned int type;
    const struct uart_ops *ops;
    unsigned int custom_divisor;
    unsigned int line;
    unsigned int minor;
    resource_size_t mapbase;
    resource_size_t mapsize;
    struct device *dev;
    unsigned char hub6;
    unsigned char suspended;
    unsigned char unused[2];
    const char *name;
    struct attribute_group *attr_group;
    const struct attribute_group **tty_groups;
    struct serial_rs485 rs485;
    struct serial_iso7816 iso7816;
    void *private_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct uart_port {
    spinlock_t lock;
    long unsigned int iobase;
    unsigned char *membase;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_divisor)(struct uart_port *, unsigned int, unsigned int *);
    void (*set_divisor)(struct uart_port *, unsigned int, unsigned int, unsigned int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
    int (*rs485_config)(struct uart_port *, struct serial_rs485 *);
    int (*iso7816_config)(struct uart_port *, struct serial_iso7816 *);
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    unsigned int fifosize;
    unsigned char x_char;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char quirks;
    unsigned int read_status_mask;
    unsigned int ignore_status_mask;
    struct uart_state *state;
    struct uart_icount icount;
    struct console *cons;
    long unsigned int sysrq;
    unsigned int sysrq_ch;
    upf_t flags;
    upstat_t status;
    int hw_stopped;
    unsigned int mctrl;
    unsigned int timeout;
    unsigned int type;
    const struct uart_ops *ops;
    unsigned int custom_divisor;
    unsigned int line;
    unsigned int minor;
    resource_size_t mapbase;
    resource_size_t mapsize;
    struct device *dev;
    unsigned char hub6;
    unsigned char suspended;
    unsigned char unused[2];
    const char *name;
    struct attribute_group *attr_group;
    const struct attribute_group **tty_groups;
    struct serial_rs485 rs485;
    struct serial_iso7816 iso7816;
    void *private_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct uart_port {
    spinlock_t lock;
    long unsigned int iobase;
    unsigned char *membase;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_divisor)(struct uart_port *, unsigned int, unsigned int *);
    void (*set_divisor)(struct uart_port *, unsigned int, unsigned int, unsigned int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
    int (*rs485_config)(struct uart_port *, struct serial_rs485 *);
    int (*iso7816_config)(struct uart_port *, struct serial_iso7816 *);
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    unsigned int fifosize;
    unsigned char x_char;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char quirks;
    unsigned int read_status_mask;
    unsigned int ignore_status_mask;
    struct uart_state *state;
    struct uart_icount icount;
    struct console *cons;
    long unsigned int sysrq;
    unsigned int sysrq_ch;
    upf_t flags;
    upstat_t status;
    int hw_stopped;
    unsigned int mctrl;
    unsigned int timeout;
    unsigned int type;
    const struct uart_ops *ops;
    unsigned int custom_divisor;
    unsigned int line;
    unsigned int minor;
    resource_size_t mapbase;
    resource_size_t mapsize;
    struct device *dev;
    unsigned char hub6;
    unsigned char suspended;
    unsigned char unused[2];
    const char *name;
    struct attribute_group *attr_group;
    const struct attribute_group **tty_groups;
    struct serial_rs485 rs485;
    struct serial_iso7816 iso7816;
    void *private_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct uart_port {
    spinlock_t lock;
    long unsigned int iobase;
    unsigned char *membase;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_divisor)(struct uart_port *, unsigned int, unsigned int *);
    void (*set_divisor)(struct uart_port *, unsigned int, unsigned int, unsigned int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
    int (*rs485_config)(struct uart_port *, struct serial_rs485 *);
    int (*iso7816_config)(struct uart_port *, struct serial_iso7816 *);
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    unsigned int fifosize;
    unsigned char x_char;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char quirks;
    unsigned int read_status_mask;
    unsigned int ignore_status_mask;
    struct uart_state *state;
    struct uart_icount icount;
    struct console *cons;
    upf_t flags;
    upstat_t status;
    int hw_stopped;
    unsigned int mctrl;
    unsigned int timeout;
    unsigned int type;
    const struct uart_ops *ops;
    unsigned int custom_divisor;
    unsigned int line;
    unsigned int minor;
    resource_size_t mapbase;
    resource_size_t mapsize;
    struct device *dev;
    long unsigned int sysrq;
    unsigned int sysrq_ch;
    unsigned char has_sysrq;
    unsigned char sysrq_seq;
    unsigned char hub6;
    unsigned char suspended;
    unsigned char console_reinit;
    const char *name;
    struct attribute_group *attr_group;
    const struct attribute_group **tty_groups;
    struct serial_rs485 rs485;
    struct gpio_desc *rs485_term_gpio;
    struct serial_iso7816 iso7816;
    void *private_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct uart_port {
    spinlock_t lock;
    long unsigned int iobase;
    unsigned char *membase;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_divisor)(struct uart_port *, unsigned int, unsigned int *);
    void (*set_divisor)(struct uart_port *, unsigned int, unsigned int, unsigned int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
    int (*rs485_config)(struct uart_port *, struct serial_rs485 *);
    int (*iso7816_config)(struct uart_port *, struct serial_iso7816 *);
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    unsigned int fifosize;
    unsigned char x_char;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char quirks;
    unsigned int read_status_mask;
    unsigned int ignore_status_mask;
    struct uart_state *state;
    struct uart_icount icount;
    struct console *cons;
    upf_t flags;
    upstat_t status;
    int hw_stopped;
    unsigned int mctrl;
    unsigned int timeout;
    unsigned int type;
    const struct uart_ops *ops;
    unsigned int custom_divisor;
    unsigned int line;
    unsigned int minor;
    resource_size_t mapbase;
    resource_size_t mapsize;
    struct device *dev;
    long unsigned int sysrq;
    unsigned int sysrq_ch;
    unsigned char has_sysrq;
    unsigned char sysrq_seq;
    unsigned char hub6;
    unsigned char suspended;
    unsigned char console_reinit;
    const char *name;
    struct attribute_group *attr_group;
    const struct attribute_group **tty_groups;
    struct serial_rs485 rs485;
    struct gpio_desc *rs485_term_gpio;
    struct serial_iso7816 iso7816;
    void *private_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct uart_port {
    spinlock_t lock;
    long unsigned int iobase;
    unsigned char *membase;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_divisor)(struct uart_port *, unsigned int, unsigned int *);
    void (*set_divisor)(struct uart_port *, unsigned int, unsigned int, unsigned int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
    int (*rs485_config)(struct uart_port *, struct serial_rs485 *);
    int (*iso7816_config)(struct uart_port *, struct serial_iso7816 *);
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    unsigned int fifosize;
    unsigned char x_char;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char quirks;
    unsigned int read_status_mask;
    unsigned int ignore_status_mask;
    struct uart_state *state;
    struct uart_icount icount;
    struct console *cons;
    upf_t flags;
    upstat_t status;
    int hw_stopped;
    unsigned int mctrl;
    unsigned int timeout;
    unsigned int type;
    const struct uart_ops *ops;
    unsigned int custom_divisor;
    unsigned int line;
    unsigned int minor;
    resource_size_t mapbase;
    resource_size_t mapsize;
    struct device *dev;
    long unsigned int sysrq;
    unsigned int sysrq_ch;
    unsigned char has_sysrq;
    unsigned char sysrq_seq;
    unsigned char hub6;
    unsigned char suspended;
    unsigned char console_reinit;
    const char *name;
    struct attribute_group *attr_group;
    const struct attribute_group **tty_groups;
    struct serial_rs485 rs485;
    struct gpio_desc *rs485_term_gpio;
    struct serial_iso7816 iso7816;
    void *private_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct uart_port {
    spinlock_t lock;
    long unsigned int iobase;
    unsigned char *membase;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_divisor)(struct uart_port *, unsigned int, unsigned int *);
    void (*set_divisor)(struct uart_port *, unsigned int, unsigned int, unsigned int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
    int (*rs485_config)(struct uart_port *, struct serial_rs485 *);
    int (*iso7816_config)(struct uart_port *, struct serial_iso7816 *);
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    unsigned int fifosize;
    unsigned char x_char;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char quirks;
    unsigned int read_status_mask;
    unsigned int ignore_status_mask;
    struct uart_state *state;
    struct uart_icount icount;
    struct console *cons;
    upf_t flags;
    upstat_t status;
    int hw_stopped;
    unsigned int mctrl;
    unsigned int timeout;
    unsigned int type;
    const struct uart_ops *ops;
    unsigned int custom_divisor;
    unsigned int line;
    unsigned int minor;
    resource_size_t mapbase;
    resource_size_t mapsize;
    struct device *dev;
    long unsigned int sysrq;
    unsigned int sysrq_ch;
    unsigned char has_sysrq;
    unsigned char sysrq_seq;
    unsigned char hub6;
    unsigned char suspended;
    unsigned char console_reinit;
    const char *name;
    struct attribute_group *attr_group;
    const struct attribute_group **tty_groups;
    struct serial_rs485 rs485;
    struct gpio_desc *rs485_term_gpio;
    struct serial_iso7816 iso7816;
    void *private_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct uart_port {
    spinlock_t lock;
    long unsigned int iobase;
    unsigned char *membase;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_divisor)(struct uart_port *, unsigned int, unsigned int *);
    void (*set_divisor)(struct uart_port *, unsigned int, unsigned int, unsigned int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
    int (*rs485_config)(struct uart_port *, struct serial_rs485 *);
    int (*iso7816_config)(struct uart_port *, struct serial_iso7816 *);
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    unsigned int fifosize;
    unsigned char x_char;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char quirks;
    unsigned int read_status_mask;
    unsigned int ignore_status_mask;
    struct uart_state *state;
    struct uart_icount icount;
    struct console *cons;
    upf_t flags;
    upstat_t status;
    int hw_stopped;
    unsigned int mctrl;
    unsigned int timeout;
    unsigned int frame_time;
    unsigned int type;
    const struct uart_ops *ops;
    unsigned int custom_divisor;
    unsigned int line;
    unsigned int minor;
    resource_size_t mapbase;
    resource_size_t mapsize;
    struct device *dev;
    long unsigned int sysrq;
    unsigned int sysrq_ch;
    unsigned char has_sysrq;
    unsigned char sysrq_seq;
    unsigned char hub6;
    unsigned char suspended;
    unsigned char console_reinit;
    const char *name;
    struct attribute_group *attr_group;
    const struct attribute_group **tty_groups;
    struct serial_rs485 rs485;
    struct gpio_desc *rs485_term_gpio;
    struct serial_iso7816 iso7816;
    void *private_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct uart_port {
    spinlock_t lock;
    long unsigned int iobase;
    unsigned char *membase;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, const struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_divisor)(struct uart_port *, unsigned int, unsigned int *);
    void (*set_divisor)(struct uart_port *, unsigned int, unsigned int, unsigned int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
    int (*rs485_config)(struct uart_port *, struct ktermios *, struct serial_rs485 *);
    int (*iso7816_config)(struct uart_port *, struct serial_iso7816 *);
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    unsigned int fifosize;
    unsigned char x_char;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char quirks;
    unsigned int read_status_mask;
    unsigned int ignore_status_mask;
    struct uart_state *state;
    struct uart_icount icount;
    struct console *cons;
    upf_t flags;
    upstat_t status;
    int hw_stopped;
    unsigned int mctrl;
    unsigned int frame_time;
    unsigned int type;
    const struct uart_ops *ops;
    unsigned int custom_divisor;
    unsigned int line;
    unsigned int minor;
    resource_size_t mapbase;
    resource_size_t mapsize;
    struct device *dev;
    long unsigned int sysrq;
    unsigned int sysrq_ch;
    unsigned char has_sysrq;
    unsigned char sysrq_seq;
    unsigned char hub6;
    unsigned char suspended;
    unsigned char console_reinit;
    const char *name;
    struct attribute_group *attr_group;
    const struct attribute_group **tty_groups;
    struct serial_rs485 rs485;
    struct serial_rs485 rs485_supported;
    struct gpio_desc *rs485_term_gpio;
    struct serial_iso7816 iso7816;
    void *private_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct uart_port {
    spinlock_t lock;
    long unsigned int iobase;
    unsigned char *membase;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, const struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_divisor)(struct uart_port *, unsigned int, unsigned int *);
    void (*set_divisor)(struct uart_port *, unsigned int, unsigned int, unsigned int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
    int (*rs485_config)(struct uart_port *, struct ktermios *, struct serial_rs485 *);
    int (*iso7816_config)(struct uart_port *, struct serial_iso7816 *);
    unsigned int ctrl_id;
    unsigned int port_id;
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    unsigned int fifosize;
    unsigned char x_char;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char quirks;
    unsigned int read_status_mask;
    unsigned int ignore_status_mask;
    struct uart_state *state;
    struct uart_icount icount;
    struct console *cons;
    upf_t flags;
    upstat_t status;
    bool hw_stopped;
    unsigned int mctrl;
    unsigned int frame_time;
    unsigned int type;
    const struct uart_ops *ops;
    unsigned int custom_divisor;
    unsigned int line;
    unsigned int minor;
    resource_size_t mapbase;
    resource_size_t mapsize;
    struct device *dev;
    struct serial_port_device *port_dev;
    long unsigned int sysrq;
    unsigned int sysrq_ch;
    unsigned char has_sysrq;
    unsigned char sysrq_seq;
    unsigned char hub6;
    unsigned char suspended;
    unsigned char console_reinit;
    const char *name;
    struct attribute_group *attr_group;
    const struct attribute_group **tty_groups;
    struct serial_rs485 rs485;
    struct serial_rs485 rs485_supported;
    struct gpio_desc *rs485_term_gpio;
    struct gpio_desc *rs485_rx_during_tx_gpio;
    struct serial_iso7816 iso7816;
    void *private_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct uart_port {
    spinlock_t lock;
    long unsigned int iobase;
    unsigned char *membase;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, const struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_divisor)(struct uart_port *, unsigned int, unsigned int *);
    void (*set_divisor)(struct uart_port *, unsigned int, unsigned int, unsigned int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
    int (*rs485_config)(struct uart_port *, struct ktermios *, struct serial_rs485 *);
    int (*iso7816_config)(struct uart_port *, struct serial_iso7816 *);
    unsigned int ctrl_id;
    unsigned int port_id;
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    unsigned int fifosize;
    unsigned char x_char;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char quirks;
    unsigned int read_status_mask;
    unsigned int ignore_status_mask;
    struct uart_state *state;
    struct uart_icount icount;
    struct console *cons;
    upf_t flags;
    upstat_t status;
    bool hw_stopped;
    unsigned int mctrl;
    unsigned int frame_time;
    unsigned int type;
    const struct uart_ops *ops;
    unsigned int custom_divisor;
    unsigned int line;
    unsigned int minor;
    resource_size_t mapbase;
    resource_size_t mapsize;
    struct device *dev;
    struct serial_port_device *port_dev;
    long unsigned int sysrq;
    u8 sysrq_ch;
    unsigned char has_sysrq;
    unsigned char sysrq_seq;
    unsigned char hub6;
    unsigned char suspended;
    unsigned char console_reinit;
    const char *name;
    struct attribute_group *attr_group;
    const struct attribute_group **tty_groups;
    struct serial_rs485 rs485;
    struct serial_rs485 rs485_supported;
    struct gpio_desc *rs485_term_gpio;
    struct gpio_desc *rs485_rx_during_tx_gpio;
    struct serial_iso7816 iso7816;
    void *private_data;
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
struct uart_port {
    spinlock_t lock;
    long unsigned int iobase;
    unsigned char *membase;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_divisor)(struct uart_port *, unsigned int, unsigned int *);
    void (*set_divisor)(struct uart_port *, unsigned int, unsigned int, unsigned int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
    int (*rs485_config)(struct uart_port *, struct serial_rs485 *);
    int (*iso7816_config)(struct uart_port *, struct serial_iso7816 *);
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    unsigned int fifosize;
    unsigned char x_char;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char quirks;
    unsigned int read_status_mask;
    unsigned int ignore_status_mask;
    struct uart_state *state;
    struct uart_icount icount;
    struct console *cons;
    long unsigned int sysrq;
    unsigned int sysrq_ch;
    upf_t flags;
    upstat_t status;
    int hw_stopped;
    unsigned int mctrl;
    unsigned int timeout;
    unsigned int type;
    const struct uart_ops *ops;
    unsigned int custom_divisor;
    unsigned int line;
    unsigned int minor;
    resource_size_t mapbase;
    resource_size_t mapsize;
    struct device *dev;
    unsigned char hub6;
    unsigned char suspended;
    unsigned char unused[2];
    const char *name;
    struct attribute_group *attr_group;
    const struct attribute_group **tty_groups;
    struct serial_rs485 rs485;
    struct serial_iso7816 iso7816;
    void *private_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct uart_port {
    spinlock_t lock;
    long unsigned int iobase;
    unsigned char *membase;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_divisor)(struct uart_port *, unsigned int, unsigned int *);
    void (*set_divisor)(struct uart_port *, unsigned int, unsigned int, unsigned int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
    int (*rs485_config)(struct uart_port *, struct serial_rs485 *);
    int (*iso7816_config)(struct uart_port *, struct serial_iso7816 *);
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    unsigned int fifosize;
    unsigned char x_char;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char quirks;
    unsigned int read_status_mask;
    unsigned int ignore_status_mask;
    struct uart_state *state;
    struct uart_icount icount;
    struct console *cons;
    long unsigned int sysrq;
    unsigned int sysrq_ch;
    upf_t flags;
    upstat_t status;
    int hw_stopped;
    unsigned int mctrl;
    unsigned int timeout;
    unsigned int type;
    const struct uart_ops *ops;
    unsigned int custom_divisor;
    unsigned int line;
    unsigned int minor;
    resource_size_t mapbase;
    resource_size_t mapsize;
    struct device *dev;
    unsigned char hub6;
    unsigned char suspended;
    unsigned char unused[2];
    const char *name;
    struct attribute_group *attr_group;
    const struct attribute_group **tty_groups;
    struct serial_rs485 rs485;
    struct serial_iso7816 iso7816;
    void *private_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct uart_port {
    spinlock_t lock;
    long unsigned int iobase;
    unsigned char *membase;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_divisor)(struct uart_port *, unsigned int, unsigned int *);
    void (*set_divisor)(struct uart_port *, unsigned int, unsigned int, unsigned int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
    int (*rs485_config)(struct uart_port *, struct serial_rs485 *);
    int (*iso7816_config)(struct uart_port *, struct serial_iso7816 *);
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    unsigned int fifosize;
    unsigned char x_char;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char quirks;
    unsigned int read_status_mask;
    unsigned int ignore_status_mask;
    struct uart_state *state;
    struct uart_icount icount;
    struct console *cons;
    long unsigned int sysrq;
    unsigned int sysrq_ch;
    upf_t flags;
    upstat_t status;
    int hw_stopped;
    unsigned int mctrl;
    unsigned int timeout;
    unsigned int type;
    const struct uart_ops *ops;
    unsigned int custom_divisor;
    unsigned int line;
    unsigned int minor;
    resource_size_t mapbase;
    resource_size_t mapsize;
    struct device *dev;
    unsigned char hub6;
    unsigned char suspended;
    unsigned char unused[2];
    const char *name;
    struct attribute_group *attr_group;
    const struct attribute_group **tty_groups;
    struct serial_rs485 rs485;
    struct serial_iso7816 iso7816;
    void *private_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct uart_port {
    spinlock_t lock;
    long unsigned int iobase;
    unsigned char *membase;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_divisor)(struct uart_port *, unsigned int, unsigned int *);
    void (*set_divisor)(struct uart_port *, unsigned int, unsigned int, unsigned int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
    int (*rs485_config)(struct uart_port *, struct serial_rs485 *);
    int (*iso7816_config)(struct uart_port *, struct serial_iso7816 *);
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    unsigned int fifosize;
    unsigned char x_char;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char quirks;
    unsigned int read_status_mask;
    unsigned int ignore_status_mask;
    struct uart_state *state;
    struct uart_icount icount;
    struct console *cons;
    long unsigned int sysrq;
    unsigned int sysrq_ch;
    upf_t flags;
    upstat_t status;
    int hw_stopped;
    unsigned int mctrl;
    unsigned int timeout;
    unsigned int type;
    const struct uart_ops *ops;
    unsigned int custom_divisor;
    unsigned int line;
    unsigned int minor;
    resource_size_t mapbase;
    resource_size_t mapsize;
    struct device *dev;
    unsigned char hub6;
    unsigned char suspended;
    unsigned char unused[2];
    const char *name;
    struct attribute_group *attr_group;
    const struct attribute_group **tty_groups;
    struct serial_rs485 rs485;
    struct serial_iso7816 iso7816;
    void *private_data;
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
struct uart_port {
    spinlock_t lock;
    long unsigned int iobase;
    unsigned char *membase;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_divisor)(struct uart_port *, unsigned int, unsigned int *);
    void (*set_divisor)(struct uart_port *, unsigned int, unsigned int, unsigned int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
    int (*rs485_config)(struct uart_port *, struct serial_rs485 *);
    int (*iso7816_config)(struct uart_port *, struct serial_iso7816 *);
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    unsigned int fifosize;
    unsigned char x_char;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char quirks;
    unsigned int read_status_mask;
    unsigned int ignore_status_mask;
    struct uart_state *state;
    struct uart_icount icount;
    struct console *cons;
    long unsigned int sysrq;
    unsigned int sysrq_ch;
    upf_t flags;
    upstat_t status;
    int hw_stopped;
    unsigned int mctrl;
    unsigned int timeout;
    unsigned int type;
    const struct uart_ops *ops;
    unsigned int custom_divisor;
    unsigned int line;
    unsigned int minor;
    resource_size_t mapbase;
    resource_size_t mapsize;
    struct device *dev;
    unsigned char hub6;
    unsigned char suspended;
    unsigned char unused[2];
    const char *name;
    struct attribute_group *attr_group;
    const struct attribute_group **tty_groups;
    struct serial_rs485 rs485;
    struct serial_iso7816 iso7816;
    void *private_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct uart_port {
    spinlock_t lock;
    long unsigned int iobase;
    unsigned char *membase;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_divisor)(struct uart_port *, unsigned int, unsigned int *);
    void (*set_divisor)(struct uart_port *, unsigned int, unsigned int, unsigned int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
    int (*rs485_config)(struct uart_port *, struct serial_rs485 *);
    int (*iso7816_config)(struct uart_port *, struct serial_iso7816 *);
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    unsigned int fifosize;
    unsigned char x_char;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char quirks;
    unsigned int read_status_mask;
    unsigned int ignore_status_mask;
    struct uart_state *state;
    struct uart_icount icount;
    struct console *cons;
    long unsigned int sysrq;
    unsigned int sysrq_ch;
    upf_t flags;
    upstat_t status;
    int hw_stopped;
    unsigned int mctrl;
    unsigned int timeout;
    unsigned int type;
    const struct uart_ops *ops;
    unsigned int custom_divisor;
    unsigned int line;
    unsigned int minor;
    resource_size_t mapbase;
    resource_size_t mapsize;
    struct device *dev;
    unsigned char hub6;
    unsigned char suspended;
    unsigned char unused[2];
    const char *name;
    struct attribute_group *attr_group;
    const struct attribute_group **tty_groups;
    struct serial_rs485 rs485;
    struct serial_iso7816 iso7816;
    void *private_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct uart_port {
    spinlock_t lock;
    long unsigned int iobase;
    unsigned char *membase;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_divisor)(struct uart_port *, unsigned int, unsigned int *);
    void (*set_divisor)(struct uart_port *, unsigned int, unsigned int, unsigned int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
    int (*rs485_config)(struct uart_port *, struct serial_rs485 *);
    int (*iso7816_config)(struct uart_port *, struct serial_iso7816 *);
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    unsigned int fifosize;
    unsigned char x_char;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char quirks;
    unsigned int read_status_mask;
    unsigned int ignore_status_mask;
    struct uart_state *state;
    struct uart_icount icount;
    struct console *cons;
    long unsigned int sysrq;
    unsigned int sysrq_ch;
    upf_t flags;
    upstat_t status;
    int hw_stopped;
    unsigned int mctrl;
    unsigned int timeout;
    unsigned int type;
    const struct uart_ops *ops;
    unsigned int custom_divisor;
    unsigned int line;
    unsigned int minor;
    resource_size_t mapbase;
    resource_size_t mapsize;
    struct device *dev;
    unsigned char hub6;
    unsigned char suspended;
    unsigned char unused[2];
    const char *name;
    struct attribute_group *attr_group;
    const struct attribute_group **tty_groups;
    struct serial_rs485 rs485;
    struct serial_iso7816 iso7816;
    void *private_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct uart_port {
    spinlock_t lock;
    long unsigned int iobase;
    unsigned char *membase;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    void (*set_mctrl)(struct uart_port *, unsigned int);
    unsigned int (*get_divisor)(struct uart_port *, unsigned int, unsigned int *);
    void (*set_divisor)(struct uart_port *, unsigned int, unsigned int, unsigned int);
    int (*startup)(struct uart_port *);
    void (*shutdown)(struct uart_port *);
    void (*throttle)(struct uart_port *);
    void (*unthrottle)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
    int (*rs485_config)(struct uart_port *, struct serial_rs485 *);
    int (*iso7816_config)(struct uart_port *, struct serial_iso7816 *);
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    unsigned int fifosize;
    unsigned char x_char;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char quirks;
    unsigned int read_status_mask;
    unsigned int ignore_status_mask;
    struct uart_state *state;
    struct uart_icount icount;
    struct console *cons;
    long unsigned int sysrq;
    unsigned int sysrq_ch;
    upf_t flags;
    upstat_t status;
    int hw_stopped;
    unsigned int mctrl;
    unsigned int timeout;
    unsigned int type;
    const struct uart_ops *ops;
    unsigned int custom_divisor;
    unsigned int line;
    unsigned int minor;
    resource_size_t mapbase;
    resource_size_t mapsize;
    struct device *dev;
    unsigned char hub6;
    unsigned char suspended;
    unsigned char unused[2];
    const char *name;
    struct attribute_group *attr_group;
    const struct attribute_group **tty_groups;
    struct serial_rs485 rs485;
    struct serial_iso7816 iso7816;
    void *private_data;
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
<code>unsigned int (*get_mctrl)(struct uart_port *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*set_ldisc)(struct uart_port *, struct ktermios *)</code>
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
<code>const char *name</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned char quirks</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned char unused1</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned char irq_wake</code>
</li>
</ul>
</details>
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
<code>unsigned int (*get_divisor)(struct uart_port *, unsigned int, unsigned int *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*set_divisor)(struct uart_port *, unsigned int, unsigned int, unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*iso7816_config)(struct uart_port *, struct serial_iso7816 *)</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int sysrq_ch</code>
</li>
<li>
<b>Field added. </b>
<code>struct serial_iso7816 iso7816</code>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned char has_sysrq</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned char sysrq_seq</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned char console_reinit</code>
</li>
<li>
<b>Field added. </b>
<code>struct gpio_desc *rs485_term_gpio</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned char unused[2]</code>
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
<code>unsigned int frame_time</code>
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
<code>struct serial_rs485 rs485_supported</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int timeout</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *)</code> ➡️ <code>void (*set_termios)(struct uart_port *, struct ktermios *, const struct ktermios *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*rs485_config)(struct uart_port *, struct serial_rs485 *)</code> ➡️ <code>int (*rs485_config)(struct uart_port *, struct ktermios *, struct serial_rs485 *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int ctrl_id</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int port_id</code>
</li>
<li>
<b>Field added. </b>
<code>struct serial_port_device *port_dev</code>
</li>
<li>
<b>Field added. </b>
<code>struct gpio_desc *rs485_rx_during_tx_gpio</code>
</li>
<li>
<b>Field type changed. </b>
<code>int hw_stopped</code> ➡️ <code>bool hw_stopped</code>
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
<code>unsigned int sysrq_ch</code> ➡️ <code>u8 sysrq_ch</code>
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
