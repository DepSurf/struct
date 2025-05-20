# Struct: <code>acpi_madt_generic_interrupt</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct acpi_madt_generic_interrupt {
    struct acpi_subtable_header header;
    u16 reserved;
    u32 cpu_interface_number;
    u32 uid;
    u32 flags;
    u32 parking_version;
    u32 performance_interrupt;
    u64 parked_address;
    u64 base_address;
    u64 gicv_base_address;
    u64 gich_base_address;
    u32 vgic_interrupt;
    u64 gicr_base_address;
    u64 arm_mpidr;
    u8 efficiency_class;
    u8 reserved2[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct acpi_madt_generic_interrupt {
    struct acpi_subtable_header header;
    u16 reserved;
    u32 cpu_interface_number;
    u32 uid;
    u32 flags;
    u32 parking_version;
    u32 performance_interrupt;
    u64 parked_address;
    u64 base_address;
    u64 gicv_base_address;
    u64 gich_base_address;
    u32 vgic_interrupt;
    u64 gicr_base_address;
    u64 arm_mpidr;
    u8 efficiency_class;
    u8 reserved2[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct acpi_madt_generic_interrupt {
    struct acpi_subtable_header header;
    u16 reserved;
    u32 cpu_interface_number;
    u32 uid;
    u32 flags;
    u32 parking_version;
    u32 performance_interrupt;
    u64 parked_address;
    u64 base_address;
    u64 gicv_base_address;
    u64 gich_base_address;
    u32 vgic_interrupt;
    u64 gicr_base_address;
    u64 arm_mpidr;
    u8 efficiency_class;
    u8 reserved2[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct acpi_madt_generic_interrupt {
    struct acpi_subtable_header header;
    u16 reserved;
    u32 cpu_interface_number;
    u32 uid;
    u32 flags;
    u32 parking_version;
    u32 performance_interrupt;
    u64 parked_address;
    u64 base_address;
    u64 gicv_base_address;
    u64 gich_base_address;
    u32 vgic_interrupt;
    u64 gicr_base_address;
    u64 arm_mpidr;
    u8 efficiency_class;
    u8 reserved2[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct acpi_madt_generic_interrupt {
    struct acpi_subtable_header header;
    u16 reserved;
    u32 cpu_interface_number;
    u32 uid;
    u32 flags;
    u32 parking_version;
    u32 performance_interrupt;
    u64 parked_address;
    u64 base_address;
    u64 gicv_base_address;
    u64 gich_base_address;
    u32 vgic_interrupt;
    u64 gicr_base_address;
    u64 arm_mpidr;
    u8 efficiency_class;
    u8 reserved2[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct acpi_madt_generic_interrupt {
    struct acpi_subtable_header header;
    u16 reserved;
    u32 cpu_interface_number;
    u32 uid;
    u32 flags;
    u32 parking_version;
    u32 performance_interrupt;
    u64 parked_address;
    u64 base_address;
    u64 gicv_base_address;
    u64 gich_base_address;
    u32 vgic_interrupt;
    u64 gicr_base_address;
    u64 arm_mpidr;
    u8 efficiency_class;
    u8 reserved2[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct acpi_madt_generic_interrupt {
    struct acpi_subtable_header header;
    u16 reserved;
    u32 cpu_interface_number;
    u32 uid;
    u32 flags;
    u32 parking_version;
    u32 performance_interrupt;
    u64 parked_address;
    u64 base_address;
    u64 gicv_base_address;
    u64 gich_base_address;
    u32 vgic_interrupt;
    u64 gicr_base_address;
    u64 arm_mpidr;
    u8 efficiency_class;
    u8 reserved2[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct acpi_madt_generic_interrupt {
    struct acpi_subtable_header header;
    u16 reserved;
    u32 cpu_interface_number;
    u32 uid;
    u32 flags;
    u32 parking_version;
    u32 performance_interrupt;
    u64 parked_address;
    u64 base_address;
    u64 gicv_base_address;
    u64 gich_base_address;
    u32 vgic_interrupt;
    u64 gicr_base_address;
    u64 arm_mpidr;
    u8 efficiency_class;
    u8 reserved2[1];
    u16 spe_interrupt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct acpi_madt_generic_interrupt {
    struct acpi_subtable_header header;
    u16 reserved;
    u32 cpu_interface_number;
    u32 uid;
    u32 flags;
    u32 parking_version;
    u32 performance_interrupt;
    u64 parked_address;
    u64 base_address;
    u64 gicv_base_address;
    u64 gich_base_address;
    u32 vgic_interrupt;
    u64 gicr_base_address;
    u64 arm_mpidr;
    u8 efficiency_class;
    u8 reserved2[1];
    u16 spe_interrupt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct acpi_madt_generic_interrupt {
    struct acpi_subtable_header header;
    u16 reserved;
    u32 cpu_interface_number;
    u32 uid;
    u32 flags;
    u32 parking_version;
    u32 performance_interrupt;
    u64 parked_address;
    u64 base_address;
    u64 gicv_base_address;
    u64 gich_base_address;
    u32 vgic_interrupt;
    u64 gicr_base_address;
    u64 arm_mpidr;
    u8 efficiency_class;
    u8 reserved2[1];
    u16 spe_interrupt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct acpi_madt_generic_interrupt {
    struct acpi_subtable_header header;
    u16 reserved;
    u32 cpu_interface_number;
    u32 uid;
    u32 flags;
    u32 parking_version;
    u32 performance_interrupt;
    u64 parked_address;
    u64 base_address;
    u64 gicv_base_address;
    u64 gich_base_address;
    u32 vgic_interrupt;
    u64 gicr_base_address;
    u64 arm_mpidr;
    u8 efficiency_class;
    u8 reserved2[1];
    u16 spe_interrupt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct acpi_madt_generic_interrupt {
    struct acpi_subtable_header header;
    u16 reserved;
    u32 cpu_interface_number;
    u32 uid;
    u32 flags;
    u32 parking_version;
    u32 performance_interrupt;
    u64 parked_address;
    u64 base_address;
    u64 gicv_base_address;
    u64 gich_base_address;
    u32 vgic_interrupt;
    u64 gicr_base_address;
    u64 arm_mpidr;
    u8 efficiency_class;
    u8 reserved2[1];
    u16 spe_interrupt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct acpi_madt_generic_interrupt {
    struct acpi_subtable_header header;
    u16 reserved;
    u32 cpu_interface_number;
    u32 uid;
    u32 flags;
    u32 parking_version;
    u32 performance_interrupt;
    u64 parked_address;
    u64 base_address;
    u64 gicv_base_address;
    u64 gich_base_address;
    u32 vgic_interrupt;
    u64 gicr_base_address;
    u64 arm_mpidr;
    u8 efficiency_class;
    u8 reserved2[1];
    u16 spe_interrupt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct acpi_madt_generic_interrupt {
    struct acpi_subtable_header header;
    u16 reserved;
    u32 cpu_interface_number;
    u32 uid;
    u32 flags;
    u32 parking_version;
    u32 performance_interrupt;
    u64 parked_address;
    u64 base_address;
    u64 gicv_base_address;
    u64 gich_base_address;
    u32 vgic_interrupt;
    u64 gicr_base_address;
    u64 arm_mpidr;
    u8 efficiency_class;
    u8 reserved2[1];
    u16 spe_interrupt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct acpi_madt_generic_interrupt {
    struct acpi_subtable_header header;
    u16 reserved;
    u32 cpu_interface_number;
    u32 uid;
    u32 flags;
    u32 parking_version;
    u32 performance_interrupt;
    u64 parked_address;
    u64 base_address;
    u64 gicv_base_address;
    u64 gich_base_address;
    u32 vgic_interrupt;
    u64 gicr_base_address;
    u64 arm_mpidr;
    u8 efficiency_class;
    u8 reserved2[1];
    u16 spe_interrupt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct acpi_madt_generic_interrupt {
    struct acpi_subtable_header header;
    u16 reserved;
    u32 cpu_interface_number;
    u32 uid;
    u32 flags;
    u32 parking_version;
    u32 performance_interrupt;
    u64 parked_address;
    u64 base_address;
    u64 gicv_base_address;
    u64 gich_base_address;
    u32 vgic_interrupt;
    u64 gicr_base_address;
    u64 arm_mpidr;
    u8 efficiency_class;
    u8 reserved2[1];
    u16 spe_interrupt;
    u16 trbe_interrupt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct acpi_madt_generic_interrupt {
    struct acpi_subtable_header header;
    u16 reserved;
    u32 cpu_interface_number;
    u32 uid;
    u32 flags;
    u32 parking_version;
    u32 performance_interrupt;
    u64 parked_address;
    u64 base_address;
    u64 gicv_base_address;
    u64 gich_base_address;
    u32 vgic_interrupt;
    u64 gicr_base_address;
    u64 arm_mpidr;
    u8 efficiency_class;
    u8 reserved2[1];
    u16 spe_interrupt;
    u16 trbe_interrupt;
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
struct acpi_madt_generic_interrupt {
    struct acpi_subtable_header header;
    u16 reserved;
    u32 cpu_interface_number;
    u32 uid;
    u32 flags;
    u32 parking_version;
    u32 performance_interrupt;
    u64 parked_address;
    u64 base_address;
    u64 gicv_base_address;
    u64 gich_base_address;
    u32 vgic_interrupt;
    u64 gicr_base_address;
    u64 arm_mpidr;
    u8 efficiency_class;
    u8 reserved2[1];
    u16 spe_interrupt;
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
struct acpi_madt_generic_interrupt {
    struct acpi_subtable_header header;
    u16 reserved;
    u32 cpu_interface_number;
    u32 uid;
    u32 flags;
    u32 parking_version;
    u32 performance_interrupt;
    u64 parked_address;
    u64 base_address;
    u64 gicv_base_address;
    u64 gich_base_address;
    u32 vgic_interrupt;
    u64 gicr_base_address;
    u64 arm_mpidr;
    u8 efficiency_class;
    u8 reserved2[1];
    u16 spe_interrupt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct acpi_madt_generic_interrupt {
    struct acpi_subtable_header header;
    u16 reserved;
    u32 cpu_interface_number;
    u32 uid;
    u32 flags;
    u32 parking_version;
    u32 performance_interrupt;
    u64 parked_address;
    u64 base_address;
    u64 gicv_base_address;
    u64 gich_base_address;
    u32 vgic_interrupt;
    u64 gicr_base_address;
    u64 arm_mpidr;
    u8 efficiency_class;
    u8 reserved2[1];
    u16 spe_interrupt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct acpi_madt_generic_interrupt {
    struct acpi_subtable_header header;
    u16 reserved;
    u32 cpu_interface_number;
    u32 uid;
    u32 flags;
    u32 parking_version;
    u32 performance_interrupt;
    u64 parked_address;
    u64 base_address;
    u64 gicv_base_address;
    u64 gich_base_address;
    u32 vgic_interrupt;
    u64 gicr_base_address;
    u64 arm_mpidr;
    u8 efficiency_class;
    u8 reserved2[1];
    u16 spe_interrupt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct acpi_madt_generic_interrupt {
    struct acpi_subtable_header header;
    u16 reserved;
    u32 cpu_interface_number;
    u32 uid;
    u32 flags;
    u32 parking_version;
    u32 performance_interrupt;
    u64 parked_address;
    u64 base_address;
    u64 gicv_base_address;
    u64 gich_base_address;
    u32 vgic_interrupt;
    u64 gicr_base_address;
    u64 arm_mpidr;
    u8 efficiency_class;
    u8 reserved2[1];
    u16 spe_interrupt;
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 spe_interrupt</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 reserved2[3]</code> ➡️ <code>u8 reserved2[1]</code>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 trbe_interrupt</code>
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
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
