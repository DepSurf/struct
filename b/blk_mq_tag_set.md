# Struct: <code>blk_mq_tag_set</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct blk_mq_tag_set {
    struct blk_mq_ops *ops;
    unsigned int nr_hw_queues;
    unsigned int queue_depth;
    unsigned int reserved_tags;
    unsigned int cmd_size;
    int numa_node;
    unsigned int timeout;
    unsigned int flags;
    void *driver_data;
    struct blk_mq_tags **tags;
    struct mutex tag_list_lock;
    struct list_head tag_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct blk_mq_tag_set {
    struct blk_mq_ops *ops;
    unsigned int nr_hw_queues;
    unsigned int queue_depth;
    unsigned int reserved_tags;
    unsigned int cmd_size;
    int numa_node;
    unsigned int timeout;
    unsigned int flags;
    void *driver_data;
    struct blk_mq_tags **tags;
    struct mutex tag_list_lock;
    struct list_head tag_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct blk_mq_tag_set {
    unsigned int *mq_map;
    struct blk_mq_ops *ops;
    unsigned int nr_hw_queues;
    unsigned int queue_depth;
    unsigned int reserved_tags;
    unsigned int cmd_size;
    int numa_node;
    unsigned int timeout;
    unsigned int flags;
    void *driver_data;
    struct blk_mq_tags **tags;
    struct mutex tag_list_lock;
    struct list_head tag_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct blk_mq_tag_set {
    unsigned int *mq_map;
    const struct blk_mq_ops *ops;
    unsigned int nr_hw_queues;
    unsigned int queue_depth;
    unsigned int reserved_tags;
    unsigned int cmd_size;
    int numa_node;
    unsigned int timeout;
    unsigned int flags;
    void *driver_data;
    struct blk_mq_tags **tags;
    struct mutex tag_list_lock;
    struct list_head tag_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct blk_mq_tag_set {
    unsigned int *mq_map;
    const struct blk_mq_ops *ops;
    unsigned int nr_hw_queues;
    unsigned int queue_depth;
    unsigned int reserved_tags;
    unsigned int cmd_size;
    int numa_node;
    unsigned int timeout;
    unsigned int flags;
    void *driver_data;
    struct blk_mq_tags **tags;
    struct mutex tag_list_lock;
    struct list_head tag_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct blk_mq_tag_set {
    unsigned int *mq_map;
    const struct blk_mq_ops *ops;
    unsigned int nr_hw_queues;
    unsigned int queue_depth;
    unsigned int reserved_tags;
    unsigned int cmd_size;
    int numa_node;
    unsigned int timeout;
    unsigned int flags;
    void *driver_data;
    struct blk_mq_tags **tags;
    struct mutex tag_list_lock;
    struct list_head tag_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct blk_mq_tag_set {
    struct blk_mq_queue_map map[3];
    unsigned int nr_maps;
    const struct blk_mq_ops *ops;
    unsigned int nr_hw_queues;
    unsigned int queue_depth;
    unsigned int reserved_tags;
    unsigned int cmd_size;
    int numa_node;
    unsigned int timeout;
    unsigned int flags;
    void *driver_data;
    struct blk_mq_tags **tags;
    struct mutex tag_list_lock;
    struct list_head tag_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct blk_mq_tag_set {
    struct blk_mq_queue_map map[3];
    unsigned int nr_maps;
    const struct blk_mq_ops *ops;
    unsigned int nr_hw_queues;
    unsigned int queue_depth;
    unsigned int reserved_tags;
    unsigned int cmd_size;
    int numa_node;
    unsigned int timeout;
    unsigned int flags;
    void *driver_data;
    struct blk_mq_tags **tags;
    struct mutex tag_list_lock;
    struct list_head tag_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct blk_mq_tag_set {
    struct blk_mq_queue_map map[3];
    unsigned int nr_maps;
    const struct blk_mq_ops *ops;
    unsigned int nr_hw_queues;
    unsigned int queue_depth;
    unsigned int reserved_tags;
    unsigned int cmd_size;
    int numa_node;
    unsigned int timeout;
    unsigned int flags;
    void *driver_data;
    struct blk_mq_tags **tags;
    struct mutex tag_list_lock;
    struct list_head tag_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct blk_mq_tag_set {
    struct blk_mq_queue_map map[3];
    unsigned int nr_maps;
    const struct blk_mq_ops *ops;
    unsigned int nr_hw_queues;
    unsigned int queue_depth;
    unsigned int reserved_tags;
    unsigned int cmd_size;
    int numa_node;
    unsigned int timeout;
    unsigned int flags;
    void *driver_data;
    struct blk_mq_tags **tags;
    struct mutex tag_list_lock;
    struct list_head tag_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct blk_mq_tag_set {
    struct blk_mq_queue_map map[3];
    unsigned int nr_maps;
    const struct blk_mq_ops *ops;
    unsigned int nr_hw_queues;
    unsigned int queue_depth;
    unsigned int reserved_tags;
    unsigned int cmd_size;
    int numa_node;
    unsigned int timeout;
    unsigned int flags;
    void *driver_data;
    atomic_t active_queues_shared_sbitmap;
    struct sbitmap_queue __bitmap_tags;
    struct sbitmap_queue __breserved_tags;
    struct blk_mq_tags **tags;
    struct mutex tag_list_lock;
    struct list_head tag_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct blk_mq_tag_set {
    struct blk_mq_queue_map map[3];
    unsigned int nr_maps;
    const struct blk_mq_ops *ops;
    unsigned int nr_hw_queues;
    unsigned int queue_depth;
    unsigned int reserved_tags;
    unsigned int cmd_size;
    int numa_node;
    unsigned int timeout;
    unsigned int flags;
    void *driver_data;
    atomic_t active_queues_shared_sbitmap;
    struct sbitmap_queue __bitmap_tags;
    struct sbitmap_queue __breserved_tags;
    struct blk_mq_tags **tags;
    struct mutex tag_list_lock;
    struct list_head tag_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct blk_mq_tag_set {
    struct blk_mq_queue_map map[3];
    unsigned int nr_maps;
    const struct blk_mq_ops *ops;
    unsigned int nr_hw_queues;
    unsigned int queue_depth;
    unsigned int reserved_tags;
    unsigned int cmd_size;
    int numa_node;
    unsigned int timeout;
    unsigned int flags;
    void *driver_data;
    atomic_t active_queues_shared_sbitmap;
    struct sbitmap_queue __bitmap_tags;
    struct sbitmap_queue __breserved_tags;
    struct blk_mq_tags **tags;
    struct mutex tag_list_lock;
    struct list_head tag_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct blk_mq_tag_set {
    struct blk_mq_queue_map map[3];
    unsigned int nr_maps;
    const struct blk_mq_ops *ops;
    unsigned int nr_hw_queues;
    unsigned int queue_depth;
    unsigned int reserved_tags;
    unsigned int cmd_size;
    int numa_node;
    unsigned int timeout;
    unsigned int flags;
    void *driver_data;
    struct blk_mq_tags **tags;
    struct blk_mq_tags *shared_tags;
    struct mutex tag_list_lock;
    struct list_head tag_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct blk_mq_tag_set {
    struct blk_mq_queue_map map[3];
    unsigned int nr_maps;
    const struct blk_mq_ops *ops;
    unsigned int nr_hw_queues;
    unsigned int queue_depth;
    unsigned int reserved_tags;
    unsigned int cmd_size;
    int numa_node;
    unsigned int timeout;
    unsigned int flags;
    void *driver_data;
    struct blk_mq_tags **tags;
    struct blk_mq_tags *shared_tags;
    struct mutex tag_list_lock;
    struct list_head tag_list;
    struct srcu_struct *srcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct blk_mq_tag_set {
    const struct blk_mq_ops *ops;
    struct blk_mq_queue_map map[3];
    unsigned int nr_maps;
    unsigned int nr_hw_queues;
    unsigned int queue_depth;
    unsigned int reserved_tags;
    unsigned int cmd_size;
    int numa_node;
    unsigned int timeout;
    unsigned int flags;
    void *driver_data;
    struct blk_mq_tags **tags;
    struct blk_mq_tags *shared_tags;
    struct mutex tag_list_lock;
    struct list_head tag_list;
    struct srcu_struct *srcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct blk_mq_tag_set {
    const struct blk_mq_ops *ops;
    struct blk_mq_queue_map map[3];
    unsigned int nr_maps;
    unsigned int nr_hw_queues;
    unsigned int queue_depth;
    unsigned int reserved_tags;
    unsigned int cmd_size;
    int numa_node;
    unsigned int timeout;
    unsigned int flags;
    void *driver_data;
    struct blk_mq_tags **tags;
    struct blk_mq_tags *shared_tags;
    struct mutex tag_list_lock;
    struct list_head tag_list;
    struct srcu_struct *srcu;
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
struct blk_mq_tag_set {
    struct blk_mq_queue_map map[3];
    unsigned int nr_maps;
    const struct blk_mq_ops *ops;
    unsigned int nr_hw_queues;
    unsigned int queue_depth;
    unsigned int reserved_tags;
    unsigned int cmd_size;
    int numa_node;
    unsigned int timeout;
    unsigned int flags;
    void *driver_data;
    struct blk_mq_tags **tags;
    struct mutex tag_list_lock;
    struct list_head tag_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct blk_mq_tag_set {
    struct blk_mq_queue_map map[3];
    unsigned int nr_maps;
    const struct blk_mq_ops *ops;
    unsigned int nr_hw_queues;
    unsigned int queue_depth;
    unsigned int reserved_tags;
    unsigned int cmd_size;
    int numa_node;
    unsigned int timeout;
    unsigned int flags;
    void *driver_data;
    struct blk_mq_tags **tags;
    struct mutex tag_list_lock;
    struct list_head tag_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct blk_mq_tag_set {
    struct blk_mq_queue_map map[3];
    unsigned int nr_maps;
    const struct blk_mq_ops *ops;
    unsigned int nr_hw_queues;
    unsigned int queue_depth;
    unsigned int reserved_tags;
    unsigned int cmd_size;
    int numa_node;
    unsigned int timeout;
    unsigned int flags;
    void *driver_data;
    struct blk_mq_tags **tags;
    struct mutex tag_list_lock;
    struct list_head tag_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct blk_mq_tag_set {
    struct blk_mq_queue_map map[3];
    unsigned int nr_maps;
    const struct blk_mq_ops *ops;
    unsigned int nr_hw_queues;
    unsigned int queue_depth;
    unsigned int reserved_tags;
    unsigned int cmd_size;
    int numa_node;
    unsigned int timeout;
    unsigned int flags;
    void *driver_data;
    struct blk_mq_tags **tags;
    struct mutex tag_list_lock;
    struct list_head tag_list;
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
struct blk_mq_tag_set {
    struct blk_mq_queue_map map[3];
    unsigned int nr_maps;
    const struct blk_mq_ops *ops;
    unsigned int nr_hw_queues;
    unsigned int queue_depth;
    unsigned int reserved_tags;
    unsigned int cmd_size;
    int numa_node;
    unsigned int timeout;
    unsigned int flags;
    void *driver_data;
    struct blk_mq_tags **tags;
    struct mutex tag_list_lock;
    struct list_head tag_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct blk_mq_tag_set {
    struct blk_mq_queue_map map[3];
    unsigned int nr_maps;
    const struct blk_mq_ops *ops;
    unsigned int nr_hw_queues;
    unsigned int queue_depth;
    unsigned int reserved_tags;
    unsigned int cmd_size;
    int numa_node;
    unsigned int timeout;
    unsigned int flags;
    void *driver_data;
    struct blk_mq_tags **tags;
    struct mutex tag_list_lock;
    struct list_head tag_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct blk_mq_tag_set {
    struct blk_mq_queue_map map[3];
    unsigned int nr_maps;
    const struct blk_mq_ops *ops;
    unsigned int nr_hw_queues;
    unsigned int queue_depth;
    unsigned int reserved_tags;
    unsigned int cmd_size;
    int numa_node;
    unsigned int timeout;
    unsigned int flags;
    void *driver_data;
    struct blk_mq_tags **tags;
    struct mutex tag_list_lock;
    struct list_head tag_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct blk_mq_tag_set {
    struct blk_mq_queue_map map[3];
    unsigned int nr_maps;
    const struct blk_mq_ops *ops;
    unsigned int nr_hw_queues;
    unsigned int queue_depth;
    unsigned int reserved_tags;
    unsigned int cmd_size;
    int numa_node;
    unsigned int timeout;
    unsigned int flags;
    void *driver_data;
    struct blk_mq_tags **tags;
    struct mutex tag_list_lock;
    struct list_head tag_list;
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
<b>Field added. </b>
<code>unsigned int *mq_map</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct blk_mq_ops *ops</code> ➡️ <code>const struct blk_mq_ops *ops</code>
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
<b>Field added. </b>
<code>struct blk_mq_queue_map map[3]</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int nr_maps</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int *mq_map</code>
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
<b>Field added. </b>
<code>atomic_t active_queues_shared_sbitmap</code>
</li>
<li>
<b>Field added. </b>
<code>struct sbitmap_queue __bitmap_tags</code>
</li>
<li>
<b>Field added. </b>
<code>struct sbitmap_queue __breserved_tags</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct blk_mq_tags *shared_tags</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t active_queues_shared_sbitmap</code>
</li>
<li>
<b>Field removed. </b>
<code>struct sbitmap_queue __bitmap_tags</code>
</li>
<li>
<b>Field removed. </b>
<code>struct sbitmap_queue __breserved_tags</code>
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
<code>struct srcu_struct *srcu</code>
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
