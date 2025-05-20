# Struct: <code>musb_platform_ops</code>

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
In <code>arm64</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct musb_platform_ops {
    u32 quirks;
    int (*init)(struct musb *);
    int (*exit)(struct musb *);
    void (*enable)(struct musb *);
    void (*disable)(struct musb *);
    u32 (*ep_offset)(u8, u16);
    void (*ep_select)(void *, u8);
    u16 fifo_mode;
    u32 (*fifo_offset)(u8);
    u32 (*busctl_offset)(u8, u16);
    u8 (*readb)(const void *, unsigned int);
    void (*writeb)(void *, unsigned int, u8);
    u16 (*readw)(const void *, unsigned int);
    void (*writew)(void *, unsigned int, u16);
    void (*read_fifo)(struct musb_hw_ep *, u16, u8 *);
    void (*write_fifo)(struct musb_hw_ep *, u16, const u8 *);
    struct dma_controller * (*dma_init)(struct musb *, void *);
    void (*dma_exit)(struct dma_controller *);
    int (*set_mode)(struct musb *, u8);
    void (*try_idle)(struct musb *, long unsigned int);
    int (*recover)(struct musb *);
    int (*vbus_status)(struct musb *);
    void (*set_vbus)(struct musb *, int);
    void (*pre_root_reset_end)(struct musb *);
    void (*post_root_reset_end)(struct musb *);
    int (*phy_callback)(enum musb_vbus_id_status);
    void (*clear_ep_rxintr)(struct musb *, int);
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
