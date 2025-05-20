# Struct: <code>ohci_hcd</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct ohci_hcd {
    spinlock_t lock;
    struct ohci_regs *regs;
    struct ohci_hcca *hcca;
    dma_addr_t hcca_dma;
    struct ed *ed_rm_list;
    struct ed *ed_bulktail;
    struct ed *ed_controltail;
    struct ed * periodic[32];
    void (*start_hnp)(struct ohci_hcd *);
    struct dma_pool *td_cache;
    struct dma_pool *ed_cache;
    struct td * td_hash[64];
    struct td *dl_start;
    struct td *dl_end;
    struct list_head pending;
    struct list_head eds_in_use;
    enum ohci_rh_state rh_state;
    int num_ports;
    int load[32];
    u32 hc_control;
    long unsigned int next_statechange;
    u32 fminterval;
    unsigned int autostop;
    unsigned int working;
    unsigned int restart_work;
    long unsigned int flags;
    unsigned int prev_frame_no;
    unsigned int wdh_cnt;
    unsigned int prev_wdh_cnt;
    u32 prev_donehead;
    struct timer_list io_watchdog;
    struct work_struct nec_work;
    struct dentry *debug_dir;
    struct dentry *debug_async;
    struct dentry *debug_periodic;
    struct dentry *debug_registers;
    long unsigned int priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ohci_hcd {
    spinlock_t lock;
    struct ohci_regs *regs;
    struct ohci_hcca *hcca;
    dma_addr_t hcca_dma;
    struct ed *ed_rm_list;
    struct ed *ed_bulktail;
    struct ed *ed_controltail;
    struct ed * periodic[32];
    void (*start_hnp)(struct ohci_hcd *);
    struct dma_pool *td_cache;
    struct dma_pool *ed_cache;
    struct td * td_hash[64];
    struct td *dl_start;
    struct td *dl_end;
    struct list_head pending;
    struct list_head eds_in_use;
    enum ohci_rh_state rh_state;
    int num_ports;
    int load[32];
    u32 hc_control;
    long unsigned int next_statechange;
    u32 fminterval;
    unsigned int autostop;
    unsigned int working;
    unsigned int restart_work;
    long unsigned int flags;
    unsigned int prev_frame_no;
    unsigned int wdh_cnt;
    unsigned int prev_wdh_cnt;
    u32 prev_donehead;
    struct timer_list io_watchdog;
    struct work_struct nec_work;
    struct dentry *debug_dir;
    struct dentry *debug_async;
    struct dentry *debug_periodic;
    struct dentry *debug_registers;
    long unsigned int priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ohci_hcd {
    spinlock_t lock;
    struct ohci_regs *regs;
    struct ohci_hcca *hcca;
    dma_addr_t hcca_dma;
    struct ed *ed_rm_list;
    struct ed *ed_bulktail;
    struct ed *ed_controltail;
    struct ed * periodic[32];
    void (*start_hnp)(struct ohci_hcd *);
    struct dma_pool *td_cache;
    struct dma_pool *ed_cache;
    struct td * td_hash[64];
    struct td *dl_start;
    struct td *dl_end;
    struct list_head pending;
    struct list_head eds_in_use;
    enum ohci_rh_state rh_state;
    int num_ports;
    int load[32];
    u32 hc_control;
    long unsigned int next_statechange;
    u32 fminterval;
    unsigned int autostop;
    unsigned int working;
    unsigned int restart_work;
    long unsigned int flags;
    unsigned int prev_frame_no;
    unsigned int wdh_cnt;
    unsigned int prev_wdh_cnt;
    u32 prev_donehead;
    struct timer_list io_watchdog;
    struct work_struct nec_work;
    struct dentry *debug_dir;
    struct dentry *debug_async;
    struct dentry *debug_periodic;
    struct dentry *debug_registers;
    long unsigned int priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ohci_hcd {
    spinlock_t lock;
    struct ohci_regs *regs;
    struct ohci_hcca *hcca;
    dma_addr_t hcca_dma;
    struct ed *ed_rm_list;
    struct ed *ed_bulktail;
    struct ed *ed_controltail;
    struct ed * periodic[32];
    void (*start_hnp)(struct ohci_hcd *);
    struct dma_pool *td_cache;
    struct dma_pool *ed_cache;
    struct td * td_hash[64];
    struct td *dl_start;
    struct td *dl_end;
    struct list_head pending;
    struct list_head eds_in_use;
    enum ohci_rh_state rh_state;
    int num_ports;
    int load[32];
    u32 hc_control;
    long unsigned int next_statechange;
    u32 fminterval;
    unsigned int autostop;
    unsigned int working;
    unsigned int restart_work;
    long unsigned int flags;
    unsigned int prev_frame_no;
    unsigned int wdh_cnt;
    unsigned int prev_wdh_cnt;
    u32 prev_donehead;
    struct timer_list io_watchdog;
    struct work_struct nec_work;
    struct dentry *debug_dir;
    struct dentry *debug_async;
    struct dentry *debug_periodic;
    struct dentry *debug_registers;
    long unsigned int priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ohci_hcd {
    spinlock_t lock;
    struct ohci_regs *regs;
    struct ohci_hcca *hcca;
    dma_addr_t hcca_dma;
    struct ed *ed_rm_list;
    struct ed *ed_bulktail;
    struct ed *ed_controltail;
    struct ed * periodic[32];
    void (*start_hnp)(struct ohci_hcd *);
    struct dma_pool *td_cache;
    struct dma_pool *ed_cache;
    struct td * td_hash[64];
    struct td *dl_start;
    struct td *dl_end;
    struct list_head pending;
    struct list_head eds_in_use;
    enum ohci_rh_state rh_state;
    int num_ports;
    int load[32];
    u32 hc_control;
    long unsigned int next_statechange;
    u32 fminterval;
    unsigned int autostop;
    unsigned int working;
    unsigned int restart_work;
    long unsigned int flags;
    unsigned int prev_frame_no;
    unsigned int wdh_cnt;
    unsigned int prev_wdh_cnt;
    u32 prev_donehead;
    struct timer_list io_watchdog;
    struct work_struct nec_work;
    struct dentry *debug_dir;
    struct dentry *debug_async;
    struct dentry *debug_periodic;
    struct dentry *debug_registers;
    long unsigned int priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ohci_hcd {
    spinlock_t lock;
    struct ohci_regs *regs;
    struct ohci_hcca *hcca;
    dma_addr_t hcca_dma;
    struct ed *ed_rm_list;
    struct ed *ed_bulktail;
    struct ed *ed_controltail;
    struct ed * periodic[32];
    void (*start_hnp)(struct ohci_hcd *);
    struct dma_pool *td_cache;
    struct dma_pool *ed_cache;
    struct td * td_hash[64];
    struct td *dl_start;
    struct td *dl_end;
    struct list_head pending;
    struct list_head eds_in_use;
    enum ohci_rh_state rh_state;
    int num_ports;
    int load[32];
    u32 hc_control;
    long unsigned int next_statechange;
    u32 fminterval;
    unsigned int autostop;
    unsigned int working;
    unsigned int restart_work;
    long unsigned int flags;
    unsigned int prev_frame_no;
    unsigned int wdh_cnt;
    unsigned int prev_wdh_cnt;
    u32 prev_donehead;
    struct timer_list io_watchdog;
    struct work_struct nec_work;
    struct dentry *debug_dir;
    long unsigned int priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ohci_hcd {
    spinlock_t lock;
    struct ohci_regs *regs;
    struct ohci_hcca *hcca;
    dma_addr_t hcca_dma;
    struct ed *ed_rm_list;
    struct ed *ed_bulktail;
    struct ed *ed_controltail;
    struct ed * periodic[32];
    void (*start_hnp)(struct ohci_hcd *);
    struct dma_pool *td_cache;
    struct dma_pool *ed_cache;
    struct td * td_hash[64];
    struct td *dl_start;
    struct td *dl_end;
    struct list_head pending;
    struct list_head eds_in_use;
    enum ohci_rh_state rh_state;
    int num_ports;
    int load[32];
    u32 hc_control;
    long unsigned int next_statechange;
    u32 fminterval;
    unsigned int autostop;
    unsigned int working;
    unsigned int restart_work;
    long unsigned int flags;
    unsigned int prev_frame_no;
    unsigned int wdh_cnt;
    unsigned int prev_wdh_cnt;
    u32 prev_donehead;
    struct timer_list io_watchdog;
    struct work_struct nec_work;
    struct dentry *debug_dir;
    long unsigned int priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ohci_hcd {
    spinlock_t lock;
    struct ohci_regs *regs;
    struct ohci_hcca *hcca;
    dma_addr_t hcca_dma;
    struct ed *ed_rm_list;
    struct ed *ed_bulktail;
    struct ed *ed_controltail;
    struct ed * periodic[32];
    void (*start_hnp)(struct ohci_hcd *);
    struct dma_pool *td_cache;
    struct dma_pool *ed_cache;
    struct td * td_hash[64];
    struct td *dl_start;
    struct td *dl_end;
    struct list_head pending;
    struct list_head eds_in_use;
    enum ohci_rh_state rh_state;
    int num_ports;
    int load[32];
    u32 hc_control;
    long unsigned int next_statechange;
    u32 fminterval;
    unsigned int autostop;
    unsigned int working;
    unsigned int restart_work;
    long unsigned int flags;
    unsigned int prev_frame_no;
    unsigned int wdh_cnt;
    unsigned int prev_wdh_cnt;
    u32 prev_donehead;
    struct timer_list io_watchdog;
    struct work_struct nec_work;
    struct dentry *debug_dir;
    long unsigned int priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ohci_hcd {
    spinlock_t lock;
    struct ohci_regs *regs;
    struct ohci_hcca *hcca;
    dma_addr_t hcca_dma;
    struct ed *ed_rm_list;
    struct ed *ed_bulktail;
    struct ed *ed_controltail;
    struct ed * periodic[32];
    void (*start_hnp)(struct ohci_hcd *);
    struct dma_pool *td_cache;
    struct dma_pool *ed_cache;
    struct td * td_hash[64];
    struct td *dl_start;
    struct td *dl_end;
    struct list_head pending;
    struct list_head eds_in_use;
    enum ohci_rh_state rh_state;
    int num_ports;
    int load[32];
    u32 hc_control;
    long unsigned int next_statechange;
    u32 fminterval;
    unsigned int autostop;
    unsigned int working;
    unsigned int restart_work;
    long unsigned int flags;
    unsigned int prev_frame_no;
    unsigned int wdh_cnt;
    unsigned int prev_wdh_cnt;
    u32 prev_donehead;
    struct timer_list io_watchdog;
    struct work_struct nec_work;
    struct dentry *debug_dir;
    long unsigned int priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ohci_hcd {
    spinlock_t lock;
    struct ohci_regs *regs;
    struct ohci_hcca *hcca;
    dma_addr_t hcca_dma;
    struct ed *ed_rm_list;
    struct ed *ed_bulktail;
    struct ed *ed_controltail;
    struct ed * periodic[32];
    void (*start_hnp)(struct ohci_hcd *);
    struct dma_pool *td_cache;
    struct dma_pool *ed_cache;
    struct td * td_hash[64];
    struct td *dl_start;
    struct td *dl_end;
    struct list_head pending;
    struct list_head eds_in_use;
    enum ohci_rh_state rh_state;
    int num_ports;
    int load[32];
    u32 hc_control;
    long unsigned int next_statechange;
    u32 fminterval;
    unsigned int autostop;
    unsigned int working;
    unsigned int restart_work;
    long unsigned int flags;
    unsigned int prev_frame_no;
    unsigned int wdh_cnt;
    unsigned int prev_wdh_cnt;
    u32 prev_donehead;
    struct timer_list io_watchdog;
    struct work_struct nec_work;
    struct dentry *debug_dir;
    long unsigned int priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ohci_hcd {
    spinlock_t lock;
    struct ohci_regs *regs;
    struct ohci_hcca *hcca;
    dma_addr_t hcca_dma;
    struct ed *ed_rm_list;
    struct ed *ed_bulktail;
    struct ed *ed_controltail;
    struct ed * periodic[32];
    void (*start_hnp)(struct ohci_hcd *);
    struct dma_pool *td_cache;
    struct dma_pool *ed_cache;
    struct td * td_hash[64];
    struct td *dl_start;
    struct td *dl_end;
    struct list_head pending;
    struct list_head eds_in_use;
    enum ohci_rh_state rh_state;
    int num_ports;
    int load[32];
    u32 hc_control;
    long unsigned int next_statechange;
    u32 fminterval;
    unsigned int autostop;
    unsigned int working;
    unsigned int restart_work;
    long unsigned int flags;
    unsigned int prev_frame_no;
    unsigned int wdh_cnt;
    unsigned int prev_wdh_cnt;
    u32 prev_donehead;
    struct timer_list io_watchdog;
    struct work_struct nec_work;
    struct dentry *debug_dir;
    long unsigned int priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ohci_hcd {
    spinlock_t lock;
    struct ohci_regs *regs;
    struct ohci_hcca *hcca;
    dma_addr_t hcca_dma;
    struct ed *ed_rm_list;
    struct ed *ed_bulktail;
    struct ed *ed_controltail;
    struct ed * periodic[32];
    void (*start_hnp)(struct ohci_hcd *);
    struct dma_pool *td_cache;
    struct dma_pool *ed_cache;
    struct td * td_hash[64];
    struct td *dl_start;
    struct td *dl_end;
    struct list_head pending;
    struct list_head eds_in_use;
    enum ohci_rh_state rh_state;
    int num_ports;
    int load[32];
    u32 hc_control;
    long unsigned int next_statechange;
    u32 fminterval;
    unsigned int autostop;
    unsigned int working;
    unsigned int restart_work;
    long unsigned int flags;
    unsigned int prev_frame_no;
    unsigned int wdh_cnt;
    unsigned int prev_wdh_cnt;
    u32 prev_donehead;
    struct timer_list io_watchdog;
    struct work_struct nec_work;
    struct dentry *debug_dir;
    long unsigned int priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ohci_hcd {
    spinlock_t lock;
    struct ohci_regs *regs;
    struct ohci_hcca *hcca;
    dma_addr_t hcca_dma;
    struct ed *ed_rm_list;
    struct ed *ed_bulktail;
    struct ed *ed_controltail;
    struct ed * periodic[32];
    void (*start_hnp)(struct ohci_hcd *);
    struct dma_pool *td_cache;
    struct dma_pool *ed_cache;
    struct td * td_hash[64];
    struct td *dl_start;
    struct td *dl_end;
    struct list_head pending;
    struct list_head eds_in_use;
    enum ohci_rh_state rh_state;
    int num_ports;
    int load[32];
    u32 hc_control;
    long unsigned int next_statechange;
    u32 fminterval;
    unsigned int autostop;
    unsigned int working;
    unsigned int restart_work;
    long unsigned int flags;
    unsigned int prev_frame_no;
    unsigned int wdh_cnt;
    unsigned int prev_wdh_cnt;
    u32 prev_donehead;
    struct timer_list io_watchdog;
    struct work_struct nec_work;
    struct dentry *debug_dir;
    long unsigned int priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ohci_hcd {
    spinlock_t lock;
    struct ohci_regs *regs;
    struct ohci_hcca *hcca;
    dma_addr_t hcca_dma;
    struct ed *ed_rm_list;
    struct ed *ed_bulktail;
    struct ed *ed_controltail;
    struct ed * periodic[32];
    void (*start_hnp)(struct ohci_hcd *);
    struct dma_pool *td_cache;
    struct dma_pool *ed_cache;
    struct td * td_hash[64];
    struct td *dl_start;
    struct td *dl_end;
    struct list_head pending;
    struct list_head eds_in_use;
    enum ohci_rh_state rh_state;
    int num_ports;
    int load[32];
    u32 hc_control;
    long unsigned int next_statechange;
    u32 fminterval;
    unsigned int autostop;
    unsigned int working;
    unsigned int restart_work;
    long unsigned int flags;
    unsigned int prev_frame_no;
    unsigned int wdh_cnt;
    unsigned int prev_wdh_cnt;
    u32 prev_donehead;
    struct timer_list io_watchdog;
    struct work_struct nec_work;
    struct dentry *debug_dir;
    long unsigned int priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ohci_hcd {
    spinlock_t lock;
    struct ohci_regs *regs;
    struct ohci_hcca *hcca;
    dma_addr_t hcca_dma;
    struct ed *ed_rm_list;
    struct ed *ed_bulktail;
    struct ed *ed_controltail;
    struct ed * periodic[32];
    void (*start_hnp)(struct ohci_hcd *);
    struct dma_pool *td_cache;
    struct dma_pool *ed_cache;
    struct td * td_hash[64];
    struct td *dl_start;
    struct td *dl_end;
    struct list_head pending;
    struct list_head eds_in_use;
    enum ohci_rh_state rh_state;
    int num_ports;
    int load[32];
    u32 hc_control;
    long unsigned int next_statechange;
    u32 fminterval;
    unsigned int autostop;
    unsigned int working;
    unsigned int restart_work;
    long unsigned int flags;
    unsigned int prev_frame_no;
    unsigned int wdh_cnt;
    unsigned int prev_wdh_cnt;
    u32 prev_donehead;
    struct timer_list io_watchdog;
    struct work_struct nec_work;
    struct dentry *debug_dir;
    long unsigned int priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ohci_hcd {
    spinlock_t lock;
    struct ohci_regs *regs;
    struct ohci_hcca *hcca;
    dma_addr_t hcca_dma;
    struct ed *ed_rm_list;
    struct ed *ed_bulktail;
    struct ed *ed_controltail;
    struct ed * periodic[32];
    void (*start_hnp)(struct ohci_hcd *);
    struct dma_pool *td_cache;
    struct dma_pool *ed_cache;
    struct td * td_hash[64];
    struct td *dl_start;
    struct td *dl_end;
    struct list_head pending;
    struct list_head eds_in_use;
    enum ohci_rh_state rh_state;
    int num_ports;
    int load[32];
    u32 hc_control;
    long unsigned int next_statechange;
    u32 fminterval;
    unsigned int autostop;
    unsigned int working;
    unsigned int restart_work;
    long unsigned int flags;
    unsigned int prev_frame_no;
    unsigned int wdh_cnt;
    unsigned int prev_wdh_cnt;
    u32 prev_donehead;
    struct timer_list io_watchdog;
    struct work_struct nec_work;
    struct dentry *debug_dir;
    long unsigned int priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ohci_hcd {
    spinlock_t lock;
    struct ohci_regs *regs;
    struct ohci_hcca *hcca;
    dma_addr_t hcca_dma;
    struct ed *ed_rm_list;
    struct ed *ed_bulktail;
    struct ed *ed_controltail;
    struct ed * periodic[32];
    void (*start_hnp)(struct ohci_hcd *);
    struct dma_pool *td_cache;
    struct dma_pool *ed_cache;
    struct td * td_hash[64];
    struct td *dl_start;
    struct td *dl_end;
    struct list_head pending;
    struct list_head eds_in_use;
    enum ohci_rh_state rh_state;
    int num_ports;
    int load[32];
    u32 hc_control;
    long unsigned int next_statechange;
    u32 fminterval;
    unsigned int autostop;
    unsigned int working;
    unsigned int restart_work;
    long unsigned int flags;
    unsigned int prev_frame_no;
    unsigned int wdh_cnt;
    unsigned int prev_wdh_cnt;
    u32 prev_donehead;
    struct timer_list io_watchdog;
    struct work_struct nec_work;
    struct dentry *debug_dir;
    long unsigned int priv[0];
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
struct ohci_hcd {
    spinlock_t lock;
    struct ohci_regs *regs;
    struct ohci_hcca *hcca;
    dma_addr_t hcca_dma;
    struct ed *ed_rm_list;
    struct ed *ed_bulktail;
    struct ed *ed_controltail;
    struct ed * periodic[32];
    void (*start_hnp)(struct ohci_hcd *);
    struct dma_pool *td_cache;
    struct dma_pool *ed_cache;
    struct td * td_hash[64];
    struct td *dl_start;
    struct td *dl_end;
    struct list_head pending;
    struct list_head eds_in_use;
    enum ohci_rh_state rh_state;
    int num_ports;
    int load[32];
    u32 hc_control;
    long unsigned int next_statechange;
    u32 fminterval;
    unsigned int autostop;
    unsigned int working;
    unsigned int restart_work;
    long unsigned int flags;
    unsigned int prev_frame_no;
    unsigned int wdh_cnt;
    unsigned int prev_wdh_cnt;
    u32 prev_donehead;
    struct timer_list io_watchdog;
    struct work_struct nec_work;
    struct dentry *debug_dir;
    long unsigned int priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ohci_hcd {
    spinlock_t lock;
    struct ohci_regs *regs;
    struct ohci_hcca *hcca;
    dma_addr_t hcca_dma;
    struct ed *ed_rm_list;
    struct ed *ed_bulktail;
    struct ed *ed_controltail;
    struct ed * periodic[32];
    void (*start_hnp)(struct ohci_hcd *);
    struct dma_pool *td_cache;
    struct dma_pool *ed_cache;
    struct td * td_hash[64];
    struct td *dl_start;
    struct td *dl_end;
    struct list_head pending;
    struct list_head eds_in_use;
    enum ohci_rh_state rh_state;
    int num_ports;
    int load[32];
    u32 hc_control;
    long unsigned int next_statechange;
    u32 fminterval;
    unsigned int autostop;
    unsigned int working;
    unsigned int restart_work;
    long unsigned int flags;
    unsigned int prev_frame_no;
    unsigned int wdh_cnt;
    unsigned int prev_wdh_cnt;
    u32 prev_donehead;
    struct timer_list io_watchdog;
    struct work_struct nec_work;
    struct dentry *debug_dir;
    long unsigned int priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ohci_hcd {
    spinlock_t lock;
    struct ohci_regs *regs;
    struct ohci_hcca *hcca;
    dma_addr_t hcca_dma;
    struct ed *ed_rm_list;
    struct ed *ed_bulktail;
    struct ed *ed_controltail;
    struct ed * periodic[32];
    void (*start_hnp)(struct ohci_hcd *);
    struct dma_pool *td_cache;
    struct dma_pool *ed_cache;
    struct td * td_hash[64];
    struct td *dl_start;
    struct td *dl_end;
    struct list_head pending;
    struct list_head eds_in_use;
    enum ohci_rh_state rh_state;
    int num_ports;
    int load[32];
    u32 hc_control;
    long unsigned int next_statechange;
    u32 fminterval;
    unsigned int autostop;
    unsigned int working;
    unsigned int restart_work;
    long unsigned int flags;
    unsigned int prev_frame_no;
    unsigned int wdh_cnt;
    unsigned int prev_wdh_cnt;
    u32 prev_donehead;
    struct timer_list io_watchdog;
    struct work_struct nec_work;
    struct dentry *debug_dir;
    long unsigned int priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ohci_hcd {
    spinlock_t lock;
    struct ohci_regs *regs;
    struct ohci_hcca *hcca;
    dma_addr_t hcca_dma;
    struct ed *ed_rm_list;
    struct ed *ed_bulktail;
    struct ed *ed_controltail;
    struct ed * periodic[32];
    void (*start_hnp)(struct ohci_hcd *);
    struct dma_pool *td_cache;
    struct dma_pool *ed_cache;
    struct td * td_hash[64];
    struct td *dl_start;
    struct td *dl_end;
    struct list_head pending;
    struct list_head eds_in_use;
    enum ohci_rh_state rh_state;
    int num_ports;
    int load[32];
    u32 hc_control;
    long unsigned int next_statechange;
    u32 fminterval;
    unsigned int autostop;
    unsigned int working;
    unsigned int restart_work;
    long unsigned int flags;
    unsigned int prev_frame_no;
    unsigned int wdh_cnt;
    unsigned int prev_wdh_cnt;
    u32 prev_donehead;
    struct timer_list io_watchdog;
    struct work_struct nec_work;
    struct dentry *debug_dir;
    long unsigned int priv[0];
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
struct ohci_hcd {
    spinlock_t lock;
    struct ohci_regs *regs;
    struct ohci_hcca *hcca;
    dma_addr_t hcca_dma;
    struct ed *ed_rm_list;
    struct ed *ed_bulktail;
    struct ed *ed_controltail;
    struct ed * periodic[32];
    void (*start_hnp)(struct ohci_hcd *);
    struct dma_pool *td_cache;
    struct dma_pool *ed_cache;
    struct td * td_hash[64];
    struct td *dl_start;
    struct td *dl_end;
    struct list_head pending;
    struct list_head eds_in_use;
    enum ohci_rh_state rh_state;
    int num_ports;
    int load[32];
    u32 hc_control;
    long unsigned int next_statechange;
    u32 fminterval;
    unsigned int autostop;
    unsigned int working;
    unsigned int restart_work;
    long unsigned int flags;
    unsigned int prev_frame_no;
    unsigned int wdh_cnt;
    unsigned int prev_wdh_cnt;
    u32 prev_donehead;
    struct timer_list io_watchdog;
    struct work_struct nec_work;
    struct dentry *debug_dir;
    long unsigned int priv[0];
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
struct ohci_hcd {
    spinlock_t lock;
    struct ohci_regs *regs;
    struct ohci_hcca *hcca;
    dma_addr_t hcca_dma;
    struct ed *ed_rm_list;
    struct ed *ed_bulktail;
    struct ed *ed_controltail;
    struct ed * periodic[32];
    void (*start_hnp)(struct ohci_hcd *);
    struct dma_pool *td_cache;
    struct dma_pool *ed_cache;
    struct td * td_hash[64];
    struct td *dl_start;
    struct td *dl_end;
    struct list_head pending;
    struct list_head eds_in_use;
    enum ohci_rh_state rh_state;
    int num_ports;
    int load[32];
    u32 hc_control;
    long unsigned int next_statechange;
    u32 fminterval;
    unsigned int autostop;
    unsigned int working;
    unsigned int restart_work;
    long unsigned int flags;
    unsigned int prev_frame_no;
    unsigned int wdh_cnt;
    unsigned int prev_wdh_cnt;
    u32 prev_donehead;
    struct timer_list io_watchdog;
    struct work_struct nec_work;
    struct dentry *debug_dir;
    long unsigned int priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ohci_hcd {
    spinlock_t lock;
    struct ohci_regs *regs;
    struct ohci_hcca *hcca;
    dma_addr_t hcca_dma;
    struct ed *ed_rm_list;
    struct ed *ed_bulktail;
    struct ed *ed_controltail;
    struct ed * periodic[32];
    void (*start_hnp)(struct ohci_hcd *);
    struct dma_pool *td_cache;
    struct dma_pool *ed_cache;
    struct td * td_hash[64];
    struct td *dl_start;
    struct td *dl_end;
    struct list_head pending;
    struct list_head eds_in_use;
    enum ohci_rh_state rh_state;
    int num_ports;
    int load[32];
    u32 hc_control;
    long unsigned int next_statechange;
    u32 fminterval;
    unsigned int autostop;
    unsigned int working;
    unsigned int restart_work;
    long unsigned int flags;
    unsigned int prev_frame_no;
    unsigned int wdh_cnt;
    unsigned int prev_wdh_cnt;
    u32 prev_donehead;
    struct timer_list io_watchdog;
    struct work_struct nec_work;
    struct dentry *debug_dir;
    long unsigned int priv[0];
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
<b>Field removed. </b>
<code>struct dentry *debug_async</code>
</li>
<li>
<b>Field removed. </b>
<code>struct dentry *debug_periodic</code>
</li>
<li>
<b>Field removed. </b>
<code>struct dentry *debug_registers</code>
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
