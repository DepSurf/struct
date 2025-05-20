# Struct: <code>nd_region</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct nd_region {
    struct device dev;
    struct ida ns_ida;
    struct ida btt_ida;
    struct ida pfn_ida;
    long unsigned int flags;
    struct device *ns_seed;
    struct device *btt_seed;
    struct device *pfn_seed;
    u16 ndr_mappings;
    u64 ndr_size;
    u64 ndr_start;
    int id;
    int num_lanes;
    int ro;
    int numa_node;
    void *provider_data;
    struct nd_interleave_set *nd_set;
    struct nd_percpu_lane *lane;
    struct nd_mapping mapping[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct nd_region {
    struct device dev;
    struct ida ns_ida;
    struct ida btt_ida;
    struct ida pfn_ida;
    struct ida dax_ida;
    long unsigned int flags;
    struct device *ns_seed;
    struct device *btt_seed;
    struct device *pfn_seed;
    struct device *dax_seed;
    u16 ndr_mappings;
    u64 ndr_size;
    u64 ndr_start;
    int id;
    int num_lanes;
    int ro;
    int numa_node;
    void *provider_data;
    struct nd_interleave_set *nd_set;
    struct nd_percpu_lane *lane;
    struct nd_mapping mapping[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct nd_region {
    struct device dev;
    struct ida ns_ida;
    struct ida btt_ida;
    struct ida pfn_ida;
    struct ida dax_ida;
    long unsigned int flags;
    struct device *ns_seed;
    struct device *btt_seed;
    struct device *pfn_seed;
    struct device *dax_seed;
    u16 ndr_mappings;
    u64 ndr_size;
    u64 ndr_start;
    int id;
    int num_lanes;
    int ro;
    int numa_node;
    void *provider_data;
    struct nd_interleave_set *nd_set;
    struct nd_percpu_lane *lane;
    struct nd_mapping mapping[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct nd_region {
    struct device dev;
    struct ida ns_ida;
    struct ida btt_ida;
    struct ida pfn_ida;
    struct ida dax_ida;
    long unsigned int flags;
    struct device *ns_seed;
    struct device *btt_seed;
    struct device *pfn_seed;
    struct device *dax_seed;
    u16 ndr_mappings;
    u64 ndr_size;
    u64 ndr_start;
    int id;
    int num_lanes;
    int ro;
    int numa_node;
    void *provider_data;
    struct kernfs_node *bb_state;
    struct badblocks bb;
    struct nd_interleave_set *nd_set;
    struct nd_percpu_lane *lane;
    struct nd_mapping mapping[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct nd_region {
    struct device dev;
    struct ida ns_ida;
    struct ida btt_ida;
    struct ida pfn_ida;
    struct ida dax_ida;
    long unsigned int flags;
    struct device *ns_seed;
    struct device *btt_seed;
    struct device *pfn_seed;
    struct device *dax_seed;
    u16 ndr_mappings;
    u64 ndr_size;
    u64 ndr_start;
    int id;
    int num_lanes;
    int ro;
    int numa_node;
    void *provider_data;
    struct kernfs_node *bb_state;
    struct badblocks bb;
    struct nd_interleave_set *nd_set;
    struct nd_percpu_lane *lane;
    struct nd_mapping mapping[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct nd_region {
    struct device dev;
    struct ida ns_ida;
    struct ida btt_ida;
    struct ida pfn_ida;
    struct ida dax_ida;
    long unsigned int flags;
    struct device *ns_seed;
    struct device *btt_seed;
    struct device *pfn_seed;
    struct device *dax_seed;
    u16 ndr_mappings;
    u64 ndr_size;
    u64 ndr_start;
    int id;
    int num_lanes;
    int ro;
    int numa_node;
    void *provider_data;
    struct kernfs_node *bb_state;
    struct badblocks bb;
    struct nd_interleave_set *nd_set;
    struct nd_percpu_lane *lane;
    struct nd_mapping mapping[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct nd_region {
    struct device dev;
    struct ida ns_ida;
    struct ida btt_ida;
    struct ida pfn_ida;
    struct ida dax_ida;
    long unsigned int flags;
    struct device *ns_seed;
    struct device *btt_seed;
    struct device *pfn_seed;
    struct device *dax_seed;
    u16 ndr_mappings;
    u64 ndr_size;
    u64 ndr_start;
    int id;
    int num_lanes;
    int ro;
    int numa_node;
    void *provider_data;
    struct kernfs_node *bb_state;
    struct badblocks bb;
    struct nd_interleave_set *nd_set;
    struct nd_percpu_lane *lane;
    struct nd_mapping mapping[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct nd_region {
    struct device dev;
    struct ida ns_ida;
    struct ida btt_ida;
    struct ida pfn_ida;
    struct ida dax_ida;
    long unsigned int flags;
    struct device *ns_seed;
    struct device *btt_seed;
    struct device *pfn_seed;
    struct device *dax_seed;
    u16 ndr_mappings;
    u64 ndr_size;
    u64 ndr_start;
    int id;
    int num_lanes;
    int ro;
    int numa_node;
    int target_node;
    void *provider_data;
    struct kernfs_node *bb_state;
    struct badblocks bb;
    struct nd_interleave_set *nd_set;
    struct nd_percpu_lane *lane;
    int (*flush)(struct nd_region *, struct bio *);
    struct nd_mapping mapping[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct nd_region {
    struct device dev;
    struct ida ns_ida;
    struct ida btt_ida;
    struct ida pfn_ida;
    struct ida dax_ida;
    long unsigned int flags;
    struct device *ns_seed;
    struct device *btt_seed;
    struct device *pfn_seed;
    struct device *dax_seed;
    u16 ndr_mappings;
    u64 ndr_size;
    u64 ndr_start;
    int id;
    int num_lanes;
    int ro;
    int numa_node;
    int target_node;
    void *provider_data;
    struct kernfs_node *bb_state;
    struct badblocks bb;
    struct nd_interleave_set *nd_set;
    struct nd_percpu_lane *lane;
    int (*flush)(struct nd_region *, struct bio *);
    struct nd_mapping mapping[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct nd_region {
    struct device dev;
    struct ida ns_ida;
    struct ida btt_ida;
    struct ida pfn_ida;
    struct ida dax_ida;
    long unsigned int flags;
    struct device *ns_seed;
    struct device *btt_seed;
    struct device *pfn_seed;
    struct device *dax_seed;
    long unsigned int align;
    u16 ndr_mappings;
    u64 ndr_size;
    u64 ndr_start;
    int id;
    int num_lanes;
    int ro;
    int numa_node;
    int target_node;
    void *provider_data;
    struct kernfs_node *bb_state;
    struct badblocks bb;
    struct nd_interleave_set *nd_set;
    struct nd_percpu_lane *lane;
    int (*flush)(struct nd_region *, struct bio *);
    struct nd_mapping mapping[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct nd_region {
    struct device dev;
    struct ida ns_ida;
    struct ida btt_ida;
    struct ida pfn_ida;
    struct ida dax_ida;
    long unsigned int flags;
    struct device *ns_seed;
    struct device *btt_seed;
    struct device *pfn_seed;
    struct device *dax_seed;
    long unsigned int align;
    u16 ndr_mappings;
    u64 ndr_size;
    u64 ndr_start;
    int id;
    int num_lanes;
    int ro;
    int numa_node;
    int target_node;
    void *provider_data;
    struct kernfs_node *bb_state;
    struct badblocks bb;
    struct nd_interleave_set *nd_set;
    struct nd_percpu_lane *lane;
    int (*flush)(struct nd_region *, struct bio *);
    struct nd_mapping mapping[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct nd_region {
    struct device dev;
    struct ida ns_ida;
    struct ida btt_ida;
    struct ida pfn_ida;
    struct ida dax_ida;
    long unsigned int flags;
    struct device *ns_seed;
    struct device *btt_seed;
    struct device *pfn_seed;
    struct device *dax_seed;
    long unsigned int align;
    u16 ndr_mappings;
    u64 ndr_size;
    u64 ndr_start;
    int id;
    int num_lanes;
    int ro;
    int numa_node;
    int target_node;
    void *provider_data;
    struct kernfs_node *bb_state;
    struct badblocks bb;
    struct nd_interleave_set *nd_set;
    struct nd_percpu_lane *lane;
    int (*flush)(struct nd_region *, struct bio *);
    struct nd_mapping mapping[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct nd_region {
    struct device dev;
    struct ida ns_ida;
    struct ida btt_ida;
    struct ida pfn_ida;
    struct ida dax_ida;
    long unsigned int flags;
    struct device *ns_seed;
    struct device *btt_seed;
    struct device *pfn_seed;
    struct device *dax_seed;
    long unsigned int align;
    u16 ndr_mappings;
    u64 ndr_size;
    u64 ndr_start;
    int id;
    int num_lanes;
    int ro;
    int numa_node;
    int target_node;
    void *provider_data;
    struct kernfs_node *bb_state;
    struct badblocks bb;
    struct nd_interleave_set *nd_set;
    struct nd_percpu_lane *lane;
    int (*flush)(struct nd_region *, struct bio *);
    struct nd_mapping mapping[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct nd_region {
    struct device dev;
    struct ida ns_ida;
    struct ida btt_ida;
    struct ida pfn_ida;
    struct ida dax_ida;
    long unsigned int flags;
    struct device *ns_seed;
    struct device *btt_seed;
    struct device *pfn_seed;
    struct device *dax_seed;
    long unsigned int align;
    u16 ndr_mappings;
    u64 ndr_size;
    u64 ndr_start;
    int id;
    int num_lanes;
    int ro;
    int numa_node;
    int target_node;
    void *provider_data;
    struct kernfs_node *bb_state;
    struct badblocks bb;
    struct nd_interleave_set *nd_set;
    struct nd_percpu_lane *lane;
    int (*flush)(struct nd_region *, struct bio *);
    struct nd_mapping mapping[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct nd_region {
    struct device dev;
    struct ida ns_ida;
    struct ida btt_ida;
    struct ida pfn_ida;
    struct ida dax_ida;
    long unsigned int flags;
    struct device *ns_seed;
    struct device *btt_seed;
    struct device *pfn_seed;
    struct device *dax_seed;
    long unsigned int align;
    u16 ndr_mappings;
    u64 ndr_size;
    u64 ndr_start;
    int id;
    int num_lanes;
    int ro;
    int numa_node;
    int target_node;
    void *provider_data;
    struct kernfs_node *bb_state;
    struct badblocks bb;
    struct nd_interleave_set *nd_set;
    struct nd_percpu_lane *lane;
    int (*flush)(struct nd_region *, struct bio *);
    struct nd_mapping mapping[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct nd_region {
    struct device dev;
    struct ida ns_ida;
    struct ida btt_ida;
    struct ida pfn_ida;
    struct ida dax_ida;
    long unsigned int flags;
    struct device *ns_seed;
    struct device *btt_seed;
    struct device *pfn_seed;
    struct device *dax_seed;
    long unsigned int align;
    u16 ndr_mappings;
    u64 ndr_size;
    u64 ndr_start;
    int id;
    int num_lanes;
    int ro;
    int numa_node;
    int target_node;
    void *provider_data;
    struct kernfs_node *bb_state;
    struct badblocks bb;
    struct nd_interleave_set *nd_set;
    struct nd_percpu_lane *lane;
    int (*flush)(struct nd_region *, struct bio *);
    struct nd_mapping mapping[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct nd_region {
    struct device dev;
    struct ida ns_ida;
    struct ida btt_ida;
    struct ida pfn_ida;
    struct ida dax_ida;
    long unsigned int flags;
    struct device *ns_seed;
    struct device *btt_seed;
    struct device *pfn_seed;
    struct device *dax_seed;
    long unsigned int align;
    u16 ndr_mappings;
    u64 ndr_size;
    u64 ndr_start;
    int id;
    int num_lanes;
    int ro;
    int numa_node;
    int target_node;
    void *provider_data;
    struct kernfs_node *bb_state;
    struct badblocks bb;
    struct nd_interleave_set *nd_set;
    struct nd_percpu_lane *lane;
    int (*flush)(struct nd_region *, struct bio *);
    struct nd_mapping mapping[0];
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
struct nd_region {
    struct device dev;
    struct ida ns_ida;
    struct ida btt_ida;
    struct ida pfn_ida;
    struct ida dax_ida;
    long unsigned int flags;
    struct device *ns_seed;
    struct device *btt_seed;
    struct device *pfn_seed;
    struct device *dax_seed;
    u16 ndr_mappings;
    u64 ndr_size;
    u64 ndr_start;
    int id;
    int num_lanes;
    int ro;
    int numa_node;
    int target_node;
    void *provider_data;
    struct kernfs_node *bb_state;
    struct badblocks bb;
    struct nd_interleave_set *nd_set;
    struct nd_percpu_lane *lane;
    int (*flush)(struct nd_region *, struct bio *);
    struct nd_mapping mapping[0];
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
struct nd_region {
    struct device dev;
    struct ida ns_ida;
    struct ida btt_ida;
    struct ida pfn_ida;
    struct ida dax_ida;
    long unsigned int flags;
    struct device *ns_seed;
    struct device *btt_seed;
    struct device *pfn_seed;
    struct device *dax_seed;
    u16 ndr_mappings;
    u64 ndr_size;
    u64 ndr_start;
    int id;
    int num_lanes;
    int ro;
    int numa_node;
    int target_node;
    void *provider_data;
    struct kernfs_node *bb_state;
    struct badblocks bb;
    struct nd_interleave_set *nd_set;
    struct nd_percpu_lane *lane;
    int (*flush)(struct nd_region *, struct bio *);
    struct nd_mapping mapping[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct nd_region {
    struct device dev;
    struct ida ns_ida;
    struct ida btt_ida;
    struct ida pfn_ida;
    struct ida dax_ida;
    long unsigned int flags;
    struct device *ns_seed;
    struct device *btt_seed;
    struct device *pfn_seed;
    struct device *dax_seed;
    u16 ndr_mappings;
    u64 ndr_size;
    u64 ndr_start;
    int id;
    int num_lanes;
    int ro;
    int numa_node;
    int target_node;
    void *provider_data;
    struct kernfs_node *bb_state;
    struct badblocks bb;
    struct nd_interleave_set *nd_set;
    struct nd_percpu_lane *lane;
    int (*flush)(struct nd_region *, struct bio *);
    struct nd_mapping mapping[0];
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
struct nd_region {
    struct device dev;
    struct ida ns_ida;
    struct ida btt_ida;
    struct ida pfn_ida;
    struct ida dax_ida;
    long unsigned int flags;
    struct device *ns_seed;
    struct device *btt_seed;
    struct device *pfn_seed;
    struct device *dax_seed;
    u16 ndr_mappings;
    u64 ndr_size;
    u64 ndr_start;
    int id;
    int num_lanes;
    int ro;
    int numa_node;
    int target_node;
    void *provider_data;
    struct kernfs_node *bb_state;
    struct badblocks bb;
    struct nd_interleave_set *nd_set;
    struct nd_percpu_lane *lane;
    int (*flush)(struct nd_region *, struct bio *);
    struct nd_mapping mapping[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct nd_region {
    struct device dev;
    struct ida ns_ida;
    struct ida btt_ida;
    struct ida pfn_ida;
    struct ida dax_ida;
    long unsigned int flags;
    struct device *ns_seed;
    struct device *btt_seed;
    struct device *pfn_seed;
    struct device *dax_seed;
    u16 ndr_mappings;
    u64 ndr_size;
    u64 ndr_start;
    int id;
    int num_lanes;
    int ro;
    int numa_node;
    int target_node;
    void *provider_data;
    struct kernfs_node *bb_state;
    struct badblocks bb;
    struct nd_interleave_set *nd_set;
    struct nd_percpu_lane *lane;
    int (*flush)(struct nd_region *, struct bio *);
    struct nd_mapping mapping[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct nd_region {
    struct device dev;
    struct ida ns_ida;
    struct ida btt_ida;
    struct ida pfn_ida;
    struct ida dax_ida;
    long unsigned int flags;
    struct device *ns_seed;
    struct device *btt_seed;
    struct device *pfn_seed;
    struct device *dax_seed;
    u16 ndr_mappings;
    u64 ndr_size;
    u64 ndr_start;
    int id;
    int num_lanes;
    int ro;
    int numa_node;
    int target_node;
    void *provider_data;
    struct kernfs_node *bb_state;
    struct badblocks bb;
    struct nd_interleave_set *nd_set;
    struct nd_percpu_lane *lane;
    int (*flush)(struct nd_region *, struct bio *);
    struct nd_mapping mapping[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct nd_region {
    struct device dev;
    struct ida ns_ida;
    struct ida btt_ida;
    struct ida pfn_ida;
    struct ida dax_ida;
    long unsigned int flags;
    struct device *ns_seed;
    struct device *btt_seed;
    struct device *pfn_seed;
    struct device *dax_seed;
    u16 ndr_mappings;
    u64 ndr_size;
    u64 ndr_start;
    int id;
    int num_lanes;
    int ro;
    int numa_node;
    int target_node;
    void *provider_data;
    struct kernfs_node *bb_state;
    struct badblocks bb;
    struct nd_interleave_set *nd_set;
    struct nd_percpu_lane *lane;
    int (*flush)(struct nd_region *, struct bio *);
    struct nd_mapping mapping[0];
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
<code>struct ida dax_ida</code>
</li>
<li>
<b>Field added. </b>
<code>struct device *dax_seed</code>
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
<code>struct kernfs_node *bb_state</code>
</li>
<li>
<b>Field added. </b>
<code>struct badblocks bb</code>
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int target_node</code>
</li>
<li>
<b>Field added. </b>
<code>int (*flush)(struct nd_region *, struct bio *)</code>
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
<code>long unsigned int align</code>
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
