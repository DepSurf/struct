# Struct: <code>pl011_dmarx_data</code>

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
struct pl011_dmarx_data {
    struct dma_chan *chan;
    struct completion complete;
    bool use_buf_b;
    struct pl011_sgbuf sgbuf_a;
    struct pl011_sgbuf sgbuf_b;
    dma_cookie_t cookie;
    bool running;
    struct timer_list timer;
    unsigned int last_residue;
    long unsigned int last_jiffies;
    bool auto_poll_rate;
    unsigned int poll_rate;
    unsigned int poll_timeout;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct pl011_dmarx_data {
    struct dma_chan *chan;
    struct completion complete;
    bool use_buf_b;
    struct pl011_sgbuf sgbuf_a;
    struct pl011_sgbuf sgbuf_b;
    dma_cookie_t cookie;
    bool running;
    struct timer_list timer;
    unsigned int last_residue;
    long unsigned int last_jiffies;
    bool auto_poll_rate;
    unsigned int poll_rate;
    unsigned int poll_timeout;
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
