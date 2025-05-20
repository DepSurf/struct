# Struct: <code>remap_data</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct remap_data {
    xen_pfn_t *mfn;
    bool contiguous;
    pgprot_t prot;
    struct mmu_update *mmu_update;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct remap_data {
    xen_pfn_t *mfn;
    bool contiguous;
    pgprot_t prot;
    struct mmu_update *mmu_update;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct remap_data {
    xen_pfn_t *mfn;
    bool contiguous;
    pgprot_t prot;
    struct mmu_update *mmu_update;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct remap_data {
    xen_pfn_t *mfn;
    bool contiguous;
    pgprot_t prot;
    struct mmu_update *mmu_update;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct remap_data {
    xen_pfn_t *mfn;
    bool contiguous;
    pgprot_t prot;
    struct mmu_update *mmu_update;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct remap_data {
    xen_pfn_t *pfn;
    bool contiguous;
    bool no_translate;
    pgprot_t prot;
    struct mmu_update *mmu_update;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct remap_data {
    xen_pfn_t *pfn;
    bool contiguous;
    bool no_translate;
    pgprot_t prot;
    struct mmu_update *mmu_update;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct remap_data {
    xen_pfn_t *pfn;
    bool contiguous;
    bool no_translate;
    pgprot_t prot;
    struct mmu_update *mmu_update;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct remap_data {
    xen_pfn_t *pfn;
    bool contiguous;
    bool no_translate;
    pgprot_t prot;
    struct mmu_update *mmu_update;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct remap_data {
    xen_pfn_t *pfn;
    bool contiguous;
    bool no_translate;
    pgprot_t prot;
    struct mmu_update *mmu_update;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct remap_data {
    xen_pfn_t *pfn;
    bool contiguous;
    bool no_translate;
    pgprot_t prot;
    struct mmu_update *mmu_update;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct remap_data {
    xen_pfn_t *pfn;
    bool contiguous;
    bool no_translate;
    pgprot_t prot;
    struct mmu_update *mmu_update;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct remap_data {
    xen_pfn_t *pfn;
    bool contiguous;
    bool no_translate;
    pgprot_t prot;
    struct mmu_update *mmu_update;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct remap_data {
    xen_pfn_t *pfn;
    bool contiguous;
    bool no_translate;
    pgprot_t prot;
    struct mmu_update *mmu_update;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct remap_data {
    xen_pfn_t *pfn;
    bool contiguous;
    bool no_translate;
    pgprot_t prot;
    struct mmu_update *mmu_update;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct remap_data {
    xen_pfn_t *pfn;
    bool contiguous;
    bool no_translate;
    pgprot_t prot;
    struct mmu_update *mmu_update;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct remap_data {
    xen_pfn_t *pfn;
    bool contiguous;
    bool no_translate;
    pgprot_t prot;
    struct mmu_update *mmu_update;
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
struct remap_data {
    xen_pfn_t *fgfn;
    int nr_fgfn;
    pgprot_t prot;
    domid_t domid;
    struct vm_area_struct *vma;
    int index;
    struct page **pages;
    struct xen_remap_gfn_info *info;
    int *err_ptr;
    int mapped;
    int h_errs[1];
    xen_ulong_t h_idxs[1];
    xen_pfn_t h_gpfns[1];
    int h_iter;
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct remap_data {
    xen_pfn_t *pfn;
    bool contiguous;
    bool no_translate;
    pgprot_t prot;
    struct mmu_update *mmu_update;
};
```
</details>
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct remap_data {
    xen_pfn_t *pfn;
    bool contiguous;
    bool no_translate;
    pgprot_t prot;
    struct mmu_update *mmu_update;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct remap_data {
    xen_pfn_t *pfn;
    bool contiguous;
    bool no_translate;
    pgprot_t prot;
    struct mmu_update *mmu_update;
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
<code>xen_pfn_t *pfn</code>
</li>
<li>
<b>Field added. </b>
<code>bool no_translate</code>
</li>
<li>
<b>Field removed. </b>
<code>xen_pfn_t *mfn</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>arm64</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>xen_pfn_t *fgfn</code>
</li>
<li>
<b>Field added. </b>
<code>int nr_fgfn</code>
</li>
<li>
<b>Field added. </b>
<code>domid_t domid</code>
</li>
<li>
<b>Field added. </b>
<code>struct vm_area_struct *vma</code>
</li>
<li>
<b>Field added. </b>
<code>int index</code>
</li>
<li>
<b>Field added. </b>
<code>struct page **pages</code>
</li>
<li>
<b>Field added. </b>
<code>struct xen_remap_gfn_info *info</code>
</li>
<li>
<b>Field added. </b>
<code>int *err_ptr</code>
</li>
<li>
<b>Field added. </b>
<code>int mapped</code>
</li>
<li>
<b>Field added. </b>
<code>int h_errs[1]</code>
</li>
<li>
<b>Field added. </b>
<code>xen_ulong_t h_idxs[1]</code>
</li>
<li>
<b>Field added. </b>
<code>xen_pfn_t h_gpfns[1]</code>
</li>
<li>
<b>Field added. </b>
<code>int h_iter</code>
</li>
<li>
<b>Field removed. </b>
<code>xen_pfn_t *pfn</code>
</li>
<li>
<b>Field removed. </b>
<code>bool contiguous</code>
</li>
<li>
<b>Field removed. </b>
<code>bool no_translate</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mmu_update *mmu_update</code>
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
