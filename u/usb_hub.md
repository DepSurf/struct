# Struct: <code>usb_hub</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct usb_hub {
    struct device *intfdev;
    struct usb_device *hdev;
    struct kref kref;
    struct urb *urb;
    u8[8] *buffer;
    union (anon) *status;
    struct mutex status_mutex;
    int error;
    int nerrors;
    long unsigned int event_bits[1];
    long unsigned int change_bits[1];
    long unsigned int removed_bits[1];
    long unsigned int wakeup_bits[1];
    long unsigned int power_bits[1];
    long unsigned int child_usage_bits[1];
    long unsigned int warm_reset_bits[1];
    struct usb_hub_descriptor *descriptor;
    struct usb_tt tt;
    unsigned int mA_per_port;
    unsigned int wakeup_enabled_descendants;
    unsigned int limited_power;
    unsigned int quiescing;
    unsigned int disconnected;
    unsigned int in_reset;
    unsigned int quirk_check_port_auto_suspend;
    unsigned int has_indicators;
    u8 indicator[31];
    struct delayed_work leds;
    struct delayed_work init_work;
    struct work_struct events;
    struct usb_port **ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct usb_hub {
    struct device *intfdev;
    struct usb_device *hdev;
    struct kref kref;
    struct urb *urb;
    u8[8] *buffer;
    union (anon) *status;
    struct mutex status_mutex;
    int error;
    int nerrors;
    long unsigned int event_bits[1];
    long unsigned int change_bits[1];
    long unsigned int removed_bits[1];
    long unsigned int wakeup_bits[1];
    long unsigned int power_bits[1];
    long unsigned int child_usage_bits[1];
    long unsigned int warm_reset_bits[1];
    struct usb_hub_descriptor *descriptor;
    struct usb_tt tt;
    unsigned int mA_per_port;
    unsigned int wakeup_enabled_descendants;
    unsigned int limited_power;
    unsigned int quiescing;
    unsigned int disconnected;
    unsigned int in_reset;
    unsigned int quirk_check_port_auto_suspend;
    unsigned int has_indicators;
    u8 indicator[31];
    struct delayed_work leds;
    struct delayed_work init_work;
    struct work_struct events;
    struct usb_port **ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct usb_hub {
    struct device *intfdev;
    struct usb_device *hdev;
    struct kref kref;
    struct urb *urb;
    u8[8] *buffer;
    union (anon) *status;
    struct mutex status_mutex;
    int error;
    int nerrors;
    long unsigned int event_bits[1];
    long unsigned int change_bits[1];
    long unsigned int removed_bits[1];
    long unsigned int wakeup_bits[1];
    long unsigned int power_bits[1];
    long unsigned int child_usage_bits[1];
    long unsigned int warm_reset_bits[1];
    struct usb_hub_descriptor *descriptor;
    struct usb_tt tt;
    unsigned int mA_per_port;
    unsigned int wakeup_enabled_descendants;
    unsigned int limited_power;
    unsigned int quiescing;
    unsigned int disconnected;
    unsigned int in_reset;
    unsigned int quirk_check_port_auto_suspend;
    unsigned int has_indicators;
    u8 indicator[31];
    struct delayed_work leds;
    struct delayed_work init_work;
    struct work_struct events;
    struct usb_port **ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct usb_hub {
    struct device *intfdev;
    struct usb_device *hdev;
    struct kref kref;
    struct urb *urb;
    u8[8] *buffer;
    union (anon) *status;
    struct mutex status_mutex;
    int error;
    int nerrors;
    long unsigned int event_bits[1];
    long unsigned int change_bits[1];
    long unsigned int removed_bits[1];
    long unsigned int wakeup_bits[1];
    long unsigned int power_bits[1];
    long unsigned int child_usage_bits[1];
    long unsigned int warm_reset_bits[1];
    struct usb_hub_descriptor *descriptor;
    struct usb_tt tt;
    unsigned int mA_per_port;
    unsigned int wakeup_enabled_descendants;
    unsigned int limited_power;
    unsigned int quiescing;
    unsigned int disconnected;
    unsigned int in_reset;
    unsigned int quirk_check_port_auto_suspend;
    unsigned int has_indicators;
    u8 indicator[31];
    struct delayed_work leds;
    struct delayed_work init_work;
    struct work_struct events;
    struct usb_port **ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct usb_hub {
    struct device *intfdev;
    struct usb_device *hdev;
    struct kref kref;
    struct urb *urb;
    u8[8] *buffer;
    union (anon) *status;
    struct mutex status_mutex;
    int error;
    int nerrors;
    long unsigned int event_bits[1];
    long unsigned int change_bits[1];
    long unsigned int removed_bits[1];
    long unsigned int wakeup_bits[1];
    long unsigned int power_bits[1];
    long unsigned int child_usage_bits[1];
    long unsigned int warm_reset_bits[1];
    struct usb_hub_descriptor *descriptor;
    struct usb_tt tt;
    unsigned int mA_per_port;
    unsigned int wakeup_enabled_descendants;
    unsigned int limited_power;
    unsigned int quiescing;
    unsigned int disconnected;
    unsigned int in_reset;
    unsigned int quirk_check_port_auto_suspend;
    unsigned int has_indicators;
    u8 indicator[31];
    struct delayed_work leds;
    struct delayed_work init_work;
    struct work_struct events;
    struct usb_port **ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct usb_hub {
    struct device *intfdev;
    struct usb_device *hdev;
    struct kref kref;
    struct urb *urb;
    u8[8] *buffer;
    union (anon) *status;
    struct mutex status_mutex;
    int error;
    int nerrors;
    long unsigned int event_bits[1];
    long unsigned int change_bits[1];
    long unsigned int removed_bits[1];
    long unsigned int wakeup_bits[1];
    long unsigned int power_bits[1];
    long unsigned int child_usage_bits[1];
    long unsigned int warm_reset_bits[1];
    struct usb_hub_descriptor *descriptor;
    struct usb_tt tt;
    unsigned int mA_per_port;
    unsigned int wakeup_enabled_descendants;
    unsigned int limited_power;
    unsigned int quiescing;
    unsigned int disconnected;
    unsigned int in_reset;
    unsigned int quirk_check_port_auto_suspend;
    unsigned int has_indicators;
    u8 indicator[31];
    struct delayed_work leds;
    struct delayed_work init_work;
    struct work_struct events;
    struct usb_port **ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct usb_hub {
    struct device *intfdev;
    struct usb_device *hdev;
    struct kref kref;
    struct urb *urb;
    u8[8] *buffer;
    union (anon) *status;
    struct mutex status_mutex;
    int error;
    int nerrors;
    long unsigned int event_bits[1];
    long unsigned int change_bits[1];
    long unsigned int removed_bits[1];
    long unsigned int wakeup_bits[1];
    long unsigned int power_bits[1];
    long unsigned int child_usage_bits[1];
    long unsigned int warm_reset_bits[1];
    struct usb_hub_descriptor *descriptor;
    struct usb_tt tt;
    unsigned int mA_per_port;
    unsigned int wakeup_enabled_descendants;
    unsigned int limited_power;
    unsigned int quiescing;
    unsigned int disconnected;
    unsigned int in_reset;
    unsigned int quirk_check_port_auto_suspend;
    unsigned int has_indicators;
    u8 indicator[31];
    struct delayed_work leds;
    struct delayed_work init_work;
    struct work_struct events;
    struct usb_port **ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct usb_hub {
    struct device *intfdev;
    struct usb_device *hdev;
    struct kref kref;
    struct urb *urb;
    u8[8] *buffer;
    union (anon) *status;
    struct mutex status_mutex;
    int error;
    int nerrors;
    long unsigned int event_bits[1];
    long unsigned int change_bits[1];
    long unsigned int removed_bits[1];
    long unsigned int wakeup_bits[1];
    long unsigned int power_bits[1];
    long unsigned int child_usage_bits[1];
    long unsigned int warm_reset_bits[1];
    struct usb_hub_descriptor *descriptor;
    struct usb_tt tt;
    unsigned int mA_per_port;
    unsigned int wakeup_enabled_descendants;
    unsigned int limited_power;
    unsigned int quiescing;
    unsigned int disconnected;
    unsigned int in_reset;
    unsigned int quirk_check_port_auto_suspend;
    unsigned int has_indicators;
    u8 indicator[31];
    struct delayed_work leds;
    struct delayed_work init_work;
    struct work_struct events;
    spinlock_t irq_urb_lock;
    struct timer_list irq_urb_retry;
    struct usb_port **ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct usb_hub {
    struct device *intfdev;
    struct usb_device *hdev;
    struct kref kref;
    struct urb *urb;
    u8[8] *buffer;
    union (anon) *status;
    struct mutex status_mutex;
    int error;
    int nerrors;
    long unsigned int event_bits[1];
    long unsigned int change_bits[1];
    long unsigned int removed_bits[1];
    long unsigned int wakeup_bits[1];
    long unsigned int power_bits[1];
    long unsigned int child_usage_bits[1];
    long unsigned int warm_reset_bits[1];
    struct usb_hub_descriptor *descriptor;
    struct usb_tt tt;
    unsigned int mA_per_port;
    unsigned int wakeup_enabled_descendants;
    unsigned int limited_power;
    unsigned int quiescing;
    unsigned int disconnected;
    unsigned int in_reset;
    unsigned int quirk_disable_autosuspend;
    unsigned int quirk_check_port_auto_suspend;
    unsigned int has_indicators;
    u8 indicator[31];
    struct delayed_work leds;
    struct delayed_work init_work;
    struct work_struct events;
    spinlock_t irq_urb_lock;
    struct timer_list irq_urb_retry;
    struct usb_port **ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct usb_hub {
    struct device *intfdev;
    struct usb_device *hdev;
    struct kref kref;
    struct urb *urb;
    u8[8] *buffer;
    union (anon) *status;
    struct mutex status_mutex;
    int error;
    int nerrors;
    long unsigned int event_bits[1];
    long unsigned int change_bits[1];
    long unsigned int removed_bits[1];
    long unsigned int wakeup_bits[1];
    long unsigned int power_bits[1];
    long unsigned int child_usage_bits[1];
    long unsigned int warm_reset_bits[1];
    struct usb_hub_descriptor *descriptor;
    struct usb_tt tt;
    unsigned int mA_per_port;
    unsigned int wakeup_enabled_descendants;
    unsigned int limited_power;
    unsigned int quiescing;
    unsigned int disconnected;
    unsigned int in_reset;
    unsigned int quirk_disable_autosuspend;
    unsigned int quirk_check_port_auto_suspend;
    unsigned int has_indicators;
    u8 indicator[31];
    struct delayed_work leds;
    struct delayed_work init_work;
    struct work_struct events;
    spinlock_t irq_urb_lock;
    struct timer_list irq_urb_retry;
    struct usb_port **ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct usb_hub {
    struct device *intfdev;
    struct usb_device *hdev;
    struct kref kref;
    struct urb *urb;
    u8[8] *buffer;
    union (anon) *status;
    struct mutex status_mutex;
    int error;
    int nerrors;
    long unsigned int event_bits[1];
    long unsigned int change_bits[1];
    long unsigned int removed_bits[1];
    long unsigned int wakeup_bits[1];
    long unsigned int power_bits[1];
    long unsigned int child_usage_bits[1];
    long unsigned int warm_reset_bits[1];
    struct usb_hub_descriptor *descriptor;
    struct usb_tt tt;
    unsigned int mA_per_port;
    unsigned int wakeup_enabled_descendants;
    unsigned int limited_power;
    unsigned int quiescing;
    unsigned int disconnected;
    unsigned int in_reset;
    unsigned int quirk_disable_autosuspend;
    unsigned int quirk_check_port_auto_suspend;
    unsigned int has_indicators;
    u8 indicator[31];
    struct delayed_work leds;
    struct delayed_work init_work;
    struct work_struct events;
    spinlock_t irq_urb_lock;
    struct timer_list irq_urb_retry;
    struct usb_port **ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct usb_hub {
    struct device *intfdev;
    struct usb_device *hdev;
    struct kref kref;
    struct urb *urb;
    u8[8] *buffer;
    union (anon) *status;
    struct mutex status_mutex;
    int error;
    int nerrors;
    long unsigned int event_bits[1];
    long unsigned int change_bits[1];
    long unsigned int removed_bits[1];
    long unsigned int wakeup_bits[1];
    long unsigned int power_bits[1];
    long unsigned int child_usage_bits[1];
    long unsigned int warm_reset_bits[1];
    struct usb_hub_descriptor *descriptor;
    struct usb_tt tt;
    unsigned int mA_per_port;
    unsigned int wakeup_enabled_descendants;
    unsigned int limited_power;
    unsigned int quiescing;
    unsigned int disconnected;
    unsigned int in_reset;
    unsigned int quirk_disable_autosuspend;
    unsigned int quirk_check_port_auto_suspend;
    unsigned int has_indicators;
    u8 indicator[31];
    struct delayed_work leds;
    struct delayed_work init_work;
    struct work_struct events;
    spinlock_t irq_urb_lock;
    struct timer_list irq_urb_retry;
    struct usb_port **ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct usb_hub {
    struct device *intfdev;
    struct usb_device *hdev;
    struct kref kref;
    struct urb *urb;
    u8[8] *buffer;
    union (anon) *status;
    struct mutex status_mutex;
    int error;
    int nerrors;
    long unsigned int event_bits[1];
    long unsigned int change_bits[1];
    long unsigned int removed_bits[1];
    long unsigned int wakeup_bits[1];
    long unsigned int power_bits[1];
    long unsigned int child_usage_bits[1];
    long unsigned int warm_reset_bits[1];
    struct usb_hub_descriptor *descriptor;
    struct usb_tt tt;
    unsigned int mA_per_port;
    unsigned int wakeup_enabled_descendants;
    unsigned int limited_power;
    unsigned int quiescing;
    unsigned int disconnected;
    unsigned int in_reset;
    unsigned int quirk_disable_autosuspend;
    unsigned int quirk_check_port_auto_suspend;
    unsigned int has_indicators;
    u8 indicator[31];
    struct delayed_work leds;
    struct delayed_work init_work;
    struct work_struct events;
    spinlock_t irq_urb_lock;
    struct timer_list irq_urb_retry;
    struct usb_port **ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct usb_hub {
    struct device *intfdev;
    struct usb_device *hdev;
    struct kref kref;
    struct urb *urb;
    u8[8] *buffer;
    union (anon) *status;
    struct mutex status_mutex;
    int error;
    int nerrors;
    long unsigned int event_bits[1];
    long unsigned int change_bits[1];
    long unsigned int removed_bits[1];
    long unsigned int wakeup_bits[1];
    long unsigned int power_bits[1];
    long unsigned int child_usage_bits[1];
    long unsigned int warm_reset_bits[1];
    struct usb_hub_descriptor *descriptor;
    struct usb_tt tt;
    unsigned int mA_per_port;
    unsigned int wakeup_enabled_descendants;
    unsigned int limited_power;
    unsigned int quiescing;
    unsigned int disconnected;
    unsigned int in_reset;
    unsigned int quirk_disable_autosuspend;
    unsigned int quirk_check_port_auto_suspend;
    unsigned int has_indicators;
    u8 indicator[31];
    struct delayed_work leds;
    struct delayed_work init_work;
    struct work_struct events;
    spinlock_t irq_urb_lock;
    struct timer_list irq_urb_retry;
    struct usb_port **ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct usb_hub {
    struct device *intfdev;
    struct usb_device *hdev;
    struct kref kref;
    struct urb *urb;
    u8[8] *buffer;
    union (anon) *status;
    struct mutex status_mutex;
    int error;
    int nerrors;
    long unsigned int event_bits[1];
    long unsigned int change_bits[1];
    long unsigned int removed_bits[1];
    long unsigned int wakeup_bits[1];
    long unsigned int power_bits[1];
    long unsigned int child_usage_bits[1];
    long unsigned int warm_reset_bits[1];
    struct usb_hub_descriptor *descriptor;
    struct usb_tt tt;
    unsigned int mA_per_port;
    unsigned int wakeup_enabled_descendants;
    unsigned int limited_power;
    unsigned int quiescing;
    unsigned int disconnected;
    unsigned int in_reset;
    unsigned int quirk_disable_autosuspend;
    unsigned int quirk_check_port_auto_suspend;
    unsigned int has_indicators;
    u8 indicator[31];
    struct delayed_work leds;
    struct delayed_work init_work;
    struct work_struct events;
    spinlock_t irq_urb_lock;
    struct timer_list irq_urb_retry;
    struct usb_port **ports;
    struct list_head onboard_hub_devs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct usb_hub {
    struct device *intfdev;
    struct usb_device *hdev;
    struct kref kref;
    struct urb *urb;
    u8[8] *buffer;
    union (anon) *status;
    struct mutex status_mutex;
    int error;
    int nerrors;
    long unsigned int event_bits[1];
    long unsigned int change_bits[1];
    long unsigned int removed_bits[1];
    long unsigned int wakeup_bits[1];
    long unsigned int power_bits[1];
    long unsigned int child_usage_bits[1];
    long unsigned int warm_reset_bits[1];
    struct usb_hub_descriptor *descriptor;
    struct usb_tt tt;
    unsigned int mA_per_port;
    unsigned int wakeup_enabled_descendants;
    unsigned int limited_power;
    unsigned int quiescing;
    unsigned int disconnected;
    unsigned int in_reset;
    unsigned int quirk_disable_autosuspend;
    unsigned int quirk_check_port_auto_suspend;
    unsigned int has_indicators;
    u8 indicator[31];
    struct delayed_work leds;
    struct delayed_work init_work;
    struct work_struct events;
    spinlock_t irq_urb_lock;
    struct timer_list irq_urb_retry;
    struct usb_port **ports;
    struct list_head onboard_hub_devs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct usb_hub {
    struct device *intfdev;
    struct usb_device *hdev;
    struct kref kref;
    struct urb *urb;
    u8[8] *buffer;
    union (anon) *status;
    struct mutex status_mutex;
    int error;
    int nerrors;
    long unsigned int event_bits[1];
    long unsigned int change_bits[1];
    long unsigned int removed_bits[1];
    long unsigned int wakeup_bits[1];
    long unsigned int power_bits[1];
    long unsigned int child_usage_bits[1];
    long unsigned int warm_reset_bits[1];
    struct usb_hub_descriptor *descriptor;
    struct usb_tt tt;
    unsigned int mA_per_port;
    unsigned int wakeup_enabled_descendants;
    unsigned int limited_power;
    unsigned int quiescing;
    unsigned int disconnected;
    unsigned int in_reset;
    unsigned int quirk_disable_autosuspend;
    unsigned int quirk_check_port_auto_suspend;
    unsigned int has_indicators;
    u8 indicator[31];
    struct delayed_work leds;
    struct delayed_work init_work;
    struct work_struct events;
    spinlock_t irq_urb_lock;
    struct timer_list irq_urb_retry;
    struct usb_port **ports;
    struct list_head onboard_hub_devs;
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
struct usb_hub {
    struct device *intfdev;
    struct usb_device *hdev;
    struct kref kref;
    struct urb *urb;
    u8[8] *buffer;
    union (anon) *status;
    struct mutex status_mutex;
    int error;
    int nerrors;
    long unsigned int event_bits[1];
    long unsigned int change_bits[1];
    long unsigned int removed_bits[1];
    long unsigned int wakeup_bits[1];
    long unsigned int power_bits[1];
    long unsigned int child_usage_bits[1];
    long unsigned int warm_reset_bits[1];
    struct usb_hub_descriptor *descriptor;
    struct usb_tt tt;
    unsigned int mA_per_port;
    unsigned int wakeup_enabled_descendants;
    unsigned int limited_power;
    unsigned int quiescing;
    unsigned int disconnected;
    unsigned int in_reset;
    unsigned int quirk_disable_autosuspend;
    unsigned int quirk_check_port_auto_suspend;
    unsigned int has_indicators;
    u8 indicator[31];
    struct delayed_work leds;
    struct delayed_work init_work;
    struct work_struct events;
    spinlock_t irq_urb_lock;
    struct timer_list irq_urb_retry;
    struct usb_port **ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct usb_hub {
    struct device *intfdev;
    struct usb_device *hdev;
    struct kref kref;
    struct urb *urb;
    u8[8] *buffer;
    union (anon) *status;
    struct mutex status_mutex;
    int error;
    int nerrors;
    long unsigned int event_bits[1];
    long unsigned int change_bits[1];
    long unsigned int removed_bits[1];
    long unsigned int wakeup_bits[1];
    long unsigned int power_bits[1];
    long unsigned int child_usage_bits[1];
    long unsigned int warm_reset_bits[1];
    struct usb_hub_descriptor *descriptor;
    struct usb_tt tt;
    unsigned int mA_per_port;
    unsigned int wakeup_enabled_descendants;
    unsigned int limited_power;
    unsigned int quiescing;
    unsigned int disconnected;
    unsigned int in_reset;
    unsigned int quirk_disable_autosuspend;
    unsigned int quirk_check_port_auto_suspend;
    unsigned int has_indicators;
    u8 indicator[31];
    struct delayed_work leds;
    struct delayed_work init_work;
    struct work_struct events;
    spinlock_t irq_urb_lock;
    struct timer_list irq_urb_retry;
    struct usb_port **ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct usb_hub {
    struct device *intfdev;
    struct usb_device *hdev;
    struct kref kref;
    struct urb *urb;
    u8[8] *buffer;
    union (anon) *status;
    struct mutex status_mutex;
    int error;
    int nerrors;
    long unsigned int event_bits[1];
    long unsigned int change_bits[1];
    long unsigned int removed_bits[1];
    long unsigned int wakeup_bits[1];
    long unsigned int power_bits[1];
    long unsigned int child_usage_bits[1];
    long unsigned int warm_reset_bits[1];
    struct usb_hub_descriptor *descriptor;
    struct usb_tt tt;
    unsigned int mA_per_port;
    unsigned int wakeup_enabled_descendants;
    unsigned int limited_power;
    unsigned int quiescing;
    unsigned int disconnected;
    unsigned int in_reset;
    unsigned int quirk_disable_autosuspend;
    unsigned int quirk_check_port_auto_suspend;
    unsigned int has_indicators;
    u8 indicator[31];
    struct delayed_work leds;
    struct delayed_work init_work;
    struct work_struct events;
    spinlock_t irq_urb_lock;
    struct timer_list irq_urb_retry;
    struct usb_port **ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct usb_hub {
    struct device *intfdev;
    struct usb_device *hdev;
    struct kref kref;
    struct urb *urb;
    u8[8] *buffer;
    union (anon) *status;
    struct mutex status_mutex;
    int error;
    int nerrors;
    long unsigned int event_bits[1];
    long unsigned int change_bits[1];
    long unsigned int removed_bits[1];
    long unsigned int wakeup_bits[1];
    long unsigned int power_bits[1];
    long unsigned int child_usage_bits[1];
    long unsigned int warm_reset_bits[1];
    struct usb_hub_descriptor *descriptor;
    struct usb_tt tt;
    unsigned int mA_per_port;
    unsigned int wakeup_enabled_descendants;
    unsigned int limited_power;
    unsigned int quiescing;
    unsigned int disconnected;
    unsigned int in_reset;
    unsigned int quirk_disable_autosuspend;
    unsigned int quirk_check_port_auto_suspend;
    unsigned int has_indicators;
    u8 indicator[31];
    struct delayed_work leds;
    struct delayed_work init_work;
    struct work_struct events;
    spinlock_t irq_urb_lock;
    struct timer_list irq_urb_retry;
    struct usb_port **ports;
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
struct usb_hub {
    struct device *intfdev;
    struct usb_device *hdev;
    struct kref kref;
    struct urb *urb;
    u8[8] *buffer;
    union (anon) *status;
    struct mutex status_mutex;
    int error;
    int nerrors;
    long unsigned int event_bits[1];
    long unsigned int change_bits[1];
    long unsigned int removed_bits[1];
    long unsigned int wakeup_bits[1];
    long unsigned int power_bits[1];
    long unsigned int child_usage_bits[1];
    long unsigned int warm_reset_bits[1];
    struct usb_hub_descriptor *descriptor;
    struct usb_tt tt;
    unsigned int mA_per_port;
    unsigned int wakeup_enabled_descendants;
    unsigned int limited_power;
    unsigned int quiescing;
    unsigned int disconnected;
    unsigned int in_reset;
    unsigned int quirk_disable_autosuspend;
    unsigned int quirk_check_port_auto_suspend;
    unsigned int has_indicators;
    u8 indicator[31];
    struct delayed_work leds;
    struct delayed_work init_work;
    struct work_struct events;
    spinlock_t irq_urb_lock;
    struct timer_list irq_urb_retry;
    struct usb_port **ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct usb_hub {
    struct device *intfdev;
    struct usb_device *hdev;
    struct kref kref;
    struct urb *urb;
    u8[8] *buffer;
    union (anon) *status;
    struct mutex status_mutex;
    int error;
    int nerrors;
    long unsigned int event_bits[1];
    long unsigned int change_bits[1];
    long unsigned int removed_bits[1];
    long unsigned int wakeup_bits[1];
    long unsigned int power_bits[1];
    long unsigned int child_usage_bits[1];
    long unsigned int warm_reset_bits[1];
    struct usb_hub_descriptor *descriptor;
    struct usb_tt tt;
    unsigned int mA_per_port;
    unsigned int wakeup_enabled_descendants;
    unsigned int limited_power;
    unsigned int quiescing;
    unsigned int disconnected;
    unsigned int in_reset;
    unsigned int quirk_disable_autosuspend;
    unsigned int quirk_check_port_auto_suspend;
    unsigned int has_indicators;
    u8 indicator[31];
    struct delayed_work leds;
    struct delayed_work init_work;
    struct work_struct events;
    spinlock_t irq_urb_lock;
    struct timer_list irq_urb_retry;
    struct usb_port **ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct usb_hub {
    struct device *intfdev;
    struct usb_device *hdev;
    struct kref kref;
    struct urb *urb;
    u8[8] *buffer;
    union (anon) *status;
    struct mutex status_mutex;
    int error;
    int nerrors;
    long unsigned int event_bits[1];
    long unsigned int change_bits[1];
    long unsigned int removed_bits[1];
    long unsigned int wakeup_bits[1];
    long unsigned int power_bits[1];
    long unsigned int child_usage_bits[1];
    long unsigned int warm_reset_bits[1];
    struct usb_hub_descriptor *descriptor;
    struct usb_tt tt;
    unsigned int mA_per_port;
    unsigned int wakeup_enabled_descendants;
    unsigned int limited_power;
    unsigned int quiescing;
    unsigned int disconnected;
    unsigned int in_reset;
    unsigned int quirk_disable_autosuspend;
    unsigned int quirk_check_port_auto_suspend;
    unsigned int has_indicators;
    u8 indicator[31];
    struct delayed_work leds;
    struct delayed_work init_work;
    struct work_struct events;
    spinlock_t irq_urb_lock;
    struct timer_list irq_urb_retry;
    struct usb_port **ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct usb_hub {
    struct device *intfdev;
    struct usb_device *hdev;
    struct kref kref;
    struct urb *urb;
    u8[8] *buffer;
    union (anon) *status;
    struct mutex status_mutex;
    int error;
    int nerrors;
    long unsigned int event_bits[1];
    long unsigned int change_bits[1];
    long unsigned int removed_bits[1];
    long unsigned int wakeup_bits[1];
    long unsigned int power_bits[1];
    long unsigned int child_usage_bits[1];
    long unsigned int warm_reset_bits[1];
    struct usb_hub_descriptor *descriptor;
    struct usb_tt tt;
    unsigned int mA_per_port;
    unsigned int wakeup_enabled_descendants;
    unsigned int limited_power;
    unsigned int quiescing;
    unsigned int disconnected;
    unsigned int in_reset;
    unsigned int quirk_disable_autosuspend;
    unsigned int quirk_check_port_auto_suspend;
    unsigned int has_indicators;
    u8 indicator[31];
    struct delayed_work leds;
    struct delayed_work init_work;
    struct work_struct events;
    spinlock_t irq_urb_lock;
    struct timer_list irq_urb_retry;
    struct usb_port **ports;
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
No changes between <code>4.15</code> and <code>4.18</code> ✅
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
<code>spinlock_t irq_urb_lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct timer_list irq_urb_retry</code>
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
<code>unsigned int quirk_disable_autosuspend</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head onboard_hub_devs</code>
</li>
</ul>
</details>
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
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
