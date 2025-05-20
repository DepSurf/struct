# Struct: <code>nvmm_type</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct nvmm_type {
    const char *name;
    unsigned int version[3];
    nvmm_register_fn *register_mgr;
    nvmm_unregister_fn *unregister_mgr;
    nvmm_get_blk_fn *get_blk_unlocked;
    nvmm_put_blk_fn *put_blk_unlocked;
    nvmm_get_blk_fn *get_blk;
    nvmm_put_blk_fn *put_blk;
    nvmm_open_blk_fn *open_blk;
    nvmm_close_blk_fn *close_blk;
    nvmm_flush_blk_fn *flush_blk;
    nvmm_submit_io_fn *submit_io;
    nvmm_erase_blk_fn *erase_blk;
    nvmm_get_lun_fn *get_lun;
    nvmm_lun_info_print_fn *lun_info_print;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct nvmm_type {
    const char *name;
    unsigned int version[3];
    nvmm_register_fn *register_mgr;
    nvmm_unregister_fn *unregister_mgr;
    nvmm_create_tgt_fn *create_tgt;
    nvmm_remove_tgt_fn *remove_tgt;
    nvmm_get_blk_fn *get_blk;
    nvmm_put_blk_fn *put_blk;
    nvmm_open_blk_fn *open_blk;
    nvmm_close_blk_fn *close_blk;
    nvmm_flush_blk_fn *flush_blk;
    nvmm_submit_io_fn *submit_io;
    nvmm_erase_blk_fn *erase_blk;
    nvmm_mark_blk_fn *mark_blk;
    nvmm_get_lun_fn *get_lun;
    nvmm_reserve_lun *reserve_lun;
    nvmm_release_lun *release_lun;
    nvmm_lun_info_print_fn *lun_info_print;
    nvmm_get_area_fn *get_area;
    nvmm_put_area_fn *put_area;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct nvmm_type {
    const char *name;
    unsigned int version[3];
    nvmm_register_fn *register_mgr;
    nvmm_unregister_fn *unregister_mgr;
    nvmm_create_tgt_fn *create_tgt;
    nvmm_remove_tgt_fn *remove_tgt;
    nvmm_submit_io_fn *submit_io;
    nvmm_erase_blk_fn *erase_blk;
    nvmm_get_area_fn *get_area;
    nvmm_put_area_fn *put_area;
    nvmm_trans_ppa_fn *trans_ppa;
    nvmm_part_to_tgt_fn *part_to_tgt;
    struct list_head list;
};
```
</details>
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
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>nvmm_create_tgt_fn *create_tgt</code>
</li>
<li>
<b>Field added. </b>
<code>nvmm_remove_tgt_fn *remove_tgt</code>
</li>
<li>
<b>Field added. </b>
<code>nvmm_mark_blk_fn *mark_blk</code>
</li>
<li>
<b>Field added. </b>
<code>nvmm_reserve_lun *reserve_lun</code>
</li>
<li>
<b>Field added. </b>
<code>nvmm_release_lun *release_lun</code>
</li>
<li>
<b>Field added. </b>
<code>nvmm_get_area_fn *get_area</code>
</li>
<li>
<b>Field added. </b>
<code>nvmm_put_area_fn *put_area</code>
</li>
<li>
<b>Field removed. </b>
<code>nvmm_get_blk_fn *get_blk_unlocked</code>
</li>
<li>
<b>Field removed. </b>
<code>nvmm_put_blk_fn *put_blk_unlocked</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>nvmm_trans_ppa_fn *trans_ppa</code>
</li>
<li>
<b>Field added. </b>
<code>nvmm_part_to_tgt_fn *part_to_tgt</code>
</li>
<li>
<b>Field removed. </b>
<code>nvmm_get_blk_fn *get_blk</code>
</li>
<li>
<b>Field removed. </b>
<code>nvmm_put_blk_fn *put_blk</code>
</li>
<li>
<b>Field removed. </b>
<code>nvmm_open_blk_fn *open_blk</code>
</li>
<li>
<b>Field removed. </b>
<code>nvmm_close_blk_fn *close_blk</code>
</li>
<li>
<b>Field removed. </b>
<code>nvmm_flush_blk_fn *flush_blk</code>
</li>
<li>
<b>Field removed. </b>
<code>nvmm_mark_blk_fn *mark_blk</code>
</li>
<li>
<b>Field removed. </b>
<code>nvmm_get_lun_fn *get_lun</code>
</li>
<li>
<b>Field removed. </b>
<code>nvmm_reserve_lun *reserve_lun</code>
</li>
<li>
<b>Field removed. </b>
<code>nvmm_release_lun *release_lun</code>
</li>
<li>
<b>Field removed. </b>
<code>nvmm_lun_info_print_fn *lun_info_print</code>
</li>
</ul>
</details>
</li>
</ul>
