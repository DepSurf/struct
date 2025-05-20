# Struct: <code>scsi_host_template</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct scsi_host_template {
    struct module *module;
    const char *name;
    int (*detect)(struct scsi_host_template *);
    int (*release)(struct Scsi_Host *);
    const char * (*info)(struct Scsi_Host *);
    int (*ioctl)(struct scsi_device *, int, void *);
    int (*compat_ioctl)(struct scsi_device *, int, void *);
    int (*queuecommand)(struct Scsi_Host *, struct scsi_cmnd *);
    int (*eh_abort_handler)(struct scsi_cmnd *);
    int (*eh_device_reset_handler)(struct scsi_cmnd *);
    int (*eh_target_reset_handler)(struct scsi_cmnd *);
    int (*eh_bus_reset_handler)(struct scsi_cmnd *);
    int (*eh_host_reset_handler)(struct scsi_cmnd *);
    int (*slave_alloc)(struct scsi_device *);
    int (*slave_configure)(struct scsi_device *);
    void (*slave_destroy)(struct scsi_device *);
    int (*target_alloc)(struct scsi_target *);
    void (*target_destroy)(struct scsi_target *);
    int (*scan_finished)(struct Scsi_Host *, long unsigned int);
    void (*scan_start)(struct Scsi_Host *);
    int (*change_queue_depth)(struct scsi_device *, int);
    int (*bios_param)(struct scsi_device *, struct block_device *, sector_t, int *);
    void (*unlock_native_capacity)(struct scsi_device *);
    int (*show_info)(struct seq_file *, struct Scsi_Host *);
    int (*write_info)(struct Scsi_Host *, char *, int);
    enum blk_eh_timer_return (*eh_timed_out)(struct scsi_cmnd *);
    int (*host_reset)(struct Scsi_Host *, int);
    const char *proc_name;
    struct proc_dir_entry *proc_dir;
    int can_queue;
    int this_id;
    short unsigned int sg_tablesize;
    short unsigned int sg_prot_tablesize;
    unsigned int max_sectors;
    long unsigned int dma_boundary;
    short int cmd_per_lun;
    unsigned char present;
    int tag_alloc_policy;
    unsigned int track_queue_depth;
    unsigned int supported_mode;
    unsigned int unchecked_isa_dma;
    unsigned int use_clustering;
    unsigned int emulated;
    unsigned int skip_settle_delay;
    unsigned int no_write_same;
    unsigned int no_async_abort;
    unsigned int max_host_blocked;
    struct device_attribute **shost_attrs;
    struct device_attribute **sdev_attrs;
    struct list_head legacy_hosts;
    u64 vendor_id;
    unsigned int cmd_size;
    struct scsi_host_cmd_pool *cmd_pool;
    bool disable_blk_mq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct scsi_host_template {
    struct module *module;
    const char *name;
    int (*detect)(struct scsi_host_template *);
    int (*release)(struct Scsi_Host *);
    const char * (*info)(struct Scsi_Host *);
    int (*ioctl)(struct scsi_device *, int, void *);
    int (*compat_ioctl)(struct scsi_device *, int, void *);
    int (*queuecommand)(struct Scsi_Host *, struct scsi_cmnd *);
    int (*eh_abort_handler)(struct scsi_cmnd *);
    int (*eh_device_reset_handler)(struct scsi_cmnd *);
    int (*eh_target_reset_handler)(struct scsi_cmnd *);
    int (*eh_bus_reset_handler)(struct scsi_cmnd *);
    int (*eh_host_reset_handler)(struct scsi_cmnd *);
    int (*slave_alloc)(struct scsi_device *);
    int (*slave_configure)(struct scsi_device *);
    void (*slave_destroy)(struct scsi_device *);
    int (*target_alloc)(struct scsi_target *);
    void (*target_destroy)(struct scsi_target *);
    int (*scan_finished)(struct Scsi_Host *, long unsigned int);
    void (*scan_start)(struct Scsi_Host *);
    int (*change_queue_depth)(struct scsi_device *, int);
    int (*bios_param)(struct scsi_device *, struct block_device *, sector_t, int *);
    void (*unlock_native_capacity)(struct scsi_device *);
    int (*show_info)(struct seq_file *, struct Scsi_Host *);
    int (*write_info)(struct Scsi_Host *, char *, int);
    enum blk_eh_timer_return (*eh_timed_out)(struct scsi_cmnd *);
    int (*host_reset)(struct Scsi_Host *, int);
    const char *proc_name;
    struct proc_dir_entry *proc_dir;
    int can_queue;
    int this_id;
    short unsigned int sg_tablesize;
    short unsigned int sg_prot_tablesize;
    unsigned int max_sectors;
    long unsigned int dma_boundary;
    short int cmd_per_lun;
    unsigned char present;
    int tag_alloc_policy;
    unsigned int track_queue_depth;
    unsigned int supported_mode;
    unsigned int unchecked_isa_dma;
    unsigned int use_clustering;
    unsigned int emulated;
    unsigned int skip_settle_delay;
    unsigned int no_write_same;
    unsigned int no_async_abort;
    unsigned int max_host_blocked;
    struct device_attribute **shost_attrs;
    struct device_attribute **sdev_attrs;
    struct list_head legacy_hosts;
    u64 vendor_id;
    unsigned int cmd_size;
    struct scsi_host_cmd_pool *cmd_pool;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct scsi_host_template {
    struct module *module;
    const char *name;
    int (*detect)(struct scsi_host_template *);
    int (*release)(struct Scsi_Host *);
    const char * (*info)(struct Scsi_Host *);
    int (*ioctl)(struct scsi_device *, int, void *);
    int (*compat_ioctl)(struct scsi_device *, int, void *);
    int (*queuecommand)(struct Scsi_Host *, struct scsi_cmnd *);
    int (*eh_abort_handler)(struct scsi_cmnd *);
    int (*eh_device_reset_handler)(struct scsi_cmnd *);
    int (*eh_target_reset_handler)(struct scsi_cmnd *);
    int (*eh_bus_reset_handler)(struct scsi_cmnd *);
    int (*eh_host_reset_handler)(struct scsi_cmnd *);
    int (*slave_alloc)(struct scsi_device *);
    int (*slave_configure)(struct scsi_device *);
    void (*slave_destroy)(struct scsi_device *);
    int (*target_alloc)(struct scsi_target *);
    void (*target_destroy)(struct scsi_target *);
    int (*scan_finished)(struct Scsi_Host *, long unsigned int);
    void (*scan_start)(struct Scsi_Host *);
    int (*change_queue_depth)(struct scsi_device *, int);
    int (*map_queues)(struct Scsi_Host *);
    int (*bios_param)(struct scsi_device *, struct block_device *, sector_t, int *);
    void (*unlock_native_capacity)(struct scsi_device *);
    int (*show_info)(struct seq_file *, struct Scsi_Host *);
    int (*write_info)(struct Scsi_Host *, char *, int);
    enum blk_eh_timer_return (*eh_timed_out)(struct scsi_cmnd *);
    int (*host_reset)(struct Scsi_Host *, int);
    const char *proc_name;
    struct proc_dir_entry *proc_dir;
    int can_queue;
    int this_id;
    short unsigned int sg_tablesize;
    short unsigned int sg_prot_tablesize;
    unsigned int max_sectors;
    long unsigned int dma_boundary;
    short int cmd_per_lun;
    unsigned char present;
    int tag_alloc_policy;
    unsigned int track_queue_depth;
    unsigned int supported_mode;
    unsigned int unchecked_isa_dma;
    unsigned int use_clustering;
    unsigned int emulated;
    unsigned int skip_settle_delay;
    unsigned int no_write_same;
    unsigned int no_async_abort;
    unsigned int max_host_blocked;
    struct device_attribute **shost_attrs;
    struct device_attribute **sdev_attrs;
    struct list_head legacy_hosts;
    u64 vendor_id;
    unsigned int cmd_size;
    struct scsi_host_cmd_pool *cmd_pool;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct scsi_host_template {
    struct module *module;
    const char *name;
    int (*detect)(struct scsi_host_template *);
    int (*release)(struct Scsi_Host *);
    const char * (*info)(struct Scsi_Host *);
    int (*ioctl)(struct scsi_device *, int, void *);
    int (*compat_ioctl)(struct scsi_device *, int, void *);
    int (*queuecommand)(struct Scsi_Host *, struct scsi_cmnd *);
    int (*eh_abort_handler)(struct scsi_cmnd *);
    int (*eh_device_reset_handler)(struct scsi_cmnd *);
    int (*eh_target_reset_handler)(struct scsi_cmnd *);
    int (*eh_bus_reset_handler)(struct scsi_cmnd *);
    int (*eh_host_reset_handler)(struct scsi_cmnd *);
    int (*slave_alloc)(struct scsi_device *);
    int (*slave_configure)(struct scsi_device *);
    void (*slave_destroy)(struct scsi_device *);
    int (*target_alloc)(struct scsi_target *);
    void (*target_destroy)(struct scsi_target *);
    int (*scan_finished)(struct Scsi_Host *, long unsigned int);
    void (*scan_start)(struct Scsi_Host *);
    int (*change_queue_depth)(struct scsi_device *, int);
    int (*map_queues)(struct Scsi_Host *);
    int (*bios_param)(struct scsi_device *, struct block_device *, sector_t, int *);
    void (*unlock_native_capacity)(struct scsi_device *);
    int (*show_info)(struct seq_file *, struct Scsi_Host *);
    int (*write_info)(struct Scsi_Host *, char *, int);
    enum blk_eh_timer_return (*eh_timed_out)(struct scsi_cmnd *);
    int (*host_reset)(struct Scsi_Host *, int);
    const char *proc_name;
    struct proc_dir_entry *proc_dir;
    int can_queue;
    int this_id;
    short unsigned int sg_tablesize;
    short unsigned int sg_prot_tablesize;
    unsigned int max_sectors;
    long unsigned int dma_boundary;
    short int cmd_per_lun;
    unsigned char present;
    int tag_alloc_policy;
    unsigned int track_queue_depth;
    unsigned int supported_mode;
    unsigned int unchecked_isa_dma;
    unsigned int use_clustering;
    unsigned int emulated;
    unsigned int skip_settle_delay;
    unsigned int no_write_same;
    unsigned int max_host_blocked;
    struct device_attribute **shost_attrs;
    struct device_attribute **sdev_attrs;
    struct list_head legacy_hosts;
    u64 vendor_id;
    unsigned int cmd_size;
    struct scsi_host_cmd_pool *cmd_pool;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct scsi_host_template {
    struct module *module;
    const char *name;
    int (*detect)(struct scsi_host_template *);
    int (*release)(struct Scsi_Host *);
    const char * (*info)(struct Scsi_Host *);
    int (*ioctl)(struct scsi_device *, int, void *);
    int (*compat_ioctl)(struct scsi_device *, int, void *);
    int (*queuecommand)(struct Scsi_Host *, struct scsi_cmnd *);
    int (*eh_abort_handler)(struct scsi_cmnd *);
    int (*eh_device_reset_handler)(struct scsi_cmnd *);
    int (*eh_target_reset_handler)(struct scsi_cmnd *);
    int (*eh_bus_reset_handler)(struct scsi_cmnd *);
    int (*eh_host_reset_handler)(struct scsi_cmnd *);
    int (*slave_alloc)(struct scsi_device *);
    int (*slave_configure)(struct scsi_device *);
    void (*slave_destroy)(struct scsi_device *);
    int (*target_alloc)(struct scsi_target *);
    void (*target_destroy)(struct scsi_target *);
    int (*scan_finished)(struct Scsi_Host *, long unsigned int);
    void (*scan_start)(struct Scsi_Host *);
    int (*change_queue_depth)(struct scsi_device *, int);
    int (*map_queues)(struct Scsi_Host *);
    int (*bios_param)(struct scsi_device *, struct block_device *, sector_t, int *);
    void (*unlock_native_capacity)(struct scsi_device *);
    int (*show_info)(struct seq_file *, struct Scsi_Host *);
    int (*write_info)(struct Scsi_Host *, char *, int);
    enum blk_eh_timer_return (*eh_timed_out)(struct scsi_cmnd *);
    int (*host_reset)(struct Scsi_Host *, int);
    const char *proc_name;
    struct proc_dir_entry *proc_dir;
    int can_queue;
    int this_id;
    short unsigned int sg_tablesize;
    short unsigned int sg_prot_tablesize;
    unsigned int max_sectors;
    long unsigned int dma_boundary;
    short int cmd_per_lun;
    unsigned char present;
    int tag_alloc_policy;
    unsigned int track_queue_depth;
    unsigned int supported_mode;
    unsigned int unchecked_isa_dma;
    unsigned int use_clustering;
    unsigned int emulated;
    unsigned int skip_settle_delay;
    unsigned int no_write_same;
    unsigned int max_host_blocked;
    struct device_attribute **shost_attrs;
    struct device_attribute **sdev_attrs;
    struct list_head legacy_hosts;
    u64 vendor_id;
    unsigned int cmd_size;
    struct scsi_host_cmd_pool *cmd_pool;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct scsi_host_template {
    struct module *module;
    const char *name;
    const char * (*info)(struct Scsi_Host *);
    int (*ioctl)(struct scsi_device *, int, void *);
    int (*compat_ioctl)(struct scsi_device *, int, void *);
    int (*queuecommand)(struct Scsi_Host *, struct scsi_cmnd *);
    int (*eh_abort_handler)(struct scsi_cmnd *);
    int (*eh_device_reset_handler)(struct scsi_cmnd *);
    int (*eh_target_reset_handler)(struct scsi_cmnd *);
    int (*eh_bus_reset_handler)(struct scsi_cmnd *);
    int (*eh_host_reset_handler)(struct scsi_cmnd *);
    int (*slave_alloc)(struct scsi_device *);
    int (*slave_configure)(struct scsi_device *);
    void (*slave_destroy)(struct scsi_device *);
    int (*target_alloc)(struct scsi_target *);
    void (*target_destroy)(struct scsi_target *);
    int (*scan_finished)(struct Scsi_Host *, long unsigned int);
    void (*scan_start)(struct Scsi_Host *);
    int (*change_queue_depth)(struct scsi_device *, int);
    int (*map_queues)(struct Scsi_Host *);
    int (*bios_param)(struct scsi_device *, struct block_device *, sector_t, int *);
    void (*unlock_native_capacity)(struct scsi_device *);
    int (*show_info)(struct seq_file *, struct Scsi_Host *);
    int (*write_info)(struct Scsi_Host *, char *, int);
    enum blk_eh_timer_return (*eh_timed_out)(struct scsi_cmnd *);
    int (*host_reset)(struct Scsi_Host *, int);
    const char *proc_name;
    struct proc_dir_entry *proc_dir;
    int can_queue;
    int this_id;
    short unsigned int sg_tablesize;
    short unsigned int sg_prot_tablesize;
    unsigned int max_sectors;
    long unsigned int dma_boundary;
    short int cmd_per_lun;
    unsigned char present;
    int tag_alloc_policy;
    unsigned int track_queue_depth;
    unsigned int supported_mode;
    unsigned int unchecked_isa_dma;
    unsigned int use_clustering;
    unsigned int emulated;
    unsigned int skip_settle_delay;
    unsigned int no_write_same;
    unsigned int force_blk_mq;
    unsigned int max_host_blocked;
    struct device_attribute **shost_attrs;
    struct device_attribute **sdev_attrs;
    const struct attribute_group **sdev_groups;
    u64 vendor_id;
    unsigned int cmd_size;
    struct scsi_host_cmd_pool *cmd_pool;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct scsi_host_template {
    struct module *module;
    const char *name;
    const char * (*info)(struct Scsi_Host *);
    int (*ioctl)(struct scsi_device *, int, void *);
    int (*compat_ioctl)(struct scsi_device *, int, void *);
    int (*queuecommand)(struct Scsi_Host *, struct scsi_cmnd *);
    int (*eh_abort_handler)(struct scsi_cmnd *);
    int (*eh_device_reset_handler)(struct scsi_cmnd *);
    int (*eh_target_reset_handler)(struct scsi_cmnd *);
    int (*eh_bus_reset_handler)(struct scsi_cmnd *);
    int (*eh_host_reset_handler)(struct scsi_cmnd *);
    int (*slave_alloc)(struct scsi_device *);
    int (*slave_configure)(struct scsi_device *);
    void (*slave_destroy)(struct scsi_device *);
    int (*target_alloc)(struct scsi_target *);
    void (*target_destroy)(struct scsi_target *);
    int (*scan_finished)(struct Scsi_Host *, long unsigned int);
    void (*scan_start)(struct Scsi_Host *);
    int (*change_queue_depth)(struct scsi_device *, int);
    int (*map_queues)(struct Scsi_Host *);
    int (*bios_param)(struct scsi_device *, struct block_device *, sector_t, int *);
    void (*unlock_native_capacity)(struct scsi_device *);
    int (*show_info)(struct seq_file *, struct Scsi_Host *);
    int (*write_info)(struct Scsi_Host *, char *, int);
    enum blk_eh_timer_return (*eh_timed_out)(struct scsi_cmnd *);
    int (*host_reset)(struct Scsi_Host *, int);
    const char *proc_name;
    struct proc_dir_entry *proc_dir;
    int can_queue;
    int this_id;
    short unsigned int sg_tablesize;
    short unsigned int sg_prot_tablesize;
    unsigned int max_sectors;
    unsigned int max_segment_size;
    long unsigned int dma_boundary;
    short int cmd_per_lun;
    unsigned char present;
    int tag_alloc_policy;
    unsigned int track_queue_depth;
    unsigned int supported_mode;
    unsigned int unchecked_isa_dma;
    unsigned int emulated;
    unsigned int skip_settle_delay;
    unsigned int no_write_same;
    unsigned int force_blk_mq;
    unsigned int max_host_blocked;
    struct device_attribute **shost_attrs;
    struct device_attribute **sdev_attrs;
    const struct attribute_group **sdev_groups;
    u64 vendor_id;
    unsigned int cmd_size;
    struct scsi_host_cmd_pool *cmd_pool;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct scsi_host_template {
    struct module *module;
    const char *name;
    const char * (*info)(struct Scsi_Host *);
    int (*ioctl)(struct scsi_device *, unsigned int, void *);
    int (*compat_ioctl)(struct scsi_device *, unsigned int, void *);
    int (*queuecommand)(struct Scsi_Host *, struct scsi_cmnd *);
    int (*eh_abort_handler)(struct scsi_cmnd *);
    int (*eh_device_reset_handler)(struct scsi_cmnd *);
    int (*eh_target_reset_handler)(struct scsi_cmnd *);
    int (*eh_bus_reset_handler)(struct scsi_cmnd *);
    int (*eh_host_reset_handler)(struct scsi_cmnd *);
    int (*slave_alloc)(struct scsi_device *);
    int (*slave_configure)(struct scsi_device *);
    void (*slave_destroy)(struct scsi_device *);
    int (*target_alloc)(struct scsi_target *);
    void (*target_destroy)(struct scsi_target *);
    int (*scan_finished)(struct Scsi_Host *, long unsigned int);
    void (*scan_start)(struct Scsi_Host *);
    int (*change_queue_depth)(struct scsi_device *, int);
    int (*map_queues)(struct Scsi_Host *);
    int (*bios_param)(struct scsi_device *, struct block_device *, sector_t, int *);
    void (*unlock_native_capacity)(struct scsi_device *);
    int (*show_info)(struct seq_file *, struct Scsi_Host *);
    int (*write_info)(struct Scsi_Host *, char *, int);
    enum blk_eh_timer_return (*eh_timed_out)(struct scsi_cmnd *);
    int (*host_reset)(struct Scsi_Host *, int);
    const char *proc_name;
    struct proc_dir_entry *proc_dir;
    int can_queue;
    int this_id;
    short unsigned int sg_tablesize;
    short unsigned int sg_prot_tablesize;
    unsigned int max_sectors;
    unsigned int max_segment_size;
    long unsigned int dma_boundary;
    long unsigned int virt_boundary_mask;
    short int cmd_per_lun;
    unsigned char present;
    int tag_alloc_policy;
    unsigned int track_queue_depth;
    unsigned int supported_mode;
    unsigned int unchecked_isa_dma;
    unsigned int emulated;
    unsigned int skip_settle_delay;
    unsigned int no_write_same;
    unsigned int force_blk_mq;
    unsigned int max_host_blocked;
    struct device_attribute **shost_attrs;
    struct device_attribute **sdev_attrs;
    const struct attribute_group **sdev_groups;
    u64 vendor_id;
    unsigned int cmd_size;
    struct scsi_host_cmd_pool *cmd_pool;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct scsi_host_template {
    struct module *module;
    const char *name;
    const char * (*info)(struct Scsi_Host *);
    int (*ioctl)(struct scsi_device *, unsigned int, void *);
    int (*compat_ioctl)(struct scsi_device *, unsigned int, void *);
    int (*queuecommand)(struct Scsi_Host *, struct scsi_cmnd *);
    void (*commit_rqs)(struct Scsi_Host *, u16);
    int (*eh_abort_handler)(struct scsi_cmnd *);
    int (*eh_device_reset_handler)(struct scsi_cmnd *);
    int (*eh_target_reset_handler)(struct scsi_cmnd *);
    int (*eh_bus_reset_handler)(struct scsi_cmnd *);
    int (*eh_host_reset_handler)(struct scsi_cmnd *);
    int (*slave_alloc)(struct scsi_device *);
    int (*slave_configure)(struct scsi_device *);
    void (*slave_destroy)(struct scsi_device *);
    int (*target_alloc)(struct scsi_target *);
    void (*target_destroy)(struct scsi_target *);
    int (*scan_finished)(struct Scsi_Host *, long unsigned int);
    void (*scan_start)(struct Scsi_Host *);
    int (*change_queue_depth)(struct scsi_device *, int);
    int (*map_queues)(struct Scsi_Host *);
    int (*bios_param)(struct scsi_device *, struct block_device *, sector_t, int *);
    void (*unlock_native_capacity)(struct scsi_device *);
    int (*show_info)(struct seq_file *, struct Scsi_Host *);
    int (*write_info)(struct Scsi_Host *, char *, int);
    enum blk_eh_timer_return (*eh_timed_out)(struct scsi_cmnd *);
    int (*host_reset)(struct Scsi_Host *, int);
    const char *proc_name;
    struct proc_dir_entry *proc_dir;
    int can_queue;
    int this_id;
    short unsigned int sg_tablesize;
    short unsigned int sg_prot_tablesize;
    unsigned int max_sectors;
    unsigned int max_segment_size;
    long unsigned int dma_boundary;
    long unsigned int virt_boundary_mask;
    short int cmd_per_lun;
    unsigned char present;
    int tag_alloc_policy;
    unsigned int track_queue_depth;
    unsigned int supported_mode;
    unsigned int unchecked_isa_dma;
    unsigned int emulated;
    unsigned int skip_settle_delay;
    unsigned int no_write_same;
    unsigned int force_blk_mq;
    unsigned int max_host_blocked;
    struct device_attribute **shost_attrs;
    struct device_attribute **sdev_attrs;
    const struct attribute_group **sdev_groups;
    u64 vendor_id;
    unsigned int cmd_size;
    struct scsi_host_cmd_pool *cmd_pool;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct scsi_host_template {
    struct module *module;
    const char *name;
    const char * (*info)(struct Scsi_Host *);
    int (*ioctl)(struct scsi_device *, unsigned int, void *);
    int (*compat_ioctl)(struct scsi_device *, unsigned int, void *);
    int (*init_cmd_priv)(struct Scsi_Host *, struct scsi_cmnd *);
    int (*exit_cmd_priv)(struct Scsi_Host *, struct scsi_cmnd *);
    int (*queuecommand)(struct Scsi_Host *, struct scsi_cmnd *);
    void (*commit_rqs)(struct Scsi_Host *, u16);
    int (*eh_abort_handler)(struct scsi_cmnd *);
    int (*eh_device_reset_handler)(struct scsi_cmnd *);
    int (*eh_target_reset_handler)(struct scsi_cmnd *);
    int (*eh_bus_reset_handler)(struct scsi_cmnd *);
    int (*eh_host_reset_handler)(struct scsi_cmnd *);
    int (*slave_alloc)(struct scsi_device *);
    int (*slave_configure)(struct scsi_device *);
    void (*slave_destroy)(struct scsi_device *);
    int (*target_alloc)(struct scsi_target *);
    void (*target_destroy)(struct scsi_target *);
    int (*scan_finished)(struct Scsi_Host *, long unsigned int);
    void (*scan_start)(struct Scsi_Host *);
    int (*change_queue_depth)(struct scsi_device *, int);
    int (*map_queues)(struct Scsi_Host *);
    bool (*dma_need_drain)(struct request *);
    int (*bios_param)(struct scsi_device *, struct block_device *, sector_t, int *);
    void (*unlock_native_capacity)(struct scsi_device *);
    int (*show_info)(struct seq_file *, struct Scsi_Host *);
    int (*write_info)(struct Scsi_Host *, char *, int);
    enum blk_eh_timer_return (*eh_timed_out)(struct scsi_cmnd *);
    int (*host_reset)(struct Scsi_Host *, int);
    const char *proc_name;
    struct proc_dir_entry *proc_dir;
    int can_queue;
    int this_id;
    short unsigned int sg_tablesize;
    short unsigned int sg_prot_tablesize;
    unsigned int max_sectors;
    unsigned int max_segment_size;
    long unsigned int dma_boundary;
    long unsigned int virt_boundary_mask;
    short int cmd_per_lun;
    unsigned char present;
    int tag_alloc_policy;
    unsigned int track_queue_depth;
    unsigned int supported_mode;
    unsigned int unchecked_isa_dma;
    unsigned int emulated;
    unsigned int skip_settle_delay;
    unsigned int no_write_same;
    unsigned int max_host_blocked;
    struct device_attribute **shost_attrs;
    struct device_attribute **sdev_attrs;
    const struct attribute_group **sdev_groups;
    u64 vendor_id;
    unsigned int cmd_size;
    struct scsi_host_cmd_pool *cmd_pool;
    int rpm_autosuspend_delay;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct scsi_host_template {
    struct module *module;
    const char *name;
    const char * (*info)(struct Scsi_Host *);
    int (*ioctl)(struct scsi_device *, unsigned int, void *);
    int (*compat_ioctl)(struct scsi_device *, unsigned int, void *);
    int (*init_cmd_priv)(struct Scsi_Host *, struct scsi_cmnd *);
    int (*exit_cmd_priv)(struct Scsi_Host *, struct scsi_cmnd *);
    int (*queuecommand)(struct Scsi_Host *, struct scsi_cmnd *);
    void (*commit_rqs)(struct Scsi_Host *, u16);
    int (*eh_abort_handler)(struct scsi_cmnd *);
    int (*eh_device_reset_handler)(struct scsi_cmnd *);
    int (*eh_target_reset_handler)(struct scsi_cmnd *);
    int (*eh_bus_reset_handler)(struct scsi_cmnd *);
    int (*eh_host_reset_handler)(struct scsi_cmnd *);
    int (*slave_alloc)(struct scsi_device *);
    int (*slave_configure)(struct scsi_device *);
    void (*slave_destroy)(struct scsi_device *);
    int (*target_alloc)(struct scsi_target *);
    void (*target_destroy)(struct scsi_target *);
    int (*scan_finished)(struct Scsi_Host *, long unsigned int);
    void (*scan_start)(struct Scsi_Host *);
    int (*change_queue_depth)(struct scsi_device *, int);
    int (*map_queues)(struct Scsi_Host *);
    bool (*dma_need_drain)(struct request *);
    int (*bios_param)(struct scsi_device *, struct block_device *, sector_t, int *);
    void (*unlock_native_capacity)(struct scsi_device *);
    int (*show_info)(struct seq_file *, struct Scsi_Host *);
    int (*write_info)(struct Scsi_Host *, char *, int);
    enum blk_eh_timer_return (*eh_timed_out)(struct scsi_cmnd *);
    int (*host_reset)(struct Scsi_Host *, int);
    const char *proc_name;
    struct proc_dir_entry *proc_dir;
    int can_queue;
    int this_id;
    short unsigned int sg_tablesize;
    short unsigned int sg_prot_tablesize;
    unsigned int max_sectors;
    unsigned int max_segment_size;
    long unsigned int dma_boundary;
    long unsigned int virt_boundary_mask;
    short int cmd_per_lun;
    unsigned char present;
    int tag_alloc_policy;
    unsigned int track_queue_depth;
    unsigned int supported_mode;
    unsigned int unchecked_isa_dma;
    unsigned int emulated;
    unsigned int skip_settle_delay;
    unsigned int no_write_same;
    unsigned int host_tagset;
    unsigned int max_host_blocked;
    struct device_attribute **shost_attrs;
    struct device_attribute **sdev_attrs;
    const struct attribute_group **sdev_groups;
    u64 vendor_id;
    unsigned int cmd_size;
    struct scsi_host_cmd_pool *cmd_pool;
    int rpm_autosuspend_delay;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct scsi_host_template {
    unsigned int cmd_size;
    int (*queuecommand)(struct Scsi_Host *, struct scsi_cmnd *);
    void (*commit_rqs)(struct Scsi_Host *, u16);
    struct module *module;
    const char *name;
    const char * (*info)(struct Scsi_Host *);
    int (*ioctl)(struct scsi_device *, unsigned int, void *);
    int (*compat_ioctl)(struct scsi_device *, unsigned int, void *);
    int (*init_cmd_priv)(struct Scsi_Host *, struct scsi_cmnd *);
    int (*exit_cmd_priv)(struct Scsi_Host *, struct scsi_cmnd *);
    int (*eh_abort_handler)(struct scsi_cmnd *);
    int (*eh_device_reset_handler)(struct scsi_cmnd *);
    int (*eh_target_reset_handler)(struct scsi_cmnd *);
    int (*eh_bus_reset_handler)(struct scsi_cmnd *);
    int (*eh_host_reset_handler)(struct scsi_cmnd *);
    int (*slave_alloc)(struct scsi_device *);
    int (*slave_configure)(struct scsi_device *);
    void (*slave_destroy)(struct scsi_device *);
    int (*target_alloc)(struct scsi_target *);
    void (*target_destroy)(struct scsi_target *);
    int (*scan_finished)(struct Scsi_Host *, long unsigned int);
    void (*scan_start)(struct Scsi_Host *);
    int (*change_queue_depth)(struct scsi_device *, int);
    int (*map_queues)(struct Scsi_Host *);
    int (*mq_poll)(struct Scsi_Host *, unsigned int);
    bool (*dma_need_drain)(struct request *);
    int (*bios_param)(struct scsi_device *, struct block_device *, sector_t, int *);
    void (*unlock_native_capacity)(struct scsi_device *);
    int (*show_info)(struct seq_file *, struct Scsi_Host *);
    int (*write_info)(struct Scsi_Host *, char *, int);
    enum blk_eh_timer_return (*eh_timed_out)(struct scsi_cmnd *);
    bool (*eh_should_retry_cmd)(struct scsi_cmnd *);
    int (*host_reset)(struct Scsi_Host *, int);
    const char *proc_name;
    struct proc_dir_entry *proc_dir;
    int can_queue;
    int this_id;
    short unsigned int sg_tablesize;
    short unsigned int sg_prot_tablesize;
    unsigned int max_sectors;
    unsigned int max_segment_size;
    long unsigned int dma_boundary;
    long unsigned int virt_boundary_mask;
    short int cmd_per_lun;
    unsigned char present;
    int tag_alloc_policy;
    unsigned int track_queue_depth;
    unsigned int supported_mode;
    unsigned int emulated;
    unsigned int skip_settle_delay;
    unsigned int no_write_same;
    unsigned int host_tagset;
    unsigned int max_host_blocked;
    struct device_attribute **shost_attrs;
    struct device_attribute **sdev_attrs;
    const struct attribute_group **sdev_groups;
    u64 vendor_id;
    struct scsi_host_cmd_pool *cmd_pool;
    int rpm_autosuspend_delay;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct scsi_host_template {
    unsigned int cmd_size;
    int (*queuecommand)(struct Scsi_Host *, struct scsi_cmnd *);
    void (*commit_rqs)(struct Scsi_Host *, u16);
    struct module *module;
    const char *name;
    const char * (*info)(struct Scsi_Host *);
    int (*ioctl)(struct scsi_device *, unsigned int, void *);
    int (*compat_ioctl)(struct scsi_device *, unsigned int, void *);
    int (*init_cmd_priv)(struct Scsi_Host *, struct scsi_cmnd *);
    int (*exit_cmd_priv)(struct Scsi_Host *, struct scsi_cmnd *);
    int (*eh_abort_handler)(struct scsi_cmnd *);
    int (*eh_device_reset_handler)(struct scsi_cmnd *);
    int (*eh_target_reset_handler)(struct scsi_cmnd *);
    int (*eh_bus_reset_handler)(struct scsi_cmnd *);
    int (*eh_host_reset_handler)(struct scsi_cmnd *);
    int (*slave_alloc)(struct scsi_device *);
    int (*slave_configure)(struct scsi_device *);
    void (*slave_destroy)(struct scsi_device *);
    int (*target_alloc)(struct scsi_target *);
    void (*target_destroy)(struct scsi_target *);
    int (*scan_finished)(struct Scsi_Host *, long unsigned int);
    void (*scan_start)(struct Scsi_Host *);
    int (*change_queue_depth)(struct scsi_device *, int);
    int (*map_queues)(struct Scsi_Host *);
    int (*mq_poll)(struct Scsi_Host *, unsigned int);
    bool (*dma_need_drain)(struct request *);
    int (*bios_param)(struct scsi_device *, struct block_device *, sector_t, int *);
    void (*unlock_native_capacity)(struct scsi_device *);
    int (*show_info)(struct seq_file *, struct Scsi_Host *);
    int (*write_info)(struct Scsi_Host *, char *, int);
    enum blk_eh_timer_return (*eh_timed_out)(struct scsi_cmnd *);
    bool (*eh_should_retry_cmd)(struct scsi_cmnd *);
    int (*host_reset)(struct Scsi_Host *, int);
    const char *proc_name;
    struct proc_dir_entry *proc_dir;
    int can_queue;
    int this_id;
    short unsigned int sg_tablesize;
    short unsigned int sg_prot_tablesize;
    unsigned int max_sectors;
    unsigned int max_segment_size;
    long unsigned int dma_boundary;
    long unsigned int virt_boundary_mask;
    short int cmd_per_lun;
    unsigned char present;
    int tag_alloc_policy;
    unsigned int track_queue_depth;
    unsigned int supported_mode;
    unsigned int emulated;
    unsigned int skip_settle_delay;
    unsigned int no_write_same;
    unsigned int host_tagset;
    unsigned int max_host_blocked;
    struct device_attribute **shost_attrs;
    struct device_attribute **sdev_attrs;
    const struct attribute_group **sdev_groups;
    u64 vendor_id;
    struct scsi_host_cmd_pool *cmd_pool;
    int rpm_autosuspend_delay;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct scsi_host_template {
    unsigned int cmd_size;
    int (*queuecommand)(struct Scsi_Host *, struct scsi_cmnd *);
    void (*commit_rqs)(struct Scsi_Host *, u16);
    struct module *module;
    const char *name;
    const char * (*info)(struct Scsi_Host *);
    int (*ioctl)(struct scsi_device *, unsigned int, void *);
    int (*compat_ioctl)(struct scsi_device *, unsigned int, void *);
    int (*init_cmd_priv)(struct Scsi_Host *, struct scsi_cmnd *);
    int (*exit_cmd_priv)(struct Scsi_Host *, struct scsi_cmnd *);
    int (*eh_abort_handler)(struct scsi_cmnd *);
    int (*eh_device_reset_handler)(struct scsi_cmnd *);
    int (*eh_target_reset_handler)(struct scsi_cmnd *);
    int (*eh_bus_reset_handler)(struct scsi_cmnd *);
    int (*eh_host_reset_handler)(struct scsi_cmnd *);
    int (*slave_alloc)(struct scsi_device *);
    int (*slave_configure)(struct scsi_device *);
    void (*slave_destroy)(struct scsi_device *);
    int (*target_alloc)(struct scsi_target *);
    void (*target_destroy)(struct scsi_target *);
    int (*scan_finished)(struct Scsi_Host *, long unsigned int);
    void (*scan_start)(struct Scsi_Host *);
    int (*change_queue_depth)(struct scsi_device *, int);
    int (*map_queues)(struct Scsi_Host *);
    int (*mq_poll)(struct Scsi_Host *, unsigned int);
    bool (*dma_need_drain)(struct request *);
    int (*bios_param)(struct scsi_device *, struct block_device *, sector_t, int *);
    void (*unlock_native_capacity)(struct scsi_device *);
    int (*show_info)(struct seq_file *, struct Scsi_Host *);
    int (*write_info)(struct Scsi_Host *, char *, int);
    enum blk_eh_timer_return (*eh_timed_out)(struct scsi_cmnd *);
    bool (*eh_should_retry_cmd)(struct scsi_cmnd *);
    int (*host_reset)(struct Scsi_Host *, int);
    const char *proc_name;
    struct proc_dir_entry *proc_dir;
    int can_queue;
    int this_id;
    short unsigned int sg_tablesize;
    short unsigned int sg_prot_tablesize;
    unsigned int max_sectors;
    unsigned int max_segment_size;
    long unsigned int dma_boundary;
    long unsigned int virt_boundary_mask;
    short int cmd_per_lun;
    unsigned char present;
    int tag_alloc_policy;
    unsigned int track_queue_depth;
    unsigned int supported_mode;
    unsigned int emulated;
    unsigned int skip_settle_delay;
    unsigned int no_write_same;
    unsigned int host_tagset;
    unsigned int max_host_blocked;
    const struct attribute_group **shost_groups;
    const struct attribute_group **sdev_groups;
    u64 vendor_id;
    int rpm_autosuspend_delay;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct scsi_host_template {
    unsigned int cmd_size;
    int (*queuecommand)(struct Scsi_Host *, struct scsi_cmnd *);
    void (*commit_rqs)(struct Scsi_Host *, u16);
    struct module *module;
    const char *name;
    const char * (*info)(struct Scsi_Host *);
    int (*ioctl)(struct scsi_device *, unsigned int, void *);
    int (*compat_ioctl)(struct scsi_device *, unsigned int, void *);
    int (*init_cmd_priv)(struct Scsi_Host *, struct scsi_cmnd *);
    int (*exit_cmd_priv)(struct Scsi_Host *, struct scsi_cmnd *);
    int (*eh_abort_handler)(struct scsi_cmnd *);
    int (*eh_device_reset_handler)(struct scsi_cmnd *);
    int (*eh_target_reset_handler)(struct scsi_cmnd *);
    int (*eh_bus_reset_handler)(struct scsi_cmnd *);
    int (*eh_host_reset_handler)(struct scsi_cmnd *);
    int (*slave_alloc)(struct scsi_device *);
    int (*slave_configure)(struct scsi_device *);
    void (*slave_destroy)(struct scsi_device *);
    int (*target_alloc)(struct scsi_target *);
    void (*target_destroy)(struct scsi_target *);
    int (*scan_finished)(struct Scsi_Host *, long unsigned int);
    void (*scan_start)(struct Scsi_Host *);
    int (*change_queue_depth)(struct scsi_device *, int);
    void (*map_queues)(struct Scsi_Host *);
    int (*mq_poll)(struct Scsi_Host *, unsigned int);
    bool (*dma_need_drain)(struct request *);
    int (*bios_param)(struct scsi_device *, struct block_device *, sector_t, int *);
    void (*unlock_native_capacity)(struct scsi_device *);
    int (*show_info)(struct seq_file *, struct Scsi_Host *);
    int (*write_info)(struct Scsi_Host *, char *, int);
    enum scsi_timeout_action (*eh_timed_out)(struct scsi_cmnd *);
    bool (*eh_should_retry_cmd)(struct scsi_cmnd *);
    int (*host_reset)(struct Scsi_Host *, int);
    const char *proc_name;
    int can_queue;
    int this_id;
    short unsigned int sg_tablesize;
    short unsigned int sg_prot_tablesize;
    unsigned int max_sectors;
    unsigned int max_segment_size;
    long unsigned int dma_boundary;
    long unsigned int virt_boundary_mask;
    short int cmd_per_lun;
    int tag_alloc_policy;
    unsigned int track_queue_depth;
    unsigned int supported_mode;
    unsigned int emulated;
    unsigned int skip_settle_delay;
    unsigned int no_write_same;
    unsigned int host_tagset;
    unsigned int max_host_blocked;
    const struct attribute_group **shost_groups;
    const struct attribute_group **sdev_groups;
    u64 vendor_id;
    int rpm_autosuspend_delay;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct scsi_host_template {
    unsigned int cmd_size;
    int (*queuecommand)(struct Scsi_Host *, struct scsi_cmnd *);
    void (*commit_rqs)(struct Scsi_Host *, u16);
    struct module *module;
    const char *name;
    const char * (*info)(struct Scsi_Host *);
    int (*ioctl)(struct scsi_device *, unsigned int, void *);
    int (*compat_ioctl)(struct scsi_device *, unsigned int, void *);
    int (*init_cmd_priv)(struct Scsi_Host *, struct scsi_cmnd *);
    int (*exit_cmd_priv)(struct Scsi_Host *, struct scsi_cmnd *);
    int (*eh_abort_handler)(struct scsi_cmnd *);
    int (*eh_device_reset_handler)(struct scsi_cmnd *);
    int (*eh_target_reset_handler)(struct scsi_cmnd *);
    int (*eh_bus_reset_handler)(struct scsi_cmnd *);
    int (*eh_host_reset_handler)(struct scsi_cmnd *);
    int (*slave_alloc)(struct scsi_device *);
    int (*slave_configure)(struct scsi_device *);
    void (*slave_destroy)(struct scsi_device *);
    int (*target_alloc)(struct scsi_target *);
    void (*target_destroy)(struct scsi_target *);
    int (*scan_finished)(struct Scsi_Host *, long unsigned int);
    void (*scan_start)(struct Scsi_Host *);
    int (*change_queue_depth)(struct scsi_device *, int);
    void (*map_queues)(struct Scsi_Host *);
    int (*mq_poll)(struct Scsi_Host *, unsigned int);
    bool (*dma_need_drain)(struct request *);
    int (*bios_param)(struct scsi_device *, struct block_device *, sector_t, int *);
    void (*unlock_native_capacity)(struct scsi_device *);
    int (*show_info)(struct seq_file *, struct Scsi_Host *);
    int (*write_info)(struct Scsi_Host *, char *, int);
    enum scsi_timeout_action (*eh_timed_out)(struct scsi_cmnd *);
    bool (*eh_should_retry_cmd)(struct scsi_cmnd *);
    int (*host_reset)(struct Scsi_Host *, int);
    const char *proc_name;
    int can_queue;
    int this_id;
    short unsigned int sg_tablesize;
    short unsigned int sg_prot_tablesize;
    unsigned int max_sectors;
    unsigned int max_segment_size;
    long unsigned int dma_boundary;
    long unsigned int virt_boundary_mask;
    short int cmd_per_lun;
    int tag_alloc_policy;
    unsigned int track_queue_depth;
    unsigned int supported_mode;
    unsigned int emulated;
    unsigned int skip_settle_delay;
    unsigned int no_write_same;
    unsigned int host_tagset;
    unsigned int queuecommand_may_block;
    unsigned int max_host_blocked;
    const struct attribute_group **shost_groups;
    const struct attribute_group **sdev_groups;
    u64 vendor_id;
    int rpm_autosuspend_delay;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct scsi_host_template {
    unsigned int cmd_size;
    int (*queuecommand)(struct Scsi_Host *, struct scsi_cmnd *);
    void (*commit_rqs)(struct Scsi_Host *, u16);
    struct module *module;
    const char *name;
    const char * (*info)(struct Scsi_Host *);
    int (*ioctl)(struct scsi_device *, unsigned int, void *);
    int (*compat_ioctl)(struct scsi_device *, unsigned int, void *);
    int (*init_cmd_priv)(struct Scsi_Host *, struct scsi_cmnd *);
    int (*exit_cmd_priv)(struct Scsi_Host *, struct scsi_cmnd *);
    int (*eh_abort_handler)(struct scsi_cmnd *);
    int (*eh_device_reset_handler)(struct scsi_cmnd *);
    int (*eh_target_reset_handler)(struct scsi_cmnd *);
    int (*eh_bus_reset_handler)(struct scsi_cmnd *);
    int (*eh_host_reset_handler)(struct scsi_cmnd *);
    int (*slave_alloc)(struct scsi_device *);
    int (*slave_configure)(struct scsi_device *);
    void (*slave_destroy)(struct scsi_device *);
    int (*target_alloc)(struct scsi_target *);
    void (*target_destroy)(struct scsi_target *);
    int (*scan_finished)(struct Scsi_Host *, long unsigned int);
    void (*scan_start)(struct Scsi_Host *);
    int (*change_queue_depth)(struct scsi_device *, int);
    void (*map_queues)(struct Scsi_Host *);
    int (*mq_poll)(struct Scsi_Host *, unsigned int);
    bool (*dma_need_drain)(struct request *);
    int (*bios_param)(struct scsi_device *, struct block_device *, sector_t, int *);
    void (*unlock_native_capacity)(struct scsi_device *);
    int (*show_info)(struct seq_file *, struct Scsi_Host *);
    int (*write_info)(struct Scsi_Host *, char *, int);
    enum scsi_timeout_action (*eh_timed_out)(struct scsi_cmnd *);
    bool (*eh_should_retry_cmd)(struct scsi_cmnd *);
    int (*host_reset)(struct Scsi_Host *, int);
    const char *proc_name;
    int can_queue;
    int this_id;
    short unsigned int sg_tablesize;
    short unsigned int sg_prot_tablesize;
    unsigned int max_sectors;
    unsigned int max_segment_size;
    long unsigned int dma_boundary;
    long unsigned int virt_boundary_mask;
    short int cmd_per_lun;
    int tag_alloc_policy;
    unsigned int track_queue_depth;
    unsigned int supported_mode;
    unsigned int emulated;
    unsigned int skip_settle_delay;
    unsigned int no_write_same;
    unsigned int host_tagset;
    unsigned int queuecommand_may_block;
    unsigned int max_host_blocked;
    const struct attribute_group **shost_groups;
    const struct attribute_group **sdev_groups;
    u64 vendor_id;
    int rpm_autosuspend_delay;
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
struct scsi_host_template {
    struct module *module;
    const char *name;
    const char * (*info)(struct Scsi_Host *);
    int (*ioctl)(struct scsi_device *, unsigned int, void *);
    int (*compat_ioctl)(struct scsi_device *, unsigned int, void *);
    int (*queuecommand)(struct Scsi_Host *, struct scsi_cmnd *);
    void (*commit_rqs)(struct Scsi_Host *, u16);
    int (*eh_abort_handler)(struct scsi_cmnd *);
    int (*eh_device_reset_handler)(struct scsi_cmnd *);
    int (*eh_target_reset_handler)(struct scsi_cmnd *);
    int (*eh_bus_reset_handler)(struct scsi_cmnd *);
    int (*eh_host_reset_handler)(struct scsi_cmnd *);
    int (*slave_alloc)(struct scsi_device *);
    int (*slave_configure)(struct scsi_device *);
    void (*slave_destroy)(struct scsi_device *);
    int (*target_alloc)(struct scsi_target *);
    void (*target_destroy)(struct scsi_target *);
    int (*scan_finished)(struct Scsi_Host *, long unsigned int);
    void (*scan_start)(struct Scsi_Host *);
    int (*change_queue_depth)(struct scsi_device *, int);
    int (*map_queues)(struct Scsi_Host *);
    int (*bios_param)(struct scsi_device *, struct block_device *, sector_t, int *);
    void (*unlock_native_capacity)(struct scsi_device *);
    int (*show_info)(struct seq_file *, struct Scsi_Host *);
    int (*write_info)(struct Scsi_Host *, char *, int);
    enum blk_eh_timer_return (*eh_timed_out)(struct scsi_cmnd *);
    int (*host_reset)(struct Scsi_Host *, int);
    const char *proc_name;
    struct proc_dir_entry *proc_dir;
    int can_queue;
    int this_id;
    short unsigned int sg_tablesize;
    short unsigned int sg_prot_tablesize;
    unsigned int max_sectors;
    unsigned int max_segment_size;
    long unsigned int dma_boundary;
    long unsigned int virt_boundary_mask;
    short int cmd_per_lun;
    unsigned char present;
    int tag_alloc_policy;
    unsigned int track_queue_depth;
    unsigned int supported_mode;
    unsigned int unchecked_isa_dma;
    unsigned int emulated;
    unsigned int skip_settle_delay;
    unsigned int no_write_same;
    unsigned int force_blk_mq;
    unsigned int max_host_blocked;
    struct device_attribute **shost_attrs;
    struct device_attribute **sdev_attrs;
    const struct attribute_group **sdev_groups;
    u64 vendor_id;
    unsigned int cmd_size;
    struct scsi_host_cmd_pool *cmd_pool;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct scsi_host_template {
    struct module *module;
    const char *name;
    const char * (*info)(struct Scsi_Host *);
    int (*ioctl)(struct scsi_device *, unsigned int, void *);
    int (*queuecommand)(struct Scsi_Host *, struct scsi_cmnd *);
    void (*commit_rqs)(struct Scsi_Host *, u16);
    int (*eh_abort_handler)(struct scsi_cmnd *);
    int (*eh_device_reset_handler)(struct scsi_cmnd *);
    int (*eh_target_reset_handler)(struct scsi_cmnd *);
    int (*eh_bus_reset_handler)(struct scsi_cmnd *);
    int (*eh_host_reset_handler)(struct scsi_cmnd *);
    int (*slave_alloc)(struct scsi_device *);
    int (*slave_configure)(struct scsi_device *);
    void (*slave_destroy)(struct scsi_device *);
    int (*target_alloc)(struct scsi_target *);
    void (*target_destroy)(struct scsi_target *);
    int (*scan_finished)(struct Scsi_Host *, long unsigned int);
    void (*scan_start)(struct Scsi_Host *);
    int (*change_queue_depth)(struct scsi_device *, int);
    int (*map_queues)(struct Scsi_Host *);
    int (*bios_param)(struct scsi_device *, struct block_device *, sector_t, int *);
    void (*unlock_native_capacity)(struct scsi_device *);
    int (*show_info)(struct seq_file *, struct Scsi_Host *);
    int (*write_info)(struct Scsi_Host *, char *, int);
    enum blk_eh_timer_return (*eh_timed_out)(struct scsi_cmnd *);
    int (*host_reset)(struct Scsi_Host *, int);
    const char *proc_name;
    struct proc_dir_entry *proc_dir;
    int can_queue;
    int this_id;
    short unsigned int sg_tablesize;
    short unsigned int sg_prot_tablesize;
    unsigned int max_sectors;
    unsigned int max_segment_size;
    long unsigned int dma_boundary;
    long unsigned int virt_boundary_mask;
    short int cmd_per_lun;
    unsigned char present;
    int tag_alloc_policy;
    unsigned int track_queue_depth;
    unsigned int supported_mode;
    unsigned int unchecked_isa_dma;
    unsigned int emulated;
    unsigned int skip_settle_delay;
    unsigned int no_write_same;
    unsigned int force_blk_mq;
    unsigned int max_host_blocked;
    struct device_attribute **shost_attrs;
    struct device_attribute **sdev_attrs;
    const struct attribute_group **sdev_groups;
    u64 vendor_id;
    unsigned int cmd_size;
    struct scsi_host_cmd_pool *cmd_pool;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct scsi_host_template {
    struct module *module;
    const char *name;
    const char * (*info)(struct Scsi_Host *);
    int (*ioctl)(struct scsi_device *, unsigned int, void *);
    int (*compat_ioctl)(struct scsi_device *, unsigned int, void *);
    int (*queuecommand)(struct Scsi_Host *, struct scsi_cmnd *);
    void (*commit_rqs)(struct Scsi_Host *, u16);
    int (*eh_abort_handler)(struct scsi_cmnd *);
    int (*eh_device_reset_handler)(struct scsi_cmnd *);
    int (*eh_target_reset_handler)(struct scsi_cmnd *);
    int (*eh_bus_reset_handler)(struct scsi_cmnd *);
    int (*eh_host_reset_handler)(struct scsi_cmnd *);
    int (*slave_alloc)(struct scsi_device *);
    int (*slave_configure)(struct scsi_device *);
    void (*slave_destroy)(struct scsi_device *);
    int (*target_alloc)(struct scsi_target *);
    void (*target_destroy)(struct scsi_target *);
    int (*scan_finished)(struct Scsi_Host *, long unsigned int);
    void (*scan_start)(struct Scsi_Host *);
    int (*change_queue_depth)(struct scsi_device *, int);
    int (*map_queues)(struct Scsi_Host *);
    int (*bios_param)(struct scsi_device *, struct block_device *, sector_t, int *);
    void (*unlock_native_capacity)(struct scsi_device *);
    int (*show_info)(struct seq_file *, struct Scsi_Host *);
    int (*write_info)(struct Scsi_Host *, char *, int);
    enum blk_eh_timer_return (*eh_timed_out)(struct scsi_cmnd *);
    int (*host_reset)(struct Scsi_Host *, int);
    const char *proc_name;
    struct proc_dir_entry *proc_dir;
    int can_queue;
    int this_id;
    short unsigned int sg_tablesize;
    short unsigned int sg_prot_tablesize;
    unsigned int max_sectors;
    unsigned int max_segment_size;
    long unsigned int dma_boundary;
    long unsigned int virt_boundary_mask;
    short int cmd_per_lun;
    unsigned char present;
    int tag_alloc_policy;
    unsigned int track_queue_depth;
    unsigned int supported_mode;
    unsigned int unchecked_isa_dma;
    unsigned int emulated;
    unsigned int skip_settle_delay;
    unsigned int no_write_same;
    unsigned int force_blk_mq;
    unsigned int max_host_blocked;
    struct device_attribute **shost_attrs;
    struct device_attribute **sdev_attrs;
    const struct attribute_group **sdev_groups;
    u64 vendor_id;
    unsigned int cmd_size;
    struct scsi_host_cmd_pool *cmd_pool;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct scsi_host_template {
    struct module *module;
    const char *name;
    const char * (*info)(struct Scsi_Host *);
    int (*ioctl)(struct scsi_device *, unsigned int, void *);
    int (*queuecommand)(struct Scsi_Host *, struct scsi_cmnd *);
    void (*commit_rqs)(struct Scsi_Host *, u16);
    int (*eh_abort_handler)(struct scsi_cmnd *);
    int (*eh_device_reset_handler)(struct scsi_cmnd *);
    int (*eh_target_reset_handler)(struct scsi_cmnd *);
    int (*eh_bus_reset_handler)(struct scsi_cmnd *);
    int (*eh_host_reset_handler)(struct scsi_cmnd *);
    int (*slave_alloc)(struct scsi_device *);
    int (*slave_configure)(struct scsi_device *);
    void (*slave_destroy)(struct scsi_device *);
    int (*target_alloc)(struct scsi_target *);
    void (*target_destroy)(struct scsi_target *);
    int (*scan_finished)(struct Scsi_Host *, long unsigned int);
    void (*scan_start)(struct Scsi_Host *);
    int (*change_queue_depth)(struct scsi_device *, int);
    int (*map_queues)(struct Scsi_Host *);
    int (*bios_param)(struct scsi_device *, struct block_device *, sector_t, int *);
    void (*unlock_native_capacity)(struct scsi_device *);
    int (*show_info)(struct seq_file *, struct Scsi_Host *);
    int (*write_info)(struct Scsi_Host *, char *, int);
    enum blk_eh_timer_return (*eh_timed_out)(struct scsi_cmnd *);
    int (*host_reset)(struct Scsi_Host *, int);
    const char *proc_name;
    struct proc_dir_entry *proc_dir;
    int can_queue;
    int this_id;
    short unsigned int sg_tablesize;
    short unsigned int sg_prot_tablesize;
    unsigned int max_sectors;
    unsigned int max_segment_size;
    long unsigned int dma_boundary;
    long unsigned int virt_boundary_mask;
    short int cmd_per_lun;
    unsigned char present;
    int tag_alloc_policy;
    unsigned int track_queue_depth;
    unsigned int supported_mode;
    unsigned int unchecked_isa_dma;
    unsigned int emulated;
    unsigned int skip_settle_delay;
    unsigned int no_write_same;
    unsigned int force_blk_mq;
    unsigned int max_host_blocked;
    struct device_attribute **shost_attrs;
    struct device_attribute **sdev_attrs;
    const struct attribute_group **sdev_groups;
    u64 vendor_id;
    unsigned int cmd_size;
    struct scsi_host_cmd_pool *cmd_pool;
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
struct scsi_host_template {
    struct module *module;
    const char *name;
    const char * (*info)(struct Scsi_Host *);
    int (*ioctl)(struct scsi_device *, unsigned int, void *);
    int (*compat_ioctl)(struct scsi_device *, unsigned int, void *);
    int (*queuecommand)(struct Scsi_Host *, struct scsi_cmnd *);
    void (*commit_rqs)(struct Scsi_Host *, u16);
    int (*eh_abort_handler)(struct scsi_cmnd *);
    int (*eh_device_reset_handler)(struct scsi_cmnd *);
    int (*eh_target_reset_handler)(struct scsi_cmnd *);
    int (*eh_bus_reset_handler)(struct scsi_cmnd *);
    int (*eh_host_reset_handler)(struct scsi_cmnd *);
    int (*slave_alloc)(struct scsi_device *);
    int (*slave_configure)(struct scsi_device *);
    void (*slave_destroy)(struct scsi_device *);
    int (*target_alloc)(struct scsi_target *);
    void (*target_destroy)(struct scsi_target *);
    int (*scan_finished)(struct Scsi_Host *, long unsigned int);
    void (*scan_start)(struct Scsi_Host *);
    int (*change_queue_depth)(struct scsi_device *, int);
    int (*map_queues)(struct Scsi_Host *);
    int (*bios_param)(struct scsi_device *, struct block_device *, sector_t, int *);
    void (*unlock_native_capacity)(struct scsi_device *);
    int (*show_info)(struct seq_file *, struct Scsi_Host *);
    int (*write_info)(struct Scsi_Host *, char *, int);
    enum blk_eh_timer_return (*eh_timed_out)(struct scsi_cmnd *);
    int (*host_reset)(struct Scsi_Host *, int);
    const char *proc_name;
    struct proc_dir_entry *proc_dir;
    int can_queue;
    int this_id;
    short unsigned int sg_tablesize;
    short unsigned int sg_prot_tablesize;
    unsigned int max_sectors;
    unsigned int max_segment_size;
    long unsigned int dma_boundary;
    long unsigned int virt_boundary_mask;
    short int cmd_per_lun;
    unsigned char present;
    int tag_alloc_policy;
    unsigned int track_queue_depth;
    unsigned int supported_mode;
    unsigned int unchecked_isa_dma;
    unsigned int emulated;
    unsigned int skip_settle_delay;
    unsigned int no_write_same;
    unsigned int force_blk_mq;
    unsigned int max_host_blocked;
    struct device_attribute **shost_attrs;
    struct device_attribute **sdev_attrs;
    const struct attribute_group **sdev_groups;
    u64 vendor_id;
    unsigned int cmd_size;
    struct scsi_host_cmd_pool *cmd_pool;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct scsi_host_template {
    struct module *module;
    const char *name;
    const char * (*info)(struct Scsi_Host *);
    int (*ioctl)(struct scsi_device *, unsigned int, void *);
    int (*compat_ioctl)(struct scsi_device *, unsigned int, void *);
    int (*queuecommand)(struct Scsi_Host *, struct scsi_cmnd *);
    void (*commit_rqs)(struct Scsi_Host *, u16);
    int (*eh_abort_handler)(struct scsi_cmnd *);
    int (*eh_device_reset_handler)(struct scsi_cmnd *);
    int (*eh_target_reset_handler)(struct scsi_cmnd *);
    int (*eh_bus_reset_handler)(struct scsi_cmnd *);
    int (*eh_host_reset_handler)(struct scsi_cmnd *);
    int (*slave_alloc)(struct scsi_device *);
    int (*slave_configure)(struct scsi_device *);
    void (*slave_destroy)(struct scsi_device *);
    int (*target_alloc)(struct scsi_target *);
    void (*target_destroy)(struct scsi_target *);
    int (*scan_finished)(struct Scsi_Host *, long unsigned int);
    void (*scan_start)(struct Scsi_Host *);
    int (*change_queue_depth)(struct scsi_device *, int);
    int (*map_queues)(struct Scsi_Host *);
    int (*bios_param)(struct scsi_device *, struct block_device *, sector_t, int *);
    void (*unlock_native_capacity)(struct scsi_device *);
    int (*show_info)(struct seq_file *, struct Scsi_Host *);
    int (*write_info)(struct Scsi_Host *, char *, int);
    enum blk_eh_timer_return (*eh_timed_out)(struct scsi_cmnd *);
    int (*host_reset)(struct Scsi_Host *, int);
    const char *proc_name;
    struct proc_dir_entry *proc_dir;
    int can_queue;
    int this_id;
    short unsigned int sg_tablesize;
    short unsigned int sg_prot_tablesize;
    unsigned int max_sectors;
    unsigned int max_segment_size;
    long unsigned int dma_boundary;
    long unsigned int virt_boundary_mask;
    short int cmd_per_lun;
    unsigned char present;
    int tag_alloc_policy;
    unsigned int track_queue_depth;
    unsigned int supported_mode;
    unsigned int unchecked_isa_dma;
    unsigned int emulated;
    unsigned int skip_settle_delay;
    unsigned int no_write_same;
    unsigned int force_blk_mq;
    unsigned int max_host_blocked;
    struct device_attribute **shost_attrs;
    struct device_attribute **sdev_attrs;
    const struct attribute_group **sdev_groups;
    u64 vendor_id;
    unsigned int cmd_size;
    struct scsi_host_cmd_pool *cmd_pool;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct scsi_host_template {
    struct module *module;
    const char *name;
    const char * (*info)(struct Scsi_Host *);
    int (*ioctl)(struct scsi_device *, unsigned int, void *);
    int (*compat_ioctl)(struct scsi_device *, unsigned int, void *);
    int (*queuecommand)(struct Scsi_Host *, struct scsi_cmnd *);
    void (*commit_rqs)(struct Scsi_Host *, u16);
    int (*eh_abort_handler)(struct scsi_cmnd *);
    int (*eh_device_reset_handler)(struct scsi_cmnd *);
    int (*eh_target_reset_handler)(struct scsi_cmnd *);
    int (*eh_bus_reset_handler)(struct scsi_cmnd *);
    int (*eh_host_reset_handler)(struct scsi_cmnd *);
    int (*slave_alloc)(struct scsi_device *);
    int (*slave_configure)(struct scsi_device *);
    void (*slave_destroy)(struct scsi_device *);
    int (*target_alloc)(struct scsi_target *);
    void (*target_destroy)(struct scsi_target *);
    int (*scan_finished)(struct Scsi_Host *, long unsigned int);
    void (*scan_start)(struct Scsi_Host *);
    int (*change_queue_depth)(struct scsi_device *, int);
    int (*map_queues)(struct Scsi_Host *);
    int (*bios_param)(struct scsi_device *, struct block_device *, sector_t, int *);
    void (*unlock_native_capacity)(struct scsi_device *);
    int (*show_info)(struct seq_file *, struct Scsi_Host *);
    int (*write_info)(struct Scsi_Host *, char *, int);
    enum blk_eh_timer_return (*eh_timed_out)(struct scsi_cmnd *);
    int (*host_reset)(struct Scsi_Host *, int);
    const char *proc_name;
    struct proc_dir_entry *proc_dir;
    int can_queue;
    int this_id;
    short unsigned int sg_tablesize;
    short unsigned int sg_prot_tablesize;
    unsigned int max_sectors;
    unsigned int max_segment_size;
    long unsigned int dma_boundary;
    long unsigned int virt_boundary_mask;
    short int cmd_per_lun;
    unsigned char present;
    int tag_alloc_policy;
    unsigned int track_queue_depth;
    unsigned int supported_mode;
    unsigned int unchecked_isa_dma;
    unsigned int emulated;
    unsigned int skip_settle_delay;
    unsigned int no_write_same;
    unsigned int force_blk_mq;
    unsigned int max_host_blocked;
    struct device_attribute **shost_attrs;
    struct device_attribute **sdev_attrs;
    const struct attribute_group **sdev_groups;
    u64 vendor_id;
    unsigned int cmd_size;
    struct scsi_host_cmd_pool *cmd_pool;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct scsi_host_template {
    struct module *module;
    const char *name;
    const char * (*info)(struct Scsi_Host *);
    int (*ioctl)(struct scsi_device *, unsigned int, void *);
    int (*compat_ioctl)(struct scsi_device *, unsigned int, void *);
    int (*queuecommand)(struct Scsi_Host *, struct scsi_cmnd *);
    void (*commit_rqs)(struct Scsi_Host *, u16);
    int (*eh_abort_handler)(struct scsi_cmnd *);
    int (*eh_device_reset_handler)(struct scsi_cmnd *);
    int (*eh_target_reset_handler)(struct scsi_cmnd *);
    int (*eh_bus_reset_handler)(struct scsi_cmnd *);
    int (*eh_host_reset_handler)(struct scsi_cmnd *);
    int (*slave_alloc)(struct scsi_device *);
    int (*slave_configure)(struct scsi_device *);
    void (*slave_destroy)(struct scsi_device *);
    int (*target_alloc)(struct scsi_target *);
    void (*target_destroy)(struct scsi_target *);
    int (*scan_finished)(struct Scsi_Host *, long unsigned int);
    void (*scan_start)(struct Scsi_Host *);
    int (*change_queue_depth)(struct scsi_device *, int);
    int (*map_queues)(struct Scsi_Host *);
    int (*bios_param)(struct scsi_device *, struct block_device *, sector_t, int *);
    void (*unlock_native_capacity)(struct scsi_device *);
    int (*show_info)(struct seq_file *, struct Scsi_Host *);
    int (*write_info)(struct Scsi_Host *, char *, int);
    enum blk_eh_timer_return (*eh_timed_out)(struct scsi_cmnd *);
    int (*host_reset)(struct Scsi_Host *, int);
    const char *proc_name;
    struct proc_dir_entry *proc_dir;
    int can_queue;
    int this_id;
    short unsigned int sg_tablesize;
    short unsigned int sg_prot_tablesize;
    unsigned int max_sectors;
    unsigned int max_segment_size;
    long unsigned int dma_boundary;
    long unsigned int virt_boundary_mask;
    short int cmd_per_lun;
    unsigned char present;
    int tag_alloc_policy;
    unsigned int track_queue_depth;
    unsigned int supported_mode;
    unsigned int unchecked_isa_dma;
    unsigned int emulated;
    unsigned int skip_settle_delay;
    unsigned int no_write_same;
    unsigned int force_blk_mq;
    unsigned int max_host_blocked;
    struct device_attribute **shost_attrs;
    struct device_attribute **sdev_attrs;
    const struct attribute_group **sdev_groups;
    u64 vendor_id;
    unsigned int cmd_size;
    struct scsi_host_cmd_pool *cmd_pool;
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
<b>Field removed. </b>
<code>bool disable_blk_mq</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*map_queues)(struct Scsi_Host *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned int no_async_abort</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct scsi_host_cmd_pool *cmd_pool</code> ➡️ <code>struct scsi_host_cmd_pool *cmd_pool</code>
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
<b>Field added. </b>
<code>unsigned int force_blk_mq</code>
</li>
<li>
<b>Field added. </b>
<code>const struct attribute_group **sdev_groups</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*detect)(struct scsi_host_template *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*release)(struct Scsi_Host *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head legacy_hosts</code>
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
<code>unsigned int max_segment_size</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int use_clustering</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int virt_boundary_mask</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*ioctl)(struct scsi_device *, int, void *)</code> ➡️ <code>int (*ioctl)(struct scsi_device *, unsigned int, void *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*compat_ioctl)(struct scsi_device *, int, void *)</code> ➡️ <code>int (*compat_ioctl)(struct scsi_device *, unsigned int, void *)</code>
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
<code>void (*commit_rqs)(struct Scsi_Host *, u16)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*init_cmd_priv)(struct Scsi_Host *, struct scsi_cmnd *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*exit_cmd_priv)(struct Scsi_Host *, struct scsi_cmnd *)</code>
</li>
<li>
<b>Field added. </b>
<code>bool (*dma_need_drain)(struct request *)</code>
</li>
<li>
<b>Field added. </b>
<code>int rpm_autosuspend_delay</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int force_blk_mq</code>
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
<code>unsigned int host_tagset</code>
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
<code>int (*mq_poll)(struct Scsi_Host *, unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>bool (*eh_should_retry_cmd)(struct scsi_cmnd *)</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int unchecked_isa_dma</code>
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
<code>const struct attribute_group **shost_groups</code>
</li>
<li>
<b>Field removed. </b>
<code>struct device_attribute **shost_attrs</code>
</li>
<li>
<b>Field removed. </b>
<code>struct device_attribute **sdev_attrs</code>
</li>
<li>
<b>Field removed. </b>
<code>struct scsi_host_cmd_pool *cmd_pool</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct proc_dir_entry *proc_dir</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned char present</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*map_queues)(struct Scsi_Host *)</code> ➡️ <code>void (*map_queues)(struct Scsi_Host *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>enum blk_eh_timer_return (*eh_timed_out)(struct scsi_cmnd *)</code> ➡️ <code>enum scsi_timeout_action (*eh_timed_out)(struct scsi_cmnd *)</code>
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
<code>unsigned int queuecommand_may_block</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*compat_ioctl)(struct scsi_device *, unsigned int, void *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*compat_ioctl)(struct scsi_device *, unsigned int, void *)</code>
</li>
</ul>
</details>
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
