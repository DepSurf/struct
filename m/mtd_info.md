# Struct: <code>mtd_info</code>

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
struct mtd_info {
    u_char type;
    uint32_t flags;
    uint32_t orig_flags;
    uint64_t size;
    uint32_t erasesize;
    uint32_t writesize;
    uint32_t writebufsize;
    uint32_t oobsize;
    uint32_t oobavail;
    unsigned int erasesize_shift;
    unsigned int writesize_shift;
    unsigned int erasesize_mask;
    unsigned int writesize_mask;
    unsigned int bitflip_threshold;
    const char *name;
    int index;
    const struct mtd_ooblayout_ops *ooblayout;
    const struct mtd_pairing_scheme *pairing;
    unsigned int ecc_step_size;
    unsigned int ecc_strength;
    int numeraseregions;
    struct mtd_erase_region_info *eraseregions;
    int (*_erase)(struct mtd_info *, struct erase_info *);
    int (*_point)(struct mtd_info *, loff_t, size_t, size_t *, void **, resource_size_t *);
    int (*_unpoint)(struct mtd_info *, loff_t, size_t);
    int (*_read)(struct mtd_info *, loff_t, size_t, size_t *, u_char *);
    int (*_write)(struct mtd_info *, loff_t, size_t, size_t *, const u_char *);
    int (*_panic_write)(struct mtd_info *, loff_t, size_t, size_t *, const u_char *);
    int (*_read_oob)(struct mtd_info *, loff_t, struct mtd_oob_ops *);
    int (*_write_oob)(struct mtd_info *, loff_t, struct mtd_oob_ops *);
    int (*_get_fact_prot_info)(struct mtd_info *, size_t, size_t *, struct otp_info *);
    int (*_read_fact_prot_reg)(struct mtd_info *, loff_t, size_t, size_t *, u_char *);
    int (*_get_user_prot_info)(struct mtd_info *, size_t, size_t *, struct otp_info *);
    int (*_read_user_prot_reg)(struct mtd_info *, loff_t, size_t, size_t *, u_char *);
    int (*_write_user_prot_reg)(struct mtd_info *, loff_t, size_t, size_t *, u_char *);
    int (*_lock_user_prot_reg)(struct mtd_info *, loff_t, size_t);
    int (*_writev)(struct mtd_info *, const struct kvec *, long unsigned int, loff_t, size_t *);
    void (*_sync)(struct mtd_info *);
    int (*_lock)(struct mtd_info *, loff_t, uint64_t);
    int (*_unlock)(struct mtd_info *, loff_t, uint64_t);
    int (*_is_locked)(struct mtd_info *, loff_t, uint64_t);
    int (*_block_isreserved)(struct mtd_info *, loff_t);
    int (*_block_isbad)(struct mtd_info *, loff_t);
    int (*_block_markbad)(struct mtd_info *, loff_t);
    int (*_max_bad_blocks)(struct mtd_info *, loff_t, size_t);
    int (*_suspend)(struct mtd_info *);
    void (*_resume)(struct mtd_info *);
    void (*_reboot)(struct mtd_info *);
    int (*_get_device)(struct mtd_info *);
    void (*_put_device)(struct mtd_info *);
    bool oops_panic_write;
    struct notifier_block reboot_notifier;
    struct mtd_ecc_stats ecc_stats;
    int subpage_sft;
    void *priv;
    struct module *owner;
    struct device dev;
    int usecount;
    struct mtd_debug_info dbg;
    struct nvmem_device *nvmem;
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
