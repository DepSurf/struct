# Struct: <code>led_classdev</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct led_classdev {
    const char *name;
    enum led_brightness brightness;
    enum led_brightness max_brightness;
    int flags;
    void (*brightness_set)(struct led_classdev *, enum led_brightness);
    int (*brightness_set_sync)(struct led_classdev *, enum led_brightness);
    enum led_brightness (*brightness_get)(struct led_classdev *);
    int (*blink_set)(struct led_classdev *, long unsigned int *, long unsigned int *);
    struct device *dev;
    const struct attribute_group **groups;
    struct list_head node;
    const char *default_trigger;
    long unsigned int blink_delay_on;
    long unsigned int blink_delay_off;
    struct timer_list blink_timer;
    int blink_brightness;
    void (*flash_resume)(struct led_classdev *);
    struct work_struct set_brightness_work;
    int delayed_set_value;
    struct rw_semaphore trigger_lock;
    struct led_trigger *trigger;
    struct list_head trig_list;
    void *trigger_data;
    bool activated;
    struct mutex led_access;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct led_classdev {
    const char *name;
    enum led_brightness brightness;
    enum led_brightness max_brightness;
    int flags;
    void (*brightness_set)(struct led_classdev *, enum led_brightness);
    int (*brightness_set_blocking)(struct led_classdev *, enum led_brightness);
    enum led_brightness (*brightness_get)(struct led_classdev *);
    int (*blink_set)(struct led_classdev *, long unsigned int *, long unsigned int *);
    struct device *dev;
    const struct attribute_group **groups;
    struct list_head node;
    const char *default_trigger;
    long unsigned int blink_delay_on;
    long unsigned int blink_delay_off;
    struct timer_list blink_timer;
    int blink_brightness;
    void (*flash_resume)(struct led_classdev *);
    struct work_struct set_brightness_work;
    int delayed_set_value;
    struct rw_semaphore trigger_lock;
    struct led_trigger *trigger;
    struct list_head trig_list;
    void *trigger_data;
    bool activated;
    struct mutex led_access;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct led_classdev {
    const char *name;
    enum led_brightness brightness;
    enum led_brightness max_brightness;
    int flags;
    long unsigned int work_flags;
    void (*brightness_set)(struct led_classdev *, enum led_brightness);
    int (*brightness_set_blocking)(struct led_classdev *, enum led_brightness);
    enum led_brightness (*brightness_get)(struct led_classdev *);
    int (*blink_set)(struct led_classdev *, long unsigned int *, long unsigned int *);
    struct device *dev;
    const struct attribute_group **groups;
    struct list_head node;
    const char *default_trigger;
    long unsigned int blink_delay_on;
    long unsigned int blink_delay_off;
    struct timer_list blink_timer;
    int blink_brightness;
    int new_blink_brightness;
    void (*flash_resume)(struct led_classdev *);
    struct work_struct set_brightness_work;
    int delayed_set_value;
    struct rw_semaphore trigger_lock;
    struct led_trigger *trigger;
    struct list_head trig_list;
    void *trigger_data;
    bool activated;
    struct mutex led_access;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct led_classdev {
    const char *name;
    enum led_brightness brightness;
    enum led_brightness max_brightness;
    int flags;
    long unsigned int work_flags;
    void (*brightness_set)(struct led_classdev *, enum led_brightness);
    int (*brightness_set_blocking)(struct led_classdev *, enum led_brightness);
    enum led_brightness (*brightness_get)(struct led_classdev *);
    int (*blink_set)(struct led_classdev *, long unsigned int *, long unsigned int *);
    struct device *dev;
    const struct attribute_group **groups;
    struct list_head node;
    const char *default_trigger;
    long unsigned int blink_delay_on;
    long unsigned int blink_delay_off;
    struct timer_list blink_timer;
    int blink_brightness;
    int new_blink_brightness;
    void (*flash_resume)(struct led_classdev *);
    struct work_struct set_brightness_work;
    int delayed_set_value;
    struct rw_semaphore trigger_lock;
    struct led_trigger *trigger;
    struct list_head trig_list;
    void *trigger_data;
    bool activated;
    int brightness_hw_changed;
    struct kernfs_node *brightness_hw_changed_kn;
    struct mutex led_access;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct led_classdev {
    const char *name;
    enum led_brightness brightness;
    enum led_brightness max_brightness;
    int flags;
    long unsigned int work_flags;
    void (*brightness_set)(struct led_classdev *, enum led_brightness);
    int (*brightness_set_blocking)(struct led_classdev *, enum led_brightness);
    enum led_brightness (*brightness_get)(struct led_classdev *);
    int (*blink_set)(struct led_classdev *, long unsigned int *, long unsigned int *);
    struct device *dev;
    const struct attribute_group **groups;
    struct list_head node;
    const char *default_trigger;
    long unsigned int blink_delay_on;
    long unsigned int blink_delay_off;
    struct timer_list blink_timer;
    int blink_brightness;
    int new_blink_brightness;
    void (*flash_resume)(struct led_classdev *);
    struct work_struct set_brightness_work;
    int delayed_set_value;
    struct rw_semaphore trigger_lock;
    struct led_trigger *trigger;
    struct list_head trig_list;
    void *trigger_data;
    bool activated;
    int brightness_hw_changed;
    struct kernfs_node *brightness_hw_changed_kn;
    struct mutex led_access;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct led_classdev {
    const char *name;
    enum led_brightness brightness;
    enum led_brightness max_brightness;
    int flags;
    long unsigned int work_flags;
    void (*brightness_set)(struct led_classdev *, enum led_brightness);
    int (*brightness_set_blocking)(struct led_classdev *, enum led_brightness);
    enum led_brightness (*brightness_get)(struct led_classdev *);
    int (*blink_set)(struct led_classdev *, long unsigned int *, long unsigned int *);
    struct device *dev;
    const struct attribute_group **groups;
    struct list_head node;
    const char *default_trigger;
    long unsigned int blink_delay_on;
    long unsigned int blink_delay_off;
    struct timer_list blink_timer;
    int blink_brightness;
    int new_blink_brightness;
    void (*flash_resume)(struct led_classdev *);
    struct work_struct set_brightness_work;
    int delayed_set_value;
    struct rw_semaphore trigger_lock;
    struct led_trigger *trigger;
    struct list_head trig_list;
    void *trigger_data;
    bool activated;
    int brightness_hw_changed;
    struct kernfs_node *brightness_hw_changed_kn;
    struct mutex led_access;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct led_classdev {
    const char *name;
    enum led_brightness brightness;
    enum led_brightness max_brightness;
    int flags;
    long unsigned int work_flags;
    void (*brightness_set)(struct led_classdev *, enum led_brightness);
    int (*brightness_set_blocking)(struct led_classdev *, enum led_brightness);
    enum led_brightness (*brightness_get)(struct led_classdev *);
    int (*blink_set)(struct led_classdev *, long unsigned int *, long unsigned int *);
    int (*pattern_set)(struct led_classdev *, struct led_pattern *, u32, int);
    int (*pattern_clear)(struct led_classdev *);
    struct device *dev;
    const struct attribute_group **groups;
    struct list_head node;
    const char *default_trigger;
    long unsigned int blink_delay_on;
    long unsigned int blink_delay_off;
    struct timer_list blink_timer;
    int blink_brightness;
    int new_blink_brightness;
    void (*flash_resume)(struct led_classdev *);
    struct work_struct set_brightness_work;
    int delayed_set_value;
    struct rw_semaphore trigger_lock;
    struct led_trigger *trigger;
    struct list_head trig_list;
    void *trigger_data;
    bool activated;
    int brightness_hw_changed;
    struct kernfs_node *brightness_hw_changed_kn;
    struct mutex led_access;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct led_classdev {
    const char *name;
    enum led_brightness brightness;
    enum led_brightness max_brightness;
    int flags;
    long unsigned int work_flags;
    void (*brightness_set)(struct led_classdev *, enum led_brightness);
    int (*brightness_set_blocking)(struct led_classdev *, enum led_brightness);
    enum led_brightness (*brightness_get)(struct led_classdev *);
    int (*blink_set)(struct led_classdev *, long unsigned int *, long unsigned int *);
    int (*pattern_set)(struct led_classdev *, struct led_pattern *, u32, int);
    int (*pattern_clear)(struct led_classdev *);
    struct device *dev;
    const struct attribute_group **groups;
    struct list_head node;
    const char *default_trigger;
    long unsigned int blink_delay_on;
    long unsigned int blink_delay_off;
    struct timer_list blink_timer;
    int blink_brightness;
    int new_blink_brightness;
    void (*flash_resume)(struct led_classdev *);
    struct work_struct set_brightness_work;
    int delayed_set_value;
    struct rw_semaphore trigger_lock;
    struct led_trigger *trigger;
    struct list_head trig_list;
    void *trigger_data;
    bool activated;
    int brightness_hw_changed;
    struct kernfs_node *brightness_hw_changed_kn;
    struct mutex led_access;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct led_classdev {
    const char *name;
    enum led_brightness brightness;
    enum led_brightness max_brightness;
    int flags;
    long unsigned int work_flags;
    void (*brightness_set)(struct led_classdev *, enum led_brightness);
    int (*brightness_set_blocking)(struct led_classdev *, enum led_brightness);
    enum led_brightness (*brightness_get)(struct led_classdev *);
    int (*blink_set)(struct led_classdev *, long unsigned int *, long unsigned int *);
    int (*pattern_set)(struct led_classdev *, struct led_pattern *, u32, int);
    int (*pattern_clear)(struct led_classdev *);
    struct device *dev;
    const struct attribute_group **groups;
    struct list_head node;
    const char *default_trigger;
    long unsigned int blink_delay_on;
    long unsigned int blink_delay_off;
    struct timer_list blink_timer;
    int blink_brightness;
    int new_blink_brightness;
    void (*flash_resume)(struct led_classdev *);
    struct work_struct set_brightness_work;
    int delayed_set_value;
    struct rw_semaphore trigger_lock;
    struct led_trigger *trigger;
    struct list_head trig_list;
    void *trigger_data;
    bool activated;
    int brightness_hw_changed;
    struct kernfs_node *brightness_hw_changed_kn;
    struct mutex led_access;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct led_classdev {
    const char *name;
    enum led_brightness brightness;
    enum led_brightness max_brightness;
    int flags;
    long unsigned int work_flags;
    void (*brightness_set)(struct led_classdev *, enum led_brightness);
    int (*brightness_set_blocking)(struct led_classdev *, enum led_brightness);
    enum led_brightness (*brightness_get)(struct led_classdev *);
    int (*blink_set)(struct led_classdev *, long unsigned int *, long unsigned int *);
    int (*pattern_set)(struct led_classdev *, struct led_pattern *, u32, int);
    int (*pattern_clear)(struct led_classdev *);
    struct device *dev;
    const struct attribute_group **groups;
    struct list_head node;
    const char *default_trigger;
    long unsigned int blink_delay_on;
    long unsigned int blink_delay_off;
    struct timer_list blink_timer;
    int blink_brightness;
    int new_blink_brightness;
    void (*flash_resume)(struct led_classdev *);
    struct work_struct set_brightness_work;
    int delayed_set_value;
    struct rw_semaphore trigger_lock;
    struct led_trigger *trigger;
    struct list_head trig_list;
    void *trigger_data;
    bool activated;
    int brightness_hw_changed;
    struct kernfs_node *brightness_hw_changed_kn;
    struct mutex led_access;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct led_classdev {
    const char *name;
    enum led_brightness brightness;
    enum led_brightness max_brightness;
    int flags;
    long unsigned int work_flags;
    void (*brightness_set)(struct led_classdev *, enum led_brightness);
    int (*brightness_set_blocking)(struct led_classdev *, enum led_brightness);
    enum led_brightness (*brightness_get)(struct led_classdev *);
    int (*blink_set)(struct led_classdev *, long unsigned int *, long unsigned int *);
    int (*pattern_set)(struct led_classdev *, struct led_pattern *, u32, int);
    int (*pattern_clear)(struct led_classdev *);
    struct device *dev;
    const struct attribute_group **groups;
    struct list_head node;
    const char *default_trigger;
    long unsigned int blink_delay_on;
    long unsigned int blink_delay_off;
    struct timer_list blink_timer;
    int blink_brightness;
    int new_blink_brightness;
    void (*flash_resume)(struct led_classdev *);
    struct work_struct set_brightness_work;
    int delayed_set_value;
    struct rw_semaphore trigger_lock;
    struct led_trigger *trigger;
    struct list_head trig_list;
    void *trigger_data;
    bool activated;
    struct led_hw_trigger_type *trigger_type;
    int brightness_hw_changed;
    struct kernfs_node *brightness_hw_changed_kn;
    struct mutex led_access;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct led_classdev {
    const char *name;
    unsigned int brightness;
    unsigned int max_brightness;
    int flags;
    long unsigned int work_flags;
    void (*brightness_set)(struct led_classdev *, enum led_brightness);
    int (*brightness_set_blocking)(struct led_classdev *, enum led_brightness);
    enum led_brightness (*brightness_get)(struct led_classdev *);
    int (*blink_set)(struct led_classdev *, long unsigned int *, long unsigned int *);
    int (*pattern_set)(struct led_classdev *, struct led_pattern *, u32, int);
    int (*pattern_clear)(struct led_classdev *);
    struct device *dev;
    const struct attribute_group **groups;
    struct list_head node;
    const char *default_trigger;
    long unsigned int blink_delay_on;
    long unsigned int blink_delay_off;
    struct timer_list blink_timer;
    int blink_brightness;
    int new_blink_brightness;
    void (*flash_resume)(struct led_classdev *);
    struct work_struct set_brightness_work;
    int delayed_set_value;
    struct rw_semaphore trigger_lock;
    struct led_trigger *trigger;
    struct list_head trig_list;
    void *trigger_data;
    bool activated;
    struct led_hw_trigger_type *trigger_type;
    int brightness_hw_changed;
    struct kernfs_node *brightness_hw_changed_kn;
    struct mutex led_access;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct led_classdev {
    const char *name;
    unsigned int brightness;
    unsigned int max_brightness;
    int flags;
    long unsigned int work_flags;
    void (*brightness_set)(struct led_classdev *, enum led_brightness);
    int (*brightness_set_blocking)(struct led_classdev *, enum led_brightness);
    enum led_brightness (*brightness_get)(struct led_classdev *);
    int (*blink_set)(struct led_classdev *, long unsigned int *, long unsigned int *);
    int (*pattern_set)(struct led_classdev *, struct led_pattern *, u32, int);
    int (*pattern_clear)(struct led_classdev *);
    struct device *dev;
    const struct attribute_group **groups;
    struct list_head node;
    const char *default_trigger;
    long unsigned int blink_delay_on;
    long unsigned int blink_delay_off;
    struct timer_list blink_timer;
    int blink_brightness;
    int new_blink_brightness;
    void (*flash_resume)(struct led_classdev *);
    struct work_struct set_brightness_work;
    int delayed_set_value;
    struct rw_semaphore trigger_lock;
    struct led_trigger *trigger;
    struct list_head trig_list;
    void *trigger_data;
    bool activated;
    struct led_hw_trigger_type *trigger_type;
    int brightness_hw_changed;
    struct kernfs_node *brightness_hw_changed_kn;
    struct mutex led_access;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct led_classdev {
    const char *name;
    unsigned int brightness;
    unsigned int max_brightness;
    int flags;
    long unsigned int work_flags;
    void (*brightness_set)(struct led_classdev *, enum led_brightness);
    int (*brightness_set_blocking)(struct led_classdev *, enum led_brightness);
    enum led_brightness (*brightness_get)(struct led_classdev *);
    int (*blink_set)(struct led_classdev *, long unsigned int *, long unsigned int *);
    int (*pattern_set)(struct led_classdev *, struct led_pattern *, u32, int);
    int (*pattern_clear)(struct led_classdev *);
    struct device *dev;
    const struct attribute_group **groups;
    struct list_head node;
    const char *default_trigger;
    long unsigned int blink_delay_on;
    long unsigned int blink_delay_off;
    struct timer_list blink_timer;
    int blink_brightness;
    int new_blink_brightness;
    void (*flash_resume)(struct led_classdev *);
    struct work_struct set_brightness_work;
    int delayed_set_value;
    struct rw_semaphore trigger_lock;
    struct led_trigger *trigger;
    struct list_head trig_list;
    void *trigger_data;
    bool activated;
    struct led_hw_trigger_type *trigger_type;
    int brightness_hw_changed;
    struct kernfs_node *brightness_hw_changed_kn;
    struct mutex led_access;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct led_classdev {
    const char *name;
    unsigned int brightness;
    unsigned int max_brightness;
    int flags;
    long unsigned int work_flags;
    void (*brightness_set)(struct led_classdev *, enum led_brightness);
    int (*brightness_set_blocking)(struct led_classdev *, enum led_brightness);
    enum led_brightness (*brightness_get)(struct led_classdev *);
    int (*blink_set)(struct led_classdev *, long unsigned int *, long unsigned int *);
    int (*pattern_set)(struct led_classdev *, struct led_pattern *, u32, int);
    int (*pattern_clear)(struct led_classdev *);
    struct device *dev;
    const struct attribute_group **groups;
    struct list_head node;
    const char *default_trigger;
    long unsigned int blink_delay_on;
    long unsigned int blink_delay_off;
    struct timer_list blink_timer;
    int blink_brightness;
    int new_blink_brightness;
    void (*flash_resume)(struct led_classdev *);
    struct work_struct set_brightness_work;
    int delayed_set_value;
    struct rw_semaphore trigger_lock;
    struct led_trigger *trigger;
    struct list_head trig_list;
    void *trigger_data;
    bool activated;
    struct led_hw_trigger_type *trigger_type;
    int brightness_hw_changed;
    struct kernfs_node *brightness_hw_changed_kn;
    struct mutex led_access;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct led_classdev {
    const char *name;
    unsigned int brightness;
    unsigned int max_brightness;
    int flags;
    long unsigned int work_flags;
    void (*brightness_set)(struct led_classdev *, enum led_brightness);
    int (*brightness_set_blocking)(struct led_classdev *, enum led_brightness);
    enum led_brightness (*brightness_get)(struct led_classdev *);
    int (*blink_set)(struct led_classdev *, long unsigned int *, long unsigned int *);
    int (*pattern_set)(struct led_classdev *, struct led_pattern *, u32, int);
    int (*pattern_clear)(struct led_classdev *);
    struct device *dev;
    const struct attribute_group **groups;
    struct list_head node;
    const char *default_trigger;
    long unsigned int blink_delay_on;
    long unsigned int blink_delay_off;
    struct timer_list blink_timer;
    int blink_brightness;
    int new_blink_brightness;
    void (*flash_resume)(struct led_classdev *);
    struct work_struct set_brightness_work;
    int delayed_set_value;
    long unsigned int delayed_delay_on;
    long unsigned int delayed_delay_off;
    struct rw_semaphore trigger_lock;
    struct led_trigger *trigger;
    struct list_head trig_list;
    void *trigger_data;
    bool activated;
    struct led_hw_trigger_type *trigger_type;
    const char *hw_control_trigger;
    int (*hw_control_is_supported)(struct led_classdev *, long unsigned int);
    int (*hw_control_set)(struct led_classdev *, long unsigned int);
    int (*hw_control_get)(struct led_classdev *, long unsigned int *);
    struct device * (*hw_control_get_device)(struct led_classdev *);
    int brightness_hw_changed;
    struct kernfs_node *brightness_hw_changed_kn;
    struct mutex led_access;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct led_classdev {
    const char *name;
    unsigned int brightness;
    unsigned int max_brightness;
    unsigned int color;
    int flags;
    long unsigned int work_flags;
    void (*brightness_set)(struct led_classdev *, enum led_brightness);
    int (*brightness_set_blocking)(struct led_classdev *, enum led_brightness);
    enum led_brightness (*brightness_get)(struct led_classdev *);
    int (*blink_set)(struct led_classdev *, long unsigned int *, long unsigned int *);
    int (*pattern_set)(struct led_classdev *, struct led_pattern *, u32, int);
    int (*pattern_clear)(struct led_classdev *);
    struct device *dev;
    const struct attribute_group **groups;
    struct list_head node;
    const char *default_trigger;
    long unsigned int blink_delay_on;
    long unsigned int blink_delay_off;
    struct timer_list blink_timer;
    int blink_brightness;
    int new_blink_brightness;
    void (*flash_resume)(struct led_classdev *);
    struct work_struct set_brightness_work;
    int delayed_set_value;
    long unsigned int delayed_delay_on;
    long unsigned int delayed_delay_off;
    struct rw_semaphore trigger_lock;
    struct led_trigger *trigger;
    struct list_head trig_list;
    void *trigger_data;
    bool activated;
    struct led_hw_trigger_type *trigger_type;
    const char *hw_control_trigger;
    int (*hw_control_is_supported)(struct led_classdev *, long unsigned int);
    int (*hw_control_set)(struct led_classdev *, long unsigned int);
    int (*hw_control_get)(struct led_classdev *, long unsigned int *);
    struct device * (*hw_control_get_device)(struct led_classdev *);
    int brightness_hw_changed;
    struct kernfs_node *brightness_hw_changed_kn;
    struct mutex led_access;
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
struct led_classdev {
    const char *name;
    enum led_brightness brightness;
    enum led_brightness max_brightness;
    int flags;
    long unsigned int work_flags;
    void (*brightness_set)(struct led_classdev *, enum led_brightness);
    int (*brightness_set_blocking)(struct led_classdev *, enum led_brightness);
    enum led_brightness (*brightness_get)(struct led_classdev *);
    int (*blink_set)(struct led_classdev *, long unsigned int *, long unsigned int *);
    int (*pattern_set)(struct led_classdev *, struct led_pattern *, u32, int);
    int (*pattern_clear)(struct led_classdev *);
    struct device *dev;
    const struct attribute_group **groups;
    struct list_head node;
    const char *default_trigger;
    long unsigned int blink_delay_on;
    long unsigned int blink_delay_off;
    struct timer_list blink_timer;
    int blink_brightness;
    int new_blink_brightness;
    void (*flash_resume)(struct led_classdev *);
    struct work_struct set_brightness_work;
    int delayed_set_value;
    struct rw_semaphore trigger_lock;
    struct led_trigger *trigger;
    struct list_head trig_list;
    void *trigger_data;
    bool activated;
    int brightness_hw_changed;
    struct kernfs_node *brightness_hw_changed_kn;
    struct mutex led_access;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct led_classdev {
    const char *name;
    enum led_brightness brightness;
    enum led_brightness max_brightness;
    int flags;
    long unsigned int work_flags;
    void (*brightness_set)(struct led_classdev *, enum led_brightness);
    int (*brightness_set_blocking)(struct led_classdev *, enum led_brightness);
    enum led_brightness (*brightness_get)(struct led_classdev *);
    int (*blink_set)(struct led_classdev *, long unsigned int *, long unsigned int *);
    int (*pattern_set)(struct led_classdev *, struct led_pattern *, u32, int);
    int (*pattern_clear)(struct led_classdev *);
    struct device *dev;
    const struct attribute_group **groups;
    struct list_head node;
    const char *default_trigger;
    long unsigned int blink_delay_on;
    long unsigned int blink_delay_off;
    struct timer_list blink_timer;
    int blink_brightness;
    int new_blink_brightness;
    void (*flash_resume)(struct led_classdev *);
    struct work_struct set_brightness_work;
    int delayed_set_value;
    struct rw_semaphore trigger_lock;
    struct led_trigger *trigger;
    struct list_head trig_list;
    void *trigger_data;
    bool activated;
    int brightness_hw_changed;
    struct kernfs_node *brightness_hw_changed_kn;
    struct mutex led_access;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct led_classdev {
    const char *name;
    enum led_brightness brightness;
    enum led_brightness max_brightness;
    int flags;
    long unsigned int work_flags;
    void (*brightness_set)(struct led_classdev *, enum led_brightness);
    int (*brightness_set_blocking)(struct led_classdev *, enum led_brightness);
    enum led_brightness (*brightness_get)(struct led_classdev *);
    int (*blink_set)(struct led_classdev *, long unsigned int *, long unsigned int *);
    int (*pattern_set)(struct led_classdev *, struct led_pattern *, u32, int);
    int (*pattern_clear)(struct led_classdev *);
    struct device *dev;
    const struct attribute_group **groups;
    struct list_head node;
    const char *default_trigger;
    long unsigned int blink_delay_on;
    long unsigned int blink_delay_off;
    struct timer_list blink_timer;
    int blink_brightness;
    int new_blink_brightness;
    void (*flash_resume)(struct led_classdev *);
    struct work_struct set_brightness_work;
    int delayed_set_value;
    struct rw_semaphore trigger_lock;
    struct led_trigger *trigger;
    struct list_head trig_list;
    void *trigger_data;
    bool activated;
    int brightness_hw_changed;
    struct kernfs_node *brightness_hw_changed_kn;
    struct mutex led_access;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct led_classdev {
    const char *name;
    enum led_brightness brightness;
    enum led_brightness max_brightness;
    int flags;
    long unsigned int work_flags;
    void (*brightness_set)(struct led_classdev *, enum led_brightness);
    int (*brightness_set_blocking)(struct led_classdev *, enum led_brightness);
    enum led_brightness (*brightness_get)(struct led_classdev *);
    int (*blink_set)(struct led_classdev *, long unsigned int *, long unsigned int *);
    int (*pattern_set)(struct led_classdev *, struct led_pattern *, u32, int);
    int (*pattern_clear)(struct led_classdev *);
    struct device *dev;
    const struct attribute_group **groups;
    struct list_head node;
    const char *default_trigger;
    long unsigned int blink_delay_on;
    long unsigned int blink_delay_off;
    struct timer_list blink_timer;
    int blink_brightness;
    int new_blink_brightness;
    void (*flash_resume)(struct led_classdev *);
    struct work_struct set_brightness_work;
    int delayed_set_value;
    struct rw_semaphore trigger_lock;
    struct led_trigger *trigger;
    struct list_head trig_list;
    void *trigger_data;
    bool activated;
    int brightness_hw_changed;
    struct kernfs_node *brightness_hw_changed_kn;
    struct mutex led_access;
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
struct led_classdev {
    const char *name;
    enum led_brightness brightness;
    enum led_brightness max_brightness;
    int flags;
    long unsigned int work_flags;
    void (*brightness_set)(struct led_classdev *, enum led_brightness);
    int (*brightness_set_blocking)(struct led_classdev *, enum led_brightness);
    enum led_brightness (*brightness_get)(struct led_classdev *);
    int (*blink_set)(struct led_classdev *, long unsigned int *, long unsigned int *);
    int (*pattern_set)(struct led_classdev *, struct led_pattern *, u32, int);
    int (*pattern_clear)(struct led_classdev *);
    struct device *dev;
    const struct attribute_group **groups;
    struct list_head node;
    const char *default_trigger;
    long unsigned int blink_delay_on;
    long unsigned int blink_delay_off;
    struct timer_list blink_timer;
    int blink_brightness;
    int new_blink_brightness;
    void (*flash_resume)(struct led_classdev *);
    struct work_struct set_brightness_work;
    int delayed_set_value;
    struct rw_semaphore trigger_lock;
    struct led_trigger *trigger;
    struct list_head trig_list;
    void *trigger_data;
    bool activated;
    int brightness_hw_changed;
    struct kernfs_node *brightness_hw_changed_kn;
    struct mutex led_access;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct led_classdev {
    const char *name;
    enum led_brightness brightness;
    enum led_brightness max_brightness;
    int flags;
    long unsigned int work_flags;
    void (*brightness_set)(struct led_classdev *, enum led_brightness);
    int (*brightness_set_blocking)(struct led_classdev *, enum led_brightness);
    enum led_brightness (*brightness_get)(struct led_classdev *);
    int (*blink_set)(struct led_classdev *, long unsigned int *, long unsigned int *);
    int (*pattern_set)(struct led_classdev *, struct led_pattern *, u32, int);
    int (*pattern_clear)(struct led_classdev *);
    struct device *dev;
    const struct attribute_group **groups;
    struct list_head node;
    const char *default_trigger;
    long unsigned int blink_delay_on;
    long unsigned int blink_delay_off;
    struct timer_list blink_timer;
    int blink_brightness;
    int new_blink_brightness;
    void (*flash_resume)(struct led_classdev *);
    struct work_struct set_brightness_work;
    int delayed_set_value;
    struct rw_semaphore trigger_lock;
    struct led_trigger *trigger;
    struct list_head trig_list;
    void *trigger_data;
    bool activated;
    int brightness_hw_changed;
    struct kernfs_node *brightness_hw_changed_kn;
    struct mutex led_access;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct led_classdev {
    const char *name;
    enum led_brightness brightness;
    enum led_brightness max_brightness;
    int flags;
    long unsigned int work_flags;
    void (*brightness_set)(struct led_classdev *, enum led_brightness);
    int (*brightness_set_blocking)(struct led_classdev *, enum led_brightness);
    enum led_brightness (*brightness_get)(struct led_classdev *);
    int (*blink_set)(struct led_classdev *, long unsigned int *, long unsigned int *);
    int (*pattern_set)(struct led_classdev *, struct led_pattern *, u32, int);
    int (*pattern_clear)(struct led_classdev *);
    struct device *dev;
    const struct attribute_group **groups;
    struct list_head node;
    const char *default_trigger;
    long unsigned int blink_delay_on;
    long unsigned int blink_delay_off;
    struct timer_list blink_timer;
    int blink_brightness;
    int new_blink_brightness;
    void (*flash_resume)(struct led_classdev *);
    struct work_struct set_brightness_work;
    int delayed_set_value;
    struct rw_semaphore trigger_lock;
    struct led_trigger *trigger;
    struct list_head trig_list;
    void *trigger_data;
    bool activated;
    int brightness_hw_changed;
    struct kernfs_node *brightness_hw_changed_kn;
    struct mutex led_access;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct led_classdev {
    const char *name;
    enum led_brightness brightness;
    enum led_brightness max_brightness;
    int flags;
    long unsigned int work_flags;
    void (*brightness_set)(struct led_classdev *, enum led_brightness);
    int (*brightness_set_blocking)(struct led_classdev *, enum led_brightness);
    enum led_brightness (*brightness_get)(struct led_classdev *);
    int (*blink_set)(struct led_classdev *, long unsigned int *, long unsigned int *);
    int (*pattern_set)(struct led_classdev *, struct led_pattern *, u32, int);
    int (*pattern_clear)(struct led_classdev *);
    struct device *dev;
    const struct attribute_group **groups;
    struct list_head node;
    const char *default_trigger;
    long unsigned int blink_delay_on;
    long unsigned int blink_delay_off;
    struct timer_list blink_timer;
    int blink_brightness;
    int new_blink_brightness;
    void (*flash_resume)(struct led_classdev *);
    struct work_struct set_brightness_work;
    int delayed_set_value;
    struct rw_semaphore trigger_lock;
    struct led_trigger *trigger;
    struct list_head trig_list;
    void *trigger_data;
    bool activated;
    int brightness_hw_changed;
    struct kernfs_node *brightness_hw_changed_kn;
    struct mutex led_access;
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
<code>int (*brightness_set_blocking)(struct led_classdev *, enum led_brightness)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*brightness_set_sync)(struct led_classdev *, enum led_brightness)</code>
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
<code>long unsigned int work_flags</code>
</li>
<li>
<b>Field added. </b>
<code>int new_blink_brightness</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int brightness_hw_changed</code>
</li>
<li>
<b>Field added. </b>
<code>struct kernfs_node *brightness_hw_changed_kn</code>
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
<code>int (*pattern_set)(struct led_classdev *, struct led_pattern *, u32, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*pattern_clear)(struct led_classdev *)</code>
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
<code>struct led_hw_trigger_type *trigger_type</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>enum led_brightness brightness</code> ➡️ <code>unsigned int brightness</code>
</li>
<li>
<b>Field type changed. </b>
<code>enum led_brightness max_brightness</code> ➡️ <code>unsigned int max_brightness</code>
</li>
</ul>
</details>
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
<b>Field added. </b>
<code>long unsigned int delayed_delay_on</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int delayed_delay_off</code>
</li>
<li>
<b>Field added. </b>
<code>const char *hw_control_trigger</code>
</li>
<li>
<b>Field added. </b>
<code>int (*hw_control_is_supported)(struct led_classdev *, long unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*hw_control_set)(struct led_classdev *, long unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*hw_control_get)(struct led_classdev *, long unsigned int *)</code>
</li>
<li>
<b>Field added. </b>
<code>struct device * (*hw_control_get_device)(struct led_classdev *)</code>
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
<code>unsigned int color</code>
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
