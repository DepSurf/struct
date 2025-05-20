# Struct: <code>musb</code>

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
struct musb {
    spinlock_t lock;
    spinlock_t list_lock;
    struct musb_io io;
    const struct musb_platform_ops *ops;
    struct musb_context_registers context;
    irqreturn_t (*isr)(int, void *);
    struct delayed_work irq_work;
    struct delayed_work deassert_reset_work;
    struct delayed_work finish_resume_work;
    struct delayed_work gadget_work;
    u16 hwvers;
    u16 intrrxe;
    u16 intrtxe;
    u32 port1_status;
    long unsigned int rh_timer;
    enum musb_h_ep0_state ep0_stage;
    struct musb_hw_ep *bulk_ep;
    struct list_head control;
    struct list_head in_bulk;
    struct list_head out_bulk;
    struct list_head pending_list;
    struct timer_list otg_timer;
    struct timer_list dev_timer;
    struct notifier_block nb;
    struct dma_controller *dma_controller;
    struct device *controller;
    void *ctrl_base;
    void *mregs;
    dma_addr_t async;
    dma_addr_t sync;
    void *sync_va;
    u8 tusb_revision;
    u8 int_usb;
    u16 int_rx;
    u16 int_tx;
    struct usb_phy *xceiv;
    struct phy *phy;
    int nIrq;
    unsigned int irq_wake;
    struct musb_hw_ep endpoints[16];
    u16 vbuserr_retry;
    u16 epmask;
    u8 nr_endpoints;
    int (*board_set_power)(int);
    u8 min_power;
    enum musb_mode port_mode;
    bool session;
    long unsigned int quirk_retries;
    bool is_host;
    int a_wait_bcon;
    long unsigned int idle_timeout;
    unsigned int is_initialized;
    unsigned int is_runtime_suspended;
    unsigned int is_active;
    unsigned int is_multipoint;
    unsigned int hb_iso_rx;
    unsigned int hb_iso_tx;
    unsigned int dyn_fifo;
    unsigned int bulk_split;
    unsigned int bulk_combine;
    unsigned int is_suspended;
    unsigned int may_wakeup;
    unsigned int is_self_powered;
    unsigned int is_bus_powered;
    unsigned int set_address;
    unsigned int test_mode;
    unsigned int softconnect;
    unsigned int flush_irq_work;
    u8 address;
    u8 test_mode_nr;
    u16 ackpend;
    enum musb_g_ep0_state ep0_state;
    struct usb_gadget g;
    struct usb_gadget_driver *gadget_driver;
    struct usb_hcd *hcd;
    const struct musb_hdrc_config *config;
    int xceiv_old_state;
    struct dentry *debugfs_root;
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
