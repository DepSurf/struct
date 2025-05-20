# Struct: <code>xencons_info</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct xencons_info {
    struct list_head list;
    struct xenbus_device *xbdev;
    struct xencons_interface *intf;
    unsigned int evtchn;
    struct hvc_struct *hvc;
    int irq;
    int vtermno;
    grant_ref_t gntref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct xencons_info {
    struct list_head list;
    struct xenbus_device *xbdev;
    struct xencons_interface *intf;
    unsigned int evtchn;
    struct hvc_struct *hvc;
    int irq;
    int vtermno;
    grant_ref_t gntref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct xencons_info {
    struct list_head list;
    struct xenbus_device *xbdev;
    struct xencons_interface *intf;
    unsigned int evtchn;
    struct hvc_struct *hvc;
    int irq;
    int vtermno;
    grant_ref_t gntref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct xencons_info {
    struct list_head list;
    struct xenbus_device *xbdev;
    struct xencons_interface *intf;
    unsigned int evtchn;
    struct hvc_struct *hvc;
    int irq;
    int vtermno;
    grant_ref_t gntref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct xencons_info {
    struct list_head list;
    struct xenbus_device *xbdev;
    struct xencons_interface *intf;
    unsigned int evtchn;
    struct hvc_struct *hvc;
    int irq;
    int vtermno;
    grant_ref_t gntref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct xencons_info {
    struct list_head list;
    struct xenbus_device *xbdev;
    struct xencons_interface *intf;
    unsigned int evtchn;
    struct hvc_struct *hvc;
    int irq;
    int vtermno;
    grant_ref_t gntref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct xencons_info {
    struct list_head list;
    struct xenbus_device *xbdev;
    struct xencons_interface *intf;
    unsigned int evtchn;
    struct hvc_struct *hvc;
    int irq;
    int vtermno;
    grant_ref_t gntref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct xencons_info {
    struct list_head list;
    struct xenbus_device *xbdev;
    struct xencons_interface *intf;
    unsigned int evtchn;
    struct hvc_struct *hvc;
    int irq;
    int vtermno;
    grant_ref_t gntref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct xencons_info {
    struct list_head list;
    struct xenbus_device *xbdev;
    struct xencons_interface *intf;
    unsigned int evtchn;
    struct hvc_struct *hvc;
    int irq;
    int vtermno;
    grant_ref_t gntref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct xencons_info {
    struct list_head list;
    struct xenbus_device *xbdev;
    struct xencons_interface *intf;
    unsigned int evtchn;
    struct hvc_struct *hvc;
    int irq;
    int vtermno;
    grant_ref_t gntref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct xencons_info {
    struct list_head list;
    struct xenbus_device *xbdev;
    struct xencons_interface *intf;
    unsigned int evtchn;
    struct hvc_struct *hvc;
    int irq;
    int vtermno;
    grant_ref_t gntref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct xencons_info {
    struct list_head list;
    struct xenbus_device *xbdev;
    struct xencons_interface *intf;
    unsigned int evtchn;
    struct hvc_struct *hvc;
    int irq;
    int vtermno;
    grant_ref_t gntref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct xencons_info {
    struct list_head list;
    struct xenbus_device *xbdev;
    struct xencons_interface *intf;
    unsigned int evtchn;
    XENCONS_RING_IDX out_cons;
    unsigned int out_cons_same;
    struct hvc_struct *hvc;
    int irq;
    int vtermno;
    grant_ref_t gntref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct xencons_info {
    struct list_head list;
    struct xenbus_device *xbdev;
    struct xencons_interface *intf;
    unsigned int evtchn;
    XENCONS_RING_IDX out_cons;
    unsigned int out_cons_same;
    struct hvc_struct *hvc;
    int irq;
    int vtermno;
    grant_ref_t gntref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct xencons_info {
    struct list_head list;
    struct xenbus_device *xbdev;
    struct xencons_interface *intf;
    unsigned int evtchn;
    XENCONS_RING_IDX out_cons;
    unsigned int out_cons_same;
    struct hvc_struct *hvc;
    int irq;
    int vtermno;
    grant_ref_t gntref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct xencons_info {
    struct list_head list;
    struct xenbus_device *xbdev;
    struct xencons_interface *intf;
    unsigned int evtchn;
    XENCONS_RING_IDX out_cons;
    unsigned int out_cons_same;
    struct hvc_struct *hvc;
    int irq;
    int vtermno;
    grant_ref_t gntref;
    spinlock_t ring_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct xencons_info {
    struct list_head list;
    struct xenbus_device *xbdev;
    struct xencons_interface *intf;
    unsigned int evtchn;
    XENCONS_RING_IDX out_cons;
    unsigned int out_cons_same;
    struct hvc_struct *hvc;
    int irq;
    int vtermno;
    grant_ref_t gntref;
    spinlock_t ring_lock;
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
struct xencons_info {
    struct list_head list;
    struct xenbus_device *xbdev;
    struct xencons_interface *intf;
    unsigned int evtchn;
    struct hvc_struct *hvc;
    int irq;
    int vtermno;
    grant_ref_t gntref;
};
```
</details>
</li>
<li>
In <code>armhf</code>: Absent ⚠️
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct xencons_info {
    struct list_head list;
    struct xenbus_device *xbdev;
    struct xencons_interface *intf;
    unsigned int evtchn;
    struct hvc_struct *hvc;
    int irq;
    int vtermno;
    grant_ref_t gntref;
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
struct xencons_info {
    struct list_head list;
    struct xenbus_device *xbdev;
    struct xencons_interface *intf;
    unsigned int evtchn;
    struct hvc_struct *hvc;
    int irq;
    int vtermno;
    grant_ref_t gntref;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct xencons_info {
    struct list_head list;
    struct xenbus_device *xbdev;
    struct xencons_interface *intf;
    unsigned int evtchn;
    struct hvc_struct *hvc;
    int irq;
    int vtermno;
    grant_ref_t gntref;
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
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>XENCONS_RING_IDX out_cons</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int out_cons_same</code>
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
<code>spinlock_t ring_lock</code>
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
