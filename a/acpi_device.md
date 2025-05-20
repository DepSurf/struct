# Struct: <code>acpi_device</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct acpi_device {
    int device_type;
    acpi_handle handle;
    struct fwnode_handle fwnode;
    struct acpi_device *parent;
    struct list_head children;
    struct list_head node;
    struct list_head wakeup_list;
    struct list_head del_list;
    struct acpi_device_status status;
    struct acpi_device_flags flags;
    struct acpi_device_pnp pnp;
    struct acpi_device_power power;
    struct acpi_device_wakeup wakeup;
    struct acpi_device_perf performance;
    struct acpi_device_dir dir;
    struct acpi_device_data data;
    struct acpi_scan_handler *handler;
    struct acpi_hotplug_context *hp;
    struct acpi_driver *driver;
    const struct acpi_gpio_mapping *driver_gpios;
    void *driver_data;
    struct device dev;
    unsigned int physical_node_count;
    unsigned int dep_unmet;
    struct list_head physical_node_list;
    struct mutex physical_node_lock;
    void (*remove)(struct acpi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct acpi_device {
    int device_type;
    acpi_handle handle;
    struct fwnode_handle fwnode;
    struct acpi_device *parent;
    struct list_head children;
    struct list_head node;
    struct list_head wakeup_list;
    struct list_head del_list;
    struct acpi_device_status status;
    struct acpi_device_flags flags;
    struct acpi_device_pnp pnp;
    struct acpi_device_power power;
    struct acpi_device_wakeup wakeup;
    struct acpi_device_perf performance;
    struct acpi_device_dir dir;
    struct acpi_device_data data;
    struct acpi_scan_handler *handler;
    struct acpi_hotplug_context *hp;
    struct acpi_driver *driver;
    const struct acpi_gpio_mapping *driver_gpios;
    void *driver_data;
    struct device dev;
    unsigned int physical_node_count;
    unsigned int dep_unmet;
    struct list_head physical_node_list;
    struct mutex physical_node_lock;
    void (*remove)(struct acpi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct acpi_device {
    int device_type;
    acpi_handle handle;
    struct fwnode_handle fwnode;
    struct acpi_device *parent;
    struct list_head children;
    struct list_head node;
    struct list_head wakeup_list;
    struct list_head del_list;
    struct acpi_device_status status;
    struct acpi_device_flags flags;
    struct acpi_device_pnp pnp;
    struct acpi_device_power power;
    struct acpi_device_wakeup wakeup;
    struct acpi_device_perf performance;
    struct acpi_device_dir dir;
    struct acpi_device_data data;
    struct acpi_scan_handler *handler;
    struct acpi_hotplug_context *hp;
    struct acpi_driver *driver;
    const struct acpi_gpio_mapping *driver_gpios;
    void *driver_data;
    struct device dev;
    unsigned int physical_node_count;
    unsigned int dep_unmet;
    struct list_head physical_node_list;
    struct mutex physical_node_lock;
    void (*remove)(struct acpi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct acpi_device {
    int device_type;
    acpi_handle handle;
    struct fwnode_handle fwnode;
    struct acpi_device *parent;
    struct list_head children;
    struct list_head node;
    struct list_head wakeup_list;
    struct list_head del_list;
    struct acpi_device_status status;
    struct acpi_device_flags flags;
    struct acpi_device_pnp pnp;
    struct acpi_device_power power;
    struct acpi_device_wakeup wakeup;
    struct acpi_device_perf performance;
    struct acpi_device_dir dir;
    struct acpi_device_data data;
    struct acpi_scan_handler *handler;
    struct acpi_hotplug_context *hp;
    struct acpi_driver *driver;
    const struct acpi_gpio_mapping *driver_gpios;
    void *driver_data;
    struct device dev;
    unsigned int physical_node_count;
    unsigned int dep_unmet;
    struct list_head physical_node_list;
    struct mutex physical_node_lock;
    void (*remove)(struct acpi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct acpi_device {
    int device_type;
    acpi_handle handle;
    struct fwnode_handle fwnode;
    struct acpi_device *parent;
    struct list_head children;
    struct list_head node;
    struct list_head wakeup_list;
    struct list_head del_list;
    struct acpi_device_status status;
    struct acpi_device_flags flags;
    struct acpi_device_pnp pnp;
    struct acpi_device_power power;
    struct acpi_device_wakeup wakeup;
    struct acpi_device_perf performance;
    struct acpi_device_dir dir;
    struct acpi_device_data data;
    struct acpi_scan_handler *handler;
    struct acpi_hotplug_context *hp;
    struct acpi_driver *driver;
    const struct acpi_gpio_mapping *driver_gpios;
    void *driver_data;
    struct device dev;
    unsigned int physical_node_count;
    unsigned int dep_unmet;
    struct list_head physical_node_list;
    struct mutex physical_node_lock;
    void (*remove)(struct acpi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct acpi_device {
    int device_type;
    acpi_handle handle;
    struct fwnode_handle fwnode;
    struct acpi_device *parent;
    struct list_head children;
    struct list_head node;
    struct list_head wakeup_list;
    struct list_head del_list;
    struct acpi_device_status status;
    struct acpi_device_flags flags;
    struct acpi_device_pnp pnp;
    struct acpi_device_power power;
    struct acpi_device_wakeup wakeup;
    struct acpi_device_perf performance;
    struct acpi_device_dir dir;
    struct acpi_device_data data;
    struct acpi_scan_handler *handler;
    struct acpi_hotplug_context *hp;
    struct acpi_driver *driver;
    const struct acpi_gpio_mapping *driver_gpios;
    void *driver_data;
    struct device dev;
    unsigned int physical_node_count;
    unsigned int dep_unmet;
    struct list_head physical_node_list;
    struct mutex physical_node_lock;
    void (*remove)(struct acpi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct acpi_device {
    int device_type;
    acpi_handle handle;
    struct fwnode_handle fwnode;
    struct acpi_device *parent;
    struct list_head children;
    struct list_head node;
    struct list_head wakeup_list;
    struct list_head del_list;
    struct acpi_device_status status;
    struct acpi_device_flags flags;
    struct acpi_device_pnp pnp;
    struct acpi_device_power power;
    struct acpi_device_wakeup wakeup;
    struct acpi_device_perf performance;
    struct acpi_device_dir dir;
    struct acpi_device_data data;
    struct acpi_scan_handler *handler;
    struct acpi_hotplug_context *hp;
    struct acpi_driver *driver;
    const struct acpi_gpio_mapping *driver_gpios;
    void *driver_data;
    struct device dev;
    unsigned int physical_node_count;
    unsigned int dep_unmet;
    struct list_head physical_node_list;
    struct mutex physical_node_lock;
    void (*remove)(struct acpi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct acpi_device {
    int device_type;
    acpi_handle handle;
    struct fwnode_handle fwnode;
    struct acpi_device *parent;
    struct list_head children;
    struct list_head node;
    struct list_head wakeup_list;
    struct list_head del_list;
    struct acpi_device_status status;
    struct acpi_device_flags flags;
    struct acpi_device_pnp pnp;
    struct acpi_device_power power;
    struct acpi_device_wakeup wakeup;
    struct acpi_device_perf performance;
    struct acpi_device_dir dir;
    struct acpi_device_data data;
    struct acpi_scan_handler *handler;
    struct acpi_hotplug_context *hp;
    struct acpi_driver *driver;
    const struct acpi_gpio_mapping *driver_gpios;
    void *driver_data;
    struct device dev;
    unsigned int physical_node_count;
    unsigned int dep_unmet;
    struct list_head physical_node_list;
    struct mutex physical_node_lock;
    void (*remove)(struct acpi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct acpi_device {
    int device_type;
    acpi_handle handle;
    struct fwnode_handle fwnode;
    struct acpi_device *parent;
    struct list_head children;
    struct list_head node;
    struct list_head wakeup_list;
    struct list_head del_list;
    struct acpi_device_status status;
    struct acpi_device_flags flags;
    struct acpi_device_pnp pnp;
    struct acpi_device_power power;
    struct acpi_device_wakeup wakeup;
    struct acpi_device_perf performance;
    struct acpi_device_dir dir;
    struct acpi_device_data data;
    struct acpi_scan_handler *handler;
    struct acpi_hotplug_context *hp;
    struct acpi_driver *driver;
    const struct acpi_gpio_mapping *driver_gpios;
    void *driver_data;
    struct device dev;
    unsigned int physical_node_count;
    unsigned int dep_unmet;
    struct list_head physical_node_list;
    struct mutex physical_node_lock;
    void (*remove)(struct acpi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct acpi_device {
    int device_type;
    acpi_handle handle;
    struct fwnode_handle fwnode;
    struct acpi_device *parent;
    struct list_head children;
    struct list_head node;
    struct list_head wakeup_list;
    struct list_head del_list;
    struct acpi_device_status status;
    struct acpi_device_flags flags;
    struct acpi_device_pnp pnp;
    struct acpi_device_power power;
    struct acpi_device_wakeup wakeup;
    struct acpi_device_perf performance;
    struct acpi_device_dir dir;
    struct acpi_device_data data;
    struct acpi_scan_handler *handler;
    struct acpi_hotplug_context *hp;
    struct acpi_driver *driver;
    const struct acpi_gpio_mapping *driver_gpios;
    void *driver_data;
    struct device dev;
    unsigned int physical_node_count;
    unsigned int dep_unmet;
    struct list_head physical_node_list;
    struct mutex physical_node_lock;
    void (*remove)(struct acpi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct acpi_device {
    int device_type;
    acpi_handle handle;
    struct fwnode_handle fwnode;
    struct acpi_device *parent;
    struct list_head children;
    struct list_head node;
    struct list_head wakeup_list;
    struct list_head del_list;
    struct acpi_device_status status;
    struct acpi_device_flags flags;
    struct acpi_device_pnp pnp;
    struct acpi_device_power power;
    struct acpi_device_wakeup wakeup;
    struct acpi_device_perf performance;
    struct acpi_device_dir dir;
    struct acpi_device_data data;
    struct acpi_scan_handler *handler;
    struct acpi_hotplug_context *hp;
    struct acpi_driver *driver;
    const struct acpi_gpio_mapping *driver_gpios;
    void *driver_data;
    struct device dev;
    unsigned int physical_node_count;
    unsigned int dep_unmet;
    struct list_head physical_node_list;
    struct mutex physical_node_lock;
    void (*remove)(struct acpi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct acpi_device {
    int device_type;
    acpi_handle handle;
    struct fwnode_handle fwnode;
    struct acpi_device *parent;
    struct list_head children;
    struct list_head node;
    struct list_head wakeup_list;
    struct list_head del_list;
    struct acpi_device_status status;
    struct acpi_device_flags flags;
    struct acpi_device_pnp pnp;
    struct acpi_device_power power;
    struct acpi_device_wakeup wakeup;
    struct acpi_device_perf performance;
    struct acpi_device_dir dir;
    struct acpi_device_data data;
    struct acpi_scan_handler *handler;
    struct acpi_hotplug_context *hp;
    struct acpi_driver *driver;
    const struct acpi_gpio_mapping *driver_gpios;
    void *driver_data;
    struct device dev;
    unsigned int physical_node_count;
    unsigned int dep_unmet;
    struct list_head physical_node_list;
    struct mutex physical_node_lock;
    void (*remove)(struct acpi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct acpi_device {
    int device_type;
    acpi_handle handle;
    struct fwnode_handle fwnode;
    struct acpi_device *parent;
    struct list_head children;
    struct list_head node;
    struct list_head wakeup_list;
    struct list_head del_list;
    struct acpi_device_status status;
    struct acpi_device_flags flags;
    struct acpi_device_pnp pnp;
    struct acpi_device_power power;
    struct acpi_device_wakeup wakeup;
    struct acpi_device_perf performance;
    struct acpi_device_dir dir;
    struct acpi_device_data data;
    struct acpi_scan_handler *handler;
    struct acpi_hotplug_context *hp;
    struct acpi_driver *driver;
    const struct acpi_gpio_mapping *driver_gpios;
    void *driver_data;
    struct device dev;
    unsigned int physical_node_count;
    unsigned int dep_unmet;
    struct list_head physical_node_list;
    struct mutex physical_node_lock;
    void (*remove)(struct acpi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct acpi_device {
    u32 pld_crc;
    int device_type;
    acpi_handle handle;
    struct fwnode_handle fwnode;
    struct acpi_device *parent;
    struct list_head children;
    struct list_head node;
    struct list_head wakeup_list;
    struct list_head del_list;
    struct acpi_device_status status;
    struct acpi_device_flags flags;
    struct acpi_device_pnp pnp;
    struct acpi_device_power power;
    struct acpi_device_wakeup wakeup;
    struct acpi_device_perf performance;
    struct acpi_device_dir dir;
    struct acpi_device_data data;
    struct acpi_scan_handler *handler;
    struct acpi_hotplug_context *hp;
    struct acpi_driver *driver;
    const struct acpi_gpio_mapping *driver_gpios;
    void *driver_data;
    struct device dev;
    unsigned int physical_node_count;
    unsigned int dep_unmet;
    struct list_head physical_node_list;
    struct mutex physical_node_lock;
    void (*remove)(struct acpi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct acpi_device {
    u32 pld_crc;
    int device_type;
    acpi_handle handle;
    struct fwnode_handle fwnode;
    struct list_head wakeup_list;
    struct list_head del_list;
    struct acpi_device_status status;
    struct acpi_device_flags flags;
    struct acpi_device_pnp pnp;
    struct acpi_device_power power;
    struct acpi_device_wakeup wakeup;
    struct acpi_device_perf performance;
    struct acpi_device_dir dir;
    struct acpi_device_data data;
    struct acpi_scan_handler *handler;
    struct acpi_hotplug_context *hp;
    const struct acpi_gpio_mapping *driver_gpios;
    void *driver_data;
    struct device dev;
    unsigned int physical_node_count;
    unsigned int dep_unmet;
    struct list_head physical_node_list;
    struct mutex physical_node_lock;
    void (*remove)(struct acpi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct acpi_device {
    u32 pld_crc;
    int device_type;
    acpi_handle handle;
    struct fwnode_handle fwnode;
    struct list_head wakeup_list;
    struct list_head del_list;
    struct acpi_device_status status;
    struct acpi_device_flags flags;
    struct acpi_device_pnp pnp;
    struct acpi_device_power power;
    struct acpi_device_wakeup wakeup;
    struct acpi_device_perf performance;
    struct acpi_device_dir dir;
    struct acpi_device_data data;
    struct acpi_scan_handler *handler;
    struct acpi_hotplug_context *hp;
    const struct acpi_gpio_mapping *driver_gpios;
    void *driver_data;
    struct device dev;
    unsigned int physical_node_count;
    unsigned int dep_unmet;
    struct list_head physical_node_list;
    struct mutex physical_node_lock;
    void (*remove)(struct acpi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct acpi_device {
    u32 pld_crc;
    int device_type;
    acpi_handle handle;
    struct fwnode_handle fwnode;
    struct list_head wakeup_list;
    struct list_head del_list;
    struct acpi_device_status status;
    struct acpi_device_flags flags;
    struct acpi_device_pnp pnp;
    struct acpi_device_power power;
    struct acpi_device_wakeup wakeup;
    struct acpi_device_perf performance;
    struct acpi_device_dir dir;
    struct acpi_device_data data;
    struct acpi_scan_handler *handler;
    struct acpi_hotplug_context *hp;
    struct acpi_device_software_nodes *swnodes;
    const struct acpi_gpio_mapping *driver_gpios;
    void *driver_data;
    struct device dev;
    unsigned int physical_node_count;
    unsigned int dep_unmet;
    struct list_head physical_node_list;
    struct mutex physical_node_lock;
    void (*remove)(struct acpi_device *);
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
struct acpi_device {
    int device_type;
    acpi_handle handle;
    struct fwnode_handle fwnode;
    struct acpi_device *parent;
    struct list_head children;
    struct list_head node;
    struct list_head wakeup_list;
    struct list_head del_list;
    struct acpi_device_status status;
    struct acpi_device_flags flags;
    struct acpi_device_pnp pnp;
    struct acpi_device_power power;
    struct acpi_device_wakeup wakeup;
    struct acpi_device_perf performance;
    struct acpi_device_dir dir;
    struct acpi_device_data data;
    struct acpi_scan_handler *handler;
    struct acpi_hotplug_context *hp;
    struct acpi_driver *driver;
    const struct acpi_gpio_mapping *driver_gpios;
    void *driver_data;
    struct device dev;
    unsigned int physical_node_count;
    unsigned int dep_unmet;
    struct list_head physical_node_list;
    struct mutex physical_node_lock;
    void (*remove)(struct acpi_device *);
};
```
</details>
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct acpi_device {
    int device_type;
    acpi_handle handle;
    struct fwnode_handle fwnode;
    struct acpi_device *parent;
    struct list_head children;
    struct list_head node;
    struct list_head wakeup_list;
    struct list_head del_list;
    struct acpi_device_status status;
    struct acpi_device_flags flags;
    struct acpi_device_pnp pnp;
    struct acpi_device_power power;
    struct acpi_device_wakeup wakeup;
    struct acpi_device_perf performance;
    struct acpi_device_dir dir;
    struct acpi_device_data data;
    struct acpi_scan_handler *handler;
    struct acpi_hotplug_context *hp;
    struct acpi_driver *driver;
    const struct acpi_gpio_mapping *driver_gpios;
    void *driver_data;
    struct device dev;
    unsigned int physical_node_count;
    unsigned int dep_unmet;
    struct list_head physical_node_list;
    struct mutex physical_node_lock;
    void (*remove)(struct acpi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct acpi_device {
    int device_type;
    acpi_handle handle;
    struct fwnode_handle fwnode;
    struct acpi_device *parent;
    struct list_head children;
    struct list_head node;
    struct list_head wakeup_list;
    struct list_head del_list;
    struct acpi_device_status status;
    struct acpi_device_flags flags;
    struct acpi_device_pnp pnp;
    struct acpi_device_power power;
    struct acpi_device_wakeup wakeup;
    struct acpi_device_perf performance;
    struct acpi_device_dir dir;
    struct acpi_device_data data;
    struct acpi_scan_handler *handler;
    struct acpi_hotplug_context *hp;
    struct acpi_driver *driver;
    const struct acpi_gpio_mapping *driver_gpios;
    void *driver_data;
    struct device dev;
    unsigned int physical_node_count;
    unsigned int dep_unmet;
    struct list_head physical_node_list;
    struct mutex physical_node_lock;
    void (*remove)(struct acpi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct acpi_device {
    int device_type;
    acpi_handle handle;
    struct fwnode_handle fwnode;
    struct acpi_device *parent;
    struct list_head children;
    struct list_head node;
    struct list_head wakeup_list;
    struct list_head del_list;
    struct acpi_device_status status;
    struct acpi_device_flags flags;
    struct acpi_device_pnp pnp;
    struct acpi_device_power power;
    struct acpi_device_wakeup wakeup;
    struct acpi_device_perf performance;
    struct acpi_device_dir dir;
    struct acpi_device_data data;
    struct acpi_scan_handler *handler;
    struct acpi_hotplug_context *hp;
    struct acpi_driver *driver;
    const struct acpi_gpio_mapping *driver_gpios;
    void *driver_data;
    struct device dev;
    unsigned int physical_node_count;
    unsigned int dep_unmet;
    struct list_head physical_node_list;
    struct mutex physical_node_lock;
    void (*remove)(struct acpi_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct acpi_device {
    int device_type;
    acpi_handle handle;
    struct fwnode_handle fwnode;
    struct acpi_device *parent;
    struct list_head children;
    struct list_head node;
    struct list_head wakeup_list;
    struct list_head del_list;
    struct acpi_device_status status;
    struct acpi_device_flags flags;
    struct acpi_device_pnp pnp;
    struct acpi_device_power power;
    struct acpi_device_wakeup wakeup;
    struct acpi_device_perf performance;
    struct acpi_device_dir dir;
    struct acpi_device_data data;
    struct acpi_scan_handler *handler;
    struct acpi_hotplug_context *hp;
    struct acpi_driver *driver;
    const struct acpi_gpio_mapping *driver_gpios;
    void *driver_data;
    struct device dev;
    unsigned int physical_node_count;
    unsigned int dep_unmet;
    struct list_head physical_node_list;
    struct mutex physical_node_lock;
    void (*remove)(struct acpi_device *);
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
No changes between <code>4.10</code> and <code>4.13</code> ✅
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
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
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
<code>u32 pld_crc</code>
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
<code>struct acpi_device *parent</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head children</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head node</code>
</li>
<li>
<b>Field removed. </b>
<code>struct acpi_driver *driver</code>
</li>
</ul>
</details>
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
<code>struct acpi_device_software_nodes *swnodes</code>
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
