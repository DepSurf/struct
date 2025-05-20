# Struct: <code>setup_header</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct setup_header {
    __u8 setup_sects;
    __u16 root_flags;
    __u32 syssize;
    __u16 ram_size;
    __u16 vid_mode;
    __u16 root_dev;
    __u16 boot_flag;
    __u16 jump;
    __u32 header;
    __u16 version;
    __u32 realmode_swtch;
    __u16 start_sys;
    __u16 kernel_version;
    __u8 type_of_loader;
    __u8 loadflags;
    __u16 setup_move_size;
    __u32 code32_start;
    __u32 ramdisk_image;
    __u32 ramdisk_size;
    __u32 bootsect_kludge;
    __u16 heap_end_ptr;
    __u8 ext_loader_ver;
    __u8 ext_loader_type;
    __u32 cmd_line_ptr;
    __u32 initrd_addr_max;
    __u32 kernel_alignment;
    __u8 relocatable_kernel;
    __u8 min_alignment;
    __u16 xloadflags;
    __u32 cmdline_size;
    __u32 hardware_subarch;
    __u64 hardware_subarch_data;
    __u32 payload_offset;
    __u32 payload_length;
    __u64 setup_data;
    __u64 pref_address;
    __u32 init_size;
    __u32 handover_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct setup_header {
    __u8 setup_sects;
    __u16 root_flags;
    __u32 syssize;
    __u16 ram_size;
    __u16 vid_mode;
    __u16 root_dev;
    __u16 boot_flag;
    __u16 jump;
    __u32 header;
    __u16 version;
    __u32 realmode_swtch;
    __u16 start_sys;
    __u16 kernel_version;
    __u8 type_of_loader;
    __u8 loadflags;
    __u16 setup_move_size;
    __u32 code32_start;
    __u32 ramdisk_image;
    __u32 ramdisk_size;
    __u32 bootsect_kludge;
    __u16 heap_end_ptr;
    __u8 ext_loader_ver;
    __u8 ext_loader_type;
    __u32 cmd_line_ptr;
    __u32 initrd_addr_max;
    __u32 kernel_alignment;
    __u8 relocatable_kernel;
    __u8 min_alignment;
    __u16 xloadflags;
    __u32 cmdline_size;
    __u32 hardware_subarch;
    __u64 hardware_subarch_data;
    __u32 payload_offset;
    __u32 payload_length;
    __u64 setup_data;
    __u64 pref_address;
    __u32 init_size;
    __u32 handover_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct setup_header {
    __u8 setup_sects;
    __u16 root_flags;
    __u32 syssize;
    __u16 ram_size;
    __u16 vid_mode;
    __u16 root_dev;
    __u16 boot_flag;
    __u16 jump;
    __u32 header;
    __u16 version;
    __u32 realmode_swtch;
    __u16 start_sys;
    __u16 kernel_version;
    __u8 type_of_loader;
    __u8 loadflags;
    __u16 setup_move_size;
    __u32 code32_start;
    __u32 ramdisk_image;
    __u32 ramdisk_size;
    __u32 bootsect_kludge;
    __u16 heap_end_ptr;
    __u8 ext_loader_ver;
    __u8 ext_loader_type;
    __u32 cmd_line_ptr;
    __u32 initrd_addr_max;
    __u32 kernel_alignment;
    __u8 relocatable_kernel;
    __u8 min_alignment;
    __u16 xloadflags;
    __u32 cmdline_size;
    __u32 hardware_subarch;
    __u64 hardware_subarch_data;
    __u32 payload_offset;
    __u32 payload_length;
    __u64 setup_data;
    __u64 pref_address;
    __u32 init_size;
    __u32 handover_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct setup_header {
    __u8 setup_sects;
    __u16 root_flags;
    __u32 syssize;
    __u16 ram_size;
    __u16 vid_mode;
    __u16 root_dev;
    __u16 boot_flag;
    __u16 jump;
    __u32 header;
    __u16 version;
    __u32 realmode_swtch;
    __u16 start_sys_seg;
    __u16 kernel_version;
    __u8 type_of_loader;
    __u8 loadflags;
    __u16 setup_move_size;
    __u32 code32_start;
    __u32 ramdisk_image;
    __u32 ramdisk_size;
    __u32 bootsect_kludge;
    __u16 heap_end_ptr;
    __u8 ext_loader_ver;
    __u8 ext_loader_type;
    __u32 cmd_line_ptr;
    __u32 initrd_addr_max;
    __u32 kernel_alignment;
    __u8 relocatable_kernel;
    __u8 min_alignment;
    __u16 xloadflags;
    __u32 cmdline_size;
    __u32 hardware_subarch;
    __u64 hardware_subarch_data;
    __u32 payload_offset;
    __u32 payload_length;
    __u64 setup_data;
    __u64 pref_address;
    __u32 init_size;
    __u32 handover_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct setup_header {
    __u8 setup_sects;
    __u16 root_flags;
    __u32 syssize;
    __u16 ram_size;
    __u16 vid_mode;
    __u16 root_dev;
    __u16 boot_flag;
    __u16 jump;
    __u32 header;
    __u16 version;
    __u32 realmode_swtch;
    __u16 start_sys_seg;
    __u16 kernel_version;
    __u8 type_of_loader;
    __u8 loadflags;
    __u16 setup_move_size;
    __u32 code32_start;
    __u32 ramdisk_image;
    __u32 ramdisk_size;
    __u32 bootsect_kludge;
    __u16 heap_end_ptr;
    __u8 ext_loader_ver;
    __u8 ext_loader_type;
    __u32 cmd_line_ptr;
    __u32 initrd_addr_max;
    __u32 kernel_alignment;
    __u8 relocatable_kernel;
    __u8 min_alignment;
    __u16 xloadflags;
    __u32 cmdline_size;
    __u32 hardware_subarch;
    __u64 hardware_subarch_data;
    __u32 payload_offset;
    __u32 payload_length;
    __u64 setup_data;
    __u64 pref_address;
    __u32 init_size;
    __u32 handover_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct setup_header {
    __u8 setup_sects;
    __u16 root_flags;
    __u32 syssize;
    __u16 ram_size;
    __u16 vid_mode;
    __u16 root_dev;
    __u16 boot_flag;
    __u16 jump;
    __u32 header;
    __u16 version;
    __u32 realmode_swtch;
    __u16 start_sys_seg;
    __u16 kernel_version;
    __u8 type_of_loader;
    __u8 loadflags;
    __u16 setup_move_size;
    __u32 code32_start;
    __u32 ramdisk_image;
    __u32 ramdisk_size;
    __u32 bootsect_kludge;
    __u16 heap_end_ptr;
    __u8 ext_loader_ver;
    __u8 ext_loader_type;
    __u32 cmd_line_ptr;
    __u32 initrd_addr_max;
    __u32 kernel_alignment;
    __u8 relocatable_kernel;
    __u8 min_alignment;
    __u16 xloadflags;
    __u32 cmdline_size;
    __u32 hardware_subarch;
    __u64 hardware_subarch_data;
    __u32 payload_offset;
    __u32 payload_length;
    __u64 setup_data;
    __u64 pref_address;
    __u32 init_size;
    __u32 handover_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct setup_header {
    __u8 setup_sects;
    __u16 root_flags;
    __u32 syssize;
    __u16 ram_size;
    __u16 vid_mode;
    __u16 root_dev;
    __u16 boot_flag;
    __u16 jump;
    __u32 header;
    __u16 version;
    __u32 realmode_swtch;
    __u16 start_sys_seg;
    __u16 kernel_version;
    __u8 type_of_loader;
    __u8 loadflags;
    __u16 setup_move_size;
    __u32 code32_start;
    __u32 ramdisk_image;
    __u32 ramdisk_size;
    __u32 bootsect_kludge;
    __u16 heap_end_ptr;
    __u8 ext_loader_ver;
    __u8 ext_loader_type;
    __u32 cmd_line_ptr;
    __u32 initrd_addr_max;
    __u32 kernel_alignment;
    __u8 relocatable_kernel;
    __u8 min_alignment;
    __u16 xloadflags;
    __u32 cmdline_size;
    __u32 hardware_subarch;
    __u64 hardware_subarch_data;
    __u32 payload_offset;
    __u32 payload_length;
    __u64 setup_data;
    __u64 pref_address;
    __u32 init_size;
    __u32 handover_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct setup_header {
    __u8 setup_sects;
    __u16 root_flags;
    __u32 syssize;
    __u16 ram_size;
    __u16 vid_mode;
    __u16 root_dev;
    __u16 boot_flag;
    __u16 jump;
    __u32 header;
    __u16 version;
    __u32 realmode_swtch;
    __u16 start_sys_seg;
    __u16 kernel_version;
    __u8 type_of_loader;
    __u8 loadflags;
    __u16 setup_move_size;
    __u32 code32_start;
    __u32 ramdisk_image;
    __u32 ramdisk_size;
    __u32 bootsect_kludge;
    __u16 heap_end_ptr;
    __u8 ext_loader_ver;
    __u8 ext_loader_type;
    __u32 cmd_line_ptr;
    __u32 initrd_addr_max;
    __u32 kernel_alignment;
    __u8 relocatable_kernel;
    __u8 min_alignment;
    __u16 xloadflags;
    __u32 cmdline_size;
    __u32 hardware_subarch;
    __u64 hardware_subarch_data;
    __u32 payload_offset;
    __u32 payload_length;
    __u64 setup_data;
    __u64 pref_address;
    __u32 init_size;
    __u32 handover_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct setup_header {
    __u8 setup_sects;
    __u16 root_flags;
    __u32 syssize;
    __u16 ram_size;
    __u16 vid_mode;
    __u16 root_dev;
    __u16 boot_flag;
    __u16 jump;
    __u32 header;
    __u16 version;
    __u32 realmode_swtch;
    __u16 start_sys_seg;
    __u16 kernel_version;
    __u8 type_of_loader;
    __u8 loadflags;
    __u16 setup_move_size;
    __u32 code32_start;
    __u32 ramdisk_image;
    __u32 ramdisk_size;
    __u32 bootsect_kludge;
    __u16 heap_end_ptr;
    __u8 ext_loader_ver;
    __u8 ext_loader_type;
    __u32 cmd_line_ptr;
    __u32 initrd_addr_max;
    __u32 kernel_alignment;
    __u8 relocatable_kernel;
    __u8 min_alignment;
    __u16 xloadflags;
    __u32 cmdline_size;
    __u32 hardware_subarch;
    __u64 hardware_subarch_data;
    __u32 payload_offset;
    __u32 payload_length;
    __u64 setup_data;
    __u64 pref_address;
    __u32 init_size;
    __u32 handover_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct setup_header {
    __u8 setup_sects;
    __u16 root_flags;
    __u32 syssize;
    __u16 ram_size;
    __u16 vid_mode;
    __u16 root_dev;
    __u16 boot_flag;
    __u16 jump;
    __u32 header;
    __u16 version;
    __u32 realmode_swtch;
    __u16 start_sys_seg;
    __u16 kernel_version;
    __u8 type_of_loader;
    __u8 loadflags;
    __u16 setup_move_size;
    __u32 code32_start;
    __u32 ramdisk_image;
    __u32 ramdisk_size;
    __u32 bootsect_kludge;
    __u16 heap_end_ptr;
    __u8 ext_loader_ver;
    __u8 ext_loader_type;
    __u32 cmd_line_ptr;
    __u32 initrd_addr_max;
    __u32 kernel_alignment;
    __u8 relocatable_kernel;
    __u8 min_alignment;
    __u16 xloadflags;
    __u32 cmdline_size;
    __u32 hardware_subarch;
    __u64 hardware_subarch_data;
    __u32 payload_offset;
    __u32 payload_length;
    __u64 setup_data;
    __u64 pref_address;
    __u32 init_size;
    __u32 handover_offset;
    __u32 kernel_info_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct setup_header {
    __u8 setup_sects;
    __u16 root_flags;
    __u32 syssize;
    __u16 ram_size;
    __u16 vid_mode;
    __u16 root_dev;
    __u16 boot_flag;
    __u16 jump;
    __u32 header;
    __u16 version;
    __u32 realmode_swtch;
    __u16 start_sys_seg;
    __u16 kernel_version;
    __u8 type_of_loader;
    __u8 loadflags;
    __u16 setup_move_size;
    __u32 code32_start;
    __u32 ramdisk_image;
    __u32 ramdisk_size;
    __u32 bootsect_kludge;
    __u16 heap_end_ptr;
    __u8 ext_loader_ver;
    __u8 ext_loader_type;
    __u32 cmd_line_ptr;
    __u32 initrd_addr_max;
    __u32 kernel_alignment;
    __u8 relocatable_kernel;
    __u8 min_alignment;
    __u16 xloadflags;
    __u32 cmdline_size;
    __u32 hardware_subarch;
    __u64 hardware_subarch_data;
    __u32 payload_offset;
    __u32 payload_length;
    __u64 setup_data;
    __u64 pref_address;
    __u32 init_size;
    __u32 handover_offset;
    __u32 kernel_info_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct setup_header {
    __u8 setup_sects;
    __u16 root_flags;
    __u32 syssize;
    __u16 ram_size;
    __u16 vid_mode;
    __u16 root_dev;
    __u16 boot_flag;
    __u16 jump;
    __u32 header;
    __u16 version;
    __u32 realmode_swtch;
    __u16 start_sys_seg;
    __u16 kernel_version;
    __u8 type_of_loader;
    __u8 loadflags;
    __u16 setup_move_size;
    __u32 code32_start;
    __u32 ramdisk_image;
    __u32 ramdisk_size;
    __u32 bootsect_kludge;
    __u16 heap_end_ptr;
    __u8 ext_loader_ver;
    __u8 ext_loader_type;
    __u32 cmd_line_ptr;
    __u32 initrd_addr_max;
    __u32 kernel_alignment;
    __u8 relocatable_kernel;
    __u8 min_alignment;
    __u16 xloadflags;
    __u32 cmdline_size;
    __u32 hardware_subarch;
    __u64 hardware_subarch_data;
    __u32 payload_offset;
    __u32 payload_length;
    __u64 setup_data;
    __u64 pref_address;
    __u32 init_size;
    __u32 handover_offset;
    __u32 kernel_info_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct setup_header {
    __u8 setup_sects;
    __u16 root_flags;
    __u32 syssize;
    __u16 ram_size;
    __u16 vid_mode;
    __u16 root_dev;
    __u16 boot_flag;
    __u16 jump;
    __u32 header;
    __u16 version;
    __u32 realmode_swtch;
    __u16 start_sys_seg;
    __u16 kernel_version;
    __u8 type_of_loader;
    __u8 loadflags;
    __u16 setup_move_size;
    __u32 code32_start;
    __u32 ramdisk_image;
    __u32 ramdisk_size;
    __u32 bootsect_kludge;
    __u16 heap_end_ptr;
    __u8 ext_loader_ver;
    __u8 ext_loader_type;
    __u32 cmd_line_ptr;
    __u32 initrd_addr_max;
    __u32 kernel_alignment;
    __u8 relocatable_kernel;
    __u8 min_alignment;
    __u16 xloadflags;
    __u32 cmdline_size;
    __u32 hardware_subarch;
    __u64 hardware_subarch_data;
    __u32 payload_offset;
    __u32 payload_length;
    __u64 setup_data;
    __u64 pref_address;
    __u32 init_size;
    __u32 handover_offset;
    __u32 kernel_info_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct setup_header {
    __u8 setup_sects;
    __u16 root_flags;
    __u32 syssize;
    __u16 ram_size;
    __u16 vid_mode;
    __u16 root_dev;
    __u16 boot_flag;
    __u16 jump;
    __u32 header;
    __u16 version;
    __u32 realmode_swtch;
    __u16 start_sys_seg;
    __u16 kernel_version;
    __u8 type_of_loader;
    __u8 loadflags;
    __u16 setup_move_size;
    __u32 code32_start;
    __u32 ramdisk_image;
    __u32 ramdisk_size;
    __u32 bootsect_kludge;
    __u16 heap_end_ptr;
    __u8 ext_loader_ver;
    __u8 ext_loader_type;
    __u32 cmd_line_ptr;
    __u32 initrd_addr_max;
    __u32 kernel_alignment;
    __u8 relocatable_kernel;
    __u8 min_alignment;
    __u16 xloadflags;
    __u32 cmdline_size;
    __u32 hardware_subarch;
    __u64 hardware_subarch_data;
    __u32 payload_offset;
    __u32 payload_length;
    __u64 setup_data;
    __u64 pref_address;
    __u32 init_size;
    __u32 handover_offset;
    __u32 kernel_info_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct setup_header {
    __u8 setup_sects;
    __u16 root_flags;
    __u32 syssize;
    __u16 ram_size;
    __u16 vid_mode;
    __u16 root_dev;
    __u16 boot_flag;
    __u16 jump;
    __u32 header;
    __u16 version;
    __u32 realmode_swtch;
    __u16 start_sys_seg;
    __u16 kernel_version;
    __u8 type_of_loader;
    __u8 loadflags;
    __u16 setup_move_size;
    __u32 code32_start;
    __u32 ramdisk_image;
    __u32 ramdisk_size;
    __u32 bootsect_kludge;
    __u16 heap_end_ptr;
    __u8 ext_loader_ver;
    __u8 ext_loader_type;
    __u32 cmd_line_ptr;
    __u32 initrd_addr_max;
    __u32 kernel_alignment;
    __u8 relocatable_kernel;
    __u8 min_alignment;
    __u16 xloadflags;
    __u32 cmdline_size;
    __u32 hardware_subarch;
    __u64 hardware_subarch_data;
    __u32 payload_offset;
    __u32 payload_length;
    __u64 setup_data;
    __u64 pref_address;
    __u32 init_size;
    __u32 handover_offset;
    __u32 kernel_info_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct setup_header {
    __u8 setup_sects;
    __u16 root_flags;
    __u32 syssize;
    __u16 ram_size;
    __u16 vid_mode;
    __u16 root_dev;
    __u16 boot_flag;
    __u16 jump;
    __u32 header;
    __u16 version;
    __u32 realmode_swtch;
    __u16 start_sys_seg;
    __u16 kernel_version;
    __u8 type_of_loader;
    __u8 loadflags;
    __u16 setup_move_size;
    __u32 code32_start;
    __u32 ramdisk_image;
    __u32 ramdisk_size;
    __u32 bootsect_kludge;
    __u16 heap_end_ptr;
    __u8 ext_loader_ver;
    __u8 ext_loader_type;
    __u32 cmd_line_ptr;
    __u32 initrd_addr_max;
    __u32 kernel_alignment;
    __u8 relocatable_kernel;
    __u8 min_alignment;
    __u16 xloadflags;
    __u32 cmdline_size;
    __u32 hardware_subarch;
    __u64 hardware_subarch_data;
    __u32 payload_offset;
    __u32 payload_length;
    __u64 setup_data;
    __u64 pref_address;
    __u32 init_size;
    __u32 handover_offset;
    __u32 kernel_info_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct setup_header {
    __u8 setup_sects;
    __u16 root_flags;
    __u32 syssize;
    __u16 ram_size;
    __u16 vid_mode;
    __u16 root_dev;
    __u16 boot_flag;
    __u16 jump;
    __u32 header;
    __u16 version;
    __u32 realmode_swtch;
    __u16 start_sys_seg;
    __u16 kernel_version;
    __u8 type_of_loader;
    __u8 loadflags;
    __u16 setup_move_size;
    __u32 code32_start;
    __u32 ramdisk_image;
    __u32 ramdisk_size;
    __u32 bootsect_kludge;
    __u16 heap_end_ptr;
    __u8 ext_loader_ver;
    __u8 ext_loader_type;
    __u32 cmd_line_ptr;
    __u32 initrd_addr_max;
    __u32 kernel_alignment;
    __u8 relocatable_kernel;
    __u8 min_alignment;
    __u16 xloadflags;
    __u32 cmdline_size;
    __u32 hardware_subarch;
    __u64 hardware_subarch_data;
    __u32 payload_offset;
    __u32 payload_length;
    __u64 setup_data;
    __u64 pref_address;
    __u32 init_size;
    __u32 handover_offset;
    __u32 kernel_info_offset;
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
struct setup_header {
    __u8 setup_sects;
    __u16 root_flags;
    __u32 syssize;
    __u16 ram_size;
    __u16 vid_mode;
    __u16 root_dev;
    __u16 boot_flag;
    __u16 jump;
    __u32 header;
    __u16 version;
    __u32 realmode_swtch;
    __u16 start_sys_seg;
    __u16 kernel_version;
    __u8 type_of_loader;
    __u8 loadflags;
    __u16 setup_move_size;
    __u32 code32_start;
    __u32 ramdisk_image;
    __u32 ramdisk_size;
    __u32 bootsect_kludge;
    __u16 heap_end_ptr;
    __u8 ext_loader_ver;
    __u8 ext_loader_type;
    __u32 cmd_line_ptr;
    __u32 initrd_addr_max;
    __u32 kernel_alignment;
    __u8 relocatable_kernel;
    __u8 min_alignment;
    __u16 xloadflags;
    __u32 cmdline_size;
    __u32 hardware_subarch;
    __u64 hardware_subarch_data;
    __u32 payload_offset;
    __u32 payload_length;
    __u64 setup_data;
    __u64 pref_address;
    __u32 init_size;
    __u32 handover_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct setup_header {
    __u8 setup_sects;
    __u16 root_flags;
    __u32 syssize;
    __u16 ram_size;
    __u16 vid_mode;
    __u16 root_dev;
    __u16 boot_flag;
    __u16 jump;
    __u32 header;
    __u16 version;
    __u32 realmode_swtch;
    __u16 start_sys_seg;
    __u16 kernel_version;
    __u8 type_of_loader;
    __u8 loadflags;
    __u16 setup_move_size;
    __u32 code32_start;
    __u32 ramdisk_image;
    __u32 ramdisk_size;
    __u32 bootsect_kludge;
    __u16 heap_end_ptr;
    __u8 ext_loader_ver;
    __u8 ext_loader_type;
    __u32 cmd_line_ptr;
    __u32 initrd_addr_max;
    __u32 kernel_alignment;
    __u8 relocatable_kernel;
    __u8 min_alignment;
    __u16 xloadflags;
    __u32 cmdline_size;
    __u32 hardware_subarch;
    __u64 hardware_subarch_data;
    __u32 payload_offset;
    __u32 payload_length;
    __u64 setup_data;
    __u64 pref_address;
    __u32 init_size;
    __u32 handover_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct setup_header {
    __u8 setup_sects;
    __u16 root_flags;
    __u32 syssize;
    __u16 ram_size;
    __u16 vid_mode;
    __u16 root_dev;
    __u16 boot_flag;
    __u16 jump;
    __u32 header;
    __u16 version;
    __u32 realmode_swtch;
    __u16 start_sys_seg;
    __u16 kernel_version;
    __u8 type_of_loader;
    __u8 loadflags;
    __u16 setup_move_size;
    __u32 code32_start;
    __u32 ramdisk_image;
    __u32 ramdisk_size;
    __u32 bootsect_kludge;
    __u16 heap_end_ptr;
    __u8 ext_loader_ver;
    __u8 ext_loader_type;
    __u32 cmd_line_ptr;
    __u32 initrd_addr_max;
    __u32 kernel_alignment;
    __u8 relocatable_kernel;
    __u8 min_alignment;
    __u16 xloadflags;
    __u32 cmdline_size;
    __u32 hardware_subarch;
    __u64 hardware_subarch_data;
    __u32 payload_offset;
    __u32 payload_length;
    __u64 setup_data;
    __u64 pref_address;
    __u32 init_size;
    __u32 handover_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct setup_header {
    __u8 setup_sects;
    __u16 root_flags;
    __u32 syssize;
    __u16 ram_size;
    __u16 vid_mode;
    __u16 root_dev;
    __u16 boot_flag;
    __u16 jump;
    __u32 header;
    __u16 version;
    __u32 realmode_swtch;
    __u16 start_sys_seg;
    __u16 kernel_version;
    __u8 type_of_loader;
    __u8 loadflags;
    __u16 setup_move_size;
    __u32 code32_start;
    __u32 ramdisk_image;
    __u32 ramdisk_size;
    __u32 bootsect_kludge;
    __u16 heap_end_ptr;
    __u8 ext_loader_ver;
    __u8 ext_loader_type;
    __u32 cmd_line_ptr;
    __u32 initrd_addr_max;
    __u32 kernel_alignment;
    __u8 relocatable_kernel;
    __u8 min_alignment;
    __u16 xloadflags;
    __u32 cmdline_size;
    __u32 hardware_subarch;
    __u64 hardware_subarch_data;
    __u32 payload_offset;
    __u32 payload_length;
    __u64 setup_data;
    __u64 pref_address;
    __u32 init_size;
    __u32 handover_offset;
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
<code>__u16 start_sys_seg</code>
</li>
<li>
<b>Field removed. </b>
<code>__u16 start_sys</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u32 kernel_info_offset</code>
</li>
</ul>
</details>
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
