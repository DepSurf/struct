# Struct: <code>fsl_ssi</code>

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
struct fsl_ssi {
    struct regmap *regs;
    int irq;
    struct snd_soc_dai_driver cpu_dai_drv;
    unsigned int dai_fmt;
    u8 streams;
    u8 i2s_net;
    bool synchronous;
    bool use_dma;
    bool use_dual_fifo;
    bool has_ipg_clk_name;
    unsigned int fifo_depth;
    unsigned int slot_width;
    unsigned int slots;
    struct fsl_ssi_regvals regvals[2];
    struct clk *clk;
    struct clk *baudclk;
    unsigned int baudclk_streams;
    u32 regcache_sfcsr;
    u32 regcache_sacnt;
    struct snd_dmaengine_dai_dma_data dma_params_tx;
    struct snd_dmaengine_dai_dma_data dma_params_rx;
    dma_addr_t ssi_phys;
    struct imx_pcm_fiq_params fiq_params;
    struct platform_device *card_pdev;
    char card_name[32];
    u32 card_idx;
    struct fsl_ssi_dbg dbg_stats;
    const struct fsl_ssi_soc_data *soc;
    struct device *dev;
    u32 fifo_watermark;
    u32 dma_maxburst;
    struct mutex ac97_reg_lock;
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
