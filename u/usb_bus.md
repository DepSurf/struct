# Struct: <code>usb_bus</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct usb_bus {
    struct device *controller;
    int busnum;
    const char *bus_name;
    u8 uses_dma;
    u8 uses_pio_for_control;
    u8 otg_port;
    unsigned int is_b_host;
    unsigned int b_hnp_enable;
    unsigned int no_stop_on_short;
    unsigned int no_sg_constraint;
    unsigned int sg_tablesize;
    int devnum_next;
    struct usb_devmap devmap;
    struct usb_device *root_hub;
    struct usb_bus *hs_companion;
    struct list_head bus_list;
    struct mutex usb_address0_mutex;
    int bandwidth_allocated;
    int bandwidth_int_reqs;
    int bandwidth_isoc_reqs;
    unsigned int resuming_ports;
    struct mon_bus *mon_bus;
    int monitored;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct usb_bus {
    struct device *controller;
    int busnum;
    const char *bus_name;
    u8 uses_dma;
    u8 uses_pio_for_control;
    u8 otg_port;
    unsigned int is_b_host;
    unsigned int b_hnp_enable;
    unsigned int no_stop_on_short;
    unsigned int no_sg_constraint;
    unsigned int sg_tablesize;
    int devnum_next;
    struct mutex devnum_next_mutex;
    struct usb_devmap devmap;
    struct usb_device *root_hub;
    struct usb_bus *hs_companion;
    int bandwidth_allocated;
    int bandwidth_int_reqs;
    int bandwidth_isoc_reqs;
    unsigned int resuming_ports;
    struct mon_bus *mon_bus;
    int monitored;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct usb_bus {
    struct device *controller;
    int busnum;
    const char *bus_name;
    u8 uses_dma;
    u8 uses_pio_for_control;
    u8 otg_port;
    unsigned int is_b_host;
    unsigned int b_hnp_enable;
    unsigned int no_stop_on_short;
    unsigned int no_sg_constraint;
    unsigned int sg_tablesize;
    int devnum_next;
    struct mutex devnum_next_mutex;
    struct usb_devmap devmap;
    struct usb_device *root_hub;
    struct usb_bus *hs_companion;
    int bandwidth_allocated;
    int bandwidth_int_reqs;
    int bandwidth_isoc_reqs;
    unsigned int resuming_ports;
    struct mon_bus *mon_bus;
    int monitored;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct usb_bus {
    struct device *controller;
    struct device *sysdev;
    int busnum;
    const char *bus_name;
    u8 uses_dma;
    u8 uses_pio_for_control;
    u8 otg_port;
    unsigned int is_b_host;
    unsigned int b_hnp_enable;
    unsigned int no_stop_on_short;
    unsigned int no_sg_constraint;
    unsigned int sg_tablesize;
    int devnum_next;
    struct mutex devnum_next_mutex;
    struct usb_devmap devmap;
    struct usb_device *root_hub;
    struct usb_bus *hs_companion;
    int bandwidth_allocated;
    int bandwidth_int_reqs;
    int bandwidth_isoc_reqs;
    unsigned int resuming_ports;
    struct mon_bus *mon_bus;
    int monitored;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct usb_bus {
    struct device *controller;
    struct device *sysdev;
    int busnum;
    const char *bus_name;
    u8 uses_dma;
    u8 uses_pio_for_control;
    u8 otg_port;
    unsigned int is_b_host;
    unsigned int b_hnp_enable;
    unsigned int no_stop_on_short;
    unsigned int no_sg_constraint;
    unsigned int sg_tablesize;
    int devnum_next;
    struct mutex devnum_next_mutex;
    struct usb_devmap devmap;
    struct usb_device *root_hub;
    struct usb_bus *hs_companion;
    int bandwidth_allocated;
    int bandwidth_int_reqs;
    int bandwidth_isoc_reqs;
    unsigned int resuming_ports;
    struct mon_bus *mon_bus;
    int monitored;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct usb_bus {
    struct device *controller;
    struct device *sysdev;
    int busnum;
    const char *bus_name;
    u8 uses_dma;
    u8 uses_pio_for_control;
    u8 otg_port;
    unsigned int is_b_host;
    unsigned int b_hnp_enable;
    unsigned int no_stop_on_short;
    unsigned int no_sg_constraint;
    unsigned int sg_tablesize;
    int devnum_next;
    struct mutex devnum_next_mutex;
    struct usb_devmap devmap;
    struct usb_device *root_hub;
    struct usb_bus *hs_companion;
    int bandwidth_allocated;
    int bandwidth_int_reqs;
    int bandwidth_isoc_reqs;
    unsigned int resuming_ports;
    struct mon_bus *mon_bus;
    int monitored;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct usb_bus {
    struct device *controller;
    struct device *sysdev;
    int busnum;
    const char *bus_name;
    u8 uses_dma;
    u8 uses_pio_for_control;
    u8 otg_port;
    unsigned int is_b_host;
    unsigned int b_hnp_enable;
    unsigned int no_stop_on_short;
    unsigned int no_sg_constraint;
    unsigned int sg_tablesize;
    int devnum_next;
    struct mutex devnum_next_mutex;
    struct usb_devmap devmap;
    struct usb_device *root_hub;
    struct usb_bus *hs_companion;
    int bandwidth_allocated;
    int bandwidth_int_reqs;
    int bandwidth_isoc_reqs;
    unsigned int resuming_ports;
    struct mon_bus *mon_bus;
    int monitored;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct usb_bus {
    struct device *controller;
    struct device *sysdev;
    int busnum;
    const char *bus_name;
    u8 uses_dma;
    u8 uses_pio_for_control;
    u8 otg_port;
    unsigned int is_b_host;
    unsigned int b_hnp_enable;
    unsigned int no_stop_on_short;
    unsigned int no_sg_constraint;
    unsigned int sg_tablesize;
    int devnum_next;
    struct mutex devnum_next_mutex;
    struct usb_devmap devmap;
    struct usb_device *root_hub;
    struct usb_bus *hs_companion;
    int bandwidth_allocated;
    int bandwidth_int_reqs;
    int bandwidth_isoc_reqs;
    unsigned int resuming_ports;
    struct mon_bus *mon_bus;
    int monitored;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct usb_bus {
    struct device *controller;
    struct device *sysdev;
    int busnum;
    const char *bus_name;
    u8 uses_pio_for_control;
    u8 otg_port;
    unsigned int is_b_host;
    unsigned int b_hnp_enable;
    unsigned int no_stop_on_short;
    unsigned int no_sg_constraint;
    unsigned int sg_tablesize;
    int devnum_next;
    struct mutex devnum_next_mutex;
    struct usb_devmap devmap;
    struct usb_device *root_hub;
    struct usb_bus *hs_companion;
    int bandwidth_allocated;
    int bandwidth_int_reqs;
    int bandwidth_isoc_reqs;
    unsigned int resuming_ports;
    struct mon_bus *mon_bus;
    int monitored;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct usb_bus {
    struct device *controller;
    struct device *sysdev;
    int busnum;
    const char *bus_name;
    u8 uses_pio_for_control;
    u8 otg_port;
    unsigned int is_b_host;
    unsigned int b_hnp_enable;
    unsigned int no_stop_on_short;
    unsigned int no_sg_constraint;
    unsigned int sg_tablesize;
    int devnum_next;
    struct mutex devnum_next_mutex;
    struct usb_devmap devmap;
    struct usb_device *root_hub;
    struct usb_bus *hs_companion;
    int bandwidth_allocated;
    int bandwidth_int_reqs;
    int bandwidth_isoc_reqs;
    unsigned int resuming_ports;
    struct mon_bus *mon_bus;
    int monitored;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct usb_bus {
    struct device *controller;
    struct device *sysdev;
    int busnum;
    const char *bus_name;
    u8 uses_pio_for_control;
    u8 otg_port;
    unsigned int is_b_host;
    unsigned int b_hnp_enable;
    unsigned int no_stop_on_short;
    unsigned int no_sg_constraint;
    unsigned int sg_tablesize;
    int devnum_next;
    struct mutex devnum_next_mutex;
    struct usb_devmap devmap;
    struct usb_device *root_hub;
    struct usb_bus *hs_companion;
    int bandwidth_allocated;
    int bandwidth_int_reqs;
    int bandwidth_isoc_reqs;
    unsigned int resuming_ports;
    struct mon_bus *mon_bus;
    int monitored;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct usb_bus {
    struct device *controller;
    struct device *sysdev;
    int busnum;
    const char *bus_name;
    u8 uses_pio_for_control;
    u8 otg_port;
    unsigned int is_b_host;
    unsigned int b_hnp_enable;
    unsigned int no_stop_on_short;
    unsigned int no_sg_constraint;
    unsigned int sg_tablesize;
    int devnum_next;
    struct mutex devnum_next_mutex;
    struct usb_devmap devmap;
    struct usb_device *root_hub;
    struct usb_bus *hs_companion;
    int bandwidth_allocated;
    int bandwidth_int_reqs;
    int bandwidth_isoc_reqs;
    unsigned int resuming_ports;
    struct mon_bus *mon_bus;
    int monitored;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct usb_bus {
    struct device *controller;
    struct device *sysdev;
    int busnum;
    const char *bus_name;
    u8 uses_pio_for_control;
    u8 otg_port;
    unsigned int is_b_host;
    unsigned int b_hnp_enable;
    unsigned int no_stop_on_short;
    unsigned int no_sg_constraint;
    unsigned int sg_tablesize;
    int devnum_next;
    struct mutex devnum_next_mutex;
    struct usb_devmap devmap;
    struct usb_device *root_hub;
    struct usb_bus *hs_companion;
    int bandwidth_allocated;
    int bandwidth_int_reqs;
    int bandwidth_isoc_reqs;
    unsigned int resuming_ports;
    struct mon_bus *mon_bus;
    int monitored;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct usb_bus {
    struct device *controller;
    struct device *sysdev;
    int busnum;
    const char *bus_name;
    u8 uses_pio_for_control;
    u8 otg_port;
    unsigned int is_b_host;
    unsigned int b_hnp_enable;
    unsigned int no_stop_on_short;
    unsigned int no_sg_constraint;
    unsigned int sg_tablesize;
    int devnum_next;
    struct mutex devnum_next_mutex;
    struct usb_devmap devmap;
    struct usb_device *root_hub;
    struct usb_bus *hs_companion;
    int bandwidth_allocated;
    int bandwidth_int_reqs;
    int bandwidth_isoc_reqs;
    unsigned int resuming_ports;
    struct mon_bus *mon_bus;
    int monitored;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct usb_bus {
    struct device *controller;
    struct device *sysdev;
    int busnum;
    const char *bus_name;
    u8 uses_pio_for_control;
    u8 otg_port;
    unsigned int is_b_host;
    unsigned int b_hnp_enable;
    unsigned int no_stop_on_short;
    unsigned int no_sg_constraint;
    unsigned int sg_tablesize;
    int devnum_next;
    struct mutex devnum_next_mutex;
    struct usb_devmap devmap;
    struct usb_device *root_hub;
    struct usb_bus *hs_companion;
    int bandwidth_allocated;
    int bandwidth_int_reqs;
    int bandwidth_isoc_reqs;
    unsigned int resuming_ports;
    struct mon_bus *mon_bus;
    int monitored;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct usb_bus {
    struct device *controller;
    struct device *sysdev;
    int busnum;
    const char *bus_name;
    u8 uses_pio_for_control;
    u8 otg_port;
    unsigned int is_b_host;
    unsigned int b_hnp_enable;
    unsigned int no_stop_on_short;
    unsigned int no_sg_constraint;
    unsigned int sg_tablesize;
    int devnum_next;
    struct mutex devnum_next_mutex;
    struct usb_devmap devmap;
    struct usb_device *root_hub;
    struct usb_bus *hs_companion;
    int bandwidth_allocated;
    int bandwidth_int_reqs;
    int bandwidth_isoc_reqs;
    unsigned int resuming_ports;
    struct mon_bus *mon_bus;
    int monitored;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct usb_bus {
    struct device *controller;
    struct device *sysdev;
    int busnum;
    const char *bus_name;
    u8 uses_pio_for_control;
    u8 otg_port;
    unsigned int is_b_host;
    unsigned int b_hnp_enable;
    unsigned int no_stop_on_short;
    unsigned int no_sg_constraint;
    unsigned int sg_tablesize;
    int devnum_next;
    struct mutex devnum_next_mutex;
    struct usb_devmap devmap;
    struct usb_device *root_hub;
    struct usb_bus *hs_companion;
    int bandwidth_allocated;
    int bandwidth_int_reqs;
    int bandwidth_isoc_reqs;
    unsigned int resuming_ports;
    struct mon_bus *mon_bus;
    int monitored;
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
struct usb_bus {
    struct device *controller;
    struct device *sysdev;
    int busnum;
    const char *bus_name;
    u8 uses_pio_for_control;
    u8 otg_port;
    unsigned int is_b_host;
    unsigned int b_hnp_enable;
    unsigned int no_stop_on_short;
    unsigned int no_sg_constraint;
    unsigned int sg_tablesize;
    int devnum_next;
    struct mutex devnum_next_mutex;
    struct usb_devmap devmap;
    struct usb_device *root_hub;
    struct usb_bus *hs_companion;
    int bandwidth_allocated;
    int bandwidth_int_reqs;
    int bandwidth_isoc_reqs;
    unsigned int resuming_ports;
    struct mon_bus *mon_bus;
    int monitored;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct usb_bus {
    struct device *controller;
    struct device *sysdev;
    int busnum;
    const char *bus_name;
    u8 uses_pio_for_control;
    u8 otg_port;
    unsigned int is_b_host;
    unsigned int b_hnp_enable;
    unsigned int no_stop_on_short;
    unsigned int no_sg_constraint;
    unsigned int sg_tablesize;
    int devnum_next;
    struct mutex devnum_next_mutex;
    struct usb_devmap devmap;
    struct usb_device *root_hub;
    struct usb_bus *hs_companion;
    int bandwidth_allocated;
    int bandwidth_int_reqs;
    int bandwidth_isoc_reqs;
    unsigned int resuming_ports;
    struct mon_bus *mon_bus;
    int monitored;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct usb_bus {
    struct device *controller;
    struct device *sysdev;
    int busnum;
    const char *bus_name;
    u8 uses_pio_for_control;
    u8 otg_port;
    unsigned int is_b_host;
    unsigned int b_hnp_enable;
    unsigned int no_stop_on_short;
    unsigned int no_sg_constraint;
    unsigned int sg_tablesize;
    int devnum_next;
    struct mutex devnum_next_mutex;
    struct usb_devmap devmap;
    struct usb_device *root_hub;
    struct usb_bus *hs_companion;
    int bandwidth_allocated;
    int bandwidth_int_reqs;
    int bandwidth_isoc_reqs;
    unsigned int resuming_ports;
    struct mon_bus *mon_bus;
    int monitored;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct usb_bus {
    struct device *controller;
    struct device *sysdev;
    int busnum;
    const char *bus_name;
    u8 uses_pio_for_control;
    u8 otg_port;
    unsigned int is_b_host;
    unsigned int b_hnp_enable;
    unsigned int no_stop_on_short;
    unsigned int no_sg_constraint;
    unsigned int sg_tablesize;
    int devnum_next;
    struct mutex devnum_next_mutex;
    struct usb_devmap devmap;
    struct usb_device *root_hub;
    struct usb_bus *hs_companion;
    int bandwidth_allocated;
    int bandwidth_int_reqs;
    int bandwidth_isoc_reqs;
    unsigned int resuming_ports;
    struct mon_bus *mon_bus;
    int monitored;
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
struct usb_bus {
    struct device *controller;
    struct device *sysdev;
    int busnum;
    const char *bus_name;
    u8 uses_pio_for_control;
    u8 otg_port;
    unsigned int is_b_host;
    unsigned int b_hnp_enable;
    unsigned int no_stop_on_short;
    unsigned int no_sg_constraint;
    unsigned int sg_tablesize;
    int devnum_next;
    struct mutex devnum_next_mutex;
    struct usb_devmap devmap;
    struct usb_device *root_hub;
    struct usb_bus *hs_companion;
    int bandwidth_allocated;
    int bandwidth_int_reqs;
    int bandwidth_isoc_reqs;
    unsigned int resuming_ports;
    struct mon_bus *mon_bus;
    int monitored;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct usb_bus {
    struct device *controller;
    struct device *sysdev;
    int busnum;
    const char *bus_name;
    u8 uses_pio_for_control;
    u8 otg_port;
    unsigned int is_b_host;
    unsigned int b_hnp_enable;
    unsigned int no_stop_on_short;
    unsigned int no_sg_constraint;
    unsigned int sg_tablesize;
    int devnum_next;
    struct mutex devnum_next_mutex;
    struct usb_devmap devmap;
    struct usb_device *root_hub;
    struct usb_bus *hs_companion;
    int bandwidth_allocated;
    int bandwidth_int_reqs;
    int bandwidth_isoc_reqs;
    unsigned int resuming_ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct usb_bus {
    struct device *controller;
    struct device *sysdev;
    int busnum;
    const char *bus_name;
    u8 uses_pio_for_control;
    u8 otg_port;
    unsigned int is_b_host;
    unsigned int b_hnp_enable;
    unsigned int no_stop_on_short;
    unsigned int no_sg_constraint;
    unsigned int sg_tablesize;
    int devnum_next;
    struct mutex devnum_next_mutex;
    struct usb_devmap devmap;
    struct usb_device *root_hub;
    struct usb_bus *hs_companion;
    int bandwidth_allocated;
    int bandwidth_int_reqs;
    int bandwidth_isoc_reqs;
    unsigned int resuming_ports;
    struct mon_bus *mon_bus;
    int monitored;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct usb_bus {
    struct device *controller;
    struct device *sysdev;
    int busnum;
    const char *bus_name;
    u8 uses_pio_for_control;
    u8 otg_port;
    unsigned int is_b_host;
    unsigned int b_hnp_enable;
    unsigned int no_stop_on_short;
    unsigned int no_sg_constraint;
    unsigned int sg_tablesize;
    int devnum_next;
    struct mutex devnum_next_mutex;
    struct usb_devmap devmap;
    struct usb_device *root_hub;
    struct usb_bus *hs_companion;
    int bandwidth_allocated;
    int bandwidth_int_reqs;
    int bandwidth_isoc_reqs;
    unsigned int resuming_ports;
    struct mon_bus *mon_bus;
    int monitored;
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
<code>struct mutex devnum_next_mutex</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head bus_list</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mutex usb_address0_mutex</code>
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
<code>struct device *sysdev</code>
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
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>u8 uses_dma</code>
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
<b>Field removed. </b>
<code>struct mon_bus *mon_bus</code>
</li>
<li>
<b>Field removed. </b>
<code>int monitored</code>
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
