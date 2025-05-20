# Struct: <code>ehci_regs</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct ehci_regs {
    u32 command;
    u32 status;
    u32 intr_enable;
    u32 frame_index;
    u32 segment;
    u32 frame_list;
    u32 async_next;
    u32 reserved1[2];
    u32 txfill_tuning;
    u32 reserved2[6];
    u32 configured_flag;
    u32 port_status[0];
    u32 reserved3[9];
    u32 usbmode;
    u32 reserved4[6];
    u32 hostpc[1];
    u32 reserved5[16];
    u32 usbmode_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ehci_regs {
    u32 command;
    u32 status;
    u32 intr_enable;
    u32 frame_index;
    u32 segment;
    u32 frame_list;
    u32 async_next;
    u32 reserved1[2];
    u32 txfill_tuning;
    u32 reserved2[6];
    u32 configured_flag;
    u32 port_status[0];
    u32 reserved3[9];
    u32 usbmode;
    u32 reserved4[6];
    u32 hostpc[0];
    u32 reserved5[17];
    u32 usbmode_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ehci_regs {
    u32 command;
    u32 status;
    u32 intr_enable;
    u32 frame_index;
    u32 segment;
    u32 frame_list;
    u32 async_next;
    u32 reserved1[2];
    u32 txfill_tuning;
    u32 reserved2[6];
    u32 configured_flag;
    u32 port_status[0];
    u32 reserved3[9];
    u32 usbmode;
    u32 reserved4[6];
    u32 hostpc[0];
    u32 reserved5[17];
    u32 usbmode_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ehci_regs {
    u32 command;
    u32 status;
    u32 intr_enable;
    u32 frame_index;
    u32 segment;
    u32 frame_list;
    u32 async_next;
    u32 reserved1[2];
    u32 txfill_tuning;
    u32 reserved2[6];
    u32 configured_flag;
    u32 port_status[0];
    u32 reserved3[9];
    u32 usbmode;
    u32 reserved4[6];
    u32 hostpc[0];
    u32 reserved5[17];
    u32 usbmode_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ehci_regs {
    u32 command;
    u32 status;
    u32 intr_enable;
    u32 frame_index;
    u32 segment;
    u32 frame_list;
    u32 async_next;
    u32 reserved1[2];
    u32 txfill_tuning;
    u32 reserved2[6];
    u32 configured_flag;
    u32 port_status[0];
    u32 reserved3[9];
    u32 usbmode;
    u32 reserved4[6];
    u32 hostpc[0];
    u32 reserved5[17];
    u32 usbmode_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ehci_regs {
    u32 command;
    u32 status;
    u32 intr_enable;
    u32 frame_index;
    u32 segment;
    u32 frame_list;
    u32 async_next;
    u32 reserved1[2];
    u32 txfill_tuning;
    u32 reserved2[6];
    u32 configured_flag;
    u32 port_status[0];
    u32 reserved3[9];
    u32 usbmode;
    u32 reserved4[6];
    u32 hostpc[0];
    u32 reserved5[17];
    u32 usbmode_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ehci_regs {
    u32 command;
    u32 status;
    u32 intr_enable;
    u32 frame_index;
    u32 segment;
    u32 frame_list;
    u32 async_next;
    u32 reserved1[2];
    u32 txfill_tuning;
    u32 reserved2[6];
    u32 configured_flag;
    u32 port_status[0];
    u32 reserved3[9];
    u32 usbmode;
    u32 reserved4[6];
    u32 hostpc[0];
    u32 reserved5[17];
    u32 usbmode_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ehci_regs {
    u32 command;
    u32 status;
    u32 intr_enable;
    u32 frame_index;
    u32 segment;
    u32 frame_list;
    u32 async_next;
    u32 reserved1[2];
    u32 txfill_tuning;
    u32 reserved2[6];
    u32 configured_flag;
    u32 port_status[0];
    u32 reserved3[9];
    u32 usbmode;
    u32 reserved4[6];
    u32 hostpc[0];
    u32 reserved5[17];
    u32 usbmode_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ehci_regs {
    u32 command;
    u32 status;
    u32 intr_enable;
    u32 frame_index;
    u32 segment;
    u32 frame_list;
    u32 async_next;
    u32 reserved1[2];
    u32 txfill_tuning;
    u32 reserved2[6];
    u32 configured_flag;
    u32 port_status[0];
    u32 reserved3[9];
    u32 usbmode;
    u32 reserved4[6];
    u32 hostpc[0];
    u32 reserved5[17];
    u32 usbmode_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ehci_regs {
    u32 command;
    u32 status;
    u32 intr_enable;
    u32 frame_index;
    u32 segment;
    u32 frame_list;
    u32 async_next;
    u32 reserved1[2];
    u32 txfill_tuning;
    u32 reserved2[6];
    u32 configured_flag;
    u32 port_status[0];
    u32 reserved3[9];
    u32 usbmode;
    u32 reserved4[6];
    u32 hostpc[0];
    u32 reserved5[17];
    u32 usbmode_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ehci_regs {
    u32 command;
    u32 status;
    u32 intr_enable;
    u32 frame_index;
    u32 segment;
    u32 frame_list;
    u32 async_next;
    u32 reserved1[2];
    u32 txfill_tuning;
    u32 reserved2[6];
    u32 configured_flag;
    u32 port_status[0];
    u32 reserved3[9];
    u32 usbmode;
    u32 reserved4[6];
    u32 hostpc[0];
    u32 reserved5[17];
    u32 usbmode_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ehci_regs {
    u32 command;
    u32 status;
    u32 intr_enable;
    u32 frame_index;
    u32 segment;
    u32 frame_list;
    u32 async_next;
    u32 reserved1[2];
    u32 txfill_tuning;
    u32 reserved2[6];
    u32 configured_flag;
    u32 port_status[0];
    u32 reserved3[9];
    u32 usbmode;
    u32 reserved4[6];
    u32 hostpc[0];
    u32 reserved5[17];
    u32 usbmode_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ehci_regs {
    u32 command;
    u32 status;
    u32 intr_enable;
    u32 frame_index;
    u32 segment;
    u32 frame_list;
    u32 async_next;
    u32 reserved1[2];
    u32 txfill_tuning;
    u32 reserved2[6];
    u32 configured_flag;
    u32 port_status[15];
    u32 reserved3[9];
    u32 usbmode;
    u32 reserved4;
    u32 hostpc[15];
    u32 brcm_insnreg[4];
    u32 reserved5[2];
    u32 usbmode_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ehci_regs {
    u32 command;
    u32 status;
    u32 intr_enable;
    u32 frame_index;
    u32 segment;
    u32 frame_list;
    u32 async_next;
    u32 reserved1[2];
    u32 txfill_tuning;
    u32 reserved2[6];
    u32 configured_flag;
    u32 port_status[15];
    u32 reserved3[9];
    u32 usbmode;
    u32 reserved4;
    u32 hostpc[15];
    u32 brcm_insnreg[4];
    u32 reserved5[2];
    u32 usbmode_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ehci_regs {
    u32 command;
    u32 status;
    u32 intr_enable;
    u32 frame_index;
    u32 segment;
    u32 frame_list;
    u32 async_next;
    u32 reserved1[2];
    u32 txfill_tuning;
    u32 reserved2[6];
    u32 configured_flag;
    u32 port_status[15];
    u32 reserved3[9];
    u32 usbmode;
    u32 reserved4;
    u32 hostpc[15];
    u32 brcm_insnreg[4];
    u32 reserved5[2];
    u32 usbmode_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ehci_regs {
    u32 command;
    u32 status;
    u32 intr_enable;
    u32 frame_index;
    u32 segment;
    u32 frame_list;
    u32 async_next;
    u32 reserved1[2];
    u32 txfill_tuning;
    u32 reserved2[6];
    u32 configured_flag;
    u32 port_status[15];
    u32 reserved3[9];
    u32 usbmode;
    u32 reserved4;
    u32 hostpc[15];
    u32 brcm_insnreg[4];
    u32 reserved5[2];
    u32 usbmode_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ehci_regs {
    u32 command;
    u32 status;
    u32 intr_enable;
    u32 frame_index;
    u32 segment;
    u32 frame_list;
    u32 async_next;
    u32 reserved1[2];
    u32 txfill_tuning;
    u32 reserved2[6];
    u32 configured_flag;
    u32 port_status[15];
    u32 reserved3[9];
    u32 usbmode;
    u32 reserved4;
    u32 hostpc[15];
    u32 brcm_insnreg[4];
    u32 reserved5[2];
    u32 usbmode_ex;
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
struct ehci_regs {
    u32 command;
    u32 status;
    u32 intr_enable;
    u32 frame_index;
    u32 segment;
    u32 frame_list;
    u32 async_next;
    u32 reserved1[2];
    u32 txfill_tuning;
    u32 reserved2[6];
    u32 configured_flag;
    u32 port_status[0];
    u32 reserved3[9];
    u32 usbmode;
    u32 reserved4[6];
    u32 hostpc[0];
    u32 reserved5[17];
    u32 usbmode_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ehci_regs {
    u32 command;
    u32 status;
    u32 intr_enable;
    u32 frame_index;
    u32 segment;
    u32 frame_list;
    u32 async_next;
    u32 reserved1[2];
    u32 txfill_tuning;
    u32 reserved2[6];
    u32 configured_flag;
    u32 port_status[0];
    u32 reserved3[9];
    u32 usbmode;
    u32 reserved4[6];
    u32 hostpc[0];
    u32 reserved5[17];
    u32 usbmode_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ehci_regs {
    u32 command;
    u32 status;
    u32 intr_enable;
    u32 frame_index;
    u32 segment;
    u32 frame_list;
    u32 async_next;
    u32 reserved1[2];
    u32 txfill_tuning;
    u32 reserved2[6];
    u32 configured_flag;
    u32 port_status[0];
    u32 reserved3[9];
    u32 usbmode;
    u32 reserved4[6];
    u32 hostpc[0];
    u32 reserved5[17];
    u32 usbmode_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ehci_regs {
    u32 command;
    u32 status;
    u32 intr_enable;
    u32 frame_index;
    u32 segment;
    u32 frame_list;
    u32 async_next;
    u32 reserved1[2];
    u32 txfill_tuning;
    u32 reserved2[6];
    u32 configured_flag;
    u32 port_status[0];
    u32 reserved3[9];
    u32 usbmode;
    u32 reserved4[6];
    u32 hostpc[0];
    u32 reserved5[17];
    u32 usbmode_ex;
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
struct ehci_regs {
    u32 command;
    u32 status;
    u32 intr_enable;
    u32 frame_index;
    u32 segment;
    u32 frame_list;
    u32 async_next;
    u32 reserved1[2];
    u32 txfill_tuning;
    u32 reserved2[6];
    u32 configured_flag;
    u32 port_status[0];
    u32 reserved3[9];
    u32 usbmode;
    u32 reserved4[6];
    u32 hostpc[0];
    u32 reserved5[17];
    u32 usbmode_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ehci_regs {
    u32 command;
    u32 status;
    u32 intr_enable;
    u32 frame_index;
    u32 segment;
    u32 frame_list;
    u32 async_next;
    u32 reserved1[2];
    u32 txfill_tuning;
    u32 reserved2[6];
    u32 configured_flag;
    u32 port_status[0];
    u32 reserved3[9];
    u32 usbmode;
    u32 reserved4[6];
    u32 hostpc[0];
    u32 reserved5[17];
    u32 usbmode_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ehci_regs {
    u32 command;
    u32 status;
    u32 intr_enable;
    u32 frame_index;
    u32 segment;
    u32 frame_list;
    u32 async_next;
    u32 reserved1[2];
    u32 txfill_tuning;
    u32 reserved2[6];
    u32 configured_flag;
    u32 port_status[0];
    u32 reserved3[9];
    u32 usbmode;
    u32 reserved4[6];
    u32 hostpc[0];
    u32 reserved5[17];
    u32 usbmode_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ehci_regs {
    u32 command;
    u32 status;
    u32 intr_enable;
    u32 frame_index;
    u32 segment;
    u32 frame_list;
    u32 async_next;
    u32 reserved1[2];
    u32 txfill_tuning;
    u32 reserved2[6];
    u32 configured_flag;
    u32 port_status[0];
    u32 reserved3[9];
    u32 usbmode;
    u32 reserved4[6];
    u32 hostpc[0];
    u32 reserved5[17];
    u32 usbmode_ex;
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
<b>Field type changed. </b>
<code>u32 hostpc[1]</code> ➡️ <code>u32 hostpc[0]</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 reserved5[16]</code> ➡️ <code>u32 reserved5[17]</code>
</li>
</ul>
</details>
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
<code>u32 brcm_insnreg[4]</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 port_status[0]</code> ➡️ <code>u32 port_status[15]</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 reserved4[6]</code> ➡️ <code>u32 reserved4</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 hostpc[0]</code> ➡️ <code>u32 hostpc[15]</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 reserved5[17]</code> ➡️ <code>u32 reserved5[2]</code>
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
