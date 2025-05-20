# Struct: <code>spi_controller</code>

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
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct spi_controller {
    struct device dev;
    struct list_head list;
    s16 bus_num;
    u16 num_chipselect;
    u16 dma_alignment;
    u16 mode_bits;
    u32 bits_per_word_mask;
    u32 min_speed_hz;
    u32 max_speed_hz;
    u16 flags;
    bool slave;
    size_t (*max_transfer_size)(struct spi_device *);
    size_t (*max_message_size)(struct spi_device *);
    struct mutex io_mutex;
    spinlock_t bus_lock_spinlock;
    struct mutex bus_lock_mutex;
    bool bus_lock_flag;
    int (*setup)(struct spi_device *);
    int (*transfer)(struct spi_device *, struct spi_message *);
    void (*cleanup)(struct spi_device *);
    bool (*can_dma)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    bool queued;
    struct kthread_worker kworker;
    struct task_struct *kworker_task;
    struct kthread_work pump_messages;
    spinlock_t queue_lock;
    struct list_head queue;
    struct spi_message *cur_msg;
    bool idling;
    bool busy;
    bool running;
    bool rt;
    bool auto_runtime_pm;
    bool cur_msg_prepared;
    bool cur_msg_mapped;
    struct completion xfer_completion;
    size_t max_dma_len;
    int (*prepare_transfer_hardware)(struct spi_controller *);
    int (*transfer_one_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_transfer_hardware)(struct spi_controller *);
    int (*prepare_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_message)(struct spi_controller *, struct spi_message *);
    int (*slave_abort)(struct spi_controller *);
    int (*spi_flash_read)(struct spi_device *, struct spi_flash_read_message *);
    bool (*spi_flash_can_dma)(struct spi_device *, struct spi_flash_read_message *);
    bool (*flash_read_supported)(struct spi_device *);
    void (*set_cs)(struct spi_device *, bool);
    int (*transfer_one)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    void (*handle_err)(struct spi_controller *, struct spi_message *);
    int *cs_gpios;
    struct spi_statistics statistics;
    struct dma_chan *dma_tx;
    struct dma_chan *dma_rx;
    void *dummy_rx;
    void *dummy_tx;
    int (*fw_translate_cs)(struct spi_controller *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct spi_controller {
    struct device dev;
    struct list_head list;
    s16 bus_num;
    u16 num_chipselect;
    u16 dma_alignment;
    u16 mode_bits;
    u32 bits_per_word_mask;
    u32 min_speed_hz;
    u32 max_speed_hz;
    u16 flags;
    bool slave;
    size_t (*max_transfer_size)(struct spi_device *);
    size_t (*max_message_size)(struct spi_device *);
    struct mutex io_mutex;
    spinlock_t bus_lock_spinlock;
    struct mutex bus_lock_mutex;
    bool bus_lock_flag;
    int (*setup)(struct spi_device *);
    int (*transfer)(struct spi_device *, struct spi_message *);
    void (*cleanup)(struct spi_device *);
    bool (*can_dma)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    bool queued;
    struct kthread_worker kworker;
    struct task_struct *kworker_task;
    struct kthread_work pump_messages;
    spinlock_t queue_lock;
    struct list_head queue;
    struct spi_message *cur_msg;
    bool idling;
    bool busy;
    bool running;
    bool rt;
    bool auto_runtime_pm;
    bool cur_msg_prepared;
    bool cur_msg_mapped;
    struct completion xfer_completion;
    size_t max_dma_len;
    int (*prepare_transfer_hardware)(struct spi_controller *);
    int (*transfer_one_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_transfer_hardware)(struct spi_controller *);
    int (*prepare_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_message)(struct spi_controller *, struct spi_message *);
    int (*slave_abort)(struct spi_controller *);
    int (*spi_flash_read)(struct spi_device *, struct spi_flash_read_message *);
    bool (*spi_flash_can_dma)(struct spi_device *, struct spi_flash_read_message *);
    bool (*flash_read_supported)(struct spi_device *);
    void (*set_cs)(struct spi_device *, bool);
    int (*transfer_one)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    void (*handle_err)(struct spi_controller *, struct spi_message *);
    int *cs_gpios;
    struct spi_statistics statistics;
    struct dma_chan *dma_tx;
    struct dma_chan *dma_rx;
    void *dummy_rx;
    void *dummy_tx;
    int (*fw_translate_cs)(struct spi_controller *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct spi_controller {
    struct device dev;
    struct list_head list;
    s16 bus_num;
    u16 num_chipselect;
    u16 dma_alignment;
    u16 mode_bits;
    u32 bits_per_word_mask;
    u32 min_speed_hz;
    u32 max_speed_hz;
    u16 flags;
    bool slave;
    size_t (*max_transfer_size)(struct spi_device *);
    size_t (*max_message_size)(struct spi_device *);
    struct mutex io_mutex;
    spinlock_t bus_lock_spinlock;
    struct mutex bus_lock_mutex;
    bool bus_lock_flag;
    int (*setup)(struct spi_device *);
    int (*transfer)(struct spi_device *, struct spi_message *);
    void (*cleanup)(struct spi_device *);
    bool (*can_dma)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    bool queued;
    struct kthread_worker kworker;
    struct task_struct *kworker_task;
    struct kthread_work pump_messages;
    spinlock_t queue_lock;
    struct list_head queue;
    struct spi_message *cur_msg;
    bool idling;
    bool busy;
    bool running;
    bool rt;
    bool auto_runtime_pm;
    bool cur_msg_prepared;
    bool cur_msg_mapped;
    struct completion xfer_completion;
    size_t max_dma_len;
    int (*prepare_transfer_hardware)(struct spi_controller *);
    int (*transfer_one_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_transfer_hardware)(struct spi_controller *);
    int (*prepare_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_message)(struct spi_controller *, struct spi_message *);
    int (*slave_abort)(struct spi_controller *);
    void (*set_cs)(struct spi_device *, bool);
    int (*transfer_one)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    void (*handle_err)(struct spi_controller *, struct spi_message *);
    const struct spi_controller_mem_ops *mem_ops;
    int *cs_gpios;
    struct spi_statistics statistics;
    struct dma_chan *dma_tx;
    struct dma_chan *dma_rx;
    void *dummy_rx;
    void *dummy_tx;
    int (*fw_translate_cs)(struct spi_controller *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct spi_controller {
    struct device dev;
    struct list_head list;
    s16 bus_num;
    u16 num_chipselect;
    u16 dma_alignment;
    u16 mode_bits;
    u32 bits_per_word_mask;
    u32 min_speed_hz;
    u32 max_speed_hz;
    u16 flags;
    bool slave;
    size_t (*max_transfer_size)(struct spi_device *);
    size_t (*max_message_size)(struct spi_device *);
    struct mutex io_mutex;
    spinlock_t bus_lock_spinlock;
    struct mutex bus_lock_mutex;
    bool bus_lock_flag;
    int (*setup)(struct spi_device *);
    int (*transfer)(struct spi_device *, struct spi_message *);
    void (*cleanup)(struct spi_device *);
    bool (*can_dma)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    bool queued;
    struct kthread_worker kworker;
    struct task_struct *kworker_task;
    struct kthread_work pump_messages;
    spinlock_t queue_lock;
    struct list_head queue;
    struct spi_message *cur_msg;
    bool idling;
    bool busy;
    bool running;
    bool rt;
    bool auto_runtime_pm;
    bool cur_msg_prepared;
    bool cur_msg_mapped;
    struct completion xfer_completion;
    size_t max_dma_len;
    int (*prepare_transfer_hardware)(struct spi_controller *);
    int (*transfer_one_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_transfer_hardware)(struct spi_controller *);
    int (*prepare_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_message)(struct spi_controller *, struct spi_message *);
    int (*slave_abort)(struct spi_controller *);
    void (*set_cs)(struct spi_device *, bool);
    int (*transfer_one)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    void (*handle_err)(struct spi_controller *, struct spi_message *);
    const struct spi_controller_mem_ops *mem_ops;
    int *cs_gpios;
    struct spi_statistics statistics;
    struct dma_chan *dma_tx;
    struct dma_chan *dma_rx;
    void *dummy_rx;
    void *dummy_tx;
    int (*fw_translate_cs)(struct spi_controller *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct spi_controller {
    struct device dev;
    struct list_head list;
    s16 bus_num;
    u16 num_chipselect;
    u16 dma_alignment;
    u32 mode_bits;
    u32 bits_per_word_mask;
    u32 min_speed_hz;
    u32 max_speed_hz;
    u16 flags;
    bool slave;
    size_t (*max_transfer_size)(struct spi_device *);
    size_t (*max_message_size)(struct spi_device *);
    struct mutex io_mutex;
    spinlock_t bus_lock_spinlock;
    struct mutex bus_lock_mutex;
    bool bus_lock_flag;
    int (*setup)(struct spi_device *);
    void (*set_cs_timing)(struct spi_device *, u8, u8, u8);
    int (*transfer)(struct spi_device *, struct spi_message *);
    void (*cleanup)(struct spi_device *);
    bool (*can_dma)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    bool queued;
    struct kthread_worker kworker;
    struct task_struct *kworker_task;
    struct kthread_work pump_messages;
    spinlock_t queue_lock;
    struct list_head queue;
    struct spi_message *cur_msg;
    bool idling;
    bool busy;
    bool running;
    bool rt;
    bool auto_runtime_pm;
    bool cur_msg_prepared;
    bool cur_msg_mapped;
    struct completion xfer_completion;
    size_t max_dma_len;
    int (*prepare_transfer_hardware)(struct spi_controller *);
    int (*transfer_one_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_transfer_hardware)(struct spi_controller *);
    int (*prepare_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_message)(struct spi_controller *, struct spi_message *);
    int (*slave_abort)(struct spi_controller *);
    void (*set_cs)(struct spi_device *, bool);
    int (*transfer_one)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    void (*handle_err)(struct spi_controller *, struct spi_message *);
    const struct spi_controller_mem_ops *mem_ops;
    int *cs_gpios;
    struct gpio_desc **cs_gpiods;
    bool use_gpio_descriptors;
    struct spi_statistics statistics;
    struct dma_chan *dma_tx;
    struct dma_chan *dma_rx;
    void *dummy_rx;
    void *dummy_tx;
    int (*fw_translate_cs)(struct spi_controller *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct spi_controller {
    struct device dev;
    struct list_head list;
    s16 bus_num;
    u16 num_chipselect;
    u16 dma_alignment;
    u32 mode_bits;
    u32 buswidth_override_bits;
    u32 bits_per_word_mask;
    u32 min_speed_hz;
    u32 max_speed_hz;
    u16 flags;
    bool slave;
    size_t (*max_transfer_size)(struct spi_device *);
    size_t (*max_message_size)(struct spi_device *);
    struct mutex io_mutex;
    spinlock_t bus_lock_spinlock;
    struct mutex bus_lock_mutex;
    bool bus_lock_flag;
    int (*setup)(struct spi_device *);
    void (*set_cs_timing)(struct spi_device *, u8, u8, u8);
    int (*transfer)(struct spi_device *, struct spi_message *);
    void (*cleanup)(struct spi_device *);
    bool (*can_dma)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    bool queued;
    struct kthread_worker kworker;
    struct task_struct *kworker_task;
    struct kthread_work pump_messages;
    spinlock_t queue_lock;
    struct list_head queue;
    struct spi_message *cur_msg;
    bool idling;
    bool busy;
    bool running;
    bool rt;
    bool auto_runtime_pm;
    bool cur_msg_prepared;
    bool cur_msg_mapped;
    struct completion xfer_completion;
    size_t max_dma_len;
    int (*prepare_transfer_hardware)(struct spi_controller *);
    int (*transfer_one_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_transfer_hardware)(struct spi_controller *);
    int (*prepare_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_message)(struct spi_controller *, struct spi_message *);
    int (*slave_abort)(struct spi_controller *);
    void (*set_cs)(struct spi_device *, bool);
    int (*transfer_one)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    void (*handle_err)(struct spi_controller *, struct spi_message *);
    const struct spi_controller_mem_ops *mem_ops;
    int *cs_gpios;
    struct gpio_desc **cs_gpiods;
    bool use_gpio_descriptors;
    struct spi_statistics statistics;
    struct dma_chan *dma_tx;
    struct dma_chan *dma_rx;
    void *dummy_rx;
    void *dummy_tx;
    int (*fw_translate_cs)(struct spi_controller *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct spi_controller {
    struct device dev;
    struct list_head list;
    s16 bus_num;
    u16 num_chipselect;
    u16 dma_alignment;
    u32 mode_bits;
    u32 buswidth_override_bits;
    u32 bits_per_word_mask;
    u32 min_speed_hz;
    u32 max_speed_hz;
    u16 flags;
    bool slave;
    size_t (*max_transfer_size)(struct spi_device *);
    size_t (*max_message_size)(struct spi_device *);
    struct mutex io_mutex;
    spinlock_t bus_lock_spinlock;
    struct mutex bus_lock_mutex;
    bool bus_lock_flag;
    int (*setup)(struct spi_device *);
    int (*set_cs_timing)(struct spi_device *, struct spi_delay *, struct spi_delay *, struct spi_delay *);
    int (*transfer)(struct spi_device *, struct spi_message *);
    void (*cleanup)(struct spi_device *);
    bool (*can_dma)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    bool queued;
    struct kthread_worker kworker;
    struct task_struct *kworker_task;
    struct kthread_work pump_messages;
    spinlock_t queue_lock;
    struct list_head queue;
    struct spi_message *cur_msg;
    bool idling;
    bool busy;
    bool running;
    bool rt;
    bool auto_runtime_pm;
    bool cur_msg_prepared;
    bool cur_msg_mapped;
    struct completion xfer_completion;
    size_t max_dma_len;
    int (*prepare_transfer_hardware)(struct spi_controller *);
    int (*transfer_one_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_transfer_hardware)(struct spi_controller *);
    int (*prepare_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_message)(struct spi_controller *, struct spi_message *);
    int (*slave_abort)(struct spi_controller *);
    void (*set_cs)(struct spi_device *, bool);
    int (*transfer_one)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    void (*handle_err)(struct spi_controller *, struct spi_message *);
    const struct spi_controller_mem_ops *mem_ops;
    struct spi_delay cs_setup;
    struct spi_delay cs_hold;
    struct spi_delay cs_inactive;
    int *cs_gpios;
    struct gpio_desc **cs_gpiods;
    bool use_gpio_descriptors;
    u8 unused_native_cs;
    u8 max_native_cs;
    struct spi_statistics statistics;
    struct dma_chan *dma_tx;
    struct dma_chan *dma_rx;
    void *dummy_rx;
    void *dummy_tx;
    int (*fw_translate_cs)(struct spi_controller *, unsigned int);
    bool ptp_sts_supported;
    long unsigned int irq_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct spi_controller {
    struct device dev;
    struct list_head list;
    s16 bus_num;
    u16 num_chipselect;
    u16 dma_alignment;
    u32 mode_bits;
    u32 buswidth_override_bits;
    u32 bits_per_word_mask;
    u32 min_speed_hz;
    u32 max_speed_hz;
    u16 flags;
    bool slave;
    size_t (*max_transfer_size)(struct spi_device *);
    size_t (*max_message_size)(struct spi_device *);
    struct mutex io_mutex;
    spinlock_t bus_lock_spinlock;
    struct mutex bus_lock_mutex;
    bool bus_lock_flag;
    int (*setup)(struct spi_device *);
    int (*set_cs_timing)(struct spi_device *, struct spi_delay *, struct spi_delay *, struct spi_delay *);
    int (*transfer)(struct spi_device *, struct spi_message *);
    void (*cleanup)(struct spi_device *);
    bool (*can_dma)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    bool queued;
    struct kthread_worker *kworker;
    struct kthread_work pump_messages;
    spinlock_t queue_lock;
    struct list_head queue;
    struct spi_message *cur_msg;
    bool idling;
    bool busy;
    bool running;
    bool rt;
    bool auto_runtime_pm;
    bool cur_msg_prepared;
    bool cur_msg_mapped;
    bool last_cs_enable;
    bool last_cs_mode_high;
    bool fallback;
    struct completion xfer_completion;
    size_t max_dma_len;
    int (*prepare_transfer_hardware)(struct spi_controller *);
    int (*transfer_one_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_transfer_hardware)(struct spi_controller *);
    int (*prepare_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_message)(struct spi_controller *, struct spi_message *);
    int (*slave_abort)(struct spi_controller *);
    void (*set_cs)(struct spi_device *, bool);
    int (*transfer_one)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    void (*handle_err)(struct spi_controller *, struct spi_message *);
    const struct spi_controller_mem_ops *mem_ops;
    struct spi_delay cs_setup;
    struct spi_delay cs_hold;
    struct spi_delay cs_inactive;
    int *cs_gpios;
    struct gpio_desc **cs_gpiods;
    bool use_gpio_descriptors;
    u8 unused_native_cs;
    u8 max_native_cs;
    struct spi_statistics statistics;
    struct dma_chan *dma_tx;
    struct dma_chan *dma_rx;
    void *dummy_rx;
    void *dummy_tx;
    int (*fw_translate_cs)(struct spi_controller *, unsigned int);
    bool ptp_sts_supported;
    long unsigned int irq_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct spi_controller {
    struct device dev;
    struct list_head list;
    s16 bus_num;
    u16 num_chipselect;
    u16 dma_alignment;
    u32 mode_bits;
    u32 buswidth_override_bits;
    u32 bits_per_word_mask;
    u32 min_speed_hz;
    u32 max_speed_hz;
    u16 flags;
    bool devm_allocated;
    bool slave;
    size_t (*max_transfer_size)(struct spi_device *);
    size_t (*max_message_size)(struct spi_device *);
    struct mutex io_mutex;
    spinlock_t bus_lock_spinlock;
    struct mutex bus_lock_mutex;
    bool bus_lock_flag;
    int (*setup)(struct spi_device *);
    int (*set_cs_timing)(struct spi_device *, struct spi_delay *, struct spi_delay *, struct spi_delay *);
    int (*transfer)(struct spi_device *, struct spi_message *);
    void (*cleanup)(struct spi_device *);
    bool (*can_dma)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    bool queued;
    struct kthread_worker *kworker;
    struct kthread_work pump_messages;
    spinlock_t queue_lock;
    struct list_head queue;
    struct spi_message *cur_msg;
    bool idling;
    bool busy;
    bool running;
    bool rt;
    bool auto_runtime_pm;
    bool cur_msg_prepared;
    bool cur_msg_mapped;
    bool last_cs_enable;
    bool last_cs_mode_high;
    bool fallback;
    struct completion xfer_completion;
    size_t max_dma_len;
    int (*prepare_transfer_hardware)(struct spi_controller *);
    int (*transfer_one_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_transfer_hardware)(struct spi_controller *);
    int (*prepare_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_message)(struct spi_controller *, struct spi_message *);
    int (*slave_abort)(struct spi_controller *);
    void (*set_cs)(struct spi_device *, bool);
    int (*transfer_one)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    void (*handle_err)(struct spi_controller *, struct spi_message *);
    const struct spi_controller_mem_ops *mem_ops;
    struct spi_delay cs_setup;
    struct spi_delay cs_hold;
    struct spi_delay cs_inactive;
    int *cs_gpios;
    struct gpio_desc **cs_gpiods;
    bool use_gpio_descriptors;
    s8 unused_native_cs;
    s8 max_native_cs;
    struct spi_statistics statistics;
    struct dma_chan *dma_tx;
    struct dma_chan *dma_rx;
    void *dummy_rx;
    void *dummy_tx;
    int (*fw_translate_cs)(struct spi_controller *, unsigned int);
    bool ptp_sts_supported;
    long unsigned int irq_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct spi_controller {
    struct device dev;
    struct list_head list;
    s16 bus_num;
    u16 num_chipselect;
    u16 dma_alignment;
    u32 mode_bits;
    u32 buswidth_override_bits;
    u32 bits_per_word_mask;
    u32 min_speed_hz;
    u32 max_speed_hz;
    u16 flags;
    bool devm_allocated;
    bool slave;
    size_t (*max_transfer_size)(struct spi_device *);
    size_t (*max_message_size)(struct spi_device *);
    struct mutex io_mutex;
    struct mutex add_lock;
    spinlock_t bus_lock_spinlock;
    struct mutex bus_lock_mutex;
    bool bus_lock_flag;
    int (*setup)(struct spi_device *);
    int (*set_cs_timing)(struct spi_device *);
    int (*transfer)(struct spi_device *, struct spi_message *);
    void (*cleanup)(struct spi_device *);
    bool (*can_dma)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    struct device *dma_map_dev;
    bool queued;
    struct kthread_worker *kworker;
    struct kthread_work pump_messages;
    spinlock_t queue_lock;
    struct list_head queue;
    struct spi_message *cur_msg;
    bool idling;
    bool busy;
    bool running;
    bool rt;
    bool auto_runtime_pm;
    bool cur_msg_prepared;
    bool cur_msg_mapped;
    bool last_cs_enable;
    bool last_cs_mode_high;
    bool fallback;
    struct completion xfer_completion;
    size_t max_dma_len;
    int (*prepare_transfer_hardware)(struct spi_controller *);
    int (*transfer_one_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_transfer_hardware)(struct spi_controller *);
    int (*prepare_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_message)(struct spi_controller *, struct spi_message *);
    int (*slave_abort)(struct spi_controller *);
    void (*set_cs)(struct spi_device *, bool);
    int (*transfer_one)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    void (*handle_err)(struct spi_controller *, struct spi_message *);
    const struct spi_controller_mem_ops *mem_ops;
    int *cs_gpios;
    struct gpio_desc **cs_gpiods;
    bool use_gpio_descriptors;
    s8 unused_native_cs;
    s8 max_native_cs;
    struct spi_statistics statistics;
    struct dma_chan *dma_tx;
    struct dma_chan *dma_rx;
    void *dummy_rx;
    void *dummy_tx;
    int (*fw_translate_cs)(struct spi_controller *, unsigned int);
    bool ptp_sts_supported;
    long unsigned int irq_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct spi_controller {
    struct device dev;
    struct list_head list;
    s16 bus_num;
    u16 num_chipselect;
    u16 dma_alignment;
    u32 mode_bits;
    u32 buswidth_override_bits;
    u32 bits_per_word_mask;
    u32 min_speed_hz;
    u32 max_speed_hz;
    u16 flags;
    bool devm_allocated;
    bool slave;
    size_t (*max_transfer_size)(struct spi_device *);
    size_t (*max_message_size)(struct spi_device *);
    struct mutex io_mutex;
    struct mutex add_lock;
    spinlock_t bus_lock_spinlock;
    struct mutex bus_lock_mutex;
    bool bus_lock_flag;
    int (*setup)(struct spi_device *);
    int (*set_cs_timing)(struct spi_device *);
    int (*transfer)(struct spi_device *, struct spi_message *);
    void (*cleanup)(struct spi_device *);
    bool (*can_dma)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    struct device *dma_map_dev;
    bool queued;
    struct kthread_worker *kworker;
    struct kthread_work pump_messages;
    spinlock_t queue_lock;
    struct list_head queue;
    struct spi_message *cur_msg;
    bool idling;
    bool busy;
    bool running;
    bool rt;
    bool auto_runtime_pm;
    bool cur_msg_prepared;
    bool cur_msg_mapped;
    char last_cs;
    bool last_cs_mode_high;
    bool fallback;
    struct completion xfer_completion;
    size_t max_dma_len;
    int (*prepare_transfer_hardware)(struct spi_controller *);
    int (*transfer_one_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_transfer_hardware)(struct spi_controller *);
    int (*prepare_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_message)(struct spi_controller *, struct spi_message *);
    int (*slave_abort)(struct spi_controller *);
    void (*set_cs)(struct spi_device *, bool);
    int (*transfer_one)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    void (*handle_err)(struct spi_controller *, struct spi_message *);
    const struct spi_controller_mem_ops *mem_ops;
    const struct spi_controller_mem_caps *mem_caps;
    struct gpio_desc **cs_gpiods;
    bool use_gpio_descriptors;
    s8 unused_native_cs;
    s8 max_native_cs;
    struct spi_statistics statistics;
    struct dma_chan *dma_tx;
    struct dma_chan *dma_rx;
    void *dummy_rx;
    void *dummy_tx;
    int (*fw_translate_cs)(struct spi_controller *, unsigned int);
    bool ptp_sts_supported;
    long unsigned int irq_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct spi_controller {
    struct device dev;
    struct list_head list;
    s16 bus_num;
    u16 num_chipselect;
    u16 dma_alignment;
    u32 mode_bits;
    u32 buswidth_override_bits;
    u32 bits_per_word_mask;
    u32 min_speed_hz;
    u32 max_speed_hz;
    u16 flags;
    bool devm_allocated;
    bool slave;
    bool target;
    size_t (*max_transfer_size)(struct spi_device *);
    size_t (*max_message_size)(struct spi_device *);
    struct mutex io_mutex;
    struct mutex add_lock;
    spinlock_t bus_lock_spinlock;
    struct mutex bus_lock_mutex;
    bool bus_lock_flag;
    int (*setup)(struct spi_device *);
    int (*set_cs_timing)(struct spi_device *);
    int (*transfer)(struct spi_device *, struct spi_message *);
    void (*cleanup)(struct spi_device *);
    bool (*can_dma)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    struct device *dma_map_dev;
    struct device *cur_rx_dma_dev;
    struct device *cur_tx_dma_dev;
    bool queued;
    struct kthread_worker *kworker;
    struct kthread_work pump_messages;
    spinlock_t queue_lock;
    struct list_head queue;
    struct spi_message *cur_msg;
    struct completion cur_msg_completion;
    bool cur_msg_incomplete;
    bool cur_msg_need_completion;
    bool busy;
    bool running;
    bool rt;
    bool auto_runtime_pm;
    bool cur_msg_mapped;
    char last_cs;
    bool last_cs_mode_high;
    bool fallback;
    struct completion xfer_completion;
    size_t max_dma_len;
    int (*prepare_transfer_hardware)(struct spi_controller *);
    int (*transfer_one_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_transfer_hardware)(struct spi_controller *);
    int (*prepare_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_message)(struct spi_controller *, struct spi_message *);
    int (*slave_abort)(struct spi_controller *);
    int (*target_abort)(struct spi_controller *);
    void (*set_cs)(struct spi_device *, bool);
    int (*transfer_one)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    void (*handle_err)(struct spi_controller *, struct spi_message *);
    const struct spi_controller_mem_ops *mem_ops;
    const struct spi_controller_mem_caps *mem_caps;
    struct gpio_desc **cs_gpiods;
    bool use_gpio_descriptors;
    s8 unused_native_cs;
    s8 max_native_cs;
    struct spi_statistics *pcpu_statistics;
    struct dma_chan *dma_tx;
    struct dma_chan *dma_rx;
    void *dummy_rx;
    void *dummy_tx;
    int (*fw_translate_cs)(struct spi_controller *, unsigned int);
    bool ptp_sts_supported;
    long unsigned int irq_flags;
    bool queue_empty;
    bool must_async;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct spi_controller {
    struct device dev;
    struct list_head list;
    s16 bus_num;
    u16 num_chipselect;
    u16 dma_alignment;
    u32 mode_bits;
    u32 buswidth_override_bits;
    u32 bits_per_word_mask;
    u32 min_speed_hz;
    u32 max_speed_hz;
    u16 flags;
    bool devm_allocated;
    bool slave;
    bool target;
    size_t (*max_transfer_size)(struct spi_device *);
    size_t (*max_message_size)(struct spi_device *);
    struct mutex io_mutex;
    struct mutex add_lock;
    spinlock_t bus_lock_spinlock;
    struct mutex bus_lock_mutex;
    bool bus_lock_flag;
    int (*setup)(struct spi_device *);
    int (*set_cs_timing)(struct spi_device *);
    int (*transfer)(struct spi_device *, struct spi_message *);
    void (*cleanup)(struct spi_device *);
    bool (*can_dma)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    struct device *dma_map_dev;
    struct device *cur_rx_dma_dev;
    struct device *cur_tx_dma_dev;
    bool queued;
    struct kthread_worker *kworker;
    struct kthread_work pump_messages;
    spinlock_t queue_lock;
    struct list_head queue;
    struct spi_message *cur_msg;
    struct completion cur_msg_completion;
    bool cur_msg_incomplete;
    bool cur_msg_need_completion;
    bool busy;
    bool running;
    bool rt;
    bool auto_runtime_pm;
    bool cur_msg_mapped;
    char last_cs;
    bool last_cs_mode_high;
    bool fallback;
    struct completion xfer_completion;
    size_t max_dma_len;
    int (*prepare_transfer_hardware)(struct spi_controller *);
    int (*transfer_one_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_transfer_hardware)(struct spi_controller *);
    int (*prepare_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_message)(struct spi_controller *, struct spi_message *);
    int (*slave_abort)(struct spi_controller *);
    int (*target_abort)(struct spi_controller *);
    void (*set_cs)(struct spi_device *, bool);
    int (*transfer_one)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    void (*handle_err)(struct spi_controller *, struct spi_message *);
    const struct spi_controller_mem_ops *mem_ops;
    const struct spi_controller_mem_caps *mem_caps;
    struct gpio_desc **cs_gpiods;
    bool use_gpio_descriptors;
    s8 unused_native_cs;
    s8 max_native_cs;
    struct spi_statistics *pcpu_statistics;
    struct dma_chan *dma_tx;
    struct dma_chan *dma_rx;
    void *dummy_rx;
    void *dummy_tx;
    int (*fw_translate_cs)(struct spi_controller *, unsigned int);
    bool ptp_sts_supported;
    long unsigned int irq_flags;
    bool queue_empty;
    bool must_async;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct spi_controller {
    struct device dev;
    struct list_head list;
    s16 bus_num;
    u16 num_chipselect;
    u16 dma_alignment;
    u32 mode_bits;
    u32 buswidth_override_bits;
    u32 bits_per_word_mask;
    u32 min_speed_hz;
    u32 max_speed_hz;
    u16 flags;
    bool devm_allocated;
    bool slave;
    bool target;
    size_t (*max_transfer_size)(struct spi_device *);
    size_t (*max_message_size)(struct spi_device *);
    struct mutex io_mutex;
    struct mutex add_lock;
    spinlock_t bus_lock_spinlock;
    struct mutex bus_lock_mutex;
    bool bus_lock_flag;
    int (*setup)(struct spi_device *);
    int (*set_cs_timing)(struct spi_device *);
    int (*transfer)(struct spi_device *, struct spi_message *);
    void (*cleanup)(struct spi_device *);
    bool (*can_dma)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    struct device *dma_map_dev;
    struct device *cur_rx_dma_dev;
    struct device *cur_tx_dma_dev;
    bool queued;
    struct kthread_worker *kworker;
    struct kthread_work pump_messages;
    spinlock_t queue_lock;
    struct list_head queue;
    struct spi_message *cur_msg;
    struct completion cur_msg_completion;
    bool cur_msg_incomplete;
    bool cur_msg_need_completion;
    bool busy;
    bool running;
    bool rt;
    bool auto_runtime_pm;
    bool cur_msg_mapped;
    char last_cs[16];
    char last_cs_index_mask;
    bool last_cs_mode_high;
    bool fallback;
    struct completion xfer_completion;
    size_t max_dma_len;
    int (*prepare_transfer_hardware)(struct spi_controller *);
    int (*transfer_one_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_transfer_hardware)(struct spi_controller *);
    int (*prepare_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_message)(struct spi_controller *, struct spi_message *);
    int (*slave_abort)(struct spi_controller *);
    int (*target_abort)(struct spi_controller *);
    void (*set_cs)(struct spi_device *, bool);
    int (*transfer_one)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    void (*handle_err)(struct spi_controller *, struct spi_message *);
    const struct spi_controller_mem_ops *mem_ops;
    const struct spi_controller_mem_caps *mem_caps;
    struct gpio_desc **cs_gpiods;
    bool use_gpio_descriptors;
    s8 unused_native_cs;
    s8 max_native_cs;
    struct spi_statistics *pcpu_statistics;
    struct dma_chan *dma_tx;
    struct dma_chan *dma_rx;
    void *dummy_rx;
    void *dummy_tx;
    int (*fw_translate_cs)(struct spi_controller *, unsigned int);
    bool ptp_sts_supported;
    long unsigned int irq_flags;
    bool queue_empty;
    bool must_async;
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
struct spi_controller {
    struct device dev;
    struct list_head list;
    s16 bus_num;
    u16 num_chipselect;
    u16 dma_alignment;
    u32 mode_bits;
    u32 buswidth_override_bits;
    u32 bits_per_word_mask;
    u32 min_speed_hz;
    u32 max_speed_hz;
    u16 flags;
    bool slave;
    size_t (*max_transfer_size)(struct spi_device *);
    size_t (*max_message_size)(struct spi_device *);
    struct mutex io_mutex;
    spinlock_t bus_lock_spinlock;
    struct mutex bus_lock_mutex;
    bool bus_lock_flag;
    int (*setup)(struct spi_device *);
    void (*set_cs_timing)(struct spi_device *, u8, u8, u8);
    int (*transfer)(struct spi_device *, struct spi_message *);
    void (*cleanup)(struct spi_device *);
    bool (*can_dma)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    bool queued;
    struct kthread_worker kworker;
    struct task_struct *kworker_task;
    struct kthread_work pump_messages;
    spinlock_t queue_lock;
    struct list_head queue;
    struct spi_message *cur_msg;
    bool idling;
    bool busy;
    bool running;
    bool rt;
    bool auto_runtime_pm;
    bool cur_msg_prepared;
    bool cur_msg_mapped;
    struct completion xfer_completion;
    size_t max_dma_len;
    int (*prepare_transfer_hardware)(struct spi_controller *);
    int (*transfer_one_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_transfer_hardware)(struct spi_controller *);
    int (*prepare_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_message)(struct spi_controller *, struct spi_message *);
    int (*slave_abort)(struct spi_controller *);
    void (*set_cs)(struct spi_device *, bool);
    int (*transfer_one)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    void (*handle_err)(struct spi_controller *, struct spi_message *);
    const struct spi_controller_mem_ops *mem_ops;
    int *cs_gpios;
    struct gpio_desc **cs_gpiods;
    bool use_gpio_descriptors;
    struct spi_statistics statistics;
    struct dma_chan *dma_tx;
    struct dma_chan *dma_rx;
    void *dummy_rx;
    void *dummy_tx;
    int (*fw_translate_cs)(struct spi_controller *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct spi_controller {
    struct device dev;
    struct list_head list;
    s16 bus_num;
    u16 num_chipselect;
    u16 dma_alignment;
    u32 mode_bits;
    u32 buswidth_override_bits;
    u32 bits_per_word_mask;
    u32 min_speed_hz;
    u32 max_speed_hz;
    u16 flags;
    bool slave;
    size_t (*max_transfer_size)(struct spi_device *);
    size_t (*max_message_size)(struct spi_device *);
    struct mutex io_mutex;
    spinlock_t bus_lock_spinlock;
    struct mutex bus_lock_mutex;
    bool bus_lock_flag;
    int (*setup)(struct spi_device *);
    void (*set_cs_timing)(struct spi_device *, u8, u8, u8);
    int (*transfer)(struct spi_device *, struct spi_message *);
    void (*cleanup)(struct spi_device *);
    bool (*can_dma)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    bool queued;
    struct kthread_worker kworker;
    struct task_struct *kworker_task;
    struct kthread_work pump_messages;
    spinlock_t queue_lock;
    struct list_head queue;
    struct spi_message *cur_msg;
    bool idling;
    bool busy;
    bool running;
    bool rt;
    bool auto_runtime_pm;
    bool cur_msg_prepared;
    bool cur_msg_mapped;
    struct completion xfer_completion;
    size_t max_dma_len;
    int (*prepare_transfer_hardware)(struct spi_controller *);
    int (*transfer_one_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_transfer_hardware)(struct spi_controller *);
    int (*prepare_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_message)(struct spi_controller *, struct spi_message *);
    int (*slave_abort)(struct spi_controller *);
    void (*set_cs)(struct spi_device *, bool);
    int (*transfer_one)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    void (*handle_err)(struct spi_controller *, struct spi_message *);
    const struct spi_controller_mem_ops *mem_ops;
    int *cs_gpios;
    struct gpio_desc **cs_gpiods;
    bool use_gpio_descriptors;
    struct spi_statistics statistics;
    struct dma_chan *dma_tx;
    struct dma_chan *dma_rx;
    void *dummy_rx;
    void *dummy_tx;
    int (*fw_translate_cs)(struct spi_controller *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct spi_controller {
    struct device dev;
    struct list_head list;
    s16 bus_num;
    u16 num_chipselect;
    u16 dma_alignment;
    u32 mode_bits;
    u32 buswidth_override_bits;
    u32 bits_per_word_mask;
    u32 min_speed_hz;
    u32 max_speed_hz;
    u16 flags;
    bool slave;
    size_t (*max_transfer_size)(struct spi_device *);
    size_t (*max_message_size)(struct spi_device *);
    struct mutex io_mutex;
    spinlock_t bus_lock_spinlock;
    struct mutex bus_lock_mutex;
    bool bus_lock_flag;
    int (*setup)(struct spi_device *);
    void (*set_cs_timing)(struct spi_device *, u8, u8, u8);
    int (*transfer)(struct spi_device *, struct spi_message *);
    void (*cleanup)(struct spi_device *);
    bool (*can_dma)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    bool queued;
    struct kthread_worker kworker;
    struct task_struct *kworker_task;
    struct kthread_work pump_messages;
    spinlock_t queue_lock;
    struct list_head queue;
    struct spi_message *cur_msg;
    bool idling;
    bool busy;
    bool running;
    bool rt;
    bool auto_runtime_pm;
    bool cur_msg_prepared;
    bool cur_msg_mapped;
    struct completion xfer_completion;
    size_t max_dma_len;
    int (*prepare_transfer_hardware)(struct spi_controller *);
    int (*transfer_one_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_transfer_hardware)(struct spi_controller *);
    int (*prepare_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_message)(struct spi_controller *, struct spi_message *);
    int (*slave_abort)(struct spi_controller *);
    void (*set_cs)(struct spi_device *, bool);
    int (*transfer_one)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    void (*handle_err)(struct spi_controller *, struct spi_message *);
    const struct spi_controller_mem_ops *mem_ops;
    int *cs_gpios;
    struct gpio_desc **cs_gpiods;
    bool use_gpio_descriptors;
    struct spi_statistics statistics;
    struct dma_chan *dma_tx;
    struct dma_chan *dma_rx;
    void *dummy_rx;
    void *dummy_tx;
    int (*fw_translate_cs)(struct spi_controller *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct spi_controller {
    struct device dev;
    struct list_head list;
    s16 bus_num;
    u16 num_chipselect;
    u16 dma_alignment;
    u32 mode_bits;
    u32 buswidth_override_bits;
    u32 bits_per_word_mask;
    u32 min_speed_hz;
    u32 max_speed_hz;
    u16 flags;
    bool slave;
    size_t (*max_transfer_size)(struct spi_device *);
    size_t (*max_message_size)(struct spi_device *);
    struct mutex io_mutex;
    spinlock_t bus_lock_spinlock;
    struct mutex bus_lock_mutex;
    bool bus_lock_flag;
    int (*setup)(struct spi_device *);
    void (*set_cs_timing)(struct spi_device *, u8, u8, u8);
    int (*transfer)(struct spi_device *, struct spi_message *);
    void (*cleanup)(struct spi_device *);
    bool (*can_dma)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    bool queued;
    struct kthread_worker kworker;
    struct task_struct *kworker_task;
    struct kthread_work pump_messages;
    spinlock_t queue_lock;
    struct list_head queue;
    struct spi_message *cur_msg;
    bool idling;
    bool busy;
    bool running;
    bool rt;
    bool auto_runtime_pm;
    bool cur_msg_prepared;
    bool cur_msg_mapped;
    struct completion xfer_completion;
    size_t max_dma_len;
    int (*prepare_transfer_hardware)(struct spi_controller *);
    int (*transfer_one_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_transfer_hardware)(struct spi_controller *);
    int (*prepare_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_message)(struct spi_controller *, struct spi_message *);
    int (*slave_abort)(struct spi_controller *);
    void (*set_cs)(struct spi_device *, bool);
    int (*transfer_one)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    void (*handle_err)(struct spi_controller *, struct spi_message *);
    const struct spi_controller_mem_ops *mem_ops;
    int *cs_gpios;
    struct gpio_desc **cs_gpiods;
    bool use_gpio_descriptors;
    struct spi_statistics statistics;
    struct dma_chan *dma_tx;
    struct dma_chan *dma_rx;
    void *dummy_rx;
    void *dummy_tx;
    int (*fw_translate_cs)(struct spi_controller *, unsigned int);
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
struct spi_controller {
    struct device dev;
    struct list_head list;
    s16 bus_num;
    u16 num_chipselect;
    u16 dma_alignment;
    u32 mode_bits;
    u32 buswidth_override_bits;
    u32 bits_per_word_mask;
    u32 min_speed_hz;
    u32 max_speed_hz;
    u16 flags;
    bool slave;
    size_t (*max_transfer_size)(struct spi_device *);
    size_t (*max_message_size)(struct spi_device *);
    struct mutex io_mutex;
    spinlock_t bus_lock_spinlock;
    struct mutex bus_lock_mutex;
    bool bus_lock_flag;
    int (*setup)(struct spi_device *);
    void (*set_cs_timing)(struct spi_device *, u8, u8, u8);
    int (*transfer)(struct spi_device *, struct spi_message *);
    void (*cleanup)(struct spi_device *);
    bool (*can_dma)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    bool queued;
    struct kthread_worker kworker;
    struct task_struct *kworker_task;
    struct kthread_work pump_messages;
    spinlock_t queue_lock;
    struct list_head queue;
    struct spi_message *cur_msg;
    bool idling;
    bool busy;
    bool running;
    bool rt;
    bool auto_runtime_pm;
    bool cur_msg_prepared;
    bool cur_msg_mapped;
    struct completion xfer_completion;
    size_t max_dma_len;
    int (*prepare_transfer_hardware)(struct spi_controller *);
    int (*transfer_one_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_transfer_hardware)(struct spi_controller *);
    int (*prepare_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_message)(struct spi_controller *, struct spi_message *);
    int (*slave_abort)(struct spi_controller *);
    void (*set_cs)(struct spi_device *, bool);
    int (*transfer_one)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    void (*handle_err)(struct spi_controller *, struct spi_message *);
    const struct spi_controller_mem_ops *mem_ops;
    int *cs_gpios;
    struct gpio_desc **cs_gpiods;
    bool use_gpio_descriptors;
    struct spi_statistics statistics;
    struct dma_chan *dma_tx;
    struct dma_chan *dma_rx;
    void *dummy_rx;
    void *dummy_tx;
    int (*fw_translate_cs)(struct spi_controller *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct spi_controller {
    struct device dev;
    struct list_head list;
    s16 bus_num;
    u16 num_chipselect;
    u16 dma_alignment;
    u32 mode_bits;
    u32 buswidth_override_bits;
    u32 bits_per_word_mask;
    u32 min_speed_hz;
    u32 max_speed_hz;
    u16 flags;
    bool slave;
    size_t (*max_transfer_size)(struct spi_device *);
    size_t (*max_message_size)(struct spi_device *);
    struct mutex io_mutex;
    spinlock_t bus_lock_spinlock;
    struct mutex bus_lock_mutex;
    bool bus_lock_flag;
    int (*setup)(struct spi_device *);
    void (*set_cs_timing)(struct spi_device *, u8, u8, u8);
    int (*transfer)(struct spi_device *, struct spi_message *);
    void (*cleanup)(struct spi_device *);
    bool (*can_dma)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    bool queued;
    struct kthread_worker kworker;
    struct task_struct *kworker_task;
    struct kthread_work pump_messages;
    spinlock_t queue_lock;
    struct list_head queue;
    struct spi_message *cur_msg;
    bool idling;
    bool busy;
    bool running;
    bool rt;
    bool auto_runtime_pm;
    bool cur_msg_prepared;
    bool cur_msg_mapped;
    struct completion xfer_completion;
    size_t max_dma_len;
    int (*prepare_transfer_hardware)(struct spi_controller *);
    int (*transfer_one_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_transfer_hardware)(struct spi_controller *);
    int (*prepare_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_message)(struct spi_controller *, struct spi_message *);
    int (*slave_abort)(struct spi_controller *);
    void (*set_cs)(struct spi_device *, bool);
    int (*transfer_one)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    void (*handle_err)(struct spi_controller *, struct spi_message *);
    const struct spi_controller_mem_ops *mem_ops;
    int *cs_gpios;
    struct gpio_desc **cs_gpiods;
    bool use_gpio_descriptors;
    struct spi_statistics statistics;
    struct dma_chan *dma_tx;
    struct dma_chan *dma_rx;
    void *dummy_rx;
    void *dummy_tx;
    int (*fw_translate_cs)(struct spi_controller *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct spi_controller {
    struct device dev;
    struct list_head list;
    s16 bus_num;
    u16 num_chipselect;
    u16 dma_alignment;
    u32 mode_bits;
    u32 buswidth_override_bits;
    u32 bits_per_word_mask;
    u32 min_speed_hz;
    u32 max_speed_hz;
    u16 flags;
    bool slave;
    size_t (*max_transfer_size)(struct spi_device *);
    size_t (*max_message_size)(struct spi_device *);
    struct mutex io_mutex;
    spinlock_t bus_lock_spinlock;
    struct mutex bus_lock_mutex;
    bool bus_lock_flag;
    int (*setup)(struct spi_device *);
    void (*set_cs_timing)(struct spi_device *, u8, u8, u8);
    int (*transfer)(struct spi_device *, struct spi_message *);
    void (*cleanup)(struct spi_device *);
    bool (*can_dma)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    bool queued;
    struct kthread_worker kworker;
    struct task_struct *kworker_task;
    struct kthread_work pump_messages;
    spinlock_t queue_lock;
    struct list_head queue;
    struct spi_message *cur_msg;
    bool idling;
    bool busy;
    bool running;
    bool rt;
    bool auto_runtime_pm;
    bool cur_msg_prepared;
    bool cur_msg_mapped;
    struct completion xfer_completion;
    size_t max_dma_len;
    int (*prepare_transfer_hardware)(struct spi_controller *);
    int (*transfer_one_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_transfer_hardware)(struct spi_controller *);
    int (*prepare_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_message)(struct spi_controller *, struct spi_message *);
    int (*slave_abort)(struct spi_controller *);
    void (*set_cs)(struct spi_device *, bool);
    int (*transfer_one)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    void (*handle_err)(struct spi_controller *, struct spi_message *);
    const struct spi_controller_mem_ops *mem_ops;
    int *cs_gpios;
    struct gpio_desc **cs_gpiods;
    bool use_gpio_descriptors;
    struct spi_statistics statistics;
    struct dma_chan *dma_tx;
    struct dma_chan *dma_rx;
    void *dummy_rx;
    void *dummy_tx;
    int (*fw_translate_cs)(struct spi_controller *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct spi_controller {
    struct device dev;
    struct list_head list;
    s16 bus_num;
    u16 num_chipselect;
    u16 dma_alignment;
    u32 mode_bits;
    u32 buswidth_override_bits;
    u32 bits_per_word_mask;
    u32 min_speed_hz;
    u32 max_speed_hz;
    u16 flags;
    bool slave;
    size_t (*max_transfer_size)(struct spi_device *);
    size_t (*max_message_size)(struct spi_device *);
    struct mutex io_mutex;
    spinlock_t bus_lock_spinlock;
    struct mutex bus_lock_mutex;
    bool bus_lock_flag;
    int (*setup)(struct spi_device *);
    void (*set_cs_timing)(struct spi_device *, u8, u8, u8);
    int (*transfer)(struct spi_device *, struct spi_message *);
    void (*cleanup)(struct spi_device *);
    bool (*can_dma)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    bool queued;
    struct kthread_worker kworker;
    struct task_struct *kworker_task;
    struct kthread_work pump_messages;
    spinlock_t queue_lock;
    struct list_head queue;
    struct spi_message *cur_msg;
    bool idling;
    bool busy;
    bool running;
    bool rt;
    bool auto_runtime_pm;
    bool cur_msg_prepared;
    bool cur_msg_mapped;
    struct completion xfer_completion;
    size_t max_dma_len;
    int (*prepare_transfer_hardware)(struct spi_controller *);
    int (*transfer_one_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_transfer_hardware)(struct spi_controller *);
    int (*prepare_message)(struct spi_controller *, struct spi_message *);
    int (*unprepare_message)(struct spi_controller *, struct spi_message *);
    int (*slave_abort)(struct spi_controller *);
    void (*set_cs)(struct spi_device *, bool);
    int (*transfer_one)(struct spi_controller *, struct spi_device *, struct spi_transfer *);
    void (*handle_err)(struct spi_controller *, struct spi_message *);
    const struct spi_controller_mem_ops *mem_ops;
    int *cs_gpios;
    struct gpio_desc **cs_gpiods;
    bool use_gpio_descriptors;
    struct spi_statistics statistics;
    struct dma_chan *dma_tx;
    struct dma_chan *dma_rx;
    void *dummy_rx;
    void *dummy_tx;
    int (*fw_translate_cs)(struct spi_controller *, unsigned int);
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const struct spi_controller_mem_ops *mem_ops</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*spi_flash_read)(struct spi_device *, struct spi_flash_read_message *)</code>
</li>
<li>
<b>Field removed. </b>
<code>bool (*spi_flash_can_dma)(struct spi_device *, struct spi_flash_read_message *)</code>
</li>
<li>
<b>Field removed. </b>
<code>bool (*flash_read_supported)(struct spi_device *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*set_cs_timing)(struct spi_device *, u8, u8, u8)</code>
</li>
<li>
<b>Field added. </b>
<code>struct gpio_desc **cs_gpiods</code>
</li>
<li>
<b>Field added. </b>
<code>bool use_gpio_descriptors</code>
</li>
<li>
<b>Field type changed. </b>
<code>u16 mode_bits</code> ➡️ <code>u32 mode_bits</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 buswidth_override_bits</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct spi_delay cs_setup</code>
</li>
<li>
<b>Field added. </b>
<code>struct spi_delay cs_hold</code>
</li>
<li>
<b>Field added. </b>
<code>struct spi_delay cs_inactive</code>
</li>
<li>
<b>Field added. </b>
<code>u8 unused_native_cs</code>
</li>
<li>
<b>Field added. </b>
<code>u8 max_native_cs</code>
</li>
<li>
<b>Field added. </b>
<code>bool ptp_sts_supported</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int irq_flags</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*set_cs_timing)(struct spi_device *, u8, u8, u8)</code> ➡️ <code>int (*set_cs_timing)(struct spi_device *, struct spi_delay *, struct spi_delay *, struct spi_delay *)</code>
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
<code>bool last_cs_enable</code>
</li>
<li>
<b>Field added. </b>
<code>bool last_cs_mode_high</code>
</li>
<li>
<b>Field added. </b>
<code>bool fallback</code>
</li>
<li>
<b>Field removed. </b>
<code>struct task_struct *kworker_task</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct kthread_worker kworker</code> ➡️ <code>struct kthread_worker *kworker</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool devm_allocated</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 unused_native_cs</code> ➡️ <code>s8 unused_native_cs</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 max_native_cs</code> ➡️ <code>s8 max_native_cs</code>
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
<code>struct mutex add_lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct device *dma_map_dev</code>
</li>
<li>
<b>Field removed. </b>
<code>struct spi_delay cs_setup</code>
</li>
<li>
<b>Field removed. </b>
<code>struct spi_delay cs_hold</code>
</li>
<li>
<b>Field removed. </b>
<code>struct spi_delay cs_inactive</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*set_cs_timing)(struct spi_device *, struct spi_delay *, struct spi_delay *, struct spi_delay *)</code> ➡️ <code>int (*set_cs_timing)(struct spi_device *)</code>
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
<code>char last_cs</code>
</li>
<li>
<b>Field added. </b>
<code>const struct spi_controller_mem_caps *mem_caps</code>
</li>
<li>
<b>Field removed. </b>
<code>bool last_cs_enable</code>
</li>
<li>
<b>Field removed. </b>
<code>int *cs_gpios</code>
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
<code>bool target</code>
</li>
<li>
<b>Field added. </b>
<code>struct device *cur_rx_dma_dev</code>
</li>
<li>
<b>Field added. </b>
<code>struct device *cur_tx_dma_dev</code>
</li>
<li>
<b>Field added. </b>
<code>struct completion cur_msg_completion</code>
</li>
<li>
<b>Field added. </b>
<code>bool cur_msg_incomplete</code>
</li>
<li>
<b>Field added. </b>
<code>bool cur_msg_need_completion</code>
</li>
<li>
<b>Field added. </b>
<code>int (*target_abort)(struct spi_controller *)</code>
</li>
<li>
<b>Field added. </b>
<code>struct spi_statistics *pcpu_statistics</code>
</li>
<li>
<b>Field added. </b>
<code>bool queue_empty</code>
</li>
<li>
<b>Field added. </b>
<code>bool must_async</code>
</li>
<li>
<b>Field removed. </b>
<code>bool idling</code>
</li>
<li>
<b>Field removed. </b>
<code>bool cur_msg_prepared</code>
</li>
<li>
<b>Field removed. </b>
<code>struct spi_statistics statistics</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>char last_cs_index_mask</code>
</li>
<li>
<b>Field type changed. </b>
<code>char last_cs</code> ➡️ <code>char last_cs[16]</code>
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
