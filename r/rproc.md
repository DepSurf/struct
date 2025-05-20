# Struct: <code>rproc</code>

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
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rproc {
    struct list_head node;
    struct iommu_domain *domain;
    const char *name;
    char *firmware;
    void *priv;
    struct rproc_ops *ops;
    struct device dev;
    atomic_t power;
    unsigned int state;
    struct mutex lock;
    struct dentry *dbg_dir;
    struct list_head traces;
    int num_traces;
    struct list_head carveouts;
    struct list_head mappings;
    u32 bootaddr;
    struct list_head rvdevs;
    struct list_head subdevs;
    struct idr notifyids;
    int index;
    struct work_struct crash_handler;
    unsigned int crash_cnt;
    bool recovery_disabled;
    int max_notifyid;
    struct resource_table *table_ptr;
    struct resource_table *cached_table;
    size_t table_sz;
    bool has_iommu;
    bool auto_boot;
    struct list_head dump_segments;
    int nb_vdev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct rproc {
    struct list_head node;
    struct iommu_domain *domain;
    const char *name;
    const char *firmware;
    void *priv;
    struct rproc_ops *ops;
    struct device dev;
    atomic_t power;
    unsigned int state;
    struct mutex lock;
    struct dentry *dbg_dir;
    struct list_head traces;
    int num_traces;
    struct list_head carveouts;
    struct list_head mappings;
    u64 bootaddr;
    struct list_head rvdevs;
    struct list_head subdevs;
    struct idr notifyids;
    int index;
    struct work_struct crash_handler;
    unsigned int crash_cnt;
    bool recovery_disabled;
    int max_notifyid;
    struct resource_table *table_ptr;
    struct resource_table *cached_table;
    size_t table_sz;
    bool has_iommu;
    bool auto_boot;
    struct list_head dump_segments;
    int nb_vdev;
    u8 elf_class;
    u16 elf_machine;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct rproc {
    struct list_head node;
    struct iommu_domain *domain;
    const char *name;
    const char *firmware;
    void *priv;
    struct rproc_ops *ops;
    struct device dev;
    atomic_t power;
    unsigned int state;
    enum rproc_dump_mechanism dump_conf;
    struct mutex lock;
    struct dentry *dbg_dir;
    struct list_head traces;
    int num_traces;
    struct list_head carveouts;
    struct list_head mappings;
    u64 bootaddr;
    struct list_head rvdevs;
    struct list_head subdevs;
    struct idr notifyids;
    int index;
    struct work_struct crash_handler;
    unsigned int crash_cnt;
    bool recovery_disabled;
    int max_notifyid;
    struct resource_table *table_ptr;
    struct resource_table *cached_table;
    size_t table_sz;
    bool has_iommu;
    bool auto_boot;
    bool autonomous;
    struct list_head dump_segments;
    int nb_vdev;
    u8 elf_class;
    u16 elf_machine;
    struct cdev cdev;
    bool cdev_put_on_release;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rproc {
    struct list_head node;
    struct iommu_domain *domain;
    const char *name;
    const char *firmware;
    void *priv;
    struct rproc_ops *ops;
    struct device dev;
    atomic_t power;
    unsigned int state;
    enum rproc_dump_mechanism dump_conf;
    struct mutex lock;
    struct dentry *dbg_dir;
    struct list_head traces;
    int num_traces;
    struct list_head carveouts;
    struct list_head mappings;
    u64 bootaddr;
    struct list_head rvdevs;
    struct list_head subdevs;
    struct idr notifyids;
    int index;
    struct work_struct crash_handler;
    unsigned int crash_cnt;
    bool recovery_disabled;
    int max_notifyid;
    struct resource_table *table_ptr;
    struct resource_table *clean_table;
    struct resource_table *cached_table;
    size_t table_sz;
    bool has_iommu;
    bool auto_boot;
    struct list_head dump_segments;
    int nb_vdev;
    u8 elf_class;
    u16 elf_machine;
    struct cdev cdev;
    bool cdev_put_on_release;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rproc {
    struct list_head node;
    struct iommu_domain *domain;
    const char *name;
    const char *firmware;
    void *priv;
    struct rproc_ops *ops;
    struct device dev;
    atomic_t power;
    unsigned int state;
    enum rproc_dump_mechanism dump_conf;
    struct mutex lock;
    struct dentry *dbg_dir;
    struct list_head traces;
    int num_traces;
    struct list_head carveouts;
    struct list_head mappings;
    u64 bootaddr;
    struct list_head rvdevs;
    struct list_head subdevs;
    struct idr notifyids;
    int index;
    struct work_struct crash_handler;
    unsigned int crash_cnt;
    bool recovery_disabled;
    int max_notifyid;
    struct resource_table *table_ptr;
    struct resource_table *clean_table;
    struct resource_table *cached_table;
    size_t table_sz;
    bool has_iommu;
    bool auto_boot;
    struct list_head dump_segments;
    int nb_vdev;
    u8 elf_class;
    u16 elf_machine;
    struct cdev cdev;
    bool cdev_put_on_release;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rproc {
    struct list_head node;
    struct iommu_domain *domain;
    const char *name;
    const char *firmware;
    void *priv;
    struct rproc_ops *ops;
    struct device dev;
    atomic_t power;
    unsigned int state;
    enum rproc_dump_mechanism dump_conf;
    struct mutex lock;
    struct dentry *dbg_dir;
    struct list_head traces;
    int num_traces;
    struct list_head carveouts;
    struct list_head mappings;
    u64 bootaddr;
    struct list_head rvdevs;
    struct list_head subdevs;
    struct idr notifyids;
    int index;
    struct work_struct crash_handler;
    unsigned int crash_cnt;
    bool recovery_disabled;
    int max_notifyid;
    struct resource_table *table_ptr;
    struct resource_table *clean_table;
    struct resource_table *cached_table;
    size_t table_sz;
    bool has_iommu;
    bool auto_boot;
    bool sysfs_read_only;
    struct list_head dump_segments;
    int nb_vdev;
    u8 elf_class;
    u16 elf_machine;
    struct cdev cdev;
    bool cdev_put_on_release;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rproc {
    struct list_head node;
    struct iommu_domain *domain;
    const char *name;
    const char *firmware;
    void *priv;
    struct rproc_ops *ops;
    struct device dev;
    atomic_t power;
    unsigned int state;
    enum rproc_dump_mechanism dump_conf;
    struct mutex lock;
    struct dentry *dbg_dir;
    struct list_head traces;
    int num_traces;
    struct list_head carveouts;
    struct list_head mappings;
    u64 bootaddr;
    struct list_head rvdevs;
    struct list_head subdevs;
    struct idr notifyids;
    int index;
    struct work_struct crash_handler;
    unsigned int crash_cnt;
    bool recovery_disabled;
    int max_notifyid;
    struct resource_table *table_ptr;
    struct resource_table *clean_table;
    struct resource_table *cached_table;
    size_t table_sz;
    bool has_iommu;
    bool auto_boot;
    bool sysfs_read_only;
    struct list_head dump_segments;
    int nb_vdev;
    u8 elf_class;
    u16 elf_machine;
    struct cdev cdev;
    bool cdev_put_on_release;
    long unsigned int features[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rproc {
    struct list_head node;
    struct iommu_domain *domain;
    const char *name;
    const char *firmware;
    void *priv;
    struct rproc_ops *ops;
    struct device dev;
    atomic_t power;
    unsigned int state;
    enum rproc_dump_mechanism dump_conf;
    struct mutex lock;
    struct dentry *dbg_dir;
    struct list_head traces;
    int num_traces;
    struct list_head carveouts;
    struct list_head mappings;
    u64 bootaddr;
    struct list_head rvdevs;
    struct list_head subdevs;
    struct idr notifyids;
    int index;
    struct work_struct crash_handler;
    unsigned int crash_cnt;
    bool recovery_disabled;
    int max_notifyid;
    struct resource_table *table_ptr;
    struct resource_table *clean_table;
    struct resource_table *cached_table;
    size_t table_sz;
    bool has_iommu;
    bool auto_boot;
    bool sysfs_read_only;
    struct list_head dump_segments;
    int nb_vdev;
    u8 elf_class;
    u16 elf_machine;
    struct cdev cdev;
    bool cdev_put_on_release;
    long unsigned int features[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rproc {
    struct list_head node;
    struct iommu_domain *domain;
    const char *name;
    const char *firmware;
    void *priv;
    struct rproc_ops *ops;
    struct device dev;
    atomic_t power;
    unsigned int state;
    enum rproc_dump_mechanism dump_conf;
    struct mutex lock;
    struct dentry *dbg_dir;
    struct list_head traces;
    int num_traces;
    struct list_head carveouts;
    struct list_head mappings;
    u64 bootaddr;
    struct list_head rvdevs;
    struct list_head subdevs;
    struct idr notifyids;
    int index;
    struct work_struct crash_handler;
    unsigned int crash_cnt;
    bool recovery_disabled;
    int max_notifyid;
    struct resource_table *table_ptr;
    struct resource_table *clean_table;
    struct resource_table *cached_table;
    size_t table_sz;
    bool has_iommu;
    bool auto_boot;
    bool sysfs_read_only;
    struct list_head dump_segments;
    int nb_vdev;
    u8 elf_class;
    u16 elf_machine;
    struct cdev cdev;
    bool cdev_put_on_release;
    long unsigned int features[1];
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
struct rproc {
    struct list_head node;
    struct iommu_domain *domain;
    const char *name;
    char *firmware;
    void *priv;
    struct rproc_ops *ops;
    struct device dev;
    atomic_t power;
    unsigned int state;
    struct mutex lock;
    struct dentry *dbg_dir;
    struct list_head traces;
    int num_traces;
    struct list_head carveouts;
    struct list_head mappings;
    u32 bootaddr;
    struct list_head rvdevs;
    struct list_head subdevs;
    struct idr notifyids;
    int index;
    struct work_struct crash_handler;
    unsigned int crash_cnt;
    bool recovery_disabled;
    int max_notifyid;
    struct resource_table *table_ptr;
    struct resource_table *cached_table;
    size_t table_sz;
    bool has_iommu;
    bool auto_boot;
    struct list_head dump_segments;
    int nb_vdev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rproc {
    struct list_head node;
    struct iommu_domain *domain;
    const char *name;
    char *firmware;
    void *priv;
    struct rproc_ops *ops;
    struct device dev;
    atomic_t power;
    unsigned int state;
    struct mutex lock;
    struct dentry *dbg_dir;
    struct list_head traces;
    int num_traces;
    struct list_head carveouts;
    struct list_head mappings;
    u32 bootaddr;
    struct list_head rvdevs;
    struct list_head subdevs;
    struct idr notifyids;
    int index;
    struct work_struct crash_handler;
    unsigned int crash_cnt;
    bool recovery_disabled;
    int max_notifyid;
    struct resource_table *table_ptr;
    struct resource_table *cached_table;
    size_t table_sz;
    bool has_iommu;
    bool auto_boot;
    struct list_head dump_segments;
    int nb_vdev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rproc {
    struct list_head node;
    struct iommu_domain *domain;
    const char *name;
    char *firmware;
    void *priv;
    struct rproc_ops *ops;
    struct device dev;
    atomic_t power;
    unsigned int state;
    struct mutex lock;
    struct dentry *dbg_dir;
    struct list_head traces;
    int num_traces;
    struct list_head carveouts;
    struct list_head mappings;
    u32 bootaddr;
    struct list_head rvdevs;
    struct list_head subdevs;
    struct idr notifyids;
    int index;
    struct work_struct crash_handler;
    unsigned int crash_cnt;
    bool recovery_disabled;
    int max_notifyid;
    struct resource_table *table_ptr;
    struct resource_table *cached_table;
    size_t table_sz;
    bool has_iommu;
    bool auto_boot;
    struct list_head dump_segments;
    int nb_vdev;
};
```
</details>
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
struct rproc {
    struct list_head node;
    struct iommu_domain *domain;
    const char *name;
    char *firmware;
    void *priv;
    struct rproc_ops *ops;
    struct device dev;
    atomic_t power;
    unsigned int state;
    struct mutex lock;
    struct dentry *dbg_dir;
    struct list_head traces;
    int num_traces;
    struct list_head carveouts;
    struct list_head mappings;
    u32 bootaddr;
    struct list_head rvdevs;
    struct list_head subdevs;
    struct idr notifyids;
    int index;
    struct work_struct crash_handler;
    unsigned int crash_cnt;
    bool recovery_disabled;
    int max_notifyid;
    struct resource_table *table_ptr;
    struct resource_table *cached_table;
    size_t table_sz;
    bool has_iommu;
    bool auto_boot;
    struct list_head dump_segments;
    int nb_vdev;
};
```
</details>
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rproc {
    struct list_head node;
    struct iommu_domain *domain;
    const char *name;
    char *firmware;
    void *priv;
    struct rproc_ops *ops;
    struct device dev;
    atomic_t power;
    unsigned int state;
    struct mutex lock;
    struct dentry *dbg_dir;
    struct list_head traces;
    int num_traces;
    struct list_head carveouts;
    struct list_head mappings;
    u32 bootaddr;
    struct list_head rvdevs;
    struct list_head subdevs;
    struct idr notifyids;
    int index;
    struct work_struct crash_handler;
    unsigned int crash_cnt;
    bool recovery_disabled;
    int max_notifyid;
    struct resource_table *table_ptr;
    struct resource_table *cached_table;
    size_t table_sz;
    bool has_iommu;
    bool auto_boot;
    struct list_head dump_segments;
    int nb_vdev;
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
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 elf_class</code>
</li>
<li>
<b>Field added. </b>
<code>u16 elf_machine</code>
</li>
<li>
<b>Field type changed. </b>
<code>char *firmware</code> ➡️ <code>const char *firmware</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 bootaddr</code> ➡️ <code>u64 bootaddr</code>
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
<code>enum rproc_dump_mechanism dump_conf</code>
</li>
<li>
<b>Field added. </b>
<code>bool autonomous</code>
</li>
<li>
<b>Field added. </b>
<code>struct cdev cdev</code>
</li>
<li>
<b>Field added. </b>
<code>bool cdev_put_on_release</code>
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
<code>struct resource_table *clean_table</code>
</li>
<li>
<b>Field removed. </b>
<code>bool autonomous</code>
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
<code>bool sysfs_read_only</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int features[1]</code>
</li>
</ul>
</details>
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
</ul>
<b>Flavor</b>
<ul>
<li>
No changes between <code>generic</code> and <code>aws</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
