# Struct: <code>device_driver</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct device_driver {
    const char *name;
    struct bus_type *bus;
    struct module *owner;
    const char *mod_name;
    bool suppress_bind_attrs;
    enum probe_type probe_type;
    const struct of_device_id *of_match_table;
    const struct acpi_device_id *acpi_match_table;
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct attribute_group **groups;
    const struct dev_pm_ops *pm;
    struct driver_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct device_driver {
    const char *name;
    struct bus_type *bus;
    struct module *owner;
    const char *mod_name;
    bool suppress_bind_attrs;
    enum probe_type probe_type;
    const struct of_device_id *of_match_table;
    const struct acpi_device_id *acpi_match_table;
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct attribute_group **groups;
    const struct dev_pm_ops *pm;
    struct driver_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct device_driver {
    const char *name;
    struct bus_type *bus;
    struct module *owner;
    const char *mod_name;
    bool suppress_bind_attrs;
    enum probe_type probe_type;
    const struct of_device_id *of_match_table;
    const struct acpi_device_id *acpi_match_table;
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct attribute_group **groups;
    const struct dev_pm_ops *pm;
    struct driver_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct device_driver {
    const char *name;
    struct bus_type *bus;
    struct module *owner;
    const char *mod_name;
    bool suppress_bind_attrs;
    enum probe_type probe_type;
    const struct of_device_id *of_match_table;
    const struct acpi_device_id *acpi_match_table;
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct attribute_group **groups;
    const struct dev_pm_ops *pm;
    struct driver_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct device_driver {
    const char *name;
    struct bus_type *bus;
    struct module *owner;
    const char *mod_name;
    bool suppress_bind_attrs;
    enum probe_type probe_type;
    const struct of_device_id *of_match_table;
    const struct acpi_device_id *acpi_match_table;
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct attribute_group **groups;
    const struct dev_pm_ops *pm;
    struct driver_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct device_driver {
    const char *name;
    struct bus_type *bus;
    struct module *owner;
    const char *mod_name;
    bool suppress_bind_attrs;
    enum probe_type probe_type;
    const struct of_device_id *of_match_table;
    const struct acpi_device_id *acpi_match_table;
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct attribute_group **groups;
    const struct dev_pm_ops *pm;
    void (*coredump)(struct device *);
    struct driver_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct device_driver {
    const char *name;
    struct bus_type *bus;
    struct module *owner;
    const char *mod_name;
    bool suppress_bind_attrs;
    enum probe_type probe_type;
    const struct of_device_id *of_match_table;
    const struct acpi_device_id *acpi_match_table;
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct attribute_group **groups;
    const struct dev_pm_ops *pm;
    void (*coredump)(struct device *);
    struct driver_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct device_driver {
    const char *name;
    struct bus_type *bus;
    struct module *owner;
    const char *mod_name;
    bool suppress_bind_attrs;
    enum probe_type probe_type;
    const struct of_device_id *of_match_table;
    const struct acpi_device_id *acpi_match_table;
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct attribute_group **groups;
    const struct dev_pm_ops *pm;
    void (*coredump)(struct device *);
    struct driver_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct device_driver {
    const char *name;
    struct bus_type *bus;
    struct module *owner;
    const char *mod_name;
    bool suppress_bind_attrs;
    enum probe_type probe_type;
    const struct of_device_id *of_match_table;
    const struct acpi_device_id *acpi_match_table;
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct attribute_group **groups;
    const struct attribute_group **dev_groups;
    const struct dev_pm_ops *pm;
    void (*coredump)(struct device *);
    struct driver_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct device_driver {
    const char *name;
    struct bus_type *bus;
    struct module *owner;
    const char *mod_name;
    bool suppress_bind_attrs;
    enum probe_type probe_type;
    const struct of_device_id *of_match_table;
    const struct acpi_device_id *acpi_match_table;
    int (*probe)(struct device *);
    void (*sync_state)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct attribute_group **groups;
    const struct attribute_group **dev_groups;
    const struct dev_pm_ops *pm;
    void (*coredump)(struct device *);
    struct driver_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct device_driver {
    const char *name;
    struct bus_type *bus;
    struct module *owner;
    const char *mod_name;
    bool suppress_bind_attrs;
    enum probe_type probe_type;
    const struct of_device_id *of_match_table;
    const struct acpi_device_id *acpi_match_table;
    int (*probe)(struct device *);
    void (*sync_state)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct attribute_group **groups;
    const struct attribute_group **dev_groups;
    const struct dev_pm_ops *pm;
    void (*coredump)(struct device *);
    struct driver_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct device_driver {
    const char *name;
    struct bus_type *bus;
    struct module *owner;
    const char *mod_name;
    bool suppress_bind_attrs;
    enum probe_type probe_type;
    const struct of_device_id *of_match_table;
    const struct acpi_device_id *acpi_match_table;
    int (*probe)(struct device *);
    void (*sync_state)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct attribute_group **groups;
    const struct attribute_group **dev_groups;
    const struct dev_pm_ops *pm;
    void (*coredump)(struct device *);
    struct driver_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct device_driver {
    const char *name;
    struct bus_type *bus;
    struct module *owner;
    const char *mod_name;
    bool suppress_bind_attrs;
    enum probe_type probe_type;
    const struct of_device_id *of_match_table;
    const struct acpi_device_id *acpi_match_table;
    int (*probe)(struct device *);
    void (*sync_state)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct attribute_group **groups;
    const struct attribute_group **dev_groups;
    const struct dev_pm_ops *pm;
    void (*coredump)(struct device *);
    struct driver_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct device_driver {
    const char *name;
    struct bus_type *bus;
    struct module *owner;
    const char *mod_name;
    bool suppress_bind_attrs;
    enum probe_type probe_type;
    const struct of_device_id *of_match_table;
    const struct acpi_device_id *acpi_match_table;
    int (*probe)(struct device *);
    void (*sync_state)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct attribute_group **groups;
    const struct attribute_group **dev_groups;
    const struct dev_pm_ops *pm;
    void (*coredump)(struct device *);
    struct driver_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct device_driver {
    const char *name;
    struct bus_type *bus;
    struct module *owner;
    const char *mod_name;
    bool suppress_bind_attrs;
    enum probe_type probe_type;
    const struct of_device_id *of_match_table;
    const struct acpi_device_id *acpi_match_table;
    int (*probe)(struct device *);
    void (*sync_state)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct attribute_group **groups;
    const struct attribute_group **dev_groups;
    const struct dev_pm_ops *pm;
    void (*coredump)(struct device *);
    struct driver_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct device_driver {
    const char *name;
    const struct bus_type *bus;
    struct module *owner;
    const char *mod_name;
    bool suppress_bind_attrs;
    enum probe_type probe_type;
    const struct of_device_id *of_match_table;
    const struct acpi_device_id *acpi_match_table;
    int (*probe)(struct device *);
    void (*sync_state)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct attribute_group **groups;
    const struct attribute_group **dev_groups;
    const struct dev_pm_ops *pm;
    void (*coredump)(struct device *);
    struct driver_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct device_driver {
    const char *name;
    const struct bus_type *bus;
    struct module *owner;
    const char *mod_name;
    bool suppress_bind_attrs;
    enum probe_type probe_type;
    const struct of_device_id *of_match_table;
    const struct acpi_device_id *acpi_match_table;
    int (*probe)(struct device *);
    void (*sync_state)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct attribute_group **groups;
    const struct attribute_group **dev_groups;
    const struct dev_pm_ops *pm;
    void (*coredump)(struct device *);
    struct driver_private *p;
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
struct device_driver {
    const char *name;
    struct bus_type *bus;
    struct module *owner;
    const char *mod_name;
    bool suppress_bind_attrs;
    enum probe_type probe_type;
    const struct of_device_id *of_match_table;
    const struct acpi_device_id *acpi_match_table;
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct attribute_group **groups;
    const struct attribute_group **dev_groups;
    const struct dev_pm_ops *pm;
    void (*coredump)(struct device *);
    struct driver_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct device_driver {
    const char *name;
    struct bus_type *bus;
    struct module *owner;
    const char *mod_name;
    bool suppress_bind_attrs;
    enum probe_type probe_type;
    const struct of_device_id *of_match_table;
    const struct acpi_device_id *acpi_match_table;
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct attribute_group **groups;
    const struct attribute_group **dev_groups;
    const struct dev_pm_ops *pm;
    void (*coredump)(struct device *);
    struct driver_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct device_driver {
    const char *name;
    struct bus_type *bus;
    struct module *owner;
    const char *mod_name;
    bool suppress_bind_attrs;
    enum probe_type probe_type;
    const struct of_device_id *of_match_table;
    const struct acpi_device_id *acpi_match_table;
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct attribute_group **groups;
    const struct attribute_group **dev_groups;
    const struct dev_pm_ops *pm;
    void (*coredump)(struct device *);
    struct driver_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct device_driver {
    const char *name;
    struct bus_type *bus;
    struct module *owner;
    const char *mod_name;
    bool suppress_bind_attrs;
    enum probe_type probe_type;
    const struct of_device_id *of_match_table;
    const struct acpi_device_id *acpi_match_table;
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct attribute_group **groups;
    const struct attribute_group **dev_groups;
    const struct dev_pm_ops *pm;
    void (*coredump)(struct device *);
    struct driver_private *p;
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
struct device_driver {
    const char *name;
    struct bus_type *bus;
    struct module *owner;
    const char *mod_name;
    bool suppress_bind_attrs;
    enum probe_type probe_type;
    const struct of_device_id *of_match_table;
    const struct acpi_device_id *acpi_match_table;
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct attribute_group **groups;
    const struct attribute_group **dev_groups;
    const struct dev_pm_ops *pm;
    void (*coredump)(struct device *);
    struct driver_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct device_driver {
    const char *name;
    struct bus_type *bus;
    struct module *owner;
    const char *mod_name;
    bool suppress_bind_attrs;
    enum probe_type probe_type;
    const struct of_device_id *of_match_table;
    const struct acpi_device_id *acpi_match_table;
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct attribute_group **groups;
    const struct attribute_group **dev_groups;
    const struct dev_pm_ops *pm;
    void (*coredump)(struct device *);
    struct driver_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct device_driver {
    const char *name;
    struct bus_type *bus;
    struct module *owner;
    const char *mod_name;
    bool suppress_bind_attrs;
    enum probe_type probe_type;
    const struct of_device_id *of_match_table;
    const struct acpi_device_id *acpi_match_table;
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct attribute_group **groups;
    const struct attribute_group **dev_groups;
    const struct dev_pm_ops *pm;
    void (*coredump)(struct device *);
    struct driver_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct device_driver {
    const char *name;
    struct bus_type *bus;
    struct module *owner;
    const char *mod_name;
    bool suppress_bind_attrs;
    enum probe_type probe_type;
    const struct of_device_id *of_match_table;
    const struct acpi_device_id *acpi_match_table;
    int (*probe)(struct device *);
    int (*remove)(struct device *);
    void (*shutdown)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct attribute_group **groups;
    const struct attribute_group **dev_groups;
    const struct dev_pm_ops *pm;
    void (*coredump)(struct device *);
    struct driver_private *p;
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
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*coredump)(struct device *)</code>
</li>
</ul>
</details>
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
<code>const struct attribute_group **dev_groups</code>
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
<code>void (*sync_state)(struct device *)</code>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct bus_type *bus</code> ➡️ <code>const struct bus_type *bus</code>
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
