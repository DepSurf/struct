# Struct: <code>folio</code>

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
In <code>5.8</code>: Absent ⚠️
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct folio {
    long unsigned int flags;
    struct list_head lru;
    void *__filler;
    unsigned int mlock_count;
    struct address_space *mapping;
    long unsigned int index;
    void *private;
    atomic_t _mapcount;
    atomic_t _refcount;
    long unsigned int memcg_data;
    struct page page;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct folio {
    long unsigned int flags;
    struct list_head lru;
    void *__filler;
    unsigned int mlock_count;
    struct address_space *mapping;
    long unsigned int index;
    void *private;
    atomic_t _mapcount;
    atomic_t _refcount;
    long unsigned int memcg_data;
    struct page page;
    long unsigned int _flags_1;
    long unsigned int _head_1;
    unsigned char _folio_dtor;
    unsigned char _folio_order;
    atomic_t _compound_mapcount;
    atomic_t _subpages_mapcount;
    atomic_t _pincount;
    unsigned int _folio_nr_pages;
    struct page __page_1;
    long unsigned int _flags_2;
    long unsigned int _head_2;
    void *_hugetlb_subpool;
    void *_hugetlb_cgroup;
    void *_hugetlb_cgroup_rsvd;
    void *_hugetlb_hwpoison;
    struct page __page_2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct folio {
    long unsigned int flags;
    struct list_head lru;
    void *__filler;
    unsigned int mlock_count;
    struct address_space *mapping;
    long unsigned int index;
    void *private;
    atomic_t _mapcount;
    atomic_t _refcount;
    long unsigned int memcg_data;
    struct page page;
    long unsigned int _flags_1;
    long unsigned int _head_1;
    unsigned char _folio_dtor;
    unsigned char _folio_order;
    atomic_t _entire_mapcount;
    atomic_t _nr_pages_mapped;
    atomic_t _pincount;
    unsigned int _folio_nr_pages;
    struct page __page_1;
    long unsigned int _flags_2;
    long unsigned int _head_2;
    void *_hugetlb_subpool;
    void *_hugetlb_cgroup;
    void *_hugetlb_cgroup_rsvd;
    void *_hugetlb_hwpoison;
    long unsigned int _flags_2a;
    long unsigned int _head_2a;
    struct list_head _deferred_list;
    struct page __page_2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct folio {
    long unsigned int flags;
    struct list_head lru;
    void *__filler;
    unsigned int mlock_count;
    struct address_space *mapping;
    long unsigned int index;
    void *private;
    swp_entry_t swap;
    atomic_t _mapcount;
    atomic_t _refcount;
    long unsigned int memcg_data;
    struct page page;
    long unsigned int _flags_1;
    long unsigned int _head_1;
    long unsigned int _folio_avail;
    atomic_t _entire_mapcount;
    atomic_t _nr_pages_mapped;
    atomic_t _pincount;
    unsigned int _folio_nr_pages;
    struct page __page_1;
    long unsigned int _flags_2;
    long unsigned int _head_2;
    void *_hugetlb_subpool;
    void *_hugetlb_cgroup;
    void *_hugetlb_cgroup_rsvd;
    void *_hugetlb_hwpoison;
    long unsigned int _flags_2a;
    long unsigned int _head_2a;
    struct list_head _deferred_list;
    struct page __page_2;
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int _flags_1</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int _head_1</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned char _folio_dtor</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned char _folio_order</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t _compound_mapcount</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t _subpages_mapcount</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t _pincount</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int _folio_nr_pages</code>
</li>
<li>
<b>Field added. </b>
<code>struct page __page_1</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int _flags_2</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int _head_2</code>
</li>
<li>
<b>Field added. </b>
<code>void *_hugetlb_subpool</code>
</li>
<li>
<b>Field added. </b>
<code>void *_hugetlb_cgroup</code>
</li>
<li>
<b>Field added. </b>
<code>void *_hugetlb_cgroup_rsvd</code>
</li>
<li>
<b>Field added. </b>
<code>void *_hugetlb_hwpoison</code>
</li>
<li>
<b>Field added. </b>
<code>struct page __page_2</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>atomic_t _entire_mapcount</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t _nr_pages_mapped</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int _flags_2a</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int _head_2a</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head _deferred_list</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t _compound_mapcount</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t _subpages_mapcount</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>swp_entry_t swap</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int _folio_avail</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned char _folio_dtor</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned char _folio_order</code>
</li>
</ul>
</details>
</li>
</ul>
