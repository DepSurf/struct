# Struct: <code>virtio_scsi</code>

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
struct virtio_scsi {
    struct virtio_device *vdev;
    struct virtio_scsi_event_node event_list[8];
    u32 num_queues;
    struct hlist_node node;
    bool stop_events;
    struct virtio_scsi_vq ctrl_vq;
    struct virtio_scsi_vq event_vq;
    struct virtio_scsi_vq req_vqs[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct virtio_scsi {
    struct virtio_device *vdev;
    struct virtio_scsi_event_node event_list[8];
    u32 num_queues;
    int io_queues[3];
    struct hlist_node node;
    bool stop_events;
    struct virtio_scsi_vq ctrl_vq;
    struct virtio_scsi_vq event_vq;
    struct virtio_scsi_vq req_vqs[0];
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
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct virtio_scsi {
    struct virtio_device *vdev;
    struct virtio_scsi_event_node event_list[8];
    u32 num_queues;
    struct hlist_node node;
    bool stop_events;
    struct virtio_scsi_vq ctrl_vq;
    struct virtio_scsi_vq event_vq;
    struct virtio_scsi_vq req_vqs[0];
};
```
</details>
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
<code>int io_queues[3]</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Flavor</b>
<ul>
</ul>
