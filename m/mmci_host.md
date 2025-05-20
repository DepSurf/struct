# Struct: <code>mmci_host</code>

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
struct mmci_host {
    phys_addr_t phybase;
    void *base;
    struct mmc_request *mrq;
    struct mmc_command *cmd;
    struct mmc_command stop_abort;
    struct mmc_data *data;
    struct mmc_host *mmc;
    struct clk *clk;
    u8 singleirq;
    struct reset_control *rst;
    spinlock_t lock;
    unsigned int mclk;
    unsigned int clock_cache;
    unsigned int cclk;
    u32 pwr_reg;
    u32 pwr_reg_add;
    u32 clk_reg;
    u32 clk_reg_add;
    u32 datactrl_reg;
    u32 busy_status;
    u32 mask1_reg;
    u8 vqmmc_enabled;
    struct mmci_platform_data *plat;
    struct mmci_host_ops *ops;
    struct variant_data *variant;
    struct pinctrl *pinctrl;
    struct pinctrl_state *pins_default;
    struct pinctrl_state *pins_opendrain;
    u8 hw_designer;
    u8 hw_revision;
    struct timer_list timer;
    unsigned int oldstat;
    struct sg_mapping_iter sg_miter;
    unsigned int size;
    int (*get_rx_fifocnt)(struct mmci_host *, u32, int);
    u8 use_dma;
    u8 dma_in_progress;
    void *dma_priv;
    s32 next_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mmci_host {
    phys_addr_t phybase;
    void *base;
    struct mmc_request *mrq;
    struct mmc_command *cmd;
    struct mmc_command stop_abort;
    struct mmc_data *data;
    struct mmc_host *mmc;
    struct clk *clk;
    u8 singleirq;
    struct reset_control *rst;
    spinlock_t lock;
    unsigned int mclk;
    unsigned int clock_cache;
    unsigned int cclk;
    u32 pwr_reg;
    u32 pwr_reg_add;
    u32 clk_reg;
    u32 clk_reg_add;
    u32 datactrl_reg;
    u32 busy_status;
    u32 mask1_reg;
    u8 vqmmc_enabled;
    struct mmci_platform_data *plat;
    struct mmci_host_ops *ops;
    struct variant_data *variant;
    struct pinctrl *pinctrl;
    struct pinctrl_state *pins_default;
    struct pinctrl_state *pins_opendrain;
    u8 hw_designer;
    u8 hw_revision;
    struct timer_list timer;
    unsigned int oldstat;
    struct sg_mapping_iter sg_miter;
    unsigned int size;
    int (*get_rx_fifocnt)(struct mmci_host *, u32, int);
    u8 use_dma;
    u8 dma_in_progress;
    void *dma_priv;
    s32 next_cookie;
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
