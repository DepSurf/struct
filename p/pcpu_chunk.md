# Struct: <code>pcpu_chunk</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct pcpu_chunk {
    struct list_head list;
    int free_size;
    int contig_hint;
    void *base_addr;
    int map_used;
    int map_alloc;
    int *map;
    struct work_struct map_extend_work;
    void *data;
    int first_free;
    bool immutable;
    int nr_populated;
    long unsigned int populated[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct pcpu_chunk {
    struct list_head list;
    int free_size;
    int contig_hint;
    void *base_addr;
    int map_used;
    int map_alloc;
    int *map;
    struct list_head map_extend_list;
    void *data;
    int first_free;
    bool immutable;
    int nr_populated;
    long unsigned int populated[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct pcpu_chunk {
    struct list_head list;
    int free_size;
    int contig_hint;
    void *base_addr;
    int map_used;
    int map_alloc;
    int *map;
    struct list_head map_extend_list;
    void *data;
    int first_free;
    bool immutable;
    int nr_populated;
    long unsigned int populated[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct pcpu_chunk {
    struct list_head list;
    int free_size;
    int contig_hint;
    void *base_addr;
    int map_used;
    int map_alloc;
    int *map;
    struct list_head map_extend_list;
    void *data;
    int first_free;
    bool immutable;
    bool has_reserved;
    int nr_populated;
    long unsigned int populated[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct pcpu_chunk {
    struct list_head list;
    int free_bytes;
    int contig_bits;
    int contig_bits_start;
    void *base_addr;
    long unsigned int *alloc_map;
    long unsigned int *bound_map;
    struct pcpu_block_md *md_blocks;
    void *data;
    int first_bit;
    bool immutable;
    int start_offset;
    int end_offset;
    int nr_pages;
    int nr_populated;
    int nr_empty_pop_pages;
    long unsigned int populated[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct pcpu_chunk {
    struct list_head list;
    int free_bytes;
    int contig_bits;
    int contig_bits_start;
    void *base_addr;
    long unsigned int *alloc_map;
    long unsigned int *bound_map;
    struct pcpu_block_md *md_blocks;
    void *data;
    int first_bit;
    bool immutable;
    int start_offset;
    int end_offset;
    int nr_pages;
    int nr_populated;
    int nr_empty_pop_pages;
    long unsigned int populated[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct pcpu_chunk {
    struct list_head list;
    int free_bytes;
    int contig_bits;
    int contig_bits_start;
    void *base_addr;
    long unsigned int *alloc_map;
    long unsigned int *bound_map;
    struct pcpu_block_md *md_blocks;
    void *data;
    int first_bit;
    bool immutable;
    int start_offset;
    int end_offset;
    int nr_pages;
    int nr_populated;
    int nr_empty_pop_pages;
    long unsigned int populated[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct pcpu_chunk {
    struct list_head list;
    int free_bytes;
    struct pcpu_block_md chunk_md;
    void *base_addr;
    long unsigned int *alloc_map;
    long unsigned int *bound_map;
    struct pcpu_block_md *md_blocks;
    void *data;
    bool immutable;
    int start_offset;
    int end_offset;
    int nr_pages;
    int nr_populated;
    int nr_empty_pop_pages;
    long unsigned int populated[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct pcpu_chunk {
    struct list_head list;
    int free_bytes;
    struct pcpu_block_md chunk_md;
    void *base_addr;
    long unsigned int *alloc_map;
    long unsigned int *bound_map;
    struct pcpu_block_md *md_blocks;
    void *data;
    bool immutable;
    int start_offset;
    int end_offset;
    int nr_pages;
    int nr_populated;
    int nr_empty_pop_pages;
    long unsigned int populated[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct pcpu_chunk {
    struct list_head list;
    int free_bytes;
    struct pcpu_block_md chunk_md;
    void *base_addr;
    long unsigned int *alloc_map;
    long unsigned int *bound_map;
    struct pcpu_block_md *md_blocks;
    void *data;
    bool immutable;
    int start_offset;
    int end_offset;
    int nr_pages;
    int nr_populated;
    int nr_empty_pop_pages;
    long unsigned int populated[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct pcpu_chunk {
    struct list_head list;
    int free_bytes;
    struct pcpu_block_md chunk_md;
    void *base_addr;
    long unsigned int *alloc_map;
    long unsigned int *bound_map;
    struct pcpu_block_md *md_blocks;
    void *data;
    bool immutable;
    int start_offset;
    int end_offset;
    struct obj_cgroup **obj_cgroups;
    int nr_pages;
    int nr_populated;
    int nr_empty_pop_pages;
    long unsigned int populated[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct pcpu_chunk {
    struct list_head list;
    int free_bytes;
    struct pcpu_block_md chunk_md;
    void *base_addr;
    long unsigned int *alloc_map;
    long unsigned int *bound_map;
    struct pcpu_block_md *md_blocks;
    void *data;
    bool immutable;
    int start_offset;
    int end_offset;
    struct obj_cgroup **obj_cgroups;
    int nr_pages;
    int nr_populated;
    int nr_empty_pop_pages;
    long unsigned int populated[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct pcpu_chunk {
    struct list_head list;
    int free_bytes;
    struct pcpu_block_md chunk_md;
    void *base_addr;
    long unsigned int *alloc_map;
    long unsigned int *bound_map;
    struct pcpu_block_md *md_blocks;
    void *data;
    bool immutable;
    bool isolated;
    int start_offset;
    int end_offset;
    struct obj_cgroup **obj_cgroups;
    int nr_pages;
    int nr_populated;
    int nr_empty_pop_pages;
    long unsigned int populated[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct pcpu_chunk {
    struct list_head list;
    int free_bytes;
    struct pcpu_block_md chunk_md;
    void *base_addr;
    long unsigned int *alloc_map;
    long unsigned int *bound_map;
    struct pcpu_block_md *md_blocks;
    void *data;
    bool immutable;
    bool isolated;
    int start_offset;
    int end_offset;
    struct obj_cgroup **obj_cgroups;
    int nr_pages;
    int nr_populated;
    int nr_empty_pop_pages;
    long unsigned int populated[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct pcpu_chunk {
    struct list_head list;
    int free_bytes;
    struct pcpu_block_md chunk_md;
    void *base_addr;
    long unsigned int *alloc_map;
    long unsigned int *bound_map;
    struct pcpu_block_md *md_blocks;
    void *data;
    bool immutable;
    bool isolated;
    int start_offset;
    int end_offset;
    struct obj_cgroup **obj_cgroups;
    int nr_pages;
    int nr_populated;
    int nr_empty_pop_pages;
    long unsigned int populated[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct pcpu_chunk {
    struct list_head list;
    int free_bytes;
    struct pcpu_block_md chunk_md;
    long unsigned int *bound_map;
    void *base_addr;
    long unsigned int *alloc_map;
    struct pcpu_block_md *md_blocks;
    void *data;
    bool immutable;
    bool isolated;
    int start_offset;
    int end_offset;
    struct obj_cgroup **obj_cgroups;
    int nr_pages;
    int nr_populated;
    int nr_empty_pop_pages;
    long unsigned int populated[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct pcpu_chunk {
    struct list_head list;
    int free_bytes;
    struct pcpu_block_md chunk_md;
    long unsigned int *bound_map;
    void *base_addr;
    long unsigned int *alloc_map;
    struct pcpu_block_md *md_blocks;
    void *data;
    bool immutable;
    bool isolated;
    int start_offset;
    int end_offset;
    struct obj_cgroup **obj_cgroups;
    int nr_pages;
    int nr_populated;
    int nr_empty_pop_pages;
    long unsigned int populated[0];
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
struct pcpu_chunk {
    struct list_head list;
    int free_bytes;
    struct pcpu_block_md chunk_md;
    void *base_addr;
    long unsigned int *alloc_map;
    long unsigned int *bound_map;
    struct pcpu_block_md *md_blocks;
    void *data;
    bool immutable;
    int start_offset;
    int end_offset;
    int nr_pages;
    int nr_populated;
    int nr_empty_pop_pages;
    long unsigned int populated[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct pcpu_chunk {
    struct list_head list;
    int free_bytes;
    struct pcpu_block_md chunk_md;
    void *base_addr;
    long unsigned int *alloc_map;
    long unsigned int *bound_map;
    struct pcpu_block_md *md_blocks;
    void *data;
    bool immutable;
    int start_offset;
    int end_offset;
    int nr_pages;
    int nr_populated;
    int nr_empty_pop_pages;
    long unsigned int populated[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct pcpu_chunk {
    struct list_head list;
    int free_bytes;
    struct pcpu_block_md chunk_md;
    void *base_addr;
    long unsigned int *alloc_map;
    long unsigned int *bound_map;
    struct pcpu_block_md *md_blocks;
    void *data;
    bool immutable;
    int start_offset;
    int end_offset;
    int nr_pages;
    int nr_populated;
    int nr_empty_pop_pages;
    long unsigned int populated[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct pcpu_chunk {
    struct list_head list;
    int free_bytes;
    struct pcpu_block_md chunk_md;
    void *base_addr;
    long unsigned int *alloc_map;
    long unsigned int *bound_map;
    struct pcpu_block_md *md_blocks;
    void *data;
    bool immutable;
    int start_offset;
    int end_offset;
    int nr_pages;
    int nr_populated;
    int nr_empty_pop_pages;
    long unsigned int populated[0];
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
struct pcpu_chunk {
    struct list_head list;
    int free_bytes;
    struct pcpu_block_md chunk_md;
    void *base_addr;
    long unsigned int *alloc_map;
    long unsigned int *bound_map;
    struct pcpu_block_md *md_blocks;
    void *data;
    bool immutable;
    int start_offset;
    int end_offset;
    int nr_pages;
    int nr_populated;
    int nr_empty_pop_pages;
    long unsigned int populated[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct pcpu_chunk {
    struct list_head list;
    int free_bytes;
    struct pcpu_block_md chunk_md;
    void *base_addr;
    long unsigned int *alloc_map;
    long unsigned int *bound_map;
    struct pcpu_block_md *md_blocks;
    void *data;
    bool immutable;
    int start_offset;
    int end_offset;
    int nr_pages;
    int nr_populated;
    int nr_empty_pop_pages;
    long unsigned int populated[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct pcpu_chunk {
    struct list_head list;
    int free_bytes;
    struct pcpu_block_md chunk_md;
    void *base_addr;
    long unsigned int *alloc_map;
    long unsigned int *bound_map;
    struct pcpu_block_md *md_blocks;
    void *data;
    bool immutable;
    int start_offset;
    int end_offset;
    int nr_pages;
    int nr_populated;
    int nr_empty_pop_pages;
    long unsigned int populated[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct pcpu_chunk {
    struct list_head list;
    int free_bytes;
    struct pcpu_block_md chunk_md;
    void *base_addr;
    long unsigned int *alloc_map;
    long unsigned int *bound_map;
    struct pcpu_block_md *md_blocks;
    void *data;
    bool immutable;
    int start_offset;
    int end_offset;
    int nr_pages;
    int nr_populated;
    int nr_empty_pop_pages;
    long unsigned int populated[0];
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
<code>struct list_head map_extend_list</code>
</li>
<li>
<b>Field removed. </b>
<code>struct work_struct map_extend_work</code>
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
<code>bool has_reserved</code>
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
<code>int free_bytes</code>
</li>
<li>
<b>Field added. </b>
<code>int contig_bits</code>
</li>
<li>
<b>Field added. </b>
<code>int contig_bits_start</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int *alloc_map</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int *bound_map</code>
</li>
<li>
<b>Field added. </b>
<code>struct pcpu_block_md *md_blocks</code>
</li>
<li>
<b>Field added. </b>
<code>int first_bit</code>
</li>
<li>
<b>Field added. </b>
<code>int start_offset</code>
</li>
<li>
<b>Field added. </b>
<code>int end_offset</code>
</li>
<li>
<b>Field added. </b>
<code>int nr_pages</code>
</li>
<li>
<b>Field added. </b>
<code>int nr_empty_pop_pages</code>
</li>
<li>
<b>Field removed. </b>
<code>int free_size</code>
</li>
<li>
<b>Field removed. </b>
<code>int contig_hint</code>
</li>
<li>
<b>Field removed. </b>
<code>int map_used</code>
</li>
<li>
<b>Field removed. </b>
<code>int map_alloc</code>
</li>
<li>
<b>Field removed. </b>
<code>int *map</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head map_extend_list</code>
</li>
<li>
<b>Field removed. </b>
<code>int first_free</code>
</li>
<li>
<b>Field removed. </b>
<code>bool has_reserved</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct pcpu_block_md chunk_md</code>
</li>
<li>
<b>Field removed. </b>
<code>int contig_bits</code>
</li>
<li>
<b>Field removed. </b>
<code>int contig_bits_start</code>
</li>
<li>
<b>Field removed. </b>
<code>int first_bit</code>
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
<code>struct obj_cgroup **obj_cgroups</code>
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
<code>bool isolated</code>
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
