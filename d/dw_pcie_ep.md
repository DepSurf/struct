# Struct: <code>dw_pcie_ep</code>

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
struct dw_pcie_ep {
    struct pci_epc *epc;
    struct dw_pcie_ep_ops *ops;
    phys_addr_t phys_base;
    size_t addr_size;
    u8 bar_to_atu[6];
    phys_addr_t *outbound_addr;
    long unsigned int ib_window_map;
    long unsigned int ob_window_map;
    u32 num_ib_windows;
    u32 num_ob_windows;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dw_pcie_ep {
    struct pci_epc *epc;
    struct dw_pcie_ep_ops *ops;
    phys_addr_t phys_base;
    size_t addr_size;
    size_t page_size;
    u8 bar_to_atu[6];
    phys_addr_t *outbound_addr;
    long unsigned int ib_window_map;
    long unsigned int ob_window_map;
    u32 num_ib_windows;
    u32 num_ob_windows;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dw_pcie_ep {
    struct pci_epc *epc;
    struct dw_pcie_ep_ops *ops;
    phys_addr_t phys_base;
    size_t addr_size;
    size_t page_size;
    u8 bar_to_atu[6];
    phys_addr_t *outbound_addr;
    long unsigned int *ib_window_map;
    long unsigned int *ob_window_map;
    u32 num_ib_windows;
    u32 num_ob_windows;
    void *msi_mem;
    phys_addr_t msi_mem_phys;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dw_pcie_ep {
    struct pci_epc *epc;
    struct dw_pcie_ep_ops *ops;
    phys_addr_t phys_base;
    size_t addr_size;
    size_t page_size;
    u8 bar_to_atu[6];
    phys_addr_t *outbound_addr;
    long unsigned int *ib_window_map;
    long unsigned int *ob_window_map;
    u32 num_ib_windows;
    u32 num_ob_windows;
    void *msi_mem;
    phys_addr_t msi_mem_phys;
    u8 msi_cap;
    u8 msix_cap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dw_pcie_ep {
    struct pci_epc *epc;
    const struct dw_pcie_ep_ops *ops;
    phys_addr_t phys_base;
    size_t addr_size;
    size_t page_size;
    u8 bar_to_atu[6];
    phys_addr_t *outbound_addr;
    long unsigned int *ib_window_map;
    long unsigned int *ob_window_map;
    u32 num_ib_windows;
    u32 num_ob_windows;
    void *msi_mem;
    phys_addr_t msi_mem_phys;
    u8 msi_cap;
    u8 msix_cap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dw_pcie_ep {
    struct pci_epc *epc;
    const struct dw_pcie_ep_ops *ops;
    phys_addr_t phys_base;
    size_t addr_size;
    size_t page_size;
    u8 bar_to_atu[6];
    phys_addr_t *outbound_addr;
    long unsigned int *ib_window_map;
    long unsigned int *ob_window_map;
    u32 num_ib_windows;
    u32 num_ob_windows;
    void *msi_mem;
    phys_addr_t msi_mem_phys;
    u8 msi_cap;
    u8 msix_cap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dw_pcie_ep {
    struct pci_epc *epc;
    const struct dw_pcie_ep_ops *ops;
    phys_addr_t phys_base;
    size_t addr_size;
    size_t page_size;
    u8 bar_to_atu[6];
    phys_addr_t *outbound_addr;
    long unsigned int *ib_window_map;
    long unsigned int *ob_window_map;
    u32 num_ib_windows;
    u32 num_ob_windows;
    void *msi_mem;
    phys_addr_t msi_mem_phys;
    u8 msi_cap;
    u8 msix_cap;
    struct pci_epf_bar * epf_bar[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dw_pcie_ep {
    struct pci_epc *epc;
    struct list_head func_list;
    const struct dw_pcie_ep_ops *ops;
    phys_addr_t phys_base;
    size_t addr_size;
    size_t page_size;
    u8 bar_to_atu[6];
    phys_addr_t *outbound_addr;
    long unsigned int *ib_window_map;
    long unsigned int *ob_window_map;
    void *msi_mem;
    phys_addr_t msi_mem_phys;
    struct pci_epf_bar * epf_bar[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dw_pcie_ep {
    struct pci_epc *epc;
    struct list_head func_list;
    const struct dw_pcie_ep_ops *ops;
    phys_addr_t phys_base;
    size_t addr_size;
    size_t page_size;
    u8 bar_to_atu[6];
    phys_addr_t *outbound_addr;
    long unsigned int *ib_window_map;
    long unsigned int *ob_window_map;
    void *msi_mem;
    phys_addr_t msi_mem_phys;
    struct pci_epf_bar * epf_bar[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dw_pcie_ep {
    struct pci_epc *epc;
    struct list_head func_list;
    const struct dw_pcie_ep_ops *ops;
    phys_addr_t phys_base;
    size_t addr_size;
    size_t page_size;
    u8 bar_to_atu[6];
    phys_addr_t *outbound_addr;
    long unsigned int *ib_window_map;
    long unsigned int *ob_window_map;
    void *msi_mem;
    phys_addr_t msi_mem_phys;
    struct pci_epf_bar * epf_bar[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dw_pcie_ep {
    struct pci_epc *epc;
    struct list_head func_list;
    const struct dw_pcie_ep_ops *ops;
    phys_addr_t phys_base;
    size_t addr_size;
    size_t page_size;
    u8 bar_to_atu[6];
    phys_addr_t *outbound_addr;
    long unsigned int *ib_window_map;
    long unsigned int *ob_window_map;
    void *msi_mem;
    phys_addr_t msi_mem_phys;
    struct pci_epf_bar * epf_bar[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dw_pcie_ep {
    struct pci_epc *epc;
    struct list_head func_list;
    const struct dw_pcie_ep_ops *ops;
    phys_addr_t phys_base;
    size_t addr_size;
    size_t page_size;
    u8 bar_to_atu[6];
    phys_addr_t *outbound_addr;
    long unsigned int *ib_window_map;
    long unsigned int *ob_window_map;
    void *msi_mem;
    phys_addr_t msi_mem_phys;
    struct pci_epf_bar * epf_bar[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dw_pcie_ep {
    struct pci_epc *epc;
    struct list_head func_list;
    const struct dw_pcie_ep_ops *ops;
    phys_addr_t phys_base;
    size_t addr_size;
    size_t page_size;
    u8 bar_to_atu[6];
    phys_addr_t *outbound_addr;
    long unsigned int *ib_window_map;
    long unsigned int *ob_window_map;
    void *msi_mem;
    phys_addr_t msi_mem_phys;
    struct pci_epf_bar * epf_bar[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dw_pcie_ep {
    struct pci_epc *epc;
    struct list_head func_list;
    const struct dw_pcie_ep_ops *ops;
    phys_addr_t phys_base;
    size_t addr_size;
    size_t page_size;
    u8 bar_to_atu[6];
    phys_addr_t *outbound_addr;
    long unsigned int *ib_window_map;
    long unsigned int *ob_window_map;
    void *msi_mem;
    phys_addr_t msi_mem_phys;
    struct pci_epf_bar * epf_bar[6];
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
struct dw_pcie_ep {
    struct pci_epc *epc;
    const struct dw_pcie_ep_ops *ops;
    phys_addr_t phys_base;
    size_t addr_size;
    size_t page_size;
    u8 bar_to_atu[6];
    phys_addr_t *outbound_addr;
    long unsigned int *ib_window_map;
    long unsigned int *ob_window_map;
    u32 num_ib_windows;
    u32 num_ob_windows;
    void *msi_mem;
    phys_addr_t msi_mem_phys;
    u8 msi_cap;
    u8 msix_cap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dw_pcie_ep {
    struct pci_epc *epc;
    const struct dw_pcie_ep_ops *ops;
    phys_addr_t phys_base;
    size_t addr_size;
    size_t page_size;
    u8 bar_to_atu[6];
    phys_addr_t *outbound_addr;
    long unsigned int *ib_window_map;
    long unsigned int *ob_window_map;
    u32 num_ib_windows;
    u32 num_ob_windows;
    void *msi_mem;
    phys_addr_t msi_mem_phys;
    u8 msi_cap;
    u8 msix_cap;
};
```
</details>
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dw_pcie_ep {
    struct pci_epc *epc;
    const struct dw_pcie_ep_ops *ops;
    phys_addr_t phys_base;
    size_t addr_size;
    size_t page_size;
    u8 bar_to_atu[6];
    phys_addr_t *outbound_addr;
    long unsigned int *ib_window_map;
    long unsigned int *ob_window_map;
    u32 num_ib_windows;
    u32 num_ob_windows;
    void *msi_mem;
    phys_addr_t msi_mem_phys;
    u8 msi_cap;
    u8 msix_cap;
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
struct dw_pcie_ep {
    struct pci_epc *epc;
    const struct dw_pcie_ep_ops *ops;
    phys_addr_t phys_base;
    size_t addr_size;
    size_t page_size;
    u8 bar_to_atu[6];
    phys_addr_t *outbound_addr;
    long unsigned int *ib_window_map;
    long unsigned int *ob_window_map;
    u32 num_ib_windows;
    u32 num_ob_windows;
    void *msi_mem;
    phys_addr_t msi_mem_phys;
    u8 msi_cap;
    u8 msix_cap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dw_pcie_ep {
    struct pci_epc *epc;
    const struct dw_pcie_ep_ops *ops;
    phys_addr_t phys_base;
    size_t addr_size;
    size_t page_size;
    u8 bar_to_atu[6];
    phys_addr_t *outbound_addr;
    long unsigned int *ib_window_map;
    long unsigned int *ob_window_map;
    u32 num_ib_windows;
    u32 num_ob_windows;
    void *msi_mem;
    phys_addr_t msi_mem_phys;
    u8 msi_cap;
    u8 msix_cap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dw_pcie_ep {
    struct pci_epc *epc;
    const struct dw_pcie_ep_ops *ops;
    phys_addr_t phys_base;
    size_t addr_size;
    size_t page_size;
    u8 bar_to_atu[6];
    phys_addr_t *outbound_addr;
    long unsigned int *ib_window_map;
    long unsigned int *ob_window_map;
    u32 num_ib_windows;
    u32 num_ob_windows;
    void *msi_mem;
    phys_addr_t msi_mem_phys;
    u8 msi_cap;
    u8 msix_cap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dw_pcie_ep {
    struct pci_epc *epc;
    const struct dw_pcie_ep_ops *ops;
    phys_addr_t phys_base;
    size_t addr_size;
    size_t page_size;
    u8 bar_to_atu[6];
    phys_addr_t *outbound_addr;
    long unsigned int *ib_window_map;
    long unsigned int *ob_window_map;
    u32 num_ib_windows;
    u32 num_ob_windows;
    void *msi_mem;
    phys_addr_t msi_mem_phys;
    u8 msi_cap;
    u8 msix_cap;
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
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>size_t page_size</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void *msi_mem</code>
</li>
<li>
<b>Field added. </b>
<code>phys_addr_t msi_mem_phys</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int ib_window_map</code> ➡️ <code>long unsigned int *ib_window_map</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int ob_window_map</code> ➡️ <code>long unsigned int *ob_window_map</code>
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
<code>u8 msi_cap</code>
</li>
<li>
<b>Field added. </b>
<code>u8 msix_cap</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct dw_pcie_ep_ops *ops</code> ➡️ <code>const struct dw_pcie_ep_ops *ops</code>
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
<b>Field added. </b>
<code>struct pci_epf_bar * epf_bar[6]</code>
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
<code>struct list_head func_list</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 num_ib_windows</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 num_ob_windows</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 msi_cap</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 msix_cap</code>
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
<li>
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>armhf</code> ✅
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
