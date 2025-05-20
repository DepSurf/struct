# Struct: <code>mem_cgroup_per_node</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct mem_cgroup_per_node {
    struct mem_cgroup_per_zone zoneinfo[5];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct mem_cgroup_per_node {
    struct lruvec lruvec;
    long unsigned int lru_size[5];
    struct mem_cgroup_reclaim_iter iter[13];
    struct rb_node tree_node;
    long unsigned int usage_in_excess;
    bool on_tree;
    struct mem_cgroup *memcg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct mem_cgroup_per_node {
    struct lruvec lruvec;
    long unsigned int lru_zone_size[25];
    struct mem_cgroup_reclaim_iter iter[13];
    struct rb_node tree_node;
    long unsigned int usage_in_excess;
    bool on_tree;
    struct mem_cgroup *memcg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct mem_cgroup_per_node {
    struct lruvec lruvec;
    struct lruvec_stat *lruvec_stat;
    long unsigned int lru_zone_size[25];
    struct mem_cgroup_reclaim_iter iter[13];
    struct rb_node tree_node;
    long unsigned int usage_in_excess;
    bool on_tree;
    struct mem_cgroup *memcg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct mem_cgroup_per_node {
    struct lruvec lruvec;
    struct lruvec_stat *lruvec_stat;
    long unsigned int lru_zone_size[25];
    struct mem_cgroup_reclaim_iter iter[13];
    struct rb_node tree_node;
    long unsigned int usage_in_excess;
    bool on_tree;
    struct mem_cgroup *memcg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct mem_cgroup_per_node {
    struct lruvec lruvec;
    struct lruvec_stat *lruvec_stat_cpu;
    atomic_long_t lruvec_stat[28];
    long unsigned int lru_zone_size[25];
    struct mem_cgroup_reclaim_iter iter[13];
    struct rb_node tree_node;
    long unsigned int usage_in_excess;
    bool on_tree;
    bool congested;
    struct mem_cgroup *memcg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct mem_cgroup_per_node {
    struct lruvec lruvec;
    struct lruvec_stat *lruvec_stat_cpu;
    atomic_long_t lruvec_stat[30];
    long unsigned int lru_zone_size[25];
    struct mem_cgroup_reclaim_iter iter[13];
    struct memcg_shrinker_map *shrinker_map;
    struct rb_node tree_node;
    long unsigned int usage_in_excess;
    bool on_tree;
    bool congested;
    struct mem_cgroup *memcg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct mem_cgroup_per_node {
    struct lruvec lruvec;
    struct lruvec_stat *lruvec_stat_local;
    struct lruvec_stat *lruvec_stat_cpu;
    atomic_long_t lruvec_stat[30];
    long unsigned int lru_zone_size[25];
    struct mem_cgroup_reclaim_iter iter[13];
    struct memcg_shrinker_map *shrinker_map;
    struct rb_node tree_node;
    long unsigned int usage_in_excess;
    bool on_tree;
    bool congested;
    struct mem_cgroup *memcg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct mem_cgroup_per_node {
    struct lruvec lruvec;
    struct lruvec_stat *lruvec_stat_local;
    struct lruvec_stat *lruvec_stat_cpu;
    atomic_long_t lruvec_stat[32];
    long unsigned int lru_zone_size[25];
    struct mem_cgroup_reclaim_iter iter[13];
    struct memcg_shrinker_map *shrinker_map;
    struct rb_node tree_node;
    long unsigned int usage_in_excess;
    bool on_tree;
    bool congested;
    struct mem_cgroup *memcg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct mem_cgroup_per_node {
    struct lruvec lruvec;
    struct lruvec_stat *lruvec_stat_local;
    struct lruvec_stat *lruvec_stat_cpu;
    atomic_long_t lruvec_stat[33];
    long unsigned int lru_zone_size[25];
    struct mem_cgroup_reclaim_iter iter;
    struct memcg_shrinker_map *shrinker_map;
    struct rb_node tree_node;
    long unsigned int usage_in_excess;
    bool on_tree;
    struct mem_cgroup *memcg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mem_cgroup_per_node {
    struct lruvec lruvec;
    struct lruvec_stat *lruvec_stat_local;
    struct lruvec_stat *lruvec_stat_cpu;
    atomic_long_t lruvec_stat[38];
    long unsigned int lru_zone_size[25];
    struct mem_cgroup_reclaim_iter iter;
    struct memcg_shrinker_map *shrinker_map;
    struct rb_node tree_node;
    long unsigned int usage_in_excess;
    bool on_tree;
    struct mem_cgroup *memcg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mem_cgroup_per_node {
    struct lruvec lruvec;
    struct lruvec_stat *lruvec_stat_local;
    struct batched_lruvec_stat *lruvec_stat_cpu;
    atomic_long_t lruvec_stat[39];
    long unsigned int lru_zone_size[25];
    struct mem_cgroup_reclaim_iter iter;
    struct shrinker_info *shrinker_info;
    struct rb_node tree_node;
    long unsigned int usage_in_excess;
    bool on_tree;
    struct mem_cgroup *memcg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mem_cgroup_per_node {
    struct lruvec lruvec;
    struct lruvec_stats_percpu *lruvec_stats_percpu;
    struct lruvec_stats lruvec_stats;
    long unsigned int lru_zone_size[25];
    struct mem_cgroup_reclaim_iter iter;
    struct shrinker_info *shrinker_info;
    struct rb_node tree_node;
    long unsigned int usage_in_excess;
    bool on_tree;
    struct mem_cgroup *memcg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mem_cgroup_per_node {
    struct lruvec lruvec;
    struct lruvec_stats_percpu *lruvec_stats_percpu;
    struct lruvec_stats lruvec_stats;
    long unsigned int lru_zone_size[25];
    struct mem_cgroup_reclaim_iter iter;
    struct shrinker_info *shrinker_info;
    struct rb_node tree_node;
    long unsigned int usage_in_excess;
    bool on_tree;
    struct mem_cgroup *memcg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mem_cgroup_per_node {
    struct lruvec lruvec;
    struct lruvec_stats_percpu *lruvec_stats_percpu;
    struct lruvec_stats lruvec_stats;
    long unsigned int lru_zone_size[25];
    struct mem_cgroup_reclaim_iter iter;
    struct shrinker_info *shrinker_info;
    struct rb_node tree_node;
    long unsigned int usage_in_excess;
    bool on_tree;
    struct mem_cgroup *memcg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mem_cgroup_per_node {
    struct lruvec lruvec;
    struct lruvec_stats_percpu *lruvec_stats_percpu;
    struct lruvec_stats lruvec_stats;
    long unsigned int lru_zone_size[25];
    struct mem_cgroup_reclaim_iter iter;
    struct shrinker_info *shrinker_info;
    struct rb_node tree_node;
    long unsigned int usage_in_excess;
    bool on_tree;
    struct mem_cgroup *memcg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mem_cgroup_per_node {
    struct lruvec lruvec;
    struct lruvec_stats_percpu *lruvec_stats_percpu;
    struct lruvec_stats lruvec_stats;
    long unsigned int lru_zone_size[25];
    struct mem_cgroup_reclaim_iter iter;
    struct shrinker_info *shrinker_info;
    struct rb_node tree_node;
    long unsigned int usage_in_excess;
    bool on_tree;
    struct mem_cgroup *memcg;
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
struct mem_cgroup_per_node {
    struct lruvec lruvec;
    struct lruvec_stat *lruvec_stat_local;
    struct lruvec_stat *lruvec_stat_cpu;
    atomic_long_t lruvec_stat[32];
    long unsigned int lru_zone_size[15];
    struct mem_cgroup_reclaim_iter iter[13];
    struct memcg_shrinker_map *shrinker_map;
    struct rb_node tree_node;
    long unsigned int usage_in_excess;
    bool on_tree;
    bool congested;
    struct mem_cgroup *memcg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mem_cgroup_per_node {
    struct lruvec lruvec;
    struct lruvec_stat *lruvec_stat_local;
    struct lruvec_stat *lruvec_stat_cpu;
    atomic_long_t lruvec_stat[32];
    long unsigned int lru_zone_size[15];
    struct mem_cgroup_reclaim_iter iter[13];
    struct memcg_shrinker_map *shrinker_map;
    struct rb_node tree_node;
    long unsigned int usage_in_excess;
    bool on_tree;
    bool congested;
    struct mem_cgroup *memcg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct mem_cgroup_per_node {
    struct lruvec lruvec;
    struct lruvec_stat *lruvec_stat_local;
    struct lruvec_stat *lruvec_stat_cpu;
    atomic_long_t lruvec_stat[32];
    long unsigned int lru_zone_size[15];
    struct mem_cgroup_reclaim_iter iter[13];
    struct memcg_shrinker_map *shrinker_map;
    struct rb_node tree_node;
    long unsigned int usage_in_excess;
    bool on_tree;
    bool congested;
    struct mem_cgroup *memcg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct mem_cgroup_per_node {
    struct lruvec lruvec;
    struct lruvec_stat *lruvec_stat_local;
    struct lruvec_stat *lruvec_stat_cpu;
    atomic_long_t lruvec_stat[32];
    long unsigned int lru_zone_size[15];
    struct mem_cgroup_reclaim_iter iter[13];
    struct memcg_shrinker_map *shrinker_map;
    struct rb_node tree_node;
    long unsigned int usage_in_excess;
    bool on_tree;
    bool congested;
    struct mem_cgroup *memcg;
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
struct mem_cgroup_per_node {
    struct lruvec lruvec;
    struct lruvec_stat *lruvec_stat_local;
    struct lruvec_stat *lruvec_stat_cpu;
    atomic_long_t lruvec_stat[32];
    long unsigned int lru_zone_size[25];
    struct mem_cgroup_reclaim_iter iter[13];
    struct memcg_shrinker_map *shrinker_map;
    struct rb_node tree_node;
    long unsigned int usage_in_excess;
    bool on_tree;
    bool congested;
    struct mem_cgroup *memcg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct mem_cgroup_per_node {
    struct lruvec lruvec;
    struct lruvec_stat *lruvec_stat_local;
    struct lruvec_stat *lruvec_stat_cpu;
    atomic_long_t lruvec_stat[32];
    long unsigned int lru_zone_size[25];
    struct mem_cgroup_reclaim_iter iter[13];
    struct memcg_shrinker_map *shrinker_map;
    struct rb_node tree_node;
    long unsigned int usage_in_excess;
    bool on_tree;
    bool congested;
    struct mem_cgroup *memcg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct mem_cgroup_per_node {
    struct lruvec lruvec;
    struct lruvec_stat *lruvec_stat_local;
    struct lruvec_stat *lruvec_stat_cpu;
    atomic_long_t lruvec_stat[32];
    long unsigned int lru_zone_size[25];
    struct mem_cgroup_reclaim_iter iter[13];
    struct memcg_shrinker_map *shrinker_map;
    struct rb_node tree_node;
    long unsigned int usage_in_excess;
    bool on_tree;
    bool congested;
    struct mem_cgroup *memcg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct mem_cgroup_per_node {
    struct lruvec lruvec;
    struct lruvec_stat *lruvec_stat_local;
    struct lruvec_stat *lruvec_stat_cpu;
    atomic_long_t lruvec_stat[32];
    long unsigned int lru_zone_size[25];
    struct mem_cgroup_reclaim_iter iter[13];
    struct memcg_shrinker_map *shrinker_map;
    struct rb_node tree_node;
    long unsigned int usage_in_excess;
    bool on_tree;
    bool congested;
    struct mem_cgroup *memcg;
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
<code>struct lruvec lruvec</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int lru_size[5]</code>
</li>
<li>
<b>Field added. </b>
<code>struct mem_cgroup_reclaim_iter iter[13]</code>
</li>
<li>
<b>Field added. </b>
<code>struct rb_node tree_node</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int usage_in_excess</code>
</li>
<li>
<b>Field added. </b>
<code>bool on_tree</code>
</li>
<li>
<b>Field added. </b>
<code>struct mem_cgroup *memcg</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mem_cgroup_per_zone zoneinfo[5]</code>
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
<code>long unsigned int lru_zone_size[25]</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int lru_size[5]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct lruvec_stat *lruvec_stat</code>
</li>
</ul>
</details>
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
<code>struct lruvec_stat *lruvec_stat_cpu</code>
</li>
<li>
<b>Field added. </b>
<code>bool congested</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct lruvec_stat *lruvec_stat</code> ➡️ <code>atomic_long_t lruvec_stat[28]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct memcg_shrinker_map *shrinker_map</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t lruvec_stat[28]</code> ➡️ <code>atomic_long_t lruvec_stat[30]</code>
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
<code>struct lruvec_stat *lruvec_stat_local</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>atomic_long_t lruvec_stat[30]</code> ➡️ <code>atomic_long_t lruvec_stat[32]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>bool congested</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t lruvec_stat[32]</code> ➡️ <code>atomic_long_t lruvec_stat[33]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct mem_cgroup_reclaim_iter iter[13]</code> ➡️ <code>struct mem_cgroup_reclaim_iter iter</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>atomic_long_t lruvec_stat[33]</code> ➡️ <code>atomic_long_t lruvec_stat[38]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct shrinker_info *shrinker_info</code>
</li>
<li>
<b>Field removed. </b>
<code>struct memcg_shrinker_map *shrinker_map</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct lruvec_stat *lruvec_stat_cpu</code> ➡️ <code>struct batched_lruvec_stat *lruvec_stat_cpu</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t lruvec_stat[38]</code> ➡️ <code>atomic_long_t lruvec_stat[39]</code>
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
<code>struct lruvec_stats_percpu *lruvec_stats_percpu</code>
</li>
<li>
<b>Field added. </b>
<code>struct lruvec_stats lruvec_stats</code>
</li>
<li>
<b>Field removed. </b>
<code>struct lruvec_stat *lruvec_stat_local</code>
</li>
<li>
<b>Field removed. </b>
<code>struct batched_lruvec_stat *lruvec_stat_cpu</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_long_t lruvec_stat[39]</code>
</li>
</ul>
</details>
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
<b>Field type changed. </b>
<code>long unsigned int lru_zone_size[25]</code> ➡️ <code>long unsigned int lru_zone_size[15]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long unsigned int lru_zone_size[25]</code> ➡️ <code>long unsigned int lru_zone_size[15]</code>
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
<code>long unsigned int lru_zone_size[25]</code> ➡️ <code>long unsigned int lru_zone_size[15]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long unsigned int lru_zone_size[25]</code> ➡️ <code>long unsigned int lru_zone_size[15]</code>
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
