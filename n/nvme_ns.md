# Struct: <code>nvme_ns</code>

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
struct nvme_ns {
    struct list_head list;
    struct nvme_ctrl *ctrl;
    struct request_queue *queue;
    struct gendisk *disk;
    enum nvme_ana_state ana_state;
    u32 ana_grpid;
    struct list_head siblings;
    struct nvm_dev *ndev;
    struct kref kref;
    struct nvme_ns_head *head;
    int lba_shift;
    u16 ms;
    u16 sgs;
    u32 sws;
    bool ext;
    u8 pi_type;
    long unsigned int flags;
    u16 noiob;
    struct nvme_fault_inject fault_inject;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct nvme_ns {
    struct list_head list;
    struct nvme_ctrl *ctrl;
    struct request_queue *queue;
    struct gendisk *disk;
    enum nvme_ana_state ana_state;
    u32 ana_grpid;
    struct list_head siblings;
    struct nvm_dev *ndev;
    struct kref kref;
    struct nvme_ns_head *head;
    int lba_shift;
    u16 ms;
    u16 sgs;
    u32 sws;
    bool ext;
    u8 pi_type;
    long unsigned int flags;
    u16 noiob;
    struct nvme_fault_inject fault_inject;
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
