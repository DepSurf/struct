# Struct: <code>mmc_blk_data</code>

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
struct mmc_blk_data {
    struct device *parent;
    struct gendisk *disk;
    struct mmc_queue queue;
    struct list_head part;
    struct list_head rpmbs;
    unsigned int flags;
    unsigned int usage;
    unsigned int read_only;
    unsigned int part_type;
    unsigned int reset_done;
    unsigned int part_curr;
    struct device_attribute force_ro;
    struct device_attribute power_ro_lock;
    int area_type;
    struct dentry *status_dentry;
    struct dentry *ext_csd_dentry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mmc_blk_data {
    struct device *parent;
    struct gendisk *disk;
    struct mmc_queue queue;
    struct list_head part;
    struct list_head rpmbs;
    unsigned int flags;
    unsigned int usage;
    unsigned int read_only;
    unsigned int part_type;
    unsigned int reset_done;
    unsigned int part_curr;
    struct device_attribute force_ro;
    struct device_attribute power_ro_lock;
    int area_type;
    struct dentry *status_dentry;
    struct dentry *ext_csd_dentry;
};
```
</details>
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct mmc_blk_data {
    struct device *parent;
    struct gendisk *disk;
    struct mmc_queue queue;
    struct list_head part;
    struct list_head rpmbs;
    unsigned int flags;
    unsigned int usage;
    unsigned int read_only;
    unsigned int part_type;
    unsigned int reset_done;
    unsigned int part_curr;
    struct device_attribute force_ro;
    struct device_attribute power_ro_lock;
    int area_type;
    struct dentry *status_dentry;
    struct dentry *ext_csd_dentry;
};
```
</details>
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
