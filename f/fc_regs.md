# Struct: <code>fc_regs</code>

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
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
In <code>5.19</code>: Absent ⚠️
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
</li>
</ul>
<b>Arch</b>
<ul>
<li>
In <code>arm64</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct fc_regs {
    u32 USB_CONTROL;
    u32 USB_STATUS;
    u32 USB_ADDRESS;
    u32 UTMI_CHARACTER_1;
    u32 TEST_CONTROL;
    u32 reserved_14;
    u32 SETUP_DATA0;
    u32 SETUP_DATA1;
    u32 USB_INT_STA;
    u32 USB_INT_ENA;
    u32 EP0_CONTROL;
    u32 EP0_STATUS;
    u32 EP0_INT_ENA;
    u32 EP0_LENGTH;
    u32 EP0_READ;
    u32 EP0_WRITE;
    struct ep_regs EP_REGS[15];
    u8 reserved_220[3552];
    u32 AHBSCTR;
    u32 AHBMCTR;
    u32 AHBBINT;
    u32 AHBBINTEN;
    u32 EPCTR;
    u32 USBF_EPTEST;
    u8 reserved_1018[8];
    u32 USBSSVER;
    u32 USBSSCONF;
    u8 reserved_1028[232];
    struct ep_dcr EP_DCR[15];
    u8 reserved_1200[3584];
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
<b>Arch</b>
<ul>
</ul>
