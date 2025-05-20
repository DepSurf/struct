# Struct: <code>acpi_pci_link_irq</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct acpi_pci_link_irq {
    u8 active;
    u8 triggering;
    u8 polarity;
    u8 resource_type;
    u8 possible_count;
    u8 possible[16];
    u8 initialized;
    u8 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct acpi_pci_link_irq {
    u32 active;
    u8 triggering;
    u8 polarity;
    u8 resource_type;
    u8 possible_count;
    u32 possible[16];
    u8 initialized;
    u8 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct acpi_pci_link_irq {
    u32 active;
    u8 triggering;
    u8 polarity;
    u8 resource_type;
    u8 possible_count;
    u32 possible[16];
    u8 initialized;
    u8 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct acpi_pci_link_irq {
    u32 active;
    u8 triggering;
    u8 polarity;
    u8 resource_type;
    u8 possible_count;
    u32 possible[16];
    u8 initialized;
    u8 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct acpi_pci_link_irq {
    u32 active;
    u8 triggering;
    u8 polarity;
    u8 resource_type;
    u8 possible_count;
    u32 possible[16];
    u8 initialized;
    u8 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct acpi_pci_link_irq {
    u32 active;
    u8 triggering;
    u8 polarity;
    u8 resource_type;
    u8 possible_count;
    u32 possible[16];
    u8 initialized;
    u8 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct acpi_pci_link_irq {
    u32 active;
    u8 triggering;
    u8 polarity;
    u8 resource_type;
    u8 possible_count;
    u32 possible[16];
    u8 initialized;
    u8 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct acpi_pci_link_irq {
    u32 active;
    u8 triggering;
    u8 polarity;
    u8 resource_type;
    u8 possible_count;
    u32 possible[16];
    u8 initialized;
    u8 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct acpi_pci_link_irq {
    u32 active;
    u8 triggering;
    u8 polarity;
    u8 resource_type;
    u8 possible_count;
    u32 possible[16];
    u8 initialized;
    u8 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct acpi_pci_link_irq {
    u32 active;
    u8 triggering;
    u8 polarity;
    u8 resource_type;
    u8 possible_count;
    u32 possible[16];
    u8 initialized;
    u8 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct acpi_pci_link_irq {
    u32 active;
    u8 triggering;
    u8 polarity;
    u8 resource_type;
    u8 possible_count;
    u32 possible[16];
    u8 initialized;
    u8 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct acpi_pci_link_irq {
    u32 active;
    u8 triggering;
    u8 polarity;
    u8 resource_type;
    u8 possible_count;
    u32 possible[16];
    u8 initialized;
    u8 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct acpi_pci_link_irq {
    u32 active;
    u8 triggering;
    u8 polarity;
    u8 resource_type;
    u8 possible_count;
    u32 possible[16];
    u8 initialized;
    u8 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct acpi_pci_link_irq {
    u32 active;
    u8 triggering;
    u8 polarity;
    u8 resource_type;
    u8 possible_count;
    u32 possible[16];
    u8 initialized;
    u8 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct acpi_pci_link_irq {
    u32 active;
    u8 triggering;
    u8 polarity;
    u8 resource_type;
    u8 possible_count;
    u32 possible[16];
    u8 initialized;
    u8 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct acpi_pci_link_irq {
    u32 active;
    u8 triggering;
    u8 polarity;
    u8 resource_type;
    u8 possible_count;
    u32 possible[16];
    u8 initialized;
    u8 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct acpi_pci_link_irq {
    u32 active;
    u8 triggering;
    u8 polarity;
    u8 resource_type;
    u8 possible_count;
    u32 possible[16];
    u8 initialized;
    u8 reserved;
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
struct acpi_pci_link_irq {
    u32 active;
    u8 triggering;
    u8 polarity;
    u8 resource_type;
    u8 possible_count;
    u32 possible[16];
    u8 initialized;
    u8 reserved;
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
struct acpi_pci_link_irq {
    u32 active;
    u8 triggering;
    u8 polarity;
    u8 resource_type;
    u8 possible_count;
    u32 possible[16];
    u8 initialized;
    u8 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct acpi_pci_link_irq {
    u32 active;
    u8 triggering;
    u8 polarity;
    u8 resource_type;
    u8 possible_count;
    u32 possible[16];
    u8 initialized;
    u8 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct acpi_pci_link_irq {
    u32 active;
    u8 triggering;
    u8 polarity;
    u8 resource_type;
    u8 possible_count;
    u32 possible[16];
    u8 initialized;
    u8 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct acpi_pci_link_irq {
    u32 active;
    u8 triggering;
    u8 polarity;
    u8 resource_type;
    u8 possible_count;
    u32 possible[16];
    u8 initialized;
    u8 reserved;
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
<code>u8 active</code> ➡️ <code>u32 active</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 possible[16]</code> ➡️ <code>u32 possible[16]</code>
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
