# Struct: <code>netns_smc</code>

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
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct netns_smc {
    struct smc_stats *smc_stats;
    struct mutex mutex_fback_rsn;
    struct smc_stats_rsn *fback_rsn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct netns_smc {
    struct smc_stats *smc_stats;
    struct mutex mutex_fback_rsn;
    struct smc_stats_rsn *fback_rsn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct netns_smc {
    struct smc_stats *smc_stats;
    struct mutex mutex_fback_rsn;
    struct smc_stats_rsn *fback_rsn;
    bool limit_smc_hs;
    struct ctl_table_header *smc_hdr;
    unsigned int sysctl_autocorking_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct netns_smc {
    struct smc_stats *smc_stats;
    struct mutex mutex_fback_rsn;
    struct smc_stats_rsn *fback_rsn;
    bool limit_smc_hs;
    struct ctl_table_header *smc_hdr;
    unsigned int sysctl_autocorking_size;
    unsigned int sysctl_smcr_buf_type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct netns_smc {
    struct smc_stats *smc_stats;
    struct mutex mutex_fback_rsn;
    struct smc_stats_rsn *fback_rsn;
    bool limit_smc_hs;
    struct ctl_table_header *smc_hdr;
    unsigned int sysctl_autocorking_size;
    unsigned int sysctl_smcr_buf_type;
    int sysctl_smcr_testlink_time;
    int sysctl_wmem;
    int sysctl_rmem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct netns_smc {
    struct smc_stats *smc_stats;
    struct mutex mutex_fback_rsn;
    struct smc_stats_rsn *fback_rsn;
    bool limit_smc_hs;
    struct ctl_table_header *smc_hdr;
    unsigned int sysctl_autocorking_size;
    unsigned int sysctl_smcr_buf_type;
    int sysctl_smcr_testlink_time;
    int sysctl_wmem;
    int sysctl_rmem;
    int sysctl_max_links_per_lgr;
    int sysctl_max_conns_per_lgr;
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
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool limit_smc_hs</code>
</li>
<li>
<b>Field added. </b>
<code>struct ctl_table_header *smc_hdr</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int sysctl_autocorking_size</code>
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
<code>unsigned int sysctl_smcr_buf_type</code>
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
<code>int sysctl_smcr_testlink_time</code>
</li>
<li>
<b>Field added. </b>
<code>int sysctl_wmem</code>
</li>
<li>
<b>Field added. </b>
<code>int sysctl_rmem</code>
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
<code>int sysctl_max_links_per_lgr</code>
</li>
<li>
<b>Field added. </b>
<code>int sysctl_max_conns_per_lgr</code>
</li>
</ul>
</details>
</li>
</ul>
