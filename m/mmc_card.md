# Struct: <code>mmc_card</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct mmc_card {
    struct mmc_host *host;
    struct device dev;
    u32 ocr;
    unsigned int rca;
    unsigned int type;
    unsigned int state;
    unsigned int quirks;
    unsigned int erase_size;
    unsigned int erase_shift;
    unsigned int pref_erase;
    unsigned int eg_boundary;
    u8 erased_byte;
    u32 raw_cid[4];
    u32 raw_csd[4];
    u32 raw_scr[2];
    struct mmc_cid cid;
    struct mmc_csd csd;
    struct mmc_ext_csd ext_csd;
    struct sd_scr scr;
    struct sd_ssr ssr;
    struct sd_switch_caps sw_caps;
    unsigned int sdio_funcs;
    struct sdio_cccr cccr;
    struct sdio_cis cis;
    struct sdio_func * sdio_func[7];
    struct sdio_func *sdio_single_irq;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
    unsigned int sd_bus_speed;
    unsigned int mmc_avail_type;
    unsigned int drive_strength;
    struct dentry *debugfs_root;
    struct mmc_part part[7];
    unsigned int nr_parts;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct mmc_card {
    struct mmc_host *host;
    struct device dev;
    u32 ocr;
    unsigned int rca;
    unsigned int type;
    unsigned int state;
    unsigned int quirks;
    unsigned int erase_size;
    unsigned int erase_shift;
    unsigned int pref_erase;
    unsigned int eg_boundary;
    u8 erased_byte;
    u32 raw_cid[4];
    u32 raw_csd[4];
    u32 raw_scr[2];
    struct mmc_cid cid;
    struct mmc_csd csd;
    struct mmc_ext_csd ext_csd;
    struct sd_scr scr;
    struct sd_ssr ssr;
    struct sd_switch_caps sw_caps;
    unsigned int sdio_funcs;
    struct sdio_cccr cccr;
    struct sdio_cis cis;
    struct sdio_func * sdio_func[7];
    struct sdio_func *sdio_single_irq;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
    unsigned int sd_bus_speed;
    unsigned int mmc_avail_type;
    unsigned int drive_strength;
    struct dentry *debugfs_root;
    struct mmc_part part[7];
    unsigned int nr_parts;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct mmc_card {
    struct mmc_host *host;
    struct device dev;
    u32 ocr;
    unsigned int rca;
    unsigned int type;
    unsigned int state;
    unsigned int quirks;
    unsigned int erase_size;
    unsigned int erase_shift;
    unsigned int pref_erase;
    unsigned int eg_boundary;
    u8 erased_byte;
    u32 raw_cid[4];
    u32 raw_csd[4];
    u32 raw_scr[2];
    u32 raw_ssr[16];
    struct mmc_cid cid;
    struct mmc_csd csd;
    struct mmc_ext_csd ext_csd;
    struct sd_scr scr;
    struct sd_ssr ssr;
    struct sd_switch_caps sw_caps;
    unsigned int sdio_funcs;
    struct sdio_cccr cccr;
    struct sdio_cis cis;
    struct sdio_func * sdio_func[7];
    struct sdio_func *sdio_single_irq;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
    unsigned int sd_bus_speed;
    unsigned int mmc_avail_type;
    unsigned int drive_strength;
    struct dentry *debugfs_root;
    struct mmc_part part[7];
    unsigned int nr_parts;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct mmc_card {
    struct mmc_host *host;
    struct device dev;
    u32 ocr;
    unsigned int rca;
    unsigned int type;
    unsigned int state;
    unsigned int quirks;
    bool reenable_cmdq;
    unsigned int erase_size;
    unsigned int erase_shift;
    unsigned int pref_erase;
    unsigned int eg_boundary;
    u8 erased_byte;
    u32 raw_cid[4];
    u32 raw_csd[4];
    u32 raw_scr[2];
    u32 raw_ssr[16];
    struct mmc_cid cid;
    struct mmc_csd csd;
    struct mmc_ext_csd ext_csd;
    struct sd_scr scr;
    struct sd_ssr ssr;
    struct sd_switch_caps sw_caps;
    unsigned int sdio_funcs;
    struct sdio_cccr cccr;
    struct sdio_cis cis;
    struct sdio_func * sdio_func[7];
    struct sdio_func *sdio_single_irq;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
    unsigned int sd_bus_speed;
    unsigned int mmc_avail_type;
    unsigned int drive_strength;
    struct dentry *debugfs_root;
    struct mmc_part part[7];
    unsigned int nr_parts;
    unsigned int bouncesz;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct mmc_card {
    struct mmc_host *host;
    struct device dev;
    u32 ocr;
    unsigned int rca;
    unsigned int type;
    unsigned int state;
    unsigned int quirks;
    bool reenable_cmdq;
    unsigned int erase_size;
    unsigned int erase_shift;
    unsigned int pref_erase;
    unsigned int eg_boundary;
    u8 erased_byte;
    u32 raw_cid[4];
    u32 raw_csd[4];
    u32 raw_scr[2];
    u32 raw_ssr[16];
    struct mmc_cid cid;
    struct mmc_csd csd;
    struct mmc_ext_csd ext_csd;
    struct sd_scr scr;
    struct sd_ssr ssr;
    struct sd_switch_caps sw_caps;
    unsigned int sdio_funcs;
    struct sdio_cccr cccr;
    struct sdio_cis cis;
    struct sdio_func * sdio_func[7];
    struct sdio_func *sdio_single_irq;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
    unsigned int sd_bus_speed;
    unsigned int mmc_avail_type;
    unsigned int drive_strength;
    struct dentry *debugfs_root;
    struct mmc_part part[7];
    unsigned int nr_parts;
    unsigned int bouncesz;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct mmc_card {
    struct mmc_host *host;
    struct device dev;
    u32 ocr;
    unsigned int rca;
    unsigned int type;
    unsigned int state;
    unsigned int quirks;
    unsigned int quirk_max_rate;
    bool reenable_cmdq;
    unsigned int erase_size;
    unsigned int erase_shift;
    unsigned int pref_erase;
    unsigned int eg_boundary;
    u8 erased_byte;
    u32 raw_cid[4];
    u32 raw_csd[4];
    u32 raw_scr[2];
    u32 raw_ssr[16];
    struct mmc_cid cid;
    struct mmc_csd csd;
    struct mmc_ext_csd ext_csd;
    struct sd_scr scr;
    struct sd_ssr ssr;
    struct sd_switch_caps sw_caps;
    unsigned int sdio_funcs;
    struct sdio_cccr cccr;
    struct sdio_cis cis;
    struct sdio_func * sdio_func[7];
    struct sdio_func *sdio_single_irq;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
    unsigned int sd_bus_speed;
    unsigned int mmc_avail_type;
    unsigned int drive_strength;
    struct dentry *debugfs_root;
    struct mmc_part part[7];
    unsigned int nr_parts;
    unsigned int bouncesz;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct mmc_card {
    struct mmc_host *host;
    struct device dev;
    u32 ocr;
    unsigned int rca;
    unsigned int type;
    unsigned int state;
    unsigned int quirks;
    unsigned int quirk_max_rate;
    bool reenable_cmdq;
    unsigned int erase_size;
    unsigned int erase_shift;
    unsigned int pref_erase;
    unsigned int eg_boundary;
    u8 erased_byte;
    u32 raw_cid[4];
    u32 raw_csd[4];
    u32 raw_scr[2];
    u32 raw_ssr[16];
    struct mmc_cid cid;
    struct mmc_csd csd;
    struct mmc_ext_csd ext_csd;
    struct sd_scr scr;
    struct sd_ssr ssr;
    struct sd_switch_caps sw_caps;
    unsigned int sdio_funcs;
    struct sdio_cccr cccr;
    struct sdio_cis cis;
    struct sdio_func * sdio_func[7];
    struct sdio_func *sdio_single_irq;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
    unsigned int sd_bus_speed;
    unsigned int mmc_avail_type;
    unsigned int drive_strength;
    struct dentry *debugfs_root;
    struct mmc_part part[7];
    unsigned int nr_parts;
    unsigned int bouncesz;
    struct workqueue_struct *complete_wq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct mmc_card {
    struct mmc_host *host;
    struct device dev;
    u32 ocr;
    unsigned int rca;
    unsigned int type;
    unsigned int state;
    unsigned int quirks;
    unsigned int quirk_max_rate;
    bool reenable_cmdq;
    unsigned int erase_size;
    unsigned int erase_shift;
    unsigned int pref_erase;
    unsigned int eg_boundary;
    unsigned int erase_arg;
    u8 erased_byte;
    u32 raw_cid[4];
    u32 raw_csd[4];
    u32 raw_scr[2];
    u32 raw_ssr[16];
    struct mmc_cid cid;
    struct mmc_csd csd;
    struct mmc_ext_csd ext_csd;
    struct sd_scr scr;
    struct sd_ssr ssr;
    struct sd_switch_caps sw_caps;
    unsigned int sdio_funcs;
    struct sdio_cccr cccr;
    struct sdio_cis cis;
    struct sdio_func * sdio_func[7];
    struct sdio_func *sdio_single_irq;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
    unsigned int sd_bus_speed;
    unsigned int mmc_avail_type;
    unsigned int drive_strength;
    struct dentry *debugfs_root;
    struct mmc_part part[7];
    unsigned int nr_parts;
    unsigned int bouncesz;
    struct workqueue_struct *complete_wq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct mmc_card {
    struct mmc_host *host;
    struct device dev;
    u32 ocr;
    unsigned int rca;
    unsigned int type;
    unsigned int state;
    unsigned int quirks;
    unsigned int quirk_max_rate;
    bool reenable_cmdq;
    unsigned int erase_size;
    unsigned int erase_shift;
    unsigned int pref_erase;
    unsigned int eg_boundary;
    unsigned int erase_arg;
    u8 erased_byte;
    u32 raw_cid[4];
    u32 raw_csd[4];
    u32 raw_scr[2];
    u32 raw_ssr[16];
    struct mmc_cid cid;
    struct mmc_csd csd;
    struct mmc_ext_csd ext_csd;
    struct sd_scr scr;
    struct sd_ssr ssr;
    struct sd_switch_caps sw_caps;
    unsigned int sdio_funcs;
    atomic_t sdio_funcs_probed;
    struct sdio_cccr cccr;
    struct sdio_cis cis;
    struct sdio_func * sdio_func[7];
    struct sdio_func *sdio_single_irq;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
    unsigned int sd_bus_speed;
    unsigned int mmc_avail_type;
    unsigned int drive_strength;
    struct dentry *debugfs_root;
    struct mmc_part part[7];
    unsigned int nr_parts;
    unsigned int bouncesz;
    struct workqueue_struct *complete_wq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct mmc_card {
    struct mmc_host *host;
    struct device dev;
    u32 ocr;
    unsigned int rca;
    unsigned int type;
    unsigned int state;
    unsigned int quirks;
    unsigned int quirk_max_rate;
    bool reenable_cmdq;
    unsigned int erase_size;
    unsigned int erase_shift;
    unsigned int pref_erase;
    unsigned int eg_boundary;
    unsigned int erase_arg;
    u8 erased_byte;
    u32 raw_cid[4];
    u32 raw_csd[4];
    u32 raw_scr[2];
    u32 raw_ssr[16];
    struct mmc_cid cid;
    struct mmc_csd csd;
    struct mmc_ext_csd ext_csd;
    struct sd_scr scr;
    struct sd_ssr ssr;
    struct sd_switch_caps sw_caps;
    unsigned int sdio_funcs;
    atomic_t sdio_funcs_probed;
    struct sdio_cccr cccr;
    struct sdio_cis cis;
    struct sdio_func * sdio_func[7];
    struct sdio_func *sdio_single_irq;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
    unsigned int sd_bus_speed;
    unsigned int mmc_avail_type;
    unsigned int drive_strength;
    struct dentry *debugfs_root;
    struct mmc_part part[7];
    unsigned int nr_parts;
    unsigned int bouncesz;
    struct workqueue_struct *complete_wq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mmc_card {
    struct mmc_host *host;
    struct device dev;
    u32 ocr;
    unsigned int rca;
    unsigned int type;
    unsigned int state;
    unsigned int quirks;
    unsigned int quirk_max_rate;
    bool reenable_cmdq;
    unsigned int erase_size;
    unsigned int erase_shift;
    unsigned int pref_erase;
    unsigned int eg_boundary;
    unsigned int erase_arg;
    u8 erased_byte;
    u32 raw_cid[4];
    u32 raw_csd[4];
    u32 raw_scr[2];
    u32 raw_ssr[16];
    struct mmc_cid cid;
    struct mmc_csd csd;
    struct mmc_ext_csd ext_csd;
    struct sd_scr scr;
    struct sd_ssr ssr;
    struct sd_switch_caps sw_caps;
    unsigned int sdio_funcs;
    atomic_t sdio_funcs_probed;
    struct sdio_cccr cccr;
    struct sdio_cis cis;
    struct sdio_func * sdio_func[7];
    struct sdio_func *sdio_single_irq;
    u8 major_rev;
    u8 minor_rev;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
    unsigned int sd_bus_speed;
    unsigned int mmc_avail_type;
    unsigned int drive_strength;
    struct dentry *debugfs_root;
    struct mmc_part part[7];
    unsigned int nr_parts;
    unsigned int bouncesz;
    struct workqueue_struct *complete_wq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mmc_card {
    struct mmc_host *host;
    struct device dev;
    u32 ocr;
    unsigned int rca;
    unsigned int type;
    unsigned int state;
    unsigned int quirks;
    unsigned int quirk_max_rate;
    bool reenable_cmdq;
    unsigned int erase_size;
    unsigned int erase_shift;
    unsigned int pref_erase;
    unsigned int eg_boundary;
    unsigned int erase_arg;
    u8 erased_byte;
    u32 raw_cid[4];
    u32 raw_csd[4];
    u32 raw_scr[2];
    u32 raw_ssr[16];
    struct mmc_cid cid;
    struct mmc_csd csd;
    struct mmc_ext_csd ext_csd;
    struct sd_scr scr;
    struct sd_ssr ssr;
    struct sd_switch_caps sw_caps;
    unsigned int sdio_funcs;
    atomic_t sdio_funcs_probed;
    struct sdio_cccr cccr;
    struct sdio_cis cis;
    struct sdio_func * sdio_func[7];
    struct sdio_func *sdio_single_irq;
    u8 major_rev;
    u8 minor_rev;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
    unsigned int sd_bus_speed;
    unsigned int mmc_avail_type;
    unsigned int drive_strength;
    struct dentry *debugfs_root;
    struct mmc_part part[7];
    unsigned int nr_parts;
    struct workqueue_struct *complete_wq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mmc_card {
    struct mmc_host *host;
    struct device dev;
    u32 ocr;
    unsigned int rca;
    unsigned int type;
    unsigned int state;
    unsigned int quirks;
    unsigned int quirk_max_rate;
    bool reenable_cmdq;
    unsigned int erase_size;
    unsigned int erase_shift;
    unsigned int pref_erase;
    unsigned int eg_boundary;
    unsigned int erase_arg;
    u8 erased_byte;
    u32 raw_cid[4];
    u32 raw_csd[4];
    u32 raw_scr[2];
    u32 raw_ssr[16];
    struct mmc_cid cid;
    struct mmc_csd csd;
    struct mmc_ext_csd ext_csd;
    struct sd_scr scr;
    struct sd_ssr ssr;
    struct sd_switch_caps sw_caps;
    struct sd_ext_reg ext_power;
    struct sd_ext_reg ext_perf;
    unsigned int sdio_funcs;
    atomic_t sdio_funcs_probed;
    struct sdio_cccr cccr;
    struct sdio_cis cis;
    struct sdio_func * sdio_func[7];
    struct sdio_func *sdio_single_irq;
    u8 major_rev;
    u8 minor_rev;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
    unsigned int sd_bus_speed;
    unsigned int mmc_avail_type;
    unsigned int drive_strength;
    struct dentry *debugfs_root;
    struct mmc_part part[7];
    unsigned int nr_parts;
    struct workqueue_struct *complete_wq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mmc_card {
    struct mmc_host *host;
    struct device dev;
    u32 ocr;
    unsigned int rca;
    unsigned int type;
    unsigned int state;
    unsigned int quirks;
    unsigned int quirk_max_rate;
    bool reenable_cmdq;
    unsigned int erase_size;
    unsigned int erase_shift;
    unsigned int pref_erase;
    unsigned int eg_boundary;
    unsigned int erase_arg;
    u8 erased_byte;
    u32 raw_cid[4];
    u32 raw_csd[4];
    u32 raw_scr[2];
    u32 raw_ssr[16];
    struct mmc_cid cid;
    struct mmc_csd csd;
    struct mmc_ext_csd ext_csd;
    struct sd_scr scr;
    struct sd_ssr ssr;
    struct sd_switch_caps sw_caps;
    struct sd_ext_reg ext_power;
    struct sd_ext_reg ext_perf;
    unsigned int sdio_funcs;
    atomic_t sdio_funcs_probed;
    struct sdio_cccr cccr;
    struct sdio_cis cis;
    struct sdio_func * sdio_func[7];
    struct sdio_func *sdio_single_irq;
    u8 major_rev;
    u8 minor_rev;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
    unsigned int sd_bus_speed;
    unsigned int mmc_avail_type;
    unsigned int drive_strength;
    struct dentry *debugfs_root;
    struct mmc_part part[7];
    unsigned int nr_parts;
    struct workqueue_struct *complete_wq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mmc_card {
    struct mmc_host *host;
    struct device dev;
    u32 ocr;
    unsigned int rca;
    unsigned int type;
    unsigned int state;
    unsigned int quirks;
    unsigned int quirk_max_rate;
    bool reenable_cmdq;
    unsigned int erase_size;
    unsigned int erase_shift;
    unsigned int pref_erase;
    unsigned int eg_boundary;
    unsigned int erase_arg;
    u8 erased_byte;
    u32 raw_cid[4];
    u32 raw_csd[4];
    u32 raw_scr[2];
    u32 raw_ssr[16];
    struct mmc_cid cid;
    struct mmc_csd csd;
    struct mmc_ext_csd ext_csd;
    struct sd_scr scr;
    struct sd_ssr ssr;
    struct sd_switch_caps sw_caps;
    struct sd_ext_reg ext_power;
    struct sd_ext_reg ext_perf;
    unsigned int sdio_funcs;
    atomic_t sdio_funcs_probed;
    struct sdio_cccr cccr;
    struct sdio_cis cis;
    struct sdio_func * sdio_func[7];
    struct sdio_func *sdio_single_irq;
    u8 major_rev;
    u8 minor_rev;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
    unsigned int sd_bus_speed;
    unsigned int mmc_avail_type;
    unsigned int drive_strength;
    struct dentry *debugfs_root;
    struct mmc_part part[7];
    unsigned int nr_parts;
    struct workqueue_struct *complete_wq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mmc_card {
    struct mmc_host *host;
    struct device dev;
    u32 ocr;
    unsigned int rca;
    unsigned int type;
    unsigned int state;
    unsigned int quirks;
    unsigned int quirk_max_rate;
    bool reenable_cmdq;
    unsigned int erase_size;
    unsigned int erase_shift;
    unsigned int pref_erase;
    unsigned int eg_boundary;
    unsigned int erase_arg;
    u8 erased_byte;
    u32 raw_cid[4];
    u32 raw_csd[4];
    u32 raw_scr[2];
    u32 raw_ssr[16];
    struct mmc_cid cid;
    struct mmc_csd csd;
    struct mmc_ext_csd ext_csd;
    struct sd_scr scr;
    struct sd_ssr ssr;
    struct sd_switch_caps sw_caps;
    struct sd_ext_reg ext_power;
    struct sd_ext_reg ext_perf;
    unsigned int sdio_funcs;
    atomic_t sdio_funcs_probed;
    struct sdio_cccr cccr;
    struct sdio_cis cis;
    struct sdio_func * sdio_func[7];
    struct sdio_func *sdio_single_irq;
    u8 major_rev;
    u8 minor_rev;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
    unsigned int sd_bus_speed;
    unsigned int mmc_avail_type;
    unsigned int drive_strength;
    struct dentry *debugfs_root;
    struct mmc_part part[7];
    unsigned int nr_parts;
    struct workqueue_struct *complete_wq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mmc_card {
    struct mmc_host *host;
    struct device dev;
    u32 ocr;
    unsigned int rca;
    unsigned int type;
    unsigned int state;
    unsigned int quirks;
    unsigned int quirk_max_rate;
    bool written_flag;
    bool reenable_cmdq;
    unsigned int erase_size;
    unsigned int erase_shift;
    unsigned int pref_erase;
    unsigned int eg_boundary;
    unsigned int erase_arg;
    u8 erased_byte;
    unsigned int wp_grp_size;
    u32 raw_cid[4];
    u32 raw_csd[4];
    u32 raw_scr[2];
    u32 raw_ssr[16];
    struct mmc_cid cid;
    struct mmc_csd csd;
    struct mmc_ext_csd ext_csd;
    struct sd_scr scr;
    struct sd_ssr ssr;
    struct sd_switch_caps sw_caps;
    struct sd_ext_reg ext_power;
    struct sd_ext_reg ext_perf;
    unsigned int sdio_funcs;
    atomic_t sdio_funcs_probed;
    struct sdio_cccr cccr;
    struct sdio_cis cis;
    struct sdio_func * sdio_func[7];
    struct sdio_func *sdio_single_irq;
    u8 major_rev;
    u8 minor_rev;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
    unsigned int sd_bus_speed;
    unsigned int mmc_avail_type;
    unsigned int drive_strength;
    struct dentry *debugfs_root;
    struct mmc_part part[7];
    unsigned int nr_parts;
    struct workqueue_struct *complete_wq;
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
struct mmc_card {
    struct mmc_host *host;
    struct device dev;
    u32 ocr;
    unsigned int rca;
    unsigned int type;
    unsigned int state;
    unsigned int quirks;
    unsigned int quirk_max_rate;
    bool reenable_cmdq;
    unsigned int erase_size;
    unsigned int erase_shift;
    unsigned int pref_erase;
    unsigned int eg_boundary;
    unsigned int erase_arg;
    u8 erased_byte;
    u32 raw_cid[4];
    u32 raw_csd[4];
    u32 raw_scr[2];
    u32 raw_ssr[16];
    struct mmc_cid cid;
    struct mmc_csd csd;
    struct mmc_ext_csd ext_csd;
    struct sd_scr scr;
    struct sd_ssr ssr;
    struct sd_switch_caps sw_caps;
    unsigned int sdio_funcs;
    atomic_t sdio_funcs_probed;
    struct sdio_cccr cccr;
    struct sdio_cis cis;
    struct sdio_func * sdio_func[7];
    struct sdio_func *sdio_single_irq;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
    unsigned int sd_bus_speed;
    unsigned int mmc_avail_type;
    unsigned int drive_strength;
    struct dentry *debugfs_root;
    struct mmc_part part[7];
    unsigned int nr_parts;
    unsigned int bouncesz;
    struct workqueue_struct *complete_wq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mmc_card {
    struct mmc_host *host;
    struct device dev;
    u32 ocr;
    unsigned int rca;
    unsigned int type;
    unsigned int state;
    unsigned int quirks;
    unsigned int quirk_max_rate;
    bool reenable_cmdq;
    unsigned int erase_size;
    unsigned int erase_shift;
    unsigned int pref_erase;
    unsigned int eg_boundary;
    unsigned int erase_arg;
    u8 erased_byte;
    u32 raw_cid[4];
    u32 raw_csd[4];
    u32 raw_scr[2];
    u32 raw_ssr[16];
    struct mmc_cid cid;
    struct mmc_csd csd;
    struct mmc_ext_csd ext_csd;
    struct sd_scr scr;
    struct sd_ssr ssr;
    struct sd_switch_caps sw_caps;
    unsigned int sdio_funcs;
    atomic_t sdio_funcs_probed;
    struct sdio_cccr cccr;
    struct sdio_cis cis;
    struct sdio_func * sdio_func[7];
    struct sdio_func *sdio_single_irq;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
    unsigned int sd_bus_speed;
    unsigned int mmc_avail_type;
    unsigned int drive_strength;
    struct dentry *debugfs_root;
    struct mmc_part part[7];
    unsigned int nr_parts;
    unsigned int bouncesz;
    struct workqueue_struct *complete_wq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct mmc_card {
    struct mmc_host *host;
    struct device dev;
    u32 ocr;
    unsigned int rca;
    unsigned int type;
    unsigned int state;
    unsigned int quirks;
    unsigned int quirk_max_rate;
    bool reenable_cmdq;
    unsigned int erase_size;
    unsigned int erase_shift;
    unsigned int pref_erase;
    unsigned int eg_boundary;
    unsigned int erase_arg;
    u8 erased_byte;
    u32 raw_cid[4];
    u32 raw_csd[4];
    u32 raw_scr[2];
    u32 raw_ssr[16];
    struct mmc_cid cid;
    struct mmc_csd csd;
    struct mmc_ext_csd ext_csd;
    struct sd_scr scr;
    struct sd_ssr ssr;
    struct sd_switch_caps sw_caps;
    unsigned int sdio_funcs;
    atomic_t sdio_funcs_probed;
    struct sdio_cccr cccr;
    struct sdio_cis cis;
    struct sdio_func * sdio_func[7];
    struct sdio_func *sdio_single_irq;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
    unsigned int sd_bus_speed;
    unsigned int mmc_avail_type;
    unsigned int drive_strength;
    struct dentry *debugfs_root;
    struct mmc_part part[7];
    unsigned int nr_parts;
    unsigned int bouncesz;
    struct workqueue_struct *complete_wq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct mmc_card {
    struct mmc_host *host;
    struct device dev;
    u32 ocr;
    unsigned int rca;
    unsigned int type;
    unsigned int state;
    unsigned int quirks;
    unsigned int quirk_max_rate;
    bool reenable_cmdq;
    unsigned int erase_size;
    unsigned int erase_shift;
    unsigned int pref_erase;
    unsigned int eg_boundary;
    unsigned int erase_arg;
    u8 erased_byte;
    u32 raw_cid[4];
    u32 raw_csd[4];
    u32 raw_scr[2];
    u32 raw_ssr[16];
    struct mmc_cid cid;
    struct mmc_csd csd;
    struct mmc_ext_csd ext_csd;
    struct sd_scr scr;
    struct sd_ssr ssr;
    struct sd_switch_caps sw_caps;
    unsigned int sdio_funcs;
    atomic_t sdio_funcs_probed;
    struct sdio_cccr cccr;
    struct sdio_cis cis;
    struct sdio_func * sdio_func[7];
    struct sdio_func *sdio_single_irq;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
    unsigned int sd_bus_speed;
    unsigned int mmc_avail_type;
    unsigned int drive_strength;
    struct dentry *debugfs_root;
    struct mmc_part part[7];
    unsigned int nr_parts;
    unsigned int bouncesz;
    struct workqueue_struct *complete_wq;
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
struct mmc_card {
    struct mmc_host *host;
    struct device dev;
    u32 ocr;
    unsigned int rca;
    unsigned int type;
    unsigned int state;
    unsigned int quirks;
    unsigned int quirk_max_rate;
    bool reenable_cmdq;
    unsigned int erase_size;
    unsigned int erase_shift;
    unsigned int pref_erase;
    unsigned int eg_boundary;
    unsigned int erase_arg;
    u8 erased_byte;
    u32 raw_cid[4];
    u32 raw_csd[4];
    u32 raw_scr[2];
    u32 raw_ssr[16];
    struct mmc_cid cid;
    struct mmc_csd csd;
    struct mmc_ext_csd ext_csd;
    struct sd_scr scr;
    struct sd_ssr ssr;
    struct sd_switch_caps sw_caps;
    unsigned int sdio_funcs;
    atomic_t sdio_funcs_probed;
    struct sdio_cccr cccr;
    struct sdio_cis cis;
    struct sdio_func * sdio_func[7];
    struct sdio_func *sdio_single_irq;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
    unsigned int sd_bus_speed;
    unsigned int mmc_avail_type;
    unsigned int drive_strength;
    struct dentry *debugfs_root;
    struct mmc_part part[7];
    unsigned int nr_parts;
    unsigned int bouncesz;
    struct workqueue_struct *complete_wq;
};
```
</details>
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct mmc_card {
    struct mmc_host *host;
    struct device dev;
    u32 ocr;
    unsigned int rca;
    unsigned int type;
    unsigned int state;
    unsigned int quirks;
    unsigned int quirk_max_rate;
    bool reenable_cmdq;
    unsigned int erase_size;
    unsigned int erase_shift;
    unsigned int pref_erase;
    unsigned int eg_boundary;
    unsigned int erase_arg;
    u8 erased_byte;
    u32 raw_cid[4];
    u32 raw_csd[4];
    u32 raw_scr[2];
    u32 raw_ssr[16];
    struct mmc_cid cid;
    struct mmc_csd csd;
    struct mmc_ext_csd ext_csd;
    struct sd_scr scr;
    struct sd_ssr ssr;
    struct sd_switch_caps sw_caps;
    unsigned int sdio_funcs;
    atomic_t sdio_funcs_probed;
    struct sdio_cccr cccr;
    struct sdio_cis cis;
    struct sdio_func * sdio_func[7];
    struct sdio_func *sdio_single_irq;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
    unsigned int sd_bus_speed;
    unsigned int mmc_avail_type;
    unsigned int drive_strength;
    struct dentry *debugfs_root;
    struct mmc_part part[7];
    unsigned int nr_parts;
    unsigned int bouncesz;
    struct workqueue_struct *complete_wq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct mmc_card {
    struct mmc_host *host;
    struct device dev;
    u32 ocr;
    unsigned int rca;
    unsigned int type;
    unsigned int state;
    unsigned int quirks;
    unsigned int quirk_max_rate;
    bool reenable_cmdq;
    unsigned int erase_size;
    unsigned int erase_shift;
    unsigned int pref_erase;
    unsigned int eg_boundary;
    unsigned int erase_arg;
    u8 erased_byte;
    u32 raw_cid[4];
    u32 raw_csd[4];
    u32 raw_scr[2];
    u32 raw_ssr[16];
    struct mmc_cid cid;
    struct mmc_csd csd;
    struct mmc_ext_csd ext_csd;
    struct sd_scr scr;
    struct sd_ssr ssr;
    struct sd_switch_caps sw_caps;
    unsigned int sdio_funcs;
    atomic_t sdio_funcs_probed;
    struct sdio_cccr cccr;
    struct sdio_cis cis;
    struct sdio_func * sdio_func[7];
    struct sdio_func *sdio_single_irq;
    unsigned int num_info;
    const char **info;
    struct sdio_func_tuple *tuples;
    unsigned int sd_bus_speed;
    unsigned int mmc_avail_type;
    unsigned int drive_strength;
    struct dentry *debugfs_root;
    struct mmc_part part[7];
    unsigned int nr_parts;
    unsigned int bouncesz;
    struct workqueue_struct *complete_wq;
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
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 raw_ssr[16]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool reenable_cmdq</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int bouncesz</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int quirk_max_rate</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct workqueue_struct *complete_wq</code>
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
<code>unsigned int erase_arg</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>atomic_t sdio_funcs_probed</code>
</li>
</ul>
</details>
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
<code>u8 major_rev</code>
</li>
<li>
<b>Field added. </b>
<code>u8 minor_rev</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned int bouncesz</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct sd_ext_reg ext_power</code>
</li>
<li>
<b>Field added. </b>
<code>struct sd_ext_reg ext_perf</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool written_flag</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int wp_grp_size</code>
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
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
