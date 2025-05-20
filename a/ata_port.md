# Struct: <code>ata_port</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct ata_port {
    struct Scsi_Host *scsi_host;
    struct ata_port_operations *ops;
    spinlock_t *lock;
    long unsigned int flags;
    unsigned int pflags;
    unsigned int print_id;
    unsigned int local_port_no;
    unsigned int port_no;
    struct ata_ioports ioaddr;
    u8 ctl;
    u8 last_ctl;
    struct ata_link *sff_pio_task_link;
    struct delayed_work sff_pio_task;
    struct ata_bmdma_prd *bmdma_prd;
    dma_addr_t bmdma_prd_dma;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    unsigned int cbl;
    struct ata_queued_cmd qcmd[32];
    long unsigned int sas_tag_allocated;
    unsigned int qc_active;
    int nr_active_links;
    unsigned int sas_last_tag;
    struct ata_link link;
    struct ata_link *slave_link;
    int nr_pmp_links;
    struct ata_link *pmp_link;
    struct ata_link *excl_link;
    struct ata_port_stats stats;
    struct ata_host *host;
    struct device *dev;
    struct device tdev;
    struct mutex scsi_scan_mutex;
    struct delayed_work hotplug_task;
    struct work_struct scsi_rescan_task;
    unsigned int hsm_task_state;
    u32 msg_enable;
    struct list_head eh_done_q;
    wait_queue_head_t eh_wait_q;
    int eh_tries;
    struct completion park_req_pending;
    pm_message_t pm_mesg;
    enum ata_lpm_policy target_lpm_policy;
    struct timer_list fastdrain_timer;
    long unsigned int fastdrain_cnt;
    int em_message_type;
    void *private_data;
    struct ata_acpi_gtm __acpi_init_gtm;
    u8 sector_buf[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ata_port {
    struct Scsi_Host *scsi_host;
    struct ata_port_operations *ops;
    spinlock_t *lock;
    long unsigned int flags;
    unsigned int pflags;
    unsigned int print_id;
    unsigned int local_port_no;
    unsigned int port_no;
    struct ata_ioports ioaddr;
    u8 ctl;
    u8 last_ctl;
    struct ata_link *sff_pio_task_link;
    struct delayed_work sff_pio_task;
    struct ata_bmdma_prd *bmdma_prd;
    dma_addr_t bmdma_prd_dma;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    unsigned int cbl;
    struct ata_queued_cmd qcmd[32];
    long unsigned int sas_tag_allocated;
    unsigned int qc_active;
    int nr_active_links;
    unsigned int sas_last_tag;
    struct ata_link link;
    struct ata_link *slave_link;
    int nr_pmp_links;
    struct ata_link *pmp_link;
    struct ata_link *excl_link;
    struct ata_port_stats stats;
    struct ata_host *host;
    struct device *dev;
    struct device tdev;
    struct mutex scsi_scan_mutex;
    struct delayed_work hotplug_task;
    struct work_struct scsi_rescan_task;
    unsigned int hsm_task_state;
    u32 msg_enable;
    struct list_head eh_done_q;
    wait_queue_head_t eh_wait_q;
    int eh_tries;
    struct completion park_req_pending;
    pm_message_t pm_mesg;
    enum ata_lpm_policy target_lpm_policy;
    struct timer_list fastdrain_timer;
    long unsigned int fastdrain_cnt;
    int em_message_type;
    void *private_data;
    struct ata_acpi_gtm __acpi_init_gtm;
    u8 sector_buf[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ata_port {
    struct Scsi_Host *scsi_host;
    struct ata_port_operations *ops;
    spinlock_t *lock;
    long unsigned int flags;
    unsigned int pflags;
    unsigned int print_id;
    unsigned int local_port_no;
    unsigned int port_no;
    struct ata_ioports ioaddr;
    u8 ctl;
    u8 last_ctl;
    struct ata_link *sff_pio_task_link;
    struct delayed_work sff_pio_task;
    struct ata_bmdma_prd *bmdma_prd;
    dma_addr_t bmdma_prd_dma;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    unsigned int cbl;
    struct ata_queued_cmd qcmd[32];
    long unsigned int sas_tag_allocated;
    unsigned int qc_active;
    int nr_active_links;
    unsigned int sas_last_tag;
    struct ata_link link;
    struct ata_link *slave_link;
    int nr_pmp_links;
    struct ata_link *pmp_link;
    struct ata_link *excl_link;
    struct ata_port_stats stats;
    struct ata_host *host;
    struct device *dev;
    struct device tdev;
    struct mutex scsi_scan_mutex;
    struct delayed_work hotplug_task;
    struct work_struct scsi_rescan_task;
    unsigned int hsm_task_state;
    u32 msg_enable;
    struct list_head eh_done_q;
    wait_queue_head_t eh_wait_q;
    int eh_tries;
    struct completion park_req_pending;
    pm_message_t pm_mesg;
    enum ata_lpm_policy target_lpm_policy;
    struct timer_list fastdrain_timer;
    long unsigned int fastdrain_cnt;
    int em_message_type;
    void *private_data;
    struct ata_acpi_gtm __acpi_init_gtm;
    u8 sector_buf[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ata_port {
    struct Scsi_Host *scsi_host;
    struct ata_port_operations *ops;
    spinlock_t *lock;
    long unsigned int flags;
    unsigned int pflags;
    unsigned int print_id;
    unsigned int local_port_no;
    unsigned int port_no;
    struct ata_ioports ioaddr;
    u8 ctl;
    u8 last_ctl;
    struct ata_link *sff_pio_task_link;
    struct delayed_work sff_pio_task;
    struct ata_bmdma_prd *bmdma_prd;
    dma_addr_t bmdma_prd_dma;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    unsigned int cbl;
    struct ata_queued_cmd qcmd[32];
    long unsigned int sas_tag_allocated;
    unsigned int qc_active;
    int nr_active_links;
    unsigned int sas_last_tag;
    struct ata_link link;
    struct ata_link *slave_link;
    int nr_pmp_links;
    struct ata_link *pmp_link;
    struct ata_link *excl_link;
    struct ata_port_stats stats;
    struct ata_host *host;
    struct device *dev;
    struct device tdev;
    struct mutex scsi_scan_mutex;
    struct delayed_work hotplug_task;
    struct work_struct scsi_rescan_task;
    unsigned int hsm_task_state;
    u32 msg_enable;
    struct list_head eh_done_q;
    wait_queue_head_t eh_wait_q;
    int eh_tries;
    struct completion park_req_pending;
    pm_message_t pm_mesg;
    enum ata_lpm_policy target_lpm_policy;
    struct timer_list fastdrain_timer;
    long unsigned int fastdrain_cnt;
    int em_message_type;
    void *private_data;
    struct ata_acpi_gtm __acpi_init_gtm;
    u8 sector_buf[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ata_port {
    struct Scsi_Host *scsi_host;
    struct ata_port_operations *ops;
    spinlock_t *lock;
    long unsigned int flags;
    unsigned int pflags;
    unsigned int print_id;
    unsigned int local_port_no;
    unsigned int port_no;
    struct ata_ioports ioaddr;
    u8 ctl;
    u8 last_ctl;
    struct ata_link *sff_pio_task_link;
    struct delayed_work sff_pio_task;
    struct ata_bmdma_prd *bmdma_prd;
    dma_addr_t bmdma_prd_dma;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    unsigned int cbl;
    struct ata_queued_cmd qcmd[32];
    long unsigned int sas_tag_allocated;
    unsigned int qc_active;
    int nr_active_links;
    unsigned int sas_last_tag;
    struct ata_link link;
    struct ata_link *slave_link;
    int nr_pmp_links;
    struct ata_link *pmp_link;
    struct ata_link *excl_link;
    struct ata_port_stats stats;
    struct ata_host *host;
    struct device *dev;
    struct device tdev;
    struct mutex scsi_scan_mutex;
    struct delayed_work hotplug_task;
    struct work_struct scsi_rescan_task;
    unsigned int hsm_task_state;
    u32 msg_enable;
    struct list_head eh_done_q;
    wait_queue_head_t eh_wait_q;
    int eh_tries;
    struct completion park_req_pending;
    pm_message_t pm_mesg;
    enum ata_lpm_policy target_lpm_policy;
    struct timer_list fastdrain_timer;
    long unsigned int fastdrain_cnt;
    int em_message_type;
    void *private_data;
    struct ata_acpi_gtm __acpi_init_gtm;
    u8 sector_buf[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ata_port {
    struct Scsi_Host *scsi_host;
    struct ata_port_operations *ops;
    spinlock_t *lock;
    long unsigned int flags;
    unsigned int pflags;
    unsigned int print_id;
    unsigned int local_port_no;
    unsigned int port_no;
    struct ata_ioports ioaddr;
    u8 ctl;
    u8 last_ctl;
    struct ata_link *sff_pio_task_link;
    struct delayed_work sff_pio_task;
    struct ata_bmdma_prd *bmdma_prd;
    dma_addr_t bmdma_prd_dma;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    unsigned int cbl;
    struct ata_queued_cmd qcmd[33];
    long unsigned int sas_tag_allocated;
    u64 qc_active;
    int nr_active_links;
    unsigned int sas_last_tag;
    struct ata_link link;
    struct ata_link *slave_link;
    int nr_pmp_links;
    struct ata_link *pmp_link;
    struct ata_link *excl_link;
    struct ata_port_stats stats;
    struct ata_host *host;
    struct device *dev;
    struct device tdev;
    struct mutex scsi_scan_mutex;
    struct delayed_work hotplug_task;
    struct work_struct scsi_rescan_task;
    unsigned int hsm_task_state;
    u32 msg_enable;
    struct list_head eh_done_q;
    wait_queue_head_t eh_wait_q;
    int eh_tries;
    struct completion park_req_pending;
    pm_message_t pm_mesg;
    enum ata_lpm_policy target_lpm_policy;
    struct timer_list fastdrain_timer;
    long unsigned int fastdrain_cnt;
    int em_message_type;
    void *private_data;
    struct ata_acpi_gtm __acpi_init_gtm;
    u8 sector_buf[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ata_port {
    struct Scsi_Host *scsi_host;
    struct ata_port_operations *ops;
    spinlock_t *lock;
    long unsigned int flags;
    unsigned int pflags;
    unsigned int print_id;
    unsigned int local_port_no;
    unsigned int port_no;
    struct ata_ioports ioaddr;
    u8 ctl;
    u8 last_ctl;
    struct ata_link *sff_pio_task_link;
    struct delayed_work sff_pio_task;
    struct ata_bmdma_prd *bmdma_prd;
    dma_addr_t bmdma_prd_dma;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    unsigned int cbl;
    struct ata_queued_cmd qcmd[33];
    long unsigned int sas_tag_allocated;
    u64 qc_active;
    int nr_active_links;
    unsigned int sas_last_tag;
    struct ata_link link;
    struct ata_link *slave_link;
    int nr_pmp_links;
    struct ata_link *pmp_link;
    struct ata_link *excl_link;
    struct ata_port_stats stats;
    struct ata_host *host;
    struct device *dev;
    struct device tdev;
    struct mutex scsi_scan_mutex;
    struct delayed_work hotplug_task;
    struct work_struct scsi_rescan_task;
    unsigned int hsm_task_state;
    u32 msg_enable;
    struct list_head eh_done_q;
    wait_queue_head_t eh_wait_q;
    int eh_tries;
    struct completion park_req_pending;
    pm_message_t pm_mesg;
    enum ata_lpm_policy target_lpm_policy;
    struct timer_list fastdrain_timer;
    long unsigned int fastdrain_cnt;
    int em_message_type;
    void *private_data;
    struct ata_acpi_gtm __acpi_init_gtm;
    u8 sector_buf[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ata_port {
    struct Scsi_Host *scsi_host;
    struct ata_port_operations *ops;
    spinlock_t *lock;
    long unsigned int flags;
    unsigned int pflags;
    unsigned int print_id;
    unsigned int local_port_no;
    unsigned int port_no;
    struct ata_ioports ioaddr;
    u8 ctl;
    u8 last_ctl;
    struct ata_link *sff_pio_task_link;
    struct delayed_work sff_pio_task;
    struct ata_bmdma_prd *bmdma_prd;
    dma_addr_t bmdma_prd_dma;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    unsigned int cbl;
    struct ata_queued_cmd qcmd[33];
    long unsigned int sas_tag_allocated;
    u64 qc_active;
    int nr_active_links;
    unsigned int sas_last_tag;
    struct ata_link link;
    struct ata_link *slave_link;
    int nr_pmp_links;
    struct ata_link *pmp_link;
    struct ata_link *excl_link;
    struct ata_port_stats stats;
    struct ata_host *host;
    struct device *dev;
    struct device tdev;
    struct mutex scsi_scan_mutex;
    struct delayed_work hotplug_task;
    struct work_struct scsi_rescan_task;
    unsigned int hsm_task_state;
    u32 msg_enable;
    struct list_head eh_done_q;
    wait_queue_head_t eh_wait_q;
    int eh_tries;
    struct completion park_req_pending;
    pm_message_t pm_mesg;
    enum ata_lpm_policy target_lpm_policy;
    struct timer_list fastdrain_timer;
    long unsigned int fastdrain_cnt;
    int em_message_type;
    void *private_data;
    struct ata_acpi_gtm __acpi_init_gtm;
    u8 sector_buf[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ata_port {
    struct Scsi_Host *scsi_host;
    struct ata_port_operations *ops;
    spinlock_t *lock;
    long unsigned int flags;
    unsigned int pflags;
    unsigned int print_id;
    unsigned int local_port_no;
    unsigned int port_no;
    struct ata_ioports ioaddr;
    u8 ctl;
    u8 last_ctl;
    struct ata_link *sff_pio_task_link;
    struct delayed_work sff_pio_task;
    struct ata_bmdma_prd *bmdma_prd;
    dma_addr_t bmdma_prd_dma;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    unsigned int cbl;
    struct ata_queued_cmd qcmd[33];
    long unsigned int sas_tag_allocated;
    u64 qc_active;
    int nr_active_links;
    unsigned int sas_last_tag;
    struct ata_link link;
    struct ata_link *slave_link;
    int nr_pmp_links;
    struct ata_link *pmp_link;
    struct ata_link *excl_link;
    struct ata_port_stats stats;
    struct ata_host *host;
    struct device *dev;
    struct device tdev;
    struct mutex scsi_scan_mutex;
    struct delayed_work hotplug_task;
    struct work_struct scsi_rescan_task;
    unsigned int hsm_task_state;
    u32 msg_enable;
    struct list_head eh_done_q;
    wait_queue_head_t eh_wait_q;
    int eh_tries;
    struct completion park_req_pending;
    pm_message_t pm_mesg;
    enum ata_lpm_policy target_lpm_policy;
    struct timer_list fastdrain_timer;
    long unsigned int fastdrain_cnt;
    int em_message_type;
    void *private_data;
    struct ata_acpi_gtm __acpi_init_gtm;
    u8 sector_buf[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ata_port {
    struct Scsi_Host *scsi_host;
    struct ata_port_operations *ops;
    spinlock_t *lock;
    long unsigned int flags;
    unsigned int pflags;
    unsigned int print_id;
    unsigned int local_port_no;
    unsigned int port_no;
    struct ata_ioports ioaddr;
    u8 ctl;
    u8 last_ctl;
    struct ata_link *sff_pio_task_link;
    struct delayed_work sff_pio_task;
    struct ata_bmdma_prd *bmdma_prd;
    dma_addr_t bmdma_prd_dma;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    unsigned int cbl;
    struct ata_queued_cmd qcmd[33];
    long unsigned int sas_tag_allocated;
    u64 qc_active;
    int nr_active_links;
    unsigned int sas_last_tag;
    struct ata_link link;
    struct ata_link *slave_link;
    int nr_pmp_links;
    struct ata_link *pmp_link;
    struct ata_link *excl_link;
    struct ata_port_stats stats;
    struct ata_host *host;
    struct device *dev;
    struct device tdev;
    struct mutex scsi_scan_mutex;
    struct delayed_work hotplug_task;
    struct work_struct scsi_rescan_task;
    unsigned int hsm_task_state;
    u32 msg_enable;
    struct list_head eh_done_q;
    wait_queue_head_t eh_wait_q;
    int eh_tries;
    struct completion park_req_pending;
    pm_message_t pm_mesg;
    enum ata_lpm_policy target_lpm_policy;
    struct timer_list fastdrain_timer;
    long unsigned int fastdrain_cnt;
    async_cookie_t cookie;
    int em_message_type;
    void *private_data;
    struct ata_acpi_gtm __acpi_init_gtm;
    u8 sector_buf[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ata_port {
    struct Scsi_Host *scsi_host;
    struct ata_port_operations *ops;
    spinlock_t *lock;
    long unsigned int flags;
    unsigned int pflags;
    unsigned int print_id;
    unsigned int local_port_no;
    unsigned int port_no;
    struct ata_ioports ioaddr;
    u8 ctl;
    u8 last_ctl;
    struct ata_link *sff_pio_task_link;
    struct delayed_work sff_pio_task;
    struct ata_bmdma_prd *bmdma_prd;
    dma_addr_t bmdma_prd_dma;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    unsigned int cbl;
    struct ata_queued_cmd qcmd[33];
    long unsigned int sas_tag_allocated;
    u64 qc_active;
    int nr_active_links;
    unsigned int sas_last_tag;
    struct ata_link link;
    struct ata_link *slave_link;
    int nr_pmp_links;
    struct ata_link *pmp_link;
    struct ata_link *excl_link;
    struct ata_port_stats stats;
    struct ata_host *host;
    struct device *dev;
    struct device tdev;
    struct mutex scsi_scan_mutex;
    struct delayed_work hotplug_task;
    struct work_struct scsi_rescan_task;
    unsigned int hsm_task_state;
    u32 msg_enable;
    struct list_head eh_done_q;
    wait_queue_head_t eh_wait_q;
    int eh_tries;
    struct completion park_req_pending;
    pm_message_t pm_mesg;
    enum ata_lpm_policy target_lpm_policy;
    struct timer_list fastdrain_timer;
    long unsigned int fastdrain_cnt;
    async_cookie_t cookie;
    int em_message_type;
    void *private_data;
    struct ata_acpi_gtm __acpi_init_gtm;
    u8 sector_buf[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ata_port {
    struct Scsi_Host *scsi_host;
    struct ata_port_operations *ops;
    spinlock_t *lock;
    long unsigned int flags;
    unsigned int pflags;
    unsigned int print_id;
    unsigned int local_port_no;
    unsigned int port_no;
    struct ata_ioports ioaddr;
    u8 ctl;
    u8 last_ctl;
    struct ata_link *sff_pio_task_link;
    struct delayed_work sff_pio_task;
    struct ata_bmdma_prd *bmdma_prd;
    dma_addr_t bmdma_prd_dma;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    unsigned int cbl;
    struct ata_queued_cmd qcmd[33];
    long unsigned int sas_tag_allocated;
    u64 qc_active;
    int nr_active_links;
    unsigned int sas_last_tag;
    struct ata_link link;
    struct ata_link *slave_link;
    int nr_pmp_links;
    struct ata_link *pmp_link;
    struct ata_link *excl_link;
    struct ata_port_stats stats;
    struct ata_host *host;
    struct device *dev;
    struct device tdev;
    struct mutex scsi_scan_mutex;
    struct delayed_work hotplug_task;
    struct work_struct scsi_rescan_task;
    unsigned int hsm_task_state;
    u32 msg_enable;
    struct list_head eh_done_q;
    wait_queue_head_t eh_wait_q;
    int eh_tries;
    struct completion park_req_pending;
    pm_message_t pm_mesg;
    enum ata_lpm_policy target_lpm_policy;
    struct timer_list fastdrain_timer;
    long unsigned int fastdrain_cnt;
    async_cookie_t cookie;
    int em_message_type;
    void *private_data;
    struct ata_acpi_gtm __acpi_init_gtm;
    u8 sector_buf[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ata_port {
    struct Scsi_Host *scsi_host;
    struct ata_port_operations *ops;
    spinlock_t *lock;
    long unsigned int flags;
    unsigned int pflags;
    unsigned int print_id;
    unsigned int local_port_no;
    unsigned int port_no;
    struct ata_ioports ioaddr;
    u8 ctl;
    u8 last_ctl;
    struct ata_link *sff_pio_task_link;
    struct delayed_work sff_pio_task;
    struct ata_bmdma_prd *bmdma_prd;
    dma_addr_t bmdma_prd_dma;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    unsigned int cbl;
    struct ata_queued_cmd qcmd[33];
    long unsigned int sas_tag_allocated;
    u64 qc_active;
    int nr_active_links;
    unsigned int sas_last_tag;
    struct ata_link link;
    struct ata_link *slave_link;
    int nr_pmp_links;
    struct ata_link *pmp_link;
    struct ata_link *excl_link;
    struct ata_port_stats stats;
    struct ata_host *host;
    struct device *dev;
    struct device tdev;
    struct mutex scsi_scan_mutex;
    struct delayed_work hotplug_task;
    struct work_struct scsi_rescan_task;
    unsigned int hsm_task_state;
    u32 msg_enable;
    struct list_head eh_done_q;
    wait_queue_head_t eh_wait_q;
    int eh_tries;
    struct completion park_req_pending;
    pm_message_t pm_mesg;
    enum ata_lpm_policy target_lpm_policy;
    struct timer_list fastdrain_timer;
    long unsigned int fastdrain_cnt;
    async_cookie_t cookie;
    int em_message_type;
    void *private_data;
    struct ata_acpi_gtm __acpi_init_gtm;
    u8 sector_buf[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ata_port {
    struct Scsi_Host *scsi_host;
    struct ata_port_operations *ops;
    spinlock_t *lock;
    long unsigned int flags;
    unsigned int pflags;
    unsigned int print_id;
    unsigned int local_port_no;
    unsigned int port_no;
    struct ata_ioports ioaddr;
    u8 ctl;
    u8 last_ctl;
    struct ata_link *sff_pio_task_link;
    struct delayed_work sff_pio_task;
    struct ata_bmdma_prd *bmdma_prd;
    dma_addr_t bmdma_prd_dma;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    unsigned int cbl;
    struct ata_queued_cmd qcmd[33];
    u64 qc_active;
    int nr_active_links;
    struct ata_link link;
    struct ata_link *slave_link;
    int nr_pmp_links;
    struct ata_link *pmp_link;
    struct ata_link *excl_link;
    struct ata_port_stats stats;
    struct ata_host *host;
    struct device *dev;
    struct device tdev;
    struct mutex scsi_scan_mutex;
    struct delayed_work hotplug_task;
    struct work_struct scsi_rescan_task;
    unsigned int hsm_task_state;
    struct list_head eh_done_q;
    wait_queue_head_t eh_wait_q;
    int eh_tries;
    struct completion park_req_pending;
    pm_message_t pm_mesg;
    enum ata_lpm_policy target_lpm_policy;
    struct timer_list fastdrain_timer;
    long unsigned int fastdrain_cnt;
    async_cookie_t cookie;
    int em_message_type;
    void *private_data;
    struct ata_acpi_gtm __acpi_init_gtm;
    u8 sector_buf[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ata_port {
    struct Scsi_Host *scsi_host;
    struct ata_port_operations *ops;
    spinlock_t *lock;
    long unsigned int flags;
    unsigned int pflags;
    unsigned int print_id;
    unsigned int local_port_no;
    unsigned int port_no;
    struct ata_ioports ioaddr;
    u8 ctl;
    u8 last_ctl;
    struct ata_link *sff_pio_task_link;
    struct delayed_work sff_pio_task;
    struct ata_bmdma_prd *bmdma_prd;
    dma_addr_t bmdma_prd_dma;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    unsigned int cbl;
    struct ata_queued_cmd qcmd[33];
    u64 qc_active;
    int nr_active_links;
    struct ata_link link;
    struct ata_link *slave_link;
    int nr_pmp_links;
    struct ata_link *pmp_link;
    struct ata_link *excl_link;
    struct ata_port_stats stats;
    struct ata_host *host;
    struct device *dev;
    struct device tdev;
    struct mutex scsi_scan_mutex;
    struct delayed_work hotplug_task;
    struct work_struct scsi_rescan_task;
    unsigned int hsm_task_state;
    struct list_head eh_done_q;
    wait_queue_head_t eh_wait_q;
    int eh_tries;
    struct completion park_req_pending;
    pm_message_t pm_mesg;
    enum ata_lpm_policy target_lpm_policy;
    struct timer_list fastdrain_timer;
    unsigned int fastdrain_cnt;
    async_cookie_t cookie;
    int em_message_type;
    void *private_data;
    struct ata_acpi_gtm __acpi_init_gtm;
    u8 sector_buf[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ata_port {
    struct Scsi_Host *scsi_host;
    struct ata_port_operations *ops;
    spinlock_t *lock;
    long unsigned int flags;
    unsigned int pflags;
    unsigned int print_id;
    unsigned int local_port_no;
    unsigned int port_no;
    struct ata_ioports ioaddr;
    u8 ctl;
    u8 last_ctl;
    struct ata_link *sff_pio_task_link;
    struct delayed_work sff_pio_task;
    struct ata_bmdma_prd *bmdma_prd;
    dma_addr_t bmdma_prd_dma;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    unsigned int cbl;
    struct ata_queued_cmd qcmd[33];
    u64 qc_active;
    int nr_active_links;
    struct ata_link link;
    struct ata_link *slave_link;
    int nr_pmp_links;
    struct ata_link *pmp_link;
    struct ata_link *excl_link;
    struct ata_port_stats stats;
    struct ata_host *host;
    struct device *dev;
    struct device tdev;
    struct mutex scsi_scan_mutex;
    struct delayed_work hotplug_task;
    struct delayed_work scsi_rescan_task;
    unsigned int hsm_task_state;
    struct list_head eh_done_q;
    wait_queue_head_t eh_wait_q;
    int eh_tries;
    struct completion park_req_pending;
    pm_message_t pm_mesg;
    enum ata_lpm_policy target_lpm_policy;
    struct timer_list fastdrain_timer;
    unsigned int fastdrain_cnt;
    async_cookie_t cookie;
    int em_message_type;
    void *private_data;
    struct ata_acpi_gtm __acpi_init_gtm;
    u8 *ncq_sense_buf;
    u8 sector_buf[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ata_port {
    struct Scsi_Host *scsi_host;
    struct ata_port_operations *ops;
    spinlock_t *lock;
    long unsigned int flags;
    unsigned int pflags;
    unsigned int print_id;
    unsigned int local_port_no;
    unsigned int port_no;
    struct ata_ioports ioaddr;
    u8 ctl;
    u8 last_ctl;
    struct ata_link *sff_pio_task_link;
    struct delayed_work sff_pio_task;
    struct ata_bmdma_prd *bmdma_prd;
    dma_addr_t bmdma_prd_dma;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    unsigned int cbl;
    struct ata_queued_cmd qcmd[33];
    u64 qc_active;
    int nr_active_links;
    struct ata_link link;
    struct ata_link *slave_link;
    int nr_pmp_links;
    struct ata_link *pmp_link;
    struct ata_link *excl_link;
    struct ata_port_stats stats;
    struct ata_host *host;
    struct device *dev;
    struct device tdev;
    struct mutex scsi_scan_mutex;
    struct delayed_work hotplug_task;
    struct delayed_work scsi_rescan_task;
    unsigned int hsm_task_state;
    struct list_head eh_done_q;
    wait_queue_head_t eh_wait_q;
    int eh_tries;
    struct completion park_req_pending;
    pm_message_t pm_mesg;
    enum ata_lpm_policy target_lpm_policy;
    struct timer_list fastdrain_timer;
    unsigned int fastdrain_cnt;
    async_cookie_t cookie;
    int em_message_type;
    void *private_data;
    struct ata_acpi_gtm __acpi_init_gtm;
    u8 *ncq_sense_buf;
    u8 sector_buf[512];
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
struct ata_port {
    struct Scsi_Host *scsi_host;
    struct ata_port_operations *ops;
    spinlock_t *lock;
    long unsigned int flags;
    unsigned int pflags;
    unsigned int print_id;
    unsigned int local_port_no;
    unsigned int port_no;
    struct ata_ioports ioaddr;
    u8 ctl;
    u8 last_ctl;
    struct ata_link *sff_pio_task_link;
    struct delayed_work sff_pio_task;
    struct ata_bmdma_prd *bmdma_prd;
    dma_addr_t bmdma_prd_dma;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    unsigned int cbl;
    struct ata_queued_cmd qcmd[33];
    long unsigned int sas_tag_allocated;
    u64 qc_active;
    int nr_active_links;
    unsigned int sas_last_tag;
    struct ata_link link;
    struct ata_link *slave_link;
    int nr_pmp_links;
    struct ata_link *pmp_link;
    struct ata_link *excl_link;
    struct ata_port_stats stats;
    struct ata_host *host;
    struct device *dev;
    struct device tdev;
    struct mutex scsi_scan_mutex;
    struct delayed_work hotplug_task;
    struct work_struct scsi_rescan_task;
    unsigned int hsm_task_state;
    u32 msg_enable;
    struct list_head eh_done_q;
    wait_queue_head_t eh_wait_q;
    int eh_tries;
    struct completion park_req_pending;
    pm_message_t pm_mesg;
    enum ata_lpm_policy target_lpm_policy;
    struct timer_list fastdrain_timer;
    long unsigned int fastdrain_cnt;
    int em_message_type;
    void *private_data;
    struct ata_acpi_gtm __acpi_init_gtm;
    u8 sector_buf[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ata_port {
    struct Scsi_Host *scsi_host;
    struct ata_port_operations *ops;
    spinlock_t *lock;
    long unsigned int flags;
    unsigned int pflags;
    unsigned int print_id;
    unsigned int local_port_no;
    unsigned int port_no;
    struct ata_ioports ioaddr;
    u8 ctl;
    u8 last_ctl;
    struct ata_link *sff_pio_task_link;
    struct delayed_work sff_pio_task;
    struct ata_bmdma_prd *bmdma_prd;
    dma_addr_t bmdma_prd_dma;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    unsigned int cbl;
    struct ata_queued_cmd qcmd[33];
    long unsigned int sas_tag_allocated;
    u64 qc_active;
    int nr_active_links;
    unsigned int sas_last_tag;
    struct ata_link link;
    struct ata_link *slave_link;
    int nr_pmp_links;
    struct ata_link *pmp_link;
    struct ata_link *excl_link;
    struct ata_port_stats stats;
    struct ata_host *host;
    struct device *dev;
    struct device tdev;
    struct mutex scsi_scan_mutex;
    struct delayed_work hotplug_task;
    struct work_struct scsi_rescan_task;
    unsigned int hsm_task_state;
    u32 msg_enable;
    struct list_head eh_done_q;
    wait_queue_head_t eh_wait_q;
    int eh_tries;
    struct completion park_req_pending;
    pm_message_t pm_mesg;
    enum ata_lpm_policy target_lpm_policy;
    struct timer_list fastdrain_timer;
    long unsigned int fastdrain_cnt;
    int em_message_type;
    void *private_data;
    u8 sector_buf[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ata_port {
    struct Scsi_Host *scsi_host;
    struct ata_port_operations *ops;
    spinlock_t *lock;
    long unsigned int flags;
    unsigned int pflags;
    unsigned int print_id;
    unsigned int local_port_no;
    unsigned int port_no;
    struct ata_ioports ioaddr;
    u8 ctl;
    u8 last_ctl;
    struct ata_link *sff_pio_task_link;
    struct delayed_work sff_pio_task;
    struct ata_bmdma_prd *bmdma_prd;
    dma_addr_t bmdma_prd_dma;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    unsigned int cbl;
    struct ata_queued_cmd qcmd[33];
    long unsigned int sas_tag_allocated;
    u64 qc_active;
    int nr_active_links;
    unsigned int sas_last_tag;
    struct ata_link link;
    struct ata_link *slave_link;
    int nr_pmp_links;
    struct ata_link *pmp_link;
    struct ata_link *excl_link;
    struct ata_port_stats stats;
    struct ata_host *host;
    struct device *dev;
    struct device tdev;
    struct mutex scsi_scan_mutex;
    struct delayed_work hotplug_task;
    struct work_struct scsi_rescan_task;
    unsigned int hsm_task_state;
    u32 msg_enable;
    struct list_head eh_done_q;
    wait_queue_head_t eh_wait_q;
    int eh_tries;
    struct completion park_req_pending;
    pm_message_t pm_mesg;
    enum ata_lpm_policy target_lpm_policy;
    struct timer_list fastdrain_timer;
    long unsigned int fastdrain_cnt;
    int em_message_type;
    void *private_data;
    u8 sector_buf[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ata_port {
    struct Scsi_Host *scsi_host;
    struct ata_port_operations *ops;
    spinlock_t *lock;
    long unsigned int flags;
    unsigned int pflags;
    unsigned int print_id;
    unsigned int local_port_no;
    unsigned int port_no;
    struct ata_ioports ioaddr;
    u8 ctl;
    u8 last_ctl;
    struct ata_link *sff_pio_task_link;
    struct delayed_work sff_pio_task;
    struct ata_bmdma_prd *bmdma_prd;
    dma_addr_t bmdma_prd_dma;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    unsigned int cbl;
    struct ata_queued_cmd qcmd[33];
    long unsigned int sas_tag_allocated;
    u64 qc_active;
    int nr_active_links;
    unsigned int sas_last_tag;
    struct ata_link link;
    struct ata_link *slave_link;
    int nr_pmp_links;
    struct ata_link *pmp_link;
    struct ata_link *excl_link;
    struct ata_port_stats stats;
    struct ata_host *host;
    struct device *dev;
    struct device tdev;
    struct mutex scsi_scan_mutex;
    struct delayed_work hotplug_task;
    struct work_struct scsi_rescan_task;
    unsigned int hsm_task_state;
    u32 msg_enable;
    struct list_head eh_done_q;
    wait_queue_head_t eh_wait_q;
    int eh_tries;
    struct completion park_req_pending;
    pm_message_t pm_mesg;
    enum ata_lpm_policy target_lpm_policy;
    struct timer_list fastdrain_timer;
    long unsigned int fastdrain_cnt;
    int em_message_type;
    void *private_data;
    u8 sector_buf[512];
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
struct ata_port {
    struct Scsi_Host *scsi_host;
    struct ata_port_operations *ops;
    spinlock_t *lock;
    long unsigned int flags;
    unsigned int pflags;
    unsigned int print_id;
    unsigned int local_port_no;
    unsigned int port_no;
    struct ata_ioports ioaddr;
    u8 ctl;
    u8 last_ctl;
    struct ata_link *sff_pio_task_link;
    struct delayed_work sff_pio_task;
    struct ata_bmdma_prd *bmdma_prd;
    dma_addr_t bmdma_prd_dma;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    unsigned int cbl;
    struct ata_queued_cmd qcmd[33];
    long unsigned int sas_tag_allocated;
    u64 qc_active;
    int nr_active_links;
    unsigned int sas_last_tag;
    struct ata_link link;
    struct ata_link *slave_link;
    int nr_pmp_links;
    struct ata_link *pmp_link;
    struct ata_link *excl_link;
    struct ata_port_stats stats;
    struct ata_host *host;
    struct device *dev;
    struct device tdev;
    struct mutex scsi_scan_mutex;
    struct delayed_work hotplug_task;
    struct work_struct scsi_rescan_task;
    unsigned int hsm_task_state;
    u32 msg_enable;
    struct list_head eh_done_q;
    wait_queue_head_t eh_wait_q;
    int eh_tries;
    struct completion park_req_pending;
    pm_message_t pm_mesg;
    enum ata_lpm_policy target_lpm_policy;
    struct timer_list fastdrain_timer;
    long unsigned int fastdrain_cnt;
    int em_message_type;
    void *private_data;
    struct ata_acpi_gtm __acpi_init_gtm;
    u8 sector_buf[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ata_port {
    struct Scsi_Host *scsi_host;
    struct ata_port_operations *ops;
    spinlock_t *lock;
    long unsigned int flags;
    unsigned int pflags;
    unsigned int print_id;
    unsigned int local_port_no;
    unsigned int port_no;
    struct ata_ioports ioaddr;
    u8 ctl;
    u8 last_ctl;
    struct ata_link *sff_pio_task_link;
    struct delayed_work sff_pio_task;
    struct ata_bmdma_prd *bmdma_prd;
    dma_addr_t bmdma_prd_dma;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    unsigned int cbl;
    struct ata_queued_cmd qcmd[33];
    long unsigned int sas_tag_allocated;
    u64 qc_active;
    int nr_active_links;
    unsigned int sas_last_tag;
    struct ata_link link;
    struct ata_link *slave_link;
    int nr_pmp_links;
    struct ata_link *pmp_link;
    struct ata_link *excl_link;
    struct ata_port_stats stats;
    struct ata_host *host;
    struct device *dev;
    struct device tdev;
    struct mutex scsi_scan_mutex;
    struct delayed_work hotplug_task;
    struct work_struct scsi_rescan_task;
    unsigned int hsm_task_state;
    u32 msg_enable;
    struct list_head eh_done_q;
    wait_queue_head_t eh_wait_q;
    int eh_tries;
    struct completion park_req_pending;
    pm_message_t pm_mesg;
    enum ata_lpm_policy target_lpm_policy;
    struct timer_list fastdrain_timer;
    long unsigned int fastdrain_cnt;
    int em_message_type;
    void *private_data;
    struct ata_acpi_gtm __acpi_init_gtm;
    u8 sector_buf[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ata_port {
    struct Scsi_Host *scsi_host;
    struct ata_port_operations *ops;
    spinlock_t *lock;
    long unsigned int flags;
    unsigned int pflags;
    unsigned int print_id;
    unsigned int local_port_no;
    unsigned int port_no;
    struct ata_ioports ioaddr;
    u8 ctl;
    u8 last_ctl;
    struct ata_link *sff_pio_task_link;
    struct delayed_work sff_pio_task;
    struct ata_bmdma_prd *bmdma_prd;
    dma_addr_t bmdma_prd_dma;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    unsigned int cbl;
    struct ata_queued_cmd qcmd[33];
    long unsigned int sas_tag_allocated;
    u64 qc_active;
    int nr_active_links;
    unsigned int sas_last_tag;
    struct ata_link link;
    struct ata_link *slave_link;
    int nr_pmp_links;
    struct ata_link *pmp_link;
    struct ata_link *excl_link;
    struct ata_port_stats stats;
    struct ata_host *host;
    struct device *dev;
    struct device tdev;
    struct mutex scsi_scan_mutex;
    struct delayed_work hotplug_task;
    struct work_struct scsi_rescan_task;
    unsigned int hsm_task_state;
    u32 msg_enable;
    struct list_head eh_done_q;
    wait_queue_head_t eh_wait_q;
    int eh_tries;
    struct completion park_req_pending;
    pm_message_t pm_mesg;
    enum ata_lpm_policy target_lpm_policy;
    struct timer_list fastdrain_timer;
    long unsigned int fastdrain_cnt;
    int em_message_type;
    void *private_data;
    struct ata_acpi_gtm __acpi_init_gtm;
    u8 sector_buf[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ata_port {
    struct Scsi_Host *scsi_host;
    struct ata_port_operations *ops;
    spinlock_t *lock;
    long unsigned int flags;
    unsigned int pflags;
    unsigned int print_id;
    unsigned int local_port_no;
    unsigned int port_no;
    struct ata_ioports ioaddr;
    u8 ctl;
    u8 last_ctl;
    struct ata_link *sff_pio_task_link;
    struct delayed_work sff_pio_task;
    struct ata_bmdma_prd *bmdma_prd;
    dma_addr_t bmdma_prd_dma;
    unsigned int pio_mask;
    unsigned int mwdma_mask;
    unsigned int udma_mask;
    unsigned int cbl;
    struct ata_queued_cmd qcmd[33];
    long unsigned int sas_tag_allocated;
    u64 qc_active;
    int nr_active_links;
    unsigned int sas_last_tag;
    struct ata_link link;
    struct ata_link *slave_link;
    int nr_pmp_links;
    struct ata_link *pmp_link;
    struct ata_link *excl_link;
    struct ata_port_stats stats;
    struct ata_host *host;
    struct device *dev;
    struct device tdev;
    struct mutex scsi_scan_mutex;
    struct delayed_work hotplug_task;
    struct work_struct scsi_rescan_task;
    unsigned int hsm_task_state;
    u32 msg_enable;
    struct list_head eh_done_q;
    wait_queue_head_t eh_wait_q;
    int eh_tries;
    struct completion park_req_pending;
    pm_message_t pm_mesg;
    enum ata_lpm_policy target_lpm_policy;
    struct timer_list fastdrain_timer;
    long unsigned int fastdrain_cnt;
    int em_message_type;
    void *private_data;
    struct ata_acpi_gtm __acpi_init_gtm;
    u8 sector_buf[512];
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.4</code> and <code>4.8</code> ✅
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
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct ata_queued_cmd qcmd[32]</code> ➡️ <code>struct ata_queued_cmd qcmd[33]</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int qc_active</code> ➡️ <code>u64 qc_active</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>async_cookie_t cookie</code>
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
<b>Field removed. </b>
<code>long unsigned int sas_tag_allocated</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int sas_last_tag</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 msg_enable</code>
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
<code>long unsigned int fastdrain_cnt</code> ➡️ <code>unsigned int fastdrain_cnt</code>
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
<code>u8 *ncq_sense_buf</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct work_struct scsi_rescan_task</code> ➡️ <code>struct delayed_work scsi_rescan_task</code>
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
<code>struct ata_acpi_gtm __acpi_init_gtm</code>
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
<code>struct ata_acpi_gtm __acpi_init_gtm</code>
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
<code>struct ata_acpi_gtm __acpi_init_gtm</code>
</li>
</ul>
</details>
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
