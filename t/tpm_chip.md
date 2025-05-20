# Struct: <code>tpm_chip</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct tpm_chip {
    struct device *pdev;
    struct device dev;
    struct cdev cdev;
    const struct tpm_class_ops *ops;
    unsigned int flags;
    int dev_num;
    char devname[7];
    long unsigned int is_open;
    int time_expired;
    struct mutex tpm_mutex;
    struct tpm_vendor_specific vendor;
    struct dentry **bios_dir;
    const struct attribute_group * groups[2];
    unsigned int groups_cnt;
    acpi_handle acpi_dev_handle;
    char ppi_version[4];
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct tpm_chip {
    struct device dev;
    struct cdev cdev;
    struct rw_semaphore ops_sem;
    const struct tpm_class_ops *ops;
    unsigned int flags;
    int dev_num;
    long unsigned int is_open;
    struct mutex tpm_mutex;
    long unsigned int timeout_a;
    long unsigned int timeout_b;
    long unsigned int timeout_c;
    long unsigned int timeout_d;
    bool timeout_adjusted;
    long unsigned int duration[3];
    bool duration_adjusted;
    struct dentry **bios_dir;
    const struct attribute_group * groups[3];
    unsigned int groups_cnt;
    acpi_handle acpi_dev_handle;
    char ppi_version[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct tpm_chip {
    struct device dev;
    struct cdev cdev;
    struct rw_semaphore ops_sem;
    const struct tpm_class_ops *ops;
    struct tpm_bios_log log;
    struct tpm_chip_seqops bin_log_seqops;
    struct tpm_chip_seqops ascii_log_seqops;
    unsigned int flags;
    int dev_num;
    long unsigned int is_open;
    struct mutex tpm_mutex;
    long unsigned int timeout_a;
    long unsigned int timeout_b;
    long unsigned int timeout_c;
    long unsigned int timeout_d;
    bool timeout_adjusted;
    long unsigned int duration[3];
    bool duration_adjusted;
    struct dentry * bios_dir[3];
    const struct attribute_group * groups[3];
    unsigned int groups_cnt;
    acpi_handle acpi_dev_handle;
    char ppi_version[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct tpm_chip {
    struct device dev;
    struct device devs;
    struct cdev cdev;
    struct cdev cdevs;
    struct rw_semaphore ops_sem;
    const struct tpm_class_ops *ops;
    struct tpm_bios_log log;
    struct tpm_chip_seqops bin_log_seqops;
    struct tpm_chip_seqops ascii_log_seqops;
    unsigned int flags;
    int dev_num;
    long unsigned int is_open;
    struct mutex tpm_mutex;
    long unsigned int timeout_a;
    long unsigned int timeout_b;
    long unsigned int timeout_c;
    long unsigned int timeout_d;
    bool timeout_adjusted;
    long unsigned int duration[3];
    bool duration_adjusted;
    struct dentry * bios_dir[3];
    const struct attribute_group * groups[3];
    unsigned int groups_cnt;
    u16 active_banks[7];
    acpi_handle acpi_dev_handle;
    char ppi_version[4];
    struct tpm_space work_space;
    u32 nr_commands;
    u32 *cc_attrs_tbl;
    int locality;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct tpm_chip {
    struct device dev;
    struct device devs;
    struct cdev cdev;
    struct cdev cdevs;
    struct rw_semaphore ops_sem;
    const struct tpm_class_ops *ops;
    struct tpm_bios_log log;
    struct tpm_chip_seqops bin_log_seqops;
    struct tpm_chip_seqops ascii_log_seqops;
    unsigned int flags;
    int dev_num;
    long unsigned int is_open;
    struct mutex tpm_mutex;
    long unsigned int timeout_a;
    long unsigned int timeout_b;
    long unsigned int timeout_c;
    long unsigned int timeout_d;
    bool timeout_adjusted;
    long unsigned int duration[3];
    bool duration_adjusted;
    struct dentry * bios_dir[3];
    const struct attribute_group * groups[3];
    unsigned int groups_cnt;
    u16 active_banks[7];
    acpi_handle acpi_dev_handle;
    char ppi_version[4];
    struct tpm_space work_space;
    u32 nr_commands;
    u32 *cc_attrs_tbl;
    int locality;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct tpm_chip {
    struct device dev;
    struct device devs;
    struct cdev cdev;
    struct cdev cdevs;
    struct rw_semaphore ops_sem;
    const struct tpm_class_ops *ops;
    struct tpm_bios_log log;
    struct tpm_chip_seqops bin_log_seqops;
    struct tpm_chip_seqops ascii_log_seqops;
    unsigned int flags;
    int dev_num;
    long unsigned int is_open;
    char hwrng_name[64];
    struct hwrng hwrng;
    struct mutex tpm_mutex;
    long unsigned int timeout_a;
    long unsigned int timeout_b;
    long unsigned int timeout_c;
    long unsigned int timeout_d;
    bool timeout_adjusted;
    long unsigned int duration[4];
    bool duration_adjusted;
    struct dentry * bios_dir[3];
    const struct attribute_group * groups[3];
    unsigned int groups_cnt;
    u16 active_banks[7];
    acpi_handle acpi_dev_handle;
    char ppi_version[4];
    struct tpm_space work_space;
    u32 nr_commands;
    u32 *cc_attrs_tbl;
    int locality;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct tpm_chip {
    struct device dev;
    struct device devs;
    struct cdev cdev;
    struct cdev cdevs;
    struct rw_semaphore ops_sem;
    const struct tpm_class_ops *ops;
    struct tpm_bios_log log;
    struct tpm_chip_seqops bin_log_seqops;
    struct tpm_chip_seqops ascii_log_seqops;
    unsigned int flags;
    int dev_num;
    long unsigned int is_open;
    char hwrng_name[64];
    struct hwrng hwrng;
    struct mutex tpm_mutex;
    long unsigned int timeout_a;
    long unsigned int timeout_b;
    long unsigned int timeout_c;
    long unsigned int timeout_d;
    bool timeout_adjusted;
    long unsigned int duration[4];
    bool duration_adjusted;
    struct dentry * bios_dir[3];
    const struct attribute_group * groups[3];
    unsigned int groups_cnt;
    u16 active_banks[7];
    acpi_handle acpi_dev_handle;
    char ppi_version[4];
    struct tpm_space work_space;
    u32 nr_commands;
    u32 *cc_attrs_tbl;
    int locality;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct tpm_chip {
    struct device dev;
    struct device devs;
    struct cdev cdev;
    struct cdev cdevs;
    struct rw_semaphore ops_sem;
    const struct tpm_class_ops *ops;
    struct tpm_bios_log log;
    struct tpm_chip_seqops bin_log_seqops;
    struct tpm_chip_seqops ascii_log_seqops;
    unsigned int flags;
    int dev_num;
    long unsigned int is_open;
    char hwrng_name[64];
    struct hwrng hwrng;
    struct mutex tpm_mutex;
    long unsigned int timeout_a;
    long unsigned int timeout_b;
    long unsigned int timeout_c;
    long unsigned int timeout_d;
    bool timeout_adjusted;
    long unsigned int duration[4];
    bool duration_adjusted;
    struct dentry * bios_dir[3];
    const struct attribute_group * groups[3];
    unsigned int groups_cnt;
    u32 nr_allocated_banks;
    struct tpm_bank_info *allocated_banks;
    acpi_handle acpi_dev_handle;
    char ppi_version[4];
    struct tpm_space work_space;
    u32 last_cc;
    u32 nr_commands;
    u32 *cc_attrs_tbl;
    int locality;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct tpm_chip {
    struct device dev;
    struct device devs;
    struct cdev cdev;
    struct cdev cdevs;
    struct rw_semaphore ops_sem;
    const struct tpm_class_ops *ops;
    struct tpm_bios_log log;
    struct tpm_chip_seqops bin_log_seqops;
    struct tpm_chip_seqops ascii_log_seqops;
    unsigned int flags;
    int dev_num;
    long unsigned int is_open;
    char hwrng_name[64];
    struct hwrng hwrng;
    struct mutex tpm_mutex;
    long unsigned int timeout_a;
    long unsigned int timeout_b;
    long unsigned int timeout_c;
    long unsigned int timeout_d;
    bool timeout_adjusted;
    long unsigned int duration[4];
    bool duration_adjusted;
    struct dentry * bios_dir[3];
    const struct attribute_group * groups[3];
    unsigned int groups_cnt;
    u32 nr_allocated_banks;
    struct tpm_bank_info *allocated_banks;
    acpi_handle acpi_dev_handle;
    char ppi_version[4];
    struct tpm_space work_space;
    u32 last_cc;
    u32 nr_commands;
    u32 *cc_attrs_tbl;
    int locality;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct tpm_chip {
    struct device dev;
    struct device devs;
    struct cdev cdev;
    struct cdev cdevs;
    struct rw_semaphore ops_sem;
    const struct tpm_class_ops *ops;
    struct tpm_bios_log log;
    struct tpm_chip_seqops bin_log_seqops;
    struct tpm_chip_seqops ascii_log_seqops;
    unsigned int flags;
    int dev_num;
    long unsigned int is_open;
    char hwrng_name[64];
    struct hwrng hwrng;
    struct mutex tpm_mutex;
    long unsigned int timeout_a;
    long unsigned int timeout_b;
    long unsigned int timeout_c;
    long unsigned int timeout_d;
    bool timeout_adjusted;
    long unsigned int duration[4];
    bool duration_adjusted;
    struct dentry * bios_dir[3];
    const struct attribute_group * groups[3];
    unsigned int groups_cnt;
    u32 nr_allocated_banks;
    struct tpm_bank_info *allocated_banks;
    acpi_handle acpi_dev_handle;
    char ppi_version[4];
    struct tpm_space work_space;
    u32 last_cc;
    u32 nr_commands;
    u32 *cc_attrs_tbl;
    int locality;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct tpm_chip {
    struct device dev;
    struct device devs;
    struct cdev cdev;
    struct cdev cdevs;
    struct rw_semaphore ops_sem;
    const struct tpm_class_ops *ops;
    struct tpm_bios_log log;
    struct tpm_chip_seqops bin_log_seqops;
    struct tpm_chip_seqops ascii_log_seqops;
    unsigned int flags;
    int dev_num;
    long unsigned int is_open;
    char hwrng_name[64];
    struct hwrng hwrng;
    struct mutex tpm_mutex;
    long unsigned int timeout_a;
    long unsigned int timeout_b;
    long unsigned int timeout_c;
    long unsigned int timeout_d;
    bool timeout_adjusted;
    long unsigned int duration[4];
    bool duration_adjusted;
    struct dentry * bios_dir[3];
    const struct attribute_group * groups[3];
    unsigned int groups_cnt;
    u32 nr_allocated_banks;
    struct tpm_bank_info *allocated_banks;
    acpi_handle acpi_dev_handle;
    char ppi_version[4];
    struct tpm_space work_space;
    u32 last_cc;
    u32 nr_commands;
    u32 *cc_attrs_tbl;
    int locality;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct tpm_chip {
    struct device dev;
    struct device devs;
    struct cdev cdev;
    struct cdev cdevs;
    struct rw_semaphore ops_sem;
    const struct tpm_class_ops *ops;
    struct tpm_bios_log log;
    struct tpm_chip_seqops bin_log_seqops;
    struct tpm_chip_seqops ascii_log_seqops;
    unsigned int flags;
    int dev_num;
    long unsigned int is_open;
    char hwrng_name[64];
    struct hwrng hwrng;
    struct mutex tpm_mutex;
    long unsigned int timeout_a;
    long unsigned int timeout_b;
    long unsigned int timeout_c;
    long unsigned int timeout_d;
    bool timeout_adjusted;
    long unsigned int duration[4];
    bool duration_adjusted;
    struct dentry * bios_dir[3];
    const struct attribute_group * groups[8];
    unsigned int groups_cnt;
    u32 nr_allocated_banks;
    struct tpm_bank_info *allocated_banks;
    acpi_handle acpi_dev_handle;
    char ppi_version[4];
    struct tpm_space work_space;
    u32 last_cc;
    u32 nr_commands;
    u32 *cc_attrs_tbl;
    int locality;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct tpm_chip {
    struct device dev;
    struct device devs;
    struct cdev cdev;
    struct cdev cdevs;
    struct rw_semaphore ops_sem;
    const struct tpm_class_ops *ops;
    struct tpm_bios_log log;
    struct tpm_chip_seqops bin_log_seqops;
    struct tpm_chip_seqops ascii_log_seqops;
    unsigned int flags;
    int dev_num;
    long unsigned int is_open;
    char hwrng_name[64];
    struct hwrng hwrng;
    struct mutex tpm_mutex;
    long unsigned int timeout_a;
    long unsigned int timeout_b;
    long unsigned int timeout_c;
    long unsigned int timeout_d;
    bool timeout_adjusted;
    long unsigned int duration[4];
    bool duration_adjusted;
    struct dentry * bios_dir[3];
    const struct attribute_group * groups[8];
    unsigned int groups_cnt;
    u32 nr_allocated_banks;
    struct tpm_bank_info *allocated_banks;
    acpi_handle acpi_dev_handle;
    char ppi_version[4];
    struct tpm_space work_space;
    u32 last_cc;
    u32 nr_commands;
    u32 *cc_attrs_tbl;
    int locality;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct tpm_chip {
    struct device dev;
    struct device devs;
    struct cdev cdev;
    struct cdev cdevs;
    struct rw_semaphore ops_sem;
    const struct tpm_class_ops *ops;
    struct tpm_bios_log log;
    struct tpm_chip_seqops bin_log_seqops;
    struct tpm_chip_seqops ascii_log_seqops;
    unsigned int flags;
    int dev_num;
    long unsigned int is_open;
    char hwrng_name[64];
    struct hwrng hwrng;
    struct mutex tpm_mutex;
    long unsigned int timeout_a;
    long unsigned int timeout_b;
    long unsigned int timeout_c;
    long unsigned int timeout_d;
    bool timeout_adjusted;
    long unsigned int duration[4];
    bool duration_adjusted;
    struct dentry * bios_dir[3];
    const struct attribute_group * groups[8];
    unsigned int groups_cnt;
    u32 nr_allocated_banks;
    struct tpm_bank_info *allocated_banks;
    acpi_handle acpi_dev_handle;
    char ppi_version[4];
    struct tpm_space work_space;
    u32 last_cc;
    u32 nr_commands;
    u32 *cc_attrs_tbl;
    int locality;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct tpm_chip {
    struct device dev;
    struct device devs;
    struct cdev cdev;
    struct cdev cdevs;
    struct rw_semaphore ops_sem;
    const struct tpm_class_ops *ops;
    struct tpm_bios_log log;
    struct tpm_chip_seqops bin_log_seqops;
    struct tpm_chip_seqops ascii_log_seqops;
    unsigned int flags;
    int dev_num;
    long unsigned int is_open;
    char hwrng_name[64];
    struct hwrng hwrng;
    struct mutex tpm_mutex;
    long unsigned int timeout_a;
    long unsigned int timeout_b;
    long unsigned int timeout_c;
    long unsigned int timeout_d;
    bool timeout_adjusted;
    long unsigned int duration[4];
    bool duration_adjusted;
    struct dentry * bios_dir[3];
    const struct attribute_group * groups[8];
    unsigned int groups_cnt;
    u32 nr_allocated_banks;
    struct tpm_bank_info *allocated_banks;
    acpi_handle acpi_dev_handle;
    char ppi_version[4];
    struct tpm_space work_space;
    u32 last_cc;
    u32 nr_commands;
    u32 *cc_attrs_tbl;
    int locality;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct tpm_chip {
    struct device dev;
    struct device devs;
    struct cdev cdev;
    struct cdev cdevs;
    struct rw_semaphore ops_sem;
    const struct tpm_class_ops *ops;
    struct tpm_bios_log log;
    struct tpm_chip_seqops bin_log_seqops;
    struct tpm_chip_seqops ascii_log_seqops;
    unsigned int flags;
    int dev_num;
    long unsigned int is_open;
    char hwrng_name[64];
    struct hwrng hwrng;
    struct mutex tpm_mutex;
    long unsigned int timeout_a;
    long unsigned int timeout_b;
    long unsigned int timeout_c;
    long unsigned int timeout_d;
    bool timeout_adjusted;
    long unsigned int duration[4];
    bool duration_adjusted;
    struct dentry * bios_dir[3];
    const struct attribute_group * groups[8];
    unsigned int groups_cnt;
    u32 nr_allocated_banks;
    struct tpm_bank_info *allocated_banks;
    acpi_handle acpi_dev_handle;
    char ppi_version[4];
    struct tpm_space work_space;
    u32 last_cc;
    u32 nr_commands;
    u32 *cc_attrs_tbl;
    int locality;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct tpm_chip {
    struct device dev;
    struct device devs;
    struct cdev cdev;
    struct cdev cdevs;
    struct rw_semaphore ops_sem;
    const struct tpm_class_ops *ops;
    struct tpm_bios_log log;
    struct tpm_chip_seqops bin_log_seqops;
    struct tpm_chip_seqops ascii_log_seqops;
    unsigned int flags;
    int dev_num;
    long unsigned int is_open;
    char hwrng_name[64];
    struct hwrng hwrng;
    struct mutex tpm_mutex;
    long unsigned int timeout_a;
    long unsigned int timeout_b;
    long unsigned int timeout_c;
    long unsigned int timeout_d;
    bool timeout_adjusted;
    long unsigned int duration[4];
    bool duration_adjusted;
    struct dentry * bios_dir[3];
    const struct attribute_group * groups[8];
    unsigned int groups_cnt;
    u32 nr_allocated_banks;
    struct tpm_bank_info *allocated_banks;
    acpi_handle acpi_dev_handle;
    char ppi_version[4];
    struct tpm_space work_space;
    u32 last_cc;
    u32 nr_commands;
    u32 *cc_attrs_tbl;
    int locality;
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
struct tpm_chip {
    struct device dev;
    struct device devs;
    struct cdev cdev;
    struct cdev cdevs;
    struct rw_semaphore ops_sem;
    const struct tpm_class_ops *ops;
    struct tpm_bios_log log;
    struct tpm_chip_seqops bin_log_seqops;
    struct tpm_chip_seqops ascii_log_seqops;
    unsigned int flags;
    int dev_num;
    long unsigned int is_open;
    char hwrng_name[64];
    struct hwrng hwrng;
    struct mutex tpm_mutex;
    long unsigned int timeout_a;
    long unsigned int timeout_b;
    long unsigned int timeout_c;
    long unsigned int timeout_d;
    bool timeout_adjusted;
    long unsigned int duration[4];
    bool duration_adjusted;
    struct dentry * bios_dir[3];
    const struct attribute_group * groups[3];
    unsigned int groups_cnt;
    u32 nr_allocated_banks;
    struct tpm_bank_info *allocated_banks;
    acpi_handle acpi_dev_handle;
    char ppi_version[4];
    struct tpm_space work_space;
    u32 last_cc;
    u32 nr_commands;
    u32 *cc_attrs_tbl;
    int locality;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct tpm_chip {
    struct device dev;
    struct device devs;
    struct cdev cdev;
    struct cdev cdevs;
    struct rw_semaphore ops_sem;
    const struct tpm_class_ops *ops;
    struct tpm_bios_log log;
    struct tpm_chip_seqops bin_log_seqops;
    struct tpm_chip_seqops ascii_log_seqops;
    unsigned int flags;
    int dev_num;
    long unsigned int is_open;
    char hwrng_name[64];
    struct hwrng hwrng;
    struct mutex tpm_mutex;
    long unsigned int timeout_a;
    long unsigned int timeout_b;
    long unsigned int timeout_c;
    long unsigned int timeout_d;
    bool timeout_adjusted;
    long unsigned int duration[4];
    bool duration_adjusted;
    struct dentry * bios_dir[3];
    const struct attribute_group * groups[3];
    unsigned int groups_cnt;
    u32 nr_allocated_banks;
    struct tpm_bank_info *allocated_banks;
    struct tpm_space work_space;
    u32 last_cc;
    u32 nr_commands;
    u32 *cc_attrs_tbl;
    int locality;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct tpm_chip {
    struct device dev;
    struct device devs;
    struct cdev cdev;
    struct cdev cdevs;
    struct rw_semaphore ops_sem;
    const struct tpm_class_ops *ops;
    struct tpm_bios_log log;
    struct tpm_chip_seqops bin_log_seqops;
    struct tpm_chip_seqops ascii_log_seqops;
    unsigned int flags;
    int dev_num;
    long unsigned int is_open;
    char hwrng_name[64];
    struct hwrng hwrng;
    struct mutex tpm_mutex;
    long unsigned int timeout_a;
    long unsigned int timeout_b;
    long unsigned int timeout_c;
    long unsigned int timeout_d;
    bool timeout_adjusted;
    long unsigned int duration[4];
    bool duration_adjusted;
    struct dentry * bios_dir[3];
    const struct attribute_group * groups[3];
    unsigned int groups_cnt;
    u32 nr_allocated_banks;
    struct tpm_bank_info *allocated_banks;
    struct tpm_space work_space;
    u32 last_cc;
    u32 nr_commands;
    u32 *cc_attrs_tbl;
    int locality;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct tpm_chip {
    struct device dev;
    struct device devs;
    struct cdev cdev;
    struct cdev cdevs;
    struct rw_semaphore ops_sem;
    const struct tpm_class_ops *ops;
    struct tpm_bios_log log;
    struct tpm_chip_seqops bin_log_seqops;
    struct tpm_chip_seqops ascii_log_seqops;
    unsigned int flags;
    int dev_num;
    long unsigned int is_open;
    char hwrng_name[64];
    struct hwrng hwrng;
    struct mutex tpm_mutex;
    long unsigned int timeout_a;
    long unsigned int timeout_b;
    long unsigned int timeout_c;
    long unsigned int timeout_d;
    bool timeout_adjusted;
    long unsigned int duration[4];
    bool duration_adjusted;
    struct dentry * bios_dir[3];
    const struct attribute_group * groups[3];
    unsigned int groups_cnt;
    u32 nr_allocated_banks;
    struct tpm_bank_info *allocated_banks;
    struct tpm_space work_space;
    u32 last_cc;
    u32 nr_commands;
    u32 *cc_attrs_tbl;
    int locality;
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
struct tpm_chip {
    struct device dev;
    struct device devs;
    struct cdev cdev;
    struct cdev cdevs;
    struct rw_semaphore ops_sem;
    const struct tpm_class_ops *ops;
    struct tpm_bios_log log;
    struct tpm_chip_seqops bin_log_seqops;
    struct tpm_chip_seqops ascii_log_seqops;
    unsigned int flags;
    int dev_num;
    long unsigned int is_open;
    char hwrng_name[64];
    struct hwrng hwrng;
    struct mutex tpm_mutex;
    long unsigned int timeout_a;
    long unsigned int timeout_b;
    long unsigned int timeout_c;
    long unsigned int timeout_d;
    bool timeout_adjusted;
    long unsigned int duration[4];
    bool duration_adjusted;
    struct dentry * bios_dir[3];
    const struct attribute_group * groups[3];
    unsigned int groups_cnt;
    u32 nr_allocated_banks;
    struct tpm_bank_info *allocated_banks;
    acpi_handle acpi_dev_handle;
    char ppi_version[4];
    struct tpm_space work_space;
    u32 last_cc;
    u32 nr_commands;
    u32 *cc_attrs_tbl;
    int locality;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct tpm_chip {
    struct device dev;
    struct device devs;
    struct cdev cdev;
    struct cdev cdevs;
    struct rw_semaphore ops_sem;
    const struct tpm_class_ops *ops;
    struct tpm_bios_log log;
    struct tpm_chip_seqops bin_log_seqops;
    struct tpm_chip_seqops ascii_log_seqops;
    unsigned int flags;
    int dev_num;
    long unsigned int is_open;
    char hwrng_name[64];
    struct hwrng hwrng;
    struct mutex tpm_mutex;
    long unsigned int timeout_a;
    long unsigned int timeout_b;
    long unsigned int timeout_c;
    long unsigned int timeout_d;
    bool timeout_adjusted;
    long unsigned int duration[4];
    bool duration_adjusted;
    struct dentry * bios_dir[3];
    const struct attribute_group * groups[3];
    unsigned int groups_cnt;
    u32 nr_allocated_banks;
    struct tpm_bank_info *allocated_banks;
    acpi_handle acpi_dev_handle;
    char ppi_version[4];
    struct tpm_space work_space;
    u32 last_cc;
    u32 nr_commands;
    u32 *cc_attrs_tbl;
    int locality;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct tpm_chip {
    struct device dev;
    struct device devs;
    struct cdev cdev;
    struct cdev cdevs;
    struct rw_semaphore ops_sem;
    const struct tpm_class_ops *ops;
    struct tpm_bios_log log;
    struct tpm_chip_seqops bin_log_seqops;
    struct tpm_chip_seqops ascii_log_seqops;
    unsigned int flags;
    int dev_num;
    long unsigned int is_open;
    char hwrng_name[64];
    struct hwrng hwrng;
    struct mutex tpm_mutex;
    long unsigned int timeout_a;
    long unsigned int timeout_b;
    long unsigned int timeout_c;
    long unsigned int timeout_d;
    bool timeout_adjusted;
    long unsigned int duration[4];
    bool duration_adjusted;
    struct dentry * bios_dir[3];
    const struct attribute_group * groups[3];
    unsigned int groups_cnt;
    u32 nr_allocated_banks;
    struct tpm_bank_info *allocated_banks;
    acpi_handle acpi_dev_handle;
    char ppi_version[4];
    struct tpm_space work_space;
    u32 last_cc;
    u32 nr_commands;
    u32 *cc_attrs_tbl;
    int locality;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct tpm_chip {
    struct device dev;
    struct device devs;
    struct cdev cdev;
    struct cdev cdevs;
    struct rw_semaphore ops_sem;
    const struct tpm_class_ops *ops;
    struct tpm_bios_log log;
    struct tpm_chip_seqops bin_log_seqops;
    struct tpm_chip_seqops ascii_log_seqops;
    unsigned int flags;
    int dev_num;
    long unsigned int is_open;
    char hwrng_name[64];
    struct hwrng hwrng;
    struct mutex tpm_mutex;
    long unsigned int timeout_a;
    long unsigned int timeout_b;
    long unsigned int timeout_c;
    long unsigned int timeout_d;
    bool timeout_adjusted;
    long unsigned int duration[4];
    bool duration_adjusted;
    struct dentry * bios_dir[3];
    const struct attribute_group * groups[3];
    unsigned int groups_cnt;
    u32 nr_allocated_banks;
    struct tpm_bank_info *allocated_banks;
    acpi_handle acpi_dev_handle;
    char ppi_version[4];
    struct tpm_space work_space;
    u32 last_cc;
    u32 nr_commands;
    u32 *cc_attrs_tbl;
    int locality;
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
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct rw_semaphore ops_sem</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int timeout_a</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int timeout_b</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int timeout_c</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int timeout_d</code>
</li>
<li>
<b>Field added. </b>
<code>bool timeout_adjusted</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int duration[3]</code>
</li>
<li>
<b>Field added. </b>
<code>bool duration_adjusted</code>
</li>
<li>
<b>Field removed. </b>
<code>struct device *pdev</code>
</li>
<li>
<b>Field removed. </b>
<code>char devname[7]</code>
</li>
<li>
<b>Field removed. </b>
<code>int time_expired</code>
</li>
<li>
<b>Field removed. </b>
<code>struct tpm_vendor_specific vendor</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head list</code>
</li>
<li>
<b>Field type changed. </b>
<code>const struct attribute_group * groups[2]</code> ➡️ <code>const struct attribute_group * groups[3]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct tpm_bios_log log</code>
</li>
<li>
<b>Field added. </b>
<code>struct tpm_chip_seqops bin_log_seqops</code>
</li>
<li>
<b>Field added. </b>
<code>struct tpm_chip_seqops ascii_log_seqops</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct dentry **bios_dir</code> ➡️ <code>struct dentry * bios_dir[3]</code>
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
<code>struct device devs</code>
</li>
<li>
<b>Field added. </b>
<code>struct cdev cdevs</code>
</li>
<li>
<b>Field added. </b>
<code>u16 active_banks[7]</code>
</li>
<li>
<b>Field added. </b>
<code>struct tpm_space work_space</code>
</li>
<li>
<b>Field added. </b>
<code>u32 nr_commands</code>
</li>
<li>
<b>Field added. </b>
<code>u32 *cc_attrs_tbl</code>
</li>
<li>
<b>Field added. </b>
<code>int locality</code>
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
<code>char hwrng_name[64]</code>
</li>
<li>
<b>Field added. </b>
<code>struct hwrng hwrng</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int duration[3]</code> ➡️ <code>long unsigned int duration[4]</code>
</li>
</ul>
</details>
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
<code>u32 nr_allocated_banks</code>
</li>
<li>
<b>Field added. </b>
<code>struct tpm_bank_info *allocated_banks</code>
</li>
<li>
<b>Field added. </b>
<code>u32 last_cc</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 active_banks[7]</code>
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
<b>Field type changed. </b>
<code>const struct attribute_group * groups[3]</code> ➡️ <code>const struct attribute_group * groups[8]</code>
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
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
<b>Arch</b>
<ul>
<li>
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>acpi_handle acpi_dev_handle</code>
</li>
<li>
<b>Field removed. </b>
<code>char ppi_version[4]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>acpi_handle acpi_dev_handle</code>
</li>
<li>
<b>Field removed. </b>
<code>char ppi_version[4]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>acpi_handle acpi_dev_handle</code>
</li>
<li>
<b>Field removed. </b>
<code>char ppi_version[4]</code>
</li>
</ul>
</details>
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
