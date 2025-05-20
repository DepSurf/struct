# Struct: <code>nvmem_layout</code>

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
struct nvmem_layout {
    const char *name;
    const struct of_device_id *of_match_table;
    int (*add_cells)(struct device *, struct nvmem_device *, struct nvmem_layout *);
    void (*fixup_cell_info)(struct nvmem_device *, struct nvmem_layout *, struct nvmem_cell_info *);
    struct module *owner;
    struct list_head node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct nvmem_layout {
    struct device dev;
    struct nvmem_device *nvmem;
    int (*add_cells)(struct nvmem_layout *);
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct device dev</code>
</li>
<li>
<b>Field added. </b>
<code>struct nvmem_device *nvmem</code>
</li>
<li>
<b>Field removed. </b>
<code>const char *name</code>
</li>
<li>
<b>Field removed. </b>
<code>const struct of_device_id *of_match_table</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*fixup_cell_info)(struct nvmem_device *, struct nvmem_layout *, struct nvmem_cell_info *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct module *owner</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head node</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*add_cells)(struct device *, struct nvmem_device *, struct nvmem_layout *)</code> ➡️ <code>int (*add_cells)(struct nvmem_layout *)</code>
</li>
</ul>
</details>
</li>
</ul>
