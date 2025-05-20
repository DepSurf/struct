# Struct: <code>rc_dev</code>

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
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rc_dev {
    struct device dev;
    bool managed_alloc;
    const struct attribute_group * sysfs_groups[5];
    const char *device_name;
    const char *input_phys;
    struct input_id input_id;
    const char *driver_name;
    const char *map_name;
    struct rc_map rc_map;
    struct mutex lock;
    unsigned int minor;
    struct ir_raw_event_ctrl *raw;
    struct input_dev *input_dev;
    enum rc_driver_type driver_type;
    bool idle;
    bool encode_wakeup;
    u64 allowed_protocols;
    u64 enabled_protocols;
    u64 allowed_wakeup_protocols;
    enum rc_proto wakeup_protocol;
    struct rc_scancode_filter scancode_filter;
    struct rc_scancode_filter scancode_wakeup_filter;
    u32 scancode_mask;
    u32 users;
    void *priv;
    spinlock_t keylock;
    bool keypressed;
    long unsigned int keyup_jiffies;
    struct timer_list timer_keyup;
    struct timer_list timer_repeat;
    u32 last_keycode;
    enum rc_proto last_protocol;
    u32 last_scancode;
    u8 last_toggle;
    u32 timeout;
    u32 min_timeout;
    u32 max_timeout;
    u32 rx_resolution;
    u32 tx_resolution;
    struct device lirc_dev;
    struct cdev lirc_cdev;
    ktime_t gap_start;
    u64 gap_duration;
    bool gap;
    spinlock_t lirc_fh_lock;
    struct list_head lirc_fh;
    bool registered;
    int (*change_protocol)(struct rc_dev *, u64 *);
    int (*open)(struct rc_dev *);
    void (*close)(struct rc_dev *);
    int (*s_tx_mask)(struct rc_dev *, u32);
    int (*s_tx_carrier)(struct rc_dev *, u32);
    int (*s_tx_duty_cycle)(struct rc_dev *, u32);
    int (*s_rx_carrier_range)(struct rc_dev *, u32, u32);
    int (*tx_ir)(struct rc_dev *, unsigned int *, unsigned int);
    void (*s_idle)(struct rc_dev *, bool);
    int (*s_learning_mode)(struct rc_dev *, int);
    int (*s_carrier_report)(struct rc_dev *, int);
    int (*s_filter)(struct rc_dev *, struct rc_scancode_filter *);
    int (*s_wakeup_filter)(struct rc_dev *, struct rc_scancode_filter *);
    int (*s_timeout)(struct rc_dev *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rc_dev {
    struct device dev;
    bool managed_alloc;
    const struct attribute_group * sysfs_groups[5];
    const char *device_name;
    const char *input_phys;
    struct input_id input_id;
    const char *driver_name;
    const char *map_name;
    struct rc_map rc_map;
    struct mutex lock;
    unsigned int minor;
    struct ir_raw_event_ctrl *raw;
    struct input_dev *input_dev;
    enum rc_driver_type driver_type;
    bool idle;
    bool encode_wakeup;
    u64 allowed_protocols;
    u64 enabled_protocols;
    u64 allowed_wakeup_protocols;
    enum rc_proto wakeup_protocol;
    struct rc_scancode_filter scancode_filter;
    struct rc_scancode_filter scancode_wakeup_filter;
    u32 scancode_mask;
    u32 users;
    void *priv;
    spinlock_t keylock;
    bool keypressed;
    long unsigned int keyup_jiffies;
    struct timer_list timer_keyup;
    struct timer_list timer_repeat;
    u32 last_keycode;
    enum rc_proto last_protocol;
    u32 last_scancode;
    u8 last_toggle;
    u32 timeout;
    u32 min_timeout;
    u32 max_timeout;
    u32 rx_resolution;
    u32 tx_resolution;
    struct device lirc_dev;
    struct cdev lirc_cdev;
    ktime_t gap_start;
    u64 gap_duration;
    bool gap;
    spinlock_t lirc_fh_lock;
    struct list_head lirc_fh;
    bool registered;
    int (*change_protocol)(struct rc_dev *, u64 *);
    int (*open)(struct rc_dev *);
    void (*close)(struct rc_dev *);
    int (*s_tx_mask)(struct rc_dev *, u32);
    int (*s_tx_carrier)(struct rc_dev *, u32);
    int (*s_tx_duty_cycle)(struct rc_dev *, u32);
    int (*s_rx_carrier_range)(struct rc_dev *, u32, u32);
    int (*tx_ir)(struct rc_dev *, unsigned int *, unsigned int);
    void (*s_idle)(struct rc_dev *, bool);
    int (*s_learning_mode)(struct rc_dev *, int);
    int (*s_carrier_report)(struct rc_dev *, int);
    int (*s_filter)(struct rc_dev *, struct rc_scancode_filter *);
    int (*s_wakeup_filter)(struct rc_dev *, struct rc_scancode_filter *);
    int (*s_timeout)(struct rc_dev *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rc_dev {
    struct device dev;
    bool managed_alloc;
    const struct attribute_group * sysfs_groups[5];
    const char *device_name;
    const char *input_phys;
    struct input_id input_id;
    const char *driver_name;
    const char *map_name;
    struct rc_map rc_map;
    struct mutex lock;
    unsigned int minor;
    struct ir_raw_event_ctrl *raw;
    struct input_dev *input_dev;
    enum rc_driver_type driver_type;
    bool idle;
    bool encode_wakeup;
    u64 allowed_protocols;
    u64 enabled_protocols;
    u64 allowed_wakeup_protocols;
    enum rc_proto wakeup_protocol;
    struct rc_scancode_filter scancode_filter;
    struct rc_scancode_filter scancode_wakeup_filter;
    u32 scancode_mask;
    u32 users;
    void *priv;
    spinlock_t keylock;
    bool keypressed;
    long unsigned int keyup_jiffies;
    struct timer_list timer_keyup;
    struct timer_list timer_repeat;
    u32 last_keycode;
    enum rc_proto last_protocol;
    u32 last_scancode;
    u8 last_toggle;
    u32 timeout;
    u32 min_timeout;
    u32 max_timeout;
    u32 rx_resolution;
    u32 tx_resolution;
    struct device lirc_dev;
    struct cdev lirc_cdev;
    ktime_t gap_start;
    u64 gap_duration;
    bool gap;
    spinlock_t lirc_fh_lock;
    struct list_head lirc_fh;
    bool registered;
    int (*change_protocol)(struct rc_dev *, u64 *);
    int (*open)(struct rc_dev *);
    void (*close)(struct rc_dev *);
    int (*s_tx_mask)(struct rc_dev *, u32);
    int (*s_tx_carrier)(struct rc_dev *, u32);
    int (*s_tx_duty_cycle)(struct rc_dev *, u32);
    int (*s_rx_carrier_range)(struct rc_dev *, u32, u32);
    int (*tx_ir)(struct rc_dev *, unsigned int *, unsigned int);
    void (*s_idle)(struct rc_dev *, bool);
    int (*s_learning_mode)(struct rc_dev *, int);
    int (*s_carrier_report)(struct rc_dev *, int);
    int (*s_filter)(struct rc_dev *, struct rc_scancode_filter *);
    int (*s_wakeup_filter)(struct rc_dev *, struct rc_scancode_filter *);
    int (*s_timeout)(struct rc_dev *, unsigned int);
};
```
</details>
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
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct rc_dev {
    struct device dev;
    bool managed_alloc;
    const struct attribute_group * sysfs_groups[5];
    const char *device_name;
    const char *input_phys;
    struct input_id input_id;
    const char *driver_name;
    const char *map_name;
    struct rc_map rc_map;
    struct mutex lock;
    unsigned int minor;
    struct ir_raw_event_ctrl *raw;
    struct input_dev *input_dev;
    enum rc_driver_type driver_type;
    bool idle;
    bool encode_wakeup;
    u64 allowed_protocols;
    u64 enabled_protocols;
    u64 allowed_wakeup_protocols;
    enum rc_proto wakeup_protocol;
    struct rc_scancode_filter scancode_filter;
    struct rc_scancode_filter scancode_wakeup_filter;
    u32 scancode_mask;
    u32 users;
    void *priv;
    spinlock_t keylock;
    bool keypressed;
    long unsigned int keyup_jiffies;
    struct timer_list timer_keyup;
    struct timer_list timer_repeat;
    u32 last_keycode;
    enum rc_proto last_protocol;
    u32 last_scancode;
    u8 last_toggle;
    u32 timeout;
    u32 min_timeout;
    u32 max_timeout;
    u32 rx_resolution;
    u32 tx_resolution;
    struct device lirc_dev;
    struct cdev lirc_cdev;
    ktime_t gap_start;
    u64 gap_duration;
    bool gap;
    spinlock_t lirc_fh_lock;
    struct list_head lirc_fh;
    bool registered;
    int (*change_protocol)(struct rc_dev *, u64 *);
    int (*open)(struct rc_dev *);
    void (*close)(struct rc_dev *);
    int (*s_tx_mask)(struct rc_dev *, u32);
    int (*s_tx_carrier)(struct rc_dev *, u32);
    int (*s_tx_duty_cycle)(struct rc_dev *, u32);
    int (*s_rx_carrier_range)(struct rc_dev *, u32, u32);
    int (*tx_ir)(struct rc_dev *, unsigned int *, unsigned int);
    void (*s_idle)(struct rc_dev *, bool);
    int (*s_learning_mode)(struct rc_dev *, int);
    int (*s_carrier_report)(struct rc_dev *, int);
    int (*s_filter)(struct rc_dev *, struct rc_scancode_filter *);
    int (*s_wakeup_filter)(struct rc_dev *, struct rc_scancode_filter *);
    int (*s_timeout)(struct rc_dev *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rc_dev {
    struct device dev;
    bool managed_alloc;
    const struct attribute_group * sysfs_groups[5];
    const char *device_name;
    const char *input_phys;
    struct input_id input_id;
    const char *driver_name;
    const char *map_name;
    struct rc_map rc_map;
    struct mutex lock;
    unsigned int minor;
    struct ir_raw_event_ctrl *raw;
    struct input_dev *input_dev;
    enum rc_driver_type driver_type;
    bool idle;
    bool encode_wakeup;
    u64 allowed_protocols;
    u64 enabled_protocols;
    u64 allowed_wakeup_protocols;
    enum rc_proto wakeup_protocol;
    struct rc_scancode_filter scancode_filter;
    struct rc_scancode_filter scancode_wakeup_filter;
    u32 scancode_mask;
    u32 users;
    void *priv;
    spinlock_t keylock;
    bool keypressed;
    long unsigned int keyup_jiffies;
    struct timer_list timer_keyup;
    struct timer_list timer_repeat;
    u32 last_keycode;
    enum rc_proto last_protocol;
    u32 last_scancode;
    u8 last_toggle;
    u32 timeout;
    u32 min_timeout;
    u32 max_timeout;
    u32 rx_resolution;
    u32 tx_resolution;
    struct device lirc_dev;
    struct cdev lirc_cdev;
    ktime_t gap_start;
    u64 gap_duration;
    bool gap;
    spinlock_t lirc_fh_lock;
    struct list_head lirc_fh;
    bool registered;
    int (*change_protocol)(struct rc_dev *, u64 *);
    int (*open)(struct rc_dev *);
    void (*close)(struct rc_dev *);
    int (*s_tx_mask)(struct rc_dev *, u32);
    int (*s_tx_carrier)(struct rc_dev *, u32);
    int (*s_tx_duty_cycle)(struct rc_dev *, u32);
    int (*s_rx_carrier_range)(struct rc_dev *, u32, u32);
    int (*tx_ir)(struct rc_dev *, unsigned int *, unsigned int);
    void (*s_idle)(struct rc_dev *, bool);
    int (*s_learning_mode)(struct rc_dev *, int);
    int (*s_carrier_report)(struct rc_dev *, int);
    int (*s_filter)(struct rc_dev *, struct rc_scancode_filter *);
    int (*s_wakeup_filter)(struct rc_dev *, struct rc_scancode_filter *);
    int (*s_timeout)(struct rc_dev *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rc_dev {
    struct device dev;
    bool managed_alloc;
    const struct attribute_group * sysfs_groups[5];
    const char *device_name;
    const char *input_phys;
    struct input_id input_id;
    const char *driver_name;
    const char *map_name;
    struct rc_map rc_map;
    struct mutex lock;
    unsigned int minor;
    struct ir_raw_event_ctrl *raw;
    struct input_dev *input_dev;
    enum rc_driver_type driver_type;
    bool idle;
    bool encode_wakeup;
    u64 allowed_protocols;
    u64 enabled_protocols;
    u64 allowed_wakeup_protocols;
    enum rc_proto wakeup_protocol;
    struct rc_scancode_filter scancode_filter;
    struct rc_scancode_filter scancode_wakeup_filter;
    u32 scancode_mask;
    u32 users;
    void *priv;
    spinlock_t keylock;
    bool keypressed;
    long unsigned int keyup_jiffies;
    struct timer_list timer_keyup;
    struct timer_list timer_repeat;
    u32 last_keycode;
    enum rc_proto last_protocol;
    u32 last_scancode;
    u8 last_toggle;
    u32 timeout;
    u32 min_timeout;
    u32 max_timeout;
    u32 rx_resolution;
    u32 tx_resolution;
    struct device lirc_dev;
    struct cdev lirc_cdev;
    ktime_t gap_start;
    u64 gap_duration;
    bool gap;
    spinlock_t lirc_fh_lock;
    struct list_head lirc_fh;
    bool registered;
    int (*change_protocol)(struct rc_dev *, u64 *);
    int (*open)(struct rc_dev *);
    void (*close)(struct rc_dev *);
    int (*s_tx_mask)(struct rc_dev *, u32);
    int (*s_tx_carrier)(struct rc_dev *, u32);
    int (*s_tx_duty_cycle)(struct rc_dev *, u32);
    int (*s_rx_carrier_range)(struct rc_dev *, u32, u32);
    int (*tx_ir)(struct rc_dev *, unsigned int *, unsigned int);
    void (*s_idle)(struct rc_dev *, bool);
    int (*s_learning_mode)(struct rc_dev *, int);
    int (*s_carrier_report)(struct rc_dev *, int);
    int (*s_filter)(struct rc_dev *, struct rc_scancode_filter *);
    int (*s_wakeup_filter)(struct rc_dev *, struct rc_scancode_filter *);
    int (*s_timeout)(struct rc_dev *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct rc_dev {
    struct device dev;
    bool managed_alloc;
    const struct attribute_group * sysfs_groups[5];
    const char *device_name;
    const char *input_phys;
    struct input_id input_id;
    const char *driver_name;
    const char *map_name;
    struct rc_map rc_map;
    struct mutex lock;
    unsigned int minor;
    struct ir_raw_event_ctrl *raw;
    struct input_dev *input_dev;
    enum rc_driver_type driver_type;
    bool idle;
    bool encode_wakeup;
    u64 allowed_protocols;
    u64 enabled_protocols;
    u64 allowed_wakeup_protocols;
    enum rc_proto wakeup_protocol;
    struct rc_scancode_filter scancode_filter;
    struct rc_scancode_filter scancode_wakeup_filter;
    u32 scancode_mask;
    u32 users;
    void *priv;
    spinlock_t keylock;
    bool keypressed;
    long unsigned int keyup_jiffies;
    struct timer_list timer_keyup;
    struct timer_list timer_repeat;
    u32 last_keycode;
    enum rc_proto last_protocol;
    u32 last_scancode;
    u8 last_toggle;
    u32 timeout;
    u32 min_timeout;
    u32 max_timeout;
    u32 rx_resolution;
    u32 tx_resolution;
    struct device lirc_dev;
    struct cdev lirc_cdev;
    ktime_t gap_start;
    u64 gap_duration;
    bool gap;
    spinlock_t lirc_fh_lock;
    struct list_head lirc_fh;
    bool registered;
    int (*change_protocol)(struct rc_dev *, u64 *);
    int (*open)(struct rc_dev *);
    void (*close)(struct rc_dev *);
    int (*s_tx_mask)(struct rc_dev *, u32);
    int (*s_tx_carrier)(struct rc_dev *, u32);
    int (*s_tx_duty_cycle)(struct rc_dev *, u32);
    int (*s_rx_carrier_range)(struct rc_dev *, u32, u32);
    int (*tx_ir)(struct rc_dev *, unsigned int *, unsigned int);
    void (*s_idle)(struct rc_dev *, bool);
    int (*s_learning_mode)(struct rc_dev *, int);
    int (*s_carrier_report)(struct rc_dev *, int);
    int (*s_filter)(struct rc_dev *, struct rc_scancode_filter *);
    int (*s_wakeup_filter)(struct rc_dev *, struct rc_scancode_filter *);
    int (*s_timeout)(struct rc_dev *, unsigned int);
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
struct rc_dev {
    struct device dev;
    bool managed_alloc;
    const struct attribute_group * sysfs_groups[5];
    const char *device_name;
    const char *input_phys;
    struct input_id input_id;
    const char *driver_name;
    const char *map_name;
    struct rc_map rc_map;
    struct mutex lock;
    unsigned int minor;
    struct ir_raw_event_ctrl *raw;
    struct input_dev *input_dev;
    enum rc_driver_type driver_type;
    bool idle;
    bool encode_wakeup;
    u64 allowed_protocols;
    u64 enabled_protocols;
    u64 allowed_wakeup_protocols;
    enum rc_proto wakeup_protocol;
    struct rc_scancode_filter scancode_filter;
    struct rc_scancode_filter scancode_wakeup_filter;
    u32 scancode_mask;
    u32 users;
    void *priv;
    spinlock_t keylock;
    bool keypressed;
    long unsigned int keyup_jiffies;
    struct timer_list timer_keyup;
    struct timer_list timer_repeat;
    u32 last_keycode;
    enum rc_proto last_protocol;
    u32 last_scancode;
    u8 last_toggle;
    u32 timeout;
    u32 min_timeout;
    u32 max_timeout;
    u32 rx_resolution;
    u32 tx_resolution;
    bool registered;
    int (*change_protocol)(struct rc_dev *, u64 *);
    int (*open)(struct rc_dev *);
    void (*close)(struct rc_dev *);
    int (*s_tx_mask)(struct rc_dev *, u32);
    int (*s_tx_carrier)(struct rc_dev *, u32);
    int (*s_tx_duty_cycle)(struct rc_dev *, u32);
    int (*s_rx_carrier_range)(struct rc_dev *, u32, u32);
    int (*tx_ir)(struct rc_dev *, unsigned int *, unsigned int);
    void (*s_idle)(struct rc_dev *, bool);
    int (*s_learning_mode)(struct rc_dev *, int);
    int (*s_carrier_report)(struct rc_dev *, int);
    int (*s_filter)(struct rc_dev *, struct rc_scancode_filter *);
    int (*s_wakeup_filter)(struct rc_dev *, struct rc_scancode_filter *);
    int (*s_timeout)(struct rc_dev *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rc_dev {
    struct device dev;
    bool managed_alloc;
    const struct attribute_group * sysfs_groups[5];
    const char *device_name;
    const char *input_phys;
    struct input_id input_id;
    const char *driver_name;
    const char *map_name;
    struct rc_map rc_map;
    struct mutex lock;
    unsigned int minor;
    struct ir_raw_event_ctrl *raw;
    struct input_dev *input_dev;
    enum rc_driver_type driver_type;
    bool idle;
    bool encode_wakeup;
    u64 allowed_protocols;
    u64 enabled_protocols;
    u64 allowed_wakeup_protocols;
    enum rc_proto wakeup_protocol;
    struct rc_scancode_filter scancode_filter;
    struct rc_scancode_filter scancode_wakeup_filter;
    u32 scancode_mask;
    u32 users;
    void *priv;
    spinlock_t keylock;
    bool keypressed;
    long unsigned int keyup_jiffies;
    struct timer_list timer_keyup;
    struct timer_list timer_repeat;
    u32 last_keycode;
    enum rc_proto last_protocol;
    u32 last_scancode;
    u8 last_toggle;
    u32 timeout;
    u32 min_timeout;
    u32 max_timeout;
    u32 rx_resolution;
    u32 tx_resolution;
    struct device lirc_dev;
    struct cdev lirc_cdev;
    ktime_t gap_start;
    u64 gap_duration;
    bool gap;
    spinlock_t lirc_fh_lock;
    struct list_head lirc_fh;
    bool registered;
    int (*change_protocol)(struct rc_dev *, u64 *);
    int (*open)(struct rc_dev *);
    void (*close)(struct rc_dev *);
    int (*s_tx_mask)(struct rc_dev *, u32);
    int (*s_tx_carrier)(struct rc_dev *, u32);
    int (*s_tx_duty_cycle)(struct rc_dev *, u32);
    int (*s_rx_carrier_range)(struct rc_dev *, u32, u32);
    int (*tx_ir)(struct rc_dev *, unsigned int *, unsigned int);
    void (*s_idle)(struct rc_dev *, bool);
    int (*s_learning_mode)(struct rc_dev *, int);
    int (*s_carrier_report)(struct rc_dev *, int);
    int (*s_filter)(struct rc_dev *, struct rc_scancode_filter *);
    int (*s_wakeup_filter)(struct rc_dev *, struct rc_scancode_filter *);
    int (*s_timeout)(struct rc_dev *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rc_dev {
    struct device dev;
    bool managed_alloc;
    const struct attribute_group * sysfs_groups[5];
    const char *device_name;
    const char *input_phys;
    struct input_id input_id;
    const char *driver_name;
    const char *map_name;
    struct rc_map rc_map;
    struct mutex lock;
    unsigned int minor;
    struct ir_raw_event_ctrl *raw;
    struct input_dev *input_dev;
    enum rc_driver_type driver_type;
    bool idle;
    bool encode_wakeup;
    u64 allowed_protocols;
    u64 enabled_protocols;
    u64 allowed_wakeup_protocols;
    enum rc_proto wakeup_protocol;
    struct rc_scancode_filter scancode_filter;
    struct rc_scancode_filter scancode_wakeup_filter;
    u32 scancode_mask;
    u32 users;
    void *priv;
    spinlock_t keylock;
    bool keypressed;
    long unsigned int keyup_jiffies;
    struct timer_list timer_keyup;
    struct timer_list timer_repeat;
    u32 last_keycode;
    enum rc_proto last_protocol;
    u32 last_scancode;
    u8 last_toggle;
    u32 timeout;
    u32 min_timeout;
    u32 max_timeout;
    u32 rx_resolution;
    u32 tx_resolution;
    struct device lirc_dev;
    struct cdev lirc_cdev;
    ktime_t gap_start;
    u64 gap_duration;
    bool gap;
    spinlock_t lirc_fh_lock;
    struct list_head lirc_fh;
    bool registered;
    int (*change_protocol)(struct rc_dev *, u64 *);
    int (*open)(struct rc_dev *);
    void (*close)(struct rc_dev *);
    int (*s_tx_mask)(struct rc_dev *, u32);
    int (*s_tx_carrier)(struct rc_dev *, u32);
    int (*s_tx_duty_cycle)(struct rc_dev *, u32);
    int (*s_rx_carrier_range)(struct rc_dev *, u32, u32);
    int (*tx_ir)(struct rc_dev *, unsigned int *, unsigned int);
    void (*s_idle)(struct rc_dev *, bool);
    int (*s_learning_mode)(struct rc_dev *, int);
    int (*s_carrier_report)(struct rc_dev *, int);
    int (*s_filter)(struct rc_dev *, struct rc_scancode_filter *);
    int (*s_wakeup_filter)(struct rc_dev *, struct rc_scancode_filter *);
    int (*s_timeout)(struct rc_dev *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rc_dev {
    struct device dev;
    bool managed_alloc;
    const struct attribute_group * sysfs_groups[5];
    const char *device_name;
    const char *input_phys;
    struct input_id input_id;
    const char *driver_name;
    const char *map_name;
    struct rc_map rc_map;
    struct mutex lock;
    unsigned int minor;
    struct ir_raw_event_ctrl *raw;
    struct input_dev *input_dev;
    enum rc_driver_type driver_type;
    bool idle;
    bool encode_wakeup;
    u64 allowed_protocols;
    u64 enabled_protocols;
    u64 allowed_wakeup_protocols;
    enum rc_proto wakeup_protocol;
    struct rc_scancode_filter scancode_filter;
    struct rc_scancode_filter scancode_wakeup_filter;
    u32 scancode_mask;
    u32 users;
    void *priv;
    spinlock_t keylock;
    bool keypressed;
    long unsigned int keyup_jiffies;
    struct timer_list timer_keyup;
    struct timer_list timer_repeat;
    u32 last_keycode;
    enum rc_proto last_protocol;
    u32 last_scancode;
    u8 last_toggle;
    u32 timeout;
    u32 min_timeout;
    u32 max_timeout;
    u32 rx_resolution;
    u32 tx_resolution;
    struct device lirc_dev;
    struct cdev lirc_cdev;
    ktime_t gap_start;
    u64 gap_duration;
    bool gap;
    spinlock_t lirc_fh_lock;
    struct list_head lirc_fh;
    bool registered;
    int (*change_protocol)(struct rc_dev *, u64 *);
    int (*open)(struct rc_dev *);
    void (*close)(struct rc_dev *);
    int (*s_tx_mask)(struct rc_dev *, u32);
    int (*s_tx_carrier)(struct rc_dev *, u32);
    int (*s_tx_duty_cycle)(struct rc_dev *, u32);
    int (*s_rx_carrier_range)(struct rc_dev *, u32, u32);
    int (*tx_ir)(struct rc_dev *, unsigned int *, unsigned int);
    void (*s_idle)(struct rc_dev *, bool);
    int (*s_learning_mode)(struct rc_dev *, int);
    int (*s_carrier_report)(struct rc_dev *, int);
    int (*s_filter)(struct rc_dev *, struct rc_scancode_filter *);
    int (*s_wakeup_filter)(struct rc_dev *, struct rc_scancode_filter *);
    int (*s_timeout)(struct rc_dev *, unsigned int);
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
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
<details>
<summary>Changed between <code>generic</code> and <code>aws</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct device lirc_dev</code>
</li>
<li>
<b>Field removed. </b>
<code>struct cdev lirc_cdev</code>
</li>
<li>
<b>Field removed. </b>
<code>ktime_t gap_start</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 gap_duration</code>
</li>
<li>
<b>Field removed. </b>
<code>bool gap</code>
</li>
<li>
<b>Field removed. </b>
<code>spinlock_t lirc_fh_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head lirc_fh</code>
</li>
</ul>
</details>
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
