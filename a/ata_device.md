# Struct: <code>ata_device</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct ata_device {
    struct ata_link *link;
    unsigned int devno;
    unsigned int horkage;
    long unsigned int flags;
    struct scsi_device *sdev;
    void *private_data;
    union acpi_object *gtf_cache;
    unsigned int gtf_filter;
    void *zpodd;
    struct device tdev;
    u64 n_sectors;
    u64 n_native_sectors;
    unsigned int class;
    long unsigned int unpark_deadline;
    u8 pio_mode;
    u8 dma_mode;
    u8 xfer_mode;
    unsigned int xfer_shift;
    unsigned int multi_count;
    unsigned int max_sectors;
    unsigned int cdb_len;
    long unsigned int pio_mask;
    long unsigned int mwdma_mask;
    long unsigned int udma_mask;
    u16 cylinders;
    u16 heads;
    u16 sectors;
    u16 id[256];
    u32 gscr[128];
    u8 devslp_timing[8];
    u8 ncq_send_recv_cmds[16];
    int spdn_cnt;
    struct ata_ering ering;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ata_device {
    struct ata_link *link;
    unsigned int devno;
    unsigned int horkage;
    long unsigned int flags;
    struct scsi_device *sdev;
    void *private_data;
    union acpi_object *gtf_cache;
    unsigned int gtf_filter;
    void *zpodd;
    struct device tdev;
    u64 n_sectors;
    u64 n_native_sectors;
    unsigned int class;
    long unsigned int unpark_deadline;
    u8 pio_mode;
    u8 dma_mode;
    u8 xfer_mode;
    unsigned int xfer_shift;
    unsigned int multi_count;
    unsigned int max_sectors;
    unsigned int cdb_len;
    long unsigned int pio_mask;
    long unsigned int mwdma_mask;
    long unsigned int udma_mask;
    u16 cylinders;
    u16 heads;
    u16 sectors;
    u16 id[256];
    u32 gscr[128];
    u8 devslp_timing[8];
    u8 ncq_send_recv_cmds[20];
    u8 ncq_non_data_cmds[64];
    u32 zac_zoned_cap;
    u32 zac_zones_optimal_open;
    u32 zac_zones_optimal_nonseq;
    u32 zac_zones_max_open;
    int spdn_cnt;
    struct ata_ering ering;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ata_device {
    struct ata_link *link;
    unsigned int devno;
    unsigned int horkage;
    long unsigned int flags;
    struct scsi_device *sdev;
    void *private_data;
    union acpi_object *gtf_cache;
    unsigned int gtf_filter;
    void *zpodd;
    struct device tdev;
    u64 n_sectors;
    u64 n_native_sectors;
    unsigned int class;
    long unsigned int unpark_deadline;
    u8 pio_mode;
    u8 dma_mode;
    u8 xfer_mode;
    unsigned int xfer_shift;
    unsigned int multi_count;
    unsigned int max_sectors;
    unsigned int cdb_len;
    long unsigned int pio_mask;
    long unsigned int mwdma_mask;
    long unsigned int udma_mask;
    u16 cylinders;
    u16 heads;
    u16 sectors;
    u16 id[256];
    u32 gscr[128];
    u8 devslp_timing[8];
    u8 ncq_send_recv_cmds[20];
    u8 ncq_non_data_cmds[64];
    u32 zac_zoned_cap;
    u32 zac_zones_optimal_open;
    u32 zac_zones_optimal_nonseq;
    u32 zac_zones_max_open;
    int spdn_cnt;
    struct ata_ering ering;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ata_device {
    struct ata_link *link;
    unsigned int devno;
    unsigned int horkage;
    long unsigned int flags;
    struct scsi_device *sdev;
    void *private_data;
    union acpi_object *gtf_cache;
    unsigned int gtf_filter;
    void *zpodd;
    struct device tdev;
    u64 n_sectors;
    u64 n_native_sectors;
    unsigned int class;
    long unsigned int unpark_deadline;
    u8 pio_mode;
    u8 dma_mode;
    u8 xfer_mode;
    unsigned int xfer_shift;
    unsigned int multi_count;
    unsigned int max_sectors;
    unsigned int cdb_len;
    long unsigned int pio_mask;
    long unsigned int mwdma_mask;
    long unsigned int udma_mask;
    u16 cylinders;
    u16 heads;
    u16 sectors;
    u16 id[256];
    u32 gscr[128];
    u8 devslp_timing[8];
    u8 ncq_send_recv_cmds[20];
    u8 ncq_non_data_cmds[64];
    u32 zac_zoned_cap;
    u32 zac_zones_optimal_open;
    u32 zac_zones_optimal_nonseq;
    u32 zac_zones_max_open;
    int spdn_cnt;
    struct ata_ering ering;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ata_device {
    struct ata_link *link;
    unsigned int devno;
    unsigned int horkage;
    long unsigned int flags;
    struct scsi_device *sdev;
    void *private_data;
    union acpi_object *gtf_cache;
    unsigned int gtf_filter;
    void *zpodd;
    struct device tdev;
    u64 n_sectors;
    u64 n_native_sectors;
    unsigned int class;
    long unsigned int unpark_deadline;
    u8 pio_mode;
    u8 dma_mode;
    u8 xfer_mode;
    unsigned int xfer_shift;
    unsigned int multi_count;
    unsigned int max_sectors;
    unsigned int cdb_len;
    long unsigned int pio_mask;
    long unsigned int mwdma_mask;
    long unsigned int udma_mask;
    u16 cylinders;
    u16 heads;
    u16 sectors;
    u16 id[256];
    u32 gscr[128];
    u8 devslp_timing[8];
    u8 ncq_send_recv_cmds[20];
    u8 ncq_non_data_cmds[64];
    u32 zac_zoned_cap;
    u32 zac_zones_optimal_open;
    u32 zac_zones_optimal_nonseq;
    u32 zac_zones_max_open;
    int spdn_cnt;
    struct ata_ering ering;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ata_device {
    struct ata_link *link;
    unsigned int devno;
    unsigned int horkage;
    long unsigned int flags;
    struct scsi_device *sdev;
    void *private_data;
    union acpi_object *gtf_cache;
    unsigned int gtf_filter;
    void *zpodd;
    struct device tdev;
    u64 n_sectors;
    u64 n_native_sectors;
    unsigned int class;
    long unsigned int unpark_deadline;
    u8 pio_mode;
    u8 dma_mode;
    u8 xfer_mode;
    unsigned int xfer_shift;
    unsigned int multi_count;
    unsigned int max_sectors;
    unsigned int cdb_len;
    long unsigned int pio_mask;
    long unsigned int mwdma_mask;
    long unsigned int udma_mask;
    u16 cylinders;
    u16 heads;
    u16 sectors;
    u16 id[256];
    u32 gscr[128];
    u8 devslp_timing[8];
    u8 ncq_send_recv_cmds[20];
    u8 ncq_non_data_cmds[64];
    u32 zac_zoned_cap;
    u32 zac_zones_optimal_open;
    u32 zac_zones_optimal_nonseq;
    u32 zac_zones_max_open;
    int spdn_cnt;
    struct ata_ering ering;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ata_device {
    struct ata_link *link;
    unsigned int devno;
    unsigned int horkage;
    long unsigned int flags;
    struct scsi_device *sdev;
    void *private_data;
    union acpi_object *gtf_cache;
    unsigned int gtf_filter;
    void *zpodd;
    struct device tdev;
    u64 n_sectors;
    u64 n_native_sectors;
    unsigned int class;
    long unsigned int unpark_deadline;
    u8 pio_mode;
    u8 dma_mode;
    u8 xfer_mode;
    unsigned int xfer_shift;
    unsigned int multi_count;
    unsigned int max_sectors;
    unsigned int cdb_len;
    long unsigned int pio_mask;
    long unsigned int mwdma_mask;
    long unsigned int udma_mask;
    u16 cylinders;
    u16 heads;
    u16 sectors;
    u16 id[256];
    u32 gscr[128];
    u8 devslp_timing[8];
    u8 ncq_send_recv_cmds[20];
    u8 ncq_non_data_cmds[64];
    u32 zac_zoned_cap;
    u32 zac_zones_optimal_open;
    u32 zac_zones_optimal_nonseq;
    u32 zac_zones_max_open;
    int spdn_cnt;
    struct ata_ering ering;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ata_device {
    struct ata_link *link;
    unsigned int devno;
    unsigned int horkage;
    long unsigned int flags;
    struct scsi_device *sdev;
    void *private_data;
    union acpi_object *gtf_cache;
    unsigned int gtf_filter;
    void *zpodd;
    struct device tdev;
    u64 n_sectors;
    u64 n_native_sectors;
    unsigned int class;
    long unsigned int unpark_deadline;
    u8 pio_mode;
    u8 dma_mode;
    u8 xfer_mode;
    unsigned int xfer_shift;
    unsigned int multi_count;
    unsigned int max_sectors;
    unsigned int cdb_len;
    long unsigned int pio_mask;
    long unsigned int mwdma_mask;
    long unsigned int udma_mask;
    u16 cylinders;
    u16 heads;
    u16 sectors;
    u16 id[256];
    u32 gscr[128];
    u8 devslp_timing[8];
    u8 ncq_send_recv_cmds[20];
    u8 ncq_non_data_cmds[64];
    u32 zac_zoned_cap;
    u32 zac_zones_optimal_open;
    u32 zac_zones_optimal_nonseq;
    u32 zac_zones_max_open;
    int spdn_cnt;
    struct ata_ering ering;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ata_device {
    struct ata_link *link;
    unsigned int devno;
    unsigned int horkage;
    long unsigned int flags;
    struct scsi_device *sdev;
    void *private_data;
    union acpi_object *gtf_cache;
    unsigned int gtf_filter;
    void *zpodd;
    struct device tdev;
    u64 n_sectors;
    u64 n_native_sectors;
    unsigned int class;
    long unsigned int unpark_deadline;
    u8 pio_mode;
    u8 dma_mode;
    u8 xfer_mode;
    unsigned int xfer_shift;
    unsigned int multi_count;
    unsigned int max_sectors;
    unsigned int cdb_len;
    long unsigned int pio_mask;
    long unsigned int mwdma_mask;
    long unsigned int udma_mask;
    u16 cylinders;
    u16 heads;
    u16 sectors;
    u16 id[256];
    u32 gscr[128];
    u8 devslp_timing[8];
    u8 ncq_send_recv_cmds[20];
    u8 ncq_non_data_cmds[64];
    u32 zac_zoned_cap;
    u32 zac_zones_optimal_open;
    u32 zac_zones_optimal_nonseq;
    u32 zac_zones_max_open;
    int spdn_cnt;
    struct ata_ering ering;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ata_device {
    struct ata_link *link;
    unsigned int devno;
    unsigned int horkage;
    long unsigned int flags;
    struct scsi_device *sdev;
    void *private_data;
    union acpi_object *gtf_cache;
    unsigned int gtf_filter;
    void *zpodd;
    struct device tdev;
    u64 n_sectors;
    u64 n_native_sectors;
    unsigned int class;
    long unsigned int unpark_deadline;
    u8 pio_mode;
    u8 dma_mode;
    u8 xfer_mode;
    unsigned int xfer_shift;
    unsigned int multi_count;
    unsigned int max_sectors;
    unsigned int cdb_len;
    long unsigned int pio_mask;
    long unsigned int mwdma_mask;
    long unsigned int udma_mask;
    u16 cylinders;
    u16 heads;
    u16 sectors;
    u16 id[256];
    u32 gscr[128];
    u8 devslp_timing[8];
    u8 ncq_send_recv_cmds[20];
    u8 ncq_non_data_cmds[64];
    u32 zac_zoned_cap;
    u32 zac_zones_optimal_open;
    u32 zac_zones_optimal_nonseq;
    u32 zac_zones_max_open;
    int spdn_cnt;
    struct ata_ering ering;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ata_device {
    struct ata_link *link;
    unsigned int devno;
    unsigned int horkage;
    long unsigned int flags;
    struct scsi_device *sdev;
    void *private_data;
    union acpi_object *gtf_cache;
    unsigned int gtf_filter;
    void *zpodd;
    struct device tdev;
    u64 n_sectors;
    u64 n_native_sectors;
    unsigned int class;
    long unsigned int unpark_deadline;
    u8 pio_mode;
    u8 dma_mode;
    u8 xfer_mode;
    unsigned int xfer_shift;
    unsigned int multi_count;
    unsigned int max_sectors;
    unsigned int cdb_len;
    long unsigned int pio_mask;
    long unsigned int mwdma_mask;
    long unsigned int udma_mask;
    u16 cylinders;
    u16 heads;
    u16 sectors;
    u16 id[256];
    u32 gscr[128];
    u8 devslp_timing[8];
    u8 ncq_send_recv_cmds[20];
    u8 ncq_non_data_cmds[64];
    u32 zac_zoned_cap;
    u32 zac_zones_optimal_open;
    u32 zac_zones_optimal_nonseq;
    u32 zac_zones_max_open;
    int spdn_cnt;
    struct ata_ering ering;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ata_device {
    struct ata_link *link;
    unsigned int devno;
    unsigned int horkage;
    long unsigned int flags;
    struct scsi_device *sdev;
    void *private_data;
    union acpi_object *gtf_cache;
    unsigned int gtf_filter;
    void *zpodd;
    struct device tdev;
    u64 n_sectors;
    u64 n_native_sectors;
    unsigned int class;
    long unsigned int unpark_deadline;
    u8 pio_mode;
    u8 dma_mode;
    u8 xfer_mode;
    unsigned int xfer_shift;
    unsigned int multi_count;
    unsigned int max_sectors;
    unsigned int cdb_len;
    long unsigned int pio_mask;
    long unsigned int mwdma_mask;
    long unsigned int udma_mask;
    u16 cylinders;
    u16 heads;
    u16 sectors;
    u16 id[256];
    u32 gscr[128];
    u8 devslp_timing[8];
    u8 ncq_send_recv_cmds[20];
    u8 ncq_non_data_cmds[64];
    u32 zac_zoned_cap;
    u32 zac_zones_optimal_open;
    u32 zac_zones_optimal_nonseq;
    u32 zac_zones_max_open;
    int spdn_cnt;
    struct ata_ering ering;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ata_device {
    struct ata_link *link;
    unsigned int devno;
    unsigned int horkage;
    long unsigned int flags;
    struct scsi_device *sdev;
    void *private_data;
    union acpi_object *gtf_cache;
    unsigned int gtf_filter;
    void *zpodd;
    struct device tdev;
    u64 n_sectors;
    u64 n_native_sectors;
    unsigned int class;
    long unsigned int unpark_deadline;
    u8 pio_mode;
    u8 dma_mode;
    u8 xfer_mode;
    unsigned int xfer_shift;
    unsigned int multi_count;
    unsigned int max_sectors;
    unsigned int cdb_len;
    long unsigned int pio_mask;
    long unsigned int mwdma_mask;
    long unsigned int udma_mask;
    u16 cylinders;
    u16 heads;
    u16 sectors;
    u16 id[256];
    u32 gscr[128];
    u8 devslp_timing[8];
    u8 ncq_send_recv_cmds[20];
    u8 ncq_non_data_cmds[64];
    u32 zac_zoned_cap;
    u32 zac_zones_optimal_open;
    u32 zac_zones_optimal_nonseq;
    u32 zac_zones_max_open;
    int spdn_cnt;
    struct ata_ering ering;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ata_device {
    struct ata_link *link;
    unsigned int devno;
    unsigned int horkage;
    long unsigned int flags;
    struct scsi_device *sdev;
    void *private_data;
    union acpi_object *gtf_cache;
    unsigned int gtf_filter;
    void *zpodd;
    struct device tdev;
    u64 n_sectors;
    u64 n_native_sectors;
    unsigned int class;
    long unsigned int unpark_deadline;
    u8 pio_mode;
    u8 dma_mode;
    u8 xfer_mode;
    unsigned int xfer_shift;
    unsigned int multi_count;
    unsigned int max_sectors;
    unsigned int cdb_len;
    long unsigned int pio_mask;
    long unsigned int mwdma_mask;
    long unsigned int udma_mask;
    u16 cylinders;
    u16 heads;
    u16 sectors;
    u16 id[256];
    u32 gscr[128];
    u8 devslp_timing[8];
    u8 ncq_send_recv_cmds[20];
    u8 ncq_non_data_cmds[64];
    u32 zac_zoned_cap;
    u32 zac_zones_optimal_open;
    u32 zac_zones_optimal_nonseq;
    u32 zac_zones_max_open;
    struct ata_cpr_log *cpr_log;
    int spdn_cnt;
    struct ata_ering ering;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ata_device {
    struct ata_link *link;
    unsigned int devno;
    unsigned int horkage;
    long unsigned int flags;
    struct scsi_device *sdev;
    void *private_data;
    union acpi_object *gtf_cache;
    unsigned int gtf_filter;
    void *zpodd;
    struct device tdev;
    u64 n_sectors;
    u64 n_native_sectors;
    unsigned int class;
    long unsigned int unpark_deadline;
    u8 pio_mode;
    u8 dma_mode;
    u8 xfer_mode;
    unsigned int xfer_shift;
    unsigned int multi_count;
    unsigned int max_sectors;
    unsigned int cdb_len;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    u16 cylinders;
    u16 heads;
    u16 sectors;
    u16 id[256];
    u32 gscr[128];
    u8 devslp_timing[8];
    u8 ncq_send_recv_cmds[20];
    u8 ncq_non_data_cmds[64];
    u32 zac_zoned_cap;
    u32 zac_zones_optimal_open;
    u32 zac_zones_optimal_nonseq;
    u32 zac_zones_max_open;
    struct ata_cpr_log *cpr_log;
    int spdn_cnt;
    struct ata_ering ering;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ata_device {
    struct ata_link *link;
    unsigned int devno;
    unsigned int horkage;
    long unsigned int flags;
    struct scsi_device *sdev;
    void *private_data;
    union acpi_object *gtf_cache;
    unsigned int gtf_filter;
    void *zpodd;
    struct device tdev;
    u64 n_sectors;
    u64 n_native_sectors;
    unsigned int class;
    long unsigned int unpark_deadline;
    u8 pio_mode;
    u8 dma_mode;
    u8 xfer_mode;
    unsigned int xfer_shift;
    unsigned int multi_count;
    unsigned int max_sectors;
    unsigned int cdb_len;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    u16 cylinders;
    u16 heads;
    u16 sectors;
    u16 id[256];
    u32 gscr[128];
    u8 devslp_timing[8];
    u8 ncq_send_recv_cmds[20];
    u8 ncq_non_data_cmds[64];
    u32 zac_zoned_cap;
    u32 zac_zones_optimal_open;
    u32 zac_zones_optimal_nonseq;
    u32 zac_zones_max_open;
    struct ata_cpr_log *cpr_log;
    u8 cdl[512];
    int spdn_cnt;
    struct ata_ering ering;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ata_device {
    struct ata_link *link;
    unsigned int devno;
    unsigned int horkage;
    long unsigned int flags;
    struct scsi_device *sdev;
    void *private_data;
    union acpi_object *gtf_cache;
    unsigned int gtf_filter;
    void *zpodd;
    struct device tdev;
    u64 n_sectors;
    u64 n_native_sectors;
    unsigned int class;
    long unsigned int unpark_deadline;
    u8 pio_mode;
    u8 dma_mode;
    u8 xfer_mode;
    unsigned int xfer_shift;
    unsigned int multi_count;
    unsigned int max_sectors;
    unsigned int cdb_len;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    u16 cylinders;
    u16 heads;
    u16 sectors;
    u16 id[256];
    u32 gscr[128];
    u8 devslp_timing[8];
    u8 ncq_send_recv_cmds[20];
    u8 ncq_non_data_cmds[64];
    u32 zac_zoned_cap;
    u32 zac_zones_optimal_open;
    u32 zac_zones_optimal_nonseq;
    u32 zac_zones_max_open;
    struct ata_cpr_log *cpr_log;
    u8 cdl[512];
    int spdn_cnt;
    struct ata_ering ering;
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
struct ata_device {
    struct ata_link *link;
    unsigned int devno;
    unsigned int horkage;
    long unsigned int flags;
    struct scsi_device *sdev;
    void *private_data;
    union acpi_object *gtf_cache;
    unsigned int gtf_filter;
    void *zpodd;
    struct device tdev;
    u64 n_sectors;
    u64 n_native_sectors;
    unsigned int class;
    long unsigned int unpark_deadline;
    u8 pio_mode;
    u8 dma_mode;
    u8 xfer_mode;
    unsigned int xfer_shift;
    unsigned int multi_count;
    unsigned int max_sectors;
    unsigned int cdb_len;
    long unsigned int pio_mask;
    long unsigned int mwdma_mask;
    long unsigned int udma_mask;
    u16 cylinders;
    u16 heads;
    u16 sectors;
    u16 id[256];
    u32 gscr[128];
    u8 devslp_timing[8];
    u8 ncq_send_recv_cmds[20];
    u8 ncq_non_data_cmds[64];
    u32 zac_zoned_cap;
    u32 zac_zones_optimal_open;
    u32 zac_zones_optimal_nonseq;
    u32 zac_zones_max_open;
    int spdn_cnt;
    struct ata_ering ering;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ata_device {
    struct ata_link *link;
    unsigned int devno;
    unsigned int horkage;
    long unsigned int flags;
    struct scsi_device *sdev;
    void *private_data;
    struct device tdev;
    u64 n_sectors;
    u64 n_native_sectors;
    unsigned int class;
    long unsigned int unpark_deadline;
    u8 pio_mode;
    u8 dma_mode;
    u8 xfer_mode;
    unsigned int xfer_shift;
    unsigned int multi_count;
    unsigned int max_sectors;
    unsigned int cdb_len;
    long unsigned int pio_mask;
    long unsigned int mwdma_mask;
    long unsigned int udma_mask;
    u16 cylinders;
    u16 heads;
    u16 sectors;
    u16 id[256];
    u32 gscr[128];
    u8 devslp_timing[8];
    u8 ncq_send_recv_cmds[20];
    u8 ncq_non_data_cmds[64];
    u32 zac_zoned_cap;
    u32 zac_zones_optimal_open;
    u32 zac_zones_optimal_nonseq;
    u32 zac_zones_max_open;
    int spdn_cnt;
    struct ata_ering ering;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ata_device {
    struct ata_link *link;
    unsigned int devno;
    unsigned int horkage;
    long unsigned int flags;
    struct scsi_device *sdev;
    void *private_data;
    struct device tdev;
    u64 n_sectors;
    u64 n_native_sectors;
    unsigned int class;
    long unsigned int unpark_deadline;
    u8 pio_mode;
    u8 dma_mode;
    u8 xfer_mode;
    unsigned int xfer_shift;
    unsigned int multi_count;
    unsigned int max_sectors;
    unsigned int cdb_len;
    long unsigned int pio_mask;
    long unsigned int mwdma_mask;
    long unsigned int udma_mask;
    u16 cylinders;
    u16 heads;
    u16 sectors;
    u16 id[256];
    u32 gscr[128];
    u8 devslp_timing[8];
    u8 ncq_send_recv_cmds[20];
    u8 ncq_non_data_cmds[64];
    u32 zac_zoned_cap;
    u32 zac_zones_optimal_open;
    u32 zac_zones_optimal_nonseq;
    u32 zac_zones_max_open;
    int spdn_cnt;
    struct ata_ering ering;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ata_device {
    struct ata_link *link;
    unsigned int devno;
    unsigned int horkage;
    long unsigned int flags;
    struct scsi_device *sdev;
    void *private_data;
    struct device tdev;
    u64 n_sectors;
    u64 n_native_sectors;
    unsigned int class;
    long unsigned int unpark_deadline;
    u8 pio_mode;
    u8 dma_mode;
    u8 xfer_mode;
    unsigned int xfer_shift;
    unsigned int multi_count;
    unsigned int max_sectors;
    unsigned int cdb_len;
    long unsigned int pio_mask;
    long unsigned int mwdma_mask;
    long unsigned int udma_mask;
    u16 cylinders;
    u16 heads;
    u16 sectors;
    u16 id[256];
    u32 gscr[128];
    u8 devslp_timing[8];
    u8 ncq_send_recv_cmds[20];
    u8 ncq_non_data_cmds[64];
    u32 zac_zoned_cap;
    u32 zac_zones_optimal_open;
    u32 zac_zones_optimal_nonseq;
    u32 zac_zones_max_open;
    int spdn_cnt;
    struct ata_ering ering;
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
struct ata_device {
    struct ata_link *link;
    unsigned int devno;
    unsigned int horkage;
    long unsigned int flags;
    struct scsi_device *sdev;
    void *private_data;
    union acpi_object *gtf_cache;
    unsigned int gtf_filter;
    struct device tdev;
    u64 n_sectors;
    u64 n_native_sectors;
    unsigned int class;
    long unsigned int unpark_deadline;
    u8 pio_mode;
    u8 dma_mode;
    u8 xfer_mode;
    unsigned int xfer_shift;
    unsigned int multi_count;
    unsigned int max_sectors;
    unsigned int cdb_len;
    long unsigned int pio_mask;
    long unsigned int mwdma_mask;
    long unsigned int udma_mask;
    u16 cylinders;
    u16 heads;
    u16 sectors;
    u16 id[256];
    u32 gscr[128];
    u8 devslp_timing[8];
    u8 ncq_send_recv_cmds[20];
    u8 ncq_non_data_cmds[64];
    u32 zac_zoned_cap;
    u32 zac_zones_optimal_open;
    u32 zac_zones_optimal_nonseq;
    u32 zac_zones_max_open;
    int spdn_cnt;
    struct ata_ering ering;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ata_device {
    struct ata_link *link;
    unsigned int devno;
    unsigned int horkage;
    long unsigned int flags;
    struct scsi_device *sdev;
    void *private_data;
    union acpi_object *gtf_cache;
    unsigned int gtf_filter;
    struct device tdev;
    u64 n_sectors;
    u64 n_native_sectors;
    unsigned int class;
    long unsigned int unpark_deadline;
    u8 pio_mode;
    u8 dma_mode;
    u8 xfer_mode;
    unsigned int xfer_shift;
    unsigned int multi_count;
    unsigned int max_sectors;
    unsigned int cdb_len;
    long unsigned int pio_mask;
    long unsigned int mwdma_mask;
    long unsigned int udma_mask;
    u16 cylinders;
    u16 heads;
    u16 sectors;
    u16 id[256];
    u32 gscr[128];
    u8 devslp_timing[8];
    u8 ncq_send_recv_cmds[20];
    u8 ncq_non_data_cmds[64];
    u32 zac_zoned_cap;
    u32 zac_zones_optimal_open;
    u32 zac_zones_optimal_nonseq;
    u32 zac_zones_max_open;
    int spdn_cnt;
    struct ata_ering ering;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ata_device {
    struct ata_link *link;
    unsigned int devno;
    unsigned int horkage;
    long unsigned int flags;
    struct scsi_device *sdev;
    void *private_data;
    union acpi_object *gtf_cache;
    unsigned int gtf_filter;
    void *zpodd;
    struct device tdev;
    u64 n_sectors;
    u64 n_native_sectors;
    unsigned int class;
    long unsigned int unpark_deadline;
    u8 pio_mode;
    u8 dma_mode;
    u8 xfer_mode;
    unsigned int xfer_shift;
    unsigned int multi_count;
    unsigned int max_sectors;
    unsigned int cdb_len;
    long unsigned int pio_mask;
    long unsigned int mwdma_mask;
    long unsigned int udma_mask;
    u16 cylinders;
    u16 heads;
    u16 sectors;
    u16 id[256];
    u32 gscr[128];
    u8 devslp_timing[8];
    u8 ncq_send_recv_cmds[20];
    u8 ncq_non_data_cmds[64];
    u32 zac_zoned_cap;
    u32 zac_zones_optimal_open;
    u32 zac_zones_optimal_nonseq;
    u32 zac_zones_max_open;
    int spdn_cnt;
    struct ata_ering ering;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ata_device {
    struct ata_link *link;
    unsigned int devno;
    unsigned int horkage;
    long unsigned int flags;
    struct scsi_device *sdev;
    void *private_data;
    union acpi_object *gtf_cache;
    unsigned int gtf_filter;
    void *zpodd;
    struct device tdev;
    u64 n_sectors;
    u64 n_native_sectors;
    unsigned int class;
    long unsigned int unpark_deadline;
    u8 pio_mode;
    u8 dma_mode;
    u8 xfer_mode;
    unsigned int xfer_shift;
    unsigned int multi_count;
    unsigned int max_sectors;
    unsigned int cdb_len;
    long unsigned int pio_mask;
    long unsigned int mwdma_mask;
    long unsigned int udma_mask;
    u16 cylinders;
    u16 heads;
    u16 sectors;
    u16 id[256];
    u32 gscr[128];
    u8 devslp_timing[8];
    u8 ncq_send_recv_cmds[20];
    u8 ncq_non_data_cmds[64];
    u32 zac_zoned_cap;
    u32 zac_zones_optimal_open;
    u32 zac_zones_optimal_nonseq;
    u32 zac_zones_max_open;
    int spdn_cnt;
    struct ata_ering ering;
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
<code>u8 ncq_non_data_cmds[64]</code>
</li>
<li>
<b>Field added. </b>
<code>u32 zac_zoned_cap</code>
</li>
<li>
<b>Field added. </b>
<code>u32 zac_zones_optimal_open</code>
</li>
<li>
<b>Field added. </b>
<code>u32 zac_zones_optimal_nonseq</code>
</li>
<li>
<b>Field added. </b>
<code>u32 zac_zones_max_open</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 ncq_send_recv_cmds[16]</code> ➡️ <code>u8 ncq_send_recv_cmds[20]</code>
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
No changes between <code>4.18</code> and <code>5.0</code> ✅
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct ata_cpr_log *cpr_log</code>
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
<code>long unsigned int pio_mask</code> ➡️ <code>unsigned int pio_mask</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int mwdma_mask</code> ➡️ <code>unsigned int mwdma_mask</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int udma_mask</code> ➡️ <code>unsigned int udma_mask</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 cdl[512]</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>union acpi_object *gtf_cache</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int gtf_filter</code>
</li>
<li>
<b>Field removed. </b>
<code>void *zpodd</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>union acpi_object *gtf_cache</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int gtf_filter</code>
</li>
<li>
<b>Field removed. </b>
<code>void *zpodd</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>union acpi_object *gtf_cache</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int gtf_filter</code>
</li>
<li>
<b>Field removed. </b>
<code>void *zpodd</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
<details>
<summary>Changed between <code>generic</code> and <code>aws</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>void *zpodd</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>generic</code> and <code>azure</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>void *zpodd</code>
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
