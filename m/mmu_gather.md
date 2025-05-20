# Struct: <code>mmu_gather</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct mmu_gather {
    struct mm_struct *mm;
    long unsigned int start;
    long unsigned int end;
    unsigned int fullmm;
    unsigned int need_flush_all;
    struct mmu_gather_batch *active;
    struct mmu_gather_batch local;
    struct page * __pages[8];
    unsigned int batch_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct mmu_gather {
    struct mm_struct *mm;
    long unsigned int start;
    long unsigned int end;
    unsigned int fullmm;
    unsigned int need_flush_all;
    struct mmu_gather_batch *active;
    struct mmu_gather_batch local;
    struct page * __pages[8];
    unsigned int batch_count;
    long unsigned int addr;
    int page_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct mmu_gather {
    struct mm_struct *mm;
    long unsigned int start;
    long unsigned int end;
    unsigned int fullmm;
    unsigned int need_flush_all;
    struct mmu_gather_batch *active;
    struct mmu_gather_batch local;
    struct page * __pages[8];
    unsigned int batch_count;
    int page_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct mmu_gather {
    struct mm_struct *mm;
    long unsigned int start;
    long unsigned int end;
    unsigned int fullmm;
    unsigned int need_flush_all;
    struct mmu_gather_batch *active;
    struct mmu_gather_batch local;
    struct page * __pages[8];
    unsigned int batch_count;
    int page_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct mmu_gather {
    struct mm_struct *mm;
    struct mmu_table_batch *batch;
    long unsigned int start;
    long unsigned int end;
    unsigned int fullmm;
    unsigned int need_flush_all;
    struct mmu_gather_batch *active;
    struct mmu_gather_batch local;
    struct page * __pages[8];
    unsigned int batch_count;
    int page_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct mmu_gather {
    struct mm_struct *mm;
    struct mmu_table_batch *batch;
    long unsigned int start;
    long unsigned int end;
    unsigned int fullmm;
    unsigned int need_flush_all;
    struct mmu_gather_batch *active;
    struct mmu_gather_batch local;
    struct page * __pages[8];
    unsigned int batch_count;
    int page_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct mmu_gather {
    struct mm_struct *mm;
    struct mmu_table_batch *batch;
    long unsigned int start;
    long unsigned int end;
    unsigned int fullmm;
    unsigned int need_flush_all;
    unsigned int freed_tables;
    unsigned int cleared_ptes;
    unsigned int cleared_pmds;
    unsigned int cleared_puds;
    unsigned int cleared_p4ds;
    struct mmu_gather_batch *active;
    struct mmu_gather_batch local;
    struct page * __pages[8];
    unsigned int batch_count;
    int page_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct mmu_gather {
    struct mm_struct *mm;
    struct mmu_table_batch *batch;
    long unsigned int start;
    long unsigned int end;
    unsigned int fullmm;
    unsigned int need_flush_all;
    unsigned int freed_tables;
    unsigned int cleared_ptes;
    unsigned int cleared_pmds;
    unsigned int cleared_puds;
    unsigned int cleared_p4ds;
    unsigned int vma_exec;
    unsigned int vma_huge;
    unsigned int batch_count;
    struct mmu_gather_batch *active;
    struct mmu_gather_batch local;
    struct page * __pages[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct mmu_gather {
    struct mm_struct *mm;
    struct mmu_table_batch *batch;
    long unsigned int start;
    long unsigned int end;
    unsigned int fullmm;
    unsigned int need_flush_all;
    unsigned int freed_tables;
    unsigned int cleared_ptes;
    unsigned int cleared_pmds;
    unsigned int cleared_puds;
    unsigned int cleared_p4ds;
    unsigned int vma_exec;
    unsigned int vma_huge;
    unsigned int batch_count;
    struct mmu_gather_batch *active;
    struct mmu_gather_batch local;
    struct page * __pages[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct mmu_gather {
    struct mm_struct *mm;
    struct mmu_table_batch *batch;
    long unsigned int start;
    long unsigned int end;
    unsigned int fullmm;
    unsigned int need_flush_all;
    unsigned int freed_tables;
    unsigned int cleared_ptes;
    unsigned int cleared_pmds;
    unsigned int cleared_puds;
    unsigned int cleared_p4ds;
    unsigned int vma_exec;
    unsigned int vma_huge;
    unsigned int batch_count;
    struct mmu_gather_batch *active;
    struct mmu_gather_batch local;
    struct page * __pages[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mmu_gather {
    struct mm_struct *mm;
    struct mmu_table_batch *batch;
    long unsigned int start;
    long unsigned int end;
    unsigned int fullmm;
    unsigned int need_flush_all;
    unsigned int freed_tables;
    unsigned int cleared_ptes;
    unsigned int cleared_pmds;
    unsigned int cleared_puds;
    unsigned int cleared_p4ds;
    unsigned int vma_exec;
    unsigned int vma_huge;
    unsigned int batch_count;
    struct mmu_gather_batch *active;
    struct mmu_gather_batch local;
    struct page * __pages[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mmu_gather {
    struct mm_struct *mm;
    struct mmu_table_batch *batch;
    long unsigned int start;
    long unsigned int end;
    unsigned int fullmm;
    unsigned int need_flush_all;
    unsigned int freed_tables;
    unsigned int cleared_ptes;
    unsigned int cleared_pmds;
    unsigned int cleared_puds;
    unsigned int cleared_p4ds;
    unsigned int vma_exec;
    unsigned int vma_huge;
    unsigned int batch_count;
    struct mmu_gather_batch *active;
    struct mmu_gather_batch local;
    struct page * __pages[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mmu_gather {
    struct mm_struct *mm;
    struct mmu_table_batch *batch;
    long unsigned int start;
    long unsigned int end;
    unsigned int fullmm;
    unsigned int need_flush_all;
    unsigned int freed_tables;
    unsigned int cleared_ptes;
    unsigned int cleared_pmds;
    unsigned int cleared_puds;
    unsigned int cleared_p4ds;
    unsigned int vma_exec;
    unsigned int vma_huge;
    unsigned int batch_count;
    struct mmu_gather_batch *active;
    struct mmu_gather_batch local;
    struct page * __pages[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mmu_gather {
    struct mm_struct *mm;
    struct mmu_table_batch *batch;
    long unsigned int start;
    long unsigned int end;
    unsigned int fullmm;
    unsigned int need_flush_all;
    unsigned int freed_tables;
    unsigned int cleared_ptes;
    unsigned int cleared_pmds;
    unsigned int cleared_puds;
    unsigned int cleared_p4ds;
    unsigned int vma_exec;
    unsigned int vma_huge;
    unsigned int vma_pfn;
    unsigned int batch_count;
    struct mmu_gather_batch *active;
    struct mmu_gather_batch local;
    struct page * __pages[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mmu_gather {
    struct mm_struct *mm;
    struct mmu_table_batch *batch;
    long unsigned int start;
    long unsigned int end;
    unsigned int fullmm;
    unsigned int need_flush_all;
    unsigned int freed_tables;
    unsigned int delayed_rmap;
    unsigned int cleared_ptes;
    unsigned int cleared_pmds;
    unsigned int cleared_puds;
    unsigned int cleared_p4ds;
    unsigned int vma_exec;
    unsigned int vma_huge;
    unsigned int vma_pfn;
    unsigned int batch_count;
    struct mmu_gather_batch *active;
    struct mmu_gather_batch local;
    struct page * __pages[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mmu_gather {
    struct mm_struct *mm;
    struct mmu_table_batch *batch;
    long unsigned int start;
    long unsigned int end;
    unsigned int fullmm;
    unsigned int need_flush_all;
    unsigned int freed_tables;
    unsigned int delayed_rmap;
    unsigned int cleared_ptes;
    unsigned int cleared_pmds;
    unsigned int cleared_puds;
    unsigned int cleared_p4ds;
    unsigned int vma_exec;
    unsigned int vma_huge;
    unsigned int vma_pfn;
    unsigned int batch_count;
    struct mmu_gather_batch *active;
    struct mmu_gather_batch local;
    struct page * __pages[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mmu_gather {
    struct mm_struct *mm;
    struct mmu_table_batch *batch;
    long unsigned int start;
    long unsigned int end;
    unsigned int fullmm;
    unsigned int need_flush_all;
    unsigned int freed_tables;
    unsigned int delayed_rmap;
    unsigned int cleared_ptes;
    unsigned int cleared_pmds;
    unsigned int cleared_puds;
    unsigned int cleared_p4ds;
    unsigned int vma_exec;
    unsigned int vma_huge;
    unsigned int vma_pfn;
    unsigned int batch_count;
    struct mmu_gather_batch *active;
    struct mmu_gather_batch local;
    struct page * __pages[8];
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
struct mmu_gather {
    struct mm_struct *mm;
    struct mmu_table_batch *batch;
    long unsigned int start;
    long unsigned int end;
    unsigned int fullmm;
    unsigned int need_flush_all;
    unsigned int freed_tables;
    unsigned int cleared_ptes;
    unsigned int cleared_pmds;
    unsigned int cleared_puds;
    unsigned int cleared_p4ds;
    unsigned int vma_exec;
    unsigned int vma_huge;
    unsigned int batch_count;
    struct mmu_gather_batch *active;
    struct mmu_gather_batch local;
    struct page * __pages[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mmu_gather {
    struct mm_struct *mm;
    long unsigned int start;
    long unsigned int end;
    unsigned int fullmm;
    unsigned int need_flush_all;
    unsigned int freed_tables;
    unsigned int cleared_ptes;
    unsigned int cleared_pmds;
    unsigned int cleared_puds;
    unsigned int cleared_p4ds;
    unsigned int vma_exec;
    unsigned int vma_huge;
    unsigned int batch_count;
    struct mmu_gather_batch *active;
    struct mmu_gather_batch local;
    struct page * __pages[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct mmu_gather {
    struct mm_struct *mm;
    struct mmu_table_batch *batch;
    long unsigned int start;
    long unsigned int end;
    unsigned int fullmm;
    unsigned int need_flush_all;
    unsigned int freed_tables;
    unsigned int cleared_ptes;
    unsigned int cleared_pmds;
    unsigned int cleared_puds;
    unsigned int cleared_p4ds;
    unsigned int vma_exec;
    unsigned int vma_huge;
    unsigned int batch_count;
    struct mmu_gather_batch *active;
    struct mmu_gather_batch local;
    struct page * __pages[8];
    unsigned int page_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct mmu_gather {
    struct mm_struct *mm;
    long unsigned int start;
    long unsigned int end;
    unsigned int fullmm;
    unsigned int need_flush_all;
    unsigned int freed_tables;
    unsigned int cleared_ptes;
    unsigned int cleared_pmds;
    unsigned int cleared_puds;
    unsigned int cleared_p4ds;
    unsigned int vma_exec;
    unsigned int vma_huge;
    unsigned int batch_count;
    struct mmu_gather_batch *active;
    struct mmu_gather_batch local;
    struct page * __pages[8];
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
struct mmu_gather {
    struct mm_struct *mm;
    struct mmu_table_batch *batch;
    long unsigned int start;
    long unsigned int end;
    unsigned int fullmm;
    unsigned int need_flush_all;
    unsigned int freed_tables;
    unsigned int cleared_ptes;
    unsigned int cleared_pmds;
    unsigned int cleared_puds;
    unsigned int cleared_p4ds;
    unsigned int vma_exec;
    unsigned int vma_huge;
    unsigned int batch_count;
    struct mmu_gather_batch *active;
    struct mmu_gather_batch local;
    struct page * __pages[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct mmu_gather {
    struct mm_struct *mm;
    struct mmu_table_batch *batch;
    long unsigned int start;
    long unsigned int end;
    unsigned int fullmm;
    unsigned int need_flush_all;
    unsigned int freed_tables;
    unsigned int cleared_ptes;
    unsigned int cleared_pmds;
    unsigned int cleared_puds;
    unsigned int cleared_p4ds;
    unsigned int vma_exec;
    unsigned int vma_huge;
    unsigned int batch_count;
    struct mmu_gather_batch *active;
    struct mmu_gather_batch local;
    struct page * __pages[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct mmu_gather {
    struct mm_struct *mm;
    struct mmu_table_batch *batch;
    long unsigned int start;
    long unsigned int end;
    unsigned int fullmm;
    unsigned int need_flush_all;
    unsigned int freed_tables;
    unsigned int cleared_ptes;
    unsigned int cleared_pmds;
    unsigned int cleared_puds;
    unsigned int cleared_p4ds;
    unsigned int vma_exec;
    unsigned int vma_huge;
    unsigned int batch_count;
    struct mmu_gather_batch *active;
    struct mmu_gather_batch local;
    struct page * __pages[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct mmu_gather {
    struct mm_struct *mm;
    struct mmu_table_batch *batch;
    long unsigned int start;
    long unsigned int end;
    unsigned int fullmm;
    unsigned int need_flush_all;
    unsigned int freed_tables;
    unsigned int cleared_ptes;
    unsigned int cleared_pmds;
    unsigned int cleared_puds;
    unsigned int cleared_p4ds;
    unsigned int vma_exec;
    unsigned int vma_huge;
    unsigned int batch_count;
    struct mmu_gather_batch *active;
    struct mmu_gather_batch local;
    struct page * __pages[8];
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
<code>long unsigned int addr</code>
</li>
<li>
<b>Field added. </b>
<code>int page_size</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>long unsigned int addr</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct mmu_table_batch *batch</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int freed_tables</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int cleared_ptes</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int cleared_pmds</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int cleared_puds</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int cleared_p4ds</code>
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
<code>unsigned int vma_exec</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int vma_huge</code>
</li>
<li>
<b>Field removed. </b>
<code>int page_size</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int vma_pfn</code>
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
<code>unsigned int delayed_rmap</code>
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
<li>
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct mmu_table_batch *batch</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int page_size</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct mmu_table_batch *batch</code>
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
