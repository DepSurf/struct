# Struct: <code>uhci_qh</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct uhci_qh {
    __le32 link;
    __le32 element;
    dma_addr_t dma_handle;
    struct list_head node;
    struct usb_host_endpoint *hep;
    struct usb_device *udev;
    struct list_head queue;
    struct uhci_td *dummy_td;
    struct uhci_td *post_td;
    struct usb_iso_packet_descriptor *iso_packet_desc;
    long unsigned int advance_jiffies;
    unsigned int unlink_frame;
    unsigned int period;
    short int phase;
    short int load;
    unsigned int iso_frame;
    int state;
    int type;
    int skel;
    unsigned int initial_toggle;
    unsigned int needs_fixup;
    unsigned int is_stopped;
    unsigned int wait_expired;
    unsigned int bandwidth_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct uhci_qh {
    __le32 link;
    __le32 element;
    dma_addr_t dma_handle;
    struct list_head node;
    struct usb_host_endpoint *hep;
    struct usb_device *udev;
    struct list_head queue;
    struct uhci_td *dummy_td;
    struct uhci_td *post_td;
    struct usb_iso_packet_descriptor *iso_packet_desc;
    long unsigned int advance_jiffies;
    unsigned int unlink_frame;
    unsigned int period;
    short int phase;
    short int load;
    unsigned int iso_frame;
    int state;
    int type;
    int skel;
    unsigned int initial_toggle;
    unsigned int needs_fixup;
    unsigned int is_stopped;
    unsigned int wait_expired;
    unsigned int bandwidth_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct uhci_qh {
    __le32 link;
    __le32 element;
    dma_addr_t dma_handle;
    struct list_head node;
    struct usb_host_endpoint *hep;
    struct usb_device *udev;
    struct list_head queue;
    struct uhci_td *dummy_td;
    struct uhci_td *post_td;
    struct usb_iso_packet_descriptor *iso_packet_desc;
    long unsigned int advance_jiffies;
    unsigned int unlink_frame;
    unsigned int period;
    short int phase;
    short int load;
    unsigned int iso_frame;
    int state;
    int type;
    int skel;
    unsigned int initial_toggle;
    unsigned int needs_fixup;
    unsigned int is_stopped;
    unsigned int wait_expired;
    unsigned int bandwidth_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct uhci_qh {
    __le32 link;
    __le32 element;
    dma_addr_t dma_handle;
    struct list_head node;
    struct usb_host_endpoint *hep;
    struct usb_device *udev;
    struct list_head queue;
    struct uhci_td *dummy_td;
    struct uhci_td *post_td;
    struct usb_iso_packet_descriptor *iso_packet_desc;
    long unsigned int advance_jiffies;
    unsigned int unlink_frame;
    unsigned int period;
    short int phase;
    short int load;
    unsigned int iso_frame;
    int state;
    int type;
    int skel;
    unsigned int initial_toggle;
    unsigned int needs_fixup;
    unsigned int is_stopped;
    unsigned int wait_expired;
    unsigned int bandwidth_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct uhci_qh {
    __le32 link;
    __le32 element;
    dma_addr_t dma_handle;
    struct list_head node;
    struct usb_host_endpoint *hep;
    struct usb_device *udev;
    struct list_head queue;
    struct uhci_td *dummy_td;
    struct uhci_td *post_td;
    struct usb_iso_packet_descriptor *iso_packet_desc;
    long unsigned int advance_jiffies;
    unsigned int unlink_frame;
    unsigned int period;
    short int phase;
    short int load;
    unsigned int iso_frame;
    int state;
    int type;
    int skel;
    unsigned int initial_toggle;
    unsigned int needs_fixup;
    unsigned int is_stopped;
    unsigned int wait_expired;
    unsigned int bandwidth_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct uhci_qh {
    __le32 link;
    __le32 element;
    dma_addr_t dma_handle;
    struct list_head node;
    struct usb_host_endpoint *hep;
    struct usb_device *udev;
    struct list_head queue;
    struct uhci_td *dummy_td;
    struct uhci_td *post_td;
    struct usb_iso_packet_descriptor *iso_packet_desc;
    long unsigned int advance_jiffies;
    unsigned int unlink_frame;
    unsigned int period;
    short int phase;
    short int load;
    unsigned int iso_frame;
    int state;
    int type;
    int skel;
    unsigned int initial_toggle;
    unsigned int needs_fixup;
    unsigned int is_stopped;
    unsigned int wait_expired;
    unsigned int bandwidth_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct uhci_qh {
    __le32 link;
    __le32 element;
    dma_addr_t dma_handle;
    struct list_head node;
    struct usb_host_endpoint *hep;
    struct usb_device *udev;
    struct list_head queue;
    struct uhci_td *dummy_td;
    struct uhci_td *post_td;
    struct usb_iso_packet_descriptor *iso_packet_desc;
    long unsigned int advance_jiffies;
    unsigned int unlink_frame;
    unsigned int period;
    short int phase;
    short int load;
    unsigned int iso_frame;
    int state;
    int type;
    int skel;
    unsigned int initial_toggle;
    unsigned int needs_fixup;
    unsigned int is_stopped;
    unsigned int wait_expired;
    unsigned int bandwidth_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct uhci_qh {
    __le32 link;
    __le32 element;
    dma_addr_t dma_handle;
    struct list_head node;
    struct usb_host_endpoint *hep;
    struct usb_device *udev;
    struct list_head queue;
    struct uhci_td *dummy_td;
    struct uhci_td *post_td;
    struct usb_iso_packet_descriptor *iso_packet_desc;
    long unsigned int advance_jiffies;
    unsigned int unlink_frame;
    unsigned int period;
    short int phase;
    short int load;
    unsigned int iso_frame;
    int state;
    int type;
    int skel;
    unsigned int initial_toggle;
    unsigned int needs_fixup;
    unsigned int is_stopped;
    unsigned int wait_expired;
    unsigned int bandwidth_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct uhci_qh {
    __le32 link;
    __le32 element;
    dma_addr_t dma_handle;
    struct list_head node;
    struct usb_host_endpoint *hep;
    struct usb_device *udev;
    struct list_head queue;
    struct uhci_td *dummy_td;
    struct uhci_td *post_td;
    struct usb_iso_packet_descriptor *iso_packet_desc;
    long unsigned int advance_jiffies;
    unsigned int unlink_frame;
    unsigned int period;
    short int phase;
    short int load;
    unsigned int iso_frame;
    int state;
    int type;
    int skel;
    unsigned int initial_toggle;
    unsigned int needs_fixup;
    unsigned int is_stopped;
    unsigned int wait_expired;
    unsigned int bandwidth_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct uhci_qh {
    __le32 link;
    __le32 element;
    dma_addr_t dma_handle;
    struct list_head node;
    struct usb_host_endpoint *hep;
    struct usb_device *udev;
    struct list_head queue;
    struct uhci_td *dummy_td;
    struct uhci_td *post_td;
    struct usb_iso_packet_descriptor *iso_packet_desc;
    long unsigned int advance_jiffies;
    unsigned int unlink_frame;
    unsigned int period;
    short int phase;
    short int load;
    unsigned int iso_frame;
    int state;
    int type;
    int skel;
    unsigned int initial_toggle;
    unsigned int needs_fixup;
    unsigned int is_stopped;
    unsigned int wait_expired;
    unsigned int bandwidth_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct uhci_qh {
    __le32 link;
    __le32 element;
    dma_addr_t dma_handle;
    struct list_head node;
    struct usb_host_endpoint *hep;
    struct usb_device *udev;
    struct list_head queue;
    struct uhci_td *dummy_td;
    struct uhci_td *post_td;
    struct usb_iso_packet_descriptor *iso_packet_desc;
    long unsigned int advance_jiffies;
    unsigned int unlink_frame;
    unsigned int period;
    short int phase;
    short int load;
    unsigned int iso_frame;
    int state;
    int type;
    int skel;
    unsigned int initial_toggle;
    unsigned int needs_fixup;
    unsigned int is_stopped;
    unsigned int wait_expired;
    unsigned int bandwidth_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct uhci_qh {
    __le32 link;
    __le32 element;
    dma_addr_t dma_handle;
    struct list_head node;
    struct usb_host_endpoint *hep;
    struct usb_device *udev;
    struct list_head queue;
    struct uhci_td *dummy_td;
    struct uhci_td *post_td;
    struct usb_iso_packet_descriptor *iso_packet_desc;
    long unsigned int advance_jiffies;
    unsigned int unlink_frame;
    unsigned int period;
    short int phase;
    short int load;
    unsigned int iso_frame;
    int state;
    int type;
    int skel;
    unsigned int initial_toggle;
    unsigned int needs_fixup;
    unsigned int is_stopped;
    unsigned int wait_expired;
    unsigned int bandwidth_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct uhci_qh {
    __le32 link;
    __le32 element;
    dma_addr_t dma_handle;
    struct list_head node;
    struct usb_host_endpoint *hep;
    struct usb_device *udev;
    struct list_head queue;
    struct uhci_td *dummy_td;
    struct uhci_td *post_td;
    struct usb_iso_packet_descriptor *iso_packet_desc;
    long unsigned int advance_jiffies;
    unsigned int unlink_frame;
    unsigned int period;
    short int phase;
    short int load;
    unsigned int iso_frame;
    int state;
    int type;
    int skel;
    unsigned int initial_toggle;
    unsigned int needs_fixup;
    unsigned int is_stopped;
    unsigned int wait_expired;
    unsigned int bandwidth_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct uhci_qh {
    __le32 link;
    __le32 element;
    dma_addr_t dma_handle;
    struct list_head node;
    struct usb_host_endpoint *hep;
    struct usb_device *udev;
    struct list_head queue;
    struct uhci_td *dummy_td;
    struct uhci_td *post_td;
    struct usb_iso_packet_descriptor *iso_packet_desc;
    long unsigned int advance_jiffies;
    unsigned int unlink_frame;
    unsigned int period;
    short int phase;
    short int load;
    unsigned int iso_frame;
    int state;
    int type;
    int skel;
    unsigned int initial_toggle;
    unsigned int needs_fixup;
    unsigned int is_stopped;
    unsigned int wait_expired;
    unsigned int bandwidth_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct uhci_qh {
    __le32 link;
    __le32 element;
    dma_addr_t dma_handle;
    struct list_head node;
    struct usb_host_endpoint *hep;
    struct usb_device *udev;
    struct list_head queue;
    struct uhci_td *dummy_td;
    struct uhci_td *post_td;
    struct usb_iso_packet_descriptor *iso_packet_desc;
    long unsigned int advance_jiffies;
    unsigned int unlink_frame;
    unsigned int period;
    short int phase;
    short int load;
    unsigned int iso_frame;
    int state;
    int type;
    int skel;
    unsigned int initial_toggle;
    unsigned int needs_fixup;
    unsigned int is_stopped;
    unsigned int wait_expired;
    unsigned int bandwidth_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct uhci_qh {
    __le32 link;
    __le32 element;
    dma_addr_t dma_handle;
    struct list_head node;
    struct usb_host_endpoint *hep;
    struct usb_device *udev;
    struct list_head queue;
    struct uhci_td *dummy_td;
    struct uhci_td *post_td;
    struct usb_iso_packet_descriptor *iso_packet_desc;
    long unsigned int advance_jiffies;
    unsigned int unlink_frame;
    unsigned int period;
    short int phase;
    short int load;
    unsigned int iso_frame;
    int state;
    int type;
    int skel;
    unsigned int initial_toggle;
    unsigned int needs_fixup;
    unsigned int is_stopped;
    unsigned int wait_expired;
    unsigned int bandwidth_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct uhci_qh {
    __le32 link;
    __le32 element;
    dma_addr_t dma_handle;
    struct list_head node;
    struct usb_host_endpoint *hep;
    struct usb_device *udev;
    struct list_head queue;
    struct uhci_td *dummy_td;
    struct uhci_td *post_td;
    struct usb_iso_packet_descriptor *iso_packet_desc;
    long unsigned int advance_jiffies;
    unsigned int unlink_frame;
    unsigned int period;
    short int phase;
    short int load;
    unsigned int iso_frame;
    int state;
    int type;
    int skel;
    unsigned int initial_toggle;
    unsigned int needs_fixup;
    unsigned int is_stopped;
    unsigned int wait_expired;
    unsigned int bandwidth_reserved;
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
struct uhci_qh {
    __le32 link;
    __le32 element;
    dma_addr_t dma_handle;
    struct list_head node;
    struct usb_host_endpoint *hep;
    struct usb_device *udev;
    struct list_head queue;
    struct uhci_td *dummy_td;
    struct uhci_td *post_td;
    struct usb_iso_packet_descriptor *iso_packet_desc;
    long unsigned int advance_jiffies;
    unsigned int unlink_frame;
    unsigned int period;
    short int phase;
    short int load;
    unsigned int iso_frame;
    int state;
    int type;
    int skel;
    unsigned int initial_toggle;
    unsigned int needs_fixup;
    unsigned int is_stopped;
    unsigned int wait_expired;
    unsigned int bandwidth_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct uhci_qh {
    __le32 link;
    __le32 element;
    dma_addr_t dma_handle;
    struct list_head node;
    struct usb_host_endpoint *hep;
    struct usb_device *udev;
    struct list_head queue;
    struct uhci_td *dummy_td;
    struct uhci_td *post_td;
    struct usb_iso_packet_descriptor *iso_packet_desc;
    long unsigned int advance_jiffies;
    unsigned int unlink_frame;
    unsigned int period;
    short int phase;
    short int load;
    unsigned int iso_frame;
    int state;
    int type;
    int skel;
    unsigned int initial_toggle;
    unsigned int needs_fixup;
    unsigned int is_stopped;
    unsigned int wait_expired;
    unsigned int bandwidth_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct uhci_qh {
    __le32 link;
    __le32 element;
    dma_addr_t dma_handle;
    struct list_head node;
    struct usb_host_endpoint *hep;
    struct usb_device *udev;
    struct list_head queue;
    struct uhci_td *dummy_td;
    struct uhci_td *post_td;
    struct usb_iso_packet_descriptor *iso_packet_desc;
    long unsigned int advance_jiffies;
    unsigned int unlink_frame;
    unsigned int period;
    short int phase;
    short int load;
    unsigned int iso_frame;
    int state;
    int type;
    int skel;
    unsigned int initial_toggle;
    unsigned int needs_fixup;
    unsigned int is_stopped;
    unsigned int wait_expired;
    unsigned int bandwidth_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct uhci_qh {
    __le32 link;
    __le32 element;
    dma_addr_t dma_handle;
    struct list_head node;
    struct usb_host_endpoint *hep;
    struct usb_device *udev;
    struct list_head queue;
    struct uhci_td *dummy_td;
    struct uhci_td *post_td;
    struct usb_iso_packet_descriptor *iso_packet_desc;
    long unsigned int advance_jiffies;
    unsigned int unlink_frame;
    unsigned int period;
    short int phase;
    short int load;
    unsigned int iso_frame;
    int state;
    int type;
    int skel;
    unsigned int initial_toggle;
    unsigned int needs_fixup;
    unsigned int is_stopped;
    unsigned int wait_expired;
    unsigned int bandwidth_reserved;
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
struct uhci_qh {
    __le32 link;
    __le32 element;
    dma_addr_t dma_handle;
    struct list_head node;
    struct usb_host_endpoint *hep;
    struct usb_device *udev;
    struct list_head queue;
    struct uhci_td *dummy_td;
    struct uhci_td *post_td;
    struct usb_iso_packet_descriptor *iso_packet_desc;
    long unsigned int advance_jiffies;
    unsigned int unlink_frame;
    unsigned int period;
    short int phase;
    short int load;
    unsigned int iso_frame;
    int state;
    int type;
    int skel;
    unsigned int initial_toggle;
    unsigned int needs_fixup;
    unsigned int is_stopped;
    unsigned int wait_expired;
    unsigned int bandwidth_reserved;
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
struct uhci_qh {
    __le32 link;
    __le32 element;
    dma_addr_t dma_handle;
    struct list_head node;
    struct usb_host_endpoint *hep;
    struct usb_device *udev;
    struct list_head queue;
    struct uhci_td *dummy_td;
    struct uhci_td *post_td;
    struct usb_iso_packet_descriptor *iso_packet_desc;
    long unsigned int advance_jiffies;
    unsigned int unlink_frame;
    unsigned int period;
    short int phase;
    short int load;
    unsigned int iso_frame;
    int state;
    int type;
    int skel;
    unsigned int initial_toggle;
    unsigned int needs_fixup;
    unsigned int is_stopped;
    unsigned int wait_expired;
    unsigned int bandwidth_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct uhci_qh {
    __le32 link;
    __le32 element;
    dma_addr_t dma_handle;
    struct list_head node;
    struct usb_host_endpoint *hep;
    struct usb_device *udev;
    struct list_head queue;
    struct uhci_td *dummy_td;
    struct uhci_td *post_td;
    struct usb_iso_packet_descriptor *iso_packet_desc;
    long unsigned int advance_jiffies;
    unsigned int unlink_frame;
    unsigned int period;
    short int phase;
    short int load;
    unsigned int iso_frame;
    int state;
    int type;
    int skel;
    unsigned int initial_toggle;
    unsigned int needs_fixup;
    unsigned int is_stopped;
    unsigned int wait_expired;
    unsigned int bandwidth_reserved;
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
