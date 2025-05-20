# Struct: <code>rio_mport</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct rio_mport {
    struct list_head dbells;
    struct list_head node;
    struct list_head nnode;
    struct resource iores;
    struct resource riores[16];
    struct rio_msg inb_msg[4];
    struct rio_msg outb_msg[4];
    int host_deviceid;
    struct rio_ops *ops;
    unsigned char id;
    unsigned char index;
    unsigned int sys_size;
    enum rio_phy_type phy_type;
    u32 phys_efptr;
    unsigned char name[40];
    struct device dev;
    void *priv;
    struct dma_device dma;
    struct rio_scan *nscan;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct rio_mport {
    struct list_head dbells;
    struct list_head pwrites;
    struct list_head node;
    struct list_head nnode;
    struct rio_net *net;
    struct mutex lock;
    struct resource iores;
    struct resource riores[16];
    struct rio_msg inb_msg[4];
    struct rio_msg outb_msg[4];
    int host_deviceid;
    struct rio_ops *ops;
    unsigned char id;
    unsigned char index;
    unsigned int sys_size;
    u32 phys_efptr;
    u32 phys_rmap;
    unsigned char name[40];
    struct device dev;
    void *priv;
    struct dma_device dma;
    struct rio_scan *nscan;
    atomic_t state;
    unsigned int pwe_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rio_mport {
    struct list_head dbells;
    struct list_head pwrites;
    struct list_head node;
    struct list_head nnode;
    struct rio_net *net;
    struct mutex lock;
    struct resource iores;
    struct resource riores[16];
    struct rio_msg inb_msg[4];
    struct rio_msg outb_msg[4];
    int host_deviceid;
    struct rio_ops *ops;
    unsigned char id;
    unsigned char index;
    unsigned int sys_size;
    u32 phys_efptr;
    u32 phys_rmap;
    unsigned char name[40];
    struct device dev;
    void *priv;
    struct dma_device dma;
    struct rio_scan *nscan;
    atomic_t state;
    unsigned int pwe_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rio_mport {
    struct list_head dbells;
    struct list_head pwrites;
    struct list_head node;
    struct list_head nnode;
    struct rio_net *net;
    struct mutex lock;
    struct resource iores;
    struct resource riores[16];
    struct rio_msg inb_msg[4];
    struct rio_msg outb_msg[4];
    int host_deviceid;
    struct rio_ops *ops;
    unsigned char id;
    unsigned char index;
    unsigned int sys_size;
    u32 phys_efptr;
    u32 phys_rmap;
    unsigned char name[40];
    struct device dev;
    void *priv;
    struct dma_device dma;
    struct rio_scan *nscan;
    atomic_t state;
    unsigned int pwe_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rio_mport {
    struct list_head dbells;
    struct list_head pwrites;
    struct list_head node;
    struct list_head nnode;
    struct rio_net *net;
    struct mutex lock;
    struct resource iores;
    struct resource riores[16];
    struct rio_msg inb_msg[4];
    struct rio_msg outb_msg[4];
    int host_deviceid;
    struct rio_ops *ops;
    unsigned char id;
    unsigned char index;
    unsigned int sys_size;
    u32 phys_efptr;
    u32 phys_rmap;
    unsigned char name[40];
    struct device dev;
    void *priv;
    struct dma_device dma;
    struct rio_scan *nscan;
    atomic_t state;
    unsigned int pwe_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rio_mport {
    struct list_head dbells;
    struct list_head pwrites;
    struct list_head node;
    struct list_head nnode;
    struct rio_net *net;
    struct mutex lock;
    struct resource iores;
    struct resource riores[16];
    struct rio_msg inb_msg[4];
    struct rio_msg outb_msg[4];
    int host_deviceid;
    struct rio_ops *ops;
    unsigned char id;
    unsigned char index;
    unsigned int sys_size;
    u32 phys_efptr;
    u32 phys_rmap;
    unsigned char name[40];
    struct device dev;
    void *priv;
    struct dma_device dma;
    struct rio_scan *nscan;
    atomic_t state;
    unsigned int pwe_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rio_mport {
    struct list_head dbells;
    struct list_head pwrites;
    struct list_head node;
    struct list_head nnode;
    struct rio_net *net;
    struct mutex lock;
    struct resource iores;
    struct resource riores[16];
    struct rio_msg inb_msg[4];
    struct rio_msg outb_msg[4];
    int host_deviceid;
    struct rio_ops *ops;
    unsigned char id;
    unsigned char index;
    unsigned int sys_size;
    u32 phys_efptr;
    u32 phys_rmap;
    unsigned char name[40];
    struct device dev;
    void *priv;
    struct dma_device dma;
    struct rio_scan *nscan;
    atomic_t state;
    unsigned int pwe_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rio_mport {
    struct list_head dbells;
    struct list_head pwrites;
    struct list_head node;
    struct list_head nnode;
    struct rio_net *net;
    struct mutex lock;
    struct resource iores;
    struct resource riores[16];
    struct rio_msg inb_msg[4];
    struct rio_msg outb_msg[4];
    int host_deviceid;
    struct rio_ops *ops;
    unsigned char id;
    unsigned char index;
    unsigned int sys_size;
    u32 phys_efptr;
    u32 phys_rmap;
    unsigned char name[40];
    struct device dev;
    void *priv;
    struct dma_device dma;
    struct rio_scan *nscan;
    atomic_t state;
    unsigned int pwe_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rio_mport {
    struct list_head dbells;
    struct list_head pwrites;
    struct list_head node;
    struct list_head nnode;
    struct rio_net *net;
    struct mutex lock;
    struct resource iores;
    struct resource riores[16];
    struct rio_msg inb_msg[4];
    struct rio_msg outb_msg[4];
    int host_deviceid;
    struct rio_ops *ops;
    unsigned char id;
    unsigned char index;
    unsigned int sys_size;
    u32 phys_efptr;
    u32 phys_rmap;
    unsigned char name[40];
    struct device dev;
    void *priv;
    struct dma_device dma;
    struct rio_scan *nscan;
    atomic_t state;
    unsigned int pwe_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct rio_mport {
    struct list_head dbells;
    struct list_head pwrites;
    struct list_head node;
    struct list_head nnode;
    struct rio_net *net;
    struct mutex lock;
    struct resource iores;
    struct resource riores[16];
    struct rio_msg inb_msg[4];
    struct rio_msg outb_msg[4];
    int host_deviceid;
    struct rio_ops *ops;
    unsigned char id;
    unsigned char index;
    unsigned int sys_size;
    u32 phys_efptr;
    u32 phys_rmap;
    unsigned char name[40];
    struct device dev;
    void *priv;
    struct dma_device dma;
    struct rio_scan *nscan;
    atomic_t state;
    unsigned int pwe_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct rio_mport {
    struct list_head dbells;
    struct list_head pwrites;
    struct list_head node;
    struct list_head nnode;
    struct rio_net *net;
    struct mutex lock;
    struct resource iores;
    struct resource riores[16];
    struct rio_msg inb_msg[4];
    struct rio_msg outb_msg[4];
    int host_deviceid;
    struct rio_ops *ops;
    unsigned char id;
    unsigned char index;
    unsigned int sys_size;
    u32 phys_efptr;
    u32 phys_rmap;
    unsigned char name[40];
    struct device dev;
    void *priv;
    struct dma_device dma;
    struct rio_scan *nscan;
    atomic_t state;
    unsigned int pwe_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rio_mport {
    struct list_head dbells;
    struct list_head pwrites;
    struct list_head node;
    struct list_head nnode;
    struct rio_net *net;
    struct mutex lock;
    struct resource iores;
    struct resource riores[16];
    struct rio_msg inb_msg[4];
    struct rio_msg outb_msg[4];
    int host_deviceid;
    struct rio_ops *ops;
    unsigned char id;
    unsigned char index;
    unsigned int sys_size;
    u32 phys_efptr;
    u32 phys_rmap;
    unsigned char name[40];
    struct device dev;
    void *priv;
    struct dma_device dma;
    struct rio_scan *nscan;
    atomic_t state;
    unsigned int pwe_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rio_mport {
    struct list_head dbells;
    struct list_head pwrites;
    struct list_head node;
    struct list_head nnode;
    struct rio_net *net;
    struct mutex lock;
    struct resource iores;
    struct resource riores[16];
    struct rio_msg inb_msg[4];
    struct rio_msg outb_msg[4];
    int host_deviceid;
    struct rio_ops *ops;
    unsigned char id;
    unsigned char index;
    unsigned int sys_size;
    u32 phys_efptr;
    u32 phys_rmap;
    unsigned char name[40];
    struct device dev;
    void *priv;
    struct dma_device dma;
    struct rio_scan *nscan;
    atomic_t state;
    unsigned int pwe_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rio_mport {
    struct list_head dbells;
    struct list_head pwrites;
    struct list_head node;
    struct list_head nnode;
    struct rio_net *net;
    struct mutex lock;
    struct resource iores;
    struct resource riores[16];
    struct rio_msg inb_msg[4];
    struct rio_msg outb_msg[4];
    int host_deviceid;
    struct rio_ops *ops;
    unsigned char id;
    unsigned char index;
    unsigned int sys_size;
    u32 phys_efptr;
    u32 phys_rmap;
    unsigned char name[40];
    struct device dev;
    void *priv;
    struct dma_device dma;
    struct rio_scan *nscan;
    atomic_t state;
    unsigned int pwe_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rio_mport {
    struct list_head dbells;
    struct list_head pwrites;
    struct list_head node;
    struct list_head nnode;
    struct rio_net *net;
    struct mutex lock;
    struct resource iores;
    struct resource riores[16];
    struct rio_msg inb_msg[4];
    struct rio_msg outb_msg[4];
    int host_deviceid;
    struct rio_ops *ops;
    unsigned char id;
    unsigned char index;
    unsigned int sys_size;
    u32 phys_efptr;
    u32 phys_rmap;
    unsigned char name[40];
    struct device dev;
    void *priv;
    struct dma_device dma;
    struct rio_scan *nscan;
    atomic_t state;
    unsigned int pwe_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rio_mport {
    struct list_head dbells;
    struct list_head pwrites;
    struct list_head node;
    struct list_head nnode;
    struct rio_net *net;
    struct mutex lock;
    struct resource iores;
    struct resource riores[16];
    struct rio_msg inb_msg[4];
    struct rio_msg outb_msg[4];
    int host_deviceid;
    struct rio_ops *ops;
    unsigned char id;
    unsigned char index;
    unsigned int sys_size;
    u32 phys_efptr;
    u32 phys_rmap;
    unsigned char name[40];
    struct device dev;
    void *priv;
    struct dma_device dma;
    struct rio_scan *nscan;
    atomic_t state;
    unsigned int pwe_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rio_mport {
    struct list_head dbells;
    struct list_head pwrites;
    struct list_head node;
    struct list_head nnode;
    struct rio_net *net;
    struct mutex lock;
    struct resource iores;
    struct resource riores[16];
    struct rio_msg inb_msg[4];
    struct rio_msg outb_msg[4];
    int host_deviceid;
    struct rio_ops *ops;
    unsigned char id;
    unsigned char index;
    unsigned int sys_size;
    u32 phys_efptr;
    u32 phys_rmap;
    unsigned char name[40];
    struct device dev;
    void *priv;
    struct dma_device dma;
    struct rio_scan *nscan;
    atomic_t state;
    unsigned int pwe_refcnt;
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
struct rio_mport {
    struct list_head dbells;
    struct list_head pwrites;
    struct list_head node;
    struct list_head nnode;
    struct rio_net *net;
    struct mutex lock;
    struct resource iores;
    struct resource riores[16];
    struct rio_msg inb_msg[4];
    struct rio_msg outb_msg[4];
    int host_deviceid;
    struct rio_ops *ops;
    unsigned char id;
    unsigned char index;
    unsigned int sys_size;
    u32 phys_efptr;
    u32 phys_rmap;
    unsigned char name[40];
    struct device dev;
    void *priv;
    struct dma_device dma;
    struct rio_scan *nscan;
    atomic_t state;
    unsigned int pwe_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rio_mport {
    struct list_head dbells;
    struct list_head pwrites;
    struct list_head node;
    struct list_head nnode;
    struct rio_net *net;
    struct mutex lock;
    struct resource iores;
    struct resource riores[16];
    struct rio_msg inb_msg[4];
    struct rio_msg outb_msg[4];
    int host_deviceid;
    struct rio_ops *ops;
    unsigned char id;
    unsigned char index;
    unsigned int sys_size;
    u32 phys_efptr;
    u32 phys_rmap;
    unsigned char name[40];
    struct device dev;
    void *priv;
    struct dma_device dma;
    struct rio_scan *nscan;
    atomic_t state;
    unsigned int pwe_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rio_mport {
    struct list_head dbells;
    struct list_head pwrites;
    struct list_head node;
    struct list_head nnode;
    struct rio_net *net;
    struct mutex lock;
    struct resource iores;
    struct resource riores[16];
    struct rio_msg inb_msg[4];
    struct rio_msg outb_msg[4];
    int host_deviceid;
    struct rio_ops *ops;
    unsigned char id;
    unsigned char index;
    unsigned int sys_size;
    u32 phys_efptr;
    u32 phys_rmap;
    unsigned char name[40];
    struct device dev;
    void *priv;
    struct dma_device dma;
    struct rio_scan *nscan;
    atomic_t state;
    unsigned int pwe_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct rio_mport {
    struct list_head dbells;
    struct list_head pwrites;
    struct list_head node;
    struct list_head nnode;
    struct rio_net *net;
    struct mutex lock;
    struct resource iores;
    struct resource riores[16];
    struct rio_msg inb_msg[4];
    struct rio_msg outb_msg[4];
    int host_deviceid;
    struct rio_ops *ops;
    unsigned char id;
    unsigned char index;
    unsigned int sys_size;
    u32 phys_efptr;
    u32 phys_rmap;
    unsigned char name[40];
    struct device dev;
    void *priv;
    struct dma_device dma;
    struct rio_scan *nscan;
    atomic_t state;
    unsigned int pwe_refcnt;
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
struct rio_mport {
    struct list_head dbells;
    struct list_head pwrites;
    struct list_head node;
    struct list_head nnode;
    struct rio_net *net;
    struct mutex lock;
    struct resource iores;
    struct resource riores[16];
    struct rio_msg inb_msg[4];
    struct rio_msg outb_msg[4];
    int host_deviceid;
    struct rio_ops *ops;
    unsigned char id;
    unsigned char index;
    unsigned int sys_size;
    u32 phys_efptr;
    u32 phys_rmap;
    unsigned char name[40];
    struct device dev;
    void *priv;
    struct dma_device dma;
    struct rio_scan *nscan;
    atomic_t state;
    unsigned int pwe_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rio_mport {
    struct list_head dbells;
    struct list_head pwrites;
    struct list_head node;
    struct list_head nnode;
    struct rio_net *net;
    struct mutex lock;
    struct resource iores;
    struct resource riores[16];
    struct rio_msg inb_msg[4];
    struct rio_msg outb_msg[4];
    int host_deviceid;
    struct rio_ops *ops;
    unsigned char id;
    unsigned char index;
    unsigned int sys_size;
    u32 phys_efptr;
    u32 phys_rmap;
    unsigned char name[40];
    struct device dev;
    void *priv;
    struct dma_device dma;
    struct rio_scan *nscan;
    atomic_t state;
    unsigned int pwe_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rio_mport {
    struct list_head dbells;
    struct list_head pwrites;
    struct list_head node;
    struct list_head nnode;
    struct rio_net *net;
    struct mutex lock;
    struct resource iores;
    struct resource riores[16];
    struct rio_msg inb_msg[4];
    struct rio_msg outb_msg[4];
    int host_deviceid;
    struct rio_ops *ops;
    unsigned char id;
    unsigned char index;
    unsigned int sys_size;
    u32 phys_efptr;
    u32 phys_rmap;
    unsigned char name[40];
    struct device dev;
    void *priv;
    struct dma_device dma;
    struct rio_scan *nscan;
    atomic_t state;
    unsigned int pwe_refcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rio_mport {
    struct list_head dbells;
    struct list_head pwrites;
    struct list_head node;
    struct list_head nnode;
    struct rio_net *net;
    struct mutex lock;
    struct resource iores;
    struct resource riores[16];
    struct rio_msg inb_msg[4];
    struct rio_msg outb_msg[4];
    int host_deviceid;
    struct rio_ops *ops;
    unsigned char id;
    unsigned char index;
    unsigned int sys_size;
    u32 phys_efptr;
    u32 phys_rmap;
    unsigned char name[40];
    struct device dev;
    void *priv;
    struct dma_device dma;
    struct rio_scan *nscan;
    atomic_t state;
    unsigned int pwe_refcnt;
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
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head pwrites</code>
</li>
<li>
<b>Field added. </b>
<code>struct rio_net *net</code>
</li>
<li>
<b>Field added. </b>
<code>struct mutex lock</code>
</li>
<li>
<b>Field added. </b>
<code>u32 phys_rmap</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t state</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int pwe_refcnt</code>
</li>
<li>
<b>Field removed. </b>
<code>enum rio_phy_type phy_type</code>
</li>
</ul>
</details>
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
