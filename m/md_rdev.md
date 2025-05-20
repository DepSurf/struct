# Struct: <code>md_rdev</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct md_rdev {
    struct list_head same_set;
    sector_t sectors;
    struct mddev *mddev;
    int last_events;
    struct block_device *meta_bdev;
    struct block_device *bdev;
    struct page *sb_page;
    struct page *bb_page;
    int sb_loaded;
    __u64 sb_events;
    sector_t data_offset;
    sector_t new_data_offset;
    sector_t sb_start;
    int sb_size;
    int preferred_minor;
    struct kobject kobj;
    long unsigned int flags;
    wait_queue_head_t blocked_wait;
    int desc_nr;
    int raid_disk;
    int new_raid_disk;
    int saved_raid_disk;
    sector_t recovery_offset;
    sector_t journal_tail;
    atomic_t nr_pending;
    atomic_t read_errors;
    struct timespec last_read_error;
    atomic_t corrected_errors;
    struct work_struct del_work;
    struct kernfs_node *sysfs_state;
    struct badblocks badblocks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct md_rdev {
    struct list_head same_set;
    sector_t sectors;
    struct mddev *mddev;
    int last_events;
    struct block_device *meta_bdev;
    struct block_device *bdev;
    struct page *sb_page;
    struct page *bb_page;
    int sb_loaded;
    __u64 sb_events;
    sector_t data_offset;
    sector_t new_data_offset;
    sector_t sb_start;
    int sb_size;
    int preferred_minor;
    struct kobject kobj;
    long unsigned int flags;
    wait_queue_head_t blocked_wait;
    int desc_nr;
    int raid_disk;
    int new_raid_disk;
    int saved_raid_disk;
    sector_t recovery_offset;
    sector_t journal_tail;
    atomic_t nr_pending;
    atomic_t read_errors;
    time64_t last_read_error;
    atomic_t corrected_errors;
    struct work_struct del_work;
    struct kernfs_node *sysfs_state;
    struct badblocks badblocks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct md_rdev {
    struct list_head same_set;
    sector_t sectors;
    struct mddev *mddev;
    int last_events;
    struct block_device *meta_bdev;
    struct block_device *bdev;
    struct page *sb_page;
    struct page *bb_page;
    int sb_loaded;
    __u64 sb_events;
    sector_t data_offset;
    sector_t new_data_offset;
    sector_t sb_start;
    int sb_size;
    int preferred_minor;
    struct kobject kobj;
    long unsigned int flags;
    wait_queue_head_t blocked_wait;
    int desc_nr;
    int raid_disk;
    int new_raid_disk;
    int saved_raid_disk;
    sector_t recovery_offset;
    sector_t journal_tail;
    atomic_t nr_pending;
    atomic_t read_errors;
    time64_t last_read_error;
    atomic_t corrected_errors;
    struct work_struct del_work;
    struct kernfs_node *sysfs_state;
    struct badblocks badblocks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct md_rdev {
    struct list_head same_set;
    sector_t sectors;
    struct mddev *mddev;
    int last_events;
    struct block_device *meta_bdev;
    struct block_device *bdev;
    struct page *sb_page;
    struct page *bb_page;
    int sb_loaded;
    __u64 sb_events;
    sector_t data_offset;
    sector_t new_data_offset;
    sector_t sb_start;
    int sb_size;
    int preferred_minor;
    struct kobject kobj;
    long unsigned int flags;
    wait_queue_head_t blocked_wait;
    int desc_nr;
    int raid_disk;
    int new_raid_disk;
    int saved_raid_disk;
    sector_t recovery_offset;
    sector_t journal_tail;
    atomic_t nr_pending;
    atomic_t read_errors;
    time64_t last_read_error;
    atomic_t corrected_errors;
    struct work_struct del_work;
    struct kernfs_node *sysfs_state;
    struct badblocks badblocks;
    struct (anon) ppl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct md_rdev {
    struct list_head same_set;
    sector_t sectors;
    struct mddev *mddev;
    int last_events;
    struct block_device *meta_bdev;
    struct block_device *bdev;
    struct page *sb_page;
    struct page *bb_page;
    int sb_loaded;
    __u64 sb_events;
    sector_t data_offset;
    sector_t new_data_offset;
    sector_t sb_start;
    int sb_size;
    int preferred_minor;
    struct kobject kobj;
    long unsigned int flags;
    wait_queue_head_t blocked_wait;
    int desc_nr;
    int raid_disk;
    int new_raid_disk;
    int saved_raid_disk;
    sector_t recovery_offset;
    sector_t journal_tail;
    atomic_t nr_pending;
    atomic_t read_errors;
    time64_t last_read_error;
    atomic_t corrected_errors;
    struct work_struct del_work;
    struct kernfs_node *sysfs_state;
    struct badblocks badblocks;
    struct (anon) ppl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct md_rdev {
    struct list_head same_set;
    sector_t sectors;
    struct mddev *mddev;
    int last_events;
    struct block_device *meta_bdev;
    struct block_device *bdev;
    struct page *sb_page;
    struct page *bb_page;
    int sb_loaded;
    __u64 sb_events;
    sector_t data_offset;
    sector_t new_data_offset;
    sector_t sb_start;
    int sb_size;
    int preferred_minor;
    struct kobject kobj;
    long unsigned int flags;
    wait_queue_head_t blocked_wait;
    int desc_nr;
    int raid_disk;
    int new_raid_disk;
    int saved_raid_disk;
    sector_t recovery_offset;
    sector_t journal_tail;
    atomic_t nr_pending;
    atomic_t read_errors;
    time64_t last_read_error;
    atomic_t corrected_errors;
    struct work_struct del_work;
    struct kernfs_node *sysfs_state;
    struct badblocks badblocks;
    struct (anon) ppl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct md_rdev {
    struct list_head same_set;
    sector_t sectors;
    struct mddev *mddev;
    int last_events;
    struct block_device *meta_bdev;
    struct block_device *bdev;
    struct page *sb_page;
    struct page *bb_page;
    int sb_loaded;
    __u64 sb_events;
    sector_t data_offset;
    sector_t new_data_offset;
    sector_t sb_start;
    int sb_size;
    int preferred_minor;
    struct kobject kobj;
    long unsigned int flags;
    wait_queue_head_t blocked_wait;
    int desc_nr;
    int raid_disk;
    int new_raid_disk;
    int saved_raid_disk;
    sector_t recovery_offset;
    sector_t journal_tail;
    atomic_t nr_pending;
    atomic_t read_errors;
    time64_t last_read_error;
    atomic_t corrected_errors;
    struct work_struct del_work;
    struct kernfs_node *sysfs_state;
    struct badblocks badblocks;
    struct (anon) ppl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct md_rdev {
    struct list_head same_set;
    sector_t sectors;
    struct mddev *mddev;
    int last_events;
    struct block_device *meta_bdev;
    struct block_device *bdev;
    struct page *sb_page;
    struct page *bb_page;
    int sb_loaded;
    __u64 sb_events;
    sector_t data_offset;
    sector_t new_data_offset;
    sector_t sb_start;
    int sb_size;
    int preferred_minor;
    struct kobject kobj;
    long unsigned int flags;
    wait_queue_head_t blocked_wait;
    int desc_nr;
    int raid_disk;
    int new_raid_disk;
    int saved_raid_disk;
    sector_t recovery_offset;
    sector_t journal_tail;
    atomic_t nr_pending;
    atomic_t read_errors;
    time64_t last_read_error;
    atomic_t corrected_errors;
    struct list_head wb_list;
    spinlock_t wb_list_lock;
    wait_queue_head_t wb_io_wait;
    struct work_struct del_work;
    struct kernfs_node *sysfs_state;
    struct badblocks badblocks;
    struct (anon) ppl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct md_rdev {
    struct list_head same_set;
    sector_t sectors;
    struct mddev *mddev;
    int last_events;
    struct block_device *meta_bdev;
    struct block_device *bdev;
    struct page *sb_page;
    struct page *bb_page;
    int sb_loaded;
    __u64 sb_events;
    sector_t data_offset;
    sector_t new_data_offset;
    sector_t sb_start;
    int sb_size;
    int preferred_minor;
    struct kobject kobj;
    long unsigned int flags;
    wait_queue_head_t blocked_wait;
    int desc_nr;
    int raid_disk;
    int new_raid_disk;
    int saved_raid_disk;
    sector_t recovery_offset;
    sector_t journal_tail;
    atomic_t nr_pending;
    atomic_t read_errors;
    time64_t last_read_error;
    atomic_t corrected_errors;
    struct list_head wb_list;
    spinlock_t wb_list_lock;
    wait_queue_head_t wb_io_wait;
    struct work_struct del_work;
    struct kernfs_node *sysfs_state;
    struct badblocks badblocks;
    struct (anon) ppl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct md_rdev {
    struct list_head same_set;
    sector_t sectors;
    struct mddev *mddev;
    int last_events;
    struct block_device *meta_bdev;
    struct block_device *bdev;
    struct page *sb_page;
    struct page *bb_page;
    int sb_loaded;
    __u64 sb_events;
    sector_t data_offset;
    sector_t new_data_offset;
    sector_t sb_start;
    int sb_size;
    int preferred_minor;
    struct kobject kobj;
    long unsigned int flags;
    wait_queue_head_t blocked_wait;
    int desc_nr;
    int raid_disk;
    int new_raid_disk;
    int saved_raid_disk;
    sector_t recovery_offset;
    sector_t journal_tail;
    atomic_t nr_pending;
    atomic_t read_errors;
    time64_t last_read_error;
    atomic_t corrected_errors;
    struct serial_in_rdev *serial;
    struct work_struct del_work;
    struct kernfs_node *sysfs_state;
    struct badblocks badblocks;
    struct (anon) ppl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct md_rdev {
    struct list_head same_set;
    sector_t sectors;
    struct mddev *mddev;
    int last_events;
    struct block_device *meta_bdev;
    struct block_device *bdev;
    struct page *sb_page;
    struct page *bb_page;
    int sb_loaded;
    __u64 sb_events;
    sector_t data_offset;
    sector_t new_data_offset;
    sector_t sb_start;
    int sb_size;
    int preferred_minor;
    struct kobject kobj;
    long unsigned int flags;
    wait_queue_head_t blocked_wait;
    int desc_nr;
    int raid_disk;
    int new_raid_disk;
    int saved_raid_disk;
    sector_t recovery_offset;
    sector_t journal_tail;
    atomic_t nr_pending;
    atomic_t read_errors;
    time64_t last_read_error;
    atomic_t corrected_errors;
    struct serial_in_rdev *serial;
    struct work_struct del_work;
    struct kernfs_node *sysfs_state;
    struct kernfs_node *sysfs_unack_badblocks;
    struct kernfs_node *sysfs_badblocks;
    struct badblocks badblocks;
    struct (anon) ppl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct md_rdev {
    struct list_head same_set;
    sector_t sectors;
    struct mddev *mddev;
    int last_events;
    struct block_device *meta_bdev;
    struct block_device *bdev;
    struct page *sb_page;
    struct page *bb_page;
    int sb_loaded;
    __u64 sb_events;
    sector_t data_offset;
    sector_t new_data_offset;
    sector_t sb_start;
    int sb_size;
    int preferred_minor;
    struct kobject kobj;
    long unsigned int flags;
    wait_queue_head_t blocked_wait;
    int desc_nr;
    int raid_disk;
    int new_raid_disk;
    int saved_raid_disk;
    sector_t recovery_offset;
    sector_t journal_tail;
    atomic_t nr_pending;
    atomic_t read_errors;
    time64_t last_read_error;
    atomic_t corrected_errors;
    struct serial_in_rdev *serial;
    struct work_struct del_work;
    struct kernfs_node *sysfs_state;
    struct kernfs_node *sysfs_unack_badblocks;
    struct kernfs_node *sysfs_badblocks;
    struct badblocks badblocks;
    struct (anon) ppl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct md_rdev {
    struct list_head same_set;
    sector_t sectors;
    struct mddev *mddev;
    int last_events;
    struct block_device *meta_bdev;
    struct block_device *bdev;
    struct page *sb_page;
    struct page *bb_page;
    int sb_loaded;
    __u64 sb_events;
    sector_t data_offset;
    sector_t new_data_offset;
    sector_t sb_start;
    int sb_size;
    int preferred_minor;
    struct kobject kobj;
    long unsigned int flags;
    wait_queue_head_t blocked_wait;
    int desc_nr;
    int raid_disk;
    int new_raid_disk;
    int saved_raid_disk;
    sector_t recovery_offset;
    sector_t journal_tail;
    atomic_t nr_pending;
    atomic_t read_errors;
    time64_t last_read_error;
    atomic_t corrected_errors;
    struct serial_in_rdev *serial;
    struct work_struct del_work;
    struct kernfs_node *sysfs_state;
    struct kernfs_node *sysfs_unack_badblocks;
    struct kernfs_node *sysfs_badblocks;
    struct badblocks badblocks;
    struct (anon) ppl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct md_rdev {
    struct list_head same_set;
    sector_t sectors;
    struct mddev *mddev;
    int last_events;
    struct block_device *meta_bdev;
    struct block_device *bdev;
    struct page *sb_page;
    struct page *bb_page;
    int sb_loaded;
    __u64 sb_events;
    sector_t data_offset;
    sector_t new_data_offset;
    sector_t sb_start;
    int sb_size;
    int preferred_minor;
    struct kobject kobj;
    long unsigned int flags;
    wait_queue_head_t blocked_wait;
    int desc_nr;
    int raid_disk;
    int new_raid_disk;
    int saved_raid_disk;
    sector_t recovery_offset;
    sector_t journal_tail;
    atomic_t nr_pending;
    atomic_t read_errors;
    time64_t last_read_error;
    atomic_t corrected_errors;
    struct serial_in_rdev *serial;
    struct work_struct del_work;
    struct kernfs_node *sysfs_state;
    struct kernfs_node *sysfs_unack_badblocks;
    struct kernfs_node *sysfs_badblocks;
    struct badblocks badblocks;
    struct (anon) ppl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct md_rdev {
    struct list_head same_set;
    sector_t sectors;
    struct mddev *mddev;
    int last_events;
    struct block_device *meta_bdev;
    struct block_device *bdev;
    struct page *sb_page;
    struct page *bb_page;
    int sb_loaded;
    __u64 sb_events;
    sector_t data_offset;
    sector_t new_data_offset;
    sector_t sb_start;
    int sb_size;
    int preferred_minor;
    struct kobject kobj;
    long unsigned int flags;
    wait_queue_head_t blocked_wait;
    int desc_nr;
    int raid_disk;
    int new_raid_disk;
    int saved_raid_disk;
    sector_t recovery_offset;
    sector_t journal_tail;
    atomic_t nr_pending;
    atomic_t read_errors;
    time64_t last_read_error;
    atomic_t corrected_errors;
    struct serial_in_rdev *serial;
    struct work_struct del_work;
    struct kernfs_node *sysfs_state;
    struct kernfs_node *sysfs_unack_badblocks;
    struct kernfs_node *sysfs_badblocks;
    struct badblocks badblocks;
    struct (anon) ppl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct md_rdev {
    struct list_head same_set;
    sector_t sectors;
    struct mddev *mddev;
    int last_events;
    struct block_device *meta_bdev;
    struct block_device *bdev;
    struct page *sb_page;
    struct page *bb_page;
    int sb_loaded;
    __u64 sb_events;
    sector_t data_offset;
    sector_t new_data_offset;
    sector_t sb_start;
    int sb_size;
    int preferred_minor;
    struct kobject kobj;
    long unsigned int flags;
    wait_queue_head_t blocked_wait;
    int desc_nr;
    int raid_disk;
    int new_raid_disk;
    int saved_raid_disk;
    sector_t recovery_offset;
    sector_t journal_tail;
    atomic_t nr_pending;
    atomic_t read_errors;
    time64_t last_read_error;
    atomic_t corrected_errors;
    struct serial_in_rdev *serial;
    struct kernfs_node *sysfs_state;
    struct kernfs_node *sysfs_unack_badblocks;
    struct kernfs_node *sysfs_badblocks;
    struct badblocks badblocks;
    struct (anon) ppl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct md_rdev {
    struct list_head same_set;
    sector_t sectors;
    struct mddev *mddev;
    int last_events;
    struct block_device *meta_bdev;
    struct block_device *bdev;
    struct bdev_handle *bdev_handle;
    struct page *sb_page;
    struct page *bb_page;
    int sb_loaded;
    __u64 sb_events;
    sector_t data_offset;
    sector_t new_data_offset;
    sector_t sb_start;
    int sb_size;
    int preferred_minor;
    struct kobject kobj;
    long unsigned int flags;
    wait_queue_head_t blocked_wait;
    int desc_nr;
    int raid_disk;
    int new_raid_disk;
    int saved_raid_disk;
    sector_t recovery_offset;
    sector_t journal_tail;
    atomic_t nr_pending;
    atomic_t read_errors;
    time64_t last_read_error;
    atomic_t corrected_errors;
    struct serial_in_rdev *serial;
    struct kernfs_node *sysfs_state;
    struct kernfs_node *sysfs_unack_badblocks;
    struct kernfs_node *sysfs_badblocks;
    struct badblocks badblocks;
    struct (anon) ppl;
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
struct md_rdev {
    struct list_head same_set;
    sector_t sectors;
    struct mddev *mddev;
    int last_events;
    struct block_device *meta_bdev;
    struct block_device *bdev;
    struct page *sb_page;
    struct page *bb_page;
    int sb_loaded;
    __u64 sb_events;
    sector_t data_offset;
    sector_t new_data_offset;
    sector_t sb_start;
    int sb_size;
    int preferred_minor;
    struct kobject kobj;
    long unsigned int flags;
    wait_queue_head_t blocked_wait;
    int desc_nr;
    int raid_disk;
    int new_raid_disk;
    int saved_raid_disk;
    sector_t recovery_offset;
    sector_t journal_tail;
    atomic_t nr_pending;
    atomic_t read_errors;
    time64_t last_read_error;
    atomic_t corrected_errors;
    struct list_head wb_list;
    spinlock_t wb_list_lock;
    wait_queue_head_t wb_io_wait;
    struct work_struct del_work;
    struct kernfs_node *sysfs_state;
    struct badblocks badblocks;
    struct (anon) ppl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct md_rdev {
    struct list_head same_set;
    sector_t sectors;
    struct mddev *mddev;
    int last_events;
    struct block_device *meta_bdev;
    struct block_device *bdev;
    struct page *sb_page;
    struct page *bb_page;
    int sb_loaded;
    __u64 sb_events;
    sector_t data_offset;
    sector_t new_data_offset;
    sector_t sb_start;
    int sb_size;
    int preferred_minor;
    struct kobject kobj;
    long unsigned int flags;
    wait_queue_head_t blocked_wait;
    int desc_nr;
    int raid_disk;
    int new_raid_disk;
    int saved_raid_disk;
    sector_t recovery_offset;
    sector_t journal_tail;
    atomic_t nr_pending;
    atomic_t read_errors;
    time64_t last_read_error;
    atomic_t corrected_errors;
    struct list_head wb_list;
    spinlock_t wb_list_lock;
    wait_queue_head_t wb_io_wait;
    struct work_struct del_work;
    struct kernfs_node *sysfs_state;
    struct badblocks badblocks;
    struct (anon) ppl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct md_rdev {
    struct list_head same_set;
    sector_t sectors;
    struct mddev *mddev;
    int last_events;
    struct block_device *meta_bdev;
    struct block_device *bdev;
    struct page *sb_page;
    struct page *bb_page;
    int sb_loaded;
    __u64 sb_events;
    sector_t data_offset;
    sector_t new_data_offset;
    sector_t sb_start;
    int sb_size;
    int preferred_minor;
    struct kobject kobj;
    long unsigned int flags;
    wait_queue_head_t blocked_wait;
    int desc_nr;
    int raid_disk;
    int new_raid_disk;
    int saved_raid_disk;
    sector_t recovery_offset;
    sector_t journal_tail;
    atomic_t nr_pending;
    atomic_t read_errors;
    time64_t last_read_error;
    atomic_t corrected_errors;
    struct list_head wb_list;
    spinlock_t wb_list_lock;
    wait_queue_head_t wb_io_wait;
    struct work_struct del_work;
    struct kernfs_node *sysfs_state;
    struct badblocks badblocks;
    struct (anon) ppl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct md_rdev {
    struct list_head same_set;
    sector_t sectors;
    struct mddev *mddev;
    int last_events;
    struct block_device *meta_bdev;
    struct block_device *bdev;
    struct page *sb_page;
    struct page *bb_page;
    int sb_loaded;
    __u64 sb_events;
    sector_t data_offset;
    sector_t new_data_offset;
    sector_t sb_start;
    int sb_size;
    int preferred_minor;
    struct kobject kobj;
    long unsigned int flags;
    wait_queue_head_t blocked_wait;
    int desc_nr;
    int raid_disk;
    int new_raid_disk;
    int saved_raid_disk;
    sector_t recovery_offset;
    sector_t journal_tail;
    atomic_t nr_pending;
    atomic_t read_errors;
    time64_t last_read_error;
    atomic_t corrected_errors;
    struct list_head wb_list;
    spinlock_t wb_list_lock;
    wait_queue_head_t wb_io_wait;
    struct work_struct del_work;
    struct kernfs_node *sysfs_state;
    struct badblocks badblocks;
    struct (anon) ppl;
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
struct md_rdev {
    struct list_head same_set;
    sector_t sectors;
    struct mddev *mddev;
    int last_events;
    struct block_device *meta_bdev;
    struct block_device *bdev;
    struct page *sb_page;
    struct page *bb_page;
    int sb_loaded;
    __u64 sb_events;
    sector_t data_offset;
    sector_t new_data_offset;
    sector_t sb_start;
    int sb_size;
    int preferred_minor;
    struct kobject kobj;
    long unsigned int flags;
    wait_queue_head_t blocked_wait;
    int desc_nr;
    int raid_disk;
    int new_raid_disk;
    int saved_raid_disk;
    sector_t recovery_offset;
    sector_t journal_tail;
    atomic_t nr_pending;
    atomic_t read_errors;
    time64_t last_read_error;
    atomic_t corrected_errors;
    struct list_head wb_list;
    spinlock_t wb_list_lock;
    wait_queue_head_t wb_io_wait;
    struct work_struct del_work;
    struct kernfs_node *sysfs_state;
    struct badblocks badblocks;
    struct (anon) ppl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct md_rdev {
    struct list_head same_set;
    sector_t sectors;
    struct mddev *mddev;
    int last_events;
    struct block_device *meta_bdev;
    struct block_device *bdev;
    struct page *sb_page;
    struct page *bb_page;
    int sb_loaded;
    __u64 sb_events;
    sector_t data_offset;
    sector_t new_data_offset;
    sector_t sb_start;
    int sb_size;
    int preferred_minor;
    struct kobject kobj;
    long unsigned int flags;
    wait_queue_head_t blocked_wait;
    int desc_nr;
    int raid_disk;
    int new_raid_disk;
    int saved_raid_disk;
    sector_t recovery_offset;
    sector_t journal_tail;
    atomic_t nr_pending;
    atomic_t read_errors;
    time64_t last_read_error;
    atomic_t corrected_errors;
    struct list_head wb_list;
    spinlock_t wb_list_lock;
    wait_queue_head_t wb_io_wait;
    struct work_struct del_work;
    struct kernfs_node *sysfs_state;
    struct badblocks badblocks;
    struct (anon) ppl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct md_rdev {
    struct list_head same_set;
    sector_t sectors;
    struct mddev *mddev;
    int last_events;
    struct block_device *meta_bdev;
    struct block_device *bdev;
    struct page *sb_page;
    struct page *bb_page;
    int sb_loaded;
    __u64 sb_events;
    sector_t data_offset;
    sector_t new_data_offset;
    sector_t sb_start;
    int sb_size;
    int preferred_minor;
    struct kobject kobj;
    long unsigned int flags;
    wait_queue_head_t blocked_wait;
    int desc_nr;
    int raid_disk;
    int new_raid_disk;
    int saved_raid_disk;
    sector_t recovery_offset;
    sector_t journal_tail;
    atomic_t nr_pending;
    atomic_t read_errors;
    time64_t last_read_error;
    atomic_t corrected_errors;
    struct list_head wb_list;
    spinlock_t wb_list_lock;
    wait_queue_head_t wb_io_wait;
    struct work_struct del_work;
    struct kernfs_node *sysfs_state;
    struct badblocks badblocks;
    struct (anon) ppl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct md_rdev {
    struct list_head same_set;
    sector_t sectors;
    struct mddev *mddev;
    int last_events;
    struct block_device *meta_bdev;
    struct block_device *bdev;
    struct page *sb_page;
    struct page *bb_page;
    int sb_loaded;
    __u64 sb_events;
    sector_t data_offset;
    sector_t new_data_offset;
    sector_t sb_start;
    int sb_size;
    int preferred_minor;
    struct kobject kobj;
    long unsigned int flags;
    wait_queue_head_t blocked_wait;
    int desc_nr;
    int raid_disk;
    int new_raid_disk;
    int saved_raid_disk;
    sector_t recovery_offset;
    sector_t journal_tail;
    atomic_t nr_pending;
    atomic_t read_errors;
    time64_t last_read_error;
    atomic_t corrected_errors;
    struct list_head wb_list;
    spinlock_t wb_list_lock;
    wait_queue_head_t wb_io_wait;
    struct work_struct del_work;
    struct kernfs_node *sysfs_state;
    struct badblocks badblocks;
    struct (anon) ppl;
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
<b>Field type changed. </b>
<code>struct timespec last_read_error</code> ➡️ <code>time64_t last_read_error</code>
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
<code>struct (anon) ppl</code>
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
<code>struct list_head wb_list</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t wb_list_lock</code>
</li>
<li>
<b>Field added. </b>
<code>wait_queue_head_t wb_io_wait</code>
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
<code>struct serial_in_rdev *serial</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head wb_list</code>
</li>
<li>
<b>Field removed. </b>
<code>spinlock_t wb_list_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>wait_queue_head_t wb_io_wait</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct kernfs_node *sysfs_unack_badblocks</code>
</li>
<li>
<b>Field added. </b>
<code>struct kernfs_node *sysfs_badblocks</code>
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
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct work_struct del_work</code>
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
<code>struct bdev_handle *bdev_handle</code>
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
