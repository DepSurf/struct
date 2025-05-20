# Struct: <code>irq_alloc_info</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct irq_alloc_info {
    enum irq_alloc_type type;
    u32 flags;
    const struct cpumask *mask;
    int unused;
    int hpet_id;
    int hpet_index;
    void *hpet_data;
    struct pci_dev *msi_dev;
    irq_hw_number_t msi_hwirq;
    int ioapic_id;
    int ioapic_pin;
    int ioapic_node;
    u32 ioapic_trigger;
    u32 ioapic_polarity;
    u32 ioapic_valid;
    struct IO_APIC_route_entry *ioapic_entry;
    int dmar_id;
    void *dmar_data;
    int ht_pos;
    int ht_idx;
    struct pci_dev *ht_dev;
    void *ht_update;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct irq_alloc_info {
    enum irq_alloc_type type;
    u32 flags;
    const struct cpumask *mask;
    int unused;
    int hpet_id;
    int hpet_index;
    void *hpet_data;
    struct pci_dev *msi_dev;
    irq_hw_number_t msi_hwirq;
    int ioapic_id;
    int ioapic_pin;
    int ioapic_node;
    u32 ioapic_trigger;
    u32 ioapic_polarity;
    u32 ioapic_valid;
    struct IO_APIC_route_entry *ioapic_entry;
    int dmar_id;
    void *dmar_data;
    int ht_pos;
    int ht_idx;
    struct pci_dev *ht_dev;
    void *ht_update;
    struct msi_desc *desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct irq_alloc_info {
    enum irq_alloc_type type;
    u32 flags;
    const struct cpumask *mask;
    int unused;
    int hpet_id;
    int hpet_index;
    void *hpet_data;
    struct pci_dev *msi_dev;
    irq_hw_number_t msi_hwirq;
    int ioapic_id;
    int ioapic_pin;
    int ioapic_node;
    u32 ioapic_trigger;
    u32 ioapic_polarity;
    u32 ioapic_valid;
    struct IO_APIC_route_entry *ioapic_entry;
    int dmar_id;
    void *dmar_data;
    int ht_pos;
    int ht_idx;
    struct pci_dev *ht_dev;
    void *ht_update;
    struct msi_desc *desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct irq_alloc_info {
    enum irq_alloc_type type;
    u32 flags;
    const struct cpumask *mask;
    int unused;
    int hpet_id;
    int hpet_index;
    void *hpet_data;
    struct pci_dev *msi_dev;
    irq_hw_number_t msi_hwirq;
    int ioapic_id;
    int ioapic_pin;
    int ioapic_node;
    u32 ioapic_trigger;
    u32 ioapic_polarity;
    u32 ioapic_valid;
    struct IO_APIC_route_entry *ioapic_entry;
    int dmar_id;
    void *dmar_data;
    int ht_pos;
    int ht_idx;
    struct pci_dev *ht_dev;
    void *ht_update;
    struct msi_desc *desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct irq_alloc_info {
    enum irq_alloc_type type;
    u32 flags;
    const struct cpumask *mask;
    int unused;
    int hpet_id;
    int hpet_index;
    void *hpet_data;
    struct pci_dev *msi_dev;
    irq_hw_number_t msi_hwirq;
    int ioapic_id;
    int ioapic_pin;
    int ioapic_node;
    u32 ioapic_trigger;
    u32 ioapic_polarity;
    u32 ioapic_valid;
    struct IO_APIC_route_entry *ioapic_entry;
    int dmar_id;
    void *dmar_data;
    struct msi_desc *desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct irq_alloc_info {
    enum irq_alloc_type type;
    u32 flags;
    const struct cpumask *mask;
    int unused;
    int hpet_id;
    int hpet_index;
    void *hpet_data;
    struct pci_dev *msi_dev;
    irq_hw_number_t msi_hwirq;
    int ioapic_id;
    int ioapic_pin;
    int ioapic_node;
    u32 ioapic_trigger;
    u32 ioapic_polarity;
    u32 ioapic_valid;
    struct IO_APIC_route_entry *ioapic_entry;
    int dmar_id;
    void *dmar_data;
    struct msi_desc *desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct irq_alloc_info {
    enum irq_alloc_type type;
    u32 flags;
    const struct cpumask *mask;
    int unused;
    int hpet_id;
    int hpet_index;
    void *hpet_data;
    struct pci_dev *msi_dev;
    irq_hw_number_t msi_hwirq;
    int ioapic_id;
    int ioapic_pin;
    int ioapic_node;
    u32 ioapic_trigger;
    u32 ioapic_polarity;
    u32 ioapic_valid;
    struct IO_APIC_route_entry *ioapic_entry;
    int dmar_id;
    void *dmar_data;
    struct msi_desc *desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct irq_alloc_info {
    enum irq_alloc_type type;
    u32 flags;
    const struct cpumask *mask;
    int unused;
    int hpet_id;
    int hpet_index;
    void *hpet_data;
    struct pci_dev *msi_dev;
    irq_hw_number_t msi_hwirq;
    int ioapic_id;
    int ioapic_pin;
    int ioapic_node;
    u32 ioapic_trigger;
    u32 ioapic_polarity;
    u32 ioapic_valid;
    struct IO_APIC_route_entry *ioapic_entry;
    int dmar_id;
    void *dmar_data;
    struct msi_desc *desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct irq_alloc_info {
    enum irq_alloc_type type;
    u32 flags;
    const struct cpumask *mask;
    int unused;
    int hpet_id;
    int hpet_index;
    void *hpet_data;
    struct pci_dev *msi_dev;
    irq_hw_number_t msi_hwirq;
    int ioapic_id;
    int ioapic_pin;
    int ioapic_node;
    u32 ioapic_trigger;
    u32 ioapic_polarity;
    u32 ioapic_valid;
    struct IO_APIC_route_entry *ioapic_entry;
    int dmar_id;
    void *dmar_data;
    int uv_limit;
    int uv_blade;
    long unsigned int uv_offset;
    char *uv_name;
    struct msi_desc *desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct irq_alloc_info {
    enum irq_alloc_type type;
    u32 flags;
    const struct cpumask *mask;
    int unused;
    int hpet_id;
    int hpet_index;
    void *hpet_data;
    struct pci_dev *msi_dev;
    irq_hw_number_t msi_hwirq;
    int ioapic_id;
    int ioapic_pin;
    int ioapic_node;
    u32 ioapic_trigger;
    u32 ioapic_polarity;
    u32 ioapic_valid;
    struct IO_APIC_route_entry *ioapic_entry;
    int dmar_id;
    void *dmar_data;
    int uv_limit;
    int uv_blade;
    long unsigned int uv_offset;
    char *uv_name;
    struct msi_desc *desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct irq_alloc_info {
    enum irq_alloc_type type;
    u32 flags;
    u32 devid;
    irq_hw_number_t hwirq;
    const struct cpumask *mask;
    struct msi_desc *desc;
    void *data;
    struct ioapic_alloc_info ioapic;
    struct uv_alloc_info uv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct irq_alloc_info {
    enum irq_alloc_type type;
    u32 flags;
    u32 devid;
    irq_hw_number_t hwirq;
    const struct cpumask *mask;
    struct msi_desc *desc;
    void *data;
    struct ioapic_alloc_info ioapic;
    struct uv_alloc_info uv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct irq_alloc_info {
    enum irq_alloc_type type;
    u32 flags;
    u32 devid;
    irq_hw_number_t hwirq;
    const struct cpumask *mask;
    struct msi_desc *desc;
    void *data;
    struct ioapic_alloc_info ioapic;
    struct uv_alloc_info uv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct irq_alloc_info {
    enum irq_alloc_type type;
    u32 flags;
    u32 devid;
    irq_hw_number_t hwirq;
    const struct cpumask *mask;
    struct msi_desc *desc;
    void *data;
    struct ioapic_alloc_info ioapic;
    struct uv_alloc_info uv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct irq_alloc_info {
    enum irq_alloc_type type;
    u32 flags;
    u32 devid;
    irq_hw_number_t hwirq;
    const struct cpumask *mask;
    struct msi_desc *desc;
    void *data;
    struct ioapic_alloc_info ioapic;
    struct uv_alloc_info uv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct irq_alloc_info {
    enum irq_alloc_type type;
    u32 flags;
    u32 devid;
    irq_hw_number_t hwirq;
    const struct cpumask *mask;
    struct msi_desc *desc;
    void *data;
    struct ioapic_alloc_info ioapic;
    struct uv_alloc_info uv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct irq_alloc_info {
    enum irq_alloc_type type;
    u32 flags;
    u32 devid;
    irq_hw_number_t hwirq;
    const struct cpumask *mask;
    struct msi_desc *desc;
    void *data;
    struct ioapic_alloc_info ioapic;
    struct uv_alloc_info uv;
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
struct irq_alloc_info {
    enum irq_alloc_type type;
    u32 flags;
    const struct cpumask *mask;
    int unused;
    int hpet_id;
    int hpet_index;
    void *hpet_data;
    struct pci_dev *msi_dev;
    irq_hw_number_t msi_hwirq;
    int ioapic_id;
    int ioapic_pin;
    int ioapic_node;
    u32 ioapic_trigger;
    u32 ioapic_polarity;
    u32 ioapic_valid;
    struct IO_APIC_route_entry *ioapic_entry;
    int dmar_id;
    void *dmar_data;
    struct msi_desc *desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct irq_alloc_info {
    enum irq_alloc_type type;
    u32 flags;
    const struct cpumask *mask;
    int unused;
    int hpet_id;
    int hpet_index;
    void *hpet_data;
    struct pci_dev *msi_dev;
    irq_hw_number_t msi_hwirq;
    int ioapic_id;
    int ioapic_pin;
    int ioapic_node;
    u32 ioapic_trigger;
    u32 ioapic_polarity;
    u32 ioapic_valid;
    struct IO_APIC_route_entry *ioapic_entry;
    int dmar_id;
    void *dmar_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct irq_alloc_info {
    enum irq_alloc_type type;
    u32 flags;
    const struct cpumask *mask;
    int unused;
    int hpet_id;
    int hpet_index;
    void *hpet_data;
    struct pci_dev *msi_dev;
    irq_hw_number_t msi_hwirq;
    int ioapic_id;
    int ioapic_pin;
    int ioapic_node;
    u32 ioapic_trigger;
    u32 ioapic_polarity;
    u32 ioapic_valid;
    struct IO_APIC_route_entry *ioapic_entry;
    int dmar_id;
    void *dmar_data;
    struct msi_desc *desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct irq_alloc_info {
    enum irq_alloc_type type;
    u32 flags;
    const struct cpumask *mask;
    int unused;
    int hpet_id;
    int hpet_index;
    void *hpet_data;
    struct pci_dev *msi_dev;
    irq_hw_number_t msi_hwirq;
    int ioapic_id;
    int ioapic_pin;
    int ioapic_node;
    u32 ioapic_trigger;
    u32 ioapic_polarity;
    u32 ioapic_valid;
    struct IO_APIC_route_entry *ioapic_entry;
    int dmar_id;
    void *dmar_data;
    int uv_limit;
    int uv_blade;
    long unsigned int uv_offset;
    char *uv_name;
    struct msi_desc *desc;
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
<code>struct msi_desc *desc</code>
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
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int ht_pos</code>
</li>
<li>
<b>Field removed. </b>
<code>int ht_idx</code>
</li>
<li>
<b>Field removed. </b>
<code>struct pci_dev *ht_dev</code>
</li>
<li>
<b>Field removed. </b>
<code>void *ht_update</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int uv_limit</code>
</li>
<li>
<b>Field added. </b>
<code>int uv_blade</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int uv_offset</code>
</li>
<li>
<b>Field added. </b>
<code>char *uv_name</code>
</li>
</ul>
</details>
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
<code>u32 devid</code>
</li>
<li>
<b>Field added. </b>
<code>irq_hw_number_t hwirq</code>
</li>
<li>
<b>Field added. </b>
<code>void *data</code>
</li>
<li>
<b>Field added. </b>
<code>struct ioapic_alloc_info ioapic</code>
</li>
<li>
<b>Field added. </b>
<code>struct uv_alloc_info uv</code>
</li>
<li>
<b>Field removed. </b>
<code>int unused</code>
</li>
<li>
<b>Field removed. </b>
<code>int hpet_id</code>
</li>
<li>
<b>Field removed. </b>
<code>int hpet_index</code>
</li>
<li>
<b>Field removed. </b>
<code>void *hpet_data</code>
</li>
<li>
<b>Field removed. </b>
<code>struct pci_dev *msi_dev</code>
</li>
<li>
<b>Field removed. </b>
<code>irq_hw_number_t msi_hwirq</code>
</li>
<li>
<b>Field removed. </b>
<code>int ioapic_id</code>
</li>
<li>
<b>Field removed. </b>
<code>int ioapic_pin</code>
</li>
<li>
<b>Field removed. </b>
<code>int ioapic_node</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 ioapic_trigger</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 ioapic_polarity</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 ioapic_valid</code>
</li>
<li>
<b>Field removed. </b>
<code>struct IO_APIC_route_entry *ioapic_entry</code>
</li>
<li>
<b>Field removed. </b>
<code>int dmar_id</code>
</li>
<li>
<b>Field removed. </b>
<code>void *dmar_data</code>
</li>
<li>
<b>Field removed. </b>
<code>int uv_limit</code>
</li>
<li>
<b>Field removed. </b>
<code>int uv_blade</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int uv_offset</code>
</li>
<li>
<b>Field removed. </b>
<code>char *uv_name</code>
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
<details>
<summary>Changed between <code>generic</code> and <code>aws</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int uv_limit</code>
</li>
<li>
<b>Field removed. </b>
<code>int uv_blade</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int uv_offset</code>
</li>
<li>
<b>Field removed. </b>
<code>char *uv_name</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>generic</code> and <code>azure</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int uv_limit</code>
</li>
<li>
<b>Field removed. </b>
<code>int uv_blade</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int uv_offset</code>
</li>
<li>
<b>Field removed. </b>
<code>char *uv_name</code>
</li>
<li>
<b>Field removed. </b>
<code>struct msi_desc *desc</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>generic</code> and <code>gcp</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int uv_limit</code>
</li>
<li>
<b>Field removed. </b>
<code>int uv_blade</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int uv_offset</code>
</li>
<li>
<b>Field removed. </b>
<code>char *uv_name</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
