# Struct: <code>virtio_blk_config</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct virtio_blk_config {
    __u64 capacity;
    __u32 size_max;
    __u32 seg_max;
    struct virtio_blk_geometry geometry;
    __u32 blk_size;
    __u8 physical_block_exp;
    __u8 alignment_offset;
    __u16 min_io_size;
    __u32 opt_io_size;
    __u8 wce;
    __u8 unused;
    __u16 num_queues;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct virtio_blk_config {
    __u64 capacity;
    __u32 size_max;
    __u32 seg_max;
    struct virtio_blk_geometry geometry;
    __u32 blk_size;
    __u8 physical_block_exp;
    __u8 alignment_offset;
    __u16 min_io_size;
    __u32 opt_io_size;
    __u8 wce;
    __u8 unused;
    __u16 num_queues;
};
```
</details>
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
struct virtio_blk_config {
    __virtio64 capacity;
    __virtio32 size_max;
    __virtio32 seg_max;
    struct virtio_blk_geometry geometry;
    __virtio32 blk_size;
    __u8 physical_block_exp;
    __u8 alignment_offset;
    __virtio16 min_io_size;
    __virtio32 opt_io_size;
    __u8 wce;
    __u8 unused;
    __virtio16 num_queues;
    __virtio32 max_discard_sectors;
    __virtio32 max_discard_seg;
    __virtio32 discard_sector_alignment;
    __virtio32 max_write_zeroes_sectors;
    __virtio32 max_write_zeroes_seg;
    __u8 write_zeroes_may_unmap;
    __u8 unused1[3];
    __virtio32 max_secure_erase_sectors;
    __virtio32 max_secure_erase_seg;
    __virtio32 secure_erase_sector_alignment;
    struct virtio_blk_zoned_characteristics zoned;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct virtio_blk_config {
    __virtio64 capacity;
    __virtio32 size_max;
    __virtio32 seg_max;
    struct virtio_blk_geometry geometry;
    __virtio32 blk_size;
    __u8 physical_block_exp;
    __u8 alignment_offset;
    __virtio16 min_io_size;
    __virtio32 opt_io_size;
    __u8 wce;
    __u8 unused;
    __virtio16 num_queues;
    __virtio32 max_discard_sectors;
    __virtio32 max_discard_seg;
    __virtio32 discard_sector_alignment;
    __virtio32 max_write_zeroes_sectors;
    __virtio32 max_write_zeroes_seg;
    __u8 write_zeroes_may_unmap;
    __u8 unused1[3];
    __virtio32 max_secure_erase_sectors;
    __virtio32 max_secure_erase_seg;
    __virtio32 secure_erase_sector_alignment;
    struct virtio_blk_zoned_characteristics zoned;
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
No changes between <code>4.4</code> and <code>4.8</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
