# Struct: <code>mmci_host_ops</code>

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
struct mmci_host_ops {
    int (*validate_data)(struct mmci_host *, struct mmc_data *);
    int (*prep_data)(struct mmci_host *, struct mmc_data *, bool);
    void (*unprep_data)(struct mmci_host *, struct mmc_data *, int);
    u32 (*get_datactrl_cfg)(struct mmci_host *);
    void (*get_next_data)(struct mmci_host *, struct mmc_data *);
    int (*dma_setup)(struct mmci_host *);
    void (*dma_release)(struct mmci_host *);
    int (*dma_start)(struct mmci_host *, unsigned int *);
    void (*dma_finalize)(struct mmci_host *, struct mmc_data *);
    void (*dma_error)(struct mmci_host *);
    void (*set_clkreg)(struct mmci_host *, unsigned int);
    void (*set_pwrreg)(struct mmci_host *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mmci_host_ops {
    int (*validate_data)(struct mmci_host *, struct mmc_data *);
    int (*prep_data)(struct mmci_host *, struct mmc_data *, bool);
    void (*unprep_data)(struct mmci_host *, struct mmc_data *, int);
    u32 (*get_datactrl_cfg)(struct mmci_host *);
    void (*get_next_data)(struct mmci_host *, struct mmc_data *);
    int (*dma_setup)(struct mmci_host *);
    void (*dma_release)(struct mmci_host *);
    int (*dma_start)(struct mmci_host *, unsigned int *);
    void (*dma_finalize)(struct mmci_host *, struct mmc_data *);
    void (*dma_error)(struct mmci_host *);
    void (*set_clkreg)(struct mmci_host *, unsigned int);
    void (*set_pwrreg)(struct mmci_host *, unsigned int);
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
