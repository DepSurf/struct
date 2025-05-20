# Struct: <code>acpi_nfit_desc</code>

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
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct acpi_nfit_desc {
    struct nvdimm_bus_descriptor nd_desc;
    struct acpi_table_header acpi_header;
    struct mutex init_mutex;
    struct list_head memdevs;
    struct list_head flushes;
    struct list_head dimms;
    struct list_head spas;
    struct list_head dcrs;
    struct list_head bdws;
    struct list_head idts;
    struct nvdimm_bus *nvdimm_bus;
    struct device *dev;
    struct nd_cmd_ars_status *ars_status;
    struct nfit_spa *scrub_spa;
    struct delayed_work dwork;
    struct list_head list;
    struct kernfs_node *scrub_count_state;
    unsigned int max_ars;
    unsigned int scrub_count;
    unsigned int scrub_mode;
    long unsigned int scrub_flags;
    long unsigned int dimm_cmd_force_en;
    long unsigned int bus_cmd_force_en;
    long unsigned int bus_nfit_cmd_force_en;
    unsigned int platform_cap;
    unsigned int scrub_tmo;
    int (*blk_do_io)(struct nd_blk_region *, resource_size_t, void *, u64, int);
};
```
</details>
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Flavor</b>
<ul>
</ul>
