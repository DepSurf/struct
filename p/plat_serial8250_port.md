# Struct: <code>plat_serial8250_port</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct plat_serial8250_port {
    long unsigned int iobase;
    void *membase;
    resource_size_t mapbase;
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    void *private_data;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char hub6;
    upf_t flags;
    unsigned int type;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct plat_serial8250_port {
    long unsigned int iobase;
    void *membase;
    resource_size_t mapbase;
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    void *private_data;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char hub6;
    upf_t flags;
    unsigned int type;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct plat_serial8250_port {
    long unsigned int iobase;
    void *membase;
    resource_size_t mapbase;
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    void *private_data;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char hub6;
    upf_t flags;
    unsigned int type;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct plat_serial8250_port {
    long unsigned int iobase;
    void *membase;
    resource_size_t mapbase;
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    void *private_data;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char hub6;
    upf_t flags;
    unsigned int type;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct plat_serial8250_port {
    long unsigned int iobase;
    void *membase;
    resource_size_t mapbase;
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    void *private_data;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char hub6;
    upf_t flags;
    unsigned int type;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct plat_serial8250_port {
    long unsigned int iobase;
    void *membase;
    resource_size_t mapbase;
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    void *private_data;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char hub6;
    upf_t flags;
    unsigned int type;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct plat_serial8250_port {
    long unsigned int iobase;
    void *membase;
    resource_size_t mapbase;
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    void *private_data;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char hub6;
    upf_t flags;
    unsigned int type;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct plat_serial8250_port {
    long unsigned int iobase;
    void *membase;
    resource_size_t mapbase;
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    void *private_data;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char hub6;
    upf_t flags;
    unsigned int type;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct plat_serial8250_port {
    long unsigned int iobase;
    void *membase;
    resource_size_t mapbase;
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    void *private_data;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char hub6;
    upf_t flags;
    unsigned int type;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct plat_serial8250_port {
    long unsigned int iobase;
    void *membase;
    resource_size_t mapbase;
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    void *private_data;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char hub6;
    unsigned char has_sysrq;
    upf_t flags;
    unsigned int type;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct plat_serial8250_port {
    long unsigned int iobase;
    void *membase;
    resource_size_t mapbase;
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    void *private_data;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char hub6;
    unsigned char has_sysrq;
    upf_t flags;
    unsigned int type;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct plat_serial8250_port {
    long unsigned int iobase;
    void *membase;
    resource_size_t mapbase;
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    void *private_data;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char hub6;
    unsigned char has_sysrq;
    upf_t flags;
    unsigned int type;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct plat_serial8250_port {
    long unsigned int iobase;
    void *membase;
    resource_size_t mapbase;
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    void *private_data;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char hub6;
    unsigned char has_sysrq;
    upf_t flags;
    unsigned int type;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct plat_serial8250_port {
    long unsigned int iobase;
    void *membase;
    resource_size_t mapbase;
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    void *private_data;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char hub6;
    unsigned char has_sysrq;
    upf_t flags;
    unsigned int type;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct plat_serial8250_port {
    long unsigned int iobase;
    void *membase;
    resource_size_t mapbase;
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    void *private_data;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char hub6;
    unsigned char has_sysrq;
    upf_t flags;
    unsigned int type;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, const struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct plat_serial8250_port {
    long unsigned int iobase;
    void *membase;
    resource_size_t mapbase;
    resource_size_t mapsize;
    unsigned int uartclk;
    unsigned int irq;
    long unsigned int irqflags;
    void *private_data;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char hub6;
    unsigned char has_sysrq;
    unsigned int type;
    upf_t flags;
    u16 bugs;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    u32 (*dl_read)(struct uart_8250_port *);
    void (*dl_write)(struct uart_8250_port *, u32);
    void (*set_termios)(struct uart_port *, struct ktermios *, const struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct plat_serial8250_port {
    long unsigned int iobase;
    void *membase;
    resource_size_t mapbase;
    resource_size_t mapsize;
    unsigned int uartclk;
    unsigned int irq;
    long unsigned int irqflags;
    void *private_data;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char hub6;
    unsigned char has_sysrq;
    unsigned int type;
    upf_t flags;
    u16 bugs;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    u32 (*dl_read)(struct uart_8250_port *);
    void (*dl_write)(struct uart_8250_port *, u32);
    void (*set_termios)(struct uart_port *, struct ktermios *, const struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
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
struct plat_serial8250_port {
    long unsigned int iobase;
    void *membase;
    resource_size_t mapbase;
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    void *private_data;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char hub6;
    upf_t flags;
    unsigned int type;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct plat_serial8250_port {
    long unsigned int iobase;
    void *membase;
    resource_size_t mapbase;
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    void *private_data;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char hub6;
    upf_t flags;
    unsigned int type;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct plat_serial8250_port {
    long unsigned int iobase;
    void *membase;
    resource_size_t mapbase;
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    void *private_data;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char hub6;
    upf_t flags;
    unsigned int type;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct plat_serial8250_port {
    long unsigned int iobase;
    void *membase;
    resource_size_t mapbase;
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    void *private_data;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char hub6;
    upf_t flags;
    unsigned int type;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
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
struct plat_serial8250_port {
    long unsigned int iobase;
    void *membase;
    resource_size_t mapbase;
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    void *private_data;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char hub6;
    upf_t flags;
    unsigned int type;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct plat_serial8250_port {
    long unsigned int iobase;
    void *membase;
    resource_size_t mapbase;
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    void *private_data;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char hub6;
    upf_t flags;
    unsigned int type;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct plat_serial8250_port {
    long unsigned int iobase;
    void *membase;
    resource_size_t mapbase;
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    void *private_data;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char hub6;
    upf_t flags;
    unsigned int type;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct plat_serial8250_port {
    long unsigned int iobase;
    void *membase;
    resource_size_t mapbase;
    unsigned int irq;
    long unsigned int irqflags;
    unsigned int uartclk;
    void *private_data;
    unsigned char regshift;
    unsigned char iotype;
    unsigned char hub6;
    upf_t flags;
    unsigned int type;
    unsigned int (*serial_in)(struct uart_port *, int);
    void (*serial_out)(struct uart_port *, int, int);
    void (*set_termios)(struct uart_port *, struct ktermios *, struct ktermios *);
    void (*set_ldisc)(struct uart_port *, struct ktermios *);
    unsigned int (*get_mctrl)(struct uart_port *);
    int (*handle_irq)(struct uart_port *);
    void (*pm)(struct uart_port *, unsigned int, unsigned int);
    void (*handle_break)(struct uart_port *);
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned char has_sysrq</code>
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
No changes between <code>5.15</code> and <code>5.19</code> ✅
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>resource_size_t mapsize</code>
</li>
<li>
<b>Field added. </b>
<code>u16 bugs</code>
</li>
<li>
<b>Field added. </b>
<code>u32 (*dl_read)(struct uart_8250_port *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*dl_write)(struct uart_8250_port *, u32)</code>
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
