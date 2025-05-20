# Struct: <code>memdev_dmi_entry</code>

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
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct memdev_dmi_entry {
    u8 type;
    u8 length;
    u16 handle;
    u16 phys_mem_array_handle;
    u16 mem_err_info_handle;
    u16 total_width;
    u16 data_width;
    u16 size;
    u8 form_factor;
    u8 device_set;
    u8 device_locator;
    u8 bank_locator;
    u8 memory_type;
    u16 type_detail;
    u16 speed;
    u8 manufacturer;
    u8 serial_number;
    u8 asset_tag;
    u8 part_number;
    u8 attributes;
    u32 extended_size;
    u16 conf_mem_clk_speed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct memdev_dmi_entry {
    u8 type;
    u8 length;
    u16 handle;
    u16 phys_mem_array_handle;
    u16 mem_err_info_handle;
    u16 total_width;
    u16 data_width;
    u16 size;
    u8 form_factor;
    u8 device_set;
    u8 device_locator;
    u8 bank_locator;
    u8 memory_type;
    u16 type_detail;
    u16 speed;
    u8 manufacturer;
    u8 serial_number;
    u8 asset_tag;
    u8 part_number;
    u8 attributes;
    u32 extended_size;
    u16 conf_mem_clk_speed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct memdev_dmi_entry {
    u8 type;
    u8 length;
    u16 handle;
    u16 phys_mem_array_handle;
    u16 mem_err_info_handle;
    u16 total_width;
    u16 data_width;
    u16 size;
    u8 form_factor;
    u8 device_set;
    u8 device_locator;
    u8 bank_locator;
    u8 memory_type;
    u16 type_detail;
    u16 speed;
    u8 manufacturer;
    u8 serial_number;
    u8 asset_tag;
    u8 part_number;
    u8 attributes;
    u32 extended_size;
    u16 conf_mem_clk_speed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct memdev_dmi_entry {
    u8 type;
    u8 length;
    u16 handle;
    u16 phys_mem_array_handle;
    u16 mem_err_info_handle;
    u16 total_width;
    u16 data_width;
    u16 size;
    u8 form_factor;
    u8 device_set;
    u8 device_locator;
    u8 bank_locator;
    u8 memory_type;
    u16 type_detail;
    u16 speed;
    u8 manufacturer;
    u8 serial_number;
    u8 asset_tag;
    u8 part_number;
    u8 attributes;
    u32 extended_size;
    u16 conf_mem_clk_speed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct memdev_dmi_entry {
    u8 type;
    u8 length;
    u16 handle;
    u16 phys_mem_array_handle;
    u16 mem_err_info_handle;
    u16 total_width;
    u16 data_width;
    u16 size;
    u8 form_factor;
    u8 device_set;
    u8 device_locator;
    u8 bank_locator;
    u8 memory_type;
    u16 type_detail;
    u16 speed;
    u8 manufacturer;
    u8 serial_number;
    u8 asset_tag;
    u8 part_number;
    u8 attributes;
    u32 extended_size;
    u16 conf_mem_clk_speed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct memdev_dmi_entry {
    u8 type;
    u8 length;
    u16 handle;
    u16 phys_mem_array_handle;
    u16 mem_err_info_handle;
    u16 total_width;
    u16 data_width;
    u16 size;
    u8 form_factor;
    u8 device_set;
    u8 device_locator;
    u8 bank_locator;
    u8 memory_type;
    u16 type_detail;
    u16 speed;
    u8 manufacturer;
    u8 serial_number;
    u8 asset_tag;
    u8 part_number;
    u8 attributes;
    u32 extended_size;
    u16 conf_mem_clk_speed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct memdev_dmi_entry {
    u8 type;
    u8 length;
    u16 handle;
    u16 phys_mem_array_handle;
    u16 mem_err_info_handle;
    u16 total_width;
    u16 data_width;
    u16 size;
    u8 form_factor;
    u8 device_set;
    u8 device_locator;
    u8 bank_locator;
    u8 memory_type;
    u16 type_detail;
    u16 speed;
    u8 manufacturer;
    u8 serial_number;
    u8 asset_tag;
    u8 part_number;
    u8 attributes;
    u32 extended_size;
    u16 conf_mem_clk_speed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct memdev_dmi_entry {
    u8 type;
    u8 length;
    u16 handle;
    u16 phys_mem_array_handle;
    u16 mem_err_info_handle;
    u16 total_width;
    u16 data_width;
    u16 size;
    u8 form_factor;
    u8 device_set;
    u8 device_locator;
    u8 bank_locator;
    u8 memory_type;
    u16 type_detail;
    u16 speed;
    u8 manufacturer;
    u8 serial_number;
    u8 asset_tag;
    u8 part_number;
    u8 attributes;
    u32 extended_size;
    u16 conf_mem_clk_speed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct memdev_dmi_entry {
    u8 type;
    u8 length;
    u16 handle;
    u16 phys_mem_array_handle;
    u16 mem_err_info_handle;
    u16 total_width;
    u16 data_width;
    u16 size;
    u8 form_factor;
    u8 device_set;
    u8 device_locator;
    u8 bank_locator;
    u8 memory_type;
    u16 type_detail;
    u16 speed;
    u8 manufacturer;
    u8 serial_number;
    u8 asset_tag;
    u8 part_number;
    u8 attributes;
    u32 extended_size;
    u16 conf_mem_clk_speed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct memdev_dmi_entry {
    u8 type;
    u8 length;
    u16 handle;
    u16 phys_mem_array_handle;
    u16 mem_err_info_handle;
    u16 total_width;
    u16 data_width;
    u16 size;
    u8 form_factor;
    u8 device_set;
    u8 device_locator;
    u8 bank_locator;
    u8 memory_type;
    u16 type_detail;
    u16 speed;
    u8 manufacturer;
    u8 serial_number;
    u8 asset_tag;
    u8 part_number;
    u8 attributes;
    u32 extended_size;
    u16 conf_mem_clk_speed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct memdev_dmi_entry {
    u8 type;
    u8 length;
    u16 handle;
    u16 phys_mem_array_handle;
    u16 mem_err_info_handle;
    u16 total_width;
    u16 data_width;
    u16 size;
    u8 form_factor;
    u8 device_set;
    u8 device_locator;
    u8 bank_locator;
    u8 memory_type;
    u16 type_detail;
    u16 speed;
    u8 manufacturer;
    u8 serial_number;
    u8 asset_tag;
    u8 part_number;
    u8 attributes;
    u32 extended_size;
    u16 conf_mem_clk_speed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct memdev_dmi_entry {
    u8 type;
    u8 length;
    u16 handle;
    u16 phys_mem_array_handle;
    u16 mem_err_info_handle;
    u16 total_width;
    u16 data_width;
    u16 size;
    u8 form_factor;
    u8 device_set;
    u8 device_locator;
    u8 bank_locator;
    u8 memory_type;
    u16 type_detail;
    u16 speed;
    u8 manufacturer;
    u8 serial_number;
    u8 asset_tag;
    u8 part_number;
    u8 attributes;
    u32 extended_size;
    u16 conf_mem_clk_speed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct memdev_dmi_entry {
    u8 type;
    u8 length;
    u16 handle;
    u16 phys_mem_array_handle;
    u16 mem_err_info_handle;
    u16 total_width;
    u16 data_width;
    u16 size;
    u8 form_factor;
    u8 device_set;
    u8 device_locator;
    u8 bank_locator;
    u8 memory_type;
    u16 type_detail;
    u16 speed;
    u8 manufacturer;
    u8 serial_number;
    u8 asset_tag;
    u8 part_number;
    u8 attributes;
    u32 extended_size;
    u16 conf_mem_clk_speed;
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
struct memdev_dmi_entry {
    u8 type;
    u8 length;
    u16 handle;
    u16 phys_mem_array_handle;
    u16 mem_err_info_handle;
    u16 total_width;
    u16 data_width;
    u16 size;
    u8 form_factor;
    u8 device_set;
    u8 device_locator;
    u8 bank_locator;
    u8 memory_type;
    u16 type_detail;
    u16 speed;
    u8 manufacturer;
    u8 serial_number;
    u8 asset_tag;
    u8 part_number;
    u8 attributes;
    u32 extended_size;
    u16 conf_mem_clk_speed;
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
In <code>aws</code>: Absent ⚠️
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct memdev_dmi_entry {
    u8 type;
    u8 length;
    u16 handle;
    u16 phys_mem_array_handle;
    u16 mem_err_info_handle;
    u16 total_width;
    u16 data_width;
    u16 size;
    u8 form_factor;
    u8 device_set;
    u8 device_locator;
    u8 bank_locator;
    u8 memory_type;
    u16 type_detail;
    u16 speed;
    u8 manufacturer;
    u8 serial_number;
    u8 asset_tag;
    u8 part_number;
    u8 attributes;
    u32 extended_size;
    u16 conf_mem_clk_speed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct memdev_dmi_entry {
    u8 type;
    u8 length;
    u16 handle;
    u16 phys_mem_array_handle;
    u16 mem_err_info_handle;
    u16 total_width;
    u16 data_width;
    u16 size;
    u8 form_factor;
    u8 device_set;
    u8 device_locator;
    u8 bank_locator;
    u8 memory_type;
    u16 type_detail;
    u16 speed;
    u8 manufacturer;
    u8 serial_number;
    u8 asset_tag;
    u8 part_number;
    u8 attributes;
    u32 extended_size;
    u16 conf_mem_clk_speed;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
