# Struct: <code>amd_ir_data</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct amd_ir_data {
    struct irq_2_irte irq_2_irte;
    union irte irte_entry;
    struct msi_msg msi_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct amd_ir_data {
    struct irq_2_irte irq_2_irte;
    union irte irte_entry;
    struct msi_msg msi_entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct amd_ir_data {
    u32 cached_ga_tag;
    struct irq_2_irte irq_2_irte;
    struct msi_msg msi_entry;
    void *entry;
    void *ref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct amd_ir_data {
    u32 cached_ga_tag;
    struct irq_2_irte irq_2_irte;
    struct msi_msg msi_entry;
    void *entry;
    void *ref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct amd_ir_data {
    u32 cached_ga_tag;
    struct irq_2_irte irq_2_irte;
    struct msi_msg msi_entry;
    void *entry;
    void *ref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct amd_ir_data {
    u32 cached_ga_tag;
    struct irq_2_irte irq_2_irte;
    struct msi_msg msi_entry;
    void *entry;
    void *ref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct amd_ir_data {
    u32 cached_ga_tag;
    struct irq_2_irte irq_2_irte;
    struct msi_msg msi_entry;
    void *entry;
    void *ref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct amd_ir_data {
    u32 cached_ga_tag;
    struct irq_2_irte irq_2_irte;
    struct msi_msg msi_entry;
    void *entry;
    void *ref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct amd_ir_data {
    u32 cached_ga_tag;
    struct irq_2_irte irq_2_irte;
    struct msi_msg msi_entry;
    void *entry;
    void *ref;
    struct irq_cfg *cfg;
    int ga_vector;
    int ga_root_ptr;
    int ga_tag;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct amd_ir_data {
    u32 cached_ga_tag;
    struct irq_2_irte irq_2_irte;
    struct msi_msg msi_entry;
    void *entry;
    void *ref;
    struct irq_cfg *cfg;
    int ga_vector;
    int ga_root_ptr;
    int ga_tag;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct amd_ir_data {
    u32 cached_ga_tag;
    struct irq_2_irte irq_2_irte;
    struct msi_msg msi_entry;
    void *entry;
    void *ref;
    struct irq_cfg *cfg;
    int ga_vector;
    int ga_root_ptr;
    int ga_tag;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct amd_ir_data {
    u32 cached_ga_tag;
    struct irq_2_irte irq_2_irte;
    struct msi_msg msi_entry;
    void *entry;
    void *ref;
    struct irq_cfg *cfg;
    int ga_vector;
    int ga_root_ptr;
    int ga_tag;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct amd_ir_data {
    u32 cached_ga_tag;
    struct irq_2_irte irq_2_irte;
    struct msi_msg msi_entry;
    void *entry;
    void *ref;
    struct irq_cfg *cfg;
    int ga_vector;
    int ga_root_ptr;
    int ga_tag;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct amd_ir_data {
    u32 cached_ga_tag;
    struct irq_2_irte irq_2_irte;
    struct msi_msg msi_entry;
    void *entry;
    void *ref;
    struct irq_cfg *cfg;
    int ga_vector;
    int ga_root_ptr;
    int ga_tag;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct amd_ir_data {
    u32 cached_ga_tag;
    struct amd_iommu *iommu;
    struct irq_2_irte irq_2_irte;
    struct msi_msg msi_entry;
    void *entry;
    void *ref;
    struct irq_cfg *cfg;
    int ga_vector;
    int ga_root_ptr;
    int ga_tag;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct amd_ir_data {
    u32 cached_ga_tag;
    struct amd_iommu *iommu;
    struct irq_2_irte irq_2_irte;
    struct msi_msg msi_entry;
    void *entry;
    struct irq_cfg *cfg;
    int ga_vector;
    u64 ga_root_ptr;
    u32 ga_tag;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct amd_ir_data {
    u32 cached_ga_tag;
    struct amd_iommu *iommu;
    struct irq_2_irte irq_2_irte;
    struct msi_msg msi_entry;
    void *entry;
    struct irq_cfg *cfg;
    int ga_vector;
    u64 ga_root_ptr;
    u32 ga_tag;
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
struct amd_ir_data {
    u32 cached_ga_tag;
    struct irq_2_irte irq_2_irte;
    struct msi_msg msi_entry;
    void *entry;
    void *ref;
    struct irq_cfg *cfg;
    int ga_vector;
    int ga_root_ptr;
    int ga_tag;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct amd_ir_data {
    u32 cached_ga_tag;
    struct irq_2_irte irq_2_irte;
    struct msi_msg msi_entry;
    void *entry;
    void *ref;
    struct irq_cfg *cfg;
    int ga_vector;
    int ga_root_ptr;
    int ga_tag;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct amd_ir_data {
    u32 cached_ga_tag;
    struct irq_2_irte irq_2_irte;
    struct msi_msg msi_entry;
    void *entry;
    void *ref;
    struct irq_cfg *cfg;
    int ga_vector;
    int ga_root_ptr;
    int ga_tag;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct amd_ir_data {
    u32 cached_ga_tag;
    struct irq_2_irte irq_2_irte;
    struct msi_msg msi_entry;
    void *entry;
    void *ref;
    struct irq_cfg *cfg;
    int ga_vector;
    int ga_root_ptr;
    int ga_tag;
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
<code>u32 cached_ga_tag</code>
</li>
<li>
<b>Field added. </b>
<code>void *entry</code>
</li>
<li>
<b>Field added. </b>
<code>void *ref</code>
</li>
<li>
<b>Field removed. </b>
<code>union irte irte_entry</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct irq_cfg *cfg</code>
</li>
<li>
<b>Field added. </b>
<code>int ga_vector</code>
</li>
<li>
<b>Field added. </b>
<code>int ga_root_ptr</code>
</li>
<li>
<b>Field added. </b>
<code>int ga_tag</code>
</li>
</ul>
</details>
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
<code>struct amd_iommu *iommu</code>
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
<code>void *ref</code>
</li>
<li>
<b>Field type changed. </b>
<code>int ga_root_ptr</code> ➡️ <code>u64 ga_root_ptr</code>
</li>
<li>
<b>Field type changed. </b>
<code>int ga_tag</code> ➡️ <code>u32 ga_tag</code>
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
