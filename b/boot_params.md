# Struct: <code>boot_params</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct boot_params {
    struct screen_info screen_info;
    struct apm_bios_info apm_bios_info;
    __u8 _pad2[4];
    __u64 tboot_addr;
    struct ist_info ist_info;
    __u8 _pad3[16];
    __u8 hd0_info[16];
    __u8 hd1_info[16];
    struct sys_desc_table sys_desc_table;
    struct olpc_ofw_header olpc_ofw_header;
    __u32 ext_ramdisk_image;
    __u32 ext_ramdisk_size;
    __u32 ext_cmd_line_ptr;
    __u8 _pad4[116];
    struct edid_info edid_info;
    struct efi_info efi_info;
    __u32 alt_mem_k;
    __u32 scratch;
    __u8 e820_entries;
    __u8 eddbuf_entries;
    __u8 edd_mbr_sig_buf_entries;
    __u8 kbd_status;
    __u8 secure_boot;
    __u8 _pad5[2];
    __u8 sentinel;
    __u8 _pad6[1];
    struct setup_header hdr;
    __u8 _pad7[40];
    __u32 edd_mbr_sig_buffer[16];
    struct e820entry e820_map[128];
    __u8 _pad8[48];
    struct edd_info eddbuf[6];
    __u8 _pad9[276];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct boot_params {
    struct screen_info screen_info;
    struct apm_bios_info apm_bios_info;
    __u8 _pad2[4];
    __u64 tboot_addr;
    struct ist_info ist_info;
    __u8 _pad3[16];
    __u8 hd0_info[16];
    __u8 hd1_info[16];
    struct sys_desc_table sys_desc_table;
    struct olpc_ofw_header olpc_ofw_header;
    __u32 ext_ramdisk_image;
    __u32 ext_ramdisk_size;
    __u32 ext_cmd_line_ptr;
    __u8 _pad4[116];
    struct edid_info edid_info;
    struct efi_info efi_info;
    __u32 alt_mem_k;
    __u32 scratch;
    __u8 e820_entries;
    __u8 eddbuf_entries;
    __u8 edd_mbr_sig_buf_entries;
    __u8 kbd_status;
    __u8 secure_boot;
    __u8 _pad5[2];
    __u8 sentinel;
    __u8 _pad6[1];
    struct setup_header hdr;
    __u8 _pad7[40];
    __u32 edd_mbr_sig_buffer[16];
    struct e820entry e820_map[128];
    __u8 _pad8[48];
    struct edd_info eddbuf[6];
    __u8 _pad9[276];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct boot_params {
    struct screen_info screen_info;
    struct apm_bios_info apm_bios_info;
    __u8 _pad2[4];
    __u64 tboot_addr;
    struct ist_info ist_info;
    __u8 _pad3[16];
    __u8 hd0_info[16];
    __u8 hd1_info[16];
    struct sys_desc_table sys_desc_table;
    struct olpc_ofw_header olpc_ofw_header;
    __u32 ext_ramdisk_image;
    __u32 ext_ramdisk_size;
    __u32 ext_cmd_line_ptr;
    __u8 _pad4[116];
    struct edid_info edid_info;
    struct efi_info efi_info;
    __u32 alt_mem_k;
    __u32 scratch;
    __u8 e820_entries;
    __u8 eddbuf_entries;
    __u8 edd_mbr_sig_buf_entries;
    __u8 kbd_status;
    __u8 secure_boot;
    __u8 _pad5[2];
    __u8 sentinel;
    __u8 _pad6[1];
    struct setup_header hdr;
    __u8 _pad7[40];
    __u32 edd_mbr_sig_buffer[16];
    struct e820entry e820_map[128];
    __u8 _pad8[48];
    struct edd_info eddbuf[6];
    __u8 _pad9[276];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct boot_params {
    struct screen_info screen_info;
    struct apm_bios_info apm_bios_info;
    __u8 _pad2[4];
    __u64 tboot_addr;
    struct ist_info ist_info;
    __u8 _pad3[16];
    __u8 hd0_info[16];
    __u8 hd1_info[16];
    struct sys_desc_table sys_desc_table;
    struct olpc_ofw_header olpc_ofw_header;
    __u32 ext_ramdisk_image;
    __u32 ext_ramdisk_size;
    __u32 ext_cmd_line_ptr;
    __u8 _pad4[116];
    struct edid_info edid_info;
    struct efi_info efi_info;
    __u32 alt_mem_k;
    __u32 scratch;
    __u8 e820_entries;
    __u8 eddbuf_entries;
    __u8 edd_mbr_sig_buf_entries;
    __u8 kbd_status;
    __u8 secure_boot;
    __u8 _pad5[2];
    __u8 sentinel;
    __u8 _pad6[1];
    struct setup_header hdr;
    __u8 _pad7[40];
    __u32 edd_mbr_sig_buffer[16];
    struct boot_e820_entry e820_table[128];
    __u8 _pad8[48];
    struct edd_info eddbuf[6];
    __u8 _pad9[276];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct boot_params {
    struct screen_info screen_info;
    struct apm_bios_info apm_bios_info;
    __u8 _pad2[4];
    __u64 tboot_addr;
    struct ist_info ist_info;
    __u8 _pad3[16];
    __u8 hd0_info[16];
    __u8 hd1_info[16];
    struct sys_desc_table sys_desc_table;
    struct olpc_ofw_header olpc_ofw_header;
    __u32 ext_ramdisk_image;
    __u32 ext_ramdisk_size;
    __u32 ext_cmd_line_ptr;
    __u8 _pad4[116];
    struct edid_info edid_info;
    struct efi_info efi_info;
    __u32 alt_mem_k;
    __u32 scratch;
    __u8 e820_entries;
    __u8 eddbuf_entries;
    __u8 edd_mbr_sig_buf_entries;
    __u8 kbd_status;
    __u8 secure_boot;
    __u8 _pad5[2];
    __u8 sentinel;
    __u8 _pad6[1];
    struct setup_header hdr;
    __u8 _pad7[40];
    __u32 edd_mbr_sig_buffer[16];
    struct boot_e820_entry e820_table[128];
    __u8 _pad8[48];
    struct edd_info eddbuf[6];
    __u8 _pad9[276];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct boot_params {
    struct screen_info screen_info;
    struct apm_bios_info apm_bios_info;
    __u8 _pad2[4];
    __u64 tboot_addr;
    struct ist_info ist_info;
    __u8 _pad3[16];
    __u8 hd0_info[16];
    __u8 hd1_info[16];
    struct sys_desc_table sys_desc_table;
    struct olpc_ofw_header olpc_ofw_header;
    __u32 ext_ramdisk_image;
    __u32 ext_ramdisk_size;
    __u32 ext_cmd_line_ptr;
    __u8 _pad4[116];
    struct edid_info edid_info;
    struct efi_info efi_info;
    __u32 alt_mem_k;
    __u32 scratch;
    __u8 e820_entries;
    __u8 eddbuf_entries;
    __u8 edd_mbr_sig_buf_entries;
    __u8 kbd_status;
    __u8 secure_boot;
    __u8 _pad5[2];
    __u8 sentinel;
    __u8 _pad6[1];
    struct setup_header hdr;
    __u8 _pad7[40];
    __u32 edd_mbr_sig_buffer[16];
    struct boot_e820_entry e820_table[128];
    __u8 _pad8[48];
    struct edd_info eddbuf[6];
    __u8 _pad9[276];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct boot_params {
    struct screen_info screen_info;
    struct apm_bios_info apm_bios_info;
    __u8 _pad2[4];
    __u64 tboot_addr;
    struct ist_info ist_info;
    __u64 acpi_rsdp_addr;
    __u8 _pad3[8];
    __u8 hd0_info[16];
    __u8 hd1_info[16];
    struct sys_desc_table sys_desc_table;
    struct olpc_ofw_header olpc_ofw_header;
    __u32 ext_ramdisk_image;
    __u32 ext_ramdisk_size;
    __u32 ext_cmd_line_ptr;
    __u8 _pad4[116];
    struct edid_info edid_info;
    struct efi_info efi_info;
    __u32 alt_mem_k;
    __u32 scratch;
    __u8 e820_entries;
    __u8 eddbuf_entries;
    __u8 edd_mbr_sig_buf_entries;
    __u8 kbd_status;
    __u8 secure_boot;
    __u8 _pad5[2];
    __u8 sentinel;
    __u8 _pad6[1];
    struct setup_header hdr;
    __u8 _pad7[40];
    __u32 edd_mbr_sig_buffer[16];
    struct boot_e820_entry e820_table[128];
    __u8 _pad8[48];
    struct edd_info eddbuf[6];
    __u8 _pad9[276];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct boot_params {
    struct screen_info screen_info;
    struct apm_bios_info apm_bios_info;
    __u8 _pad2[4];
    __u64 tboot_addr;
    struct ist_info ist_info;
    __u64 acpi_rsdp_addr;
    __u8 _pad3[8];
    __u8 hd0_info[16];
    __u8 hd1_info[16];
    struct sys_desc_table sys_desc_table;
    struct olpc_ofw_header olpc_ofw_header;
    __u32 ext_ramdisk_image;
    __u32 ext_ramdisk_size;
    __u32 ext_cmd_line_ptr;
    __u8 _pad4[116];
    struct edid_info edid_info;
    struct efi_info efi_info;
    __u32 alt_mem_k;
    __u32 scratch;
    __u8 e820_entries;
    __u8 eddbuf_entries;
    __u8 edd_mbr_sig_buf_entries;
    __u8 kbd_status;
    __u8 secure_boot;
    __u8 _pad5[2];
    __u8 sentinel;
    __u8 _pad6[1];
    struct setup_header hdr;
    __u8 _pad7[40];
    __u32 edd_mbr_sig_buffer[16];
    struct boot_e820_entry e820_table[128];
    __u8 _pad8[48];
    struct edd_info eddbuf[6];
    __u8 _pad9[276];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct boot_params {
    struct screen_info screen_info;
    struct apm_bios_info apm_bios_info;
    __u8 _pad2[4];
    __u64 tboot_addr;
    struct ist_info ist_info;
    __u64 acpi_rsdp_addr;
    __u8 _pad3[8];
    __u8 hd0_info[16];
    __u8 hd1_info[16];
    struct sys_desc_table sys_desc_table;
    struct olpc_ofw_header olpc_ofw_header;
    __u32 ext_ramdisk_image;
    __u32 ext_ramdisk_size;
    __u32 ext_cmd_line_ptr;
    __u8 _pad4[116];
    struct edid_info edid_info;
    struct efi_info efi_info;
    __u32 alt_mem_k;
    __u32 scratch;
    __u8 e820_entries;
    __u8 eddbuf_entries;
    __u8 edd_mbr_sig_buf_entries;
    __u8 kbd_status;
    __u8 secure_boot;
    __u8 _pad5[2];
    __u8 sentinel;
    __u8 _pad6[1];
    struct setup_header hdr;
    __u8 _pad7[40];
    __u32 edd_mbr_sig_buffer[16];
    struct boot_e820_entry e820_table[128];
    __u8 _pad8[48];
    struct edd_info eddbuf[6];
    __u8 _pad9[276];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct boot_params {
    struct screen_info screen_info;
    struct apm_bios_info apm_bios_info;
    __u8 _pad2[4];
    __u64 tboot_addr;
    struct ist_info ist_info;
    __u64 acpi_rsdp_addr;
    __u8 _pad3[8];
    __u8 hd0_info[16];
    __u8 hd1_info[16];
    struct sys_desc_table sys_desc_table;
    struct olpc_ofw_header olpc_ofw_header;
    __u32 ext_ramdisk_image;
    __u32 ext_ramdisk_size;
    __u32 ext_cmd_line_ptr;
    __u8 _pad4[116];
    struct edid_info edid_info;
    struct efi_info efi_info;
    __u32 alt_mem_k;
    __u32 scratch;
    __u8 e820_entries;
    __u8 eddbuf_entries;
    __u8 edd_mbr_sig_buf_entries;
    __u8 kbd_status;
    __u8 secure_boot;
    __u8 _pad5[2];
    __u8 sentinel;
    __u8 _pad6[1];
    struct setup_header hdr;
    __u8 _pad7[36];
    __u32 edd_mbr_sig_buffer[16];
    struct boot_e820_entry e820_table[128];
    __u8 _pad8[48];
    struct edd_info eddbuf[6];
    __u8 _pad9[276];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct boot_params {
    struct screen_info screen_info;
    struct apm_bios_info apm_bios_info;
    __u8 _pad2[4];
    __u64 tboot_addr;
    struct ist_info ist_info;
    __u64 acpi_rsdp_addr;
    __u8 _pad3[8];
    __u8 hd0_info[16];
    __u8 hd1_info[16];
    struct sys_desc_table sys_desc_table;
    struct olpc_ofw_header olpc_ofw_header;
    __u32 ext_ramdisk_image;
    __u32 ext_ramdisk_size;
    __u32 ext_cmd_line_ptr;
    __u8 _pad4[116];
    struct edid_info edid_info;
    struct efi_info efi_info;
    __u32 alt_mem_k;
    __u32 scratch;
    __u8 e820_entries;
    __u8 eddbuf_entries;
    __u8 edd_mbr_sig_buf_entries;
    __u8 kbd_status;
    __u8 secure_boot;
    __u8 _pad5[2];
    __u8 sentinel;
    __u8 _pad6[1];
    struct setup_header hdr;
    __u8 _pad7[36];
    __u32 edd_mbr_sig_buffer[16];
    struct boot_e820_entry e820_table[128];
    __u8 _pad8[48];
    struct edd_info eddbuf[6];
    __u8 _pad9[276];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct boot_params {
    struct screen_info screen_info;
    struct apm_bios_info apm_bios_info;
    __u8 _pad2[4];
    __u64 tboot_addr;
    struct ist_info ist_info;
    __u64 acpi_rsdp_addr;
    __u8 _pad3[8];
    __u8 hd0_info[16];
    __u8 hd1_info[16];
    struct sys_desc_table sys_desc_table;
    struct olpc_ofw_header olpc_ofw_header;
    __u32 ext_ramdisk_image;
    __u32 ext_ramdisk_size;
    __u32 ext_cmd_line_ptr;
    __u8 _pad4[116];
    struct edid_info edid_info;
    struct efi_info efi_info;
    __u32 alt_mem_k;
    __u32 scratch;
    __u8 e820_entries;
    __u8 eddbuf_entries;
    __u8 edd_mbr_sig_buf_entries;
    __u8 kbd_status;
    __u8 secure_boot;
    __u8 _pad5[2];
    __u8 sentinel;
    __u8 _pad6[1];
    struct setup_header hdr;
    __u8 _pad7[36];
    __u32 edd_mbr_sig_buffer[16];
    struct boot_e820_entry e820_table[128];
    __u8 _pad8[48];
    struct edd_info eddbuf[6];
    __u8 _pad9[276];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct boot_params {
    struct screen_info screen_info;
    struct apm_bios_info apm_bios_info;
    __u8 _pad2[4];
    __u64 tboot_addr;
    struct ist_info ist_info;
    __u64 acpi_rsdp_addr;
    __u8 _pad3[8];
    __u8 hd0_info[16];
    __u8 hd1_info[16];
    struct sys_desc_table sys_desc_table;
    struct olpc_ofw_header olpc_ofw_header;
    __u32 ext_ramdisk_image;
    __u32 ext_ramdisk_size;
    __u32 ext_cmd_line_ptr;
    __u8 _pad4[116];
    struct edid_info edid_info;
    struct efi_info efi_info;
    __u32 alt_mem_k;
    __u32 scratch;
    __u8 e820_entries;
    __u8 eddbuf_entries;
    __u8 edd_mbr_sig_buf_entries;
    __u8 kbd_status;
    __u8 secure_boot;
    __u8 _pad5[2];
    __u8 sentinel;
    __u8 _pad6[1];
    struct setup_header hdr;
    __u8 _pad7[36];
    __u32 edd_mbr_sig_buffer[16];
    struct boot_e820_entry e820_table[128];
    __u8 _pad8[48];
    struct edd_info eddbuf[6];
    __u8 _pad9[276];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct boot_params {
    struct screen_info screen_info;
    struct apm_bios_info apm_bios_info;
    __u8 _pad2[4];
    __u64 tboot_addr;
    struct ist_info ist_info;
    __u64 acpi_rsdp_addr;
    __u8 _pad3[8];
    __u8 hd0_info[16];
    __u8 hd1_info[16];
    struct sys_desc_table sys_desc_table;
    struct olpc_ofw_header olpc_ofw_header;
    __u32 ext_ramdisk_image;
    __u32 ext_ramdisk_size;
    __u32 ext_cmd_line_ptr;
    __u8 _pad4[112];
    __u32 cc_blob_address;
    struct edid_info edid_info;
    struct efi_info efi_info;
    __u32 alt_mem_k;
    __u32 scratch;
    __u8 e820_entries;
    __u8 eddbuf_entries;
    __u8 edd_mbr_sig_buf_entries;
    __u8 kbd_status;
    __u8 secure_boot;
    __u8 _pad5[2];
    __u8 sentinel;
    __u8 _pad6[1];
    struct setup_header hdr;
    __u8 _pad7[36];
    __u32 edd_mbr_sig_buffer[16];
    struct boot_e820_entry e820_table[128];
    __u8 _pad8[48];
    struct edd_info eddbuf[6];
    __u8 _pad9[276];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct boot_params {
    struct screen_info screen_info;
    struct apm_bios_info apm_bios_info;
    __u8 _pad2[4];
    __u64 tboot_addr;
    struct ist_info ist_info;
    __u64 acpi_rsdp_addr;
    __u8 _pad3[8];
    __u8 hd0_info[16];
    __u8 hd1_info[16];
    struct sys_desc_table sys_desc_table;
    struct olpc_ofw_header olpc_ofw_header;
    __u32 ext_ramdisk_image;
    __u32 ext_ramdisk_size;
    __u32 ext_cmd_line_ptr;
    __u8 _pad4[112];
    __u32 cc_blob_address;
    struct edid_info edid_info;
    struct efi_info efi_info;
    __u32 alt_mem_k;
    __u32 scratch;
    __u8 e820_entries;
    __u8 eddbuf_entries;
    __u8 edd_mbr_sig_buf_entries;
    __u8 kbd_status;
    __u8 secure_boot;
    __u8 _pad5[2];
    __u8 sentinel;
    __u8 _pad6[1];
    struct setup_header hdr;
    __u8 _pad7[36];
    __u32 edd_mbr_sig_buffer[16];
    struct boot_e820_entry e820_table[128];
    __u8 _pad8[48];
    struct edd_info eddbuf[6];
    __u8 _pad9[276];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct boot_params {
    struct screen_info screen_info;
    struct apm_bios_info apm_bios_info;
    __u8 _pad2[4];
    __u64 tboot_addr;
    struct ist_info ist_info;
    __u64 acpi_rsdp_addr;
    __u8 _pad3[8];
    __u8 hd0_info[16];
    __u8 hd1_info[16];
    struct sys_desc_table sys_desc_table;
    struct olpc_ofw_header olpc_ofw_header;
    __u32 ext_ramdisk_image;
    __u32 ext_ramdisk_size;
    __u32 ext_cmd_line_ptr;
    __u8 _pad4[112];
    __u32 cc_blob_address;
    struct edid_info edid_info;
    struct efi_info efi_info;
    __u32 alt_mem_k;
    __u32 scratch;
    __u8 e820_entries;
    __u8 eddbuf_entries;
    __u8 edd_mbr_sig_buf_entries;
    __u8 kbd_status;
    __u8 secure_boot;
    __u8 _pad5[2];
    __u8 sentinel;
    __u8 _pad6[1];
    struct setup_header hdr;
    __u8 _pad7[36];
    __u32 edd_mbr_sig_buffer[16];
    struct boot_e820_entry e820_table[128];
    __u8 _pad8[48];
    struct edd_info eddbuf[6];
    __u8 _pad9[276];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct boot_params {
    struct screen_info screen_info;
    struct apm_bios_info apm_bios_info;
    __u8 _pad2[4];
    __u64 tboot_addr;
    struct ist_info ist_info;
    __u64 acpi_rsdp_addr;
    __u8 _pad3[8];
    __u8 hd0_info[16];
    __u8 hd1_info[16];
    struct sys_desc_table sys_desc_table;
    struct olpc_ofw_header olpc_ofw_header;
    __u32 ext_ramdisk_image;
    __u32 ext_ramdisk_size;
    __u32 ext_cmd_line_ptr;
    __u8 _pad4[112];
    __u32 cc_blob_address;
    struct edid_info edid_info;
    struct efi_info efi_info;
    __u32 alt_mem_k;
    __u32 scratch;
    __u8 e820_entries;
    __u8 eddbuf_entries;
    __u8 edd_mbr_sig_buf_entries;
    __u8 kbd_status;
    __u8 secure_boot;
    __u8 _pad5[2];
    __u8 sentinel;
    __u8 _pad6[1];
    struct setup_header hdr;
    __u8 _pad7[36];
    __u32 edd_mbr_sig_buffer[16];
    struct boot_e820_entry e820_table[128];
    __u8 _pad8[48];
    struct edd_info eddbuf[6];
    __u8 _pad9[276];
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
struct boot_params {
    struct screen_info screen_info;
    struct apm_bios_info apm_bios_info;
    __u8 _pad2[4];
    __u64 tboot_addr;
    struct ist_info ist_info;
    __u64 acpi_rsdp_addr;
    __u8 _pad3[8];
    __u8 hd0_info[16];
    __u8 hd1_info[16];
    struct sys_desc_table sys_desc_table;
    struct olpc_ofw_header olpc_ofw_header;
    __u32 ext_ramdisk_image;
    __u32 ext_ramdisk_size;
    __u32 ext_cmd_line_ptr;
    __u8 _pad4[116];
    struct edid_info edid_info;
    struct efi_info efi_info;
    __u32 alt_mem_k;
    __u32 scratch;
    __u8 e820_entries;
    __u8 eddbuf_entries;
    __u8 edd_mbr_sig_buf_entries;
    __u8 kbd_status;
    __u8 secure_boot;
    __u8 _pad5[2];
    __u8 sentinel;
    __u8 _pad6[1];
    struct setup_header hdr;
    __u8 _pad7[40];
    __u32 edd_mbr_sig_buffer[16];
    struct boot_e820_entry e820_table[128];
    __u8 _pad8[48];
    struct edd_info eddbuf[6];
    __u8 _pad9[276];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct boot_params {
    struct screen_info screen_info;
    struct apm_bios_info apm_bios_info;
    __u8 _pad2[4];
    __u64 tboot_addr;
    struct ist_info ist_info;
    __u64 acpi_rsdp_addr;
    __u8 _pad3[8];
    __u8 hd0_info[16];
    __u8 hd1_info[16];
    struct sys_desc_table sys_desc_table;
    struct olpc_ofw_header olpc_ofw_header;
    __u32 ext_ramdisk_image;
    __u32 ext_ramdisk_size;
    __u32 ext_cmd_line_ptr;
    __u8 _pad4[116];
    struct edid_info edid_info;
    struct efi_info efi_info;
    __u32 alt_mem_k;
    __u32 scratch;
    __u8 e820_entries;
    __u8 eddbuf_entries;
    __u8 edd_mbr_sig_buf_entries;
    __u8 kbd_status;
    __u8 secure_boot;
    __u8 _pad5[2];
    __u8 sentinel;
    __u8 _pad6[1];
    struct setup_header hdr;
    __u8 _pad7[40];
    __u32 edd_mbr_sig_buffer[16];
    struct boot_e820_entry e820_table[128];
    __u8 _pad8[48];
    struct edd_info eddbuf[6];
    __u8 _pad9[276];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct boot_params {
    struct screen_info screen_info;
    struct apm_bios_info apm_bios_info;
    __u8 _pad2[4];
    __u64 tboot_addr;
    struct ist_info ist_info;
    __u64 acpi_rsdp_addr;
    __u8 _pad3[8];
    __u8 hd0_info[16];
    __u8 hd1_info[16];
    struct sys_desc_table sys_desc_table;
    struct olpc_ofw_header olpc_ofw_header;
    __u32 ext_ramdisk_image;
    __u32 ext_ramdisk_size;
    __u32 ext_cmd_line_ptr;
    __u8 _pad4[116];
    struct edid_info edid_info;
    struct efi_info efi_info;
    __u32 alt_mem_k;
    __u32 scratch;
    __u8 e820_entries;
    __u8 eddbuf_entries;
    __u8 edd_mbr_sig_buf_entries;
    __u8 kbd_status;
    __u8 secure_boot;
    __u8 _pad5[2];
    __u8 sentinel;
    __u8 _pad6[1];
    struct setup_header hdr;
    __u8 _pad7[40];
    __u32 edd_mbr_sig_buffer[16];
    struct boot_e820_entry e820_table[128];
    __u8 _pad8[48];
    struct edd_info eddbuf[6];
    __u8 _pad9[276];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct boot_params {
    struct screen_info screen_info;
    struct apm_bios_info apm_bios_info;
    __u8 _pad2[4];
    __u64 tboot_addr;
    struct ist_info ist_info;
    __u64 acpi_rsdp_addr;
    __u8 _pad3[8];
    __u8 hd0_info[16];
    __u8 hd1_info[16];
    struct sys_desc_table sys_desc_table;
    struct olpc_ofw_header olpc_ofw_header;
    __u32 ext_ramdisk_image;
    __u32 ext_ramdisk_size;
    __u32 ext_cmd_line_ptr;
    __u8 _pad4[116];
    struct edid_info edid_info;
    struct efi_info efi_info;
    __u32 alt_mem_k;
    __u32 scratch;
    __u8 e820_entries;
    __u8 eddbuf_entries;
    __u8 edd_mbr_sig_buf_entries;
    __u8 kbd_status;
    __u8 secure_boot;
    __u8 _pad5[2];
    __u8 sentinel;
    __u8 _pad6[1];
    struct setup_header hdr;
    __u8 _pad7[40];
    __u32 edd_mbr_sig_buffer[16];
    struct boot_e820_entry e820_table[128];
    __u8 _pad8[48];
    struct edd_info eddbuf[6];
    __u8 _pad9[276];
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
<code>struct boot_e820_entry e820_table[128]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct e820entry e820_map[128]</code>
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
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u64 acpi_rsdp_addr</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u8 _pad3[16]</code> ➡️ <code>__u8 _pad3[8]</code>
</li>
</ul>
</details>
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
<b>Field type changed. </b>
<code>__u8 _pad7[40]</code> ➡️ <code>__u8 _pad7[36]</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u32 cc_blob_address</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u8 _pad4[116]</code> ➡️ <code>__u8 _pad4[112]</code>
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
