# Struct: <code>acpi_pld_info</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct acpi_pld_info {
    u8 revision;
    u8 ignore_color;
    u8 red;
    u8 green;
    u8 blue;
    u16 width;
    u16 height;
    u8 user_visible;
    u8 dock;
    u8 lid;
    u8 panel;
    u8 vertical_position;
    u8 horizontal_position;
    u8 shape;
    u8 group_orientation;
    u8 group_token;
    u8 group_position;
    u8 bay;
    u8 ejectable;
    u8 ospm_eject_required;
    u8 cabinet_number;
    u8 card_cage_number;
    u8 reference;
    u8 rotation;
    u8 order;
    u8 reserved;
    u16 vertical_offset;
    u16 horizontal_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct acpi_pld_info {
    u8 revision;
    u8 ignore_color;
    u8 red;
    u8 green;
    u8 blue;
    u16 width;
    u16 height;
    u8 user_visible;
    u8 dock;
    u8 lid;
    u8 panel;
    u8 vertical_position;
    u8 horizontal_position;
    u8 shape;
    u8 group_orientation;
    u8 group_token;
    u8 group_position;
    u8 bay;
    u8 ejectable;
    u8 ospm_eject_required;
    u8 cabinet_number;
    u8 card_cage_number;
    u8 reference;
    u8 rotation;
    u8 order;
    u8 reserved;
    u16 vertical_offset;
    u16 horizontal_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct acpi_pld_info {
    u8 revision;
    u8 ignore_color;
    u8 red;
    u8 green;
    u8 blue;
    u16 width;
    u16 height;
    u8 user_visible;
    u8 dock;
    u8 lid;
    u8 panel;
    u8 vertical_position;
    u8 horizontal_position;
    u8 shape;
    u8 group_orientation;
    u8 group_token;
    u8 group_position;
    u8 bay;
    u8 ejectable;
    u8 ospm_eject_required;
    u8 cabinet_number;
    u8 card_cage_number;
    u8 reference;
    u8 rotation;
    u8 order;
    u8 reserved;
    u16 vertical_offset;
    u16 horizontal_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct acpi_pld_info {
    u8 revision;
    u8 ignore_color;
    u8 red;
    u8 green;
    u8 blue;
    u16 width;
    u16 height;
    u8 user_visible;
    u8 dock;
    u8 lid;
    u8 panel;
    u8 vertical_position;
    u8 horizontal_position;
    u8 shape;
    u8 group_orientation;
    u8 group_token;
    u8 group_position;
    u8 bay;
    u8 ejectable;
    u8 ospm_eject_required;
    u8 cabinet_number;
    u8 card_cage_number;
    u8 reference;
    u8 rotation;
    u8 order;
    u8 reserved;
    u16 vertical_offset;
    u16 horizontal_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct acpi_pld_info {
    u8 revision;
    u8 ignore_color;
    u8 red;
    u8 green;
    u8 blue;
    u16 width;
    u16 height;
    u8 user_visible;
    u8 dock;
    u8 lid;
    u8 panel;
    u8 vertical_position;
    u8 horizontal_position;
    u8 shape;
    u8 group_orientation;
    u8 group_token;
    u8 group_position;
    u8 bay;
    u8 ejectable;
    u8 ospm_eject_required;
    u8 cabinet_number;
    u8 card_cage_number;
    u8 reference;
    u8 rotation;
    u8 order;
    u8 reserved;
    u16 vertical_offset;
    u16 horizontal_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct acpi_pld_info {
    u8 revision;
    u8 ignore_color;
    u8 red;
    u8 green;
    u8 blue;
    u16 width;
    u16 height;
    u8 user_visible;
    u8 dock;
    u8 lid;
    u8 panel;
    u8 vertical_position;
    u8 horizontal_position;
    u8 shape;
    u8 group_orientation;
    u8 group_token;
    u8 group_position;
    u8 bay;
    u8 ejectable;
    u8 ospm_eject_required;
    u8 cabinet_number;
    u8 card_cage_number;
    u8 reference;
    u8 rotation;
    u8 order;
    u8 reserved;
    u16 vertical_offset;
    u16 horizontal_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct acpi_pld_info {
    u8 revision;
    u8 ignore_color;
    u8 red;
    u8 green;
    u8 blue;
    u16 width;
    u16 height;
    u8 user_visible;
    u8 dock;
    u8 lid;
    u8 panel;
    u8 vertical_position;
    u8 horizontal_position;
    u8 shape;
    u8 group_orientation;
    u8 group_token;
    u8 group_position;
    u8 bay;
    u8 ejectable;
    u8 ospm_eject_required;
    u8 cabinet_number;
    u8 card_cage_number;
    u8 reference;
    u8 rotation;
    u8 order;
    u8 reserved;
    u16 vertical_offset;
    u16 horizontal_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct acpi_pld_info {
    u8 revision;
    u8 ignore_color;
    u8 red;
    u8 green;
    u8 blue;
    u16 width;
    u16 height;
    u8 user_visible;
    u8 dock;
    u8 lid;
    u8 panel;
    u8 vertical_position;
    u8 horizontal_position;
    u8 shape;
    u8 group_orientation;
    u8 group_token;
    u8 group_position;
    u8 bay;
    u8 ejectable;
    u8 ospm_eject_required;
    u8 cabinet_number;
    u8 card_cage_number;
    u8 reference;
    u8 rotation;
    u8 order;
    u8 reserved;
    u16 vertical_offset;
    u16 horizontal_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct acpi_pld_info {
    u8 revision;
    u8 ignore_color;
    u8 red;
    u8 green;
    u8 blue;
    u16 width;
    u16 height;
    u8 user_visible;
    u8 dock;
    u8 lid;
    u8 panel;
    u8 vertical_position;
    u8 horizontal_position;
    u8 shape;
    u8 group_orientation;
    u8 group_token;
    u8 group_position;
    u8 bay;
    u8 ejectable;
    u8 ospm_eject_required;
    u8 cabinet_number;
    u8 card_cage_number;
    u8 reference;
    u8 rotation;
    u8 order;
    u8 reserved;
    u16 vertical_offset;
    u16 horizontal_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct acpi_pld_info {
    u8 revision;
    u8 ignore_color;
    u8 red;
    u8 green;
    u8 blue;
    u16 width;
    u16 height;
    u8 user_visible;
    u8 dock;
    u8 lid;
    u8 panel;
    u8 vertical_position;
    u8 horizontal_position;
    u8 shape;
    u8 group_orientation;
    u8 group_token;
    u8 group_position;
    u8 bay;
    u8 ejectable;
    u8 ospm_eject_required;
    u8 cabinet_number;
    u8 card_cage_number;
    u8 reference;
    u8 rotation;
    u8 order;
    u8 reserved;
    u16 vertical_offset;
    u16 horizontal_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct acpi_pld_info {
    u8 revision;
    u8 ignore_color;
    u8 red;
    u8 green;
    u8 blue;
    u16 width;
    u16 height;
    u8 user_visible;
    u8 dock;
    u8 lid;
    u8 panel;
    u8 vertical_position;
    u8 horizontal_position;
    u8 shape;
    u8 group_orientation;
    u8 group_token;
    u8 group_position;
    u8 bay;
    u8 ejectable;
    u8 ospm_eject_required;
    u8 cabinet_number;
    u8 card_cage_number;
    u8 reference;
    u8 rotation;
    u8 order;
    u8 reserved;
    u16 vertical_offset;
    u16 horizontal_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct acpi_pld_info {
    u8 revision;
    u8 ignore_color;
    u8 red;
    u8 green;
    u8 blue;
    u16 width;
    u16 height;
    u8 user_visible;
    u8 dock;
    u8 lid;
    u8 panel;
    u8 vertical_position;
    u8 horizontal_position;
    u8 shape;
    u8 group_orientation;
    u8 group_token;
    u8 group_position;
    u8 bay;
    u8 ejectable;
    u8 ospm_eject_required;
    u8 cabinet_number;
    u8 card_cage_number;
    u8 reference;
    u8 rotation;
    u8 order;
    u8 reserved;
    u16 vertical_offset;
    u16 horizontal_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct acpi_pld_info {
    u8 revision;
    u8 ignore_color;
    u8 red;
    u8 green;
    u8 blue;
    u16 width;
    u16 height;
    u8 user_visible;
    u8 dock;
    u8 lid;
    u8 panel;
    u8 vertical_position;
    u8 horizontal_position;
    u8 shape;
    u8 group_orientation;
    u8 group_token;
    u8 group_position;
    u8 bay;
    u8 ejectable;
    u8 ospm_eject_required;
    u8 cabinet_number;
    u8 card_cage_number;
    u8 reference;
    u8 rotation;
    u8 order;
    u8 reserved;
    u16 vertical_offset;
    u16 horizontal_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct acpi_pld_info {
    u8 revision;
    u8 ignore_color;
    u8 red;
    u8 green;
    u8 blue;
    u16 width;
    u16 height;
    u8 user_visible;
    u8 dock;
    u8 lid;
    u8 panel;
    u8 vertical_position;
    u8 horizontal_position;
    u8 shape;
    u8 group_orientation;
    u8 group_token;
    u8 group_position;
    u8 bay;
    u8 ejectable;
    u8 ospm_eject_required;
    u8 cabinet_number;
    u8 card_cage_number;
    u8 reference;
    u8 rotation;
    u8 order;
    u8 reserved;
    u16 vertical_offset;
    u16 horizontal_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct acpi_pld_info {
    u8 revision;
    u8 ignore_color;
    u8 red;
    u8 green;
    u8 blue;
    u16 width;
    u16 height;
    u8 user_visible;
    u8 dock;
    u8 lid;
    u8 panel;
    u8 vertical_position;
    u8 horizontal_position;
    u8 shape;
    u8 group_orientation;
    u8 group_token;
    u8 group_position;
    u8 bay;
    u8 ejectable;
    u8 ospm_eject_required;
    u8 cabinet_number;
    u8 card_cage_number;
    u8 reference;
    u8 rotation;
    u8 order;
    u8 reserved;
    u16 vertical_offset;
    u16 horizontal_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct acpi_pld_info {
    u8 revision;
    u8 ignore_color;
    u8 red;
    u8 green;
    u8 blue;
    u16 width;
    u16 height;
    u8 user_visible;
    u8 dock;
    u8 lid;
    u8 panel;
    u8 vertical_position;
    u8 horizontal_position;
    u8 shape;
    u8 group_orientation;
    u8 group_token;
    u8 group_position;
    u8 bay;
    u8 ejectable;
    u8 ospm_eject_required;
    u8 cabinet_number;
    u8 card_cage_number;
    u8 reference;
    u8 rotation;
    u8 order;
    u8 reserved;
    u16 vertical_offset;
    u16 horizontal_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct acpi_pld_info {
    u8 revision;
    u8 ignore_color;
    u8 red;
    u8 green;
    u8 blue;
    u16 width;
    u16 height;
    u8 user_visible;
    u8 dock;
    u8 lid;
    u8 panel;
    u8 vertical_position;
    u8 horizontal_position;
    u8 shape;
    u8 group_orientation;
    u8 group_token;
    u8 group_position;
    u8 bay;
    u8 ejectable;
    u8 ospm_eject_required;
    u8 cabinet_number;
    u8 card_cage_number;
    u8 reference;
    u8 rotation;
    u8 order;
    u8 reserved;
    u16 vertical_offset;
    u16 horizontal_offset;
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
struct acpi_pld_info {
    u8 revision;
    u8 ignore_color;
    u8 red;
    u8 green;
    u8 blue;
    u16 width;
    u16 height;
    u8 user_visible;
    u8 dock;
    u8 lid;
    u8 panel;
    u8 vertical_position;
    u8 horizontal_position;
    u8 shape;
    u8 group_orientation;
    u8 group_token;
    u8 group_position;
    u8 bay;
    u8 ejectable;
    u8 ospm_eject_required;
    u8 cabinet_number;
    u8 card_cage_number;
    u8 reference;
    u8 rotation;
    u8 order;
    u8 reserved;
    u16 vertical_offset;
    u16 horizontal_offset;
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
struct acpi_pld_info {
    u8 revision;
    u8 ignore_color;
    u8 red;
    u8 green;
    u8 blue;
    u16 width;
    u16 height;
    u8 user_visible;
    u8 dock;
    u8 lid;
    u8 panel;
    u8 vertical_position;
    u8 horizontal_position;
    u8 shape;
    u8 group_orientation;
    u8 group_token;
    u8 group_position;
    u8 bay;
    u8 ejectable;
    u8 ospm_eject_required;
    u8 cabinet_number;
    u8 card_cage_number;
    u8 reference;
    u8 rotation;
    u8 order;
    u8 reserved;
    u16 vertical_offset;
    u16 horizontal_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct acpi_pld_info {
    u8 revision;
    u8 ignore_color;
    u8 red;
    u8 green;
    u8 blue;
    u16 width;
    u16 height;
    u8 user_visible;
    u8 dock;
    u8 lid;
    u8 panel;
    u8 vertical_position;
    u8 horizontal_position;
    u8 shape;
    u8 group_orientation;
    u8 group_token;
    u8 group_position;
    u8 bay;
    u8 ejectable;
    u8 ospm_eject_required;
    u8 cabinet_number;
    u8 card_cage_number;
    u8 reference;
    u8 rotation;
    u8 order;
    u8 reserved;
    u16 vertical_offset;
    u16 horizontal_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct acpi_pld_info {
    u8 revision;
    u8 ignore_color;
    u8 red;
    u8 green;
    u8 blue;
    u16 width;
    u16 height;
    u8 user_visible;
    u8 dock;
    u8 lid;
    u8 panel;
    u8 vertical_position;
    u8 horizontal_position;
    u8 shape;
    u8 group_orientation;
    u8 group_token;
    u8 group_position;
    u8 bay;
    u8 ejectable;
    u8 ospm_eject_required;
    u8 cabinet_number;
    u8 card_cage_number;
    u8 reference;
    u8 rotation;
    u8 order;
    u8 reserved;
    u16 vertical_offset;
    u16 horizontal_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct acpi_pld_info {
    u8 revision;
    u8 ignore_color;
    u8 red;
    u8 green;
    u8 blue;
    u16 width;
    u16 height;
    u8 user_visible;
    u8 dock;
    u8 lid;
    u8 panel;
    u8 vertical_position;
    u8 horizontal_position;
    u8 shape;
    u8 group_orientation;
    u8 group_token;
    u8 group_position;
    u8 bay;
    u8 ejectable;
    u8 ospm_eject_required;
    u8 cabinet_number;
    u8 card_cage_number;
    u8 reference;
    u8 rotation;
    u8 order;
    u8 reserved;
    u16 vertical_offset;
    u16 horizontal_offset;
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
