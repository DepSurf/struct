# Struct: <code>nand_chip</code>

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
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct nand_chip {
    struct nand_device base;
    struct nand_legacy legacy;
    int (*setup_read_retry)(struct nand_chip *, int);
    unsigned int options;
    unsigned int bbt_options;
    int page_shift;
    int phys_erase_shift;
    int bbt_erase_shift;
    int chip_shift;
    int pagemask;
    u8 *data_buf;
    struct (anon) pagecache;
    int subpagesize;
    int onfi_timing_mode_default;
    unsigned int badblockpos;
    int badblockbits;
    struct nand_id id;
    struct nand_parameters parameters;
    struct nand_data_interface data_interface;
    int cur_cs;
    int read_retries;
    struct mutex lock;
    unsigned int suspended;
    uint8_t *oob_poi;
    struct nand_controller *controller;
    struct nand_ecc_ctrl ecc;
    long unsigned int buf_align;
    uint8_t *bbt;
    struct nand_bbt_descr *bbt_td;
    struct nand_bbt_descr *bbt_md;
    struct nand_bbt_descr *badblock_pattern;
    void *priv;
    struct (anon) manufacturer;
};
```
</details>
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
<b>Arch</b>
<ul>
</ul>
