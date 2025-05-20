# Struct: <code>pnv_phb</code>

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
struct pnv_phb {
    struct pci_controller *hose;
    enum pnv_phb_type type;
    enum pnv_phb_model model;
    u64 hub_id;
    u64 opal_id;
    int flags;
    void *regs;
    u64 regs_phys;
    int initialized;
    spinlock_t lock;
    int has_dbgfs;
    struct dentry *dbgfs;
    unsigned int msi_base;
    unsigned int msi32_support;
    struct msi_bitmap msi_bmp;
    int (*msi_setup)(struct pnv_phb *, struct pci_dev *, unsigned int, unsigned int, unsigned int, struct msi_msg *);
    void (*dma_dev_setup)(struct pnv_phb *, struct pci_dev *);
    int (*init_m64)(struct pnv_phb *);
    int (*get_pe_state)(struct pnv_phb *, int);
    void (*freeze_pe)(struct pnv_phb *, int);
    int (*unfreeze_pe)(struct pnv_phb *, int, int);
    struct (anon) ioda;
    unsigned int diag_data_size;
    u8 *diag_data;
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
