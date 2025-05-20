# Struct: <code>usb_role_switch_desc</code>

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
In <code>5.0</code>: Absent ⚠️
</li>
<li>
In <code>5.3</code>: Absent ⚠️
</li>
<li>
In <code>5.4</code>: Absent ⚠️
</li>
<li>
In <code>5.8</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct usb_role_switch_desc {
    struct fwnode_handle *fwnode;
    struct device *usb2_port;
    struct device *usb3_port;
    struct device *udc;
    usb_role_switch_set_t set;
    usb_role_switch_get_t get;
    bool allow_userspace_control;
    void *driver_data;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct usb_role_switch_desc {
    struct fwnode_handle *fwnode;
    struct device *usb2_port;
    struct device *usb3_port;
    struct device *udc;
    usb_role_switch_set_t set;
    usb_role_switch_get_t get;
    bool allow_userspace_control;
    void *driver_data;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct usb_role_switch_desc {
    struct fwnode_handle *fwnode;
    struct device *usb2_port;
    struct device *usb3_port;
    struct device *udc;
    usb_role_switch_set_t set;
    usb_role_switch_get_t get;
    bool allow_userspace_control;
    void *driver_data;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct usb_role_switch_desc {
    struct fwnode_handle *fwnode;
    struct device *usb2_port;
    struct device *usb3_port;
    struct device *udc;
    usb_role_switch_set_t set;
    usb_role_switch_get_t get;
    bool allow_userspace_control;
    void *driver_data;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct usb_role_switch_desc {
    struct fwnode_handle *fwnode;
    struct device *usb2_port;
    struct device *usb3_port;
    struct device *udc;
    usb_role_switch_set_t set;
    usb_role_switch_get_t get;
    bool allow_userspace_control;
    void *driver_data;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct usb_role_switch_desc {
    struct fwnode_handle *fwnode;
    struct device *usb2_port;
    struct device *usb3_port;
    struct device *udc;
    usb_role_switch_set_t set;
    usb_role_switch_get_t get;
    bool allow_userspace_control;
    void *driver_data;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct usb_role_switch_desc {
    struct fwnode_handle *fwnode;
    struct device *usb2_port;
    struct device *usb3_port;
    struct device *udc;
    usb_role_switch_set_t set;
    usb_role_switch_get_t get;
    bool allow_userspace_control;
    void *driver_data;
    const char *name;
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
struct usb_role_switch_desc {
    struct fwnode_handle *fwnode;
    struct device *usb2_port;
    struct device *usb3_port;
    struct device *udc;
    usb_role_switch_set_t set;
    usb_role_switch_get_t get;
    bool allow_userspace_control;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct usb_role_switch_desc {
    struct fwnode_handle *fwnode;
    struct device *usb2_port;
    struct device *usb3_port;
    struct device *udc;
    usb_role_switch_set_t set;
    usb_role_switch_get_t get;
    bool allow_userspace_control;
};
```
</details>
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
</li>
<li>
In <code>riscv64</code>: Absent ⚠️
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
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
</ul>
