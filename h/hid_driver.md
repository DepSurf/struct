# Struct: <code>hid_driver</code>

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
struct hid_driver {
    char *name;
    const struct hid_device_id *id_table;
    struct list_head dyn_list;
    spinlock_t dyn_lock;
    bool (*match)(struct hid_device *, bool);
    int (*probe)(struct hid_device *, const struct hid_device_id *);
    void (*remove)(struct hid_device *);
    const struct hid_report_id *report_table;
    int (*raw_event)(struct hid_device *, struct hid_report *, u8 *, int);
    const struct hid_usage_id *usage_table;
    int (*event)(struct hid_device *, struct hid_field *, struct hid_usage *, __s32);
    void (*report)(struct hid_device *, struct hid_report *);
    __u8 * (*report_fixup)(struct hid_device *, __u8 *, unsigned int *);
    int (*input_mapping)(struct hid_device *, struct hid_input *, struct hid_field *, struct hid_usage *, long unsigned int **, int *);
    int (*input_mapped)(struct hid_device *, struct hid_input *, struct hid_field *, struct hid_usage *, long unsigned int **, int *);
    int (*input_configured)(struct hid_device *, struct hid_input *);
    void (*feature_mapping)(struct hid_device *, struct hid_field *, struct hid_usage *);
    int (*suspend)(struct hid_device *, pm_message_t);
    int (*resume)(struct hid_device *);
    int (*reset_resume)(struct hid_device *);
    struct device_driver driver;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct hid_driver {
    char *name;
    const struct hid_device_id *id_table;
    struct list_head dyn_list;
    spinlock_t dyn_lock;
    bool (*match)(struct hid_device *, bool);
    int (*probe)(struct hid_device *, const struct hid_device_id *);
    void (*remove)(struct hid_device *);
    const struct hid_report_id *report_table;
    int (*raw_event)(struct hid_device *, struct hid_report *, u8 *, int);
    const struct hid_usage_id *usage_table;
    int (*event)(struct hid_device *, struct hid_field *, struct hid_usage *, __s32);
    void (*report)(struct hid_device *, struct hid_report *);
    __u8 * (*report_fixup)(struct hid_device *, __u8 *, unsigned int *);
    int (*input_mapping)(struct hid_device *, struct hid_input *, struct hid_field *, struct hid_usage *, long unsigned int **, int *);
    int (*input_mapped)(struct hid_device *, struct hid_input *, struct hid_field *, struct hid_usage *, long unsigned int **, int *);
    int (*input_configured)(struct hid_device *, struct hid_input *);
    void (*feature_mapping)(struct hid_device *, struct hid_field *, struct hid_usage *);
    int (*suspend)(struct hid_device *, pm_message_t);
    int (*resume)(struct hid_device *);
    int (*reset_resume)(struct hid_device *);
    struct device_driver driver;
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
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
