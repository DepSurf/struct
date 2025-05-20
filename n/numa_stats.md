# Struct: <code>numa_stats</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct numa_stats {
    long unsigned int nr_running;
    long unsigned int load;
    long unsigned int compute_capacity;
    long unsigned int task_capacity;
    int has_free_capacity;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct numa_stats {
    long unsigned int nr_running;
    long unsigned int load;
    long unsigned int compute_capacity;
    long unsigned int task_capacity;
    int has_free_capacity;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct numa_stats {
    long unsigned int nr_running;
    long unsigned int load;
    long unsigned int compute_capacity;
    long unsigned int task_capacity;
    int has_free_capacity;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct numa_stats {
    long unsigned int nr_running;
    long unsigned int load;
    long unsigned int compute_capacity;
    long unsigned int task_capacity;
    int has_free_capacity;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct numa_stats {
    long unsigned int nr_running;
    long unsigned int load;
    long unsigned int compute_capacity;
    long unsigned int task_capacity;
    int has_free_capacity;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct numa_stats {
    long unsigned int nr_running;
    long unsigned int load;
    long unsigned int compute_capacity;
    long unsigned int task_capacity;
    int has_free_capacity;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct numa_stats {
    long unsigned int load;
    long unsigned int compute_capacity;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct numa_stats {
    long unsigned int load;
    long unsigned int compute_capacity;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct numa_stats {
    long unsigned int load;
    long unsigned int compute_capacity;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct numa_stats {
    long unsigned int load;
    long unsigned int util;
    long unsigned int compute_capacity;
    unsigned int nr_running;
    unsigned int weight;
    enum numa_type node_type;
    int idle_cpu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct numa_stats {
    long unsigned int load;
    long unsigned int runnable;
    long unsigned int util;
    long unsigned int compute_capacity;
    unsigned int nr_running;
    unsigned int weight;
    enum numa_type node_type;
    int idle_cpu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct numa_stats {
    long unsigned int load;
    long unsigned int runnable;
    long unsigned int util;
    long unsigned int compute_capacity;
    unsigned int nr_running;
    unsigned int weight;
    enum numa_type node_type;
    int idle_cpu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct numa_stats {
    long unsigned int load;
    long unsigned int runnable;
    long unsigned int util;
    long unsigned int compute_capacity;
    unsigned int nr_running;
    unsigned int weight;
    enum numa_type node_type;
    int idle_cpu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct numa_stats {
    long unsigned int load;
    long unsigned int runnable;
    long unsigned int util;
    long unsigned int compute_capacity;
    unsigned int nr_running;
    unsigned int weight;
    enum numa_type node_type;
    int idle_cpu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct numa_stats {
    long unsigned int load;
    long unsigned int runnable;
    long unsigned int util;
    long unsigned int compute_capacity;
    unsigned int nr_running;
    unsigned int weight;
    enum numa_type node_type;
    int idle_cpu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct numa_stats {
    long unsigned int load;
    long unsigned int runnable;
    long unsigned int util;
    long unsigned int compute_capacity;
    unsigned int nr_running;
    unsigned int weight;
    enum numa_type node_type;
    int idle_cpu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct numa_stats {
    long unsigned int load;
    long unsigned int runnable;
    long unsigned int util;
    long unsigned int compute_capacity;
    unsigned int nr_running;
    unsigned int weight;
    enum numa_type node_type;
    int idle_cpu;
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
struct numa_stats {
    long unsigned int load;
    long unsigned int compute_capacity;
};
```
</details>
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct numa_stats {
    long unsigned int load;
    long unsigned int compute_capacity;
};
```
</details>
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
struct numa_stats {
    long unsigned int load;
    long unsigned int compute_capacity;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct numa_stats {
    long unsigned int load;
    long unsigned int compute_capacity;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct numa_stats {
    long unsigned int load;
    long unsigned int compute_capacity;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct numa_stats {
    long unsigned int load;
    long unsigned int compute_capacity;
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
<b>Field removed. </b>
<code>long unsigned int nr_running</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int task_capacity</code>
</li>
<li>
<b>Field removed. </b>
<code>int has_free_capacity</code>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int util</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int nr_running</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int weight</code>
</li>
<li>
<b>Field added. </b>
<code>enum numa_type node_type</code>
</li>
<li>
<b>Field added. </b>
<code>int idle_cpu</code>
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
<code>long unsigned int runnable</code>
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
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
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
