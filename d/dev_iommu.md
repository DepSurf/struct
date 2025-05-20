# Struct: <code>dev_iommu</code>

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
struct dev_iommu {
    struct mutex lock;
    struct iommu_fault_param *fault_param;
    struct iommu_fwspec *fwspec;
    struct iommu_device *iommu_dev;
    void *priv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dev_iommu {
    struct mutex lock;
    struct iommu_fault_param *fault_param;
    struct iommu_fwspec *fwspec;
    struct iommu_device *iommu_dev;
    void *priv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dev_iommu {
    struct mutex lock;
    struct iommu_fault_param *fault_param;
    struct iopf_device_param *iopf_param;
    struct iommu_fwspec *fwspec;
    struct iommu_device *iommu_dev;
    void *priv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dev_iommu {
    struct mutex lock;
    struct iommu_fault_param *fault_param;
    struct iopf_device_param *iopf_param;
    struct iommu_fwspec *fwspec;
    struct iommu_device *iommu_dev;
    void *priv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dev_iommu {
    struct mutex lock;
    struct iommu_fault_param *fault_param;
    struct iopf_device_param *iopf_param;
    struct iommu_fwspec *fwspec;
    struct iommu_device *iommu_dev;
    void *priv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dev_iommu {
    struct mutex lock;
    struct iommu_fault_param *fault_param;
    struct iopf_device_param *iopf_param;
    struct iommu_fwspec *fwspec;
    struct iommu_device *iommu_dev;
    void *priv;
    u32 max_pasids;
    u32 attach_deferred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dev_iommu {
    struct mutex lock;
    struct iommu_fault_param *fault_param;
    struct iopf_device_param *iopf_param;
    struct iommu_fwspec *fwspec;
    struct iommu_device *iommu_dev;
    void *priv;
    u32 max_pasids;
    u32 attach_deferred;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dev_iommu {
    struct mutex lock;
    struct iommu_fault_param *fault_param;
    struct iopf_device_param *iopf_param;
    struct iommu_fwspec *fwspec;
    struct iommu_device *iommu_dev;
    void *priv;
    u32 max_pasids;
    u32 attach_deferred;
    u32 pci_32bit_workaround;
    u32 require_direct;
    u32 shadow_on_flush;
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
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct iopf_device_param *iopf_param</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct iopf_device_param *iopf_param</code> ➡️ <code>struct iopf_device_param *iopf_param</code>
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
<code>u32 max_pasids</code>
</li>
<li>
<b>Field added. </b>
<code>u32 attach_deferred</code>
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
<code>u32 pci_32bit_workaround</code>
</li>
<li>
<b>Field added. </b>
<code>u32 require_direct</code>
</li>
<li>
<b>Field added. </b>
<code>u32 shadow_on_flush</code>
</li>
</ul>
</details>
</li>
</ul>
