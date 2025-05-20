# Struct: <code>irq_chip</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct irq_chip {
    const char *name;
    unsigned int (*irq_startup)(struct irq_data *);
    void (*irq_shutdown)(struct irq_data *);
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_ack)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
    void (*irq_mask_ack)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_eoi)(struct irq_data *);
    int (*irq_set_affinity)(struct irq_data *, const struct cpumask *, bool);
    int (*irq_retrigger)(struct irq_data *);
    int (*irq_set_type)(struct irq_data *, unsigned int);
    int (*irq_set_wake)(struct irq_data *, unsigned int);
    void (*irq_bus_lock)(struct irq_data *);
    void (*irq_bus_sync_unlock)(struct irq_data *);
    void (*irq_cpu_online)(struct irq_data *);
    void (*irq_cpu_offline)(struct irq_data *);
    void (*irq_suspend)(struct irq_data *);
    void (*irq_resume)(struct irq_data *);
    void (*irq_pm_shutdown)(struct irq_data *);
    void (*irq_calc_mask)(struct irq_data *);
    void (*irq_print_chip)(struct irq_data *, struct seq_file *);
    int (*irq_request_resources)(struct irq_data *);
    void (*irq_release_resources)(struct irq_data *);
    void (*irq_compose_msi_msg)(struct irq_data *, struct msi_msg *);
    void (*irq_write_msi_msg)(struct irq_data *, struct msi_msg *);
    int (*irq_get_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool *);
    int (*irq_set_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool);
    int (*irq_set_vcpu_affinity)(struct irq_data *, void *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct irq_chip {
    struct device *parent_device;
    const char *name;
    unsigned int (*irq_startup)(struct irq_data *);
    void (*irq_shutdown)(struct irq_data *);
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_ack)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
    void (*irq_mask_ack)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_eoi)(struct irq_data *);
    int (*irq_set_affinity)(struct irq_data *, const struct cpumask *, bool);
    int (*irq_retrigger)(struct irq_data *);
    int (*irq_set_type)(struct irq_data *, unsigned int);
    int (*irq_set_wake)(struct irq_data *, unsigned int);
    void (*irq_bus_lock)(struct irq_data *);
    void (*irq_bus_sync_unlock)(struct irq_data *);
    void (*irq_cpu_online)(struct irq_data *);
    void (*irq_cpu_offline)(struct irq_data *);
    void (*irq_suspend)(struct irq_data *);
    void (*irq_resume)(struct irq_data *);
    void (*irq_pm_shutdown)(struct irq_data *);
    void (*irq_calc_mask)(struct irq_data *);
    void (*irq_print_chip)(struct irq_data *, struct seq_file *);
    int (*irq_request_resources)(struct irq_data *);
    void (*irq_release_resources)(struct irq_data *);
    void (*irq_compose_msi_msg)(struct irq_data *, struct msi_msg *);
    void (*irq_write_msi_msg)(struct irq_data *, struct msi_msg *);
    int (*irq_get_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool *);
    int (*irq_set_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool);
    int (*irq_set_vcpu_affinity)(struct irq_data *, void *);
    void (*ipi_send_single)(struct irq_data *, unsigned int);
    void (*ipi_send_mask)(struct irq_data *, const struct cpumask *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct irq_chip {
    struct device *parent_device;
    const char *name;
    unsigned int (*irq_startup)(struct irq_data *);
    void (*irq_shutdown)(struct irq_data *);
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_ack)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
    void (*irq_mask_ack)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_eoi)(struct irq_data *);
    int (*irq_set_affinity)(struct irq_data *, const struct cpumask *, bool);
    int (*irq_retrigger)(struct irq_data *);
    int (*irq_set_type)(struct irq_data *, unsigned int);
    int (*irq_set_wake)(struct irq_data *, unsigned int);
    void (*irq_bus_lock)(struct irq_data *);
    void (*irq_bus_sync_unlock)(struct irq_data *);
    void (*irq_cpu_online)(struct irq_data *);
    void (*irq_cpu_offline)(struct irq_data *);
    void (*irq_suspend)(struct irq_data *);
    void (*irq_resume)(struct irq_data *);
    void (*irq_pm_shutdown)(struct irq_data *);
    void (*irq_calc_mask)(struct irq_data *);
    void (*irq_print_chip)(struct irq_data *, struct seq_file *);
    int (*irq_request_resources)(struct irq_data *);
    void (*irq_release_resources)(struct irq_data *);
    void (*irq_compose_msi_msg)(struct irq_data *, struct msi_msg *);
    void (*irq_write_msi_msg)(struct irq_data *, struct msi_msg *);
    int (*irq_get_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool *);
    int (*irq_set_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool);
    int (*irq_set_vcpu_affinity)(struct irq_data *, void *);
    void (*ipi_send_single)(struct irq_data *, unsigned int);
    void (*ipi_send_mask)(struct irq_data *, const struct cpumask *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct irq_chip {
    struct device *parent_device;
    const char *name;
    unsigned int (*irq_startup)(struct irq_data *);
    void (*irq_shutdown)(struct irq_data *);
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_ack)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
    void (*irq_mask_ack)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_eoi)(struct irq_data *);
    int (*irq_set_affinity)(struct irq_data *, const struct cpumask *, bool);
    int (*irq_retrigger)(struct irq_data *);
    int (*irq_set_type)(struct irq_data *, unsigned int);
    int (*irq_set_wake)(struct irq_data *, unsigned int);
    void (*irq_bus_lock)(struct irq_data *);
    void (*irq_bus_sync_unlock)(struct irq_data *);
    void (*irq_cpu_online)(struct irq_data *);
    void (*irq_cpu_offline)(struct irq_data *);
    void (*irq_suspend)(struct irq_data *);
    void (*irq_resume)(struct irq_data *);
    void (*irq_pm_shutdown)(struct irq_data *);
    void (*irq_calc_mask)(struct irq_data *);
    void (*irq_print_chip)(struct irq_data *, struct seq_file *);
    int (*irq_request_resources)(struct irq_data *);
    void (*irq_release_resources)(struct irq_data *);
    void (*irq_compose_msi_msg)(struct irq_data *, struct msi_msg *);
    void (*irq_write_msi_msg)(struct irq_data *, struct msi_msg *);
    int (*irq_get_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool *);
    int (*irq_set_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool);
    int (*irq_set_vcpu_affinity)(struct irq_data *, void *);
    void (*ipi_send_single)(struct irq_data *, unsigned int);
    void (*ipi_send_mask)(struct irq_data *, const struct cpumask *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct irq_chip {
    struct device *parent_device;
    const char *name;
    unsigned int (*irq_startup)(struct irq_data *);
    void (*irq_shutdown)(struct irq_data *);
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_ack)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
    void (*irq_mask_ack)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_eoi)(struct irq_data *);
    int (*irq_set_affinity)(struct irq_data *, const struct cpumask *, bool);
    int (*irq_retrigger)(struct irq_data *);
    int (*irq_set_type)(struct irq_data *, unsigned int);
    int (*irq_set_wake)(struct irq_data *, unsigned int);
    void (*irq_bus_lock)(struct irq_data *);
    void (*irq_bus_sync_unlock)(struct irq_data *);
    void (*irq_cpu_online)(struct irq_data *);
    void (*irq_cpu_offline)(struct irq_data *);
    void (*irq_suspend)(struct irq_data *);
    void (*irq_resume)(struct irq_data *);
    void (*irq_pm_shutdown)(struct irq_data *);
    void (*irq_calc_mask)(struct irq_data *);
    void (*irq_print_chip)(struct irq_data *, struct seq_file *);
    int (*irq_request_resources)(struct irq_data *);
    void (*irq_release_resources)(struct irq_data *);
    void (*irq_compose_msi_msg)(struct irq_data *, struct msi_msg *);
    void (*irq_write_msi_msg)(struct irq_data *, struct msi_msg *);
    int (*irq_get_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool *);
    int (*irq_set_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool);
    int (*irq_set_vcpu_affinity)(struct irq_data *, void *);
    void (*ipi_send_single)(struct irq_data *, unsigned int);
    void (*ipi_send_mask)(struct irq_data *, const struct cpumask *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct irq_chip {
    struct device *parent_device;
    const char *name;
    unsigned int (*irq_startup)(struct irq_data *);
    void (*irq_shutdown)(struct irq_data *);
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_ack)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
    void (*irq_mask_ack)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_eoi)(struct irq_data *);
    int (*irq_set_affinity)(struct irq_data *, const struct cpumask *, bool);
    int (*irq_retrigger)(struct irq_data *);
    int (*irq_set_type)(struct irq_data *, unsigned int);
    int (*irq_set_wake)(struct irq_data *, unsigned int);
    void (*irq_bus_lock)(struct irq_data *);
    void (*irq_bus_sync_unlock)(struct irq_data *);
    void (*irq_cpu_online)(struct irq_data *);
    void (*irq_cpu_offline)(struct irq_data *);
    void (*irq_suspend)(struct irq_data *);
    void (*irq_resume)(struct irq_data *);
    void (*irq_pm_shutdown)(struct irq_data *);
    void (*irq_calc_mask)(struct irq_data *);
    void (*irq_print_chip)(struct irq_data *, struct seq_file *);
    int (*irq_request_resources)(struct irq_data *);
    void (*irq_release_resources)(struct irq_data *);
    void (*irq_compose_msi_msg)(struct irq_data *, struct msi_msg *);
    void (*irq_write_msi_msg)(struct irq_data *, struct msi_msg *);
    int (*irq_get_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool *);
    int (*irq_set_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool);
    int (*irq_set_vcpu_affinity)(struct irq_data *, void *);
    void (*ipi_send_single)(struct irq_data *, unsigned int);
    void (*ipi_send_mask)(struct irq_data *, const struct cpumask *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct irq_chip {
    struct device *parent_device;
    const char *name;
    unsigned int (*irq_startup)(struct irq_data *);
    void (*irq_shutdown)(struct irq_data *);
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_ack)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
    void (*irq_mask_ack)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_eoi)(struct irq_data *);
    int (*irq_set_affinity)(struct irq_data *, const struct cpumask *, bool);
    int (*irq_retrigger)(struct irq_data *);
    int (*irq_set_type)(struct irq_data *, unsigned int);
    int (*irq_set_wake)(struct irq_data *, unsigned int);
    void (*irq_bus_lock)(struct irq_data *);
    void (*irq_bus_sync_unlock)(struct irq_data *);
    void (*irq_cpu_online)(struct irq_data *);
    void (*irq_cpu_offline)(struct irq_data *);
    void (*irq_suspend)(struct irq_data *);
    void (*irq_resume)(struct irq_data *);
    void (*irq_pm_shutdown)(struct irq_data *);
    void (*irq_calc_mask)(struct irq_data *);
    void (*irq_print_chip)(struct irq_data *, struct seq_file *);
    int (*irq_request_resources)(struct irq_data *);
    void (*irq_release_resources)(struct irq_data *);
    void (*irq_compose_msi_msg)(struct irq_data *, struct msi_msg *);
    void (*irq_write_msi_msg)(struct irq_data *, struct msi_msg *);
    int (*irq_get_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool *);
    int (*irq_set_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool);
    int (*irq_set_vcpu_affinity)(struct irq_data *, void *);
    void (*ipi_send_single)(struct irq_data *, unsigned int);
    void (*ipi_send_mask)(struct irq_data *, const struct cpumask *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct irq_chip {
    struct device *parent_device;
    const char *name;
    unsigned int (*irq_startup)(struct irq_data *);
    void (*irq_shutdown)(struct irq_data *);
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_ack)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
    void (*irq_mask_ack)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_eoi)(struct irq_data *);
    int (*irq_set_affinity)(struct irq_data *, const struct cpumask *, bool);
    int (*irq_retrigger)(struct irq_data *);
    int (*irq_set_type)(struct irq_data *, unsigned int);
    int (*irq_set_wake)(struct irq_data *, unsigned int);
    void (*irq_bus_lock)(struct irq_data *);
    void (*irq_bus_sync_unlock)(struct irq_data *);
    void (*irq_cpu_online)(struct irq_data *);
    void (*irq_cpu_offline)(struct irq_data *);
    void (*irq_suspend)(struct irq_data *);
    void (*irq_resume)(struct irq_data *);
    void (*irq_pm_shutdown)(struct irq_data *);
    void (*irq_calc_mask)(struct irq_data *);
    void (*irq_print_chip)(struct irq_data *, struct seq_file *);
    int (*irq_request_resources)(struct irq_data *);
    void (*irq_release_resources)(struct irq_data *);
    void (*irq_compose_msi_msg)(struct irq_data *, struct msi_msg *);
    void (*irq_write_msi_msg)(struct irq_data *, struct msi_msg *);
    int (*irq_get_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool *);
    int (*irq_set_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool);
    int (*irq_set_vcpu_affinity)(struct irq_data *, void *);
    void (*ipi_send_single)(struct irq_data *, unsigned int);
    void (*ipi_send_mask)(struct irq_data *, const struct cpumask *);
    int (*irq_nmi_setup)(struct irq_data *);
    void (*irq_nmi_teardown)(struct irq_data *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct irq_chip {
    struct device *parent_device;
    const char *name;
    unsigned int (*irq_startup)(struct irq_data *);
    void (*irq_shutdown)(struct irq_data *);
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_ack)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
    void (*irq_mask_ack)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_eoi)(struct irq_data *);
    int (*irq_set_affinity)(struct irq_data *, const struct cpumask *, bool);
    int (*irq_retrigger)(struct irq_data *);
    int (*irq_set_type)(struct irq_data *, unsigned int);
    int (*irq_set_wake)(struct irq_data *, unsigned int);
    void (*irq_bus_lock)(struct irq_data *);
    void (*irq_bus_sync_unlock)(struct irq_data *);
    void (*irq_cpu_online)(struct irq_data *);
    void (*irq_cpu_offline)(struct irq_data *);
    void (*irq_suspend)(struct irq_data *);
    void (*irq_resume)(struct irq_data *);
    void (*irq_pm_shutdown)(struct irq_data *);
    void (*irq_calc_mask)(struct irq_data *);
    void (*irq_print_chip)(struct irq_data *, struct seq_file *);
    int (*irq_request_resources)(struct irq_data *);
    void (*irq_release_resources)(struct irq_data *);
    void (*irq_compose_msi_msg)(struct irq_data *, struct msi_msg *);
    void (*irq_write_msi_msg)(struct irq_data *, struct msi_msg *);
    int (*irq_get_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool *);
    int (*irq_set_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool);
    int (*irq_set_vcpu_affinity)(struct irq_data *, void *);
    void (*ipi_send_single)(struct irq_data *, unsigned int);
    void (*ipi_send_mask)(struct irq_data *, const struct cpumask *);
    int (*irq_nmi_setup)(struct irq_data *);
    void (*irq_nmi_teardown)(struct irq_data *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct irq_chip {
    struct device *parent_device;
    const char *name;
    unsigned int (*irq_startup)(struct irq_data *);
    void (*irq_shutdown)(struct irq_data *);
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_ack)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
    void (*irq_mask_ack)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_eoi)(struct irq_data *);
    int (*irq_set_affinity)(struct irq_data *, const struct cpumask *, bool);
    int (*irq_retrigger)(struct irq_data *);
    int (*irq_set_type)(struct irq_data *, unsigned int);
    int (*irq_set_wake)(struct irq_data *, unsigned int);
    void (*irq_bus_lock)(struct irq_data *);
    void (*irq_bus_sync_unlock)(struct irq_data *);
    void (*irq_cpu_online)(struct irq_data *);
    void (*irq_cpu_offline)(struct irq_data *);
    void (*irq_suspend)(struct irq_data *);
    void (*irq_resume)(struct irq_data *);
    void (*irq_pm_shutdown)(struct irq_data *);
    void (*irq_calc_mask)(struct irq_data *);
    void (*irq_print_chip)(struct irq_data *, struct seq_file *);
    int (*irq_request_resources)(struct irq_data *);
    void (*irq_release_resources)(struct irq_data *);
    void (*irq_compose_msi_msg)(struct irq_data *, struct msi_msg *);
    void (*irq_write_msi_msg)(struct irq_data *, struct msi_msg *);
    int (*irq_get_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool *);
    int (*irq_set_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool);
    int (*irq_set_vcpu_affinity)(struct irq_data *, void *);
    void (*ipi_send_single)(struct irq_data *, unsigned int);
    void (*ipi_send_mask)(struct irq_data *, const struct cpumask *);
    int (*irq_nmi_setup)(struct irq_data *);
    void (*irq_nmi_teardown)(struct irq_data *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct irq_chip {
    struct device *parent_device;
    const char *name;
    unsigned int (*irq_startup)(struct irq_data *);
    void (*irq_shutdown)(struct irq_data *);
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_ack)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
    void (*irq_mask_ack)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_eoi)(struct irq_data *);
    int (*irq_set_affinity)(struct irq_data *, const struct cpumask *, bool);
    int (*irq_retrigger)(struct irq_data *);
    int (*irq_set_type)(struct irq_data *, unsigned int);
    int (*irq_set_wake)(struct irq_data *, unsigned int);
    void (*irq_bus_lock)(struct irq_data *);
    void (*irq_bus_sync_unlock)(struct irq_data *);
    void (*irq_cpu_online)(struct irq_data *);
    void (*irq_cpu_offline)(struct irq_data *);
    void (*irq_suspend)(struct irq_data *);
    void (*irq_resume)(struct irq_data *);
    void (*irq_pm_shutdown)(struct irq_data *);
    void (*irq_calc_mask)(struct irq_data *);
    void (*irq_print_chip)(struct irq_data *, struct seq_file *);
    int (*irq_request_resources)(struct irq_data *);
    void (*irq_release_resources)(struct irq_data *);
    void (*irq_compose_msi_msg)(struct irq_data *, struct msi_msg *);
    void (*irq_write_msi_msg)(struct irq_data *, struct msi_msg *);
    int (*irq_get_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool *);
    int (*irq_set_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool);
    int (*irq_set_vcpu_affinity)(struct irq_data *, void *);
    void (*ipi_send_single)(struct irq_data *, unsigned int);
    void (*ipi_send_mask)(struct irq_data *, const struct cpumask *);
    int (*irq_nmi_setup)(struct irq_data *);
    void (*irq_nmi_teardown)(struct irq_data *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct irq_chip {
    struct device *parent_device;
    const char *name;
    unsigned int (*irq_startup)(struct irq_data *);
    void (*irq_shutdown)(struct irq_data *);
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_ack)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
    void (*irq_mask_ack)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_eoi)(struct irq_data *);
    int (*irq_set_affinity)(struct irq_data *, const struct cpumask *, bool);
    int (*irq_retrigger)(struct irq_data *);
    int (*irq_set_type)(struct irq_data *, unsigned int);
    int (*irq_set_wake)(struct irq_data *, unsigned int);
    void (*irq_bus_lock)(struct irq_data *);
    void (*irq_bus_sync_unlock)(struct irq_data *);
    void (*irq_cpu_online)(struct irq_data *);
    void (*irq_cpu_offline)(struct irq_data *);
    void (*irq_suspend)(struct irq_data *);
    void (*irq_resume)(struct irq_data *);
    void (*irq_pm_shutdown)(struct irq_data *);
    void (*irq_calc_mask)(struct irq_data *);
    void (*irq_print_chip)(struct irq_data *, struct seq_file *);
    int (*irq_request_resources)(struct irq_data *);
    void (*irq_release_resources)(struct irq_data *);
    void (*irq_compose_msi_msg)(struct irq_data *, struct msi_msg *);
    void (*irq_write_msi_msg)(struct irq_data *, struct msi_msg *);
    int (*irq_get_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool *);
    int (*irq_set_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool);
    int (*irq_set_vcpu_affinity)(struct irq_data *, void *);
    void (*ipi_send_single)(struct irq_data *, unsigned int);
    void (*ipi_send_mask)(struct irq_data *, const struct cpumask *);
    int (*irq_nmi_setup)(struct irq_data *);
    void (*irq_nmi_teardown)(struct irq_data *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct irq_chip {
    struct device *parent_device;
    const char *name;
    unsigned int (*irq_startup)(struct irq_data *);
    void (*irq_shutdown)(struct irq_data *);
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_ack)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
    void (*irq_mask_ack)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_eoi)(struct irq_data *);
    int (*irq_set_affinity)(struct irq_data *, const struct cpumask *, bool);
    int (*irq_retrigger)(struct irq_data *);
    int (*irq_set_type)(struct irq_data *, unsigned int);
    int (*irq_set_wake)(struct irq_data *, unsigned int);
    void (*irq_bus_lock)(struct irq_data *);
    void (*irq_bus_sync_unlock)(struct irq_data *);
    void (*irq_cpu_online)(struct irq_data *);
    void (*irq_cpu_offline)(struct irq_data *);
    void (*irq_suspend)(struct irq_data *);
    void (*irq_resume)(struct irq_data *);
    void (*irq_pm_shutdown)(struct irq_data *);
    void (*irq_calc_mask)(struct irq_data *);
    void (*irq_print_chip)(struct irq_data *, struct seq_file *);
    int (*irq_request_resources)(struct irq_data *);
    void (*irq_release_resources)(struct irq_data *);
    void (*irq_compose_msi_msg)(struct irq_data *, struct msi_msg *);
    void (*irq_write_msi_msg)(struct irq_data *, struct msi_msg *);
    int (*irq_get_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool *);
    int (*irq_set_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool);
    int (*irq_set_vcpu_affinity)(struct irq_data *, void *);
    void (*ipi_send_single)(struct irq_data *, unsigned int);
    void (*ipi_send_mask)(struct irq_data *, const struct cpumask *);
    int (*irq_nmi_setup)(struct irq_data *);
    void (*irq_nmi_teardown)(struct irq_data *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct irq_chip {
    const char *name;
    unsigned int (*irq_startup)(struct irq_data *);
    void (*irq_shutdown)(struct irq_data *);
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_ack)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
    void (*irq_mask_ack)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_eoi)(struct irq_data *);
    int (*irq_set_affinity)(struct irq_data *, const struct cpumask *, bool);
    int (*irq_retrigger)(struct irq_data *);
    int (*irq_set_type)(struct irq_data *, unsigned int);
    int (*irq_set_wake)(struct irq_data *, unsigned int);
    void (*irq_bus_lock)(struct irq_data *);
    void (*irq_bus_sync_unlock)(struct irq_data *);
    void (*irq_suspend)(struct irq_data *);
    void (*irq_resume)(struct irq_data *);
    void (*irq_pm_shutdown)(struct irq_data *);
    void (*irq_calc_mask)(struct irq_data *);
    void (*irq_print_chip)(struct irq_data *, struct seq_file *);
    int (*irq_request_resources)(struct irq_data *);
    void (*irq_release_resources)(struct irq_data *);
    void (*irq_compose_msi_msg)(struct irq_data *, struct msi_msg *);
    void (*irq_write_msi_msg)(struct irq_data *, struct msi_msg *);
    int (*irq_get_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool *);
    int (*irq_set_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool);
    int (*irq_set_vcpu_affinity)(struct irq_data *, void *);
    void (*ipi_send_single)(struct irq_data *, unsigned int);
    void (*ipi_send_mask)(struct irq_data *, const struct cpumask *);
    int (*irq_nmi_setup)(struct irq_data *);
    void (*irq_nmi_teardown)(struct irq_data *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct irq_chip {
    const char *name;
    unsigned int (*irq_startup)(struct irq_data *);
    void (*irq_shutdown)(struct irq_data *);
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_ack)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
    void (*irq_mask_ack)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_eoi)(struct irq_data *);
    int (*irq_set_affinity)(struct irq_data *, const struct cpumask *, bool);
    int (*irq_retrigger)(struct irq_data *);
    int (*irq_set_type)(struct irq_data *, unsigned int);
    int (*irq_set_wake)(struct irq_data *, unsigned int);
    void (*irq_bus_lock)(struct irq_data *);
    void (*irq_bus_sync_unlock)(struct irq_data *);
    void (*irq_suspend)(struct irq_data *);
    void (*irq_resume)(struct irq_data *);
    void (*irq_pm_shutdown)(struct irq_data *);
    void (*irq_calc_mask)(struct irq_data *);
    void (*irq_print_chip)(struct irq_data *, struct seq_file *);
    int (*irq_request_resources)(struct irq_data *);
    void (*irq_release_resources)(struct irq_data *);
    void (*irq_compose_msi_msg)(struct irq_data *, struct msi_msg *);
    void (*irq_write_msi_msg)(struct irq_data *, struct msi_msg *);
    int (*irq_get_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool *);
    int (*irq_set_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool);
    int (*irq_set_vcpu_affinity)(struct irq_data *, void *);
    void (*ipi_send_single)(struct irq_data *, unsigned int);
    void (*ipi_send_mask)(struct irq_data *, const struct cpumask *);
    int (*irq_nmi_setup)(struct irq_data *);
    void (*irq_nmi_teardown)(struct irq_data *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct irq_chip {
    const char *name;
    unsigned int (*irq_startup)(struct irq_data *);
    void (*irq_shutdown)(struct irq_data *);
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_ack)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
    void (*irq_mask_ack)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_eoi)(struct irq_data *);
    int (*irq_set_affinity)(struct irq_data *, const struct cpumask *, bool);
    int (*irq_retrigger)(struct irq_data *);
    int (*irq_set_type)(struct irq_data *, unsigned int);
    int (*irq_set_wake)(struct irq_data *, unsigned int);
    void (*irq_bus_lock)(struct irq_data *);
    void (*irq_bus_sync_unlock)(struct irq_data *);
    void (*irq_suspend)(struct irq_data *);
    void (*irq_resume)(struct irq_data *);
    void (*irq_pm_shutdown)(struct irq_data *);
    void (*irq_calc_mask)(struct irq_data *);
    void (*irq_print_chip)(struct irq_data *, struct seq_file *);
    int (*irq_request_resources)(struct irq_data *);
    void (*irq_release_resources)(struct irq_data *);
    void (*irq_compose_msi_msg)(struct irq_data *, struct msi_msg *);
    void (*irq_write_msi_msg)(struct irq_data *, struct msi_msg *);
    int (*irq_get_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool *);
    int (*irq_set_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool);
    int (*irq_set_vcpu_affinity)(struct irq_data *, void *);
    void (*ipi_send_single)(struct irq_data *, unsigned int);
    void (*ipi_send_mask)(struct irq_data *, const struct cpumask *);
    int (*irq_nmi_setup)(struct irq_data *);
    void (*irq_nmi_teardown)(struct irq_data *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct irq_chip {
    const char *name;
    unsigned int (*irq_startup)(struct irq_data *);
    void (*irq_shutdown)(struct irq_data *);
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_ack)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
    void (*irq_mask_ack)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_eoi)(struct irq_data *);
    int (*irq_set_affinity)(struct irq_data *, const struct cpumask *, bool);
    int (*irq_retrigger)(struct irq_data *);
    int (*irq_set_type)(struct irq_data *, unsigned int);
    int (*irq_set_wake)(struct irq_data *, unsigned int);
    void (*irq_bus_lock)(struct irq_data *);
    void (*irq_bus_sync_unlock)(struct irq_data *);
    void (*irq_suspend)(struct irq_data *);
    void (*irq_resume)(struct irq_data *);
    void (*irq_pm_shutdown)(struct irq_data *);
    void (*irq_calc_mask)(struct irq_data *);
    void (*irq_print_chip)(struct irq_data *, struct seq_file *);
    int (*irq_request_resources)(struct irq_data *);
    void (*irq_release_resources)(struct irq_data *);
    void (*irq_compose_msi_msg)(struct irq_data *, struct msi_msg *);
    void (*irq_write_msi_msg)(struct irq_data *, struct msi_msg *);
    int (*irq_get_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool *);
    int (*irq_set_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool);
    int (*irq_set_vcpu_affinity)(struct irq_data *, void *);
    void (*ipi_send_single)(struct irq_data *, unsigned int);
    void (*ipi_send_mask)(struct irq_data *, const struct cpumask *);
    int (*irq_nmi_setup)(struct irq_data *);
    void (*irq_nmi_teardown)(struct irq_data *);
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
struct irq_chip {
    struct device *parent_device;
    const char *name;
    unsigned int (*irq_startup)(struct irq_data *);
    void (*irq_shutdown)(struct irq_data *);
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_ack)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
    void (*irq_mask_ack)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_eoi)(struct irq_data *);
    int (*irq_set_affinity)(struct irq_data *, const struct cpumask *, bool);
    int (*irq_retrigger)(struct irq_data *);
    int (*irq_set_type)(struct irq_data *, unsigned int);
    int (*irq_set_wake)(struct irq_data *, unsigned int);
    void (*irq_bus_lock)(struct irq_data *);
    void (*irq_bus_sync_unlock)(struct irq_data *);
    void (*irq_cpu_online)(struct irq_data *);
    void (*irq_cpu_offline)(struct irq_data *);
    void (*irq_suspend)(struct irq_data *);
    void (*irq_resume)(struct irq_data *);
    void (*irq_pm_shutdown)(struct irq_data *);
    void (*irq_calc_mask)(struct irq_data *);
    void (*irq_print_chip)(struct irq_data *, struct seq_file *);
    int (*irq_request_resources)(struct irq_data *);
    void (*irq_release_resources)(struct irq_data *);
    void (*irq_compose_msi_msg)(struct irq_data *, struct msi_msg *);
    void (*irq_write_msi_msg)(struct irq_data *, struct msi_msg *);
    int (*irq_get_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool *);
    int (*irq_set_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool);
    int (*irq_set_vcpu_affinity)(struct irq_data *, void *);
    void (*ipi_send_single)(struct irq_data *, unsigned int);
    void (*ipi_send_mask)(struct irq_data *, const struct cpumask *);
    int (*irq_nmi_setup)(struct irq_data *);
    void (*irq_nmi_teardown)(struct irq_data *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct irq_chip {
    struct device *parent_device;
    const char *name;
    unsigned int (*irq_startup)(struct irq_data *);
    void (*irq_shutdown)(struct irq_data *);
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_ack)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
    void (*irq_mask_ack)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_eoi)(struct irq_data *);
    int (*irq_set_affinity)(struct irq_data *, const struct cpumask *, bool);
    int (*irq_retrigger)(struct irq_data *);
    int (*irq_set_type)(struct irq_data *, unsigned int);
    int (*irq_set_wake)(struct irq_data *, unsigned int);
    void (*irq_bus_lock)(struct irq_data *);
    void (*irq_bus_sync_unlock)(struct irq_data *);
    void (*irq_cpu_online)(struct irq_data *);
    void (*irq_cpu_offline)(struct irq_data *);
    void (*irq_suspend)(struct irq_data *);
    void (*irq_resume)(struct irq_data *);
    void (*irq_pm_shutdown)(struct irq_data *);
    void (*irq_calc_mask)(struct irq_data *);
    void (*irq_print_chip)(struct irq_data *, struct seq_file *);
    int (*irq_request_resources)(struct irq_data *);
    void (*irq_release_resources)(struct irq_data *);
    void (*irq_compose_msi_msg)(struct irq_data *, struct msi_msg *);
    void (*irq_write_msi_msg)(struct irq_data *, struct msi_msg *);
    int (*irq_get_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool *);
    int (*irq_set_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool);
    int (*irq_set_vcpu_affinity)(struct irq_data *, void *);
    void (*ipi_send_single)(struct irq_data *, unsigned int);
    void (*ipi_send_mask)(struct irq_data *, const struct cpumask *);
    int (*irq_nmi_setup)(struct irq_data *);
    void (*irq_nmi_teardown)(struct irq_data *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct irq_chip {
    struct device *parent_device;
    const char *name;
    unsigned int (*irq_startup)(struct irq_data *);
    void (*irq_shutdown)(struct irq_data *);
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_ack)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
    void (*irq_mask_ack)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_eoi)(struct irq_data *);
    int (*irq_set_affinity)(struct irq_data *, const struct cpumask *, bool);
    int (*irq_retrigger)(struct irq_data *);
    int (*irq_set_type)(struct irq_data *, unsigned int);
    int (*irq_set_wake)(struct irq_data *, unsigned int);
    void (*irq_bus_lock)(struct irq_data *);
    void (*irq_bus_sync_unlock)(struct irq_data *);
    void (*irq_cpu_online)(struct irq_data *);
    void (*irq_cpu_offline)(struct irq_data *);
    void (*irq_suspend)(struct irq_data *);
    void (*irq_resume)(struct irq_data *);
    void (*irq_pm_shutdown)(struct irq_data *);
    void (*irq_calc_mask)(struct irq_data *);
    void (*irq_print_chip)(struct irq_data *, struct seq_file *);
    int (*irq_request_resources)(struct irq_data *);
    void (*irq_release_resources)(struct irq_data *);
    void (*irq_compose_msi_msg)(struct irq_data *, struct msi_msg *);
    void (*irq_write_msi_msg)(struct irq_data *, struct msi_msg *);
    int (*irq_get_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool *);
    int (*irq_set_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool);
    int (*irq_set_vcpu_affinity)(struct irq_data *, void *);
    void (*ipi_send_single)(struct irq_data *, unsigned int);
    void (*ipi_send_mask)(struct irq_data *, const struct cpumask *);
    int (*irq_nmi_setup)(struct irq_data *);
    void (*irq_nmi_teardown)(struct irq_data *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct irq_chip {
    struct device *parent_device;
    const char *name;
    unsigned int (*irq_startup)(struct irq_data *);
    void (*irq_shutdown)(struct irq_data *);
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_ack)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
    void (*irq_mask_ack)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_eoi)(struct irq_data *);
    int (*irq_set_affinity)(struct irq_data *, const struct cpumask *, bool);
    int (*irq_retrigger)(struct irq_data *);
    int (*irq_set_type)(struct irq_data *, unsigned int);
    int (*irq_set_wake)(struct irq_data *, unsigned int);
    void (*irq_bus_lock)(struct irq_data *);
    void (*irq_bus_sync_unlock)(struct irq_data *);
    void (*irq_cpu_online)(struct irq_data *);
    void (*irq_cpu_offline)(struct irq_data *);
    void (*irq_suspend)(struct irq_data *);
    void (*irq_resume)(struct irq_data *);
    void (*irq_pm_shutdown)(struct irq_data *);
    void (*irq_calc_mask)(struct irq_data *);
    void (*irq_print_chip)(struct irq_data *, struct seq_file *);
    int (*irq_request_resources)(struct irq_data *);
    void (*irq_release_resources)(struct irq_data *);
    void (*irq_compose_msi_msg)(struct irq_data *, struct msi_msg *);
    void (*irq_write_msi_msg)(struct irq_data *, struct msi_msg *);
    int (*irq_get_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool *);
    int (*irq_set_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool);
    int (*irq_set_vcpu_affinity)(struct irq_data *, void *);
    void (*ipi_send_single)(struct irq_data *, unsigned int);
    void (*ipi_send_mask)(struct irq_data *, const struct cpumask *);
    int (*irq_nmi_setup)(struct irq_data *);
    void (*irq_nmi_teardown)(struct irq_data *);
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
struct irq_chip {
    struct device *parent_device;
    const char *name;
    unsigned int (*irq_startup)(struct irq_data *);
    void (*irq_shutdown)(struct irq_data *);
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_ack)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
    void (*irq_mask_ack)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_eoi)(struct irq_data *);
    int (*irq_set_affinity)(struct irq_data *, const struct cpumask *, bool);
    int (*irq_retrigger)(struct irq_data *);
    int (*irq_set_type)(struct irq_data *, unsigned int);
    int (*irq_set_wake)(struct irq_data *, unsigned int);
    void (*irq_bus_lock)(struct irq_data *);
    void (*irq_bus_sync_unlock)(struct irq_data *);
    void (*irq_cpu_online)(struct irq_data *);
    void (*irq_cpu_offline)(struct irq_data *);
    void (*irq_suspend)(struct irq_data *);
    void (*irq_resume)(struct irq_data *);
    void (*irq_pm_shutdown)(struct irq_data *);
    void (*irq_calc_mask)(struct irq_data *);
    void (*irq_print_chip)(struct irq_data *, struct seq_file *);
    int (*irq_request_resources)(struct irq_data *);
    void (*irq_release_resources)(struct irq_data *);
    void (*irq_compose_msi_msg)(struct irq_data *, struct msi_msg *);
    void (*irq_write_msi_msg)(struct irq_data *, struct msi_msg *);
    int (*irq_get_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool *);
    int (*irq_set_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool);
    int (*irq_set_vcpu_affinity)(struct irq_data *, void *);
    void (*ipi_send_single)(struct irq_data *, unsigned int);
    void (*ipi_send_mask)(struct irq_data *, const struct cpumask *);
    int (*irq_nmi_setup)(struct irq_data *);
    void (*irq_nmi_teardown)(struct irq_data *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct irq_chip {
    struct device *parent_device;
    const char *name;
    unsigned int (*irq_startup)(struct irq_data *);
    void (*irq_shutdown)(struct irq_data *);
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_ack)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
    void (*irq_mask_ack)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_eoi)(struct irq_data *);
    int (*irq_set_affinity)(struct irq_data *, const struct cpumask *, bool);
    int (*irq_retrigger)(struct irq_data *);
    int (*irq_set_type)(struct irq_data *, unsigned int);
    int (*irq_set_wake)(struct irq_data *, unsigned int);
    void (*irq_bus_lock)(struct irq_data *);
    void (*irq_bus_sync_unlock)(struct irq_data *);
    void (*irq_cpu_online)(struct irq_data *);
    void (*irq_cpu_offline)(struct irq_data *);
    void (*irq_suspend)(struct irq_data *);
    void (*irq_resume)(struct irq_data *);
    void (*irq_pm_shutdown)(struct irq_data *);
    void (*irq_calc_mask)(struct irq_data *);
    void (*irq_print_chip)(struct irq_data *, struct seq_file *);
    int (*irq_request_resources)(struct irq_data *);
    void (*irq_release_resources)(struct irq_data *);
    void (*irq_compose_msi_msg)(struct irq_data *, struct msi_msg *);
    void (*irq_write_msi_msg)(struct irq_data *, struct msi_msg *);
    int (*irq_get_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool *);
    int (*irq_set_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool);
    int (*irq_set_vcpu_affinity)(struct irq_data *, void *);
    void (*ipi_send_single)(struct irq_data *, unsigned int);
    void (*ipi_send_mask)(struct irq_data *, const struct cpumask *);
    int (*irq_nmi_setup)(struct irq_data *);
    void (*irq_nmi_teardown)(struct irq_data *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct irq_chip {
    struct device *parent_device;
    const char *name;
    unsigned int (*irq_startup)(struct irq_data *);
    void (*irq_shutdown)(struct irq_data *);
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_ack)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
    void (*irq_mask_ack)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_eoi)(struct irq_data *);
    int (*irq_set_affinity)(struct irq_data *, const struct cpumask *, bool);
    int (*irq_retrigger)(struct irq_data *);
    int (*irq_set_type)(struct irq_data *, unsigned int);
    int (*irq_set_wake)(struct irq_data *, unsigned int);
    void (*irq_bus_lock)(struct irq_data *);
    void (*irq_bus_sync_unlock)(struct irq_data *);
    void (*irq_cpu_online)(struct irq_data *);
    void (*irq_cpu_offline)(struct irq_data *);
    void (*irq_suspend)(struct irq_data *);
    void (*irq_resume)(struct irq_data *);
    void (*irq_pm_shutdown)(struct irq_data *);
    void (*irq_calc_mask)(struct irq_data *);
    void (*irq_print_chip)(struct irq_data *, struct seq_file *);
    int (*irq_request_resources)(struct irq_data *);
    void (*irq_release_resources)(struct irq_data *);
    void (*irq_compose_msi_msg)(struct irq_data *, struct msi_msg *);
    void (*irq_write_msi_msg)(struct irq_data *, struct msi_msg *);
    int (*irq_get_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool *);
    int (*irq_set_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool);
    int (*irq_set_vcpu_affinity)(struct irq_data *, void *);
    void (*ipi_send_single)(struct irq_data *, unsigned int);
    void (*ipi_send_mask)(struct irq_data *, const struct cpumask *);
    int (*irq_nmi_setup)(struct irq_data *);
    void (*irq_nmi_teardown)(struct irq_data *);
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct irq_chip {
    struct device *parent_device;
    const char *name;
    unsigned int (*irq_startup)(struct irq_data *);
    void (*irq_shutdown)(struct irq_data *);
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_ack)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
    void (*irq_mask_ack)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_eoi)(struct irq_data *);
    int (*irq_set_affinity)(struct irq_data *, const struct cpumask *, bool);
    int (*irq_retrigger)(struct irq_data *);
    int (*irq_set_type)(struct irq_data *, unsigned int);
    int (*irq_set_wake)(struct irq_data *, unsigned int);
    void (*irq_bus_lock)(struct irq_data *);
    void (*irq_bus_sync_unlock)(struct irq_data *);
    void (*irq_cpu_online)(struct irq_data *);
    void (*irq_cpu_offline)(struct irq_data *);
    void (*irq_suspend)(struct irq_data *);
    void (*irq_resume)(struct irq_data *);
    void (*irq_pm_shutdown)(struct irq_data *);
    void (*irq_calc_mask)(struct irq_data *);
    void (*irq_print_chip)(struct irq_data *, struct seq_file *);
    int (*irq_request_resources)(struct irq_data *);
    void (*irq_release_resources)(struct irq_data *);
    void (*irq_compose_msi_msg)(struct irq_data *, struct msi_msg *);
    void (*irq_write_msi_msg)(struct irq_data *, struct msi_msg *);
    int (*irq_get_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool *);
    int (*irq_set_irqchip_state)(struct irq_data *, enum irqchip_irq_state, bool);
    int (*irq_set_vcpu_affinity)(struct irq_data *, void *);
    void (*ipi_send_single)(struct irq_data *, unsigned int);
    void (*ipi_send_mask)(struct irq_data *, const struct cpumask *);
    int (*irq_nmi_setup)(struct irq_data *);
    void (*irq_nmi_teardown)(struct irq_data *);
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
<code>struct device *parent_device</code>
</li>
<li>
<b>Field added. </b>
<code>void (*ipi_send_single)(struct irq_data *, unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*ipi_send_mask)(struct irq_data *, const struct cpumask *)</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*irq_nmi_setup)(struct irq_data *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*irq_nmi_teardown)(struct irq_data *)</code>
</li>
</ul>
</details>
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
<b>Field removed. </b>
<code>struct device *parent_device</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*irq_cpu_online)(struct irq_data *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*irq_cpu_offline)(struct irq_data *)</code>
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
