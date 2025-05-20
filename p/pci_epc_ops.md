# Struct: <code>pci_epc_ops</code>

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
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct pci_epc_ops {
    int (*write_header)(struct pci_epc *, struct pci_epf_header *);
    int (*set_bar)(struct pci_epc *, enum pci_barno, dma_addr_t, size_t, int);
    void (*clear_bar)(struct pci_epc *, enum pci_barno);
    int (*map_addr)(struct pci_epc *, phys_addr_t, u64, size_t);
    void (*unmap_addr)(struct pci_epc *, phys_addr_t);
    int (*set_msi)(struct pci_epc *, u8);
    int (*get_msi)(struct pci_epc *);
    int (*raise_irq)(struct pci_epc *, enum pci_epc_irq_type, u8);
    int (*start)(struct pci_epc *);
    void (*stop)(struct pci_epc *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct pci_epc_ops {
    int (*write_header)(struct pci_epc *, struct pci_epf_header *);
    int (*set_bar)(struct pci_epc *, enum pci_barno, dma_addr_t, size_t, int);
    void (*clear_bar)(struct pci_epc *, enum pci_barno);
    int (*map_addr)(struct pci_epc *, phys_addr_t, u64, size_t);
    void (*unmap_addr)(struct pci_epc *, phys_addr_t);
    int (*set_msi)(struct pci_epc *, u8);
    int (*get_msi)(struct pci_epc *);
    int (*raise_irq)(struct pci_epc *, enum pci_epc_irq_type, u8);
    int (*start)(struct pci_epc *);
    void (*stop)(struct pci_epc *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct pci_epc_ops {
    int (*write_header)(struct pci_epc *, u8, struct pci_epf_header *);
    int (*set_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    void (*clear_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    int (*map_addr)(struct pci_epc *, u8, phys_addr_t, u64, size_t);
    void (*unmap_addr)(struct pci_epc *, u8, phys_addr_t);
    int (*set_msi)(struct pci_epc *, u8, u8);
    int (*get_msi)(struct pci_epc *, u8);
    int (*raise_irq)(struct pci_epc *, u8, enum pci_epc_irq_type, u8);
    int (*start)(struct pci_epc *);
    void (*stop)(struct pci_epc *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct pci_epc_ops {
    int (*write_header)(struct pci_epc *, u8, struct pci_epf_header *);
    int (*set_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    void (*clear_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    int (*map_addr)(struct pci_epc *, u8, phys_addr_t, u64, size_t);
    void (*unmap_addr)(struct pci_epc *, u8, phys_addr_t);
    int (*set_msi)(struct pci_epc *, u8, u8);
    int (*get_msi)(struct pci_epc *, u8);
    int (*set_msix)(struct pci_epc *, u8, u16);
    int (*get_msix)(struct pci_epc *, u8);
    int (*raise_irq)(struct pci_epc *, u8, enum pci_epc_irq_type, u16);
    int (*start)(struct pci_epc *);
    void (*stop)(struct pci_epc *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct pci_epc_ops {
    int (*write_header)(struct pci_epc *, u8, struct pci_epf_header *);
    int (*set_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    void (*clear_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    int (*map_addr)(struct pci_epc *, u8, phys_addr_t, u64, size_t);
    void (*unmap_addr)(struct pci_epc *, u8, phys_addr_t);
    int (*set_msi)(struct pci_epc *, u8, u8);
    int (*get_msi)(struct pci_epc *, u8);
    int (*set_msix)(struct pci_epc *, u8, u16);
    int (*get_msix)(struct pci_epc *, u8);
    int (*raise_irq)(struct pci_epc *, u8, enum pci_epc_irq_type, u16);
    int (*start)(struct pci_epc *);
    void (*stop)(struct pci_epc *);
    const struct pci_epc_features * (*get_features)(struct pci_epc *, u8);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct pci_epc_ops {
    int (*write_header)(struct pci_epc *, u8, struct pci_epf_header *);
    int (*set_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    void (*clear_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    int (*map_addr)(struct pci_epc *, u8, phys_addr_t, u64, size_t);
    void (*unmap_addr)(struct pci_epc *, u8, phys_addr_t);
    int (*set_msi)(struct pci_epc *, u8, u8);
    int (*get_msi)(struct pci_epc *, u8);
    int (*set_msix)(struct pci_epc *, u8, u16);
    int (*get_msix)(struct pci_epc *, u8);
    int (*raise_irq)(struct pci_epc *, u8, enum pci_epc_irq_type, u16);
    int (*start)(struct pci_epc *);
    void (*stop)(struct pci_epc *);
    const struct pci_epc_features * (*get_features)(struct pci_epc *, u8);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct pci_epc_ops {
    int (*write_header)(struct pci_epc *, u8, struct pci_epf_header *);
    int (*set_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    void (*clear_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    int (*map_addr)(struct pci_epc *, u8, phys_addr_t, u64, size_t);
    void (*unmap_addr)(struct pci_epc *, u8, phys_addr_t);
    int (*set_msi)(struct pci_epc *, u8, u8);
    int (*get_msi)(struct pci_epc *, u8);
    int (*set_msix)(struct pci_epc *, u8, u16, enum pci_barno, u32);
    int (*get_msix)(struct pci_epc *, u8);
    int (*raise_irq)(struct pci_epc *, u8, enum pci_epc_irq_type, u16);
    int (*start)(struct pci_epc *);
    void (*stop)(struct pci_epc *);
    const struct pci_epc_features * (*get_features)(struct pci_epc *, u8);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct pci_epc_ops {
    int (*write_header)(struct pci_epc *, u8, struct pci_epf_header *);
    int (*set_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    void (*clear_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    int (*map_addr)(struct pci_epc *, u8, phys_addr_t, u64, size_t);
    void (*unmap_addr)(struct pci_epc *, u8, phys_addr_t);
    int (*set_msi)(struct pci_epc *, u8, u8);
    int (*get_msi)(struct pci_epc *, u8);
    int (*set_msix)(struct pci_epc *, u8, u16, enum pci_barno, u32);
    int (*get_msix)(struct pci_epc *, u8);
    int (*raise_irq)(struct pci_epc *, u8, enum pci_epc_irq_type, u16);
    int (*start)(struct pci_epc *);
    void (*stop)(struct pci_epc *);
    const struct pci_epc_features * (*get_features)(struct pci_epc *, u8);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct pci_epc_ops {
    int (*write_header)(struct pci_epc *, u8, struct pci_epf_header *);
    int (*set_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    void (*clear_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    int (*map_addr)(struct pci_epc *, u8, phys_addr_t, u64, size_t);
    void (*unmap_addr)(struct pci_epc *, u8, phys_addr_t);
    int (*set_msi)(struct pci_epc *, u8, u8);
    int (*get_msi)(struct pci_epc *, u8);
    int (*set_msix)(struct pci_epc *, u8, u16, enum pci_barno, u32);
    int (*get_msix)(struct pci_epc *, u8);
    int (*raise_irq)(struct pci_epc *, u8, enum pci_epc_irq_type, u16);
    int (*map_msi_irq)(struct pci_epc *, u8, phys_addr_t, u8, u32, u32 *, u32 *);
    int (*start)(struct pci_epc *);
    void (*stop)(struct pci_epc *);
    const struct pci_epc_features * (*get_features)(struct pci_epc *, u8);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct pci_epc_ops {
    int (*write_header)(struct pci_epc *, u8, u8, struct pci_epf_header *);
    int (*set_bar)(struct pci_epc *, u8, u8, struct pci_epf_bar *);
    void (*clear_bar)(struct pci_epc *, u8, u8, struct pci_epf_bar *);
    int (*map_addr)(struct pci_epc *, u8, u8, phys_addr_t, u64, size_t);
    void (*unmap_addr)(struct pci_epc *, u8, u8, phys_addr_t);
    int (*set_msi)(struct pci_epc *, u8, u8, u8);
    int (*get_msi)(struct pci_epc *, u8, u8);
    int (*set_msix)(struct pci_epc *, u8, u8, u16, enum pci_barno, u32);
    int (*get_msix)(struct pci_epc *, u8, u8);
    int (*raise_irq)(struct pci_epc *, u8, u8, enum pci_epc_irq_type, u16);
    int (*map_msi_irq)(struct pci_epc *, u8, u8, phys_addr_t, u8, u32, u32 *, u32 *);
    int (*start)(struct pci_epc *);
    void (*stop)(struct pci_epc *);
    const struct pci_epc_features * (*get_features)(struct pci_epc *, u8, u8);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct pci_epc_ops {
    int (*write_header)(struct pci_epc *, u8, u8, struct pci_epf_header *);
    int (*set_bar)(struct pci_epc *, u8, u8, struct pci_epf_bar *);
    void (*clear_bar)(struct pci_epc *, u8, u8, struct pci_epf_bar *);
    int (*map_addr)(struct pci_epc *, u8, u8, phys_addr_t, u64, size_t);
    void (*unmap_addr)(struct pci_epc *, u8, u8, phys_addr_t);
    int (*set_msi)(struct pci_epc *, u8, u8, u8);
    int (*get_msi)(struct pci_epc *, u8, u8);
    int (*set_msix)(struct pci_epc *, u8, u8, u16, enum pci_barno, u32);
    int (*get_msix)(struct pci_epc *, u8, u8);
    int (*raise_irq)(struct pci_epc *, u8, u8, enum pci_epc_irq_type, u16);
    int (*map_msi_irq)(struct pci_epc *, u8, u8, phys_addr_t, u8, u32, u32 *, u32 *);
    int (*start)(struct pci_epc *);
    void (*stop)(struct pci_epc *);
    const struct pci_epc_features * (*get_features)(struct pci_epc *, u8, u8);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct pci_epc_ops {
    int (*write_header)(struct pci_epc *, u8, u8, struct pci_epf_header *);
    int (*set_bar)(struct pci_epc *, u8, u8, struct pci_epf_bar *);
    void (*clear_bar)(struct pci_epc *, u8, u8, struct pci_epf_bar *);
    int (*map_addr)(struct pci_epc *, u8, u8, phys_addr_t, u64, size_t);
    void (*unmap_addr)(struct pci_epc *, u8, u8, phys_addr_t);
    int (*set_msi)(struct pci_epc *, u8, u8, u8);
    int (*get_msi)(struct pci_epc *, u8, u8);
    int (*set_msix)(struct pci_epc *, u8, u8, u16, enum pci_barno, u32);
    int (*get_msix)(struct pci_epc *, u8, u8);
    int (*raise_irq)(struct pci_epc *, u8, u8, enum pci_epc_irq_type, u16);
    int (*map_msi_irq)(struct pci_epc *, u8, u8, phys_addr_t, u8, u32, u32 *, u32 *);
    int (*start)(struct pci_epc *);
    void (*stop)(struct pci_epc *);
    const struct pci_epc_features * (*get_features)(struct pci_epc *, u8, u8);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct pci_epc_ops {
    int (*write_header)(struct pci_epc *, u8, u8, struct pci_epf_header *);
    int (*set_bar)(struct pci_epc *, u8, u8, struct pci_epf_bar *);
    void (*clear_bar)(struct pci_epc *, u8, u8, struct pci_epf_bar *);
    int (*map_addr)(struct pci_epc *, u8, u8, phys_addr_t, u64, size_t);
    void (*unmap_addr)(struct pci_epc *, u8, u8, phys_addr_t);
    int (*set_msi)(struct pci_epc *, u8, u8, u8);
    int (*get_msi)(struct pci_epc *, u8, u8);
    int (*set_msix)(struct pci_epc *, u8, u8, u16, enum pci_barno, u32);
    int (*get_msix)(struct pci_epc *, u8, u8);
    int (*raise_irq)(struct pci_epc *, u8, u8, enum pci_epc_irq_type, u16);
    int (*map_msi_irq)(struct pci_epc *, u8, u8, phys_addr_t, u8, u32, u32 *, u32 *);
    int (*start)(struct pci_epc *);
    void (*stop)(struct pci_epc *);
    const struct pci_epc_features * (*get_features)(struct pci_epc *, u8, u8);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct pci_epc_ops {
    int (*write_header)(struct pci_epc *, u8, u8, struct pci_epf_header *);
    int (*set_bar)(struct pci_epc *, u8, u8, struct pci_epf_bar *);
    void (*clear_bar)(struct pci_epc *, u8, u8, struct pci_epf_bar *);
    int (*map_addr)(struct pci_epc *, u8, u8, phys_addr_t, u64, size_t);
    void (*unmap_addr)(struct pci_epc *, u8, u8, phys_addr_t);
    int (*set_msi)(struct pci_epc *, u8, u8, u8);
    int (*get_msi)(struct pci_epc *, u8, u8);
    int (*set_msix)(struct pci_epc *, u8, u8, u16, enum pci_barno, u32);
    int (*get_msix)(struct pci_epc *, u8, u8);
    int (*raise_irq)(struct pci_epc *, u8, u8, unsigned int, u16);
    int (*map_msi_irq)(struct pci_epc *, u8, u8, phys_addr_t, u8, u32, u32 *, u32 *);
    int (*start)(struct pci_epc *);
    void (*stop)(struct pci_epc *);
    const struct pci_epc_features * (*get_features)(struct pci_epc *, u8, u8);
    struct module *owner;
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
struct pci_epc_ops {
    int (*write_header)(struct pci_epc *, u8, struct pci_epf_header *);
    int (*set_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    void (*clear_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    int (*map_addr)(struct pci_epc *, u8, phys_addr_t, u64, size_t);
    void (*unmap_addr)(struct pci_epc *, u8, phys_addr_t);
    int (*set_msi)(struct pci_epc *, u8, u8);
    int (*get_msi)(struct pci_epc *, u8);
    int (*set_msix)(struct pci_epc *, u8, u16);
    int (*get_msix)(struct pci_epc *, u8);
    int (*raise_irq)(struct pci_epc *, u8, enum pci_epc_irq_type, u16);
    int (*start)(struct pci_epc *);
    void (*stop)(struct pci_epc *);
    const struct pci_epc_features * (*get_features)(struct pci_epc *, u8);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct pci_epc_ops {
    int (*write_header)(struct pci_epc *, u8, struct pci_epf_header *);
    int (*set_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    void (*clear_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    int (*map_addr)(struct pci_epc *, u8, phys_addr_t, u64, size_t);
    void (*unmap_addr)(struct pci_epc *, u8, phys_addr_t);
    int (*set_msi)(struct pci_epc *, u8, u8);
    int (*get_msi)(struct pci_epc *, u8);
    int (*set_msix)(struct pci_epc *, u8, u16);
    int (*get_msix)(struct pci_epc *, u8);
    int (*raise_irq)(struct pci_epc *, u8, enum pci_epc_irq_type, u16);
    int (*start)(struct pci_epc *);
    void (*stop)(struct pci_epc *);
    const struct pci_epc_features * (*get_features)(struct pci_epc *, u8);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct pci_epc_ops {
    int (*write_header)(struct pci_epc *, u8, struct pci_epf_header *);
    int (*set_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    void (*clear_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    int (*map_addr)(struct pci_epc *, u8, phys_addr_t, u64, size_t);
    void (*unmap_addr)(struct pci_epc *, u8, phys_addr_t);
    int (*set_msi)(struct pci_epc *, u8, u8);
    int (*get_msi)(struct pci_epc *, u8);
    int (*set_msix)(struct pci_epc *, u8, u16);
    int (*get_msix)(struct pci_epc *, u8);
    int (*raise_irq)(struct pci_epc *, u8, enum pci_epc_irq_type, u16);
    int (*start)(struct pci_epc *);
    void (*stop)(struct pci_epc *);
    const struct pci_epc_features * (*get_features)(struct pci_epc *, u8);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct pci_epc_ops {
    int (*write_header)(struct pci_epc *, u8, struct pci_epf_header *);
    int (*set_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    void (*clear_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    int (*map_addr)(struct pci_epc *, u8, phys_addr_t, u64, size_t);
    void (*unmap_addr)(struct pci_epc *, u8, phys_addr_t);
    int (*set_msi)(struct pci_epc *, u8, u8);
    int (*get_msi)(struct pci_epc *, u8);
    int (*set_msix)(struct pci_epc *, u8, u16);
    int (*get_msix)(struct pci_epc *, u8);
    int (*raise_irq)(struct pci_epc *, u8, enum pci_epc_irq_type, u16);
    int (*start)(struct pci_epc *);
    void (*stop)(struct pci_epc *);
    const struct pci_epc_features * (*get_features)(struct pci_epc *, u8);
    struct module *owner;
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
struct pci_epc_ops {
    int (*write_header)(struct pci_epc *, u8, struct pci_epf_header *);
    int (*set_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    void (*clear_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    int (*map_addr)(struct pci_epc *, u8, phys_addr_t, u64, size_t);
    void (*unmap_addr)(struct pci_epc *, u8, phys_addr_t);
    int (*set_msi)(struct pci_epc *, u8, u8);
    int (*get_msi)(struct pci_epc *, u8);
    int (*set_msix)(struct pci_epc *, u8, u16);
    int (*get_msix)(struct pci_epc *, u8);
    int (*raise_irq)(struct pci_epc *, u8, enum pci_epc_irq_type, u16);
    int (*start)(struct pci_epc *);
    void (*stop)(struct pci_epc *);
    const struct pci_epc_features * (*get_features)(struct pci_epc *, u8);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct pci_epc_ops {
    int (*write_header)(struct pci_epc *, u8, struct pci_epf_header *);
    int (*set_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    void (*clear_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    int (*map_addr)(struct pci_epc *, u8, phys_addr_t, u64, size_t);
    void (*unmap_addr)(struct pci_epc *, u8, phys_addr_t);
    int (*set_msi)(struct pci_epc *, u8, u8);
    int (*get_msi)(struct pci_epc *, u8);
    int (*set_msix)(struct pci_epc *, u8, u16);
    int (*get_msix)(struct pci_epc *, u8);
    int (*raise_irq)(struct pci_epc *, u8, enum pci_epc_irq_type, u16);
    int (*start)(struct pci_epc *);
    void (*stop)(struct pci_epc *);
    const struct pci_epc_features * (*get_features)(struct pci_epc *, u8);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct pci_epc_ops {
    int (*write_header)(struct pci_epc *, u8, struct pci_epf_header *);
    int (*set_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    void (*clear_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    int (*map_addr)(struct pci_epc *, u8, phys_addr_t, u64, size_t);
    void (*unmap_addr)(struct pci_epc *, u8, phys_addr_t);
    int (*set_msi)(struct pci_epc *, u8, u8);
    int (*get_msi)(struct pci_epc *, u8);
    int (*set_msix)(struct pci_epc *, u8, u16);
    int (*get_msix)(struct pci_epc *, u8);
    int (*raise_irq)(struct pci_epc *, u8, enum pci_epc_irq_type, u16);
    int (*start)(struct pci_epc *);
    void (*stop)(struct pci_epc *);
    const struct pci_epc_features * (*get_features)(struct pci_epc *, u8);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct pci_epc_ops {
    int (*write_header)(struct pci_epc *, u8, struct pci_epf_header *);
    int (*set_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    void (*clear_bar)(struct pci_epc *, u8, struct pci_epf_bar *);
    int (*map_addr)(struct pci_epc *, u8, phys_addr_t, u64, size_t);
    void (*unmap_addr)(struct pci_epc *, u8, phys_addr_t);
    int (*set_msi)(struct pci_epc *, u8, u8);
    int (*get_msi)(struct pci_epc *, u8);
    int (*set_msix)(struct pci_epc *, u8, u16);
    int (*get_msix)(struct pci_epc *, u8);
    int (*raise_irq)(struct pci_epc *, u8, enum pci_epc_irq_type, u16);
    int (*start)(struct pci_epc *);
    void (*stop)(struct pci_epc *);
    const struct pci_epc_features * (*get_features)(struct pci_epc *, u8);
    struct module *owner;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*write_header)(struct pci_epc *, struct pci_epf_header *)</code> ➡️ <code>int (*write_header)(struct pci_epc *, u8, struct pci_epf_header *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*set_bar)(struct pci_epc *, enum pci_barno, dma_addr_t, size_t, int)</code> ➡️ <code>int (*set_bar)(struct pci_epc *, u8, struct pci_epf_bar *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*clear_bar)(struct pci_epc *, enum pci_barno)</code> ➡️ <code>void (*clear_bar)(struct pci_epc *, u8, struct pci_epf_bar *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*map_addr)(struct pci_epc *, phys_addr_t, u64, size_t)</code> ➡️ <code>int (*map_addr)(struct pci_epc *, u8, phys_addr_t, u64, size_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*unmap_addr)(struct pci_epc *, phys_addr_t)</code> ➡️ <code>void (*unmap_addr)(struct pci_epc *, u8, phys_addr_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*set_msi)(struct pci_epc *, u8)</code> ➡️ <code>int (*set_msi)(struct pci_epc *, u8, u8)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*get_msi)(struct pci_epc *)</code> ➡️ <code>int (*get_msi)(struct pci_epc *, u8)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*raise_irq)(struct pci_epc *, enum pci_epc_irq_type, u8)</code> ➡️ <code>int (*raise_irq)(struct pci_epc *, u8, enum pci_epc_irq_type, u8)</code>
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
<code>int (*set_msix)(struct pci_epc *, u8, u16)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*get_msix)(struct pci_epc *, u8)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*raise_irq)(struct pci_epc *, u8, enum pci_epc_irq_type, u8)</code> ➡️ <code>int (*raise_irq)(struct pci_epc *, u8, enum pci_epc_irq_type, u16)</code>
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
<code>const struct pci_epc_features * (*get_features)(struct pci_epc *, u8)</code>
</li>
</ul>
</details>
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
<code>int (*set_msix)(struct pci_epc *, u8, u16)</code> ➡️ <code>int (*set_msix)(struct pci_epc *, u8, u16, enum pci_barno, u32)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*map_msi_irq)(struct pci_epc *, u8, phys_addr_t, u8, u32, u32 *, u32 *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*write_header)(struct pci_epc *, u8, struct pci_epf_header *)</code> ➡️ <code>int (*write_header)(struct pci_epc *, u8, u8, struct pci_epf_header *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*set_bar)(struct pci_epc *, u8, struct pci_epf_bar *)</code> ➡️ <code>int (*set_bar)(struct pci_epc *, u8, u8, struct pci_epf_bar *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*clear_bar)(struct pci_epc *, u8, struct pci_epf_bar *)</code> ➡️ <code>void (*clear_bar)(struct pci_epc *, u8, u8, struct pci_epf_bar *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*map_addr)(struct pci_epc *, u8, phys_addr_t, u64, size_t)</code> ➡️ <code>int (*map_addr)(struct pci_epc *, u8, u8, phys_addr_t, u64, size_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*unmap_addr)(struct pci_epc *, u8, phys_addr_t)</code> ➡️ <code>void (*unmap_addr)(struct pci_epc *, u8, u8, phys_addr_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*set_msi)(struct pci_epc *, u8, u8)</code> ➡️ <code>int (*set_msi)(struct pci_epc *, u8, u8, u8)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*get_msi)(struct pci_epc *, u8)</code> ➡️ <code>int (*get_msi)(struct pci_epc *, u8, u8)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*set_msix)(struct pci_epc *, u8, u16, enum pci_barno, u32)</code> ➡️ <code>int (*set_msix)(struct pci_epc *, u8, u8, u16, enum pci_barno, u32)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*get_msix)(struct pci_epc *, u8)</code> ➡️ <code>int (*get_msix)(struct pci_epc *, u8, u8)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*raise_irq)(struct pci_epc *, u8, enum pci_epc_irq_type, u16)</code> ➡️ <code>int (*raise_irq)(struct pci_epc *, u8, u8, enum pci_epc_irq_type, u16)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*map_msi_irq)(struct pci_epc *, u8, phys_addr_t, u8, u32, u32 *, u32 *)</code> ➡️ <code>int (*map_msi_irq)(struct pci_epc *, u8, u8, phys_addr_t, u8, u32, u32 *, u32 *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>const struct pci_epc_features * (*get_features)(struct pci_epc *, u8)</code> ➡️ <code>const struct pci_epc_features * (*get_features)(struct pci_epc *, u8, u8)</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*raise_irq)(struct pci_epc *, u8, u8, enum pci_epc_irq_type, u16)</code> ➡️ <code>int (*raise_irq)(struct pci_epc *, u8, u8, unsigned int, u16)</code>
</li>
</ul>
</details>
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
