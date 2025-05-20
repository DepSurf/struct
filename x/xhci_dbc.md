# Struct: <code>xhci_dbc</code>

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
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct xhci_dbc {
    spinlock_t lock;
    struct xhci_hcd *xhci;
    struct dbc_regs *regs;
    struct xhci_ring *ring_evt;
    struct xhci_ring *ring_in;
    struct xhci_ring *ring_out;
    struct xhci_erst erst;
    struct xhci_container_ctx *ctx;
    struct dbc_str_descs *string;
    dma_addr_t string_dma;
    size_t string_size;
    enum dbc_state state;
    struct delayed_work event_work;
    unsigned int resume_required;
    struct dbc_ep eps[2];
    struct dbc_port port;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct xhci_dbc {
    spinlock_t lock;
    struct xhci_hcd *xhci;
    struct dbc_regs *regs;
    struct xhci_ring *ring_evt;
    struct xhci_ring *ring_in;
    struct xhci_ring *ring_out;
    struct xhci_erst erst;
    struct xhci_container_ctx *ctx;
    struct dbc_str_descs *string;
    dma_addr_t string_dma;
    size_t string_size;
    enum dbc_state state;
    struct delayed_work event_work;
    unsigned int resume_required;
    struct dbc_ep eps[2];
    struct dbc_port port;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct xhci_dbc {
    spinlock_t lock;
    struct xhci_hcd *xhci;
    struct dbc_regs *regs;
    struct xhci_ring *ring_evt;
    struct xhci_ring *ring_in;
    struct xhci_ring *ring_out;
    struct xhci_erst erst;
    struct xhci_container_ctx *ctx;
    struct dbc_str_descs *string;
    dma_addr_t string_dma;
    size_t string_size;
    enum dbc_state state;
    struct delayed_work event_work;
    unsigned int resume_required;
    struct dbc_ep eps[2];
    struct dbc_port port;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct xhci_dbc {
    spinlock_t lock;
    struct xhci_hcd *xhci;
    struct dbc_regs *regs;
    struct xhci_ring *ring_evt;
    struct xhci_ring *ring_in;
    struct xhci_ring *ring_out;
    struct xhci_erst erst;
    struct xhci_container_ctx *ctx;
    struct dbc_str_descs *string;
    dma_addr_t string_dma;
    size_t string_size;
    enum dbc_state state;
    struct delayed_work event_work;
    unsigned int resume_required;
    struct dbc_ep eps[2];
    struct dbc_port port;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct xhci_dbc {
    spinlock_t lock;
    struct xhci_hcd *xhci;
    struct dbc_regs *regs;
    struct xhci_ring *ring_evt;
    struct xhci_ring *ring_in;
    struct xhci_ring *ring_out;
    struct xhci_erst erst;
    struct xhci_container_ctx *ctx;
    struct dbc_str_descs *string;
    dma_addr_t string_dma;
    size_t string_size;
    enum dbc_state state;
    struct delayed_work event_work;
    unsigned int resume_required;
    struct dbc_ep eps[2];
    struct dbc_port port;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct xhci_dbc {
    spinlock_t lock;
    struct xhci_hcd *xhci;
    struct dbc_regs *regs;
    struct xhci_ring *ring_evt;
    struct xhci_ring *ring_in;
    struct xhci_ring *ring_out;
    struct xhci_erst erst;
    struct xhci_container_ctx *ctx;
    struct dbc_str_descs *string;
    dma_addr_t string_dma;
    size_t string_size;
    enum dbc_state state;
    struct delayed_work event_work;
    unsigned int resume_required;
    struct dbc_ep eps[2];
    struct dbc_port port;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct xhci_dbc {
    spinlock_t lock;
    struct device *dev;
    struct xhci_hcd *xhci;
    struct dbc_regs *regs;
    struct xhci_ring *ring_evt;
    struct xhci_ring *ring_in;
    struct xhci_ring *ring_out;
    struct xhci_erst erst;
    struct xhci_container_ctx *ctx;
    struct dbc_str_descs *string;
    dma_addr_t string_dma;
    size_t string_size;
    enum dbc_state state;
    struct delayed_work event_work;
    unsigned int resume_required;
    struct dbc_ep eps[2];
    const struct dbc_driver *driver;
    void *priv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct xhci_dbc {
    spinlock_t lock;
    struct device *dev;
    struct xhci_hcd *xhci;
    struct dbc_regs *regs;
    struct xhci_ring *ring_evt;
    struct xhci_ring *ring_in;
    struct xhci_ring *ring_out;
    struct xhci_erst erst;
    struct xhci_container_ctx *ctx;
    struct dbc_str_descs *string;
    dma_addr_t string_dma;
    size_t string_size;
    enum dbc_state state;
    struct delayed_work event_work;
    unsigned int resume_required;
    struct dbc_ep eps[2];
    const struct dbc_driver *driver;
    void *priv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct xhci_dbc {
    spinlock_t lock;
    struct device *dev;
    struct xhci_hcd *xhci;
    struct dbc_regs *regs;
    struct xhci_ring *ring_evt;
    struct xhci_ring *ring_in;
    struct xhci_ring *ring_out;
    struct xhci_erst erst;
    struct xhci_container_ctx *ctx;
    struct dbc_str_descs *string;
    dma_addr_t string_dma;
    size_t string_size;
    enum dbc_state state;
    struct delayed_work event_work;
    unsigned int resume_required;
    struct dbc_ep eps[2];
    const struct dbc_driver *driver;
    void *priv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct xhci_dbc {
    spinlock_t lock;
    struct device *dev;
    struct xhci_hcd *xhci;
    struct dbc_regs *regs;
    struct xhci_ring *ring_evt;
    struct xhci_ring *ring_in;
    struct xhci_ring *ring_out;
    struct xhci_erst erst;
    struct xhci_container_ctx *ctx;
    struct dbc_str_descs *string;
    dma_addr_t string_dma;
    size_t string_size;
    enum dbc_state state;
    struct delayed_work event_work;
    unsigned int resume_required;
    struct dbc_ep eps[2];
    const struct dbc_driver *driver;
    void *priv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct xhci_dbc {
    spinlock_t lock;
    struct device *dev;
    struct xhci_hcd *xhci;
    struct dbc_regs *regs;
    struct xhci_ring *ring_evt;
    struct xhci_ring *ring_in;
    struct xhci_ring *ring_out;
    struct xhci_erst erst;
    struct xhci_container_ctx *ctx;
    struct dbc_str_descs *string;
    dma_addr_t string_dma;
    size_t string_size;
    enum dbc_state state;
    struct delayed_work event_work;
    unsigned int resume_required;
    struct dbc_ep eps[2];
    const struct dbc_driver *driver;
    void *priv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct xhci_dbc {
    spinlock_t lock;
    struct device *dev;
    struct xhci_hcd *xhci;
    struct dbc_regs *regs;
    struct xhci_ring *ring_evt;
    struct xhci_ring *ring_in;
    struct xhci_ring *ring_out;
    struct xhci_erst erst;
    struct xhci_container_ctx *ctx;
    struct dbc_str_descs *string;
    dma_addr_t string_dma;
    size_t string_size;
    u16 idVendor;
    u16 idProduct;
    u16 bcdDevice;
    u8 bInterfaceProtocol;
    enum dbc_state state;
    struct delayed_work event_work;
    unsigned int resume_required;
    struct dbc_ep eps[2];
    const struct dbc_driver *driver;
    void *priv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct xhci_dbc {
    spinlock_t lock;
    struct device *dev;
    struct xhci_hcd *xhci;
    struct dbc_regs *regs;
    struct xhci_ring *ring_evt;
    struct xhci_ring *ring_in;
    struct xhci_ring *ring_out;
    struct xhci_erst erst;
    struct xhci_container_ctx *ctx;
    struct dbc_str_descs *string;
    dma_addr_t string_dma;
    size_t string_size;
    u16 idVendor;
    u16 idProduct;
    u16 bcdDevice;
    u8 bInterfaceProtocol;
    enum dbc_state state;
    struct delayed_work event_work;
    unsigned int resume_required;
    struct dbc_ep eps[2];
    const struct dbc_driver *driver;
    void *priv;
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
struct xhci_dbc {
    spinlock_t lock;
    struct xhci_hcd *xhci;
    struct dbc_regs *regs;
    struct xhci_ring *ring_evt;
    struct xhci_ring *ring_in;
    struct xhci_ring *ring_out;
    struct xhci_erst erst;
    struct xhci_container_ctx *ctx;
    struct dbc_str_descs *string;
    dma_addr_t string_dma;
    size_t string_size;
    enum dbc_state state;
    struct delayed_work event_work;
    unsigned int resume_required;
    struct dbc_ep eps[2];
    struct dbc_port port;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct xhci_dbc {
    spinlock_t lock;
    struct xhci_hcd *xhci;
    struct dbc_regs *regs;
    struct xhci_ring *ring_evt;
    struct xhci_ring *ring_in;
    struct xhci_ring *ring_out;
    struct xhci_erst erst;
    struct xhci_container_ctx *ctx;
    struct dbc_str_descs *string;
    dma_addr_t string_dma;
    size_t string_size;
    enum dbc_state state;
    struct delayed_work event_work;
    unsigned int resume_required;
    struct dbc_ep eps[2];
    struct dbc_port port;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct xhci_dbc {
    spinlock_t lock;
    struct xhci_hcd *xhci;
    struct dbc_regs *regs;
    struct xhci_ring *ring_evt;
    struct xhci_ring *ring_in;
    struct xhci_ring *ring_out;
    struct xhci_erst erst;
    struct xhci_container_ctx *ctx;
    struct dbc_str_descs *string;
    dma_addr_t string_dma;
    size_t string_size;
    enum dbc_state state;
    struct delayed_work event_work;
    unsigned int resume_required;
    struct dbc_ep eps[2];
    struct dbc_port port;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct xhci_dbc {
    spinlock_t lock;
    struct xhci_hcd *xhci;
    struct dbc_regs *regs;
    struct xhci_ring *ring_evt;
    struct xhci_ring *ring_in;
    struct xhci_ring *ring_out;
    struct xhci_erst erst;
    struct xhci_container_ctx *ctx;
    struct dbc_str_descs *string;
    dma_addr_t string_dma;
    size_t string_size;
    enum dbc_state state;
    struct delayed_work event_work;
    unsigned int resume_required;
    struct dbc_ep eps[2];
    struct dbc_port port;
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
struct xhci_dbc {
    spinlock_t lock;
    struct xhci_hcd *xhci;
    struct dbc_regs *regs;
    struct xhci_ring *ring_evt;
    struct xhci_ring *ring_in;
    struct xhci_ring *ring_out;
    struct xhci_erst erst;
    struct xhci_container_ctx *ctx;
    struct dbc_str_descs *string;
    dma_addr_t string_dma;
    size_t string_size;
    enum dbc_state state;
    struct delayed_work event_work;
    unsigned int resume_required;
    struct dbc_ep eps[2];
    struct dbc_port port;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct xhci_dbc {
    spinlock_t lock;
    struct xhci_hcd *xhci;
    struct dbc_regs *regs;
    struct xhci_ring *ring_evt;
    struct xhci_ring *ring_in;
    struct xhci_ring *ring_out;
    struct xhci_erst erst;
    struct xhci_container_ctx *ctx;
    struct dbc_str_descs *string;
    dma_addr_t string_dma;
    size_t string_size;
    enum dbc_state state;
    struct delayed_work event_work;
    unsigned int resume_required;
    struct dbc_ep eps[2];
    struct dbc_port port;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct xhci_dbc {
    spinlock_t lock;
    struct xhci_hcd *xhci;
    struct dbc_regs *regs;
    struct xhci_ring *ring_evt;
    struct xhci_ring *ring_in;
    struct xhci_ring *ring_out;
    struct xhci_erst erst;
    struct xhci_container_ctx *ctx;
    struct dbc_str_descs *string;
    dma_addr_t string_dma;
    size_t string_size;
    enum dbc_state state;
    struct delayed_work event_work;
    unsigned int resume_required;
    struct dbc_ep eps[2];
    struct dbc_port port;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct xhci_dbc {
    spinlock_t lock;
    struct xhci_hcd *xhci;
    struct dbc_regs *regs;
    struct xhci_ring *ring_evt;
    struct xhci_ring *ring_in;
    struct xhci_ring *ring_out;
    struct xhci_erst erst;
    struct xhci_container_ctx *ctx;
    struct dbc_str_descs *string;
    dma_addr_t string_dma;
    size_t string_size;
    enum dbc_state state;
    struct delayed_work event_work;
    unsigned int resume_required;
    struct dbc_ep eps[2];
    struct dbc_port port;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct device *dev</code>
</li>
<li>
<b>Field added. </b>
<code>const struct dbc_driver *driver</code>
</li>
<li>
<b>Field added. </b>
<code>void *priv</code>
</li>
<li>
<b>Field removed. </b>
<code>struct dbc_port port</code>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 idVendor</code>
</li>
<li>
<b>Field added. </b>
<code>u16 idProduct</code>
</li>
<li>
<b>Field added. </b>
<code>u16 bcdDevice</code>
</li>
<li>
<b>Field added. </b>
<code>u8 bInterfaceProtocol</code>
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
