# Struct: <code>spi_master</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct spi_master {
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
    spinlock_t bus_lock_spinlock;
    struct mutex bus_lock_mutex;
    bool bus_lock_flag;
    int (*setup)(struct spi_device *);
    int (*transfer)(struct spi_device *, struct spi_message *);
    void (*cleanup)(struct spi_device *);
    bool (*can_dma)(struct spi_master *, struct spi_device *, struct spi_transfer *);
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
    int (*prepare_transfer_hardware)(struct spi_master *);
    int (*transfer_one_message)(struct spi_master *, struct spi_message *);
    int (*unprepare_transfer_hardware)(struct spi_master *);
    int (*prepare_message)(struct spi_master *, struct spi_message *);
    int (*unprepare_message)(struct spi_master *, struct spi_message *);
    void (*set_cs)(struct spi_device *, bool);
    int (*transfer_one)(struct spi_master *, struct spi_device *, struct spi_transfer *);
    void (*handle_err)(struct spi_master *, struct spi_message *);
    int *cs_gpios;
    struct spi_statistics statistics;
    struct dma_chan *dma_tx;
    struct dma_chan *dma_rx;
    void *dummy_rx;
    void *dummy_tx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct spi_master {
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
    size_t (*max_transfer_size)(struct spi_device *);
    struct mutex io_mutex;
    spinlock_t bus_lock_spinlock;
    struct mutex bus_lock_mutex;
    bool bus_lock_flag;
    int (*setup)(struct spi_device *);
    int (*transfer)(struct spi_device *, struct spi_message *);
    void (*cleanup)(struct spi_device *);
    bool (*can_dma)(struct spi_master *, struct spi_device *, struct spi_transfer *);
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
    int (*prepare_transfer_hardware)(struct spi_master *);
    int (*transfer_one_message)(struct spi_master *, struct spi_message *);
    int (*unprepare_transfer_hardware)(struct spi_master *);
    int (*prepare_message)(struct spi_master *, struct spi_message *);
    int (*unprepare_message)(struct spi_master *, struct spi_message *);
    int (*spi_flash_read)(struct spi_device *, struct spi_flash_read_message *);
    bool (*flash_read_supported)(struct spi_device *);
    void (*set_cs)(struct spi_device *, bool);
    int (*transfer_one)(struct spi_master *, struct spi_device *, struct spi_transfer *);
    void (*handle_err)(struct spi_master *, struct spi_message *);
    int *cs_gpios;
    struct spi_statistics statistics;
    struct dma_chan *dma_tx;
    struct dma_chan *dma_rx;
    void *dummy_rx;
    void *dummy_tx;
    int (*fw_translate_cs)(struct spi_master *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct spi_master {
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
    size_t (*max_transfer_size)(struct spi_device *);
    size_t (*max_message_size)(struct spi_device *);
    struct mutex io_mutex;
    spinlock_t bus_lock_spinlock;
    struct mutex bus_lock_mutex;
    bool bus_lock_flag;
    int (*setup)(struct spi_device *);
    int (*transfer)(struct spi_device *, struct spi_message *);
    void (*cleanup)(struct spi_device *);
    bool (*can_dma)(struct spi_master *, struct spi_device *, struct spi_transfer *);
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
    int (*prepare_transfer_hardware)(struct spi_master *);
    int (*transfer_one_message)(struct spi_master *, struct spi_message *);
    int (*unprepare_transfer_hardware)(struct spi_master *);
    int (*prepare_message)(struct spi_master *, struct spi_message *);
    int (*unprepare_message)(struct spi_master *, struct spi_message *);
    int (*spi_flash_read)(struct spi_device *, struct spi_flash_read_message *);
    bool (*flash_read_supported)(struct spi_device *);
    void (*set_cs)(struct spi_device *, bool);
    int (*transfer_one)(struct spi_master *, struct spi_device *, struct spi_transfer *);
    void (*handle_err)(struct spi_master *, struct spi_message *);
    int *cs_gpios;
    struct spi_statistics statistics;
    struct dma_chan *dma_tx;
    struct dma_chan *dma_rx;
    void *dummy_rx;
    void *dummy_tx;
    int (*fw_translate_cs)(struct spi_master *, unsigned int);
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
<code>size_t (*max_transfer_size)(struct spi_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>struct mutex io_mutex</code>
</li>
<li>
<b>Field added. </b>
<code>int (*spi_flash_read)(struct spi_device *, struct spi_flash_read_message *)</code>
</li>
<li>
<b>Field added. </b>
<code>bool (*flash_read_supported)(struct spi_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*fw_translate_cs)(struct spi_master *, unsigned int)</code>
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
<code>size_t (*max_message_size)(struct spi_device *)</code>
</li>
</ul>
</details>
</li>
</ul>
