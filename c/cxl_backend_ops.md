# Struct: <code>cxl_backend_ops</code>

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
struct cxl_backend_ops {
    struct module *module;
    int (*adapter_reset)(struct cxl *);
    int (*alloc_one_irq)(struct cxl *);
    void (*release_one_irq)(struct cxl *, int);
    int (*alloc_irq_ranges)(struct cxl_irq_ranges *, struct cxl *, unsigned int);
    void (*release_irq_ranges)(struct cxl_irq_ranges *, struct cxl *);
    int (*setup_irq)(struct cxl *, unsigned int, unsigned int);
    irqreturn_t (*handle_psl_slice_error)(struct cxl_context *, u64, u64);
    irqreturn_t (*psl_interrupt)(int, void *);
    int (*ack_irq)(struct cxl_context *, u64, u64);
    void (*irq_wait)(struct cxl_context *);
    int (*attach_process)(struct cxl_context *, bool, u64, u64);
    int (*detach_process)(struct cxl_context *);
    void (*update_ivtes)(struct cxl_context *);
    bool (*support_attributes)(const char *, enum cxl_attrs);
    bool (*link_ok)(struct cxl *, struct cxl_afu *);
    void (*release_afu)(struct device *);
    ssize_t (*afu_read_err_buffer)(struct cxl_afu *, char *, loff_t, size_t);
    int (*afu_check_and_enable)(struct cxl_afu *);
    int (*afu_activate_mode)(struct cxl_afu *, int);
    int (*afu_deactivate_mode)(struct cxl_afu *, int);
    int (*afu_reset)(struct cxl_afu *);
    int (*afu_cr_read8)(struct cxl_afu *, int, u64, u8 *);
    int (*afu_cr_read16)(struct cxl_afu *, int, u64, u16 *);
    int (*afu_cr_read32)(struct cxl_afu *, int, u64, u32 *);
    int (*afu_cr_read64)(struct cxl_afu *, int, u64, u64 *);
    int (*afu_cr_write8)(struct cxl_afu *, int, u64, u8);
    int (*afu_cr_write16)(struct cxl_afu *, int, u64, u16);
    int (*afu_cr_write32)(struct cxl_afu *, int, u64, u32);
    ssize_t (*read_adapter_vpd)(struct cxl *, void *, size_t);
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
