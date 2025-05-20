# Struct: <code>acpi_table_spcr</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct acpi_table_spcr {
    struct acpi_table_header header;
    u8 interface_type;
    u8 reserved[3];
    struct acpi_generic_address serial_port;
    u8 interrupt_type;
    u8 pc_interrupt;
    u32 interrupt;
    u8 baud_rate;
    u8 parity;
    u8 stop_bits;
    u8 flow_control;
    u8 terminal_type;
    u8 reserved1;
    u16 pci_device_id;
    u16 pci_vendor_id;
    u8 pci_bus;
    u8 pci_device;
    u8 pci_function;
    u32 pci_flags;
    u8 pci_segment;
    u32 reserved2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct acpi_table_spcr {
    struct acpi_table_header header;
    u8 interface_type;
    u8 reserved[3];
    struct acpi_generic_address serial_port;
    u8 interrupt_type;
    u8 pc_interrupt;
    u32 interrupt;
    u8 baud_rate;
    u8 parity;
    u8 stop_bits;
    u8 flow_control;
    u8 terminal_type;
    u8 reserved1;
    u16 pci_device_id;
    u16 pci_vendor_id;
    u8 pci_bus;
    u8 pci_device;
    u8 pci_function;
    u32 pci_flags;
    u8 pci_segment;
    u32 reserved2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct acpi_table_spcr {
    struct acpi_table_header header;
    u8 interface_type;
    u8 reserved[3];
    struct acpi_generic_address serial_port;
    u8 interrupt_type;
    u8 pc_interrupt;
    u32 interrupt;
    u8 baud_rate;
    u8 parity;
    u8 stop_bits;
    u8 flow_control;
    u8 terminal_type;
    u8 reserved1;
    u16 pci_device_id;
    u16 pci_vendor_id;
    u8 pci_bus;
    u8 pci_device;
    u8 pci_function;
    u32 pci_flags;
    u8 pci_segment;
    u32 reserved2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct acpi_table_spcr {
    struct acpi_table_header header;
    u8 interface_type;
    u8 reserved[3];
    struct acpi_generic_address serial_port;
    u8 interrupt_type;
    u8 pc_interrupt;
    u32 interrupt;
    u8 baud_rate;
    u8 parity;
    u8 stop_bits;
    u8 flow_control;
    u8 terminal_type;
    u8 reserved1;
    u16 pci_device_id;
    u16 pci_vendor_id;
    u8 pci_bus;
    u8 pci_device;
    u8 pci_function;
    u32 pci_flags;
    u8 pci_segment;
    u32 reserved2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct acpi_table_spcr {
    struct acpi_table_header header;
    u8 interface_type;
    u8 reserved[3];
    struct acpi_generic_address serial_port;
    u8 interrupt_type;
    u8 pc_interrupt;
    u32 interrupt;
    u8 baud_rate;
    u8 parity;
    u8 stop_bits;
    u8 flow_control;
    u8 terminal_type;
    u8 reserved1;
    u16 pci_device_id;
    u16 pci_vendor_id;
    u8 pci_bus;
    u8 pci_device;
    u8 pci_function;
    u32 pci_flags;
    u8 pci_segment;
    u32 reserved2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct acpi_table_spcr {
    struct acpi_table_header header;
    u8 interface_type;
    u8 reserved[3];
    struct acpi_generic_address serial_port;
    u8 interrupt_type;
    u8 pc_interrupt;
    u32 interrupt;
    u8 baud_rate;
    u8 parity;
    u8 stop_bits;
    u8 flow_control;
    u8 terminal_type;
    u8 reserved1;
    u16 pci_device_id;
    u16 pci_vendor_id;
    u8 pci_bus;
    u8 pci_device;
    u8 pci_function;
    u32 pci_flags;
    u8 pci_segment;
    u32 reserved2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct acpi_table_spcr {
    struct acpi_table_header header;
    u8 interface_type;
    u8 reserved[3];
    struct acpi_generic_address serial_port;
    u8 interrupt_type;
    u8 pc_interrupt;
    u32 interrupt;
    u8 baud_rate;
    u8 parity;
    u8 stop_bits;
    u8 flow_control;
    u8 terminal_type;
    u8 reserved1;
    u16 pci_device_id;
    u16 pci_vendor_id;
    u8 pci_bus;
    u8 pci_device;
    u8 pci_function;
    u32 pci_flags;
    u8 pci_segment;
    u32 reserved2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct acpi_table_spcr {
    struct acpi_table_header header;
    u8 interface_type;
    u8 reserved[3];
    struct acpi_generic_address serial_port;
    u8 interrupt_type;
    u8 pc_interrupt;
    u32 interrupt;
    u8 baud_rate;
    u8 parity;
    u8 stop_bits;
    u8 flow_control;
    u8 terminal_type;
    u8 reserved1;
    u16 pci_device_id;
    u16 pci_vendor_id;
    u8 pci_bus;
    u8 pci_device;
    u8 pci_function;
    u32 pci_flags;
    u8 pci_segment;
    u32 reserved2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct acpi_table_spcr {
    struct acpi_table_header header;
    u8 interface_type;
    u8 reserved[3];
    struct acpi_generic_address serial_port;
    u8 interrupt_type;
    u8 pc_interrupt;
    u32 interrupt;
    u8 baud_rate;
    u8 parity;
    u8 stop_bits;
    u8 flow_control;
    u8 terminal_type;
    u8 reserved1;
    u16 pci_device_id;
    u16 pci_vendor_id;
    u8 pci_bus;
    u8 pci_device;
    u8 pci_function;
    u32 pci_flags;
    u8 pci_segment;
    u32 reserved2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct acpi_table_spcr {
    struct acpi_table_header header;
    u8 interface_type;
    u8 reserved[3];
    struct acpi_generic_address serial_port;
    u8 interrupt_type;
    u8 pc_interrupt;
    u32 interrupt;
    u8 baud_rate;
    u8 parity;
    u8 stop_bits;
    u8 flow_control;
    u8 terminal_type;
    u8 reserved1;
    u16 pci_device_id;
    u16 pci_vendor_id;
    u8 pci_bus;
    u8 pci_device;
    u8 pci_function;
    u32 pci_flags;
    u8 pci_segment;
    u32 reserved2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct acpi_table_spcr {
    struct acpi_table_header header;
    u8 interface_type;
    u8 reserved[3];
    struct acpi_generic_address serial_port;
    u8 interrupt_type;
    u8 pc_interrupt;
    u32 interrupt;
    u8 baud_rate;
    u8 parity;
    u8 stop_bits;
    u8 flow_control;
    u8 terminal_type;
    u8 reserved1;
    u16 pci_device_id;
    u16 pci_vendor_id;
    u8 pci_bus;
    u8 pci_device;
    u8 pci_function;
    u32 pci_flags;
    u8 pci_segment;
    u32 reserved2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct acpi_table_spcr {
    struct acpi_table_header header;
    u8 interface_type;
    u8 reserved[3];
    struct acpi_generic_address serial_port;
    u8 interrupt_type;
    u8 pc_interrupt;
    u32 interrupt;
    u8 baud_rate;
    u8 parity;
    u8 stop_bits;
    u8 flow_control;
    u8 terminal_type;
    u8 reserved1;
    u16 pci_device_id;
    u16 pci_vendor_id;
    u8 pci_bus;
    u8 pci_device;
    u8 pci_function;
    u32 pci_flags;
    u8 pci_segment;
    u32 reserved2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct acpi_table_spcr {
    struct acpi_table_header header;
    u8 interface_type;
    u8 reserved[3];
    struct acpi_generic_address serial_port;
    u8 interrupt_type;
    u8 pc_interrupt;
    u32 interrupt;
    u8 baud_rate;
    u8 parity;
    u8 stop_bits;
    u8 flow_control;
    u8 terminal_type;
    u8 reserved1;
    u16 pci_device_id;
    u16 pci_vendor_id;
    u8 pci_bus;
    u8 pci_device;
    u8 pci_function;
    u32 pci_flags;
    u8 pci_segment;
    u32 reserved2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct acpi_table_spcr {
    struct acpi_table_header header;
    u8 interface_type;
    u8 reserved[3];
    struct acpi_generic_address serial_port;
    u8 interrupt_type;
    u8 pc_interrupt;
    u32 interrupt;
    u8 baud_rate;
    u8 parity;
    u8 stop_bits;
    u8 flow_control;
    u8 terminal_type;
    u8 reserved1;
    u16 pci_device_id;
    u16 pci_vendor_id;
    u8 pci_bus;
    u8 pci_device;
    u8 pci_function;
    u32 pci_flags;
    u8 pci_segment;
    u32 reserved2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct acpi_table_spcr {
    struct acpi_table_header header;
    u8 interface_type;
    u8 reserved[3];
    struct acpi_generic_address serial_port;
    u8 interrupt_type;
    u8 pc_interrupt;
    u32 interrupt;
    u8 baud_rate;
    u8 parity;
    u8 stop_bits;
    u8 flow_control;
    u8 terminal_type;
    u8 reserved1;
    u16 pci_device_id;
    u16 pci_vendor_id;
    u8 pci_bus;
    u8 pci_device;
    u8 pci_function;
    u32 pci_flags;
    u8 pci_segment;
    u32 reserved2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct acpi_table_spcr {
    struct acpi_table_header header;
    u8 interface_type;
    u8 reserved[3];
    struct acpi_generic_address serial_port;
    u8 interrupt_type;
    u8 pc_interrupt;
    u32 interrupt;
    u8 baud_rate;
    u8 parity;
    u8 stop_bits;
    u8 flow_control;
    u8 terminal_type;
    u8 reserved1;
    u16 pci_device_id;
    u16 pci_vendor_id;
    u8 pci_bus;
    u8 pci_device;
    u8 pci_function;
    u32 pci_flags;
    u8 pci_segment;
    u32 reserved2;
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
struct acpi_table_spcr {
    struct acpi_table_header header;
    u8 interface_type;
    u8 reserved[3];
    struct acpi_generic_address serial_port;
    u8 interrupt_type;
    u8 pc_interrupt;
    u32 interrupt;
    u8 baud_rate;
    u8 parity;
    u8 stop_bits;
    u8 flow_control;
    u8 terminal_type;
    u8 reserved1;
    u16 pci_device_id;
    u16 pci_vendor_id;
    u8 pci_bus;
    u8 pci_device;
    u8 pci_function;
    u32 pci_flags;
    u8 pci_segment;
    u32 reserved2;
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
struct acpi_table_spcr {
    struct acpi_table_header header;
    u8 interface_type;
    u8 reserved[3];
    struct acpi_generic_address serial_port;
    u8 interrupt_type;
    u8 pc_interrupt;
    u32 interrupt;
    u8 baud_rate;
    u8 parity;
    u8 stop_bits;
    u8 flow_control;
    u8 terminal_type;
    u8 reserved1;
    u16 pci_device_id;
    u16 pci_vendor_id;
    u8 pci_bus;
    u8 pci_device;
    u8 pci_function;
    u32 pci_flags;
    u8 pci_segment;
    u32 reserved2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct acpi_table_spcr {
    struct acpi_table_header header;
    u8 interface_type;
    u8 reserved[3];
    struct acpi_generic_address serial_port;
    u8 interrupt_type;
    u8 pc_interrupt;
    u32 interrupt;
    u8 baud_rate;
    u8 parity;
    u8 stop_bits;
    u8 flow_control;
    u8 terminal_type;
    u8 reserved1;
    u16 pci_device_id;
    u16 pci_vendor_id;
    u8 pci_bus;
    u8 pci_device;
    u8 pci_function;
    u32 pci_flags;
    u8 pci_segment;
    u32 reserved2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct acpi_table_spcr {
    struct acpi_table_header header;
    u8 interface_type;
    u8 reserved[3];
    struct acpi_generic_address serial_port;
    u8 interrupt_type;
    u8 pc_interrupt;
    u32 interrupt;
    u8 baud_rate;
    u8 parity;
    u8 stop_bits;
    u8 flow_control;
    u8 terminal_type;
    u8 reserved1;
    u16 pci_device_id;
    u16 pci_vendor_id;
    u8 pci_bus;
    u8 pci_device;
    u8 pci_function;
    u32 pci_flags;
    u8 pci_segment;
    u32 reserved2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct acpi_table_spcr {
    struct acpi_table_header header;
    u8 interface_type;
    u8 reserved[3];
    struct acpi_generic_address serial_port;
    u8 interrupt_type;
    u8 pc_interrupt;
    u32 interrupt;
    u8 baud_rate;
    u8 parity;
    u8 stop_bits;
    u8 flow_control;
    u8 terminal_type;
    u8 reserved1;
    u16 pci_device_id;
    u16 pci_vendor_id;
    u8 pci_bus;
    u8 pci_device;
    u8 pci_function;
    u32 pci_flags;
    u8 pci_segment;
    u32 reserved2;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
