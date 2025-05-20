# Struct: <code>pmc_dev</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct pmc_dev {
    u32 base_addr;
    void *regmap;
    const struct pmc_reg_map *map;
    struct dentry *dbgfs_dir;
    bool init;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct pmc_dev {
    u32 base_addr;
    void *regmap;
    const struct pmc_reg_map *map;
    struct dentry *dbgfs_dir;
    bool init;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct pmc_dev {
    u32 base_addr;
    void *regmap;
    const struct pmc_reg_map *map;
    struct dentry *dbgfs_dir;
    bool init;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct pmc_dev {
    u32 base_addr;
    void *regbase;
    const struct pmc_reg_map *map;
    struct dentry *dbgfs_dir;
    bool has_slp_s0_res;
    int pmc_xram_read_bit;
    struct mutex lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct pmc_dev {
    u32 base_addr;
    void *regbase;
    const struct pmc_reg_map *map;
    struct dentry *dbgfs_dir;
    int pmc_xram_read_bit;
    struct mutex lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct pmc_dev {
    u32 base_addr;
    void *regbase;
    const struct pmc_reg_map *map;
    struct dentry *dbgfs_dir;
    int pmc_xram_read_bit;
    struct mutex lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct pmc_dev {
    u32 base_addr;
    void *regbase;
    const struct pmc_reg_map *map;
    struct dentry *dbgfs_dir;
    int pmc_xram_read_bit;
    struct mutex lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct pmc_dev {
    u32 base_addr;
    void *regbase;
    const struct pmc_reg_map *map;
    struct dentry *dbgfs_dir;
    int pmc_xram_read_bit;
    struct mutex lock;
    bool check_counters;
    u64 pc10_counter;
    u64 s0ix_counter;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct pmc_dev {
    u32 base_addr;
    void *regbase;
    const struct pmc_reg_map *map;
    struct dentry *dbgfs_dir;
    int pmc_xram_read_bit;
    struct mutex lock;
    bool check_counters;
    u64 pc10_counter;
    u64 s0ix_counter;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct pmc_dev {
    u32 base_addr;
    void *regbase;
    const struct pmc_reg_map *map;
    struct dentry *dbgfs_dir;
    int pmc_xram_read_bit;
    struct mutex lock;
    bool check_counters;
    u64 pc10_counter;
    u64 s0ix_counter;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct pmc_dev {
    u32 base_addr;
    void *regbase;
    const struct pmc_reg_map *map;
    struct dentry *dbgfs_dir;
    int pmc_xram_read_bit;
    struct mutex lock;
    bool check_counters;
    u64 pc10_counter;
    u64 s0ix_counter;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct pmc_dev {
    u32 base_addr;
    void *regbase;
    const struct pmc_reg_map *map;
    struct dentry *dbgfs_dir;
    int pmc_xram_read_bit;
    struct mutex lock;
    bool check_counters;
    u64 pc10_counter;
    u64 s0ix_counter;
    int num_lpm_modes;
    int lpm_en_modes[8];
    u32 *lpm_req_regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct pmc_dev {
    u32 base_addr;
    void *regbase;
    const struct pmc_reg_map *map;
    struct dentry *dbgfs_dir;
    int pmc_xram_read_bit;
    struct mutex lock;
    bool check_counters;
    u64 pc10_counter;
    u64 s0ix_counter;
    int num_lpm_modes;
    int lpm_en_modes[8];
    u32 *lpm_req_regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct pmc_dev {
    u32 base_addr;
    void *regbase;
    const struct pmc_reg_map *map;
    struct dentry *dbgfs_dir;
    int pmc_xram_read_bit;
    struct mutex lock;
    bool check_counters;
    u64 pc10_counter;
    u64 s0ix_counter;
    int num_lpm_modes;
    int lpm_en_modes[8];
    u32 *lpm_req_regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct pmc_dev {
    u32 base_addr;
    void *regbase;
    const struct pmc_reg_map *map;
    struct dentry *dbgfs_dir;
    struct platform_device *pdev;
    int pmc_xram_read_bit;
    struct mutex lock;
    bool check_counters;
    u64 pc10_counter;
    u64 s0ix_counter;
    int num_lpm_modes;
    int lpm_en_modes[8];
    u32 *lpm_req_regs;
    void (*core_configure)(struct pmc_dev *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct pmc_dev {
    struct pmc * pmcs[3];
    struct dentry *dbgfs_dir;
    struct platform_device *pdev;
    struct pci_dev *ssram_pcidev;
    int pmc_xram_read_bit;
    struct mutex lock;
    u64 pc10_counter;
    u64 s0ix_counter;
    int num_lpm_modes;
    int lpm_en_modes[8];
    int (*resume)(struct pmc_dev *);
    bool has_die_c6;
    u32 die_c6_offset;
    struct telem_endpoint *punit_ep;
    struct pmc_info *regmap_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct pmc_dev {
    u32 base_addr;
    void *regmap;
    const struct pmc_reg_map *map;
    struct dentry *dbgfs_dir;
    bool init;
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct pmc_dev {
    u32 base_addr;
    void *regbase;
    const struct pmc_reg_map *map;
    struct dentry *dbgfs_dir;
    int pmc_xram_read_bit;
    struct mutex lock;
    bool check_counters;
    u64 pc10_counter;
    u64 s0ix_counter;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct pmc_dev {
    u32 base_addr;
    void *regbase;
    const struct pmc_reg_map *map;
    struct dentry *dbgfs_dir;
    int pmc_xram_read_bit;
    struct mutex lock;
    bool check_counters;
    u64 pc10_counter;
    u64 s0ix_counter;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct pmc_dev {
    u32 base_addr;
    void *regbase;
    const struct pmc_reg_map *map;
    struct dentry *dbgfs_dir;
    int pmc_xram_read_bit;
    struct mutex lock;
    bool check_counters;
    u64 pc10_counter;
    u64 s0ix_counter;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct pmc_dev {
    u32 base_addr;
    void *regbase;
    const struct pmc_reg_map *map;
    struct dentry *dbgfs_dir;
    int pmc_xram_read_bit;
    struct mutex lock;
    bool check_counters;
    u64 pc10_counter;
    u64 s0ix_counter;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.4</code> and <code>4.8</code> ✅
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void *regbase</code>
</li>
<li>
<b>Field added. </b>
<code>bool has_slp_s0_res</code>
</li>
<li>
<b>Field added. </b>
<code>int pmc_xram_read_bit</code>
</li>
<li>
<b>Field added. </b>
<code>struct mutex lock</code>
</li>
<li>
<b>Field removed. </b>
<code>void *regmap</code>
</li>
<li>
<b>Field removed. </b>
<code>bool init</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>bool has_slp_s0_res</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool check_counters</code>
</li>
<li>
<b>Field added. </b>
<code>u64 pc10_counter</code>
</li>
<li>
<b>Field added. </b>
<code>u64 s0ix_counter</code>
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
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int num_lpm_modes</code>
</li>
<li>
<b>Field added. </b>
<code>int lpm_en_modes[8]</code>
</li>
<li>
<b>Field added. </b>
<code>u32 *lpm_req_regs</code>
</li>
</ul>
</details>
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
<code>struct platform_device *pdev</code>
</li>
<li>
<b>Field added. </b>
<code>void (*core_configure)(struct pmc_dev *)</code>
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
<code>struct pmc * pmcs[3]</code>
</li>
<li>
<b>Field added. </b>
<code>struct pci_dev *ssram_pcidev</code>
</li>
<li>
<b>Field added. </b>
<code>int (*resume)(struct pmc_dev *)</code>
</li>
<li>
<b>Field added. </b>
<code>bool has_die_c6</code>
</li>
<li>
<b>Field added. </b>
<code>u32 die_c6_offset</code>
</li>
<li>
<b>Field added. </b>
<code>struct telem_endpoint *punit_ep</code>
</li>
<li>
<b>Field added. </b>
<code>struct pmc_info *regmap_list</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 base_addr</code>
</li>
<li>
<b>Field removed. </b>
<code>void *regbase</code>
</li>
<li>
<b>Field removed. </b>
<code>const struct pmc_reg_map *map</code>
</li>
<li>
<b>Field removed. </b>
<code>bool check_counters</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 *lpm_req_regs</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*core_configure)(struct pmc_dev *)</code>
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
<code>u32 base_addr</code>
</li>
<li>
<b>Field added. </b>
<code>void *regmap</code>
</li>
<li>
<b>Field added. </b>
<code>const struct pmc_reg_map *map</code>
</li>
<li>
<b>Field added. </b>
<code>bool init</code>
</li>
<li>
<b>Field removed. </b>
<code>struct pmc * pmcs[3]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct platform_device *pdev</code>
</li>
<li>
<b>Field removed. </b>
<code>struct pci_dev *ssram_pcidev</code>
</li>
<li>
<b>Field removed. </b>
<code>int pmc_xram_read_bit</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mutex lock</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 pc10_counter</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 s0ix_counter</code>
</li>
<li>
<b>Field removed. </b>
<code>int num_lpm_modes</code>
</li>
<li>
<b>Field removed. </b>
<code>int lpm_en_modes[8]</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*resume)(struct pmc_dev *)</code>
</li>
<li>
<b>Field removed. </b>
<code>bool has_die_c6</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 die_c6_offset</code>
</li>
<li>
<b>Field removed. </b>
<code>struct telem_endpoint *punit_ep</code>
</li>
<li>
<b>Field removed. </b>
<code>struct pmc_info *regmap_list</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Arch</b>
<ul>
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
