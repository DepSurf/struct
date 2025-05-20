# Struct: <code>pcie_port_service_driver</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct pcie_port_service_driver {
    const char *name;
    int (*probe)(struct pcie_device *);
    void (*remove)(struct pcie_device *);
    int (*suspend)(struct pcie_device *);
    int (*resume)(struct pcie_device *);
    const struct pci_error_handlers *err_handler;
    pci_ers_result_t (*reset_link)(struct pci_dev *);
    int port_type;
    u32 service;
    struct device_driver driver;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct pcie_port_service_driver {
    const char *name;
    int (*probe)(struct pcie_device *);
    void (*remove)(struct pcie_device *);
    int (*suspend)(struct pcie_device *);
    int (*resume)(struct pcie_device *);
    const struct pci_error_handlers *err_handler;
    pci_ers_result_t (*reset_link)(struct pci_dev *);
    int port_type;
    u32 service;
    struct device_driver driver;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct pcie_port_service_driver {
    const char *name;
    int (*probe)(struct pcie_device *);
    void (*remove)(struct pcie_device *);
    int (*suspend)(struct pcie_device *);
    int (*resume)(struct pcie_device *);
    const struct pci_error_handlers *err_handler;
    pci_ers_result_t (*reset_link)(struct pci_dev *);
    int port_type;
    u32 service;
    struct device_driver driver;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct pcie_port_service_driver {
    const char *name;
    int (*probe)(struct pcie_device *);
    void (*remove)(struct pcie_device *);
    int (*suspend)(struct pcie_device *);
    int (*resume)(struct pcie_device *);
    const struct pci_error_handlers *err_handler;
    pci_ers_result_t (*reset_link)(struct pci_dev *);
    int port_type;
    u32 service;
    struct device_driver driver;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct pcie_port_service_driver {
    const char *name;
    int (*probe)(struct pcie_device *);
    void (*remove)(struct pcie_device *);
    int (*suspend)(struct pcie_device *);
    int (*resume)(struct pcie_device *);
    void (*error_resume)(struct pci_dev *);
    pci_ers_result_t (*reset_link)(struct pci_dev *);
    int port_type;
    u32 service;
    struct device_driver driver;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct pcie_port_service_driver {
    const char *name;
    int (*probe)(struct pcie_device *);
    void (*remove)(struct pcie_device *);
    int (*suspend)(struct pcie_device *);
    int (*resume)(struct pcie_device *);
    void (*error_resume)(struct pci_dev *);
    pci_ers_result_t (*reset_link)(struct pci_dev *);
    int port_type;
    u32 service;
    struct device_driver driver;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct pcie_port_service_driver {
    const char *name;
    int (*probe)(struct pcie_device *);
    void (*remove)(struct pcie_device *);
    int (*suspend)(struct pcie_device *);
    int (*resume_noirq)(struct pcie_device *);
    int (*resume)(struct pcie_device *);
    int (*runtime_suspend)(struct pcie_device *);
    int (*runtime_resume)(struct pcie_device *);
    void (*error_resume)(struct pci_dev *);
    pci_ers_result_t (*reset_link)(struct pci_dev *);
    int port_type;
    u32 service;
    struct device_driver driver;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct pcie_port_service_driver {
    const char *name;
    int (*probe)(struct pcie_device *);
    void (*remove)(struct pcie_device *);
    int (*suspend)(struct pcie_device *);
    int (*resume_noirq)(struct pcie_device *);
    int (*resume)(struct pcie_device *);
    int (*runtime_suspend)(struct pcie_device *);
    int (*runtime_resume)(struct pcie_device *);
    void (*error_resume)(struct pci_dev *);
    pci_ers_result_t (*reset_link)(struct pci_dev *);
    int port_type;
    u32 service;
    struct device_driver driver;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct pcie_port_service_driver {
    const char *name;
    int (*probe)(struct pcie_device *);
    void (*remove)(struct pcie_device *);
    int (*suspend)(struct pcie_device *);
    int (*resume_noirq)(struct pcie_device *);
    int (*resume)(struct pcie_device *);
    int (*runtime_suspend)(struct pcie_device *);
    int (*runtime_resume)(struct pcie_device *);
    void (*error_resume)(struct pci_dev *);
    pci_ers_result_t (*reset_link)(struct pci_dev *);
    int port_type;
    u32 service;
    struct device_driver driver;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct pcie_port_service_driver {
    const char *name;
    int (*probe)(struct pcie_device *);
    void (*remove)(struct pcie_device *);
    int (*suspend)(struct pcie_device *);
    int (*resume_noirq)(struct pcie_device *);
    int (*resume)(struct pcie_device *);
    int (*runtime_suspend)(struct pcie_device *);
    int (*runtime_resume)(struct pcie_device *);
    void (*error_resume)(struct pci_dev *);
    int port_type;
    u32 service;
    struct device_driver driver;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct pcie_port_service_driver {
    const char *name;
    int (*probe)(struct pcie_device *);
    void (*remove)(struct pcie_device *);
    int (*suspend)(struct pcie_device *);
    int (*resume_noirq)(struct pcie_device *);
    int (*resume)(struct pcie_device *);
    int (*runtime_suspend)(struct pcie_device *);
    int (*runtime_resume)(struct pcie_device *);
    void (*error_resume)(struct pci_dev *);
    int port_type;
    u32 service;
    struct device_driver driver;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct pcie_port_service_driver {
    const char *name;
    int (*probe)(struct pcie_device *);
    void (*remove)(struct pcie_device *);
    int (*suspend)(struct pcie_device *);
    int (*resume_noirq)(struct pcie_device *);
    int (*resume)(struct pcie_device *);
    int (*runtime_suspend)(struct pcie_device *);
    int (*runtime_resume)(struct pcie_device *);
    void (*error_resume)(struct pci_dev *);
    int port_type;
    u32 service;
    struct device_driver driver;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct pcie_port_service_driver {
    const char *name;
    int (*probe)(struct pcie_device *);
    void (*remove)(struct pcie_device *);
    int (*suspend)(struct pcie_device *);
    int (*resume_noirq)(struct pcie_device *);
    int (*resume)(struct pcie_device *);
    int (*runtime_suspend)(struct pcie_device *);
    int (*runtime_resume)(struct pcie_device *);
    void (*error_resume)(struct pci_dev *);
    int port_type;
    u32 service;
    struct device_driver driver;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct pcie_port_service_driver {
    const char *name;
    int (*probe)(struct pcie_device *);
    void (*remove)(struct pcie_device *);
    int (*suspend)(struct pcie_device *);
    int (*resume_noirq)(struct pcie_device *);
    int (*resume)(struct pcie_device *);
    int (*runtime_suspend)(struct pcie_device *);
    int (*runtime_resume)(struct pcie_device *);
    int (*slot_reset)(struct pcie_device *);
    int port_type;
    u32 service;
    struct device_driver driver;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct pcie_port_service_driver {
    const char *name;
    int (*probe)(struct pcie_device *);
    void (*remove)(struct pcie_device *);
    int (*suspend)(struct pcie_device *);
    int (*resume_noirq)(struct pcie_device *);
    int (*resume)(struct pcie_device *);
    int (*runtime_suspend)(struct pcie_device *);
    int (*runtime_resume)(struct pcie_device *);
    int (*slot_reset)(struct pcie_device *);
    int port_type;
    u32 service;
    struct device_driver driver;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct pcie_port_service_driver {
    const char *name;
    int (*probe)(struct pcie_device *);
    void (*remove)(struct pcie_device *);
    int (*suspend)(struct pcie_device *);
    int (*resume_noirq)(struct pcie_device *);
    int (*resume)(struct pcie_device *);
    int (*runtime_suspend)(struct pcie_device *);
    int (*runtime_resume)(struct pcie_device *);
    int (*slot_reset)(struct pcie_device *);
    int port_type;
    u32 service;
    struct device_driver driver;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct pcie_port_service_driver {
    const char *name;
    int (*probe)(struct pcie_device *);
    void (*remove)(struct pcie_device *);
    int (*suspend)(struct pcie_device *);
    int (*resume_noirq)(struct pcie_device *);
    int (*resume)(struct pcie_device *);
    int (*runtime_suspend)(struct pcie_device *);
    int (*runtime_resume)(struct pcie_device *);
    int (*slot_reset)(struct pcie_device *);
    int port_type;
    u32 service;
    struct device_driver driver;
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
struct pcie_port_service_driver {
    const char *name;
    int (*probe)(struct pcie_device *);
    void (*remove)(struct pcie_device *);
    int (*suspend)(struct pcie_device *);
    int (*resume_noirq)(struct pcie_device *);
    int (*resume)(struct pcie_device *);
    int (*runtime_suspend)(struct pcie_device *);
    int (*runtime_resume)(struct pcie_device *);
    void (*error_resume)(struct pci_dev *);
    pci_ers_result_t (*reset_link)(struct pci_dev *);
    int port_type;
    u32 service;
    struct device_driver driver;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct pcie_port_service_driver {
    const char *name;
    int (*probe)(struct pcie_device *);
    void (*remove)(struct pcie_device *);
    int (*suspend)(struct pcie_device *);
    int (*resume_noirq)(struct pcie_device *);
    int (*resume)(struct pcie_device *);
    int (*runtime_suspend)(struct pcie_device *);
    int (*runtime_resume)(struct pcie_device *);
    void (*error_resume)(struct pci_dev *);
    pci_ers_result_t (*reset_link)(struct pci_dev *);
    int port_type;
    u32 service;
    struct device_driver driver;
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
struct pcie_port_service_driver {
    const char *name;
    int (*probe)(struct pcie_device *);
    void (*remove)(struct pcie_device *);
    int (*suspend)(struct pcie_device *);
    int (*resume_noirq)(struct pcie_device *);
    int (*resume)(struct pcie_device *);
    int (*runtime_suspend)(struct pcie_device *);
    int (*runtime_resume)(struct pcie_device *);
    void (*error_resume)(struct pci_dev *);
    pci_ers_result_t (*reset_link)(struct pci_dev *);
    int port_type;
    u32 service;
    struct device_driver driver;
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
struct pcie_port_service_driver {
    const char *name;
    int (*probe)(struct pcie_device *);
    void (*remove)(struct pcie_device *);
    int (*suspend)(struct pcie_device *);
    int (*resume_noirq)(struct pcie_device *);
    int (*resume)(struct pcie_device *);
    int (*runtime_suspend)(struct pcie_device *);
    int (*runtime_resume)(struct pcie_device *);
    void (*error_resume)(struct pci_dev *);
    pci_ers_result_t (*reset_link)(struct pci_dev *);
    int port_type;
    u32 service;
    struct device_driver driver;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct pcie_port_service_driver {
    const char *name;
    int (*probe)(struct pcie_device *);
    void (*remove)(struct pcie_device *);
    int (*suspend)(struct pcie_device *);
    int (*resume_noirq)(struct pcie_device *);
    int (*resume)(struct pcie_device *);
    int (*runtime_suspend)(struct pcie_device *);
    int (*runtime_resume)(struct pcie_device *);
    void (*error_resume)(struct pci_dev *);
    pci_ers_result_t (*reset_link)(struct pci_dev *);
    int port_type;
    u32 service;
    struct device_driver driver;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct pcie_port_service_driver {
    const char *name;
    int (*probe)(struct pcie_device *);
    void (*remove)(struct pcie_device *);
    int (*suspend)(struct pcie_device *);
    int (*resume_noirq)(struct pcie_device *);
    int (*resume)(struct pcie_device *);
    int (*runtime_suspend)(struct pcie_device *);
    int (*runtime_resume)(struct pcie_device *);
    void (*error_resume)(struct pci_dev *);
    pci_ers_result_t (*reset_link)(struct pci_dev *);
    int port_type;
    u32 service;
    struct device_driver driver;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct pcie_port_service_driver {
    const char *name;
    int (*probe)(struct pcie_device *);
    void (*remove)(struct pcie_device *);
    int (*suspend)(struct pcie_device *);
    int (*resume_noirq)(struct pcie_device *);
    int (*resume)(struct pcie_device *);
    int (*runtime_suspend)(struct pcie_device *);
    int (*runtime_resume)(struct pcie_device *);
    void (*error_resume)(struct pci_dev *);
    pci_ers_result_t (*reset_link)(struct pci_dev *);
    int port_type;
    u32 service;
    struct device_driver driver;
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
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*error_resume)(struct pci_dev *)</code>
</li>
<li>
<b>Field removed. </b>
<code>const struct pci_error_handlers *err_handler</code>
</li>
</ul>
</details>
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
<code>int (*resume_noirq)(struct pcie_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*runtime_suspend)(struct pcie_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*runtime_resume)(struct pcie_device *)</code>
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
<b>Field removed. </b>
<code>pci_ers_result_t (*reset_link)(struct pci_dev *)</code>
</li>
</ul>
</details>
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
<b>Field added. </b>
<code>int (*slot_reset)(struct pcie_device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*error_resume)(struct pci_dev *)</code>
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
