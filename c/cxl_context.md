# Struct: <code>cxl_context</code>

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
struct cxl_context {
    struct cxl_afu *afu;
    phys_addr_t psn_phys;
    u64 psn_size;
    struct address_space *mapping;
    struct mutex mapping_lock;
    struct page *ff_page;
    bool mmio_err_ff;
    bool kernelapi;
    spinlock_t sste_lock;
    struct cxl_sste *sstp;
    u64 sstp0;
    u64 sstp1;
    unsigned int sst_size;
    unsigned int sst_lru;
    wait_queue_head_t wq;
    struct pid *pid;
    spinlock_t lock;
    u64 process_token;
    void *priv;
    long unsigned int *irq_bitmap;
    struct cxl_irq_ranges irqs;
    struct list_head irq_names;
    u64 fault_addr;
    u64 fault_dsisr;
    u64 afu_err;
    enum cxl_context_status status;
    struct mutex status_mutex;
    struct work_struct fault_work;
    u64 dsisr;
    u64 dar;
    struct cxl_process_element *elem;
    int pe;
    int external_pe;
    u32 irq_count;
    bool pe_inserted;
    bool master;
    bool kernel;
    bool pending_irq;
    bool pending_fault;
    bool pending_afu_err;
    struct cxl_afu_driver_ops *afu_driver_ops;
    atomic_t afu_driver_events;
    struct callback_head rcu;
    struct mm_struct *mm;
    u16 tidr;
    bool assign_tidr;
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
