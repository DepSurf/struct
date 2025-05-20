# Struct: <code>xhci_virt_device</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct xhci_virt_device {
    struct usb_device *udev;
    struct xhci_container_ctx *out_ctx;
    struct xhci_container_ctx *in_ctx;
    struct xhci_ring **ring_cache;
    int num_rings_cached;
    struct xhci_virt_ep eps[31];
    struct completion cmd_completion;
    u8 fake_port;
    u8 real_port;
    struct xhci_interval_bw_table *bw_table;
    struct xhci_tt_bw_info *tt_info;
    u16 current_mel;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct xhci_virt_device {
    struct usb_device *udev;
    struct xhci_container_ctx *out_ctx;
    struct xhci_container_ctx *in_ctx;
    struct xhci_ring **ring_cache;
    int num_rings_cached;
    struct xhci_virt_ep eps[31];
    struct completion cmd_completion;
    u8 fake_port;
    u8 real_port;
    struct xhci_interval_bw_table *bw_table;
    struct xhci_tt_bw_info *tt_info;
    u16 current_mel;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct xhci_virt_device {
    struct usb_device *udev;
    struct xhci_container_ctx *out_ctx;
    struct xhci_container_ctx *in_ctx;
    struct xhci_ring **ring_cache;
    int num_rings_cached;
    struct xhci_virt_ep eps[31];
    u8 fake_port;
    u8 real_port;
    struct xhci_interval_bw_table *bw_table;
    struct xhci_tt_bw_info *tt_info;
    u16 current_mel;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct xhci_virt_device {
    struct usb_device *udev;
    struct xhci_container_ctx *out_ctx;
    struct xhci_container_ctx *in_ctx;
    struct xhci_virt_ep eps[31];
    u8 fake_port;
    u8 real_port;
    struct xhci_interval_bw_table *bw_table;
    struct xhci_tt_bw_info *tt_info;
    u16 current_mel;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct xhci_virt_device {
    struct usb_device *udev;
    struct xhci_container_ctx *out_ctx;
    struct xhci_container_ctx *in_ctx;
    struct xhci_virt_ep eps[31];
    u8 fake_port;
    u8 real_port;
    struct xhci_interval_bw_table *bw_table;
    struct xhci_tt_bw_info *tt_info;
    u16 current_mel;
    void *debugfs_private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct xhci_virt_device {
    struct usb_device *udev;
    struct xhci_container_ctx *out_ctx;
    struct xhci_container_ctx *in_ctx;
    struct xhci_virt_ep eps[31];
    u8 fake_port;
    u8 real_port;
    struct xhci_interval_bw_table *bw_table;
    struct xhci_tt_bw_info *tt_info;
    u16 current_mel;
    void *debugfs_private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct xhci_virt_device {
    struct usb_device *udev;
    struct xhci_container_ctx *out_ctx;
    struct xhci_container_ctx *in_ctx;
    struct xhci_virt_ep eps[31];
    u8 fake_port;
    u8 real_port;
    struct xhci_interval_bw_table *bw_table;
    struct xhci_tt_bw_info *tt_info;
    u16 current_mel;
    void *debugfs_private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct xhci_virt_device {
    struct usb_device *udev;
    struct xhci_container_ctx *out_ctx;
    struct xhci_container_ctx *in_ctx;
    struct xhci_virt_ep eps[31];
    u8 fake_port;
    u8 real_port;
    struct xhci_interval_bw_table *bw_table;
    struct xhci_tt_bw_info *tt_info;
    long unsigned int flags;
    u16 current_mel;
    void *debugfs_private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct xhci_virt_device {
    struct usb_device *udev;
    struct xhci_container_ctx *out_ctx;
    struct xhci_container_ctx *in_ctx;
    struct xhci_virt_ep eps[31];
    u8 fake_port;
    u8 real_port;
    struct xhci_interval_bw_table *bw_table;
    struct xhci_tt_bw_info *tt_info;
    long unsigned int flags;
    u16 current_mel;
    void *debugfs_private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct xhci_virt_device {
    struct usb_device *udev;
    struct xhci_container_ctx *out_ctx;
    struct xhci_container_ctx *in_ctx;
    struct xhci_virt_ep eps[31];
    u8 fake_port;
    u8 real_port;
    struct xhci_interval_bw_table *bw_table;
    struct xhci_tt_bw_info *tt_info;
    long unsigned int flags;
    u16 current_mel;
    void *debugfs_private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct xhci_virt_device {
    struct usb_device *udev;
    struct xhci_container_ctx *out_ctx;
    struct xhci_container_ctx *in_ctx;
    struct xhci_virt_ep eps[31];
    u8 fake_port;
    u8 real_port;
    struct xhci_interval_bw_table *bw_table;
    struct xhci_tt_bw_info *tt_info;
    long unsigned int flags;
    u16 current_mel;
    void *debugfs_private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct xhci_virt_device {
    int slot_id;
    struct usb_device *udev;
    struct xhci_container_ctx *out_ctx;
    struct xhci_container_ctx *in_ctx;
    struct xhci_virt_ep eps[31];
    u8 fake_port;
    u8 real_port;
    struct xhci_interval_bw_table *bw_table;
    struct xhci_tt_bw_info *tt_info;
    long unsigned int flags;
    u16 current_mel;
    void *debugfs_private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct xhci_virt_device {
    int slot_id;
    struct usb_device *udev;
    struct xhci_container_ctx *out_ctx;
    struct xhci_container_ctx *in_ctx;
    struct xhci_virt_ep eps[31];
    u8 fake_port;
    u8 real_port;
    struct xhci_interval_bw_table *bw_table;
    struct xhci_tt_bw_info *tt_info;
    long unsigned int flags;
    u16 current_mel;
    void *debugfs_private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct xhci_virt_device {
    int slot_id;
    struct usb_device *udev;
    struct xhci_container_ctx *out_ctx;
    struct xhci_container_ctx *in_ctx;
    struct xhci_virt_ep eps[31];
    u8 fake_port;
    u8 real_port;
    struct xhci_interval_bw_table *bw_table;
    struct xhci_tt_bw_info *tt_info;
    long unsigned int flags;
    u16 current_mel;
    void *debugfs_private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct xhci_virt_device {
    int slot_id;
    struct usb_device *udev;
    struct xhci_container_ctx *out_ctx;
    struct xhci_container_ctx *in_ctx;
    struct xhci_virt_ep eps[31];
    u8 fake_port;
    u8 real_port;
    struct xhci_interval_bw_table *bw_table;
    struct xhci_tt_bw_info *tt_info;
    long unsigned int flags;
    u16 current_mel;
    void *debugfs_private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct xhci_virt_device {
    int slot_id;
    struct usb_device *udev;
    struct xhci_container_ctx *out_ctx;
    struct xhci_container_ctx *in_ctx;
    struct xhci_virt_ep eps[31];
    u8 fake_port;
    u8 real_port;
    struct xhci_interval_bw_table *bw_table;
    struct xhci_tt_bw_info *tt_info;
    long unsigned int flags;
    u16 current_mel;
    void *debugfs_private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct xhci_virt_device {
    int slot_id;
    struct usb_device *udev;
    struct xhci_container_ctx *out_ctx;
    struct xhci_container_ctx *in_ctx;
    struct xhci_virt_ep eps[31];
    u8 fake_port;
    u8 real_port;
    struct xhci_interval_bw_table *bw_table;
    struct xhci_tt_bw_info *tt_info;
    long unsigned int flags;
    u16 current_mel;
    void *debugfs_private;
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
struct xhci_virt_device {
    struct usb_device *udev;
    struct xhci_container_ctx *out_ctx;
    struct xhci_container_ctx *in_ctx;
    struct xhci_virt_ep eps[31];
    u8 fake_port;
    u8 real_port;
    struct xhci_interval_bw_table *bw_table;
    struct xhci_tt_bw_info *tt_info;
    long unsigned int flags;
    u16 current_mel;
    void *debugfs_private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct xhci_virt_device {
    struct usb_device *udev;
    struct xhci_container_ctx *out_ctx;
    struct xhci_container_ctx *in_ctx;
    struct xhci_virt_ep eps[31];
    u8 fake_port;
    u8 real_port;
    struct xhci_interval_bw_table *bw_table;
    struct xhci_tt_bw_info *tt_info;
    long unsigned int flags;
    u16 current_mel;
    void *debugfs_private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct xhci_virt_device {
    struct usb_device *udev;
    struct xhci_container_ctx *out_ctx;
    struct xhci_container_ctx *in_ctx;
    struct xhci_virt_ep eps[31];
    u8 fake_port;
    u8 real_port;
    struct xhci_interval_bw_table *bw_table;
    struct xhci_tt_bw_info *tt_info;
    long unsigned int flags;
    u16 current_mel;
    void *debugfs_private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct xhci_virt_device {
    struct usb_device *udev;
    struct xhci_container_ctx *out_ctx;
    struct xhci_container_ctx *in_ctx;
    struct xhci_virt_ep eps[31];
    u8 fake_port;
    u8 real_port;
    struct xhci_interval_bw_table *bw_table;
    struct xhci_tt_bw_info *tt_info;
    long unsigned int flags;
    u16 current_mel;
    void *debugfs_private;
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
struct xhci_virt_device {
    struct usb_device *udev;
    struct xhci_container_ctx *out_ctx;
    struct xhci_container_ctx *in_ctx;
    struct xhci_virt_ep eps[31];
    u8 fake_port;
    u8 real_port;
    struct xhci_interval_bw_table *bw_table;
    struct xhci_tt_bw_info *tt_info;
    long unsigned int flags;
    u16 current_mel;
    void *debugfs_private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct xhci_virt_device {
    struct usb_device *udev;
    struct xhci_container_ctx *out_ctx;
    struct xhci_container_ctx *in_ctx;
    struct xhci_virt_ep eps[31];
    u8 fake_port;
    u8 real_port;
    struct xhci_interval_bw_table *bw_table;
    struct xhci_tt_bw_info *tt_info;
    long unsigned int flags;
    u16 current_mel;
    void *debugfs_private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct xhci_virt_device {
    struct usb_device *udev;
    struct xhci_container_ctx *out_ctx;
    struct xhci_container_ctx *in_ctx;
    struct xhci_virt_ep eps[31];
    u8 fake_port;
    u8 real_port;
    struct xhci_interval_bw_table *bw_table;
    struct xhci_tt_bw_info *tt_info;
    long unsigned int flags;
    u16 current_mel;
    void *debugfs_private;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct xhci_virt_device {
    struct usb_device *udev;
    struct xhci_container_ctx *out_ctx;
    struct xhci_container_ctx *in_ctx;
    struct xhci_virt_ep eps[31];
    u8 fake_port;
    u8 real_port;
    struct xhci_interval_bw_table *bw_table;
    struct xhci_tt_bw_info *tt_info;
    long unsigned int flags;
    u16 current_mel;
    void *debugfs_private;
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
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct completion cmd_completion</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct xhci_ring **ring_cache</code>
</li>
<li>
<b>Field removed. </b>
<code>int num_rings_cached</code>
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
<code>void *debugfs_private</code>
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int flags</code>
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
<code>int slot_id</code>
</li>
</ul>
</details>
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
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
