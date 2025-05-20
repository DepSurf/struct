# Struct: <code>nvme_ns_head</code>

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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct nvme_ns_head {
    struct list_head list;
    struct srcu_struct srcu;
    struct nvme_subsystem *subsys;
    unsigned int ns_id;
    struct nvme_ns_ids ids;
    struct list_head entry;
    struct kref ref;
    int instance;
    struct gendisk *disk;
    struct bio_list requeue_list;
    spinlock_t requeue_lock;
    struct work_struct requeue_work;
    struct mutex lock;
    struct nvme_ns * current_path[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct nvme_ns_head {
    struct list_head list;
    struct srcu_struct srcu;
    struct nvme_subsystem *subsys;
    unsigned int ns_id;
    struct nvme_ns_ids ids;
    struct list_head entry;
    struct kref ref;
    int instance;
    struct gendisk *disk;
    struct bio_list requeue_list;
    spinlock_t requeue_lock;
    struct work_struct requeue_work;
    struct mutex lock;
    struct nvme_ns * current_path[0];
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
