# Struct: <code>acpi_create_field_info</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct acpi_create_field_info {
    struct acpi_namespace_node *region_node;
    struct acpi_namespace_node *field_node;
    struct acpi_namespace_node *register_node;
    struct acpi_namespace_node *data_register_node;
    struct acpi_namespace_node *connection_node;
    u8 *resource_buffer;
    u32 bank_value;
    u32 field_bit_position;
    u32 field_bit_length;
    u16 resource_length;
    u16 pin_number_index;
    u8 field_flags;
    u8 attribute;
    u8 field_type;
    u8 access_length;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct acpi_create_field_info {
    struct acpi_namespace_node *region_node;
    struct acpi_namespace_node *field_node;
    struct acpi_namespace_node *register_node;
    struct acpi_namespace_node *data_register_node;
    struct acpi_namespace_node *connection_node;
    u8 *resource_buffer;
    u32 bank_value;
    u32 field_bit_position;
    u32 field_bit_length;
    u16 resource_length;
    u16 pin_number_index;
    u8 field_flags;
    u8 attribute;
    u8 field_type;
    u8 access_length;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct acpi_create_field_info {
    struct acpi_namespace_node *region_node;
    struct acpi_namespace_node *field_node;
    struct acpi_namespace_node *register_node;
    struct acpi_namespace_node *data_register_node;
    struct acpi_namespace_node *connection_node;
    u8 *resource_buffer;
    u32 bank_value;
    u32 field_bit_position;
    u32 field_bit_length;
    u16 resource_length;
    u16 pin_number_index;
    u8 field_flags;
    u8 attribute;
    u8 field_type;
    u8 access_length;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct acpi_create_field_info {
    struct acpi_namespace_node *region_node;
    struct acpi_namespace_node *field_node;
    struct acpi_namespace_node *register_node;
    struct acpi_namespace_node *data_register_node;
    struct acpi_namespace_node *connection_node;
    u8 *resource_buffer;
    u32 bank_value;
    u32 field_bit_position;
    u32 field_bit_length;
    u16 resource_length;
    u16 pin_number_index;
    u8 field_flags;
    u8 attribute;
    u8 field_type;
    u8 access_length;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct acpi_create_field_info {
    struct acpi_namespace_node *region_node;
    struct acpi_namespace_node *field_node;
    struct acpi_namespace_node *register_node;
    struct acpi_namespace_node *data_register_node;
    struct acpi_namespace_node *connection_node;
    u8 *resource_buffer;
    u32 bank_value;
    u32 field_bit_position;
    u32 field_bit_length;
    u16 resource_length;
    u16 pin_number_index;
    u8 field_flags;
    u8 attribute;
    u8 field_type;
    u8 access_length;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct acpi_create_field_info {
    struct acpi_namespace_node *region_node;
    struct acpi_namespace_node *field_node;
    struct acpi_namespace_node *register_node;
    struct acpi_namespace_node *data_register_node;
    struct acpi_namespace_node *connection_node;
    u8 *resource_buffer;
    u32 bank_value;
    u32 field_bit_position;
    u32 field_bit_length;
    u16 resource_length;
    u16 pin_number_index;
    u8 field_flags;
    u8 attribute;
    u8 field_type;
    u8 access_length;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct acpi_create_field_info {
    struct acpi_namespace_node *region_node;
    struct acpi_namespace_node *field_node;
    struct acpi_namespace_node *register_node;
    struct acpi_namespace_node *data_register_node;
    struct acpi_namespace_node *connection_node;
    u8 *resource_buffer;
    u32 bank_value;
    u32 field_bit_position;
    u32 field_bit_length;
    u16 resource_length;
    u16 pin_number_index;
    u8 field_flags;
    u8 attribute;
    u8 field_type;
    u8 access_length;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct acpi_create_field_info {
    struct acpi_namespace_node *region_node;
    struct acpi_namespace_node *field_node;
    struct acpi_namespace_node *register_node;
    struct acpi_namespace_node *data_register_node;
    struct acpi_namespace_node *connection_node;
    u8 *resource_buffer;
    u32 bank_value;
    u32 field_bit_position;
    u32 field_bit_length;
    u16 resource_length;
    u16 pin_number_index;
    u8 field_flags;
    u8 attribute;
    u8 field_type;
    u8 access_length;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct acpi_create_field_info {
    struct acpi_namespace_node *region_node;
    struct acpi_namespace_node *field_node;
    struct acpi_namespace_node *register_node;
    struct acpi_namespace_node *data_register_node;
    struct acpi_namespace_node *connection_node;
    u8 *resource_buffer;
    u32 bank_value;
    u32 field_bit_position;
    u32 field_bit_length;
    u16 resource_length;
    u16 pin_number_index;
    u8 field_flags;
    u8 attribute;
    u8 field_type;
    u8 access_length;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct acpi_create_field_info {
    struct acpi_namespace_node *region_node;
    struct acpi_namespace_node *field_node;
    struct acpi_namespace_node *register_node;
    struct acpi_namespace_node *data_register_node;
    struct acpi_namespace_node *connection_node;
    u8 *resource_buffer;
    u32 bank_value;
    u32 field_bit_position;
    u32 field_bit_length;
    u16 resource_length;
    u16 pin_number_index;
    u8 field_flags;
    u8 attribute;
    u8 field_type;
    u8 access_length;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct acpi_create_field_info {
    struct acpi_namespace_node *region_node;
    struct acpi_namespace_node *field_node;
    struct acpi_namespace_node *register_node;
    struct acpi_namespace_node *data_register_node;
    struct acpi_namespace_node *connection_node;
    u8 *resource_buffer;
    u32 bank_value;
    u32 field_bit_position;
    u32 field_bit_length;
    u16 resource_length;
    u16 pin_number_index;
    u8 field_flags;
    u8 attribute;
    u8 field_type;
    u8 access_length;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct acpi_create_field_info {
    struct acpi_namespace_node *region_node;
    struct acpi_namespace_node *field_node;
    struct acpi_namespace_node *register_node;
    struct acpi_namespace_node *data_register_node;
    struct acpi_namespace_node *connection_node;
    u8 *resource_buffer;
    u32 bank_value;
    u32 field_bit_position;
    u32 field_bit_length;
    u16 resource_length;
    u16 pin_number_index;
    u8 field_flags;
    u8 attribute;
    u8 field_type;
    u8 access_length;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct acpi_create_field_info {
    struct acpi_namespace_node *region_node;
    struct acpi_namespace_node *field_node;
    struct acpi_namespace_node *register_node;
    struct acpi_namespace_node *data_register_node;
    struct acpi_namespace_node *connection_node;
    u8 *resource_buffer;
    u32 bank_value;
    u32 field_bit_position;
    u32 field_bit_length;
    u16 resource_length;
    u16 pin_number_index;
    u8 field_flags;
    u8 attribute;
    u8 field_type;
    u8 access_length;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct acpi_create_field_info {
    struct acpi_namespace_node *region_node;
    struct acpi_namespace_node *field_node;
    struct acpi_namespace_node *register_node;
    struct acpi_namespace_node *data_register_node;
    struct acpi_namespace_node *connection_node;
    u8 *resource_buffer;
    u32 bank_value;
    u32 field_bit_position;
    u32 field_bit_length;
    u16 resource_length;
    u16 pin_number_index;
    u8 field_flags;
    u8 attribute;
    u8 field_type;
    u8 access_length;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct acpi_create_field_info {
    struct acpi_namespace_node *region_node;
    struct acpi_namespace_node *field_node;
    struct acpi_namespace_node *register_node;
    struct acpi_namespace_node *data_register_node;
    struct acpi_namespace_node *connection_node;
    u8 *resource_buffer;
    u32 bank_value;
    u32 field_bit_position;
    u32 field_bit_length;
    u16 resource_length;
    u16 pin_number_index;
    u8 field_flags;
    u8 attribute;
    u8 field_type;
    u8 access_length;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct acpi_create_field_info {
    struct acpi_namespace_node *region_node;
    struct acpi_namespace_node *field_node;
    struct acpi_namespace_node *register_node;
    struct acpi_namespace_node *data_register_node;
    struct acpi_namespace_node *connection_node;
    u8 *resource_buffer;
    u32 bank_value;
    u32 field_bit_position;
    u32 field_bit_length;
    u16 resource_length;
    u16 pin_number_index;
    u8 field_flags;
    u8 attribute;
    u8 field_type;
    u8 access_length;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct acpi_create_field_info {
    struct acpi_namespace_node *region_node;
    struct acpi_namespace_node *field_node;
    struct acpi_namespace_node *register_node;
    struct acpi_namespace_node *data_register_node;
    struct acpi_namespace_node *connection_node;
    u8 *resource_buffer;
    u32 bank_value;
    u32 field_bit_position;
    u32 field_bit_length;
    u16 resource_length;
    u16 pin_number_index;
    u8 field_flags;
    u8 attribute;
    u8 field_type;
    u8 access_length;
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
struct acpi_create_field_info {
    struct acpi_namespace_node *region_node;
    struct acpi_namespace_node *field_node;
    struct acpi_namespace_node *register_node;
    struct acpi_namespace_node *data_register_node;
    struct acpi_namespace_node *connection_node;
    u8 *resource_buffer;
    u32 bank_value;
    u32 field_bit_position;
    u32 field_bit_length;
    u16 resource_length;
    u16 pin_number_index;
    u8 field_flags;
    u8 attribute;
    u8 field_type;
    u8 access_length;
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
struct acpi_create_field_info {
    struct acpi_namespace_node *region_node;
    struct acpi_namespace_node *field_node;
    struct acpi_namespace_node *register_node;
    struct acpi_namespace_node *data_register_node;
    struct acpi_namespace_node *connection_node;
    u8 *resource_buffer;
    u32 bank_value;
    u32 field_bit_position;
    u32 field_bit_length;
    u16 resource_length;
    u16 pin_number_index;
    u8 field_flags;
    u8 attribute;
    u8 field_type;
    u8 access_length;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct acpi_create_field_info {
    struct acpi_namespace_node *region_node;
    struct acpi_namespace_node *field_node;
    struct acpi_namespace_node *register_node;
    struct acpi_namespace_node *data_register_node;
    struct acpi_namespace_node *connection_node;
    u8 *resource_buffer;
    u32 bank_value;
    u32 field_bit_position;
    u32 field_bit_length;
    u16 resource_length;
    u16 pin_number_index;
    u8 field_flags;
    u8 attribute;
    u8 field_type;
    u8 access_length;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct acpi_create_field_info {
    struct acpi_namespace_node *region_node;
    struct acpi_namespace_node *field_node;
    struct acpi_namespace_node *register_node;
    struct acpi_namespace_node *data_register_node;
    struct acpi_namespace_node *connection_node;
    u8 *resource_buffer;
    u32 bank_value;
    u32 field_bit_position;
    u32 field_bit_length;
    u16 resource_length;
    u16 pin_number_index;
    u8 field_flags;
    u8 attribute;
    u8 field_type;
    u8 access_length;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct acpi_create_field_info {
    struct acpi_namespace_node *region_node;
    struct acpi_namespace_node *field_node;
    struct acpi_namespace_node *register_node;
    struct acpi_namespace_node *data_register_node;
    struct acpi_namespace_node *connection_node;
    u8 *resource_buffer;
    u32 bank_value;
    u32 field_bit_position;
    u32 field_bit_length;
    u16 resource_length;
    u16 pin_number_index;
    u8 field_flags;
    u8 attribute;
    u8 field_type;
    u8 access_length;
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
