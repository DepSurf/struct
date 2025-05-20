# Struct: <code>dmar_domain</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct dmar_domain {
    int nid;
    unsigned int iommu_refcnt[128];
    u16 iommu_did[128];
    struct list_head devices;
    struct iova_domain iovad;
    struct dma_pte *pgd;
    int gaw;
    int agaw;
    int flags;
    int iommu_coherency;
    int iommu_snooping;
    int iommu_count;
    int iommu_superpage;
    u64 max_addr;
    struct iommu_domain domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct dmar_domain {
    int nid;
    unsigned int iommu_refcnt[128];
    u16 iommu_did[128];
    bool has_iotlb_device;
    struct list_head devices;
    struct iova_domain iovad;
    struct dma_pte *pgd;
    int gaw;
    int agaw;
    int flags;
    int iommu_coherency;
    int iommu_snooping;
    int iommu_count;
    int iommu_superpage;
    u64 max_addr;
    struct iommu_domain domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct dmar_domain {
    int nid;
    unsigned int iommu_refcnt[128];
    u16 iommu_did[128];
    bool has_iotlb_device;
    struct list_head devices;
    struct iova_domain iovad;
    struct dma_pte *pgd;
    int gaw;
    int agaw;
    int flags;
    int iommu_coherency;
    int iommu_snooping;
    int iommu_count;
    int iommu_superpage;
    u64 max_addr;
    struct iommu_domain domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct dmar_domain {
    int nid;
    unsigned int iommu_refcnt[128];
    u16 iommu_did[128];
    bool has_iotlb_device;
    struct list_head devices;
    struct iova_domain iovad;
    struct dma_pte *pgd;
    int gaw;
    int agaw;
    int flags;
    int iommu_coherency;
    int iommu_snooping;
    int iommu_count;
    int iommu_superpage;
    u64 max_addr;
    struct iommu_domain domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dmar_domain {
    int nid;
    unsigned int iommu_refcnt[128];
    u16 iommu_did[128];
    bool has_iotlb_device;
    struct list_head devices;
    struct iova_domain iovad;
    struct dma_pte *pgd;
    int gaw;
    int agaw;
    int flags;
    int iommu_coherency;
    int iommu_snooping;
    int iommu_count;
    int iommu_superpage;
    u64 max_addr;
    struct iommu_domain domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dmar_domain {
    int nid;
    unsigned int iommu_refcnt[128];
    u16 iommu_did[128];
    bool has_iotlb_device;
    struct list_head devices;
    struct iova_domain iovad;
    struct dma_pte *pgd;
    int gaw;
    int agaw;
    int flags;
    int iommu_coherency;
    int iommu_snooping;
    int iommu_count;
    int iommu_superpage;
    u64 max_addr;
    struct iommu_domain domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dmar_domain {
    int nid;
    unsigned int iommu_refcnt[128];
    u16 iommu_did[128];
    bool has_iotlb_device;
    struct list_head devices;
    struct iova_domain iovad;
    struct dma_pte *pgd;
    int gaw;
    int agaw;
    int flags;
    int iommu_coherency;
    int iommu_snooping;
    int iommu_count;
    int iommu_superpage;
    u64 max_addr;
    struct iommu_domain domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dmar_domain {
    int nid;
    unsigned int iommu_refcnt[128];
    u16 iommu_did[128];
    unsigned int auxd_refcnt;
    bool has_iotlb_device;
    struct list_head devices;
    struct list_head auxd;
    struct iova_domain iovad;
    struct dma_pte *pgd;
    int gaw;
    int agaw;
    int flags;
    int iommu_coherency;
    int iommu_snooping;
    int iommu_count;
    int iommu_superpage;
    u64 max_addr;
    int default_pasid;
    struct iommu_domain domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dmar_domain {
    int nid;
    unsigned int iommu_refcnt[128];
    u16 iommu_did[128];
    unsigned int auxd_refcnt;
    bool has_iotlb_device;
    struct list_head devices;
    struct list_head auxd;
    struct iova_domain iovad;
    struct dma_pte *pgd;
    int gaw;
    int agaw;
    int flags;
    int iommu_coherency;
    int iommu_snooping;
    int iommu_count;
    int iommu_superpage;
    u64 max_addr;
    int default_pasid;
    struct iommu_domain domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dmar_domain {
    int nid;
    unsigned int iommu_refcnt[128];
    u16 iommu_did[128];
    unsigned int auxd_refcnt;
    bool has_iotlb_device;
    struct list_head devices;
    struct list_head auxd;
    struct iova_domain iovad;
    struct dma_pte *pgd;
    int gaw;
    int agaw;
    int flags;
    int iommu_coherency;
    int iommu_snooping;
    int iommu_count;
    int iommu_superpage;
    u64 max_addr;
    int default_pasid;
    struct iommu_domain domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dmar_domain {
    int nid;
    unsigned int iommu_refcnt[128];
    u16 iommu_did[128];
    bool has_iotlb_device;
    struct list_head devices;
    struct list_head subdevices;
    struct iova_domain iovad;
    struct dma_pte *pgd;
    int gaw;
    int agaw;
    int flags;
    int iommu_coherency;
    int iommu_snooping;
    int iommu_count;
    int iommu_superpage;
    u64 max_addr;
    u32 default_pasid;
    struct iommu_domain domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dmar_domain {
    int nid;
    unsigned int iommu_refcnt[128];
    u16 iommu_did[128];
    bool has_iotlb_device;
    struct list_head devices;
    struct list_head subdevices;
    struct iova_domain iovad;
    struct dma_pte *pgd;
    int gaw;
    int agaw;
    int flags;
    int iommu_coherency;
    int iommu_snooping;
    int iommu_count;
    int iommu_superpage;
    u64 max_addr;
    u32 default_pasid;
    struct iommu_domain domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dmar_domain {
    int nid;
    unsigned int iommu_refcnt[128];
    u16 iommu_did[128];
    u8 has_iotlb_device;
    u8 iommu_coherency;
    u8 iommu_snooping;
    struct list_head devices;
    struct list_head subdevices;
    struct iova_domain iovad;
    struct dma_pte *pgd;
    int gaw;
    int agaw;
    int flags;
    int iommu_superpage;
    u64 max_addr;
    u32 default_pasid;
    struct iommu_domain domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dmar_domain {
    int nid;
    unsigned int iommu_refcnt[128];
    u16 iommu_did[128];
    u8 has_iotlb_device;
    u8 iommu_coherency;
    u8 force_snooping;
    u8 set_pte_snp;
    struct list_head devices;
    struct iova_domain iovad;
    struct dma_pte *pgd;
    int gaw;
    int agaw;
    int flags;
    int iommu_superpage;
    u64 max_addr;
    struct iommu_domain domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dmar_domain {
    int nid;
    struct xarray iommu_array;
    u8 has_iotlb_device;
    u8 iommu_coherency;
    u8 force_snooping;
    u8 set_pte_snp;
    u8 use_first_level;
    spinlock_t lock;
    struct list_head devices;
    struct dma_pte *pgd;
    int gaw;
    int agaw;
    int iommu_superpage;
    u64 max_addr;
    struct iommu_domain domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dmar_domain {
    int nid;
    struct xarray iommu_array;
    u8 has_iotlb_device;
    u8 iommu_coherency;
    u8 force_snooping;
    u8 set_pte_snp;
    u8 use_first_level;
    spinlock_t lock;
    struct list_head devices;
    struct dma_pte *pgd;
    int gaw;
    int agaw;
    int iommu_superpage;
    u64 max_addr;
    struct iommu_domain domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dmar_domain {
    int nid;
    struct xarray iommu_array;
    u8 has_iotlb_device;
    u8 iommu_coherency;
    u8 force_snooping;
    u8 set_pte_snp;
    u8 use_first_level;
    u8 dirty_tracking;
    u8 nested_parent;
    u8 has_mappings;
    spinlock_t lock;
    struct list_head devices;
    struct list_head dev_pasids;
    int iommu_superpage;
    struct dma_pte *pgd;
    int gaw;
    int agaw;
    u64 max_addr;
    spinlock_t s1_lock;
    struct list_head s1_domains;
    struct dmar_domain *s2_domain;
    long unsigned int s1_pgtbl;
    struct iommu_hwpt_vtd_s1 s1_cfg;
    struct list_head s2_link;
    struct iommu_domain domain;
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
struct dmar_domain {
    int nid;
    unsigned int iommu_refcnt[128];
    u16 iommu_did[128];
    unsigned int auxd_refcnt;
    bool has_iotlb_device;
    struct list_head devices;
    struct list_head auxd;
    struct iova_domain iovad;
    struct dma_pte *pgd;
    int gaw;
    int agaw;
    int flags;
    int iommu_coherency;
    int iommu_snooping;
    int iommu_count;
    int iommu_superpage;
    u64 max_addr;
    int default_pasid;
    struct iommu_domain domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dmar_domain {
    int nid;
    unsigned int iommu_refcnt[128];
    u16 iommu_did[128];
    unsigned int auxd_refcnt;
    bool has_iotlb_device;
    struct list_head devices;
    struct list_head auxd;
    struct iova_domain iovad;
    struct dma_pte *pgd;
    int gaw;
    int agaw;
    int flags;
    int iommu_coherency;
    int iommu_snooping;
    int iommu_count;
    int iommu_superpage;
    u64 max_addr;
    int default_pasid;
    struct iommu_domain domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dmar_domain {
    int nid;
    unsigned int iommu_refcnt[128];
    u16 iommu_did[128];
    unsigned int auxd_refcnt;
    bool has_iotlb_device;
    struct list_head devices;
    struct list_head auxd;
    struct iova_domain iovad;
    struct dma_pte *pgd;
    int gaw;
    int agaw;
    int flags;
    int iommu_coherency;
    int iommu_snooping;
    int iommu_count;
    int iommu_superpage;
    u64 max_addr;
    int default_pasid;
    struct iommu_domain domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dmar_domain {
    int nid;
    unsigned int iommu_refcnt[128];
    u16 iommu_did[128];
    unsigned int auxd_refcnt;
    bool has_iotlb_device;
    struct list_head devices;
    struct list_head auxd;
    struct iova_domain iovad;
    struct dma_pte *pgd;
    int gaw;
    int agaw;
    int flags;
    int iommu_coherency;
    int iommu_snooping;
    int iommu_count;
    int iommu_superpage;
    u64 max_addr;
    int default_pasid;
    struct iommu_domain domain;
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
<code>bool has_iotlb_device</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
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
<code>unsigned int auxd_refcnt</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head auxd</code>
</li>
<li>
<b>Field added. </b>
<code>int default_pasid</code>
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
<code>struct list_head subdevices</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int auxd_refcnt</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head auxd</code>
</li>
<li>
<b>Field type changed. </b>
<code>int default_pasid</code> ➡️ <code>u32 default_pasid</code>
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
<code>int iommu_count</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool has_iotlb_device</code> ➡️ <code>u8 has_iotlb_device</code>
</li>
<li>
<b>Field type changed. </b>
<code>int iommu_coherency</code> ➡️ <code>u8 iommu_coherency</code>
</li>
<li>
<b>Field type changed. </b>
<code>int iommu_snooping</code> ➡️ <code>u8 iommu_snooping</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 force_snooping</code>
</li>
<li>
<b>Field added. </b>
<code>u8 set_pte_snp</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 iommu_snooping</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head subdevices</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 default_pasid</code>
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
<code>struct xarray iommu_array</code>
</li>
<li>
<b>Field added. </b>
<code>u8 use_first_level</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t lock</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int iommu_refcnt[128]</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 iommu_did[128]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct iova_domain iovad</code>
</li>
<li>
<b>Field removed. </b>
<code>int flags</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 dirty_tracking</code>
</li>
<li>
<b>Field added. </b>
<code>u8 nested_parent</code>
</li>
<li>
<b>Field added. </b>
<code>u8 has_mappings</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head dev_pasids</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t s1_lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head s1_domains</code>
</li>
<li>
<b>Field added. </b>
<code>struct dmar_domain *s2_domain</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int s1_pgtbl</code>
</li>
<li>
<b>Field added. </b>
<code>struct iommu_hwpt_vtd_s1 s1_cfg</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head s2_link</code>
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
