# Struct: <code>blkcg_policy</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct blkcg_policy {
    int plid;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    blkcg_pol_alloc_cpd_fn *cpd_alloc_fn;
    blkcg_pol_init_cpd_fn *cpd_init_fn;
    blkcg_pol_free_cpd_fn *cpd_free_fn;
    blkcg_pol_bind_cpd_fn *cpd_bind_fn;
    blkcg_pol_alloc_pd_fn *pd_alloc_fn;
    blkcg_pol_init_pd_fn *pd_init_fn;
    blkcg_pol_online_pd_fn *pd_online_fn;
    blkcg_pol_offline_pd_fn *pd_offline_fn;
    blkcg_pol_free_pd_fn *pd_free_fn;
    blkcg_pol_reset_pd_stats_fn *pd_reset_stats_fn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct blkcg_policy {
    int plid;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    blkcg_pol_alloc_cpd_fn *cpd_alloc_fn;
    blkcg_pol_init_cpd_fn *cpd_init_fn;
    blkcg_pol_free_cpd_fn *cpd_free_fn;
    blkcg_pol_bind_cpd_fn *cpd_bind_fn;
    blkcg_pol_alloc_pd_fn *pd_alloc_fn;
    blkcg_pol_init_pd_fn *pd_init_fn;
    blkcg_pol_online_pd_fn *pd_online_fn;
    blkcg_pol_offline_pd_fn *pd_offline_fn;
    blkcg_pol_free_pd_fn *pd_free_fn;
    blkcg_pol_reset_pd_stats_fn *pd_reset_stats_fn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct blkcg_policy {
    int plid;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    blkcg_pol_alloc_cpd_fn *cpd_alloc_fn;
    blkcg_pol_init_cpd_fn *cpd_init_fn;
    blkcg_pol_free_cpd_fn *cpd_free_fn;
    blkcg_pol_bind_cpd_fn *cpd_bind_fn;
    blkcg_pol_alloc_pd_fn *pd_alloc_fn;
    blkcg_pol_init_pd_fn *pd_init_fn;
    blkcg_pol_online_pd_fn *pd_online_fn;
    blkcg_pol_offline_pd_fn *pd_offline_fn;
    blkcg_pol_free_pd_fn *pd_free_fn;
    blkcg_pol_reset_pd_stats_fn *pd_reset_stats_fn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct blkcg_policy {
    int plid;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    blkcg_pol_alloc_cpd_fn *cpd_alloc_fn;
    blkcg_pol_init_cpd_fn *cpd_init_fn;
    blkcg_pol_free_cpd_fn *cpd_free_fn;
    blkcg_pol_bind_cpd_fn *cpd_bind_fn;
    blkcg_pol_alloc_pd_fn *pd_alloc_fn;
    blkcg_pol_init_pd_fn *pd_init_fn;
    blkcg_pol_online_pd_fn *pd_online_fn;
    blkcg_pol_offline_pd_fn *pd_offline_fn;
    blkcg_pol_free_pd_fn *pd_free_fn;
    blkcg_pol_reset_pd_stats_fn *pd_reset_stats_fn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct blkcg_policy {
    int plid;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    blkcg_pol_alloc_cpd_fn *cpd_alloc_fn;
    blkcg_pol_init_cpd_fn *cpd_init_fn;
    blkcg_pol_free_cpd_fn *cpd_free_fn;
    blkcg_pol_bind_cpd_fn *cpd_bind_fn;
    blkcg_pol_alloc_pd_fn *pd_alloc_fn;
    blkcg_pol_init_pd_fn *pd_init_fn;
    blkcg_pol_online_pd_fn *pd_online_fn;
    blkcg_pol_offline_pd_fn *pd_offline_fn;
    blkcg_pol_free_pd_fn *pd_free_fn;
    blkcg_pol_reset_pd_stats_fn *pd_reset_stats_fn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct blkcg_policy {
    int plid;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    blkcg_pol_alloc_cpd_fn *cpd_alloc_fn;
    blkcg_pol_init_cpd_fn *cpd_init_fn;
    blkcg_pol_free_cpd_fn *cpd_free_fn;
    blkcg_pol_bind_cpd_fn *cpd_bind_fn;
    blkcg_pol_alloc_pd_fn *pd_alloc_fn;
    blkcg_pol_init_pd_fn *pd_init_fn;
    blkcg_pol_online_pd_fn *pd_online_fn;
    blkcg_pol_offline_pd_fn *pd_offline_fn;
    blkcg_pol_free_pd_fn *pd_free_fn;
    blkcg_pol_reset_pd_stats_fn *pd_reset_stats_fn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct blkcg_policy {
    int plid;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    blkcg_pol_alloc_cpd_fn *cpd_alloc_fn;
    blkcg_pol_init_cpd_fn *cpd_init_fn;
    blkcg_pol_free_cpd_fn *cpd_free_fn;
    blkcg_pol_bind_cpd_fn *cpd_bind_fn;
    blkcg_pol_alloc_pd_fn *pd_alloc_fn;
    blkcg_pol_init_pd_fn *pd_init_fn;
    blkcg_pol_online_pd_fn *pd_online_fn;
    blkcg_pol_offline_pd_fn *pd_offline_fn;
    blkcg_pol_free_pd_fn *pd_free_fn;
    blkcg_pol_reset_pd_stats_fn *pd_reset_stats_fn;
    blkcg_pol_stat_pd_fn *pd_stat_fn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct blkcg_policy {
    int plid;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    blkcg_pol_alloc_cpd_fn *cpd_alloc_fn;
    blkcg_pol_init_cpd_fn *cpd_init_fn;
    blkcg_pol_free_cpd_fn *cpd_free_fn;
    blkcg_pol_bind_cpd_fn *cpd_bind_fn;
    blkcg_pol_alloc_pd_fn *pd_alloc_fn;
    blkcg_pol_init_pd_fn *pd_init_fn;
    blkcg_pol_online_pd_fn *pd_online_fn;
    blkcg_pol_offline_pd_fn *pd_offline_fn;
    blkcg_pol_free_pd_fn *pd_free_fn;
    blkcg_pol_reset_pd_stats_fn *pd_reset_stats_fn;
    blkcg_pol_stat_pd_fn *pd_stat_fn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct blkcg_policy {
    int plid;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    blkcg_pol_alloc_cpd_fn *cpd_alloc_fn;
    blkcg_pol_init_cpd_fn *cpd_init_fn;
    blkcg_pol_free_cpd_fn *cpd_free_fn;
    blkcg_pol_bind_cpd_fn *cpd_bind_fn;
    blkcg_pol_alloc_pd_fn *pd_alloc_fn;
    blkcg_pol_init_pd_fn *pd_init_fn;
    blkcg_pol_online_pd_fn *pd_online_fn;
    blkcg_pol_offline_pd_fn *pd_offline_fn;
    blkcg_pol_free_pd_fn *pd_free_fn;
    blkcg_pol_reset_pd_stats_fn *pd_reset_stats_fn;
    blkcg_pol_stat_pd_fn *pd_stat_fn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct blkcg_policy {
    int plid;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    blkcg_pol_alloc_cpd_fn *cpd_alloc_fn;
    blkcg_pol_init_cpd_fn *cpd_init_fn;
    blkcg_pol_free_cpd_fn *cpd_free_fn;
    blkcg_pol_bind_cpd_fn *cpd_bind_fn;
    blkcg_pol_alloc_pd_fn *pd_alloc_fn;
    blkcg_pol_init_pd_fn *pd_init_fn;
    blkcg_pol_online_pd_fn *pd_online_fn;
    blkcg_pol_offline_pd_fn *pd_offline_fn;
    blkcg_pol_free_pd_fn *pd_free_fn;
    blkcg_pol_reset_pd_stats_fn *pd_reset_stats_fn;
    blkcg_pol_stat_pd_fn *pd_stat_fn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct blkcg_policy {
    int plid;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    blkcg_pol_alloc_cpd_fn *cpd_alloc_fn;
    blkcg_pol_init_cpd_fn *cpd_init_fn;
    blkcg_pol_free_cpd_fn *cpd_free_fn;
    blkcg_pol_bind_cpd_fn *cpd_bind_fn;
    blkcg_pol_alloc_pd_fn *pd_alloc_fn;
    blkcg_pol_init_pd_fn *pd_init_fn;
    blkcg_pol_online_pd_fn *pd_online_fn;
    blkcg_pol_offline_pd_fn *pd_offline_fn;
    blkcg_pol_free_pd_fn *pd_free_fn;
    blkcg_pol_reset_pd_stats_fn *pd_reset_stats_fn;
    blkcg_pol_stat_pd_fn *pd_stat_fn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct blkcg_policy {
    int plid;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    blkcg_pol_alloc_cpd_fn *cpd_alloc_fn;
    blkcg_pol_init_cpd_fn *cpd_init_fn;
    blkcg_pol_free_cpd_fn *cpd_free_fn;
    blkcg_pol_bind_cpd_fn *cpd_bind_fn;
    blkcg_pol_alloc_pd_fn *pd_alloc_fn;
    blkcg_pol_init_pd_fn *pd_init_fn;
    blkcg_pol_online_pd_fn *pd_online_fn;
    blkcg_pol_offline_pd_fn *pd_offline_fn;
    blkcg_pol_free_pd_fn *pd_free_fn;
    blkcg_pol_reset_pd_stats_fn *pd_reset_stats_fn;
    blkcg_pol_stat_pd_fn *pd_stat_fn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct blkcg_policy {
    int plid;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    blkcg_pol_alloc_cpd_fn *cpd_alloc_fn;
    blkcg_pol_init_cpd_fn *cpd_init_fn;
    blkcg_pol_free_cpd_fn *cpd_free_fn;
    blkcg_pol_bind_cpd_fn *cpd_bind_fn;
    blkcg_pol_alloc_pd_fn *pd_alloc_fn;
    blkcg_pol_init_pd_fn *pd_init_fn;
    blkcg_pol_online_pd_fn *pd_online_fn;
    blkcg_pol_offline_pd_fn *pd_offline_fn;
    blkcg_pol_free_pd_fn *pd_free_fn;
    blkcg_pol_reset_pd_stats_fn *pd_reset_stats_fn;
    blkcg_pol_stat_pd_fn *pd_stat_fn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct blkcg_policy {
    int plid;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    blkcg_pol_alloc_cpd_fn *cpd_alloc_fn;
    blkcg_pol_init_cpd_fn *cpd_init_fn;
    blkcg_pol_free_cpd_fn *cpd_free_fn;
    blkcg_pol_bind_cpd_fn *cpd_bind_fn;
    blkcg_pol_alloc_pd_fn *pd_alloc_fn;
    blkcg_pol_init_pd_fn *pd_init_fn;
    blkcg_pol_online_pd_fn *pd_online_fn;
    blkcg_pol_offline_pd_fn *pd_offline_fn;
    blkcg_pol_free_pd_fn *pd_free_fn;
    blkcg_pol_reset_pd_stats_fn *pd_reset_stats_fn;
    blkcg_pol_stat_pd_fn *pd_stat_fn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct blkcg_policy {
    int plid;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    blkcg_pol_alloc_cpd_fn *cpd_alloc_fn;
    blkcg_pol_init_cpd_fn *cpd_init_fn;
    blkcg_pol_free_cpd_fn *cpd_free_fn;
    blkcg_pol_bind_cpd_fn *cpd_bind_fn;
    blkcg_pol_alloc_pd_fn *pd_alloc_fn;
    blkcg_pol_init_pd_fn *pd_init_fn;
    blkcg_pol_online_pd_fn *pd_online_fn;
    blkcg_pol_offline_pd_fn *pd_offline_fn;
    blkcg_pol_free_pd_fn *pd_free_fn;
    blkcg_pol_reset_pd_stats_fn *pd_reset_stats_fn;
    blkcg_pol_stat_pd_fn *pd_stat_fn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct blkcg_policy {
    int plid;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    blkcg_pol_alloc_cpd_fn *cpd_alloc_fn;
    blkcg_pol_free_cpd_fn *cpd_free_fn;
    blkcg_pol_alloc_pd_fn *pd_alloc_fn;
    blkcg_pol_init_pd_fn *pd_init_fn;
    blkcg_pol_online_pd_fn *pd_online_fn;
    blkcg_pol_offline_pd_fn *pd_offline_fn;
    blkcg_pol_free_pd_fn *pd_free_fn;
    blkcg_pol_reset_pd_stats_fn *pd_reset_stats_fn;
    blkcg_pol_stat_pd_fn *pd_stat_fn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct blkcg_policy {
    int plid;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    blkcg_pol_alloc_cpd_fn *cpd_alloc_fn;
    blkcg_pol_free_cpd_fn *cpd_free_fn;
    blkcg_pol_alloc_pd_fn *pd_alloc_fn;
    blkcg_pol_init_pd_fn *pd_init_fn;
    blkcg_pol_online_pd_fn *pd_online_fn;
    blkcg_pol_offline_pd_fn *pd_offline_fn;
    blkcg_pol_free_pd_fn *pd_free_fn;
    blkcg_pol_reset_pd_stats_fn *pd_reset_stats_fn;
    blkcg_pol_stat_pd_fn *pd_stat_fn;
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
struct blkcg_policy {
    int plid;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    blkcg_pol_alloc_cpd_fn *cpd_alloc_fn;
    blkcg_pol_init_cpd_fn *cpd_init_fn;
    blkcg_pol_free_cpd_fn *cpd_free_fn;
    blkcg_pol_bind_cpd_fn *cpd_bind_fn;
    blkcg_pol_alloc_pd_fn *pd_alloc_fn;
    blkcg_pol_init_pd_fn *pd_init_fn;
    blkcg_pol_online_pd_fn *pd_online_fn;
    blkcg_pol_offline_pd_fn *pd_offline_fn;
    blkcg_pol_free_pd_fn *pd_free_fn;
    blkcg_pol_reset_pd_stats_fn *pd_reset_stats_fn;
    blkcg_pol_stat_pd_fn *pd_stat_fn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct blkcg_policy {
    int plid;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    blkcg_pol_alloc_cpd_fn *cpd_alloc_fn;
    blkcg_pol_init_cpd_fn *cpd_init_fn;
    blkcg_pol_free_cpd_fn *cpd_free_fn;
    blkcg_pol_bind_cpd_fn *cpd_bind_fn;
    blkcg_pol_alloc_pd_fn *pd_alloc_fn;
    blkcg_pol_init_pd_fn *pd_init_fn;
    blkcg_pol_online_pd_fn *pd_online_fn;
    blkcg_pol_offline_pd_fn *pd_offline_fn;
    blkcg_pol_free_pd_fn *pd_free_fn;
    blkcg_pol_reset_pd_stats_fn *pd_reset_stats_fn;
    blkcg_pol_stat_pd_fn *pd_stat_fn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct blkcg_policy {
    int plid;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    blkcg_pol_alloc_cpd_fn *cpd_alloc_fn;
    blkcg_pol_init_cpd_fn *cpd_init_fn;
    blkcg_pol_free_cpd_fn *cpd_free_fn;
    blkcg_pol_bind_cpd_fn *cpd_bind_fn;
    blkcg_pol_alloc_pd_fn *pd_alloc_fn;
    blkcg_pol_init_pd_fn *pd_init_fn;
    blkcg_pol_online_pd_fn *pd_online_fn;
    blkcg_pol_offline_pd_fn *pd_offline_fn;
    blkcg_pol_free_pd_fn *pd_free_fn;
    blkcg_pol_reset_pd_stats_fn *pd_reset_stats_fn;
    blkcg_pol_stat_pd_fn *pd_stat_fn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct blkcg_policy {
    int plid;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    blkcg_pol_alloc_cpd_fn *cpd_alloc_fn;
    blkcg_pol_init_cpd_fn *cpd_init_fn;
    blkcg_pol_free_cpd_fn *cpd_free_fn;
    blkcg_pol_bind_cpd_fn *cpd_bind_fn;
    blkcg_pol_alloc_pd_fn *pd_alloc_fn;
    blkcg_pol_init_pd_fn *pd_init_fn;
    blkcg_pol_online_pd_fn *pd_online_fn;
    blkcg_pol_offline_pd_fn *pd_offline_fn;
    blkcg_pol_free_pd_fn *pd_free_fn;
    blkcg_pol_reset_pd_stats_fn *pd_reset_stats_fn;
    blkcg_pol_stat_pd_fn *pd_stat_fn;
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
struct blkcg_policy {
    int plid;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    blkcg_pol_alloc_cpd_fn *cpd_alloc_fn;
    blkcg_pol_init_cpd_fn *cpd_init_fn;
    blkcg_pol_free_cpd_fn *cpd_free_fn;
    blkcg_pol_bind_cpd_fn *cpd_bind_fn;
    blkcg_pol_alloc_pd_fn *pd_alloc_fn;
    blkcg_pol_init_pd_fn *pd_init_fn;
    blkcg_pol_online_pd_fn *pd_online_fn;
    blkcg_pol_offline_pd_fn *pd_offline_fn;
    blkcg_pol_free_pd_fn *pd_free_fn;
    blkcg_pol_reset_pd_stats_fn *pd_reset_stats_fn;
    blkcg_pol_stat_pd_fn *pd_stat_fn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct blkcg_policy {
    int plid;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    blkcg_pol_alloc_cpd_fn *cpd_alloc_fn;
    blkcg_pol_init_cpd_fn *cpd_init_fn;
    blkcg_pol_free_cpd_fn *cpd_free_fn;
    blkcg_pol_bind_cpd_fn *cpd_bind_fn;
    blkcg_pol_alloc_pd_fn *pd_alloc_fn;
    blkcg_pol_init_pd_fn *pd_init_fn;
    blkcg_pol_online_pd_fn *pd_online_fn;
    blkcg_pol_offline_pd_fn *pd_offline_fn;
    blkcg_pol_free_pd_fn *pd_free_fn;
    blkcg_pol_reset_pd_stats_fn *pd_reset_stats_fn;
    blkcg_pol_stat_pd_fn *pd_stat_fn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct blkcg_policy {
    int plid;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    blkcg_pol_alloc_cpd_fn *cpd_alloc_fn;
    blkcg_pol_init_cpd_fn *cpd_init_fn;
    blkcg_pol_free_cpd_fn *cpd_free_fn;
    blkcg_pol_bind_cpd_fn *cpd_bind_fn;
    blkcg_pol_alloc_pd_fn *pd_alloc_fn;
    blkcg_pol_init_pd_fn *pd_init_fn;
    blkcg_pol_online_pd_fn *pd_online_fn;
    blkcg_pol_offline_pd_fn *pd_offline_fn;
    blkcg_pol_free_pd_fn *pd_free_fn;
    blkcg_pol_reset_pd_stats_fn *pd_reset_stats_fn;
    blkcg_pol_stat_pd_fn *pd_stat_fn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct blkcg_policy {
    int plid;
    struct cftype *dfl_cftypes;
    struct cftype *legacy_cftypes;
    blkcg_pol_alloc_cpd_fn *cpd_alloc_fn;
    blkcg_pol_init_cpd_fn *cpd_init_fn;
    blkcg_pol_free_cpd_fn *cpd_free_fn;
    blkcg_pol_bind_cpd_fn *cpd_bind_fn;
    blkcg_pol_alloc_pd_fn *pd_alloc_fn;
    blkcg_pol_init_pd_fn *pd_init_fn;
    blkcg_pol_online_pd_fn *pd_online_fn;
    blkcg_pol_offline_pd_fn *pd_offline_fn;
    blkcg_pol_free_pd_fn *pd_free_fn;
    blkcg_pol_reset_pd_stats_fn *pd_reset_stats_fn;
    blkcg_pol_stat_pd_fn *pd_stat_fn;
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
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>blkcg_pol_stat_pd_fn *pd_stat_fn</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>blkcg_pol_init_cpd_fn *cpd_init_fn</code>
</li>
<li>
<b>Field removed. </b>
<code>blkcg_pol_bind_cpd_fn *cpd_bind_fn</code>
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
