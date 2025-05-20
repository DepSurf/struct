# Struct: <code>usb_phy</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct usb_phy {
    struct device *dev;
    const char *label;
    unsigned int flags;
    enum usb_phy_type type;
    enum usb_phy_events last_event;
    struct usb_otg *otg;
    struct device *io_dev;
    struct usb_phy_io_ops *io_ops;
    void *io_priv;
    struct atomic_notifier_head notifier;
    u16 port_status;
    u16 port_change;
    struct list_head head;
    int (*init)(struct usb_phy *);
    void (*shutdown)(struct usb_phy *);
    int (*set_vbus)(struct usb_phy *, int);
    int (*set_power)(struct usb_phy *, unsigned int);
    int (*set_suspend)(struct usb_phy *, int);
    int (*set_wakeup)(struct usb_phy *, bool);
    int (*notify_connect)(struct usb_phy *, enum usb_device_speed);
    int (*notify_disconnect)(struct usb_phy *, enum usb_device_speed);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct usb_phy {
    struct device *dev;
    const char *label;
    unsigned int flags;
    enum usb_phy_type type;
    enum usb_phy_events last_event;
    struct usb_otg *otg;
    struct device *io_dev;
    struct usb_phy_io_ops *io_ops;
    void *io_priv;
    struct atomic_notifier_head notifier;
    u16 port_status;
    u16 port_change;
    struct list_head head;
    int (*init)(struct usb_phy *);
    void (*shutdown)(struct usb_phy *);
    int (*set_vbus)(struct usb_phy *, int);
    int (*set_power)(struct usb_phy *, unsigned int);
    int (*set_suspend)(struct usb_phy *, int);
    int (*set_wakeup)(struct usb_phy *, bool);
    int (*notify_connect)(struct usb_phy *, enum usb_device_speed);
    int (*notify_disconnect)(struct usb_phy *, enum usb_device_speed);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct usb_phy {
    struct device *dev;
    const char *label;
    unsigned int flags;
    enum usb_phy_type type;
    enum usb_phy_events last_event;
    struct usb_otg *otg;
    struct device *io_dev;
    struct usb_phy_io_ops *io_ops;
    void *io_priv;
    struct atomic_notifier_head notifier;
    u16 port_status;
    u16 port_change;
    struct list_head head;
    int (*init)(struct usb_phy *);
    void (*shutdown)(struct usb_phy *);
    int (*set_vbus)(struct usb_phy *, int);
    int (*set_power)(struct usb_phy *, unsigned int);
    int (*set_suspend)(struct usb_phy *, int);
    int (*set_wakeup)(struct usb_phy *, bool);
    int (*notify_connect)(struct usb_phy *, enum usb_device_speed);
    int (*notify_disconnect)(struct usb_phy *, enum usb_device_speed);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct usb_phy {
    struct device *dev;
    const char *label;
    unsigned int flags;
    enum usb_phy_type type;
    enum usb_phy_events last_event;
    struct usb_otg *otg;
    struct device *io_dev;
    struct usb_phy_io_ops *io_ops;
    void *io_priv;
    struct extcon_dev *edev;
    struct extcon_dev *id_edev;
    struct notifier_block vbus_nb;
    struct notifier_block id_nb;
    struct atomic_notifier_head notifier;
    u16 port_status;
    u16 port_change;
    struct list_head head;
    int (*init)(struct usb_phy *);
    void (*shutdown)(struct usb_phy *);
    int (*set_vbus)(struct usb_phy *, int);
    int (*set_power)(struct usb_phy *, unsigned int);
    int (*set_suspend)(struct usb_phy *, int);
    int (*set_wakeup)(struct usb_phy *, bool);
    int (*notify_connect)(struct usb_phy *, enum usb_device_speed);
    int (*notify_disconnect)(struct usb_phy *, enum usb_device_speed);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct usb_phy {
    struct device *dev;
    const char *label;
    unsigned int flags;
    enum usb_phy_type type;
    enum usb_phy_events last_event;
    struct usb_otg *otg;
    struct device *io_dev;
    struct usb_phy_io_ops *io_ops;
    void *io_priv;
    struct extcon_dev *edev;
    struct extcon_dev *id_edev;
    struct notifier_block vbus_nb;
    struct notifier_block id_nb;
    struct notifier_block type_nb;
    enum usb_charger_type chg_type;
    enum usb_charger_state chg_state;
    struct usb_charger_current chg_cur;
    struct work_struct chg_work;
    struct atomic_notifier_head notifier;
    u16 port_status;
    u16 port_change;
    struct list_head head;
    int (*init)(struct usb_phy *);
    void (*shutdown)(struct usb_phy *);
    int (*set_vbus)(struct usb_phy *, int);
    int (*set_power)(struct usb_phy *, unsigned int);
    int (*set_suspend)(struct usb_phy *, int);
    int (*set_wakeup)(struct usb_phy *, bool);
    int (*notify_connect)(struct usb_phy *, enum usb_device_speed);
    int (*notify_disconnect)(struct usb_phy *, enum usb_device_speed);
    enum usb_charger_type (*charger_detect)(struct usb_phy *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct usb_phy {
    struct device *dev;
    const char *label;
    unsigned int flags;
    enum usb_phy_type type;
    enum usb_phy_events last_event;
    struct usb_otg *otg;
    struct device *io_dev;
    struct usb_phy_io_ops *io_ops;
    void *io_priv;
    struct extcon_dev *edev;
    struct extcon_dev *id_edev;
    struct notifier_block vbus_nb;
    struct notifier_block id_nb;
    struct notifier_block type_nb;
    enum usb_charger_type chg_type;
    enum usb_charger_state chg_state;
    struct usb_charger_current chg_cur;
    struct work_struct chg_work;
    struct atomic_notifier_head notifier;
    u16 port_status;
    u16 port_change;
    struct list_head head;
    int (*init)(struct usb_phy *);
    void (*shutdown)(struct usb_phy *);
    int (*set_vbus)(struct usb_phy *, int);
    int (*set_power)(struct usb_phy *, unsigned int);
    int (*set_suspend)(struct usb_phy *, int);
    int (*set_wakeup)(struct usb_phy *, bool);
    int (*notify_connect)(struct usb_phy *, enum usb_device_speed);
    int (*notify_disconnect)(struct usb_phy *, enum usb_device_speed);
    enum usb_charger_type (*charger_detect)(struct usb_phy *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct usb_phy {
    struct device *dev;
    const char *label;
    unsigned int flags;
    enum usb_phy_type type;
    enum usb_phy_events last_event;
    struct usb_otg *otg;
    struct device *io_dev;
    struct usb_phy_io_ops *io_ops;
    void *io_priv;
    struct extcon_dev *edev;
    struct extcon_dev *id_edev;
    struct notifier_block vbus_nb;
    struct notifier_block id_nb;
    struct notifier_block type_nb;
    enum usb_charger_type chg_type;
    enum usb_charger_state chg_state;
    struct usb_charger_current chg_cur;
    struct work_struct chg_work;
    struct atomic_notifier_head notifier;
    u16 port_status;
    u16 port_change;
    struct list_head head;
    int (*init)(struct usb_phy *);
    void (*shutdown)(struct usb_phy *);
    int (*set_vbus)(struct usb_phy *, int);
    int (*set_power)(struct usb_phy *, unsigned int);
    int (*set_suspend)(struct usb_phy *, int);
    int (*set_wakeup)(struct usb_phy *, bool);
    int (*notify_connect)(struct usb_phy *, enum usb_device_speed);
    int (*notify_disconnect)(struct usb_phy *, enum usb_device_speed);
    enum usb_charger_type (*charger_detect)(struct usb_phy *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct usb_phy {
    struct device *dev;
    const char *label;
    unsigned int flags;
    enum usb_phy_type type;
    enum usb_phy_events last_event;
    struct usb_otg *otg;
    struct device *io_dev;
    struct usb_phy_io_ops *io_ops;
    void *io_priv;
    struct extcon_dev *edev;
    struct extcon_dev *id_edev;
    struct notifier_block vbus_nb;
    struct notifier_block id_nb;
    struct notifier_block type_nb;
    enum usb_charger_type chg_type;
    enum usb_charger_state chg_state;
    struct usb_charger_current chg_cur;
    struct work_struct chg_work;
    struct atomic_notifier_head notifier;
    u16 port_status;
    u16 port_change;
    struct list_head head;
    int (*init)(struct usb_phy *);
    void (*shutdown)(struct usb_phy *);
    int (*set_vbus)(struct usb_phy *, int);
    int (*set_power)(struct usb_phy *, unsigned int);
    int (*set_suspend)(struct usb_phy *, int);
    int (*set_wakeup)(struct usb_phy *, bool);
    int (*notify_connect)(struct usb_phy *, enum usb_device_speed);
    int (*notify_disconnect)(struct usb_phy *, enum usb_device_speed);
    enum usb_charger_type (*charger_detect)(struct usb_phy *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct usb_phy {
    struct device *dev;
    const char *label;
    unsigned int flags;
    enum usb_phy_type type;
    enum usb_phy_events last_event;
    struct usb_otg *otg;
    struct device *io_dev;
    struct usb_phy_io_ops *io_ops;
    void *io_priv;
    struct extcon_dev *edev;
    struct extcon_dev *id_edev;
    struct notifier_block vbus_nb;
    struct notifier_block id_nb;
    struct notifier_block type_nb;
    enum usb_charger_type chg_type;
    enum usb_charger_state chg_state;
    struct usb_charger_current chg_cur;
    struct work_struct chg_work;
    struct atomic_notifier_head notifier;
    u16 port_status;
    u16 port_change;
    struct list_head head;
    int (*init)(struct usb_phy *);
    void (*shutdown)(struct usb_phy *);
    int (*set_vbus)(struct usb_phy *, int);
    int (*set_power)(struct usb_phy *, unsigned int);
    int (*set_suspend)(struct usb_phy *, int);
    int (*set_wakeup)(struct usb_phy *, bool);
    int (*notify_connect)(struct usb_phy *, enum usb_device_speed);
    int (*notify_disconnect)(struct usb_phy *, enum usb_device_speed);
    enum usb_charger_type (*charger_detect)(struct usb_phy *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct usb_phy {
    struct device *dev;
    const char *label;
    unsigned int flags;
    enum usb_phy_type type;
    enum usb_phy_events last_event;
    struct usb_otg *otg;
    struct device *io_dev;
    struct usb_phy_io_ops *io_ops;
    void *io_priv;
    struct extcon_dev *edev;
    struct extcon_dev *id_edev;
    struct notifier_block vbus_nb;
    struct notifier_block id_nb;
    struct notifier_block type_nb;
    enum usb_charger_type chg_type;
    enum usb_charger_state chg_state;
    struct usb_charger_current chg_cur;
    struct work_struct chg_work;
    struct atomic_notifier_head notifier;
    u16 port_status;
    u16 port_change;
    struct list_head head;
    int (*init)(struct usb_phy *);
    void (*shutdown)(struct usb_phy *);
    int (*set_vbus)(struct usb_phy *, int);
    int (*set_power)(struct usb_phy *, unsigned int);
    int (*set_suspend)(struct usb_phy *, int);
    int (*set_wakeup)(struct usb_phy *, bool);
    int (*notify_connect)(struct usb_phy *, enum usb_device_speed);
    int (*notify_disconnect)(struct usb_phy *, enum usb_device_speed);
    enum usb_charger_type (*charger_detect)(struct usb_phy *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct usb_phy {
    struct device *dev;
    const char *label;
    unsigned int flags;
    enum usb_phy_type type;
    enum usb_phy_events last_event;
    struct usb_otg *otg;
    struct device *io_dev;
    struct usb_phy_io_ops *io_ops;
    void *io_priv;
    struct extcon_dev *edev;
    struct extcon_dev *id_edev;
    struct notifier_block vbus_nb;
    struct notifier_block id_nb;
    struct notifier_block type_nb;
    enum usb_charger_type chg_type;
    enum usb_charger_state chg_state;
    struct usb_charger_current chg_cur;
    struct work_struct chg_work;
    struct atomic_notifier_head notifier;
    u16 port_status;
    u16 port_change;
    struct list_head head;
    int (*init)(struct usb_phy *);
    void (*shutdown)(struct usb_phy *);
    int (*set_vbus)(struct usb_phy *, int);
    int (*set_power)(struct usb_phy *, unsigned int);
    int (*set_suspend)(struct usb_phy *, int);
    int (*set_wakeup)(struct usb_phy *, bool);
    int (*notify_connect)(struct usb_phy *, enum usb_device_speed);
    int (*notify_disconnect)(struct usb_phy *, enum usb_device_speed);
    enum usb_charger_type (*charger_detect)(struct usb_phy *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct usb_phy {
    struct device *dev;
    const char *label;
    unsigned int flags;
    enum usb_phy_type type;
    enum usb_phy_events last_event;
    struct usb_otg *otg;
    struct device *io_dev;
    struct usb_phy_io_ops *io_ops;
    void *io_priv;
    struct extcon_dev *edev;
    struct extcon_dev *id_edev;
    struct notifier_block vbus_nb;
    struct notifier_block id_nb;
    struct notifier_block type_nb;
    enum usb_charger_type chg_type;
    enum usb_charger_state chg_state;
    struct usb_charger_current chg_cur;
    struct work_struct chg_work;
    struct atomic_notifier_head notifier;
    u16 port_status;
    u16 port_change;
    struct list_head head;
    int (*init)(struct usb_phy *);
    void (*shutdown)(struct usb_phy *);
    int (*set_vbus)(struct usb_phy *, int);
    int (*set_power)(struct usb_phy *, unsigned int);
    int (*set_suspend)(struct usb_phy *, int);
    int (*set_wakeup)(struct usb_phy *, bool);
    int (*notify_connect)(struct usb_phy *, enum usb_device_speed);
    int (*notify_disconnect)(struct usb_phy *, enum usb_device_speed);
    enum usb_charger_type (*charger_detect)(struct usb_phy *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct usb_phy {
    struct device *dev;
    const char *label;
    unsigned int flags;
    enum usb_phy_type type;
    enum usb_phy_events last_event;
    struct usb_otg *otg;
    struct device *io_dev;
    struct usb_phy_io_ops *io_ops;
    void *io_priv;
    struct extcon_dev *edev;
    struct extcon_dev *id_edev;
    struct notifier_block vbus_nb;
    struct notifier_block id_nb;
    struct notifier_block type_nb;
    enum usb_charger_type chg_type;
    enum usb_charger_state chg_state;
    struct usb_charger_current chg_cur;
    struct work_struct chg_work;
    struct atomic_notifier_head notifier;
    u16 port_status;
    u16 port_change;
    struct list_head head;
    int (*init)(struct usb_phy *);
    void (*shutdown)(struct usb_phy *);
    int (*set_vbus)(struct usb_phy *, int);
    int (*set_power)(struct usb_phy *, unsigned int);
    int (*set_suspend)(struct usb_phy *, int);
    int (*set_wakeup)(struct usb_phy *, bool);
    int (*notify_connect)(struct usb_phy *, enum usb_device_speed);
    int (*notify_disconnect)(struct usb_phy *, enum usb_device_speed);
    enum usb_charger_type (*charger_detect)(struct usb_phy *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct usb_phy {
    struct device *dev;
    const char *label;
    unsigned int flags;
    enum usb_phy_type type;
    enum usb_phy_events last_event;
    struct usb_otg *otg;
    struct device *io_dev;
    struct usb_phy_io_ops *io_ops;
    void *io_priv;
    struct extcon_dev *edev;
    struct extcon_dev *id_edev;
    struct notifier_block vbus_nb;
    struct notifier_block id_nb;
    struct notifier_block type_nb;
    enum usb_charger_type chg_type;
    enum usb_charger_state chg_state;
    struct usb_charger_current chg_cur;
    struct work_struct chg_work;
    struct atomic_notifier_head notifier;
    u16 port_status;
    u16 port_change;
    struct list_head head;
    int (*init)(struct usb_phy *);
    void (*shutdown)(struct usb_phy *);
    int (*set_vbus)(struct usb_phy *, int);
    int (*set_power)(struct usb_phy *, unsigned int);
    int (*set_suspend)(struct usb_phy *, int);
    int (*set_wakeup)(struct usb_phy *, bool);
    int (*notify_connect)(struct usb_phy *, enum usb_device_speed);
    int (*notify_disconnect)(struct usb_phy *, enum usb_device_speed);
    enum usb_charger_type (*charger_detect)(struct usb_phy *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct usb_phy {
    struct device *dev;
    const char *label;
    unsigned int flags;
    enum usb_phy_type type;
    enum usb_phy_events last_event;
    struct usb_otg *otg;
    struct device *io_dev;
    struct usb_phy_io_ops *io_ops;
    void *io_priv;
    struct extcon_dev *edev;
    struct extcon_dev *id_edev;
    struct notifier_block vbus_nb;
    struct notifier_block id_nb;
    struct notifier_block type_nb;
    enum usb_charger_type chg_type;
    enum usb_charger_state chg_state;
    struct usb_charger_current chg_cur;
    struct work_struct chg_work;
    struct atomic_notifier_head notifier;
    u16 port_status;
    u16 port_change;
    struct list_head head;
    int (*init)(struct usb_phy *);
    void (*shutdown)(struct usb_phy *);
    int (*set_vbus)(struct usb_phy *, int);
    int (*set_power)(struct usb_phy *, unsigned int);
    int (*set_suspend)(struct usb_phy *, int);
    int (*set_wakeup)(struct usb_phy *, bool);
    int (*notify_connect)(struct usb_phy *, enum usb_device_speed);
    int (*notify_disconnect)(struct usb_phy *, enum usb_device_speed);
    enum usb_charger_type (*charger_detect)(struct usb_phy *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct usb_phy {
    struct device *dev;
    const char *label;
    unsigned int flags;
    enum usb_phy_type type;
    enum usb_phy_events last_event;
    struct usb_otg *otg;
    struct device *io_dev;
    struct usb_phy_io_ops *io_ops;
    void *io_priv;
    struct extcon_dev *edev;
    struct extcon_dev *id_edev;
    struct notifier_block vbus_nb;
    struct notifier_block id_nb;
    struct notifier_block type_nb;
    enum usb_charger_type chg_type;
    enum usb_charger_state chg_state;
    struct usb_charger_current chg_cur;
    struct work_struct chg_work;
    struct atomic_notifier_head notifier;
    u16 port_status;
    u16 port_change;
    struct list_head head;
    int (*init)(struct usb_phy *);
    void (*shutdown)(struct usb_phy *);
    int (*set_vbus)(struct usb_phy *, int);
    int (*set_power)(struct usb_phy *, unsigned int);
    int (*set_suspend)(struct usb_phy *, int);
    int (*set_wakeup)(struct usb_phy *, bool);
    int (*notify_connect)(struct usb_phy *, enum usb_device_speed);
    int (*notify_disconnect)(struct usb_phy *, enum usb_device_speed);
    enum usb_charger_type (*charger_detect)(struct usb_phy *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct usb_phy {
    struct device *dev;
    const char *label;
    unsigned int flags;
    enum usb_phy_type type;
    enum usb_phy_events last_event;
    struct usb_otg *otg;
    struct device *io_dev;
    struct usb_phy_io_ops *io_ops;
    void *io_priv;
    struct extcon_dev *edev;
    struct extcon_dev *id_edev;
    struct notifier_block vbus_nb;
    struct notifier_block id_nb;
    struct notifier_block type_nb;
    enum usb_charger_type chg_type;
    enum usb_charger_state chg_state;
    struct usb_charger_current chg_cur;
    struct work_struct chg_work;
    struct atomic_notifier_head notifier;
    u16 port_status;
    u16 port_change;
    struct list_head head;
    int (*init)(struct usb_phy *);
    void (*shutdown)(struct usb_phy *);
    int (*set_vbus)(struct usb_phy *, int);
    int (*set_power)(struct usb_phy *, unsigned int);
    int (*set_suspend)(struct usb_phy *, int);
    int (*set_wakeup)(struct usb_phy *, bool);
    int (*notify_connect)(struct usb_phy *, enum usb_device_speed);
    int (*notify_disconnect)(struct usb_phy *, enum usb_device_speed);
    enum usb_charger_type (*charger_detect)(struct usb_phy *);
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
struct usb_phy {
    struct device *dev;
    const char *label;
    unsigned int flags;
    enum usb_phy_type type;
    enum usb_phy_events last_event;
    struct usb_otg *otg;
    struct device *io_dev;
    struct usb_phy_io_ops *io_ops;
    void *io_priv;
    struct extcon_dev *edev;
    struct extcon_dev *id_edev;
    struct notifier_block vbus_nb;
    struct notifier_block id_nb;
    struct notifier_block type_nb;
    enum usb_charger_type chg_type;
    enum usb_charger_state chg_state;
    struct usb_charger_current chg_cur;
    struct work_struct chg_work;
    struct atomic_notifier_head notifier;
    u16 port_status;
    u16 port_change;
    struct list_head head;
    int (*init)(struct usb_phy *);
    void (*shutdown)(struct usb_phy *);
    int (*set_vbus)(struct usb_phy *, int);
    int (*set_power)(struct usb_phy *, unsigned int);
    int (*set_suspend)(struct usb_phy *, int);
    int (*set_wakeup)(struct usb_phy *, bool);
    int (*notify_connect)(struct usb_phy *, enum usb_device_speed);
    int (*notify_disconnect)(struct usb_phy *, enum usb_device_speed);
    enum usb_charger_type (*charger_detect)(struct usb_phy *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct usb_phy {
    struct device *dev;
    const char *label;
    unsigned int flags;
    enum usb_phy_type type;
    enum usb_phy_events last_event;
    struct usb_otg *otg;
    struct device *io_dev;
    struct usb_phy_io_ops *io_ops;
    void *io_priv;
    struct extcon_dev *edev;
    struct extcon_dev *id_edev;
    struct notifier_block vbus_nb;
    struct notifier_block id_nb;
    struct notifier_block type_nb;
    enum usb_charger_type chg_type;
    enum usb_charger_state chg_state;
    struct usb_charger_current chg_cur;
    struct work_struct chg_work;
    struct atomic_notifier_head notifier;
    u16 port_status;
    u16 port_change;
    struct list_head head;
    int (*init)(struct usb_phy *);
    void (*shutdown)(struct usb_phy *);
    int (*set_vbus)(struct usb_phy *, int);
    int (*set_power)(struct usb_phy *, unsigned int);
    int (*set_suspend)(struct usb_phy *, int);
    int (*set_wakeup)(struct usb_phy *, bool);
    int (*notify_connect)(struct usb_phy *, enum usb_device_speed);
    int (*notify_disconnect)(struct usb_phy *, enum usb_device_speed);
    enum usb_charger_type (*charger_detect)(struct usb_phy *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct usb_phy {
    struct device *dev;
    const char *label;
    unsigned int flags;
    enum usb_phy_type type;
    enum usb_phy_events last_event;
    struct usb_otg *otg;
    struct device *io_dev;
    struct usb_phy_io_ops *io_ops;
    void *io_priv;
    struct extcon_dev *edev;
    struct extcon_dev *id_edev;
    struct notifier_block vbus_nb;
    struct notifier_block id_nb;
    struct notifier_block type_nb;
    enum usb_charger_type chg_type;
    enum usb_charger_state chg_state;
    struct usb_charger_current chg_cur;
    struct work_struct chg_work;
    struct atomic_notifier_head notifier;
    u16 port_status;
    u16 port_change;
    struct list_head head;
    int (*init)(struct usb_phy *);
    void (*shutdown)(struct usb_phy *);
    int (*set_vbus)(struct usb_phy *, int);
    int (*set_power)(struct usb_phy *, unsigned int);
    int (*set_suspend)(struct usb_phy *, int);
    int (*set_wakeup)(struct usb_phy *, bool);
    int (*notify_connect)(struct usb_phy *, enum usb_device_speed);
    int (*notify_disconnect)(struct usb_phy *, enum usb_device_speed);
    enum usb_charger_type (*charger_detect)(struct usb_phy *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct usb_phy {
    struct device *dev;
    const char *label;
    unsigned int flags;
    enum usb_phy_type type;
    enum usb_phy_events last_event;
    struct usb_otg *otg;
    struct device *io_dev;
    struct usb_phy_io_ops *io_ops;
    void *io_priv;
    struct extcon_dev *edev;
    struct extcon_dev *id_edev;
    struct notifier_block vbus_nb;
    struct notifier_block id_nb;
    struct notifier_block type_nb;
    enum usb_charger_type chg_type;
    enum usb_charger_state chg_state;
    struct usb_charger_current chg_cur;
    struct work_struct chg_work;
    struct atomic_notifier_head notifier;
    u16 port_status;
    u16 port_change;
    struct list_head head;
    int (*init)(struct usb_phy *);
    void (*shutdown)(struct usb_phy *);
    int (*set_vbus)(struct usb_phy *, int);
    int (*set_power)(struct usb_phy *, unsigned int);
    int (*set_suspend)(struct usb_phy *, int);
    int (*set_wakeup)(struct usb_phy *, bool);
    int (*notify_connect)(struct usb_phy *, enum usb_device_speed);
    int (*notify_disconnect)(struct usb_phy *, enum usb_device_speed);
    enum usb_charger_type (*charger_detect)(struct usb_phy *);
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
struct usb_phy {
    struct device *dev;
    const char *label;
    unsigned int flags;
    enum usb_phy_type type;
    enum usb_phy_events last_event;
    struct usb_otg *otg;
    struct device *io_dev;
    struct usb_phy_io_ops *io_ops;
    void *io_priv;
    struct extcon_dev *edev;
    struct extcon_dev *id_edev;
    struct notifier_block vbus_nb;
    struct notifier_block id_nb;
    struct notifier_block type_nb;
    enum usb_charger_type chg_type;
    enum usb_charger_state chg_state;
    struct usb_charger_current chg_cur;
    struct work_struct chg_work;
    struct atomic_notifier_head notifier;
    u16 port_status;
    u16 port_change;
    struct list_head head;
    int (*init)(struct usb_phy *);
    void (*shutdown)(struct usb_phy *);
    int (*set_vbus)(struct usb_phy *, int);
    int (*set_power)(struct usb_phy *, unsigned int);
    int (*set_suspend)(struct usb_phy *, int);
    int (*set_wakeup)(struct usb_phy *, bool);
    int (*notify_connect)(struct usb_phy *, enum usb_device_speed);
    int (*notify_disconnect)(struct usb_phy *, enum usb_device_speed);
    enum usb_charger_type (*charger_detect)(struct usb_phy *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct usb_phy {
    struct device *dev;
    const char *label;
    unsigned int flags;
    enum usb_phy_type type;
    enum usb_phy_events last_event;
    struct usb_otg *otg;
    struct device *io_dev;
    struct usb_phy_io_ops *io_ops;
    void *io_priv;
    struct extcon_dev *edev;
    struct extcon_dev *id_edev;
    struct notifier_block vbus_nb;
    struct notifier_block id_nb;
    struct notifier_block type_nb;
    enum usb_charger_type chg_type;
    enum usb_charger_state chg_state;
    struct usb_charger_current chg_cur;
    struct work_struct chg_work;
    struct atomic_notifier_head notifier;
    u16 port_status;
    u16 port_change;
    struct list_head head;
    int (*init)(struct usb_phy *);
    void (*shutdown)(struct usb_phy *);
    int (*set_vbus)(struct usb_phy *, int);
    int (*set_power)(struct usb_phy *, unsigned int);
    int (*set_suspend)(struct usb_phy *, int);
    int (*set_wakeup)(struct usb_phy *, bool);
    int (*notify_connect)(struct usb_phy *, enum usb_device_speed);
    int (*notify_disconnect)(struct usb_phy *, enum usb_device_speed);
    enum usb_charger_type (*charger_detect)(struct usb_phy *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct usb_phy {
    struct device *dev;
    const char *label;
    unsigned int flags;
    enum usb_phy_type type;
    enum usb_phy_events last_event;
    struct usb_otg *otg;
    struct device *io_dev;
    struct usb_phy_io_ops *io_ops;
    void *io_priv;
    struct extcon_dev *edev;
    struct extcon_dev *id_edev;
    struct notifier_block vbus_nb;
    struct notifier_block id_nb;
    struct notifier_block type_nb;
    enum usb_charger_type chg_type;
    enum usb_charger_state chg_state;
    struct usb_charger_current chg_cur;
    struct work_struct chg_work;
    struct atomic_notifier_head notifier;
    u16 port_status;
    u16 port_change;
    struct list_head head;
    int (*init)(struct usb_phy *);
    void (*shutdown)(struct usb_phy *);
    int (*set_vbus)(struct usb_phy *, int);
    int (*set_power)(struct usb_phy *, unsigned int);
    int (*set_suspend)(struct usb_phy *, int);
    int (*set_wakeup)(struct usb_phy *, bool);
    int (*notify_connect)(struct usb_phy *, enum usb_device_speed);
    int (*notify_disconnect)(struct usb_phy *, enum usb_device_speed);
    enum usb_charger_type (*charger_detect)(struct usb_phy *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct usb_phy {
    struct device *dev;
    const char *label;
    unsigned int flags;
    enum usb_phy_type type;
    enum usb_phy_events last_event;
    struct usb_otg *otg;
    struct device *io_dev;
    struct usb_phy_io_ops *io_ops;
    void *io_priv;
    struct extcon_dev *edev;
    struct extcon_dev *id_edev;
    struct notifier_block vbus_nb;
    struct notifier_block id_nb;
    struct notifier_block type_nb;
    enum usb_charger_type chg_type;
    enum usb_charger_state chg_state;
    struct usb_charger_current chg_cur;
    struct work_struct chg_work;
    struct atomic_notifier_head notifier;
    u16 port_status;
    u16 port_change;
    struct list_head head;
    int (*init)(struct usb_phy *);
    void (*shutdown)(struct usb_phy *);
    int (*set_vbus)(struct usb_phy *, int);
    int (*set_power)(struct usb_phy *, unsigned int);
    int (*set_suspend)(struct usb_phy *, int);
    int (*set_wakeup)(struct usb_phy *, bool);
    int (*notify_connect)(struct usb_phy *, enum usb_device_speed);
    int (*notify_disconnect)(struct usb_phy *, enum usb_device_speed);
    enum usb_charger_type (*charger_detect)(struct usb_phy *);
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
<code>struct extcon_dev *edev</code>
</li>
<li>
<b>Field added. </b>
<code>struct extcon_dev *id_edev</code>
</li>
<li>
<b>Field added. </b>
<code>struct notifier_block vbus_nb</code>
</li>
<li>
<b>Field added. </b>
<code>struct notifier_block id_nb</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct notifier_block type_nb</code>
</li>
<li>
<b>Field added. </b>
<code>enum usb_charger_type chg_type</code>
</li>
<li>
<b>Field added. </b>
<code>enum usb_charger_state chg_state</code>
</li>
<li>
<b>Field added. </b>
<code>struct usb_charger_current chg_cur</code>
</li>
<li>
<b>Field added. </b>
<code>struct work_struct chg_work</code>
</li>
<li>
<b>Field added. </b>
<code>enum usb_charger_type (*charger_detect)(struct usb_phy *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
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
<details>
<summary>Changed between <code>generic</code> and <code>azure</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct extcon_dev *edev</code> ➡️ <code>struct extcon_dev *edev</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct extcon_dev *id_edev</code> ➡️ <code>struct extcon_dev *id_edev</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
