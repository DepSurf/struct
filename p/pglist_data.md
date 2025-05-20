# Struct: <code>pglist_data</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct pglist_data {
    struct zone node_zones[5];
    struct zonelist node_zonelists[2];
    int nr_zones;
    spinlock_t node_size_lock;
    long unsigned int node_start_pfn;
    long unsigned int node_present_pages;
    long unsigned int node_spanned_pages;
    int node_id;
    wait_queue_head_t kswapd_wait;
    wait_queue_head_t pfmemalloc_wait;
    struct task_struct *kswapd;
    int kswapd_max_order;
    enum zone_type classzone_idx;
    spinlock_t numabalancing_migrate_lock;
    long unsigned int numabalancing_migrate_next_window;
    long unsigned int numabalancing_migrate_nr_pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct pglist_data {
    struct zone node_zones[5];
    struct zonelist node_zonelists[2];
    int nr_zones;
    spinlock_t node_size_lock;
    long unsigned int node_start_pfn;
    long unsigned int node_present_pages;
    long unsigned int node_spanned_pages;
    int node_id;
    wait_queue_head_t kswapd_wait;
    wait_queue_head_t pfmemalloc_wait;
    struct task_struct *kswapd;
    int kswapd_order;
    enum zone_type kswapd_classzone_idx;
    int kcompactd_max_order;
    enum zone_type kcompactd_classzone_idx;
    wait_queue_head_t kcompactd_wait;
    struct task_struct *kcompactd;
    spinlock_t numabalancing_migrate_lock;
    long unsigned int numabalancing_migrate_next_window;
    long unsigned int numabalancing_migrate_nr_pages;
    long unsigned int totalreserve_pages;
    long unsigned int min_unmapped_pages;
    long unsigned int min_slab_pages;
    struct zone_padding _pad1_;
    spinlock_t lru_lock;
    spinlock_t split_queue_lock;
    struct list_head split_queue;
    long unsigned int split_queue_len;
    struct lruvec lruvec;
    unsigned int inactive_ratio;
    long unsigned int flags;
    struct zone_padding _pad2_;
    struct per_cpu_nodestat *per_cpu_nodestats;
    atomic_long_t vm_stat[26];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct pglist_data {
    struct zone node_zones[5];
    struct zonelist node_zonelists[2];
    int nr_zones;
    spinlock_t node_size_lock;
    long unsigned int node_start_pfn;
    long unsigned int node_present_pages;
    long unsigned int node_spanned_pages;
    int node_id;
    wait_queue_head_t kswapd_wait;
    wait_queue_head_t pfmemalloc_wait;
    struct task_struct *kswapd;
    int kswapd_order;
    enum zone_type kswapd_classzone_idx;
    int kcompactd_max_order;
    enum zone_type kcompactd_classzone_idx;
    wait_queue_head_t kcompactd_wait;
    struct task_struct *kcompactd;
    spinlock_t numabalancing_migrate_lock;
    long unsigned int numabalancing_migrate_next_window;
    long unsigned int numabalancing_migrate_nr_pages;
    long unsigned int totalreserve_pages;
    long unsigned int min_unmapped_pages;
    long unsigned int min_slab_pages;
    struct zone_padding _pad1_;
    spinlock_t lru_lock;
    spinlock_t split_queue_lock;
    struct list_head split_queue;
    long unsigned int split_queue_len;
    struct lruvec lruvec;
    unsigned int inactive_ratio;
    long unsigned int flags;
    struct zone_padding _pad2_;
    struct per_cpu_nodestat *per_cpu_nodestats;
    atomic_long_t vm_stat[26];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct pglist_data {
    struct zone node_zones[5];
    struct zonelist node_zonelists[2];
    int nr_zones;
    spinlock_t node_size_lock;
    long unsigned int node_start_pfn;
    long unsigned int node_present_pages;
    long unsigned int node_spanned_pages;
    int node_id;
    wait_queue_head_t kswapd_wait;
    wait_queue_head_t pfmemalloc_wait;
    struct task_struct *kswapd;
    int kswapd_order;
    enum zone_type kswapd_classzone_idx;
    int kswapd_failures;
    int kcompactd_max_order;
    enum zone_type kcompactd_classzone_idx;
    wait_queue_head_t kcompactd_wait;
    struct task_struct *kcompactd;
    spinlock_t numabalancing_migrate_lock;
    long unsigned int numabalancing_migrate_next_window;
    long unsigned int numabalancing_migrate_nr_pages;
    long unsigned int totalreserve_pages;
    long unsigned int min_unmapped_pages;
    long unsigned int min_slab_pages;
    struct zone_padding _pad1_;
    spinlock_t lru_lock;
    spinlock_t split_queue_lock;
    struct list_head split_queue;
    long unsigned int split_queue_len;
    struct lruvec lruvec;
    unsigned int inactive_ratio;
    long unsigned int flags;
    struct zone_padding _pad2_;
    struct per_cpu_nodestat *per_cpu_nodestats;
    atomic_long_t vm_stat[27];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct pglist_data {
    struct zone node_zones[5];
    struct zonelist node_zonelists[2];
    int nr_zones;
    spinlock_t node_size_lock;
    long unsigned int node_start_pfn;
    long unsigned int node_present_pages;
    long unsigned int node_spanned_pages;
    int node_id;
    wait_queue_head_t kswapd_wait;
    wait_queue_head_t pfmemalloc_wait;
    struct task_struct *kswapd;
    int kswapd_order;
    enum zone_type kswapd_classzone_idx;
    int kswapd_failures;
    int kcompactd_max_order;
    enum zone_type kcompactd_classzone_idx;
    wait_queue_head_t kcompactd_wait;
    struct task_struct *kcompactd;
    spinlock_t numabalancing_migrate_lock;
    long unsigned int numabalancing_migrate_next_window;
    long unsigned int numabalancing_migrate_nr_pages;
    long unsigned int totalreserve_pages;
    long unsigned int min_unmapped_pages;
    long unsigned int min_slab_pages;
    struct zone_padding _pad1_;
    spinlock_t lru_lock;
    spinlock_t split_queue_lock;
    struct list_head split_queue;
    long unsigned int split_queue_len;
    struct lruvec lruvec;
    long unsigned int flags;
    struct zone_padding _pad2_;
    struct per_cpu_nodestat *per_cpu_nodestats;
    atomic_long_t vm_stat[27];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct pglist_data {
    struct zone node_zones[5];
    struct zonelist node_zonelists[2];
    int nr_zones;
    spinlock_t node_size_lock;
    long unsigned int node_start_pfn;
    long unsigned int node_present_pages;
    long unsigned int node_spanned_pages;
    int node_id;
    wait_queue_head_t kswapd_wait;
    wait_queue_head_t pfmemalloc_wait;
    struct task_struct *kswapd;
    int kswapd_order;
    enum zone_type kswapd_classzone_idx;
    int kswapd_failures;
    int kcompactd_max_order;
    enum zone_type kcompactd_classzone_idx;
    wait_queue_head_t kcompactd_wait;
    struct task_struct *kcompactd;
    spinlock_t numabalancing_migrate_lock;
    long unsigned int numabalancing_migrate_next_window;
    long unsigned int numabalancing_migrate_nr_pages;
    long unsigned int totalreserve_pages;
    long unsigned int min_unmapped_pages;
    long unsigned int min_slab_pages;
    struct zone_padding _pad1_;
    spinlock_t lru_lock;
    spinlock_t split_queue_lock;
    struct list_head split_queue;
    long unsigned int split_queue_len;
    struct lruvec lruvec;
    long unsigned int flags;
    struct zone_padding _pad2_;
    struct per_cpu_nodestat *per_cpu_nodestats;
    atomic_long_t vm_stat[28];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct pglist_data {
    struct zone node_zones[5];
    struct zonelist node_zonelists[2];
    int nr_zones;
    spinlock_t node_size_lock;
    long unsigned int node_start_pfn;
    long unsigned int node_present_pages;
    long unsigned int node_spanned_pages;
    int node_id;
    wait_queue_head_t kswapd_wait;
    wait_queue_head_t pfmemalloc_wait;
    struct task_struct *kswapd;
    int kswapd_order;
    enum zone_type kswapd_classzone_idx;
    int kswapd_failures;
    int kcompactd_max_order;
    enum zone_type kcompactd_classzone_idx;
    wait_queue_head_t kcompactd_wait;
    struct task_struct *kcompactd;
    long unsigned int totalreserve_pages;
    long unsigned int min_unmapped_pages;
    long unsigned int min_slab_pages;
    struct zone_padding _pad1_;
    spinlock_t lru_lock;
    spinlock_t split_queue_lock;
    struct list_head split_queue;
    long unsigned int split_queue_len;
    struct lruvec lruvec;
    long unsigned int flags;
    struct zone_padding _pad2_;
    struct per_cpu_nodestat *per_cpu_nodestats;
    atomic_long_t vm_stat[30];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct pglist_data {
    struct zone node_zones[5];
    struct zonelist node_zonelists[2];
    int nr_zones;
    spinlock_t node_size_lock;
    long unsigned int node_start_pfn;
    long unsigned int node_present_pages;
    long unsigned int node_spanned_pages;
    int node_id;
    wait_queue_head_t kswapd_wait;
    wait_queue_head_t pfmemalloc_wait;
    struct task_struct *kswapd;
    int kswapd_order;
    enum zone_type kswapd_classzone_idx;
    int kswapd_failures;
    int kcompactd_max_order;
    enum zone_type kcompactd_classzone_idx;
    wait_queue_head_t kcompactd_wait;
    struct task_struct *kcompactd;
    long unsigned int totalreserve_pages;
    long unsigned int min_unmapped_pages;
    long unsigned int min_slab_pages;
    struct zone_padding _pad1_;
    spinlock_t lru_lock;
    spinlock_t split_queue_lock;
    struct list_head split_queue;
    long unsigned int split_queue_len;
    struct lruvec lruvec;
    long unsigned int flags;
    struct zone_padding _pad2_;
    struct per_cpu_nodestat *per_cpu_nodestats;
    atomic_long_t vm_stat[30];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct pglist_data {
    struct zone node_zones[5];
    struct zonelist node_zonelists[2];
    int nr_zones;
    spinlock_t node_size_lock;
    long unsigned int node_start_pfn;
    long unsigned int node_present_pages;
    long unsigned int node_spanned_pages;
    int node_id;
    wait_queue_head_t kswapd_wait;
    wait_queue_head_t pfmemalloc_wait;
    struct task_struct *kswapd;
    int kswapd_order;
    enum zone_type kswapd_classzone_idx;
    int kswapd_failures;
    int kcompactd_max_order;
    enum zone_type kcompactd_classzone_idx;
    wait_queue_head_t kcompactd_wait;
    struct task_struct *kcompactd;
    long unsigned int totalreserve_pages;
    long unsigned int min_unmapped_pages;
    long unsigned int min_slab_pages;
    struct zone_padding _pad1_;
    spinlock_t lru_lock;
    struct deferred_split deferred_split_queue;
    struct lruvec lruvec;
    long unsigned int flags;
    struct zone_padding _pad2_;
    struct per_cpu_nodestat *per_cpu_nodestats;
    atomic_long_t vm_stat[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct pglist_data {
    struct zone node_zones[5];
    struct zonelist node_zonelists[2];
    int nr_zones;
    spinlock_t node_size_lock;
    long unsigned int node_start_pfn;
    long unsigned int node_present_pages;
    long unsigned int node_spanned_pages;
    int node_id;
    wait_queue_head_t kswapd_wait;
    wait_queue_head_t pfmemalloc_wait;
    struct task_struct *kswapd;
    int kswapd_order;
    enum zone_type kswapd_highest_zoneidx;
    int kswapd_failures;
    int kcompactd_max_order;
    enum zone_type kcompactd_highest_zoneidx;
    wait_queue_head_t kcompactd_wait;
    struct task_struct *kcompactd;
    long unsigned int totalreserve_pages;
    long unsigned int min_unmapped_pages;
    long unsigned int min_slab_pages;
    struct zone_padding _pad1_;
    spinlock_t lru_lock;
    struct deferred_split deferred_split_queue;
    struct lruvec __lruvec;
    long unsigned int flags;
    struct zone_padding _pad2_;
    struct per_cpu_nodestat *per_cpu_nodestats;
    atomic_long_t vm_stat[33];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct pglist_data {
    struct zone node_zones[5];
    struct zonelist node_zonelists[2];
    int nr_zones;
    spinlock_t node_size_lock;
    long unsigned int node_start_pfn;
    long unsigned int node_present_pages;
    long unsigned int node_spanned_pages;
    int node_id;
    wait_queue_head_t kswapd_wait;
    wait_queue_head_t pfmemalloc_wait;
    struct task_struct *kswapd;
    int kswapd_order;
    enum zone_type kswapd_highest_zoneidx;
    int kswapd_failures;
    int kcompactd_max_order;
    enum zone_type kcompactd_highest_zoneidx;
    wait_queue_head_t kcompactd_wait;
    struct task_struct *kcompactd;
    long unsigned int totalreserve_pages;
    long unsigned int min_unmapped_pages;
    long unsigned int min_slab_pages;
    struct zone_padding _pad1_;
    struct deferred_split deferred_split_queue;
    struct lruvec __lruvec;
    long unsigned int flags;
    struct zone_padding _pad2_;
    struct per_cpu_nodestat *per_cpu_nodestats;
    atomic_long_t vm_stat[38];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct pglist_data {
    struct zone node_zones[5];
    struct zonelist node_zonelists[2];
    int nr_zones;
    spinlock_t node_size_lock;
    long unsigned int node_start_pfn;
    long unsigned int node_present_pages;
    long unsigned int node_spanned_pages;
    int node_id;
    wait_queue_head_t kswapd_wait;
    wait_queue_head_t pfmemalloc_wait;
    struct task_struct *kswapd;
    int kswapd_order;
    enum zone_type kswapd_highest_zoneidx;
    int kswapd_failures;
    int kcompactd_max_order;
    enum zone_type kcompactd_highest_zoneidx;
    wait_queue_head_t kcompactd_wait;
    struct task_struct *kcompactd;
    long unsigned int totalreserve_pages;
    long unsigned int min_unmapped_pages;
    long unsigned int min_slab_pages;
    struct zone_padding _pad1_;
    struct deferred_split deferred_split_queue;
    struct lruvec __lruvec;
    long unsigned int flags;
    struct zone_padding _pad2_;
    struct per_cpu_nodestat *per_cpu_nodestats;
    atomic_long_t vm_stat[39];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct pglist_data {
    struct zone node_zones[5];
    struct zonelist node_zonelists[2];
    int nr_zones;
    spinlock_t node_size_lock;
    long unsigned int node_start_pfn;
    long unsigned int node_present_pages;
    long unsigned int node_spanned_pages;
    int node_id;
    wait_queue_head_t kswapd_wait;
    wait_queue_head_t pfmemalloc_wait;
    struct task_struct *kswapd;
    int kswapd_order;
    enum zone_type kswapd_highest_zoneidx;
    int kswapd_failures;
    int kcompactd_max_order;
    enum zone_type kcompactd_highest_zoneidx;
    wait_queue_head_t kcompactd_wait;
    struct task_struct *kcompactd;
    bool proactive_compact_trigger;
    long unsigned int totalreserve_pages;
    long unsigned int min_unmapped_pages;
    long unsigned int min_slab_pages;
    struct zone_padding _pad1_;
    struct deferred_split deferred_split_queue;
    struct lruvec __lruvec;
    long unsigned int flags;
    struct zone_padding _pad2_;
    struct per_cpu_nodestat *per_cpu_nodestats;
    atomic_long_t vm_stat[39];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct pglist_data {
    struct zone node_zones[5];
    struct zonelist node_zonelists[2];
    int nr_zones;
    spinlock_t node_size_lock;
    long unsigned int node_start_pfn;
    long unsigned int node_present_pages;
    long unsigned int node_spanned_pages;
    int node_id;
    wait_queue_head_t kswapd_wait;
    wait_queue_head_t pfmemalloc_wait;
    wait_queue_head_t reclaim_wait[4];
    atomic_t nr_writeback_throttled;
    long unsigned int nr_reclaim_start;
    struct task_struct *kswapd;
    int kswapd_order;
    enum zone_type kswapd_highest_zoneidx;
    int kswapd_failures;
    int kcompactd_max_order;
    enum zone_type kcompactd_highest_zoneidx;
    wait_queue_head_t kcompactd_wait;
    struct task_struct *kcompactd;
    bool proactive_compact_trigger;
    long unsigned int totalreserve_pages;
    long unsigned int min_unmapped_pages;
    long unsigned int min_slab_pages;
    struct zone_padding _pad1_;
    struct deferred_split deferred_split_queue;
    struct lruvec __lruvec;
    long unsigned int flags;
    struct zone_padding _pad2_;
    struct per_cpu_nodestat *per_cpu_nodestats;
    atomic_long_t vm_stat[41];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct pglist_data {
    struct zone node_zones[5];
    struct zonelist node_zonelists[2];
    int nr_zones;
    spinlock_t node_size_lock;
    long unsigned int node_start_pfn;
    long unsigned int node_present_pages;
    long unsigned int node_spanned_pages;
    int node_id;
    wait_queue_head_t kswapd_wait;
    wait_queue_head_t pfmemalloc_wait;
    wait_queue_head_t reclaim_wait[4];
    atomic_t nr_writeback_throttled;
    long unsigned int nr_reclaim_start;
    struct mutex kswapd_lock;
    struct task_struct *kswapd;
    int kswapd_order;
    enum zone_type kswapd_highest_zoneidx;
    int kswapd_failures;
    int kcompactd_max_order;
    enum zone_type kcompactd_highest_zoneidx;
    wait_queue_head_t kcompactd_wait;
    struct task_struct *kcompactd;
    bool proactive_compact_trigger;
    long unsigned int totalreserve_pages;
    long unsigned int min_unmapped_pages;
    long unsigned int min_slab_pages;
    struct cacheline_padding _pad1_;
    struct deferred_split deferred_split_queue;
    unsigned int nbp_rl_start;
    long unsigned int nbp_rl_nr_cand;
    unsigned int nbp_threshold;
    unsigned int nbp_th_start;
    long unsigned int nbp_th_nr_cand;
    struct lruvec __lruvec;
    long unsigned int flags;
    struct lru_gen_mm_walk mm_walk;
    struct cacheline_padding _pad2_;
    struct per_cpu_nodestat *per_cpu_nodestats;
    atomic_long_t vm_stat[43];
    struct memory_tier *memtier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct pglist_data {
    struct zone node_zones[5];
    struct zonelist node_zonelists[2];
    int nr_zones;
    spinlock_t node_size_lock;
    long unsigned int node_start_pfn;
    long unsigned int node_present_pages;
    long unsigned int node_spanned_pages;
    int node_id;
    wait_queue_head_t kswapd_wait;
    wait_queue_head_t pfmemalloc_wait;
    wait_queue_head_t reclaim_wait[4];
    atomic_t nr_writeback_throttled;
    long unsigned int nr_reclaim_start;
    struct mutex kswapd_lock;
    struct task_struct *kswapd;
    int kswapd_order;
    enum zone_type kswapd_highest_zoneidx;
    int kswapd_failures;
    int kcompactd_max_order;
    enum zone_type kcompactd_highest_zoneidx;
    wait_queue_head_t kcompactd_wait;
    struct task_struct *kcompactd;
    bool proactive_compact_trigger;
    long unsigned int totalreserve_pages;
    long unsigned int min_unmapped_pages;
    long unsigned int min_slab_pages;
    struct cacheline_padding _pad1_;
    struct deferred_split deferred_split_queue;
    unsigned int nbp_rl_start;
    long unsigned int nbp_rl_nr_cand;
    unsigned int nbp_threshold;
    unsigned int nbp_th_start;
    long unsigned int nbp_th_nr_cand;
    struct lruvec __lruvec;
    long unsigned int flags;
    struct lru_gen_mm_walk mm_walk;
    struct lru_gen_memcg memcg_lru;
    struct cacheline_padding _pad2_;
    struct per_cpu_nodestat *per_cpu_nodestats;
    atomic_long_t vm_stat[43];
    struct memory_tier *memtier;
    struct memory_failure_stats mf_stats;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct pglist_data {
    struct zone node_zones[5];
    struct zonelist node_zonelists[2];
    int nr_zones;
    spinlock_t node_size_lock;
    long unsigned int node_start_pfn;
    long unsigned int node_present_pages;
    long unsigned int node_spanned_pages;
    int node_id;
    wait_queue_head_t kswapd_wait;
    wait_queue_head_t pfmemalloc_wait;
    wait_queue_head_t reclaim_wait[4];
    atomic_t nr_writeback_throttled;
    long unsigned int nr_reclaim_start;
    struct mutex kswapd_lock;
    struct task_struct *kswapd;
    int kswapd_order;
    enum zone_type kswapd_highest_zoneidx;
    int kswapd_failures;
    int kcompactd_max_order;
    enum zone_type kcompactd_highest_zoneidx;
    wait_queue_head_t kcompactd_wait;
    struct task_struct *kcompactd;
    bool proactive_compact_trigger;
    long unsigned int totalreserve_pages;
    long unsigned int min_unmapped_pages;
    long unsigned int min_slab_pages;
    struct cacheline_padding _pad1_;
    struct deferred_split deferred_split_queue;
    unsigned int nbp_rl_start;
    long unsigned int nbp_rl_nr_cand;
    unsigned int nbp_threshold;
    unsigned int nbp_th_start;
    long unsigned int nbp_th_nr_cand;
    struct lruvec __lruvec;
    long unsigned int flags;
    struct lru_gen_mm_walk mm_walk;
    struct lru_gen_memcg memcg_lru;
    struct cacheline_padding _pad2_;
    struct per_cpu_nodestat *per_cpu_nodestats;
    atomic_long_t vm_stat[46];
    struct memory_tier *memtier;
    struct memory_failure_stats mf_stats;
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
struct pglist_data {
    struct zone node_zones[3];
    struct zonelist node_zonelists[2];
    int nr_zones;
    spinlock_t node_size_lock;
    long unsigned int node_start_pfn;
    long unsigned int node_present_pages;
    long unsigned int node_spanned_pages;
    int node_id;
    wait_queue_head_t kswapd_wait;
    wait_queue_head_t pfmemalloc_wait;
    struct task_struct *kswapd;
    int kswapd_order;
    enum zone_type kswapd_classzone_idx;
    int kswapd_failures;
    int kcompactd_max_order;
    enum zone_type kcompactd_classzone_idx;
    wait_queue_head_t kcompactd_wait;
    struct task_struct *kcompactd;
    long unsigned int totalreserve_pages;
    long unsigned int min_unmapped_pages;
    long unsigned int min_slab_pages;
    struct zone_padding _pad1_;
    spinlock_t lru_lock;
    struct deferred_split deferred_split_queue;
    struct lruvec lruvec;
    long unsigned int flags;
    struct zone_padding _pad2_;
    struct per_cpu_nodestat *per_cpu_nodestats;
    atomic_long_t vm_stat[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct pglist_data {
    struct zone node_zones[3];
    struct zonelist node_zonelists[1];
    int nr_zones;
    struct page *node_mem_map;
    struct page_ext *node_page_ext;
    long unsigned int node_start_pfn;
    long unsigned int node_present_pages;
    long unsigned int node_spanned_pages;
    int node_id;
    wait_queue_head_t kswapd_wait;
    wait_queue_head_t pfmemalloc_wait;
    struct task_struct *kswapd;
    int kswapd_order;
    enum zone_type kswapd_classzone_idx;
    int kswapd_failures;
    int kcompactd_max_order;
    enum zone_type kcompactd_classzone_idx;
    wait_queue_head_t kcompactd_wait;
    struct task_struct *kcompactd;
    long unsigned int totalreserve_pages;
    struct zone_padding _pad1_;
    spinlock_t lru_lock;
    struct lruvec lruvec;
    long unsigned int flags;
    struct zone_padding _pad2_;
    struct per_cpu_nodestat *per_cpu_nodestats;
    atomic_long_t vm_stat[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct pglist_data {
    struct zone node_zones[3];
    struct zonelist node_zonelists[2];
    int nr_zones;
    spinlock_t node_size_lock;
    long unsigned int node_start_pfn;
    long unsigned int node_present_pages;
    long unsigned int node_spanned_pages;
    int node_id;
    wait_queue_head_t kswapd_wait;
    wait_queue_head_t pfmemalloc_wait;
    struct task_struct *kswapd;
    int kswapd_order;
    enum zone_type kswapd_classzone_idx;
    int kswapd_failures;
    int kcompactd_max_order;
    enum zone_type kcompactd_classzone_idx;
    wait_queue_head_t kcompactd_wait;
    struct task_struct *kcompactd;
    long unsigned int totalreserve_pages;
    long unsigned int min_unmapped_pages;
    long unsigned int min_slab_pages;
    struct zone_padding _pad1_;
    spinlock_t lru_lock;
    struct deferred_split deferred_split_queue;
    struct lruvec lruvec;
    long unsigned int flags;
    struct zone_padding _pad2_;
    struct per_cpu_nodestat *per_cpu_nodestats;
    atomic_long_t vm_stat[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct pglist_data {
    struct zone node_zones[3];
    struct zonelist node_zonelists[1];
    int nr_zones;
    long unsigned int node_start_pfn;
    long unsigned int node_present_pages;
    long unsigned int node_spanned_pages;
    int node_id;
    wait_queue_head_t kswapd_wait;
    wait_queue_head_t pfmemalloc_wait;
    struct task_struct *kswapd;
    int kswapd_order;
    enum zone_type kswapd_classzone_idx;
    int kswapd_failures;
    int kcompactd_max_order;
    enum zone_type kcompactd_classzone_idx;
    wait_queue_head_t kcompactd_wait;
    struct task_struct *kcompactd;
    long unsigned int totalreserve_pages;
    struct zone_padding _pad1_;
    spinlock_t lru_lock;
    struct lruvec lruvec;
    long unsigned int flags;
    struct zone_padding _pad2_;
    struct per_cpu_nodestat *per_cpu_nodestats;
    atomic_long_t vm_stat[32];
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
struct pglist_data {
    struct zone node_zones[5];
    struct zonelist node_zonelists[2];
    int nr_zones;
    spinlock_t node_size_lock;
    long unsigned int node_start_pfn;
    long unsigned int node_present_pages;
    long unsigned int node_spanned_pages;
    int node_id;
    wait_queue_head_t kswapd_wait;
    wait_queue_head_t pfmemalloc_wait;
    struct task_struct *kswapd;
    int kswapd_order;
    enum zone_type kswapd_classzone_idx;
    int kswapd_failures;
    int kcompactd_max_order;
    enum zone_type kcompactd_classzone_idx;
    wait_queue_head_t kcompactd_wait;
    struct task_struct *kcompactd;
    long unsigned int totalreserve_pages;
    long unsigned int min_unmapped_pages;
    long unsigned int min_slab_pages;
    struct zone_padding _pad1_;
    spinlock_t lru_lock;
    struct deferred_split deferred_split_queue;
    struct lruvec lruvec;
    long unsigned int flags;
    struct zone_padding _pad2_;
    struct per_cpu_nodestat *per_cpu_nodestats;
    atomic_long_t vm_stat[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct pglist_data {
    struct zone node_zones[5];
    struct zonelist node_zonelists[2];
    int nr_zones;
    spinlock_t node_size_lock;
    long unsigned int node_start_pfn;
    long unsigned int node_present_pages;
    long unsigned int node_spanned_pages;
    int node_id;
    wait_queue_head_t kswapd_wait;
    wait_queue_head_t pfmemalloc_wait;
    struct task_struct *kswapd;
    int kswapd_order;
    enum zone_type kswapd_classzone_idx;
    int kswapd_failures;
    int kcompactd_max_order;
    enum zone_type kcompactd_classzone_idx;
    wait_queue_head_t kcompactd_wait;
    struct task_struct *kcompactd;
    long unsigned int totalreserve_pages;
    long unsigned int min_unmapped_pages;
    long unsigned int min_slab_pages;
    struct zone_padding _pad1_;
    spinlock_t lru_lock;
    struct deferred_split deferred_split_queue;
    struct lruvec lruvec;
    long unsigned int flags;
    struct zone_padding _pad2_;
    struct per_cpu_nodestat *per_cpu_nodestats;
    atomic_long_t vm_stat[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct pglist_data {
    struct zone node_zones[5];
    struct zonelist node_zonelists[2];
    int nr_zones;
    spinlock_t node_size_lock;
    long unsigned int node_start_pfn;
    long unsigned int node_present_pages;
    long unsigned int node_spanned_pages;
    int node_id;
    wait_queue_head_t kswapd_wait;
    wait_queue_head_t pfmemalloc_wait;
    struct task_struct *kswapd;
    int kswapd_order;
    enum zone_type kswapd_classzone_idx;
    int kswapd_failures;
    int kcompactd_max_order;
    enum zone_type kcompactd_classzone_idx;
    wait_queue_head_t kcompactd_wait;
    struct task_struct *kcompactd;
    long unsigned int totalreserve_pages;
    long unsigned int min_unmapped_pages;
    long unsigned int min_slab_pages;
    struct zone_padding _pad1_;
    spinlock_t lru_lock;
    struct deferred_split deferred_split_queue;
    struct lruvec lruvec;
    long unsigned int flags;
    struct zone_padding _pad2_;
    struct per_cpu_nodestat *per_cpu_nodestats;
    atomic_long_t vm_stat[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct pglist_data {
    struct zone node_zones[5];
    struct zonelist node_zonelists[2];
    int nr_zones;
    spinlock_t node_size_lock;
    long unsigned int node_start_pfn;
    long unsigned int node_present_pages;
    long unsigned int node_spanned_pages;
    int node_id;
    wait_queue_head_t kswapd_wait;
    wait_queue_head_t pfmemalloc_wait;
    struct task_struct *kswapd;
    int kswapd_order;
    enum zone_type kswapd_classzone_idx;
    int kswapd_failures;
    int kcompactd_max_order;
    enum zone_type kcompactd_classzone_idx;
    wait_queue_head_t kcompactd_wait;
    struct task_struct *kcompactd;
    long unsigned int totalreserve_pages;
    long unsigned int min_unmapped_pages;
    long unsigned int min_slab_pages;
    struct zone_padding _pad1_;
    spinlock_t lru_lock;
    struct deferred_split deferred_split_queue;
    struct lruvec lruvec;
    long unsigned int flags;
    struct zone_padding _pad2_;
    struct per_cpu_nodestat *per_cpu_nodestats;
    atomic_long_t vm_stat[32];
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
<code>int kswapd_order</code>
</li>
<li>
<b>Field added. </b>
<code>enum zone_type kswapd_classzone_idx</code>
</li>
<li>
<b>Field added. </b>
<code>int kcompactd_max_order</code>
</li>
<li>
<b>Field added. </b>
<code>enum zone_type kcompactd_classzone_idx</code>
</li>
<li>
<b>Field added. </b>
<code>wait_queue_head_t kcompactd_wait</code>
</li>
<li>
<b>Field added. </b>
<code>struct task_struct *kcompactd</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int totalreserve_pages</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int min_unmapped_pages</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int min_slab_pages</code>
</li>
<li>
<b>Field added. </b>
<code>struct zone_padding _pad1_</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t lru_lock</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t split_queue_lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head split_queue</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int split_queue_len</code>
</li>
<li>
<b>Field added. </b>
<code>struct lruvec lruvec</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int inactive_ratio</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int flags</code>
</li>
<li>
<b>Field added. </b>
<code>struct zone_padding _pad2_</code>
</li>
<li>
<b>Field added. </b>
<code>struct per_cpu_nodestat *per_cpu_nodestats</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t vm_stat[26]</code>
</li>
<li>
<b>Field removed. </b>
<code>int kswapd_max_order</code>
</li>
<li>
<b>Field removed. </b>
<code>enum zone_type classzone_idx</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int kswapd_failures</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t vm_stat[26]</code> ➡️ <code>atomic_long_t vm_stat[27]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned int inactive_ratio</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>atomic_long_t vm_stat[27]</code> ➡️ <code>atomic_long_t vm_stat[28]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>spinlock_t numabalancing_migrate_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int numabalancing_migrate_next_window</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int numabalancing_migrate_nr_pages</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t vm_stat[28]</code> ➡️ <code>atomic_long_t vm_stat[30]</code>
</li>
</ul>
</details>
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
<code>struct deferred_split deferred_split_queue</code>
</li>
<li>
<b>Field removed. </b>
<code>spinlock_t split_queue_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head split_queue</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int split_queue_len</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t vm_stat[30]</code> ➡️ <code>atomic_long_t vm_stat[32]</code>
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
<code>enum zone_type kswapd_highest_zoneidx</code>
</li>
<li>
<b>Field added. </b>
<code>enum zone_type kcompactd_highest_zoneidx</code>
</li>
<li>
<b>Field added. </b>
<code>struct lruvec __lruvec</code>
</li>
<li>
<b>Field removed. </b>
<code>enum zone_type kswapd_classzone_idx</code>
</li>
<li>
<b>Field removed. </b>
<code>enum zone_type kcompactd_classzone_idx</code>
</li>
<li>
<b>Field removed. </b>
<code>struct lruvec lruvec</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t vm_stat[32]</code> ➡️ <code>atomic_long_t vm_stat[33]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>spinlock_t lru_lock</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t vm_stat[33]</code> ➡️ <code>atomic_long_t vm_stat[38]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>atomic_long_t vm_stat[38]</code> ➡️ <code>atomic_long_t vm_stat[39]</code>
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
<code>bool proactive_compact_trigger</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>wait_queue_head_t reclaim_wait[4]</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t nr_writeback_throttled</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int nr_reclaim_start</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t vm_stat[39]</code> ➡️ <code>atomic_long_t vm_stat[41]</code>
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
<code>struct mutex kswapd_lock</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int nbp_rl_start</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int nbp_rl_nr_cand</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int nbp_threshold</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int nbp_th_start</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int nbp_th_nr_cand</code>
</li>
<li>
<b>Field added. </b>
<code>struct lru_gen_mm_walk mm_walk</code>
</li>
<li>
<b>Field added. </b>
<code>struct memory_tier *memtier</code>
</li>
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
<code>atomic_long_t vm_stat[41]</code> ➡️ <code>atomic_long_t vm_stat[43]</code>
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
<code>struct lru_gen_memcg memcg_lru</code>
</li>
<li>
<b>Field added. </b>
<code>struct memory_failure_stats mf_stats</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>atomic_long_t vm_stat[43]</code> ➡️ <code>atomic_long_t vm_stat[46]</code>
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
<code>struct zone node_zones[5]</code> ➡️ <code>struct zone node_zones[3]</code>
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
<code>struct page *node_mem_map</code>
</li>
<li>
<b>Field added. </b>
<code>struct page_ext *node_page_ext</code>
</li>
<li>
<b>Field removed. </b>
<code>spinlock_t node_size_lock</code>
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
<code>struct deferred_split deferred_split_queue</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct zone node_zones[5]</code> ➡️ <code>struct zone node_zones[3]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct zonelist node_zonelists[2]</code> ➡️ <code>struct zonelist node_zonelists[1]</code>
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
<code>struct zone node_zones[5]</code> ➡️ <code>struct zone node_zones[3]</code>
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
<code>spinlock_t node_size_lock</code>
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
<code>struct deferred_split deferred_split_queue</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct zone node_zones[5]</code> ➡️ <code>struct zone node_zones[3]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct zonelist node_zonelists[2]</code> ➡️ <code>struct zonelist node_zonelists[1]</code>
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
