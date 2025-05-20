# Struct: <code>dm_stat</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct dm_stat {
    struct list_head list_entry;
    int id;
    unsigned int stat_flags;
    size_t n_entries;
    sector_t start;
    sector_t end;
    sector_t step;
    unsigned int n_histogram_entries;
    long long unsigned int *histogram_boundaries;
    const char *program_id;
    const char *aux_data;
    struct callback_head callback_head;
    size_t shared_alloc_size;
    size_t percpu_alloc_size;
    size_t histogram_alloc_size;
    struct dm_stat_percpu * stat_percpu[256];
    struct dm_stat_shared stat_shared[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct dm_stat {
    struct list_head list_entry;
    int id;
    unsigned int stat_flags;
    size_t n_entries;
    sector_t start;
    sector_t end;
    sector_t step;
    unsigned int n_histogram_entries;
    long long unsigned int *histogram_boundaries;
    const char *program_id;
    const char *aux_data;
    struct callback_head callback_head;
    size_t shared_alloc_size;
    size_t percpu_alloc_size;
    size_t histogram_alloc_size;
    struct dm_stat_percpu * stat_percpu[256];
    struct dm_stat_shared stat_shared[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct dm_stat {
    struct list_head list_entry;
    int id;
    unsigned int stat_flags;
    size_t n_entries;
    sector_t start;
    sector_t end;
    sector_t step;
    unsigned int n_histogram_entries;
    long long unsigned int *histogram_boundaries;
    const char *program_id;
    const char *aux_data;
    struct callback_head callback_head;
    size_t shared_alloc_size;
    size_t percpu_alloc_size;
    size_t histogram_alloc_size;
    struct dm_stat_percpu * stat_percpu[8192];
    struct dm_stat_shared stat_shared[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct dm_stat {
    struct list_head list_entry;
    int id;
    unsigned int stat_flags;
    size_t n_entries;
    sector_t start;
    sector_t end;
    sector_t step;
    unsigned int n_histogram_entries;
    long long unsigned int *histogram_boundaries;
    const char *program_id;
    const char *aux_data;
    struct callback_head callback_head;
    size_t shared_alloc_size;
    size_t percpu_alloc_size;
    size_t histogram_alloc_size;
    struct dm_stat_percpu * stat_percpu[8192];
    struct dm_stat_shared stat_shared[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dm_stat {
    struct list_head list_entry;
    int id;
    unsigned int stat_flags;
    size_t n_entries;
    sector_t start;
    sector_t end;
    sector_t step;
    unsigned int n_histogram_entries;
    long long unsigned int *histogram_boundaries;
    const char *program_id;
    const char *aux_data;
    struct callback_head callback_head;
    size_t shared_alloc_size;
    size_t percpu_alloc_size;
    size_t histogram_alloc_size;
    struct dm_stat_percpu * stat_percpu[8192];
    struct dm_stat_shared stat_shared[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dm_stat {
    struct list_head list_entry;
    int id;
    unsigned int stat_flags;
    size_t n_entries;
    sector_t start;
    sector_t end;
    sector_t step;
    unsigned int n_histogram_entries;
    long long unsigned int *histogram_boundaries;
    const char *program_id;
    const char *aux_data;
    struct callback_head callback_head;
    size_t shared_alloc_size;
    size_t percpu_alloc_size;
    size_t histogram_alloc_size;
    struct dm_stat_percpu * stat_percpu[8192];
    struct dm_stat_shared stat_shared[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dm_stat {
    struct list_head list_entry;
    int id;
    unsigned int stat_flags;
    size_t n_entries;
    sector_t start;
    sector_t end;
    sector_t step;
    unsigned int n_histogram_entries;
    long long unsigned int *histogram_boundaries;
    const char *program_id;
    const char *aux_data;
    struct callback_head callback_head;
    size_t shared_alloc_size;
    size_t percpu_alloc_size;
    size_t histogram_alloc_size;
    struct dm_stat_percpu * stat_percpu[8192];
    struct dm_stat_shared stat_shared[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dm_stat {
    struct list_head list_entry;
    int id;
    unsigned int stat_flags;
    size_t n_entries;
    sector_t start;
    sector_t end;
    sector_t step;
    unsigned int n_histogram_entries;
    long long unsigned int *histogram_boundaries;
    const char *program_id;
    const char *aux_data;
    struct callback_head callback_head;
    size_t shared_alloc_size;
    size_t percpu_alloc_size;
    size_t histogram_alloc_size;
    struct dm_stat_percpu * stat_percpu[8192];
    struct dm_stat_shared stat_shared[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dm_stat {
    struct list_head list_entry;
    int id;
    unsigned int stat_flags;
    size_t n_entries;
    sector_t start;
    sector_t end;
    sector_t step;
    unsigned int n_histogram_entries;
    long long unsigned int *histogram_boundaries;
    const char *program_id;
    const char *aux_data;
    struct callback_head callback_head;
    size_t shared_alloc_size;
    size_t percpu_alloc_size;
    size_t histogram_alloc_size;
    struct dm_stat_percpu * stat_percpu[8192];
    struct dm_stat_shared stat_shared[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dm_stat {
    struct list_head list_entry;
    int id;
    unsigned int stat_flags;
    size_t n_entries;
    sector_t start;
    sector_t end;
    sector_t step;
    unsigned int n_histogram_entries;
    long long unsigned int *histogram_boundaries;
    const char *program_id;
    const char *aux_data;
    struct callback_head callback_head;
    size_t shared_alloc_size;
    size_t percpu_alloc_size;
    size_t histogram_alloc_size;
    struct dm_stat_percpu * stat_percpu[8192];
    struct dm_stat_shared stat_shared[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dm_stat {
    struct list_head list_entry;
    int id;
    unsigned int stat_flags;
    size_t n_entries;
    sector_t start;
    sector_t end;
    sector_t step;
    unsigned int n_histogram_entries;
    long long unsigned int *histogram_boundaries;
    const char *program_id;
    const char *aux_data;
    struct callback_head callback_head;
    size_t shared_alloc_size;
    size_t percpu_alloc_size;
    size_t histogram_alloc_size;
    struct dm_stat_percpu * stat_percpu[8192];
    struct dm_stat_shared stat_shared[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dm_stat {
    struct list_head list_entry;
    int id;
    unsigned int stat_flags;
    size_t n_entries;
    sector_t start;
    sector_t end;
    sector_t step;
    unsigned int n_histogram_entries;
    long long unsigned int *histogram_boundaries;
    const char *program_id;
    const char *aux_data;
    struct callback_head callback_head;
    size_t shared_alloc_size;
    size_t percpu_alloc_size;
    size_t histogram_alloc_size;
    struct dm_stat_percpu * stat_percpu[8192];
    struct dm_stat_shared stat_shared[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dm_stat {
    struct list_head list_entry;
    int id;
    unsigned int stat_flags;
    size_t n_entries;
    sector_t start;
    sector_t end;
    sector_t step;
    unsigned int n_histogram_entries;
    long long unsigned int *histogram_boundaries;
    const char *program_id;
    const char *aux_data;
    struct callback_head callback_head;
    size_t shared_alloc_size;
    size_t percpu_alloc_size;
    size_t histogram_alloc_size;
    struct dm_stat_percpu * stat_percpu[8192];
    struct dm_stat_shared stat_shared[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dm_stat {
    struct list_head list_entry;
    int id;
    unsigned int stat_flags;
    size_t n_entries;
    sector_t start;
    sector_t end;
    sector_t step;
    unsigned int n_histogram_entries;
    long long unsigned int *histogram_boundaries;
    const char *program_id;
    const char *aux_data;
    struct callback_head callback_head;
    size_t shared_alloc_size;
    size_t percpu_alloc_size;
    size_t histogram_alloc_size;
    struct dm_stat_percpu * stat_percpu[8192];
    struct dm_stat_shared stat_shared[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dm_stat {
    struct list_head list_entry;
    int id;
    unsigned int stat_flags;
    size_t n_entries;
    sector_t start;
    sector_t end;
    sector_t step;
    unsigned int n_histogram_entries;
    long long unsigned int *histogram_boundaries;
    const char *program_id;
    const char *aux_data;
    struct callback_head callback_head;
    size_t shared_alloc_size;
    size_t percpu_alloc_size;
    size_t histogram_alloc_size;
    struct dm_stat_percpu * stat_percpu[8192];
    struct dm_stat_shared stat_shared[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dm_stat {
    struct list_head list_entry;
    int id;
    unsigned int stat_flags;
    size_t n_entries;
    sector_t start;
    sector_t end;
    sector_t step;
    unsigned int n_histogram_entries;
    long long unsigned int *histogram_boundaries;
    const char *program_id;
    const char *aux_data;
    struct callback_head callback_head;
    size_t shared_alloc_size;
    size_t percpu_alloc_size;
    size_t histogram_alloc_size;
    struct dm_stat_percpu * stat_percpu[8192];
    struct dm_stat_shared stat_shared[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dm_stat {
    struct list_head list_entry;
    int id;
    unsigned int stat_flags;
    size_t n_entries;
    sector_t start;
    sector_t end;
    sector_t step;
    unsigned int n_histogram_entries;
    long long unsigned int *histogram_boundaries;
    const char *program_id;
    const char *aux_data;
    struct callback_head callback_head;
    size_t shared_alloc_size;
    size_t percpu_alloc_size;
    size_t histogram_alloc_size;
    struct dm_stat_percpu * stat_percpu[8192];
    struct dm_stat_shared stat_shared[0];
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
struct dm_stat {
    struct list_head list_entry;
    int id;
    unsigned int stat_flags;
    size_t n_entries;
    sector_t start;
    sector_t end;
    sector_t step;
    unsigned int n_histogram_entries;
    long long unsigned int *histogram_boundaries;
    const char *program_id;
    const char *aux_data;
    struct callback_head callback_head;
    size_t shared_alloc_size;
    size_t percpu_alloc_size;
    size_t histogram_alloc_size;
    struct dm_stat_percpu * stat_percpu[256];
    struct dm_stat_shared stat_shared[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dm_stat {
    struct list_head list_entry;
    int id;
    unsigned int stat_flags;
    size_t n_entries;
    sector_t start;
    sector_t end;
    sector_t step;
    unsigned int n_histogram_entries;
    long long unsigned int *histogram_boundaries;
    const char *program_id;
    const char *aux_data;
    struct callback_head callback_head;
    size_t shared_alloc_size;
    size_t percpu_alloc_size;
    size_t histogram_alloc_size;
    struct dm_stat_percpu * stat_percpu[4];
    struct dm_stat_shared stat_shared[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dm_stat {
    struct list_head list_entry;
    int id;
    unsigned int stat_flags;
    size_t n_entries;
    sector_t start;
    sector_t end;
    sector_t step;
    unsigned int n_histogram_entries;
    long long unsigned int *histogram_boundaries;
    const char *program_id;
    const char *aux_data;
    struct callback_head callback_head;
    size_t shared_alloc_size;
    size_t percpu_alloc_size;
    size_t histogram_alloc_size;
    struct dm_stat_percpu * stat_percpu[2048];
    struct dm_stat_shared stat_shared[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dm_stat {
    struct list_head list_entry;
    int id;
    unsigned int stat_flags;
    size_t n_entries;
    sector_t start;
    sector_t end;
    sector_t step;
    unsigned int n_histogram_entries;
    long long unsigned int *histogram_boundaries;
    const char *program_id;
    const char *aux_data;
    struct callback_head callback_head;
    size_t shared_alloc_size;
    size_t percpu_alloc_size;
    size_t histogram_alloc_size;
    struct dm_stat_percpu * stat_percpu[8];
    struct dm_stat_shared stat_shared[0];
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
struct dm_stat {
    struct list_head list_entry;
    int id;
    unsigned int stat_flags;
    size_t n_entries;
    sector_t start;
    sector_t end;
    sector_t step;
    unsigned int n_histogram_entries;
    long long unsigned int *histogram_boundaries;
    const char *program_id;
    const char *aux_data;
    struct callback_head callback_head;
    size_t shared_alloc_size;
    size_t percpu_alloc_size;
    size_t histogram_alloc_size;
    struct dm_stat_percpu * stat_percpu[8192];
    struct dm_stat_shared stat_shared[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dm_stat {
    struct list_head list_entry;
    int id;
    unsigned int stat_flags;
    size_t n_entries;
    sector_t start;
    sector_t end;
    sector_t step;
    unsigned int n_histogram_entries;
    long long unsigned int *histogram_boundaries;
    const char *program_id;
    const char *aux_data;
    struct callback_head callback_head;
    size_t shared_alloc_size;
    size_t percpu_alloc_size;
    size_t histogram_alloc_size;
    struct dm_stat_percpu * stat_percpu[8192];
    struct dm_stat_shared stat_shared[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dm_stat {
    struct list_head list_entry;
    int id;
    unsigned int stat_flags;
    size_t n_entries;
    sector_t start;
    sector_t end;
    sector_t step;
    unsigned int n_histogram_entries;
    long long unsigned int *histogram_boundaries;
    const char *program_id;
    const char *aux_data;
    struct callback_head callback_head;
    size_t shared_alloc_size;
    size_t percpu_alloc_size;
    size_t histogram_alloc_size;
    struct dm_stat_percpu * stat_percpu[8192];
    struct dm_stat_shared stat_shared[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dm_stat {
    struct list_head list_entry;
    int id;
    unsigned int stat_flags;
    size_t n_entries;
    sector_t start;
    sector_t end;
    sector_t step;
    unsigned int n_histogram_entries;
    long long unsigned int *histogram_boundaries;
    const char *program_id;
    const char *aux_data;
    struct callback_head callback_head;
    size_t shared_alloc_size;
    size_t percpu_alloc_size;
    size_t histogram_alloc_size;
    struct dm_stat_percpu * stat_percpu[8192];
    struct dm_stat_shared stat_shared[0];
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
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct dm_stat_percpu * stat_percpu[256]</code> ➡️ <code>struct dm_stat_percpu * stat_percpu[8192]</code>
</li>
</ul>
</details>
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
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>arm64</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct dm_stat_percpu * stat_percpu[8192]</code> ➡️ <code>struct dm_stat_percpu * stat_percpu[256]</code>
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
<code>struct dm_stat_percpu * stat_percpu[8192]</code> ➡️ <code>struct dm_stat_percpu * stat_percpu[4]</code>
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
<code>struct dm_stat_percpu * stat_percpu[8192]</code> ➡️ <code>struct dm_stat_percpu * stat_percpu[2048]</code>
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
<code>struct dm_stat_percpu * stat_percpu[8192]</code> ➡️ <code>struct dm_stat_percpu * stat_percpu[8]</code>
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
