# Struct: <code>amd_iommu</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct amd_iommu {
    struct list_head list;
    int index;
    spinlock_t lock;
    struct pci_dev *dev;
    struct pci_dev *root_pdev;
    u64 mmio_phys;
    u64 mmio_phys_end;
    u8 *mmio_base;
    u32 cap;
    u8 acpi_flags;
    u64 features;
    bool is_iommu_v2;
    u16 devid;
    u16 cap_ptr;
    u16 pci_seg;
    u64 exclusion_start;
    u64 exclusion_length;
    u8 *cmd_buf;
    u8 *evt_buf;
    u8 *ppr_log;
    bool int_enabled;
    bool need_sync;
    struct device *iommu_dev;
    u32 stored_addr_lo;
    u32 stored_addr_hi;
    u32 stored_l1[108];
    u32 stored_l2[131];
    u8 max_banks;
    u8 max_counters;
    struct irq_domain *ir_domain;
    struct irq_domain *msi_domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct amd_iommu {
    struct list_head list;
    int index;
    spinlock_t lock;
    struct pci_dev *dev;
    struct pci_dev *root_pdev;
    u64 mmio_phys;
    u64 mmio_phys_end;
    u8 *mmio_base;
    u32 cap;
    u8 acpi_flags;
    u64 features;
    bool is_iommu_v2;
    u16 devid;
    u16 cap_ptr;
    u16 pci_seg;
    u64 exclusion_start;
    u64 exclusion_length;
    u8 *cmd_buf;
    u8 *evt_buf;
    u8 *ppr_log;
    bool int_enabled;
    bool need_sync;
    struct device *iommu_dev;
    u32 stored_addr_lo;
    u32 stored_addr_hi;
    u32 stored_l1[108];
    u32 stored_l2[131];
    u8 max_banks;
    u8 max_counters;
    struct irq_domain *ir_domain;
    struct irq_domain *msi_domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct amd_iommu {
    struct list_head list;
    int index;
    spinlock_t lock;
    struct pci_dev *dev;
    struct pci_dev *root_pdev;
    u64 mmio_phys;
    u64 mmio_phys_end;
    u8 *mmio_base;
    u32 cap;
    u8 acpi_flags;
    u64 features;
    bool is_iommu_v2;
    u16 devid;
    u16 cap_ptr;
    u16 pci_seg;
    u64 exclusion_start;
    u64 exclusion_length;
    u8 *cmd_buf;
    u8 *evt_buf;
    u8 *ppr_log;
    u8 *ga_log;
    u8 *ga_log_tail;
    bool int_enabled;
    bool need_sync;
    struct device *iommu_dev;
    u32 stored_addr_lo;
    u32 stored_addr_hi;
    u32 stored_l1[108];
    u32 stored_l2[131];
    u8 max_banks;
    u8 max_counters;
    struct irq_domain *ir_domain;
    struct irq_domain *msi_domain;
    struct amd_irte_ops *irte_ops;
    volatile u64 cmd_sem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct amd_iommu {
    struct list_head list;
    int index;
    spinlock_t lock;
    struct pci_dev *dev;
    struct pci_dev *root_pdev;
    u64 mmio_phys;
    u64 mmio_phys_end;
    u8 *mmio_base;
    u32 cap;
    u8 acpi_flags;
    u64 features;
    bool is_iommu_v2;
    u16 devid;
    u16 cap_ptr;
    u16 pci_seg;
    u64 exclusion_start;
    u64 exclusion_length;
    u8 *cmd_buf;
    u32 cmd_buf_head;
    u32 cmd_buf_tail;
    u8 *evt_buf;
    u8 *ppr_log;
    u8 *ga_log;
    u8 *ga_log_tail;
    bool int_enabled;
    bool need_sync;
    struct iommu_device iommu;
    u32 stored_addr_lo;
    u32 stored_addr_hi;
    u32 stored_l1[108];
    u32 stored_l2[131];
    u8 max_banks;
    u8 max_counters;
    struct irq_domain *ir_domain;
    struct irq_domain *msi_domain;
    struct amd_irte_ops *irte_ops;
    volatile u64 cmd_sem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct amd_iommu {
    struct list_head list;
    int index;
    spinlock_t lock;
    struct pci_dev *dev;
    struct pci_dev *root_pdev;
    u64 mmio_phys;
    u64 mmio_phys_end;
    u8 *mmio_base;
    u32 cap;
    u8 acpi_flags;
    u64 features;
    bool is_iommu_v2;
    u16 devid;
    u16 cap_ptr;
    u16 pci_seg;
    u64 exclusion_start;
    u64 exclusion_length;
    u8 *cmd_buf;
    u32 cmd_buf_head;
    u32 cmd_buf_tail;
    u8 *evt_buf;
    u8 *ppr_log;
    u8 *ga_log;
    u8 *ga_log_tail;
    bool int_enabled;
    bool need_sync;
    struct iommu_device iommu;
    u32 stored_addr_lo;
    u32 stored_addr_hi;
    u32 stored_l1[108];
    u32 stored_l2[131];
    u8 max_banks;
    u8 max_counters;
    struct irq_domain *ir_domain;
    struct irq_domain *msi_domain;
    struct amd_irte_ops *irte_ops;
    u32 flags;
    volatile u64 cmd_sem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct amd_iommu {
    struct list_head list;
    int index;
    raw_spinlock_t lock;
    struct pci_dev *dev;
    struct pci_dev *root_pdev;
    u64 mmio_phys;
    u64 mmio_phys_end;
    u8 *mmio_base;
    u32 cap;
    u8 acpi_flags;
    u64 features;
    bool is_iommu_v2;
    u16 devid;
    u16 cap_ptr;
    u16 pci_seg;
    u64 exclusion_start;
    u64 exclusion_length;
    u8 *cmd_buf;
    u32 cmd_buf_head;
    u32 cmd_buf_tail;
    u8 *evt_buf;
    u8 *ppr_log;
    u8 *ga_log;
    u8 *ga_log_tail;
    bool int_enabled;
    bool need_sync;
    struct iommu_device iommu;
    u32 stored_addr_lo;
    u32 stored_addr_hi;
    u32 stored_l1[108];
    u32 stored_l2[131];
    u8 max_banks;
    u8 max_counters;
    struct irq_domain *ir_domain;
    struct irq_domain *msi_domain;
    struct amd_irte_ops *irte_ops;
    u32 flags;
    volatile u64 cmd_sem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct amd_iommu {
    struct list_head list;
    int index;
    raw_spinlock_t lock;
    struct pci_dev *dev;
    struct pci_dev *root_pdev;
    u64 mmio_phys;
    u64 mmio_phys_end;
    u8 *mmio_base;
    u32 cap;
    u8 acpi_flags;
    u64 features;
    bool is_iommu_v2;
    u16 devid;
    u16 cap_ptr;
    u16 pci_seg;
    u64 exclusion_start;
    u64 exclusion_length;
    u8 *cmd_buf;
    u32 cmd_buf_head;
    u32 cmd_buf_tail;
    u8 *evt_buf;
    u8 *ppr_log;
    u8 *ga_log;
    u8 *ga_log_tail;
    bool int_enabled;
    bool need_sync;
    struct iommu_device iommu;
    u32 stored_addr_lo;
    u32 stored_addr_hi;
    u32 stored_l1[108];
    u32 stored_l2[131];
    u8 max_banks;
    u8 max_counters;
    struct irq_domain *ir_domain;
    struct irq_domain *msi_domain;
    struct amd_irte_ops *irte_ops;
    u32 flags;
    volatile u64 cmd_sem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct amd_iommu {
    struct list_head list;
    int index;
    raw_spinlock_t lock;
    struct pci_dev *dev;
    struct pci_dev *root_pdev;
    u64 mmio_phys;
    u64 mmio_phys_end;
    u8 *mmio_base;
    u32 cap;
    u8 acpi_flags;
    u64 features;
    bool is_iommu_v2;
    u16 devid;
    u16 cap_ptr;
    u16 pci_seg;
    u64 exclusion_start;
    u64 exclusion_length;
    u8 *cmd_buf;
    u32 cmd_buf_head;
    u32 cmd_buf_tail;
    u8 *evt_buf;
    u8 *ppr_log;
    u8 *ga_log;
    u8 *ga_log_tail;
    bool int_enabled;
    bool need_sync;
    struct iommu_device iommu;
    u32 stored_addr_lo;
    u32 stored_addr_hi;
    u32 stored_l1[108];
    u32 stored_l2[131];
    u8 max_banks;
    u8 max_counters;
    struct irq_domain *ir_domain;
    struct irq_domain *msi_domain;
    struct amd_irte_ops *irte_ops;
    u32 flags;
    volatile u64 cmd_sem;
    struct irq_affinity_notify intcapxt_notify;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct amd_iommu {
    struct list_head list;
    int index;
    raw_spinlock_t lock;
    struct pci_dev *dev;
    struct pci_dev *root_pdev;
    u64 mmio_phys;
    u64 mmio_phys_end;
    u8 *mmio_base;
    u32 cap;
    u8 acpi_flags;
    u64 features;
    bool is_iommu_v2;
    u16 devid;
    u16 cap_ptr;
    u16 pci_seg;
    u64 exclusion_start;
    u64 exclusion_length;
    u8 *cmd_buf;
    u32 cmd_buf_head;
    u32 cmd_buf_tail;
    u8 *evt_buf;
    u8 *ppr_log;
    u8 *ga_log;
    u8 *ga_log_tail;
    bool int_enabled;
    bool need_sync;
    struct iommu_device iommu;
    u32 stored_addr_lo;
    u32 stored_addr_hi;
    u32 stored_l1[108];
    u32 stored_l2[131];
    u8 max_banks;
    u8 max_counters;
    struct irq_domain *ir_domain;
    struct irq_domain *msi_domain;
    struct amd_irte_ops *irte_ops;
    u32 flags;
    volatile u64 cmd_sem;
    struct irq_affinity_notify intcapxt_notify;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct amd_iommu {
    struct list_head list;
    int index;
    raw_spinlock_t lock;
    struct pci_dev *dev;
    struct pci_dev *root_pdev;
    u64 mmio_phys;
    u64 mmio_phys_end;
    u8 *mmio_base;
    u32 cap;
    u8 acpi_flags;
    u64 features;
    bool is_iommu_v2;
    u16 devid;
    u16 cap_ptr;
    u16 pci_seg;
    u64 exclusion_start;
    u64 exclusion_length;
    u8 *cmd_buf;
    u32 cmd_buf_head;
    u32 cmd_buf_tail;
    u8 *evt_buf;
    u8 *ppr_log;
    u8 *ga_log;
    u8 *ga_log_tail;
    bool int_enabled;
    bool need_sync;
    struct iommu_device iommu;
    u32 stored_addr_lo;
    u32 stored_addr_hi;
    u32 stored_l1[108];
    u32 stored_l2[131];
    u8 max_banks;
    u8 max_counters;
    struct irq_domain *ir_domain;
    struct irq_domain *msi_domain;
    struct amd_irte_ops *irte_ops;
    u32 flags;
    volatile u64 cmd_sem;
    struct irq_affinity_notify intcapxt_notify;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct amd_iommu {
    struct list_head list;
    int index;
    raw_spinlock_t lock;
    struct pci_dev *dev;
    struct pci_dev *root_pdev;
    u64 mmio_phys;
    u64 mmio_phys_end;
    u8 *mmio_base;
    u32 cap;
    u8 acpi_flags;
    u64 features;
    bool is_iommu_v2;
    u16 devid;
    u16 cap_ptr;
    u16 pci_seg;
    u64 exclusion_start;
    u64 exclusion_length;
    u8 *cmd_buf;
    u32 cmd_buf_head;
    u32 cmd_buf_tail;
    u8 *evt_buf;
    u8 *ppr_log;
    u8 *ga_log;
    u8 *ga_log_tail;
    bool int_enabled;
    bool need_sync;
    struct iommu_device iommu;
    u32 stored_addr_lo;
    u32 stored_addr_hi;
    u32 stored_l1[108];
    u32 stored_l2[131];
    u8 max_banks;
    u8 max_counters;
    struct irq_domain *ir_domain;
    struct irq_domain *msi_domain;
    struct amd_irte_ops *irte_ops;
    u32 flags;
    volatile u64 *cmd_sem;
    u64 cmd_sem_val;
    struct irq_affinity_notify intcapxt_notify;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct amd_iommu {
    struct list_head list;
    int index;
    raw_spinlock_t lock;
    struct pci_dev *dev;
    struct pci_dev *root_pdev;
    u64 mmio_phys;
    u64 mmio_phys_end;
    u8 *mmio_base;
    u32 cap;
    u8 acpi_flags;
    u64 features;
    bool is_iommu_v2;
    u16 devid;
    u16 cap_ptr;
    u16 pci_seg;
    u64 exclusion_start;
    u64 exclusion_length;
    u8 *cmd_buf;
    u32 cmd_buf_head;
    u32 cmd_buf_tail;
    u8 *evt_buf;
    u8 *ppr_log;
    u8 *ga_log;
    u8 *ga_log_tail;
    bool int_enabled;
    bool need_sync;
    struct iommu_device iommu;
    u32 stored_addr_lo;
    u32 stored_addr_hi;
    u32 stored_l1[108];
    u32 stored_l2[131];
    u8 max_banks;
    u8 max_counters;
    struct irq_domain *ir_domain;
    struct irq_domain *msi_domain;
    struct amd_irte_ops *irte_ops;
    u32 flags;
    volatile u64 *cmd_sem;
    u64 cmd_sem_val;
    struct irq_affinity_notify intcapxt_notify;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct amd_iommu {
    struct list_head list;
    int index;
    raw_spinlock_t lock;
    struct pci_dev *dev;
    struct pci_dev *root_pdev;
    u64 mmio_phys;
    u64 mmio_phys_end;
    u8 *mmio_base;
    u32 cap;
    u8 acpi_flags;
    u64 features;
    bool is_iommu_v2;
    u16 devid;
    u16 cap_ptr;
    u16 pci_seg;
    u64 exclusion_start;
    u64 exclusion_length;
    u8 *cmd_buf;
    u32 cmd_buf_head;
    u32 cmd_buf_tail;
    u8 *evt_buf;
    u8 *ppr_log;
    u8 *ga_log;
    u8 *ga_log_tail;
    bool int_enabled;
    bool need_sync;
    struct iommu_device iommu;
    u32 stored_addr_lo;
    u32 stored_addr_hi;
    u32 stored_l1[108];
    u32 stored_l2[131];
    u8 max_banks;
    u8 max_counters;
    struct irq_domain *ir_domain;
    struct irq_domain *msi_domain;
    struct amd_irte_ops *irte_ops;
    u32 flags;
    volatile u64 *cmd_sem;
    u64 cmd_sem_val;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct amd_iommu {
    struct list_head list;
    int index;
    raw_spinlock_t lock;
    struct pci_dev *dev;
    struct pci_dev *root_pdev;
    u64 mmio_phys;
    u64 mmio_phys_end;
    u8 *mmio_base;
    u32 cap;
    u8 acpi_flags;
    u64 features;
    bool is_iommu_v2;
    u16 devid;
    u16 cap_ptr;
    u16 pci_seg;
    u64 exclusion_start;
    u64 exclusion_length;
    u8 *cmd_buf;
    u32 cmd_buf_head;
    u32 cmd_buf_tail;
    u8 *evt_buf;
    u8 *ppr_log;
    u8 *ga_log;
    u8 *ga_log_tail;
    bool int_enabled;
    bool need_sync;
    struct iommu_device iommu;
    u32 stored_addr_lo;
    u32 stored_addr_hi;
    u32 stored_l1[108];
    u32 stored_l2[131];
    u8 max_banks;
    u8 max_counters;
    struct irq_domain *ir_domain;
    struct irq_domain *msi_domain;
    struct amd_irte_ops *irte_ops;
    u32 flags;
    volatile u64 *cmd_sem;
    u64 cmd_sem_val;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct amd_iommu {
    struct list_head list;
    int index;
    raw_spinlock_t lock;
    struct pci_dev *dev;
    struct pci_dev *root_pdev;
    u64 mmio_phys;
    u64 mmio_phys_end;
    u8 *mmio_base;
    u32 cap;
    u8 acpi_flags;
    u64 features;
    u64 features2;
    bool is_iommu_v2;
    u16 devid;
    u16 cap_ptr;
    struct amd_iommu_pci_seg *pci_seg;
    u64 exclusion_start;
    u64 exclusion_length;
    u8 *cmd_buf;
    u32 cmd_buf_head;
    u32 cmd_buf_tail;
    u8 *evt_buf;
    u8 *ppr_log;
    u8 *ga_log;
    u8 *ga_log_tail;
    bool int_enabled;
    bool need_sync;
    struct iommu_device iommu;
    u32 stored_addr_lo;
    u32 stored_addr_hi;
    u32 stored_l1[108];
    u32 stored_l2[131];
    u8 max_banks;
    u8 max_counters;
    struct irq_domain *ir_domain;
    struct amd_irte_ops *irte_ops;
    u32 flags;
    volatile u64 *cmd_sem;
    u64 cmd_sem_val;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct amd_iommu {
    struct list_head list;
    int index;
    raw_spinlock_t lock;
    struct pci_dev *dev;
    struct pci_dev *root_pdev;
    u64 mmio_phys;
    u64 mmio_phys_end;
    u8 *mmio_base;
    u32 cap;
    u8 acpi_flags;
    u64 features;
    u64 features2;
    bool is_iommu_v2;
    u16 devid;
    u16 cap_ptr;
    struct amd_iommu_pci_seg *pci_seg;
    u64 exclusion_start;
    u64 exclusion_length;
    u8 *cmd_buf;
    u32 cmd_buf_head;
    u32 cmd_buf_tail;
    u8 *evt_buf;
    u8 *ppr_log;
    u8 *ga_log;
    u8 *ga_log_tail;
    bool int_enabled;
    bool need_sync;
    bool irtcachedis_enabled;
    struct iommu_device iommu;
    u32 stored_addr_lo;
    u32 stored_addr_hi;
    u32 stored_l1[108];
    u32 stored_l2[131];
    u8 max_banks;
    u8 max_counters;
    struct irq_domain *ir_domain;
    struct amd_irte_ops *irte_ops;
    u32 flags;
    volatile u64 *cmd_sem;
    atomic64_t cmd_sem_val;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct amd_iommu {
    struct list_head list;
    int index;
    raw_spinlock_t lock;
    struct pci_dev *dev;
    struct pci_dev *root_pdev;
    u64 mmio_phys;
    u64 mmio_phys_end;
    u8 *mmio_base;
    u32 cap;
    u8 acpi_flags;
    u64 features;
    u64 features2;
    u16 devid;
    u16 cap_ptr;
    struct amd_iommu_pci_seg *pci_seg;
    u64 exclusion_start;
    u64 exclusion_length;
    u8 *cmd_buf;
    u32 cmd_buf_head;
    u32 cmd_buf_tail;
    u8 *evt_buf;
    unsigned char evt_irq_name[16];
    u8 *ppr_log;
    unsigned char ppr_irq_name[16];
    u8 *ga_log;
    unsigned char ga_irq_name[16];
    u8 *ga_log_tail;
    bool int_enabled;
    bool need_sync;
    bool irtcachedis_enabled;
    struct iommu_device iommu;
    u32 stored_addr_lo;
    u32 stored_addr_hi;
    u32 stored_l1[108];
    u32 stored_l2[131];
    u8 max_banks;
    u8 max_counters;
    struct irq_domain *ir_domain;
    struct amd_irte_ops *irte_ops;
    u32 flags;
    volatile u64 *cmd_sem;
    atomic64_t cmd_sem_val;
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
struct amd_iommu {
    struct list_head list;
    int index;
    raw_spinlock_t lock;
    struct pci_dev *dev;
    struct pci_dev *root_pdev;
    u64 mmio_phys;
    u64 mmio_phys_end;
    u8 *mmio_base;
    u32 cap;
    u8 acpi_flags;
    u64 features;
    bool is_iommu_v2;
    u16 devid;
    u16 cap_ptr;
    u16 pci_seg;
    u64 exclusion_start;
    u64 exclusion_length;
    u8 *cmd_buf;
    u32 cmd_buf_head;
    u32 cmd_buf_tail;
    u8 *evt_buf;
    u8 *ppr_log;
    u8 *ga_log;
    u8 *ga_log_tail;
    bool int_enabled;
    bool need_sync;
    struct iommu_device iommu;
    u32 stored_addr_lo;
    u32 stored_addr_hi;
    u32 stored_l1[108];
    u32 stored_l2[131];
    u8 max_banks;
    u8 max_counters;
    struct irq_domain *ir_domain;
    struct irq_domain *msi_domain;
    struct amd_irte_ops *irte_ops;
    u32 flags;
    volatile u64 cmd_sem;
    struct irq_affinity_notify intcapxt_notify;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct amd_iommu {
    struct list_head list;
    int index;
    raw_spinlock_t lock;
    struct pci_dev *dev;
    struct pci_dev *root_pdev;
    u64 mmio_phys;
    u64 mmio_phys_end;
    u8 *mmio_base;
    u32 cap;
    u8 acpi_flags;
    u64 features;
    bool is_iommu_v2;
    u16 devid;
    u16 cap_ptr;
    u16 pci_seg;
    u64 exclusion_start;
    u64 exclusion_length;
    u8 *cmd_buf;
    u32 cmd_buf_head;
    u32 cmd_buf_tail;
    u8 *evt_buf;
    u8 *ppr_log;
    u8 *ga_log;
    u8 *ga_log_tail;
    bool int_enabled;
    bool need_sync;
    struct iommu_device iommu;
    u32 stored_addr_lo;
    u32 stored_addr_hi;
    u32 stored_l1[108];
    u32 stored_l2[131];
    u8 max_banks;
    u8 max_counters;
    struct irq_domain *ir_domain;
    struct irq_domain *msi_domain;
    struct amd_irte_ops *irte_ops;
    u32 flags;
    volatile u64 cmd_sem;
    struct irq_affinity_notify intcapxt_notify;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct amd_iommu {
    struct list_head list;
    int index;
    raw_spinlock_t lock;
    struct pci_dev *dev;
    struct pci_dev *root_pdev;
    u64 mmio_phys;
    u64 mmio_phys_end;
    u8 *mmio_base;
    u32 cap;
    u8 acpi_flags;
    u64 features;
    bool is_iommu_v2;
    u16 devid;
    u16 cap_ptr;
    u16 pci_seg;
    u64 exclusion_start;
    u64 exclusion_length;
    u8 *cmd_buf;
    u32 cmd_buf_head;
    u32 cmd_buf_tail;
    u8 *evt_buf;
    u8 *ppr_log;
    u8 *ga_log;
    u8 *ga_log_tail;
    bool int_enabled;
    bool need_sync;
    struct iommu_device iommu;
    u32 stored_addr_lo;
    u32 stored_addr_hi;
    u32 stored_l1[108];
    u32 stored_l2[131];
    u8 max_banks;
    u8 max_counters;
    struct irq_domain *ir_domain;
    struct irq_domain *msi_domain;
    struct amd_irte_ops *irte_ops;
    u32 flags;
    volatile u64 cmd_sem;
    struct irq_affinity_notify intcapxt_notify;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct amd_iommu {
    struct list_head list;
    int index;
    raw_spinlock_t lock;
    struct pci_dev *dev;
    struct pci_dev *root_pdev;
    u64 mmio_phys;
    u64 mmio_phys_end;
    u8 *mmio_base;
    u32 cap;
    u8 acpi_flags;
    u64 features;
    bool is_iommu_v2;
    u16 devid;
    u16 cap_ptr;
    u16 pci_seg;
    u64 exclusion_start;
    u64 exclusion_length;
    u8 *cmd_buf;
    u32 cmd_buf_head;
    u32 cmd_buf_tail;
    u8 *evt_buf;
    u8 *ppr_log;
    u8 *ga_log;
    u8 *ga_log_tail;
    bool int_enabled;
    bool need_sync;
    struct iommu_device iommu;
    u32 stored_addr_lo;
    u32 stored_addr_hi;
    u32 stored_l1[108];
    u32 stored_l2[131];
    u8 max_banks;
    u8 max_counters;
    struct irq_domain *ir_domain;
    struct irq_domain *msi_domain;
    struct amd_irte_ops *irte_ops;
    u32 flags;
    volatile u64 cmd_sem;
    struct irq_affinity_notify intcapxt_notify;
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
<code>u8 *ga_log</code>
</li>
<li>
<b>Field added. </b>
<code>u8 *ga_log_tail</code>
</li>
<li>
<b>Field added. </b>
<code>struct amd_irte_ops *irte_ops</code>
</li>
<li>
<b>Field added. </b>
<code>volatile u64 cmd_sem</code>
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
<code>u32 cmd_buf_head</code>
</li>
<li>
<b>Field added. </b>
<code>u32 cmd_buf_tail</code>
</li>
<li>
<b>Field added. </b>
<code>struct iommu_device iommu</code>
</li>
<li>
<b>Field removed. </b>
<code>struct device *iommu_dev</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 flags</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>spinlock_t lock</code> ➡️ <code>raw_spinlock_t lock</code>
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
<code>struct irq_affinity_notify intcapxt_notify</code>
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
<code>u64 cmd_sem_val</code>
</li>
<li>
<b>Field type changed. </b>
<code>volatile u64 cmd_sem</code> ➡️ <code>volatile u64 *cmd_sem</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct irq_affinity_notify intcapxt_notify</code>
</li>
</ul>
</details>
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
<code>u64 features2</code>
</li>
<li>
<b>Field removed. </b>
<code>struct irq_domain *msi_domain</code>
</li>
<li>
<b>Field type changed. </b>
<code>u16 pci_seg</code> ➡️ <code>struct amd_iommu_pci_seg *pci_seg</code>
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
<code>bool irtcachedis_enabled</code>
</li>
<li>
<b>Field type changed. </b>
<code>u64 cmd_sem_val</code> ➡️ <code>atomic64_t cmd_sem_val</code>
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
<code>unsigned char evt_irq_name[16]</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned char ppr_irq_name[16]</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned char ga_irq_name[16]</code>
</li>
<li>
<b>Field removed. </b>
<code>bool is_iommu_v2</code>
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
