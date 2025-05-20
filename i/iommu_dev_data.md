# Struct: <code>iommu_dev_data</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct iommu_dev_data {
    struct list_head list;
    struct list_head dev_data_list;
    struct protection_domain *domain;
    u16 devid;
    bool iommu_v2;
    bool passthrough;
    struct (anon) ats;
    bool pri_tlp;
    u32 errata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct iommu_dev_data {
    struct list_head list;
    struct list_head dev_data_list;
    struct protection_domain *domain;
    u16 devid;
    u16 alias;
    bool iommu_v2;
    bool passthrough;
    struct (anon) ats;
    bool pri_tlp;
    u32 errata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct iommu_dev_data {
    struct list_head list;
    struct list_head dev_data_list;
    struct protection_domain *domain;
    u16 devid;
    u16 alias;
    bool iommu_v2;
    bool passthrough;
    struct (anon) ats;
    bool pri_tlp;
    u32 errata;
    bool use_vapic;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct iommu_dev_data {
    struct list_head list;
    struct list_head dev_data_list;
    struct protection_domain *domain;
    u16 devid;
    u16 alias;
    bool iommu_v2;
    bool passthrough;
    struct (anon) ats;
    bool pri_tlp;
    u32 errata;
    bool use_vapic;
    struct ratelimit_state rs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct iommu_dev_data {
    struct list_head list;
    struct list_head dev_data_list;
    struct protection_domain *domain;
    u16 devid;
    u16 alias;
    bool iommu_v2;
    bool passthrough;
    struct (anon) ats;
    bool pri_tlp;
    u32 errata;
    bool use_vapic;
    bool defer_attach;
    struct ratelimit_state rs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct iommu_dev_data {
    struct list_head list;
    struct llist_node dev_data_list;
    struct protection_domain *domain;
    u16 devid;
    u16 alias;
    bool iommu_v2;
    bool passthrough;
    struct (anon) ats;
    bool pri_tlp;
    u32 errata;
    bool use_vapic;
    bool defer_attach;
    struct ratelimit_state rs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct iommu_dev_data {
    struct list_head list;
    struct llist_node dev_data_list;
    struct protection_domain *domain;
    u16 devid;
    u16 alias;
    bool iommu_v2;
    bool passthrough;
    struct (anon) ats;
    bool pri_tlp;
    u32 errata;
    bool use_vapic;
    bool defer_attach;
    struct ratelimit_state rs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct iommu_dev_data {
    struct list_head list;
    struct llist_node dev_data_list;
    struct protection_domain *domain;
    u16 devid;
    u16 alias;
    bool iommu_v2;
    bool passthrough;
    struct (anon) ats;
    bool pri_tlp;
    u32 errata;
    bool use_vapic;
    bool defer_attach;
    struct ratelimit_state rs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct iommu_dev_data {
    spinlock_t lock;
    struct list_head list;
    struct llist_node dev_data_list;
    struct protection_domain *domain;
    struct pci_dev *pdev;
    u16 devid;
    bool iommu_v2;
    bool passthrough;
    struct (anon) ats;
    bool pri_tlp;
    u32 errata;
    bool use_vapic;
    bool defer_attach;
    struct ratelimit_state rs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct iommu_dev_data {
    spinlock_t lock;
    struct list_head list;
    struct llist_node dev_data_list;
    struct protection_domain *domain;
    struct pci_dev *pdev;
    u16 devid;
    bool iommu_v2;
    struct (anon) ats;
    bool pri_tlp;
    u32 errata;
    bool use_vapic;
    bool defer_attach;
    struct ratelimit_state rs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct iommu_dev_data {
    spinlock_t lock;
    struct list_head list;
    struct llist_node dev_data_list;
    struct protection_domain *domain;
    struct pci_dev *pdev;
    u16 devid;
    bool iommu_v2;
    struct (anon) ats;
    bool pri_tlp;
    u32 errata;
    bool use_vapic;
    bool defer_attach;
    struct ratelimit_state rs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct iommu_dev_data {
    spinlock_t lock;
    struct list_head list;
    struct llist_node dev_data_list;
    struct protection_domain *domain;
    struct pci_dev *pdev;
    u16 devid;
    bool iommu_v2;
    struct (anon) ats;
    bool pri_tlp;
    bool use_vapic;
    bool defer_attach;
    struct ratelimit_state rs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct iommu_dev_data {
    spinlock_t lock;
    struct list_head list;
    struct llist_node dev_data_list;
    struct protection_domain *domain;
    struct pci_dev *pdev;
    u16 devid;
    bool iommu_v2;
    struct (anon) ats;
    bool pri_tlp;
    bool use_vapic;
    bool defer_attach;
    struct ratelimit_state rs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct iommu_dev_data {
    spinlock_t lock;
    struct list_head list;
    struct llist_node dev_data_list;
    struct protection_domain *domain;
    struct pci_dev *pdev;
    u16 devid;
    bool iommu_v2;
    struct (anon) ats;
    bool pri_tlp;
    bool use_vapic;
    bool defer_attach;
    struct ratelimit_state rs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct iommu_dev_data {
    spinlock_t lock;
    struct list_head list;
    struct llist_node dev_data_list;
    struct protection_domain *domain;
    struct device *dev;
    u16 devid;
    bool iommu_v2;
    struct (anon) ats;
    bool pri_tlp;
    bool use_vapic;
    bool defer_attach;
    struct ratelimit_state rs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct iommu_dev_data {
    spinlock_t lock;
    struct list_head list;
    struct llist_node dev_data_list;
    struct protection_domain *domain;
    struct device *dev;
    u16 devid;
    bool iommu_v2;
    struct (anon) ats;
    bool pri_tlp;
    bool use_vapic;
    bool defer_attach;
    struct ratelimit_state rs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct iommu_dev_data {
    spinlock_t lock;
    struct list_head list;
    struct llist_node dev_data_list;
    struct protection_domain *domain;
    struct device *dev;
    u16 devid;
    u32 flags;
    int ats_qdep;
    u8 ats_enabled;
    u8 pri_enabled;
    u8 pasid_enabled;
    u8 pri_tlp;
    u8 ppr;
    bool use_vapic;
    bool defer_attach;
    struct ratelimit_state rs;
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
struct iommu_dev_data {
    spinlock_t lock;
    struct list_head list;
    struct llist_node dev_data_list;
    struct protection_domain *domain;
    struct pci_dev *pdev;
    u16 devid;
    bool iommu_v2;
    bool passthrough;
    struct (anon) ats;
    bool pri_tlp;
    u32 errata;
    bool use_vapic;
    bool defer_attach;
    struct ratelimit_state rs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct iommu_dev_data {
    spinlock_t lock;
    struct list_head list;
    struct llist_node dev_data_list;
    struct protection_domain *domain;
    struct pci_dev *pdev;
    u16 devid;
    bool iommu_v2;
    bool passthrough;
    struct (anon) ats;
    bool pri_tlp;
    u32 errata;
    bool use_vapic;
    bool defer_attach;
    struct ratelimit_state rs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct iommu_dev_data {
    spinlock_t lock;
    struct list_head list;
    struct llist_node dev_data_list;
    struct protection_domain *domain;
    struct pci_dev *pdev;
    u16 devid;
    bool iommu_v2;
    bool passthrough;
    struct (anon) ats;
    bool pri_tlp;
    u32 errata;
    bool use_vapic;
    bool defer_attach;
    struct ratelimit_state rs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct iommu_dev_data {
    spinlock_t lock;
    struct list_head list;
    struct llist_node dev_data_list;
    struct protection_domain *domain;
    struct pci_dev *pdev;
    u16 devid;
    bool iommu_v2;
    bool passthrough;
    struct (anon) ats;
    bool pri_tlp;
    u32 errata;
    bool use_vapic;
    bool defer_attach;
    struct ratelimit_state rs;
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
<code>u16 alias</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool use_vapic</code>
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
<code>struct ratelimit_state rs</code>
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
<code>bool defer_attach</code>
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
<code>struct list_head dev_data_list</code> ➡️ <code>struct llist_node dev_data_list</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>spinlock_t lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct pci_dev *pdev</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 alias</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>bool passthrough</code>
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
<b>Field removed. </b>
<code>u32 errata</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
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
<code>struct device *dev</code>
</li>
<li>
<b>Field removed. </b>
<code>struct pci_dev *pdev</code>
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
<code>u32 flags</code>
</li>
<li>
<b>Field added. </b>
<code>int ats_qdep</code>
</li>
<li>
<b>Field added. </b>
<code>u8 ats_enabled</code>
</li>
<li>
<b>Field added. </b>
<code>u8 pri_enabled</code>
</li>
<li>
<b>Field added. </b>
<code>u8 pasid_enabled</code>
</li>
<li>
<b>Field added. </b>
<code>u8 ppr</code>
</li>
<li>
<b>Field removed. </b>
<code>bool iommu_v2</code>
</li>
<li>
<b>Field removed. </b>
<code>struct (anon) ats</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool pri_tlp</code> ➡️ <code>u8 pri_tlp</code>
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
