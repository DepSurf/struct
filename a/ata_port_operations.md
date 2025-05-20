# Struct: <code>ata_port_operations</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct ata_port_operations {
    int (*qc_defer)(struct ata_queued_cmd *);
    int (*check_atapi_dma)(struct ata_queued_cmd *);
    void (*qc_prep)(struct ata_queued_cmd *);
    unsigned int (*qc_issue)(struct ata_queued_cmd *);
    bool (*qc_fill_rtf)(struct ata_queued_cmd *);
    int (*cable_detect)(struct ata_port *);
    long unsigned int (*mode_filter)(struct ata_device *, long unsigned int);
    void (*set_piomode)(struct ata_port *, struct ata_device *);
    void (*set_dmamode)(struct ata_port *, struct ata_device *);
    int (*set_mode)(struct ata_link *, struct ata_device **);
    unsigned int (*read_id)(struct ata_device *, struct ata_taskfile *, u16 *);
    void (*dev_config)(struct ata_device *);
    void (*freeze)(struct ata_port *);
    void (*thaw)(struct ata_port *);
    ata_prereset_fn_t prereset;
    ata_reset_fn_t softreset;
    ata_reset_fn_t hardreset;
    ata_postreset_fn_t postreset;
    ata_prereset_fn_t pmp_prereset;
    ata_reset_fn_t pmp_softreset;
    ata_reset_fn_t pmp_hardreset;
    ata_postreset_fn_t pmp_postreset;
    void (*error_handler)(struct ata_port *);
    void (*lost_interrupt)(struct ata_port *);
    void (*post_internal_cmd)(struct ata_queued_cmd *);
    void (*sched_eh)(struct ata_port *);
    void (*end_eh)(struct ata_port *);
    int (*scr_read)(struct ata_link *, unsigned int, u32 *);
    int (*scr_write)(struct ata_link *, unsigned int, u32);
    void (*pmp_attach)(struct ata_port *);
    void (*pmp_detach)(struct ata_port *);
    int (*set_lpm)(struct ata_link *, enum ata_lpm_policy, unsigned int);
    int (*port_suspend)(struct ata_port *, pm_message_t);
    int (*port_resume)(struct ata_port *);
    int (*port_start)(struct ata_port *);
    void (*port_stop)(struct ata_port *);
    void (*host_stop)(struct ata_host *);
    void (*sff_dev_select)(struct ata_port *, unsigned int);
    void (*sff_set_devctl)(struct ata_port *, u8);
    u8 (*sff_check_status)(struct ata_port *);
    u8 (*sff_check_altstatus)(struct ata_port *);
    void (*sff_tf_load)(struct ata_port *, const struct ata_taskfile *);
    void (*sff_tf_read)(struct ata_port *, struct ata_taskfile *);
    void (*sff_exec_command)(struct ata_port *, const struct ata_taskfile *);
    unsigned int (*sff_data_xfer)(struct ata_device *, unsigned char *, unsigned int, int);
    void (*sff_irq_on)(struct ata_port *);
    bool (*sff_irq_check)(struct ata_port *);
    void (*sff_irq_clear)(struct ata_port *);
    void (*sff_drain_fifo)(struct ata_queued_cmd *);
    void (*bmdma_setup)(struct ata_queued_cmd *);
    void (*bmdma_start)(struct ata_queued_cmd *);
    void (*bmdma_stop)(struct ata_queued_cmd *);
    u8 (*bmdma_status)(struct ata_port *);
    ssize_t (*em_show)(struct ata_port *, char *);
    ssize_t (*em_store)(struct ata_port *, const char *, size_t);
    ssize_t (*sw_activity_show)(struct ata_device *, char *);
    ssize_t (*sw_activity_store)(struct ata_device *, enum sw_activity);
    ssize_t (*transmit_led_message)(struct ata_port *, u32, ssize_t);
    void (*phy_reset)(struct ata_port *);
    void (*eng_timeout)(struct ata_port *);
    const struct ata_port_operations *inherits;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ata_port_operations {
    int (*qc_defer)(struct ata_queued_cmd *);
    int (*check_atapi_dma)(struct ata_queued_cmd *);
    void (*qc_prep)(struct ata_queued_cmd *);
    unsigned int (*qc_issue)(struct ata_queued_cmd *);
    bool (*qc_fill_rtf)(struct ata_queued_cmd *);
    int (*cable_detect)(struct ata_port *);
    long unsigned int (*mode_filter)(struct ata_device *, long unsigned int);
    void (*set_piomode)(struct ata_port *, struct ata_device *);
    void (*set_dmamode)(struct ata_port *, struct ata_device *);
    int (*set_mode)(struct ata_link *, struct ata_device **);
    unsigned int (*read_id)(struct ata_device *, struct ata_taskfile *, u16 *);
    void (*dev_config)(struct ata_device *);
    void (*freeze)(struct ata_port *);
    void (*thaw)(struct ata_port *);
    ata_prereset_fn_t prereset;
    ata_reset_fn_t softreset;
    ata_reset_fn_t hardreset;
    ata_postreset_fn_t postreset;
    ata_prereset_fn_t pmp_prereset;
    ata_reset_fn_t pmp_softreset;
    ata_reset_fn_t pmp_hardreset;
    ata_postreset_fn_t pmp_postreset;
    void (*error_handler)(struct ata_port *);
    void (*lost_interrupt)(struct ata_port *);
    void (*post_internal_cmd)(struct ata_queued_cmd *);
    void (*sched_eh)(struct ata_port *);
    void (*end_eh)(struct ata_port *);
    int (*scr_read)(struct ata_link *, unsigned int, u32 *);
    int (*scr_write)(struct ata_link *, unsigned int, u32);
    void (*pmp_attach)(struct ata_port *);
    void (*pmp_detach)(struct ata_port *);
    int (*set_lpm)(struct ata_link *, enum ata_lpm_policy, unsigned int);
    int (*port_suspend)(struct ata_port *, pm_message_t);
    int (*port_resume)(struct ata_port *);
    int (*port_start)(struct ata_port *);
    void (*port_stop)(struct ata_port *);
    void (*host_stop)(struct ata_host *);
    void (*sff_dev_select)(struct ata_port *, unsigned int);
    void (*sff_set_devctl)(struct ata_port *, u8);
    u8 (*sff_check_status)(struct ata_port *);
    u8 (*sff_check_altstatus)(struct ata_port *);
    void (*sff_tf_load)(struct ata_port *, const struct ata_taskfile *);
    void (*sff_tf_read)(struct ata_port *, struct ata_taskfile *);
    void (*sff_exec_command)(struct ata_port *, const struct ata_taskfile *);
    unsigned int (*sff_data_xfer)(struct ata_device *, unsigned char *, unsigned int, int);
    void (*sff_irq_on)(struct ata_port *);
    bool (*sff_irq_check)(struct ata_port *);
    void (*sff_irq_clear)(struct ata_port *);
    void (*sff_drain_fifo)(struct ata_queued_cmd *);
    void (*bmdma_setup)(struct ata_queued_cmd *);
    void (*bmdma_start)(struct ata_queued_cmd *);
    void (*bmdma_stop)(struct ata_queued_cmd *);
    u8 (*bmdma_status)(struct ata_port *);
    ssize_t (*em_show)(struct ata_port *, char *);
    ssize_t (*em_store)(struct ata_port *, const char *, size_t);
    ssize_t (*sw_activity_show)(struct ata_device *, char *);
    ssize_t (*sw_activity_store)(struct ata_device *, enum sw_activity);
    ssize_t (*transmit_led_message)(struct ata_port *, u32, ssize_t);
    void (*phy_reset)(struct ata_port *);
    void (*eng_timeout)(struct ata_port *);
    const struct ata_port_operations *inherits;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ata_port_operations {
    int (*qc_defer)(struct ata_queued_cmd *);
    int (*check_atapi_dma)(struct ata_queued_cmd *);
    void (*qc_prep)(struct ata_queued_cmd *);
    unsigned int (*qc_issue)(struct ata_queued_cmd *);
    bool (*qc_fill_rtf)(struct ata_queued_cmd *);
    int (*cable_detect)(struct ata_port *);
    long unsigned int (*mode_filter)(struct ata_device *, long unsigned int);
    void (*set_piomode)(struct ata_port *, struct ata_device *);
    void (*set_dmamode)(struct ata_port *, struct ata_device *);
    int (*set_mode)(struct ata_link *, struct ata_device **);
    unsigned int (*read_id)(struct ata_device *, struct ata_taskfile *, u16 *);
    void (*dev_config)(struct ata_device *);
    void (*freeze)(struct ata_port *);
    void (*thaw)(struct ata_port *);
    ata_prereset_fn_t prereset;
    ata_reset_fn_t softreset;
    ata_reset_fn_t hardreset;
    ata_postreset_fn_t postreset;
    ata_prereset_fn_t pmp_prereset;
    ata_reset_fn_t pmp_softreset;
    ata_reset_fn_t pmp_hardreset;
    ata_postreset_fn_t pmp_postreset;
    void (*error_handler)(struct ata_port *);
    void (*lost_interrupt)(struct ata_port *);
    void (*post_internal_cmd)(struct ata_queued_cmd *);
    void (*sched_eh)(struct ata_port *);
    void (*end_eh)(struct ata_port *);
    int (*scr_read)(struct ata_link *, unsigned int, u32 *);
    int (*scr_write)(struct ata_link *, unsigned int, u32);
    void (*pmp_attach)(struct ata_port *);
    void (*pmp_detach)(struct ata_port *);
    int (*set_lpm)(struct ata_link *, enum ata_lpm_policy, unsigned int);
    int (*port_suspend)(struct ata_port *, pm_message_t);
    int (*port_resume)(struct ata_port *);
    int (*port_start)(struct ata_port *);
    void (*port_stop)(struct ata_port *);
    void (*host_stop)(struct ata_host *);
    void (*sff_dev_select)(struct ata_port *, unsigned int);
    void (*sff_set_devctl)(struct ata_port *, u8);
    u8 (*sff_check_status)(struct ata_port *);
    u8 (*sff_check_altstatus)(struct ata_port *);
    void (*sff_tf_load)(struct ata_port *, const struct ata_taskfile *);
    void (*sff_tf_read)(struct ata_port *, struct ata_taskfile *);
    void (*sff_exec_command)(struct ata_port *, const struct ata_taskfile *);
    unsigned int (*sff_data_xfer)(struct ata_device *, unsigned char *, unsigned int, int);
    void (*sff_irq_on)(struct ata_port *);
    bool (*sff_irq_check)(struct ata_port *);
    void (*sff_irq_clear)(struct ata_port *);
    void (*sff_drain_fifo)(struct ata_queued_cmd *);
    void (*bmdma_setup)(struct ata_queued_cmd *);
    void (*bmdma_start)(struct ata_queued_cmd *);
    void (*bmdma_stop)(struct ata_queued_cmd *);
    u8 (*bmdma_status)(struct ata_port *);
    ssize_t (*em_show)(struct ata_port *, char *);
    ssize_t (*em_store)(struct ata_port *, const char *, size_t);
    ssize_t (*sw_activity_show)(struct ata_device *, char *);
    ssize_t (*sw_activity_store)(struct ata_device *, enum sw_activity);
    ssize_t (*transmit_led_message)(struct ata_port *, u32, ssize_t);
    void (*phy_reset)(struct ata_port *);
    void (*eng_timeout)(struct ata_port *);
    const struct ata_port_operations *inherits;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ata_port_operations {
    int (*qc_defer)(struct ata_queued_cmd *);
    int (*check_atapi_dma)(struct ata_queued_cmd *);
    void (*qc_prep)(struct ata_queued_cmd *);
    unsigned int (*qc_issue)(struct ata_queued_cmd *);
    bool (*qc_fill_rtf)(struct ata_queued_cmd *);
    int (*cable_detect)(struct ata_port *);
    long unsigned int (*mode_filter)(struct ata_device *, long unsigned int);
    void (*set_piomode)(struct ata_port *, struct ata_device *);
    void (*set_dmamode)(struct ata_port *, struct ata_device *);
    int (*set_mode)(struct ata_link *, struct ata_device **);
    unsigned int (*read_id)(struct ata_device *, struct ata_taskfile *, u16 *);
    void (*dev_config)(struct ata_device *);
    void (*freeze)(struct ata_port *);
    void (*thaw)(struct ata_port *);
    ata_prereset_fn_t prereset;
    ata_reset_fn_t softreset;
    ata_reset_fn_t hardreset;
    ata_postreset_fn_t postreset;
    ata_prereset_fn_t pmp_prereset;
    ata_reset_fn_t pmp_softreset;
    ata_reset_fn_t pmp_hardreset;
    ata_postreset_fn_t pmp_postreset;
    void (*error_handler)(struct ata_port *);
    void (*lost_interrupt)(struct ata_port *);
    void (*post_internal_cmd)(struct ata_queued_cmd *);
    void (*sched_eh)(struct ata_port *);
    void (*end_eh)(struct ata_port *);
    int (*scr_read)(struct ata_link *, unsigned int, u32 *);
    int (*scr_write)(struct ata_link *, unsigned int, u32);
    void (*pmp_attach)(struct ata_port *);
    void (*pmp_detach)(struct ata_port *);
    int (*set_lpm)(struct ata_link *, enum ata_lpm_policy, unsigned int);
    int (*port_suspend)(struct ata_port *, pm_message_t);
    int (*port_resume)(struct ata_port *);
    int (*port_start)(struct ata_port *);
    void (*port_stop)(struct ata_port *);
    void (*host_stop)(struct ata_host *);
    void (*sff_dev_select)(struct ata_port *, unsigned int);
    void (*sff_set_devctl)(struct ata_port *, u8);
    u8 (*sff_check_status)(struct ata_port *);
    u8 (*sff_check_altstatus)(struct ata_port *);
    void (*sff_tf_load)(struct ata_port *, const struct ata_taskfile *);
    void (*sff_tf_read)(struct ata_port *, struct ata_taskfile *);
    void (*sff_exec_command)(struct ata_port *, const struct ata_taskfile *);
    unsigned int (*sff_data_xfer)(struct ata_queued_cmd *, unsigned char *, unsigned int, int);
    void (*sff_irq_on)(struct ata_port *);
    bool (*sff_irq_check)(struct ata_port *);
    void (*sff_irq_clear)(struct ata_port *);
    void (*sff_drain_fifo)(struct ata_queued_cmd *);
    void (*bmdma_setup)(struct ata_queued_cmd *);
    void (*bmdma_start)(struct ata_queued_cmd *);
    void (*bmdma_stop)(struct ata_queued_cmd *);
    u8 (*bmdma_status)(struct ata_port *);
    ssize_t (*em_show)(struct ata_port *, char *);
    ssize_t (*em_store)(struct ata_port *, const char *, size_t);
    ssize_t (*sw_activity_show)(struct ata_device *, char *);
    ssize_t (*sw_activity_store)(struct ata_device *, enum sw_activity);
    ssize_t (*transmit_led_message)(struct ata_port *, u32, ssize_t);
    void (*phy_reset)(struct ata_port *);
    void (*eng_timeout)(struct ata_port *);
    const struct ata_port_operations *inherits;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ata_port_operations {
    int (*qc_defer)(struct ata_queued_cmd *);
    int (*check_atapi_dma)(struct ata_queued_cmd *);
    void (*qc_prep)(struct ata_queued_cmd *);
    unsigned int (*qc_issue)(struct ata_queued_cmd *);
    bool (*qc_fill_rtf)(struct ata_queued_cmd *);
    int (*cable_detect)(struct ata_port *);
    long unsigned int (*mode_filter)(struct ata_device *, long unsigned int);
    void (*set_piomode)(struct ata_port *, struct ata_device *);
    void (*set_dmamode)(struct ata_port *, struct ata_device *);
    int (*set_mode)(struct ata_link *, struct ata_device **);
    unsigned int (*read_id)(struct ata_device *, struct ata_taskfile *, u16 *);
    void (*dev_config)(struct ata_device *);
    void (*freeze)(struct ata_port *);
    void (*thaw)(struct ata_port *);
    ata_prereset_fn_t prereset;
    ata_reset_fn_t softreset;
    ata_reset_fn_t hardreset;
    ata_postreset_fn_t postreset;
    ata_prereset_fn_t pmp_prereset;
    ata_reset_fn_t pmp_softreset;
    ata_reset_fn_t pmp_hardreset;
    ata_postreset_fn_t pmp_postreset;
    void (*error_handler)(struct ata_port *);
    void (*lost_interrupt)(struct ata_port *);
    void (*post_internal_cmd)(struct ata_queued_cmd *);
    void (*sched_eh)(struct ata_port *);
    void (*end_eh)(struct ata_port *);
    int (*scr_read)(struct ata_link *, unsigned int, u32 *);
    int (*scr_write)(struct ata_link *, unsigned int, u32);
    void (*pmp_attach)(struct ata_port *);
    void (*pmp_detach)(struct ata_port *);
    int (*set_lpm)(struct ata_link *, enum ata_lpm_policy, unsigned int);
    int (*port_suspend)(struct ata_port *, pm_message_t);
    int (*port_resume)(struct ata_port *);
    int (*port_start)(struct ata_port *);
    void (*port_stop)(struct ata_port *);
    void (*host_stop)(struct ata_host *);
    void (*sff_dev_select)(struct ata_port *, unsigned int);
    void (*sff_set_devctl)(struct ata_port *, u8);
    u8 (*sff_check_status)(struct ata_port *);
    u8 (*sff_check_altstatus)(struct ata_port *);
    void (*sff_tf_load)(struct ata_port *, const struct ata_taskfile *);
    void (*sff_tf_read)(struct ata_port *, struct ata_taskfile *);
    void (*sff_exec_command)(struct ata_port *, const struct ata_taskfile *);
    unsigned int (*sff_data_xfer)(struct ata_queued_cmd *, unsigned char *, unsigned int, int);
    void (*sff_irq_on)(struct ata_port *);
    bool (*sff_irq_check)(struct ata_port *);
    void (*sff_irq_clear)(struct ata_port *);
    void (*sff_drain_fifo)(struct ata_queued_cmd *);
    void (*bmdma_setup)(struct ata_queued_cmd *);
    void (*bmdma_start)(struct ata_queued_cmd *);
    void (*bmdma_stop)(struct ata_queued_cmd *);
    u8 (*bmdma_status)(struct ata_port *);
    ssize_t (*em_show)(struct ata_port *, char *);
    ssize_t (*em_store)(struct ata_port *, const char *, size_t);
    ssize_t (*sw_activity_show)(struct ata_device *, char *);
    ssize_t (*sw_activity_store)(struct ata_device *, enum sw_activity);
    ssize_t (*transmit_led_message)(struct ata_port *, u32, ssize_t);
    void (*phy_reset)(struct ata_port *);
    void (*eng_timeout)(struct ata_port *);
    const struct ata_port_operations *inherits;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ata_port_operations {
    int (*qc_defer)(struct ata_queued_cmd *);
    int (*check_atapi_dma)(struct ata_queued_cmd *);
    void (*qc_prep)(struct ata_queued_cmd *);
    unsigned int (*qc_issue)(struct ata_queued_cmd *);
    bool (*qc_fill_rtf)(struct ata_queued_cmd *);
    int (*cable_detect)(struct ata_port *);
    long unsigned int (*mode_filter)(struct ata_device *, long unsigned int);
    void (*set_piomode)(struct ata_port *, struct ata_device *);
    void (*set_dmamode)(struct ata_port *, struct ata_device *);
    int (*set_mode)(struct ata_link *, struct ata_device **);
    unsigned int (*read_id)(struct ata_device *, struct ata_taskfile *, u16 *);
    void (*dev_config)(struct ata_device *);
    void (*freeze)(struct ata_port *);
    void (*thaw)(struct ata_port *);
    ata_prereset_fn_t prereset;
    ata_reset_fn_t softreset;
    ata_reset_fn_t hardreset;
    ata_postreset_fn_t postreset;
    ata_prereset_fn_t pmp_prereset;
    ata_reset_fn_t pmp_softreset;
    ata_reset_fn_t pmp_hardreset;
    ata_postreset_fn_t pmp_postreset;
    void (*error_handler)(struct ata_port *);
    void (*lost_interrupt)(struct ata_port *);
    void (*post_internal_cmd)(struct ata_queued_cmd *);
    void (*sched_eh)(struct ata_port *);
    void (*end_eh)(struct ata_port *);
    int (*scr_read)(struct ata_link *, unsigned int, u32 *);
    int (*scr_write)(struct ata_link *, unsigned int, u32);
    void (*pmp_attach)(struct ata_port *);
    void (*pmp_detach)(struct ata_port *);
    int (*set_lpm)(struct ata_link *, enum ata_lpm_policy, unsigned int);
    int (*port_suspend)(struct ata_port *, pm_message_t);
    int (*port_resume)(struct ata_port *);
    int (*port_start)(struct ata_port *);
    void (*port_stop)(struct ata_port *);
    void (*host_stop)(struct ata_host *);
    void (*sff_dev_select)(struct ata_port *, unsigned int);
    void (*sff_set_devctl)(struct ata_port *, u8);
    u8 (*sff_check_status)(struct ata_port *);
    u8 (*sff_check_altstatus)(struct ata_port *);
    void (*sff_tf_load)(struct ata_port *, const struct ata_taskfile *);
    void (*sff_tf_read)(struct ata_port *, struct ata_taskfile *);
    void (*sff_exec_command)(struct ata_port *, const struct ata_taskfile *);
    unsigned int (*sff_data_xfer)(struct ata_queued_cmd *, unsigned char *, unsigned int, int);
    void (*sff_irq_on)(struct ata_port *);
    bool (*sff_irq_check)(struct ata_port *);
    void (*sff_irq_clear)(struct ata_port *);
    void (*sff_drain_fifo)(struct ata_queued_cmd *);
    void (*bmdma_setup)(struct ata_queued_cmd *);
    void (*bmdma_start)(struct ata_queued_cmd *);
    void (*bmdma_stop)(struct ata_queued_cmd *);
    u8 (*bmdma_status)(struct ata_port *);
    ssize_t (*em_show)(struct ata_port *, char *);
    ssize_t (*em_store)(struct ata_port *, const char *, size_t);
    ssize_t (*sw_activity_show)(struct ata_device *, char *);
    ssize_t (*sw_activity_store)(struct ata_device *, enum sw_activity);
    ssize_t (*transmit_led_message)(struct ata_port *, u32, ssize_t);
    void (*phy_reset)(struct ata_port *);
    void (*eng_timeout)(struct ata_port *);
    const struct ata_port_operations *inherits;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ata_port_operations {
    int (*qc_defer)(struct ata_queued_cmd *);
    int (*check_atapi_dma)(struct ata_queued_cmd *);
    void (*qc_prep)(struct ata_queued_cmd *);
    unsigned int (*qc_issue)(struct ata_queued_cmd *);
    bool (*qc_fill_rtf)(struct ata_queued_cmd *);
    int (*cable_detect)(struct ata_port *);
    long unsigned int (*mode_filter)(struct ata_device *, long unsigned int);
    void (*set_piomode)(struct ata_port *, struct ata_device *);
    void (*set_dmamode)(struct ata_port *, struct ata_device *);
    int (*set_mode)(struct ata_link *, struct ata_device **);
    unsigned int (*read_id)(struct ata_device *, struct ata_taskfile *, u16 *);
    void (*dev_config)(struct ata_device *);
    void (*freeze)(struct ata_port *);
    void (*thaw)(struct ata_port *);
    ata_prereset_fn_t prereset;
    ata_reset_fn_t softreset;
    ata_reset_fn_t hardreset;
    ata_postreset_fn_t postreset;
    ata_prereset_fn_t pmp_prereset;
    ata_reset_fn_t pmp_softreset;
    ata_reset_fn_t pmp_hardreset;
    ata_postreset_fn_t pmp_postreset;
    void (*error_handler)(struct ata_port *);
    void (*lost_interrupt)(struct ata_port *);
    void (*post_internal_cmd)(struct ata_queued_cmd *);
    void (*sched_eh)(struct ata_port *);
    void (*end_eh)(struct ata_port *);
    int (*scr_read)(struct ata_link *, unsigned int, u32 *);
    int (*scr_write)(struct ata_link *, unsigned int, u32);
    void (*pmp_attach)(struct ata_port *);
    void (*pmp_detach)(struct ata_port *);
    int (*set_lpm)(struct ata_link *, enum ata_lpm_policy, unsigned int);
    int (*port_suspend)(struct ata_port *, pm_message_t);
    int (*port_resume)(struct ata_port *);
    int (*port_start)(struct ata_port *);
    void (*port_stop)(struct ata_port *);
    void (*host_stop)(struct ata_host *);
    void (*sff_dev_select)(struct ata_port *, unsigned int);
    void (*sff_set_devctl)(struct ata_port *, u8);
    u8 (*sff_check_status)(struct ata_port *);
    u8 (*sff_check_altstatus)(struct ata_port *);
    void (*sff_tf_load)(struct ata_port *, const struct ata_taskfile *);
    void (*sff_tf_read)(struct ata_port *, struct ata_taskfile *);
    void (*sff_exec_command)(struct ata_port *, const struct ata_taskfile *);
    unsigned int (*sff_data_xfer)(struct ata_queued_cmd *, unsigned char *, unsigned int, int);
    void (*sff_irq_on)(struct ata_port *);
    bool (*sff_irq_check)(struct ata_port *);
    void (*sff_irq_clear)(struct ata_port *);
    void (*sff_drain_fifo)(struct ata_queued_cmd *);
    void (*bmdma_setup)(struct ata_queued_cmd *);
    void (*bmdma_start)(struct ata_queued_cmd *);
    void (*bmdma_stop)(struct ata_queued_cmd *);
    u8 (*bmdma_status)(struct ata_port *);
    ssize_t (*em_show)(struct ata_port *, char *);
    ssize_t (*em_store)(struct ata_port *, const char *, size_t);
    ssize_t (*sw_activity_show)(struct ata_device *, char *);
    ssize_t (*sw_activity_store)(struct ata_device *, enum sw_activity);
    ssize_t (*transmit_led_message)(struct ata_port *, u32, ssize_t);
    void (*phy_reset)(struct ata_port *);
    void (*eng_timeout)(struct ata_port *);
    const struct ata_port_operations *inherits;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ata_port_operations {
    int (*qc_defer)(struct ata_queued_cmd *);
    int (*check_atapi_dma)(struct ata_queued_cmd *);
    void (*qc_prep)(struct ata_queued_cmd *);
    unsigned int (*qc_issue)(struct ata_queued_cmd *);
    bool (*qc_fill_rtf)(struct ata_queued_cmd *);
    int (*cable_detect)(struct ata_port *);
    long unsigned int (*mode_filter)(struct ata_device *, long unsigned int);
    void (*set_piomode)(struct ata_port *, struct ata_device *);
    void (*set_dmamode)(struct ata_port *, struct ata_device *);
    int (*set_mode)(struct ata_link *, struct ata_device **);
    unsigned int (*read_id)(struct ata_device *, struct ata_taskfile *, u16 *);
    void (*dev_config)(struct ata_device *);
    void (*freeze)(struct ata_port *);
    void (*thaw)(struct ata_port *);
    ata_prereset_fn_t prereset;
    ata_reset_fn_t softreset;
    ata_reset_fn_t hardreset;
    ata_postreset_fn_t postreset;
    ata_prereset_fn_t pmp_prereset;
    ata_reset_fn_t pmp_softreset;
    ata_reset_fn_t pmp_hardreset;
    ata_postreset_fn_t pmp_postreset;
    void (*error_handler)(struct ata_port *);
    void (*lost_interrupt)(struct ata_port *);
    void (*post_internal_cmd)(struct ata_queued_cmd *);
    void (*sched_eh)(struct ata_port *);
    void (*end_eh)(struct ata_port *);
    int (*scr_read)(struct ata_link *, unsigned int, u32 *);
    int (*scr_write)(struct ata_link *, unsigned int, u32);
    void (*pmp_attach)(struct ata_port *);
    void (*pmp_detach)(struct ata_port *);
    int (*set_lpm)(struct ata_link *, enum ata_lpm_policy, unsigned int);
    int (*port_suspend)(struct ata_port *, pm_message_t);
    int (*port_resume)(struct ata_port *);
    int (*port_start)(struct ata_port *);
    void (*port_stop)(struct ata_port *);
    void (*host_stop)(struct ata_host *);
    void (*sff_dev_select)(struct ata_port *, unsigned int);
    void (*sff_set_devctl)(struct ata_port *, u8);
    u8 (*sff_check_status)(struct ata_port *);
    u8 (*sff_check_altstatus)(struct ata_port *);
    void (*sff_tf_load)(struct ata_port *, const struct ata_taskfile *);
    void (*sff_tf_read)(struct ata_port *, struct ata_taskfile *);
    void (*sff_exec_command)(struct ata_port *, const struct ata_taskfile *);
    unsigned int (*sff_data_xfer)(struct ata_queued_cmd *, unsigned char *, unsigned int, int);
    void (*sff_irq_on)(struct ata_port *);
    bool (*sff_irq_check)(struct ata_port *);
    void (*sff_irq_clear)(struct ata_port *);
    void (*sff_drain_fifo)(struct ata_queued_cmd *);
    void (*bmdma_setup)(struct ata_queued_cmd *);
    void (*bmdma_start)(struct ata_queued_cmd *);
    void (*bmdma_stop)(struct ata_queued_cmd *);
    u8 (*bmdma_status)(struct ata_port *);
    ssize_t (*em_show)(struct ata_port *, char *);
    ssize_t (*em_store)(struct ata_port *, const char *, size_t);
    ssize_t (*sw_activity_show)(struct ata_device *, char *);
    ssize_t (*sw_activity_store)(struct ata_device *, enum sw_activity);
    ssize_t (*transmit_led_message)(struct ata_port *, u32, ssize_t);
    void (*phy_reset)(struct ata_port *);
    void (*eng_timeout)(struct ata_port *);
    const struct ata_port_operations *inherits;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ata_port_operations {
    int (*qc_defer)(struct ata_queued_cmd *);
    int (*check_atapi_dma)(struct ata_queued_cmd *);
    void (*qc_prep)(struct ata_queued_cmd *);
    unsigned int (*qc_issue)(struct ata_queued_cmd *);
    bool (*qc_fill_rtf)(struct ata_queued_cmd *);
    int (*cable_detect)(struct ata_port *);
    long unsigned int (*mode_filter)(struct ata_device *, long unsigned int);
    void (*set_piomode)(struct ata_port *, struct ata_device *);
    void (*set_dmamode)(struct ata_port *, struct ata_device *);
    int (*set_mode)(struct ata_link *, struct ata_device **);
    unsigned int (*read_id)(struct ata_device *, struct ata_taskfile *, u16 *);
    void (*dev_config)(struct ata_device *);
    void (*freeze)(struct ata_port *);
    void (*thaw)(struct ata_port *);
    ata_prereset_fn_t prereset;
    ata_reset_fn_t softreset;
    ata_reset_fn_t hardreset;
    ata_postreset_fn_t postreset;
    ata_prereset_fn_t pmp_prereset;
    ata_reset_fn_t pmp_softreset;
    ata_reset_fn_t pmp_hardreset;
    ata_postreset_fn_t pmp_postreset;
    void (*error_handler)(struct ata_port *);
    void (*lost_interrupt)(struct ata_port *);
    void (*post_internal_cmd)(struct ata_queued_cmd *);
    void (*sched_eh)(struct ata_port *);
    void (*end_eh)(struct ata_port *);
    int (*scr_read)(struct ata_link *, unsigned int, u32 *);
    int (*scr_write)(struct ata_link *, unsigned int, u32);
    void (*pmp_attach)(struct ata_port *);
    void (*pmp_detach)(struct ata_port *);
    int (*set_lpm)(struct ata_link *, enum ata_lpm_policy, unsigned int);
    int (*port_suspend)(struct ata_port *, pm_message_t);
    int (*port_resume)(struct ata_port *);
    int (*port_start)(struct ata_port *);
    void (*port_stop)(struct ata_port *);
    void (*host_stop)(struct ata_host *);
    void (*sff_dev_select)(struct ata_port *, unsigned int);
    void (*sff_set_devctl)(struct ata_port *, u8);
    u8 (*sff_check_status)(struct ata_port *);
    u8 (*sff_check_altstatus)(struct ata_port *);
    void (*sff_tf_load)(struct ata_port *, const struct ata_taskfile *);
    void (*sff_tf_read)(struct ata_port *, struct ata_taskfile *);
    void (*sff_exec_command)(struct ata_port *, const struct ata_taskfile *);
    unsigned int (*sff_data_xfer)(struct ata_queued_cmd *, unsigned char *, unsigned int, int);
    void (*sff_irq_on)(struct ata_port *);
    bool (*sff_irq_check)(struct ata_port *);
    void (*sff_irq_clear)(struct ata_port *);
    void (*sff_drain_fifo)(struct ata_queued_cmd *);
    void (*bmdma_setup)(struct ata_queued_cmd *);
    void (*bmdma_start)(struct ata_queued_cmd *);
    void (*bmdma_stop)(struct ata_queued_cmd *);
    u8 (*bmdma_status)(struct ata_port *);
    ssize_t (*em_show)(struct ata_port *, char *);
    ssize_t (*em_store)(struct ata_port *, const char *, size_t);
    ssize_t (*sw_activity_show)(struct ata_device *, char *);
    ssize_t (*sw_activity_store)(struct ata_device *, enum sw_activity);
    ssize_t (*transmit_led_message)(struct ata_port *, u32, ssize_t);
    void (*phy_reset)(struct ata_port *);
    void (*eng_timeout)(struct ata_port *);
    const struct ata_port_operations *inherits;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ata_port_operations {
    int (*qc_defer)(struct ata_queued_cmd *);
    int (*check_atapi_dma)(struct ata_queued_cmd *);
    enum ata_completion_errors (*qc_prep)(struct ata_queued_cmd *);
    unsigned int (*qc_issue)(struct ata_queued_cmd *);
    bool (*qc_fill_rtf)(struct ata_queued_cmd *);
    int (*cable_detect)(struct ata_port *);
    long unsigned int (*mode_filter)(struct ata_device *, long unsigned int);
    void (*set_piomode)(struct ata_port *, struct ata_device *);
    void (*set_dmamode)(struct ata_port *, struct ata_device *);
    int (*set_mode)(struct ata_link *, struct ata_device **);
    unsigned int (*read_id)(struct ata_device *, struct ata_taskfile *, u16 *);
    void (*dev_config)(struct ata_device *);
    void (*freeze)(struct ata_port *);
    void (*thaw)(struct ata_port *);
    ata_prereset_fn_t prereset;
    ata_reset_fn_t softreset;
    ata_reset_fn_t hardreset;
    ata_postreset_fn_t postreset;
    ata_prereset_fn_t pmp_prereset;
    ata_reset_fn_t pmp_softreset;
    ata_reset_fn_t pmp_hardreset;
    ata_postreset_fn_t pmp_postreset;
    void (*error_handler)(struct ata_port *);
    void (*lost_interrupt)(struct ata_port *);
    void (*post_internal_cmd)(struct ata_queued_cmd *);
    void (*sched_eh)(struct ata_port *);
    void (*end_eh)(struct ata_port *);
    int (*scr_read)(struct ata_link *, unsigned int, u32 *);
    int (*scr_write)(struct ata_link *, unsigned int, u32);
    void (*pmp_attach)(struct ata_port *);
    void (*pmp_detach)(struct ata_port *);
    int (*set_lpm)(struct ata_link *, enum ata_lpm_policy, unsigned int);
    int (*port_suspend)(struct ata_port *, pm_message_t);
    int (*port_resume)(struct ata_port *);
    int (*port_start)(struct ata_port *);
    void (*port_stop)(struct ata_port *);
    void (*host_stop)(struct ata_host *);
    void (*sff_dev_select)(struct ata_port *, unsigned int);
    void (*sff_set_devctl)(struct ata_port *, u8);
    u8 (*sff_check_status)(struct ata_port *);
    u8 (*sff_check_altstatus)(struct ata_port *);
    void (*sff_tf_load)(struct ata_port *, const struct ata_taskfile *);
    void (*sff_tf_read)(struct ata_port *, struct ata_taskfile *);
    void (*sff_exec_command)(struct ata_port *, const struct ata_taskfile *);
    unsigned int (*sff_data_xfer)(struct ata_queued_cmd *, unsigned char *, unsigned int, int);
    void (*sff_irq_on)(struct ata_port *);
    bool (*sff_irq_check)(struct ata_port *);
    void (*sff_irq_clear)(struct ata_port *);
    void (*sff_drain_fifo)(struct ata_queued_cmd *);
    void (*bmdma_setup)(struct ata_queued_cmd *);
    void (*bmdma_start)(struct ata_queued_cmd *);
    void (*bmdma_stop)(struct ata_queued_cmd *);
    u8 (*bmdma_status)(struct ata_port *);
    ssize_t (*em_show)(struct ata_port *, char *);
    ssize_t (*em_store)(struct ata_port *, const char *, size_t);
    ssize_t (*sw_activity_show)(struct ata_device *, char *);
    ssize_t (*sw_activity_store)(struct ata_device *, enum sw_activity);
    ssize_t (*transmit_led_message)(struct ata_port *, u32, ssize_t);
    void (*phy_reset)(struct ata_port *);
    void (*eng_timeout)(struct ata_port *);
    const struct ata_port_operations *inherits;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ata_port_operations {
    int (*qc_defer)(struct ata_queued_cmd *);
    int (*check_atapi_dma)(struct ata_queued_cmd *);
    enum ata_completion_errors (*qc_prep)(struct ata_queued_cmd *);
    unsigned int (*qc_issue)(struct ata_queued_cmd *);
    bool (*qc_fill_rtf)(struct ata_queued_cmd *);
    int (*cable_detect)(struct ata_port *);
    long unsigned int (*mode_filter)(struct ata_device *, long unsigned int);
    void (*set_piomode)(struct ata_port *, struct ata_device *);
    void (*set_dmamode)(struct ata_port *, struct ata_device *);
    int (*set_mode)(struct ata_link *, struct ata_device **);
    unsigned int (*read_id)(struct ata_device *, struct ata_taskfile *, u16 *);
    void (*dev_config)(struct ata_device *);
    void (*freeze)(struct ata_port *);
    void (*thaw)(struct ata_port *);
    ata_prereset_fn_t prereset;
    ata_reset_fn_t softreset;
    ata_reset_fn_t hardreset;
    ata_postreset_fn_t postreset;
    ata_prereset_fn_t pmp_prereset;
    ata_reset_fn_t pmp_softreset;
    ata_reset_fn_t pmp_hardreset;
    ata_postreset_fn_t pmp_postreset;
    void (*error_handler)(struct ata_port *);
    void (*lost_interrupt)(struct ata_port *);
    void (*post_internal_cmd)(struct ata_queued_cmd *);
    void (*sched_eh)(struct ata_port *);
    void (*end_eh)(struct ata_port *);
    int (*scr_read)(struct ata_link *, unsigned int, u32 *);
    int (*scr_write)(struct ata_link *, unsigned int, u32);
    void (*pmp_attach)(struct ata_port *);
    void (*pmp_detach)(struct ata_port *);
    int (*set_lpm)(struct ata_link *, enum ata_lpm_policy, unsigned int);
    int (*port_suspend)(struct ata_port *, pm_message_t);
    int (*port_resume)(struct ata_port *);
    int (*port_start)(struct ata_port *);
    void (*port_stop)(struct ata_port *);
    void (*host_stop)(struct ata_host *);
    void (*sff_dev_select)(struct ata_port *, unsigned int);
    void (*sff_set_devctl)(struct ata_port *, u8);
    u8 (*sff_check_status)(struct ata_port *);
    u8 (*sff_check_altstatus)(struct ata_port *);
    void (*sff_tf_load)(struct ata_port *, const struct ata_taskfile *);
    void (*sff_tf_read)(struct ata_port *, struct ata_taskfile *);
    void (*sff_exec_command)(struct ata_port *, const struct ata_taskfile *);
    unsigned int (*sff_data_xfer)(struct ata_queued_cmd *, unsigned char *, unsigned int, int);
    void (*sff_irq_on)(struct ata_port *);
    bool (*sff_irq_check)(struct ata_port *);
    void (*sff_irq_clear)(struct ata_port *);
    void (*sff_drain_fifo)(struct ata_queued_cmd *);
    void (*bmdma_setup)(struct ata_queued_cmd *);
    void (*bmdma_start)(struct ata_queued_cmd *);
    void (*bmdma_stop)(struct ata_queued_cmd *);
    u8 (*bmdma_status)(struct ata_port *);
    ssize_t (*em_show)(struct ata_port *, char *);
    ssize_t (*em_store)(struct ata_port *, const char *, size_t);
    ssize_t (*sw_activity_show)(struct ata_device *, char *);
    ssize_t (*sw_activity_store)(struct ata_device *, enum sw_activity);
    ssize_t (*transmit_led_message)(struct ata_port *, u32, ssize_t);
    void (*phy_reset)(struct ata_port *);
    void (*eng_timeout)(struct ata_port *);
    const struct ata_port_operations *inherits;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ata_port_operations {
    int (*qc_defer)(struct ata_queued_cmd *);
    int (*check_atapi_dma)(struct ata_queued_cmd *);
    enum ata_completion_errors (*qc_prep)(struct ata_queued_cmd *);
    unsigned int (*qc_issue)(struct ata_queued_cmd *);
    bool (*qc_fill_rtf)(struct ata_queued_cmd *);
    int (*cable_detect)(struct ata_port *);
    long unsigned int (*mode_filter)(struct ata_device *, long unsigned int);
    void (*set_piomode)(struct ata_port *, struct ata_device *);
    void (*set_dmamode)(struct ata_port *, struct ata_device *);
    int (*set_mode)(struct ata_link *, struct ata_device **);
    unsigned int (*read_id)(struct ata_device *, struct ata_taskfile *, u16 *);
    void (*dev_config)(struct ata_device *);
    void (*freeze)(struct ata_port *);
    void (*thaw)(struct ata_port *);
    ata_prereset_fn_t prereset;
    ata_reset_fn_t softreset;
    ata_reset_fn_t hardreset;
    ata_postreset_fn_t postreset;
    ata_prereset_fn_t pmp_prereset;
    ata_reset_fn_t pmp_softreset;
    ata_reset_fn_t pmp_hardreset;
    ata_postreset_fn_t pmp_postreset;
    void (*error_handler)(struct ata_port *);
    void (*lost_interrupt)(struct ata_port *);
    void (*post_internal_cmd)(struct ata_queued_cmd *);
    void (*sched_eh)(struct ata_port *);
    void (*end_eh)(struct ata_port *);
    int (*scr_read)(struct ata_link *, unsigned int, u32 *);
    int (*scr_write)(struct ata_link *, unsigned int, u32);
    void (*pmp_attach)(struct ata_port *);
    void (*pmp_detach)(struct ata_port *);
    int (*set_lpm)(struct ata_link *, enum ata_lpm_policy, unsigned int);
    int (*port_suspend)(struct ata_port *, pm_message_t);
    int (*port_resume)(struct ata_port *);
    int (*port_start)(struct ata_port *);
    void (*port_stop)(struct ata_port *);
    void (*host_stop)(struct ata_host *);
    void (*sff_dev_select)(struct ata_port *, unsigned int);
    void (*sff_set_devctl)(struct ata_port *, u8);
    u8 (*sff_check_status)(struct ata_port *);
    u8 (*sff_check_altstatus)(struct ata_port *);
    void (*sff_tf_load)(struct ata_port *, const struct ata_taskfile *);
    void (*sff_tf_read)(struct ata_port *, struct ata_taskfile *);
    void (*sff_exec_command)(struct ata_port *, const struct ata_taskfile *);
    unsigned int (*sff_data_xfer)(struct ata_queued_cmd *, unsigned char *, unsigned int, int);
    void (*sff_irq_on)(struct ata_port *);
    bool (*sff_irq_check)(struct ata_port *);
    void (*sff_irq_clear)(struct ata_port *);
    void (*sff_drain_fifo)(struct ata_queued_cmd *);
    void (*bmdma_setup)(struct ata_queued_cmd *);
    void (*bmdma_start)(struct ata_queued_cmd *);
    void (*bmdma_stop)(struct ata_queued_cmd *);
    u8 (*bmdma_status)(struct ata_port *);
    ssize_t (*em_show)(struct ata_port *, char *);
    ssize_t (*em_store)(struct ata_port *, const char *, size_t);
    ssize_t (*sw_activity_show)(struct ata_device *, char *);
    ssize_t (*sw_activity_store)(struct ata_device *, enum sw_activity);
    ssize_t (*transmit_led_message)(struct ata_port *, u32, ssize_t);
    void (*phy_reset)(struct ata_port *);
    void (*eng_timeout)(struct ata_port *);
    const struct ata_port_operations *inherits;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ata_port_operations {
    int (*qc_defer)(struct ata_queued_cmd *);
    int (*check_atapi_dma)(struct ata_queued_cmd *);
    enum ata_completion_errors (*qc_prep)(struct ata_queued_cmd *);
    unsigned int (*qc_issue)(struct ata_queued_cmd *);
    bool (*qc_fill_rtf)(struct ata_queued_cmd *);
    int (*cable_detect)(struct ata_port *);
    long unsigned int (*mode_filter)(struct ata_device *, long unsigned int);
    void (*set_piomode)(struct ata_port *, struct ata_device *);
    void (*set_dmamode)(struct ata_port *, struct ata_device *);
    int (*set_mode)(struct ata_link *, struct ata_device **);
    unsigned int (*read_id)(struct ata_device *, struct ata_taskfile *, u16 *);
    void (*dev_config)(struct ata_device *);
    void (*freeze)(struct ata_port *);
    void (*thaw)(struct ata_port *);
    ata_prereset_fn_t prereset;
    ata_reset_fn_t softreset;
    ata_reset_fn_t hardreset;
    ata_postreset_fn_t postreset;
    ata_prereset_fn_t pmp_prereset;
    ata_reset_fn_t pmp_softreset;
    ata_reset_fn_t pmp_hardreset;
    ata_postreset_fn_t pmp_postreset;
    void (*error_handler)(struct ata_port *);
    void (*lost_interrupt)(struct ata_port *);
    void (*post_internal_cmd)(struct ata_queued_cmd *);
    void (*sched_eh)(struct ata_port *);
    void (*end_eh)(struct ata_port *);
    int (*scr_read)(struct ata_link *, unsigned int, u32 *);
    int (*scr_write)(struct ata_link *, unsigned int, u32);
    void (*pmp_attach)(struct ata_port *);
    void (*pmp_detach)(struct ata_port *);
    int (*set_lpm)(struct ata_link *, enum ata_lpm_policy, unsigned int);
    int (*port_suspend)(struct ata_port *, pm_message_t);
    int (*port_resume)(struct ata_port *);
    int (*port_start)(struct ata_port *);
    void (*port_stop)(struct ata_port *);
    void (*host_stop)(struct ata_host *);
    void (*sff_dev_select)(struct ata_port *, unsigned int);
    void (*sff_set_devctl)(struct ata_port *, u8);
    u8 (*sff_check_status)(struct ata_port *);
    u8 (*sff_check_altstatus)(struct ata_port *);
    void (*sff_tf_load)(struct ata_port *, const struct ata_taskfile *);
    void (*sff_tf_read)(struct ata_port *, struct ata_taskfile *);
    void (*sff_exec_command)(struct ata_port *, const struct ata_taskfile *);
    unsigned int (*sff_data_xfer)(struct ata_queued_cmd *, unsigned char *, unsigned int, int);
    void (*sff_irq_on)(struct ata_port *);
    bool (*sff_irq_check)(struct ata_port *);
    void (*sff_irq_clear)(struct ata_port *);
    void (*sff_drain_fifo)(struct ata_queued_cmd *);
    void (*bmdma_setup)(struct ata_queued_cmd *);
    void (*bmdma_start)(struct ata_queued_cmd *);
    void (*bmdma_stop)(struct ata_queued_cmd *);
    u8 (*bmdma_status)(struct ata_port *);
    ssize_t (*em_show)(struct ata_port *, char *);
    ssize_t (*em_store)(struct ata_port *, const char *, size_t);
    ssize_t (*sw_activity_show)(struct ata_device *, char *);
    ssize_t (*sw_activity_store)(struct ata_device *, enum sw_activity);
    ssize_t (*transmit_led_message)(struct ata_port *, u32, ssize_t);
    void (*phy_reset)(struct ata_port *);
    void (*eng_timeout)(struct ata_port *);
    const struct ata_port_operations *inherits;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ata_port_operations {
    int (*qc_defer)(struct ata_queued_cmd *);
    int (*check_atapi_dma)(struct ata_queued_cmd *);
    enum ata_completion_errors (*qc_prep)(struct ata_queued_cmd *);
    unsigned int (*qc_issue)(struct ata_queued_cmd *);
    bool (*qc_fill_rtf)(struct ata_queued_cmd *);
    int (*cable_detect)(struct ata_port *);
    long unsigned int (*mode_filter)(struct ata_device *, long unsigned int);
    void (*set_piomode)(struct ata_port *, struct ata_device *);
    void (*set_dmamode)(struct ata_port *, struct ata_device *);
    int (*set_mode)(struct ata_link *, struct ata_device **);
    unsigned int (*read_id)(struct ata_device *, struct ata_taskfile *, __le16 *);
    void (*dev_config)(struct ata_device *);
    void (*freeze)(struct ata_port *);
    void (*thaw)(struct ata_port *);
    ata_prereset_fn_t prereset;
    ata_reset_fn_t softreset;
    ata_reset_fn_t hardreset;
    ata_postreset_fn_t postreset;
    ata_prereset_fn_t pmp_prereset;
    ata_reset_fn_t pmp_softreset;
    ata_reset_fn_t pmp_hardreset;
    ata_postreset_fn_t pmp_postreset;
    void (*error_handler)(struct ata_port *);
    void (*lost_interrupt)(struct ata_port *);
    void (*post_internal_cmd)(struct ata_queued_cmd *);
    void (*sched_eh)(struct ata_port *);
    void (*end_eh)(struct ata_port *);
    int (*scr_read)(struct ata_link *, unsigned int, u32 *);
    int (*scr_write)(struct ata_link *, unsigned int, u32);
    void (*pmp_attach)(struct ata_port *);
    void (*pmp_detach)(struct ata_port *);
    int (*set_lpm)(struct ata_link *, enum ata_lpm_policy, unsigned int);
    int (*port_suspend)(struct ata_port *, pm_message_t);
    int (*port_resume)(struct ata_port *);
    int (*port_start)(struct ata_port *);
    void (*port_stop)(struct ata_port *);
    void (*host_stop)(struct ata_host *);
    void (*sff_dev_select)(struct ata_port *, unsigned int);
    void (*sff_set_devctl)(struct ata_port *, u8);
    u8 (*sff_check_status)(struct ata_port *);
    u8 (*sff_check_altstatus)(struct ata_port *);
    void (*sff_tf_load)(struct ata_port *, const struct ata_taskfile *);
    void (*sff_tf_read)(struct ata_port *, struct ata_taskfile *);
    void (*sff_exec_command)(struct ata_port *, const struct ata_taskfile *);
    unsigned int (*sff_data_xfer)(struct ata_queued_cmd *, unsigned char *, unsigned int, int);
    void (*sff_irq_on)(struct ata_port *);
    bool (*sff_irq_check)(struct ata_port *);
    void (*sff_irq_clear)(struct ata_port *);
    void (*sff_drain_fifo)(struct ata_queued_cmd *);
    void (*bmdma_setup)(struct ata_queued_cmd *);
    void (*bmdma_start)(struct ata_queued_cmd *);
    void (*bmdma_stop)(struct ata_queued_cmd *);
    u8 (*bmdma_status)(struct ata_port *);
    ssize_t (*em_show)(struct ata_port *, char *);
    ssize_t (*em_store)(struct ata_port *, const char *, size_t);
    ssize_t (*sw_activity_show)(struct ata_device *, char *);
    ssize_t (*sw_activity_store)(struct ata_device *, enum sw_activity);
    ssize_t (*transmit_led_message)(struct ata_port *, u32, ssize_t);
    void (*phy_reset)(struct ata_port *);
    void (*eng_timeout)(struct ata_port *);
    const struct ata_port_operations *inherits;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ata_port_operations {
    int (*qc_defer)(struct ata_queued_cmd *);
    int (*check_atapi_dma)(struct ata_queued_cmd *);
    enum ata_completion_errors (*qc_prep)(struct ata_queued_cmd *);
    unsigned int (*qc_issue)(struct ata_queued_cmd *);
    bool (*qc_fill_rtf)(struct ata_queued_cmd *);
    int (*cable_detect)(struct ata_port *);
    unsigned int (*mode_filter)(struct ata_device *, unsigned int);
    void (*set_piomode)(struct ata_port *, struct ata_device *);
    void (*set_dmamode)(struct ata_port *, struct ata_device *);
    int (*set_mode)(struct ata_link *, struct ata_device **);
    unsigned int (*read_id)(struct ata_device *, struct ata_taskfile *, __le16 *);
    void (*dev_config)(struct ata_device *);
    void (*freeze)(struct ata_port *);
    void (*thaw)(struct ata_port *);
    ata_prereset_fn_t prereset;
    ata_reset_fn_t softreset;
    ata_reset_fn_t hardreset;
    ata_postreset_fn_t postreset;
    ata_prereset_fn_t pmp_prereset;
    ata_reset_fn_t pmp_softreset;
    ata_reset_fn_t pmp_hardreset;
    ata_postreset_fn_t pmp_postreset;
    void (*error_handler)(struct ata_port *);
    void (*lost_interrupt)(struct ata_port *);
    void (*post_internal_cmd)(struct ata_queued_cmd *);
    void (*sched_eh)(struct ata_port *);
    void (*end_eh)(struct ata_port *);
    int (*scr_read)(struct ata_link *, unsigned int, u32 *);
    int (*scr_write)(struct ata_link *, unsigned int, u32);
    void (*pmp_attach)(struct ata_port *);
    void (*pmp_detach)(struct ata_port *);
    int (*set_lpm)(struct ata_link *, enum ata_lpm_policy, unsigned int);
    int (*port_suspend)(struct ata_port *, pm_message_t);
    int (*port_resume)(struct ata_port *);
    int (*port_start)(struct ata_port *);
    void (*port_stop)(struct ata_port *);
    void (*host_stop)(struct ata_host *);
    void (*sff_dev_select)(struct ata_port *, unsigned int);
    void (*sff_set_devctl)(struct ata_port *, u8);
    u8 (*sff_check_status)(struct ata_port *);
    u8 (*sff_check_altstatus)(struct ata_port *);
    void (*sff_tf_load)(struct ata_port *, const struct ata_taskfile *);
    void (*sff_tf_read)(struct ata_port *, struct ata_taskfile *);
    void (*sff_exec_command)(struct ata_port *, const struct ata_taskfile *);
    unsigned int (*sff_data_xfer)(struct ata_queued_cmd *, unsigned char *, unsigned int, int);
    void (*sff_irq_on)(struct ata_port *);
    bool (*sff_irq_check)(struct ata_port *);
    void (*sff_irq_clear)(struct ata_port *);
    void (*sff_drain_fifo)(struct ata_queued_cmd *);
    void (*bmdma_setup)(struct ata_queued_cmd *);
    void (*bmdma_start)(struct ata_queued_cmd *);
    void (*bmdma_stop)(struct ata_queued_cmd *);
    u8 (*bmdma_status)(struct ata_port *);
    ssize_t (*em_show)(struct ata_port *, char *);
    ssize_t (*em_store)(struct ata_port *, const char *, size_t);
    ssize_t (*sw_activity_show)(struct ata_device *, char *);
    ssize_t (*sw_activity_store)(struct ata_device *, enum sw_activity);
    ssize_t (*transmit_led_message)(struct ata_port *, u32, ssize_t);
    void (*phy_reset)(struct ata_port *);
    void (*eng_timeout)(struct ata_port *);
    const struct ata_port_operations *inherits;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ata_port_operations {
    int (*qc_defer)(struct ata_queued_cmd *);
    int (*check_atapi_dma)(struct ata_queued_cmd *);
    enum ata_completion_errors (*qc_prep)(struct ata_queued_cmd *);
    unsigned int (*qc_issue)(struct ata_queued_cmd *);
    void (*qc_fill_rtf)(struct ata_queued_cmd *);
    void (*qc_ncq_fill_rtf)(struct ata_port *, u64);
    int (*cable_detect)(struct ata_port *);
    unsigned int (*mode_filter)(struct ata_device *, unsigned int);
    void (*set_piomode)(struct ata_port *, struct ata_device *);
    void (*set_dmamode)(struct ata_port *, struct ata_device *);
    int (*set_mode)(struct ata_link *, struct ata_device **);
    unsigned int (*read_id)(struct ata_device *, struct ata_taskfile *, __le16 *);
    void (*dev_config)(struct ata_device *);
    void (*freeze)(struct ata_port *);
    void (*thaw)(struct ata_port *);
    ata_prereset_fn_t prereset;
    ata_reset_fn_t softreset;
    ata_reset_fn_t hardreset;
    ata_postreset_fn_t postreset;
    ata_prereset_fn_t pmp_prereset;
    ata_reset_fn_t pmp_softreset;
    ata_reset_fn_t pmp_hardreset;
    ata_postreset_fn_t pmp_postreset;
    void (*error_handler)(struct ata_port *);
    void (*lost_interrupt)(struct ata_port *);
    void (*post_internal_cmd)(struct ata_queued_cmd *);
    void (*sched_eh)(struct ata_port *);
    void (*end_eh)(struct ata_port *);
    int (*scr_read)(struct ata_link *, unsigned int, u32 *);
    int (*scr_write)(struct ata_link *, unsigned int, u32);
    void (*pmp_attach)(struct ata_port *);
    void (*pmp_detach)(struct ata_port *);
    int (*set_lpm)(struct ata_link *, enum ata_lpm_policy, unsigned int);
    int (*port_suspend)(struct ata_port *, pm_message_t);
    int (*port_resume)(struct ata_port *);
    int (*port_start)(struct ata_port *);
    void (*port_stop)(struct ata_port *);
    void (*host_stop)(struct ata_host *);
    void (*sff_dev_select)(struct ata_port *, unsigned int);
    void (*sff_set_devctl)(struct ata_port *, u8);
    u8 (*sff_check_status)(struct ata_port *);
    u8 (*sff_check_altstatus)(struct ata_port *);
    void (*sff_tf_load)(struct ata_port *, const struct ata_taskfile *);
    void (*sff_tf_read)(struct ata_port *, struct ata_taskfile *);
    void (*sff_exec_command)(struct ata_port *, const struct ata_taskfile *);
    unsigned int (*sff_data_xfer)(struct ata_queued_cmd *, unsigned char *, unsigned int, int);
    void (*sff_irq_on)(struct ata_port *);
    bool (*sff_irq_check)(struct ata_port *);
    void (*sff_irq_clear)(struct ata_port *);
    void (*sff_drain_fifo)(struct ata_queued_cmd *);
    void (*bmdma_setup)(struct ata_queued_cmd *);
    void (*bmdma_start)(struct ata_queued_cmd *);
    void (*bmdma_stop)(struct ata_queued_cmd *);
    u8 (*bmdma_status)(struct ata_port *);
    ssize_t (*em_show)(struct ata_port *, char *);
    ssize_t (*em_store)(struct ata_port *, const char *, size_t);
    ssize_t (*sw_activity_show)(struct ata_device *, char *);
    ssize_t (*sw_activity_store)(struct ata_device *, enum sw_activity);
    ssize_t (*transmit_led_message)(struct ata_port *, u32, ssize_t);
    void (*phy_reset)(struct ata_port *);
    void (*eng_timeout)(struct ata_port *);
    const struct ata_port_operations *inherits;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ata_port_operations {
    int (*qc_defer)(struct ata_queued_cmd *);
    int (*check_atapi_dma)(struct ata_queued_cmd *);
    enum ata_completion_errors (*qc_prep)(struct ata_queued_cmd *);
    unsigned int (*qc_issue)(struct ata_queued_cmd *);
    void (*qc_fill_rtf)(struct ata_queued_cmd *);
    void (*qc_ncq_fill_rtf)(struct ata_port *, u64);
    int (*cable_detect)(struct ata_port *);
    unsigned int (*mode_filter)(struct ata_device *, unsigned int);
    void (*set_piomode)(struct ata_port *, struct ata_device *);
    void (*set_dmamode)(struct ata_port *, struct ata_device *);
    int (*set_mode)(struct ata_link *, struct ata_device **);
    unsigned int (*read_id)(struct ata_device *, struct ata_taskfile *, __le16 *);
    void (*dev_config)(struct ata_device *);
    void (*freeze)(struct ata_port *);
    void (*thaw)(struct ata_port *);
    ata_prereset_fn_t prereset;
    ata_reset_fn_t softreset;
    ata_reset_fn_t hardreset;
    ata_postreset_fn_t postreset;
    ata_prereset_fn_t pmp_prereset;
    ata_reset_fn_t pmp_softreset;
    ata_reset_fn_t pmp_hardreset;
    ata_postreset_fn_t pmp_postreset;
    void (*error_handler)(struct ata_port *);
    void (*lost_interrupt)(struct ata_port *);
    void (*post_internal_cmd)(struct ata_queued_cmd *);
    void (*sched_eh)(struct ata_port *);
    void (*end_eh)(struct ata_port *);
    int (*scr_read)(struct ata_link *, unsigned int, u32 *);
    int (*scr_write)(struct ata_link *, unsigned int, u32);
    void (*pmp_attach)(struct ata_port *);
    void (*pmp_detach)(struct ata_port *);
    int (*set_lpm)(struct ata_link *, enum ata_lpm_policy, unsigned int);
    int (*port_suspend)(struct ata_port *, pm_message_t);
    int (*port_resume)(struct ata_port *);
    int (*port_start)(struct ata_port *);
    void (*port_stop)(struct ata_port *);
    void (*host_stop)(struct ata_host *);
    void (*sff_dev_select)(struct ata_port *, unsigned int);
    void (*sff_set_devctl)(struct ata_port *, u8);
    u8 (*sff_check_status)(struct ata_port *);
    u8 (*sff_check_altstatus)(struct ata_port *);
    void (*sff_tf_load)(struct ata_port *, const struct ata_taskfile *);
    void (*sff_tf_read)(struct ata_port *, struct ata_taskfile *);
    void (*sff_exec_command)(struct ata_port *, const struct ata_taskfile *);
    unsigned int (*sff_data_xfer)(struct ata_queued_cmd *, unsigned char *, unsigned int, int);
    void (*sff_irq_on)(struct ata_port *);
    bool (*sff_irq_check)(struct ata_port *);
    void (*sff_irq_clear)(struct ata_port *);
    void (*sff_drain_fifo)(struct ata_queued_cmd *);
    void (*bmdma_setup)(struct ata_queued_cmd *);
    void (*bmdma_start)(struct ata_queued_cmd *);
    void (*bmdma_stop)(struct ata_queued_cmd *);
    u8 (*bmdma_status)(struct ata_port *);
    ssize_t (*em_show)(struct ata_port *, char *);
    ssize_t (*em_store)(struct ata_port *, const char *, size_t);
    ssize_t (*sw_activity_show)(struct ata_device *, char *);
    ssize_t (*sw_activity_store)(struct ata_device *, enum sw_activity);
    ssize_t (*transmit_led_message)(struct ata_port *, u32, ssize_t);
    const struct ata_port_operations *inherits;
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
struct ata_port_operations {
    int (*qc_defer)(struct ata_queued_cmd *);
    int (*check_atapi_dma)(struct ata_queued_cmd *);
    void (*qc_prep)(struct ata_queued_cmd *);
    unsigned int (*qc_issue)(struct ata_queued_cmd *);
    bool (*qc_fill_rtf)(struct ata_queued_cmd *);
    int (*cable_detect)(struct ata_port *);
    long unsigned int (*mode_filter)(struct ata_device *, long unsigned int);
    void (*set_piomode)(struct ata_port *, struct ata_device *);
    void (*set_dmamode)(struct ata_port *, struct ata_device *);
    int (*set_mode)(struct ata_link *, struct ata_device **);
    unsigned int (*read_id)(struct ata_device *, struct ata_taskfile *, u16 *);
    void (*dev_config)(struct ata_device *);
    void (*freeze)(struct ata_port *);
    void (*thaw)(struct ata_port *);
    ata_prereset_fn_t prereset;
    ata_reset_fn_t softreset;
    ata_reset_fn_t hardreset;
    ata_postreset_fn_t postreset;
    ata_prereset_fn_t pmp_prereset;
    ata_reset_fn_t pmp_softreset;
    ata_reset_fn_t pmp_hardreset;
    ata_postreset_fn_t pmp_postreset;
    void (*error_handler)(struct ata_port *);
    void (*lost_interrupt)(struct ata_port *);
    void (*post_internal_cmd)(struct ata_queued_cmd *);
    void (*sched_eh)(struct ata_port *);
    void (*end_eh)(struct ata_port *);
    int (*scr_read)(struct ata_link *, unsigned int, u32 *);
    int (*scr_write)(struct ata_link *, unsigned int, u32);
    void (*pmp_attach)(struct ata_port *);
    void (*pmp_detach)(struct ata_port *);
    int (*set_lpm)(struct ata_link *, enum ata_lpm_policy, unsigned int);
    int (*port_suspend)(struct ata_port *, pm_message_t);
    int (*port_resume)(struct ata_port *);
    int (*port_start)(struct ata_port *);
    void (*port_stop)(struct ata_port *);
    void (*host_stop)(struct ata_host *);
    void (*sff_dev_select)(struct ata_port *, unsigned int);
    void (*sff_set_devctl)(struct ata_port *, u8);
    u8 (*sff_check_status)(struct ata_port *);
    u8 (*sff_check_altstatus)(struct ata_port *);
    void (*sff_tf_load)(struct ata_port *, const struct ata_taskfile *);
    void (*sff_tf_read)(struct ata_port *, struct ata_taskfile *);
    void (*sff_exec_command)(struct ata_port *, const struct ata_taskfile *);
    unsigned int (*sff_data_xfer)(struct ata_queued_cmd *, unsigned char *, unsigned int, int);
    void (*sff_irq_on)(struct ata_port *);
    bool (*sff_irq_check)(struct ata_port *);
    void (*sff_irq_clear)(struct ata_port *);
    void (*sff_drain_fifo)(struct ata_queued_cmd *);
    void (*bmdma_setup)(struct ata_queued_cmd *);
    void (*bmdma_start)(struct ata_queued_cmd *);
    void (*bmdma_stop)(struct ata_queued_cmd *);
    u8 (*bmdma_status)(struct ata_port *);
    ssize_t (*em_show)(struct ata_port *, char *);
    ssize_t (*em_store)(struct ata_port *, const char *, size_t);
    ssize_t (*sw_activity_show)(struct ata_device *, char *);
    ssize_t (*sw_activity_store)(struct ata_device *, enum sw_activity);
    ssize_t (*transmit_led_message)(struct ata_port *, u32, ssize_t);
    void (*phy_reset)(struct ata_port *);
    void (*eng_timeout)(struct ata_port *);
    const struct ata_port_operations *inherits;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ata_port_operations {
    int (*qc_defer)(struct ata_queued_cmd *);
    int (*check_atapi_dma)(struct ata_queued_cmd *);
    void (*qc_prep)(struct ata_queued_cmd *);
    unsigned int (*qc_issue)(struct ata_queued_cmd *);
    bool (*qc_fill_rtf)(struct ata_queued_cmd *);
    int (*cable_detect)(struct ata_port *);
    long unsigned int (*mode_filter)(struct ata_device *, long unsigned int);
    void (*set_piomode)(struct ata_port *, struct ata_device *);
    void (*set_dmamode)(struct ata_port *, struct ata_device *);
    int (*set_mode)(struct ata_link *, struct ata_device **);
    unsigned int (*read_id)(struct ata_device *, struct ata_taskfile *, u16 *);
    void (*dev_config)(struct ata_device *);
    void (*freeze)(struct ata_port *);
    void (*thaw)(struct ata_port *);
    ata_prereset_fn_t prereset;
    ata_reset_fn_t softreset;
    ata_reset_fn_t hardreset;
    ata_postreset_fn_t postreset;
    ata_prereset_fn_t pmp_prereset;
    ata_reset_fn_t pmp_softreset;
    ata_reset_fn_t pmp_hardreset;
    ata_postreset_fn_t pmp_postreset;
    void (*error_handler)(struct ata_port *);
    void (*lost_interrupt)(struct ata_port *);
    void (*post_internal_cmd)(struct ata_queued_cmd *);
    void (*sched_eh)(struct ata_port *);
    void (*end_eh)(struct ata_port *);
    int (*scr_read)(struct ata_link *, unsigned int, u32 *);
    int (*scr_write)(struct ata_link *, unsigned int, u32);
    void (*pmp_attach)(struct ata_port *);
    void (*pmp_detach)(struct ata_port *);
    int (*set_lpm)(struct ata_link *, enum ata_lpm_policy, unsigned int);
    int (*port_suspend)(struct ata_port *, pm_message_t);
    int (*port_resume)(struct ata_port *);
    int (*port_start)(struct ata_port *);
    void (*port_stop)(struct ata_port *);
    void (*host_stop)(struct ata_host *);
    void (*sff_dev_select)(struct ata_port *, unsigned int);
    void (*sff_set_devctl)(struct ata_port *, u8);
    u8 (*sff_check_status)(struct ata_port *);
    u8 (*sff_check_altstatus)(struct ata_port *);
    void (*sff_tf_load)(struct ata_port *, const struct ata_taskfile *);
    void (*sff_tf_read)(struct ata_port *, struct ata_taskfile *);
    void (*sff_exec_command)(struct ata_port *, const struct ata_taskfile *);
    unsigned int (*sff_data_xfer)(struct ata_queued_cmd *, unsigned char *, unsigned int, int);
    void (*sff_irq_on)(struct ata_port *);
    bool (*sff_irq_check)(struct ata_port *);
    void (*sff_irq_clear)(struct ata_port *);
    void (*sff_drain_fifo)(struct ata_queued_cmd *);
    void (*bmdma_setup)(struct ata_queued_cmd *);
    void (*bmdma_start)(struct ata_queued_cmd *);
    void (*bmdma_stop)(struct ata_queued_cmd *);
    u8 (*bmdma_status)(struct ata_port *);
    ssize_t (*em_show)(struct ata_port *, char *);
    ssize_t (*em_store)(struct ata_port *, const char *, size_t);
    ssize_t (*sw_activity_show)(struct ata_device *, char *);
    ssize_t (*sw_activity_store)(struct ata_device *, enum sw_activity);
    ssize_t (*transmit_led_message)(struct ata_port *, u32, ssize_t);
    void (*phy_reset)(struct ata_port *);
    void (*eng_timeout)(struct ata_port *);
    const struct ata_port_operations *inherits;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ata_port_operations {
    int (*qc_defer)(struct ata_queued_cmd *);
    int (*check_atapi_dma)(struct ata_queued_cmd *);
    void (*qc_prep)(struct ata_queued_cmd *);
    unsigned int (*qc_issue)(struct ata_queued_cmd *);
    bool (*qc_fill_rtf)(struct ata_queued_cmd *);
    int (*cable_detect)(struct ata_port *);
    long unsigned int (*mode_filter)(struct ata_device *, long unsigned int);
    void (*set_piomode)(struct ata_port *, struct ata_device *);
    void (*set_dmamode)(struct ata_port *, struct ata_device *);
    int (*set_mode)(struct ata_link *, struct ata_device **);
    unsigned int (*read_id)(struct ata_device *, struct ata_taskfile *, u16 *);
    void (*dev_config)(struct ata_device *);
    void (*freeze)(struct ata_port *);
    void (*thaw)(struct ata_port *);
    ata_prereset_fn_t prereset;
    ata_reset_fn_t softreset;
    ata_reset_fn_t hardreset;
    ata_postreset_fn_t postreset;
    ata_prereset_fn_t pmp_prereset;
    ata_reset_fn_t pmp_softreset;
    ata_reset_fn_t pmp_hardreset;
    ata_postreset_fn_t pmp_postreset;
    void (*error_handler)(struct ata_port *);
    void (*lost_interrupt)(struct ata_port *);
    void (*post_internal_cmd)(struct ata_queued_cmd *);
    void (*sched_eh)(struct ata_port *);
    void (*end_eh)(struct ata_port *);
    int (*scr_read)(struct ata_link *, unsigned int, u32 *);
    int (*scr_write)(struct ata_link *, unsigned int, u32);
    void (*pmp_attach)(struct ata_port *);
    void (*pmp_detach)(struct ata_port *);
    int (*set_lpm)(struct ata_link *, enum ata_lpm_policy, unsigned int);
    int (*port_suspend)(struct ata_port *, pm_message_t);
    int (*port_resume)(struct ata_port *);
    int (*port_start)(struct ata_port *);
    void (*port_stop)(struct ata_port *);
    void (*host_stop)(struct ata_host *);
    void (*sff_dev_select)(struct ata_port *, unsigned int);
    void (*sff_set_devctl)(struct ata_port *, u8);
    u8 (*sff_check_status)(struct ata_port *);
    u8 (*sff_check_altstatus)(struct ata_port *);
    void (*sff_tf_load)(struct ata_port *, const struct ata_taskfile *);
    void (*sff_tf_read)(struct ata_port *, struct ata_taskfile *);
    void (*sff_exec_command)(struct ata_port *, const struct ata_taskfile *);
    unsigned int (*sff_data_xfer)(struct ata_queued_cmd *, unsigned char *, unsigned int, int);
    void (*sff_irq_on)(struct ata_port *);
    bool (*sff_irq_check)(struct ata_port *);
    void (*sff_irq_clear)(struct ata_port *);
    void (*sff_drain_fifo)(struct ata_queued_cmd *);
    void (*bmdma_setup)(struct ata_queued_cmd *);
    void (*bmdma_start)(struct ata_queued_cmd *);
    void (*bmdma_stop)(struct ata_queued_cmd *);
    u8 (*bmdma_status)(struct ata_port *);
    ssize_t (*em_show)(struct ata_port *, char *);
    ssize_t (*em_store)(struct ata_port *, const char *, size_t);
    ssize_t (*sw_activity_show)(struct ata_device *, char *);
    ssize_t (*sw_activity_store)(struct ata_device *, enum sw_activity);
    ssize_t (*transmit_led_message)(struct ata_port *, u32, ssize_t);
    void (*phy_reset)(struct ata_port *);
    void (*eng_timeout)(struct ata_port *);
    const struct ata_port_operations *inherits;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ata_port_operations {
    int (*qc_defer)(struct ata_queued_cmd *);
    int (*check_atapi_dma)(struct ata_queued_cmd *);
    void (*qc_prep)(struct ata_queued_cmd *);
    unsigned int (*qc_issue)(struct ata_queued_cmd *);
    bool (*qc_fill_rtf)(struct ata_queued_cmd *);
    int (*cable_detect)(struct ata_port *);
    long unsigned int (*mode_filter)(struct ata_device *, long unsigned int);
    void (*set_piomode)(struct ata_port *, struct ata_device *);
    void (*set_dmamode)(struct ata_port *, struct ata_device *);
    int (*set_mode)(struct ata_link *, struct ata_device **);
    unsigned int (*read_id)(struct ata_device *, struct ata_taskfile *, u16 *);
    void (*dev_config)(struct ata_device *);
    void (*freeze)(struct ata_port *);
    void (*thaw)(struct ata_port *);
    ata_prereset_fn_t prereset;
    ata_reset_fn_t softreset;
    ata_reset_fn_t hardreset;
    ata_postreset_fn_t postreset;
    ata_prereset_fn_t pmp_prereset;
    ata_reset_fn_t pmp_softreset;
    ata_reset_fn_t pmp_hardreset;
    ata_postreset_fn_t pmp_postreset;
    void (*error_handler)(struct ata_port *);
    void (*lost_interrupt)(struct ata_port *);
    void (*post_internal_cmd)(struct ata_queued_cmd *);
    void (*sched_eh)(struct ata_port *);
    void (*end_eh)(struct ata_port *);
    int (*scr_read)(struct ata_link *, unsigned int, u32 *);
    int (*scr_write)(struct ata_link *, unsigned int, u32);
    void (*pmp_attach)(struct ata_port *);
    void (*pmp_detach)(struct ata_port *);
    int (*set_lpm)(struct ata_link *, enum ata_lpm_policy, unsigned int);
    int (*port_suspend)(struct ata_port *, pm_message_t);
    int (*port_resume)(struct ata_port *);
    int (*port_start)(struct ata_port *);
    void (*port_stop)(struct ata_port *);
    void (*host_stop)(struct ata_host *);
    void (*sff_dev_select)(struct ata_port *, unsigned int);
    void (*sff_set_devctl)(struct ata_port *, u8);
    u8 (*sff_check_status)(struct ata_port *);
    u8 (*sff_check_altstatus)(struct ata_port *);
    void (*sff_tf_load)(struct ata_port *, const struct ata_taskfile *);
    void (*sff_tf_read)(struct ata_port *, struct ata_taskfile *);
    void (*sff_exec_command)(struct ata_port *, const struct ata_taskfile *);
    unsigned int (*sff_data_xfer)(struct ata_queued_cmd *, unsigned char *, unsigned int, int);
    void (*sff_irq_on)(struct ata_port *);
    bool (*sff_irq_check)(struct ata_port *);
    void (*sff_irq_clear)(struct ata_port *);
    void (*sff_drain_fifo)(struct ata_queued_cmd *);
    void (*bmdma_setup)(struct ata_queued_cmd *);
    void (*bmdma_start)(struct ata_queued_cmd *);
    void (*bmdma_stop)(struct ata_queued_cmd *);
    u8 (*bmdma_status)(struct ata_port *);
    ssize_t (*em_show)(struct ata_port *, char *);
    ssize_t (*em_store)(struct ata_port *, const char *, size_t);
    ssize_t (*sw_activity_show)(struct ata_device *, char *);
    ssize_t (*sw_activity_store)(struct ata_device *, enum sw_activity);
    ssize_t (*transmit_led_message)(struct ata_port *, u32, ssize_t);
    void (*phy_reset)(struct ata_port *);
    void (*eng_timeout)(struct ata_port *);
    const struct ata_port_operations *inherits;
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
struct ata_port_operations {
    int (*qc_defer)(struct ata_queued_cmd *);
    int (*check_atapi_dma)(struct ata_queued_cmd *);
    void (*qc_prep)(struct ata_queued_cmd *);
    unsigned int (*qc_issue)(struct ata_queued_cmd *);
    bool (*qc_fill_rtf)(struct ata_queued_cmd *);
    int (*cable_detect)(struct ata_port *);
    long unsigned int (*mode_filter)(struct ata_device *, long unsigned int);
    void (*set_piomode)(struct ata_port *, struct ata_device *);
    void (*set_dmamode)(struct ata_port *, struct ata_device *);
    int (*set_mode)(struct ata_link *, struct ata_device **);
    unsigned int (*read_id)(struct ata_device *, struct ata_taskfile *, u16 *);
    void (*dev_config)(struct ata_device *);
    void (*freeze)(struct ata_port *);
    void (*thaw)(struct ata_port *);
    ata_prereset_fn_t prereset;
    ata_reset_fn_t softreset;
    ata_reset_fn_t hardreset;
    ata_postreset_fn_t postreset;
    ata_prereset_fn_t pmp_prereset;
    ata_reset_fn_t pmp_softreset;
    ata_reset_fn_t pmp_hardreset;
    ata_postreset_fn_t pmp_postreset;
    void (*error_handler)(struct ata_port *);
    void (*lost_interrupt)(struct ata_port *);
    void (*post_internal_cmd)(struct ata_queued_cmd *);
    void (*sched_eh)(struct ata_port *);
    void (*end_eh)(struct ata_port *);
    int (*scr_read)(struct ata_link *, unsigned int, u32 *);
    int (*scr_write)(struct ata_link *, unsigned int, u32);
    void (*pmp_attach)(struct ata_port *);
    void (*pmp_detach)(struct ata_port *);
    int (*set_lpm)(struct ata_link *, enum ata_lpm_policy, unsigned int);
    int (*port_suspend)(struct ata_port *, pm_message_t);
    int (*port_resume)(struct ata_port *);
    int (*port_start)(struct ata_port *);
    void (*port_stop)(struct ata_port *);
    void (*host_stop)(struct ata_host *);
    void (*sff_dev_select)(struct ata_port *, unsigned int);
    void (*sff_set_devctl)(struct ata_port *, u8);
    u8 (*sff_check_status)(struct ata_port *);
    u8 (*sff_check_altstatus)(struct ata_port *);
    void (*sff_tf_load)(struct ata_port *, const struct ata_taskfile *);
    void (*sff_tf_read)(struct ata_port *, struct ata_taskfile *);
    void (*sff_exec_command)(struct ata_port *, const struct ata_taskfile *);
    unsigned int (*sff_data_xfer)(struct ata_queued_cmd *, unsigned char *, unsigned int, int);
    void (*sff_irq_on)(struct ata_port *);
    bool (*sff_irq_check)(struct ata_port *);
    void (*sff_irq_clear)(struct ata_port *);
    void (*sff_drain_fifo)(struct ata_queued_cmd *);
    void (*bmdma_setup)(struct ata_queued_cmd *);
    void (*bmdma_start)(struct ata_queued_cmd *);
    void (*bmdma_stop)(struct ata_queued_cmd *);
    u8 (*bmdma_status)(struct ata_port *);
    ssize_t (*em_show)(struct ata_port *, char *);
    ssize_t (*em_store)(struct ata_port *, const char *, size_t);
    ssize_t (*sw_activity_show)(struct ata_device *, char *);
    ssize_t (*sw_activity_store)(struct ata_device *, enum sw_activity);
    ssize_t (*transmit_led_message)(struct ata_port *, u32, ssize_t);
    void (*phy_reset)(struct ata_port *);
    void (*eng_timeout)(struct ata_port *);
    const struct ata_port_operations *inherits;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ata_port_operations {
    int (*qc_defer)(struct ata_queued_cmd *);
    int (*check_atapi_dma)(struct ata_queued_cmd *);
    void (*qc_prep)(struct ata_queued_cmd *);
    unsigned int (*qc_issue)(struct ata_queued_cmd *);
    bool (*qc_fill_rtf)(struct ata_queued_cmd *);
    int (*cable_detect)(struct ata_port *);
    long unsigned int (*mode_filter)(struct ata_device *, long unsigned int);
    void (*set_piomode)(struct ata_port *, struct ata_device *);
    void (*set_dmamode)(struct ata_port *, struct ata_device *);
    int (*set_mode)(struct ata_link *, struct ata_device **);
    unsigned int (*read_id)(struct ata_device *, struct ata_taskfile *, u16 *);
    void (*dev_config)(struct ata_device *);
    void (*freeze)(struct ata_port *);
    void (*thaw)(struct ata_port *);
    ata_prereset_fn_t prereset;
    ata_reset_fn_t softreset;
    ata_reset_fn_t hardreset;
    ata_postreset_fn_t postreset;
    ata_prereset_fn_t pmp_prereset;
    ata_reset_fn_t pmp_softreset;
    ata_reset_fn_t pmp_hardreset;
    ata_postreset_fn_t pmp_postreset;
    void (*error_handler)(struct ata_port *);
    void (*lost_interrupt)(struct ata_port *);
    void (*post_internal_cmd)(struct ata_queued_cmd *);
    void (*sched_eh)(struct ata_port *);
    void (*end_eh)(struct ata_port *);
    int (*scr_read)(struct ata_link *, unsigned int, u32 *);
    int (*scr_write)(struct ata_link *, unsigned int, u32);
    void (*pmp_attach)(struct ata_port *);
    void (*pmp_detach)(struct ata_port *);
    int (*set_lpm)(struct ata_link *, enum ata_lpm_policy, unsigned int);
    int (*port_suspend)(struct ata_port *, pm_message_t);
    int (*port_resume)(struct ata_port *);
    int (*port_start)(struct ata_port *);
    void (*port_stop)(struct ata_port *);
    void (*host_stop)(struct ata_host *);
    void (*sff_dev_select)(struct ata_port *, unsigned int);
    void (*sff_set_devctl)(struct ata_port *, u8);
    u8 (*sff_check_status)(struct ata_port *);
    u8 (*sff_check_altstatus)(struct ata_port *);
    void (*sff_tf_load)(struct ata_port *, const struct ata_taskfile *);
    void (*sff_tf_read)(struct ata_port *, struct ata_taskfile *);
    void (*sff_exec_command)(struct ata_port *, const struct ata_taskfile *);
    unsigned int (*sff_data_xfer)(struct ata_queued_cmd *, unsigned char *, unsigned int, int);
    void (*sff_irq_on)(struct ata_port *);
    bool (*sff_irq_check)(struct ata_port *);
    void (*sff_irq_clear)(struct ata_port *);
    void (*sff_drain_fifo)(struct ata_queued_cmd *);
    void (*bmdma_setup)(struct ata_queued_cmd *);
    void (*bmdma_start)(struct ata_queued_cmd *);
    void (*bmdma_stop)(struct ata_queued_cmd *);
    u8 (*bmdma_status)(struct ata_port *);
    ssize_t (*em_show)(struct ata_port *, char *);
    ssize_t (*em_store)(struct ata_port *, const char *, size_t);
    ssize_t (*sw_activity_show)(struct ata_device *, char *);
    ssize_t (*sw_activity_store)(struct ata_device *, enum sw_activity);
    ssize_t (*transmit_led_message)(struct ata_port *, u32, ssize_t);
    void (*phy_reset)(struct ata_port *);
    void (*eng_timeout)(struct ata_port *);
    const struct ata_port_operations *inherits;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ata_port_operations {
    int (*qc_defer)(struct ata_queued_cmd *);
    int (*check_atapi_dma)(struct ata_queued_cmd *);
    void (*qc_prep)(struct ata_queued_cmd *);
    unsigned int (*qc_issue)(struct ata_queued_cmd *);
    bool (*qc_fill_rtf)(struct ata_queued_cmd *);
    int (*cable_detect)(struct ata_port *);
    long unsigned int (*mode_filter)(struct ata_device *, long unsigned int);
    void (*set_piomode)(struct ata_port *, struct ata_device *);
    void (*set_dmamode)(struct ata_port *, struct ata_device *);
    int (*set_mode)(struct ata_link *, struct ata_device **);
    unsigned int (*read_id)(struct ata_device *, struct ata_taskfile *, u16 *);
    void (*dev_config)(struct ata_device *);
    void (*freeze)(struct ata_port *);
    void (*thaw)(struct ata_port *);
    ata_prereset_fn_t prereset;
    ata_reset_fn_t softreset;
    ata_reset_fn_t hardreset;
    ata_postreset_fn_t postreset;
    ata_prereset_fn_t pmp_prereset;
    ata_reset_fn_t pmp_softreset;
    ata_reset_fn_t pmp_hardreset;
    ata_postreset_fn_t pmp_postreset;
    void (*error_handler)(struct ata_port *);
    void (*lost_interrupt)(struct ata_port *);
    void (*post_internal_cmd)(struct ata_queued_cmd *);
    void (*sched_eh)(struct ata_port *);
    void (*end_eh)(struct ata_port *);
    int (*scr_read)(struct ata_link *, unsigned int, u32 *);
    int (*scr_write)(struct ata_link *, unsigned int, u32);
    void (*pmp_attach)(struct ata_port *);
    void (*pmp_detach)(struct ata_port *);
    int (*set_lpm)(struct ata_link *, enum ata_lpm_policy, unsigned int);
    int (*port_suspend)(struct ata_port *, pm_message_t);
    int (*port_resume)(struct ata_port *);
    int (*port_start)(struct ata_port *);
    void (*port_stop)(struct ata_port *);
    void (*host_stop)(struct ata_host *);
    void (*sff_dev_select)(struct ata_port *, unsigned int);
    void (*sff_set_devctl)(struct ata_port *, u8);
    u8 (*sff_check_status)(struct ata_port *);
    u8 (*sff_check_altstatus)(struct ata_port *);
    void (*sff_tf_load)(struct ata_port *, const struct ata_taskfile *);
    void (*sff_tf_read)(struct ata_port *, struct ata_taskfile *);
    void (*sff_exec_command)(struct ata_port *, const struct ata_taskfile *);
    unsigned int (*sff_data_xfer)(struct ata_queued_cmd *, unsigned char *, unsigned int, int);
    void (*sff_irq_on)(struct ata_port *);
    bool (*sff_irq_check)(struct ata_port *);
    void (*sff_irq_clear)(struct ata_port *);
    void (*sff_drain_fifo)(struct ata_queued_cmd *);
    void (*bmdma_setup)(struct ata_queued_cmd *);
    void (*bmdma_start)(struct ata_queued_cmd *);
    void (*bmdma_stop)(struct ata_queued_cmd *);
    u8 (*bmdma_status)(struct ata_port *);
    ssize_t (*em_show)(struct ata_port *, char *);
    ssize_t (*em_store)(struct ata_port *, const char *, size_t);
    ssize_t (*sw_activity_show)(struct ata_device *, char *);
    ssize_t (*sw_activity_store)(struct ata_device *, enum sw_activity);
    ssize_t (*transmit_led_message)(struct ata_port *, u32, ssize_t);
    void (*phy_reset)(struct ata_port *);
    void (*eng_timeout)(struct ata_port *);
    const struct ata_port_operations *inherits;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ata_port_operations {
    int (*qc_defer)(struct ata_queued_cmd *);
    int (*check_atapi_dma)(struct ata_queued_cmd *);
    void (*qc_prep)(struct ata_queued_cmd *);
    unsigned int (*qc_issue)(struct ata_queued_cmd *);
    bool (*qc_fill_rtf)(struct ata_queued_cmd *);
    int (*cable_detect)(struct ata_port *);
    long unsigned int (*mode_filter)(struct ata_device *, long unsigned int);
    void (*set_piomode)(struct ata_port *, struct ata_device *);
    void (*set_dmamode)(struct ata_port *, struct ata_device *);
    int (*set_mode)(struct ata_link *, struct ata_device **);
    unsigned int (*read_id)(struct ata_device *, struct ata_taskfile *, u16 *);
    void (*dev_config)(struct ata_device *);
    void (*freeze)(struct ata_port *);
    void (*thaw)(struct ata_port *);
    ata_prereset_fn_t prereset;
    ata_reset_fn_t softreset;
    ata_reset_fn_t hardreset;
    ata_postreset_fn_t postreset;
    ata_prereset_fn_t pmp_prereset;
    ata_reset_fn_t pmp_softreset;
    ata_reset_fn_t pmp_hardreset;
    ata_postreset_fn_t pmp_postreset;
    void (*error_handler)(struct ata_port *);
    void (*lost_interrupt)(struct ata_port *);
    void (*post_internal_cmd)(struct ata_queued_cmd *);
    void (*sched_eh)(struct ata_port *);
    void (*end_eh)(struct ata_port *);
    int (*scr_read)(struct ata_link *, unsigned int, u32 *);
    int (*scr_write)(struct ata_link *, unsigned int, u32);
    void (*pmp_attach)(struct ata_port *);
    void (*pmp_detach)(struct ata_port *);
    int (*set_lpm)(struct ata_link *, enum ata_lpm_policy, unsigned int);
    int (*port_suspend)(struct ata_port *, pm_message_t);
    int (*port_resume)(struct ata_port *);
    int (*port_start)(struct ata_port *);
    void (*port_stop)(struct ata_port *);
    void (*host_stop)(struct ata_host *);
    void (*sff_dev_select)(struct ata_port *, unsigned int);
    void (*sff_set_devctl)(struct ata_port *, u8);
    u8 (*sff_check_status)(struct ata_port *);
    u8 (*sff_check_altstatus)(struct ata_port *);
    void (*sff_tf_load)(struct ata_port *, const struct ata_taskfile *);
    void (*sff_tf_read)(struct ata_port *, struct ata_taskfile *);
    void (*sff_exec_command)(struct ata_port *, const struct ata_taskfile *);
    unsigned int (*sff_data_xfer)(struct ata_queued_cmd *, unsigned char *, unsigned int, int);
    void (*sff_irq_on)(struct ata_port *);
    bool (*sff_irq_check)(struct ata_port *);
    void (*sff_irq_clear)(struct ata_port *);
    void (*sff_drain_fifo)(struct ata_queued_cmd *);
    void (*bmdma_setup)(struct ata_queued_cmd *);
    void (*bmdma_start)(struct ata_queued_cmd *);
    void (*bmdma_stop)(struct ata_queued_cmd *);
    u8 (*bmdma_status)(struct ata_port *);
    ssize_t (*em_show)(struct ata_port *, char *);
    ssize_t (*em_store)(struct ata_port *, const char *, size_t);
    ssize_t (*sw_activity_show)(struct ata_device *, char *);
    ssize_t (*sw_activity_store)(struct ata_device *, enum sw_activity);
    ssize_t (*transmit_led_message)(struct ata_port *, u32, ssize_t);
    void (*phy_reset)(struct ata_port *);
    void (*eng_timeout)(struct ata_port *);
    const struct ata_port_operations *inherits;
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
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>unsigned int (*sff_data_xfer)(struct ata_device *, unsigned char *, unsigned int, int)</code> ➡️ <code>unsigned int (*sff_data_xfer)(struct ata_queued_cmd *, unsigned char *, unsigned int, int)</code>
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
<b>Field type changed. </b>
<code>void (*qc_prep)(struct ata_queued_cmd *)</code> ➡️ <code>enum ata_completion_errors (*qc_prep)(struct ata_queued_cmd *)</code>
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
<b>Field type changed. </b>
<code>unsigned int (*read_id)(struct ata_device *, struct ata_taskfile *, u16 *)</code> ➡️ <code>unsigned int (*read_id)(struct ata_device *, struct ata_taskfile *, __le16 *)</code>
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
<code>long unsigned int (*mode_filter)(struct ata_device *, long unsigned int)</code> ➡️ <code>unsigned int (*mode_filter)(struct ata_device *, unsigned int)</code>
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
<code>void (*qc_ncq_fill_rtf)(struct ata_port *, u64)</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool (*qc_fill_rtf)(struct ata_queued_cmd *)</code> ➡️ <code>void (*qc_fill_rtf)(struct ata_queued_cmd *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>void (*phy_reset)(struct ata_port *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*eng_timeout)(struct ata_port *)</code>
</li>
</ul>
</details>
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
