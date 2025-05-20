# Struct: <code>hmm_range</code>

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
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct hmm_range {
    struct list_head list;
    long unsigned int start;
    long unsigned int end;
    hmm_pfn_t *pfns;
    bool valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct hmm_range {
    struct vm_area_struct *vma;
    struct list_head list;
    long unsigned int start;
    long unsigned int end;
    uint64_t *pfns;
    const uint64_t *flags;
    const uint64_t *values;
    uint8_t pfn_shift;
    bool valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct hmm_range {
    struct vm_area_struct *vma;
    struct list_head list;
    long unsigned int start;
    long unsigned int end;
    uint64_t *pfns;
    const uint64_t *flags;
    const uint64_t *values;
    uint8_t pfn_shift;
    bool valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct hmm_range {
    struct hmm *hmm;
    struct vm_area_struct *vma;
    struct list_head list;
    long unsigned int start;
    long unsigned int end;
    uint64_t *pfns;
    const uint64_t *flags;
    const uint64_t *values;
    uint64_t default_flags;
    uint64_t pfn_flags_mask;
    uint8_t page_shift;
    uint8_t pfn_shift;
    bool valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct hmm_range {
    struct hmm *hmm;
    struct list_head list;
    long unsigned int start;
    long unsigned int end;
    uint64_t *pfns;
    const uint64_t *flags;
    const uint64_t *values;
    uint64_t default_flags;
    uint64_t pfn_flags_mask;
    uint8_t pfn_shift;
    bool valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct hmm_range {
    struct mmu_interval_notifier *notifier;
    long unsigned int notifier_seq;
    long unsigned int start;
    long unsigned int end;
    long unsigned int *hmm_pfns;
    long unsigned int default_flags;
    long unsigned int pfn_flags_mask;
    void *dev_private_owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct hmm_range {
    struct mmu_interval_notifier *notifier;
    long unsigned int notifier_seq;
    long unsigned int start;
    long unsigned int end;
    long unsigned int *hmm_pfns;
    long unsigned int default_flags;
    long unsigned int pfn_flags_mask;
    void *dev_private_owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct hmm_range {
    struct mmu_interval_notifier *notifier;
    long unsigned int notifier_seq;
    long unsigned int start;
    long unsigned int end;
    long unsigned int *hmm_pfns;
    long unsigned int default_flags;
    long unsigned int pfn_flags_mask;
    void *dev_private_owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct hmm_range {
    struct mmu_interval_notifier *notifier;
    long unsigned int notifier_seq;
    long unsigned int start;
    long unsigned int end;
    long unsigned int *hmm_pfns;
    long unsigned int default_flags;
    long unsigned int pfn_flags_mask;
    void *dev_private_owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct hmm_range {
    struct mmu_interval_notifier *notifier;
    long unsigned int notifier_seq;
    long unsigned int start;
    long unsigned int end;
    long unsigned int *hmm_pfns;
    long unsigned int default_flags;
    long unsigned int pfn_flags_mask;
    void *dev_private_owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct hmm_range {
    struct mmu_interval_notifier *notifier;
    long unsigned int notifier_seq;
    long unsigned int start;
    long unsigned int end;
    long unsigned int *hmm_pfns;
    long unsigned int default_flags;
    long unsigned int pfn_flags_mask;
    void *dev_private_owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct hmm_range {
    struct mmu_interval_notifier *notifier;
    long unsigned int notifier_seq;
    long unsigned int start;
    long unsigned int end;
    long unsigned int *hmm_pfns;
    long unsigned int default_flags;
    long unsigned int pfn_flags_mask;
    void *dev_private_owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct hmm_range {
    struct mmu_interval_notifier *notifier;
    long unsigned int notifier_seq;
    long unsigned int start;
    long unsigned int end;
    long unsigned int *hmm_pfns;
    long unsigned int default_flags;
    long unsigned int pfn_flags_mask;
    void *dev_private_owner;
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
struct hmm_range {
    struct hmm *hmm;
    struct list_head list;
    long unsigned int start;
    long unsigned int end;
    uint64_t *pfns;
    const uint64_t *flags;
    const uint64_t *values;
    uint64_t default_flags;
    uint64_t pfn_flags_mask;
    uint8_t pfn_shift;
    bool valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct hmm_range {
    struct hmm *hmm;
    struct list_head list;
    long unsigned int start;
    long unsigned int end;
    uint64_t *pfns;
    const uint64_t *flags;
    const uint64_t *values;
    uint64_t default_flags;
    uint64_t pfn_flags_mask;
    uint8_t pfn_shift;
    bool valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct hmm_range {
    struct hmm *hmm;
    struct list_head list;
    long unsigned int start;
    long unsigned int end;
    uint64_t *pfns;
    const uint64_t *flags;
    const uint64_t *values;
    uint64_t default_flags;
    uint64_t pfn_flags_mask;
    uint8_t pfn_shift;
    bool valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct hmm_range {
    struct hmm *hmm;
    struct list_head list;
    long unsigned int start;
    long unsigned int end;
    uint64_t *pfns;
    const uint64_t *flags;
    const uint64_t *values;
    uint64_t default_flags;
    uint64_t pfn_flags_mask;
    uint8_t pfn_shift;
    bool valid;
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
struct hmm_range {
    struct hmm *hmm;
    struct list_head list;
    long unsigned int start;
    long unsigned int end;
    uint64_t *pfns;
    const uint64_t *flags;
    const uint64_t *values;
    uint64_t default_flags;
    uint64_t pfn_flags_mask;
    uint8_t pfn_shift;
    bool valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct hmm_range {
    struct hmm *hmm;
    struct list_head list;
    long unsigned int start;
    long unsigned int end;
    uint64_t *pfns;
    const uint64_t *flags;
    const uint64_t *values;
    uint64_t default_flags;
    uint64_t pfn_flags_mask;
    uint8_t pfn_shift;
    bool valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct hmm_range {
    struct hmm *hmm;
    struct list_head list;
    long unsigned int start;
    long unsigned int end;
    uint64_t *pfns;
    const uint64_t *flags;
    const uint64_t *values;
    uint64_t default_flags;
    uint64_t pfn_flags_mask;
    uint8_t pfn_shift;
    bool valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct hmm_range {
    struct hmm *hmm;
    struct list_head list;
    long unsigned int start;
    long unsigned int end;
    uint64_t *pfns;
    const uint64_t *flags;
    const uint64_t *values;
    uint64_t default_flags;
    uint64_t pfn_flags_mask;
    uint8_t pfn_shift;
    bool valid;
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
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct vm_area_struct *vma</code>
</li>
<li>
<b>Field added. </b>
<code>const uint64_t *flags</code>
</li>
<li>
<b>Field added. </b>
<code>const uint64_t *values</code>
</li>
<li>
<b>Field added. </b>
<code>uint8_t pfn_shift</code>
</li>
<li>
<b>Field type changed. </b>
<code>hmm_pfn_t *pfns</code> ➡️ <code>uint64_t *pfns</code>
</li>
</ul>
</details>
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
<code>struct hmm *hmm</code>
</li>
<li>
<b>Field added. </b>
<code>uint64_t default_flags</code>
</li>
<li>
<b>Field added. </b>
<code>uint64_t pfn_flags_mask</code>
</li>
<li>
<b>Field added. </b>
<code>uint8_t page_shift</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct vm_area_struct *vma</code>
</li>
<li>
<b>Field removed. </b>
<code>uint8_t page_shift</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct mmu_interval_notifier *notifier</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int notifier_seq</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int *hmm_pfns</code>
</li>
<li>
<b>Field added. </b>
<code>void *dev_private_owner</code>
</li>
<li>
<b>Field removed. </b>
<code>struct hmm *hmm</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head list</code>
</li>
<li>
<b>Field removed. </b>
<code>uint64_t *pfns</code>
</li>
<li>
<b>Field removed. </b>
<code>const uint64_t *flags</code>
</li>
<li>
<b>Field removed. </b>
<code>const uint64_t *values</code>
</li>
<li>
<b>Field removed. </b>
<code>uint8_t pfn_shift</code>
</li>
<li>
<b>Field removed. </b>
<code>bool valid</code>
</li>
<li>
<b>Field type changed. </b>
<code>uint64_t default_flags</code> ➡️ <code>long unsigned int default_flags</code>
</li>
<li>
<b>Field type changed. </b>
<code>uint64_t pfn_flags_mask</code> ➡️ <code>long unsigned int pfn_flags_mask</code>
</li>
</ul>
</details>
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
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>armhf</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>riscv64</code> ✅
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
