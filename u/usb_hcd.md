# Struct: <code>usb_hcd</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct usb_hcd {
    struct usb_bus self;
    struct kref kref;
    const char *product_desc;
    int speed;
    char irq_descr[24];
    struct timer_list rh_timer;
    struct urb *status_urb;
    struct work_struct wakeup_work;
    const struct hc_driver *driver;
    struct usb_phy *usb_phy;
    struct phy *phy;
    long unsigned int flags;
    unsigned int rh_registered;
    unsigned int rh_pollable;
    unsigned int msix_enabled;
    unsigned int remove_phy;
    unsigned int uses_new_polling;
    unsigned int wireless;
    unsigned int has_tt;
    unsigned int amd_resume_bug;
    unsigned int can_do_streams;
    unsigned int tpl_support;
    unsigned int cant_recv_wakeups;
    unsigned int irq;
    void *regs;
    resource_size_t rsrc_start;
    resource_size_t rsrc_len;
    unsigned int power_budget;
    struct giveback_urb_bh high_prio_bh;
    struct giveback_urb_bh low_prio_bh;
    struct mutex *bandwidth_mutex;
    struct usb_hcd *shared_hcd;
    struct usb_hcd *primary_hcd;
    struct dma_pool * pool[4];
    int state;
    long unsigned int hcd_priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct usb_hcd {
    struct usb_bus self;
    struct kref kref;
    const char *product_desc;
    int speed;
    char irq_descr[24];
    struct timer_list rh_timer;
    struct urb *status_urb;
    struct work_struct wakeup_work;
    const struct hc_driver *driver;
    struct usb_phy *usb_phy;
    struct phy *phy;
    long unsigned int flags;
    unsigned int rh_registered;
    unsigned int rh_pollable;
    unsigned int msix_enabled;
    unsigned int remove_phy;
    unsigned int uses_new_polling;
    unsigned int wireless;
    unsigned int has_tt;
    unsigned int amd_resume_bug;
    unsigned int can_do_streams;
    unsigned int tpl_support;
    unsigned int cant_recv_wakeups;
    unsigned int irq;
    void *regs;
    resource_size_t rsrc_start;
    resource_size_t rsrc_len;
    unsigned int power_budget;
    struct giveback_urb_bh high_prio_bh;
    struct giveback_urb_bh low_prio_bh;
    struct mutex *address0_mutex;
    struct mutex *bandwidth_mutex;
    struct usb_hcd *shared_hcd;
    struct usb_hcd *primary_hcd;
    struct dma_pool * pool[4];
    int state;
    long unsigned int hcd_priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct usb_hcd {
    struct usb_bus self;
    struct kref kref;
    const char *product_desc;
    int speed;
    char irq_descr[24];
    struct timer_list rh_timer;
    struct urb *status_urb;
    struct work_struct wakeup_work;
    const struct hc_driver *driver;
    struct usb_phy *usb_phy;
    struct phy *phy;
    long unsigned int flags;
    unsigned int rh_registered;
    unsigned int rh_pollable;
    unsigned int msix_enabled;
    unsigned int remove_phy;
    unsigned int uses_new_polling;
    unsigned int wireless;
    unsigned int has_tt;
    unsigned int amd_resume_bug;
    unsigned int can_do_streams;
    unsigned int tpl_support;
    unsigned int cant_recv_wakeups;
    unsigned int irq;
    void *regs;
    resource_size_t rsrc_start;
    resource_size_t rsrc_len;
    unsigned int power_budget;
    struct giveback_urb_bh high_prio_bh;
    struct giveback_urb_bh low_prio_bh;
    struct mutex *address0_mutex;
    struct mutex *bandwidth_mutex;
    struct usb_hcd *shared_hcd;
    struct usb_hcd *primary_hcd;
    struct dma_pool * pool[4];
    int state;
    long unsigned int hcd_priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct usb_hcd {
    struct usb_bus self;
    struct kref kref;
    const char *product_desc;
    int speed;
    char irq_descr[24];
    struct timer_list rh_timer;
    struct urb *status_urb;
    struct work_struct wakeup_work;
    const struct hc_driver *driver;
    struct usb_phy *usb_phy;
    struct phy *phy;
    long unsigned int flags;
    unsigned int rh_registered;
    unsigned int rh_pollable;
    unsigned int msix_enabled;
    unsigned int msi_enabled;
    unsigned int remove_phy;
    unsigned int uses_new_polling;
    unsigned int wireless;
    unsigned int has_tt;
    unsigned int amd_resume_bug;
    unsigned int can_do_streams;
    unsigned int tpl_support;
    unsigned int cant_recv_wakeups;
    unsigned int irq;
    void *regs;
    resource_size_t rsrc_start;
    resource_size_t rsrc_len;
    unsigned int power_budget;
    struct giveback_urb_bh high_prio_bh;
    struct giveback_urb_bh low_prio_bh;
    struct mutex *address0_mutex;
    struct mutex *bandwidth_mutex;
    struct usb_hcd *shared_hcd;
    struct usb_hcd *primary_hcd;
    struct dma_pool * pool[4];
    int state;
    long unsigned int hcd_priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct usb_hcd {
    struct usb_bus self;
    struct kref kref;
    const char *product_desc;
    int speed;
    char irq_descr[24];
    struct timer_list rh_timer;
    struct urb *status_urb;
    struct work_struct wakeup_work;
    const struct hc_driver *driver;
    struct usb_phy *usb_phy;
    struct phy *phy;
    long unsigned int flags;
    unsigned int rh_registered;
    unsigned int rh_pollable;
    unsigned int msix_enabled;
    unsigned int msi_enabled;
    unsigned int remove_phy;
    unsigned int uses_new_polling;
    unsigned int wireless;
    unsigned int has_tt;
    unsigned int amd_resume_bug;
    unsigned int can_do_streams;
    unsigned int tpl_support;
    unsigned int cant_recv_wakeups;
    unsigned int irq;
    void *regs;
    resource_size_t rsrc_start;
    resource_size_t rsrc_len;
    unsigned int power_budget;
    struct giveback_urb_bh high_prio_bh;
    struct giveback_urb_bh low_prio_bh;
    struct mutex *address0_mutex;
    struct mutex *bandwidth_mutex;
    struct usb_hcd *shared_hcd;
    struct usb_hcd *primary_hcd;
    struct dma_pool * pool[4];
    int state;
    long unsigned int hcd_priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct usb_hcd {
    struct usb_bus self;
    struct kref kref;
    const char *product_desc;
    int speed;
    char irq_descr[24];
    struct timer_list rh_timer;
    struct urb *status_urb;
    struct work_struct wakeup_work;
    const struct hc_driver *driver;
    struct usb_phy *usb_phy;
    struct usb_phy_roothub *phy_roothub;
    long unsigned int flags;
    unsigned int rh_registered;
    unsigned int rh_pollable;
    unsigned int msix_enabled;
    unsigned int msi_enabled;
    unsigned int skip_phy_initialization;
    unsigned int uses_new_polling;
    unsigned int wireless;
    unsigned int has_tt;
    unsigned int amd_resume_bug;
    unsigned int can_do_streams;
    unsigned int tpl_support;
    unsigned int cant_recv_wakeups;
    unsigned int irq;
    void *regs;
    resource_size_t rsrc_start;
    resource_size_t rsrc_len;
    unsigned int power_budget;
    struct giveback_urb_bh high_prio_bh;
    struct giveback_urb_bh low_prio_bh;
    struct mutex *address0_mutex;
    struct mutex *bandwidth_mutex;
    struct usb_hcd *shared_hcd;
    struct usb_hcd *primary_hcd;
    struct dma_pool * pool[4];
    int state;
    long unsigned int hcd_priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct usb_hcd {
    struct usb_bus self;
    struct kref kref;
    const char *product_desc;
    int speed;
    char irq_descr[24];
    struct timer_list rh_timer;
    struct urb *status_urb;
    struct work_struct wakeup_work;
    const struct hc_driver *driver;
    struct usb_phy *usb_phy;
    struct usb_phy_roothub *phy_roothub;
    long unsigned int flags;
    unsigned int rh_registered;
    unsigned int rh_pollable;
    unsigned int msix_enabled;
    unsigned int msi_enabled;
    unsigned int skip_phy_initialization;
    unsigned int uses_new_polling;
    unsigned int wireless;
    unsigned int has_tt;
    unsigned int amd_resume_bug;
    unsigned int can_do_streams;
    unsigned int tpl_support;
    unsigned int cant_recv_wakeups;
    unsigned int irq;
    void *regs;
    resource_size_t rsrc_start;
    resource_size_t rsrc_len;
    unsigned int power_budget;
    struct giveback_urb_bh high_prio_bh;
    struct giveback_urb_bh low_prio_bh;
    struct mutex *address0_mutex;
    struct mutex *bandwidth_mutex;
    struct usb_hcd *shared_hcd;
    struct usb_hcd *primary_hcd;
    struct dma_pool * pool[4];
    int state;
    long unsigned int hcd_priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct usb_hcd {
    struct usb_bus self;
    struct kref kref;
    const char *product_desc;
    int speed;
    char irq_descr[24];
    struct timer_list rh_timer;
    struct urb *status_urb;
    struct work_struct wakeup_work;
    struct work_struct died_work;
    const struct hc_driver *driver;
    struct usb_phy *usb_phy;
    struct usb_phy_roothub *phy_roothub;
    long unsigned int flags;
    enum usb_dev_authorize_policy dev_policy;
    unsigned int rh_registered;
    unsigned int rh_pollable;
    unsigned int msix_enabled;
    unsigned int msi_enabled;
    unsigned int skip_phy_initialization;
    unsigned int uses_new_polling;
    unsigned int wireless;
    unsigned int has_tt;
    unsigned int amd_resume_bug;
    unsigned int can_do_streams;
    unsigned int tpl_support;
    unsigned int cant_recv_wakeups;
    unsigned int irq;
    void *regs;
    resource_size_t rsrc_start;
    resource_size_t rsrc_len;
    unsigned int power_budget;
    struct giveback_urb_bh high_prio_bh;
    struct giveback_urb_bh low_prio_bh;
    struct mutex *address0_mutex;
    struct mutex *bandwidth_mutex;
    struct usb_hcd *shared_hcd;
    struct usb_hcd *primary_hcd;
    struct dma_pool * pool[4];
    int state;
    struct gen_pool *localmem_pool;
    long unsigned int hcd_priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct usb_hcd {
    struct usb_bus self;
    struct kref kref;
    const char *product_desc;
    int speed;
    char irq_descr[24];
    struct timer_list rh_timer;
    struct urb *status_urb;
    struct work_struct wakeup_work;
    struct work_struct died_work;
    const struct hc_driver *driver;
    struct usb_phy *usb_phy;
    struct usb_phy_roothub *phy_roothub;
    long unsigned int flags;
    enum usb_dev_authorize_policy dev_policy;
    unsigned int rh_registered;
    unsigned int rh_pollable;
    unsigned int msix_enabled;
    unsigned int msi_enabled;
    unsigned int skip_phy_initialization;
    unsigned int uses_new_polling;
    unsigned int wireless;
    unsigned int has_tt;
    unsigned int amd_resume_bug;
    unsigned int can_do_streams;
    unsigned int tpl_support;
    unsigned int cant_recv_wakeups;
    unsigned int irq;
    void *regs;
    resource_size_t rsrc_start;
    resource_size_t rsrc_len;
    unsigned int power_budget;
    struct giveback_urb_bh high_prio_bh;
    struct giveback_urb_bh low_prio_bh;
    struct mutex *address0_mutex;
    struct mutex *bandwidth_mutex;
    struct usb_hcd *shared_hcd;
    struct usb_hcd *primary_hcd;
    struct dma_pool * pool[4];
    int state;
    struct gen_pool *localmem_pool;
    long unsigned int hcd_priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct usb_hcd {
    struct usb_bus self;
    struct kref kref;
    const char *product_desc;
    int speed;
    char irq_descr[24];
    struct timer_list rh_timer;
    struct urb *status_urb;
    struct work_struct wakeup_work;
    struct work_struct died_work;
    const struct hc_driver *driver;
    struct usb_phy *usb_phy;
    struct usb_phy_roothub *phy_roothub;
    long unsigned int flags;
    enum usb_dev_authorize_policy dev_policy;
    unsigned int rh_registered;
    unsigned int rh_pollable;
    unsigned int msix_enabled;
    unsigned int msi_enabled;
    unsigned int skip_phy_initialization;
    unsigned int uses_new_polling;
    unsigned int wireless;
    unsigned int has_tt;
    unsigned int amd_resume_bug;
    unsigned int can_do_streams;
    unsigned int tpl_support;
    unsigned int cant_recv_wakeups;
    unsigned int irq;
    void *regs;
    resource_size_t rsrc_start;
    resource_size_t rsrc_len;
    unsigned int power_budget;
    struct giveback_urb_bh high_prio_bh;
    struct giveback_urb_bh low_prio_bh;
    struct mutex *address0_mutex;
    struct mutex *bandwidth_mutex;
    struct usb_hcd *shared_hcd;
    struct usb_hcd *primary_hcd;
    struct dma_pool * pool[4];
    int state;
    struct gen_pool *localmem_pool;
    long unsigned int hcd_priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct usb_hcd {
    struct usb_bus self;
    struct kref kref;
    const char *product_desc;
    int speed;
    char irq_descr[24];
    struct timer_list rh_timer;
    struct urb *status_urb;
    struct work_struct wakeup_work;
    struct work_struct died_work;
    const struct hc_driver *driver;
    struct usb_phy *usb_phy;
    struct usb_phy_roothub *phy_roothub;
    long unsigned int flags;
    enum usb_dev_authorize_policy dev_policy;
    unsigned int rh_registered;
    unsigned int rh_pollable;
    unsigned int msix_enabled;
    unsigned int msi_enabled;
    unsigned int skip_phy_initialization;
    unsigned int uses_new_polling;
    unsigned int wireless;
    unsigned int has_tt;
    unsigned int amd_resume_bug;
    unsigned int can_do_streams;
    unsigned int tpl_support;
    unsigned int cant_recv_wakeups;
    unsigned int irq;
    void *regs;
    resource_size_t rsrc_start;
    resource_size_t rsrc_len;
    unsigned int power_budget;
    struct giveback_urb_bh high_prio_bh;
    struct giveback_urb_bh low_prio_bh;
    struct mutex *address0_mutex;
    struct mutex *bandwidth_mutex;
    struct usb_hcd *shared_hcd;
    struct usb_hcd *primary_hcd;
    struct dma_pool * pool[4];
    int state;
    struct gen_pool *localmem_pool;
    long unsigned int hcd_priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct usb_hcd {
    struct usb_bus self;
    struct kref kref;
    const char *product_desc;
    int speed;
    char irq_descr[24];
    struct timer_list rh_timer;
    struct urb *status_urb;
    struct work_struct wakeup_work;
    struct work_struct died_work;
    const struct hc_driver *driver;
    struct usb_phy *usb_phy;
    struct usb_phy_roothub *phy_roothub;
    long unsigned int flags;
    enum usb_dev_authorize_policy dev_policy;
    unsigned int rh_registered;
    unsigned int rh_pollable;
    unsigned int msix_enabled;
    unsigned int msi_enabled;
    unsigned int skip_phy_initialization;
    unsigned int uses_new_polling;
    unsigned int wireless;
    unsigned int has_tt;
    unsigned int amd_resume_bug;
    unsigned int can_do_streams;
    unsigned int tpl_support;
    unsigned int cant_recv_wakeups;
    unsigned int irq;
    void *regs;
    resource_size_t rsrc_start;
    resource_size_t rsrc_len;
    unsigned int power_budget;
    struct giveback_urb_bh high_prio_bh;
    struct giveback_urb_bh low_prio_bh;
    struct mutex *address0_mutex;
    struct mutex *bandwidth_mutex;
    struct usb_hcd *shared_hcd;
    struct usb_hcd *primary_hcd;
    struct dma_pool * pool[4];
    int state;
    struct gen_pool *localmem_pool;
    long unsigned int hcd_priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct usb_hcd {
    struct usb_bus self;
    struct kref kref;
    const char *product_desc;
    int speed;
    char irq_descr[24];
    struct timer_list rh_timer;
    struct urb *status_urb;
    struct work_struct wakeup_work;
    struct work_struct died_work;
    const struct hc_driver *driver;
    struct usb_phy *usb_phy;
    struct usb_phy_roothub *phy_roothub;
    long unsigned int flags;
    enum usb_dev_authorize_policy dev_policy;
    unsigned int rh_registered;
    unsigned int rh_pollable;
    unsigned int msix_enabled;
    unsigned int msi_enabled;
    unsigned int skip_phy_initialization;
    unsigned int uses_new_polling;
    unsigned int wireless;
    unsigned int has_tt;
    unsigned int amd_resume_bug;
    unsigned int can_do_streams;
    unsigned int tpl_support;
    unsigned int cant_recv_wakeups;
    unsigned int irq;
    void *regs;
    resource_size_t rsrc_start;
    resource_size_t rsrc_len;
    unsigned int power_budget;
    struct giveback_urb_bh high_prio_bh;
    struct giveback_urb_bh low_prio_bh;
    struct mutex *address0_mutex;
    struct mutex *bandwidth_mutex;
    struct usb_hcd *shared_hcd;
    struct usb_hcd *primary_hcd;
    struct dma_pool * pool[4];
    int state;
    struct gen_pool *localmem_pool;
    long unsigned int hcd_priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct usb_hcd {
    struct usb_bus self;
    struct kref kref;
    const char *product_desc;
    int speed;
    char irq_descr[24];
    struct timer_list rh_timer;
    struct urb *status_urb;
    struct work_struct wakeup_work;
    struct work_struct died_work;
    const struct hc_driver *driver;
    struct usb_phy *usb_phy;
    struct usb_phy_roothub *phy_roothub;
    long unsigned int flags;
    enum usb_dev_authorize_policy dev_policy;
    unsigned int rh_registered;
    unsigned int rh_pollable;
    unsigned int msix_enabled;
    unsigned int msi_enabled;
    unsigned int skip_phy_initialization;
    unsigned int uses_new_polling;
    unsigned int wireless;
    unsigned int has_tt;
    unsigned int amd_resume_bug;
    unsigned int can_do_streams;
    unsigned int tpl_support;
    unsigned int cant_recv_wakeups;
    unsigned int irq;
    void *regs;
    resource_size_t rsrc_start;
    resource_size_t rsrc_len;
    unsigned int power_budget;
    struct giveback_urb_bh high_prio_bh;
    struct giveback_urb_bh low_prio_bh;
    struct mutex *address0_mutex;
    struct mutex *bandwidth_mutex;
    struct usb_hcd *shared_hcd;
    struct usb_hcd *primary_hcd;
    struct dma_pool * pool[4];
    int state;
    struct gen_pool *localmem_pool;
    long unsigned int hcd_priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct usb_hcd {
    struct usb_bus self;
    struct kref kref;
    const char *product_desc;
    int speed;
    char irq_descr[24];
    struct timer_list rh_timer;
    struct urb *status_urb;
    struct work_struct wakeup_work;
    struct work_struct died_work;
    const struct hc_driver *driver;
    struct usb_phy *usb_phy;
    struct usb_phy_roothub *phy_roothub;
    long unsigned int flags;
    enum usb_dev_authorize_policy dev_policy;
    unsigned int rh_registered;
    unsigned int rh_pollable;
    unsigned int msix_enabled;
    unsigned int msi_enabled;
    unsigned int skip_phy_initialization;
    unsigned int uses_new_polling;
    unsigned int wireless;
    unsigned int has_tt;
    unsigned int amd_resume_bug;
    unsigned int can_do_streams;
    unsigned int tpl_support;
    unsigned int cant_recv_wakeups;
    unsigned int irq;
    void *regs;
    resource_size_t rsrc_start;
    resource_size_t rsrc_len;
    unsigned int power_budget;
    struct giveback_urb_bh high_prio_bh;
    struct giveback_urb_bh low_prio_bh;
    struct mutex *address0_mutex;
    struct mutex *bandwidth_mutex;
    struct usb_hcd *shared_hcd;
    struct usb_hcd *primary_hcd;
    struct dma_pool * pool[4];
    int state;
    struct gen_pool *localmem_pool;
    long unsigned int hcd_priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct usb_hcd {
    struct usb_bus self;
    struct kref kref;
    const char *product_desc;
    int speed;
    char irq_descr[24];
    struct timer_list rh_timer;
    struct urb *status_urb;
    struct work_struct wakeup_work;
    struct work_struct died_work;
    const struct hc_driver *driver;
    struct usb_phy *usb_phy;
    struct usb_phy_roothub *phy_roothub;
    long unsigned int flags;
    enum usb_dev_authorize_policy dev_policy;
    unsigned int rh_registered;
    unsigned int rh_pollable;
    unsigned int msix_enabled;
    unsigned int msi_enabled;
    unsigned int skip_phy_initialization;
    unsigned int uses_new_polling;
    unsigned int wireless;
    unsigned int has_tt;
    unsigned int amd_resume_bug;
    unsigned int can_do_streams;
    unsigned int tpl_support;
    unsigned int cant_recv_wakeups;
    unsigned int irq;
    void *regs;
    resource_size_t rsrc_start;
    resource_size_t rsrc_len;
    unsigned int power_budget;
    struct giveback_urb_bh high_prio_bh;
    struct giveback_urb_bh low_prio_bh;
    struct mutex *address0_mutex;
    struct mutex *bandwidth_mutex;
    struct usb_hcd *shared_hcd;
    struct usb_hcd *primary_hcd;
    struct dma_pool * pool[4];
    int state;
    struct gen_pool *localmem_pool;
    long unsigned int hcd_priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct usb_hcd {
    struct usb_bus self;
    struct kref kref;
    const char *product_desc;
    int speed;
    char irq_descr[24];
    struct timer_list rh_timer;
    struct urb *status_urb;
    struct work_struct wakeup_work;
    struct work_struct died_work;
    const struct hc_driver *driver;
    struct usb_phy *usb_phy;
    struct usb_phy_roothub *phy_roothub;
    long unsigned int flags;
    enum usb_dev_authorize_policy dev_policy;
    unsigned int rh_registered;
    unsigned int rh_pollable;
    unsigned int msix_enabled;
    unsigned int msi_enabled;
    unsigned int skip_phy_initialization;
    unsigned int uses_new_polling;
    unsigned int has_tt;
    unsigned int amd_resume_bug;
    unsigned int can_do_streams;
    unsigned int tpl_support;
    unsigned int cant_recv_wakeups;
    unsigned int irq;
    void *regs;
    resource_size_t rsrc_start;
    resource_size_t rsrc_len;
    unsigned int power_budget;
    struct giveback_urb_bh high_prio_bh;
    struct giveback_urb_bh low_prio_bh;
    struct mutex *address0_mutex;
    struct mutex *bandwidth_mutex;
    struct usb_hcd *shared_hcd;
    struct usb_hcd *primary_hcd;
    struct dma_pool * pool[4];
    int state;
    struct gen_pool *localmem_pool;
    long unsigned int hcd_priv[0];
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
struct usb_hcd {
    struct usb_bus self;
    struct kref kref;
    const char *product_desc;
    int speed;
    char irq_descr[24];
    struct timer_list rh_timer;
    struct urb *status_urb;
    struct work_struct wakeup_work;
    struct work_struct died_work;
    const struct hc_driver *driver;
    struct usb_phy *usb_phy;
    struct usb_phy_roothub *phy_roothub;
    long unsigned int flags;
    enum usb_dev_authorize_policy dev_policy;
    unsigned int rh_registered;
    unsigned int rh_pollable;
    unsigned int msix_enabled;
    unsigned int msi_enabled;
    unsigned int skip_phy_initialization;
    unsigned int uses_new_polling;
    unsigned int wireless;
    unsigned int has_tt;
    unsigned int amd_resume_bug;
    unsigned int can_do_streams;
    unsigned int tpl_support;
    unsigned int cant_recv_wakeups;
    unsigned int irq;
    void *regs;
    resource_size_t rsrc_start;
    resource_size_t rsrc_len;
    unsigned int power_budget;
    struct giveback_urb_bh high_prio_bh;
    struct giveback_urb_bh low_prio_bh;
    struct mutex *address0_mutex;
    struct mutex *bandwidth_mutex;
    struct usb_hcd *shared_hcd;
    struct usb_hcd *primary_hcd;
    struct dma_pool * pool[4];
    int state;
    struct gen_pool *localmem_pool;
    long unsigned int hcd_priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct usb_hcd {
    struct usb_bus self;
    struct kref kref;
    const char *product_desc;
    int speed;
    char irq_descr[24];
    struct timer_list rh_timer;
    struct urb *status_urb;
    struct work_struct wakeup_work;
    struct work_struct died_work;
    const struct hc_driver *driver;
    struct usb_phy *usb_phy;
    struct usb_phy_roothub *phy_roothub;
    long unsigned int flags;
    enum usb_dev_authorize_policy dev_policy;
    unsigned int rh_registered;
    unsigned int rh_pollable;
    unsigned int msix_enabled;
    unsigned int msi_enabled;
    unsigned int skip_phy_initialization;
    unsigned int uses_new_polling;
    unsigned int wireless;
    unsigned int has_tt;
    unsigned int amd_resume_bug;
    unsigned int can_do_streams;
    unsigned int tpl_support;
    unsigned int cant_recv_wakeups;
    unsigned int irq;
    void *regs;
    resource_size_t rsrc_start;
    resource_size_t rsrc_len;
    unsigned int power_budget;
    struct giveback_urb_bh high_prio_bh;
    struct giveback_urb_bh low_prio_bh;
    struct mutex *address0_mutex;
    struct mutex *bandwidth_mutex;
    struct usb_hcd *shared_hcd;
    struct usb_hcd *primary_hcd;
    struct dma_pool * pool[4];
    int state;
    struct gen_pool *localmem_pool;
    long unsigned int hcd_priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct usb_hcd {
    struct usb_bus self;
    struct kref kref;
    const char *product_desc;
    int speed;
    char irq_descr[24];
    struct timer_list rh_timer;
    struct urb *status_urb;
    struct work_struct wakeup_work;
    struct work_struct died_work;
    const struct hc_driver *driver;
    struct usb_phy *usb_phy;
    struct usb_phy_roothub *phy_roothub;
    long unsigned int flags;
    enum usb_dev_authorize_policy dev_policy;
    unsigned int rh_registered;
    unsigned int rh_pollable;
    unsigned int msix_enabled;
    unsigned int msi_enabled;
    unsigned int skip_phy_initialization;
    unsigned int uses_new_polling;
    unsigned int wireless;
    unsigned int has_tt;
    unsigned int amd_resume_bug;
    unsigned int can_do_streams;
    unsigned int tpl_support;
    unsigned int cant_recv_wakeups;
    unsigned int irq;
    void *regs;
    resource_size_t rsrc_start;
    resource_size_t rsrc_len;
    unsigned int power_budget;
    struct giveback_urb_bh high_prio_bh;
    struct giveback_urb_bh low_prio_bh;
    struct mutex *address0_mutex;
    struct mutex *bandwidth_mutex;
    struct usb_hcd *shared_hcd;
    struct usb_hcd *primary_hcd;
    struct dma_pool * pool[4];
    int state;
    struct gen_pool *localmem_pool;
    long unsigned int hcd_priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct usb_hcd {
    struct usb_bus self;
    struct kref kref;
    const char *product_desc;
    int speed;
    char irq_descr[24];
    struct timer_list rh_timer;
    struct urb *status_urb;
    struct work_struct wakeup_work;
    struct work_struct died_work;
    const struct hc_driver *driver;
    struct usb_phy *usb_phy;
    struct usb_phy_roothub *phy_roothub;
    long unsigned int flags;
    enum usb_dev_authorize_policy dev_policy;
    unsigned int rh_registered;
    unsigned int rh_pollable;
    unsigned int msix_enabled;
    unsigned int msi_enabled;
    unsigned int skip_phy_initialization;
    unsigned int uses_new_polling;
    unsigned int wireless;
    unsigned int has_tt;
    unsigned int amd_resume_bug;
    unsigned int can_do_streams;
    unsigned int tpl_support;
    unsigned int cant_recv_wakeups;
    unsigned int irq;
    void *regs;
    resource_size_t rsrc_start;
    resource_size_t rsrc_len;
    unsigned int power_budget;
    struct giveback_urb_bh high_prio_bh;
    struct giveback_urb_bh low_prio_bh;
    struct mutex *address0_mutex;
    struct mutex *bandwidth_mutex;
    struct usb_hcd *shared_hcd;
    struct usb_hcd *primary_hcd;
    struct dma_pool * pool[4];
    int state;
    struct gen_pool *localmem_pool;
    long unsigned int hcd_priv[0];
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
struct usb_hcd {
    struct usb_bus self;
    struct kref kref;
    const char *product_desc;
    int speed;
    char irq_descr[24];
    struct timer_list rh_timer;
    struct urb *status_urb;
    struct work_struct wakeup_work;
    struct work_struct died_work;
    const struct hc_driver *driver;
    struct usb_phy *usb_phy;
    struct usb_phy_roothub *phy_roothub;
    long unsigned int flags;
    enum usb_dev_authorize_policy dev_policy;
    unsigned int rh_registered;
    unsigned int rh_pollable;
    unsigned int msix_enabled;
    unsigned int msi_enabled;
    unsigned int skip_phy_initialization;
    unsigned int uses_new_polling;
    unsigned int wireless;
    unsigned int has_tt;
    unsigned int amd_resume_bug;
    unsigned int can_do_streams;
    unsigned int tpl_support;
    unsigned int cant_recv_wakeups;
    unsigned int irq;
    void *regs;
    resource_size_t rsrc_start;
    resource_size_t rsrc_len;
    unsigned int power_budget;
    struct giveback_urb_bh high_prio_bh;
    struct giveback_urb_bh low_prio_bh;
    struct mutex *address0_mutex;
    struct mutex *bandwidth_mutex;
    struct usb_hcd *shared_hcd;
    struct usb_hcd *primary_hcd;
    struct dma_pool * pool[4];
    int state;
    struct gen_pool *localmem_pool;
    long unsigned int hcd_priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct usb_hcd {
    struct usb_bus self;
    struct kref kref;
    const char *product_desc;
    int speed;
    char irq_descr[24];
    struct timer_list rh_timer;
    struct urb *status_urb;
    struct work_struct wakeup_work;
    struct work_struct died_work;
    const struct hc_driver *driver;
    struct usb_phy *usb_phy;
    struct usb_phy_roothub *phy_roothub;
    long unsigned int flags;
    enum usb_dev_authorize_policy dev_policy;
    unsigned int rh_registered;
    unsigned int rh_pollable;
    unsigned int msix_enabled;
    unsigned int msi_enabled;
    unsigned int skip_phy_initialization;
    unsigned int uses_new_polling;
    unsigned int wireless;
    unsigned int has_tt;
    unsigned int amd_resume_bug;
    unsigned int can_do_streams;
    unsigned int tpl_support;
    unsigned int cant_recv_wakeups;
    unsigned int irq;
    void *regs;
    resource_size_t rsrc_start;
    resource_size_t rsrc_len;
    unsigned int power_budget;
    struct giveback_urb_bh high_prio_bh;
    struct giveback_urb_bh low_prio_bh;
    struct mutex *address0_mutex;
    struct mutex *bandwidth_mutex;
    struct usb_hcd *shared_hcd;
    struct usb_hcd *primary_hcd;
    struct dma_pool * pool[4];
    int state;
    struct gen_pool *localmem_pool;
    long unsigned int hcd_priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct usb_hcd {
    struct usb_bus self;
    struct kref kref;
    const char *product_desc;
    int speed;
    char irq_descr[24];
    struct timer_list rh_timer;
    struct urb *status_urb;
    struct work_struct wakeup_work;
    struct work_struct died_work;
    const struct hc_driver *driver;
    struct usb_phy *usb_phy;
    struct usb_phy_roothub *phy_roothub;
    long unsigned int flags;
    enum usb_dev_authorize_policy dev_policy;
    unsigned int rh_registered;
    unsigned int rh_pollable;
    unsigned int msix_enabled;
    unsigned int msi_enabled;
    unsigned int skip_phy_initialization;
    unsigned int uses_new_polling;
    unsigned int wireless;
    unsigned int has_tt;
    unsigned int amd_resume_bug;
    unsigned int can_do_streams;
    unsigned int tpl_support;
    unsigned int cant_recv_wakeups;
    unsigned int irq;
    void *regs;
    resource_size_t rsrc_start;
    resource_size_t rsrc_len;
    unsigned int power_budget;
    struct giveback_urb_bh high_prio_bh;
    struct giveback_urb_bh low_prio_bh;
    struct mutex *address0_mutex;
    struct mutex *bandwidth_mutex;
    struct usb_hcd *shared_hcd;
    struct usb_hcd *primary_hcd;
    struct dma_pool * pool[4];
    int state;
    struct gen_pool *localmem_pool;
    long unsigned int hcd_priv[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct usb_hcd {
    struct usb_bus self;
    struct kref kref;
    const char *product_desc;
    int speed;
    char irq_descr[24];
    struct timer_list rh_timer;
    struct urb *status_urb;
    struct work_struct wakeup_work;
    struct work_struct died_work;
    const struct hc_driver *driver;
    struct usb_phy *usb_phy;
    struct usb_phy_roothub *phy_roothub;
    long unsigned int flags;
    enum usb_dev_authorize_policy dev_policy;
    unsigned int rh_registered;
    unsigned int rh_pollable;
    unsigned int msix_enabled;
    unsigned int msi_enabled;
    unsigned int skip_phy_initialization;
    unsigned int uses_new_polling;
    unsigned int wireless;
    unsigned int has_tt;
    unsigned int amd_resume_bug;
    unsigned int can_do_streams;
    unsigned int tpl_support;
    unsigned int cant_recv_wakeups;
    unsigned int irq;
    void *regs;
    resource_size_t rsrc_start;
    resource_size_t rsrc_len;
    unsigned int power_budget;
    struct giveback_urb_bh high_prio_bh;
    struct giveback_urb_bh low_prio_bh;
    struct mutex *address0_mutex;
    struct mutex *bandwidth_mutex;
    struct usb_hcd *shared_hcd;
    struct usb_hcd *primary_hcd;
    struct dma_pool * pool[4];
    int state;
    struct gen_pool *localmem_pool;
    long unsigned int hcd_priv[0];
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
<code>struct mutex *address0_mutex</code>
</li>
</ul>
</details>
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
<code>unsigned int msi_enabled</code>
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
<code>struct usb_phy_roothub *phy_roothub</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int skip_phy_initialization</code>
</li>
<li>
<b>Field removed. </b>
<code>struct phy *phy</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int remove_phy</code>
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
<code>struct work_struct died_work</code>
</li>
<li>
<b>Field added. </b>
<code>enum usb_dev_authorize_policy dev_policy</code>
</li>
<li>
<b>Field added. </b>
<code>struct gen_pool *localmem_pool</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned int wireless</code>
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
