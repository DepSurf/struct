# Struct: <code>variant_data</code>

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
struct variant_data {
    unsigned int clkreg;
    unsigned int clkreg_enable;
    unsigned int clkreg_8bit_bus_enable;
    unsigned int clkreg_neg_edge_enable;
    unsigned int cmdreg_cpsm_enable;
    unsigned int cmdreg_lrsp_crc;
    unsigned int cmdreg_srsp_crc;
    unsigned int cmdreg_srsp;
    unsigned int cmdreg_stop;
    unsigned int datalength_bits;
    unsigned int fifosize;
    unsigned int fifohalfsize;
    unsigned int data_cmd_enable;
    unsigned int datactrl_mask_ddrmode;
    unsigned int datactrl_mask_sdio;
    unsigned int datactrl_blocksz;
    u8 datactrl_first;
    u8 datacnt_useless;
    u8 st_sdio;
    u8 st_clkdiv;
    u8 stm32_clkdiv;
    u32 pwrreg_powerup;
    u32 f_max;
    u8 signal_direction;
    u8 pwrreg_clkgate;
    u8 busy_detect;
    u32 busy_dpsm_flag;
    u32 busy_detect_flag;
    u32 busy_detect_mask;
    u8 pwrreg_nopower;
    u8 explicit_mclk_control;
    u8 qcom_fifo;
    u8 qcom_dml;
    u8 reversed_irq_handling;
    u8 mmcimask1;
    unsigned int irq_pio_mask;
    u32 start_err;
    u32 opendrain;
    u8 dma_lli;
    u32 stm32_idmabsize_mask;
    void (*init)(struct mmci_host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct variant_data {
    unsigned int clkreg;
    unsigned int clkreg_enable;
    unsigned int clkreg_8bit_bus_enable;
    unsigned int clkreg_neg_edge_enable;
    unsigned int cmdreg_cpsm_enable;
    unsigned int cmdreg_lrsp_crc;
    unsigned int cmdreg_srsp_crc;
    unsigned int cmdreg_srsp;
    unsigned int cmdreg_stop;
    unsigned int datalength_bits;
    unsigned int fifosize;
    unsigned int fifohalfsize;
    unsigned int data_cmd_enable;
    unsigned int datactrl_mask_ddrmode;
    unsigned int datactrl_mask_sdio;
    unsigned int datactrl_blocksz;
    u8 datactrl_first;
    u8 datacnt_useless;
    u8 st_sdio;
    u8 st_clkdiv;
    u8 stm32_clkdiv;
    u32 pwrreg_powerup;
    u32 f_max;
    u8 signal_direction;
    u8 pwrreg_clkgate;
    u8 busy_detect;
    u32 busy_dpsm_flag;
    u32 busy_detect_flag;
    u32 busy_detect_mask;
    u8 pwrreg_nopower;
    u8 explicit_mclk_control;
    u8 qcom_fifo;
    u8 qcom_dml;
    u8 reversed_irq_handling;
    u8 mmcimask1;
    unsigned int irq_pio_mask;
    u32 start_err;
    u32 opendrain;
    u8 dma_lli;
    u32 stm32_idmabsize_mask;
    void (*init)(struct mmci_host *);
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
