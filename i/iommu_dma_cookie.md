# Struct: <code>iommu_dma_cookie</code>

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
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct iommu_dma_cookie {
    enum iommu_dma_cookie_type type;
    struct iova_domain iovad;
    dma_addr_t msi_iova;
    struct list_head msi_page_list;
    struct iommu_domain *fq_domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct iommu_dma_cookie {
    enum iommu_dma_cookie_type type;
    struct iova_domain iovad;
    dma_addr_t msi_iova;
    struct list_head msi_page_list;
    struct iommu_domain *fq_domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct iommu_dma_cookie {
    enum iommu_dma_cookie_type type;
    struct iova_domain iovad;
    dma_addr_t msi_iova;
    struct list_head msi_page_list;
    struct iommu_domain *fq_domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct iommu_dma_cookie {
    enum iommu_dma_cookie_type type;
    struct iova_domain iovad;
    dma_addr_t msi_iova;
    struct list_head msi_page_list;
    struct iommu_domain *fq_domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct iommu_dma_cookie {
    enum iommu_dma_cookie_type type;
    struct iova_domain iovad;
    struct iova_fq *fq;
    atomic64_t fq_flush_start_cnt;
    atomic64_t fq_flush_finish_cnt;
    struct timer_list fq_timer;
    atomic_t fq_timer_on;
    dma_addr_t msi_iova;
    struct list_head msi_page_list;
    struct iommu_domain *fq_domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct iommu_dma_cookie {
    enum iommu_dma_cookie_type type;
    struct iova_domain iovad;
    struct iova_fq *fq;
    atomic64_t fq_flush_start_cnt;
    atomic64_t fq_flush_finish_cnt;
    struct timer_list fq_timer;
    atomic_t fq_timer_on;
    dma_addr_t msi_iova;
    struct list_head msi_page_list;
    struct iommu_domain *fq_domain;
    struct mutex mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct iommu_dma_cookie {
    enum iommu_dma_cookie_type type;
    struct iova_domain iovad;
    struct iova_fq *fq;
    atomic64_t fq_flush_start_cnt;
    atomic64_t fq_flush_finish_cnt;
    struct timer_list fq_timer;
    atomic_t fq_timer_on;
    dma_addr_t msi_iova;
    struct list_head msi_page_list;
    struct iommu_domain *fq_domain;
    struct mutex mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct iommu_dma_cookie {
    enum iommu_dma_cookie_type type;
    struct iova_domain iovad;
    struct iova_fq *single_fq;
    struct iova_fq *percpu_fq;
    atomic64_t fq_flush_start_cnt;
    atomic64_t fq_flush_finish_cnt;
    struct timer_list fq_timer;
    atomic_t fq_timer_on;
    dma_addr_t msi_iova;
    struct list_head msi_page_list;
    struct iommu_domain *fq_domain;
    struct iommu_dma_options options;
    struct mutex mutex;
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct iommu_dma_cookie {
    enum iommu_dma_cookie_type type;
    struct iova_domain iovad;
    dma_addr_t msi_iova;
    struct list_head msi_page_list;
    struct iommu_domain *fq_domain;
};
```
</details>
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
<b>Regular</b>
<ul>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
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
<b>Field added. </b>
<code>struct iova_fq *fq</code>
</li>
<li>
<b>Field added. </b>
<code>atomic64_t fq_flush_start_cnt</code>
</li>
<li>
<b>Field added. </b>
<code>atomic64_t fq_flush_finish_cnt</code>
</li>
<li>
<b>Field added. </b>
<code>struct timer_list fq_timer</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t fq_timer_on</code>
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
<code>struct mutex mutex</code>
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
<code>struct iova_fq *single_fq</code>
</li>
<li>
<b>Field added. </b>
<code>struct iova_fq *percpu_fq</code>
</li>
<li>
<b>Field added. </b>
<code>struct iommu_dma_options options</code>
</li>
<li>
<b>Field removed. </b>
<code>struct iova_fq *fq</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Arch</b>
<ul>
</ul>
