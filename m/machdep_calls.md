# Struct: <code>machdep_calls</code>

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
struct machdep_calls {
    char *name;
    void (*iommu_save)();
    void (*iommu_restore)();
    long unsigned int (*memory_block_size)();
    void (*dma_set_mask)(struct device *, u64);
    int (*probe)();
    void (*setup_arch)();
    void (*show_cpuinfo)(struct seq_file *);
    void (*show_percpuinfo)(struct seq_file *, int);
    long unsigned int (*get_proc_freq)(unsigned int);
    void (*init_IRQ)();
    unsigned int (*get_irq)();
    void (*pcibios_fixup)();
    void (*pci_irq_fixup)(struct pci_dev *);
    int (*pcibios_root_bridge_prepare)(struct pci_host_bridge *);
    int (*pci_setup_phb)(struct pci_controller *);
    volatile void(*)(char *) *restart;
    volatile void(*)() *halt;
    void (*panic)(char *);
    void (*cpu_die)();
    long int (*time_init)();
    int (*set_rtc_time)(struct rtc_time *);
    void (*get_rtc_time)(struct rtc_time *);
    time64_t (*get_boot_time)();
    unsigned char (*rtc_read_val)(int);
    void (*rtc_write_val)(int, unsigned char);
    void (*calibrate_decr)();
    void (*progress)(char *, short unsigned int);
    void (*log_error)(char *, unsigned int, int);
    unsigned char (*nvram_read_val)(int);
    void (*nvram_write_val)(int, unsigned char);
    ssize_t (*nvram_write)(char *, size_t, loff_t *);
    ssize_t (*nvram_read)(char *, size_t, loff_t *);
    ssize_t (*nvram_size)();
    void (*nvram_sync)();
    int (*system_reset_exception)(struct pt_regs *);
    int (*machine_check_exception)(struct pt_regs *);
    int (*handle_hmi_exception)(struct pt_regs *);
    int (*hmi_exception_early)(struct pt_regs *);
    long int (*machine_check_early)(struct pt_regs *);
    bool (*mce_check_early_recovery)(struct pt_regs *);
    long int (*feature_call)(unsigned int, void);
    int (*pci_get_legacy_ide_irq)(struct pci_dev *, int);
    pgprot_t (*phys_mem_access_prot)(struct file *, long unsigned int, long unsigned int, pgprot_t);
    void (*power_save)();
    void (*enable_pmcs)();
    int (*set_dabr)(long unsigned int, long unsigned int);
    int (*set_dawr)(long unsigned int, long unsigned int);
    int (*pci_exclude_device)(struct pci_controller *, unsigned char, unsigned char);
    void (*pcibios_fixup_resources)(struct pci_dev *);
    void (*pcibios_fixup_bus)(struct pci_bus *);
    void (*pcibios_fixup_phb)(struct pci_controller *);
    void (*pcibios_bus_add_device)(struct pci_dev *);
    resource_size_t (*pcibios_default_alignment)();
    void (*pcibios_fixup_sriov)(struct pci_dev *);
    resource_size_t (*pcibios_iov_resource_alignment)(struct pci_dev *, int);
    int (*pcibios_sriov_enable)(struct pci_dev *, u16);
    int (*pcibios_sriov_disable)(struct pci_dev *);
    void (*machine_shutdown)();
    void (*kexec_cpu_down)(int, int);
    int (*machine_kexec_prepare)(struct kimage *);
    void (*machine_kexec)(struct kimage *);
    void (*suspend_disable_irqs)();
    void (*suspend_enable_irqs)();
    int (*suspend_disable_cpu)();
    ssize_t (*cpu_probe)(const char *, size_t);
    ssize_t (*cpu_release)(const char *, size_t);
    int (*get_random_seed)(long unsigned int *);
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
