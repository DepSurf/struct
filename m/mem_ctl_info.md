# Struct: <code>mem_ctl_info</code>

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
struct mem_ctl_info {
    struct device dev;
    struct bus_type *bus;
    struct list_head link;
    struct module *owner;
    long unsigned int mtype_cap;
    long unsigned int edac_ctl_cap;
    long unsigned int edac_cap;
    long unsigned int scrub_cap;
    enum scrub_type scrub_mode;
    int (*set_sdram_scrub_rate)(struct mem_ctl_info *, u32);
    int (*get_sdram_scrub_rate)(struct mem_ctl_info *);
    void (*edac_check)(struct mem_ctl_info *);
    long unsigned int (*ctl_page_to_phys)(struct mem_ctl_info *, long unsigned int);
    int mc_idx;
    struct csrow_info **csrows;
    unsigned int nr_csrows;
    unsigned int num_cschannel;
    unsigned int n_layers;
    struct edac_mc_layer *layers;
    bool csbased;
    unsigned int tot_dimms;
    struct dimm_info **dimms;
    struct device *pdev;
    const char *mod_name;
    const char *mod_ver;
    const char *ctl_name;
    const char *dev_name;
    void *pvt_info;
    long unsigned int start_time;
    u32 ce_noinfo_count;
    u32 ue_noinfo_count;
    u32 ue_mc;
    u32 ce_mc;
    u32 * ce_per_layer[3];
    u32 * ue_per_layer[3];
    struct completion complete;
    const struct mcidev_sysfs_attribute *mc_driver_sysfs_attributes;
    struct delayed_work work;
    struct edac_raw_error_desc error_desc;
    int op_state;
    struct dentry *debugfs;
    u8 fake_inject_layer[3];
    bool fake_inject_ue;
    u16 fake_inject_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct mem_ctl_info {
    struct device dev;
    struct bus_type *bus;
    struct list_head link;
    struct module *owner;
    long unsigned int mtype_cap;
    long unsigned int edac_ctl_cap;
    long unsigned int edac_cap;
    long unsigned int scrub_cap;
    enum scrub_type scrub_mode;
    int (*set_sdram_scrub_rate)(struct mem_ctl_info *, u32);
    int (*get_sdram_scrub_rate)(struct mem_ctl_info *);
    void (*edac_check)(struct mem_ctl_info *);
    long unsigned int (*ctl_page_to_phys)(struct mem_ctl_info *, long unsigned int);
    int mc_idx;
    struct csrow_info **csrows;
    unsigned int nr_csrows;
    unsigned int num_cschannel;
    unsigned int n_layers;
    struct edac_mc_layer *layers;
    bool csbased;
    unsigned int tot_dimms;
    struct dimm_info **dimms;
    struct device *pdev;
    const char *mod_name;
    const char *ctl_name;
    const char *dev_name;
    void *pvt_info;
    long unsigned int start_time;
    u32 ce_noinfo_count;
    u32 ue_noinfo_count;
    u32 ue_mc;
    u32 ce_mc;
    u32 * ce_per_layer[3];
    u32 * ue_per_layer[3];
    struct completion complete;
    const struct mcidev_sysfs_attribute *mc_driver_sysfs_attributes;
    struct delayed_work work;
    struct edac_raw_error_desc error_desc;
    int op_state;
    struct dentry *debugfs;
    u8 fake_inject_layer[3];
    bool fake_inject_ue;
    u16 fake_inject_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct mem_ctl_info {
    struct device dev;
    struct bus_type *bus;
    struct list_head link;
    struct module *owner;
    long unsigned int mtype_cap;
    long unsigned int edac_ctl_cap;
    long unsigned int edac_cap;
    long unsigned int scrub_cap;
    enum scrub_type scrub_mode;
    int (*set_sdram_scrub_rate)(struct mem_ctl_info *, u32);
    int (*get_sdram_scrub_rate)(struct mem_ctl_info *);
    void (*edac_check)(struct mem_ctl_info *);
    long unsigned int (*ctl_page_to_phys)(struct mem_ctl_info *, long unsigned int);
    int mc_idx;
    struct csrow_info **csrows;
    unsigned int nr_csrows;
    unsigned int num_cschannel;
    unsigned int n_layers;
    struct edac_mc_layer *layers;
    bool csbased;
    unsigned int tot_dimms;
    struct dimm_info **dimms;
    struct device *pdev;
    const char *mod_name;
    const char *ctl_name;
    const char *dev_name;
    void *pvt_info;
    long unsigned int start_time;
    u32 ce_noinfo_count;
    u32 ue_noinfo_count;
    u32 ue_mc;
    u32 ce_mc;
    u32 * ce_per_layer[3];
    u32 * ue_per_layer[3];
    struct completion complete;
    const struct mcidev_sysfs_attribute *mc_driver_sysfs_attributes;
    struct delayed_work work;
    struct edac_raw_error_desc error_desc;
    int op_state;
    struct dentry *debugfs;
    u8 fake_inject_layer[3];
    bool fake_inject_ue;
    u16 fake_inject_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct mem_ctl_info {
    struct device dev;
    struct bus_type *bus;
    struct list_head link;
    struct module *owner;
    long unsigned int mtype_cap;
    long unsigned int edac_ctl_cap;
    long unsigned int edac_cap;
    long unsigned int scrub_cap;
    enum scrub_type scrub_mode;
    int (*set_sdram_scrub_rate)(struct mem_ctl_info *, u32);
    int (*get_sdram_scrub_rate)(struct mem_ctl_info *);
    void (*edac_check)(struct mem_ctl_info *);
    long unsigned int (*ctl_page_to_phys)(struct mem_ctl_info *, long unsigned int);
    int mc_idx;
    struct csrow_info **csrows;
    unsigned int nr_csrows;
    unsigned int num_cschannel;
    unsigned int n_layers;
    struct edac_mc_layer *layers;
    bool csbased;
    unsigned int tot_dimms;
    struct dimm_info **dimms;
    struct device *pdev;
    const char *mod_name;
    const char *ctl_name;
    const char *dev_name;
    void *pvt_info;
    long unsigned int start_time;
    u32 ce_noinfo_count;
    u32 ue_noinfo_count;
    u32 ue_mc;
    u32 ce_mc;
    u32 * ce_per_layer[3];
    u32 * ue_per_layer[3];
    struct completion complete;
    const struct mcidev_sysfs_attribute *mc_driver_sysfs_attributes;
    struct delayed_work work;
    struct edac_raw_error_desc error_desc;
    int op_state;
    struct dentry *debugfs;
    u8 fake_inject_layer[3];
    bool fake_inject_ue;
    u16 fake_inject_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct mem_ctl_info {
    struct device dev;
    struct bus_type *bus;
    struct list_head link;
    struct module *owner;
    long unsigned int mtype_cap;
    long unsigned int edac_ctl_cap;
    long unsigned int edac_cap;
    long unsigned int scrub_cap;
    enum scrub_type scrub_mode;
    int (*set_sdram_scrub_rate)(struct mem_ctl_info *, u32);
    int (*get_sdram_scrub_rate)(struct mem_ctl_info *);
    void (*edac_check)(struct mem_ctl_info *);
    long unsigned int (*ctl_page_to_phys)(struct mem_ctl_info *, long unsigned int);
    int mc_idx;
    struct csrow_info **csrows;
    unsigned int nr_csrows;
    unsigned int num_cschannel;
    unsigned int n_layers;
    struct edac_mc_layer *layers;
    bool csbased;
    unsigned int tot_dimms;
    struct dimm_info **dimms;
    struct device *pdev;
    const char *mod_name;
    const char *ctl_name;
    const char *dev_name;
    void *pvt_info;
    long unsigned int start_time;
    u32 ce_noinfo_count;
    u32 ue_noinfo_count;
    u32 ue_mc;
    u32 ce_mc;
    u32 * ce_per_layer[3];
    u32 * ue_per_layer[3];
    struct completion complete;
    const struct mcidev_sysfs_attribute *mc_driver_sysfs_attributes;
    struct delayed_work work;
    struct edac_raw_error_desc error_desc;
    int op_state;
    struct dentry *debugfs;
    u8 fake_inject_layer[3];
    bool fake_inject_ue;
    u16 fake_inject_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct mem_ctl_info {
    struct device dev;
    struct bus_type *bus;
    struct list_head link;
    struct module *owner;
    long unsigned int mtype_cap;
    long unsigned int edac_ctl_cap;
    long unsigned int edac_cap;
    long unsigned int scrub_cap;
    enum scrub_type scrub_mode;
    int (*set_sdram_scrub_rate)(struct mem_ctl_info *, u32);
    int (*get_sdram_scrub_rate)(struct mem_ctl_info *);
    void (*edac_check)(struct mem_ctl_info *);
    long unsigned int (*ctl_page_to_phys)(struct mem_ctl_info *, long unsigned int);
    int mc_idx;
    struct csrow_info **csrows;
    unsigned int nr_csrows;
    unsigned int num_cschannel;
    unsigned int n_layers;
    struct edac_mc_layer *layers;
    bool csbased;
    unsigned int tot_dimms;
    struct dimm_info **dimms;
    struct device *pdev;
    const char *mod_name;
    const char *ctl_name;
    const char *dev_name;
    void *pvt_info;
    long unsigned int start_time;
    u32 ce_noinfo_count;
    u32 ue_noinfo_count;
    u32 ue_mc;
    u32 ce_mc;
    u32 * ce_per_layer[3];
    u32 * ue_per_layer[3];
    struct completion complete;
    const struct mcidev_sysfs_attribute *mc_driver_sysfs_attributes;
    struct delayed_work work;
    struct edac_raw_error_desc error_desc;
    int op_state;
    struct dentry *debugfs;
    u8 fake_inject_layer[3];
    bool fake_inject_ue;
    u16 fake_inject_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct mem_ctl_info {
    struct device dev;
    struct bus_type *bus;
    struct list_head link;
    struct module *owner;
    long unsigned int mtype_cap;
    long unsigned int edac_ctl_cap;
    long unsigned int edac_cap;
    long unsigned int scrub_cap;
    enum scrub_type scrub_mode;
    int (*set_sdram_scrub_rate)(struct mem_ctl_info *, u32);
    int (*get_sdram_scrub_rate)(struct mem_ctl_info *);
    void (*edac_check)(struct mem_ctl_info *);
    long unsigned int (*ctl_page_to_phys)(struct mem_ctl_info *, long unsigned int);
    int mc_idx;
    struct csrow_info **csrows;
    unsigned int nr_csrows;
    unsigned int num_cschannel;
    unsigned int n_layers;
    struct edac_mc_layer *layers;
    bool csbased;
    unsigned int tot_dimms;
    struct dimm_info **dimms;
    struct device *pdev;
    const char *mod_name;
    const char *ctl_name;
    const char *dev_name;
    void *pvt_info;
    long unsigned int start_time;
    u32 ce_noinfo_count;
    u32 ue_noinfo_count;
    u32 ue_mc;
    u32 ce_mc;
    struct completion complete;
    const struct mcidev_sysfs_attribute *mc_driver_sysfs_attributes;
    struct delayed_work work;
    struct edac_raw_error_desc error_desc;
    int op_state;
    struct dentry *debugfs;
    u8 fake_inject_layer[3];
    bool fake_inject_ue;
    u16 fake_inject_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mem_ctl_info {
    struct device dev;
    struct bus_type *bus;
    struct list_head link;
    struct module *owner;
    long unsigned int mtype_cap;
    long unsigned int edac_ctl_cap;
    long unsigned int edac_cap;
    long unsigned int scrub_cap;
    enum scrub_type scrub_mode;
    int (*set_sdram_scrub_rate)(struct mem_ctl_info *, u32);
    int (*get_sdram_scrub_rate)(struct mem_ctl_info *);
    void (*edac_check)(struct mem_ctl_info *);
    long unsigned int (*ctl_page_to_phys)(struct mem_ctl_info *, long unsigned int);
    int mc_idx;
    struct csrow_info **csrows;
    unsigned int nr_csrows;
    unsigned int num_cschannel;
    unsigned int n_layers;
    struct edac_mc_layer *layers;
    bool csbased;
    unsigned int tot_dimms;
    struct dimm_info **dimms;
    struct device *pdev;
    const char *mod_name;
    const char *ctl_name;
    const char *dev_name;
    void *pvt_info;
    long unsigned int start_time;
    u32 ce_noinfo_count;
    u32 ue_noinfo_count;
    u32 ue_mc;
    u32 ce_mc;
    struct completion complete;
    const struct mcidev_sysfs_attribute *mc_driver_sysfs_attributes;
    struct delayed_work work;
    struct edac_raw_error_desc error_desc;
    int op_state;
    struct dentry *debugfs;
    u8 fake_inject_layer[3];
    bool fake_inject_ue;
    u16 fake_inject_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mem_ctl_info {
    struct device dev;
    struct bus_type *bus;
    struct list_head link;
    struct module *owner;
    long unsigned int mtype_cap;
    long unsigned int edac_ctl_cap;
    long unsigned int edac_cap;
    long unsigned int scrub_cap;
    enum scrub_type scrub_mode;
    int (*set_sdram_scrub_rate)(struct mem_ctl_info *, u32);
    int (*get_sdram_scrub_rate)(struct mem_ctl_info *);
    void (*edac_check)(struct mem_ctl_info *);
    long unsigned int (*ctl_page_to_phys)(struct mem_ctl_info *, long unsigned int);
    int mc_idx;
    struct csrow_info **csrows;
    unsigned int nr_csrows;
    unsigned int num_cschannel;
    unsigned int n_layers;
    struct edac_mc_layer *layers;
    bool csbased;
    unsigned int tot_dimms;
    struct dimm_info **dimms;
    struct device *pdev;
    const char *mod_name;
    const char *ctl_name;
    const char *dev_name;
    void *pvt_info;
    long unsigned int start_time;
    u32 ce_noinfo_count;
    u32 ue_noinfo_count;
    u32 ue_mc;
    u32 ce_mc;
    struct completion complete;
    const struct mcidev_sysfs_attribute *mc_driver_sysfs_attributes;
    struct delayed_work work;
    struct edac_raw_error_desc error_desc;
    int op_state;
    struct dentry *debugfs;
    u8 fake_inject_layer[3];
    bool fake_inject_ue;
    u16 fake_inject_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mem_ctl_info {
    struct device dev;
    struct bus_type *bus;
    struct list_head link;
    struct module *owner;
    long unsigned int mtype_cap;
    long unsigned int edac_ctl_cap;
    long unsigned int edac_cap;
    long unsigned int scrub_cap;
    enum scrub_type scrub_mode;
    int (*set_sdram_scrub_rate)(struct mem_ctl_info *, u32);
    int (*get_sdram_scrub_rate)(struct mem_ctl_info *);
    void (*edac_check)(struct mem_ctl_info *);
    long unsigned int (*ctl_page_to_phys)(struct mem_ctl_info *, long unsigned int);
    int mc_idx;
    struct csrow_info **csrows;
    unsigned int nr_csrows;
    unsigned int num_cschannel;
    unsigned int n_layers;
    struct edac_mc_layer *layers;
    bool csbased;
    unsigned int tot_dimms;
    struct dimm_info **dimms;
    struct device *pdev;
    const char *mod_name;
    const char *ctl_name;
    const char *dev_name;
    void *pvt_info;
    long unsigned int start_time;
    u32 ce_noinfo_count;
    u32 ue_noinfo_count;
    u32 ue_mc;
    u32 ce_mc;
    struct completion complete;
    const struct mcidev_sysfs_attribute *mc_driver_sysfs_attributes;
    struct delayed_work work;
    struct edac_raw_error_desc error_desc;
    int op_state;
    struct dentry *debugfs;
    u8 fake_inject_layer[3];
    bool fake_inject_ue;
    u16 fake_inject_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mem_ctl_info {
    struct device dev;
    struct bus_type *bus;
    struct list_head link;
    struct module *owner;
    long unsigned int mtype_cap;
    long unsigned int edac_ctl_cap;
    long unsigned int edac_cap;
    long unsigned int scrub_cap;
    enum scrub_type scrub_mode;
    int (*set_sdram_scrub_rate)(struct mem_ctl_info *, u32);
    int (*get_sdram_scrub_rate)(struct mem_ctl_info *);
    void (*edac_check)(struct mem_ctl_info *);
    long unsigned int (*ctl_page_to_phys)(struct mem_ctl_info *, long unsigned int);
    int mc_idx;
    struct csrow_info **csrows;
    unsigned int nr_csrows;
    unsigned int num_cschannel;
    unsigned int n_layers;
    struct edac_mc_layer *layers;
    bool csbased;
    unsigned int tot_dimms;
    struct dimm_info **dimms;
    struct device *pdev;
    const char *mod_name;
    const char *ctl_name;
    const char *dev_name;
    void *pvt_info;
    long unsigned int start_time;
    u32 ce_noinfo_count;
    u32 ue_noinfo_count;
    u32 ue_mc;
    u32 ce_mc;
    struct completion complete;
    const struct mcidev_sysfs_attribute *mc_driver_sysfs_attributes;
    struct delayed_work work;
    struct edac_raw_error_desc error_desc;
    int op_state;
    struct dentry *debugfs;
    u8 fake_inject_layer[3];
    bool fake_inject_ue;
    u16 fake_inject_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mem_ctl_info {
    struct device dev;
    struct bus_type *bus;
    struct list_head link;
    struct module *owner;
    long unsigned int mtype_cap;
    long unsigned int edac_ctl_cap;
    long unsigned int edac_cap;
    long unsigned int scrub_cap;
    enum scrub_type scrub_mode;
    int (*set_sdram_scrub_rate)(struct mem_ctl_info *, u32);
    int (*get_sdram_scrub_rate)(struct mem_ctl_info *);
    void (*edac_check)(struct mem_ctl_info *);
    long unsigned int (*ctl_page_to_phys)(struct mem_ctl_info *, long unsigned int);
    int mc_idx;
    struct csrow_info **csrows;
    unsigned int nr_csrows;
    unsigned int num_cschannel;
    unsigned int n_layers;
    struct edac_mc_layer *layers;
    bool csbased;
    unsigned int tot_dimms;
    struct dimm_info **dimms;
    struct device *pdev;
    const char *mod_name;
    const char *ctl_name;
    const char *dev_name;
    void *pvt_info;
    long unsigned int start_time;
    u32 ce_noinfo_count;
    u32 ue_noinfo_count;
    u32 ue_mc;
    u32 ce_mc;
    struct completion complete;
    const struct mcidev_sysfs_attribute *mc_driver_sysfs_attributes;
    struct delayed_work work;
    struct edac_raw_error_desc error_desc;
    int op_state;
    struct dentry *debugfs;
    u8 fake_inject_layer[3];
    bool fake_inject_ue;
    u16 fake_inject_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mem_ctl_info {
    struct device dev;
    struct bus_type *bus;
    struct list_head link;
    struct module *owner;
    long unsigned int mtype_cap;
    long unsigned int edac_ctl_cap;
    long unsigned int edac_cap;
    long unsigned int scrub_cap;
    enum scrub_type scrub_mode;
    int (*set_sdram_scrub_rate)(struct mem_ctl_info *, u32);
    int (*get_sdram_scrub_rate)(struct mem_ctl_info *);
    void (*edac_check)(struct mem_ctl_info *);
    long unsigned int (*ctl_page_to_phys)(struct mem_ctl_info *, long unsigned int);
    int mc_idx;
    struct csrow_info **csrows;
    unsigned int nr_csrows;
    unsigned int num_cschannel;
    unsigned int n_layers;
    struct edac_mc_layer *layers;
    bool csbased;
    unsigned int tot_dimms;
    struct dimm_info **dimms;
    struct device *pdev;
    const char *mod_name;
    const char *ctl_name;
    const char *dev_name;
    void *pvt_info;
    long unsigned int start_time;
    u32 ce_noinfo_count;
    u32 ue_noinfo_count;
    u32 ue_mc;
    u32 ce_mc;
    struct completion complete;
    const struct mcidev_sysfs_attribute *mc_driver_sysfs_attributes;
    struct delayed_work work;
    struct edac_raw_error_desc error_desc;
    int op_state;
    struct dentry *debugfs;
    u8 fake_inject_layer[3];
    bool fake_inject_ue;
    u16 fake_inject_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mem_ctl_info {
    struct device dev;
    const struct bus_type *bus;
    struct list_head link;
    struct module *owner;
    long unsigned int mtype_cap;
    long unsigned int edac_ctl_cap;
    long unsigned int edac_cap;
    long unsigned int scrub_cap;
    enum scrub_type scrub_mode;
    int (*set_sdram_scrub_rate)(struct mem_ctl_info *, u32);
    int (*get_sdram_scrub_rate)(struct mem_ctl_info *);
    void (*edac_check)(struct mem_ctl_info *);
    long unsigned int (*ctl_page_to_phys)(struct mem_ctl_info *, long unsigned int);
    int mc_idx;
    struct csrow_info **csrows;
    unsigned int nr_csrows;
    unsigned int num_cschannel;
    unsigned int n_layers;
    struct edac_mc_layer *layers;
    bool csbased;
    unsigned int tot_dimms;
    struct dimm_info **dimms;
    struct device *pdev;
    const char *mod_name;
    const char *ctl_name;
    const char *dev_name;
    void *pvt_info;
    long unsigned int start_time;
    u32 ce_noinfo_count;
    u32 ue_noinfo_count;
    u32 ue_mc;
    u32 ce_mc;
    struct completion complete;
    const struct mcidev_sysfs_attribute *mc_driver_sysfs_attributes;
    struct delayed_work work;
    struct edac_raw_error_desc error_desc;
    int op_state;
    struct dentry *debugfs;
    u8 fake_inject_layer[3];
    bool fake_inject_ue;
    u16 fake_inject_count;
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
struct mem_ctl_info {
    struct device dev;
    struct bus_type *bus;
    struct list_head link;
    struct module *owner;
    long unsigned int mtype_cap;
    long unsigned int edac_ctl_cap;
    long unsigned int edac_cap;
    long unsigned int scrub_cap;
    enum scrub_type scrub_mode;
    int (*set_sdram_scrub_rate)(struct mem_ctl_info *, u32);
    int (*get_sdram_scrub_rate)(struct mem_ctl_info *);
    void (*edac_check)(struct mem_ctl_info *);
    long unsigned int (*ctl_page_to_phys)(struct mem_ctl_info *, long unsigned int);
    int mc_idx;
    struct csrow_info **csrows;
    unsigned int nr_csrows;
    unsigned int num_cschannel;
    unsigned int n_layers;
    struct edac_mc_layer *layers;
    bool csbased;
    unsigned int tot_dimms;
    struct dimm_info **dimms;
    struct device *pdev;
    const char *mod_name;
    const char *ctl_name;
    const char *dev_name;
    void *pvt_info;
    long unsigned int start_time;
    u32 ce_noinfo_count;
    u32 ue_noinfo_count;
    u32 ue_mc;
    u32 ce_mc;
    u32 * ce_per_layer[3];
    u32 * ue_per_layer[3];
    struct completion complete;
    const struct mcidev_sysfs_attribute *mc_driver_sysfs_attributes;
    struct delayed_work work;
    struct edac_raw_error_desc error_desc;
    int op_state;
    struct dentry *debugfs;
    u8 fake_inject_layer[3];
    bool fake_inject_ue;
    u16 fake_inject_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mem_ctl_info {
    struct device dev;
    struct bus_type *bus;
    struct list_head link;
    struct module *owner;
    long unsigned int mtype_cap;
    long unsigned int edac_ctl_cap;
    long unsigned int edac_cap;
    long unsigned int scrub_cap;
    enum scrub_type scrub_mode;
    int (*set_sdram_scrub_rate)(struct mem_ctl_info *, u32);
    int (*get_sdram_scrub_rate)(struct mem_ctl_info *);
    void (*edac_check)(struct mem_ctl_info *);
    long unsigned int (*ctl_page_to_phys)(struct mem_ctl_info *, long unsigned int);
    int mc_idx;
    struct csrow_info **csrows;
    unsigned int nr_csrows;
    unsigned int num_cschannel;
    unsigned int n_layers;
    struct edac_mc_layer *layers;
    bool csbased;
    unsigned int tot_dimms;
    struct dimm_info **dimms;
    struct device *pdev;
    const char *mod_name;
    const char *ctl_name;
    const char *dev_name;
    void *pvt_info;
    long unsigned int start_time;
    u32 ce_noinfo_count;
    u32 ue_noinfo_count;
    u32 ue_mc;
    u32 ce_mc;
    u32 * ce_per_layer[3];
    u32 * ue_per_layer[3];
    struct completion complete;
    const struct mcidev_sysfs_attribute *mc_driver_sysfs_attributes;
    struct delayed_work work;
    struct edac_raw_error_desc error_desc;
    int op_state;
    struct dentry *debugfs;
    u8 fake_inject_layer[3];
    bool fake_inject_ue;
    u16 fake_inject_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct mem_ctl_info {
    struct device dev;
    struct bus_type *bus;
    struct list_head link;
    struct module *owner;
    long unsigned int mtype_cap;
    long unsigned int edac_ctl_cap;
    long unsigned int edac_cap;
    long unsigned int scrub_cap;
    enum scrub_type scrub_mode;
    int (*set_sdram_scrub_rate)(struct mem_ctl_info *, u32);
    int (*get_sdram_scrub_rate)(struct mem_ctl_info *);
    void (*edac_check)(struct mem_ctl_info *);
    long unsigned int (*ctl_page_to_phys)(struct mem_ctl_info *, long unsigned int);
    int mc_idx;
    struct csrow_info **csrows;
    unsigned int nr_csrows;
    unsigned int num_cschannel;
    unsigned int n_layers;
    struct edac_mc_layer *layers;
    bool csbased;
    unsigned int tot_dimms;
    struct dimm_info **dimms;
    struct device *pdev;
    const char *mod_name;
    const char *ctl_name;
    const char *dev_name;
    void *pvt_info;
    long unsigned int start_time;
    u32 ce_noinfo_count;
    u32 ue_noinfo_count;
    u32 ue_mc;
    u32 ce_mc;
    u32 * ce_per_layer[3];
    u32 * ue_per_layer[3];
    struct completion complete;
    const struct mcidev_sysfs_attribute *mc_driver_sysfs_attributes;
    struct delayed_work work;
    struct edac_raw_error_desc error_desc;
    int op_state;
    struct dentry *debugfs;
    u8 fake_inject_layer[3];
    bool fake_inject_ue;
    u16 fake_inject_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct mem_ctl_info {
    struct device dev;
    struct bus_type *bus;
    struct list_head link;
    struct module *owner;
    long unsigned int mtype_cap;
    long unsigned int edac_ctl_cap;
    long unsigned int edac_cap;
    long unsigned int scrub_cap;
    enum scrub_type scrub_mode;
    int (*set_sdram_scrub_rate)(struct mem_ctl_info *, u32);
    int (*get_sdram_scrub_rate)(struct mem_ctl_info *);
    void (*edac_check)(struct mem_ctl_info *);
    long unsigned int (*ctl_page_to_phys)(struct mem_ctl_info *, long unsigned int);
    int mc_idx;
    struct csrow_info **csrows;
    unsigned int nr_csrows;
    unsigned int num_cschannel;
    unsigned int n_layers;
    struct edac_mc_layer *layers;
    bool csbased;
    unsigned int tot_dimms;
    struct dimm_info **dimms;
    struct device *pdev;
    const char *mod_name;
    const char *ctl_name;
    const char *dev_name;
    void *pvt_info;
    long unsigned int start_time;
    u32 ce_noinfo_count;
    u32 ue_noinfo_count;
    u32 ue_mc;
    u32 ce_mc;
    u32 * ce_per_layer[3];
    u32 * ue_per_layer[3];
    struct completion complete;
    const struct mcidev_sysfs_attribute *mc_driver_sysfs_attributes;
    struct delayed_work work;
    struct edac_raw_error_desc error_desc;
    int op_state;
    struct dentry *debugfs;
    u8 fake_inject_layer[3];
    bool fake_inject_ue;
    u16 fake_inject_count;
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
struct mem_ctl_info {
    struct device dev;
    struct bus_type *bus;
    struct list_head link;
    struct module *owner;
    long unsigned int mtype_cap;
    long unsigned int edac_ctl_cap;
    long unsigned int edac_cap;
    long unsigned int scrub_cap;
    enum scrub_type scrub_mode;
    int (*set_sdram_scrub_rate)(struct mem_ctl_info *, u32);
    int (*get_sdram_scrub_rate)(struct mem_ctl_info *);
    void (*edac_check)(struct mem_ctl_info *);
    long unsigned int (*ctl_page_to_phys)(struct mem_ctl_info *, long unsigned int);
    int mc_idx;
    struct csrow_info **csrows;
    unsigned int nr_csrows;
    unsigned int num_cschannel;
    unsigned int n_layers;
    struct edac_mc_layer *layers;
    bool csbased;
    unsigned int tot_dimms;
    struct dimm_info **dimms;
    struct device *pdev;
    const char *mod_name;
    const char *ctl_name;
    const char *dev_name;
    void *pvt_info;
    long unsigned int start_time;
    u32 ce_noinfo_count;
    u32 ue_noinfo_count;
    u32 ue_mc;
    u32 ce_mc;
    u32 * ce_per_layer[3];
    u32 * ue_per_layer[3];
    struct completion complete;
    const struct mcidev_sysfs_attribute *mc_driver_sysfs_attributes;
    struct delayed_work work;
    struct edac_raw_error_desc error_desc;
    int op_state;
    struct dentry *debugfs;
    u8 fake_inject_layer[3];
    bool fake_inject_ue;
    u16 fake_inject_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct mem_ctl_info {
    struct device dev;
    struct bus_type *bus;
    struct list_head link;
    struct module *owner;
    long unsigned int mtype_cap;
    long unsigned int edac_ctl_cap;
    long unsigned int edac_cap;
    long unsigned int scrub_cap;
    enum scrub_type scrub_mode;
    int (*set_sdram_scrub_rate)(struct mem_ctl_info *, u32);
    int (*get_sdram_scrub_rate)(struct mem_ctl_info *);
    void (*edac_check)(struct mem_ctl_info *);
    long unsigned int (*ctl_page_to_phys)(struct mem_ctl_info *, long unsigned int);
    int mc_idx;
    struct csrow_info **csrows;
    unsigned int nr_csrows;
    unsigned int num_cschannel;
    unsigned int n_layers;
    struct edac_mc_layer *layers;
    bool csbased;
    unsigned int tot_dimms;
    struct dimm_info **dimms;
    struct device *pdev;
    const char *mod_name;
    const char *ctl_name;
    const char *dev_name;
    void *pvt_info;
    long unsigned int start_time;
    u32 ce_noinfo_count;
    u32 ue_noinfo_count;
    u32 ue_mc;
    u32 ce_mc;
    u32 * ce_per_layer[3];
    u32 * ue_per_layer[3];
    struct completion complete;
    const struct mcidev_sysfs_attribute *mc_driver_sysfs_attributes;
    struct delayed_work work;
    struct edac_raw_error_desc error_desc;
    int op_state;
    struct dentry *debugfs;
    u8 fake_inject_layer[3];
    bool fake_inject_ue;
    u16 fake_inject_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct mem_ctl_info {
    struct device dev;
    struct bus_type *bus;
    struct list_head link;
    struct module *owner;
    long unsigned int mtype_cap;
    long unsigned int edac_ctl_cap;
    long unsigned int edac_cap;
    long unsigned int scrub_cap;
    enum scrub_type scrub_mode;
    int (*set_sdram_scrub_rate)(struct mem_ctl_info *, u32);
    int (*get_sdram_scrub_rate)(struct mem_ctl_info *);
    void (*edac_check)(struct mem_ctl_info *);
    long unsigned int (*ctl_page_to_phys)(struct mem_ctl_info *, long unsigned int);
    int mc_idx;
    struct csrow_info **csrows;
    unsigned int nr_csrows;
    unsigned int num_cschannel;
    unsigned int n_layers;
    struct edac_mc_layer *layers;
    bool csbased;
    unsigned int tot_dimms;
    struct dimm_info **dimms;
    struct device *pdev;
    const char *mod_name;
    const char *ctl_name;
    const char *dev_name;
    void *pvt_info;
    long unsigned int start_time;
    u32 ce_noinfo_count;
    u32 ue_noinfo_count;
    u32 ue_mc;
    u32 ce_mc;
    u32 * ce_per_layer[3];
    u32 * ue_per_layer[3];
    struct completion complete;
    const struct mcidev_sysfs_attribute *mc_driver_sysfs_attributes;
    struct delayed_work work;
    struct edac_raw_error_desc error_desc;
    int op_state;
    struct dentry *debugfs;
    u8 fake_inject_layer[3];
    bool fake_inject_ue;
    u16 fake_inject_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct mem_ctl_info {
    struct device dev;
    struct bus_type *bus;
    struct list_head link;
    struct module *owner;
    long unsigned int mtype_cap;
    long unsigned int edac_ctl_cap;
    long unsigned int edac_cap;
    long unsigned int scrub_cap;
    enum scrub_type scrub_mode;
    int (*set_sdram_scrub_rate)(struct mem_ctl_info *, u32);
    int (*get_sdram_scrub_rate)(struct mem_ctl_info *);
    void (*edac_check)(struct mem_ctl_info *);
    long unsigned int (*ctl_page_to_phys)(struct mem_ctl_info *, long unsigned int);
    int mc_idx;
    struct csrow_info **csrows;
    unsigned int nr_csrows;
    unsigned int num_cschannel;
    unsigned int n_layers;
    struct edac_mc_layer *layers;
    bool csbased;
    unsigned int tot_dimms;
    struct dimm_info **dimms;
    struct device *pdev;
    const char *mod_name;
    const char *ctl_name;
    const char *dev_name;
    void *pvt_info;
    long unsigned int start_time;
    u32 ce_noinfo_count;
    u32 ue_noinfo_count;
    u32 ue_mc;
    u32 ce_mc;
    u32 * ce_per_layer[3];
    u32 * ue_per_layer[3];
    struct completion complete;
    const struct mcidev_sysfs_attribute *mc_driver_sysfs_attributes;
    struct delayed_work work;
    struct edac_raw_error_desc error_desc;
    int op_state;
    struct dentry *debugfs;
    u8 fake_inject_layer[3];
    bool fake_inject_ue;
    u16 fake_inject_count;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>const char *mod_ver</code>
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
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>u32 * ce_per_layer[3]</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 * ue_per_layer[3]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
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
<b>Field type changed. </b>
<code>struct bus_type *bus</code> ➡️ <code>const struct bus_type *bus</code>
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
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
