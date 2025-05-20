# Struct: <code>dw_pcie_host_ops</code>

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
struct dw_pcie_host_ops {
    int (*rd_own_conf)(struct pcie_port *, int, int, u32 *);
    int (*wr_own_conf)(struct pcie_port *, int, int, u32);
    int (*rd_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32 *);
    int (*wr_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32);
    void (*host_init)(struct pcie_port *);
    void (*msi_set_irq)(struct pcie_port *, int);
    void (*msi_clear_irq)(struct pcie_port *, int);
    phys_addr_t (*get_msi_addr)(struct pcie_port *);
    u32 (*get_msi_data)(struct pcie_port *, int);
    void (*scan_bus)(struct pcie_port *);
    int (*msi_host_init)(struct pcie_port *, struct msi_controller *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dw_pcie_host_ops {
    int (*rd_own_conf)(struct pcie_port *, int, int, u32 *);
    int (*wr_own_conf)(struct pcie_port *, int, int, u32);
    int (*rd_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32 *);
    int (*wr_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32);
    int (*host_init)(struct pcie_port *);
    void (*msi_set_irq)(struct pcie_port *, int);
    void (*msi_clear_irq)(struct pcie_port *, int);
    phys_addr_t (*get_msi_addr)(struct pcie_port *);
    u32 (*get_msi_data)(struct pcie_port *, int);
    void (*scan_bus)(struct pcie_port *);
    int (*msi_host_init)(struct pcie_port *, struct msi_controller *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dw_pcie_host_ops {
    int (*rd_own_conf)(struct pcie_port *, int, int, u32 *);
    int (*wr_own_conf)(struct pcie_port *, int, int, u32);
    int (*rd_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32 *);
    int (*wr_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32);
    int (*host_init)(struct pcie_port *);
    void (*msi_set_irq)(struct pcie_port *, int);
    void (*msi_clear_irq)(struct pcie_port *, int);
    phys_addr_t (*get_msi_addr)(struct pcie_port *);
    u32 (*get_msi_data)(struct pcie_port *, int);
    void (*scan_bus)(struct pcie_port *);
    void (*set_num_vectors)(struct pcie_port *);
    int (*msi_host_init)(struct pcie_port *);
    void (*msi_irq_ack)(int, struct pcie_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dw_pcie_host_ops {
    int (*rd_own_conf)(struct pcie_port *, int, int, u32 *);
    int (*wr_own_conf)(struct pcie_port *, int, int, u32);
    int (*rd_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32 *);
    int (*wr_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32);
    int (*host_init)(struct pcie_port *);
    void (*msi_set_irq)(struct pcie_port *, int);
    void (*msi_clear_irq)(struct pcie_port *, int);
    phys_addr_t (*get_msi_addr)(struct pcie_port *);
    u32 (*get_msi_data)(struct pcie_port *, int);
    void (*scan_bus)(struct pcie_port *);
    void (*set_num_vectors)(struct pcie_port *);
    int (*msi_host_init)(struct pcie_port *);
    void (*msi_irq_ack)(int, struct pcie_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dw_pcie_host_ops {
    int (*rd_own_conf)(struct pcie_port *, int, int, u32 *);
    int (*wr_own_conf)(struct pcie_port *, int, int, u32);
    int (*rd_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32 *);
    int (*wr_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32);
    int (*host_init)(struct pcie_port *);
    void (*scan_bus)(struct pcie_port *);
    void (*set_num_vectors)(struct pcie_port *);
    int (*msi_host_init)(struct pcie_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dw_pcie_host_ops {
    int (*rd_own_conf)(struct pcie_port *, int, int, u32 *);
    int (*wr_own_conf)(struct pcie_port *, int, int, u32);
    int (*rd_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32 *);
    int (*wr_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32);
    int (*host_init)(struct pcie_port *);
    void (*scan_bus)(struct pcie_port *);
    void (*set_num_vectors)(struct pcie_port *);
    int (*msi_host_init)(struct pcie_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dw_pcie_host_ops {
    int (*rd_own_conf)(struct pcie_port *, int, int, u32 *);
    int (*wr_own_conf)(struct pcie_port *, int, int, u32);
    int (*rd_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32 *);
    int (*wr_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32);
    int (*host_init)(struct pcie_port *);
    void (*scan_bus)(struct pcie_port *);
    void (*set_num_vectors)(struct pcie_port *);
    int (*msi_host_init)(struct pcie_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dw_pcie_host_ops {
    int (*host_init)(struct pcie_port *);
    int (*msi_host_init)(struct pcie_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dw_pcie_host_ops {
    int (*host_init)(struct pcie_port *);
    int (*msi_host_init)(struct pcie_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dw_pcie_host_ops {
    int (*host_init)(struct pcie_port *);
    int (*msi_host_init)(struct pcie_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dw_pcie_host_ops {
    int (*host_init)(struct pcie_port *);
    int (*msi_host_init)(struct pcie_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dw_pcie_host_ops {
    int (*host_init)(struct dw_pcie_rp *);
    void (*host_deinit)(struct dw_pcie_rp *);
    int (*msi_host_init)(struct dw_pcie_rp *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dw_pcie_host_ops {
    int (*host_init)(struct dw_pcie_rp *);
    void (*host_deinit)(struct dw_pcie_rp *);
    int (*msi_host_init)(struct dw_pcie_rp *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dw_pcie_host_ops {
    int (*init)(struct dw_pcie_rp *);
    void (*deinit)(struct dw_pcie_rp *);
    void (*post_init)(struct dw_pcie_rp *);
    int (*msi_init)(struct dw_pcie_rp *);
    void (*pme_turn_off)(struct dw_pcie_rp *);
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
struct dw_pcie_host_ops {
    int (*rd_own_conf)(struct pcie_port *, int, int, u32 *);
    int (*wr_own_conf)(struct pcie_port *, int, int, u32);
    int (*rd_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32 *);
    int (*wr_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32);
    int (*host_init)(struct pcie_port *);
    void (*scan_bus)(struct pcie_port *);
    void (*set_num_vectors)(struct pcie_port *);
    int (*msi_host_init)(struct pcie_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dw_pcie_host_ops {
    int (*rd_own_conf)(struct pcie_port *, int, int, u32 *);
    int (*wr_own_conf)(struct pcie_port *, int, int, u32);
    int (*rd_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32 *);
    int (*wr_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32);
    int (*host_init)(struct pcie_port *);
    void (*scan_bus)(struct pcie_port *);
    void (*set_num_vectors)(struct pcie_port *);
    int (*msi_host_init)(struct pcie_port *);
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
struct dw_pcie_host_ops {
    int (*rd_own_conf)(struct pcie_port *, int, int, u32 *);
    int (*wr_own_conf)(struct pcie_port *, int, int, u32);
    int (*rd_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32 *);
    int (*wr_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32);
    int (*host_init)(struct pcie_port *);
    void (*scan_bus)(struct pcie_port *);
    void (*set_num_vectors)(struct pcie_port *);
    int (*msi_host_init)(struct pcie_port *);
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
struct dw_pcie_host_ops {
    int (*rd_own_conf)(struct pcie_port *, int, int, u32 *);
    int (*wr_own_conf)(struct pcie_port *, int, int, u32);
    int (*rd_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32 *);
    int (*wr_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32);
    int (*host_init)(struct pcie_port *);
    void (*scan_bus)(struct pcie_port *);
    void (*set_num_vectors)(struct pcie_port *);
    int (*msi_host_init)(struct pcie_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dw_pcie_host_ops {
    int (*rd_own_conf)(struct pcie_port *, int, int, u32 *);
    int (*wr_own_conf)(struct pcie_port *, int, int, u32);
    int (*rd_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32 *);
    int (*wr_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32);
    int (*host_init)(struct pcie_port *);
    void (*scan_bus)(struct pcie_port *);
    void (*set_num_vectors)(struct pcie_port *);
    int (*msi_host_init)(struct pcie_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dw_pcie_host_ops {
    int (*rd_own_conf)(struct pcie_port *, int, int, u32 *);
    int (*wr_own_conf)(struct pcie_port *, int, int, u32);
    int (*rd_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32 *);
    int (*wr_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32);
    int (*host_init)(struct pcie_port *);
    void (*scan_bus)(struct pcie_port *);
    void (*set_num_vectors)(struct pcie_port *);
    int (*msi_host_init)(struct pcie_port *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dw_pcie_host_ops {
    int (*rd_own_conf)(struct pcie_port *, int, int, u32 *);
    int (*wr_own_conf)(struct pcie_port *, int, int, u32);
    int (*rd_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32 *);
    int (*wr_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32);
    int (*host_init)(struct pcie_port *);
    void (*scan_bus)(struct pcie_port *);
    void (*set_num_vectors)(struct pcie_port *);
    int (*msi_host_init)(struct pcie_port *);
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
<b>Field type changed. </b>
<code>void (*host_init)(struct pcie_port *)</code> ➡️ <code>int (*host_init)(struct pcie_port *)</code>
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
<code>void (*set_num_vectors)(struct pcie_port *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*msi_irq_ack)(int, struct pcie_port *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*msi_host_init)(struct pcie_port *, struct msi_controller *)</code> ➡️ <code>int (*msi_host_init)(struct pcie_port *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>void (*msi_set_irq)(struct pcie_port *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*msi_clear_irq)(struct pcie_port *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>phys_addr_t (*get_msi_addr)(struct pcie_port *)</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 (*get_msi_data)(struct pcie_port *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*msi_irq_ack)(int, struct pcie_port *)</code>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*rd_own_conf)(struct pcie_port *, int, int, u32 *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*wr_own_conf)(struct pcie_port *, int, int, u32)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*rd_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32 *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*wr_other_conf)(struct pcie_port *, struct pci_bus *, unsigned int, int, int, u32)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*scan_bus)(struct pcie_port *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*set_num_vectors)(struct pcie_port *)</code>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*host_deinit)(struct dw_pcie_rp *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*host_init)(struct pcie_port *)</code> ➡️ <code>int (*host_init)(struct dw_pcie_rp *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*msi_host_init)(struct pcie_port *)</code> ➡️ <code>int (*msi_host_init)(struct dw_pcie_rp *)</code>
</li>
</ul>
</details>
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
<code>int (*init)(struct dw_pcie_rp *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*deinit)(struct dw_pcie_rp *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*post_init)(struct dw_pcie_rp *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*msi_init)(struct dw_pcie_rp *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*pme_turn_off)(struct dw_pcie_rp *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*host_init)(struct dw_pcie_rp *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*host_deinit)(struct dw_pcie_rp *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*msi_host_init)(struct dw_pcie_rp *)</code>
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
