# Struct: <code>dw_pcie</code>

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
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct dw_pcie {
    struct device *dev;
    void *dbi_base;
    void *dbi_base2;
    u32 num_viewport;
    u8 iatu_unroll_enabled;
    struct pcie_port pp;
    struct dw_pcie_ep ep;
    const struct dw_pcie_ops *ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dw_pcie {
    struct device *dev;
    void *dbi_base;
    void *dbi_base2;
    u32 num_viewport;
    u8 iatu_unroll_enabled;
    struct pcie_port pp;
    struct dw_pcie_ep ep;
    const struct dw_pcie_ops *ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dw_pcie {
    struct device *dev;
    void *dbi_base;
    void *dbi_base2;
    u32 num_viewport;
    u8 iatu_unroll_enabled;
    struct pcie_port pp;
    struct dw_pcie_ep ep;
    const struct dw_pcie_ops *ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dw_pcie {
    struct device *dev;
    void *dbi_base;
    void *dbi_base2;
    void *atu_base;
    u32 num_viewport;
    u8 iatu_unroll_enabled;
    struct pcie_port pp;
    struct dw_pcie_ep ep;
    const struct dw_pcie_ops *ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dw_pcie {
    struct device *dev;
    void *dbi_base;
    void *dbi_base2;
    void *atu_base;
    u32 num_viewport;
    u8 iatu_unroll_enabled;
    struct pcie_port pp;
    struct dw_pcie_ep ep;
    const struct dw_pcie_ops *ops;
    unsigned int version;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dw_pcie {
    struct device *dev;
    void *dbi_base;
    void *dbi_base2;
    void *atu_base;
    u32 num_viewport;
    u8 iatu_unroll_enabled;
    struct pcie_port pp;
    struct dw_pcie_ep ep;
    const struct dw_pcie_ops *ops;
    unsigned int version;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dw_pcie {
    struct device *dev;
    void *dbi_base;
    void *dbi_base2;
    void *atu_base;
    u32 num_viewport;
    u8 iatu_unroll_enabled;
    struct pcie_port pp;
    struct dw_pcie_ep ep;
    const struct dw_pcie_ops *ops;
    unsigned int version;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dw_pcie {
    struct device *dev;
    void *dbi_base;
    void *dbi_base2;
    void *atu_base;
    size_t atu_size;
    u32 num_ib_windows;
    u32 num_ob_windows;
    struct pcie_port pp;
    struct dw_pcie_ep ep;
    const struct dw_pcie_ops *ops;
    unsigned int version;
    int num_lanes;
    int link_gen;
    u8 n_fts[2];
    bool iatu_unroll_enabled;
    bool io_cfg_atu_shared;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dw_pcie {
    struct device *dev;
    void *dbi_base;
    void *dbi_base2;
    void *atu_base;
    size_t atu_size;
    u32 num_ib_windows;
    u32 num_ob_windows;
    struct pcie_port pp;
    struct dw_pcie_ep ep;
    const struct dw_pcie_ops *ops;
    unsigned int version;
    int num_lanes;
    int link_gen;
    u8 n_fts[2];
    bool iatu_unroll_enabled;
    bool io_cfg_atu_shared;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dw_pcie {
    struct device *dev;
    void *dbi_base;
    void *dbi_base2;
    void *atu_base;
    size_t atu_size;
    u32 num_ib_windows;
    u32 num_ob_windows;
    struct pcie_port pp;
    struct dw_pcie_ep ep;
    const struct dw_pcie_ops *ops;
    unsigned int version;
    int num_lanes;
    int link_gen;
    u8 n_fts[2];
    bool iatu_unroll_enabled;
    bool io_cfg_atu_shared;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dw_pcie {
    struct device *dev;
    void *dbi_base;
    void *dbi_base2;
    void *atu_base;
    size_t atu_size;
    u32 num_ib_windows;
    u32 num_ob_windows;
    struct pcie_port pp;
    struct dw_pcie_ep ep;
    const struct dw_pcie_ops *ops;
    unsigned int version;
    int num_lanes;
    int link_gen;
    u8 n_fts[2];
    bool iatu_unroll_enabled;
    bool io_cfg_atu_shared;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dw_pcie {
    struct device *dev;
    void *dbi_base;
    void *dbi_base2;
    void *atu_base;
    size_t atu_size;
    u32 num_ib_windows;
    u32 num_ob_windows;
    u32 region_align;
    u64 region_limit;
    struct dw_pcie_rp pp;
    struct dw_pcie_ep ep;
    const struct dw_pcie_ops *ops;
    u32 version;
    u32 type;
    long unsigned int caps;
    int num_lanes;
    int link_gen;
    u8 n_fts[2];
    struct clk_bulk_data app_clks[3];
    struct clk_bulk_data core_clks[4];
    struct reset_control_bulk_data app_rsts[3];
    struct reset_control_bulk_data core_rsts[7];
    struct gpio_desc *pe_rst;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dw_pcie {
    struct device *dev;
    void *dbi_base;
    void *dbi_base2;
    void *atu_base;
    size_t atu_size;
    u32 num_ib_windows;
    u32 num_ob_windows;
    u32 region_align;
    u64 region_limit;
    struct dw_pcie_rp pp;
    struct dw_pcie_ep ep;
    const struct dw_pcie_ops *ops;
    u32 version;
    u32 type;
    long unsigned int caps;
    int num_lanes;
    int link_gen;
    u8 n_fts[2];
    struct dw_edma_chip edma;
    struct clk_bulk_data app_clks[3];
    struct clk_bulk_data core_clks[4];
    struct reset_control_bulk_data app_rsts[3];
    struct reset_control_bulk_data core_rsts[7];
    struct gpio_desc *pe_rst;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dw_pcie {
    struct device *dev;
    void *dbi_base;
    void *dbi_base2;
    void *atu_base;
    size_t atu_size;
    u32 num_ib_windows;
    u32 num_ob_windows;
    u32 region_align;
    u64 region_limit;
    struct dw_pcie_rp pp;
    struct dw_pcie_ep ep;
    const struct dw_pcie_ops *ops;
    u32 version;
    u32 type;
    long unsigned int caps;
    int num_lanes;
    int link_gen;
    u8 n_fts[2];
    struct dw_edma_chip edma;
    struct clk_bulk_data app_clks[3];
    struct clk_bulk_data core_clks[4];
    struct reset_control_bulk_data app_rsts[3];
    struct reset_control_bulk_data core_rsts[7];
    struct gpio_desc *pe_rst;
    bool suspended;
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct dw_pcie {
    struct device *dev;
    void *dbi_base;
    void *dbi_base2;
    void *atu_base;
    u32 num_viewport;
    u8 iatu_unroll_enabled;
    struct pcie_port pp;
    struct dw_pcie_ep ep;
    const struct dw_pcie_ops *ops;
    unsigned int version;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dw_pcie {
    struct device *dev;
    void *dbi_base;
    void *dbi_base2;
    void *atu_base;
    u32 num_viewport;
    u8 iatu_unroll_enabled;
    struct pcie_port pp;
    struct dw_pcie_ep ep;
    const struct dw_pcie_ops *ops;
    unsigned int version;
};
```
</details>
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dw_pcie {
    struct device *dev;
    void *dbi_base;
    void *dbi_base2;
    void *atu_base;
    u32 num_viewport;
    u8 iatu_unroll_enabled;
    struct pcie_port pp;
    struct dw_pcie_ep ep;
    const struct dw_pcie_ops *ops;
    unsigned int version;
};
```
</details>
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct dw_pcie {
    struct device *dev;
    void *dbi_base;
    void *dbi_base2;
    void *atu_base;
    u32 num_viewport;
    u8 iatu_unroll_enabled;
    struct pcie_port pp;
    struct dw_pcie_ep ep;
    const struct dw_pcie_ops *ops;
    unsigned int version;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dw_pcie {
    struct device *dev;
    void *dbi_base;
    void *dbi_base2;
    void *atu_base;
    u32 num_viewport;
    u8 iatu_unroll_enabled;
    struct pcie_port pp;
    struct dw_pcie_ep ep;
    const struct dw_pcie_ops *ops;
    unsigned int version;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dw_pcie {
    struct device *dev;
    void *dbi_base;
    void *dbi_base2;
    void *atu_base;
    u32 num_viewport;
    u8 iatu_unroll_enabled;
    struct pcie_port pp;
    struct dw_pcie_ep ep;
    const struct dw_pcie_ops *ops;
    unsigned int version;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dw_pcie {
    struct device *dev;
    void *dbi_base;
    void *dbi_base2;
    void *atu_base;
    u32 num_viewport;
    u8 iatu_unroll_enabled;
    struct pcie_port pp;
    struct dw_pcie_ep ep;
    const struct dw_pcie_ops *ops;
    unsigned int version;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void *atu_base</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int version</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>size_t atu_size</code>
</li>
<li>
<b>Field added. </b>
<code>u32 num_ib_windows</code>
</li>
<li>
<b>Field added. </b>
<code>u32 num_ob_windows</code>
</li>
<li>
<b>Field added. </b>
<code>int num_lanes</code>
</li>
<li>
<b>Field added. </b>
<code>int link_gen</code>
</li>
<li>
<b>Field added. </b>
<code>u8 n_fts[2]</code>
</li>
<li>
<b>Field added. </b>
<code>bool io_cfg_atu_shared</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 num_viewport</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 iatu_unroll_enabled</code> ➡️ <code>bool iatu_unroll_enabled</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 region_align</code>
</li>
<li>
<b>Field added. </b>
<code>u64 region_limit</code>
</li>
<li>
<b>Field added. </b>
<code>u32 type</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int caps</code>
</li>
<li>
<b>Field added. </b>
<code>struct clk_bulk_data app_clks[3]</code>
</li>
<li>
<b>Field added. </b>
<code>struct clk_bulk_data core_clks[4]</code>
</li>
<li>
<b>Field added. </b>
<code>struct reset_control_bulk_data app_rsts[3]</code>
</li>
<li>
<b>Field added. </b>
<code>struct reset_control_bulk_data core_rsts[7]</code>
</li>
<li>
<b>Field added. </b>
<code>struct gpio_desc *pe_rst</code>
</li>
<li>
<b>Field removed. </b>
<code>bool iatu_unroll_enabled</code>
</li>
<li>
<b>Field removed. </b>
<code>bool io_cfg_atu_shared</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct pcie_port pp</code> ➡️ <code>struct dw_pcie_rp pp</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int version</code> ➡️ <code>u32 version</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct dw_edma_chip edma</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool suspended</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>armhf</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>riscv64</code> ✅
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
No changes between <code>generic</code> and <code>aws</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
