# Struct: <code>device_domain_info</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct device_domain_info {
    struct list_head link;
    struct list_head global;
    u8 bus;
    u8 devfn;
    u8 pasid_supported;
    u8 pasid_enabled;
    u8 pri_supported;
    u8 pri_enabled;
    u8 ats_supported;
    u8 ats_enabled;
    u8 ats_qdep;
    struct device *dev;
    struct intel_iommu *iommu;
    struct dmar_domain *domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct device_domain_info {
    struct list_head link;
    struct list_head global;
    u8 bus;
    u8 devfn;
    u8 pasid_supported;
    u8 pasid_enabled;
    u8 pri_supported;
    u8 pri_enabled;
    u8 ats_supported;
    u8 ats_enabled;
    u8 ats_qdep;
    struct device *dev;
    struct intel_iommu *iommu;
    struct dmar_domain *domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct device_domain_info {
    struct list_head link;
    struct list_head global;
    u8 bus;
    u8 devfn;
    u8 pasid_supported;
    u8 pasid_enabled;
    u8 pri_supported;
    u8 pri_enabled;
    u8 ats_supported;
    u8 ats_enabled;
    u8 ats_qdep;
    struct device *dev;
    struct intel_iommu *iommu;
    struct dmar_domain *domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct device_domain_info {
    struct list_head link;
    struct list_head global;
    u8 bus;
    u8 devfn;
    u8 pasid_supported;
    u8 pasid_enabled;
    u8 pri_supported;
    u8 pri_enabled;
    u8 ats_supported;
    u8 ats_enabled;
    u8 ats_qdep;
    struct device *dev;
    struct intel_iommu *iommu;
    struct dmar_domain *domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct device_domain_info {
    struct list_head link;
    struct list_head global;
    u8 bus;
    u8 devfn;
    u8 pasid_supported;
    u8 pasid_enabled;
    u8 pri_supported;
    u8 pri_enabled;
    u8 ats_supported;
    u8 ats_enabled;
    u8 ats_qdep;
    struct device *dev;
    struct intel_iommu *iommu;
    struct dmar_domain *domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct device_domain_info {
    struct list_head link;
    struct list_head global;
    u8 bus;
    u8 devfn;
    u16 pfsid;
    u8 pasid_supported;
    u8 pasid_enabled;
    u8 pri_supported;
    u8 pri_enabled;
    u8 ats_supported;
    u8 ats_enabled;
    u8 ats_qdep;
    struct device *dev;
    struct intel_iommu *iommu;
    struct dmar_domain *domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct device_domain_info {
    struct list_head link;
    struct list_head global;
    struct list_head table;
    u8 bus;
    u8 devfn;
    u16 pfsid;
    u8 pasid_supported;
    u8 pasid_enabled;
    u8 pri_supported;
    u8 pri_enabled;
    u8 ats_supported;
    u8 ats_enabled;
    u8 ats_qdep;
    struct device *dev;
    struct intel_iommu *iommu;
    struct dmar_domain *domain;
    struct pasid_table *pasid_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct device_domain_info {
    struct list_head link;
    struct list_head global;
    struct list_head table;
    struct list_head auxiliary_domains;
    u8 bus;
    u8 devfn;
    u16 pfsid;
    u8 pasid_supported;
    u8 pasid_enabled;
    u8 pri_supported;
    u8 pri_enabled;
    u8 ats_supported;
    u8 ats_enabled;
    u8 auxd_enabled;
    u8 ats_qdep;
    struct device *dev;
    struct intel_iommu *iommu;
    struct dmar_domain *domain;
    struct pasid_table *pasid_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct device_domain_info {
    struct list_head link;
    struct list_head global;
    struct list_head table;
    struct list_head auxiliary_domains;
    u8 bus;
    u8 devfn;
    u16 pfsid;
    u8 pasid_supported;
    u8 pasid_enabled;
    u8 pri_supported;
    u8 pri_enabled;
    u8 ats_supported;
    u8 ats_enabled;
    u8 auxd_enabled;
    u8 ats_qdep;
    struct device *dev;
    struct intel_iommu *iommu;
    struct dmar_domain *domain;
    struct pasid_table *pasid_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct device_domain_info {
    struct list_head link;
    struct list_head global;
    struct list_head table;
    struct list_head auxiliary_domains;
    u32 segment;
    u8 bus;
    u8 devfn;
    u16 pfsid;
    u8 pasid_supported;
    u8 pasid_enabled;
    u8 pri_supported;
    u8 pri_enabled;
    u8 ats_supported;
    u8 ats_enabled;
    u8 auxd_enabled;
    u8 ats_qdep;
    struct device *dev;
    struct intel_iommu *iommu;
    struct dmar_domain *domain;
    struct pasid_table *pasid_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct device_domain_info {
    struct list_head link;
    struct list_head global;
    struct list_head table;
    struct list_head subdevices;
    u32 segment;
    u8 bus;
    u8 devfn;
    u16 pfsid;
    u8 pasid_supported;
    u8 pasid_enabled;
    u8 pri_supported;
    u8 pri_enabled;
    u8 ats_supported;
    u8 ats_enabled;
    u8 auxd_enabled;
    u8 ats_qdep;
    struct device *dev;
    struct intel_iommu *iommu;
    struct dmar_domain *domain;
    struct pasid_table *pasid_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct device_domain_info {
    struct list_head link;
    struct list_head global;
    struct list_head table;
    struct list_head subdevices;
    u32 segment;
    u8 bus;
    u8 devfn;
    u16 pfsid;
    u8 pasid_supported;
    u8 pasid_enabled;
    u8 pri_supported;
    u8 pri_enabled;
    u8 ats_supported;
    u8 ats_enabled;
    u8 auxd_enabled;
    u8 ats_qdep;
    struct device *dev;
    struct intel_iommu *iommu;
    struct dmar_domain *domain;
    struct pasid_table *pasid_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct device_domain_info {
    struct list_head link;
    struct list_head global;
    struct list_head table;
    struct list_head subdevices;
    u32 segment;
    u8 bus;
    u8 devfn;
    u16 pfsid;
    u8 pasid_supported;
    u8 pasid_enabled;
    u8 pri_supported;
    u8 pri_enabled;
    u8 ats_supported;
    u8 ats_enabled;
    u8 auxd_enabled;
    u8 ats_qdep;
    struct device *dev;
    struct intel_iommu *iommu;
    struct dmar_domain *domain;
    struct pasid_table *pasid_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct device_domain_info {
    struct list_head link;
    struct list_head global;
    u32 segment;
    u8 bus;
    u8 devfn;
    u16 pfsid;
    u8 pasid_supported;
    u8 pasid_enabled;
    u8 pri_supported;
    u8 pri_enabled;
    u8 ats_supported;
    u8 ats_enabled;
    u8 ats_qdep;
    struct device *dev;
    struct intel_iommu *iommu;
    struct dmar_domain *domain;
    struct pasid_table *pasid_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct device_domain_info {
    struct list_head link;
    u32 segment;
    u8 bus;
    u8 devfn;
    u16 pfsid;
    u8 pasid_supported;
    u8 pasid_enabled;
    u8 pri_supported;
    u8 pri_enabled;
    u8 ats_supported;
    u8 ats_enabled;
    u8 dtlb_extra_inval;
    u8 ats_qdep;
    struct device *dev;
    struct intel_iommu *iommu;
    struct dmar_domain *domain;
    struct pasid_table *pasid_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct device_domain_info {
    struct list_head link;
    u32 segment;
    u8 bus;
    u8 devfn;
    u16 pfsid;
    u8 pasid_supported;
    u8 pasid_enabled;
    u8 pri_supported;
    u8 pri_enabled;
    u8 ats_supported;
    u8 ats_enabled;
    u8 dtlb_extra_inval;
    u8 ats_qdep;
    struct device *dev;
    struct intel_iommu *iommu;
    struct dmar_domain *domain;
    struct pasid_table *pasid_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct device_domain_info {
    struct list_head link;
    u32 segment;
    u8 bus;
    u8 devfn;
    u16 pfsid;
    u8 pasid_supported;
    u8 pasid_enabled;
    u8 pri_supported;
    u8 pri_enabled;
    u8 ats_supported;
    u8 ats_enabled;
    u8 dtlb_extra_inval;
    u8 ats_qdep;
    struct device *dev;
    struct intel_iommu *iommu;
    struct dmar_domain *domain;
    struct pasid_table *pasid_table;
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
struct device_domain_info {
    struct list_head link;
    struct list_head global;
    struct list_head table;
    struct list_head auxiliary_domains;
    u8 bus;
    u8 devfn;
    u16 pfsid;
    u8 pasid_supported;
    u8 pasid_enabled;
    u8 pri_supported;
    u8 pri_enabled;
    u8 ats_supported;
    u8 ats_enabled;
    u8 auxd_enabled;
    u8 ats_qdep;
    struct device *dev;
    struct intel_iommu *iommu;
    struct dmar_domain *domain;
    struct pasid_table *pasid_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct device_domain_info {
    struct list_head link;
    struct list_head global;
    struct list_head table;
    struct list_head auxiliary_domains;
    u8 bus;
    u8 devfn;
    u16 pfsid;
    u8 pasid_supported;
    u8 pasid_enabled;
    u8 pri_supported;
    u8 pri_enabled;
    u8 ats_supported;
    u8 ats_enabled;
    u8 auxd_enabled;
    u8 ats_qdep;
    struct device *dev;
    struct intel_iommu *iommu;
    struct dmar_domain *domain;
    struct pasid_table *pasid_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct device_domain_info {
    struct list_head link;
    struct list_head global;
    struct list_head table;
    struct list_head auxiliary_domains;
    u8 bus;
    u8 devfn;
    u16 pfsid;
    u8 pasid_supported;
    u8 pasid_enabled;
    u8 pri_supported;
    u8 pri_enabled;
    u8 ats_supported;
    u8 ats_enabled;
    u8 auxd_enabled;
    u8 ats_qdep;
    struct device *dev;
    struct intel_iommu *iommu;
    struct dmar_domain *domain;
    struct pasid_table *pasid_table;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct device_domain_info {
    struct list_head link;
    struct list_head global;
    struct list_head table;
    struct list_head auxiliary_domains;
    u8 bus;
    u8 devfn;
    u16 pfsid;
    u8 pasid_supported;
    u8 pasid_enabled;
    u8 pri_supported;
    u8 pri_enabled;
    u8 ats_supported;
    u8 ats_enabled;
    u8 auxd_enabled;
    u8 ats_qdep;
    struct device *dev;
    struct intel_iommu *iommu;
    struct dmar_domain *domain;
    struct pasid_table *pasid_table;
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
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 pfsid</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head table</code>
</li>
<li>
<b>Field added. </b>
<code>struct pasid_table *pasid_table</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head auxiliary_domains</code>
</li>
<li>
<b>Field added. </b>
<code>u8 auxd_enabled</code>
</li>
</ul>
</details>
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
<code>u32 segment</code>
</li>
</ul>
</details>
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
<code>struct list_head auxiliary_domains</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct list_head table</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head subdevices</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 auxd_enabled</code>
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
<code>u8 dtlb_extra_inval</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head global</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
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
