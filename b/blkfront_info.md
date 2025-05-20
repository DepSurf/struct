# Struct: <code>blkfront_info</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct blkfront_info {
    spinlock_t io_lock;
    struct mutex mutex;
    struct xenbus_device *xbdev;
    struct gendisk *gd;
    int vdevice;
    blkif_vdev_t handle;
    enum blkif_state connected;
    int ring_ref[16];
    unsigned int nr_ring_pages;
    struct blkif_front_ring ring;
    unsigned int evtchn;
    unsigned int irq;
    struct request_queue *rq;
    struct work_struct work;
    struct gnttab_free_callback callback;
    struct blk_shadow shadow[512];
    struct list_head grants;
    struct list_head indirect_pages;
    unsigned int persistent_gnts_c;
    long unsigned int shadow_free;
    unsigned int feature_flush;
    unsigned int feature_discard;
    unsigned int feature_secdiscard;
    unsigned int discard_granularity;
    unsigned int discard_alignment;
    unsigned int feature_persistent;
    unsigned int max_indirect_segments;
    int is_ready;
    struct blk_mq_tag_set tag_set;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct blkfront_info {
    struct mutex mutex;
    struct xenbus_device *xbdev;
    struct gendisk *gd;
    u16 sector_size;
    unsigned int physical_sector_size;
    int vdevice;
    blkif_vdev_t handle;
    enum blkif_state connected;
    unsigned int nr_ring_pages;
    struct request_queue *rq;
    unsigned int feature_flush;
    unsigned int feature_fua;
    unsigned int feature_discard;
    unsigned int feature_secdiscard;
    unsigned int discard_granularity;
    unsigned int discard_alignment;
    unsigned int feature_persistent;
    unsigned int max_indirect_segments;
    int is_ready;
    struct blk_mq_tag_set tag_set;
    struct blkfront_ring_info *rinfo;
    unsigned int nr_rings;
    struct list_head requests;
    struct bio_list bio_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct blkfront_info {
    struct mutex mutex;
    struct xenbus_device *xbdev;
    struct gendisk *gd;
    u16 sector_size;
    unsigned int physical_sector_size;
    int vdevice;
    blkif_vdev_t handle;
    enum blkif_state connected;
    unsigned int nr_ring_pages;
    struct request_queue *rq;
    unsigned int feature_flush;
    unsigned int feature_fua;
    unsigned int feature_discard;
    unsigned int feature_secdiscard;
    unsigned int feature_persistent;
    unsigned int discard_granularity;
    unsigned int discard_alignment;
    unsigned int max_indirect_segments;
    int is_ready;
    struct blk_mq_tag_set tag_set;
    struct blkfront_ring_info *rinfo;
    unsigned int nr_rings;
    struct list_head requests;
    struct bio_list bio_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct blkfront_info {
    struct mutex mutex;
    struct xenbus_device *xbdev;
    struct gendisk *gd;
    u16 sector_size;
    unsigned int physical_sector_size;
    int vdevice;
    blkif_vdev_t handle;
    enum blkif_state connected;
    unsigned int nr_ring_pages;
    struct request_queue *rq;
    unsigned int feature_flush;
    unsigned int feature_fua;
    unsigned int feature_discard;
    unsigned int feature_secdiscard;
    unsigned int feature_persistent;
    unsigned int discard_granularity;
    unsigned int discard_alignment;
    unsigned int max_indirect_segments;
    int is_ready;
    struct blk_mq_tag_set tag_set;
    struct blkfront_ring_info *rinfo;
    unsigned int nr_rings;
    struct list_head requests;
    struct bio_list bio_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct blkfront_info {
    struct mutex mutex;
    struct xenbus_device *xbdev;
    struct gendisk *gd;
    u16 sector_size;
    unsigned int physical_sector_size;
    int vdevice;
    blkif_vdev_t handle;
    enum blkif_state connected;
    unsigned int nr_ring_pages;
    struct request_queue *rq;
    unsigned int feature_flush;
    unsigned int feature_fua;
    unsigned int feature_discard;
    unsigned int feature_secdiscard;
    unsigned int feature_persistent;
    unsigned int discard_granularity;
    unsigned int discard_alignment;
    unsigned int max_indirect_segments;
    int is_ready;
    struct blk_mq_tag_set tag_set;
    struct blkfront_ring_info *rinfo;
    unsigned int nr_rings;
    struct list_head requests;
    struct bio_list bio_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct blkfront_info {
    struct mutex mutex;
    struct xenbus_device *xbdev;
    struct gendisk *gd;
    u16 sector_size;
    unsigned int physical_sector_size;
    int vdevice;
    blkif_vdev_t handle;
    enum blkif_state connected;
    unsigned int nr_ring_pages;
    struct request_queue *rq;
    unsigned int feature_flush;
    unsigned int feature_fua;
    unsigned int feature_discard;
    unsigned int feature_secdiscard;
    unsigned int feature_persistent;
    unsigned int discard_granularity;
    unsigned int discard_alignment;
    unsigned int max_indirect_segments;
    int is_ready;
    struct blk_mq_tag_set tag_set;
    struct blkfront_ring_info *rinfo;
    unsigned int nr_rings;
    struct list_head requests;
    struct bio_list bio_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct blkfront_info {
    struct mutex mutex;
    struct xenbus_device *xbdev;
    struct gendisk *gd;
    u16 sector_size;
    unsigned int physical_sector_size;
    int vdevice;
    blkif_vdev_t handle;
    enum blkif_state connected;
    unsigned int nr_ring_pages;
    struct request_queue *rq;
    unsigned int feature_flush;
    unsigned int feature_fua;
    unsigned int feature_discard;
    unsigned int feature_secdiscard;
    unsigned int feature_persistent;
    unsigned int discard_granularity;
    unsigned int discard_alignment;
    unsigned int max_indirect_segments;
    int is_ready;
    struct blk_mq_tag_set tag_set;
    struct blkfront_ring_info *rinfo;
    unsigned int nr_rings;
    struct list_head requests;
    struct bio_list bio_list;
    struct list_head info_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct blkfront_info {
    struct mutex mutex;
    struct xenbus_device *xbdev;
    struct gendisk *gd;
    u16 sector_size;
    unsigned int physical_sector_size;
    int vdevice;
    blkif_vdev_t handle;
    enum blkif_state connected;
    unsigned int nr_ring_pages;
    struct request_queue *rq;
    unsigned int feature_flush;
    unsigned int feature_fua;
    unsigned int feature_discard;
    unsigned int feature_secdiscard;
    unsigned int feature_persistent;
    unsigned int discard_granularity;
    unsigned int discard_alignment;
    unsigned int max_indirect_segments;
    int is_ready;
    struct blk_mq_tag_set tag_set;
    struct blkfront_ring_info *rinfo;
    unsigned int nr_rings;
    struct list_head requests;
    struct bio_list bio_list;
    struct list_head info_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct blkfront_info {
    struct mutex mutex;
    struct xenbus_device *xbdev;
    struct gendisk *gd;
    u16 sector_size;
    unsigned int physical_sector_size;
    int vdevice;
    blkif_vdev_t handle;
    enum blkif_state connected;
    unsigned int nr_ring_pages;
    struct request_queue *rq;
    unsigned int feature_flush;
    unsigned int feature_fua;
    unsigned int feature_discard;
    unsigned int feature_secdiscard;
    unsigned int feature_persistent;
    unsigned int discard_granularity;
    unsigned int discard_alignment;
    unsigned int max_indirect_segments;
    int is_ready;
    struct blk_mq_tag_set tag_set;
    struct blkfront_ring_info *rinfo;
    unsigned int nr_rings;
    struct list_head requests;
    struct bio_list bio_list;
    struct list_head info_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct blkfront_info {
    struct mutex mutex;
    struct xenbus_device *xbdev;
    struct gendisk *gd;
    u16 sector_size;
    unsigned int physical_sector_size;
    int vdevice;
    blkif_vdev_t handle;
    enum blkif_state connected;
    unsigned int nr_ring_pages;
    struct request_queue *rq;
    unsigned int feature_flush;
    unsigned int feature_fua;
    unsigned int feature_discard;
    unsigned int feature_secdiscard;
    unsigned int feature_persistent;
    unsigned int discard_granularity;
    unsigned int discard_alignment;
    unsigned int max_indirect_segments;
    int is_ready;
    struct blk_mq_tag_set tag_set;
    struct blkfront_ring_info *rinfo;
    unsigned int nr_rings;
    unsigned int rinfo_size;
    struct list_head requests;
    struct bio_list bio_list;
    struct list_head info_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct blkfront_info {
    struct mutex mutex;
    struct xenbus_device *xbdev;
    struct gendisk *gd;
    u16 sector_size;
    unsigned int physical_sector_size;
    int vdevice;
    blkif_vdev_t handle;
    enum blkif_state connected;
    unsigned int nr_ring_pages;
    struct request_queue *rq;
    unsigned int feature_flush;
    unsigned int feature_fua;
    unsigned int feature_discard;
    unsigned int feature_secdiscard;
    unsigned int feature_persistent;
    unsigned int discard_granularity;
    unsigned int discard_alignment;
    unsigned int max_indirect_segments;
    int is_ready;
    struct blk_mq_tag_set tag_set;
    struct blkfront_ring_info *rinfo;
    unsigned int nr_rings;
    unsigned int rinfo_size;
    struct list_head requests;
    struct bio_list bio_list;
    struct list_head info_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct blkfront_info {
    struct mutex mutex;
    struct xenbus_device *xbdev;
    struct gendisk *gd;
    u16 sector_size;
    unsigned int physical_sector_size;
    int vdevice;
    blkif_vdev_t handle;
    enum blkif_state connected;
    unsigned int nr_ring_pages;
    struct request_queue *rq;
    unsigned int feature_flush;
    unsigned int feature_fua;
    unsigned int feature_discard;
    unsigned int feature_secdiscard;
    unsigned int feature_persistent;
    unsigned int discard_granularity;
    unsigned int discard_alignment;
    unsigned int max_indirect_segments;
    int is_ready;
    struct blk_mq_tag_set tag_set;
    struct blkfront_ring_info *rinfo;
    unsigned int nr_rings;
    unsigned int rinfo_size;
    struct list_head requests;
    struct bio_list bio_list;
    struct list_head info_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct blkfront_info {
    struct mutex mutex;
    struct xenbus_device *xbdev;
    struct gendisk *gd;
    u16 sector_size;
    unsigned int physical_sector_size;
    int vdevice;
    blkif_vdev_t handle;
    enum blkif_state connected;
    unsigned int nr_ring_pages;
    struct request_queue *rq;
    unsigned int feature_flush;
    unsigned int feature_fua;
    unsigned int feature_discard;
    unsigned int feature_secdiscard;
    unsigned int feature_persistent;
    unsigned int discard_granularity;
    unsigned int discard_alignment;
    unsigned int max_indirect_segments;
    int is_ready;
    struct blk_mq_tag_set tag_set;
    struct blkfront_ring_info *rinfo;
    unsigned int nr_rings;
    unsigned int rinfo_size;
    struct list_head requests;
    struct bio_list bio_list;
    struct list_head info_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct blkfront_info {
    struct mutex mutex;
    struct xenbus_device *xbdev;
    struct gendisk *gd;
    u16 sector_size;
    unsigned int physical_sector_size;
    long unsigned int vdisk_info;
    int vdevice;
    blkif_vdev_t handle;
    enum blkif_state connected;
    unsigned int nr_ring_pages;
    struct request_queue *rq;
    unsigned int feature_flush;
    unsigned int feature_fua;
    unsigned int feature_discard;
    unsigned int feature_secdiscard;
    unsigned int feature_persistent;
    unsigned int bounce;
    unsigned int discard_granularity;
    unsigned int discard_alignment;
    unsigned int max_indirect_segments;
    int is_ready;
    struct blk_mq_tag_set tag_set;
    struct blkfront_ring_info *rinfo;
    unsigned int nr_rings;
    unsigned int rinfo_size;
    struct list_head requests;
    struct bio_list bio_list;
    struct list_head info_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct blkfront_info {
    struct mutex mutex;
    struct xenbus_device *xbdev;
    struct gendisk *gd;
    u16 sector_size;
    unsigned int physical_sector_size;
    long unsigned int vdisk_info;
    int vdevice;
    blkif_vdev_t handle;
    enum blkif_state connected;
    unsigned int nr_ring_pages;
    struct request_queue *rq;
    unsigned int feature_flush;
    unsigned int feature_fua;
    unsigned int feature_discard;
    unsigned int feature_secdiscard;
    unsigned int feature_persistent_parm;
    unsigned int feature_persistent;
    unsigned int bounce;
    unsigned int discard_granularity;
    unsigned int discard_alignment;
    unsigned int max_indirect_segments;
    int is_ready;
    struct blk_mq_tag_set tag_set;
    struct blkfront_ring_info *rinfo;
    unsigned int nr_rings;
    unsigned int rinfo_size;
    struct list_head requests;
    struct bio_list bio_list;
    struct list_head info_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct blkfront_info {
    struct mutex mutex;
    struct xenbus_device *xbdev;
    struct gendisk *gd;
    u16 sector_size;
    unsigned int physical_sector_size;
    long unsigned int vdisk_info;
    int vdevice;
    blkif_vdev_t handle;
    enum blkif_state connected;
    unsigned int nr_ring_pages;
    struct request_queue *rq;
    unsigned int feature_flush;
    unsigned int feature_fua;
    unsigned int feature_discard;
    unsigned int feature_secdiscard;
    unsigned int feature_persistent_parm;
    unsigned int feature_persistent;
    unsigned int bounce;
    unsigned int discard_granularity;
    unsigned int discard_alignment;
    unsigned int max_indirect_segments;
    int is_ready;
    struct blk_mq_tag_set tag_set;
    struct blkfront_ring_info *rinfo;
    unsigned int nr_rings;
    unsigned int rinfo_size;
    struct list_head requests;
    struct bio_list bio_list;
    struct list_head info_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct blkfront_info {
    struct mutex mutex;
    struct xenbus_device *xbdev;
    struct gendisk *gd;
    u16 sector_size;
    unsigned int physical_sector_size;
    long unsigned int vdisk_info;
    int vdevice;
    blkif_vdev_t handle;
    enum blkif_state connected;
    unsigned int nr_ring_pages;
    struct request_queue *rq;
    unsigned int feature_flush;
    unsigned int feature_fua;
    unsigned int feature_discard;
    unsigned int feature_secdiscard;
    unsigned int feature_persistent_parm;
    unsigned int feature_persistent;
    unsigned int bounce;
    unsigned int discard_granularity;
    unsigned int discard_alignment;
    unsigned int max_indirect_segments;
    int is_ready;
    struct blk_mq_tag_set tag_set;
    struct blkfront_ring_info *rinfo;
    unsigned int nr_rings;
    unsigned int rinfo_size;
    struct list_head requests;
    struct bio_list bio_list;
    struct list_head info_list;
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
struct blkfront_info {
    struct mutex mutex;
    struct xenbus_device *xbdev;
    struct gendisk *gd;
    u16 sector_size;
    unsigned int physical_sector_size;
    int vdevice;
    blkif_vdev_t handle;
    enum blkif_state connected;
    unsigned int nr_ring_pages;
    struct request_queue *rq;
    unsigned int feature_flush;
    unsigned int feature_fua;
    unsigned int feature_discard;
    unsigned int feature_secdiscard;
    unsigned int feature_persistent;
    unsigned int discard_granularity;
    unsigned int discard_alignment;
    unsigned int max_indirect_segments;
    int is_ready;
    struct blk_mq_tag_set tag_set;
    struct blkfront_ring_info *rinfo;
    unsigned int nr_rings;
    struct list_head requests;
    struct bio_list bio_list;
    struct list_head info_list;
};
```
</details>
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
struct blkfront_info {
    struct mutex mutex;
    struct xenbus_device *xbdev;
    struct gendisk *gd;
    u16 sector_size;
    unsigned int physical_sector_size;
    int vdevice;
    blkif_vdev_t handle;
    enum blkif_state connected;
    unsigned int nr_ring_pages;
    struct request_queue *rq;
    unsigned int feature_flush;
    unsigned int feature_fua;
    unsigned int feature_discard;
    unsigned int feature_secdiscard;
    unsigned int feature_persistent;
    unsigned int discard_granularity;
    unsigned int discard_alignment;
    unsigned int max_indirect_segments;
    int is_ready;
    struct blk_mq_tag_set tag_set;
    struct blkfront_ring_info *rinfo;
    unsigned int nr_rings;
    struct list_head requests;
    struct bio_list bio_list;
    struct list_head info_list;
    struct completion wait_backend_disconnected;
};
```
</details>
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct blkfront_info {
    struct mutex mutex;
    struct xenbus_device *xbdev;
    struct gendisk *gd;
    u16 sector_size;
    unsigned int physical_sector_size;
    int vdevice;
    blkif_vdev_t handle;
    enum blkif_state connected;
    unsigned int nr_ring_pages;
    struct request_queue *rq;
    unsigned int feature_flush;
    unsigned int feature_fua;
    unsigned int feature_discard;
    unsigned int feature_secdiscard;
    unsigned int feature_persistent;
    unsigned int discard_granularity;
    unsigned int discard_alignment;
    unsigned int max_indirect_segments;
    int is_ready;
    struct blk_mq_tag_set tag_set;
    struct blkfront_ring_info *rinfo;
    unsigned int nr_rings;
    struct list_head requests;
    struct bio_list bio_list;
    struct list_head info_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct blkfront_info {
    struct mutex mutex;
    struct xenbus_device *xbdev;
    struct gendisk *gd;
    u16 sector_size;
    unsigned int physical_sector_size;
    int vdevice;
    blkif_vdev_t handle;
    enum blkif_state connected;
    unsigned int nr_ring_pages;
    struct request_queue *rq;
    unsigned int feature_flush;
    unsigned int feature_fua;
    unsigned int feature_discard;
    unsigned int feature_secdiscard;
    unsigned int feature_persistent;
    unsigned int discard_granularity;
    unsigned int discard_alignment;
    unsigned int max_indirect_segments;
    int is_ready;
    struct blk_mq_tag_set tag_set;
    struct blkfront_ring_info *rinfo;
    unsigned int nr_rings;
    struct list_head requests;
    struct bio_list bio_list;
    struct list_head info_list;
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
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 sector_size</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int physical_sector_size</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int feature_fua</code>
</li>
<li>
<b>Field added. </b>
<code>struct blkfront_ring_info *rinfo</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int nr_rings</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head requests</code>
</li>
<li>
<b>Field added. </b>
<code>struct bio_list bio_list</code>
</li>
<li>
<b>Field removed. </b>
<code>spinlock_t io_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>int ring_ref[16]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct blkif_front_ring ring</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int evtchn</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int irq</code>
</li>
<li>
<b>Field removed. </b>
<code>struct work_struct work</code>
</li>
<li>
<b>Field removed. </b>
<code>struct gnttab_free_callback callback</code>
</li>
<li>
<b>Field removed. </b>
<code>struct blk_shadow shadow[512]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head grants</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head indirect_pages</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int persistent_gnts_c</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int shadow_free</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head info_list</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int rinfo_size</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
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
<code>long unsigned int vdisk_info</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int bounce</code>
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
<code>unsigned int feature_persistent_parm</code>
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
</ul>
<b>Flavor</b>
<ul>
<li>
<details>
<summary>Changed between <code>generic</code> and <code>aws</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct completion wait_backend_disconnected</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
