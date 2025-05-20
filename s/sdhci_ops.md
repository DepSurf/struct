# Struct: <code>sdhci_ops</code>

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
struct sdhci_ops {
    u32 (*read_l)(struct sdhci_host *, int);
    u16 (*read_w)(struct sdhci_host *, int);
    u8 (*read_b)(struct sdhci_host *, int);
    void (*write_l)(struct sdhci_host *, u32, int);
    void (*write_w)(struct sdhci_host *, u16, int);
    void (*write_b)(struct sdhci_host *, u8, int);
    void (*set_clock)(struct sdhci_host *, unsigned int);
    void (*set_power)(struct sdhci_host *, unsigned char, short unsigned int);
    u32 (*irq)(struct sdhci_host *, u32);
    int (*set_dma_mask)(struct sdhci_host *);
    int (*enable_dma)(struct sdhci_host *);
    unsigned int (*get_max_clock)(struct sdhci_host *);
    unsigned int (*get_min_clock)(struct sdhci_host *);
    unsigned int (*get_timeout_clock)(struct sdhci_host *);
    unsigned int (*get_max_timeout_count)(struct sdhci_host *);
    void (*set_timeout)(struct sdhci_host *, struct mmc_command *);
    void (*set_bus_width)(struct sdhci_host *, int);
    void (*platform_send_init_74_clocks)(struct sdhci_host *, u8);
    unsigned int (*get_ro)(struct sdhci_host *);
    void (*reset)(struct sdhci_host *, u8);
    int (*platform_execute_tuning)(struct sdhci_host *, u32);
    void (*set_uhs_signaling)(struct sdhci_host *, unsigned int);
    void (*hw_reset)(struct sdhci_host *);
    void (*adma_workaround)(struct sdhci_host *, u32);
    void (*card_event)(struct sdhci_host *);
    void (*voltage_switch)(struct sdhci_host *);
    void (*adma_write_desc)(struct sdhci_host *, void **, dma_addr_t, int, unsigned int);
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
