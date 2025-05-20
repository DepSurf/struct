# Struct: <code>target_type</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct target_type {
    uint64_t features;
    const char *name;
    struct module *module;
    unsigned int version[3];
    dm_ctr_fn ctr;
    dm_dtr_fn dtr;
    dm_map_fn map;
    dm_map_request_fn map_rq;
    dm_clone_and_map_request_fn clone_and_map_rq;
    dm_release_clone_request_fn release_clone_rq;
    dm_endio_fn end_io;
    dm_request_endio_fn rq_end_io;
    dm_presuspend_fn presuspend;
    dm_presuspend_undo_fn presuspend_undo;
    dm_postsuspend_fn postsuspend;
    dm_preresume_fn preresume;
    dm_resume_fn resume;
    dm_status_fn status;
    dm_message_fn message;
    dm_prepare_ioctl_fn prepare_ioctl;
    dm_busy_fn busy;
    dm_iterate_devices_fn iterate_devices;
    dm_io_hints_fn io_hints;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct target_type {
    uint64_t features;
    const char *name;
    struct module *module;
    unsigned int version[3];
    dm_ctr_fn ctr;
    dm_dtr_fn dtr;
    dm_map_fn map;
    dm_map_request_fn map_rq;
    dm_clone_and_map_request_fn clone_and_map_rq;
    dm_release_clone_request_fn release_clone_rq;
    dm_endio_fn end_io;
    dm_request_endio_fn rq_end_io;
    dm_presuspend_fn presuspend;
    dm_presuspend_undo_fn presuspend_undo;
    dm_postsuspend_fn postsuspend;
    dm_preresume_fn preresume;
    dm_resume_fn resume;
    dm_status_fn status;
    dm_message_fn message;
    dm_prepare_ioctl_fn prepare_ioctl;
    dm_busy_fn busy;
    dm_iterate_devices_fn iterate_devices;
    dm_io_hints_fn io_hints;
    dm_direct_access_fn direct_access;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct target_type {
    uint64_t features;
    const char *name;
    struct module *module;
    unsigned int version[3];
    dm_ctr_fn ctr;
    dm_dtr_fn dtr;
    dm_map_fn map;
    dm_map_request_fn map_rq;
    dm_clone_and_map_request_fn clone_and_map_rq;
    dm_release_clone_request_fn release_clone_rq;
    dm_endio_fn end_io;
    dm_request_endio_fn rq_end_io;
    dm_presuspend_fn presuspend;
    dm_presuspend_undo_fn presuspend_undo;
    dm_postsuspend_fn postsuspend;
    dm_preresume_fn preresume;
    dm_resume_fn resume;
    dm_status_fn status;
    dm_message_fn message;
    dm_prepare_ioctl_fn prepare_ioctl;
    dm_busy_fn busy;
    dm_iterate_devices_fn iterate_devices;
    dm_io_hints_fn io_hints;
    dm_direct_access_fn direct_access;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct target_type {
    uint64_t features;
    const char *name;
    struct module *module;
    unsigned int version[3];
    dm_ctr_fn ctr;
    dm_dtr_fn dtr;
    dm_map_fn map;
    dm_clone_and_map_request_fn clone_and_map_rq;
    dm_release_clone_request_fn release_clone_rq;
    dm_endio_fn end_io;
    dm_request_endio_fn rq_end_io;
    dm_presuspend_fn presuspend;
    dm_presuspend_undo_fn presuspend_undo;
    dm_postsuspend_fn postsuspend;
    dm_preresume_fn preresume;
    dm_resume_fn resume;
    dm_status_fn status;
    dm_message_fn message;
    dm_prepare_ioctl_fn prepare_ioctl;
    dm_busy_fn busy;
    dm_iterate_devices_fn iterate_devices;
    dm_io_hints_fn io_hints;
    dm_dax_direct_access_fn direct_access;
    dm_dax_copy_from_iter_fn dax_copy_from_iter;
    dm_dax_flush_fn dax_flush;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct target_type {
    uint64_t features;
    const char *name;
    struct module *module;
    unsigned int version[3];
    dm_ctr_fn ctr;
    dm_dtr_fn dtr;
    dm_map_fn map;
    dm_clone_and_map_request_fn clone_and_map_rq;
    dm_release_clone_request_fn release_clone_rq;
    dm_endio_fn end_io;
    dm_request_endio_fn rq_end_io;
    dm_presuspend_fn presuspend;
    dm_presuspend_undo_fn presuspend_undo;
    dm_postsuspend_fn postsuspend;
    dm_preresume_fn preresume;
    dm_resume_fn resume;
    dm_status_fn status;
    dm_message_fn message;
    dm_prepare_ioctl_fn prepare_ioctl;
    dm_busy_fn busy;
    dm_iterate_devices_fn iterate_devices;
    dm_io_hints_fn io_hints;
    dm_dax_direct_access_fn direct_access;
    dm_dax_copy_from_iter_fn dax_copy_from_iter;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct target_type {
    uint64_t features;
    const char *name;
    struct module *module;
    unsigned int version[3];
    dm_ctr_fn ctr;
    dm_dtr_fn dtr;
    dm_map_fn map;
    dm_clone_and_map_request_fn clone_and_map_rq;
    dm_release_clone_request_fn release_clone_rq;
    dm_endio_fn end_io;
    dm_request_endio_fn rq_end_io;
    dm_presuspend_fn presuspend;
    dm_presuspend_undo_fn presuspend_undo;
    dm_postsuspend_fn postsuspend;
    dm_preresume_fn preresume;
    dm_resume_fn resume;
    dm_status_fn status;
    dm_message_fn message;
    dm_prepare_ioctl_fn prepare_ioctl;
    dm_busy_fn busy;
    dm_iterate_devices_fn iterate_devices;
    dm_io_hints_fn io_hints;
    dm_dax_direct_access_fn direct_access;
    dm_dax_copy_iter_fn dax_copy_from_iter;
    dm_dax_copy_iter_fn dax_copy_to_iter;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct target_type {
    uint64_t features;
    const char *name;
    struct module *module;
    unsigned int version[3];
    dm_ctr_fn ctr;
    dm_dtr_fn dtr;
    dm_map_fn map;
    dm_clone_and_map_request_fn clone_and_map_rq;
    dm_release_clone_request_fn release_clone_rq;
    dm_endio_fn end_io;
    dm_request_endio_fn rq_end_io;
    dm_presuspend_fn presuspend;
    dm_presuspend_undo_fn presuspend_undo;
    dm_postsuspend_fn postsuspend;
    dm_preresume_fn preresume;
    dm_resume_fn resume;
    dm_status_fn status;
    dm_message_fn message;
    dm_prepare_ioctl_fn prepare_ioctl;
    dm_report_zones_fn report_zones;
    dm_busy_fn busy;
    dm_iterate_devices_fn iterate_devices;
    dm_io_hints_fn io_hints;
    dm_dax_direct_access_fn direct_access;
    dm_dax_copy_iter_fn dax_copy_from_iter;
    dm_dax_copy_iter_fn dax_copy_to_iter;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct target_type {
    uint64_t features;
    const char *name;
    struct module *module;
    unsigned int version[3];
    dm_ctr_fn ctr;
    dm_dtr_fn dtr;
    dm_map_fn map;
    dm_clone_and_map_request_fn clone_and_map_rq;
    dm_release_clone_request_fn release_clone_rq;
    dm_endio_fn end_io;
    dm_request_endio_fn rq_end_io;
    dm_presuspend_fn presuspend;
    dm_presuspend_undo_fn presuspend_undo;
    dm_postsuspend_fn postsuspend;
    dm_preresume_fn preresume;
    dm_resume_fn resume;
    dm_status_fn status;
    dm_message_fn message;
    dm_prepare_ioctl_fn prepare_ioctl;
    dm_report_zones_fn report_zones;
    dm_busy_fn busy;
    dm_iterate_devices_fn iterate_devices;
    dm_io_hints_fn io_hints;
    dm_dax_direct_access_fn direct_access;
    dm_dax_copy_iter_fn dax_copy_from_iter;
    dm_dax_copy_iter_fn dax_copy_to_iter;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct target_type {
    uint64_t features;
    const char *name;
    struct module *module;
    unsigned int version[3];
    dm_ctr_fn ctr;
    dm_dtr_fn dtr;
    dm_map_fn map;
    dm_clone_and_map_request_fn clone_and_map_rq;
    dm_release_clone_request_fn release_clone_rq;
    dm_endio_fn end_io;
    dm_request_endio_fn rq_end_io;
    dm_presuspend_fn presuspend;
    dm_presuspend_undo_fn presuspend_undo;
    dm_postsuspend_fn postsuspend;
    dm_preresume_fn preresume;
    dm_resume_fn resume;
    dm_status_fn status;
    dm_message_fn message;
    dm_prepare_ioctl_fn prepare_ioctl;
    dm_report_zones_fn report_zones;
    dm_busy_fn busy;
    dm_iterate_devices_fn iterate_devices;
    dm_io_hints_fn io_hints;
    dm_dax_direct_access_fn direct_access;
    dm_dax_copy_iter_fn dax_copy_from_iter;
    dm_dax_copy_iter_fn dax_copy_to_iter;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct target_type {
    uint64_t features;
    const char *name;
    struct module *module;
    unsigned int version[3];
    dm_ctr_fn ctr;
    dm_dtr_fn dtr;
    dm_map_fn map;
    dm_clone_and_map_request_fn clone_and_map_rq;
    dm_release_clone_request_fn release_clone_rq;
    dm_endio_fn end_io;
    dm_request_endio_fn rq_end_io;
    dm_presuspend_fn presuspend;
    dm_presuspend_undo_fn presuspend_undo;
    dm_postsuspend_fn postsuspend;
    dm_preresume_fn preresume;
    dm_resume_fn resume;
    dm_status_fn status;
    dm_message_fn message;
    dm_prepare_ioctl_fn prepare_ioctl;
    dm_report_zones_fn report_zones;
    dm_busy_fn busy;
    dm_iterate_devices_fn iterate_devices;
    dm_io_hints_fn io_hints;
    dm_dax_direct_access_fn direct_access;
    dm_dax_copy_iter_fn dax_copy_from_iter;
    dm_dax_copy_iter_fn dax_copy_to_iter;
    dm_dax_zero_page_range_fn dax_zero_page_range;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct target_type {
    uint64_t features;
    const char *name;
    struct module *module;
    unsigned int version[3];
    dm_ctr_fn ctr;
    dm_dtr_fn dtr;
    dm_map_fn map;
    dm_clone_and_map_request_fn clone_and_map_rq;
    dm_release_clone_request_fn release_clone_rq;
    dm_endio_fn end_io;
    dm_request_endio_fn rq_end_io;
    dm_presuspend_fn presuspend;
    dm_presuspend_undo_fn presuspend_undo;
    dm_postsuspend_fn postsuspend;
    dm_preresume_fn preresume;
    dm_resume_fn resume;
    dm_status_fn status;
    dm_message_fn message;
    dm_prepare_ioctl_fn prepare_ioctl;
    dm_report_zones_fn report_zones;
    dm_busy_fn busy;
    dm_iterate_devices_fn iterate_devices;
    dm_io_hints_fn io_hints;
    dm_dax_direct_access_fn direct_access;
    dm_dax_copy_iter_fn dax_copy_from_iter;
    dm_dax_copy_iter_fn dax_copy_to_iter;
    dm_dax_zero_page_range_fn dax_zero_page_range;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct target_type {
    uint64_t features;
    const char *name;
    struct module *module;
    unsigned int version[3];
    dm_ctr_fn ctr;
    dm_dtr_fn dtr;
    dm_map_fn map;
    dm_clone_and_map_request_fn clone_and_map_rq;
    dm_release_clone_request_fn release_clone_rq;
    dm_endio_fn end_io;
    dm_request_endio_fn rq_end_io;
    dm_presuspend_fn presuspend;
    dm_presuspend_undo_fn presuspend_undo;
    dm_postsuspend_fn postsuspend;
    dm_preresume_fn preresume;
    dm_resume_fn resume;
    dm_status_fn status;
    dm_message_fn message;
    dm_prepare_ioctl_fn prepare_ioctl;
    dm_report_zones_fn report_zones;
    dm_busy_fn busy;
    dm_iterate_devices_fn iterate_devices;
    dm_io_hints_fn io_hints;
    dm_dax_direct_access_fn direct_access;
    dm_dax_copy_iter_fn dax_copy_from_iter;
    dm_dax_copy_iter_fn dax_copy_to_iter;
    dm_dax_zero_page_range_fn dax_zero_page_range;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct target_type {
    uint64_t features;
    const char *name;
    struct module *module;
    unsigned int version[3];
    dm_ctr_fn ctr;
    dm_dtr_fn dtr;
    dm_map_fn map;
    dm_clone_and_map_request_fn clone_and_map_rq;
    dm_release_clone_request_fn release_clone_rq;
    dm_endio_fn end_io;
    dm_request_endio_fn rq_end_io;
    dm_presuspend_fn presuspend;
    dm_presuspend_undo_fn presuspend_undo;
    dm_postsuspend_fn postsuspend;
    dm_preresume_fn preresume;
    dm_resume_fn resume;
    dm_status_fn status;
    dm_message_fn message;
    dm_prepare_ioctl_fn prepare_ioctl;
    dm_report_zones_fn report_zones;
    dm_busy_fn busy;
    dm_iterate_devices_fn iterate_devices;
    dm_io_hints_fn io_hints;
    dm_dax_direct_access_fn direct_access;
    dm_dax_copy_iter_fn dax_copy_from_iter;
    dm_dax_copy_iter_fn dax_copy_to_iter;
    dm_dax_zero_page_range_fn dax_zero_page_range;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct target_type {
    uint64_t features;
    const char *name;
    struct module *module;
    unsigned int version[3];
    dm_ctr_fn ctr;
    dm_dtr_fn dtr;
    dm_map_fn map;
    dm_clone_and_map_request_fn clone_and_map_rq;
    dm_release_clone_request_fn release_clone_rq;
    dm_endio_fn end_io;
    dm_request_endio_fn rq_end_io;
    dm_presuspend_fn presuspend;
    dm_presuspend_undo_fn presuspend_undo;
    dm_postsuspend_fn postsuspend;
    dm_preresume_fn preresume;
    dm_resume_fn resume;
    dm_status_fn status;
    dm_message_fn message;
    dm_prepare_ioctl_fn prepare_ioctl;
    dm_report_zones_fn report_zones;
    dm_busy_fn busy;
    dm_iterate_devices_fn iterate_devices;
    dm_io_hints_fn io_hints;
    dm_dax_direct_access_fn direct_access;
    dm_dax_zero_page_range_fn dax_zero_page_range;
    dm_dax_recovery_write_fn dax_recovery_write;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct target_type {
    uint64_t features;
    const char *name;
    struct module *module;
    unsigned int version[3];
    dm_ctr_fn ctr;
    dm_dtr_fn dtr;
    dm_map_fn map;
    dm_clone_and_map_request_fn clone_and_map_rq;
    dm_release_clone_request_fn release_clone_rq;
    dm_endio_fn end_io;
    dm_request_endio_fn rq_end_io;
    dm_presuspend_fn presuspend;
    dm_presuspend_undo_fn presuspend_undo;
    dm_postsuspend_fn postsuspend;
    dm_preresume_fn preresume;
    dm_resume_fn resume;
    dm_status_fn status;
    dm_message_fn message;
    dm_prepare_ioctl_fn prepare_ioctl;
    dm_report_zones_fn report_zones;
    dm_busy_fn busy;
    dm_iterate_devices_fn iterate_devices;
    dm_io_hints_fn io_hints;
    dm_dax_direct_access_fn direct_access;
    dm_dax_zero_page_range_fn dax_zero_page_range;
    dm_dax_recovery_write_fn dax_recovery_write;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct target_type {
    uint64_t features;
    const char *name;
    struct module *module;
    unsigned int version[3];
    dm_ctr_fn ctr;
    dm_dtr_fn dtr;
    dm_map_fn map;
    dm_clone_and_map_request_fn clone_and_map_rq;
    dm_release_clone_request_fn release_clone_rq;
    dm_endio_fn end_io;
    dm_request_endio_fn rq_end_io;
    dm_presuspend_fn presuspend;
    dm_presuspend_undo_fn presuspend_undo;
    dm_postsuspend_fn postsuspend;
    dm_preresume_fn preresume;
    dm_resume_fn resume;
    dm_status_fn status;
    dm_message_fn message;
    dm_prepare_ioctl_fn prepare_ioctl;
    dm_report_zones_fn report_zones;
    dm_busy_fn busy;
    dm_iterate_devices_fn iterate_devices;
    dm_io_hints_fn io_hints;
    dm_dax_direct_access_fn direct_access;
    dm_dax_zero_page_range_fn dax_zero_page_range;
    dm_dax_recovery_write_fn dax_recovery_write;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct target_type {
    uint64_t features;
    const char *name;
    struct module *module;
    unsigned int version[3];
    dm_ctr_fn ctr;
    dm_dtr_fn dtr;
    dm_map_fn map;
    dm_clone_and_map_request_fn clone_and_map_rq;
    dm_release_clone_request_fn release_clone_rq;
    dm_endio_fn end_io;
    dm_request_endio_fn rq_end_io;
    dm_presuspend_fn presuspend;
    dm_presuspend_undo_fn presuspend_undo;
    dm_postsuspend_fn postsuspend;
    dm_preresume_fn preresume;
    dm_resume_fn resume;
    dm_status_fn status;
    dm_message_fn message;
    dm_prepare_ioctl_fn prepare_ioctl;
    dm_report_zones_fn report_zones;
    dm_busy_fn busy;
    dm_iterate_devices_fn iterate_devices;
    dm_io_hints_fn io_hints;
    dm_dax_direct_access_fn direct_access;
    dm_dax_zero_page_range_fn dax_zero_page_range;
    dm_dax_recovery_write_fn dax_recovery_write;
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
struct target_type {
    uint64_t features;
    const char *name;
    struct module *module;
    unsigned int version[3];
    dm_ctr_fn ctr;
    dm_dtr_fn dtr;
    dm_map_fn map;
    dm_clone_and_map_request_fn clone_and_map_rq;
    dm_release_clone_request_fn release_clone_rq;
    dm_endio_fn end_io;
    dm_request_endio_fn rq_end_io;
    dm_presuspend_fn presuspend;
    dm_presuspend_undo_fn presuspend_undo;
    dm_postsuspend_fn postsuspend;
    dm_preresume_fn preresume;
    dm_resume_fn resume;
    dm_status_fn status;
    dm_message_fn message;
    dm_prepare_ioctl_fn prepare_ioctl;
    dm_report_zones_fn report_zones;
    dm_busy_fn busy;
    dm_iterate_devices_fn iterate_devices;
    dm_io_hints_fn io_hints;
    dm_dax_direct_access_fn direct_access;
    dm_dax_copy_iter_fn dax_copy_from_iter;
    dm_dax_copy_iter_fn dax_copy_to_iter;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct target_type {
    uint64_t features;
    const char *name;
    struct module *module;
    unsigned int version[3];
    dm_ctr_fn ctr;
    dm_dtr_fn dtr;
    dm_map_fn map;
    dm_clone_and_map_request_fn clone_and_map_rq;
    dm_release_clone_request_fn release_clone_rq;
    dm_endio_fn end_io;
    dm_request_endio_fn rq_end_io;
    dm_presuspend_fn presuspend;
    dm_presuspend_undo_fn presuspend_undo;
    dm_postsuspend_fn postsuspend;
    dm_preresume_fn preresume;
    dm_resume_fn resume;
    dm_status_fn status;
    dm_message_fn message;
    dm_prepare_ioctl_fn prepare_ioctl;
    dm_report_zones_fn report_zones;
    dm_busy_fn busy;
    dm_iterate_devices_fn iterate_devices;
    dm_io_hints_fn io_hints;
    dm_dax_direct_access_fn direct_access;
    dm_dax_copy_iter_fn dax_copy_from_iter;
    dm_dax_copy_iter_fn dax_copy_to_iter;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct target_type {
    uint64_t features;
    const char *name;
    struct module *module;
    unsigned int version[3];
    dm_ctr_fn ctr;
    dm_dtr_fn dtr;
    dm_map_fn map;
    dm_clone_and_map_request_fn clone_and_map_rq;
    dm_release_clone_request_fn release_clone_rq;
    dm_endio_fn end_io;
    dm_request_endio_fn rq_end_io;
    dm_presuspend_fn presuspend;
    dm_presuspend_undo_fn presuspend_undo;
    dm_postsuspend_fn postsuspend;
    dm_preresume_fn preresume;
    dm_resume_fn resume;
    dm_status_fn status;
    dm_message_fn message;
    dm_prepare_ioctl_fn prepare_ioctl;
    dm_report_zones_fn report_zones;
    dm_busy_fn busy;
    dm_iterate_devices_fn iterate_devices;
    dm_io_hints_fn io_hints;
    dm_dax_direct_access_fn direct_access;
    dm_dax_copy_iter_fn dax_copy_from_iter;
    dm_dax_copy_iter_fn dax_copy_to_iter;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct target_type {
    uint64_t features;
    const char *name;
    struct module *module;
    unsigned int version[3];
    dm_ctr_fn ctr;
    dm_dtr_fn dtr;
    dm_map_fn map;
    dm_clone_and_map_request_fn clone_and_map_rq;
    dm_release_clone_request_fn release_clone_rq;
    dm_endio_fn end_io;
    dm_request_endio_fn rq_end_io;
    dm_presuspend_fn presuspend;
    dm_presuspend_undo_fn presuspend_undo;
    dm_postsuspend_fn postsuspend;
    dm_preresume_fn preresume;
    dm_resume_fn resume;
    dm_status_fn status;
    dm_message_fn message;
    dm_prepare_ioctl_fn prepare_ioctl;
    dm_report_zones_fn report_zones;
    dm_busy_fn busy;
    dm_iterate_devices_fn iterate_devices;
    dm_io_hints_fn io_hints;
    dm_dax_direct_access_fn direct_access;
    dm_dax_copy_iter_fn dax_copy_from_iter;
    dm_dax_copy_iter_fn dax_copy_to_iter;
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
struct target_type {
    uint64_t features;
    const char *name;
    struct module *module;
    unsigned int version[3];
    dm_ctr_fn ctr;
    dm_dtr_fn dtr;
    dm_map_fn map;
    dm_clone_and_map_request_fn clone_and_map_rq;
    dm_release_clone_request_fn release_clone_rq;
    dm_endio_fn end_io;
    dm_request_endio_fn rq_end_io;
    dm_presuspend_fn presuspend;
    dm_presuspend_undo_fn presuspend_undo;
    dm_postsuspend_fn postsuspend;
    dm_preresume_fn preresume;
    dm_resume_fn resume;
    dm_status_fn status;
    dm_message_fn message;
    dm_prepare_ioctl_fn prepare_ioctl;
    dm_report_zones_fn report_zones;
    dm_busy_fn busy;
    dm_iterate_devices_fn iterate_devices;
    dm_io_hints_fn io_hints;
    dm_dax_direct_access_fn direct_access;
    dm_dax_copy_iter_fn dax_copy_from_iter;
    dm_dax_copy_iter_fn dax_copy_to_iter;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct target_type {
    uint64_t features;
    const char *name;
    struct module *module;
    unsigned int version[3];
    dm_ctr_fn ctr;
    dm_dtr_fn dtr;
    dm_map_fn map;
    dm_clone_and_map_request_fn clone_and_map_rq;
    dm_release_clone_request_fn release_clone_rq;
    dm_endio_fn end_io;
    dm_request_endio_fn rq_end_io;
    dm_presuspend_fn presuspend;
    dm_presuspend_undo_fn presuspend_undo;
    dm_postsuspend_fn postsuspend;
    dm_preresume_fn preresume;
    dm_resume_fn resume;
    dm_status_fn status;
    dm_message_fn message;
    dm_prepare_ioctl_fn prepare_ioctl;
    dm_report_zones_fn report_zones;
    dm_busy_fn busy;
    dm_iterate_devices_fn iterate_devices;
    dm_io_hints_fn io_hints;
    dm_dax_direct_access_fn direct_access;
    dm_dax_copy_iter_fn dax_copy_from_iter;
    dm_dax_copy_iter_fn dax_copy_to_iter;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct target_type {
    uint64_t features;
    const char *name;
    struct module *module;
    unsigned int version[3];
    dm_ctr_fn ctr;
    dm_dtr_fn dtr;
    dm_map_fn map;
    dm_clone_and_map_request_fn clone_and_map_rq;
    dm_release_clone_request_fn release_clone_rq;
    dm_endio_fn end_io;
    dm_request_endio_fn rq_end_io;
    dm_presuspend_fn presuspend;
    dm_presuspend_undo_fn presuspend_undo;
    dm_postsuspend_fn postsuspend;
    dm_preresume_fn preresume;
    dm_resume_fn resume;
    dm_status_fn status;
    dm_message_fn message;
    dm_prepare_ioctl_fn prepare_ioctl;
    dm_report_zones_fn report_zones;
    dm_busy_fn busy;
    dm_iterate_devices_fn iterate_devices;
    dm_io_hints_fn io_hints;
    dm_dax_direct_access_fn direct_access;
    dm_dax_copy_iter_fn dax_copy_from_iter;
    dm_dax_copy_iter_fn dax_copy_to_iter;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct target_type {
    uint64_t features;
    const char *name;
    struct module *module;
    unsigned int version[3];
    dm_ctr_fn ctr;
    dm_dtr_fn dtr;
    dm_map_fn map;
    dm_clone_and_map_request_fn clone_and_map_rq;
    dm_release_clone_request_fn release_clone_rq;
    dm_endio_fn end_io;
    dm_request_endio_fn rq_end_io;
    dm_presuspend_fn presuspend;
    dm_presuspend_undo_fn presuspend_undo;
    dm_postsuspend_fn postsuspend;
    dm_preresume_fn preresume;
    dm_resume_fn resume;
    dm_status_fn status;
    dm_message_fn message;
    dm_prepare_ioctl_fn prepare_ioctl;
    dm_report_zones_fn report_zones;
    dm_busy_fn busy;
    dm_iterate_devices_fn iterate_devices;
    dm_io_hints_fn io_hints;
    dm_dax_direct_access_fn direct_access;
    dm_dax_copy_iter_fn dax_copy_from_iter;
    dm_dax_copy_iter_fn dax_copy_to_iter;
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
<details>
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>dm_direct_access_fn direct_access</code>
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
<code>dm_dax_copy_from_iter_fn dax_copy_from_iter</code>
</li>
<li>
<b>Field added. </b>
<code>dm_dax_flush_fn dax_flush</code>
</li>
<li>
<b>Field removed. </b>
<code>dm_map_request_fn map_rq</code>
</li>
<li>
<b>Field type changed. </b>
<code>dm_direct_access_fn direct_access</code> ➡️ <code>dm_dax_direct_access_fn direct_access</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>dm_dax_flush_fn dax_flush</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>dm_dax_copy_iter_fn dax_copy_to_iter</code>
</li>
<li>
<b>Field type changed. </b>
<code>dm_dax_copy_from_iter_fn dax_copy_from_iter</code> ➡️ <code>dm_dax_copy_iter_fn dax_copy_from_iter</code>
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
<code>dm_report_zones_fn report_zones</code>
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
<code>dm_dax_zero_page_range_fn dax_zero_page_range</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>dm_dax_recovery_write_fn dax_recovery_write</code>
</li>
<li>
<b>Field removed. </b>
<code>dm_dax_copy_iter_fn dax_copy_from_iter</code>
</li>
<li>
<b>Field removed. </b>
<code>dm_dax_copy_iter_fn dax_copy_to_iter</code>
</li>
</ul>
</details>
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
