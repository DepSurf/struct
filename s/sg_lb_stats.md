# Struct: <code>sg_lb_stats</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct sg_lb_stats {
    long unsigned int avg_load;
    long unsigned int group_load;
    long unsigned int sum_weighted_load;
    long unsigned int load_per_task;
    long unsigned int group_capacity;
    long unsigned int group_util;
    unsigned int sum_nr_running;
    unsigned int idle_cpus;
    unsigned int group_weight;
    enum group_type group_type;
    int group_no_capacity;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct sg_lb_stats {
    long unsigned int avg_load;
    long unsigned int group_load;
    long unsigned int sum_weighted_load;
    long unsigned int load_per_task;
    long unsigned int group_capacity;
    long unsigned int group_util;
    unsigned int sum_nr_running;
    unsigned int idle_cpus;
    unsigned int group_weight;
    enum group_type group_type;
    int group_no_capacity;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct sg_lb_stats {
    long unsigned int avg_load;
    long unsigned int group_load;
    long unsigned int sum_weighted_load;
    long unsigned int load_per_task;
    long unsigned int group_capacity;
    long unsigned int group_util;
    unsigned int sum_nr_running;
    unsigned int idle_cpus;
    unsigned int group_weight;
    enum group_type group_type;
    int group_no_capacity;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct sg_lb_stats {
    long unsigned int avg_load;
    long unsigned int group_load;
    long unsigned int sum_weighted_load;
    long unsigned int load_per_task;
    long unsigned int group_capacity;
    long unsigned int group_util;
    unsigned int sum_nr_running;
    unsigned int idle_cpus;
    unsigned int group_weight;
    enum group_type group_type;
    int group_no_capacity;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct sg_lb_stats {
    long unsigned int avg_load;
    long unsigned int group_load;
    long unsigned int sum_weighted_load;
    long unsigned int load_per_task;
    long unsigned int group_capacity;
    long unsigned int group_util;
    unsigned int sum_nr_running;
    unsigned int idle_cpus;
    unsigned int group_weight;
    enum group_type group_type;
    int group_no_capacity;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct sg_lb_stats {
    long unsigned int avg_load;
    long unsigned int group_load;
    long unsigned int sum_weighted_load;
    long unsigned int load_per_task;
    long unsigned int group_capacity;
    long unsigned int group_util;
    unsigned int sum_nr_running;
    unsigned int idle_cpus;
    unsigned int group_weight;
    enum group_type group_type;
    int group_no_capacity;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct sg_lb_stats {
    long unsigned int avg_load;
    long unsigned int group_load;
    long unsigned int sum_weighted_load;
    long unsigned int load_per_task;
    long unsigned int group_capacity;
    long unsigned int group_util;
    unsigned int sum_nr_running;
    unsigned int idle_cpus;
    unsigned int group_weight;
    enum group_type group_type;
    int group_no_capacity;
    long unsigned int group_misfit_task_load;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct sg_lb_stats {
    long unsigned int avg_load;
    long unsigned int group_load;
    long unsigned int load_per_task;
    long unsigned int group_capacity;
    long unsigned int group_util;
    unsigned int sum_nr_running;
    unsigned int idle_cpus;
    unsigned int group_weight;
    enum group_type group_type;
    int group_no_capacity;
    long unsigned int group_misfit_task_load;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct sg_lb_stats {
    long unsigned int avg_load;
    long unsigned int group_load;
    long unsigned int load_per_task;
    long unsigned int group_capacity;
    long unsigned int group_util;
    unsigned int sum_nr_running;
    unsigned int idle_cpus;
    unsigned int group_weight;
    enum group_type group_type;
    int group_no_capacity;
    long unsigned int group_misfit_task_load;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct sg_lb_stats {
    long unsigned int avg_load;
    long unsigned int group_load;
    long unsigned int group_capacity;
    long unsigned int group_util;
    long unsigned int group_runnable;
    unsigned int sum_nr_running;
    unsigned int sum_h_nr_running;
    unsigned int idle_cpus;
    unsigned int group_weight;
    enum group_type group_type;
    unsigned int group_asym_packing;
    long unsigned int group_misfit_task_load;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct sg_lb_stats {
    long unsigned int avg_load;
    long unsigned int group_load;
    long unsigned int group_capacity;
    long unsigned int group_util;
    long unsigned int group_runnable;
    unsigned int sum_nr_running;
    unsigned int sum_h_nr_running;
    unsigned int idle_cpus;
    unsigned int group_weight;
    enum group_type group_type;
    unsigned int group_asym_packing;
    long unsigned int group_misfit_task_load;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct sg_lb_stats {
    long unsigned int avg_load;
    long unsigned int group_load;
    long unsigned int group_capacity;
    long unsigned int group_util;
    long unsigned int group_runnable;
    unsigned int sum_nr_running;
    unsigned int sum_h_nr_running;
    unsigned int idle_cpus;
    unsigned int group_weight;
    enum group_type group_type;
    unsigned int group_asym_packing;
    long unsigned int group_misfit_task_load;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct sg_lb_stats {
    long unsigned int avg_load;
    long unsigned int group_load;
    long unsigned int group_capacity;
    long unsigned int group_util;
    long unsigned int group_runnable;
    unsigned int sum_nr_running;
    unsigned int sum_h_nr_running;
    unsigned int idle_cpus;
    unsigned int group_weight;
    enum group_type group_type;
    unsigned int group_asym_packing;
    long unsigned int group_misfit_task_load;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct sg_lb_stats {
    long unsigned int avg_load;
    long unsigned int group_load;
    long unsigned int group_capacity;
    long unsigned int group_util;
    long unsigned int group_runnable;
    unsigned int sum_nr_running;
    unsigned int sum_h_nr_running;
    unsigned int idle_cpus;
    unsigned int group_weight;
    enum group_type group_type;
    unsigned int group_asym_packing;
    long unsigned int group_misfit_task_load;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct sg_lb_stats {
    long unsigned int avg_load;
    long unsigned int group_load;
    long unsigned int group_capacity;
    long unsigned int group_util;
    long unsigned int group_runnable;
    unsigned int sum_nr_running;
    unsigned int sum_h_nr_running;
    unsigned int idle_cpus;
    unsigned int group_weight;
    enum group_type group_type;
    unsigned int group_asym_packing;
    long unsigned int group_misfit_task_load;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct sg_lb_stats {
    long unsigned int avg_load;
    long unsigned int group_load;
    long unsigned int group_capacity;
    long unsigned int group_util;
    long unsigned int group_runnable;
    unsigned int sum_nr_running;
    unsigned int sum_h_nr_running;
    unsigned int idle_cpus;
    unsigned int group_weight;
    enum group_type group_type;
    unsigned int group_asym_packing;
    long unsigned int group_misfit_task_load;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct sg_lb_stats {
    long unsigned int avg_load;
    long unsigned int group_load;
    long unsigned int group_capacity;
    long unsigned int group_util;
    long unsigned int group_runnable;
    unsigned int sum_nr_running;
    unsigned int sum_h_nr_running;
    unsigned int idle_cpus;
    unsigned int group_weight;
    enum group_type group_type;
    unsigned int group_asym_packing;
    unsigned int group_smt_balance;
    long unsigned int group_misfit_task_load;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
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
struct sg_lb_stats {
    long unsigned int avg_load;
    long unsigned int group_load;
    long unsigned int load_per_task;
    long unsigned int group_capacity;
    long unsigned int group_util;
    unsigned int sum_nr_running;
    unsigned int idle_cpus;
    unsigned int group_weight;
    enum group_type group_type;
    int group_no_capacity;
    long unsigned int group_misfit_task_load;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct sg_lb_stats {
    long unsigned int avg_load;
    long unsigned int group_load;
    long unsigned int load_per_task;
    long unsigned int group_capacity;
    long unsigned int group_util;
    unsigned int sum_nr_running;
    unsigned int idle_cpus;
    unsigned int group_weight;
    enum group_type group_type;
    int group_no_capacity;
    long unsigned int group_misfit_task_load;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct sg_lb_stats {
    long unsigned int avg_load;
    long unsigned int group_load;
    long unsigned int load_per_task;
    long unsigned int group_capacity;
    long unsigned int group_util;
    unsigned int sum_nr_running;
    unsigned int idle_cpus;
    unsigned int group_weight;
    enum group_type group_type;
    int group_no_capacity;
    long unsigned int group_misfit_task_load;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct sg_lb_stats {
    long unsigned int avg_load;
    long unsigned int group_load;
    long unsigned int load_per_task;
    long unsigned int group_capacity;
    long unsigned int group_util;
    unsigned int sum_nr_running;
    unsigned int idle_cpus;
    unsigned int group_weight;
    enum group_type group_type;
    int group_no_capacity;
    long unsigned int group_misfit_task_load;
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
struct sg_lb_stats {
    long unsigned int avg_load;
    long unsigned int group_load;
    long unsigned int load_per_task;
    long unsigned int group_capacity;
    long unsigned int group_util;
    unsigned int sum_nr_running;
    unsigned int idle_cpus;
    unsigned int group_weight;
    enum group_type group_type;
    int group_no_capacity;
    long unsigned int group_misfit_task_load;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct sg_lb_stats {
    long unsigned int avg_load;
    long unsigned int group_load;
    long unsigned int load_per_task;
    long unsigned int group_capacity;
    long unsigned int group_util;
    unsigned int sum_nr_running;
    unsigned int idle_cpus;
    unsigned int group_weight;
    enum group_type group_type;
    int group_no_capacity;
    long unsigned int group_misfit_task_load;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct sg_lb_stats {
    long unsigned int avg_load;
    long unsigned int group_load;
    long unsigned int load_per_task;
    long unsigned int group_capacity;
    long unsigned int group_util;
    unsigned int sum_nr_running;
    unsigned int idle_cpus;
    unsigned int group_weight;
    enum group_type group_type;
    int group_no_capacity;
    long unsigned int group_misfit_task_load;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct sg_lb_stats {
    long unsigned int avg_load;
    long unsigned int group_load;
    long unsigned int load_per_task;
    long unsigned int group_capacity;
    long unsigned int group_util;
    unsigned int sum_nr_running;
    unsigned int idle_cpus;
    unsigned int group_weight;
    enum group_type group_type;
    int group_no_capacity;
    long unsigned int group_misfit_task_load;
    unsigned int nr_numa_running;
    unsigned int nr_preferred_running;
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
<code>long unsigned int group_misfit_task_load</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>long unsigned int sum_weighted_load</code>
</li>
</ul>
</details>
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
<code>long unsigned int group_runnable</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int sum_h_nr_running</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int group_asym_packing</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int load_per_task</code>
</li>
<li>
<b>Field removed. </b>
<code>int group_no_capacity</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int group_smt_balance</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned int nr_numa_running</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int nr_preferred_running</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned int nr_numa_running</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int nr_preferred_running</code>
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
