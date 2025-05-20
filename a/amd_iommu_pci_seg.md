# Struct: <code>amd_iommu_pci_seg</code>

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
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct amd_iommu_pci_seg {
    struct list_head list;
    struct llist_head dev_data_list;
    u16 id;
    u16 last_bdf;
    u32 dev_table_size;
    u32 alias_table_size;
    u32 rlookup_table_size;
    struct dev_table_entry *dev_table;
    struct amd_iommu **rlookup_table;
    struct irq_remap_table **irq_lookup_table;
    struct dev_table_entry *old_dev_tbl_cpy;
    u16 *alias_table;
    struct list_head unity_map;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct amd_iommu_pci_seg {
    struct list_head list;
    struct llist_head dev_data_list;
    u16 id;
    u16 last_bdf;
    u32 dev_table_size;
    u32 alias_table_size;
    u32 rlookup_table_size;
    struct dev_table_entry *dev_table;
    struct amd_iommu **rlookup_table;
    struct irq_remap_table **irq_lookup_table;
    struct dev_table_entry *old_dev_tbl_cpy;
    u16 *alias_table;
    struct list_head unity_map;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct amd_iommu_pci_seg {
    struct list_head list;
    struct llist_head dev_data_list;
    u16 id;
    u16 last_bdf;
    u32 dev_table_size;
    u32 alias_table_size;
    u32 rlookup_table_size;
    struct dev_table_entry *dev_table;
    struct amd_iommu **rlookup_table;
    struct irq_remap_table **irq_lookup_table;
    struct dev_table_entry *old_dev_tbl_cpy;
    u16 *alias_table;
    struct list_head unity_map;
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
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
