# Struct: <code>cxl_service_layer_ops</code>

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
struct cxl_service_layer_ops {
    int (*adapter_regs_init)(struct cxl *, struct pci_dev *);
    int (*invalidate_all)(struct cxl *);
    int (*afu_regs_init)(struct cxl_afu *);
    int (*sanitise_afu_regs)(struct cxl_afu *);
    int (*register_serr_irq)(struct cxl_afu *);
    void (*release_serr_irq)(struct cxl_afu *);
    irqreturn_t (*handle_interrupt)(int, struct cxl_context *, struct cxl_irq_info *);
    irqreturn_t (*fail_irq)(struct cxl_afu *, struct cxl_irq_info *);
    int (*activate_dedicated_process)(struct cxl_afu *);
    int (*attach_afu_directed)(struct cxl_context *, u64, u64);
    int (*attach_dedicated_process)(struct cxl_context *, u64, u64);
    void (*update_dedicated_ivtes)(struct cxl_context *);
    void (*debugfs_add_adapter_regs)(struct cxl *, struct dentry *);
    void (*debugfs_add_afu_regs)(struct cxl_afu *, struct dentry *);
    void (*psl_irq_dump_registers)(struct cxl_context *);
    void (*err_irq_dump_registers)(struct cxl *);
    void (*debugfs_stop_trace)(struct cxl *);
    void (*write_timebase_ctrl)(struct cxl *);
    u64 (*timebase_read)(struct cxl *);
    int capi_mode;
    bool needs_reset_before_disable;
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
