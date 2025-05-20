# Struct: <code>usb_ehci_pdata</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct usb_ehci_pdata {
    int caps_offset;
    unsigned int has_tt;
    unsigned int has_synopsys_hc_bug;
    unsigned int big_endian_desc;
    unsigned int big_endian_mmio;
    unsigned int no_io_watchdog;
    unsigned int reset_on_resume;
    unsigned int dma_mask_64;
    int (*power_on)(struct platform_device *);
    void (*power_off)(struct platform_device *);
    void (*power_suspend)(struct platform_device *);
    int (*pre_setup)(struct usb_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct usb_ehci_pdata {
    int caps_offset;
    unsigned int has_tt;
    unsigned int has_synopsys_hc_bug;
    unsigned int big_endian_desc;
    unsigned int big_endian_mmio;
    unsigned int no_io_watchdog;
    unsigned int reset_on_resume;
    unsigned int dma_mask_64;
    int (*power_on)(struct platform_device *);
    void (*power_off)(struct platform_device *);
    void (*power_suspend)(struct platform_device *);
    int (*pre_setup)(struct usb_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct usb_ehci_pdata {
    int caps_offset;
    unsigned int has_tt;
    unsigned int has_synopsys_hc_bug;
    unsigned int big_endian_desc;
    unsigned int big_endian_mmio;
    unsigned int no_io_watchdog;
    unsigned int reset_on_resume;
    unsigned int dma_mask_64;
    int (*power_on)(struct platform_device *);
    void (*power_off)(struct platform_device *);
    void (*power_suspend)(struct platform_device *);
    int (*pre_setup)(struct usb_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct usb_ehci_pdata {
    int caps_offset;
    unsigned int has_tt;
    unsigned int has_synopsys_hc_bug;
    unsigned int big_endian_desc;
    unsigned int big_endian_mmio;
    unsigned int no_io_watchdog;
    unsigned int reset_on_resume;
    unsigned int dma_mask_64;
    int (*power_on)(struct platform_device *);
    void (*power_off)(struct platform_device *);
    void (*power_suspend)(struct platform_device *);
    int (*pre_setup)(struct usb_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct usb_ehci_pdata {
    int caps_offset;
    unsigned int has_tt;
    unsigned int has_synopsys_hc_bug;
    unsigned int big_endian_desc;
    unsigned int big_endian_mmio;
    unsigned int no_io_watchdog;
    unsigned int reset_on_resume;
    unsigned int dma_mask_64;
    int (*power_on)(struct platform_device *);
    void (*power_off)(struct platform_device *);
    void (*power_suspend)(struct platform_device *);
    int (*pre_setup)(struct usb_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct usb_ehci_pdata {
    int caps_offset;
    unsigned int has_tt;
    unsigned int has_synopsys_hc_bug;
    unsigned int big_endian_desc;
    unsigned int big_endian_mmio;
    unsigned int no_io_watchdog;
    unsigned int reset_on_resume;
    unsigned int dma_mask_64;
    int (*power_on)(struct platform_device *);
    void (*power_off)(struct platform_device *);
    void (*power_suspend)(struct platform_device *);
    int (*pre_setup)(struct usb_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct usb_ehci_pdata {
    int caps_offset;
    unsigned int has_tt;
    unsigned int has_synopsys_hc_bug;
    unsigned int big_endian_desc;
    unsigned int big_endian_mmio;
    unsigned int no_io_watchdog;
    unsigned int reset_on_resume;
    unsigned int dma_mask_64;
    int (*power_on)(struct platform_device *);
    void (*power_off)(struct platform_device *);
    void (*power_suspend)(struct platform_device *);
    int (*pre_setup)(struct usb_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct usb_ehci_pdata {
    int caps_offset;
    unsigned int has_tt;
    unsigned int has_synopsys_hc_bug;
    unsigned int big_endian_desc;
    unsigned int big_endian_mmio;
    unsigned int no_io_watchdog;
    unsigned int reset_on_resume;
    unsigned int dma_mask_64;
    int (*power_on)(struct platform_device *);
    void (*power_off)(struct platform_device *);
    void (*power_suspend)(struct platform_device *);
    int (*pre_setup)(struct usb_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct usb_ehci_pdata {
    int caps_offset;
    unsigned int has_tt;
    unsigned int has_synopsys_hc_bug;
    unsigned int big_endian_desc;
    unsigned int big_endian_mmio;
    unsigned int no_io_watchdog;
    unsigned int reset_on_resume;
    unsigned int dma_mask_64;
    int (*power_on)(struct platform_device *);
    void (*power_off)(struct platform_device *);
    void (*power_suspend)(struct platform_device *);
    int (*pre_setup)(struct usb_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct usb_ehci_pdata {
    int caps_offset;
    unsigned int has_tt;
    unsigned int has_synopsys_hc_bug;
    unsigned int big_endian_desc;
    unsigned int big_endian_mmio;
    unsigned int no_io_watchdog;
    unsigned int reset_on_resume;
    unsigned int dma_mask_64;
    int (*power_on)(struct platform_device *);
    void (*power_off)(struct platform_device *);
    void (*power_suspend)(struct platform_device *);
    int (*pre_setup)(struct usb_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct usb_ehci_pdata {
    int caps_offset;
    unsigned int has_tt;
    unsigned int has_synopsys_hc_bug;
    unsigned int big_endian_desc;
    unsigned int big_endian_mmio;
    unsigned int no_io_watchdog;
    unsigned int reset_on_resume;
    unsigned int dma_mask_64;
    int (*power_on)(struct platform_device *);
    void (*power_off)(struct platform_device *);
    void (*power_suspend)(struct platform_device *);
    int (*pre_setup)(struct usb_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct usb_ehci_pdata {
    int caps_offset;
    unsigned int has_tt;
    unsigned int has_synopsys_hc_bug;
    unsigned int big_endian_desc;
    unsigned int big_endian_mmio;
    unsigned int no_io_watchdog;
    unsigned int reset_on_resume;
    unsigned int dma_mask_64;
    unsigned int spurious_oc;
    int (*power_on)(struct platform_device *);
    void (*power_off)(struct platform_device *);
    void (*power_suspend)(struct platform_device *);
    int (*pre_setup)(struct usb_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct usb_ehci_pdata {
    int caps_offset;
    unsigned int has_tt;
    unsigned int has_synopsys_hc_bug;
    unsigned int big_endian_desc;
    unsigned int big_endian_mmio;
    unsigned int no_io_watchdog;
    unsigned int reset_on_resume;
    unsigned int dma_mask_64;
    unsigned int spurious_oc;
    int (*power_on)(struct platform_device *);
    void (*power_off)(struct platform_device *);
    void (*power_suspend)(struct platform_device *);
    int (*pre_setup)(struct usb_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct usb_ehci_pdata {
    int caps_offset;
    unsigned int has_tt;
    unsigned int has_synopsys_hc_bug;
    unsigned int big_endian_desc;
    unsigned int big_endian_mmio;
    unsigned int no_io_watchdog;
    unsigned int reset_on_resume;
    unsigned int dma_mask_64;
    unsigned int spurious_oc;
    int (*power_on)(struct platform_device *);
    void (*power_off)(struct platform_device *);
    void (*power_suspend)(struct platform_device *);
    int (*pre_setup)(struct usb_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct usb_ehci_pdata {
    int caps_offset;
    unsigned int has_tt;
    unsigned int has_synopsys_hc_bug;
    unsigned int big_endian_desc;
    unsigned int big_endian_mmio;
    unsigned int no_io_watchdog;
    unsigned int reset_on_resume;
    unsigned int dma_mask_64;
    unsigned int spurious_oc;
    int (*power_on)(struct platform_device *);
    void (*power_off)(struct platform_device *);
    void (*power_suspend)(struct platform_device *);
    int (*pre_setup)(struct usb_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct usb_ehci_pdata {
    int caps_offset;
    unsigned int has_tt;
    unsigned int has_synopsys_hc_bug;
    unsigned int big_endian_desc;
    unsigned int big_endian_mmio;
    unsigned int no_io_watchdog;
    unsigned int reset_on_resume;
    unsigned int dma_mask_64;
    unsigned int spurious_oc;
    int (*power_on)(struct platform_device *);
    void (*power_off)(struct platform_device *);
    void (*power_suspend)(struct platform_device *);
    int (*pre_setup)(struct usb_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct usb_ehci_pdata {
    int caps_offset;
    unsigned int has_tt;
    unsigned int has_synopsys_hc_bug;
    unsigned int big_endian_desc;
    unsigned int big_endian_mmio;
    unsigned int no_io_watchdog;
    unsigned int reset_on_resume;
    unsigned int dma_mask_64;
    unsigned int spurious_oc;
    int (*power_on)(struct platform_device *);
    void (*power_off)(struct platform_device *);
    void (*power_suspend)(struct platform_device *);
    int (*pre_setup)(struct usb_hcd *);
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
In <code>arm64</code>: Absent ⚠️
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
struct usb_ehci_pdata {
    int caps_offset;
    unsigned int has_tt;
    unsigned int has_synopsys_hc_bug;
    unsigned int big_endian_desc;
    unsigned int big_endian_mmio;
    unsigned int no_io_watchdog;
    unsigned int reset_on_resume;
    unsigned int dma_mask_64;
    int (*power_on)(struct platform_device *);
    void (*power_off)(struct platform_device *);
    void (*power_suspend)(struct platform_device *);
    int (*pre_setup)(struct usb_hcd *);
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
struct usb_ehci_pdata {
    int caps_offset;
    unsigned int has_tt;
    unsigned int has_synopsys_hc_bug;
    unsigned int big_endian_desc;
    unsigned int big_endian_mmio;
    unsigned int no_io_watchdog;
    unsigned int reset_on_resume;
    unsigned int dma_mask_64;
    int (*power_on)(struct platform_device *);
    void (*power_off)(struct platform_device *);
    void (*power_suspend)(struct platform_device *);
    int (*pre_setup)(struct usb_hcd *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct usb_ehci_pdata {
    int caps_offset;
    unsigned int has_tt;
    unsigned int has_synopsys_hc_bug;
    unsigned int big_endian_desc;
    unsigned int big_endian_mmio;
    unsigned int no_io_watchdog;
    unsigned int reset_on_resume;
    unsigned int dma_mask_64;
    int (*power_on)(struct platform_device *);
    void (*power_off)(struct platform_device *);
    void (*power_suspend)(struct platform_device *);
    int (*pre_setup)(struct usb_hcd *);
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
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int spurious_oc</code>
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
