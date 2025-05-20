# Struct: <code>aer_rpc</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct aer_rpc {
    struct pcie_device *rpd;
    struct work_struct dpc_handler;
    struct aer_err_source e_sources[100];
    short unsigned int prod_idx;
    short unsigned int cons_idx;
    int isr;
    spinlock_t e_lock;
    struct mutex rpc_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct aer_rpc {
    struct pcie_device *rpd;
    struct work_struct dpc_handler;
    struct aer_err_source e_sources[100];
    short unsigned int prod_idx;
    short unsigned int cons_idx;
    int isr;
    spinlock_t e_lock;
    struct mutex rpc_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct aer_rpc {
    struct pcie_device *rpd;
    struct work_struct dpc_handler;
    struct aer_err_source e_sources[100];
    struct aer_err_info e_info;
    short unsigned int prod_idx;
    short unsigned int cons_idx;
    int isr;
    spinlock_t e_lock;
    struct mutex rpc_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct aer_rpc {
    struct pcie_device *rpd;
    struct work_struct dpc_handler;
    struct aer_err_source e_sources[100];
    struct aer_err_info e_info;
    short unsigned int prod_idx;
    short unsigned int cons_idx;
    int isr;
    spinlock_t e_lock;
    struct mutex rpc_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct aer_rpc {
    struct pcie_device *rpd;
    struct work_struct dpc_handler;
    struct aer_err_source e_sources[100];
    struct aer_err_info e_info;
    short unsigned int prod_idx;
    short unsigned int cons_idx;
    int isr;
    spinlock_t e_lock;
    struct mutex rpc_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct aer_rpc {
    struct pci_dev *rpd;
    struct work_struct dpc_handler;
    struct aer_err_source e_sources[100];
    struct aer_err_info e_info;
    short unsigned int prod_idx;
    short unsigned int cons_idx;
    int isr;
    spinlock_t e_lock;
    struct mutex rpc_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct aer_rpc {
    struct pci_dev *rpd;
    struct (anon) aer_fifo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct aer_rpc {
    struct pci_dev *rpd;
    struct (anon) aer_fifo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct aer_rpc {
    struct pci_dev *rpd;
    struct (anon) aer_fifo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct aer_rpc {
    struct pci_dev *rpd;
    struct (anon) aer_fifo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct aer_rpc {
    struct pci_dev *rpd;
    struct (anon) aer_fifo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct aer_rpc {
    struct pci_dev *rpd;
    struct (anon) aer_fifo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct aer_rpc {
    struct pci_dev *rpd;
    struct (anon) aer_fifo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct aer_rpc {
    struct pci_dev *rpd;
    struct (anon) aer_fifo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct aer_rpc {
    struct pci_dev *rpd;
    struct (anon) aer_fifo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct aer_rpc {
    struct pci_dev *rpd;
    struct (anon) aer_fifo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct aer_rpc {
    struct pci_dev *rpd;
    struct (anon) aer_fifo;
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
struct aer_rpc {
    struct pci_dev *rpd;
    struct (anon) aer_fifo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct aer_rpc {
    struct pci_dev *rpd;
    struct (anon) aer_fifo;
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
struct aer_rpc {
    struct pci_dev *rpd;
    struct (anon) aer_fifo;
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
struct aer_rpc {
    struct pci_dev *rpd;
    struct (anon) aer_fifo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct aer_rpc {
    struct pci_dev *rpd;
    struct (anon) aer_fifo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct aer_rpc {
    struct pci_dev *rpd;
    struct (anon) aer_fifo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct aer_rpc {
    struct pci_dev *rpd;
    struct (anon) aer_fifo;
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
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct aer_err_info e_info</code>
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
<b>Field type changed. </b>
<code>struct pcie_device *rpd</code> ➡️ <code>struct pci_dev *rpd</code>
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
<code>struct (anon) aer_fifo</code>
</li>
<li>
<b>Field removed. </b>
<code>struct work_struct dpc_handler</code>
</li>
<li>
<b>Field removed. </b>
<code>struct aer_err_source e_sources[100]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct aer_err_info e_info</code>
</li>
<li>
<b>Field removed. </b>
<code>short unsigned int prod_idx</code>
</li>
<li>
<b>Field removed. </b>
<code>short unsigned int cons_idx</code>
</li>
<li>
<b>Field removed. </b>
<code>int isr</code>
</li>
<li>
<b>Field removed. </b>
<code>spinlock_t e_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mutex rpc_mutex</code>
</li>
</ul>
</details>
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
