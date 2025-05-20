# Struct: <code>md_cluster_operations</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct md_cluster_operations {
    int (*join)(struct mddev *, int);
    int (*leave)(struct mddev *);
    int (*slot_number)(struct mddev *);
    int (*resync_info_update)(struct mddev *, sector_t, sector_t);
    int (*metadata_update_start)(struct mddev *);
    int (*metadata_update_finish)(struct mddev *);
    void (*metadata_update_cancel)(struct mddev *);
    int (*resync_start)(struct mddev *);
    int (*resync_finish)(struct mddev *);
    int (*area_resyncing)(struct mddev *, int, sector_t, sector_t);
    int (*add_new_disk)(struct mddev *, struct md_rdev *);
    void (*add_new_disk_cancel)(struct mddev *);
    int (*new_disk_ack)(struct mddev *, bool);
    int (*remove_disk)(struct mddev *, struct md_rdev *);
    int (*gather_bitmaps)(struct md_rdev *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct md_cluster_operations {
    int (*join)(struct mddev *, int);
    int (*leave)(struct mddev *);
    int (*slot_number)(struct mddev *);
    int (*resync_info_update)(struct mddev *, sector_t, sector_t);
    int (*metadata_update_start)(struct mddev *);
    int (*metadata_update_finish)(struct mddev *);
    void (*metadata_update_cancel)(struct mddev *);
    int (*resync_start)(struct mddev *);
    int (*resync_finish)(struct mddev *);
    int (*area_resyncing)(struct mddev *, int, sector_t, sector_t);
    int (*add_new_disk)(struct mddev *, struct md_rdev *);
    void (*add_new_disk_cancel)(struct mddev *);
    int (*new_disk_ack)(struct mddev *, bool);
    int (*remove_disk)(struct mddev *, struct md_rdev *);
    void (*load_bitmaps)(struct mddev *, int);
    int (*gather_bitmaps)(struct md_rdev *);
    int (*lock_all_bitmaps)(struct mddev *);
    void (*unlock_all_bitmaps)(struct mddev *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct md_cluster_operations {
    int (*join)(struct mddev *, int);
    int (*leave)(struct mddev *);
    int (*slot_number)(struct mddev *);
    int (*resync_info_update)(struct mddev *, sector_t, sector_t);
    int (*metadata_update_start)(struct mddev *);
    int (*metadata_update_finish)(struct mddev *);
    void (*metadata_update_cancel)(struct mddev *);
    int (*resync_start)(struct mddev *);
    int (*resync_finish)(struct mddev *);
    int (*area_resyncing)(struct mddev *, int, sector_t, sector_t);
    int (*add_new_disk)(struct mddev *, struct md_rdev *);
    void (*add_new_disk_cancel)(struct mddev *);
    int (*new_disk_ack)(struct mddev *, bool);
    int (*remove_disk)(struct mddev *, struct md_rdev *);
    void (*load_bitmaps)(struct mddev *, int);
    int (*gather_bitmaps)(struct md_rdev *);
    int (*lock_all_bitmaps)(struct mddev *);
    void (*unlock_all_bitmaps)(struct mddev *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct md_cluster_operations {
    int (*join)(struct mddev *, int);
    int (*leave)(struct mddev *);
    int (*slot_number)(struct mddev *);
    int (*resync_info_update)(struct mddev *, sector_t, sector_t);
    int (*metadata_update_start)(struct mddev *);
    int (*metadata_update_finish)(struct mddev *);
    void (*metadata_update_cancel)(struct mddev *);
    int (*resync_start)(struct mddev *);
    int (*resync_finish)(struct mddev *);
    int (*area_resyncing)(struct mddev *, int, sector_t, sector_t);
    int (*add_new_disk)(struct mddev *, struct md_rdev *);
    void (*add_new_disk_cancel)(struct mddev *);
    int (*new_disk_ack)(struct mddev *, bool);
    int (*remove_disk)(struct mddev *, struct md_rdev *);
    void (*load_bitmaps)(struct mddev *, int);
    int (*gather_bitmaps)(struct md_rdev *);
    int (*lock_all_bitmaps)(struct mddev *);
    void (*unlock_all_bitmaps)(struct mddev *);
    void (*update_size)(struct mddev *, sector_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct md_cluster_operations {
    int (*join)(struct mddev *, int);
    int (*leave)(struct mddev *);
    int (*slot_number)(struct mddev *);
    int (*resync_info_update)(struct mddev *, sector_t, sector_t);
    int (*metadata_update_start)(struct mddev *);
    int (*metadata_update_finish)(struct mddev *);
    void (*metadata_update_cancel)(struct mddev *);
    int (*resync_start)(struct mddev *);
    int (*resync_finish)(struct mddev *);
    int (*area_resyncing)(struct mddev *, int, sector_t, sector_t);
    int (*add_new_disk)(struct mddev *, struct md_rdev *);
    void (*add_new_disk_cancel)(struct mddev *);
    int (*new_disk_ack)(struct mddev *, bool);
    int (*remove_disk)(struct mddev *, struct md_rdev *);
    void (*load_bitmaps)(struct mddev *, int);
    int (*gather_bitmaps)(struct md_rdev *);
    int (*lock_all_bitmaps)(struct mddev *);
    void (*unlock_all_bitmaps)(struct mddev *);
    void (*update_size)(struct mddev *, sector_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct md_cluster_operations {
    int (*join)(struct mddev *, int);
    int (*leave)(struct mddev *);
    int (*slot_number)(struct mddev *);
    int (*resync_info_update)(struct mddev *, sector_t, sector_t);
    int (*metadata_update_start)(struct mddev *);
    int (*metadata_update_finish)(struct mddev *);
    void (*metadata_update_cancel)(struct mddev *);
    int (*resync_start)(struct mddev *);
    int (*resync_finish)(struct mddev *);
    int (*area_resyncing)(struct mddev *, int, sector_t, sector_t);
    int (*add_new_disk)(struct mddev *, struct md_rdev *);
    void (*add_new_disk_cancel)(struct mddev *);
    int (*new_disk_ack)(struct mddev *, bool);
    int (*remove_disk)(struct mddev *, struct md_rdev *);
    void (*load_bitmaps)(struct mddev *, int);
    int (*gather_bitmaps)(struct md_rdev *);
    int (*lock_all_bitmaps)(struct mddev *);
    void (*unlock_all_bitmaps)(struct mddev *);
    void (*update_size)(struct mddev *, sector_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct md_cluster_operations {
    int (*join)(struct mddev *, int);
    int (*leave)(struct mddev *);
    int (*slot_number)(struct mddev *);
    int (*resync_info_update)(struct mddev *, sector_t, sector_t);
    void (*resync_info_get)(struct mddev *, sector_t *, sector_t *);
    int (*metadata_update_start)(struct mddev *);
    int (*metadata_update_finish)(struct mddev *);
    void (*metadata_update_cancel)(struct mddev *);
    int (*resync_start)(struct mddev *);
    int (*resync_finish)(struct mddev *);
    int (*area_resyncing)(struct mddev *, int, sector_t, sector_t);
    int (*add_new_disk)(struct mddev *, struct md_rdev *);
    void (*add_new_disk_cancel)(struct mddev *);
    int (*new_disk_ack)(struct mddev *, bool);
    int (*remove_disk)(struct mddev *, struct md_rdev *);
    void (*load_bitmaps)(struct mddev *, int);
    int (*gather_bitmaps)(struct md_rdev *);
    int (*resize_bitmaps)(struct mddev *, sector_t, sector_t);
    int (*lock_all_bitmaps)(struct mddev *);
    void (*unlock_all_bitmaps)(struct mddev *);
    void (*update_size)(struct mddev *, sector_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct md_cluster_operations {
    int (*join)(struct mddev *, int);
    int (*leave)(struct mddev *);
    int (*slot_number)(struct mddev *);
    int (*resync_info_update)(struct mddev *, sector_t, sector_t);
    void (*resync_info_get)(struct mddev *, sector_t *, sector_t *);
    int (*metadata_update_start)(struct mddev *);
    int (*metadata_update_finish)(struct mddev *);
    void (*metadata_update_cancel)(struct mddev *);
    int (*resync_start)(struct mddev *);
    int (*resync_finish)(struct mddev *);
    int (*area_resyncing)(struct mddev *, int, sector_t, sector_t);
    int (*add_new_disk)(struct mddev *, struct md_rdev *);
    void (*add_new_disk_cancel)(struct mddev *);
    int (*new_disk_ack)(struct mddev *, bool);
    int (*remove_disk)(struct mddev *, struct md_rdev *);
    void (*load_bitmaps)(struct mddev *, int);
    int (*gather_bitmaps)(struct md_rdev *);
    int (*resize_bitmaps)(struct mddev *, sector_t, sector_t);
    int (*lock_all_bitmaps)(struct mddev *);
    void (*unlock_all_bitmaps)(struct mddev *);
    void (*update_size)(struct mddev *, sector_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct md_cluster_operations {
    int (*join)(struct mddev *, int);
    int (*leave)(struct mddev *);
    int (*slot_number)(struct mddev *);
    int (*resync_info_update)(struct mddev *, sector_t, sector_t);
    void (*resync_info_get)(struct mddev *, sector_t *, sector_t *);
    int (*metadata_update_start)(struct mddev *);
    int (*metadata_update_finish)(struct mddev *);
    void (*metadata_update_cancel)(struct mddev *);
    int (*resync_start)(struct mddev *);
    int (*resync_finish)(struct mddev *);
    int (*area_resyncing)(struct mddev *, int, sector_t, sector_t);
    int (*add_new_disk)(struct mddev *, struct md_rdev *);
    void (*add_new_disk_cancel)(struct mddev *);
    int (*new_disk_ack)(struct mddev *, bool);
    int (*remove_disk)(struct mddev *, struct md_rdev *);
    void (*load_bitmaps)(struct mddev *, int);
    int (*gather_bitmaps)(struct md_rdev *);
    int (*resize_bitmaps)(struct mddev *, sector_t, sector_t);
    int (*lock_all_bitmaps)(struct mddev *);
    void (*unlock_all_bitmaps)(struct mddev *);
    void (*update_size)(struct mddev *, sector_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct md_cluster_operations {
    int (*join)(struct mddev *, int);
    int (*leave)(struct mddev *);
    int (*slot_number)(struct mddev *);
    int (*resync_info_update)(struct mddev *, sector_t, sector_t);
    void (*resync_info_get)(struct mddev *, sector_t *, sector_t *);
    int (*metadata_update_start)(struct mddev *);
    int (*metadata_update_finish)(struct mddev *);
    void (*metadata_update_cancel)(struct mddev *);
    int (*resync_start)(struct mddev *);
    int (*resync_finish)(struct mddev *);
    int (*area_resyncing)(struct mddev *, int, sector_t, sector_t);
    int (*add_new_disk)(struct mddev *, struct md_rdev *);
    void (*add_new_disk_cancel)(struct mddev *);
    int (*new_disk_ack)(struct mddev *, bool);
    int (*remove_disk)(struct mddev *, struct md_rdev *);
    void (*load_bitmaps)(struct mddev *, int);
    int (*gather_bitmaps)(struct md_rdev *);
    int (*resize_bitmaps)(struct mddev *, sector_t, sector_t);
    int (*lock_all_bitmaps)(struct mddev *);
    void (*unlock_all_bitmaps)(struct mddev *);
    void (*update_size)(struct mddev *, sector_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct md_cluster_operations {
    int (*join)(struct mddev *, int);
    int (*leave)(struct mddev *);
    int (*slot_number)(struct mddev *);
    int (*resync_info_update)(struct mddev *, sector_t, sector_t);
    void (*resync_info_get)(struct mddev *, sector_t *, sector_t *);
    int (*metadata_update_start)(struct mddev *);
    int (*metadata_update_finish)(struct mddev *);
    void (*metadata_update_cancel)(struct mddev *);
    int (*resync_start)(struct mddev *);
    int (*resync_finish)(struct mddev *);
    int (*area_resyncing)(struct mddev *, int, sector_t, sector_t);
    int (*add_new_disk)(struct mddev *, struct md_rdev *);
    void (*add_new_disk_cancel)(struct mddev *);
    int (*new_disk_ack)(struct mddev *, bool);
    int (*remove_disk)(struct mddev *, struct md_rdev *);
    void (*load_bitmaps)(struct mddev *, int);
    int (*gather_bitmaps)(struct md_rdev *);
    int (*resize_bitmaps)(struct mddev *, sector_t, sector_t);
    int (*lock_all_bitmaps)(struct mddev *);
    void (*unlock_all_bitmaps)(struct mddev *);
    void (*update_size)(struct mddev *, sector_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct md_cluster_operations {
    int (*join)(struct mddev *, int);
    int (*leave)(struct mddev *);
    int (*slot_number)(struct mddev *);
    int (*resync_info_update)(struct mddev *, sector_t, sector_t);
    void (*resync_info_get)(struct mddev *, sector_t *, sector_t *);
    int (*metadata_update_start)(struct mddev *);
    int (*metadata_update_finish)(struct mddev *);
    void (*metadata_update_cancel)(struct mddev *);
    int (*resync_start)(struct mddev *);
    int (*resync_finish)(struct mddev *);
    int (*area_resyncing)(struct mddev *, int, sector_t, sector_t);
    int (*add_new_disk)(struct mddev *, struct md_rdev *);
    void (*add_new_disk_cancel)(struct mddev *);
    int (*new_disk_ack)(struct mddev *, bool);
    int (*remove_disk)(struct mddev *, struct md_rdev *);
    void (*load_bitmaps)(struct mddev *, int);
    int (*gather_bitmaps)(struct md_rdev *);
    int (*resize_bitmaps)(struct mddev *, sector_t, sector_t);
    int (*lock_all_bitmaps)(struct mddev *);
    void (*unlock_all_bitmaps)(struct mddev *);
    void (*update_size)(struct mddev *, sector_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct md_cluster_operations {
    int (*join)(struct mddev *, int);
    int (*leave)(struct mddev *);
    int (*slot_number)(struct mddev *);
    int (*resync_info_update)(struct mddev *, sector_t, sector_t);
    void (*resync_info_get)(struct mddev *, sector_t *, sector_t *);
    int (*metadata_update_start)(struct mddev *);
    int (*metadata_update_finish)(struct mddev *);
    void (*metadata_update_cancel)(struct mddev *);
    int (*resync_start)(struct mddev *);
    int (*resync_finish)(struct mddev *);
    int (*area_resyncing)(struct mddev *, int, sector_t, sector_t);
    int (*add_new_disk)(struct mddev *, struct md_rdev *);
    void (*add_new_disk_cancel)(struct mddev *);
    int (*new_disk_ack)(struct mddev *, bool);
    int (*remove_disk)(struct mddev *, struct md_rdev *);
    void (*load_bitmaps)(struct mddev *, int);
    int (*gather_bitmaps)(struct md_rdev *);
    int (*resize_bitmaps)(struct mddev *, sector_t, sector_t);
    int (*lock_all_bitmaps)(struct mddev *);
    void (*unlock_all_bitmaps)(struct mddev *);
    void (*update_size)(struct mddev *, sector_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct md_cluster_operations {
    int (*join)(struct mddev *, int);
    int (*leave)(struct mddev *);
    int (*slot_number)(struct mddev *);
    int (*resync_info_update)(struct mddev *, sector_t, sector_t);
    void (*resync_info_get)(struct mddev *, sector_t *, sector_t *);
    int (*metadata_update_start)(struct mddev *);
    int (*metadata_update_finish)(struct mddev *);
    void (*metadata_update_cancel)(struct mddev *);
    int (*resync_start)(struct mddev *);
    int (*resync_finish)(struct mddev *);
    int (*area_resyncing)(struct mddev *, int, sector_t, sector_t);
    int (*add_new_disk)(struct mddev *, struct md_rdev *);
    void (*add_new_disk_cancel)(struct mddev *);
    int (*new_disk_ack)(struct mddev *, bool);
    int (*remove_disk)(struct mddev *, struct md_rdev *);
    void (*load_bitmaps)(struct mddev *, int);
    int (*gather_bitmaps)(struct md_rdev *);
    int (*resize_bitmaps)(struct mddev *, sector_t, sector_t);
    int (*lock_all_bitmaps)(struct mddev *);
    void (*unlock_all_bitmaps)(struct mddev *);
    void (*update_size)(struct mddev *, sector_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct md_cluster_operations {
    int (*join)(struct mddev *, int);
    int (*leave)(struct mddev *);
    int (*slot_number)(struct mddev *);
    int (*resync_info_update)(struct mddev *, sector_t, sector_t);
    void (*resync_info_get)(struct mddev *, sector_t *, sector_t *);
    int (*metadata_update_start)(struct mddev *);
    int (*metadata_update_finish)(struct mddev *);
    void (*metadata_update_cancel)(struct mddev *);
    int (*resync_start)(struct mddev *);
    int (*resync_finish)(struct mddev *);
    int (*area_resyncing)(struct mddev *, int, sector_t, sector_t);
    int (*add_new_disk)(struct mddev *, struct md_rdev *);
    void (*add_new_disk_cancel)(struct mddev *);
    int (*new_disk_ack)(struct mddev *, bool);
    int (*remove_disk)(struct mddev *, struct md_rdev *);
    void (*load_bitmaps)(struct mddev *, int);
    int (*gather_bitmaps)(struct md_rdev *);
    int (*resize_bitmaps)(struct mddev *, sector_t, sector_t);
    int (*lock_all_bitmaps)(struct mddev *);
    void (*unlock_all_bitmaps)(struct mddev *);
    void (*update_size)(struct mddev *, sector_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct md_cluster_operations {
    int (*join)(struct mddev *, int);
    int (*leave)(struct mddev *);
    int (*slot_number)(struct mddev *);
    int (*resync_info_update)(struct mddev *, sector_t, sector_t);
    void (*resync_info_get)(struct mddev *, sector_t *, sector_t *);
    int (*metadata_update_start)(struct mddev *);
    int (*metadata_update_finish)(struct mddev *);
    void (*metadata_update_cancel)(struct mddev *);
    int (*resync_start)(struct mddev *);
    int (*resync_finish)(struct mddev *);
    int (*area_resyncing)(struct mddev *, int, sector_t, sector_t);
    int (*add_new_disk)(struct mddev *, struct md_rdev *);
    void (*add_new_disk_cancel)(struct mddev *);
    int (*new_disk_ack)(struct mddev *, bool);
    int (*remove_disk)(struct mddev *, struct md_rdev *);
    void (*load_bitmaps)(struct mddev *, int);
    int (*gather_bitmaps)(struct md_rdev *);
    int (*resize_bitmaps)(struct mddev *, sector_t, sector_t);
    int (*lock_all_bitmaps)(struct mddev *);
    void (*unlock_all_bitmaps)(struct mddev *);
    void (*update_size)(struct mddev *, sector_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct md_cluster_operations {
    int (*join)(struct mddev *, int);
    int (*leave)(struct mddev *);
    int (*slot_number)(struct mddev *);
    int (*resync_info_update)(struct mddev *, sector_t, sector_t);
    void (*resync_info_get)(struct mddev *, sector_t *, sector_t *);
    int (*metadata_update_start)(struct mddev *);
    int (*metadata_update_finish)(struct mddev *);
    void (*metadata_update_cancel)(struct mddev *);
    int (*resync_start)(struct mddev *);
    int (*resync_finish)(struct mddev *);
    int (*area_resyncing)(struct mddev *, int, sector_t, sector_t);
    int (*add_new_disk)(struct mddev *, struct md_rdev *);
    void (*add_new_disk_cancel)(struct mddev *);
    int (*new_disk_ack)(struct mddev *, bool);
    int (*remove_disk)(struct mddev *, struct md_rdev *);
    void (*load_bitmaps)(struct mddev *, int);
    int (*gather_bitmaps)(struct md_rdev *);
    int (*resize_bitmaps)(struct mddev *, sector_t, sector_t);
    int (*lock_all_bitmaps)(struct mddev *);
    void (*unlock_all_bitmaps)(struct mddev *);
    void (*update_size)(struct mddev *, sector_t);
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
struct md_cluster_operations {
    int (*join)(struct mddev *, int);
    int (*leave)(struct mddev *);
    int (*slot_number)(struct mddev *);
    int (*resync_info_update)(struct mddev *, sector_t, sector_t);
    void (*resync_info_get)(struct mddev *, sector_t *, sector_t *);
    int (*metadata_update_start)(struct mddev *);
    int (*metadata_update_finish)(struct mddev *);
    void (*metadata_update_cancel)(struct mddev *);
    int (*resync_start)(struct mddev *);
    int (*resync_finish)(struct mddev *);
    int (*area_resyncing)(struct mddev *, int, sector_t, sector_t);
    int (*add_new_disk)(struct mddev *, struct md_rdev *);
    void (*add_new_disk_cancel)(struct mddev *);
    int (*new_disk_ack)(struct mddev *, bool);
    int (*remove_disk)(struct mddev *, struct md_rdev *);
    void (*load_bitmaps)(struct mddev *, int);
    int (*gather_bitmaps)(struct md_rdev *);
    int (*resize_bitmaps)(struct mddev *, sector_t, sector_t);
    int (*lock_all_bitmaps)(struct mddev *);
    void (*unlock_all_bitmaps)(struct mddev *);
    void (*update_size)(struct mddev *, sector_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct md_cluster_operations {
    int (*join)(struct mddev *, int);
    int (*leave)(struct mddev *);
    int (*slot_number)(struct mddev *);
    int (*resync_info_update)(struct mddev *, sector_t, sector_t);
    void (*resync_info_get)(struct mddev *, sector_t *, sector_t *);
    int (*metadata_update_start)(struct mddev *);
    int (*metadata_update_finish)(struct mddev *);
    void (*metadata_update_cancel)(struct mddev *);
    int (*resync_start)(struct mddev *);
    int (*resync_finish)(struct mddev *);
    int (*area_resyncing)(struct mddev *, int, sector_t, sector_t);
    int (*add_new_disk)(struct mddev *, struct md_rdev *);
    void (*add_new_disk_cancel)(struct mddev *);
    int (*new_disk_ack)(struct mddev *, bool);
    int (*remove_disk)(struct mddev *, struct md_rdev *);
    void (*load_bitmaps)(struct mddev *, int);
    int (*gather_bitmaps)(struct md_rdev *);
    int (*resize_bitmaps)(struct mddev *, sector_t, sector_t);
    int (*lock_all_bitmaps)(struct mddev *);
    void (*unlock_all_bitmaps)(struct mddev *);
    void (*update_size)(struct mddev *, sector_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct md_cluster_operations {
    int (*join)(struct mddev *, int);
    int (*leave)(struct mddev *);
    int (*slot_number)(struct mddev *);
    int (*resync_info_update)(struct mddev *, sector_t, sector_t);
    void (*resync_info_get)(struct mddev *, sector_t *, sector_t *);
    int (*metadata_update_start)(struct mddev *);
    int (*metadata_update_finish)(struct mddev *);
    void (*metadata_update_cancel)(struct mddev *);
    int (*resync_start)(struct mddev *);
    int (*resync_finish)(struct mddev *);
    int (*area_resyncing)(struct mddev *, int, sector_t, sector_t);
    int (*add_new_disk)(struct mddev *, struct md_rdev *);
    void (*add_new_disk_cancel)(struct mddev *);
    int (*new_disk_ack)(struct mddev *, bool);
    int (*remove_disk)(struct mddev *, struct md_rdev *);
    void (*load_bitmaps)(struct mddev *, int);
    int (*gather_bitmaps)(struct md_rdev *);
    int (*resize_bitmaps)(struct mddev *, sector_t, sector_t);
    int (*lock_all_bitmaps)(struct mddev *);
    void (*unlock_all_bitmaps)(struct mddev *);
    void (*update_size)(struct mddev *, sector_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct md_cluster_operations {
    int (*join)(struct mddev *, int);
    int (*leave)(struct mddev *);
    int (*slot_number)(struct mddev *);
    int (*resync_info_update)(struct mddev *, sector_t, sector_t);
    void (*resync_info_get)(struct mddev *, sector_t *, sector_t *);
    int (*metadata_update_start)(struct mddev *);
    int (*metadata_update_finish)(struct mddev *);
    void (*metadata_update_cancel)(struct mddev *);
    int (*resync_start)(struct mddev *);
    int (*resync_finish)(struct mddev *);
    int (*area_resyncing)(struct mddev *, int, sector_t, sector_t);
    int (*add_new_disk)(struct mddev *, struct md_rdev *);
    void (*add_new_disk_cancel)(struct mddev *);
    int (*new_disk_ack)(struct mddev *, bool);
    int (*remove_disk)(struct mddev *, struct md_rdev *);
    void (*load_bitmaps)(struct mddev *, int);
    int (*gather_bitmaps)(struct md_rdev *);
    int (*resize_bitmaps)(struct mddev *, sector_t, sector_t);
    int (*lock_all_bitmaps)(struct mddev *);
    void (*unlock_all_bitmaps)(struct mddev *);
    void (*update_size)(struct mddev *, sector_t);
};
```
</details>
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct md_cluster_operations {
    int (*join)(struct mddev *, int);
    int (*leave)(struct mddev *);
    int (*slot_number)(struct mddev *);
    int (*resync_info_update)(struct mddev *, sector_t, sector_t);
    void (*resync_info_get)(struct mddev *, sector_t *, sector_t *);
    int (*metadata_update_start)(struct mddev *);
    int (*metadata_update_finish)(struct mddev *);
    void (*metadata_update_cancel)(struct mddev *);
    int (*resync_start)(struct mddev *);
    int (*resync_finish)(struct mddev *);
    int (*area_resyncing)(struct mddev *, int, sector_t, sector_t);
    int (*add_new_disk)(struct mddev *, struct md_rdev *);
    void (*add_new_disk_cancel)(struct mddev *);
    int (*new_disk_ack)(struct mddev *, bool);
    int (*remove_disk)(struct mddev *, struct md_rdev *);
    void (*load_bitmaps)(struct mddev *, int);
    int (*gather_bitmaps)(struct md_rdev *);
    int (*resize_bitmaps)(struct mddev *, sector_t, sector_t);
    int (*lock_all_bitmaps)(struct mddev *);
    void (*unlock_all_bitmaps)(struct mddev *);
    void (*update_size)(struct mddev *, sector_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct md_cluster_operations {
    int (*join)(struct mddev *, int);
    int (*leave)(struct mddev *);
    int (*slot_number)(struct mddev *);
    int (*resync_info_update)(struct mddev *, sector_t, sector_t);
    void (*resync_info_get)(struct mddev *, sector_t *, sector_t *);
    int (*metadata_update_start)(struct mddev *);
    int (*metadata_update_finish)(struct mddev *);
    void (*metadata_update_cancel)(struct mddev *);
    int (*resync_start)(struct mddev *);
    int (*resync_finish)(struct mddev *);
    int (*area_resyncing)(struct mddev *, int, sector_t, sector_t);
    int (*add_new_disk)(struct mddev *, struct md_rdev *);
    void (*add_new_disk_cancel)(struct mddev *);
    int (*new_disk_ack)(struct mddev *, bool);
    int (*remove_disk)(struct mddev *, struct md_rdev *);
    void (*load_bitmaps)(struct mddev *, int);
    int (*gather_bitmaps)(struct md_rdev *);
    int (*resize_bitmaps)(struct mddev *, sector_t, sector_t);
    int (*lock_all_bitmaps)(struct mddev *);
    void (*unlock_all_bitmaps)(struct mddev *);
    void (*update_size)(struct mddev *, sector_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct md_cluster_operations {
    int (*join)(struct mddev *, int);
    int (*leave)(struct mddev *);
    int (*slot_number)(struct mddev *);
    int (*resync_info_update)(struct mddev *, sector_t, sector_t);
    void (*resync_info_get)(struct mddev *, sector_t *, sector_t *);
    int (*metadata_update_start)(struct mddev *);
    int (*metadata_update_finish)(struct mddev *);
    void (*metadata_update_cancel)(struct mddev *);
    int (*resync_start)(struct mddev *);
    int (*resync_finish)(struct mddev *);
    int (*area_resyncing)(struct mddev *, int, sector_t, sector_t);
    int (*add_new_disk)(struct mddev *, struct md_rdev *);
    void (*add_new_disk_cancel)(struct mddev *);
    int (*new_disk_ack)(struct mddev *, bool);
    int (*remove_disk)(struct mddev *, struct md_rdev *);
    void (*load_bitmaps)(struct mddev *, int);
    int (*gather_bitmaps)(struct md_rdev *);
    int (*resize_bitmaps)(struct mddev *, sector_t, sector_t);
    int (*lock_all_bitmaps)(struct mddev *);
    void (*unlock_all_bitmaps)(struct mddev *);
    void (*update_size)(struct mddev *, sector_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct md_cluster_operations {
    int (*join)(struct mddev *, int);
    int (*leave)(struct mddev *);
    int (*slot_number)(struct mddev *);
    int (*resync_info_update)(struct mddev *, sector_t, sector_t);
    void (*resync_info_get)(struct mddev *, sector_t *, sector_t *);
    int (*metadata_update_start)(struct mddev *);
    int (*metadata_update_finish)(struct mddev *);
    void (*metadata_update_cancel)(struct mddev *);
    int (*resync_start)(struct mddev *);
    int (*resync_finish)(struct mddev *);
    int (*area_resyncing)(struct mddev *, int, sector_t, sector_t);
    int (*add_new_disk)(struct mddev *, struct md_rdev *);
    void (*add_new_disk_cancel)(struct mddev *);
    int (*new_disk_ack)(struct mddev *, bool);
    int (*remove_disk)(struct mddev *, struct md_rdev *);
    void (*load_bitmaps)(struct mddev *, int);
    int (*gather_bitmaps)(struct md_rdev *);
    int (*resize_bitmaps)(struct mddev *, sector_t, sector_t);
    int (*lock_all_bitmaps)(struct mddev *);
    void (*unlock_all_bitmaps)(struct mddev *);
    void (*update_size)(struct mddev *, sector_t);
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
<code>void (*load_bitmaps)(struct mddev *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*lock_all_bitmaps)(struct mddev *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*unlock_all_bitmaps)(struct mddev *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*update_size)(struct mddev *, sector_t)</code>
</li>
</ul>
</details>
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
<code>void (*resync_info_get)(struct mddev *, sector_t *, sector_t *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*resize_bitmaps)(struct mddev *, sector_t, sector_t)</code>
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
No changes between <code>5.4</code> and <code>5.8</code> ✅
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
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
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
<li>
No changes between <code>amd64</code> and <code>armhf</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>riscv64</code> ✅
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
No changes between <code>generic</code> and <code>aws</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
