# Struct: <code>pci_controller</code>

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
In <code>5.19</code>: Absent ⚠️
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
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
struct pci_controller {
    struct pci_bus *bus;
    char is_dynamic;
    int node;
    struct device_node *dn;
    struct list_head list_node;
    struct device *parent;
    int first_busno;
    int last_busno;
    int self_busno;
    struct resource busn;
    void *io_base_virt;
    void *io_base_alloc;
    resource_size_t io_base_phys;
    resource_size_t pci_io_size;
    resource_size_t isa_mem_phys;
    resource_size_t isa_mem_size;
    struct pci_controller_ops controller_ops;
    struct pci_ops *ops;
    unsigned int *cfg_addr;
    void *cfg_data;
    u32 indirect_type;
    struct resource io_resource;
    struct resource mem_resources[3];
    resource_size_t mem_offset[3];
    int global_number;
    resource_size_t dma_window_base_cur;
    resource_size_t dma_window_size;
    long unsigned int buid;
    struct pci_dn *pci_data;
    void *private_data;
    struct npu *npu;
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
<b>Arch</b>
<ul>
</ul>
