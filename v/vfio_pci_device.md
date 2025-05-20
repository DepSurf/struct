# Struct: <code>vfio_pci_device</code>

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
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct vfio_pci_device {
    struct pci_dev *pdev;
    void * barmap[6];
    bool bar_mmap_supported[6];
    u8 *pci_config_map;
    u8 *vconfig;
    struct perm_bits *msi_perm;
    spinlock_t irqlock;
    struct mutex igate;
    struct vfio_pci_irq_ctx *ctx;
    int num_ctx;
    int irq_type;
    int num_regions;
    struct vfio_pci_region *region;
    u8 msi_qmax;
    u8 msix_bar;
    u16 msix_size;
    u32 msix_offset;
    u32 rbar[7];
    bool pci_2_3;
    bool virq_disabled;
    bool reset_works;
    bool extended_caps;
    bool bardirty;
    bool has_vga;
    bool needs_reset;
    bool nointx;
    bool needs_pm_restore;
    struct pci_saved_state *pci_saved_state;
    struct pci_saved_state *pm_save;
    struct vfio_pci_reflck *reflck;
    int refcnt;
    int ioeventfds_nr;
    struct eventfd_ctx *err_trigger;
    struct eventfd_ctx *req_trigger;
    struct list_head dummy_resources_list;
    struct mutex ioeventfds_lock;
    struct list_head ioeventfds_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct vfio_pci_device {
    struct pci_dev *pdev;
    void * barmap[6];
    bool bar_mmap_supported[6];
    u8 *pci_config_map;
    u8 *vconfig;
    struct perm_bits *msi_perm;
    spinlock_t irqlock;
    struct mutex igate;
    struct vfio_pci_irq_ctx *ctx;
    int num_ctx;
    int irq_type;
    int num_regions;
    struct vfio_pci_region *region;
    u8 msi_qmax;
    u8 msix_bar;
    u16 msix_size;
    u32 msix_offset;
    u32 rbar[7];
    bool pci_2_3;
    bool virq_disabled;
    bool reset_works;
    bool extended_caps;
    bool bardirty;
    bool has_vga;
    bool needs_reset;
    bool nointx;
    bool needs_pm_restore;
    struct pci_saved_state *pci_saved_state;
    struct pci_saved_state *pm_save;
    struct vfio_pci_reflck *reflck;
    int refcnt;
    int ioeventfds_nr;
    struct eventfd_ctx *err_trigger;
    struct eventfd_ctx *req_trigger;
    struct list_head dummy_resources_list;
    struct mutex ioeventfds_lock;
    struct list_head ioeventfds_list;
    struct vfio_pci_vf_token *vf_token;
    struct notifier_block nb;
    struct mutex vma_lock;
    struct list_head vma_list;
    struct rw_semaphore memory_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct vfio_pci_device {
    struct pci_dev *pdev;
    void * barmap[6];
    bool bar_mmap_supported[6];
    u8 *pci_config_map;
    u8 *vconfig;
    struct perm_bits *msi_perm;
    spinlock_t irqlock;
    struct mutex igate;
    struct vfio_pci_irq_ctx *ctx;
    int num_ctx;
    int irq_type;
    int num_regions;
    struct vfio_pci_region *region;
    u8 msi_qmax;
    u8 msix_bar;
    u16 msix_size;
    u32 msix_offset;
    u32 rbar[7];
    bool pci_2_3;
    bool virq_disabled;
    bool reset_works;
    bool extended_caps;
    bool bardirty;
    bool has_vga;
    bool needs_reset;
    bool nointx;
    bool needs_pm_restore;
    struct pci_saved_state *pci_saved_state;
    struct pci_saved_state *pm_save;
    struct vfio_pci_reflck *reflck;
    int refcnt;
    int ioeventfds_nr;
    struct eventfd_ctx *err_trigger;
    struct eventfd_ctx *req_trigger;
    struct list_head dummy_resources_list;
    struct mutex ioeventfds_lock;
    struct list_head ioeventfds_list;
    struct vfio_pci_vf_token *vf_token;
    struct notifier_block nb;
    struct mutex vma_lock;
    struct list_head vma_list;
    struct rw_semaphore memory_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct vfio_pci_device {
    struct vfio_device vdev;
    struct pci_dev *pdev;
    void * barmap[6];
    bool bar_mmap_supported[6];
    u8 *pci_config_map;
    u8 *vconfig;
    struct perm_bits *msi_perm;
    spinlock_t irqlock;
    struct mutex igate;
    struct vfio_pci_irq_ctx *ctx;
    int num_ctx;
    int irq_type;
    int num_regions;
    struct vfio_pci_region *region;
    u8 msi_qmax;
    u8 msix_bar;
    u16 msix_size;
    u32 msix_offset;
    u32 rbar[7];
    bool pci_2_3;
    bool virq_disabled;
    bool reset_works;
    bool extended_caps;
    bool bardirty;
    bool has_vga;
    bool needs_reset;
    bool nointx;
    bool needs_pm_restore;
    struct pci_saved_state *pci_saved_state;
    struct pci_saved_state *pm_save;
    struct vfio_pci_reflck *reflck;
    int refcnt;
    int ioeventfds_nr;
    struct eventfd_ctx *err_trigger;
    struct eventfd_ctx *req_trigger;
    struct list_head dummy_resources_list;
    struct mutex ioeventfds_lock;
    struct list_head ioeventfds_list;
    struct vfio_pci_vf_token *vf_token;
    struct notifier_block nb;
    struct mutex vma_lock;
    struct list_head vma_list;
    struct rw_semaphore memory_lock;
};
```
</details>
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
struct vfio_pci_device {
    struct pci_dev *pdev;
    void * barmap[6];
    bool bar_mmap_supported[6];
    u8 *pci_config_map;
    u8 *vconfig;
    struct perm_bits *msi_perm;
    spinlock_t irqlock;
    struct mutex igate;
    struct vfio_pci_irq_ctx *ctx;
    int num_ctx;
    int irq_type;
    int num_regions;
    struct vfio_pci_region *region;
    u8 msi_qmax;
    u8 msix_bar;
    u16 msix_size;
    u32 msix_offset;
    u32 rbar[7];
    bool pci_2_3;
    bool virq_disabled;
    bool reset_works;
    bool extended_caps;
    bool bardirty;
    bool has_vga;
    bool needs_reset;
    bool nointx;
    bool needs_pm_restore;
    struct pci_saved_state *pci_saved_state;
    struct pci_saved_state *pm_save;
    struct vfio_pci_reflck *reflck;
    int refcnt;
    int ioeventfds_nr;
    struct eventfd_ctx *err_trigger;
    struct eventfd_ctx *req_trigger;
    struct list_head dummy_resources_list;
    struct mutex ioeventfds_lock;
    struct list_head ioeventfds_list;
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
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct vfio_pci_device {
    struct pci_dev *pdev;
    void * barmap[6];
    bool bar_mmap_supported[6];
    u8 *pci_config_map;
    u8 *vconfig;
    struct perm_bits *msi_perm;
    spinlock_t irqlock;
    struct mutex igate;
    struct vfio_pci_irq_ctx *ctx;
    int num_ctx;
    int irq_type;
    int num_regions;
    struct vfio_pci_region *region;
    u8 msi_qmax;
    u8 msix_bar;
    u16 msix_size;
    u32 msix_offset;
    u32 rbar[7];
    bool pci_2_3;
    bool virq_disabled;
    bool reset_works;
    bool extended_caps;
    bool bardirty;
    bool has_vga;
    bool needs_reset;
    bool nointx;
    bool needs_pm_restore;
    struct pci_saved_state *pci_saved_state;
    struct pci_saved_state *pm_save;
    struct vfio_pci_reflck *reflck;
    int refcnt;
    int ioeventfds_nr;
    struct eventfd_ctx *err_trigger;
    struct eventfd_ctx *req_trigger;
    struct list_head dummy_resources_list;
    struct mutex ioeventfds_lock;
    struct list_head ioeventfds_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct vfio_pci_device {
    struct pci_dev *pdev;
    void * barmap[6];
    bool bar_mmap_supported[6];
    u8 *pci_config_map;
    u8 *vconfig;
    struct perm_bits *msi_perm;
    spinlock_t irqlock;
    struct mutex igate;
    struct vfio_pci_irq_ctx *ctx;
    int num_ctx;
    int irq_type;
    int num_regions;
    struct vfio_pci_region *region;
    u8 msi_qmax;
    u8 msix_bar;
    u16 msix_size;
    u32 msix_offset;
    u32 rbar[7];
    bool pci_2_3;
    bool virq_disabled;
    bool reset_works;
    bool extended_caps;
    bool bardirty;
    bool has_vga;
    bool needs_reset;
    bool nointx;
    bool needs_pm_restore;
    struct pci_saved_state *pci_saved_state;
    struct pci_saved_state *pm_save;
    struct vfio_pci_reflck *reflck;
    int refcnt;
    int ioeventfds_nr;
    struct eventfd_ctx *err_trigger;
    struct eventfd_ctx *req_trigger;
    struct list_head dummy_resources_list;
    struct mutex ioeventfds_lock;
    struct list_head ioeventfds_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct vfio_pci_device {
    struct pci_dev *pdev;
    void * barmap[6];
    bool bar_mmap_supported[6];
    u8 *pci_config_map;
    u8 *vconfig;
    struct perm_bits *msi_perm;
    spinlock_t irqlock;
    struct mutex igate;
    struct vfio_pci_irq_ctx *ctx;
    int num_ctx;
    int irq_type;
    int num_regions;
    struct vfio_pci_region *region;
    u8 msi_qmax;
    u8 msix_bar;
    u16 msix_size;
    u32 msix_offset;
    u32 rbar[7];
    bool pci_2_3;
    bool virq_disabled;
    bool reset_works;
    bool extended_caps;
    bool bardirty;
    bool has_vga;
    bool needs_reset;
    bool nointx;
    bool needs_pm_restore;
    struct pci_saved_state *pci_saved_state;
    struct pci_saved_state *pm_save;
    struct vfio_pci_reflck *reflck;
    int refcnt;
    int ioeventfds_nr;
    struct eventfd_ctx *err_trigger;
    struct eventfd_ctx *req_trigger;
    struct list_head dummy_resources_list;
    struct mutex ioeventfds_lock;
    struct list_head ioeventfds_list;
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
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct vfio_pci_vf_token *vf_token</code>
</li>
<li>
<b>Field added. </b>
<code>struct notifier_block nb</code>
</li>
<li>
<b>Field added. </b>
<code>struct mutex vma_lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head vma_list</code>
</li>
<li>
<b>Field added. </b>
<code>struct rw_semaphore memory_lock</code>
</li>
</ul>
</details>
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
<code>struct vfio_device vdev</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
</li>
</ul>
<b>Flavor</b>
<ul>
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
