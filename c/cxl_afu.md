# Struct: <code>cxl_afu</code>

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
In <code>armhf</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct cxl_afu {
    struct cxl_afu_native *native;
    struct cxl_afu_guest *guest;
    irq_hw_number_t serr_hwirq;
    unsigned int serr_virq;
    char *psl_irq_name;
    char *err_irq_name;
    void *p2n_mmio;
    phys_addr_t psn_phys;
    u64 pp_size;
    struct cxl *adapter;
    struct device dev;
    struct cdev afu_cdev_s;
    struct cdev afu_cdev_m;
    struct cdev afu_cdev_d;
    struct device *chardev_s;
    struct device *chardev_m;
    struct device *chardev_d;
    struct idr contexts_idr;
    struct dentry *debugfs;
    struct mutex contexts_lock;
    spinlock_t afu_cntl_lock;
    atomic_t configured_state;
    u64 eb_len;
    u64 eb_offset;
    struct bin_attribute attr_eb;
    struct pci_controller *phb;
    int pp_irqs;
    int irqs_max;
    int num_procs;
    int max_procs_virtualised;
    int slice;
    int modes_supported;
    int current_mode;
    int crs_num;
    u64 crs_len;
    u64 crs_offset;
    struct list_head crs;
    enum prefault_modes prefault_mode;
    bool psa;
    bool pp_psa;
    bool enabled;
};
```
</details>
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
