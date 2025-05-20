# Struct: <code>mcinfo_logical_cpu</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct mcinfo_logical_cpu {
    uint32_t mc_cpunr;
    uint32_t mc_chipid;
    uint16_t mc_coreid;
    uint16_t mc_threadid;
    uint32_t mc_apicid;
    uint32_t mc_clusterid;
    uint32_t mc_ncores;
    uint32_t mc_ncores_active;
    uint32_t mc_nthreads;
    uint32_t mc_cpuid_level;
    uint32_t mc_family;
    uint32_t mc_vendor;
    uint32_t mc_model;
    uint32_t mc_step;
    char mc_vendorid[16];
    char mc_brandid[64];
    uint32_t mc_cpu_caps[7];
    uint32_t mc_cache_size;
    uint32_t mc_cache_alignment;
    uint32_t mc_nmsrvals;
    struct mcinfo_msr mc_msrvalues[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct mcinfo_logical_cpu {
    uint32_t mc_cpunr;
    uint32_t mc_chipid;
    uint16_t mc_coreid;
    uint16_t mc_threadid;
    uint32_t mc_apicid;
    uint32_t mc_clusterid;
    uint32_t mc_ncores;
    uint32_t mc_ncores_active;
    uint32_t mc_nthreads;
    uint32_t mc_cpuid_level;
    uint32_t mc_family;
    uint32_t mc_vendor;
    uint32_t mc_model;
    uint32_t mc_step;
    char mc_vendorid[16];
    char mc_brandid[64];
    uint32_t mc_cpu_caps[7];
    uint32_t mc_cache_size;
    uint32_t mc_cache_alignment;
    uint32_t mc_nmsrvals;
    struct mcinfo_msr mc_msrvalues[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct mcinfo_logical_cpu {
    uint32_t mc_cpunr;
    uint32_t mc_chipid;
    uint16_t mc_coreid;
    uint16_t mc_threadid;
    uint32_t mc_apicid;
    uint32_t mc_clusterid;
    uint32_t mc_ncores;
    uint32_t mc_ncores_active;
    uint32_t mc_nthreads;
    uint32_t mc_cpuid_level;
    uint32_t mc_family;
    uint32_t mc_vendor;
    uint32_t mc_model;
    uint32_t mc_step;
    char mc_vendorid[16];
    char mc_brandid[64];
    uint32_t mc_cpu_caps[7];
    uint32_t mc_cache_size;
    uint32_t mc_cache_alignment;
    uint32_t mc_nmsrvals;
    struct mcinfo_msr mc_msrvalues[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct mcinfo_logical_cpu {
    uint32_t mc_cpunr;
    uint32_t mc_chipid;
    uint16_t mc_coreid;
    uint16_t mc_threadid;
    uint32_t mc_apicid;
    uint32_t mc_clusterid;
    uint32_t mc_ncores;
    uint32_t mc_ncores_active;
    uint32_t mc_nthreads;
    uint32_t mc_cpuid_level;
    uint32_t mc_family;
    uint32_t mc_vendor;
    uint32_t mc_model;
    uint32_t mc_step;
    char mc_vendorid[16];
    char mc_brandid[64];
    uint32_t mc_cpu_caps[7];
    uint32_t mc_cache_size;
    uint32_t mc_cache_alignment;
    uint32_t mc_nmsrvals;
    struct mcinfo_msr mc_msrvalues[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct mcinfo_logical_cpu {
    uint32_t mc_cpunr;
    uint32_t mc_chipid;
    uint16_t mc_coreid;
    uint16_t mc_threadid;
    uint32_t mc_apicid;
    uint32_t mc_clusterid;
    uint32_t mc_ncores;
    uint32_t mc_ncores_active;
    uint32_t mc_nthreads;
    uint32_t mc_cpuid_level;
    uint32_t mc_family;
    uint32_t mc_vendor;
    uint32_t mc_model;
    uint32_t mc_step;
    char mc_vendorid[16];
    char mc_brandid[64];
    uint32_t mc_cpu_caps[7];
    uint32_t mc_cache_size;
    uint32_t mc_cache_alignment;
    uint32_t mc_nmsrvals;
    struct mcinfo_msr mc_msrvalues[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct mcinfo_logical_cpu {
    uint32_t mc_cpunr;
    uint32_t mc_chipid;
    uint16_t mc_coreid;
    uint16_t mc_threadid;
    uint32_t mc_apicid;
    uint32_t mc_clusterid;
    uint32_t mc_ncores;
    uint32_t mc_ncores_active;
    uint32_t mc_nthreads;
    uint32_t mc_cpuid_level;
    uint32_t mc_family;
    uint32_t mc_vendor;
    uint32_t mc_model;
    uint32_t mc_step;
    char mc_vendorid[16];
    char mc_brandid[64];
    uint32_t mc_cpu_caps[7];
    uint32_t mc_cache_size;
    uint32_t mc_cache_alignment;
    uint32_t mc_nmsrvals;
    struct mcinfo_msr mc_msrvalues[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct mcinfo_logical_cpu {
    uint32_t mc_cpunr;
    uint32_t mc_chipid;
    uint16_t mc_coreid;
    uint16_t mc_threadid;
    uint32_t mc_apicid;
    uint32_t mc_clusterid;
    uint32_t mc_ncores;
    uint32_t mc_ncores_active;
    uint32_t mc_nthreads;
    uint32_t mc_cpuid_level;
    uint32_t mc_family;
    uint32_t mc_vendor;
    uint32_t mc_model;
    uint32_t mc_step;
    char mc_vendorid[16];
    char mc_brandid[64];
    uint32_t mc_cpu_caps[7];
    uint32_t mc_cache_size;
    uint32_t mc_cache_alignment;
    uint32_t mc_nmsrvals;
    struct mcinfo_msr mc_msrvalues[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct mcinfo_logical_cpu {
    uint32_t mc_cpunr;
    uint32_t mc_chipid;
    uint16_t mc_coreid;
    uint16_t mc_threadid;
    uint32_t mc_apicid;
    uint32_t mc_clusterid;
    uint32_t mc_ncores;
    uint32_t mc_ncores_active;
    uint32_t mc_nthreads;
    uint32_t mc_cpuid_level;
    uint32_t mc_family;
    uint32_t mc_vendor;
    uint32_t mc_model;
    uint32_t mc_step;
    char mc_vendorid[16];
    char mc_brandid[64];
    uint32_t mc_cpu_caps[7];
    uint32_t mc_cache_size;
    uint32_t mc_cache_alignment;
    uint32_t mc_nmsrvals;
    struct mcinfo_msr mc_msrvalues[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct mcinfo_logical_cpu {
    uint32_t mc_cpunr;
    uint32_t mc_chipid;
    uint16_t mc_coreid;
    uint16_t mc_threadid;
    uint32_t mc_apicid;
    uint32_t mc_clusterid;
    uint32_t mc_ncores;
    uint32_t mc_ncores_active;
    uint32_t mc_nthreads;
    uint32_t mc_cpuid_level;
    uint32_t mc_family;
    uint32_t mc_vendor;
    uint32_t mc_model;
    uint32_t mc_step;
    char mc_vendorid[16];
    char mc_brandid[64];
    uint32_t mc_cpu_caps[7];
    uint32_t mc_cache_size;
    uint32_t mc_cache_alignment;
    uint32_t mc_nmsrvals;
    struct mcinfo_msr mc_msrvalues[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct mcinfo_logical_cpu {
    uint32_t mc_cpunr;
    uint32_t mc_chipid;
    uint16_t mc_coreid;
    uint16_t mc_threadid;
    uint32_t mc_apicid;
    uint32_t mc_clusterid;
    uint32_t mc_ncores;
    uint32_t mc_ncores_active;
    uint32_t mc_nthreads;
    uint32_t mc_cpuid_level;
    uint32_t mc_family;
    uint32_t mc_vendor;
    uint32_t mc_model;
    uint32_t mc_step;
    char mc_vendorid[16];
    char mc_brandid[64];
    uint32_t mc_cpu_caps[7];
    uint32_t mc_cache_size;
    uint32_t mc_cache_alignment;
    uint32_t mc_nmsrvals;
    struct mcinfo_msr mc_msrvalues[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mcinfo_logical_cpu {
    uint32_t mc_cpunr;
    uint32_t mc_chipid;
    uint16_t mc_coreid;
    uint16_t mc_threadid;
    uint32_t mc_apicid;
    uint32_t mc_clusterid;
    uint32_t mc_ncores;
    uint32_t mc_ncores_active;
    uint32_t mc_nthreads;
    uint32_t mc_cpuid_level;
    uint32_t mc_family;
    uint32_t mc_vendor;
    uint32_t mc_model;
    uint32_t mc_step;
    char mc_vendorid[16];
    char mc_brandid[64];
    uint32_t mc_cpu_caps[7];
    uint32_t mc_cache_size;
    uint32_t mc_cache_alignment;
    uint32_t mc_nmsrvals;
    struct mcinfo_msr mc_msrvalues[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mcinfo_logical_cpu {
    uint32_t mc_cpunr;
    uint32_t mc_chipid;
    uint16_t mc_coreid;
    uint16_t mc_threadid;
    uint32_t mc_apicid;
    uint32_t mc_clusterid;
    uint32_t mc_ncores;
    uint32_t mc_ncores_active;
    uint32_t mc_nthreads;
    uint32_t mc_cpuid_level;
    uint32_t mc_family;
    uint32_t mc_vendor;
    uint32_t mc_model;
    uint32_t mc_step;
    char mc_vendorid[16];
    char mc_brandid[64];
    uint32_t mc_cpu_caps[7];
    uint32_t mc_cache_size;
    uint32_t mc_cache_alignment;
    uint32_t mc_nmsrvals;
    struct mcinfo_msr mc_msrvalues[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mcinfo_logical_cpu {
    uint32_t mc_cpunr;
    uint32_t mc_chipid;
    uint16_t mc_coreid;
    uint16_t mc_threadid;
    uint32_t mc_apicid;
    uint32_t mc_clusterid;
    uint32_t mc_ncores;
    uint32_t mc_ncores_active;
    uint32_t mc_nthreads;
    uint32_t mc_cpuid_level;
    uint32_t mc_family;
    uint32_t mc_vendor;
    uint32_t mc_model;
    uint32_t mc_step;
    char mc_vendorid[16];
    char mc_brandid[64];
    uint32_t mc_cpu_caps[7];
    uint32_t mc_cache_size;
    uint32_t mc_cache_alignment;
    uint32_t mc_nmsrvals;
    struct mcinfo_msr mc_msrvalues[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mcinfo_logical_cpu {
    uint32_t mc_cpunr;
    uint32_t mc_chipid;
    uint16_t mc_coreid;
    uint16_t mc_threadid;
    uint32_t mc_apicid;
    uint32_t mc_clusterid;
    uint32_t mc_ncores;
    uint32_t mc_ncores_active;
    uint32_t mc_nthreads;
    uint32_t mc_cpuid_level;
    uint32_t mc_family;
    uint32_t mc_vendor;
    uint32_t mc_model;
    uint32_t mc_step;
    char mc_vendorid[16];
    char mc_brandid[64];
    uint32_t mc_cpu_caps[7];
    uint32_t mc_cache_size;
    uint32_t mc_cache_alignment;
    uint32_t mc_nmsrvals;
    struct mcinfo_msr mc_msrvalues[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mcinfo_logical_cpu {
    uint32_t mc_cpunr;
    uint32_t mc_chipid;
    uint16_t mc_coreid;
    uint16_t mc_threadid;
    uint32_t mc_apicid;
    uint32_t mc_clusterid;
    uint32_t mc_ncores;
    uint32_t mc_ncores_active;
    uint32_t mc_nthreads;
    uint32_t mc_cpuid_level;
    uint32_t mc_family;
    uint32_t mc_vendor;
    uint32_t mc_model;
    uint32_t mc_step;
    char mc_vendorid[16];
    char mc_brandid[64];
    uint32_t mc_cpu_caps[7];
    uint32_t mc_cache_size;
    uint32_t mc_cache_alignment;
    uint32_t mc_nmsrvals;
    struct mcinfo_msr mc_msrvalues[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mcinfo_logical_cpu {
    uint32_t mc_cpunr;
    uint32_t mc_chipid;
    uint16_t mc_coreid;
    uint16_t mc_threadid;
    uint32_t mc_apicid;
    uint32_t mc_clusterid;
    uint32_t mc_ncores;
    uint32_t mc_ncores_active;
    uint32_t mc_nthreads;
    uint32_t mc_cpuid_level;
    uint32_t mc_family;
    uint32_t mc_vendor;
    uint32_t mc_model;
    uint32_t mc_step;
    char mc_vendorid[16];
    char mc_brandid[64];
    uint32_t mc_cpu_caps[7];
    uint32_t mc_cache_size;
    uint32_t mc_cache_alignment;
    uint32_t mc_nmsrvals;
    struct mcinfo_msr mc_msrvalues[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mcinfo_logical_cpu {
    uint32_t mc_cpunr;
    uint32_t mc_chipid;
    uint16_t mc_coreid;
    uint16_t mc_threadid;
    uint32_t mc_apicid;
    uint32_t mc_clusterid;
    uint32_t mc_ncores;
    uint32_t mc_ncores_active;
    uint32_t mc_nthreads;
    uint32_t mc_cpuid_level;
    uint32_t mc_family;
    uint32_t mc_vendor;
    uint32_t mc_model;
    uint32_t mc_step;
    char mc_vendorid[16];
    char mc_brandid[64];
    uint32_t mc_cpu_caps[7];
    uint32_t mc_cache_size;
    uint32_t mc_cache_alignment;
    uint32_t mc_nmsrvals;
    struct mcinfo_msr mc_msrvalues[8];
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct mcinfo_logical_cpu {
    uint32_t mc_cpunr;
    uint32_t mc_chipid;
    uint16_t mc_coreid;
    uint16_t mc_threadid;
    uint32_t mc_apicid;
    uint32_t mc_clusterid;
    uint32_t mc_ncores;
    uint32_t mc_ncores_active;
    uint32_t mc_nthreads;
    uint32_t mc_cpuid_level;
    uint32_t mc_family;
    uint32_t mc_vendor;
    uint32_t mc_model;
    uint32_t mc_step;
    char mc_vendorid[16];
    char mc_brandid[64];
    uint32_t mc_cpu_caps[7];
    uint32_t mc_cache_size;
    uint32_t mc_cache_alignment;
    uint32_t mc_nmsrvals;
    struct mcinfo_msr mc_msrvalues[8];
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
struct mcinfo_logical_cpu {
    uint32_t mc_cpunr;
    uint32_t mc_chipid;
    uint16_t mc_coreid;
    uint16_t mc_threadid;
    uint32_t mc_apicid;
    uint32_t mc_clusterid;
    uint32_t mc_ncores;
    uint32_t mc_ncores_active;
    uint32_t mc_nthreads;
    uint32_t mc_cpuid_level;
    uint32_t mc_family;
    uint32_t mc_vendor;
    uint32_t mc_model;
    uint32_t mc_step;
    char mc_vendorid[16];
    char mc_brandid[64];
    uint32_t mc_cpu_caps[7];
    uint32_t mc_cache_size;
    uint32_t mc_cache_alignment;
    uint32_t mc_nmsrvals;
    struct mcinfo_msr mc_msrvalues[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct mcinfo_logical_cpu {
    uint32_t mc_cpunr;
    uint32_t mc_chipid;
    uint16_t mc_coreid;
    uint16_t mc_threadid;
    uint32_t mc_apicid;
    uint32_t mc_clusterid;
    uint32_t mc_ncores;
    uint32_t mc_ncores_active;
    uint32_t mc_nthreads;
    uint32_t mc_cpuid_level;
    uint32_t mc_family;
    uint32_t mc_vendor;
    uint32_t mc_model;
    uint32_t mc_step;
    char mc_vendorid[16];
    char mc_brandid[64];
    uint32_t mc_cpu_caps[7];
    uint32_t mc_cache_size;
    uint32_t mc_cache_alignment;
    uint32_t mc_nmsrvals;
    struct mcinfo_msr mc_msrvalues[8];
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
