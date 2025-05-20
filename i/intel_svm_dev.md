# Struct: <code>intel_svm_dev</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct intel_svm_dev {
    struct list_head list;
    struct callback_head rcu;
    struct device *dev;
    struct svm_dev_ops *ops;
    int users;
    u16 did;
    u16 dev_iotlb;
    u16 sid;
    u16 qdep;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct intel_svm_dev {
    struct list_head list;
    struct callback_head rcu;
    struct device *dev;
    struct svm_dev_ops *ops;
    int users;
    u16 did;
    u16 dev_iotlb;
    u16 sid;
    u16 qdep;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct intel_svm_dev {
    struct list_head list;
    struct callback_head rcu;
    struct device *dev;
    struct svm_dev_ops *ops;
    int users;
    u16 did;
    u16 dev_iotlb;
    u16 sid;
    u16 qdep;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct intel_svm_dev {
    struct list_head list;
    struct callback_head rcu;
    struct device *dev;
    struct svm_dev_ops *ops;
    int users;
    u16 did;
    u16 dev_iotlb;
    u16 sid;
    u16 qdep;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct intel_svm_dev {
    struct list_head list;
    struct callback_head rcu;
    struct device *dev;
    struct svm_dev_ops *ops;
    int users;
    u16 did;
    u16 dev_iotlb;
    u16 sid;
    u16 qdep;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct intel_svm_dev {
    struct list_head list;
    struct callback_head rcu;
    struct device *dev;
    struct svm_dev_ops *ops;
    int users;
    u16 did;
    u16 dev_iotlb;
    u16 sid;
    u16 qdep;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct intel_svm_dev {
    struct list_head list;
    struct callback_head rcu;
    struct device *dev;
    struct svm_dev_ops *ops;
    int users;
    u16 did;
    u16 dev_iotlb;
    u16 sid;
    u16 qdep;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct intel_svm_dev {
    struct list_head list;
    struct callback_head rcu;
    struct device *dev;
    struct svm_dev_ops *ops;
    int users;
    u16 did;
    u16 dev_iotlb;
    u16 sid;
    u16 qdep;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct intel_svm_dev {
    struct list_head list;
    struct callback_head rcu;
    struct device *dev;
    struct svm_dev_ops *ops;
    int users;
    u16 did;
    u16 dev_iotlb;
    u16 sid;
    u16 qdep;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct intel_svm_dev {
    struct list_head list;
    struct callback_head rcu;
    struct device *dev;
    struct svm_dev_ops *ops;
    struct iommu_sva sva;
    int pasid;
    int users;
    u16 did;
    u16 dev_iotlb;
    u16 sid;
    u16 qdep;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct intel_svm_dev {
    struct list_head list;
    struct callback_head rcu;
    struct device *dev;
    struct intel_iommu *iommu;
    struct svm_dev_ops *ops;
    struct iommu_sva sva;
    u32 pasid;
    int users;
    u16 did;
    u16 dev_iotlb;
    u16 sid;
    u16 qdep;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct intel_svm_dev {
    struct list_head list;
    struct callback_head rcu;
    struct device *dev;
    struct intel_iommu *iommu;
    struct iommu_sva sva;
    u32 pasid;
    int users;
    u16 did;
    u16 dev_iotlb;
    u16 sid;
    u16 qdep;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct intel_svm_dev {
    struct list_head list;
    struct callback_head rcu;
    struct device *dev;
    struct intel_iommu *iommu;
    struct iommu_sva sva;
    long unsigned int prq_seq_number;
    u32 pasid;
    int users;
    u16 did;
    u16 dev_iotlb;
    u16 sid;
    u16 qdep;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct intel_svm_dev {
    struct list_head list;
    struct callback_head rcu;
    struct device *dev;
    struct intel_iommu *iommu;
    struct iommu_sva sva;
    long unsigned int prq_seq_number;
    u32 pasid;
    int users;
    u16 did;
    u16 dev_iotlb;
    u16 sid;
    u16 qdep;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct intel_svm_dev {
    struct list_head list;
    struct callback_head rcu;
    struct device *dev;
    struct intel_iommu *iommu;
    struct iommu_sva sva;
    u32 pasid;
    int users;
    u16 did;
    u16 dev_iotlb;
    u16 sid;
    u16 qdep;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct intel_svm_dev {
    struct list_head list;
    struct callback_head rcu;
    struct device *dev;
    struct intel_iommu *iommu;
    u16 did;
    u16 sid;
    u16 qdep;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct intel_svm_dev {
    struct list_head list;
    struct callback_head rcu;
    struct device *dev;
    struct intel_iommu *iommu;
    u16 did;
    u16 sid;
    u16 qdep;
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
struct intel_svm_dev {
    struct list_head list;
    struct callback_head rcu;
    struct device *dev;
    struct svm_dev_ops *ops;
    int users;
    u16 did;
    u16 dev_iotlb;
    u16 sid;
    u16 qdep;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct intel_svm_dev {
    struct list_head list;
    struct callback_head rcu;
    struct device *dev;
    struct svm_dev_ops *ops;
    int users;
    u16 did;
    u16 dev_iotlb;
    u16 sid;
    u16 qdep;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct intel_svm_dev {
    struct list_head list;
    struct callback_head rcu;
    struct device *dev;
    struct svm_dev_ops *ops;
    int users;
    u16 did;
    u16 dev_iotlb;
    u16 sid;
    u16 qdep;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct intel_svm_dev {
    struct list_head list;
    struct callback_head rcu;
    struct device *dev;
    struct svm_dev_ops *ops;
    int users;
    u16 did;
    u16 dev_iotlb;
    u16 sid;
    u16 qdep;
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct iommu_sva sva</code>
</li>
<li>
<b>Field added. </b>
<code>int pasid</code>
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
<code>struct intel_iommu *iommu</code>
</li>
<li>
<b>Field type changed. </b>
<code>int pasid</code> ➡️ <code>u32 pasid</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct svm_dev_ops *ops</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int prq_seq_number</code>
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
<b>Field removed. </b>
<code>long unsigned int prq_seq_number</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct iommu_sva sva</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 pasid</code>
</li>
<li>
<b>Field removed. </b>
<code>int users</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 dev_iotlb</code>
</li>
</ul>
</details>
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
