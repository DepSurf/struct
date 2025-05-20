# Struct: <code>acpi_device_flags</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct acpi_device_flags {
    u32 dynamic_status;
    u32 removable;
    u32 ejectable;
    u32 power_manageable;
    u32 match_driver;
    u32 initialized;
    u32 visited;
    u32 hotplug_notify;
    u32 is_dock_station;
    u32 of_compatible_ok;
    u32 coherent_dma;
    u32 cca_seen;
    u32 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct acpi_device_flags {
    u32 dynamic_status;
    u32 removable;
    u32 ejectable;
    u32 power_manageable;
    u32 match_driver;
    u32 initialized;
    u32 visited;
    u32 hotplug_notify;
    u32 is_dock_station;
    u32 of_compatible_ok;
    u32 coherent_dma;
    u32 cca_seen;
    u32 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct acpi_device_flags {
    u32 dynamic_status;
    u32 removable;
    u32 ejectable;
    u32 power_manageable;
    u32 match_driver;
    u32 initialized;
    u32 visited;
    u32 hotplug_notify;
    u32 is_dock_station;
    u32 of_compatible_ok;
    u32 coherent_dma;
    u32 cca_seen;
    u32 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct acpi_device_flags {
    u32 dynamic_status;
    u32 removable;
    u32 ejectable;
    u32 power_manageable;
    u32 match_driver;
    u32 initialized;
    u32 visited;
    u32 hotplug_notify;
    u32 is_dock_station;
    u32 of_compatible_ok;
    u32 coherent_dma;
    u32 cca_seen;
    u32 spi_i2c_slave;
    u32 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct acpi_device_flags {
    u32 dynamic_status;
    u32 removable;
    u32 ejectable;
    u32 power_manageable;
    u32 match_driver;
    u32 initialized;
    u32 visited;
    u32 hotplug_notify;
    u32 is_dock_station;
    u32 of_compatible_ok;
    u32 coherent_dma;
    u32 cca_seen;
    u32 enumeration_by_parent;
    u32 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct acpi_device_flags {
    u32 dynamic_status;
    u32 removable;
    u32 ejectable;
    u32 power_manageable;
    u32 match_driver;
    u32 initialized;
    u32 visited;
    u32 hotplug_notify;
    u32 is_dock_station;
    u32 of_compatible_ok;
    u32 coherent_dma;
    u32 cca_seen;
    u32 enumeration_by_parent;
    u32 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct acpi_device_flags {
    u32 dynamic_status;
    u32 removable;
    u32 ejectable;
    u32 power_manageable;
    u32 match_driver;
    u32 initialized;
    u32 visited;
    u32 hotplug_notify;
    u32 is_dock_station;
    u32 of_compatible_ok;
    u32 coherent_dma;
    u32 cca_seen;
    u32 enumeration_by_parent;
    u32 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct acpi_device_flags {
    u32 dynamic_status;
    u32 removable;
    u32 ejectable;
    u32 power_manageable;
    u32 match_driver;
    u32 initialized;
    u32 visited;
    u32 hotplug_notify;
    u32 is_dock_station;
    u32 of_compatible_ok;
    u32 coherent_dma;
    u32 cca_seen;
    u32 enumeration_by_parent;
    u32 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct acpi_device_flags {
    u32 dynamic_status;
    u32 removable;
    u32 ejectable;
    u32 power_manageable;
    u32 match_driver;
    u32 initialized;
    u32 visited;
    u32 hotplug_notify;
    u32 is_dock_station;
    u32 of_compatible_ok;
    u32 coherent_dma;
    u32 cca_seen;
    u32 enumeration_by_parent;
    u32 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct acpi_device_flags {
    u32 dynamic_status;
    u32 removable;
    u32 ejectable;
    u32 power_manageable;
    u32 match_driver;
    u32 initialized;
    u32 visited;
    u32 hotplug_notify;
    u32 is_dock_station;
    u32 of_compatible_ok;
    u32 coherent_dma;
    u32 cca_seen;
    u32 enumeration_by_parent;
    u32 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct acpi_device_flags {
    u32 dynamic_status;
    u32 removable;
    u32 ejectable;
    u32 power_manageable;
    u32 match_driver;
    u32 initialized;
    u32 visited;
    u32 hotplug_notify;
    u32 is_dock_station;
    u32 of_compatible_ok;
    u32 coherent_dma;
    u32 cca_seen;
    u32 enumeration_by_parent;
    u32 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct acpi_device_flags {
    u32 dynamic_status;
    u32 removable;
    u32 ejectable;
    u32 power_manageable;
    u32 match_driver;
    u32 initialized;
    u32 visited;
    u32 hotplug_notify;
    u32 is_dock_station;
    u32 of_compatible_ok;
    u32 coherent_dma;
    u32 cca_seen;
    u32 enumeration_by_parent;
    u32 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct acpi_device_flags {
    u32 dynamic_status;
    u32 removable;
    u32 ejectable;
    u32 power_manageable;
    u32 match_driver;
    u32 initialized;
    u32 visited;
    u32 hotplug_notify;
    u32 is_dock_station;
    u32 of_compatible_ok;
    u32 coherent_dma;
    u32 cca_seen;
    u32 enumeration_by_parent;
    u32 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct acpi_device_flags {
    u32 dynamic_status;
    u32 removable;
    u32 ejectable;
    u32 power_manageable;
    u32 match_driver;
    u32 initialized;
    u32 visited;
    u32 hotplug_notify;
    u32 is_dock_station;
    u32 of_compatible_ok;
    u32 coherent_dma;
    u32 cca_seen;
    u32 enumeration_by_parent;
    u32 honor_deps;
    u32 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct acpi_device_flags {
    u32 dynamic_status;
    u32 removable;
    u32 ejectable;
    u32 power_manageable;
    u32 match_driver;
    u32 initialized;
    u32 visited;
    u32 hotplug_notify;
    u32 is_dock_station;
    u32 of_compatible_ok;
    u32 coherent_dma;
    u32 cca_seen;
    u32 enumeration_by_parent;
    u32 honor_deps;
    u32 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct acpi_device_flags {
    u32 dynamic_status;
    u32 removable;
    u32 ejectable;
    u32 power_manageable;
    u32 match_driver;
    u32 initialized;
    u32 visited;
    u32 hotplug_notify;
    u32 is_dock_station;
    u32 of_compatible_ok;
    u32 coherent_dma;
    u32 cca_seen;
    u32 enumeration_by_parent;
    u32 honor_deps;
    u32 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct acpi_device_flags {
    u32 dynamic_status;
    u32 removable;
    u32 ejectable;
    u32 power_manageable;
    u32 match_driver;
    u32 initialized;
    u32 visited;
    u32 hotplug_notify;
    u32 is_dock_station;
    u32 of_compatible_ok;
    u32 coherent_dma;
    u32 cca_seen;
    u32 enumeration_by_parent;
    u32 honor_deps;
    u32 reserved;
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
struct acpi_device_flags {
    u32 dynamic_status;
    u32 removable;
    u32 ejectable;
    u32 power_manageable;
    u32 match_driver;
    u32 initialized;
    u32 visited;
    u32 hotplug_notify;
    u32 is_dock_station;
    u32 of_compatible_ok;
    u32 coherent_dma;
    u32 cca_seen;
    u32 enumeration_by_parent;
    u32 reserved;
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
struct acpi_device_flags {
    u32 dynamic_status;
    u32 removable;
    u32 ejectable;
    u32 power_manageable;
    u32 match_driver;
    u32 initialized;
    u32 visited;
    u32 hotplug_notify;
    u32 is_dock_station;
    u32 of_compatible_ok;
    u32 coherent_dma;
    u32 cca_seen;
    u32 enumeration_by_parent;
    u32 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct acpi_device_flags {
    u32 dynamic_status;
    u32 removable;
    u32 ejectable;
    u32 power_manageable;
    u32 match_driver;
    u32 initialized;
    u32 visited;
    u32 hotplug_notify;
    u32 is_dock_station;
    u32 of_compatible_ok;
    u32 coherent_dma;
    u32 cca_seen;
    u32 enumeration_by_parent;
    u32 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct acpi_device_flags {
    u32 dynamic_status;
    u32 removable;
    u32 ejectable;
    u32 power_manageable;
    u32 match_driver;
    u32 initialized;
    u32 visited;
    u32 hotplug_notify;
    u32 is_dock_station;
    u32 of_compatible_ok;
    u32 coherent_dma;
    u32 cca_seen;
    u32 enumeration_by_parent;
    u32 reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct acpi_device_flags {
    u32 dynamic_status;
    u32 removable;
    u32 ejectable;
    u32 power_manageable;
    u32 match_driver;
    u32 initialized;
    u32 visited;
    u32 hotplug_notify;
    u32 is_dock_station;
    u32 of_compatible_ok;
    u32 coherent_dma;
    u32 cca_seen;
    u32 enumeration_by_parent;
    u32 reserved;
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
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 spi_i2c_slave</code>
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
<code>u32 enumeration_by_parent</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 spi_i2c_slave</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 honor_deps</code>
</li>
</ul>
</details>
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
