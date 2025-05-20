# Struct: <code>ext4_group_info</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct ext4_group_info {
    long unsigned int bb_state;
    struct rb_root bb_free_root;
    ext4_grpblk_t bb_first_free;
    ext4_grpblk_t bb_free;
    ext4_grpblk_t bb_fragments;
    ext4_grpblk_t bb_largest_free_order;
    struct list_head bb_prealloc_list;
    struct rw_semaphore alloc_sem;
    ext4_grpblk_t bb_counters[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ext4_group_info {
    long unsigned int bb_state;
    struct rb_root bb_free_root;
    ext4_grpblk_t bb_first_free;
    ext4_grpblk_t bb_free;
    ext4_grpblk_t bb_fragments;
    ext4_grpblk_t bb_largest_free_order;
    struct list_head bb_prealloc_list;
    struct rw_semaphore alloc_sem;
    ext4_grpblk_t bb_counters[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ext4_group_info {
    long unsigned int bb_state;
    struct rb_root bb_free_root;
    ext4_grpblk_t bb_first_free;
    ext4_grpblk_t bb_free;
    ext4_grpblk_t bb_fragments;
    ext4_grpblk_t bb_largest_free_order;
    struct list_head bb_prealloc_list;
    struct rw_semaphore alloc_sem;
    ext4_grpblk_t bb_counters[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ext4_group_info {
    long unsigned int bb_state;
    struct rb_root bb_free_root;
    ext4_grpblk_t bb_first_free;
    ext4_grpblk_t bb_free;
    ext4_grpblk_t bb_fragments;
    ext4_grpblk_t bb_largest_free_order;
    struct list_head bb_prealloc_list;
    struct rw_semaphore alloc_sem;
    ext4_grpblk_t bb_counters[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ext4_group_info {
    long unsigned int bb_state;
    struct rb_root bb_free_root;
    ext4_grpblk_t bb_first_free;
    ext4_grpblk_t bb_free;
    ext4_grpblk_t bb_fragments;
    ext4_grpblk_t bb_largest_free_order;
    struct list_head bb_prealloc_list;
    struct rw_semaphore alloc_sem;
    ext4_grpblk_t bb_counters[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ext4_group_info {
    long unsigned int bb_state;
    struct rb_root bb_free_root;
    ext4_grpblk_t bb_first_free;
    ext4_grpblk_t bb_free;
    ext4_grpblk_t bb_fragments;
    ext4_grpblk_t bb_largest_free_order;
    struct list_head bb_prealloc_list;
    struct rw_semaphore alloc_sem;
    ext4_grpblk_t bb_counters[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ext4_group_info {
    long unsigned int bb_state;
    struct rb_root bb_free_root;
    ext4_grpblk_t bb_first_free;
    ext4_grpblk_t bb_free;
    ext4_grpblk_t bb_fragments;
    ext4_grpblk_t bb_largest_free_order;
    struct list_head bb_prealloc_list;
    struct rw_semaphore alloc_sem;
    ext4_grpblk_t bb_counters[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ext4_group_info {
    long unsigned int bb_state;
    struct rb_root bb_free_root;
    ext4_grpblk_t bb_first_free;
    ext4_grpblk_t bb_free;
    ext4_grpblk_t bb_fragments;
    ext4_grpblk_t bb_largest_free_order;
    struct list_head bb_prealloc_list;
    struct rw_semaphore alloc_sem;
    ext4_grpblk_t bb_counters[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ext4_group_info {
    long unsigned int bb_state;
    struct rb_root bb_free_root;
    ext4_grpblk_t bb_first_free;
    ext4_grpblk_t bb_free;
    ext4_grpblk_t bb_fragments;
    ext4_grpblk_t bb_largest_free_order;
    struct list_head bb_prealloc_list;
    struct rw_semaphore alloc_sem;
    ext4_grpblk_t bb_counters[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ext4_group_info {
    long unsigned int bb_state;
    struct rb_root bb_free_root;
    ext4_grpblk_t bb_first_free;
    ext4_grpblk_t bb_free;
    ext4_grpblk_t bb_fragments;
    ext4_grpblk_t bb_largest_free_order;
    struct list_head bb_prealloc_list;
    struct rw_semaphore alloc_sem;
    ext4_grpblk_t bb_counters[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ext4_group_info {
    long unsigned int bb_state;
    struct rb_root bb_free_root;
    ext4_grpblk_t bb_first_free;
    ext4_grpblk_t bb_free;
    ext4_grpblk_t bb_fragments;
    ext4_grpblk_t bb_largest_free_order;
    struct list_head bb_prealloc_list;
    struct rw_semaphore alloc_sem;
    ext4_grpblk_t bb_counters[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ext4_group_info {
    long unsigned int bb_state;
    struct rb_root bb_free_root;
    ext4_grpblk_t bb_first_free;
    ext4_grpblk_t bb_free;
    ext4_grpblk_t bb_fragments;
    ext4_grpblk_t bb_largest_free_order;
    ext4_group_t bb_group;
    struct list_head bb_prealloc_list;
    struct rw_semaphore alloc_sem;
    struct rb_node bb_avg_fragment_size_rb;
    struct list_head bb_largest_free_order_node;
    ext4_grpblk_t bb_counters[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ext4_group_info {
    long unsigned int bb_state;
    struct rb_root bb_free_root;
    ext4_grpblk_t bb_first_free;
    ext4_grpblk_t bb_free;
    ext4_grpblk_t bb_fragments;
    ext4_grpblk_t bb_largest_free_order;
    ext4_group_t bb_group;
    struct list_head bb_prealloc_list;
    struct rw_semaphore alloc_sem;
    struct rb_node bb_avg_fragment_size_rb;
    struct list_head bb_largest_free_order_node;
    ext4_grpblk_t bb_counters[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ext4_group_info {
    long unsigned int bb_state;
    struct rb_root bb_free_root;
    ext4_grpblk_t bb_first_free;
    ext4_grpblk_t bb_free;
    ext4_grpblk_t bb_fragments;
    ext4_grpblk_t bb_largest_free_order;
    ext4_group_t bb_group;
    struct list_head bb_prealloc_list;
    struct rw_semaphore alloc_sem;
    struct rb_node bb_avg_fragment_size_rb;
    struct list_head bb_largest_free_order_node;
    ext4_grpblk_t bb_counters[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ext4_group_info {
    long unsigned int bb_state;
    struct rb_root bb_free_root;
    ext4_grpblk_t bb_first_free;
    ext4_grpblk_t bb_free;
    ext4_grpblk_t bb_fragments;
    int bb_avg_fragment_size_order;
    ext4_grpblk_t bb_largest_free_order;
    ext4_group_t bb_group;
    struct list_head bb_prealloc_list;
    struct rw_semaphore alloc_sem;
    struct list_head bb_avg_fragment_size_node;
    struct list_head bb_largest_free_order_node;
    ext4_grpblk_t bb_counters[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ext4_group_info {
    long unsigned int bb_state;
    struct rb_root bb_free_root;
    ext4_grpblk_t bb_first_free;
    ext4_grpblk_t bb_free;
    ext4_grpblk_t bb_fragments;
    int bb_avg_fragment_size_order;
    ext4_grpblk_t bb_largest_free_order;
    ext4_group_t bb_group;
    struct list_head bb_prealloc_list;
    struct rw_semaphore alloc_sem;
    struct list_head bb_avg_fragment_size_node;
    struct list_head bb_largest_free_order_node;
    ext4_grpblk_t bb_counters[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ext4_group_info {
    long unsigned int bb_state;
    struct rb_root bb_free_root;
    ext4_grpblk_t bb_first_free;
    ext4_grpblk_t bb_free;
    ext4_grpblk_t bb_fragments;
    int bb_avg_fragment_size_order;
    ext4_grpblk_t bb_largest_free_order;
    ext4_group_t bb_group;
    struct list_head bb_prealloc_list;
    struct rw_semaphore alloc_sem;
    struct list_head bb_avg_fragment_size_node;
    struct list_head bb_largest_free_order_node;
    ext4_grpblk_t bb_counters[0];
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
struct ext4_group_info {
    long unsigned int bb_state;
    struct rb_root bb_free_root;
    ext4_grpblk_t bb_first_free;
    ext4_grpblk_t bb_free;
    ext4_grpblk_t bb_fragments;
    ext4_grpblk_t bb_largest_free_order;
    struct list_head bb_prealloc_list;
    struct rw_semaphore alloc_sem;
    ext4_grpblk_t bb_counters[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ext4_group_info {
    long unsigned int bb_state;
    struct rb_root bb_free_root;
    ext4_grpblk_t bb_first_free;
    ext4_grpblk_t bb_free;
    ext4_grpblk_t bb_fragments;
    ext4_grpblk_t bb_largest_free_order;
    struct list_head bb_prealloc_list;
    struct rw_semaphore alloc_sem;
    ext4_grpblk_t bb_counters[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ext4_group_info {
    long unsigned int bb_state;
    struct rb_root bb_free_root;
    ext4_grpblk_t bb_first_free;
    ext4_grpblk_t bb_free;
    ext4_grpblk_t bb_fragments;
    ext4_grpblk_t bb_largest_free_order;
    struct list_head bb_prealloc_list;
    struct rw_semaphore alloc_sem;
    ext4_grpblk_t bb_counters[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ext4_group_info {
    long unsigned int bb_state;
    struct rb_root bb_free_root;
    ext4_grpblk_t bb_first_free;
    ext4_grpblk_t bb_free;
    ext4_grpblk_t bb_fragments;
    ext4_grpblk_t bb_largest_free_order;
    struct list_head bb_prealloc_list;
    struct rw_semaphore alloc_sem;
    ext4_grpblk_t bb_counters[0];
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
struct ext4_group_info {
    long unsigned int bb_state;
    struct rb_root bb_free_root;
    ext4_grpblk_t bb_first_free;
    ext4_grpblk_t bb_free;
    ext4_grpblk_t bb_fragments;
    ext4_grpblk_t bb_largest_free_order;
    struct list_head bb_prealloc_list;
    struct rw_semaphore alloc_sem;
    ext4_grpblk_t bb_counters[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ext4_group_info {
    long unsigned int bb_state;
    struct rb_root bb_free_root;
    ext4_grpblk_t bb_first_free;
    ext4_grpblk_t bb_free;
    ext4_grpblk_t bb_fragments;
    ext4_grpblk_t bb_largest_free_order;
    struct list_head bb_prealloc_list;
    struct rw_semaphore alloc_sem;
    ext4_grpblk_t bb_counters[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ext4_group_info {
    long unsigned int bb_state;
    struct rb_root bb_free_root;
    ext4_grpblk_t bb_first_free;
    ext4_grpblk_t bb_free;
    ext4_grpblk_t bb_fragments;
    ext4_grpblk_t bb_largest_free_order;
    struct list_head bb_prealloc_list;
    struct rw_semaphore alloc_sem;
    ext4_grpblk_t bb_counters[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ext4_group_info {
    long unsigned int bb_state;
    struct rb_root bb_free_root;
    ext4_grpblk_t bb_first_free;
    ext4_grpblk_t bb_free;
    ext4_grpblk_t bb_fragments;
    ext4_grpblk_t bb_largest_free_order;
    struct list_head bb_prealloc_list;
    struct rw_semaphore alloc_sem;
    ext4_grpblk_t bb_counters[0];
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
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>ext4_group_t bb_group</code>
</li>
<li>
<b>Field added. </b>
<code>struct rb_node bb_avg_fragment_size_rb</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head bb_largest_free_order_node</code>
</li>
</ul>
</details>
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
<code>int bb_avg_fragment_size_order</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head bb_avg_fragment_size_node</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rb_node bb_avg_fragment_size_rb</code>
</li>
</ul>
</details>
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
