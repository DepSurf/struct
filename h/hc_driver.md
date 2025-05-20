# Struct: <code>hc_driver</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct hc_driver {
    const char *description;
    const char *product_desc;
    size_t hcd_priv_size;
    irqreturn_t (*irq)(struct usb_hcd *);
    int flags;
    int (*reset)(struct usb_hcd *);
    int (*start)(struct usb_hcd *);
    int (*pci_suspend)(struct usb_hcd *, bool);
    int (*pci_resume)(struct usb_hcd *, bool);
    void (*stop)(struct usb_hcd *);
    void (*shutdown)(struct usb_hcd *);
    int (*get_frame_number)(struct usb_hcd *);
    int (*urb_enqueue)(struct usb_hcd *, struct urb *, gfp_t);
    int (*urb_dequeue)(struct usb_hcd *, struct urb *, int);
    int (*map_urb_for_dma)(struct usb_hcd *, struct urb *, gfp_t);
    void (*unmap_urb_for_dma)(struct usb_hcd *, struct urb *);
    void (*endpoint_disable)(struct usb_hcd *, struct usb_host_endpoint *);
    void (*endpoint_reset)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*hub_status_data)(struct usb_hcd *, char *);
    int (*hub_control)(struct usb_hcd *, u16, u16, u16, char *, u16);
    int (*bus_suspend)(struct usb_hcd *);
    int (*bus_resume)(struct usb_hcd *);
    int (*start_port_reset)(struct usb_hcd *, unsigned int);
    void (*relinquish_port)(struct usb_hcd *, int);
    int (*port_handed_over)(struct usb_hcd *, int);
    void (*clear_tt_buffer_complete)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*alloc_dev)(struct usb_hcd *, struct usb_device *);
    void (*free_dev)(struct usb_hcd *, struct usb_device *);
    int (*alloc_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, unsigned int, gfp_t);
    int (*free_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, gfp_t);
    int (*add_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*drop_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*check_bandwidth)(struct usb_hcd *, struct usb_device *);
    void (*reset_bandwidth)(struct usb_hcd *, struct usb_device *);
    int (*address_device)(struct usb_hcd *, struct usb_device *);
    int (*enable_device)(struct usb_hcd *, struct usb_device *);
    int (*update_hub_device)(struct usb_hcd *, struct usb_device *, struct usb_tt *, gfp_t);
    int (*reset_device)(struct usb_hcd *, struct usb_device *);
    int (*update_device)(struct usb_hcd *, struct usb_device *);
    int (*set_usb2_hw_lpm)(struct usb_hcd *, struct usb_device *, int);
    int (*enable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*disable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*find_raw_port_number)(struct usb_hcd *, int);
    int (*port_power)(struct usb_hcd *, int, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct hc_driver {
    const char *description;
    const char *product_desc;
    size_t hcd_priv_size;
    irqreturn_t (*irq)(struct usb_hcd *);
    int flags;
    int (*reset)(struct usb_hcd *);
    int (*start)(struct usb_hcd *);
    int (*pci_suspend)(struct usb_hcd *, bool);
    int (*pci_resume)(struct usb_hcd *, bool);
    void (*stop)(struct usb_hcd *);
    void (*shutdown)(struct usb_hcd *);
    int (*get_frame_number)(struct usb_hcd *);
    int (*urb_enqueue)(struct usb_hcd *, struct urb *, gfp_t);
    int (*urb_dequeue)(struct usb_hcd *, struct urb *, int);
    int (*map_urb_for_dma)(struct usb_hcd *, struct urb *, gfp_t);
    void (*unmap_urb_for_dma)(struct usb_hcd *, struct urb *);
    void (*endpoint_disable)(struct usb_hcd *, struct usb_host_endpoint *);
    void (*endpoint_reset)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*hub_status_data)(struct usb_hcd *, char *);
    int (*hub_control)(struct usb_hcd *, u16, u16, u16, char *, u16);
    int (*bus_suspend)(struct usb_hcd *);
    int (*bus_resume)(struct usb_hcd *);
    int (*start_port_reset)(struct usb_hcd *, unsigned int);
    void (*relinquish_port)(struct usb_hcd *, int);
    int (*port_handed_over)(struct usb_hcd *, int);
    void (*clear_tt_buffer_complete)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*alloc_dev)(struct usb_hcd *, struct usb_device *);
    void (*free_dev)(struct usb_hcd *, struct usb_device *);
    int (*alloc_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, unsigned int, gfp_t);
    int (*free_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, gfp_t);
    int (*add_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*drop_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*check_bandwidth)(struct usb_hcd *, struct usb_device *);
    void (*reset_bandwidth)(struct usb_hcd *, struct usb_device *);
    int (*address_device)(struct usb_hcd *, struct usb_device *);
    int (*enable_device)(struct usb_hcd *, struct usb_device *);
    int (*update_hub_device)(struct usb_hcd *, struct usb_device *, struct usb_tt *, gfp_t);
    int (*reset_device)(struct usb_hcd *, struct usb_device *);
    int (*update_device)(struct usb_hcd *, struct usb_device *);
    int (*set_usb2_hw_lpm)(struct usb_hcd *, struct usb_device *, int);
    int (*enable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*disable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*find_raw_port_number)(struct usb_hcd *, int);
    int (*port_power)(struct usb_hcd *, int, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct hc_driver {
    const char *description;
    const char *product_desc;
    size_t hcd_priv_size;
    irqreturn_t (*irq)(struct usb_hcd *);
    int flags;
    int (*reset)(struct usb_hcd *);
    int (*start)(struct usb_hcd *);
    int (*pci_suspend)(struct usb_hcd *, bool);
    int (*pci_resume)(struct usb_hcd *, bool);
    void (*stop)(struct usb_hcd *);
    void (*shutdown)(struct usb_hcd *);
    int (*get_frame_number)(struct usb_hcd *);
    int (*urb_enqueue)(struct usb_hcd *, struct urb *, gfp_t);
    int (*urb_dequeue)(struct usb_hcd *, struct urb *, int);
    int (*map_urb_for_dma)(struct usb_hcd *, struct urb *, gfp_t);
    void (*unmap_urb_for_dma)(struct usb_hcd *, struct urb *);
    void (*endpoint_disable)(struct usb_hcd *, struct usb_host_endpoint *);
    void (*endpoint_reset)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*hub_status_data)(struct usb_hcd *, char *);
    int (*hub_control)(struct usb_hcd *, u16, u16, u16, char *, u16);
    int (*bus_suspend)(struct usb_hcd *);
    int (*bus_resume)(struct usb_hcd *);
    int (*start_port_reset)(struct usb_hcd *, unsigned int);
    void (*relinquish_port)(struct usb_hcd *, int);
    int (*port_handed_over)(struct usb_hcd *, int);
    void (*clear_tt_buffer_complete)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*alloc_dev)(struct usb_hcd *, struct usb_device *);
    void (*free_dev)(struct usb_hcd *, struct usb_device *);
    int (*alloc_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, unsigned int, gfp_t);
    int (*free_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, gfp_t);
    int (*add_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*drop_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*check_bandwidth)(struct usb_hcd *, struct usb_device *);
    void (*reset_bandwidth)(struct usb_hcd *, struct usb_device *);
    int (*address_device)(struct usb_hcd *, struct usb_device *);
    int (*enable_device)(struct usb_hcd *, struct usb_device *);
    int (*update_hub_device)(struct usb_hcd *, struct usb_device *, struct usb_tt *, gfp_t);
    int (*reset_device)(struct usb_hcd *, struct usb_device *);
    int (*update_device)(struct usb_hcd *, struct usb_device *);
    int (*set_usb2_hw_lpm)(struct usb_hcd *, struct usb_device *, int);
    int (*enable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*disable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*find_raw_port_number)(struct usb_hcd *, int);
    int (*port_power)(struct usb_hcd *, int, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct hc_driver {
    const char *description;
    const char *product_desc;
    size_t hcd_priv_size;
    irqreturn_t (*irq)(struct usb_hcd *);
    int flags;
    int (*reset)(struct usb_hcd *);
    int (*start)(struct usb_hcd *);
    int (*pci_suspend)(struct usb_hcd *, bool);
    int (*pci_resume)(struct usb_hcd *, bool);
    void (*stop)(struct usb_hcd *);
    void (*shutdown)(struct usb_hcd *);
    int (*get_frame_number)(struct usb_hcd *);
    int (*urb_enqueue)(struct usb_hcd *, struct urb *, gfp_t);
    int (*urb_dequeue)(struct usb_hcd *, struct urb *, int);
    int (*map_urb_for_dma)(struct usb_hcd *, struct urb *, gfp_t);
    void (*unmap_urb_for_dma)(struct usb_hcd *, struct urb *);
    void (*endpoint_disable)(struct usb_hcd *, struct usb_host_endpoint *);
    void (*endpoint_reset)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*hub_status_data)(struct usb_hcd *, char *);
    int (*hub_control)(struct usb_hcd *, u16, u16, u16, char *, u16);
    int (*bus_suspend)(struct usb_hcd *);
    int (*bus_resume)(struct usb_hcd *);
    int (*start_port_reset)(struct usb_hcd *, unsigned int);
    void (*relinquish_port)(struct usb_hcd *, int);
    int (*port_handed_over)(struct usb_hcd *, int);
    void (*clear_tt_buffer_complete)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*alloc_dev)(struct usb_hcd *, struct usb_device *);
    void (*free_dev)(struct usb_hcd *, struct usb_device *);
    int (*alloc_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, unsigned int, gfp_t);
    int (*free_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, gfp_t);
    int (*add_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*drop_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*check_bandwidth)(struct usb_hcd *, struct usb_device *);
    void (*reset_bandwidth)(struct usb_hcd *, struct usb_device *);
    int (*address_device)(struct usb_hcd *, struct usb_device *);
    int (*enable_device)(struct usb_hcd *, struct usb_device *);
    int (*update_hub_device)(struct usb_hcd *, struct usb_device *, struct usb_tt *, gfp_t);
    int (*reset_device)(struct usb_hcd *, struct usb_device *);
    int (*update_device)(struct usb_hcd *, struct usb_device *);
    int (*set_usb2_hw_lpm)(struct usb_hcd *, struct usb_device *, int);
    int (*enable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*disable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*find_raw_port_number)(struct usb_hcd *, int);
    int (*port_power)(struct usb_hcd *, int, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct hc_driver {
    const char *description;
    const char *product_desc;
    size_t hcd_priv_size;
    irqreturn_t (*irq)(struct usb_hcd *);
    int flags;
    int (*reset)(struct usb_hcd *);
    int (*start)(struct usb_hcd *);
    int (*pci_suspend)(struct usb_hcd *, bool);
    int (*pci_resume)(struct usb_hcd *, bool);
    void (*stop)(struct usb_hcd *);
    void (*shutdown)(struct usb_hcd *);
    int (*get_frame_number)(struct usb_hcd *);
    int (*urb_enqueue)(struct usb_hcd *, struct urb *, gfp_t);
    int (*urb_dequeue)(struct usb_hcd *, struct urb *, int);
    int (*map_urb_for_dma)(struct usb_hcd *, struct urb *, gfp_t);
    void (*unmap_urb_for_dma)(struct usb_hcd *, struct urb *);
    void (*endpoint_disable)(struct usb_hcd *, struct usb_host_endpoint *);
    void (*endpoint_reset)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*hub_status_data)(struct usb_hcd *, char *);
    int (*hub_control)(struct usb_hcd *, u16, u16, u16, char *, u16);
    int (*bus_suspend)(struct usb_hcd *);
    int (*bus_resume)(struct usb_hcd *);
    int (*start_port_reset)(struct usb_hcd *, unsigned int);
    void (*relinquish_port)(struct usb_hcd *, int);
    int (*port_handed_over)(struct usb_hcd *, int);
    void (*clear_tt_buffer_complete)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*alloc_dev)(struct usb_hcd *, struct usb_device *);
    void (*free_dev)(struct usb_hcd *, struct usb_device *);
    int (*alloc_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, unsigned int, gfp_t);
    int (*free_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, gfp_t);
    int (*add_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*drop_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*check_bandwidth)(struct usb_hcd *, struct usb_device *);
    void (*reset_bandwidth)(struct usb_hcd *, struct usb_device *);
    int (*address_device)(struct usb_hcd *, struct usb_device *);
    int (*enable_device)(struct usb_hcd *, struct usb_device *);
    int (*update_hub_device)(struct usb_hcd *, struct usb_device *, struct usb_tt *, gfp_t);
    int (*reset_device)(struct usb_hcd *, struct usb_device *);
    int (*update_device)(struct usb_hcd *, struct usb_device *);
    int (*set_usb2_hw_lpm)(struct usb_hcd *, struct usb_device *, int);
    int (*enable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*disable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*find_raw_port_number)(struct usb_hcd *, int);
    int (*port_power)(struct usb_hcd *, int, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct hc_driver {
    const char *description;
    const char *product_desc;
    size_t hcd_priv_size;
    irqreturn_t (*irq)(struct usb_hcd *);
    int flags;
    int (*reset)(struct usb_hcd *);
    int (*start)(struct usb_hcd *);
    int (*pci_suspend)(struct usb_hcd *, bool);
    int (*pci_resume)(struct usb_hcd *, bool);
    void (*stop)(struct usb_hcd *);
    void (*shutdown)(struct usb_hcd *);
    int (*get_frame_number)(struct usb_hcd *);
    int (*urb_enqueue)(struct usb_hcd *, struct urb *, gfp_t);
    int (*urb_dequeue)(struct usb_hcd *, struct urb *, int);
    int (*map_urb_for_dma)(struct usb_hcd *, struct urb *, gfp_t);
    void (*unmap_urb_for_dma)(struct usb_hcd *, struct urb *);
    void (*endpoint_disable)(struct usb_hcd *, struct usb_host_endpoint *);
    void (*endpoint_reset)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*hub_status_data)(struct usb_hcd *, char *);
    int (*hub_control)(struct usb_hcd *, u16, u16, u16, char *, u16);
    int (*bus_suspend)(struct usb_hcd *);
    int (*bus_resume)(struct usb_hcd *);
    int (*start_port_reset)(struct usb_hcd *, unsigned int);
    void (*relinquish_port)(struct usb_hcd *, int);
    int (*port_handed_over)(struct usb_hcd *, int);
    void (*clear_tt_buffer_complete)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*alloc_dev)(struct usb_hcd *, struct usb_device *);
    void (*free_dev)(struct usb_hcd *, struct usb_device *);
    int (*alloc_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, unsigned int, gfp_t);
    int (*free_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, gfp_t);
    int (*add_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*drop_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*check_bandwidth)(struct usb_hcd *, struct usb_device *);
    void (*reset_bandwidth)(struct usb_hcd *, struct usb_device *);
    int (*address_device)(struct usb_hcd *, struct usb_device *);
    int (*enable_device)(struct usb_hcd *, struct usb_device *);
    int (*update_hub_device)(struct usb_hcd *, struct usb_device *, struct usb_tt *, gfp_t);
    int (*reset_device)(struct usb_hcd *, struct usb_device *);
    int (*update_device)(struct usb_hcd *, struct usb_device *);
    int (*set_usb2_hw_lpm)(struct usb_hcd *, struct usb_device *, int);
    int (*enable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*disable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*find_raw_port_number)(struct usb_hcd *, int);
    int (*port_power)(struct usb_hcd *, int, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct hc_driver {
    const char *description;
    const char *product_desc;
    size_t hcd_priv_size;
    irqreturn_t (*irq)(struct usb_hcd *);
    int flags;
    int (*reset)(struct usb_hcd *);
    int (*start)(struct usb_hcd *);
    int (*pci_suspend)(struct usb_hcd *, bool);
    int (*pci_resume)(struct usb_hcd *, bool);
    void (*stop)(struct usb_hcd *);
    void (*shutdown)(struct usb_hcd *);
    int (*get_frame_number)(struct usb_hcd *);
    int (*urb_enqueue)(struct usb_hcd *, struct urb *, gfp_t);
    int (*urb_dequeue)(struct usb_hcd *, struct urb *, int);
    int (*map_urb_for_dma)(struct usb_hcd *, struct urb *, gfp_t);
    void (*unmap_urb_for_dma)(struct usb_hcd *, struct urb *);
    void (*endpoint_disable)(struct usb_hcd *, struct usb_host_endpoint *);
    void (*endpoint_reset)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*hub_status_data)(struct usb_hcd *, char *);
    int (*hub_control)(struct usb_hcd *, u16, u16, u16, char *, u16);
    int (*bus_suspend)(struct usb_hcd *);
    int (*bus_resume)(struct usb_hcd *);
    int (*start_port_reset)(struct usb_hcd *, unsigned int);
    long unsigned int (*get_resuming_ports)(struct usb_hcd *);
    void (*relinquish_port)(struct usb_hcd *, int);
    int (*port_handed_over)(struct usb_hcd *, int);
    void (*clear_tt_buffer_complete)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*alloc_dev)(struct usb_hcd *, struct usb_device *);
    void (*free_dev)(struct usb_hcd *, struct usb_device *);
    int (*alloc_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, unsigned int, gfp_t);
    int (*free_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, gfp_t);
    int (*add_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*drop_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*check_bandwidth)(struct usb_hcd *, struct usb_device *);
    void (*reset_bandwidth)(struct usb_hcd *, struct usb_device *);
    int (*address_device)(struct usb_hcd *, struct usb_device *);
    int (*enable_device)(struct usb_hcd *, struct usb_device *);
    int (*update_hub_device)(struct usb_hcd *, struct usb_device *, struct usb_tt *, gfp_t);
    int (*reset_device)(struct usb_hcd *, struct usb_device *);
    int (*update_device)(struct usb_hcd *, struct usb_device *);
    int (*set_usb2_hw_lpm)(struct usb_hcd *, struct usb_device *, int);
    int (*enable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*disable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*find_raw_port_number)(struct usb_hcd *, int);
    int (*port_power)(struct usb_hcd *, int, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct hc_driver {
    const char *description;
    const char *product_desc;
    size_t hcd_priv_size;
    irqreturn_t (*irq)(struct usb_hcd *);
    int flags;
    int (*reset)(struct usb_hcd *);
    int (*start)(struct usb_hcd *);
    int (*pci_suspend)(struct usb_hcd *, bool);
    int (*pci_resume)(struct usb_hcd *, bool);
    void (*stop)(struct usb_hcd *);
    void (*shutdown)(struct usb_hcd *);
    int (*get_frame_number)(struct usb_hcd *);
    int (*urb_enqueue)(struct usb_hcd *, struct urb *, gfp_t);
    int (*urb_dequeue)(struct usb_hcd *, struct urb *, int);
    int (*map_urb_for_dma)(struct usb_hcd *, struct urb *, gfp_t);
    void (*unmap_urb_for_dma)(struct usb_hcd *, struct urb *);
    void (*endpoint_disable)(struct usb_hcd *, struct usb_host_endpoint *);
    void (*endpoint_reset)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*hub_status_data)(struct usb_hcd *, char *);
    int (*hub_control)(struct usb_hcd *, u16, u16, u16, char *, u16);
    int (*bus_suspend)(struct usb_hcd *);
    int (*bus_resume)(struct usb_hcd *);
    int (*start_port_reset)(struct usb_hcd *, unsigned int);
    long unsigned int (*get_resuming_ports)(struct usb_hcd *);
    void (*relinquish_port)(struct usb_hcd *, int);
    int (*port_handed_over)(struct usb_hcd *, int);
    void (*clear_tt_buffer_complete)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*alloc_dev)(struct usb_hcd *, struct usb_device *);
    void (*free_dev)(struct usb_hcd *, struct usb_device *);
    int (*alloc_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, unsigned int, gfp_t);
    int (*free_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, gfp_t);
    int (*add_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*drop_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*check_bandwidth)(struct usb_hcd *, struct usb_device *);
    void (*reset_bandwidth)(struct usb_hcd *, struct usb_device *);
    int (*address_device)(struct usb_hcd *, struct usb_device *);
    int (*enable_device)(struct usb_hcd *, struct usb_device *);
    int (*update_hub_device)(struct usb_hcd *, struct usb_device *, struct usb_tt *, gfp_t);
    int (*reset_device)(struct usb_hcd *, struct usb_device *);
    int (*update_device)(struct usb_hcd *, struct usb_device *);
    int (*set_usb2_hw_lpm)(struct usb_hcd *, struct usb_device *, int);
    int (*enable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*disable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*find_raw_port_number)(struct usb_hcd *, int);
    int (*port_power)(struct usb_hcd *, int, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct hc_driver {
    const char *description;
    const char *product_desc;
    size_t hcd_priv_size;
    irqreturn_t (*irq)(struct usb_hcd *);
    int flags;
    int (*reset)(struct usb_hcd *);
    int (*start)(struct usb_hcd *);
    int (*pci_suspend)(struct usb_hcd *, bool);
    int (*pci_resume)(struct usb_hcd *, bool);
    void (*stop)(struct usb_hcd *);
    void (*shutdown)(struct usb_hcd *);
    int (*get_frame_number)(struct usb_hcd *);
    int (*urb_enqueue)(struct usb_hcd *, struct urb *, gfp_t);
    int (*urb_dequeue)(struct usb_hcd *, struct urb *, int);
    int (*map_urb_for_dma)(struct usb_hcd *, struct urb *, gfp_t);
    void (*unmap_urb_for_dma)(struct usb_hcd *, struct urb *);
    void (*endpoint_disable)(struct usb_hcd *, struct usb_host_endpoint *);
    void (*endpoint_reset)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*hub_status_data)(struct usb_hcd *, char *);
    int (*hub_control)(struct usb_hcd *, u16, u16, u16, char *, u16);
    int (*bus_suspend)(struct usb_hcd *);
    int (*bus_resume)(struct usb_hcd *);
    int (*start_port_reset)(struct usb_hcd *, unsigned int);
    long unsigned int (*get_resuming_ports)(struct usb_hcd *);
    void (*relinquish_port)(struct usb_hcd *, int);
    int (*port_handed_over)(struct usb_hcd *, int);
    void (*clear_tt_buffer_complete)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*alloc_dev)(struct usb_hcd *, struct usb_device *);
    void (*free_dev)(struct usb_hcd *, struct usb_device *);
    int (*alloc_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, unsigned int, gfp_t);
    int (*free_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, gfp_t);
    int (*add_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*drop_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*check_bandwidth)(struct usb_hcd *, struct usb_device *);
    void (*reset_bandwidth)(struct usb_hcd *, struct usb_device *);
    int (*address_device)(struct usb_hcd *, struct usb_device *);
    int (*enable_device)(struct usb_hcd *, struct usb_device *);
    int (*update_hub_device)(struct usb_hcd *, struct usb_device *, struct usb_tt *, gfp_t);
    int (*reset_device)(struct usb_hcd *, struct usb_device *);
    int (*update_device)(struct usb_hcd *, struct usb_device *);
    int (*set_usb2_hw_lpm)(struct usb_hcd *, struct usb_device *, int);
    int (*enable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*disable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*find_raw_port_number)(struct usb_hcd *, int);
    int (*port_power)(struct usb_hcd *, int, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct hc_driver {
    const char *description;
    const char *product_desc;
    size_t hcd_priv_size;
    irqreturn_t (*irq)(struct usb_hcd *);
    int flags;
    int (*reset)(struct usb_hcd *);
    int (*start)(struct usb_hcd *);
    int (*pci_suspend)(struct usb_hcd *, bool);
    int (*pci_resume)(struct usb_hcd *, bool);
    void (*stop)(struct usb_hcd *);
    void (*shutdown)(struct usb_hcd *);
    int (*get_frame_number)(struct usb_hcd *);
    int (*urb_enqueue)(struct usb_hcd *, struct urb *, gfp_t);
    int (*urb_dequeue)(struct usb_hcd *, struct urb *, int);
    int (*map_urb_for_dma)(struct usb_hcd *, struct urb *, gfp_t);
    void (*unmap_urb_for_dma)(struct usb_hcd *, struct urb *);
    void (*endpoint_disable)(struct usb_hcd *, struct usb_host_endpoint *);
    void (*endpoint_reset)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*hub_status_data)(struct usb_hcd *, char *);
    int (*hub_control)(struct usb_hcd *, u16, u16, u16, char *, u16);
    int (*bus_suspend)(struct usb_hcd *);
    int (*bus_resume)(struct usb_hcd *);
    int (*start_port_reset)(struct usb_hcd *, unsigned int);
    long unsigned int (*get_resuming_ports)(struct usb_hcd *);
    void (*relinquish_port)(struct usb_hcd *, int);
    int (*port_handed_over)(struct usb_hcd *, int);
    void (*clear_tt_buffer_complete)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*alloc_dev)(struct usb_hcd *, struct usb_device *);
    void (*free_dev)(struct usb_hcd *, struct usb_device *);
    int (*alloc_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, unsigned int, gfp_t);
    int (*free_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, gfp_t);
    int (*add_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*drop_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*check_bandwidth)(struct usb_hcd *, struct usb_device *);
    void (*reset_bandwidth)(struct usb_hcd *, struct usb_device *);
    int (*address_device)(struct usb_hcd *, struct usb_device *);
    int (*enable_device)(struct usb_hcd *, struct usb_device *);
    int (*update_hub_device)(struct usb_hcd *, struct usb_device *, struct usb_tt *, gfp_t);
    int (*reset_device)(struct usb_hcd *, struct usb_device *);
    int (*update_device)(struct usb_hcd *, struct usb_device *);
    int (*set_usb2_hw_lpm)(struct usb_hcd *, struct usb_device *, int);
    int (*enable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*disable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*find_raw_port_number)(struct usb_hcd *, int);
    int (*port_power)(struct usb_hcd *, int, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct hc_driver {
    const char *description;
    const char *product_desc;
    size_t hcd_priv_size;
    irqreturn_t (*irq)(struct usb_hcd *);
    int flags;
    int (*reset)(struct usb_hcd *);
    int (*start)(struct usb_hcd *);
    int (*pci_suspend)(struct usb_hcd *, bool);
    int (*pci_resume)(struct usb_hcd *, bool);
    void (*stop)(struct usb_hcd *);
    void (*shutdown)(struct usb_hcd *);
    int (*get_frame_number)(struct usb_hcd *);
    int (*urb_enqueue)(struct usb_hcd *, struct urb *, gfp_t);
    int (*urb_dequeue)(struct usb_hcd *, struct urb *, int);
    int (*map_urb_for_dma)(struct usb_hcd *, struct urb *, gfp_t);
    void (*unmap_urb_for_dma)(struct usb_hcd *, struct urb *);
    void (*endpoint_disable)(struct usb_hcd *, struct usb_host_endpoint *);
    void (*endpoint_reset)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*hub_status_data)(struct usb_hcd *, char *);
    int (*hub_control)(struct usb_hcd *, u16, u16, u16, char *, u16);
    int (*bus_suspend)(struct usb_hcd *);
    int (*bus_resume)(struct usb_hcd *);
    int (*start_port_reset)(struct usb_hcd *, unsigned int);
    long unsigned int (*get_resuming_ports)(struct usb_hcd *);
    void (*relinquish_port)(struct usb_hcd *, int);
    int (*port_handed_over)(struct usb_hcd *, int);
    void (*clear_tt_buffer_complete)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*alloc_dev)(struct usb_hcd *, struct usb_device *);
    void (*free_dev)(struct usb_hcd *, struct usb_device *);
    int (*alloc_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, unsigned int, gfp_t);
    int (*free_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, gfp_t);
    int (*add_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*drop_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*check_bandwidth)(struct usb_hcd *, struct usb_device *);
    void (*reset_bandwidth)(struct usb_hcd *, struct usb_device *);
    int (*address_device)(struct usb_hcd *, struct usb_device *);
    int (*enable_device)(struct usb_hcd *, struct usb_device *);
    int (*update_hub_device)(struct usb_hcd *, struct usb_device *, struct usb_tt *, gfp_t);
    int (*reset_device)(struct usb_hcd *, struct usb_device *);
    int (*update_device)(struct usb_hcd *, struct usb_device *);
    int (*set_usb2_hw_lpm)(struct usb_hcd *, struct usb_device *, int);
    int (*enable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*disable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*find_raw_port_number)(struct usb_hcd *, int);
    int (*port_power)(struct usb_hcd *, int, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct hc_driver {
    const char *description;
    const char *product_desc;
    size_t hcd_priv_size;
    irqreturn_t (*irq)(struct usb_hcd *);
    int flags;
    int (*reset)(struct usb_hcd *);
    int (*start)(struct usb_hcd *);
    int (*pci_suspend)(struct usb_hcd *, bool);
    int (*pci_resume)(struct usb_hcd *, bool);
    void (*stop)(struct usb_hcd *);
    void (*shutdown)(struct usb_hcd *);
    int (*get_frame_number)(struct usb_hcd *);
    int (*urb_enqueue)(struct usb_hcd *, struct urb *, gfp_t);
    int (*urb_dequeue)(struct usb_hcd *, struct urb *, int);
    int (*map_urb_for_dma)(struct usb_hcd *, struct urb *, gfp_t);
    void (*unmap_urb_for_dma)(struct usb_hcd *, struct urb *);
    void (*endpoint_disable)(struct usb_hcd *, struct usb_host_endpoint *);
    void (*endpoint_reset)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*hub_status_data)(struct usb_hcd *, char *);
    int (*hub_control)(struct usb_hcd *, u16, u16, u16, char *, u16);
    int (*bus_suspend)(struct usb_hcd *);
    int (*bus_resume)(struct usb_hcd *);
    int (*start_port_reset)(struct usb_hcd *, unsigned int);
    long unsigned int (*get_resuming_ports)(struct usb_hcd *);
    void (*relinquish_port)(struct usb_hcd *, int);
    int (*port_handed_over)(struct usb_hcd *, int);
    void (*clear_tt_buffer_complete)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*alloc_dev)(struct usb_hcd *, struct usb_device *);
    void (*free_dev)(struct usb_hcd *, struct usb_device *);
    int (*alloc_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, unsigned int, gfp_t);
    int (*free_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, gfp_t);
    int (*add_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*drop_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*check_bandwidth)(struct usb_hcd *, struct usb_device *);
    void (*reset_bandwidth)(struct usb_hcd *, struct usb_device *);
    int (*address_device)(struct usb_hcd *, struct usb_device *);
    int (*enable_device)(struct usb_hcd *, struct usb_device *);
    int (*update_hub_device)(struct usb_hcd *, struct usb_device *, struct usb_tt *, gfp_t);
    int (*reset_device)(struct usb_hcd *, struct usb_device *);
    int (*update_device)(struct usb_hcd *, struct usb_device *);
    int (*set_usb2_hw_lpm)(struct usb_hcd *, struct usb_device *, int);
    int (*enable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*disable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*find_raw_port_number)(struct usb_hcd *, int);
    int (*port_power)(struct usb_hcd *, int, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct hc_driver {
    const char *description;
    const char *product_desc;
    size_t hcd_priv_size;
    irqreturn_t (*irq)(struct usb_hcd *);
    int flags;
    int (*reset)(struct usb_hcd *);
    int (*start)(struct usb_hcd *);
    int (*pci_suspend)(struct usb_hcd *, bool);
    int (*pci_resume)(struct usb_hcd *, bool);
    void (*stop)(struct usb_hcd *);
    void (*shutdown)(struct usb_hcd *);
    int (*get_frame_number)(struct usb_hcd *);
    int (*urb_enqueue)(struct usb_hcd *, struct urb *, gfp_t);
    int (*urb_dequeue)(struct usb_hcd *, struct urb *, int);
    int (*map_urb_for_dma)(struct usb_hcd *, struct urb *, gfp_t);
    void (*unmap_urb_for_dma)(struct usb_hcd *, struct urb *);
    void (*endpoint_disable)(struct usb_hcd *, struct usb_host_endpoint *);
    void (*endpoint_reset)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*hub_status_data)(struct usb_hcd *, char *);
    int (*hub_control)(struct usb_hcd *, u16, u16, u16, char *, u16);
    int (*bus_suspend)(struct usb_hcd *);
    int (*bus_resume)(struct usb_hcd *);
    int (*start_port_reset)(struct usb_hcd *, unsigned int);
    long unsigned int (*get_resuming_ports)(struct usb_hcd *);
    void (*relinquish_port)(struct usb_hcd *, int);
    int (*port_handed_over)(struct usb_hcd *, int);
    void (*clear_tt_buffer_complete)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*alloc_dev)(struct usb_hcd *, struct usb_device *);
    void (*free_dev)(struct usb_hcd *, struct usb_device *);
    int (*alloc_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, unsigned int, gfp_t);
    int (*free_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, gfp_t);
    int (*add_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*drop_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*check_bandwidth)(struct usb_hcd *, struct usb_device *);
    void (*reset_bandwidth)(struct usb_hcd *, struct usb_device *);
    int (*address_device)(struct usb_hcd *, struct usb_device *);
    int (*enable_device)(struct usb_hcd *, struct usb_device *);
    int (*update_hub_device)(struct usb_hcd *, struct usb_device *, struct usb_tt *, gfp_t);
    int (*reset_device)(struct usb_hcd *, struct usb_device *);
    int (*update_device)(struct usb_hcd *, struct usb_device *);
    int (*set_usb2_hw_lpm)(struct usb_hcd *, struct usb_device *, int);
    int (*enable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*disable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*find_raw_port_number)(struct usb_hcd *, int);
    int (*port_power)(struct usb_hcd *, int, bool);
    int (*submit_single_step_set_feature)(struct usb_hcd *, struct urb *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct hc_driver {
    const char *description;
    const char *product_desc;
    size_t hcd_priv_size;
    irqreturn_t (*irq)(struct usb_hcd *);
    int flags;
    int (*reset)(struct usb_hcd *);
    int (*start)(struct usb_hcd *);
    int (*pci_suspend)(struct usb_hcd *, bool);
    int (*pci_resume)(struct usb_hcd *, bool);
    void (*stop)(struct usb_hcd *);
    void (*shutdown)(struct usb_hcd *);
    int (*get_frame_number)(struct usb_hcd *);
    int (*urb_enqueue)(struct usb_hcd *, struct urb *, gfp_t);
    int (*urb_dequeue)(struct usb_hcd *, struct urb *, int);
    int (*map_urb_for_dma)(struct usb_hcd *, struct urb *, gfp_t);
    void (*unmap_urb_for_dma)(struct usb_hcd *, struct urb *);
    void (*endpoint_disable)(struct usb_hcd *, struct usb_host_endpoint *);
    void (*endpoint_reset)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*hub_status_data)(struct usb_hcd *, char *);
    int (*hub_control)(struct usb_hcd *, u16, u16, u16, char *, u16);
    int (*bus_suspend)(struct usb_hcd *);
    int (*bus_resume)(struct usb_hcd *);
    int (*start_port_reset)(struct usb_hcd *, unsigned int);
    long unsigned int (*get_resuming_ports)(struct usb_hcd *);
    void (*relinquish_port)(struct usb_hcd *, int);
    int (*port_handed_over)(struct usb_hcd *, int);
    void (*clear_tt_buffer_complete)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*alloc_dev)(struct usb_hcd *, struct usb_device *);
    void (*free_dev)(struct usb_hcd *, struct usb_device *);
    int (*alloc_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, unsigned int, gfp_t);
    int (*free_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, gfp_t);
    int (*add_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*drop_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*check_bandwidth)(struct usb_hcd *, struct usb_device *);
    void (*reset_bandwidth)(struct usb_hcd *, struct usb_device *);
    int (*address_device)(struct usb_hcd *, struct usb_device *);
    int (*enable_device)(struct usb_hcd *, struct usb_device *);
    int (*update_hub_device)(struct usb_hcd *, struct usb_device *, struct usb_tt *, gfp_t);
    int (*reset_device)(struct usb_hcd *, struct usb_device *);
    int (*update_device)(struct usb_hcd *, struct usb_device *);
    int (*set_usb2_hw_lpm)(struct usb_hcd *, struct usb_device *, int);
    int (*enable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*disable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*find_raw_port_number)(struct usb_hcd *, int);
    int (*port_power)(struct usb_hcd *, int, bool);
    int (*submit_single_step_set_feature)(struct usb_hcd *, struct urb *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct hc_driver {
    const char *description;
    const char *product_desc;
    size_t hcd_priv_size;
    irqreturn_t (*irq)(struct usb_hcd *);
    int flags;
    int (*reset)(struct usb_hcd *);
    int (*start)(struct usb_hcd *);
    int (*pci_suspend)(struct usb_hcd *, bool);
    int (*pci_resume)(struct usb_hcd *, bool);
    int (*pci_poweroff_late)(struct usb_hcd *, bool);
    void (*stop)(struct usb_hcd *);
    void (*shutdown)(struct usb_hcd *);
    int (*get_frame_number)(struct usb_hcd *);
    int (*urb_enqueue)(struct usb_hcd *, struct urb *, gfp_t);
    int (*urb_dequeue)(struct usb_hcd *, struct urb *, int);
    int (*map_urb_for_dma)(struct usb_hcd *, struct urb *, gfp_t);
    void (*unmap_urb_for_dma)(struct usb_hcd *, struct urb *);
    void (*endpoint_disable)(struct usb_hcd *, struct usb_host_endpoint *);
    void (*endpoint_reset)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*hub_status_data)(struct usb_hcd *, char *);
    int (*hub_control)(struct usb_hcd *, u16, u16, u16, char *, u16);
    int (*bus_suspend)(struct usb_hcd *);
    int (*bus_resume)(struct usb_hcd *);
    int (*start_port_reset)(struct usb_hcd *, unsigned int);
    long unsigned int (*get_resuming_ports)(struct usb_hcd *);
    void (*relinquish_port)(struct usb_hcd *, int);
    int (*port_handed_over)(struct usb_hcd *, int);
    void (*clear_tt_buffer_complete)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*alloc_dev)(struct usb_hcd *, struct usb_device *);
    void (*free_dev)(struct usb_hcd *, struct usb_device *);
    int (*alloc_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, unsigned int, gfp_t);
    int (*free_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, gfp_t);
    int (*add_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*drop_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*check_bandwidth)(struct usb_hcd *, struct usb_device *);
    void (*reset_bandwidth)(struct usb_hcd *, struct usb_device *);
    int (*address_device)(struct usb_hcd *, struct usb_device *);
    int (*enable_device)(struct usb_hcd *, struct usb_device *);
    int (*update_hub_device)(struct usb_hcd *, struct usb_device *, struct usb_tt *, gfp_t);
    int (*reset_device)(struct usb_hcd *, struct usb_device *);
    int (*update_device)(struct usb_hcd *, struct usb_device *);
    int (*set_usb2_hw_lpm)(struct usb_hcd *, struct usb_device *, int);
    int (*enable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*disable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*find_raw_port_number)(struct usb_hcd *, int);
    int (*port_power)(struct usb_hcd *, int, bool);
    int (*submit_single_step_set_feature)(struct usb_hcd *, struct urb *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct hc_driver {
    const char *description;
    const char *product_desc;
    size_t hcd_priv_size;
    irqreturn_t (*irq)(struct usb_hcd *);
    int flags;
    int (*reset)(struct usb_hcd *);
    int (*start)(struct usb_hcd *);
    int (*pci_suspend)(struct usb_hcd *, bool);
    int (*pci_resume)(struct usb_hcd *, pm_message_t);
    int (*pci_poweroff_late)(struct usb_hcd *, bool);
    void (*stop)(struct usb_hcd *);
    void (*shutdown)(struct usb_hcd *);
    int (*get_frame_number)(struct usb_hcd *);
    int (*urb_enqueue)(struct usb_hcd *, struct urb *, gfp_t);
    int (*urb_dequeue)(struct usb_hcd *, struct urb *, int);
    int (*map_urb_for_dma)(struct usb_hcd *, struct urb *, gfp_t);
    void (*unmap_urb_for_dma)(struct usb_hcd *, struct urb *);
    void (*endpoint_disable)(struct usb_hcd *, struct usb_host_endpoint *);
    void (*endpoint_reset)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*hub_status_data)(struct usb_hcd *, char *);
    int (*hub_control)(struct usb_hcd *, u16, u16, u16, char *, u16);
    int (*bus_suspend)(struct usb_hcd *);
    int (*bus_resume)(struct usb_hcd *);
    int (*start_port_reset)(struct usb_hcd *, unsigned int);
    long unsigned int (*get_resuming_ports)(struct usb_hcd *);
    void (*relinquish_port)(struct usb_hcd *, int);
    int (*port_handed_over)(struct usb_hcd *, int);
    void (*clear_tt_buffer_complete)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*alloc_dev)(struct usb_hcd *, struct usb_device *);
    void (*free_dev)(struct usb_hcd *, struct usb_device *);
    int (*alloc_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, unsigned int, gfp_t);
    int (*free_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, gfp_t);
    int (*add_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*drop_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*check_bandwidth)(struct usb_hcd *, struct usb_device *);
    void (*reset_bandwidth)(struct usb_hcd *, struct usb_device *);
    int (*address_device)(struct usb_hcd *, struct usb_device *);
    int (*enable_device)(struct usb_hcd *, struct usb_device *);
    int (*update_hub_device)(struct usb_hcd *, struct usb_device *, struct usb_tt *, gfp_t);
    int (*reset_device)(struct usb_hcd *, struct usb_device *);
    int (*update_device)(struct usb_hcd *, struct usb_device *);
    int (*set_usb2_hw_lpm)(struct usb_hcd *, struct usb_device *, int);
    int (*enable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*disable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*find_raw_port_number)(struct usb_hcd *, int);
    int (*port_power)(struct usb_hcd *, int, bool);
    int (*submit_single_step_set_feature)(struct usb_hcd *, struct urb *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct hc_driver {
    const char *description;
    const char *product_desc;
    size_t hcd_priv_size;
    irqreturn_t (*irq)(struct usb_hcd *);
    int flags;
    int (*reset)(struct usb_hcd *);
    int (*start)(struct usb_hcd *);
    int (*pci_suspend)(struct usb_hcd *, bool);
    int (*pci_resume)(struct usb_hcd *, pm_message_t);
    int (*pci_poweroff_late)(struct usb_hcd *, bool);
    void (*stop)(struct usb_hcd *);
    void (*shutdown)(struct usb_hcd *);
    int (*get_frame_number)(struct usb_hcd *);
    int (*urb_enqueue)(struct usb_hcd *, struct urb *, gfp_t);
    int (*urb_dequeue)(struct usb_hcd *, struct urb *, int);
    int (*map_urb_for_dma)(struct usb_hcd *, struct urb *, gfp_t);
    void (*unmap_urb_for_dma)(struct usb_hcd *, struct urb *);
    void (*endpoint_disable)(struct usb_hcd *, struct usb_host_endpoint *);
    void (*endpoint_reset)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*hub_status_data)(struct usb_hcd *, char *);
    int (*hub_control)(struct usb_hcd *, u16, u16, u16, char *, u16);
    int (*bus_suspend)(struct usb_hcd *);
    int (*bus_resume)(struct usb_hcd *);
    int (*start_port_reset)(struct usb_hcd *, unsigned int);
    long unsigned int (*get_resuming_ports)(struct usb_hcd *);
    void (*relinquish_port)(struct usb_hcd *, int);
    int (*port_handed_over)(struct usb_hcd *, int);
    void (*clear_tt_buffer_complete)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*alloc_dev)(struct usb_hcd *, struct usb_device *);
    void (*free_dev)(struct usb_hcd *, struct usb_device *);
    int (*alloc_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, unsigned int, gfp_t);
    int (*free_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, gfp_t);
    int (*add_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*drop_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*check_bandwidth)(struct usb_hcd *, struct usb_device *);
    void (*reset_bandwidth)(struct usb_hcd *, struct usb_device *);
    int (*address_device)(struct usb_hcd *, struct usb_device *, unsigned int);
    int (*enable_device)(struct usb_hcd *, struct usb_device *);
    int (*update_hub_device)(struct usb_hcd *, struct usb_device *, struct usb_tt *, gfp_t);
    int (*reset_device)(struct usb_hcd *, struct usb_device *);
    int (*update_device)(struct usb_hcd *, struct usb_device *);
    int (*set_usb2_hw_lpm)(struct usb_hcd *, struct usb_device *, int);
    int (*enable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*disable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*find_raw_port_number)(struct usb_hcd *, int);
    int (*port_power)(struct usb_hcd *, int, bool);
    int (*submit_single_step_set_feature)(struct usb_hcd *, struct urb *, int);
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
struct hc_driver {
    const char *description;
    const char *product_desc;
    size_t hcd_priv_size;
    irqreturn_t (*irq)(struct usb_hcd *);
    int flags;
    int (*reset)(struct usb_hcd *);
    int (*start)(struct usb_hcd *);
    int (*pci_suspend)(struct usb_hcd *, bool);
    int (*pci_resume)(struct usb_hcd *, bool);
    void (*stop)(struct usb_hcd *);
    void (*shutdown)(struct usb_hcd *);
    int (*get_frame_number)(struct usb_hcd *);
    int (*urb_enqueue)(struct usb_hcd *, struct urb *, gfp_t);
    int (*urb_dequeue)(struct usb_hcd *, struct urb *, int);
    int (*map_urb_for_dma)(struct usb_hcd *, struct urb *, gfp_t);
    void (*unmap_urb_for_dma)(struct usb_hcd *, struct urb *);
    void (*endpoint_disable)(struct usb_hcd *, struct usb_host_endpoint *);
    void (*endpoint_reset)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*hub_status_data)(struct usb_hcd *, char *);
    int (*hub_control)(struct usb_hcd *, u16, u16, u16, char *, u16);
    int (*bus_suspend)(struct usb_hcd *);
    int (*bus_resume)(struct usb_hcd *);
    int (*start_port_reset)(struct usb_hcd *, unsigned int);
    long unsigned int (*get_resuming_ports)(struct usb_hcd *);
    void (*relinquish_port)(struct usb_hcd *, int);
    int (*port_handed_over)(struct usb_hcd *, int);
    void (*clear_tt_buffer_complete)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*alloc_dev)(struct usb_hcd *, struct usb_device *);
    void (*free_dev)(struct usb_hcd *, struct usb_device *);
    int (*alloc_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, unsigned int, gfp_t);
    int (*free_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, gfp_t);
    int (*add_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*drop_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*check_bandwidth)(struct usb_hcd *, struct usb_device *);
    void (*reset_bandwidth)(struct usb_hcd *, struct usb_device *);
    int (*address_device)(struct usb_hcd *, struct usb_device *);
    int (*enable_device)(struct usb_hcd *, struct usb_device *);
    int (*update_hub_device)(struct usb_hcd *, struct usb_device *, struct usb_tt *, gfp_t);
    int (*reset_device)(struct usb_hcd *, struct usb_device *);
    int (*update_device)(struct usb_hcd *, struct usb_device *);
    int (*set_usb2_hw_lpm)(struct usb_hcd *, struct usb_device *, int);
    int (*enable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*disable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*find_raw_port_number)(struct usb_hcd *, int);
    int (*port_power)(struct usb_hcd *, int, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct hc_driver {
    const char *description;
    const char *product_desc;
    size_t hcd_priv_size;
    irqreturn_t (*irq)(struct usb_hcd *);
    int flags;
    int (*reset)(struct usb_hcd *);
    int (*start)(struct usb_hcd *);
    int (*pci_suspend)(struct usb_hcd *, bool);
    int (*pci_resume)(struct usb_hcd *, bool);
    void (*stop)(struct usb_hcd *);
    void (*shutdown)(struct usb_hcd *);
    int (*get_frame_number)(struct usb_hcd *);
    int (*urb_enqueue)(struct usb_hcd *, struct urb *, gfp_t);
    int (*urb_dequeue)(struct usb_hcd *, struct urb *, int);
    int (*map_urb_for_dma)(struct usb_hcd *, struct urb *, gfp_t);
    void (*unmap_urb_for_dma)(struct usb_hcd *, struct urb *);
    void (*endpoint_disable)(struct usb_hcd *, struct usb_host_endpoint *);
    void (*endpoint_reset)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*hub_status_data)(struct usb_hcd *, char *);
    int (*hub_control)(struct usb_hcd *, u16, u16, u16, char *, u16);
    int (*bus_suspend)(struct usb_hcd *);
    int (*bus_resume)(struct usb_hcd *);
    int (*start_port_reset)(struct usb_hcd *, unsigned int);
    long unsigned int (*get_resuming_ports)(struct usb_hcd *);
    void (*relinquish_port)(struct usb_hcd *, int);
    int (*port_handed_over)(struct usb_hcd *, int);
    void (*clear_tt_buffer_complete)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*alloc_dev)(struct usb_hcd *, struct usb_device *);
    void (*free_dev)(struct usb_hcd *, struct usb_device *);
    int (*alloc_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, unsigned int, gfp_t);
    int (*free_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, gfp_t);
    int (*add_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*drop_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*check_bandwidth)(struct usb_hcd *, struct usb_device *);
    void (*reset_bandwidth)(struct usb_hcd *, struct usb_device *);
    int (*address_device)(struct usb_hcd *, struct usb_device *);
    int (*enable_device)(struct usb_hcd *, struct usb_device *);
    int (*update_hub_device)(struct usb_hcd *, struct usb_device *, struct usb_tt *, gfp_t);
    int (*reset_device)(struct usb_hcd *, struct usb_device *);
    int (*update_device)(struct usb_hcd *, struct usb_device *);
    int (*set_usb2_hw_lpm)(struct usb_hcd *, struct usb_device *, int);
    int (*enable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*disable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*find_raw_port_number)(struct usb_hcd *, int);
    int (*port_power)(struct usb_hcd *, int, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct hc_driver {
    const char *description;
    const char *product_desc;
    size_t hcd_priv_size;
    irqreturn_t (*irq)(struct usb_hcd *);
    int flags;
    int (*reset)(struct usb_hcd *);
    int (*start)(struct usb_hcd *);
    int (*pci_suspend)(struct usb_hcd *, bool);
    int (*pci_resume)(struct usb_hcd *, bool);
    void (*stop)(struct usb_hcd *);
    void (*shutdown)(struct usb_hcd *);
    int (*get_frame_number)(struct usb_hcd *);
    int (*urb_enqueue)(struct usb_hcd *, struct urb *, gfp_t);
    int (*urb_dequeue)(struct usb_hcd *, struct urb *, int);
    int (*map_urb_for_dma)(struct usb_hcd *, struct urb *, gfp_t);
    void (*unmap_urb_for_dma)(struct usb_hcd *, struct urb *);
    void (*endpoint_disable)(struct usb_hcd *, struct usb_host_endpoint *);
    void (*endpoint_reset)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*hub_status_data)(struct usb_hcd *, char *);
    int (*hub_control)(struct usb_hcd *, u16, u16, u16, char *, u16);
    int (*bus_suspend)(struct usb_hcd *);
    int (*bus_resume)(struct usb_hcd *);
    int (*start_port_reset)(struct usb_hcd *, unsigned int);
    long unsigned int (*get_resuming_ports)(struct usb_hcd *);
    void (*relinquish_port)(struct usb_hcd *, int);
    int (*port_handed_over)(struct usb_hcd *, int);
    void (*clear_tt_buffer_complete)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*alloc_dev)(struct usb_hcd *, struct usb_device *);
    void (*free_dev)(struct usb_hcd *, struct usb_device *);
    int (*alloc_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, unsigned int, gfp_t);
    int (*free_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, gfp_t);
    int (*add_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*drop_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*check_bandwidth)(struct usb_hcd *, struct usb_device *);
    void (*reset_bandwidth)(struct usb_hcd *, struct usb_device *);
    int (*address_device)(struct usb_hcd *, struct usb_device *);
    int (*enable_device)(struct usb_hcd *, struct usb_device *);
    int (*update_hub_device)(struct usb_hcd *, struct usb_device *, struct usb_tt *, gfp_t);
    int (*reset_device)(struct usb_hcd *, struct usb_device *);
    int (*update_device)(struct usb_hcd *, struct usb_device *);
    int (*set_usb2_hw_lpm)(struct usb_hcd *, struct usb_device *, int);
    int (*enable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*disable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*find_raw_port_number)(struct usb_hcd *, int);
    int (*port_power)(struct usb_hcd *, int, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct hc_driver {
    const char *description;
    const char *product_desc;
    size_t hcd_priv_size;
    irqreturn_t (*irq)(struct usb_hcd *);
    int flags;
    int (*reset)(struct usb_hcd *);
    int (*start)(struct usb_hcd *);
    int (*pci_suspend)(struct usb_hcd *, bool);
    int (*pci_resume)(struct usb_hcd *, bool);
    void (*stop)(struct usb_hcd *);
    void (*shutdown)(struct usb_hcd *);
    int (*get_frame_number)(struct usb_hcd *);
    int (*urb_enqueue)(struct usb_hcd *, struct urb *, gfp_t);
    int (*urb_dequeue)(struct usb_hcd *, struct urb *, int);
    int (*map_urb_for_dma)(struct usb_hcd *, struct urb *, gfp_t);
    void (*unmap_urb_for_dma)(struct usb_hcd *, struct urb *);
    void (*endpoint_disable)(struct usb_hcd *, struct usb_host_endpoint *);
    void (*endpoint_reset)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*hub_status_data)(struct usb_hcd *, char *);
    int (*hub_control)(struct usb_hcd *, u16, u16, u16, char *, u16);
    int (*bus_suspend)(struct usb_hcd *);
    int (*bus_resume)(struct usb_hcd *);
    int (*start_port_reset)(struct usb_hcd *, unsigned int);
    long unsigned int (*get_resuming_ports)(struct usb_hcd *);
    void (*relinquish_port)(struct usb_hcd *, int);
    int (*port_handed_over)(struct usb_hcd *, int);
    void (*clear_tt_buffer_complete)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*alloc_dev)(struct usb_hcd *, struct usb_device *);
    void (*free_dev)(struct usb_hcd *, struct usb_device *);
    int (*alloc_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, unsigned int, gfp_t);
    int (*free_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, gfp_t);
    int (*add_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*drop_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*check_bandwidth)(struct usb_hcd *, struct usb_device *);
    void (*reset_bandwidth)(struct usb_hcd *, struct usb_device *);
    int (*address_device)(struct usb_hcd *, struct usb_device *);
    int (*enable_device)(struct usb_hcd *, struct usb_device *);
    int (*update_hub_device)(struct usb_hcd *, struct usb_device *, struct usb_tt *, gfp_t);
    int (*reset_device)(struct usb_hcd *, struct usb_device *);
    int (*update_device)(struct usb_hcd *, struct usb_device *);
    int (*set_usb2_hw_lpm)(struct usb_hcd *, struct usb_device *, int);
    int (*enable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*disable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*find_raw_port_number)(struct usb_hcd *, int);
    int (*port_power)(struct usb_hcd *, int, bool);
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
struct hc_driver {
    const char *description;
    const char *product_desc;
    size_t hcd_priv_size;
    irqreturn_t (*irq)(struct usb_hcd *);
    int flags;
    int (*reset)(struct usb_hcd *);
    int (*start)(struct usb_hcd *);
    int (*pci_suspend)(struct usb_hcd *, bool);
    int (*pci_resume)(struct usb_hcd *, bool);
    void (*stop)(struct usb_hcd *);
    void (*shutdown)(struct usb_hcd *);
    int (*get_frame_number)(struct usb_hcd *);
    int (*urb_enqueue)(struct usb_hcd *, struct urb *, gfp_t);
    int (*urb_dequeue)(struct usb_hcd *, struct urb *, int);
    int (*map_urb_for_dma)(struct usb_hcd *, struct urb *, gfp_t);
    void (*unmap_urb_for_dma)(struct usb_hcd *, struct urb *);
    void (*endpoint_disable)(struct usb_hcd *, struct usb_host_endpoint *);
    void (*endpoint_reset)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*hub_status_data)(struct usb_hcd *, char *);
    int (*hub_control)(struct usb_hcd *, u16, u16, u16, char *, u16);
    int (*bus_suspend)(struct usb_hcd *);
    int (*bus_resume)(struct usb_hcd *);
    int (*start_port_reset)(struct usb_hcd *, unsigned int);
    long unsigned int (*get_resuming_ports)(struct usb_hcd *);
    void (*relinquish_port)(struct usb_hcd *, int);
    int (*port_handed_over)(struct usb_hcd *, int);
    void (*clear_tt_buffer_complete)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*alloc_dev)(struct usb_hcd *, struct usb_device *);
    void (*free_dev)(struct usb_hcd *, struct usb_device *);
    int (*alloc_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, unsigned int, gfp_t);
    int (*free_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, gfp_t);
    int (*add_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*drop_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*check_bandwidth)(struct usb_hcd *, struct usb_device *);
    void (*reset_bandwidth)(struct usb_hcd *, struct usb_device *);
    int (*address_device)(struct usb_hcd *, struct usb_device *);
    int (*enable_device)(struct usb_hcd *, struct usb_device *);
    int (*update_hub_device)(struct usb_hcd *, struct usb_device *, struct usb_tt *, gfp_t);
    int (*reset_device)(struct usb_hcd *, struct usb_device *);
    int (*update_device)(struct usb_hcd *, struct usb_device *);
    int (*set_usb2_hw_lpm)(struct usb_hcd *, struct usb_device *, int);
    int (*enable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*disable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*find_raw_port_number)(struct usb_hcd *, int);
    int (*port_power)(struct usb_hcd *, int, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct hc_driver {
    const char *description;
    const char *product_desc;
    size_t hcd_priv_size;
    irqreturn_t (*irq)(struct usb_hcd *);
    int flags;
    int (*reset)(struct usb_hcd *);
    int (*start)(struct usb_hcd *);
    int (*pci_suspend)(struct usb_hcd *, bool);
    int (*pci_resume)(struct usb_hcd *, bool);
    void (*stop)(struct usb_hcd *);
    void (*shutdown)(struct usb_hcd *);
    int (*get_frame_number)(struct usb_hcd *);
    int (*urb_enqueue)(struct usb_hcd *, struct urb *, gfp_t);
    int (*urb_dequeue)(struct usb_hcd *, struct urb *, int);
    int (*map_urb_for_dma)(struct usb_hcd *, struct urb *, gfp_t);
    void (*unmap_urb_for_dma)(struct usb_hcd *, struct urb *);
    void (*endpoint_disable)(struct usb_hcd *, struct usb_host_endpoint *);
    void (*endpoint_reset)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*hub_status_data)(struct usb_hcd *, char *);
    int (*hub_control)(struct usb_hcd *, u16, u16, u16, char *, u16);
    int (*bus_suspend)(struct usb_hcd *);
    int (*bus_resume)(struct usb_hcd *);
    int (*start_port_reset)(struct usb_hcd *, unsigned int);
    long unsigned int (*get_resuming_ports)(struct usb_hcd *);
    void (*relinquish_port)(struct usb_hcd *, int);
    int (*port_handed_over)(struct usb_hcd *, int);
    void (*clear_tt_buffer_complete)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*alloc_dev)(struct usb_hcd *, struct usb_device *);
    void (*free_dev)(struct usb_hcd *, struct usb_device *);
    int (*alloc_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, unsigned int, gfp_t);
    int (*free_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, gfp_t);
    int (*add_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*drop_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*check_bandwidth)(struct usb_hcd *, struct usb_device *);
    void (*reset_bandwidth)(struct usb_hcd *, struct usb_device *);
    int (*address_device)(struct usb_hcd *, struct usb_device *);
    int (*enable_device)(struct usb_hcd *, struct usb_device *);
    int (*update_hub_device)(struct usb_hcd *, struct usb_device *, struct usb_tt *, gfp_t);
    int (*reset_device)(struct usb_hcd *, struct usb_device *);
    int (*update_device)(struct usb_hcd *, struct usb_device *);
    int (*set_usb2_hw_lpm)(struct usb_hcd *, struct usb_device *, int);
    int (*enable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*disable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*find_raw_port_number)(struct usb_hcd *, int);
    int (*port_power)(struct usb_hcd *, int, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct hc_driver {
    const char *description;
    const char *product_desc;
    size_t hcd_priv_size;
    irqreturn_t (*irq)(struct usb_hcd *);
    int flags;
    int (*reset)(struct usb_hcd *);
    int (*start)(struct usb_hcd *);
    int (*pci_suspend)(struct usb_hcd *, bool);
    int (*pci_resume)(struct usb_hcd *, bool);
    void (*stop)(struct usb_hcd *);
    void (*shutdown)(struct usb_hcd *);
    int (*get_frame_number)(struct usb_hcd *);
    int (*urb_enqueue)(struct usb_hcd *, struct urb *, gfp_t);
    int (*urb_dequeue)(struct usb_hcd *, struct urb *, int);
    int (*map_urb_for_dma)(struct usb_hcd *, struct urb *, gfp_t);
    void (*unmap_urb_for_dma)(struct usb_hcd *, struct urb *);
    void (*endpoint_disable)(struct usb_hcd *, struct usb_host_endpoint *);
    void (*endpoint_reset)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*hub_status_data)(struct usb_hcd *, char *);
    int (*hub_control)(struct usb_hcd *, u16, u16, u16, char *, u16);
    int (*bus_suspend)(struct usb_hcd *);
    int (*bus_resume)(struct usb_hcd *);
    int (*start_port_reset)(struct usb_hcd *, unsigned int);
    long unsigned int (*get_resuming_ports)(struct usb_hcd *);
    void (*relinquish_port)(struct usb_hcd *, int);
    int (*port_handed_over)(struct usb_hcd *, int);
    void (*clear_tt_buffer_complete)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*alloc_dev)(struct usb_hcd *, struct usb_device *);
    void (*free_dev)(struct usb_hcd *, struct usb_device *);
    int (*alloc_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, unsigned int, gfp_t);
    int (*free_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, gfp_t);
    int (*add_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*drop_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*check_bandwidth)(struct usb_hcd *, struct usb_device *);
    void (*reset_bandwidth)(struct usb_hcd *, struct usb_device *);
    int (*address_device)(struct usb_hcd *, struct usb_device *);
    int (*enable_device)(struct usb_hcd *, struct usb_device *);
    int (*update_hub_device)(struct usb_hcd *, struct usb_device *, struct usb_tt *, gfp_t);
    int (*reset_device)(struct usb_hcd *, struct usb_device *);
    int (*update_device)(struct usb_hcd *, struct usb_device *);
    int (*set_usb2_hw_lpm)(struct usb_hcd *, struct usb_device *, int);
    int (*enable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*disable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*find_raw_port_number)(struct usb_hcd *, int);
    int (*port_power)(struct usb_hcd *, int, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct hc_driver {
    const char *description;
    const char *product_desc;
    size_t hcd_priv_size;
    irqreturn_t (*irq)(struct usb_hcd *);
    int flags;
    int (*reset)(struct usb_hcd *);
    int (*start)(struct usb_hcd *);
    int (*pci_suspend)(struct usb_hcd *, bool);
    int (*pci_resume)(struct usb_hcd *, bool);
    void (*stop)(struct usb_hcd *);
    void (*shutdown)(struct usb_hcd *);
    int (*get_frame_number)(struct usb_hcd *);
    int (*urb_enqueue)(struct usb_hcd *, struct urb *, gfp_t);
    int (*urb_dequeue)(struct usb_hcd *, struct urb *, int);
    int (*map_urb_for_dma)(struct usb_hcd *, struct urb *, gfp_t);
    void (*unmap_urb_for_dma)(struct usb_hcd *, struct urb *);
    void (*endpoint_disable)(struct usb_hcd *, struct usb_host_endpoint *);
    void (*endpoint_reset)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*hub_status_data)(struct usb_hcd *, char *);
    int (*hub_control)(struct usb_hcd *, u16, u16, u16, char *, u16);
    int (*bus_suspend)(struct usb_hcd *);
    int (*bus_resume)(struct usb_hcd *);
    int (*start_port_reset)(struct usb_hcd *, unsigned int);
    long unsigned int (*get_resuming_ports)(struct usb_hcd *);
    void (*relinquish_port)(struct usb_hcd *, int);
    int (*port_handed_over)(struct usb_hcd *, int);
    void (*clear_tt_buffer_complete)(struct usb_hcd *, struct usb_host_endpoint *);
    int (*alloc_dev)(struct usb_hcd *, struct usb_device *);
    void (*free_dev)(struct usb_hcd *, struct usb_device *);
    int (*alloc_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, unsigned int, gfp_t);
    int (*free_streams)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint **, unsigned int, gfp_t);
    int (*add_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*drop_endpoint)(struct usb_hcd *, struct usb_device *, struct usb_host_endpoint *);
    int (*check_bandwidth)(struct usb_hcd *, struct usb_device *);
    void (*reset_bandwidth)(struct usb_hcd *, struct usb_device *);
    int (*address_device)(struct usb_hcd *, struct usb_device *);
    int (*enable_device)(struct usb_hcd *, struct usb_device *);
    int (*update_hub_device)(struct usb_hcd *, struct usb_device *, struct usb_tt *, gfp_t);
    int (*reset_device)(struct usb_hcd *, struct usb_device *);
    int (*update_device)(struct usb_hcd *, struct usb_device *);
    int (*set_usb2_hw_lpm)(struct usb_hcd *, struct usb_device *, int);
    int (*enable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*disable_usb3_lpm_timeout)(struct usb_hcd *, struct usb_device *, enum usb3_link_state);
    int (*find_raw_port_number)(struct usb_hcd *, int);
    int (*port_power)(struct usb_hcd *, int, bool);
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
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int (*get_resuming_ports)(struct usb_hcd *)</code>
</li>
</ul>
</details>
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
<code>int (*submit_single_step_set_feature)(struct usb_hcd *, struct urb *, int)</code>
</li>
</ul>
</details>
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
<code>int (*pci_poweroff_late)(struct usb_hcd *, bool)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*pci_resume)(struct usb_hcd *, bool)</code> ➡️ <code>int (*pci_resume)(struct usb_hcd *, pm_message_t)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*address_device)(struct usb_hcd *, struct usb_device *)</code> ➡️ <code>int (*address_device)(struct usb_hcd *, struct usb_device *, unsigned int)</code>
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
