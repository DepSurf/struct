# Struct: <code>edd_device_params</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct edd_device_params {
    __u16 length;
    __u16 info_flags;
    __u32 num_default_cylinders;
    __u32 num_default_heads;
    __u32 sectors_per_track;
    __u64 number_of_sectors;
    __u16 bytes_per_sector;
    __u32 dpte_ptr;
    __u16 key;
    __u8 device_path_info_length;
    __u8 reserved2;
    __u16 reserved3;
    __u8 host_bus_type[4];
    __u8 interface_type[8];
    union (anon) interface_path;
    union (anon) device_path;
    __u8 reserved4;
    __u8 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct edd_device_params {
    __u16 length;
    __u16 info_flags;
    __u32 num_default_cylinders;
    __u32 num_default_heads;
    __u32 sectors_per_track;
    __u64 number_of_sectors;
    __u16 bytes_per_sector;
    __u32 dpte_ptr;
    __u16 key;
    __u8 device_path_info_length;
    __u8 reserved2;
    __u16 reserved3;
    __u8 host_bus_type[4];
    __u8 interface_type[8];
    union (anon) interface_path;
    union (anon) device_path;
    __u8 reserved4;
    __u8 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct edd_device_params {
    __u16 length;
    __u16 info_flags;
    __u32 num_default_cylinders;
    __u32 num_default_heads;
    __u32 sectors_per_track;
    __u64 number_of_sectors;
    __u16 bytes_per_sector;
    __u32 dpte_ptr;
    __u16 key;
    __u8 device_path_info_length;
    __u8 reserved2;
    __u16 reserved3;
    __u8 host_bus_type[4];
    __u8 interface_type[8];
    union (anon) interface_path;
    union (anon) device_path;
    __u8 reserved4;
    __u8 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct edd_device_params {
    __u16 length;
    __u16 info_flags;
    __u32 num_default_cylinders;
    __u32 num_default_heads;
    __u32 sectors_per_track;
    __u64 number_of_sectors;
    __u16 bytes_per_sector;
    __u32 dpte_ptr;
    __u16 key;
    __u8 device_path_info_length;
    __u8 reserved2;
    __u16 reserved3;
    __u8 host_bus_type[4];
    __u8 interface_type[8];
    union (anon) interface_path;
    union (anon) device_path;
    __u8 reserved4;
    __u8 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct edd_device_params {
    __u16 length;
    __u16 info_flags;
    __u32 num_default_cylinders;
    __u32 num_default_heads;
    __u32 sectors_per_track;
    __u64 number_of_sectors;
    __u16 bytes_per_sector;
    __u32 dpte_ptr;
    __u16 key;
    __u8 device_path_info_length;
    __u8 reserved2;
    __u16 reserved3;
    __u8 host_bus_type[4];
    __u8 interface_type[8];
    union (anon) interface_path;
    union (anon) device_path;
    __u8 reserved4;
    __u8 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct edd_device_params {
    __u16 length;
    __u16 info_flags;
    __u32 num_default_cylinders;
    __u32 num_default_heads;
    __u32 sectors_per_track;
    __u64 number_of_sectors;
    __u16 bytes_per_sector;
    __u32 dpte_ptr;
    __u16 key;
    __u8 device_path_info_length;
    __u8 reserved2;
    __u16 reserved3;
    __u8 host_bus_type[4];
    __u8 interface_type[8];
    union (anon) interface_path;
    union (anon) device_path;
    __u8 reserved4;
    __u8 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct edd_device_params {
    __u16 length;
    __u16 info_flags;
    __u32 num_default_cylinders;
    __u32 num_default_heads;
    __u32 sectors_per_track;
    __u64 number_of_sectors;
    __u16 bytes_per_sector;
    __u32 dpte_ptr;
    __u16 key;
    __u8 device_path_info_length;
    __u8 reserved2;
    __u16 reserved3;
    __u8 host_bus_type[4];
    __u8 interface_type[8];
    union (anon) interface_path;
    union (anon) device_path;
    __u8 reserved4;
    __u8 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct edd_device_params {
    __u16 length;
    __u16 info_flags;
    __u32 num_default_cylinders;
    __u32 num_default_heads;
    __u32 sectors_per_track;
    __u64 number_of_sectors;
    __u16 bytes_per_sector;
    __u32 dpte_ptr;
    __u16 key;
    __u8 device_path_info_length;
    __u8 reserved2;
    __u16 reserved3;
    __u8 host_bus_type[4];
    __u8 interface_type[8];
    union (anon) interface_path;
    union (anon) device_path;
    __u8 reserved4;
    __u8 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct edd_device_params {
    __u16 length;
    __u16 info_flags;
    __u32 num_default_cylinders;
    __u32 num_default_heads;
    __u32 sectors_per_track;
    __u64 number_of_sectors;
    __u16 bytes_per_sector;
    __u32 dpte_ptr;
    __u16 key;
    __u8 device_path_info_length;
    __u8 reserved2;
    __u16 reserved3;
    __u8 host_bus_type[4];
    __u8 interface_type[8];
    union (anon) interface_path;
    union (anon) device_path;
    __u8 reserved4;
    __u8 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct edd_device_params {
    __u16 length;
    __u16 info_flags;
    __u32 num_default_cylinders;
    __u32 num_default_heads;
    __u32 sectors_per_track;
    __u64 number_of_sectors;
    __u16 bytes_per_sector;
    __u32 dpte_ptr;
    __u16 key;
    __u8 device_path_info_length;
    __u8 reserved2;
    __u16 reserved3;
    __u8 host_bus_type[4];
    __u8 interface_type[8];
    union (anon) interface_path;
    union (anon) device_path;
    __u8 reserved4;
    __u8 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct edd_device_params {
    __u16 length;
    __u16 info_flags;
    __u32 num_default_cylinders;
    __u32 num_default_heads;
    __u32 sectors_per_track;
    __u64 number_of_sectors;
    __u16 bytes_per_sector;
    __u32 dpte_ptr;
    __u16 key;
    __u8 device_path_info_length;
    __u8 reserved2;
    __u16 reserved3;
    __u8 host_bus_type[4];
    __u8 interface_type[8];
    union (anon) interface_path;
    union (anon) device_path;
    __u8 reserved4;
    __u8 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct edd_device_params {
    __u16 length;
    __u16 info_flags;
    __u32 num_default_cylinders;
    __u32 num_default_heads;
    __u32 sectors_per_track;
    __u64 number_of_sectors;
    __u16 bytes_per_sector;
    __u32 dpte_ptr;
    __u16 key;
    __u8 device_path_info_length;
    __u8 reserved2;
    __u16 reserved3;
    __u8 host_bus_type[4];
    __u8 interface_type[8];
    union (anon) interface_path;
    union (anon) device_path;
    __u8 reserved4;
    __u8 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct edd_device_params {
    __u16 length;
    __u16 info_flags;
    __u32 num_default_cylinders;
    __u32 num_default_heads;
    __u32 sectors_per_track;
    __u64 number_of_sectors;
    __u16 bytes_per_sector;
    __u32 dpte_ptr;
    __u16 key;
    __u8 device_path_info_length;
    __u8 reserved2;
    __u16 reserved3;
    __u8 host_bus_type[4];
    __u8 interface_type[8];
    union (anon) interface_path;
    union (anon) device_path;
    __u8 reserved4;
    __u8 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct edd_device_params {
    __u16 length;
    __u16 info_flags;
    __u32 num_default_cylinders;
    __u32 num_default_heads;
    __u32 sectors_per_track;
    __u64 number_of_sectors;
    __u16 bytes_per_sector;
    __u32 dpte_ptr;
    __u16 key;
    __u8 device_path_info_length;
    __u8 reserved2;
    __u16 reserved3;
    __u8 host_bus_type[4];
    __u8 interface_type[8];
    union (anon) interface_path;
    union (anon) device_path;
    __u8 reserved4;
    __u8 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct edd_device_params {
    __u16 length;
    __u16 info_flags;
    __u32 num_default_cylinders;
    __u32 num_default_heads;
    __u32 sectors_per_track;
    __u64 number_of_sectors;
    __u16 bytes_per_sector;
    __u32 dpte_ptr;
    __u16 key;
    __u8 device_path_info_length;
    __u8 reserved2;
    __u16 reserved3;
    __u8 host_bus_type[4];
    __u8 interface_type[8];
    union (anon) interface_path;
    union (anon) device_path;
    __u8 reserved4;
    __u8 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct edd_device_params {
    __u16 length;
    __u16 info_flags;
    __u32 num_default_cylinders;
    __u32 num_default_heads;
    __u32 sectors_per_track;
    __u64 number_of_sectors;
    __u16 bytes_per_sector;
    __u32 dpte_ptr;
    __u16 key;
    __u8 device_path_info_length;
    __u8 reserved2;
    __u16 reserved3;
    __u8 host_bus_type[4];
    __u8 interface_type[8];
    union (anon) interface_path;
    union (anon) device_path;
    __u8 reserved4;
    __u8 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct edd_device_params {
    __u16 length;
    __u16 info_flags;
    __u32 num_default_cylinders;
    __u32 num_default_heads;
    __u32 sectors_per_track;
    __u64 number_of_sectors;
    __u16 bytes_per_sector;
    __u32 dpte_ptr;
    __u16 key;
    __u8 device_path_info_length;
    __u8 reserved2;
    __u16 reserved3;
    __u8 host_bus_type[4];
    __u8 interface_type[8];
    union (anon) interface_path;
    union (anon) device_path;
    __u8 reserved4;
    __u8 checksum;
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
struct edd_device_params {
    __u16 length;
    __u16 info_flags;
    __u32 num_default_cylinders;
    __u32 num_default_heads;
    __u32 sectors_per_track;
    __u64 number_of_sectors;
    __u16 bytes_per_sector;
    __u32 dpte_ptr;
    __u16 key;
    __u8 device_path_info_length;
    __u8 reserved2;
    __u16 reserved3;
    __u8 host_bus_type[4];
    __u8 interface_type[8];
    union (anon) interface_path;
    union (anon) device_path;
    __u8 reserved4;
    __u8 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct edd_device_params {
    __u16 length;
    __u16 info_flags;
    __u32 num_default_cylinders;
    __u32 num_default_heads;
    __u32 sectors_per_track;
    __u64 number_of_sectors;
    __u16 bytes_per_sector;
    __u32 dpte_ptr;
    __u16 key;
    __u8 device_path_info_length;
    __u8 reserved2;
    __u16 reserved3;
    __u8 host_bus_type[4];
    __u8 interface_type[8];
    union (anon) interface_path;
    union (anon) device_path;
    __u8 reserved4;
    __u8 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct edd_device_params {
    __u16 length;
    __u16 info_flags;
    __u32 num_default_cylinders;
    __u32 num_default_heads;
    __u32 sectors_per_track;
    __u64 number_of_sectors;
    __u16 bytes_per_sector;
    __u32 dpte_ptr;
    __u16 key;
    __u8 device_path_info_length;
    __u8 reserved2;
    __u16 reserved3;
    __u8 host_bus_type[4];
    __u8 interface_type[8];
    union (anon) interface_path;
    union (anon) device_path;
    __u8 reserved4;
    __u8 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct edd_device_params {
    __u16 length;
    __u16 info_flags;
    __u32 num_default_cylinders;
    __u32 num_default_heads;
    __u32 sectors_per_track;
    __u64 number_of_sectors;
    __u16 bytes_per_sector;
    __u32 dpte_ptr;
    __u16 key;
    __u8 device_path_info_length;
    __u8 reserved2;
    __u16 reserved3;
    __u8 host_bus_type[4];
    __u8 interface_type[8];
    union (anon) interface_path;
    union (anon) device_path;
    __u8 reserved4;
    __u8 checksum;
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
