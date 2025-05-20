# Struct: <code>efi</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct efi {
    efi_system_table_t *systab;
    unsigned int runtime_version;
    long unsigned int mps;
    long unsigned int acpi;
    long unsigned int acpi20;
    long unsigned int smbios;
    long unsigned int smbios3;
    long unsigned int sal_systab;
    long unsigned int boot_info;
    long unsigned int hcdp;
    long unsigned int uga;
    long unsigned int uv_systab;
    long unsigned int fw_vendor;
    long unsigned int runtime;
    long unsigned int config_table;
    long unsigned int esrt;
    long unsigned int properties_table;
    efi_get_time_t *get_time;
    efi_set_time_t *set_time;
    efi_get_wakeup_time_t *get_wakeup_time;
    efi_set_wakeup_time_t *set_wakeup_time;
    efi_get_variable_t *get_variable;
    efi_get_next_variable_t *get_next_variable;
    efi_set_variable_t *set_variable;
    efi_set_variable_nonblocking_t *set_variable_nonblocking;
    efi_query_variable_info_t *query_variable_info;
    efi_update_capsule_t *update_capsule;
    efi_query_capsule_caps_t *query_capsule_caps;
    efi_get_next_high_mono_count_t *get_next_high_mono_count;
    efi_reset_system_t *reset_system;
    efi_set_virtual_address_map_t *set_virtual_address_map;
    struct efi_memory_map *memmap;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct efi {
    efi_system_table_t *systab;
    unsigned int runtime_version;
    long unsigned int mps;
    long unsigned int acpi;
    long unsigned int acpi20;
    long unsigned int smbios;
    long unsigned int smbios3;
    long unsigned int sal_systab;
    long unsigned int boot_info;
    long unsigned int hcdp;
    long unsigned int uga;
    long unsigned int uv_systab;
    long unsigned int fw_vendor;
    long unsigned int runtime;
    long unsigned int config_table;
    long unsigned int esrt;
    long unsigned int properties_table;
    long unsigned int mem_attr_table;
    efi_get_time_t *get_time;
    efi_set_time_t *set_time;
    efi_get_wakeup_time_t *get_wakeup_time;
    efi_set_wakeup_time_t *set_wakeup_time;
    efi_get_variable_t *get_variable;
    efi_get_next_variable_t *get_next_variable;
    efi_set_variable_t *set_variable;
    efi_set_variable_t *set_variable_nonblocking;
    efi_query_variable_info_t *query_variable_info;
    efi_query_variable_info_t *query_variable_info_nonblocking;
    efi_update_capsule_t *update_capsule;
    efi_query_capsule_caps_t *query_capsule_caps;
    efi_get_next_high_mono_count_t *get_next_high_mono_count;
    efi_reset_system_t *reset_system;
    efi_set_virtual_address_map_t *set_virtual_address_map;
    struct efi_memory_map memmap;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct efi {
    efi_system_table_t *systab;
    unsigned int runtime_version;
    long unsigned int mps;
    long unsigned int acpi;
    long unsigned int acpi20;
    long unsigned int smbios;
    long unsigned int smbios3;
    long unsigned int sal_systab;
    long unsigned int boot_info;
    long unsigned int hcdp;
    long unsigned int uga;
    long unsigned int uv_systab;
    long unsigned int fw_vendor;
    long unsigned int runtime;
    long unsigned int config_table;
    long unsigned int esrt;
    long unsigned int properties_table;
    long unsigned int mem_attr_table;
    long unsigned int rng_seed;
    efi_get_time_t *get_time;
    efi_set_time_t *set_time;
    efi_get_wakeup_time_t *get_wakeup_time;
    efi_set_wakeup_time_t *set_wakeup_time;
    efi_get_variable_t *get_variable;
    efi_get_next_variable_t *get_next_variable;
    efi_set_variable_t *set_variable;
    efi_set_variable_t *set_variable_nonblocking;
    efi_query_variable_info_t *query_variable_info;
    efi_query_variable_info_t *query_variable_info_nonblocking;
    efi_update_capsule_t *update_capsule;
    efi_query_capsule_caps_t *query_capsule_caps;
    efi_get_next_high_mono_count_t *get_next_high_mono_count;
    efi_reset_system_t *reset_system;
    efi_set_virtual_address_map_t *set_virtual_address_map;
    struct efi_memory_map memmap;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct efi {
    efi_system_table_t *systab;
    unsigned int runtime_version;
    long unsigned int mps;
    long unsigned int acpi;
    long unsigned int acpi20;
    long unsigned int smbios;
    long unsigned int smbios3;
    long unsigned int sal_systab;
    long unsigned int boot_info;
    long unsigned int hcdp;
    long unsigned int uga;
    long unsigned int uv_systab;
    long unsigned int fw_vendor;
    long unsigned int runtime;
    long unsigned int config_table;
    long unsigned int esrt;
    long unsigned int properties_table;
    long unsigned int mem_attr_table;
    long unsigned int rng_seed;
    efi_get_time_t *get_time;
    efi_set_time_t *set_time;
    efi_get_wakeup_time_t *get_wakeup_time;
    efi_set_wakeup_time_t *set_wakeup_time;
    efi_get_variable_t *get_variable;
    efi_get_next_variable_t *get_next_variable;
    efi_set_variable_t *set_variable;
    efi_set_variable_t *set_variable_nonblocking;
    efi_query_variable_info_t *query_variable_info;
    efi_query_variable_info_t *query_variable_info_nonblocking;
    efi_update_capsule_t *update_capsule;
    efi_query_capsule_caps_t *query_capsule_caps;
    efi_get_next_high_mono_count_t *get_next_high_mono_count;
    efi_reset_system_t *reset_system;
    efi_set_virtual_address_map_t *set_virtual_address_map;
    struct efi_memory_map memmap;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct efi {
    efi_system_table_t *systab;
    unsigned int runtime_version;
    long unsigned int mps;
    long unsigned int acpi;
    long unsigned int acpi20;
    long unsigned int smbios;
    long unsigned int smbios3;
    long unsigned int sal_systab;
    long unsigned int boot_info;
    long unsigned int hcdp;
    long unsigned int uga;
    long unsigned int uv_systab;
    long unsigned int fw_vendor;
    long unsigned int runtime;
    long unsigned int config_table;
    long unsigned int esrt;
    long unsigned int properties_table;
    long unsigned int mem_attr_table;
    long unsigned int rng_seed;
    efi_get_time_t *get_time;
    efi_set_time_t *set_time;
    efi_get_wakeup_time_t *get_wakeup_time;
    efi_set_wakeup_time_t *set_wakeup_time;
    efi_get_variable_t *get_variable;
    efi_get_next_variable_t *get_next_variable;
    efi_set_variable_t *set_variable;
    efi_set_variable_t *set_variable_nonblocking;
    efi_query_variable_info_t *query_variable_info;
    efi_query_variable_info_t *query_variable_info_nonblocking;
    efi_update_capsule_t *update_capsule;
    efi_query_capsule_caps_t *query_capsule_caps;
    efi_get_next_high_mono_count_t *get_next_high_mono_count;
    efi_reset_system_t *reset_system;
    efi_set_virtual_address_map_t *set_virtual_address_map;
    struct efi_memory_map memmap;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct efi {
    efi_system_table_t *systab;
    unsigned int runtime_version;
    long unsigned int mps;
    long unsigned int acpi;
    long unsigned int acpi20;
    long unsigned int smbios;
    long unsigned int smbios3;
    long unsigned int sal_systab;
    long unsigned int boot_info;
    long unsigned int hcdp;
    long unsigned int uga;
    long unsigned int uv_systab;
    long unsigned int fw_vendor;
    long unsigned int runtime;
    long unsigned int config_table;
    long unsigned int esrt;
    long unsigned int properties_table;
    long unsigned int mem_attr_table;
    long unsigned int rng_seed;
    long unsigned int tpm_log;
    efi_get_time_t *get_time;
    efi_set_time_t *set_time;
    efi_get_wakeup_time_t *get_wakeup_time;
    efi_set_wakeup_time_t *set_wakeup_time;
    efi_get_variable_t *get_variable;
    efi_get_next_variable_t *get_next_variable;
    efi_set_variable_t *set_variable;
    efi_set_variable_t *set_variable_nonblocking;
    efi_query_variable_info_t *query_variable_info;
    efi_query_variable_info_t *query_variable_info_nonblocking;
    efi_update_capsule_t *update_capsule;
    efi_query_capsule_caps_t *query_capsule_caps;
    efi_get_next_high_mono_count_t *get_next_high_mono_count;
    efi_reset_system_t *reset_system;
    efi_set_virtual_address_map_t *set_virtual_address_map;
    struct efi_memory_map memmap;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct efi {
    efi_system_table_t *systab;
    unsigned int runtime_version;
    long unsigned int mps;
    long unsigned int acpi;
    long unsigned int acpi20;
    long unsigned int smbios;
    long unsigned int smbios3;
    long unsigned int sal_systab;
    long unsigned int boot_info;
    long unsigned int hcdp;
    long unsigned int uga;
    long unsigned int uv_systab;
    long unsigned int fw_vendor;
    long unsigned int runtime;
    long unsigned int config_table;
    long unsigned int esrt;
    long unsigned int properties_table;
    long unsigned int mem_attr_table;
    long unsigned int rng_seed;
    long unsigned int tpm_log;
    long unsigned int mem_reserve;
    efi_get_time_t *get_time;
    efi_set_time_t *set_time;
    efi_get_wakeup_time_t *get_wakeup_time;
    efi_set_wakeup_time_t *set_wakeup_time;
    efi_get_variable_t *get_variable;
    efi_get_next_variable_t *get_next_variable;
    efi_set_variable_t *set_variable;
    efi_set_variable_t *set_variable_nonblocking;
    efi_query_variable_info_t *query_variable_info;
    efi_query_variable_info_t *query_variable_info_nonblocking;
    efi_update_capsule_t *update_capsule;
    efi_query_capsule_caps_t *query_capsule_caps;
    efi_get_next_high_mono_count_t *get_next_high_mono_count;
    efi_reset_system_t *reset_system;
    efi_set_virtual_address_map_t *set_virtual_address_map;
    struct efi_memory_map memmap;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct efi {
    efi_system_table_t *systab;
    unsigned int runtime_version;
    long unsigned int mps;
    long unsigned int acpi;
    long unsigned int acpi20;
    long unsigned int smbios;
    long unsigned int smbios3;
    long unsigned int sal_systab;
    long unsigned int boot_info;
    long unsigned int hcdp;
    long unsigned int uga;
    long unsigned int uv_systab;
    long unsigned int fw_vendor;
    long unsigned int runtime;
    long unsigned int config_table;
    long unsigned int esrt;
    long unsigned int properties_table;
    long unsigned int mem_attr_table;
    long unsigned int rng_seed;
    long unsigned int tpm_log;
    long unsigned int tpm_final_log;
    long unsigned int mem_reserve;
    efi_get_time_t *get_time;
    efi_set_time_t *set_time;
    efi_get_wakeup_time_t *get_wakeup_time;
    efi_set_wakeup_time_t *set_wakeup_time;
    efi_get_variable_t *get_variable;
    efi_get_next_variable_t *get_next_variable;
    efi_set_variable_t *set_variable;
    efi_set_variable_t *set_variable_nonblocking;
    efi_query_variable_info_t *query_variable_info;
    efi_query_variable_info_t *query_variable_info_nonblocking;
    efi_update_capsule_t *update_capsule;
    efi_query_capsule_caps_t *query_capsule_caps;
    efi_get_next_high_mono_count_t *get_next_high_mono_count;
    efi_reset_system_t *reset_system;
    efi_set_virtual_address_map_t *set_virtual_address_map;
    struct efi_memory_map memmap;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct efi {
    efi_system_table_t *systab;
    unsigned int runtime_version;
    long unsigned int mps;
    long unsigned int acpi;
    long unsigned int acpi20;
    long unsigned int smbios;
    long unsigned int smbios3;
    long unsigned int boot_info;
    long unsigned int hcdp;
    long unsigned int uga;
    long unsigned int fw_vendor;
    long unsigned int runtime;
    long unsigned int config_table;
    long unsigned int esrt;
    long unsigned int properties_table;
    long unsigned int mem_attr_table;
    long unsigned int rng_seed;
    long unsigned int tpm_log;
    long unsigned int tpm_final_log;
    long unsigned int mem_reserve;
    efi_get_time_t *get_time;
    efi_set_time_t *set_time;
    efi_get_wakeup_time_t *get_wakeup_time;
    efi_set_wakeup_time_t *set_wakeup_time;
    efi_get_variable_t *get_variable;
    efi_get_next_variable_t *get_next_variable;
    efi_set_variable_t *set_variable;
    efi_set_variable_t *set_variable_nonblocking;
    efi_query_variable_info_t *query_variable_info;
    efi_query_variable_info_t *query_variable_info_nonblocking;
    efi_update_capsule_t *update_capsule;
    efi_query_capsule_caps_t *query_capsule_caps;
    efi_get_next_high_mono_count_t *get_next_high_mono_count;
    efi_reset_system_t *reset_system;
    efi_set_virtual_address_map_t *set_virtual_address_map;
    struct efi_memory_map memmap;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct efi {
    const efi_runtime_services_t *runtime;
    unsigned int runtime_version;
    unsigned int runtime_supported_mask;
    long unsigned int acpi;
    long unsigned int acpi20;
    long unsigned int smbios;
    long unsigned int smbios3;
    long unsigned int esrt;
    long unsigned int tpm_log;
    long unsigned int tpm_final_log;
    efi_get_time_t *get_time;
    efi_set_time_t *set_time;
    efi_get_wakeup_time_t *get_wakeup_time;
    efi_set_wakeup_time_t *set_wakeup_time;
    efi_get_variable_t *get_variable;
    efi_get_next_variable_t *get_next_variable;
    efi_set_variable_t *set_variable;
    efi_set_variable_t *set_variable_nonblocking;
    efi_query_variable_info_t *query_variable_info;
    efi_query_variable_info_t *query_variable_info_nonblocking;
    efi_update_capsule_t *update_capsule;
    efi_query_capsule_caps_t *query_capsule_caps;
    efi_get_next_high_mono_count_t *get_next_high_mono_count;
    efi_reset_system_t *reset_system;
    struct efi_memory_map memmap;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct efi {
    const efi_runtime_services_t *runtime;
    unsigned int runtime_version;
    unsigned int runtime_supported_mask;
    long unsigned int acpi;
    long unsigned int acpi20;
    long unsigned int smbios;
    long unsigned int smbios3;
    long unsigned int esrt;
    long unsigned int tpm_log;
    long unsigned int tpm_final_log;
    long unsigned int mokvar_table;
    efi_get_time_t *get_time;
    efi_set_time_t *set_time;
    efi_get_wakeup_time_t *get_wakeup_time;
    efi_set_wakeup_time_t *set_wakeup_time;
    efi_get_variable_t *get_variable;
    efi_get_next_variable_t *get_next_variable;
    efi_set_variable_t *set_variable;
    efi_set_variable_t *set_variable_nonblocking;
    efi_query_variable_info_t *query_variable_info;
    efi_query_variable_info_t *query_variable_info_nonblocking;
    efi_update_capsule_t *update_capsule;
    efi_query_capsule_caps_t *query_capsule_caps;
    efi_get_next_high_mono_count_t *get_next_high_mono_count;
    efi_reset_system_t *reset_system;
    struct efi_memory_map memmap;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct efi {
    const efi_runtime_services_t *runtime;
    unsigned int runtime_version;
    unsigned int runtime_supported_mask;
    long unsigned int acpi;
    long unsigned int acpi20;
    long unsigned int smbios;
    long unsigned int smbios3;
    long unsigned int esrt;
    long unsigned int tpm_log;
    long unsigned int tpm_final_log;
    long unsigned int mokvar_table;
    efi_get_time_t *get_time;
    efi_set_time_t *set_time;
    efi_get_wakeup_time_t *get_wakeup_time;
    efi_set_wakeup_time_t *set_wakeup_time;
    efi_get_variable_t *get_variable;
    efi_get_next_variable_t *get_next_variable;
    efi_set_variable_t *set_variable;
    efi_set_variable_t *set_variable_nonblocking;
    efi_query_variable_info_t *query_variable_info;
    efi_query_variable_info_t *query_variable_info_nonblocking;
    efi_update_capsule_t *update_capsule;
    efi_query_capsule_caps_t *query_capsule_caps;
    efi_get_next_high_mono_count_t *get_next_high_mono_count;
    efi_reset_system_t *reset_system;
    struct efi_memory_map memmap;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct efi {
    const efi_runtime_services_t *runtime;
    unsigned int runtime_version;
    unsigned int runtime_supported_mask;
    long unsigned int acpi;
    long unsigned int acpi20;
    long unsigned int smbios;
    long unsigned int smbios3;
    long unsigned int esrt;
    long unsigned int tpm_log;
    long unsigned int tpm_final_log;
    long unsigned int mokvar_table;
    efi_get_time_t *get_time;
    efi_set_time_t *set_time;
    efi_get_wakeup_time_t *get_wakeup_time;
    efi_set_wakeup_time_t *set_wakeup_time;
    efi_get_variable_t *get_variable;
    efi_get_next_variable_t *get_next_variable;
    efi_set_variable_t *set_variable;
    efi_set_variable_t *set_variable_nonblocking;
    efi_query_variable_info_t *query_variable_info;
    efi_query_variable_info_t *query_variable_info_nonblocking;
    efi_update_capsule_t *update_capsule;
    efi_query_capsule_caps_t *query_capsule_caps;
    efi_get_next_high_mono_count_t *get_next_high_mono_count;
    efi_reset_system_t *reset_system;
    struct efi_memory_map memmap;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct efi {
    const efi_runtime_services_t *runtime;
    unsigned int runtime_version;
    unsigned int runtime_supported_mask;
    long unsigned int acpi;
    long unsigned int acpi20;
    long unsigned int smbios;
    long unsigned int smbios3;
    long unsigned int esrt;
    long unsigned int tpm_log;
    long unsigned int tpm_final_log;
    long unsigned int mokvar_table;
    long unsigned int coco_secret;
    efi_get_time_t *get_time;
    efi_set_time_t *set_time;
    efi_get_wakeup_time_t *get_wakeup_time;
    efi_set_wakeup_time_t *set_wakeup_time;
    efi_get_variable_t *get_variable;
    efi_get_next_variable_t *get_next_variable;
    efi_set_variable_t *set_variable;
    efi_set_variable_t *set_variable_nonblocking;
    efi_query_variable_info_t *query_variable_info;
    efi_query_variable_info_t *query_variable_info_nonblocking;
    efi_update_capsule_t *update_capsule;
    efi_query_capsule_caps_t *query_capsule_caps;
    efi_get_next_high_mono_count_t *get_next_high_mono_count;
    efi_reset_system_t *reset_system;
    struct efi_memory_map memmap;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct efi {
    const efi_runtime_services_t *runtime;
    unsigned int runtime_version;
    unsigned int runtime_supported_mask;
    long unsigned int acpi;
    long unsigned int acpi20;
    long unsigned int smbios;
    long unsigned int smbios3;
    long unsigned int esrt;
    long unsigned int tpm_log;
    long unsigned int tpm_final_log;
    long unsigned int mokvar_table;
    long unsigned int coco_secret;
    efi_get_time_t *get_time;
    efi_set_time_t *set_time;
    efi_get_wakeup_time_t *get_wakeup_time;
    efi_set_wakeup_time_t *set_wakeup_time;
    efi_get_variable_t *get_variable;
    efi_get_next_variable_t *get_next_variable;
    efi_set_variable_t *set_variable;
    efi_set_variable_t *set_variable_nonblocking;
    efi_query_variable_info_t *query_variable_info;
    efi_query_variable_info_t *query_variable_info_nonblocking;
    efi_update_capsule_t *update_capsule;
    efi_query_capsule_caps_t *query_capsule_caps;
    efi_get_next_high_mono_count_t *get_next_high_mono_count;
    efi_reset_system_t *reset_system;
    struct efi_memory_map memmap;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct efi {
    const efi_runtime_services_t *runtime;
    unsigned int runtime_version;
    unsigned int runtime_supported_mask;
    long unsigned int acpi;
    long unsigned int acpi20;
    long unsigned int smbios;
    long unsigned int smbios3;
    long unsigned int esrt;
    long unsigned int tpm_log;
    long unsigned int tpm_final_log;
    long unsigned int mokvar_table;
    long unsigned int coco_secret;
    long unsigned int unaccepted;
    efi_get_time_t *get_time;
    efi_set_time_t *set_time;
    efi_get_wakeup_time_t *get_wakeup_time;
    efi_set_wakeup_time_t *set_wakeup_time;
    efi_get_variable_t *get_variable;
    efi_get_next_variable_t *get_next_variable;
    efi_set_variable_t *set_variable;
    efi_set_variable_t *set_variable_nonblocking;
    efi_query_variable_info_t *query_variable_info;
    efi_query_variable_info_t *query_variable_info_nonblocking;
    efi_update_capsule_t *update_capsule;
    efi_query_capsule_caps_t *query_capsule_caps;
    efi_get_next_high_mono_count_t *get_next_high_mono_count;
    efi_reset_system_t *reset_system;
    struct efi_memory_map memmap;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct efi {
    const efi_runtime_services_t *runtime;
    unsigned int runtime_version;
    unsigned int runtime_supported_mask;
    long unsigned int acpi;
    long unsigned int acpi20;
    long unsigned int smbios;
    long unsigned int smbios3;
    long unsigned int esrt;
    long unsigned int tpm_log;
    long unsigned int tpm_final_log;
    long unsigned int mokvar_table;
    long unsigned int coco_secret;
    long unsigned int unaccepted;
    efi_get_time_t *get_time;
    efi_set_time_t *set_time;
    efi_get_wakeup_time_t *get_wakeup_time;
    efi_set_wakeup_time_t *set_wakeup_time;
    efi_get_variable_t *get_variable;
    efi_get_next_variable_t *get_next_variable;
    efi_set_variable_t *set_variable;
    efi_set_variable_t *set_variable_nonblocking;
    efi_query_variable_info_t *query_variable_info;
    efi_query_variable_info_t *query_variable_info_nonblocking;
    efi_update_capsule_t *update_capsule;
    efi_query_capsule_caps_t *query_capsule_caps;
    efi_get_next_high_mono_count_t *get_next_high_mono_count;
    efi_reset_system_t *reset_system;
    struct efi_memory_map memmap;
    long unsigned int flags;
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
struct efi {
    efi_system_table_t *systab;
    unsigned int runtime_version;
    long unsigned int mps;
    long unsigned int acpi;
    long unsigned int acpi20;
    long unsigned int smbios;
    long unsigned int smbios3;
    long unsigned int boot_info;
    long unsigned int hcdp;
    long unsigned int uga;
    long unsigned int fw_vendor;
    long unsigned int runtime;
    long unsigned int config_table;
    long unsigned int esrt;
    long unsigned int properties_table;
    long unsigned int mem_attr_table;
    long unsigned int rng_seed;
    long unsigned int tpm_log;
    long unsigned int tpm_final_log;
    long unsigned int mem_reserve;
    efi_get_time_t *get_time;
    efi_set_time_t *set_time;
    efi_get_wakeup_time_t *get_wakeup_time;
    efi_set_wakeup_time_t *set_wakeup_time;
    efi_get_variable_t *get_variable;
    efi_get_next_variable_t *get_next_variable;
    efi_set_variable_t *set_variable;
    efi_set_variable_t *set_variable_nonblocking;
    efi_query_variable_info_t *query_variable_info;
    efi_query_variable_info_t *query_variable_info_nonblocking;
    efi_update_capsule_t *update_capsule;
    efi_query_capsule_caps_t *query_capsule_caps;
    efi_get_next_high_mono_count_t *get_next_high_mono_count;
    efi_reset_system_t *reset_system;
    efi_set_virtual_address_map_t *set_virtual_address_map;
    struct efi_memory_map memmap;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct efi {
    efi_system_table_t *systab;
    unsigned int runtime_version;
    long unsigned int mps;
    long unsigned int acpi;
    long unsigned int acpi20;
    long unsigned int smbios;
    long unsigned int smbios3;
    long unsigned int boot_info;
    long unsigned int hcdp;
    long unsigned int uga;
    long unsigned int fw_vendor;
    long unsigned int runtime;
    long unsigned int config_table;
    long unsigned int esrt;
    long unsigned int properties_table;
    long unsigned int mem_attr_table;
    long unsigned int rng_seed;
    long unsigned int tpm_log;
    long unsigned int tpm_final_log;
    long unsigned int mem_reserve;
    efi_get_time_t *get_time;
    efi_set_time_t *set_time;
    efi_get_wakeup_time_t *get_wakeup_time;
    efi_set_wakeup_time_t *set_wakeup_time;
    efi_get_variable_t *get_variable;
    efi_get_next_variable_t *get_next_variable;
    efi_set_variable_t *set_variable;
    efi_set_variable_t *set_variable_nonblocking;
    efi_query_variable_info_t *query_variable_info;
    efi_query_variable_info_t *query_variable_info_nonblocking;
    efi_update_capsule_t *update_capsule;
    efi_query_capsule_caps_t *query_capsule_caps;
    efi_get_next_high_mono_count_t *get_next_high_mono_count;
    efi_reset_system_t *reset_system;
    efi_set_virtual_address_map_t *set_virtual_address_map;
    struct efi_memory_map memmap;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct efi {
    efi_system_table_t *systab;
    unsigned int runtime_version;
    long unsigned int mps;
    long unsigned int acpi;
    long unsigned int acpi20;
    long unsigned int smbios;
    long unsigned int smbios3;
    long unsigned int boot_info;
    long unsigned int hcdp;
    long unsigned int uga;
    long unsigned int fw_vendor;
    long unsigned int runtime;
    long unsigned int config_table;
    long unsigned int esrt;
    long unsigned int properties_table;
    long unsigned int mem_attr_table;
    long unsigned int rng_seed;
    long unsigned int tpm_log;
    long unsigned int tpm_final_log;
    long unsigned int mem_reserve;
    efi_get_time_t *get_time;
    efi_set_time_t *set_time;
    efi_get_wakeup_time_t *get_wakeup_time;
    efi_set_wakeup_time_t *set_wakeup_time;
    efi_get_variable_t *get_variable;
    efi_get_next_variable_t *get_next_variable;
    efi_set_variable_t *set_variable;
    efi_set_variable_t *set_variable_nonblocking;
    efi_query_variable_info_t *query_variable_info;
    efi_query_variable_info_t *query_variable_info_nonblocking;
    efi_update_capsule_t *update_capsule;
    efi_query_capsule_caps_t *query_capsule_caps;
    efi_get_next_high_mono_count_t *get_next_high_mono_count;
    efi_reset_system_t *reset_system;
    efi_set_virtual_address_map_t *set_virtual_address_map;
    struct efi_memory_map memmap;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct efi {
    efi_system_table_t *systab;
    unsigned int runtime_version;
    long unsigned int mps;
    long unsigned int acpi;
    long unsigned int acpi20;
    long unsigned int smbios;
    long unsigned int smbios3;
    long unsigned int boot_info;
    long unsigned int hcdp;
    long unsigned int uga;
    long unsigned int fw_vendor;
    long unsigned int runtime;
    long unsigned int config_table;
    long unsigned int esrt;
    long unsigned int properties_table;
    long unsigned int mem_attr_table;
    long unsigned int rng_seed;
    long unsigned int tpm_log;
    long unsigned int tpm_final_log;
    long unsigned int mem_reserve;
    efi_get_time_t *get_time;
    efi_set_time_t *set_time;
    efi_get_wakeup_time_t *get_wakeup_time;
    efi_set_wakeup_time_t *set_wakeup_time;
    efi_get_variable_t *get_variable;
    efi_get_next_variable_t *get_next_variable;
    efi_set_variable_t *set_variable;
    efi_set_variable_t *set_variable_nonblocking;
    efi_query_variable_info_t *query_variable_info;
    efi_query_variable_info_t *query_variable_info_nonblocking;
    efi_update_capsule_t *update_capsule;
    efi_query_capsule_caps_t *query_capsule_caps;
    efi_get_next_high_mono_count_t *get_next_high_mono_count;
    efi_reset_system_t *reset_system;
    efi_set_virtual_address_map_t *set_virtual_address_map;
    struct efi_memory_map memmap;
    long unsigned int flags;
};
```
</details>
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct efi {
    efi_system_table_t *systab;
    unsigned int runtime_version;
    long unsigned int mps;
    long unsigned int acpi;
    long unsigned int acpi20;
    long unsigned int smbios;
    long unsigned int smbios3;
    long unsigned int boot_info;
    long unsigned int hcdp;
    long unsigned int uga;
    long unsigned int fw_vendor;
    long unsigned int runtime;
    long unsigned int config_table;
    long unsigned int esrt;
    long unsigned int properties_table;
    long unsigned int mem_attr_table;
    long unsigned int rng_seed;
    long unsigned int tpm_log;
    long unsigned int tpm_final_log;
    long unsigned int mem_reserve;
    efi_get_time_t *get_time;
    efi_set_time_t *set_time;
    efi_get_wakeup_time_t *get_wakeup_time;
    efi_set_wakeup_time_t *set_wakeup_time;
    efi_get_variable_t *get_variable;
    efi_get_next_variable_t *get_next_variable;
    efi_set_variable_t *set_variable;
    efi_set_variable_t *set_variable_nonblocking;
    efi_query_variable_info_t *query_variable_info;
    efi_query_variable_info_t *query_variable_info_nonblocking;
    efi_update_capsule_t *update_capsule;
    efi_query_capsule_caps_t *query_capsule_caps;
    efi_get_next_high_mono_count_t *get_next_high_mono_count;
    efi_reset_system_t *reset_system;
    efi_set_virtual_address_map_t *set_virtual_address_map;
    struct efi_memory_map memmap;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct efi {
    efi_system_table_t *systab;
    unsigned int runtime_version;
    long unsigned int mps;
    long unsigned int acpi;
    long unsigned int acpi20;
    long unsigned int smbios;
    long unsigned int smbios3;
    long unsigned int boot_info;
    long unsigned int hcdp;
    long unsigned int uga;
    long unsigned int fw_vendor;
    long unsigned int runtime;
    long unsigned int config_table;
    long unsigned int esrt;
    long unsigned int properties_table;
    long unsigned int mem_attr_table;
    long unsigned int rng_seed;
    long unsigned int tpm_log;
    long unsigned int tpm_final_log;
    long unsigned int mem_reserve;
    efi_get_time_t *get_time;
    efi_set_time_t *set_time;
    efi_get_wakeup_time_t *get_wakeup_time;
    efi_set_wakeup_time_t *set_wakeup_time;
    efi_get_variable_t *get_variable;
    efi_get_next_variable_t *get_next_variable;
    efi_set_variable_t *set_variable;
    efi_set_variable_t *set_variable_nonblocking;
    efi_query_variable_info_t *query_variable_info;
    efi_query_variable_info_t *query_variable_info_nonblocking;
    efi_update_capsule_t *update_capsule;
    efi_query_capsule_caps_t *query_capsule_caps;
    efi_get_next_high_mono_count_t *get_next_high_mono_count;
    efi_reset_system_t *reset_system;
    efi_set_virtual_address_map_t *set_virtual_address_map;
    struct efi_memory_map memmap;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct efi {
    efi_system_table_t *systab;
    unsigned int runtime_version;
    long unsigned int mps;
    long unsigned int acpi;
    long unsigned int acpi20;
    long unsigned int smbios;
    long unsigned int smbios3;
    long unsigned int boot_info;
    long unsigned int hcdp;
    long unsigned int uga;
    long unsigned int fw_vendor;
    long unsigned int runtime;
    long unsigned int config_table;
    long unsigned int esrt;
    long unsigned int properties_table;
    long unsigned int mem_attr_table;
    long unsigned int rng_seed;
    long unsigned int tpm_log;
    long unsigned int tpm_final_log;
    long unsigned int mem_reserve;
    efi_get_time_t *get_time;
    efi_set_time_t *set_time;
    efi_get_wakeup_time_t *get_wakeup_time;
    efi_set_wakeup_time_t *set_wakeup_time;
    efi_get_variable_t *get_variable;
    efi_get_next_variable_t *get_next_variable;
    efi_set_variable_t *set_variable;
    efi_set_variable_t *set_variable_nonblocking;
    efi_query_variable_info_t *query_variable_info;
    efi_query_variable_info_t *query_variable_info_nonblocking;
    efi_update_capsule_t *update_capsule;
    efi_query_capsule_caps_t *query_capsule_caps;
    efi_get_next_high_mono_count_t *get_next_high_mono_count;
    efi_reset_system_t *reset_system;
    efi_set_virtual_address_map_t *set_virtual_address_map;
    struct efi_memory_map memmap;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct efi {
    efi_system_table_t *systab;
    unsigned int runtime_version;
    long unsigned int mps;
    long unsigned int acpi;
    long unsigned int acpi20;
    long unsigned int smbios;
    long unsigned int smbios3;
    long unsigned int boot_info;
    long unsigned int hcdp;
    long unsigned int uga;
    long unsigned int fw_vendor;
    long unsigned int runtime;
    long unsigned int config_table;
    long unsigned int esrt;
    long unsigned int properties_table;
    long unsigned int mem_attr_table;
    long unsigned int rng_seed;
    long unsigned int tpm_log;
    long unsigned int tpm_final_log;
    long unsigned int mem_reserve;
    efi_get_time_t *get_time;
    efi_set_time_t *set_time;
    efi_get_wakeup_time_t *get_wakeup_time;
    efi_set_wakeup_time_t *set_wakeup_time;
    efi_get_variable_t *get_variable;
    efi_get_next_variable_t *get_next_variable;
    efi_set_variable_t *set_variable;
    efi_set_variable_t *set_variable_nonblocking;
    efi_query_variable_info_t *query_variable_info;
    efi_query_variable_info_t *query_variable_info_nonblocking;
    efi_update_capsule_t *update_capsule;
    efi_query_capsule_caps_t *query_capsule_caps;
    efi_get_next_high_mono_count_t *get_next_high_mono_count;
    efi_reset_system_t *reset_system;
    efi_set_virtual_address_map_t *set_virtual_address_map;
    struct efi_memory_map memmap;
    long unsigned int flags;
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
<b>Field added. </b>
<code>long unsigned int mem_attr_table</code>
</li>
<li>
<b>Field added. </b>
<code>efi_query_variable_info_t *query_variable_info_nonblocking</code>
</li>
<li>
<b>Field type changed. </b>
<code>efi_set_variable_nonblocking_t *set_variable_nonblocking</code> ➡️ <code>efi_set_variable_t *set_variable_nonblocking</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct efi_memory_map *memmap</code> ➡️ <code>struct efi_memory_map memmap</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int rng_seed</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int tpm_log</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int mem_reserve</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int tpm_final_log</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>long unsigned int sal_systab</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int uv_systab</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int runtime_supported_mask</code>
</li>
<li>
<b>Field removed. </b>
<code>efi_system_table_t *systab</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int mps</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int boot_info</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int hcdp</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int uga</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int fw_vendor</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int config_table</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int properties_table</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int mem_attr_table</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int rng_seed</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int mem_reserve</code>
</li>
<li>
<b>Field removed. </b>
<code>efi_set_virtual_address_map_t *set_virtual_address_map</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int runtime</code> ➡️ <code>const efi_runtime_services_t *runtime</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int mokvar_table</code>
</li>
</ul>
</details>
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
<code>long unsigned int coco_secret</code>
</li>
</ul>
</details>
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
<code>long unsigned int unaccepted</code>
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
<li>
No changes between <code>amd64</code> and <code>armhf</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>riscv64</code> ✅
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
