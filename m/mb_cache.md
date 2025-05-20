# Struct: <code>mb_cache</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct mb_cache {
    struct list_head c_cache_list;
    const char *c_name;
    atomic_t c_entry_count;
    int c_max_entries;
    int c_bucket_bits;
    struct kmem_cache *c_entry_cache;
    struct hlist_bl_head *c_block_hash;
    struct hlist_bl_head *c_index_hash;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct mb_cache {
    struct hlist_bl_head *c_hash;
    int c_bucket_bits;
    int c_max_entries;
    spinlock_t c_list_lock;
    struct list_head c_list;
    long unsigned int c_entry_count;
    struct shrinker c_shrink;
    struct work_struct c_shrink_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct mb_cache {
    struct hlist_bl_head *c_hash;
    int c_bucket_bits;
    long unsigned int c_max_entries;
    spinlock_t c_list_lock;
    struct list_head c_list;
    long unsigned int c_entry_count;
    struct shrinker c_shrink;
    struct work_struct c_shrink_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct mb_cache {
    struct hlist_bl_head *c_hash;
    int c_bucket_bits;
    long unsigned int c_max_entries;
    spinlock_t c_list_lock;
    struct list_head c_list;
    long unsigned int c_entry_count;
    struct shrinker c_shrink;
    struct work_struct c_shrink_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct mb_cache {
    struct hlist_bl_head *c_hash;
    int c_bucket_bits;
    long unsigned int c_max_entries;
    spinlock_t c_list_lock;
    struct list_head c_list;
    long unsigned int c_entry_count;
    struct shrinker c_shrink;
    struct work_struct c_shrink_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct mb_cache {
    struct hlist_bl_head *c_hash;
    int c_bucket_bits;
    long unsigned int c_max_entries;
    spinlock_t c_list_lock;
    struct list_head c_list;
    long unsigned int c_entry_count;
    struct shrinker c_shrink;
    struct work_struct c_shrink_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct mb_cache {
    struct hlist_bl_head *c_hash;
    int c_bucket_bits;
    long unsigned int c_max_entries;
    spinlock_t c_list_lock;
    struct list_head c_list;
    long unsigned int c_entry_count;
    struct shrinker c_shrink;
    struct work_struct c_shrink_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct mb_cache {
    struct hlist_bl_head *c_hash;
    int c_bucket_bits;
    long unsigned int c_max_entries;
    spinlock_t c_list_lock;
    struct list_head c_list;
    long unsigned int c_entry_count;
    struct shrinker c_shrink;
    struct work_struct c_shrink_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct mb_cache {
    struct hlist_bl_head *c_hash;
    int c_bucket_bits;
    long unsigned int c_max_entries;
    spinlock_t c_list_lock;
    struct list_head c_list;
    long unsigned int c_entry_count;
    struct shrinker c_shrink;
    struct work_struct c_shrink_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct mb_cache {
    struct hlist_bl_head *c_hash;
    int c_bucket_bits;
    long unsigned int c_max_entries;
    spinlock_t c_list_lock;
    struct list_head c_list;
    long unsigned int c_entry_count;
    struct shrinker c_shrink;
    struct work_struct c_shrink_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mb_cache {
    struct hlist_bl_head *c_hash;
    int c_bucket_bits;
    long unsigned int c_max_entries;
    spinlock_t c_list_lock;
    struct list_head c_list;
    long unsigned int c_entry_count;
    struct shrinker c_shrink;
    struct work_struct c_shrink_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mb_cache {
    struct hlist_bl_head *c_hash;
    int c_bucket_bits;
    long unsigned int c_max_entries;
    spinlock_t c_list_lock;
    struct list_head c_list;
    long unsigned int c_entry_count;
    struct shrinker c_shrink;
    struct work_struct c_shrink_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mb_cache {
    struct hlist_bl_head *c_hash;
    int c_bucket_bits;
    long unsigned int c_max_entries;
    spinlock_t c_list_lock;
    struct list_head c_list;
    long unsigned int c_entry_count;
    struct shrinker c_shrink;
    struct work_struct c_shrink_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mb_cache {
    struct hlist_bl_head *c_hash;
    int c_bucket_bits;
    long unsigned int c_max_entries;
    spinlock_t c_list_lock;
    struct list_head c_list;
    long unsigned int c_entry_count;
    struct shrinker c_shrink;
    struct work_struct c_shrink_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mb_cache {
    struct hlist_bl_head *c_hash;
    int c_bucket_bits;
    long unsigned int c_max_entries;
    spinlock_t c_list_lock;
    struct list_head c_list;
    long unsigned int c_entry_count;
    struct shrinker c_shrink;
    struct work_struct c_shrink_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mb_cache {
    struct hlist_bl_head *c_hash;
    int c_bucket_bits;
    long unsigned int c_max_entries;
    spinlock_t c_list_lock;
    struct list_head c_list;
    long unsigned int c_entry_count;
    struct shrinker c_shrink;
    struct work_struct c_shrink_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mb_cache {
    struct hlist_bl_head *c_hash;
    int c_bucket_bits;
    long unsigned int c_max_entries;
    spinlock_t c_list_lock;
    struct list_head c_list;
    long unsigned int c_entry_count;
    struct shrinker *c_shrink;
    struct work_struct c_shrink_work;
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
struct mb_cache {
    struct hlist_bl_head *c_hash;
    int c_bucket_bits;
    long unsigned int c_max_entries;
    spinlock_t c_list_lock;
    struct list_head c_list;
    long unsigned int c_entry_count;
    struct shrinker c_shrink;
    struct work_struct c_shrink_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mb_cache {
    struct hlist_bl_head *c_hash;
    int c_bucket_bits;
    long unsigned int c_max_entries;
    spinlock_t c_list_lock;
    struct list_head c_list;
    long unsigned int c_entry_count;
    struct shrinker c_shrink;
    struct work_struct c_shrink_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct mb_cache {
    struct hlist_bl_head *c_hash;
    int c_bucket_bits;
    long unsigned int c_max_entries;
    spinlock_t c_list_lock;
    struct list_head c_list;
    long unsigned int c_entry_count;
    struct shrinker c_shrink;
    struct work_struct c_shrink_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct mb_cache {
    struct hlist_bl_head *c_hash;
    int c_bucket_bits;
    long unsigned int c_max_entries;
    spinlock_t c_list_lock;
    struct list_head c_list;
    long unsigned int c_entry_count;
    struct shrinker c_shrink;
    struct work_struct c_shrink_work;
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
struct mb_cache {
    struct hlist_bl_head *c_hash;
    int c_bucket_bits;
    long unsigned int c_max_entries;
    spinlock_t c_list_lock;
    struct list_head c_list;
    long unsigned int c_entry_count;
    struct shrinker c_shrink;
    struct work_struct c_shrink_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct mb_cache {
    struct hlist_bl_head *c_hash;
    int c_bucket_bits;
    long unsigned int c_max_entries;
    spinlock_t c_list_lock;
    struct list_head c_list;
    long unsigned int c_entry_count;
    struct shrinker c_shrink;
    struct work_struct c_shrink_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct mb_cache {
    struct hlist_bl_head *c_hash;
    int c_bucket_bits;
    long unsigned int c_max_entries;
    spinlock_t c_list_lock;
    struct list_head c_list;
    long unsigned int c_entry_count;
    struct shrinker c_shrink;
    struct work_struct c_shrink_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct mb_cache {
    struct hlist_bl_head *c_hash;
    int c_bucket_bits;
    long unsigned int c_max_entries;
    spinlock_t c_list_lock;
    struct list_head c_list;
    long unsigned int c_entry_count;
    struct shrinker c_shrink;
    struct work_struct c_shrink_work;
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
<code>struct hlist_bl_head *c_hash</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t c_list_lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head c_list</code>
</li>
<li>
<b>Field added. </b>
<code>struct shrinker c_shrink</code>
</li>
<li>
<b>Field added. </b>
<code>struct work_struct c_shrink_work</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head c_cache_list</code>
</li>
<li>
<b>Field removed. </b>
<code>const char *c_name</code>
</li>
<li>
<b>Field removed. </b>
<code>struct kmem_cache *c_entry_cache</code>
</li>
<li>
<b>Field removed. </b>
<code>struct hlist_bl_head *c_block_hash</code>
</li>
<li>
<b>Field removed. </b>
<code>struct hlist_bl_head *c_index_hash</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_t c_entry_count</code> ➡️ <code>long unsigned int c_entry_count</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int c_max_entries</code> ➡️ <code>long unsigned int c_max_entries</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct shrinker c_shrink</code> ➡️ <code>struct shrinker *c_shrink</code>
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
