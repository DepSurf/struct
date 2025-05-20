# Struct: <code>usb_gadget_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct usb_gadget_ops {
    int (*get_frame)(struct usb_gadget *);
    int (*wakeup)(struct usb_gadget *);
    int (*set_selfpowered)(struct usb_gadget *, int);
    int (*vbus_session)(struct usb_gadget *, int);
    int (*vbus_draw)(struct usb_gadget *, unsigned int);
    int (*pullup)(struct usb_gadget *, int);
    int (*ioctl)(struct usb_gadget *, unsigned int, long unsigned int);
    void (*get_config_params)(struct usb_dcd_config_params *);
    int (*udc_start)(struct usb_gadget *, struct usb_gadget_driver *);
    int (*udc_stop)(struct usb_gadget *);
    struct usb_ep * (*match_ep)(struct usb_gadget *, struct usb_endpoint_descriptor *, struct usb_ss_ep_comp_descriptor *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct usb_gadget_ops {
    int (*get_frame)(struct usb_gadget *);
    int (*wakeup)(struct usb_gadget *);
    int (*set_selfpowered)(struct usb_gadget *, int);
    int (*vbus_session)(struct usb_gadget *, int);
    int (*vbus_draw)(struct usb_gadget *, unsigned int);
    int (*pullup)(struct usb_gadget *, int);
    int (*ioctl)(struct usb_gadget *, unsigned int, long unsigned int);
    void (*get_config_params)(struct usb_dcd_config_params *);
    int (*udc_start)(struct usb_gadget *, struct usb_gadget_driver *);
    int (*udc_stop)(struct usb_gadget *);
    struct usb_ep * (*match_ep)(struct usb_gadget *, struct usb_endpoint_descriptor *, struct usb_ss_ep_comp_descriptor *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct usb_gadget_ops {
    int (*get_frame)(struct usb_gadget *);
    int (*wakeup)(struct usb_gadget *);
    int (*set_selfpowered)(struct usb_gadget *, int);
    int (*vbus_session)(struct usb_gadget *, int);
    int (*vbus_draw)(struct usb_gadget *, unsigned int);
    int (*pullup)(struct usb_gadget *, int);
    int (*ioctl)(struct usb_gadget *, unsigned int, long unsigned int);
    void (*get_config_params)(struct usb_dcd_config_params *);
    int (*udc_start)(struct usb_gadget *, struct usb_gadget_driver *);
    int (*udc_stop)(struct usb_gadget *);
    struct usb_ep * (*match_ep)(struct usb_gadget *, struct usb_endpoint_descriptor *, struct usb_ss_ep_comp_descriptor *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct usb_gadget_ops {
    int (*get_frame)(struct usb_gadget *);
    int (*wakeup)(struct usb_gadget *);
    int (*set_selfpowered)(struct usb_gadget *, int);
    int (*vbus_session)(struct usb_gadget *, int);
    int (*vbus_draw)(struct usb_gadget *, unsigned int);
    int (*pullup)(struct usb_gadget *, int);
    int (*ioctl)(struct usb_gadget *, unsigned int, long unsigned int);
    void (*get_config_params)(struct usb_dcd_config_params *);
    int (*udc_start)(struct usb_gadget *, struct usb_gadget_driver *);
    int (*udc_stop)(struct usb_gadget *);
    void (*udc_set_speed)(struct usb_gadget *, enum usb_device_speed);
    struct usb_ep * (*match_ep)(struct usb_gadget *, struct usb_endpoint_descriptor *, struct usb_ss_ep_comp_descriptor *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct usb_gadget_ops {
    int (*get_frame)(struct usb_gadget *);
    int (*wakeup)(struct usb_gadget *);
    int (*set_selfpowered)(struct usb_gadget *, int);
    int (*vbus_session)(struct usb_gadget *, int);
    int (*vbus_draw)(struct usb_gadget *, unsigned int);
    int (*pullup)(struct usb_gadget *, int);
    int (*ioctl)(struct usb_gadget *, unsigned int, long unsigned int);
    void (*get_config_params)(struct usb_dcd_config_params *);
    int (*udc_start)(struct usb_gadget *, struct usb_gadget_driver *);
    int (*udc_stop)(struct usb_gadget *);
    void (*udc_set_speed)(struct usb_gadget *, enum usb_device_speed);
    struct usb_ep * (*match_ep)(struct usb_gadget *, struct usb_endpoint_descriptor *, struct usb_ss_ep_comp_descriptor *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct usb_gadget_ops {
    int (*get_frame)(struct usb_gadget *);
    int (*wakeup)(struct usb_gadget *);
    int (*set_selfpowered)(struct usb_gadget *, int);
    int (*vbus_session)(struct usb_gadget *, int);
    int (*vbus_draw)(struct usb_gadget *, unsigned int);
    int (*pullup)(struct usb_gadget *, int);
    int (*ioctl)(struct usb_gadget *, unsigned int, long unsigned int);
    void (*get_config_params)(struct usb_dcd_config_params *);
    int (*udc_start)(struct usb_gadget *, struct usb_gadget_driver *);
    int (*udc_stop)(struct usb_gadget *);
    void (*udc_set_speed)(struct usb_gadget *, enum usb_device_speed);
    struct usb_ep * (*match_ep)(struct usb_gadget *, struct usb_endpoint_descriptor *, struct usb_ss_ep_comp_descriptor *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct usb_gadget_ops {
    int (*get_frame)(struct usb_gadget *);
    int (*wakeup)(struct usb_gadget *);
    int (*set_selfpowered)(struct usb_gadget *, int);
    int (*vbus_session)(struct usb_gadget *, int);
    int (*vbus_draw)(struct usb_gadget *, unsigned int);
    int (*pullup)(struct usb_gadget *, int);
    int (*ioctl)(struct usb_gadget *, unsigned int, long unsigned int);
    void (*get_config_params)(struct usb_dcd_config_params *);
    int (*udc_start)(struct usb_gadget *, struct usb_gadget_driver *);
    int (*udc_stop)(struct usb_gadget *);
    void (*udc_set_speed)(struct usb_gadget *, enum usb_device_speed);
    struct usb_ep * (*match_ep)(struct usb_gadget *, struct usb_endpoint_descriptor *, struct usb_ss_ep_comp_descriptor *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct usb_gadget_ops {
    int (*get_frame)(struct usb_gadget *);
    int (*wakeup)(struct usb_gadget *);
    int (*set_selfpowered)(struct usb_gadget *, int);
    int (*vbus_session)(struct usb_gadget *, int);
    int (*vbus_draw)(struct usb_gadget *, unsigned int);
    int (*pullup)(struct usb_gadget *, int);
    int (*ioctl)(struct usb_gadget *, unsigned int, long unsigned int);
    void (*get_config_params)(struct usb_gadget *, struct usb_dcd_config_params *);
    int (*udc_start)(struct usb_gadget *, struct usb_gadget_driver *);
    int (*udc_stop)(struct usb_gadget *);
    void (*udc_set_speed)(struct usb_gadget *, enum usb_device_speed);
    struct usb_ep * (*match_ep)(struct usb_gadget *, struct usb_endpoint_descriptor *, struct usb_ss_ep_comp_descriptor *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct usb_gadget_ops {
    int (*get_frame)(struct usb_gadget *);
    int (*wakeup)(struct usb_gadget *);
    int (*set_selfpowered)(struct usb_gadget *, int);
    int (*vbus_session)(struct usb_gadget *, int);
    int (*vbus_draw)(struct usb_gadget *, unsigned int);
    int (*pullup)(struct usb_gadget *, int);
    int (*ioctl)(struct usb_gadget *, unsigned int, long unsigned int);
    void (*get_config_params)(struct usb_gadget *, struct usb_dcd_config_params *);
    int (*udc_start)(struct usb_gadget *, struct usb_gadget_driver *);
    int (*udc_stop)(struct usb_gadget *);
    void (*udc_set_speed)(struct usb_gadget *, enum usb_device_speed);
    struct usb_ep * (*match_ep)(struct usb_gadget *, struct usb_endpoint_descriptor *, struct usb_ss_ep_comp_descriptor *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct usb_gadget_ops {
    int (*get_frame)(struct usb_gadget *);
    int (*wakeup)(struct usb_gadget *);
    int (*set_selfpowered)(struct usb_gadget *, int);
    int (*vbus_session)(struct usb_gadget *, int);
    int (*vbus_draw)(struct usb_gadget *, unsigned int);
    int (*pullup)(struct usb_gadget *, int);
    int (*ioctl)(struct usb_gadget *, unsigned int, long unsigned int);
    void (*get_config_params)(struct usb_gadget *, struct usb_dcd_config_params *);
    int (*udc_start)(struct usb_gadget *, struct usb_gadget_driver *);
    int (*udc_stop)(struct usb_gadget *);
    void (*udc_set_speed)(struct usb_gadget *, enum usb_device_speed);
    struct usb_ep * (*match_ep)(struct usb_gadget *, struct usb_endpoint_descriptor *, struct usb_ss_ep_comp_descriptor *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct usb_gadget_ops {
    int (*get_frame)(struct usb_gadget *);
    int (*wakeup)(struct usb_gadget *);
    int (*set_selfpowered)(struct usb_gadget *, int);
    int (*vbus_session)(struct usb_gadget *, int);
    int (*vbus_draw)(struct usb_gadget *, unsigned int);
    int (*pullup)(struct usb_gadget *, int);
    int (*ioctl)(struct usb_gadget *, unsigned int, long unsigned int);
    void (*get_config_params)(struct usb_gadget *, struct usb_dcd_config_params *);
    int (*udc_start)(struct usb_gadget *, struct usb_gadget_driver *);
    int (*udc_stop)(struct usb_gadget *);
    void (*udc_set_speed)(struct usb_gadget *, enum usb_device_speed);
    struct usb_ep * (*match_ep)(struct usb_gadget *, struct usb_endpoint_descriptor *, struct usb_ss_ep_comp_descriptor *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct usb_gadget_ops {
    int (*get_frame)(struct usb_gadget *);
    int (*wakeup)(struct usb_gadget *);
    int (*set_selfpowered)(struct usb_gadget *, int);
    int (*vbus_session)(struct usb_gadget *, int);
    int (*vbus_draw)(struct usb_gadget *, unsigned int);
    int (*pullup)(struct usb_gadget *, int);
    int (*ioctl)(struct usb_gadget *, unsigned int, long unsigned int);
    void (*get_config_params)(struct usb_gadget *, struct usb_dcd_config_params *);
    int (*udc_start)(struct usb_gadget *, struct usb_gadget_driver *);
    int (*udc_stop)(struct usb_gadget *);
    void (*udc_set_speed)(struct usb_gadget *, enum usb_device_speed);
    void (*udc_set_ssp_rate)(struct usb_gadget *, enum usb_ssp_rate);
    struct usb_ep * (*match_ep)(struct usb_gadget *, struct usb_endpoint_descriptor *, struct usb_ss_ep_comp_descriptor *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct usb_gadget_ops {
    int (*get_frame)(struct usb_gadget *);
    int (*wakeup)(struct usb_gadget *);
    int (*set_selfpowered)(struct usb_gadget *, int);
    int (*vbus_session)(struct usb_gadget *, int);
    int (*vbus_draw)(struct usb_gadget *, unsigned int);
    int (*pullup)(struct usb_gadget *, int);
    int (*ioctl)(struct usb_gadget *, unsigned int, long unsigned int);
    void (*get_config_params)(struct usb_gadget *, struct usb_dcd_config_params *);
    int (*udc_start)(struct usb_gadget *, struct usb_gadget_driver *);
    int (*udc_stop)(struct usb_gadget *);
    void (*udc_set_speed)(struct usb_gadget *, enum usb_device_speed);
    void (*udc_set_ssp_rate)(struct usb_gadget *, enum usb_ssp_rate);
    void (*udc_async_callbacks)(struct usb_gadget *, bool);
    struct usb_ep * (*match_ep)(struct usb_gadget *, struct usb_endpoint_descriptor *, struct usb_ss_ep_comp_descriptor *);
    int (*check_config)(struct usb_gadget *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct usb_gadget_ops {
    int (*get_frame)(struct usb_gadget *);
    int (*wakeup)(struct usb_gadget *);
    int (*set_selfpowered)(struct usb_gadget *, int);
    int (*vbus_session)(struct usb_gadget *, int);
    int (*vbus_draw)(struct usb_gadget *, unsigned int);
    int (*pullup)(struct usb_gadget *, int);
    int (*ioctl)(struct usb_gadget *, unsigned int, long unsigned int);
    void (*get_config_params)(struct usb_gadget *, struct usb_dcd_config_params *);
    int (*udc_start)(struct usb_gadget *, struct usb_gadget_driver *);
    int (*udc_stop)(struct usb_gadget *);
    void (*udc_set_speed)(struct usb_gadget *, enum usb_device_speed);
    void (*udc_set_ssp_rate)(struct usb_gadget *, enum usb_ssp_rate);
    void (*udc_async_callbacks)(struct usb_gadget *, bool);
    struct usb_ep * (*match_ep)(struct usb_gadget *, struct usb_endpoint_descriptor *, struct usb_ss_ep_comp_descriptor *);
    int (*check_config)(struct usb_gadget *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct usb_gadget_ops {
    int (*get_frame)(struct usb_gadget *);
    int (*wakeup)(struct usb_gadget *);
    int (*set_selfpowered)(struct usb_gadget *, int);
    int (*vbus_session)(struct usb_gadget *, int);
    int (*vbus_draw)(struct usb_gadget *, unsigned int);
    int (*pullup)(struct usb_gadget *, int);
    int (*ioctl)(struct usb_gadget *, unsigned int, long unsigned int);
    void (*get_config_params)(struct usb_gadget *, struct usb_dcd_config_params *);
    int (*udc_start)(struct usb_gadget *, struct usb_gadget_driver *);
    int (*udc_stop)(struct usb_gadget *);
    void (*udc_set_speed)(struct usb_gadget *, enum usb_device_speed);
    void (*udc_set_ssp_rate)(struct usb_gadget *, enum usb_ssp_rate);
    void (*udc_async_callbacks)(struct usb_gadget *, bool);
    struct usb_ep * (*match_ep)(struct usb_gadget *, struct usb_endpoint_descriptor *, struct usb_ss_ep_comp_descriptor *);
    int (*check_config)(struct usb_gadget *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct usb_gadget_ops {
    int (*get_frame)(struct usb_gadget *);
    int (*wakeup)(struct usb_gadget *);
    int (*func_wakeup)(struct usb_gadget *, int);
    int (*set_remote_wakeup)(struct usb_gadget *, int);
    int (*set_selfpowered)(struct usb_gadget *, int);
    int (*vbus_session)(struct usb_gadget *, int);
    int (*vbus_draw)(struct usb_gadget *, unsigned int);
    int (*pullup)(struct usb_gadget *, int);
    int (*ioctl)(struct usb_gadget *, unsigned int, long unsigned int);
    void (*get_config_params)(struct usb_gadget *, struct usb_dcd_config_params *);
    int (*udc_start)(struct usb_gadget *, struct usb_gadget_driver *);
    int (*udc_stop)(struct usb_gadget *);
    void (*udc_set_speed)(struct usb_gadget *, enum usb_device_speed);
    void (*udc_set_ssp_rate)(struct usb_gadget *, enum usb_ssp_rate);
    void (*udc_async_callbacks)(struct usb_gadget *, bool);
    struct usb_ep * (*match_ep)(struct usb_gadget *, struct usb_endpoint_descriptor *, struct usb_ss_ep_comp_descriptor *);
    int (*check_config)(struct usb_gadget *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct usb_gadget_ops {
    int (*get_frame)(struct usb_gadget *);
    int (*wakeup)(struct usb_gadget *);
    int (*func_wakeup)(struct usb_gadget *, int);
    int (*set_remote_wakeup)(struct usb_gadget *, int);
    int (*set_selfpowered)(struct usb_gadget *, int);
    int (*vbus_session)(struct usb_gadget *, int);
    int (*vbus_draw)(struct usb_gadget *, unsigned int);
    int (*pullup)(struct usb_gadget *, int);
    int (*ioctl)(struct usb_gadget *, unsigned int, long unsigned int);
    void (*get_config_params)(struct usb_gadget *, struct usb_dcd_config_params *);
    int (*udc_start)(struct usb_gadget *, struct usb_gadget_driver *);
    int (*udc_stop)(struct usb_gadget *);
    void (*udc_set_speed)(struct usb_gadget *, enum usb_device_speed);
    void (*udc_set_ssp_rate)(struct usb_gadget *, enum usb_ssp_rate);
    void (*udc_async_callbacks)(struct usb_gadget *, bool);
    struct usb_ep * (*match_ep)(struct usb_gadget *, struct usb_endpoint_descriptor *, struct usb_ss_ep_comp_descriptor *);
    int (*check_config)(struct usb_gadget *);
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
struct usb_gadget_ops {
    int (*get_frame)(struct usb_gadget *);
    int (*wakeup)(struct usb_gadget *);
    int (*set_selfpowered)(struct usb_gadget *, int);
    int (*vbus_session)(struct usb_gadget *, int);
    int (*vbus_draw)(struct usb_gadget *, unsigned int);
    int (*pullup)(struct usb_gadget *, int);
    int (*ioctl)(struct usb_gadget *, unsigned int, long unsigned int);
    void (*get_config_params)(struct usb_gadget *, struct usb_dcd_config_params *);
    int (*udc_start)(struct usb_gadget *, struct usb_gadget_driver *);
    int (*udc_stop)(struct usb_gadget *);
    void (*udc_set_speed)(struct usb_gadget *, enum usb_device_speed);
    struct usb_ep * (*match_ep)(struct usb_gadget *, struct usb_endpoint_descriptor *, struct usb_ss_ep_comp_descriptor *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct usb_gadget_ops {
    int (*get_frame)(struct usb_gadget *);
    int (*wakeup)(struct usb_gadget *);
    int (*set_selfpowered)(struct usb_gadget *, int);
    int (*vbus_session)(struct usb_gadget *, int);
    int (*vbus_draw)(struct usb_gadget *, unsigned int);
    int (*pullup)(struct usb_gadget *, int);
    int (*ioctl)(struct usb_gadget *, unsigned int, long unsigned int);
    void (*get_config_params)(struct usb_gadget *, struct usb_dcd_config_params *);
    int (*udc_start)(struct usb_gadget *, struct usb_gadget_driver *);
    int (*udc_stop)(struct usb_gadget *);
    void (*udc_set_speed)(struct usb_gadget *, enum usb_device_speed);
    struct usb_ep * (*match_ep)(struct usb_gadget *, struct usb_endpoint_descriptor *, struct usb_ss_ep_comp_descriptor *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct usb_gadget_ops {
    int (*get_frame)(struct usb_gadget *);
    int (*wakeup)(struct usb_gadget *);
    int (*set_selfpowered)(struct usb_gadget *, int);
    int (*vbus_session)(struct usb_gadget *, int);
    int (*vbus_draw)(struct usb_gadget *, unsigned int);
    int (*pullup)(struct usb_gadget *, int);
    int (*ioctl)(struct usb_gadget *, unsigned int, long unsigned int);
    void (*get_config_params)(struct usb_gadget *, struct usb_dcd_config_params *);
    int (*udc_start)(struct usb_gadget *, struct usb_gadget_driver *);
    int (*udc_stop)(struct usb_gadget *);
    void (*udc_set_speed)(struct usb_gadget *, enum usb_device_speed);
    struct usb_ep * (*match_ep)(struct usb_gadget *, struct usb_endpoint_descriptor *, struct usb_ss_ep_comp_descriptor *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct usb_gadget_ops {
    int (*get_frame)(struct usb_gadget *);
    int (*wakeup)(struct usb_gadget *);
    int (*set_selfpowered)(struct usb_gadget *, int);
    int (*vbus_session)(struct usb_gadget *, int);
    int (*vbus_draw)(struct usb_gadget *, unsigned int);
    int (*pullup)(struct usb_gadget *, int);
    int (*ioctl)(struct usb_gadget *, unsigned int, long unsigned int);
    void (*get_config_params)(struct usb_gadget *, struct usb_dcd_config_params *);
    int (*udc_start)(struct usb_gadget *, struct usb_gadget_driver *);
    int (*udc_stop)(struct usb_gadget *);
    void (*udc_set_speed)(struct usb_gadget *, enum usb_device_speed);
    struct usb_ep * (*match_ep)(struct usb_gadget *, struct usb_endpoint_descriptor *, struct usb_ss_ep_comp_descriptor *);
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
struct usb_gadget_ops {
    int (*get_frame)(struct usb_gadget *);
    int (*wakeup)(struct usb_gadget *);
    int (*set_selfpowered)(struct usb_gadget *, int);
    int (*vbus_session)(struct usb_gadget *, int);
    int (*vbus_draw)(struct usb_gadget *, unsigned int);
    int (*pullup)(struct usb_gadget *, int);
    int (*ioctl)(struct usb_gadget *, unsigned int, long unsigned int);
    void (*get_config_params)(struct usb_gadget *, struct usb_dcd_config_params *);
    int (*udc_start)(struct usb_gadget *, struct usb_gadget_driver *);
    int (*udc_stop)(struct usb_gadget *);
    void (*udc_set_speed)(struct usb_gadget *, enum usb_device_speed);
    struct usb_ep * (*match_ep)(struct usb_gadget *, struct usb_endpoint_descriptor *, struct usb_ss_ep_comp_descriptor *);
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
struct usb_gadget_ops {
    int (*get_frame)(struct usb_gadget *);
    int (*wakeup)(struct usb_gadget *);
    int (*set_selfpowered)(struct usb_gadget *, int);
    int (*vbus_session)(struct usb_gadget *, int);
    int (*vbus_draw)(struct usb_gadget *, unsigned int);
    int (*pullup)(struct usb_gadget *, int);
    int (*ioctl)(struct usb_gadget *, unsigned int, long unsigned int);
    void (*get_config_params)(struct usb_gadget *, struct usb_dcd_config_params *);
    int (*udc_start)(struct usb_gadget *, struct usb_gadget_driver *);
    int (*udc_stop)(struct usb_gadget *);
    void (*udc_set_speed)(struct usb_gadget *, enum usb_device_speed);
    struct usb_ep * (*match_ep)(struct usb_gadget *, struct usb_endpoint_descriptor *, struct usb_ss_ep_comp_descriptor *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct usb_gadget_ops {
    int (*get_frame)(struct usb_gadget *);
    int (*wakeup)(struct usb_gadget *);
    int (*set_selfpowered)(struct usb_gadget *, int);
    int (*vbus_session)(struct usb_gadget *, int);
    int (*vbus_draw)(struct usb_gadget *, unsigned int);
    int (*pullup)(struct usb_gadget *, int);
    int (*ioctl)(struct usb_gadget *, unsigned int, long unsigned int);
    void (*get_config_params)(struct usb_gadget *, struct usb_dcd_config_params *);
    int (*udc_start)(struct usb_gadget *, struct usb_gadget_driver *);
    int (*udc_stop)(struct usb_gadget *);
    void (*udc_set_speed)(struct usb_gadget *, enum usb_device_speed);
    struct usb_ep * (*match_ep)(struct usb_gadget *, struct usb_endpoint_descriptor *, struct usb_ss_ep_comp_descriptor *);
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
<code>void (*udc_set_speed)(struct usb_gadget *, enum usb_device_speed)</code>
</li>
</ul>
</details>
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
<b>Field type changed. </b>
<code>void (*get_config_params)(struct usb_dcd_config_params *)</code> ➡️ <code>void (*get_config_params)(struct usb_gadget *, struct usb_dcd_config_params *)</code>
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
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*udc_set_ssp_rate)(struct usb_gadget *, enum usb_ssp_rate)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*udc_async_callbacks)(struct usb_gadget *, bool)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*check_config)(struct usb_gadget *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*func_wakeup)(struct usb_gadget *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_remote_wakeup)(struct usb_gadget *, int)</code>
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
