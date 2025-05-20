# Struct: <code>uhci_hcd</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct uhci_hcd {
    struct dentry *dentry;
    long unsigned int io_addr;
    void *regs;
    struct dma_pool *qh_pool;
    struct dma_pool *td_pool;
    struct uhci_td *term_td;
    struct uhci_qh * skelqh[11];
    struct uhci_qh *next_qh;
    spinlock_t lock;
    dma_addr_t frame_dma_handle;
    __le32 *frame;
    void **frame_cpu;
    enum uhci_rh_state rh_state;
    long unsigned int auto_stop_time;
    unsigned int frame_number;
    unsigned int is_stopped;
    unsigned int last_iso_frame;
    unsigned int cur_iso_frame;
    unsigned int scan_in_progress;
    unsigned int need_rescan;
    unsigned int dead;
    unsigned int RD_enable;
    unsigned int is_initialized;
    unsigned int fsbr_is_on;
    unsigned int fsbr_is_wanted;
    unsigned int fsbr_expiring;
    struct timer_list fsbr_timer;
    unsigned int oc_low;
    unsigned int wait_for_hp;
    unsigned int big_endian_mmio;
    unsigned int big_endian_desc;
    long unsigned int port_c_suspend;
    long unsigned int resuming_ports;
    long unsigned int ports_timeout;
    struct list_head idle_qh_list;
    int rh_numports;
    wait_queue_head_t waitqh;
    int num_waiting;
    int total_load;
    short int load[32];
    void (*reset_hc)(struct uhci_hcd *);
    int (*check_and_reset_hc)(struct uhci_hcd *);
    void (*configure_hc)(struct uhci_hcd *);
    int (*resume_detect_interrupts_are_broken)(struct uhci_hcd *);
    int (*global_suspend_mode_is_broken)(struct uhci_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct uhci_hcd {
    struct dentry *dentry;
    long unsigned int io_addr;
    void *regs;
    struct dma_pool *qh_pool;
    struct dma_pool *td_pool;
    struct uhci_td *term_td;
    struct uhci_qh * skelqh[11];
    struct uhci_qh *next_qh;
    spinlock_t lock;
    dma_addr_t frame_dma_handle;
    __le32 *frame;
    void **frame_cpu;
    enum uhci_rh_state rh_state;
    long unsigned int auto_stop_time;
    unsigned int frame_number;
    unsigned int is_stopped;
    unsigned int last_iso_frame;
    unsigned int cur_iso_frame;
    unsigned int scan_in_progress;
    unsigned int need_rescan;
    unsigned int dead;
    unsigned int RD_enable;
    unsigned int is_initialized;
    unsigned int fsbr_is_on;
    unsigned int fsbr_is_wanted;
    unsigned int fsbr_expiring;
    struct timer_list fsbr_timer;
    unsigned int oc_low;
    unsigned int wait_for_hp;
    unsigned int big_endian_mmio;
    unsigned int big_endian_desc;
    long unsigned int port_c_suspend;
    long unsigned int resuming_ports;
    long unsigned int ports_timeout;
    struct list_head idle_qh_list;
    int rh_numports;
    wait_queue_head_t waitqh;
    int num_waiting;
    int total_load;
    short int load[32];
    void (*reset_hc)(struct uhci_hcd *);
    int (*check_and_reset_hc)(struct uhci_hcd *);
    void (*configure_hc)(struct uhci_hcd *);
    int (*resume_detect_interrupts_are_broken)(struct uhci_hcd *);
    int (*global_suspend_mode_is_broken)(struct uhci_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct uhci_hcd {
    struct dentry *dentry;
    long unsigned int io_addr;
    void *regs;
    struct dma_pool *qh_pool;
    struct dma_pool *td_pool;
    struct uhci_td *term_td;
    struct uhci_qh * skelqh[11];
    struct uhci_qh *next_qh;
    spinlock_t lock;
    dma_addr_t frame_dma_handle;
    __le32 *frame;
    void **frame_cpu;
    enum uhci_rh_state rh_state;
    long unsigned int auto_stop_time;
    unsigned int frame_number;
    unsigned int is_stopped;
    unsigned int last_iso_frame;
    unsigned int cur_iso_frame;
    unsigned int scan_in_progress;
    unsigned int need_rescan;
    unsigned int dead;
    unsigned int RD_enable;
    unsigned int is_initialized;
    unsigned int fsbr_is_on;
    unsigned int fsbr_is_wanted;
    unsigned int fsbr_expiring;
    struct timer_list fsbr_timer;
    unsigned int oc_low;
    unsigned int wait_for_hp;
    unsigned int big_endian_mmio;
    unsigned int big_endian_desc;
    long unsigned int port_c_suspend;
    long unsigned int resuming_ports;
    long unsigned int ports_timeout;
    struct list_head idle_qh_list;
    int rh_numports;
    wait_queue_head_t waitqh;
    int num_waiting;
    int total_load;
    short int load[32];
    void (*reset_hc)(struct uhci_hcd *);
    int (*check_and_reset_hc)(struct uhci_hcd *);
    void (*configure_hc)(struct uhci_hcd *);
    int (*resume_detect_interrupts_are_broken)(struct uhci_hcd *);
    int (*global_suspend_mode_is_broken)(struct uhci_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct uhci_hcd {
    struct dentry *dentry;
    long unsigned int io_addr;
    void *regs;
    struct dma_pool *qh_pool;
    struct dma_pool *td_pool;
    struct uhci_td *term_td;
    struct uhci_qh * skelqh[11];
    struct uhci_qh *next_qh;
    spinlock_t lock;
    dma_addr_t frame_dma_handle;
    __le32 *frame;
    void **frame_cpu;
    enum uhci_rh_state rh_state;
    long unsigned int auto_stop_time;
    unsigned int frame_number;
    unsigned int is_stopped;
    unsigned int last_iso_frame;
    unsigned int cur_iso_frame;
    unsigned int scan_in_progress;
    unsigned int need_rescan;
    unsigned int dead;
    unsigned int RD_enable;
    unsigned int is_initialized;
    unsigned int fsbr_is_on;
    unsigned int fsbr_is_wanted;
    unsigned int fsbr_expiring;
    struct timer_list fsbr_timer;
    unsigned int oc_low;
    unsigned int wait_for_hp;
    unsigned int big_endian_mmio;
    unsigned int big_endian_desc;
    unsigned int is_aspeed;
    long unsigned int port_c_suspend;
    long unsigned int resuming_ports;
    long unsigned int ports_timeout;
    struct list_head idle_qh_list;
    int rh_numports;
    wait_queue_head_t waitqh;
    int num_waiting;
    int total_load;
    short int load[32];
    void (*reset_hc)(struct uhci_hcd *);
    int (*check_and_reset_hc)(struct uhci_hcd *);
    void (*configure_hc)(struct uhci_hcd *);
    int (*resume_detect_interrupts_are_broken)(struct uhci_hcd *);
    int (*global_suspend_mode_is_broken)(struct uhci_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct uhci_hcd {
    struct dentry *dentry;
    long unsigned int io_addr;
    void *regs;
    struct dma_pool *qh_pool;
    struct dma_pool *td_pool;
    struct uhci_td *term_td;
    struct uhci_qh * skelqh[11];
    struct uhci_qh *next_qh;
    spinlock_t lock;
    dma_addr_t frame_dma_handle;
    __le32 *frame;
    void **frame_cpu;
    enum uhci_rh_state rh_state;
    long unsigned int auto_stop_time;
    unsigned int frame_number;
    unsigned int is_stopped;
    unsigned int last_iso_frame;
    unsigned int cur_iso_frame;
    unsigned int scan_in_progress;
    unsigned int need_rescan;
    unsigned int dead;
    unsigned int RD_enable;
    unsigned int is_initialized;
    unsigned int fsbr_is_on;
    unsigned int fsbr_is_wanted;
    unsigned int fsbr_expiring;
    struct timer_list fsbr_timer;
    unsigned int oc_low;
    unsigned int wait_for_hp;
    unsigned int big_endian_mmio;
    unsigned int big_endian_desc;
    unsigned int is_aspeed;
    long unsigned int port_c_suspend;
    long unsigned int resuming_ports;
    long unsigned int ports_timeout;
    struct list_head idle_qh_list;
    int rh_numports;
    wait_queue_head_t waitqh;
    int num_waiting;
    int total_load;
    short int load[32];
    void (*reset_hc)(struct uhci_hcd *);
    int (*check_and_reset_hc)(struct uhci_hcd *);
    void (*configure_hc)(struct uhci_hcd *);
    int (*resume_detect_interrupts_are_broken)(struct uhci_hcd *);
    int (*global_suspend_mode_is_broken)(struct uhci_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct uhci_hcd {
    struct dentry *dentry;
    long unsigned int io_addr;
    void *regs;
    struct dma_pool *qh_pool;
    struct dma_pool *td_pool;
    struct uhci_td *term_td;
    struct uhci_qh * skelqh[11];
    struct uhci_qh *next_qh;
    spinlock_t lock;
    dma_addr_t frame_dma_handle;
    __le32 *frame;
    void **frame_cpu;
    enum uhci_rh_state rh_state;
    long unsigned int auto_stop_time;
    unsigned int frame_number;
    unsigned int is_stopped;
    unsigned int last_iso_frame;
    unsigned int cur_iso_frame;
    unsigned int scan_in_progress;
    unsigned int need_rescan;
    unsigned int dead;
    unsigned int RD_enable;
    unsigned int is_initialized;
    unsigned int fsbr_is_on;
    unsigned int fsbr_is_wanted;
    unsigned int fsbr_expiring;
    struct timer_list fsbr_timer;
    unsigned int oc_low;
    unsigned int wait_for_hp;
    unsigned int big_endian_mmio;
    unsigned int big_endian_desc;
    unsigned int is_aspeed;
    long unsigned int port_c_suspend;
    long unsigned int resuming_ports;
    long unsigned int ports_timeout;
    struct list_head idle_qh_list;
    int rh_numports;
    wait_queue_head_t waitqh;
    int num_waiting;
    int total_load;
    short int load[32];
    struct clk *clk;
    void (*reset_hc)(struct uhci_hcd *);
    int (*check_and_reset_hc)(struct uhci_hcd *);
    void (*configure_hc)(struct uhci_hcd *);
    int (*resume_detect_interrupts_are_broken)(struct uhci_hcd *);
    int (*global_suspend_mode_is_broken)(struct uhci_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct uhci_hcd {
    struct dentry *dentry;
    long unsigned int io_addr;
    void *regs;
    struct dma_pool *qh_pool;
    struct dma_pool *td_pool;
    struct uhci_td *term_td;
    struct uhci_qh * skelqh[11];
    struct uhci_qh *next_qh;
    spinlock_t lock;
    dma_addr_t frame_dma_handle;
    __le32 *frame;
    void **frame_cpu;
    enum uhci_rh_state rh_state;
    long unsigned int auto_stop_time;
    unsigned int frame_number;
    unsigned int is_stopped;
    unsigned int last_iso_frame;
    unsigned int cur_iso_frame;
    unsigned int scan_in_progress;
    unsigned int need_rescan;
    unsigned int dead;
    unsigned int RD_enable;
    unsigned int is_initialized;
    unsigned int fsbr_is_on;
    unsigned int fsbr_is_wanted;
    unsigned int fsbr_expiring;
    struct timer_list fsbr_timer;
    unsigned int oc_low;
    unsigned int wait_for_hp;
    unsigned int big_endian_mmio;
    unsigned int big_endian_desc;
    unsigned int is_aspeed;
    long unsigned int port_c_suspend;
    long unsigned int resuming_ports;
    long unsigned int ports_timeout;
    struct list_head idle_qh_list;
    int rh_numports;
    wait_queue_head_t waitqh;
    int num_waiting;
    int total_load;
    short int load[32];
    struct clk *clk;
    void (*reset_hc)(struct uhci_hcd *);
    int (*check_and_reset_hc)(struct uhci_hcd *);
    void (*configure_hc)(struct uhci_hcd *);
    int (*resume_detect_interrupts_are_broken)(struct uhci_hcd *);
    int (*global_suspend_mode_is_broken)(struct uhci_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct uhci_hcd {
    struct dentry *dentry;
    long unsigned int io_addr;
    void *regs;
    struct dma_pool *qh_pool;
    struct dma_pool *td_pool;
    struct uhci_td *term_td;
    struct uhci_qh * skelqh[11];
    struct uhci_qh *next_qh;
    spinlock_t lock;
    dma_addr_t frame_dma_handle;
    __le32 *frame;
    void **frame_cpu;
    enum uhci_rh_state rh_state;
    long unsigned int auto_stop_time;
    unsigned int frame_number;
    unsigned int is_stopped;
    unsigned int last_iso_frame;
    unsigned int cur_iso_frame;
    unsigned int scan_in_progress;
    unsigned int need_rescan;
    unsigned int dead;
    unsigned int RD_enable;
    unsigned int is_initialized;
    unsigned int fsbr_is_on;
    unsigned int fsbr_is_wanted;
    unsigned int fsbr_expiring;
    struct timer_list fsbr_timer;
    unsigned int oc_low;
    unsigned int wait_for_hp;
    unsigned int big_endian_mmio;
    unsigned int big_endian_desc;
    unsigned int is_aspeed;
    long unsigned int port_c_suspend;
    long unsigned int resuming_ports;
    long unsigned int ports_timeout;
    struct list_head idle_qh_list;
    int rh_numports;
    wait_queue_head_t waitqh;
    int num_waiting;
    int total_load;
    short int load[32];
    struct clk *clk;
    void (*reset_hc)(struct uhci_hcd *);
    int (*check_and_reset_hc)(struct uhci_hcd *);
    void (*configure_hc)(struct uhci_hcd *);
    int (*resume_detect_interrupts_are_broken)(struct uhci_hcd *);
    int (*global_suspend_mode_is_broken)(struct uhci_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct uhci_hcd {
    struct dentry *dentry;
    long unsigned int io_addr;
    void *regs;
    struct dma_pool *qh_pool;
    struct dma_pool *td_pool;
    struct uhci_td *term_td;
    struct uhci_qh * skelqh[11];
    struct uhci_qh *next_qh;
    spinlock_t lock;
    dma_addr_t frame_dma_handle;
    __le32 *frame;
    void **frame_cpu;
    enum uhci_rh_state rh_state;
    long unsigned int auto_stop_time;
    unsigned int frame_number;
    unsigned int is_stopped;
    unsigned int last_iso_frame;
    unsigned int cur_iso_frame;
    unsigned int scan_in_progress;
    unsigned int need_rescan;
    unsigned int dead;
    unsigned int RD_enable;
    unsigned int is_initialized;
    unsigned int fsbr_is_on;
    unsigned int fsbr_is_wanted;
    unsigned int fsbr_expiring;
    struct timer_list fsbr_timer;
    unsigned int oc_low;
    unsigned int wait_for_hp;
    unsigned int big_endian_mmio;
    unsigned int big_endian_desc;
    unsigned int is_aspeed;
    long unsigned int port_c_suspend;
    long unsigned int resuming_ports;
    long unsigned int ports_timeout;
    struct list_head idle_qh_list;
    int rh_numports;
    wait_queue_head_t waitqh;
    int num_waiting;
    int total_load;
    short int load[32];
    struct clk *clk;
    void (*reset_hc)(struct uhci_hcd *);
    int (*check_and_reset_hc)(struct uhci_hcd *);
    void (*configure_hc)(struct uhci_hcd *);
    int (*resume_detect_interrupts_are_broken)(struct uhci_hcd *);
    int (*global_suspend_mode_is_broken)(struct uhci_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct uhci_hcd {
    struct dentry *dentry;
    long unsigned int io_addr;
    void *regs;
    struct dma_pool *qh_pool;
    struct dma_pool *td_pool;
    struct uhci_td *term_td;
    struct uhci_qh * skelqh[11];
    struct uhci_qh *next_qh;
    spinlock_t lock;
    dma_addr_t frame_dma_handle;
    __le32 *frame;
    void **frame_cpu;
    enum uhci_rh_state rh_state;
    long unsigned int auto_stop_time;
    unsigned int frame_number;
    unsigned int is_stopped;
    unsigned int last_iso_frame;
    unsigned int cur_iso_frame;
    unsigned int scan_in_progress;
    unsigned int need_rescan;
    unsigned int dead;
    unsigned int RD_enable;
    unsigned int is_initialized;
    unsigned int fsbr_is_on;
    unsigned int fsbr_is_wanted;
    unsigned int fsbr_expiring;
    struct timer_list fsbr_timer;
    unsigned int oc_low;
    unsigned int wait_for_hp;
    unsigned int big_endian_mmio;
    unsigned int big_endian_desc;
    unsigned int is_aspeed;
    long unsigned int port_c_suspend;
    long unsigned int resuming_ports;
    long unsigned int ports_timeout;
    struct list_head idle_qh_list;
    int rh_numports;
    wait_queue_head_t waitqh;
    int num_waiting;
    int total_load;
    short int load[32];
    struct clk *clk;
    void (*reset_hc)(struct uhci_hcd *);
    int (*check_and_reset_hc)(struct uhci_hcd *);
    void (*configure_hc)(struct uhci_hcd *);
    int (*resume_detect_interrupts_are_broken)(struct uhci_hcd *);
    int (*global_suspend_mode_is_broken)(struct uhci_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct uhci_hcd {
    struct dentry *dentry;
    long unsigned int io_addr;
    void *regs;
    struct dma_pool *qh_pool;
    struct dma_pool *td_pool;
    struct uhci_td *term_td;
    struct uhci_qh * skelqh[11];
    struct uhci_qh *next_qh;
    spinlock_t lock;
    dma_addr_t frame_dma_handle;
    __le32 *frame;
    void **frame_cpu;
    enum uhci_rh_state rh_state;
    long unsigned int auto_stop_time;
    unsigned int frame_number;
    unsigned int is_stopped;
    unsigned int last_iso_frame;
    unsigned int cur_iso_frame;
    unsigned int scan_in_progress;
    unsigned int need_rescan;
    unsigned int dead;
    unsigned int RD_enable;
    unsigned int is_initialized;
    unsigned int fsbr_is_on;
    unsigned int fsbr_is_wanted;
    unsigned int fsbr_expiring;
    struct timer_list fsbr_timer;
    unsigned int oc_low;
    unsigned int wait_for_hp;
    unsigned int big_endian_mmio;
    unsigned int big_endian_desc;
    unsigned int is_aspeed;
    long unsigned int port_c_suspend;
    long unsigned int resuming_ports;
    long unsigned int ports_timeout;
    struct list_head idle_qh_list;
    int rh_numports;
    wait_queue_head_t waitqh;
    int num_waiting;
    int total_load;
    short int load[32];
    struct clk *clk;
    void (*reset_hc)(struct uhci_hcd *);
    int (*check_and_reset_hc)(struct uhci_hcd *);
    void (*configure_hc)(struct uhci_hcd *);
    int (*resume_detect_interrupts_are_broken)(struct uhci_hcd *);
    int (*global_suspend_mode_is_broken)(struct uhci_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct uhci_hcd {
    long unsigned int io_addr;
    void *regs;
    struct dma_pool *qh_pool;
    struct dma_pool *td_pool;
    struct uhci_td *term_td;
    struct uhci_qh * skelqh[11];
    struct uhci_qh *next_qh;
    spinlock_t lock;
    dma_addr_t frame_dma_handle;
    __le32 *frame;
    void **frame_cpu;
    enum uhci_rh_state rh_state;
    long unsigned int auto_stop_time;
    unsigned int frame_number;
    unsigned int is_stopped;
    unsigned int last_iso_frame;
    unsigned int cur_iso_frame;
    unsigned int scan_in_progress;
    unsigned int need_rescan;
    unsigned int dead;
    unsigned int RD_enable;
    unsigned int is_initialized;
    unsigned int fsbr_is_on;
    unsigned int fsbr_is_wanted;
    unsigned int fsbr_expiring;
    struct timer_list fsbr_timer;
    unsigned int oc_low;
    unsigned int wait_for_hp;
    unsigned int big_endian_mmio;
    unsigned int big_endian_desc;
    unsigned int is_aspeed;
    long unsigned int port_c_suspend;
    long unsigned int resuming_ports;
    long unsigned int ports_timeout;
    struct list_head idle_qh_list;
    int rh_numports;
    wait_queue_head_t waitqh;
    int num_waiting;
    int total_load;
    short int load[32];
    struct clk *clk;
    void (*reset_hc)(struct uhci_hcd *);
    int (*check_and_reset_hc)(struct uhci_hcd *);
    void (*configure_hc)(struct uhci_hcd *);
    int (*resume_detect_interrupts_are_broken)(struct uhci_hcd *);
    int (*global_suspend_mode_is_broken)(struct uhci_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct uhci_hcd {
    long unsigned int io_addr;
    void *regs;
    struct dma_pool *qh_pool;
    struct dma_pool *td_pool;
    struct uhci_td *term_td;
    struct uhci_qh * skelqh[11];
    struct uhci_qh *next_qh;
    spinlock_t lock;
    dma_addr_t frame_dma_handle;
    __le32 *frame;
    void **frame_cpu;
    enum uhci_rh_state rh_state;
    long unsigned int auto_stop_time;
    unsigned int frame_number;
    unsigned int is_stopped;
    unsigned int last_iso_frame;
    unsigned int cur_iso_frame;
    unsigned int scan_in_progress;
    unsigned int need_rescan;
    unsigned int dead;
    unsigned int RD_enable;
    unsigned int is_initialized;
    unsigned int fsbr_is_on;
    unsigned int fsbr_is_wanted;
    unsigned int fsbr_expiring;
    struct timer_list fsbr_timer;
    unsigned int oc_low;
    unsigned int wait_for_hp;
    unsigned int big_endian_mmio;
    unsigned int big_endian_desc;
    unsigned int is_aspeed;
    long unsigned int port_c_suspend;
    long unsigned int resuming_ports;
    long unsigned int ports_timeout;
    struct list_head idle_qh_list;
    int rh_numports;
    wait_queue_head_t waitqh;
    int num_waiting;
    int total_load;
    short int load[32];
    struct clk *clk;
    void (*reset_hc)(struct uhci_hcd *);
    int (*check_and_reset_hc)(struct uhci_hcd *);
    void (*configure_hc)(struct uhci_hcd *);
    int (*resume_detect_interrupts_are_broken)(struct uhci_hcd *);
    int (*global_suspend_mode_is_broken)(struct uhci_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct uhci_hcd {
    long unsigned int io_addr;
    void *regs;
    struct dma_pool *qh_pool;
    struct dma_pool *td_pool;
    struct uhci_td *term_td;
    struct uhci_qh * skelqh[11];
    struct uhci_qh *next_qh;
    spinlock_t lock;
    dma_addr_t frame_dma_handle;
    __le32 *frame;
    void **frame_cpu;
    enum uhci_rh_state rh_state;
    long unsigned int auto_stop_time;
    unsigned int frame_number;
    unsigned int is_stopped;
    unsigned int last_iso_frame;
    unsigned int cur_iso_frame;
    unsigned int scan_in_progress;
    unsigned int need_rescan;
    unsigned int dead;
    unsigned int RD_enable;
    unsigned int is_initialized;
    unsigned int fsbr_is_on;
    unsigned int fsbr_is_wanted;
    unsigned int fsbr_expiring;
    struct timer_list fsbr_timer;
    unsigned int oc_low;
    unsigned int wait_for_hp;
    unsigned int big_endian_mmio;
    unsigned int big_endian_desc;
    unsigned int is_aspeed;
    long unsigned int port_c_suspend;
    long unsigned int resuming_ports;
    long unsigned int ports_timeout;
    struct list_head idle_qh_list;
    int rh_numports;
    wait_queue_head_t waitqh;
    int num_waiting;
    int total_load;
    short int load[32];
    struct clk *clk;
    void (*reset_hc)(struct uhci_hcd *);
    int (*check_and_reset_hc)(struct uhci_hcd *);
    void (*configure_hc)(struct uhci_hcd *);
    int (*resume_detect_interrupts_are_broken)(struct uhci_hcd *);
    int (*global_suspend_mode_is_broken)(struct uhci_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct uhci_hcd {
    long unsigned int io_addr;
    void *regs;
    struct dma_pool *qh_pool;
    struct dma_pool *td_pool;
    struct uhci_td *term_td;
    struct uhci_qh * skelqh[11];
    struct uhci_qh *next_qh;
    spinlock_t lock;
    dma_addr_t frame_dma_handle;
    __le32 *frame;
    void **frame_cpu;
    enum uhci_rh_state rh_state;
    long unsigned int auto_stop_time;
    unsigned int frame_number;
    unsigned int is_stopped;
    unsigned int last_iso_frame;
    unsigned int cur_iso_frame;
    unsigned int scan_in_progress;
    unsigned int need_rescan;
    unsigned int dead;
    unsigned int RD_enable;
    unsigned int is_initialized;
    unsigned int fsbr_is_on;
    unsigned int fsbr_is_wanted;
    unsigned int fsbr_expiring;
    struct timer_list fsbr_timer;
    unsigned int oc_low;
    unsigned int wait_for_hp;
    unsigned int big_endian_mmio;
    unsigned int big_endian_desc;
    unsigned int is_aspeed;
    long unsigned int port_c_suspend;
    long unsigned int resuming_ports;
    long unsigned int ports_timeout;
    struct list_head idle_qh_list;
    int rh_numports;
    wait_queue_head_t waitqh;
    int num_waiting;
    int total_load;
    short int load[32];
    struct clk *clk;
    void (*reset_hc)(struct uhci_hcd *);
    int (*check_and_reset_hc)(struct uhci_hcd *);
    void (*configure_hc)(struct uhci_hcd *);
    int (*resume_detect_interrupts_are_broken)(struct uhci_hcd *);
    int (*global_suspend_mode_is_broken)(struct uhci_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct uhci_hcd {
    long unsigned int io_addr;
    void *regs;
    struct dma_pool *qh_pool;
    struct dma_pool *td_pool;
    struct uhci_td *term_td;
    struct uhci_qh * skelqh[11];
    struct uhci_qh *next_qh;
    spinlock_t lock;
    dma_addr_t frame_dma_handle;
    __le32 *frame;
    void **frame_cpu;
    enum uhci_rh_state rh_state;
    long unsigned int auto_stop_time;
    unsigned int frame_number;
    unsigned int is_stopped;
    unsigned int last_iso_frame;
    unsigned int cur_iso_frame;
    unsigned int scan_in_progress;
    unsigned int need_rescan;
    unsigned int dead;
    unsigned int RD_enable;
    unsigned int is_initialized;
    unsigned int fsbr_is_on;
    unsigned int fsbr_is_wanted;
    unsigned int fsbr_expiring;
    struct timer_list fsbr_timer;
    unsigned int oc_low;
    unsigned int wait_for_hp;
    unsigned int big_endian_mmio;
    unsigned int big_endian_desc;
    unsigned int is_aspeed;
    long unsigned int port_c_suspend;
    long unsigned int resuming_ports;
    long unsigned int ports_timeout;
    struct list_head idle_qh_list;
    int rh_numports;
    wait_queue_head_t waitqh;
    int num_waiting;
    int total_load;
    short int load[32];
    struct clk *clk;
    void (*reset_hc)(struct uhci_hcd *);
    int (*check_and_reset_hc)(struct uhci_hcd *);
    void (*configure_hc)(struct uhci_hcd *);
    int (*resume_detect_interrupts_are_broken)(struct uhci_hcd *);
    int (*global_suspend_mode_is_broken)(struct uhci_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct uhci_hcd {
    long unsigned int io_addr;
    void *regs;
    struct dma_pool *qh_pool;
    struct dma_pool *td_pool;
    struct uhci_td *term_td;
    struct uhci_qh * skelqh[11];
    struct uhci_qh *next_qh;
    spinlock_t lock;
    dma_addr_t frame_dma_handle;
    __le32 *frame;
    void **frame_cpu;
    enum uhci_rh_state rh_state;
    long unsigned int auto_stop_time;
    unsigned int frame_number;
    unsigned int is_stopped;
    unsigned int last_iso_frame;
    unsigned int cur_iso_frame;
    unsigned int scan_in_progress;
    unsigned int need_rescan;
    unsigned int dead;
    unsigned int RD_enable;
    unsigned int is_initialized;
    unsigned int fsbr_is_on;
    unsigned int fsbr_is_wanted;
    unsigned int fsbr_expiring;
    struct timer_list fsbr_timer;
    unsigned int oc_low;
    unsigned int wait_for_hp;
    unsigned int big_endian_mmio;
    unsigned int big_endian_desc;
    unsigned int is_aspeed;
    long unsigned int port_c_suspend;
    long unsigned int resuming_ports;
    long unsigned int ports_timeout;
    struct list_head idle_qh_list;
    int rh_numports;
    wait_queue_head_t waitqh;
    int num_waiting;
    int total_load;
    short int load[32];
    struct clk *clk;
    void (*reset_hc)(struct uhci_hcd *);
    int (*check_and_reset_hc)(struct uhci_hcd *);
    void (*configure_hc)(struct uhci_hcd *);
    int (*resume_detect_interrupts_are_broken)(struct uhci_hcd *);
    int (*global_suspend_mode_is_broken)(struct uhci_hcd *);
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
struct uhci_hcd {
    struct dentry *dentry;
    long unsigned int io_addr;
    void *regs;
    struct dma_pool *qh_pool;
    struct dma_pool *td_pool;
    struct uhci_td *term_td;
    struct uhci_qh * skelqh[11];
    struct uhci_qh *next_qh;
    spinlock_t lock;
    dma_addr_t frame_dma_handle;
    __le32 *frame;
    void **frame_cpu;
    enum uhci_rh_state rh_state;
    long unsigned int auto_stop_time;
    unsigned int frame_number;
    unsigned int is_stopped;
    unsigned int last_iso_frame;
    unsigned int cur_iso_frame;
    unsigned int scan_in_progress;
    unsigned int need_rescan;
    unsigned int dead;
    unsigned int RD_enable;
    unsigned int is_initialized;
    unsigned int fsbr_is_on;
    unsigned int fsbr_is_wanted;
    unsigned int fsbr_expiring;
    struct timer_list fsbr_timer;
    unsigned int oc_low;
    unsigned int wait_for_hp;
    unsigned int big_endian_mmio;
    unsigned int big_endian_desc;
    unsigned int is_aspeed;
    long unsigned int port_c_suspend;
    long unsigned int resuming_ports;
    long unsigned int ports_timeout;
    struct list_head idle_qh_list;
    int rh_numports;
    wait_queue_head_t waitqh;
    int num_waiting;
    int total_load;
    short int load[32];
    struct clk *clk;
    void (*reset_hc)(struct uhci_hcd *);
    int (*check_and_reset_hc)(struct uhci_hcd *);
    void (*configure_hc)(struct uhci_hcd *);
    int (*resume_detect_interrupts_are_broken)(struct uhci_hcd *);
    int (*global_suspend_mode_is_broken)(struct uhci_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct uhci_hcd {
    struct dentry *dentry;
    long unsigned int io_addr;
    void *regs;
    struct dma_pool *qh_pool;
    struct dma_pool *td_pool;
    struct uhci_td *term_td;
    struct uhci_qh * skelqh[11];
    struct uhci_qh *next_qh;
    spinlock_t lock;
    dma_addr_t frame_dma_handle;
    __le32 *frame;
    void **frame_cpu;
    enum uhci_rh_state rh_state;
    long unsigned int auto_stop_time;
    unsigned int frame_number;
    unsigned int is_stopped;
    unsigned int last_iso_frame;
    unsigned int cur_iso_frame;
    unsigned int scan_in_progress;
    unsigned int need_rescan;
    unsigned int dead;
    unsigned int RD_enable;
    unsigned int is_initialized;
    unsigned int fsbr_is_on;
    unsigned int fsbr_is_wanted;
    unsigned int fsbr_expiring;
    struct timer_list fsbr_timer;
    unsigned int oc_low;
    unsigned int wait_for_hp;
    unsigned int big_endian_mmio;
    unsigned int big_endian_desc;
    unsigned int is_aspeed;
    long unsigned int port_c_suspend;
    long unsigned int resuming_ports;
    long unsigned int ports_timeout;
    struct list_head idle_qh_list;
    int rh_numports;
    wait_queue_head_t waitqh;
    int num_waiting;
    int total_load;
    short int load[32];
    struct clk *clk;
    void (*reset_hc)(struct uhci_hcd *);
    int (*check_and_reset_hc)(struct uhci_hcd *);
    void (*configure_hc)(struct uhci_hcd *);
    int (*resume_detect_interrupts_are_broken)(struct uhci_hcd *);
    int (*global_suspend_mode_is_broken)(struct uhci_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct uhci_hcd {
    struct dentry *dentry;
    long unsigned int io_addr;
    void *regs;
    struct dma_pool *qh_pool;
    struct dma_pool *td_pool;
    struct uhci_td *term_td;
    struct uhci_qh * skelqh[11];
    struct uhci_qh *next_qh;
    spinlock_t lock;
    dma_addr_t frame_dma_handle;
    __le32 *frame;
    void **frame_cpu;
    enum uhci_rh_state rh_state;
    long unsigned int auto_stop_time;
    unsigned int frame_number;
    unsigned int is_stopped;
    unsigned int last_iso_frame;
    unsigned int cur_iso_frame;
    unsigned int scan_in_progress;
    unsigned int need_rescan;
    unsigned int dead;
    unsigned int RD_enable;
    unsigned int is_initialized;
    unsigned int fsbr_is_on;
    unsigned int fsbr_is_wanted;
    unsigned int fsbr_expiring;
    struct timer_list fsbr_timer;
    unsigned int oc_low;
    unsigned int wait_for_hp;
    unsigned int big_endian_mmio;
    unsigned int big_endian_desc;
    unsigned int is_aspeed;
    long unsigned int port_c_suspend;
    long unsigned int resuming_ports;
    long unsigned int ports_timeout;
    struct list_head idle_qh_list;
    int rh_numports;
    wait_queue_head_t waitqh;
    int num_waiting;
    int total_load;
    short int load[32];
    struct clk *clk;
    void (*reset_hc)(struct uhci_hcd *);
    int (*check_and_reset_hc)(struct uhci_hcd *);
    void (*configure_hc)(struct uhci_hcd *);
    int (*resume_detect_interrupts_are_broken)(struct uhci_hcd *);
    int (*global_suspend_mode_is_broken)(struct uhci_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct uhci_hcd {
    struct dentry *dentry;
    long unsigned int io_addr;
    void *regs;
    struct dma_pool *qh_pool;
    struct dma_pool *td_pool;
    struct uhci_td *term_td;
    struct uhci_qh * skelqh[11];
    struct uhci_qh *next_qh;
    spinlock_t lock;
    dma_addr_t frame_dma_handle;
    __le32 *frame;
    void **frame_cpu;
    enum uhci_rh_state rh_state;
    long unsigned int auto_stop_time;
    unsigned int frame_number;
    unsigned int is_stopped;
    unsigned int last_iso_frame;
    unsigned int cur_iso_frame;
    unsigned int scan_in_progress;
    unsigned int need_rescan;
    unsigned int dead;
    unsigned int RD_enable;
    unsigned int is_initialized;
    unsigned int fsbr_is_on;
    unsigned int fsbr_is_wanted;
    unsigned int fsbr_expiring;
    struct timer_list fsbr_timer;
    unsigned int oc_low;
    unsigned int wait_for_hp;
    unsigned int big_endian_mmio;
    unsigned int big_endian_desc;
    unsigned int is_aspeed;
    long unsigned int port_c_suspend;
    long unsigned int resuming_ports;
    long unsigned int ports_timeout;
    struct list_head idle_qh_list;
    int rh_numports;
    wait_queue_head_t waitqh;
    int num_waiting;
    int total_load;
    short int load[32];
    struct clk *clk;
    void (*reset_hc)(struct uhci_hcd *);
    int (*check_and_reset_hc)(struct uhci_hcd *);
    void (*configure_hc)(struct uhci_hcd *);
    int (*resume_detect_interrupts_are_broken)(struct uhci_hcd *);
    int (*global_suspend_mode_is_broken)(struct uhci_hcd *);
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
struct uhci_hcd {
    struct dentry *dentry;
    long unsigned int io_addr;
    void *regs;
    struct dma_pool *qh_pool;
    struct dma_pool *td_pool;
    struct uhci_td *term_td;
    struct uhci_qh * skelqh[11];
    struct uhci_qh *next_qh;
    spinlock_t lock;
    dma_addr_t frame_dma_handle;
    __le32 *frame;
    void **frame_cpu;
    enum uhci_rh_state rh_state;
    long unsigned int auto_stop_time;
    unsigned int frame_number;
    unsigned int is_stopped;
    unsigned int last_iso_frame;
    unsigned int cur_iso_frame;
    unsigned int scan_in_progress;
    unsigned int need_rescan;
    unsigned int dead;
    unsigned int RD_enable;
    unsigned int is_initialized;
    unsigned int fsbr_is_on;
    unsigned int fsbr_is_wanted;
    unsigned int fsbr_expiring;
    struct timer_list fsbr_timer;
    unsigned int oc_low;
    unsigned int wait_for_hp;
    unsigned int big_endian_mmio;
    unsigned int big_endian_desc;
    unsigned int is_aspeed;
    long unsigned int port_c_suspend;
    long unsigned int resuming_ports;
    long unsigned int ports_timeout;
    struct list_head idle_qh_list;
    int rh_numports;
    wait_queue_head_t waitqh;
    int num_waiting;
    int total_load;
    short int load[32];
    struct clk *clk;
    void (*reset_hc)(struct uhci_hcd *);
    int (*check_and_reset_hc)(struct uhci_hcd *);
    void (*configure_hc)(struct uhci_hcd *);
    int (*resume_detect_interrupts_are_broken)(struct uhci_hcd *);
    int (*global_suspend_mode_is_broken)(struct uhci_hcd *);
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
struct uhci_hcd {
    struct dentry *dentry;
    long unsigned int io_addr;
    void *regs;
    struct dma_pool *qh_pool;
    struct dma_pool *td_pool;
    struct uhci_td *term_td;
    struct uhci_qh * skelqh[11];
    struct uhci_qh *next_qh;
    spinlock_t lock;
    dma_addr_t frame_dma_handle;
    __le32 *frame;
    void **frame_cpu;
    enum uhci_rh_state rh_state;
    long unsigned int auto_stop_time;
    unsigned int frame_number;
    unsigned int is_stopped;
    unsigned int last_iso_frame;
    unsigned int cur_iso_frame;
    unsigned int scan_in_progress;
    unsigned int need_rescan;
    unsigned int dead;
    unsigned int RD_enable;
    unsigned int is_initialized;
    unsigned int fsbr_is_on;
    unsigned int fsbr_is_wanted;
    unsigned int fsbr_expiring;
    struct timer_list fsbr_timer;
    unsigned int oc_low;
    unsigned int wait_for_hp;
    unsigned int big_endian_mmio;
    unsigned int big_endian_desc;
    unsigned int is_aspeed;
    long unsigned int port_c_suspend;
    long unsigned int resuming_ports;
    long unsigned int ports_timeout;
    struct list_head idle_qh_list;
    int rh_numports;
    wait_queue_head_t waitqh;
    int num_waiting;
    int total_load;
    short int load[32];
    struct clk *clk;
    void (*reset_hc)(struct uhci_hcd *);
    int (*check_and_reset_hc)(struct uhci_hcd *);
    void (*configure_hc)(struct uhci_hcd *);
    int (*resume_detect_interrupts_are_broken)(struct uhci_hcd *);
    int (*global_suspend_mode_is_broken)(struct uhci_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct uhci_hcd {
    struct dentry *dentry;
    long unsigned int io_addr;
    void *regs;
    struct dma_pool *qh_pool;
    struct dma_pool *td_pool;
    struct uhci_td *term_td;
    struct uhci_qh * skelqh[11];
    struct uhci_qh *next_qh;
    spinlock_t lock;
    dma_addr_t frame_dma_handle;
    __le32 *frame;
    void **frame_cpu;
    enum uhci_rh_state rh_state;
    long unsigned int auto_stop_time;
    unsigned int frame_number;
    unsigned int is_stopped;
    unsigned int last_iso_frame;
    unsigned int cur_iso_frame;
    unsigned int scan_in_progress;
    unsigned int need_rescan;
    unsigned int dead;
    unsigned int RD_enable;
    unsigned int is_initialized;
    unsigned int fsbr_is_on;
    unsigned int fsbr_is_wanted;
    unsigned int fsbr_expiring;
    struct timer_list fsbr_timer;
    unsigned int oc_low;
    unsigned int wait_for_hp;
    unsigned int big_endian_mmio;
    unsigned int big_endian_desc;
    unsigned int is_aspeed;
    long unsigned int port_c_suspend;
    long unsigned int resuming_ports;
    long unsigned int ports_timeout;
    struct list_head idle_qh_list;
    int rh_numports;
    wait_queue_head_t waitqh;
    int num_waiting;
    int total_load;
    short int load[32];
    struct clk *clk;
    void (*reset_hc)(struct uhci_hcd *);
    int (*check_and_reset_hc)(struct uhci_hcd *);
    void (*configure_hc)(struct uhci_hcd *);
    int (*resume_detect_interrupts_are_broken)(struct uhci_hcd *);
    int (*global_suspend_mode_is_broken)(struct uhci_hcd *);
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
<b>Field added. </b>
<code>unsigned int is_aspeed</code>
</li>
</ul>
</details>
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
<code>struct clk *clk</code>
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
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct dentry *dentry</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct clk *clk</code> ➡️ <code>struct clk *clk</code>
</li>
</ul>
</details>
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
