# Struct: <code>apic</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct apic {
    char *name;
    int (*probe)();
    int (*acpi_madt_oem_check)(char *, char *);
    int (*apic_id_valid)(int);
    int (*apic_id_registered)();
    u32 irq_delivery_mode;
    u32 irq_dest_mode;
    const struct cpumask * (*target_cpus)();
    int disable_esr;
    int dest_logical;
    long unsigned int (*check_apicid_used)(physid_mask_t *, int);
    void (*vector_allocation_domain)(int, struct cpumask *, const struct cpumask *);
    void (*init_apic_ldr)();
    void (*ioapic_phys_id_map)(physid_mask_t *, physid_mask_t *);
    void (*setup_apic_routing)();
    int (*cpu_present_to_apicid)(int);
    void (*apicid_to_cpu_present)(int, physid_mask_t *);
    int (*check_phys_apicid_present)(int);
    int (*phys_pkg_id)(int, int);
    unsigned int (*get_apic_id)(long unsigned int);
    long unsigned int (*set_apic_id)(unsigned int);
    long unsigned int apic_id_mask;
    int (*cpu_mask_to_apicid_and)(const struct cpumask *, const struct cpumask *, unsigned int *);
    void (*send_IPI_mask)(const struct cpumask *, int);
    void (*send_IPI_mask_allbutself)(const struct cpumask *, int);
    void (*send_IPI_allbutself)(int);
    void (*send_IPI_all)(int);
    void (*send_IPI_self)(int);
    int (*wakeup_secondary_cpu)(int, long unsigned int);
    void (*inquire_remote_apic)(int);
    u32 (*read)(u32);
    void (*write)(u32, u32);
    void (*eoi_write)(u32, u32);
    u64 (*icr_read)();
    void (*icr_write)(u32, u32);
    void (*wait_icr_idle)();
    u32 (*safe_wait_icr_idle)();
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct apic {
    char *name;
    int (*probe)();
    int (*acpi_madt_oem_check)(char *, char *);
    int (*apic_id_valid)(int);
    int (*apic_id_registered)();
    u32 irq_delivery_mode;
    u32 irq_dest_mode;
    const struct cpumask * (*target_cpus)();
    int disable_esr;
    int dest_logical;
    long unsigned int (*check_apicid_used)(physid_mask_t *, int);
    void (*vector_allocation_domain)(int, struct cpumask *, const struct cpumask *);
    void (*init_apic_ldr)();
    void (*ioapic_phys_id_map)(physid_mask_t *, physid_mask_t *);
    void (*setup_apic_routing)();
    int (*cpu_present_to_apicid)(int);
    void (*apicid_to_cpu_present)(int, physid_mask_t *);
    int (*check_phys_apicid_present)(int);
    int (*phys_pkg_id)(int, int);
    unsigned int (*get_apic_id)(long unsigned int);
    long unsigned int (*set_apic_id)(unsigned int);
    int (*cpu_mask_to_apicid_and)(const struct cpumask *, const struct cpumask *, unsigned int *);
    void (*send_IPI)(int, int);
    void (*send_IPI_mask)(const struct cpumask *, int);
    void (*send_IPI_mask_allbutself)(const struct cpumask *, int);
    void (*send_IPI_allbutself)(int);
    void (*send_IPI_all)(int);
    void (*send_IPI_self)(int);
    int (*wakeup_secondary_cpu)(int, long unsigned int);
    void (*inquire_remote_apic)(int);
    u32 (*read)(u32);
    void (*write)(u32, u32);
    void (*eoi_write)(u32, u32);
    u64 (*icr_read)();
    void (*icr_write)(u32, u32);
    void (*wait_icr_idle)();
    u32 (*safe_wait_icr_idle)();
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct apic {
    char *name;
    int (*probe)();
    int (*acpi_madt_oem_check)(char *, char *);
    int (*apic_id_valid)(int);
    int (*apic_id_registered)();
    u32 irq_delivery_mode;
    u32 irq_dest_mode;
    const struct cpumask * (*target_cpus)();
    int disable_esr;
    int dest_logical;
    long unsigned int (*check_apicid_used)(physid_mask_t *, int);
    void (*vector_allocation_domain)(int, struct cpumask *, const struct cpumask *);
    void (*init_apic_ldr)();
    void (*ioapic_phys_id_map)(physid_mask_t *, physid_mask_t *);
    void (*setup_apic_routing)();
    int (*cpu_present_to_apicid)(int);
    void (*apicid_to_cpu_present)(int, physid_mask_t *);
    int (*check_phys_apicid_present)(int);
    int (*phys_pkg_id)(int, int);
    unsigned int (*get_apic_id)(long unsigned int);
    long unsigned int (*set_apic_id)(unsigned int);
    int (*cpu_mask_to_apicid_and)(const struct cpumask *, const struct cpumask *, unsigned int *);
    void (*send_IPI)(int, int);
    void (*send_IPI_mask)(const struct cpumask *, int);
    void (*send_IPI_mask_allbutself)(const struct cpumask *, int);
    void (*send_IPI_allbutself)(int);
    void (*send_IPI_all)(int);
    void (*send_IPI_self)(int);
    int (*wakeup_secondary_cpu)(int, long unsigned int);
    void (*inquire_remote_apic)(int);
    u32 (*read)(u32);
    void (*write)(u32, u32);
    void (*eoi_write)(u32, u32);
    void (*native_eoi_write)(u32, u32);
    u64 (*icr_read)();
    void (*icr_write)(u32, u32);
    void (*wait_icr_idle)();
    u32 (*safe_wait_icr_idle)();
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct apic {
    char *name;
    int (*probe)();
    int (*acpi_madt_oem_check)(char *, char *);
    int (*apic_id_valid)(int);
    int (*apic_id_registered)();
    u32 irq_delivery_mode;
    u32 irq_dest_mode;
    const struct cpumask * (*target_cpus)();
    int disable_esr;
    int dest_logical;
    long unsigned int (*check_apicid_used)(physid_mask_t *, int);
    void (*vector_allocation_domain)(int, struct cpumask *, const struct cpumask *);
    void (*init_apic_ldr)();
    void (*ioapic_phys_id_map)(physid_mask_t *, physid_mask_t *);
    void (*setup_apic_routing)();
    int (*cpu_present_to_apicid)(int);
    void (*apicid_to_cpu_present)(int, physid_mask_t *);
    int (*check_phys_apicid_present)(int);
    int (*phys_pkg_id)(int, int);
    unsigned int (*get_apic_id)(long unsigned int);
    long unsigned int (*set_apic_id)(unsigned int);
    int (*cpu_mask_to_apicid)(const struct cpumask *, struct irq_data *, unsigned int *);
    void (*send_IPI)(int, int);
    void (*send_IPI_mask)(const struct cpumask *, int);
    void (*send_IPI_mask_allbutself)(const struct cpumask *, int);
    void (*send_IPI_allbutself)(int);
    void (*send_IPI_all)(int);
    void (*send_IPI_self)(int);
    int (*wakeup_secondary_cpu)(int, long unsigned int);
    void (*inquire_remote_apic)(int);
    u32 (*read)(u32);
    void (*write)(u32, u32);
    void (*eoi_write)(u32, u32);
    void (*native_eoi_write)(u32, u32);
    u64 (*icr_read)();
    void (*icr_write)(u32, u32);
    void (*wait_icr_idle)();
    u32 (*safe_wait_icr_idle)();
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct apic {
    void (*eoi_write)(u32, u32);
    void (*native_eoi_write)(u32, u32);
    void (*write)(u32, u32);
    u32 (*read)(u32);
    void (*wait_icr_idle)();
    u32 (*safe_wait_icr_idle)();
    void (*send_IPI)(int, int);
    void (*send_IPI_mask)(const struct cpumask *, int);
    void (*send_IPI_mask_allbutself)(const struct cpumask *, int);
    void (*send_IPI_allbutself)(int);
    void (*send_IPI_all)(int);
    void (*send_IPI_self)(int);
    u32 dest_logical;
    u32 disable_esr;
    u32 irq_delivery_mode;
    u32 irq_dest_mode;
    void (*vector_allocation_domain)(int, struct cpumask *, const struct cpumask *);
    int (*cpu_mask_to_apicid)(const struct cpumask *, struct irq_data *, unsigned int *);
    u32 (*calc_dest_apicid)(unsigned int);
    u64 (*icr_read)();
    void (*icr_write)(u32, u32);
    int (*probe)();
    int (*acpi_madt_oem_check)(char *, char *);
    int (*apic_id_valid)(int);
    int (*apic_id_registered)();
    bool (*check_apicid_used)(physid_mask_t *, int);
    void (*init_apic_ldr)();
    void (*ioapic_phys_id_map)(physid_mask_t *, physid_mask_t *);
    void (*setup_apic_routing)();
    int (*cpu_present_to_apicid)(int);
    void (*apicid_to_cpu_present)(int, physid_mask_t *);
    int (*check_phys_apicid_present)(int);
    int (*phys_pkg_id)(int, int);
    u32 (*get_apic_id)(long unsigned int);
    u32 (*set_apic_id)(unsigned int);
    int (*wakeup_secondary_cpu)(int, long unsigned int);
    void (*inquire_remote_apic)(int);
    char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct apic {
    void (*eoi_write)(u32, u32);
    void (*native_eoi_write)(u32, u32);
    void (*write)(u32, u32);
    u32 (*read)(u32);
    void (*wait_icr_idle)();
    u32 (*safe_wait_icr_idle)();
    void (*send_IPI)(int, int);
    void (*send_IPI_mask)(const struct cpumask *, int);
    void (*send_IPI_mask_allbutself)(const struct cpumask *, int);
    void (*send_IPI_allbutself)(int);
    void (*send_IPI_all)(int);
    void (*send_IPI_self)(int);
    u32 dest_logical;
    u32 disable_esr;
    u32 irq_delivery_mode;
    u32 irq_dest_mode;
    u32 (*calc_dest_apicid)(unsigned int);
    u64 (*icr_read)();
    void (*icr_write)(u32, u32);
    int (*probe)();
    int (*acpi_madt_oem_check)(char *, char *);
    int (*apic_id_valid)(u32);
    int (*apic_id_registered)();
    bool (*check_apicid_used)(physid_mask_t *, int);
    void (*init_apic_ldr)();
    void (*ioapic_phys_id_map)(physid_mask_t *, physid_mask_t *);
    void (*setup_apic_routing)();
    int (*cpu_present_to_apicid)(int);
    void (*apicid_to_cpu_present)(int, physid_mask_t *);
    int (*check_phys_apicid_present)(int);
    int (*phys_pkg_id)(int, int);
    u32 (*get_apic_id)(long unsigned int);
    u32 (*set_apic_id)(unsigned int);
    int (*wakeup_secondary_cpu)(int, long unsigned int);
    void (*inquire_remote_apic)(int);
    char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct apic {
    void (*eoi_write)(u32, u32);
    void (*native_eoi_write)(u32, u32);
    void (*write)(u32, u32);
    u32 (*read)(u32);
    void (*wait_icr_idle)();
    u32 (*safe_wait_icr_idle)();
    void (*send_IPI)(int, int);
    void (*send_IPI_mask)(const struct cpumask *, int);
    void (*send_IPI_mask_allbutself)(const struct cpumask *, int);
    void (*send_IPI_allbutself)(int);
    void (*send_IPI_all)(int);
    void (*send_IPI_self)(int);
    u32 dest_logical;
    u32 disable_esr;
    u32 irq_delivery_mode;
    u32 irq_dest_mode;
    u32 (*calc_dest_apicid)(unsigned int);
    u64 (*icr_read)();
    void (*icr_write)(u32, u32);
    int (*probe)();
    int (*acpi_madt_oem_check)(char *, char *);
    int (*apic_id_valid)(u32);
    int (*apic_id_registered)();
    bool (*check_apicid_used)(physid_mask_t *, int);
    void (*init_apic_ldr)();
    void (*ioapic_phys_id_map)(physid_mask_t *, physid_mask_t *);
    void (*setup_apic_routing)();
    int (*cpu_present_to_apicid)(int);
    void (*apicid_to_cpu_present)(int, physid_mask_t *);
    int (*check_phys_apicid_present)(int);
    int (*phys_pkg_id)(int, int);
    u32 (*get_apic_id)(long unsigned int);
    u32 (*set_apic_id)(unsigned int);
    int (*wakeup_secondary_cpu)(int, long unsigned int);
    void (*inquire_remote_apic)(int);
    char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct apic {
    void (*eoi_write)(u32, u32);
    void (*native_eoi_write)(u32, u32);
    void (*write)(u32, u32);
    u32 (*read)(u32);
    void (*wait_icr_idle)();
    u32 (*safe_wait_icr_idle)();
    void (*send_IPI)(int, int);
    void (*send_IPI_mask)(const struct cpumask *, int);
    void (*send_IPI_mask_allbutself)(const struct cpumask *, int);
    void (*send_IPI_allbutself)(int);
    void (*send_IPI_all)(int);
    void (*send_IPI_self)(int);
    u32 dest_logical;
    u32 disable_esr;
    u32 irq_delivery_mode;
    u32 irq_dest_mode;
    u32 (*calc_dest_apicid)(unsigned int);
    u64 (*icr_read)();
    void (*icr_write)(u32, u32);
    int (*probe)();
    int (*acpi_madt_oem_check)(char *, char *);
    int (*apic_id_valid)(u32);
    int (*apic_id_registered)();
    bool (*check_apicid_used)(physid_mask_t *, int);
    void (*init_apic_ldr)();
    void (*ioapic_phys_id_map)(physid_mask_t *, physid_mask_t *);
    void (*setup_apic_routing)();
    int (*cpu_present_to_apicid)(int);
    void (*apicid_to_cpu_present)(int, physid_mask_t *);
    int (*check_phys_apicid_present)(int);
    int (*phys_pkg_id)(int, int);
    u32 (*get_apic_id)(long unsigned int);
    u32 (*set_apic_id)(unsigned int);
    int (*wakeup_secondary_cpu)(int, long unsigned int);
    void (*inquire_remote_apic)(int);
    char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct apic {
    void (*eoi_write)(u32, u32);
    void (*native_eoi_write)(u32, u32);
    void (*write)(u32, u32);
    u32 (*read)(u32);
    void (*wait_icr_idle)();
    u32 (*safe_wait_icr_idle)();
    void (*send_IPI)(int, int);
    void (*send_IPI_mask)(const struct cpumask *, int);
    void (*send_IPI_mask_allbutself)(const struct cpumask *, int);
    void (*send_IPI_allbutself)(int);
    void (*send_IPI_all)(int);
    void (*send_IPI_self)(int);
    u32 dest_logical;
    u32 disable_esr;
    u32 irq_delivery_mode;
    u32 irq_dest_mode;
    u32 (*calc_dest_apicid)(unsigned int);
    u64 (*icr_read)();
    void (*icr_write)(u32, u32);
    int (*probe)();
    int (*acpi_madt_oem_check)(char *, char *);
    int (*apic_id_valid)(u32);
    int (*apic_id_registered)();
    bool (*check_apicid_used)(physid_mask_t *, int);
    void (*init_apic_ldr)();
    void (*ioapic_phys_id_map)(physid_mask_t *, physid_mask_t *);
    void (*setup_apic_routing)();
    int (*cpu_present_to_apicid)(int);
    void (*apicid_to_cpu_present)(int, physid_mask_t *);
    int (*check_phys_apicid_present)(int);
    int (*phys_pkg_id)(int, int);
    u32 (*get_apic_id)(long unsigned int);
    u32 (*set_apic_id)(unsigned int);
    int (*wakeup_secondary_cpu)(int, long unsigned int);
    void (*inquire_remote_apic)(int);
    char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct apic {
    void (*eoi_write)(u32, u32);
    void (*native_eoi_write)(u32, u32);
    void (*write)(u32, u32);
    u32 (*read)(u32);
    void (*wait_icr_idle)();
    u32 (*safe_wait_icr_idle)();
    void (*send_IPI)(int, int);
    void (*send_IPI_mask)(const struct cpumask *, int);
    void (*send_IPI_mask_allbutself)(const struct cpumask *, int);
    void (*send_IPI_allbutself)(int);
    void (*send_IPI_all)(int);
    void (*send_IPI_self)(int);
    u32 dest_logical;
    u32 disable_esr;
    u32 irq_delivery_mode;
    u32 irq_dest_mode;
    u32 (*calc_dest_apicid)(unsigned int);
    u64 (*icr_read)();
    void (*icr_write)(u32, u32);
    int (*probe)();
    int (*acpi_madt_oem_check)(char *, char *);
    int (*apic_id_valid)(u32);
    int (*apic_id_registered)();
    bool (*check_apicid_used)(physid_mask_t *, int);
    void (*init_apic_ldr)();
    void (*ioapic_phys_id_map)(physid_mask_t *, physid_mask_t *);
    void (*setup_apic_routing)();
    int (*cpu_present_to_apicid)(int);
    void (*apicid_to_cpu_present)(int, physid_mask_t *);
    int (*check_phys_apicid_present)(int);
    int (*phys_pkg_id)(int, int);
    u32 (*get_apic_id)(long unsigned int);
    u32 (*set_apic_id)(unsigned int);
    int (*wakeup_secondary_cpu)(int, long unsigned int);
    void (*inquire_remote_apic)(int);
    char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct apic {
    void (*eoi_write)(u32, u32);
    void (*native_eoi_write)(u32, u32);
    void (*write)(u32, u32);
    u32 (*read)(u32);
    void (*wait_icr_idle)();
    u32 (*safe_wait_icr_idle)();
    void (*send_IPI)(int, int);
    void (*send_IPI_mask)(const struct cpumask *, int);
    void (*send_IPI_mask_allbutself)(const struct cpumask *, int);
    void (*send_IPI_allbutself)(int);
    void (*send_IPI_all)(int);
    void (*send_IPI_self)(int);
    u32 disable_esr;
    enum apic_delivery_modes delivery_mode;
    bool dest_mode_logical;
    u32 (*calc_dest_apicid)(unsigned int);
    u64 (*icr_read)();
    void (*icr_write)(u32, u32);
    int (*probe)();
    int (*acpi_madt_oem_check)(char *, char *);
    int (*apic_id_valid)(u32);
    int (*apic_id_registered)();
    bool (*check_apicid_used)(physid_mask_t *, int);
    void (*init_apic_ldr)();
    void (*ioapic_phys_id_map)(physid_mask_t *, physid_mask_t *);
    void (*setup_apic_routing)();
    int (*cpu_present_to_apicid)(int);
    void (*apicid_to_cpu_present)(int, physid_mask_t *);
    int (*check_phys_apicid_present)(int);
    int (*phys_pkg_id)(int, int);
    u32 (*get_apic_id)(long unsigned int);
    u32 (*set_apic_id)(unsigned int);
    int (*wakeup_secondary_cpu)(int, long unsigned int);
    void (*inquire_remote_apic)(int);
    char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct apic {
    void (*eoi_write)(u32, u32);
    void (*native_eoi_write)(u32, u32);
    void (*write)(u32, u32);
    u32 (*read)(u32);
    void (*wait_icr_idle)();
    u32 (*safe_wait_icr_idle)();
    void (*send_IPI)(int, int);
    void (*send_IPI_mask)(const struct cpumask *, int);
    void (*send_IPI_mask_allbutself)(const struct cpumask *, int);
    void (*send_IPI_allbutself)(int);
    void (*send_IPI_all)(int);
    void (*send_IPI_self)(int);
    u32 disable_esr;
    enum apic_delivery_modes delivery_mode;
    bool dest_mode_logical;
    u32 (*calc_dest_apicid)(unsigned int);
    u64 (*icr_read)();
    void (*icr_write)(u32, u32);
    int (*probe)();
    int (*acpi_madt_oem_check)(char *, char *);
    int (*apic_id_valid)(u32);
    int (*apic_id_registered)();
    bool (*check_apicid_used)(physid_mask_t *, int);
    void (*init_apic_ldr)();
    void (*ioapic_phys_id_map)(physid_mask_t *, physid_mask_t *);
    void (*setup_apic_routing)();
    int (*cpu_present_to_apicid)(int);
    void (*apicid_to_cpu_present)(int, physid_mask_t *);
    int (*check_phys_apicid_present)(int);
    int (*phys_pkg_id)(int, int);
    u32 (*get_apic_id)(long unsigned int);
    u32 (*set_apic_id)(unsigned int);
    int (*wakeup_secondary_cpu)(int, long unsigned int);
    void (*inquire_remote_apic)(int);
    char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct apic {
    void (*eoi_write)(u32, u32);
    void (*native_eoi_write)(u32, u32);
    void (*write)(u32, u32);
    u32 (*read)(u32);
    void (*wait_icr_idle)();
    u32 (*safe_wait_icr_idle)();
    void (*send_IPI)(int, int);
    void (*send_IPI_mask)(const struct cpumask *, int);
    void (*send_IPI_mask_allbutself)(const struct cpumask *, int);
    void (*send_IPI_allbutself)(int);
    void (*send_IPI_all)(int);
    void (*send_IPI_self)(int);
    u32 disable_esr;
    enum apic_delivery_modes delivery_mode;
    bool dest_mode_logical;
    u32 (*calc_dest_apicid)(unsigned int);
    u64 (*icr_read)();
    void (*icr_write)(u32, u32);
    int (*probe)();
    int (*acpi_madt_oem_check)(char *, char *);
    int (*apic_id_valid)(u32);
    int (*apic_id_registered)();
    bool (*check_apicid_used)(physid_mask_t *, int);
    void (*init_apic_ldr)();
    void (*ioapic_phys_id_map)(physid_mask_t *, physid_mask_t *);
    void (*setup_apic_routing)();
    int (*cpu_present_to_apicid)(int);
    void (*apicid_to_cpu_present)(int, physid_mask_t *);
    int (*check_phys_apicid_present)(int);
    int (*phys_pkg_id)(int, int);
    u32 (*get_apic_id)(long unsigned int);
    u32 (*set_apic_id)(unsigned int);
    int (*wakeup_secondary_cpu)(int, long unsigned int);
    void (*inquire_remote_apic)(int);
    char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct apic {
    void (*eoi_write)(u32, u32);
    void (*native_eoi_write)(u32, u32);
    void (*write)(u32, u32);
    u32 (*read)(u32);
    void (*wait_icr_idle)();
    u32 (*safe_wait_icr_idle)();
    void (*send_IPI)(int, int);
    void (*send_IPI_mask)(const struct cpumask *, int);
    void (*send_IPI_mask_allbutself)(const struct cpumask *, int);
    void (*send_IPI_allbutself)(int);
    void (*send_IPI_all)(int);
    void (*send_IPI_self)(int);
    u32 disable_esr;
    enum apic_delivery_modes delivery_mode;
    bool dest_mode_logical;
    u32 (*calc_dest_apicid)(unsigned int);
    u64 (*icr_read)();
    void (*icr_write)(u32, u32);
    int (*probe)();
    int (*acpi_madt_oem_check)(char *, char *);
    int (*apic_id_valid)(u32);
    int (*apic_id_registered)();
    bool (*check_apicid_used)(physid_mask_t *, int);
    void (*init_apic_ldr)();
    void (*ioapic_phys_id_map)(physid_mask_t *, physid_mask_t *);
    void (*setup_apic_routing)();
    int (*cpu_present_to_apicid)(int);
    void (*apicid_to_cpu_present)(int, physid_mask_t *);
    int (*check_phys_apicid_present)(int);
    int (*phys_pkg_id)(int, int);
    u32 (*get_apic_id)(long unsigned int);
    u32 (*set_apic_id)(unsigned int);
    int (*wakeup_secondary_cpu)(int, long unsigned int);
    int (*wakeup_secondary_cpu_64)(int, long unsigned int);
    void (*inquire_remote_apic)(int);
    char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct apic {
    void (*eoi_write)(u32, u32);
    void (*native_eoi_write)(u32, u32);
    void (*write)(u32, u32);
    u32 (*read)(u32);
    void (*wait_icr_idle)();
    u32 (*safe_wait_icr_idle)();
    void (*send_IPI)(int, int);
    void (*send_IPI_mask)(const struct cpumask *, int);
    void (*send_IPI_mask_allbutself)(const struct cpumask *, int);
    void (*send_IPI_allbutself)(int);
    void (*send_IPI_all)(int);
    void (*send_IPI_self)(int);
    u32 disable_esr;
    enum apic_delivery_modes delivery_mode;
    bool dest_mode_logical;
    u32 (*calc_dest_apicid)(unsigned int);
    u64 (*icr_read)();
    void (*icr_write)(u32, u32);
    int (*probe)();
    int (*acpi_madt_oem_check)(char *, char *);
    int (*apic_id_valid)(u32);
    int (*apic_id_registered)();
    bool (*check_apicid_used)(physid_mask_t *, int);
    void (*init_apic_ldr)();
    void (*ioapic_phys_id_map)(physid_mask_t *, physid_mask_t *);
    void (*setup_apic_routing)();
    int (*cpu_present_to_apicid)(int);
    void (*apicid_to_cpu_present)(int, physid_mask_t *);
    int (*check_phys_apicid_present)(int);
    int (*phys_pkg_id)(int, int);
    u32 (*get_apic_id)(long unsigned int);
    u32 (*set_apic_id)(unsigned int);
    int (*wakeup_secondary_cpu)(int, long unsigned int);
    int (*wakeup_secondary_cpu_64)(int, long unsigned int);
    void (*inquire_remote_apic)(int);
    char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct apic {
    void (*eoi_write)(u32, u32);
    void (*native_eoi_write)(u32, u32);
    void (*write)(u32, u32);
    u32 (*read)(u32);
    void (*wait_icr_idle)();
    u32 (*safe_wait_icr_idle)();
    void (*send_IPI)(int, int);
    void (*send_IPI_mask)(const struct cpumask *, int);
    void (*send_IPI_mask_allbutself)(const struct cpumask *, int);
    void (*send_IPI_allbutself)(int);
    void (*send_IPI_all)(int);
    void (*send_IPI_self)(int);
    u32 disable_esr;
    enum apic_delivery_modes delivery_mode;
    bool dest_mode_logical;
    u32 (*calc_dest_apicid)(unsigned int);
    u64 (*icr_read)();
    void (*icr_write)(u32, u32);
    int (*probe)();
    int (*acpi_madt_oem_check)(char *, char *);
    int (*apic_id_valid)(u32);
    int (*apic_id_registered)();
    bool (*check_apicid_used)(physid_mask_t *, int);
    void (*init_apic_ldr)();
    void (*ioapic_phys_id_map)(physid_mask_t *, physid_mask_t *);
    void (*setup_apic_routing)();
    int (*cpu_present_to_apicid)(int);
    void (*apicid_to_cpu_present)(int, physid_mask_t *);
    int (*check_phys_apicid_present)(int);
    int (*phys_pkg_id)(int, int);
    u32 (*get_apic_id)(long unsigned int);
    u32 (*set_apic_id)(unsigned int);
    int (*wakeup_secondary_cpu)(int, long unsigned int);
    int (*wakeup_secondary_cpu_64)(int, long unsigned int);
    void (*inquire_remote_apic)(int);
    char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct apic {
    void (*eoi)();
    void (*native_eoi)();
    void (*write)(u32, u32);
    u32 (*read)(u32);
    void (*wait_icr_idle)();
    u32 (*safe_wait_icr_idle)();
    void (*send_IPI)(int, int);
    void (*send_IPI_mask)(const struct cpumask *, int);
    void (*send_IPI_mask_allbutself)(const struct cpumask *, int);
    void (*send_IPI_allbutself)(int);
    void (*send_IPI_all)(int);
    void (*send_IPI_self)(int);
    u32 disable_esr;
    u32 dest_mode_logical;
    u32 x2apic_set_max_apicid;
    u32 nmi_to_offline_cpu;
    u32 (*calc_dest_apicid)(unsigned int);
    u64 (*icr_read)();
    void (*icr_write)(u32, u32);
    u32 max_apic_id;
    int (*probe)();
    int (*acpi_madt_oem_check)(char *, char *);
    bool (*apic_id_registered)();
    bool (*check_apicid_used)(physid_mask_t *, u32);
    void (*init_apic_ldr)();
    void (*ioapic_phys_id_map)(physid_mask_t *, physid_mask_t *);
    u32 (*cpu_present_to_apicid)(int);
    u32 (*phys_pkg_id)(u32, int);
    u32 (*get_apic_id)(u32);
    u32 (*set_apic_id)(u32);
    int (*wakeup_secondary_cpu)(u32, long unsigned int);
    int (*wakeup_secondary_cpu_64)(u32, long unsigned int);
    char *name;
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
struct apic {
    void (*eoi_write)(u32, u32);
    void (*native_eoi_write)(u32, u32);
    void (*write)(u32, u32);
    u32 (*read)(u32);
    void (*wait_icr_idle)();
    u32 (*safe_wait_icr_idle)();
    void (*send_IPI)(int, int);
    void (*send_IPI_mask)(const struct cpumask *, int);
    void (*send_IPI_mask_allbutself)(const struct cpumask *, int);
    void (*send_IPI_allbutself)(int);
    void (*send_IPI_all)(int);
    void (*send_IPI_self)(int);
    u32 dest_logical;
    u32 disable_esr;
    u32 irq_delivery_mode;
    u32 irq_dest_mode;
    u32 (*calc_dest_apicid)(unsigned int);
    u64 (*icr_read)();
    void (*icr_write)(u32, u32);
    int (*probe)();
    int (*acpi_madt_oem_check)(char *, char *);
    int (*apic_id_valid)(u32);
    int (*apic_id_registered)();
    bool (*check_apicid_used)(physid_mask_t *, int);
    void (*init_apic_ldr)();
    void (*ioapic_phys_id_map)(physid_mask_t *, physid_mask_t *);
    void (*setup_apic_routing)();
    int (*cpu_present_to_apicid)(int);
    void (*apicid_to_cpu_present)(int, physid_mask_t *);
    int (*check_phys_apicid_present)(int);
    int (*phys_pkg_id)(int, int);
    u32 (*get_apic_id)(long unsigned int);
    u32 (*set_apic_id)(unsigned int);
    int (*wakeup_secondary_cpu)(int, long unsigned int);
    void (*inquire_remote_apic)(int);
    char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct apic {
    void (*eoi_write)(u32, u32);
    void (*native_eoi_write)(u32, u32);
    void (*write)(u32, u32);
    u32 (*read)(u32);
    void (*wait_icr_idle)();
    u32 (*safe_wait_icr_idle)();
    void (*send_IPI)(int, int);
    void (*send_IPI_mask)(const struct cpumask *, int);
    void (*send_IPI_mask_allbutself)(const struct cpumask *, int);
    void (*send_IPI_allbutself)(int);
    void (*send_IPI_all)(int);
    void (*send_IPI_self)(int);
    u32 dest_logical;
    u32 disable_esr;
    u32 irq_delivery_mode;
    u32 irq_dest_mode;
    u32 (*calc_dest_apicid)(unsigned int);
    u64 (*icr_read)();
    void (*icr_write)(u32, u32);
    int (*probe)();
    int (*acpi_madt_oem_check)(char *, char *);
    int (*apic_id_valid)(u32);
    int (*apic_id_registered)();
    bool (*check_apicid_used)(physid_mask_t *, int);
    void (*init_apic_ldr)();
    void (*ioapic_phys_id_map)(physid_mask_t *, physid_mask_t *);
    void (*setup_apic_routing)();
    int (*cpu_present_to_apicid)(int);
    void (*apicid_to_cpu_present)(int, physid_mask_t *);
    int (*check_phys_apicid_present)(int);
    int (*phys_pkg_id)(int, int);
    u32 (*get_apic_id)(long unsigned int);
    u32 (*set_apic_id)(unsigned int);
    int (*wakeup_secondary_cpu)(int, long unsigned int);
    void (*inquire_remote_apic)(int);
    char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct apic {
    void (*eoi_write)(u32, u32);
    void (*native_eoi_write)(u32, u32);
    void (*write)(u32, u32);
    u32 (*read)(u32);
    void (*wait_icr_idle)();
    u32 (*safe_wait_icr_idle)();
    void (*send_IPI)(int, int);
    void (*send_IPI_mask)(const struct cpumask *, int);
    void (*send_IPI_mask_allbutself)(const struct cpumask *, int);
    void (*send_IPI_allbutself)(int);
    void (*send_IPI_all)(int);
    void (*send_IPI_self)(int);
    u32 dest_logical;
    u32 disable_esr;
    u32 irq_delivery_mode;
    u32 irq_dest_mode;
    u32 (*calc_dest_apicid)(unsigned int);
    u64 (*icr_read)();
    void (*icr_write)(u32, u32);
    int (*probe)();
    int (*acpi_madt_oem_check)(char *, char *);
    int (*apic_id_valid)(u32);
    int (*apic_id_registered)();
    bool (*check_apicid_used)(physid_mask_t *, int);
    void (*init_apic_ldr)();
    void (*ioapic_phys_id_map)(physid_mask_t *, physid_mask_t *);
    void (*setup_apic_routing)();
    int (*cpu_present_to_apicid)(int);
    void (*apicid_to_cpu_present)(int, physid_mask_t *);
    int (*check_phys_apicid_present)(int);
    int (*phys_pkg_id)(int, int);
    u32 (*get_apic_id)(long unsigned int);
    u32 (*set_apic_id)(unsigned int);
    int (*wakeup_secondary_cpu)(int, long unsigned int);
    void (*inquire_remote_apic)(int);
    char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct apic {
    void (*eoi_write)(u32, u32);
    void (*native_eoi_write)(u32, u32);
    void (*write)(u32, u32);
    u32 (*read)(u32);
    void (*wait_icr_idle)();
    u32 (*safe_wait_icr_idle)();
    void (*send_IPI)(int, int);
    void (*send_IPI_mask)(const struct cpumask *, int);
    void (*send_IPI_mask_allbutself)(const struct cpumask *, int);
    void (*send_IPI_allbutself)(int);
    void (*send_IPI_all)(int);
    void (*send_IPI_self)(int);
    u32 dest_logical;
    u32 disable_esr;
    u32 irq_delivery_mode;
    u32 irq_dest_mode;
    u32 (*calc_dest_apicid)(unsigned int);
    u64 (*icr_read)();
    void (*icr_write)(u32, u32);
    int (*probe)();
    int (*acpi_madt_oem_check)(char *, char *);
    int (*apic_id_valid)(u32);
    int (*apic_id_registered)();
    bool (*check_apicid_used)(physid_mask_t *, int);
    void (*init_apic_ldr)();
    void (*ioapic_phys_id_map)(physid_mask_t *, physid_mask_t *);
    void (*setup_apic_routing)();
    int (*cpu_present_to_apicid)(int);
    void (*apicid_to_cpu_present)(int, physid_mask_t *);
    int (*check_phys_apicid_present)(int);
    int (*phys_pkg_id)(int, int);
    u32 (*get_apic_id)(long unsigned int);
    u32 (*set_apic_id)(unsigned int);
    int (*wakeup_secondary_cpu)(int, long unsigned int);
    void (*inquire_remote_apic)(int);
    char *name;
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
<code>void (*send_IPI)(int, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int apic_id_mask</code>
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
<code>void (*native_eoi_write)(u32, u32)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*cpu_mask_to_apicid)(const struct cpumask *, struct irq_data *, unsigned int *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*cpu_mask_to_apicid_and)(const struct cpumask *, const struct cpumask *, unsigned int *)</code>
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
<code>u32 (*calc_dest_apicid)(unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>const struct cpumask * (*target_cpus)()</code>
</li>
<li>
<b>Field type changed. </b>
<code>int disable_esr</code> ➡️ <code>u32 disable_esr</code>
</li>
<li>
<b>Field type changed. </b>
<code>int dest_logical</code> ➡️ <code>u32 dest_logical</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int (*check_apicid_used)(physid_mask_t *, int)</code> ➡️ <code>bool (*check_apicid_used)(physid_mask_t *, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int (*get_apic_id)(long unsigned int)</code> ➡️ <code>u32 (*get_apic_id)(long unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int (*set_apic_id)(unsigned int)</code> ➡️ <code>u32 (*set_apic_id)(unsigned int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>void (*vector_allocation_domain)(int, struct cpumask *, const struct cpumask *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*cpu_mask_to_apicid)(const struct cpumask *, struct irq_data *, unsigned int *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*apic_id_valid)(int)</code> ➡️ <code>int (*apic_id_valid)(u32)</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>enum apic_delivery_modes delivery_mode</code>
</li>
<li>
<b>Field added. </b>
<code>bool dest_mode_logical</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 dest_logical</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 irq_delivery_mode</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 irq_dest_mode</code>
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
<code>int (*wakeup_secondary_cpu_64)(int, long unsigned int)</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*eoi)()</code>
</li>
<li>
<b>Field added. </b>
<code>void (*native_eoi)()</code>
</li>
<li>
<b>Field added. </b>
<code>u32 x2apic_set_max_apicid</code>
</li>
<li>
<b>Field added. </b>
<code>u32 nmi_to_offline_cpu</code>
</li>
<li>
<b>Field added. </b>
<code>u32 max_apic_id</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*eoi_write)(u32, u32)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*native_eoi_write)(u32, u32)</code>
</li>
<li>
<b>Field removed. </b>
<code>enum apic_delivery_modes delivery_mode</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*apic_id_valid)(u32)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*setup_apic_routing)()</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*apicid_to_cpu_present)(int, physid_mask_t *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*check_phys_apicid_present)(int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*inquire_remote_apic)(int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool dest_mode_logical</code> ➡️ <code>u32 dest_mode_logical</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*apic_id_registered)()</code> ➡️ <code>bool (*apic_id_registered)()</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool (*check_apicid_used)(physid_mask_t *, int)</code> ➡️ <code>bool (*check_apicid_used)(physid_mask_t *, u32)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*cpu_present_to_apicid)(int)</code> ➡️ <code>u32 (*cpu_present_to_apicid)(int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*phys_pkg_id)(int, int)</code> ➡️ <code>u32 (*phys_pkg_id)(u32, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 (*get_apic_id)(long unsigned int)</code> ➡️ <code>u32 (*get_apic_id)(u32)</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 (*set_apic_id)(unsigned int)</code> ➡️ <code>u32 (*set_apic_id)(u32)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*wakeup_secondary_cpu)(int, long unsigned int)</code> ➡️ <code>int (*wakeup_secondary_cpu)(u32, long unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*wakeup_secondary_cpu_64)(int, long unsigned int)</code> ➡️ <code>int (*wakeup_secondary_cpu_64)(u32, long unsigned int)</code>
</li>
</ul>
</details>
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
