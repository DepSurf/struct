# Struct: <code>pci_epf</code>

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
struct pci_epf {
    struct device dev;
    const char *name;
    struct pci_epf_header *header;
    struct pci_epf_bar bar[6];
    u8 msi_interrupts;
    u8 func_no;
    struct pci_epc *epc;
    struct pci_epf_driver *driver;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct pci_epf {
    struct device dev;
    const char *name;
    struct pci_epf_header *header;
    struct pci_epf_bar bar[6];
    u8 msi_interrupts;
    u8 func_no;
    struct pci_epc *epc;
    struct pci_epf_driver *driver;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct pci_epf {
    struct device dev;
    const char *name;
    struct pci_epf_header *header;
    struct pci_epf_bar bar[6];
    u8 msi_interrupts;
    u8 func_no;
    struct pci_epc *epc;
    struct pci_epf_driver *driver;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct pci_epf {
    struct device dev;
    const char *name;
    struct pci_epf_header *header;
    struct pci_epf_bar bar[6];
    u8 msi_interrupts;
    u16 msix_interrupts;
    u8 func_no;
    struct pci_epc *epc;
    struct pci_epf_driver *driver;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct pci_epf {
    struct device dev;
    const char *name;
    struct pci_epf_header *header;
    struct pci_epf_bar bar[6];
    u8 msi_interrupts;
    u16 msix_interrupts;
    u8 func_no;
    struct pci_epc *epc;
    struct pci_epf_driver *driver;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct pci_epf {
    struct device dev;
    const char *name;
    struct pci_epf_header *header;
    struct pci_epf_bar bar[6];
    u8 msi_interrupts;
    u16 msix_interrupts;
    u8 func_no;
    struct pci_epc *epc;
    struct pci_epf_driver *driver;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct pci_epf {
    struct device dev;
    const char *name;
    struct pci_epf_header *header;
    struct pci_epf_bar bar[6];
    u8 msi_interrupts;
    u16 msix_interrupts;
    u8 func_no;
    struct pci_epc *epc;
    struct pci_epf_driver *driver;
    struct list_head list;
    struct notifier_block nb;
    struct mutex lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct pci_epf {
    struct device dev;
    const char *name;
    struct pci_epf_header *header;
    struct pci_epf_bar bar[6];
    u8 msi_interrupts;
    u16 msix_interrupts;
    u8 func_no;
    struct pci_epc *epc;
    struct pci_epf_driver *driver;
    struct list_head list;
    struct notifier_block nb;
    struct mutex lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct pci_epf {
    struct device dev;
    const char *name;
    struct pci_epf_header *header;
    struct pci_epf_bar bar[6];
    u8 msi_interrupts;
    u16 msix_interrupts;
    u8 func_no;
    struct pci_epc *epc;
    struct pci_epf_driver *driver;
    struct list_head list;
    struct notifier_block nb;
    struct mutex lock;
    struct pci_epc *sec_epc;
    struct list_head sec_epc_list;
    struct pci_epf_bar sec_epc_bar[6];
    u8 sec_epc_func_no;
    struct config_group *group;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct pci_epf {
    struct device dev;
    const char *name;
    struct pci_epf_header *header;
    struct pci_epf_bar bar[6];
    u8 msi_interrupts;
    u16 msix_interrupts;
    u8 func_no;
    u8 vfunc_no;
    struct pci_epc *epc;
    struct pci_epf *epf_pf;
    struct pci_epf_driver *driver;
    struct list_head list;
    struct notifier_block nb;
    struct mutex lock;
    struct pci_epc *sec_epc;
    struct list_head sec_epc_list;
    struct pci_epf_bar sec_epc_bar[6];
    u8 sec_epc_func_no;
    struct config_group *group;
    unsigned int is_bound;
    unsigned int is_vf;
    long unsigned int vfunction_num_map;
    struct list_head pci_vepf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct pci_epf {
    struct device dev;
    const char *name;
    struct pci_epf_header *header;
    struct pci_epf_bar bar[6];
    u8 msi_interrupts;
    u16 msix_interrupts;
    u8 func_no;
    u8 vfunc_no;
    struct pci_epc *epc;
    struct pci_epf *epf_pf;
    struct pci_epf_driver *driver;
    struct list_head list;
    struct notifier_block nb;
    struct mutex lock;
    struct pci_epc *sec_epc;
    struct list_head sec_epc_list;
    struct pci_epf_bar sec_epc_bar[6];
    u8 sec_epc_func_no;
    struct config_group *group;
    unsigned int is_bound;
    unsigned int is_vf;
    long unsigned int vfunction_num_map;
    struct list_head pci_vepf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct pci_epf {
    struct device dev;
    const char *name;
    struct pci_epf_header *header;
    struct pci_epf_bar bar[6];
    u8 msi_interrupts;
    u16 msix_interrupts;
    u8 func_no;
    u8 vfunc_no;
    struct pci_epc *epc;
    struct pci_epf *epf_pf;
    struct pci_epf_driver *driver;
    struct list_head list;
    struct notifier_block nb;
    struct mutex lock;
    struct pci_epc *sec_epc;
    struct list_head sec_epc_list;
    struct pci_epf_bar sec_epc_bar[6];
    u8 sec_epc_func_no;
    struct config_group *group;
    unsigned int is_bound;
    unsigned int is_vf;
    long unsigned int vfunction_num_map;
    struct list_head pci_vepf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct pci_epf {
    struct device dev;
    const char *name;
    struct pci_epf_header *header;
    struct pci_epf_bar bar[6];
    u8 msi_interrupts;
    u16 msix_interrupts;
    u8 func_no;
    u8 vfunc_no;
    struct pci_epc *epc;
    struct pci_epf *epf_pf;
    struct pci_epf_driver *driver;
    const struct pci_epf_device_id *id;
    struct list_head list;
    struct mutex lock;
    struct pci_epc *sec_epc;
    struct list_head sec_epc_list;
    struct pci_epf_bar sec_epc_bar[6];
    u8 sec_epc_func_no;
    struct config_group *group;
    unsigned int is_bound;
    unsigned int is_vf;
    long unsigned int vfunction_num_map;
    struct list_head pci_vepf;
    const struct pci_epc_event_ops *event_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct pci_epf {
    struct device dev;
    const char *name;
    struct pci_epf_header *header;
    struct pci_epf_bar bar[6];
    u8 msi_interrupts;
    u16 msix_interrupts;
    u8 func_no;
    u8 vfunc_no;
    struct pci_epc *epc;
    struct pci_epf *epf_pf;
    struct pci_epf_driver *driver;
    const struct pci_epf_device_id *id;
    struct list_head list;
    struct mutex lock;
    struct pci_epc *sec_epc;
    struct list_head sec_epc_list;
    struct pci_epf_bar sec_epc_bar[6];
    u8 sec_epc_func_no;
    struct config_group *group;
    unsigned int is_bound;
    unsigned int is_vf;
    long unsigned int vfunction_num_map;
    struct list_head pci_vepf;
    const struct pci_epc_event_ops *event_ops;
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
struct pci_epf {
    struct device dev;
    const char *name;
    struct pci_epf_header *header;
    struct pci_epf_bar bar[6];
    u8 msi_interrupts;
    u16 msix_interrupts;
    u8 func_no;
    struct pci_epc *epc;
    struct pci_epf_driver *driver;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct pci_epf {
    struct device dev;
    const char *name;
    struct pci_epf_header *header;
    struct pci_epf_bar bar[6];
    u8 msi_interrupts;
    u16 msix_interrupts;
    u8 func_no;
    struct pci_epc *epc;
    struct pci_epf_driver *driver;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct pci_epf {
    struct device dev;
    const char *name;
    struct pci_epf_header *header;
    struct pci_epf_bar bar[6];
    u8 msi_interrupts;
    u16 msix_interrupts;
    u8 func_no;
    struct pci_epc *epc;
    struct pci_epf_driver *driver;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct pci_epf {
    struct device dev;
    const char *name;
    struct pci_epf_header *header;
    struct pci_epf_bar bar[6];
    u8 msi_interrupts;
    u16 msix_interrupts;
    u8 func_no;
    struct pci_epc *epc;
    struct pci_epf_driver *driver;
    struct list_head list;
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
struct pci_epf {
    struct device dev;
    const char *name;
    struct pci_epf_header *header;
    struct pci_epf_bar bar[6];
    u8 msi_interrupts;
    u16 msix_interrupts;
    u8 func_no;
    struct pci_epc *epc;
    struct pci_epf_driver *driver;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct pci_epf {
    struct device dev;
    const char *name;
    struct pci_epf_header *header;
    struct pci_epf_bar bar[6];
    u8 msi_interrupts;
    u16 msix_interrupts;
    u8 func_no;
    struct pci_epc *epc;
    struct pci_epf_driver *driver;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct pci_epf {
    struct device dev;
    const char *name;
    struct pci_epf_header *header;
    struct pci_epf_bar bar[6];
    u8 msi_interrupts;
    u16 msix_interrupts;
    u8 func_no;
    struct pci_epc *epc;
    struct pci_epf_driver *driver;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct pci_epf {
    struct device dev;
    const char *name;
    struct pci_epf_header *header;
    struct pci_epf_bar bar[6];
    u8 msi_interrupts;
    u16 msix_interrupts;
    u8 func_no;
    struct pci_epc *epc;
    struct pci_epf_driver *driver;
    struct list_head list;
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
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 msix_interrupts</code>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct notifier_block nb</code>
</li>
<li>
<b>Field added. </b>
<code>struct mutex lock</code>
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
<code>struct pci_epc *sec_epc</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head sec_epc_list</code>
</li>
<li>
<b>Field added. </b>
<code>struct pci_epf_bar sec_epc_bar[6]</code>
</li>
<li>
<b>Field added. </b>
<code>u8 sec_epc_func_no</code>
</li>
<li>
<b>Field added. </b>
<code>struct config_group *group</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 vfunc_no</code>
</li>
<li>
<b>Field added. </b>
<code>struct pci_epf *epf_pf</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int is_bound</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int is_vf</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int vfunction_num_map</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head pci_vepf</code>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const struct pci_epf_device_id *id</code>
</li>
<li>
<b>Field added. </b>
<code>const struct pci_epc_event_ops *event_ops</code>
</li>
<li>
<b>Field removed. </b>
<code>struct notifier_block nb</code>
</li>
</ul>
</details>
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
