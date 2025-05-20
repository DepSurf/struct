# Struct: <code>intel_iommu</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct intel_iommu {
    void *reg;
    u64 reg_phys;
    u64 reg_size;
    u64 cap;
    u64 ecap;
    u32 gcmd;
    raw_spinlock_t register_lock;
    int seq_id;
    int agaw;
    int msagaw;
    unsigned int irq;
    unsigned int pr_irq;
    u16 segment;
    unsigned char name[13];
    long unsigned int *domain_ids;
    struct dmar_domain ***domains;
    spinlock_t lock;
    struct root_entry *root_entry;
    struct iommu_flush flush;
    struct pasid_entry *pasid_table;
    struct pasid_state_entry *pasid_state_table;
    struct page_req_dsc *prq;
    unsigned char prq_name[16];
    struct idr pasid_idr;
    struct q_inval *qi;
    u32 *iommu_state;
    struct ir_table *ir_table;
    struct irq_domain *ir_domain;
    struct irq_domain *ir_msi_domain;
    struct device *iommu_dev;
    int node;
    u32 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct intel_iommu {
    void *reg;
    u64 reg_phys;
    u64 reg_size;
    u64 cap;
    u64 ecap;
    u32 gcmd;
    raw_spinlock_t register_lock;
    int seq_id;
    int agaw;
    int msagaw;
    unsigned int irq;
    unsigned int pr_irq;
    u16 segment;
    unsigned char name[13];
    long unsigned int *domain_ids;
    struct dmar_domain ***domains;
    spinlock_t lock;
    struct root_entry *root_entry;
    struct iommu_flush flush;
    struct pasid_entry *pasid_table;
    struct pasid_state_entry *pasid_state_table;
    struct page_req_dsc *prq;
    unsigned char prq_name[16];
    struct idr pasid_idr;
    struct q_inval *qi;
    u32 *iommu_state;
    struct ir_table *ir_table;
    struct irq_domain *ir_domain;
    struct irq_domain *ir_msi_domain;
    struct device *iommu_dev;
    int node;
    u32 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct intel_iommu {
    void *reg;
    u64 reg_phys;
    u64 reg_size;
    u64 cap;
    u64 ecap;
    u32 gcmd;
    raw_spinlock_t register_lock;
    int seq_id;
    int agaw;
    int msagaw;
    unsigned int irq;
    unsigned int pr_irq;
    u16 segment;
    unsigned char name[13];
    long unsigned int *domain_ids;
    struct dmar_domain ***domains;
    spinlock_t lock;
    struct root_entry *root_entry;
    struct iommu_flush flush;
    struct pasid_entry *pasid_table;
    struct pasid_state_entry *pasid_state_table;
    struct page_req_dsc *prq;
    unsigned char prq_name[16];
    struct idr pasid_idr;
    u32 pasid_max;
    struct q_inval *qi;
    u32 *iommu_state;
    struct ir_table *ir_table;
    struct irq_domain *ir_domain;
    struct irq_domain *ir_msi_domain;
    struct device *iommu_dev;
    int node;
    u32 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct intel_iommu {
    void *reg;
    u64 reg_phys;
    u64 reg_size;
    u64 cap;
    u64 ecap;
    u32 gcmd;
    raw_spinlock_t register_lock;
    int seq_id;
    int agaw;
    int msagaw;
    unsigned int irq;
    unsigned int pr_irq;
    u16 segment;
    unsigned char name[13];
    long unsigned int *domain_ids;
    struct dmar_domain ***domains;
    spinlock_t lock;
    struct root_entry *root_entry;
    struct iommu_flush flush;
    struct pasid_entry *pasid_table;
    struct pasid_state_entry *pasid_state_table;
    struct page_req_dsc *prq;
    unsigned char prq_name[16];
    struct idr pasid_idr;
    u32 pasid_max;
    struct q_inval *qi;
    u32 *iommu_state;
    struct ir_table *ir_table;
    struct irq_domain *ir_domain;
    struct irq_domain *ir_msi_domain;
    struct iommu_device iommu;
    int node;
    u32 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct intel_iommu {
    void *reg;
    u64 reg_phys;
    u64 reg_size;
    u64 cap;
    u64 ecap;
    u32 gcmd;
    raw_spinlock_t register_lock;
    int seq_id;
    int agaw;
    int msagaw;
    unsigned int irq;
    unsigned int pr_irq;
    u16 segment;
    unsigned char name[13];
    long unsigned int *domain_ids;
    struct dmar_domain ***domains;
    spinlock_t lock;
    struct root_entry *root_entry;
    struct iommu_flush flush;
    struct pasid_entry *pasid_table;
    struct pasid_state_entry *pasid_state_table;
    struct page_req_dsc *prq;
    unsigned char prq_name[16];
    struct idr pasid_idr;
    u32 pasid_max;
    struct q_inval *qi;
    u32 *iommu_state;
    struct ir_table *ir_table;
    struct irq_domain *ir_domain;
    struct irq_domain *ir_msi_domain;
    struct iommu_device iommu;
    int node;
    u32 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct intel_iommu {
    void *reg;
    u64 reg_phys;
    u64 reg_size;
    u64 cap;
    u64 ecap;
    u32 gcmd;
    raw_spinlock_t register_lock;
    int seq_id;
    int agaw;
    int msagaw;
    unsigned int irq;
    unsigned int pr_irq;
    u16 segment;
    unsigned char name[13];
    long unsigned int *domain_ids;
    struct dmar_domain ***domains;
    spinlock_t lock;
    struct root_entry *root_entry;
    struct iommu_flush flush;
    struct pasid_entry *pasid_table;
    struct pasid_state_entry *pasid_state_table;
    struct page_req_dsc *prq;
    unsigned char prq_name[16];
    struct idr pasid_idr;
    u32 pasid_max;
    struct q_inval *qi;
    u32 *iommu_state;
    struct ir_table *ir_table;
    struct irq_domain *ir_domain;
    struct irq_domain *ir_msi_domain;
    struct iommu_device iommu;
    int node;
    u32 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct intel_iommu {
    void *reg;
    u64 reg_phys;
    u64 reg_size;
    u64 cap;
    u64 ecap;
    u32 gcmd;
    raw_spinlock_t register_lock;
    int seq_id;
    int agaw;
    int msagaw;
    unsigned int irq;
    unsigned int pr_irq;
    u16 segment;
    unsigned char name[13];
    long unsigned int *domain_ids;
    struct dmar_domain ***domains;
    spinlock_t lock;
    struct root_entry *root_entry;
    struct iommu_flush flush;
    struct page_req_dsc *prq;
    unsigned char prq_name[16];
    struct q_inval *qi;
    u32 *iommu_state;
    struct ir_table *ir_table;
    struct irq_domain *ir_domain;
    struct irq_domain *ir_msi_domain;
    struct iommu_device iommu;
    int node;
    u32 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct intel_iommu {
    void *reg;
    u64 reg_phys;
    u64 reg_size;
    u64 cap;
    u64 ecap;
    u32 gcmd;
    raw_spinlock_t register_lock;
    int seq_id;
    int agaw;
    int msagaw;
    unsigned int irq;
    unsigned int pr_irq;
    u16 segment;
    unsigned char name[13];
    long unsigned int *domain_ids;
    struct dmar_domain ***domains;
    spinlock_t lock;
    struct root_entry *root_entry;
    struct iommu_flush flush;
    struct page_req_dsc *prq;
    unsigned char prq_name[16];
    struct q_inval *qi;
    u32 *iommu_state;
    struct ir_table *ir_table;
    struct irq_domain *ir_domain;
    struct irq_domain *ir_msi_domain;
    struct iommu_device iommu;
    int node;
    u32 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct intel_iommu {
    void *reg;
    u64 reg_phys;
    u64 reg_size;
    u64 cap;
    u64 ecap;
    u32 gcmd;
    raw_spinlock_t register_lock;
    int seq_id;
    int agaw;
    int msagaw;
    unsigned int irq;
    unsigned int pr_irq;
    u16 segment;
    unsigned char name[13];
    long unsigned int *domain_ids;
    struct dmar_domain ***domains;
    spinlock_t lock;
    struct root_entry *root_entry;
    struct iommu_flush flush;
    struct page_req_dsc *prq;
    unsigned char prq_name[16];
    struct q_inval *qi;
    u32 *iommu_state;
    struct ir_table *ir_table;
    struct irq_domain *ir_domain;
    struct irq_domain *ir_msi_domain;
    struct iommu_device iommu;
    int node;
    u32 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct intel_iommu {
    void *reg;
    u64 reg_phys;
    u64 reg_size;
    u64 cap;
    u64 ecap;
    u64 vccap;
    u32 gcmd;
    raw_spinlock_t register_lock;
    int seq_id;
    int agaw;
    int msagaw;
    unsigned int irq;
    unsigned int pr_irq;
    u16 segment;
    unsigned char name[13];
    long unsigned int *domain_ids;
    struct dmar_domain ***domains;
    spinlock_t lock;
    struct root_entry *root_entry;
    struct iommu_flush flush;
    struct page_req_dsc *prq;
    unsigned char prq_name[16];
    struct completion prq_complete;
    struct ioasid_allocator_ops pasid_allocator;
    struct q_inval *qi;
    u32 *iommu_state;
    struct ir_table *ir_table;
    struct irq_domain *ir_domain;
    struct irq_domain *ir_msi_domain;
    struct iommu_device iommu;
    int node;
    u32 flags;
    struct dmar_drhd_unit *drhd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct intel_iommu {
    void *reg;
    u64 reg_phys;
    u64 reg_size;
    u64 cap;
    u64 ecap;
    u64 vccap;
    u32 gcmd;
    raw_spinlock_t register_lock;
    int seq_id;
    int agaw;
    int msagaw;
    unsigned int irq;
    unsigned int pr_irq;
    u16 segment;
    unsigned char name[13];
    long unsigned int *domain_ids;
    struct dmar_domain ***domains;
    spinlock_t lock;
    struct root_entry *root_entry;
    struct iommu_flush flush;
    struct page_req_dsc *prq;
    unsigned char prq_name[16];
    struct completion prq_complete;
    struct ioasid_allocator_ops pasid_allocator;
    struct q_inval *qi;
    u32 *iommu_state;
    struct ir_table *ir_table;
    struct irq_domain *ir_domain;
    struct irq_domain *ir_msi_domain;
    struct iommu_device iommu;
    int node;
    u32 flags;
    struct dmar_drhd_unit *drhd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct intel_iommu {
    void *reg;
    u64 reg_phys;
    u64 reg_size;
    u64 cap;
    u64 ecap;
    u64 vccap;
    u32 gcmd;
    raw_spinlock_t register_lock;
    int seq_id;
    int agaw;
    int msagaw;
    unsigned int irq;
    unsigned int pr_irq;
    u16 segment;
    unsigned char name[13];
    long unsigned int *domain_ids;
    struct dmar_domain ***domains;
    spinlock_t lock;
    struct root_entry *root_entry;
    struct iommu_flush flush;
    struct page_req_dsc *prq;
    unsigned char prq_name[16];
    struct completion prq_complete;
    struct ioasid_allocator_ops pasid_allocator;
    struct q_inval *qi;
    u32 *iommu_state;
    struct ir_table *ir_table;
    struct irq_domain *ir_domain;
    struct irq_domain *ir_msi_domain;
    struct iommu_device iommu;
    int node;
    u32 flags;
    struct dmar_drhd_unit *drhd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct intel_iommu {
    void *reg;
    u64 reg_phys;
    u64 reg_size;
    u64 cap;
    u64 ecap;
    u64 vccap;
    u32 gcmd;
    raw_spinlock_t register_lock;
    int seq_id;
    int agaw;
    int msagaw;
    unsigned int irq;
    unsigned int pr_irq;
    u16 segment;
    unsigned char name[13];
    long unsigned int *domain_ids;
    struct dmar_domain ***domains;
    spinlock_t lock;
    struct root_entry *root_entry;
    struct iommu_flush flush;
    struct page_req_dsc *prq;
    unsigned char prq_name[16];
    struct completion prq_complete;
    struct ioasid_allocator_ops pasid_allocator;
    struct iopf_queue *iopf_queue;
    unsigned char iopfq_name[16];
    struct q_inval *qi;
    u32 *iommu_state;
    struct ir_table *ir_table;
    struct irq_domain *ir_domain;
    struct irq_domain *ir_msi_domain;
    struct iommu_device iommu;
    int node;
    u32 flags;
    struct dmar_drhd_unit *drhd;
    void *perf_statistic;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct intel_iommu {
    void *reg;
    u64 reg_phys;
    u64 reg_size;
    u64 cap;
    u64 ecap;
    u64 vccap;
    u32 gcmd;
    raw_spinlock_t register_lock;
    int seq_id;
    int agaw;
    int msagaw;
    unsigned int irq;
    unsigned int pr_irq;
    u16 segment;
    unsigned char name[13];
    long unsigned int *domain_ids;
    spinlock_t lock;
    struct root_entry *root_entry;
    struct iommu_flush flush;
    struct page_req_dsc *prq;
    unsigned char prq_name[16];
    struct completion prq_complete;
    struct ioasid_allocator_ops pasid_allocator;
    struct iopf_queue *iopf_queue;
    unsigned char iopfq_name[16];
    struct q_inval *qi;
    u32 *iommu_state;
    struct ir_table *ir_table;
    struct irq_domain *ir_domain;
    struct irq_domain *ir_msi_domain;
    struct iommu_device iommu;
    int node;
    u32 flags;
    struct dmar_drhd_unit *drhd;
    void *perf_statistic;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct intel_iommu {
    void *reg;
    u64 reg_phys;
    u64 reg_size;
    u64 cap;
    u64 ecap;
    u64 vccap;
    u32 gcmd;
    raw_spinlock_t register_lock;
    int seq_id;
    int agaw;
    int msagaw;
    unsigned int irq;
    unsigned int pr_irq;
    u16 segment;
    unsigned char name[13];
    long unsigned int *domain_ids;
    long unsigned int *copied_tables;
    spinlock_t lock;
    struct root_entry *root_entry;
    struct iommu_flush flush;
    struct page_req_dsc *prq;
    unsigned char prq_name[16];
    long unsigned int prq_seq_number;
    struct completion prq_complete;
    struct ioasid_allocator_ops pasid_allocator;
    struct iopf_queue *iopf_queue;
    unsigned char iopfq_name[16];
    struct q_inval *qi;
    u32 *iommu_state;
    struct ir_table *ir_table;
    struct irq_domain *ir_domain;
    struct iommu_device iommu;
    int node;
    u32 flags;
    struct dmar_drhd_unit *drhd;
    void *perf_statistic;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct intel_iommu {
    void *reg;
    u64 reg_phys;
    u64 reg_size;
    u64 cap;
    u64 ecap;
    u64 vccap;
    u64 ecmdcap[4];
    u32 gcmd;
    raw_spinlock_t register_lock;
    int seq_id;
    int agaw;
    int msagaw;
    unsigned int irq;
    unsigned int pr_irq;
    unsigned int perf_irq;
    u16 segment;
    unsigned char name[13];
    long unsigned int *domain_ids;
    long unsigned int *copied_tables;
    spinlock_t lock;
    struct root_entry *root_entry;
    struct iommu_flush flush;
    struct page_req_dsc *prq;
    unsigned char prq_name[16];
    long unsigned int prq_seq_number;
    struct completion prq_complete;
    struct iopf_queue *iopf_queue;
    unsigned char iopfq_name[16];
    struct q_inval *qi;
    u32 *iommu_state;
    struct ir_table *ir_table;
    struct irq_domain *ir_domain;
    struct iommu_device iommu;
    int node;
    u32 flags;
    struct dmar_drhd_unit *drhd;
    void *perf_statistic;
    struct iommu_pmu *pmu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct intel_iommu {
    void *reg;
    u64 reg_phys;
    u64 reg_size;
    u64 cap;
    u64 ecap;
    u64 vccap;
    u64 ecmdcap[4];
    u32 gcmd;
    raw_spinlock_t register_lock;
    int seq_id;
    int agaw;
    int msagaw;
    unsigned int irq;
    unsigned int pr_irq;
    unsigned int perf_irq;
    u16 segment;
    unsigned char name[13];
    long unsigned int *domain_ids;
    long unsigned int *copied_tables;
    spinlock_t lock;
    struct root_entry *root_entry;
    struct iommu_flush flush;
    struct page_req_dsc *prq;
    unsigned char prq_name[16];
    long unsigned int prq_seq_number;
    struct completion prq_complete;
    struct iopf_queue *iopf_queue;
    unsigned char iopfq_name[16];
    struct q_inval *qi;
    u32 iommu_state[4];
    struct ir_table *ir_table;
    struct irq_domain *ir_domain;
    struct iommu_device iommu;
    int node;
    u32 flags;
    struct dmar_drhd_unit *drhd;
    void *perf_statistic;
    struct iommu_pmu *pmu;
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
struct intel_iommu {
    void *reg;
    u64 reg_phys;
    u64 reg_size;
    u64 cap;
    u64 ecap;
    u32 gcmd;
    raw_spinlock_t register_lock;
    int seq_id;
    int agaw;
    int msagaw;
    unsigned int irq;
    unsigned int pr_irq;
    u16 segment;
    unsigned char name[13];
    long unsigned int *domain_ids;
    struct dmar_domain ***domains;
    spinlock_t lock;
    struct root_entry *root_entry;
    struct iommu_flush flush;
    struct page_req_dsc *prq;
    unsigned char prq_name[16];
    struct q_inval *qi;
    u32 *iommu_state;
    struct ir_table *ir_table;
    struct irq_domain *ir_domain;
    struct irq_domain *ir_msi_domain;
    struct iommu_device iommu;
    int node;
    u32 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct intel_iommu {
    void *reg;
    u64 reg_phys;
    u64 reg_size;
    u64 cap;
    u64 ecap;
    u32 gcmd;
    raw_spinlock_t register_lock;
    int seq_id;
    int agaw;
    int msagaw;
    unsigned int irq;
    unsigned int pr_irq;
    u16 segment;
    unsigned char name[13];
    long unsigned int *domain_ids;
    struct dmar_domain ***domains;
    spinlock_t lock;
    struct root_entry *root_entry;
    struct iommu_flush flush;
    struct page_req_dsc *prq;
    unsigned char prq_name[16];
    struct q_inval *qi;
    u32 *iommu_state;
    struct ir_table *ir_table;
    struct irq_domain *ir_domain;
    struct irq_domain *ir_msi_domain;
    struct iommu_device iommu;
    int node;
    u32 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct intel_iommu {
    void *reg;
    u64 reg_phys;
    u64 reg_size;
    u64 cap;
    u64 ecap;
    u32 gcmd;
    raw_spinlock_t register_lock;
    int seq_id;
    int agaw;
    int msagaw;
    unsigned int irq;
    unsigned int pr_irq;
    u16 segment;
    unsigned char name[13];
    long unsigned int *domain_ids;
    struct dmar_domain ***domains;
    spinlock_t lock;
    struct root_entry *root_entry;
    struct iommu_flush flush;
    struct page_req_dsc *prq;
    unsigned char prq_name[16];
    struct q_inval *qi;
    u32 *iommu_state;
    struct ir_table *ir_table;
    struct irq_domain *ir_domain;
    struct irq_domain *ir_msi_domain;
    struct iommu_device iommu;
    int node;
    u32 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct intel_iommu {
    void *reg;
    u64 reg_phys;
    u64 reg_size;
    u64 cap;
    u64 ecap;
    u32 gcmd;
    raw_spinlock_t register_lock;
    int seq_id;
    int agaw;
    int msagaw;
    unsigned int irq;
    unsigned int pr_irq;
    u16 segment;
    unsigned char name[13];
    long unsigned int *domain_ids;
    struct dmar_domain ***domains;
    spinlock_t lock;
    struct root_entry *root_entry;
    struct iommu_flush flush;
    struct page_req_dsc *prq;
    unsigned char prq_name[16];
    struct q_inval *qi;
    u32 *iommu_state;
    struct ir_table *ir_table;
    struct irq_domain *ir_domain;
    struct irq_domain *ir_msi_domain;
    struct iommu_device iommu;
    int node;
    u32 flags;
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
<code>u32 pasid_max</code>
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
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct pasid_entry *pasid_table</code>
</li>
<li>
<b>Field removed. </b>
<code>struct pasid_state_entry *pasid_state_table</code>
</li>
<li>
<b>Field removed. </b>
<code>struct idr pasid_idr</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 pasid_max</code>
</li>
</ul>
</details>
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
<b>Field added. </b>
<code>u64 vccap</code>
</li>
<li>
<b>Field added. </b>
<code>struct completion prq_complete</code>
</li>
<li>
<b>Field added. </b>
<code>struct ioasid_allocator_ops pasid_allocator</code>
</li>
<li>
<b>Field added. </b>
<code>struct dmar_drhd_unit *drhd</code>
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
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct iopf_queue *iopf_queue</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned char iopfq_name[16]</code>
</li>
<li>
<b>Field added. </b>
<code>void *perf_statistic</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct dmar_domain ***domains</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int *copied_tables</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int prq_seq_number</code>
</li>
<li>
<b>Field removed. </b>
<code>struct irq_domain *ir_msi_domain</code>
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
<code>u64 ecmdcap[4]</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int perf_irq</code>
</li>
<li>
<b>Field added. </b>
<code>struct iommu_pmu *pmu</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ioasid_allocator_ops pasid_allocator</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>u32 *iommu_state</code> ➡️ <code>u32 iommu_state[4]</code>
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
