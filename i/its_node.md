# Struct: <code>its_node</code>

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
struct its_node {
    raw_spinlock_t lock;
    struct mutex dev_alloc_lock;
    struct list_head entry;
    void *base;
    phys_addr_t phys_base;
    struct its_cmd_block *cmd_base;
    struct its_cmd_block *cmd_write;
    struct its_baser tables[8];
    struct its_collection *collections;
    struct fwnode_handle *fwnode_handle;
    u64 (*get_msi_base)(struct its_device *);
    u64 cbaser_save;
    u32 ctlr_save;
    struct list_head its_device_list;
    u64 flags;
    long unsigned int list_nr;
    u32 ite_size;
    u32 device_ids;
    int numa_node;
    unsigned int msi_domain_flags;
    u32 pre_its_base;
    bool is_v4;
    int vlpi_redist_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct its_node {
    raw_spinlock_t lock;
    struct mutex dev_alloc_lock;
    struct list_head entry;
    void *base;
    phys_addr_t phys_base;
    struct its_cmd_block *cmd_base;
    struct its_cmd_block *cmd_write;
    struct its_baser tables[8];
    struct its_collection *collections;
    struct fwnode_handle *fwnode_handle;
    u64 (*get_msi_base)(struct its_device *);
    u64 cbaser_save;
    u32 ctlr_save;
    struct list_head its_device_list;
    u64 flags;
    long unsigned int list_nr;
    u32 ite_size;
    u32 device_ids;
    int numa_node;
    unsigned int msi_domain_flags;
    u32 pre_its_base;
    bool is_v4;
    int vlpi_redist_offset;
};
```
</details>
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
<b>Arch</b>
<ul>
</ul>
