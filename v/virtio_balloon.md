# Struct: <code>virtio_balloon</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct virtio_balloon {
    struct virtio_device *vdev;
    struct virtqueue *inflate_vq;
    struct virtqueue *deflate_vq;
    struct virtqueue *stats_vq;
    wait_queue_head_t config_change;
    struct task_struct *thread;
    wait_queue_head_t acked;
    unsigned int num_pages;
    struct balloon_dev_info vb_dev_info;
    struct mutex balloon_lock;
    unsigned int num_pfns;
    u32 pfns[256];
    int need_stats_update;
    struct virtio_balloon_stat stats[6];
    struct notifier_block nb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct virtio_balloon {
    struct virtio_device *vdev;
    struct virtqueue *inflate_vq;
    struct virtqueue *deflate_vq;
    struct virtqueue *stats_vq;
    struct work_struct update_balloon_stats_work;
    struct work_struct update_balloon_size_work;
    spinlock_t stop_update_lock;
    bool stop_update;
    wait_queue_head_t acked;
    unsigned int num_pages;
    struct balloon_dev_info vb_dev_info;
    struct mutex balloon_lock;
    unsigned int num_pfns;
    __virtio32 pfns[256];
    struct virtio_balloon_stat stats[7];
    struct notifier_block nb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct virtio_balloon {
    struct virtio_device *vdev;
    struct virtqueue *inflate_vq;
    struct virtqueue *deflate_vq;
    struct virtqueue *stats_vq;
    struct work_struct update_balloon_stats_work;
    struct work_struct update_balloon_size_work;
    spinlock_t stop_update_lock;
    bool stop_update;
    wait_queue_head_t acked;
    unsigned int num_pages;
    struct balloon_dev_info vb_dev_info;
    struct mutex balloon_lock;
    unsigned int num_pfns;
    __virtio32 pfns[256];
    struct virtio_balloon_stat stats[7];
    struct notifier_block nb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct virtio_balloon {
    struct virtio_device *vdev;
    struct virtqueue *inflate_vq;
    struct virtqueue *deflate_vq;
    struct virtqueue *stats_vq;
    struct work_struct update_balloon_stats_work;
    struct work_struct update_balloon_size_work;
    spinlock_t stop_update_lock;
    bool stop_update;
    wait_queue_head_t acked;
    unsigned int num_pages;
    struct balloon_dev_info vb_dev_info;
    struct mutex balloon_lock;
    unsigned int num_pfns;
    __virtio32 pfns[256];
    struct virtio_balloon_stat stats[7];
    struct notifier_block nb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct virtio_balloon {
    struct virtio_device *vdev;
    struct virtqueue *inflate_vq;
    struct virtqueue *deflate_vq;
    struct virtqueue *stats_vq;
    struct work_struct update_balloon_stats_work;
    struct work_struct update_balloon_size_work;
    spinlock_t stop_update_lock;
    bool stop_update;
    wait_queue_head_t acked;
    unsigned int num_pages;
    struct balloon_dev_info vb_dev_info;
    struct mutex balloon_lock;
    unsigned int num_pfns;
    __virtio32 pfns[256];
    struct virtio_balloon_stat stats[7];
    struct notifier_block nb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct virtio_balloon {
    struct virtio_device *vdev;
    struct virtqueue *inflate_vq;
    struct virtqueue *deflate_vq;
    struct virtqueue *stats_vq;
    struct work_struct update_balloon_stats_work;
    struct work_struct update_balloon_size_work;
    spinlock_t stop_update_lock;
    bool stop_update;
    wait_queue_head_t acked;
    unsigned int num_pages;
    struct balloon_dev_info vb_dev_info;
    struct mutex balloon_lock;
    unsigned int num_pfns;
    __virtio32 pfns[256];
    struct virtio_balloon_stat stats[10];
    struct notifier_block nb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct virtio_balloon {
    struct virtio_device *vdev;
    struct virtqueue *inflate_vq;
    struct virtqueue *deflate_vq;
    struct virtqueue *stats_vq;
    struct virtqueue *free_page_vq;
    struct workqueue_struct *balloon_wq;
    struct work_struct report_free_page_work;
    struct work_struct update_balloon_stats_work;
    struct work_struct update_balloon_size_work;
    spinlock_t stop_update_lock;
    bool stop_update;
    long unsigned int config_read_bitmap;
    struct list_head free_page_list;
    spinlock_t free_page_list_lock;
    long unsigned int num_free_page_blocks;
    u32 cmd_id_received_cache;
    __virtio32 cmd_id_active;
    __virtio32 cmd_id_stop;
    wait_queue_head_t acked;
    unsigned int num_pages;
    struct balloon_dev_info vb_dev_info;
    struct mutex balloon_lock;
    unsigned int num_pfns;
    __virtio32 pfns[256];
    struct virtio_balloon_stat stats[10];
    struct shrinker shrinker;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct virtio_balloon {
    struct virtio_device *vdev;
    struct virtqueue *inflate_vq;
    struct virtqueue *deflate_vq;
    struct virtqueue *stats_vq;
    struct virtqueue *free_page_vq;
    struct workqueue_struct *balloon_wq;
    struct work_struct report_free_page_work;
    struct work_struct update_balloon_stats_work;
    struct work_struct update_balloon_size_work;
    spinlock_t stop_update_lock;
    bool stop_update;
    long unsigned int config_read_bitmap;
    struct list_head free_page_list;
    spinlock_t free_page_list_lock;
    long unsigned int num_free_page_blocks;
    u32 cmd_id_received_cache;
    __virtio32 cmd_id_active;
    __virtio32 cmd_id_stop;
    wait_queue_head_t acked;
    unsigned int num_pages;
    struct balloon_dev_info vb_dev_info;
    struct mutex balloon_lock;
    unsigned int num_pfns;
    __virtio32 pfns[256];
    struct virtio_balloon_stat stats[10];
    struct shrinker shrinker;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct virtio_balloon {
    struct virtio_device *vdev;
    struct virtqueue *inflate_vq;
    struct virtqueue *deflate_vq;
    struct virtqueue *stats_vq;
    struct virtqueue *free_page_vq;
    struct workqueue_struct *balloon_wq;
    struct work_struct report_free_page_work;
    struct work_struct update_balloon_stats_work;
    struct work_struct update_balloon_size_work;
    spinlock_t stop_update_lock;
    bool stop_update;
    long unsigned int config_read_bitmap;
    struct list_head free_page_list;
    spinlock_t free_page_list_lock;
    long unsigned int num_free_page_blocks;
    u32 cmd_id_received_cache;
    __virtio32 cmd_id_active;
    __virtio32 cmd_id_stop;
    wait_queue_head_t acked;
    unsigned int num_pages;
    struct balloon_dev_info vb_dev_info;
    struct mutex balloon_lock;
    unsigned int num_pfns;
    __virtio32 pfns[256];
    struct virtio_balloon_stat stats[10];
    struct shrinker shrinker;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct virtio_balloon {
    struct virtio_device *vdev;
    struct virtqueue *inflate_vq;
    struct virtqueue *deflate_vq;
    struct virtqueue *stats_vq;
    struct virtqueue *free_page_vq;
    struct workqueue_struct *balloon_wq;
    struct work_struct report_free_page_work;
    struct work_struct update_balloon_stats_work;
    struct work_struct update_balloon_size_work;
    spinlock_t stop_update_lock;
    bool stop_update;
    long unsigned int config_read_bitmap;
    struct list_head free_page_list;
    spinlock_t free_page_list_lock;
    long unsigned int num_free_page_blocks;
    u32 cmd_id_received_cache;
    __virtio32 cmd_id_active;
    __virtio32 cmd_id_stop;
    wait_queue_head_t acked;
    unsigned int num_pages;
    struct balloon_dev_info vb_dev_info;
    struct mutex balloon_lock;
    unsigned int num_pfns;
    __virtio32 pfns[256];
    struct virtio_balloon_stat stats[10];
    struct shrinker shrinker;
    struct notifier_block oom_nb;
    struct virtqueue *reporting_vq;
    struct page_reporting_dev_info pr_dev_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct virtio_balloon {
    struct virtio_device *vdev;
    struct virtqueue *inflate_vq;
    struct virtqueue *deflate_vq;
    struct virtqueue *stats_vq;
    struct virtqueue *free_page_vq;
    struct workqueue_struct *balloon_wq;
    struct work_struct report_free_page_work;
    struct work_struct update_balloon_stats_work;
    struct work_struct update_balloon_size_work;
    spinlock_t stop_update_lock;
    bool stop_update;
    long unsigned int config_read_bitmap;
    struct list_head free_page_list;
    spinlock_t free_page_list_lock;
    long unsigned int num_free_page_blocks;
    u32 cmd_id_received_cache;
    __virtio32 cmd_id_active;
    __virtio32 cmd_id_stop;
    wait_queue_head_t acked;
    unsigned int num_pages;
    struct balloon_dev_info vb_dev_info;
    struct mutex balloon_lock;
    unsigned int num_pfns;
    __virtio32 pfns[256];
    struct virtio_balloon_stat stats[10];
    struct shrinker shrinker;
    struct notifier_block oom_nb;
    struct virtqueue *reporting_vq;
    struct page_reporting_dev_info pr_dev_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct virtio_balloon {
    struct virtio_device *vdev;
    struct virtqueue *inflate_vq;
    struct virtqueue *deflate_vq;
    struct virtqueue *stats_vq;
    struct virtqueue *free_page_vq;
    struct workqueue_struct *balloon_wq;
    struct work_struct report_free_page_work;
    struct work_struct update_balloon_stats_work;
    struct work_struct update_balloon_size_work;
    spinlock_t stop_update_lock;
    bool stop_update;
    long unsigned int config_read_bitmap;
    struct list_head free_page_list;
    spinlock_t free_page_list_lock;
    long unsigned int num_free_page_blocks;
    u32 cmd_id_received_cache;
    __virtio32 cmd_id_active;
    __virtio32 cmd_id_stop;
    wait_queue_head_t acked;
    unsigned int num_pages;
    struct balloon_dev_info vb_dev_info;
    struct mutex balloon_lock;
    unsigned int num_pfns;
    __virtio32 pfns[256];
    struct virtio_balloon_stat stats[10];
    struct shrinker shrinker;
    struct notifier_block oom_nb;
    struct virtqueue *reporting_vq;
    struct page_reporting_dev_info pr_dev_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct virtio_balloon {
    struct virtio_device *vdev;
    struct virtqueue *inflate_vq;
    struct virtqueue *deflate_vq;
    struct virtqueue *stats_vq;
    struct virtqueue *free_page_vq;
    struct workqueue_struct *balloon_wq;
    struct work_struct report_free_page_work;
    struct work_struct update_balloon_stats_work;
    struct work_struct update_balloon_size_work;
    spinlock_t stop_update_lock;
    bool stop_update;
    long unsigned int config_read_bitmap;
    struct list_head free_page_list;
    spinlock_t free_page_list_lock;
    long unsigned int num_free_page_blocks;
    u32 cmd_id_received_cache;
    __virtio32 cmd_id_active;
    __virtio32 cmd_id_stop;
    wait_queue_head_t acked;
    unsigned int num_pages;
    struct balloon_dev_info vb_dev_info;
    struct mutex balloon_lock;
    unsigned int num_pfns;
    __virtio32 pfns[256];
    struct virtio_balloon_stat stats[10];
    struct shrinker shrinker;
    struct notifier_block oom_nb;
    struct virtqueue *reporting_vq;
    struct page_reporting_dev_info pr_dev_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct virtio_balloon {
    struct virtio_device *vdev;
    struct virtqueue *inflate_vq;
    struct virtqueue *deflate_vq;
    struct virtqueue *stats_vq;
    struct virtqueue *free_page_vq;
    struct workqueue_struct *balloon_wq;
    struct work_struct report_free_page_work;
    struct work_struct update_balloon_stats_work;
    struct work_struct update_balloon_size_work;
    spinlock_t stop_update_lock;
    bool stop_update;
    long unsigned int config_read_bitmap;
    struct list_head free_page_list;
    spinlock_t free_page_list_lock;
    long unsigned int num_free_page_blocks;
    u32 cmd_id_received_cache;
    __virtio32 cmd_id_active;
    __virtio32 cmd_id_stop;
    wait_queue_head_t acked;
    unsigned int num_pages;
    struct balloon_dev_info vb_dev_info;
    struct mutex balloon_lock;
    unsigned int num_pfns;
    __virtio32 pfns[256];
    struct virtio_balloon_stat stats[10];
    struct shrinker shrinker;
    struct notifier_block oom_nb;
    struct virtqueue *reporting_vq;
    struct page_reporting_dev_info pr_dev_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct virtio_balloon {
    struct virtio_device *vdev;
    struct virtqueue *inflate_vq;
    struct virtqueue *deflate_vq;
    struct virtqueue *stats_vq;
    struct virtqueue *free_page_vq;
    struct workqueue_struct *balloon_wq;
    struct work_struct report_free_page_work;
    struct work_struct update_balloon_stats_work;
    struct work_struct update_balloon_size_work;
    spinlock_t stop_update_lock;
    bool stop_update;
    long unsigned int config_read_bitmap;
    struct list_head free_page_list;
    spinlock_t free_page_list_lock;
    long unsigned int num_free_page_blocks;
    u32 cmd_id_received_cache;
    __virtio32 cmd_id_active;
    __virtio32 cmd_id_stop;
    wait_queue_head_t acked;
    unsigned int num_pages;
    struct balloon_dev_info vb_dev_info;
    struct mutex balloon_lock;
    unsigned int num_pfns;
    __virtio32 pfns[256];
    struct virtio_balloon_stat stats[10];
    struct shrinker shrinker;
    struct notifier_block oom_nb;
    struct virtqueue *reporting_vq;
    struct page_reporting_dev_info pr_dev_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct virtio_balloon {
    struct virtio_device *vdev;
    struct virtqueue *inflate_vq;
    struct virtqueue *deflate_vq;
    struct virtqueue *stats_vq;
    struct virtqueue *free_page_vq;
    struct workqueue_struct *balloon_wq;
    struct work_struct report_free_page_work;
    struct work_struct update_balloon_stats_work;
    struct work_struct update_balloon_size_work;
    spinlock_t stop_update_lock;
    bool stop_update;
    long unsigned int config_read_bitmap;
    struct list_head free_page_list;
    spinlock_t free_page_list_lock;
    long unsigned int num_free_page_blocks;
    u32 cmd_id_received_cache;
    __virtio32 cmd_id_active;
    __virtio32 cmd_id_stop;
    wait_queue_head_t acked;
    unsigned int num_pages;
    struct balloon_dev_info vb_dev_info;
    struct mutex balloon_lock;
    unsigned int num_pfns;
    __virtio32 pfns[256];
    struct virtio_balloon_stat stats[10];
    struct shrinker shrinker;
    struct notifier_block oom_nb;
    struct virtqueue *reporting_vq;
    struct page_reporting_dev_info pr_dev_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct virtio_balloon {
    struct virtio_device *vdev;
    struct virtqueue *inflate_vq;
    struct virtqueue *deflate_vq;
    struct virtqueue *stats_vq;
    struct virtqueue *free_page_vq;
    struct workqueue_struct *balloon_wq;
    struct work_struct report_free_page_work;
    struct work_struct update_balloon_stats_work;
    struct work_struct update_balloon_size_work;
    spinlock_t stop_update_lock;
    bool stop_update;
    long unsigned int config_read_bitmap;
    struct list_head free_page_list;
    spinlock_t free_page_list_lock;
    long unsigned int num_free_page_blocks;
    u32 cmd_id_received_cache;
    __virtio32 cmd_id_active;
    __virtio32 cmd_id_stop;
    wait_queue_head_t acked;
    unsigned int num_pages;
    struct balloon_dev_info vb_dev_info;
    struct mutex balloon_lock;
    unsigned int num_pfns;
    __virtio32 pfns[256];
    struct virtio_balloon_stat stats[10];
    struct shrinker *shrinker;
    struct notifier_block oom_nb;
    struct virtqueue *reporting_vq;
    struct page_reporting_dev_info pr_dev_info;
    spinlock_t adjustment_lock;
    bool adjustment_signal_pending;
    bool adjustment_in_progress;
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
struct virtio_balloon {
    struct virtio_device *vdev;
    struct virtqueue *inflate_vq;
    struct virtqueue *deflate_vq;
    struct virtqueue *stats_vq;
    struct virtqueue *free_page_vq;
    struct workqueue_struct *balloon_wq;
    struct work_struct report_free_page_work;
    struct work_struct update_balloon_stats_work;
    struct work_struct update_balloon_size_work;
    spinlock_t stop_update_lock;
    bool stop_update;
    long unsigned int config_read_bitmap;
    struct list_head free_page_list;
    spinlock_t free_page_list_lock;
    long unsigned int num_free_page_blocks;
    u32 cmd_id_received_cache;
    __virtio32 cmd_id_active;
    __virtio32 cmd_id_stop;
    wait_queue_head_t acked;
    unsigned int num_pages;
    struct balloon_dev_info vb_dev_info;
    struct mutex balloon_lock;
    unsigned int num_pfns;
    __virtio32 pfns[256];
    struct virtio_balloon_stat stats[10];
    struct shrinker shrinker;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct virtio_balloon {
    struct virtio_device *vdev;
    struct virtqueue *inflate_vq;
    struct virtqueue *deflate_vq;
    struct virtqueue *stats_vq;
    struct virtqueue *free_page_vq;
    struct workqueue_struct *balloon_wq;
    struct work_struct report_free_page_work;
    struct work_struct update_balloon_stats_work;
    struct work_struct update_balloon_size_work;
    spinlock_t stop_update_lock;
    bool stop_update;
    long unsigned int config_read_bitmap;
    struct list_head free_page_list;
    spinlock_t free_page_list_lock;
    long unsigned int num_free_page_blocks;
    u32 cmd_id_received_cache;
    __virtio32 cmd_id_active;
    __virtio32 cmd_id_stop;
    wait_queue_head_t acked;
    unsigned int num_pages;
    struct balloon_dev_info vb_dev_info;
    struct mutex balloon_lock;
    unsigned int num_pfns;
    __virtio32 pfns[256];
    struct virtio_balloon_stat stats[10];
    struct shrinker shrinker;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct virtio_balloon {
    struct virtio_device *vdev;
    struct virtqueue *inflate_vq;
    struct virtqueue *deflate_vq;
    struct virtqueue *stats_vq;
    struct virtqueue *free_page_vq;
    struct workqueue_struct *balloon_wq;
    struct work_struct report_free_page_work;
    struct work_struct update_balloon_stats_work;
    struct work_struct update_balloon_size_work;
    spinlock_t stop_update_lock;
    bool stop_update;
    long unsigned int config_read_bitmap;
    struct list_head free_page_list;
    spinlock_t free_page_list_lock;
    long unsigned int num_free_page_blocks;
    u32 cmd_id_received_cache;
    __virtio32 cmd_id_active;
    __virtio32 cmd_id_stop;
    wait_queue_head_t acked;
    unsigned int num_pages;
    struct balloon_dev_info vb_dev_info;
    struct mutex balloon_lock;
    unsigned int num_pfns;
    __virtio32 pfns[256];
    struct virtio_balloon_stat stats[10];
    struct shrinker shrinker;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct virtio_balloon {
    struct virtio_device *vdev;
    struct virtqueue *inflate_vq;
    struct virtqueue *deflate_vq;
    struct virtqueue *stats_vq;
    struct virtqueue *free_page_vq;
    struct workqueue_struct *balloon_wq;
    struct work_struct report_free_page_work;
    struct work_struct update_balloon_stats_work;
    struct work_struct update_balloon_size_work;
    spinlock_t stop_update_lock;
    bool stop_update;
    long unsigned int config_read_bitmap;
    struct list_head free_page_list;
    spinlock_t free_page_list_lock;
    long unsigned int num_free_page_blocks;
    u32 cmd_id_received_cache;
    __virtio32 cmd_id_active;
    __virtio32 cmd_id_stop;
    wait_queue_head_t acked;
    unsigned int num_pages;
    struct balloon_dev_info vb_dev_info;
    struct mutex balloon_lock;
    unsigned int num_pfns;
    __virtio32 pfns[256];
    struct virtio_balloon_stat stats[10];
    struct shrinker shrinker;
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
struct virtio_balloon {
    struct virtio_device *vdev;
    struct virtqueue *inflate_vq;
    struct virtqueue *deflate_vq;
    struct virtqueue *stats_vq;
    struct virtqueue *free_page_vq;
    struct workqueue_struct *balloon_wq;
    struct work_struct report_free_page_work;
    struct work_struct update_balloon_stats_work;
    struct work_struct update_balloon_size_work;
    spinlock_t stop_update_lock;
    bool stop_update;
    long unsigned int config_read_bitmap;
    struct list_head free_page_list;
    spinlock_t free_page_list_lock;
    long unsigned int num_free_page_blocks;
    u32 cmd_id_received_cache;
    __virtio32 cmd_id_active;
    __virtio32 cmd_id_stop;
    wait_queue_head_t acked;
    unsigned int num_pages;
    struct balloon_dev_info vb_dev_info;
    struct mutex balloon_lock;
    unsigned int num_pfns;
    __virtio32 pfns[256];
    struct virtio_balloon_stat stats[10];
    struct shrinker shrinker;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct virtio_balloon {
    struct virtio_device *vdev;
    struct virtqueue *inflate_vq;
    struct virtqueue *deflate_vq;
    struct virtqueue *stats_vq;
    struct virtqueue *free_page_vq;
    struct workqueue_struct *balloon_wq;
    struct work_struct report_free_page_work;
    struct work_struct update_balloon_stats_work;
    struct work_struct update_balloon_size_work;
    spinlock_t stop_update_lock;
    bool stop_update;
    long unsigned int config_read_bitmap;
    struct list_head free_page_list;
    spinlock_t free_page_list_lock;
    long unsigned int num_free_page_blocks;
    u32 cmd_id_received_cache;
    __virtio32 cmd_id_active;
    __virtio32 cmd_id_stop;
    wait_queue_head_t acked;
    unsigned int num_pages;
    struct balloon_dev_info vb_dev_info;
    struct mutex balloon_lock;
    unsigned int num_pfns;
    __virtio32 pfns[256];
    struct virtio_balloon_stat stats[10];
    struct shrinker shrinker;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct virtio_balloon {
    struct virtio_device *vdev;
    struct virtqueue *inflate_vq;
    struct virtqueue *deflate_vq;
    struct virtqueue *stats_vq;
    struct virtqueue *free_page_vq;
    struct workqueue_struct *balloon_wq;
    struct work_struct report_free_page_work;
    struct work_struct update_balloon_stats_work;
    struct work_struct update_balloon_size_work;
    spinlock_t stop_update_lock;
    bool stop_update;
    long unsigned int config_read_bitmap;
    struct list_head free_page_list;
    spinlock_t free_page_list_lock;
    long unsigned int num_free_page_blocks;
    u32 cmd_id_received_cache;
    __virtio32 cmd_id_active;
    __virtio32 cmd_id_stop;
    wait_queue_head_t acked;
    unsigned int num_pages;
    struct balloon_dev_info vb_dev_info;
    struct mutex balloon_lock;
    unsigned int num_pfns;
    __virtio32 pfns[256];
    struct virtio_balloon_stat stats[10];
    struct shrinker shrinker;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct virtio_balloon {
    struct virtio_device *vdev;
    struct virtqueue *inflate_vq;
    struct virtqueue *deflate_vq;
    struct virtqueue *stats_vq;
    struct virtqueue *free_page_vq;
    struct workqueue_struct *balloon_wq;
    struct work_struct report_free_page_work;
    struct work_struct update_balloon_stats_work;
    struct work_struct update_balloon_size_work;
    spinlock_t stop_update_lock;
    bool stop_update;
    long unsigned int config_read_bitmap;
    struct list_head free_page_list;
    spinlock_t free_page_list_lock;
    long unsigned int num_free_page_blocks;
    u32 cmd_id_received_cache;
    __virtio32 cmd_id_active;
    __virtio32 cmd_id_stop;
    wait_queue_head_t acked;
    unsigned int num_pages;
    struct balloon_dev_info vb_dev_info;
    struct mutex balloon_lock;
    unsigned int num_pfns;
    __virtio32 pfns[256];
    struct virtio_balloon_stat stats[10];
    struct shrinker shrinker;
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
<code>struct work_struct update_balloon_stats_work</code>
</li>
<li>
<b>Field added. </b>
<code>struct work_struct update_balloon_size_work</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t stop_update_lock</code>
</li>
<li>
<b>Field added. </b>
<code>bool stop_update</code>
</li>
<li>
<b>Field removed. </b>
<code>wait_queue_head_t config_change</code>
</li>
<li>
<b>Field removed. </b>
<code>struct task_struct *thread</code>
</li>
<li>
<b>Field removed. </b>
<code>int need_stats_update</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 pfns[256]</code> ➡️ <code>__virtio32 pfns[256]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct virtio_balloon_stat stats[6]</code> ➡️ <code>struct virtio_balloon_stat stats[7]</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct virtio_balloon_stat stats[7]</code> ➡️ <code>struct virtio_balloon_stat stats[10]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct virtqueue *free_page_vq</code>
</li>
<li>
<b>Field added. </b>
<code>struct workqueue_struct *balloon_wq</code>
</li>
<li>
<b>Field added. </b>
<code>struct work_struct report_free_page_work</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int config_read_bitmap</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head free_page_list</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t free_page_list_lock</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int num_free_page_blocks</code>
</li>
<li>
<b>Field added. </b>
<code>u32 cmd_id_received_cache</code>
</li>
<li>
<b>Field added. </b>
<code>__virtio32 cmd_id_active</code>
</li>
<li>
<b>Field added. </b>
<code>__virtio32 cmd_id_stop</code>
</li>
<li>
<b>Field added. </b>
<code>struct shrinker shrinker</code>
</li>
<li>
<b>Field removed. </b>
<code>struct notifier_block nb</code>
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
<code>struct notifier_block oom_nb</code>
</li>
<li>
<b>Field added. </b>
<code>struct virtqueue *reporting_vq</code>
</li>
<li>
<b>Field added. </b>
<code>struct page_reporting_dev_info pr_dev_info</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>spinlock_t adjustment_lock</code>
</li>
<li>
<b>Field added. </b>
<code>bool adjustment_signal_pending</code>
</li>
<li>
<b>Field added. </b>
<code>bool adjustment_in_progress</code>
</li>
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
