# Struct: <code>iommu_fwspec</code>

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
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct iommu_fwspec {
    const struct iommu_ops *ops;
    struct fwnode_handle *iommu_fwnode;
    void *iommu_priv;
    unsigned int num_ids;
    u32 ids[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct iommu_fwspec {
    const struct iommu_ops *ops;
    struct fwnode_handle *iommu_fwnode;
    void *iommu_priv;
    unsigned int num_ids;
    u32 ids[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct iommu_fwspec {
    const struct iommu_ops *ops;
    struct fwnode_handle *iommu_fwnode;
    void *iommu_priv;
    unsigned int num_ids;
    u32 ids[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct iommu_fwspec {
    const struct iommu_ops *ops;
    struct fwnode_handle *iommu_fwnode;
    void *iommu_priv;
    unsigned int num_ids;
    u32 ids[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct iommu_fwspec {
    const struct iommu_ops *ops;
    struct fwnode_handle *iommu_fwnode;
    void *iommu_priv;
    unsigned int num_ids;
    u32 ids[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct iommu_fwspec {
    const struct iommu_ops *ops;
    struct fwnode_handle *iommu_fwnode;
    void *iommu_priv;
    u32 flags;
    unsigned int num_ids;
    u32 ids[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct iommu_fwspec {
    const struct iommu_ops *ops;
    struct fwnode_handle *iommu_fwnode;
    void *iommu_priv;
    u32 flags;
    unsigned int num_ids;
    u32 ids[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct iommu_fwspec {
    const struct iommu_ops *ops;
    struct fwnode_handle *iommu_fwnode;
    u32 flags;
    u32 num_pasid_bits;
    unsigned int num_ids;
    u32 ids[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct iommu_fwspec {
    const struct iommu_ops *ops;
    struct fwnode_handle *iommu_fwnode;
    u32 flags;
    u32 num_pasid_bits;
    unsigned int num_ids;
    u32 ids[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct iommu_fwspec {
    const struct iommu_ops *ops;
    struct fwnode_handle *iommu_fwnode;
    u32 flags;
    unsigned int num_ids;
    u32 ids[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct iommu_fwspec {
    const struct iommu_ops *ops;
    struct fwnode_handle *iommu_fwnode;
    u32 flags;
    unsigned int num_ids;
    u32 ids[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct iommu_fwspec {
    const struct iommu_ops *ops;
    struct fwnode_handle *iommu_fwnode;
    u32 flags;
    unsigned int num_ids;
    u32 ids[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct iommu_fwspec {
    const struct iommu_ops *ops;
    struct fwnode_handle *iommu_fwnode;
    u32 flags;
    unsigned int num_ids;
    u32 ids[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct iommu_fwspec {
    const struct iommu_ops *ops;
    struct fwnode_handle *iommu_fwnode;
    u32 flags;
    unsigned int num_ids;
    u32 ids[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct iommu_fwspec {
    const struct iommu_ops *ops;
    struct fwnode_handle *iommu_fwnode;
    u32 flags;
    unsigned int num_ids;
    u32 ids[0];
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
struct iommu_fwspec {
    const struct iommu_ops *ops;
    struct fwnode_handle *iommu_fwnode;
    void *iommu_priv;
    u32 flags;
    unsigned int num_ids;
    u32 ids[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct iommu_fwspec {
    const struct iommu_ops *ops;
    struct fwnode_handle *iommu_fwnode;
    void *iommu_priv;
    u32 flags;
    unsigned int num_ids;
    u32 ids[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct iommu_fwspec {
    const struct iommu_ops *ops;
    struct fwnode_handle *iommu_fwnode;
    void *iommu_priv;
    u32 flags;
    unsigned int num_ids;
    u32 ids[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct iommu_fwspec {
};
```
</details>
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct iommu_fwspec {
    const struct iommu_ops *ops;
    struct fwnode_handle *iommu_fwnode;
    void *iommu_priv;
    u32 flags;
    unsigned int num_ids;
    u32 ids[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct iommu_fwspec {
    const struct iommu_ops *ops;
    struct fwnode_handle *iommu_fwnode;
    void *iommu_priv;
    u32 flags;
    unsigned int num_ids;
    u32 ids[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct iommu_fwspec {
    const struct iommu_ops *ops;
    struct fwnode_handle *iommu_fwnode;
    void *iommu_priv;
    u32 flags;
    unsigned int num_ids;
    u32 ids[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct iommu_fwspec {
    const struct iommu_ops *ops;
    struct fwnode_handle *iommu_fwnode;
    void *iommu_priv;
    u32 flags;
    unsigned int num_ids;
    u32 ids[1];
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
<code>u32 flags</code>
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
<code>u32 num_pasid_bits</code>
</li>
<li>
<b>Field removed. </b>
<code>void *iommu_priv</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 ids[1]</code> ➡️ <code>u32 ids[0]</code>
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
<code>u32 num_pasid_bits</code>
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
No changes between <code>5.19</code> and <code>6.2</code> ✅
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
<li>
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>armhf</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>const struct iommu_ops *ops</code>
</li>
<li>
<b>Field removed. </b>
<code>struct fwnode_handle *iommu_fwnode</code>
</li>
<li>
<b>Field removed. </b>
<code>void *iommu_priv</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 flags</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int num_ids</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 ids[1]</code>
</li>
</ul>
</details>
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
