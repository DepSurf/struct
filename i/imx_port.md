# Struct: <code>imx_port</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
In <code>4.8</code>: Absent ⚠️
</li>
<li>
In <code>4.10</code>: Absent ⚠️
</li>
<li>
In <code>4.13</code>: Absent ⚠️
</li>
<li>
In <code>4.15</code>: Absent ⚠️
</li>
<li>
In <code>4.18</code>: Absent ⚠️
</li>
<li>
In <code>5.0</code>: Absent ⚠️
</li>
<li>
In <code>5.3</code>: Absent ⚠️
</li>
<li>
In <code>5.4</code>: Absent ⚠️
</li>
<li>
In <code>5.8</code>: Absent ⚠️
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
In <code>5.19</code>: Absent ⚠️
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct imx_port {
    struct uart_port port;
    struct timer_list timer;
    unsigned int old_status;
    unsigned int have_rtscts;
    unsigned int have_rtsgpio;
    unsigned int dte_mode;
    struct clk *clk_ipg;
    struct clk *clk_per;
    const struct imx_uart_data *devdata;
    struct mctrl_gpios *gpios;
    unsigned int ucr1;
    unsigned int ucr2;
    unsigned int ucr3;
    unsigned int ucr4;
    unsigned int ufcr;
    unsigned int dma_is_enabled;
    unsigned int dma_is_rxing;
    unsigned int dma_is_txing;
    struct dma_chan *dma_chan_rx;
    struct dma_chan *dma_chan_tx;
    struct scatterlist rx_sgl;
    struct scatterlist tx_sgl[2];
    void *rx_buf;
    struct circ_buf rx_ring;
    unsigned int rx_periods;
    dma_cookie_t rx_cookie;
    unsigned int tx_bytes;
    unsigned int dma_tx_nents;
    unsigned int saved_reg[10];
    bool context_saved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct imx_port {
    struct uart_port port;
    struct timer_list timer;
    unsigned int old_status;
    unsigned int have_rtscts;
    unsigned int have_rtsgpio;
    unsigned int dte_mode;
    struct clk *clk_ipg;
    struct clk *clk_per;
    const struct imx_uart_data *devdata;
    struct mctrl_gpios *gpios;
    unsigned int ucr1;
    unsigned int ucr2;
    unsigned int ucr3;
    unsigned int ucr4;
    unsigned int ufcr;
    unsigned int dma_is_enabled;
    unsigned int dma_is_rxing;
    unsigned int dma_is_txing;
    struct dma_chan *dma_chan_rx;
    struct dma_chan *dma_chan_tx;
    struct scatterlist rx_sgl;
    struct scatterlist tx_sgl[2];
    void *rx_buf;
    struct circ_buf rx_ring;
    unsigned int rx_periods;
    dma_cookie_t rx_cookie;
    unsigned int tx_bytes;
    unsigned int dma_tx_nents;
    unsigned int saved_reg[10];
    bool context_saved;
};
```
</details>
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
</li>
<li>
In <code>riscv64</code>: Absent ⚠️
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
In <code>aws</code>: Absent ⚠️
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Arch</b>
<ul>
</ul>
