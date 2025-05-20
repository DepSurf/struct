# Struct: <code>uart_amba_port</code>

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
struct uart_amba_port {
    struct uart_port port;
    const u16 *reg_offset;
    struct clk *clk;
    const struct vendor_data *vendor;
    unsigned int dmacr;
    unsigned int im;
    unsigned int old_status;
    unsigned int fifosize;
    unsigned int old_cr;
    unsigned int fixed_baud;
    char type[12];
    bool using_tx_dma;
    bool using_rx_dma;
    struct pl011_dmarx_data dmarx;
    struct pl011_dmatx_data dmatx;
    bool dma_probed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct uart_amba_port {
    struct uart_port port;
    const u16 *reg_offset;
    struct clk *clk;
    const struct vendor_data *vendor;
    unsigned int dmacr;
    unsigned int im;
    unsigned int old_status;
    unsigned int fifosize;
    unsigned int old_cr;
    unsigned int fixed_baud;
    char type[12];
    bool using_tx_dma;
    bool using_rx_dma;
    struct pl011_dmarx_data dmarx;
    struct pl011_dmatx_data dmatx;
    bool dma_probed;
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
