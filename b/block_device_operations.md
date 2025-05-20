# Struct: <code>block_device_operations</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct block_device_operations {
    int (*open)(struct block_device *, fmode_t);
    void (*release)(struct gendisk *, fmode_t);
    int (*rw_page)(struct block_device *, sector_t, struct page *, int);
    int (*ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    long int (*direct_access)(struct block_device *, sector_t, void **, long unsigned int *);
    unsigned int (*check_events)(struct gendisk *, unsigned int);
    int (*media_changed)(struct gendisk *);
    void (*unlock_native_capacity)(struct gendisk *);
    int (*revalidate_disk)(struct gendisk *);
    int (*getgeo)(struct block_device *, struct hd_geometry *);
    void (*swap_slot_free_notify)(struct block_device *, long unsigned int);
    struct module *owner;
    const struct pr_ops *pr_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct block_device_operations {
    int (*open)(struct block_device *, fmode_t);
    void (*release)(struct gendisk *, fmode_t);
    int (*rw_page)(struct block_device *, sector_t, struct page *, bool);
    int (*ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    long int (*direct_access)(struct block_device *, sector_t, void **, pfn_t *, long int);
    unsigned int (*check_events)(struct gendisk *, unsigned int);
    int (*media_changed)(struct gendisk *);
    void (*unlock_native_capacity)(struct gendisk *);
    int (*revalidate_disk)(struct gendisk *);
    int (*getgeo)(struct block_device *, struct hd_geometry *);
    void (*swap_slot_free_notify)(struct block_device *, long unsigned int);
    struct module *owner;
    const struct pr_ops *pr_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct block_device_operations {
    int (*open)(struct block_device *, fmode_t);
    void (*release)(struct gendisk *, fmode_t);
    int (*rw_page)(struct block_device *, sector_t, struct page *, bool);
    int (*ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    long int (*direct_access)(struct block_device *, sector_t, void **, pfn_t *, long int);
    unsigned int (*check_events)(struct gendisk *, unsigned int);
    int (*media_changed)(struct gendisk *);
    void (*unlock_native_capacity)(struct gendisk *);
    int (*revalidate_disk)(struct gendisk *);
    int (*getgeo)(struct block_device *, struct hd_geometry *);
    void (*swap_slot_free_notify)(struct block_device *, long unsigned int);
    struct module *owner;
    const struct pr_ops *pr_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct block_device_operations {
    int (*open)(struct block_device *, fmode_t);
    void (*release)(struct gendisk *, fmode_t);
    int (*rw_page)(struct block_device *, sector_t, struct page *, bool);
    int (*ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    unsigned int (*check_events)(struct gendisk *, unsigned int);
    int (*media_changed)(struct gendisk *);
    void (*unlock_native_capacity)(struct gendisk *);
    int (*revalidate_disk)(struct gendisk *);
    int (*getgeo)(struct block_device *, struct hd_geometry *);
    void (*swap_slot_free_notify)(struct block_device *, long unsigned int);
    struct module *owner;
    const struct pr_ops *pr_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct block_device_operations {
    int (*open)(struct block_device *, fmode_t);
    void (*release)(struct gendisk *, fmode_t);
    int (*rw_page)(struct block_device *, sector_t, struct page *, bool);
    int (*ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    unsigned int (*check_events)(struct gendisk *, unsigned int);
    int (*media_changed)(struct gendisk *);
    void (*unlock_native_capacity)(struct gendisk *);
    int (*revalidate_disk)(struct gendisk *);
    int (*getgeo)(struct block_device *, struct hd_geometry *);
    void (*swap_slot_free_notify)(struct block_device *, long unsigned int);
    struct module *owner;
    const struct pr_ops *pr_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct block_device_operations {
    int (*open)(struct block_device *, fmode_t);
    void (*release)(struct gendisk *, fmode_t);
    int (*rw_page)(struct block_device *, sector_t, struct page *, bool);
    int (*ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    unsigned int (*check_events)(struct gendisk *, unsigned int);
    int (*media_changed)(struct gendisk *);
    void (*unlock_native_capacity)(struct gendisk *);
    int (*revalidate_disk)(struct gendisk *);
    int (*getgeo)(struct block_device *, struct hd_geometry *);
    void (*swap_slot_free_notify)(struct block_device *, long unsigned int);
    struct module *owner;
    const struct pr_ops *pr_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct block_device_operations {
    int (*open)(struct block_device *, fmode_t);
    void (*release)(struct gendisk *, fmode_t);
    int (*rw_page)(struct block_device *, sector_t, struct page *, unsigned int);
    int (*ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    unsigned int (*check_events)(struct gendisk *, unsigned int);
    int (*media_changed)(struct gendisk *);
    void (*unlock_native_capacity)(struct gendisk *);
    int (*revalidate_disk)(struct gendisk *);
    int (*getgeo)(struct block_device *, struct hd_geometry *);
    void (*swap_slot_free_notify)(struct block_device *, long unsigned int);
    int (*report_zones)(struct gendisk *, sector_t, struct blk_zone *, unsigned int *, gfp_t);
    struct module *owner;
    const struct pr_ops *pr_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct block_device_operations {
    int (*open)(struct block_device *, fmode_t);
    void (*release)(struct gendisk *, fmode_t);
    int (*rw_page)(struct block_device *, sector_t, struct page *, unsigned int);
    int (*ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    unsigned int (*check_events)(struct gendisk *, unsigned int);
    int (*media_changed)(struct gendisk *);
    void (*unlock_native_capacity)(struct gendisk *);
    int (*revalidate_disk)(struct gendisk *);
    int (*getgeo)(struct block_device *, struct hd_geometry *);
    void (*swap_slot_free_notify)(struct block_device *, long unsigned int);
    int (*report_zones)(struct gendisk *, sector_t, struct blk_zone *, unsigned int *);
    struct module *owner;
    const struct pr_ops *pr_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct block_device_operations {
    int (*open)(struct block_device *, fmode_t);
    void (*release)(struct gendisk *, fmode_t);
    int (*rw_page)(struct block_device *, sector_t, struct page *, unsigned int);
    int (*ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    unsigned int (*check_events)(struct gendisk *, unsigned int);
    int (*media_changed)(struct gendisk *);
    void (*unlock_native_capacity)(struct gendisk *);
    int (*revalidate_disk)(struct gendisk *);
    int (*getgeo)(struct block_device *, struct hd_geometry *);
    void (*swap_slot_free_notify)(struct block_device *, long unsigned int);
    int (*report_zones)(struct gendisk *, sector_t, struct blk_zone *, unsigned int *);
    struct module *owner;
    const struct pr_ops *pr_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct block_device_operations {
    int (*open)(struct block_device *, fmode_t);
    void (*release)(struct gendisk *, fmode_t);
    int (*rw_page)(struct block_device *, sector_t, struct page *, unsigned int);
    int (*ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    unsigned int (*check_events)(struct gendisk *, unsigned int);
    int (*media_changed)(struct gendisk *);
    void (*unlock_native_capacity)(struct gendisk *);
    int (*revalidate_disk)(struct gendisk *);
    int (*getgeo)(struct block_device *, struct hd_geometry *);
    void (*swap_slot_free_notify)(struct block_device *, long unsigned int);
    int (*report_zones)(struct gendisk *, sector_t, unsigned int, report_zones_cb, void *);
    char * (*devnode)(struct gendisk *, umode_t *);
    struct module *owner;
    const struct pr_ops *pr_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct block_device_operations {
    blk_qc_t (*submit_bio)(struct bio *);
    int (*open)(struct block_device *, fmode_t);
    void (*release)(struct gendisk *, fmode_t);
    int (*rw_page)(struct block_device *, sector_t, struct page *, unsigned int);
    int (*ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    unsigned int (*check_events)(struct gendisk *, unsigned int);
    void (*unlock_native_capacity)(struct gendisk *);
    int (*revalidate_disk)(struct gendisk *);
    int (*getgeo)(struct block_device *, struct hd_geometry *);
    int (*set_read_only)(struct block_device *, bool);
    void (*swap_slot_free_notify)(struct block_device *, long unsigned int);
    int (*report_zones)(struct gendisk *, sector_t, unsigned int, report_zones_cb, void *);
    char * (*devnode)(struct gendisk *, umode_t *);
    struct module *owner;
    const struct pr_ops *pr_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct block_device_operations {
    blk_qc_t (*submit_bio)(struct bio *);
    int (*open)(struct block_device *, fmode_t);
    void (*release)(struct gendisk *, fmode_t);
    int (*rw_page)(struct block_device *, sector_t, struct page *, unsigned int);
    int (*ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    unsigned int (*check_events)(struct gendisk *, unsigned int);
    void (*unlock_native_capacity)(struct gendisk *);
    int (*getgeo)(struct block_device *, struct hd_geometry *);
    int (*set_read_only)(struct block_device *, bool);
    void (*swap_slot_free_notify)(struct block_device *, long unsigned int);
    int (*report_zones)(struct gendisk *, sector_t, unsigned int, report_zones_cb, void *);
    char * (*devnode)(struct gendisk *, umode_t *);
    struct module *owner;
    const struct pr_ops *pr_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct block_device_operations {
    blk_qc_t (*submit_bio)(struct bio *);
    int (*open)(struct block_device *, fmode_t);
    void (*release)(struct gendisk *, fmode_t);
    int (*rw_page)(struct block_device *, sector_t, struct page *, unsigned int);
    int (*ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    unsigned int (*check_events)(struct gendisk *, unsigned int);
    void (*unlock_native_capacity)(struct gendisk *);
    int (*getgeo)(struct block_device *, struct hd_geometry *);
    int (*set_read_only)(struct block_device *, bool);
    void (*swap_slot_free_notify)(struct block_device *, long unsigned int);
    int (*report_zones)(struct gendisk *, sector_t, unsigned int, report_zones_cb, void *);
    char * (*devnode)(struct gendisk *, umode_t *);
    struct module *owner;
    const struct pr_ops *pr_ops;
    int (*alternative_gpt_sector)(struct gendisk *, sector_t *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct block_device_operations {
    void (*submit_bio)(struct bio *);
    int (*poll_bio)(struct bio *, struct io_comp_batch *, unsigned int);
    int (*open)(struct block_device *, fmode_t);
    void (*release)(struct gendisk *, fmode_t);
    int (*rw_page)(struct block_device *, sector_t, struct page *, unsigned int);
    int (*ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    unsigned int (*check_events)(struct gendisk *, unsigned int);
    void (*unlock_native_capacity)(struct gendisk *);
    int (*getgeo)(struct block_device *, struct hd_geometry *);
    int (*set_read_only)(struct block_device *, bool);
    void (*free_disk)(struct gendisk *);
    void (*swap_slot_free_notify)(struct block_device *, long unsigned int);
    int (*report_zones)(struct gendisk *, sector_t, unsigned int, report_zones_cb, void *);
    char * (*devnode)(struct gendisk *, umode_t *);
    int (*get_unique_id)(struct gendisk *, u8 *, enum blk_unique_id);
    struct module *owner;
    const struct pr_ops *pr_ops;
    int (*alternative_gpt_sector)(struct gendisk *, sector_t *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct block_device_operations {
    void (*submit_bio)(struct bio *);
    int (*poll_bio)(struct bio *, struct io_comp_batch *, unsigned int);
    int (*open)(struct block_device *, fmode_t);
    void (*release)(struct gendisk *, fmode_t);
    int (*rw_page)(struct block_device *, sector_t, struct page *, enum req_op);
    int (*ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    unsigned int (*check_events)(struct gendisk *, unsigned int);
    void (*unlock_native_capacity)(struct gendisk *);
    int (*getgeo)(struct block_device *, struct hd_geometry *);
    int (*set_read_only)(struct block_device *, bool);
    void (*free_disk)(struct gendisk *);
    void (*swap_slot_free_notify)(struct block_device *, long unsigned int);
    int (*report_zones)(struct gendisk *, sector_t, unsigned int, report_zones_cb, void *);
    char * (*devnode)(struct gendisk *, umode_t *);
    int (*get_unique_id)(struct gendisk *, u8 *, enum blk_unique_id);
    struct module *owner;
    const struct pr_ops *pr_ops;
    int (*alternative_gpt_sector)(struct gendisk *, sector_t *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct block_device_operations {
    void (*submit_bio)(struct bio *);
    int (*poll_bio)(struct bio *, struct io_comp_batch *, unsigned int);
    int (*open)(struct gendisk *, blk_mode_t);
    void (*release)(struct gendisk *);
    int (*ioctl)(struct block_device *, blk_mode_t, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct block_device *, blk_mode_t, unsigned int, long unsigned int);
    unsigned int (*check_events)(struct gendisk *, unsigned int);
    void (*unlock_native_capacity)(struct gendisk *);
    int (*getgeo)(struct block_device *, struct hd_geometry *);
    int (*set_read_only)(struct block_device *, bool);
    void (*free_disk)(struct gendisk *);
    void (*swap_slot_free_notify)(struct block_device *, long unsigned int);
    int (*report_zones)(struct gendisk *, sector_t, unsigned int, report_zones_cb, void *);
    char * (*devnode)(struct gendisk *, umode_t *);
    int (*get_unique_id)(struct gendisk *, u8 *, enum blk_unique_id);
    struct module *owner;
    const struct pr_ops *pr_ops;
    int (*alternative_gpt_sector)(struct gendisk *, sector_t *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct block_device_operations {
    void (*submit_bio)(struct bio *);
    int (*poll_bio)(struct bio *, struct io_comp_batch *, unsigned int);
    int (*open)(struct gendisk *, blk_mode_t);
    void (*release)(struct gendisk *);
    int (*ioctl)(struct block_device *, blk_mode_t, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct block_device *, blk_mode_t, unsigned int, long unsigned int);
    unsigned int (*check_events)(struct gendisk *, unsigned int);
    void (*unlock_native_capacity)(struct gendisk *);
    int (*getgeo)(struct block_device *, struct hd_geometry *);
    int (*set_read_only)(struct block_device *, bool);
    void (*free_disk)(struct gendisk *);
    void (*swap_slot_free_notify)(struct block_device *, long unsigned int);
    int (*report_zones)(struct gendisk *, sector_t, unsigned int, report_zones_cb, void *);
    char * (*devnode)(struct gendisk *, umode_t *);
    int (*get_unique_id)(struct gendisk *, u8 *, enum blk_unique_id);
    struct module *owner;
    const struct pr_ops *pr_ops;
    int (*alternative_gpt_sector)(struct gendisk *, sector_t *);
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
struct block_device_operations {
    int (*open)(struct block_device *, fmode_t);
    void (*release)(struct gendisk *, fmode_t);
    int (*rw_page)(struct block_device *, sector_t, struct page *, unsigned int);
    int (*ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    unsigned int (*check_events)(struct gendisk *, unsigned int);
    int (*media_changed)(struct gendisk *);
    void (*unlock_native_capacity)(struct gendisk *);
    int (*revalidate_disk)(struct gendisk *);
    int (*getgeo)(struct block_device *, struct hd_geometry *);
    void (*swap_slot_free_notify)(struct block_device *, long unsigned int);
    int (*report_zones)(struct gendisk *, sector_t, struct blk_zone *, unsigned int *);
    struct module *owner;
    const struct pr_ops *pr_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct block_device_operations {
    int (*open)(struct block_device *, fmode_t);
    void (*release)(struct gendisk *, fmode_t);
    int (*rw_page)(struct block_device *, sector_t, struct page *, unsigned int);
    int (*ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    unsigned int (*check_events)(struct gendisk *, unsigned int);
    int (*media_changed)(struct gendisk *);
    void (*unlock_native_capacity)(struct gendisk *);
    int (*revalidate_disk)(struct gendisk *);
    int (*getgeo)(struct block_device *, struct hd_geometry *);
    void (*swap_slot_free_notify)(struct block_device *, long unsigned int);
    int (*report_zones)(struct gendisk *, sector_t, struct blk_zone *, unsigned int *);
    struct module *owner;
    const struct pr_ops *pr_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct block_device_operations {
    int (*open)(struct block_device *, fmode_t);
    void (*release)(struct gendisk *, fmode_t);
    int (*rw_page)(struct block_device *, sector_t, struct page *, unsigned int);
    int (*ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    unsigned int (*check_events)(struct gendisk *, unsigned int);
    int (*media_changed)(struct gendisk *);
    void (*unlock_native_capacity)(struct gendisk *);
    int (*revalidate_disk)(struct gendisk *);
    int (*getgeo)(struct block_device *, struct hd_geometry *);
    void (*swap_slot_free_notify)(struct block_device *, long unsigned int);
    int (*report_zones)(struct gendisk *, sector_t, struct blk_zone *, unsigned int *);
    struct module *owner;
    const struct pr_ops *pr_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct block_device_operations {
    int (*open)(struct block_device *, fmode_t);
    void (*release)(struct gendisk *, fmode_t);
    int (*rw_page)(struct block_device *, sector_t, struct page *, unsigned int);
    int (*ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    unsigned int (*check_events)(struct gendisk *, unsigned int);
    int (*media_changed)(struct gendisk *);
    void (*unlock_native_capacity)(struct gendisk *);
    int (*revalidate_disk)(struct gendisk *);
    int (*getgeo)(struct block_device *, struct hd_geometry *);
    void (*swap_slot_free_notify)(struct block_device *, long unsigned int);
    int (*report_zones)(struct gendisk *, sector_t, struct blk_zone *, unsigned int *);
    struct module *owner;
    const struct pr_ops *pr_ops;
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
struct block_device_operations {
    int (*open)(struct block_device *, fmode_t);
    void (*release)(struct gendisk *, fmode_t);
    int (*rw_page)(struct block_device *, sector_t, struct page *, unsigned int);
    int (*ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    unsigned int (*check_events)(struct gendisk *, unsigned int);
    int (*media_changed)(struct gendisk *);
    void (*unlock_native_capacity)(struct gendisk *);
    int (*revalidate_disk)(struct gendisk *);
    int (*getgeo)(struct block_device *, struct hd_geometry *);
    void (*swap_slot_free_notify)(struct block_device *, long unsigned int);
    int (*report_zones)(struct gendisk *, sector_t, struct blk_zone *, unsigned int *);
    struct module *owner;
    const struct pr_ops *pr_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct block_device_operations {
    int (*open)(struct block_device *, fmode_t);
    void (*release)(struct gendisk *, fmode_t);
    int (*rw_page)(struct block_device *, sector_t, struct page *, unsigned int);
    int (*ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    unsigned int (*check_events)(struct gendisk *, unsigned int);
    int (*media_changed)(struct gendisk *);
    void (*unlock_native_capacity)(struct gendisk *);
    int (*revalidate_disk)(struct gendisk *);
    int (*getgeo)(struct block_device *, struct hd_geometry *);
    void (*swap_slot_free_notify)(struct block_device *, long unsigned int);
    int (*report_zones)(struct gendisk *, sector_t, struct blk_zone *, unsigned int *);
    struct module *owner;
    const struct pr_ops *pr_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct block_device_operations {
    int (*open)(struct block_device *, fmode_t);
    void (*release)(struct gendisk *, fmode_t);
    int (*rw_page)(struct block_device *, sector_t, struct page *, unsigned int);
    int (*ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    unsigned int (*check_events)(struct gendisk *, unsigned int);
    int (*media_changed)(struct gendisk *);
    void (*unlock_native_capacity)(struct gendisk *);
    int (*revalidate_disk)(struct gendisk *);
    int (*getgeo)(struct block_device *, struct hd_geometry *);
    void (*swap_slot_free_notify)(struct block_device *, long unsigned int);
    int (*report_zones)(struct gendisk *, sector_t, struct blk_zone *, unsigned int *);
    struct module *owner;
    const struct pr_ops *pr_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct block_device_operations {
    int (*open)(struct block_device *, fmode_t);
    void (*release)(struct gendisk *, fmode_t);
    int (*rw_page)(struct block_device *, sector_t, struct page *, unsigned int);
    int (*ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int);
    unsigned int (*check_events)(struct gendisk *, unsigned int);
    int (*media_changed)(struct gendisk *);
    void (*unlock_native_capacity)(struct gendisk *);
    int (*revalidate_disk)(struct gendisk *);
    int (*getgeo)(struct block_device *, struct hd_geometry *);
    void (*swap_slot_free_notify)(struct block_device *, long unsigned int);
    int (*report_zones)(struct gendisk *, sector_t, struct blk_zone *, unsigned int *);
    struct module *owner;
    const struct pr_ops *pr_ops;
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
<b>Field type changed. </b>
<code>int (*rw_page)(struct block_device *, sector_t, struct page *, int)</code> ➡️ <code>int (*rw_page)(struct block_device *, sector_t, struct page *, bool)</code>
</li>
<li>
<b>Field type changed. </b>
<code>long int (*direct_access)(struct block_device *, sector_t, void **, long unsigned int *)</code> ➡️ <code>long int (*direct_access)(struct block_device *, sector_t, void **, pfn_t *, long int)</code>
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
<b>Field removed. </b>
<code>long int (*direct_access)(struct block_device *, sector_t, void **, pfn_t *, long int)</code>
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
<code>int (*report_zones)(struct gendisk *, sector_t, struct blk_zone *, unsigned int *, gfp_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*rw_page)(struct block_device *, sector_t, struct page *, bool)</code> ➡️ <code>int (*rw_page)(struct block_device *, sector_t, struct page *, unsigned int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*report_zones)(struct gendisk *, sector_t, struct blk_zone *, unsigned int *, gfp_t)</code> ➡️ <code>int (*report_zones)(struct gendisk *, sector_t, struct blk_zone *, unsigned int *)</code>
</li>
</ul>
</details>
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
<code>char * (*devnode)(struct gendisk *, umode_t *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*report_zones)(struct gendisk *, sector_t, struct blk_zone *, unsigned int *)</code> ➡️ <code>int (*report_zones)(struct gendisk *, sector_t, unsigned int, report_zones_cb, void *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>blk_qc_t (*submit_bio)(struct bio *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_read_only)(struct block_device *, bool)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*media_changed)(struct gendisk *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*revalidate_disk)(struct gendisk *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*alternative_gpt_sector)(struct gendisk *, sector_t *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*poll_bio)(struct bio *, struct io_comp_batch *, unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*free_disk)(struct gendisk *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*get_unique_id)(struct gendisk *, u8 *, enum blk_unique_id)</code>
</li>
<li>
<b>Field type changed. </b>
<code>blk_qc_t (*submit_bio)(struct bio *)</code> ➡️ <code>void (*submit_bio)(struct bio *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*rw_page)(struct block_device *, sector_t, struct page *, unsigned int)</code> ➡️ <code>int (*rw_page)(struct block_device *, sector_t, struct page *, enum req_op)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*rw_page)(struct block_device *, sector_t, struct page *, enum req_op)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*open)(struct block_device *, fmode_t)</code> ➡️ <code>int (*open)(struct gendisk *, blk_mode_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*release)(struct gendisk *, fmode_t)</code> ➡️ <code>void (*release)(struct gendisk *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int)</code> ➡️ <code>int (*ioctl)(struct block_device *, blk_mode_t, unsigned int, long unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*compat_ioctl)(struct block_device *, fmode_t, unsigned int, long unsigned int)</code> ➡️ <code>int (*compat_ioctl)(struct block_device *, blk_mode_t, unsigned int, long unsigned int)</code>
</li>
</ul>
</details>
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
