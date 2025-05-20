# Struct: <code>iommu_domain</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct iommu_domain {
    unsigned int type;
    const struct iommu_ops *ops;
    iommu_fault_handler_t handler;
    void *handler_token;
    struct iommu_domain_geometry geometry;
    void *iova_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct iommu_domain {
    unsigned int type;
    const struct iommu_ops *ops;
    long unsigned int pgsize_bitmap;
    iommu_fault_handler_t handler;
    void *handler_token;
    struct iommu_domain_geometry geometry;
    void *iova_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct iommu_domain {
    unsigned int type;
    const struct iommu_ops *ops;
    long unsigned int pgsize_bitmap;
    iommu_fault_handler_t handler;
    void *handler_token;
    struct iommu_domain_geometry geometry;
    void *iova_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct iommu_domain {
    unsigned int type;
    const struct iommu_ops *ops;
    long unsigned int pgsize_bitmap;
    iommu_fault_handler_t handler;
    void *handler_token;
    struct iommu_domain_geometry geometry;
    void *iova_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct iommu_domain {
    unsigned int type;
    const struct iommu_ops *ops;
    long unsigned int pgsize_bitmap;
    iommu_fault_handler_t handler;
    void *handler_token;
    struct iommu_domain_geometry geometry;
    void *iova_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct iommu_domain {
    unsigned int type;
    const struct iommu_ops *ops;
    long unsigned int pgsize_bitmap;
    iommu_fault_handler_t handler;
    void *handler_token;
    struct iommu_domain_geometry geometry;
    void *iova_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct iommu_domain {
    unsigned int type;
    const struct iommu_ops *ops;
    long unsigned int pgsize_bitmap;
    iommu_fault_handler_t handler;
    void *handler_token;
    struct iommu_domain_geometry geometry;
    void *iova_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct iommu_domain {
    unsigned int type;
    const struct iommu_ops *ops;
    long unsigned int pgsize_bitmap;
    iommu_fault_handler_t handler;
    void *handler_token;
    struct iommu_domain_geometry geometry;
    void *iova_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct iommu_domain {
    unsigned int type;
    const struct iommu_ops *ops;
    long unsigned int pgsize_bitmap;
    iommu_fault_handler_t handler;
    void *handler_token;
    struct iommu_domain_geometry geometry;
    void *iova_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct iommu_domain {
    unsigned int type;
    const struct iommu_ops *ops;
    long unsigned int pgsize_bitmap;
    iommu_fault_handler_t handler;
    void *handler_token;
    struct iommu_domain_geometry geometry;
    void *iova_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct iommu_domain {
    unsigned int type;
    const struct iommu_ops *ops;
    long unsigned int pgsize_bitmap;
    iommu_fault_handler_t handler;
    void *handler_token;
    struct iommu_domain_geometry geometry;
    void *iova_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct iommu_domain {
    unsigned int type;
    const struct iommu_ops *ops;
    long unsigned int pgsize_bitmap;
    iommu_fault_handler_t handler;
    void *handler_token;
    struct iommu_domain_geometry geometry;
    void *iova_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct iommu_domain {
    unsigned int type;
    const struct iommu_ops *ops;
    long unsigned int pgsize_bitmap;
    iommu_fault_handler_t handler;
    void *handler_token;
    struct iommu_domain_geometry geometry;
    struct iommu_dma_cookie *iova_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct iommu_domain {
    unsigned int type;
    const struct iommu_domain_ops *ops;
    long unsigned int pgsize_bitmap;
    iommu_fault_handler_t handler;
    void *handler_token;
    struct iommu_domain_geometry geometry;
    struct iommu_dma_cookie *iova_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct iommu_domain {
    unsigned int type;
    const struct iommu_domain_ops *ops;
    long unsigned int pgsize_bitmap;
    struct iommu_domain_geometry geometry;
    struct iommu_dma_cookie *iova_cookie;
    enum iommu_page_response_code (*iopf_handler)(struct iommu_fault *, void *);
    void *fault_data;
    iommu_fault_handler_t handler;
    void *handler_token;
    struct mm_struct *mm;
    int users;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct iommu_domain {
    unsigned int type;
    const struct iommu_domain_ops *ops;
    long unsigned int pgsize_bitmap;
    struct iommu_domain_geometry geometry;
    struct iommu_dma_cookie *iova_cookie;
    enum iommu_page_response_code (*iopf_handler)(struct iommu_fault *, void *);
    void *fault_data;
    iommu_fault_handler_t handler;
    void *handler_token;
    struct mm_struct *mm;
    int users;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct iommu_domain {
    unsigned int type;
    const struct iommu_domain_ops *ops;
    const struct iommu_dirty_ops *dirty_ops;
    const struct iommu_ops *owner;
    long unsigned int pgsize_bitmap;
    struct iommu_domain_geometry geometry;
    struct iommu_dma_cookie *iova_cookie;
    enum iommu_page_response_code (*iopf_handler)(struct iommu_fault *, void *);
    void *fault_data;
    iommu_fault_handler_t handler;
    void *handler_token;
    struct mm_struct *mm;
    int users;
    struct list_head next;
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
struct iommu_domain {
    unsigned int type;
    const struct iommu_ops *ops;
    long unsigned int pgsize_bitmap;
    iommu_fault_handler_t handler;
    void *handler_token;
    struct iommu_domain_geometry geometry;
    void *iova_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct iommu_domain {
    unsigned int type;
    const struct iommu_ops *ops;
    long unsigned int pgsize_bitmap;
    iommu_fault_handler_t handler;
    void *handler_token;
    struct iommu_domain_geometry geometry;
    void *iova_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct iommu_domain {
    unsigned int type;
    const struct iommu_ops *ops;
    long unsigned int pgsize_bitmap;
    iommu_fault_handler_t handler;
    void *handler_token;
    struct iommu_domain_geometry geometry;
    void *iova_cookie;
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct iommu_domain {
    unsigned int type;
    const struct iommu_ops *ops;
    long unsigned int pgsize_bitmap;
    iommu_fault_handler_t handler;
    void *handler_token;
    struct iommu_domain_geometry geometry;
    void *iova_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct iommu_domain {
    unsigned int type;
    const struct iommu_ops *ops;
    long unsigned int pgsize_bitmap;
    iommu_fault_handler_t handler;
    void *handler_token;
    struct iommu_domain_geometry geometry;
    void *iova_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct iommu_domain {
    unsigned int type;
    const struct iommu_ops *ops;
    long unsigned int pgsize_bitmap;
    iommu_fault_handler_t handler;
    void *handler_token;
    struct iommu_domain_geometry geometry;
    void *iova_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct iommu_domain {
    unsigned int type;
    const struct iommu_ops *ops;
    long unsigned int pgsize_bitmap;
    iommu_fault_handler_t handler;
    void *handler_token;
    struct iommu_domain_geometry geometry;
    void *iova_cookie;
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
<code>long unsigned int pgsize_bitmap</code>
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
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
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
<b>Field type changed. </b>
<code>void *iova_cookie</code> ➡️ <code>struct iommu_dma_cookie *iova_cookie</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>const struct iommu_ops *ops</code> ➡️ <code>const struct iommu_domain_ops *ops</code>
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
<code>enum iommu_page_response_code (*iopf_handler)(struct iommu_fault *, void *)</code>
</li>
<li>
<b>Field added. </b>
<code>void *fault_data</code>
</li>
<li>
<b>Field added. </b>
<code>struct mm_struct *mm</code>
</li>
<li>
<b>Field added. </b>
<code>int users</code>
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
<code>const struct iommu_dirty_ops *dirty_ops</code>
</li>
<li>
<b>Field added. </b>
<code>const struct iommu_ops *owner</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head next</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>armhf</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
</li>
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
