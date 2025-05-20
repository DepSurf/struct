# Struct: <code>dm_table</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct dm_table {
    int undefined__;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct dm_table {
    struct mapped_device *md;
    unsigned int type;
    unsigned int depth;
    unsigned int counts[16];
    sector_t * index[16];
    unsigned int num_targets;
    unsigned int num_allocated;
    sector_t *highs;
    struct dm_target *targets;
    struct target_type *immutable_target_type;
    bool integrity_supported;
    bool singleton;
    bool all_blk_mq;
    fmode_t mode;
    struct list_head devices;
    void (*event_fn)(void *);
    void *event_context;
    struct dm_md_mempools *mempools;
    struct list_head target_callbacks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct dm_table {
    struct mapped_device *md;
    unsigned int type;
    unsigned int depth;
    unsigned int counts[16];
    sector_t * index[16];
    unsigned int num_targets;
    unsigned int num_allocated;
    sector_t *highs;
    struct dm_target *targets;
    struct target_type *immutable_target_type;
    bool integrity_supported;
    bool singleton;
    bool all_blk_mq;
    fmode_t mode;
    struct list_head devices;
    void (*event_fn)(void *);
    void *event_context;
    struct dm_md_mempools *mempools;
    struct list_head target_callbacks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct dm_table {
    struct mapped_device *md;
    enum dm_queue_mode type;
    unsigned int depth;
    unsigned int counts[16];
    sector_t * index[16];
    unsigned int num_targets;
    unsigned int num_allocated;
    sector_t *highs;
    struct dm_target *targets;
    struct target_type *immutable_target_type;
    bool integrity_supported;
    bool singleton;
    bool all_blk_mq;
    unsigned int integrity_added;
    fmode_t mode;
    struct list_head devices;
    void (*event_fn)(void *);
    void *event_context;
    struct dm_md_mempools *mempools;
    struct list_head target_callbacks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dm_table {
    struct mapped_device *md;
    enum dm_queue_mode type;
    unsigned int depth;
    unsigned int counts[16];
    sector_t * index[16];
    unsigned int num_targets;
    unsigned int num_allocated;
    sector_t *highs;
    struct dm_target *targets;
    struct target_type *immutable_target_type;
    bool integrity_supported;
    bool singleton;
    bool all_blk_mq;
    unsigned int integrity_added;
    fmode_t mode;
    struct list_head devices;
    void (*event_fn)(void *);
    void *event_context;
    struct dm_md_mempools *mempools;
    struct list_head target_callbacks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dm_table {
    struct mapped_device *md;
    enum dm_queue_mode type;
    unsigned int depth;
    unsigned int counts[16];
    sector_t * index[16];
    unsigned int num_targets;
    unsigned int num_allocated;
    sector_t *highs;
    struct dm_target *targets;
    struct target_type *immutable_target_type;
    bool integrity_supported;
    bool singleton;
    bool all_blk_mq;
    unsigned int integrity_added;
    fmode_t mode;
    struct list_head devices;
    void (*event_fn)(void *);
    void *event_context;
    struct dm_md_mempools *mempools;
    struct list_head target_callbacks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dm_table {
    struct mapped_device *md;
    enum dm_queue_mode type;
    unsigned int depth;
    unsigned int counts[16];
    sector_t * index[16];
    unsigned int num_targets;
    unsigned int num_allocated;
    sector_t *highs;
    struct dm_target *targets;
    struct target_type *immutable_target_type;
    bool integrity_supported;
    bool singleton;
    unsigned int integrity_added;
    fmode_t mode;
    struct list_head devices;
    void (*event_fn)(void *);
    void *event_context;
    struct dm_md_mempools *mempools;
    struct list_head target_callbacks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dm_table {
    struct mapped_device *md;
    enum dm_queue_mode type;
    unsigned int depth;
    unsigned int counts[16];
    sector_t * index[16];
    unsigned int num_targets;
    unsigned int num_allocated;
    sector_t *highs;
    struct dm_target *targets;
    struct target_type *immutable_target_type;
    bool integrity_supported;
    bool singleton;
    unsigned int integrity_added;
    fmode_t mode;
    struct list_head devices;
    void (*event_fn)(void *);
    void *event_context;
    struct dm_md_mempools *mempools;
    struct list_head target_callbacks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dm_table {
    struct mapped_device *md;
    enum dm_queue_mode type;
    unsigned int depth;
    unsigned int counts[16];
    sector_t * index[16];
    unsigned int num_targets;
    unsigned int num_allocated;
    sector_t *highs;
    struct dm_target *targets;
    struct target_type *immutable_target_type;
    bool integrity_supported;
    bool singleton;
    unsigned int integrity_added;
    fmode_t mode;
    struct list_head devices;
    void (*event_fn)(void *);
    void *event_context;
    struct dm_md_mempools *mempools;
    struct list_head target_callbacks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dm_table {
    struct mapped_device *md;
    enum dm_queue_mode type;
    unsigned int depth;
    unsigned int counts[16];
    sector_t * index[16];
    unsigned int num_targets;
    unsigned int num_allocated;
    sector_t *highs;
    struct dm_target *targets;
    struct target_type *immutable_target_type;
    bool integrity_supported;
    bool singleton;
    unsigned int integrity_added;
    fmode_t mode;
    struct list_head devices;
    void (*event_fn)(void *);
    void *event_context;
    struct dm_md_mempools *mempools;
    struct list_head target_callbacks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dm_table {
    struct mapped_device *md;
    enum dm_queue_mode type;
    unsigned int depth;
    unsigned int counts[16];
    sector_t * index[16];
    unsigned int num_targets;
    unsigned int num_allocated;
    sector_t *highs;
    struct dm_target *targets;
    struct target_type *immutable_target_type;
    bool integrity_supported;
    bool singleton;
    unsigned int integrity_added;
    fmode_t mode;
    struct list_head devices;
    void (*event_fn)(void *);
    void *event_context;
    struct dm_md_mempools *mempools;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dm_table {
    struct mapped_device *md;
    enum dm_queue_mode type;
    unsigned int depth;
    unsigned int counts[16];
    sector_t * index[16];
    unsigned int num_targets;
    unsigned int num_allocated;
    sector_t *highs;
    struct dm_target *targets;
    struct target_type *immutable_target_type;
    bool integrity_supported;
    bool singleton;
    unsigned int integrity_added;
    fmode_t mode;
    struct list_head devices;
    void (*event_fn)(void *);
    void *event_context;
    struct dm_md_mempools *mempools;
    struct blk_keyslot_manager *ksm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dm_table {
    struct mapped_device *md;
    enum dm_queue_mode type;
    unsigned int depth;
    unsigned int counts[16];
    sector_t * index[16];
    unsigned int num_targets;
    unsigned int num_allocated;
    sector_t *highs;
    struct dm_target *targets;
    struct target_type *immutable_target_type;
    bool integrity_supported;
    bool singleton;
    unsigned int integrity_added;
    fmode_t mode;
    struct list_head devices;
    void (*event_fn)(void *);
    void *event_context;
    struct dm_md_mempools *mempools;
    struct blk_keyslot_manager *ksm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dm_table {
    struct mapped_device *md;
    enum dm_queue_mode type;
    unsigned int depth;
    unsigned int counts[16];
    sector_t * index[16];
    unsigned int num_targets;
    unsigned int num_allocated;
    sector_t *highs;
    struct dm_target *targets;
    struct target_type *immutable_target_type;
    bool integrity_supported;
    bool singleton;
    unsigned int integrity_added;
    fmode_t mode;
    struct list_head devices;
    void (*event_fn)(void *);
    void *event_context;
    struct dm_md_mempools *mempools;
    struct blk_crypto_profile *crypto_profile;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dm_table {
    struct mapped_device *md;
    enum dm_queue_mode type;
    unsigned int depth;
    unsigned int counts[16];
    sector_t * index[16];
    unsigned int num_targets;
    unsigned int num_allocated;
    sector_t *highs;
    struct dm_target *targets;
    struct target_type *immutable_target_type;
    bool integrity_supported;
    bool singleton;
    unsigned int integrity_added;
    fmode_t mode;
    struct list_head devices;
    void (*event_fn)(void *);
    void *event_context;
    struct dm_md_mempools *mempools;
    struct blk_crypto_profile *crypto_profile;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dm_table {
    struct mapped_device *md;
    enum dm_queue_mode type;
    unsigned int depth;
    unsigned int counts[16];
    sector_t * index[16];
    unsigned int num_targets;
    unsigned int num_allocated;
    sector_t *highs;
    struct dm_target *targets;
    struct target_type *immutable_target_type;
    bool integrity_supported;
    bool singleton;
    unsigned int integrity_added;
    blk_mode_t mode;
    struct list_head devices;
    void (*event_fn)(void *);
    void *event_context;
    struct dm_md_mempools *mempools;
    struct blk_crypto_profile *crypto_profile;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dm_table {
    struct mapped_device *md;
    enum dm_queue_mode type;
    unsigned int depth;
    unsigned int counts[16];
    sector_t * index[16];
    unsigned int num_targets;
    unsigned int num_allocated;
    sector_t *highs;
    struct dm_target *targets;
    struct target_type *immutable_target_type;
    bool integrity_supported;
    bool singleton;
    unsigned int integrity_added;
    blk_mode_t mode;
    struct list_head devices;
    struct rw_semaphore devices_lock;
    void (*event_fn)(void *);
    void *event_context;
    struct dm_md_mempools *mempools;
    struct blk_crypto_profile *crypto_profile;
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
struct dm_table {
    struct mapped_device *md;
    enum dm_queue_mode type;
    unsigned int depth;
    unsigned int counts[16];
    sector_t * index[16];
    unsigned int num_targets;
    unsigned int num_allocated;
    sector_t *highs;
    struct dm_target *targets;
    struct target_type *immutable_target_type;
    bool integrity_supported;
    bool singleton;
    unsigned int integrity_added;
    fmode_t mode;
    struct list_head devices;
    void (*event_fn)(void *);
    void *event_context;
    struct dm_md_mempools *mempools;
    struct list_head target_callbacks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dm_table {
    struct mapped_device *md;
    enum dm_queue_mode type;
    unsigned int depth;
    unsigned int counts[16];
    sector_t * index[16];
    unsigned int num_targets;
    unsigned int num_allocated;
    sector_t *highs;
    struct dm_target *targets;
    struct target_type *immutable_target_type;
    bool integrity_supported;
    bool singleton;
    unsigned int integrity_added;
    fmode_t mode;
    struct list_head devices;
    void (*event_fn)(void *);
    void *event_context;
    struct dm_md_mempools *mempools;
    struct list_head target_callbacks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dm_table {
    struct mapped_device *md;
    enum dm_queue_mode type;
    unsigned int depth;
    unsigned int counts[16];
    sector_t * index[16];
    unsigned int num_targets;
    unsigned int num_allocated;
    sector_t *highs;
    struct dm_target *targets;
    struct target_type *immutable_target_type;
    bool integrity_supported;
    bool singleton;
    unsigned int integrity_added;
    fmode_t mode;
    struct list_head devices;
    void (*event_fn)(void *);
    void *event_context;
    struct dm_md_mempools *mempools;
    struct list_head target_callbacks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dm_table {
    struct mapped_device *md;
    enum dm_queue_mode type;
    unsigned int depth;
    unsigned int counts[16];
    sector_t * index[16];
    unsigned int num_targets;
    unsigned int num_allocated;
    sector_t *highs;
    struct dm_target *targets;
    struct target_type *immutable_target_type;
    bool integrity_supported;
    bool singleton;
    unsigned int integrity_added;
    fmode_t mode;
    struct list_head devices;
    void (*event_fn)(void *);
    void *event_context;
    struct dm_md_mempools *mempools;
    struct list_head target_callbacks;
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
struct dm_table {
    struct mapped_device *md;
    enum dm_queue_mode type;
    unsigned int depth;
    unsigned int counts[16];
    sector_t * index[16];
    unsigned int num_targets;
    unsigned int num_allocated;
    sector_t *highs;
    struct dm_target *targets;
    struct target_type *immutable_target_type;
    bool integrity_supported;
    bool singleton;
    unsigned int integrity_added;
    fmode_t mode;
    struct list_head devices;
    void (*event_fn)(void *);
    void *event_context;
    struct dm_md_mempools *mempools;
    struct list_head target_callbacks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dm_table {
    struct mapped_device *md;
    enum dm_queue_mode type;
    unsigned int depth;
    unsigned int counts[16];
    sector_t * index[16];
    unsigned int num_targets;
    unsigned int num_allocated;
    sector_t *highs;
    struct dm_target *targets;
    struct target_type *immutable_target_type;
    bool integrity_supported;
    bool singleton;
    unsigned int integrity_added;
    fmode_t mode;
    struct list_head devices;
    void (*event_fn)(void *);
    void *event_context;
    struct dm_md_mempools *mempools;
    struct list_head target_callbacks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dm_table {
    struct mapped_device *md;
    enum dm_queue_mode type;
    unsigned int depth;
    unsigned int counts[16];
    sector_t * index[16];
    unsigned int num_targets;
    unsigned int num_allocated;
    sector_t *highs;
    struct dm_target *targets;
    struct target_type *immutable_target_type;
    bool integrity_supported;
    bool singleton;
    unsigned int integrity_added;
    fmode_t mode;
    struct list_head devices;
    void (*event_fn)(void *);
    void *event_context;
    struct dm_md_mempools *mempools;
    struct list_head target_callbacks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dm_table {
    struct mapped_device *md;
    enum dm_queue_mode type;
    unsigned int depth;
    unsigned int counts[16];
    sector_t * index[16];
    unsigned int num_targets;
    unsigned int num_allocated;
    sector_t *highs;
    struct dm_target *targets;
    struct target_type *immutable_target_type;
    bool integrity_supported;
    bool singleton;
    unsigned int integrity_added;
    fmode_t mode;
    struct list_head devices;
    void (*event_fn)(void *);
    void *event_context;
    struct dm_md_mempools *mempools;
    struct list_head target_callbacks;
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
<code>struct mapped_device *md</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int type</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int depth</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int counts[16]</code>
</li>
<li>
<b>Field added. </b>
<code>sector_t * index[16]</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int num_targets</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int num_allocated</code>
</li>
<li>
<b>Field added. </b>
<code>sector_t *highs</code>
</li>
<li>
<b>Field added. </b>
<code>struct dm_target *targets</code>
</li>
<li>
<b>Field added. </b>
<code>struct target_type *immutable_target_type</code>
</li>
<li>
<b>Field added. </b>
<code>bool integrity_supported</code>
</li>
<li>
<b>Field added. </b>
<code>bool singleton</code>
</li>
<li>
<b>Field added. </b>
<code>bool all_blk_mq</code>
</li>
<li>
<b>Field added. </b>
<code>fmode_t mode</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head devices</code>
</li>
<li>
<b>Field added. </b>
<code>void (*event_fn)(void *)</code>
</li>
<li>
<b>Field added. </b>
<code>void *event_context</code>
</li>
<li>
<b>Field added. </b>
<code>struct dm_md_mempools *mempools</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head target_callbacks</code>
</li>
<li>
<b>Field removed. </b>
<code>int undefined__</code>
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
<code>unsigned int integrity_added</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int type</code> ➡️ <code>enum dm_queue_mode type</code>
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
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>bool all_blk_mq</code>
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
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct list_head target_callbacks</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct blk_keyslot_manager *ksm</code>
</li>
</ul>
</details>
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
<code>struct blk_crypto_profile *crypto_profile</code>
</li>
<li>
<b>Field removed. </b>
<code>struct blk_keyslot_manager *ksm</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>fmode_t mode</code> ➡️ <code>blk_mode_t mode</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct rw_semaphore devices_lock</code>
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
