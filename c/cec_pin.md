# Struct: <code>cec_pin</code>

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
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct cec_pin {
    struct cec_adapter *adap;
    const struct cec_pin_ops *ops;
    struct task_struct *kthread;
    wait_queue_head_t kthread_waitq;
    struct hrtimer timer;
    ktime_t ts;
    unsigned int wait_usecs;
    u16 la_mask;
    bool enabled;
    bool monitor_all;
    bool rx_eom;
    bool enable_irq_failed;
    enum cec_pin_state state;
    struct cec_msg tx_msg;
    u32 tx_bit;
    bool tx_nacked;
    u32 tx_signal_free_time;
    bool tx_toggle;
    struct cec_msg rx_msg;
    u32 rx_bit;
    bool rx_toggle;
    u32 rx_start_bit_low_too_short_cnt;
    u64 rx_start_bit_low_too_short_ts;
    u32 rx_start_bit_low_too_short_delta;
    u32 rx_start_bit_too_short_cnt;
    u64 rx_start_bit_too_short_ts;
    u32 rx_start_bit_too_short_delta;
    u32 rx_start_bit_too_long_cnt;
    u32 rx_data_bit_too_short_cnt;
    u64 rx_data_bit_too_short_ts;
    u32 rx_data_bit_too_short_delta;
    u32 rx_data_bit_too_long_cnt;
    u32 rx_low_drive_cnt;
    struct cec_msg work_rx_msg;
    u8 work_tx_status;
    ktime_t work_tx_ts;
    atomic_t work_irq_change;
    atomic_t work_pin_num_events;
    unsigned int work_pin_events_wr;
    unsigned int work_pin_events_rd;
    ktime_t work_pin_ts[128];
    u8 work_pin_events[128];
    bool work_pin_events_dropped;
    u32 work_pin_events_dropped_cnt;
    ktime_t timer_ts;
    u32 timer_cnt;
    u32 timer_100ms_overruns;
    u32 timer_300ms_overruns;
    u32 timer_max_overrun;
    u32 timer_sum_overrun;
    u32 tx_custom_low_usecs;
    u32 tx_custom_high_usecs;
    bool tx_ignore_nack_until_eom;
    bool tx_custom_pulse;
    bool tx_generated_poll;
    bool tx_post_eom;
    u8 tx_extra_bytes;
    u32 tx_low_drive_cnt;
};
```
</details>
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
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cec_pin {
    struct cec_adapter *adap;
    const struct cec_pin_ops *ops;
    struct task_struct *kthread;
    wait_queue_head_t kthread_waitq;
    struct hrtimer timer;
    ktime_t ts;
    unsigned int wait_usecs;
    u16 la_mask;
    bool enabled;
    bool monitor_all;
    bool rx_eom;
    bool enable_irq_failed;
    enum cec_pin_state state;
    struct cec_msg tx_msg;
    u32 tx_bit;
    bool tx_nacked;
    u32 tx_signal_free_time;
    bool tx_toggle;
    struct cec_msg rx_msg;
    u32 rx_bit;
    bool rx_toggle;
    u32 rx_start_bit_low_too_short_cnt;
    u64 rx_start_bit_low_too_short_ts;
    u32 rx_start_bit_low_too_short_delta;
    u32 rx_start_bit_too_short_cnt;
    u64 rx_start_bit_too_short_ts;
    u32 rx_start_bit_too_short_delta;
    u32 rx_start_bit_too_long_cnt;
    u32 rx_data_bit_too_short_cnt;
    u64 rx_data_bit_too_short_ts;
    u32 rx_data_bit_too_short_delta;
    u32 rx_data_bit_too_long_cnt;
    u32 rx_low_drive_cnt;
    struct cec_msg work_rx_msg;
    u8 work_tx_status;
    ktime_t work_tx_ts;
    atomic_t work_irq_change;
    atomic_t work_pin_num_events;
    unsigned int work_pin_events_wr;
    unsigned int work_pin_events_rd;
    ktime_t work_pin_ts[128];
    u8 work_pin_events[128];
    bool work_pin_events_dropped;
    u32 work_pin_events_dropped_cnt;
    ktime_t timer_ts;
    u32 timer_cnt;
    u32 timer_100ms_overruns;
    u32 timer_300ms_overruns;
    u32 timer_max_overrun;
    u32 timer_sum_overrun;
    u32 tx_custom_low_usecs;
    u32 tx_custom_high_usecs;
    bool tx_ignore_nack_until_eom;
    bool tx_custom_pulse;
    bool tx_generated_poll;
    bool tx_post_eom;
    u8 tx_extra_bytes;
    u32 tx_low_drive_cnt;
};
```
</details>
</li>
</ul>

## Differences
<b>Arch</b>
<ul>
</ul>
<b>Flavor</b>
<ul>
</ul>
