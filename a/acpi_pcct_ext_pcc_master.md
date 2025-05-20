# Struct: <code>acpi_pcct_ext_pcc_master</code>

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
In <code>4.15</code>: Absent ⚠️
</li>
<li>
In <code>4.18</code>: Absent ⚠️
</li>
<li>
In <code>5.0</code>: Absent ⚠️
</li>
<li>
In <code>5.3</code>: Absent ⚠️
</li>
<li>
In <code>5.4</code>: Absent ⚠️
</li>
<li>
In <code>5.8</code>: Absent ⚠️
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct acpi_pcct_ext_pcc_master {
    struct acpi_subtable_header header;
    u32 platform_interrupt;
    u8 flags;
    u8 reserved1;
    u64 base_address;
    u32 length;
    struct acpi_generic_address doorbell_register;
    u64 preserve_mask;
    u64 write_mask;
    u32 latency;
    u32 max_access_rate;
    u32 min_turnaround_time;
    struct acpi_generic_address platform_ack_register;
    u64 ack_preserve_mask;
    u64 ack_set_mask;
    u64 reserved2;
    struct acpi_generic_address cmd_complete_register;
    u64 cmd_complete_mask;
    struct acpi_generic_address cmd_update_register;
    u64 cmd_update_preserve_mask;
    u64 cmd_update_set_mask;
    struct acpi_generic_address error_status_register;
    u64 error_status_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct acpi_pcct_ext_pcc_master {
    struct acpi_subtable_header header;
    u32 platform_interrupt;
    u8 flags;
    u8 reserved1;
    u64 base_address;
    u32 length;
    struct acpi_generic_address doorbell_register;
    u64 preserve_mask;
    u64 write_mask;
    u32 latency;
    u32 max_access_rate;
    u32 min_turnaround_time;
    struct acpi_generic_address platform_ack_register;
    u64 ack_preserve_mask;
    u64 ack_set_mask;
    u64 reserved2;
    struct acpi_generic_address cmd_complete_register;
    u64 cmd_complete_mask;
    struct acpi_generic_address cmd_update_register;
    u64 cmd_update_preserve_mask;
    u64 cmd_update_set_mask;
    struct acpi_generic_address error_status_register;
    u64 error_status_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct acpi_pcct_ext_pcc_master {
    struct acpi_subtable_header header;
    u32 platform_interrupt;
    u8 flags;
    u8 reserved1;
    u64 base_address;
    u32 length;
    struct acpi_generic_address doorbell_register;
    u64 preserve_mask;
    u64 write_mask;
    u32 latency;
    u32 max_access_rate;
    u32 min_turnaround_time;
    struct acpi_generic_address platform_ack_register;
    u64 ack_preserve_mask;
    u64 ack_set_mask;
    u64 reserved2;
    struct acpi_generic_address cmd_complete_register;
    u64 cmd_complete_mask;
    struct acpi_generic_address cmd_update_register;
    u64 cmd_update_preserve_mask;
    u64 cmd_update_set_mask;
    struct acpi_generic_address error_status_register;
    u64 error_status_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct acpi_pcct_ext_pcc_master {
    struct acpi_subtable_header header;
    u32 platform_interrupt;
    u8 flags;
    u8 reserved1;
    u64 base_address;
    u32 length;
    struct acpi_generic_address doorbell_register;
    u64 preserve_mask;
    u64 write_mask;
    u32 latency;
    u32 max_access_rate;
    u32 min_turnaround_time;
    struct acpi_generic_address platform_ack_register;
    u64 ack_preserve_mask;
    u64 ack_set_mask;
    u64 reserved2;
    struct acpi_generic_address cmd_complete_register;
    u64 cmd_complete_mask;
    struct acpi_generic_address cmd_update_register;
    u64 cmd_update_preserve_mask;
    u64 cmd_update_set_mask;
    struct acpi_generic_address error_status_register;
    u64 error_status_mask;
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
In <code>aws</code>: Absent ⚠️
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
