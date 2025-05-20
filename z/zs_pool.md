# Struct: <code>zs_pool</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct zs_pool {
    const char *name;
    struct size_class **size_class;
    struct kmem_cache *handle_cachep;
    gfp_t flags;
    atomic_long_t pages_allocated;
    struct zs_pool_stats stats;
    struct shrinker shrinker;
    bool shrinker_enabled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct zs_pool {
    const char *name;
    struct size_class **size_class;
    struct kmem_cache *handle_cachep;
    struct kmem_cache *zspage_cachep;
    atomic_long_t pages_allocated;
    struct zs_pool_stats stats;
    struct shrinker shrinker;
    bool shrinker_enabled;
    struct inode *inode;
    struct work_struct free_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct zs_pool {
    const char *name;
    struct size_class **size_class;
    struct kmem_cache *handle_cachep;
    struct kmem_cache *zspage_cachep;
    atomic_long_t pages_allocated;
    struct zs_pool_stats stats;
    struct shrinker shrinker;
    bool shrinker_enabled;
    struct inode *inode;
    struct work_struct free_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct zs_pool {
    const char *name;
    struct size_class * size_class[255];
    struct kmem_cache *handle_cachep;
    struct kmem_cache *zspage_cachep;
    atomic_long_t pages_allocated;
    struct zs_pool_stats stats;
    struct shrinker shrinker;
    bool shrinker_enabled;
    struct inode *inode;
    struct work_struct free_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct zs_pool {
    const char *name;
    struct size_class * size_class[255];
    struct kmem_cache *handle_cachep;
    struct kmem_cache *zspage_cachep;
    atomic_long_t pages_allocated;
    struct zs_pool_stats stats;
    struct shrinker shrinker;
    bool shrinker_enabled;
    struct inode *inode;
    struct work_struct free_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct zs_pool {
    const char *name;
    struct size_class * size_class[255];
    struct kmem_cache *handle_cachep;
    struct kmem_cache *zspage_cachep;
    atomic_long_t pages_allocated;
    struct zs_pool_stats stats;
    struct shrinker shrinker;
    struct inode *inode;
    struct work_struct free_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct zs_pool {
    const char *name;
    struct size_class * size_class[255];
    struct kmem_cache *handle_cachep;
    struct kmem_cache *zspage_cachep;
    atomic_long_t pages_allocated;
    struct zs_pool_stats stats;
    struct shrinker shrinker;
    struct inode *inode;
    struct work_struct free_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct zs_pool {
    const char *name;
    struct size_class * size_class[255];
    struct kmem_cache *handle_cachep;
    struct kmem_cache *zspage_cachep;
    atomic_long_t pages_allocated;
    struct zs_pool_stats stats;
    struct shrinker shrinker;
    struct inode *inode;
    struct work_struct free_work;
    struct wait_queue_head migration_wait;
    atomic_long_t isolated_pages;
    bool destroying;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct zs_pool {
    const char *name;
    struct size_class * size_class[255];
    struct kmem_cache *handle_cachep;
    struct kmem_cache *zspage_cachep;
    atomic_long_t pages_allocated;
    struct zs_pool_stats stats;
    struct shrinker shrinker;
    struct inode *inode;
    struct work_struct free_work;
    struct wait_queue_head migration_wait;
    atomic_long_t isolated_pages;
    bool destroying;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct zs_pool {
    const char *name;
    struct size_class * size_class[255];
    struct kmem_cache *handle_cachep;
    struct kmem_cache *zspage_cachep;
    atomic_long_t pages_allocated;
    struct zs_pool_stats stats;
    struct shrinker shrinker;
    struct inode *inode;
    struct work_struct free_work;
    struct wait_queue_head migration_wait;
    atomic_long_t isolated_pages;
    bool destroying;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct zs_pool {
    const char *name;
    struct size_class * size_class[255];
    struct kmem_cache *handle_cachep;
    struct kmem_cache *zspage_cachep;
    atomic_long_t pages_allocated;
    struct zs_pool_stats stats;
    struct shrinker shrinker;
    struct inode *inode;
    struct work_struct free_work;
    struct wait_queue_head migration_wait;
    atomic_long_t isolated_pages;
    bool destroying;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct zs_pool {
    const char *name;
    struct size_class * size_class[255];
    struct kmem_cache *handle_cachep;
    struct kmem_cache *zspage_cachep;
    atomic_long_t pages_allocated;
    struct zs_pool_stats stats;
    struct shrinker shrinker;
    struct inode *inode;
    struct work_struct free_work;
    struct wait_queue_head migration_wait;
    atomic_long_t isolated_pages;
    bool destroying;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct zs_pool {
    const char *name;
    struct size_class * size_class[255];
    struct kmem_cache *handle_cachep;
    struct kmem_cache *zspage_cachep;
    atomic_long_t pages_allocated;
    struct zs_pool_stats stats;
    struct shrinker shrinker;
    struct inode *inode;
    struct work_struct free_work;
    struct wait_queue_head migration_wait;
    atomic_long_t isolated_pages;
    bool destroying;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct zs_pool {
    const char *name;
    struct size_class * size_class[255];
    struct kmem_cache *handle_cachep;
    struct kmem_cache *zspage_cachep;
    atomic_long_t pages_allocated;
    struct zs_pool_stats stats;
    struct shrinker shrinker;
    struct inode *inode;
    struct work_struct free_work;
    rwlock_t migrate_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct zs_pool {
    const char *name;
    struct size_class * size_class[255];
    struct kmem_cache *handle_cachep;
    struct kmem_cache *zspage_cachep;
    atomic_long_t pages_allocated;
    struct zs_pool_stats stats;
    struct shrinker shrinker;
    struct list_head lru;
    struct zpool *zpool;
    const struct zpool_ops *zpool_ops;
    struct work_struct free_work;
    spinlock_t lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct zs_pool {
    const char *name;
    struct size_class * size_class[255];
    struct kmem_cache *handle_cachep;
    struct kmem_cache *zspage_cachep;
    atomic_long_t pages_allocated;
    struct zs_pool_stats stats;
    struct shrinker shrinker;
    struct work_struct free_work;
    spinlock_t lock;
    atomic_t compaction_in_progress;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct zs_pool {
    const char *name;
    struct size_class * size_class[255];
    struct kmem_cache *handle_cachep;
    struct kmem_cache *zspage_cachep;
    atomic_long_t pages_allocated;
    struct zs_pool_stats stats;
    struct shrinker *shrinker;
    struct work_struct free_work;
    spinlock_t lock;
    atomic_t compaction_in_progress;
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
struct zs_pool {
    const char *name;
    struct size_class * size_class[255];
    struct kmem_cache *handle_cachep;
    struct kmem_cache *zspage_cachep;
    atomic_long_t pages_allocated;
    struct zs_pool_stats stats;
    struct shrinker shrinker;
    struct inode *inode;
    struct work_struct free_work;
    struct wait_queue_head migration_wait;
    atomic_long_t isolated_pages;
    bool destroying;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct zs_pool {
    const char *name;
    struct size_class * size_class[255];
    struct kmem_cache *handle_cachep;
    struct kmem_cache *zspage_cachep;
    atomic_long_t pages_allocated;
    struct zs_pool_stats stats;
    struct shrinker shrinker;
    struct inode *inode;
    struct work_struct free_work;
    struct wait_queue_head migration_wait;
    atomic_long_t isolated_pages;
    bool destroying;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct zs_pool {
    const char *name;
    struct size_class * size_class[257];
    struct kmem_cache *handle_cachep;
    struct kmem_cache *zspage_cachep;
    atomic_long_t pages_allocated;
    struct zs_pool_stats stats;
    struct shrinker shrinker;
    struct inode *inode;
    struct work_struct free_work;
    struct wait_queue_head migration_wait;
    atomic_long_t isolated_pages;
    bool destroying;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct zs_pool {
    const char *name;
    struct size_class * size_class[255];
    struct kmem_cache *handle_cachep;
    struct kmem_cache *zspage_cachep;
    atomic_long_t pages_allocated;
    struct zs_pool_stats stats;
    struct shrinker shrinker;
    struct inode *inode;
    struct work_struct free_work;
    struct wait_queue_head migration_wait;
    atomic_long_t isolated_pages;
    bool destroying;
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
struct zs_pool {
    const char *name;
    struct size_class * size_class[255];
    struct kmem_cache *handle_cachep;
    struct kmem_cache *zspage_cachep;
    atomic_long_t pages_allocated;
    struct zs_pool_stats stats;
    struct shrinker shrinker;
    struct inode *inode;
    struct work_struct free_work;
    struct wait_queue_head migration_wait;
    atomic_long_t isolated_pages;
    bool destroying;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct zs_pool {
    const char *name;
    struct size_class * size_class[255];
    struct kmem_cache *handle_cachep;
    struct kmem_cache *zspage_cachep;
    atomic_long_t pages_allocated;
    struct zs_pool_stats stats;
    struct shrinker shrinker;
    struct inode *inode;
    struct work_struct free_work;
    struct wait_queue_head migration_wait;
    atomic_long_t isolated_pages;
    bool destroying;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct zs_pool {
    const char *name;
    struct size_class * size_class[255];
    struct kmem_cache *handle_cachep;
    struct kmem_cache *zspage_cachep;
    atomic_long_t pages_allocated;
    struct zs_pool_stats stats;
    struct shrinker shrinker;
    struct inode *inode;
    struct work_struct free_work;
    struct wait_queue_head migration_wait;
    atomic_long_t isolated_pages;
    bool destroying;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct zs_pool {
    const char *name;
    struct size_class * size_class[255];
    struct kmem_cache *handle_cachep;
    struct kmem_cache *zspage_cachep;
    atomic_long_t pages_allocated;
    struct zs_pool_stats stats;
    struct shrinker shrinker;
    struct inode *inode;
    struct work_struct free_work;
    struct wait_queue_head migration_wait;
    atomic_long_t isolated_pages;
    bool destroying;
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
<code>struct kmem_cache *zspage_cachep</code>
</li>
<li>
<b>Field added. </b>
<code>struct inode *inode</code>
</li>
<li>
<b>Field added. </b>
<code>struct work_struct free_work</code>
</li>
<li>
<b>Field removed. </b>
<code>gfp_t flags</code>
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
<b>Field type changed. </b>
<code>struct size_class **size_class</code> ➡️ <code>struct size_class * size_class[255]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>bool shrinker_enabled</code>
</li>
</ul>
</details>
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
<code>struct wait_queue_head migration_wait</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t isolated_pages</code>
</li>
<li>
<b>Field added. </b>
<code>bool destroying</code>
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
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>rwlock_t migrate_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>struct wait_queue_head migration_wait</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_long_t isolated_pages</code>
</li>
<li>
<b>Field removed. </b>
<code>bool destroying</code>
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
<code>struct list_head lru</code>
</li>
<li>
<b>Field added. </b>
<code>struct zpool *zpool</code>
</li>
<li>
<b>Field added. </b>
<code>const struct zpool_ops *zpool_ops</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t lock</code>
</li>
<li>
<b>Field removed. </b>
<code>struct inode *inode</code>
</li>
<li>
<b>Field removed. </b>
<code>rwlock_t migrate_lock</code>
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
<code>atomic_t compaction_in_progress</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head lru</code>
</li>
<li>
<b>Field removed. </b>
<code>struct zpool *zpool</code>
</li>
<li>
<b>Field removed. </b>
<code>const struct zpool_ops *zpool_ops</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct shrinker shrinker</code> ➡️ <code>struct shrinker *shrinker</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct size_class * size_class[255]</code> ➡️ <code>struct size_class * size_class[257]</code>
</li>
</ul>
</details>
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
