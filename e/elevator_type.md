# Struct: <code>elevator_type</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct elevator_type {
    struct kmem_cache *icq_cache;
    struct elevator_ops ops;
    size_t icq_size;
    size_t icq_align;
    struct elv_fs_entry *elevator_attrs;
    char elevator_name[16];
    struct module *elevator_owner;
    char icq_cache_name[21];
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct elevator_type {
    struct kmem_cache *icq_cache;
    struct elevator_ops ops;
    size_t icq_size;
    size_t icq_align;
    struct elv_fs_entry *elevator_attrs;
    char elevator_name[16];
    struct module *elevator_owner;
    char icq_cache_name[21];
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct elevator_type {
    struct kmem_cache *icq_cache;
    struct elevator_ops ops;
    size_t icq_size;
    size_t icq_align;
    struct elv_fs_entry *elevator_attrs;
    char elevator_name[16];
    struct module *elevator_owner;
    char icq_cache_name[21];
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct elevator_type {
    struct kmem_cache *icq_cache;
    union (anon) ops;
    size_t icq_size;
    size_t icq_align;
    struct elv_fs_entry *elevator_attrs;
    char elevator_name[16];
    struct module *elevator_owner;
    bool uses_mq;
    const struct blk_mq_debugfs_attr *queue_debugfs_attrs;
    const struct blk_mq_debugfs_attr *hctx_debugfs_attrs;
    char icq_cache_name[22];
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct elevator_type {
    struct kmem_cache *icq_cache;
    union (anon) ops;
    size_t icq_size;
    size_t icq_align;
    struct elv_fs_entry *elevator_attrs;
    char elevator_name[16];
    const char *elevator_alias;
    struct module *elevator_owner;
    bool uses_mq;
    const struct blk_mq_debugfs_attr *queue_debugfs_attrs;
    const struct blk_mq_debugfs_attr *hctx_debugfs_attrs;
    char icq_cache_name[22];
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct elevator_type {
    struct kmem_cache *icq_cache;
    union (anon) ops;
    size_t icq_size;
    size_t icq_align;
    struct elv_fs_entry *elevator_attrs;
    char elevator_name[16];
    const char *elevator_alias;
    struct module *elevator_owner;
    bool uses_mq;
    const struct blk_mq_debugfs_attr *queue_debugfs_attrs;
    const struct blk_mq_debugfs_attr *hctx_debugfs_attrs;
    char icq_cache_name[22];
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct elevator_type {
    struct kmem_cache *icq_cache;
    struct elevator_mq_ops ops;
    size_t icq_size;
    size_t icq_align;
    struct elv_fs_entry *elevator_attrs;
    char elevator_name[16];
    const char *elevator_alias;
    struct module *elevator_owner;
    const struct blk_mq_debugfs_attr *queue_debugfs_attrs;
    const struct blk_mq_debugfs_attr *hctx_debugfs_attrs;
    char icq_cache_name[22];
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct elevator_type {
    struct kmem_cache *icq_cache;
    struct elevator_mq_ops ops;
    size_t icq_size;
    size_t icq_align;
    struct elv_fs_entry *elevator_attrs;
    const char *elevator_name;
    const char *elevator_alias;
    struct module *elevator_owner;
    const struct blk_mq_debugfs_attr *queue_debugfs_attrs;
    const struct blk_mq_debugfs_attr *hctx_debugfs_attrs;
    char icq_cache_name[22];
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct elevator_type {
    struct kmem_cache *icq_cache;
    struct elevator_mq_ops ops;
    size_t icq_size;
    size_t icq_align;
    struct elv_fs_entry *elevator_attrs;
    const char *elevator_name;
    const char *elevator_alias;
    const unsigned int elevator_features;
    struct module *elevator_owner;
    const struct blk_mq_debugfs_attr *queue_debugfs_attrs;
    const struct blk_mq_debugfs_attr *hctx_debugfs_attrs;
    char icq_cache_name[22];
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct elevator_type {
    struct kmem_cache *icq_cache;
    struct elevator_mq_ops ops;
    size_t icq_size;
    size_t icq_align;
    struct elv_fs_entry *elevator_attrs;
    const char *elevator_name;
    const char *elevator_alias;
    const unsigned int elevator_features;
    struct module *elevator_owner;
    const struct blk_mq_debugfs_attr *queue_debugfs_attrs;
    const struct blk_mq_debugfs_attr *hctx_debugfs_attrs;
    char icq_cache_name[22];
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct elevator_type {
    struct kmem_cache *icq_cache;
    struct elevator_mq_ops ops;
    size_t icq_size;
    size_t icq_align;
    struct elv_fs_entry *elevator_attrs;
    const char *elevator_name;
    const char *elevator_alias;
    const unsigned int elevator_features;
    struct module *elevator_owner;
    const struct blk_mq_debugfs_attr *queue_debugfs_attrs;
    const struct blk_mq_debugfs_attr *hctx_debugfs_attrs;
    char icq_cache_name[22];
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct elevator_type {
    struct kmem_cache *icq_cache;
    struct elevator_mq_ops ops;
    size_t icq_size;
    size_t icq_align;
    struct elv_fs_entry *elevator_attrs;
    const char *elevator_name;
    const char *elevator_alias;
    const unsigned int elevator_features;
    struct module *elevator_owner;
    const struct blk_mq_debugfs_attr *queue_debugfs_attrs;
    const struct blk_mq_debugfs_attr *hctx_debugfs_attrs;
    char icq_cache_name[22];
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct elevator_type {
    struct kmem_cache *icq_cache;
    struct elevator_mq_ops ops;
    size_t icq_size;
    size_t icq_align;
    struct elv_fs_entry *elevator_attrs;
    const char *elevator_name;
    const char *elevator_alias;
    const unsigned int elevator_features;
    struct module *elevator_owner;
    const struct blk_mq_debugfs_attr *queue_debugfs_attrs;
    const struct blk_mq_debugfs_attr *hctx_debugfs_attrs;
    char icq_cache_name[22];
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct elevator_type {
    struct kmem_cache *icq_cache;
    struct elevator_mq_ops ops;
    size_t icq_size;
    size_t icq_align;
    struct elv_fs_entry *elevator_attrs;
    const char *elevator_name;
    const char *elevator_alias;
    const unsigned int elevator_features;
    struct module *elevator_owner;
    const struct blk_mq_debugfs_attr *queue_debugfs_attrs;
    const struct blk_mq_debugfs_attr *hctx_debugfs_attrs;
    char icq_cache_name[22];
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct elevator_type {
    struct kmem_cache *icq_cache;
    struct elevator_mq_ops ops;
    size_t icq_size;
    size_t icq_align;
    struct elv_fs_entry *elevator_attrs;
    const char *elevator_name;
    const char *elevator_alias;
    const unsigned int elevator_features;
    struct module *elevator_owner;
    const struct blk_mq_debugfs_attr *queue_debugfs_attrs;
    const struct blk_mq_debugfs_attr *hctx_debugfs_attrs;
    char icq_cache_name[22];
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct elevator_type {
    struct kmem_cache *icq_cache;
    struct elevator_mq_ops ops;
    size_t icq_size;
    size_t icq_align;
    struct elv_fs_entry *elevator_attrs;
    const char *elevator_name;
    const char *elevator_alias;
    const unsigned int elevator_features;
    struct module *elevator_owner;
    const struct blk_mq_debugfs_attr *queue_debugfs_attrs;
    const struct blk_mq_debugfs_attr *hctx_debugfs_attrs;
    char icq_cache_name[22];
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct elevator_type {
    struct kmem_cache *icq_cache;
    struct elevator_mq_ops ops;
    size_t icq_size;
    size_t icq_align;
    struct elv_fs_entry *elevator_attrs;
    const char *elevator_name;
    const char *elevator_alias;
    const unsigned int elevator_features;
    struct module *elevator_owner;
    const struct blk_mq_debugfs_attr *queue_debugfs_attrs;
    const struct blk_mq_debugfs_attr *hctx_debugfs_attrs;
    char icq_cache_name[22];
    struct list_head list;
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
struct elevator_type {
    struct kmem_cache *icq_cache;
    struct elevator_mq_ops ops;
    size_t icq_size;
    size_t icq_align;
    struct elv_fs_entry *elevator_attrs;
    const char *elevator_name;
    const char *elevator_alias;
    const unsigned int elevator_features;
    struct module *elevator_owner;
    const struct blk_mq_debugfs_attr *queue_debugfs_attrs;
    const struct blk_mq_debugfs_attr *hctx_debugfs_attrs;
    char icq_cache_name[22];
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct elevator_type {
    struct kmem_cache *icq_cache;
    struct elevator_mq_ops ops;
    size_t icq_size;
    size_t icq_align;
    struct elv_fs_entry *elevator_attrs;
    const char *elevator_name;
    const char *elevator_alias;
    const unsigned int elevator_features;
    struct module *elevator_owner;
    const struct blk_mq_debugfs_attr *queue_debugfs_attrs;
    const struct blk_mq_debugfs_attr *hctx_debugfs_attrs;
    char icq_cache_name[22];
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct elevator_type {
    struct kmem_cache *icq_cache;
    struct elevator_mq_ops ops;
    size_t icq_size;
    size_t icq_align;
    struct elv_fs_entry *elevator_attrs;
    const char *elevator_name;
    const char *elevator_alias;
    const unsigned int elevator_features;
    struct module *elevator_owner;
    const struct blk_mq_debugfs_attr *queue_debugfs_attrs;
    const struct blk_mq_debugfs_attr *hctx_debugfs_attrs;
    char icq_cache_name[22];
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct elevator_type {
    struct kmem_cache *icq_cache;
    struct elevator_mq_ops ops;
    size_t icq_size;
    size_t icq_align;
    struct elv_fs_entry *elevator_attrs;
    const char *elevator_name;
    const char *elevator_alias;
    const unsigned int elevator_features;
    struct module *elevator_owner;
    const struct blk_mq_debugfs_attr *queue_debugfs_attrs;
    const struct blk_mq_debugfs_attr *hctx_debugfs_attrs;
    char icq_cache_name[22];
    struct list_head list;
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
struct elevator_type {
    struct kmem_cache *icq_cache;
    struct elevator_mq_ops ops;
    size_t icq_size;
    size_t icq_align;
    struct elv_fs_entry *elevator_attrs;
    const char *elevator_name;
    const char *elevator_alias;
    const unsigned int elevator_features;
    struct module *elevator_owner;
    const struct blk_mq_debugfs_attr *queue_debugfs_attrs;
    const struct blk_mq_debugfs_attr *hctx_debugfs_attrs;
    char icq_cache_name[22];
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct elevator_type {
    struct kmem_cache *icq_cache;
    struct elevator_mq_ops ops;
    size_t icq_size;
    size_t icq_align;
    struct elv_fs_entry *elevator_attrs;
    const char *elevator_name;
    const char *elevator_alias;
    const unsigned int elevator_features;
    struct module *elevator_owner;
    const struct blk_mq_debugfs_attr *queue_debugfs_attrs;
    const struct blk_mq_debugfs_attr *hctx_debugfs_attrs;
    char icq_cache_name[22];
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct elevator_type {
    struct kmem_cache *icq_cache;
    struct elevator_mq_ops ops;
    size_t icq_size;
    size_t icq_align;
    struct elv_fs_entry *elevator_attrs;
    const char *elevator_name;
    const char *elevator_alias;
    const unsigned int elevator_features;
    struct module *elevator_owner;
    const struct blk_mq_debugfs_attr *queue_debugfs_attrs;
    const struct blk_mq_debugfs_attr *hctx_debugfs_attrs;
    char icq_cache_name[22];
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct elevator_type {
    struct kmem_cache *icq_cache;
    struct elevator_mq_ops ops;
    size_t icq_size;
    size_t icq_align;
    struct elv_fs_entry *elevator_attrs;
    const char *elevator_name;
    const char *elevator_alias;
    const unsigned int elevator_features;
    struct module *elevator_owner;
    const struct blk_mq_debugfs_attr *queue_debugfs_attrs;
    const struct blk_mq_debugfs_attr *hctx_debugfs_attrs;
    char icq_cache_name[22];
    struct list_head list;
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
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool uses_mq</code>
</li>
<li>
<b>Field added. </b>
<code>const struct blk_mq_debugfs_attr *queue_debugfs_attrs</code>
</li>
<li>
<b>Field added. </b>
<code>const struct blk_mq_debugfs_attr *hctx_debugfs_attrs</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct elevator_ops ops</code> ➡️ <code>union (anon) ops</code>
</li>
<li>
<b>Field type changed. </b>
<code>char icq_cache_name[21]</code> ➡️ <code>char icq_cache_name[22]</code>
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
<code>const char *elevator_alias</code>
</li>
</ul>
</details>
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
<code>bool uses_mq</code>
</li>
<li>
<b>Field type changed. </b>
<code>union (anon) ops</code> ➡️ <code>struct elevator_mq_ops ops</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>char elevator_name[16]</code> ➡️ <code>const char *elevator_name</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const unsigned int elevator_features</code>
</li>
</ul>
</details>
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
