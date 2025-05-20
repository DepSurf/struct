# Struct: <code>agp_bridge_data</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct agp_bridge_data {
    const struct agp_version *version;
    const struct agp_bridge_driver *driver;
    const struct vm_operations_struct *vm_ops;
    void *previous_size;
    void *current_size;
    void *dev_private_data;
    struct pci_dev *dev;
    u32 *gatt_table;
    u32 *gatt_table_real;
    long unsigned int scratch_page;
    struct page *scratch_page_page;
    dma_addr_t scratch_page_dma;
    long unsigned int gart_bus_addr;
    long unsigned int gatt_bus_addr;
    u32 mode;
    enum chipset_type type;
    long unsigned int *key_list;
    atomic_t current_memory_agp;
    atomic_t agp_in_use;
    int max_memory_agp;
    int aperture_size_idx;
    int capndx;
    int flags;
    char major_version;
    char minor_version;
    struct list_head list;
    u32 apbase_config;
    struct list_head mapped_list;
    spinlock_t mapped_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct agp_bridge_data {
    const struct agp_version *version;
    const struct agp_bridge_driver *driver;
    const struct vm_operations_struct *vm_ops;
    void *previous_size;
    void *current_size;
    void *dev_private_data;
    struct pci_dev *dev;
    u32 *gatt_table;
    u32 *gatt_table_real;
    long unsigned int scratch_page;
    struct page *scratch_page_page;
    dma_addr_t scratch_page_dma;
    long unsigned int gart_bus_addr;
    long unsigned int gatt_bus_addr;
    u32 mode;
    enum chipset_type type;
    long unsigned int *key_list;
    atomic_t current_memory_agp;
    atomic_t agp_in_use;
    int max_memory_agp;
    int aperture_size_idx;
    int capndx;
    int flags;
    char major_version;
    char minor_version;
    struct list_head list;
    u32 apbase_config;
    struct list_head mapped_list;
    spinlock_t mapped_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct agp_bridge_data {
    const struct agp_version *version;
    const struct agp_bridge_driver *driver;
    const struct vm_operations_struct *vm_ops;
    void *previous_size;
    void *current_size;
    void *dev_private_data;
    struct pci_dev *dev;
    u32 *gatt_table;
    u32 *gatt_table_real;
    long unsigned int scratch_page;
    struct page *scratch_page_page;
    dma_addr_t scratch_page_dma;
    long unsigned int gart_bus_addr;
    long unsigned int gatt_bus_addr;
    u32 mode;
    enum chipset_type type;
    long unsigned int *key_list;
    atomic_t current_memory_agp;
    atomic_t agp_in_use;
    int max_memory_agp;
    int aperture_size_idx;
    int capndx;
    int flags;
    char major_version;
    char minor_version;
    struct list_head list;
    u32 apbase_config;
    struct list_head mapped_list;
    spinlock_t mapped_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct agp_bridge_data {
    const struct agp_version *version;
    const struct agp_bridge_driver *driver;
    const struct vm_operations_struct *vm_ops;
    void *previous_size;
    void *current_size;
    void *dev_private_data;
    struct pci_dev *dev;
    u32 *gatt_table;
    u32 *gatt_table_real;
    long unsigned int scratch_page;
    struct page *scratch_page_page;
    dma_addr_t scratch_page_dma;
    long unsigned int gart_bus_addr;
    long unsigned int gatt_bus_addr;
    u32 mode;
    enum chipset_type type;
    long unsigned int *key_list;
    atomic_t current_memory_agp;
    atomic_t agp_in_use;
    int max_memory_agp;
    int aperture_size_idx;
    int capndx;
    int flags;
    char major_version;
    char minor_version;
    struct list_head list;
    u32 apbase_config;
    struct list_head mapped_list;
    spinlock_t mapped_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct agp_bridge_data {
    const struct agp_version *version;
    const struct agp_bridge_driver *driver;
    const struct vm_operations_struct *vm_ops;
    void *previous_size;
    void *current_size;
    void *dev_private_data;
    struct pci_dev *dev;
    u32 *gatt_table;
    u32 *gatt_table_real;
    long unsigned int scratch_page;
    struct page *scratch_page_page;
    dma_addr_t scratch_page_dma;
    long unsigned int gart_bus_addr;
    long unsigned int gatt_bus_addr;
    u32 mode;
    enum chipset_type type;
    long unsigned int *key_list;
    atomic_t current_memory_agp;
    atomic_t agp_in_use;
    int max_memory_agp;
    int aperture_size_idx;
    int capndx;
    int flags;
    char major_version;
    char minor_version;
    struct list_head list;
    u32 apbase_config;
    struct list_head mapped_list;
    spinlock_t mapped_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct agp_bridge_data {
    const struct agp_version *version;
    const struct agp_bridge_driver *driver;
    const struct vm_operations_struct *vm_ops;
    void *previous_size;
    void *current_size;
    void *dev_private_data;
    struct pci_dev *dev;
    u32 *gatt_table;
    u32 *gatt_table_real;
    long unsigned int scratch_page;
    struct page *scratch_page_page;
    dma_addr_t scratch_page_dma;
    long unsigned int gart_bus_addr;
    long unsigned int gatt_bus_addr;
    u32 mode;
    enum chipset_type type;
    long unsigned int *key_list;
    atomic_t current_memory_agp;
    atomic_t agp_in_use;
    int max_memory_agp;
    int aperture_size_idx;
    int capndx;
    int flags;
    char major_version;
    char minor_version;
    struct list_head list;
    u32 apbase_config;
    struct list_head mapped_list;
    spinlock_t mapped_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct agp_bridge_data {
    const struct agp_version *version;
    const struct agp_bridge_driver *driver;
    const struct vm_operations_struct *vm_ops;
    void *previous_size;
    void *current_size;
    void *dev_private_data;
    struct pci_dev *dev;
    u32 *gatt_table;
    u32 *gatt_table_real;
    long unsigned int scratch_page;
    struct page *scratch_page_page;
    dma_addr_t scratch_page_dma;
    long unsigned int gart_bus_addr;
    long unsigned int gatt_bus_addr;
    u32 mode;
    enum chipset_type type;
    long unsigned int *key_list;
    atomic_t current_memory_agp;
    atomic_t agp_in_use;
    int max_memory_agp;
    int aperture_size_idx;
    int capndx;
    int flags;
    char major_version;
    char minor_version;
    struct list_head list;
    u32 apbase_config;
    struct list_head mapped_list;
    spinlock_t mapped_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct agp_bridge_data {
    const struct agp_version *version;
    const struct agp_bridge_driver *driver;
    const struct vm_operations_struct *vm_ops;
    void *previous_size;
    void *current_size;
    void *dev_private_data;
    struct pci_dev *dev;
    u32 *gatt_table;
    u32 *gatt_table_real;
    long unsigned int scratch_page;
    struct page *scratch_page_page;
    dma_addr_t scratch_page_dma;
    long unsigned int gart_bus_addr;
    long unsigned int gatt_bus_addr;
    u32 mode;
    enum chipset_type type;
    long unsigned int *key_list;
    atomic_t current_memory_agp;
    atomic_t agp_in_use;
    int max_memory_agp;
    int aperture_size_idx;
    int capndx;
    int flags;
    char major_version;
    char minor_version;
    struct list_head list;
    u32 apbase_config;
    struct list_head mapped_list;
    spinlock_t mapped_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct agp_bridge_data {
    const struct agp_version *version;
    const struct agp_bridge_driver *driver;
    const struct vm_operations_struct *vm_ops;
    void *previous_size;
    void *current_size;
    void *dev_private_data;
    struct pci_dev *dev;
    u32 *gatt_table;
    u32 *gatt_table_real;
    long unsigned int scratch_page;
    struct page *scratch_page_page;
    dma_addr_t scratch_page_dma;
    long unsigned int gart_bus_addr;
    long unsigned int gatt_bus_addr;
    u32 mode;
    enum chipset_type type;
    long unsigned int *key_list;
    atomic_t current_memory_agp;
    atomic_t agp_in_use;
    int max_memory_agp;
    int aperture_size_idx;
    int capndx;
    int flags;
    char major_version;
    char minor_version;
    struct list_head list;
    u32 apbase_config;
    struct list_head mapped_list;
    spinlock_t mapped_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct agp_bridge_data {
    const struct agp_version *version;
    const struct agp_bridge_driver *driver;
    const struct vm_operations_struct *vm_ops;
    void *previous_size;
    void *current_size;
    void *dev_private_data;
    struct pci_dev *dev;
    u32 *gatt_table;
    u32 *gatt_table_real;
    long unsigned int scratch_page;
    struct page *scratch_page_page;
    dma_addr_t scratch_page_dma;
    long unsigned int gart_bus_addr;
    long unsigned int gatt_bus_addr;
    u32 mode;
    enum chipset_type type;
    long unsigned int *key_list;
    atomic_t current_memory_agp;
    atomic_t agp_in_use;
    int max_memory_agp;
    int aperture_size_idx;
    int capndx;
    int flags;
    char major_version;
    char minor_version;
    struct list_head list;
    u32 apbase_config;
    struct list_head mapped_list;
    spinlock_t mapped_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct agp_bridge_data {
    const struct agp_version *version;
    const struct agp_bridge_driver *driver;
    const struct vm_operations_struct *vm_ops;
    void *previous_size;
    void *current_size;
    void *dev_private_data;
    struct pci_dev *dev;
    u32 *gatt_table;
    u32 *gatt_table_real;
    long unsigned int scratch_page;
    struct page *scratch_page_page;
    dma_addr_t scratch_page_dma;
    long unsigned int gart_bus_addr;
    long unsigned int gatt_bus_addr;
    u32 mode;
    enum chipset_type type;
    long unsigned int *key_list;
    atomic_t current_memory_agp;
    atomic_t agp_in_use;
    int max_memory_agp;
    int aperture_size_idx;
    int capndx;
    int flags;
    char major_version;
    char minor_version;
    struct list_head list;
    u32 apbase_config;
    struct list_head mapped_list;
    spinlock_t mapped_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct agp_bridge_data {
    const struct agp_version *version;
    const struct agp_bridge_driver *driver;
    const struct vm_operations_struct *vm_ops;
    void *previous_size;
    void *current_size;
    void *dev_private_data;
    struct pci_dev *dev;
    u32 *gatt_table;
    u32 *gatt_table_real;
    long unsigned int scratch_page;
    struct page *scratch_page_page;
    dma_addr_t scratch_page_dma;
    long unsigned int gart_bus_addr;
    long unsigned int gatt_bus_addr;
    u32 mode;
    enum chipset_type type;
    long unsigned int *key_list;
    atomic_t current_memory_agp;
    atomic_t agp_in_use;
    int max_memory_agp;
    int aperture_size_idx;
    int capndx;
    int flags;
    char major_version;
    char minor_version;
    struct list_head list;
    u32 apbase_config;
    struct list_head mapped_list;
    spinlock_t mapped_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct agp_bridge_data {
    const struct agp_version *version;
    const struct agp_bridge_driver *driver;
    const struct vm_operations_struct *vm_ops;
    void *previous_size;
    void *current_size;
    void *dev_private_data;
    struct pci_dev *dev;
    u32 *gatt_table;
    u32 *gatt_table_real;
    long unsigned int scratch_page;
    struct page *scratch_page_page;
    dma_addr_t scratch_page_dma;
    long unsigned int gart_bus_addr;
    long unsigned int gatt_bus_addr;
    u32 mode;
    enum chipset_type type;
    long unsigned int *key_list;
    atomic_t current_memory_agp;
    atomic_t agp_in_use;
    int max_memory_agp;
    int aperture_size_idx;
    int capndx;
    int flags;
    char major_version;
    char minor_version;
    struct list_head list;
    u32 apbase_config;
    struct list_head mapped_list;
    spinlock_t mapped_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct agp_bridge_data {
    const struct agp_version *version;
    const struct agp_bridge_driver *driver;
    const struct vm_operations_struct *vm_ops;
    void *previous_size;
    void *current_size;
    void *dev_private_data;
    struct pci_dev *dev;
    u32 *gatt_table;
    u32 *gatt_table_real;
    long unsigned int scratch_page;
    struct page *scratch_page_page;
    dma_addr_t scratch_page_dma;
    long unsigned int gart_bus_addr;
    long unsigned int gatt_bus_addr;
    u32 mode;
    enum chipset_type type;
    long unsigned int *key_list;
    atomic_t current_memory_agp;
    atomic_t agp_in_use;
    int max_memory_agp;
    int aperture_size_idx;
    int capndx;
    int flags;
    char major_version;
    char minor_version;
    struct list_head list;
    u32 apbase_config;
    struct list_head mapped_list;
    spinlock_t mapped_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct agp_bridge_data {
    const struct agp_version *version;
    const struct agp_bridge_driver *driver;
    const struct vm_operations_struct *vm_ops;
    void *previous_size;
    void *current_size;
    void *dev_private_data;
    struct pci_dev *dev;
    u32 *gatt_table;
    u32 *gatt_table_real;
    long unsigned int scratch_page;
    struct page *scratch_page_page;
    dma_addr_t scratch_page_dma;
    long unsigned int gart_bus_addr;
    long unsigned int gatt_bus_addr;
    u32 mode;
    enum chipset_type type;
    long unsigned int *key_list;
    atomic_t current_memory_agp;
    atomic_t agp_in_use;
    int max_memory_agp;
    int aperture_size_idx;
    int capndx;
    int flags;
    char major_version;
    char minor_version;
    struct list_head list;
    u32 apbase_config;
    struct list_head mapped_list;
    spinlock_t mapped_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct agp_bridge_data {
    const struct agp_version *version;
    const struct agp_bridge_driver *driver;
    const struct vm_operations_struct *vm_ops;
    void *previous_size;
    void *current_size;
    void *dev_private_data;
    struct pci_dev *dev;
    u32 *gatt_table;
    u32 *gatt_table_real;
    long unsigned int scratch_page;
    struct page *scratch_page_page;
    dma_addr_t scratch_page_dma;
    long unsigned int gart_bus_addr;
    long unsigned int gatt_bus_addr;
    u32 mode;
    enum chipset_type type;
    long unsigned int *key_list;
    atomic_t current_memory_agp;
    atomic_t agp_in_use;
    int max_memory_agp;
    int aperture_size_idx;
    int capndx;
    int flags;
    char major_version;
    char minor_version;
    struct list_head list;
    u32 apbase_config;
    struct list_head mapped_list;
    spinlock_t mapped_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct agp_bridge_data {
    const struct agp_version *version;
    const struct agp_bridge_driver *driver;
    const struct vm_operations_struct *vm_ops;
    void *previous_size;
    void *current_size;
    void *dev_private_data;
    struct pci_dev *dev;
    u32 *gatt_table;
    u32 *gatt_table_real;
    long unsigned int scratch_page;
    struct page *scratch_page_page;
    dma_addr_t scratch_page_dma;
    long unsigned int gart_bus_addr;
    long unsigned int gatt_bus_addr;
    u32 mode;
    enum chipset_type type;
    long unsigned int *key_list;
    atomic_t current_memory_agp;
    atomic_t agp_in_use;
    int max_memory_agp;
    int aperture_size_idx;
    int capndx;
    int flags;
    char major_version;
    char minor_version;
    struct list_head list;
    u32 apbase_config;
    struct list_head mapped_list;
    spinlock_t mapped_lock;
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
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct agp_bridge_data {
    const struct agp_version *version;
    const struct agp_bridge_driver *driver;
    const struct vm_operations_struct *vm_ops;
    void *previous_size;
    void *current_size;
    void *dev_private_data;
    struct pci_dev *dev;
    u32 *gatt_table;
    u32 *gatt_table_real;
    long unsigned int scratch_page;
    struct page *scratch_page_page;
    dma_addr_t scratch_page_dma;
    long unsigned int gart_bus_addr;
    long unsigned int gatt_bus_addr;
    u32 mode;
    enum chipset_type type;
    long unsigned int *key_list;
    atomic_t current_memory_agp;
    atomic_t agp_in_use;
    int max_memory_agp;
    int aperture_size_idx;
    int capndx;
    int flags;
    char major_version;
    char minor_version;
    struct list_head list;
    u32 apbase_config;
    struct list_head mapped_list;
    spinlock_t mapped_lock;
};
```
</details>
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
struct agp_bridge_data {
    const struct agp_version *version;
    const struct agp_bridge_driver *driver;
    const struct vm_operations_struct *vm_ops;
    void *previous_size;
    void *current_size;
    void *dev_private_data;
    struct pci_dev *dev;
    u32 *gatt_table;
    u32 *gatt_table_real;
    long unsigned int scratch_page;
    struct page *scratch_page_page;
    dma_addr_t scratch_page_dma;
    long unsigned int gart_bus_addr;
    long unsigned int gatt_bus_addr;
    u32 mode;
    enum chipset_type type;
    long unsigned int *key_list;
    atomic_t current_memory_agp;
    atomic_t agp_in_use;
    int max_memory_agp;
    int aperture_size_idx;
    int capndx;
    int flags;
    char major_version;
    char minor_version;
    struct list_head list;
    u32 apbase_config;
    struct list_head mapped_list;
    spinlock_t mapped_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct agp_bridge_data {
    const struct agp_version *version;
    const struct agp_bridge_driver *driver;
    const struct vm_operations_struct *vm_ops;
    void *previous_size;
    void *current_size;
    void *dev_private_data;
    struct pci_dev *dev;
    u32 *gatt_table;
    u32 *gatt_table_real;
    long unsigned int scratch_page;
    struct page *scratch_page_page;
    dma_addr_t scratch_page_dma;
    long unsigned int gart_bus_addr;
    long unsigned int gatt_bus_addr;
    u32 mode;
    enum chipset_type type;
    long unsigned int *key_list;
    atomic_t current_memory_agp;
    atomic_t agp_in_use;
    int max_memory_agp;
    int aperture_size_idx;
    int capndx;
    int flags;
    char major_version;
    char minor_version;
    struct list_head list;
    u32 apbase_config;
    struct list_head mapped_list;
    spinlock_t mapped_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct agp_bridge_data {
    const struct agp_version *version;
    const struct agp_bridge_driver *driver;
    const struct vm_operations_struct *vm_ops;
    void *previous_size;
    void *current_size;
    void *dev_private_data;
    struct pci_dev *dev;
    u32 *gatt_table;
    u32 *gatt_table_real;
    long unsigned int scratch_page;
    struct page *scratch_page_page;
    dma_addr_t scratch_page_dma;
    long unsigned int gart_bus_addr;
    long unsigned int gatt_bus_addr;
    u32 mode;
    enum chipset_type type;
    long unsigned int *key_list;
    atomic_t current_memory_agp;
    atomic_t agp_in_use;
    int max_memory_agp;
    int aperture_size_idx;
    int capndx;
    int flags;
    char major_version;
    char minor_version;
    struct list_head list;
    u32 apbase_config;
    struct list_head mapped_list;
    spinlock_t mapped_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct agp_bridge_data {
    const struct agp_version *version;
    const struct agp_bridge_driver *driver;
    const struct vm_operations_struct *vm_ops;
    void *previous_size;
    void *current_size;
    void *dev_private_data;
    struct pci_dev *dev;
    u32 *gatt_table;
    u32 *gatt_table_real;
    long unsigned int scratch_page;
    struct page *scratch_page_page;
    dma_addr_t scratch_page_dma;
    long unsigned int gart_bus_addr;
    long unsigned int gatt_bus_addr;
    u32 mode;
    enum chipset_type type;
    long unsigned int *key_list;
    atomic_t current_memory_agp;
    atomic_t agp_in_use;
    int max_memory_agp;
    int aperture_size_idx;
    int capndx;
    int flags;
    char major_version;
    char minor_version;
    struct list_head list;
    u32 apbase_config;
    struct list_head mapped_list;
    spinlock_t mapped_lock;
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
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
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
