# Struct: <code>dw_edma_chip</code>

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
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dw_edma_chip {
    struct device *dev;
    int nr_irqs;
    const struct dw_edma_plat_ops *ops;
    u32 flags;
    void *reg_base;
    u16 ll_wr_cnt;
    u16 ll_rd_cnt;
    struct dw_edma_region ll_region_wr[8];
    struct dw_edma_region ll_region_rd[8];
    struct dw_edma_region dt_region_wr[8];
    struct dw_edma_region dt_region_rd[8];
    enum dw_edma_map_format mf;
    struct dw_edma *dw;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dw_edma_chip {
    struct device *dev;
    int nr_irqs;
    const struct dw_edma_plat_ops *ops;
    u32 flags;
    void *reg_base;
    u16 ll_wr_cnt;
    u16 ll_rd_cnt;
    struct dw_edma_region ll_region_wr[8];
    struct dw_edma_region ll_region_rd[8];
    struct dw_edma_region dt_region_wr[8];
    struct dw_edma_region dt_region_rd[8];
    enum dw_edma_map_format mf;
    struct dw_edma *dw;
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
In <code>arm64</code>: Absent ⚠️
</li>
<li>
In <code>armhf</code>: Absent ⚠️
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
<b>Regular</b>
<ul>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
