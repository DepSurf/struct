# Struct: <code>cec_adapter</code>

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
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct cec_adapter {
    struct module *owner;
    char name[32];
    struct cec_devnode devnode;
    struct mutex lock;
    struct rc_dev *rc;
    struct list_head transmit_queue;
    unsigned int transmit_queue_sz;
    struct list_head wait_queue;
    struct cec_data *transmitting;
    bool transmit_in_progress;
    struct task_struct *kthread_config;
    struct completion config_completion;
    struct task_struct *kthread;
    wait_queue_head_t kthread_waitq;
    wait_queue_head_t waitq;
    const struct cec_adap_ops *ops;
    void *priv;
    u32 capabilities;
    u8 available_log_addrs;
    u16 phys_addr;
    bool needs_hpd;
    bool is_configuring;
    bool is_configured;
    bool cec_pin_is_high;
    u8 last_initiator;
    u32 monitor_all_cnt;
    u32 monitor_pin_cnt;
    u32 follower_cnt;
    struct cec_fh *cec_follower;
    struct cec_fh *cec_initiator;
    bool passthrough;
    struct cec_log_addrs log_addrs;
    u32 tx_timeouts;
    struct cec_notifier *notifier;
    struct dentry *cec_dir;
    struct dentry *status_file;
    struct dentry *error_inj_file;
    u16 phys_addrs[15];
    u32 sequence;
    char input_phys[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct cec_adapter {
    struct module *owner;
    char name[32];
    struct cec_devnode devnode;
    struct mutex lock;
    struct rc_dev *rc;
    struct list_head transmit_queue;
    unsigned int transmit_queue_sz;
    struct list_head wait_queue;
    struct cec_data *transmitting;
    bool transmit_in_progress;
    struct task_struct *kthread_config;
    struct completion config_completion;
    struct task_struct *kthread;
    wait_queue_head_t kthread_waitq;
    wait_queue_head_t waitq;
    const struct cec_adap_ops *ops;
    void *priv;
    u32 capabilities;
    u8 available_log_addrs;
    u16 phys_addr;
    bool needs_hpd;
    bool is_configuring;
    bool is_configured;
    bool cec_pin_is_high;
    u8 last_initiator;
    u32 monitor_all_cnt;
    u32 monitor_pin_cnt;
    u32 follower_cnt;
    struct cec_fh *cec_follower;
    struct cec_fh *cec_initiator;
    bool passthrough;
    struct cec_log_addrs log_addrs;
    struct cec_connector_info conn_info;
    u32 tx_timeouts;
    struct cec_notifier *notifier;
    struct dentry *cec_dir;
    struct dentry *status_file;
    struct dentry *error_inj_file;
    u16 phys_addrs[15];
    u32 sequence;
    char input_phys[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct cec_adapter {
    struct module *owner;
    char name[32];
    struct cec_devnode devnode;
    struct mutex lock;
    struct rc_dev *rc;
    struct list_head transmit_queue;
    unsigned int transmit_queue_sz;
    struct list_head wait_queue;
    struct cec_data *transmitting;
    bool transmit_in_progress;
    struct task_struct *kthread_config;
    struct completion config_completion;
    struct task_struct *kthread;
    wait_queue_head_t kthread_waitq;
    wait_queue_head_t waitq;
    const struct cec_adap_ops *ops;
    void *priv;
    u32 capabilities;
    u8 available_log_addrs;
    u16 phys_addr;
    bool needs_hpd;
    bool is_configuring;
    bool is_configured;
    bool cec_pin_is_high;
    u8 last_initiator;
    u32 monitor_all_cnt;
    u32 monitor_pin_cnt;
    u32 follower_cnt;
    struct cec_fh *cec_follower;
    struct cec_fh *cec_initiator;
    bool passthrough;
    struct cec_log_addrs log_addrs;
    struct cec_connector_info conn_info;
    u32 tx_timeouts;
    struct cec_notifier *notifier;
    struct dentry *cec_dir;
    struct dentry *status_file;
    struct dentry *error_inj_file;
    u16 phys_addrs[15];
    u32 sequence;
    char input_phys[32];
};
```
</details>
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
struct cec_adapter {
    struct module *owner;
    char name[32];
    struct cec_devnode devnode;
    struct mutex lock;
    struct rc_dev *rc;
    struct list_head transmit_queue;
    unsigned int transmit_queue_sz;
    struct list_head wait_queue;
    struct cec_data *transmitting;
    bool transmit_in_progress;
    struct task_struct *kthread_config;
    struct completion config_completion;
    struct task_struct *kthread;
    wait_queue_head_t kthread_waitq;
    wait_queue_head_t waitq;
    const struct cec_adap_ops *ops;
    void *priv;
    u32 capabilities;
    u8 available_log_addrs;
    u16 phys_addr;
    bool needs_hpd;
    bool is_configuring;
    bool is_configured;
    bool cec_pin_is_high;
    u8 last_initiator;
    u32 monitor_all_cnt;
    u32 monitor_pin_cnt;
    u32 follower_cnt;
    struct cec_fh *cec_follower;
    struct cec_fh *cec_initiator;
    bool passthrough;
    struct cec_log_addrs log_addrs;
    struct cec_connector_info conn_info;
    u32 tx_timeouts;
    struct cec_notifier *notifier;
    struct cec_pin *pin;
    struct dentry *cec_dir;
    struct dentry *status_file;
    struct dentry *error_inj_file;
    u16 phys_addrs[15];
    u32 sequence;
    char input_phys[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct cec_adapter {
    struct module *owner;
    char name[32];
    struct cec_devnode devnode;
    struct mutex lock;
    struct rc_dev *rc;
    struct list_head transmit_queue;
    unsigned int transmit_queue_sz;
    struct list_head wait_queue;
    struct cec_data *transmitting;
    bool transmit_in_progress;
    struct task_struct *kthread_config;
    struct completion config_completion;
    struct task_struct *kthread;
    wait_queue_head_t kthread_waitq;
    wait_queue_head_t waitq;
    const struct cec_adap_ops *ops;
    void *priv;
    u32 capabilities;
    u8 available_log_addrs;
    u16 phys_addr;
    bool needs_hpd;
    bool is_configuring;
    bool is_configured;
    bool cec_pin_is_high;
    u8 last_initiator;
    u32 monitor_all_cnt;
    u32 monitor_pin_cnt;
    u32 follower_cnt;
    struct cec_fh *cec_follower;
    struct cec_fh *cec_initiator;
    bool passthrough;
    struct cec_log_addrs log_addrs;
    struct cec_connector_info conn_info;
    u32 tx_timeouts;
    struct cec_notifier *notifier;
    struct dentry *cec_dir;
    struct dentry *status_file;
    struct dentry *error_inj_file;
    u16 phys_addrs[15];
    u32 sequence;
    char input_phys[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct cec_adapter {
    struct module *owner;
    char name[32];
    struct cec_devnode devnode;
    struct mutex lock;
    struct rc_dev *rc;
    struct list_head transmit_queue;
    unsigned int transmit_queue_sz;
    struct list_head wait_queue;
    struct cec_data *transmitting;
    bool transmit_in_progress;
    struct task_struct *kthread_config;
    struct completion config_completion;
    struct task_struct *kthread;
    wait_queue_head_t kthread_waitq;
    wait_queue_head_t waitq;
    const struct cec_adap_ops *ops;
    void *priv;
    u32 capabilities;
    u8 available_log_addrs;
    u16 phys_addr;
    bool needs_hpd;
    bool is_configuring;
    bool is_configured;
    bool cec_pin_is_high;
    u8 last_initiator;
    u32 monitor_all_cnt;
    u32 monitor_pin_cnt;
    u32 follower_cnt;
    struct cec_fh *cec_follower;
    struct cec_fh *cec_initiator;
    bool passthrough;
    struct cec_log_addrs log_addrs;
    struct cec_connector_info conn_info;
    u32 tx_timeouts;
    struct cec_notifier *notifier;
    struct dentry *cec_dir;
    struct dentry *status_file;
    struct dentry *error_inj_file;
    u16 phys_addrs[15];
    u32 sequence;
    char input_phys[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct cec_adapter {
    struct module *owner;
    char name[32];
    struct cec_devnode devnode;
    struct mutex lock;
    struct rc_dev *rc;
    struct list_head transmit_queue;
    unsigned int transmit_queue_sz;
    struct list_head wait_queue;
    struct cec_data *transmitting;
    bool transmit_in_progress;
    struct task_struct *kthread_config;
    struct completion config_completion;
    struct task_struct *kthread;
    wait_queue_head_t kthread_waitq;
    wait_queue_head_t waitq;
    const struct cec_adap_ops *ops;
    void *priv;
    u32 capabilities;
    u8 available_log_addrs;
    u16 phys_addr;
    bool needs_hpd;
    bool is_configuring;
    bool is_configured;
    bool cec_pin_is_high;
    u8 last_initiator;
    u32 monitor_all_cnt;
    u32 monitor_pin_cnt;
    u32 follower_cnt;
    struct cec_fh *cec_follower;
    struct cec_fh *cec_initiator;
    bool passthrough;
    struct cec_log_addrs log_addrs;
    struct cec_connector_info conn_info;
    u32 tx_timeouts;
    struct cec_notifier *notifier;
    struct dentry *cec_dir;
    struct dentry *status_file;
    struct dentry *error_inj_file;
    u16 phys_addrs[15];
    u32 sequence;
    char input_phys[32];
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
struct cec_adapter {
    struct module *owner;
    char name[32];
    struct cec_devnode devnode;
    struct mutex lock;
    struct rc_dev *rc;
    struct list_head transmit_queue;
    unsigned int transmit_queue_sz;
    struct list_head wait_queue;
    struct cec_data *transmitting;
    bool transmit_in_progress;
    struct task_struct *kthread_config;
    struct completion config_completion;
    struct task_struct *kthread;
    wait_queue_head_t kthread_waitq;
    wait_queue_head_t waitq;
    const struct cec_adap_ops *ops;
    void *priv;
    u32 capabilities;
    u8 available_log_addrs;
    u16 phys_addr;
    bool needs_hpd;
    bool is_configuring;
    bool is_configured;
    bool cec_pin_is_high;
    u8 last_initiator;
    u32 monitor_all_cnt;
    u32 monitor_pin_cnt;
    u32 follower_cnt;
    struct cec_fh *cec_follower;
    struct cec_fh *cec_initiator;
    bool passthrough;
    struct cec_log_addrs log_addrs;
    struct cec_connector_info conn_info;
    u32 tx_timeouts;
    struct cec_notifier *notifier;
    struct dentry *cec_dir;
    struct dentry *status_file;
    struct dentry *error_inj_file;
    u16 phys_addrs[15];
    u32 sequence;
    char input_phys[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct cec_adapter {
    struct module *owner;
    char name[32];
    struct cec_devnode devnode;
    struct mutex lock;
    struct rc_dev *rc;
    struct list_head transmit_queue;
    unsigned int transmit_queue_sz;
    struct list_head wait_queue;
    struct cec_data *transmitting;
    bool transmit_in_progress;
    struct task_struct *kthread_config;
    struct completion config_completion;
    struct task_struct *kthread;
    wait_queue_head_t kthread_waitq;
    wait_queue_head_t waitq;
    const struct cec_adap_ops *ops;
    void *priv;
    u32 capabilities;
    u8 available_log_addrs;
    u16 phys_addr;
    bool needs_hpd;
    bool is_configuring;
    bool is_configured;
    bool cec_pin_is_high;
    u8 last_initiator;
    u32 monitor_all_cnt;
    u32 monitor_pin_cnt;
    u32 follower_cnt;
    struct cec_fh *cec_follower;
    struct cec_fh *cec_initiator;
    bool passthrough;
    struct cec_log_addrs log_addrs;
    struct cec_connector_info conn_info;
    u32 tx_timeouts;
    struct cec_notifier *notifier;
    struct dentry *cec_dir;
    struct dentry *status_file;
    struct dentry *error_inj_file;
    u16 phys_addrs[15];
    u32 sequence;
    char input_phys[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct cec_adapter {
    struct module *owner;
    char name[32];
    struct cec_devnode devnode;
    struct mutex lock;
    struct rc_dev *rc;
    struct list_head transmit_queue;
    unsigned int transmit_queue_sz;
    struct list_head wait_queue;
    struct cec_data *transmitting;
    bool transmit_in_progress;
    struct task_struct *kthread_config;
    struct completion config_completion;
    struct task_struct *kthread;
    wait_queue_head_t kthread_waitq;
    wait_queue_head_t waitq;
    const struct cec_adap_ops *ops;
    void *priv;
    u32 capabilities;
    u8 available_log_addrs;
    u16 phys_addr;
    bool needs_hpd;
    bool is_configuring;
    bool is_configured;
    bool cec_pin_is_high;
    u8 last_initiator;
    u32 monitor_all_cnt;
    u32 monitor_pin_cnt;
    u32 follower_cnt;
    struct cec_fh *cec_follower;
    struct cec_fh *cec_initiator;
    bool passthrough;
    struct cec_log_addrs log_addrs;
    struct cec_connector_info conn_info;
    u32 tx_timeouts;
    struct cec_notifier *notifier;
    struct dentry *cec_dir;
    struct dentry *status_file;
    struct dentry *error_inj_file;
    u16 phys_addrs[15];
    u32 sequence;
    char input_phys[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cec_adapter {
    struct module *owner;
    char name[32];
    struct cec_devnode devnode;
    struct mutex lock;
    struct rc_dev *rc;
    struct list_head transmit_queue;
    unsigned int transmit_queue_sz;
    struct list_head wait_queue;
    struct cec_data *transmitting;
    bool transmit_in_progress;
    struct task_struct *kthread_config;
    struct completion config_completion;
    struct task_struct *kthread;
    wait_queue_head_t kthread_waitq;
    wait_queue_head_t waitq;
    const struct cec_adap_ops *ops;
    void *priv;
    u32 capabilities;
    u8 available_log_addrs;
    u16 phys_addr;
    bool needs_hpd;
    bool is_configuring;
    bool is_configured;
    bool cec_pin_is_high;
    u8 last_initiator;
    u32 monitor_all_cnt;
    u32 monitor_pin_cnt;
    u32 follower_cnt;
    struct cec_fh *cec_follower;
    struct cec_fh *cec_initiator;
    bool passthrough;
    struct cec_log_addrs log_addrs;
    struct cec_connector_info conn_info;
    u32 tx_timeouts;
    struct cec_notifier *notifier;
    struct cec_pin *pin;
    struct dentry *cec_dir;
    struct dentry *status_file;
    struct dentry *error_inj_file;
    u16 phys_addrs[15];
    u32 sequence;
    char input_phys[32];
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
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct cec_connector_info conn_info</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>arm64</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct cec_pin *pin</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>generic</code> and <code>lowlatency</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct cec_pin *pin</code>
</li>
</ul>
</details>
</li>
</ul>
