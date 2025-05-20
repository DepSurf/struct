# Struct: <code>usb_driver</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct usb_driver {
    const char *name;
    int (*probe)(struct usb_interface *, const struct usb_device_id *);
    void (*disconnect)(struct usb_interface *);
    int (*unlocked_ioctl)(struct usb_interface *, unsigned int, void *);
    int (*suspend)(struct usb_interface *, pm_message_t);
    int (*resume)(struct usb_interface *);
    int (*reset_resume)(struct usb_interface *);
    int (*pre_reset)(struct usb_interface *);
    int (*post_reset)(struct usb_interface *);
    const struct usb_device_id *id_table;
    struct usb_dynids dynids;
    struct usbdrv_wrap drvwrap;
    unsigned int no_dynamic_id;
    unsigned int supports_autosuspend;
    unsigned int disable_hub_initiated_lpm;
    unsigned int soft_unbind;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct usb_driver {
    const char *name;
    int (*probe)(struct usb_interface *, const struct usb_device_id *);
    void (*disconnect)(struct usb_interface *);
    int (*unlocked_ioctl)(struct usb_interface *, unsigned int, void *);
    int (*suspend)(struct usb_interface *, pm_message_t);
    int (*resume)(struct usb_interface *);
    int (*reset_resume)(struct usb_interface *);
    int (*pre_reset)(struct usb_interface *);
    int (*post_reset)(struct usb_interface *);
    const struct usb_device_id *id_table;
    struct usb_dynids dynids;
    struct usbdrv_wrap drvwrap;
    unsigned int no_dynamic_id;
    unsigned int supports_autosuspend;
    unsigned int disable_hub_initiated_lpm;
    unsigned int soft_unbind;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct usb_driver {
    const char *name;
    int (*probe)(struct usb_interface *, const struct usb_device_id *);
    void (*disconnect)(struct usb_interface *);
    int (*unlocked_ioctl)(struct usb_interface *, unsigned int, void *);
    int (*suspend)(struct usb_interface *, pm_message_t);
    int (*resume)(struct usb_interface *);
    int (*reset_resume)(struct usb_interface *);
    int (*pre_reset)(struct usb_interface *);
    int (*post_reset)(struct usb_interface *);
    const struct usb_device_id *id_table;
    struct usb_dynids dynids;
    struct usbdrv_wrap drvwrap;
    unsigned int no_dynamic_id;
    unsigned int supports_autosuspend;
    unsigned int disable_hub_initiated_lpm;
    unsigned int soft_unbind;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct usb_driver {
    const char *name;
    int (*probe)(struct usb_interface *, const struct usb_device_id *);
    void (*disconnect)(struct usb_interface *);
    int (*unlocked_ioctl)(struct usb_interface *, unsigned int, void *);
    int (*suspend)(struct usb_interface *, pm_message_t);
    int (*resume)(struct usb_interface *);
    int (*reset_resume)(struct usb_interface *);
    int (*pre_reset)(struct usb_interface *);
    int (*post_reset)(struct usb_interface *);
    const struct usb_device_id *id_table;
    struct usb_dynids dynids;
    struct usbdrv_wrap drvwrap;
    unsigned int no_dynamic_id;
    unsigned int supports_autosuspend;
    unsigned int disable_hub_initiated_lpm;
    unsigned int soft_unbind;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct usb_driver {
    const char *name;
    int (*probe)(struct usb_interface *, const struct usb_device_id *);
    void (*disconnect)(struct usb_interface *);
    int (*unlocked_ioctl)(struct usb_interface *, unsigned int, void *);
    int (*suspend)(struct usb_interface *, pm_message_t);
    int (*resume)(struct usb_interface *);
    int (*reset_resume)(struct usb_interface *);
    int (*pre_reset)(struct usb_interface *);
    int (*post_reset)(struct usb_interface *);
    const struct usb_device_id *id_table;
    struct usb_dynids dynids;
    struct usbdrv_wrap drvwrap;
    unsigned int no_dynamic_id;
    unsigned int supports_autosuspend;
    unsigned int disable_hub_initiated_lpm;
    unsigned int soft_unbind;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct usb_driver {
    const char *name;
    int (*probe)(struct usb_interface *, const struct usb_device_id *);
    void (*disconnect)(struct usb_interface *);
    int (*unlocked_ioctl)(struct usb_interface *, unsigned int, void *);
    int (*suspend)(struct usb_interface *, pm_message_t);
    int (*resume)(struct usb_interface *);
    int (*reset_resume)(struct usb_interface *);
    int (*pre_reset)(struct usb_interface *);
    int (*post_reset)(struct usb_interface *);
    const struct usb_device_id *id_table;
    struct usb_dynids dynids;
    struct usbdrv_wrap drvwrap;
    unsigned int no_dynamic_id;
    unsigned int supports_autosuspend;
    unsigned int disable_hub_initiated_lpm;
    unsigned int soft_unbind;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct usb_driver {
    const char *name;
    int (*probe)(struct usb_interface *, const struct usb_device_id *);
    void (*disconnect)(struct usb_interface *);
    int (*unlocked_ioctl)(struct usb_interface *, unsigned int, void *);
    int (*suspend)(struct usb_interface *, pm_message_t);
    int (*resume)(struct usb_interface *);
    int (*reset_resume)(struct usb_interface *);
    int (*pre_reset)(struct usb_interface *);
    int (*post_reset)(struct usb_interface *);
    const struct usb_device_id *id_table;
    struct usb_dynids dynids;
    struct usbdrv_wrap drvwrap;
    unsigned int no_dynamic_id;
    unsigned int supports_autosuspend;
    unsigned int disable_hub_initiated_lpm;
    unsigned int soft_unbind;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct usb_driver {
    const char *name;
    int (*probe)(struct usb_interface *, const struct usb_device_id *);
    void (*disconnect)(struct usb_interface *);
    int (*unlocked_ioctl)(struct usb_interface *, unsigned int, void *);
    int (*suspend)(struct usb_interface *, pm_message_t);
    int (*resume)(struct usb_interface *);
    int (*reset_resume)(struct usb_interface *);
    int (*pre_reset)(struct usb_interface *);
    int (*post_reset)(struct usb_interface *);
    const struct usb_device_id *id_table;
    struct usb_dynids dynids;
    struct usbdrv_wrap drvwrap;
    unsigned int no_dynamic_id;
    unsigned int supports_autosuspend;
    unsigned int disable_hub_initiated_lpm;
    unsigned int soft_unbind;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct usb_driver {
    const char *name;
    int (*probe)(struct usb_interface *, const struct usb_device_id *);
    void (*disconnect)(struct usb_interface *);
    int (*unlocked_ioctl)(struct usb_interface *, unsigned int, void *);
    int (*suspend)(struct usb_interface *, pm_message_t);
    int (*resume)(struct usb_interface *);
    int (*reset_resume)(struct usb_interface *);
    int (*pre_reset)(struct usb_interface *);
    int (*post_reset)(struct usb_interface *);
    const struct usb_device_id *id_table;
    const struct attribute_group **dev_groups;
    struct usb_dynids dynids;
    struct usbdrv_wrap drvwrap;
    unsigned int no_dynamic_id;
    unsigned int supports_autosuspend;
    unsigned int disable_hub_initiated_lpm;
    unsigned int soft_unbind;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct usb_driver {
    const char *name;
    int (*probe)(struct usb_interface *, const struct usb_device_id *);
    void (*disconnect)(struct usb_interface *);
    int (*unlocked_ioctl)(struct usb_interface *, unsigned int, void *);
    int (*suspend)(struct usb_interface *, pm_message_t);
    int (*resume)(struct usb_interface *);
    int (*reset_resume)(struct usb_interface *);
    int (*pre_reset)(struct usb_interface *);
    int (*post_reset)(struct usb_interface *);
    const struct usb_device_id *id_table;
    const struct attribute_group **dev_groups;
    struct usb_dynids dynids;
    struct usbdrv_wrap drvwrap;
    unsigned int no_dynamic_id;
    unsigned int supports_autosuspend;
    unsigned int disable_hub_initiated_lpm;
    unsigned int soft_unbind;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct usb_driver {
    const char *name;
    int (*probe)(struct usb_interface *, const struct usb_device_id *);
    void (*disconnect)(struct usb_interface *);
    int (*unlocked_ioctl)(struct usb_interface *, unsigned int, void *);
    int (*suspend)(struct usb_interface *, pm_message_t);
    int (*resume)(struct usb_interface *);
    int (*reset_resume)(struct usb_interface *);
    int (*pre_reset)(struct usb_interface *);
    int (*post_reset)(struct usb_interface *);
    const struct usb_device_id *id_table;
    const struct attribute_group **dev_groups;
    struct usb_dynids dynids;
    struct usbdrv_wrap drvwrap;
    unsigned int no_dynamic_id;
    unsigned int supports_autosuspend;
    unsigned int disable_hub_initiated_lpm;
    unsigned int soft_unbind;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct usb_driver {
    const char *name;
    int (*probe)(struct usb_interface *, const struct usb_device_id *);
    void (*disconnect)(struct usb_interface *);
    int (*unlocked_ioctl)(struct usb_interface *, unsigned int, void *);
    int (*suspend)(struct usb_interface *, pm_message_t);
    int (*resume)(struct usb_interface *);
    int (*reset_resume)(struct usb_interface *);
    int (*pre_reset)(struct usb_interface *);
    int (*post_reset)(struct usb_interface *);
    const struct usb_device_id *id_table;
    const struct attribute_group **dev_groups;
    struct usb_dynids dynids;
    struct usbdrv_wrap drvwrap;
    unsigned int no_dynamic_id;
    unsigned int supports_autosuspend;
    unsigned int disable_hub_initiated_lpm;
    unsigned int soft_unbind;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct usb_driver {
    const char *name;
    int (*probe)(struct usb_interface *, const struct usb_device_id *);
    void (*disconnect)(struct usb_interface *);
    int (*unlocked_ioctl)(struct usb_interface *, unsigned int, void *);
    int (*suspend)(struct usb_interface *, pm_message_t);
    int (*resume)(struct usb_interface *);
    int (*reset_resume)(struct usb_interface *);
    int (*pre_reset)(struct usb_interface *);
    int (*post_reset)(struct usb_interface *);
    const struct usb_device_id *id_table;
    const struct attribute_group **dev_groups;
    struct usb_dynids dynids;
    struct usbdrv_wrap drvwrap;
    unsigned int no_dynamic_id;
    unsigned int supports_autosuspend;
    unsigned int disable_hub_initiated_lpm;
    unsigned int soft_unbind;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct usb_driver {
    const char *name;
    int (*probe)(struct usb_interface *, const struct usb_device_id *);
    void (*disconnect)(struct usb_interface *);
    int (*unlocked_ioctl)(struct usb_interface *, unsigned int, void *);
    int (*suspend)(struct usb_interface *, pm_message_t);
    int (*resume)(struct usb_interface *);
    int (*reset_resume)(struct usb_interface *);
    int (*pre_reset)(struct usb_interface *);
    int (*post_reset)(struct usb_interface *);
    const struct usb_device_id *id_table;
    const struct attribute_group **dev_groups;
    struct usb_dynids dynids;
    struct usbdrv_wrap drvwrap;
    unsigned int no_dynamic_id;
    unsigned int supports_autosuspend;
    unsigned int disable_hub_initiated_lpm;
    unsigned int soft_unbind;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct usb_driver {
    const char *name;
    int (*probe)(struct usb_interface *, const struct usb_device_id *);
    void (*disconnect)(struct usb_interface *);
    int (*unlocked_ioctl)(struct usb_interface *, unsigned int, void *);
    int (*suspend)(struct usb_interface *, pm_message_t);
    int (*resume)(struct usb_interface *);
    int (*reset_resume)(struct usb_interface *);
    int (*pre_reset)(struct usb_interface *);
    int (*post_reset)(struct usb_interface *);
    const struct usb_device_id *id_table;
    const struct attribute_group **dev_groups;
    struct usb_dynids dynids;
    struct usbdrv_wrap drvwrap;
    unsigned int no_dynamic_id;
    unsigned int supports_autosuspend;
    unsigned int disable_hub_initiated_lpm;
    unsigned int soft_unbind;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct usb_driver {
    const char *name;
    int (*probe)(struct usb_interface *, const struct usb_device_id *);
    void (*disconnect)(struct usb_interface *);
    int (*unlocked_ioctl)(struct usb_interface *, unsigned int, void *);
    int (*suspend)(struct usb_interface *, pm_message_t);
    int (*resume)(struct usb_interface *);
    int (*reset_resume)(struct usb_interface *);
    int (*pre_reset)(struct usb_interface *);
    int (*post_reset)(struct usb_interface *);
    const struct usb_device_id *id_table;
    const struct attribute_group **dev_groups;
    struct usb_dynids dynids;
    struct usbdrv_wrap drvwrap;
    unsigned int no_dynamic_id;
    unsigned int supports_autosuspend;
    unsigned int disable_hub_initiated_lpm;
    unsigned int soft_unbind;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct usb_driver {
    const char *name;
    int (*probe)(struct usb_interface *, const struct usb_device_id *);
    void (*disconnect)(struct usb_interface *);
    int (*unlocked_ioctl)(struct usb_interface *, unsigned int, void *);
    int (*suspend)(struct usb_interface *, pm_message_t);
    int (*resume)(struct usb_interface *);
    int (*reset_resume)(struct usb_interface *);
    int (*pre_reset)(struct usb_interface *);
    int (*post_reset)(struct usb_interface *);
    const struct usb_device_id *id_table;
    const struct attribute_group **dev_groups;
    struct usb_dynids dynids;
    struct device_driver driver;
    unsigned int no_dynamic_id;
    unsigned int supports_autosuspend;
    unsigned int disable_hub_initiated_lpm;
    unsigned int soft_unbind;
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
struct usb_driver {
    const char *name;
    int (*probe)(struct usb_interface *, const struct usb_device_id *);
    void (*disconnect)(struct usb_interface *);
    int (*unlocked_ioctl)(struct usb_interface *, unsigned int, void *);
    int (*suspend)(struct usb_interface *, pm_message_t);
    int (*resume)(struct usb_interface *);
    int (*reset_resume)(struct usb_interface *);
    int (*pre_reset)(struct usb_interface *);
    int (*post_reset)(struct usb_interface *);
    const struct usb_device_id *id_table;
    const struct attribute_group **dev_groups;
    struct usb_dynids dynids;
    struct usbdrv_wrap drvwrap;
    unsigned int no_dynamic_id;
    unsigned int supports_autosuspend;
    unsigned int disable_hub_initiated_lpm;
    unsigned int soft_unbind;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct usb_driver {
    const char *name;
    int (*probe)(struct usb_interface *, const struct usb_device_id *);
    void (*disconnect)(struct usb_interface *);
    int (*unlocked_ioctl)(struct usb_interface *, unsigned int, void *);
    int (*suspend)(struct usb_interface *, pm_message_t);
    int (*resume)(struct usb_interface *);
    int (*reset_resume)(struct usb_interface *);
    int (*pre_reset)(struct usb_interface *);
    int (*post_reset)(struct usb_interface *);
    const struct usb_device_id *id_table;
    const struct attribute_group **dev_groups;
    struct usb_dynids dynids;
    struct usbdrv_wrap drvwrap;
    unsigned int no_dynamic_id;
    unsigned int supports_autosuspend;
    unsigned int disable_hub_initiated_lpm;
    unsigned int soft_unbind;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct usb_driver {
    const char *name;
    int (*probe)(struct usb_interface *, const struct usb_device_id *);
    void (*disconnect)(struct usb_interface *);
    int (*unlocked_ioctl)(struct usb_interface *, unsigned int, void *);
    int (*suspend)(struct usb_interface *, pm_message_t);
    int (*resume)(struct usb_interface *);
    int (*reset_resume)(struct usb_interface *);
    int (*pre_reset)(struct usb_interface *);
    int (*post_reset)(struct usb_interface *);
    const struct usb_device_id *id_table;
    const struct attribute_group **dev_groups;
    struct usb_dynids dynids;
    struct usbdrv_wrap drvwrap;
    unsigned int no_dynamic_id;
    unsigned int supports_autosuspend;
    unsigned int disable_hub_initiated_lpm;
    unsigned int soft_unbind;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct usb_driver {
    const char *name;
    int (*probe)(struct usb_interface *, const struct usb_device_id *);
    void (*disconnect)(struct usb_interface *);
    int (*unlocked_ioctl)(struct usb_interface *, unsigned int, void *);
    int (*suspend)(struct usb_interface *, pm_message_t);
    int (*resume)(struct usb_interface *);
    int (*reset_resume)(struct usb_interface *);
    int (*pre_reset)(struct usb_interface *);
    int (*post_reset)(struct usb_interface *);
    const struct usb_device_id *id_table;
    const struct attribute_group **dev_groups;
    struct usb_dynids dynids;
    struct usbdrv_wrap drvwrap;
    unsigned int no_dynamic_id;
    unsigned int supports_autosuspend;
    unsigned int disable_hub_initiated_lpm;
    unsigned int soft_unbind;
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
struct usb_driver {
    const char *name;
    int (*probe)(struct usb_interface *, const struct usb_device_id *);
    void (*disconnect)(struct usb_interface *);
    int (*unlocked_ioctl)(struct usb_interface *, unsigned int, void *);
    int (*suspend)(struct usb_interface *, pm_message_t);
    int (*resume)(struct usb_interface *);
    int (*reset_resume)(struct usb_interface *);
    int (*pre_reset)(struct usb_interface *);
    int (*post_reset)(struct usb_interface *);
    const struct usb_device_id *id_table;
    const struct attribute_group **dev_groups;
    struct usb_dynids dynids;
    struct usbdrv_wrap drvwrap;
    unsigned int no_dynamic_id;
    unsigned int supports_autosuspend;
    unsigned int disable_hub_initiated_lpm;
    unsigned int soft_unbind;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct usb_driver {
    const char *name;
    int (*probe)(struct usb_interface *, const struct usb_device_id *);
    void (*disconnect)(struct usb_interface *);
    int (*unlocked_ioctl)(struct usb_interface *, unsigned int, void *);
    int (*suspend)(struct usb_interface *, pm_message_t);
    int (*resume)(struct usb_interface *);
    int (*reset_resume)(struct usb_interface *);
    int (*pre_reset)(struct usb_interface *);
    int (*post_reset)(struct usb_interface *);
    const struct usb_device_id *id_table;
    const struct attribute_group **dev_groups;
    struct usb_dynids dynids;
    struct usbdrv_wrap drvwrap;
    unsigned int no_dynamic_id;
    unsigned int supports_autosuspend;
    unsigned int disable_hub_initiated_lpm;
    unsigned int soft_unbind;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct usb_driver {
    const char *name;
    int (*probe)(struct usb_interface *, const struct usb_device_id *);
    void (*disconnect)(struct usb_interface *);
    int (*unlocked_ioctl)(struct usb_interface *, unsigned int, void *);
    int (*suspend)(struct usb_interface *, pm_message_t);
    int (*resume)(struct usb_interface *);
    int (*reset_resume)(struct usb_interface *);
    int (*pre_reset)(struct usb_interface *);
    int (*post_reset)(struct usb_interface *);
    const struct usb_device_id *id_table;
    const struct attribute_group **dev_groups;
    struct usb_dynids dynids;
    struct usbdrv_wrap drvwrap;
    unsigned int no_dynamic_id;
    unsigned int supports_autosuspend;
    unsigned int disable_hub_initiated_lpm;
    unsigned int soft_unbind;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct usb_driver {
    const char *name;
    int (*probe)(struct usb_interface *, const struct usb_device_id *);
    void (*disconnect)(struct usb_interface *);
    int (*unlocked_ioctl)(struct usb_interface *, unsigned int, void *);
    int (*suspend)(struct usb_interface *, pm_message_t);
    int (*resume)(struct usb_interface *);
    int (*reset_resume)(struct usb_interface *);
    int (*pre_reset)(struct usb_interface *);
    int (*post_reset)(struct usb_interface *);
    const struct usb_device_id *id_table;
    const struct attribute_group **dev_groups;
    struct usb_dynids dynids;
    struct usbdrv_wrap drvwrap;
    unsigned int no_dynamic_id;
    unsigned int supports_autosuspend;
    unsigned int disable_hub_initiated_lpm;
    unsigned int soft_unbind;
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
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const struct attribute_group **dev_groups</code>
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
<b>Field added. </b>
<code>struct device_driver driver</code>
</li>
<li>
<b>Field removed. </b>
<code>struct usbdrv_wrap drvwrap</code>
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
