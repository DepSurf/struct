# Struct: <code>dwc2_qh</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct dwc2_qh {
    u8 ep_type;
    u8 ep_is_in;
    u16 maxp;
    u8 dev_speed;
    u8 data_toggle;
    u8 ping_state;
    u8 do_split;
    u8 td_first;
    u8 td_last;
    u16 usecs;
    u16 interval;
    u16 sched_frame;
    u16 frame_usecs[8];
    u16 start_split_frame;
    u16 ntd;
    u8 *dw_align_buf;
    int dw_align_buf_size;
    dma_addr_t dw_align_buf_dma;
    struct list_head qtd_list;
    struct dwc2_host_chan *channel;
    struct list_head qh_list_entry;
    struct dwc2_hcd_dma_desc *desc_list;
    dma_addr_t desc_list_dma;
    u32 *n_bytes;
    unsigned int tt_buffer_dirty;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct dwc2_qh {
    struct dwc2_hsotg *hsotg;
    u8 ep_type;
    u8 ep_is_in;
    u16 maxp;
    u8 dev_speed;
    u8 data_toggle;
    u8 ping_state;
    u8 do_split;
    u8 td_first;
    u8 td_last;
    u16 host_us;
    u16 device_us;
    u16 host_interval;
    u16 device_interval;
    u16 next_active_frame;
    u16 start_active_frame;
    s16 num_hs_transfers;
    struct dwc2_hs_transfer_time hs_transfers[8];
    u32 ls_start_schedule_slice;
    u16 ntd;
    struct list_head qtd_list;
    struct dwc2_host_chan *channel;
    struct list_head qh_list_entry;
    struct dwc2_hcd_dma_desc *desc_list;
    dma_addr_t desc_list_dma;
    u32 desc_list_sz;
    u32 *n_bytes;
    struct timer_list unreserve_timer;
    struct dwc2_tt *dwc_tt;
    int ttport;
    unsigned int tt_buffer_dirty;
    unsigned int unreserve_pending;
    unsigned int schedule_low_speed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct dwc2_qh {
    struct dwc2_hsotg *hsotg;
    u8 ep_type;
    u8 ep_is_in;
    u16 maxp;
    u8 dev_speed;
    u8 data_toggle;
    u8 ping_state;
    u8 do_split;
    u8 td_first;
    u8 td_last;
    u16 host_us;
    u16 device_us;
    u16 host_interval;
    u16 device_interval;
    u16 next_active_frame;
    u16 start_active_frame;
    s16 num_hs_transfers;
    struct dwc2_hs_transfer_time hs_transfers[8];
    u32 ls_start_schedule_slice;
    u16 ntd;
    struct list_head qtd_list;
    struct dwc2_host_chan *channel;
    struct list_head qh_list_entry;
    struct dwc2_dma_desc *desc_list;
    dma_addr_t desc_list_dma;
    u32 desc_list_sz;
    u32 *n_bytes;
    struct timer_list unreserve_timer;
    struct dwc2_tt *dwc_tt;
    int ttport;
    unsigned int tt_buffer_dirty;
    unsigned int unreserve_pending;
    unsigned int schedule_low_speed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct dwc2_qh {
    struct dwc2_hsotg *hsotg;
    u8 ep_type;
    u8 ep_is_in;
    u16 maxp;
    u8 dev_speed;
    u8 data_toggle;
    u8 ping_state;
    u8 do_split;
    u8 td_first;
    u8 td_last;
    u16 host_us;
    u16 device_us;
    u16 host_interval;
    u16 device_interval;
    u16 next_active_frame;
    u16 start_active_frame;
    s16 num_hs_transfers;
    struct dwc2_hs_transfer_time hs_transfers[8];
    u32 ls_start_schedule_slice;
    u16 ntd;
    struct list_head qtd_list;
    struct dwc2_host_chan *channel;
    struct list_head qh_list_entry;
    struct dwc2_dma_desc *desc_list;
    dma_addr_t desc_list_dma;
    u32 desc_list_sz;
    u32 *n_bytes;
    struct timer_list unreserve_timer;
    struct dwc2_tt *dwc_tt;
    int ttport;
    unsigned int tt_buffer_dirty;
    unsigned int unreserve_pending;
    unsigned int schedule_low_speed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dwc2_qh {
    struct dwc2_hsotg *hsotg;
    u8 ep_type;
    u8 ep_is_in;
    u16 maxp;
    u8 dev_speed;
    u8 data_toggle;
    u8 ping_state;
    u8 do_split;
    u8 td_first;
    u8 td_last;
    u16 host_us;
    u16 device_us;
    u16 host_interval;
    u16 device_interval;
    u16 next_active_frame;
    u16 start_active_frame;
    s16 num_hs_transfers;
    struct dwc2_hs_transfer_time hs_transfers[8];
    u32 ls_start_schedule_slice;
    u16 ntd;
    struct list_head qtd_list;
    struct dwc2_host_chan *channel;
    struct list_head qh_list_entry;
    struct dwc2_dma_desc *desc_list;
    dma_addr_t desc_list_dma;
    u32 desc_list_sz;
    u32 *n_bytes;
    struct timer_list unreserve_timer;
    struct dwc2_tt *dwc_tt;
    int ttport;
    unsigned int tt_buffer_dirty;
    unsigned int unreserve_pending;
    unsigned int schedule_low_speed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dwc2_qh {
    struct dwc2_hsotg *hsotg;
    u8 ep_type;
    u8 ep_is_in;
    u16 maxp;
    u8 dev_speed;
    u8 data_toggle;
    u8 ping_state;
    u8 do_split;
    u8 td_first;
    u8 td_last;
    u16 host_us;
    u16 device_us;
    u16 host_interval;
    u16 device_interval;
    u16 next_active_frame;
    u16 start_active_frame;
    s16 num_hs_transfers;
    struct dwc2_hs_transfer_time hs_transfers[8];
    u32 ls_start_schedule_slice;
    u16 ntd;
    u8 *dw_align_buf;
    dma_addr_t dw_align_buf_dma;
    struct list_head qtd_list;
    struct dwc2_host_chan *channel;
    struct list_head qh_list_entry;
    struct dwc2_dma_desc *desc_list;
    dma_addr_t desc_list_dma;
    u32 desc_list_sz;
    u32 *n_bytes;
    struct timer_list unreserve_timer;
    struct timer_list wait_timer;
    struct dwc2_tt *dwc_tt;
    int ttport;
    unsigned int tt_buffer_dirty;
    unsigned int unreserve_pending;
    unsigned int schedule_low_speed;
    unsigned int want_wait;
    unsigned int wait_timer_cancel;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dwc2_qh {
    struct dwc2_hsotg *hsotg;
    u8 ep_type;
    u8 ep_is_in;
    u16 maxp;
    u8 dev_speed;
    u8 data_toggle;
    u8 ping_state;
    u8 do_split;
    u8 td_first;
    u8 td_last;
    u16 host_us;
    u16 device_us;
    u16 host_interval;
    u16 device_interval;
    u16 next_active_frame;
    u16 start_active_frame;
    s16 num_hs_transfers;
    struct dwc2_hs_transfer_time hs_transfers[8];
    u32 ls_start_schedule_slice;
    u16 ntd;
    u8 *dw_align_buf;
    dma_addr_t dw_align_buf_dma;
    struct list_head qtd_list;
    struct dwc2_host_chan *channel;
    struct list_head qh_list_entry;
    struct dwc2_dma_desc *desc_list;
    dma_addr_t desc_list_dma;
    u32 desc_list_sz;
    u32 *n_bytes;
    struct timer_list unreserve_timer;
    struct hrtimer wait_timer;
    struct dwc2_tt *dwc_tt;
    int ttport;
    unsigned int tt_buffer_dirty;
    unsigned int unreserve_pending;
    unsigned int schedule_low_speed;
    unsigned int want_wait;
    unsigned int wait_timer_cancel;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dwc2_qh {
    struct dwc2_hsotg *hsotg;
    u8 ep_type;
    u8 ep_is_in;
    u16 maxp;
    u16 maxp_mult;
    u8 dev_speed;
    u8 data_toggle;
    u8 ping_state;
    u8 do_split;
    u8 td_first;
    u8 td_last;
    u16 host_us;
    u16 device_us;
    u16 host_interval;
    u16 device_interval;
    u16 next_active_frame;
    u16 start_active_frame;
    s16 num_hs_transfers;
    struct dwc2_hs_transfer_time hs_transfers[8];
    u32 ls_start_schedule_slice;
    u16 ntd;
    u8 *dw_align_buf;
    dma_addr_t dw_align_buf_dma;
    struct list_head qtd_list;
    struct dwc2_host_chan *channel;
    struct list_head qh_list_entry;
    struct dwc2_dma_desc *desc_list;
    dma_addr_t desc_list_dma;
    u32 desc_list_sz;
    u32 *n_bytes;
    struct timer_list unreserve_timer;
    struct hrtimer wait_timer;
    struct dwc2_tt *dwc_tt;
    int ttport;
    unsigned int tt_buffer_dirty;
    unsigned int unreserve_pending;
    unsigned int schedule_low_speed;
    unsigned int want_wait;
    unsigned int wait_timer_cancel;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dwc2_qh {
    struct dwc2_hsotg *hsotg;
    u8 ep_type;
    u8 ep_is_in;
    u16 maxp;
    u16 maxp_mult;
    u8 dev_speed;
    u8 data_toggle;
    u8 ping_state;
    u8 do_split;
    u8 td_first;
    u8 td_last;
    u16 host_us;
    u16 device_us;
    u16 host_interval;
    u16 device_interval;
    u16 next_active_frame;
    u16 start_active_frame;
    s16 num_hs_transfers;
    struct dwc2_hs_transfer_time hs_transfers[8];
    u32 ls_start_schedule_slice;
    u16 ntd;
    u8 *dw_align_buf;
    dma_addr_t dw_align_buf_dma;
    struct list_head qtd_list;
    struct dwc2_host_chan *channel;
    struct list_head qh_list_entry;
    struct dwc2_dma_desc *desc_list;
    dma_addr_t desc_list_dma;
    u32 desc_list_sz;
    u32 *n_bytes;
    struct timer_list unreserve_timer;
    struct hrtimer wait_timer;
    struct dwc2_tt *dwc_tt;
    int ttport;
    unsigned int tt_buffer_dirty;
    unsigned int unreserve_pending;
    unsigned int schedule_low_speed;
    unsigned int want_wait;
    unsigned int wait_timer_cancel;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dwc2_qh {
    struct dwc2_hsotg *hsotg;
    u8 ep_type;
    u8 ep_is_in;
    u16 maxp;
    u16 maxp_mult;
    u8 dev_speed;
    u8 data_toggle;
    u8 ping_state;
    u8 do_split;
    u8 td_first;
    u8 td_last;
    u16 host_us;
    u16 device_us;
    u16 host_interval;
    u16 device_interval;
    u16 next_active_frame;
    u16 start_active_frame;
    s16 num_hs_transfers;
    struct dwc2_hs_transfer_time hs_transfers[8];
    u32 ls_start_schedule_slice;
    u16 ntd;
    u8 *dw_align_buf;
    dma_addr_t dw_align_buf_dma;
    struct list_head qtd_list;
    struct dwc2_host_chan *channel;
    struct list_head qh_list_entry;
    struct dwc2_dma_desc *desc_list;
    dma_addr_t desc_list_dma;
    u32 desc_list_sz;
    u32 *n_bytes;
    struct timer_list unreserve_timer;
    struct hrtimer wait_timer;
    struct dwc2_tt *dwc_tt;
    int ttport;
    unsigned int tt_buffer_dirty;
    unsigned int unreserve_pending;
    unsigned int schedule_low_speed;
    unsigned int want_wait;
    unsigned int wait_timer_cancel;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dwc2_qh {
    struct dwc2_hsotg *hsotg;
    u8 ep_type;
    u8 ep_is_in;
    u16 maxp;
    u16 maxp_mult;
    u8 dev_speed;
    u8 data_toggle;
    u8 ping_state;
    u8 do_split;
    u8 td_first;
    u8 td_last;
    u16 host_us;
    u16 device_us;
    u16 host_interval;
    u16 device_interval;
    u16 next_active_frame;
    u16 start_active_frame;
    s16 num_hs_transfers;
    struct dwc2_hs_transfer_time hs_transfers[8];
    u32 ls_start_schedule_slice;
    u16 ntd;
    u8 *dw_align_buf;
    dma_addr_t dw_align_buf_dma;
    struct list_head qtd_list;
    struct dwc2_host_chan *channel;
    struct list_head qh_list_entry;
    struct dwc2_dma_desc *desc_list;
    dma_addr_t desc_list_dma;
    u32 desc_list_sz;
    u32 *n_bytes;
    struct timer_list unreserve_timer;
    struct hrtimer wait_timer;
    struct dwc2_tt *dwc_tt;
    int ttport;
    unsigned int tt_buffer_dirty;
    unsigned int unreserve_pending;
    unsigned int schedule_low_speed;
    unsigned int want_wait;
    unsigned int wait_timer_cancel;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dwc2_qh {
    struct dwc2_hsotg *hsotg;
    u8 ep_type;
    u8 ep_is_in;
    u16 maxp;
    u16 maxp_mult;
    u8 dev_speed;
    u8 data_toggle;
    u8 ping_state;
    u8 do_split;
    u8 td_first;
    u8 td_last;
    u16 host_us;
    u16 device_us;
    u16 host_interval;
    u16 device_interval;
    u16 next_active_frame;
    u16 start_active_frame;
    s16 num_hs_transfers;
    struct dwc2_hs_transfer_time hs_transfers[8];
    u32 ls_start_schedule_slice;
    u16 ntd;
    u8 *dw_align_buf;
    dma_addr_t dw_align_buf_dma;
    struct list_head qtd_list;
    struct dwc2_host_chan *channel;
    struct list_head qh_list_entry;
    struct dwc2_dma_desc *desc_list;
    dma_addr_t desc_list_dma;
    u32 desc_list_sz;
    u32 *n_bytes;
    struct timer_list unreserve_timer;
    struct hrtimer wait_timer;
    struct dwc2_tt *dwc_tt;
    int ttport;
    unsigned int tt_buffer_dirty;
    unsigned int unreserve_pending;
    unsigned int schedule_low_speed;
    unsigned int want_wait;
    unsigned int wait_timer_cancel;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dwc2_qh {
    struct dwc2_hsotg *hsotg;
    u8 ep_type;
    u8 ep_is_in;
    u16 maxp;
    u16 maxp_mult;
    u8 dev_speed;
    u8 data_toggle;
    u8 ping_state;
    u8 do_split;
    u8 td_first;
    u8 td_last;
    u16 host_us;
    u16 device_us;
    u16 host_interval;
    u16 device_interval;
    u16 next_active_frame;
    u16 start_active_frame;
    s16 num_hs_transfers;
    struct dwc2_hs_transfer_time hs_transfers[8];
    u32 ls_start_schedule_slice;
    u16 ntd;
    u8 *dw_align_buf;
    dma_addr_t dw_align_buf_dma;
    struct list_head qtd_list;
    struct dwc2_host_chan *channel;
    struct list_head qh_list_entry;
    struct dwc2_dma_desc *desc_list;
    dma_addr_t desc_list_dma;
    u32 desc_list_sz;
    u32 *n_bytes;
    struct timer_list unreserve_timer;
    struct hrtimer wait_timer;
    struct dwc2_tt *dwc_tt;
    int ttport;
    unsigned int tt_buffer_dirty;
    unsigned int unreserve_pending;
    unsigned int schedule_low_speed;
    unsigned int want_wait;
    unsigned int wait_timer_cancel;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dwc2_qh {
    struct dwc2_hsotg *hsotg;
    u8 ep_type;
    u8 ep_is_in;
    u16 maxp;
    u16 maxp_mult;
    u8 dev_speed;
    u8 data_toggle;
    u8 ping_state;
    u8 do_split;
    u8 td_first;
    u8 td_last;
    u16 host_us;
    u16 device_us;
    u16 host_interval;
    u16 device_interval;
    u16 next_active_frame;
    u16 start_active_frame;
    s16 num_hs_transfers;
    struct dwc2_hs_transfer_time hs_transfers[8];
    u32 ls_start_schedule_slice;
    u16 ntd;
    u8 *dw_align_buf;
    dma_addr_t dw_align_buf_dma;
    struct list_head qtd_list;
    struct dwc2_host_chan *channel;
    struct list_head qh_list_entry;
    struct dwc2_dma_desc *desc_list;
    dma_addr_t desc_list_dma;
    u32 desc_list_sz;
    u32 *n_bytes;
    struct timer_list unreserve_timer;
    struct hrtimer wait_timer;
    struct dwc2_tt *dwc_tt;
    int ttport;
    unsigned int tt_buffer_dirty;
    unsigned int unreserve_pending;
    unsigned int schedule_low_speed;
    unsigned int want_wait;
    unsigned int wait_timer_cancel;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dwc2_qh {
    struct dwc2_hsotg *hsotg;
    u8 ep_type;
    u8 ep_is_in;
    u16 maxp;
    u16 maxp_mult;
    u8 dev_speed;
    u8 data_toggle;
    u8 ping_state;
    u8 do_split;
    u8 td_first;
    u8 td_last;
    u16 host_us;
    u16 device_us;
    u16 host_interval;
    u16 device_interval;
    u16 next_active_frame;
    u16 start_active_frame;
    s16 num_hs_transfers;
    struct dwc2_hs_transfer_time hs_transfers[8];
    u32 ls_start_schedule_slice;
    u16 ntd;
    u8 *dw_align_buf;
    dma_addr_t dw_align_buf_dma;
    struct list_head qtd_list;
    struct dwc2_host_chan *channel;
    struct list_head qh_list_entry;
    struct dwc2_dma_desc *desc_list;
    dma_addr_t desc_list_dma;
    u32 desc_list_sz;
    u32 *n_bytes;
    struct timer_list unreserve_timer;
    struct hrtimer wait_timer;
    struct dwc2_tt *dwc_tt;
    int ttport;
    unsigned int tt_buffer_dirty;
    unsigned int unreserve_pending;
    unsigned int schedule_low_speed;
    unsigned int want_wait;
    unsigned int wait_timer_cancel;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dwc2_qh {
    struct dwc2_hsotg *hsotg;
    u8 ep_type;
    u8 ep_is_in;
    u16 maxp;
    u16 maxp_mult;
    u8 dev_speed;
    u8 data_toggle;
    u8 ping_state;
    u8 do_split;
    u8 td_first;
    u8 td_last;
    u16 host_us;
    u16 device_us;
    u16 host_interval;
    u16 device_interval;
    u16 next_active_frame;
    u16 start_active_frame;
    s16 num_hs_transfers;
    struct dwc2_hs_transfer_time hs_transfers[8];
    u32 ls_start_schedule_slice;
    u16 ntd;
    u8 *dw_align_buf;
    dma_addr_t dw_align_buf_dma;
    struct list_head qtd_list;
    struct dwc2_host_chan *channel;
    struct list_head qh_list_entry;
    struct dwc2_dma_desc *desc_list;
    dma_addr_t desc_list_dma;
    u32 desc_list_sz;
    u32 *n_bytes;
    struct timer_list unreserve_timer;
    struct hrtimer wait_timer;
    struct dwc2_tt *dwc_tt;
    int ttport;
    unsigned int tt_buffer_dirty;
    unsigned int unreserve_pending;
    unsigned int schedule_low_speed;
    unsigned int want_wait;
    unsigned int wait_timer_cancel;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dwc2_qh {
    struct dwc2_hsotg *hsotg;
    u8 ep_type;
    u8 ep_is_in;
    u16 maxp;
    u16 maxp_mult;
    u8 dev_speed;
    u8 data_toggle;
    u8 ping_state;
    u8 do_split;
    u8 td_first;
    u8 td_last;
    u16 host_us;
    u16 device_us;
    u16 host_interval;
    u16 device_interval;
    u16 next_active_frame;
    u16 start_active_frame;
    s16 num_hs_transfers;
    struct dwc2_hs_transfer_time hs_transfers[8];
    u32 ls_start_schedule_slice;
    u16 ntd;
    u8 *dw_align_buf;
    dma_addr_t dw_align_buf_dma;
    struct list_head qtd_list;
    struct dwc2_host_chan *channel;
    struct list_head qh_list_entry;
    struct dwc2_dma_desc *desc_list;
    dma_addr_t desc_list_dma;
    u32 desc_list_sz;
    u32 *n_bytes;
    struct timer_list unreserve_timer;
    struct hrtimer wait_timer;
    struct dwc2_tt *dwc_tt;
    int ttport;
    unsigned int tt_buffer_dirty;
    unsigned int unreserve_pending;
    unsigned int schedule_low_speed;
    unsigned int want_wait;
    unsigned int wait_timer_cancel;
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
struct dwc2_qh {
    struct dwc2_hsotg *hsotg;
    u8 ep_type;
    u8 ep_is_in;
    u16 maxp;
    u16 maxp_mult;
    u8 dev_speed;
    u8 data_toggle;
    u8 ping_state;
    u8 do_split;
    u8 td_first;
    u8 td_last;
    u16 host_us;
    u16 device_us;
    u16 host_interval;
    u16 device_interval;
    u16 next_active_frame;
    u16 start_active_frame;
    s16 num_hs_transfers;
    struct dwc2_hs_transfer_time hs_transfers[8];
    u32 ls_start_schedule_slice;
    u16 ntd;
    u8 *dw_align_buf;
    dma_addr_t dw_align_buf_dma;
    struct list_head qtd_list;
    struct dwc2_host_chan *channel;
    struct list_head qh_list_entry;
    struct dwc2_dma_desc *desc_list;
    dma_addr_t desc_list_dma;
    u32 desc_list_sz;
    u32 *n_bytes;
    struct timer_list unreserve_timer;
    struct hrtimer wait_timer;
    struct dwc2_tt *dwc_tt;
    int ttport;
    unsigned int tt_buffer_dirty;
    unsigned int unreserve_pending;
    unsigned int schedule_low_speed;
    unsigned int want_wait;
    unsigned int wait_timer_cancel;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dwc2_qh {
    struct dwc2_hsotg *hsotg;
    u8 ep_type;
    u8 ep_is_in;
    u16 maxp;
    u16 maxp_mult;
    u8 dev_speed;
    u8 data_toggle;
    u8 ping_state;
    u8 do_split;
    u8 td_first;
    u8 td_last;
    u16 host_us;
    u16 device_us;
    u16 host_interval;
    u16 device_interval;
    u16 next_active_frame;
    u16 start_active_frame;
    s16 num_hs_transfers;
    struct dwc2_hs_transfer_time hs_transfers[8];
    u32 ls_start_schedule_slice;
    u16 ntd;
    u8 *dw_align_buf;
    dma_addr_t dw_align_buf_dma;
    struct list_head qtd_list;
    struct dwc2_host_chan *channel;
    struct list_head qh_list_entry;
    struct dwc2_dma_desc *desc_list;
    dma_addr_t desc_list_dma;
    u32 desc_list_sz;
    u32 *n_bytes;
    struct timer_list unreserve_timer;
    struct hrtimer wait_timer;
    struct dwc2_tt *dwc_tt;
    int ttport;
    unsigned int tt_buffer_dirty;
    unsigned int unreserve_pending;
    unsigned int schedule_low_speed;
    unsigned int want_wait;
    unsigned int wait_timer_cancel;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dwc2_qh {
    struct dwc2_hsotg *hsotg;
    u8 ep_type;
    u8 ep_is_in;
    u16 maxp;
    u16 maxp_mult;
    u8 dev_speed;
    u8 data_toggle;
    u8 ping_state;
    u8 do_split;
    u8 td_first;
    u8 td_last;
    u16 host_us;
    u16 device_us;
    u16 host_interval;
    u16 device_interval;
    u16 next_active_frame;
    u16 start_active_frame;
    s16 num_hs_transfers;
    struct dwc2_hs_transfer_time hs_transfers[8];
    u32 ls_start_schedule_slice;
    u16 ntd;
    u8 *dw_align_buf;
    dma_addr_t dw_align_buf_dma;
    struct list_head qtd_list;
    struct dwc2_host_chan *channel;
    struct list_head qh_list_entry;
    struct dwc2_dma_desc *desc_list;
    dma_addr_t desc_list_dma;
    u32 desc_list_sz;
    u32 *n_bytes;
    struct timer_list unreserve_timer;
    struct hrtimer wait_timer;
    struct dwc2_tt *dwc_tt;
    int ttport;
    unsigned int tt_buffer_dirty;
    unsigned int unreserve_pending;
    unsigned int schedule_low_speed;
    unsigned int want_wait;
    unsigned int wait_timer_cancel;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dwc2_qh {
    struct dwc2_hsotg *hsotg;
    u8 ep_type;
    u8 ep_is_in;
    u16 maxp;
    u16 maxp_mult;
    u8 dev_speed;
    u8 data_toggle;
    u8 ping_state;
    u8 do_split;
    u8 td_first;
    u8 td_last;
    u16 host_us;
    u16 device_us;
    u16 host_interval;
    u16 device_interval;
    u16 next_active_frame;
    u16 start_active_frame;
    s16 num_hs_transfers;
    struct dwc2_hs_transfer_time hs_transfers[8];
    u32 ls_start_schedule_slice;
    u16 ntd;
    u8 *dw_align_buf;
    dma_addr_t dw_align_buf_dma;
    struct list_head qtd_list;
    struct dwc2_host_chan *channel;
    struct list_head qh_list_entry;
    struct dwc2_dma_desc *desc_list;
    dma_addr_t desc_list_dma;
    u32 desc_list_sz;
    u32 *n_bytes;
    struct timer_list unreserve_timer;
    struct hrtimer wait_timer;
    struct dwc2_tt *dwc_tt;
    int ttport;
    unsigned int tt_buffer_dirty;
    unsigned int unreserve_pending;
    unsigned int schedule_low_speed;
    unsigned int want_wait;
    unsigned int wait_timer_cancel;
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
struct dwc2_qh {
    struct dwc2_hsotg *hsotg;
    u8 ep_type;
    u8 ep_is_in;
    u16 maxp;
    u16 maxp_mult;
    u8 dev_speed;
    u8 data_toggle;
    u8 ping_state;
    u8 do_split;
    u8 td_first;
    u8 td_last;
    u16 host_us;
    u16 device_us;
    u16 host_interval;
    u16 device_interval;
    u16 next_active_frame;
    u16 start_active_frame;
    s16 num_hs_transfers;
    struct dwc2_hs_transfer_time hs_transfers[8];
    u32 ls_start_schedule_slice;
    u16 ntd;
    u8 *dw_align_buf;
    dma_addr_t dw_align_buf_dma;
    struct list_head qtd_list;
    struct dwc2_host_chan *channel;
    struct list_head qh_list_entry;
    struct dwc2_dma_desc *desc_list;
    dma_addr_t desc_list_dma;
    u32 desc_list_sz;
    u32 *n_bytes;
    struct timer_list unreserve_timer;
    struct hrtimer wait_timer;
    struct dwc2_tt *dwc_tt;
    int ttport;
    unsigned int tt_buffer_dirty;
    unsigned int unreserve_pending;
    unsigned int schedule_low_speed;
    unsigned int want_wait;
    unsigned int wait_timer_cancel;
};
```
</details>
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dwc2_qh {
    struct dwc2_hsotg *hsotg;
    u8 ep_type;
    u8 ep_is_in;
    u16 maxp;
    u16 maxp_mult;
    u8 dev_speed;
    u8 data_toggle;
    u8 ping_state;
    u8 do_split;
    u8 td_first;
    u8 td_last;
    u16 host_us;
    u16 device_us;
    u16 host_interval;
    u16 device_interval;
    u16 next_active_frame;
    u16 start_active_frame;
    s16 num_hs_transfers;
    struct dwc2_hs_transfer_time hs_transfers[8];
    u32 ls_start_schedule_slice;
    u16 ntd;
    u8 *dw_align_buf;
    dma_addr_t dw_align_buf_dma;
    struct list_head qtd_list;
    struct dwc2_host_chan *channel;
    struct list_head qh_list_entry;
    struct dwc2_dma_desc *desc_list;
    dma_addr_t desc_list_dma;
    u32 desc_list_sz;
    u32 *n_bytes;
    struct timer_list unreserve_timer;
    struct hrtimer wait_timer;
    struct dwc2_tt *dwc_tt;
    int ttport;
    unsigned int tt_buffer_dirty;
    unsigned int unreserve_pending;
    unsigned int schedule_low_speed;
    unsigned int want_wait;
    unsigned int wait_timer_cancel;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dwc2_qh {
    struct dwc2_hsotg *hsotg;
    u8 ep_type;
    u8 ep_is_in;
    u16 maxp;
    u16 maxp_mult;
    u8 dev_speed;
    u8 data_toggle;
    u8 ping_state;
    u8 do_split;
    u8 td_first;
    u8 td_last;
    u16 host_us;
    u16 device_us;
    u16 host_interval;
    u16 device_interval;
    u16 next_active_frame;
    u16 start_active_frame;
    s16 num_hs_transfers;
    struct dwc2_hs_transfer_time hs_transfers[8];
    u32 ls_start_schedule_slice;
    u16 ntd;
    u8 *dw_align_buf;
    dma_addr_t dw_align_buf_dma;
    struct list_head qtd_list;
    struct dwc2_host_chan *channel;
    struct list_head qh_list_entry;
    struct dwc2_dma_desc *desc_list;
    dma_addr_t desc_list_dma;
    u32 desc_list_sz;
    u32 *n_bytes;
    struct timer_list unreserve_timer;
    struct hrtimer wait_timer;
    struct dwc2_tt *dwc_tt;
    int ttport;
    unsigned int tt_buffer_dirty;
    unsigned int unreserve_pending;
    unsigned int schedule_low_speed;
    unsigned int want_wait;
    unsigned int wait_timer_cancel;
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
<code>struct dwc2_hsotg *hsotg</code>
</li>
<li>
<b>Field added. </b>
<code>u16 host_us</code>
</li>
<li>
<b>Field added. </b>
<code>u16 device_us</code>
</li>
<li>
<b>Field added. </b>
<code>u16 host_interval</code>
</li>
<li>
<b>Field added. </b>
<code>u16 device_interval</code>
</li>
<li>
<b>Field added. </b>
<code>u16 next_active_frame</code>
</li>
<li>
<b>Field added. </b>
<code>u16 start_active_frame</code>
</li>
<li>
<b>Field added. </b>
<code>s16 num_hs_transfers</code>
</li>
<li>
<b>Field added. </b>
<code>struct dwc2_hs_transfer_time hs_transfers[8]</code>
</li>
<li>
<b>Field added. </b>
<code>u32 ls_start_schedule_slice</code>
</li>
<li>
<b>Field added. </b>
<code>u32 desc_list_sz</code>
</li>
<li>
<b>Field added. </b>
<code>struct timer_list unreserve_timer</code>
</li>
<li>
<b>Field added. </b>
<code>struct dwc2_tt *dwc_tt</code>
</li>
<li>
<b>Field added. </b>
<code>int ttport</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int unreserve_pending</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int schedule_low_speed</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 usecs</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 interval</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 sched_frame</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 frame_usecs[8]</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 start_split_frame</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 *dw_align_buf</code>
</li>
<li>
<b>Field removed. </b>
<code>int dw_align_buf_size</code>
</li>
<li>
<b>Field removed. </b>
<code>dma_addr_t dw_align_buf_dma</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct dwc2_hcd_dma_desc *desc_list</code> ➡️ <code>struct dwc2_dma_desc *desc_list</code>
</li>
</ul>
</details>
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
<b>Field added. </b>
<code>u8 *dw_align_buf</code>
</li>
<li>
<b>Field added. </b>
<code>dma_addr_t dw_align_buf_dma</code>
</li>
<li>
<b>Field added. </b>
<code>struct timer_list wait_timer</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int want_wait</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int wait_timer_cancel</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct timer_list wait_timer</code> ➡️ <code>struct hrtimer wait_timer</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 maxp_mult</code>
</li>
</ul>
</details>
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
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
