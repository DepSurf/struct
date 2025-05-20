# Struct: <code>hid_device</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
In <code>4.8</code>: Absent ⚠️
</li>
<li>
In <code>4.10</code>: Absent ⚠️
</li>
<li>
In <code>4.13</code>: Absent ⚠️
</li>
<li>
In <code>4.15</code>: Absent ⚠️
</li>
<li>
In <code>4.18</code>: Absent ⚠️
</li>
<li>
In <code>5.0</code>: Absent ⚠️
</li>
<li>
In <code>5.3</code>: Absent ⚠️
</li>
<li>
In <code>5.4</code>: Absent ⚠️
</li>
<li>
In <code>5.8</code>: Absent ⚠️
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
In <code>5.19</code>: Absent ⚠️
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct hid_device {
    __u8 *dev_rdesc;
    unsigned int dev_rsize;
    __u8 *rdesc;
    unsigned int rsize;
    struct hid_collection *collection;
    unsigned int collection_size;
    unsigned int maxcollection;
    unsigned int maxapplication;
    __u16 bus;
    __u16 group;
    __u32 vendor;
    __u32 product;
    __u32 version;
    enum hid_type type;
    unsigned int country;
    struct hid_report_enum report_enum[3];
    struct work_struct led_work;
    struct semaphore driver_input_lock;
    struct device dev;
    struct hid_driver *driver;
    void *devres_group_id;
    const struct hid_ll_driver *ll_driver;
    struct mutex ll_open_lock;
    unsigned int ll_open_count;
    struct power_supply *battery;
    __s32 battery_capacity;
    __s32 battery_min;
    __s32 battery_max;
    __s32 battery_report_type;
    __s32 battery_report_id;
    __s32 battery_charge_status;
    enum hid_battery_status battery_status;
    bool battery_avoid_query;
    ktime_t battery_ratelimit_time;
    long unsigned int status;
    unsigned int claimed;
    unsigned int quirks;
    unsigned int initial_quirks;
    bool io_started;
    struct list_head inputs;
    void *hiddev;
    void *hidraw;
    char name[128];
    char phys[64];
    char uniq[64];
    void *driver_data;
    int (*ff_init)(struct hid_device *);
    int (*hiddev_connect)(struct hid_device *, unsigned int);
    void (*hiddev_disconnect)(struct hid_device *);
    void (*hiddev_hid_event)(struct hid_device *, struct hid_field *, struct hid_usage *, __s32);
    void (*hiddev_report_event)(struct hid_device *, struct hid_report *);
    short unsigned int debug;
    struct dentry *debug_dir;
    struct dentry *debug_rdesc;
    struct dentry *debug_events;
    struct list_head debug_list;
    spinlock_t debug_list_lock;
    wait_queue_head_t debug_wait;
    unsigned int id;
    struct hid_bpf bpf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct hid_device {
    __u8 *dev_rdesc;
    unsigned int dev_rsize;
    __u8 *rdesc;
    unsigned int rsize;
    struct hid_collection *collection;
    unsigned int collection_size;
    unsigned int maxcollection;
    unsigned int maxapplication;
    __u16 bus;
    __u16 group;
    __u32 vendor;
    __u32 product;
    __u32 version;
    enum hid_type type;
    unsigned int country;
    struct hid_report_enum report_enum[3];
    struct work_struct led_work;
    struct semaphore driver_input_lock;
    struct device dev;
    struct hid_driver *driver;
    void *devres_group_id;
    const struct hid_ll_driver *ll_driver;
    struct mutex ll_open_lock;
    unsigned int ll_open_count;
    struct power_supply *battery;
    __s32 battery_capacity;
    __s32 battery_min;
    __s32 battery_max;
    __s32 battery_report_type;
    __s32 battery_report_id;
    __s32 battery_charge_status;
    enum hid_battery_status battery_status;
    bool battery_avoid_query;
    ktime_t battery_ratelimit_time;
    long unsigned int status;
    unsigned int claimed;
    unsigned int quirks;
    unsigned int initial_quirks;
    bool io_started;
    struct list_head inputs;
    void *hiddev;
    void *hidraw;
    char name[128];
    char phys[64];
    char uniq[64];
    void *driver_data;
    int (*ff_init)(struct hid_device *);
    int (*hiddev_connect)(struct hid_device *, unsigned int);
    void (*hiddev_disconnect)(struct hid_device *);
    void (*hiddev_hid_event)(struct hid_device *, struct hid_field *, struct hid_usage *, __s32);
    void (*hiddev_report_event)(struct hid_device *, struct hid_report *);
    short unsigned int debug;
    struct dentry *debug_dir;
    struct dentry *debug_rdesc;
    struct dentry *debug_events;
    struct list_head debug_list;
    spinlock_t debug_list_lock;
    wait_queue_head_t debug_wait;
    struct kref ref;
    unsigned int id;
    struct hid_bpf bpf;
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
In <code>arm64</code>: Absent ⚠️
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
</li>
<li>
In <code>riscv64</code>: Absent ⚠️
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
In <code>aws</code>: Absent ⚠️
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct kref ref</code>
</li>
</ul>
</details>
</li>
</ul>
