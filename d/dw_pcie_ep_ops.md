# Struct: <code>dw_pcie_ep_ops</code>

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
struct dw_pcie_ep_ops {
    void (*ep_init)(struct dw_pcie_ep *);
    int (*raise_irq)(struct dw_pcie_ep *, enum pci_epc_irq_type, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dw_pcie_ep_ops {
    void (*ep_init)(struct dw_pcie_ep *);
    int (*raise_irq)(struct dw_pcie_ep *, enum pci_epc_irq_type, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dw_pcie_ep_ops {
    void (*ep_init)(struct dw_pcie_ep *);
    int (*raise_irq)(struct dw_pcie_ep *, u8, enum pci_epc_irq_type, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dw_pcie_ep_ops {
    void (*ep_init)(struct dw_pcie_ep *);
    int (*raise_irq)(struct dw_pcie_ep *, u8, enum pci_epc_irq_type, u16);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dw_pcie_ep_ops {
    void (*ep_init)(struct dw_pcie_ep *);
    int (*raise_irq)(struct dw_pcie_ep *, u8, enum pci_epc_irq_type, u16);
    const struct pci_epc_features * (*get_features)(struct dw_pcie_ep *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dw_pcie_ep_ops {
    void (*ep_init)(struct dw_pcie_ep *);
    int (*raise_irq)(struct dw_pcie_ep *, u8, enum pci_epc_irq_type, u16);
    const struct pci_epc_features * (*get_features)(struct dw_pcie_ep *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dw_pcie_ep_ops {
    void (*ep_init)(struct dw_pcie_ep *);
    int (*raise_irq)(struct dw_pcie_ep *, u8, enum pci_epc_irq_type, u16);
    const struct pci_epc_features * (*get_features)(struct dw_pcie_ep *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dw_pcie_ep_ops {
    void (*ep_init)(struct dw_pcie_ep *);
    int (*raise_irq)(struct dw_pcie_ep *, u8, enum pci_epc_irq_type, u16);
    const struct pci_epc_features * (*get_features)(struct dw_pcie_ep *);
    unsigned int (*func_conf_select)(struct dw_pcie_ep *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dw_pcie_ep_ops {
    void (*ep_init)(struct dw_pcie_ep *);
    int (*raise_irq)(struct dw_pcie_ep *, u8, enum pci_epc_irq_type, u16);
    const struct pci_epc_features * (*get_features)(struct dw_pcie_ep *);
    unsigned int (*func_conf_select)(struct dw_pcie_ep *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dw_pcie_ep_ops {
    void (*ep_init)(struct dw_pcie_ep *);
    int (*raise_irq)(struct dw_pcie_ep *, u8, enum pci_epc_irq_type, u16);
    const struct pci_epc_features * (*get_features)(struct dw_pcie_ep *);
    unsigned int (*func_conf_select)(struct dw_pcie_ep *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dw_pcie_ep_ops {
    void (*ep_init)(struct dw_pcie_ep *);
    int (*raise_irq)(struct dw_pcie_ep *, u8, enum pci_epc_irq_type, u16);
    const struct pci_epc_features * (*get_features)(struct dw_pcie_ep *);
    unsigned int (*func_conf_select)(struct dw_pcie_ep *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dw_pcie_ep_ops {
    void (*ep_init)(struct dw_pcie_ep *);
    int (*raise_irq)(struct dw_pcie_ep *, u8, enum pci_epc_irq_type, u16);
    const struct pci_epc_features * (*get_features)(struct dw_pcie_ep *);
    unsigned int (*func_conf_select)(struct dw_pcie_ep *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dw_pcie_ep_ops {
    void (*ep_init)(struct dw_pcie_ep *);
    int (*raise_irq)(struct dw_pcie_ep *, u8, enum pci_epc_irq_type, u16);
    const struct pci_epc_features * (*get_features)(struct dw_pcie_ep *);
    unsigned int (*func_conf_select)(struct dw_pcie_ep *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dw_pcie_ep_ops {
    void (*pre_init)(struct dw_pcie_ep *);
    void (*init)(struct dw_pcie_ep *);
    void (*deinit)(struct dw_pcie_ep *);
    int (*raise_irq)(struct dw_pcie_ep *, u8, unsigned int, u16);
    const struct pci_epc_features * (*get_features)(struct dw_pcie_ep *);
    unsigned int (*get_dbi_offset)(struct dw_pcie_ep *, u8);
    unsigned int (*get_dbi2_offset)(struct dw_pcie_ep *, u8);
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
struct dw_pcie_ep_ops {
    void (*ep_init)(struct dw_pcie_ep *);
    int (*raise_irq)(struct dw_pcie_ep *, u8, enum pci_epc_irq_type, u16);
    const struct pci_epc_features * (*get_features)(struct dw_pcie_ep *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dw_pcie_ep_ops {
    void (*ep_init)(struct dw_pcie_ep *);
    int (*raise_irq)(struct dw_pcie_ep *, u8, enum pci_epc_irq_type, u16);
    const struct pci_epc_features * (*get_features)(struct dw_pcie_ep *);
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
struct dw_pcie_ep_ops {
    void (*ep_init)(struct dw_pcie_ep *);
    int (*raise_irq)(struct dw_pcie_ep *, u8, enum pci_epc_irq_type, u16);
    const struct pci_epc_features * (*get_features)(struct dw_pcie_ep *);
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
struct dw_pcie_ep_ops {
    void (*ep_init)(struct dw_pcie_ep *);
    int (*raise_irq)(struct dw_pcie_ep *, u8, enum pci_epc_irq_type, u16);
    const struct pci_epc_features * (*get_features)(struct dw_pcie_ep *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dw_pcie_ep_ops {
    void (*ep_init)(struct dw_pcie_ep *);
    int (*raise_irq)(struct dw_pcie_ep *, u8, enum pci_epc_irq_type, u16);
    const struct pci_epc_features * (*get_features)(struct dw_pcie_ep *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dw_pcie_ep_ops {
    void (*ep_init)(struct dw_pcie_ep *);
    int (*raise_irq)(struct dw_pcie_ep *, u8, enum pci_epc_irq_type, u16);
    const struct pci_epc_features * (*get_features)(struct dw_pcie_ep *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dw_pcie_ep_ops {
    void (*ep_init)(struct dw_pcie_ep *);
    int (*raise_irq)(struct dw_pcie_ep *, u8, enum pci_epc_irq_type, u16);
    const struct pci_epc_features * (*get_features)(struct dw_pcie_ep *);
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
<code>int (*raise_irq)(struct dw_pcie_ep *, enum pci_epc_irq_type, u8)</code> ➡️ <code>int (*raise_irq)(struct dw_pcie_ep *, u8, enum pci_epc_irq_type, u8)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*raise_irq)(struct dw_pcie_ep *, u8, enum pci_epc_irq_type, u8)</code> ➡️ <code>int (*raise_irq)(struct dw_pcie_ep *, u8, enum pci_epc_irq_type, u16)</code>
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
<code>const struct pci_epc_features * (*get_features)(struct dw_pcie_ep *)</code>
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
<b>Field added. </b>
<code>unsigned int (*func_conf_select)(struct dw_pcie_ep *, u8)</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*pre_init)(struct dw_pcie_ep *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*init)(struct dw_pcie_ep *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*deinit)(struct dw_pcie_ep *)</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int (*get_dbi_offset)(struct dw_pcie_ep *, u8)</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int (*get_dbi2_offset)(struct dw_pcie_ep *, u8)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*ep_init)(struct dw_pcie_ep *)</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int (*func_conf_select)(struct dw_pcie_ep *, u8)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*raise_irq)(struct dw_pcie_ep *, u8, enum pci_epc_irq_type, u16)</code> ➡️ <code>int (*raise_irq)(struct dw_pcie_ep *, u8, unsigned int, u16)</code>
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
