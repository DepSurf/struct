# Struct: <code>vme_bridge</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct vme_bridge {
    char name[16];
    int num;
    struct list_head master_resources;
    struct list_head slave_resources;
    struct list_head dma_resources;
    struct list_head lm_resources;
    struct list_head vme_error_handlers;
    struct list_head devices;
    struct device *parent;
    void *driver_priv;
    struct list_head bus_list;
    struct vme_irq irq[7];
    struct mutex irq_mtx;
    int (*slave_get)(struct vme_slave_resource *, int *, long long unsigned int *, long long unsigned int *, dma_addr_t *, u32 *, u32 *);
    int (*slave_set)(struct vme_slave_resource *, int, long long unsigned int, long long unsigned int, dma_addr_t, u32, u32);
    int (*master_get)(struct vme_master_resource *, int *, long long unsigned int *, long long unsigned int *, u32 *, u32 *, u32 *);
    int (*master_set)(struct vme_master_resource *, int, long long unsigned int, long long unsigned int, u32, u32, u32);
    ssize_t (*master_read)(struct vme_master_resource *, void *, size_t, loff_t);
    ssize_t (*master_write)(struct vme_master_resource *, void *, size_t, loff_t);
    unsigned int (*master_rmw)(struct vme_master_resource *, unsigned int, unsigned int, unsigned int, loff_t);
    int (*dma_list_add)(struct vme_dma_list *, struct vme_dma_attr *, struct vme_dma_attr *, size_t);
    int (*dma_list_exec)(struct vme_dma_list *);
    int (*dma_list_empty)(struct vme_dma_list *);
    void (*irq_set)(struct vme_bridge *, int, int, int);
    int (*irq_generate)(struct vme_bridge *, int, int);
    int (*lm_set)(struct vme_lm_resource *, long long unsigned int, u32, u32);
    int (*lm_get)(struct vme_lm_resource *, long long unsigned int *, u32 *, u32 *);
    int (*lm_attach)(struct vme_lm_resource *, int, void(*)(int));
    int (*lm_detach)(struct vme_lm_resource *, int);
    int (*slot_get)(struct vme_bridge *);
    void * (*alloc_consistent)(struct device *, size_t, dma_addr_t *);
    void (*free_consistent)(struct device *, size_t, void *, dma_addr_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct vme_bridge {
    char name[16];
    int num;
    struct list_head master_resources;
    struct list_head slave_resources;
    struct list_head dma_resources;
    struct list_head lm_resources;
    struct list_head vme_error_handlers;
    struct list_head devices;
    struct device *parent;
    void *driver_priv;
    struct list_head bus_list;
    struct vme_irq irq[7];
    struct mutex irq_mtx;
    int (*slave_get)(struct vme_slave_resource *, int *, long long unsigned int *, long long unsigned int *, dma_addr_t *, u32 *, u32 *);
    int (*slave_set)(struct vme_slave_resource *, int, long long unsigned int, long long unsigned int, dma_addr_t, u32, u32);
    int (*master_get)(struct vme_master_resource *, int *, long long unsigned int *, long long unsigned int *, u32 *, u32 *, u32 *);
    int (*master_set)(struct vme_master_resource *, int, long long unsigned int, long long unsigned int, u32, u32, u32);
    ssize_t (*master_read)(struct vme_master_resource *, void *, size_t, loff_t);
    ssize_t (*master_write)(struct vme_master_resource *, void *, size_t, loff_t);
    unsigned int (*master_rmw)(struct vme_master_resource *, unsigned int, unsigned int, unsigned int, loff_t);
    int (*dma_list_add)(struct vme_dma_list *, struct vme_dma_attr *, struct vme_dma_attr *, size_t);
    int (*dma_list_exec)(struct vme_dma_list *);
    int (*dma_list_empty)(struct vme_dma_list *);
    void (*irq_set)(struct vme_bridge *, int, int, int);
    int (*irq_generate)(struct vme_bridge *, int, int);
    int (*lm_set)(struct vme_lm_resource *, long long unsigned int, u32, u32);
    int (*lm_get)(struct vme_lm_resource *, long long unsigned int *, u32 *, u32 *);
    int (*lm_attach)(struct vme_lm_resource *, int, void(*)(int));
    int (*lm_detach)(struct vme_lm_resource *, int);
    int (*slot_get)(struct vme_bridge *);
    void * (*alloc_consistent)(struct device *, size_t, dma_addr_t *);
    void (*free_consistent)(struct device *, size_t, void *, dma_addr_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct vme_bridge {
    char name[16];
    int num;
    struct list_head master_resources;
    struct list_head slave_resources;
    struct list_head dma_resources;
    struct list_head lm_resources;
    struct list_head vme_error_handlers;
    struct list_head devices;
    struct device *parent;
    void *driver_priv;
    struct list_head bus_list;
    struct vme_irq irq[7];
    struct mutex irq_mtx;
    int (*slave_get)(struct vme_slave_resource *, int *, long long unsigned int *, long long unsigned int *, dma_addr_t *, u32 *, u32 *);
    int (*slave_set)(struct vme_slave_resource *, int, long long unsigned int, long long unsigned int, dma_addr_t, u32, u32);
    int (*master_get)(struct vme_master_resource *, int *, long long unsigned int *, long long unsigned int *, u32 *, u32 *, u32 *);
    int (*master_set)(struct vme_master_resource *, int, long long unsigned int, long long unsigned int, u32, u32, u32);
    ssize_t (*master_read)(struct vme_master_resource *, void *, size_t, loff_t);
    ssize_t (*master_write)(struct vme_master_resource *, void *, size_t, loff_t);
    unsigned int (*master_rmw)(struct vme_master_resource *, unsigned int, unsigned int, unsigned int, loff_t);
    int (*dma_list_add)(struct vme_dma_list *, struct vme_dma_attr *, struct vme_dma_attr *, size_t);
    int (*dma_list_exec)(struct vme_dma_list *);
    int (*dma_list_empty)(struct vme_dma_list *);
    void (*irq_set)(struct vme_bridge *, int, int, int);
    int (*irq_generate)(struct vme_bridge *, int, int);
    int (*lm_set)(struct vme_lm_resource *, long long unsigned int, u32, u32);
    int (*lm_get)(struct vme_lm_resource *, long long unsigned int *, u32 *, u32 *);
    int (*lm_attach)(struct vme_lm_resource *, int, void(*)(void *), void *);
    int (*lm_detach)(struct vme_lm_resource *, int);
    int (*slot_get)(struct vme_bridge *);
    void * (*alloc_consistent)(struct device *, size_t, dma_addr_t *);
    void (*free_consistent)(struct device *, size_t, void *, dma_addr_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct vme_bridge {
    char name[16];
    int num;
    struct list_head master_resources;
    struct list_head slave_resources;
    struct list_head dma_resources;
    struct list_head lm_resources;
    struct list_head vme_error_handlers;
    struct list_head devices;
    struct device *parent;
    void *driver_priv;
    struct list_head bus_list;
    struct vme_irq irq[7];
    struct mutex irq_mtx;
    int (*slave_get)(struct vme_slave_resource *, int *, long long unsigned int *, long long unsigned int *, dma_addr_t *, u32 *, u32 *);
    int (*slave_set)(struct vme_slave_resource *, int, long long unsigned int, long long unsigned int, dma_addr_t, u32, u32);
    int (*master_get)(struct vme_master_resource *, int *, long long unsigned int *, long long unsigned int *, u32 *, u32 *, u32 *);
    int (*master_set)(struct vme_master_resource *, int, long long unsigned int, long long unsigned int, u32, u32, u32);
    ssize_t (*master_read)(struct vme_master_resource *, void *, size_t, loff_t);
    ssize_t (*master_write)(struct vme_master_resource *, void *, size_t, loff_t);
    unsigned int (*master_rmw)(struct vme_master_resource *, unsigned int, unsigned int, unsigned int, loff_t);
    int (*dma_list_add)(struct vme_dma_list *, struct vme_dma_attr *, struct vme_dma_attr *, size_t);
    int (*dma_list_exec)(struct vme_dma_list *);
    int (*dma_list_empty)(struct vme_dma_list *);
    void (*irq_set)(struct vme_bridge *, int, int, int);
    int (*irq_generate)(struct vme_bridge *, int, int);
    int (*lm_set)(struct vme_lm_resource *, long long unsigned int, u32, u32);
    int (*lm_get)(struct vme_lm_resource *, long long unsigned int *, u32 *, u32 *);
    int (*lm_attach)(struct vme_lm_resource *, int, void(*)(void *), void *);
    int (*lm_detach)(struct vme_lm_resource *, int);
    int (*slot_get)(struct vme_bridge *);
    void * (*alloc_consistent)(struct device *, size_t, dma_addr_t *);
    void (*free_consistent)(struct device *, size_t, void *, dma_addr_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct vme_bridge {
    char name[16];
    int num;
    struct list_head master_resources;
    struct list_head slave_resources;
    struct list_head dma_resources;
    struct list_head lm_resources;
    struct list_head vme_error_handlers;
    struct list_head devices;
    struct device *parent;
    void *driver_priv;
    struct list_head bus_list;
    struct vme_irq irq[7];
    struct mutex irq_mtx;
    int (*slave_get)(struct vme_slave_resource *, int *, long long unsigned int *, long long unsigned int *, dma_addr_t *, u32 *, u32 *);
    int (*slave_set)(struct vme_slave_resource *, int, long long unsigned int, long long unsigned int, dma_addr_t, u32, u32);
    int (*master_get)(struct vme_master_resource *, int *, long long unsigned int *, long long unsigned int *, u32 *, u32 *, u32 *);
    int (*master_set)(struct vme_master_resource *, int, long long unsigned int, long long unsigned int, u32, u32, u32);
    ssize_t (*master_read)(struct vme_master_resource *, void *, size_t, loff_t);
    ssize_t (*master_write)(struct vme_master_resource *, void *, size_t, loff_t);
    unsigned int (*master_rmw)(struct vme_master_resource *, unsigned int, unsigned int, unsigned int, loff_t);
    int (*dma_list_add)(struct vme_dma_list *, struct vme_dma_attr *, struct vme_dma_attr *, size_t);
    int (*dma_list_exec)(struct vme_dma_list *);
    int (*dma_list_empty)(struct vme_dma_list *);
    void (*irq_set)(struct vme_bridge *, int, int, int);
    int (*irq_generate)(struct vme_bridge *, int, int);
    int (*lm_set)(struct vme_lm_resource *, long long unsigned int, u32, u32);
    int (*lm_get)(struct vme_lm_resource *, long long unsigned int *, u32 *, u32 *);
    int (*lm_attach)(struct vme_lm_resource *, int, void(*)(void *), void *);
    int (*lm_detach)(struct vme_lm_resource *, int);
    int (*slot_get)(struct vme_bridge *);
    void * (*alloc_consistent)(struct device *, size_t, dma_addr_t *);
    void (*free_consistent)(struct device *, size_t, void *, dma_addr_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct vme_bridge {
    char name[16];
    int num;
    struct list_head master_resources;
    struct list_head slave_resources;
    struct list_head dma_resources;
    struct list_head lm_resources;
    struct list_head vme_error_handlers;
    struct list_head devices;
    struct device *parent;
    void *driver_priv;
    struct list_head bus_list;
    struct vme_irq irq[7];
    struct mutex irq_mtx;
    int (*slave_get)(struct vme_slave_resource *, int *, long long unsigned int *, long long unsigned int *, dma_addr_t *, u32 *, u32 *);
    int (*slave_set)(struct vme_slave_resource *, int, long long unsigned int, long long unsigned int, dma_addr_t, u32, u32);
    int (*master_get)(struct vme_master_resource *, int *, long long unsigned int *, long long unsigned int *, u32 *, u32 *, u32 *);
    int (*master_set)(struct vme_master_resource *, int, long long unsigned int, long long unsigned int, u32, u32, u32);
    ssize_t (*master_read)(struct vme_master_resource *, void *, size_t, loff_t);
    ssize_t (*master_write)(struct vme_master_resource *, void *, size_t, loff_t);
    unsigned int (*master_rmw)(struct vme_master_resource *, unsigned int, unsigned int, unsigned int, loff_t);
    int (*dma_list_add)(struct vme_dma_list *, struct vme_dma_attr *, struct vme_dma_attr *, size_t);
    int (*dma_list_exec)(struct vme_dma_list *);
    int (*dma_list_empty)(struct vme_dma_list *);
    void (*irq_set)(struct vme_bridge *, int, int, int);
    int (*irq_generate)(struct vme_bridge *, int, int);
    int (*lm_set)(struct vme_lm_resource *, long long unsigned int, u32, u32);
    int (*lm_get)(struct vme_lm_resource *, long long unsigned int *, u32 *, u32 *);
    int (*lm_attach)(struct vme_lm_resource *, int, void(*)(void *), void *);
    int (*lm_detach)(struct vme_lm_resource *, int);
    int (*slot_get)(struct vme_bridge *);
    void * (*alloc_consistent)(struct device *, size_t, dma_addr_t *);
    void (*free_consistent)(struct device *, size_t, void *, dma_addr_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct vme_bridge {
    char name[16];
    int num;
    struct list_head master_resources;
    struct list_head slave_resources;
    struct list_head dma_resources;
    struct list_head lm_resources;
    struct list_head vme_error_handlers;
    struct list_head devices;
    struct device *parent;
    void *driver_priv;
    struct list_head bus_list;
    struct vme_irq irq[7];
    struct mutex irq_mtx;
    int (*slave_get)(struct vme_slave_resource *, int *, long long unsigned int *, long long unsigned int *, dma_addr_t *, u32 *, u32 *);
    int (*slave_set)(struct vme_slave_resource *, int, long long unsigned int, long long unsigned int, dma_addr_t, u32, u32);
    int (*master_get)(struct vme_master_resource *, int *, long long unsigned int *, long long unsigned int *, u32 *, u32 *, u32 *);
    int (*master_set)(struct vme_master_resource *, int, long long unsigned int, long long unsigned int, u32, u32, u32);
    ssize_t (*master_read)(struct vme_master_resource *, void *, size_t, loff_t);
    ssize_t (*master_write)(struct vme_master_resource *, void *, size_t, loff_t);
    unsigned int (*master_rmw)(struct vme_master_resource *, unsigned int, unsigned int, unsigned int, loff_t);
    int (*dma_list_add)(struct vme_dma_list *, struct vme_dma_attr *, struct vme_dma_attr *, size_t);
    int (*dma_list_exec)(struct vme_dma_list *);
    int (*dma_list_empty)(struct vme_dma_list *);
    void (*irq_set)(struct vme_bridge *, int, int, int);
    int (*irq_generate)(struct vme_bridge *, int, int);
    int (*lm_set)(struct vme_lm_resource *, long long unsigned int, u32, u32);
    int (*lm_get)(struct vme_lm_resource *, long long unsigned int *, u32 *, u32 *);
    int (*lm_attach)(struct vme_lm_resource *, int, void(*)(void *), void *);
    int (*lm_detach)(struct vme_lm_resource *, int);
    int (*slot_get)(struct vme_bridge *);
    void * (*alloc_consistent)(struct device *, size_t, dma_addr_t *);
    void (*free_consistent)(struct device *, size_t, void *, dma_addr_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct vme_bridge {
    char name[16];
    int num;
    struct list_head master_resources;
    struct list_head slave_resources;
    struct list_head dma_resources;
    struct list_head lm_resources;
    struct list_head vme_error_handlers;
    struct list_head devices;
    struct device *parent;
    void *driver_priv;
    struct list_head bus_list;
    struct vme_irq irq[7];
    struct mutex irq_mtx;
    int (*slave_get)(struct vme_slave_resource *, int *, long long unsigned int *, long long unsigned int *, dma_addr_t *, u32 *, u32 *);
    int (*slave_set)(struct vme_slave_resource *, int, long long unsigned int, long long unsigned int, dma_addr_t, u32, u32);
    int (*master_get)(struct vme_master_resource *, int *, long long unsigned int *, long long unsigned int *, u32 *, u32 *, u32 *);
    int (*master_set)(struct vme_master_resource *, int, long long unsigned int, long long unsigned int, u32, u32, u32);
    ssize_t (*master_read)(struct vme_master_resource *, void *, size_t, loff_t);
    ssize_t (*master_write)(struct vme_master_resource *, void *, size_t, loff_t);
    unsigned int (*master_rmw)(struct vme_master_resource *, unsigned int, unsigned int, unsigned int, loff_t);
    int (*dma_list_add)(struct vme_dma_list *, struct vme_dma_attr *, struct vme_dma_attr *, size_t);
    int (*dma_list_exec)(struct vme_dma_list *);
    int (*dma_list_empty)(struct vme_dma_list *);
    void (*irq_set)(struct vme_bridge *, int, int, int);
    int (*irq_generate)(struct vme_bridge *, int, int);
    int (*lm_set)(struct vme_lm_resource *, long long unsigned int, u32, u32);
    int (*lm_get)(struct vme_lm_resource *, long long unsigned int *, u32 *, u32 *);
    int (*lm_attach)(struct vme_lm_resource *, int, void(*)(void *), void *);
    int (*lm_detach)(struct vme_lm_resource *, int);
    int (*slot_get)(struct vme_bridge *);
    void * (*alloc_consistent)(struct device *, size_t, dma_addr_t *);
    void (*free_consistent)(struct device *, size_t, void *, dma_addr_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct vme_bridge {
    char name[16];
    int num;
    struct list_head master_resources;
    struct list_head slave_resources;
    struct list_head dma_resources;
    struct list_head lm_resources;
    struct list_head vme_error_handlers;
    struct list_head devices;
    struct device *parent;
    void *driver_priv;
    struct list_head bus_list;
    struct vme_irq irq[7];
    struct mutex irq_mtx;
    int (*slave_get)(struct vme_slave_resource *, int *, long long unsigned int *, long long unsigned int *, dma_addr_t *, u32 *, u32 *);
    int (*slave_set)(struct vme_slave_resource *, int, long long unsigned int, long long unsigned int, dma_addr_t, u32, u32);
    int (*master_get)(struct vme_master_resource *, int *, long long unsigned int *, long long unsigned int *, u32 *, u32 *, u32 *);
    int (*master_set)(struct vme_master_resource *, int, long long unsigned int, long long unsigned int, u32, u32, u32);
    ssize_t (*master_read)(struct vme_master_resource *, void *, size_t, loff_t);
    ssize_t (*master_write)(struct vme_master_resource *, void *, size_t, loff_t);
    unsigned int (*master_rmw)(struct vme_master_resource *, unsigned int, unsigned int, unsigned int, loff_t);
    int (*dma_list_add)(struct vme_dma_list *, struct vme_dma_attr *, struct vme_dma_attr *, size_t);
    int (*dma_list_exec)(struct vme_dma_list *);
    int (*dma_list_empty)(struct vme_dma_list *);
    void (*irq_set)(struct vme_bridge *, int, int, int);
    int (*irq_generate)(struct vme_bridge *, int, int);
    int (*lm_set)(struct vme_lm_resource *, long long unsigned int, u32, u32);
    int (*lm_get)(struct vme_lm_resource *, long long unsigned int *, u32 *, u32 *);
    int (*lm_attach)(struct vme_lm_resource *, int, void(*)(void *), void *);
    int (*lm_detach)(struct vme_lm_resource *, int);
    int (*slot_get)(struct vme_bridge *);
    void * (*alloc_consistent)(struct device *, size_t, dma_addr_t *);
    void (*free_consistent)(struct device *, size_t, void *, dma_addr_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct vme_bridge {
    char name[16];
    int num;
    struct list_head master_resources;
    struct list_head slave_resources;
    struct list_head dma_resources;
    struct list_head lm_resources;
    struct list_head vme_error_handlers;
    struct list_head devices;
    struct device *parent;
    void *driver_priv;
    struct list_head bus_list;
    struct vme_irq irq[7];
    struct mutex irq_mtx;
    int (*slave_get)(struct vme_slave_resource *, int *, long long unsigned int *, long long unsigned int *, dma_addr_t *, u32 *, u32 *);
    int (*slave_set)(struct vme_slave_resource *, int, long long unsigned int, long long unsigned int, dma_addr_t, u32, u32);
    int (*master_get)(struct vme_master_resource *, int *, long long unsigned int *, long long unsigned int *, u32 *, u32 *, u32 *);
    int (*master_set)(struct vme_master_resource *, int, long long unsigned int, long long unsigned int, u32, u32, u32);
    ssize_t (*master_read)(struct vme_master_resource *, void *, size_t, loff_t);
    ssize_t (*master_write)(struct vme_master_resource *, void *, size_t, loff_t);
    unsigned int (*master_rmw)(struct vme_master_resource *, unsigned int, unsigned int, unsigned int, loff_t);
    int (*dma_list_add)(struct vme_dma_list *, struct vme_dma_attr *, struct vme_dma_attr *, size_t);
    int (*dma_list_exec)(struct vme_dma_list *);
    int (*dma_list_empty)(struct vme_dma_list *);
    void (*irq_set)(struct vme_bridge *, int, int, int);
    int (*irq_generate)(struct vme_bridge *, int, int);
    int (*lm_set)(struct vme_lm_resource *, long long unsigned int, u32, u32);
    int (*lm_get)(struct vme_lm_resource *, long long unsigned int *, u32 *, u32 *);
    int (*lm_attach)(struct vme_lm_resource *, int, void(*)(void *), void *);
    int (*lm_detach)(struct vme_lm_resource *, int);
    int (*slot_get)(struct vme_bridge *);
    void * (*alloc_consistent)(struct device *, size_t, dma_addr_t *);
    void (*free_consistent)(struct device *, size_t, void *, dma_addr_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct vme_bridge {
    char name[16];
    int num;
    struct list_head master_resources;
    struct list_head slave_resources;
    struct list_head dma_resources;
    struct list_head lm_resources;
    struct list_head vme_error_handlers;
    struct list_head devices;
    struct device *parent;
    void *driver_priv;
    struct list_head bus_list;
    struct vme_irq irq[7];
    struct mutex irq_mtx;
    int (*slave_get)(struct vme_slave_resource *, int *, long long unsigned int *, long long unsigned int *, dma_addr_t *, u32 *, u32 *);
    int (*slave_set)(struct vme_slave_resource *, int, long long unsigned int, long long unsigned int, dma_addr_t, u32, u32);
    int (*master_get)(struct vme_master_resource *, int *, long long unsigned int *, long long unsigned int *, u32 *, u32 *, u32 *);
    int (*master_set)(struct vme_master_resource *, int, long long unsigned int, long long unsigned int, u32, u32, u32);
    ssize_t (*master_read)(struct vme_master_resource *, void *, size_t, loff_t);
    ssize_t (*master_write)(struct vme_master_resource *, void *, size_t, loff_t);
    unsigned int (*master_rmw)(struct vme_master_resource *, unsigned int, unsigned int, unsigned int, loff_t);
    int (*dma_list_add)(struct vme_dma_list *, struct vme_dma_attr *, struct vme_dma_attr *, size_t);
    int (*dma_list_exec)(struct vme_dma_list *);
    int (*dma_list_empty)(struct vme_dma_list *);
    void (*irq_set)(struct vme_bridge *, int, int, int);
    int (*irq_generate)(struct vme_bridge *, int, int);
    int (*lm_set)(struct vme_lm_resource *, long long unsigned int, u32, u32);
    int (*lm_get)(struct vme_lm_resource *, long long unsigned int *, u32 *, u32 *);
    int (*lm_attach)(struct vme_lm_resource *, int, void(*)(void *), void *);
    int (*lm_detach)(struct vme_lm_resource *, int);
    int (*slot_get)(struct vme_bridge *);
    void * (*alloc_consistent)(struct device *, size_t, dma_addr_t *);
    void (*free_consistent)(struct device *, size_t, void *, dma_addr_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct vme_bridge {
    char name[16];
    int num;
    struct list_head master_resources;
    struct list_head slave_resources;
    struct list_head dma_resources;
    struct list_head lm_resources;
    struct list_head vme_error_handlers;
    struct list_head devices;
    struct device *parent;
    void *driver_priv;
    struct list_head bus_list;
    struct vme_irq irq[7];
    struct mutex irq_mtx;
    int (*slave_get)(struct vme_slave_resource *, int *, long long unsigned int *, long long unsigned int *, dma_addr_t *, u32 *, u32 *);
    int (*slave_set)(struct vme_slave_resource *, int, long long unsigned int, long long unsigned int, dma_addr_t, u32, u32);
    int (*master_get)(struct vme_master_resource *, int *, long long unsigned int *, long long unsigned int *, u32 *, u32 *, u32 *);
    int (*master_set)(struct vme_master_resource *, int, long long unsigned int, long long unsigned int, u32, u32, u32);
    ssize_t (*master_read)(struct vme_master_resource *, void *, size_t, loff_t);
    ssize_t (*master_write)(struct vme_master_resource *, void *, size_t, loff_t);
    unsigned int (*master_rmw)(struct vme_master_resource *, unsigned int, unsigned int, unsigned int, loff_t);
    int (*dma_list_add)(struct vme_dma_list *, struct vme_dma_attr *, struct vme_dma_attr *, size_t);
    int (*dma_list_exec)(struct vme_dma_list *);
    int (*dma_list_empty)(struct vme_dma_list *);
    void (*irq_set)(struct vme_bridge *, int, int, int);
    int (*irq_generate)(struct vme_bridge *, int, int);
    int (*lm_set)(struct vme_lm_resource *, long long unsigned int, u32, u32);
    int (*lm_get)(struct vme_lm_resource *, long long unsigned int *, u32 *, u32 *);
    int (*lm_attach)(struct vme_lm_resource *, int, void(*)(void *), void *);
    int (*lm_detach)(struct vme_lm_resource *, int);
    int (*slot_get)(struct vme_bridge *);
    void * (*alloc_consistent)(struct device *, size_t, dma_addr_t *);
    void (*free_consistent)(struct device *, size_t, void *, dma_addr_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct vme_bridge {
    char name[16];
    int num;
    struct list_head master_resources;
    struct list_head slave_resources;
    struct list_head dma_resources;
    struct list_head lm_resources;
    struct list_head vme_error_handlers;
    struct list_head devices;
    struct device *parent;
    void *driver_priv;
    struct list_head bus_list;
    struct vme_irq irq[7];
    struct mutex irq_mtx;
    int (*slave_get)(struct vme_slave_resource *, int *, long long unsigned int *, long long unsigned int *, dma_addr_t *, u32 *, u32 *);
    int (*slave_set)(struct vme_slave_resource *, int, long long unsigned int, long long unsigned int, dma_addr_t, u32, u32);
    int (*master_get)(struct vme_master_resource *, int *, long long unsigned int *, long long unsigned int *, u32 *, u32 *, u32 *);
    int (*master_set)(struct vme_master_resource *, int, long long unsigned int, long long unsigned int, u32, u32, u32);
    ssize_t (*master_read)(struct vme_master_resource *, void *, size_t, loff_t);
    ssize_t (*master_write)(struct vme_master_resource *, void *, size_t, loff_t);
    unsigned int (*master_rmw)(struct vme_master_resource *, unsigned int, unsigned int, unsigned int, loff_t);
    int (*dma_list_add)(struct vme_dma_list *, struct vme_dma_attr *, struct vme_dma_attr *, size_t);
    int (*dma_list_exec)(struct vme_dma_list *);
    int (*dma_list_empty)(struct vme_dma_list *);
    void (*irq_set)(struct vme_bridge *, int, int, int);
    int (*irq_generate)(struct vme_bridge *, int, int);
    int (*lm_set)(struct vme_lm_resource *, long long unsigned int, u32, u32);
    int (*lm_get)(struct vme_lm_resource *, long long unsigned int *, u32 *, u32 *);
    int (*lm_attach)(struct vme_lm_resource *, int, void(*)(void *), void *);
    int (*lm_detach)(struct vme_lm_resource *, int);
    int (*slot_get)(struct vme_bridge *);
    void * (*alloc_consistent)(struct device *, size_t, dma_addr_t *);
    void (*free_consistent)(struct device *, size_t, void *, dma_addr_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct vme_bridge {
    char name[16];
    int num;
    struct list_head master_resources;
    struct list_head slave_resources;
    struct list_head dma_resources;
    struct list_head lm_resources;
    struct list_head vme_error_handlers;
    struct list_head devices;
    struct device *parent;
    void *driver_priv;
    struct list_head bus_list;
    struct vme_irq irq[7];
    struct mutex irq_mtx;
    int (*slave_get)(struct vme_slave_resource *, int *, long long unsigned int *, long long unsigned int *, dma_addr_t *, u32 *, u32 *);
    int (*slave_set)(struct vme_slave_resource *, int, long long unsigned int, long long unsigned int, dma_addr_t, u32, u32);
    int (*master_get)(struct vme_master_resource *, int *, long long unsigned int *, long long unsigned int *, u32 *, u32 *, u32 *);
    int (*master_set)(struct vme_master_resource *, int, long long unsigned int, long long unsigned int, u32, u32, u32);
    ssize_t (*master_read)(struct vme_master_resource *, void *, size_t, loff_t);
    ssize_t (*master_write)(struct vme_master_resource *, void *, size_t, loff_t);
    unsigned int (*master_rmw)(struct vme_master_resource *, unsigned int, unsigned int, unsigned int, loff_t);
    int (*dma_list_add)(struct vme_dma_list *, struct vme_dma_attr *, struct vme_dma_attr *, size_t);
    int (*dma_list_exec)(struct vme_dma_list *);
    int (*dma_list_empty)(struct vme_dma_list *);
    void (*irq_set)(struct vme_bridge *, int, int, int);
    int (*irq_generate)(struct vme_bridge *, int, int);
    int (*lm_set)(struct vme_lm_resource *, long long unsigned int, u32, u32);
    int (*lm_get)(struct vme_lm_resource *, long long unsigned int *, u32 *, u32 *);
    int (*lm_attach)(struct vme_lm_resource *, int, void(*)(void *), void *);
    int (*lm_detach)(struct vme_lm_resource *, int);
    int (*slot_get)(struct vme_bridge *);
    void * (*alloc_consistent)(struct device *, size_t, dma_addr_t *);
    void (*free_consistent)(struct device *, size_t, void *, dma_addr_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct vme_bridge {
    char name[16];
    int num;
    struct list_head master_resources;
    struct list_head slave_resources;
    struct list_head dma_resources;
    struct list_head lm_resources;
    struct list_head vme_error_handlers;
    struct list_head devices;
    struct device *parent;
    void *driver_priv;
    struct list_head bus_list;
    struct vme_irq irq[7];
    struct mutex irq_mtx;
    int (*slave_get)(struct vme_slave_resource *, int *, long long unsigned int *, long long unsigned int *, dma_addr_t *, u32 *, u32 *);
    int (*slave_set)(struct vme_slave_resource *, int, long long unsigned int, long long unsigned int, dma_addr_t, u32, u32);
    int (*master_get)(struct vme_master_resource *, int *, long long unsigned int *, long long unsigned int *, u32 *, u32 *, u32 *);
    int (*master_set)(struct vme_master_resource *, int, long long unsigned int, long long unsigned int, u32, u32, u32);
    ssize_t (*master_read)(struct vme_master_resource *, void *, size_t, loff_t);
    ssize_t (*master_write)(struct vme_master_resource *, void *, size_t, loff_t);
    unsigned int (*master_rmw)(struct vme_master_resource *, unsigned int, unsigned int, unsigned int, loff_t);
    int (*dma_list_add)(struct vme_dma_list *, struct vme_dma_attr *, struct vme_dma_attr *, size_t);
    int (*dma_list_exec)(struct vme_dma_list *);
    int (*dma_list_empty)(struct vme_dma_list *);
    void (*irq_set)(struct vme_bridge *, int, int, int);
    int (*irq_generate)(struct vme_bridge *, int, int);
    int (*lm_set)(struct vme_lm_resource *, long long unsigned int, u32, u32);
    int (*lm_get)(struct vme_lm_resource *, long long unsigned int *, u32 *, u32 *);
    int (*lm_attach)(struct vme_lm_resource *, int, void(*)(void *), void *);
    int (*lm_detach)(struct vme_lm_resource *, int);
    int (*slot_get)(struct vme_bridge *);
    void * (*alloc_consistent)(struct device *, size_t, dma_addr_t *);
    void (*free_consistent)(struct device *, size_t, void *, dma_addr_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct vme_bridge {
    char name[16];
    int num;
    struct list_head master_resources;
    struct list_head slave_resources;
    struct list_head dma_resources;
    struct list_head lm_resources;
    struct list_head vme_error_handlers;
    struct list_head devices;
    struct device *parent;
    void *driver_priv;
    struct list_head bus_list;
    struct vme_irq irq[7];
    struct mutex irq_mtx;
    int (*slave_get)(struct vme_slave_resource *, int *, long long unsigned int *, long long unsigned int *, dma_addr_t *, u32 *, u32 *);
    int (*slave_set)(struct vme_slave_resource *, int, long long unsigned int, long long unsigned int, dma_addr_t, u32, u32);
    int (*master_get)(struct vme_master_resource *, int *, long long unsigned int *, long long unsigned int *, u32 *, u32 *, u32 *);
    int (*master_set)(struct vme_master_resource *, int, long long unsigned int, long long unsigned int, u32, u32, u32);
    ssize_t (*master_read)(struct vme_master_resource *, void *, size_t, loff_t);
    ssize_t (*master_write)(struct vme_master_resource *, void *, size_t, loff_t);
    unsigned int (*master_rmw)(struct vme_master_resource *, unsigned int, unsigned int, unsigned int, loff_t);
    int (*dma_list_add)(struct vme_dma_list *, struct vme_dma_attr *, struct vme_dma_attr *, size_t);
    int (*dma_list_exec)(struct vme_dma_list *);
    int (*dma_list_empty)(struct vme_dma_list *);
    void (*irq_set)(struct vme_bridge *, int, int, int);
    int (*irq_generate)(struct vme_bridge *, int, int);
    int (*lm_set)(struct vme_lm_resource *, long long unsigned int, u32, u32);
    int (*lm_get)(struct vme_lm_resource *, long long unsigned int *, u32 *, u32 *);
    int (*lm_attach)(struct vme_lm_resource *, int, void(*)(void *), void *);
    int (*lm_detach)(struct vme_lm_resource *, int);
    int (*slot_get)(struct vme_bridge *);
    void * (*alloc_consistent)(struct device *, size_t, dma_addr_t *);
    void (*free_consistent)(struct device *, size_t, void *, dma_addr_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct vme_bridge {
    char name[16];
    int num;
    struct list_head master_resources;
    struct list_head slave_resources;
    struct list_head dma_resources;
    struct list_head lm_resources;
    struct list_head vme_error_handlers;
    struct list_head devices;
    struct device *parent;
    void *driver_priv;
    struct list_head bus_list;
    struct vme_irq irq[7];
    struct mutex irq_mtx;
    int (*slave_get)(struct vme_slave_resource *, int *, long long unsigned int *, long long unsigned int *, dma_addr_t *, u32 *, u32 *);
    int (*slave_set)(struct vme_slave_resource *, int, long long unsigned int, long long unsigned int, dma_addr_t, u32, u32);
    int (*master_get)(struct vme_master_resource *, int *, long long unsigned int *, long long unsigned int *, u32 *, u32 *, u32 *);
    int (*master_set)(struct vme_master_resource *, int, long long unsigned int, long long unsigned int, u32, u32, u32);
    ssize_t (*master_read)(struct vme_master_resource *, void *, size_t, loff_t);
    ssize_t (*master_write)(struct vme_master_resource *, void *, size_t, loff_t);
    unsigned int (*master_rmw)(struct vme_master_resource *, unsigned int, unsigned int, unsigned int, loff_t);
    int (*dma_list_add)(struct vme_dma_list *, struct vme_dma_attr *, struct vme_dma_attr *, size_t);
    int (*dma_list_exec)(struct vme_dma_list *);
    int (*dma_list_empty)(struct vme_dma_list *);
    void (*irq_set)(struct vme_bridge *, int, int, int);
    int (*irq_generate)(struct vme_bridge *, int, int);
    int (*lm_set)(struct vme_lm_resource *, long long unsigned int, u32, u32);
    int (*lm_get)(struct vme_lm_resource *, long long unsigned int *, u32 *, u32 *);
    int (*lm_attach)(struct vme_lm_resource *, int, void(*)(void *), void *);
    int (*lm_detach)(struct vme_lm_resource *, int);
    int (*slot_get)(struct vme_bridge *);
    void * (*alloc_consistent)(struct device *, size_t, dma_addr_t *);
    void (*free_consistent)(struct device *, size_t, void *, dma_addr_t);
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
struct vme_bridge {
    char name[16];
    int num;
    struct list_head master_resources;
    struct list_head slave_resources;
    struct list_head dma_resources;
    struct list_head lm_resources;
    struct list_head vme_error_handlers;
    struct list_head devices;
    struct device *parent;
    void *driver_priv;
    struct list_head bus_list;
    struct vme_irq irq[7];
    struct mutex irq_mtx;
    int (*slave_get)(struct vme_slave_resource *, int *, long long unsigned int *, long long unsigned int *, dma_addr_t *, u32 *, u32 *);
    int (*slave_set)(struct vme_slave_resource *, int, long long unsigned int, long long unsigned int, dma_addr_t, u32, u32);
    int (*master_get)(struct vme_master_resource *, int *, long long unsigned int *, long long unsigned int *, u32 *, u32 *, u32 *);
    int (*master_set)(struct vme_master_resource *, int, long long unsigned int, long long unsigned int, u32, u32, u32);
    ssize_t (*master_read)(struct vme_master_resource *, void *, size_t, loff_t);
    ssize_t (*master_write)(struct vme_master_resource *, void *, size_t, loff_t);
    unsigned int (*master_rmw)(struct vme_master_resource *, unsigned int, unsigned int, unsigned int, loff_t);
    int (*dma_list_add)(struct vme_dma_list *, struct vme_dma_attr *, struct vme_dma_attr *, size_t);
    int (*dma_list_exec)(struct vme_dma_list *);
    int (*dma_list_empty)(struct vme_dma_list *);
    void (*irq_set)(struct vme_bridge *, int, int, int);
    int (*irq_generate)(struct vme_bridge *, int, int);
    int (*lm_set)(struct vme_lm_resource *, long long unsigned int, u32, u32);
    int (*lm_get)(struct vme_lm_resource *, long long unsigned int *, u32 *, u32 *);
    int (*lm_attach)(struct vme_lm_resource *, int, void(*)(void *), void *);
    int (*lm_detach)(struct vme_lm_resource *, int);
    int (*slot_get)(struct vme_bridge *);
    void * (*alloc_consistent)(struct device *, size_t, dma_addr_t *);
    void (*free_consistent)(struct device *, size_t, void *, dma_addr_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct vme_bridge {
    char name[16];
    int num;
    struct list_head master_resources;
    struct list_head slave_resources;
    struct list_head dma_resources;
    struct list_head lm_resources;
    struct list_head vme_error_handlers;
    struct list_head devices;
    struct device *parent;
    void *driver_priv;
    struct list_head bus_list;
    struct vme_irq irq[7];
    struct mutex irq_mtx;
    int (*slave_get)(struct vme_slave_resource *, int *, long long unsigned int *, long long unsigned int *, dma_addr_t *, u32 *, u32 *);
    int (*slave_set)(struct vme_slave_resource *, int, long long unsigned int, long long unsigned int, dma_addr_t, u32, u32);
    int (*master_get)(struct vme_master_resource *, int *, long long unsigned int *, long long unsigned int *, u32 *, u32 *, u32 *);
    int (*master_set)(struct vme_master_resource *, int, long long unsigned int, long long unsigned int, u32, u32, u32);
    ssize_t (*master_read)(struct vme_master_resource *, void *, size_t, loff_t);
    ssize_t (*master_write)(struct vme_master_resource *, void *, size_t, loff_t);
    unsigned int (*master_rmw)(struct vme_master_resource *, unsigned int, unsigned int, unsigned int, loff_t);
    int (*dma_list_add)(struct vme_dma_list *, struct vme_dma_attr *, struct vme_dma_attr *, size_t);
    int (*dma_list_exec)(struct vme_dma_list *);
    int (*dma_list_empty)(struct vme_dma_list *);
    void (*irq_set)(struct vme_bridge *, int, int, int);
    int (*irq_generate)(struct vme_bridge *, int, int);
    int (*lm_set)(struct vme_lm_resource *, long long unsigned int, u32, u32);
    int (*lm_get)(struct vme_lm_resource *, long long unsigned int *, u32 *, u32 *);
    int (*lm_attach)(struct vme_lm_resource *, int, void(*)(void *), void *);
    int (*lm_detach)(struct vme_lm_resource *, int);
    int (*slot_get)(struct vme_bridge *);
    void * (*alloc_consistent)(struct device *, size_t, dma_addr_t *);
    void (*free_consistent)(struct device *, size_t, void *, dma_addr_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct vme_bridge {
    char name[16];
    int num;
    struct list_head master_resources;
    struct list_head slave_resources;
    struct list_head dma_resources;
    struct list_head lm_resources;
    struct list_head vme_error_handlers;
    struct list_head devices;
    struct device *parent;
    void *driver_priv;
    struct list_head bus_list;
    struct vme_irq irq[7];
    struct mutex irq_mtx;
    int (*slave_get)(struct vme_slave_resource *, int *, long long unsigned int *, long long unsigned int *, dma_addr_t *, u32 *, u32 *);
    int (*slave_set)(struct vme_slave_resource *, int, long long unsigned int, long long unsigned int, dma_addr_t, u32, u32);
    int (*master_get)(struct vme_master_resource *, int *, long long unsigned int *, long long unsigned int *, u32 *, u32 *, u32 *);
    int (*master_set)(struct vme_master_resource *, int, long long unsigned int, long long unsigned int, u32, u32, u32);
    ssize_t (*master_read)(struct vme_master_resource *, void *, size_t, loff_t);
    ssize_t (*master_write)(struct vme_master_resource *, void *, size_t, loff_t);
    unsigned int (*master_rmw)(struct vme_master_resource *, unsigned int, unsigned int, unsigned int, loff_t);
    int (*dma_list_add)(struct vme_dma_list *, struct vme_dma_attr *, struct vme_dma_attr *, size_t);
    int (*dma_list_exec)(struct vme_dma_list *);
    int (*dma_list_empty)(struct vme_dma_list *);
    void (*irq_set)(struct vme_bridge *, int, int, int);
    int (*irq_generate)(struct vme_bridge *, int, int);
    int (*lm_set)(struct vme_lm_resource *, long long unsigned int, u32, u32);
    int (*lm_get)(struct vme_lm_resource *, long long unsigned int *, u32 *, u32 *);
    int (*lm_attach)(struct vme_lm_resource *, int, void(*)(void *), void *);
    int (*lm_detach)(struct vme_lm_resource *, int);
    int (*slot_get)(struct vme_bridge *);
    void * (*alloc_consistent)(struct device *, size_t, dma_addr_t *);
    void (*free_consistent)(struct device *, size_t, void *, dma_addr_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct vme_bridge {
    char name[16];
    int num;
    struct list_head master_resources;
    struct list_head slave_resources;
    struct list_head dma_resources;
    struct list_head lm_resources;
    struct list_head vme_error_handlers;
    struct list_head devices;
    struct device *parent;
    void *driver_priv;
    struct list_head bus_list;
    struct vme_irq irq[7];
    struct mutex irq_mtx;
    int (*slave_get)(struct vme_slave_resource *, int *, long long unsigned int *, long long unsigned int *, dma_addr_t *, u32 *, u32 *);
    int (*slave_set)(struct vme_slave_resource *, int, long long unsigned int, long long unsigned int, dma_addr_t, u32, u32);
    int (*master_get)(struct vme_master_resource *, int *, long long unsigned int *, long long unsigned int *, u32 *, u32 *, u32 *);
    int (*master_set)(struct vme_master_resource *, int, long long unsigned int, long long unsigned int, u32, u32, u32);
    ssize_t (*master_read)(struct vme_master_resource *, void *, size_t, loff_t);
    ssize_t (*master_write)(struct vme_master_resource *, void *, size_t, loff_t);
    unsigned int (*master_rmw)(struct vme_master_resource *, unsigned int, unsigned int, unsigned int, loff_t);
    int (*dma_list_add)(struct vme_dma_list *, struct vme_dma_attr *, struct vme_dma_attr *, size_t);
    int (*dma_list_exec)(struct vme_dma_list *);
    int (*dma_list_empty)(struct vme_dma_list *);
    void (*irq_set)(struct vme_bridge *, int, int, int);
    int (*irq_generate)(struct vme_bridge *, int, int);
    int (*lm_set)(struct vme_lm_resource *, long long unsigned int, u32, u32);
    int (*lm_get)(struct vme_lm_resource *, long long unsigned int *, u32 *, u32 *);
    int (*lm_attach)(struct vme_lm_resource *, int, void(*)(void *), void *);
    int (*lm_detach)(struct vme_lm_resource *, int);
    int (*slot_get)(struct vme_bridge *);
    void * (*alloc_consistent)(struct device *, size_t, dma_addr_t *);
    void (*free_consistent)(struct device *, size_t, void *, dma_addr_t);
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
struct vme_bridge {
    char name[16];
    int num;
    struct list_head master_resources;
    struct list_head slave_resources;
    struct list_head dma_resources;
    struct list_head lm_resources;
    struct list_head vme_error_handlers;
    struct list_head devices;
    struct device *parent;
    void *driver_priv;
    struct list_head bus_list;
    struct vme_irq irq[7];
    struct mutex irq_mtx;
    int (*slave_get)(struct vme_slave_resource *, int *, long long unsigned int *, long long unsigned int *, dma_addr_t *, u32 *, u32 *);
    int (*slave_set)(struct vme_slave_resource *, int, long long unsigned int, long long unsigned int, dma_addr_t, u32, u32);
    int (*master_get)(struct vme_master_resource *, int *, long long unsigned int *, long long unsigned int *, u32 *, u32 *, u32 *);
    int (*master_set)(struct vme_master_resource *, int, long long unsigned int, long long unsigned int, u32, u32, u32);
    ssize_t (*master_read)(struct vme_master_resource *, void *, size_t, loff_t);
    ssize_t (*master_write)(struct vme_master_resource *, void *, size_t, loff_t);
    unsigned int (*master_rmw)(struct vme_master_resource *, unsigned int, unsigned int, unsigned int, loff_t);
    int (*dma_list_add)(struct vme_dma_list *, struct vme_dma_attr *, struct vme_dma_attr *, size_t);
    int (*dma_list_exec)(struct vme_dma_list *);
    int (*dma_list_empty)(struct vme_dma_list *);
    void (*irq_set)(struct vme_bridge *, int, int, int);
    int (*irq_generate)(struct vme_bridge *, int, int);
    int (*lm_set)(struct vme_lm_resource *, long long unsigned int, u32, u32);
    int (*lm_get)(struct vme_lm_resource *, long long unsigned int *, u32 *, u32 *);
    int (*lm_attach)(struct vme_lm_resource *, int, void(*)(void *), void *);
    int (*lm_detach)(struct vme_lm_resource *, int);
    int (*slot_get)(struct vme_bridge *);
    void * (*alloc_consistent)(struct device *, size_t, dma_addr_t *);
    void (*free_consistent)(struct device *, size_t, void *, dma_addr_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct vme_bridge {
    char name[16];
    int num;
    struct list_head master_resources;
    struct list_head slave_resources;
    struct list_head dma_resources;
    struct list_head lm_resources;
    struct list_head vme_error_handlers;
    struct list_head devices;
    struct device *parent;
    void *driver_priv;
    struct list_head bus_list;
    struct vme_irq irq[7];
    struct mutex irq_mtx;
    int (*slave_get)(struct vme_slave_resource *, int *, long long unsigned int *, long long unsigned int *, dma_addr_t *, u32 *, u32 *);
    int (*slave_set)(struct vme_slave_resource *, int, long long unsigned int, long long unsigned int, dma_addr_t, u32, u32);
    int (*master_get)(struct vme_master_resource *, int *, long long unsigned int *, long long unsigned int *, u32 *, u32 *, u32 *);
    int (*master_set)(struct vme_master_resource *, int, long long unsigned int, long long unsigned int, u32, u32, u32);
    ssize_t (*master_read)(struct vme_master_resource *, void *, size_t, loff_t);
    ssize_t (*master_write)(struct vme_master_resource *, void *, size_t, loff_t);
    unsigned int (*master_rmw)(struct vme_master_resource *, unsigned int, unsigned int, unsigned int, loff_t);
    int (*dma_list_add)(struct vme_dma_list *, struct vme_dma_attr *, struct vme_dma_attr *, size_t);
    int (*dma_list_exec)(struct vme_dma_list *);
    int (*dma_list_empty)(struct vme_dma_list *);
    void (*irq_set)(struct vme_bridge *, int, int, int);
    int (*irq_generate)(struct vme_bridge *, int, int);
    int (*lm_set)(struct vme_lm_resource *, long long unsigned int, u32, u32);
    int (*lm_get)(struct vme_lm_resource *, long long unsigned int *, u32 *, u32 *);
    int (*lm_attach)(struct vme_lm_resource *, int, void(*)(void *), void *);
    int (*lm_detach)(struct vme_lm_resource *, int);
    int (*slot_get)(struct vme_bridge *);
    void * (*alloc_consistent)(struct device *, size_t, dma_addr_t *);
    void (*free_consistent)(struct device *, size_t, void *, dma_addr_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct vme_bridge {
    char name[16];
    int num;
    struct list_head master_resources;
    struct list_head slave_resources;
    struct list_head dma_resources;
    struct list_head lm_resources;
    struct list_head vme_error_handlers;
    struct list_head devices;
    struct device *parent;
    void *driver_priv;
    struct list_head bus_list;
    struct vme_irq irq[7];
    struct mutex irq_mtx;
    int (*slave_get)(struct vme_slave_resource *, int *, long long unsigned int *, long long unsigned int *, dma_addr_t *, u32 *, u32 *);
    int (*slave_set)(struct vme_slave_resource *, int, long long unsigned int, long long unsigned int, dma_addr_t, u32, u32);
    int (*master_get)(struct vme_master_resource *, int *, long long unsigned int *, long long unsigned int *, u32 *, u32 *, u32 *);
    int (*master_set)(struct vme_master_resource *, int, long long unsigned int, long long unsigned int, u32, u32, u32);
    ssize_t (*master_read)(struct vme_master_resource *, void *, size_t, loff_t);
    ssize_t (*master_write)(struct vme_master_resource *, void *, size_t, loff_t);
    unsigned int (*master_rmw)(struct vme_master_resource *, unsigned int, unsigned int, unsigned int, loff_t);
    int (*dma_list_add)(struct vme_dma_list *, struct vme_dma_attr *, struct vme_dma_attr *, size_t);
    int (*dma_list_exec)(struct vme_dma_list *);
    int (*dma_list_empty)(struct vme_dma_list *);
    void (*irq_set)(struct vme_bridge *, int, int, int);
    int (*irq_generate)(struct vme_bridge *, int, int);
    int (*lm_set)(struct vme_lm_resource *, long long unsigned int, u32, u32);
    int (*lm_get)(struct vme_lm_resource *, long long unsigned int *, u32 *, u32 *);
    int (*lm_attach)(struct vme_lm_resource *, int, void(*)(void *), void *);
    int (*lm_detach)(struct vme_lm_resource *, int);
    int (*slot_get)(struct vme_bridge *);
    void * (*alloc_consistent)(struct device *, size_t, dma_addr_t *);
    void (*free_consistent)(struct device *, size_t, void *, dma_addr_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct vme_bridge {
    char name[16];
    int num;
    struct list_head master_resources;
    struct list_head slave_resources;
    struct list_head dma_resources;
    struct list_head lm_resources;
    struct list_head vme_error_handlers;
    struct list_head devices;
    struct device *parent;
    void *driver_priv;
    struct list_head bus_list;
    struct vme_irq irq[7];
    struct mutex irq_mtx;
    int (*slave_get)(struct vme_slave_resource *, int *, long long unsigned int *, long long unsigned int *, dma_addr_t *, u32 *, u32 *);
    int (*slave_set)(struct vme_slave_resource *, int, long long unsigned int, long long unsigned int, dma_addr_t, u32, u32);
    int (*master_get)(struct vme_master_resource *, int *, long long unsigned int *, long long unsigned int *, u32 *, u32 *, u32 *);
    int (*master_set)(struct vme_master_resource *, int, long long unsigned int, long long unsigned int, u32, u32, u32);
    ssize_t (*master_read)(struct vme_master_resource *, void *, size_t, loff_t);
    ssize_t (*master_write)(struct vme_master_resource *, void *, size_t, loff_t);
    unsigned int (*master_rmw)(struct vme_master_resource *, unsigned int, unsigned int, unsigned int, loff_t);
    int (*dma_list_add)(struct vme_dma_list *, struct vme_dma_attr *, struct vme_dma_attr *, size_t);
    int (*dma_list_exec)(struct vme_dma_list *);
    int (*dma_list_empty)(struct vme_dma_list *);
    void (*irq_set)(struct vme_bridge *, int, int, int);
    int (*irq_generate)(struct vme_bridge *, int, int);
    int (*lm_set)(struct vme_lm_resource *, long long unsigned int, u32, u32);
    int (*lm_get)(struct vme_lm_resource *, long long unsigned int *, u32 *, u32 *);
    int (*lm_attach)(struct vme_lm_resource *, int, void(*)(void *), void *);
    int (*lm_detach)(struct vme_lm_resource *, int);
    int (*slot_get)(struct vme_bridge *);
    void * (*alloc_consistent)(struct device *, size_t, dma_addr_t *);
    void (*free_consistent)(struct device *, size_t, void *, dma_addr_t);
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
<b>Field type changed. </b>
<code>int (*lm_attach)(struct vme_lm_resource *, int, void(*)(int))</code> ➡️ <code>int (*lm_attach)(struct vme_lm_resource *, int, void(*)(void *), void *)</code>
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
