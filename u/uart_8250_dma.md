# Struct: <code>uart_8250_dma</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct uart_8250_dma {
    int (*tx_dma)(struct uart_8250_port *);
    int (*rx_dma)(struct uart_8250_port *, unsigned int);
    dma_filter_fn fn;
    void *rx_param;
    void *tx_param;
    struct dma_slave_config rxconf;
    struct dma_slave_config txconf;
    struct dma_chan *rxchan;
    struct dma_chan *txchan;
    dma_addr_t rx_addr;
    dma_addr_t tx_addr;
    dma_cookie_t rx_cookie;
    dma_cookie_t tx_cookie;
    void *rx_buf;
    size_t rx_size;
    size_t tx_size;
    unsigned char tx_running;
    unsigned char tx_err;
    unsigned char rx_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct uart_8250_dma {
    int (*tx_dma)(struct uart_8250_port *);
    int (*rx_dma)(struct uart_8250_port *);
    dma_filter_fn fn;
    void *rx_param;
    void *tx_param;
    struct dma_slave_config rxconf;
    struct dma_slave_config txconf;
    struct dma_chan *rxchan;
    struct dma_chan *txchan;
    dma_addr_t rx_addr;
    dma_addr_t tx_addr;
    dma_cookie_t rx_cookie;
    dma_cookie_t tx_cookie;
    void *rx_buf;
    size_t rx_size;
    size_t tx_size;
    unsigned char tx_running;
    unsigned char tx_err;
    unsigned char rx_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct uart_8250_dma {
    int (*tx_dma)(struct uart_8250_port *);
    int (*rx_dma)(struct uart_8250_port *);
    dma_filter_fn fn;
    void *rx_param;
    void *tx_param;
    struct dma_slave_config rxconf;
    struct dma_slave_config txconf;
    struct dma_chan *rxchan;
    struct dma_chan *txchan;
    phys_addr_t rx_dma_addr;
    phys_addr_t tx_dma_addr;
    dma_addr_t rx_addr;
    dma_addr_t tx_addr;
    dma_cookie_t rx_cookie;
    dma_cookie_t tx_cookie;
    void *rx_buf;
    size_t rx_size;
    size_t tx_size;
    unsigned char tx_running;
    unsigned char tx_err;
    unsigned char rx_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct uart_8250_dma {
    int (*tx_dma)(struct uart_8250_port *);
    int (*rx_dma)(struct uart_8250_port *);
    dma_filter_fn fn;
    void *rx_param;
    void *tx_param;
    struct dma_slave_config rxconf;
    struct dma_slave_config txconf;
    struct dma_chan *rxchan;
    struct dma_chan *txchan;
    phys_addr_t rx_dma_addr;
    phys_addr_t tx_dma_addr;
    dma_addr_t rx_addr;
    dma_addr_t tx_addr;
    dma_cookie_t rx_cookie;
    dma_cookie_t tx_cookie;
    void *rx_buf;
    size_t rx_size;
    size_t tx_size;
    unsigned char tx_running;
    unsigned char tx_err;
    unsigned char rx_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct uart_8250_dma {
    int (*tx_dma)(struct uart_8250_port *);
    int (*rx_dma)(struct uart_8250_port *);
    dma_filter_fn fn;
    void *rx_param;
    void *tx_param;
    struct dma_slave_config rxconf;
    struct dma_slave_config txconf;
    struct dma_chan *rxchan;
    struct dma_chan *txchan;
    phys_addr_t rx_dma_addr;
    phys_addr_t tx_dma_addr;
    dma_addr_t rx_addr;
    dma_addr_t tx_addr;
    dma_cookie_t rx_cookie;
    dma_cookie_t tx_cookie;
    void *rx_buf;
    size_t rx_size;
    size_t tx_size;
    unsigned char tx_running;
    unsigned char tx_err;
    unsigned char rx_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct uart_8250_dma {
    int (*tx_dma)(struct uart_8250_port *);
    int (*rx_dma)(struct uart_8250_port *);
    dma_filter_fn fn;
    void *rx_param;
    void *tx_param;
    struct dma_slave_config rxconf;
    struct dma_slave_config txconf;
    struct dma_chan *rxchan;
    struct dma_chan *txchan;
    phys_addr_t rx_dma_addr;
    phys_addr_t tx_dma_addr;
    dma_addr_t rx_addr;
    dma_addr_t tx_addr;
    dma_cookie_t rx_cookie;
    dma_cookie_t tx_cookie;
    void *rx_buf;
    size_t rx_size;
    size_t tx_size;
    unsigned char tx_running;
    unsigned char tx_err;
    unsigned char rx_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct uart_8250_dma {
    int (*tx_dma)(struct uart_8250_port *);
    int (*rx_dma)(struct uart_8250_port *);
    dma_filter_fn fn;
    void *rx_param;
    void *tx_param;
    struct dma_slave_config rxconf;
    struct dma_slave_config txconf;
    struct dma_chan *rxchan;
    struct dma_chan *txchan;
    phys_addr_t rx_dma_addr;
    phys_addr_t tx_dma_addr;
    dma_addr_t rx_addr;
    dma_addr_t tx_addr;
    dma_cookie_t rx_cookie;
    dma_cookie_t tx_cookie;
    void *rx_buf;
    size_t rx_size;
    size_t tx_size;
    unsigned char tx_running;
    unsigned char tx_err;
    unsigned char rx_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct uart_8250_dma {
    int (*tx_dma)(struct uart_8250_port *);
    int (*rx_dma)(struct uart_8250_port *);
    dma_filter_fn fn;
    void *rx_param;
    void *tx_param;
    struct dma_slave_config rxconf;
    struct dma_slave_config txconf;
    struct dma_chan *rxchan;
    struct dma_chan *txchan;
    phys_addr_t rx_dma_addr;
    phys_addr_t tx_dma_addr;
    dma_addr_t rx_addr;
    dma_addr_t tx_addr;
    dma_cookie_t rx_cookie;
    dma_cookie_t tx_cookie;
    void *rx_buf;
    size_t rx_size;
    size_t tx_size;
    unsigned char tx_running;
    unsigned char tx_err;
    unsigned char rx_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct uart_8250_dma {
    int (*tx_dma)(struct uart_8250_port *);
    int (*rx_dma)(struct uart_8250_port *);
    dma_filter_fn fn;
    void *rx_param;
    void *tx_param;
    struct dma_slave_config rxconf;
    struct dma_slave_config txconf;
    struct dma_chan *rxchan;
    struct dma_chan *txchan;
    phys_addr_t rx_dma_addr;
    phys_addr_t tx_dma_addr;
    dma_addr_t rx_addr;
    dma_addr_t tx_addr;
    dma_cookie_t rx_cookie;
    dma_cookie_t tx_cookie;
    void *rx_buf;
    size_t rx_size;
    size_t tx_size;
    unsigned char tx_running;
    unsigned char tx_err;
    unsigned char rx_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct uart_8250_dma {
    int (*tx_dma)(struct uart_8250_port *);
    int (*rx_dma)(struct uart_8250_port *);
    dma_filter_fn fn;
    void *rx_param;
    void *tx_param;
    struct dma_slave_config rxconf;
    struct dma_slave_config txconf;
    struct dma_chan *rxchan;
    struct dma_chan *txchan;
    phys_addr_t rx_dma_addr;
    phys_addr_t tx_dma_addr;
    dma_addr_t rx_addr;
    dma_addr_t tx_addr;
    dma_cookie_t rx_cookie;
    dma_cookie_t tx_cookie;
    void *rx_buf;
    size_t rx_size;
    size_t tx_size;
    unsigned char tx_running;
    unsigned char tx_err;
    unsigned char rx_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct uart_8250_dma {
    int (*tx_dma)(struct uart_8250_port *);
    int (*rx_dma)(struct uart_8250_port *);
    dma_filter_fn fn;
    void *rx_param;
    void *tx_param;
    struct dma_slave_config rxconf;
    struct dma_slave_config txconf;
    struct dma_chan *rxchan;
    struct dma_chan *txchan;
    phys_addr_t rx_dma_addr;
    phys_addr_t tx_dma_addr;
    dma_addr_t rx_addr;
    dma_addr_t tx_addr;
    dma_cookie_t rx_cookie;
    dma_cookie_t tx_cookie;
    void *rx_buf;
    size_t rx_size;
    size_t tx_size;
    unsigned char tx_running;
    unsigned char tx_err;
    unsigned char rx_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct uart_8250_dma {
    int (*tx_dma)(struct uart_8250_port *);
    int (*rx_dma)(struct uart_8250_port *);
    dma_filter_fn fn;
    void *rx_param;
    void *tx_param;
    struct dma_slave_config rxconf;
    struct dma_slave_config txconf;
    struct dma_chan *rxchan;
    struct dma_chan *txchan;
    phys_addr_t rx_dma_addr;
    phys_addr_t tx_dma_addr;
    dma_addr_t rx_addr;
    dma_addr_t tx_addr;
    dma_cookie_t rx_cookie;
    dma_cookie_t tx_cookie;
    void *rx_buf;
    size_t rx_size;
    size_t tx_size;
    unsigned char tx_running;
    unsigned char tx_err;
    unsigned char rx_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct uart_8250_dma {
    int (*tx_dma)(struct uart_8250_port *);
    int (*rx_dma)(struct uart_8250_port *);
    dma_filter_fn fn;
    void *rx_param;
    void *tx_param;
    struct dma_slave_config rxconf;
    struct dma_slave_config txconf;
    struct dma_chan *rxchan;
    struct dma_chan *txchan;
    phys_addr_t rx_dma_addr;
    phys_addr_t tx_dma_addr;
    dma_addr_t rx_addr;
    dma_addr_t tx_addr;
    dma_cookie_t rx_cookie;
    dma_cookie_t tx_cookie;
    void *rx_buf;
    size_t rx_size;
    size_t tx_size;
    unsigned char tx_running;
    unsigned char tx_err;
    unsigned char rx_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct uart_8250_dma {
    int (*tx_dma)(struct uart_8250_port *);
    int (*rx_dma)(struct uart_8250_port *);
    void (*prepare_tx_dma)(struct uart_8250_port *);
    void (*prepare_rx_dma)(struct uart_8250_port *);
    dma_filter_fn fn;
    void *rx_param;
    void *tx_param;
    struct dma_slave_config rxconf;
    struct dma_slave_config txconf;
    struct dma_chan *rxchan;
    struct dma_chan *txchan;
    phys_addr_t rx_dma_addr;
    phys_addr_t tx_dma_addr;
    dma_addr_t rx_addr;
    dma_addr_t tx_addr;
    dma_cookie_t rx_cookie;
    dma_cookie_t tx_cookie;
    void *rx_buf;
    size_t rx_size;
    size_t tx_size;
    unsigned char tx_running;
    unsigned char tx_err;
    unsigned char rx_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct uart_8250_dma {
    int (*tx_dma)(struct uart_8250_port *);
    int (*rx_dma)(struct uart_8250_port *);
    void (*prepare_tx_dma)(struct uart_8250_port *);
    void (*prepare_rx_dma)(struct uart_8250_port *);
    dma_filter_fn fn;
    void *rx_param;
    void *tx_param;
    struct dma_slave_config rxconf;
    struct dma_slave_config txconf;
    struct dma_chan *rxchan;
    struct dma_chan *txchan;
    phys_addr_t rx_dma_addr;
    phys_addr_t tx_dma_addr;
    dma_addr_t rx_addr;
    dma_addr_t tx_addr;
    dma_cookie_t rx_cookie;
    dma_cookie_t tx_cookie;
    void *rx_buf;
    size_t rx_size;
    size_t tx_size;
    unsigned char tx_running;
    unsigned char tx_err;
    unsigned char rx_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct uart_8250_dma {
    int (*tx_dma)(struct uart_8250_port *);
    int (*rx_dma)(struct uart_8250_port *);
    void (*prepare_tx_dma)(struct uart_8250_port *);
    void (*prepare_rx_dma)(struct uart_8250_port *);
    dma_filter_fn fn;
    void *rx_param;
    void *tx_param;
    struct dma_slave_config rxconf;
    struct dma_slave_config txconf;
    struct dma_chan *rxchan;
    struct dma_chan *txchan;
    phys_addr_t rx_dma_addr;
    phys_addr_t tx_dma_addr;
    dma_addr_t rx_addr;
    dma_addr_t tx_addr;
    dma_cookie_t rx_cookie;
    dma_cookie_t tx_cookie;
    void *rx_buf;
    size_t rx_size;
    size_t tx_size;
    unsigned char tx_running;
    unsigned char tx_err;
    unsigned char rx_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct uart_8250_dma {
    int (*tx_dma)(struct uart_8250_port *);
    int (*rx_dma)(struct uart_8250_port *);
    void (*prepare_tx_dma)(struct uart_8250_port *);
    void (*prepare_rx_dma)(struct uart_8250_port *);
    dma_filter_fn fn;
    void *rx_param;
    void *tx_param;
    struct dma_slave_config rxconf;
    struct dma_slave_config txconf;
    struct dma_chan *rxchan;
    struct dma_chan *txchan;
    phys_addr_t rx_dma_addr;
    phys_addr_t tx_dma_addr;
    dma_addr_t rx_addr;
    dma_addr_t tx_addr;
    dma_cookie_t rx_cookie;
    dma_cookie_t tx_cookie;
    void *rx_buf;
    size_t rx_size;
    size_t tx_size;
    unsigned char tx_running;
    unsigned char tx_err;
    unsigned char rx_running;
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
struct uart_8250_dma {
    int (*tx_dma)(struct uart_8250_port *);
    int (*rx_dma)(struct uart_8250_port *);
    dma_filter_fn fn;
    void *rx_param;
    void *tx_param;
    struct dma_slave_config rxconf;
    struct dma_slave_config txconf;
    struct dma_chan *rxchan;
    struct dma_chan *txchan;
    phys_addr_t rx_dma_addr;
    phys_addr_t tx_dma_addr;
    dma_addr_t rx_addr;
    dma_addr_t tx_addr;
    dma_cookie_t rx_cookie;
    dma_cookie_t tx_cookie;
    void *rx_buf;
    size_t rx_size;
    size_t tx_size;
    unsigned char tx_running;
    unsigned char tx_err;
    unsigned char rx_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct uart_8250_dma {
    int (*tx_dma)(struct uart_8250_port *);
    int (*rx_dma)(struct uart_8250_port *);
    dma_filter_fn fn;
    void *rx_param;
    void *tx_param;
    struct dma_slave_config rxconf;
    struct dma_slave_config txconf;
    struct dma_chan *rxchan;
    struct dma_chan *txchan;
    phys_addr_t rx_dma_addr;
    phys_addr_t tx_dma_addr;
    dma_addr_t rx_addr;
    dma_addr_t tx_addr;
    dma_cookie_t rx_cookie;
    dma_cookie_t tx_cookie;
    void *rx_buf;
    size_t rx_size;
    size_t tx_size;
    unsigned char tx_running;
    unsigned char tx_err;
    unsigned char rx_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct uart_8250_dma {
    int (*tx_dma)(struct uart_8250_port *);
    int (*rx_dma)(struct uart_8250_port *);
    dma_filter_fn fn;
    void *rx_param;
    void *tx_param;
    struct dma_slave_config rxconf;
    struct dma_slave_config txconf;
    struct dma_chan *rxchan;
    struct dma_chan *txchan;
    phys_addr_t rx_dma_addr;
    phys_addr_t tx_dma_addr;
    dma_addr_t rx_addr;
    dma_addr_t tx_addr;
    dma_cookie_t rx_cookie;
    dma_cookie_t tx_cookie;
    void *rx_buf;
    size_t rx_size;
    size_t tx_size;
    unsigned char tx_running;
    unsigned char tx_err;
    unsigned char rx_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct uart_8250_dma {
    int (*tx_dma)(struct uart_8250_port *);
    int (*rx_dma)(struct uart_8250_port *);
    dma_filter_fn fn;
    void *rx_param;
    void *tx_param;
    struct dma_slave_config rxconf;
    struct dma_slave_config txconf;
    struct dma_chan *rxchan;
    struct dma_chan *txchan;
    phys_addr_t rx_dma_addr;
    phys_addr_t tx_dma_addr;
    dma_addr_t rx_addr;
    dma_addr_t tx_addr;
    dma_cookie_t rx_cookie;
    dma_cookie_t tx_cookie;
    void *rx_buf;
    size_t rx_size;
    size_t tx_size;
    unsigned char tx_running;
    unsigned char tx_err;
    unsigned char rx_running;
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
struct uart_8250_dma {
    int (*tx_dma)(struct uart_8250_port *);
    int (*rx_dma)(struct uart_8250_port *);
    dma_filter_fn fn;
    void *rx_param;
    void *tx_param;
    struct dma_slave_config rxconf;
    struct dma_slave_config txconf;
    struct dma_chan *rxchan;
    struct dma_chan *txchan;
    phys_addr_t rx_dma_addr;
    phys_addr_t tx_dma_addr;
    dma_addr_t rx_addr;
    dma_addr_t tx_addr;
    dma_cookie_t rx_cookie;
    dma_cookie_t tx_cookie;
    void *rx_buf;
    size_t rx_size;
    size_t tx_size;
    unsigned char tx_running;
    unsigned char tx_err;
    unsigned char rx_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct uart_8250_dma {
    int (*tx_dma)(struct uart_8250_port *);
    int (*rx_dma)(struct uart_8250_port *);
    dma_filter_fn fn;
    void *rx_param;
    void *tx_param;
    struct dma_slave_config rxconf;
    struct dma_slave_config txconf;
    struct dma_chan *rxchan;
    struct dma_chan *txchan;
    phys_addr_t rx_dma_addr;
    phys_addr_t tx_dma_addr;
    dma_addr_t rx_addr;
    dma_addr_t tx_addr;
    dma_cookie_t rx_cookie;
    dma_cookie_t tx_cookie;
    void *rx_buf;
    size_t rx_size;
    size_t tx_size;
    unsigned char tx_running;
    unsigned char tx_err;
    unsigned char rx_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct uart_8250_dma {
    int (*tx_dma)(struct uart_8250_port *);
    int (*rx_dma)(struct uart_8250_port *);
    dma_filter_fn fn;
    void *rx_param;
    void *tx_param;
    struct dma_slave_config rxconf;
    struct dma_slave_config txconf;
    struct dma_chan *rxchan;
    struct dma_chan *txchan;
    phys_addr_t rx_dma_addr;
    phys_addr_t tx_dma_addr;
    dma_addr_t rx_addr;
    dma_addr_t tx_addr;
    dma_cookie_t rx_cookie;
    dma_cookie_t tx_cookie;
    void *rx_buf;
    size_t rx_size;
    size_t tx_size;
    unsigned char tx_running;
    unsigned char tx_err;
    unsigned char rx_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct uart_8250_dma {
    int (*tx_dma)(struct uart_8250_port *);
    int (*rx_dma)(struct uart_8250_port *);
    dma_filter_fn fn;
    void *rx_param;
    void *tx_param;
    struct dma_slave_config rxconf;
    struct dma_slave_config txconf;
    struct dma_chan *rxchan;
    struct dma_chan *txchan;
    phys_addr_t rx_dma_addr;
    phys_addr_t tx_dma_addr;
    dma_addr_t rx_addr;
    dma_addr_t tx_addr;
    dma_cookie_t rx_cookie;
    dma_cookie_t tx_cookie;
    void *rx_buf;
    size_t rx_size;
    size_t tx_size;
    unsigned char tx_running;
    unsigned char tx_err;
    unsigned char rx_running;
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
<code>int (*rx_dma)(struct uart_8250_port *, unsigned int)</code> ➡️ <code>int (*rx_dma)(struct uart_8250_port *)</code>
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
<code>phys_addr_t rx_dma_addr</code>
</li>
<li>
<b>Field added. </b>
<code>phys_addr_t tx_dma_addr</code>
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
<code>void (*prepare_tx_dma)(struct uart_8250_port *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*prepare_rx_dma)(struct uart_8250_port *)</code>
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
