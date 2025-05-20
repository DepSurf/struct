# Struct: <code>mfd_cell</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct mfd_cell {
    const char *name;
    int id;
    atomic_t *usage_count;
    int (*enable)(struct platform_device *);
    int (*disable)(struct platform_device *);
    int (*suspend)(struct platform_device *);
    int (*resume)(struct platform_device *);
    void *platform_data;
    size_t pdata_size;
    const struct property_set *pset;
    const char *of_compatible;
    const struct mfd_cell_acpi_match *acpi_match;
    int num_resources;
    const struct resource *resources;
    bool ignore_resource_conflicts;
    bool pm_runtime_no_callbacks;
    const const char * *parent_supplies;
    int num_parent_supplies;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct mfd_cell {
    const char *name;
    int id;
    atomic_t *usage_count;
    int (*enable)(struct platform_device *);
    int (*disable)(struct platform_device *);
    int (*suspend)(struct platform_device *);
    int (*resume)(struct platform_device *);
    void *platform_data;
    size_t pdata_size;
    struct property_entry *properties;
    const char *of_compatible;
    const struct mfd_cell_acpi_match *acpi_match;
    int num_resources;
    const struct resource *resources;
    bool ignore_resource_conflicts;
    bool pm_runtime_no_callbacks;
    const const char * *parent_supplies;
    int num_parent_supplies;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct mfd_cell {
    const char *name;
    int id;
    atomic_t *usage_count;
    int (*enable)(struct platform_device *);
    int (*disable)(struct platform_device *);
    int (*suspend)(struct platform_device *);
    int (*resume)(struct platform_device *);
    void *platform_data;
    size_t pdata_size;
    struct property_entry *properties;
    const char *of_compatible;
    const struct mfd_cell_acpi_match *acpi_match;
    int num_resources;
    const struct resource *resources;
    bool ignore_resource_conflicts;
    bool pm_runtime_no_callbacks;
    const const char * *parent_supplies;
    int num_parent_supplies;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct mfd_cell {
    const char *name;
    int id;
    atomic_t *usage_count;
    int (*enable)(struct platform_device *);
    int (*disable)(struct platform_device *);
    int (*suspend)(struct platform_device *);
    int (*resume)(struct platform_device *);
    void *platform_data;
    size_t pdata_size;
    struct property_entry *properties;
    const char *of_compatible;
    const struct mfd_cell_acpi_match *acpi_match;
    int num_resources;
    const struct resource *resources;
    bool ignore_resource_conflicts;
    bool pm_runtime_no_callbacks;
    const const char * *parent_supplies;
    int num_parent_supplies;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct mfd_cell {
    const char *name;
    int id;
    atomic_t *usage_count;
    int (*enable)(struct platform_device *);
    int (*disable)(struct platform_device *);
    int (*suspend)(struct platform_device *);
    int (*resume)(struct platform_device *);
    void *platform_data;
    size_t pdata_size;
    struct property_entry *properties;
    const char *of_compatible;
    const struct mfd_cell_acpi_match *acpi_match;
    int num_resources;
    const struct resource *resources;
    bool ignore_resource_conflicts;
    bool pm_runtime_no_callbacks;
    const const char * *parent_supplies;
    int num_parent_supplies;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct mfd_cell {
    const char *name;
    int id;
    atomic_t *usage_count;
    int (*enable)(struct platform_device *);
    int (*disable)(struct platform_device *);
    int (*suspend)(struct platform_device *);
    int (*resume)(struct platform_device *);
    void *platform_data;
    size_t pdata_size;
    struct property_entry *properties;
    const char *of_compatible;
    const struct mfd_cell_acpi_match *acpi_match;
    int num_resources;
    const struct resource *resources;
    bool ignore_resource_conflicts;
    bool pm_runtime_no_callbacks;
    const const char * *parent_supplies;
    int num_parent_supplies;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct mfd_cell {
    const char *name;
    int id;
    atomic_t *usage_count;
    int (*enable)(struct platform_device *);
    int (*disable)(struct platform_device *);
    int (*suspend)(struct platform_device *);
    int (*resume)(struct platform_device *);
    void *platform_data;
    size_t pdata_size;
    struct property_entry *properties;
    const char *of_compatible;
    const struct mfd_cell_acpi_match *acpi_match;
    int num_resources;
    const struct resource *resources;
    bool ignore_resource_conflicts;
    bool pm_runtime_no_callbacks;
    const const char * *parent_supplies;
    int num_parent_supplies;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct mfd_cell {
    const char *name;
    int id;
    atomic_t *usage_count;
    int (*enable)(struct platform_device *);
    int (*disable)(struct platform_device *);
    int (*suspend)(struct platform_device *);
    int (*resume)(struct platform_device *);
    void *platform_data;
    size_t pdata_size;
    struct property_entry *properties;
    const char *of_compatible;
    const struct mfd_cell_acpi_match *acpi_match;
    int num_resources;
    const struct resource *resources;
    bool ignore_resource_conflicts;
    bool pm_runtime_no_callbacks;
    const const char * *parent_supplies;
    int num_parent_supplies;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct mfd_cell {
    const char *name;
    int id;
    atomic_t *usage_count;
    int (*enable)(struct platform_device *);
    int (*disable)(struct platform_device *);
    int (*suspend)(struct platform_device *);
    int (*resume)(struct platform_device *);
    void *platform_data;
    size_t pdata_size;
    struct property_entry *properties;
    const char *of_compatible;
    const struct mfd_cell_acpi_match *acpi_match;
    int num_resources;
    const struct resource *resources;
    bool ignore_resource_conflicts;
    bool pm_runtime_no_callbacks;
    const const char * *parent_supplies;
    int num_parent_supplies;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct mfd_cell {
    const char *name;
    int id;
    int (*enable)(struct platform_device *);
    int (*disable)(struct platform_device *);
    int (*suspend)(struct platform_device *);
    int (*resume)(struct platform_device *);
    void *platform_data;
    size_t pdata_size;
    const struct property_entry *properties;
    const char *of_compatible;
    const struct mfd_cell_acpi_match *acpi_match;
    int num_resources;
    const struct resource *resources;
    bool ignore_resource_conflicts;
    bool pm_runtime_no_callbacks;
    const const char * *parent_supplies;
    int num_parent_supplies;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mfd_cell {
    const char *name;
    int id;
    int level;
    int (*enable)(struct platform_device *);
    int (*disable)(struct platform_device *);
    int (*suspend)(struct platform_device *);
    int (*resume)(struct platform_device *);
    void *platform_data;
    size_t pdata_size;
    const struct property_entry *properties;
    const char *of_compatible;
    const u64 of_reg;
    bool use_of_reg;
    const struct mfd_cell_acpi_match *acpi_match;
    int num_resources;
    const struct resource *resources;
    bool ignore_resource_conflicts;
    bool pm_runtime_no_callbacks;
    const const char * *parent_supplies;
    int num_parent_supplies;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mfd_cell {
    const char *name;
    int id;
    int level;
    int (*enable)(struct platform_device *);
    int (*disable)(struct platform_device *);
    int (*suspend)(struct platform_device *);
    int (*resume)(struct platform_device *);
    void *platform_data;
    size_t pdata_size;
    const struct software_node *swnode;
    const char *of_compatible;
    const u64 of_reg;
    bool use_of_reg;
    const struct mfd_cell_acpi_match *acpi_match;
    int num_resources;
    const struct resource *resources;
    bool ignore_resource_conflicts;
    bool pm_runtime_no_callbacks;
    const const char * *parent_supplies;
    int num_parent_supplies;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mfd_cell {
    const char *name;
    int id;
    int level;
    int (*enable)(struct platform_device *);
    int (*disable)(struct platform_device *);
    int (*suspend)(struct platform_device *);
    int (*resume)(struct platform_device *);
    void *platform_data;
    size_t pdata_size;
    const struct software_node *swnode;
    const char *of_compatible;
    const u64 of_reg;
    bool use_of_reg;
    const struct mfd_cell_acpi_match *acpi_match;
    int num_resources;
    const struct resource *resources;
    bool ignore_resource_conflicts;
    bool pm_runtime_no_callbacks;
    const const char * *parent_supplies;
    int num_parent_supplies;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mfd_cell {
    const char *name;
    int id;
    int level;
    int (*enable)(struct platform_device *);
    int (*disable)(struct platform_device *);
    int (*suspend)(struct platform_device *);
    int (*resume)(struct platform_device *);
    void *platform_data;
    size_t pdata_size;
    const struct software_node *swnode;
    const char *of_compatible;
    const u64 of_reg;
    bool use_of_reg;
    const struct mfd_cell_acpi_match *acpi_match;
    int num_resources;
    const struct resource *resources;
    bool ignore_resource_conflicts;
    bool pm_runtime_no_callbacks;
    const const char * *parent_supplies;
    int num_parent_supplies;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mfd_cell {
    const char *name;
    int id;
    int level;
    int (*enable)(struct platform_device *);
    int (*disable)(struct platform_device *);
    int (*suspend)(struct platform_device *);
    int (*resume)(struct platform_device *);
    void *platform_data;
    size_t pdata_size;
    const struct software_node *swnode;
    const char *of_compatible;
    const u64 of_reg;
    bool use_of_reg;
    const struct mfd_cell_acpi_match *acpi_match;
    int num_resources;
    const struct resource *resources;
    bool ignore_resource_conflicts;
    bool pm_runtime_no_callbacks;
    const const char * *parent_supplies;
    int num_parent_supplies;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mfd_cell {
    const char *name;
    int id;
    int level;
    int (*suspend)(struct platform_device *);
    int (*resume)(struct platform_device *);
    void *platform_data;
    size_t pdata_size;
    const struct mfd_cell_acpi_match *acpi_match;
    const struct software_node *swnode;
    const char *of_compatible;
    const u64 of_reg;
    bool use_of_reg;
    int num_resources;
    const struct resource *resources;
    bool ignore_resource_conflicts;
    bool pm_runtime_no_callbacks;
    int num_parent_supplies;
    const const char * *parent_supplies;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mfd_cell {
    const char *name;
    int id;
    int level;
    int (*suspend)(struct platform_device *);
    int (*resume)(struct platform_device *);
    void *platform_data;
    size_t pdata_size;
    const struct mfd_cell_acpi_match *acpi_match;
    const struct software_node *swnode;
    const char *of_compatible;
    u64 of_reg;
    bool use_of_reg;
    int num_resources;
    const struct resource *resources;
    bool ignore_resource_conflicts;
    bool pm_runtime_no_callbacks;
    int num_parent_supplies;
    const const char * *parent_supplies;
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
struct mfd_cell {
    const char *name;
    int id;
    atomic_t *usage_count;
    int (*enable)(struct platform_device *);
    int (*disable)(struct platform_device *);
    int (*suspend)(struct platform_device *);
    int (*resume)(struct platform_device *);
    void *platform_data;
    size_t pdata_size;
    struct property_entry *properties;
    const char *of_compatible;
    const struct mfd_cell_acpi_match *acpi_match;
    int num_resources;
    const struct resource *resources;
    bool ignore_resource_conflicts;
    bool pm_runtime_no_callbacks;
    const const char * *parent_supplies;
    int num_parent_supplies;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mfd_cell {
    const char *name;
    int id;
    atomic_t *usage_count;
    int (*enable)(struct platform_device *);
    int (*disable)(struct platform_device *);
    int (*suspend)(struct platform_device *);
    int (*resume)(struct platform_device *);
    void *platform_data;
    size_t pdata_size;
    struct property_entry *properties;
    const char *of_compatible;
    const struct mfd_cell_acpi_match *acpi_match;
    int num_resources;
    const struct resource *resources;
    bool ignore_resource_conflicts;
    bool pm_runtime_no_callbacks;
    const const char * *parent_supplies;
    int num_parent_supplies;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct mfd_cell {
    const char *name;
    int id;
    atomic_t *usage_count;
    int (*enable)(struct platform_device *);
    int (*disable)(struct platform_device *);
    int (*suspend)(struct platform_device *);
    int (*resume)(struct platform_device *);
    void *platform_data;
    size_t pdata_size;
    struct property_entry *properties;
    const char *of_compatible;
    const struct mfd_cell_acpi_match *acpi_match;
    int num_resources;
    const struct resource *resources;
    bool ignore_resource_conflicts;
    bool pm_runtime_no_callbacks;
    const const char * *parent_supplies;
    int num_parent_supplies;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct mfd_cell {
    const char *name;
    int id;
    atomic_t *usage_count;
    int (*enable)(struct platform_device *);
    int (*disable)(struct platform_device *);
    int (*suspend)(struct platform_device *);
    int (*resume)(struct platform_device *);
    void *platform_data;
    size_t pdata_size;
    struct property_entry *properties;
    const char *of_compatible;
    const struct mfd_cell_acpi_match *acpi_match;
    int num_resources;
    const struct resource *resources;
    bool ignore_resource_conflicts;
    bool pm_runtime_no_callbacks;
    const const char * *parent_supplies;
    int num_parent_supplies;
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
struct mfd_cell {
    const char *name;
    int id;
    atomic_t *usage_count;
    int (*enable)(struct platform_device *);
    int (*disable)(struct platform_device *);
    int (*suspend)(struct platform_device *);
    int (*resume)(struct platform_device *);
    void *platform_data;
    size_t pdata_size;
    struct property_entry *properties;
    const char *of_compatible;
    const struct mfd_cell_acpi_match *acpi_match;
    int num_resources;
    const struct resource *resources;
    bool ignore_resource_conflicts;
    bool pm_runtime_no_callbacks;
    const const char * *parent_supplies;
    int num_parent_supplies;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct mfd_cell {
    const char *name;
    int id;
    atomic_t *usage_count;
    int (*enable)(struct platform_device *);
    int (*disable)(struct platform_device *);
    int (*suspend)(struct platform_device *);
    int (*resume)(struct platform_device *);
    void *platform_data;
    size_t pdata_size;
    struct property_entry *properties;
    const char *of_compatible;
    const struct mfd_cell_acpi_match *acpi_match;
    int num_resources;
    const struct resource *resources;
    bool ignore_resource_conflicts;
    bool pm_runtime_no_callbacks;
    const const char * *parent_supplies;
    int num_parent_supplies;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct mfd_cell {
    const char *name;
    int id;
    atomic_t *usage_count;
    int (*enable)(struct platform_device *);
    int (*disable)(struct platform_device *);
    int (*suspend)(struct platform_device *);
    int (*resume)(struct platform_device *);
    void *platform_data;
    size_t pdata_size;
    struct property_entry *properties;
    const char *of_compatible;
    const struct mfd_cell_acpi_match *acpi_match;
    int num_resources;
    const struct resource *resources;
    bool ignore_resource_conflicts;
    bool pm_runtime_no_callbacks;
    const const char * *parent_supplies;
    int num_parent_supplies;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct mfd_cell {
    const char *name;
    int id;
    atomic_t *usage_count;
    int (*enable)(struct platform_device *);
    int (*disable)(struct platform_device *);
    int (*suspend)(struct platform_device *);
    int (*resume)(struct platform_device *);
    void *platform_data;
    size_t pdata_size;
    struct property_entry *properties;
    const char *of_compatible;
    const struct mfd_cell_acpi_match *acpi_match;
    int num_resources;
    const struct resource *resources;
    bool ignore_resource_conflicts;
    bool pm_runtime_no_callbacks;
    const const char * *parent_supplies;
    int num_parent_supplies;
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
<code>struct property_entry *properties</code>
</li>
<li>
<b>Field removed. </b>
<code>const struct property_set *pset</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>atomic_t *usage_count</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct property_entry *properties</code> ➡️ <code>const struct property_entry *properties</code>
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
<code>int level</code>
</li>
<li>
<b>Field added. </b>
<code>const u64 of_reg</code>
</li>
<li>
<b>Field added. </b>
<code>bool use_of_reg</code>
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
<code>const struct software_node *swnode</code>
</li>
<li>
<b>Field removed. </b>
<code>const struct property_entry *properties</code>
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
<b>Field removed. </b>
<code>int (*enable)(struct platform_device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*disable)(struct platform_device *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>const u64 of_reg</code> ➡️ <code>u64 of_reg</code>
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
