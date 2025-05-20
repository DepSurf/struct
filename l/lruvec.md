# Struct: <code>lruvec</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct lruvec {
    struct list_head lists[5];
    struct zone_reclaim_stat reclaim_stat;
    struct zone *zone;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct lruvec {
    struct list_head lists[5];
    struct zone_reclaim_stat reclaim_stat;
    atomic_long_t inactive_age;
    struct pglist_data *pgdat;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct lruvec {
    struct list_head lists[5];
    struct zone_reclaim_stat reclaim_stat;
    atomic_long_t inactive_age;
    struct pglist_data *pgdat;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct lruvec {
    struct list_head lists[5];
    struct zone_reclaim_stat reclaim_stat;
    atomic_long_t inactive_age;
    long unsigned int refaults;
    struct pglist_data *pgdat;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct lruvec {
    struct list_head lists[5];
    struct zone_reclaim_stat reclaim_stat;
    atomic_long_t inactive_age;
    long unsigned int refaults;
    struct pglist_data *pgdat;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct lruvec {
    struct list_head lists[5];
    struct zone_reclaim_stat reclaim_stat;
    atomic_long_t inactive_age;
    long unsigned int refaults;
    struct pglist_data *pgdat;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct lruvec {
    struct list_head lists[5];
    struct zone_reclaim_stat reclaim_stat;
    atomic_long_t inactive_age;
    long unsigned int refaults;
    struct pglist_data *pgdat;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct lruvec {
    struct list_head lists[5];
    struct zone_reclaim_stat reclaim_stat;
    atomic_long_t inactive_age;
    long unsigned int refaults;
    struct pglist_data *pgdat;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct lruvec {
    struct list_head lists[5];
    struct zone_reclaim_stat reclaim_stat;
    atomic_long_t inactive_age;
    long unsigned int refaults;
    struct pglist_data *pgdat;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct lruvec {
    struct list_head lists[5];
    long unsigned int anon_cost;
    long unsigned int file_cost;
    atomic_long_t nonresident_age;
    long unsigned int refaults;
    long unsigned int flags;
    struct pglist_data *pgdat;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct lruvec {
    struct list_head lists[5];
    spinlock_t lru_lock;
    long unsigned int anon_cost;
    long unsigned int file_cost;
    atomic_long_t nonresident_age;
    long unsigned int refaults[2];
    long unsigned int flags;
    struct pglist_data *pgdat;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct lruvec {
    struct list_head lists[5];
    spinlock_t lru_lock;
    long unsigned int anon_cost;
    long unsigned int file_cost;
    atomic_long_t nonresident_age;
    long unsigned int refaults[2];
    long unsigned int flags;
    struct pglist_data *pgdat;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct lruvec {
    struct list_head lists[5];
    spinlock_t lru_lock;
    long unsigned int anon_cost;
    long unsigned int file_cost;
    atomic_long_t nonresident_age;
    long unsigned int refaults[2];
    long unsigned int flags;
    struct pglist_data *pgdat;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct lruvec {
    struct list_head lists[5];
    spinlock_t lru_lock;
    long unsigned int anon_cost;
    long unsigned int file_cost;
    atomic_long_t nonresident_age;
    long unsigned int refaults[2];
    long unsigned int flags;
    struct pglist_data *pgdat;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct lruvec {
    struct list_head lists[5];
    spinlock_t lru_lock;
    long unsigned int anon_cost;
    long unsigned int file_cost;
    atomic_long_t nonresident_age;
    long unsigned int refaults[2];
    long unsigned int flags;
    struct lru_gen_struct lrugen;
    struct lru_gen_mm_state mm_state;
    struct pglist_data *pgdat;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct lruvec {
    struct list_head lists[5];
    spinlock_t lru_lock;
    long unsigned int anon_cost;
    long unsigned int file_cost;
    atomic_long_t nonresident_age;
    long unsigned int refaults[2];
    long unsigned int flags;
    struct lru_gen_folio lrugen;
    struct lru_gen_mm_state mm_state;
    struct pglist_data *pgdat;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct lruvec {
    struct list_head lists[5];
    spinlock_t lru_lock;
    long unsigned int anon_cost;
    long unsigned int file_cost;
    atomic_long_t nonresident_age;
    long unsigned int refaults[2];
    long unsigned int flags;
    struct lru_gen_folio lrugen;
    struct lru_gen_mm_state mm_state;
    struct pglist_data *pgdat;
    struct zswap_lruvec_state zswap_lruvec_state;
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
struct lruvec {
    struct list_head lists[5];
    struct zone_reclaim_stat reclaim_stat;
    atomic_long_t inactive_age;
    long unsigned int refaults;
    struct pglist_data *pgdat;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct lruvec {
    struct list_head lists[5];
    struct zone_reclaim_stat reclaim_stat;
    atomic_long_t inactive_age;
    long unsigned int refaults;
    struct pglist_data *pgdat;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct lruvec {
    struct list_head lists[5];
    struct zone_reclaim_stat reclaim_stat;
    atomic_long_t inactive_age;
    long unsigned int refaults;
    struct pglist_data *pgdat;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct lruvec {
    struct list_head lists[5];
    struct zone_reclaim_stat reclaim_stat;
    atomic_long_t inactive_age;
    long unsigned int refaults;
    struct pglist_data *pgdat;
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
struct lruvec {
    struct list_head lists[5];
    struct zone_reclaim_stat reclaim_stat;
    atomic_long_t inactive_age;
    long unsigned int refaults;
    struct pglist_data *pgdat;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct lruvec {
    struct list_head lists[5];
    struct zone_reclaim_stat reclaim_stat;
    atomic_long_t inactive_age;
    long unsigned int refaults;
    struct pglist_data *pgdat;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct lruvec {
    struct list_head lists[5];
    struct zone_reclaim_stat reclaim_stat;
    atomic_long_t inactive_age;
    long unsigned int refaults;
    struct pglist_data *pgdat;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct lruvec {
    struct list_head lists[5];
    struct zone_reclaim_stat reclaim_stat;
    atomic_long_t inactive_age;
    long unsigned int refaults;
    struct pglist_data *pgdat;
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
<code>atomic_long_t inactive_age</code>
</li>
<li>
<b>Field added. </b>
<code>struct pglist_data *pgdat</code>
</li>
<li>
<b>Field removed. </b>
<code>struct zone *zone</code>
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
<code>long unsigned int refaults</code>
</li>
</ul>
</details>
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
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int anon_cost</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int file_cost</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t nonresident_age</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int flags</code>
</li>
<li>
<b>Field removed. </b>
<code>struct zone_reclaim_stat reclaim_stat</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_long_t inactive_age</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>spinlock_t lru_lock</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int refaults</code> ➡️ <code>long unsigned int refaults[2]</code>
</li>
</ul>
</details>
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
<code>struct lru_gen_struct lrugen</code>
</li>
<li>
<b>Field added. </b>
<code>struct lru_gen_mm_state mm_state</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct lru_gen_struct lrugen</code> ➡️ <code>struct lru_gen_folio lrugen</code>
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
<code>struct zswap_lruvec_state zswap_lruvec_state</code>
</li>
</ul>
</details>
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
