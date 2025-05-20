# Struct: <code>dw_i2c_dev</code>

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
struct dw_i2c_dev {
    struct device *dev;
    void *base;
    struct completion cmd_complete;
    struct clk *clk;
    struct reset_control *rst;
    struct i2c_client *slave;
    u32 (*get_clk_rate_khz)(struct dw_i2c_dev *);
    struct dw_pci_controller *controller;
    int cmd_err;
    struct i2c_msg *msgs;
    int msgs_num;
    int msg_write_idx;
    u32 tx_buf_len;
    u8 *tx_buf;
    int msg_read_idx;
    u32 rx_buf_len;
    u8 *rx_buf;
    int msg_err;
    unsigned int status;
    u32 abort_source;
    int irq;
    u32 flags;
    struct i2c_adapter adapter;
    u32 functionality;
    u32 master_cfg;
    u32 slave_cfg;
    unsigned int tx_fifo_depth;
    unsigned int rx_fifo_depth;
    int rx_outstanding;
    u32 clk_freq;
    u32 sda_hold_time;
    u32 sda_falling_time;
    u32 scl_falling_time;
    u16 ss_hcnt;
    u16 ss_lcnt;
    u16 fs_hcnt;
    u16 fs_lcnt;
    u16 fp_hcnt;
    u16 fp_lcnt;
    u16 hs_hcnt;
    u16 hs_lcnt;
    struct pm_qos_request pm_qos;
    int (*acquire_lock)(struct dw_i2c_dev *);
    void (*release_lock)(struct dw_i2c_dev *);
    bool pm_disabled;
    void (*disable)(struct dw_i2c_dev *);
    void (*disable_int)(struct dw_i2c_dev *);
    int (*init)(struct dw_i2c_dev *);
    int mode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dw_i2c_dev {
    struct device *dev;
    void *base;
    struct completion cmd_complete;
    struct clk *clk;
    struct reset_control *rst;
    struct i2c_client *slave;
    u32 (*get_clk_rate_khz)(struct dw_i2c_dev *);
    struct dw_pci_controller *controller;
    int cmd_err;
    struct i2c_msg *msgs;
    int msgs_num;
    int msg_write_idx;
    u32 tx_buf_len;
    u8 *tx_buf;
    int msg_read_idx;
    u32 rx_buf_len;
    u8 *rx_buf;
    int msg_err;
    unsigned int status;
    u32 abort_source;
    int irq;
    u32 flags;
    struct i2c_adapter adapter;
    u32 functionality;
    u32 master_cfg;
    u32 slave_cfg;
    unsigned int tx_fifo_depth;
    unsigned int rx_fifo_depth;
    int rx_outstanding;
    u32 clk_freq;
    u32 sda_hold_time;
    u32 sda_falling_time;
    u32 scl_falling_time;
    u16 ss_hcnt;
    u16 ss_lcnt;
    u16 fs_hcnt;
    u16 fs_lcnt;
    u16 fp_hcnt;
    u16 fp_lcnt;
    u16 hs_hcnt;
    u16 hs_lcnt;
    struct pm_qos_request pm_qos;
    int (*acquire_lock)(struct dw_i2c_dev *);
    void (*release_lock)(struct dw_i2c_dev *);
    bool pm_disabled;
    bool suspended;
    bool skip_resume;
    void (*disable)(struct dw_i2c_dev *);
    void (*disable_int)(struct dw_i2c_dev *);
    int (*init)(struct dw_i2c_dev *);
    int mode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dw_i2c_dev {
    struct device *dev;
    void *base;
    struct completion cmd_complete;
    struct clk *clk;
    struct reset_control *rst;
    struct i2c_client *slave;
    u32 (*get_clk_rate_khz)(struct dw_i2c_dev *);
    struct dw_pci_controller *controller;
    int cmd_err;
    struct i2c_msg *msgs;
    int msgs_num;
    int msg_write_idx;
    u32 tx_buf_len;
    u8 *tx_buf;
    int msg_read_idx;
    u32 rx_buf_len;
    u8 *rx_buf;
    int msg_err;
    unsigned int status;
    u32 abort_source;
    int irq;
    u32 flags;
    struct i2c_adapter adapter;
    u32 functionality;
    u32 master_cfg;
    u32 slave_cfg;
    unsigned int tx_fifo_depth;
    unsigned int rx_fifo_depth;
    int rx_outstanding;
    u32 clk_freq;
    u32 sda_hold_time;
    u32 sda_falling_time;
    u32 scl_falling_time;
    u16 ss_hcnt;
    u16 ss_lcnt;
    u16 fs_hcnt;
    u16 fs_lcnt;
    u16 fp_hcnt;
    u16 fp_lcnt;
    u16 hs_hcnt;
    u16 hs_lcnt;
    struct pm_qos_request pm_qos;
    int (*acquire_lock)(struct dw_i2c_dev *);
    void (*release_lock)(struct dw_i2c_dev *);
    bool pm_disabled;
    void (*disable)(struct dw_i2c_dev *);
    void (*disable_int)(struct dw_i2c_dev *);
    int (*init)(struct dw_i2c_dev *);
    int mode;
    struct i2c_bus_recovery_info rinfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dw_i2c_dev {
    struct device *dev;
    void *base;
    void *ext;
    struct completion cmd_complete;
    struct clk *clk;
    struct reset_control *rst;
    struct i2c_client *slave;
    u32 (*get_clk_rate_khz)(struct dw_i2c_dev *);
    struct dw_pci_controller *controller;
    int cmd_err;
    struct i2c_msg *msgs;
    int msgs_num;
    int msg_write_idx;
    u32 tx_buf_len;
    u8 *tx_buf;
    int msg_read_idx;
    u32 rx_buf_len;
    u8 *rx_buf;
    int msg_err;
    unsigned int status;
    u32 abort_source;
    int irq;
    u32 flags;
    struct i2c_adapter adapter;
    u32 functionality;
    u32 master_cfg;
    u32 slave_cfg;
    unsigned int tx_fifo_depth;
    unsigned int rx_fifo_depth;
    int rx_outstanding;
    struct i2c_timings timings;
    u32 sda_hold_time;
    u16 ss_hcnt;
    u16 ss_lcnt;
    u16 fs_hcnt;
    u16 fs_lcnt;
    u16 fp_hcnt;
    u16 fp_lcnt;
    u16 hs_hcnt;
    u16 hs_lcnt;
    int (*acquire_lock)();
    void (*release_lock)();
    bool shared_with_punit;
    void (*disable)(struct dw_i2c_dev *);
    void (*disable_int)(struct dw_i2c_dev *);
    int (*init)(struct dw_i2c_dev *);
    int (*set_sda_hold_time)(struct dw_i2c_dev *);
    int mode;
    struct i2c_bus_recovery_info rinfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dw_i2c_dev {
    struct device *dev;
    void *base;
    void *ext;
    struct completion cmd_complete;
    struct clk *clk;
    struct clk *pclk;
    struct reset_control *rst;
    struct i2c_client *slave;
    u32 (*get_clk_rate_khz)(struct dw_i2c_dev *);
    struct dw_pci_controller *controller;
    int cmd_err;
    struct i2c_msg *msgs;
    int msgs_num;
    int msg_write_idx;
    u32 tx_buf_len;
    u8 *tx_buf;
    int msg_read_idx;
    u32 rx_buf_len;
    u8 *rx_buf;
    int msg_err;
    unsigned int status;
    u32 abort_source;
    int irq;
    u32 flags;
    struct i2c_adapter adapter;
    u32 functionality;
    u32 master_cfg;
    u32 slave_cfg;
    unsigned int tx_fifo_depth;
    unsigned int rx_fifo_depth;
    int rx_outstanding;
    struct i2c_timings timings;
    u32 sda_hold_time;
    u16 ss_hcnt;
    u16 ss_lcnt;
    u16 fs_hcnt;
    u16 fs_lcnt;
    u16 fp_hcnt;
    u16 fp_lcnt;
    u16 hs_hcnt;
    u16 hs_lcnt;
    int (*acquire_lock)();
    void (*release_lock)();
    bool shared_with_punit;
    void (*disable)(struct dw_i2c_dev *);
    void (*disable_int)(struct dw_i2c_dev *);
    int (*init)(struct dw_i2c_dev *);
    int (*set_sda_hold_time)(struct dw_i2c_dev *);
    int mode;
    struct i2c_bus_recovery_info rinfo;
    bool suspended;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dw_i2c_dev {
    struct device *dev;
    void *base;
    void *ext;
    struct completion cmd_complete;
    struct clk *clk;
    struct clk *pclk;
    struct reset_control *rst;
    struct i2c_client *slave;
    u32 (*get_clk_rate_khz)(struct dw_i2c_dev *);
    struct dw_pci_controller *controller;
    int cmd_err;
    struct i2c_msg *msgs;
    int msgs_num;
    int msg_write_idx;
    u32 tx_buf_len;
    u8 *tx_buf;
    int msg_read_idx;
    u32 rx_buf_len;
    u8 *rx_buf;
    int msg_err;
    unsigned int status;
    u32 abort_source;
    int irq;
    u32 flags;
    struct i2c_adapter adapter;
    u32 functionality;
    u32 master_cfg;
    u32 slave_cfg;
    unsigned int tx_fifo_depth;
    unsigned int rx_fifo_depth;
    int rx_outstanding;
    struct i2c_timings timings;
    u32 sda_hold_time;
    u16 ss_hcnt;
    u16 ss_lcnt;
    u16 fs_hcnt;
    u16 fs_lcnt;
    u16 fp_hcnt;
    u16 fp_lcnt;
    u16 hs_hcnt;
    u16 hs_lcnt;
    int (*acquire_lock)();
    void (*release_lock)();
    bool shared_with_punit;
    void (*disable)(struct dw_i2c_dev *);
    void (*disable_int)(struct dw_i2c_dev *);
    int (*init)(struct dw_i2c_dev *);
    int (*set_sda_hold_time)(struct dw_i2c_dev *);
    int mode;
    struct i2c_bus_recovery_info rinfo;
    bool suspended;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dw_i2c_dev {
    struct device *dev;
    struct regmap *map;
    struct regmap *sysmap;
    void *base;
    void *ext;
    struct completion cmd_complete;
    struct clk *clk;
    struct clk *pclk;
    struct reset_control *rst;
    struct i2c_client *slave;
    u32 (*get_clk_rate_khz)(struct dw_i2c_dev *);
    int cmd_err;
    struct i2c_msg *msgs;
    int msgs_num;
    int msg_write_idx;
    u32 tx_buf_len;
    u8 *tx_buf;
    int msg_read_idx;
    u32 rx_buf_len;
    u8 *rx_buf;
    int msg_err;
    unsigned int status;
    u32 abort_source;
    int irq;
    u32 flags;
    struct i2c_adapter adapter;
    u32 functionality;
    u32 master_cfg;
    u32 slave_cfg;
    unsigned int tx_fifo_depth;
    unsigned int rx_fifo_depth;
    int rx_outstanding;
    struct i2c_timings timings;
    u32 sda_hold_time;
    u16 ss_hcnt;
    u16 ss_lcnt;
    u16 fs_hcnt;
    u16 fs_lcnt;
    u16 fp_hcnt;
    u16 fp_lcnt;
    u16 hs_hcnt;
    u16 hs_lcnt;
    int (*acquire_lock)();
    void (*release_lock)();
    bool shared_with_punit;
    void (*disable)(struct dw_i2c_dev *);
    void (*disable_int)(struct dw_i2c_dev *);
    int (*init)(struct dw_i2c_dev *);
    int (*set_sda_hold_time)(struct dw_i2c_dev *);
    int mode;
    struct i2c_bus_recovery_info rinfo;
    bool suspended;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dw_i2c_dev {
    struct device *dev;
    struct regmap *map;
    struct regmap *sysmap;
    void *base;
    void *ext;
    struct completion cmd_complete;
    struct clk *clk;
    struct clk *pclk;
    struct reset_control *rst;
    struct i2c_client *slave;
    u32 (*get_clk_rate_khz)(struct dw_i2c_dev *);
    int cmd_err;
    struct i2c_msg *msgs;
    int msgs_num;
    int msg_write_idx;
    u32 tx_buf_len;
    u8 *tx_buf;
    int msg_read_idx;
    u32 rx_buf_len;
    u8 *rx_buf;
    int msg_err;
    unsigned int status;
    u32 abort_source;
    int irq;
    u32 flags;
    struct i2c_adapter adapter;
    u32 functionality;
    u32 master_cfg;
    u32 slave_cfg;
    unsigned int tx_fifo_depth;
    unsigned int rx_fifo_depth;
    int rx_outstanding;
    struct i2c_timings timings;
    u32 sda_hold_time;
    u16 ss_hcnt;
    u16 ss_lcnt;
    u16 fs_hcnt;
    u16 fs_lcnt;
    u16 fp_hcnt;
    u16 fp_lcnt;
    u16 hs_hcnt;
    u16 hs_lcnt;
    int (*acquire_lock)();
    void (*release_lock)();
    bool shared_with_punit;
    void (*disable)(struct dw_i2c_dev *);
    void (*disable_int)(struct dw_i2c_dev *);
    int (*init)(struct dw_i2c_dev *);
    int (*set_sda_hold_time)(struct dw_i2c_dev *);
    int mode;
    struct i2c_bus_recovery_info rinfo;
    bool suspended;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dw_i2c_dev {
    struct device *dev;
    struct regmap *map;
    struct regmap *sysmap;
    void *base;
    void *ext;
    struct completion cmd_complete;
    struct clk *clk;
    struct clk *pclk;
    struct reset_control *rst;
    struct i2c_client *slave;
    u32 (*get_clk_rate_khz)(struct dw_i2c_dev *);
    int cmd_err;
    struct i2c_msg *msgs;
    int msgs_num;
    int msg_write_idx;
    u32 tx_buf_len;
    u8 *tx_buf;
    int msg_read_idx;
    u32 rx_buf_len;
    u8 *rx_buf;
    int msg_err;
    unsigned int status;
    u32 abort_source;
    int irq;
    u32 flags;
    struct i2c_adapter adapter;
    u32 functionality;
    u32 master_cfg;
    u32 slave_cfg;
    unsigned int tx_fifo_depth;
    unsigned int rx_fifo_depth;
    int rx_outstanding;
    struct i2c_timings timings;
    u32 sda_hold_time;
    u16 ss_hcnt;
    u16 ss_lcnt;
    u16 fs_hcnt;
    u16 fs_lcnt;
    u16 fp_hcnt;
    u16 fp_lcnt;
    u16 hs_hcnt;
    u16 hs_lcnt;
    int (*acquire_lock)();
    void (*release_lock)();
    bool shared_with_punit;
    void (*disable)(struct dw_i2c_dev *);
    void (*disable_int)(struct dw_i2c_dev *);
    int (*init)(struct dw_i2c_dev *);
    int (*set_sda_hold_time)(struct dw_i2c_dev *);
    int mode;
    struct i2c_bus_recovery_info rinfo;
    bool suspended;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dw_i2c_dev {
    struct device *dev;
    struct regmap *map;
    struct regmap *sysmap;
    void *base;
    void *ext;
    struct completion cmd_complete;
    struct clk *clk;
    struct clk *pclk;
    struct reset_control *rst;
    struct i2c_client *slave;
    u32 (*get_clk_rate_khz)(struct dw_i2c_dev *);
    int cmd_err;
    struct i2c_msg *msgs;
    int msgs_num;
    int msg_write_idx;
    u32 tx_buf_len;
    u8 *tx_buf;
    int msg_read_idx;
    u32 rx_buf_len;
    u8 *rx_buf;
    int msg_err;
    unsigned int status;
    u32 abort_source;
    int irq;
    u32 flags;
    struct i2c_adapter adapter;
    u32 functionality;
    u32 master_cfg;
    u32 slave_cfg;
    unsigned int tx_fifo_depth;
    unsigned int rx_fifo_depth;
    int rx_outstanding;
    struct i2c_timings timings;
    u32 sda_hold_time;
    u16 ss_hcnt;
    u16 ss_lcnt;
    u16 fs_hcnt;
    u16 fs_lcnt;
    u16 fp_hcnt;
    u16 fp_lcnt;
    u16 hs_hcnt;
    u16 hs_lcnt;
    int (*acquire_lock)();
    void (*release_lock)();
    bool shared_with_punit;
    void (*disable)(struct dw_i2c_dev *);
    void (*disable_int)(struct dw_i2c_dev *);
    int (*init)(struct dw_i2c_dev *);
    int (*set_sda_hold_time)(struct dw_i2c_dev *);
    int mode;
    struct i2c_bus_recovery_info rinfo;
    bool suspended;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dw_i2c_dev {
    struct device *dev;
    struct regmap *map;
    struct regmap *sysmap;
    void *base;
    void *ext;
    struct completion cmd_complete;
    struct clk *clk;
    struct clk *pclk;
    struct reset_control *rst;
    struct i2c_client *slave;
    u32 (*get_clk_rate_khz)(struct dw_i2c_dev *);
    int cmd_err;
    struct i2c_msg *msgs;
    int msgs_num;
    int msg_write_idx;
    u32 tx_buf_len;
    u8 *tx_buf;
    int msg_read_idx;
    u32 rx_buf_len;
    u8 *rx_buf;
    int msg_err;
    unsigned int status;
    u32 abort_source;
    int irq;
    u32 flags;
    struct i2c_adapter adapter;
    u32 functionality;
    u32 master_cfg;
    u32 slave_cfg;
    unsigned int tx_fifo_depth;
    unsigned int rx_fifo_depth;
    int rx_outstanding;
    struct i2c_timings timings;
    u32 sda_hold_time;
    u16 ss_hcnt;
    u16 ss_lcnt;
    u16 fs_hcnt;
    u16 fs_lcnt;
    u16 fp_hcnt;
    u16 fp_lcnt;
    u16 hs_hcnt;
    u16 hs_lcnt;
    int (*acquire_lock)();
    void (*release_lock)();
    int semaphore_idx;
    bool shared_with_punit;
    void (*disable)(struct dw_i2c_dev *);
    void (*disable_int)(struct dw_i2c_dev *);
    int (*init)(struct dw_i2c_dev *);
    int (*set_sda_hold_time)(struct dw_i2c_dev *);
    int mode;
    struct i2c_bus_recovery_info rinfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dw_i2c_dev {
    struct device *dev;
    struct regmap *map;
    struct regmap *sysmap;
    void *base;
    void *ext;
    struct completion cmd_complete;
    struct clk *clk;
    struct clk *pclk;
    struct reset_control *rst;
    struct i2c_client *slave;
    u32 (*get_clk_rate_khz)(struct dw_i2c_dev *);
    int cmd_err;
    struct i2c_msg *msgs;
    int msgs_num;
    int msg_write_idx;
    u32 tx_buf_len;
    u8 *tx_buf;
    int msg_read_idx;
    u32 rx_buf_len;
    u8 *rx_buf;
    int msg_err;
    unsigned int status;
    u32 abort_source;
    int irq;
    u32 flags;
    struct i2c_adapter adapter;
    u32 functionality;
    u32 master_cfg;
    u32 slave_cfg;
    unsigned int tx_fifo_depth;
    unsigned int rx_fifo_depth;
    int rx_outstanding;
    struct i2c_timings timings;
    u32 sda_hold_time;
    u16 ss_hcnt;
    u16 ss_lcnt;
    u16 fs_hcnt;
    u16 fs_lcnt;
    u16 fp_hcnt;
    u16 fp_lcnt;
    u16 hs_hcnt;
    u16 hs_lcnt;
    int (*acquire_lock)();
    void (*release_lock)();
    int semaphore_idx;
    bool shared_with_punit;
    void (*disable)(struct dw_i2c_dev *);
    int (*init)(struct dw_i2c_dev *);
    int (*set_sda_hold_time)(struct dw_i2c_dev *);
    int mode;
    struct i2c_bus_recovery_info rinfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dw_i2c_dev {
    struct device *dev;
    struct regmap *map;
    struct regmap *sysmap;
    void *base;
    void *ext;
    struct completion cmd_complete;
    struct clk *clk;
    struct clk *pclk;
    struct reset_control *rst;
    struct i2c_client *slave;
    u32 (*get_clk_rate_khz)(struct dw_i2c_dev *);
    int cmd_err;
    struct i2c_msg *msgs;
    int msgs_num;
    int msg_write_idx;
    u32 tx_buf_len;
    u8 *tx_buf;
    int msg_read_idx;
    u32 rx_buf_len;
    u8 *rx_buf;
    int msg_err;
    unsigned int status;
    unsigned int abort_source;
    int irq;
    u32 flags;
    struct i2c_adapter adapter;
    u32 functionality;
    u32 master_cfg;
    u32 slave_cfg;
    unsigned int tx_fifo_depth;
    unsigned int rx_fifo_depth;
    int rx_outstanding;
    struct i2c_timings timings;
    u32 sda_hold_time;
    u16 ss_hcnt;
    u16 ss_lcnt;
    u16 fs_hcnt;
    u16 fs_lcnt;
    u16 fp_hcnt;
    u16 fp_lcnt;
    u16 hs_hcnt;
    u16 hs_lcnt;
    int (*acquire_lock)();
    void (*release_lock)();
    int semaphore_idx;
    bool shared_with_punit;
    void (*disable)(struct dw_i2c_dev *);
    int (*init)(struct dw_i2c_dev *);
    int (*set_sda_hold_time)(struct dw_i2c_dev *);
    int mode;
    struct i2c_bus_recovery_info rinfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dw_i2c_dev {
    struct device *dev;
    struct regmap *map;
    struct regmap *sysmap;
    void *base;
    void *ext;
    struct completion cmd_complete;
    struct clk *clk;
    struct clk *pclk;
    struct reset_control *rst;
    struct i2c_client *slave;
    u32 (*get_clk_rate_khz)(struct dw_i2c_dev *);
    int cmd_err;
    struct i2c_msg *msgs;
    int msgs_num;
    int msg_write_idx;
    u32 tx_buf_len;
    u8 *tx_buf;
    int msg_read_idx;
    u32 rx_buf_len;
    u8 *rx_buf;
    int msg_err;
    unsigned int status;
    unsigned int abort_source;
    int irq;
    u32 flags;
    struct i2c_adapter adapter;
    u32 functionality;
    u32 master_cfg;
    u32 slave_cfg;
    unsigned int tx_fifo_depth;
    unsigned int rx_fifo_depth;
    int rx_outstanding;
    struct i2c_timings timings;
    u32 sda_hold_time;
    u16 ss_hcnt;
    u16 ss_lcnt;
    u16 fs_hcnt;
    u16 fs_lcnt;
    u16 fp_hcnt;
    u16 fp_lcnt;
    u16 hs_hcnt;
    u16 hs_lcnt;
    int (*acquire_lock)();
    void (*release_lock)();
    int semaphore_idx;
    bool shared_with_punit;
    void (*disable)(struct dw_i2c_dev *);
    int (*init)(struct dw_i2c_dev *);
    int (*set_sda_hold_time)(struct dw_i2c_dev *);
    int mode;
    struct i2c_bus_recovery_info rinfo;
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
struct dw_i2c_dev {
    struct device *dev;
    void *base;
    void *ext;
    struct completion cmd_complete;
    struct clk *clk;
    struct clk *pclk;
    struct reset_control *rst;
    struct i2c_client *slave;
    u32 (*get_clk_rate_khz)(struct dw_i2c_dev *);
    struct dw_pci_controller *controller;
    int cmd_err;
    struct i2c_msg *msgs;
    int msgs_num;
    int msg_write_idx;
    u32 tx_buf_len;
    u8 *tx_buf;
    int msg_read_idx;
    u32 rx_buf_len;
    u8 *rx_buf;
    int msg_err;
    unsigned int status;
    u32 abort_source;
    int irq;
    u32 flags;
    struct i2c_adapter adapter;
    u32 functionality;
    u32 master_cfg;
    u32 slave_cfg;
    unsigned int tx_fifo_depth;
    unsigned int rx_fifo_depth;
    int rx_outstanding;
    struct i2c_timings timings;
    u32 sda_hold_time;
    u16 ss_hcnt;
    u16 ss_lcnt;
    u16 fs_hcnt;
    u16 fs_lcnt;
    u16 fp_hcnt;
    u16 fp_lcnt;
    u16 hs_hcnt;
    u16 hs_lcnt;
    int (*acquire_lock)();
    void (*release_lock)();
    bool shared_with_punit;
    void (*disable)(struct dw_i2c_dev *);
    void (*disable_int)(struct dw_i2c_dev *);
    int (*init)(struct dw_i2c_dev *);
    int (*set_sda_hold_time)(struct dw_i2c_dev *);
    int mode;
    struct i2c_bus_recovery_info rinfo;
    bool suspended;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dw_i2c_dev {
    struct device *dev;
    void *base;
    void *ext;
    struct completion cmd_complete;
    struct clk *clk;
    struct clk *pclk;
    struct reset_control *rst;
    struct i2c_client *slave;
    u32 (*get_clk_rate_khz)(struct dw_i2c_dev *);
    struct dw_pci_controller *controller;
    int cmd_err;
    struct i2c_msg *msgs;
    int msgs_num;
    int msg_write_idx;
    u32 tx_buf_len;
    u8 *tx_buf;
    int msg_read_idx;
    u32 rx_buf_len;
    u8 *rx_buf;
    int msg_err;
    unsigned int status;
    u32 abort_source;
    int irq;
    u32 flags;
    struct i2c_adapter adapter;
    u32 functionality;
    u32 master_cfg;
    u32 slave_cfg;
    unsigned int tx_fifo_depth;
    unsigned int rx_fifo_depth;
    int rx_outstanding;
    struct i2c_timings timings;
    u32 sda_hold_time;
    u16 ss_hcnt;
    u16 ss_lcnt;
    u16 fs_hcnt;
    u16 fs_lcnt;
    u16 fp_hcnt;
    u16 fp_lcnt;
    u16 hs_hcnt;
    u16 hs_lcnt;
    int (*acquire_lock)();
    void (*release_lock)();
    bool shared_with_punit;
    void (*disable)(struct dw_i2c_dev *);
    void (*disable_int)(struct dw_i2c_dev *);
    int (*init)(struct dw_i2c_dev *);
    int (*set_sda_hold_time)(struct dw_i2c_dev *);
    int mode;
    struct i2c_bus_recovery_info rinfo;
    bool suspended;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dw_i2c_dev {
    struct device *dev;
    void *base;
    void *ext;
    struct completion cmd_complete;
    struct clk *clk;
    struct clk *pclk;
    struct reset_control *rst;
    struct i2c_client *slave;
    u32 (*get_clk_rate_khz)(struct dw_i2c_dev *);
    struct dw_pci_controller *controller;
    int cmd_err;
    struct i2c_msg *msgs;
    int msgs_num;
    int msg_write_idx;
    u32 tx_buf_len;
    u8 *tx_buf;
    int msg_read_idx;
    u32 rx_buf_len;
    u8 *rx_buf;
    int msg_err;
    unsigned int status;
    u32 abort_source;
    int irq;
    u32 flags;
    struct i2c_adapter adapter;
    u32 functionality;
    u32 master_cfg;
    u32 slave_cfg;
    unsigned int tx_fifo_depth;
    unsigned int rx_fifo_depth;
    int rx_outstanding;
    struct i2c_timings timings;
    u32 sda_hold_time;
    u16 ss_hcnt;
    u16 ss_lcnt;
    u16 fs_hcnt;
    u16 fs_lcnt;
    u16 fp_hcnt;
    u16 fp_lcnt;
    u16 hs_hcnt;
    u16 hs_lcnt;
    int (*acquire_lock)();
    void (*release_lock)();
    bool shared_with_punit;
    void (*disable)(struct dw_i2c_dev *);
    void (*disable_int)(struct dw_i2c_dev *);
    int (*init)(struct dw_i2c_dev *);
    int (*set_sda_hold_time)(struct dw_i2c_dev *);
    int mode;
    struct i2c_bus_recovery_info rinfo;
    bool suspended;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dw_i2c_dev {
    struct device *dev;
    void *base;
    void *ext;
    struct completion cmd_complete;
    struct clk *clk;
    struct clk *pclk;
    struct reset_control *rst;
    struct i2c_client *slave;
    u32 (*get_clk_rate_khz)(struct dw_i2c_dev *);
    struct dw_pci_controller *controller;
    int cmd_err;
    struct i2c_msg *msgs;
    int msgs_num;
    int msg_write_idx;
    u32 tx_buf_len;
    u8 *tx_buf;
    int msg_read_idx;
    u32 rx_buf_len;
    u8 *rx_buf;
    int msg_err;
    unsigned int status;
    u32 abort_source;
    int irq;
    u32 flags;
    struct i2c_adapter adapter;
    u32 functionality;
    u32 master_cfg;
    u32 slave_cfg;
    unsigned int tx_fifo_depth;
    unsigned int rx_fifo_depth;
    int rx_outstanding;
    struct i2c_timings timings;
    u32 sda_hold_time;
    u16 ss_hcnt;
    u16 ss_lcnt;
    u16 fs_hcnt;
    u16 fs_lcnt;
    u16 fp_hcnt;
    u16 fp_lcnt;
    u16 hs_hcnt;
    u16 hs_lcnt;
    int (*acquire_lock)();
    void (*release_lock)();
    bool shared_with_punit;
    void (*disable)(struct dw_i2c_dev *);
    void (*disable_int)(struct dw_i2c_dev *);
    int (*init)(struct dw_i2c_dev *);
    int (*set_sda_hold_time)(struct dw_i2c_dev *);
    int mode;
    struct i2c_bus_recovery_info rinfo;
    bool suspended;
};
```
</details>
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
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dw_i2c_dev {
    struct device *dev;
    void *base;
    void *ext;
    struct completion cmd_complete;
    struct clk *clk;
    struct clk *pclk;
    struct reset_control *rst;
    struct i2c_client *slave;
    u32 (*get_clk_rate_khz)(struct dw_i2c_dev *);
    struct dw_pci_controller *controller;
    int cmd_err;
    struct i2c_msg *msgs;
    int msgs_num;
    int msg_write_idx;
    u32 tx_buf_len;
    u8 *tx_buf;
    int msg_read_idx;
    u32 rx_buf_len;
    u8 *rx_buf;
    int msg_err;
    unsigned int status;
    u32 abort_source;
    int irq;
    u32 flags;
    struct i2c_adapter adapter;
    u32 functionality;
    u32 master_cfg;
    u32 slave_cfg;
    unsigned int tx_fifo_depth;
    unsigned int rx_fifo_depth;
    int rx_outstanding;
    struct i2c_timings timings;
    u32 sda_hold_time;
    u16 ss_hcnt;
    u16 ss_lcnt;
    u16 fs_hcnt;
    u16 fs_lcnt;
    u16 fp_hcnt;
    u16 fp_lcnt;
    u16 hs_hcnt;
    u16 hs_lcnt;
    int (*acquire_lock)();
    void (*release_lock)();
    bool shared_with_punit;
    void (*disable)(struct dw_i2c_dev *);
    void (*disable_int)(struct dw_i2c_dev *);
    int (*init)(struct dw_i2c_dev *);
    int (*set_sda_hold_time)(struct dw_i2c_dev *);
    int mode;
    struct i2c_bus_recovery_info rinfo;
    bool suspended;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dw_i2c_dev {
    struct device *dev;
    void *base;
    void *ext;
    struct completion cmd_complete;
    struct clk *clk;
    struct clk *pclk;
    struct reset_control *rst;
    struct i2c_client *slave;
    u32 (*get_clk_rate_khz)(struct dw_i2c_dev *);
    struct dw_pci_controller *controller;
    int cmd_err;
    struct i2c_msg *msgs;
    int msgs_num;
    int msg_write_idx;
    u32 tx_buf_len;
    u8 *tx_buf;
    int msg_read_idx;
    u32 rx_buf_len;
    u8 *rx_buf;
    int msg_err;
    unsigned int status;
    u32 abort_source;
    int irq;
    u32 flags;
    struct i2c_adapter adapter;
    u32 functionality;
    u32 master_cfg;
    u32 slave_cfg;
    unsigned int tx_fifo_depth;
    unsigned int rx_fifo_depth;
    int rx_outstanding;
    struct i2c_timings timings;
    u32 sda_hold_time;
    u16 ss_hcnt;
    u16 ss_lcnt;
    u16 fs_hcnt;
    u16 fs_lcnt;
    u16 fp_hcnt;
    u16 fp_lcnt;
    u16 hs_hcnt;
    u16 hs_lcnt;
    int (*acquire_lock)();
    void (*release_lock)();
    bool shared_with_punit;
    void (*disable)(struct dw_i2c_dev *);
    void (*disable_int)(struct dw_i2c_dev *);
    int (*init)(struct dw_i2c_dev *);
    int (*set_sda_hold_time)(struct dw_i2c_dev *);
    int mode;
    struct i2c_bus_recovery_info rinfo;
    bool suspended;
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
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool suspended</code>
</li>
<li>
<b>Field added. </b>
<code>bool skip_resume</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct i2c_bus_recovery_info rinfo</code>
</li>
<li>
<b>Field removed. </b>
<code>bool suspended</code>
</li>
<li>
<b>Field removed. </b>
<code>bool skip_resume</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void *ext</code>
</li>
<li>
<b>Field added. </b>
<code>struct i2c_timings timings</code>
</li>
<li>
<b>Field added. </b>
<code>bool shared_with_punit</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_sda_hold_time)(struct dw_i2c_dev *)</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 clk_freq</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 sda_falling_time</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 scl_falling_time</code>
</li>
<li>
<b>Field removed. </b>
<code>struct pm_qos_request pm_qos</code>
</li>
<li>
<b>Field removed. </b>
<code>bool pm_disabled</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*acquire_lock)(struct dw_i2c_dev *)</code> ➡️ <code>int (*acquire_lock)()</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*release_lock)(struct dw_i2c_dev *)</code> ➡️ <code>void (*release_lock)()</code>
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
<code>struct clk *pclk</code>
</li>
<li>
<b>Field added. </b>
<code>bool suspended</code>
</li>
</ul>
</details>
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
<code>struct regmap *map</code>
</li>
<li>
<b>Field added. </b>
<code>struct regmap *sysmap</code>
</li>
<li>
<b>Field removed. </b>
<code>struct dw_pci_controller *controller</code>
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
<b>Field added. </b>
<code>int semaphore_idx</code>
</li>
<li>
<b>Field removed. </b>
<code>bool suspended</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>void (*disable_int)(struct dw_i2c_dev *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>u32 abort_source</code> ➡️ <code>unsigned int abort_source</code>
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
<li>
<b>Field type changed. </b>
<code>struct clk *pclk</code> ➡️ <code>struct clk *pclk</code>
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
