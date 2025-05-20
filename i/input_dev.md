# Struct: <code>input_dev</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct input_dev {
    const char *name;
    const char *phys;
    const char *uniq;
    struct input_id id;
    long unsigned int propbit[1];
    long unsigned int evbit[1];
    long unsigned int keybit[12];
    long unsigned int relbit[1];
    long unsigned int absbit[1];
    long unsigned int mscbit[1];
    long unsigned int ledbit[1];
    long unsigned int sndbit[1];
    long unsigned int ffbit[2];
    long unsigned int swbit[1];
    unsigned int hint_events_per_packet;
    unsigned int keycodemax;
    unsigned int keycodesize;
    void *keycode;
    int (*setkeycode)(struct input_dev *, const struct input_keymap_entry *, unsigned int *);
    int (*getkeycode)(struct input_dev *, struct input_keymap_entry *);
    struct ff_device *ff;
    unsigned int repeat_key;
    struct timer_list timer;
    int rep[2];
    struct input_mt *mt;
    struct input_absinfo *absinfo;
    long unsigned int key[12];
    long unsigned int led[1];
    long unsigned int snd[1];
    long unsigned int sw[1];
    int (*open)(struct input_dev *);
    void (*close)(struct input_dev *);
    int (*flush)(struct input_dev *, struct file *);
    int (*event)(struct input_dev *, unsigned int, unsigned int, int);
    struct input_handle *grab;
    spinlock_t event_lock;
    struct mutex mutex;
    unsigned int users;
    bool going_away;
    struct device dev;
    struct list_head h_list;
    struct list_head node;
    unsigned int num_vals;
    unsigned int max_vals;
    struct input_value *vals;
    bool devres_managed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct input_dev {
    const char *name;
    const char *phys;
    const char *uniq;
    struct input_id id;
    long unsigned int propbit[1];
    long unsigned int evbit[1];
    long unsigned int keybit[12];
    long unsigned int relbit[1];
    long unsigned int absbit[1];
    long unsigned int mscbit[1];
    long unsigned int ledbit[1];
    long unsigned int sndbit[1];
    long unsigned int ffbit[2];
    long unsigned int swbit[1];
    unsigned int hint_events_per_packet;
    unsigned int keycodemax;
    unsigned int keycodesize;
    void *keycode;
    int (*setkeycode)(struct input_dev *, const struct input_keymap_entry *, unsigned int *);
    int (*getkeycode)(struct input_dev *, struct input_keymap_entry *);
    struct ff_device *ff;
    unsigned int repeat_key;
    struct timer_list timer;
    int rep[2];
    struct input_mt *mt;
    struct input_absinfo *absinfo;
    long unsigned int key[12];
    long unsigned int led[1];
    long unsigned int snd[1];
    long unsigned int sw[1];
    int (*open)(struct input_dev *);
    void (*close)(struct input_dev *);
    int (*flush)(struct input_dev *, struct file *);
    int (*event)(struct input_dev *, unsigned int, unsigned int, int);
    struct input_handle *grab;
    spinlock_t event_lock;
    struct mutex mutex;
    unsigned int users;
    bool going_away;
    struct device dev;
    struct list_head h_list;
    struct list_head node;
    unsigned int num_vals;
    unsigned int max_vals;
    struct input_value *vals;
    bool devres_managed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct input_dev {
    const char *name;
    const char *phys;
    const char *uniq;
    struct input_id id;
    long unsigned int propbit[1];
    long unsigned int evbit[1];
    long unsigned int keybit[12];
    long unsigned int relbit[1];
    long unsigned int absbit[1];
    long unsigned int mscbit[1];
    long unsigned int ledbit[1];
    long unsigned int sndbit[1];
    long unsigned int ffbit[2];
    long unsigned int swbit[1];
    unsigned int hint_events_per_packet;
    unsigned int keycodemax;
    unsigned int keycodesize;
    void *keycode;
    int (*setkeycode)(struct input_dev *, const struct input_keymap_entry *, unsigned int *);
    int (*getkeycode)(struct input_dev *, struct input_keymap_entry *);
    struct ff_device *ff;
    unsigned int repeat_key;
    struct timer_list timer;
    int rep[2];
    struct input_mt *mt;
    struct input_absinfo *absinfo;
    long unsigned int key[12];
    long unsigned int led[1];
    long unsigned int snd[1];
    long unsigned int sw[1];
    int (*open)(struct input_dev *);
    void (*close)(struct input_dev *);
    int (*flush)(struct input_dev *, struct file *);
    int (*event)(struct input_dev *, unsigned int, unsigned int, int);
    struct input_handle *grab;
    spinlock_t event_lock;
    struct mutex mutex;
    unsigned int users;
    bool going_away;
    struct device dev;
    struct list_head h_list;
    struct list_head node;
    unsigned int num_vals;
    unsigned int max_vals;
    struct input_value *vals;
    bool devres_managed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct input_dev {
    const char *name;
    const char *phys;
    const char *uniq;
    struct input_id id;
    unsigned int flags;
    long unsigned int propbit[1];
    long unsigned int evbit[1];
    long unsigned int keybit[12];
    long unsigned int relbit[1];
    long unsigned int absbit[1];
    long unsigned int mscbit[1];
    long unsigned int ledbit[1];
    long unsigned int sndbit[1];
    long unsigned int ffbit[2];
    long unsigned int swbit[1];
    unsigned int hint_events_per_packet;
    unsigned int keycodemax;
    unsigned int keycodesize;
    void *keycode;
    int (*setkeycode)(struct input_dev *, const struct input_keymap_entry *, unsigned int *);
    int (*getkeycode)(struct input_dev *, struct input_keymap_entry *);
    struct ff_device *ff;
    unsigned int repeat_key;
    struct timer_list timer;
    int rep[2];
    struct input_mt *mt;
    struct input_absinfo *absinfo;
    long unsigned int key[12];
    long unsigned int led[1];
    long unsigned int snd[1];
    long unsigned int sw[1];
    int (*open)(struct input_dev *);
    void (*close)(struct input_dev *);
    int (*flush)(struct input_dev *, struct file *);
    int (*event)(struct input_dev *, unsigned int, unsigned int, int);
    struct input_handle *grab;
    spinlock_t event_lock;
    struct mutex mutex;
    unsigned int users;
    bool going_away;
    struct device dev;
    struct list_head h_list;
    struct list_head node;
    unsigned int num_vals;
    unsigned int max_vals;
    struct input_value *vals;
    bool devres_managed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct input_dev {
    const char *name;
    const char *phys;
    const char *uniq;
    struct input_id id;
    unsigned int flags;
    long unsigned int propbit[1];
    long unsigned int evbit[1];
    long unsigned int keybit[12];
    long unsigned int relbit[1];
    long unsigned int absbit[1];
    long unsigned int mscbit[1];
    long unsigned int ledbit[1];
    long unsigned int sndbit[1];
    long unsigned int ffbit[2];
    long unsigned int swbit[1];
    unsigned int hint_events_per_packet;
    unsigned int keycodemax;
    unsigned int keycodesize;
    void *keycode;
    int (*setkeycode)(struct input_dev *, const struct input_keymap_entry *, unsigned int *);
    int (*getkeycode)(struct input_dev *, struct input_keymap_entry *);
    struct ff_device *ff;
    unsigned int repeat_key;
    struct timer_list timer;
    int rep[2];
    struct input_mt *mt;
    struct input_absinfo *absinfo;
    long unsigned int key[12];
    long unsigned int led[1];
    long unsigned int snd[1];
    long unsigned int sw[1];
    int (*open)(struct input_dev *);
    void (*close)(struct input_dev *);
    int (*flush)(struct input_dev *, struct file *);
    int (*event)(struct input_dev *, unsigned int, unsigned int, int);
    struct input_handle *grab;
    spinlock_t event_lock;
    struct mutex mutex;
    unsigned int users;
    bool going_away;
    struct device dev;
    struct list_head h_list;
    struct list_head node;
    unsigned int num_vals;
    unsigned int max_vals;
    struct input_value *vals;
    bool devres_managed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct input_dev {
    const char *name;
    const char *phys;
    const char *uniq;
    struct input_id id;
    unsigned int flags;
    long unsigned int propbit[1];
    long unsigned int evbit[1];
    long unsigned int keybit[12];
    long unsigned int relbit[1];
    long unsigned int absbit[1];
    long unsigned int mscbit[1];
    long unsigned int ledbit[1];
    long unsigned int sndbit[1];
    long unsigned int ffbit[2];
    long unsigned int swbit[1];
    unsigned int hint_events_per_packet;
    unsigned int keycodemax;
    unsigned int keycodesize;
    void *keycode;
    int (*setkeycode)(struct input_dev *, const struct input_keymap_entry *, unsigned int *);
    int (*getkeycode)(struct input_dev *, struct input_keymap_entry *);
    struct ff_device *ff;
    unsigned int repeat_key;
    struct timer_list timer;
    int rep[2];
    struct input_mt *mt;
    struct input_absinfo *absinfo;
    long unsigned int key[12];
    long unsigned int led[1];
    long unsigned int snd[1];
    long unsigned int sw[1];
    int (*open)(struct input_dev *);
    void (*close)(struct input_dev *);
    int (*flush)(struct input_dev *, struct file *);
    int (*event)(struct input_dev *, unsigned int, unsigned int, int);
    struct input_handle *grab;
    spinlock_t event_lock;
    struct mutex mutex;
    unsigned int users;
    bool going_away;
    struct device dev;
    struct list_head h_list;
    struct list_head node;
    unsigned int num_vals;
    unsigned int max_vals;
    struct input_value *vals;
    bool devres_managed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct input_dev {
    const char *name;
    const char *phys;
    const char *uniq;
    struct input_id id;
    unsigned int flags;
    long unsigned int propbit[1];
    long unsigned int evbit[1];
    long unsigned int keybit[12];
    long unsigned int relbit[1];
    long unsigned int absbit[1];
    long unsigned int mscbit[1];
    long unsigned int ledbit[1];
    long unsigned int sndbit[1];
    long unsigned int ffbit[2];
    long unsigned int swbit[1];
    unsigned int hint_events_per_packet;
    unsigned int keycodemax;
    unsigned int keycodesize;
    void *keycode;
    int (*setkeycode)(struct input_dev *, const struct input_keymap_entry *, unsigned int *);
    int (*getkeycode)(struct input_dev *, struct input_keymap_entry *);
    struct ff_device *ff;
    unsigned int repeat_key;
    struct timer_list timer;
    int rep[2];
    struct input_mt *mt;
    struct input_absinfo *absinfo;
    long unsigned int key[12];
    long unsigned int led[1];
    long unsigned int snd[1];
    long unsigned int sw[1];
    int (*open)(struct input_dev *);
    void (*close)(struct input_dev *);
    int (*flush)(struct input_dev *, struct file *);
    int (*event)(struct input_dev *, unsigned int, unsigned int, int);
    struct input_handle *grab;
    spinlock_t event_lock;
    struct mutex mutex;
    unsigned int users;
    bool going_away;
    struct device dev;
    struct list_head h_list;
    struct list_head node;
    unsigned int num_vals;
    unsigned int max_vals;
    struct input_value *vals;
    bool devres_managed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct input_dev {
    const char *name;
    const char *phys;
    const char *uniq;
    struct input_id id;
    unsigned int flags;
    long unsigned int propbit[1];
    long unsigned int evbit[1];
    long unsigned int keybit[12];
    long unsigned int relbit[1];
    long unsigned int absbit[1];
    long unsigned int mscbit[1];
    long unsigned int ledbit[1];
    long unsigned int sndbit[1];
    long unsigned int ffbit[2];
    long unsigned int swbit[1];
    unsigned int hint_events_per_packet;
    unsigned int keycodemax;
    unsigned int keycodesize;
    void *keycode;
    int (*setkeycode)(struct input_dev *, const struct input_keymap_entry *, unsigned int *);
    int (*getkeycode)(struct input_dev *, struct input_keymap_entry *);
    struct ff_device *ff;
    unsigned int repeat_key;
    struct timer_list timer;
    int rep[2];
    struct input_mt *mt;
    struct input_absinfo *absinfo;
    long unsigned int key[12];
    long unsigned int led[1];
    long unsigned int snd[1];
    long unsigned int sw[1];
    int (*open)(struct input_dev *);
    void (*close)(struct input_dev *);
    int (*flush)(struct input_dev *, struct file *);
    int (*event)(struct input_dev *, unsigned int, unsigned int, int);
    struct input_handle *grab;
    spinlock_t event_lock;
    struct mutex mutex;
    unsigned int users;
    bool going_away;
    struct device dev;
    struct list_head h_list;
    struct list_head node;
    unsigned int num_vals;
    unsigned int max_vals;
    struct input_value *vals;
    bool devres_managed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct input_dev {
    const char *name;
    const char *phys;
    const char *uniq;
    struct input_id id;
    long unsigned int propbit[1];
    long unsigned int evbit[1];
    long unsigned int keybit[12];
    long unsigned int relbit[1];
    long unsigned int absbit[1];
    long unsigned int mscbit[1];
    long unsigned int ledbit[1];
    long unsigned int sndbit[1];
    long unsigned int ffbit[2];
    long unsigned int swbit[1];
    unsigned int hint_events_per_packet;
    unsigned int keycodemax;
    unsigned int keycodesize;
    void *keycode;
    int (*setkeycode)(struct input_dev *, const struct input_keymap_entry *, unsigned int *);
    int (*getkeycode)(struct input_dev *, struct input_keymap_entry *);
    struct ff_device *ff;
    struct input_dev_poller *poller;
    unsigned int repeat_key;
    struct timer_list timer;
    int rep[2];
    struct input_mt *mt;
    struct input_absinfo *absinfo;
    long unsigned int key[12];
    long unsigned int led[1];
    long unsigned int snd[1];
    long unsigned int sw[1];
    int (*open)(struct input_dev *);
    void (*close)(struct input_dev *);
    int (*flush)(struct input_dev *, struct file *);
    int (*event)(struct input_dev *, unsigned int, unsigned int, int);
    struct input_handle *grab;
    spinlock_t event_lock;
    struct mutex mutex;
    unsigned int users;
    bool going_away;
    struct device dev;
    struct list_head h_list;
    struct list_head node;
    unsigned int num_vals;
    unsigned int max_vals;
    struct input_value *vals;
    bool devres_managed;
    ktime_t timestamp[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct input_dev {
    const char *name;
    const char *phys;
    const char *uniq;
    struct input_id id;
    long unsigned int propbit[1];
    long unsigned int evbit[1];
    long unsigned int keybit[12];
    long unsigned int relbit[1];
    long unsigned int absbit[1];
    long unsigned int mscbit[1];
    long unsigned int ledbit[1];
    long unsigned int sndbit[1];
    long unsigned int ffbit[2];
    long unsigned int swbit[1];
    unsigned int hint_events_per_packet;
    unsigned int keycodemax;
    unsigned int keycodesize;
    void *keycode;
    int (*setkeycode)(struct input_dev *, const struct input_keymap_entry *, unsigned int *);
    int (*getkeycode)(struct input_dev *, struct input_keymap_entry *);
    struct ff_device *ff;
    struct input_dev_poller *poller;
    unsigned int repeat_key;
    struct timer_list timer;
    int rep[2];
    struct input_mt *mt;
    struct input_absinfo *absinfo;
    long unsigned int key[12];
    long unsigned int led[1];
    long unsigned int snd[1];
    long unsigned int sw[1];
    int (*open)(struct input_dev *);
    void (*close)(struct input_dev *);
    int (*flush)(struct input_dev *, struct file *);
    int (*event)(struct input_dev *, unsigned int, unsigned int, int);
    struct input_handle *grab;
    spinlock_t event_lock;
    struct mutex mutex;
    unsigned int users;
    bool going_away;
    struct device dev;
    struct list_head h_list;
    struct list_head node;
    unsigned int num_vals;
    unsigned int max_vals;
    struct input_value *vals;
    bool devres_managed;
    ktime_t timestamp[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct input_dev {
    const char *name;
    const char *phys;
    const char *uniq;
    struct input_id id;
    long unsigned int propbit[1];
    long unsigned int evbit[1];
    long unsigned int keybit[12];
    long unsigned int relbit[1];
    long unsigned int absbit[1];
    long unsigned int mscbit[1];
    long unsigned int ledbit[1];
    long unsigned int sndbit[1];
    long unsigned int ffbit[2];
    long unsigned int swbit[1];
    unsigned int hint_events_per_packet;
    unsigned int keycodemax;
    unsigned int keycodesize;
    void *keycode;
    int (*setkeycode)(struct input_dev *, const struct input_keymap_entry *, unsigned int *);
    int (*getkeycode)(struct input_dev *, struct input_keymap_entry *);
    struct ff_device *ff;
    struct input_dev_poller *poller;
    unsigned int repeat_key;
    struct timer_list timer;
    int rep[2];
    struct input_mt *mt;
    struct input_absinfo *absinfo;
    long unsigned int key[12];
    long unsigned int led[1];
    long unsigned int snd[1];
    long unsigned int sw[1];
    int (*open)(struct input_dev *);
    void (*close)(struct input_dev *);
    int (*flush)(struct input_dev *, struct file *);
    int (*event)(struct input_dev *, unsigned int, unsigned int, int);
    struct input_handle *grab;
    spinlock_t event_lock;
    struct mutex mutex;
    unsigned int users;
    bool going_away;
    struct device dev;
    struct list_head h_list;
    struct list_head node;
    unsigned int num_vals;
    unsigned int max_vals;
    struct input_value *vals;
    bool devres_managed;
    ktime_t timestamp[3];
    bool inhibited;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct input_dev {
    const char *name;
    const char *phys;
    const char *uniq;
    struct input_id id;
    long unsigned int propbit[1];
    long unsigned int evbit[1];
    long unsigned int keybit[12];
    long unsigned int relbit[1];
    long unsigned int absbit[1];
    long unsigned int mscbit[1];
    long unsigned int ledbit[1];
    long unsigned int sndbit[1];
    long unsigned int ffbit[2];
    long unsigned int swbit[1];
    unsigned int hint_events_per_packet;
    unsigned int keycodemax;
    unsigned int keycodesize;
    void *keycode;
    int (*setkeycode)(struct input_dev *, const struct input_keymap_entry *, unsigned int *);
    int (*getkeycode)(struct input_dev *, struct input_keymap_entry *);
    struct ff_device *ff;
    struct input_dev_poller *poller;
    unsigned int repeat_key;
    struct timer_list timer;
    int rep[2];
    struct input_mt *mt;
    struct input_absinfo *absinfo;
    long unsigned int key[12];
    long unsigned int led[1];
    long unsigned int snd[1];
    long unsigned int sw[1];
    int (*open)(struct input_dev *);
    void (*close)(struct input_dev *);
    int (*flush)(struct input_dev *, struct file *);
    int (*event)(struct input_dev *, unsigned int, unsigned int, int);
    struct input_handle *grab;
    spinlock_t event_lock;
    struct mutex mutex;
    unsigned int users;
    bool going_away;
    struct device dev;
    struct list_head h_list;
    struct list_head node;
    unsigned int num_vals;
    unsigned int max_vals;
    struct input_value *vals;
    bool devres_managed;
    ktime_t timestamp[3];
    bool inhibited;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct input_dev {
    const char *name;
    const char *phys;
    const char *uniq;
    struct input_id id;
    long unsigned int propbit[1];
    long unsigned int evbit[1];
    long unsigned int keybit[12];
    long unsigned int relbit[1];
    long unsigned int absbit[1];
    long unsigned int mscbit[1];
    long unsigned int ledbit[1];
    long unsigned int sndbit[1];
    long unsigned int ffbit[2];
    long unsigned int swbit[1];
    unsigned int hint_events_per_packet;
    unsigned int keycodemax;
    unsigned int keycodesize;
    void *keycode;
    int (*setkeycode)(struct input_dev *, const struct input_keymap_entry *, unsigned int *);
    int (*getkeycode)(struct input_dev *, struct input_keymap_entry *);
    struct ff_device *ff;
    struct input_dev_poller *poller;
    unsigned int repeat_key;
    struct timer_list timer;
    int rep[2];
    struct input_mt *mt;
    struct input_absinfo *absinfo;
    long unsigned int key[12];
    long unsigned int led[1];
    long unsigned int snd[1];
    long unsigned int sw[1];
    int (*open)(struct input_dev *);
    void (*close)(struct input_dev *);
    int (*flush)(struct input_dev *, struct file *);
    int (*event)(struct input_dev *, unsigned int, unsigned int, int);
    struct input_handle *grab;
    spinlock_t event_lock;
    struct mutex mutex;
    unsigned int users;
    bool going_away;
    struct device dev;
    struct list_head h_list;
    struct list_head node;
    unsigned int num_vals;
    unsigned int max_vals;
    struct input_value *vals;
    bool devres_managed;
    ktime_t timestamp[3];
    bool inhibited;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct input_dev {
    const char *name;
    const char *phys;
    const char *uniq;
    struct input_id id;
    long unsigned int propbit[1];
    long unsigned int evbit[1];
    long unsigned int keybit[12];
    long unsigned int relbit[1];
    long unsigned int absbit[1];
    long unsigned int mscbit[1];
    long unsigned int ledbit[1];
    long unsigned int sndbit[1];
    long unsigned int ffbit[2];
    long unsigned int swbit[1];
    unsigned int hint_events_per_packet;
    unsigned int keycodemax;
    unsigned int keycodesize;
    void *keycode;
    int (*setkeycode)(struct input_dev *, const struct input_keymap_entry *, unsigned int *);
    int (*getkeycode)(struct input_dev *, struct input_keymap_entry *);
    struct ff_device *ff;
    struct input_dev_poller *poller;
    unsigned int repeat_key;
    struct timer_list timer;
    int rep[2];
    struct input_mt *mt;
    struct input_absinfo *absinfo;
    long unsigned int key[12];
    long unsigned int led[1];
    long unsigned int snd[1];
    long unsigned int sw[1];
    int (*open)(struct input_dev *);
    void (*close)(struct input_dev *);
    int (*flush)(struct input_dev *, struct file *);
    int (*event)(struct input_dev *, unsigned int, unsigned int, int);
    struct input_handle *grab;
    spinlock_t event_lock;
    struct mutex mutex;
    unsigned int users;
    bool going_away;
    struct device dev;
    struct list_head h_list;
    struct list_head node;
    unsigned int num_vals;
    unsigned int max_vals;
    struct input_value *vals;
    bool devres_managed;
    ktime_t timestamp[3];
    bool inhibited;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct input_dev {
    const char *name;
    const char *phys;
    const char *uniq;
    struct input_id id;
    long unsigned int propbit[1];
    long unsigned int evbit[1];
    long unsigned int keybit[12];
    long unsigned int relbit[1];
    long unsigned int absbit[1];
    long unsigned int mscbit[1];
    long unsigned int ledbit[1];
    long unsigned int sndbit[1];
    long unsigned int ffbit[2];
    long unsigned int swbit[1];
    unsigned int hint_events_per_packet;
    unsigned int keycodemax;
    unsigned int keycodesize;
    void *keycode;
    int (*setkeycode)(struct input_dev *, const struct input_keymap_entry *, unsigned int *);
    int (*getkeycode)(struct input_dev *, struct input_keymap_entry *);
    struct ff_device *ff;
    struct input_dev_poller *poller;
    unsigned int repeat_key;
    struct timer_list timer;
    int rep[2];
    struct input_mt *mt;
    struct input_absinfo *absinfo;
    long unsigned int key[12];
    long unsigned int led[1];
    long unsigned int snd[1];
    long unsigned int sw[1];
    int (*open)(struct input_dev *);
    void (*close)(struct input_dev *);
    int (*flush)(struct input_dev *, struct file *);
    int (*event)(struct input_dev *, unsigned int, unsigned int, int);
    struct input_handle *grab;
    spinlock_t event_lock;
    struct mutex mutex;
    unsigned int users;
    bool going_away;
    struct device dev;
    struct list_head h_list;
    struct list_head node;
    unsigned int num_vals;
    unsigned int max_vals;
    struct input_value *vals;
    bool devres_managed;
    ktime_t timestamp[3];
    bool inhibited;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct input_dev {
    const char *name;
    const char *phys;
    const char *uniq;
    struct input_id id;
    long unsigned int propbit[1];
    long unsigned int evbit[1];
    long unsigned int keybit[12];
    long unsigned int relbit[1];
    long unsigned int absbit[1];
    long unsigned int mscbit[1];
    long unsigned int ledbit[1];
    long unsigned int sndbit[1];
    long unsigned int ffbit[2];
    long unsigned int swbit[1];
    unsigned int hint_events_per_packet;
    unsigned int keycodemax;
    unsigned int keycodesize;
    void *keycode;
    int (*setkeycode)(struct input_dev *, const struct input_keymap_entry *, unsigned int *);
    int (*getkeycode)(struct input_dev *, struct input_keymap_entry *);
    struct ff_device *ff;
    struct input_dev_poller *poller;
    unsigned int repeat_key;
    struct timer_list timer;
    int rep[2];
    struct input_mt *mt;
    struct input_absinfo *absinfo;
    long unsigned int key[12];
    long unsigned int led[1];
    long unsigned int snd[1];
    long unsigned int sw[1];
    int (*open)(struct input_dev *);
    void (*close)(struct input_dev *);
    int (*flush)(struct input_dev *, struct file *);
    int (*event)(struct input_dev *, unsigned int, unsigned int, int);
    struct input_handle *grab;
    spinlock_t event_lock;
    struct mutex mutex;
    unsigned int users;
    bool going_away;
    struct device dev;
    struct list_head h_list;
    struct list_head node;
    unsigned int num_vals;
    unsigned int max_vals;
    struct input_value *vals;
    bool devres_managed;
    ktime_t timestamp[3];
    bool inhibited;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct input_dev {
    const char *name;
    const char *phys;
    const char *uniq;
    struct input_id id;
    long unsigned int propbit[1];
    long unsigned int evbit[1];
    long unsigned int keybit[12];
    long unsigned int relbit[1];
    long unsigned int absbit[1];
    long unsigned int mscbit[1];
    long unsigned int ledbit[1];
    long unsigned int sndbit[1];
    long unsigned int ffbit[2];
    long unsigned int swbit[1];
    unsigned int hint_events_per_packet;
    unsigned int keycodemax;
    unsigned int keycodesize;
    void *keycode;
    int (*setkeycode)(struct input_dev *, const struct input_keymap_entry *, unsigned int *);
    int (*getkeycode)(struct input_dev *, struct input_keymap_entry *);
    struct ff_device *ff;
    struct input_dev_poller *poller;
    unsigned int repeat_key;
    struct timer_list timer;
    int rep[2];
    struct input_mt *mt;
    struct input_absinfo *absinfo;
    long unsigned int key[12];
    long unsigned int led[1];
    long unsigned int snd[1];
    long unsigned int sw[1];
    int (*open)(struct input_dev *);
    void (*close)(struct input_dev *);
    int (*flush)(struct input_dev *, struct file *);
    int (*event)(struct input_dev *, unsigned int, unsigned int, int);
    struct input_handle *grab;
    spinlock_t event_lock;
    struct mutex mutex;
    unsigned int users;
    bool going_away;
    struct device dev;
    struct list_head h_list;
    struct list_head node;
    unsigned int num_vals;
    unsigned int max_vals;
    struct input_value *vals;
    bool devres_managed;
    ktime_t timestamp[3];
    bool inhibited;
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
struct input_dev {
    const char *name;
    const char *phys;
    const char *uniq;
    struct input_id id;
    long unsigned int propbit[1];
    long unsigned int evbit[1];
    long unsigned int keybit[12];
    long unsigned int relbit[1];
    long unsigned int absbit[1];
    long unsigned int mscbit[1];
    long unsigned int ledbit[1];
    long unsigned int sndbit[1];
    long unsigned int ffbit[2];
    long unsigned int swbit[1];
    unsigned int hint_events_per_packet;
    unsigned int keycodemax;
    unsigned int keycodesize;
    void *keycode;
    int (*setkeycode)(struct input_dev *, const struct input_keymap_entry *, unsigned int *);
    int (*getkeycode)(struct input_dev *, struct input_keymap_entry *);
    struct ff_device *ff;
    struct input_dev_poller *poller;
    unsigned int repeat_key;
    struct timer_list timer;
    int rep[2];
    struct input_mt *mt;
    struct input_absinfo *absinfo;
    long unsigned int key[12];
    long unsigned int led[1];
    long unsigned int snd[1];
    long unsigned int sw[1];
    int (*open)(struct input_dev *);
    void (*close)(struct input_dev *);
    int (*flush)(struct input_dev *, struct file *);
    int (*event)(struct input_dev *, unsigned int, unsigned int, int);
    struct input_handle *grab;
    spinlock_t event_lock;
    struct mutex mutex;
    unsigned int users;
    bool going_away;
    struct device dev;
    struct list_head h_list;
    struct list_head node;
    unsigned int num_vals;
    unsigned int max_vals;
    struct input_value *vals;
    bool devres_managed;
    ktime_t timestamp[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct input_dev {
    const char *name;
    const char *phys;
    const char *uniq;
    struct input_id id;
    long unsigned int propbit[1];
    long unsigned int evbit[1];
    long unsigned int keybit[24];
    long unsigned int relbit[1];
    long unsigned int absbit[2];
    long unsigned int mscbit[1];
    long unsigned int ledbit[1];
    long unsigned int sndbit[1];
    long unsigned int ffbit[4];
    long unsigned int swbit[1];
    unsigned int hint_events_per_packet;
    unsigned int keycodemax;
    unsigned int keycodesize;
    void *keycode;
    int (*setkeycode)(struct input_dev *, const struct input_keymap_entry *, unsigned int *);
    int (*getkeycode)(struct input_dev *, struct input_keymap_entry *);
    struct ff_device *ff;
    struct input_dev_poller *poller;
    unsigned int repeat_key;
    struct timer_list timer;
    int rep[2];
    struct input_mt *mt;
    struct input_absinfo *absinfo;
    long unsigned int key[24];
    long unsigned int led[1];
    long unsigned int snd[1];
    long unsigned int sw[1];
    int (*open)(struct input_dev *);
    void (*close)(struct input_dev *);
    int (*flush)(struct input_dev *, struct file *);
    int (*event)(struct input_dev *, unsigned int, unsigned int, int);
    struct input_handle *grab;
    spinlock_t event_lock;
    struct mutex mutex;
    unsigned int users;
    bool going_away;
    struct device dev;
    struct list_head h_list;
    struct list_head node;
    unsigned int num_vals;
    unsigned int max_vals;
    struct input_value *vals;
    bool devres_managed;
    ktime_t timestamp[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct input_dev {
    const char *name;
    const char *phys;
    const char *uniq;
    struct input_id id;
    long unsigned int propbit[1];
    long unsigned int evbit[1];
    long unsigned int keybit[12];
    long unsigned int relbit[1];
    long unsigned int absbit[1];
    long unsigned int mscbit[1];
    long unsigned int ledbit[1];
    long unsigned int sndbit[1];
    long unsigned int ffbit[2];
    long unsigned int swbit[1];
    unsigned int hint_events_per_packet;
    unsigned int keycodemax;
    unsigned int keycodesize;
    void *keycode;
    int (*setkeycode)(struct input_dev *, const struct input_keymap_entry *, unsigned int *);
    int (*getkeycode)(struct input_dev *, struct input_keymap_entry *);
    struct ff_device *ff;
    struct input_dev_poller *poller;
    unsigned int repeat_key;
    struct timer_list timer;
    int rep[2];
    struct input_mt *mt;
    struct input_absinfo *absinfo;
    long unsigned int key[12];
    long unsigned int led[1];
    long unsigned int snd[1];
    long unsigned int sw[1];
    int (*open)(struct input_dev *);
    void (*close)(struct input_dev *);
    int (*flush)(struct input_dev *, struct file *);
    int (*event)(struct input_dev *, unsigned int, unsigned int, int);
    struct input_handle *grab;
    spinlock_t event_lock;
    struct mutex mutex;
    unsigned int users;
    bool going_away;
    struct device dev;
    struct list_head h_list;
    struct list_head node;
    unsigned int num_vals;
    unsigned int max_vals;
    struct input_value *vals;
    bool devres_managed;
    ktime_t timestamp[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct input_dev {
    const char *name;
    const char *phys;
    const char *uniq;
    struct input_id id;
    long unsigned int propbit[1];
    long unsigned int evbit[1];
    long unsigned int keybit[12];
    long unsigned int relbit[1];
    long unsigned int absbit[1];
    long unsigned int mscbit[1];
    long unsigned int ledbit[1];
    long unsigned int sndbit[1];
    long unsigned int ffbit[2];
    long unsigned int swbit[1];
    unsigned int hint_events_per_packet;
    unsigned int keycodemax;
    unsigned int keycodesize;
    void *keycode;
    int (*setkeycode)(struct input_dev *, const struct input_keymap_entry *, unsigned int *);
    int (*getkeycode)(struct input_dev *, struct input_keymap_entry *);
    struct ff_device *ff;
    struct input_dev_poller *poller;
    unsigned int repeat_key;
    struct timer_list timer;
    int rep[2];
    struct input_mt *mt;
    struct input_absinfo *absinfo;
    long unsigned int key[12];
    long unsigned int led[1];
    long unsigned int snd[1];
    long unsigned int sw[1];
    int (*open)(struct input_dev *);
    void (*close)(struct input_dev *);
    int (*flush)(struct input_dev *, struct file *);
    int (*event)(struct input_dev *, unsigned int, unsigned int, int);
    struct input_handle *grab;
    spinlock_t event_lock;
    struct mutex mutex;
    unsigned int users;
    bool going_away;
    struct device dev;
    struct list_head h_list;
    struct list_head node;
    unsigned int num_vals;
    unsigned int max_vals;
    struct input_value *vals;
    bool devres_managed;
    ktime_t timestamp[3];
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
struct input_dev {
    const char *name;
    const char *phys;
    const char *uniq;
    struct input_id id;
    long unsigned int propbit[1];
    long unsigned int evbit[1];
    long unsigned int keybit[12];
    long unsigned int relbit[1];
    long unsigned int absbit[1];
    long unsigned int mscbit[1];
    long unsigned int ledbit[1];
    long unsigned int sndbit[1];
    long unsigned int ffbit[2];
    long unsigned int swbit[1];
    unsigned int hint_events_per_packet;
    unsigned int keycodemax;
    unsigned int keycodesize;
    void *keycode;
    int (*setkeycode)(struct input_dev *, const struct input_keymap_entry *, unsigned int *);
    int (*getkeycode)(struct input_dev *, struct input_keymap_entry *);
    struct ff_device *ff;
    struct input_dev_poller *poller;
    unsigned int repeat_key;
    struct timer_list timer;
    int rep[2];
    struct input_mt *mt;
    struct input_absinfo *absinfo;
    long unsigned int key[12];
    long unsigned int led[1];
    long unsigned int snd[1];
    long unsigned int sw[1];
    int (*open)(struct input_dev *);
    void (*close)(struct input_dev *);
    int (*flush)(struct input_dev *, struct file *);
    int (*event)(struct input_dev *, unsigned int, unsigned int, int);
    struct input_handle *grab;
    spinlock_t event_lock;
    struct mutex mutex;
    unsigned int users;
    bool going_away;
    struct device dev;
    struct list_head h_list;
    struct list_head node;
    unsigned int num_vals;
    unsigned int max_vals;
    struct input_value *vals;
    bool devres_managed;
    ktime_t timestamp[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct input_dev {
    const char *name;
    const char *phys;
    const char *uniq;
    struct input_id id;
    long unsigned int propbit[1];
    long unsigned int evbit[1];
    long unsigned int keybit[12];
    long unsigned int relbit[1];
    long unsigned int absbit[1];
    long unsigned int mscbit[1];
    long unsigned int ledbit[1];
    long unsigned int sndbit[1];
    long unsigned int ffbit[2];
    long unsigned int swbit[1];
    unsigned int hint_events_per_packet;
    unsigned int keycodemax;
    unsigned int keycodesize;
    void *keycode;
    int (*setkeycode)(struct input_dev *, const struct input_keymap_entry *, unsigned int *);
    int (*getkeycode)(struct input_dev *, struct input_keymap_entry *);
    struct ff_device *ff;
    struct input_dev_poller *poller;
    unsigned int repeat_key;
    struct timer_list timer;
    int rep[2];
    struct input_mt *mt;
    struct input_absinfo *absinfo;
    long unsigned int key[12];
    long unsigned int led[1];
    long unsigned int snd[1];
    long unsigned int sw[1];
    int (*open)(struct input_dev *);
    void (*close)(struct input_dev *);
    int (*flush)(struct input_dev *, struct file *);
    int (*event)(struct input_dev *, unsigned int, unsigned int, int);
    struct input_handle *grab;
    spinlock_t event_lock;
    struct mutex mutex;
    unsigned int users;
    bool going_away;
    struct device dev;
    struct list_head h_list;
    struct list_head node;
    unsigned int num_vals;
    unsigned int max_vals;
    struct input_value *vals;
    bool devres_managed;
    ktime_t timestamp[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct input_dev {
    const char *name;
    const char *phys;
    const char *uniq;
    struct input_id id;
    long unsigned int propbit[1];
    long unsigned int evbit[1];
    long unsigned int keybit[12];
    long unsigned int relbit[1];
    long unsigned int absbit[1];
    long unsigned int mscbit[1];
    long unsigned int ledbit[1];
    long unsigned int sndbit[1];
    long unsigned int ffbit[2];
    long unsigned int swbit[1];
    unsigned int hint_events_per_packet;
    unsigned int keycodemax;
    unsigned int keycodesize;
    void *keycode;
    int (*setkeycode)(struct input_dev *, const struct input_keymap_entry *, unsigned int *);
    int (*getkeycode)(struct input_dev *, struct input_keymap_entry *);
    struct ff_device *ff;
    struct input_dev_poller *poller;
    unsigned int repeat_key;
    struct timer_list timer;
    int rep[2];
    struct input_mt *mt;
    struct input_absinfo *absinfo;
    long unsigned int key[12];
    long unsigned int led[1];
    long unsigned int snd[1];
    long unsigned int sw[1];
    int (*open)(struct input_dev *);
    void (*close)(struct input_dev *);
    int (*flush)(struct input_dev *, struct file *);
    int (*event)(struct input_dev *, unsigned int, unsigned int, int);
    struct input_handle *grab;
    spinlock_t event_lock;
    struct mutex mutex;
    unsigned int users;
    bool going_away;
    struct device dev;
    struct list_head h_list;
    struct list_head node;
    unsigned int num_vals;
    unsigned int max_vals;
    struct input_value *vals;
    bool devres_managed;
    ktime_t timestamp[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct input_dev {
    const char *name;
    const char *phys;
    const char *uniq;
    struct input_id id;
    long unsigned int propbit[1];
    long unsigned int evbit[1];
    long unsigned int keybit[12];
    long unsigned int relbit[1];
    long unsigned int absbit[1];
    long unsigned int mscbit[1];
    long unsigned int ledbit[1];
    long unsigned int sndbit[1];
    long unsigned int ffbit[2];
    long unsigned int swbit[1];
    unsigned int hint_events_per_packet;
    unsigned int keycodemax;
    unsigned int keycodesize;
    void *keycode;
    int (*setkeycode)(struct input_dev *, const struct input_keymap_entry *, unsigned int *);
    int (*getkeycode)(struct input_dev *, struct input_keymap_entry *);
    struct ff_device *ff;
    struct input_dev_poller *poller;
    unsigned int repeat_key;
    struct timer_list timer;
    int rep[2];
    struct input_mt *mt;
    struct input_absinfo *absinfo;
    long unsigned int key[12];
    long unsigned int led[1];
    long unsigned int snd[1];
    long unsigned int sw[1];
    int (*open)(struct input_dev *);
    void (*close)(struct input_dev *);
    int (*flush)(struct input_dev *, struct file *);
    int (*event)(struct input_dev *, unsigned int, unsigned int, int);
    struct input_handle *grab;
    spinlock_t event_lock;
    struct mutex mutex;
    unsigned int users;
    bool going_away;
    struct device dev;
    struct list_head h_list;
    struct list_head node;
    unsigned int num_vals;
    unsigned int max_vals;
    struct input_value *vals;
    bool devres_managed;
    ktime_t timestamp[3];
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
<code>unsigned int flags</code>
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
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct input_dev_poller *poller</code>
</li>
<li>
<b>Field added. </b>
<code>ktime_t timestamp[3]</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int flags</code>
</li>
</ul>
</details>
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
<code>bool inhibited</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long unsigned int keybit[12]</code> ➡️ <code>long unsigned int keybit[24]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int absbit[1]</code> ➡️ <code>long unsigned int absbit[2]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int ffbit[2]</code> ➡️ <code>long unsigned int ffbit[4]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int key[12]</code> ➡️ <code>long unsigned int key[24]</code>
</li>
</ul>
</details>
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
