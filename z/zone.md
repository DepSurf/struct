# Struct: <code>zone</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct zone {
    long unsigned int watermark[3];
    long unsigned int nr_reserved_highatomic;
    long int lowmem_reserve[5];
    int node;
    unsigned int inactive_ratio;
    struct pglist_data *zone_pgdat;
    struct per_cpu_pageset *pageset;
    long unsigned int dirty_balance_reserve;
    long unsigned int min_unmapped_pages;
    long unsigned int min_slab_pages;
    long unsigned int zone_start_pfn;
    long unsigned int managed_pages;
    long unsigned int spanned_pages;
    long unsigned int present_pages;
    const char *name;
    long unsigned int nr_isolate_pageblock;
    seqlock_t span_seqlock;
    wait_queue_head_t *wait_table;
    long unsigned int wait_table_hash_nr_entries;
    long unsigned int wait_table_bits;
    struct zone_padding _pad1_;
    struct free_area free_area[11];
    long unsigned int flags;
    spinlock_t lock;
    struct zone_padding _pad2_;
    spinlock_t lru_lock;
    struct lruvec lruvec;
    atomic_long_t inactive_age;
    long unsigned int percpu_drift_mark;
    long unsigned int compact_cached_free_pfn;
    long unsigned int compact_cached_migrate_pfn[2];
    unsigned int compact_considered;
    unsigned int compact_defer_shift;
    int compact_order_failed;
    bool compact_blockskip_flush;
    struct zone_padding _pad3_;
    atomic_long_t vm_stat[39];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct zone {
    long unsigned int watermark[3];
    long unsigned int nr_reserved_highatomic;
    long int lowmem_reserve[5];
    int node;
    struct pglist_data *zone_pgdat;
    struct per_cpu_pageset *pageset;
    long unsigned int zone_start_pfn;
    long unsigned int managed_pages;
    long unsigned int spanned_pages;
    long unsigned int present_pages;
    const char *name;
    long unsigned int nr_isolate_pageblock;
    seqlock_t span_seqlock;
    wait_queue_head_t *wait_table;
    long unsigned int wait_table_hash_nr_entries;
    long unsigned int wait_table_bits;
    struct zone_padding _pad1_;
    struct free_area free_area[11];
    long unsigned int flags;
    spinlock_t lock;
    struct zone_padding _pad2_;
    long unsigned int percpu_drift_mark;
    long unsigned int compact_cached_free_pfn;
    long unsigned int compact_cached_migrate_pfn[2];
    unsigned int compact_considered;
    unsigned int compact_defer_shift;
    int compact_order_failed;
    bool compact_blockskip_flush;
    bool contiguous;
    struct zone_padding _pad3_;
    atomic_long_t vm_stat[21];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct zone {
    long unsigned int watermark[3];
    long unsigned int nr_reserved_highatomic;
    long int lowmem_reserve[5];
    int node;
    struct pglist_data *zone_pgdat;
    struct per_cpu_pageset *pageset;
    long unsigned int zone_start_pfn;
    long unsigned int managed_pages;
    long unsigned int spanned_pages;
    long unsigned int present_pages;
    const char *name;
    long unsigned int nr_isolate_pageblock;
    seqlock_t span_seqlock;
    int initialized;
    struct zone_padding _pad1_;
    struct free_area free_area[11];
    long unsigned int flags;
    spinlock_t lock;
    struct zone_padding _pad2_;
    long unsigned int percpu_drift_mark;
    long unsigned int compact_cached_free_pfn;
    long unsigned int compact_cached_migrate_pfn[2];
    unsigned int compact_considered;
    unsigned int compact_defer_shift;
    int compact_order_failed;
    bool compact_blockskip_flush;
    bool contiguous;
    struct zone_padding _pad3_;
    atomic_long_t vm_stat[21];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct zone {
    long unsigned int watermark[3];
    long unsigned int nr_reserved_highatomic;
    long int lowmem_reserve[5];
    int node;
    struct pglist_data *zone_pgdat;
    struct per_cpu_pageset *pageset;
    long unsigned int zone_start_pfn;
    long unsigned int managed_pages;
    long unsigned int spanned_pages;
    long unsigned int present_pages;
    const char *name;
    long unsigned int nr_isolate_pageblock;
    seqlock_t span_seqlock;
    int initialized;
    struct zone_padding _pad1_;
    struct free_area free_area[11];
    long unsigned int flags;
    spinlock_t lock;
    struct zone_padding _pad2_;
    long unsigned int percpu_drift_mark;
    long unsigned int compact_cached_free_pfn;
    long unsigned int compact_cached_migrate_pfn[2];
    unsigned int compact_considered;
    unsigned int compact_defer_shift;
    int compact_order_failed;
    bool compact_blockskip_flush;
    bool contiguous;
    struct zone_padding _pad3_;
    atomic_long_t vm_stat[19];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct zone {
    long unsigned int watermark[3];
    long unsigned int nr_reserved_highatomic;
    long int lowmem_reserve[5];
    int node;
    struct pglist_data *zone_pgdat;
    struct per_cpu_pageset *pageset;
    long unsigned int zone_start_pfn;
    long unsigned int managed_pages;
    long unsigned int spanned_pages;
    long unsigned int present_pages;
    const char *name;
    long unsigned int nr_isolate_pageblock;
    seqlock_t span_seqlock;
    int initialized;
    struct zone_padding _pad1_;
    struct free_area free_area[11];
    long unsigned int flags;
    spinlock_t lock;
    struct zone_padding _pad2_;
    long unsigned int percpu_drift_mark;
    long unsigned int compact_cached_free_pfn;
    long unsigned int compact_cached_migrate_pfn[2];
    unsigned int compact_considered;
    unsigned int compact_defer_shift;
    int compact_order_failed;
    bool compact_blockskip_flush;
    bool contiguous;
    struct zone_padding _pad3_;
    atomic_long_t vm_stat[13];
    atomic_long_t vm_numa_stat[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct zone {
    long unsigned int watermark[3];
    long unsigned int nr_reserved_highatomic;
    long int lowmem_reserve[5];
    int node;
    struct pglist_data *zone_pgdat;
    struct per_cpu_pageset *pageset;
    long unsigned int zone_start_pfn;
    long unsigned int managed_pages;
    long unsigned int spanned_pages;
    long unsigned int present_pages;
    const char *name;
    long unsigned int nr_isolate_pageblock;
    seqlock_t span_seqlock;
    int initialized;
    struct zone_padding _pad1_;
    struct free_area free_area[11];
    long unsigned int flags;
    spinlock_t lock;
    struct zone_padding _pad2_;
    long unsigned int percpu_drift_mark;
    long unsigned int compact_cached_free_pfn;
    long unsigned int compact_cached_migrate_pfn[2];
    unsigned int compact_considered;
    unsigned int compact_defer_shift;
    int compact_order_failed;
    bool compact_blockskip_flush;
    bool contiguous;
    struct zone_padding _pad3_;
    atomic_long_t vm_stat[13];
    atomic_long_t vm_numa_stat[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct zone {
    long unsigned int _watermark[3];
    long unsigned int watermark_boost;
    long unsigned int nr_reserved_highatomic;
    long int lowmem_reserve[5];
    int node;
    struct pglist_data *zone_pgdat;
    struct per_cpu_pageset *pageset;
    long unsigned int zone_start_pfn;
    atomic_long_t managed_pages;
    long unsigned int spanned_pages;
    long unsigned int present_pages;
    const char *name;
    long unsigned int nr_isolate_pageblock;
    seqlock_t span_seqlock;
    int initialized;
    struct zone_padding _pad1_;
    struct free_area free_area[11];
    long unsigned int flags;
    spinlock_t lock;
    struct zone_padding _pad2_;
    long unsigned int percpu_drift_mark;
    long unsigned int compact_cached_free_pfn;
    long unsigned int compact_cached_migrate_pfn[2];
    unsigned int compact_considered;
    unsigned int compact_defer_shift;
    int compact_order_failed;
    bool compact_blockskip_flush;
    bool contiguous;
    struct zone_padding _pad3_;
    atomic_long_t vm_stat[13];
    atomic_long_t vm_numa_stat[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct zone {
    long unsigned int _watermark[3];
    long unsigned int watermark_boost;
    long unsigned int nr_reserved_highatomic;
    long int lowmem_reserve[5];
    int node;
    struct pglist_data *zone_pgdat;
    struct per_cpu_pageset *pageset;
    long unsigned int zone_start_pfn;
    atomic_long_t managed_pages;
    long unsigned int spanned_pages;
    long unsigned int present_pages;
    const char *name;
    long unsigned int nr_isolate_pageblock;
    seqlock_t span_seqlock;
    int initialized;
    struct zone_padding _pad1_;
    struct free_area free_area[11];
    long unsigned int flags;
    spinlock_t lock;
    struct zone_padding _pad2_;
    long unsigned int percpu_drift_mark;
    long unsigned int compact_cached_free_pfn;
    long unsigned int compact_cached_migrate_pfn[2];
    long unsigned int compact_init_migrate_pfn;
    long unsigned int compact_init_free_pfn;
    unsigned int compact_considered;
    unsigned int compact_defer_shift;
    int compact_order_failed;
    bool compact_blockskip_flush;
    bool contiguous;
    struct zone_padding _pad3_;
    atomic_long_t vm_stat[13];
    atomic_long_t vm_numa_stat[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct zone {
    long unsigned int _watermark[3];
    long unsigned int watermark_boost;
    long unsigned int nr_reserved_highatomic;
    long int lowmem_reserve[5];
    int node;
    struct pglist_data *zone_pgdat;
    struct per_cpu_pageset *pageset;
    long unsigned int zone_start_pfn;
    atomic_long_t managed_pages;
    long unsigned int spanned_pages;
    long unsigned int present_pages;
    const char *name;
    long unsigned int nr_isolate_pageblock;
    seqlock_t span_seqlock;
    int initialized;
    struct zone_padding _pad1_;
    struct free_area free_area[11];
    long unsigned int flags;
    spinlock_t lock;
    struct zone_padding _pad2_;
    long unsigned int percpu_drift_mark;
    long unsigned int compact_cached_free_pfn;
    long unsigned int compact_cached_migrate_pfn[2];
    long unsigned int compact_init_migrate_pfn;
    long unsigned int compact_init_free_pfn;
    unsigned int compact_considered;
    unsigned int compact_defer_shift;
    int compact_order_failed;
    bool compact_blockskip_flush;
    bool contiguous;
    struct zone_padding _pad3_;
    atomic_long_t vm_stat[13];
    atomic_long_t vm_numa_stat[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct zone {
    long unsigned int _watermark[3];
    long unsigned int watermark_boost;
    long unsigned int nr_reserved_highatomic;
    long int lowmem_reserve[5];
    int node;
    struct pglist_data *zone_pgdat;
    struct per_cpu_pageset *pageset;
    long unsigned int zone_start_pfn;
    atomic_long_t managed_pages;
    long unsigned int spanned_pages;
    long unsigned int present_pages;
    const char *name;
    long unsigned int nr_isolate_pageblock;
    seqlock_t span_seqlock;
    int initialized;
    struct zone_padding _pad1_;
    struct free_area free_area[11];
    long unsigned int flags;
    spinlock_t lock;
    struct zone_padding _pad2_;
    long unsigned int percpu_drift_mark;
    long unsigned int compact_cached_free_pfn;
    long unsigned int compact_cached_migrate_pfn[2];
    long unsigned int compact_init_migrate_pfn;
    long unsigned int compact_init_free_pfn;
    unsigned int compact_considered;
    unsigned int compact_defer_shift;
    int compact_order_failed;
    bool compact_blockskip_flush;
    bool contiguous;
    struct zone_padding _pad3_;
    atomic_long_t vm_stat[13];
    atomic_long_t vm_numa_stat[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct zone {
    long unsigned int _watermark[3];
    long unsigned int watermark_boost;
    long unsigned int nr_reserved_highatomic;
    long int lowmem_reserve[5];
    int node;
    struct pglist_data *zone_pgdat;
    struct per_cpu_pageset *pageset;
    int pageset_high;
    int pageset_batch;
    long unsigned int zone_start_pfn;
    atomic_long_t managed_pages;
    long unsigned int spanned_pages;
    long unsigned int present_pages;
    const char *name;
    long unsigned int nr_isolate_pageblock;
    seqlock_t span_seqlock;
    int initialized;
    struct zone_padding _pad1_;
    struct free_area free_area[11];
    long unsigned int flags;
    spinlock_t lock;
    struct zone_padding _pad2_;
    long unsigned int percpu_drift_mark;
    long unsigned int compact_cached_free_pfn;
    long unsigned int compact_cached_migrate_pfn[2];
    long unsigned int compact_init_migrate_pfn;
    long unsigned int compact_init_free_pfn;
    unsigned int compact_considered;
    unsigned int compact_defer_shift;
    int compact_order_failed;
    bool compact_blockskip_flush;
    bool contiguous;
    struct zone_padding _pad3_;
    atomic_long_t vm_stat[11];
    atomic_long_t vm_numa_stat[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct zone {
    long unsigned int _watermark[3];
    long unsigned int watermark_boost;
    long unsigned int nr_reserved_highatomic;
    long int lowmem_reserve[5];
    int node;
    struct pglist_data *zone_pgdat;
    struct per_cpu_pageset *pageset;
    int pageset_high;
    int pageset_batch;
    long unsigned int zone_start_pfn;
    atomic_long_t managed_pages;
    long unsigned int spanned_pages;
    long unsigned int present_pages;
    const char *name;
    long unsigned int nr_isolate_pageblock;
    seqlock_t span_seqlock;
    int initialized;
    struct zone_padding _pad1_;
    struct free_area free_area[11];
    long unsigned int flags;
    spinlock_t lock;
    struct zone_padding _pad2_;
    long unsigned int percpu_drift_mark;
    long unsigned int compact_cached_free_pfn;
    long unsigned int compact_cached_migrate_pfn[2];
    long unsigned int compact_init_migrate_pfn;
    long unsigned int compact_init_free_pfn;
    unsigned int compact_considered;
    unsigned int compact_defer_shift;
    int compact_order_failed;
    bool compact_blockskip_flush;
    bool contiguous;
    struct zone_padding _pad3_;
    atomic_long_t vm_stat[11];
    atomic_long_t vm_numa_stat[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct zone {
    long unsigned int _watermark[3];
    long unsigned int watermark_boost;
    long unsigned int nr_reserved_highatomic;
    long int lowmem_reserve[5];
    int node;
    struct pglist_data *zone_pgdat;
    struct per_cpu_pages *per_cpu_pageset;
    struct per_cpu_zonestat *per_cpu_zonestats;
    int pageset_high;
    int pageset_batch;
    long unsigned int zone_start_pfn;
    atomic_long_t managed_pages;
    long unsigned int spanned_pages;
    long unsigned int present_pages;
    long unsigned int present_early_pages;
    const char *name;
    long unsigned int nr_isolate_pageblock;
    seqlock_t span_seqlock;
    int initialized;
    struct zone_padding _pad1_;
    struct free_area free_area[11];
    long unsigned int flags;
    spinlock_t lock;
    struct zone_padding _pad2_;
    long unsigned int percpu_drift_mark;
    long unsigned int compact_cached_free_pfn;
    long unsigned int compact_cached_migrate_pfn[2];
    long unsigned int compact_init_migrate_pfn;
    long unsigned int compact_init_free_pfn;
    unsigned int compact_considered;
    unsigned int compact_defer_shift;
    int compact_order_failed;
    bool compact_blockskip_flush;
    bool contiguous;
    struct zone_padding _pad3_;
    atomic_long_t vm_stat[11];
    atomic_long_t vm_numa_event[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct zone {
    long unsigned int _watermark[4];
    long unsigned int watermark_boost;
    long unsigned int nr_reserved_highatomic;
    long int lowmem_reserve[5];
    int node;
    struct pglist_data *zone_pgdat;
    struct per_cpu_pages *per_cpu_pageset;
    struct per_cpu_zonestat *per_cpu_zonestats;
    int pageset_high;
    int pageset_batch;
    long unsigned int zone_start_pfn;
    atomic_long_t managed_pages;
    long unsigned int spanned_pages;
    long unsigned int present_pages;
    long unsigned int present_early_pages;
    const char *name;
    long unsigned int nr_isolate_pageblock;
    seqlock_t span_seqlock;
    int initialized;
    struct zone_padding _pad1_;
    struct free_area free_area[11];
    long unsigned int flags;
    spinlock_t lock;
    struct zone_padding _pad2_;
    long unsigned int percpu_drift_mark;
    long unsigned int compact_cached_free_pfn;
    long unsigned int compact_cached_migrate_pfn[2];
    long unsigned int compact_init_migrate_pfn;
    long unsigned int compact_init_free_pfn;
    unsigned int compact_considered;
    unsigned int compact_defer_shift;
    int compact_order_failed;
    bool compact_blockskip_flush;
    bool contiguous;
    struct zone_padding _pad3_;
    atomic_long_t vm_stat[11];
    atomic_long_t vm_numa_event[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct zone {
    long unsigned int _watermark[4];
    long unsigned int watermark_boost;
    long unsigned int nr_reserved_highatomic;
    long int lowmem_reserve[5];
    int node;
    struct pglist_data *zone_pgdat;
    struct per_cpu_pages *per_cpu_pageset;
    struct per_cpu_zonestat *per_cpu_zonestats;
    int pageset_high;
    int pageset_batch;
    long unsigned int zone_start_pfn;
    atomic_long_t managed_pages;
    long unsigned int spanned_pages;
    long unsigned int present_pages;
    long unsigned int present_early_pages;
    const char *name;
    long unsigned int nr_isolate_pageblock;
    seqlock_t span_seqlock;
    int initialized;
    struct cacheline_padding _pad1_;
    struct free_area free_area[11];
    long unsigned int flags;
    spinlock_t lock;
    struct cacheline_padding _pad2_;
    long unsigned int percpu_drift_mark;
    long unsigned int compact_cached_free_pfn;
    long unsigned int compact_cached_migrate_pfn[2];
    long unsigned int compact_init_migrate_pfn;
    long unsigned int compact_init_free_pfn;
    unsigned int compact_considered;
    unsigned int compact_defer_shift;
    int compact_order_failed;
    bool compact_blockskip_flush;
    bool contiguous;
    struct cacheline_padding _pad3_;
    atomic_long_t vm_stat[11];
    atomic_long_t vm_numa_event[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct zone {
    long unsigned int _watermark[4];
    long unsigned int watermark_boost;
    long unsigned int nr_reserved_highatomic;
    long int lowmem_reserve[5];
    int node;
    struct pglist_data *zone_pgdat;
    struct per_cpu_pages *per_cpu_pageset;
    struct per_cpu_zonestat *per_cpu_zonestats;
    int pageset_high;
    int pageset_batch;
    long unsigned int zone_start_pfn;
    atomic_long_t managed_pages;
    long unsigned int spanned_pages;
    long unsigned int present_pages;
    long unsigned int present_early_pages;
    const char *name;
    long unsigned int nr_isolate_pageblock;
    seqlock_t span_seqlock;
    int initialized;
    struct cacheline_padding _pad1_;
    struct free_area free_area[11];
    struct list_head unaccepted_pages;
    long unsigned int flags;
    spinlock_t lock;
    struct cacheline_padding _pad2_;
    long unsigned int percpu_drift_mark;
    long unsigned int compact_cached_free_pfn;
    long unsigned int compact_cached_migrate_pfn[2];
    long unsigned int compact_init_migrate_pfn;
    long unsigned int compact_init_free_pfn;
    unsigned int compact_considered;
    unsigned int compact_defer_shift;
    int compact_order_failed;
    bool compact_blockskip_flush;
    bool contiguous;
    struct cacheline_padding _pad3_;
    atomic_long_t vm_stat[12];
    atomic_long_t vm_numa_event[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct zone {
    long unsigned int _watermark[4];
    long unsigned int watermark_boost;
    long unsigned int nr_reserved_highatomic;
    long int lowmem_reserve[5];
    int node;
    struct pglist_data *zone_pgdat;
    struct per_cpu_pages *per_cpu_pageset;
    struct per_cpu_zonestat *per_cpu_zonestats;
    int pageset_high_min;
    int pageset_high_max;
    int pageset_batch;
    long unsigned int zone_start_pfn;
    atomic_long_t managed_pages;
    long unsigned int spanned_pages;
    long unsigned int present_pages;
    long unsigned int present_early_pages;
    const char *name;
    long unsigned int nr_isolate_pageblock;
    seqlock_t span_seqlock;
    int initialized;
    struct cacheline_padding _pad1_;
    struct free_area free_area[11];
    struct list_head unaccepted_pages;
    long unsigned int flags;
    spinlock_t lock;
    struct cacheline_padding _pad2_;
    long unsigned int percpu_drift_mark;
    long unsigned int compact_cached_free_pfn;
    long unsigned int compact_cached_migrate_pfn[2];
    long unsigned int compact_init_migrate_pfn;
    long unsigned int compact_init_free_pfn;
    unsigned int compact_considered;
    unsigned int compact_defer_shift;
    int compact_order_failed;
    bool compact_blockskip_flush;
    bool contiguous;
    struct cacheline_padding _pad3_;
    atomic_long_t vm_stat[12];
    atomic_long_t vm_numa_event[6];
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
struct zone {
    long unsigned int _watermark[3];
    long unsigned int watermark_boost;
    long unsigned int nr_reserved_highatomic;
    long int lowmem_reserve[3];
    int node;
    struct pglist_data *zone_pgdat;
    struct per_cpu_pageset *pageset;
    long unsigned int zone_start_pfn;
    atomic_long_t managed_pages;
    long unsigned int spanned_pages;
    long unsigned int present_pages;
    const char *name;
    long unsigned int nr_isolate_pageblock;
    seqlock_t span_seqlock;
    int initialized;
    struct zone_padding _pad1_;
    struct free_area free_area[13];
    long unsigned int flags;
    spinlock_t lock;
    struct zone_padding _pad2_;
    long unsigned int percpu_drift_mark;
    long unsigned int compact_cached_free_pfn;
    long unsigned int compact_cached_migrate_pfn[2];
    long unsigned int compact_init_migrate_pfn;
    long unsigned int compact_init_free_pfn;
    unsigned int compact_considered;
    unsigned int compact_defer_shift;
    int compact_order_failed;
    bool compact_blockskip_flush;
    bool contiguous;
    struct zone_padding _pad3_;
    atomic_long_t vm_stat[13];
    atomic_long_t vm_numa_stat[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct zone {
    long unsigned int _watermark[3];
    long unsigned int watermark_boost;
    long unsigned int nr_reserved_highatomic;
    long int lowmem_reserve[3];
    struct pglist_data *zone_pgdat;
    struct per_cpu_pageset *pageset;
    long unsigned int *pageblock_flags;
    long unsigned int zone_start_pfn;
    atomic_long_t managed_pages;
    long unsigned int spanned_pages;
    long unsigned int present_pages;
    const char *name;
    long unsigned int nr_isolate_pageblock;
    int initialized;
    struct zone_padding _pad1_;
    struct free_area free_area[12];
    long unsigned int flags;
    spinlock_t lock;
    struct zone_padding _pad2_;
    long unsigned int percpu_drift_mark;
    long unsigned int compact_cached_free_pfn;
    long unsigned int compact_cached_migrate_pfn[2];
    long unsigned int compact_init_migrate_pfn;
    long unsigned int compact_init_free_pfn;
    unsigned int compact_considered;
    unsigned int compact_defer_shift;
    int compact_order_failed;
    bool compact_blockskip_flush;
    bool contiguous;
    struct zone_padding _pad3_;
    atomic_long_t vm_stat[13];
    atomic_long_t vm_numa_stat[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct zone {
    long unsigned int _watermark[3];
    long unsigned int watermark_boost;
    long unsigned int nr_reserved_highatomic;
    long int lowmem_reserve[3];
    int node;
    struct pglist_data *zone_pgdat;
    struct per_cpu_pageset *pageset;
    long unsigned int zone_start_pfn;
    atomic_long_t managed_pages;
    long unsigned int spanned_pages;
    long unsigned int present_pages;
    const char *name;
    long unsigned int nr_isolate_pageblock;
    seqlock_t span_seqlock;
    int initialized;
    struct zone_padding _pad1_;
    struct free_area free_area[9];
    long unsigned int flags;
    spinlock_t lock;
    struct zone_padding _pad2_;
    long unsigned int percpu_drift_mark;
    long unsigned int compact_cached_free_pfn;
    long unsigned int compact_cached_migrate_pfn[2];
    long unsigned int compact_init_migrate_pfn;
    long unsigned int compact_init_free_pfn;
    unsigned int compact_considered;
    unsigned int compact_defer_shift;
    int compact_order_failed;
    bool compact_blockskip_flush;
    bool contiguous;
    struct zone_padding _pad3_;
    atomic_long_t vm_stat[13];
    atomic_long_t vm_numa_stat[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct zone {
    long unsigned int _watermark[3];
    long unsigned int watermark_boost;
    long unsigned int nr_reserved_highatomic;
    long int lowmem_reserve[3];
    struct pglist_data *zone_pgdat;
    struct per_cpu_pageset *pageset;
    long unsigned int zone_start_pfn;
    atomic_long_t managed_pages;
    long unsigned int spanned_pages;
    long unsigned int present_pages;
    const char *name;
    long unsigned int nr_isolate_pageblock;
    int initialized;
    struct zone_padding _pad1_;
    struct free_area free_area[11];
    long unsigned int flags;
    spinlock_t lock;
    struct zone_padding _pad2_;
    long unsigned int percpu_drift_mark;
    long unsigned int compact_cached_free_pfn;
    long unsigned int compact_cached_migrate_pfn[2];
    long unsigned int compact_init_migrate_pfn;
    long unsigned int compact_init_free_pfn;
    unsigned int compact_considered;
    unsigned int compact_defer_shift;
    int compact_order_failed;
    bool compact_blockskip_flush;
    bool contiguous;
    struct zone_padding _pad3_;
    atomic_long_t vm_stat[13];
    atomic_long_t vm_numa_stat[0];
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
struct zone {
    long unsigned int _watermark[3];
    long unsigned int watermark_boost;
    long unsigned int nr_reserved_highatomic;
    long int lowmem_reserve[5];
    int node;
    struct pglist_data *zone_pgdat;
    struct per_cpu_pageset *pageset;
    long unsigned int zone_start_pfn;
    atomic_long_t managed_pages;
    long unsigned int spanned_pages;
    long unsigned int present_pages;
    const char *name;
    long unsigned int nr_isolate_pageblock;
    seqlock_t span_seqlock;
    int initialized;
    struct zone_padding _pad1_;
    struct free_area free_area[11];
    long unsigned int flags;
    spinlock_t lock;
    struct zone_padding _pad2_;
    long unsigned int percpu_drift_mark;
    long unsigned int compact_cached_free_pfn;
    long unsigned int compact_cached_migrate_pfn[2];
    long unsigned int compact_init_migrate_pfn;
    long unsigned int compact_init_free_pfn;
    unsigned int compact_considered;
    unsigned int compact_defer_shift;
    int compact_order_failed;
    bool compact_blockskip_flush;
    bool contiguous;
    struct zone_padding _pad3_;
    atomic_long_t vm_stat[13];
    atomic_long_t vm_numa_stat[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct zone {
    long unsigned int _watermark[3];
    long unsigned int watermark_boost;
    long unsigned int nr_reserved_highatomic;
    long int lowmem_reserve[5];
    int node;
    struct pglist_data *zone_pgdat;
    struct per_cpu_pageset *pageset;
    long unsigned int zone_start_pfn;
    atomic_long_t managed_pages;
    long unsigned int spanned_pages;
    long unsigned int present_pages;
    const char *name;
    long unsigned int nr_isolate_pageblock;
    seqlock_t span_seqlock;
    int initialized;
    struct zone_padding _pad1_;
    struct free_area free_area[11];
    long unsigned int flags;
    spinlock_t lock;
    struct zone_padding _pad2_;
    long unsigned int percpu_drift_mark;
    long unsigned int compact_cached_free_pfn;
    long unsigned int compact_cached_migrate_pfn[2];
    long unsigned int compact_init_migrate_pfn;
    long unsigned int compact_init_free_pfn;
    unsigned int compact_considered;
    unsigned int compact_defer_shift;
    int compact_order_failed;
    bool compact_blockskip_flush;
    bool contiguous;
    struct zone_padding _pad3_;
    atomic_long_t vm_stat[13];
    atomic_long_t vm_numa_stat[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct zone {
    long unsigned int _watermark[3];
    long unsigned int watermark_boost;
    long unsigned int nr_reserved_highatomic;
    long int lowmem_reserve[5];
    int node;
    struct pglist_data *zone_pgdat;
    struct per_cpu_pageset *pageset;
    long unsigned int zone_start_pfn;
    atomic_long_t managed_pages;
    long unsigned int spanned_pages;
    long unsigned int present_pages;
    const char *name;
    long unsigned int nr_isolate_pageblock;
    seqlock_t span_seqlock;
    int initialized;
    struct zone_padding _pad1_;
    struct free_area free_area[11];
    long unsigned int flags;
    spinlock_t lock;
    struct zone_padding _pad2_;
    long unsigned int percpu_drift_mark;
    long unsigned int compact_cached_free_pfn;
    long unsigned int compact_cached_migrate_pfn[2];
    long unsigned int compact_init_migrate_pfn;
    long unsigned int compact_init_free_pfn;
    unsigned int compact_considered;
    unsigned int compact_defer_shift;
    int compact_order_failed;
    bool compact_blockskip_flush;
    bool contiguous;
    struct zone_padding _pad3_;
    atomic_long_t vm_stat[13];
    atomic_long_t vm_numa_stat[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct zone {
    long unsigned int _watermark[3];
    long unsigned int watermark_boost;
    long unsigned int nr_reserved_highatomic;
    long int lowmem_reserve[5];
    int node;
    struct pglist_data *zone_pgdat;
    struct per_cpu_pageset *pageset;
    long unsigned int zone_start_pfn;
    atomic_long_t managed_pages;
    long unsigned int spanned_pages;
    long unsigned int present_pages;
    const char *name;
    long unsigned int nr_isolate_pageblock;
    seqlock_t span_seqlock;
    int initialized;
    struct zone_padding _pad1_;
    struct free_area free_area[11];
    long unsigned int flags;
    spinlock_t lock;
    struct zone_padding _pad2_;
    long unsigned int percpu_drift_mark;
    long unsigned int compact_cached_free_pfn;
    long unsigned int compact_cached_migrate_pfn[2];
    long unsigned int compact_init_migrate_pfn;
    long unsigned int compact_init_free_pfn;
    unsigned int compact_considered;
    unsigned int compact_defer_shift;
    int compact_order_failed;
    bool compact_blockskip_flush;
    bool contiguous;
    struct zone_padding _pad3_;
    atomic_long_t vm_stat[13];
    atomic_long_t vm_numa_stat[6];
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
<code>bool contiguous</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int inactive_ratio</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int dirty_balance_reserve</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int min_unmapped_pages</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int min_slab_pages</code>
</li>
<li>
<b>Field removed. </b>
<code>spinlock_t lru_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>struct lruvec lruvec</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_long_t inactive_age</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t vm_stat[39]</code> ➡️ <code>atomic_long_t vm_stat[21]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int initialized</code>
</li>
<li>
<b>Field removed. </b>
<code>wait_queue_head_t *wait_table</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int wait_table_hash_nr_entries</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int wait_table_bits</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>atomic_long_t vm_stat[21]</code> ➡️ <code>atomic_long_t vm_stat[19]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>atomic_long_t vm_numa_stat[6]</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t vm_stat[19]</code> ➡️ <code>atomic_long_t vm_stat[13]</code>
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
<code>long unsigned int _watermark[3]</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int watermark_boost</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int watermark[3]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int managed_pages</code> ➡️ <code>atomic_long_t managed_pages</code>
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
<code>long unsigned int compact_init_migrate_pfn</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int compact_init_free_pfn</code>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int pageset_high</code>
</li>
<li>
<b>Field added. </b>
<code>int pageset_batch</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t vm_stat[13]</code> ➡️ <code>atomic_long_t vm_stat[11]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct per_cpu_pages *per_cpu_pageset</code>
</li>
<li>
<b>Field added. </b>
<code>struct per_cpu_zonestat *per_cpu_zonestats</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int present_early_pages</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t vm_numa_event[6]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct per_cpu_pageset *pageset</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_long_t vm_numa_stat[6]</code>
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
<code>long unsigned int _watermark[3]</code> ➡️ <code>long unsigned int _watermark[4]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct zone_padding _pad1_</code> ➡️ <code>struct cacheline_padding _pad1_</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct zone_padding _pad2_</code> ➡️ <code>struct cacheline_padding _pad2_</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct zone_padding _pad3_</code> ➡️ <code>struct cacheline_padding _pad3_</code>
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
<code>struct list_head unaccepted_pages</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t vm_stat[11]</code> ➡️ <code>atomic_long_t vm_stat[12]</code>
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
<code>int pageset_high_min</code>
</li>
<li>
<b>Field added. </b>
<code>int pageset_high_max</code>
</li>
<li>
<b>Field removed. </b>
<code>int pageset_high</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>arm64</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long int lowmem_reserve[5]</code> ➡️ <code>long int lowmem_reserve[3]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct free_area free_area[11]</code> ➡️ <code>struct free_area free_area[13]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int *pageblock_flags</code>
</li>
<li>
<b>Field removed. </b>
<code>int node</code>
</li>
<li>
<b>Field removed. </b>
<code>seqlock_t span_seqlock</code>
</li>
<li>
<b>Field type changed. </b>
<code>long int lowmem_reserve[5]</code> ➡️ <code>long int lowmem_reserve[3]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct free_area free_area[11]</code> ➡️ <code>struct free_area free_area[12]</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t vm_numa_stat[6]</code> ➡️ <code>atomic_long_t vm_numa_stat[0]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long int lowmem_reserve[5]</code> ➡️ <code>long int lowmem_reserve[3]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct free_area free_area[11]</code> ➡️ <code>struct free_area free_area[9]</code>
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
<code>int node</code>
</li>
<li>
<b>Field removed. </b>
<code>seqlock_t span_seqlock</code>
</li>
<li>
<b>Field type changed. </b>
<code>long int lowmem_reserve[5]</code> ➡️ <code>long int lowmem_reserve[3]</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t vm_numa_stat[6]</code> ➡️ <code>atomic_long_t vm_numa_stat[0]</code>
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
